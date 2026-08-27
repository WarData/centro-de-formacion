# Utilidades en la comunicación WMT-Prestashop (Artículos)

## Artículos

**Nota importate:** en caso de dudas acerca de los estados de sincronización es conveniente comprobar el listado "Estados de la sincronización" o "Estados de la sincronización (stock)"

<figure><img src="../../../../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

En la ficha de un artículo podremos saber el ID del producto en la web, saber si hay algún error en la verificación/alta **(Estado sincronización)** o saber si la sincronización de stock se ha podido realizar de forma satisfactoria **(Estados sincronización Stock)**.

En caso de que el artículo sea una combinación (hijo) en "ID Web" podremos saber el código del producto padre y el código del producto hijo. Ejemplo: 1032 - 1033.

<figure><img src="../../../../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

## Opciones

#### ¿Existe ya en la web?

Comprobación de la existencia y comparativa del artículo entre web y WMT. Utilizable desde el alta manual desde la ficha de un artículo y desde el alta en tanda desde un listado de artículos.

El botón en el artículo es:

<figure><img src="../../../../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

En el listado (En esta opción se puede ejecutar sobre artículos con incidencias o que ya están enlazados para verificar su estado. Si su estado es otro habrá que ver el problema concreto (error comunicación, incidencia extraña, etc.):

<figure><img src="../../../../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

#### Familia (Categorías):

* Solamente comprobaremos si existe la familia en la web en base al código que guardemos en la ficha de la familia. El dato se guarda en el campo Código en Web de la ficha de la familia:

<figure><img src="../../../../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

* En caso de venir SIN familia el artículo no especificaremos nada
* En caso de venir tener familia pero NO tener código que lo relaciona con la categoría de la web se tratará de buscar si se le puede aplicar el código en base al nombre
* NO crearemos nuevas familias al necesitarse esquemas muy concretos de herencias (será un trabajo MANUAL y que habrá que casar entre categorías de la web y familias del programa). Recordar que si no se han enlazado previamente es porque no coinciden en nombre o hay categorías en la web que repiten el MISMO nombre.

En marcas el control funciona de la misma forma y el código de la marca en la web está en la ficha del formulario de las Marcas.

<figure><img src="../../../../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>



#### Alta de artículos

**Desde ficha de artículo:** Esta opción permite dar de alta en la web el artículo seleccionado. En primer lugar, se comprobará si el artículo ya existe en la web. Si no existe, se realizará el alta y se guardará en Winmotor el código del producto asignado en la web. De esta forma, el artículo quedará enlazado y se podrá controlar posteriormente la actualización de su stock en la web.

<figure><img src="../../../../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

Para poder realizar el alta, el artículo debe encontrarse en estado **"No sincronizado"** o **"Pendiente de crearse"**.

Una vez realizado el enlace, también se actualizará el stock del artículo en la web.



**Desde listado de artículos (Maestros > Artículos):** También se podrá realizar el alta de artículos de forma masiva desde la rejilla de artículos. Los artículos seleccionados se crearán en la web siempre que no existan previamente y su estado permita realizar el alta, es decir, que se encuentren en estado **"No sincronizado"** o **"Pendiente de crearse"**.

<figure><img src="../../../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>



#### Actualizar stock de artículos

El funcionamiento es similar al proceso de alta de artículos. La actualización de stock se podrá realizar tanto desde la ficha de un artículo como desde el listado de artículos.

<figure><img src="../../../../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

Para poder actualizar el stock de uno o varios artículos en la web, estos deben estar **enlazados**. Esto significa que el estado de sincronización del artículo en Winmotor debe ser **"Enlazado"**.



#### Información extra

**Comprobación de estado de artículos:** Es posible comprobar el estado de sincronización de un artículo y contrastarlo con su situación real en la web desde el listado de artículos **(Maestros > Artículos)**. Para ello, desde la rejilla de artículos, acceder a **Opciones > Lista > Generar vista con otro visor** y seleccionar la rejilla **"Artículos (Web - Prestashop)"**. Esta vista permitirá consultar la información necesaria para comprobar la situación de los artículos y su sincronización con la web en caso de duda.

<figure><img src="../../../../../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

**Presentar en web:** Los productos solamente se enviarán a la web siempre y cuando estén marcados de esa forma en Winmotor. La opción está dentro de los artículos > Pestaña Web > Presentar en Web.

**Imágenes:** Si el artículo tiene imagen asociada también se dará de alta en la web. La imagen que se sube a la web será la imagen localizada dentro del artículo > Web > Imagen (Imagen ampliada). Solamente se subirá una sola y en caso de querer poner habrá que hacerlo desde la propia web.
