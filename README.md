# Análisis de Cancelación en TelecomX

## 1. Descripción del Proyecto 

Este notebook realiza un **análisis exploratorio de datos** sobre la evasión de clientes (cancelación) en TelecomX, con el objetivo de:
- Identificar patrones y características de los clientes que cancelan.
- Entender cómo variables como gasto total, factura mensual y antigüedad se relacionan con el churn.
- Proveer insights y recomendaciones para mejorar la retención.

## 2. Estructura del Repositorio 

challenge2-data-science-LATAM/
├── README.md ← Este documento de introducción y guía
├── TelecomX_Data.json ← Archivo fuente con los datos brutos (extraídos vía API)
├── TelecomX_LATAM.ipynb ← Notebook principal con todo el código, gráficos y análisis
└── TelecomX_diccionario.md ← Diccionario de datos: descripción de cada campo del JSON

## 3. Uso (Google Colab)

Antes de todo, asegúrate de importar las librerías necesarias ejecutando esta celda al principio:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

1. Abre Colab y carga directamente desde GitHub:
   - Ve a https://colab.research.google.com  
   - En la pestaña **GitHub**, pega la URL de tu repositorio:
     ```
     https://github.com/RaulMirabal28/challenge2-data-science-LATAM.git
     ```
   - Selecciona el archivo `TelecomX_LATAM.ipynb` y haz click en **Abrir**.

2. (Opcional) Si quieres guardar cambios en tu propio Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```
3. Instalar dependencias (si es necesario)

   ```!pip install pandas numpy matplotlib seaborn```

4. Ejecutar el notebook
  - Corre todas las celdas en orden:
  - Importaciones y carga de datos
  - Limpieza y transformación
  - EDA y visualizaciones
  - Conclusiones y recomendaciones

5. Contenido del Notebook

  - Carga y limpieza de datos – Normalización, conversión de tipos, tratamiento de outliers e inconsistencias.
  - Análisis descriptivo – Resúmenes estadísticos y visualizaciones iniciales (distribuciones, proporciones y creación de nuevas variables como CostoDiario).
  - Visualizaciones avanzadas – Boxplots comparativos de gasto, tenencia y factura mensual.
  - Conclusiones e Insights – Principales hallazgos sobre patrones de cancelación.
  - Recomendaciones – Estrategias de retención temprana, ajuste de precios y fidelización.
