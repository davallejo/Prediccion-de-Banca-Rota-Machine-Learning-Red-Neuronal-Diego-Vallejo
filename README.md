# 📉 Predicción de Bancarrota Empresarial con Machine Learning

### Red Neuronal para Evaluación de Riesgo Financiero

**Autor: Diego Vallejo**

------------------------------------------------------------------------

## 🎯 Resumen Ejecutivo

Desarrollo de un modelo predictivo basado en Redes Neuronales
Artificiales (ANN) para identificar riesgo de bancarrota empresarial
utilizando información financiera histórica.

El proyecto demuestra la aplicación práctica de:

-   Modelado predictivo con Deep Learning
-   Reducción de dimensionalidad (PCA)
-   Análisis estadístico avanzado (ANOVA, VIF)
-   Preprocesamiento robusto de datos financieros
-   Evaluación comparativa con y sin tratamiento de outliers

Resultado destacado:

> ✅ **93.21% de accuracy en datos de prueba**\
> Arquitectura eficiente con solo **43 parámetros entrenables**

------------------------------------------------------------------------

## 🧠 Problema de Negocio

La detección temprana de bancarrota permite:

-   Reducir riesgo crediticio
-   Optimizar decisiones de inversión
-   Mejorar evaluación de cartera
-   Minimizar pérdidas financieras

Este modelo puede integrarse en procesos de scoring financiero o
análisis de riesgo corporativo.

------------------------------------------------------------------------

## 📊 Datos

-   78,682 registros originales
-   21 variables financieras
-   Variable objetivo binaria: Empresa Activa / Quebrada
-   Dataset tratado con y sin eliminación de outliers (IQR)

------------------------------------------------------------------------

## ⚙️ Enfoque Técnico

### 1️⃣ Análisis Exploratorio

-   Distribución de clases
-   Correlaciones financieras
-   ANOVA para selección estadística
-   Evaluación de multicolinealidad (VIF)

### 2️⃣ Ingeniería de Características

-   Estandarización (StandardScaler)
-   Reducción de dimensionalidad con PCA
    -   Modelo 1: 8 componentes (97.5% varianza)
    -   Modelo 2: 7 componentes (85% varianza)

### 3️⃣ Modelado

Red neuronal implementada en TensorFlow/Keras:

-   Capas densas con activación ReLU
-   Regularización mediante Dropout
-   Función de pérdida: Binary Crossentropy
-   Optimizador: Adam

Arquitectura ligera y eficiente orientada a escalabilidad.

------------------------------------------------------------------------

## 📈 Resultados Clave

  Modelo     Tratamiento Outliers   Accuracy Test
  ---------- ---------------------- ----------------------------------------
  Modelo 1   No                     **93.21%**
  Modelo 2   Sí (IQR)               Comparable con menor tamaño de muestra

Hallazgos relevantes:

-   Variables como EBIT y EBITDA muestran alta capacidad predictiva.
-   El tratamiento de outliers reduce significativamente el tamaño
    muestral.
-   La reducción de dimensionalidad mejora estabilidad del modelo.

------------------------------------------------------------------------

## 🛠 Stack Tecnológico

-   Python
-   Pandas / NumPy
-   Scikit-learn
-   TensorFlow / Keras
-   Statsmodels
-   Matplotlib / Seaborn

------------------------------------------------------------------------

## 🚀 Potencial de Escalabilidad

Este proyecto puede evolucionar hacia:

-   API de scoring financiero (FastAPI)
-   Integración con sistemas bancarios
-   Validación cruzada K-Fold
-   Optimización con XGBoost o modelos ensemble
-   Pipeline automatizado en entorno productivo

------------------------------------------------------------------------

## 👨‍💻 Perfil Profesional

Proyecto desarrollado por:

**Diego Vallejo**\
Machine Learning \| Data Science \| Análisis Financiero

Especializado en:

-   Modelos predictivos aplicados a finanzas
-   Análisis cuantitativo
-   Transformación de datos en decisiones estratégicas

------------------------------------------------------------------------

📩 Disponible para oportunidades en Data Science, Risk Modeling y
Machine Learning aplicado a Finanzas.
