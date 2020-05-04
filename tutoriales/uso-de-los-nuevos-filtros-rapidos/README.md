# Uso de los Nuevos Filtros Rápidos

Los nuevos filtros rápidos permiten seleccionar los registros que desees, filtrando aquellos cuyo valor sea igual a los registros seleccionados de una columna, quitando de la lista los seleccionados, filtrando por valores de una columna e incluso aplicando criterios sobre una columna. Todo de forma visual, sencilla y rápida para el usuario. **Filtra rápidamente.**

Veamos algún caso práctico sobre nuestra aplicación Winmotor V7:

Por ejemplo, listamos pedidos de compras o directamente desde el panel y, haciendo clic en un campo concreto de una columna con el botón derecho, localizamos "filtros" aplicables a la selección \(es posible seleccionar más de una fila\):

![](../../.gitbook/assets/image%20%28157%29.png)

Seleccionando más de una fila, el filtro se aplicará sobre el conjunto seleccionado:

![](../../.gitbook/assets/image%20%28454%29.png)

Entrando más en detalle, este submenú incluye una serie de opciones para filtrar una lista, es decir, para quitar de la lista aquellos registros que no cumplan una determinada condición. Las opciones disponibles son:

**Igual a seleccionados de la columna \(Control + F\)**

Si seleccionamos una o más filas de una misma columna, podremos dejar en la lista solamente aquellos registros que en la columna seleccionada contengan los mismos valores que los seleccionados.

**Filtro por columna \(Control + Shift + F\)**

Nos permite filtrar por una columna, o bien por **valores** o bien por **criterio**.

**Valores**

Presenta una lista con todos los valores distintos que tenga la columna seleccionada.

Podemos seleccionar uno o varios valores:

![](https://doc.velneo.es/assets/filtro_valores.png)

O escribir directamente el valor a buscar, en cuyo caso en la lista quedarán solamente los valores coincidentes con la cadena escrita y todos seleccionados:

![](https://doc.velneo.es/assets/filtro_valores_edicion.png)

Para localizar el dato podemos usar caracteres comodín:

| Expresión | Sintaxis | Descripción |
| :--- | :--- | :--- |
| Un carácter cualquiera | ? | Coincidencia con cualquier carácter individual. |
| Cero o más caracteres cualesquiera | \* | Coincidencia con uno o más caracteres. Por ejemplo, new\* devuelve cualquier texto que incluya "new", como newfile.txt. |
| Un carácter cualquiera del conjunto | \[ \] | Coincidencia con cualquier carácter especificado en el juego de caracteres que se incluya entre los corchetes. Por ejemplo \[ABC\]. |
| Un carácter cualquiera del rango indicado en el conjunto | \[ - \] | Coincidencia con cualquier carácter especificado en el juego de caracteres que se incluya entre los corchetes. Por ejemplo \[B-E\], devolverá todos los registros que contengan caracteres comprendidos en es rango \(B, C, D o E\). |

Si pulsamos el botón _aceptar_ se aplicará el filtro.

**Criterio**

Nos permite especificar un criterio de filtrado. Los criterios disponibles dependerán del tipo de dato de la columna y son:

* **Vacío**: dejará en la rejilla los registros que tengan la celda vacía.
* **No vacío**: dejará en la rejilla los registros que tengan algún contenido en la celda.
* **Mayor que**: pedirá que especifiquemos un dato y dejará en la rejilla aquellos registros que en la columna tengan un dato mayor al especificado.
* **Mayor o igual que**: pedirá que especifiquemos un dato y dejará en la rejilla aquellos registros que en la columna tengan un dato igual o mayor al especificado.
* **Menor que**: pedirá que especifiquemos un dato y dejará en la rejilla aquellos registros que en la columna tengan un dato menor que el especificado.
* **Menor o igual que**: pedirá que especifiquemos un dato y dejará en la rejilla aquellos registros que en la columna tengan un dato igual o menor al especificado.
* **Igual a**: pedirá que especifiquemos un dato y dejará en la rejilla aquellos registros que en la columna tengan un dato igual al especificado.
* **Distinto de**: pedirá que especifiquemos un dato y dejará en la rejilla aquellos registros que en la columna tengan un dato distinto del especificado.
* **Está entre**: pedirá que especifiquemos dos valores y dejará en la rejilla aquellos registros que en la columna tengan un valor comprendido entre ambos.
* **No está entre**: pedirá que especifiquemos dos valores y dejará en la rejilla aquellos registros que en la columna tengan un valor no comprendido entre ambos.
* **Contiene**: pedirá que introduzcamos una cadena y dejará en la rejilla aquellos registros que la contengan.
* **No contiene**: pedirá que introduzcamos una cadena y dejará en la rejilla aquellos registros que no la contengan.
* **Verdadero**: para campos booleanos. Dejará en la rejilla los que tengan el campo = 1.
* **Falso**: para campos booleanos. Dejará en la rejilla los que tengan el campo = 0.

**Filtro por fórmula \(Control + F3\)**

La condición a evaluar se establecerá por medio de una fórmula por lo que se abrirá el asistente para la edición de fórmulas. En él tendremos acceso a las **Funciones estándar** de fórmulas, a la **lista de campos de la tabla** y a las **variables del sistema**.

Una vez establecida la condición, pulsar el botón _aceptar_ para ejecutar el filtro o el botón _cancelar_ para cancelarlo.

**Quitar seleccionados \(Control + Shift + U\)**

Como su propio nombre indica, permite quitar de la lista todos los registros que estén seleccionados.

Para más información y detalle, os dejamos un vídeo de Velneo sobre los nuevos filtros rápidos aplicados a la versión 25.

{% embed url="https://youtu.be/r0yCNrfTUaM" %}



