# challenge-data-science-telecom
Análisis de evasión de clientes para Telecom X
# 📡 Telecom X - Churn Analysis Project

## 📋 Descripción del Proyecto
Este proyecto analiza los datos de clientes de una empresa de telecomunicaciones ("Telecom X") para identificar patrones de evasión (Churn). El objetivo es entender qué factores influyen en que un cliente cancele su servicio y proponer insights basados en datos.

## 🛠️ Tecnologías Utilizadas
* **Python**: Lenguaje principal.
* **Pandas**: Para la manipulación y limpieza de datos (ETL).
* **Matplotlib & Seaborn**: Para la visualización de datos.
* **Jupyter Notebook / Google Colab**: Entorno de desarrollo.

## 🔄 Flujo de Trabajo (Pipeline)
1.  **Extracción**: Carga de datos desde una API (JSON) alojada en GitHub.
2.  **Transformación (ETL)**:
    * Aplanamiento de datos anidados (`customer`, `phone`, `internet`, `account`).
    * Conversión de tipos de datos (Corrección de `TotalCharges` a numérico).
    * Limpieza de valores nulos y estandarización de categorías ("No internet service" -> "No").
3.  **Feature Engineering**: Creación de nuevas variables como `Charges.Daily`.
4.  **Análisis Exploratorio (EDA)**:
    * Cálculo de estadísticas descriptivas.
    * Visualización de distribución de Churn.
    * Análisis de fugas por tipo de contrato y servicios.
    * Análisis de correlaciones.

## 📊 Hallazgos Clave
* **Tasa de Evasión**: El **26.6%** de los clientes abandonaron el servicio.
* **Factor Crítico - Contratos**: Los clientes con contratos mensuales ("Month-to-month") tienen una tasa de evasión drásticamente superior a los de contratos de 1 o 2 años.
* **Antigüedad**: Existe una correlación negativa entre antigüedad y churn; los clientes nuevos son los más propensos a irse.
* **Servicios**: Los clientes sin servicios de seguridad online o soporte técnico tienden a cancelar más el servicio.

## 🚀 Cómo ejecutar este proyecto
1.  Clonar el repositorio.
2.  Instalar las dependencias: `pip install pandas matplotlib seaborn`.
3.  Ejecutar el notebook `Analisis_Churn_TelecomX.ipynb`.

---
*Proyecto realizado para el desafío de Data Science LATAM.*
