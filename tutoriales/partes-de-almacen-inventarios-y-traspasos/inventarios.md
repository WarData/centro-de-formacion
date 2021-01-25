# Inventarios

Vamos a ver el proceso para crear un inventario en un [almacén](../../manuales/almacenes/) de la empresa \(recomendamos realizar este modo con todo el stock de la empresa, tanto disponible como reservado a fin de realizar una regularización perfecta\). Es posible regular la cantidad de artículos en stock y también regular el PMC \(precio medio de compra\).

**¿Qué es un inventario?**

**El inventario es una relación detallada, ordenada y valorada de los productos que tiene una la empresa en stock.‌**

**¿Qué sucede en cada artículo cuando se incluye en un inventario?‌**

**Un inventario, reseteará el stock de un producto en un almacén concreto desde la fecha/hora marcada.**‌

Por tanto, el stock de un artículo / almacén siempre será el resultado de las compras+entradas de almacén, menos las ventas+salidas de almacén en orden cronológico. Pero cuando hay un inventario, desde esa fecha/hora se impondrá como stock lo definido en ese inventario.‌

**FAQ:** ¿si incluyo por ejemplo un documento de compra con fecha anterior al inventario, las unidades se suman al stock total del artículo? No, siempre que la compra sea en el mismo almacén inventariado, puesto que el inventario resetea el stock desde su fecha/hora.

Podemos incorporar el inventario directamente incluyendo artículos a las líneas del parte de Winmotor o importando un archivo de texto \(.txt\) en el botón indicado de la siguiente imagen. **El archivo puede incluir el almacén o la ubicación de cada artículo inventariado para facilitar el mismo.** El formato del archivo de texto será: referencia,unidades \(ejemplo &gt; BS10265,25\):

![](../../.gitbook/assets/image%20%28280%29.png)

Dentro de almacenes &gt; Partes de almacén &gt; abrimos el panel de inventarios:

![](../../.gitbook/assets/image%20%2817%29.png)

Una vez creamos un parte de almacén nuevo, para realizar un inventario simplemente seleccionamos dicha opción, elegimos almacén a inventariar \(volvemos a recomendar el almacén global para inventarios\) y comenzamos a añadir artículos:

![](../../.gitbook/assets/image%20%28341%29%20%282%29.png)

Todas las líneas tienen el mismo stock que el inventario salvo la última línea, a la que hemos añadido un artículo. Al introducir la referencia y tabular, el programa nos indica las ubicaciones del artículo dentro del almacén principal si hay más de una o pone directamente la única disponible y las unidades en stock. Si hay diferencia, únicamente tendremos que indicar el total resultante del inventario.

Pulsamos en "Confirmar" y regularizamos el inventario:

![](../../.gitbook/assets/image%20%28204%29%20%281%29.png)

Como vemos en la imagen superior, el artículo del que inicialmente no teníamos stock, tras el inventario tenemos la unidad incluida.

Para regular el PMC simplemente hay que indicar la referencia y seleccionar el check "Regularización de precio medio del artículo" &gt; si hay más de una ubicación del mismo artículo habrá que seleccionar sobre qué ubicación se realizará la regularización.

![](../../.gitbook/assets/imagen.png)

