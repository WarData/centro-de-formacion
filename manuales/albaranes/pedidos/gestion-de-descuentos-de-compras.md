# Gestión de descuentos y clasificación de compras

Dado que algunas marcas imponen que, según el artículo que se inserte en un pedido de compras, este será urgente o de reposición, hemos montado un nuevo sistema de gestión de descuentos de compras para automatizar esta división al generar pedidos de compras desde pedidos de ventas y órdenes de reparación.&#x20;

Esto implica que cada artículo en su tarifa de compra tendrá un código específico de clasificador de descuento de compra y que éste código implica un tipo de pedido (urgente, reposición, garantía).&#x20;

<mark style="color:orange;">**Uso del sistema:**</mark>&#x20;

●     Definir el tipo de pedido de compra por cada clasificador de descuento en las condiciones de compras del proveedor (pestaña “Comerciales” en la ficha del proveedor)

<figure><img src="../../../.gitbook/assets/imagen (9) (1).png" alt=""><figcaption></figcaption></figure>

* La última es una nueva columna “Forzar a descuento” que admite los valores “Urgente”, “Reposición” o “Garantía”.
  * Rellenar este campo con uno de estos valores implica que el programa forzará a ese tipo de pedido a proveedor cualquier artículo que utilice el clasificador de descuento definido en la línea.
  * La única excepción a esta regla son las líneas de órdenes de reparación que se definen en garantía: en este caso es mandatorio el tipo de línea (garantía) y se ignora por lo tanto el tipo de pedido definido en esta tabla.

●     Por cada artículo hay que definir en su tarifa de compras principal el clasificador de descuento que nos aporte el proveedor. Verás que al definir el clasificador el programa calculará automáticamente el tipo de pedido de compras según lo definido en la tabla de descuentos del proveedor y el porcentaje de descuento en caso de haberlo definido también:

<figure><img src="../../../.gitbook/assets/imagen (1) (2).png" alt=""><figcaption></figcaption></figure>

A partir de este momento verás que si grabas una línea de pedido de cliente con un artículo en el que hayas definido el clasificador descuento el programa calcula y rellena un nuevo campo en la línea del pedido de ventas: “Tipo de pedido compra”. Lo mismo pasa si lo haces desde una orden de reparación.&#x20;

<mark style="color:orange;">**Series de de pedidos de ventas y de órdenes de reparación**</mark>&#x20;

<figure><img src="../../../.gitbook/assets/imagen (1) (7).png" alt=""><figcaption></figcaption></figure>

El programa permite ahora definir una serie de pedido de compras “destino” por cada tipo de pedido que estamos definiendo en las líneas de pedidos de ventas y órdenes de reparación; es decir, desde un pedido de ventas u orden de reparación podríamos si se diera el caso, crear tres pedidos de compras según los artículos que se incluyan en el documento.

Damos ahora, por lo tanto, la posibilidad de definir por cada serie de pedido de clientes tres distintas series de pedido de compras destino según el tipo de pedido calculado por cada línea. Lo mismo pasa con las órdenes de reparación.&#x20;

En caso de que el artículo no tenga definido ningún clasificador de descuento y por lo tanto no haya tipo pedido de compras enlazado, el programa tomará como serie la definida para “Reposición”.&#x20;

Se considera por lo tanto que hay cuatro tipos de pedidos de compras que son: urgente, reposición, garantía y SIN TIPO
