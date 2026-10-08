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

----
Godot
ingredientes -> motor -> videojuego.
(Codigo - escenas - recursos - fisica - audio - input) -> godot engine -> videojuego 

node: pizza
scene: conjunto de nodos
scene tree: arbol de nodos
inspecto edita propiedades
script gdscript
signals eventos

---
Como elegir un videojuego?
tipo de juego: 2d, 3d, movil, web
equipo y experiencia: lenguajes q ya se conocen
plataforma de deiseño: pc, movil, consola, web
licencia y costo: libre, gratuita o de pago
comunidad y documentacion: tutoriales
rendimiento y escala: tamaño del proyecto

No existe el mejor motor: existe el más adecuado para el proyecto

-----
del code a videojuego
programacion -> ing sw -> patrones -> motor -> videojuego.

Un juego es un sistema vivo: cada mecánica bien ordenada te permite añadir la siguiente sin romper lo anterior

-----
Que es diseñar un juego
idea - diseño - produccion  - pruebas - lanzamiento

Diseño: define q hace el jugador y pq es divertido
programacion: hace lo diseñado funcoine
documento: gdd (guia comun todo el equipo)
Un buen diseño evita cambios costosos durante el desarrollo 

------
8 pasos del diseño:
1. idea
2. publico
3. genero
4. mecanicas
5. reglas
6. narrativa
7. arte y sonido
8. prototipo

despues documentar (gdd) · definir el alcance actividad en grupos

----
roles en la fase de diseño.
Un videojuego se diseña en equipo.
Director creativo.- define la vision del game
game designer.- mecanicas, reglas y bucles
level designer.- estructura y ritmo de los niveles
narrative designer.- historia, personajes y dialogos
diseñador ux/ui.- interfaz y experiencia del usuario
artista / dir. de arte.- estilo visual coherente
diseñador de sonido.- efectos y musica
programador.- viabilidad tecnica y prototipos
productor.- planifica tiempo y alcance
qa/tester.- prueba y reporta problemas.

En equipos pequeños, una persona cumple varios roles

-------
1. Idea: director creativo. game designer
2. publico y plataforma.- productor, diseñador ui,ux
3. genero y referencias game desginer, dir. de arte
4. mecanicas: game designer, programador
5. reglas y objetivos: game designer, level designer, qa
6. narrativa y mundo: narrative designer, artista
7. arte, sonido einterfaz: artista ,sonido, ui/ux
8. prototipo y pruevas


-------
PASO 1: LA IDEA Y EL CONCEPTO
resumme tu juego en una sola frase:
Un (personaje) que (accion) en (mundo) para (objetivo)
ejm: un robot que recoge baterias en una cueva oscura para volver a casa

PASO 2: Público y plataforma
Jugador objetivo: edad y experiencia
Duración: sesion de 2 min o de 1 hr
plataforma: pc, movil, o web
controles: teclados, tactil o mando
accesibilidad: contraste subtitulos, daltonismo
alcance: equipo y tiempo disponible

Ejemplo: juego casual de 5 min para movil en un solo boton

Paso 3: genero y referencias
plataformas: saltar y esquivar
puzzle: resolver acertijos
arcade: puntuacion y reflejos
aventura: explorar y narrar
estrategia: planificar recursos
supervivencia: gestionar riesgo.

elige 2 juegos de referencia y anota q tomaras de cada uno

PASO4: Mecanicasy buble de juego
el core loop es lo q el jugador repite:
accion -> regla -> respuesta -> recompensa -> repetir


paso 5: reglas y objetivos
objetivo: q debe lograr
victoria: cuando gana
derrota: vidas o tiempo
dificultad: sube gradualmente

paso 6:  narrativa, personajes y mundo
da contexto y motivacion al jugador

Personaje -> conflicto -> mundo -> meta
(qn es y q quiere) -> (q se lo impide) -> (donde ocurre y sus reglas) -> (humor misterio o epico)

Paso 7: coherencia visual y sonora antes q complejos complejos
arte (krita). un estilo visualmente coherente
3d (blender): solo si el alcance lo permite
audio (audacity): efectos y musicas simples 
intefaz (hub): mostrar solo lo necesario

Paso 8: prototipo, y pruebas de jugabilidad
probar pronto es mas barato q corregir tarde
papel - prototipo - playtest - ajustes - iterar

prototipo en papel
playtest
anota lo q el jugador hace, no solo lo q dice

-------
El documento de diseño (GDD)
guia viva del proyecto
concepto pitch y publico
mecanicas bucle y reglas
niveles estuctura y dificultad
personajes rol y aspecto
arte y audio estilo y referencias
tecnologia motor y herramientas
alcance mvp y prioridades 
cronograma hitos y responsables
se acualiza con cada decision del equipo


-----

Alcance y planificacion. iseña pequeño, termina y luego amploa
imprescindible mvp (movimiento, objetivo, victoria o derrota)
deseable (sonido, niveles extra, menu)
opcional (logros, historia, multijgador)
mvp: la version minima q ya se peude jugar
error comun: diseñar un juego enorme para un equipo pequeño

----
