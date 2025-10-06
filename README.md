# Diagramas de arquitectura

## BIZO
BIZO cuyas siglas significan, Bideojuego Increible Zuper Original, es un videojuego Roguelite de oleadas, por oleadas nos referimos a rondas, por cada ronda una cantidad predeterminada de enemigos aparecera en el mapa y atacara al jugador, para ganar la oleada o ronda el jugador debera eliminar a todos los enemigos, al terminarse la oleada el jugador pasara a una tienda donde podra comprar mejoras para que las siguientes rondas no sean tan dificiles

# Explicacion de los diagramas
## Diagrama del sistema del juego (Secuencia: Untitled_Diagram.drawio)

Este diagrama muestra como se conectan las distintas partes del juego.
El jugador interactua con el sistema de juego, que se encarga de todo lo que pasa durante una partida (movimiento, enemigos, oleadas, etc.).
Mientras se juega, el gestor de progresion va registrando los avances y resultados, y se los pasa al sistema de recompensas, que entrega monedas, puntos o mejoras segun como fue la partida.
Despues, el jugador puede usar esas recompensas en la tienda o sistema de mejoras para subir estadisticas o desbloquear cosas nuevas.
En pocas palabras, muestra el ciclo general del juego: jugar > progresar > recibir recompensas > mejorar > volver a jugar.

## Diagrama de arquitectura del proyecto (Arquitectura: DIagrama_de_Arquitectura.drawio)

Este diagrama explica como esta armado el proyecto por dentro.
Se pueden ver las distintas partes que hacen que todo funcione:

Por un lado, lo visual y el sonido (lo que el jugador ve y escucha).

En el medio, todo lo que tiene que ver con la jugabilidad: el control del jugador, los enemigos y el sistema de oleadas.

Tambien hay un sistema que guarda las mejoras y el progreso del jugador entre partidas.

Y por ultimo, algunas partes que manejan datos generales del juego, como la musica o variables globales.

En resumen, muestra como se organiza todo para que el juego funcione de manera ordenada y sea facil de entender o ampliar mas adelante.
