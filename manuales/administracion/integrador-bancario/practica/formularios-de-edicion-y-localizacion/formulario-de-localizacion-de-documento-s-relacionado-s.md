# Formulario de localización de documento/s relacionado/s

Para los siguientes tipos de movimientos el integrador necesita localizar el o los documentos relacionados con el mismo:&#x20;

■        Devolución a cliente

■        Pago a proveedor / acreedor

■        Cobro a cliente

■        Devolución a proveedor



○        Siempre que en un registro de este tipo no esté identificado el documento relacionado aparecerá en la columna anterior este icono:

<figure><img src="../../../../../.gitbook/assets/imagen (11) (6).png" alt=""><figcaption></figcaption></figure>

Al pulsarlo entramos en el formulario de localización de documentos y registros de cartera:

<figure><img src="../../../../../.gitbook/assets/imagen (13) (5).png" alt=""><figcaption></figcaption></figure>

●        En la parte superior vemos a nivel de consulta los datos que ya están identificados en el registro (entidad, fechas, importe, descripción).

●        Dentro de la pestaña “Seleccionar-buscar” es donde el usuario tendrá que filtrar para localizar el documento relativo al registro.

○        Importe desde: por defecto el programa presenta diez euros menos del importe del registro para contemplar el caso de que hubiera pequeñas diferencias de importe entre el documento y el pago / cobro.

○        Importe hasta: por defecto el programa presenta diez euros más del importe del registro.

○        Fecha desde: por defecto se busca desde un mes antes de la fecha del registro.

○        Fecha hasta: por defecto se busca hasta un mes después de la fecha del registro.

●        Hay que recordar aquí que el programa sólo busca documentos pendientes de pago y que no estén ya relacionados con un registro bancario.

●        Es muy importante tener en cuenta que al entrar en este formulario el programa ya ha ejecutado la búsqueda con estos parámetros y si hubiera encontrado algo lo estaría presentando debajo: si le damos a la lupa sin cambiar nada no aparecerá ningún documento. Por lo tanto, al llegar a este punto si el documento o registro de cartera relativo a este movimiento bancario no aparece puede ser por:

○        El documento que estamos buscando está fuera de estos filtros y por lo tanto hay que ampliarlos en fechas o en importe.

○        No se trata de un documento sino de varios. Si pensamos que puede ser este el caso hay que disminuir el filtro “Importe desde” puesto que estaremos buscando más de un registro de menor importe.

●        Utilizando el ejemplo anterior hemos abierto los filtros de importes y fechas y vemos esto:&#x20;

<figure><img src="../../../../../.gitbook/assets/imagen (14) (8).png" alt=""><figcaption></figcaption></figure>

●        El sistema ha localizado ahora un compromiso de pago de Vodafone que cumplen los criterios del filtro.

●        ![](<../../../../../.gitbook/assets/imagen (15).png>) Con el botón de comprobación de los importes seleccionados vamos a ver si la suma de los dos primeros se ajustan al importe del registro.&#x20;

●        Una vez confirmamos que la suma de esos dos registros “casi” cuadran con el importe del registro confirmamos la selección con el botón de la derecha:

&#x20;![](<../../../../../.gitbook/assets/imagen (16).png>)

&#x20;&#x20;

<figure><img src="../../../../../.gitbook/assets/imagen (18).png" alt=""><figcaption></figcaption></figure>

●        Al confirmar, el sistema detecta la diferencia de importes y nos presenta el siguiente cuadro de diálogo:

<figure><img src="../../../../../.gitbook/assets/imagen (19).png" alt=""><figcaption></figcaption></figure>

●        Según marquemos que la diferencia es aplicable a gastos bancarios o a compensación el programa utilizar para generar el asiento de tesorería uno u otro concepto y en consecuencia su correspondiente cuenta contable:

○        Gastos bancarios: toma la cuenta contable de gastos definida en la cuenta bancaria.

○        Compensación: la compensación es un sistema general del programa utilizado en el cobro y pago de efectos: implica que por la razón que sea hemos pagado o cobrado una factura con alguna pequeña diferencia pero queremos dar el documento por pagado o cobrado. La cuenta contable correspondiente (según estemos cobrando o pagando) se toma de parámetros - administración - Contables - General: Compensación en cobros / pagos.

●        El procedimiento para la aplicación de un documento es exactamente el mismo que acabamos de explicar.

●        ![](<../../../../../.gitbook/assets/imagen (20).png>) En última instancia, si por cualquier razón no conseguimos localizar el documento relativo a un registro tenemos la opción de la “Selección directa”. Pulsando este botón nos aparece un localizador donde podremos seleccionar cualquier documento de la base de datos por su código y quedará vinculado al registro bancario sin ningún tipo de control.
