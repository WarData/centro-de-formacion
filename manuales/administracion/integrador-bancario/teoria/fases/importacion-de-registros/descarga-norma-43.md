# Descarga norma 43

* Esta descarga aporta mucha más información al sistema en cuanto al tipo de movimiento bancario, pero sólo se puede hacer al día siguiente de la fecha de la operación. Al hacer esta descarga el programa conocerá dos datos fundamentales:
  * Concepto común: es un código de clasificación del movimiento que viene determinado por el consejo superior bancario que aunque algo anticuado aporta información sobre el mismo.
    * Puedes consultar la lista de estos conceptos en el menú del integrador en la opción “Conceptos comunes - Norma 43”.
    * Inexplicablemente algunos bancos como el BSCH no aportan este dato, lo rellenan siempre con ceros.
  * Concepto propio: es una codificación interna que hace cada entidad mucho más amplia y detallada que el concepto común y que no deja duda en cuanto al tipo de movimiento descargado.
* Estos campos los podrá ver en el registro descargado siempre que lo consulte al día siguiente de su “Fecha de operación”.
* La mayoría de entidades no tienen activo este sistema por defecto, hay que solicitar su activación. En algunos casos lleva a engaño que en la consulta de movimientos en la página del banco aparece como opción “Norma 43” pero no hace una descarga real en este formato, simplemente nos da un Excel con los campos que se ven al descargar la norma 43.
