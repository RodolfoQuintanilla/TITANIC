Este archivo Jupyter Notebook, titulado `Index.ipynb`, documenta un flujo de trabajo de Ciencia de Datos aplicado al famoso conjunto de datos del **Titanic** (`titanic3.csv`).

A continuación, presento un resumen de los pasos principales realizados:

### 1. Preparación y Carga de Datos

* **Carga de librerías:** Se importaron herramientas fundamentales como `pandas`, `numpy`, `matplotlib` y `seaborn`.
* **Importación:** Se cargó el conjunto de datos desde un repositorio en GitHub mediante una URL.
* **Descripción:** El archivo incluye una guía detallada de las variables del dataset (clase de pasajero, supervivencia, nombre, sexo, edad, número de hermanos/cónyuges, tarifa, cabina, puerto de embarque, etc.).

### 2. Análisis Exploratorio de Datos (EDA)

Se realizó una exploración inicial para entender la estructura y características del dataset:

* **Dimensiones:** El dataset tiene 1309 filas y 14 columnas.
* **Inspección:** Se verificaron los tipos de datos y los valores nulos (por ejemplo, se observó que la variable `age` tiene valores faltantes).
* **Análisis Univariado y Bivariado:**
* Se analizó la **supervivencia** general (`survived`).
* Se comparó la tasa de supervivencia según el **sexo** y la **clase de pasajero** (`pclass`), encontrando diferencias significativas.
* Se exploró la relación de otras variables como el número de hermanos/cónyuges (`sibsp`) y el número de padres/hijos (`parch`) con la probabilidad de supervivencia.



### 3. Procesamiento y Modelado

* **Ingeniería de variables:** Se aplicó una técnica de *One-Hot Encoding* para transformar variables categóricas (como el sexo) en formato numérico y se concatenaron los resultados al DataFrame original.
* **Entrenamiento de modelos:** El cuaderno contiene ejemplos de implementación de modelos de clasificación utilizando `scikit-learn`, incluyendo:
* **K-Nearest Neighbors (KNN):** Se configuró y entrenó un clasificador `KNeighborsClassifier`.
* **Random Forest:** Se observa código relacionado con la configuración y uso de un modelo `RandomForestClassifier`.



En resumen, el archivo es un ejercicio práctico completo que va desde la carga de datos y el análisis estadístico descriptivo hasta la preparación de variables y la ejecución de algoritmos de Machine Learning para predecir la supervivencia de los pasajeros.
