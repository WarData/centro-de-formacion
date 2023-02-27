# Pedidos

**PEDIDOS DE VENTAS**

Mediante este menú, podremos grabar, modificar o consultar todos los pedidos que han realizado nuestros clientes. Al entrar en ella, nos aparece un panel en el que se nos presentan opciones para crear un nuevo pedido, buscar uno ya creado, sacar listados de pedidos y consultar las unidades pendientes de recibir de un determinado artículo. Además de estas opciones, podemos ver una rejilla con todos los pedidos en curso y su situación, con al menos una referencia pendiente de entregar o recibir:

<figure><img src="../../../.gitbook/assets/imagen (143).png" alt=""><figcaption></figcaption></figure>

**1 - NUEVO PEDIDO**

Permite dar de alta un nuevo pedido de material rellenando el siguiente formulario:

<figure><img src="../../../.gitbook/assets/imagen (142).png" alt=""><figcaption></figcaption></figure>

Un pedido está compuesto por la cabecera, donde se introducen los datos generales del pedido, como la serie, la fecha o cliente, y las líneas, donde se va grabando en cada una de ellas la referencia y la cantidad que se va a añadir al pedido.

La imagen anterior nos muestra un formulario de pedidos de material, donde se graban tanto los datos generales, como las líneas con las referencias. La cabecera de un pedido está compuesta por los siguientes campos:

* **Serie:** es un campo imprescindible de rellenar, y por defecto toma el valor definido en los parámetros del programa. Podemos utilizarlo para clasificar diferentes tipos de pedidos, como por ejemplo, serie B para pedidos de boutique y R para recambios. Además, en las series de los documentos se pueden definir distintas características que tomará el pedido por defecto, entre ellas, se puede indicar que calcule los impuestos, lo que significa que el pedido llevará calculado en sus bases el impuesto correspondiente.
* **Número:** todos los documentos están clasificados por su serie y un número, que siempre será por defecto el siguiente al último grabado de la misma serie. Tanto el número como la serie de un documento se podrán modificar manualmente, aunque, a menos que sea imprescindible el cambio, no es aconsejable.
* **Fecha:** se indica aquí la fecha de grabación del documento. Esta fecha debe de estar dentro de los rangos definidos en parámetros.
* **Situación:** este campo no es manipulable por el usuario, y nos indica la situación del pedido. Esta puede ser, PENDIENTE TRAMITAR, nos indica que todas las referencias solicitadas aún están pendiente de recibir y tramitar, TRAMITADO, indica que el pedido ha sido solicitado al proveedor y el documento pasará a esta situación si se imprime, envía por e-mail o se genera el fichero correspondiente para tramitarlo mediante algún método utilizado por el proveedor, INCOMPLETO, indica que se ha recibido parte del pedido, RECIBIDO, indica que todas las referencias han sido recibidas.
* **Referencia:** se puede anotar aquí la referencia del pedido del proveedor y localizar el pedido mediante este campo en "Buscar" y el localizador "Referencia".
* **Centro:** este campo solo será visible por aquellas aplicaciones en las que se trabaje con más de un centro de trabajo y así se haya indicado en parámetros. Se utiliza para indicar el centro de trabajo para el que se hace el pedido. Este campo, se rellena automáticamente y solo será manipulable por aquellos usuarios autorizados.
* **Tipo de pedido:** se indica aquí si el pedido es de reposición, urgente, campaña o garantía.
* **Proveedor:** indicamos aquí el proveedor al que vamos a realizar el pedido. Y mediante botón insertado en el campo del código del proveedor, podremos localizarlo, grabar uno nuevo o modificar el seleccionado. Además, podremos cambiar los datos del proveedor seleccionado en este pedido a través de los campos situados justo debajo del código del proveedor. Estos campos solo afectarán a este pedido y no se cambiará la ficha del proveedor.
* **Divisa:** presenta la divisa en la que se genera el pedido.
* **Régimen de IVA:** en este campo se indica el régimen de IVA que afecta al conjunto de las líneas añadidas al pedido.

**Barra de pestañas**

* **LÍNEAS:** contiene una rejilla en la que se nos presentan las líneas de pedidos de material ordenadas por el campo contador de cada línea. Mediante está rejilla podremos consultar, grabar, modificar o eliminar cualquier línea de pedido.

Para grabar una nueva línea de pedido, podemos utilizar cualquiera de los métodos utilizados sobre cualquier otra rejilla. Se nos presentará el formulario de grabación de líneas con los siguientes campos:

<figure><img src="../../../.gitbook/assets/imagen (130).png" alt=""><figcaption></figcaption></figure>

\* **Artículo**: campo en el que introducimos la referencia del artículo que vamos a pedir. Se podrá meter la referencia manualmente, o utilizando la opción "Localizar Artículo" de los botones incrustados de este campo. Una vez asignado el pedido no se puede cambiar el artículo pero si podemos ver su ficha, en el botón que se encuentra al lado del nombre.

Si no localizamos la referencia en la base de datos de artículos, podemos utilizar  el campo "Referencia". Con esta opción, el programa buscará en primer lugar en el fichero de artículos, y si no la encontrara, buscará en el de tarifas. Una vez localizada, se nos presentará el siguiente formulario, desde el que podremos crear la referencia directamente (es imprescindible indicar tipo de artículo para el alta):

<figure><img src="../../../.gitbook/assets/imagen (135).png" alt=""><figcaption></figcaption></figure>

Los otros dos botones incrustados que contiene el campo de artículo, son para consultar/editar la referencia seleccionada, o para crear una nueva.

La descripción del artículo tomará por defecto la definida en su ficha, pero podrá ser modificada manualmente.

Una vez añadida la línea, se muestra su contenido con doble clic. Especial atención a que, cada artículo puede tener asociado en su tarifa de proveedor un tipo de pedido de compras por defecto, modificable, pero si no lo tiene, se puede seleccionar directamente entrando en la línea del pedido de ventas:

<figure><img src="../../../.gitbook/assets/imagen (152).png" alt=""><figcaption></figcaption></figure>

Una vez se confirma el pedido, automáticamente se reservarán los artículos en stock y/o se realizarán los pedidos de compras en caso de falta de stock de algún artículo. Se darán de alta nuevos pedidos por proveedor o se usarán si son del mismo proveedor en situación "Pendiente de tramitar".

En la parte de gestión del pedido se muestran los siguientes campos:

\- **Pedidas**: campo para insertar las unidades que solicitamos al proveedor.

\- **Anuladas**: este campo podrá ser utilizado para anular unidades pendientes de recibir del proveedor y que vayamos a recibirlas.

\- **Reservadas de stock**: unidades reservadas del stock. En la ficha del artículo se mostrará en la pestaña "Stock" las unidades físicas totales, las reservadas de stock y un botón info\* arriba para ver qué pedidos tienen la reserva, el stock disponible más las unidades pendientes de recibirse y las unidades reservadas por pedido de compras dando un total previsto:

<figure><img src="../../../.gitbook/assets/imagen (145).png" alt=""><figcaption></figcaption></figure>

\*Botón info:

<figure><img src="../../../.gitbook/assets/imagen (129).png" alt=""><figcaption></figcaption></figure>



También es posible anular y [reasignar artículos ya asignados a pedidos (pulse para ir a la página)](../../../tutoriales/reasignacion-de-articulos-ya-asignados-a-pedido.md) - **Recibidas**: nos presenta las unidades que hemos recibido (no manipulable por el usuario). Para anular el total de reservas hay que pulsar en el botón al lado de info\* (una papelera), indicando el sistema lo que va a realizar (sólo para usuarios supervisores):

<figure><img src="../../../.gitbook/assets/imagen (136).png" alt=""><figcaption></figcaption></figure>

Indicará las unidades anuladas y cambiará la línea de stock:

<figure><img src="../../../.gitbook/assets/imagen (141).png" alt=""><figcaption></figcaption></figure>

A la vez, en los pedidos de ventas se indicará anuladas en la línea de alta:

<figure><img src="../../../.gitbook/assets/imagen (155).png" alt=""><figcaption></figcaption></figure>

\- **Pendientes de recibir**: unidades pedidas aún no recepcionadas mediante albarán de compras o recepción del pedido de compras

\- **Entregables**: del total de unidades de la línea, muestra las que se pueden entregar al cliente mediante un albarán de ventas

\- **Entregadas**: unidades que han salido del stock mediante un albarán de ventas

\- **Pendientes de entregar**: diferencia de unidades entre las pedidas y las entregadas

\- **Stock actual**: muestra en campo stock disponible del artículo a modo informativo

En el resto del formulario:

\- **Precio**: importe del artículo.

\- **Parcial**: valor total del artículo (sin sumar los impuestos) resultante de multiplicar las unidades pedidas por el precio menos los descuentos.

\- **Acción**: es una rejilla en la que podemos ver si las unidades pedidas en esta línea han sido reservadas por algún cliente o agente. Muestra diferentes acciones como Pedido Proveedor, Recepción, Asignación y Anulación:

<figure><img src="../../../.gitbook/assets/imagen (140).png" alt=""><figcaption></figcaption></figure>

![](<../../../.gitbook/assets/imagen (55).png>)

\- **Contador**: este campo es utilizado para ordenar todas las líneas del pedido. Mantendrán el orden de menor a mayor en la presentación de las rejillas y en los impresos. Se podrá modificar para variar el orden según las necesidades.

![](<../../../.gitbook/assets/imagen (54).png>)

\- **Fecha**: es en la que se produce la **acción**

\- **Documento**: tipo y número de documento que genera la acción (es posible la apertura del documento mostrado con doble clic del ratón o seleccionando y pulsando intro)

\- **Entidad**: la asignada al documento generado por la **acción**

\- **Unidades**: cantidad de artículos por cada **acción**

**Opciones de las líneas de pedido**

\- **Aceptar**: con este botón guardamos los cambios realizados.

\- **Cancelar**: abortamos el alta o modificación de la línea.

\- **Borrar**: eliminamos la línea del pedido.

\- **Tramitar**: activa el pedido de ventas

**PESTAÑAS**

**Estadística:** presenta una rejilla similar a líneas, pero añadiendo los campos costo, beneficio y % de beneficio. Además, añade botones en la parte inferior para aumentar el % de beneficio sobre el mostrado en la línea seleccionada y para modificar el incremento sobre el costo mostrado.

**Totales**: presenta el desglose de importe totales del pedido de material:

<figure><img src="../../../.gitbook/assets/imagen (151).png" alt=""><figcaption></figcaption></figure>

**Observaciones**: aquí podremos anotar todas las notas que necesitemos relativas al pedido de material.

**Archivos**: permite almacenar en el servidor cualquier tipo de archivo para su apertura en remoto. [Véase "Archivos"](../../maestros/articulos/ficha-del-articulo/archivos.md)

**Seguimientos**: añade asuntos a la agendas de los usuarios para el control del documento, permitiendo en ésta añadir avisos a horas programables.

**Email**: control de correos electrónicos enviados o no enviados generados desde el botón "Crear Email":

![](<../../../.gitbook/assets/imagen (57).png>)

**SMS:** pestaña que muestra los SMS enviados al cliente referentes al pedidos de ventas (si se completa o de forma manual), indicando fecha y hora, teléfono / entidad, mensaje y estado de entrega.

**Auditoría**: control de las modificaciones por usuario y evento

**Acciones**: control de acciones sobre el documento en función de qué, quién y cuándo se ha realizado.

**Opciones desde un pedido de material**

**Guardar:** si pulsamos esta opción, quedarán guardados todos los cambios que hayamos realizado sobre la ficha del pedido

**Eliminar:** si pulsamos este botón y pedido no tiene ninguna unidad recibida o reservada, lo eliminaremos. De lo contrario, el botón se desactivará.

**Imprimir:** botón utilizado para imprimir el pedido valorado o sin valorar. Se nos preguntará el modo de impreso al pulsarlo. Si la situación del pedido es pendiente, ésta cambiará a ser tramitado.

**Crear E-mail:** también podremos enviar el pedido por correo electrónico. Si pulsamos esta opción, el programa creará un correo electrónico adjuntando un fichero de texto con el contenido del pedido. La dirección de correo del destinatario será por defecto la definida en la ficha del proveedor, aunque se podrá modificar antes de ser enviado el correo. Para poder enviarlo, tendremos que hacerlo desde nuestra bandeja de salidas de correos electrónicos. Al igual que con la opción imprimir, la situación del pedido pasará a tramitada, si la situación actual del pedido es pendiente.

**Entregar**: muestra un formulario de unidades entregables a fin de entregarlas al cliente generando un albarán de ventas

**Anticipo**: permite recibir anticipos de pagos (sólo entidades no genéricas - no cliente contado o mostrador sin CIF) asociados al pedido de ventas

**SMS**: permite enviar un SMS predefinido (similar al que se genera a la recepción del material pedido por compras) y que es editable en todo su contenido:

<figure><img src="../../../.gitbook/assets/imagen (131).png" alt=""><figcaption></figcaption></figure>

**2 - BUSCAR**

Localizador de pedidos de material a través de distintos criterios. Nos permite consultar, borrar o modificar la información de un pedido. Al acceder a esta opción encontraremos la siguiente pantalla:

Este localizador nos permite buscar un pedido por los siguientes criterios:

* **Número de documento:** el cursor se irá situando en el pedido cuyo número coincida con el seleccionado.
* **Fecha:** el cursor se irá situando en el primer pedido cuya fecha coincida con la seleccionada.
* **Referencia:** el cursor se irá situando en el pedido cuya referencia coincida con la seleccionada.
* **Nombre de entidad:** el cursor se irá situando en el pedido cuya razón social vaya coincidiendo con lo introducido en el campo de edición.

<figure><img src="../../../.gitbook/assets/imagen (154).png" alt=""><figcaption></figcaption></figure>

Para acceder a la ficha del pedido seleccionado, se puede hacer doble clic sobre él o seleccionar la línea y teclear el botón intro del teclado.

El formulario que se presenta es el mismo que el de grabación.

**3 - LISTADO**

Esta opción lanza una búsqueda que nos presentará un listado de pedidos. Este listado se puede acotar a través del filtro de búsqueda que se presenta a continuación:

<figure><img src="../../../.gitbook/assets/imagen (134).png" alt=""><figcaption></figcaption></figure>

Después de indicar los criterios deseados, nos aparecerá una rejilla con todos los pedidos que los cumplan. La rejilla presentada es similar a la del menú:

<figure><img src="../../../.gitbook/assets/imagen (148).png" alt=""><figcaption></figcaption></figure>

**4 - ENTREGAR MATERIAL**

Mediante esta opción, podremos sacar un listado de todas las líneas de pedidos pendientes por un determinado cliente y serie de pedido de ventas:

<figure><img src="../../../.gitbook/assets/imagen (138).png" alt=""><figcaption></figcaption></figure>

Y a continuación la rejilla con información sobre la recepción y reparto de las unidades reservadas de stock, pendientes de entregar, stock actual, entregadas ahora, importe, artículo, cliente y pedido:

<figure><img src="../../../.gitbook/assets/imagen (133).png" alt=""><figcaption></figcaption></figure>

En la rejilla anterior es posible seleccionar varios pedidos y crear albaranes para entregar, así como mostrar los pedidos relacionados.

**5 - MATERIAL PENDIENTE DE ENTREGAR**

Muestra un listado de los artículos pendientes de entregar por cliente con campos diferentes al punto 4:

<figure><img src="../../../.gitbook/assets/imagen (139).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/imagen (6).png" alt=""><figcaption></figcaption></figure>
