# ProyectoFinal
Clasificador de imágenes con TensorFlow y Keras, utilizando Redes Neuronales Convolucionales

Nombre: Francisco Salazar H.

Saludos

En este repositorio se encuentra el proyecto final realizada para la clase de tratamiento de datos.

La estructura de archivos es la siguiente:

entrenar.py: En este archivo se implementa la red neuronal convolucional que ve va a entrenar para generar el modelo de predicción que se utilizará para este proyecto.

predecir.py: En este archivo se carga el modelo generado y se crealizarán las predicciones de las imágenes que se cargue.

Adicional se debe cargar una carpeta llamada Data dentro de la que se deben colocar las imágenes tanto de Entrenamiento como de Validación en sus respectivas carpetas de clasificiación.

Notebook.ipynb: Este es el notebook jupyter del proyecto, ya que para el proyecto se utilizó un entorno virtual con python 2.6, en jupyter no se pudo implementar la misma versión, por lo que los comandos de tensorflow y keras no corrían, además que el tiempo que tardó la red neuronal en entrenarse duró aproximadamente unos 4 horas. Así que para ilustrar el proceso que se siguió, se generó un código similar como ejemplo de lo realizado en el programa principal pero unicamante tomando dos clases como ejemplo y disminuyendo los parámetros con los que se alimentó a la red neuronal.

En el siguiente enlace se encuentra el modelo de predicción generado, con una prosición aproximadamente del 93% como se muestra en la imagen Precisión del Clasificador.jpg

https://drive.google.com/drive/folders/1GqL34FGl0xz34Wnx-NgrF8cts13Etchj?usp=sharing

![Presición del clasificador](https://user-images.githubusercontent.com/101531467/188278092-c3bb7724-f868-4f45-974d-38870f2d2813.jpg)


Finalmente como trabajo adicional se suven dos ejemplos adicionales de clasificadores de imagenes con redes neuronales convolucionales, con estos ejemplos se profundizó en la compresión de la materia. Estos archivos son:

Clasificación2.ipynb


Clasificación3.ipynb

Finalmente se adjunta la matriz de confusión realizada con 100 muestras de las cuales 50 pertenecían a la clase 5 y 50 a otras clases, todas las muestras tomadas de la carpeta de evaluación.

MATRIZ DE CONFUSIÓN

![image](https://user-images.githubusercontent.com/101531467/188279259-b50d17f7-9ffd-409e-bd3d-92268968b388.png)


Esta matriz cambiaba dependiendo de la clase que se evaluara, esto debido al número de muestras disponibles en el entrenamiento del modelo. En el cuadro mostrado anteriormente se evaluó la clase 5, ya que era la que tenpia un mayor número de muestras disponibles en la generación del modelo y la que mejores resultados demostró en las pruebas realizadas.



