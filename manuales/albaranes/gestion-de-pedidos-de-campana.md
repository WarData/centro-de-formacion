# Gestión de Pedidos de Campaña

Se trata de la operativa en pedidos para gestionar campañas de proveedores. Consideramos una campaña cuando un proveedor nos propone la entrega en condiciones económicas especiales de una serie de productos pero a largo plazo.

La operativa especial consiste en que los pedidos de ventas de este tipo no se actualizan en el artículo como unidades pendientes de entregar a clientes, van directamente a pedidos a proveedor.

Los pedidos de compras tampoco afectan al artículo inicialmente: se crean con un campo especial “Vencimiento Campaña” que será la fecha en la que se libera el pedido para poder activarlo y que pase a funcionar como un pedido normal.

Para gestionar pedidos de Campaña hay que hacer lo siguiente:

* **Crear una serie de pedidos de compras marcando en el tipo de pedido de compra “Campaña”**

<figure><img src="../../.gitbook/assets/imagen (210).png" alt=""><figcaption></figcaption></figure>

* **Crear una serie de pedidos de ventas marcando la propiedad “Pedidos de campaña” y relacionándola con la serie de compras creada previamente**. Comprobarás que al definir que la serie es para “pedidos de campaña” el selector de serie de pedidos de compras destino cambia y presenta sólo una para definir la serie de “Campaña”:

<figure><img src="../../.gitbook/assets/imagen (211).png" alt=""><figcaption></figcaption></figure>

* **Definir en la ficha del proveedor - pestaña comercial el mes / día previsto de recepción** para los pedidos de campaña. El programa lo tomará como fecha inicial prevista de entrega para los pedidos de compras que se generen de ese proveedor.

<figure><img src="../../.gitbook/assets/imagen (212).png" alt=""><figcaption></figcaption></figure>

*   **Grabar el pedido de ventas en esta nueva serie para que sea un pedido de campaña.**&#x20;

    * Según tengas marcado en la serie de pedidos de ventas “Generar pedidos únicos” o no, el programa se añadirá a un pedido abierto de este proveedor o generará un nuevo pedido.
    * Este tipo de pedido no dejará ninguna huella en la ficha del artículo hasta que se reciba el pedido a proveedor, entonces aparecerán las unidades reflejadas en unidades reservadas de pedido.


* **Se habrá creado un pedido de compras del tipo “Campaña” con una fecha prevista de entrega** calculada a partir de los datos de la ficha del proveedor. Antes de confirmar el pedido puedes editar la fecha.
*   **Tramitar el pedido de compras**

    * En la ficha del artículo no se reflejará ninguna cantidad pendiente de recibir del proveedor relativa a este pedido y si ejecutas la opción de recepcionar pedidos tampoco aparecerán.
    * En el pedido no aparecerá el botón “Recepcionar”.


* **Activar el pedido:** supone la puesta en marcha del mismo y en principio estará activa la opción cuando hayamos llegado a la fecha prevista de entrega o la hayamos superado. Junto a la fecha prevista aparece un nuevo botón:

<figure><img src="../../.gitbook/assets/imagen (5) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

\*\*\* Si el usuario tiene permisos de modificación de pedidos de compras al pulsar el botón podrá:

* Modificar la fecha prevista de entrega

<figure><img src="../../.gitbook/assets/imagen (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

* Si la fecha de vencimiento es igual o superior a hoy aparecerá el botón de activación

<figure><img src="../../.gitbook/assets/imagen (3) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

* Al pulsar el botón de “Activar” el programa pedirá confirmación para liberar el pedido. Si se acepta pasará a funcionar como un pedido normal y automáticamente se reflejarán en los artículos incluidos las cantidades como pendientes de recibir y reservadas de pedido.
* Aparecerá también en el pedido el botón “Recepcionar”.
* En el panel de pedidos de compras, los pedidos de campaña aparecerán con un icono identificativo de un calendario a fin de indicar que está programado:

<figure><img src="../../.gitbook/assets/imagen (213).png" alt=""><figcaption></figcaption></figure>

\
