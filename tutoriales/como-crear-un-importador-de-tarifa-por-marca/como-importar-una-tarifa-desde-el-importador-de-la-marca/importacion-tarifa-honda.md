# Importación Tarifa Honda

**1.- DIVIDIR ARCHIVO TARIFA EN TROZOS**

Una tarifa como la de Honda puede tener más de 150.000 referencias, por ello y para evitar que el proceso sea excesivamente largo y que se puedan provocar caídas del servicio vServer o problemas en la Base de Datos, es imprescindible cortar y pegar unas 25000 – 26000 referencias desde el archivo txt original a unos nuevos a los que hemos llamado Tarifa Honda fecha – 1, 2, 3…así sucesivamente hasta el 6:

![](<../../../.gitbook/assets/imagen (109).png>)&#x20;

En el editor de textos de Windows, para elegir la línea correcta sólo debemos colocar el puntero y seleccionar donde indica la flecha roja, de esta manera sabremos qué línea es:

![](<../../../.gitbook/assets/imagen (108).png>)

En la imagen anterior se indica la línea 1 y debemos buscar, aproximadamente el total de líneas del archivo y dividirlo entre 6 trozos o más si lo estimáis oportuno:&#x20;

![](<../../../.gitbook/assets/imagen (112).png>)&#x20;

Hemos buscado la cifra aproximada y ahora tenemos que CORTAR (NO COPIAR) el texto de ahí al principio (hacia arriba) usando el botón derecho una vez seleccionada esa primera parte:

![](<../../../.gitbook/assets/imagen (107).png>)&#x20;

Quedarían seleccionadas de esta forma las líneas y pulsando el botón derecho saldría el menú donde pulsamos en “Cortar”:

****![](<../../../.gitbook/assets/imagen (104).png>)** **

Justo después de cortar, vamos al archivo vacío que creamos al principio y marcado como 1 y pegamos el contenido dentro de la misma forma, usando botón derecho y “Pegar”:

** **![](<../../../.gitbook/assets/imagen (106).png>)****

Se guarda el archivo y de nuevo se vuelve al archivo principal y se repite el proceso hasta que quede vacío y los 6 archivos con unas 26.000 líneas aproximadamente:

** **![](<../../../.gitbook/assets/imagen (114).png>)****

Podemos observar en la lista que el primero queda vacío y los 6 archivos quedan con un tamaño similar.** **

**2.- IMPORTAR ARCHIVOS TXT POR TROZOS**

Una vez dividida la tarifa vamos al menú MAESTROS > opción Tarifa de artículos > botón Importador (lateral izquierdo). Se nos abre el importador y hacemos doble clic en el “Importador Honda”. Aquí sólo hay que pulsar en el botón de la parte inferior “Importar” (no tocar ninguno de los campos creados en el importador):

![](<../../../.gitbook/assets/imagen (110).png>)

![](<../../../.gitbook/assets/imagen (115).png>)

Seleccionamos el archivo 1 y esperamos (el proceso deja la sesión de Winmotor actual sin uso y si se trata de comprobar indica que el proceso está tardando y pregunta si el usuario quiere reiniciar > DEJAR QUE TERMINE EL PROCESO, aunque esté “pensando”)&#x20;

Cada fichero, teniendo en cuenta el número de líneas indicado, tarda unos 8 minutos en actualizarse.&#x20;

Aparecerá esta ventana emergente cuando el proceso haya terminado correctamente:

** **![](<../../../.gitbook/assets/imagen (105).png>)****

Pulsamos en salir y ejecutamos el mismo proceso para los 5 archivos restantes quedando la tarifa importada (aún no actualizada OJO).** **

**3.- ACTUALIZAR ARTÍCULOS (CENTRAL Y CENTROS)**

Este proceso se realiza desde el menú de Tarifas de artículos > botón Actualizar artículos:

![](<../../../.gitbook/assets/imagen (113).png>)

Aparecerá una nueva ventana donde tendremos que indicar únicamente:

**1.- Proveedor**

**2.- Marca**

**3.- Actualizar**

**En caso de tener una empresa MULTI-CENTRO, en un segundo paso tenemos que realizar los mismos pasos, pero seleccionando los centros en los que aplicar la tarifa si fuera necesario (pulsamos la tecla “Ctrl” y vamos seleccionando cada uno de los centros hasta que queden marcados y pulsamos en Actualizar)**

**4.- FIN DEL PROCESO DE IMPORTACIÓN Y ACTUALIZACIÓN DE ARTÍCULOS**

** **

** **

** **
