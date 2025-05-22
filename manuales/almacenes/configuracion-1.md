# Almacenes

Los almacenes en Winmotor sirven para clasificar o ubicar el stock de cada artículo. Cada almacén se corresponde con una ubicación física. Podrá ser por ejemplo una nave, o dentro de esta nave una calle, estantería, balda, etc.

<figure><img src="../../.gitbook/assets/image (618).png" alt=""><figcaption></figcaption></figure>

**CAMPOS**

* <mark style="color:red;">**Código**</mark>: identificador único del almacén.

Es importante que la creación de almacenes siga una estructura arbolada. El primero será el almacén principal, que representa a la empresa y cuyo identificador solo podrá tener un dígito (por ejemplo, E ). Si la empresa es multicentro, el siguiente nivel del árbol será el almacén de cada centro, cuyo identificador debe tener tres dígitos (por ejemplo, EM- ). Dentro de cada centro, o si no existen centros, se crearán almacenes por cada ubicación específica (nave, calle, estantería, etc).

{% hint style="info" %}
El identificador de cada almacén, nave, calle, estantería, etc. debe empezar por el ID del almacén al que pertenece
{% endhint %}

* A continuación un ejemplo:
  * E - Empresa
  * ES- Tienda Sevilla
  * ES-T Taller tienda Sevilla
  * ES-TC1 - Calle 1 taller tienda Sevilla
  * ES-TC1E1 - Estantería 1 calle 1 taller tienda Sevilla
  * ES-TC1E1C1 - Caja 1 estantería 1 calle 1 taller tienda Sevilla
  * ES-E Exposición tienda Sevilla
  * ...
  * EV- Tienda Valencia
  * ...
  * **No es obligatorio el desglose de cada ubicación. Podemos crear y clasificar los almacenes que nos interese.**
* <mark style="color:yellow;">Nombre:</mark> descripción del almacén
* <mark style="color:yellow;">Empresa:</mark> solo rellenable cuando grabamos el almacén raiz de la empresa ( E )
* <mark style="color:yellow;">Centro:</mark> solo rellenable cuando grabamos el almacén raiz de cada centro ( ES- )
* <mark style="color:yellow;">Restringido:</mark> si marcamos este check, el stock que haya en él no se podrá vender ni reservar. Sí se podrá ubicar material en este almacén en compras. También podremos usarlo en partes de almacén.

CONFIGURACIÓN

<mark style="color:yellow;">**Objetivo**</mark>

Configurar el tratamiento de almacenes en toda la aplicación

<mark style="color:yellow;">**Gestión**</mark>

**A) Niveles de configuración de menor a mayor prioridad**

o Por usuario

o Por perfil de usuario

o Por empresa

o Por centro (solo aplicaciones multicentro)

o Por serie

En la grabación de documentos, el orden de prioridad es de abajo arriba. Es decir, primero se analiza si la serie tiene almacén, si no, el centro, si no la empresa, si no el perfil del usuario y por último el almacén del usuario

B) **Asignación de almacenes**

o Cada almacén se podrá asignar a una sola empresa o centro. Esto se hace desde la ficha del almacén

o A mayores, se podrá seleccionar en cada almacén relaciones con series de documentos. De esta forma asignamos a cada serie que almacén por defecto tiene.

o Y por último, también podremos crear relaciones en cada almacén con un usuario concreto o un perfil de usuario.

**C) Otra configuración de tener en cuenta**

o Parámetro “Control de almacenes por líneas de documentos” en centro o empresa: marcando este check, se puede decidir si en la grabación de líneas de documentos, se pueden usar sub-almacenes. Por ejemplo, en una distribución donde existan los almacenes…

P (almacén principal) // P-N (nave) // P-E (exposición)

o …si el documento tiene por defecto el almacén P, se podrá elegir en la línea cualquiera de sus dos SUB-almacenes.

<mark style="color:yellow;">ALMACENES RESTRINGIDOS:</mark> Esto hará que el stock que exista en este almacén no pueda ser reservado ni usado para vender. En los listados de stock, se podrá incluir o quitar los almacenes bloqueados
