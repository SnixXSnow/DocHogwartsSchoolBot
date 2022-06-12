# Twitch BOT 
## Tematica de Harry Potter 
---
##### Autor: Rebeca Ponce
##### AKA: Geminis21 o SnixXSnow
---


Este es un bot creado para manejar un sistema de puntaje entre la comunidad, similar a las casas de Hogwarts.

Las casas son las siguientes:
- Gryffindor
- Hufflepuff
- Ravenclaw
- Slytherin

Los comandos de ayuda e informacion son los siguientes:
- !helphp
- !sorteocasa

Los comandos disponibles para toda la comunidad son:
- !signup
- !score
- !mvp
- !mvp [gryff|raven|huff|slyth]
- !wp
- !wp [gryff|raven|huff|slyth]
- !mypoints
- !points @usuario
- !students
- !myhouse
- !house @username
- !top[3-10]
- !top[3-10] [gryff|raven|huff|slyth]
- !duel @usuario [1-300]
- !accept
- !decline
- !infoduel [idDuelo]
- !mycurrentduel

Los comandos para mods son los siguientes:
- !join @username [gryff|raven|huff|slyth]
- !add @username X (Donde X es el numero de puntos a otorgar al usuario)
- !take @username X (Donde X es el numero de puntos a quitar al usuario)
- !cancel [idDuelo]
- !runduel [idDuelo]
- !dip

## NOTAS IMPORTANTES

1. Está es la versión Beta del Bot.
2. Todos los comandos pueden ser modificados. Tambien pueden ser añadidos mas a petición del streamer y de la comunidad.
3. Es importante que todos los comandos que requieran como parametro el nombre del usuario, sea utilizando la etiquetacion del mismo mediante el uso de la @, esto para evitar errores, duplicidad o basura, y así asegurar que el procesamiento de la información sea mas efectiva.
4. Se planea que este bot pueda ser utilizado en mas de un canal, por lo que , en futuras versiones, podran hacerce las solicitudes correspondientes.
5. El bot hace uso de una base de datos donde están almacenados todos los datos del uso del bot (puntajes, estadisticas, eventos, etc), por lo que aunque el stream finalice, toda la actividad registrada no se perderá.
6. El bot fue creado para que funcione por eventos (uno a la vez), es decir, para aquellos que quieran que los puntos generados entre un periodo de fechas sean considerados para alguna actividad en especial del streamer, como un sorteo por ejemplo. En futuras versiones se podrá incluir la opción de crear dichos eventos. De momento, pueden pedir al desarrollador que cree el evento que desean.
7. A futuro se planea desarrollar un portal en el que los streamer puedan administrar el bot. Ademas se creará un ejecutable del bot, esto para no requerir de un servidor donde esté albergado el bot.

> OJO: El bot no es perfecto, de modo que si desean enviar sus feedback puede comunicarse con al correo snixxsnow@gmail.com 
Esto ayudará al desarrollador a mejorar y otorgar una mejor experiencia al usuario.

