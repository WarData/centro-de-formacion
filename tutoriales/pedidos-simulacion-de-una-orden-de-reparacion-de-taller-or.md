---
description: >-
  Generamos una OR que reserve varios artículos y que pida otros al proveedor,
  confirmando dicha orden de reparación, recepcionando el material e instalando
  las piezas en el vehículo para poder facturar
---

# Pedidos - simulación de una orden de reparación de taller OR

En este apartado vamos a simular que un cliente quiere realizar una revisión de 500 kilómetros en su vehículo en el taller, necesitando dicha intervención varios artículos de los que no conocemos su stock:

![Alta de la OR](../.gitbook/assets/image%20%28330%29.png)

![OR sin confirmar](../.gitbook/assets/image%20%28385%29.png)

![](../.gitbook/assets/image%20%28166%29.png)

El cliente B necesita varias referencias para una revisión \(en este caso hay varias en stock\) y otras dos sin stock \(51413-GB4-003 y BS10260\) para su vehículo, que generará un pedido de compras al proveedor correspondiente.

Una vez añadidas las líneas y/o conceptos a la OR pulsamos en el botón inferior "Confirmar" \(mensaje indicando que reserva artículos en stock - **PODEMOS INSTALARLOS EN EL MOMENTO** y/o realiza el pedido o pedidos a uno o varios proveedores de los artículos indicados en la ventana emergente\):

![](../.gitbook/assets/image%20%28486%29.png)

La OR queda en situación "En Curso" - materiales "Pendientes de Recibir / Pendientes de Entregar":

![Panel de ORs - Filtros existentes para control](../.gitbook/assets/image%20%28308%29.png)

Si la OR contenía algún artículo o artículos sin stock, Winmotor genera automáticamente el **pedido de compras** **a cada proveedor si no había ninguno ya existente sin tramitar \(si antes de confirmar el pedido de ventas ya existiera un pedido de compras al mismo proveedor del que el cliente solicita artículo sin stock, el sistema añadirá dicha pieza al pedido de compras existente\):**

![](../.gitbook/assets/image%20%28258%29.png)

Desde la pantalla anterior podemos abrir el pedido de compras generado por el artículo sin stock del pedido de ventas. **Es un pedido de compras SIN CONFIRMAR por lo que, otras líneas de pedidos de ventas u ORs al mismo proveedor y/o líneas adicionales para stock, se irán sumando hasta que se confirme el pedido de compras:**

![En esta situaci&#xF3;n se pueden a&#xF1;adir m&#xE1;s art&#xED;culos al pedido](../.gitbook/assets/image%20%281%29.png)

![Confirmaci&#xF3;n de la tramitaci&#xF3;n](../.gitbook/assets/image%20%28358%29.png)

Al tramitar, Winmotor nos permite enviarle al proveedor \(requiere configuración y que el proveedor disponga del sistema necesario para tramitar el documento\) un archivo con las líneas del pedido.

![](../.gitbook/assets/image%20%28156%29.png)

Una vez tramitado el pedido, existen [4 métodos de recepción de los pedidos de compras](../videos/metodos-de-recepcion-de-pedidos.md) que quedan resumidos en el vídeo del enlace:

1.- Pulsando en el botón recepcionar del pedido de compras

2.- En el panel de pedidos de compras &gt; pulsar en "Recepcionar" &gt; esta opción permite recepcionar artículos de uno o varios pedidos de un proveedor, mostrando todos los artículos pendientes de recibirse y generando un albarán de compras de los seleccionados

3.- Aperturando un albarán de compras al mismo proveedor que el indicado en el pedido de compras &gt; el sistema comparará artículos del albarán con los pendientes de recepcionarse y los dará como recibidos

4.- Mediante un archivo generado por el proveedor y que se podría introducir en Winmotor recepcionando automáticamente lo recibido y generando su albarán correspondiente \(el proveedor suele exigir el pedido de compras mediante archivo\)

Tras seleccionar el método de recepción de pedidos que mejor se adapte, el sistema generará un albarán de compras de las líneas recepcionadas \(en la siguiente imagen, sobre la línea marcada, podremos hacer doble clic e indicar las cantidades suministradas si difieren de las solicitadas originalmente\):

![Recepci&#xF3;n de pedidos](../.gitbook/assets/image%20%28483%29.png)

Pulsamos en "Crear albarán", dando por recepcionado el total del pedido \(podremos generar tantos albaranes como sean necesarios hasta dar el pedido de compras por completado, mientras, quedará en situación parcialmente recepcionado.

![Albar&#xE1;n de compras](../.gitbook/assets/image%20%283%29.png)

Existe un método para anular líneas cuando el albarán está confirmado en el siguiente enlace: [anular línea o líneas de un albarán de compras confirmado](albaranes/anular-una-linea-en-albaran-de-compras-confirmado.md)

Sobre el albarán obtenemos información sobre el pedido de ventas origen fácilmente, simplemente pulsando sobre el botón "Ventas relacionadas":

![Ventas relacionadas](../.gitbook/assets/image%20%2872%29.png)

Desde esta ventana podremos avisar al cliente mediante un SMS con un formato predefinido o uno de forma manual. Además, en la parte superior nos indica que esta pieza completa el pedido de ventas u OR, podemos instalar todo el material.

Observar el código de colores de la OR que indica su situación:

![Cat&#xE1;logo de colores en l&#xED;neas](../.gitbook/assets/image%20%28500%29.png)

Instalar el material \(código azul de color en las líneas de artículos\) seleccionando todas las líneas y pulsando en el botón "Instalar material" según la siguiente imagen:

![](../.gitbook/assets/image%20%2816%29.png)

![](../.gitbook/assets/image%20%28416%29.png)

![](../.gitbook/assets/image%20%2831%29.png)

![](../.gitbook/assets/image%20%28478%29.png)

Orden de reparación que permite:

1.- Aceptar \(guarda la OR - cierra la ventana\)

2.- Imprimir

3.- Impresión selectiva de la OR \(taller o cliente\)

4.- Cobrar anticipo de la OR

5.- Imprimir en PDF

6.- Aplicar situación \(Cerrar - permite enviar SMS a cliente notificando la finalización - no factura aún &gt; sólo desde pestaña "Facturación"

7.- Envío de SMS sin cerrar la OR

8.- Comprobar opciones en las pestañas \(intervenciones, recepción, tramitación de garantía, totales, facturación, estadísticas, también añadir archivos a la ficha de la OR, etc...\)

Comprobar cambios en el panel de ORs de la orden de reparación

![](../.gitbook/assets/image%20%28359%29.png)

Facturamos la OR, seleccionando la imputación correspondiente \(es posible dar de alta varias imputaciones iguales y varias imputaciones distintas como garantías, internas, siniestros...\). Al facturar observamos el cambio de situación en el panel de ordenes de reparación:

![](../.gitbook/assets/image%20%28267%29.png)





