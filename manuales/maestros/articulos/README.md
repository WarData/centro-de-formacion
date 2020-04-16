---
description: Aquella mercancía que puede comercializarse
---

# Artículos

El fichero de artículos es en el que se recogen todas las referencias, piezas, productos o recambios que se compran, instalan y venden en el concesionario. Son una de las partes más importantes del módulo de recambios y se encuentran enlazados con todas sus opciones \(presupuestos, pedidos albaranes, movimientos de almacén, etc...\). 

El menú de artículos presenta un listado de ellos ordenados alfabéticamente por su código. 

Pasamos a mostrar el panel de artículos donde encontramos las habituales opciones de búsqueda y filtrado además de la rejilla que muestra los campos "referencia", "denominación", "familia", "precio neto", "stock físico" y "stock disponible" y los botones que explicaremos a continuación "imprimir tarifa", "Imprimir informe", "Filtrar", "Modificar artículos", "Incluir en tarifa" e "Incluir en oferta":

![](../../../.gitbook/assets/image%20%28446%29.png)

* **Botones inferiores:**

                o   _Imprimir Tarifa:_ filtramos los artículos según las necesidades para presentarlos en la rejilla. Una vez mostrados, al pulsar el botón mostrará:

![](../../../.gitbook/assets/image%20%28428%29.png)

Tras pulsar en "F1 imprimir" nos mostrará el listado siguiente con los artículos filtrados y con la capacidad de variar el formato de impresión, así como características de la impresión:

![](../../../.gitbook/assets/image%20%28430%29.png)

                o   _Imprimir informe:_ filtramos los artículos según las necesidades para presentarlos en la rejilla. Una vez mostrados, al pulsar el botón mostrará los siguientes informes disponibles para aplicar a los artículos filtrados en la rejilla:

![](../../../.gitbook/assets/image%20%28136%29.png)

Seleccionamos con doble clic el informe, mostrando la aplicación la ventana de selección de impresora para imprimirlo.

               o   _Filtrar:_ filtramos los artículos según las necesidades para presentarlos en la rejilla. Una vez mostrados, al pulsar el botón mostrará la siguiente ventana, donde podremos filtrar aún más la búsqueda por texto, centrada en el campo "denominación":

![](../../../.gitbook/assets/image%20%28220%29.png)

                o   _Modificar artículos:_ filtramos los artículos según las necesidades para presentarlos en la rejilla. Una vez mostrados, seleccionamos únicamente aquellos a los que queremos aplicar la modificación. Al pulsar el botón mostrará la siguiente ventana, donde podremos modificar las propiedades de los artículos al nivel indicado en la imagen \(el menú muestra en la parte inferior el número de artículos seleccionados\): 

![](../../../.gitbook/assets/image%20%28348%29.png)

                o   _Incluir en tarifa:_ filtramos los artículos según las necesidades para presentarlos en la rejilla. Una vez mostrados, seleccionamos únicamente aquellos que queremos incluir en alguna de las tarifas existentes \(véase ["Tarifas de Ventas"](../tarifas-de-ventas.md) en "Maestros"\) y pulsamos el botón, obteniendo la rejilla de tarifas de ventas donde hacemos doble clic en la que queramos incluir los artículos seleccionados.

![](../../../.gitbook/assets/image%20%28219%29.png)

                o   _Incluir en oferta:_ filtramos los artículos según las necesidades para presentarlos en la rejilla. Una vez mostrados, seleccionamos únicamente aquellos que queremos incluir en alguna de las ofertas existentes \(véase "Ofertas" dentro del panel de artículos\) y pulsamos el botón, obteniendo la rejilla de ofertas donde hacemos doble clic en la que queramos incluir los artículos seleccionados.

![](../../../.gitbook/assets/image%20%28190%29.png)

* **Botones lateral izquierdo:**

               **** o   _Nuevo artículo:_ permite dar de alta a un nuevo artículo rellenando el siguiente formulario:

![](../../../.gitbook/assets/image%20%2847%29.png)

                               **o   Referencia:** se aconseja que se especifique la del artículo indicada por el proveedor que la suministra. El objetivo de esto es la fácil grabación de la entrada de material y su posterior venta. Si el proveedor nos envía la mercancía etiquetada, con un lector de códigos de barras podremos ir grabando albaranes de entrada de mercancía. De igual modo, en todos los documentos de venta, podremos utilizar el lector para ir incluyendo los artículos solicitados por el cliente.

                                **o   Nombre:** indicamos aquí, la denominación o nombre del producto.

                                **o   Familia:** sirve para clasificar una serie de artículos que reúnen alguna característica en común. Por ejemplo, artículos de boutique. Es la clasificación más importante que tienen los artículos, e incluso heredarán de su familia campos importantes como son los  datos contables y datos para los cálculos del precio de venta. Se puede crear una familia accediendo al menú del campo o desde el "Maestro" &gt; "Familias".

                                 **o   Marca:** agrupa todos los artículos y familias bajo una única denominación, es el nivel superior de la estructura de artículo.

                                 **o   Tipo de artículo:** sirve para poder clasificar una serie de artículos. Los grupos son creados por nuestro equipo de Winmotor según las necesidades del cliente.

                                 **o   Ubicaciones:** son tres campos en los que podremos indicar la ubicación o ubicaciones \(almacén/es o subalmacén/es\) de los artículos. En la grabación de los inventarios, también se puede indicar la ubicación de los que se va incluyendo, pasando estas ubicaciones directamente a la ficha del artículo. La gestión de las ubicaciones se realiza al mismo nivel que un almacén. Las ubicaciones se visualizan en la grabación de un albarán de venta y en los movimientos de almacén.

                                 **o   Proveedor:** indicamos aquí el proveedor que suministra este artículo. En el caso de que un mismo artículo podamos comprarlo a diferentes proveedores, se puede indicar aquí el proveedor que nos aparecerá en los documentos de compra por defecto \(el más común\).

                                 **o   Precio de compra:** precio bruto de compra del artículo al proveedor

                                 **o   Descuento 1 - Descuento 2 - Descuento 3:** se pueden definir hasta tres posibles descuentos. Estos descuentos son los que te ofrece el proveedor.

                                 **o   Precio de venta:** precio bruto de venta del artículo al cliente. Es posible crear tarifas de ventas personalizadas y aplicarlas mediante el botón inferior "Ver tarifas personalizadas":

![](../../../.gitbook/assets/image%20%28186%29.png)

                                 **o   Precio de venta recomendado \(P.V.R.\):** recomendación del fabricante / marca sobre el precio de venta final al cliente.

                                 **o   Porcentaje de IVA:** porcentaje de IVA que se aplicará sobre este artículo en ventas con régimen general por defecto y con posibilidad de seleccionar otro.

                                 **o   Precio de venta al público \(P.V.P.\):** precio de venta final impuestos incluidos.

                     o   _Buscar Artículo:_ Localizador de artículos a través de distintos criterios. Nos permite consultar, borrar o modificar la información de un artículo. La rejilla de este localizador nos muestra la referencia, denominación, información de stock de cada artículo además del P.V.P.. Al acceder a esta opción encontraremos la siguiente pantalla:

![](../../../.gitbook/assets/image%20%28101%29.png)

Este localizador nos permite buscar un artículo por los siguientes criterios:

                                 **o   Alfabético:** el cursor se irá situando en el artículo cuya descripción vaya coincidiendo con lo introducido en el campo de edición.

                                 **o   Trozos de palabras:** se nos presentarán todos los artículos cuyas descripción contenga las palabras que introduzcamos en el campo de edición \(búsqueda mínima a partir de 3 caracteres\)

                                 **o   Referencias activas:** el cursor se irá situando en el artículo cuyo código vaya coincidiendo con lo introducido en el campo de edición.

                                 **o   Trozos de referencias:** se nos presentarán todos los artículos cuya referencia contenga los caracteres que introduzcamos en el campo de edición \(búsqueda mínima a partir de 3 caracteres\)

                                 **o   Palabras auxiliares:**

                                 **o   Referencias todas:**

                                 **o   Palabras descripción proveedor**

![](../../../.gitbook/assets/image%20%28393%29.png)

Para acceder a la ficha del artículo seleccionado, se puede hacer doble clic sobre él o pulsar el botón intro del teclado una vez seleccionado.

