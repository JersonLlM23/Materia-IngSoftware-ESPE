# **Parcial I - Sistemas Operativos** 
## Principios básicos de los sistemas operativos.
**Objetivo:** 
	Administrar todos los dispositivos y proporcionar a los programas de usuarios una interfaz sencilla.
	Proporcionar a los programas y usuarios un modelo de computadora mejor, mas simple y pulcro, asi como encargarse de la administración de todos los recursos.

## Qué es un S.O
Es un conjunto de programas en un sistema informático que administra recursos de Hardware y proporciona servicios a programas de aplicaciones de Software. El SO está entre el Software y Hardware.
Es la porción de software que opera en modo de Kernel o modo supervisor, y esta protegido de la intervención del usuario por el hardware.

Usuario -><- Aplicaciones Software -><- S.O -><- Hardware -><- S.O -><- Usuario.

Es el medio de comunicación entre el user y la computadora, maneja la carga y ejecución de programas de aplicación y administra la transferencia de datos y archivos hacia y desde dispositivos periféricos.

Un SO explota los recursos de hardware de uno o más procesadores para ofrecer un conjunto de sv a los usuarios del sistema.

## Elementos básicos de lo S.O
- Procesador 
- Memoria principal 
- Interconexión de Sistemas
Todo esto se ve en el administrador de tareas.

-------------
## Funciones de los S.O
- Acepta datos de dispositivos de entrada y los transfiere a la memoria de la computadora.
- Asegúrese de que cualquier salida se envíe al dispositivo de salida correcto.
- Gestiona la transferencia de datos entre la memoria de la computadora y los dispositivos de almacenamiento de respaldo
- Asigna espacio de memoria a programas y datos
- Carga el software de las aplicaciones en la memoria y controla su ejecución.
- Se ocupa de cualquier error que se produzca cuando se ejecuta un programa e informa al usuario.
---------
- Gestión de memoria
- Gestión de ficheros
- G. Red
- G. Procesos
- G. Recursos.
- Protección y seguridad
- Administración de usuarios.
- G. Dispositivos E/S
---------
Aplicaciones -><- Kernel -><- (cpu) , (memory), (devices)


----------
## Componentes de un S.O
Shell ( Sevicio (API) ( Núcelo ))

Los SO se pueden ver desde dos POV:
Administradores de recursos: EL SO administra las distintas partes del sistema en forma eficiente.
Maquinas extendidas: capa entre user y hw q ofrece una maquina extendida ...

----------
1 Generacion (1925-1955)
SO inexistente, se utilizaban tubos al vacio,
Lenguaje de máquina

2 Generacion (1955-1965)
Se utilizaba el procesamiento en serie,
Transistores
Tarjetas perforadas

**LATEX: Evoluciones, generaciones, años de segmentos una descripción y todo lo q escribamos y detallemos debe estar referenciado (autor, año) + compilation no plagio + individual + referencias + calidad (gráfica) + PDF + imprimir de lado y lado + tipo de letra arial 12 | COMPLETA LA EVOLUCION HISTORIA DE LOS S.O + flash USB + mapa estructurado**     


--------
1950: inicio de lo SO
Los primeros so eran muy basicos y estban diseñados para realizar tareas especificas en compu de gran tamaño mainframes. Los operadores cargaban programas en la maquina de fomra manual.
Ejm: El supervisor del sistema IBM 701
1960: multiprogramacion y sistemas en lote
permiten ejecutar varios trabajos sin intervencion humana directa. Tambien nace el conepto de multprogramacion donde varias programas se cargaban en la memoria para aprovecha mejor los recursos.
en esta decada surgen los primeros sitemas tiempo compartido, que permitian que varios usuarios interactuaran con el sistema e manuera simultanea. CTSS (compatible time-sharing system) y multics, que influyó posteriormente en unix.

flash booteable: sistema booteable linux

1970: Sistemas de  tiempo compartido y unix
aparece unix uno de los so mas influyebtes desarrollado por at/t unix fue diseñado para ser portatil simple y multitarea marcando un cambio hacia so mas accesibles  y versatiles
Comienzan a implementarse so con soporte para redes rumentarias, lo q seria clave en la evolucion futura Ejm: Unix, y VMS (Virtual memory system) de DEC.

1980: sistemas o. para pc y gui
los so para computadoras personales PCs comenzaron a proliferar. MS-DOS y Apple DOS fueron clave en esta epoca. Además se desarrollan los primeros so con interfaces graficas de usuario GUI como macintosh system sw de apple.
Unix continuó expandiendose mientras que el mercado de pc crecia rapidamente. Ejm: Mac, OS, la s primeras versiones de windows

1990 Windowss y linux
Esta decada marco la dominacion de microsoft windows en pc con su entorno grafico. windows paso de ser un sumple gui sobre DOS a un so como windows 95
En paralelo, surge Linux un so basado en unix de codigo abierto y gratuito que comenzo a ganar popularidad entre desarrolladores y empresas por su flexibilidad y seguridad. 


2000 SO moviles y virtulizacion
El auge de dispositivos moviles y la computacion en la nube marco la pauta. Windows siguió dominando las PCs. pero Linux gano territorio en servidores.
En el mundo movil iOS, y android emergieron como los sitemas operativos dominantes, basados en unix y linux respectivamente.
Se popularizan tambien las teconologias de visualizacion y contenedores, con el uso de maquinas virtuales en sistemas operativos para mejorar la eficiencia de los centros de datos.

2010: So moviles y en la nube. La computacion moil sigue creciendo con android e ios dominando el mercado. Los so tambien se adaptan a la comptutacion en la nube con servicios como AWS y AZURE.
Linux se convierte en la base de muchos servicios en la nube, y su uso se expande mas alla de los sv tradicionales
El concepto de contenedores con docker por ejm. y la orquestacion Kubernetes llevan a llinux a nuevas areas de gestion de infraestructura a gran escala. Ejm: android,ubuntu, windows 10

2020 Seguridad, virtualizacion avanzada y IoT
La seguridad se convierte en una prioridad con so enfocados en proteger los ususarios frente a ciber amenazas crecientes. 
La virtulizazcion sigue avanzado con un enfoque en contenedores y  computacion distribuidad.
SO para internet de las cosas IoT como raspbian y tinyOS empiezana a desempeñar un papel más relevante.
Ejemplo: android, ios. so para IoT

------
## Tipos de SO
SO mainframe
SO de servidores
so multiprocesadores
so compu personal
so computadoras de bolsillo
so integrados
so nodos sensores
so tiempo real
so de tarjetas inteligentes

----
### Sistemas Operativos de mainframe.
Están orientados hacia el procesamiento de muchos trabajos a la vez de los cuales la mayor parte requiere muchas operaciones de Entrada/Salida.
3 tipos de serivicios:
- Procesamiento de lotes,
- Procesamiento de transacciones,
- Tiempo compartido.
Trabaja por unidades de procesos pequeñas pero maneja miles de unidades de procesos. 

(saca 3 ejemplos tio Ejm: Entidades financieras)

Los SO mainframe -> gestionan grandes y poderosas computadoras, conocidas como mainframes. eSTOS SISTEMAS SE USAN EN ORGANIZACIONES Q REQUIEREN MANEJAR GRANDES VOLUMENTes de datos y gestionar multiples usuarios simultaneamente como bancos, gobiernosm intstituciones educativas y grandes coporaciones.
Los mainframes son concoidso por su capacidad de procesamiento, estabilidad, fiabildiad t y su habilidad para maneaajr transacciones criticas en tiempo real. Los sitemas operativos de MF como IBM z/OS o mvs permiten q estas maquinas realicen tareas complejas como procesamiento de transacciones en linea, administracion  de bases de datos masivas y virtualizacion de recursos.

-------
### Sistemas operativos de servidores.
Se ejecutan en sv, estaicones de trabajo o incluso MF
Varios usuarios a la vez
Permiten compartir los recursos de hw y sw
Solaris, FreeBSD, Linux, Windows Server 200x

So esta diseñado para adminsitrar svs que son encargadas de ofrecer servicios a toros dispostivvos en una red.
Este so se usa en empresas para gestioanr recursos como bd archivos aplicaciones web y servicios de red, optimizado para ejecutar tareas de alrendimiento de manera continua.
Los so de sv son altamente escalables, permitiendo la adicion de mas recursos a medidad qeue crece dla demanda. Ejm: linux server, winows server, unix, red hay enterprise linux
Esos so suelen ser más robustos en cuanto la seguridad, estabildiad y la capacidad de manejar multiples users y procesos al mismo tiempo.

-----
### Sistemas operativos de multiprocesadores
A menudo son variaciones de los so de sv con caracteristicas especiales para la comunicacion conectividad y consistencia.
.
.
Los so de multipro estan diseñados para funcionar en entornos de compus que cuentan con mas de un procesador fisico paermitiendo q multiples undiades de preocesamiento trabajen de manera simultanea
Optimizan El uso de varios nulceos de procesami para ejectuar tareas complejas de manera mas eficiente. Se usan en aplicaciones que requieren un algto poder de computo como simulaciones cientificias nalasis de grandes volumentes de datos
El objetivo de lo sistemas es maximizar la capacidad de procesamiento reducir los tiempos derespuesta y mejorar el rendimiento en situaciones de alta carga.
Ejm: so para multiprocesadores incluyen versiones epsecializadas de linux y windows server.

----
### Sistemas operativos computadores personales
So modernos soportan la multiprogramacion
Soporte para un user (procesamiento de texto, hojas de calculo y acceso de internet)
Estan diseñados para uso individual en dispostivos como compus escritorio y portatiles
Estan orientados a proporcionar una GUI amigable y funciones accesibles para tareas generales como navegacion web, procesamiento de textos, multimedia juegos
Se enfocan en la facilidad de uso compatibilidad con una amplia gama de sw y dispositivos perifericos.
los + conocidos son winws macos linux cada 1 con caracteristicas particulares:
wsw destaca por su compatibildidad con aplicaciones comerciales
Macos por su integracion con el ecosistema de apple
linux por su flexiblidad y code abierto.

----------

## Gestión de Recursos
Gestión de procesos, memoria, E/S, redes, proteccion, archivos, Intérprete de órdenes.

1 2(redes)  E/S proteccion (3), gestion archivos, interprete de ordenes (5)


gestion de redes
exponer caracteristicas de cada gestion (q componen, q hacen, donde se aplica, como actua esa gestion en el S.O)


--------
Evolucion de los s.o
Traditional hw: 
app app app
OPERATING SYSTEM
HARDWARE

->
Virtualized deployment:

Virtual Machine{
App app
Bin/Library
Operating System
}

Virtual Machine{
App app
Bin/Library
Operating System
}

--
Hypervisor
Operating system
hardware


->
Container Deployment:

Container{
App App
BIN/LIBRARY
}

Container{
App App
BIN/LIBRARY
}

--
Container Runtime
Operating System
HW




--------
Microsoft Windows, Windows 3.1 95 98 2000 me xp vista 7 8 8.1 10



----
Windows server OS
1993 w net 3.1
1994 w nt 3.5
1995 w nt 3.51
1996 w nt 4.0
2000 w 2000 sv
2003 w server 2003
2006 w server 2003 r2
2008 w server 2008
2009 w server 2008 r2
2012 w server 2012
2013 w server 2012 r2
2017 semi annual channel and long-term servicing channel releases
2018 w server 2019
2021 w server 2022

---
Historia de apple
1976  1977: apple II
1977-1998 1984: Maicntosh
1998 1985: laserWriter
2001-2007 2001: iPod
2007-2013 2003: itunes store
2013 2007: iphone
     2010: iPad

------
Arquitectura linux
HW comprende recursos de cpu memoria interna almacenamiento y dispositivos de entrada y salida
Aplicaciones{
shell{
kernel{
hardware{ terminales printers disk }
}
}
}
el shell proporciona un metodo para comunicarse con el sistema operativo. Esta comunicacion se porduce de fomra interactiva con la CLI o como un script de shell. Un scrip de hell es una secuencia de comandos de shell y del so que se almacenan en un archivo
Los hell incorporan un lenguaje de programacion apara controlar procesos y archivos e iniciar y controlar otros programas.

El kernel o nucleo es una parte dfundamental del so encargada de otorgar acceso al hw de forma segura a todo.

-------

## tipos de nucleo
el kernel es la parte central de un so gestiona los recuros del sistema mem y procesador
es un punete entre la aplicacion y el hw de la compu
se ejecuta en modo provilegiado tambien conocido como modo jernel
proporciona controladores para dispositivos conectados a los diferentes buses del sisetema como USB PCI SATA e IDE
El kernel se puede clasificar ademas en microkernel y monolithic kernel


arquitectua windows
W tiene una estructura con un enfoque de kernel hibrido que ofrece una arquitectura versatil y eficiente para el so el acceso directo al hw y la memoria del sistema permite que los componentes y servicios criticos funcionen en modo jernel mientras que los servicios del usuario se ejecutan de forma aislada y segura para garantizar la estabilidad y la comptabilidad.

the architecture of windows nt https://medium.com/@putrasulung2108/windows-architecture-d2b022f136d3

como son los 
![[Pasted image 20260422101149.png]]


-------
La arq andorid contiene diferentes componentes para satosfacer necesidades
El sw de andorid incluye un kernel de linux de code abierto con una coleccion de bibliotecas c/c++ q se exponen a traves de servicios de marco de aplciaciones
Entre todos lso componentes el kernel de linux proporciona la funcionalidad prinicpal de las funciones del so para telefonos inteligentes y la maquina virutual Dalvik DVM proporciona una plataforma para jecutar una aplicacion de android.
Los pinricpales componentes de la arquitecutra de andorid son los siguientes: aplicaciones marco de aplicaciones tiempo de ejecucion de andorid bibliotecas de plataforma y jernel de linux

![[Pasted image 20260422103937.png]]

----
ios es el sstema operativo movil propietario de apple q solo se ejecuta en los iphones de apple
Apple presento la primera vesoin de ios en 2007 y se ejecuto en la primera genreacion del iphone
la interfaz grafica predeterminada oips es cocoa touch 
ios se distingue por:
su interfaz grafica intuitiva
Servicio icloud para alamacenamiento y sincornizacion de adatos
altos estadares de seguridad y provacidad
app store para descargar y comprar aplicaciones

medium/@lucideus/understanding-the-structure-of-an-ios-aplication
![[Pasted image 20260422103646.png]]


------
MacOs es el so que se ejecuta en todas las compus mac. 
ES una serie de sistemas op graficos desarrollados por apple desde 2001
la ultima version es ventura q se lanzo en oct 2022
xnu es un kernel desarrollado originalmente por next e implementado por apple inc en 2000
aqua es el nombre comercial de la apareiencia gui del so mac.
![[Pasted image 20260422103843.png]]
----
Clasificacion de so.
tutorialandexample types of-operatingsystem
![[Pasted image 20260422104147.png]]

----
El so multitarea es una extension logica de un sistema de multiprogramacion que permite multiples programas simultanemanete. Permite a un usuario realizar mas de una tarea informatica al mismo tiempo.

------
soste,a de archivos q usa el so para almacenr y recueperar archivos en unidades de disco duro HDD y unidades de estado solido SSD
El sistema de archivos FAT32 no puede almacenar archivos individuales de mas de 4 gb mientras que el sistema de archivos ntfs si
en comparacion con fat32, el sistema de archivos ntfs tiene una myor utilizacion del disco





![[Pasted image 20260422104246.png]]


Busca definiciones ejemplos q esta haciendo y en donde esta aplicado. Similar
para cada uno de ellos "clasificacion de sistemas operativos". Buscar en todas las plataformas linux, windows, o si existe en sistemas aplicaciones moviles

---
Un sistema de archivos es todo lo siguiente:
Almacenamiento de datos:
la funcion principal de cualqueri sistema de arhivos es ser un lugar estructuradao para lamacenar y recueprar datos
Espacio de 


-----
Open source sw
code abierto:
En 19838 se inicio 


(Evaluacion: q son cada uno, )


----
Free Software 
Richard Stallman fundó la free software foundation en 1985 para proporcionar la estructura sus ideas sobre el sw libre.
Las 4 freedoms?


Steve Jobs 1955 feb
computadoras con fuentes
servicios de streaming
telefonos inteligentes
televisores con conexion a internet
tabletas comerciales

Bill Gates 1955 usa
fundador de microsoft en 1975 junto con paul allen 
introduccion a msdos
Linux Tovalds


-----
Ubuntu server es la distro linux mas popular gracias a su gran flexibilidad escalabildiad y seguridad en los centros de datos empresariales
Un s.o proporiona una variedad de contencion de falla, tolerancia a errores
![[Pasted image 20260429093343.png]]

-------
Estructura de los SO red y distribuidos
Sistemas monoliticos
de capas
microkernels
modelo cliente sv
maquinas virtuales
exokernel


------
Sistmeas monolitcos
Considerados como la organizacion mas comun
tiene una estructura basica para el so
1. Un programa pincipal que invoca el procedimiento de servicio solicitado
2. Un conjunto de procedimientos de servidores que llevan a cabo las llamadas al sistema
3. Un conjunto de procedimientos utilitarios que ayudan a los procedimientos de servicio
Usuarios sencillos
Estructura de un sistema monolítico
Procedimiento principal -> Procedimiento de servicio -> prodecimientos utilitarios
hay una jerarquita


![[Pasted image 20260429093256.png]]

-----
capas
general los sistemas de capas organizan a los so como jerarquias de capas
Es un diseño màs modular y escalable que el sistema monolitico

programa->  [capa2{capa1{capa0}}]


------
microkernel divide al sistema operativo en modulos pequeños y bien distribuidos con el objetivo de brindar confiabildiad al usuario

![[Pasted image 20260429093417.png]]

-----


------
Modelo cliente-servidor
Similar al modelo de microkernel con la diferencia q es posible diferenciar dos clases de procesos:
	Los servidores cada uno de los cuales proporciona cierto servicio
	Los clientes que utilizan estos servicios
![[Pasted image 20260429094212.png]]

-----
Maquinas virtuales 
Mediante se se proporciona a los programas la emulacion de un hw que no existe.
Se pueden ejecutar varias maquinas virtuales al msimo tiempo
Los recursos reales se reparten entre las distintas maquians virtuales

mediante sw se proporciona a los programas la emulacion de un hw que no existe
se pueden ejecutar varias maquinas virtuales al mismo tiempo
los recursos reales se reparten entre las distintas maquinas virtuales

ventajas: 

-----------
ping entre las dos máquinas virtuales

### Estados de procesos
El SO gestiona los recursos disponibles entre los procesos q en ese momento estan activos en el sistema de tal forma q para ellos el sistema se comporte como si fuera monousuario.

El principal concepto en any SO es el de proceso
Un proceso es un programa en ejecucion, incluyendo el valor del rogram counter, los registros yvariables
Cada proceso tiene un hilo thread de ejecucion que es visto como un CPU virtual.
El recurso procesador es alternado entre los diferentes procesos que existan en el sistema, dando la idea de que ejecutan en paralelo (multiprogramacion)

Cada proceso tiene un id

pc -> [proceso 1] pc -> [Proceso 2] pc-> [proceso n]
(esperando por recurso) (asignado al procesador) (esperando por recurso)
El proceso 2 -> Procesador 

### Memoria del proceso
Un proceso en memoria se constituye de varias secciones
codigo teext: instrucciones del proceso
datos (data); variables globales del proceso
memoria dinamica heap: mem dinamica que genera el proceso
pila stack: utilizado para preservar el estado en la invocacion anidadaa de procedimiento y funciones

## Modelo de dos estados:
Se trata de dos archivos, un objeto ejecutable 


MOdelo 5

![[Pasted image 20260504114617.png]]


Nuevo
Listo
Ejecucion
Espera
Terminado

"De ejecución a bloqueado: Se realiza esta transición cuando queda en espera"

man
ls
cd
mkdir
rm
cp
mv
pwd
find
grep
cat


-----
Maquina virtual VM Esuna instancia simulada de un so que se ejecuta sobre hw virtualizado. Cada VM actua como si tuviera sus propios recursos dedicados
Hipervisor: sw q permite 

---
Clases de virtualizacion
Virtualizacion de servidores


-------
## Contenedores / Contenización / Docker
responde a la misma necesidad de empaquerar una applicacion, pero crea una esrcutura contenedora mas liviana
Esta estructura solo contiene la aplicacion, sus dependencias y posiblemente algunos servicios del so en vez de un so completo.

se benefician de una forma de virtualziacion del so onde se usan caracteristicas del nucelo del so por ejm: espacios de nombres cgroups de linux, 
donde se usa virtualizacion y contenedores




# **Parcial II - Gestión de memoria**
## **Gestión de memoria**
evaluar cada uno de los temas de: la gestion de memoria desde el punto de vista academico y cientifico. 

Generar un informe del tema por cada uno de los conceptos que existen , relaciones a las nuevas tendencias - articulos academicos
scopus, google scholar

## **Gestión de dispositivos de E/S**
Es una de las responsabilidades clave del so para permitir la interaccion entre el Hw y los procesos del sistema. 
La gestion eficiente de e/s es crucial debido a las diferencias de velocidad entre los dispositivos de hw (discos, teclados, impresoras) y el procesador.
El SO debe proporcionar un nivel de abstraccion para que las aplicaciones no necesiten preocuparse por las complejidades de hw.

### **Organización de sistemas E/S**

### 2.1 componentes clave
**Controladores de dispositivo:**
sw q gestiona la comunicacion entre el so y un dipsoitivo especifico.
Ejm: un controlador para una impresora convierte comandso del so en señales entendibles para la impresora

**Colas de solicitudes**
Los dis E/S utilzian colas para gestionar multiples solicitudes de procesos.
Ejm: un disco duro almacena solicitudes de lec y wr en una cola y las procesa por oden o segun una politica especifica (como scan o c-scan)

**Spooling**
Simultaneous preripheral operations on line permite q un dispositivo lento como una impresoa almacene trabajs en un area temporal antes de procesarlos.
Ejm: En un entorno de oficina, las sollicitudes de impresion se almacenan en una cola mientras la impresona imprime trabajos en curso.

### 2.2. Politicas de organizacion
- **Acceso secuencial:** los datos se procesan en el orden en q estan almacenados
	EJM: Lectura de archivos en una cinta magnetinca
- **Acceso aleatorio:** los datos se acceden deirectamente en una posicion especifica
	Ejm: un  disco duro que busca un sector especifico para leer/wr datos
- **Programación de E/S:** determina el orden en el que las solicitudes de E/S se procesan,
	Ejemplo: uso de algoritmos como FCFS (First come, first served) o SCAN  para manejar solicitudes de disco.

Ejemplo practico: un sistema e cajeros automaticos requeire gestionar multiples dispositivos E/S
EN: Lectrura de tarjeta teclado
SA: impresion de recibos, visualizacion en pantalla. El sistema organiza las solicitudes de E/S en colas para evitar conflictos y usa controladores especificos para cada dospositivo

varios ingresos y soluciones simultaneas

**Capa de aplicacion:** Representa las aplicaciones del usuario, como programas de texto o herramientas graficas que generan solicitudes de E/S
**Capa del SO:** gestiona las solicitudes de E/S provenients de la capa superor. Incluye colas para oganizar las solicitudes y coordinar el acceso a los dispositivo
**Controladores de dispositivos:** Interfazan entre el sistema o. y los dispositivos fisicos como teclados, impresoras y discos.
**Hardware:** Dispositivos reales que ejecutan las operaciones de E/S

### **Interfaz de aplicaciones**
la interfaz con aplicaciones permite q las aplicaciones se comuniquen con lo dispositivos de hw a traves de llamadas al sistema
Esta interfaz abstrae los detalles del hw para facilitar el desarrollo de aplicaciones.
Las llamadas al sistema proporcionan una API (interfaz de programacion de aplciaciones) estandar para interactuar con dispositivos

### 3.2 Llamadas al Sistema más comunes
- read(): lee datos desde un dispo de E
	EJM: leer caracteres desde un teclado.
- write(): escribe datos en un dispo de S
	EJM: Enviar datos a una impresora.
- open() y close(): Abren y cierran la conexión con un dispositivo.
	EJM: Abrir un archivo para r/wr
- ioctl(): Proporciona control aanzado sobre un dispositivo.
	EJM: Cambiar la configuración de una tarjeta de red

3.3 Capas de abstraccion
capas superiores: 
interactuan con el sw del user
	EJM: un programa de edicion de texto usa la funcion write() para guardar datos en un archivo
capas intermedias: traducen las llamadas al sistema en comandos de hw
	EJm. un sistema de archivos convierte una solicitud de escritura en bloques en el disco
capas inferiores: comunican directamente con el hw mediante controladores

Ejemplo practico: una aplicacion de reproduccion de musica usa la interfaz de E/S para comunicarse con los altavoces:
open(): abre el dispositivo de audio
write(): envia los datos de la cancion del hw de audio.
close(): Libera el dispositivo al terminal


**Aplicaciones:** generan solicitureds como lectura, wr o apertura de archivos.
**Llamadas al sistema:** como read(), write(), y open (), actuan como puentes entre las aplciacioens y el hw
**Capas de abstraccion:** el so oculta las complejidades del hw y proporciona una API estandar apara simplificar la interaccion
**Dispositivos:** incluyen teclados, discos, impresoras, entre otros, que reciben las solicitudes y ejecutan las operaciones necesarias.


*Deber: instalación y configuración de dispositivos administrados sus interfaces E/S plataforma Windows, Linux y MacOS*


# **Parcial III - Sistemas de  Archivos**
## **Sistemas de Archivos.**
Necesidad de gestionar el almacenamiento volátil.
En el SO existe la necesidad de almacenar y recuperar informacion.
Cararcteristica fundamental del medio de almacenamiento: NO VOLATILIDAD
Variedad de medios donde almacenar informacion: discos magneticos, cintas magneticas, discos opticos, etc.
**Ventaja:**
Permite elegir el medio mas adecuado en funcion de las necesidades pariculares: cantidad de info a almacenar, velocidad de acceso, fiabilidad, etc...
**Desventaja:**
Requiere conocer las particularidades de cada medio

----
El sistema de archivos es la parte del sistema operativo encargada de administrar el almacenamiento secundario.
Es el responsable de la informacion y para q esta sea compartida por los usuarios de forma controlada.
Las funciones más importantes que debe realizar un sistema de gestión de archivos son las siguientes:
- Creacion de archivos: dar un name y reservar un espacio en disco.
- Borrar archivos: liberar el espacio q ocupaba
- Abrir archivos: para ser usados con las caracteristicas especificas (lectura (r), escritura (wr),ejecucion, etc)
- Cerrar archivos: para finalizar un prodceso e impedir su utilizacion posterior.
- Consultar archivos: en modo lectura, escritura, modificacion

a

----
Aparte de su contenido, todo archivo tiene atributos que lo describen:
nombre (cadena de caracteres)
tipo de archivo (necesario en sistemas que reconocen distintos tipos)
ubicacion en el dispositivos
tamaño
informacion de proteccion
fechas, horas e identificacion del user

**¿Que estructura nos permite organizar y acceder a los archivos?**
- Los atributos de los archivos deben guardarse en alguna estructura: Directorio o Tabla de contenidos.
- Los directorios al igual que los archivos deben ser no volatiles, se almacenan en disco
- Deben traerse a memoria cuando se necestian.

-----
Operaciones sobre archivos
La mayor parte de las operaciones implican buscar la entrada en el directorio asociada al archivo 

Mejora: Operaciones para open and close archivos
- Tabla de archivos open
- Indice, puntero, descriptor de 
.....
.
.

--------
La información guardada puede ser de muchos tipos.
Una tecnica comun para implementar lso tipos de archivos es incluir el tipo como parte del nombre del archivo (extension)
Basados en el tipo de archivo la estructura interna:
¿Debe el SO reconocer y manejar la estructura interna de diferentes tipos de archivos que pueden existir en un sistema?
Todos los.....

----------
Metodos de acceso
Archivo: Secuencia de registros logicos de longitud fija
De q manera se accede a la informacion alamacenada en los archivos?
	Algunos SO ofrecen un solo metodo de acceso mientras que otros ofrecen diferentes metodos de acceso
- Acceso secuencial

-
-
-

--------
Sistemas de archivos
SISTEMA DE ARCHIVO FAT
usa una tabla de 
.
.


Taller 1: Realizar una consulta bibliografica acerca de los diferentes tipos de archivos, con sus ventajas, desventajas, caracteristicas utiles y en que SO son o fueron usados (como se describe en linux, windows, ventajas y desventajas de cada SO)
Base: de donde se saca 

--------
Gestion de cuentas
Es el conjunto de mecanismos herramientas y politica


Lab1: realiza un lab en linux. 




## **Gestion de servicios MAIL/FTP**
Gestion de servicios MAIL. 
Los servicios de correo elec permite envir / recibir msj entre users. Se gestionan mediante protocolos como SMTP, POP3, IMAP.

![[Pasted image 20260708093616.png]]

------------
### SMT (Simple mail transfer protocol o protocolo simple de transferencia)
SMTP Procotolo usado para transferir correos electronicos entre svidores de correo electronico. Es el protocolo mas usado ya q permite enbiar y recibir msj a traves de diferentes redes y ordenadores.

(imagen)

----------
ventajas:
mayor velocdad de envio: iun sv smtp dedicado aumentara la velocidad de envio de tus correos, especialmente si lo comparas con los sv propios
mayot capacidad para archivos adjuntos
mejor entregabilidad

Desventajas:
protocolo inseguro
Velocidad limitada


-----
POP3 (post office protocol 3)
Protocolo usado para descargarmensajes de correo elecronico desde un servidor de correo electronico a un ordenador local o dispositivo movil. A diferencia de SMTP, POP3 Solo permite descargar mensajes y no enviarlos. Ademas, POP3 borra los correos del servidor una vez descargados.

![[Pasted image 20260708093922.png]]

------
Ventajas:
- Poder usar un cliente de correo para descargarlo en un dispositivo u ordenador, y poder leerlos luego aun sin tener conexion a internet
- .
Desventajas:
- Si el dispositivo donde estan almacenados los correos descargadors tiene una averia, es extraviado orobado se pierden los correos
- .

-----
IMAP (Internet message access protocol)
Protocolo que perimte el acceso a msj dde correo electronico q se encuentran almacendaos en un sv desde cualquier ordenador q tenga conexion a internet. Hay q indicar q imap es un procolo de acceso a nuestro correo electronico pero no es un procolo de envio de email.

![[Pasted image 20260708094343.png]]

Ventajas: 
- comunicacion bidireccional
- Los correos estan en todo momento en el servidor
- En caso de averia en el ordenador en el q este configurado el buzon, o si por cualquier razon se elimina la cuenta, siempre se puede recuperar.
- .
- .

------
Configuracion en linux:
- Servidores comunes: Postfix, sendEmail,exim.
- Configuracion basica en /etc/postfix/main.cf

myhostname = mail.ejemplo.com
mydomain = ejemplo.com
myorigin = $mydomain
inet_interfaces = all

configuracion en windows
.
.

-----
Gestion de servicios FTP
FTP (File transfer protocol)
servicio q se usa para el envio y disposicion de archivos entre 2 equipos (cliente - servidor,) mediante una red. Toma en cuenta que:
servidor ftp: sw ubicado en los sv conectados a internet o una red local LAN y permite q los clientes FTP puedan conectarse para subir odescargar archivos.
protocol ftp: metodo establecido para brindar el acceso a los users, asi como la red conectada que brinda soporte para eel elojamiento los distintos archivos.
aAcceso FTP: para acceder al sv ftp hace falta ...

---
FTP (File transfer proctol)
en este tipo de arq el sv estara esperado peticiones del cliente para transferir informacion ...
![[Pasted image 20260708094934.png]]


ventajas: conexion fast con el sv
desventajas:


TALELR: Realizar una investigacion bibliografica de los protocolos FTP, FTPS y SFTP, los cuales describan:

Caracteristicas
Funcionalidad
Semejanzas y diferencias
Ventajas y Desventajas para cada protocolo.






