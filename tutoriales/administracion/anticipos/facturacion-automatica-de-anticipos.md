# Facturación automática de anticipos

Opcionalmente podemos configurar Winmotor para que genere una factura por cada anticipo que se grabe sobre un pedido, operación u orden de reparación de taller.

En caso de activarse esta opción el sistema generará automáticamente una factura por cada anticipo grabado, calculando una base sin IVA sobre el importe recibido de manera que el total de la factura coincida dentro de lo posible con el anticipo. Dado que estamos limitados a dos decimales hay casos en los que quedará una diferencia de un céntimo entre los importes. Al hacer la factura definitiva por el resto este importe quedará compensado.

A diferencia del sistema sin factura en el que es el importe pendiente de cobro el que se reduce por el importe del anticipo, con este sistema activado, la factura final por el resto del importe se genera con una línea de descuento igual a la base del anticipo anteriormente recibido, de manera que el importe de la factura será la diferencia entre el anticipo y el total.

Por lo tanto si está activado el sistema de facturación de anticipos se imposibilita la posibilidad de cobrar anticipos por el total de un pedido u operación ya que la factura final sería de importe cero y en Winmotor no se permiten facturas sin importe.\


<mark style="color:yellow;">**Configuración**</mark>\


Accediendo a parámetros - Administración al final hay una nueva pestaña “Facturación de anticipos”:\


<figure><img src="https://lh7-us.googleusercontent.com/cS4_rxdZlMU4esotRcoVCWB6iiD4jAd3JFFNhq1LISb2F9YmcO6PeNpXnyiF9XksR5iVWl5CrpZ5Aajd6MqWXIhuL_P4_4yo89V-BKRgsxmV65kT3W1NRvIjzXKnSJ_zyvlhuvlELg-lJb4dqVR8BhA" alt=""><figcaption></figcaption></figure>

* El primer check hace de activador del sistema.
* Se puede seleccionar una serie específica para facturar los anticipos o seleccionar que se facturen en la “serie relativa al documento origen”. Esto quiere decir marcando este check, en caso de grabar un anticipo sobre un pedido de cliente éste se facturará en la serie de factura relativa al pedido (pedido - albarán - factura). En caso de una operación de vehículos o una orden de reparación el programa hace el mismo cálculo con las series.
* Hay que crear un servicio que actuará como concepto en la línea de anticipo tanto en la factura del anticipo como en la factura final donde éste se compensa.
  * No debe tener ninguna propiedad en particular&#x20;
  * Tampoco es necesaria una cuenta contable puesto que para estos casos el programa utilizará la cuenta de anticipos de clientes como explicaremos más adelante.
  * El nombre del servicio tampoco se utiliza ya que en la factura del anticipo el programa monta un texto compuesto con el documento origen: “Anticipo relativo a la operación: OPVN24-7” por ejemplo. En la factura de compensación se utiliza el mismo código para grabar el descuento por el anticipo pero en el concepto impone el texto “Compensación del anticipo”
  * El régimen de IVA si es importante: siempre que el régimen de IVA relativo al cliente aplique un porcentaje de IVA se aplicará el definido en este servicio. Si el IVA relativo al cliente no aplica cuota, no se aplicará ninguno.
* El tipo de pago es “neutro”, no va a afectar en nada a la factura generada ya que esta se va a dar siempre por cobrada por el asiento de tesorería relativo al anticipo; simplemente debe ser un tipo de pago de contado para que no se genere cartera por esta factura.
* Como ya hemos explicado el importe mínimo de la diferencia no puede ser inferior a un Euro pero se puede aumentar.

\
<mark style="color:yellow;">**Funcionamiento**</mark>\


Además de crear esta configuración no hay que hacer nada especial para el funcionamiento de los anticipos, la factura se generará automáticamente cuando se cree un anticipo y éste se compensará en la factura final del documento desde el que se haya creado.\


<mark style="color:yellow;">**Contabilización**</mark>\


En caso de estar activado este sistema, la contabilización de los anticipos cambia completamente ya que en lugar de gestionarse la cuenta de anticipos de clientes (438) por tesorería se hace por gestión.

* La contabilización del asiento de tesorería por el cobro del anticipo queda así:

<figure><img src="https://lh7-us.googleusercontent.com/46r6fHjqrwUShlep4Mgte0M-YudFoMirUMGC-z8tYn7VaxuG1sBhwnz3Ru_6koY9CA472Nwm2VR_tSVWiO1wPt7S3HRKwCYtX6hJLkHXXYgESTonY0UIqGrrwjJR1mvvRQpKgZl0b4Ux6c6tGJ3eADk" alt=""><figcaption></figcaption></figure>

* El asiento relativo a la factura del anticipo aplica como base la 438 en lugar de una cuenta del grupo 7:

<figure><img src="https://lh7-us.googleusercontent.com/q1XdLSq4uhm5tGr9q-4dFr42_7ykMCRpGdRdLzcJfINHFEyLdJZ37XcAMV-4ZQr5W-wCM7Kte1gGAEaCg1vqx92WFHjAuBlCmWnaSndPBIamO5rIh9feIKri8e3OyCKeUh03tt8oETc-fa_pDERYWy0" alt=""><figcaption></figcaption></figure>

* El asiento de la factura final donde se compensa el anticipo regulariza la 438&#x20;

<figure><img src="https://lh7-us.googleusercontent.com/_Fw02W9XOdwImuKoozN96PpgDwNLktMMHVR-Cr491RpDS_ZPKBip5f4-CjgLXZRkLy6ZuBNYxkwsPmzV6jf0l_4vL-eo70lop-o9PlZdMzfQWwEfVoXVm2DDA7M7Z2LywcheGNgqxpK3rLYmHUlzFtQ" alt=""><figcaption></figcaption></figure>

El programa crea automáticamente la 438 relativa al cliente en caso de que no exista.

\
