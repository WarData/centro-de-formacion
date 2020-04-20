---
description: Módulo opcional Winmotor V7
---

# SII - Suministro Inmediato de Información

**Parametrización** 

La puesta en marcha del sistema SII implica la configuración y parametrización de una serie de datos, el principal es el certificado digital de la empresa proporcionado por la AEAT. 

Dado que la generación del certificado y la clave privada desde el archivo .PEM que proporciona la AEAT es bastante complejo, en Winmotor haremos este proceso a partir del certificado que nos envíen y lo dejaremos registrado en los parámetros.

![\* Figura 1 &#x2013; Par&#xE1;metros](../../../.gitbook/assets/image%20%2862%29.png)

Al igual que el certificado y la clave, también dejaremos registrado toda la parametrización para la conexión con los servidores de la agencia tributaria, tanto para el envío de facturas emitidas y recibidas como para la consulta de entidades.

 La parametrización de los días de envío es en la que interviene el responsable de la empresa y se explica a continuación.

**Operativa**

* Alta de clientes, proveedores y acreedores

**a.-** El SII exige que todo cliente, proveedor o acreedor que se identifique en cualquier factura que enviemos esté registrado en la AEAT por lo que el primer paso que hace el programa es controlar su registro en el proceso de alta. 

**b.-** En el momento del alta de uno de estos tipos de entidades la aplicación verificará con la AEAT que están registrados. Para el caso de particulares la AEAT verifica el NIF y el nombre dado que la ley de protección de datos así lo exige, pero para el caso de sociedades sólo verifica el NIF. En caso de que estemos dando de alta una sociedad y el nombre fiscal registrado en la aplicación sea distinto del que está registrado en la AEAT el programa lo modificará automáticamente.

![\* Figura 2 &#x2013; Alta de entidad](../../../.gitbook/assets/image%20%28386%29.png)

  
**c.-** El uso del botón “Verificar DNI/CIF” es opcional por si queremos consultar; el programa hará la verificación automática en el momento de aceptar el alta de la ficha.

* **Envío de facturas emitidas y recibidas**

**a.-** Simplificando la normativa del SII diremos que la AEAT exige que las facturas emitidas se envíen en un plazo máximo de cuatro días desde su expedición y las facturas recibidas cuatro días naturales desde la fecha en que se produce el registro contable de la factura.

Más información en el siguiente enlace de la Agencia Tributaria:

{% embed url="https://www.agenciatributaria.es/AEAT.internet/Inicio/Ayuda/Modelos\_\_Procedimientos\_y\_Servicios/Ayuda\_P\_G417\_\_\_\_IVA\_\_Llevanza\_de\_libros\_registro\_\_SII\_/Informacion\_general/Preguntas\_frecuentes/1\_\_Cuestiones\_generales/1\_12\_\_\_Cuando\_hay\_que\_enviar\_los\_registros\_de\_facturacion\_a\_la\_AEAT\_\_.shtml" %}

**b.-** En la parametrización definiremos por tanto el número de días después de su creación que queremos que se cuenten para el envío de las facturas y lo mismo para las recibidas 

* Winmotor enviará todas las noches mediante una tarea programada todas las facturas no enviadas cuya antigüedad llegue a los días definidos según su tipo en la parametrización. Por cada envío se crea un registro indicando la fecha y hora del envío

![\* Figura 3 &#x2013; Consulta de env&#xED;o  ](../../../.gitbook/assets/image%20%28233%29.png)

**a.-** Cada uno de estos envíos queda registrado con un “Código seguro de verificación” que genera la AEAT y que facilita su consulta en su página en caso de necesitar hacer alguna comprobación.

**Verificación y corrección de errores**

Winmotor después de cada envío generará un correo electrónico a los destinatarios definidos en la parametrización \(último campo de la figura 1\) indicando el resultado de los envíos de esa noche.

Todo el sistema de consultas y listados del SII está en un menú especial al que sólo tiene acceso un usuario supervisor. La ruta es “Configuración/Opciones especiales/SII”. En este menú encontraremos opciones para listar tanto facturas emitidas como recibidas, así como para listar y consultar registros de envíos y sus detalles.

Al consultar una factura desde este menú veremos un botón especial donde se muestra el estado de sus envíos al SII.

![\* Figura 4 &#x2013; Consulta de factura desde SII](../../../.gitbook/assets/image%20%28175%29.png)

Una factura con errores se puede volver a enviar al SII desde este listado seleccionándola y utilizando el botón “SII – Envío de facturas”

![\* Figura 5 &#x2013; Listado de facturas desde el men&#xFA; SII](../../../.gitbook/assets/image%20%28360%29.png)

Realmente hay que entender que estas opciones no son de uso normal sino para circunstancias especiales en las que ha habido algún problema con alguna factura por lo que en estos casos siempre se tendrá ayuda de personal de Winmotor, al menos en el período de puesta en marcha del sistema.

**Detalles importantes a tener en cuenta en la operativa SII**

**a.-** Tipos de facturas

Winmotor calculará automáticamente uno de estos tipos de factura según sus datos:

| **Código** | **Nombre** |
| :--- | :--- |
| F1 | Factura |
| F2 | Factura simplificada |
| F3 | Factura emitida en sustitución de facturas simplificadas |
| F4 | Asiento resumen de facturas |
| F5 | DUA |
| F6 | Documento contable |
| R1 | Factura Rectificativa \(Error fundado en derecho y Art. 80 |
| R2 | Factura Rectificativa \(Art. 80.3\) |
| R3 | Factura Rectificativa \(Art. 80.4\) |
| R4 | Factura Rectificativa \(Resto\) |
| R5 | Factura Rectificativa en facturas simplificadas |

**b.-** Facturas simplificadas

El sistema identificará como factura simplificada aquella cuyo cliente esté marcado como “Entidad genérica”. Según la AEAT una factura a un cliente de este tipo no puede superar un importe de 400€ por lo que el parámetro correspondiente a este valor \(véase figura 1 arriba a la derecha\) debe estar relleno.

Estando relleno no se permitirá crear una factura a un cliente genérico con un importe superior a este.

**c.-** Facturas intracomunitarias

A nivel del SII son facturas tipo “F1 – Factura” pero su régimen de IVA la identificará como intracomunitaria y el cliente lógicamente será de un país fuera de España e intracomunitario. Es importante tener en cuenta que la AEAT rechazará una factura con el tipo de IVA “Régimen Intracomunitario” que no cumpla estos requisitos. 

Por otro lado, para este tipo de facturas es fundamental tener en cuenta que la lista de países intracomunitarios debe estar actualizada y que el código del país identificado debe ser el correcto. Inicialmente Winmotor actualizará la base de datos de países correcta.

