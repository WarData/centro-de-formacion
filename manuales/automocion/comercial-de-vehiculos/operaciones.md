# Operaciones

Este menú presenta un panel donde se obtiene una rejilla de datos con las operaciones en distintas situaciones, distintos tipos de vehículos, filtros de fecha, vendedor, cliente y marca y 2 botoneras en el lateral izquierdo:

<figure><img src="../../../.gitbook/assets/imagen (24).png" alt=""><figcaption></figcaption></figure>

<mark style="color:yellow;">OPERACIÓN</mark>

Desde el momento en el que se realiza un presupuesto y sus situaciones posteriores se entiende que se da de alta una nueva operación.

Está formada por todos los documentos que se pueden generar en ella, desde un presupuesto hasta los pedidos de ventas, OR de pre-entrega, albaranes y facturas; el bastidor asociado a la operación confirmada y todos los anticipos y cobros realizados.

Todo se podrá gestionar desde el propio documento de la operación sin necesidad de recurrir a otras opciones de la aplicación.

<mark style="color:yellow;">TIPO DE VEHÍCULO</mark>

Filtra en la rejilla las operaciones por tipo de vehículo

<figure><img src="../../../.gitbook/assets/imagen (11).png" alt=""><figcaption></figcaption></figure>

<mark style="color:yellow;">SITUACIONES</mark>

Desde el momento del alta de una operación hasta su finalización se producen varias situaciones que nos permitirán gestionar y controlarlas.

* <mark style="color:blue;">Iniciadas</mark>: son aquellas que constan como mínimo de un presupuesto y una entidad pre-cliente o cliente. Su alta grabará un registro de control para seguimientos en la [agenda del vendedor](../../utilidades/agenda.md). **El color de la situación es gris claro salvo iniciadas con anticipo que cuyo **<mark style="color:red;">**color de la situación es rojo.**</mark>
* <mark style="color:blue;">Pre-reservadas</mark>: desde la ficha de un vehículo nuevo o usado en stock, en la botonera inferior encontramos "Pre-reservar". **El color de la **<mark style="color:green;">****</mark>** situación es gris claro**:

<figure><img src="../../../.gitbook/assets/imagen (2).png" alt=""><figcaption></figcaption></figure>

Este botón da de alta una nueva operación en la situación indicada, similar a iniciada, pero con la gran diferencia de que reserva el bastidor a la operación, indicándolo además en el stock de vehículos:&#x20;

<figure><img src="../../../.gitbook/assets/imagen (16).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Confirmadas</mark>: son aquellas que, estando en la situación iniciadas o pre-reservadas, han sido confirmadas mediante el botón del panel de operaciones o desde la propia operación, generando una reserva del bastidor y pasando su estado a generar pedidos de venta de vehículo y solicitar pedidos de compra si el bastidor no está en stock. <mark style="color:green;">El color de la situación es verde</mark>
* <mark style="color:blue;">En curso</mark>: engloba varias situaciones identificadas de tal forma que no estén pendientes de confirmación o están finalizadas (salvo iniciadas con anticipo que sí se considera en curso y <mark style="color:red;">su color de situación es rojo</mark>) y que requieren de algún proceso como la recepción de material o vehículo, pagos, entrega de vehículo. Es decir, operación puesta en marcha mediante el pago de un anticipo, confirmadas con o sin cobro y confirmadas con material pendiente de recibir o entregar. <mark style="color:blue;">El color de la situación es azul.</mark>
* <mark style="color:blue;">Cobradas</mark>: engloba todas las situaciones cobradas, estén pendientes de recibir o entregar material. <mark style="color:blue;">El color de la situación es azul.</mark>
* <mark style="color:blue;">Entregadas</mark>: son aquellas operaciones cuyo vehículo y opciones han sido entregados al cliente. **El color de la situación es gris claro.**
* <mark style="color:blue;">Expediente finalizado</mark>: son aquellas marcadas con el botón "Expediente finalizado" incluido en la operación y que sirve como referencia al vendedor o concesionario de un momento concreto de la operación de forma manual:

<figure><img src="../../../.gitbook/assets/imagen (20).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Anuladas</mark>: son aquellas operaciones marcadas con el botón "Anular" del panel de operaciones. Son operaciones que no deben tener cobros asociados y estar en situación iniciada. <mark style="color:orange;">El color de la situación es naranja</mark>:

<figure><img src="../../../.gitbook/assets/imagen (22).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">Todas</mark>: engloba todos los tipos de situaciones. Recomendamos su uso junto con el filtro de fecha para evitar mostrar excesivos datos en la rejilla

<mark style="color:yellow;">BOTONERAS</mark>

**Botonera alta, búsqueda y listado de operaciones:**

<figure><img src="../../../.gitbook/assets/imagen (1).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">F1 - Nueva</mark>: muestra el formulario de alta de una operación:

<figure><img src="../../../.gitbook/assets/imagen (8).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">F2 - Buscar</mark>: muestra el localizador de búsqueda por índices:

<figure><img src="../../../.gitbook/assets/imagen (26).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:blue;">F3 - Listado</mark>: potente filtro para la localización de operaciones mediante serie, situación, rangos de fecha por apertura, confirmación, cobro y entrega, tipo de vehículo, marca, cliente, vendedor y ventas con agentes:

<figure><img src="../../../.gitbook/assets/imagen (28).png" alt=""><figcaption></figcaption></figure>

**Botonera de confirmación, cobro, entrega y anulación:**

<figure><img src="../../../.gitbook/assets/imagen (30).png" alt=""><figcaption></figcaption></figure>

Seleccionando una operación en el panel principal **aplica la acción directamente** sobre ella sin necesidad de acceder a la ficha del documento.

* <mark style="color:blue;">Anular</mark>: cancela la operación siempre que se encuentre en situación iniciada y sin cobros
* <mark style="color:blue;">Confirmar</mark>: desde situación iniciada o pre-reservada cambia la situación generando los documentos necesarios para la venta en función de lo que requiera la operación
* <mark style="color:blue;">Cobrar</mark>: activa el cobro de la operación restando los anticipos, generando además automáticamente la OR de pre-entrega. Esta OR se puede generar manualmente desde el botón de la operación "Acciones Especiales" > "Crear OR Pre-entrega"
* <mark style="color:blue;">Entregar</mark>: cuando la operación se encuentre cobrada y el vehículo en stock, se entrega al cliente permitiendo actualizar o no los datos de matriculación y generando la factura del vehículo.
