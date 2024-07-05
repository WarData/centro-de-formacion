# Teoría

<mark style="color:yellow;">**Qué es el integrador bancario**</mark>&#x20;

Es un módulo opcional que el cliente puede contratar con Winmotor y sirve para descargar los movimientos bancarios de todas aquellas cuentas o tarjetas que hayamos dado de alta en la base de datos. El integrador los analiza y según esté configurado, genera en la base de datos los registros de tesorería o asientos contables necesarios.  Es por lo tanto una herramienta que reducirá enormemente el tiempo que los contables y administrativos de la empresa dedican a realizar diariamente este trabajo rutinario.&#x20;

Según se van descargando registros y el contable va definiendo la interpretación de cada uno, el sistema va “aprendiendo” de manera que cada vez serán menos los registros bancarios que haya que resolver manualmente.&#x20;

Integra por otro lado una herramienta para el gerente que le facilita la consulta de los saldos y movimientos de las cuentas aportándole además un análisis de los gastos e ingresos de cada una de ellas.

<mark style="color:yellow;">**Fases del integrador**</mark>&#x20;

1. **Importación de registros**&#x20;

Para la importación de registros el usuario no tiene que hacer absolutamente nada, Winmotor configura las distintas descargas de datos de forma que se hacen automáticamente. Si es importante entender que existen dos fases en la descarga de cada movimiento:

●        **Descarga intradía:**

* En la ficha de cada movimiento descargado verás un apartado “Movimiento intradía” donde se muestra el código de clasificación que este sistema aporta y la descripción que recoge de la entidad.
  * El código del movimiento que aporta la entidad en este nivel de descarga es bastante pobre y en muchos casos confunde más que aclara de qué se trata el mismo. Puedes consultar la lista en el menú del integrador en la opción “Tipos de movimiento - agregador bancario”&#x20;

●        **Descarga según formato de la norma 43**

*   Esta descarga aporta mucha más información al sistema en cuanto al tipo de movimiento bancario, pero sólo se puede hacer al día siguiente de la fecha de la operación. Al hacer esta descarga el programa conocerá dos datos fundamentales:

    * Concepto común: es un código de clasificación del movimiento que viene determinado por el consejo superior bancario que aunque algo anticuado aporta información sobre el mismo.
      * Puedes consultar la lista de estos conceptos en el menú del integrador en la opción “Conceptos comunes - Norma 43”.
      * Inexplicablemente algunos bancos como el BSCH no aportan este dato, lo rellenan siempre con ceros.
    * Concepto propio: es una codificación interna que hace cada entidad mucho más amplia y detallada que el concepto común y que no deja duda en cuanto al tipo de movimiento descargado.


* Estos campos los podrá ver en el registro descargado siempre que lo consulte al día siguiente de su “Fecha de operación”.
* La mayoría de entidades no tienen activo este sistema por defecto, hay que solicitar su activación. En algunos casos lleva a engaño que en la consulta de movimientos en la página del banco aparece como opción “Norma 43” pero no hace una descarga real en este formato, simplemente nos da un Excel con los campos que se ven al descargar la norma 43.
* Hay que tener en cuenta que cada entidad tiene un distinto proceso de “consolidación de movimientos” que en algunos casos puede incluso implicar un cambio de fecha en los mismos,  aunque es bastante raro. Si al hacer la descarga en el formato de la norma 43 la aplicación no localiza el registro correspondiente ya descargado por el sistema intradía se generará un “registro provisional” que el usuario tendrá que editar para decidir si es alguno de los ya descargados con alguna diferencia o hay que añadir el registro.&#x20;

2. **Interpretación**&#x20;

La interpretación de los registros descargados implica no sólo entender qué es cada movimiento sino relacionarlo dentro de lo posible con un documento o con otra ficha contenida en la base de datos: en informática a este proceso se le llama _“parseo”_. El integrador bancario divide el proceso de interpretación en tres fases fundamentales:

●        ¿Qué tipo de movimiento es?

●        ¿Con qué entidad o cuenta bancaria está relacionado?

●        ¿A qué documento corresponde?&#x20;

<mark style="color:blue;">**Tipo de movimiento**</mark>&#x20;

Winmotor hace una clasificación interna de los movimientos y en base a ésta trata de localizar el documento o ficha relacionado.

Este campo se calcula según los códigos aportados por la entidad que hemos mencionado anteriormente y en la lista de movimientos aparece como “Concepto”.&#x20;

Los tipos de movimiento en los que Winmotor clasifica los registros bancarios son:&#x20;

●       <mark style="color:blue;">Gastos</mark>

* Amortización de préstamo
* Gastos bancarios
* Devolución a cliente
* Impuestos
* Pago a empleado (Nómina)
* Pago a proveedor - acreedor
* Traspaso - salida

●       <mark style="color:blue;">Ingresos</mark>

* Ingresos bancarios
* Cobro a cliente
* Devolución a proveedor
* Remesa de efectos
* Traspaso - entrada&#x20;

No es posible que el programa por sí sólo al descargar los datos sepa interpretar desde el primer día todos los tipos de movimientos: el único dato que tiene es si el importe es positivo o negativo y el contenido de la descripción del movimiento que le da el banco. Necesita por lo tanto “aprender” a identificar cada uno de estos tipos según el contenido de la descripción y el usuario tiene que ir dándole las claves para ello. Más adelante veremos cómo se hace esto.&#x20;

<mark style="color:green;">**Entidad**</mark>&#x20;

Para los tipos de movimientos que están vinculados con documentos de la aplicación el integrador tiene primero que localizar la entidad. Los tipos de movimientos que requieren una entidad son:

●        <mark style="color:green;">Gastos</mark>

* Devolución a cliente
* Pago a empleado (Nómina)
* Pago a proveedor - acreedor

●       <mark style="color:green;">Ingresos</mark>

* Cobro a cliente
* Devolución a proveedor&#x20;

Para esta identificación cuenta con el contenido del campo “descripción” que el banco ha aportado. Dado que muchas veces se hace complicado identificar la entidad hay varios sistemas que ayudan al programa a hacerlo y los estudiaremos en el siguiente bloque. Si es importante entender que el integrador utiliza todos los datos que están a su alcance en la base de datos para identificar cada campo. Si por ejemplo tenemos un cobro y la entidad localizada no tiene marcado que es cliente pero si proveedor o acreedor, el integrador interpretará automáticamente que se trata de un abono a proveedor y buscará facturas recibidas de abono.&#x20;

El integrador utiliza un tipo añadido especial de entidad: la “entidad financiera”. Nos referimos a las entidades que financian operaciones de ventas o de compras y que por lo tanto al recibir el cobro o el pago lo que vemos en el registro bancario es el nombre de esa entidad. En el bloque práctico veremos cómo tiene el usuario que definir y gestionar este tipo de entidades para que el integrador pueda identificar el o los documentos que se están cobrando o pagando.&#x20;

<mark style="color:orange;">**Cuenta**</mark>&#x20;

Para los registros tipo “Traspaso salida” y “Traspaso entrada” el integrador necesita identificar en lugar de una entidad, una cuenta de tesorería de contrapartida. Por defecto los “Traspaso entrada” el integrador los registra como nulos ya que el movimiento que se va a contabilizar es el de salida. Existe una excepción para esta regla que es el caso de los abonos de TPV; en el bloque siguiente explicaremos cómo funciona.&#x20;

<mark style="color:red;">**Documento**</mark>&#x20;

Es el dato más complejo de localizar dado que se pueden dar muchas casuísticas. Lo importante es entender que inicialmente el integrador busca documentos y registros de cartera por el importe, la entidad y la fecha.&#x20;

Además de estos datos el integrador hace varias búsquedas en el contenido de la descripción:&#x20;

●        Códigos de documentos Winmotor

●        Código del proveedor en facturas recibidas&#x20;

Para el caso de las transferencias es prioritario dar instrucciones a los vendedores para que pidan a los clientes que van a pagar por transferencia que indiquen el número de documento Winmotor en la misma: esto facilitará enormemente el trabajo de localización.&#x20;

Lo importante es saber que el programa sólo buscará documentos pendientes de pago o de cobro y que no estén ya relacionados con otro registro bancario.&#x20;

En el caso de que el cobro o pago esté relacionado con varios documentos el integrador no los podrá localizar, pero mostrará un asistente para hacer una multiselección presentando documentos de la misma entidad y en un intervalo de fechas que puedan cuadrar con el registro.&#x20;

3. **Cierre**&#x20;

El cierre del registro sólo se puede hacer si se ha localizado su contrapartida y supone la generación de un registro de tesorería, un asiento contable o la contabilización de una remesa. Un registro cerrado ya no se puede modificar pero existe una opción para “reaperturarlo”.&#x20;

<mark style="color:orange;">Los tipos de cierre</mark> por lo tanto pueden ser:

●        <mark style="color:orange;">Por tesorería:</mark> el movimiento bancario está relacionado con un documento de la aplicación que habrá que cobrar / pagar  a través de un asiento en el módulo de tesorería.

●       <mark style="color:orange;">Por contabilidad:</mark> para el resto de tipos de movimientos excepto las remesas el cierre del registro supone la generación de un asiento contable. Si el movimiento es un traspaso entre cuentas la contrapartida será la de la otra cuenta. Si son gastos o ingresos bancarios la contrapartida está definida en el propio tipo de movimiento y si es un pago a un empleado será la cuenta del empleado.

●        Como caso excepcional están <mark style="color:orange;">las remesas:</mark> el cierre de un registro tipo remesa es igual a la acción que supone pulsar el botón “Contabilizar” de la remesa. Por lo tanto, si cerramos un registro de este tipo la aplicación marcará la remesa como contabilizada y generará el asiento contable.&#x20;

Por cada tipo de movimiento se gestiona el tipo de cierre y los datos relativos a este proceso.&#x20;

Aunque por defecto en todos los tipos de movimientos está definido que el cierre se haga manualmente se puede marcar que sea automático. El cierre automático implica que si se ha localizado la contrapartida de un movimiento se ejecute el cierre automáticamente, sea del tipo que sea. Para el caso del cierre por tesorería se puede incluso definir que se contabilice también automáticamente con lo que facilitamos aún más el trabajo del contable.
