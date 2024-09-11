# Botones lateral izquierdo

o _Nuevo artículo:_ permite dar de alta a un nuevo artículo rellenando el siguiente formulario:

![](<../../../../.gitbook/assets/image (484).png>)

o Referencia: se aconseja que se especifique la del artículo indicada por el proveedor que la suministra. El objetivo de esto es la fácil grabación de la entrada de material y su posterior venta. Si el proveedor nos envía la mercancía etiquetada, con un lector de códigos de barras podremos ir grabando albaranes de entrada de mercancía. De igual modo, en todos los documentos de venta, podremos utilizar el lector para ir incluyendo los artículos solicitados por el cliente.

o Nombre: indicamos aquí, la denominación o nombre del producto.

o Familia: sirve para clasificar una serie de artículos que reúnen alguna característica en común. Por ejemplo, artículos de boutique. Es la clasificación más importante que tienen los artículos, e incluso heredarán de su familia campos importantes como son los datos contables y datos para los cálculos del precio de venta. Se puede crear una familia accediendo al menú del campo o desde el "Maestro" > "Familias".

o Marca: agrupa todos los artículos y familias bajo una única denominación, es el nivel superior de la estructura de artículo.

o Tipo de artículo: sirve para poder clasificar una serie de artículos. Los grupos son creados por nuestro equipo de Winmotor según las necesidades del cliente.

o Ubicaciones: son tres campos en los que podremos indicar la ubicación o ubicaciones (almacén/es o subalmacén/es) de los artículos. En la grabación de los inventarios, también se puede indicar la ubicación de los que se va incluyendo, pasando estas ubicaciones directamente a la ficha del artículo. La gestión de las ubicaciones se realiza al mismo nivel que un almacén. Las ubicaciones se visualizan en la grabación de un albarán de venta y en los movimientos de almacén.

o Proveedor: indicamos aquí el proveedor que suministra este artículo. En el caso de que un mismo artículo podamos comprarlo a diferentes proveedores, se puede indicar aquí el proveedor que nos aparecerá en los documentos de compra por defecto (el más común).

o Precio de compra: precio bruto de compra del artículo al proveedor

**o Descuento 1 - Descuento 2 - Descuento 3:** se pueden definir hasta tres posibles descuentos. Estos descuentos son los que te ofrece el proveedor.

**o Precio de venta:** precio bruto de venta del artículo al cliente. Es posible crear tarifas de ventas y ofertas personalizadas y aplicarlas mediante el botón inferior "Ver tarifas personalizadas" siempre que coincida en algún campo con el artículo que se está dando de alta (véase ["Gestión de precios y Tarifas de ventas"](../gestion-de-precios-y-tarifas-de-ventas.md)):

![](<../../../../.gitbook/assets/image (488).png>)

o Precio de venta recomendado (P.V.R.): recomendación del fabricante / marca sobre el precio de venta final al cliente.

o Porcentaje de IVA: porcentaje de IVA que se aplicará sobre este artículo en ventas con régimen general por defecto y con posibilidad de seleccionar otro.

o Precio de venta al público (P.V.P.): precio de venta final impuestos incluidos.

o _Buscar Artículo:_ Localizador de artículos a través de distintos criterios. Nos permite consultar, borrar o modificar la información de un artículo. La rejilla de este localizador nos muestra la referencia, denominación, información de stock de cada artículo además del P.V.P.. Al acceder a esta opción encontraremos la siguiente pantalla:

![](<../../../../.gitbook/assets/image (486).png>)

Este localizador nos permite buscar un artículo por los siguientes criterios:

o Alfabético: el cursor se irá situando en el artículo cuya descripción vaya coincidiendo con lo introducido en el campo de edición.

o Trozos de palabras: se nos presentarán todos los artículos cuya descripción contenga las palabras que introduzcamos en el campo de edición (búsqueda mínima a partir de 3 caracteres)

o Referencias activas: el cursor se irá situando en el artículo cuyo código vaya coincidiendo con lo introducido en el campo de edición.

o Trozos de referencias: se nos presentarán todos los artículos cuya referencia contenga los caracteres que introduzcamos en el campo de edición (búsqueda mínima a partir de 3 caracteres)

o Palabras auxiliares: se nos presentarán todos los artículos que contengan esas palabras coincidentes al campo "descripción" de la pestaña auxiliares (pestaña de la ficha de artículo)

o Referencias todas: el cursor se irá situando en el artículo cuyo código vaya coincidiendo con lo introducido en el campo de edición **sin diferenciar entre las activas y las pasivas.**

o Palabras descripción proveedor: se nos presentarán todos los artículos que contengan esas palabras coincidentes al campo "nombre" en la línea de tarifa condicionada por proveedor \*\*(ficha de artículo > línea de proveedor > personalización del proveedor > nombre)

![](<../../../../.gitbook/assets/image (485).png>)

Para acceder a la ficha del artículo seleccionado, se puede hacer doble clic sobre él o pulsar el botón intro del teclado una vez seleccionado (véase ["Ficha del artículo"](../ficha-del-articulo/))

o _Listados:_ muestra un panel desplegable con las siguientes opciones de listados sobre los artículos:

o Básico: muestra los artículos filtrados por los siguientes requisitos (muestra referencia, denominación, PVP y Precio Venta)

![](<../../../../.gitbook/assets/image (564).png>)

o Stocks general: muestra los artículos filtrados por los siguientes requisitos (muestra referencia, nombre, Stock, PMC y Valor de Stock):

![](<../../../../.gitbook/assets/image (565).png>)

o Stocks por almacén: muestra los artículos filtrados por los siguientes requisitos (muestra referencia / artículo, nombre, Almacén, Stock, tipo de artículo, PMC, Valor stock y permite localizar artículos por palabras y quitar de la búsqueda almacenes restringidos):

<figure><img src="../../../../.gitbook/assets/imagen (261).png" alt=""><figcaption></figcaption></figure>

Genera un listado que permite:

* **Traspasar stock:**
  * Crea un parte de traspaso de las líneas seleccionadas desde el almacén de la línea hasta el almacén que se seleccione.
  * Si la serie está puesta como que se inicia en "borrador" se podrán cambiar las unidades antes de confirmar.
  * No se podrán traspasar líneas de distintos almacenes a la vez.
* **Desactivar almacén:**
  * Desactiva el almacén del artículo en las líneas seleccionadas. Deben de estar sin stock
* **Activar almacén:**
  * Activa el almacén del artículo en las líneas seleccionadas

<figure><img src="../../../../.gitbook/assets/imagen (260).png" alt=""><figcaption></figcaption></figure>

o Stocks a fecha: muestra los artículos filtrados por los siguientes requisitos (muestra referencia, nombre, Stock, Costo, Valor stock):

![](<../../../../.gitbook/assets/image (567).png>)

o Movimientos: presenta movimientos entre fechas de un artículo determinado:

![](<../../../../.gitbook/assets/image (568).png>)

o Artículos pasivos: aquellos artículos inactivos y que son controlables desde el panel de artículos pasivos del mismo modo que desde el panel de artículos:

![](<../../../../.gitbook/assets/image (569).png>)

o Revisión de precios: realizando el filtrado de los artículos nos presenta un menú con los artículos que cumplan los requisitos especificados, que al seleccionar 1 o varios, indica los documentos (tarifas de precios, ofertas...) y sus valores, observando a la vez y en conjunto la tarifa del artículo, condiciones aplicadas a éste en las tarifas de ventas y su PVR:

![](<../../../../.gitbook/assets/image (570).png>)

![Menú Revisión de Precios](<../../../../.gitbook/assets/image (571).png>)

o Análisis rotación: muestra los artículos filtrados por los siguientes requisitos (muestra referencia, nombre, familia, primera compra, unidades compradas, unidades vendidas, Stock físico, Valor de Stock Pendientes de recibir, Pendientes de entregar, Stock previsto, Días desde la última venta, Importe de compras, Importe de ventas, Costo actual, Beneficio Real y % de Beneficio):

![](<../../../../.gitbook/assets/image (572).png>)

![Análisis de Rotación](<../../../../.gitbook/assets/image (573).png>)

o _Ofertas:_ muestra un panel desplegable con las siguientes opciones de listados sobre los artículos: Véase ["Gestión de precios y Tarifas de ventas"](../gestion-de-precios-y-tarifas-de-ventas.md) - Panel de Ofertas - Permite realizar ofertas con condiciones determinadas en el propio documento, por marca, familia, artículo, tipo de artículo y un precio, descuento o incremento sobre el costo.

![](<../../../../.gitbook/assets/image (574).png>)

![](<../../../../.gitbook/assets/image (575).png>)

o Sustituciones: muestra un panel indicando Fecha, referencia anterior, referencia nueva y comentarios de las sustituciones. El panel dispone de los botones Localizar que permite realizar la búsqueda de la referencia y Nueva para dar de alta una nueva sustitución:

![](<../../../../.gitbook/assets/image (576).png>)

o _Rotación y consumos:_ [_véase "Gestión de la rotación de consumos y el stock mínimo"_](../gestion-de-la-rotacion-de-consumos-y-el-stock-minimo.md)

![](<../../../../.gitbook/assets/image (577).png>)
