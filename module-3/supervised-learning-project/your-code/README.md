![IronHack Logo](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d5c5793015fec3be28a63c4fa3dd4d55.png)

# Supervised Learning Project


## Predicción calidad de los vinos.

Este proyecto es el correspondiente al proyecto correspondiente al módulo 3 del curso Data Analytics de IronHack.

El objetivo de este proyecto es implementar un solución utilizando un algoritmo de aprendizaje automático supervisado. Al existir múltiples tipos de modelos, lo idóneo es construir varios modelos y elegir el que más se ajusta a nuestro contenido e intención.

---

## Objetivo

* Lo que se pretende es construir un modelo que estime la calidad de los vinos en función de propiedades físicas y químicas. 
* Para ello, nos apoyamos en los datos que nos proporcionan unos expertos en el vino.

---

## Pre-requisitos para la visualización del proyecto

- import numpy as np
- import pandas as pd
- import matplotlib.pyplot as plt
- from sklearn.linear_model import LinearRegression
- from sklearn.model_selection import train_test_split

---

## Extracción, tratamiento y limpieza de los datos

Para este primer tratamiento de datos, he aprovechado el dataset que he usado en el projecto de Visualizaciñon de datos del módulo 2, ya que ahí hice el trabajo de limpieza de datos.


* a. https://archive.ics.uci.edu/ml/datasets/Wine+Quality 
* b. Dos dataset, uno de vinos tintos y otro de vinos blancos
* c. Trabajamos primero los dos por separado


### Información del dataset

Incluye los siguientes campos:

* 1 - fixed acidity 
* 2 - volatile acidity 
* 3 - citric acid 
* 4 - residual sugar 
* 5 - chlorides 
* 6 - free sulfur dioxide 
* 7 - total sulfur dioxide 
* 8 - density 
* 9 - pH 
* 10 - sulphates 
* 11 - alcohol 
* Output variable (based on sensory data): 
* 12 - quality (score between 0 and 10)

---

## Búsqueda del mejor modelo


* En el conjunto de datos que hemos importado mediante pandas, se encuentran juntas la variable dependiente y las independientes, por lo que es necesario separarlas en dos conjuntos. 

* El primer conjunto es 'x', con las variables independientes:

* **x** = wine **[features]**

El segundo es 'y', con la variable dependiente:

* **y** = wine **[target]**

---

* Una vez separadas las variables independientes de la dependiente, creamos un conjunto de entrenamiento y test utilizando la función **train_test_split**, que se usa para identificar la existencia del posible sobreajuste en el modelo. 
* Una vez hecho esto, se puede crear el modelo y comprobar los resultados obtenidos en ambos conjuntos de datos.

---

## Resultados

Los resultados obtenidos son:

- * R2 en **entrenamiento** es: 0.28323279729956563 
- * R2 en **validación** es: 0.2755723745472719

Esto significa que posiblemente exista sobreajuste en el conjunto, por lo que es necesario revisar las características utilizadas.

---

### Modelo utilizado

El modelo entrenado y evaluado: **Regression Linear**

### Agradecimientos

Octavio :)

