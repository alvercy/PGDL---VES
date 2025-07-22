📂 Aprendizaje Profundo Guiado por la Física para la Inversión No Supervisada de Datos de Resistividad Eléctrica en 1D
Este repositorio contiene la implementación de un enfoque de aprendizaje profundo guiado por la física (Physics-Guided Deep Learning, PGDL) para la inversión no supervisada de datos de resistividad eléctrica en 1D, típicamente obtenidos mediante sondeos eléctricos verticales (SEV).

El método combina una red neuronal totalmente conectada con un operador directo diferenciable, construido a partir de las ecuaciones físicas del problema (ley de Ohm y ecuación de Poisson), permitiendo estimar perfiles de resistividad directamente a partir de los datos de resistividad aparente sin necesidad de modelos etiquetados.

🎯 Objetivo
Estimar modelos de resistividad subterránea en 1D usando solo datos observados.

Incorporar el conocimiento físico del problema en el entrenamiento del modelo.

Superar en precisión y resolución a métodos tradicionales como IPI2Win o Pygimli.

📒 Contenido
El repositorio incluye un único notebook alojado en Google Colab:

📘 PGDL_inversion_SEV_1D.ipynb

Este notebook contiene todo el flujo de trabajo:

Preparación de datos sintéticos o reales.

Definición del modelo de red neuronal en TensorFlow.

Implementación del operador directo diferenciable.

Función de pérdida basada en la física.

Entrenamiento no supervisado del modelo.

Visualización de resultados.

⚙️ Requisitos
Google Colab

TensorFlow ≥ 2.x

NumPy

Matplotlib

Todo el entorno se configura automáticamente en Colab al ejecutar el notebook.
