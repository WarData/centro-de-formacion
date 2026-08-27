# Estados de la sincronización (Stock)

Estados para saber la situación real del stock de un artículo en comparación a la web.

| Estado                 | Cuándo se produce                                                                                   | Significado                                                                                                                                                                                                                 |
| ---------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Sincronizado**       | El stock de WMT y PrestaShop coincide, o la actualización se realiza correctamente                  | El stock del artículo/combinación está correctamente sincronizado con PrestaShop.                                                                                                                                           |
| **Error comunicación** | La API devuelve `STATUS` vacío o `STATUS > 399`                                                     | No se ha podido consultar o actualizar correctamente el stock en PrestaShop. Es un problema de comunicación/API, no necesariamente de existencia del producto. También se usa si falta `ID_STK_WEB` al intentar actualizar. |
| **Incidencia stock**   | Se encuentra el producto/combinación, pero no existe su registro `stock_available`                  | El elemento existe en PrestaShop, pero no se ha localizado su ficha de stock. Por tanto, no se puede consultar/actualizar su cantidad.                                                                                      |
| **Error stock**        | El hijo no tiene `SKU_HIJ`, o en un hijo procesado individualmente falta el ID del padre o del hijo | WMT no tiene la información mínima necesaria para localizar correctamente el stock de la combinación en PrestaShop.                                                                                                         |



### Agrupados por situación

#### ✅ Correctamente sincronizado

* Sincronizado
  * El stock ya coincide.
  * O se ha actualizado correctamente en PrestaShop.

#### 🔴 Requiere revisión

* Incidencia stock
  * Existe el producto/combinación, pero no existe su ficha stock\_available.
* Error stock
  * Faltan IDs/configuración necesaria en WMT para poder localizar el stock.

#### 🟠 Problema técnico / comunicación

* Error comunicación
  * Error HTTP/API al consultar o actualizar.
  * También se utiliza cuando el proceso encuentra un ID\_STK\_WEB vacío y, por tanto, no puede ejecutar la actualización.
