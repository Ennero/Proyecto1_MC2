# Manual Tecnico Proyecto MC2

El presente es el manual para el proyecto de **Matemática para la Computación 2**, orientado al tema de algoritmos de búsqueda a lo ancho y a lo largo. Estos algoritmos de búsqueda son fundamentales en el ámbito de la ciencia de la computación y la inteligencia artificial, pues se utilizan en una amplia variedad de aplicaciones, desde la resolución de problemas en grafos hasta la optimización de rutas en sistemas de navegación. El grupo tuvo la libertad de codificar en el lenguaje más cómodo para ellos, y en este caso, el proyecto se desarrolló utilizando *Python*. Para llevar a cabo el código, se utilizaron diferentes bibliotecas, y toda la sintaxis está organizada para el desarrollo óptimo de la aplicación.

Este código es un programa en *Python* el cual utiliza la biblioteca *networkx* para crear y visualizar gráficos y la biblioteca *matplotlib* para dibujar estos gráficos en una interfaz gráfica de usuario (GUI) utilizando *tkinter*.

En resumen, este programa permite al usuario construir un grafo interactivo utilizando una interfaz gráfica de usuario, agregar vértices y aristas y realizar búsquedas en anchura y en profundidad en el grafo creado.

### Objetivos

#### Objetivo General
1. Exponer los metodos que se usan para determinar cual es el mejor camino por medio de los algoritmos de busqueda.

#### Objetivos Especificos
1. Explicar la manera de implementar los algoritmos de búsqueda a lo largo y a lo ancho.
2. Aplicar los metodos a una sintaxis de Phyton por medio de una interfaz grafica interactiva, por la cual observaremos como es que funciona.
3. Comprender como funcionan los dos algoritmos en situaciones iguales o más extensas.


### Logica del Sistema


1. ![Importación de bibliotecas](/images/t1.png)
   *Importación de bibliotecas*:
   python
   from matplotlib.figure import Figure
   import networkx as nx
   import tkinter as tk
   from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
   
   - matplotlib.figure: Importa la clase Figure de la biblioteca matplotlib, que se utiliza para crear figuras de gráficos.
   - networkx as nx: Importa la biblioteca networkx con el alias nx, que se utiliza para trabajar con grafos.
   - tkinter as tk: Importa la biblioteca tkinter con el alias tk, que se utiliza para crear la interfaz gráfica de usuario.
   - matplotlib.backends.backend_tkagg: Importa la clase FigureCanvasTkAgg de matplotlib.backends, que se utiliza para mostrar figuras de matplotlib en una ventana de tkinter.

2. ![Inicialización del grafo y la interfaz gráfica](/images/t2.png)
   *Inicialización del grafo y la interfaz gráfica*:

   python
   G = nx.Graph()
   root = tk.Tk()
   root.title("Algoritmo de búsqueda")
   
   - Se crea un objeto nx.Graph() que representa un grafo vacío.
   - Se crea una ventana de tkinter con el título "Algoritmo de búsqueda".

3. ![Funciones para agregar vértices y aristas al grafo](/images/t21.png)
   *Funciones para agregar vértices y aristas al grafo*:
   python
   def add_vertex():
       # Código para agregar un vértice al grafo

   def add_edge():
       # Código para agregar una arista al grafo
   
   - add_vertex(): Agrega un vértice al grafo utilizando el texto ingresado en vertex_entry.
   - add_edge(): Agrega una arista al grafo utilizando los textos ingresados en edge_entry_1 y edge_entry_2.

4. ![Función para dibujar el grafo](/images/t22.png)
   *Función para dibujar el grafo*:
   python
   def draw_graph(bfs_edges=None, dfs_edges=None):
       # Código para dibujar el grafo con opciones de resaltar aristas para BFS y DFS
   
   - draw_graph(): Dibuja el grafo en el lienzo (canvas). Opcionalmente, puede resaltar las aristas de un recorrido en anchura (BFS) o en profundidad (DFS).

5. ![Funciones para realizar la búsqueda en anchura y en profundidad](/images/t3.png) ![Funciones para realizar la búsqueda en anchura y en profundidad](/images/t4.png)
   *Funciones para realizar la búsqueda en anchura y en profundidad*:
   python
   def show_bfs():
       # Código para realizar una búsqueda en anchura y dibujar el resultado

   def show_dfs():
       # Código para realizar una búsqueda en profundidad y dibujar el resultado
   
   - show_bfs(): Realiza una búsqueda en anchura desde el vértice ingresado y resalta las aristas encontradas.
   - show_dfs(): Realiza una búsqueda en profundidad desde el vértice ingresado y resalta las aristas encontradas.

6. *Creación de la interfaz gráfica*:

   1.  ![Creación de las entradas de los vértices](/images/t5.png)
   *Creación de las entradas de los vértices*
   - Se crean etiquetas (Label) para indicar qué realizar, entradas (Entry) para ingresar vértices y aristas, botones (Button) para agregar vértices.
   2. ![Creación del lienzo para el grafo](/images/t9.png)
   *Creación del lienzo para el grafo*
   - Se crea una figura (Figure) de *matplotlib* y se agrega un lienzo (canvas) de *tkinter* para dibujar el grafo.
   3. ![Creación de los botones de búsqueda](/images/t6.png)
   *Creación de los botones de búsqueda*
   - Se cran los botones para realizar las búsquedas en anchura y en profundidad gracias a que llaman las funciones que realizan estas acciones.
   4. ![Ejecución del bucle principal de la interfaz gráfica](/images/t7.png)
   *Ejecución del bucle principal de la interfaz gráfica*:
   python
   root.mainloop()
   
   - Inicia el bucle principal de la interfaz gráfica de tkinter, donde se espera que el usuario interactúe con la aplicación.

### [Video Explicativo ](https://youtu.be/nkzDdbQEhLQ?si=Q_IHvOQjbO2OCVUC)



