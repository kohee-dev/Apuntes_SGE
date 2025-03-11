---
titulo: Opera en Jidoor I
subtitulo: Unidad 4
autor: Alejandro Bartolomé
header-includes: |
lang: es-ES
keywords: [DAM, SGE]
titlepage: true,
---



*Warnings*

Para la realización de esta actividad voy a tener los siguientes supuestos:
+ Eres capaz de leer y entender oraciones **largas** y eres capaz de comprender **lo que hay que hacer**.
+ Eres capaz de manejar rutas relativas y absolutas con precisión y te tomas en serio la actividad. Si no realizas las rutas correctamente, no voy a hacer mi trabajo *(tendrás un 0 en el apartado)*
+ Cada actividad va a ser corregida de forma *individual* y separada del resto de actividades.
+ Soy consciente de que estamos tratando retos que no hemos trabajado en profundidad en clase, por ello mismo no tengáis miedo en hacer preguntas.
+ Cuando hagáis comandos, recomiendo encarecidamente apuntarlos puesto que serán relevantes más adelante.
+ Si alguien realiza algún tipo de *brujeria* o *plagio* lo sabré.

*Waymarks*
+ Puesto que esta parte es el setup es un poco más corta de lo habitual, dedicadle tiempo a preparar bien el entorno y a conseguir la integración con VSCode bien.

Opera en Jidoor
==============================

![UODM](../img/opera.png.jpg)

[Recomendación musical](https://www.youtube.com/watch?v=yYzq0am3B4I)

*Bienvenidos a Jidoor para una NOCHE MÁGICA*

The Impresario os ha contratado para la preparación del retorno triunfal al mundo de la opera de Maria en la obra **María y Draco** justo cuando os avisa de que tiene un **gran problema**. Han informatizado toda la orquesta y el público está listo para su regreso, pero está cundiendo el **caos** absoluto entre todos los artistas: se han perdido instrumentos, encargados de seguridad han desaparecido, los músicos están desconcertados y la artista principal esta bajo la amenaza de que puede ser secuestrada en cualquier momento. La actuación es esta misma noche, asi que el tiempo apremia.

La situación es la siguiente, tenemos una organización llamada Teatro Jidor *(teatro_jidoor)*, una serie de empleados, artistas y músicos. Pero por desgracia María no puede actuar con seguridad asi que The Impresario ha tenido que solicitar ayuda a un extraño en última hora aunque todavía no está preparada asi que hay que arriesgarse, *¡TODO ES UN DESASTRE!*

# Usuarios

El teatro tiene los siguientes artistas:
- María
- Draco
- Ralse
- Narrador

Los músicos los podréis encontrar en el csv en la ruta `/src/Músicos.csv`

## Tarea 1: Organización interna

Artista deberá de contener los siguientes campos como mínimo:
 + Nombre
 + Apellido 
 + Dirección 
 + Fecha de Nacimiento 
 + Nacionalidad 
 + Sueldo 

 Músico deberá tener los siguientes campos como mínimo:
 + Nombre
 + Apellidos
 + Dirección
 + Edad
 + Nacionalidad
 + Sueldo
 + Instrumento
 + Grupo    

Deberás crear una aplicación Lightning que nos permita gestionar todo el sistema.

## Tarea 1: Vista de los espectadores

Con el fin de que los asistentes puedan ver el espectáculo, se ha pensado crear un objeto `espectador`.

Espectador tendrá los siguientes campos como mínimo:
 + Nombre
 + Apellido
 + Obra
 + Asiento
 + Tipo de entrada

Espectador deberá contener las entradas Locke Cole y Celes Chere, los cuales han sido invitados por Impresario. Añade algunos campos adicionales.

# Acto I: Obertura

Impresario está buscando todas las partituras y no es capaz de localizarlas por ningún lado. El tiempo apremia asi que te solicita que prepares toda la estructura de la obra a partir de una serie de hojas sueltas.

## Tarea 2: Creación de actos

La Obra esta compuesta por 4 actos:

+ Obertura (30 min)
+ Aria di Mezzo Carattere (1h)
+ Wedding Waltz ~ Duel (50 min)
+ Grand Finale (30 min)

Todos estos actos tienen una partitura escrita la cual tiene que encontrarse reflejada en el sistema (con que tenga escrito el nombre del acto es suficiente, pero utiliza el tipo de datos correcto).

La obra tiene que comenzar a las 21:00h y tiene pausas de 10 min entre actos. 

Cada uno de los actos tiene una serie de artistas asociados los cuales se ven reflejados en la siguiente tabla.

|Acto|Maria|Draco|Ralse|Narrador|
|:-|:-:|:-:|:-:|:-:|
|Obertura|x||x|x|
|Aria di Mezzo Carattere|x|x||x|
|Wedding Waltz ~ Duel|x|x|x||
|Grand Finale|x|x|x|x|

Crea un objeto que permita reflejar toda esta información.

