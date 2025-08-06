# Telecom_X_Parte_2

Por supuesto, aquí tienes un ejemplo de un archivo **README.md** para tu proyecto **Telecom X - Parte 2** que puedes ajustar según tus necesidades:

```markdown
# Proyecto Telecom X – Parte 2: Predicción de Cancelación de Clientes (Churn)

---

## 📌 Propósito del Proyecto

El objetivo principal de este proyecto es desarrollar modelos predictivos que permitan anticipar la cancelación de clientes (churn) en Telecom X. Mediante el análisis de variables relevantes, buscamos identificar patrones que ayuden a entender y predecir qué clientes tienen mayor probabilidad de abandonar el servicio, con la finalidad de diseñar estrategias de retención efectivas.

---

## 📁 Estructura del Proyecto

- `TelecomX_Parte2_Análisis.ipynb`  
  Cuaderno principal donde se realiza todo el análisis, preprocesamiento, modelado y evaluación.

- `data/TelecomX_Data.csv`  
  Archivo CSV con los datos limpios y tratados para el modelado.

- `visualizations/`  
  Carpeta que contiene gráficos y visualizaciones generadas durante el análisis exploratorio y modelado.

---

## 🛠️ Proceso de Preparación de Datos

1. **Clasificación de Variables**  
   - Variables categóricas: `customer_gender`, `internet_InternetService`, `account_Contract`, `account_PaymentMethod`, entre otras.  
   - Variables numéricas: `customer_tenure`, `account_Charges_Total`, `account_Charges_Monthly`, etc.

2. **Codificación y Normalización**  
   - Se aplicó *One-Hot Encoding* para convertir variables categóricas en formato numérico compatible con los modelos.  
   - Variables numéricas fueron normalizadas para modelos sensibles a escala (Regresión Logística, KNN, SVM).  
   - Modelos basados en árboles (Random Forest) usaron datos sin normalizar, pues no son sensibles a la escala.

3. **Separación de Datos**  
   - División en conjuntos de entrenamiento (70%) y prueba (30%) con estratificación para mantener la proporción de cancelación.

---

## 📊 Ejemplos de Análisis Exploratorio de Datos (EDA) e Insights

- Visualización de la proporción de churn entre clientes.  
- Correlación destacada entre el tiempo como cliente (`customer_tenure`) y la cancelación, indicando que clientes nuevos tienen mayor riesgo.  
- Impacto significativo del tipo de contrato y método de pago en la cancelación.  
- Gráficos boxplots y scatter plots que evidencian tendencias claras en variables clave.

---

## 🚀 Instrucciones para Ejecutar el Cuaderno

### Requisitos

- Python 3.7 o superior  
- Bibliotecas Python necesarias:
```

pandas
numpy
scikit-learn
imblearn
matplotlib
seaborn

````

Puedes instalar las bibliotecas con:
```bash
pip install pandas numpy scikit-learn imblearn matplotlib seaborn
````

### Cargar los Datos Tratados

Asegúrate de colocar el archivo `TelecomX_Data.csv` dentro de la carpeta `/data/`.

En el cuaderno, carga los datos con:

```python
import pandas as pd

df = pd.read_csv('data/TelecomX_Data.csv')
```

---

## 📌 Justificaciones durante la Modelización

* Se aplicó *SMOTE* para balancear las clases debido al desbalance inicial entre clientes que cancelan y los que permanecen.
* Se seleccionaron modelos sensibles y no sensibles a la escala para comparar rendimiento y facilitar interpretabilidad.
* La selección de variables se fundamentó en análisis de correlación e importancia según cada modelo.
* Se usaron métricas múltiples (accuracy, precision, recall, F1-score) para evaluar integralmente el desempeño.

---

¡Gracias por revisar el proyecto! Para dudas o sugerencias, no dudes en contactarme.

---

```

¿Quieres que te ayude a adaptar o agregar algo más específico?
```
