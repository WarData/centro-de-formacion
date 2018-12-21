# Gestión de la rotación de consumos y el stock mínimo de artículos

Se trata del proceso mediante el que el programa calcula de forma automática y según los parámetros definidos el stock mínimo o de seguridad que queremos establecer para cada artículo o grupo de artículos. El programa ejecuta este proceso de cálculo diariamente en el servidor.

Los parámetros básicos para establecer una cantidad de stock mínimo para un artículo son:

-          **Días para el cálculo del consumo medio**: se trata de definir el número de días para que el programa analice el consumo de cada artículo. Se entiende que son los días hasta el momento del cálculo

-          **Fórmula para el cálculo del stock mínimo**: es la fórmula mediante la que definiremos para cada artículo su stock mínimo. Lo lógico será utilizar en esta fórmula los días de consumo calculados \(Por ejemplo, el consumo de los últimos 180 días divididos por seis sería el consumo medio de los seis últimos meses\). También se puede utilizar en esta fórmula el plazo de entrega del proveedor pero esto requiere una parametrización a nivel proveedor o artículo.

Para evitar el enorme trabajo que supondría establecer estos parámetros en cada artículo la aplicación da la posibilidad de definir los parámetros a nivel:

-          Tipo de artículo

-          Marca

-          Proveedor

-          Familia

-          Artículo

Esta parametrización es escalable, es decir, podemos definir por ejemplo una fórmula general para toda una familia de artículos pero si queremos que uno en concreto tenga un cálculo distinto definiendo una fórmula para ese artículo ésta prevalecerá sobre la de la familia. El orden en el que hemos presentado la definición es el inverso al que el programa analiza para saber la fórmula de cada artículo, es decir, prevalecerá una fórmula para un artículo sobre una fórmula para una familia, una de familia sobre una de proveedor, etc.

Dado este criterio los **parámetros mínimos** a definir para gestionar en la aplicación el stock mínimo serán por lo tanto uno por cada tipo de artículo.

Es fundamental tener en cuenta que la aplicación utiliza como dato de stock para saber si estamos por debajo del mínimo no el stock físico de cada artículo sino su **stock previsto.**

1.       Puesta en marcha / configuración

Los usuarios con nivel por encima del básico podrán acceder a la configuración del stock mínimo bien desde el formulario de parámetros o bien desde la opción que se encuentra en el panel de gestión del stock mínimo. En la rejilla presentada haciendo doble clic en cualquier posición se presentará este formulario:

![](../.gitbook/assets/image%20%2848%29.png)

En este ejemplo estamos definiendo para todos los artículos tipo “Varios” un período de cálculo de consumo medio de 30 días y la fórmula se ha establecido que el stock mínimo será el Consumo Medio \(\#CM rehacer imagen\)  multiplicado por 2.

Existe por otro lado la posibilidad de definir para un artículo su stock mínimo manualmente. Esto hay que hacerlo directamente en la pestaña “Consumos / rotación” del artículo y en caso de estar definido el campo éste prevalecerá sobre el cálculo automático que pueda afectar al artículo.

2.       Proceso de cálculo

Como se ha mencionado anteriormente el sistema ejecuta diariamente en los procesos de mantenimiento el cálculo del consumo medio \(y en consecuencia del stock mínimo\) de todos los artículos activos de la base de datos.

A consecuencia de este cálculo la aplicación clasificará los artículos en estos posibles estados de consumo:

a.       En rotación

Artículos que tienen alguna unidad consumida en el período de consumo.

**En caso de que el stock previsto de un artículo esté por debajo de su stock mínimo quedará marcado como bajo mínimo.**

b.       Obsoleto

Artículos que no tienen ninguna unidad consumida en el período de consumo.

                                                               i.      PASAR AUTOMÁTICAMENTE A EN ROTACIÓN EN EL MOMENTO QUE TENGA CONSUMO. Lo pasará automáticamente el proceso diario pero hay que analizar si hacerlo por actualización \( ¿ de la ficha de consumo ¿\)

c.       Estacional \(analizar qué hacemos a este respecto con los artículos estacionales en los que se marca que si queremos analizar su consumo fuera del período estacional\).

                                                               i.      En período de aprovisionamiento

1.       Aprovisionado

2.       No aprovisionado

                                                             ii.      En período estacional

                                                           iii.      Fuera del período estacional

3.       Artículos con consumo estacional

Son aquellos cuyo consumo tiene un comportamiento especial en cierta estación del año. Pueden ser artículos que sólo se consumen en un período concreto o que en ese período tienen un consumo especial.

La definición de artículos estacionales hay que hacerla forzosamente por cada artículo, no se puede aplicar un criterio por grupos aunque sí hay una herramienta para aplicar los criterios de artículo estacional para una lista completa de artículos.

-          Alta de artículos estacionales

Accediendo a la pestaña “Rotación/consumos” de la ficha del artículo veremos un botón para definir un consumo estacional. Los parámetros a definir son:

-          **Período estacional**: son períodos que deben estar previamente creados por el usuario administrador del sistema en la pestaña “Gestión – períodos” del formulario de parámetros. Se definen en estas fechas el día/mes de inicio y fin de un período y se le asigna un nombre. Este campo indica por lo tanto cuál es el período de consumo especial del artículo.

-          **Unidades de aprovisionamiento**: son las unidades que consideramos que debemos tener en stock a la llegada del período estacional. Para facilitarnos el cálculo el programa nos presenta un botón junto a este campo con el que podemos calcular el consumo de este artículo en su período en el año anterior. El valor propuesto se puede manipular pero quedará modificado si volvemos a pulsar el botón.

§  **Plazo de aprovisionamiento**: es el número de días antes del inicio del período estacional en el que el artículo pasará a “Período de aprovisionamiento”.

4.       Panel de gestión y consulta

Desde el menú de artículos accedemos al panel de **gestión de consumos y stock mínimos**  mediante la opción que aparece a tal efecto.

\*\*\* IMAGEN DEL PANEL

En el panel se presentarán las distintas clasificaciones de los artículos en base a sus consumos:

-          Artículos bajo mínimo

o   Se presentan en la rejilla los valores de stock de cada artículo y debajo una barra de herramientas mediante la que podremos:

§  Generar pedidos. Marcando los artículos sobre los que queremos generar pedido al pulsar el botón la aplicación creará \( o añadirá a pedidos de compras no tramitados\) los artículos seleccionados clasificándolos por su proveedor

§  Listar

o    

-          Artículos obsoletos

-          Artículos estacionales

5.       Notificación automática de los cambios en rotación de stocks

