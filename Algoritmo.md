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
- **!dip** Listará los duelos activos (estatus 1,2)

## Posibles estatus del duelo:
0: **Cancelado** (Cuando el streamer o un mod deciden cancelar un duelo)
1: **Preparado** (Cuando el retador hace la propuesta del reto)
2: **Aceptado** (Cuando el oponente acepta el duelo)
3: **Rechazado** (Cuando el oponente rechaza el duelo)
4: **En ejecución** (Cuando se está ejecutando el duelo)
5: **Terminado** (Cuando termina el duelo)


## Algoritmo
1. Se verifica que ambos jugadores no esten involucrados en otro duelo.
    - Si al menos uno lo está se cancelará el duelo.
2. Se verifica que ambos jugadores esten registrados en alguna casa y que sean de casas diferentes.
3. Se verifica que el retador tenga los puntos apostados.
    - En caso de no tenerlos, alertar de la falta de puntos.
4. Registrar en DB el nuevo duelo.
5. Notificar al estudiante que ha sido retado.
    - Si no acepta, notificar que no habrá duelo.
6. Se ejecuta el duelo.
7. Se actualiza el registro del duelo.
8. Se procede a restar puntos al perdedor y otorgarlos al ganador.

 

    


