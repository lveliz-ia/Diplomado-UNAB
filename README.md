# 📈 Clasificación de Popularidad de Artículos de Noticias con Machine Learning

## 📋 Descripción del Proyecto
Este proyecto tiene como objetivo desarrollar y evaluar modelos de Machine Learning para clasificar la popularidad (medida en la cantidad de veces que se comparte un artículo: `shares`) de noticias publicadas en internet. El modelo permite a las empresas de medios predecir el impacto de su contenido antes de publicarlo, optimizando las estrategias editoriales y de monetización.

## 📊 Metodología y Ciclo de Vida del Modelo
El desarrollo del proyecto se estructuró bajo el marco de trabajo de Ciencia de Datos, cubriendo las siguientes fases:

1. **Análisis Descriptivo (EDA):** Exploración de variables, distribución de los datos y detección de correlaciones o anomalías.
2. **Ingeniería de Características:** Selección de variables relevantes y reducción de dimensionalidad para optimizar los tiempos de cómputo.
3. **Discretización del Objetivo:** Transformación de la variable continua `shares` en 3 categorías discretas:
   * 📉 **Menor:** Artículos con bajo impacto de compartidos.
   * 📊 **Medio:** Artículos con rendimiento estándar.
   * 🚀 **Superior:** Artículos altamente virales.
4. **Entrenamiento de Modelos:** Evaluación de múltiples algoritmos de clasificación (ej. Regresión Logística, Random Forest, Gradient Boosting).
5. **Optimización de Hiperparámetros:** Búsqueda sistemática (GridSearch/RandomSearch) para extraer el máximo rendimiento de los modelos.
6. **Evaluación Avanzada:** Uso de Matrices de Confusión, Curvas ROC y métricas AUC para medir la capacidad de discriminación del modelo seleccionado.

## ⚙️ Stack Tecnológico Utilizado
* **Lenguaje:** Python
* **Librerías Core:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
* **Entorno:** Jupyter Notebooks / Google Cloud Vertex AI Workbench

## 💼 Impacto de Negocio (Enfoque Project Management)
* **Gestión del Alcance:** Clasificación multiclase efectiva para la toma de decisiones editoriales en tiempo real.
* **Optimización de Recursos:** La selección de variables críticas reduce el costo de infraestructura en la nube al evitar procesar datos redundantes.

* ## 🏆 Modelo Seleccionado y Resultados
Tras evaluar y optimizar múltiples algoritmos, el modelo basado en **Random Forest** obtuvo el mejor rendimiento global (mayor AUC bajo la curva ROC). 

* **Capacidad de Discriminación:** El modelo demostró una alta robustez para diferenciar correctamente entre artículos de popularidad Menor, Medio y Superior, minimizando los falsos positivos en la categoría "Superior" (viral).
* **Variables Clave:** Los hiperparámetros optimizados mediante búsqueda sistemática permitieron estabilizar el modelo contra el sobreajuste (overfitting), asegurando una excelente capacidad de generalización con datos nuevos.

