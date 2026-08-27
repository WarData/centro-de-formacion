# Puesta en marcha + Configuración

### Activación webservice en Prestashop:

1. Habrá que ir al panel de administrador de la web de Prestashop > Parámetros avanzados > Webservice.
2. En este panel debe estar activo el check "Activar el servicio web"

<figure><img src="../../../../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

3. Seguido habrá que pulsar en "Añadir una nueva clase webservice"
   1. Generamos una clave, rellenamos la descripción con: Sincronización Tecnimoto-WMT con la web Prestashop y activaremos los permisos que requerimos:

<table data-search="false"><thead><tr><th>Recurso</th><th>Métodos</th></tr></thead><tbody><tr><td><strong>orders</strong> (Pedidos)</td><td>GET</td></tr><tr><td><strong>products</strong> (Artículos simples o padre)</td><td>GET, POST, PUT</td></tr><tr><td><strong>combinations</strong> (Artículos hijo)</td><td>GET, POST, PUT</td></tr><tr><td><strong>stock_availables</strong> (Stock)</td><td>GET, PUT</td></tr><tr><td><strong>manufacturers</strong> (Marcas)</td><td>GET</td></tr><tr><td><strong>categories</strong> (Categorías (artículo, vehículo, etc.))</td><td>GET</td></tr><tr><td><strong>product_options</strong> (Atributos: color, talla, modelo...)</td><td>GET</td></tr><tr><td><strong>product_option_values</strong> (Valores de atributos: rojo, XL, etc.)</td><td>GET</td></tr><tr><td><strong>product_features</strong> (Características)</td><td>GET</td></tr><tr><td><strong>product_feature_values</strong> (Valores de características)</td><td>GET</td></tr><tr><td><strong>customers</strong> (Clientes)</td><td>GET</td></tr><tr><td><strong>addresses</strong> (Direcciones de clientes)</td><td>GET</td></tr><tr><td><strong>images</strong> (Imágenes)</td><td>GET,POST,PUT</td></tr></tbody></table>

* Con esta configuración damos permisos para:
  * Consultar pedidos.
  * Consultar clientes y sus direcciones.
  * Consultar marcas, atributos, valores de atributos, características y categorías.
  * Crear y modificar productos y combinaciones.
  * Actualizar el stock de los productos.



### Puesta en marcha del módulo de pedidos (alta automática en Winmotor del pedido de la web).

* Usaremos un módulo externo (ps\_webhooks) para obtener los pedidos recién creados en Winmotor Para instalarlo hay que ir a la web de Prestashop: Módulos > Gestor de módulos > Subir el .zip en la web de Prestashop.
*   Ahora en Parámetros avanzados de la web saldrá la opción: Webhooks

    * Habrá que configurarlo:

    <figure><img src="../../../../../.gitbook/assets/image (4) (3).png" alt=""><figcaption></figcaption></figure>

    * \[Opcional] Activar proceso en API en Winmotor: PRE\_REC\_PED\_WEB
* Configurar serie por defecto en Parámetros > Web > Serie de pedido boutique. Habrá que rellenar el dato con alguna serie de pedido de ventas.
* Configurar apache en el servidor del cliente para que se pueda acceder al proceso PRE\_REC\_PED\_WEB (tendrá que estar SIEMPRE activo apache).
