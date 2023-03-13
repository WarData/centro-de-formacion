# Alta de una OR

<mark style="color:yellow;">**NUEVA OR**</mark>

Permite dar de alta a una nueva orden de reparación, rellenando el siguiente formulario:

<figure><img src="../../../../.gitbook/assets/imagen (7) (1).png" alt=""><figcaption></figcaption></figure>

El alta de una OR está compuesta por un formulario, donde se introducen los datos generales, como la serie, la fecha, [tipo de orden](../tipos-or.md), respecto al vehículo la matrícula, bastidor y cliente (pulsando tabulador después de introducir cualquiera de los datos anteriores rellenará automáticamente el resto), imputación, avería / síntoma, [tempario](../temparios.md), sección de taller, fechas de recepción y entrega prevista, kilometraje / horas, combustible, teléfono de la entidad y permite añadir y efectos personales.

**Serie**: es un campo imprescindible de rellenar, y por defecto toma el valor definido en la ficha del usuario que graba la OR. Esta serie permite multitud de ajustes debido a su <mark style="color:blue;">capacidad de generar distintos pedidos de compra en función del tipo de pedido del artículo</mark> (urgente, reposición o garantía), <mark style="color:blue;">hasta 4 líneas de facturación</mark>, una por cada imputación posible y <mark style="color:yellow;">avisos por llegada de mercancia reservada a la OR en la pestaña "Avisos"</mark>:

<figure><img src="../../../../.gitbook/assets/imagen (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Aviso recibido mediante la configuración de la serie OR > pestaña "Avisos":

<figure><img src="../../../../.gitbook/assets/imagen (2) (4).png" alt=""><figcaption></figcaption></figure>

**Fecha de apertura**: se indica aquí la fecha de grabación del documento. Esta fecha debe de estar dentro de los rangos definidos en parámetros.

**Tipo**: permite seleccionar uno de los existentes y que se pueden listar, modificar, borrar y dar de alta desde la opción Automoción > Taller > Tipos OR. El tipo permite organizar y localizar órdenes de reparación del mismo tipo, así como rellenar automáticamente la imputación y el tempario según el alta del tipo de OR que hayamos creado.

**Centro**: este campo solo será visible por aquellas aplicaciones en las que se trabaje con más de un centro de trabajo y así se haya indicado en parámetros. Se utiliza para indicar el centro de trabajo para el que se hace el albarán. Este campo, se rellena automáticamente y solo será editable por aquellos usuarios autorizados.

**Check - Presupuesto**: al marcar el check nos permite rellenar un nuevo campo "Referencia" a fin de control posterior por parte del cliente. La situación de la OR quedará como "Presupuesto" hasta que se confirme la OR que pasará a "En curso". Desde la versión presupuesto es posible crear nuevas versiones usando el botón ![](<../../../../.gitbook/assets/imagen (6) (1) (6).png>) mientras no se haya confirmado. Tanto si se genera una OR como presupuesto como las posteriores versiones del mismo quedarán registradas para su control y posible lectura desde la pestaña "Versiones del presupuesto" (sólo activa cuando se genera una OR como presupuesto).

**Matrícula y bastidor**: ambos campos pertenecen al mismo vehículo por lo que, rellenando total o parcialmente uno de ellos y tabulando rellenará el contrario y el cliente. Al dar de alta una nueva matrícula o bastidor, uno completa el otro en el alta y permite asociar el vehículo a un cliente nuevo o existente en la base de datos, quedando asignado a él:

<figure><img src="../../../../.gitbook/assets/imagen (2) (1).png" alt=""><figcaption><p>Alta vehículo en taller</p></figcaption></figure>

<mark style="color:yellow;">**\*\*\* Para dar de alta un vehículo que entra por primera vez en el taller, es decir, no se ha vendido por parte de la empresa, únicamente hay que rellenar la marca mediante el localizador, modelo se rellena a mano poniendo lo más completo posible, color, bastidor y matrícula (si es posible, obtener los datos de fecha de matriculación, fin de garantía y próxima ITV). Finalmente asignar o crear un propietario (cliente) y aceptar.**</mark> [<mark style="color:orange;">**Véase enlace a FAQ - "Asignar nuevos vehículos a nuevos clientes, existentes o asignar vehículo existente a otro cliente"**</mark>](../../../../faq/taller/asignar-nuevos-vehiculos-a-nuevos-clientes-existentes-o-asignar-vehiculo-existente-a-otro-cliente.md)<mark style="color:orange;">****</mark>

**Cliente**: tipo de entidad propietaria del vehículo y a la que se facturará por defecto la OR, aunque es posible modificar la línea de facturación para cambiar la entidad a petición del cliente. Contiene botones incrustados para localizar, grabar o editar el cliente.

<mark style="color:yellow;">\*\*\* Si un vehículo asociado a un cliente cambia de propietario, es posible rellenar la matrícula, cliente o bastidor, tabular para que se rellenen todos los datos y cambiar la entidad. Aparecerá un botón "Crear transferencia" \* que activará el histórico del nuevo propietario y mantendrá el histórico del anterior:</mark>

<figure><img src="../../../../.gitbook/assets/imagen (14).png" alt=""><figcaption></figcaption></figure>

**Imputación**: indica hacia qué departamento irá el cargo de la reparación. Existen 4 tipos estándar y se pueden dar de alta adicionales para servicios especiales como Honda ARE:

* Cliente: por defecto será el propietario del vehículo, pero se podrá modificar aunque siempre será hacia una entidad tipo cliente
* Siniestro: permite el uso de la pestaña ["Versión para la compañía" - pulse para ver instrucciones de uso](../../../../faq/ordenes-de-reparacion-ors/version-para-la-compania-en-la-or.md)
* Interna: el cargo irá a la empresa y habrá que especificar un departamento
* Garantía: en función de la marca, las garantías que requieran una facturación de la mano de obra se podrán efectuar usando este tipo

**Departamento interno**: si la imputación es interna, aparecerá un nuevo campo con el localizador de departamentos internos, teniendo que indicar qué departamento se hago cargo. Véase ["Departamentos internos"](../departamentos-internos.md):

<figure><img src="../../../../.gitbook/assets/imagen (1) (3).png" alt=""><figcaption></figcaption></figure>

**Avería / Síntoma:** campo cuya función es la de indicar el trabajo principal a realizar en el vehículo. El texto completará la línea de imputación marcándola en amarillo en la OR. En la OR se podrán añadir tantas como se deseen, tanto a un tipo de imputación como a otros, siendo la suma de las imputaciones la línea de facturación total en la pestaña de la OR "Facturación".

**Tempario**: es un tipo de servicio especial que además de un tiempo de mano de obra con su coste y precio de venta específico, permite añadir líneas de artículo y texto de los trabajos a realizar, simplificando las tareas habituales rellenando únicamente la referencia del tempario. Dentro del tempario podremos además duplicarlo para completar temparios similares cuyo contenido varíe poco y así agilizar el alta de nuevos. [Véase "Temparios"](../temparios.md)

**Sección de taller**: permite organizar las ORs por secciones de taller como soldadura, lavado, mecánica, chapa, etc. [Véase "Secciones de taller"](../secciones-de-taller.md)

**Almacén**: identifica el almacén general por defecto, pudiendo seleccionar otro del que se abastecerán las líneas de artículo de la OR. [Véase "Almacenes"](../../../almacenes/configuracion-1.md) y tutorial ["Almancén"](../../../../tutoriales/almacen/)

**Vendedor**: tomará por defecto el vendedor definido en la ficha del cliente. Se podrá modificar manualmente.

**Check - Vehículo recepcionado:** activa la recepción del vehículo por el taller y junto con la agenda de citas marca la cita como "Realizada", mostrando información sobre día y hora de recepción. Si la OR no existe y sí una cita por parte de un recepcionista, en el momento en el que se da de alta la OR y confirma, marca este check automáticamente.

**Fec. Prevista Recepción**: muestra una hora prevista de llegada del vehículo y, si se marca el check "Vehículo recepcionado", cambia el campo a "Fec. Recepción" como confirmación de la entrada del vehículo en el taller. Al igual que el check anterior, la agenda de citas en la recepción del vehículo y alta de la OR, tras su confirmación marca este campo con fecha y hora.

**Fec. Prevista Entrega**: muestra una fecha y hora a la que se estima se entregará el vehículo terminado. Al igual que los campos anteriores, la agenda de citas en la entrega alimentará este campo con la hora de entrega del vehículo, pudiéndose en todos los casos modificarlos manualmente.

**Recepcionista**: campo informativo sobre el usuario que está dando de alta la orden de reparación. Al igual que cualquier campo de Winmotor, se podrá presentar en los informes de impresión a modo informativo o con intención de valorar su atención por parte del cliente.

**CIF / NIF**: muestra el documento alimentado por el campo existente en la entidad

**Kilómetros / Horas**: campo de edición manual que <mark style="color:yellow;">servirá para alimentar información en otros campos como "Información de interés" en las citas que muestra los kilómetros / horas de la última OR</mark>, fecha de la misma, fecha de venta del vehículo si fue vendido por la empresa y fecha de fin de garantía.

**Combustible**: permite grabar el nivel al alta de la OR para control

**Teléfono**: el primer campo es libre a fin de grabar únicamente un número cualquier para avisos en la OR y el segundo campo coge el campo teléfono móvil del cliente, no es editable.

**Efectos personales**: campo que permite grabar cualquier detalle que el cliente deje en la moto y requiera de control como un casco, un mono, maletas, etc. Como hemos comentado anteriormente, este y cualquier campo se puede presentar en el informe de impresión de la OR de taller y cliente.

**Botonera inferior del alta de OR**

**Aceptar:** da de alta la OR con los datos introducidos en el formulario

**Aceptar y entregar vehículo de cortesía:** similar a aceptar y además abre formulario de entrega de vehículo de cortesía asociado al cliente del alta de la OR:

<figure><img src="../../../../.gitbook/assets/imagen (9).png" alt=""><figcaption></figcaption></figure>

**Cancelar**: omite el alta de la OR y sólo se realizaría la transferencia del vehículo a otro propietario si se hubiera dado el caso <mark style="color:yellow;">\*</mark>

<mark style="color:orange;">****</mark>
