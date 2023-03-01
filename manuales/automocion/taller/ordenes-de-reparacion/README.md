# Órdenes de Reparación

Mediante este menú, podremos grabar, modificar o consultar todas los ordenes de reparación que hemos realizado. Al entrar en ella, nos aparecen varios filtros con calendario, vehículo y cliente, por tipo de OR y por situación de la OR y de los recambios asociados a ella:

<figure><img src="../../../../.gitbook/assets/imagen (9).png" alt=""><figcaption></figcaption></figure>

Algo característico de los documentos orden de reparación son el campo [tipo de OR](../tipos-or.md), la situación de la OR y sus recambios y disponer de 4 a 5 (en Honda) imputaciones distintas como siniestro, cliente, garantía e interno. Los tipos de OR sirven tanto para identificar y clasificar las OR como para un alta más ligera, al permitir que, al indicar un tipo en el alta, se rellene automáticamente un tipo de imputación y un [tempario](../temparios.md).

* <mark style="color:orange;">Tipos de OR</mark>: [véase "Tipos de OR"](../tipos-or.md)
* <mark style="color:orange;">Situación de la OR</mark>:&#x20;
  * Inicialmente una OR se abre como "Pte. aceptar" o como "Presupuesto"
  * Confirmada en cualquier modo de apertura pasa a estado "En curso" y los repuestos asociados a ella podrán estar en situación "Pte. Recibir" para aquellos que no estaban en stock en el momento de confirmar la OR y han generado pedido de compras, "Pte. Instalar" para los recambios que estaban en stock y que han quedado reservados a la OR y "Pte. Recibir / Pte. Instalar" en aquellas ORs en las que se dan ambos casos
  * Sobre los artículos reservados en stock o que hayan sido recibidos (en azul - véase código de colores abajo) se puede realizar la instalación, seleccionado todas las líneas pulsando en el recuadro en blanco situado a la izquierda de "Almacén" o de una en una y pulsando en el botón "Instalar material", pasando las líneas instaladas a color verde.
  * Tras instalar la OR puede quedar "Pte. Facturar", "Facturada" y "Parc. Facturada" para aquellas aún sin facturar, facturadas y las que tienen más de una imputación y sólo se ha facturado una parte de ellas.

<figure><img src="../../../../.gitbook/assets/imagen (11).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:orange;">Imputaciones estándar de la OR</mark>: <mark style="color:yellow;">indican hacia dónde va el cargo del conjunto de líneas incluidas en ella. Si se modifica la línea de la imputación, se modifica el conjunto de líneas:</mark>
  * Cliente: por defecto será el propietario del vehículo, pero se podrá modificar aunque siempre será hacia una entidad tipo cliente
  * Siniestro: permite el uso de la pestaña ["Versión para la compañía" - pulse para ver instrucciones de uso](../../../../faq/ordenes-de-reparacion-ors/version-para-la-compania-en-la-or.md)
  * Interna: el cargo irá a la empresa y habrá que especificar un departamento
  * Garantía: en función de la marca, las garantías que requieran una facturación de la mano de obra se podrán efectuar usando este tipo

1 - NUEVA OR

Permite dar de alta a una nueva orden de reparación, rellenando el siguiente formulario:

<figure><img src="../../../../.gitbook/assets/imagen.png" alt=""><figcaption></figcaption></figure>

El alta de una OR está compuesta por un formulario, donde se introducen los datos generales, como la serie, la fecha, [tipo de orden](../tipos-or.md), respecto al vehículo la matrícula, bastidor y cliente (pulsando tabulador después de introducir cualquiera de los datos anteriores rellenará automáticamente el resto), imputación, avería / síntoma, [tempario](../temparios.md), sección de taller, fechas de recepción y entrega prevista, kilometraje / horas, combustible, teléfono de la entidad y permite añadir y efectos personales.

**Serie**: es un campo imprescindible de rellenar, y por defecto toma el valor definido en la ficha del usuario que graba la OR. Esta serie permite multitud de ajustes debido a su <mark style="color:blue;">capacidad de generar distintos pedidos de compra en función del tipo de pedido del artículo</mark> (urgente, reposición o garantía), <mark style="color:blue;">hasta 4 líneas de facturación</mark>, una por cada imputación posible y <mark style="color:yellow;">avisos por llegada de mercancia reservada a la OR en la pestaña "Avisos"</mark>:

<figure><img src="../../../../.gitbook/assets/imagen (1).png" alt=""><figcaption></figcaption></figure>

Aviso recibido mediante la configuración de la serie OR > pestaña "Avisos":

<figure><img src="../../../../.gitbook/assets/imagen (2) (2).png" alt=""><figcaption></figcaption></figure>

**Fecha de apertura**: se indica aquí la fecha de grabación del documento. Esta fecha debe de estar dentro de los rangos definidos en parámetros.

**Tipo**: permite seleccionar uno de los existentes y que se pueden listar, modificar, borrar y dar de alta desde la opción Automoción > Taller > Tipos OR. El tipo permite organizar y localizar órdenes de reparación del mismo tipo, así como rellenar automáticamente la imputación y el tempario según el alta del tipo de OR que hayamos creado.

**Centro**: este campo solo será visible por aquellas aplicaciones en las que se trabaje con más de un centro de trabajo y así se haya indicado en parámetros. Se utiliza para indicar el centro de trabajo para el que se hace el albarán. Este campo, se rellena automáticamente y solo será editable por aquellos usuarios autorizados.

**Check - Presupuesto**: al marcar el check nos permite rellenar un nuevo campo "Referencia" a fin de control posterior por parte del cliente. La situación de la OR quedará como "Presupuesto" hasta que se confirme la OR que pasará a "En curso". Desde la versión presupuesto es posible crear nuevas versiones usando el botón ![](<../../../../.gitbook/assets/imagen (2).png>) mientras no se haya confirmado. Tanto si se genera una OR como presupuesto como las posteriores versiones del mismo quedarán registradas para su control y posible lectura desde la pestaña "Versiones del presupuesto" (sólo activa cuando se genera una OR como presupuesto).

**Vendedor**: tomará por defecto el vendedor definido en la ficha del cliente o agente. Se podrá modificar manualmente.

**Cliente**: tipo de entidad propietaria del vehículo y a la que se facturará por defecto la OR, aunque es posible modificar la línea de facturación para cambiar la entidad a petición del cliente. Contiene botones incrustados para localizar, grabar o editar el cliente.

**Imputación**:

**Departamento interno**: si la serie del albarán es INTERNA, se podrá seleccionar el departamento para el que se graba dicho albarán.



Barra de pestañas

CONCEPTOS: contiene una rejilla en la que se nos presentan las líneas de albaranes de venta ordenadas por el campo contador de cada línea. Mediante está rejilla podremos consultar, grabar, modificar o eliminar cualquier línea de albarán.

Para grabar una nueva línea, podemos utilizar cualquiera de los métodos utilizados sobre cualquier otra rejilla. Se nos presentará el formulario de grabación de líneas con los siguientes campos:

\- Almacén: indicamos aquí el almacén del que saldrá el material. Estará activo si la serie tiene marcado que permite varios almacenes. De lo contrario, tomará por defecto el almacén definido en la serie.

\- Artículo: campo en el que introducimos la referencia del artículo. Se podrá meter la referencia manualmente, o utilizando la opción Buscar Artículo de los botones incrustados de este campo.

Si no localizamos la referencia en la base de datos de artículos, podemos utilizar la opción Referencia.

Con esta opción, el programa buscará en primer lugar en el fichero de artículos, y si no la encontrara, buscará en el de tarifas. Una vez localizada, se nos presentará el siguiente formulario, desde el que podremos crear la referencia directamente.

Los otros dos botones incrustados que contiene el campo de artículo, son para consultar/editar la referencia seleccionada, o para crear una nueva.

La descripción del artículo tomará por defecto la definida en su ficha, y solo se podrá modificar si el artículo no está incluido en la tarifa.

\- Stock disponible, ubicaciones y descuento: son campos que muestran información directa del artículo, el stock disponible, las ubicaciones del artículo y el descuento de compra.

\- Cantidad: indicamos aquí las unidades que vayan a salir.

\- Precio: importe de venta del artículo. En los presupuestos, pedidos, albaranes de venta y en las órdenes de reparación, tanto el precio de venta como el descuento se calcularán en función a la tabla de descuento definida en el vendedor, y si no tuviera, la definida en el cliente. El funcionamiento específico de las tablas de descuentos se explicarán en el menú comercial, opción B – tablas de descuentos. Si no se hubiera indicado ninguna tabla de descuentos, el precio será el definido en la ficha de la referencia.

\- Descuento: porcentaje de descuento que se le realizará al cliente.

\- Parcial: valor total del artículo (sin sumar los impuestos) resultante de multiplicar las unidades pedidas por el precio menos los descuentos.

\- Costo: valor de compra del artículo.

\- Tipo de IVA: tomará por defecto el tipo de IVA definido en la ficha del artículo si el albarán tiene el tipo de IVA general. De lo contrario, será el 0 %.

\- Contador: campo destinado a ordenar todas las líneas del albarán. Mantendrán el orden de menor a mayor en la presentación de las rejillas y en los impresos. Se podrá modificar para variar el orden según las necesidades.

\- Operación: estos campos se utilizan para imputar una línea de albarán de venta a un cheque regalo de una operación. Mediante el localizador presentado, veremos los vales activos que tiene el cliente / agente. Al seleccionar uno de ellos, se presentarán en la línea del albarán los datos relativos al cheque regalo.

Opciones de las líneas de albarán

\- Aceptar: con este botón guardamos los cambios realizados.

\- Cancelar: abortamos el alta o modificación de la línea.

Para eliminar una línea de albaranes de venta, tendremos que marcar la línea a eliminar pulsar el botón Supr del teclado o el botón secundario del ratón y seleccionar formulario de baja. Nos aparecerá un formulario desde el que podremos eliminar la línea.

\-TOTALES: presenta el desglose de importe totales del albarán de venta.

\-INTERNAS: muestra el beneficio de las líneas incluidas en el albarán de venta.

\-SEGUIMIENTOS: se podrá grabar seguimientos relacionados con los albaranes de ventas, en esta pestaña se presentan los grabados.

Opciones desde un albarán de venta:

Aceptar: si pulsamos esta opción, quedarán guardados todos los cambios que hayamos realizado sobre la ficha del albarán.

Cancelar: con este botón, saldremos de la ficha del albarán sin guardar los posibles cambios que hayamos realizado. Se puede pulsar la tecla ESC para ejecutar esta opción.

Borrar: sirve para eliminar el albarán, y solo lo podrán hacer usuarios supervisores y cuando no esté facturado.

Notas: presenta un formulario en el que se podrán incluir notas relacionadas con el albarán.

Facturar: facturará el albarán. Se podrá indicar en las series de las facturas que se imprima el documento al generar la factura, y por tanto, si este estuviera marcado en el momento de facturar desde este botón, se imprimirá la factura generada.

Imprimir: imprime el albarán de venta con el modelo indicado en la serie del albarán.

Impresión selectiva: imprime el albarán de venta con el modelo que se seleccione al pulsar el botón. Nos aparecerá un recuadro en el que tendremos que indicar el modelo.

Exportar a TXT: mediante este botón podremos generar un fichero en formato TXT con la cabecera y el contenido del albarán de venta. Tendremos que seleccionar la carpeta donde guardaremos el fichero. El nombre de este será el código del albarán de venta (serie + número). Este fichero podrá ser utilizado por el cliente o agente del albarán para grabar directamente en su base de datos la compra realizada. La estructura del fichero podrá ser solicitada a los técnicos de Velmotor.

Importar de TXT: mediante este botón podremos crear un albarán de venta a partir de un fichero TXT generado desde cualquier aplicación Velmotor, que contenga la estructura de un albarán de compra.

2 - BUSCAR

Localizador de albaranes de ventas a través de distintos criterios. Nos permite consultar, borrar o modificar la información de un albarán. Al acceder a esta opción encontraremos la siguiente pantalla:

Este localizador nos permite buscar un albarán por los siguientes criterios:

\-NÚMERO, FECHA, CLIENTE, NOMBRE DEL CLIENTE y VENDEDOR / MES: el cursor se irá situando en el albarán cuyo número, fecha, código de cliente, nombre del cliente coincida con lo seleccionado.

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

&#x20;
