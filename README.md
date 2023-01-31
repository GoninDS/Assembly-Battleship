# **CI-0119 Proyecto integrado Battleship**

## **Repositorio para el curso CI-0119 con proyecto integrado de Battleship.**

### **Integrantes:**

Archibald Emmanuel Carrion Claeys - C01736

Fabián Vega Meza - C08369

Alberto González Avendaño - C13248

Luis David Solano Santamaría - C17634

### **Descripción de proyecto:**

Este repositorio se utilizó para desarrollar una aplicación para jugar el juego de mesa Battleship. Para la realización del proyecto se utilizó conexión entre C++ para la representación gráfica  y lenguaje ensamblador para el control de juego.

### **Reglas de juego:**

1. Los jugadores deben colocar todas sus naves en posiciones y direcciones (horizontal o vertical) válidas.

2. El juego se realiza por medio de turnos. En caso de dañar una nave el turno se repite.

3. La partida puede terminar si alguno de los dos jugadores decide abandonarla.

4. Para que un jugador termine la partida victorioso, todas las naves del oponente deben ser eliminadas.

5. La manera de eliminar una nave consiste en adivinar atacando una posición. En caso de que la posición tenga una nave, se registrará como un disparo exitoso. Para poder eliminar una nave todas sus casillas deben ser disparadas.

6. No se pueden acceder posiciones fuera del tablero ni posiciones que ya fueron atacadas.

7. Los jugadores no pueden ver las posiciones de las naves de su oponente.

### **¿Cómo jugar?**

La etapa de juego se divide en dos fases. La primera consiste en colocar naves.

Para colocar un barco se deben seguir los siguientes pasos:

1. Presionar el número de columna

2. Presionar la tecla enter para confirmar su selección

3. Presionar el número de fila

4. Presionar la tecla enter para confirmar su selección

5. Presionar la flecha para escoger la dirección de la nave

6. Presionar el botón **PLACE SHIP**

Para la etapa de ataque se deben seguir los siguientes pasos:

1. Presionar el número de columna

2. Presionar la tecla enter para confirmar su selección

3. Presionar el número de fila

4. Presionar la tecla enter para confirmar su selección

5. Presionar el botón **ATTACK**

En caso de haber escogido una fila o columna errónea, sin haber presionado enter, se puede deshacer la selección con la tecla backspace.

### **Instrucciones de compilación:**

Para poder compilar el programa debe encontrarse en una distribución de Linux, preferiblemente Ubuntu. La interfaz gráfica se realiza utilizando la herramienta **SFML.** Para esto debe tenerla instalada. En caso de no tener **SFML** puede ejecutar el siguiente comando:

    sudo apt-get install libsfml-dev

En caso de tener más consultas sobre la instalación de **SFML** en Linux puede consultar

    https://www.sfml-dev.org/tutorials/2.5/start-linux.php

Para compilar puede ejecutar el siguiente comando dentro de la carpeta src:

    make

Luego para ejecutar inserte en linea de comandos:

    ./game.out
