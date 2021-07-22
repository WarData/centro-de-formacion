# API de compras

**RECEPCIÓN ALBARANES DE COMPRA VIA API WINMOTOR**

  
Montado nuevo sistema para la recepción de albaranes de compra via API WINMOTOR. 

El proceso creará un albarán de compra en modo borrador. Una vez se confirme este, se crearán las reparticiones pertinentes. Se ha querido montar así para que de forma asistida el usuario pueda editar estas reparticiones y/o gestionar los avisos a los clientes o taller.

Se recibirá una URL con los siguientes parámetros:

* CIF: el CIF del proveedor. El albarán se creará sobre la entidad que tenga asignado este CIF. Si no existe ninguna no se creará el albarán. Parámetro obligatorio
* REF\_SER\_AC: la referencia de la serie de albarán de compra que se creará. Tampoco se creará el albarán si la referencia no existe. Parámetro obligatorio
* FEC: fecha del albarán. El formato será siempre ddmmaaaa \(día completo, mes completo, año completo\). Parámetro obligatorio
* REF\_AC: referencia que el proveedor le ha dado al albarán. Este parámetro NO es obligatorio. Si se rellena, no se podrá crear un albarán para el mismo proveedor con el mismo nº. De esta forma se controla que no se pueda importar dos veces el mismo albarán
* LIN: en él se indica el contenido del albarán, todas las líneas. Este parámetro hay que pasarlo con las siguientes indicaciones:
  * Cada línea irá separada por el carácter &gt;
  * Hay dos tipos de línea, LA = línea de artículos o servicios y LT = línea de texto. Cada línea empezará siempre por LA o LT
  * Líneas LA: contiene siempre obligatoriamente 5 campos
    * Cada campo dentro de una línea irá separada por el carácter $
    * El orden de los campos siempre será el mismo
      1. Referencia: contiene la referencia del artículo o servicio
      2. Unidades: cantidad que puede llevar un - en caso de ser negativa. Admite hasta 2 decimales
      3. Precio: precio unitario del producto. Siempre será positivo. Admite hasta 4 decimales
      4. Descuento 1. Admite hasta 2 decimales
      5. Descuento 2. Admite hasta 2 decimales
    * En todos los campos numéricos, la parte decimal se separa por un punto, "."
    * Si no se localiza el artículo se buscará en artículos tarifa y si aquí existe se crea automáticamente.
    * Si no existe tampoco como artículo tarifa, se creará una línea de texto indicando en el concepto la referencia y demás campos leídos.
  * Líneas LT: contiene solo texto

Ejemplo de URL

[http://IPSERVIDOR/NOMREINSTANCIA/vERP\_2\_dat\_dat/v1/\_process/REC\_AC\_API\_WA?param\[REF\_SER\_AC\]=ACBV&param\[FEC\]=28032019&param\[REF\_AC\]=ZZ234799&param\[CIF\]=B99999998&param\[lin\]=LTTEXTO&gt;LA2654604-Y22-52$5$330.9900$25.15$00.00&gt;LA1654580-U40-58$1$10.9900$25.15$5.00&gt;LTOTRA&gt;LA2654604-Y22-11111$5$330.9900$25.15$00.00&api\_key=123ABC](http://IPSERVIDOR/NOMREINSTANCIA/vERP_2_dat_dat/v1/_process/REC_AC_API_WA?param%5bREF_SER_AC%5d=ACBV&param%5bFEC%5d=28032019&param%5bREF_AC%5d=ZZ234799&param%5bCIF%5d=B99999998&param%5blin%5d=LTTEXTO%3eLA2654604-Y22-52$5$330.9900$25.15$00.00%3eLA1654580-U40-58$1$10.9900$25.15$5.00%3eLTOTRA%3eLA2654604-Y22-11111$5$330.9900$25.15$00.00&api_key=123ABC)

 En la anterior URL hay 5 líneas:

1. LTTEXTO
2. LA2654604-Y22-52$5$330.9900$25.15$00.00
3. LA1654580-U40-58$1$10.9900$25.15$5.00
4. LTOTRA
5. LA2654604-Y22-11111$5$330.9900$25.15$00.00

La 1 y 4 son líneas de texto, el resto líneas de artículo.

