# Parcial I 

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





















