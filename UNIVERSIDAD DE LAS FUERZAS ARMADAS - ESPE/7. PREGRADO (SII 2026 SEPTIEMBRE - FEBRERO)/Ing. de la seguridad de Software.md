# UNIDAD I

## Conceptos básicos de seguridad informática

**Datos.-** Representación de hechos, valores o elementos que pueden ser procesados.

**Integridad.-** Propiedad que garantiza que la información se mantenga correcta, completa y sin modificaciones no autorizadas.

**Privacidad.-** Protección de la información personal para evitar su acceso, uso o divulgación no autorizada.

**Resguardo.-** Conjunto de medidas destinadas a proteger la información y los recursos frente a pérdida, daño, acceso no autorizado u otras amenazas.

**Garantía.-** Compromiso o mecanismo que busca asegurar que una condición, servicio o protección se cumpla de manera adecuada.

**Activo** .- Fuente de ingreso, valor en cualquier ámbito, importancia, beneficio, o que podría causar su ausencia.

**¿Qué tendría que proteger una universidad?**  
Computadores, servidores, información, sistemas, redes, bases de datos, cuentas, documentos, estudiantes, dinero, instalaciones.

**Seguridad.** Es la condición y el conjunto de medidas orientadas a proteger algo de situaciones que puedan afectarlo.

**Seguridad informática**.- La seguridad informática se ocupa de proteger la información y los sistemas informáticos que la procesan, almacenan y transmiten.

Ejemplo: Un sistema de matrícula.

Estudiante -> sistema de matrícula -> bd -> servidor -> red

Todos estos elementos participan en el tratamiento de información.

_La seguridad informática no consiste únicamente en proteger computadores._

**Dato:** Es una representación de un hecho, valor o elemento.

**Información:** Dato interpretado dentro de un contexto.

Una universidad puede manejar:

- Información académica
- Información financiera
- Información de docentes
- Información de estudiantes
- Investigación
- Contratos
- Credenciales
- Información administrativa.

¿Toda esa información tiene el mismo valor? No necesariamente.

**Sistema** Donde se encuentra o como se procesa la información.

**Sistema Informático** Conjunto de componentes que interactuan para procesar, almacenar, transmitir o utilizar información.

Sistema matrícula puede involucrar:

Aplicación web, BD, Servidores, Red, Computadores, Autenticación, almacenamiento, usuarios.

_La información depende del entorno._

**Activo** Que tiene valor para la organización,

Un **activo** es un elemento que tiene valor para una organización y q por ello puede requerir protección tiene valor pq contribuye al funcionamiento de un proceso, permite prestar un servicio contiene información procesa información o constituye un recurso necesario para la organización.

------
### Ejemplo: Sistema de matrícula universitaria

Un estudiante ingresa al **sistema de matrícula** para registrarse en sus asignaturas.

- **Dato:** `Jerson`, `Ingeniería de Software`, `Séptimo semestre`, `Aplicaciones Distribuidas`.
- **Información:** Los datos anteriores, interpretados dentro del contexto académico, indican qué estudiante es, qué carrera cursa y qué asignatura está matriculando.
- **Sistema:** El entorno donde se encuentra y procesa esta información.
- **Sistema informático:** Está compuesto por la aplicación web, servidores, base de datos, red, computadores, sistema de autenticación y usuarios.
- **Activo:** La base de datos, las cuentas de usuario, los servidores, la aplicación y la información académica son activos porque tienen valor para la universidad y son necesarios para prestar el servicio de matrícula.
- **Seguridad:** Se aplican medidas para proteger estos elementos frente a situaciones que puedan afectarlos.
- **Seguridad informática:** Protege específicamente la información y los componentes informáticos que la procesan, almacenan y transmiten.

**Flujo:**

`Estudiante → Aplicación de matrícula → Red → Servidor → Base de datos`

------------

## Confidencialidad, Integridad y Disponibilidad

**Confidencialidad**.- Garantiza que la información solo sea accesible para las personas, sistemas o procesos autorizados.

**Integridad** La confianza que se tiene sobre los datos, que no estén alterados. No exista modificación sin alguna autorización.

**Disponibilidad**.- Garantiza que la información y los recursos estén accesibles y funcionando cuando sean necesarios para los usuarios autorizados.

---

### Seguridad de la información

**Seguridad de la información.-** Protege la información sin importar si está en papel, voz, formato digital u otro medio.

La información puede encontrarse **almacenada, en procesamiento o transmitiéndose**, por lo que debe protegerse durante todo su ciclo de vida.

---

### Seguridad informática

**Seguridad informática.-** Protege sistemas, equipos, software, datos y recursos de TI.

**Seguridad informática:** proteger el sistema que procesa la información.

El sistema combina **personas, software, hardware, datos y recursos**.

Proteger el sistema implica evitar **acceso, modificación, interrupción o uso no autorizado**.

---

### Ciberseguridad

**Ciberseguridad.-** Protege las interacciones y los recursos en el entorno digital conectado, especialmente frente a amenazas que utilizan redes, Internet y sistemas interconectados.

Para un desarrollador, la ciberseguridad también aparece en las **APIs, autenticación, sesiones, datos y configuraciones**.

---

### Seguridad del software

**Seguridad del software.-** Una propiedad que se construye durante el ciclo de vida.

No se agrega al final, se integra en **requisitos, diseño, implementación, pruebas y operación**.

- **Requisitos.-** Qué elementos proteger y qué necesidades de seguridad existen.
- **Diseño.-** Límites y controles.
- **Código.-** Evitar fallos y vulnerabilidades.
- **Pruebas.-** Buscar debilidades.
- **Despliegue.-** Configurar seguro.
- **Operación.-** Corregir y aprender.

**Objetivo:** reducir vulnerabilidades, limitar su impacto y corregir causas raíz en el desarrollo.

-------
## Recurso, sistema y servicio

**Recurso, sistema y servicio:** 3 niveles diferentes.

**Recurso.-** Elemento que entrega valor o que es necesario para realizar una actividad.

**Sistema.-** Recursos organizados para procesar, almacenar y comunicar información.

**Servicio.-** Funcionalidad que un sistema ofrece a uno o varios usuarios para satisfacer una necesidad.

**Relación:**

**Recursos → Sistema → Servicio → Usuario**

Ejemplo:

- **Recurso:** Base de datos de estudiantes.
- **Sistema:** Sistema de matrícula.
- **Servicio:** Matrícula en línea.
- **Usuario:** Estudiante.

---

## Usuario, rol y privilegio

**Usuario.-** Persona, sistema o entidad que interactúa con un recurso o servicio.

**Rol.-** Conjunto de funciones o responsabilidades que determina qué acciones puede realizar un usuario.

**Privilegio.-** Permiso específico que permite realizar una acción sobre un recurso.

Ejemplo:

**Usuario:** Jerson  
**Rol:** Estudiante  
**Privilegio:** Consultar sus propias calificaciones.

---

## Control

**Control:** Una medida que modifica el riesgo.

El control actúa sobre el problema; no es una frase decorativa en una política.

**Problema:** Un estudiante puede solicitar el registro de otro.

**Control:** Verificar que el usuario actual sea el propietario del recurso o tenga los permisos necesarios.

**Resultado:** `403 Forbidden` — acceso no autorizado bloqueado.

---

## Evento e incidente

**Evento ≠ Incidente**

**Evento.-** Suceso observable que ocurre dentro de un sistema, servicio o entorno.

**Incidente.-** Evento o conjunto de eventos que compromete o amenaza de forma relevante la seguridad y requiere una respuesta.

**Todo incidente contiene eventos observables, pero no todo evento produce un impacto en la seguridad.**

Ejemplo:

**Inicio normal → Evento → Anomalía → Incidente → Respuesta**

Ejemplo práctico:

- Un usuario inicia sesión correctamente → **Evento**
- Se detectan 20 intentos fallidos desde una misma cuenta → **Anomalía**
- Se logra acceder a la cuenta sin autorización → **Incidente**
- Se bloquea la cuenta y se investiga lo ocurrido → **Respuesta**

**Idea clave:** No todo evento es un problema de seguridad; se habla de **incidente** cuando existe una afectación o amenaza relevante para la seguridad y es necesaria una respuesta.

Crear cuenta (contraseña segura)
Login básico, con 3 intentos máximos de acceso. 


-------
***05/11/2026***

**Seguridad informática.-** Protege sistemas, equipos, software, datos y recursos de TI.

**Seguridad de la información.-** Protege la información sin importar si está en papel, voz, formato digital u otro medio.

**Ciberseguridad.-** Protege las interacciones y los recursos en el entorno digital conectado.

**Seguridad del software.-** Una propiedad que se construye durante el ciclo de vida.

----------
Caso de software:
Una aplicación usa /api/notas/1001. El estudiante cambia el ID por 1002 y obtiene daos de otra persona. La aplicación sigue funcionado, pero la confidencialidad está comprometida.

Controles asociados:
- Autorización por recurso: (ejm)
- Control de acceso (ejm ambos están relacionados con la parte electrónica y programable)
- cifrado
- manejo adecuado de sesiones
- minimización de datos
 
**Integridad**
La integridad busca que la información y los sistemas mantengan exactitud, consistencia y ausencia de modifcaciones no autorizadas.

Caso de software
Si la API acepta directamente saldo = 9999 enviado por el cliente sin validación de autorización ni reglas de negocio, la integridad está en riesgo.

Controles asociados
- Validación del lado servidor
- Reglas de negocio
- Controles de autorización
- Transacciones
- Formas o verificaciones de integridad cuando corresponda

**Disponibilidad**
CIA No son 3 cajas aisladas, los 3 principios se relacionan entre sí:

Confidencialidad + integridad.
Un expediente médico no solo debe mantenerse privado; también debe estar correcto.
Ejemplo: Si un atacante puede leer un diagnóstico, se afecta confidencialmente. Si ademas se puede modificar, se afecta la integridad.

Integridad + Disponibilidad
Que un servicio esté up, no sirve si enrega datos incorrectos.
Un sistema bancario responde correctamente, pero muestra saldos alterados. Hay disponibilidad pero no integridad.

Confidencialidad+ Disponibilidad
Un sericio debe estar disponible para quien corresponde no para cualquier persona.
Ejm

Autorizar vs autenticar
autorizar: validación adicional para corroborar q el user es quien dice ser ?

-------
DEl triangulo al hexagono:
Parker amplia cia con posesion/control, autenticidad y utilidad para distinguir porblemas q CIA puede agrupal demasiado

Confiencialidad - posesion/control
Integridad - autenticidad
Disponibilidad - utilidad

Posesión/control
Se refiere a quien tiene control fisico o lógico sobre la información o el activo.
	Un ejemplo, un portátil corporativo cifrado es robado. Tal vez el ladrón no pueda leer los datos, por lo que la confidencialidad puede mantenerse. Sin embargo la organización perdió 
	posesion/control dispositivo

Autenticidad
Se refiere a 
.
.
.
CIA: Confiencialidad, integridad, disponibilidad. qn accede? esta correcto? está disponible?
Hexag: quien controla? , ..


-----
Miniquiz:
1. Un usuario consulta daots de otro usuario sin autorización. q propiedad se afecta
2.  Un pedido cambia de 50 a 500 $ sin autorizacion. Que propiedad se afecta?
3. El servicio está caido durante la matricula. ¿Qué propiedad se afecta?
	La Disponibilidad es afectada porque el servicio no se encuentra accesible cuando los usuarios lo necesitan
4. Un dispositivo cifrado es robado. Que propiedad adicional del Hexad ayuda a analizar el caso?
		La posesión/Control. Aunque la información permanezca cifrada y confidencial, el dispositivo físico ya no está bajo el control de su propietario.
	
5. Un respaldo existe pero no puede restaurarse q propiedad permite describir mejor el problema

------
## Autenticidad / trazabilidad

Autenticidad
Permite establecer que una identidad, entidad, mensaje, archivo o transacción es genuina y corresponder realmente a quien afirma ser. 

Ejemplo: Un usuario inicia sesión con sus credenciales y un segundo factor. EL sistema no solo recibe un nombre de usuario: intenta comprobar que la persona que se presenta como jsllumiquinga1 es realmente quien dice ser.

Riesgo
Si la autenticidad falla, un atacante puede hacerse pasar por otra persona servicio o sistema.

Trazabilidad
Permite registrar, reconstruir y seguir las acciones realizadas dentro de un sistema.
Un log es útil, debe tener:
-  Fecha y hora
-  Usuario o identidad
- Direccion ip o contexto de origen
- operacion realizada
- recurso afectado
- resultado
- identificador de correlacion cuando corresponda

-----
Responsabilidad
. . .

---
No repudio:
El no repudio busca disponer de evidencia suficiente para que una entidad no pueda negar posteriormente haber realizado una acción relevante.

EJemplos: 
- firma digital de un documento
- Aprobación registrada de una transferencia
- confirmación de una operacion con evidencia verificable
- ransaccion asociada a identidad, tiempo y mecanismos criptograficos

EL no repudio no es sinonimo de autenticidad o trazabilidad, se apoya de ellas.

-----
Amenaza, vulnerabilidad, riesgo y ataque
Modelo de analisis
activo / amenza / vulnerabilidad/ ataque / impacto / riesgo / control /verificacion

Activo:
ES aquello que tiene valor y debe protegerse.
	Credenciales, datos personales, apis, codigo fuente, disponibilidad de una aplicación, reputación

Amenaza:
Es una circunstancia, actor o evento con capacidad de causar daño a un activo.
	Cibrdelicuente, error humano, fallo eléctrico, malware, incendios
La amenaza puede existir aunque no haya ataque

Vulnerabilidad.
Es una debilidad ue puede ser aprovechada por una amenaza
	Contraseña debil, 










































