#  Carpeta de Referencias

Esta carpeta reúne el material complementario y las entregas anteriores del proyecto **Diagnóstico de Endometriosis mediante Aprendizaje Automático**.

---

##  Primera entrega

Diagnóstico de Endometriosis
Profesor: Nicolas, Caballero.
Tema: Parcial Aprendizaje Automático
Estudiante: Guillermo, Carcamo.
Contexto y relevancia
La endometriosis es una enfermedad crónica que afecta aproximadamente al 10 % de las mujeres en edad
reproductiva (OMS, 2023).
Se caracteriza por el crecimiento de tejido endometrial fuera del útero, generando dolor pélvico, infertilidad y una
reducción significativa en la calidad de vida.
Su diagnóstico suele demorarse entre 7 y 10 años, debido a la complejidad clínica y a la falta de herramientas
predictivas confiables.
En este contexto, el aprendizaje automático ofrece la posibilidad de analizar datos clínicos para identificar patrones
que contribuyan a una detección temprana y precisa.
Este proyecto busca desarrollar un modelo predictivo que funcione como herramienta de apoyo al diagnóstico
médico, ayudando a reducir los tiempos y errores de detección de la endometriosis.
Objetivo general
Desarrollar un modelo de Aprendizaje Supervisado que prediga la probabilidad de padecer endometriosis a partir de
variables clínicas y de estilo de vida, utilizando técnicas de clasificación y reducción de dimensionalidad que
permitan mejorar la precisión y la interpretabilidad del modelo.
Objetivos específicos
• Analizar y limpiar el conjunto de datos clínicos, identificando valores faltantes, correlaciones y posibles
sesgos.
• Aplicar técnicas de análisis exploratorio y de reducción de dimensionalidad (PCA) para visualizar patrones
entre las pacientes.
• Entrenar y comparar modelos de clasificación.
• Evaluar el desempeño mediante métricas como Accuracy, Recall, F1-score y ROC-AUC.
• Determinar las variables más relevantes y su contribución al diagnóstico.
Tipo de Problema
El proyecto aborda un problema de clasificación binaria supervisada, dado que la variable objetivo (Diagnosis) indica
si la paciente presenta (1) o no (0) endometriosis.
Además, se complementará con un análisis exploratorio no supervisado (PCA) para detectar posibles agrupamientos
naturales entre las variables clínicas.
Modelos Propuestos (hasta el momento)
• Regresión Logística: modelo base utilizado para estimar probabilidades y analizar la influencia de cada
variable.
• Árbol de Decisión: permite generar reglas interpretables tipo “si–entonces” y visualizar la importancia de las
variables.
• Random Forest: mejora la precisión del árbol de decisión reduciendo el sobreajuste mediante el uso de
múltiples árboles.
• SVM (Support Vector Machine): clasificador robusto ante datos no lineales; se probarán kernels lineal y
radial.
• PCA (Análisis de Componentes Principales): técnica no supervisada para explorar relaciones entre variables
y visualizar la estructura de los datos.
Conclusión
El proyecto busca integrar modelos de aprendizaje automático con fundamentos médicos para mejorar la detección
temprana de la endometriosis.
Se propone un enfoque híbrido, combinando interpretabilidad y potencia predictiva.
A través de la comparación de distintos algoritmos, se espera identificar el modelo más eficaz y comprensible para su
aplicación en contextos clínicos reales, contribuyendo a reducir los tiempos de diagnóstico y mejorar la calidad de
vida de las pacientes.

##  Propósito

La carpeta `references/` permite mantener una **trazabilidad académica completa** del proyecto, conservando tanto el desarrollo técnico como las observaciones recibidas y las mejoras implementadas a lo largo de las entregas.
