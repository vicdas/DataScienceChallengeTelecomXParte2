# 📊 DataScienceChallengeTelecomX

## 🚀 Telecom X - Análisis de Evasión de Clientes (Parte 2)

Este proyecto tiene como objetivo desarrollar modelos predictivos capaces de prever qué clientes tienen mayor probabilidad de cancelar sus servicios en **Telecom X**, y así ayudar a la empresa a anticiparse y diseñar estrategias de retención efectivas.

---

## 🎯 Misión

Diseñar un **pipeline robusto de modelado predictivo**, desde la preparación de datos hasta la interpretación de resultados, con foco en la cancelación de servicios (*Churn*).

---

## 🧠 Objetivos del Desafío

- ✅ Preparar los datos para el modelado (tratamiento de valores nulos, codificación y normalización).
- ✅ Realizar un análisis de correlación y seleccionar variables clave.
- ✅ Entrenar dos modelos de clasificación: **Logistic Regression** y **Random Forest**.
- ✅ Evaluar los modelos utilizando métricas como *accuracy*, *precision*, *recall*, *f1-score* y matriz de confusión.
- ✅ Interpretar los resultados, identificando las variables más influyentes en la cancelación.
- ✅ Elaborar una **conclusión estratégica** con recomendaciones accionables.

---

## 🧪 Tecnologías y librerías utilizadas

- `Python` + `Pandas` + `NumPy`  
- `scikit-learn` (modelado, métricas, SMOTE, pipelines)
- `Seaborn` y `Matplotlib` (visualización)
- `Google Colab` y `Google Drive` (entorno de ejecución)

---

## 🗂️ Estructura del Proyecto

### 📌 1. Extracción
✅ Los datos fueron importados eficientemente desde una API o Drive.

### 🔧 2. Transformación
✅ Se aplicó un pipeline de **ETL** con:
- Conversión de variables categóricas (`OneHotEncoder`)
- Escalamiento (`StandardScaler`)
- Balanceo de clases (`SMOTE`)

### 📊 3. Análisis Exploratorio (EDA)
✅ Visualizaciones clave para comprender:
- Distribución del churn
- Correlación entre variables
- Impacto de contratos, servicios, métodos de pago y antigüedad

### 🤖 4. Modelado y Evaluación
Se entrenaron dos modelos:

| Modelo               | Accuracy | Precision | Recall | F1-score |
|----------------------|----------|-----------|--------|----------|
| Logistic Regression  | **0.7949**  | **0.6393**   | **0.5214** | **0.5744** |
| Random Forest        | 0.7850   | 0.6220    | 0.4840 | 0.5444   |

✅ **Logistic Regression fue el modelo más efectivo**, con mejor balance entre precisión y recall.

### 📌 5. Interpretación y Variables Clave

Principales variables que influyen en la cancelación:

| Variable                         | Influencia | Interpretación |
|----------------------------------|------------|----------------|
| `account.Contract_Month-to-month` | Positiva   | Clientes con contrato mensual son más propensos a cancelar. |
| `account.Contract_Two year`       | Negativa   | Contratos largos reducen el churn. |
| `internet.TechSupport_Yes`       | Negativa   | Soporte técnico retiene clientes. |
| `account.PaymentMethod_Electronic check` | Positiva | Asociado a mayor cancelación. |
| `customer.tenure`                | Negativa   | Mayor antigüedad reduce la cancelación. |

---

## 🧩 Conclusión Estratégica

Los hallazgos más relevantes indican que **la duración del contrato**, **la forma de pago**, y **los servicios adicionales contratados** (como soporte técnico o seguridad en línea) son factores determinantes en la retención del cliente.

### 🎯 Recomendaciones:

- Incentivar la migración a **contratos de largo plazo** mediante promociones.
- Ofrecer **servicios de valor agregado** como soporte técnico o seguridad como parte de paquetes básicos.
- Fomentar el uso de métodos de pago **automáticos o estables**.
- Realizar campañas de fidelización para usuarios con mayor antigüedad.
- Crear planes adaptados para perfiles vulnerables (por ejemplo, **adultos mayores**).

---

## ▶️ Ejecución del Notebook

Para ejecutar el análisis y visualizar resultados en Google Colab:

1. **Acceder a Google Colab**: [https://colab.research.google.com/](https://colab.research.google.com/)
2. **Subir el notebook**: Menú `Archivo > Subir notebook` y seleccione `TelecomX_LATAM.ipynb`.
3. **Conectar a Google Drive**: Autorice el acceso cuando sea solicitado para leer los datos.
4. **Ejecutar las celdas**: Use el botón ▶️ o presione `Shift + Enter` para avanzar paso a paso.
5. **Visualizar los resultados**: Observe gráficos, métricas y conclusiones generadas al final del análisis.

---

## 📈 Informe Final y Visualizaciones

El informe final incluye:

- Métricas detalladas de evaluación de modelos.
- Gráficos de importancia de variables.
- Matrices de confusión.
- Recomendaciones estratégicas basadas en datos.

> ✉️ Para más información o dudas, 📬 Contacto: Victor David Arriola - vicdarrsa@gmail.com | [LinkedIn]([https://www.linkedin.com/in/david-arriola/](https://www.linkedin.com/in/vidaarsa/))
.
