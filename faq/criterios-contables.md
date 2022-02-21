# Criterios Contables

**Entidades**

![](<../.gitbook/assets/image (615).png>)

Como ya sabemos en Winmotor no hay archivos de clientes, proveedores o acreedores, hay un solo archivo llamado “entidades” que se clasifica por múltiples tipos de manera que una misma ficha puede ser a la vez cliente y proveedor, por ejemplo. Cuando vamos a grabar un documento de compras el programa nos permitirá seleccionar una entidad que esté definida como proveedor y si es de ventas tendrá que ser cliente, etc.

La operativa contable automática por lo tanto consiste en que si creamos una nueva entidad y la marcamos como cliente el programa creará automáticamente una cuenta contable 4300 relacionada con la ficha de la entidad asignándole el código de auxiliar igual al código de la entidad. Si a esta misma entidad luego la marcamos también como proveedor el programa automáticamente creará una cuenta 4000 con el código auxiliar igual al código de la entidad. En este caso si por ejemplo la ficha fuera “Empresa ejemplo” con el código 244 tendríamos las siguientes cuentas contables:

·         4300.244 – Empresa ejemplo

·         4000.244 – Empresa ejemplo&#x20;

En la opción “Extractos” dentro de asientos contables contamos además de con la posibilidad normal de consultar el extracto de una cuenta con la operativa para consultar extractos “combinados” de manera que podemos ver por ejemplo en el mismo extracto las dos cuentas relacionadas con una entidad como en el ejemplo anterior: el programa presentará los apuntes de estas dos cuentas en el mismo listado ordenados por fechas. Para esto simplemente hay que utilizar el botón “Mezclar en el extracto” que aparece abajo a la izquierda en el panel de extractos una vez hemos sacado el extracto de la primera cuenta que queremos ver; al pulsar el botón el programa nos pedirá la segunda cuenta a “mezclar” e insertará sus movimientos en el extracto en pantalla.

&#x20;

**Cierres fiscales**

![](<../.gitbook/assets/image (612).png>)

Dado que Winmotor es una aplicación multiusuario y por lo tanto varios usuarios pueden tener acceso a las mismas opciones, existe la posibilidad de que el usuario administrador bloquee la modificación y grabación de documentos y apuntes porque afectan a los impuestos presentados en un período o por cualquier otra razón.

Supongamos por ejemplo que se ha presentado el modelo 303 del primer trimestre, el usuario administrador podrá en ese momento imposibilitar la modificación de facturas de ventas, compras o gastos de ese período para cualquier usuario, incluido él mismo: el sistema en este caso sería crear un cierre de gestión al 31/03 y desde ese momento cualquier documento administrativo con fecha anterior quedará bloqueado para su modificación o borrado; tampoco se podrán grabar nuevos documentos anteriores a esa fecha de cierre.

Los cierres están separados en “gestión” y “contables”. Los cierres de gestión afectan a las facturas de ventas, compras y gastos y los contables a los asientos. De la misma forma el enlace contable desde gestión estará bloqueado para generar asientos con fecha anterior al último cierre contable.

Se accede a la gestión de cierres desde la opción de parámetros en la pestaña “Administración / cierres fiscales”. Si por alguna razón quisiéramos modificar un documento o un asiento contable que está dentro de un período cerrado el sistema permite eliminar el último cierre creado de manera que la fecha de cierre pasaría a la del cierre anterior.



**Tributos**

**Modelo 303**

Dentro del menú de administración tenemos la opción para calcular tributos: para calcular un tributo el programa nos pedirá si queremos hacerlo por un mes, un trimestre o un período libre (fecha desde / fecha hasta) y después nos pedirá el ejercicio.

![](<../.gitbook/assets/image (609).png>)



Es fundamental tener en cuenta que el modelo 303 se calcula desde las facturas emitidas y recibidas por lo que Winmotor para presentarlo lee las facturas del período indicado y no asientos contables como otros programas.

El programa calcula cada partida del modelo en base al régimen de IVA de las facturas implicadas en el período calculado. En las fichas de los tipos de IVA está el campo clasificador para el modelo 303 y se llama “Tipo de IVA repercutido” en el caso de los regímenes de IVA aplicados en las facturas emitidas y “Tipo de IVA soportado” en el caso de las facturas recibidas.&#x20;

![](<../.gitbook/assets/image (611).png>)

&#x20;Los tipos posibles para facturas recibidas son:

·         Régimen general + recargo equivalencia

·         Prestaciones intracomunitarias de servicios

·         Adquisiciones intracomunitarias

·         Entregas intracomunitarias

·         Exportaciones

·         Operaciones no sujetas o con inversión sujeto pasivo con derecho a deducción

Para facturas emitidas:

·         Operaciones interiores bienes corrientes

·         Importaciones bienes corrientes

·         Adquisiciones intracomunitarias de bienes corrientes

·         Compensaciones régimen especial A G Y P

·         Regularización inversiones

·         Operaciones interiores bienes inversión

·         Importaciones bienes inversión

·         Adquisiciones intracomunitarias bienes inversión

·         Inversión del sujeto pasivo

&#x20;

![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image009.jpg)

Al final de la página 1 veremos la totalización del cálculo del impuesto que está desglosado lógicamente en cada una de las partidas según sus tipos de iva como ya hemos indicado.

Disponemos como herramientas de comprobación de dos botones:

·         Comprobación emitidas

·         Comprobación recibidas

Cada uno de ellos presenta el informe resumen correspondiente a las facturas del período del tributo desglosado por el tipo de iva repercutido o soportado según el listado seleccionado. Este informe es exactamente el mismo que podemos obtener en el menú de facturas de ventas, compras y gastos en la opción “Listado Iva”, botón “listado comprobación” y modelo resumen.

El botón “Generar fichero” crea el archivo que podemos subir a la página de hacienda: al pulsarlo el programa pedirá la ruta para guardarlo.

&#x20;

**Modelo 347**

Para el cálculo de este modelo el programa sólo pedirá el ejercicio. Se generarán en la primera página los valores totalizados y en la segunda el detalle de cada entidad con la que hemos superado una facturación de 3.005,06 € en el ejercicio indicado. Por cada una de estas entidades se presenta el volumen trimestral y total calculado:

![](file:///C:/Users/warda/AppData/Local/Temp/msohtmlclip1/01/clip\_image011.jpg)

En ambos modelos los importes calculados por el programa que no son totalizaciones son editables: es decir, si por alguna razón queremos modificar un importe se puede hacer haciendo doble click en la línea correspondiente, el programa recalculará los importes a las que este cambio afecte.

&#x20;
