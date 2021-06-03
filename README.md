# Modelo para la Detección de Depresión
La depresión es un trastorno mental que afecta a alrededor de 300 millones de personas alrededor del
mundo. Por eso, es un tema que ha sido muy estudiado en el área de Inteligencia Artificial. Este proyecto tuvo
como objetivo construir un modelo de NLP para detectar si un texto tiene un tono depresivo o no. El trabajo fue inspirado 
por el siguiente paper: https://arxiv.org/abs/1804.07000.

## Para correr la aplicación
En este repositorio se proporcionan todos los archivos generados por el código para que se puedan incluir en el ambiente. No obstante,
se usó una base de datos externa que no se incluye aquí, revisar la sección de **Notas adicionales**. El archivo que contiene la 
implementación principal es el Jupyter Notebook, y el resto de los archivos son necesarios para correrlo, o bien, son producto
de este Jupyter Notebook.

Dentro del mismo Notebook se proporcionan explicaciones del código que se realizó, así como el razonamiento detrás de la lógica que 
se usó y el análisis que se hizo a lo largo del desarrollo de este proyecto.

Para correr el Notebook en Google Colab, este se debe cargar al ambiente, y además, los otros archivos (especialmente el requirements.txt) deben subirse al ambiente para que todo funcione adecuadamente. 

## Funcionalidad principal
El trabajo realizado consiste en dos partes principales:
- Creación del dataset
- Transfer-learning aplicado a 3 modelos que incorporan transformadores, importados del módulo de [HuggingFace](https://huggingface.co/models)

Ambas secciones se explican en detalle dentro del Notebook.

## Poster académico
Dentro de este mismo repositorio se encuentra el póster académico que se realizó. Checar el archivo **Poster Academico A01282778.pdf**.

## Notas adicionales
- La base de datos utilizada se puede encontar en la siguiente [liga](https://www.kaggle.com/nikhileswarkomati/suicide-watch/version/13).
- Los archivos presentes en el folder **Data** deben cargarse en el **folder raíz** de Google Collab. Si se carga el folder Data directamente
el Notebook no leerá los archivos correctamente.
- Es necesario proporcionar un **client_id** y un **client_secret** del API de Reddit. Se puede crear una App con esos datos en la siguiente [liga](https://ssl.reddit.com/prefs/apps/). Es necesario contar con una cuenta de Reddit para poder crear la app.
