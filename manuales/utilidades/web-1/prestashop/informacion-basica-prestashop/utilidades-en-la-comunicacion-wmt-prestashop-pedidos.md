# Utilidades en la comunicación WMT-Prestashop (Pedidos)

## Alta de pedidos creados en la web

<figure><img src="../../../../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

#### ¿Qué hace este proceso?

Cuando un cliente realiza un pedido en la tienda online (PrestaShop), ese pedido se da de alta automáticamente en Winmotor, sin que nadie tenga que introducirlo a mano.

#### ¿Cómo se dispara?

La propia tienda online avisa a Winmotor en el momento en que se crea un pedido, enviándole toda la información necesaria. Winmotor recibe ese aviso y hace el resto del trabajo automáticamente.

#### ¿Qué pasos sigue?

1. Identifica al cliente. Busca en Winmotor a qué cliente corresponde el pedido, primero por su DNI/NIF y, si no lo encuentra, por su email o su nombre.
2. Comprueba que no esté duplicado. Si ese mismo pedido ya se había recibido antes, no se vuelve a crear.
3. Crea el pedido. Da de alta la cabecera del pedido en Winmotor, asociada al cliente encontrado.
4. Añade los productos. Por cada artículo del pedido, busca ese producto en el ERP y lo añade con su cantidad y precio. Si algún producto no se localiza, se añade igualmente como anotación de texto, para que se pueda revisar a mano.
5. Deja constancia de lo ocurrido. Se guarda un registro de log de cada pedido recibido, tanto si se ha dado de alta correctamente como si ha habido algún problema.

#### ¿Qué debe estar bien configurado para que funcione?

**En la tienda online:**

* El cliente debe rellenar su DNI/NIF al hacer el pedido. Al menos su cuenta de correo o nombre. No está contemplado que se cree la entidad en Winmotor si no existe en el programa dicho cliente.
* Cada producto debe tener correctamente puesta su referencia y debe concordar con la de Winmotor.

**En Winmotor:**

* Debe tener acceso configurado a la tienda online (para poder consultar los datos del cliente). Esto quiere decir que debe estar configurado Apache en el servidor para la recepción de la información de la web.
* Debe tener definida una serie por defecto donde se crean estos pedidos (Configuración > Parámetros > Web > Serie pedido boutique).
