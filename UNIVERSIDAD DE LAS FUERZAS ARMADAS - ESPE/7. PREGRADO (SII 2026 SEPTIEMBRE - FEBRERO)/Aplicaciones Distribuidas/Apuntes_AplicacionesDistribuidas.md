# Unidad I

## Conceptos básicos de las aplicaciones distribuidas.
### ¿Qué es una aplicación distribuida?

Una **aplicación distribuida** es un sistema compuesto por varios componentes que se ejecutan en **diferentes computadores o nodos**, pero trabajan juntos mediante una red para ofrecer un servicio al usuario.

Los componentes pueden comunicarse, compartir información y coordinarse como si formaran un solo sistema.

**Ejemplo:** una aplicación web puede tener un servidor para la aplicación, otro para la base de datos y otro para almacenar archivos.

---

### Principales ventajas

- **Escalabilidad:** permite agregar más recursos o nodos cuando aumenta la demanda.
- **Disponibilidad:** si un nodo falla, otros pueden continuar proporcionando el servicio.
- **Compartición de recursos:** varios componentes pueden utilizar recursos distribuidos.
- **Rendimiento:** las tareas pueden repartirse entre diferentes nodos.
- **Flexibilidad:** los componentes pueden actualizarse o modificarse de manera independiente.

---

### Principales desafíos

- **Comunicación:** los nodos dependen de una red que puede tener retrasos o fallas.
- **Fallos parciales:** un componente puede fallar mientras los demás continúan funcionando.
- **Consistencia:** mantener la información sincronizada entre diferentes nodos puede ser complicado.
- **Seguridad:** existen más puntos de comunicación que deben protegerse.
- **Coordinación:** los nodos deben ponerse de acuerdo para realizar determinadas operaciones.
- **Complejidad:** administrar varios componentes es más complejo que administrar un único sistema.

---

## Falacias de las aplicaciones distribuidas

Las **falacias de la computación distribuida** son suposiciones incorrectas que los desarrolladores suelen hacer al diseñar sistemas distribuidos.

Las principales son:

1. **La red es confiable.**  
    → Una red puede fallar, perder paquetes o desconectar nodos.
2. **La latencia es cero.**  
    → La comunicación por red siempre tiene cierto tiempo de respuesta.
3. **El ancho de banda es infinito.**  
    → La capacidad de la red es limitada.
4. **La red es segura.**  
    → Los datos pueden ser interceptados, modificados o atacados.
5. **La topología no cambia.**  
    → Los nodos y conexiones de una red pueden cambiar.
6. **Existe un solo administrador.**  
    → Un sistema distribuido puede involucrar diferentes administradores, servicios o equipos.
7. **El costo de transporte es cero.**  
    → Comunicarse entre nodos consume recursos y tiempo.
8. **La red es homogénea.**  
    → Los nodos pueden utilizar diferentes sistemas operativos, tecnologías, hardware o protocolos.

**Idea clave:** las falacias representan cosas que **parecen ciertas cuando trabajamos con un sistema local**, pero dejan de serlo cuando interviene una red.

---

## Teorema CAP

El **teorema CAP** establece que un sistema distribuido, ante una **partición de red**, no puede garantizar simultáneamente las tres propiedades:

- **C — Consistencia (Consistency)**
- **A — Disponibilidad (Availability)**
- **P — Tolerancia a particiones (Partition Tolerance)**

### C — Consistencia

Todos los nodos deben proporcionar **la misma información en un momento determinado**.

**Ejemplo:** si un usuario actualiza su saldo, cualquier nodo que consulte ese saldo debe obtener el mismo valor.

### A — Disponibilidad

Cada solicitud recibida debe obtener una **respuesta**, aunque algún componente del sistema esté fallando.

**Ejemplo:** aunque un nodo esté caído, otro nodo puede responder la solicitud.

### P — Tolerancia a particiones

El sistema debe continuar funcionando aunque exista una **interrupción de comunicación entre algunos nodos**.

**Ejemplo:** dos servidores dejan de poder comunicarse entre sí, pero ambos siguen funcionando.

---

### ¿Por qué no se pueden tener las 3 CAP?

Aquí hay una pequeña precisión importante: **CAP no dice que un sistema distribuido nunca pueda tener C, A y P simultáneamente en condiciones normales.** El punto es que **cuando ocurre una partición de red (P), no puede garantizar al mismo tiempo C y A**.

Imagina dos nodos:

```
Nodo A  ←──X──→  Nodo B
          ↓
     Partición de red
```

Los nodos ya no pueden comunicarse.

Si el sistema quiere mantener **Consistencia (C)**, puede decidir **no aceptar algunas operaciones** hasta recuperar la comunicación.

→ Mantiene **C + P**, pero sacrifica **A**.

Si el sistema quiere mantener **Disponibilidad (A)**, puede permitir que ambos nodos sigan respondiendo aunque tengan información diferente temporalmente.

→ Mantiene **A + P**, pero sacrifica **C**.

Por eso:

> **Ante una partición de red, un sistema distribuido debe elegir entre Consistencia y Disponibilidad.**

### Resumen rápido

| Propiedad              | Significa                                              |
| ---------------------- | ------------------------------------------------------ |
| **C — Consistencia**   | Todos ven los mismos datos.                            |
| **A — Disponibilidad** | El sistema siempre responde.                           |
| **P — Partición**      | El sistema soporta fallos de comunicación entre nodos. |

**CAP → Cuando hay una Partición (P), eliges entre Consistencia (C) o Disponibilidad (A).**

### C + P — Consistencia + Tolerancia a particiones

**Ejemplo:** un sistema bancario.

Supongamos que hay dos servidores:

```
Servidor A ──X── Servidor B
              ↑
        Se rompe la red
```

Un usuario intenta retirar **$100** desde el servidor A.

Como A no puede comunicarse con B, el sistema **rechaza o bloquea la operación** para evitar que B tenga información diferente.

- **C:** evita inconsistencias.
- **P:** sigue funcionando correctamente ante la partición.
- ❌ **A:** algunas operaciones no están disponibles durante el problema.

**Idea:** _"Prefiero no responder antes que entregar información incorrecta."_

---

### A + P — Disponibilidad + Tolerancia a particiones

**Ejemplo:** una red social.

Supongamos que dos servidores pierden comunicación:

```
Servidor A ──X── Servidor B
```

Un usuario publica algo desde A. B todavía no conoce esa publicación, pero **ambos servidores continúan respondiendo solicitudes**.

Cuando vuelve la comunicación, los datos pueden sincronizarse.

- **A:** los servidores continúan respondiendo.
-  **P:** el sistema tolera la separación.
- ❌ **C:** temporalmente pueden existir datos diferentes entre los nodos.

**Idea:** _"Prefiero responder aunque la información pueda tardar en sincronizarse."_

----
## Framework vs. Librería

### ¿Qué es una librería?

Una **librería** es un conjunto de código reutilizable que proporciona funciones para resolver problemas específicos.

El **programador decide cuándo y cómo utilizarla**.

**Ejemplo:** una librería para trabajar con fechas proporciona funciones para calcular, comparar o formatear fechas.
### ¿Qué es un framework?

Un **framework** es una estructura que proporciona una base para desarrollar una aplicación.

En un framework, el programa sigue ciertas reglas y el framework puede encargarse del flujo principal de ejecución.

### Diferencia principal

| Librería                                     | Framework                                                |
| -------------------------------------------- | -------------------------------------------------------- |
| Tú controlas el flujo.                       | El framework controla gran parte del flujo.              |
| Utilizas sus funciones cuando las necesitas. | Proporciona una estructura para construir la aplicación. |
| Mayor libertad de organización.              | Establece reglas y estructura.                           |
**Ejemplos de frameworks:**
•  Angular (para interfaces web)
• Django (para desarrollo backend con Python)
• Laravel (para desarrollo web con PHP)

---

## Lenguaje y tecnología
### ¿Qué es un lenguaje?
Un **lenguaje de programación** es un lenguaje formal utilizado para escribir instrucciones que una computadora puede ejecutar.

**Ejemplos:** Java, Python, JavaScript, C++.

### ¿Qué es una tecnología?

Una **tecnología** es una herramienta, plataforma, sistema, técnica o conjunto de herramientas utilizadas para resolver un problema o desarrollar una solución.
Puede incluir **lenguajes, frameworks, librerías, protocolos, bases de datos, servidores, etc.**

### Diferencia

> **Lenguaje:** permite expresar las instrucciones del programa.  
> **Tecnología:** engloba herramientas y soluciones utilizadas para construir el sistema.

---
## Concurrencia
### ¿Qué es concurrencia?

La **concurrencia** es la capacidad de un sistema para **gestionar varias tareas que avanzan durante el mismo período de tiempo**, pudiendo alternar entre ellas o ejecutarlas simultáneamente.

**Ejemplo:**

Una aplicación puede:

```
Descargar archivo
Procesar datos
Responder al usuario
```

sin tener que terminar completamente una tarea antes de comenzar a trabajar con otra.

**Concurrencia ≠ paralelismo**

- **Concurrencia:** varias tareas progresan de forma intercalada.
- **Paralelismo:** varias tareas se ejecutan realmente al mismo tiempo, normalmente usando varios núcleos.

---

### Concurrencia en sistemas distribuidos

En un **sistema distribuido**, la concurrencia ocurre cuando **varios procesos o componentes ubicados en diferentes nodos ejecutan operaciones al mismo tiempo o de forma independiente**.

Ejemplo:

```
        Sistema distribuido

Servidor A → procesa pedido 1
Servidor B → procesa pedido 2
Servidor C → procesa pedido 3
```

Los diferentes nodos pueden trabajar simultáneamente y necesitan **coordinarse** cuando acceden o modifican recursos compartidos.

### Diferencia

**Concurrencia tradicional:**
Varias tareas pueden ejecutarse dentro de un mismo sistema o computador.

**Concurrencia distribuida:**
Varias tareas pueden ejecutarse en diferentes computadores o nodos y necesitan comunicarse y coordinarse mediante una red.

---
## Hilos

### ¿Qué es un hilo?

Un **hilo** es una unidad de ejecución dentro de un proceso.

Un proceso puede tener **varios hilos**, que comparten recursos del proceso pero pueden ejecutar diferentes tareas.

**Ejemplo:**

```
Aplicación
│
├── Hilo 1 → interfaz
├── Hilo 2 → descarga
└── Hilo 3 → procesamiento
```

Los hilos permiten realizar varias tareas de forma concurrente dentro de una aplicación.

---

### Hilos en sistemas distribuidos

En un sistema distribuido, los hilos pueden utilizarse dentro de los diferentes nodos para **atender múltiples solicitudes o ejecutar varias tareas concurrentemente**.

Ejemplo:

```
Servidor
│
├── Hilo 1 → Cliente A
├── Hilo 2 → Cliente B
├── Hilo 3 → Cliente C
└── Hilo 4 → Cliente D
```

Cada servidor puede tener sus propios hilos, mientras que los servidores se comunican mediante la red.

### Diferencia importante

**Hilos normales:**

Ejecutan tareas concurrentes dentro de un mismo computador/proceso.

**Hilos en sistemas distribuidos:**

Ejecutan tareas concurrentes en los diferentes nodos del sistema, que además deben comunicarse mediante la red.

---
## Sockets

### ¿Qué es un socket?

Un **socket** es un mecanismo que permite que **dos procesos se comuniquen a través de una red**.

Puede entenderse como un **punto de comunicación** entre aplicaciones.

Normalmente se identifica mediante:

```
Dirección IP + Puerto
```

Por ejemplo:

```
192.168.1.10:8080
```

- `192.168.1.10` → dirección del equipo.
- `8080` → puerto donde escucha la aplicación.

### ¿Cómo funcionan?

```
Cliente                         Servidor
   │                               │
   │────── conexión ──────────────→│
   │                               │
   │────── solicitud ─────────────→│
   │                               │
   │←───── respuesta ──────────────│
   │                               │
```

El **servidor** espera conexiones y el **cliente** inicia la comunicación.

### Tipos comunes

- **TCP:** comunicación orientada a conexión, confiable y ordenada.
- **UDP:** comunicación más rápida y ligera, pero no garantiza entrega ni orden.

### Idea clave

> **Un socket es un punto de comunicación que permite a dos procesos intercambiar datos a través de una red.**




-----------
Nodo.- Punto dentro de la conexión (se interconecta mediante aristas). No siempre va a ser un computador, pero tendrá al menos 1 procesador para  que pueda procesar.

Hacker.- Sombrero blanco (genera productos sw que no tengan vulnerabilidades), negro, gris, rojo (busca vulnerabilidades y las corrige)

	Cracker.- Modificar sistemas ya lanzados.

Docker vs Sistema Operativos

Falacias.- 
La red es confiable, latencia es 0, el ancho de banda es infinito, la red es segura, la topología no cambia, hay un solo administrador.


http Permite ver que información transita por la red
y https q hacen meaing,www (red global), wwwc (red ..?? compañias que pertenecen a la standar de la red. Permite trabajar a todos en la web de la misma manera)

Semántica en la web. 

xml
html

Framework vs libreria

La historia:

1969 ARPANET 1er mensaje
1978 Lamport relojes logicos
1984 RPC / NFS Birell-NElson; Sun
1989 World Wlde web CERN
1991 CORBA Objetos distribuidos
1999 P2P / SETI @ home napster: compute voluntario
2000 REST - CAP Fielding: brewer
2004 MapReduce  Google
2006 Nube pública AWS 3 EC2
2009 Bitcoin BLockchain
2011 WebSocket RFC6455
2014 Kubernets contenedores orquestados
2024 Lavarel Reverb WebSOckets nativos php
2026 IA en la nube K8s


CAP
Cuando ocurre una particion de red (P), es decir, cuando parte de los nodos no puede comunicarse con el resto, el sistema debe elegir entre C (responder solo con datos correctos, aunq rechace peticiones) y dispoinibilidad (a: responder siempre, aunque con datos posiblemente desactualizados). Como las particiones son inevtiables en una red real, la decision practica es q hacer cuando ocurren. CAP es un piunto de partida util pero simplificado; el diseño real exige analizar cada operación.

porque no se pueden tener los 3 a la vez?


ventajas 
Esalabilidad
Disponibilidad
REndimiento
COmpartir recursos
Cercania geografica
Independencia ecnologica y de equipos


desventajas
COmplejidad
Fallos parciales
Latencia de red
COnsistencia
seguridad
prueba y depuracion


-----
diferencias 

framework vs librerias
lenguaje vs tecnologias
concurrencia vs concurrencia en distribuida
hilos vs hilos en sistemas distribuidos
socket


----------















