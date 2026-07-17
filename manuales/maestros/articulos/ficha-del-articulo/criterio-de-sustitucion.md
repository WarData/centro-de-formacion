---
description: Criterio de asignación de referencias de sustitución
---

# Criterio de sustitución

El criterio de asignación consiste en aplicar la referencia que disponga de stock, independientemente de que sea anterior o posterior a la referencia introducida.

Por ejemplo, si se introduce la referencia C y la cadena de sustituciones es A → B → C → D → E, el sistema iniciará la búsqueda desde la primera referencia de la cadena (A) y avanzará hasta localizar la primera referencia con stock. Se considera que una referencia tiene stock cuando existe disponibilidad en el almacén del documento desde el que se desea dar salida al artículo.

Si, por ejemplo, la referencia B dispone de stock, será la referencia propuesta en lugar de la C, que fue la introducida inicialmente. El comportamiento posterior dependerá de si el proceso es manual o automático:

*   **Alta manual de líneas:** En el alta manual de líneas, cuando se localice una referencia con stock distinta de la introducida, el sistema solicitará al usuario que decida entre:

    * Mantener la referencia introducida manualmente.
    * Aplicar la referencia localizada con stock.

    Este comportamiento se aplica al alta de líneas de artículos en:

    * Albaranes de venta
    * Pedidos de venta
    * Presupuestos de venta
    * Venta abierta
    * ORs
    * Operaciones
*   **Importación automática:** En los procesos automáticos **no se solicitará confirmación al usuario**. El sistema aplicará directamente la referencia resultante del criterio de asignación descrito anteriormente.

    Este comportamiento se aplica a:

    * La importación desde DSR.
    * La importación de despieces (botón **Despiece**) en ORs, Presupuestos de venta y Pedidos de venta.

Si ninguna de las referencias de la cadena dispone de stock, se aplicará la última referencia de sustitución (E).

