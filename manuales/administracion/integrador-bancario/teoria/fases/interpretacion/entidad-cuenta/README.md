# Entidad / cuenta

Para los tipos de movimientos que están vinculados con documentos de la aplicación el integrador tiene primero que localizar la entidad. Los tipos de movimientos que requieren una entidad son:

● <mark style="color:red;">Gastos</mark>

* Devolución a cliente
* Pago a empleado (Nómina)
* Pago a proveedor - acreedor

● <mark style="color:green;">Ingresos</mark>

* Cobro a cliente
* Devolución a proveedor

Para esta identificación cuenta con el contenido del campo “descripción” que el banco ha aportado. Dado que muchas veces se hace complicado identificar la entidad hay varios sistemas que ayudan al programa a hacerlo y los estudiaremos en el siguiente bloque. Si es importante entender que el integrador utiliza todos los datos que están a su alcance en la base de datos para identificar cada campo. Si por ejemplo tenemos un cobro y la entidad localizada no tiene marcado que es cliente pero si proveedor o acreedor, el integrador interpretará automáticamente que se trata de un abono a proveedor y buscará facturas recibidas de abono.

