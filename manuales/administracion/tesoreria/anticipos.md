# Anticipos

Winmotor incorpora para la gestión administrativa de clientes un control sobre los anticipos recibidos. En resumen consiste en relacionar en el momento que se genera una factura a un cliente que nos ha entregado un anticipo la factura generada con el anticipo recibido previamente y controlarlo además en la contabilización.

* Datos base

![](../../../.gitbook/assets/image%20%28281%29.png)

* * Crear concepto "Anticipo de clientes"
    * En la tabla de conceptos de tesorería hay que crear un nuevo concepto para aplicarlo en los anticipos. Es prioritario que tenga marcado el nuevo check "anticipo", que sea del tipo “cobro” y que no esté marcado "Pedir factura".

![](../../../.gitbook/assets/image%20%2899%29.png)

* * Marcar en parámetros la cuenta contable general para anticipos de clientes : Parámetros - administración - contables - Cuenta anticipo de clientes
    * Paralelamente en contabilidad hay que marcar la cuenta aquí definida como cuenta de "Clientes"

![](../../../.gitbook/assets/image%20%28250%29.png)

* * Marcar en parámetros el código del concepto creado para anticipos y definir si queremos que la aplicación en caso de anticipos no asignados a pedidos aplique automáticamente a las facturas generadas los anticipos pendientes de liquidar de clientes. En caso de no estar marcado este check y para este caso habrá que hacer la casación con los anticipos manualmente. Más abajo se explica en detalle los posibles funcionamientos
* Funcionamiento
  * En el momento de recibir un anticipo de cliente se graba un asiento de tesorería especificando el cliente y lógicamente el importe del anticipo.
  * Opcionalmente se podrá asignar el anticipo a un pedido concreto, de manera que sólo cuando se generen facturas relativas a este pedido el programa lo aplicará a dichas facturas. La creación del registro de anticipo se puede hacer manualmente desde el alta de un asiento de tesorería o de forma automatizada desde el formulario de pedidos de clientes mediante el botón que aparece a este efecto cuando el pedido queda confirmado. Dejar definido en parámetros el código del concepto de anticipo tiene la finalidad de que en este punto el sistema pueda dejarlo ya aplicado en el asiento en el momento de grabarlo desde el pedido.

![](../../../.gitbook/assets/image%20%28358%29.png)

* * Cuando este anticipo quede aplicado a alguna factura ésta aparecerá en la rejilla indicando el importe aplicado. En el caso de por alguna razón quisiéramos “desaplicar” un abono basta con eliminar la línea correspondiente en la rejilla.
  * Al contabilizar la tesorería se genera un asiento de la siguiente forma : 
    * Debe : cuenta contable relativa a la cuenta de tesorería
    * Haber : cuenta contable de anticipos y auxiliar del cliente
  * Al generar una factura contra un cliente que tenga anticipos pendientes de compensar pueden pasar tres cosas:
    * El anticipo está relacionado con un pedido. Si la factura contiene alguna línea relativa a ese pedido hará la compensación correspondiente.
    * El anticipo no está relacionado a un pedido y el check “Aplicación automática de anticipos” está marcado: el programa aplicará el importe del anticipo sobre la factura generada.
    * El anticipo no está relacionado a un pedido y el check “Aplicación automática de anticipos” está desmarcado: el programa no hará nada, la aplicación de anticipos se hará manualmente desde el botón a este efecto que aparece en la factura.
      * Es fundamental tener en cuenta que el sistema no le permitirá aplicar anticipos aunque el cliente los tenga pendientes de compensar en caso de que la factura haya generado registros de cartera y que éstos sean giros remesados. Si se da este caso el programa le avisará con un mensaje impidiendo continuar el proceso.
      * Por otro lado hay que tener en cuenta que en el caso de que la factura tenga registros de cartera generados y apliquemos manualmente un anticipo la cartera se recalculará sobre el importe pendiente de cobro de la factura.

![](../../../.gitbook/assets/image%20%28269%29.png)

* * El programa contempla el caso de que un anticipo se pudiera aplicar a una o varias facturas puesto que pudiera ser que después de obtenido un anticipo de un cliente se le generara una factura por importe inferior al anticipado. Así mismo también está contemplado el caso contrario en el que a una misma factura se podría aplicar más de un anticipo.
  * Al contabilizar la factura de ventas la aplicación generará además de los apuntes correspondientes a la factura \( total al cliente, bases a los conceptos e impuestos\) dos líneas de compensación del anticipo de la siguiente forma:
    * Debe : cuenta contable de anticipos y auxiliar del cliente
    * Haber : cuenta contable del cliente y auxiliar del cliente
  * Al abonar una factura que tenga aplicado un anticipo la aplicación generará automáticamente una “descompensación” del anticipo en el mismo asiento general del anticipo aplicando en negativo el importe que corresponda. Este importe lo calculará la aplicación en función del total de la factura abonada y del total del anticipo según el criterio general de aplicación de anticipos a facturas.
  * En el caso de tener que devolver un anticipo a un cliente el procedimiento consiste en situarse en el apunte de tesorería donde se creó el anticipo y pulsar el botón “Retroceder” que aparece abajo.
    * El programa pedirá confirmación de la fecha y la cuenta. Por defecto la fecha será la de hoy y la cuenta la misma desde la que se creó el anticipo.
    * Al confirmar el formulario  se creará un asiento de retrocesión en la fecha y cuenta indicada.
  * Al consultar la ficha de un cliente que tenga anticipos pendientes de compensar en la pestaña "riesgo" dentro de los datos administrativos aparecerá reflejado los  anticipos pendientes a su favor. Es importante tener en cuenta que en la pestaña “riesgo” en clientes sólo se ven datos si hay algún valor que implique riesgo.

![](../../../.gitbook/assets/image%20%28123%29.png)



