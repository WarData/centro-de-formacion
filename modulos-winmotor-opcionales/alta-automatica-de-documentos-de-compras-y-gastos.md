---
description: (Importación de compras)
---

# Alta automática de documentos de compras y gastos

Leyendo facturas o albaranes en PDF mediante OCR y plantillas:

Este sistema lee un PDF aportado por el proveedor con el albarán o factura del material recepcionado o servicios facturados y crea las líneas del albarán en Winmotor.

Para que esto funcione, en cada proveedor se podrán definir distintas plantillas para la importación de documentos:

<figure><img src="../.gitbook/assets/imagen (257).png" alt=""><figcaption></figcaption></figure>

En cada plantilla se define la posición de cada dato a leer, así como el detalle de líneas. De momento, los técnicos de Winmotor serán los únicos encargados de rellenar dichas plantillas a partir de los PDF que se les aporte por cada proveedor.

Al crear un nuevo albarán de un proveedor con plantillas definidas, aparecerá el botón Importar PDF en la parte inferior del formulario:

<figure><img src="../.gitbook/assets/imagen (258).png" alt=""><figcaption></figcaption></figure>

Cuando pulsemos nos aparecerá un formulario donde veremos los siguientes datos:

<figure><img src="../.gitbook/assets/imagen (259).png" alt=""><figcaption></figcaption></figure>

·         **Modelo OCR**: plantilla del PDF a importar, por defecto cogerá la primera y podremos cambiarla en caso de que haya más de una.

·         **Archivo a subir**: seleccionaremos el archivo a importar. Podremos pulsar en la carpeta para seleccionar del PC cualquier archivo PDF.

·         **Engine**: por defecto será siempre el 2. En caso de que haya que cambiarlo Winmotor informará. <mark style="color:red;">Recomendamos no tocar este parámetro.</mark>

·         **Botón SUBIR**: pulsaremos este botón para que actúe el OCR y lea el archivo para importar los datos. NO CREA LAS LÍNEAS DE ALBARÁN, solo crea las líneas en esta pantalla de forma provisional (se puede cancelar el proceso).

·         Una vez pulsado el botón se rellenarán todos los datos configurados. Todos ellos se podrán editar.

o   Referencia

o   Fecha origen

o   Líneas

* Se podrán crear nuevas líneas manualmente, editar y borrar
* Si alguno de los artículos no existe en Winmotor se buscará en la tabla de artículos tarifa. Y si aquí tampoco existirán se creará automáticamente

·         **Botón IMPORTAR**: este botón si crea ya las líneas en el albarán según la pantalla anterior. Una vez importadas faltaría confirmar el albarán y ejecutará los repartos correspondientes de pedidos.
