# Asignar nuevos vehículos a nuevos clientes, existentes o asignar vehículo existente a otro cliente

Existen la posibilidad de requerir el alta de un vehículo que no está en su base de datos y asignarlo tanto a un cliente existente como un cliente nuevo o asignar un vehículo existente a un nuevo cliente o existente.

Estos casos ocurren cuando:

* La base de datos es nueva y no tiene creados ni vehículos ni clientes
* La base de datos es nueva y no tiene creado vehículos, pero sí tiene clientes
* Es un cliente nuevo de taller con un vehículo existente en la base de datos (lo compró de segunda mano)
* Es un cliente nuevo con un vehículo no existente en la base de datos
* El vehículo existe en la base de datos, pero no coincide con el cliente actual, pudiendo ser nuevo o existente > <mark style="color:yellow;">**requiere crear transferencia desde el alta de la OR**</mark>

Para ambos casos, el procedimiento es muy similar y aquí os contamos las excepciones y el proceso completo desde el alta de una OR:

1.- Si el cliente existe rellenará automáticamente los datos de vehículo en el alta de la OR, de la misma forma si se rellena la matrícula, identificará el cliente al tabular:

<figure><img src="../../.gitbook/assets/imagen (39) (3).png" alt=""><figcaption></figcaption></figure>

2.- Si el vehículo pertenece a otro cliente existente en la base de datos, localizarlo y cambiarlo en el alta, apareciendo el botón "Crear transferencia" y de igual modo si no existe, darlo de alta pulsando en el botón ![](<../../.gitbook/assets/imagen (116).png>) señalado en la imagen siguiente y proceder pulsando "Crear transferencia":

<figure><img src="../../.gitbook/assets/imagen (81).png" alt=""><figcaption></figcaption></figure>

* A partir de ese momento, se guardará el histórico anterior y se generará uno nuevo para el cliente
* Este método sirve tanto si el cliente existe como si es nuevo, sólo debe existir el bastidor

3.- Si no existe el vehículo (se introduce la matrícula y no rellena ningún dato) es posible que haya cambiado la matrícula, por lo que durante el alta como nuevo vehículo dará un error por existir el bastidor. Cancelar proceso y buscar en "Automoción" > "Histórico vehículos" el bastidor por si existe en la base de datos. Para el alta del vehículo nuevo en la aplicación:

* Desde el alta de la OR pulsar en el localizador > Nuevo y aparecerá un formulario de alta:

<figure><img src="../../.gitbook/assets/imagen (94) (2).png" alt=""><figcaption></figcaption></figure>

* Formulario de alta de vehículo en el que hay que <mark style="color:yellow;">**indicar marca y color mediante el localizador**</mark> y <mark style="color:yellow;">**rellenar manualmente modelo (no rellenar gama ni versión):**</mark>

<figure><img src="../../.gitbook/assets/imagen (34) (3).png" alt=""><figcaption></figcaption></figure>

* En el caso de existir el cliente, localizarlo en el campo propietario:

<figure><img src="../../.gitbook/assets/imagen (6) (1).png" alt=""><figcaption></figcaption></figure>

* En el caso de no existir el cliente, darlo de alta usando el campo "Nuevo" en el campo propietario:

<figure><img src="../../.gitbook/assets/imagen (107) (5).png" alt=""><figcaption></figcaption></figure>

<mark style="color:yellow;">**\*\*\* Rellenar todos los datos necesarios de la entidad y seleccionar tipo "Cliente"**</mark>

<figure><img src="../../.gitbook/assets/imagen (105).png" alt=""><figcaption></figcaption></figure>

4.- Una vez asignado el cliente a un vehículo dado de alta desde la OR y aceptando el formulario y tabulando posteriormente, asignará el nuevo vehículo al cliente:

<figure><img src="../../.gitbook/assets/imagen (102) (2).png" alt=""><figcaption></figcaption></figure>

Tras aceptar la OR y tabular:

<figure><img src="../../.gitbook/assets/imagen (38).png" alt=""><figcaption></figcaption></figure>

<mark style="color:yellow;">**5.- NO ES NECESARIO COMPLETAR LA OR SI NO ES NECESARIO, EL ALTA DE VEHÍCULO / TRANSFERENCIA SE HA PRODUCIDO, POR LO QUE AUNQUE SE CANCELE LA OR, SE MANTENDRÁN LAS ALTAS Y TRANSFERENCIAS**</mark>
