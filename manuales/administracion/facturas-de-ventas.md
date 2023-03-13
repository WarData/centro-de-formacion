# Facturas de gastos

Accederemos con esta opción al menú de facturas de gastos, donde podremos grabar, modificar o consultar todas las facturas de gastos recibidas de nuestros acreedores. El menú contiene un calendario mediante el que podremos ver las facturas del día seleccionado, una serie de opciones, y una rejilla en la que se presentan las facturas del día seleccionado.

<figure><img src="../../.gitbook/assets/imagen (20) (1).png" alt=""><figcaption></figcaption></figure>

**1 – NUEVA FACTURA**

Permite dar de alta a una nueva factura de gastos mediante el siguiente formulario:

<figure><img src="../../.gitbook/assets/imagen (17).png" alt=""><figcaption></figcaption></figure>

Están compuestos por su cabecera, donde se guardan todos los datos generales de la factura, y las líneas, donde se va a guardar el detalle de la factura. Dependiendo de la serie de la factura, el contenido de ella será diferente. Definiremos el tipo de factura en la [serie de los documentos](../configuracion/series-de-documentos.md) de facturas de gastos.

La cabecera de las facturas de gastos está compuesta por los siguientes campos:

* **Serie de documento:** campo para indicar la serie a la que pertenecerá la factura. Mediante la serie indicaremos al programa el tipo de factura que estamos grabando.
* **Número:** todos los documentos están clasificados por su serie y un número, que siempre será por defecto el siguiente al último grabado de la misma serie. Tanto el número como la serie de un documento se podrán modificar manualmente, aunque, a menos que sea imprescindible, no es aconsejable.
* **Fecha recepción:** se indica aquí la fecha de grabación del documento. Esta fecha debe de estar dentro de los rangos definidos en parámetros.
* **Fecha Emisión:** podremos indicar aquí la fecha de emisión del documento. La fecha contable se podrá elegir en el momento del traspaso a contabilidad. Donde podremos seleccionar la fecha de grabación, o la de origen.
* **Acreedor:** mediante este campo podremos seleccionar un acreedor, localizarlo, editar el seleccionado o incluso modificar el seleccionado editando sus datos desde la siguiente opción (sólo válido para el documento generado, no modifica la ficha):

<figure><img src="../../.gitbook/assets/imagen (14) (1).png" alt=""><figcaption></figcaption></figure>

* **Nombre, tipo de pago y vencimientos:** muestra, respectivamente, el nombre, tipo de pago y vencimientos del acreedor seleccionado. Se podrán modificar sin que estos cambios afecten a la ficha. Recordar que tanto el tipo de pago como los vencimientos son campos relacionados con su propia tabla de datos en las que se graban las diferentes posibilidades que se pueden escoger. El acceso a estas dos tablas, lo podrás encontrar en el apartado **Submaestros > Administración >** [**Tipos de pago**](../submaestros/administracion-1/tipos-de-pago.md) **y** [**Vencimientos**](../submaestros/administracion-1/vencimientos.md)****
* **Referencia:** podemos guardar en este campo el código o referencia de la factura que nos ha emitido el acreedor.
* **Centro:** este campo solo será visible por aquellas aplicaciones en las que se trabaje con más de un centro de trabajo y así se haya indicado en parámetros. Se utiliza para indicar el centro de trabajo para el que se graba la factura. Este campo, se rellena automáticamente y solo será manipulable por aquellos usuarios autorizados.
* **Régimen de IVA:** este campo tomará por defecto el régimen de IVA definido en la ficha del acreedor. Se podrá modificar manualmente.
* **Régimen:** Por defecto tomará el régimen general R1 para aquellos proveedores que sean sociedades. El cálculo de los impuestos será diferente en cada caso.
* **Añadir Albarán de gastos**: indicamos aquí el albarán de gastos a facturar. Podremos utilizar los botones incrustados a este campo para localizar un albarán no facturado o editar el seleccionado. El campo **fecha** presentado a la derecha del albarán seleccionado no es editable y presentará la fecha de grabación del albarán.
* **Desfacturar Albarán**: una vez eliminado el apunte de tesorería (pago), podremos abrir la factura para modificarla, pudiendo llegar a vaciarla "desfacturando" para incorporar una modificación del albarán de compras añadido inicialmente.
* **Número de orden (referente a líneas de la rejilla en "detalle")**: este campo sirve para ordenar las líneas tanto en las rejillas como cuando se imprime la factura.
* **Bases IVA**: el programa tomará por defecto los importes definidos en la ficha del vehículo o del concepto. Se podrán modificar manualmente.
* **Total base, total IVA** y **total línea**

**Barra de pestañas**

* **Detalle:** presenta la rejilla que corresponde en función del tipo de factura que estemos grabando. Mediante está rejilla podremos consultar, grabar, modificar o eliminar cualquier línea de factura. Al hacer doble click sobre cualquier línea vacía o pulsar el botón del lateral izquierdo "Nueva línea de servicio" se nos presentará el formulario de grabación de líneas correspondiente a cada tipo de factura:

<figure><img src="../../.gitbook/assets/imagen (3) (1) (5).png" alt=""><figcaption></figcaption></figure>

* **Pagos**: en esta pestaña se visualizará la rejilla de apuntes cuando el tipo de pago sea contado, o la de recibos de pago para tipos de pago aplazados. La creación de los apuntes o recibos se realizará automáticamente cuando así se indique en el tipo de pago, o manualmente. También se podrán realizar manualmente grabándolos directamente desde la rejilla o mediante los botones rehacer pagos o pago directo. La opción de rehacer pagos, eliminará los que ya se hayan creado y los volverá a crear de nuevo. Y la opción de pago directo, presentará el formulario de alta de apuntes para grabarlos manualmente:

<figure><img src="../../.gitbook/assets/imagen (8) (5).png" alt=""><figcaption></figcaption></figure>

* **Totales**: muestra la información totalizada de bases, porcentajes de IVA, importe de IVA y parciales, así como importe pagado y pendiente si es que han existido anticipos de pago asociados al documento:

<figure><img src="../../.gitbook/assets/imagen (4) (1) (6).png" alt=""><figcaption></figcaption></figure>

* **Observaciones**: permite añadir texto libre que únicamente aparecerá en este documento. Es posible imprimir el contenido en los informes de impresión indicándolo al departamento de soporte (es posible que la realización incluya costes de programación)
* **Archivos**: permite almacenar en el servidor cualquier tipo de archivo para su apertura en remoto [(véase "Archivos")](../maestros/articulos/ficha-del-articulo/archivos.md)

![](<../../.gitbook/assets/imagen (44).png>)

**Opciones de las líneas de facturas de gastos:**

* **Aceptar**: con este botón guardamos los cambios realizados.
* **Cancelar**: omite y cancela la modificación de la línea aunque se haya realizado algún cambio
* **Eliminar**: si la factura no está contabilizada, se podrá borrar la línea mediante este botón. Si está pagada habrá que eliminar el pago desde la pestaña "Pagos".
* **Auditoría**: muestra el momento y usuario que creó y/o modificó la línea

<figure><img src="../../.gitbook/assets/imagen (10) (1) (2).png" alt=""><figcaption></figcaption></figure>

**Opciones desde una factura de gastos:**

* **Aceptar:** si pulsamos esta opción, quedarán guardados todos los cambios que hayamos realizado sobre la ficha de la factura
* **Eliminar**: borrará completamente la factura (no debe tener pagos).
* **Cerrar factura**: se darán de alta los asientos en contabilidad y la factura no se podrá modificar

<figure><img src="../../.gitbook/assets/imagen (1) (1) (5).png" alt=""><figcaption></figcaption></figure>

**2 - BUSCAR FACTURA**

Localizador de facturas de gastos a través de distintos criterios. Nos permite consultar, borrar o modificar la información de una factura. Al acceder a esta opción encontraremos la siguiente pantalla:

<figure><img src="../../.gitbook/assets/imagen (16) (1).png" alt=""><figcaption></figcaption></figure>

Este localizador nos permite buscar una factura por los siguientes criterios:

* **Número de documento:** el cursor se irá situando en la factura cuyo número coincida con el seleccionado.
* **Fecha:** el cursor se irá situando en la factura cuya fecha coincida con la seleccionada.
* **Referencia:** el cursor se irá situando en la factura cuya referencia del mismo campo vaya coincidiendo con la introducida en el campo de edición.
* **Nombre entidad:** el cursor se irá situando en la factura cuya razón social vaya coincidiendo con lo introducido en el campo de edición.

Para acceder a la ficha de la factura seleccionada, se puede hacer doble clic sobre ella o, una vez seleccionada, pulsar el botón intro del teclado.

El formulario que se presenta es el mismo que el de grabación.

**3 – LISTADO GENERAL**

Permite obtener un listado de facturas por varios filtros como serie, ejercicio, fechas de recepción y emisión, entidad, tipo de pago, estado de pago, régimen de IVA y país:

<figure><img src="../../.gitbook/assets/imagen (2) (1) (5).png" alt=""><figcaption></figcaption></figure>

La información de**l** listado se presenta en las siguientes rejillas. Cada una de ellas, tiene asociado un informe que se podrá sacar por impresora:

<figure><img src="../../.gitbook/assets/imagen (5) (1) (3).png" alt=""><figcaption></figcaption></figure>

**4 – LISTADO DE IVA**

Muestra un listado de facturas para IVA por intervalo de fechas con las bases e impuestos desglosados. Presenta el siguiente formulario de búsqueda:

<figure><img src="../../.gitbook/assets/imagen (19) (1).png" alt=""><figcaption></figcaption></figure>

La información de**l** listado se presenta en las siguientes rejillas. Cada una de ellas, tiene asociado un informe que se podrá sacar por impresora:

<figure><img src="../../.gitbook/assets/imagen (18) (1).png" alt=""><figcaption></figcaption></figure>

* Revisión: permite controlar la contabilización de las facturas mostradas
* Exportación a Excel: realiza la exportación a un fichero Excel
* Listado IVA: imprime el listado mostrado
* Listado comprobación: imprime la verificación contabilizado o no
