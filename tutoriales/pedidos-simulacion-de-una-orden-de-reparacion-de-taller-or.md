---
description: >-
  Generamos una OR que reserve varios artículos y que pida otros al proveedor,
  confirmando dicha orden de reparación, recepcionando el material e instalando
  las piezas en el vehículo para poder facturar
---

# Pedidos - simulación de una orden de reparación de taller OR

En este apartado vamos a simular que un cliente quiere realizar una revisión de 500 kilómetros en su vehículo en el taller, necesitando dicha intervención varios artículos de los que no conocemos su stock:

![Alta de la OR](<../.gitbook/assets/image (387).png>)

![OR sin confirmar](<../.gitbook/assets/image (389).png>)

![](<../.gitbook/assets/image (388).png>)

El cliente B necesita varias referencias para una revisión (en este caso hay varias en stock) y otras dos sin stock (51413-GB4-003 y BS10260) para su vehículo, que generará un pedido de compras al proveedor correspondiente.

Una vez añadidas las líneas y/o conceptos a la OR pulsamos en el botón inferior "Confirmar" (mensaje indicando que reserva artículos en stock - **PODEMOS INSTALARLOS EN EL MOMENTO** y/o realiza el pedido o pedidos a uno o varios proveedores de los artículos indicados en la ventana emergente):

![](<../.gitbook/assets/image (390).png>)

La OR queda en situación "En Curso" - materiales "Pendientes de Recibir / Pendientes de Entregar":

![Panel de ORs - Filtros existentes para control](<../.gitbook/assets/image (392).png>)

Si la OR contenía algún artículo o artículos sin stock, Winmotor genera automáticamente el **pedido de compras** **a cada proveedor si no había ninguno ya existente sin tramitar (si antes de confirmar el pedido de ventas ya existiera un pedido de compras al mismo proveedor del que el cliente solicita artículo sin stock, el sistema añadirá dicha pieza al pedido de compras existente):**

![](<../.gitbook/assets/image (391).png>)

Desde la pantalla anterior podemos abrir el pedido de compras generado por el artículo sin stock del pedido de ventas. **Es un pedido de compras SIN CONFIRMAR por lo que, otras líneas de pedidos de ventas u ORs al mismo proveedor y/o líneas adicionales para stock, se irán sumando hasta que se confirme el pedido de compras:**

![En esta situación se pueden añadir más artículos al pedido](<../.gitbook/assets/image (377).png>)

![Confirmación de la tramitación](<../.gitbook/assets/image (378).png>)

Al tramitar, Winmotor nos permite enviarle al proveedor (requiere configuración y que el proveedor disponga del sistema necesario para tramitar el documento) un archivo con las líneas del pedido.

![](<../.gitbook/assets/image (379).png>)

Una vez tramitado el pedido, existen [4 métodos de recepción de los pedidos de compras](../videos/metodos-de-recepcion-de-pedidos.md) que quedan resumidos en el vídeo del enlace:

1.- Pulsando en el botón recepcionar del pedido de compras

2.- En el panel de pedidos de compras > pulsar en "Recepcionar" > esta opción permite recepcionar artículos de uno o varios pedidos de un proveedor, mostrando todos los artículos pendientes de recibirse y generando un albarán de compras de los seleccionados

3.- Aperturando un albarán de compras al mismo proveedor que el indicado en el pedido de compras > el sistema comparará artículos del albarán con los pendientes de recepcionarse y los dará como recibidos

4.- Mediante un archivo generado por el proveedor y que se podría introducir en Winmotor recepcionando automáticamente lo recibido y generando su albarán correspondiente (el proveedor suele exigir el pedido de compras mediante archivo)

Tras seleccionar el método de recepción de pedidos que mejor se adapte, el sistema generará un albarán de compras de las líneas recepcionadas (en la siguiente imagen, sobre la línea marcada, podremos hacer doble clic e indicar las cantidades suministradas si difieren de las solicitadas originalmente):

![Recepción de pedidos](<../.gitbook/assets/image (393).png>)

Pulsamos en "Crear albarán", dando por recepcionado el total del pedido (podremos generar tantos albaranes como sean necesarios hasta dar el pedido de compras por completado, mientras, quedará en situación parcialmente recepcionado.

![Albarán de compras](<../.gitbook/assets/image (394).png>)

Existe un método para anular líneas cuando el albarán está confirmado en el siguiente enlace: [anular línea o líneas de un albarán de compras confirmado](albaranes/anular-una-linea-en-albaran-de-compras-confirmado.md)

Sobre el albarán obtenemos información sobre el pedido de ventas origen fácilmente, simplemente pulsando sobre el botón "Ventas relacionadas":

![Ventas relacionadas](<../.gitbook/assets/image (395).png>)

Desde esta ventana podremos avisar al cliente mediante un SMS con un formato predefinido o uno de forma manual. Además, en la parte superior nos indica que esta pieza completa el pedido de ventas u OR, podemos instalar todo el material.

Observar el código de colores de la OR que indica su situación:

![Catálogo de colores en líneas](<../.gitbook/assets/image (396).png>)

Instalar el material (código azul de color en las líneas de artículos) seleccionando todas las líneas y pulsando en el botón "Instalar material" según la siguiente imagen:

![](<../.gitbook/assets/image (398).png>)

![](<../.gitbook/assets/image (399).png>)

![](<../.gitbook/assets/image (400).png>)

![](<../.gitbook/assets/image (401).png>)

Orden de reparación que permite:

1.- Aceptar (guarda la OR - cierra la ventana)

2.- Imprimir

3.- Impresión selectiva de la OR (taller o cliente)

4.- Cobrar anticipo de la OR

5.- Imprimir en PDF

6.- Aplicar situación (Cerrar - permite enviar SMS a cliente notificando la finalización - no factura aún > sólo desde pestaña "Facturación"

7.- Envío de SMS sin cerrar la OR

8.- Comprobar opciones en las pestañas (intervenciones, recepción, tramitación de garantía, totales, facturación, estadísticas, también añadir archivos a la ficha de la OR, etc...)

Comprobar cambios en el panel de ORs de la orden de reparación

![](<../.gitbook/assets/image (402).png>)

Facturamos la OR, seleccionando la imputación correspondiente (es posible dar de alta varias imputaciones iguales y varias imputaciones distintas como garantías, internas, siniestros...). Al facturar observamos el cambio de situación en el panel de ordenes de reparación:

![](<../.gitbook/assets/image (403).png>)
