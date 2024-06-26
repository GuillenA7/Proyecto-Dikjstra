# Proyecto Final - Visualizador de Dijkstra - Estructura de Datos y Algoritmia

Este proyecto HTML muestra una red de nodos interactiva y utiliza el algoritmo de Dijkstra para encontrar el camino más corto entre nodos específicos.

## Archivos y Bibliotecas

### HTML (index.html)
Define la estructura de la página web y carga la biblioteca vis.js para visualizar la red.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Visualizador de Dijkstra</title>
    <style>
        /* Estilos para el contenedor de la red y controles */
        #mynetwork {
            width: 100%;
            height: 600px;
            border: 1px solid lightgray;
        }
        .controls {
            margin-top: 20px;
        }
    </style>
    <!-- Importación de la biblioteca vis.js para la visualización de la red -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/vis/4.21.0/vis.min.js"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/vis/4.21.0/vis.min.css" rel="stylesheet" type="text/css">
</head>
<body>
    <!-- Contenedor para la red -->
    <div id="mynetwork"></div>
    <div class="controls">
        <!-- Botón para encontrar el camino más corto -->
        <button onclick="findShortestPath()">Encuentra el camino más corto</button>
    </div>

    <script src="script.js"></script>
</body>
</html>
```
### JavaScript (script.js)
Contiene la lógica para crear la red de nodos y aristas, implementa el algoritmo de Dijkstra, y maneja la interacción del usuario para encontrar y resaltar el camino más corto.

Este proyecto combina visualización de datos con algoritmos de grafos, proporcionando una manera efectiva de entender y demostrar el algoritmo de Dijkstra en acción.

## Componentes Principales
### Red de Nodos y Aristas
- Define nodos (A, B, C, ...) y aristas con etiquetas de peso y longitudes.
- Utiliza vis.js para la visualización en el contenedor <div> con id mynetwork.
### Algoritmo de Dijkstra
- Implementado en JavaScript para calcular el camino más corto entre dos nodos.
- Usa una cola de prioridad para manejar las distancias y reconstruir el camino una vez encontrado.
### Interacción del Usuario
- Un botón permite al usuario encontrar el camino más corto entre dos nodos seleccionados (por defecto, de 'C' a 'A').
- Después de ejecutar Dijkstra, resalta visualmente el camino más corto en la red utilizando colores.
## Personalización y Uso
- **Personalización de la Red:** Puedes modificar nodos y aristas en el código para crear diferentes topologías y pesos.
- **Uso en Educación o Demostraciones:** Útil para enseñar el algoritmo de Dijkstra y visualizar cómo funciona para rutas más cortas en una red.
## Ejemplo de Uso
- Abre `index.html` en un navegador web.
- Haz clic en el botón "Encuentra el camino más corto".
- Observa cómo se resalta el camino más corto entre los nodos seleccionados.

Este proyecto proporciona una herramienta útil para explorar visualmente grafos y entender el algoritmo de Dijkstra mediante una interfaz interactiva.
