# 🧠 Predicción de la Demanda de Servicios de Salud Ocupacional en Municipios Colombianos

Este proyecto propone un modelo predictivo basado en series temporales para anticipar la demanda mensual de servicios de salud ocupacional (accidentes y enfermedades laborales) en municipios de Colombia, utilizando modelos de aprendizaje profundo y estadístico.

---

## 📌 Objetivo

Desarrollar un sistema capaz de predecir, con alta precisión, la demanda de atenciones médicas laborales a nivel municipal, integrando patrones históricos, estacionalidad y características exógenas.

---

## 🛠️ Modelos Implementados

| Modelo          | Descripción |
|------------------|-------------|
| **LSTM**         | Red neuronal recurrente para capturar dependencias temporales largas. |
| **N-BEATS**      | Arquitectura especializada en forecasting univariado, basada en bloques residuales. |
| **ARIMA + XGBoost** | Modelo híbrido que combina componentes lineales (ARIMA) con relaciones no lineales (XGBoost). |

> ✅ **Modelo seleccionado**: `N-BEATS`  
> 🔎 Motivo: obtuvo el mejor desempeño en métricas de error (RMSE, MAE, SMAPE, MASE).

---

## 📊 Métricas de Desempeño

| Modelo          | RMSE     | MAE     |
|------------------|----------|---------|
| **N-BEATS**      | 27.74    | 19.36   |
| LSTM             | 60.79    | 49.95   |
| ARIMA + XGBoost  | 36.78    | 29.98   |

> Nota: RMSE y MAE reflejan el error absoluto en la escala de la variable objetivo, que representa la cantidad diaria de servicios. Estos valores deben interpretarse en relación con la magnitud promedio de la demanda en cada municipio.

---

## 📈 Resultados y Visualizaciones

- 📉 Predicción por municipios principales
- 📅 Análisis de la demanda
- 🧩 Descomposición de series (tendencia + estacionalidad)
- 📍 Identificación de municipios con mayor crecimiento de demanda.

¡Incluye notebooks y gráficos!

---

## 🔍 Dataset

Los datos fueron provistos por una ARL (Administradora de Riesgos Laborales) e incluyen:

- Registro de atenciones médicas mensuales.
- Variables dadas por municipio
- Clasificación por tipo de atención.

> ⚠️ Nota: Por privacidad, los dataset se manejan de maner privada.

---

## 🧠 Tecnologías Usadas

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Deep Learning (PyTorch / TensorFlow)
- Statsmodels, Scikit-learn, XGBoost
- N-BEATS (pytorch-forecasting)

---

