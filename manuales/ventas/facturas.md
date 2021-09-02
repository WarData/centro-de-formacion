# Facturas

FACTURAS DE VENTAS

Mediante esta opción, podremos grabar, modificar o consultar todas las facturas de venta que hemos realizado. Al entrar en ella, nos aparece un menú con calendario en el que se nos presentan opciones para grabar, consultar y listar facturas, y una rejilla que nos muestra todas las que hemos realizado en el día seleccionado en el calendario.

1 - GRABAR

Permite dar de alta a una nueva factura de venta de manera directa rellenando el siguiente formulario. Además de este modo de grabación, para dar de alta una factura se pueden utilizar otros métodos, directamente desde un albarán de venta, desde un vehículo u operación de venta de vehículos, desde una orden de reparación, o los procesos de facturación en tanda de albaranes de venta u órdenes de reparación. Una factura está compuesta por su cabecera, donde se introducen los datos generales, como la serie, la fecha o cliente, y las líneas, donde se guardan los documentos que se facturan \(albaranes, vehículos u órdenes de reparación\).

La cabecera está compuesta por los siguientes campos:

**-SERIE:** es un campo imprescindible de rellenar, y de él depende la presentación o contenido que tendrá la factura. Entre otras cosas, en una serie de factura de venta se define si será de recambios \(albaranes de ventas\), de taller \(órdenes de reparación\), de vehículos nuevos o de ocasión \(ambas contienen vehículos\). Todas las posibilidades de las series de documentos se detallan en la sección…explicación de series de documentos.

**-NÚMERO:** todos los documentos están clasificados por su serie y un número, que siempre será por defecto el siguiente al último grabado de la misma serie. Tanto el número como la serie de un documento se podrán modificar manualmente, aunque, a menos que sea imprescindible el cambio, no es aconsejable.         

**-FECHA:** se indica aquí la fecha de la factura. Esta fecha debe de estar dentro de los rangos definidos en parámetros.

**-CLIENTE o AGENTE:** en los documentos de ventas, se podrá indicar si se está vendiendo a un cliente o a un agente. Hay que recordar que son tablas de datos diferentes y solo se podrá indicar uno de ellos por factura. Ambos campos contienen botones incrustados para localizar, grabar o editar el cliente o agente seleccionado. Además de código del cliente o agente, se presenta en la factura su razón social, su dirección de facturación y el CIF. Además de estos, bajo el CIF se presentará un campo con las notas de facturación del cliente o agente, si tuvieran.

**-CENTRO:** este campo solo será visible por aquellas aplicaciones en las que se trabaje con más de un centro de trabajo y así se haya indicado en parámetros. Se utiliza para indicar el centro de trabajo para el que se hace la factura. Este campo, se rellena automáticamente y solo será manipulable por aquellos usuarios autorizados.

**-DEPARTAMENTO INTERNO:** si la serie de la factura es INTERNA, se podrá seleccionar el departamento para el que se graba la factura, sino este campo no se presentará.

**-VENDEDOR:** tomará por defecto el vendedor definido en la ficha del cliente o agente. Se podrá modificar manualmente.

**-TIPO DE PAGO 1 y 2, VENCIMIENTOS  e IMPORTES:** una factura de venta podrá tener hasta 2 tipos de pago diferentes. En ese caso, habrá que utilizar los campos **IMP** situados justo a la derecha de cada tipo de pago, para indicar el importe que corresponde a cada tipo. Cuando el albarán corresponde a un cheque regalo, el tipo de pago tomará por defecto modelo VALE.

**-TIPO DE IVA:** este campo tomará por defecto el tipo de IVA definido en la ficha del cliente o del agente seleccionado en el albarán. Se podrá modificar manualmente. Los diferentes tipos de IVA y de exentos, se explican en la sección proveedores – tipos de IVA.

**-DOCUMENTO ACREDITATIVO:** si el cliente es intracomunitario, y tiene documento acreditativo, se presentarán los campos relativos a este documento en esta pantalla. Si fuera intracomunitario y no tuviera documento acreditativo, saltará un mensaje indicándolo.

**-OPERACIÓN ORIGEN y FECHA:** si la factura proviene de una operación de venta de vehículos, se presentarán estos campos, indicando el número de la operación y su fecha. Además se presentará un botón con el que se podrá consultar la operación.

**PESTAÑERO**

**-CONTENIDO:** se presentará una rejilla diferente para cada tipo de factura.

·          Facturas de recambios

Se presenta una rejilla en la que se muestran los albaranes de ventas que componen la factura. Se pueden grabar nuevas líneas para facturar albaranes haciendo doble click sobre cualquier línea en blanco o pulsando el botón **+** o **Insert** del teclado. Nos aparecerá la siguiente pantalla.

En este formulario podremos localizar los albaranes pendientes de facturar del cliente o agente seleccionado mediante el botón incrustado en el campo albarán de ventas. También se podrá editar el albarán seleccionado.

El formulario tiene botones para **Aceptar** los cambios realizados, **Cancelar** los cambios o **Borrar** la línea.

·          Facturas de taller

Se presenta una rejilla en la que se muestran las líneas de las órdenes de reparación incluidas en la factura. Se podrán visualizar haciendo doble click sobre cualquiera de ellas y nos aparecerá el siguiente formulario.

Para añadir o eliminar líneas de órdenes en la factura, hay que utilizar los botones situados justo debajo de la rejilla.

**Añadir ORs**: sirve para incluir en la factura otras órdenes del mismo cliente o agente. Al pulsar sobre el botón nos aparecerá el siguiente formulario, mediante el que seleccionaremos la orden a facturar.

A continuación, se presentará una rejilla con todas las líneas que componen la orden de reparación. Tendremos que seleccionar aquellas líneas que vayamos a facturar y pulsar el botón que aparece justo debajo de la rejilla.

**Borrar ORs**: mediante este botón, quitaremos de la factura la orden de reparación que seleccionemos en el localizador que nos aparece.

·          Facturas de vehículos \(el funcionamiento es similar para vehículos nuevos y de ocasión, salvo la rejilla del que nos muestra los vehículos facturados\)

En ambas rejillas se nos presentan los vehículos o conceptos facturados. Podremos editar cada línea haciendo doble click sobre cualquiera de ellas. Nos aparecerá el siguiente formulario.

-          Bastidor: aquí podremos localizar el bastidor que vayamos a facturar. No se podrá seleccionar un bastidor que no esté en stock.

-          Matrícula: este campo no es manipulable y presentará la matrícula del bastidor seleccionado.

-          Concepto: además de poder facturar un bastidor, se podrán facturar conceptos de vehículos, como por ejemplo, el transporte o las tasas.

-          Nombre del concepto: equivale a la descripción de cada línea.

-          Base IVA: campos destinado a presentar el desglose de IVA del bastidor o concepto.

-          Base IM: campos para definir el impuesto de matriculación que lleva cada línea. Tanto el IVA como el impuesto de matriculación tendrán por defecto el valor definido en la ficha del vehículo o del concepto, aunque se pueden modificar en la propia factura. Se han incluido unos botones para aplicar o quitar el IM en una línea de factura cuando en la ficha del vehículo o del concepto no estén definidos y se quieran aplicar, o lo estén y se quieran quitar.

-          Total base: corresponde a la suma de las bases de la línea de factura.

-          Total IM: suma total del impuesto de matriculación.

-          Total IVA: suma total del IVA.

-          Total línea: equivale a la suma total de los campos anteriores.

-          Número de orden: campo destinado a ordenar tanto en las rejillas como en los impresos, las líneas de las facturas.

-          Operación: muestra la operación de la que proviene.

Además, cada línea contiene los botones generales para **Aceptar**, **Cancelar** o **Borrar** la ficha.

**-DETALLE:** esta pestaña solo se verá cuando estemos en una factura de recambios, y mostrará todas las líneas que componen los albaranes incluidos en la factura.

**-TOTALES:** presenta el desglose del importe total de la factura de venta.

**-COBROS:** muestra los apuntes o efectos de venta realizados. Los apuntes de caja equivalen a los tipos de pago en efectivo, y los efectos a los aplazados.

**-INTERNAS:** muestra el beneficio de las líneas incluidas en la factura de venta. Dependiendo del tipo de factura, se presentará una rejilla diferente.

·           Facturas de recambios

·          Facturas de taller

·          Facturas de vehículos

**-AGENTE:** cuando la factura es de vehículos, se presentará esta pestaña, en la que se puede indicar si intervino o no un agente, y modificar  el porcentaje de comisión que tendremos que pagarle y además imprimir la factura de comisión del agente.

**-APUNTE CONTABLE:** si la factura está contabilizada, se podrá ver en esta pestaña los apuntes contables generados. Esto solo será posible si el programa está enlazado con la contabilidad Velconta.

**-NOTAS INTERNAS:** podemos anotar aquí cualquier nota interna relacionada con la factura.

**-COMENTARIOS:** también podemos anotar notas en este campo, pero con la salvedad de que estos comentarios podrán imprimirse en el documento de venta.

**Opciones desde una factura de venta**

**Aceptar:** si pulsamos esta opción, quedarán guardados todos los cambios que hayamos realizado sobre la ficha de la factura.

**Cancelar:** con este botón, saldremos de la ficha de la factura sin guardar los posibles cambios que hayamos realizado. Se puede pulsar la tecla ESC para ejecutar esta opción.

**Borrar:** sirve para eliminar la factura, y solo lo podrán hacer usuarios supervisores y cuando no esté ni contabilizada ni cobrada.

**Imprimir:** imprime la factura de venta con el modelo indicado en la serie de la factura.

**Abonar:** solo es posible crear documentos automáticos de abono sobre facturas de vehículos y de recambios. En el caso de las facturas de vehículos, creará una factura de venta de abono con las mismas líneas que la factura original, volviendo a quedar el vehículo en stock. En el caso de las facturas de recambios, se creará un albarán de abono por cada albarán que contenga la factura, y la correspondiente factura de abono.

**Impresión selectiva:** imprime la factura de venta con el modelo que se seleccione al pulsar el botón. Nos aparecerá un recuadro en el que tendremos que indicar el modelo.

**Factura de comisión:** imprime un documento de venta equivalente a la factura de la comisión pagada al agente por la venta del vehiculo.

**Cobro directo:** con esta opción realizamos el cobro de la factura. Se nos abrirá la ventana de apuntes donde debemos seleccionar la cuenta contable, así como el concepto. Una vez cobrado nos da la opción de imprimir el recibo.

2 – BUSCAR

Localizador de facturas de ventas a través de distintos criterios. Nos permite consultar, borrar o modificar la información de una factura. Al acceder a esta opción encontraremos la siguiente pantalla:

Criterios de búsqueda:

**-NÚMERO, FECHA y CLIENTE:** el cursor se irá situando en la factura cuyo número, fecha y código de cliente coincida con lo seleccionado.

**-PALABRAS NOMBRE CLIENTE:** el localizador presentará en pantalla aquellas facturas cuyo cliente contenga la palabra o palabras introducidas.

Para acceder a la ficha de la factura seleccionada, se puede hacer doble clic sobre él, pulsar el botón SELEC., o teclear el botón intro del teclado.

El formulario que se presenta es el mismo que el de grabación.

3 – GRÁFICO DE VENTAS

Esta opción lanza una búsqueda que nos presentará un gráfico de facturas de venta. Este listado se puede acotar a través del filtro de búsqueda que se presenta a continuación.

Después de indicar los criterios deseados, nos aparecerá un gráfico con todas las ventas del intervalo.

4 – IMPRESIÓN CONTINUA

Esta opción lanza la búsqueda de la opción anterior, pero en vez de presentar un gráfico, imprime las facturas del intervalo.

5 – LISTAR

También se utiliza en esta opción el mismo filtro de búsqueda, pero en este caso, muestra una rejilla con el resultado.

6 – LISTADO de IVA

Misma opción que la anterior, pero en la rejilla se desglosan los impuestos.

