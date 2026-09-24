# KPI   producción taller

_**KPI – Producción de taller (exclusivo Yamaha)**_

* Informe estadístico con el que podremos sacar la productividad del taller. Desde esta opción se puede sacar la información de distintas formas en función de los filtros que apliquemos. Siempre la información es sobre las órdenes facturadas.

<figure><img src="../../../../../.gitbook/assets/image (750).png" alt="" width="270"><figcaption></figcaption></figure>



* ### **Por mecánico**
  * Muestra un resumen de productividad por cada mecánico informando de:
    * **Nº de órdenes:** número de órdenes en las que ha intervenido.
    * **Horas presencia:** se calcula según el módulo del control presencial, no sobre intervenciones. Existen distintas formas de controlar la entrada y salida de un mecánico a trabajar:
      * **Logeo en panel control presencial:** este panel tendrá que estar abierto en un equipo accesible por todos. Cada mecánico, cuando empiece o finalice su jornada laboral, pasará su código para que el sistema lo identifique y abra o cierre el tiempo.
      * **Automático:** cuando el usuario abra su sesión en el sistema, automáticamente lo dará por logeado. Es necesario configurar cada mecánico en su ficha de usuario.
    * **Horas empleadas:** suma de las horas intervenidas en cada OR del mecánico.
    * **Horas facturadas:** total de horas facturadas entre el número de mecánicos que intervienen en la orden.
    * **Recambios:** importe total facturado en recambios entre el número de mecánicos que intervienen en la orden. Si intervienen en la orden más de un mecánico, este importe será el resultado de dividir el total facturado de recambios entre el número de mecánicos. Si hay dos y se facturan 500 € en recambios, el importe presentado aquí será 250 €. Si se excluyen accesorios, no se sumarán a esta cifra.
    * **Mano de obra:** importe total facturado de mano de obra (temparios) entre el número de mecánicos que intervienen en la orden.
    * **Conceptos:** importe total facturado en servicios externos o conceptos entre el número de mecánicos que intervienen en la orden.
    * **Beneficio:** los valores anteriores menos el coste de cada partida.
    * **% ocupación:** se calcula dividiendo el tiempo trabajado entre el tiempo de presencia.
    * **% eficiencia:** se calcula dividiendo el tiempo facturado entre el tiempo trabajado.
    * **% productividad:** se calcula dividiendo el tiempo facturado entre el tiempo de presencia.
  * Si hay órdenes en las que no ha intervenido ningún mecánico, se presentará una primera línea “sin operario” para acumular los valores de nº de ORs e importes.
  * Si se hace doble clic sobre el valor de recambios, mano de obra o conceptos de un mecánico, se nos presentará el detalle de líneas de donde procede ese valor.
  * Si marcamos “incluir comparativa”, por cada dato se nos calcularán dos columnas: una por el periodo del año seleccionado en el filtro y otra por el año anterior.

<figure><img src="../../../../../.gitbook/assets/image (751).png" alt=""><figcaption></figcaption></figure>

* ### Resumen Intervalo
  * Presenta la evolución del año dividido en meses de la facturación de mano de obra, facturación de recambios y facturación de servicios externos o conceptos.
  * Lo ideal es mantener como intervalo el año completo en el filtro presentado.

<figure><img src="../../../../../.gitbook/assets/image (752).png" alt=""><figcaption></figcaption></figure>
