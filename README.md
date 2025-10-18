# Diagnóstico de Endometriosis mediante Aprendizaje Automático

##  Contexto

Este proyecto se desarrolla en el marco de la materia **Aprendizaje Automático** de la carrera **Ciencia de Datos e Inteligencia Artificial**.  
El objetivo general es aplicar técnicas de *Machine Learning supervisado* para apoyar el diagnóstico de **endometriosis**, una enfermedad ginecológica crónica que afecta aproximadamente al **10 % de las mujeres en edad reproductiva** (OMS, 2023).

---

##  Objetivos del Proyecto

- Predecir la probabilidad de padecer endometriosis a partir de variables clínicas.  
- Evaluar distintos modelos de clasificación supervisada y comparar su desempeño.  
- Identificar las variables con mayor influencia en la predicción.  
- Generar un pipeline reproducible y documentado para futuras extensiones del análisis.

---

##  Dataset

| Característica | Descripción |
|----------------|-------------|
| **Fuente** | [Kaggle – Endometriosis Dataset](https://www.kaggle.com/datasets/michaelanietie/endometriosis-dataset) |
| **Registros** | 10.000 (sintéticos, no sensibles) |
| **Tipo** | Tabular, clínico |
| **Variable objetivo** | `Diagnosis` (0 = No Endometriosis / 1 = Endometriosis) |
| **Variables predictoras** | Edad, IMC, nivel de dolor, irregularidad menstrual, alteraciones hormonales, infertilidad, entre otras |

---

##  Metodología

El trabajo sigue la metodología de **Cookiecutter Data Science**, con un flujo ordenado de análisis:

1. **Exploración y limpieza de datos**  
   - Análisis descriptivo, detección de valores faltantes y outliers.  
   - Evaluación del balance de clases y correlaciones entre variables.

2. **Modelado base**  
   - Implementación de modelos de *Regresión Logística* y *Árbol de Decisión* como líneas base.  
   - División de datos en entrenamiento y prueba con `train_test_split`.  
   - Escalado de variables numéricas y codificación de categóricas.

3. **Evaluación comparativa**  
   - Métricas: Accuracy, Precision, Recall, F1-score y ROC-AUC.  
   - Matriz de confusión y curvas ROC/Precision-Recall.  
   - Análisis de importancia de variables.

4. **Informe final**  
   - Presentación de resultados, conclusiones y recomendaciones.

---

## Estructura del Repositorio

AA_Endometriosis/
│
├── README.md
├── LICENSE
├── requirements.txt
├── Makefile
│
├── data/
│   ├── raw/            <- Dataset original descargado de Kaggle
│   ├── interim/        <- Datasets limpios o con transformaciones parciales
│   └── processed/      <- Datasets finales listos para modelar
│
├── notebooks/
│   ├── 1.0-GC-exploracion.ipynb     <- Análisis exploratorio (EDA)
│   ├── 2.0-GC-modelado_base.ipynb   <- Modelos base (LogReg y Árbol)
│   └── 3.0-GC-evaluacion.ipynb      <- Evaluación y comparación de modelos
│
├── reports/
│   ├── figures/        <- Gráficos generados (EDA, curvas ROC, etc.)
│   ├── metrics/        <- Tablas de métricas, matrices de confusión
│   └── pdf/            <- Entregas exportadas en PDF
│
├── src/
│   ├── data/           <- Scripts de carga y limpieza
│   ├── features/       <- Feature engineering y escalado
│   ├── models/         <- Entrenamiento, evaluación y guardado
│   └── visualization/  <- Funciones de gráficos reutilizables
│
└── references/
    ├── notas_clase/                <- Apuntes de cátedra
    └── definiciones_teoricas.md    <- Conceptos y referencias teóricas



<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
