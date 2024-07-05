# Tipo de movimiento

Winmotor hace una clasificación interna de los movimientos y en base a ésta trata de localizar el documento o ficha relacionado.

Este campo se calcula según los códigos aportados por la entidad que hemos mencionado anteriormente y en la lista de movimientos aparece como “Concepto”.

Los tipos de movimiento en los que Winmotor clasifica los registros bancarios son:

● <mark style="color:red;">Gastos</mark>

* Amortización de préstamo
* Gastos bancarios
* Devolución a cliente
* Impuestos
* Pago a empleado (Nómina)
* Pago a proveedor - acreedor
* Traspaso - salida

● <mark style="color:green;">Ingresos</mark>

* Ingresos bancarios
* Cobro a cliente
* Devolución a proveedor
* Remesa de efectos
* Traspaso - entrada

No es posible que el programa por sí sólo al descargar los datos sepa interpretar desde el primer día todos los tipos de movimientos: el único dato que tiene es si el importe es positivo o negativo y el contenido de la descripción del movimiento que le da el banco. Necesita por lo tanto “aprender” a identificar cada uno de estos tipos según el contenido de la descripción y el usuario tiene que ir dándole las claves para ello. Más adelante veremos cómo se hace esto.
