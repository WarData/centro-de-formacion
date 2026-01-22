---
description: Ventas
---

# Presupuestos

<figure><img src="../../.gitbook/assets/imagen (8) (1) (2) (1).png" alt=""><figcaption><p>Panel de presupuestos de ventas</p></figcaption></figure>

<mark style="color:red;">**Vídeo sobre cómo dar de alta de un presupuesto de ventas:**</mark>

{% embed url="https://youtu.be/s2j5MX-R9Dk" %}

Mediante este menú accedemos al panel de presupuestos de ventas donde podremos filtrar por fecha, ver importes y situación (pendiente de pedir, pendiente de entregar, borrador, cerrado, anulado). Los filtros de intervalo de fecha y cliente se presentan en la parte superior y en el lateral izquierdo tenemos una botonera con opciones para dar de alta un presupuesto nuevo, buscar presupuesto y listar presupuestos usando un filtro avanzado:

<figure><img src="../../.gitbook/assets/imagen (1) (1) (1) (4) (1) (2).png" alt=""><figcaption></figcaption></figure>

Y cambio de versión que permite pasar de una versión del presupuesto a otra siempre que exista alguna versión creada usando el botón ![](<../../.gitbook/assets/imagen (4) (1) (5).png>) dentro de un presupuesto. Todas las versiones quedarán registradas en la pestaña "Versiones" del presupuesto.

**1 - F1 Nuevo Presupuesto**

Permite dar de alta a un nuevo presupuesto de venta de manera directa rellenando el siguiente formulario:

<figure><img src="../../.gitbook/assets/imagen (132).png" alt=""><figcaption></figcaption></figure>

Un presupuesto está compuesto por su cabecera, donde se introducen los datos generales, como la serie, la fecha o cliente, y las líneas.

La cabecera está compuesta por los siguientes campos:

-SERIE: es un campo imprescindible de rellenar, y de él depende la presentación o contenido que tendrá el presupuesto. Entre otras cosas, en una serie de presupuesto de venta se define qué contenido tendrán las líneas que se incluyan. Todas las posibilidades de las series de documentos se detallan en la sección

-NÚMERO: todos los documentos están clasificados por su serie y un número, que siempre será por defecto el siguiente al último grabado de la misma serie. Tanto el número como la serie de un documento se podrán modificar manualmente, aunque, a menos que sea imprescindible el cambio, no es aconsejable.

-FECHA: se indica aquí la fecha de la factura. Esta fecha debe de estar dentro de los rangos definidos en parámetros.

-CLIENTE: Dispone de botones incrustados para localizar, grabar o editar el cliente seleccionado. Además de código del cliente, se presenta su razón social, su dirección de facturación y el CIF. Además de estos, bajo el CIF se presentará un campo con las notas de facturación del cliente si tuviera.

-CENTRO: este campo solo será visible por aquellas aplicaciones en las que se trabaje con más de un centro de trabajo y así se haya indicado en parámetros. Se utiliza para indicar el centro de trabajo para el que se hace el presupuesto. Este campo, se rellena automáticamente y solo será manipulable por aquellos usuarios autorizados.

-TIPO DE PAGO, VENCIMIENTOS e IMPORTES: un presupuesto de venta podrá tener distintos tipos de pago diferentes.

-TIPO DE IVA: este campo tomará por defecto el tipo de IVA definido en la ficha del cliente seleccionado. Se podrá modificar manualmente. Los diferentes tipos de IVA y de exentos, se explican en la sección

_PESTAÑERO_

* LÍNEAS: se presentará una rejilla con las líneas de artículos y/o servicios con su referencia, descripción, unidades, importe unitario, descuento  parcial.
* ESTADíSTICA: presenta una rejilla similar a líneas, pero añadiendo los campos costo, beneficio y % de beneficio. Además, añade botones en la parte inferior para aumentar el % de beneficio sobre el mostrado en la línea seleccionada y para modificar el incremento sobre el costo mostrado.
* TOTALES: muestra una tabla con las bases, % IVA, impuesto de IVA y parcial de cada tipo de IVA junto a la totalización del presupuesto

<figure><img src="../../.gitbook/assets/imagen (146).png" alt=""><figcaption></figcaption></figure>

* VERSIONES: Si se usa el botón inferior ![](<../../.gitbook/assets/imagen (144).png>) se darán de alta sucesivas versiones que se presentarán en esta pestaña a fin de trabajar con la versión seleccionada por el cliente.
* OBSERVACIONES: permite grabar texto para el cliente y observaciones internas que sólo se reflejarán en el documento dado de alta
* ARCHIVOS: [véase "Archivos"](../maestros/articulos/ficha-del-articulo/archivos.md)
* SEGUIMIENTOS: En las fichas de los documentos como presupuestos, facturas, albaranes...disponemos de la pestaña "Seguimientos" donde podemos añadir directamente asuntos tanto a nuestra agenda como a la de otros usuarios con el documento embebido desde el que se genera dicho asunto, pudiendo añadir fecha, avisos, y cualquier información que queramos. Este seguimiento quedará registrado en el documento de origen y en la agenda o agendas de los usuarios destinatarios del asunto
* EMAIL: muestra las pestañas enviados y no enviados para controlar los envíos por email del presupuesto
* ACCIONES: rejilla que indica las acciones realizadas por un usuario y cuando las realizó (similar a un log)

**Opciones desde un presupuesto de venta**

Aceptar: si pulsamos esta opción, quedarán guardados todos los cambios que hayamos realizado sobre la ficha del presupuesto.

Confirmar presupuesto: esta acción realiza el alta de un pedido, conservándose el presupuesto, sobre el que se realizará una nueva confirmación, sirviendo de documento para las entregas con albaranes y su control y como asociación con el documento pedido de compras para asignar las recepciones de material. Realiaza la reserva de los artículos en stock permitiendo su entrega mediante albarán y realiza los pedidos al proveedor o proveedores de los artículos sin stock y que quedarán asociados al presupuesto, indicando en el panel la situación de los artículos del pedido de compras.

Anular presupuesto: con este botón, cancelará el presupuesto no eliminándolo, por lo que se podrá gestionar a modo control posteriormente.

Eliminar: elimina el presupuesto, y solo lo podrán hacer usuarios supervisores.

Nueva versión: genera una versión del presupuesto anterior guardándose el anterior en la pestaña "Versiones", siendo accesibles en cualquier momento.

Imprimir: imprime el presupuesto de venta con el modelo indicado en la serie del presupuesto.

Crear email: genera un correo electrónico con el documento adjunto en PDF. El email se podrá contolar desde la pestaña "Email"

Despiece: si la marca tiene un despiece que genera archivos de texto o csv, es posible importarlos mediante este botón al presupuesto, rellenando automáticamente las líneas.

**2 – F2 - Buscar Presupuesto**

Localizador de presupuestos de ventas a través de distintos criterios. Nos permite consultar, borrar o modificar la información de un presupuesto. Al acceder a esta opción encontraremos la siguiente pantalla:

<figure><img src="../../.gitbook/assets/imagen (137).png" alt=""><figcaption></figcaption></figure>

Criterios de búsqueda:

<figure><img src="../../.gitbook/assets/imagen (147).png" alt=""><figcaption></figcaption></figure>

**3 - F3 - Listado:** muestra un listado en función de los filtros aplicados en este formulario:

<figure><img src="../../.gitbook/assets/imagen (150).png" alt=""><figcaption></figcaption></figure>

**4.- F4 - Cambiar versión:** permite moverse entre versiones desde el panel principal del menú sin necesidad de acceder al presupuesto y pestaña "Versiones".
