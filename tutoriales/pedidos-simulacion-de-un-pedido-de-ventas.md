---
description: >-
  Generamos un pedido de ventas que reserve un artículo y que pida otro al
  proveedor, tramitando dicho pedido, recepcionándolo y entregando las piezas al
  cliente
---

# Pedidos - simulación de un pedido de ventas

En este apartado vamos a simular que entra un cliente a recambios y realiza un pedido de 2 artículos de los que no conocemos su stock:

![Vista del pedido de ventas - botones para a&#xF1;adir cliente y l&#xED;neas al pedido](../.gitbook/assets/image%20%28168%29.png)

El cliente A solicita una referencia en stock y otra sin stock, que generará un pedido al proveedor correspondiente \(también se pueden añadir líneas desde el despiece del proveedor pulsando en el botón "Despiece - Marca" y seleccionando el archivo generado\):

![Ejemplo de selecci&#xF3;n de art&#xED;culo en stock](../.gitbook/assets/image%20%28187%29.png)

![Ejemplo de selecci&#xF3;n de art&#xED;culo sin stock](../.gitbook/assets/image%20%28116%29.png)

Una vez añadidas las líneas y/o conceptos al pedido pulsamos en el botón inferior "Confirmar" para tramitar el pedido \(mensaje indicando que reserva artículos en stock - **PODEMOS ENTREGARLOS DESDE EL PEDIDO DE VENTAS EN EL MOMENTO** y/o realiza el pedido o pedidos a uno o varios proveedores\):

![](../.gitbook/assets/image%20%28189%29.png)

El pedido de ventas queda en situación "Pendiente de recibir / Pendiente de entregar":

![](../.gitbook/assets/image%20%28233%29.png)

Si el pedido de ventas contenía algún artículo o artículos sin stock, Winmotor genera automáticamente el **pedido de compras** **a cada proveedor si no había ninguno ya existente sin tramitar \(si antes de confirmar el pedido de ventas ya existiera un pedido de compras al mismo proveedor del que el cliente solicita artículo sin stock, el sistema añadirá dicha pieza al pedido de compras existente\):**

![Vista de pedidos generados tras pulsar &quot;Si&quot; en la ventana de confirmaci&#xF3;n anterior](../.gitbook/assets/image%20%28414%29.png)

Desde la pantalla anterior podemos abrir el pedido de compras generado por el artículo sin stock del pedido de ventas. **Es un pedido de compras SIN CONFIRMAR por lo que, otras líneas de pedidos de ventas u ORs al mismo proveedor y/o líneas adicionales para stock, se irán sumando hasta que se confirme el pedido de compras:**

![En esta situaci&#xF3;n se pueden a&#xF1;adir m&#xE1;s art&#xED;culos al pedido](../.gitbook/assets/image%20%281%29.png)

![Confirmaci&#xF3;n de la tramitaci&#xF3;n](../.gitbook/assets/image%20%28329%29.png)

Al tramitar, Winmotor nos permite enviarle al proveedor \(requiere configuración y que el proveedor disponga del sistema necesario para tramitar el documento\) un archivo con las líneas del pedido.

![](../.gitbook/assets/image%20%28142%29.png)

Una vez tramitado el pedido, existen [4 métodos de recepción de los pedidos de compras](../videos/metodos-de-recepcion-de-pedidos.md) que quedan resumidos en el vídeo del enlace:

1.- Pulsando en el botón recepcionar del pedido de compras

2.- En el panel de pedidos de compras &gt; pulsar en "Recepcionar" &gt; esta opción permite recepcionar artículos de uno o varios pedidos de un proveedor, mostrando todos los artículos pendientes de recibirse y generando un albarán de compras de los seleccionados

3.- Aperturando un albarán de compras al mismo proveedor que el indicado en el pedido de compras &gt; el sistema comparará artículos del albarán con los pendientes de recepcionarse y los dará como recibidos

4.- Mediante un archivo generado por el proveedor y que se podría introducir en Winmotor recepcionando automáticamente lo recibido y generando su albarán correspondiente \(el proveedor suele exigir el pedido de compras mediante archivo\)

Tras seleccionar el método de recepción de pedidos que mejor se adapte, el sistema generará un albarán de compras de las líneas recepcionadas \(en la siguiente imagen, sobre la línea marcada, podremos hacer doble clic e indicar las cantidades suministradas si difieren de las solicitadas originalmente\):

![Recepci&#xF3;n de Pedidos](../.gitbook/assets/image%20%28203%29.png)

Pulsamos en "Crear albarán", dando por recepcionado el total del pedido \(podremos generar tantos albaranes como sean necesarios hasta dar el pedido de compras por completado, mientras, quedará en situación parcialmente recepcionado.

![Albar&#xE1;n de compras](../.gitbook/assets/image%20%28388%29.png)

Existe un método para anular líneas cuando el albarán está confirmado en el siguiente enlace: [anular línea o líneas de un albarán de compras confirmado](albaranes/anular-una-linea-en-albaran-de-compras-confirmado.md)

Sobre el albarán obtenemos información sobre el pedido de ventas origen fácilmente, simplemente pulsando sobre el botón "Ventas relacionadas":

![](../.gitbook/assets/image%20%28420%29.png)

Desde esta ventana podremos avisar al cliente mediante un SMS con un formato predefinido o uno de forma manual. Además, en la parte superior nos indica que esta pieza completa el pedido de ventas, podemos entregar todo el material.

![](../.gitbook/assets/image%20%28408%29.png)

En el pedido de ventas podremos entregar los artículos reservados de stock y/o reservados por los pedidos de compras recepcionados pulsando en el botón "Entregar":

![](../.gitbook/assets/image%20%2824%29.png)

Pulsando en el recuadro blanco a la izquierda del cliente, podremos seleccionar todos los artículos incluidos en la venta, sino también podremos seleccionar cada artículos de forma independiente. **Luego pulsamos en "Crear albaranes" para entregar el material o en "Crear líneas OR" en caso de que el cliente decida que todo o parte del material, quiere que lo monte el taller \(la OR debe estar creada con anterioridad a la entrega del pedido\)**:

![](../.gitbook/assets/image%20%28195%29.png)

Albarán con opciones de:

1.- Guardarlo \(siempre se guarda en cualquier caso\)

2.- Eliminarlo

3.- Enviarlo por email \(el sistema lo convierte automáticamente en PDF, recoge los datos de la entidad rellenando su email e incluso se podría crear un cuerpo con un contenido predeterminado\)

4.- [Facturar](facturas_tutoriales/factura-cambiar-contenido.md) \(imprescindible para cobros\)

5.- Imprimir

6.- Imprimir en PDF

7.- Impresión selectiva \(muestra todas las opciones de impresión\)

8.- [Abono de línea o líneas](facturas_tutoriales/factura-abono-de-lineas-o-completo.md) - enlace a abonos una vez facturado el albarán



