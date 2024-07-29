
# INMERSIÓN DE DATOS CON PYTHON 📊

Este proyecto se enfoca en el preprocesamiento y exploración de datos de un conjunto de datos de crédito alemán. La finalidad es construir un modelo de machine learning para evaluar la probabilidad de incumplimiento crediticio.



## Problema de Negocio 📉

La importancia de reducir el riesgo crediticio ha llevado a una institución financiera alemana a buscar soluciones innovadoras. Como científicos de datos, hemos sido convocados para construir un modelo de machine learning preciso y confiable que sea capaz de evaluar con mayor precisión la probabilidad de incumplimiento crediticio de sus clientes.
# Tareas Principales 💻

- Preprocesamiento de Datos: Realizar limpieza de datos, manejar valores faltantes, codificación de variables categóricas y normalización/escalado de datos.
- Exploración de Datos: Analizar y comprender el conjunto de datos proporcionado, identificar variables clave y realizar visualizaciones para entender las relaciones entre las variables y seleccionar las características relevantes.
- Construcción de Modelos: Experimentar con algunos algoritmos de machine learning como Regresión Logística, Árboles de Decisión, Random Forest, Naive Bayes, entre otros.
- Evaluación y Selección del Modelo: Evaluar los modelos utilizando métricas como precisión, recall, área bajo la curva ROC y F1-score. Seleccionar el modelo con el mejor rendimiento para la predicción de la solvencia crediticia.
## Desarrollo 👩🏻‍💻

El desarrollo del proyecto se llevó a cabo en varias etapas. 

**1. Configuración del Ambiente**

Primero, se configuró el ambiente de trabajo importando las bibliotecas necesarias para la manipulación y visualización de datos, así como para la construcción y evaluación de modelos de machine learning. Además, se montó Google Drive para acceder al conjunto de datos.

```import pandas as pd```

```import matplotlib.pyplot as plt```

```import seaborn as sns```

```import warnings```

```from google.colab import drive```

```from sklearn.model_selection import train_test_split```

```from sklearn.linear_model import LogisticRegression```

```from sklearn.preprocessing import StandardScaler```

```from sklearn.metrics import accuracy_score, confusion_matrix, classification_report```

```from imblearn.over_sampling import SMOTE```

```from sklearn.feature_selection import SelectKBest, f_classif```

```import joblib```

**2. Preprocesamiento de Datos**

En esta etapa, se realizó la limpieza del conjunto de datos eliminando duplicados y manejando valores faltantes. Se codificaron las variables categóricas en valores numéricos para poder ser utilizadas en los modelos de machine learning. Este paso es crucial para asegurar que los datos estén en un formato adecuado para el análisis y modelado.

**3. Exploración de Datos**

Se llevó a cabo un análisis exploratorio de los datos para comprender mejor su distribución y las relaciones entre las variables. Se crearon visualizaciones, como histogramas, para identificar patrones y posibles valores atípicos en las variables. Este análisis ayudó a seleccionar las características más relevantes para la construcción del modelo.

**4. Construcción de Modelos**

Se entrenó un modelo inicial de Regresión Logística utilizando el conjunto de datos preprocesado. Este modelo se seleccionó por su simplicidad y eficacia en problemas de clasificación binaria. Se evaluó el modelo inicial mediante la matriz de confusión y el reporte de clasificación, que proporcionaron métricas como la precisión, el recall y el F1-score.

**5. Evaluación y Selección del Modelo**
Para mejorar el rendimiento del modelo, se abordaron varios **desafíos**:

- Evaluar la Matriz de Confusión: Se compararon las matrices de confusión para diferentes enfoques para entender mejor los errores de clasificación.
- Balancear la Variable Target: Se utilizó la técnica SMOTE (Synthetic Minority Over-sampling Technique) para balancear las clases en la variable target, reduciendo el sesgo hacia la clase mayoritaria.
- Seleccionar Solo Algunas Variables y Reevaluar: Se empleó SelectKBest para seleccionar las características más importantes, lo que ayudó a mejorar la precisión del modelo eliminando características irrelevantes o redundantes.

# Visualización de las Matrices de Confusión

Finalmente, se visualizaron las matrices de confusión para cada uno de los enfoques (modelo original, modelo balanceado y modelo con selección de características) para comparar su rendimiento. Estas visualizaciones permitieron identificar claramente cómo cada modificación afectó la capacidad del modelo para clasificar correctamente las instancias.

## Conclusiones del Proyecto 📊

En esta segunda clase, logramos:

- Regresión Logística: Fue seleccionada debido a su alto AUC-ROC y balance razonable entre precisión y recall.
- Balanceo de Datos: El uso de SMOTE mejoró significativamente la capacidad del modelo para detectar las clases minoritarias.
- Selección de Características: Utilizando SelectKBest se logró mejorar la precisión del modelo, destacando la importancia de la selección adecuada de características en el proceso de modelado.


## Agradecimientos 👏🏻

Este proyecto fue realizado como parte del curso **Inmersión Datos con Python** impartido por **Alura Latam** (@aluralatam) en la Clase 02: Construcción, Evaluación y Selección del Mejor Modelo.

Quiero expresar mi gratitud a los instructores por su excelente enseñanza y apoyo:

- **Álvaro** (@ahcamachod)
- **Alejandro Gamarra** (@elprofealejo.info)
- **Christian Velasco** (@christian_pva)

Gracias por proporcionar una experiencia de aprendizaje enriquecedora y por su dedicación a la educación en ciencia de datos.

**#InmersionDatosAlura**
