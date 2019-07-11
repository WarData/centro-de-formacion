---
description: Módulo adicional a la Contabilidad Integrada
---

# Contabilidad Analítica

## **Contabilidad Analítica – Centros de Costes**

Para que este módulo esté activado en el programa debe solicitarlo a Winmotor, es opcional. Una vez activado aparecerán en el menú de contabilidad las siguientes opciones:

**Analítica**

* Centros de costes
* Costes
* Balance analítico
* Desviaciones presupuestarias
* Crear repartos
* Eliminar repartos

**Centros de costes**

Lo primero a decidir es el criterio para crear los centros de costes: para el ejemplo hemos tomado uno de los más claros: crearemos un centro por cada tienda de la empresa. Definiremos por lo tanto primero un centro de costes “genérico” con esta raíz:

![](../../../.gitbook/assets/image%20%28138%29.png)

Antes de definir los criterios de reparto en este centro tendremos que definir un centro por cada tienda de la empresa:

![](../../../.gitbook/assets/image%20%28144%29.png)

Los centros tienen estructura arbolada lo que hace más fácil su visualización: de ahí que los códigos de los centros de las tiendas empiecen con el prefijo “TIE-“.

![](../../../.gitbook/assets/image%20%28137%29.png)

Una vez definida la estructura de nuestros centros \(contamos sólo en la empresa en este caso con dos tiendas\), pasamos a definir el criterio de reparto. La operativa de funcionamiento es como sigue:

·         Cada vez que grabamos un asiento de gasto o ingreso aplicaremos ese gasto o ingreso a uno o varios centros de costes.

o   En el caso de ingresos lo normal es que sepamos cuál es la tienda que ha ingresado.

o   Para los gastos en muchos casos no ha entrado a un centro concreto, sino que es un gasto de la empresa que tendremos que “repartir”.

·         El proceso de “repartir” consiste por lo tanto en que cada vez que grabamos un asiento para repartir le aplicaremos un centro de costes de reparto y mensualmente \(o en el período que queramos\) ejecutaremos la opción de reparto que calculará los centros finales para ese asiento y su importe según el cálculo.

Existen dos distintos métodos o criterios de reparto \(importante marcar primero el check “Reparto de costes indirectos”\):

1 - Cálculo dinámico:

![](../../../.gitbook/assets/image%20%2838%29.png)

Tendremos que definir por un lado qué centros son los afectados cuando hagamos el cálculo “Centros de costes destino del reparto” y por otro lado las cuentas y el criterio por el que se va a repartir.

Lo más lógico en este tipo de reparto es utilizar como cuenta de reparto una cuenta genérica de ingresos y utilizar como criterio de reparto su acumulado haber o su saldo.

Este criterio de reparto implica que en el momento del reparto el programa calculará para cada asiento a repartir un importe según el porcentaje de ingresos que tenga cada una de las tiendas sobre la cuenta general de ingresos. Veremos esto en detalle más adelante cuando lleguemos a la opción de repartos.

2 - Cálculo por cuotas fijas

![](../../../.gitbook/assets/image%20%2854%29.png)

El cálculo por cuotas fijas es tan fácil como pasar a la derecha los centros a los que queremos que afecte y definir haciendo doble click sobre cada uno de ellos el porcentaje que queremos repercutir.

Por lo demás para el alta de centros de costes no hay que definir mucho más a excepción de las partidas presupuestarias que las veremos al llegar a esa opción. Las dos primeras pestañas “Asientos” y “Saldos” son para consulta, aparecerán los aplicados a cada centro y la opción para plantillas en centros de costes aún no es funcional.

**Costes**

La opción en sí es simplemente para consulta y listado de asientos de costes, no podemos grabar directamente en ella. Al entrar aparecerá una pantalla parecida a la de diario de asientos donde podremos filtrar por fechas, centro de costes y posibles estados de los asientos \(Pendiente de repartir, reparto realizado o generado por reparto\).

![](../../../.gitbook/assets/image%20%2889%29.png)

Vamos a ver por lo tanto cómo se graban estos asientos utilizando para el ejemplo un asiento de compras que vamos a repercutir al centro de reparto “TIE”:

·         Al grabar el apunte de compras en un asiento **pulsaremos el botón con el ojo** al lado de “Costes”

![](../../../.gitbook/assets/image%20%28227%29.png)

·         Al pulsar el botón aparecerá esta pantalla

![](../../../.gitbook/assets/image%20%28182%29.png)

·         Pulsaremos el botón “+” y aparecerá esta pantalla para grabar el centro y el importe a imputar:

![](../../../.gitbook/assets/image%20%28212%29.png)

·         Hemos definido en este apunte de costes el centro “TIE” que es un centro de reparto y el importe total de la compra: 2.000€.

·         Si aceptamos este formulario y cerramos el asiento al volver a la opción de “costes” y pulsar la lupa para buscar aparecerá el nuevo asiento de costes:

![](../../../.gitbook/assets/image%20%2859%29.png)

**Balance analítico**

Nos presentará los saldos de los distintos centros de costes detallado por meses y cuentas. Al igual que en un balance normal de sumas y saldos podremos filtrar hasta un mes, por centro de costes y/o por cuentas y presenta esta información:

![](../../../.gitbook/assets/image%20%2824%29.png)

Desviaciones presupuestarias \(en fase de programación\)

**Crear reparto**

Al ejecutar la opción de crear repartos el programa presenta el siguiente filtro para el cálculo:

![](../../../.gitbook/assets/image%20%28199%29.png)

Al aceptar el programa realizará los cálculos correspondientes y presentará el resultado del reparto:

![](../../../.gitbook/assets/image%20%28267%29.png)

Podemos ver como ha repartido el gasto de 2.000€ imputado al centro genérico “TIE” entre la tienda de Sevilla y Málaga según el saldo de la cuenta 700 en las delegaciones de Sevilla y Málaga.

Volvemos aquí a analizar los criterios de cálculo de repartos:

·         Cálculo dinámico

o   En el centro de reparto habíamos definido los centros destino del reparto, así como el criterio de reparto que sería el saldo de la cuenta 700.

o   **Es fundamental tener en cuenta para entender este proceso de cálculo que el programa buscará y acumulará el saldo de la cuenta especificada en los centros destino del reparto y repartirá en base a la proporción de cada uno sobre el acumulado de la cuenta en todos los centros.**

o   En el ejemplo:

§  Saldo 700 tienda de Málaga       5.804,96€

§  Saldo 700 tienda de Sevilla         1.000,00€

§  Acumulado 700                               6.804.96€

§  Importe a repartir \(gastos\)         2.000,00€

§  Imputado a Málaga

·         5.804,96 sobre 6.804,96 = 85,3 %

·         85,3% sobre 2.000 = 1.706€

§  Imputado a Sevilla

·         1.000,00 sobre 6.804,96 = 14,7 %

·         85,3% sobre 2.000 = 294€

·         Cálculo por cuotas fijas

o   En el centro de reparto definimos los centros destino de reparto y la cuota de reparto de cada uno

o   En este caso el cálculo es mucho más sencillo: el programa simplemente calculará ese porcentaje sobre el importe a repartir y creará un asiento por cada centro destino del reparto.

**Eliminar reparto**

Con esta opción simplemente deshacemos un reparto previamente calculado. Se puede utilizar en cualquier momento especificando los siguientes datos:

![](../../../.gitbook/assets/image%20%28183%29.png)

Al aceptar el programa eliminará el reparto especificado y dará el mensaje de fin.

