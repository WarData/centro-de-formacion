# Proceso General de Pedidos

**Operativa general de pedidos**

![](../../../.gitbook/assets/image%20%28175%29.png)

El diagrama refleja la siguiente operativa:

1.        Un cliente requiere un material. Esta necesidad puede nacer en un pedido de cliente o en una orden de reparación

2.        Al confirmar el documento \(pedido u orden de reparación\) la aplicación analiza la situación de stock de cada uno de los artículos incluidos y según haya o no stock disponible lo reservará o generará los correspondientes pedidos a proveedor.

          \* En caso de que haya stock disponible el documento generará una “reserva”, quiere decir, acumulará en el stock reservado del artículo la cantidad necesitada por el cliente.

          \* En caso de no haber stock disponible se entra en el proceso de generación de pedidos a proveedor que se ejecuta de la siguiente forma :

                       A.- No existen pedidos al proveedor del artículo : se crea un nuevo pedido y se añade la línea del artículo

                       B.- Existen pedidos al proveedor del artículo

           \* El pedido no está tramitado: se añade la línea del artículo, o si ya hay una línea con el mismo artículo se suma la cantidad pedida por el cliente a la pedida a proveedor.

           \* El pedido está tramitado

                        A.- Hay material pendiente de recibir no asignado a otros pedidos de clientes : se reserva de este material pendiente de recibir para el pedido de ventas

                        B.- No hay material pendiente de recibir no asignado a cliente: se ejecuta el primer paso, generación de un nuevo pedido al proveedor.

                        C.- Si hacemos en este momento doble click en la línea del pedido de ventas o la orden,  la aplicación nos muestra en la lista de seguimientos uno con la acción “Pedido a proveedor” donde podremos ver en qué pedido se ha tramitado la línea.

3.        Al recibir el pedido de proveedor se genera un albarán de entrada

4.        Cuando se crea un albarán de entrada con origen en un pedido el programa analiza las “asignaciones” del pedido: es decir, los pedidos de ventas u órdenes que originaron el pedido a proveedor. Esto quiere decir que automáticamente en el momento de crear el albarán de entrada se estarán modificando el estado de los pedidos u órdenes que solicitaron la mercancía, asignándola al documento y reservándola del stock creado para su entrega a esos clientes.

            \* Si hacemos en este momento doble click en las líneas de pedidos de ventas o de compras se visualizan en la lista de seguimientos estas “asignaciones”.

            \* Si teníamos un pedido de cliente pendiente de recibir material y en este momento hemos recibido todo lo pendiente el pedido pasará automáticamente de “Pendiente de recibir” a “Pendiente de entregar”. En el caso de las órdenes de reparación pasarán a estado “Pendiente de instalar”.

5.        Según sea el documento de ventas que originó el ciclo, en el caso de un pedido de cliente se podrá generar un albarán y en el caso de una orden de reparación podremos ejecutar la opción interna de “instalar”.

6.        En el caso de haber generado albaranes de ventas, en su momento éstos se convertirán en facturas. En el caso de las órdenes cuando estén completamente instaladas se podrán convertir en facturas.

**Operativa completa de compras**

![](../../../.gitbook/assets/image%20%2837%29.png)

El diagrama refleja la siguiente operativa:

1.        Partimos del pedido de compras ya creado. Este pedido se ha podido generar bien manualmente, bien desde pedidos de clientes u órdenes de reparación  o también desde una propuesta de pedidos. Se da por hecho que el pedido se ha tramitado con la fábrica.

2.         Al ejecutar el proceso de importación del Excel de la Pre-factura de fábrica el programa nos presenta en una lista en pantalla el material que nos confirman que van a entregar. En este documento la fábrica reseña  nuestros pedidos mediante una referencia que ellos asignan y que debemos dejar reflejada en dichos pedidos en el campo “Referencia”  de manera que al ejecutar el proceso la aplicación sepa relacionar cada línea del documento con nuestro pedido origen. Por otro lado en este proceso de importación se gestionan las “sustituciones” de artículos según las que se indiquen en el documento.

3.        La confirmación del proceso de importación supone la generación del embarque que a su vez va a marcar en cada línea de pedido la fecha prevista de recepción del material según la fecha indicada en el Excel de la pre-factura.

4.        Al recibir el material físicamente utilizaremos el proceso de piking de las PDA’S para hacer el recuento y confirmación de la entrada. En este proceso uno o varios usuarios utilizarán como documento de recepción **el embarque** de manera que el programa irá comparando lo pikado con las líneas del embarque. Se han montado nuevas pestañas de comprobación de estos datos tanto en los documentos que pueden originar un piking \(pedidos o embarques\) como en un nuevo panel general en el menú de compras donde se puede consultar las líneas leídas por cada usuario de las PDA’S. El proceso de finalización y confirmación de un piking se hará desde estas nuevas pestañas en los documentos, con el botón “Generar albarán”. Al ejecutar esta acción de creación del albarán el documento embarque quedará en situación cerrado y no se podrá manipular ni utilizar en otro proceso de piking. Se ha creado por otra parte una opción alternativa de creación directa del albarán de entrada desde el embarque sin pasar por el proceso de piking para el caso en el que se considere necesario.

5.        Como se explica en el punto 1 sobre la operativa general de pedidos la confirmación de este albarán de compras supone la “repartición” mediante asignaciones del material recibido. Si el pedido de compras que genera el ciclo del proceso ha quedado completamente recibido pasará automáticamente a estado “Recibido”.  
****

**Operativa de pedidos en distribución multicentro**

![](../../../.gitbook/assets/image%20%28116%29.png)

Llamamos “Distribución multicentro” a la implantación de la aplicación en una base de datos en la que éstos están divididos por centros de trabajo. Dentro de estos centros existe siempre uno definido como “central” que en este caso es la importadora y uno o varios centros de distribución o tiendas. En una distribución de este tipo cada documento existente en la base de datos tiene especificado como dato principal en la cabecera su “Centro”.

En una distribución de este tipo en las fichas de los artículos se exige para cada artículo la definición de un proveedor por cada centro. Es decir, el proveedor de un artículo en la central será el fabricante X y en la tienda puede ser otro, en la mayoría de casos la propia central.

Se representa en el gráfico anterior el caso en el que proveedor del material solicitado por el cliente es la propia central-importadora. En caso de que no lo fuera, el proceso es igual al definido en el apartado anterior de compras.

El diagrama representa la siguiente operativa:

1.        El cliente solicita material a través de una orden de reparación o un pedido.

2.        Al ser el proveedor para este artículo y centro la propia central se genera un pedido a proveedor en el que éste es la central.

3.        El sistema reconoce que es un documento interno \(al ser el proveedor del pedido un centro de la empresa\) y mediante el **sistema de réplicas de documentos** genera automáticamente en la central un pedido de cliente, siendo lógicamente el cliente el centro tienda.

4.        Según haya o no stock del material solicitado en el pedido, al confirmarlo se generará directamente un albarán de ventas o se pasará al sistema de pedidos de compras \(gráfico 1\). Si es éste el caso, al recibir el material y generar el albarán de entrada, éste hará la repartición por asignación en el pedido de clientes y se podrá generar el albarán de ventas.

5.        El albarán de ventas generado tendrá por lo tanto como centro la central-importadora y como cliente el centro “tienda”. Al ser el cliente un centro de la empresa el sistema lo reconoce como documento interno y mediante el sistema de réplicas de documentos creará automáticamente un albarán de compras  en la tienda.

6.        Tal como se explica en el proceso del ciclo de pedidos este albarán de entrada como cualquier otro ejecutará automáticamente la repartición por asignaciones en los pedidos de ventas y/o órdenes de reparación que lo originaron.

