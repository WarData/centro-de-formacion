# Web - Documentación API REST

**Winmotor incorpora un API REST** de forma opcional que permite acceder vía HTTP al contenido de todas las tablas, procesos y búsquedas que existen en la aplicación y por supuesto, seleccionar únicamente aquellos a los que dar acceso.

**Disponer de esa tecnología significa que tu aplicación está abierta al mundo y permite a un desarrollador dar soluciones basadas en tu aplicación** y sus datos como:

* Aplicaciones para dispositivos móviles.
  * iOS
  * Android
  * Windows Mobile
  * iPadOS
* Aplicaciones web.
  * Tiendas online con Prestashop , Magento , WOOCommerce , etc usando sus APIs.
  * Conexión con plugins WordPress
  * Catálogos de productos, servicios, tarifas de precios y cualquier desarrollo que te puedas imaginar

## ¿Puedo usar esta API REST sin heredar o usar Velneo vERP? <a id="h.qgiu87q0crky"></a>

Sí, para hacerlo tendrás que integrar en tus proyectos los siguientes objetos que encontrarás en los proyectos de Velneo vERP. Lógicamente debes añadir los objetos del proyecto de datos en tu proyectos de datos y lo mismo con los de aplicación.

### Objetos a integrar del proyecto de datos vERP.dat <a id="objetos-a-integrar-del-proyecto-de-datos-verp-dat"></a>

#### Scripts <a id="scripts"></a>

![](https://gblobscdn.gitbook.com/assets%2F-M7D2zitZhY9szSsa5EK%2Fsync%2Fb114809f503e67d21f88a3fb6988581dde0c89df.png?alt=media)Captura de pantalla 2016-05-31 a las 9.29.26.png

Exportar la carpeta de script **js/api\_rest\_v1** que contiene los scripts:

* **api\_rest\_funciones\_v1.js**
* **swagger.js**
* **v1.js**

Se puede importar la carpeta directamente o bien cada uno de los scripts de forma individual. Lo verdaderamente importante es mantener la estructura de carpetas, es decir, que exista la carpeta js y dentro de esta la carpeta api\_rest\_v1 donde ubicaremos ambos scripts. De esta forma el resto de objetos que hacen referencia a estas ubicaciones serán operativos al pegarlos en nuestro proyecto sin necesidad de revisar sus propiedades.

Exportar el script **activarVista.js** que está incluido en la carpeta /js/interface/ e importarlo en nuestra aplicación en la misma estructura de carpetas. Este script es necesario para el control de vista activa del menú de API Keys.

#### Tablas <a id="tablas"></a>

![](https://gblobscdn.gitbook.com/assets%2F-M7D2zitZhY9szSsa5EK%2Fsync%2F6947488c360f9447cc65adea7087e64a97a72408.png?alt=media)

Carpeta Tablas/Configuración

* **API\_KEY\_W** \(API keys\)
* **API\_SEG\_W** \(API seguridad\)

#### Dibujos <a id="dibujos"></a>

![](https://gblobscdn.gitbook.com/assets%2F-M7D2zitZhY9szSsa5EK%2Fsync%2F3e46d10b7839db779c6472fe07073842df119e01.png?alt=media)Captura de pantalla 2016-05-31 a las 9.32.13.png

Carpeta Dibujos/Tablas/Configuración

* **API\_KEY\_W \(API keys\)**
* **API\_SEG\_W \(API seguridad\)**

#### Procesos <a id="procesos"></a>

![](https://gblobscdn.gitbook.com/assets%2F-M7D2zitZhY9szSsa5EK%2Fsync%2F7b0c6a9f0141b84824be9b517181bd9ad22561ec.png?alt=media)

Carpeta Procesos/API REST v1

* **SWAGGER**
* **API\_REST\_v1**

### Objetos a integrar del proyecto de aplicación vERP.app <a id="objetos-a-integrar-del-proyecto-de-aplicacion-verp-app"></a>

#### Carpetas con objetos de interfaz <a id="carpetas-con-objetos-de-interfaz"></a>

![](https://gblobscdn.gitbook.com/assets%2F-M7D2zitZhY9szSsa5EK%2Fsync%2Fc41296d43e1faf21d2ad8c670aea2a382a3445fd.png?alt=media)Captura de pantalla 2016-05-31 a las 9.34.39.png

Dentro de la carpeta Configuración copiar la carpeta API keys con todas sus subcarpetas.

#### Opción de menú para ejecutar la interfaz <a id="opcion-de-menu-para-ejecutar-la-interfaz"></a>

Para ejecutar la opción de menú que muestra la interfaz de API keys donde se define toda la seguridad debemos lanzar la acción **API\_KEY\_W\_MEN** es recomendable que esta opción sólo esté disponible para administradores o usuarios avanzados.Captura de pantalla 2016-05-31 a las 9.37.03.png

![](https://gblobscdn.gitbook.com/assets%2F-M7D2zitZhY9szSsa5EK%2Fsync%2Ffdf042a3cb810b90175a0ab311ee37228a5b73d8.png?alt=media)

![](https://gblobscdn.gitbook.com/assets%2F-M7D2zitZhY9szSsa5EK%2Fsync%2Fce668c6b1c514961c3b0e66991b1307f4a3cf66c.png?alt=media)

Guardar y reiniciar las instancias en el servidor.

## Ejecutar la aplicación y configurar la seguridad <a id="h.75wthxkvhxe"></a>

La seguridad del API REST está basada en 2 capas actualmente:

* Capa 1: clave API key.
* Capa 2: configuración de seguridad a nivel de tablas, campos, procesos y búsquedas.

La capa 1 consiste en una clave definible por el programador o el usuario en tiempo de ejecución que se configura desde el menú Supervisor -&gt; API keys.

![](https://gblobscdn.gitbook.com/assets%2F-M7D2zitZhY9szSsa5EK%2Fsync%2F8b44168ae28e5e2c6afbd95e9bc4245575fc0160.png?alt=media)

Al ejecutar esta opción se muestra el formulario de menú de API keys

![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-M7D2zitZhY9szSsa5EK%2Fsync%2F67eafe2c624ca2f45ad81dfda681c291083add25.png?generation=1589374147796469&alt=media)

Podemos crear tantos registros como queramos, en cada registro de API key debemos grabar una descripción y el valor de la clave del API key.

![](https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-M7D2zitZhY9szSsa5EK%2Fsync%2F5368d456eed6dbca3f5c780e572f3d6a9d623d23.png?generation=1589374147840072&alt=media)

En la pestaña seguridad del API key podremos generar tantos registros como tablas tenemos en nuestros proyectos de datos más un registro para los objetos poder configurar la seguridad de los procesos que no tienen tabla destino declarada.

![](https://gblobscdn.gitbook.com/assets%2F-M7D2zitZhY9szSsa5EK%2Fsync%2F1e58eb3ca2f75869a7d4faba1408b9b31db2dbd3.png?alt=media)

En el formulario se puede configurar con el check si es para procesos sin tabla destino, una vez marcado sólo nos aparecerá la pestaña de procesos.

En la parte superior izquierda tenemos 4 checks para configurar si este API key soporta los métodos GET, PUT, POST y DELETE.

En caso de no marcar el check sin tabla nos aparecerán 3 pestañas para configurar la seguridad de campos, procesos y búsquedas.

Para seleccionar un proceso, lo que debemos seleccionar en los combo boxes son el proyecto de datos donde está tabla de destino y la tabla de destino.

![](https://gblobscdn.gitbook.com/assets%2F-M7D2zitZhY9szSsa5EK%2Fsync%2F5c8ceaf5d52d878cbaf201e8a2735a3db70c5b39.png?alt=media)

En el caso de configurar una tabla debemos seleccionar un proyecto de datos de todos los cargados en ejecución y una vez seleccionado el proyecto podremos elegir la tabla sobre la que vamos a configurar la seguridad.

De igual modo podemos configurar en la parte superior derecha los métodos aceptados para dicha tabla \(GET, PUT, POST y DELETE\).

Las tres pestañas de seguridad de campos procesos y búsquedas tiene la misma funcionalidad y usabilidad.

Por defecto el API REST no permitirá devolver información de un campo, proceso o búsqueda que tengan marcado el estilo **privado**.

En la de campos tenemos un check que nos permite indicar si queremos que todos los campos de la tabla que no sean privados estén disponibles para el API. Conviene marcarlos si queremos que estén accesibles la mayoría de campos, en ese caso los campos que seleccionemos en la rejilla inferior serán excluidos del retorno de información que genere el API.

Los campos que devolverá el JSON al ejecutar el proceso son los que se marquen en la pestaña **campos** del API, que no hay que programar nada en el proceso.

Si queremos dejar accesible un número pequeño de campos es mejor no marcar el check y hacer la selección de los campos accesible. En definitiva lo que se trata es de seleccionar de la lista el menor número de elementos utilizando el check para dicho fin.

Los procesos y las búsquedas funcionan igual con un check que permite seleccionar todas excluyendo las seleccionadas o solo incluir las seleccionadas si no marcamos el check.

![](https://gblobscdn.gitbook.com/assets%2F-M7D2zitZhY9szSsa5EK%2Fsync%2F4a4d4832dacdffaa5afdd556c5c2dd8b011421bc.png?alt=media)

![](https://gblobscdn.gitbook.com/assets%2F-M7D2zitZhY9szSsa5EK%2Fsync%2F5bcd4f0108002472a1641b44a9649d2aec214e1a.png?alt=media)

## Instalar y configurar el componente vModApache <a id="h.bojc5dgs8ou"></a>

Para poder acceder al API REST se usa el componente vModApache que permite que el servidor web Apache pueda servir de forma automática la documentación swagger y el API REST de tu aplicación.

La instalación lleva mismos pasos que la instalación habitual de [vModApache](https://doc.velneo.com/velneo-vmodapache/que-es-velneo-vmodapache).

Es extremadamente importante que configures el Apache en HTTPS con un certificado. De esta forma evitas que la información http viaje en plano y sea accesible por terceros.

### Configuración del servidor Apache <a id="h.nb11uva66ni"></a>

Modificar el fichero D:\Apache24\conf\extra\httpd-ahssl.conf y añadir una directiva _location_ para conectarse a la instancia de la aplicación. Ejemplo:

```text
<Location /verp-api>    setHandler velneo    Vrl vatp://pepe:verp1234@c22.velneo.com:7050/VERP</Location>
```

### Reinicir el Apache <a id="h.mlvw29emk4"></a>

Una vez aplicadas las configuraciones, reiniciamos el servidor Apache.

### Probar el API desde Swagger <a id="probar-el-api-desde-swagger"></a>

#### ¿Qué es Swagger? <a id="que-es-swagger"></a>

Swagger es estándar para definir interfaces de API REST que permite que tanto personas como máquinas puedan entender y comprender las capacidades de un servicio sin acceder al código fuente o una documentación específica. Actualmente swagger forma parte de la especificación OpenApi.

El API REST de Velneo genera dinámicamente un fichero de definición swagger del API disponible en tu aplicación.

Para acceder Swagger usa la siguiente url:[Swagger UIdemoapi.velneo.com](https://demoapi.velneo.com/swagger/)

Si estás usando la versión anterior de la API rest, entonces has de usar esta otra URL:

​[https://demoapi.velneo.com/swagger\_old/](https://demoapi.velneo.com/swagger_old/)​

Verás que al cargar la página propone la url de acceso a la instancia web que tenemos de la demo de Velneo vERP \([https://demoapi.velneo.com/verp-api/vERP\_2\_dat\_dat/swagger](https://demoapi.velneo.com/verp-api/vERP_2_dat_dat/swagger)\) y nos pide que introduzcamos la APIKey. En el caso de la demo de vERP ésta es: api123

Así ya podrás comprobar cómo funciona.

Para poder ver una documentación vistosa de tu API, puedes introducir tu url de definición de Swagger en la URherramienta swagger ui.[http://petstore.swagger.io/](https://www.google.com/url?q=http://petstore.swagger.io/&sa=D&ust=1489485501837000&usg=AFQjCNFkClaochIeZIynVgsu8eriZJR-LQ), en la casilla superior y pulsar explorar. Si quieres acceder desde una red privada puedes descargar la herramienta swagger ui a tu ordenador y generar la documentación de tu API en local [https://github.com/swagger-api/swagger-ui](https://www.google.com/url?q=https://github.com/swagger-api/swagger-ui&sa=D&ust=1489485501838000&usg=AFQjCNGneyJTQcDBsU3Nkj0c4DQkFg_SOg)​

Desde swagger ui, no solamente puedes ver la documentación de la API, sino que podrás probar los distintos recursos y testear contra los datos reales de las aplicaciones.

Recuerda introducir el API key que has puesto en vERP en la página de Swagger UI para poder simular las mismas opciones que se puedan hacer con dichao API key.

**Doble factor de validación**

Tras mostrarse la interfaz de Swagger, es necesario conocer el nombre de la API y asignarla a la variable “api\_name”. Una vez comprobada su validez, se mostrarán los recursos disponibles y será necesaria la validación del “api\_key” para usarlos.

**Información del API Rest configurable**

Los texto que se muestran en la pantalla inicial del API Rest, son obtenidos de la pestaña “Comentarios” del proyecto.

Una vez validado con un api\_name, la información será sustituida por la que exista en las observaciones de la tabla del API.

**Información de las tablas configurable**

La información adicional mostrada en las tablas, procesos y/o búsquedas es obtenida desde el campo “Comentarios” de cada tabla.

**Métodos append, cross y delete para los filtros**

El filtrado por defecto realiza un _{cross}_ \(cruce de registros\). Por ejemplo, si filtramos por los artículos que contengan la palabra “cámara” y como segundo filtro le asignamos que la familia sea “A01”, nos devolverá las cámaras cuya familia sea A01.

​[https://midominio.velneo.net/verp-api/vERP\_2\_dat\_dat/v1/art\_m?fields=id,name,fam&filter\[words\]=camara&filter\[fam\]=A01&api\_key=apideejemplo](https://midominio.velneo.net/verp-api/vERP_2_dat_dat/v1/art_m?fields=id,name,fam&filter[words]=camara&filter[fam]=A01&api_key=apideejemplo)​

También es posible añdair registros en filtrado, usando el método _{add}._ Para que en el mismo ejemplo sume los registros que contengan la palabra cámara a los que contengan la familia A01, sería:

​[https://midominio.velneo.net/verp-api/vERP\_2\_dat\_dat/v1/art\_m?fields=id,name,fam&filter\[words\]=camara&filter\[fam{add}\]=A01&api\_key=apideejemplo](https://midominio.velneo.net/verp-api/vERP_2_dat_dat/v1/art_m?fields=id,name,fam&filter[words]=camara&filter[fam]=A01&api_key=apideejemplo)​

También es posible quitar registros en el filtrado, mediante el método _{delete}._ Para que en el mismo ejemplo quite los registros que contengan la familia A01 dejando solo los que contengan la palabra “cámara” y no sean de la familia A01.

​[https://midominio.velneo.net/verp-api/vERP\_2\_dat\_dat/v1/art\_m?fields=id,name,fam&filter\[words\]=camara&filter\[fam{delete}\]=A01&api\_key=apideejemplo](https://midominio.velneo.net/verp-api/vERP_2_dat_dat/v1/art_m?fields=id,name,fam&filter[words]=camara&filter[fam]=A01&api_key=apideejemplo)​

**Agrupamiento de recursos por** _**tags**_

Todos los recursos mostrados por el API Rest \(tablas con sus métodos, procesos y búsquedas\) son agrupado por nombre de tabla y pueden mostrarse y/o ocultarse.

**Interfaz**

La interfaz permite añadir mediante botones más usables los parámetros de búsqueda, nuevos botones para copiar la llamada y la respuesta del API, …

Ejemplos:

Url Swagger vERP Demo: \(clave api= api123\)

​[https://demoapi.velneo.com/swagger/](https://demoapi.velneo.com/swagger/)​

Url Swagger para el registro de tu propia documentación:

​[http://petstore.swagger.io/](http://petstore.swagger.io/)​

**Todos los artículos:**

​[https://demoapi.velneo.com/verp-api/vERP\_2\_dat\_dat/v1/art\_m?api\_key=api123](https://demoapi.velneo.com/verp-api/vERP_2_dat_dat/v1/art_m?api_key=api123)​

Todos los artículos pero mostrando los campos id, name, dsc:

​[https://demoapi.velneo.com/verp-api/vERP\_2\_dat\_dat/v1/art\_m?fields=id%2Cname%2Cdsc&api\_key=api123](https://demoapi.velneo.com/verp-api/vERP_2_dat_dat/v1/art_m?fields=id%2Cname%2Cdsc&api_key=api123)​

El artículo con id=1

​[https://demoapi.velneo.com/verp-api/](https://demoapi.velneo.com/verp-api/vERP_2_dat_dat/v1/art_m?filter[id]=1&api_key=api123)

[vERP\_2\_dat\_dat/v1/art\_m?filter%5Bid%5D=1&api\_key=api123](https://demoapi.velneo.com/verp-api/vERP_2_dat_dat/v1/art_m?filter[id]=1&api_key=api123)​

Los artículos con id 1, 3 y 5

​[https://demoapi.velneo.com/verp-api/vERP\_2\_dat\_dat/v1/art\_m?filter%5Bid%5D=1%2C%203%2C%205&api\_key=api123](https://demoapi.velneo.com/verp-api/vERP_2_dat_dat/v1/art_m?filter[id]=1%2C%203%2C%205&api_key=api123)​

Todos los clientes:

\[[https://demoapi.velneo.com/verp-api/vERP\_2\_dat\_dat/v1/ent\_m?api\_key=api123\]\(https://demoapi.velneo.com/verp-api/vERP\_2\_dat\_dat/v1/ent\_m?api\_key=ap](https://demoapi.velneo.com/verp-api/vERP_2_dat_dat/v1/ent_m?api_key=api123]%28https://demoapi.velneo.com/verp-api/vERP_2_dat_dat/v1/ent_m?api_key=ap)

{% hint style="info" %}
Si bien Swagger requiere [CORS](https://es.wikipedia.org/wiki/Intercambio_de_recursos_de_origen_cruzado) \(\(Cross-Origin-Resource-Sharing\) si usamos el API Rest de Velneo vERP no es necesario activarlo en Apache, pues las propias cabeceras de nuestra API Rest ya lo activan directamente.
{% endhint %}

[Enlace a Opciones Específicas](opciones-especificas/) \(API de [pedidos](opciones-especificas/api-de-pedidos.md) y [compras](opciones-especificas/api-de-compras.md)\)

