# Detección de Sesgos de Género en Traducción Automática 🤖🌐

Proyecto de Machine Learning enfocado en detectar y predecir la presencia de sesgos de género en las traducciones del inglés al español, analizando si se mantienen estereotipos en diversas profesiones.

### 📊 Descripción
Se utiliza un dataset de frases en inglés que vinculan profesiones con acciones específicas. A través de la librería `deep_translator`, se procesan las traducciones al español para identificar si el modelo asigna géneros de forma sesgada (ej. asociar sistemáticamente "physician" con "el" o "nurse" con "la").

### 🎯 Objetivo
Construir un modelo de clasificación binaria capaz de predecir la probabilidad de que una traducción contenga un sesgo de género, evaluando la precisión de los sistemas de traducción automática actuales.

### ⚙️ Tecnologías
* Python
* Pandas / NumPy (Procesamiento de datos)
* Scikit-learn (Machine Learning & TF-IDF)
* Deep-translator (Integración con Google Translator API)
* Matplotlib / Seaborn (Visualización de datos)

### 🔍 Proceso
1. Carga y Limpieza: Procesamiento de datasets "Pro-Estereotipo" y "Anti-Estereotipo".
2. Pipeline de Traducción: Traducción automatizada y normalización de texto mediante Regex.
3. Detección de Sesgos: Creación de una lógica de etiquetado basada en concordancia de género.
4. Ingeniería de Características: Transformación de texto a vectores numéricos usando **TF-IDF**.
5. Entrenamiento: Implementación de un modelo **Random Forest Classifier** con balanceo de clases.
6. Evaluación: Análisis mediante matrices de confusión y reportes de precisión/recall.

### 📈 Resultados
El modelo alcanzó una **precisión del 81.25%**, demostrando una alta capacidad para identificar automáticamente cuándo una traducción ha incurrido en un sesgo de género basado en el contexto de la frase.

### 🚀 Uso
```bash
pip install pandas numpy scikit-learn deep-translator seaborn matplotlib
# Ejecutar el notebook o script principal
python Proyecto_final.py
```

### 📁 Dataset
Dataset basado en esquemas de resolución de correferencia (tipo Winogender/WinoBias) adaptado para pruebas de traducción automática.
