# Gold-Prediction-Model

# Gold Recovery Optimization ML

## Resumen del Proyecto

Este proyecto se enfoca en optimizar el proceso de **recuperación de oro** para la empresa **Zyfra** mediante la construcción de un modelo de Machine Learning capaz de predecir la cantidad de oro extraído del mineral. El objetivo principal es identificar y eliminar parámetros no rentables en la producción, lo que conducirá a una mayor eficiencia y rentabilidad.

## 🎯 Objetivos del Proyecto

* Construir un **modelo de Machine Learning** para predecir la cantidad de oro extraído.
* Identificar y limpiar **parámetros no rentables** en el proceso de extracción y purificación.

## 🛠️ Tecnologías y Librerías Utilizadas

* **Python**: Lenguaje de programación principal.
* **Pandas**: Manipulación y análisis de datos.
* **NumPy**: Computación numérica.
* **Scikit-learn**: Construcción y evaluación de modelos de Machine Learning (ej. `RandomForestRegressor`).
* **Matplotlib / Seaborn**: Visualización de datos.

## 📈 Metodología y Desarrollo

### 1. **Procesamiento de Datos**

* Se realizó una limpieza exhaustiva de los datasets de entrenamiento (`train`), prueba (`test`) y completo (`full`).
* Se manejaron **valores ausentes** mediante eliminación para evitar la introducción de información falsa.
* Se verificó la **correcta tipificación** de los datos de fecha y se realizaron las conversiones necesarias.
* Se identificó que el dataset de prueba carecía de ciertas características de cálculo `rougher` y otras del producto final, lo cual no impactó negativamente el entrenamiento del modelo.

### 2. **Preprocesamiento de Datos**

* Para agilizar y precisar el proceso de entrenamiento, se trabajó con una **muestra representativa** del dataset de entrenamiento.

### 3. **Cálculo de Recuperación**

* Se llevó a cabo una **validación del cálculo de recuperación** para asegurar la precisión de los datos. No se encontraron diferencias significativas, confirmando la fiabilidad de la información en el dataset de entrenamiento.

### 4. **Análisis de Distribución de Características**

* Se analizaron las **distribuciones de los metales** en las diferentes etapas de purificación y en el producto final. Los resultados mostraron coherencia con los procesos de producción.

### 5. **Construcción y Evaluación del Modelo**

* Se implementó una **función personalizada para calcular el sMAPE** (Symmetric Mean Absolute Percentage Error), métrica clave para evaluar la precisión del modelo en la predicción de la recuperación de oro.
* Se experimentó con diferentes modelos, seleccionando finalmente **`RandomForestRegressor`** como el más adecuado.
* El modelo final obtuvo una **puntuación de sMAPE de 2.581**, demostrando una alta capacidad predictiva para la recuperación de oro.

## 📊 Conclusiones Clave

* El proceso de **limpieza y preprocesamiento de datos** fue fundamental para asegurar la calidad de la información utilizada en el modelo.
* La validación de los cálculos de recuperación confirmó la **integridad de los datos** proporcionados.
* El análisis de la distribución de las características aportó **insights valiosos** sobre el comportamiento de los metales en el proceso de purificación.
* El modelo **`RandomForestRegressor`** demostró ser altamente efectivo, logrando un **sMAPE de 2.581**, lo que indica una **predicción robusta y confiable** de la cantidad de oro extraído.
* Este modelo puede ser una herramienta clave para **Zyfra** en la **optimización de su producción de oro** y la identificación de parámetros no rentables, mejorando así la eficiencia y rentabilidad operativa.
