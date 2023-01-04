# Honda ARE - Configuración de cuentas contables

En el procedimiento de contabilización de gastos e ingresos Honda – ARE la contabilidad se genera utilizando el sistema de variación de existencias y de costes de ventas y para esto han definido un plan contable específico dentro del grupo “0”.

**Las fuentes de cuentas contables que utiliza Winmotor para calcular cada partida de una factura son:**

* Familias de productos:
  * Honda clasifica las familias de productos en Reposición, Mantenimiento, Accesorios, Aceites y Neumáticos. El código de cada una de estas familias en el programa debe estar referenciado en la pestaña “Generales” de los parámetros de Honda ARE y todos los productos que se creen en el programa deben estar definidos en una de estas familias o sus subfamilias.
  * Dentro de la ficha de cada familia veremos siempre un botón “Honda” donde se definen sus cuentas contables y una vez pulsemos este botón veremos los tres tipos de cuentas que se manejan en las familias separados en tres distintas pestañas:
    * Albaranes
    * Órdenes de reparación
    * Compras y existencias
* Series de vehículos
  * Todos los vehículos que demos de alta en la aplicación deben estar dentro de la siguiente estructura de datos:
    * Modelo – Versión – Gama – Serie
  * Es en las series de vehículos (Naked, Super Sport, Touring, etc) donde Honda define las cuentas relacionadas para la contabilización de compras y ventas. Llegamos a la lista de series desde el menú “Automoción - Comercial – Modelos – Listados – Series de vehículos”
  * En todas las series aparece un botón “Honda” que presenta el formulario de configuración de cuentas contables.
* Servicios
  * Llamamos “Servicio” en Winmotor a cualquier cosa que se compre o venda y no sea ni un producto del que controlemos existencias ni mano de obra de taller. Los servicios se crean y consultan en un panel específico “Maestros – Servicios”.
  * Al igual que en las familias y en las series de vehículos en el formulario de cada servicio aparece un botón “Honda” donde se define el procedimiento de contabilización del servicio.
  * En Honda ARE un servicio se puede contabilizar de tres formas distintas: “Directa”, “Directa y analítica” y “Por serie de vehículo”. La documentación específica para esto se encuentra en: [Honda ARE - Contabilización de Servicios](https://winmotor.gitbook.io/project/manuales/administracion/enlace-contable/honda-are-contabilizacion-de-servicios)
* Parámetros
  * Podemos decir que todo lo que no es una venta o compra de vehículo, de un producto de stock o de un servicio se configura en parámetros.
  * Accedemos a la configuración Honda ARE en la pestaña de parámetros -Marcas – Honda – ARE. A nivel contable se parametriza en las pestañas:
    * Vehículos nuevos (otras marcas)
    * VO
    * Mano de obra taller
    * Cargo interno

Por otro lado, en Honda ARE se hacen diferenciaciones de compras y ventas según sean Honda o no y también en el caso de ventas se diferencia por ejemplo si es a cliente final o a agentes: todas estas variaciones están contempladas en cada una de las pestañas que hemos detallado.

**Localización de cuentas específicas según la partida de la factura:**

* Documentos de Ventas
  * Cuenta de ingresos
    * Taller
      * Mano de obra
        * General
          * Parámetros – Marcas – Honda – ARE – “Mano de obra taller”
        * Facturas internas
          * Parámetros – Marcas – Honda – ARE – “Cargo interno taller”
      * Recambios
        * Familia – Honda – “Órdenes de reparación”
    * Recambios
      * Familia – “Honda”
      * Separados en “Albaranes” y “Órdenes de reparación”
    * Vehículos
      * Serie del vehículo – “Honda”
    * Servicios
      * Servicio – “Honda”
  * Costes de ventas y existencias
    * Taller
      * Facturas internas
        * Parámetros – Marcas – Honda – ARE – “Cargo interno taller”
      * Otras facturas
        * Parámetros – Marcas – Honda – ARE – “Mano de obra taller”
    * Recambios
      * Familia – “Honda”
    * Vehículos
      * Serie del vehículo – “Honda”
    * Servicios
      * Servicio – “Honda”
      * Ampliación de los criterios en la ayuda ya existente – [Honda ARE - Contabilización de Servicios](https://winmotor.gitbook.io/project/manuales/administracion/enlace-contable/honda-are-contabilizacion-de-servicios)
      * Compras
        * Recambios
          * Familias – “Honda “ – “Compras y existencias”
        * Vehículos
          * Series – “Honda” – En el mismo formulario se configuran cuentas de ventas y de compras.
