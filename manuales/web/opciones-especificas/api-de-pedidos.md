# API de pedidos

**GESTIÓN PEDIDOS DE VENTA A CLIENTES VIA API WINMOTOR**

**Recepción**

El proceso creará un pedido de venta sin confirmar. Una vez se confirme este, se crearán las reservas o pedidos a proveedor en caso de que no exista stock,

Se recibirá una URL con los siguientes parámetros:

* NIF: el nif del cliente. El pedido se creará sobre la entidad que tenga asignado este NIF. Si no existe ninguna no se creará. Parámetro obligatorio
* TIP\_PED: tipo de pedido, normal o garantía.
* LIN: en él se indica el contenido del pedido, todas las líneas. Este parámetro hay que pasarlo con las siguientes indicaciones:
  * Ejemplo1: LA3201017-155-XXL$4&gt;LA91000490$5&gt;LTlinea%20de%20texto
  * Ejemplo2: LAreferencia-articulo$unidades&gt;LAreferencia-articulo$unidades&gt;LTlinea%20de%20texto
    * Cada línea irá separada por el carácter &gt;
    * Hay dos tipos de línea, LA = línea de artículos o servicios y LT = línea de texto. Cada línea empezará siempre por LA o LT
    * Líneas LA: contiene siempre 2 campos
      1. Cada campo dentro de una línea irá separado por el carácter $
      2. El orden de los campos siempre será el mismo
         * Referencia: contiene la referencia del artículo o servicio
         * Unidades: cantidad que puede llevar un - en caso de ser negativa. Admite hasta 2 decimales
      3. En todos los campos numéricos, la parte decimal se separa por un punto, "."
      4. Si no se localiza el artículo se buscará en artículos tarifa y si aquí existe se crea automáticamente.
      5. Si no existe tampoco como artículo tarifa, se creará una línea de texto indicando en el concepto la referencia y demás campos leídos.
    * Líneas LT: contiene solo texto

Ejemplo de URL

[http://IPSERVIDOR/NOMBREINSTANCIA/dat\_winmotor\_dat/v1/\_process/REC\_PED\_API\_WA?param\[tip\_ped\]=pr&param\[lin\]=LAMO4T00024$2&param\[nif\]=X99999900&api\_key=1234](http://IPSERVIDOR/NOMBREINSTANCIA/vERP_2_dat_dat/v1/_process/REC_PED_API_WA?param%5btip_ped%5d=pr&param%5blin%5d=LAMO4T00024$2&param%5bnif%5d=X99999900&api_key=1234)

**Consultas**

Cabeceras de pedidos:

·         Ejemplo:

http://IPSERVIDOR/NOMBREINSTANCIA/vERP\_2\_dat\_dat/v1/\_query/ped\_x\_sit?param%5Bent%5D=8952&param%5Btip\_doc%5D=PV&fields=id%2Cfecha%2Ccod\_completo%2Centidad%2Cnombre%2Ccif%2Creferencia%2Cextension\_w7\_cd\_pe.sit.name&api\_key=win123

·         La url tiene los siguientes parámetros:

o   ent: id de la entidad

o   tip\_doc: hay que poner siempre PV, pedidos de venta

·         Esta url devuelve los campos que se definan en la configuración del API

Líneas de pedidos por cliente/nº pedido

·         Ejemplo:

[http://IPSERVIDOR/NOMBREINSTANCIA/vERP\_2\_dat\_dat/v1/\_process/lis\_ped\_cli?param\[nif\]=B99999999&param\[ped\]=999&api\_key=1234](http://IPSERVIDOR/NOMBREINSTANCIA/vERP_2_dat_dat/v1/_process/lis_ped_cli?param%5bnif%5d=B99999999&param%5bped%5d=999&api_key=1234)

·         La url tiene los siguientes parámetros:

o    nif: del cliente

o    ped: ID del pedido generado

·         Si no se le pasa el ID del pedido, devuelve todas las líneas de pedidos del cliente

Líneas de compras de un cliente \(pedidos ya entregados\):

·         Ejemplo:

[http://IPSERVIDOR/NOMBREINSTANCIA/vERP\_2\_dat\_dat/v1/\_query/lin\_est?param%5Bentidad%5D=33267&param%5Bfec\_fin%5D=31122020&param%5Bfec\_ini%5D=01012000&param%5Btipo\_doc%5D=AV&api\_key=win123](http://IPSERVIDOR/NOMBREINSTANCIA/vERP_2_dat_dat/v1/_query/lin_est?param%5Bentidad%5D=33267&param%5Bfec_fin%5D=31122020&param%5Bfec_ini%5D=01012000&param%5Btipo_doc%5D=AV&api_key=win123)

·         La url tiene los siguientes parámetros:

o   entidad: id de la entidad

o    fec\_fin: fecha hasta la que se buscan líneas de documentos. Se representa la fecha 01012000 \(1 enero 2000\)

o    fec\_ini: fecha desde la que se buscan líneas de documentos

o    tip\_doc: hay que poner siempre AV, albaranes de venta

