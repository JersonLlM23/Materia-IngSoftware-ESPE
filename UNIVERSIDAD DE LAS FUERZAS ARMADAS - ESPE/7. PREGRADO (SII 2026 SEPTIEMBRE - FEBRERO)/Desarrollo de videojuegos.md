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