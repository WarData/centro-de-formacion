---
description: Configuración
---

# Almacenes

**Objetivo**

Configurar el tratamiento de almacenes en toda la aplicación

**Gestión**

· **Niveles de configuración de menor a mayor prioridad**

o Por usuario

o Por perfil de usuario

o Por empresa

o Por centro (solo aplicaciones multicentro)

o Por serie

En la grabación de documentos, el orden de prioridad es de abajo arriba. Es decir, primero se analiza si la serie tiene almacén, si no, el centro, si no la empresa, si no el perfil del usuario y por último el almacén del usuario

· **Asignación de almacenes**

o Cada almacén se podrá asignar a una sola empresa o centro. Esto se hace desde la ficha del almacén

o A mayores, se podrá seleccionar en cada almacén relaciones con series de documentos. De esta forma asignamos a cada serie que almacén por defecto tiene.

o Y por último, también podremos crear relaciones en cada almacén con un usuario concreto o un perfil de usuario.

· **Otra configuración de tener en cuenta**

o Parámetro “Control de almacenes por líneas de documentos” en centro o empresa: marcando este check, se puede decidir si en la grabación de líneas de documentos, se pueden usar sub-almacenes. Por ejemplo, en una distribución donde existan los almacenes…

P (almacén principal) // P-N (nave) // P-E (exposición)

o …si el documento tiene por defecto el almacén P, se podrá elegir en la línea cualquiera de sus dos SUB-almacenes.

· **Funcionamiento**

**PARA PROGRAMADORES**

o Al arrancar la aplicación, en la variable ALM X DEF MEM se guarda el almacén por defecto con los siguientes criterios (el orden de prioridad es de arriba abajo, es decir, si se cumple lo de abajo prevalece sobre lo de arriba)

* Almacén asignado al usuario, si lo tiene (este es el que prevalece sobre los siguientes).
* Si no, el almacén asignado al perfil
* Si no, si la distribución es multicentro, el almacén asignado al centro
* Y si no, el almacén asignado a la empresa.

o En documentos (todos, no hay excepción, incluso los que no son de “stock”)

* El almacén asociado a la serie, si lo hay
* Si no, el almacén guardado en el arranque (variable).
* Si no, si la distribución es multicentro, el almacén asignado al centro del documento.
* Si no, el almacén asignado a la empresa definida en parámetros

o En líneas de documentos

* Albaranes de compra

· Si se pueden seleccionar sub-almacenes, parámetro marcado en centro o empresa, se permite seleccionar alguno de los almacenes donde ha llegado a estar el artículo. Si no ha estado en ningún almacén, te da a elegir de entre todos los sub-almacenes disponibles. Se permite cambiar en el formulario de modificación

· Si no, directamente coge el de la cabecera.

* Albaranes de venta

· Idéntico a compras, pero siempre buscando almacenes con disponibilidad de stock del articulo seleccionado.

· No se puede modificar el almacén ni en el formulario de modificación ni en el de alta.
