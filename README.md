# Diagnóstico de Endometriosis mediante Aprendizaje Automático

##  Contexto

Este proyecto se desarrolla en el marco de la materia **Aprendizaje Automático** de la carrera **Ciencia de Datos e Inteligencia Artificial**.  
El objetivo general es aplicar técnicas de *Machine Learning supervisado* para apoyar el diagnóstico de **endometriosis**, una enfermedad ginecológica crónica que afecta aproximadamente al **10 % de las mujeres en edad reproductiva** (OMS, 2023).

---

##  Objetivos del Proyecto

Desarrollar, entrenar y comparar modelos de clasificación supervisada que permitan estimar la probabilidad de diagnóstico de endometriosis.

**Objetivos específicos**

Realizar una exploración y descripción completa del dataset.

Analizar la relación entre síntomas clínicos y diagnóstico.

Entrenar y comparar múltiples modelos supervisados:

Regresión Logística (modelo base)

Árbol de Decisión

Random Forest

Evaluar el desempeño mediante métricas cuantitativas (Accuracy, Precision, Recall, F1, ROC-AUC) y análisis visual (Curvas ROC, Matriz de Confusión).

Interpretar los resultados desde una perspectiva técnica y aplicada, orientada al apoyo diagnóstico.
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

##  Estructura del Repositorio

La siguiente estructura sigue el estándar **Cookiecutter Data Science**, adaptado al proyecto.

```bash
Parcial_Aprendizaje_Automatico/
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
├── notebooks/          <- Carpeta reservada para los notebooks del proyecto
│
├── reports/
│   ├── figures/        <- Gráficos generados (EDA, curvas ROC, etc.)
│   ├── metrics/        <- Tablas de métricas, matrices de confusión
│   └── pdf/            <- Entregas exportadas en PDF
│
└── references/
    └── notas_clase/                <- Apuntes de cátedra
