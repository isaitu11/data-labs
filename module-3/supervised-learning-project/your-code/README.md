![IronHack Logo](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d5c5793015fec3be28a63c4fa3dd4d55.png)

# Supervised Learning Project

## Objetivo

* Lo que se pretende es construir un modelo que estime la calidad de los vinos en función de propiedades físicas y químicas. 
* Para ello, nos apoyamos en los datos que nos proporcionan unos expertos en el vino.

---

* En el conjunto de datos que hemos importado mediante pandas, se encuentran juntas la variable dependiente y las independientes, por lo que es necesario separarlas en dos conjuntos. El primer conjunto es 'x', con las variables independientes:
* **x** = wine **[features]**
El segundo es 'y', con la variable dependiente:
* **y** = wine **[target]**

---

* Una vez separadas las variables independientes de la dependiente, creamos un conjunto de entrenamiento y test utilizando la función **train_test_split**, que se usa para identificar la existencia del posible sobreajuste en el modelo. 
* Una vez hecho esto, se puede crear el modelo y comprobar los resultados obtenidos en ambos conjuntos de datos.

---

Los resultados obtenidos son:

- * R2 en **entrenamiento** es: 0.28323279729956563 
- * R2 en **validación** es: 0.2755723745472719

Esto significa que posiblemente exista sobreajuste en el conjunto, por lo que es necesario revisar las características utilizadas.



