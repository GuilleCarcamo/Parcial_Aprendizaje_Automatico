# Notebooks del Proyecto – Aprendizaje Automático

Esta carpeta contiene los **Jupyter Notebooks** desarrollados para el proyecto **Diagnóstico de Endometriosis mediante Aprendizaje Automático**.  
Cada notebook corresponde a una **etapa del proceso de análisis y modelado**, siguiendo la metodología del curso.

---

##  Estructura general

| Archivo | Descripción | Entrega |
|----------|--------------|----------|
| **1.0-GC-exploracion.ipynb** | Carga y descripción del dataset. Incluye cantidad de instancias, variables, tipos de datos, valores nulos y duplicados. 
| **2.0-GC-modelado_base.ipynb** | Entrenamiento de modelos base de clasificación (Regresión Logística y Árbol de Decisión). Incluye métricas, Curva ROC y Matriz de Confusión. 
| **3.0-GC-evaluacion.ipynb** | Implementación de Random Forest y comparación final con los modelos base. Incluye métricas, Curva ROC e Importancia de Variables. 
| **4.0-GC-exploracion_PCA.ipynbb** | Análisis exploratorio mediante PCA para detectar colinealidades y visualizar agrupamientos naturales. 

---

##  Rutas relativas

Cada notebook utiliza **rutas relativas** para mantener la portabilidad dentro de la estructura del proyecto (formato Cookiecutter Data Science):

```python
from pathlib import Path
import pandas as pd

DATA_PATH = Path("../data/raw/structured_endometriosis_data.csv")
df = pd.read_csv(DATA_PATH)
