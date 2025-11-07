

# Clasificación de Currículums y Extracción de Habilidades con NLP

##  Descripción General

Este proyecto aborda la **clasificación de currículums** y la **extracción de habilidades profesionales** utilizando diferentes enfoques de **Procesamiento del Lenguaje Natural (NLP)**.
Se implementaron modelos basados en **transformers**, **redes neuronales** y **métodos clásicos**, evaluando su rendimiento en un dataset de más de **2.400 currículums** categorizados por área laboral.

##  Objetivo

Desarrollar y comparar modelos supervisados capaces de identificar la categoría laboral y extraer habilidades relevantes, asegurando una evaluación justa mediante el uso de métricas como **Accuracy**, **Precision**, **Recall** y especialmente **F1-Score ponderado**, que se adoptó como métrica principal por su robustez frente al desbalance de clases.

##  Preparación y Procesamiento de Datos

Antes del entrenamiento, se aplicaron distintas estrategias para **mejorar la calidad y representatividad de los datos**:

* **Mitigación de ruido:** limpieza de texto, control de vocabulario y eliminación de términos irrelevantes.
* **Manejo del desbalance de clases:** aumento de datos (data augmentation) en categorías minoritarias usando técnicas de reemplazo y permutación de palabras.
* **División estratificada:** separación rigurosa en conjuntos de entrenamiento, validación y prueba para evitar fugas de información.
* **Vectorización controlada:** tokenización y representación de texto adaptadas a cada tipo de modelo (TF-IDF, embeddings, o tokenización de transformers).

Estas acciones garantizaron un flujo de datos consistente, limpio y libre de sesgos, optimizando el desempeño de los modelos.

##  Modelos Implementados

1. **DistilBERT / RoBERTa-base (fine-tuned)**
2. **Word2Vec + BiLSTM**
3. **CNN-1D**
4. **TF-IDF + XGBoost (GPU)**
5. **FastText**

##  Resultados y Conclusiones

Cada modelo fue entrenado y evaluado bajo el mismo esquema experimental.
Los resultados evidenciaron diferencias en rendimiento y eficiencia, destacando los modelos **basados en transformers** por su mayor precisión, aunque con mayor costo computacional.
El análisis demuestra la efectividad del NLP en tareas de **análisis automatizado de currículums**, aportando valor en procesos de **selección y gestión del talento humano**.




```{tableofcontents}
```
