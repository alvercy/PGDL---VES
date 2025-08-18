# 📂 Aprendizaje Profundo Guiado por la Física para la Inversión No Supervisada de Datos de Resistividad Eléctrica en 1D

Este repositorio contiene la implementación de un enfoque de **aprendizaje profundo guiado por la física (Physics-Guided Deep Learning, PGDL)** para la **inversión no supervisada de datos de resistividad eléctrica en 1D**, típicamente obtenidos mediante **sondeos eléctricos verticales (SEV)**.

El método combina una red neuronal totalmente conectada con un **operador directo diferenciable**, basado en las ecuaciones físicas del problema (ley de Ohm y ecuación de Poisson), lo cual permite estimar perfiles de resistividad directamente desde los datos observados **sin necesidad de modelos etiquetados**.

## 📒 Contenido

Este repositorio incluye un único notebook desarrollado para ser ejecutado en Google Colab:

> 📘 [`DL_VES_TEST1.ipynb`]

Este notebook contiene:

- Generación o carga de datos de resistividad aparente (sintéticos).
- Definición del modelo neuronal en TensorFlow.
- Implementación del operador directo diferenciable.
- Función de pérdida basada en la física.
- Entrenamiento no supervisado del modelo.
- Visualización e interpretación de resultados.

## ⚙️ Requisitos

- TensorFlow ≥ 2.x  
- NumPy  
- Matplotlib  

> ⚠️ No necesitas instalar nada localmente si usas Google Colab.

## 📈 Resultados

El modelo reconstruye perfiles de resistividad precisos, incluso en presencia de ruido, y captura interfaces geológicas que los métodos clásicos tienden a suavizar o perder. El enfoque demuestra mayor precisión y resolución en comparación con IPI2win y pyGIMLi.

