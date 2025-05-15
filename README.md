# Proyecto Final - Data Science Bootcamp
## Detección de Fraude en Transacciones Financieras

Este proyecto analiza un conjunto de datos de transacciones financieras para construir un modelo predictivo que permita identificar posibles fraudes. A través de técnicas de análisis exploratorio, balanceo de clases, modelado supervisado y optimización, se busca entender qué factores contribuyen a predecir conductas fraudulentas y qué tan efectivo es cada algoritmo en esa tarea.

---

## Objetivo

- Detectar transacciones fraudulentas utilizando modelos de clasificación.
- Evaluar el impacto de distintas variables en la ocurrencia de fraude.
- Comparar el rendimiento de modelos antes y después del balanceo de clases (SMOTE).
- Identificar el mejor modelo según métricas clave como ROC-AUC, Recall y F1-score.

---

## Tecnologías y Librerías

- Python 3.12
- pandas, numpy
- scikit-learn
- xgboost
- imbalanced-learn
- matplotlib, seaborn

---

## Metodología

1. **Carga y limpieza de datos**
2. **Análisis exploratorio (EDA)**
3. **Ingeniería de atributos (One-Hot Encoding, imputaciones)**
4. **Balanceo de clases con SMOTE**
5. **Entrenamiento de modelos:**
   - Decision Tree
   - Random Forest
   - Gradient Boosting
   - XGBoost
6. **Optimización con RandomizedSearchCV**
7. **Evaluación con métricas:**
   - Precision, Recall, F1-Score
   - ROC-AUC
8. **Interpretación con `feature_importances_`**

---

## Resultados

- **Modelo seleccionado:** XGBoost
- **ROC-AUC final:** ~0.99
- **Variables más influyentes:**
  - Número de transacciones en las últimas 24h
  - Método de pago
  - Tipo de dispositivo
- **Insights clave:**
  - El monto de la transacción no es un predictor significativo.
  - El tipo de dispositivo influye moderadamente.
  - La antigüedad de la cuenta no es un factor clave.

---
