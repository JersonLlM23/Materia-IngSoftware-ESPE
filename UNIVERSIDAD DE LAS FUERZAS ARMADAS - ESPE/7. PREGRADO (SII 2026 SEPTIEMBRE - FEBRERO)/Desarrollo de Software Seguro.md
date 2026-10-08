*

ENTORNOS GREENFILE
Iniciar desde 0, desde los requisitos hasta 
—---------

Desarrollo de sw seg

  

Estudio de vulnerabilidades.

La seguridad del sw

es una disciplina que protege las aplicaciones a lo largo de todo su ciclo de vida para reducir vulnerabilidades y el riesgo operativo

  

1. Requisitos.- Integrar requisitos de seguridad desde el inicio considerando riesgos y cumplimiento.
    
2. Diseño.- Aplicar principios de seguridad y definir controles en la arquitectura y diseño
    
3. Implementación.- Desarrollar código seguro, realizar revisiones y pruebas estáticas/dinámicas para detectar fallas.
    
4. Despliegue.- Configurar entornos de forma segura, gestionar dependencias y aplicar controles de liberación
    
5. Operación.- Monitorear, detectar incidentes, gestionar vulnerabilidades y mantener mejoras continuas.
    

  

pq importa.- reduce el riesgo de perdidas economicas, interrupciones del servicio y daños a la confianza de los usuarios.

q se protege.- activos del sw: datos, servicios, procesos, y reputación de la organización.

frente a que.- amenazas como errores de desarrollo, ataques maliciosos, malas configuraciones, y dependencias de terceros.

como se logra.- mediante controles de seguridad: prevención, detección, respuesta y recuperación.

  

La seguridad del software es transversal al ciclo de vida y no una actividad aislada.

  

DTO

DevOP

  
  

Ciclo de vida del desarrollo de sw SDLC con seguridad

1. Requisitos 
    

2. Requisitos de seguridad
    

3. Diseño
    

4. Modelado de amenazas y arquitectura segura
    

5. Desarrollo
    

6. Codificación segura y revisión
    

7. Pruebas
    

8. SAST, DAST, pruebas funcionales de seguridad
    

9. Despliegue
    

10. Hardening e infraestructura segura.
    

11. Operación
    

12. Monitoreo, parches y respuestas a incidentes.
    

  

Beneficios de integrar seguridad temprano:

Incorporar la seguridad desde las primeras etapas de SDLC proporciona importantes ventajas:

Menor coste, menor retrabajo, makro exposición, mayor confiabilidad.

  

Integrar seguridad desde el inicio del SDLC reduce vulnerabilidades y costes de corrección.

  

Amenazas, vulneabilidaes, riesgos, y controles.

  

1. Activo (cualquier elemento de valor para la orgnanización como datos, sw, servicios. procesos o infraestructura)
    
2. Vulnerabilidad (Debilidad en el sw la configuración o el proceso que puede ser explotada por una amenaza)
    
3. Amenaza (Entidad, evento o condición que podría explotar una vulnerabilidad para causar un daño al activo)
    
4. Riesgo (Probabilidad de que ocurra una amenaza y el impacto que genera sobre el activo si se explota la vulnerabilidad)
    
5. Control (medida administrativa, técnica o física que reduce la probabilidad de que se explote la vulnerabilidad o el impacto del riesgo)
    

  

Ejemplo práctico: Formulario web público

Activo ( aplicación web y datos de los mensajes)

Vulnerabilidad (Validación de entrada débil por ejm: campos sin sanitizar)

Amenaza (Atacante externo que envía entradas maliciosas, como inyección de código)

Riesgo (Acceso no autorizado o alteración de datos de la aplicación)

Control (Validación de entradas WAF Web Application Firewall y consultas parametrizadas)

  

Exposición: Una vulnerabilidad expone al activo a una amenaza

Impacto: El riesgo considera el posible daño sobre el activo.

Probabilidad: Depende de la existencia de la amenaza y de la facilidad de explotación de la vulnerabilidad.

Mitigación: Los controles reducen la probabilidad y/o el impacto del riesgo.

  

El riesgo aparece cuando una amenaza puede explotar una vulnerabilidad sobre un activo; los controles reducen probabilidad o impacto.
  
  

Activo | Tipo | Consecuencia de …. (q pasa si los datos del usuario son modificados)

Datos de usuarios, credenciales | información, información sensible

  
**

---------
Software vs Programa vs Sistema


Qué es la seguridad del sw
Disciplina orientada a diseñar, desarrollar, desplegar y mantener sw capaz de resistri ataques, errores y condiciones adversas, reduciendo vulnerabilidades y riesgo.

Seguridad del sw
Propuedades y prácticas incorporadas al producto de software para prevenir, detectar y responder a amenazas.

Ciberseguridad
Protección del ecosistema digital frente  a amenazas, ataques y riesgos que afecta a personas, organizaciones y sistemas.

Seguridad de aplicaciones.
Protección de aplicaciones durante su ciclo de vida (desarrollo, pruebas, despliegue, y ejecución para evitar y mitigar vulnerabilidades)Software vs Programa vs Sistema


Qué es la seguridad del sw
Disciplina orientada a diseñar, desarrollar, desplegar y mantener sw capaz de resistri ataques, errores y condiciones adversas, reduciendo vulnerabilidades y riesgo.

Seguridad del sw
Propuedades y prácticas incorporadas al producto de software para prevenir, detectar y responder a amenazas.

Ciberseguridad
Protección del ecosistema digital frente  a amenazas, ataques y riesgos que afecta a personas, organizaciones y sistemas.

Seguridad de aplicaciones.
Protección de aplicaciones durante su ciclo de vida (desarrollo, pruebas, despliegue, y ejecución para evitar y mitigar vulnerabilidades)

Seguridad de la información
Protección de la confidencialidad, integridad y disponibilidad de la información independientemente del medio o formato.

no usar d1 con wifi gratis.

La seguridad debe diseñarse, no añadirse al final.

---------

RELACIÓN CON OTRAS DISIPLINAS:
Seguridad del software:
Se centra en el producto y su ciclo de vida.
Busca prevenir, identificar, mitigar vulnerabilidades a lo largo de todo el ciclo de vida de sw (diseño, etc)

Ciberseguridad.-
Protege organizaciones, redes, servicios y usuarios.
SE enfoca en defender los sistemas de informacion redes infraestructura y ususarios frente a ameanzas en el entorno digital aplicando controles tenicos administrativos y fisicos

Seguridad de aplicaciones:
Prácticas y herramientas para proteger aplicaciones.
COnjunto de practicas estandares y herramientas orientadas a prevenir y detectar vulnrabildiades especificas en aplicaciones durante su desarrollo y operación.

Seguridad de la información 
Preserva confidencialidad, integridad y disponibilidad de los datos.
SE enfoca en proteger la informacion de la organizacion garantizando su confidencialidad integridad y disponibilidad independientemente del medio en el q se almacena o procesa.

Puntos en común: 
Gestion de riesgos: identificacion valoracion y priorizacion
Controles: Implementacion de medidas tecnicas administrativas y fisicas.
Monitoreo: Deteccion continua de amenazas y anomalias.
Respuesta: Acciones ante incidentes de seguridad
Cumplimiento: alineacion con normas, estandares, y regulaciones.

Ejemplo practico:sistema de matriculas requiere:
code seguro para evitar vulnerabilidades 
infraestructura protegida para mantener la disponibilidad (ciberseguridad)
pruebas de seguridad de aplicaciones 
proteccion de los datos

---
Objetivos y beneficios:
1. Prevenir vulnerabilidades: Evitar la introducción de vulnerabilidades y reducir la superficie de ataque
2.  Detectar: Identificar oportunamente amenazas, vulnerabilidades, y comportamientos anómalos.
3. Responder: Contener y mitigar incidentes de seguridad de formas efectiva.
4. Recuperarse: Restablecer el servicio y aprender de lo incidentes para mejorar continuamente

---
Reducir vulnerabiliades.- Disminuir las debilidades en el sw ante de su puesta en producción
Proteger la información: Garantizar la confidencialidad, integridad y disponibilidad de lso datos y tansacciones.
Mantener la disponibilidad: Asegurar la continuidad de servicio y minimizar el tiempo de inactividad.
Aumentar la confianza: Generar confianza en usuarios, clientes y partes interesadas en sw y la organizacion
Reducir constes: disminuir la cantidad de incidentes los gastos de recuperacion y las posibles sanciones regulatorias.
Cumplir requisitos: satisfacer normas politcas regulaciones y buenas practicas de seguridad aplicables al sw.

*Invertir en seguridad del sw mejora confiabilidad, continuidad y valor para el negocio*


--------
## **Seguridad por diseño**

Integra requisitos, amenazas, controles y verificación desde las primeras fases del ciclo de vida.

**Enfoque reactivo: La seguridad se aborda después de que ocurren los problemas.**

Descubrir (identificar vulnerabilidades después del despliegue) -> Corregir (Aplicar parches y correciones de emergencia) -> Recuperar (Restaurar sericios y mitigar el impacto del incidente)

Mayor coste: Las correciones suelen ser más caras
Retrabajo: Se requiere rediseñar cambios en el código
Presión de tiempo: Se traba bajo urgencia y con menos análisis.
Mayor exposición: Más tiempo expuesto a amenazas.

**Enfoque preventivo: La seguridad se integra desde el inicio de ciclo de vida.** 
Diseñar (Integrar requisitos de seguridad y modelar amenazas desde el inicio) -> Verificar (Comprobar controles y validar la seguridad durante el desarrollo y pruebas) -> Monitorear (Supervisar, detectar anomalías y mejorar de forma continua en producción)

Menor exposición: Se reducen las vulnerabilidades desde el inicio.
Controles temporales: Se incorporan controles en todas las fases del ciclo de vida
Automatización: Se integran pruebas y análisis autmoáticos de seguridad
Mejora continua: SE aprende mide y se fortalecen los controles.



*Practicas clave:* 
1. Modelado de amenazas
2. Validacion de entradas
3. Minimo privilegio
4. Gestion de dependencias
5. Pruebas de seguridad
6. Hardening 
Diseñar seguridad desde el inicio reduce exposición retrabajo y coste de correción.
Respuesta: Acciones ante incidentes de seguridad
Cumplimiento: alineacion con normas, estandares, y regulaciones.

Ejemplo practico:sistema de matriculas requiere:
code seguro para evitar vulnerabilidades 
infraestructura protegida para mantener la disponibilidad (ciberseguridad)
pruebas de seguridad de aplicaciones 
proteccion de los datos

---

Control de lectura: LIFO
## 0 Trust
## Shifleft

La importancia de la seguridad en el software.
31 % de las brechas> Explotación de vulnerabilidades como vector de acceso inicial.
	Explotación de vulnerabilidades > Aprovechando de fallas en software, configuraciones o componentes para obtener acceso no autorizado.
	
48 % de las brechas > Involucran a terceros / cadenas de suministro.
	Ransomware > Cifrado de sistemas y datos para exigir un rescate, con alto impacto en la continuidad del negocio.
40 % > más tasa mediana de clics exitosos en pishing móvil frente al correo electrónico.
	Credenciales / Pishing móvil > Robo de credenciales mediante ing. social, especialmente a través de dispositivos móviles.

ENISA 2024 > Amenazas principales: Disponibilidad, ransomware, 
	Terceros / Cadena de suministros > Compromiso de proveedores y componentes de  terceros que impacta en toda la cadena de valor.
	
checkmarks

*El panorama actual combina explotación técnica, terceros y amenazas cada vez más automatizadas.*

-------
## Las vulnerabilidades y sus costos.
CVE > Exposición de vulnerabilidades comunes
OWASP > (Open Worldwide Application Security Project)  Top 10 2025 
A01: Pérdida de control de acceso
A02: Configuración de seguridad incorrecta.
A03: Fallas en la cadena de suministro de software.
A04: Fallas criptográficas.
A05: Inyección
A06: Diseño inseguro
A07: Fallas de autenticación
A08: Fallas en la integridad del software o de lo datos
A09: Fallas en el registro, alerta y monitoreo de seguridad.
A10: Manejo inadecuado de condiciones excepcionales.

-------
## Gestion de vulnerabilidades mediante taxonomias

CVE.- Identifica vulnerabilidades.
CWE.- Describe la debilidad raíz.
CVSS.- Puntúa severidad
CPE / NVD.- Relaciona productos y contexto.
CAPEC.- Conecta con patrones de ataque
KEV / EPSS.- Prioriza explotación real y probable.

Descubrir > Clasificar > Puntuar > Priorizar > Remediar > Verificar

--------
Prueba: Vector de ataque av.n/ac.l/pr-
https://nvd.nist.gov/vuln-metrics/cvss/v3-calculator
un caso o nos da el vector de ataque e identificarlo 

![[Pasted image 20261006100941.png]]

------
## Gestión de riesgos de seguridad del software.
Dato: Hecho aislado y sin contexto. --------
- Valores
- Identificadores
- Atributos
- Sin significados por sí solos

--------> Información: Dato procesado, con contexto y valor.
CVE-2026-1234
- CVSS: 9.8
- CWE-79 (XSS)
- Producto: Product X
- Versión: 1.2.3
- Publicado: 15 jul. 2026
- Permite priorizar, evaluar el riesgo y toma de decisiones. 

------
## Pirámide DIKW:
Sabiduría (Priorizar y decidir / Acción priorizada)
	- Decisiones y mejora continua. (Estrategia de seguridad, políticas y priorización, mitigación de riesgos / Actualizar políticas, rediseñar la arquitectura, asignar recursos.)
Conocimiento (Patrones y tendencias / Análisis de riesgo)
	- Significado y contexto (Relaciones entre vulnerabildiades, causas y patrones (cwe), contexto del negocio / cwe-79 inyeccion xss comun en aplicaciones web)
Información (CVE crítica en Product X / Contexto y relación)
	-  Datos processados y organizados (CVE, CVSS, vectores de ataque, clasificacion y metrica, reportes y dashboards / cve 2026-1234, cvss: 9.8 (critica), exploit disponible )
Datos (Logs, CVE, IP, CVSS / Registros aislados)
	- Hechos sin contextos (Registros, eventos, logs; observaciones individuales, sin interpretación. / IP: 192.168.100.10, codigo 500, acceso fallido)

-----
###  La información como activo.
Información (Activo que aporta valor y debe protegerse) 
-> Valor para la organización (Procesos, decisiones y servicios, dependen de ella)
-> Riesgos y amenazas (Alteración, pérdida, exposición o disponibilidad)
-> Confidencialidad · integridad · disponibilidad (Propiedades escenciales del SGSI)
-> Gestión de riesgo (Identificar -> Evaluar -> Tratar -> monitorear).
*Proteger la información significa proteger el valor que sostiene al software y al negocio*

-----
## SGSI (Sistema gestion de seguridad de la informacion)
**Definición**
Es un marco para establecer, implementar, mantener y mejorar continuamente la seguridad del a información (ISO/IEC 27001:2022).

**Propósito**
Gestionar riesgos sobre la confidencialidad, integridad y disponibilidad de la información (ISO/IEC 27001:2022).

**Base conceptual**
Integra personas, procesos, tecnologías, y políticas para proteger activos de información (ISO/IEC 270001:2022).

**En software**
Orienta decisiones, controles y prioridades de seguridad a lo largo del ciclo de vida del sw

_Proteger el valor del negocio mediante la gestión sistemática _

Van a revisar (ISO/IEC 27001:2022) aplicada al sw y proponer 
Proyecto Parcial I: Chat con salas seguras. Desarrollar un aplicativo con salas de chat seguras con autenticación cada uno. QUe al enviar archivos modificados, detecte con escenografia. Sigue la norma (ISO/IEC 270001:2022). (Análisis, Diseño, Codificación, Pruebas, Producción)


**Analizar el OWASP TOP 10 de apis y OWASP top 10 de xxxx? (amenazas comunes para apis y aplicaciones web)**

--------

Proceso de gestión de riesgo en un SGSI.
1. Identificar.- Activos, amenazas, vulnerabilidades y escnearios
2. Analizar.- Probabilidad e impacto del riesgo.
3. Evaluar.- Compara con crietrios y apetito de riesgo
4. Tratar.- Evitar, mitigar, transferir o aceptar.
5. Monitorear.- Seguimiento continuo y revisión

Riesgo = Probabilidad x Impacto
Por ejm: API expuesta con CVE critica.

1.  
enviando archivos. Nuestro chat soporta: Imagen, audio, video (e incluso de 1 sola vista), 
la 1 version: documentos, 2 version: archivos multimedia.

como detectar estenografia: quizas un modelo de ia, libreria 

2. que tan probable es una inyeccion sql . Que tan probable es q ocurra un tipo de ataque de estenografia 


----
**Relación con la seguridad en el software**
1. **Requisitos** : Criterio e historias de seguridad. 
2. **Diseño:** Threat modeling y arquitectura segura.
3. **Desarrollo:** Revisión de código y dependencias.
4. **Pruebas:** SAST/DAST y validación
5. **Despliegue:** Hardening y CI/CD seguro.
6. **Operación:**  Monitoreo y respuesta.

El SSDF identifica recomienda integrar prácticas seguras en todo el SDLC para reducir vulnerabilidades y sus causas raíz (NIST SP 800-218, 2022)
El SGSI aporta gobierno, criterio y controles.

-----
**Normas y marcos que apoyan este propósito**
ISO / IEC 27 000:2026
	Conceptos y principios del SGSI
ISO / IEC 27 001:2022
	Requisitos del SGSI
ISO / IEC 27 002:2022
	Controles de seguridad
ISO / IEC 27 005:2022
	Gestión del riesgo
Nist CSF2.0 2024
	Funciones para gestionar riesgo cibernético
NIST SP 800 - 218 (2022)
	Practicas de desarrollo seguro
NIST SP 800 - 61r4 025 integra respuesta a incidentes con la gestión del riesgo







































