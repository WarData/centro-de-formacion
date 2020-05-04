# Preparación de Entregas

Se trata de un sistema que guiará al usuario en el proceso de preparación de entregas de material que puede ser con origen en pedidos, albaranes o facturas de ventas. El usuario podrá utilizar para esto una tableta, PDA o teléfono móvil con un mínimo de tamaño de pantalla de 5”.

En un primer paso hay que definir en los parámetros de la aplicación \(Parámetros - Gestión - Generales\), el tipo de documento que se utiliza en la empresa para la preparación de entregas y en segundo lugar definir también en qué orden queremos que aparezcan luego los artículos.

Una vez seleccionada la opción “Preparación pedidos” se nos presentará una pantalla con aquellos documentos pendientes de entregar para seleccionar el que vamos a preparar.

![](../.gitbook/assets/image%20%28357%29.png)

Haciendo click sobre uno de los documentos se presentará el detalle de su contenido.

En el momento en que un usuario selecciona un documento para preparar su entrega éste quedará bloqueado en la base de datos para cualquier modificación apareciendo un mensaje en su cabecera que lo indica en caso de que otro usuario accediera al documento.

En la columna de unidades se presentan las unidades a embalar y las ya embaladas. Esta columna está totalizada para ayudar al usuario en el control.

![](../.gitbook/assets/image%20%28228%29.png)

La operativa para ir preparando líneas puede ser o bien pinchando en una línea o bien escaneando un código de barras. Al hacerlo aparecerá en la cabecera de la pantalla el artículo seleccionado y podremos hacer dos cosas:

·         Si hemos escaneado automáticamente se marcará una unidad como preparada.

·         Si lo hemos seleccionado en la lista tendremos que pulsar el icono de aceptación de la lectura y se marcará una unidad como preparada.

![](../.gitbook/assets/image%20%2884%29.png)

![](../.gitbook/assets/image%20%28365%29.png)

Si queremos que la aplicación considere que todas las unidades de ese producto han sido preparadas tendremos que pulsar en el botón de acumulación del total de la línea, en otro caso habrá que escanear tantas unidades como haya que embalar.

![](../.gitbook/assets/image%20%28214%29.png)

La línea que ha quedado completamente preparada aparecerá con fondo amarillo.

![](../.gitbook/assets/image%20%2813%29.png)

El sistema de caja funciona de la siguiente forma:

·         Se considera que siempre empezamos por la caja 1 \(el número de caja en curso aparece junto al botón de cambio de caja\).

·         Cuando queremos decirle al programa que empezamos a embalar en la siguiente caja pulsaremos sobre el botón de cambio de cajas.

·         Si de una misma línea hay productos en más de una caja lo indicaremos así en el botón de acumulación del total de líneas que nos presenta el total de productos contados

![](../.gitbook/assets/image%20%28299%29.png)

En el ejemplo en pantalla vemos que la línea de la ROSA MOSQUETA ha quedado guardada en la caja 2 y en la caja 3.

Al consultar luego el documento en el PC se nos mostrará una nueva pestaña “Cajas” que detalla qué contiene exactamente cada caja.

Para la finalización del proceso basta con pulsar el botón “Entregar” que se encenderá cuando estén embaladas todas las unidades del documento. En caso de que el operario quiera dejar el proceso sin terminar puede pulsar el botón “Pausar” y cuando vuelva a seleccionar el documento se lo presentará tal como lo dejó. En caso de pulsar “Salir” se considera el proceso abortado y cuando se recupera el documento de nuevo empieza el recuento desde el principio.

