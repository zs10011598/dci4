
Con los datos limpios nuestras respuestas sobre las estadisticas generales fueron las siguientes usando los notebooks adjuntos.

## Pregunta 1

En cada una de los datasets(extrusion, impresion y sellado) encontramos 40 semanas.


## Pregunta 2

### Extrusion
 
SEMANA   freq   
1        131
2        289
3        229
4        255
5        270
6        202
7        334
8        239
9        299
10       265
11       263
12       270
13       298
14       352
15       346
16       163
17       307
18       275
19       277
20       269
21       250
22       333
23       212
24       208
25       225
26       283
27       207
28       217
29       173
30       246
31       157
32       243
33       251
34       258
35       305
36       264
37       278
38       143
39       252
40        46

### Impresion

SEMANA   freq      
1.0       58
2.0      118
3.0      124
4.0       90
5.0      144
6.0       85
7.0      115
8.0      106
9.0      159
10.0     163
11.0     176
12.0     188
13.0     216
14.0     181
15.0     173
16.0     119
17.0     178
18.0     278
19.0     165
20.0     211
21.0     247
22.0     197
23.0      88
24.0     202
25.0     205
26.0     177
27.0     200
28.0     202
29.0     126
30.0     158
31.0     123
32.0     178
33.0     182
34.0     179
35.0     159
36.0     159
37.0     166
38.0     156
39.0     127
40.0      94

## Sellado

SEMANA    freq      
1         31
2         64
3         66
4         83
5         98
6         67
7         79
8         77
9         83
10       101
11        82
12        89
13       116
14       122
15       123
16        79
17       129
18       112
19       114
20        96
21       100
22       109
23       111
24       100
25        95
26        90
27        89
28        98
29        98
30       103
31        69
32       100
33       108
34       116
35       102
36       113
37       116
38        79
39       107
40        54


## Pregunta 3

### Extrusion

Encontramos 9 operadores.

### Impresion 

Encontramos 11 operadores.

### Sellado

Encontramos 63 operadores.


## Pregunta 4

Encontramos 10 extrusoras identificadas por 2, 4, 5, 6, 7, 8 , 10, 11, 12 y 13.


## Pregunta 5

Encontramos 6 impresoras identificadas por 4, 5, 6, 7, 8 y 9.


## Pregunta 6

### Extrusion

Promedio de turnos por operador: 1098.222222

### Impresion 

Promedio de turnos por operador: 579.272727

### Sellado

Promedio de turnos por operador: 59.809524


## Pregunta 7

Se puede observar por la descripción de los datos que los primeros tres cuartiles son consistentes a diferencia del último que parece contener outliers con valores muy altos, dado que el máximo en el calibre real está en el orden 1x10^4. Se adjuntan unas gráficas de caja en el notebook para observar este frnómeno.

Como se puede observar en el caso del calibre pedido la mayoría de los datos se concentran entre los valores 50 y 200, en el caso del calibre real parece que también, a continuación se eliminan los outliers y se plotean gráficas de caja e historgramas para verificar sus distribuciones.

Por lo que se puede observar en las gráficas de cajas ambas distribuciones son muy similares, esto también se ve reflejado en la descripción de los datos en la media y la desviación estandar. 

Como se puede observar en las series de tiempo se confirma, en su mayoría, la similitud de las distribuciones a excepción del mes de julio donde se observa una diferencia notable entre el pedido y el real, lo que motiva a una rervisión en los procesos de esas fechas para buscar la posible causa de este fenómeno.


## Pregunta 8

Al igual que en la pregunta 7, en el proceso de extrusión, la mayoría de los valores se encuentran aglomerados entre 20 y 200 con algunos valores outliers fuera de este rango. Los outliers son omitidos y se vuelven a graficar los datos con un diagrama de cajas y un histograma para observar su distribución.

Como se puede observar en estas últimas gráficas, despueśde el proceso de sellado hay una importante pérdida de material, con ello se podría cuantificar la merma despúes de cada proceso.


## Pregunta 9

Retomando el histograma de la distribución de los valores de la variable calibre del dataset de sellado podemos observar varios montículos siendo los más prominentes el que se aglomera al rededor de 60 aproximadamente y el que se aglomera al rededor de 200. Con lo que podemos intuir que sigue una distribución de probabilidad multinomial con m=2.


## Pregunta Adicional 1

En base a las graficas generadas adjuntas concluimos lo siguiente

### Extrusion

* Turno 1: Jueves
* Turno 2: Jueves
* Turno 3: Miercoles

### Impresion

* Turno 1: Jueves
* Turno 2: Jueves
* Turno 3: Miercoles

### Sellado

* Turno 1: Jueves
* Turno 2: Jueves
* Turno 3: Martes


## Pregunta Adicional 2

En base a las graficas generadas adjuntas concluimos lo siguiente

### Extrusion

* Turno 1: Mayo
* Turno 2: Abril
* Turno 3: Mayo

### Impresion

* Turno 1: Mayo
* Turno 2: Mayo
* Turno 3: Abril

### Sellado

* Turno 1: Abril
* Turno 2: Abril
* Turno 3: Mayo


## Pregunta Adicional 8

Imagenes: `mes_3_clibre.png` y `semana_3_calibre.png`. 