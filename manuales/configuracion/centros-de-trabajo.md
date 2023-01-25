# Centros de Trabajo

**Descripción**

Llamamos “Distribución multicentro” a la implantación de la aplicación en una base de datos en la que éstos están divididos por centros de trabajo. Dentro de estos centros existe siempre uno definido como “central” y uno o varios centros de distribución o “puntos de venta”. En una distribución de este tipo cada documento existente en la base de datos tiene especificado como dato principal en la cabecera su “Centro”.

Para que esta operativa esté activada debe intervenir por un lado Winmotor marcando la distribución como “Multicentro” y por otro lado el administrador de la base de datos creando la estructura de centros. Los centros se crean dentro de la opción general “configuración” e internamente son fichas de entidades. Esta opción no será visible en "Configuración" en caso de que la base de datos sea monocentro.

Como hemos dicho al principio debe existir en este tipo de distribución un centro definido como “central” y al menos uno más como “punto de venta”. El centro “central” en principio será además una entidad “Proveedor” y el centro punto de venta será también “Cliente”.

**Base de datos**

En este tipo de distribución la base de datos se estructura de la siguiente forma:

* Artículos

o Son comunes a todos los centros pero para cada ficha de artículo el programa exige definir una ficha de tarifa de proveedor donde éste podrá ser distinto para cada centro. Normalmente en el centro “central” el proveedor será el fabricante del producto y en los puntos de ventas el proveedor será la propia central. Así mismo los precios de costo pueden variar para un mismo artículo en uno u otro centro.

o El stock de cada artículo queda a su vez separado por centros aunque se puede luego consultar y listar a nivel centro o a nivel general de la empresa. En el cálculo de stock y disponibilidad de un artículo en un documento se tendrá en cuenta el de su centro, no el de la empresa. Esto quiere decir que si estamos grabando por ejemplo un albarán de ventas en un centro concreto y en éste no hay disponibilidad de stock la aplicación no permitirá su grabación.

o Los movimientos de stock entre centro están contemplados en el programa de forma automatizada mediante pedidos y albaranes. Puntualmente pueden utilizarse para este fin partes de almacén pero no es lo lógico ni lo más cómodo para el usuario ya que no serán automáticos.

* Almacenes

o Se definen para cada centro

* Cuentas de tesorería

o Se definen para cada centro. Esto implica que la aplicación no permitirá usar a un usuario de un centro una cuenta de otro. Por otro lado si se permitirá en un centro grabar un asiento de tesorería de un documento relativo a otro centro, en este caso el programa avisa al usuario para evitar que haga la grabación por error pero la permite.

* Resto de archivos maestros y submaestros

o Son comunes a todos los centros

* Tarifas de venta

o Se definen por centros, lo que implica que un mismo producto en uno u otro centro pueda tener distintos precios de ventas e incluso, que un mismo cliente según compre en uno u otro centro tenga también un distinto precio.

* Documentos

o Están forzosamente separados por centros, cualquier tipo de documento exigirá como dato de cabecera su centro. Para este caso nos apoyamos en las “**series de documentos**” de manera que al dar de alta una serie en una distribución multicentro definimos su centro de trabajo ahorrando así el tener que especificar el centro cada vez que se grava un documento.

**Permisos / accesos**

El usuario administrador de la base de datos definirá los permisos de acceso por centros para cada perfil. Un perfil se corresponde con un tipo de usuario y por lo tanto se puede aplicar a uno o varios usuarios. Un mismo usuario no puede tener más de un perfil aplicado.

Esto implica que una vez asignado a un usuario su perfil y a éste su centro, al entrar en la aplicación no podrá ver, grabar ni hacer ningún tipo de modificación en documentos del otro centro.

Como excepción a esta regla están los usuarios administradores o gerentes a los que se les puede dar acceso a la base de datos general sin ninguna restricción por centro. Se hace simplemente asignándoles un perfil que no tenga aplicado un centro concreto. Este tipo de usuarios podrá listar, consultar, grabar y manipular documentos de cualquier centro

**Contabilidad**

Estando activada la distribución por centro podremos hacer una contabilización analítica, es decir, asignar a cada asiento de gastos o ingresos su centro de costes como dato añadido sin que intervengan para esto las cuentas contables.

La asignación se hace lógicamente definiendo en contabilidad centros de costes y en los centros de gestión definiremos su equivalente en contabilidad. A partir de ahí la aplicación generará automáticamente la contabilidad analítica.

Imaginemos por ejemplo un asiento de una venta: en la línea relativa a la cuenta de ingresos se recogerá la cuenta contable de ingresos definida para esa partida, que lógicamente es común a cualquier centro. El programa en el apunte del diario añadirá un campo más en el que especificaré al centro relativo al ingreso. De esta forma podremos calcular en contabilidad informes por centros (balances, cuentas de pérdidas y ganancias, desviaciones presupuestarias, etc...).
