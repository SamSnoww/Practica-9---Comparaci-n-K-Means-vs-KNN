# Practica-9---Comparaci-n-K-Means-vs-KNN

Este código realiza la implementación de dos algoritmos de aprendizaje automático: K-Means y K-Nearest Neighbors (KNN).
Ambos algoritmos se aplican a un conjunto de datos relacionado con la predicción de la diabetes. Aquí tienes un resumen del desarrollo:

#K-Means:
1. **Preprocesamiento de datos:**
   - Se carga un conjunto de datos desde un archivo Excel.
   - Se eliminan las filas que contienen valores nulos en las columnas 'gender' y 'smoking_history'.
   - Se codifican las variables categóricas 'gender' y 'smoking_history'.
   - Se divide el conjunto de datos en conjuntos de entrenamiento y prueba.

2. **Normalización:**
   - Se inicializan los pesos aleatorios y se agrega una columna de unos para el sesgo (bias).
   - Se calculan manualmente la media y la desviación estándar de las características de entrenamiento.
   - Se normalizan las características de entrenamiento y prueba.

3. **Implementación de K-Means:**
   - Se inicializan centroides aleatorios.
   - Se realiza la asignación de puntos a clústeres y la actualización de centroides en un bucle iterativo hasta la convergencia o el número
     máximo de iteraciones.
   - Se asignan clústeres a los datos de prueba.

4. **Evaluación del modelo:**
   - Se comparan las asignaciones de clústeres con las etiquetas reales.
   - Se calcula y muestra la precisión del modelo K-Means.

# K-Nearest Neighbors (KNN):
1. **Preprocesamiento de datos:**
   - Se carga nuevamente el conjunto de datos y se realiza la codificación de variables categóricas.

2. **Normalización:**
   - Se calcula manualmente la media y la desviación estándar de las características de entrenamiento.
   - Se normalizan las características de entrenamiento y prueba.

3. **Implementación de KNN:**
   - Se define una función para calcular la distancia euclidiana entre dos puntos.
   - Se implementa la función `knn_predict` para realizar predicciones utilizando KNN.
   - Se realizan predicciones en el conjunto de prueba y se evalúa la precisión del modelo.

4. **Evaluación del modelo:**
   - Se muestra la precisión del modelo KNN.

Este código proporciona un enfoque práctico para implementar y evaluar modelos de aprendizaje automático utilizando K-Means y KNN
en un problema de predicción de diabetes.
