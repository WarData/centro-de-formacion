# Control Presencial

Objetivo

Se gestiona en este panel las entradas y salidas del personal de la empresa a su puesto de trabajo. El control se realiza mediante la lectura del carné de cada trabajador en un panel (panel de intervenciones).

Funcionamiento

**IMPRESIÓN DEL CARNÉ**

Lo primero que hay que realizar, es la impresión del carné de cada trabajador. Lo podemos hacer desde la ficha de cada usuario, en cualquiera de los formularios disponibles:

* Barra opciones / opciones / mi configuración
* Formulario de entidad (botón en el formulario principal si estamos en un usuario, botón en la pestaña operario si estamos en un operario)
* Formulario de edición de entidad en listado de entidades del panel de control presencial

**LECTURA DE USUARIO ENTRADA / SALIDA**

* **Lector de códigos de barras**

Instalar y configurar un lector de códigos de barras para leer en el panel los carnés de los trabajadores.

* **Lector de huellas dactilares** (Módulo opcional)

Mediante el uso de lectores marca ZKTeco el sistema incorporará las huellas de los usuarios a la base de datos para el control de entradas y salidas. Actualización huella dactilar:

En noviembre de 2023, la **Agencia Española de Protección de Datos (AEPD)** ha publicado la [Guía sobre la utilización de datos biométricos para el control de presencia y acceso](https://www.aepd.es/documento/guia-control-presencia-biometrico-nov-2023.pdf), en la cual establece que las personas empleadoras deben utilizar otros **sistemas de fichaje que no almacenen ni traten con datos biométricos** de las personas empleadas. Por lo tanto, ha dejado de considerarse legal fichar con huella dactilar y, en general, empleando un sistema de fichaje biométrico.

[Véase "Reconocimiento por huella dactilar"](control-presencial/reconocimiento-por-huella-dactilar.md)

* ID / Pin: corresponde con el código de entidad de la ficha del usuario y funciona en el panel con huella, ID y código de barras:

<figure><img src="../../.gitbook/assets/imagen (4) (1).png" alt=""><figcaption></figcaption></figure>

**PANEL**

A continuación hay que crear y configurar un usuario para acceder exclusivamente a este panel. Esta configuración se realiza en el gestor del servidor (Winmotor le ayudará con este punto). En aplicaciones multicentro, habrá que crear un usuario por centro.

Este panel podrá estar abierto en el dispositivo que más nos interese (pc sobremesa, portátil, tabletas) y en los sistemas operativos compatibles (Windows, Linux, Mac, iOS, Android)

En el panel distinguimos 4 partes:

\- La primera es un texto de edición donde leeremos el código de barras. Si no disponemos de código de barras, podremos teclear a través de teclado la información que vemos en el código de barras del carné del trabajador

\- La segunda es un campo de edición no manipulable por el usuario, donde veremos el actual trabajador logueado, o en su defecto un texto indicando que no hay ningún logueado.

\- La tercera es una rejilla donde veremos todas las picadas del día en curso realizadas por los trabajadores, ordenadas de más reciente (arriba) a más antigua (abajo). A la derecha de esta rejilla, se verá los trabajadores que están “ahora” con la jornada laborar abierta.

* Botonera para introducir la IP / pin

<figure><img src="../../.gitbook/assets/imagen (284).png" alt=""><figcaption></figcaption></figure>

Un trabajador solo tendrá que pasar su carné cuando entre en su puesto de trabajo, y pasar de nuevo su carné cuando se vaya:

![](<../../.gitbook/assets/image (22).png>)

El panel será distinto si lo abre un usuario supervisor. En el podremos ver opciones para sacar listados, crear un nuevo trabajador o listar todos los ya creados

![](<../../.gitbook/assets/image (23).png>)

Listados

La opción listado nos presenta en pantalla los movimientos registrados en el intervalo definido en el filtro. Sobre la lista presentada, se podrán sacar tantos informes como estén configurados, como base los siguientes

· Listado de movimientos: nos presenta los movimientos en pantalla, agrupados por fecha de cada trabajador

· Listado de horas: nos presenta la totalización de horas de presencia de cada trabajador
