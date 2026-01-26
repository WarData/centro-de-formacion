# Albaranes Gastos

**ALBARANES DE GASTOS**

Mediante esta opción, podremos grabar, modificar o consultar todos los albaranes de gastos de los servicios o productos recibidos de nuestros acreedores. Al entrar en ella, nos aparece un menú con calendario en el que se nos presentan diferentes opciones, un calendario que contendrá por defecto la fecha de hoy y se podrá modificar, y una rejilla que presentará todos los albaranes de gastos con la fecha indicada en el calendario.

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

**1.- NUEVO ALBARÁN**

Permite dar de alta a un nuevo albarán de gastos mediante el siguiente formulario:

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Al igual que los pedidos de material y los demás documentos de compra y venta, los albaranes están compuestos por su cabecera, donde se guardan todos los datos generales del albarán, y las líneas, donde se va guarda el detalle de los gastos, referencia relacionada, cantidad, importe, etc.

La cabecera de los albaranes de compras está compuesta por los siguientes campos:

* **Serie**: campo que clasifica a los albaranes por grupos y dependiendo de la configuración de la serie, el albarán tomará unos valores u otros. En el botón "lupa" es posible seleccionar entre las distintas series. Véase ["Series"](../configuracion/series-de-documentos.md) para configuración y ["Perfiles"](../configuracion/opciones-especiales/permisos-de-usuario.md) para asignación automática de series a un perfil determinado.
* **Número:** todos los documentos están clasificados por su serie y un número, que siempre será por defecto el siguiente al último grabado de la misma serie. Tanto el número como la serie de un documento se podrán modificar manualmente una vez dado de alta el documento, aunque, a menos que sea imprescindible, no es aconsejable.
* **Fecha:** se indica aquí la fecha de grabación del documento. Esta fecha debe de estar dentro de los rangos definidos en [parámetros](../configuracion/parametros/).
* **Hora:** se encuentre situado justo a la derecha de la fecha, y muestra la hora de grabación del documento. No es manipulable por el usuario.
* **Referencia:** podemos guardar en este campo la referencia del albarán que hemos recibido del acreedor. Será una buena forma de identificar un documento concreto en los localizadores de albaranes de gastos.
* **Centro:** este campo solo será visible por aquellas aplicaciones Winmotor Multi-Centro, en las que se trabaje con más de un centro de trabajo y así se haya indicado en parámetros. Se utiliza para indicar el centro de trabajo para el que se graba el albarán. Este campo, se rellena automáticamente y solo será manipulable por aquellos usuarios autorizados.
* **Régimen de IVA:** este campo tomará por defecto el tipo de IVA definido en la ficha del proveedor seleccionado en el albarán. Se podrá modificar manualmente.
* **Acreedor:** indicamos aquí el acreedor, cuyo formulario de opciones contiene cuatro botones insertados para poder localizar el acreedor deseado, crear uno nuevo, editarlo y cambiar los datos:

<figure><img src="../../.gitbook/assets/image (5) (1) (1).png" alt=""><figcaption></figcaption></figure>

* **Dirección, CIF, tipo de pago y vencimientos:** muestra, respectivamente, la dirección, CIF, tipo de pago y vencimientos del acreedor seleccionado. Se podrán modificar sin que estos cambios afecten a la ficha del acreedor. Recordar que tanto el tipo de pago como los vencimientos son campos relacionados con su propia tabla de datos en las que se graban las diferentes posibilidades que se pueden escoger. El acceso a estas dos tablas, lo podrás encontrar en el apartado **Submaestros > Administración >** [**Tipos de pago**](../submaestros/administracion-1/tipos-de-pago.md) **y** [**Vencimientos**](../submaestros/administracion-1/vencimientos.md)

**Barra de pestañas**

* **Líneas:** contiene una rejilla en la que se nos presentan las líneas del albarán de gastos ordenadas por el campo contador de cada línea. Mediante está rejilla podremos consultar, grabar, modificar o eliminar cualquier línea del albarán o añadir / borrar / modificar líneas de texto. El alta de un artículo se realiza con doble clic en la rejilla en blanco o con el botón ![](<../../.gitbook/assets/image (18).png>):

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

* **Totales**: muestra la información totalizada de bases, porcentajes de IVA, importe de IVA y parciales, así como importe pagado y pendiente si es que han existido anticipos de pago asociados al documento:

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

* **Observaciones**: permite añadir texto libre que únicamente aparecerá en este documento. Es posible imprimir el contenido en los informes de impresión indicándolo al departamento de soporte (es posible que la realización incluya costes de programación)
* **Archivos**: permite almacenar en el servidor cualquier tipo de archivo para su apertura en remoto. [Véase "Archivos"](../maestros/articulos/ficha-del-articulo/archivos.md)

![](<../../.gitbook/assets/imagen (43) (1).png>)

* **Seguimientos**: añade asuntos a la agendas de los usuarios para el control del documento, permitiendo en ésta añadir avisos a horas programables.
* **Acciones**: control de acciones sobre el documento en función de qué, quién y cuándo se ha realizado.

**Alta de líneas**

Al hacer doble clic sobre cualquier línea vacía o pulsar el botón del lateral izquierdo "Nueva línea de artículo o concepto" se nos presentará el formulario de grabación de líneas con los siguientes campos:

\- Artículo: campo en el que introducimos la referencia del artículo que vamos a recepcionar. Se podrá meter la referencia manualmente, o utilizando la opción Buscar Artículo de los botones incrustados de este campo.

\- Almacén: indicamos aquí el almacén en el que entra la mercancía. Será por defecto el definido en la serie del albarán, y no se podrá modificar a menos que así lo indique también en la serie.

Si no localizamos la referencia en la base de datos de artículos, podemos utilizar la opción Referencia, siempre que hayamos importado una tarifa de artículos del proveedor. ["Véase Importador de Tarifas"](../../tutoriales/como-crear-un-importador-de-tarifa-por-marca/):

<figure><img src="../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

Los otros botones incrustados que contiene el campo de artículo, son para consultar/editar la referencia seleccionada, <mark style="color:yellow;">**localizar servicio (suele ser la línea más habitual en gastos)**</mark> o modelo, además de permitir su alta.

La descripción del artículo o servicio tomará por defecto la definida en su ficha, pero podrá ser modificada manualmente.

\- Unidades: es un campo manipulable por el usuario, y e indicaremos aquí las unidades que hemos recibido.

\- Precio: importe de compra del artículo o servicio

\- Descuento y Descuento 2: podremos indicar hasta dos posibles descuentos. Si se modifican, también saltará la pantalla de control de precios del artículo.

\- Parcial: valor total del artículo (sin sumar los impuestos) resultante de multiplicar las unidades recibidas por el precio, menos los descuentos.

\- % IVA: tomará el porcentaje de IVA definido en la ficha del artículo o servicio si en el albarán se tienen que calcular los impuestos y <mark style="color:yellow;">**no permitirá su modificación, es imprescindible modificarlo en el artículo o servicio antes de añadir la línea- recomendamos crear varios servicios añadiendo al nombre el porcentaje de IVA como por ejemplo COMIDA10 para comidas de empresa con IVA al 10%**</mark>:

<figure><img src="../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

**Opciones de las líneas de albarán**

* **Aceptar**: con este botón guardamos los cambios realizados.
* **Cancelar**: abortamos el alta o modificación de la línea.

Para eliminar una línea de albarán, tendremos que hacer doble clic en la línea a borrar o editar, se abrirá la ventana del artículo o servicio y pulsaremos el botón "Eliminar":

<figure><img src="../../.gitbook/assets/image (5) (1).png" alt=""><figcaption></figcaption></figure>

* Eliminar: borra la línea del albarán de gastos
* Auditoría: muestra la fecha y hora de creación y modificación a la vez que el usuario de cada uno y las operaciones sobre el documento junto a la fecha, tipo de operación, hora, usuario y log:

<figure><img src="../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

**Opciones desde un albarán de gastos:**

* **Aceptar:** si pulsamos esta opción, quedarán guardados todos los cambios que hayamos realizado sobre la ficha del albarán.
* **Eliminar:** el botón solo estará activo si el albarán no está facturado, si se pulsa, se eliminará completamente.
* **Facturar:** este botón sirve para facturar el albarán. Se nos pedirá confirmación del proceso, y a continuación aparecerá en pantalla la factura generada.
* **Imprimir:** podemos imprimir el albarán mediante este botón.

<figure><img src="../../.gitbook/assets/image (6) (1).png" alt=""><figcaption><p>Durante el alta del albarán</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Tras facturar</p></figcaption></figure>

**2 - BUSCAR ALBARÁN**

Localizador de albaranes de gastos a través de distintos criterios. Nos permite consultar, borrar o modificar la información de un albarán. Al acceder a esta opción encontraremos la siguiente pantalla:

<figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

Este localizador nos permite buscar un albarán por los siguientes criterios:

* **Número de documento:** el cursor se irá situando en el albarán cuyo número coincida con el seleccionado
* **Fecha:** el cursor se irá situando en el primer albarán cuya fecha coincida con la seleccionada
* **Referencia**: búsqueda relacionada con el campo "Referencia" del albarán
* **Nombre de entidad:** el cursor se irá situando en el albarán cuya razón social vaya coincidiendo con lo introducido en el campo de edición.

Para acceder a la ficha del albarán de compra seleccionado, se puede hacer doble clic sobre él o teclear el botón intro del teclado.

El formulario que se presenta es el mismo que el de grabación.

**3 - LISTADO**

Esta opción lanza una búsqueda que nos presentará un listado de albaranes de gastos. Este listado se puede acotar a través del filtro de búsqueda que se presenta a continuación:

<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

Se podrá filtrar por una determinada serie o todas, por un intervalo de fechas, acreedor (entidad), centro, tipo de pago, estado (facturado o pendiente) y por estado del albarán (facturados, pendientes de facturar o todos). Después de indicar los criterios deseados, nos aparecerá una rejilla con los albaranes que cumplan esas condiciones.

**4 – FACTURACIÓN**

Mediante esta opción, podremos crear facturas de gastos en tanda por todos aquellos albaranes de gastos pendientes de facturar. Al ejecutar la opción nos aparecerá el siguiente formulario de búsqueda, en el que podremos filtrar por varios criterios como acreedor, fecha, serie, tipo de pago, importe mínimo a facturar y fecha de facturación:

<figure><img src="../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

El funcionamiento de esta opción es bastante sencillo, bastará con seleccionar los albaranes que se quieran facturar, y a continuación pulsar sobre el botón situado en la barra de herramientas inferior. El programa se encargará de crear una factura dividiendo los albaranes por series, tipos de pagos, proveedor y régimen de IVA.

![Selección de 6 albaranes de gastos](<../../.gitbook/assets/imagen (40) (1).png>)

![Al facturar, se muestra el resultado de la facturación](<../../.gitbook/assets/imagen (41) (1).png>)
