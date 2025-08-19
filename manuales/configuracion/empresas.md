# Empresas

En la opción  _Empresas_ se encuentran todas las entidades dadas de alta con <mark style="color:red;">tipo de entidad Empresa</mark>.&#x20;

La entidad dada de alta como tipo Empresa será la que servirá al programa para administrar sus datos en los diferentes informes, así como la asignación del almacén principal, control de réplica de documentos, series por defecto a nivel empresa (es posible configurar series por defecto a nivel perfil de usuario) y configuración de departamentos laborales y RRHH.

<figure><img src="../../.gitbook/assets/image (652).png" alt=""><figcaption></figcaption></figure>

A continuación se muestra un ejemplo de ficha de entidad marcada como <mark style="color:red;">Empresa.</mark> Dentro de esta ficha, hay una pestaña llamada _**Conf. Empresa**_ en las que se configuran ciertos parámetro.

<figure><img src="../../.gitbook/assets/image (654).png" alt=""><figcaption></figcaption></figure>

**PESTAÑAS:**

{% tabs %}
{% tab title="Generales" %}
<table><thead><tr><th width="222">Campo</th><th width="594">Descripción</th></tr></thead><tbody><tr><td>Inscripción</td><td>En el registro para su impresión en los informes</td></tr><tr><td>Nº registro industria</td><td></td></tr><tr><td>Instancia</td><td>*NO MODIFICAR, CAMPO MANTENIDO POR WINMOTOR*</td></tr><tr><td>Almacén de la empresa</td><td>Identificación del almacén principal asignado</td></tr><tr><td>Control de almacenes por líneas de documentos</td><td>Permite que las líneas de un documento puedan tener origen en almacenes distintos</td></tr><tr><td>Tipo de empresa</td><td>En distribuciones <em>multicentro</em> nos permite indicar qué sede es la central y cuáles serían los puntos de venta o tiendas</td></tr><tr><td>Serie traspaso stock VO</td><td>Identificación de la serie de traspaso de VO si fuera necesario</td></tr><tr><td>Conexión Make</td><td>URL del escenario de Make de contactos</td></tr></tbody></table>
{% endtab %}

{% tab title="Series de documentos" %}
S
{% endtab %}

{% tab title="Departamentos laborales" %}

{% endtab %}

{% tab title="Empresa - Horarios" %}

{% endtab %}

{% tab title="Festivos" %}

{% endtab %}
{% endtabs %}

*

![](<../../.gitbook/assets/image (452).png>)

* Series de documentos: Aquí disponemos de 2 pestañas:

o Series por defecto: podemos definir qué series por defecto aparecerán al dar de alta documentos como por ejemplo albaranes, facturas, pero a nivel empresa, ya que también podemos asignar series por defecto a perfiles que a su vez incluyen usuarios, por lo que el nivel de control en la asignación se realizará a un nivel más detallado.

![](<../../.gitbook/assets/image (453).png>)

o Réplica de documentos: si la empresa dispone de la distribución multicentro y cuenta con una central y un punto de venta, es posible configurar la réplica de documentos generando el documento contrario al creado con pulsar únicamente el botón "Replicar documento". Aparece en pedidos y albaranes (depende de las necesidades del cliente): creando un albarán de ventas cuyo proveedor sea la central, permitirá crear el albarán de compras automáticamente en el punto de venta.

![](<../../.gitbook/assets/image (454).png>)

* Departamentos laborales - Empresa - horarios y Festivos (exclusivamente del módulo RRHH): las 3 pestañas corresponden a la configuración del módulo RRHH en cuanto a qué departamento laboral o departamentos hemos asignado el control de recursos humanos, horario a nivel empresa y festivos.

![](<../../.gitbook/assets/image (455).png>)

Ficha del departamento laboral Taller > [Véase módulo de RRHH](../recursos-humanos-1/recursos-humanos/)

![Ficha del departamento laboral (2-T > Demo-Taller)](<../../.gitbook/assets/image (456).png>)

![Horarios a nivel empresa - RRHH](<../../.gitbook/assets/image (459).png>)

![Festivos a nivel empresa - RRHH](<../../.gitbook/assets/image (458).png>)
