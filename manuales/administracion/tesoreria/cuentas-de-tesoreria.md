# Cuentas de tesorería

Para dar de alta una nueva cuenta de tesorería desde el panel de Tesorería, debemos dar clic derecho _→_ Alta de ficha o dando doble clic en una zona sin datos de la rejilla

<figure><img src="../../../.gitbook/assets/image.png" alt="" width="362"><figcaption></figcaption></figure>

{% hint style="info" %}
IMPORTANTE

Para que un usuario pueda hacer uso de una cuenta de tesorería, es necesario que dicha cuenta esté configurada en el <mark style="color:red;">perfil</mark> de usuario correspondiente (a continuación se explica cómo realizar esta configuración).&#x20;

Una vez configurada, el usuario debe <mark style="color:red;">cerrar y volver a abrir el programa</mark> para que los cambios en el perfil se apliquen correctamente.
{% endhint %}

En el alta nos aparecerá una ventana emergente donde nos pide rellenar una serie de datos como el nombre de la cuenta, el tipo de cuenta o el número de cuenta

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

Los tipos de cuentas básicas son <mark style="color:red;">**Caja**</mark> y <mark style="color:red;">**Banco**</mark> determinando cada una el tipo de cuenta.&#x20;

* **Cuenta tipo CAJA**

<figure><img src="../../../.gitbook/assets/image (669).png" alt=""><figcaption></figcaption></figure>

Los campos a rellenar son:

<table><thead><tr><th width="188">Campo</th><th width="594">Descripción</th></tr></thead><tbody><tr><td>Código</td><td>Identificador interno de la cuenta. Se rellena automáticamente</td></tr><tr><td>Identificador</td><td>Identificador de la cuenta , por ejemplo CJ para la cuenta Caja Taller</td></tr><tr><td>Check Activa</td><td>Marca la situación de la cuenta (activa / inactiva)</td></tr><tr><td>Cuenta contable</td><td>Añade la cuenta de tesorería a la contabilidad</td></tr><tr><td>Crear asiento apertura<sup><mark style="color:red;">1</mark></sup></td><td>En el proceso de cierre de cuentas que permite generar automáticamente el asiento de apertura de caja correspondiente al día siguiente del cierre</td></tr><tr><td>Tipo de movimiento</td><td>"Movimientos especiales" / "Movimientos oficiales" / "Indistinto"</td></tr><tr><td>Canales de contado</td><td>Indican el procedimiento por el cual se realiza el pago</td></tr><tr><td> Cuentas contables (de cada canal)</td><td>Por cada uno de los 4 posibles canales de una cuenta de tesorería, es posible indicar una cuenta contable hacia la contabilidad</td></tr></tbody></table>

> <sup><mark style="color:red;">1<mark style="color:red;"></sup> Más información sobre la opción de Crear asiento apertura al cerrar cuenta
>
> Para su funcionamiento debe estar relleno el parámetro **Concepto apertura caja** dentro del formulario de Parámetros _→_ Administración _→_ Generales.&#x20;
>
> **Funcionamiento**
>
> En la opción **F6 - Cerrar cuenta**  del panel de tesorería, cuando seleccionemos una cuenta que tenga marcado el check mencionado anteriormente, nos aparecerán campos para definir la fecha del asiento (por defecto un día después a la fecha de cierre seleccionada), y el saldo de apertura (por defecto el saldo de la cuenta hasta el día de cierre. Solo tiene en cuenta movimientos con canal efectivo, es decir, que el canal del asiento sea igual al canal definido como canal de efectivo en la cuenta). Después de rellenar estos datos, el programa automáticamente creará en el día indicado una asiento de la caja correspodiente, con el concepto definido en el parámetro "concepto apertura caja", y el importe o saldo indicado.



* **Cuenta tipo BANCO**

&#x20;&#x20;

![](<../../../.gitbook/assets/imagen (116) (2).png>)

Se pueden añadir cuentas de tesorería tipo "Caja" con hasta 4 canales de entrada o añadir cuentas de forma independiente para cada canal, incluso cajas por departamento.

o Código: es un campo auto-numérico que nos servirá para identificar cada cuenta, en este caso el orden en el listado

o Identificador: es un campo auto-numérico que nos servirá para identificar cada cuenta, en este caso por tipo

o Check "Activa": marca la situación de la cuenta (activa / inactiva)

o Cuenta contable: añade la cuenta de tesorería a la contabilidad

o Tipo de cuenta: indica si la cuenta es tipo "Caja" o tipo "Banco"

o Cuenta bancaria: añade la cuenta bancaria a la que se asocia dicha cuenta de tesorería

o Opciones "Movimientos especiales" / "Movimientos oficiales" / "Indistinto": queda restringido a "movimientos oficiales"

Pestañas:

o Cierres: muestra los cierres de caja a su fecha (opción cerrar cuenta F6 del panel de tesorería), es decir, si el anterior cierre que se muestra es de hace una semana, el último acumulará el cierre de la cuenta de tesorería por intervalo de una semana.

o Perfiles: muestra los perfiles que tienen acceso a la cuenta de tesorería, además de permitir añadir o eliminar el acceso perfiles.

o Pagarés: permite configurar la impresión de pagarés

o Auditoría: datos sobre fecha de creación, usuario y fecha de modificación y usuario.
