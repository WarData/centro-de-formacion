# Temparios

Son servicios especiales que incluyen coste y venta de tiempos de mano de obra, productos y/o temparios adicionales y líneas de texto. Una revisión de un vehículo incluiría filtros, aceites, tiempo de mano de obra y una serie de líneas de texto, el trabajo en conjunto sería un tempario.

El conjunto forma una referencia que puede ser añadida a una línea de OR o a una línea de imputación, formando una única línea por el valor de venta del tempario en el primer caso y desglosando todas las líneas de artículos, temparios y texto que lo componen en el segundo.

En la opción obtenemos un panel que muestra varias funciones y una rejilla con las referencias de los temparios, la denominación, modelo (si uso) y sección de taller , unidad de tiempo usada y el P.V.P.:

<figure><img src="../../../.gitbook/assets/imagen (7) (5).png" alt=""><figcaption></figcaption></figure>

Opciones del panel:

A) **F1 - Nuevo**: alta de un nuevo tempario que muestra el siguiente formulario:

<figure><img src="../../../.gitbook/assets/imagen (12).png" alt=""><figcaption></figcaption></figure>

* Referencia: campo con el objetivo de facilitar la localización / grabación de la línea en las ORs mediante una abreviatura o de la denominación del tempario
* Denominación: nombre que identifica el trabajo a realizar
* Modelo de taller: sin uso
* Sección de taller: permite organizar el taller por secciones como soldadura, lavado, mecánica, chapa, etc. permitiendo identificar fácilmente el destino del tempario
* Observaciones: campo libre para cualquier aclaración sobre el tempario

<mark style="color:yellow;">Referente a tiempo y mano de obra</mark>

* Medida de tiempo: permite definir el precio de costo y venta mediante hora o décimas de hora (la décima de hora se establece como dividir 1 hora en 10 partes)
* Precio Costo: relativo el valor de la unidad de mano de obra **para el taller** sobre ese tempario concreto
* Precio Venta: relativo al valor de la unidad de mano de obra **para el cliente** sobre ese tempario concreto
* Tiempo: unidades en la medida de tiempo escogida en "Medida de tiempo"
* Precio Vta. Total (Sin imp.): valor del precio de venta multiplicado por el campo "Tiempo" sin aplicar impuestos
* Tipo impuesto: permite seleccionar el valor del impuesto entre los mostrados en el localizador

<figure><img src="../../../.gitbook/assets/imagen (9).png" alt=""><figcaption></figcaption></figure>

* Tiempo real concesionario: en la agenda de taller, al incorporar un tempario al alta de una cita ocupará el valor indicado en este campo en las horas de taller, no el indicado en el campo "Tiempo". Se usa para establecer un tiempo medio real entre lo estimado para el cliente y taller.

<mark style="color:yellow;">Referente a contabilidad</mark>

* Cuentas contables de compras, ventas y abonos: permite configurar las cuentas auxiliares de cada tempario si el nivel contable es de servicios

<mark style="color:yellow;">Pestañas</mark>

* Trabajo a realizar: indica los puntos a realizar y se identifica con el impreso de taller
* Texto para el cliente: indica los trabajos realizados y se identifica con el impreso de cliente
* Productos: añade artículos indicando las unidades a añadir al tempario

<figure><img src="../../../.gitbook/assets/imagen (3) (3).png" alt=""><figcaption></figcaption></figure>

* Temparios: añade temparios existentes - no requiere indicar unidades al ser trabajos (servicios)

<figure><img src="../../../.gitbook/assets/imagen (8) (5).png" alt=""><figcaption></figcaption></figure>

* Auditoría: muestra la fecha y hora de creación y modificación así como el usuario que realizó cada operación y el log de cada modificación o borrado del tempario

<figure><img src="../../../.gitbook/assets/imagen (5) (3).png" alt=""><figcaption></figcaption></figure>

<mark style="color:yellow;">Botonera inferior</mark>

<figure><img src="../../../.gitbook/assets/imagen (14).png" alt=""><figcaption></figcaption></figure>

* Aceptar: graba o activa las modificaciones realizadas en el tempario
* Cancelar: cierra y cancela las modificaciones realizadas en el tempario
* Eliminar: borra el tempario (mientras no exista histórico del mismo)
* Copiar tempario: permite duplicar el tempario mostrando un formulario de copia con los datos del tempario a copiar y la referencia y denominación del nuevo con el contenido anterior, permitiendo cambiar la referencia, la denominación y añadir o quitar productos, tiempo y/o temparios. El objetivo es facilitar el alta de temparios similares:

<figure><img src="../../../.gitbook/assets/imagen (15).png" alt=""><figcaption></figcaption></figure>

* Desactivar: no elimina el tempario, únicamente evita ser mostrado en localizadores así como ser incorporado a documentos.

B) **F2 - Buscar**:

Muestra un formulario de búsqueda con diferentes localizadores (ver imagen) y una rejilla con el filtrado obtenido de temparios:

<figure><img src="../../../.gitbook/assets/imagen (11) (1).png" alt=""><figcaption></figcaption></figure>

C) **F3 - Listar**:

Muestra una rejilla con el listado de todos los temparios y su referencia, denominación, modelo y sección de taller, unidades de tiempo y P.V.P.:

<figure><img src="../../../.gitbook/assets/imagen (4) (5).png" alt=""><figcaption></figcaption></figure>

D) **F4 - Copiar tempario**:

Permite mostrar el formulario de copia del tempario seleccionado en la rejilla del panel de temparios, evitando la necesidad de acceder a la ficha del tempario a copiar. Mostraría el mismo formulario de copia:

<figure><img src="../../../.gitbook/assets/imagen (1) (5).png" alt=""><figcaption></figcaption></figure>

<mark style="color:yellow;">\*\*\* Los temparios son fundamentales para obtener la máxima agilidad, imagen cara al cliente y rendiemiento en la agenda de taller.</mark> <mark style="color:orange;"></mark> [<mark style="color:orange;">Recomendamos ver el manual "Agenda de taller"</mark>](agenda-de-taller/)<mark style="color:orange;"></mark>
