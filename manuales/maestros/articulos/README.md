---
description: Aquella mercancía que puede comercializarse
---

# Artículos

El fichero de artículos es en el que se recogen todas las referencias, piezas, productos o recambios que se compran, instalan y venden en el concesionario. Son una de las partes más importantes del módulo de recambios y se encuentran enlazados con todas sus opciones \(presupuestos, pedidos albaranes, movimientos de almacén, etc...\). 

El menú de artículos presenta un listado de ellos ordenados alfabéticamente por su código. 

Pasamos a mostrar el panel de artículos donde encontramos las habituales opciones de búsqueda y filtrado además de la rejilla que muestra los campos "referencia", "denominación", "familia", "precio neto", "stock físico" y "stock disponible" y los botones que explicaremos a continuación "imprimir tarifa", "Imprimir informe", "Filtrar", "Modificar artículos", "Incluir en tarifa" e "Incluir en oferta":

![](../../../.gitbook/assets/image%20%28442%29.png)

* **Botones inferiores:**

                o   _Imprimir Tarifa:_ filtramos los artículos según las necesidades para presentarlos en la rejilla. Una vez mostrados, al pulsar el botón mostrará:

![](../../../.gitbook/assets/image%20%28424%29.png)

Tras pulsar en "F1 imprimir" nos mostrará el listado siguiente con los artículos filtrados y con la capacidad de variar el formato de impresión, así como características de la impresión:

![](../../../.gitbook/assets/image%20%28426%29.png)

                o   _Imprimir informe:_ filtramos los artículos según las necesidades para presentarlos en la rejilla. Una vez mostrados, al pulsar el botón mostrará los siguientes informes disponibles para aplicar a los artículos filtrados en la rejilla:

![](../../../.gitbook/assets/image%20%28135%29.png)

Seleccionamos con doble clic el informe, mostrando la aplicación la ventana de selección de impresora para imprimirlo.

               o   _Filtrar:_ filtramos los artículos según las necesidades para presentarlos en la rejilla. Una vez mostrados, al pulsar el botón mostrará la siguiente ventana, donde podremos filtrar aún más la búsqueda por texto, centrada en el campo "denominación":

![](../../../.gitbook/assets/image%20%28218%29.png)

                o   _Modificar artículos:_ filtramos los artículos según las necesidades para presentarlos en la rejilla. Una vez mostrados, seleccionamos únicamente aquellos a los que queremos aplicar la modificación. Al pulsar el botón mostrará la siguiente ventana, donde podremos modificar las propiedades de los artículos al nivel indicado en la imagen \(el menú muestra en la parte inferior el número de artículos seleccionados\): 

![](../../../.gitbook/assets/image%20%28345%29.png)

                o   _Incluir en tarifa:_ filtramos los artículos según las necesidades para presentarlos en la rejilla. Una vez mostrados, seleccionamos únicamente aquellos que queremos incluir en alguna de las tarifas existentes \(véase ["Tarifas de Ventas"](../tarifas-de-ventas.md) en "Maestros"\) y pulsamos el botón, obteniendo la rejilla de tarifas de ventas donde hacemos doble clic en la que queramos incluir los artículos seleccionados.

![](../../../.gitbook/assets/image%20%28217%29.png)

                o   _Incluir en oferta:_ filtramos los artículos según las necesidades para presentarlos en la rejilla. Una vez mostrados, seleccionamos únicamente aquellos que queremos incluir en alguna de las ofertas existentes \(véase "Ofertas" dentro del panel de artículos\) y pulsamos el botón, obteniendo la rejilla de ofertas donde hacemos doble clic en la que queramos incluir los artículos seleccionados.

![](../../../.gitbook/assets/image%20%28188%29.png)

* **Botones lateral izquierdo:**

               **** o   _Nuevo artículo:_ permite dar de alta a un nuevo artículo rellenando el siguiente formulario:

![](../../../.gitbook/assets/image%20%2847%29.png)

                               **o   Referencia:** se aconseja que se especifique la del artículo indicada por el proveedor que la suministra. El objetivo de esto es la fácil grabación de la entrada de material y su posterior venta. Si el proveedor nos envía la mercancía etiquetada, con un lector de códigos de barras podremos ir grabando albaranes de entrada de mercancía. De igual modo, en todos los documentos de venta, podremos utilizar el lector para ir incluyendo los artículos solicitados por el cliente.

                                **o   Nombre:** indicamos aquí, la denominación o nombre del producto.

                                **o   Familia:** sirve para clasificar una serie de artículos que reúnen alguna característica en común. Por ejemplo, artículos de boutique. Es la clasificación más importante que tienen los artículos, e incluso heredarán de su familia campos importantes como son los  datos contables y datos para los cálculos del precio de venta. Se puede crear una familia accediendo al menú del campo o desde el "Maestro" &gt; "Familias".

                                 **o   Marca:** agrupa todos los artículos y familias bajo una única denominación, es el nivel superior de la estructura de artículo.

                                 **o   Tipo de artículo:** sirve para poder clasificar una serie de artículos. Los grupos son creados por nuestro equipo de Winmotor según las necesidades del cliente.

                                 **o   Proveedor:** indicamos aquí el proveedor que suministra este artículo. En el caso de que un mismo artículo podamos comprarlo a diferentes proveedores, se puede indicar aquí el proveedor que nos aparecerá en los documentos de compra por defecto \(el más común\).

**-ALTERNATIVA 1, ALTERNATIVA 2** y **ALTERNATIVA 3:** se pueden indicar aquí referencias, alternativas al artículo. Puede servirnos para saber consultando la ficha de un artículo, que otros artículos puedo ofrecer o instalar en un vehículo, si no dispongo de stock en el primero.

**-OBSERVACIONES:** podremos insertar aquí, observaciones sobre el artículo.

**-STOCK MÍNIMO:** si rellenamos este campo, y tenemos marcado el parámetro necesario, mensaje artículos stock mínimo, el programa mostrará un aviso al usuario en el momento de realizar una venta de dicho artículo.

**-STOCK MÁXIMO:** este campo se calculará en base al consumo del artículo una vez grabemos documentos en la aplicación y sirve posteriormente para el cálculo de propuestas de pedidos de reposición. Inicialmente el usuario puede establecer el valor que estime.

**-MÍNIMO DE COMPRAS:** Se utiliza también para el cálculo de propuestas de pedidos de reposición e indica el número de unidades que entran en un paquete o caja.

**-UBICACIÓN:** son dos campos en los que podremos indicar la ubicación de los artículos. En la grabación de los inventarios, también se puede indicar la ubicación de los que se va incluyendo, pasando estas ubicaciones directamente a la ficha del artículo.

Los dos campos habilitados para indicar las ubicaciones, se visualizan en la grabación de un albarán de venta y en los movimientos de almacén.

**-CUENTAS CONTABLES:**

Estos campos sirven para especificar las cuentas contables donde se incluirá el importe de venta o compra en la contabilidad. Tendrá más sentido rellenarlas en el caso de que el programa estuviera enlazado con alguna contabilidad.

Se pueden indicar hasta cuatro tipos de cuentas contables diferentes para **compras,  devolución de compras, ventas** y **devolución de ventas.**

**-PRECIOS DE COMPRA:**

**-PRECIO TARIFA:** es el precio de compra del artículo.

**-DESCUENTO 1, DESCUENTO 2** y **DESCUENTO 3:** se pueden definir hasta tres posibles descuentos. Estos descuentos son los que te ofrece el proveedor.

**-PRECIO NETO:** es el resultado de restar al precio tarifa los descuentos especificados.

**-PRECIOS DE VENTA:**

Se pueden definir hasta cuatro tipos de fórmulas diferentes para calcular el precio de venta de un artículo. Sólo se puede definir una de ellas, y se explican a continuación:

**-DESCUENTO \(S/TARIFA\):** el precio de venta será el resultado de restar al precio tarifa el porcentaje de descuento definido aquí.

**-INCREMENTO \(S/TARIFA\):** en este caso, el porcentaje definido se suma al precio tarifa para definir el precio de venta.

**-INCREMENTO \(S/NETO\):** la fórmula es similar a la anterior, pero sobre el precio neto.

**-BENEFICIO \(S/NETO\)**

**-PVP:** precio de venta sin IVA calculado a través de los campos anteriores.

**-% IVA:** porcentaje de IVA que se aplicará sobre este artículo en ventas con régimen general.

**-PVP + IVA:** precio de venta más IVA.

