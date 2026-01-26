# Cómo importar una Tarifa desde el Importador de la Marca

**Una vez hayamos creado o tengamos creado desde inicio un importador de una marca según el enlace en el pie de página (izquierda), ya sólo nos queda adaptar el archivo de la tarifa e importarlo según las siguientes instrucciones.**

<mark style="color:red;">**MUY IMPORTANTE: En el importador de la marca, en el campo "Nombre de hoja", hay que indicar el nombre de la hoja de Excel. Si es muy grande o tiene algún carácter especial, sustituir por un nombre más sencillo:**</mark>

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

<mark style="color:red;">**En Excel:**</mark>

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

**\*\*\* Si ha seguido los pasos de "Crear un Importador de Tarifa de Marca" habrá introducido en observaciones qué ha modificado en el archivo Excel o Texto de la tarifa. En caso de que no lo tenga incluido, recomendamos incorporar las modificaciones y características de importación de la tarifa (columnas, qué se elimina, etc...) para poder importarla dentro del importador, en la pestaña "Observaciones".**

**\*\*\*Al final de este tutorial encontrará claves fundamentales para un procedimiento correcto\*\*\***

**IMPORTANTE CAMPO FAMILIA > Para usar y/o crear una familia existente o no en Winmotor, es imprescindible añadir al nombre de la familia una A delante. Por ejemplo, familia CASCOS tendría en el archivo que llamarse ACASCOS al usarse la línea del importador "Familia".**

**Si la familia se añade en la cabecera del importador, no se debe añadir también como línea.**

**\*\*\* Para importar archivos Excel es necesaria la instalación del siguiente componente redistribuible del motor de base de datos de Microsoft Access 2016:**

[**https://www.microsoft.com/en-us/download/details.aspx?id=54920**](https://www.microsoft.com/en-us/download/details.aspx?id=54920) **(descargar y ejecutar versión x64)**

**Tenemos 2 tipos de ficheros posibles a importar:**

**1.- Excel (Columna Origen Excel: A - enumerar columnas por letras)**

**2.- TXT (Columna Origen TXT: 0 - enumerar columnas por números)**

**Ejemplo con archivo Excel**

![ARCHIVOS EXCEL: COLUMNA ORIGEN A (ENUMERAR COLUMNAS CON LETRAS)](<../../../.gitbook/assets/image (86).png>)

![ARCHIVOS TXT: COLUMNA ORIGEN 0 (ENUMERAR COLUMNAS CON NÚMEROS)](<../../../.gitbook/assets/image (87).png>)

![Tarifa sin modificar](<../../../.gitbook/assets/image (88).png>)

**En el archivo de la tarifa, debemos eliminar logos y las líneas superiores, dejando como primera filas los títulos de las columnas (referencia, artículo, precio, descuento, etc...), a fin de que quede como la siguiente imagen:**

![Tarifa modificada](<../../../.gitbook/assets/image (89).png>)

![](<../../../.gitbook/assets/image (90).png>)

En la pestaña "Líneas", pulsamos doble clic o botón derecho "Alta de línea" y procedemos a añadir las columnas que deseamos importar de la tarifa. **En este caso vamos a NO IMPORTAR la columna D que son los precios sin IVA por lo que añadiremos 4 altas de línea relacionadas con cada campo a importar (referencia, nombre, tipo de artículo y precio de venta)**

![Una vez rellenos los datos, preparado el archivo de la tarifa según las instrucciones y añadidas las líneas, pulsamos en el botón "IMPORTAR"](<../../../.gitbook/assets/image (91).png>)

![](<../../../.gitbook/assets/image (92).png>)

En la ventana emergente de la imagen seleccionamos el archivo Excel modificado, verificamos las columnas (pondrá el total de columnas, pero no importará las que no tengan línea en el importador) **y en la última fila, que está señalado con un círculo rojo, a modo de prueba del importador, sustituimos la cifra por 12 como testeo breve. Quedaría de este modo:**

![](<../../../.gitbook/assets/image (93).png>)

**En hoja: poner exactamente lo que ponga (copiar / pegar)**

**Todo relleno, pulsamos en aceptar y esperamos al mensaje de finalización de importación**

![](<../../../.gitbook/assets/image (94).png>)

Si tras comprobar los artículos importados, todo queda perfecto, repetir el paso del botón "IMPORTAR" cambiando la última fila 12 por la última fila que contenga datos que deseemos importar (podemos realizar la importación por partes, familias, etc...usando varios importadores y misma tarifa).

\*\*El proceso de importación se puede repetir todas las veces que queramos, no se duplica nada. \*\*

**Tras finalizar el proceso, hay que actualizar los artículos existentes con los elementos de la tarifa de artículos nuevos desde la opción "Tarifa de Artículos" > botón "Actualizar Artículos"**

**\*\*\* MUY IMPORTANTE: Recomendamos añadir a la pestaña "Observaciones", dentro del importador, todo lo modificado en el archivo Excel o texto de la tarifa a importar para que quede constancia del procedimiento, así cualquier usuario podrá actualizarla sin ningún inconveniente.**[<br>](https://winmotor.gitbook.io/project/~/drafts/-LUFfE7ntUBm_NjWthNB/primary/faq/es-posible-borrar-cualquier-factura-1)
