# Wincoins

1.- <mark style="color:orange;">**Información:**</mark>



Se trata de controlar en la aplicación la gestión de puntos que se acumularán por cada venta, y que servirán para aplicar en futuras ventas como descuento de la misma.

Por defecto el nombre de la "moneda" será Wincoins pero cada empresa podrá establecer el nombre que más le interese.

* Se puede definir una cuota de aplicación en series de albaranes de venta, OR y facturas de venta. Y como añadido, se podrá tanto en familias como en artículos definir una cuota de aplicación o puntos por unidad
  * Prevalece lo definido en el artículo, luego lo definido en la familia, y por último lo de la serie. Se podrá por ejemplo solo definir una cuota de aplicación por serie y no definir ni en artículos ni familias. En series es imprescindible definir.
* Por otro lado, se podrán compensar puntos, es decir, hacer descuento, solo en las series de albaranes de venta, OR o facturas que marquemos: "descuentos aplicables".
* Cada Wincoin acumulado equivale siempre a 1 euro. Si tengo 7 Wincoins acumulados, descontaremos en la venta 7 euros.
* Se podrá parametrizar los tipos de entidad a los que se excluye la aplicación de Wincoins. Esta acción solo la podrá realizar Winmotor.
* Se podrán excluir líneas de venta puntales de la aplicación de Wincoins. Para ello hay un nuevo check en líneas de documento "excluir Wincoins".
* Los abonos de las ventas que generaron Wincoins descontarán saldo en el monedero del cliente.
* Los abonos de las ventas que consumieron Wincoins devolverán el saldo consumido al monedero del cliente.
* En el ticket o factura, se indicarán los puntos descontados en esa venta, así como el saldo actual del cliente.
  * Esto está pendiente de que nos indiquen en que parte del informe añadir.
* Cada venta que acumule saldo registrará la fecha de la venta y tendrá un periodo de validez definido en parámetros.
  * Si tenemos definido que el periodo de validez son 365 días, y el cliente ha realizado dos compras, la caducidad quedará así:
    * Venta 15 enero, 5 Wincoins, caducan el 14 de enero del año siguiente.
    * Venta 20 mayo, 7 Wincoins, caducan el 19 de mayo del año siguiente.

2.-  <mark style="color:orange;">**Configuración a realizar:**</mark>

* &#x20;Cuota de aplicación en series, familias (opcional) y artículos (opcional)
* Marcar en que series se aplica descuentos.
*   Parámetros a rellenar:



<figure><img src="../.gitbook/assets/4e16cb54-7e22-4a57-aeda-d4a80c67ef31.png" alt=""><figcaption></figcaption></figure>

3.- <mark style="color:orange;">**Funcionamiento:**</mark>

* Si por ejemplo hemos rellenado en la serie AV una cuota de aplicación del 2%, por cada línea grabada el programa calculará automáticamente un 2% sobre la base en Wincoins.
* Se podrá consultar los Wincoins aplicados en cada línea y totales con el botón situado en la parte inferior "Wincoins"
* Se podrá disponer de esos Wincoins en cualquier otra venta de serie donde hayamos marcado "descuentos aplicables". Para ello nos aparecerá un botón "compensar saldo". Al pulsarlo nos aparecerá un botón con la base del documento, los Wincoins disponibles, y el importe a aplicar. Podemos seleccionar como máximo ese importe, pero también podremos aplicar menos. En ese mismo formulario hay un botón para ver en detalle el saldo, así como el histórico (por si queremos ver líneas caducadas, consumidas, etc.). Si aceptamos este formulario con un importe positivo, se creará una nueva línea en el documento con el servicio parametrizado.
* En los clientes, hay un nuevo botón para ver el saldo y el histórico de Wincoins ![](<../.gitbook/assets/Screenshot\_3 (1).png>)

<figure><img src="../.gitbook/assets/Screenshot_4 (1).png" alt=""><figcaption></figcaption></figure>

* En el panel de entidades hay un nuevo botón para sacar listado de clientes con saldo, el detalle del saldo, etc.

<figure><img src="../.gitbook/assets/Screenshot_2 (1).png" alt=""><figcaption></figcaption></figure>
