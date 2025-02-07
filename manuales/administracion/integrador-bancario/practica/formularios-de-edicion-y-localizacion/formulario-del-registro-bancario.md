# Formulario del registro bancario



<figure><img src="../../../../../.gitbook/assets/imagen (21).png" alt=""><figcaption></figcaption></figure>

Dependiendo del estado y del tipo del registro la información que vemos en este formulario cambia. Mostramos arriba un registro de pago a proveedor / acreedor en estado “Confirmado”, dado que es uno de los más completos que podemos ver. Pasamos a explicar qué hace cada uno de los botones que vemos:

●        ![](<../../../../../.gitbook/assets/imagen (1) (1) (1) (1) (1) (1) (1) (1).png>) Modificar el tipo de movimiento. Es una función que tendremos que utilizar más de una vez al comenzar a trabajar con el integrador ya que como hemos explicado anteriormente el sistema tiene que “aprender” a identificar el tipo de movimiento según el contenido de la descripción de cada registro.

○        Al pulsar el botón según estemos en un gasto o un ingreso el programa presenta la lista de movimientos del tipo correspondiente:

<figure><img src="../../../../../.gitbook/assets/imagen (2) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

○        Simplemente hay que hacer doble clic seleccionando el que queremos aplicar.

○        Dado que hemos aplicado un cambio el sistema automáticamente nos propone establecer una regla para que cuando en el futuro descarguemos un movimiento de este tipo sepa identificarlo y aplicarle el tipo que hemos seleccionado. Imaginemos que tenemos este registro bancario:

<figure><img src="../../../../../.gitbook/assets/imagen (5) (1) (1).png" alt=""><figcaption></figcaption></figure>

Supongamos que es la primera vez que hemos descargado este tipo de movimiento que en realidad es de “Gastos bancarios”. Pulsamos el botón de modificar el tipo y seleccionamos después en la lista “Gastos bancarios”

<figure><img src="../../../../../.gitbook/assets/imagen (4) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

●        El programa nos pedirá confirmación para este cambio y a continuación presentará esta ventana:

<figure><img src="../../../../../.gitbook/assets/imagen (3) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

&#x20;

●        En esta se presenta palabra a palabra el contenido de la descripción del movimiento excluyendo las cadenas numéricas.

●        Se trata de seleccionar aquellas palabras que consideremos que en el futuro servirán para identificar el tipo de movimiento “Gastos bancarios” en cualquier registro que descarguemos de cualquier banco.

●        Podemos seleccionar una o varias palabras, pero si son más de una la selección debe ser correlativa.

<figure><img src="../../../../../.gitbook/assets/imagen (6) (1).png" alt=""><figcaption></figcaption></figure>

&#x20;

●        Hemos seleccionado en el ejemplo toda la cadena “ADEUDO POR DOMICILIACI”. Esta selección se guarda en el tipo de movimiento y a partir de este momento siempre que el programa lea en un movimiento de gastos esta cadena identificará el movimiento como “Gastos bancarios”.

●        Es importante tener en cuenta que esta localización es para gastos. Es decir, si entrara un registro de ingresos con esa misma cadena el programa nunca lo aplicará a “Gastos bancarios”.&#x20;

●        ![](<../../../../../.gitbook/assets/imagen (7) (1).png>) Ampliación de datos de lectura: es sólo un formulario de consulta y nos presenta en detalle todos los datos que hemos descargado del banco tanto en la descarga intradía como en la de la Norma 43.

<figure><img src="../../../../../.gitbook/assets/imagen (8) (1).png" alt=""><figcaption></figcaption></figure>

●        El primer código que vemos se corresponde con el que da el proveedor del servicio de descarga intradía : 18 - pago de recibos

●        Dentro de la Norma 43 vemos:

○        El “concepto común” según el Consejo superior bancario: 03 - Adeudos - Recibos - Letras - Pagos por su cuenta.

○        El “concepto propio” que asigna la entidad, en este caso el BBVA a este tipo de movimiento: 136 - Adeudo a su cargo.

○        La referencia y el concepto son datos de extensión que obtenemos también en la descarga de la norma 43.

●        Es por esto que es importante para el caso de registros no reconocidos en la descarga intradía esperar a la descarga de la Norma 43 ya que ésta siempre aporta más información.&#x20;

●        El siguiente botón que encontramos en el formulario del registro es para la “Gestión de la entidad”.

&#x20;

<figure><img src="../../../../../.gitbook/assets/imagen (9) (1).png" alt=""><figcaption></figcaption></figure>

●        Pulsando en el lápiz accedemos a un formulario especial para editar, eliminar y/o modificar la entidad:

&#x20;

<figure><img src="../../../../../.gitbook/assets/imagen (10) (1).png" alt=""><figcaption></figcaption></figure>

●        En el formulario vemos el código y el nombre fiscal y comercial de la entidad en caso de tenerlo.

●        Debajo vemos los tipos de entidad que tiene definidos.

●        ![](<../../../../../.gitbook/assets/imagen (11) (1).png>) El primer botón simplemente edita la ficha de la entidad.

●       ![](<../../../../../.gitbook/assets/imagen (12) (1).png>) Con este quitamos la entidad del registro

●        ![](<../../../../../.gitbook/assets/imagen (15) (1).png>) El botón localizar aparecerá cuando no haya entidad definida. Es muy importante tener en cuenta que si en un registro que no había entidad la aplicamos con el localizador y aceptamos, el sistema lanzará automáticamente una búsqueda de documentos que puedan cuadrar con el registro y la entidad localizada y en caso de localizarlo lo asigna automáticamente.

![](<../../../../../.gitbook/assets/imagen (14) (1).png>) Este es el “Asistente para guardar alias de localización”.

Lo explicamos: de la misma manera que podemos guardar una regla de localización para un tipo de movimiento las podemos guardar también para las entidades. Imaginemos que en un registro tenemos esta descripción:&#x20;

“2024064001308335-ADEUDO-POR-DOMICILIACI-SUCARG-ES15000A36494706-ES40000B90102195-187451-COREVELNEO-04MA-67740-”&#x20;

Tenemos claro que la entidad en este caso es “Velneo” pero lógicamente en su ficha aparece como tal y no como “COREVELNEO”. &#x20;

Primero asignaremos al registro la entidad “Velneo” utilizando el localizador de entidades.&#x20;

A continuación pulsando el botón del asistente nos aparecerá como en el caso de los tipos de movimientos, una lista de palabras contenidas en la descripción del registro para que seleccionemos aquella o aquellas con las que queremos que en el futuro se pueda identificar a la entidad que hemos seleccionado:

&#x20;

<figure><img src="../../../../../.gitbook/assets/imagen (16) (1).png" alt=""><figcaption></figcaption></figure>

●        Al seleccionar la palabra “COREVELNEO” y aceptar, el integrador la guardará en la ficha de la entidad como “Alias” de Velneo y en el futuro siempre que en un registro aparezca esta palabra el sistema lo asociará a la entidad Velneo.

●        Podemos consultar esta información en la ficha de la entidad en la pestaña “Integrador” donde aparecen los “Alias”  que se le han aplicado.

●        A diferencia del caso de los tipos de movimientos la utilización del alias en las entidades no se hace por cadenas sino por palabras. Es decir si para el ejemplo de la entidad Velneo en su lista de alias aparece: “COREVELNEO-VELNEOSOFT” el programa no asociará en el futuro esa entidad a un registro que contenga esa cadena completa sino a cualquiera que contenga la palabra “COREVELNEO” o “VELNEOSOFT”.

●        En el campo “Alias” de la entidad se quedan siempre las palabras guardadas separadas por guiones.&#x20;

●        La siguiente zona que encontramos en el formulario es la relativa  al documento:

&#x20;&#x20;

<figure><img src="../../../../../.gitbook/assets/imagen (17) (1).png" alt=""><figcaption></figcaption></figure>

●        Además de los datos relativos a la factura en este caso, vemos un botón para editarla y otro para borrar la relación: es decir “quitaríamos” esa factura de este registro para localizar después la correcta.

●        La localización de un nuevo documento se hace siempre desde el botón de la rejilla específico para esto que se explica más adelante.&#x20;

●      **Gastos bancarios**

&#x20;         ○        El programa contempla para todos los registros de pago que pueda haber una cantidad aplicable a gastos bancarios, tanto para traspasos como para pagos a proveedores o empleados.l

&#x20;         ○        Si se trata de un pago a proveedor o a empleado se imputará por defecto la diferencia entre el documento a pagar o el salario del empleado a esta partida. En cualquier caso el usuario puede modificarla.

&#x20;         ○        Al cerrar un registro que tenga un importe definido en gastos bancarios si son pagos de factura o a empleados tomarán siempre la cuenta contable de gastos que esté definida en la cuenta bancaria. En el resto de casos, si hay cuenta definida en el tipo de movimiento tomará esta cuenta y si no la hay tomará la de la cuenta bancaria.

●        **A compensar**

&#x20;         ○        Otro caso que se puede dar que provoque diferencias en un cobro o pago pueden ser los “importes a compensar”. Éstos se contemplan en los cobros y pagos de cartera y son la posible diferencia que puede haber entre lo que hay pendiente de cobro o pago en una factura y lo que se cobra o paga en el movimiento bancario.

&#x20;         ○        Según la compensación sea sobre un cobro o un pago se utilizarán las cuentas contables definidas en parámetros - administración - contables - general: “Compensación en cobros / pagos”.

●        ![](<../../../../../.gitbook/assets/imagen (18) (1).png>) **Cerrar el registro** ![](<../../../../../.gitbook/assets/imagen (19) (1).png>)

&#x20;         ○        Este botón sólo aparecerá si el registro ha llegado a estado confirmado y no está activado en este tipo de movimiento el cierre automático.

&#x20;         ○        El sistema pedirá confirmación y tal como se explica en el punto 3 del bloque de teoría generará un asiento contable, uno de tesorería o ambos.

&#x20;         ○        El registro pasará a estado “Cerrado” y presentará un candado en la última columna del listado. Si hacemos doble clic nos mostrará el asiento de tesorería generado, el asiento contable o ambos.

●        ![](<../../../../../.gitbook/assets/imagen (20) (1).png>) Opciones especiales: según el estado y el tipo del registro nos aparecerán las siguientes opciones:

&#x20;         ○        Registros abiertos

&#x20;         ■     **Crear cobro/pago manual**

&#x20;                   ●        Para movimientos relativos a cobros / pagos de documentos (también a devoluciones) aparecerá esta opción para cobrar o pagar según sea el tipo de movimiento.

&#x20;                   ●        Seleccionando esta opción el programa ignora si hay o no entidad y/o documento localizado y lo que hace es crear un asiento de tesorería aplicando la fecha, la cuenta bancaria y el importe del registro.

&#x20;                   ●        Al terminar el proceso marcará el registro como cerrado.

&#x20;         ■       **Crear asiento manual**

&#x20;                   ●        Esta opción aparece para cualquier tipo de movimiento

&#x20;                   ●        Pulsando este botón se genera un asiento contable en la fecha del registro bancario incluyendo un primer apunte con la cuenta contable relativa a la cuenta bancaria y el importe del asiento.

&#x20;                   ●        Al terminar el proceso marcará el registro como cerrado.

&#x20;        ■        **Cierre neutro**

&#x20;                   ●        Esta opción no hace nada más que marcar el registro actual como cerrado sin generar ni modificar ningún dato en todo el programa.

&#x20;        ○        **Registros cerrados**

&#x20;        ■       **Reaperturar**

&#x20;                   ●        Este botón deshace completamente la operación de cierre que hubiera ejecutado eliminando el registro de tesorería generado, el asiento contable o ambos.

&#x20;                   ●        Al ejecutar la opción el registro vuelve al estado “Confirmado”.
