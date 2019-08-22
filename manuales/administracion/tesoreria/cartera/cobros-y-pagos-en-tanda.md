# Cobros y Pagos en Tanda

Con objeto de agilizar la gestión de cobros y pagos tenemos la opción de hacerlos “en tanda”, es decir, desde una lista de cobros o pagos de una misma entidad. Además la aplicación contempla la posibilidad de que el cobro o el pago no coincidan exactamente con las facturas a cobrar o pagar y el usuario decida en ese caso si contabiliza la diferencia como “compensación” o la lleva a anticipo de cliente o proveedor.

Esta operativa comienza por definir en parámetros las cuentas contables para la compensación:

* Parámetros – Administración - contables

![](../../../../.gitbook/assets/image%20%28254%29.png)

Una vez definidos estos parámetros la operativa es igual para cobros y pagos. Vamos a detallar a continuación cómo se utiliza esta opción desde la cartera de cobros, entendiéndose que es idéntica la operativa para la cartera de pagos.

![](../../../../.gitbook/assets/image%20%2893%29.png)

Para cobrar varios efectos se sigue el siguiente procedimiento:

·         Desde una lista de derechos de cobros \(se puede hacer en el propio panel o en el listado de cobros\), utilizando el selector de la izquierda marcaremos los registros que queremos cobrar.

o    Los registros deben cumplir estas premisas:

* Deben ser del mismo cliente
* Deben estar en situación “En cartera”

·         Una vez estando seleccionados los registros pulsamos abajo en el botón “Cobrar “ y aparecerá el siguiente formulario

![](../../../../.gitbook/assets/image%20%28153%29.png)

La aplicación nos propone como importe a cobrar la suma de los importes pendientes de todos los registros seleccionados. Para darlos por cobrados basta con especificar la cuenta de cobro. En el campo concepto aparecerá el que esté parametrizado por defecto como concepto de cobro de facturas.

Al aceptar el formulario se creará un registro de tesorería por el importe total cobrado contra la cuenta especificada y la fecha de cobro.

En caso de que el importe cobrado no sea exactamente la suma de los importes pendientes tendremos que modificar el “importe recibido” y el formulario cambiará de la siguiente forma:

![](../../../../.gitbook/assets/image%20%28138%29.png)

En el caso visualizado hemos cobrado un exceso de 10€. Las posibles aplicaciones de las diferencias de cobros son las siguientes:

·         Cobros en exceso

o    Si tenemos marcado el check “compensar diferencias” el recibo se dará como cobrado por su importe y en el efecto de tesorería que se cree se compensará este recibo y se creará un ingreso por “regularización” de 10€ que al contabilizará irá a la cuenta definida en parámetros como “compensación de cobros positivos”.

o    Si desmarcamos el check el ingreso de más se guardará en el asiento de tesorería como “anticipo de cliente” y quedará en su cuenta pendiente de compensar.

·         Cobros insuficientes

o    Con el check marcado “compensar diferencias” se dará por cobrado el recibo y se generará el asiento de tesorería llevando la diferencia a “regularización” que se contabilizará en la cuenta definida para “compensación de cobros negativos”. Esta diferencia lógicamente aparecerá en el asiento de tesorería en negativo de manera que el importe total del asiento coincida con la cantidad cobrada real.

o    Con el check desmarcado no se dará por cobrado el recibo, quedando la diferencia como pendiente de cobro.

Toda esta operativa de compensación es igual al cobrar un solo efecto con el botón que hay dentro del formulario.

Es importante recordar que la operativa en pagos es idéntica a la explicada anteriormente para cobros.

