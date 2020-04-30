# Crear un Importador de Tarifa de Marca

En éste tutorial vamos a crear un[ importador](./) para una marca en particular.

De ésta forma habrá uno o varios importadores almacenados para las marcas que la empresa gestione y posteriormente ir actualizando las nuevas tarifas con sólo pulsar un botón y modificar el archivo para adecuarlo al importador creado.

**Al final de este tutorial encontrará claves fundamentales para un procedimiento correcto \*\*\***

![Abrir &quot;Maestros&quot; &amp;gt; abrir &quot;Tarifa de art&#xED;culos&quot;](../../.gitbook/assets/image%20%28267%29.png)

![Pulsar en F4 o en el bot&#xF3;n &quot;F4 Importador&quot;](../../.gitbook/assets/image%20%28325%29.png)

![En la nueva pesta&#xF1;a pulsar en F1 o bot&#xF3;n &quot;F1 Nuevo&quot;](../../.gitbook/assets/image%20%28294%29.png)

![](../../.gitbook/assets/image%20%28103%29.png)

Le damos un nombre al importador \(recomendamos relacionarlo con la marca de la tarifa\), seleccionamos el proveedor de la marca, la marca y si se va a importar la tarifa de una familia concreta \(recordamos que de una misma marca se pueden crear varios importadores por si envían las tarifas diferenciadas por familias por ejemplo\).

**Tenemos 2 tipos de ficheros posibles a importar:**

**1.- Excel \(Columna Origen Excel: A - enumerar columnas por letras\)**

**2.- TXT \(Columna Origen TXT: 0 - enumerar columnas por números\)**

**Ejemplo con archivo Excel**

![ARCHIVOS EXCEL: COLUMNA ORIGEN A \(ENUMERAR COLUMNAS CON LETRAS\)](../../.gitbook/assets/image%20%28192%29.png)

![ARCHIVOS TXT: COLUMNA ORIGEN 0 \(ENUMERAR COLUMNAS CON N&#xDA;MEROS\)](../../.gitbook/assets/image%20%28342%29.png)

![Tarifa sin modificar](../../.gitbook/assets/image%20%2843%29.png)

**En el archivo de la tarifa, debemos eliminar logos y las líneas superiores, dejando como primera filas los títulos de las columnas \(referencia, artículo, precio, descuento, etc...\), a fin de que quede como la siguiente imagen:**

![Tarifa modificada](../../.gitbook/assets/image%20%28517%29.png)

En la pestaña "Líneas", pulsamos doble clic o botón derecho "Alta de línea" y procedemos a añadir las columnas que deseamos importar de la tarifa. **En este caso vamos a NO IMPORTAR la columna D que son los precios sin IVA por lo que añadiremos 4 altas de línea relacionadas con cada campo a importar \(referencia, nombre, tipo de artículo y precio de venta\)**

![Una vez rellenos los datos, preparado el archivo de la tarifa seg&#xFA;n las instrucciones y a&#xF1;adidas las l&#xED;neas, pulsamos en el bot&#xF3;n &quot;IMPORTAR&quot;](../../.gitbook/assets/image%20%28276%29.png)

![](../../.gitbook/assets/image%20%28150%29.png)

En la ventana emergente de la imagen seleccionamos el archivo Excel modificado, verificamos las columnas \(pondrá el total de columnas, pero no importará las que no tengan línea en el importador\) **y en la última fila, que está señalado con un círculo rojo, a modo de prueba del importador, sustituimos la cifra por 12 como testeo breve. Quedaría de este modo:**

![](../../.gitbook/assets/image%20%28159%29.png)

**En hoja: poner exactamente lo que ponga \(copiar / pegar\)**

**Todo relleno, pulsamos en aceptar y esperamos al mensaje de finalización de importación**

![](../../.gitbook/assets/image%20%28185%29.png)

Si tras comprobar los artículos importados, todo queda perfecto, repetir el paso del botón "IMPORTAR" cambiando la última fila 12 por la última fila que contenga datos que deseemos importar \(podemos realizar la importación por partes, familias, etc...usando varios importadores y misma tarifa\).

**El proceso de importación se puede repetir todas las veces que queramos, no se duplica nada. El proceso actualiza artículos existentes y añade elementos de la tarifa de artículos nuevos.**

**\*\*\* MUY IMPORTANTE: Recomendamos añadir a la pestaña "Observaciones", dentro del importador, todo lo modificado en el archivo Excel o texto de la tarifa a importar para que quede constancia del procedimiento, así cualquier usuario podrá actualizarla sin ningún inconveniente.**

