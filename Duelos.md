# Sistema de Duelos entre alumnos de Hogwarts

### Como funciona
Todos los alumnos que hayan generado puntos para su casa, podrán batirse a un duelo con cualquier alumno que no pertenezca a su misma casa.
El duelo consiste en un juego por turnos, cada uno deberá ejecutar el comando !roll para obtener un número entre 1 y 300. Ganará el primero que tire 1.
El rango de busqueda del numero 1 irá haciendose mas corta conforme vayan avanzando los turnos dado que el número máximo de busqueda del siguiente turno será el número menos obtenido en el turno actual. 
Por ejemplo:
> - En el primer turno, ambos jugadores obtendrán un numero entre 1 y 300. 
> - El jugador 1 obtiene 289 y el jugador 2 obtiene 212, en el turno 2, la busqueda será entre los números 1 y 212 

La busqueda es totalmente aleatoria, de modo que ambos jugadores tienen la misma posibilidad de ganar el duelo.
El alumno que resulte ganador se le otorgarán los puntos apostados a su casa y al jugador que resulte perdedor les serán descontados los puntos apostados.


### Reglas del Juego
1.  Los jugadores deberán de contar con puntos disponibles.
2.  La apuesta máxima de puntos será de 300 puntos.
3.  El alumno que es retado deberá de ser conciente de que el retador puede apostar mas puntos de los que dispone.
4.  Para continuar el duelo el retador deberá estar de acuerdo con el reto y los puntos apostados.
5.  Si uno de los 2 jugadores decide abandonar el duelo, automaticamente perderá los puntos apostados.
6.  El duelo puede ser cancelado por un mod o el streamer si así lo creen conveniente y siempre y cuando el duelo no se haya ejecutado.
7.  No se puede estar en mas de un duelo a la vez.
8.  El alumno retado tiene derecho de rechazar el duelo.
9.  Los jugadores deberán pertenecer a casas diferentes.


### Cosas a tomar en cuenta:
1. Los participantes deberán pertenecer a casas diferentes.
2. Solo se podrán apostar los puntos generados por el retador. Si el retador solo dispone de 200 puntos, no podrá apostar mas de esa cantidad.
3. El alumno retado tendrá el derecho a rechazar el duelo.

