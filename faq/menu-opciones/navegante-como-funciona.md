---
description: Función del menú "Opciones"
---

# Navegante - ¿Cómo funciona?

Como su nombre indica, el Navegante permite navegar por la información contenida en las distintas tablas de datos del proyecto de datos ejecutada a través los enlaces declarados y usando los objetos visuales disponibles. Partiendo de una rejilla origen, se puede ir obteniendo información asociada de forma simple y rápida. Los resultados de las operaciones realizadas con el Navegante son visualizados en el objeto de lista público que seleccionemos.

Los navegantes se nutren de forma automática de los objetos disponibles en el proyecto. Cuando usamos alguna de las opciones de navegación, a maestro o plurales, además de presentar las tablas por las que podemos navegar, presenta los objetos correspondientes a las tablas que pueden usarse.

Los objetos que un navegante puede usar han de estar públicos. Si un objeto tiene el estilo Privado activo, el navegante no hará uso de estos objetos. Por tanto, si queremos que el usuario no pueda navegar a una tabla concreta, basta que no tenga objetos de lista disponibles correspondientes a esa tabla, es decir, que no tenga ningún objeto público, y ya no podrá navegar.

El Navegante puede utilizarse múltiples veces sin ninguna limitación. Puede combinar varias listas y utilizar de nuevo el Navegante con los resultados obtenidos, y así sucesivamente.

Las opciones disponibles son:

**Maestros…**

Esta opción nos permite ver los registros de una tabla maestra que están siendo apuntados por los registros de la lista actual. Al ejecutarla se presentará una ventana donde solamente se mostrarán los campos de la tabla que están enlazados a otras tablas y los objetos de lista públicos que podemos usar para ver dichos registros:

![](../../.gitbook/assets/image%20%2889%29.png)

Seleccionar el campo y pulsar el botón _aceptar_ para continuar o pulsar el botón _cancelar_ para cancelar la navegación a maestros. Si aceptamos el sistema abrirá una nueva pestaña en el panel de registros con los registros de la tabla maestra que están siendo apuntados por los registros de la lista de origen.

Ejemplo: desde una lista de libros podremos obtener los autores de dichos los mismos.

Este comando está optimizado de modo que se pasa la lista de registros al servidor para que la carga de sus maestros se realice en 3er plano.

**Plurales**

Esta opción nos permite ver los registros de una tabla plural de un registro de la lista actual. Para ejecutar esta opción, por tanto, es necesario que hayamos seleccionado previamente un registro de la lista. Una vez seleccionado el registro y ejecutada esta opción, si la tabla tiene más de un histórico, se presentará una ventana para seleccionar el que se desea cargar y la selección del objeto de lista público que queramos usar para ver dichos registros:

![](../../.gitbook/assets/image%20%28232%29.png)

Seleccionar el campo y pulsar el botón _aceptar_ para continuar o pulsar el botón _cancelar_ para cancelar la navegación a plurales. Si aceptamos el sistema abrirá una nueva pestaña en el panel de registros con los plurales de esa ficha.

En el caso de que la tabla tenga únicamente un plural, no se presentará el formulario para su selección sino que será abierta directamente la rejilla con los plurales de la ficha.

Esta opción puede activarse mediante la pulsación de la tecla **F4**

Ejemplo: desde una lista de clientes podremos obtener todas las facturas de uno de ellos.

Este comando está optimizado de modo que se pasa el registro al servidor para que la carga de sus plurales se realice en 3er plano, excepto en el caso de las tablas en memoria, que se hará en primer plano.

**Plurales de todos…**

Esta opción es igual que la anterior; la diferencia radica en que lo que cargará son los plurales de todos los registros de la lista actual.

De esta forma tan sencilla podemos controlar aquellas tablas a las que no queremos que el usuario final tenga acceso mediante la navegación.

Este comando está optimizado de modo que se pasa la lista de registros al servidor para que la carga de sus plurales se realice en 3er plano.

![](../../.gitbook/assets/image%20%2835%29.png)

