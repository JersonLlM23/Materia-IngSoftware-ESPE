
#  UNIDAD 1 - Introducción a la red de datos.

## Decibelios:
En el contexto de la atenuación, los decibelios dB son la unidad de medida que se utiliza para cuantificar la perdida de intensidad de una señal. La atenuación es la reducción gradual de la amplitud de una señal a medida que se desplaza a través de un medio como un cable o aire

**Escala logarítmica**: El db es una unidad logarítmica que compara la potencia de señal en la entrada con la potencia de la señal en la salida. Esta escala es ideal para medir el amplio rango de intensidad de las señales.
**Pérdida de señal**: A diferencia de la ganancia (amplificación), la atenuación resulta en un valor negativo de db. Esto indica que la potencia de salida es menor que la de entrada.
Al ser negativo, significa que la potencia de entrada es menor a la que la salida?

------
0 dB: Significa que no hay perdida de señal.
-3 dB: Indica que la potencia de la señal se ha reducido a la mitad.
-6 dB: Significa que la potencia de la señal se ha reducido a la cuarta parte

**Factores de atenuación**: La atenuación se debe a diversos factores, como la distancia que recorre la señal el material del medio de transmisión y la frecuencia. Por ejemplo. en una red de telecomunicaciones la atenuación puede ser causada por inferencias de frecuencias de radio o fugas en los cables.

-------
Atenuacion: si introducimos una señal electrica con una potencia P2 en un circuito pasivo, como puede ser un cable esta sufrira una atenuacion ual final de dicho circuito obtendremos una potencia P1

La atenuacion (alpha) sera igual a la diferencia entre ambas potencias

en el ejercicio, si hacemos con 2.4 GHZ, 10 GHZ, 100 Ghz no varia pq?
muchos ejercicios más...

-----
**Transimisión**
Es la transeferencia fisica de datos (un flujo digital de bits) por un canal de comunicación punto a punto  o punto a multipunto.
Según el sentido de la transmisión, existen 3 tipos diferentes de medios de transmisión.

- Simplex (como antena -> TV)
- Semi-Dúplex (half-duplex) ejemplo un walkie talkie (puedes hablar o escuchar, no los dos a la vez)
- Dúplex o dúplex completo (full - duplex)


Pst: Un bit son la unidad de medida de la información (0,1)
 y un byte? 
 
  -------------------
 **Transmisión paralela** : De datos de byte a byte, sobre un minimo de 8 lineas a traves de uan interfaz paralela.
**Transmision en serie**: es le envio de datos bit a bit sobre una interfaz de serie (es el más seguro para enviar datos)
grafico byte

------------
**Sistema de comunicacion:** La composiscion de una red depende en gran meduida del ontexto podria ser un modelo de comunicacion simple una red publica de  conmutacion o una red de area local (LAN)
Modelo de comunicacion simplificado:
grafico


ejm: fuente de zoom 
Fuente: docente
Transductor de entrada (señal mecanica -> digital y viceversa): microfono
Transmitor: PC/ZOOM
Medio de transmision: red
Receptor: pc/zoom
Transductor de salida: parlantes 
Destino: Estudiantes

2 Graficoo
3 graficos 

--------
Red de area local LAN: 
control de acceso al medio
protocolos: conjunto de instrucciones
topologia
medio de transmision 

La seguridad: es el elemento que permite garantizar la confidencialidad la autenticacion y la intergridad de los datos.

----------
Componentes de una red
- Medios no guiados o inalámbricos
- Medios guiados o alámbricos
		Cable coaxial: conexion antena a TV
		Cable Par trenzado: 
		Fibra Optica



## Clase 4:
Direccion ip: ...
Tiene 3 clases:
CLASE A: 10.40.X.X  pocas redes pero muchos dispositivos
	mascara:
		11111111 00000000 00000000 00000000
		 RED        |   HOST
		 2^n            2^n
		 2^8            2^24
		
CLASE B: 172.16.X.X
		 11111111 11111111  |  00000000 00000000
		 RED                                HOST
		 2^16                              2^16

CLASE C: 192.168.X.X
		 11111111 11111111  11111111 | 00000000
		 RED                                                HOST
		 2^24                                              2^8


Mi direccion ip:
 10.240.0.255 (CLASE A) -> 10.40.X.X

- Direcion IP -> 1PV4, 1PV6
- MÁSCARA RED -> Se puede configurar hasta:

- GATEWAY Puerta que me permite salir de una red hacia otra red
- 



![[Pasted image 20251021095529.png]]

Ejemplo con CLASE C_
Direccion RED:  192.168.0.0    abarca todas las direccioens ip de las habitacion de nuestra casa 
Direccion IP/HOST: 192.168.0.5
MASK: 255.255.255.0 ?
GATEWAY: puerta donde un equipo sa
![[Pasted image 20251021095853.png]]
192.168.0.0
255.255.255.0 a binario ->
 11111111 11111111  11111111 | 00000000
RED				 2^24                            2^8  HOST

							#dispositivos: 2^n -2
							 2^8 -2=254 -> IP RED , IP BROODCAST
El gateway seria la siguiente direccion IP de la direccion de red:

192.168.0.0
192.168.0.1
.
.
.
192.168.0.254  se puede configurar hasta aqui (=) porque es el broodcast, desde el 0.1 hasta 0.254 es el host
192.168.0.255

Gateway: 192.168.0.1
(Servidor) DNS: domain ned server
(servidor) DHCP: suele ser iguall que la puerta de enlace predeterminada (gateway) esto debido a que posiblemente un equipo puede ser firewall. Se encarga de 


Topologia es la forma en la que se conectan los ordenadores
Estrella:
![[Pasted image 20251021105053.png]]
Bus: conectados en linea
Anillo: conectados en circulo
Jerárquica: 
1. Core/Nucle -> hacia internet
2. Distribucion
3. acceso
4. PC/LAPTOPS/IMPRESORASS


## Clase 5 creo
Recordatorio de los tipos de direccionamiento ip?

**Clase A** 
IP inicio:  0.0.0.0
IP final: 127.255.255.255

Máscara de red:
	Digital: 255.0.0.0
	Binario: 11111111.00000000.0000
	Reducido: /8
	
**Clase B**
IP inicio: 128.0.0.0
IP final: 191.255.255.255

Máscara de red:
	Digital: 255.255.0.0
	Binario: 11111111.11111111.00000000.00000000
	Reducido: /16

**Clase C**
IP inicio: 192.0.0.0
IP final: 223.255.255.255

Máscara de red:
	Digital: 255.255.255.0
	Binario: 11111111.11111111.11111111.00000000
	Reducido: /24

-------
Ejemplo: 
**Dirección Red: 192.168.16.0  /24**

Binario: 11111111.11111111.11111111.00000000
REDES:  11111111.11111111.11111111 -> 16777216 redes 
HOSTS: 00000000 -> 256 hosts 

por lo tanto, la RED{ :
Dirección red: 192.168.16.0
Mascara: 255.255.255.0

Gateway {
desde: 192.168.16.1 
hasta: 192.168.16.254
	    }
dirección broadcast: 192.168.16.255
}
hay dos direcciones que no se ocupan, por lo tanto la fórmula para calcular el numero de redes:
(2^n), y para el numero de hosts seria: (2^n) - 2

-----
### ¿Cuántas subredes puedo configurar para que en cada subred haya solo 24 host? Usando la dirección clase C: 192.168.17.0 /24

1. **Calcular n dependiendo si son hosts o redes.** 
	Usamos:  (2^n) - 2. Para que n sea igual o mayor a 24 sería *n=5*
2. **Usar la notación binaria:**
	Binario: 11111111.11111111.11111111.{00000000} 8 bits
	Cuando nos piden hacer host, nos ponemos desde la *derecha hacia la izquierda* por lo tanto:
	Binario: 11111111.11111111.11111111.000  (0  0  0  0  0) 5 ceros porque n=5, los 3 ceros faltantes, les convertimos en red (1)
	Binario: 11111111.11111111.11111111.111  (0  0  0  0  0) ahora es /27, en decimal sería:
	Máscara: 255.255.255.X 
3. **Calcular X.**
	En este caso, podemos iniciar asi: 
	128  64   32   16   8    4   2   1 
	  1   1    1     0    0   0   0   0
	Y.. suma los números donde están los 1 -> 128+64+32 = 224 por lo tanto:
	*Máscara: 255.255.255.224* 
4. **Cuantas subredes se pueden obtener**
	*Primera subred: 192.168.17.0  /27*
		Desde: 192.168.17.1 
		Hasta: 192.168.17.30
	BroadCast: 192.168.17.31  /27


	*Segunda subred: 192.168.17.32  /27*
		Desde: 192.168.17.33 
		Hasta: 192.168.17.62
	BroadCast: 192.168.17.63


	*Tercera subred: 192.168.17.64  /27*
		Desde: 192.168.17.65 
		Hasta: 192.168.17.94
	BroadCast: 192.168.17.95


	Cuarta subred: 192.168.17.96 /27



	Quinta subred: 192.168.17.128 /27


	Sexta subred: 192.168.17.160/27


	Séptima subred:  192.168.17.192/27


	Octava subred:  192.168.17.224/27

-------
### Ahora, configurar 2 subredes y calcular cuantos host por cada subred puedo configurar.

1. **Calcular n dependiendo si son hosts o redes.** 
	En este caso ahora usamos 2^n . Nos dice 2 subredes, entonces 2^n = 2. Para que se cumpla esta igualdad, *n=1*
2.  **Usar la notación binaria:**
	Binario: 11111111.11111111.11111111. | 00000000
	Cuando nos piden hacer subred. nos ponemos desde la *la raya de izquierda a derecha* por lo tanto:
	:            11111111.11111111.11111111. | 10000000
Máscara: 255.255.255.X /25
3. **Calcular X.**
	En este caso, podemos iniciar asi: 
	128  64   32   16   8    4   2   1 
	  1   0    0     0    0   0   0   0
	Y.. suma los números donde están los 1 -> 128 = 128 por lo tanto:
	*Máscara: 255.255.255.128* 
4. **Cuantas subredes se pueden obtener**
	1ra subred: 192.168.17.0  /25
			Desde: 192.168.17.1 
			Hasta: 192.168.17.127
	Broadcast: 192.168.17.127

	2da subred: 192.168.17.128  /25		
			Desde: 192.168.17.129
			Hasta: 192.168.17.254
	Broadcast: 192.168.17.255

-----
Cuantas subredes puedo obtener de la red 192.168.19.0 /24 para que en cada subred haya unicamente 2 host. Escribir las 5 primeras subredes especificando: Direccion de red, direccion de broadcast, rango de direcciones 

## Clase 6

11111111.11111111.00000000.00000000

octeto: 11111111
16 bits puedo configurar subredes: .00000000.00000000
## Configurar 16 subredes con ip clase B 172.16.0.0 /16 y responder: Cuantos hosts por subred puedo configurar. Describir las 5 primeras subredes (dirección red, rango ip, dirección broadcast)

11111111.11111111.00000000.00000000

subredes: 2^n
hosts: (2^n)-2
Salto = 256 − (valor decimal del último octeto de la máscara)
Ejemplos:
- Máscara 255.255.255.252 → salto = 256 − 252 = 4 (subredes cada 4)
- Máscara 255.255.255.224 → salto = 256 − 224 = 32 (subredes cada 32)

Como nos pide configurar  subredes usamos esta formula:
			2n=16   n=4
11111111.11111111 | .~~0000~~0000.00000000
				   ->  n=4
11111111.11111111 | .11110000.00000000  /20

128 64 32 16 8 4 2 1
1     1   1    1  0 0 0 0 
128+64+32+16=240 por lo tanto
255.255.240.0 /20
1.forma Salto = 256-240 = 16 (se puede configurar 16 subredes)
host x subred = 2^12 -2 = 4094  ( por cada subred, se puede configurar 4094 hosts)

2forma: 2^4 = 16

1 Subred: 172.16.0.0 / 20 -> Dirección subred
Rangos de IPs:  172.16.0.1 - 172.16.15.254
Dirección del BroadCast: 172.16.15.255


2 Subred: 172.16.16.0 /20 -> Dirección Subred
Rangos de Ips: 172.16.16.1 - 172.16.31.254
Dirección del BroadCast: 172.16.31.255
	

3 Subred 172.16.32.0/20

# UNIDAD 2 -

## SSID
2.4 GHz trabaja el WIFI, en equipos inalámbricos hay canales
La red wifi tiene 11 

Port Status
SSID
2.4 Ghz Channel
Coverage Range 
Authentication.
![[Pasted image 20251120093154.png]]

----
## Diferencia entre fast Ehternet, GigaBitEthernet
IEEE 802.3

Fast Ethernet: 
- Velocidad: 100 MBPS  
- Estándar: 802.3u
- Distancia máxima: 100 metros
- LAN corta, mediana distancia
- Aplicaciones: Conexión internet banda ancha.
- Si se envía un archivo de 1GB: 80 seg
Gigabit Ethernet
- Velocidad: 1000 MBPS
- Estándar: 802.3ab
- Distancia máxima: 100 metros
- LAN larga distancia
- Centros de datos, conexión internet alta velocidad.
# UNIDAD 3

Direccionamiento IP:
CLASE A: 255.0.0.0         /8        256 REDES / 16 M hosts
CLASE B: 255.255.0.0      /16     65000 REDES / 65 000 hosts
CLASE C: 255.255.255.0  /24     16 M REDES /254 hosts

-------
Subneting:
Hosts= 2^n -2
Redes = 2^n 

192.168.10.0/24 Redes con 254 hosts (sin subneting)
Configurar redes que tengan 58 hosts por cada subred.
	   Como dice configurar hosts, entonces usamos: 2^n -2
		 Hosts = 2^n -2
	     2^n -2 = 58 (mayor o igual)
	     n=6, por lo tanto, se puede configurar.
	     Si tomamos n=6 en redes clase C , sobran 2 para la otra cosa jij
	     2^2 = 4 subredes


-------
4 Departamentos financieros con 50 hosts, tecnológicas 25 hosts, desarrollo 10 hosts, auditoria 5 hosts. Configurar el direccionamiento ip pero usando VLSM.

1. **Ordena los requerimientos de mayor a menor. (El departamento con mayor # de requerimientos)**
	Financiero = 50 hosts
	Tecnologías = 25 hosts
	Desarrollo = 10 hosts
	Auditoria = 5 hosts	 

2. **Halla las máscaras de red para cada departamento.**
	 Financiero = 50 hosts.
		 Hosts = 2^n -2
	     2^n -2 = 50 (mayor o igual) 
	     n=6
	     Máscara: /26 (255.255.255.192)
	Tecnologías = 25 hosts
		  Hosts = 2^n -2
	     2^n -2 = 25 (mayor o igual) 
	     n=5
	     Máscara: /27 (255.255.255.224)
	 Desarrollo = 10 hosts
		  Hosts = 2^n -2
	     2^n -2 = 10 (mayor o igual)
	     n = 4
	     Máscara = /28 (255.255.255.240)
	 Auditoria = 5 hosts
		  Hosts = 2^n -2
	     2^n -2 = 5 (mayor o igual)
	     n=3
	     Máscara = /29 (255.255.255.248)


3. Asignar direcciones ip para cada departamento:
	**Financiero:** /26
		Dirección RED: 192.168.10.0
		Rango IP: 192.168.10.1 - 192.168.10.62
		Broadcast: 192.168.10.63
		Saltos: (64)

	**Tecnologías:**  /27
		Dirección RED: 192.168.10.64
		Rango IP: 192.168.10.65 - 192.168.10.94
		Broadcast: 192.168.10.95
		Saltos: (32)

	**Desarrollo:**  /28
		Dirección RED: 192.168.10.96
		Rango IP: 192.168.10.97 - 192.168.10.110
		Broadcast: 192.168.10.111
		Saltos: (16)
		
	**Tecnologías:**  /29
		Dirección RED: 192.168.10.112
		Rango IP: 192.168.10.113 - 192.168.10.118
		Broadcast: 192.168.10.119
		Saltos: (8)

-------
Agregando un nuevo departamento:
Gerencia = 2 hosts

   Gerencia = 2 hosts
		  Hosts = 2^n -2
	     2^n -2 = 2 (mayor o igual)
	     n=2
	     Máscara = /30 (255.255.255.252)

		Dirección RED: 192.168.10.120
		Rango IP: 192.168.10.121 - 192.168.10.122
		Broadcast: 192.168.10.123
		Saltos: (4)



--------
## Router 
- Interconectar diferentes redes.
- Encaminar paquetes de datos.
- Componentes básicos:
	- CPU: Procesar decisiones de enrutamiento.
	- RAM: Random Access Memory, ejecuta el IOS y guarda las tablas del router.
	- NVRAM: Guardar la configuración (startup-config)
	- Flash: Almacena el sistema operativo IOS
	- Interfaces Fast, Ethernet
- Tipos.
	- Según el entorno:
		- Entorno doméstico
		- Entorno empresarial
		- Router ISL (core router)
	- Según la tecnología
		- Router inalámbrico
		- Router cableado
		- Router Virtual (router-on-a-stick, Routers en la nube)
- Funciones
	- Separar dominios de broadcast
	- Seleccionar la mejor ruta
	- Conectar diferentes
	- Implementar funciones de seguridad (ACL, NAT, FireWall)
	- Soportar protocolos de enrutamiento.

## Enrutamiento (direcciones IP, máscaras y métricas)
1. Recibir un paquete de datos.
2. Analizar la IP de destino
3. Consultar su tabla de enrutamiento
4. Decidir por donde enviar el paquete
- show ip route (redes conectadas )
- **Tipos de enrutamiento:**
	- Directo (Redes conectada directamente al router. Se agrega de forma automática)
	- Estático (Rutas configuradas de forma manual por un administrador)
		- **Ventajas** (Simple, seguro, bajo consumo).
		- **Desventajas** (No escalable, No se adapta a los fallos
	- Ruta por defecto (Se usa cuando no hay una ruta específica)
		- Routers por borde
	- Dinámico: (Routres, aprenden las rutas de forma automática mediante protocolos)-
		- RIP: Vector distancia / saltos
		- OSPF: estado de enlace / costo
		- EIGRP: Híbrido / ancho de banda
		- BGP: Vector ruta / políticas



-----
## WildCard 
**Máscara de red, aplicando el complemento**
A: 255.0.0.0
B: 255.255.0.0
C: 255.255.255.0

Ejm: 
10.10.10.0/30
255.255.255.252 -> Para llegar a 255.255.255.255 es: 0.0.0.3

**Process ID** : 1 Hasta el 65535


#configure terminal
config# router ospf 1
config-router# network 192.168.0.0 0.0.0.255 area 1
config-router# network X.X.X.X 0.0.0.3 area 1
config-router# network Y.Y.Y.Y 0.0.0.3 area 1

config terminal
config# interface serial 0/X/0
config-if# bandwith 50