# Empresas

En la opción  _Empresas_ se encuentran todas las entidades dadas de alta con <mark style="color:red;">tipo de entidad Empresa</mark>.&#x20;

La entidad dada de alta como tipo Empresa será la que servirá al programa para administrar sus datos en los diferentes informes, así como la asignación del almacén principal, control de réplica de documentos, series por defecto a nivel empresa (es posible configurar series por defecto a nivel perfil de usuario) y configuración de departamentos laborales y RRHH.

<figure><img src="../../.gitbook/assets/image (652).png" alt=""><figcaption></figcaption></figure>

A continuación se muestra un ejemplo de ficha de entidad marcada como <mark style="color:red;">Empresa.</mark> Dentro de esta ficha, hay una pestaña llamada _**Conf. Empresa**_ en las que se configuran ciertos parámetros.

<figure><img src="../../.gitbook/assets/image (654).png" alt=""><figcaption></figcaption></figure>

**PESTAÑAS:**

{% tabs %}
{% tab title="Generales" %}
<figure><img src="../../.gitbook/assets/image (655).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="222">Campo</th><th width="594">Descripción</th></tr></thead><tbody><tr><td>Inscripción</td><td>En el registro para su impresión en los informes</td></tr><tr><td>Nº registro industria</td><td></td></tr><tr><td>Instancia</td><td>*NO MODIFICAR, CAMPO MANTENIDO POR WINMOTOR*</td></tr><tr><td>Almacén de la empresa</td><td>Identificación del almacén principal asignado</td></tr><tr><td>Control de almacenes por líneas de documentos</td><td>Permite que las líneas de un documento puedan tener origen en almacenes distintos</td></tr><tr><td>Tipo de empresa</td><td>En distribuciones <em>multicentro</em> nos permite indicar qué sede es la central y cuáles serían los puntos de venta o tiendas</td></tr><tr><td>Serie traspaso stock VO</td><td>Identificación de la serie de traspaso de VO si fuera necesario</td></tr><tr><td>Conexión Make</td><td>URL del escenario de Make de contactos</td></tr></tbody></table>
{% endtab %}

{% tab title="Series de documentos" %}
En esta pestaña nos encontramos con dos subpestañas:

* Series por defecto

<figure><img src="../../.gitbook/assets/image (657).png" alt=""><figcaption></figcaption></figure>

En ella podemos definir qué series por defecto aparecerán al dar de alta documentos a nivel empresa. Esto también es parametrizable a nivel [perfiles de usuarios](permisos-perfiles/perfiles.md) de forma que el nivel de control en la asignación se realizará a un nivel más detallado.&#x20;

* Réplica de documentos

En caso de que la empresa disponga de la <mark style="color:red;">distribución multicentro</mark> y cuenta con una central y un punto de venta, esta opción permite replicar documentos (pedidos y albaranes) generando el documento contrario. \
Por ejemplo, creando un albarán de ventas cuyo proveedor sea la central, permitirá crear el albarán de compras automáticamente en el punto de venta.

Para su funcionamiento se deberán rellenar los siguientes campos:

<figure><img src="../../.gitbook/assets/image (658).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Departamentos laborales" %}
\*Necesario módulo RRHH

En esta pestaña aparecen los distintos departamentos laborales creados anteriormente en la configuración del módulo de recursos humanos. Más información [aquí](../recursos-humanos-1/recursos-humanos/).

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Empresa - Horarios" %}
\*Necesario módulo RRHH

En esta pestaña aparecen los horarios de la empresa configurados anteriormente al igual que los departamentos. Para su configuración véase el siguiente [enlace](../recursos-humanos-1/recursos-humanos/).&#x20;

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Festivos" %}
\*Necesario módulo RRHH

En la pestaña de festivos aparecen los distintos ejercicios y sus correspondientes festivos. Sigue el siguiente [enlace](../recursos-humanos-1/recursos-humanos/) para ver la configuración de los festivos.

Leyenda de colores:

<div align="left"><figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure></div>

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}





* Departamentos laborales - Empresa - horarios y Festivos (exclusivamente del módulo RRHH): las 3 pestañas corresponden a la configuración del módulo RRHH en cuanto a qué departamento laboral o departamentos hemos asignado el control de recursos humanos, horario a nivel empresa y festivos.

![](<../../.gitbook/assets/image (455).png>)

Ficha del departamento laboral Taller > [Véase módulo de RRHH](../recursos-humanos-1/recursos-humanos/)

![Ficha del departamento laboral (2-T > Demo-Taller)](<../../.gitbook/assets/image (456).png>)

![Horarios a nivel empresa - RRHH](<../../.gitbook/assets/image (459).png>)

![Festivos a nivel empresa - RRHH](<../../.gitbook/assets/image (458).png>)
