# Explicacion 

## Exploracion

Al principio hicimos fue la exploracion de los datos, lo primero fue obtencion de estadisticas basicas de cada una de las columnas del dataset. Al parecer los datos tienen medidas muy parecidas en las variables, por lo que se utiliza para el siguiente paso solamente el conjunto de entrenamiento. Luego, obtuvimos la correlacion dos a dos de las columnas y la variable objetivo con lo que pudimos observar como se relaciona la variable 0 con la variable 4 (la variable objetivo) de manera lineal con lo que un modelo líneal simple con estas dos variables podŕia ser suficiente. Para este paso usamos el lenguaje de programacion python con la libreria pandas. 

## Proceso de creacion del Algoritmo e implementacion

Realizamos varios intentos con distintos modelos, pero para cada uno de ellos escalamos los datos de modo que cada una de sus columnas tuviera media cero y desviacion estantar 1 (Escalamiento Estandar). El criterio para decidir el mejor modelo fue la norma MSE (Mean Square Error) con las variables objetivo de los datos de prueba. Todos nuestros modelos fueron generamos con el lenguaje de programacion python con la libreria scikitlearn.

* Modelo 1: Linear Regression - MSE = 28.630616849456338
* Modelo 2: Decision Tree Regression con  random_state=0 - MSE = 21.35690773249739
* Modelo 3: Multi Layer Perceptron Network Regression con activation=logistic, hidden_layer_sizes=(32, 24, 32) y solver=adam - MSE = 17.265880970119255.

Por lo que escogimos el Modelo 3 para calcular las variables objetivo de los datos de validacion. Evidencias: [https://github.com/zs10011598/dci4].

## Integrantes 

- Pedro R (Capitan) [promerowork26@gmail.com]
- Santiago [santiago.gm1191@gmail.com]
- Daniel [angel.rm.daniel@gmail.com]
- Victor [vida092@gmail.com]
