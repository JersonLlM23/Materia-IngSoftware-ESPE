# **UNIDAD 1**
## **Página web vs Sitio web vs Aplicación web**

PW -> Informativo
SW -> Conjunto de paginas informativas o transaccionales (Interactuan con Bases de Datos)
AW ->

- Página web: Es un doc escrito en lenguaje html (lenguaje de marcas con hipertexto) _CSS( lenguaje de hojas de estilo )_ , puede tener css, JS 
- Sitio web: Conjunto de paginas web estructurados en un dominio (direccion, por ejemplo de la espe: monster.edu.ec, monster es la empresa, edu es el tipo de organización y ec el país ) en MVC se usa: ec.edu.monster.modelo/controlador/prueba/servicios. _En java son paquetes, en .net son carpetas_  como google.com, facebook.com por ejemplo en ed.team hay una pagina web de inicio, una pag web de cursos. Todo ese conjunto de estas dos paginas web en el dominio, son un sitio web. 
  Se divide en dos tipos:
	1. informativos: Los sitios web, su objetivo es el marketing, ese sitio web no es el negocio, es solo marketing (colegios, restaurante), Aqui se usan CMS (como hubspot, WB, WIX) para crear un sitio informativo, no requiere code (y si tambien), solo se necesita marketing digital. 
	2. aplicaciones web: Es un software creado con tecnologias web. Si es el negocio (EDteam, ESPE, Netflix, Google, Facebook). Para hacerlo, se necesita algo personalizado, ya no se usa CMS, sino librerias, frameworks, lenguajes de programación. Se necesita desarrolladores web profesionales, no de marketing digital.

_IEEE 830 son los requerimientos del software, hay funcionales y no funcionales. FN: Que voy a hacer?, negocio,  FNN: Como lo voy a hacer?_ 
**Front end, Back end, Full Stack**
Sv hace la validacion de que el cliente tenga los permisos. Con php se conecta a la BD. 
FE ->  logica en el lado del cliente, tiene 3 etapas: 
	1. Llegada de html5, css3, angular JS. Tambien mongodb, node js, ...
	2. Llegada de la 6 edicion de JavaSctript, trae nuevas funciones, ya no se uso el JQuery, y reactJS apareció ... (debemos anotar lo que está en el video graphql)
	3.  La que estamos empezando a vivir, 1. Web assembly (codigo nativo), Houdini. Hay 3 roles: Diseñador UI, Maquetador (usa html), Programador frontend
	es la programacion en el cliente
BE -> logica de la programacion/negocio, todas las funciones desarrolladas para el cliente. El backend debe crear la API y se debe conectar a la BD también. 
dos tipos de apps: _monolitos (Personal, recursos humanos, finanzas, marketing. Falla algo y se arruina todo. (Personal es un monstro chiquito, recursos humanos monstros chiquitos) y Microservicios_ El backend debe tener en cuenta la seguridad, rendimiento. Backend developer, database administrator, cloud computing
para conectar a los dos, se usa API. es la programacion en el sv



stack: conjunto de teconologias para hacer un sw

FS -> Hace BE y FE, elstack mas usado fue STACKS: LAMP (Linux (S.O) Apache (Servidor de aplicaciones) MYSQL (GESTOR BASE DE DATOS) PHP (ID desarrollo)) , y XAMPP (X= sistema operativo, A= Apache, M= MYSQL o MariaBD. P= PHP myAdmin, P= Perp / PHP (es el IDE)). MEAD mongo express angularJS Node js. 

Taller: Investiga **Que es un desarrollo web FE, BE, FS, que roles hay en cada uno de ellos, ventajas/desventajas, aplicabilidad**  conclusiones, recomendaciones, bibliografia 



## MVC (Modelo-Vista-Controlador)
Es un Patrón de diseño arquitectónico (hay dos, Patrón de diseño (como solucionar un problema con un patron q ya existe) y Patrón  d diseño arquitectónico. creo).
MODELO: Donde ingresa datos los usuarios.
VISTA: 
CONTROLADOR:
Vamos a usarlo desde el diseño, es decir, desde el diagrama SECUENCIA. La manera en la que disñamos una app. Fue creado en 1979 para separar la funcionalidad de la aplicacion.
- User Interfaces
- Business Logic
Objetivos: 
- No repetir.
- Programación estructurada.
- Promueve la programación organizada.
No solo es ventana, sino debe interactuar con la bd y para eso, se necesita la logica del negocio. 

**MVC Frameworks:**
Ruby:
- Ruby on Rails
- Sinatra
PHP:
	- CakPho
	- Zend
	- Code Igniter
	- Laravel
Python:
- Django
- Flask
JS.
- express
- sails
- backbone
- angular
Net:
- ASP MVC

----------
Como trabaja la web?
**USER FLOW**

**VIEW:**
*Cliente:*
- NAVEGADOR
- HTML /CSS / JS

 ->
 
**CONTROLLER:**
*Servidor:*
- LINUX / WINDOWS SERVER
- SERVER SIDE PROGRAMMING LANGUAGES

El controlador debe almacenar todos esos datos por lo tanto ->

**MODEL**
*DataBase:*
- SQL MySQL / NOSQL MongoDB
- Store All Data
--------
MODELO:
- Data related logic
- Interacting with DB (select, insertm update, delete -> todo esto es el CRUD C: Create (Insert un nuevo registro en una tabla), R: Read (Select .. ...), U: Update (te actualiza todooo menos la llave primaria), D: Delete (siempre cuando hagas un delete o uptade, siempre debe ir un WHERE)). El CRUD se hace tanto en el backend (Base de Datos) como en el front (IDE -> lenguaje de programacion) 
- Communicates with controller
- Can update the views depending of the framework
- La base de datos no se puede conectar directamente con...?
-------------
VIEW:
- What the user sees UI
- Just speaks with the controller
- Usually consist of HTML/CSS
- Communicates with the controller
- can be passed dynamic value from the contoller
- Templates engines 
- views libraries
Un usuario solo debe interactuar con la interfaz, solo habla con la interfaz, que este habla con la logica
----------
CONTROLLER:
La parte logica
- process request (GET, PUT, POST, DELETE)
- Is in the middle of the view and the model:
	-take user information
	-communication with db
	-gets data from the model
	-pass data to the view
x
------
User (routing processing http://gogle.com) -> View -> Controllador (recibe este link, hace una consulta a -> MODELO (BD)

User -> View -> controller -> model 
User <- View <- controller <- model
En el controlador tendremos nuestro servidor de aplicaciones con dos ambientes: JAVA, .NET.
En JAVA Hay 2 IDES : Apache netbeans (glassfish obsoleto, se cambió a Payava?) y en .net: eclipse (IIS. internet information server) , (YBoss obsoleto, ahora es WildFly. 


---------
JSP para mostrar contenido web dinamico
Serviets desarrollar 
fragmentos extraer marcadores comunies en fragmentos de code




Extra: 
- la cédula jamás será PK por motivos de paises y eso
- SQL: (Structured Query Language)
- Trabajo: Consulta de todos los 5 principios de solid + MVC y formulario web sin MVC, .... y con MVC, ....  .NET Y JS?
- MVC en JAVA 003 (sin mvc en java(, 004 (con mvc en java)
- JSP -> JavaServerPages se cambió a JSFaces -> RichFace, BoatFace y toooodo esto es } VISTA


d

-------

## CLASE 3
IEEE 830 Para la especificacion requisitos, tienen dos:
RF: que debo hacer -> negocio
RNF: como? -> teconologias de informacion

La seguridad y calidad antes eran RNF, ahora son RF 
La seguridad y calidad se inician con el proyecto


## Qué es un ORM
- BD: Son conjuntos de datos organizados en forma de sistema (guardar info y consultar info). pst: hay 5-6 formas normales... boys and cout ? permite que se cumpla el programa o el acrónimo ACID en la base de datos.
	A: Atomicidad ()
	C: Consistencia ()
	I: Islamiento ()
	D: Durabilidad (que persiste en el tiempo).
- SQL: Es el tipo más usado, es relacional pq es usado con tablas, structure query language.
- CRUD: Iniciales:
	- C: Create
	- R: Leer Read
	- U: Editar Update (!)
	- D: Borrar Delete (!)
	! Necesitas si o si poner un WHERE.
- POO: Programación Orientada a Objetos es el paradigma más usado.

**ORM**: Toda aplicacion debe conectarse a una red de datos. No importa el lenguaje del backend, para conectarse a la BD se necesita SQL.

O bjetc : Referencia a POO 
R elational : BD Relacional
M apping: Empareja valores

Tabla -> Clase
Fila -> Objeto

**VENTAJAS Y DESVENTAJAS**
VENTAJAS:
- No se usa SQL

-----------
**TIPOS DE ORM**
Para PHP: Laravel, Symfomy
JS: 

![[99fbab95-59c4-451a-85ec-0b311c18a1f1.png]]
-------
## **POWER DESIGNER**
Es una herramienta CASE para modelar.
C: Computer
A: Aided
S: Software
E: Engineering
Hay dos modelos imporantes:
- Modelo orientado a objetos. -> Diagramas UML (UML es una herramienta para metodología, pero no es una metodologia)
- Modelo orientado a datos. -> (MODELO ENTIDAD RELACION -> Conceptual, Logico, Fisico)

Para hacer una entidad, el CODE:
X (Subsistema)
	- Personal (P)
	-Finanzas (F)
	-Seguridad (S)
	-Académico (A)
Y (Tipo de Objeto)
	-Entidad
	-Relación
	-Vistas (logicas, las tablas son fisicas)

xxx (nombre corto de la tabla, siempre 3)

zzz zzz (nombre largo de la tabla

XYxxx_zzzzzz

P E EMP_EMPLE

Que es PK? identificador que 
Displayed: si se vaa desplejar en la tabla (ocultar pero que se guarde)

DOCUMENTACION: Hacer un video de 1 minuto donde se demuestra la corrida del sistema. Y habla la diferencia entre usar MVC y sin MVC, por ejm: en cada paquete hay clases y eso. (Debe aparecer la foto, y cuando despliegue debe aparecer la misma foto?)
Puntos extra si arreglas ese JAVA
IDE27 JAKARTA 10 PAYARA 6 JDK 21

MER: Modelo entidad RELACION
BDD: BASE DE DATOS


-----------

## Para el proyecto: IEEE 830 PLANTILLA
1. Documento: especificación de requisitos.
2. CASO DE ESTUDIO: Planteamiento del problema
3. Introduccion: tal cual, solo cambia lo ultimo
4. NÓMINA, recuerda las faltas ortografias.
5. PERSONAL Y FINANZAS son iguales. y.. elimina financiamiento en presupuesto/financiamiento 
6. Definiciones: IDE q es. 2do parcial: apache/JAVA, Netbeans. y en el 3 Parcial: DotNet C# o APNET.  BASES DE DATOS: MariaDB o MYSQL , SQL SERVER y herramienta CASE: POWER DESIGNER. q son los gestores de bases de datos, def corta de mysql, sql server.
7. Acronimos: Usuario no deberia estar ahi, sino en definiciones. ERS o SRS RF: REQUERIMIENTO FUNCIONAL. 
8. ERS: Es la carta y en el ECUD: cómo se hace la sopa 
9. REFERENCIAS: ehh el ieee está bien? 
10. CASOS DE USOS: La norma para describir los casos de uso son: verbo en infinitivo (1 letra en infinitivo, la segunda palabra un objeto. ELIMINAR FACTURA, AGREGAR, si se hace un CRUD, -> GESTIONAR)
11. CASO DE USO GENERAL
12. Actores: los que usan el sistema
13. no debe quedar titulos al final del documento
14. color same
15. listado de requerimientos funcionales y no funcionales
-------
## Documento ECUD
CASO DE USO de cada requerimiento detallado
PON CASOS DE USO DEL SISTEMA DE SEGURIDAD PRIMERO: crear perfiles, cambiar contraseña, etc.
Una tabla en el diagrama E-R es un caso de uso -> (diagrama acrividad, secuencia), clase del diagrama de clases


## Casos de USO
Representa el comportamiendo de sw en la interaccion con el user para q este alcance un objetivo
Describe lo que el sw debe hacer y para quien, no como este será implementado.
La tecnica de casos de uso está compuesta por:
- Diagrama de casos de uso.
- Descripción de los actores
- Especificacion de los  casos de uso

-----
## Diagrama de casos de uso
- Compone el producto en analisis
- Representa gráficamente

### Elementos:
**ACTOR**
Representa una persona (o un grupo de personas) que desempeñan un papel o interactúan con el software. No se limita a eso y puede ser cualquier "cosa" que interactúe con el software con la finalidad de cumplir un trabajo significativo, como otros productos de software o mismos equipamientos.

**CASO DE USO:** Representa una funcionalidad que atiende a uno o mas requisitos del cliente. Como nombre, se sugiere usar un verbo infinitivo con un complemento. Los casos de uso pueden opcionalmente estar encerrados por un rectángulo que representa los limites de sistema.

**RELACION (ASOCIACION):** Un actor interactúa con un caso de uso y es representado por una relación. Los casos de uso también pueden relacionarse entre si

### RELACIONES:
La asociación entre el autor y un caso de uso es denominado relacion de comunicación.

**ACTOR ACTIVO**: Inicia o dispara la ejecución del caso de uso. (La flecha si hay), apunta al caso de uso
![[Pasted image 20251027102123.png]]

**ACTOR PASIVO**: No es iniciado por el actor, el caso de uso reacciona ante una provocación de software que inicia la comunicación. La flecha apunta para el actor
![[Pasted image 20251027102222.png]]

![[Pasted image 20251027102317.png]]



## Diagrama ENTIDAD - RELACIÓN
Es una representación graifca

## Relaciones:
- 1:1
	![[Pasted image 20251029093746.png]]

- 1:N
![[Pasted image 20251029100412.png]]

**Hija -> Padre dependiente **

HIJA voy a tener una PK compuesto: PK padre + PK de otros cargos


Un empleado tieen 1 solo ESTADO_CIVIL (padre)
## CDM, LDM, PDM

CDM -> LDM -> PDM
conceptual model -> 
logical data model -> 
physical data model (mysql, oracle) -> script con ddl (data definitva language) -> BDD

# **UNIDAD 2**

## **ORM**
Un ORM abstrae la base de datos para que el programador haga consultas en el lenguaje en el que está programando, sin necesitar SQL.
![[ORM[1].jpg]]

## CRUD
Create. Sentencia INSERT INTO TABLE VALUES Crea nuevos registros
Read. SELECT FROM * Lee los datos del registro
Update Actualiza los datos del registro
Delete Elimina los datos del registro
![[CRUD[1].jpg]]

-------
## Pal proyecto

Es como un submenu asi como pestaña archivo word:
- Archivo:
	login, logout, input data, export data
- Admin tab básico
	Académico
Procesos
Product


----
# **UNIDAD 3** 

**SQL (Structured Query Language):** 
- Organiza los datos en tablas
- Cada Registro en una Fila
- Los datos de las entidades están definidas
- Su manejo es transaccional
- Búsqueda indxeada.

**NoSQL (Not Only SQL)** :
- Organiza los datos en colecciones.
- Cada registro es un nodo o documento.
- Los datos son flexibles, pueden estar presentes o no.
- Su manejo no es transaccional.
- Búsqueda semántica.

## **Modelos NOSQL**
### Modelo documental 
-> Mongo DB, Couch DB, 10gen
Documentos JSON (JAVASCRIPT OBJECT, 
{
Nombres: 'xxxx'
Apellidos: 'yyyy'
Edad: zz
}

### Modelo Grafos.
-> HyperGraphDB, AllegroGraph, InfiniteGraph

### Modelo Clave-Valor
Dynamo, BigTable, Riak

clave:x1,x2,x3
clave2: x2,z2,
clave3:y3,z3


--------
SQL: Normalizacion (RELACIONAL)
NOSQL:  No hay normalizacion  (documentales, clave-valor, columnales, grafos


Ecosistema no sql - 
HBASE, cassandra (sistema distribuido)
REDIS ( BD Clave valor)
Neo4J

MongoDB (Documental, formato BSON)
caracteristicas: indexacion , soporte para sql, consultas, transacciones, gran escabilidad horizontal, sinergia con javascript

-----
## **Bases de datos documentales MongoDB**
Las bases de datos documentales BDD están concebidas para el procesamiento captura almacenamiento distribución y recuperación de información vinculada con la representación del conocimiento registrado en los documentos.

**¿Qué son las bases de datos documentales?**
Es un conjunto de información estructurada en registros y almacenada en un soporte electrónico legible desde un ordenador.
Gestionan tipos de datos muy complejos (documentos científicos y técnicos) y actividades muy simples como la entrada y salida de documentos.
Poseen un sistema de recuperación de información.

**Tipos de búsqueda:**
- **Búsqueda directa:** 
Se teclea directamente una o varias palabras en el espacio reservado para ello por el sistema de interrogación en la bd
Interrogación en texto libre
Interrogación en campos individuales
- **Búsqueda a través de índices:**
En vez de teclear un termino, el usuario visualiza un diccionario o índice alfabético de las entradas de todos los campos y selecciona los más adecuados para su búsqueda.

pst: En sql las búsquedas se realizan con índices y en nosql de manera semántica (por el contenido)
.
.
.


-----
## **Base de datos SQL vs Base de datos NOSQL**
**SQL (Structured Query Language):** 
CRUD -> Relational DataBase Management System (RDBMS)

**NOSQL**
CRUD -> Application Programming interfaces (API), Documentación
- Clave valor
- Documento
- Grafos
- Columnares

Ventajas:
- Versatilidad (agregar información o cambios en el sistema sin necesidad de hacer cambios externos)
- Crecimiento horizontal
- Guarda cualquier tipo de dato
- Consultas usando JSON

-----
## **Tipos de bases de datos NOSQL**

*Tipos de bases de datos nosql*

**Clave-Valor:** 
Una clave sirve como un identificador único.
Documentales
Grafos

.
.
.

------
## **MongoDB**
*Que es MongoDB*
Base de datos NoSQL escalable y orientado a documentos.






dif entre sql
4 nosqls
ventajas desventajas casos de uso
