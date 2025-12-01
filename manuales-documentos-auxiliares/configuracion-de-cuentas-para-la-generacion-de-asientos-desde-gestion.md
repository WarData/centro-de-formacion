---
description: >-
  (Sólo si es el ejercicio en curso y se tienen que crear nuevos asientos desde
  gestión en esa contabilidad)
---

# Configuración de cuentas para la generación de asientos desde gestión (ejercicio en curso)

Capturas de imagen en [Administración > Contabilidad](../manuales/administracion/enlace-contable/configuracion-de-cuentas-para-la-generacion-de-asientos-desde-gestion.md)

Configurar cuentas contables (Muy importante: los ceros a la izquierda de las cuentas auxiliares no son necesarios, es decir la cuenta 1 de ventas debe ser 7000.1 y no 7000.00001)

* Impuestos y cuentas generales
  * Parámetros – Administración – contables
    * Definir las cuentas contables en todas las pestañas tal como estén en otra distribución y notificando al contable por si luego quiere definir alguna diferencia (se le puede por ejemplo pasar pantallazos de todas estas pestañas una vez rellenas y siempre que tengan cuentas contables).
* Cuentas de gastos e ingresos (el contable debe decidir a qué nivel configura estas cuentas) \*
  * A nivel tipo de producto
    * Parámetros – Contables – Cuentas por tipo de producto
  * A nivel Serie de documento
    * Entrando en cada serie de ventas, compras y gastos definir la cuenta contable de esa serie en la pestaña “Contabilidad”.
  * Por familias
    * Definir cuentas de ventas y gastos en la pantalla principal de familias<br>
* **Criterio para el cálculo de las cuentas contables de una línea de factura :**
  * Facturas de vehículos de ocasión
    * Cuenta de explotación (compras / ventas)
      * Si la hay en la serie la toma de la serie, sino la toma del tipo de producto 'O'
    * Cuentas de existencias, variación de existencias y costes de ventas
      * Las toma siempre del tipo de producto
  * Resto de facturas
    * Cuenta de explotación
      * Se calcula siempre en base a este criterio:
        * Cuenta del artículo en caso de servicios o cuenta de la familia del artículo en los articulos&#x20;
        * Cuenta de la serie
        * Cuenta del tipo de producto
    * Cuentas de existencias, variación de existencias y costes de ventas
      * Las toma siempre del tipo de producto

`*Como se ve y por simplificar digamos que se pueden definir de menor detalle (tipo de producto) a mayor detalle (familias); últimamente dado que todas las estadísticas y análisis se pueden hacer en contabilidad los contables suelen elegir el menor detalle por simplificar. Como es lógico de lo que se trata es de simplificar y que no haya que definir una cuenta contable de gastos y de ingresos en cada artículo.`

* Cuentas de servicios \*\*
  * En cada servicio habrá que definir la cuenta de ingresos o de gastos según se utilice el servicio en compras y gastos o en ventas o en ambas

`** Las cuentas contables de servicios si se utilizan siempre estas. Es decir, la parametrización anterior es sólo para artículos y es variable, para los servicios el programa siempre lee la cuenta del propio servicio.`
