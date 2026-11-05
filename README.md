# Visualizador de recorridos BFS y DFS en grafos

Aplicación gráfica Python para crear vértices/aristas y visualizar búsquedas en anchura y profundidad. Usa NetworkX para los recorridos y Matplotlib integrado en Tkinter para dibujar el grafo.

## Requisitos

Python 3 con Tkinter y dependencias de requirements.txt. Requiere una sesión gráfica.

## Ejecución

Los comandos parten de la raíz del repositorio, salvo donde se indica otra terminal.

```bash
python -m pip install -r requirements.txt
python Metodos_de_busqueda.py
```

## Recorrido de demostración

Crear varios vértices, agregar aristas y seleccionar un vértice existente como origen. Ejecutar BFS o DFS y observar cómo se resalta el recorrido. El grafo es no dirigido (nx.Graph).

## Organización

Carpetas de la entrega: [`images/`](images/).

## Documentación

- [Manual Tecnico](Manual%20Tecnico.md)
- [Manual de usuario](Manual%20de%20usuario.md)

## Alcance y límites

No usa Graphviz ni implementa un motor de autómatas. Los datos están en memoria; elegir un origen inexistente no representa un caso válido para el recorrido.

La documentación anterior a la actualización se conserva en [README-anterior.md](README-anterior.md) como referencia histórica; para iniciar el proyecto, seguir esta guía.

## Contexto y licencia

Trabajo académico o de aprendizaje conservado en el portafolio de [Enner Mendizabal](https://github.com/Ennero). Los créditos de los trabajos en grupo se conservan en sus entregas y manuales.

Consultar [LICENSE](LICENSE) para la licencia de la raíz. Las dependencias y los componentes con avisos o licencias propios conservan sus condiciones.
