# TelecomX_Challenge
Repositorio de Telecom X
# Telecom Customer Churn Prediction

Este proyecto se centra en el análisis y la predicción del churn (abandono) de clientes en una empresa de telecomunicaciones utilizando datos proporcionados en formato JSON. El objetivo es identificar los factores clave que influyen en la decisión de un cliente de irse y construir un modelo predictivo para identificar a los clientes con alto riesgo de churn.

## Contenido del Repositorio

*   **`TelecomX_Data.json`**: Archivo de datos original en formato JSON.
*   **`notebook.ipynb`**: Notebook de Google Colab que contiene todo el código para la extracción, transformación, análisis exploratorio de datos (EDA) y potencialmente la implementación de modelos predictivos. (Asegúrate de que el nombre del archivo coincida con el de tu notebook).

## Proceso del Proyecto

El proyecto sigue un flujo de trabajo típico de ciencia de datos, que incluye las siguientes etapas:

1.  **Extracción de Datos:** Carga de los datos desde la URL del archivo JSON y normalización de las estructuras anidadas.
2.  **Transformación de Datos:**
    *   Manejo de tipos de datos, incluyendo la conversión a categorías, enteros y flotantes.
    *   Renombrado de columnas para una mejor legibilidad.
    *   Manejo de valores nulos (imputación en la columna 'CARGO\_TOTAL').
    *   Creación de nuevas características ('Cuentas\_Diarias').
    *   Normalización de valores en columnas categóricas ('Yes' a 'Si', etc.).
3.  **Análisis Exploratorio de Datos (EDA):**
    *   Visualización de la distribución de la variable objetivo (CHURN).
    *   Análisis del churn por género, estado civil y número de dependientes.
    *   Visualización del comportamiento de facturación diaria en relación con el churn.
    *   Análisis del churn por tipo de contrato y otros servicios.
    *   Cálculo y visualización de la tasa de churn por diversas características categóricas.
4.  **Informe Final:** Resumen de los hallazgos clave del análisis de datos, identificando los factores más relevantes asociados con el churn.
5.  **Recomendaciones:** Propuesta de estrategias basadas en el análisis para reducir la tasa de churn.
6.  **Modelado Predictivo (Opcional, si se añade):**
    *   Preprocesamiento de datos para el modelado (por ejemplo, codificación One-Hot para variables categóricas).
    *   División de datos en conjuntos de entrenamiento y prueba.
    *   Implementación y evaluación de modelos de machine learning (por ejemplo, Regresión Logística, Random Forest, Gradient Boosting).
    *   Evaluación del rendimiento del modelo utilizando métricas como Accuracy, Precision, Recall y ROC-AUC [1].

## Requisitos

Para ejecutar el notebook de Google Colab, no se requieren instalaciones locales. Sin embargo, si deseas ejecutar el código localmente, necesitarás tener Python instalado junto con las siguientes bibliotecas:

*   pandas
*   requests
*   matplotlib
*   seaborn
*   scikit-learn (si se añade modelado predictivo)

Puedes instalar estas bibliotecas usando pip:
