# Albaranes

ALBARANES DE VENTA

Mediante esta opción, podremos grabar, modificar o consultar todos los albaranes de venta que hemos realizado. Al entrar en ella, nos aparece un menú con calendario, filtros de facturación y cliente en el que se nos presentan hasta 4 opciones y una rejilla que nos muestra todos los albaranes que hemos realizado en el día seleccionado en el calendario tras pulsación de F5 o el botón Actualizar.

**AÑADIDO NUEVO MENÚ 2.0 DE ALBARANES DE VENTAS**

Se ha hecho un cambio visual y operativo al menú de albaranes de ventas para que sea más intuitivo y con nuevas utilidades para mejorar la navegación del usuario en el programa.

Sustituye el anterior panel de albaranes de ventas, por lo que el acceso es el mismo VENTAS > ALBARANES

![](<../../.gitbook/assets/imagen (7) (2) (1) (1).png>)

El nuevo diseño del panel:

![](<../../.gitbook/assets/imagen (9) (2) (1).png>)

Lo primero que se puede apreciar es el rango de fechas de los albaranes que queremos cargar. Se puede meter manualmente como hasta ahora, pero se ha añadido una nueva utilidad.

![](<../../.gitbook/assets/imagen (6) (2) (1).png>)

&#x20;               Al pulsar el botón del selector de períodos se podrá seleccionar que el rango de fechas sea en un rango fechas fijo como Hoy, Mes o Año. Pero a su vez en No seleccionado se puede seleccionar un rango diferente como por ejemplo desde hoy a 5 días atrás.

![](<../../.gitbook/assets/imagen (5) (2) (1).png>)

Como veremos más adelante **\*\*\*** se podrá guardar como **filtro por defecto** el rango de fechas que más utilicemos para que cuando entremos al panel siempre tenga ese rango de fechas cargado de serie (si no se define como filtro por defecto, la selección de fecha volverá al estado anterior la próxima vez)

También se puede filtrar por Centro y cliente como la serie, el vendedor o si está facturado o no desde la ampliación de filtros.

![](<../../.gitbook/assets/imagen (1) (2) (1) (1).png>)

Una vez se dé a cerrar o recalcular, se cargará con los filtros seleccionados. Dependiendo lo seleccionado se indicará un texto en el propio menú con los filtros extendidos.

![](<../../.gitbook/assets/imagen (118).png>)

En el botón de opciones se podrá buscar, listar o facturar en tanda, además de imprimir, cambiar de vista a una rejilla avanzada o vista en modo bloc.

![](<../../.gitbook/assets/imagen (120) (1).png>)

**\*\*\*** La última opción es la anteriormente mencionada: **Establecer filtro por defecto**. Con esta opción se guardará la búsqueda con los filtros utilizados en ese momento y se cargará de esa forma en los siguientes accesos al menú.

![](<../../.gitbook/assets/imagen (119).png>)

**1 – NUEVO ALBARÁN**

Permite dar de alta a un nuevo albarán de venta rellenando el siguiente formulario. Un albarán está compuesto por la cabecera, donde se introducen los datos generales, como la serie, la fecha o cliente, y las líneas, donde se van grabando las referencias y la cantidad que se pide:

![](<../../.gitbook/assets/imagen (76) (1).png>)

La imagen anterior nos muestra un formulario de albaranes de venta, donde se graban todos los datos. La cabecera está compuesta por los siguientes campos:

* **Serie:** es un campo imprescindible de rellenar, y por defecto toma el valor definido en la ficha del usuario que graba el albarán. Si este no tuviera definida ninguna serie de albarán en su ficha, se tomará la de los parámetros del programa. En la serie del albarán se define, por ejemplo, el almacén que tomará por defecto las líneas del albarán. Todas las posibilidades de las series de documentos se detallan en la sección…explicación de series de documentos.
* **Número:** todos los documentos están clasificados por su serie y un número, que siempre será por defecto el siguiente al último grabado de la misma serie. Tanto el número como la serie de un documento se podrán modificar manualmente, aunque, a menos que sea imprescindible el cambio, no es aconsejable.
* **Fecha:** se indica aquí la fecha de grabación del documento. Esta fecha debe de estar dentro de los rangos definidos en parámetros.
* **Hora:** presenta la hora de grabación del albarán, no es manipulable por los usuarios.
* **Referencia**: campo libre para incluir datos. Un ejemplo puede ser añadir en él nombre y número del cliente en caso de ser el cliente contado (genérico sin NIF o CIF)
* **Centro:** este campo solo será visible por aquellas aplicaciones en las que se trabaje con más de un centro de trabajo y así se haya indicado en parámetros. Se utiliza para indicar el centro de trabajo para el que se hace el albarán. Este campo, se rellena automáticamente y solo será manipulable por aquellos usuarios autorizados.
* **Vendedor:** tomará por defecto el vendedor definido en la ficha del cliente o agente. Se podrá modificar manualmente.
* **Agencia de transportes:** tomará por defecto la agencia definida en la ficha del cliente o agente. Se podrá modificar manualmente.
* **Cliente o Agente:** en los documentos de ventas, se podrá indicar si se está vendiendo a un cliente o a un agente. Hay que recordar que son tablas de datos diferentes y solo se podrá indicar uno de ellos por albarán. Ambos campos contienen botones incrustados para localizar, grabar o editar el cliente o agente seleccionado. Los campos situados justo debajo, presentarán la razón social, saldo, tipo de pago, régimen de IVA, vencimiento y, en caso de estar activado en la serie, vehículo al que se asigna la venta.

\- Si el cliente tiene anticipos activos de alguna operación que haya realizado, se presentará en el campo "Saldo", al igual si tiene alguna deuda saldrá valor en negativo. En la factura, aparecerá un botón "Aplicar anticipo" que mostrará una ventana con los anticipos disponibles indicando la cantidad que se aplicará.

* **Documento acreditativo:** si el cliente es intracomunitario, y tiene documento acreditativo, se presentarán los campos relativos a este documento en esta pantalla. Si fuera intracomunitario y no tuviera documento acreditativo, saltará un mensaje indicándolo.
* **Tipo de IVA:** este campo tomará por defecto el tipo de IVA definido en la ficha del cliente o del agente seleccionado en el albarán. Se podrá modificar manualmente. Los diferentes tipos de IVA y de exentos, se explican en la sección proveedores – tipos de IVA.
* **Departamento interno:** si la serie del albarán es INTERNA, se podrá seleccionar el departamento para el que se graba dicho albarán.
* **Observaciones:** campo para introducir observaciones relacionadas con el albarán. Se podrá configurar para que salgan en el impreso, aunque por defecto no se imprime.
* **Tipo de pago 1 y 2, vencimientos e importes:** un albarán de venta podrá tener hasta 2 tipos de pago diferentes. En ese caso, habrá que utilizar los campos **IMP** situados justo a la derecha de cada tipo de pago, para indicar el importe que corresponde a cada tipo. Cuando el albarán corresponde a un cheque regalo, el tipo de pago tomará por defecto modelo VALE.
* **Dto:** en este campo se guarda el importe de descuento calculado a través de un formulario que nos pedirá el porcentaje cuando pulsemos el botón correspondiente. El descuento se calculará sobre la base del albarán.
* **Portes:** valor de los portes del albarán. Para grabar el dato, tendremos que pulsar sobre el botón portes, e introducir el importe.
* **Total IVA incluido:** presenta el importe total de pedido con impuesto incluido.

**Barra de pestañas**

* **CONCEPTOS:** contiene una rejilla en la que se nos presentan las líneas de albaranes de venta ordenadas por el campo contador de cada línea. Mediante está rejilla podremos consultar, grabar, modificar o eliminar cualquier línea de albarán.

Para grabar una nueva línea, podemos utilizar cualquiera de los métodos utilizados sobre cualquier otra rejilla. Se nos presentará el formulario de grabación de líneas con los siguientes campos:

\- **Almacén**: indicamos aquí el almacén del que saldrá el material. Estará activo si la serie tiene marcado que permite varios almacenes. De lo contrario, tomará por defecto el almacén definido en la serie.

\- **Artículo**: campo en el que introducimos la referencia del artículo. Se podrá meter la referencia manualmente, o utilizando la opción Buscar Artículo de los botones incrustados de este campo.

Si no localizamos la referencia en la base de datos de artículos, podemos utilizar la opción Referencia.

Con esta opción, el programa buscará en primer lugar en el fichero de artículos, y si no la encontrara, buscará en el de tarifas. Una vez localizada, se nos presentará el siguiente formulario, desde el que podremos crear la referencia directamente.

Los otros dos botones incrustados que contiene el campo de artículo, son para consultar/editar la referencia seleccionada, o para crear una nueva.

La descripción del artículo tomará por defecto la definida en su ficha, y solo se podrá modificar si el artículo no está incluido en la tarifa.

\- **Stock disponible, ubicaciones y descuento**: son campos que muestran información directa del artículo, el stock disponible, las ubicaciones del artículo y el descuento de compra.

\- **Cantidad**: indicamos aquí las unidades que vayan a salir.

\- **Precio**: importe de venta del artículo. En los presupuestos, pedidos, albaranes de venta y en las órdenes de reparación, tanto el precio de venta como el descuento se calcularán en función a la tabla de descuento definida en el vendedor, y si no tuviera, la definida en el cliente. El funcionamiento específico de las tablas de descuentos se explicarán en el menú comercial, opción B – tablas de descuentos. Si no se hubiera indicado ninguna tabla de descuentos, el precio será el definido en la ficha de la referencia.

\- **Descuento**: porcentaje de descuento que se le realizará al cliente.

\- **Parcial**: valor total del artículo (sin sumar los impuestos) resultante de multiplicar las unidades pedidas por el precio menos los descuentos.

\- **Costo**: valor de compra del artículo.

\- **Tipo de IVA**: tomará por defecto el tipo de IVA definido en la ficha del artículo si el albarán tiene el tipo de IVA general. De lo contrario, será el 0 %.

\- **Contador**: campo destinado a ordenar todas las líneas del albarán. Mantendrán el orden de menor a mayor en la presentación de las rejillas y en los impresos. Se podrá modificar para variar el orden según las necesidades.

\- **Operación**: estos campos se utilizan para imputar una línea de albarán de venta a un cheque regalo de una operación. Mediante el localizador presentado, veremos los vales activos que tiene el cliente / agente. Al seleccionar uno de ellos, se presentarán en la línea del albarán los datos relativos al cheque regalo.

**Opciones de las líneas de albarán**

\- **Aceptar**: con este botón guardamos los cambios realizados.

\- **Cancelar**: abortamos el alta o modificación de la línea.

Para eliminar una línea de albaranes de venta, tendremos que marcar la línea a eliminar pulsar el botón **Supr** del teclado o el botón secundario del ratón y seleccionar **formulario de baja**. Nos aparecerá un formulario desde el que podremos eliminar la línea.

**-TOTALES:** presenta el desglose de importe totales del albarán de venta.

**-INTERNAS:** muestra el beneficio de las líneas incluidas en el albarán de venta.

**-SEGUIMIENTOS:** se podrá grabar seguimientos relacionados con los albaranes de ventas, en esta pestaña se presentan los grabados.

**Opciones desde un albarán de venta:**

**Aceptar:** si pulsamos esta opción, quedarán guardados todos los cambios que hayamos realizado sobre la ficha del albarán.

**Cancelar:** con este botón, saldremos de la ficha del albarán sin guardar los posibles cambios que hayamos realizado. Se puede pulsar la tecla ESC para ejecutar esta opción.

**Borrar:** sirve para eliminar el albarán, y solo lo podrán hacer usuarios supervisores y cuando no esté facturado.

**Notas:** presenta un formulario en el que se podrán incluir notas relacionadas con el albarán.

**Facturar:** facturará el albarán. Se podrá indicar en las series de las facturas que se imprima el documento al generar la factura, y por tanto, si este estuviera marcado en el momento de facturar desde este botón, se imprimirá la factura generada.

**Imprimir:** imprime el albarán de venta con el modelo indicado en la serie del albarán.

**Impresión selectiva:** imprime el albarán de venta con el modelo que se seleccione al pulsar el botón. Nos aparecerá un recuadro en el que tendremos que indicar el modelo.

**Exportar a TXT:** mediante este botón podremos generar un fichero en formato TXT con la cabecera y el contenido del albarán de venta. Tendremos que seleccionar la carpeta donde guardaremos el fichero. El nombre de este será el código del albarán de venta (serie + número). Este fichero podrá ser utilizado por el cliente o agente del albarán para grabar directamente en su base de datos la compra realizada. La estructura del fichero podrá ser solicitada a los técnicos de Velmotor.

**Importar de TXT:** mediante este botón podremos crear un albarán de venta a partir de un fichero TXT generado desde cualquier aplicación Velmotor, que contenga la estructura de un albarán de compra.

2 - BUSCAR

Localizador de albaranes de ventas a través de distintos criterios. Nos permite consultar, borrar o modificar la información de un albarán. Al acceder a esta opción encontraremos la siguiente pantalla:

Este localizador nos permite buscar un albarán por los siguientes criterios:

**-NÚMERO, FECHA, CLIENTE, NOMBRE DEL CLIENTE y VENDEDOR / MES:** el cursor se irá situando en el albarán cuyo número, fecha, código de cliente, nombre del cliente coincida con lo seleccionado.

Para acceder a la ficha del pedido seleccionado, se puede hacer doble clic sobre él, pulsar el botón SELEC., o teclear el botón intro del teclado.

El formulario que se presenta es el mismo que el de grabación.

3 - LISTAR

Esta opción lanza una búsqueda que nos presentará un listado de albaranes de venta. Este listado se puede acotar a través del filtro de búsqueda que se presenta a continuación.

Después de indicar los criterios deseados, nos aparecerá una rejilla con todos los albaranes que los cumplan.

4 – IMPRESIÓN CONTINUA

Esta opción lanza la búsqueda del listado anterior, pero en vez de presentar una rejilla con los albaranes que cumplen los criterios seleccionados, imprimir todos ellos.

5 – FACTURACIÓN AUTOMÁTICA

Mediante esta opción podremos facturar varios albaranes de ventas simultáneamente. El funcionamiento es el siguiente.

Al seleccionar la opción, nos aparece un filtro de búsqueda en el que podremos acotar los albaranes a facturar. Además, podremos seleccionar una fecha concreta de facturación (fecha que tomarán las facturas) y elegir entre que se tomen las series de las facturas definidas en cada serie de albarán de venta, o seleccionar una serie de facturación concreta.

A continuación aparece una rejilla presentando la facturación previa (todavía no se ha generado ninguna factura). El programa ha agrupado todos los albaranes pendientes de facturar por cada cliente / agente, por tipo de pago y vencimientos, y por serie de facturación.

En esta pantalla, se podrán rebuscar albaranes. Esta opción se encuentra sobre la rejilla, y vuelve a presentar el filtro de albaranes para incluir en la facturación previa más albaranes. Esto puede servir en los casos en los que queramos facturar simultáneamente albaranes de dos series diferentes.

Además, la rejilla es multi-selección, de modo que solo tendremos que imprimir o generar la factura definitiva de aquellas facturas previas que queramos. Estas dos opciones las encontramos en la parte inferior de la rejilla.

Cuando ejecutamos la opción de facturar, nos aparecerá a continuación un listado con todas las facturas generadas.

Podremos consultar todas las facturas previas generadas haciendo doble click sobre la deseada.

En esta podemos modificar el número de factura que se va a generar, así como la fecha. Además podemos seleccionar los albaranes que no queramos incluir en dicha factura y pulsando Excluir albaranes no los incluirá en la factura que se genera.

6 – LOCALIZAR REFERENCIAS

Con esta opción podremos localizar cualquier referencia, independientemente de que esté grabada como artículo o no. [Opción explicada en el menú de artículos](file:///C:/Users/warda/OneDrive/Documents/Manual%20Velmotor/Manual\_Velmotor/nuevo\_manual/articulos.htm#localizar).

7 – LISTADO DETALLE

Presenta las líneas de albaranes de ventas que cumplan las condiciones que se presentan en el filtro siguiente.

8 – IMPUTAR A OR

Mediante esta opción podremos añadir a una orden de reparación cualquier artículo. Además se podrá utilizar el lector de códigos de barras para seleccionar el artículo.

9 – LOCALIZAR ARTÍCULOS

Esta opción muestra un localizador de artículos, mediante el cual podremos consultar cualquiera de ellos. [Opción explicada en el menú de artículos](file:///C:/Users/warda/OneDrive/Documents/Manual%20Velmotor/Manual\_Velmotor/nuevo\_manual/articulos.htm#buscar).

A – LOCALIZAR TARIFAS

Esta opción muestra un localizador de tarifas, mediante el cual podremos consultar cualquiera de ellas. [Opción explicada en el menú de tarifas](file:///C:/Users/warda/OneDrive/Documents/Manual%20Velmotor/Manual\_Velmotor/nuevo\_manual/tarifas.htm#buscar).

B – ENTREGAR MATERIAL PENDIENTE

Con esta opción veremos de una manera rápida y cómoda todo el material que nos ha pedido un cliente o agente y que está pendiente de entregar. Además, podremos crear directamente desde aquí mismo, los albaranes de entrega. Al ejecutar la opción, tendremos que seleccionar el cliente o agente del que queramos consultar lo pendiente de entregar. Y a continuación nos aparecerá la siguiente rejilla.

En esta rejilla podemos ver los artículos, las unidades pedidas, las pendientes, las unidades que se pidieron al proveedor, las que ya se han recibido, las que se han recibido y no hemos entregado al cliente o agente, las unidades que vamos a entregar en este momento, el importe parcial de la venta, el número de pedido y la fecha del pedido. Una vez seleccionadas las línea entregar, pulsaremos sobre el botón situado bajo la rejilla y se creará el albarán de venta correspondiente.

Podremos modificar las unidades a entregar, pero no podrá ser superior a las unidades pendientes.
