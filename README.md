# MetodosOrdenacion_CSharp

Este proyecto se centra en la implementación y análisis comparativo de distintos algoritmos de ordenación dentro de una aplicación de consola en C#. Los algoritmos de ordenación son esenciales en la informática, pues organizan los datos de forma eficiente, facilitando su acceso y procesamiento. En nuestro caso, exploramos diversas técnicas, entre las cuales se incluyen:

Ordenamiento Burbuja: Es un algoritmo muy intuitivo pero poco eficiente para volúmenes grandes de datos, debido a su complejidad O(n²).
Ordenamiento de Sacudida: Se trata de una mejora del método burbuja, que recorre el arreglo en ambas direcciones, logrando optimizaciones menores.
Ordenamiento por Inserción: Ideal para arreglos pequeños o que ya vienen casi ordenados, aunque en el peor de los casos también tiene una complejidad O(n²).
Ordenamiento por Selección: Opera seleccionando el elemento más pequeño y colocándolo en la posición correcta, realizando menos intercambios que el burbuja.
Shell Sort: Una evolución del método de inserción que utiliza saltos (gaps) para reorganizar parcialmente el arreglo antes de una ordenación final, alcanzando frecuentemente una eficiencia de O(n log n).
Quicksort: Basado en la estrategia de "divide y vencerás", este algoritmo es altamente eficiente en promedio (O(n log n)), aunque depende en cierta medida de la elección del pivote.
Heapsort: Emplea una estructura de datos en forma de árbol (heap) para ordenar, garantizando un rendimiento constante de O(n log n) sin depender de pivotes.

Para facilitar el mantenimiento y la comparación de cada algoritmo, el código se organizó en archivos separados. El archivo Programa.cs se encarga de:

Recoger la entrada de datos desde la consola.
Mostrar un menú interactivo para elegir el algoritmo de ordenación.
Ejecutar el método seleccionado y medir el tiempo de ejecución mediante Stopwatch.
Visualizar el arreglo ordenado junto con el tiempo empleado en la operación.

Conclusiones sobre el Rendimiento Cada algoritmo muestra fortalezas y limitaciones según el tipo de datos y el tamaño del arreglo a ordenar:

Burbuja y Sacudida: Aunque sencillos de implementar, ambos métodos se vuelven lentos para conjuntos más grandes, siendo recomendables únicamente para arreglos muy pequeños o parcialmente ordenados.
Inserción y Selección:
Inserción resulta eficaz en listas pequeñas o casi ordenadas, a pesar de su complejidad teórica O(n²).
Selección también opera en O(n²) pero realiza menos intercambios, lo que puede ser ventajoso en escenarios donde mover los datos es costoso.
Shell Sort: Aprovecha la idea de la inserción, reduciendo la cantidad de movimientos necesarios gracias a una secuencia de intervalos (gaps), lo que frecuentemente mejora la eficiencia a un orden aproximado de O(n log n).
Quicksort: Destaca por su rapidez en promedio y es la opción preferente para grandes volúmenes de datos desordenados, a pesar de que su rendimiento puede variar según el pivote elegido.
Heapsort: Ofrece una eficiencia consistente mediante el uso de una estructura en forma de heap, siendo especialmente útil cuando se busca estabilidad en el desempeño.

Tabla comparativa:
