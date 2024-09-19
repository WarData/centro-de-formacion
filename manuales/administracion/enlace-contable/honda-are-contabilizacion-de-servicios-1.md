# Operativa para la gestión de las motos eléctricas en el informe Honda ARE

Nueva operativa específica de Honda ARE para gestionar en el informe mensual y en la contabilidad las motos eléctricas en códigos específicos. Por otro lado Honda exige que la venta de cada moto eléctrica incluya la batería y el cargador que deben detallarse en la factura y aparecer sin cargo.

El objetivo de Honda en definitiva se resume en :

* Obtener datos de ventas y stock en las nuevas casillas que han creado para ello en el Honda ARE.
* A nivel contable recoger como coste de cada venta de moto eléctrica el coste de la moto, la batería y el cargador.

A nivel Winmotor tanto la batería como el cargador son artículos normales del tipo recambio con lo que podremos controlar sus stocks como los de cualquier otro recambio . Más abajo explicamos lo que hay que hacer para gestionarlos en los documentos de ventas.



_**Cómo funciona:**_

* En contabilidad debes crear las siguientes cuentas auxiliares:

<figure><img src="../../../.gitbook/assets/Screenshot_1 (2).png" alt=""><figcaption></figcaption></figure>

* Para el control de la moto eléctrica
  * Marcar en la ficha del modelo de vehículo si es eléctrico en el nuevo campo

<figure><img src="../../../.gitbook/assets/Screenshot_2 (2).png" alt=""><figcaption></figcaption></figure>

* Para el control de la batería el cargador&#x20;
  * Marcar en las fichas de los artículos que deben entregarse con el vehículo que son "Aplicables  a vehículo eléctrico". Hay que entrar en la pestaña "Propiedades" de cada uno de estos artículos

<figure><img src="../../../.gitbook/assets/Screenshot_3 (2).png" alt=""><figcaption></figcaption></figure>

* Estos artículos pueden venderse también sin estar relacionados con la venta de un vehículo. El programa los considerará a incluir en el ARE como venta de un vehículo cuando estén incluidos en un documento de ventas en el que haya un vehículo y se hayan grabado después del vehículo.
* Si quieres que queden incluidos automáticamente cada vez que se vende un vehículo eléctrico se pueden añadir como "Anexos del vehículo". Los anexos los puedes crear desde la propia ficha del vehículo o desde el panel de gestión de anexos y tarifas de vehículos. Al crearlos, para que el proceso completo quede automatizado marca las casillas "Incluir en factura de vehículo" y "Detallar en factura"

<figure><img src="../../../.gitbook/assets/Screenshot_4 (2).png" alt=""><figcaption></figcaption></figure>

* Para que la moto aparezca en el ARE en su casilla correcta tienes que crear la serie SCEL - "Scooter eléctrico" y aplicarle la gama de vehículo que tengas asociado a los modelos eléctricos.

<figure><img src="../../../.gitbook/assets/Screenshot_5 (1).png" alt=""><figcaption></figcaption></figure>

* Después en el botón "Honda" definir todos los parámetros de cuentas contables y códigos ICIS de la siguiente forma:

<figure><img src="../../../.gitbook/assets/Screenshot_6 (1).png" alt=""><figcaption></figcaption></figure>

* Los nuevos códigos ICIS relativos a motos eléctricas los hemos creado ya desde Winmotor.
