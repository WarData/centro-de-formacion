# Barra de pestañas de la OR

**GENERAL**: contiene una rejilla en la que se nos presentan las líneas de la orden de reparación ordenadas por el campo contador de cada línea y por una imputación / incidencia (línea amarilla que indica hacia quien va el cargo y la incidencia ocurrida). Mediante está rejilla podremos consultar, grabar, modificar o eliminar cualquier línea de la OR o imputación.

<mark style="color:green;">Botonera en General:</mark>

**A) IMPUTACIÓN** ![](<../../../../.gitbook/assets/imagen (159).png>) > Al grabar una nueva imputación se nos presentará el formulario de grabación de línea de imputación con los siguientes campos:

<figure><img src="../../../../.gitbook/assets/imagen (163).png" alt=""><figcaption></figcaption></figure>

1.- **Imputación** > muestra las opciones disponible de cargo (cliente, siniestro, interno y garantía - algunas marcas requieren una imputación adicional siendo posible su configuración)

2.- **Tempario** > selección de tempario asociado al alta de la imputación [(véase temparios)](../temparios.md)

3.- **Sección de taller** > departamento del taller a la que pertenecería la intervención a realizar [(véase secciones de taller)](../secciones-de-taller.md)

4.- **Título** > nombre que recibe la avería a intervenir

5.- **Avería / Síntoma** > breve explicación de la avería que permite incluir varias líneas de texto

<figure><img src="../../../../.gitbook/assets/imagen (35).png" alt=""><figcaption></figcaption></figure>

B) **NUEVA LÍNEA DE ARTÍCULO O SERVICIO** ![](<../../../../.gitbook/assets/imagen (164).png>) > Al grabar una nueva línea de artículo o servicio se nos presentará el formulario de grabación con los siguientes campos:

<figure><img src="../../../../.gitbook/assets/imagen (102) (1).png" alt=""><figcaption></figcaption></figure>

1.- **Partida** > indica la imputación destino de la línea pudiendo, en caso de haber más de 1 imputación, pulsar en el botón y seleccionar el destino de la línea entre las distintas imputaciones de la OR.

2.- **Artículo** > campo para introducir la referencia del artículo o servicio tanto usando el localizador como de forma manual. Permite además dar de alta un artículo / servicio o crear buscar una referencia en la tarifa de artículos como "Localizar Referencia":

<figure><img src="../../../../.gitbook/assets/imagen (157).png" alt=""><figcaption></figcaption></figure>

3.- **Check "Pedir a proveedor"** > fuerza pedir al proveedor la línea de artículo / servicio aunque haya stock del artículo

4.- **Imputación** > indicación a modo de aviso de a quien se cargará la línea (no es editable)

5.- **Proveedor** > al rellenar el campo artículo, se rellenará con el proveedor preferente del mismo. Al pulsar la lupa nos mostrará los distintos proveedores disponibles del artículo, así como ver la ficha del seleccionado

6.- **Unidades / Precio / Descuento / Parcial** > campos estandar para aumentar o disminuir la cantidad a añadir a la OR, su precio de venta, el descuento y el parcial. Los 3 primeros campos son editables aunque vengan marcados por la tarifa del artículo, tarifas de ventas o descuentos promocionales.

7.- **Check "Interna"** > la línea irá a la imputación principal, pero no se imprimirá en la OR ni en la factura:

<figure><img src="../../../../.gitbook/assets/imagen (94) (1).png" alt=""><figcaption></figcaption></figure>

C) **AÑADIR LÍNEAS DE TEXTO** ![](<../../../../.gitbook/assets/imagen (160).png>) > añade líneas de texto a la OR. Permite seleccionar la partida de destino:

<figure><img src="../../../../.gitbook/assets/imagen (156).png" alt=""><figcaption></figcaption></figure>

D) **ELIMINAR LÍNEAS SELECCIONADAS** ![](<../../../../.gitbook/assets/imagen (39) (2).png>) > permite eliminar cualquier tipo de línea salvo las imputaciones, que hay que proceder desde la propia línea con doble clic <mark style="color:yellow;">(se avisa que elimina la imputación y las líneas que contiene)</mark> y de los artículos instalados, que hay que proceder del mismo modo, entrando en la línea con doble clic y pulsar "Opciones" > "Eliminar". En líneas con pedidos de compras relacionados, se procederá a la anulación de la línea del pedido de compras.

E) **REFRESCAR VISTA DE LÍNEAS** ![](<../../../../.gitbook/assets/imagen (37).png>) > tras modificar algún elemento como la posición de las líneas en la OR, sirve para actualizar y mostrar el resultado final

F) **ABONAR LÍNEA/S SELECCIONADA/S** ![](<../../../../.gitbook/assets/imagen (108).png>) > realiza un abono de línea creando una nueva línea idéntica a la seleccionada, pero con valor negativo.
