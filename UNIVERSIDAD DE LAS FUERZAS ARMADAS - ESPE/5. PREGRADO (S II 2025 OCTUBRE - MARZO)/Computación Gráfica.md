# UNIDAD 1
## Transformaciones Geométricas en 2D
Se refieren a operaciones que modifican la posición, orientación, tamaño o forma de objetos bidimensionales.
## **Translación**
Mueve un objeto de una posición a otra sin cambiar su forma tamaño u orientación.
x'=x+T_x , y'= y+T_y

## **Rotación**
Gira un objeto alredeor de un origen o un punto fijo.
Fórmula (rotación antihoraria):
x' = x cos (tetha) - y sin (theta)
y'=x sin(tetha) + y cos (theta)

## **Escala**
Cambia el tamaño de un objeto.
x'=x * S_x 
y'= y * S_y


-----------

# UNIDAD 2
## Ec. Circunferencia 
x^2 + y^2 = r^2 en el centro.
Precisa utilizar raiz cuadrada y redondeo uso del punto flotante
dibujo de la circunferencia con huecos 

simetria de 8 lados

Suposiciones inidciales:
1. La circunferencia tiene centro en h,k
2. Radio = r
3. Se trabaja inicialmente en el primer octante (debido a la simetria de la circunferencia) y los resultados se reflejan a los demas octantes

Inicializar los valores:
Si p<0 El siguiente pixel está dentro o sobre la circunferencia, . .. .

Algoritmo de relleno de figuras
los algoritmos de relleno de figuras son los utilizados para ortorgar o reemplazar el color existente dentro de las  celdas o pixeles q componen una figura (mapa de bits)
Se suele realizar la opcion conocida como "bote de pintura" que con hacer clic dentro de una region, se pintaba.
El algoritmo se conoce como FloodFill, un metodo recursivo que trabaja usando una pila en la que almacena todas las posiciones que conforman la zona a colorear.
Se ingresa 1 punto dentro de la figura este es el punto inicial. Se cambia su color al deseado.
Se realiza una verificacion de los puntos vecinos ya sea tomando cuatro direcciones (S,N,E,W) y se almacena en la pila
Se saca el ultimo elemento de la pila, se cambia su color y nuevamente se verifican sus vecinos

Crea un programa que permita dibujar figuras mediante líneas rectas e implementar el algoritmo de relleno de figura. Adicionalmente se deberá mostrar la lista de pixeles que serán pintados.
Dar un "punto semilla" y a partir de ese punto que se vaya rellenando (lista de pixeles calculadors usando un textbox, o textboxarea, etc) El relleno debe ser animado.
Busca 2 algoritmos más de circunferencia
Busca 2 algoritmos más de relleno para no petar la maquina implementa


---------
## Algoritmos de relleno de figuras.
El algoritmo de Cohen-Sutherland es un método eficiente y ampliamente usado para recortar líneas en computación gráfica.

### **Codificación de regiones**
1. Asignación de códigos

![[Pasted image 20251202113834.png]]
1. Caso trivial de aceptación: si ambos extremos tienen el codigo 0000 la línea esta completamente dentro de la  ventana y se acepta.
	Caso trivial de rechazo: si la operacion lógica AND entre los códigos de ambos extremos no es 0000, la línea esta completamente fuera de la ventana y la rechaza.
2. Recorte: si la linea no es aceptada ni rechazada directamente, se calcula la interseccion del segmento con los bordes del a ventana. 
	Se recorta el extremo que está afuera de la ventana y se repite el proceso con el nuevo segmento.

p1: 0101
p2: 0110 
AND: 0100 (si hay dos 1, entonces es 1)
Como es diferente de 0000, 


p1: 0010
p2: 0001
AND: 0000
Hallar la interseccion

con este algoritmo usaremos el recorte en algoritmos

------
Recorte de poligonos
Algoritmo de Sutherland hodgman
Es una tecnica usada para recortar un poligono arbitrario (normalmente convexo) contra una ventana del recorte.

input: 
lista de vertices en sentido horario / antihorario
ventana de recortes

algoritmo de recorte
lineas
elipses
relleno
recorte


--------
## Curvas Bézier.
Pierre bezier
Las curvas permiten representar trayectorias suaves y controlables mediante un conjunto de puntos de control.

es una curva parametrica definida mediante una combinacion lineal de puntos de control. Los puntos de control determinan la forma de la curva y esta se genera interpolando entre dichos puntos segun una formula matematica especifica basad en polinomios de bernstein.
