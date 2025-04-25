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

| Modelo          | RMSE     | MAE      | SMAPE    | MASE    |
|------------------|----------|----------|----------|----------|
| **N-BEATS**      | 36.23    | 25.36    | 57.83%   | 0.52     |
| LSTM             | 86.03    | 71.29    | 114.01%  | 1.29     |
| ARIMA + XGBoost  | 47.54    | 39.01    | 74.16%   | 0.77     |

---

## 📈 Resultados y Visualizaciones

- 📉 Predicción vs. Valores reales por municipio
- 📅 Análisis mensual y anual de la demanda
- 🧩 Descomposición de series (tendencia + estacionalidad)
- 📍 Identificación de municipios con mayor crecimiento de demanda

¡Incluye notebooks interactivos y gráficos generados automáticamente!

---

## 🔍 Dataset

Los datos fueron provistos por una ARL (Administradora de Riesgos Laborales) e incluyen:

- Registro de atenciones médicas mensuales
- Variables demográficas y económicas por municipio
- Clasificación por tipo de atención (accidentes vs. enfermedades)

> ⚠️ Nota: Por privacidad, los datos sensibles han sido anonimizados.

---

## 🧠 Tecnologías Usadas

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Deep Learning (PyTorch / TensorFlow)
- Statsmodels, Scikit-learn, XGBoost
- N-BEATS (pytorch-forecasting)

---

