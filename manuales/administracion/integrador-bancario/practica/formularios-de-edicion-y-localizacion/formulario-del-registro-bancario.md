# Formulario del registro bancario



Dependiendo del estado y del tipo del registro la información que vemos en este formulario cambia. Mostramos arriba un registro de pago a proveedor / acreedor en estado “Confirmado”, dado que es uno de los más completos que podemos ver. Pasamos a explicar qué hace cada uno de los botones que vemos:

●        ![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image004.jpg) Modificar el tipo de movimiento. Es una función que tendremos que utilizar más de una vez al comenzar a trabajar con el integrador ya que como hemos explicado anteriormente el sistema tiene que “aprender” a identificar el tipo de movimiento según el contenido de la descripción de cada registro.

○        Al pulsar el botón según estemos en un gasto o un ingreso el programa presenta la lista de movimientos del tipo correspondiente:

○        ![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image006.jpg)

○        Simplemente hay que hacer doble click seleccionando el que queremos aplicar.

○        Dado que hemos aplicado un cambio el sistema automáticamente nos propone establecer una regla para que cuando en el futuro descarguemos un movimiento de este tipo sepa identificarlo y aplicarle el tipo que hemos seleccionado. Imaginemos que tenemos este registro bancario:

&#x20;

![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image008.jpg)

●        Supongamos que es la primera vez que hemos descargado este tipo de movimiento que en realidad es de “Gastos bancarios”. Pulsamos el botón de modificar el tipo y seleccionamos después en la lista “Gastos bancarios”

○        ![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image010.jpg)

●        El programa nos pedirá confirmación para  este cambio y a continuación presentará esta ventana:

![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image012.jpg)

&#x20;

●        En esta se presenta palabra a palabra el contenido de la descripción del movimiento excluyendo las cadenas numéricas.

●        Se trata de seleccionar aquellas palabras que consideremos que en el futuro servirán para identificar el tipo de movimiento “Gastos bancarios” en cualquier registro que descarguemos de cualquier banco.

●        Podemos seleccionar una o varias palabras pero si son más de una la selección debe ser correlativa.

![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image014.jpg)

&#x20;

●        Hemos seleccionado en el ejemplo toda la cadena “LIQUIDACION DEL CONTRATO”. Esta selección se guarda en el tipo de movimiento y a partir de este momento siempre que el programa lea en un movimiento de gastos esta cadena identificará el movimiento como “Gastos bancarios”.

●        Es importante tener en cuenta que esta localización es para gastos. Es decir, si entrara un registro de ingresos con esa misma cadena el programa nunca lo aplicará a “Gastos bancarios”.

&#x20;

●        ![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image016.jpg) Ampliación de datos de lectura: es sólo un formulario de consulta y nos presenta en detalle todos los datos que hemos descargado del banco tanto en la descarga intradía como en la de la Norma 43.

●        &#x20;

![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image018.jpg)

●        El primer código que vemos se corresponde con el que da el proveedor del servicio de descarga intradía : 18 - pago de recibos

●        Dentro de la Norma 43 vemos:

○        El “concepto común” según el Consejo superior bancario: 03 - Adeudos - Recibos - Letras - Pagos por su cuenta.

○        El “concepto propio” que asigna la entidad, en este caso el BBVA a este tipo de movimiento: 136 - Adeudo a su cargo.

○        La referencia y el concepto son datos de extensión que obtenemos también en la descarga de la norma 43.

●        Es por esto que es importante para el caso de registros no reconocidos en la descarga intradía esperar a la descarga de la Norma 43 ya que ésta siempre aporta más información.

&#x20;

●        El siguiente botón que encontramos en el formulario del registro es para la “Gestión de la entidad”.

&#x20;

![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image020.jpg)

●        Pulsando en el lápiz accedemos a un formulario especial para editar, eliminar y/o modificar la entidad:

![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image022.jpg)

&#x20;

●        En el formulario vemos el código y el nombre fiscal y comercial de la entidad en caso de tenerlo.

●        Debajo vemos los tipos de entidad que tiene definidos.

●        ![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image024.jpg)El primer botón simplemente edita la ficha de la entidad.

●        ![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image026.jpg)Con este quitamos la entidad del registro

●        ![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image028.jpg) El botón localizar aparecerá cuando no haya entidad definida. Es muy importante tener en cuenta que si en un registro que no había entidad la aplicamos con el localizador y aceptamos, el sistema lanzará automáticamente una búsqueda de documentos que puedan cuadrar con el registro y la entidad localizada y en caso de localizarlo lo asigna automáticamente.

![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image030.jpg) Este es el “Asistente para guardar alias de localización”.

Lo explicamos: de la misma manera que podemos guardar una regla de localización  para un tipo de movimiento las podemos guardar también para las entidades. Imaginemos que en un registro tenemos esta descripción:

&#x20;

“2024064001308335-ADEUDO-POR-DOMICILIACI-SUCARG-ES15000A36494706-ES40000B90102195-187451-COREVELNEO-04MA-67740-”

&#x20;

Tenemos claro que la entidad en este caso es “Velneo” pero lógicamente en su ficha aparece como tal y no como “COREVELNEO”.&#x20;

&#x20;

Primero asignaremos al registro la entidad “Velneo” utilizando el localizador de entidades.

&#x20;

A continuación pulsando el botón del asistente nos aparecerá como en el caso de los tipos de movimientos, una lista de palabras contenidas en la descripción del registro para que seleccionemos aquella o aquellas con las que queremos que en el futuro se pueda identificar a la entidad que hemos seleccionado:

&#x20;

&#x20;               ![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image032.jpg)

&#x20;

●        Al seleccionar la palabra “COREVELNEO” y aceptar, el integrador la guardará en la ficha de la entidad como “Alias” de Velneo y en el futuro siempre que en un registro aparezca esta palabra el sistema lo asociará a la entidad Velneo.

●        Podemos consultar esta información en la ficha de la entidad en la pestaña “Integrador” donde aparecen los “Alias”  que se le han aplicado.

●        A diferencia del caso de los tipos de movimientos la utilización del alias en las entidades no se hace por cadenas sino por palabras. Es decir si para el ejemplo de la entidad Velneo en su lista de alias aparece: “COREVELNEO-VELNEOSOFT” el programa no asociará en el futuro esa entidad a un registro que contenga esa cadena completa sino a cualquiera que contenga la palabra “COREVELNEO” o “VELNEOSOFT”.

●        En el campo “Alias” de la entidad se quedan siempre las palabras guardadas separadas por guiones.

&#x20;

●        La siguiente zona que encontramos en el formulario es la relativa  al documento:

&#x20;

![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image034.jpg)

&#x20;

●        Además de los datos relativos a la factura en este caso, vemos un botón para editarla y otro para borrar la relación: es decir “quitaríamos” esa factura de este registro para localizar después la correcta.

●        La localización de un nuevo documento se hace siempre desde el botón de la rejilla específico para esto que se explica más adelante.

&#x20;

●        Gastos bancarios

○        El programa contempla para todos los registros de pago que pueda haber una cantidad aplicable a gastos bancarios, tanto para traspasos como para pagos a proveedores o empleados.l

○        Si se trata de un pago a proveedor o a empleado se imputará por defecto la diferencia entre el documento a pagar o el salario del empleado a esta partida. En cualquier caso el usuario puede modificarla.

○        Al cerrar un registro que tenga un importe definido en gastos bancarios si son pagos de factura o a empleados tomarán siempre la cuenta contable de gastos que esté definida en la cuenta bancaria. En el resto de casos, si hay cuenta definida en el tipo de movimiento tomará esta cuenta y si no la hay tomará la de la cuenta bancaria.

●        A compensar

○        Otro caso que se puede dar que provoque diferencias en un cobro o pago pueden ser los “importes a compensar”. Éstos se contemplan en los cobros y pagos de cartera y son la posible diferencia que puede haber entre lo que hay pendiente de cobro o pago en una factura y lo que se cobra o paga en el movimiento bancario.

○        Según la compensación sea sobre un cobro o un pago se utilizarán las cuentas contables definidas en parámetros - administración - contables - general: “Compensación en cobros / pagos”.

●        ![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image036.jpg) Cerrar el registro ![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image038.jpg)

○        Este botón sólo aparecerá si el registro ha llegado a estado confirmado y no está activado en este tipo de movimiento el cierre automático.

○        El sistema pedirá confirmación y tal como se explica en el punto 3 del bloque de teoría generará un asiento contable, uno de tesorería o ambos.

○        El registro pasará a estado “Cerrado” y presentará un candado en la última columna del listado. Si hacemos doble click nos mostrará el asiento de tesorería generado, el asiento contable o ambos.

●        ![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image040.jpg) Opciones especiales: según el estado y el tipo del registro nos aparecerán las siguientes opciones:

○        Registros abiertos

■        Crear cobro/pago manual

●        Para movimientos relativos a cobros / pagos de documentos (también a devoluciones) aparecerá esta opción para cobrar o pagar según sea el tipo de movimiento.

●        Seleccionando esta opción el programa ignora si hay o no entidad y/o documento localizado y lo que hace es crear un asiento de tesorería aplicando la fecha, la cuenta bancaria y el importe del registro.

●        Al terminar el proceso marcará el registro como cerrado.

■        Crear asiento manual

●        Esta opción aparece para cualquier tipo de movimiento

●        Pulsando este botón se genera un asiento contable en la fecha del registro bancario incluyendo un primer apunte con la cuenta contable relativa a la cuenta bancaria y el importe del asiento.

●        Al terminar el proceso marcará el registro como cerrado.

■        Cierre neutro

●        Esta opción no hace nada más que marcar el registro actual como cerrado sin generar ni modificar ningún dato en todo el programa.

○        Registros cerrados

■        Reaperturar

●        Este botón deshace completamente la operación de cierre que hubiera ejecutado eliminando el registro de tesorería generado, el asiento contable o ambos.

●        Al ejecutar la opción el registro vuelve al estado “Confirmado”.
