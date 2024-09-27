# Proyecto de Búsqueda IA - Pinocho

Este proyecto implementa tres algoritmos de búsqueda fundamentales: Búsqueda en Profundidad (DFS), Búsqueda en Amplitud (BFS) y Búsqueda de Costo Uniforme (UCS) para ayudar a Pinocho a encontrar a Gepetto en una matriz 5x5. La matriz está poblada con obstáculos como cigarrillos y zorros, los cuales incrementan el costo de la búsqueda.

## Descripción del Proyecto

En este proyecto, Pinocho debe navegar por una cuadrícula para encontrar a Gepetto. Las reglas de movimiento son las siguientes:

- **Costos de Movimiento:**
  - Moverse a un espacio vacío o hacia Gepetto cuesta **1**.
  - Pasar por un espacio con cigarrillos cuesta **2**.
  - Pasar por un espacio con un zorro cuesta **3**.

La configuración de la cuadrícula se carga desde un archivo de texto externo, lo que permite diferentes escenarios mientras se mantiene un tamaño fijo de 5x5. El proyecto utiliza tres estrategias de búsqueda:

- **Búsqueda en Amplitud (BFS):** Explora los nodos nivel por nivel, alternando la dirección de búsqueda entre izquierda a derecha y derecha a izquierda.
- **Búsqueda en Profundidad (DFS):** Explora lo más profundo posible en cada rama antes de retroceder.
- **Búsqueda de Costo Uniforme (UCS):** Explora el nodo con el menor costo acumulado, asegurando que se siga el camino de menor costo.

## Características

- **Configuración Dinámica de la Cuadrícula:** El diseño de la cuadrícula se carga desde un archivo externo, lo que permite diferentes escenarios sin necesidad de codificar la matriz.
- **Interfaz Gráfica de Usuario (GUI):** Se ha creado una interfaz amigable con **PyQt5** para visualizar el proceso de búsqueda y la ruta de Pinocho.
- **Propuesta de Raycasting:** Se implementa un módulo separado que utiliza **pygame** para demostrar técnicas de raycasting, ofreciendo una perspectiva única del movimiento del agente dentro de la cuadrícula.

## Requisitos

### Instalación de PyQt5

Para ejecutar la interfaz gráfica del proyecto, necesitas instalar **PyQt5**. Puedes hacerlo utilizando el siguiente comando:

  ```bash
  pip install PyQt5
  ```

Asegúrate de instalarlo en la raíz del proyecto.

### Instalación de Pygame


Para el componente de raycasting, necesitas instalar pygame:

  ```bash
  pip install pygame
  ```

## Ejecutar el Proyecto

### Algoritmo de Búsqueda Principal

Para ejecutar el algoritmo de búsqueda principal con Pinocho navegando por la cuadrícula, ejecuta el siguiente comando:

  ```bash
  python main.py
  ```

Esto cargará la interfaz gráfica y mostrará la cuadrícula con el movimiento de Pinocho según el algoritmo de búsqueda seleccionado.

### Simulación de Raycasting
Para ejecutar la propuesta de raycasting de forma independiente, navega a la carpeta raycasting y ejecuta:

  ```bash
  python mainCasting.py
  ```
Esto abrirá una ventana separada que demostrará la simulación de raycasting para el proyecto.

![Demo del Proyecto](public/gifDemoLaberintoIA.gif.gif)
