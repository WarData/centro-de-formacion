---
description: Campos Especiales en las Fichas de Servicios
---

# Servicios

![](<../../.gitbook/assets/image (519).png>)

Dentro de la ficha de un servicio encontramos una serie de “checks” que tienen una utilidad específica dentro del programa. Pasamos a detallarlos:

**o Pestaña Observaciones:**

* **Aplicable a vehículos**

&#x20;        o Al utilizar un servicio con este check marcado en un documento de ventas o de compras el programa pedirá los bastidores afectados.

&#x20;        o Para todos los bastidores que se incluyan se les repercutirá en su estadística el importe correspondiente como gasto o ingreso según el tipo de documento donde se esté aplicando.

* **Abono de garantías**

&#x20;        o Las garantías de reparaciones se pueden facturar en el programa de dos formas según lo que establezca el fabricante (este dato se define en la ficha de la marca) :

&#x20;              1.- Por factura de ventas

&#x20;              2.- Por abono de compras

&#x20;        o Para el caso de factura de ventas el sistema de facturación de las garantías es como cualquier otra facturación, simplemente el programa al saber que estamos facturando una garantía emitirá la factura contra el fabricante en lugar de hacerlo contra el cliente de la orden.

&#x20;        o Para el caso de que la marca lo que haga sea emitir una factura de abono tendremos que utilizar un servicio con este check marcado para la grabación de dicha factura de abono de garantía.

&#x20;              1.- Al utilizar este tipo de servicio en una factura de compras o de gastos el programa presentará un localizador de órdenes de reparación para que indiquemos qué orden es la que se está abonando.

&#x20;              2.- Al definir la orden esta quedará como facturada en su partida de garantía.

* **Tramitación de vehículos**

&#x20;         o Habilita la capacidad del servicio de tramitar traspasos cuando se activa junto a "Transferencia" y "Aplicable a vehículos"

* **Transferencia**

&#x20;         o Implica que el servicio se utilizará en una tramitación de una transferencia. La tramitación de una transferencia le indica el programa el cambio de propietario de un vehículo, con lo que al utilizar este tipo de servicio el vehículo pasará a aparecer en el programa en la ficha del “comprador”.

* **Bonificación**

&#x20;         o Obsoleto – no tiene utilidad

* **Acumular coste en ventas**

&#x20;         o El check marcado implica que al imputar líneas de ingresos con este servicio al vehículo el coste de la línea no se le repercutirá puesto que vendrá luego reflejado en una factura de gastos. Solamente aplicable en caso de estar marcada la opción 'Aplicable a vehículos'.

&#x20;         o Se utiliza en el caso de que el servicio definido se utilice en documentos de ventas y queramos además imputar el coste del servicio al vehículo.

&#x20;         o Estará activo por lo tanto sólo en el caso de que esté marcado “Aplicable a vehículos”.

* **Excluir de impuestos** (informe 347)

&#x20;         o Para casos de servicios especiales cuyo importe no debe repercutir en el cálculo del 347 (fianzas, tasas, etc...).

* **Exigir coste**

&#x20;         o Al utilizar este servicio en una línea de documento de ventas el usuario tendrá que imputar forzosamente un costo en la línea (caso por ejemplo de querer dejar reflejado en el documento de ventas el coste de un servicio externo simplemente a nivel estadístico).

&#x20;         o Pestaña Líneas de facturas de ventas: muestra la rejilla de documentos de venta indicando entidad, fecha, unidades y parcial de servicios.

![](<../../.gitbook/assets/image (520).png>)

&#x20;       o Pestaña Líneas de facturas de compras: muestra la rejilla de documentos de compra indicando entidad, fecha, unidades y parcial de servicios.

![](<../../.gitbook/assets/image (521).png>)

&#x20;       o Pestaña Auditoría: Permite controlar la creación del documento / ficha y la última modificación (usuarios). Además, se ha incorporado el control log de cada ficha que contenga la pestaña "Auditoría" que muestra el historial de modificaciones por parte de usuarios con fecha / hora / operación y acción realizada.
