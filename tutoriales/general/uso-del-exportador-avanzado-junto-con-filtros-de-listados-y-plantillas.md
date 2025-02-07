---
description: Importar y guardar plantillas al final del documento de ayuda
---

# Uso del exportador avanzado junto con filtros de listados y plantillas

En este tutorial queremos explicaros el uso general del Exportador Avanzado para la obtención de listados muy concretos. Pondremos un ejemplo de uso para obtener un listado de clientes con fecha de alta desde el 1 de febrero de 2020 hasta el 13 de octubre de 2022, nombre, números de contacto y correos electrónicos.

Empezaremos obteniendo un listado filtrado de entidades con la fecha de alta indicada anteriormente:&#x20;

1.- Desde el panel de entidades pulsar el botón F3 Listar Entidades

<figure><img src="../../.gitbook/assets/imagen (3) (1) (3) (1).png" alt=""><figcaption></figcaption></figure>

&#x20;2.- Seleccionáis tipo de entidad “Cliente” y vais directamente a la pestaña de “Filtros avanzados”

<figure><img src="../../.gitbook/assets/imagen (6) (4) (1).png" alt=""><figcaption><p>En Filtros avanzados indicas el intervalo de fecha de alta</p></figcaption></figure>

&#x20;3.- Con el resultado en pantalla, verás que tienes todos los datos menos la fecha. Para ello, selecciona una de las líneas de cliente y pulsa el botón de la parte superior Opciones > Exportador Avanzado:

<figure><img src="../../.gitbook/assets/imagen (3) (1).png" alt=""><figcaption></figcaption></figure>

4.- Como indicamos al principio, **los campos son fecha de alta, nombre, correo y número de contacto** por lo que buscáis los códigos adecuados y vais añadiendo con doble clic. Os recomiendo que siempre que necesitéis un listado y uséis este sistema, pongáis siempre campos de más, ya que en Excel es sencillo eliminar una columna entera quedando lo que realmente necesitáis. La fórmula con todos los datos extendidos, que podéis pegar donde señalo abajo es fecha de alta, nombre y datos de contacto (móviles, fijos y otros más email 1, 2, 3 y 4) > {"table\_id":"dat\_winmotor/W7\_ENT","table\_name":"Entidades","fields":\[{"id":"ALT\_FEC","name":"Fecha de alta","type":"7","objectType":"-1","guid":"8b6e31f9-722b-4ade-ac32-15d3eb703baf","tableId":"dat\_winmotor/W7\_ENT","fieldNumber":"49"},{"id":"NAME","name":"Nombre Comercial","type":"0","objectType":"-1","guid":"f6f1869b-bc4d-4b46-aaac-0ebea54d82b3","tableId":"dat\_winmotor/W7\_ENT","fieldNumber":"1"},{"id":"TLF\_FIJO","name":"Teléfono fijo","type":"0","objectType":"-1","guid":"824339e0-6001-4984-a3b8-174193059879","tableId":"dat\_winmotor/W7\_ENT","fieldNumber":"10"},{"id":"TLF\_MOV","name":"Teléfono Móvil","type":"0","objectType":"-1","guid":"768d4718-09a1-4241-8451-44687acccd50","tableId":"dat\_winmotor/W7\_ENT","fieldNumber":"12"},{"id":"TLF\_OTRO","name":"Teléfono otro","type":"0","objectType":"-1","guid":"98d05c2f-2ff5-4cba-b15e-d28d5115281a","tableId":"dat\_winmotor/W7\_ENT","fieldNumber":"14"},{"id":"EM1","name":"Email 1","type":"0","objectType":"-1","guid":"3c24fa0a-31d0-4bc8-8bf2-ffb4e33e7c24","tableId":"dat\_winmotor/W7\_ENT","fieldNumber":"20"},{"id":"EM2","name":"Email 2","type":"0","objectType":"-1","guid":"e7e6f8ac-0b2f-4fef-b312-25b9be2063b8","tableId":"dat\_winmotor/W7\_ENT","fieldNumber":"22"},{"id":"EM3","name":"Email 3","type":"0","objectType":"-1","guid":"6f223899-9d27-44b5-a5fa-5b7eec0ffc4d","tableId":"dat\_winmotor/W7\_ENT","fieldNumber":"24"},{"id":"EM4","name":"Email 4","type":"0","objectType":"-1","guid":"0f562582-9e43-4c8b-8934-2d76cb4c9295","tableId":"dat\_winmotor/W7\_ENT","fieldNumber":"26"}]}

<figure><img src="../../.gitbook/assets/imagen (5).png" alt=""><figcaption></figcaption></figure>

5.- Al pulsar en el botón inferior derecha “Exportar”, obtendréis el Excel con todos los campos. Si alguno no lo necesitáis, pulsáis botón derecho encima de la letra de la columna y “Eliminar”

6.- Es posible guardar la plantilla generada donde indica la flecha de la derecha pulsando en el botón "Guardar plantilla":

<figure><img src="../../.gitbook/assets/imagen (1) (1).png" alt=""><figcaption></figcaption></figure>

Se añade un nombre a la plantilla (hay que tener en cuenta que una misma plantilla podría usarse en diferentes paneles o rejillas) y se acepta para guardar

Para usar las plantillas guardadas pulsamos en "Importar plantilla" mostrándonos el listado disponible generado desde cualquier tabla / rejilla, seleccionar y añade todos los campos a añadir al archivo Excel (permite editar las plantillas pulsando en el botón "Editar" indicado en la siguiente imagen):

<figure><img src="../../.gitbook/assets/imagen (2) (1).png" alt=""><figcaption></figcaption></figure>

\*\*\* IMPORTANTE: esta información es válida para cualquier rejilla de datos de Winmotor, por lo que podéis obtener listados personalizados tras filtrar lo necesario de forma sencilla.
