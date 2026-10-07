# Unidad I

Jugador - entrada - logica - motor- render - resultado

Entradas: Teclado, mando, táctil.
Lógica: Reglas: vidas, puntos
Físicas: gravedad, colisiones
Gráficos: sprites y escenarios
Audio: pasos, música
IA: enemigos q me persiguen
Interacción: recoger, abrir
Tiempo real: todo se actualiza en cada frame

Gameloop: el corazón de todo videojuego
Gameloop: ciclo q repite todo
Update: acutaliza la logica
REndering: dibuja cada frame
scenes: niveles y menus
input: lo q hace el jugador
physics: movimiento y choques
eventos: algo ocurrio
objets/nodes piezas del juego

----
Variables: guardan vidas, puntos
funciones: acciones reutilizables
_ready() y process()
al iniciar / escala frama
señales: avisan q algo ocurrio

En godot, cada script se adjunta a un nodo y hereda sus capacidades con extends.

Un videojuego es un sistema de sw complejo.
Prototipo fast:
Todo en script - rapido hoy, fragil mañana - dificil de compartir.
VIdeojuego mantenible:
modulos y escenas: git - pruebas - facil de amplar en equipo


-----
Ciclo devida de un vj
idea (requisitos: q debe tener el videojuego)
diseño (arquitectura: escenas y modulos)
codigo (programacion: codigo modular)
integracion (git: unir el work)
pruebas ( pruebas: jugabilidad y unitarias)
ajuste (mantenimiento: refactorizar)
version (relase: version estable)

el ciclo de vida es iterativo: cada version vuelve a la idea con lo aprendido

------
Arquitectura básica:
Entrada del jugador - Lógica del juego - Entidades / Escenas - Motor  - Render - audio - física

Separacion de responsabildiades: cada script debe hacer 1 cosa
Modularidad: piezas independientes
reutilizacion: una escena, muchas copias
mantenibilidad: cambiar sin romper

-----
CControl de versiones y trabajo en equipo
git: la maquina del tiempo de tu proyecto.
repository: carpeta con historial
commit: foto del proyecto
branch: rama para probar ideas
merge: une dos ramas
versionado

-----
teoria: acoplamiento y cohesion
dos ideas que deciden si tu juego crece sano
alto complamiento: player.gd modifica directamente el hud, el puntaje y a los enemigos
bajo complamiento: el jugador emite una señal y cada sistema decide como reaccionar

Resp. unica: un script - una tareaa.
cohesion alta: lo relaciono va junto
acoplamiento bajo: pocas dependencias

si cambiar el puntaje te obliga a editar player.gd, hay acoplamiento

---------
Patron de diseño
Como una receta: no reinventamos como cocinar cada vez
Problema recurrente -> solución conocida -> patrón de diseño

Problema: muchos elementos necesitan avisar al HUD (patron: observer)
Problema: un personaje con muchos comportamientos (patron state)
problema: un oslo gestor de la partida (singleton)
Un patron es una idea reutilizable, no code para copiar y pegar.

------
Singleton
un unico gamemanager global
player - enemy - hud - gamermanager

observer: coin recogida - evento - puntos
jugador recoge monedas - envento coin_collected - score manager +10

state
un estado activo a la vez
idle - run - jump - attack - dead

-------
patron sate:
Un solo estado decide el comportamiento:
idle - run - jump - dead
organizacion clara, mantenimiento facil, añadir estados nuevos, menos if anidados

----
observer y singleton
ventaja o: el emisor no conoce a lo receptores
riesgo: demasiados eventos son dificiles de rastrear

ventaja s: acceso global simple al gamemanager
riesgo: estado global y dependencias ocultas

------
Motor de videojuegos:
Divide el trabajo para que programes tu juego.
Conjunto de herramientas que permite construir y ejecutar un videojuego.
Rendering dibuja graficos
fisica: colisiones
audio: sonido
animacion (movimiento)
escenas: niveles y menus
entrada: teclado y mando
scripting: gdscript
recursos: modelos (blender)

