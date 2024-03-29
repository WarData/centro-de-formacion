# Remesa de cobros

Una remesa de cobro es un conjunto de efectos a cobrar que el usuario incluye en el documento 'remesa' y que envía al banco en un fichero generado por la aplicación. Este fichero admite varios formatos que hay que acordar con el banco.

En Winmotor disponemos de la opción de remesas de cobros, pagos [(véase remesa de pagos)](remesa-de-pagos/) y nóminas [(véase remesa de nóminas)](remesa-de-pagos/remesa-de-nominas.md)

Para realizar una remesa de cobros los pasos son los siguientes:

1.- Dar de alta una serie de remesas de cobros. La imagen muestra la opción de cobros y pagos por lo que es importante diferenciarla al inicio de la configuración:

<figure><img src="../../../.gitbook/assets/imagen (4) (3) (1) (1).png" alt=""><figcaption></figcaption></figure>

En la serie nos permite seleccionar la cuenta bancaria, tipo de remesa y el formato del archivo para el banco por defecto, aunque posteriormente veremos que se puede modificar antes de crear la remesa.

2.- En el menú ADMINISTRACIÓN > Remesas de cobros > obtendremos el panel de remesas con una serie de opciones (intervalo, serie a mostrar en la rejilla, cambio a rejilla avanzada, localizar remesa por código y definir el panel con las opciones elegidas como por defecto) y una rejilla con las remesas creadas indicando su código, fecha de alta, cuenta bancaria, registro, control de devoluciones y el importe total de la remesa:

<figure><img src="../../../.gitbook/assets/imagen (15) (3) (1).png" alt=""><figcaption></figcaption></figure>

3.- Pulsando el siguiente botón daremos de alta una nueva remesa:

<figure><img src="../../../.gitbook/assets/imagen (9) (2) (2).png" alt=""><figcaption></figcaption></figure>

4.- En el formulario de alta seleccionaremos la cuenta (si en la serie indicamos una saldrá por defecto aunque es modificable en el alta), intervalo de vencimiento y tipo de pago:

<figure><img src="../../../.gitbook/assets/imagen (1) (3) (1) (1).png" alt=""><figcaption></figcaption></figure>

5.- En el siguiente panel nos mostrará todas las facturas de ventas:

<figure><img src="../../../.gitbook/assets/imagen (105) (2).png" alt=""><figcaption></figcaption></figure>

6.- Ahora seleccionamos aquellas que queremos incorporar al fichero para el banco y pulsamos en la flecha que indica hacia abajo. De igual modo, podemos seleccionar facturas añadidas al fichero y pulsar en la flecha que indica hacia arriba para que sea "remesable" no "remesada":

<figure><img src="../../../.gitbook/assets/imagen (5) (3) (1).png" alt=""><figcaption></figcaption></figure>

7.- Una vez remesados, nos aparece un nuevo botón "Crear archivo bancario" para guardar el archivo generado en el equipo pudiendo aquí cambiar el formato de la remesa, la fecha disco y la fecha cargo:

<figure><img src="../../../.gitbook/assets/imagen (6) (1) (2).png" alt=""><figcaption></figcaption></figure>

Antes de pasar las facturas, en la remesa de cobro ya dada de alta, tenemos opciones modificables como el vencimiento, tipo de pago y selección por texto con lo que podremos ir añadiendo facturas a una misma remesa con diferentes opciones tras modificar los parámetros indicados.

Esto quiere decir que conforme hayamos añadido facturas al panel "remesados", podemos cambiar los valores de vencimiento o tipo de pago y añadir nuevas facturas a "remesados".

La remesa de cobro dada de alta irá añadiendo facturas a "remesables" conforme se vayan dando de alta y estas cumplan los requisitos de tipo de pago y vencimiento indicados en la misma.
