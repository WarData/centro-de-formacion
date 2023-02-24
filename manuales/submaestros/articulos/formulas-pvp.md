# Fórmulas PVP

Para una gestión automatizada de los precios de ventas se aconseja no definir manualmente ningún precio de venta sino establecer una regla para su cálculo de manera que cuando cambie el precio de compra se modificará automáticamente el precio de venta del producto.

![](<../../../.gitbook/assets/image (16) (1).png>)

Estas reglas se pueden definir en su opción correspondiente en el menú de Submaestros > Artículos > “Fórmulas PVP” o manualmente desde una ficha de familia o de artículo. Si definimos en una familia una “fórmula para el cálculo del pvp” ésta se aplicará automáticamente a los artículos a los que se asigne dicha familia.

Para la edición de fórmulas de cálculo de pvp el programa presenta un asistente donde se podrá operar con los datos del artículo. Lo más lógico será siempre establecer una fórmula que parta del precio de tarifa de compras o del precio neto de compras del artículo y sobre éste aplicar un incremento. Dado que el asistente es algo complejo se recomienda solicitar ayuda a Winmotor la primera vez que se vaya a utilizar.

**Ejemplos:**

1 - Poner manualmente el precio de venta en el artículo

2 - Crear una fórmula para el calculo del PVP: serie : #ART.TAR\_COMP\_PREF.PTARIFA \* 1.15

\- Esta fórmula la podemos aplicar en una **familia** (se actualizará el precio de venta en todos los articulos de la familia aplicando a su precio tarifa un 15% de incremento) o **directamente en el artículo**
