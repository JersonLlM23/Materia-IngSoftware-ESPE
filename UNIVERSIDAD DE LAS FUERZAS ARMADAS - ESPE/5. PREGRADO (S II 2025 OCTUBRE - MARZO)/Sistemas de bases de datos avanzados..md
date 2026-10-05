# **UNIDAD No. 1**
- **DATOS E INFORMACIÓN**
	**Data lake vs Data Warehouse**
	La principal diferencia entre ambos el la forma en la que almacenan los datos asi un data lake permite guardar en bruto un data warehouse solo admite datos que estén estructurados ambos son una manera excelente de procesar una gran cantidad de información.
	**DISEÑO RELACIONAL**
	1. Requisitos
	2.  Diseño conceptual (CDM)->  entidades, atributos, asociaciones, cardinalidad. Mediante la norma ansci?.
	3. Diseño lógico (LDM) -> Considerando la normalización, se analiza el tipo de dato, se pierden las asociaciones.
	4. Modelo Físico (PDM) -> Consideras el gestor de base de datos (administración de la data), Características que debe tener una BD: Seguridad, consistencia, disponibilidad, concurrencia (investigad), Debe tener un script que permita la creación de la base de datos. En la normalización minimo debe tener 4 fases. Fase 1: Eliminar repetidos, en esta forma se debe tener cuidado (cuaderno). [Entidad es algo del mundo real]. [Atributos son caracteriticas de las entidades?] Fase 2: Tiene que estar en la Fase 1, no debe haber dependencias funcionales/parciales, [Axiomas de Amstrong], Fase 3: Tiene que estar en fase 2 y Debe tener transitividad, Fase 4:  debe estar en fase 3, y eliminar atributos multivaluadas.                             Ahora viene las asociaciones, que son:

## DATA WARE HOUSE - DATA LAKE
Es como un modelo relacional.
**Tablas dimensiones:** donde q quien
- cuando? proporcionan el conexto
- Suelen tener un pequño numero de filas y un gran numero de colmnas desnormalizadas
- Suele incluir llaves (subrogadas jerarquia) la clave del negocio, campos clave para indetificar la fuente.
**Hechos**
- Proporciona las mediciones
- Ocupan aproximadamente 90% de la BD

**Desnormalizar**
Es el proceso de procurar optimizar el funcionamiento de una base de datos por medio de agregar datos redundates.
*tablas con redundancia* 
Arquitectura:
*imagen*
![[Pasted image 20251015083839.png]]

Se hace inteligencia del negocio.

----------
**Tabla de hechos**
- Tabla principal del modelo dimensional?
- contiene campos claves que se unen a las tablas de dimension
- evita la redundancia de atributos por eos existen las tablas de deminesiones
- Crece constantemente, con registros diarios o semanales. Millones de registros
- Los registros no se actualizan a no ser que se derecten errores en los datos
- Existe una llave externa por cada dimension
- La PK puede estar compuesta por las llaves de las dimensiones
- No deben existir nulos en los campos de las llaves


--------
**Tabla de dimensiones**
Tablas simples desnormalizadas
Se unen a las tablas de hechos atraves de un campo clave
no hay limite de tabla de dim
normalmente tiene pocos registors
recomendacion: ...


-------
Data Lake:
Un repositorio centralizado de todos los datos, tanto estr como no estruc sin que importe el volumen
*imagen*

--------
Data lake
*tabla*

--------
**Análisis exploratorio de datos:**
Comprender los datos antes de aplicar modelos o tomar decisiones
Estapa del flujo:
se realiza después de obtener los datos
Tareas comunes: 
descripción estadística (x, me, desv est)
visualización de distribuciones y relaciones (gráficos de dispersión histogramas)
Deteccin devalores atpicos o datos faltantes
Limpieza incial de datos para analisis posterior
Herramientas tipicas: python (panda, matplotlib), R, Jupyter, Notebooks

-----

## Data marts Data house
Data mark es para algo especifico, por ejemplo un registro de profesores (ejr1_taller3) es data mark porque solo es para esa area
Data house tiene toooodo de la empresa, financiero 

pasos para hacer Data mark o data house
1. identificar las tablas de dimensiones y luego las tablas de hechos (Tabla de hechos van los calculos por ejemplo: (ejr1_taller3 Cuantos estudiantes se registran)). (DIMENSIONES: cantidad de alumnos matriculados en cierto periodo, dimension tiempo nunca debe  faltar, Los data mark responden a una pregunta, la idea es que hayan varias preguntas pero sin embargo, solo nos concentraremos en un problema. Existen 2 metodologias mas usadas:
		 Aimno
	     Kimball?


## **Modelo Kimball (Bottom-Up)**

### **Filosofía**

- Se centra en **entregar valor rápido al usuario**.
    
- Construye **Data Marts primero**, que luego se integran en un Data Warehouse.
    
- Es **orientado al negocio**: cada Data Mart sirve a un área específica.
    

### **Diseño**

- Modelo **desnormalizado**, usando:
    
    - **Tabla de hechos:** datos medibles y cuantificables (ventas, ingresos, cantidad de productos).
        
    - **Tablas de dimensiones:** datos descriptivos que permiten filtrar, agrupar y analizar (clientes, productos, tiempo, región).
        
- Los modelos típicos son:
    
    - **Esquema estrella:** tabla de hechos central + tablas de dimensiones alrededor.
        
    - **Esquema copo de nieve:** las dimensiones se normalizan un poco para evitar redundancia.
    - - Cada Data Mart es independiente pero se puede integrar con otros más adelante para formar un DW corporativo.
    

### **Ventajas**

- Entrega rápida de resultados al negocio.
    
- Fácil de entender por usuarios finales.
    
- Flexible: puedes empezar con un área pequeña y luego crecer.
    

### **Desventajas**

- Riesgo de inconsistencias entre Data Marts si no se integran bien.
    
- Menos adecuado para análisis corporativos complejos desde el inicio.
## **Modelo Inmon (Top-Down)**

### **Filosofía**

- Busca un **Data Warehouse corporativo integrado** desde el inicio.
    
- Es **orientado a la empresa**, no a un área específica.
    
- Los Data Marts se derivan del DW central.
    

### **Diseño**

- Modelo **normalizado (3NF)** a nivel corporativo:
    
    - Reduce redundancia y asegura consistencia.
        
    - Centraliza la definición de dimensiones y hechos.
        
- Data Marts se crean después, usualmente desnormalizados para análisis rápido de un área.
- - Este DW central contiene todos los datos limpios, integrados y consistentes.
    

### **Ventajas**

- Datos consistentes y centralizados desde el inicio.
    
- Ideal para grandes empresas con múltiples áreas y sistemas.
    
- Facilita análisis complejos y corporativos.
### **Desventajas**

- Requiere mucho tiempo y planificación antes de entregar resultados.
    
- Más complejo de implementar y mantener.


| Característica        | Kimball                        | Inmon                         |
| --------------------- | ------------------------------ | ----------------------------- |
| Enfoque               | Bottom-Up (Data Marts)         | Top-Down (DW corporativo)     |
| Modelo                | Desnormalizado                 | Normalizado (3NF)             |
| Inicio                | Proyectos por área             | DW corporativo primero        |
| Tiempo de entrega     | Rápido                         | Lento                         |
| Consistencia de datos | Media                          | Alta                          |
| Orientación           | Negocio/Usuario final          | Empresa completa              |
| Mejor uso             | Entrega rápida, áreas pequeñas | Análisis corporativos grandes |

- **Kimball → “Bottom-Up” → empieza chico, crece con Data Marts**
    
- **Inmon → “Top-Down” → empieza grande, se divide en Data Marts**


- Saber qué necesita el negocio.
    
- Identificar de dónde vienen los datos.
    
- Diseñar modelo (Kimball o Inmon).
    
- Cargar datos con ETL.
    
- Crear reportes/cubos.
    
- Mantener y actualizar.


dimension es una especie de tabla. Son objetos del mundo real que traera informacion dependiendo del negocio, tiene caracteristicas como:

Tienen PK, atributos
Tabla de hechos: datos numericos (sumas, totales, promedios. )

Las dimensiones se unen mediante las llaves primarias 


OLTP: BD Relacionales
OLAP: BD multidimensionales

Kimball (metodologia agil, los entregables son fast)
1. Identificar el negocio
2. analizar las preguntas claves (TR1_TALLER3 cuantos estudiantes estan matriculados?)
3. a partir de la pregunta clave, hacer las dimensiones.



--------
## Clase 221025
Metodología inmon (top-down) Bill inmon considerado el padre del data warehouse propone un enfoque descendente centrado en la integración global de los datos corporativos

1. Diseño de un datawarehouse corporativo centrailizado
		1. Se crea una BD corporativa única normalmente en 3NF para garantizar integridad y consistencia
		2. Toda la organización comparte la misma estructura global
2. Integracion
3. Diseño de data marts derivados
		1. Despues del data warehouse central, se crean data marts tematicos (ventras, finanzas, etc) que derivan de los datos consolidaddos.
4. Normalizacion y modelado relacional
	1.  Se usa un modeleo relacional normalizacio antes de aplicar modelado dimensional
	2. El proposito es asegurar consistencia global
5. uso analitico 
	1. Los data marts permiten realizar analsisi especificos sin comprometerla integridad del data waehouse corporativo?

VENTAJAS:
- Vision integrada y coherente de toda la empresa
- Menor redundadncia y alta integridad de datos
- Escalable y adecuado para oganizaciones grandes y reguladas.
Desventajas:
- Mayor tiempo de implementacion inicial
- Puede ser menos felxivble

-----
Metodologia kimball (bottom-up) Ralph kimball en cambio propone un enfoque ascendente o por data marts, donde cada area del negocio construyse su porpio modelo dimensional que luego se integra:
1. Identificacion del proceso de negocio
	1. Se elige un area (ejm ventas) como puinto de inciio para definir los requerimientos de analis
2. 3
3. Diseño del modelo dimensional:
	    1. Se construye un modelo en estrella o copo de nieve, con tablas de hechos (medidas) y tablas de diemnsiones (clientes, productos, tiempo) (el tiempo es importante controlar y siempre estara)
4. Creacion de data marts independientes
	1. Se desarrollan data marts por departamento, asegurando que las dimensiones compartidas sean confomadas para mantener compatibilidad entre ellos.
5. iNTEGRACION DE UN DATA warehouse glonal
6 
7

Ventajas: 
Rapideez  en la entrega de resultados
Fkexubilidad puede adaptarse a cambios en el negocio
Mayot adopcion por parte delas areas operativas

desventajas

-------
generar un obdc 
instalar en el backend mysql, al momento de levantarlo, va a aparecer el obdc de mysql
Del modelo logico se obtienen los datos para la tabla de dimensiones

ORACLE person21

## DataWarehouse 
Es toodo el negocio de la empresa. Nos va a permitir hacer un control de la empresa, mediante los KPI (practicamente un termometro para la empresa. Cuantas ventas se realizaron en cierto tiempo, que vendedor, bla bla bla). Data mark con mi data warehouse

![[Pasted image 20251027082158.png]]

Las dos metodologias más usadas (hay más, pero las dos son):
- INNON (TOP_DOWN): Data Warehoue -> Data Mark (empresa grande, cuanddo no se que quiero controlar)
- KIMBOLL (BOTOM_UP): Data mark1. Data mak2, data mark3 -> DW (cuando ya sabemos qué queremos controlar)
Cuando usar cada cosa?

que es granularidad? 

cuando es:
Pais
|
ciudad
|
surcursal (de abajo hacia arriba) esto se le denomina constelación. Hay dos más: copo de nieve y estrella



# **Unidad No. 2**

## Particionamiento/Fragmentación.
### CONCEPTO DE ACID
- Atomicidad: Requiere que cada transacción sea "todo o nada": Si una parte de la transacción falla, toda las operaciones de la
- Consistencia: 
- Aislamiento: El aislamiento asegura que (q es concurrencia)
- Durabilidad

### Bases de datos Distribuidas (BDD)
Son varios BD interrelacionadas lógicamente y situadas en diferentes nodos de una red de ordenadores. Son redundantes

1. Esquema conceptual:  Identificar que tablas son las que van a crecer más.
2. Mapear el esquema conceptual, donde almacenar la información
3. fraf

Fragmentar los índices.
Puede reducir significativamente el impacto

Table space: debe tener uno o mas 
Data files: los cajones 

---------
TablesSpaces

--------
## Particiones:
Desde el Modelo Conceptual, hay que ver las tablas que van a crecer (en este caso ventas, el atributo FECHA)
1. Se debe crear el usuario NO SYSTEM


C:\Users\JERSON>sqlplus / as sysdba

SQL*Plus: Release 21.0.0.0.0 - Production on Lun Nov 24 07:28:58 2025
Version 21.3.0.0.0

Copyright (c) 1982, 2021, Oracle.  All rights reserved.


Conectado a:
Oracle Database 21c Express Edition Release 21.0.0.0.0 - Production
Version 21.3.0.0.0

SQL> ALTER SESSION SET container = XEPDB1;

SQL> CREATE TABLESPACE TS_ACADEMICO
  2  DATAFILE 'C:\APP\JERSON\PRODUCT\21C\ORADATA\XE\TS_ACADEMICO01.DBF'
  3  SIZE 20M
  4  AUTOEXTEND ON NEXT 5M MAXSIZE 100M;

Tablespace creado.

SQL>

CREATE TABLE ESTUDIANTE (
    ID_ESTUDIANTE NUMBER GENERATED BY DEFAULT AS IDENTITY,
    NOMBRE        VARCHAR2(100) NOT NULL,
    APELLIDO      VARCHAR2(100) NOT NULL,
    CORREO        VARCHAR2(150),
    FECHA_REGISTRO DATE DEFAULT SYSDATE,
    CONSTRAINT PK_ESTUDIANTE PRIMARY KEY (ID_ESTUDIANTE)
);


CREATE TABLE VENTAS (
id NUMBER,
fecha DATE,
producto VARCHAR2(50),
cantidad NUMBER,
precio NUMBER);

CREATE TABLE VENTITAS (
    id       NUMBER PRIMARY KEY,
    fecha    DATE,
    producto VARCHAR2(50),
    cantidad NUMBER,
    precio   NUMBER
);

---------
CREATE TABLESPACE TEISIC
DATAFILE 'teisic.dbf' SIZE 20M
AUTOEXTEND ON NEXT 5M MAXSIZE 200M;

CREATE TABLESPACE TEITEX
DATAFILE 'teitex.dbf' SIZE 20M
AUTOEXTEND ON NEXT 5M MAXSIZE 200M;

ALTER TABLE sales
  ADD PARTITION jan99 VALUES LESS THAN ('01-FEB-1999')
  TABLESPACE tsx;

ALTER TABLE sales DROP PARTITION dec99;
ALTER INDEX sales_area_ix REBUILD;

DELETE FROM sales PARTITION (dec99);
ALTER TABLE sales DROP PARTITION dec99;

ALTER TABLE sales DROP PARTITION dec99;
UPDATE INDEXES;

------------
## Particionamiento HASH
Cuando no tenemos un criterio claro de qué tablas pueden crecer

## Fragmentación vertical:
Realizar views?


## Bases de Datos Distribuidas:

**MODELO RELACIONAL:**
![[Pasted image 20251201072924.png]]

Ventajas: 
- Más rápido de respuesta
- Si un nodo muere, sigue funcionando
Desventajas:
- Costoso 

-------
## **Replicación de Bases de Datos** 
Relacional: Se organizan datos en tablas definidas, esquemas normalizados
No relacional: Datos más flexibles, JSON, grafos.

RELACIONAL: 
[Foto]

SIMILITUDES EN REPLICACION SQL Y NO SQL
[FOTO]


## Cliente server.

Client: Solo habrá servicios de conexión. IDE SQL para conectarse al equipo

Server: DBMS, configurar: tnsnames.orq

-------


# **Unidad No. 3**
## **CRUD EN MONGODB**
Las operaciones CRUD son (u know) documentos.
- La operacion de creacion/insercion alade documentos a una coleccion.
- Iportante: Si la coleccion no existe actualmente, las operaciones de insercion crearán la coleccióon.
- 