# 📂 Aprendizaje Profundo Guiado por la Física para la Inversión No Supervisada de Datos de Resistividad Eléctrica en 1D

Este repositorio contiene la implementación de un enfoque de **aprendizaje profundo guiado por la física (Physics-Guided Deep Learning, PGDL)** para la **inversión no supervisada de datos de resistividad eléctrica en 1D**, típicamente obtenidos mediante **sondeos eléctricos verticales (SEV)**.

El método combina una red neuronal totalmente conectada con un **operador directo diferenciable**, basado en las ecuaciones físicas del problema (ley de Ohm y ecuación de Poisson), lo cual permite estimar perfiles de resistividad directamente desde los datos observados **sin necesidad de modelos etiquetados**.

## 🎯 Objetivo

- Estimar modelos de resistividad subterránea en 1D usando solo datos de resistividad aparente.
- Incorporar conocimiento físico en el entrenamiento de redes neuronales.
- Superar métodos tradicionales como IPI2Win o Pygimli en escenarios sintéticos y reales.

## 📒 Contenido

Este repositorio incluye un único notebook desarrollado para ser ejecutado en Google Colab:

> 📘 [`DL_VES_TEST1.ipynb`]

Este notebook contiene:

- Generación o carga de datos de resistividad aparente (sintéticos o reales).
- Definición del modelo neuronal en TensorFlow.
- Implementación del operador directo diferenciable.
- Función de pérdida basada en la física.
- Entrenamiento no supervisado del modelo.
- Visualización e interpretación de resultados.

## 🚀 Ejecución en Colab

Haz clic en el siguiente botón para abrir y ejecutar el notebook directamente en Google Colab:

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tu_usuario/tu_repositorio/blob/main/notebooks/PGDL_inversion_SEV_1D.ipynb)

## ⚙️ Requisitos

- TensorFlow ≥ 2.x  
- NumPy  
- Matplotlib  

> ⚠️ No necesitas instalar nada localmente si usas Google Colab.

## 📈 Resultados

El modelo reconstruye perfiles de resistividad precisos, incluso en presencia de ruido, y captura interfaces geológicas que los métodos clásicos tienden a suavizar o perder. El enfoque demuestra mayor precisión y resolución en comparación con IPI2Win y Pygimli.

## 📄 Licencia

Este código está disponible bajo la Licencia MIT.
