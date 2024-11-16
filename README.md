La práctica ha sido desarrollada en Google Colab para disponer de GPU. No se incluyen ficheros pero el libro muestra los resultados ejecutados y todo el código está comentado con markdown para seguir un hilo conductor.
El primer punto consiste en un procesamiento de datos realizado de forma conjunta al modelo 1D y al modelo 2D para poder tener más adelante muestras correspondientes a ambos mundos (tabular e imagen)
El segundo punto es un modelo 1D de deep learning con un problema de regresión sobre datos tabulares. 9 features y 1 output que es el precio
El tercer punto es un modelo 2D de computer vision preentrenado(keras y tensorflow) con un problema de clasificación sobre imágenes. La clasificación se ha hecho a la variable de estudio precio dividiendo por la mediana (0 más barato, 1 más caro).
El cuarto punto es una fusión tardía de ambos modelos ya preentrenados en donde el output de dichos modelos forman el input para un problema de regresión.
El quinto punto es una fusión temprana de los mismos modelos preentrenados en donde el input fusiona las capas previas a la regresión y a la clasificación para generar un problema de regresión.
