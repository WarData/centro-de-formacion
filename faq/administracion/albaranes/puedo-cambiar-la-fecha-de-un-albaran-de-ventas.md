# ¿Puedo cambiar la fecha de un albarán de ventas?

A diferencia del albarán de compras, el de ventas es un documento que SACA material del almacén por lo que el programa cada vez que grabamos una línea del albarán comprueba si en el almacén relativo al albarán hay existencias disponibles suficientes para poder grabar la línea. Al grabar una compra no es necesaria ninguna comprobación de este tipo, simplemente se añade material al stock.

Por otro lado, en Winmotor controlamos el stock y el precio medio de coste línea a línea lo que posibilita que podamos hacer una consulta de stock a fecha. Esto quiere decir que, por cada línea de documento relativo a stock que grabamos se calcula el stock resultante y el PMC aplicable a esa línea. Si es un albarán de compras, el PMC se recalcula, si es de ventas, se aplica el que ya hubiera. Se puede hacer esta comprobación fácilmente en la ficha de un artículo, en la pestaña 'Histórico - Movimientos de stock'.

Para poder controlar esto de una forma rigurosa y con sentido hay que evitar que un albarán pueda cambiar de fecha: para hacerlo el programa tendría que calcular por cada una de sus líneas si es posible o no el cambio de fecha y recalcular por otro lado el stock y el precio medio de costo de todas las líneas posteriores a la nueva fecha aplicada en cada uno de los artículos afectados
