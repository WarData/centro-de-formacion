# Gestión de Precios y Tarifas de Ventas

La gestión de precios en Winmotor está pensada de manera que el usuario final que graba documentos no tenga que tomar ninguna decisión en cuanto al cálculo del precio de compras ni de ventas de los productos.

![](../../../.gitbook/assets/image%20%2883%29.png)

Para el cálculo del precio de compras se utiliza la tarifa de compras en base a la cual se define el proveedor preferente del artículo y su precio de compra final \(precio de tarifa menos descuentos\). Dado que para un mismo artículo podemos definir varios proveedores el programa exige que uno de ellos sea el “preferente”, es decir, el que se va a tomar por defecto cuando se genere un pedido de compras. La primera tarifa de compras grabada para un artículo queda asignada automáticamente como preferente, una vez que se definen más tarifas se puede asignar la preferente a la que el usuario quiera.

El programa se puede parametrizar para que cuando en un albarán de compras cambie el precio de un producto se haga lo siguiente en la tarifa de compras del artículo:

·         Actualizar la tarifa automáticamente

·         Preguntar al usuario: esto presentará el formulario de tarifa de compras del artículo con los nuevos precios calculados dando opción a que el usuario decida si es una modificación definitiva sobre el artículo o no.

·         No hacer nada: el precio de compras de los artículos nunca se cambiará desde el albarán de compras, habrá que entrar manualmente en la ficha para modificarlo.

Para una gestión automatizada de los precios de ventas se aconseja no definir manualmente ningún precio de venta sino establecer una regla para su cálculo de manera que cuando cambie el precio de compra se modificará automáticamente el precio de venta del producto.

![](../../../.gitbook/assets/image%20%2877%29.png)

Estas reglas se pueden definir en su opción correspondiente en el menú de submaestros “Fórmulas PVP” o manualmente desde una ficha de familia o de artículo. Si definimos en una familia una “fórmula para el cálculo del pvp” ésta se aplicará automáticamente a los artículos a los que se asigne dicha familia.

Para la edición de fórmulas de cálculo de pvp el programa presenta un asistente donde se podrá operar con los datos del artículo. Lo más lógico será siempre establecer una fórmula que parta del precio de tarifa de compras o del precio neto de compras del artículo y sobre éste aplicar un incremento. Dado que el asistente es algo complejo se recomienda solicitar ayuda a Winmotor la primera vez que se vaya a utilizar.

Una vez establecido para un artículo su precio de compras y de ventas entramos en la gestión de “condiciones de ventas” que explicamos a continuación.

En Winmotor gestionamos los precios de venta de los artículos de manera que son ilimitados, un mismo artículo podrá tener múltiples precios de venta según a quién se vende y que se encuentre o no en oferta.

![](../../../.gitbook/assets/image%20%2840%29.png)

Para la gestión de precios utilizamos las líneas de condiciones que se aplican luego en distintas fichas que veremos más abajo. Las líneas de condiciones se pueden definir según uno de estos criterios:

·         Tipo de producto

·         Marca

·         Familia

·         Artículo

En una línea de condición sólo se puede utilizar uno de estos criterios, es decir, sólo podremos rellenar un campo excepto para el caso de familia y marca que si se pueden usar combinadas y prevalecerán sobre una condición definida para la familia o la marca como se explica más abajo.

El programa utiliza la gestión de condiciones en el cálculo del precio de un artículo en una línea de presupuesto de ventas, pedido, albarán o factura.

Podemos definir una condición definiendo descuentos \(Descuento 1, Descuento 2\) o incrementos sobre el costo del producto. Sólo en el caso de definir una línea de condición sobre un artículo concreto podemos aplicar un precio directo. Este sistema es el menos aconsejable ya que si se cambia de precio de venta el artículo no lo van a hacer de forma automática las tarifas directas que tenga definidas, las tendrá que modificar el usuario manualmente.

Las líneas de tarifas se pueden definir en distintas opciones del programa que son:

**Tarifas**

![](../../../.gitbook/assets/image%20%2853%29.png)

Las tarifas definen una serie de condiciones de venta \(líneas de tarifas\) que se aplicarán sobre los clientes que tengan aplicada en su ficha dicha tarifa. La asignación de tarifa a un cliente se puede hacer de dos formas:

·         Tarifa directa: rellenando el campo tarifa en la ficha del cliente

·         Tarifa por tipo de producto: pulsando el botón correspondiente que aparece en la pestaña “comerciales” de la ficha del cliente podremos asignar a un mismo cliente una tarifa por cada tipo de producto.

También se puede definir una tarifa para una o varias “clases” de clientes. La clase es un clasificador de clientes que si se deja vinculado a una tarifa provocará que al aplicar una clase a un cliente se asigne por defecto la tarifa de la clase.

La opción para acceder al menú de tarifas la encontramos en el menú de “maestros” que incluye además un sistema de consulta rápida de manera que al pinchar en la lista de tarifas que nos aparece en la izquierda veremos en el centro todas sus líneas.

Existe por otro lado la posibilidad de definir una “Tarifa de exclusividad”, es decir, podemos definir para un cliente determinado que sólo se le puedan vender los artículos afectados por una tarifa concreta. Para esto hay que entrar en la pestaña “Comerciales” de la ficha del cliente y marcar el check “Tarifa de exclusividad” que aparece junto al campo tarifa.

**Condiciones especiales de clientes**

![](../../../.gitbook/assets/image%20%2872%29.png)

Un mismo cliente además de estar acogido o no a una tarifa puede tener “condiciones especiales”. Es decir, serán condiciones aplicables exclusivamente a ese cliente. Esto hace por lo tanto innecesario y sin sentido definir tarifas para un solo cliente, se puede utilizar esta opción.

Las condiciones especiales de un cliente prevalecerán sobre su tarifa, por lo tanto, si un cliente está acogido a una tarifa donde la marca “X” tiene un descuento del 20% pero le definimos en su ficha una condición especial para la misma marca, ésta prevalecerá sobre la tarifa.

**Ofertas**

![](../../../.gitbook/assets/image%20%28260%29.png)

Una oferta es un documento especial con una fecha de caducidad. La oferta se define con el mismo formulario de líneas de tarifas que utilizamos en los documentos anteriores pero la oferta prevalece sobre cualquier condición definida para un producto o grupo de productos. Es decir, si en una tarifa hemos definido un descuento para una familia “X” y utilizamos esa misma familia en una oferta, las condiciones aquí definidas prevalecerán sobre la tarifa o las condiciones especiales de un cliente. Como excepción a esta norma hay que tener en cuenta que si un cliente tiene marcado en su ficha que su tarifa es “de exclusividad” no se tendrán en cuenta para él las condiciones definidas en ofertas.

El sistema “desactivará“ automáticamente una oferta llegada su fecha de caducidad, con lo que dejará de afectar a los precios de un artículo, pero la ficha de la oferta permanecerá en la aplicación de manera que se podrá consultar.

En el menú de Ventas tenemos el acceso al de ofertas, pero también se puede crear de forma asistida desde el listado de artículos obsoletos en el menú de “rotación y consumos” dentro del menú de artículos.

Criterios para el cálculo de precios en un documento de ventas

Como hemos visto un artículo concreto que vamos a vender puede estar afectado por múltiples condiciones definidas en los documentos mencionados \(tarifas, condiciones especiales de clientes u ofertas\).  Hemos explicado ya la prioridad de estos documentos en el cálculo del precio de un artículo, el programa busca dichos documentos en este orden

1.       Oferta

2.       Condición especial de cliente

3.       Tarifas

En cualquiera de estos documentos un mismo artículo puede estar afectado por más de una condición, es decir, puede haber más de una línea en el documento que apunte a un artículo concreto. Imaginemos que en una tarifa hemos definido una línea con descuento para la marca “X” y en la misma tarifa un descuento específico para la familia “F”. Puede darse por lo tanto el caso de que artículos de esa familia además sean de la marca “X”: ¿Cómo actúa el programa en este caso?

El criterio de la aplicación para aplicar la tarifa es el inverso al orden en el que se presentan los datos en las líneas de tarifas, es decir:

·         Artículo

·         Familia y marca

·         Familia

·         Marca

·         Tipo de producto

O sea, una condición definida específicamente para un artículo prevalecerá sobre una condición para una familia y marca, una por familia prevalecerá sobre una condición de marca y en último lugar se evaluará la condición del tipo de producto.

**Artículos dependientes**

Si en su aplicación ha configurado para alguno de los tipos de artículos que se admitan artículos dependientes el programa también contará con sus relaciones para el cálculo de precios.

El programa calcula para los artículos dependientes y sus “artículos padres” la genealogía, es decir, el programa internamente calcula si un artículo es “Abuelo” \(no tiene artículo padre y tiene artículos dependientes\), “Padre” \(tiene artículo padre y artículos dependientes\) o “Nieto” \(tiene artículo padre y no tiene artículos dependientes\). Si incluimos uno de estos artículos en una condición de ventas en el momento de la venta tendrá preferencia el nieto, luego el padre y luego el abuelo.

Imaginemos que hemos definido para un artículo sus artículos dependientes que serían por ejemplo las distintas tallas: si para cada una de esas tallas definimos artículos dependientes por colores ya tenemos el abuelo \(artículo inicial\), los padres \(tallas\) y los nietos \(colores\). Si en una condición de ventas queremos establecer por ejemplo un descuento para todos estos artículos basta con que lo hagamos para el artículo raíz y el programa se la aplicará a todos sus hijos y nietos. Si quisiéramos que un color concreto tenga una distinta condición de ventas y lo incluimos en el mismo documento \(una tarifa por ejemplo\), el precio de éste prevalecerá sobre el definido para toda la gama del artículo.

**Consultas de condiciones de ventas**

![](../../../.gitbook/assets/image%20%28289%29.png)

Para facilitar la consulta de los posibles precios de un artículo contamos con una utilidad en el formulario del artículo: la consulta de precios. Al pulsar ese botón el programa calculará según todas las condiciones de ventas que pueden afectar al artículo su precio final y las presentará en el orden en el que hemos indicado que se calculan en los documentos.

