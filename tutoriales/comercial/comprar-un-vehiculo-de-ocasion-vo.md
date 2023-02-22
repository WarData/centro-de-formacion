---
description: >-
  Tutorial paso a paso para la compra de un VO tanto si existe el bastidor en la
  base de datos como si no existe.
---

# Comprar un vehículo de ocasión VO

Hay una serie de **requisitos que deben estar bien configurados en su BBDD:**

1.- La serie del documento **albarán de compra VO debe tener marcado el check "Serie para VO"**

![](<../../.gitbook/assets/image (607) (1) (1).png>)

2.- Para entidades particulares, al dar de alta un albarán podemos seleccionar una entidad tipo cliente y Winmotor añadirá el tipo "Proveedor". **Verficar que el régimen de IVA es R7 (No sujeto) o R8 (Régimen de bienes usados). Valdría cualquiera de los 2 tipos siempre que la entidad sea "PARTICULAR".**

![](<../../.gitbook/assets/image (606) (1).png>)

3.- Para **entidades empresa** también se actualizará a tipo "Proveedor", pero el **régimen de IVA será R1 (General) y no aplicará REBU.**

**----------------------------------------------------------------------------------------------------**

**\*\*\* PROCESO GENERAL DE ALTA DE UN ALBARÁN DE COMPRAS VO PARA LA ADQUISICIÓN DE UN VEHÍCULO QUE SE DA DE ALTA EN LA BBDD POR PRIMERA VEZ:**

A > Seleccionar Serie de Albarán de Compras VO

![](<../../.gitbook/assets/image (613) (1) (1) (1).png>)

B > Usar la lupa de búsqueda en cualquier caso para añadir tipo de entidad "Proveedor" a una entidad > si la entidad existe como proveedor, verificar régimen y tipo de proveedor (particular o sociedad). Si existe sólo como cliente, verificar igualmente régimen y tipo

![](<../../.gitbook/assets/image (611) (1).png>)

Verificar régimen de IVA en compras R7 / R8 para particulares

![](<../../.gitbook/assets/image (614) (1) (1) (1).png>)

C > Botón "Crear entrada VO" > ![](<../../.gitbook/assets/image (610) (1).png>)

**Único método para la entrada de un vehículo de ocasión VO. No usar ningún otro método ni botón**

D > La ventana emergente mostrará los campos para el alta, de los cuales sólo es necesario usar "Marca", "Modelo", "Color", "Bastidor", "Matrícula", "Precio de compra" y opcionalmente "PVP" ya que este puede variar. En cualquier caso siempre se podrá modificar durante la venta, tanto si está a 0 como **si se rellena un importe PVP (incluye los impuestos sobre la parte del beneficio y exención sobre la base para REBU).**&#x20;

Los campos "Gama - Versión" se pueden rellenar, pero **no es necesario ya que se puede hacer de forma manual en el campo "Modelo":**

![](<../../.gitbook/assets/image (612) (1).png>)

E > Aceptar y pulsar botón ![](<../../.gitbook/assets/image (609) (1) (1).png>) o F5 (Actualizar) > **aparecerá la línea del vehículo en el albarán**

F > Pulsar en "Confirmar" ![](<../../.gitbook/assets/image (605) (1).png>) **para pasar el vehículo de ocasión VO al STOCK**

****![](<../../.gitbook/assets/image (608).png>)****

**----------------------------------------------------------------------------------------------------**

**\*\*\* PROCESO GENERAL DE ALTA DE UN ALBARÁN DE COMPRAS VO PARA LA ADQUISICIÓN DE UN VEHÍCULO EXISTENTE EN LA BBDD:**

A > Seleccionar Serie de Albarán de Compras VO

B > Usar la lupa de búsqueda en cualquier caso para añadir tipo de entidad "Proveedor" a una entidad > si la entidad existe como proveedor, verificar régimen y tipo de proveedor (particular o sociedad). Si existe sólo como cliente, verificar igualmente régimen y tipo

C > Botón "Crear entrada VO" > ![](<../../.gitbook/assets/image (610) (1).png>)

D > Introducir el bastidor de un vehículo en el campo "Bastidor" y pulsar tabulador. Aparecerá un botón que indica que el bastidor existe y lo pulse para actualizar con los datos guardados en la BBDD:

![](<../../.gitbook/assets/image (604) (1) (1).png>)

Al pulsar el botón se rellenan los datos automáticamente y ahora rellenar precios y algún posible cambio y "Aceptar":

![](<../../.gitbook/assets/image (613) (1) (1).png>)

E > Aceptar y pulsar botón ![](<../../.gitbook/assets/image (609) (1) (1).png>) o F5 (Actualizar) > **aparecerá la línea del vehículo en el albarán**

F > Pulsar en "Confirmar" ![](<../../.gitbook/assets/image (605) (1).png>) **para pasar el vehículo de ocasión VO al STOCK**
