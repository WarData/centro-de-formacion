# Modelos

Esta opción permite dar de alta y gestionar las estructuras de modelo para operaciones comerciales. Dicha estructura se basa en:

* Marca
* Gama
* Versión - Serie
* Modelo
* Modelo - Color

Dada la estructura mostramos el sistema arbolado por el cual se presenta los modelos dados de alta y los bastidores que corresponden al modelo - color:

<figure><img src="../../../.gitbook/assets/imagen (1) (1).png" alt=""><figcaption></figcaption></figure>

<mark style="color:yellow;">**BOTONERA SUPERIOR**</mark>

<figure><img src="../../../.gitbook/assets/imagen (8) (1).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Actualizar</mark>: refresca la vista arbolada tras actualizar o dar de alta algún modelo
* <mark style="color:blue;">F1 - Nuevo Modelo</mark>: permite dar de alta cada una de las partes de la estructura que constituye un modelo. Para ello muestra un formulario donde existe la posibilidad de seleccionar partes del modelo ya dadas de alta. En caso de que el localizador de la marca, gama o versión no contenga datos, no tendrá tampoco datos ninguno de los elementos posteriores, teniéndolo que dar de alta.

<mark style="color:orange;">Ejemplo de alta de un modelo con marca existente, pero sin gama ni versión:</mark>

1.- Seleccionar la marca del listado del desplegable (si no existe requiere darla de alta - [véase "Marcas")](../../maestros/marcas.md):

<figure><img src="../../../.gitbook/assets/imagen (2) (1) (2).png" alt=""><figcaption></figcaption></figure>

2.- Aunque exista alguna gama en la marca TEST, vamos a crear una nueva:

<figure><img src="../../../.gitbook/assets/imagen (9) (6).png" alt=""><figcaption></figcaption></figure>

* En el formulario de alta, localizamos la marca para asociarla con la nueva gama y ponemos el código y nombre, en este caso pondremos 400 en ambos y dejaremos el blanco el código del fabricante en caso de que éste no nos lo proporcione <mark style="color:yellow;">**(recomendamos que los códigos y referencias sean cortos y concisos para facilitar que todos los usuarios los entiendan y se use un mismo sistema de introducción de datos):**</mark>

<figure><img src="../../../.gitbook/assets/imagen (14) (6).png" alt=""><figcaption></figcaption></figure>

* Al dar de alta la nueva gama, se verá reflejada automáticamente en el formulario de alta:

<figure><img src="../../../.gitbook/assets/imagen (5) (9).png" alt=""><figcaption></figcaption></figure>

3.- Daremos de alta la versión del mismo modo y usando un formulario específico:

<figure><img src="../../../.gitbook/assets/imagen (6).png" alt=""><figcaption></figcaption></figure>

<mark style="color:yellow;">**Es fundamental seguir estos pasos detenidamente para la correcta alta del modelo completo**</mark>

* En el formulario de alta, localizamos la gama dada de alta en el paso anterior para asociarla con la nueva versión, posteriormente pondremos el código y nombre, en este caso CY y CYBER en código y nombre respectivamente y dejaremos el blanco el código del fabricante en caso de que no nos lo proporcione <mark style="color:red;">**(IMPORTANTE: sobre la versión, no sobre el modelo)**</mark>

<figure><img src="../../../.gitbook/assets/imagen (3) (4) (3).png" alt=""><figcaption></figcaption></figure>

* En la versión disponemos de un campo "Serie" referente a una estructura solicitada por algunas marcas. Además de poder dar de alta las series que queramos, existen unas series por defecto por lo que sólo habría que seleccionar la correcta si existe:

<figure><img src="../../../.gitbook/assets/imagen (13) (1).png" alt=""><figcaption></figcaption></figure>

* El formulario de alta de la versión quedaría así:

<figure><img src="../../../.gitbook/assets/imagen (4) (3).png" alt=""><figcaption></figcaption></figure>

4.- Por último habría que rellenar el resto del formulario de alta del modelo empezando por <mark style="color:red;">**código de modelo y referencia del fabricante que, en caso de que éste no los aporte, tendremos que crear un código de modelo y ponerlo idéntico en la referencia del fabricante. Recomendamos el uso de la estructura Marca - Gama - Versión (MGV) para ello.**</mark>&#x20;

En este ejemplo, el vehículo dado de alta sería TEST 400 CYBER cogiendo MARCA - GAMA - VERSIÓN y su <mark style="color:yellow;">**código de modelo y referencia dadas de alta por nosotros sería**</mark>** **<mark style="color:orange;">**T400CYE7**</mark>

A veces el modelo además tiene algún dato que podremos añadir al final como por ejemplo EURO 7, haciendo este modelo dependiente de una misma MARCA, GAMA y VERSIÓN, pudiendo crear nuevos modelos que dichas partes de la estructura ya creadas añadiendo EURO 8 o 2023 o GTR, lo que formarían nuevos modelos.

Al ejemplo le añadimos EURO 7, <mark style="color:yellow;">**código y referencia T400CYE7**</mark>, año de fabricación 2023, precio de costo e impuesto de matriculación 1 (0%) y ya tenemos creado el <mark style="color:yellow;">**MODELO**</mark>, ahora falta añadirle color o colores para obtener el <mark style="color:yellow;">**MODELO - COLOR:**</mark>

<figure><img src="../../../.gitbook/assets/imagen (1) (2) (1).png" alt=""><figcaption></figcaption></figure>

5.- Actualizamos las estructuras arboladas y desplegamos la marca, gama y versión hasta visualizar el modelo y hacemos doble clic en él para acceder a la ficha:

<figure><img src="../../../.gitbook/assets/imagen (17) (1).png" alt=""><figcaption></figcaption></figure>

* Seleccionamos la pestaña "Colores" y pulsamos en "Crear color" seleccionando uno de los existentes o dando de alta uno nuevo (los colores pueden tener sobreprecio al modelo y colores básicos, es decir, colores metalizados o edición limitada pueden tener un precio superior editable en su ficha y en el alta del color):

<figure><img src="../../../.gitbook/assets/imagen (18) (1).png" alt=""><figcaption></figcaption></figure>

* Seleccionamos AD79 RED PLUS:

<figure><img src="../../../.gitbook/assets/imagen (15).png" alt=""><figcaption></figcaption></figure>

* Al aceptar nos aparece el modelo - color en la ficha (no es necesario desbloquear la ficha y aceptar, es posible el alta del color y modelo - color con la ficha bloqueada y pulsando en cancelar, esa parte quedará guardada.

6.- Al actualizar la estructura de modelos podremos desplegar marca, gama, versión y modelo hasta obtener el modelo - color que se podrá introducir en operaciones comerciales:

<figure><img src="../../../.gitbook/assets/imagen (173).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">F2 - Buscar modelo</mark>: muestra un localizador mediante varios índices de búsqueda como trozos de palabras y referencia de fabricante y modelos / colores, modelos y colores por separado. Es similar al localizador de modelos usado en albaranes de compras de vehículos y operaciones:

<figure><img src="../../../.gitbook/assets/imagen (5) (1).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">F3 - Listados</mark>: presenta varias opciones sobre los listados a mostrar:

<figure><img src="../../../.gitbook/assets/imagen (19).png" alt=""><figcaption></figcaption></figure>

Ejemplo de series mostrado en panel similar a modelos:

<figure><img src="../../../.gitbook/assets/imagen (3) (2).png" alt=""><figcaption></figcaption></figure>

Ejemplo de listado de colores:

<figure><img src="../../../.gitbook/assets/imagen (29).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">F4 - Modelos de taller</mark>: permite el alta y consulta de modelos creados para taller
* <mark style="color:blue;">F6 - Opciones</mark>: presenta opciones para importar modelos, actualizar precios y revisión de modelos:

<figure><img src="../../../.gitbook/assets/imagen (13).png" alt=""><figcaption></figcaption></figure>

1.- Importar modelos de vehículos

<figure><img src="../../../.gitbook/assets/imagen (23).png" alt=""><figcaption></figcaption></figure>

2.- Actualizar precios modelos

<figure><img src="../../../.gitbook/assets/imagen (21).png" alt=""><figcaption></figcaption></figure>

3.- Revisión de modelos

Presenta un panel para control y revisión de modelos creados o alta de gamas, versiones:

<figure><img src="../../../.gitbook/assets/imagen (4) (2).png" alt=""><figcaption></figcaption></figure>
