# 📊 Proyecto de Predicción de Churn

Este proyecto utiliza Machine Learning (estándar y Spark) para predecir la probabilidad de que un cliente de telecomunicaciones abandone el servicio (**Churn**). Se comparan diferentes modelos y se simulan estrategias de retención para evaluar su impacto en el negocio.

---

## 📌 **Estructura del Proyecto**

```
/ChurnRetention-SP
│── /data
│   ├── raw_customerChurn.csv
│   ├── cleaned_customerChurn.csv  # Listo para usarse en Power BI
│   ├── preprocessed_customerChurn.csv  # Listo para entrenar los modelos 
│── /models
│   ├── best_model.joblib  # Mejor modelo estándar
│   ├── best_spark_model.?? # Mejor modelo de Spark MLlib
│── /notebooks
│   ├── Exploratory_Analysis.ipynb  # Limpieza de datos & visualización
│   ├── Preprocessing.ipynb  # Preparación de los datos para entrenar los modelos
│   ├── Model_Training.ipynb  # Entrenamiento de modelos estándar y tuning
│   ├── Spark_Model_Training.ipynb  # Entrenamiento de modelos de la librería Spark MLlib
│   ├── Simulation.ipynb # Simulación de la reducción de Churn  
│── README.md
```

---

## 📊 **1. Análisis Exploratorio**
El archivo ['Exploratory_Analysis.ipynb'](notebooks/Exploratory_Analysis.ipynb) contiene:  
✅ Carga y limpieza de datos  
✅ Visualización de tendencias de Churn con **Matplotlib & Seaborn**  
✅ Análisis de correlaciones y factores clave   

📌 El dataset que resulta tras el EDA se guarda en: /data/cleaned_customerChurn.csv. Este dataset se usa para crear los dashboards en PowerBI ('Enlace')

---

## ⚙️ **2. Preprocesamiento de Datos**
El archivo ['Preprocessing.ipynb'](notebooks/Preprocessing.ipynb) incluye los pasos para preparar los datos antes del modelado:  
✅ Transformación de valores categóricos con **One-Hot Encoding**  
✅ **Normalización y estandarización** de variables  
✅ **Tratamiento de valores nulos y outliers**

📌 El dataset preprocesado se guarda en: /data/preprocessed_customerChurn.csv, listo para su uso en modelos.  

---

## 🤖 **3. Modelado y Evaluación**
El archivo ['Model_Training.ipynb'](notebooks/Model_Training.ipynb) desarrolla:  
✅ **Balanceo de datos** con **SMOTE y RandomUnderSampler**  
✅ Modelos como **Regresión Logística, Decisión Tree, Random Forest, XGBoost y LightGBM**  
✅ Evaluación de los modelos con **SHAP Values, Matriz de confusión, Curva ROC y Curva Precision-Recall**  
✅ **Optimización de hiperparámetros** con **Grid Search**

📌 **El mejor modelo se guarda en** `/models/best_model.joblib`

---

## 🎯 **4. Simulación de Reducción de Churn**
 
El archivo ['Simulation.ipynb']
(notebooks/Model_Training.ipynb) calcula el impacto de estrategias de retención:  
✅ Simulación de estrategias de retención  
✅ **Cálculo del ahorro financiero y ROI**

---

## 🤖 **5. Modelado y Evaluación en Spark**
El archivo ['Spark_Model_Training.ipynb'](notebooks/Spark_Model_Training.ipynb) desarrolla modelos utilizando Spark MLlib, una librería optimizada para procesamiento en Big Data.  
✅ Transformación de datos con **VectorAssembler** para trabajar con Spark.  
✅ Entrenamiento de modelos como **Decision Tree, Random Forest y Gradient-Boosted Trees (GBTClassifier)**.    
✅ Comparación de métricas con el best_model.joblib 
✅ **Optimización con CrossValidator y ParamGridBuilder** para mejorar los hiperparámetros.  

📌 **El mejor modelo de Spark se guarda en** /models/best_spark_model.??.

---

## 📥 **6. Instalación y Uso**
### **Descargar el Repositorio**
```
bash
git clone https://github.com/angelfergar/ChurnRetention-SP.git
cd ChurnRetention-SP
```

---

## 📈 **7. Resultados Clave**
* RELLENAR CON Resultados

📊 _RELLENAR CON Gráficos y visualizaciones detalladas en los notebooks y PowerBI._

---

## 🤝 **8. Contribución**
¡Sugerencias y mejoras son bienvenidas! 🚀

📌 **Desarrollado por**: Ángel Fernández  
✉️ Contacto: anfernagar@gmail.com
