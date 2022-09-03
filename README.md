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

# Técnicas de procesamiento:

Definición del modelo a implementarse:
1.	Cambio de tamaño: Se ajusta a una altura de 100 pixeles y longitud de 100 pixeles a todas las imágenes
2.	Se define el número de épocas en 20.
3.	Se define el número de imágenes a procesarse en cada paso en 32.
4.	Se define el número de pasos en cada época como 1000.
5.	Se define el número de pasos de validación como 200, a fin de comprobar como va avanzando el modelo.
6.	Se definen dos filtros de convolución el primero con una profundidad de 32 y el segundo con una profundidad de 64.
7.	Se establecen los tamaños de cada filtro, el primero (3,3) y el segundo (2,2) en altura y longitud.
8.	Se define el tamaño del pool (3,3) para el max poolling.
9.	Se define el número de clases de 8 aunque en la clase 1 no se tienen datos.
10.	Finalmente se establece el learning rate en 0.0005 para que la red neuronal se vaya ajustando a fin de mejorar el modelo.

Preprocesamiento de imágenes
1.	Re escalado de imágenes cambio el valor de los pixeles de 1 a 255 a valores entre 0 y 1 a fin de hacer más eficiente el proceso.
2.	Se genera función shear range para que el algoritmo aprenda también con imágenes cortadas.
3.	 Se genera función zoom range para que el algoritmo aprenda también con imágenes acercadas o alejadas.
4.	Se genera función horizontal flip para que el algoritmo aprenda también con imágenes invertidas.



Finalmente se adjunta la matriz de confusión realizada con 100 muestras de las cuales 50 pertenecían a la clase 5 y 50 a otras clases, todas las muestras tomadas de la carpeta de evaluación.

MATRIZ DE CONFUSIÓN

![image](https://user-images.githubusercontent.com/101531467/188279259-b50d17f7-9ffd-409e-bd3d-92268968b388.png)


Esta matriz cambiaba dependiendo de la clase que se evaluara, esto debido al número de muestras disponibles en el entrenamiento del modelo. En el cuadro mostrado anteriormente se evaluó la clase 5, ya que era la que tenpia un mayor número de muestras disponibles en la generación del modelo y la que mejores resultados demostró en las pruebas realizadas.


![image](https://user-images.githubusercontent.com/101531467/188279786-fa3bb8f9-7c77-4393-abbc-50b2f20226a7.png)




