
Promotor: el que tiene la iniciativa de hacer algo.

# INTRODUCCIÓN - UNIDAD 1.
## **Síntomas y razones de una ingeniería de requerimientos IR inapropiada.

**Causas de proyectos fallidos:** 
- Problemas técnicos 8.7 %
- Falta de recursos 10.6 %
- Falta de gestión de ti 8.7 %
- El producto queda obsoleto 7.5 %
- Ausencia de apoyo de la dirección 8.7%
- Ausencia de planificación 8.1%
- Causas de proyectos fallidos 44.1 % asociadas a IR
- Requisitos no realistas 9.9%
- Cambios en requisitos 8.7%
- Requisitos incompletos 13.1%
- Falta de implicación de los usuarios 12.4%

---------
**Análisis de requisitos: problemas típicos**

Desafíos para el análisis de requisitos:
- Diferentes y usos de lenguajes (no de programación). 
- Objetivos inciertos.
- Requisitos en constante cambio.
- Requisitos de poca calidad.
- Atributos innecesarios.
- Alta complejidad.
- Planificación poco precisa.

---------
**Requisitos de poca calidad**
- **Requisitos faltantes**
	- Porque es "obvio" (requisitos implícitos).
	- Porque se debe hacer de inmediato.
	- Porque no se han usado todas las fuentes de información.
- **Requisitos incorrectos:**
	- Porque se han utilizado fuentes de información incorrectos/equivocadas.
- **Contradicciones.**
Las contradicciones se producen cuando dos o mas requisitos se  excluyen mutuamente o presentan afirmaciones incompatibles. Esto genera:
1. Ambigüedad.
2. Conflictos en el diseño y desarrollo.
3. Imposibilidad de verificación y validación.
4. Perdida de confianza en el documento de requisitos.

- **Redundancias.**
Las redundancias son repeticiones innecesarias de requisitos ya sea de forma literal o con ligeras variaciones. Aunque parecen inofensivas, generan:
1. Sobrecarga cognitiva. Ejemplo: repetir "El sistema debe registrar el acceso del usuario" en varias secciones sin aportar detalles nuevos.
2. Riesgo de inconsistencias futuras.
3. Dificultad en trazabilidad (relacion de un requi con otro).
4. Desgaste en la validación.

------
Requisitos de poca calidad
**Ambiguos**
conducen a múltiples interpretaciones
**Diferentes enfoques**
Distintas características culturales y de formacion (background) conducen a interpretaciones distintas.

Requisitos completos y de alta calidad son la base del éxito de un proyecto
Los requisitos faltantes deben ser detectados en forma temprana.
A través de la IR se identifican los riesgos y pueden ser tratados de forma temprana.

-------
ATRIBUTOS DE CALIDAD         contradicciones (C)  redundancuas (r)
CLARIDAD CR
CONSISTENCIA CR
TRAZABILIDAD CR
VERIFICABILIDAD CR
MANTENIBILIDAD CR

-----
## Definición de requerimiento y requisito.
## ¿Qué son los requerimientos?
Acción y efecto de requerir (RAE): 
D1: Necesitar una persona o una cosa que se le dedique algo.
D2: Pedir alguna cosa a una persona.
D3: Decir a una autoridad, a una persona que debe hacer algo.

## ¿Qué son los requisitos?
Requisito (1-IEEE): Condición necesaria para una cosa.

-a: Una condición o capacidad requerida por un usuario una persona o sistema para resolver un problema o como un medio para alcanzar un objetivo.
-b: Una condición o capacidad que debe cumplirse o estar presente en el sistema o subsistema para satisfacer un contrato estándar una especificación u otro documento formal.
-c: Una representación en forma de documento de una condicion o capacidad como las expresadas en (a) o en (b).

1968: IR
(2-DoD 1994): caracteristica del sistema que es una condicion para su aceptacion
3-DoD 1996? propiedad que un sistema deberia tener para lograr exito en el entorno en el que se usara

sin embargo a pesar de estar apararente simplicidad del concepto, es frecuente encontrar eletermino rquisito calificado con adjetivos que pueden resultar consusos en primer momento: de sistema, hw, sw, de user de cleinte , fun y no fun

---------
## IR ("REQUIEREMENTS ENGINEERING)
La IR es un enfoque sistemático y disciplinado para la especificación y gestion de equisitos con los siguientes objetivos:
1. Conocer los requisitos relevantes, asegurar un consenso entre todos los implicados acerca de estos, documentarlos de acuerdo a los estándares establecidos y gestionarlos automáticamente.
2. Entender y documentar los deseos y necesidades de los implicados, especificar y gestionar los requerimientos para minimizar el riesgo de poner en producción un sistema que no cumple con los deseos y necesidades de los stakeholders.

--------


## Clase 4
## **¿Por qué importan los requerimientos?**

La parte más dificil de construir un sistema es precisamente saber que construir. Ninguna otra parte del trabajo conceptual es tan dificil como establecer los requerimientos técnicos detallados, incluyendo todas las interfaces con gente, maquinas y otros sistemas. Ninguna otra parte del trabajo afecta tanto el sistema si es hecha mal. Ninguna es tan difícil de corregir mas adelante. Entonces, la tarea mas importante que el ing de sw hace para el cliente es la extracción iterativa y el refinamiento de los requerimientos del producto. Frederick P. Brooks [Brooks, 1987]

----------
Los requerimientos se deben descubrir antes de empezar a construir un producto software, y que puede ser algo que el producto software debe hacer o una *cualidad que el producto software debe tener.*

Un requerimiento existe ya sea porque el tipo de producto demanda ciertas funciones o cualidades, o porque el cliente quiere que ese requerimiento sea parte del producto final.

desarrollar mantenimiento obtener

Asi que si no se tienen los requerimientos correctos, no se puede diseñar o construir el producto correcto y consecuentemente el producto no permitirá a los usuarios finales a realizar su trabajo. Y essto esta confirmado por estudios que demuestran que mas del 60% de los errores de diseño se originan durante las etapas de requerimientos y análisis.

----------
## 5 actividades principales de la IR

ELICITAR ELICIT (3 personas, R. humanos (David. Dome. Jerson), R. materiales, Material: depreciación del equipo anual, depreciación del celular, rentabilidad de la nube. ) 
Actividades para recabar la información que nos permita entender las necesidades del usuario, utilizando diferentes técnicas...
Identificar, detallar y refinar las actividades de los usuarios.
->

-> ANALIZAR ANALYZE  
Procesos y actividades que permiten entender los tipos de requerimientos Identifica oportunidades para el software. Modelan el ambiente actuales y permite comunicarlo al requipo de desarrollo.
->

-> ESPECIFICAR SPECIFY 
- Establecer el entendimiento común de los requisitos.
- Definir la forma de documentar (lenguaje natural o modelado) adecuado para el proyecto
- Escribir los requisitos y el doc
-> 

-> VERIFICAR Y AJUSTAR VERIFY AND ADJUST 
- Asegurar la calidad en una fase temprana.
- Actividades para la aceptación, rechazo y retroalimentación de los requerimiento.

-> 
ADMINISTRAR MANAGE -> 
Estructurar y organizar los requerimientos, gestionar su disponibilidad, modificar los requerimientos de forma consistente e implementarlos en el proyecto.

(ciclo)

**Modelo en Cascada**
- Proceso secuencial
- IR en fases tempranas del proyecto (antes del diseño)
- Baja volatilidad de requisitos
- Requisitos bien estables
- Procesos pequeños

**Modelo Ágil (XP,S Scrum)** 
- Los requerimientos se obtienen cuando van a ser implementados.
- Alta volatilidad de requisitos.
- Incorporación cercana del cliente
- Consumidor al procesos
- Cuando los requisitos son muy cambiantes.
- Incorporación cercanas del cliente
- Cuando el cliente... no sabe tanto.

**Modelo Iterativo - Incremental (RUP)**
- IR una actividad continua
- Empresa grande.
- Requisitos estables.
- La planificación del proyecto y los requerimientos están fuertemente vinculados

-------
## EL PAPEL DE LA COMUNICACION EN LA IR 
Los requerimientos deben ser comunicados.
**Factores de lo que depende:** 
- El lenguaje como medio para comunicar
- La forma de comunicación elegida
- Elección de las expresiones más sencillas
- Conocimiento Implícito (entender al negocio)
**Influido por:** 
- Bagaje cultural (background)
- Experiencia y educación 
- Aspectos sociales

----------
- El cliente no me dice lo que quiere
- Falta de empatía
- Preguntar para conocer la situación actual del usuario.
- Preguntas que nos haga saber:
		Como esta hoy, como se encuentra, cuales son sus objetivos, sus deseos, etc

-----------
## **CARACTERISTICAS DE UN INGENIERO DE REQUISITOS
Puesto clave en un proyecto, punto central en la recopilación y administrador de la información

Organización{ 
DIRECCION
MARKETING
GESTION DE CALIDAD

{
Cliente
Jefe de proyecto 
Ingeniero de Requisitos
Documentadores
Desarrollador
arquitecto del sistma 
Tester

}
}
Legislador
![[Pasted image 20251024125556.png]]
no tester, sino legislador jij

-------
1. **Seguridad en si mismo (autoconfianza)** 
		1. Justificada por su competencia y sobre todo por su competencia en el negocio.
		2. Determinación en el seguimiento y clarificación en puntos abiertos (pendientes de aclaración)
2. **No debe sobreestimar sus propias capacidades.**
		1. Como interlocutor en un debate con especialistas. No es posible creer que tiene conocimiento de todo.
		2. Deberá mediar entre los puntos de vista de los distintos interesados.
		3. Detectar y resolver conflictos.
3. **Habilidad para convencer.**
		1. Comportamiento orientado a la solución.
		2. No está abierto a compromisos corruptos.
		3. Perseverancia.
4. **Habilidad para moderar y habilidad para empatizar.**
		1. Disposición para ponerse en el lugar de otra persona.
		2. Negocia entre implicados.
		3. Reconoce los deseos del cliente/usuario.
		4. Genera un proceso de aprendizaje común con el grupo de trabajo.
		5. Asegura que se tomen decisiones y obtienen resultados.
5. **Pensamiento Analítico.**
		1. Captura conceptos complejos (issues) del negocio.
		2. Descomponer los conceptos de negocio en sus partes más básicas.
		3. Reconocer las conexiones entre elementos
		4. Describir los conceptos del negocio sin dejar dudas o suposiciones.
6. **Habilidades de comunicación.**
		1. Ser capaz de expresarse en el lenguaje de cliente/ usuario.
		2. También a nivel internacional.
---------
## Clasificación de los requerimientos.
**¿Cómo sabemos que ya tenemos todos los requerimientos?**
- Está la información completa.
**¿Todos los requerimientos son iguales en tipo?**
- La información es la misma o es del mismo tipo
**¿Todos los requerimientos tienen la misma prioridad?**
- Decisiones con respecto a lo que va a realizar y a lo que no.
- Que debo hacer primero y que debo hacer después.
---------
Entender en que nivel nos encontramos:
- **NIVELES**
	- Negocio
	- Usuario
	- Sistema
- **TIPOS**
	- Funcionales
	- No funcionales
- **Prioridades**
	- Obligatorios
	- Importantes
	- Deseables
	- No implementables
-----
NEGOCIO
- Porque es importante el proyecto
USUARIO
- Para quien?
- Quien lo va a usar y en que actividades
SISTEMA
- Funciones del sw que van a sostener todo esto.
- Aqui están las especificaciones del deber ser

![[Pasted image 20251027121913.png]]

--------------
NEGOCIO: 
Especificación de visión y alcance.
- Necesidad y problema a resolver.
	- El estado actual de la organización cliente, y se establecen las razones para desarrollar el proyecto.
	- Descripción general de la historia o situación que nos lleva a reconocer la necesidad del producto sw
	- Resultados que se obtienen actualmente, los que no se han podido obtener, la forma de trabajo actual y los impedimentos que la organización a encontrado.
	
- Perfiles de stakeholders
- Objetivos del negocio


--------
USUARIO:
Identificar e involucrar a los usuarios permite cerrar la brecha de las expectativas.
- Diferencia entre lo que el usuario espera y lo que el desarrollador entrega.
- Establecemos las expectativas mediante la identificación de actividades que quieren hacer con el software
---------
SISTEMA:
- Especificación funcional, no funcionales y manual técnico.
- Atributo de calidad
- Interfaces y ambiente operativo

--------
**FUNCIONALES**
- Funciones que encontramos en lugares específicos del software.
- El funcional sabes donde está: EJM: Abrir un archivo, cargar un archivo
- Siempre inicia con un verbo infinitivo
**NO FUNCIONALES**
- Atributos que definen el comportamiento esperado del sw
- Parte de un todo, ejm: seguridad, rapidez, no solo es una parte sino de toda la aplicación.
--------
## Clasificación de los requerimientos - PRIORIDAD
**Obligatorios**
- Elementos necesarios para que el proyecto cubra los objetivos
- Sin ellos, el sistema no sirve
- El sistema debe mover los productos entre ubicaciones
**Importantes**
- Aportan valor, pero se le incluye si lo permite el calendario o pueden ser diferidos para otras entregas
- El sistema debe mover un lote de producto con una sola acción
**Deseables**
- Características cosméticas, se agrupan solo si el calendario lo permite, o se pueden omitir completamente.
- El sistema debe mover los productos con una acción de arrastrar y soltar.
**No Necesarios**
- Son los que no aportan valor.
- Están fuera de línea con los objetivos
- Son necesarios para un pequeño grupo de personas.
- El sistema debe animar los productos en tercera dimensión.

----------
## **Consideraciones:**
Definir el alcance es el arte de QUITAR características en lugar de agregarlas
- Los requerimientos deben satisfacer la necesidad de los usuarios.
- Entender la necesidad es un reto, una actividad colaborativa.
--------
## **Acciones a realizar:**
Comprender las actividades de los usuarios:
Qué están haciendo?
Qué objetivos tienen al  hacerlo?
Por qué hago esa actividad?
Por qué un proceso es complicado?

-----
## **¿Para que sirven los requisitos?**
- Para mostrar los resultados que los interesados (stakeholders) quieren.
- Para dar a los interesados la oportunidad de describir lo que quieren.
- Para representar distintos puntos de vista.
- Para revisar el diseño.
- Para medir progreso.
- Para aceptar productos respecto a un criterio preciso.
-----
## **¿Para quienes son los requisitos?**
**Usuarios**
Alguien que esta involucrado en el uso de sistemas cuando esté trabajando.
**Desarrolladores:**
Alguien involucrado en el desarrollo de un sistema que satisfaga los requerimientos del cliente
Ingeniero de Requeriminetos:
Alguien que ayuda a formular y entender los requerimientos de los usuarios.
Stakeholders:
Alguien que tiene una justificación para que se le permita influir sobre los requerimientos.
Cliente:
Alguien que paga para que el sistema sea desarrollado.

-------
## **TIPOS DE REQUISITOS**
### Técnicos:
1. Funcionales
	Describen las transformaciones que el sistema realiza sobre las entradas para producir las salidas.
2. No funcionales:
	Restricciones de los servicios o funciones que debe proveer el sistema (rendimientos, estándares, herramientas de desarrollo, etc)
### No técnicos:
1. Restricciones organizacionales o externas sobre el producto o su provisión (legales, costos, tiempos...)

------
## FUNCIONALES
- Relacionados con la descripcion del comportamiento fundamental de los componentes de w
- Las funciones son especificadas en términos de entradas, procesos y salidas
- Una vista dinámica podría considerar aspectos como el control, el tiempo de las funciones (de comienzo a fin) y su comportamiento en situaciones excepcionales.
-----
###  **Ejemplo de Requisitos funcionales**
El sistema deberá localizar un cliente para registrarle el cobro, utilizando criterios de búsqueda ~~adecuados.~~ *(esto es ambiguo) 

El sistema debe localizar un cliente para registrarle el cobro, presionando un ~~botón~~ que le permita buscar por el nombre del cliente y el identificador del cliente. (Incluye detalles de implementación) *No debe haber elementos externos, solo lo que debe hacer*
"" "", utilizando como criterios de búsqueda el nombre del cliente y el identificador del cliente.

Cada clase de usuarios puede requerir diferentes factores de calidad y restricciones ademas de asignarle diferentes prioridadaes segun sus tareas y perspectiva 
Durante la captura de requerimientos con frecuencia el user tiende a especificar restricciones sobre el sistema que en verdad esconden factores de calidad. El analista debe indagar acerca del porque de la restriccion, para identificar el factor de calidad implicito.

---------
## NO FUNCIONALES
- los factores de calidad y las restricciones conforman los requerimientos no funcionales.
- Mientras que los requerimientos funcionales especifican **qué** debe hacer el sistema, los requerimientos no funcionales establecen **cómo** debe hacerlo.
-----
**Factores de calidad:**
- Son atributos que influyen en el nivel de satisfacción que brinda el producto al cliente e incluso pueden determinar el éxito del proyecto.
- Establecen las cualidades del comportamiento
- Es importante capturarlos antes de que se diseñe la solución y no cuando el producto se verifica.
Los factores de calidad se dividen en:
## **1. EXTERNOS**
Son percibidos y valorados por los usuarios.
 
- Describen características observables cuando el sw está ejecutándose.
- Influyen poderosamente en el nivel de calidad que percibirá el usuario.
- Es el usuario quien debe indicar sus expectativas relacionadas con cada atributo de calidad externo y participa en la definición del criterio para medir la satisfacción.

**Disponibilidad** 
	- Se refiere al tiempo durante el cual el sistema estará en servicio ofreciendo toda su funcionabilidad.
	- El sistema está en servicio desde que comienza a funcionar hasta que deja de ejecutarse por una falla o por una parada de mantenimiento planificada o no.
	- Las tareas de mantenimiento pueden ser borrar archivos temporarios, transferir datos o recibirlos, desfragmentar el disco, etc.
	- Observemos que la palabra mantenimiento se está utilizando para referirse a una tarea y a una etapa en el proceso de desarrollo.
	- Hay funcionalidades más criticas que otras en el sentido de que son esenciales para que el usuario realice tu tarea.
	- Para cada funcionalidad o conjunto de funcionalidades. el usuario debe indicar en que periodos requiere disponibilidad y durante cuanto tiempo.
	- La disponibilidad está muy relacionada con confiabilidad y está fuertemente condicionada por la mantenibilidad que es una categoría de la modificabilidad.
	- La disponibilidad de considerarse particularmente en sitios web, aplicaciones basadas en la nube y aplicaciones distribuidas geográficamente.
	- En todos lo casos la disponibilidad depende de la **conectividad**.
**Instalabilidad**
	- El sw puede comenzar a usarse a partir del momento en que está correctamente instalado en el dispositivo que corresponde sobre una plataforma adecuada.
	- Se refiere al tiempo y capacitación que requiere realizar las operaciones que permiten que el sistema pueda comenzar a usarse.
	- *Por ejemplo:* descargar una aplicación en un celular, mover un sw desde una PC a un servidor web o actualizar un sistema operativo.
**Integridad**
	- Se ocupa de prevenir la perdida de información y preservar cierto nivel de correctitud en los datos.
	- Los datos deben protegerse de errores accidentales e intencionales.
	- Los ataques deliberados pueden tener las mismas consecuencias que los accidentes.
	- Los controles de validez en los datos ingresados por el usuario permiten garantizar cierto nivel de integridad.
	- La integridad requiere controlar también los datos recibidos de otros sistemas.
	- Es necesario además controlar la recepción de software para proteger a los datos.
	- El sistema puede preservar la integridad sin comprometer otros factores, como por ejemplo la sabilidad.
	- Un sitio web que inicializa todo un formulario cuando detecta que el usuario completó incorrectamente un campo, seguramente no va a satisfacerlo.
	- La integridad de los datos suele considerarse como parte de los requerimientos de seguridad.
	- En ocasiones se considera que la seguridad es una parte de la integridad, porque los requerimientos de seguridad suelen enfocarse a prevenir el acceso a los datos por usuarios no autorizados.
**Interoperatibilidad**
	- Muchos requerimientos de interperatibilidad pueden especificar como requerimientos con interfaces externas.
	- Cualquiera sea la clasificación adoptada, el analista debe elegir una categoría e incluir cada requerimiento en un solo lugar.
Performance
	- Es uno de los factores de calidad que aparece con mayor frecuencia, incluye a varios atributos y depende de varias cuestiones como la velocidad de la computadora y las conexiones en red.
	- Es una cualidad externa íntimamente relacionada con una cualidad interna: *la eficiencia*.
	- Una baja perfomance ante una consulta provoca irritacion y rechazo cpor parte del usuario pero ademas puede poner en riesgo a las condiciones de seguridad.
	- Los requerimientos de performance afectan alas estrategias de diseño de sw y la selección de hw
	- El usuario va a querer siempre tiempo de respuesta inmediato, pero la criticidad del traductor de un procesador de texto no es la misma que la de un radar de misiles.
**Confiabilidad**
	-Se refiere a la capacidad del sw para ejecutarse sin fallar por un periodo de tiempo.
	- Los problemas de confiabilidad se producen cuando se ingresan datos no validos, el codigo tiene errores, una componente no está disponible cuando se la necesita, el hw falla.
	- La confiabilidad está entonces íntimamente ligada a robustez y disponibilidad.
	- Está también muy ligada a verificabilidad. Los sistemas con grandes requerimientos de confiabilidad deben ver verificados rigurosamente.
	- **La manera de medir la confiabilidad puede ser:**
	- Porcentaje de operaciones que se ejecutan correctamente en un periodo
	- Promedio de tiempo entre fallas.
	- Los requerimientos de confiabilidad deberian cuantificarse considerando el impacto que provoca cada tipo de falla y el costo que provoca aumentar la confiabilidad.
	- Una falla puede provocar que el usuario tenga que rehacer su tarea. Es engorroso pero no catastrófico.
	- Por ejemplo si una transacción no se pudo complementar y se cancela completa, el usuario va a tener que repetirla.
	- Si se completa parcialmente y el usuario no lo percibe los datos pueden ser inconsistentes.
**Robustez**
	- Robustez/tolerancia a fallas, es la capacidad de un sistema de seguir funcionando adecuadamente ante situaciones anormales como fallas de hw datos no validos, ataques externos o condiciones operativas inesperadas.
	- Un sw robusto se recupera de situaciones imprevistas sin consecuencias graves.
Seguridad
	- Los requerimientos de seguridad se orientan a mitigar el riesgo de ataques y prevenir amenazas.
	- No hay tolerancia a fallas de seguridad, un sistema se considera seguro hasta que se detecta que es vulnerable.
	- La confiabilidad en cambio puede medirse en niveles de intensidad.
	- Se refiere a la capacidad del sistema para prevenir daños a las personas y pueden estar establecidos por regulaciones externas o internas.
	- Los dispositivos de hw controlados por un sistema de sw pueden poner en riesgo la vida y la salud de las personas.
	- Con frecuencia se especifican como condiciones o acciones que el sistema debe evitar que corran.
Usabilidad
	- Se refiere al esfuerzo que el usuario debe hacer para ingresar datos e interpretar la salida.
	- Incluye a todas las cualidades que hacen que un sistema se perciba como "amigable"
	- Uno de los aspectos claves de usabilidad es lograr satisfacer a un espectro heterogéneo de usuarios.
	- La simplicidad se refiere a cuan fácil es un sistema de aprender a usarse.
	- Son dos cualidades que pueden enferntarse.
## **2. INTERNO**
No pueden observarse durante la ejecución del sistema, afectan únicamente al equipo de desarrollo.
### **Eficiencia:** 
la eficiencia mide que tan bien utiliza el sistema a:
- el procesador 
- espacio en memo
- el ancho de banda
Si el sistema consume demasiados recursos el user percibe una degradación en la performance son factores fuertemente ligados.
La eficiencia es uno de los principales factores que determina la arquitectura del sistema e influye en la manera que el diseñador distribuye la computación y las funciones entre los componentes.
Es necesario que el analista estimule al usuario a considerar otros aspectos vinculando eficiencia con performance y anticipando el crecimiento de la demanda o la carga.
### **Modificabilidad**
La modificabilidad es la capacidad del diseño y la implementación para interpretarse, modificarse y extenderse.
Es un factor critico en aplicaciones desarrolladas para entornos dinámicos, desarrolladas con un modelo de ciclo de vida incremental o iterativo.
Está muy ligada a mantenibilidad y verificabilidad.
**Tipo de mantenimiento.**
- **Correctivo:**
	- Corrige defectos que no fueron detectados en la verificación o no se consideraron críticos.
- **Perfectivo:**
	- Mejora algunas funcionalidades para amentar la satisfacción de las necesidades del negocio nuevas o ya existentes.
- **Adaptativo:**
	- Modifica el sistema en respuesta a cambios en el entorno operativo, sin alterar su funcionalidad.
Cuando el diseñador y el desarrollador anticipan cambios pueden tomar decisiones que favorezcan la modificabilidad.
La modificabilidad puede medirse considerando el tiempo promedio requerido para realizar un mantenimiento correctivo, perfectivo o adaptativo.

### **Portabilidad**
- Se refiere al esfuerzo que requiere migrar un producto sw de un entorno operativo a otro.
- Algunos autores incluyen en este facto el esfuerzo requerido para internacionalizar un producto.
- Los aspectos de diseño que influyen en la portabilidad son similares a los que afectan a la portabilidad.
- Es un requerimiento importante en aplicaciones que deben ejeccutarse en distintos sistemas operativos o dispositivos como PC tablets, y celulares.
### **Reusabilidad**
- Indica que esfuerzo relativo requiere convertir una componente de sw para que sea utilizada en otras aplicaciones.
- El uso de metodologías rigurosas y estándares favorece la reusabilidad.
- Una componente reusable debe ser modular y estar documentada.
- Una componente genérica tiene mayor posibilidad de ser reusada que una específica.
- Los paquetes son componentes reusables y su utilización contribuye a implementar nuevos módulos de código reusables. 
- Idealmente una componente reusable debe ser independiente del entorno operativo de la aplicación para la cual fue desarrollada.
- Es un factor difícil de cuantificar pero el objetivo de reusar se aplica en dos niveles:
	- Ante un nuevo producto reusar todas las componentes que resulten adecuadas.
	- Desarrollar nuevas componentes considerando la posibilidad de que en el futuro puedan reusarse en otras aplicaciones.
### **Escalabilidad**
- Es la habilidad de una aplicación de crecer para adaptarse a escalabilidad un mayor número de usuarios, datos, servidores, localizaciones geográficas, transacciones, etc. Sin comprometer la performance o la correctitud.
- Está relacionada con modificabilidad y robustez.
- La robustez considera cómo se comporta el sistema cuando se excede el límite de su capacidad.
### **Verificabilidad**
- Se refiere a como los componentes de software el producto integrado puede evalarse para demostrar si el comportamiento del sistema es el esperado.
- Con frecuencia el responsable del testing desarrolla sw para verificar el sistema.
- Es un factor critico si el producto contiene algoritmos complejos o hay dependencias entre funcionalidades
- Tambien es un factor importante cuando el producto va a sufrir cambios frecuentes, porque va a ser necesario controlar que los cambios no dañen la funcionalidad existente.

PST: RNF CUANTIFICADORES


--------

## **TRADE OFF**
En un mundo ideal cada sistema deberia alcanzar el maximo nivel posible de cada factor de calidad.
Un sistema deberia ser accesible en todo momento, jamás fallar, brindar resultados inmediatos y correctos siempre, impedir cualquier intento de acceso no autorizado
Sin embargo, algunos factores están enfrentados y no es posible maximizar todos simultanteamente.

## **MEDIDAS**
**Medibles directamente pueden cuantificarse.** Es posible establecer una escala con valores minimos y maximos.
Por ejm eficiencia (tiempo,  espacio de almacenamiento), confiabilidad (tiempo entre fallas, fallas por unidad de tiempo).
**Medibles indirectamente** no se les puede asociar valores en concretos pero si indicadores que permitan decidir si se cumplieron o no.
Ejm: usabilidad, mantenimiento.

## **CAPTURA**
En un mismo sistema puede haber módulos que requieran un mayor nivel de calidad en cierto factor que otras.
Por ejemplo, algunas partes deben ser muy fáciles de aprender a usar, otras muy eficientes.
La captura de los factores de calidad requiere un procedimiento riguroso de interacción entre el analista y el resto de los participantes.

- ## Preguntas que no debes hacer:
	- **¿Usted considera que el sistema tiene que ser seguro? ¿Necesita que sea eficiente?**
	- **¿Qué nivel de seguridad debe garantizar el sistema?**

El *analista* guía al *usuario* en la exploración del proceso de negocios buscando como valorar cada factor
Nuevamente, no se trata solo del sw, es el sistema completo el que debe analizarse desde la perspectiva de cada factor de calidad seleccionado.

- ## **Preguntas que si debes hacer:**
	- **¿Cuál es el tiempo de respuesta que usted considera aceptable para que el sistema responda la consulta q1?**
	- **¿Cuál es el tiempo de respuesta que usted considera inaceptable para que el sistema responda la consulta q1?**
Si bien los requerimientos no funcionales pueden ser por un lado los más dificiles de detectar, también son los que pueden tener más aspectos en común entre un proyecto y otro.
El analista puede tener una lista de preguntas prestablecidas y luego seleccionar o reformular las que considera relevantes.
Una buena alternativa es combinar dos técnicas de captura: un cuestionario con un encuentro de captura
Los usuarios reciben el cuestionario anticipadamente, tienen oportunidad de pensar la respuesta con tiempo, pero la elaboran guiados por el analista durante un encuentro.
Pueden opinar varios representantes de la clase y el líder de usuarios decide.


# UNIDAD 2
## **Técnicas de elicitación / Captura de requisitos.
Sirven para: 
- Conseguir que los interesados humanos articulen sus requisitos.
- Recopilar el conocimiento sobre los requisitos del sistema.
**Este conocimiento debe estar estructurado:**
 - Partición -> Agregando conocimiento relacionado.
 - Abstracción -> Reconociendo generalidades.
- Proyección -> Organizándolo de acuerdo  a una perspectiva.
-------
### Talleres de discusión

### **Entrevistas**
Son la técnica de elicitación más usada, y son prácticamente inevitables en cualquier desarrollo ya que son una de las formas de comunicación más **naturales**
 ### **FASE 1: Preparación de la entrevista**
**1. Estudiar el dominio del problema.**
	Conocer las categorias y conceptos de la comunidad de clientes y usuarios es fundamenteal para poder entender las necesidades de deicha comunidad y su forma de expersarlas. Para generar en los clientes y users la confianza de que el ing de requisitos entiende sus problemas
	Para conocer el dominio del problema se recurre a:
	- Técnicas de estudio de documentación
	- Bibliografía sobre el  tema
	- Documentación de productos similares realizados anteriormente
	-  La inmersión dentro de la organización para la que se va a desarrollar
	- Periodos de aprendizaje por partes de los ingenieros.

**2 . Seleccionar a las personas a entrevistar.**
	- Se debe minimizar el numero de entrevistas a realizar, por lo que es fundamental seleccionar a las personas a entrevistar.
	- Normalmente se comienza por los directivos, que pueden ofrecer una vision global y se continua con los futuros usuarios, que pueden aportar información más detallada y con el personal técnico que aporta detalles sobre el entorno operacional de la organización.
	- Conviene también estudiar el perfil de los entrevistados, buscando puntos en común con el entrevistador que ayuden a romper el hielo.

**3 . Determinar el objetivo y contenido de las entrevistas.**
	- Para minimizar el tiempo de la entrevista es fundamental fijar el objetivo que se pretende alcanzar y determinar previamente su contenido.
	- Se puede anticipadamente enviar cuestionarios que los futuros entrevistados deben rellenar y devolver, y un pequeño documento de introducción al proyecto de desarrollo de forma que el entrevistado conozca los temas que se van a tratar y el entrevistador recoja información para preparar la entrevista.
	- Qué decir.
	- Cómo decirlo.
	- A quién le digo.
	- Cuándo decirlo.
	- Dónde decirlo.
	- Es importante que los cuestionarios, si se usan, se preparen cuidadosamente teniendo en cuenta quien los va a responder y no incluir conceptos que se asuman conocidos cuando puedan no serlo.

**4 . Planificar las entrevistas.**
	La fecha, hora, lugar y duración de las entrevista deben fijarse teniendo en cuenta siempre la agenda del entrevistado. En general, se deben buscar sitios agradables donde no se produzcan interrupciones y que resulten naturales a los entrevistados.
	1. **Apertura:**
		El entrevistador debe presentarse e informar al entrevistado sobre *la razón de la entrevista*, que se espera conseguir cómo se utilizará la información, mecánica de preguntas, etc.
		Si se va a utilizar algún tipo de notación gráfica o matemática que el entrevistado no conozca debe explicarse antes de utilizarse.
		Es fundamental causar buena impresión en los primeros minutos.
	2.  **Desarrollo**
		La entrevista en si no debería durar más de 2 horas. 20% para el entrevistador y un 80% para el entrevistado.
		Se deben evitar los monólogos y mantener el control por parte del entrevistador, contemplando la posibilidad de que una tercera persona tome notas durante la entrevista o grabar la entrevista en cinta de video o audio. Siempre que el entrevistado esté de acuerdo.
		Durante esta fase se pueden emplear distintas técnicas:
			1. **Preguntas Abiertas.**
				También denominadas de libre contexto estas preguntas no pueden responderse con un "si" o un "no", permite una mayor comunicación y evitan la sensación de interrogatorio.
				Estas preguntas se suelen utilizar al comienzo de la entrevista, pasando posteriormente a preguntas más concretas.
			2. **Utilizar palabras apropiadas:**
				Se deben evitar tecnicismos que no conozca el entrevistado y palabras o frases que pueden pertubar emocionalmente la comunicación.
			3. **Mostrar interés en todo momento.**
				Comunicación no verbal durante la entrevista: tono de voz, movimiento, expresión facial, etc.
	3. **Terminación**
		Al terminar la entrevista se debe recapitular para confirmar que no ha habido confusiones en la información recogida, agradecer al entrevistado su colabiración y citarle para una nueva entrevista si fuera necesario, dejando siempre abierta la posibilidad de volver a contactar para aclarar dudas que surjan al estudiar la información o al contrastarla con otros entrevistados.

#### Fase 3: Análisis de la entrevista.
Una vez realizada la entrevista es necesario leer las notas toamdas, pasarlas a limpio (minutas), reorganizar la información, contrastarla con otras entrevistas o fuentes de inforamción.
Una vez elaborada la informacion se puede enviar al entrevistado para confirmar los contenidos. Tambien es imporante evaluar la propia entrevista para determinar los aspectos mejorables.

Preparación: 
Investigar la situaacion 
Identificar las personas a entrevistar
Preparacion del objetivo y contenido
Planificar lugar y fecha

Conducción / Relización:
Apertura
Desarrollo Tempos: entrevistadso 80%
Terminacion

Analisis: 
Pasar a limpio las notas
Reorganizar las informacion y contrastarla
Evaluar la entrevista tenidentes a mejorar

### Cuestionarios, fichas, etc.
- Tormenta de ideas (brainstorming)
- Prototipos
- Escenarios (casos de uso)
- Flujos de trabajo, Storyboards
---------
## **JAD**
Joint application development, desarrollo conjunto de aplicaciones. Desarrollada por IBM en 1977, es una alternativa a las entrevistas individuales que se desarrolla a lo largo de un conjunto de reuniones en grupo durante un periodo de 2 a 4 días
En estas reuniones se ayuda a los clientes y users a formular problemas y explorar posibles soluciones, involucrándolos y haciéndolos sentirse partícipes del desarrollo.

------
JAD - PRINCIPIOS
1. Dinamica del grupo
2. Uso de ayudas visuales para mejorar la comunicacion (diagramas, transpaprencias, mutimedia)
3. Mantener un proceso organizado y racional
4. Filosofia de documentacion WYSIWYG What you see is what you get. LOo que se ve es lo que se obtiene por lo que durante las reuniones se trabaja directamente con los documentos a generar.


------
JAD - PASOS
1. JAD / PLAN cuyo objetivo es elicitar y especificar requisitos
2. JAD / DESIGN ?  En el que se aborda el diseño del sw

----------
Ventajas 
Ahorra tiempo al evitar que las opinioes de los clientes se contrasten por separado.
Todo el grupo, incluyendo clientes y futuros usuarios revisa la documentacion generada, no solo los ing de requisitos
Implica mas a losclientes y usuarios en el desarrollo.

--------
Desventajas
No suele adaptarse bien a los horarios de  trabajo de los clientes y usuarios.
No suele emplearse con frecuencia.
A muchos les parece una tecnica dificil.

-------
JAD - PARTICIPANTE.
JEFE: Es el responsable de todo el proceso y asume el control durante las reuniones . Debe tener dotes de comunicacion y liderazgo.
Habilidades:
1. Entender y promover la dinamica de grupo
2. Iniciar y centrar discusiones
3. Reconocer cuando se esta desviando del tema y reconucirla
4. Manejar las distintas personalidades y formas de ser de los participantes
5. Evitar que decaiga la reunion aunque sea larga

----------
Analista:
Es el responsable de la produccion de los documentos que se deben generar durante las sesiones JAD.
Debe tener la habilidad de organizar bien las ideas y expresarlas claramente por escrito.
En el caso de que se utilizan herramintas sw durante las sesiones, debe ser capaz de manejarlas eficientemente.

------
PATROCINADOR EJECUTIVO.
promotor/stakehodler. Es el que tiene ladecision final de que se lleve a cabo el desarrollo. Debe proporcionar a los demas participantes informacion sobre la necesidad del nuevo sistema y los beneficiones que se espera obtener de el

*Representatnes de sistemas de informacion
Son personas expertos en sistemas de informacion que debene auudar a los users a comprender que es o no factible con la tecnologia actual y el esfuerzo que implica.*

-------------
REPRESENTANTES DE LOS USUARIOS.
Durante el Jad/PLan suelen ser directivos con una vision global del sistema.
Durante el Jad/Design suelen incorporarse futuros usuaros finales.

Especialistas
Son personas que pueden proporcionar informacion detallada sobre aspectos muy conocretos
Desde el punto de vista de los users porque concoen muy bien el funionamiento de una parte de la organizacion
Desde le POV desarrolladores porque conocen. perfectamente ciertos aspectos tecnicos de la isntalacion hw de la organizacion

-----------
Adaptacion -> celebracion de las sesiones JAD -> Conclusiones

-----
Adaptacion
El jefe JAD es quien debe adaptar la sesion a las caracteristicas propias del proeyecto en curso. Para ello debe:
1. Documentarse sobre la organizacion y el proyecto
2. Decidir cuestiones organizativas sobre las sesiones JAD: numero y duracion, lugar,fechas
3. Seleccionar a los participantes adecuados para cada reunion.

-------
FASE DE SESIONES
Esta dividida en una serie de pasos:
Presentacion: al igual que en la entrevista individual, el jefe del JAD y el patrocinador ejecutivo se presentan. eL PATROCINADOR EXPLICA LOS MOTIVOS DEL PROYECTO
eL JEFE DEL jad EXPLICA LA MECANICA DE LA REUNION.

Definicion de requisitos de alto nivel: Esto ya es parte del trabajo productivo. El jefe del JAD hace preguntas del tipo "pq se construye el sistema", "que beneficiones se esperan del nuevo sistema", "Como puede beneficiar a la organizacion en el futuro"

A medida que se va elicitando requisitos, el analista los escribe en transparencias o en algun otro medio que permita que permanezcan visibles durante la discusión. Una posibilidad es utilizar para ello plantillas.

Delimitar el ámbito del sistema: cuando se ha reunido un conjunto de requisitos lo suficientemente grande se les puede organizar y decidir el ambito del sistema. En el caso de los S.Infr es util identificar a los usuers potenciales, actores y determinar que tareas les ayudará a realizar (casos de uso)

Documentar temas abiertos: Si un tema queda sin resolver se  debe documentar para otra sesion y asignar una persona responsable de su solucion, para lo cual puede utilizarse la plantilla de conflictos.
Concluir la sesion: el jefe del JAD hace un repaso de la informacino obtenida con los participantes.
Se da la oportunidad a todos los participantes de expressar cualquier consideracion adicional, fomentando por parte del jefe del JAD el sentimiento de propiedad y compromiso de todos los participantes sobre los requisitos elicitados.

--------
	Conclusion se trata de producir un doc con la informacion recabada en la fase anterior. Hay 3 partes que se siguen secuencialmente:
1. Compilar la documentacion: La doc recofgida se redacta en un doc normalizado.
2. Revisar la documentacion: Se envia la documentacion a los participantes para que efectuen correciones
3. Validar la documentacion: El patrocinador ejecutivo da su aprobacion. Una vez aprobado el documento se envian copias definitivas a cada uno de los participantes.
4. 



--------
## **Brainstorming** 
o tormenta de ideas es una técnica de reuniones en grupo cuyo objetivo es la generación de ideas en un ambiente libre de criticas o juicios (gause y weinberg 1989)
Las sesiones de brainstorming suelen estar formadas por un numero de  4 a 10 participantes uno de los cuales s el jefe de la sesión encargado mas de comenzar la sesión que de controlarla (diferencia entre JAD)

El brainstorming puede ayudar a generar una gran variedad de vistas del problema y a formularlo de diferentes formas, sobre todo al comienzo del proceso de elicitacion, cuando los requisitos son todavia muy difusos.
Ventaja:
Frente al JAD, el branstorming tiene la ventaja de que ees facil de aprender y requiere poca organizacion de hecho hay propuestas de realización de brainstorming por video-conferencia a traves de Internet.
Desventaja:
Al ser un proceso poco estructurado, puede no producir resultados con la misma calidad o nivel de detalle que otras tecnicas.

FASES:
Preparacion -> Generacion -> Consolacion -> Documentacion

----
Preparación
La preparación para una sesion de brainstorming requiere que se seleccione a los participantes y al jefe de la sesión citarlos y preparar la sala donde se llevará a cabo la sesión
Los participantes en una sesión de brainstorming para elicitacion de requisitos son normalmente clientes, usuarios, ing. de requisitos, desarrolladores y, si es necesario, algun experto en temas relevantes para el proyecto.

Generacion
El jefe abre la sesion exponiendo un enunciado general del problema a tratar, que hace la semilla para que se vayan generando ideas.
Los participantes aportan libremente nuevas ideas sobre el problema semilla, bien por un orden establecido por el jefe de la sesion, bien aleatoriamente.

El jefe es siempre el responsable de dar la palabra a un participante. Este proceso continua hasta que el jefe decide parar, bien pq no se están generando suficientes ideas, en cuyo caso la reunion se pospone, bien pq el numero de  ideas sea suficiente para pasar a la siguiente fase.

Durante esta fase se deben observar las siguientes reglas:
- Se prohibe la critica de ideas, de forma q los participantes se sietnan libres de formular cualquier idea.
- Se fomenta las ideas mas avanzadas que aunque no sean factibles, estimulan a alos demas participantes a explorar nuevas soluciones mas creativas.
- se debe generar un gran numero de ideas ya que cuantas mas ideas sep resenten mas problable sera que se genern mejores ideas.
- Se debe adelantar a los participantes a combianar o completar las ideas de los participantes. Para ello es necesario al iguak que en la tecnica del Jad que todas las ideas generadas.
- ........

Consolacion: Se deben organizar y evaluar las ideas generadas durante la fase anterior. Se sigue:
1. Revisar ideas: se revisan las ideas generadas pra clarificarlas. Es habitual identificar ideas siilares, en cuyo caso se unifican en un solo enunciado.
2. Descartar ideas: Aquellas ideas que los participantes consideren excesivamente avanzadas se descartan
3. Priorizar ideas: sepriorizan ideas restantes identificando las aboslutamente esecnciales las que estarian bien pero no son esenciales y las que podrian ser apropiadas para una proxima version del sistema a desarrollar.

DOCUMENTACION
despues de la sesion el jefe produce la doumentacion oportuna conteniendo las idesa priorizadas u comentarios generados durante la consolidacion


----------
Casos de uso los  casos de uso son una tecnica para la especificacion de req funcionales que actualmente forma partde de la propiesta DE UML

presentan ciertas ventajas ya que facilitan la elictacion de requisitos y son facilmente comprensibles por los clientes y users ademas, pueden servi de base a la s priebas del sistema u a la documentacion para los usauios.
sE PROPONE LA UTILIZACION DE LOS CASOS DE USO como tecnica tanto de elicitacion como de especificación de los requisitos funcionales del sistema.

----------
## **Diagramas de casos de uso**
Los C.U. tienen una representación grafica de los denominados diagramas de casos de uso.
ACTOR: Alguien o algo externo al sistema que interactúa con el desempeñando un rol.
Un caso de uso siempre es iniciado por un actor externo.
Caso de uso: Interacción entre actores y el sistema que produce un resultado observable de valor para un actor.
Limite del sistema: agrupa casos de uso dentro de un mismo sistema. Util cuando tenemos varios sistemas/subsistemas
Asociación:  la participación de un actor es necesario para realizar un caso de uso.

Verbo en infinitivo en los óvalos

-----
Extensión: 
es en cambiar la contraseña, algo que ejecutaré pero no siempre?
Ejemplo:
Un actor administrador puede entrar en el sistema, dar de alta a un pintor y marcharse

Un actor administrador puede entrar en el sistema, asignar a un pintor una restauracion y marcharse.

Un administrador puede entrar en el sistema, empezar a asignar a un pintor una restauración durante el proceso darse cuenta de que el pintor no esta en el sistema, darlo de alta sobre la marcha, terminar la asignación y marcharse.

-----
Inclusión
"Cuando siempre voy a buscar" 
Un actor administrador puede entrar en el sistema, asignar a un pintor una restauración y marcharse.
Para elegir una restauración a la que asignar un pintor, el admin debe realizar una bisqueda entre todas las restauraciones existentes y seleccionar una


1. ACTORES
2. FUNCIONALIDADES
3. ENLACES O ASOCIACIONES (actor - usuario, include, extense)
El include y extense es solo entre casos de uso, uno es obligatorio y otro "depende


---------
Una empresa comercializadora desea invertir en la adquision de un sistema orientado al control de las ventas de sus productos, los requerimientos que el sistema debe satisfacer son:
1. Permitir que los vendedores registren las ventas, para ello deberán consultar el saldo de los productos.


---------
## **Historias de usuario**
Es una pequeña descripción simple y clara de un requerimiento del usuario. Está escrita en lenguaje natural y debe ser verificable, es decir, debe tener una prueba asociada. Se escriben en una pequeña hoja  autoadherible para tenerla en la pared o pizarra. Cada historia se discute con el user para aclararla cada vez más

Responde: ¿Quién? ¿Qué hace? y ¿Por qué lo hace? en un solo párrafo
	Aprobación de nuevos usuarios.
	Yo como administrador del foro quisiera poder aceptar o rechazar los nuevos users registrados para para poder evitar que el foro se llene de spammers.

----
## **UML Análisis de requisitos**
### Diagramas de UML
Un modelo es una descripción completa de un sistema desde una perspectiva concreta.
Del modelo, salen los diagramas: de clases, objetos, componentes, distribución, actividad, estados, colaboración, secuencia, casos de uso.

**Diagramas de estructuras:**
clase, objetos
**Diagramas Comportamiento**
casos de uso estados actividad
**Diagramas Interacción:**
secuencia colaboración
**Diagramas Implementación:**
componentes despliege

-----
**Caso de Estudio -Punto de venta.**
Supongamos como caso de estudio el sistema de una terminal de punto de venta. Esta terminal es un sistema automatizado con el que se registran las ventas y se realizan los pagos.
Por lo general este tipo de sistemas comprenden Hardware (un computador y un lector de código de barras) y software (el sistema que se ejecuta en la terminal).

----------
Los requerimientos son una descripción de las necesidades o deseos que debe satisfacer un producto.
**Definir al menos los siguientes puntos:**
- Panorama general Este proyecto tiene por objeto crear un sistema de terminal para un punto de venta que se utilizará en las ventas de un supermercado.
- Metas: En términos generales , la menta es un mayor automatización del pago en las cajas registradoras, y dar soporte a servicios más rápidos, más baratos y mejores. Concretamente, la meta incluye:
	- Pago Rápido de los clientes.
	- Análisis rápido y exacto de las ventas.
	- Control automático del inventario.
- Funciones del sistema: Las funciones del sistema serán lo que este deberá hacer:
	Las funciones pueden clasificarse en tres categorías: evidentes, ocultas y superfluas.
	- Las evidentes deben realizarse y el usuario deben saber que se han realizado.
	- Las ocultas también debe realizarse, y puede que no sean visibles para el usuario.
	- Las superfluas son opcionales, y su inclusión no repercute significativamente en el costo ni en otras funciones.
-

-----
Ejemplo de CU de alto nivel.
Describe clara y concisamente el proceso de comprar productos en una tienda cuando se emplea una terminal en el punto de venta.
Caso de uso: comprar productos
Actores: cliente, cajero
Tipo primario
Descripción: un cliente llega a la caja registradora con los artículos que comprará. El cajero registra los artículos y cobra el importe. Al terminar la operación, el cliente se marcha con los productos.

Ejemplo de uncaso expandido de uso:
casi de uso: comprar productos en efectivo
Actores Cliente iniciador, cajero
Propóstio Capturar una venta y su pago en efectivo.
Resumen: Un cliente llega a la caja registaradora con los artículos que desea comprar


Construccion de casos de usos:
Un caso de uso debe ser simple, inteligible, claro y conciso.
Generalmente hay pocos actores asociados a cada caso de uso.
Preguntas:
cuales son las tareas del actor?
que informacion crea, guarda, modifica, destruye o lee el actor?
debe el actor notificar al sistema los cambios externos?
debe el sistema informar al actor de los cambios internos?




------
# UNIDAD 3#
## Modelo conceptual.
- Un MC explica a los creadores los conceptos significativos de un dominio del problema
- Es el artefacto más importante a crear durante el análisis orientado a objetos.
- En métodos OO que carecen de una técnica de captura de requisitos se comienza inmediatamente con la construcción del MC
- Una cualidad esencial del MC es que representa cosas del mundo real, no componentes del SW.

La siguiente figura muestra un modelo conceptual parcial del dominio de la tienda y las ventas.
CONCEPTO
ASOCIACIÓN
ATRIBUTOS

-------
En UML se ilustra con un grupo de diagramas de estructura estática donde no se define ninguna operacion. Puede mostrar:
Conceptos, asociaciones entre conceptos, atributos entre conceptos.

----
MC - Conceptos:
Concpetos:
Informalmente ->idea cosa u objeto
Formalmente
	Simbolo. Palabras o img respresentando un concpeto
	Definicion
	Extension


-------

Un concepto tiene un símbolo, una definición y una extensión

------
## **Modelo conceptual - Estrategias para identificar los conceptos**
Es mejor exagerar y especificar un modelo conceptual con muchos conceptos detallados que no especificarlo cabalmente.

No excluya conceptos simples solo porque en los requerimientos no se indique
.
.


---------
## Recomendaciones para crear el MC.
- Denomine los conceptos y atributos con los nombres que tienen en el mundo real.
- Excluya conceptos del mundo real que no sean pertinentes a los requerimientos.
- No adiciones cosas que no estén bajo consideración en el dominio del problema
- Si en el mundo real no consideramos algún concepto X como número o texto, probablemente X sea un concepto y no un atributo.

--------

Asociaciones
Una asociacion es una relacion entre dos conceptos que indica alguna conexion significativa entre ellos. Las asociaciones utiles a determinar suelen incluir el conocimiento de relacion que ha de preservarse por algun tiempo: puede tratarse de miliseg o de años (segun el contexto). Por ejm: debemos recordar cuales instancias de ventas LineaDeProductos estan aosciadas a venta? Si pq de lo contrario no seria posible reconstuir la venta, imprimir la boleta ni calcular el total de la venta.


-----
## Modelo Conceptual - Multiplicidad


-------
## Vidio

Análisis de Requerimientos - Desarrollo de sistemas web y aplicaciones móviles.
Es fundamental para las empresas. Algunas empresas no consideran las necesidades, prioridades, tiempo, costo estimado, por ende ....

Líderes sacan costos,
Cuál es el problema que encontramos, sus procesos, 2 propuestas de solución, el que gane le daremos caña al SRS con la propuesta ganadora.

--------
sistema complejo bla bla
el analisis de requerimientos: 
las aplicaciones de sw interactuan con actores en un sistema complejo (hw, redes). Eso es el contexto, ahi hay informacion importante para requisitos No funcionales. 

Hardware capacidad, versiones. Cantidad actualizable. Cual es la disponibilidad para cambiar de nuevo.
El sistema debe ser adecuado, entender el contexto es importante.

Dominio de la información: 
Cliente: dispositivo o programa que se comunica con un servidor 
Entidades + relaciones en el dominio: analisis del dominio es un diccionario de datos. Qué significa cada palabra/sustantivo? Es una descripción de alto nivel.

Procesamiento de informacion:
En el analisis de req hay que definir como y donde 

comportamiento : es la descripcion de como debe portarse el sistema ante escenarios de exito o errors

descrpcion de req:  permite entender el sistema en alto nivel, herramientas: diagramas uml, secuencia, clases, actividad. No sobredocumentar. Usar un diagrama de contexto, clases, secuencia y actividades

------

2 propuestas. 
Si en la 1 p

la 1 propuesta debe solucionar (mejorar en tiempos, productividad) (descripcion alto nivel, descripciones)
la 2 propuesta es nuestro plus (solo el plus, si creas un proceso adicional, redactamos eso)
Los lideres representan los costos de cada CU


------
expandido del 1 y 2


----------------

## Verificación y ajuste de requisitos.
Por qué validar?
- Detección temprana de defectos en contenido o en documentación a efectos de su aprobación.
- Cumplimiento de criterios de calidad definidos , a fin de obtener su aprobación para la siguiente fase de desarrollo.
- Evaluación respecto de lo criterios de calidad.
**a) Completitud, corrección**
- Carencias en el contexto conducen a la carencia en funcionalidades o funcionalidades mal implementadas.

**b) Comprensibilidad no ambigüedad y consistencia.**
- Depurar inconsistencias
- Peligro de una mala implementación
- Cambios en la base de los requisitos no son comunicados.

**c) Ponderación basada en criticidad / estabilidad.**
- Un énfasis erróneo conduce a la insatisfacción del cliente.

**d) Verificabilidad**
- Prueba de aceptación: Requisitos ambiguos conducen a discusiones con el cliente.
- Consecuencias legales por disputas contractuales.

**e) Capacidad de ser modificado**
- Una gestión complicada de requisitos conduce a la ineficiencia en el transcurso del proyecto.
- En el caso de haber redundancias, el cambio conduce a inconsistencias.

**f) Trazabilidad**
- Análisis de impacto: Cambios en requisitos conducen a una estimación errónea del esfuerzo.


--------
## Fundamento del ajuste de requisitos.
- Si no existe consenso respecto de lo requisitos entre los implicados existe, 
	- Peligro de no realización de requisitos.
	- Peligro de no aceptación de requisitos.
- Resolución de conflictos como una oportunidad para desarrollar nuevas ideas. 
- Conformación de un entendimiento colectivo entre todos los implicados relevantes.
- Tipos de acuerdo asociados a requisitos.
	- De forma continua.
	- Tiempo y esfuerzo consumido.
	- Minimización del riesgo.



9 horas -> 156 -> 144 horas





*Propuesta V1.0.0 | Corregido -> V1.0.1*


--------
## Evaluación de los aspectos de calidad de los requisitos.
- **Contenido ->**
	- Calidad de información contenida en la descripción de los requisitos.
	- Se han levantado y documentado todos los requisitos relevantes con el nivel de detalle apropiado? (esto debemos evaluar al otro grupo)
- **-> Documentación ->**
	- Todos los requisitos se han documentado con respecto a las guías de documentación y especificaciones establecidas?
- **- > Nivel de acuerdo:**
	- Todos los implicados están de acuerdo con los requisitos documentados?
	- Han sido resueltos todos los conflictos?

### Criterios para validar la calidad del contenido:
1. **Completitud del documento de requisitos.**
	- Todos los requisitos relevantes para el sistema a desarrollarse se han documentado?
2. **Completitud de cada requisito individual**
3. **Trazabilidad**
4. **Corrección y adecuación**
	- Los requisitos reflejan las necesidades y deseos del promotor?
5. **Sin decisiones de diseño prematuras.**
	- No se deben tomar decisiones de diseño antes de que sean establecidas las restricciones relevantes.
6. **Necesidad**
	- Los requisitos que están especificando contribuyen a alcanzar un objetivo definido?
7. **Verificabilidad**
	- Criterios de aceptación y prueba basados en los requisitos.

------
### Criterios para validar la calidad de documentación
1. **Conformidad con el formato de documentación.*+
	- Aplicación de plantillas, obligatorias, notación..?
2. **Conformidad con la estructura de la documentación.**
3. **Comprensibilidad.**
	- En el contexto dado, uso de un glosario (acrónimos, API, HTML, etc).
4. **Claridad y no ambigüedad.**
	- Única interpretación del documento de requisitos.
5. **Conformidad con normas de documentación.**
	- Conformidad con la sintaxis del lenguaje de modelado aplicado.

---------
### Criterios para validar la calidad del producto.
1. **Claridad y ausencia de ambigüedad**
	- Los requisitos deben estar redactados de forma precisa, sin interpretaciones múltiples.
	- Uso de lenguaje sencillo, términos definidos y consistentes.
2. **Completitud**
	- La especificacion debe cubrir todas las funciones, restricciones y condiciones del sistema.
	- No deben faltar requisitos criticos para la operacion o seguridad
3. **Consistencia**
	- Los requisitos no deben entrar en conflicto entre si.
	- Se debe mantener coherencia en términos, numeración y formato
4. **Verificabilidad**
	- Cada requisito debe poder ser probado, medido o validado mediante casos de prueba o inspección.
	- Evitar requisitos subjetivos como "el sistema debe ser fácil de usar" sin métricas asociadas.
5. **Trazabilidad**
	- Los requisitos deben poder rastrearse desde su origen (cliente, normativa, caso de uso) hasta su implementación y pruebas.
	- Se recomienda usar matrices de  trazabilidad para asegurar cobertura.


--------
### Calidad nivel adecuado

1. **Conciliación**
	- Todos los requisitos han sido acordados con todos los interesados involucrados?
2.  **Conciliación tras el cambio**
	- Todos los requisitos modificaron han sido acordados por todos los implicados ?
3. **Conflictos resueltos**
	- Han sido resueltos todos los conflictos conocidos respecto de los requisitos ?

------
### Validacion de requisitos en la practica
1. **Involucrar a los implicados correctos**
	- Asegurar el principio de los 4 ojos para la revisión
	- Organizar revisores internos y externos
	- Evitar que el autor del requerimiento sea quien valide
2. **Separar el descubrimiento de errores de la corrección de errores**
	- Principio: encontrar - evaluar - decidir - corregir
	- Concentrarse en la detección de defectos
3. **Comprobar desde distintos puntos de vista.**
	- Diferentes implicados
	- Lectura basada en la perspectiva.
4. **Adecuar el cambio del tipo de documentación**
	- Evaluar los diferentes tipos de documentación
	- Pasos distintos cuando se aplica el conocimiento documentado.
5. **Construcción de artefactos de desarrollo.**
	- Evaluar la adecuación de un requisito dado para el desarrollo de artefactos
6. **Repetir comprobaciones**
	- En diferentes puntos durante la evolución del proyecto con diferente conocimiento.

Tecnicas para la validacion de requisitos
- Informes de expertos (- costo, - efectividad)
- Revisiones guiadas
- Inspecciones (+ costo, + efectividad)

-------------------------> 
Costo / esfuerzo , efectividad



--------
## Técnicas para la validación de requisitos - Basados en la IEEE 1028
### Informes de experto:
- Forma más simple de una revisión, con frecuencia iniciada por el autor.
- En lo que respecta a la elección de lo revisores, solo es necesaria competencia funcional.
- No es necesaria una reunión
- Los resultados son documentados y transferidos en listas, se realizan observaciones al documento.
- Normalmente se realiza en la forma de una lectura cruzada del objeto bajo evaluación por pares, basada en criterios de calidad

-----
Ventajas: 
Ejecución rápida
Barata

Desventaja:
No hay actas
Resultados de calidad variable

Las revisiones informales y técnicas (basada en el IEEE 1028) se distinguen por el grado de formalismo. La revisión informal ofrece lagunas simplificaciones por ejemplo, simple lectura cruzada en lugar de una reunión sin actas.


-------
### Revisión guiada (walkthrough)
1. Procedimiento menos formal
2. Versión ligera de la definición de roles
	1.  Revisor
	2. Autor = moderador
	3. Secretario
3. El objeto de revisión (el doc) también es distribuido a los revisores con antelación
4. Procedimiento: Durante la presentación paso a paso, del objeto a evaluar por parte del autor, los revisores observan y discuten defectos y problemas.

**Ventajas:**
Menor esfuerzo de preparacion - a pesar de que la reunion puede durar menos que la de una inspeccion.
La reunion puede ser iniciada con poca antelacion
Los conflictos pueden ser resueltos durante la discusion (dialogando)

**Desventajas**
El autor modera y puede tener una fuerte influencia sobre el proceso
- Peligro, posiciones cirticas que no sean discutidas con detalle suficiente
Bajo grado de seguimiento, dado que el autor también es responsable del seguimiento.
Menos efectiva que una inspeccion

--------
### Inspección
- Procedimiento altamente formal.
- Enfoque estrictamente formal a través del seguimiento de fases:
-  Planificación -> Presentación general -> Deteccion de defectos -> Lista de hallazgos + Consolidación de defectos
- Roles claramentes definidos:
	- Organizador
	- Presentador (lector)
	- Moderador (independiente, entrenando)
	- Revisor
	- autor
	- Secretario

1. **Fase de presentación**
	- Presentación del objeto bajo inspección por parte del autor.
2. **Los revisores (normalmente pares)**
	1. Evalúan el objeto de prueba bajo lo criterios de devaluación según fueron definidos
	2. Listas de comprobación, métricas
3. **Revisión de la preparación del objeto se determina con antelación.**
	1. Determinación de los criterios de entrada y salida
4. **El resultado es un informe de inspección / lista de hallazgos.**

-------
### Factores de éxito de las revisiones
1. Las revisiones deben ser realizadas con enfoque a los objetivos
2. Los autores de los documentos evaluados deberían ser "tratados de forma positiva" por la revisión
	- "Su documento está mejorando" en lugar de "su documento está muy mal"
3. Se debe aportar un presupuesto adecuado (del 10% al 15% del presupuesto total de desarrollo) para la ejecución de revisiones.
4. Hacer énfasis en los efectos de aprendizaje ( realimentación /mejora continua ) con la experiencia ganada en las revisiones ejecutadas previamente.
5. Duración de la reunión máximo de 2 horas.
6. Obligatoria a la participación de los implicados relevantes en las revisiones.

-----
## **Técnicas para la validación de requisitos - Otras técnicas.**
Lectura basada en perspectiva -> Comprobación a través de prototipos -> Uso de listas de comprobación

-------
### Lectura basada en perspectiva
- Uso en combinación con otras técnicas.
- Perspectivas de calidad, ejm: doc, contenido, aprobación
- Perspectivas de implicados: ejm: cliente/user, arquitecto de sw, probador.
- Requiere instrucciones detalladas con respecto a como evaluar cada perspectiva, ejm: cuestionario, lista de comprobación.
- Consolidación de respuestas / listas de comprobación
- Reunión de conclusión.

--------
### Comprobación a través de prototipos.
1. Prototipo evolutivo (desechable)
	- Desarrollo a través de múltiples fases, algo consumo de tiempo.
2. Enfoque
	- Selección de requisitos bajo evaluación
	- Realización del prototipo
	- Preparación de la evaluación
		- Formación del user para q sea capaz  de operar el prototipo
		- Diseño de escenarios de prueba incluido datos
		- Diseño de criterios de evaluación para evaluar criterios
3. Ejecución - autónoma sin influencia-
4. Pruebas experimentales (En contexto de habilidades)
5. Documentación de lo resultados de la evaluación por parte del revisor y del observador
6. Valoración - revisión de los requisitos o del prototipo.

--------
### Uso de listas de comprobación
1. Las preguntas incluidas hacen *más fácil la detección de defectos* especialmente en asuntos complejos
2. Las listas de comprobación son desarrolladas antes de su uso en una evualuación
3. Mejora continua de las listas de comprobación durante el curso del proyecto.
4. Las listas de comprobación no deben ser obligatorias, pero si de apoyo.
	- Medios para estructurar por ejm: entrevistas
	- Las listas de comprobación normalizan la evaluación de contenido
5. El uso eficaz de las listas de comprobación depende de:
	-  Complejidad moderada, una p{agina de preguntas propuestas.
	- Concretas, preguntas sobre temas precisos.

-----
## **4 TAREAS DURANTE LA CONCILIACION DE REQUISITOS 
Conciliación se genera when hay conflictos
1. Identificación del conflicto
	- Durante la valoración, evaluación, sistematización.
	- Entre los distintos implicados, conflictos de objetivos.
2. Análisis del conflicto
	- Determinar el tipo del conflicto.
	- Elaboración de la resolución / conciliación de estrategias.
3. Resolución del conflicto
	- Factor clave de éxito para proyectos.
	- Fundamental involucrar a los implicados.
4. Documentación de la resolución del conflicto.
	- Previene la reaparción de conflictos ya resueltos.
	- Conserva la información adquirida para ser reutilizada en otros conflictos.

------
## **TIPOS DE CONFLICTOS**
**Conflicto sobre contenido.**
- interpretaciones diferentes, falta de información.
**Intereses Opuestos** 
- Departamento de dominio vs Departamento de TI.
**Conflictos sobre valores**
- Valores personales, valoración diferente respecto de valores comunes.
**Conflictos sobre relaciones**
- Justificado emocionalmente (por ejm: situaciones de rivalidad).
**Conflictos sobre estructura**
- Basado en diferencias en poder y autoridad.

---------
## **Gestión de Requisitos.**
Los requisitos cambian durante el ciclo de vida de desarrollo de producto. Los cambios deben controlarse y documentarse, es decir, hay que convivir con ellos y por ello la gestión de cabios es esencial para tratar dichos cambios.
Cuando, durante el proyecto y una vez aceptada la línea base de requisitos, se solicita un cambio sobre esta línea base, estos cambios no se pueden aceptar sin más ya que podrían afectar al desarrollo de todo el sistema, o alguna parte esencial del mismo.

---------
### Lección 1: Aportar atributos de un requisito.
Para gestionar requisitos durante todo el ciclo de vida del sistema, es necesario recoger información sobre lo mismos de forma estructurada.
La definición de la estructura de atributos para los requisitos se lleva a cabo mediante un esquema de atributos que puede definirse en forma tabular o creando un modelo de información.

**Atributos habituales:**
- Identificador: único, identificación del requisito relevante para el proyecto.
- Nombre: Permite una fácil descripción del tema de requisitos.
- Descripción: Descripción corta del contenido.
- Obligatoriedad: debe, debería o se hará.
- Versión: De acuerdo con la gestión de versiones.
- Fuente: Origen del requisito.
- Estabilidad: baja estabilidad si los requisitos son susceptibles de cambio.
- Criticidad: Determinado por los riesgos técnicos de la implementación.
- Prioridad: Establecido desde el POV del cliente o la gestión del proyecto.

----
IMG

-----
### **Lección 2: Diferentes vistas de requisitos.**
- Creación de diferentes vistas de requisitos.
- Cada implicado  tiene una vista especifica y diferente de los requisitos.
- Los clientes quieren ver el avance del proyecto
- Los probadores necesitan información sobre los requisitos iniciales para el diseño de cada caso de prueba


2. **Vistas selectivas dependientes del tipo de requisito**
	**Vista de documentos prospectivos.**
	- **Vista de gestión:** muestra los objetivos básicos del sistema y las relaciones para requisitos inferidos / derivados
	**Vista de comportamiento**
		Analista: transferir la descripción ( diagrama de estado) del comportamiento actual, a una descripción con otra forma (requisito funcional)
	**Vista de requisitos funcionales:**
	- Desarrolladores: base para la programación
	- Probador: Diseño de casos de prueba funcionales.
	- Diseñador de GUI: Diseña un sistema consistente de GUI basado en la descripción del comportamiento del sistema.
	- Editor técnico: seleccionar todos los requisitos relacionados a una entrega especifica del producto
	- Jefe del proyecto: selecciona requisitos de criticidad alta en el contexto de gestión del riesgo.
	- Diseño grafico: Busca requisitos relacionados con la GUI
	**Vista de grado de cobertura:**
		Jefe de rueba: cobertura de casos de prueba
	**Vista de la consistencia de la trazabilidad**
		Ing requisitos
	**Vista del estado de acutualizacion de trazas.**
		Los requisitos base han sido modificados? o los requisitos derivados requieren ser modificados?

--------
### **Lección 3: Priorización de requisitos**
- La mitad de todos los requisitos del sistema no son usados con posteridad.
- Diferente significado, impacto de priorización
- Satisfacción del cliente a través del desarrollo de los requisitos más importantes.
- Especialmente importante en enfoques iterativos e incrementales
- Aportación de atributos: necesario, deseado, opcional.
- Alto, medio, bajo son poco específicos.


Determinar los objetivos y restricciones. -> Definir criterios de priorización {
Coste de la implementacion
Consideraciones de riesgo
Daño causado por una implementación infructuosa
Volatilidad
Importancia
Duración
}
-> Determinar los implicados que deben involucrarse -> Seleccionar los artefactos


**Técnica ad-hoc**
- Clasificación, orden secuencial de los requisitos
- Los diez mejores ("top-ten")
**Clasificación por un criterio**
- Respecto del valor de un requisito para el éxito del sistema: obligatorio, opcional, es bueno tener.
**Clasificación de Kano**
- Requerido
- Opcional
- Conveniente
**Matriz de prioridad de Carl Woegers**


Prioridad = valor % / (costo % * peso relativo + riesgo % * peso riesgo)


----
#### Lección 4: Trazabilidad.
Una especificación de un requerimiento de sw es trazable si:
El origen de cada requerimiento está claro y si se facilita la referencia de cada requerimiento en el desarrollo futuro o en la documentacion
Es la capacidad d describir y de seguir la vida de un requisito tanto en direccion hacia adelante, y hacia atras. es decir, desde sus origenes a traves de su desarrollo y especifiaccion a us despliege y uso subsecuentes y a traves de periodos de refinamiento y de la iteracion en curso  en cualesquiera de estas fases


Beneficios:
Simplifica verificabilidad
Permite la identificacion de exceso de tamaño
En els sitema
En los requisitos
apoya el analisis de impacto 
apoya la reusabilidad de lasdefiniciones de erquisitos
apoy el aprovechamiento de recuross
Asignacion de esfuerzo
....

-------
Trazabilidad pre-requisitos
Relaciones de los requisitos con sus fuentes ejm: documento, vision de negocio
Entre - requisitos
Relaciones y dependencias entre requisitos
Post- requisitos
relaciones de los requisitos con artefactos que se desarollan. 

----------
Razones de usar trazabilidad.
1. Se dispone de informacion en la evaluacion de los cambios de requerimientos
2. Son la base para el control de costos y calidad
Importancia:
permite rasterar los requerimientos durante todo el desarrollo de producto sw
Ademas permite a prori conocer cuales serian las consecuencias  de cambiar o eliminar un requerimiento en el sistema, lo que en estrategias carentes de  trazabilidad, no se podía visualizar tan facilmente.

requisite pro

------
### Lección 5: Versionado de  requisitos.
Req 1 V1.3 -> Documento de requerimientos V1.1 <- Req 2 V1.0 / Req 3 V1.1

Construcción de versiones y gestión de versiones.
Unrequisito tienen una única versión de estado
La version de estado de un documento está comprendida por las versiones de los requisitos asociados.
La numeracion de versiones consistente, al menos de 2 partes: Versión e incremento.
Version: modificado como consecuencia de grandes cambios.
Incremento: cambios menores.

--------
Linea base de requisitos. ("requirement baseline")
Es la configuracion documentada de requisitos que de fora habitual comprende versiones estables de requisitos individuales.
1. Se documentan requisitos de una madurez especifica. 
2. Apoya las siguientes actividades en el proceso de desarrollo.
	1. Base para la planificación de entregas
	2. Estimación del esfuerzo de desarrollo
	3. Comparación de productos con los que compite.
3. Punto de inicio para solicitudes de cambio.