# Stocks vehículos

La primera opción que nos muestra el menú comercial nos presenta una rejilla con un filtrado automático de vehículos por marca. <mark style="color:yellow;">Es importante recalcar que cada usuario podrá personalizar su panel cada vez que entre siguiendo unas breves instrucciones explicadas más adelante (establecer filtro por defecto).</mark>

El refresco del panel se puede automatizar en los parámetros de la aplicación para mostrar el listado de vehículos en stock o permitir filtrar primero y luego refrescar. Además, es posible auto-refrescar el panel independientemente del parámetro elegido y guardar este ajuste asociado al usuario pulsando el botón "Filtros" <img src="../../../.gitbook/assets/imagen (8).png" alt="" data-size="line">

<figure><img src="../../../.gitbook/assets/imagen (2).png" alt=""><figcaption></figcaption></figure>

Además, cada perfil dispone de la posibilidad de realizar varias configuraciones en el panel como:

1.- Restringir la venta de vehículos por centro: activo sólo en aquellos perfiles con centro aplicado. Imposibilita la venta de vehículos de centros distintos al que tiene aplicado el perfil

2.- Ver sólo el stock de vehículos de mi centro: filtra vehículos del centro aplicado en el perfil

3.- Ver todo el stock de vehículos de ocasión: sólo aplica si el check "ver sólo stock de vehículos de mi centro" está activo. Muestra los vehículos del centro aplicado en el perfil y los VO de todos los centros.

4.- Añadir stock de otros centros de las marcas: sólo aplica si el check "ver sólo stock de vehículos de mi centro" está activo. Muestra los vehículos del centro aplicado en el perfil y los de las marcas (de 1 a 5 como máximo) indicadas en el perfil.

<figure><img src="../../../.gitbook/assets/imagen (3).png" alt=""><figcaption></figcaption></figure>

El panel muestra la cabecera de cada una de las marcas seguida de los modelos de vehículos pertenecientes a la misma, situación de los vehículos (stock / reservados) por modelo y totalización de los vehículos al final, indicando la marca, por situación (stock / reservados):

<figure><img src="../../../.gitbook/assets/imagen (1).png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../../../.gitbook/assets/imagen (35) (1).png" alt=""><figcaption></figcaption></figure>

* Modelo: muestra marca, modelos y el total de modelos de la marca
* Stock (nuevos - ocasión - empresa): estos campos muestran el stock físico de los vehículos (no afecta a la reserva ya que se presentan en el siguiente campo)
* Reservados (nuevos - ocasión): identifican las reservas de los vehículos en stock físico&#x20;
* Pedidos a proveedor: vehículos pedidos sin reserva en operaciones
* Pedidos a proveedor reservados: vehículos pedidos con reserva en operaciones
* Stock disponible: disponibilidad para asignar a operaciones o documentos de ventas
* Stock Previsto: resultado de sumar el stock físico, reservado y disponible

<mark style="color:yellow;">BOTONERA SUPERIOR</mark>

Tipos de vehículos a mostrar en la rejilla principal de stock (requiere pulsar en "Actualizar" o F5):

<figure><img src="../../../.gitbook/assets/imagen (4).png" alt=""><figcaption></figcaption></figure>

Botones de filtros, opciones, búsqueda de vehículo en general, panel de comprobación de stocks, información sobre la rejilla y actualizar el panel:

<figure><img src="../../../.gitbook/assets/imagen (5).png" alt=""><figcaption></figcaption></figure>

A) Filtro ![](<../../../.gitbook/assets/imagen (6).png>)

Amplía la selección de múltiples filtros de marca y bastidor a estos más modelo, serie, reservadas o todas, en depósito, almacén o todas, cesiones y si están publicados en web o no. Pulsando en cerrar o actualizando se aplican los filtros, mostrándose los aplicados en la parte superior:

<figure><img src="../../../.gitbook/assets/imagen (9).png" alt=""><figcaption></figcaption></figure>

B) Opciones ![](<../../../.gitbook/assets/imagen (10).png>)

Muestra las siguiente opciones:

<figure><img src="../../../.gitbook/assets/imagen (11).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Localizar vehículo stock</mark>

Muestra un localizador con los índices "Alfabético (bastidor)", "Trozos de bastidor", "Trozos de matrícula" y "Trozos de palabras datos vehículo y propietario". En la barra de aplicación y botón "Opciones" podremos editar el localizador por defecto y siempre podemos usar cualquiera de los otros 3 disponibles. El uso es similar a otros localizadores de la aplicación en los que la búsqueda se inicia introduciendo como mínimo 3 caracteres de bastidor o matrícula en el que corresponda e igual en trozos de vehículo y propietario salvo que realiza la búsqueda en más campos de forma simultánea.

Este localizador incluye un filtrado previo de los vehículos por stock activo, en caso de no estar en stock no aparecerá.

<figure><img src="../../../.gitbook/assets/imagen (36) (5).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Listado de stock de vehículos</mark>

Permite listar el stock a fecha de hoy, a una fecha determinada, de vehículos nuevos o de ocasión o de empresa o todos y por marca, gama y versión mediante el uso de un ligero formulario:

<figure><img src="../../../.gitbook/assets/imagen (3) (8).png" alt=""><figcaption></figcaption></figure>

Mostramos un ejemplo de listado con el valor a hoy del stock y todos los vehículos:

<figure><img src="../../../.gitbook/assets/imagen (10) (3).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">F4 - Ampliar</mark>

Muestra un pequeño formulario que presentará rejillas de datos similares a la rejilla principal, pero centrándose en los datos escogidos en el formulario:

<figure><img src="../../../.gitbook/assets/imagen (16) (1) (1).png" alt=""><figcaption></figcaption></figure>

En este caso se muestra la rejilla basada en datos de ventas, no apareciendo costes de compra:

<figure><img src="../../../.gitbook/assets/imagen (8) (6).png" alt=""><figcaption></figcaption></figure>

En la siguiente imagen seleccionamos compras para mostrar el ejemplo:

<figure><img src="../../../.gitbook/assets/imagen (34).png" alt=""><figcaption></figcaption></figure>

Y por último (todo es similar a la rejilla del panel de stocks) el valor "Sin precios", eliminando de la rejilla los campos de compra y venta:

<figure><img src="../../../.gitbook/assets/imagen (2) (1) (1) (1) (2) (1).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Imprimir</mark>

Muestra las distintas posibilidades de impresión ofrecidas por la aplicación y el sistema operativo para imprimir el listado de stock:

<figure><img src="../../../.gitbook/assets/imagen (6) (8).png" alt=""><figcaption></figcaption></figure>

PDF de ejemplo - Página 1 del listado de stock de vehículos:

<figure><img src="../../../.gitbook/assets/imagen (7) (1) (1).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Establecer filtro por defecto</mark>

Una vez definidos los filtros y check de auto-refresco o no permite establecerlo como configuración del usuario por defecto cada vez que vuelva a abrir el panel, pudiendo modificar los parámetros puntualmente o hasta que decida establecer un nuevo filtrado por defecto

C) F2- Buscar vehículo ![](<../../../.gitbook/assets/imagen (12).png>)&#x20;

Muestra un localizador similar a la función "localizar vehículo stock", pero su operativa no lleva un filtrado previo por lo que <mark style="color:yellow;">**mostrará cualquier vehículo existente en la base de datos**</mark> mediante el uso de los distintos índices de búsqueda disponibles.

<mark style="color:yellow;">BOTONERA INFERIOR</mark>

<figure><img src="../../../.gitbook/assets/imagen (13).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Crear / Devolver depósito</mark>

Realiza el alta de un albarán de depósito hacia un agente (cambia la ubicación mostrada en la rejilla del stock) o desde un agente, creando el albarán de devolución de depósito en caso de estar el vehículo ya en el agente:

<figure><img src="../../../.gitbook/assets/imagen (14) (5).png" alt=""><figcaption></figcaption></figure>

Sólo requiere indicar la entidad agente y que la serie de depósitos de vehículos esté dada de alta [(véase "Series")](../../configuracion/series-de-documentos.md)

* <mark style="color:blue;">Crear Traslado</mark>

Movimiento entre almacenes o ubicaciones. Muestra el parte de almacén con el origen teniendo que indicar el almacén de destino:

<figure><img src="../../../.gitbook/assets/imagen (12) (4).png" alt=""><figcaption></figcaption></figure>

Una vez creado el traslado, se muestra el parte de almacén para confirmar y que sea efectivo o para guardarlo a fin de realizar la operativa en otro momento:

<figure><img src="../../../.gitbook/assets/imagen (4) (6).png" alt=""><figcaption></figcaption></figure>

Se indica una regularización de las líneas para el control de stock:

<figure><img src="../../../.gitbook/assets/imagen (1) (1) (1) (4) (2).png" alt=""><figcaption></figcaption></figure>

Finalmente cambia la ubicación mostrándose en la rejilla del panel de stock de vehículos:

<figure><img src="../../../.gitbook/assets/imagen (9) (5).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Crear Pedido</mark>

Da de alta un pedido de ventas hacia un cliente del vehículo seleccionado en la rejilla, ejecutándose la venta del vehículo mediante la facturación del albarán del pedido:

<figure><img src="../../../.gitbook/assets/imagen (5) (8).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Entregar</mark>

Da de alta un albarán de ventas hacia un cliente del vehículo seleccionado en la rejilla, ejecutándose la venta del vehículo mediante la facturación del mismo. Al ser similar a la entrega en la operación de un vehículo, mostrará la posibilidad de actualizar los datos de matriculación y el siguiente formulario en caso de aceptar la actualización:

<figure><img src="../../../.gitbook/assets/imagen (17) (4) (1).png" alt=""><figcaption></figcaption></figure>

Tras actualizar los datos de matriculación, aparecerá el formulario de alta del albarán de ventas, donde únicamente tendremos que rellenar la entidad cliente, ya que el documento recogerá el precio de venta estipulado en la ficha del vehículo seleccionado <mark style="color:yellow;">**(por ello es importante verificar que el importe del albarán es correcto o no está a 0 ya que no se podrá facturar**</mark>):

<figure><img src="../../../.gitbook/assets/imagen (15) (6) (1).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Imprimir</mark>

Muestra las distintas posibilidades de impresión ofrecidas por la aplicación y el sistema operativo para imprimir el listado de stock:

<figure><img src="../../../.gitbook/assets/imagen (6) (8).png" alt=""><figcaption></figcaption></figure>

PDF de ejemplo - Página 1 del listado de stock de vehículos:

<figure><img src="../../../.gitbook/assets/imagen (7) (1) (1).png" alt=""><figcaption></figcaption></figure>
