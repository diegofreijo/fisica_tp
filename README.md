# TP de Nociones de Física 1

## Metodología

|                        |                               |
| ---------------------- | ----------------------------- |
| Integrantes por grupo: | 1 o 2                         |
| Se aprueba con         | 6                             |
| Fecha de entrega       | Domingo 9 de Junio, 23:59 hs  |
| Fecha de re-entrega    | Domingo 16 de Junio, 23:59 hs |

### Objetivos

- Aplicar en Unity los conceptos de física que vimos en clase.
- Familiarizarse con Unity y un poco con C#.
- Mejorar el trabajo en equipo.
- Aprender a aclararse las dudas de los requerimientos ambiguos.

### Comentarios Adicionales

No les pido que entreguen un juego completo. Estas son solamente demos técnicas, muestran una simulación física. En los próximos años van a aprender todas las partes que se necesitan para armar un juego completo.

Quiero darles la mayor libertad posible para que los resuelvan como quieran. Incluso pueden no usar lo que vimos en clase si saben otra forma. Pueden usar Google, trabajar junto a otros equipos, usar ChatGPT, etc. 

Lo que les pido es que:

- Estén hechos en Unity.
- Si trabajaron junto a otro grupo, no me entreguen el mismo TP. Cada grupo debería implementarlo a su manera.
- Si usaron algo que no vimos en clase, me justifiquen en el oral por qué les pareció mejor opción.

Pueden usar cualquier pack de gráficos que gusten. En clase siempre usamos los de Kenny pero pueden googlear y van a encontrar muchos mas y gratis. Hasta pueden dibujarlos ustedes si quieren, pero no lo recomiendo porque les va a llevar mucho tiempo. Recuerden que acá no voy a evaluar el arte que produjeron.

Si tienen dudas, pregúntenme. Podrían terminar perdiendo mucho tiempo por no preguntarme algo.

Recuerden que, por lo general, la solución más simple es la mejor.

----

## Entrega

### Para los de primer año

Para entregarme, van a hacer lo siguiente **antes de la fecha de entrega**:

1. Cerrar Unity y Visual Studio Code
2. Borrar la carpeta `Library`, pesa mucho y no sirve enviarla
3. Comprimir toda la carpeta del proyecto en un `.zip`
4. Mandarme el `.zip` a me@diegofreijo.com

Antes de ese horario me tienen que mandar el link del repo por mail a <me@diegofreijo.com>.

Tiene que haber una `tag` que se llame `tp1`. Ese commit es el que voy a corregir.

Si crearon branches por feature o por ejercicio, no los borren. Así puedo ver cómo estuvieron trabajando. Pero para este TP no es necesario que se vuelvan locos con GitFlow. Igual les recomiendo que lo practiquen si pueden porque para los demás TPs va a ser necesario.

### Para los de segundo año

Me lo mandan por `git` a me@diegofreijo.com y con un tag `tp` como ya saben hacer gracias a Programación 2. 

Recuerden crear un `.gitignore` o usar el que usamos en clase para no estar subiendo cosas pesadas.

### Defensa oral

Va a ser por Google Meet. Me van a explicar lo que hicieron, por que lo hicieron, etc. El horario exacto para cada grupo lo voy a estar mandando después de la entrega.

### Re-entrega

Si no aprobaron la entrega, o quieren subir la nota, pueden re-entregar una semana mas tarde. También les voy a tomar una defensa oral en la re-entrega.

----

## ArcoHombre

Vamos a desarrollar una versión bien simple de [Bowman](https://www.crazygames.com/game/bowman), Angry Birds, [Gravity Fleet](http://coffeepoweredmachine.com/gravity-fleet/), etc.

No vamos a tener las cosas que lo hacen un "juego" como una UI con un menú principal, flujo de juego, input del jugador, puntajes, etc. Solamente me interesa que armen escenas donde muestren los conceptos de física que vimos en clase.

No hace falta que la cámara se mueva. Todas las simulaciones pueden suceder en el espacio que ocupa en la pantalla.

No hace falta que implementen las funciones cinemáticas "a mano" en C#, como les mostré al principio de la clase 4. Mejor va a ser que usen todas las herramientas físicas que trae Unity.

Todos los ejercicios van a ser en 2 dimensiones, como vimos en clase.

## Ejercicios

### 1. Flechas 🎯(4 puntos)

Primero vamos a armar una escena parecida al Bowman original. En una punta va a estar el personaje que disparando. En la otra punta, varios objetos. 

Al darle play a la escena el personaje va a lanzar al menos 2 tiros en distintos angulos y/o potencias de tiro. La idea es que alguno le pegue a los objetos en la otra punta.

Fíjense que acá no estamos pidiendo el input del usuario. Los disparos no se van a realizar en base al ángulo o potencia del mouse del jugador. Esos valores los pueden configurar en el inspector de Unity como vimos en clase.

No hace falta que el pack de gráficos sea un arquero tirando flechas. Puede ser un tanque tirando balas, una gomera tirando pájaros, etc. Lo mismo con los objetos: pueden ser cajas, chanchos, autos, pelotas, etc. Usen lo que gusten.

### 2. Explosiones 💥(3 puntos)

La segunda escena va a ser parecida a la primera, pero esta vez las flechas van a explotar! La idea es que logren lanzar por los aires a al menos un objeto de los que posicionaron. Otra vez, debería disparar al menos 2 veces.

### 3. Tejo ⛱️ (3 puntos)

En esta escena vamos a estar jugando al tejo (no importa si nunca lo jugaron). Van a tener que usar lo que vimos de rozamiento.

Esta vez el personaje va a disparar un solo proyectil. Va a impactar en un objeto que esta en la mitad de la pantalla, lo que lo va a impulsar hacia el otro borde de la pantalla. Lo que tienen que lograr es que frene justo antes de llegar al borde. Van a tener que ajustar los valores de la fuerza de impacto del proyectil, la masa del objeto y sus propiedades de rozamiento para lograrlo.
