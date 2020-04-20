# Rejillas - Funciones Especiales

## ¿Qué es una rejilla?

 La rejilla es un objeto que sirve para presentar listas de registros de las tablas. Está compuesta por una serie de celdas distribuidas en forma de filas y columnas. Una fila se corresponde con un registro de una tabla y una columna con un campo de la tabla. Una celda, por tanto, permitirá mostrar un dato concreto de un registro concreto de la tabla.

![](../.gitbook/assets/image%20%28446%29.png)

## ¿Qué puedo hacer en las rejillas?

En cualquier rejilla de Velneo vClient es posible añadir, modificar y/o borrar registros de una tabla. Las opciones de ficha están contenidas en el menú Ficha \(botón derecho encima de un campo\). Veamos algunas de esas opciones:

### Invertir <a id="selecci&#xF3;n-m&#xFA;ltiple-de-registros-multiselecci&#xF3;n"></a>

Invierte el orden de los registros de la lista usando para ello el campo por el que ésta se encontrase ordenada.

Ejemplo: si se dispara una búsqueda por el índice nombre, el resultado será la lista ordenada alfabéticamente en orden ascendente. Si se invierte la lista, ésta será reordenada alfabéticamente en orden descendente.

### [Filtros](../tutoriales/uso-de-los-nuevos-filtros-rapidos.md) <a id="selecci&#xF3;n-m&#xFA;ltiple-de-registros-multiselecci&#xF3;n"></a>

Este submenú incluye una serie de opciones para filtrar una lista, es decir, para quitar de la lista aquellos registros que no cumplan una determinada condición.

### Ordenar <a id="selecci&#xF3;n-m&#xFA;ltiple-de-registros-multiselecci&#xF3;n"></a>

Reordena los elementos de la rejilla por el campo seleccionado. Cuando se ejecuta esta opción se desplegará una ventana con la lista de campos de la tabla asociada a la rejilla.

Podremos seleccionar un campo tanto de la propia tabla como de sus maestros.

La ordenación se hará por defecto en orden ascendente. Si queremos hacerla en orden descendente activaremos la opción Invertir lista.

Una vez seleccionado el campo, pulsar el botón _aceptar_ para reordenar la lista o el botón _cancelar_ para cancelar la ordenación.

### Campos duplicados... <a id="selecci&#xF3;n-m&#xFA;ltiple-de-registros-multiselecci&#xF3;n"></a>

Esta opción crea un nueva lista con los registros de la rejilla en curso que posean el contenido de un campo duplicado. Este campo ha de ser seleccionado en la ventana que aparece al ejecutar esta opción.

Es útil para la localización de códigos o claves duplicadas en una tabla de datos.

### Copiar <a id="selecci&#xF3;n-m&#xFA;ltiple-de-registros-multiselecci&#xF3;n"></a>

Permite copiar el contenido de la rejilla al portapapeles y pegarlo en hojas de cálculo, editores de texto, etc...

Se incluirán todos los campos alfabéticos, numéricos, fórmulas, etc..., excepto campos objeto binario e imágenes, incluyendo además la cabecera en la información que se copia.

En textos que contengan Intro o tabulador, el texto se copiará con el delimitador "". El formato numérico aplicado será el que en ese momento sea visible.

### Selección múltiple de registros \(multiselección\) <a id="selecci&#xF3;n-m&#xFA;ltiple-de-registros-multiselecci&#xF3;n"></a>

Es posible seleccionar más de un registro en una rejilla para luego realzar alguna acción con ellos. Podremos hacer la selección, bien con el ratón, o bien a través del teclado.

![](../.gitbook/assets/image%20%28149%29.png)

Si la rejilla tiene a la izquierda la columna de multiselección, haciendo clic sobre un ítem, éste quedará seleccionado. Si volvemos a hacer clic sobre él, se quitará de la selección.

Si hacemos clic sobre la cabecera de la columna de multiselección, se seleccionarán todos los registros. Si volvemos a hacer clic, se quitarán todos de la selección.

Es posible también seleccionar registros haciendo clic sobre cualquier celda de la rejilla. Al hacer un clic quedará seleccionado el registro entero.

Si hacemos clic sobre otra línea, se quitará la selección del ítem o ítems que hubiese seleccionados y quedará seleccionado solamente éste.

Si queremos seleccionar un bloque continuo de registros lo que haremos será poner situar el foco en el primero de ellos y, con la tecla **Shift** pulsada, con las teclas de cursor arriba y abajo avanzar hasta el último registro que se quiere seleccionar.

Lo anterior también podemos hacerlo si hacemos clic con el ratón sobre el primer ítem a seleccionar, pulsamos la techa **Shift** y, sin soltarla, hacemos clic con el ratón sobre el último ítem a seleccionar.

Si queremos seleccionar registros alternos, entonces lo haremos manteniendo pulsada la tecla **Control** y haciendo clic con el ratón sobre cada registro a seleccionar.

Si tenemos seleccionado uno o varios registros y queremos seleccionar otro bloque, pulsar la tecla **Control** y la techa **Shift** de forma simultanea y, sin soltarlas, hacer clic sobre el primer ítem a seleccionar y luego sobre el último. De este modo, el bloque seleccionado se añadirá a la selección.

