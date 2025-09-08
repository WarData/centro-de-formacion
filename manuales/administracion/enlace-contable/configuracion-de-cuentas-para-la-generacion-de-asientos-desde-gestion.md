---
description: Exclusivamente para el ejercicio en curso
---

# Configuración de cuentas para la generación de asientos desde gestión

**Configuración de cuentas para la generación de asientos desde gestión**

(Sólo si es el ejercicio en curso y se tienen que crear nuevos asientos desde gestión en esa contabilidad)

* Configurar cuentas contables

**(Muy importante: los ceros a la izquierda de las cuentas auxiliares no son necesarios, es decir la cuenta 1 de ventas debe ser 7000.1 y no 7000.00001)**

1.- Impuestos y cuentas generales

1.1.- Parámetros – Administración – contables

1.1.1.- Comprobar la definición estándar de las cuentas contables en todas las pestañas y notificar al contable por si luego quiere definir alguna diferencia.

![](<../../../.gitbook/assets/imagen (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png>)

1.2.- Cuentas de gastos e ingresos **\*** (el contable debe decidir a qué nivel configura estas cuentas)

1.2.1.- A nivel tipo de producto

1.2.1.1.- Parámetros – Contables – Cuentas por tipo de producto

![](<../../../.gitbook/assets/imagen (3) (1) (1) (1) (1) (1) (1) (1) (1).png>)

1.2.2.- A nivel Serie de documento

1.2.1.1.- Entrando en cada serie de ventas, compras y gastos definir la cuenta contable de esa serie en la pestaña “Contabilidad”.

![](<../../../.gitbook/assets/imagen (4) (1) (1) (1) (1) (1) (1) (1).png>)

1.2.3.- Por familias

1.2.3.1.- Definir cuentas de ventas y gastos en la pantalla principal de familias

![](<../../../.gitbook/assets/imagen (5) (1) (1) (1) (1) (1) (1).png>)



* **Criterio para el cálculo de las cuentas contables de una línea de factura :**
  * Facturas de vehículos de ocasión
    * Cuenta de explotación (compras / ventas)
      * Si la hay en la serie la toma de la serie, sino la toma del tipo de producto 'O'
    * Cuentas de existencias, variación de existencias y costes de ventas
      * Las toma siempre del tipo de producto
  * Resto de facturas
    * Cuenta de explotación
      * Se calcula siempre en base a este criterio:
        * Cuenta del artículo en caso de servicios o cuenta de la familia del artículo en los artículos&#x20;
        * Cuenta de la serie
        * Cuenta del tipo de producto
    * Cuentas de existencias, variación de existencias y costes de ventas
      * Las toma siempre del tipo de producto

. Como se ve y por simplificar digamos que se pueden definir de menor detalle (tipo de producto) a mayor detalle (familias); últimamente dado que todas las estadísticas y análisis se pueden hacer en contabilidad los contables suelen elegir el menor detalle por simplificar. Como es lógico de lo que se trata es de simplificar y que no haya que definir una cuenta contable de gastos y de ingresos en cada artículo.

1.3.- Cuentas de servicios \*\*

1.3.1.- En cada servicio habrá que definir la cuenta de ingresos o de gastos según se utilice el servicio en compras y gastos o en ventas o en ambas

![](<../../../.gitbook/assets/imagen (6) (1) (1) (1) (1).png>)

\*\* Las cuentas contables de servicios sí se utilizan siempre estas. Es decir, la parametrización anterior es sólo para artículos y es variable, para los servicios el programa siempre lee la cuenta del propio servicio.
