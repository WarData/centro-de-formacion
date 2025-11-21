# Series de Documentos

Todos los documentos en Winmotor se clasifican por series. Cada serie implica un contador para los documentos que incluya.

{% hint style="info" %}
Las series son ilimitadas. Se pueden crear tantas series por tipo de documento como se desee
{% endhint %}

<figure><img src="../../.gitbook/assets/image (619).png" alt="" width="563"><figcaption></figcaption></figure>

Los campos a rellenar al crear una serie son:

<table><thead><tr><th width="170">Campo</th><th width="594">Descripción</th></tr></thead><tbody><tr><td>Código</td><td>Identificador interno de la serie. Se rellena automáticamente</td></tr><tr><td>Referencia</td><td>Identificador de la serie con tamaño máximo de 6 caracteres alfanuméricos. Se recomienda utilizar abreviaturas que identifiquen claramente el tipo de documento sobre el que se va a utilizar, por ejemplo, AC para Albarán de compras / FVVO para Factura de ventas de vehículo de ocasión</td></tr><tr><td>Empresa</td><td>Presenta por defecto la empresa activa en parámetros, se rellena automáticamente</td></tr><tr><td>Tipo de documento</td><td>Hace referencia al tipo de documento sobre el que se podrá utilizar la serie</td></tr><tr><td>Serie abono</td><td>Check que marca si la serie se utilizará para abono de documentos en caso de ser albaranes o facturas</td></tr><tr><td>Serie activa</td><td>Check que indica si la serie puede ser utilizada o no. En caso de estar desmarcada no aparecerá al seleccionar serie en un documento</td></tr></tbody></table>

Tenemos dos formas de dar de alta una serie:

* Haciendo doble clic en la rejilla de forma que crearemos de cero la serie
* Desde el botón <mark style="color:red;">**Duplicar**</mark> de una serie ya existente. De esta forma se creará una nueva serie a la que le tendremos que poner una nueva referencia y empezar con el contador e histórico de cero. Las características y configuraciones las copiará de la serie original

<figure><img src="../../.gitbook/assets/image (642).png" alt="" width="563"><figcaption></figcaption></figure>

**PESTAÑAS:**

**Pestaña “Valores por defecto”:** Según el tipo de documento relacionado a la serie se nos presentarán en esta pestaña distintos campos. Vamos a ir enumerándolos por tipos de documentos:

\*\* Facturas Emitidas \*\*

o Serie de abono

Si estamos grabando una serie para albaranes o facturas identificaremos aquí la serie que se utilizará para crear un documento de abono relativo a un documento de esta serie. Para definir aquí una serie de abono es necesario haber grabado previamente una serie de facturas de ventas identificada como “Serie de abono”.

o Descuento máximo aplicable

Nos permite definir un descuento máximo para aplicar en las líneas de la factura. Rellenando este campo limitaremos el porcentaje de descuento que un usuario final podrá aplicar en esta serie de documentos. Los usuarios “supervisores” quedan fuera de esta restricción, podrán utilizar un descuento superior al aquí definido.

o Forzar Vencimiento

Marcando este check el programa cuando genera una factura automáticamente desde uno o varios albaranes ignorará el tipo de pago y los vencimientos definidos en la ficha del cliente e impondrá para estos campos los que se definan dentro del recuadro.

**Albaranes de ventas**

o Facturar automáticamente: Marcando este check forzaremos a que en el momento de confirmar un albarán de esta serie quedará automáticamente facturado. Muy práctico por ejemplo para ventas de mostrador en las que es necesario crear siempre una factura por cada albarán o ticket emitido sin necesidad de que el usuario tenga que recordarlo.

o Serie para garantías: Si utiliza una distribución de Winmotor para concesionarios de vehículos le aparecerá este check que indica que la serie en curso se utilizará para entregas de mercancía en garantía.

o Serie destino: Para el caso de albaranes de ventas en serie destino tendremos que identificar la serie de facturación que recogerá los albaranes de esta serie.

o Serie abono: Identifica la serie de albarán de ventas que recogerá a este albarán en caso de abonarse alguna de sus líneas. Para identificar aquí una serie de abono es necesario haber creado previamente una serie de albaranes de ventas identificada como “Serie de abono”.

o Entidad por defecto: Con este campo podemos forzar a que todos los albaranes creados con esta serie tomen siempre el mismo cliente. Muy usado para configuración de TPV (Terminales punto de venta) en los que se identifica en este campo el código de “Clientes varios”.

o Descuento máximo aplicable: Nos permite definir un descuento máximo para aplicar en las líneas de la factura. Rellenando este campo limitaremos el porcentaje de descuento que un usuario final podrá aplicar en esta serie de documentos. Los usuarios “supervisores” quedan fuera de esta restricción, podrán utilizar un descuento superior al aquí definido

\*\* Presupuestos de ventas \*\*

o Serie destino pedido cliente: Identifica la serie que tomará el pedido de ventas en caso de confirmar un presupuesto creado en esta serie.

o Serie destino factura: Identifica la serie que tomará la factura de ventas que se genere en caso de convertir directamente el presupuesto en factura.

o Imputación: En distribuciones de Winmotor para Servicios de Asistencia Técnica se utilizará este campo para definir en la generación de un parte de trabajo el tipo de imputación que generará en dicho parte ( cliente, garantía, etc).

o Descuento máximo aplicable: Nos permite definir un descuento máximo para aplicar en las líneas de la factura. Rellenando este campo limitaremos el porcentaje de descuento que un usuario final podrá aplicar en esta serie de documentos. Los usuarios “supervisores” quedan fuera de esta restricción, podrán utilizar un descuento superior al aquí definido

**Pedido Cliente**

o Serie para garantía: Si utiliza una distribución de Winmotor para concesionarios de vehículos le aparecerá este check que indica que la serie en curso se utilizará para entregas de mercancía en garantía.

o Serie pedido compra: Identifica la serie que debe tomar el pedido de ventas en caso de generar un pedido a proveedor al tramitarlo.

o Serie albarán venta: Identifica la serie que tomará en el caso de confirmar un pedido y convertirlo en albarán de entrega.

o Genera pedidos de compras únicos: Marcando este check definimos para el proceso de generación de pedidos de compras que genere siempre un nuevo pedido a proveedor aunque haya otros pedidos de compras abiertos de este proveedor. En caso de no estar marcado y existir un pedido a proveedor abierto el programa añadirá las unidades a pedir en ese pedido.

o Generar pedidos de compras por todas las unidades pedidas: Normalmente el programa generará pedidos de compras por la diferencia entre lo que nos pide el cliente y el stock disponible del artículo. Si marcamos este check el comportamiento del programa será generar pedidos de compras por todas las unidades pedidas por el cliente, independientemente del stock disponible que tengamos.

o Descuento máximo aplicable: Nos permite definir un descuento máximo para aplicar en las líneas de la factura. Rellenando este campo limitaremos el porcentaje de descuento que un usuario final podrá aplicar en esta serie de documentos. Los usuarios “supervisores” quedan fuera de esta restricción, podrán utilizar un descuento superior al aquí definido

o Pedidos de ventas no tramitables: La marcación de este check fuerza a los pedidos generados en esta serie a que no se puedan tramitar, o sea, convertir en albarán de ventas. Se utiliza para distribuciones de Winmotor en las que manejamos pedidos que sirven otras empresas.

\*\* Facturas recibidas \*\*

o Serie de abono: Identifica para el caso de abonar una factura de proveedor en esta serie en qué serie se generará el abono.

\*\* Albarán de compras \*\*

o Facturar automáticamente: Al marcar este check forzamos a que la confirmación de un albarán de esta serie generará automáticamente su correspondiente factura recibida.

o Serie destino: Identifica la serie de factura emitida en la que se recogerá este albarán en el caso de facturarse.

o Serie abono: Identifica la serie de albarán de compras que recogerá a este albarán en caso de abonarse alguna de sus líneas. Para identificar aquí una serie de abono es necesario haber creado previamente una serie de albaranes de compras identificada como “Serie de abono”.

\*\* Pedido Proveedor \*\*

o Serie destino: Identifica la serie de albarán de compras en la que se generarán las líneas del pedido en caso de recibirse.

o Propuesta de pedido

o Serie destino: Identifica la serie para el pedido de compras que se generará en caso de confirmar la propuesta.

o Modelo de rejilla: Según seleccionemos “ampliado” o “reducido” se presentarán más columnas en la rejilla de líneas de la propuesta. Para seleccionar la rejilla ampliada es recomendable utilizar una pantalla para confeccionar propuestas con una alta resolución.

o Tipos de artículo a incluir en el cálculo: Podemos con este campo limitar la propuesta de pedido a un tipo de artículo concreto. En caso de no seleccionar nada el programa calculará la propuesta para todos los tipos de artículos de nuestra distribución.

Pestaña "Contabilidad”: afecta a las opciones contables de las series:

o Serie regulada: activa y controlada por la aplicación

o Serie interna: aquella destinada a procesos internos del Concesionario y/o entre departamentos

o Contabilizar: check que permite activar o no la serie en contabilidad

<figure><img src="../../.gitbook/assets/image (624).png" alt="" width="563"><figcaption></figcaption></figure>

Pestaña "Impresión": permite variar las opciones referentes a la impresión de los informes asociados a dicha serie:

o Impresión por tipo de pago: permite diferenciar el informe por tipo de pago

o Identificadores: indican el código del informe que usará la serie para realizar la impresión, así como el destino (impresora), PDF y número de copias.

o Notas al pie de página y otros textos: permite añadir textos al informe pre-diseñado.

<figure><img src="../../.gitbook/assets/image (625).png" alt="" width="563"><figcaption></figcaption></figure>

**Pestaña "Logos":** permite añadir logotipos para identificar las distintas serie

<figure><img src="../../.gitbook/assets/image (626).png" alt="" width="563"><figcaption></figcaption></figure>

**Pestaña "Observaciones":** si el informe dispone de un campo observaciones, se aplicarán las añadidas a la serie. También permite añadir observaciones internas que únicamente aparecerán en esta pestaña y campo:

<figure><img src="../../.gitbook/assets/image (627).png" alt="" width="563"><figcaption></figcaption></figure>

Pestaña "Contadores": mediante el uso de fórmulas, permite controlar el número de documentos que ha generado dicha serie por cada ejercicio, permitiendo empezar desde desde contador=1 o continuando la numeración del ejercicio anterior. Para comenzar un nuevo ejercicio manteniendo la numeración del anterior, al crear el nuevo contador se ha de indicar el mismo número del último documento.

<figure><img src="../../.gitbook/assets/image (628).png" alt="" width="563"><figcaption></figcaption></figure>

**Pestaña "Avanzado":** situación inicial de la serie al configurarse - consulte con el personal de Winmotor para más información

<figure><img src="../../.gitbook/assets/image (629).png" alt="" width="563"><figcaption></figcaption></figure>
