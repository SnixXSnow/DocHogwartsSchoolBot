# Desarrollo del algoritmo de los Duelos y otras notas
-------

## Comandos Previstos:
- **!duel @usuario [puntosAportados]:**  Crear un duelo.
- **!acceptD:** Aceptar un duelo.
- **!declineD:** Rechazar un duelo.
- **!cancelD [idDuelo]:** Cancela un duelo (Solo lo podran ejecutar el streamer o un mod)
- **!runD: [idDuelo]** Iniciará un duelo de manera forzada (Solo lo podrán ejecutar el streamer o un mod)
- **!infoD [idDuelo]** Mostrará la informacion de duelo. Ejemplo: @Geminis21 ha retado a @SoraTakarai a un duelo por 300 puntos
- **!rulesD** Mostrará las reglas de los duelos
- **!myduels** Mostrará la estadistica de duelos de quien lo ejecute
- **!mvD** Mostrará quien es el mejor duelista de Hogwarts
- **!wD** Mostrará quien es el peor duelista de Hogwarts
- **!mvD [gryff|raven|huff|slyth]** Mostrará quien es el mejor duelista de una casa
- **!wD [gryff|raven|huff|slyth]** Mostrará quien es el peor duelista de una casa


## Posibles estatus del duelo:
1: **Preparado**
2: **Aceptado**
3: **Rechazado**
4: **En ejecución**
5: **Terminado**


## Algoritmo
1. Se verifica que ambos jugadores esten registrados en alguna casa y que sean de casas diferentes
2. Se verifica que el retador tenga los puntos apostados
    - En caso de no tenerlos, alertar de la falta de puntos
3. Registrar en DB el nuevo duelo
4. Notificar al estudiante que ha sido retado
    - Si no acepta, notificar que no habrá duelo
5. Se ejecuta el duelo
6. Se actualiza el registro del duelo
7. Se procede a restar puntos al perdedor y otorgarlos al ganador

 

    


