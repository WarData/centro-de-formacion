---
description: >-
  Para casos en los que la base de datos maneja un gran número de marcas existe
  un sistema para facilitar la consulta de éstas en el cuadro de mandos.
---

# Clasificadores de marcas

En el panel del cuadro de mandos aparece ahora un nuevo botón “Clasificadores” junto al botón “Actualizar”, al pulsarlo entramos en la gestión de los clasificadores de marcas.

El primer paso a dar será crear clasificadores para las marcas según las queramos ver en la vista general del cuadro de mandos (dentro de la vista por centros no hemos cambiado nada). En el ejemplo hemos creado marcas para Motos, Recambios, Boutique, Bicicletas y Varios.

![](<../../.gitbook/assets/imagen (104).png>)

El siguiente paso será asignar a todas las marcas que gestionamos en la base de datos uno de estos clasificadores para lo que hemos dotado a este panel de una serie de herramientas.

1\.       **Ver Marcas sin clasificador**: nos mostrará todas aquellas a las que aún no hemos asignado ningún clasificador. Al pulsarlo en nuestro ejemplo han aparecido las siguientes

![](<../../.gitbook/assets/imagen (110).png>)

2\.       **Asignar clasificador**: seleccionamos las marcas que queramos y pulsando este botón el programa nos preguntará cuál de los clasificadores creados queremos asignarles- para el ejemplo las vamos a pasar a “Motos”. También podemos lógicamente utilizar este botón para marcas que ya tienen clasificador con lo que simplemente se lo modificamos.

Una vez hemos asignado clasificadores a todas las marcas cuando se calcule un cuadro de mandos el resultado será este:

![](<../../.gitbook/assets/imagen (112).png>)

Después de los centros aparecerán los distintos clasificadores creados y dentro de cada uno de ellos las marcas asignadas. Si pinchamos en uno de los clasificadores se abrirá para presentar sus marcas, pero no se han calculado para ellos resultados, sólo actúan como clasificadores, no como totalizadores.

El número de clasificadores que se pueden crear es ilimitado e incluso se pueden anidar ya que está montado con una estructura arbolada. En el ejemplo se puede ver que hemos asignado a Boutique el código “BOU”; podemos crear subclasificadores dentro de estos con el criterio de siempre en Winmotor, jugando con el código. Si creamos BOU-ROP para ropa y BOU-CAS para cascos es cuestión luego de asignar cada marca a uno de éstos y los podremos luego consultar por separado.

El tamaño máximo del clasificador es de 8 caracteres por lo que utilizando códigos de tres dígitos sólo podremos hacer dos ramas: en caso de querer hacer más ramas será cuestión de utilizar una codificación con menos dígitos.
