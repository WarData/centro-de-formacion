# Inventarios

Vamos a ver el proceso para crear un inventario en un [almacén](../../manuales/almacenes/) de la empresa (recomendamos realizar este modo con todo el stock de la empresa, tanto disponible como reservado a fin de realizar una regularización perfecta). Es posible regular la cantidad de artículos en stock y también regular el PMC (precio medio de compra).

<mark style="color:yellow;">**Métodos para Inventariar**</mark>

Existen tres métodos principales para llevar a cabo un inventario:

1. **Inventario mediante parte de almacén: Menú Almacenes > opción Partes de Almacén > Inventario (explicado tras inventario por listado de stock por almacén)**
2. **Inventario mediante archivo**: mediante importación de archivo txt

Podemos incorporar el inventario directamente incluyendo artículos a las líneas del parte de Winmotor o importando un archivo de texto (.txt) en el botón indicado de la siguiente imagen. **El archivo puede incluir el almacén o la ubicación de cada artículo inventariado para facilitar el mismo.** El formato del archivo de texto será: referencia,unidades (ejemplo > BS10265,25):

![](<../../.gitbook/assets/image (134).png>)

3. **Inventario mediante listado de stock por almacén:**

En panel de artículos > botón "Listados" > seleccionar Stock por almacén e introducir almacén a inventariar y todos los artículos (es importante porque saldrán artículos sin stock que puede que sí tengan stock realmente):

<figure><img src="../../.gitbook/assets/imagen (1).png" alt=""><figcaption></figcaption></figure>

Generará un listado con todos los artículos, seleccionamos todos pulsando en la casilla superior izquierda y pulsamos en "Generación de inventario":

<figure><img src="../../.gitbook/assets/imagen (2).png" alt=""><figcaption></figcaption></figure>

Saldrá este mensaje y hay que desmarcar no mostrar sin stock para que sí lo haga:

<figure><img src="../../.gitbook/assets/imagen (3).png" alt=""><figcaption></figcaption></figure>

Ahora podremos trabajar sobre un inventario existente, corrigiendo las cantidades indicadas:

<figure><img src="../../.gitbook/assets/imagen (4).png" alt=""><figcaption></figcaption></figure>

¿Qué es un inventario?

**El inventario es una relación detallada, ordenada y valorada de los productos que tiene una empresa en stock.‌**

**¿Qué sucede en cada artículo cuando se incluye en un inventario?‌**

**\* Un inventario, reseteará el stock de un producto en un almacén concreto desde la fecha/hora marcada.**

\*\* **Si tras confirmar el inventario, pulsamos en la opción "Inicializar inventario",** todas las referencias **NO INCLUIDAS en el parte de almacén de tipo "Inventario" y que tienen como ubicación de almacenaje el almacén indicado en el parte, SE PONDRÁN A CERO STOCK.**

**\*\*\* Si durante el inventario se localiza el mismo artículo en líneas distintas la aplicación Winmotor las fusionará en el momento que pulsemos el botón "Cerrar" tras confirmar el inventario (al confirmar aparece la opción "Inicializar"). La opción cerrar es reversible, abriendo el inventario (las unidades fusionadas quedan fusionadas siempre que sea el mismo almacén o sub-almacén, no se fusionan mismas referencias en ubicaciones distintas).**

Por tanto, el stock de un artículo / almacén siempre será el resultado de las compras + entradas de almacén, menos las ventas + salidas de almacén en orden cronológico. Pero cuando hay un inventario, desde esa fecha/hora se impondrá como stock lo definido en ese inventario.‌

**FAQ:** ¿si incluyo por ejemplo un documento de compra con fecha anterior al inventario, las unidades se suman al stock total del artículo? No, siempre que la compra sea en el mismo almacén inventariado, puesto que el inventario resetea el stock desde su fecha / hora.



Dentro de almacenes > Partes de almacén > abrimos el panel de inventarios:

![](<../../.gitbook/assets/image (123).png>)

Una vez creamos un parte de almacén nuevo, para realizar un inventario simplemente seleccionamos dicha opción, elegimos almacén a inventariar (volvemos a recomendar el almacén global para inventarios) y comenzamos a añadir artículos:

![](<../../.gitbook/assets/image (132).png>)

Todas las líneas tienen el mismo stock que el inventario salvo la última línea, a la que hemos añadido un artículo. Al introducir la referencia y tabular, el programa nos indica las ubicaciones del artículo dentro del almacén principal si hay más de una o pone directamente la única disponible y las unidades en stock. Si hay diferencia, únicamente tendremos que indicar el total resultante del inventario.

Pulsamos en "Confirmar" y regularizamos el inventario:

![](<../../.gitbook/assets/image (133).png>)

Como vemos en la imagen superior, el artículo del que inicialmente no teníamos stock, tras el inventario tenemos la unidad incluida.

A la vez, en la misma imagen vemos que tras "Confirmar" el parte de almacén de tipo inventario, aparece **el botón "Inicializar artículos" cuya función es poner todas las referencias NO INCLUIDAS  y que tienen como ubicación de almacenaje el almacén indicado en el parte, A CERO STOCK.**

**Opción para regularizar el PMC:** simplemente hay que indicar la referencia y seleccionar el check "Regularización de precio medio del artículo" > si hay más de una ubicación del mismo artículo habrá que seleccionar sobre qué ubicación se realizará la regularización.

![](<../../.gitbook/assets/imagen (3) (1) (2).png>)
