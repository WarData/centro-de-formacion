# Cuentas de tesorería

Para dar de alta una nueva cuenta de tesorería desde el panel de Tesorería, debemos dar clic derecho _→_ Alta de ficha o dando doble clic en una zona sin datos de la rejilla

<figure><img src="../../../.gitbook/assets/image (1).png" alt="" width="362"><figcaption></figcaption></figure>

{% hint style="info" %}
IMPORTANTE

Para que un usuario pueda hacer uso de una cuenta de tesorería, es necesario que dicha cuenta esté configurada en el <mark style="color:red;">perfil</mark> de usuario correspondiente (al final, en pestañas comunes, se explica cómo realizar esta configuración).&#x20;

Una vez configurada, el usuario debe <mark style="color:red;">cerrar y volver a abrir el programa</mark> para que los cambios en el perfil se apliquen correctamente.
{% endhint %}

En el alta nos aparecerá una ventana emergente donde nos pide rellenar una serie de datos como el nombre de la cuenta, el tipo de cuenta o el número de cuenta

<figure><img src="../../../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../../../.gitbook/assets/image (671).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="188">Campo</th><th width="594">Descripción</th></tr></thead><tbody><tr><td>Código</td><td>Identificador interno de la cuenta. Se rellena automáticamente</td></tr><tr><td>Identificador</td><td>Identificador de la cuenta , por ejemplo CJ para la cuenta Caja Taller</td></tr><tr><td>Check Activa</td><td>Marca la situación de la cuenta (activa / inactiva)</td></tr><tr><td>Cuenta contable</td><td>Añade la cuenta de tesorería a la contabilidad</td></tr><tr><td>Cuenta bancaria</td><td>Añade la cuenta bancaria a la que se asocia dicha cuenta de tesorería</td></tr><tr><td>Tipo de movimiento</td><td>"Movimientos especiales" / "Movimientos oficiales" / "Indistinto"</td></tr><tr><td>Canales de contado</td><td>Indican el procedimiento por el cual se realiza el pago</td></tr><tr><td> Cuentas contables (de cada canal)</td><td>Por cada uno de los 4 posibles canales de una cuenta de tesorería, es posible indicar una cuenta contable hacia la contabilidad</td></tr></tbody></table>

**Pestañas comunes de cuentas de tesorería:**

{% tabs %}
{% tab title="Cierres" %}
Muestra los cierres de caja a su fecha (opción cerrar cuenta F6 del panel de tesorería), es decir, si el anterior cierre que se muestra es de hace una semana, el último acumulará el cierre de la cuenta de tesorería por intervalo de una semana.

<figure><img src="../../../.gitbook/assets/image (673).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Perfiles" %}
Muestra los perfiles que tienen acceso a la cuenta de tesorería en la rejilla izquierda y en la rejilla derecha los perfiles que no tienen acceso. Para quitar o añadir un perfil basta con seleccionarlo y clicar en la flecha correspondiente

<figure><img src="../../../.gitbook/assets/image (674).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Integrador Bancario" %}
<figure><img src="../../../.gitbook/assets/image (675).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Pagarés" %}
Permite configurar la impresión de pagarés

<figure><img src="../../../.gitbook/assets/image (676).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Auditoría" %}
Indica datos sobre fecha de creación y usuario que lo creó y, fecha de modificación y usuario que modificó

<figure><img src="../../../.gitbook/assets/image (677).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
