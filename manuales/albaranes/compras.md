# Albaranes

**ALBARANES DE COMPRAS**

Mediante esta opción, podremos grabar, modificar o consultar todos los albaranes de compras de la mercancía recibida de nuestros proveedores. Al entrar en ella, nos aparece un menú con calendario en el que se nos presentan diferentes opciones, un calendario que contendrá por defecto la fecha de hoy y se podrá modificar, y una rejilla que presentaré todos los albaranes de compras con la fecha indicada en el calendario.

![](<../../.gitbook/assets/imagen (23).png>)

**1.- NUEVO ALBARÁN**

Permite dar de alta a un nuevo albarán de compra mediante el siguiente formulario.

![](<../../.gitbook/assets/imagen (24).png>)

Al igual que los pedidos de material y los demás documentos de compra y venta, los albaranes están compuestos por su cabecera, donde se guardan todos los datos generales del albarán, y las líneas, donde se va guarda el detalle de la compra, referencia decepcionada, cantidad, importe, etc.

La cabecera de los albaranes de compras está compuesta por los siguientes campos:

* **Serie**: campo que clasifica a los albaranes por grupos y dependiendo de la configuración de la serie, el albarán tomará unos valores u otros. Por ejemplo, una serie se puede configurar para que en todos sus albaranes no se calculen los impuestos. En el botón "lupa" es posible seleccionar entre las distintas series. Véase ["Series"](../configuracion/series-de-documentos.md) para configuración y ["Perfiles"](../configuracion/opciones-especiales/permisos-de-usuario.md) para asignación automática de series a un perfil determinado.
* **Número:** todos los documentos están clasificados por su serie y un número, que siempre será por defecto el siguiente al último grabado de la misma serie. Tanto el número como la serie de un documento se podrán modificar manualmente una vez dado de alta el documento, aunque, a menos que sea imprescindible, no es aconsejable.
* **Fecha:** se indica aquí la fecha de grabación del documento. Esta fecha debe de estar dentro de los rangos definidos en [parámetros](../configuracion/parametros/).
* **Hora:** se encuentre situado justo a la derecha de la fecha, y muestra la hora de grabación del documento. No es manipulable por el usuario.
* **Referencia:** podemos guardar en este campo la referencia del albarán que hemos recibido del proveedor. Será una buena forma de identificar un documento concreto en los localizadores de albaranes de compras.
* **Factura:** se presenta aquí el número del documento y la fecha en la que se ha facturado el albarán de compra además de un botón "Ver" que permite la apertura de la factura desde el propio albarán:

![](<../../.gitbook/assets/imagen (25) (1).png>)

* **Centro:** este campo solo será visible por aquellas aplicaciones Winmotor Multi-Centro, en las que se trabaje con más de un centro de trabajo y así se haya indicado en parámetros. Se utiliza para indicar el centro de trabajo para el que se graba el albarán. Este campo, se rellena automáticamente y solo será manipulable por aquellos usuarios autorizados.
* **Régimen de IVA:** este campo tomará por defecto el tipo de IVA definido en la ficha del proveedor seleccionado en el albarán. Se podrá modificar manualmente.
* **Proveedor:** indicamos aquí el proveedor de la mercancía. Contiene cuatro botones insertados para poder localizar el proveedor deseado, crear uno nuevo, editrlo y cambiar los datos:

![](<../../.gitbook/assets/imagen (26) (1).png>)

* **Dirección, CIF, tipo de pago y vencimientos:** muestra, respectivamente, la dirección, CIF, tipo de pago y vencimientos del proveedor seleccionado. Se podrán modificar sin que estos cambios afecten a la ficha del proveedor. Recordar que tanto el tipo de pago como los vencimientos son campos relacionados con su propia tabla de datos en las que se graban las diferentes posibilidades que se pueden escoger. El acceso a estas dos tablas, lo podrás encontrar en el apartado Maestros del menú Administración.
* **IMPORTE y % de IGIC:** presenta el importe pagado de IGIC por la recepción de la mercancía. El porcentaje se calculará en base al valor total del albarán (quitando el importe de IGIC y de GASTOS añadidos). Para añadir a un albarán el importe de IGIC podemos utilizar el botón situado justo encima de estos campos “insertar importe de IGIC”.
* **Tipo pedido y Gastos de transporte:** muestra los tipos urgente, reposición, garantía y vental al por mayor y presenta el importe pagado de GASTOS por la recepción de la mercancía. El porcentaje se calculará en base al valor total del albarán.

**Barra de pestañas**

* **Artículos:** contiene una rejilla en la que se nos presentan las líneas del albarán de compra ordenadas por el campo contador de cada línea. Mediante está rejilla podremos consultar, grabar, modificar o eliminar cualquier línea de albarán.
* **Totales**: muestra la información totalizada de bases, porcetajes de IVA, importe de IVA y parciales, así como importe pagado y pendiente si es que han existido anticipos de pago asociados al documento.
* **Observaciones**: permite añadir texto libre que únicamente aparecerá en este documento. Es posible imprimir el contenido en los informes de impresión indicándolo al departamento de soporte (es posible que la realización incluya costes de programación)
* **Archivos**: permite almacenar en el servidor cualquier tipo de archivo para su apertura en remoto.

![](<../../.gitbook/assets/imagen (43).png>)

* **Seguimientos**: añade asuntos a la agendas de los usuarios para el control del documento, permitiendo en ésta añadir avisos a horas programables.
* **Auditoría**: control de las modificaciones por usuario y evento
* **Acciones**: control de acciones sobre el documento en función de qué, quién y cuándo se ha realizado.

**Alta de líneas**

Al hacer doble click sobre cualquier línea vacía o pulsar el botón del lateral izquierdo "Nueva línea de artículo o concepto" se nos presentará el formulario de grabación de líneas con los siguientes campos:

\- Artículo: campo en el que introducimos la referencia del artículo que vamos a recepcionar. Se podrá meter la referencia manualmente, o utilizando la opción Buscar Artículo de los botones incrustados de este campo.

\- Almacén: indicamos aquí el almacén en el que entra la mercancía. Será por defecto el definido en la serie del albarán, y no se podrá modificar a menos que así lo indique también en la serie.

Si no localizamos la referencia en la base de datos de artículos, podemos utilizar la opción Referencia, siempre que hayamos importado una tarifa de artículos del proveedor. ["Véase Importador de Tarifas"](../../tutoriales/como-crear-un-importador-de-tarifa-por-marca/)

Los otros botones incrustados que contiene el campo de artículo, son para consultar/editar la referencia seleccionada, servicio o modelo, además de permitir su alta.

La descripción del artículo tomará por defecto la definida en su ficha, pero podrá ser modificada manualmente.

\- Unidades: es un campo manipulable por el usuario, y e indicaremos aquí las unidades que hemos recibido.

\- Precio: importe de compra del artículo. Por defecto tomará el que tuviera el artículo antes de ser recepcionado. Si se modifica este precio, saltará la pantalla de control de precios (ver siguiente imagen), donde podremos modificar los precios directamente en la ficha del artículo:

![](<../../.gitbook/assets/imagen (30).png>)

\- Descuento y Descuento 2: podremos indicar hasta dos posibles descuentos. Si se modifican, también saltará la pantalla de control de precios del artículo.

\- Parcial: valor total del artículo (sin sumar los impuestos) resultante de multiplicar las unidades recibidas por el precio, menos los descuentos.

\- % IVA: tomará el porcentaje de IVA definido en la ficha del artículo si en el albarán se tienen que calcular los impuestos y permitirá su modificación mediante el desplegable:

![](<../../.gitbook/assets/imagen (28).png>)

**Opciones de las líneas de albarán**

* **Aceptar**: con este botón guardamos los cambios realizados.
* **Cancelar**: abortamos el alta o modificación de la línea.

Para eliminar una línea de albarán, tendremos que hacer doble clic en la línea a borrar o editar, se abrirá la ventana del artículo o servicio y pulsaremos el botón "Eliminar":

![](<../../.gitbook/assets/imagen (29).png>)

* **Totales:** presenta el desglose de importe totales del albarán de compra.

**Totales (tipo de impuesto IVA)**

**Totales (tipo de impuesto IGIC)**

![](<../../.gitbook/assets/imagen (31) (1).png>)

* **Observaciones:** aquí podremos anotar todas las notas que necesitemos relativas al albarán de compra.

**Opciones desde un albarán de compra:**

* **Guardar:** si pulsamos esta opción, quedarán guardados todos los cambios que hayamos realizado sobre la ficha del albarán.
* Confirmar: activa el albarán moviendo los artículos a stock (compras)
* **Reparto**: permite mostrar los repartos de los distintos artículos siempre que el albarán haya sido generado desde un pedido de compras con relación a un pedido de ventas u OR, sino se mostrará el contenido vacío al no existir relación a cliente.
* **Cancelar:** con este botón, saldremos de la ficha del albarán sin guardar los posibles cambios que hayamos realizado. Se puede pulsar la tecla ESC para ejecutar esta opción.
* **Eliminar:** el botón solo estará activo si el albarán no está facturado, si se pulsa, se eliminará completamente.
* **Imprimir:** podemos imprimir el albarán mediante este botón.
* **Imprimir Etiquetas:** mediante esta opción podremos emitir las etiquetas de los artículo recibidos. Nos aparecerá la siguiente rejilla. Véase ["Impresión de etiquetas"](../../faq/impresion-de-etiquetas.md)
* **Importar GREC**: opción exclusiva de Yamaha para la importación de albaranes electrónicos
* **Facturar:** este botón sirve para facturar el albarán. Se nos pedirá confirmación del proceso, y a continuación aparecerá en pantalla la factura generada.

![Botones de albarán SIN CONFIRMAR](<../../.gitbook/assets/imagen (32).png>)

![Botones de albarán CONFIRMADO](<../../.gitbook/assets/imagen (33) (1).png>)

![Albarán en modo BORRADOR](<../../.gitbook/assets/imagen (34).png>)

![Albarán CERRADO](<../../.gitbook/assets/imagen (35).png>)

**2 - BUSCAR**

Localizador de albaranes de compras a través de distintos criterios. Nos permite consultar, borrar o modificar la información de un albarán. Al acceder a esta opción encontraremos la siguiente pantalla:

Este localizador nos permite buscar un albarán por los siguientes criterios:

* **Número de documento:** el cursor se irá situando en el albarán cuyo número coincida con el seleccionado.
* \*\*Referencia: \*\*búsqueda relacionada con el campo "Referencia" del albarán
* **Fecha:** el cursor se irá situando en el primer albarán cuya fecha coincida con la seleccionada.
* **Nombre de entidad:** el cursor se irá situando en el albarán cuya razón social vaya coincidiendo con lo introducido en el campo de edición.

Para acceder a la ficha del albarán de compra seleccionado, se puede hacer doble clic sobre él o teclear el botón intro del teclado.

El formulario que se presenta es el mismo que el de grabación.

**3 - LISTADO**

Esta opción lanza una búsqueda que nos presentará un listado de albaranes de compras. Este listado se puede acotar a través del filtro de búsqueda que se presenta a continuación:

![](<../../.gitbook/assets/imagen (36).png>)

Se podrá filtrar por una determinada serie o todas, por un intervalo de fechas, proveedor, centro, tipo de pago, estado (facturado o pendiente) y por la situación del albarán (facturados, pendientes de facturar o todos). Después de indicar los criterios deseados, nos aparecerá una rejilla con los albaranes que cumplan esas condiciones.

**4 – RECEPCIONAR**

[\*\*\* Recomendamos ver primero los 4 métodos de recepción pulsando aquí.](../../videos/metodos-de-recepcion-de-pedidos.md)

Esta opción es una de las cuatro . En este caso, al seleccionar la opción, se nos pedirá un proveedor y una serie (aparece la serie por defecto del perfil).

A continuación aparecerán todas las referencias pendientes de recibir de dicho proveedor. Podremos marcar aquellas líneas a las que le vayamos a dar entrada, así como las unidades que recepcionamos de cada una.

La rejilla es multi-selección, para poder seleccionar las referencias recibidas, y editable, para indicar las unidades que se reciben.

Las opciones que se presentan en esta rejilla, son las mismas que las explicadas en la opción "recibir" de los pedidos de material, un botón para crear los albaranes por las referencias seleccionadas, otro para sustituir referencias, y el último para ver el documento origen de cada línea.

La diferencia entre lanzar la opción desde pedidos de material o lanzarla desde esta opción está en que en la primera solo se creará un albarán de compras por todas las líneas seleccionadas, y en esta segunda opción, creará un albarán por cada serie de albaranes de compras destino existente. Hay que recordar que, en la serie de los pedidos de material se define a que serie de albarán de compra se vinculará cada pedido.

**5 – FACTURACIÓN**

Mediante esta opción, podremos crear facturas de compras en tanda por todos aquellos albaranes de compras pendientes de facturar. Al ejecutar la opción nos aparecerá el siguiente formulario de búsqueda, en el que podremos filtrar por varios criterios como proveedor, fecha, serie, tipo de pago, importe mínimo a facturar y fecha de facturación.

El funcionamiento de esta opción es bastante sencillo, bastará con seleccionar los albaranes que se quieran facturar, y a continuación pulsar sobre el botón situado en la barra de herramientas inferior. El programa se encargará de crear una factura dividiendo los albaranes por series, tipos de pagos, proveedor y régimen de IVA.

![](<../../.gitbook/assets/imagen (39).png>)

![Selección de 6 albaranes de compras](<../../.gitbook/assets/imagen (40).png>)

![Al facturar, se muestra el resultado de la facturación](<../../.gitbook/assets/imagen (41).png>)

**6 - FACTURACIÓN POR SELECCIÓN**

Permite facturar directamente todos los albaranes seleccionados previo filtro de serie, fecha, entidad y/o tipo de pago:

![](<../../.gitbook/assets/imagen (37) (1).png>)

![](<../../.gitbook/assets/imagen (38).png>)
