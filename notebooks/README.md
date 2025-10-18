# Notebooks del Proyecto – Aprendizaje Automático

Esta carpeta contiene los **cuadernos de trabajo (Jupyter Notebooks)** desarrollados para el proyecto **Diagnóstico de Endometriosis mediante Aprendizaje Automático**.  
Cada notebook corresponde a una **etapa del proceso de análisis y modelado**, siguiendo la metodología del curso.

---

##  Estructura general

| Archivo | Descripción | Entrega |
|----------|--------------|----------|
| **1.0-GC-exploracion.ipynb** | Carga y descripción del dataset. Incluye cantidad de instancias, variables, tipos de datos, valores nulos y duplicados. | Entrega 2 |

---

##  Rutas relativas

Cada notebook utiliza **rutas relativas** para mantener la portabilidad dentro de la estructura del proyecto (formato Cookiecutter Data Science):

```python
from pathlib import Path
import pandas as pd

DATA_PATH = Path("../data/raw/structured_endometriosis_data.csv")
df = pd.read_csv(DATA_PATH)
