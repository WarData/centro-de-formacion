# Generación de "Pedidos Únicos"

Para la gestión de pedidos de campaña o de cualquier otro tipo de pedido se nos puede dar el caso de necesitar que al confirmar un pedido de ventas las unidades que se tengan que pedir a proveedor no se añadan en ningún caso a un pedido de compras ya existente sino que generen siempre un nuevo pedido de compras.

Hemos creado para esto un check en las series de pedidos de ventas:

<figure><img src="../../.gitbook/assets/imagen (214).png" alt=""><figcaption></figcaption></figure>

Un pedido de cliente creado en una serie de este tipo, en caso de necesitar pedir a proveedor no añadirá nunca sus líneas a un pedido de compras ya existente, creará siempre un nuevo pedido de compras.

\
