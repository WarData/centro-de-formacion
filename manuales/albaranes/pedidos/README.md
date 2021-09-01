# Pedidos

**PEDIDOS DE COMPRAS**

Mediante esta opción, podremos grabar, modificar o consultar todos los pedidos que hemos realizado a nuestros proveedores. Al entrar en ella, nos aparece un menú en el que se nos presentan opciones para crear un nuevo pedido, buscar uno ya creado, sacar listados de pedidos y consultar las unidades pendientes de recibir de un determinado artículo. Además de estas opciones, podemos ver una rejilla con todos los pedidos en curso, con al menos una referencia pendiente de recibir.

**1 - NUEVO PEDIDO**

Permite dar de alta un nuevo pedido de material rellenando el siguiente formulario. Un pedido está compuesto por la cabecera, donde se introducen los datos generales del pedido, como la serie, la fecha o proveedor, y las líneas, donde se va grabando en cada una de ellas la referencia y la cantidad que se va a pedir.

La imagen anterior nos muestra un formulario de pedidos de material, donde se graban tanto los datos generales, como las líneas con las referencias a pedir. La cabecera de un pedido está compuesta por los siguientes campos:

* **Serie:** es un campo imprescindible de rellenar, y por defecto toma el valor definido en los parámetros del programa. Podemos utilizarlo para clasificar diferentes tipos de pedidos, como por ejemplo, serie B para pedidos de boutique y R para recambios. Además, en las series de los documentos se pueden definir distintas características que tomará el pedido por defecto, entre ellas, se puede indicar que calcule los impuestos, lo que significa que el pedido llevará calculado en sus bases el impuesto correspondiente.



* **Número:** todos los documentos están clasificados por su serie y un número, que siempre será por defecto el siguiente al último grabado de la misma serie. Tanto el número como la serie de un documento se podrán modificar manualmente, aunque, a menos que sea imprescindible el cambio, no es aconsejable.



* **Fecha:** se indica aquí la fecha de grabación del documento. Esta fecha debe de estar dentro de los rangos definidos en parámetros.



* **Situación:** este campo no es manipulable por el usuario, y nos indica la situación del pedido. Esta puede ser, PENDIENTE TRAMITAR, nos indica que todas las referencias solicitadas aún están pendiente de recibir y tramitar, TRAMITADO, indica que el pedido ha sido solicitado al proveedor y el documento pasará a esta situación si se imprime, envía por e-mail o se genera el fichero correspondiente para tramitarlo mediante algún método utilizado por el proveedor, INCOMPLETO, indica que se ha recibido parte del pedido, RECIBIDO, indica que todas las referencias han sido recibidas.



* **Referencia:** se puede anotar aquí la referencia del pedido del proveedor.



* **Centro:** este campo solo será visible por aquellas aplicaciones en las que se trabaje con más de un centro de trabajo y así se haya indicado en parámetros. Se utiliza para indicar el centro de trabajo para el que se hace el pedido. Este campo, se rellena automáticamente y solo será manipulable por aquellos usuarios autorizados.



* **Tipo de pedido:** se indica aquí si el pedido es de reposición, urgente, campaña o garantía.



* **Proveedor:** indicamos aquí el proveedor al que vamos a realizar el pedido. Y mediante botón insertado en el campo del código del proveedor, podremos localizarlo, grabar uno nuevo o modificar el seleccionado. Además, podremos cambiar los datos del proveedor seleccionado en este pedido a través de los campos situados justo debajo del código del proveedor. Estos campos solo afectarán a este pedido y no se cambiará la ficha del proveedor.



* **SUMA DE BASES:** presenta la suma total de las bases de las líneas del pedido. No es un campo manipulable por el usuario.



* **SUMA IVA:** en este campo se acumula el importe de IVA de las líneas.



* **TOTAL:** presenta el importe total del pedido, con IVA incluido.

**Barra de pestañas**

* **LÍNEAS:** contiene una rejilla en la que se nos presentan las líneas de pedidos de material ordenadas por el campo contador de cada línea. Mediante está rejilla podremos consultar, grabar, modificar o eliminar cualquier línea de pedido.

Para grabar una nueva línea de pedido, podemos utilizar cualquiera de los métodos utilizados sobre cualquier otra rejilla. Se nos presentará el formulario de grabación de líneas con los siguientes campos:

            - **Almacén**: indicamos aquí el almacén para el cual estamos realizando el pedido.

            - **Artículo**: campo en el que introducimos la referencia del artículo que vamos a pedir. Se podrá meter la referencia manualmente, o utilizando la opción Buscar Artículo de los  botones incrustados de este campo. Una vez asignado el pedido no se puede cambiar el artículo pero si podemos ver su ficha, en el botón que se encuentra al lado del nombre.

Si no localizamos la referencia en la base de datos de artículos, podemos utilizar la opción Referencia.

Con esta opción, el programa buscará en primer lugar en el fichero de artículos, y si no la encontrara, buscará en el de tarifas. Una vez localizada, se nos presentará el siguiente formulario, desde el que podremos crear la referencia directamente.

Los otros dos botones incrustados que contiene el campo de artículo, son para consultar/editar la referencia seleccionada, o para crear una nueva.

La descripción del artículo tomará por defecto la definida en su ficha, pero podrá ser modificada manualmente.

            - **Unidades pedidas**: campo para insertar las unidades que solicitamos al proveedor.

            - **Unidades recibidas**: nos es un campo manipulable por el usuario, y nos presenta las unidades que hemos recibido.

            - **Unidades rectificadas**: este campo podrá ser utilizado para anular unidades pendientes de recibir del proveedor y que ya vayamos a recibirlas.

            - **Unidades pendientes**: unidades pendientes de recibir \(unidades pedidas, menos las recibidas y menos las rectificadas\).

            - **Precio**: importe del artículo.

            - **Descuento 1 y descuento 2**: podremos indicar hasta dos descuentos en las líneas de pedidos.

            -          **Parcial**: valor total del artículo \(sin sumar los impuestos\) resultante de multiplicar las unidades pedidas por el precio menos los descuentos.

            -          **Asignaciones**: es una rejilla en la que podemos ver si las unidades pedidas en esta línea han sido reservadas por algún cliente o agente.

            -          **Contador**: este campo es utilizado para ordenar todas las líneas del pedido. Mantendrán el orden de menor a mayor en la presentación de las rejillas y en los impresos. Se podrá modificar para variar el orden según las necesidades.

            -          **Recibida**: indica si la línea está totalmente recibida o no.

**Opciones de las líneas de pedido**

            -          **Aceptar**: con este botón guardamos los cambios realizados.

            -          **Cancelar**: abortamos el alta o modificación de la línea.

            -          **Borrar**: eliminamos la línea del pedido.

**-TOTALES:** presenta el desglose de importe totales del pedido de material.

**-NOTAS:** aquí podremos anotar todas las notas que necesitemos relativas al pedido de material.

**Opciones desde un pedido de material**

**Aceptar:** si pulsamos esta opción, quedarán guardados todos los cambios que hayamos realizado sobre la ficha del pedido.

**Cancelar:** con este botón, saldremos de la ficha del pedido sin guardar los posibles cambios que hayamos realizado. Se puede pulsar la tecla ESC para ejecutar esta opción.

**Borrar:** si pulsamos este botón y pedido no tiene ninguna unidad recibida o reservada, lo eliminaremos. De lo contrario, el botón se desactivará.

**Imprimir:** botón utilizado para imprimir el pedido valorado o sin valorar. Se nos preguntará el modo de impreso al pulsarlo. Si la situación del pedido es pendiente, ésta cambiará a ser tramitado.

**E-mail:** también podremos enviar el pedido por correo electrónico. Si pulsamos esta opción, el programa creará un correo electrónico adjuntando un fichero de texto con el contenido del pedido. La dirección de correo del destinatario será por defecto la definida en la ficha del proveedor, aunque se podrá modificar antes de ser enviado el correo. Para poder enviarlo, tendremos que hacerlo desde nuestra bandeja de salidas de correos electrónicos. Al igual que con la opción imprimir, la situación del pedido pasará a tramitada, si la situación actual del pedido es pendiente.

**Fichero Honda, Suzuki, Harley o Kawasaki:** dependiendo del proveedor, el programa emite, hasta el momento, cuatro  tipos de ficheros diferentes con el contenido del pedido. Este fichero, podrá ser utilizado posteriormente, para tramitar el pedido directamente a nuestro proveedor utilizando el método que él le facilite \(FTP, vía Web, E-mail, intranet, etc.\)

El fichero se guardará en la ruta indicada en los parámetros del programa. Además de esta ruta, para poder utilizar este sistema, será necesario configurar otros parámetros correspondientes al sistema de cada proveedor.

**Recibir:** pulsando este botón, accederemos a una pantalla para poder crear los albaranes de recepción de la mercancía, recibir las unidades solicitadas. Se nos presentará la siguiente pantalla, y a continuación se describen las diferentes opciones que podemos realizar desde ella.

Esta rejilla es multi-selección, y contiene, en la parte de inferior, tres botones que actuarán sobre las líneas seleccionadas. Todas estas líneas, corresponden a aquellas con unidades pendientes de recibir.

Podremos modificar las unidades que recibimos en este momento haciendo doble click en la línea deseada. El campo cantidad a recibir comenzará a parpadear y podremos modificar la cantidad \(siempre deberá se inferior o igual a lo pendiente de recibir\).

Con el primero de los tres campos, daremos por recibidas las líneas seleccionadas, creando así el albarán correspondiente.

Con el segundo, sustituir referencia seleccionada, podremos modificar la referencia que inicialmente habíamos pedido por la que realmente hayamos recibido. Estos casos se pueden dar por ejemplo cuando se ha pedido una referencia obsoleta, y el proveedor nos envía la que le sustituye. Otro caso puede ser, que el proveedor, al no tener en stock de la referencia solicitada, nos envíe otra de similares características.

Y con el tercer botón, podremos visualizar los documentos origen de las líneas seleccionadas \(reservas\).

**Zoom:** botón para visualizar las líneas de pedidos en una pantalla más amplia.

**Rectificar unidades pendientes:** botón utilizado para anular todas las unidades pendientes de recibir. El pedido pasará a situación Servido.

2 - BUSCAR

Localizador de pedidos de material a través de distintos criterios. Nos permite consultar, borrar o modificar la información de un pedido. Al acceder a esta opción encontraremos la siguiente pantalla:

Este localizador nos permite buscar un pedido por los siguientes criterios:

**-FECHA:** el cursor se irá situando en el primer pedido cuya fecha coincida con la seleccionada.

**-NOMBRE PROVEEDOR:** el cursor se irá situando en el pedido cuya razón social vaya coincidiendo con lo introducido en el campo de edición.

**-SU REFERENCIA:** el cursor se irá situando en el pedido cuya referencia coincida con la seleccionada.

**-PROVEEDOR:** el cursor se irá situando en el pedido cuyo código de proveedor coincida con el seleccionado.

**-NÚMERO:** el cursor se irá situando en el pedido cuyo número coincida con el seleccionado.

Para acceder a la ficha del pedido seleccionado, se puede hacer doble clic sobre él, pulsar el botón SELEC., o teclear el botón intro del teclado.

El formulario que se presenta es el mismo que el de grabación.

3 - LISTAR

Esta opción lanza una búsqueda que nos presentará un listado de pedidos. Este listado se puede acotar a través del filtro de búsqueda que se presenta a continuación.

Después de indicar los criterios deseados, nos aparecerá una rejilla con todos los pedidos que los cumplan. La rejilla presentada es similar a la del menú.

4 - PENDIENTES

Mediante esta opción, podremos sacar un listado de todas las líneas de pedidos pendiente por un determinado artículo. Se lanzará una búsqueda en cuyo filtro se no pide el artículo del que queremos sacar el listado

Y a continuación una rejilla con información de las unidades pendientes, recibidas, fecha, número de pedido, etc.

