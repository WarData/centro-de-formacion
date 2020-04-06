---
description: Nueva Opción Agosto 2019
---

# Cierres Fiscales

Como mejora en la seguridad de la base de datos hemos creado la opción de **“Cierres fiscales”**. 

Consiste básicamente en definir una fecha hasta la que todos los datos fiscales de la aplicación dejan de poder modificarse. **Al definir un cierre fiscal, el programa bloquea la posibilidad de grabar, borrar o modificar facturas de ventas, compras y gastos, así como asientos contables con fecha anterior o igual a la del cierre fiscal.**

El ejemplo básico sería que acabamos de hacer la declaración trimestral de IVA y queremos imposibilitar la modificación de algún dato relativo a esta declaración.

La operativa para crear un cierre fiscal es accediendo al formulario de parámetros en la pestaña “Administración” aparece una nueva pestaña “Cierres fiscales”. Si hacemos doble click aparecerá el formulario para crear un nuevo cierre:

![](../../../.gitbook/assets/image%20%2887%29.png)

![](../../../.gitbook/assets/image%20%28199%29.png)

En la gestión de fichas de cierres hay que tener en cuenta:

* No se podrá crear un cierre con fecha anterior al último cierre
* Los cierres pueden ser de cualquier período \(un día después del último, una semana, un mes o lo que el usuario administrador considere\).
* Un cierre se puede deshacer simplemente borrándolo con lo que la fecha de cierre fiscal pasará a ser hasta el anterior cierre. Se puede eliminar cuando se quiera y luego volver a grabarlo.
* El programa sólo permitirá eliminar el último cierre grabado.
* Una vez grabada la ficha de cierre hay que aceptar el formulario de parámetros: **el cierre será efectivo a partir de ese momento a los usuarios que entren después en el programa, los que ya están dentro tendrán que salir y volver a entrar.**

En el panel de inicio del programa aparece ahora a la derecha del nombre de la empresa la fecha del último cierre fiscal como dato recordatorio. En caso de no haber ningún cierre aparecerá la fecha de inicio de la base de datos:

![](../../../.gitbook/assets/image%20%28360%29.png)

Al presentar una factura o asiento contable de fecha anterior al último cierre aparecerá ahora un candado rojo indicando que está bloqueado:

![](../../../.gitbook/assets/image%20%28273%29.png)

Lógicamente se han bloqueado no sólo los propios formularios para imposibilitar la modificación, sino cualquier opción que pueda afectar al período \(facturación de albaranes, contabilización de facturas, etc...\).

