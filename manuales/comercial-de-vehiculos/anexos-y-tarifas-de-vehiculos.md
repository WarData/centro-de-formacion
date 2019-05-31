# Anexos y Tarifas de Vehículos

  
_**Gestión de cargos impuestos por el concesionario - Documentación - Anexos**_

**Criterios de aplicación**

* Se aplican y calculan sobre todos los modelos-color \(los que se pueden vender\) afectados por los campos Marca y Gama - Versión - Modelo del anexo 
* En caso de tener marcado un centro, se aplicarán específicamente en los documentos de ese centro, si no lo tienen definido se aplicarán en todos los centros \(para aplicación Winmotor multicentro los anexos podrán ir independientemente por centro\). La selección del centro aparece encima de la marca en la imagen superior.

![](../../.gitbook/assets/image%20%28203%29.png)

               o   En la consulta de modelos si hay cargos aplicados a centros se calculará en base al centro del usuario que está consultando.

![](../../.gitbook/assets/image%20%28220%29.png)

               o   Si el usuario es un administrador del sistema y no tiene centro se le presentarán los precios calculados sobre todos los centros.

* En caso de marcarse “Incluir en factura de vehículo” se añadirán al importe del vehículo en la factura. **Caso de no estar marcado se añadirán en el resto de documentos de ventas, pero no en la factura. Si no está marcado no se podrá aplicar Impuesto de matriculación**

![](../../.gitbook/assets/image%20%2841%29.png)

* En caso de marcarse “Detallar en factura” se añadirán a la factura en una línea aparte \(y por lo tanto lógicamente no se añadirán al importe del vehículo\). Lógicamente sólo se podrá marcar “detallar en factura” si se ha marcado previamente “incluir en factura de vehículo”.

![](../../.gitbook/assets/image%20%28229%29.png)

* En el resto de documentos de ventas, en caso de estar marcado “Detallar en factura” aparecerán como una línea aparte, pero **en caso de no estar marcado se añadirán siempre al importe del vehículo esté o no marcado el check “Incluir en factura”.**
* El impuesto de matriculación de un anexo sólo se podrá aplicar en caso de marcar “incluir en factura de vehículo” y “detallar en factura”.
* **El check "El del servicio"** se refiere a que, si está marcado, cogerá el precio del servicio permitiendo mantener los anexos año tras año variando únicamente un precio o, si no está marcado, añadirlo manualmente a cada Marca y Gama - Versión - Modelo.

![](../../.gitbook/assets/image%20%28243%29.png)

Finalmente, así quedaría en el alta de una operación comercial / tráfico:

![](../../.gitbook/assets/image%20%28116%29.png)

