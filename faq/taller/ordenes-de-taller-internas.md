# Órdenes de taller internas

**Sistema general de tratamiento para las órdenes de taller internas - Factura no reglada**



* Una orden con cargo interno no genera ningún importe, todo es pérdida. Es decir, la empresa no recibe nada por la reparación por lo que todo el coste de la orden es pérdida.
* Al grabar una partida con cargo interno dentro de una orden nos pedirá un “Departamento”. Es un dato estadístico e implica qué departamento de la empresa asume el costo de esa reparación. En el caso de las preentregas será con cargo al departamento comercial, y por lo general, en el resto de casos serán con cargo al taller (reparaciones incorrectas, pérdidas de material, etc). En el panel de estadísticas de recambios se puede hacer un filtro por este departamento siempre que se incluyan los tipos de documentos “Órdenes de reparación”. Una vez calculada la estadística aparece un botón donde podemos filtrar por departamento.
* Dado que en Winmotor los importes que se muestran en la pestaña inicial de las órdenes es el importe a recibir, en el caso de las órdenes internas todos los importes aparecen a cero.

<img src="../../.gitbook/assets/unknown (21).png" alt="" height="81" width="624">

* Si queremos ver los importes en detalle de una factura de este tipo es cuestión de ir a la pestaña “Estadísticas” de la OR y hacer doble click en la línea de cargo “Interno”. Nos mostrará en detalle cada coste repercutido a la orden:

<img src="../../.gitbook/assets/unknown (22).png" alt="" height="567" width="624">

* Aunque las órdenes internas se facturan las facturas generadas no son “reguladas”. Es decir, facturamos la orden para darla por terminada y las facturas generadas no se contabilizan ni se incluyen en el cálculo de ningún impuesto puesto que configuramos las series con esos parámetros:

<img src="../../.gitbook/assets/unknown (23).png" alt="" height="151" width="624">

* Las facturas generadas desde una orden interna de este tipo están “trucadas”: aparentemente tienen como importe el coste pero si vemos la estadística en la factura veremos que no toma en cuenta ese importe, todo el importe de la factura sigue siendo pérdida.

\
<br>
