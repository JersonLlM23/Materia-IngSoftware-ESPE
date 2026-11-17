# Parcial I - Introducción a la Calidad de Software

## Introducción a la calidad del software
Qué es la calidad.- Capacidad de desarrollar diseñar manufacturar y mantener un producto de valor. Este producto debe ser el más económico el más útil y satisfactorio para el consumidor final. *Dar valor a algo*
La calidad del sw muestra qué tan bueno y confiable es un producto. Para transcmitir un ejemplo de titulo asociado, piense en un sw funcionalmente correcto.

La calidad de un producto de se implica que hay un modelo de calidad adyacente que define un conjunto de caracteristicas de producto.

*"Capacidad de un producto de sw para cumplir funciones esperadas baajo condicioines definididas"*

Conjunto de caracteristicas que determinan la capacidad de un producto sw para satisfacer necesidades explicitas e implicitas, incluyendo funcionalidad, fiabilidad, usabilidad, eficiencia, mantenibilidad y portabilidad evaluadas bajo condiciones especificas y numeradas con estandares como ISO 25010

----
Según la norma ISO IEC 25010 el concepto de calidad del sw se divide en varias caracteristicas.

Funcionaldiad.- El sw hace lo q se supone q debe hacer 9.5/10
Usabilidad.- Es fácil de entender, aprender, y usar. 8.5/10
Mantenibilidad.- Es fácil de modificar, corregir y mejorar 8.5/10
Fiabilidad El sw mantiene un nivel de rendimiento especificado sin fallos en condiciones normales 9/10
Rendimiento.- sa eficientemente los recursos bajo condiciones especificas
Portabilidad.- Puede funcionar en any entorno 7.5


-------
Informe del caos.
El informe de caos viene siendo publicado por standish group desde 1994 dando una vision sobre el fracaso o exito de los proyectos
En el informe de 2015, han estudiado 50 000 proyectos desde los más pequeños hasta los más grandes.

----
La mayoría de los clientes busca calidad al mejor precio, sin embargo, lo que puede verse "excelente" para algunos, no lo es para otros. Cuando un individuo adquiere un producto o servicio lo hace para satisfacer una necesidad, pero siempre espera que la nueva adquisición funcione como lo esperado o al menos como se los prometieron.

*Lo barato sale caro*


----
Cómo lograr que el consumidor se convierta en nuestro cliente.
Calidad que se espera:
Se da cuando existen propiedades y características que los consumidores dan por sentado que econtnraran en los productos o servicios. Cuando encuentran esto, se sienten satisfechos pero si no, pailas.

Calidad que satisface.-  Se da cuando existen propiedades y características que los consumidores solicitan especificamente. 

Calidad que deleita.- Se da cuando existen propiedades caracteristicas q los consumidores no solicitan pero satisfacen


--------
CALIDAD:
Conjunto de actividades que permiten satisfacer necesidades de un colectivo.
Grado en el que un conjunto de características cumple con los req
Satisfaccion del cliente y cobformidad con sus req
Grado de satisfacción que produce el cliente

-----
Evolución:
1960
En las primeras etapas, el sw se desarrollaba sin metodologias formales
La calidad se media por la ausencia de errores
El enfoque era reaccionario, corregir errores despues de su deteccion
Surgieron problemas como el "crisis del sw" por proyectos q excedían presupuestos y plazos.

----
Los requisitos de sw son la base de las medidas de calidad.
Empacto estratégico. Oportunidad de ventaja competitiva.
Planificación, fijación de objetivos, coordinación, formación y adaptación para toda la organización
Una filosofía, una cultura, una estrategia, un estilo de gerencia de la empresa.

------
DEfinición del término costo.
uh

Costes de las pruebas.- Costes derivados de probar el sw para evitar los defectos lleguen a producción
Prevencion.- Costes derivados de mejorar los procesos de desarrollo (herramientas, técnicas, arquitectura, métodos, prácticas) y de capacitación de las personas (formación) para minimizar la inyección de defectos de sw
Costos de fallo interno 
Costes de fallo en producción

-----
Costos de sw
Costos para asegurar la calidad o costos de 
COstos por falta de calidad o costos de no conformidad

Costos de prevencion, evaluacion, fallas internas, fallas externas


---------
1970> pruebas manuales y correcion de errores
1983> ieee 730 estandar que grantiza la calidad
1991 cmm nivel 5 madurez de procesos
1995 ISO 2196 mantenibilidad / portabilidad
2001 metodlogia agiles
2010 DEvops + ci/cd integracion de la calidad
2015 Automatizacion masiva de pruebas
2020 IA y monitoreo predictivo en calidad

------
Uno de los factores para promover un proceso de mejoramiento continuo de la calidad consiste en recopilar, documentar, y usar la informacion sobre los costos relacionados con la calidad.

---
## Factores clave de calidad del software
- Funcionalidad.- Cumple con lo que el usuario necesita > presicion, interoperatibilidad, seguridad funcional
- Rendimiento / eficiencia> uso eficiente de recursos 
- Usabilidad > facil de aprender y usar
- Confiabilidad > funciona sin fallos durante tiempo prolongado
- Seguridad >resiste accesos no autorizados
- Mantenibilidad facil de modificar corregir o mejorar
- Portabilidad > se adapta a diferentes entornos.

-----
## Como se mide la calidad del software
- Pruebas automatizadas: Cobertura de código (% de líneas probadas), número de bugs encontrados vs resueltos. 
- Métricas técnicas.- Tiempo de respuesta <2 seg es ideal, uso de cpu/memoria bajo condiciones máximas, rendimiento en pruebas de carga (ejm: 1000 users)
- Prácticas de desarrollo: Integración continua CI/CD, REvisiones de code, uso de estándares (SOLID)
- UX: tiempo promedio para completar una tarea, tasa de abandono en procesos clave, encuestaas de satisfacciòn (NPS, CSAT)

----
## Aseguramiento de la calidad (SQA)
### Aseguramiento de la calidad 
Es el conjunto de acividades planificadas y sistematicas neceasrias para aportar la confianza que el sw satisfara los req dados de calidad. ESte aseguraimiento se dseña para cada aplicacion antes de comenzar a desarrollarla y no despues. El aseguramiento de la calidad del sw engloba:

**Técnicas de aseguramiento de la calidad**
Las técnicas de adminsitracion de calidad de sw pueden ser clasificadas en muchos sentidos: entaticas, personales-intensivas, analiticas y dinamicas.
TEcnicnas para evaluacion de la calidad:
Las mediciones que se realizan sobre la calidad pueden tener . . .


Aseguramiento de la calida SQA:
Proceso sistemataico para garantizar q el sw cumpla con reeq funcionales y no funcionales.
OBJETIVOS:
- detectar errores temprano
- mejorar experiencia del user
- reducir scostos de mantenimiento
enfoques modernos, automaticacion ci/cd , IA

- Enfoque de gestion de claidad
- metodos y herramientas dentro de ing sw
- revisiones tecnicas formales aplicables en el proceso de sw
- usna estrategia de prueba multiescala
- el control de la documentacion del sw y de los cmabios realizados
- procedimientos para ajustarse a los estandares de desarrollo del sw
- mecanismos de medicion y generacion de informes

**Portabilidad, usabilidad, reusabilidad, correcteness, mantanibildiad, error control**


------
Quality assurance QA: Mejoramiento continuo por medio de plan, do, check, act process
La mejora continua es un esfuerzo continuo para mejorar productos, servicios o procesos.
Estos esfuerzaos pueden buscar una mejora inceremental a lo largo del tiempo o una mejora revolucionaria de una sola vez.
PDCA Deming es la herramienta mas usada ara la mejora continua.

QUE ES CYCLE PDCA


-----
TECNIAS PARA EL ASEGURAMIENTO
TEcnincas estaticas:
se aplican sin sjecutar el code - enfocadas en prevenir defectos (revision code, analisis estatico)
tecnicas dinamicas: 
requieren ejecucion del sw - enfocadas en detectar defectos (preubas unitarias, pruebas de cargas)



Tecnicas estaticas: prevencion antes de la ejecucion
anlisis delsw sin ejecutarlo, enfocado en encontrar errores en diseño arquitectura codigo fuente o documentacion
Tipos principales:
reiciones tecnicas (inspecciones, recision por pares)
analisis estatido de codigo SAST
metricas de calidad (complejidad, duplicacion

ventajas: detectar errores temprano, reducen costos de correcion, nmejorar legibildida y mantenibilidd.
Por ejm: usar pylint para revisar un script python antes de su ejeccion)





**JUEVES PRUEBA LOL**





















# Parcial II - Estándares para Calidad del Proceso

### **Qué es una entidad muy pequeña (VSE)?**

- **$\le 25$ personas**
    
- **Una VSE** _(Very Small Entity)_ o pequeña organización (PO) **desarrolla sistemas o software con un equipo de hasta 25 personas**.
    

**Tipos de entidades:**

- **Empresa pequeña:** Microempresas y emprendimientos de software o de sistemas.
    
- **Organización:** Entidades públicas, ONG o universidades con equipos reducidos.
    
- **Departamento o área:** Unidad de TI dentro de una empresa grande.
    
- **Proyecto o equipo:** Proyecto puntual con un equipo pequeño, aun en una gran empresa.


---
### **Desarrollo de software: los desafíos de siempre**
- **40–50 %** del tiempo de los especialistas se va en retrabajo evitable, en lugar de hacer las cosas bien al primer intento.    
- _Si no cambiamos nada, la situación no mejorará._

**Objetivos / Desafíos:**
- **Más rápido:** Ciclos de entrega más cortos.
    
- **Mejor calidad:** Menos defectos en producción.
    
- **Más barato:** Sin excesos de presupuesto.
    
- **Sin retrasos:** Cumplir el calendario pactado.
    
- **Más productividad:** Menos esfuerzo desperdiciado.
    
- **Primero al mercado:** Ventaja competitiva real.
    
_(Fuente del costo de retrabajo: Charette (2005), se mantiene por su valor histórico y su vigencia como referencia)_


----
### **Micro y pequeñas empresas: el 99 % del total**

- **Unión Europea (2022) (32,3 millones de empresas):**
    
    - **Micro y pequeñas:** 99.0 % de empresas | 48.0 % del empleo
        
    - **Medianas:** 0.8 % de empresas | 15.0 % del empleo
        
    - **Grandes:** 0.2 % de empresas | 37.0 % del empleo
        

**Datos destacados:**

- **Unión Europea:** Las micro y pequeñas empresas (hasta 49 personas) son el 99 % de las empresas y emplean al 48 % de los trabajadores (Eurostat, 2024).
    
- **Ecuador:** 1 228 415 empresas registradas en 2022; en Quito, cerca del 93 % son microempresas (INEC, s. f.).
    

_(Datos: Eurostat (2024), año de referencia 2022; INEC (s. f.), Directorio de Empresas 2022)_

-----

### **Las VSE están en toda la cadena de suministro**

- **Pirámide de la cadena de suministro:**
    
    - **1 Fabricante**
        
    - **60 Proveedores prime**
        
    - **600 Proveedores**
        
    - **$\approx 6\,000$ Productores (VSE)**
        

**Datos e implicaciones:**

- **> US$ 200 millones** de pérdida para un fabricante de electrónica por un defecto de software introducido por uno de sus $\approx 6\,000$ productores (Shintani, 2006, citado en Laporte, 2016).
    
- **La calidad del producto final depende de los eslabones más pequeños:** hay VSE en casi todas las organizaciones.

----------
### **¿Por qué las VSE no usan normas?**

- **Motivos declarados (% de respuestas):**
    
    - **28 %**: Falta de recursos
        
    - **24 %**: No lo necesitan
        
    - **15 %**: Normas difíciles o burocráticas
        
    - **9 %**: Toma demasiado tiempo
        
    - (Otros porcentajes menores visibles en la gráfica para "Otro" y "Falta de apoyo").
        

### **Estadísticas destacadas:**

- **18 %** de las VSE estaban certificadas (frente a más del 53 % de las grandes).
    
- **74 %** considera importante ser reconocida o certificada.
    
- **62 %** pide más orientación y ejemplos.
    
- **55 %** pide normas «ligeras», fáciles y con plantillas.
    

(Encuesta internacional del WG 24: más de 435 respuestas de 32 países, cuestionario en 9 idiomas [Laporte, 2016])

------
### **¿Quién elabora la ISO/IEC 29110?**

- **ISO/IEC JTC 1**: Comité técnico conjunto para estándares de tecnologías de la información.
    
- **Subcomité SC 7**: Ingeniería de software y de sistemas: procesos, herramientas y tecnologías de soporte.
    
- **Grupo de Trabajo WG 24**: Perfiles de ciclo de vida para entidades muy pequeñas (serie 29110).
    

**Participación internacional:**

- Delegaciones nacionales de América, Europa, Asia y África (Argentina, Brasil, Canadá, Colombia, México, Perú, España, Japón, Tailandia, entre otras).
    
- Organizaciones de enlace: INCOSE, AFIS e IEEE.
    
- La norma mexicana MoProSoft (NMX-I-059-NYCE) fue una de sus bases (Laporte, 2016).
-----
### **Estrategia del WG 24: perfiles progresivos**
- Un perfil es un conjunto de normas base adaptadas para cumplir una función concreta. El Grupo de Perfiles Genérico se dirige a VSE que no desarrollan software crítico.
    
**Niveles de perfiles:**

- **Entrada:** Proyectos pequeños ($\approx 6$ personas-mes) o emprendimientos que inician.
    
- **Básico:** VSE que desarrolla un solo proyecto a la vez.
    
- **Intermedio:** Varios proyectos en paralelo en el contexto de la organización.
    
- **Avanzado:** VSE que quiere sostenerse y crecer como empresa independiente y competitiva.
    
_(Además existen perfiles para ingeniería de sistemas (hardware + software) y para prestación de servicios [Laporte, 2016])._


----

### **Mapa de la familia ISO/IEC 29110**



- **Visión general y vocabulario:**
    
      
    - 29110-1-1 y 1-2 (2024): conceptos, taxonomía y términos comunes. Punto de partida para todos.
        
          
        
- **Perfiles: «qué hacer»**
    
      
    - 29110-2 (marco y taxonomía), 29110-4 (requisitos de perfiles genéricos) y 29110-6 (perfiles específicos).
        
          
        
- **Evaluación y certificación:**
    
      
    - 29110-3-x: guías y esquemas para evaluadores, certificadores y las propias VSE.
        
          
        
- **Guías: «cómo hacerlo»**
    
      
    - 29110-5 (guías genéricas de gestión, ingeniería y servicios) y 29110-7 (guías específicas).
        
          
        

_(Figura: estructura de la serie ISO/IEC 29110 según su nueva numeración [ISO/IEC, 2024a])._


----

### **Documentos clave y su edición vigente**

|**Parte**|**Título (resumido)**|**Edición**|**Nota**|
|---|---|---|---|
|**29110-1-1**|Visión general|2024|Reemplaza al TR 29110-1:2016; descarga gratuita en ISO|
|**29110-1-2**|Vocabulario|2024|Términos comunes de toda la serie|
|**29110-2-1**|Marco y taxonomía de perfiles|2015|Para productores de normas|
|**29110-3-1**|Guía de evaluación|2020|Para evaluadores y VSE|
|**29110-3-3**|Esquema de certificación de conformidad|2018 + Amd 1:2025|La enmienda elimina el requisito de recertificar cada 3 años|
|**29110-4-1**|Especificaciones de perfiles de software|2018|Referencia normativa para certificar|
|**29110-5-1-1 / 5-1-2**|Guías de software: Entrada / Básico|2012 / 2011|Disponibles sin costo como TR|
|**29110-5-1-3 / 5-1-4**|Guías de software: Intermedio / Avanzado|2017 / 2018|Gestión de varios proyectos y de la organización|
|**29110-5-3**|Guía de prestación de servicios|2018|Para VSE que operan servicios de TI|
|**29110-5-4**|Guía de desarrollo ágil de software|2025|73 páginas; integra eventos ágiles con el Perfil Básico|
|**29110-5-6-1 / 5-6-2**|Ingeniería de sistemas: Entrada / Básico|2015 / 2014|Productos con hardware y software|

_(Fuentes: catálogo ISO [ISO/IEC, 2024a, 2024b, 2025a, 2025b] y Laporte [2016])._

------

### **Documentos según su audiencia**

  

  

- **«Qué hacer»**
    
      
    - **Especificaciones de perfil (Parte 4)**
        
          
        
    - Lista de requisitos normativos. Audiencia: productores de normas, proveedores de herramientas y metodologías, organismos certificadores.
        
          
        
- **Evaluar**
    
      
    - **Evaluación y certificación (Parte 3)**
        
          
        
    - Cómo comprobar la conformidad de un proceso o de una VSE. Audiencia: evaluadores, auditores y VSE.
        
          
        
- **«Cómo hacerlo»**
    
      
    - **Guías de gestión e ingeniería (Parte 5)**
        
          
        
    - Procesos, actividades, tareas, roles y productos listos para aplicar. Audiencia principal: las VSE.
        
          
        

_(Varias guías técnicas [TR] pueden descargarse sin costo en ISO Publicly Available Standards [Laporte, 2016])._

----
### **Perfil Básico: visión de conjunto**

**Flujo con el Cliente y Gestión:**

- **Cliente** $\rightarrow$ **Enunciado del trabajo** $\rightarrow$ **Proceso de Gestión del Proyecto (GP)**
    
      
    
- **Proceso de Gestión del Proyecto (GP)** $\rightarrow$ **Configuración de software** $\rightarrow$ **Cliente**
    
      
    
- Base: **Gestión de la VSE**
    
      
    

**Proceso de Gestión del Proyecto (GP):** _(interactúa bidireccionalmente con IS)_

  

- **GP.1** Planificación
    
      
    
- **GP.2** Ejecución del plan
    
      
    
- **GP.3** Evaluación y control
    
      
    
- **GP.4** Cierre
    
      
    

**Proceso de Implementación de Software (IS):**

  

- **IS.1** Inicio de la implementación
    
      
    
- **IS.2** Análisis de requisitos
    
      
    
- **IS.3** Arquitectura y diseño detallado
    
      
    
- **IS.4** Construcción
    
      
    
- **IS.5** Integración y pruebas
    
      
    
- **IS.6** Entrega del producto
    
      
    

_(La serie no excluye ningún ciclo de vida: cascada, iterativo, incremental, evolutivo o ágil [Laporte, 2016])._

-----

### **Proceso de Gestión del Proyecto (GP)**

  

  

- **GP.1 Planificación**
    
      
    - **Entrada:** Enunciado del trabajo
        
          
        
    - **Salidas:** Plan del proyecto, repositorio del proyecto, acta de reunión
        
          
        
- **GP.2 Ejecución del plan**
    
      
    - **Usa:** Plan del proyecto
        
          
        
    - **Salidas:** reportes de avance, actas, respaldo del repositorio
        
          
        
- **GP.3 Evaluación y control**
    
      
    - Compara avance real vs. plan
        
          
        
    - **Salidas:** acciones correctivas, solicitudes de cambio
        
          
        
- **GP.4 Cierre**
    
      
    - Entrega formal al cliente
        
          
        
    - **Salidas:** acta de aceptación, configuración de software
        
          
        

_(GP.3 retroalimenta a GP.2: las acciones correctivas y los cambios aprobados vuelven al plan [Laporte, 2016])._

---
### **Proceso de Implementación de Software (IS)**

- **IS.1 Inicio:** Revisión del plan con el equipo de trabajo.
    
- **IS.2 Requisitos:** Especificación de requisitos verificada y validada.
    
- **IS.3 Arquitectura y diseño:** Diseño de software y trazabilidad.
    
- **IS.4 Construcción:** Componentes y pruebas unitarias.
    
- **IS.5 Integración y pruebas:** Casos, procedimientos e informe de pruebas.
    
- **IS.6 Entrega:** Configuración de software, guías de usuario y mantenimiento.
    

**Nota clave:**

- **Verificación y validación en cada actividad:** el producto de trabajo se revisa (verificación) y el cliente confirma que responde a su necesidad (validación) antes de avanzar.
-

-------

### **Así se describe una tarea en la norma**

|**Rol**|**Tarea**|**Producto de entrada**|**Producto de salida**|
|---|---|---|---|
|**GP, LT**|GP.1.1 Revisar el Enunciado del trabajo|Enunciado del trabajo|Enunciado del trabajo [revisado]|
|**GP, CL**|GP.1.2 Definir con el cliente las instrucciones de entrega de cada entregable del Enunciado del trabajo|Enunciado del trabajo [revisado]|Plan del proyecto: instrucciones de entrega|
|**CL, AN**|IS.2.4 Validar y obtener la aprobación de la Especificación de requisitos (incluye usabilidad de la interfaz); se corrige hasta que el cliente la aprueba|Especificación de requisitos [verificada]|Resultado de validación; Especificación de requisitos [validada]|

**Roles:**

  

- **GP:** Gestor del proyecto
    
      
    
- **LT:** Líder técnico
    
      
    
- **CL:** Cliente
    
      
    
- **AN:** Analista



------

### **Roles del Perfil Básico**

  

  

- **Cliente (CL):** Define necesidades, valida y acepta entregables.
    
      
    
- **Gestor del proyecto (GP):** Planifica, controla y cierra el proyecto.
    
      
    
- **Líder técnico (LT):** Dirige las decisiones técnicas del equipo.
    
      
    
- **Analista (AN):** Obtiene, especifica y valida requisitos.
    
      
    
- **Diseñador (DIS):** Define arquitectura y diseño detallado.
    
      
    
- **Programador (PR):** Construye componentes y pruebas unitarias.
    
      
    
- **Equipo de trabajo (ET):** Participa en revisiones, integración y pruebas.
    
      
    

_(En una VSE la misma persona puede asumir varios roles, siempre que tenga la competencia requerida [Laporte, 2016])._


-----
### **Producto de trabajo: la Solicitud de cambio**

  
- **Definición:** Requerimiento de una modificación para corregir un problema o incorporar una mejora en el software o en su documentación.
    
      
    
- **Origen:**
    
      
    - Implementación de software
        
          
        
    - Cliente
        
          
        
    - Gestión del proyecto
        
          
        
- **Estados aplicables:** Propuesta $\rightarrow$ Evaluada $\rightarrow$ Aceptada
    
      
    

**Información que puede contener:**

  

- Propósito del cambio
    
      
    
- Estado de la solicitud
    
      
    
- Datos de contacto del solicitante
    
      
    
- Sistema(s) afectado(s)
    
      
    
- Impacto en la operación de sistemas existentes
    
      
    
- Impacto en la documentación asociada
    
      
    
- Criticidad de la solicitud y fecha requerida


-------
### **ISO/IEC 29110 y agilidad: la nueva guía 5-4:2025**

  

  

- **29110-5-4:**
    
      
    - Publicada en septiembre de 2025 (73 p.).
        
          
        
    - Orienta a las VSE que quieren reforzar su entorno ágil usando las prácticas de la serie 29110. Aplica a VSE que no desarrollan productos críticos para el negocio o para la seguridad (ISO/IEC, 2025b).
        
          
        

**Correspondencia orientativa entre eventos ágiles y el Perfil Básico:**

  

- **Planificación del sprint** $\rightarrow$ GP.1 / GP.2: tareas, estimación, calendario.
    
      
    
- **Daily scrum** $\rightarrow$ GP.2 / GP.3: avance, impedimentos, acciones.
    
      
    
- **Revisión del sprint** $\rightarrow$ GP.3 e IS.2.4: validación con el cliente.
    
      
    
- **Retrospectiva** $\rightarrow$ GP.3: acciones correctivas y mejora del proceso.
    
      
    
- **Incremento del producto** $\rightarrow$ IS.4 a IS.6: construcción, pruebas y entrega.
    
      
    

(La correspondencia es un apoyo didáctico; la guía oficial detalla eventos, tareas y resultados [GP, IS, O] que cada uno cubre).


-----

### **Certificación de conformidad ISO/IEC 29110**

- **1. Solicitud:** La VSE pide la certificación a un organismo acreditado.
    
- **2. Certificación Inicial:** Auditoría de proceso frente a 29110-4-1.
    
- **3. Vigilancia:** Auditorías de seguimiento periódicas.
 
- **4. Renovación:** Desde la Amd 1:2025 ya no se exige recertificar cada 3 años.


**Detalles complementarios:**

  

- **Base normativa:** Esquema de producto/proceso conforme a ISO/IEC 17065 (requisitos para organismos que certifican productos, procesos y servicios).
    
      
    
- **Reconocimiento:** Certificados reconocidos en los países miembros del IAF, mediante los acuerdos de reconocimiento multilateral.
    
      
    
- **Ejemplo reciente:** iApp Technology (Tailandia) obtuvo la certificación bajo 29110-4-1:2018 el 12 de marzo de 2025 (iApp Technology, 2025).


---
### **Paquetes de despliegue (DP)**
- **Qué es un DP:**
    - Conjunto de artefactos que facilita implementar un grupo de prácticas en una VSE sin adoptar todo el marco a la vez.
        
- **Contenido típico:**
    
      
    - Descripción de procesos, tareas y roles.
        
          
        
    - Plantillas, ejemplos y listas de verificación.
        
          
        
    - Herramientas sugeridas.
        
          
        
    - Correspondencia con ISO 9001, ISO/IEC/IEEE 12207 y CMMI-DEV.
        
          
        

**Áreas / Paquetes representados:**

  

- Gestión del proyecto
    
      
    
- Análisis de requisitos
    
      
    
- Arquitectura y diseño detallado
    
      
    
- Construcción y pruebas unitarias
    
      
    
- Integración y pruebas
    
      
    
- Verificación y validación
    
      
    
- Control de versiones
    
      
    
- Entrega del producto
    
      
    
- Autoevaluación
    
      
    

_(Acceso libre versión en español del Perfil Básico traducida por la Universidad Peruana de Ciencias Aplicadas [Laporte, 2016])._


-----

### **Caso 1 · BitPerfect, emprendimiento de TI en Perú**

  

  

- **Esfuerzo del proyecto: 882 horas**
    
      
    - **585:** Ejecución
        
          
        
    - **159:** Corrección de defectos
        
          
        
    - **124:** Revisión
        
          
        
    - **14:** Prevención
        
          
        

**Datos clave y resultados:**

  

- **4 $\rightarrow$ 23** personas entre 2012 y 2016.
    
      
    
- **6 sprints** de una semana, con enfoque ágil.
    
      
    
- **18 %** de retrabajo (159 de 882 h).
    
      
    
- **Julio 2014:** primera VSE peruana certificada (auditor de ABNT, Brasil).
    
      
    

_Proyecto: sistema de consulta legal para una aseguradora. La certificación facilitó el acceso a clientes nuevos y proyectos de mayor tamaño._

  

_(Fuente: García [2015])._

----

### **Caso 4 · CSiT, empresa joven de transporte (Canadá)**

- **Problema:** Clientes de transporte público (p. ej., metros) exigían CMMI nivel 2; con 4 personas (2012) eso era demasiado exigente.
    
      
    
- **Estrategia:** Implantar el Perfil Básico de Ingeniería de Sistemas 29110 como base y completarlo con el INCOSE Handbook, PMBOK y CMMI.
    
      
    
- **Resultado:** Análisis de brechas CMMI–29110 y prácticas añadidas para una evaluación CMMI nivel 2 exitosa; 10 personas en 2016.
    
      
    

**Tabla comparativa de proyectos:**

  

||**Ligero**|**Estándar**|**Completo**|
|---|---|---|---|
|**Tipo de proyecto**|Prueba de concepto o prototipo (pequeño)|Proyecto típico instalado en el cliente (mediano)|Cliente exige CMMI nivel 2 (grande)|
|**Marco**|29110-5-6-1 Entrada + CMMI SAM|29110-5-6-2 Básico + CMMI SAM|CMMI nivel 2|

_(SAM: Supplier Agreement Management [gestión de acuerdos con proveedores] de CMMI)._

  

**Crecimiento:**

  

- **4 $\rightarrow$ 10 personas** entre 2012 y 2016, con procesos escalados según el tamaño del proyecto.
    
      
    

_(Fuente: Laporte [2016])._


------


  

### **Conclusiones**

- **Hecha para VSE:** Diseñada para equipos de hasta 25 personas que no tienen tiempo, presupuesto ni conocimiento para adaptar ISO 12207 o 15288.
    
      
    
- **Progresiva:** Perfiles Entrada, Básico, Intermedio y Avanzado, más perfiles de sistemas y de servicios.
    
      EXAMEN PQ NO TAL ROL PARA TAL PROYECTO
    
- **Compatible con ágil:** No impone ciclo de vida; la guía 5-4:2025 la integra con prácticas ágiles.
    
      
    
- **Beneficios medibles:** Menos incidentes, retrabajo controlado y retorno económico en los casos estudiados.
    
      
    
- **Certificable:** Esquema de conformidad actualizado en 2025 y reconocimiento internacional.
    
      
    
- **Apoyo abierto:** Guías TR y paquetes de despliegue gratuitos facilitan su adopción.






-----
## Actividades del perfil básico
1. Elegir el perfil
2. Revisar el enunciado del trabajo
3. Armar el plan del proyecto
4. Validar requisitos con el cliente
5. Gestionar una solicitud de cambio
6. Medir el retrabajo y cerrar
	cual seria el porcentaje de tamaño tuvo el proyecto 
	y como se cierra este trabajo formalmente?
	Porcentaje de trabajo = (horas de trabajo / horas totales ) * 100 