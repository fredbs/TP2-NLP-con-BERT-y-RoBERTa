# TP2-NLP-con-BERT-y-RoBERTa

**Autor:**Brito, Fred

**Resumen:** Este proyecto trata sobre el análisis de tuits, con el objetivo de realizar un Análisis de Sentimiento utilizando los modelos pre-entrenados BERT y RoBERTa, para luego implementar nuestro propio modelo de predección de sentimientos. 

En particular, tanto BERT como RoBERTa se ajustarán utilizando el conjunto de datos proporcionado para mejorar el rendimiento general del modelo.

Antes de enviar los datos a los algoritmos, los tweets se limpiarán profundamente para eliminar enlaces, hashtags al final de las oraciones y puntuación para permitir que los algoritmos comprendan mejor el texto y mejoren el rendimiento de la predicción.

**Objetivo:** El objetivo de este trabajo es perfilar el uso correcto de NLP.


**Descripción de Datos:** Lista de documentos .txt en idioma Inglés. Contiene  lineas de texto que representan emociones y sus respectivas etiquetas que clasifican dicha emociones, la cual puede pertenecer a una de las siguientes clases:
* 'sadness'
* 'anger'
* 'love'
* 'surprise'
* 'fear'
*  'joy

El conjunto de datos se encuentra dividido en train.txt, test.txt y val.txt para facilitar la construcción del modelo de aprendizaje automático.

  Los mismos serán importados desde kaggle:
  https://www.kaggle.com/praveengovi/emotions-dataset-for-nlp

  Se puede usar la API command de kaggle:
  `kaggle datasets download -d praveengovi/emotions-dataset-for-nlp`

| Etiqueta | Tipo de Dato | Descripción |
| :--- | :--- | :--- |
| text  | Texto (string)   | Linea de texto que expresa un sentimiento | 
| emotion  | Texto (string) | Etiqueta de emoción expresado en text| 

Ejemplo:

| text | emotion |
| :--- | :--- | 
| i feel like I am still looking at a blank canvas blank pieces of paper  | sadness  |  

**Nota:** La columna text ya posee un preprocesamiento de limpieza de datos.
