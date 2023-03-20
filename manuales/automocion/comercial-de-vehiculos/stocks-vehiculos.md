# Stocks vehículos

La primera opción que nos muestra el menú comercial nos presenta una rejilla con un filtrado automático de vehículos por marca, presentando la cabecera de cada una seguida de los vehículos pertenecientes a la misma, situación de los vehículos (stock / reservados) por modelo y totalización de los vehículos al final, indicando la marca, por situación (stock / reservados):

<figure><img src="../../../.gitbook/assets/imagen (17) (3).png" alt=""><figcaption></figcaption></figure>

<mark style="color:yellow;">PESTAÑAS</mark>

<mark style="color:blue;">DETALLES (rejilla con la información detallada de marcas y vehículos en stock):</mark>

* Nombre: identifica la marca y los modelos asociados a ella
* Bastidor: identifica el vehículo con su bastidor
* Color: de cada modelo, identifica su color para facilitar el control de stock
* Ubicación: lugar donde se encuentra el vehículo. Puede mostrar el almacén principal, uno de tránsito e incluso el nombre de un agente que tiene el vehículo en depósito:

<figure><img src="../../../.gitbook/assets/imagen (1) (6).png" alt=""><figcaption></figcaption></figure>

* Reservado: muestra si el vehículo se encuentra en pre-reserva o reserva en una operación indicando el nombre de la entidad cliente
* Días Stock: indica el número de días que han pasado desde la entrada del vehículo en el stock mediante albarán de compras
* Días Último Movimiento: indica los días que han pasado desde que hubo algún movimiento del vehículo, ya sea entrada al stock, traslados o depósitos.
* Días Vencimiento Cmp (compra): cálculo de días desde hoy hasta la fecha de entrada y salida del vehículo. Es un cálculo interno de la aplicación
* CES (cesión): icono que aparece en este campo indicando si el vehículo se encuentra cedido
* EXT (extras): icono que aparece en este campo indicando si el vehículo tiene extras

<mark style="color:blue;">TOTALES (rejilla con la información relativa al stock en función con el tipo de vehículo, reservas en función del tipo de vehículo, pedidos a proveedor, pedidos a proveedor con reserva, stock disponible y stock previsto (sumas entre los distintos campos que muestra el resultado disponible)):</mark>

<figure><img src="../../../.gitbook/assets/imagen (35).png" alt=""><figcaption></figcaption></figure>

* Modelo: muestra marca, modelos y el total de modelos de la marca
* Stock (nuevos - ocasión - empresa): estos campos muestran el stock físico de los vehículos (no afecta a la reserva ya que se presentan en el siguiente campo)
* Reservados (nuevos - ocasión): identifican las reservas de los vehículos en stock físico&#x20;
* Pedidos a proveedor: vehículos pedidos sin reserva en operaciones
* Pedidos a proveedor reservados: vehículos pedidos con reserva en operaciones
* Stock disponible: disponibilidad para asignar a operaciones o documentos de ventas
* Stock Previsto: resultado de sumar el stock físico, reservado y disponible

<mark style="color:yellow;">BOTONERA SUPERIOR</mark>

Tipos de vehículos a mostrar en la rejilla principal de stock (requiere pulsar en "Actualizar" o F5:

<figure><img src="../../../.gitbook/assets/imagen (11).png" alt=""><figcaption></figcaption></figure>

Botones de opciones sobre el stock:

<figure><img src="../../../.gitbook/assets/imagen (12) (3).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">F1 - Buscar Vehículo Stock</mark>

Muestra un localizador con los índices "Alfabético (bastidor)", "Trozos de bastidor", "Trozos de matrícula" y "Trozos de palabras datos vehículo y propietario". En la barra de aplicación y botón "Opciones" podremos editar el localizador por defecto y siempre podemos usar cualquiera de los otros 3 disponibles. El uso es similar a otros localizadores de la aplicación en los que la búsqueda se inicia introduciendo como mínimo 3 caracteres de bastidor o matrícula en el que corresponda e igual en trozos de vehículo y propietario salvo que realiza la búsqueda en más campos de forma simultánea.

Este localizador incluye un filtrado previo de los vehículos por stock activo, en caso de no estar en stock no aparecerá.

<figure><img src="../../../.gitbook/assets/imagen (36).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">F2 - Buscar Vehículo</mark>

Muestra un localizador idéntico a la función anterior, pero su operativa no lleva un filtrado previo por lo que <mark style="color:yellow;">**mostrará cualquier vehículo existente en la base de datos**</mark> mediante el uso de los distintos índices de búsqueda disponibles.

* <mark style="color:blue;">F3 - Listar Stocks</mark>

Permite listar el stock a fecha de hoy, a una fecha determinada, de vehículos nuevos o de ocasión o de empresa o todos y por marca, gama y versión mediante el uso de un ligero formulario:

<figure><img src="../../../.gitbook/assets/imagen (3) (8).png" alt=""><figcaption></figcaption></figure>

Mostramos un ejemplo de listado con el valor a hoy del stock y todos los vehículos:

<figure><img src="../../../.gitbook/assets/imagen (10) (3).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">F4 - Ampliar</mark>

Muestra un pequeño formulario que presentará rejillas de datos similares a la rejilla principal, pero centrándose en los datos escogidos en el formulario:

<figure><img src="../../../.gitbook/assets/imagen (16).png" alt=""><figcaption></figcaption></figure>

En este caso se muestra la rejilla basada en datos de ventas, no apareciendo costes de compra:

<figure><img src="../../../.gitbook/assets/imagen (8) (6).png" alt=""><figcaption></figcaption></figure>

En la siguiente imagen seleccionamos compras para mostrar el ejemplo:

<figure><img src="../../../.gitbook/assets/imagen (34).png" alt=""><figcaption></figcaption></figure>

Y por último (todo es similar a la rejilla del panel de stocks) el valor "Sin precios", eliminando de la rejilla los campos de compra y venta:

<figure><img src="../../../.gitbook/assets/imagen (2) (1).png" alt=""><figcaption></figcaption></figure>

<mark style="color:yellow;">BOTONERA INFERIOR</mark>

<figure><img src="../../../.gitbook/assets/imagen (13) (4).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Crear / Devolver depósito</mark>

Realiza el alta de un albarán de depósito hacia un agente (cambia la ubicación mostrada en la rejilla del stock) o desde un agente, creando el albarán de devolución de depósito en caso de estar el vehículo ya en el agente:

<figure><img src="../../../.gitbook/assets/imagen (14) (5).png" alt=""><figcaption></figcaption></figure>

Sólo requiere indicar la entidad agente y que la serie de depósitos de vehículos esté dada de alta [(véase "Series")](../../configuracion/series-de-documentos.md)

* <mark style="color:blue;">Crear Traslado</mark>

Movimiento entre almacenes o ubicaciones. Muestra el parte de almacén con el origen teniendo que indicar el almacén de destino:

<figure><img src="../../../.gitbook/assets/imagen (12).png" alt=""><figcaption></figcaption></figure>

Una vez creado el traslado, se muestra el parte de almacén para confirmar y que sea efectivo o para guardarlo a fin de realizar la operativa en otro momento:

<figure><img src="../../../.gitbook/assets/imagen (4) (6).png" alt=""><figcaption></figcaption></figure>

Se indica una regularización de las líneas para el control de stock:

<figure><img src="../../../.gitbook/assets/imagen (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Finalmente cambia la ubicación mostrándose en la rejilla del panel de stock de vehículos:

<figure><img src="../../../.gitbook/assets/imagen (9) (5).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Crear Pedido</mark>

Da de alta un pedido de ventas hacia un cliente del vehículo seleccionado en la rejilla, ejecutándose la venta del vehículo mediante la facturación del albarán del pedido:

<figure><img src="../../../.gitbook/assets/imagen (5) (8).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Entregar</mark>

Da de alta un albarán de ventas hacia un cliente del vehículo seleccionado en la rejilla, ejecutándose la venta del vehículo mediante la facturación del mismo. Al ser similar a la entrega en la operación de un vehículo, mostrará la posibilidad de actualizar los datos de matriculación y el siguiente formulario en caso de aceptar la actualización:

<figure><img src="../../../.gitbook/assets/imagen (17) (4).png" alt=""><figcaption></figcaption></figure>

Tras actualizar los datos de matriculación, aparecerá el formulario de alta del albarán de ventas, donde únicamente tendremos que rellenar la entidad cliente, ya que el documento recogerá el precio de venta estipulado en la ficha del vehículo seleccionado <mark style="color:yellow;">**(por ello es importante verificar que el importe del albarán es correcto o no está a 0 ya que no se podrá facturar**</mark>):

<figure><img src="../../../.gitbook/assets/imagen (15) (6).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Imprimir</mark>

Muestra las distintas posibilidades de impresión ofrecidas por la aplicación y el sistema operativo para imprimir el listado de stock:

<figure><img src="../../../.gitbook/assets/imagen (6) (8).png" alt=""><figcaption></figcaption></figure>

PDF de ejemplo - Página 1 del listado de stock de vehículos:

<figure><img src="../../../.gitbook/assets/imagen (7).png" alt=""><figcaption></figcaption></figure>
