# Facturas

Accederemos con esta opción al menú de facturas de compras, donde podremos grabar, modificar o consultar todas las facturas de compras recibidas de nuestros proveedores. El menú contiene un calendario mediante el que podremos ver las facturas del día seleccionado, una serie de opciones, y una rejilla en la que se presentan las facturas del día seleccionado.

**1 – NUEVA FACTURA**

Permite dar de alta a una nueva factura de compra mediante el siguiente formulario:

![](../../.gitbook/assets/imagen%20%2826%29.png)

Están compuestos por su cabecera, donde se guardan todos los datos generales de la factura, y las líneas, donde se va a guardar el detalle de la factura. Dependiendo de la serie de la factura, el contenido de ella será diferente. Puede haber hasta 3 posibles tipos de facturas de compras, de recambios, que utilizaremos para  facturar los albaranes de compras o garantías, de vehículos nuevos y de vehículos de ocasión, en las que facturaremos todos los vehículos y posibles conceptos. Definiremos el tipo de factura en la [serie de los documentos](../configuracion/series-de-documentos.md) de facturas de compras.

La cabecera de las facturas de compras está compuesta por los siguientes campos:

* **Serie de documento:** campo para indicar la serie a la que pertenecerá la factura. Mediante la  serie indicaremos al programa el tipo de factura que estamos grabando \(recambios, vehículos nuevos o vehículos de ocasión\).



* **Número:** todos los documentos están clasificados por su serie y un número, que siempre será por defecto el siguiente al último grabado de la misma serie. Tanto el número como la serie de un documento se podrán modificar manualmente, aunque, a menos que sea imprescindible, no es aconsejable.



* **Fecha recepción:** se indica aquí la fecha de grabación del documento. Esta fecha debe de estar dentro de los rangos definidos en parámetros.



* **Fecha Emisión:** podremos indicar aquí la fecha de emisión del documento. La fecha contable se podrá elegir en el momento del traspaso a contabilidad. Donde podremos seleccionar la fecha de grabación, o la de origen.



* **Proveedor:** mediante este campo podremos seleccionar un proveedor, localizarlo, editar el seleccionado o incluso crear un proveedor importando los datos de su ficha de cliente. Esta última opción la lanzaremos mediante el botón incrustado cliente, nos aparecerá un formulario para seleccionar el cliente desde el que importaremos los datos, y el programa creará automáticamente la ficha del nuevo proveedor \(la ficha de cliente seguirá existiendo\).



* **Nombre, tipo de pago y vencimientos:** muestra, respectivamente, el nombre, tipo de pago y vencimientos del proveedor seleccionado. Se podrán modificar sin que estos cambios afecten a la ficha del proveedor. Recordar que tanto el tipo de pago como los vencimientos son campos relacionados con su propia tabla de datos en las que se graban las diferentes posibilidades que se pueden escoger. El acceso a estas dos tablas, lo podrás encontrar en el apartado Submaestros del menú principal



* **Referencia:** podemos guardar en este campo el código o referencia de la factura que nos ha emitido el proveedor.



* **Centro:** este campo solo será visible por aquellas aplicaciones en las que se trabaje con más de un centro de trabajo y así se haya indicado en parámetros. Se utiliza para indicar el centro de trabajo para el que se graba la factura. Este campo, se rellena automáticamente y solo será manipulable por aquellos usuarios autorizados.



* **Régimen de IVA:** este campo tomará por defecto el régimen de IVA definido en la ficha del proveedor seleccionado en el albarán. Se podrá modificar manualmente.



* **Régimen:** este campo solo será visible para las facturas de vehículos de ocasión, e indicaremos si el tipo de compra se rige por el régimen general o especial de vehículos usados. Por defecto tomará el régimen general para aquellos proveedores que sean sociedades. El cálculo de los impuestos será diferente en cada caso.



* **Documentaciones:** solo será visible para las facturas de vehículos, y en él podemos indicar donde se encuentra su documentación.



* **Añadir Albarán de compra**: indicamos aquí el albarán de compra a facturar. Podremos utilizar los botones incrustados a este campo para localizar un albarán no facturado o editar el seleccionado. El campo **fecha** presentado a la derecha del albarán seleccionado no es editable y presentará la fecha de grabación del albarán.



* **Desfacturar Albarán**: una vez eliminado el apunte de tesorería \(pago\), podremos abrir la factura para modificarla, pudiendo llegar a vaciarla "desfacturando" para incorporar una modificación del albarán de compras añadido inicialmente.



* **Número de orden \(referente a líneas de la rejilla en "detalle"**: este campo sirve para ordenar las líneas tanto en las rejillas como cuando se imprime la factura.



* **Grabación de líneas de vehículos nuevos o de ocasión**: en estas líneas podremos indicar el vehículo o concepto que se va a facturar. Los campos que se nos presentan son:



* **Concepto**: mediante este campo, podemos facturar un concepto relacionado con un determinado bastidor. Para ello indicaremos además del concepto el bastidor con el que lo relacionaremos.



* **Bastidor**: indicaremos aquí el bastidor que vamos a facturar. Debe de haber grabado un albarán de entrada de vehículos del bastidor que vamos facturar anteriormente. De lo contrario, nos saltará un aviso y no podremos facturarlo.



* **Matrícula**: campo no editable por el usuario que presenta la matrícula del vehículo seleccionado, si la tuviera.



* **Nombre del concepto**: este campo tomará por defecto el nombre del concepto seleccionado o del bastidor. Se podrá manipular manualmente.



* **Bases IVA**: el programa tomará por defecto los importes definidos en la ficha del vehículo o del concepto. Se podrán modificar manualmente.



* **Total base, total IVA** y **total línea**

\*\*\*\*

**Barra de pestañas**

\*\*\*\*

* **Detalle:** presenta la rejilla que corresponde en función del tipo de factura que estemos grabando. En el caso de las facturas de recambios, nos presentará los documentos origen que componen la factura, y en las de vehículos nuevos u ocasión, los bastidores que se están facturando pero con diferentes rejillas. Mediante está rejilla podremos consultar, grabar, modificar o eliminar cualquier línea de factura. Al hacer doble click sobre cualquier línea vacía o pulsar el botón del lateral izquierdo "Nueva línea de artículo o concepto" se nos presentará el formulario de grabación de líneas correspondiente a cada tipo de factura:

                ·    Grabación de líneas de recambios: en estas líneas podremos indicar los       documentos origen que compondrán la factura. Estos pueden ser albaranes de compras, garantías, órdenes de garantías, promociones o bonificaciones / penalizaciones de documentaciones. Los campos que la componen son los siguientes:

* **Pagos**: en esta pestaña se visualizará la rejilla de apuntes cuando el tipo de pago sea contado, o la de recibos de pago para tipos de pago aplazados. La creación de los apuntes o recibos se realizará automáticamente cuando así se indique en el tipo de pago, o manualmente. También se podrán realizar manualmente grabándolos directamente desde la rejilla o mediante los botones rehacer pagos o pago directo. La opción de rehacer pagos, eliminará los que ya se hayan creado y los volverá a crear de nuevo. Y la opción de pago directo, presentará el formulario de alta de apuntes para grabarlos manualmente.



* **Totales**: muestra la información totalizada de bases, porcetajes de IVA, importe de IVA y parciales, así como importe pagado y pendiente si es que han existido anticipos de pago asociados al documento.



* **Observaciones**: permite añadir texto libre que únicamente aparecerá en este documento. Es posible imprimir el contenido en los informes de impresión indicándolo al departamento de soporte \(es posible que la realización incluya costes de programación\)



* **Archivos**: permite almacenar en el servidor cualquier tipo de archivo para su apertura en remoto

![](../../.gitbook/assets/imagen%20%2844%29.png)

**Opciones de las líneas de facturas de compras:**

\*\*\*\*

* **Aceptar**: con este botón guardamos los cambios realizados.



* **Cancelar**: abortamos el alta o modificación de la línea.



* **Eliminar**: si la factura no está contabilizada, se podrá borrar la línea mediante este botón.

**Opciones desde una factura de compras:**

\*\*\*\*

* **Aceptar:** si pulsamos esta opción, quedarán guardados todos los cambios que hayamos realizado sobre la ficha de la factura.



* **Cancelar:** con este botón, saldremos de la ficha de la factura sin guardar los posibles cambios que hayamos realizado. Se puede pulsar la tecla ESC para ejecutar esta opción.



* **Borrar:** el botón solo estará activo si la factura no está contabilizada, y si se pulsa, se borrará completamente la factura.



* **Imprimir:** botón para imprimir una copia de la factura de compras.



**2 - BUSCAR**

Localizador de facturas de compras a través de distintos criterios. Nos permite consultar, borrar o modificar la información de una factura. Al acceder a esta opción encontraremos la siguiente pantalla:

![](../../.gitbook/assets/imagen%20%2857%29.png)

Este localizador nos permite buscar una factura por los siguientes criterios:

* **Número de documento:** el cursor se irá situando en la factura cuyo número coincida con el seleccionado.



* **Fecha:** el cursor se irá situando en la factura cuya fecha coincida con la seleccionada.



* **Referencia:** el cursor se irá situando en la factura cuya referencia del mismo campo vaya coincidiendo con la introducida en el campo de edición.



* **Nombre entidad:** el cursor se irá situando en la factura cuya razón social vaya coincidiendo con lo introducido en el campo de edición.

Para acceder a la ficha de la factura seleccionada, se puede hacer doble clic sobre ella o, una vez seleccionada, pulsar el botón intro del teclado.

El formulario que se presenta es el mismo que el de grabación.

**3 – LISTADO GENERAL**

Permite obtener un listado de facturas por varios filtros como serie, ejercicio, fechas de recepción y emisión, entidad, tipo de pago, estado de pago, régimen de IVA y país:

![](../../.gitbook/assets/imagen%20%2851%29.png)

La información de**l** listado se presenta en las siguientes rejillas. Cada una de ellas, tiene asociado un informe que se podrá sacar por impresora:

![](../../.gitbook/assets/imagen%20%2861%29.png)

**4 – LISTADO DE IVA**

Muestra un listado de facturas para IVA por intervalo de fechas con las bases e impuestos desglosados. Presenta el siguiente formulario de búsqueda:

![](../../.gitbook/assets/imagen%20%2856%29.png)

La información de**l** listado se presenta en las siguientes rejillas. Cada una de ellas, tiene asociado un informe que se podrá sacar por impresora:

![](../../.gitbook/assets/imagen%20%2863%29.png)

* Revisión: permite controlar la contabilización de las facturas mostradas
* Exportación a Excel: realiza la exportación a un fichero Excel
* Listado IVA: imprime el listado mostrado
* Listado comprobación: imprime la verificación contabilizado o no

**5 - CÁLCULO 347 COMPRAS**

Acumula los importes de facturas de compra y gastos por cada entidad:

![Filtro 347 compras](../../.gitbook/assets/imagen%20%2855%29.png)

![](../../.gitbook/assets/imagen%20%2850%29.png)
