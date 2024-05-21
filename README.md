<h1 align="center"><b><big>💸Financial Fraud detection📊</big></b></h1>




![](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)![Scikit-learn Logo](https://img.shields.io/badge/scikit--learn-5C9CD9?style=for-the-badge&logo=scikit-learn&logoColor=white)![Machine Learning](https://img.shields.io/badge/Machine%20Learning-008000?style=for-the-badge)![](https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white)![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)![](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)![Seaborn Logo](https://img.shields.io/badge/Seaborn-3881E3?style=for-the-badge&logo=seaborn&logoColor=white)

---

La surgencia por detectar fraudes en transacciones móviles de dinero ha llevado a una empresa del segmento Fintech a buscar soluciones innovadoras. 
Como científicos de datos hemos sido convocados para desarrollar un modelo de machine learning que pueda distinguir de manera precisa entre transacciones legítimas y fraudulentas, 
estableciendo así un estándar de seguridad en el sector financiero móvil global.

## Objetivo 📋

Desarrollar un modelo de machine learning altamente preciso y confiable que pueda distinguir de manera precisa entre transacciones legítimas y fraudulentas en el sector financiero móvil global. Este modelo establecerá un estándar 
de seguridad líder en la industria al proporcionar una detección precisa y temprana de actividades fraudulentas, protegiendo así los activos y la privacidad de los usuarios de servicios financieros móviles en todo el mundo. 
Nuestro objetivo es no solo detectar y prevenir fraudes, sino también generar confianza en las transacciones móviles y garantizar una experiencia segura y sin problemas para los usuarios, fortaleciendo así la integridad y la reputación del sector financiero móvil global.

## Problematica 🚫 


Nos enfrentamos a un desafío significativo al trabajar con un conjunto de datos de seis millones de registros, donde la variable objetivo "isFraud" presenta un desequilibrio considerable: el 99% de las transacciones son clasificadas como no fraudulentas, 
mientras que solo el 0.1% se catalogan como fraudulentas.

+ Etiqueta 0: Transacción legítima. ⭕️
+ Etiqueta 1: Transacción fraudulenta. ❌

Este desequilibrio en la distribución de las etiquetas presenta un desafío para entrenar modelos de machine learning que puedan detectar con precisión las transacciones fraudulentas en medio de una mayoría abrumadora de transacciones legítimas. La tarea consiste en desarrollar
estrategias efectivas para abordar este desequilibrio y crear modelos que puedan identificar con precisión los casos de fraude.
  
<p align="center">
  <img src="https://github.com/GabrielChavezC/Financial_Fraud_Detection/assets/155968191/38603db4-c7ef-4e57-9aca-b2c7f362005d" alt="Descripción de la imagen">
</p>

## **Conociendo a los datos** 🗺️

Como podemos observar, el primer día del mes es cuando se registran la mayoría de las transacciones.

<p align="center">
  <img src="https://github.com/GabrielChavezC/Financial_Fraud_Detection/assets/155968191/008a3d47-7aa2-42bd-8464-dfbaa49d5ad7" alt="Descripción de la imagen">
</p>


El rango en donde se hacen mas transacciones son en la tarde y noche.

<p align="center">
  <img src="https://github.com/GabrielChavezC/Financial_Fraud_Detection/assets/155968191/9e252d48-3d28-463d-b685-65febb22fd2f" alt="Descripción de la imagen">
</p>


# **Feature engineering** 💻

La creación de nuevas variables es una práctica fundamental en el desarrollo de modelos de machine learning, ya que puede mejorar significativamente la capacidad predictiva y 
la eficacia general del modelo. Al introducir nuevas variables derivadas de las características existentes, se puede capturar información adicional y mejorar la representación de los datos.

Métodos utilizados. 📚

+ get_dummies: Se utiliza para convertir variables categóricas en variables dummy.

+ Standarscaler: Se u para estandarizar las características numéricas de un conjunto de datos.

  ![image](https://github.com/GabrielChavezC/Financial_Fraud_Detection/assets/155968191/7af82d5c-e39a-4987-89f6-cb516a88320f)


# **Modelado** 🔎

## Modelos utilizados 📋

+ Decision Tree Classifier
+ RandomForestClassifier
+ LogisticRegression
+ HistGradientBoostingClassifier

  ## Métricas evaludas de cada modelo 📉

| Algoritmo                       | Estrategia                  | Recall | AUC-ROC | Precisión | Exactitud | F1-score | Tiempo (s) |
| ------------------------------- | --------------------------- | ------ | ------- | --------- | --------- | -------- | ---------- |
| DecisionTreeClassifier          | Penalización para compensar | 0.51   | 0.71    | 0.46      | 0.91      | 0.01     | 65         |
| RandomForestClassifier          | Penalización para compensar | 0.89   | 0.88    | 0.008     | 0.87      | 0.01     | 27         |
| HistGradient BoostingClassifier | Penalización para compensar | 0.90   | 0.89    | 0.01      | 0.89      | 0.02     | 22         |
| Logistic Regression             | Penalización para compensar | 0.87   | 0.85    | 0.006     | 0.84      | 0.85     | 466        |

# Métricas
![image](https://github.com/GabrielChavezC/Financial_Fraud_Detection/assets/155968191/8057ace6-9ff2-44ac-a9a0-a2ccde81f440)

# Matriz de Confusión
![image](https://github.com/GabrielChavezC/Financial_Fraud_Detection/assets/155968191/67bc6cf1-ca83-43bb-958f-46b7613eb49e)

# ¿Cúal Seria el mejor Modelo? ❓


## HistGradient Boosting Classifier 📊 💯

| Algoritmo               | Estrategia                  | Recall | Auc-Roc | Precision | Accuracy | F1-score |
|-------------------------|-----------------------------|--------|---------|-----------|----------|----------|
| HistGradientBoostingClassifier | Penalización para compensar | 0.90   | 0.89    | 0.01      | 0.88     | 0.02     |



Matriz de Confusión.

|        |        |
|--------|--------|
| 1415126| 173561 |
| 186    | 1782   |



En este escenario, el modelo demostró un desempeño superior al predecir con mayor precisión los verdaderos negativos, identificando correctamente 1782 transacciones fraudulentas. Además, exhibió una baja tasa de falsos positivos, con solo 186 casos de 
transacciones legítimas clasificadas erróneamente como fraudes. Este aspecto es crítico, ya que minimiza el riesgo de pérdidas para la empresa.

Sin embargo, hay margen para mejorar la identificación de los falsos negativos, que representan 173561 transacciones legítimas erróneamente etiquetadas como fraudulentas. Reducir esta cifra no solo optimizará los costos asociados 
con la verificación de estas transacciones, sino que también mejorará la experiencia del cliente al evitar bloqueos innecesarios de sus transacciones legítimas.


## Estrategias para mejorar el Modelo 📈

 Lidiar con un conjunto de datos de seis millones de registros, donde apenas el 0.01% se clasifican como fraudulentos, plantea un desafío significativo que los científicos de datos debemos abordar. Nuestro objetivo fue reducir las transacciones incorrectamente 
 identificadas como fraude, logrando un alto recall. Sin embargo, debido al volumen de datos, enfrentamos un problema de falsos positivos, donde transacciones legítimas se clasifican erróneamente como fraudulentas, con consecuencias potencialmente costosas para el departamento 
 encargado de investigar estas incidencias.

Para mitigar este problema, proponemos la inclusión de más características en nuestro modelo de detección de fraude. Esto nos permitirá mejorar nuestras predicciones y reducir la tasa de falsos positivos, aumentando así la eficiencia y precisión de nuestro sistema de detección.

![image](https://github.com/GabrielChavezC/Financial_Fraud_Detection/assets/155968191/d1621216-19b6-447c-8b5f-8ccf6dd99830)

