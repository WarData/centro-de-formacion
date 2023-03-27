# Órdenes de Reparación

Mediante este menú, podremos grabar, modificar o consultar todas los ordenes de reparación que hemos realizado. Al entrar en ella, nos aparecen varios filtros con calendario, vehículo y cliente, por tipo de OR y por situación de la OR y de los recambios asociados a ella:

<figure><img src="../../../../.gitbook/assets/imagen (9) (1) (3).png" alt=""><figcaption></figcaption></figure>

Algo característico de los documentos orden de reparación son el campo [tipo de OR](../tipos-or.md), la situación de la OR y sus recambios y disponer de 4 a 5 (en Honda) imputaciones distintas como siniestro, cliente, garantía e interno. Los tipos de OR sirven tanto para identificar y clasificar las OR como para un alta más ligera, al permitir que, al indicar un tipo en el alta, se rellene automáticamente un tipo de imputación y un [tempario](../temparios.md).

* <mark style="color:orange;">Tipos de OR</mark>: [véase "Tipos de OR"](../tipos-or.md)
* <mark style="color:orange;">Situación de la OR</mark>:&#x20;
  * Inicialmente una OR se abre como "Pte. aceptar" o como "Presupuesto"
  * Confirmada en cualquier modo de apertura pasa a estado "En curso" y los repuestos asociados a ella podrán estar en situación "Pte. Recibir" para aquellos que no estaban en stock en el momento de confirmar la OR y han generado pedido de compras, "Pte. Instalar" para los recambios que estaban en stock y que han quedado reservados a la OR y "Pte. Recibir / Pte. Instalar" en aquellas ORs en las que se dan ambos casos
  * Sobre los artículos reservados en stock o que hayan sido recibidos (en azul - véase código de colores abajo) se puede realizar la instalación, seleccionado todas las líneas pulsando en el recuadro en blanco situado a la izquierda de "Almacén" o de una en una y pulsando en el botón "Instalar material", pasando las líneas instaladas a color verde.
  * Tras instalar la OR puede quedar "Pte. Facturar", "Facturada" y "Parc. Facturada" para aquellas aún sin facturar, facturadas y las que tienen más de una imputación y sólo se ha facturado una parte de ellas.

<figure><img src="../../../../.gitbook/assets/imagen (11) (1) (2).png" alt=""><figcaption></figcaption></figure>

* <mark style="color:orange;">Imputaciones estándar de la OR</mark>: <mark style="color:yellow;">indican hacia dónde va el cargo del conjunto de líneas incluidas en ella. Si se modifica la línea de la imputación, se modifica el conjunto de líneas:</mark>
  * Cliente: por defecto será el propietario del vehículo, pero se podrá modificar aunque siempre será hacia una entidad tipo cliente
  * Siniestro: permite el uso de la pestaña ["Versión para la compañía" - pulse para ver instrucciones de uso](../../../../faq/ordenes-de-reparacion-ors/version-para-la-compania-en-la-or.md)
  * Interna: el cargo irá a la empresa y habrá que especificar un departamento
  * Garantía: en función de la marca, las garantías que requieran una facturación de la mano de obra se podrán efectuar usando este tipo

