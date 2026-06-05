# Contabilización de facturas internas

Hasta ahora las facturas internas en Winmotor no se contabilizaban: era un documento que quedaba en gestión y afectaba por lo tanto a las estadísticas y al stock. A partir de ahora se podrán contabilizar las facturas internas utilizando cuentas del grupo “0” (con una excepción que explicaremos más adelante). Además, sólo se podían hacer facturas internas desde órdenes de reparación, ahora también se pueden hacer albaranes internos y facturarlos.

\
<mark style="color:$primary;">**Configuración**</mark>

* **Activación**
  * Activar el parámetro general “Contabilizar facturas internas” en parámetros - Administración - Contables - General:
  *

      <figure><img src="../../.gitbook/assets/image (726).png" alt=""><figcaption></figcaption></figure>
  * Marcar el campo “Contabilizar” en  las series de facturas que queramos que se contabilicen (lógicamente series de facturas internas)
  *

      <img src="../../.gitbook/assets/unknown (7).png" alt="" height="129" width="402">
  * Las series de órdenes para contabilizar también deben tener marcado el departamento “Taller” en la pestaña de parámetros&#x20;
  *

      <img src="../../.gitbook/assets/unknown (8).png" alt="" height="75" width="1021">
  * Las series de albaranes deben tener marcado el tipo “interno”. Se recomienda también para este tipo de albaranes activar el check “Permite aplicar vehículos” de la pestaña de parámetros. Esto provocará que al grabar el albarán se pida también el campo vehículo y por lo tanto se aplique el coste de ese albarán a la estadística del mismo.
* **Contabilización**
  * El núcleo de este nuevo sistema de contabilización está en los “tipos de órdenes”; hemos creado nuevos campos para gestionar todas las posibles estructuras de asientos. También se ha creado una nueva cuenta contable para los tipos de producto y para los servicios y temparios. Lo explicamos en detalle:
    * Tipos de órdenes&#x20;
      * Se han definido estos tipos dentro de las órdenes internas:
        * Preentrega VN
        *

            <img src="../../.gitbook/assets/unknown (9).png" alt="" height="247" width="964">
        * Preentrega VO
        *

            <img src="../../.gitbook/assets/unknown (10).png" alt="" height="247" width="959">
        * Gastos internos (reparaciones internas, consumos internos, etc)
        *

            <img src="../../.gitbook/assets/unknown (11).png" alt="" height="246" width="959">
        * Reacondicionamiento (normalmente reparación de un VO para su venta)
        *

            <img src="../../.gitbook/assets/unknown (12).png" alt="" height="251" width="961">
        * Regalos
        *

            <img src="../../.gitbook/assets/unknown (13).png" alt="" height="245" width="965">
      * Cada uno de estos tipos contempla nuevos campos para su contabilización. El primero y principal es el tipo de orden interna, que puede ser&#x20;
        * Gasto
          * Según el tipo de orden se generará el asiento contable con una estructura distinta según las cuentas que se hayan definido en la parametrización: se puede definir una cuenta a la que aplicar el total de la orden o cuentas separadas para la totalización de los materiales y la mano de obra.
        * Existencias
          * El total de la orden se imputará como incremento de las existencias relativas al vehículo reparado (podrá ser VN o VO) y su cuenta se tomará de la definida para el tipo de producto (Vehículo o Vehículo de ocasión). Dado que se utiliza la cuenta “fiscal” de existencias para este asiento se utilizarán también para las partidas de ingreso, en lugar de cuentas analíticas las cuentas fiscales de ventas (grupo 700).
      * Estas cuentas afectan a la totalización de la orden, el detalle (los recambios aplicados y la mano de obra) tomarán la cuenta contable de su correspondiente ficha de tipo de producto o del tempario. En caso de aplicar servicios la cuenta se leerá del servicio.
  * Temparios
    * Se ha creado una nueva cuenta contable para la contabilización de facturas internas:
      *

          <img src="../../.gitbook/assets/unknown (14).png" alt="" height="662" width="1087">
      * Tipos de producto&#x20;
        *

            <img src="../../.gitbook/assets/unknown (15).png" alt="" height="516" width="997">
      * Servicios
        *

            <img src="../../.gitbook/assets/unknown (16).png" alt="" height="311" width="813">
* Como se puede ver la parametrización de estas cuentas está montada en el formulario de cada una de las fichas a las que afectan (tipos de orden, tipos de producto, temparios y servicios); para facilitar la edición y la consulta de todas se ellas hemos añadido una nueva pestaña en parámetros donde las podemos ver en conjunto:
  *

      <img src="../../.gitbook/assets/unknown (17).png" alt="" height="527" width="1880">
  * Tipos de albaranes
    * Los tipos de albaranes sólo se pueden configurar en esta pestaña de parametrización de las facturas internas. Su tratamiento es casi idéntico al de los tipos de órdenes con la excepción de que no se contemplan albaranes internos del tipo “Existencias”, serán siempre tipo “Gastos”.

<mark style="color:$primary;">**Funcionamiento**</mark>

Una vez se han configurado todas las tablas y parámetros anteriormente descritos la operativa es bastante sencilla: simplemente hay que pasar por el enlace contable las facturas internas que a su vez se han generado desde las órdenes internas en las que se ha definido para cada una el tipo de orden.

Sólo en el caso de los albaranes internos hay un tratamiento especial ya que al grabar uno aparecerán en la cabecera los dos campos necesarios (y exigibles) para grabar el albarán.

<br>
