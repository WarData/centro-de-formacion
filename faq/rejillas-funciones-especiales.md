# Rejillas - Funciones Especiales - Rejillas avanzadas

## ¿Qué es una rejilla?

La rejilla es un objeto que sirve para presentar listas de registros de las tablas. Está compuesta por una serie de celdas distribuidas en forma de filas y columnas. Una fila se corresponde con un registro de una tabla y una columna con un campo de la tabla. Una celda, por tanto, permitirá mostrar un dato concreto de un registro concreto de la tabla.

![](<../.gitbook/assets/image (310).png>)

## ¿Qué puedo hacer en las rejillas?

En cualquier rejilla de Velneo vClient es posible añadir, modificar y/o borrar registros de una tabla. Las opciones de ficha están contenidas en el menú Ficha (botón derecho encima de un campo). Veamos algunas de esas opciones:

### Invertir <a href="#seleccion-multiple-de-registros-multiseleccion" id="seleccion-multiple-de-registros-multiseleccion"></a>

Invierte el orden de los registros de la lista usando para ello el campo por el que ésta se encontrase ordenada.

Ejemplo: si se dispara una búsqueda por el índice nombre, el resultado será la lista ordenada alfabéticamente en orden ascendente. Si se invierte la lista, ésta será reordenada alfabéticamente en orden descendente.

### [Filtros](../tutoriales/uso-de-los-nuevos-filtros-rapidos/) <a href="#seleccion-multiple-de-registros-multiseleccion" id="seleccion-multiple-de-registros-multiseleccion"></a>

Este submenú incluye una serie de opciones para filtrar una lista, es decir, para quitar de la lista aquellos registros que no cumplan una determinada condición.

### Ordenar <a href="#seleccion-multiple-de-registros-multiseleccion" id="seleccion-multiple-de-registros-multiseleccion"></a>

Reordena los elementos de la rejilla por el campo seleccionado. Cuando se ejecuta esta opción se desplegará una ventana con la lista de campos de la tabla asociada a la rejilla.

Podremos seleccionar un campo tanto de la propia tabla como de sus maestros.

La ordenación se hará por defecto en orden ascendente. Si queremos hacerla en orden descendente activaremos la opción Invertir lista.

Una vez seleccionado el campo, pulsar el botón _aceptar_ para reordenar la lista o el botón _cancelar_ para cancelar la ordenación.

### Campos duplicados... <a href="#seleccion-multiple-de-registros-multiseleccion" id="seleccion-multiple-de-registros-multiseleccion"></a>

Esta opción crea un nueva lista con los registros de la rejilla en curso que posean el contenido de un campo duplicado. Este campo ha de ser seleccionado en la ventana que aparece al ejecutar esta opción.

Es útil para la localización de códigos o claves duplicadas en una tabla de datos.

### Copiar <a href="#seleccion-multiple-de-registros-multiseleccion" id="seleccion-multiple-de-registros-multiseleccion"></a>

Permite copiar el contenido de la rejilla al portapapeles y pegarlo en hojas de cálculo, editores de texto, etc...

Se incluirán todos los campos alfabéticos, numéricos, fórmulas, etc..., excepto campos objeto binario e imágenes, incluyendo además la cabecera en la información que se copia.

En textos que contengan Intro o tabulador, el texto se copiará con el delimitador "". El formato numérico aplicado será el que en ese momento sea visible.

### Selección múltiple de registros (multiselección) <a href="#seleccion-multiple-de-registros-multiseleccion" id="seleccion-multiple-de-registros-multiseleccion"></a>

Es posible seleccionar más de un registro en una rejilla para luego realzar alguna acción con ellos. Podremos hacer la selección, bien con el ratón, o bien a través del teclado.

![](<../.gitbook/assets/image (311).png>)

Si la rejilla tiene a la izquierda la columna de multiselección, haciendo clic sobre un ítem, éste quedará seleccionado. Si volvemos a hacer clic sobre él, se quitará de la selección.

Si hacemos clic sobre la cabecera de la columna de multiselección, se seleccionarán todos los registros. Si volvemos a hacer clic, se quitarán todos de la selección.

Es posible también seleccionar registros haciendo clic sobre cualquier celda de la rejilla. Al hacer un clic quedará seleccionado el registro entero.

Si hacemos clic sobre otra línea, se quitará la selección del ítem o ítems que hubiese seleccionados y quedará seleccionado solamente éste.

Si queremos seleccionar un bloque continuo de registros lo que haremos será poner situar el foco en el primero de ellos y, con la tecla **Shift** pulsada, con las teclas de cursor arriba y abajo avanzar hasta el último registro que se quiere seleccionar.

Lo anterior también podemos hacerlo si hacemos clic con el ratón sobre el primer ítem a seleccionar, pulsamos la techa **Shift** y, sin soltarla, hacemos clic con el ratón sobre el último ítem a seleccionar.

Si queremos seleccionar registros alternos, entonces lo haremos manteniendo pulsada la tecla **Control** y haciendo clic con el ratón sobre cada registro a seleccionar.

Si tenemos seleccionado uno o varios registros y queremos seleccionar otro bloque, pulsar la tecla **Control** y la techa **Shift** de forma simultanea y, sin soltarlas, hacer clic sobre el primer ítem a seleccionar y luego sobre el último. De este modo, el bloque seleccionado se añadirá a la selección.

**REJILLAS AVANZADAS**

Existen un tipo de rejillas llamadas avanzadas que son personalizables e incluso es posible determinar por defecto esa rejilla avanzada y su configuración en cualquier panel que presente tanto una rejilla estándar como una rejilla avanzada.

La personalización incluye poder mover, quitar o añadir (dentro de las posibilidades del documento) las columnas, añadir sumatorios al final de cada columna y agrupar los datos de las columnas moviendo una de ellas a la zona de agrupación para mostrar datos unificados.

Ponemos a continuación varios ejemplos de los indicado:

Para añadir la totalización, basta con clicar con el botón secundario del ratón sobre la base de la columna entradas y seleccionar 'suma'. Lo mismo en la columna salidas:

<figure><img src="../.gitbook/assets/imagen (7) (2).png" alt=""><figcaption></figcaption></figure>

Si también quiere quitar por ejemplo las dos últimas columnas, tiene que clicar en el icono superior izquierdo de la rejilla y deseleccione las columnas que no quiera:

<figure><img src="../.gitbook/assets/imagen (123).png" alt=""><figcaption></figcaption></figure>

Para guardar esta configuración simplemente pulse sobre cualquier sitio de la rejilla con el botón secundario y pulse en opciones/guardar configuración. Verá que en estas opciones también está disponible aumentar / reducir el tamaño de letra:

<figure><img src="../.gitbook/assets/imagen (2) (2).png" alt=""><figcaption></figcaption></figure>

Para convertir un listado con rejilla estandar (un listado estadístico de las ORs por ejemplo) a un panel de rejilla avanzada simplemente hay que seleccionar una de las líneas presentadas en el panel e ir a la barra de herrmientas principal > Opciones > Lista > Generar vista con otro visor y seleccionar una de las opciones que indique "rejilla avanzada". Ponemos el ejemplo del listado estadístico de las ORs:

<figure><img src="../.gitbook/assets/imagen (1) (1).png" alt=""><figcaption></figcaption></figure>

Por defecto nos muestra una rejilla estandar:

<figure><img src="../.gitbook/assets/imagen (6) (1).png" alt=""><figcaption></figcaption></figure>

Para pasarlo a rejilla avanzada y poderlo configurar los pasos son los siguientes:

1.- Seleccionar una línea, ir a Opciones > Lista > Generar vista con otro visor y seleccionar una de las opciones que indique "rejilla avanzada":

<figure><img src="../.gitbook/assets/imagen (108) (3).png" alt=""><figcaption></figcaption></figure>

2.- En el lateral izquierda tenemos el menú de columnas, donde podremos activar o desactivarlas:

<figure><img src="../.gitbook/assets/imagen (116).png" alt=""><figcaption></figcaption></figure>

3.- Las totalizaciones podemos quitarlas o activarlas pulsando botón derecho encima de los campos de suma, además de poder indicar la cifra máxima o mínima, la media, el número de elementos que componen la suma, totalización y por último ninguno:

<figure><img src="../.gitbook/assets/imagen (107) (3).png" alt=""><figcaption></figcaption></figure>

4.- Las agrupaciones nos pueden ayudar a gestionar los datos de la forma más interesante. Su uso es tan sencillo como arrastrar la parte superior de la columna a formar la agrupación:

**Antes**

<figure><img src="../.gitbook/assets/imagen (122).png" alt=""><figcaption></figcaption></figure>

**Después (agrupando por imputación)**

<figure><img src="../.gitbook/assets/imagen (121).png" alt=""><figcaption></figcaption></figure>

**Resultado (imputación cliente)**

<figure><img src="../.gitbook/assets/imagen (117).png" alt=""><figcaption></figcaption></figure>

**Resultado (resto de imputaciones)**

<figure><img src="../.gitbook/assets/imagen (15).png" alt=""><figcaption></figcaption></figure>

Por último, una vez obtenida la configuración deseada, podemos pulsar con el botón derecho en la rejilla y guardar la configuración. Del mismo modo, podemos revertir la configuración usando el botón "Restaurar configuración":

<figure><img src="../.gitbook/assets/imagen (9).png" alt=""><figcaption></figcaption></figure>
