# Intervenciones



![](../../.gitbook/assets/image%20%28307%29.png)

En el menú distinguimos 3 partes:

-          La primera es un texto de edición donde leeremos el código de barras. Si no disponemos de código de barras, podremos teclear a través de teclado la información que vemos en el código de barras de la incidencia de la orden, el carné de operario, o el código de operación de taller.

-          La segunda es un campo de edición no manipulable por el usuario, donde veremos el actual operario logueado, o en su defecto un texto indicando que no hay ningún operario logueado.

-          La tercera es una rejilla donde veremos todos los tajos o intervenciones abiertas en este momento \(podremos ver en qué está trabajando cada operario\).

Grabación de intervención.

                En la lectura de carné, tenemos que distinguir 3 tipos de código a leer:

-          Código de logueo en aplicación: Para logar el operario en la aplicación, leeremos el carné de operario previamente impreso.

-          Código de incidencia de OR: Para empezar en un nuevo trabajo, el operario pasa por el lector de códigos de barra su carnet e inmediatamente después, pasa el código de barras impreso de la intervención de la orden de reparación que va a ejecutar. Para finalizar su trabajo, el operario puede volver a pasar su carnet o la orden de reparación y se interpreta el fin del trabajo en curso.

Es importante recordar que podremos tener más de una intervención en una sola orden, de modo que habrá que tener claro en cuál de las incidencias de la OR vamos a trabajar.

-          Código de operación especial: son aquellas que no son órdenes de reparación propiamente dichas pero son trabajos que hay que realizar, se imprimen por ello a parte \(en su opción\) y sirven para identificar la tarea en la que se halla ocupado un determinado trabajador.

Como ejemplos podemos poner por ejemplo limpieza del taller, ordenación de herramientas, parada para desayunar, etc.

Un punto muy a tener en cuenta es que si un operario está logueado en ese momento \(aparece su nombre en el panel de intervenciones\), no deberá volver a loguearse para abrir una intervención en una OR o una operación especial, de modo que un operario solo debe loguearse cuando no esté su nombre escrito en el panel.

