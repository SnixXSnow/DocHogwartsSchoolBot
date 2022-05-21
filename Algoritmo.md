# Desarrollo del algoritmo de los Duelos y otras notas
-------

## Comandos Previstos:
- **!duel @usuario [puntosAportados]:**  Crear un duelo.
- **!acceptD:** Aceptar un duelo.
- **!declineD:** Rechazar un duelo.
- **!cancelD [idDuelo]:** Cancela un duelo (Solo lo podran ejecutar el streamer o un mod)
- **!runD:**
- **!infoD [idDuelo]**
- **!rulesD**

## Posibles estatus del duelo:
1: **Preparado**
2: **Aceptado**
3: **Rechazado**
4: **En ejecución**
5: **Terminado**


## Algoritmo
1. El <i style="color:#ff0000">retador</i> inicia el duelo
2. Se verifica que el retador tenga los puntos apostados
    - Si no los tiene se alerta que no puede aportar X puntos porque no los tiene
    - Sino se crea el registro del duelo, quedando en estatus Preparado
3. Se espera confirmación del oponente.
    - Si no acepta, alertar que el duelo no fue aceptado
    - Si el oponente acepta comienza el duelo.
4. Se establece número máximo y se crea registro de turno 
    - Se verifica que no haya lanzado ya el jugador en el turno actual
        - Si ya lanzó, mandar mensaje de esperando al oponente (se puede poner el nombre del usuario)
    - Se ejecuta la funcion roll y se registra el numero obtenido
        - Si el numero obtenido es 1, se termina el turno, el duelo y se declara ganador
    - Se verifica que ambos jugadores hayan completado su turno.
        - Si aun falta alguien se notifica
        - Si no se repite el proceso hasta que haya un ganador.
    

    


