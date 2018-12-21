# Cómo crear un Importador de Tarifa por Marca

En éste tutorial vamos a crear un importador para una marca en particular.

 De ésta forma habrá uno o varios importadores almacenados para las marcas que la empresa gestione y posteriormente ir actualizando las nuevas tarifas con sólo pulsar un botón y modificar el archivo para adecuarlo al importador creado.

* ![](https://www.winmotor.net/wp-content/uploads/2018/11/Tarifa-artículos-1-1024x576.jpg) Abrir "Maestros" &gt; abrir "Tarifa de artículos"

![](https://www.winmotor.net/wp-content/uploads/2018/11/F4_Importador-1024x576.jpg)Pulsar en F4 o en el botón "F4 Importador"![](https://www.winmotor.net/wp-content/uploads/2018/11/F1_Nuevo-importador-1024x576.jpg)En la nueva pestaña pulsar en F1 o botón "F1 Nuevo"![](https://www.winmotor.net/wp-content/uploads/2018/11/Rellenar-datos-1024x576.jpg)

Le damos un nombre al importador \(recomendamos relacionarlo con la marca de la tarifa\), seleccionamos el proveedor de la marca, la marca y si se va a importar la tarifa de una familia concreta \(recordamos que de una misma marca se pueden crear varios importadores por si envían las tarifas diferenciadas por familias por ejemplo\).

**Tenemos 2 tipos de ficheros posibles a importar:**

**1.- Excel \(Columna Origen Excel: A - enumerar columnas por letras\)**

**2.- TXT \(Columna Origen TXT: 0 - enumerar columnas por números\)**

**Ejemplo con archivo Excel**

* ![](https://www.winmotor.net/wp-content/uploads/2018/11/Excel_A-1024x576.jpg)ARCHIVOS EXCEL: COLUMNA ORIGEN A \(ENUMERAR COLUMNAS CON LETRAS\)

![](https://www.winmotor.net/wp-content/uploads/2018/11/TXT_0-1024x576.jpg)ARCHIVOS TXT: COLUMNA ORIGEN 0 \(ENUMERAR COLUMNAS CON NÚMEROS\)

* ![](https://www.winmotor.net/wp-content/uploads/2018/11/Tarifa-sin-modificar-1-1024x576.jpg)Tarifa sin modificar

**En el archivo de la tarifa, debemos eliminar logos y las líneas superiores, dejando como primera filas los títulos de las columnas \(referencia, artículo, precio, descuento, etc...\), a fin de que quede como la siguiente imagen:**![](https://www.winmotor.net/wp-content/uploads/2018/11/Tarifa-modificada-1-1024x576.jpg)Tarifa modificada![](https://www.winmotor.net/wp-content/uploads/2018/11/Añadir-líneas-excluyendo-no-aparezcan-1024x576.jpg)

En la pestaña "Líneas", pulsamos doble clic o botón derecho "Alta de línea" y procedemos a añadir las columnas que deseamos importar de la tarifa. **En este caso vamos a NO IMPORTAR la columna D que son los precios sin IVA por lo que añadiremos 4 altas de línea relacionadas con cada campo a importar \(referencia, nombre, tipo de artículo y precio de venta\)**![](https://www.winmotor.net/wp-content/uploads/2018/11/Botón-Importar-1024x576.jpg)Una vez rellenos los datos, preparado el archivo de la tarifa según las instrucciones y añadidas las líneas, pulsamos en el botón "IMPORTAR"![](https://www.winmotor.net/wp-content/uploads/2018/11/Indicar-fin-saltos-intermedios-1024x576.jpg)

En la ventana emergente de la imagen seleccionamos el archivo Excel modificado, verificamos las columnas \(pondrá el total de columnas, pero no importará las que no tengan línea en el importador\) **y en la última fila, que está señalado con un círculo rojo, a modo de prueba del importador, sustituimos la cifra por 12 como testeo breve. Quedaría de este modo:**![](https://www.winmotor.net/wp-content/uploads/2018/11/Test-inicial-12-líneas-línea-1-y-poner-lo-que-ponga-en-la-hoja-1024x576.jpg)

**En hoja: poner exactamente lo que ponga \(copiar / pegar\)**

**Todo relleno, pulsamos en aceptar y esperamos al mensaje de finalización de importación**![](https://www.winmotor.net/wp-content/uploads/2018/11/Finalización-importación-volver-a-importar-con-el-total-1024x576.jpg)

Si tras comprobar los artículos importados, todo queda perfecto, repetir el paso del botón "IMPORTAR" cambiando la última fila 12 por la última fila que contenga datos que deseemos importar \(podemos realizar la importación por partes, familias, etc...usando varios importadores y misma tarifa\).

**El proceso de importación se puede repetir todas las veces que queramos, no se duplica nada. El proceso actualiza artículos existentes y añade elementos de la tarifa de artículos nuevos.**

