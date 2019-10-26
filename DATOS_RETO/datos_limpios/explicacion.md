# DATOS DE EXTRUSION

Último día de operacioes: 1 de octubre de 2019

Se eliminaron 3375 filas después del último día de operación registrado que no contenían información.

Después de elminar las filas con la mayoría de infromación faltante se llenaron los datos faltantes en el dataset resultante con interpolaciones según los valores existentes.

Las fechas tenían un formato escrito, es decir, estaban escritas con los nombres de los meses y días también por lo que se procesaron para obtener un formato homogéneo de fecha.

En la columna `'SEMANA'` había valores basura como `'#REF!'` que fueron sustituidos con valores nulos para después ser interpolados.

Después de limpiar los datos se genera una columna nueva de semana a partir de las fechas y se compara con la columna original para determinar el número de valores no coincidentes que fueron los siguientes:

índice | ORIGINALES | CALCULADOS
|:------------- |-------------:| -----:|
5323 | 20.0 | 21
5324 | 20.0 | 21
5325 | 20.0 | 21
5326 | 20.0 | 21
5327 | 20.0 | 21
6121 | 23.0 | 24
6122 | 23.0 | 24
7785 | 24.0 | 31
8590 | 34.0 | 35
8927 | 2.0 | 36
8928 | 2.0 | 36
8929 | 2.0 | 36
9050 | 3.0 | 36
9051 | 3.0 | 36


# DATOS IMPRESION

Ultimo dia de operaciones: 3 de Octubre de 2019

Habia 5546 filas con valor de fecha despues de las operaciones del ultimo dia de operaciones que fueron eliminadas del dataset.

Despues de la eliminacion anterior habia 3 valores nulos que fueron llenados con interpolacion de acuerdo a los valores existentes.

Habia 4 registros con fechas que no eran de 2019, por lo que se cambiaron los anhos a 2019. 

Habia 34 registros con valores nulos en semana y 8 con valores no compatibles con los demas 'ALVARADO 1.25K', '3/30/19', '30/', '4/11/19', '4/23/19', '7/3/19', '9/4/19', 'B' que se convirtieron a nulo. Luego generamos una tabla con los dias del anho con su correspondiente semana dentro del anho hicimos un merge con el dataset para ver si coincidian las semanas generadas con las que estaban en el dataset 

y encontramos 36 registros cuya fecha no coincidia por lo que corregimos.

índice | ORIGINALES | CALCULADOS
|:------------- |-------------:| -----:|
2019-03-01 | 0.0 | 9.0
2019-03-04 | 0.0 | 10.0
2019-03-27 | 0.0 | 13.0
2019-04-28 | 18.0 | 17.0
2019-04-28 | 18.0 | 17.0
2019-04-06 | 6.0 | 14.0
2019-01-16 | 16.0 | 3.0
2019-05-26 | 22.0 | 21.0
2019-05-29 | 0.0 | 22.0
2019-05-05 | 19.0 | 18.0
2019-05-05 | 19.0 | 18.0
2019-05-05 | 19.0 | 18.0
2019-05-05 | 19.0 | 18.0
2019-05-05 | 19.0 | 18.0
2019-05-05 | 19.0 | 18.0
2019-05-05 | 19.0 | 18.0
2019-05-05 | 19.0 | 18.0
2019-05-05 | 19.0 | 18.0
2019-05-05 | 19.0 | 18.0
2019-05-05 | 19.0 | 18.0
2019-05-05 | 19.0 | 18.0
2019-05-05 | 19.0 | 18.0
2019-05-05 | 19.0 | 18.0
2019-01-08 | 23.0 | 2.0
2019-06-26 | 0.0 | 26.0
2019-07-28 | 31.0 | 30.0
2019-08-25 | 35.0 | 34.0
2019-08-25 | 35.0 | 34.0
2019-08-25 | 35.0 | 34.0
2019-08-25 | 35.0 | 34.0
2019-08-25 | 35.0 | 34.0
2019-08-25 | 35.0 | 34.0
2019-08-25 | 35.0 | 34.0
2019-08-25 | 35.0 | 34.0
2019-09-01 | 36.0 | 35.0

En cada fila se muestra la fecha, la semana en el dataset y la semana calculada por nosotros

# DATOS SELLADO