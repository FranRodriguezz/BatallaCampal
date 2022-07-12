# Trabajo Practico Batalla Campal
Trabajo practico grupal para Algoritmos y Programación ll - Catedra Calvo, Facultad de Ingenieria de la Universidad de Buenos Aires


### Acerca del trabajo
El trabajo práctico ha consistido en implementar un juego basado en turnos denominado Batalla
Campal, en el cual al menos dos jugadores pelean entre sí con el objetivo de conquistar el
tablero. El tablero consiste en una serie de casilleros en formato de tres dimensiones los cuales son
ocupados por unidades, a saber, soldados, aviones o barcos. Cada jugador comienza con una cantidad
de soldados determinada por los jugadores, y la intención es que a través de estas unidades, el jugador
ataque al enemigo y derribe a todos sus oponentes. El juego también posee un mazo de cartas las cuales
provocan distintos eventos.
Cada ataque realizado el enemigo inhabilita el casillero objetivo del ataque, y en caso de estar
ocupado por un soldado (sea enemigo o no), este es eliminado.
Los casilleros poseen un tipo de terreno, y dependiendo de éste las unidades podrán situarse sobre
ellos o no. Estos tipo de terrenos son:
- Tierra
- Agua
- Aire

Los jugadores se turnan entre sí, en cada turno el jugador realiza un ataque dependiendo de la
cantidad y del tipo de unidades que posea, asimismo, existe la posibilidad de lanzar misiles. Además los
jugadores pueden mover uno de sus soldados a posiciones de tipo tierra vecinas, teniendo la posibilidad
de recorrer gran parte del terreno y, en caso de que la posicion elegida sea una ocupada por un soldado
(sea enemigo o no), ambos soldados son eliminados.
Luego de realizar de mover una de sus soldados el jugador levanta una carta del mazo y se juega
inmediatamente. Los tipo de cartas implementados son:
- Misil
- Nuevo avión
- Nuevo Barco
- Somnífero
- Francotirador
- Harakiri

En todo momento los jugadores pueden observar sus propias piezas desplegadas en todo el tablero,
pero no así las del enemigo, las cuales permanecen ocultas. El mapa se puede observar en los archivos
BMP generados por el programa.
Para la implementacion de este trabajo práctico se ha utilizado memoria dinámica de forma ardua,
tanto para el tablero, como para los casilleros, los jugadores, las unidades y las cartas. También se ha
utilizado la plataforma de GitHub como entorno colaborativo para el desarrollo del mismo.

En el manual de usuario se puede ver mas acerca de la jugabilidad del mismo.

### Especificaciones:
- El trabajo se realizo en el lenguaje C++.
- La rama main se encuentra en el archivo tp2
- Compilacion: g++ -std=c++98 -ansi -pedantic -Wall -g *.cpp -o main
- Para dar imagen al tablero se uso la libreria EasyBMP, la cual nos da una imagen por cada "nivel/piso" del tablero, para cada jugador, en la carpeta donde
se encuentra el juego. Se puede apreciar la vista en el manual de usuario.
- EasyBMP: http://easybmp.sourceforge.net/download.html
