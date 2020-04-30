---
description: Ejemplo básico y avanzado de uso
---

# Mailing - Cómo funciona y trucos para sacarle partido

La opción "Mailing" incluida en Winmotor \(en función del número de módulos también puede estar dentro de "Comunicaciones"\) permite el envío de emails a determinadas entidades, mediante el uso de filtros y desde varias localizaciones.

Vamos a ver la primera localización donde podremos configurar un Mailing:

![](../.gitbook/assets/image%20%28139%29.png)

Desde el panel de Mailings aperturamos uno nuevo, obteniendo una imagen similar a la de arriba. Aquí podremos configurar todos los datos necesarios como el asunto, desde qué cuenta enviaremos el email, destinatarios, archivos adjuntos, etc...

En la opción "Formato de envío", el mailing nos permite hacer un envío con texto genérico para todas las entidades \(modo libre\) o personalizar para cada entidad la cabecera \(modo personalizado\). Ejemplo: Estimado cliente, o Estimado "nombre de entidad".

En tipo de envío, nos permitirá enviar el mailing por diferentes métodos, por email, SMS e incluso comprobando si la entidad no tiene mail enviarlo por el móvil disponible \(calculado\).

En el cuerpo del mensaje podremos incluir el texto que queramos o incluso un código HTML que primero tendrá que estar alojado en un servidor web para poder mostrar el contenido: 

> "&lt;IMG SRC=\``direccion_web/archivo_imagen.jpg`´&gt;"
>
> &lt;br&gt; son espacio en blanco
>
> El contenido completo lo introduciremos en el editor del contenido dinámico para que nos presente todo como código HTML y lo ejecute en el email, **siendo fundamental:**
>
> * **Comillas dobles al principio y al final del código HTML " "**
> * **Comillas simples para todo el contenido ' '**
>
> Os mostramos un ejemplo real sobre nuestra felicitación de navidad 2019:

![](../.gitbook/assets/image%20%28282%29.png)

En la pestaña "Destinatarios" haciendo doble clic podremos añadir entidades una a una, más abajo podremos obtener el listado completo de entidades usado en anteriores mailings \(botón inferior "Importar destinatarios desde otro mailing\) y otra forma es directamente desde listados:

![](../.gitbook/assets/image%20%28342%29.png)

Desde los listados, como por ejemplo desde "Maestros" &gt; "Entidades" &gt; podemos crear directamente con las entidades filtradas un nuevo mailing o añadir las entidades seleccionadas a uno existente, al cual podremos añadir más de forma manual como en la imagen anterior:

![](../.gitbook/assets/image%20%28195%29.png)

Como extra, si en esta misma pantalla pulsamos en F3 - Listar Entidades, podremos filtrar aún más y de forma más definida el listado que queremos obtener para enviar el mailing:

![](../.gitbook/assets/image%20%28284%29.png)

En filtros avanzados definimos aún más, llegando a poder definir tipo de cliente, si tiene o no email, etc...:

![](../.gitbook/assets/image%20%2844%29.png)

Una vez añadidos los destinatarios, posibles archivos adjuntos y cuerpo del mensaje, al enviar, desde esta pestaña podremos controlar a quien se le ha podido enviar correctamente y a quien no:

![](../.gitbook/assets/image%20%2825%29.png)

\*\*\* Existen numerosos programas para crear plantillas HTML para mailings como MailStyler 2 con los que obtendremos el código y los ficheros de imágenes que tendremos que poner en una Web para poder acceder desde cualquier punto a ellas.

Un ejemplo con MailStyler sería este:

![](../.gitbook/assets/image%20%28418%29.png)

El código a introducir cuando hayamos subido las imágenes que obtenemos en una carpeta \_files al exportar a HTML al editor personalizado de Winmotor - Mailings:

{% code title="Ejemplo para Mailing sobre Blog" %}
```text
"<!DOCTYPE html PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN' 'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
<html xmlns='http://www.w3.org/1999/xhtml' xmlns:v='urn:schemas-microsoft-com:vml' xmlns:o='urn:schemas-microsoft-com:office:office'>
<head>
<meta http-equiv='Content-Type' content='text/html; charset=utf-8' />
<meta name='x-apple-disable-message-reformatting' />
<meta name='viewport' content='width=device-width, initial-scale=1.0' />
<style type='text/css'>
    body, .maintable { height:100% !important; width:100% !important; margin:0; padding:0;}
    img, a img { border:0; outline:none; text-decoration:none;}
    p {margin-top:0; margin-right:0; margin-left:0; padding:0;}
    .ReadMsgBody {width:100%;}
    .ExternalClass {width:100%;}
    .ExternalClass, .ExternalClass p, .ExternalClass span, .ExternalClass font, .ExternalClass td, .ExternalClass div {line-height:100%;}
    img {-ms-interpolation-mode: bicubic;}
    body, table, td, p, a, li, blockquote {-ms-text-size-adjust:100%; -webkit-text-size-adjust:100%;}
</style>
<style type='text/css'>
@media only screen and (max-width: 480px) {
 .rtable {width: 100% !important;}
 .rtable tr {height:auto !important; display: block;}
 .contenttd {max-width: 100% !important; display: block; width: auto !important;}
 .contenttd:after {content: ''; display: table; clear: both;}
 .hiddentds {display: none;}
 .imgtable, .imgtable table {max-width: 100% !important; height: auto; float: none; margin: 0 auto;}
 .imgtable.btnset td {display: inline-block;}
 .imgtable img {width: 100%; height: auto !important;display: block;}
 table {float: none;}
 .mobileHide {display: none !important;}
}
</style>
<!--[if gte mso 9]>
<xml>
  <o:OfficeDocumentSettings>
    <o:AllowPNG/>
    <o:PixelsPerInch>96</o:PixelsPerInch>
  </o:OfficeDocumentSettings>
</xml>
<![endif]-->
<title></title>
</head>
<body style='overflow: auto; padding:0; margin:0; font-size: 14px; font-family: arial, helvetica, sans-serif; cursor:auto; background-color:#feffff'>
<table cellspacing='0' cellpadding='0' width='100%' bgcolor='#feffff'>
<tr>
<td style='FONT-SIZE: 0px; HEIGHT: 0px; LINE-HEIGHT: 0'></td>
</tr>
<tr>
<td valign='top'>
<table class='rtable' style='WIDTH: 600px; MARGIN: 0px auto' cellspacing='0' cellpadding='0' width='600' align='center' border='0'>
<tr>
<th class='contenttd' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 600px; BORDER-BOTTOM: medium none; FONT-WEIGHT: normal; PADDING-BOTTOM: 0px; TEXT-ALIGN: left; PADDING-TOP: 0px; PADDING-LEFT: 0px; BORDER-LEFT: medium none; PADDING-RIGHT: 0px; BACKGROUND-COLOR: #f0f0ef'>
<table style='WIDTH: 100%' cellspacing='0' cellpadding='0' align='left'>
<tr style='HEIGHT: 106px' height='106'>
<th class='contenttd' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 207px; VERTICAL-ALIGN: top; BORDER-BOTTOM: medium none; FONT-WEIGHT: normal; PADDING-BOTTOM: 0px; TEXT-ALIGN: left; PADDING-TOP: 0px; PADDING-LEFT: 10px; BORDER-LEFT: medium none; PADDING-RIGHT: 10px; BACKGROUND-COLOR: #f2f2f2'><!--[if gte mso 12]>
    <table cellspacing='0' cellpadding='0' border='0' width='100%'><tr><td align='center'>
<![endif]-->
<table class='imgtable' style='MARGIN: 0px auto' cellspacing='0' cellpadding='0' align='center' border='0'>
<tr>
<td style='PADDING-BOTTOM: 10px; PADDING-TOP: 10px; PADDING-LEFT: 10px; PADDING-RIGHT: 10px' align='center'>
<table cellspacing='0' cellpadding='0' border='0'>
<tr>
<td style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; BORDER-BOTTOM: medium none; BORDER-LEFT: medium none; BACKGROUND-COLOR: transparent'><img style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; BORDER-BOTTOM: medium none; BORDER-LEFT: medium none; DISPLAY: block' alt='' src='https://www.winmotor.net/wp-content/uploads/2019/09/Image_1_711066fd4f604f4d8aa2a3a3d7d417fb.png' width='187' hspace='0' vspace='0' /></td>
</tr>
</table>
</td>
</tr>
</table>
<!--[if gte mso 12]>
    </td></tr></table>
<![endif]--></th>
<th class='contenttd' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 353px; VERTICAL-ALIGN: bottom; BORDER-BOTTOM: medium none; FONT-WEIGHT: normal; PADDING-BOTTOM: 10px; TEXT-ALIGN: left; PADDING-TOP: 10px; PADDING-LEFT: 10px; BORDER-LEFT: medium none; PADDING-RIGHT: 10px; BACKGROUND-COLOR: transparent'>
<p style='FONT-SIZE: 18px; MARGIN-BOTTOM: 1em; FONT-FAMILY: arial, helvetica, sans-serif; MARGIN-TOP: 0px; COLOR: #ff7533; TEXT-ALIGN: center; LINE-HEIGHT: 22px; BACKGROUND-COLOR: transparent; mso-line-height-rule: exactly' align='center'><strong>SOFTWARE WINMOTOR - BOLET&Iacute;N INFORMATIVO SOBRE BLOG INCLUIDO EN WINMOTOR V7</strong></p>
</th>
</tr>
</table>
</th>
</tr>
<tr>
<th class='contenttd' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 600px; BORDER-BOTTOM: medium none; FONT-WEIGHT: normal; PADDING-BOTTOM: 0px; TEXT-ALIGN: left; PADDING-TOP: 0px; PADDING-LEFT: 0px; BORDER-LEFT: medium none; PADDING-RIGHT: 0px; BACKGROUND-COLOR: #f0f0ef'>
<table style='WIDTH: 100%' cellspacing='0' cellpadding='0' align='left'>
<tr style='HEIGHT: 338px' height='338'>
<th class='contenttd' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 600px; VERTICAL-ALIGN: top; BORDER-BOTTOM: medium none; FONT-WEIGHT: normal; PADDING-BOTTOM: 0px; TEXT-ALIGN: left; PADDING-TOP: 0px; PADDING-LEFT: 0px; BORDER-LEFT: medium none; PADDING-RIGHT: 0px; BACKGROUND-COLOR: transparent'><!--[if gte mso 12]>
    <table cellspacing='0' cellpadding='0' border='0' width='100%'><tr><td align='center'>
<![endif]-->
<table class='imgtable' style='MARGIN: 0px auto' cellspacing='0' cellpadding='0' align='center' border='0'>
<tr>
<td style='PADDING-BOTTOM: 0px; PADDING-TOP: 0px; PADDING-LEFT: 0px; PADDING-RIGHT: 0px' align='center'>
<table cellspacing='0' cellpadding='0' border='0'>
<tr>
<td style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; BORDER-BOTTOM: medium none; BORDER-LEFT: medium none; BACKGROUND-COLOR: transparent'><img style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; BORDER-BOTTOM: medium none; BORDER-LEFT: medium none; DISPLAY: block' alt='' src='https://www.winmotor.net/wp-content/uploads/2019/09/Image_2_e0b9a1baaaf348cca2620bff3663814d.png' width='600' hspace='0' vspace='0' /></td>
</tr>
</table>
</td>
</tr>
</table>
<!--[if gte mso 12]>
    </td></tr></table>
<![endif]--></th>
</tr>
</table>
</th>
</tr>
<tr>
<th class='contenttd' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 600px; BORDER-BOTTOM: medium none; FONT-WEIGHT: normal; PADDING-BOTTOM: 20px; TEXT-ALIGN: left; PADDING-TOP: 10px; PADDING-LEFT: 0px; BORDER-LEFT: medium none; PADDING-RIGHT: 0px; BACKGROUND-COLOR: #50688d'>
<table style='WIDTH: 100%' cellspacing='0' cellpadding='0' align='left'>
<tr style='HEIGHT: 297px' height='297'>
<th class='contenttd' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 580px; VERTICAL-ALIGN: top; BORDER-BOTTOM: medium none; FONT-WEIGHT: normal; PADDING-BOTTOM: 20px; TEXT-ALIGN: left; PADDING-TOP: 10px; PADDING-LEFT: 10px; BORDER-LEFT: medium none; PADDING-RIGHT: 10px; BACKGROUND-COLOR: transparent'>
<p style='FONT-SIZE: 36px; MARGIN-BOTTOM: 1em; FONT-FAMILY: geneve, arial, helvetica, sans-serif; MARGIN-TOP: 0px; COLOR: #fefffe; TEXT-ALIGN: center; LINE-HEIGHT: 45px; mso-line-height-rule: exactly' align='center'>Actualizaci&oacute;n Winmotor V7 - 19-8-1</p>
<p style='FONT-SIZE: 18px; MARGIN-BOTTOM: 1em; FONT-FAMILY: arial, helvetica, sans-serif; MARGIN-TOP: 0px; COLOR: #fefffe; TEXT-ALIGN: center; LINE-HEIGHT: 30px; BACKGROUND-COLOR: transparent; mso-line-height-rule: exactly' align='center'>La nueva actualizaci&oacute;n que se est&aacute; incorporando por fases a todos los clientes de Winmotor V7, incorpora muchas novedades, funciones y sistemas de ayuda como el Blog Winmotor integrado (winmotor.blog) y la barra de Favoritos.</p>
<!--[if gte mso 12]>
    <table cellspacing='0' cellpadding='0' border='0' width='100%'><tr><td align='center'>
<![endif]-->
<table class='imgtable btnset' style='TEXT-ALIGN: center; MARGIN: 0px auto' cellspacing='0' cellpadding='0' border='0'>
<tr>
<td class='contenttd' style='VERTICAL-ALIGN: middle; PADDING-BOTTOM: 0px; PADDING-TOP: 0px; PADDING-LEFT: 0px; PADDING-RIGHT: 0px'><a href='http://www.winmotor.blog/' target='_blank'><img title='Blog Winmotor' border='none' alt='Visita el Blog' src='https://www.winmotor.net/wp-content/uploads/2019/09/Image_3_a73a33d550e74b3ea8deb64dce060758.png' /></a> </td>
</tr>
</table>
<!--[if gte mso 12]>
    </td></tr></table>
<![endif]--></th>
</tr>
</table>
</th>
</tr>
<tr>
<th class='contenttd' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 600px; BORDER-BOTTOM: medium none; FONT-WEIGHT: normal; PADDING-BOTTOM: 20px; TEXT-ALIGN: left; PADDING-TOP: 10px; PADDING-LEFT: 0px; BORDER-LEFT: medium none; PADDING-RIGHT: 0px; BACKGROUND-COLOR: #f0f0ef'>
<table style='WIDTH: 100%' cellspacing='0' cellpadding='0' align='left'>
<tr style='HEIGHT: 462px' height='462'>
<th class='contenttd' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 280px; VERTICAL-ALIGN: top; BORDER-BOTTOM: medium none; FONT-WEIGHT: normal; PADDING-BOTTOM: 10px; TEXT-ALIGN: left; PADDING-TOP: 10px; PADDING-LEFT: 10px; BORDER-LEFT: medium none; PADDING-RIGHT: 10px; BACKGROUND-COLOR: transparent'>
<p style='FONT-SIZE: 24px; MARGIN-BOTTOM: 1em; FONT-FAMILY: geneve, arial, helvetica, sans-serif; MARGIN-TOP: 0px; COLOR: #50688d; TEXT-ALIGN: left; LINE-HEIGHT: 30px; BACKGROUND-COLOR: transparent; mso-line-height-rule: exactly' align='left'>Categor&iacute;as y B&uacute;squeda</p>
<!--[if gte mso 12]>
    <table cellspacing='0' cellpadding='0' border='0' width='100%'><tr><td align='center'>
<![endif]-->
<table class='imgtable' style='MARGIN: 0px auto' cellspacing='0' cellpadding='0' align='center' border='0'>
<tr>
<td style='PADDING-BOTTOM: 15px; PADDING-TOP: 0px; PADDING-LEFT: 0px; PADDING-RIGHT: 0px' align='center'>
<table cellspacing='0' cellpadding='0' border='0'>
<tr>
<td style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; BORDER-BOTTOM: medium none; BORDER-LEFT: medium none; BACKGROUND-COLOR: transparent'><img style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; BORDER-BOTTOM: medium none; BORDER-LEFT: medium none; DISPLAY: block' alt='' src='https://www.winmotor.net/wp-content/uploads/2019/09/Image_4_5205e6a6909f4403a46935ec7266d996.jpg' width='280' hspace='0' vspace='0' /></td>
</tr>
</table>
</td>
</tr>
</table>
<!--[if gte mso 12]>
    </td></tr></table>
<![endif]-->
<p style='FONT-SIZE: 14px; MARGIN-BOTTOM: 1em; FONT-FAMILY: arial, helvetica, sans-serif; MARGIN-TOP: 0px; COLOR: #283548; TEXT-ALIGN: left; LINE-HEIGHT: 23px; BACKGROUND-COLOR: transparent; mso-line-height-rule: exactly' align='left'>En el lateral derecho del Blog integrado pod&eacute;is usar la b&uacute;squeda por palabra o por categor&iacute;as. Peri&oacute;dicamente iremos incorporando noticias, novedades y todo lo que os pueda interesar sobre Winmotor V7, as&iacute; como temas que nos indiqu&eacute;is.</p>
<!--[if gte mso 12]>
    <table cellspacing='0' cellpadding='0' border='0' width='100%'><tr><td align='right'>
<![endif]-->
<table class='imgtable btnset' style='TEXT-ALIGN: right; MARGIN-LEFT: auto; MARGIN-RIGHT: 0px' cellspacing='0' cellpadding='0' border='0'>
<tr>
<td class='contenttd' style='VERTICAL-ALIGN: middle; PADDING-BOTTOM: 0px; PADDING-TOP: 0px; PADDING-LEFT: 0px; PADDING-RIGHT: 0px'><a href='http://www.winmotor.blog/' target='_blank'><img title='Blog' border='none' alt='Blog Winmotor' src='https://www.winmotor.net/wp-content/uploads/2019/09/Image_5_21f5e615f8c54f958de912f46d5480fd.png' /></a> </td>
</tr>
</table>
<!--[if gte mso 12]>
    </td></tr></table>
<![endif]--></th>
<th class='contenttd' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 280px; VERTICAL-ALIGN: top; BORDER-BOTTOM: medium none; FONT-WEIGHT: normal; PADDING-BOTTOM: 10px; TEXT-ALIGN: left; PADDING-TOP: 10px; PADDING-LEFT: 10px; BORDER-LEFT: medium none; PADDING-RIGHT: 10px; BACKGROUND-COLOR: transparent'>
<p style='FONT-SIZE: 24px; MARGIN-BOTTOM: 1em; FONT-FAMILY: geneve, arial, helvetica, sans-serif; MARGIN-TOP: 0px; COLOR: #50688d; TEXT-ALIGN: left; LINE-HEIGHT: 30px; BACKGROUND-COLOR: transparent; mso-line-height-rule: exactly' align='left'>Centro de Ayuda</p>
<!--[if gte mso 12]>
    <table cellspacing='0' cellpadding='0' border='0' width='100%'><tr><td align='center'>
<![endif]-->
<table class='imgtable' style='MARGIN: 0px auto' cellspacing='0' cellpadding='0' align='center' border='0'>
<tr>
<td style='PADDING-BOTTOM: 15px; PADDING-TOP: 0px; PADDING-LEFT: 0px; PADDING-RIGHT: 0px' align='center'>
<table cellspacing='0' cellpadding='0' border='0'>
<tr>
<td style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; BORDER-BOTTOM: medium none; BORDER-LEFT: medium none; BACKGROUND-COLOR: transparent'><img style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; BORDER-BOTTOM: medium none; BORDER-LEFT: medium none; DISPLAY: block' alt='' src='https://www.winmotor.net/wp-content/uploads/2019/09/Image_6_9cee99d5df4c49f1a11baf7c961dfe44.jpg' width='280' hspace='0' vspace='0' /></td>
</tr>
</table>
</td>
</tr>
</table>
<!--[if gte mso 12]>
    </td></tr></table>
<![endif]-->
<p style='FONT-SIZE: 14px; MARGIN-BOTTOM: 1em; FONT-FAMILY: arial, helvetica, sans-serif; MARGIN-TOP: 0px; COLOR: #283548; TEXT-ALIGN: left; LINE-HEIGHT: 23px; BACKGROUND-COLOR: transparent; mso-line-height-rule: exactly' align='left'>Adem&aacute;s de la opci&oacute;n del men&uacute; AYUDA, ya incluida anteriormente, hemos incorporado un acceso directo al Centro de Ayuda y enlaces activos dentro de las entradas del Blog para facilitar llegar a la informaci&oacute;n m&aacute;s r&aacute;pidamente.</p>
<!--[if gte mso 12]>
    <table cellspacing='0' cellpadding='0' border='0' width='100%'><tr><td align='right'>
<![endif]-->
<table class='imgtable btnset' style='TEXT-ALIGN: right; MARGIN-LEFT: auto; MARGIN-RIGHT: 0px' cellspacing='0' cellpadding='0' border='0'>
<tr>
<td class='contenttd' style='VERTICAL-ALIGN: middle; PADDING-BOTTOM: 0px; PADDING-TOP: 0px; PADDING-LEFT: 0px; PADDING-RIGHT: 0px'><a href='http://www.winmotor.blog/' target='_blank'><img title='Blog' border='none' alt='Blog Winmotor' src='https://www.winmotor.net/wp-content/uploads/2019/09/Image_7_7ae46899a4f74bbb8d0363115059bc14.png' /></a> </td>
</tr>
</table>
<!--[if gte mso 12]>
    </td></tr></table>
<![endif]--></th>
</tr>
</table>
</th>
</tr>
<tr>
<th class='contenttd' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 600px; BORDER-BOTTOM: medium none; FONT-WEIGHT: normal; PADDING-BOTTOM: 10px; TEXT-ALIGN: left; PADDING-TOP: 10px; PADDING-LEFT: 0px; BORDER-LEFT: medium none; PADDING-RIGHT: 0px; BACKGROUND-COLOR: transparent'>
<table style='WIDTH: 100%' cellspacing='0' cellpadding='0' align='left'>
<tr style='HEIGHT: 68px' height='68'>
<th class='contenttd' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 600px; VERTICAL-ALIGN: top; BORDER-BOTTOM: medium none; FONT-WEIGHT: normal; PADDING-BOTTOM: 0px; TEXT-ALIGN: left; PADDING-TOP: 0px; PADDING-LEFT: 0px; BORDER-LEFT: medium none; PADDING-RIGHT: 0px; BACKGROUND-COLOR: transparent'>
<div style='PADDING-BOTTOM: 10px; TEXT-ALIGN: center; PADDING-TOP: 10px; PADDING-LEFT: 10px; PADDING-RIGHT: 10px'>
<table class='imgtable' style='DISPLAY: inline-block' cellspacing='0' cellpadding='0' border='0'>
<tr>
<td style='PADDING-RIGHT: 5px'><a href='https://www.facebook.com/softwinmotor/' target='_blank'><img title='Facebook' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; BORDER-BOTTOM: medium none; BORDER-LEFT: medium none; DISPLAY: block' alt='Facebook' src='https://www.winmotor.net/wp-content/uploads/2019/09/Image_8_f7d483d47ca84c79a0ef1061a11b48d4.png' width='48' /></a> </td>
<td style='PADDING-RIGHT: 5px'><a href='https://twitter.com/winmotor' target='_blank'><img title='Twitter' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; BORDER-BOTTOM: medium none; BORDER-LEFT: medium none; DISPLAY: block' alt='Twitter' src='https://www.winmotor.net/wp-content/uploads/2019/09/Image_9_8b0b0e4fea764c8fbaafd27b13beec52.png' width='48' /></a> </td>
<td><a href='mailto:comercial@winmotor.net' target='_blank'><img title='Email' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; BORDER-BOTTOM: medium none; BORDER-LEFT: medium none; DISPLAY: block' alt='Email' src='https://www.winmotor.net/wp-content/uploads/2019/09/Image_10_d8ae4ae963204e2e84942cc79ee7e06d.png' width='48' /></a> </td>
</tr>
</table>
</div>
</th>
</tr>
</table>
</th>
</tr>
<tr>
<th class='contenttd' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 600px; BORDER-BOTTOM: medium none; FONT-WEIGHT: normal; PADDING-BOTTOM: 1px; TEXT-ALIGN: left; PADDING-TOP: 1px; PADDING-LEFT: 0px; BORDER-LEFT: medium none; PADDING-RIGHT: 0px; BACKGROUND-COLOR: transparent'>
<table style='WIDTH: 100%' cellspacing='0' cellpadding='0' align='left'>
<tr style='HEIGHT: 592px' height='592'>
<th class='contenttd' style='BORDER-TOP: medium none; BORDER-RIGHT: medium none; WIDTH: 580px; VERTICAL-ALIGN: top; BORDER-BOTTOM: medium none; FONT-WEIGHT: normal; PADDING-BOTTOM: 1px; TEXT-ALIGN: left; PADDING-TOP: 1px; PADDING-LEFT: 10px; BORDER-LEFT: medium none; PADDING-RIGHT: 10px; BACKGROUND-COLOR: transparent'>
<p style='FONT-SIZE: 12px; MARGIN-BOTTOM: 1em; FONT-FAMILY: arial, helvetica, sans-serif; MARGIN-TOP: 0px; COLOR: #4a6082; TEXT-ALIGN: center; LINE-HEIGHT: 15px; BACKGROUND-COLOR: transparent; mso-line-height-rule: exactly' align='center'>Software Winmotor - Glorieta Fernando Qui&ntilde;ones, Edificio Centris Planta 1 - m&oacute;dulo 7A Tomares - Sevilla<br />
<br />
&nbsp;<a title='' style='COLOR: #6f87ac' href='https://www.winmotor.net/'>winmotor.net</a> - <a title='' style='COLOR: #6f87ac' href='mailto:comercial@winmotor.net'>mailto:comercial@winmotor.net</a></p>
<p style='FONT-SIZE: 12px; MARGIN-BOTTOM: 1em; FONT-FAMILY: arial, helvetica, sans-serif; MARGIN-TOP: 0px; COLOR: #4a6082; TEXT-ALIGN: center; LINE-HEIGHT: 15px; BACKGROUND-COLOR: transparent; mso-line-height-rule: exactly' align='center'>Si necesita informaci&oacute;n a cerca de nuestra Pol&iacute;tica de Privacidad, pulse <a title='' style='COLOR: #6f87ac' href='https://www.winmotor.net/politica-privacidad/'>AQU&Iacute;</a><br />
<br />
Si no quiere seguir recibiendo estos emails, por favor, comun&iacute;quelo en el siguiente enlace <a title='' style='COLOR: #6f87ac' href='mailto:comercial@winmotor.net'>CANCELAR ENV&Iacute;OS</a><br />
<br />
&copy;2019 Software Winmotor. Reservados todos los Derechos.</p>
<p style='FONT-SIZE: 12px; MARGIN-BOTTOM: 1em; FONT-FAMILY: arial, helvetica, sans-serif; MARGIN-TOP: 0px; COLOR: #4a6082; TEXT-ALIGN: center; LINE-HEIGHT: 15px; BACKGROUND-COLOR: transparent; mso-line-height-rule: exactly' align='center'>Este mensaje es privado y confidencial; solamente tiene acceso a su contenido la persona a la que va dirigido. Si usted ha recibido este mensaje por error, no debe revelar, copiar, distribuir o usarlo en ning&uacute;n sentido. Le rogamos lo comunique al remitente y borre dicho mensaje y cualquier otro documento adjunto que pudiera contener. No hay renuncia al derecho a la confidencialidad ni a ning&uacute;n privilegio por causa de transmisi&oacute;n err&oacute;nea o mal funcionamiento. En cumplimiento de lo establecido en la L.O. 3/2018 de Protecci&oacute;n de Datos de Car&aacute;cter Personal y el Reglamento (UE) 679/2016, le informo que sus datos personales son objeto de tratamiento por parte de SOFTWARE WINMOTOR S.L., con la finalidad de posibilitar las comunicaciones con los diferentes contactos que &eacute;sta mantiene en el ejercicio de su actividad y enviarle informaci&oacute;n sobre nuestras actividades y eventos. Todos los datos recogidos son almacenados bajo la confidencialidad y las medidas de seguridad legalmente establecidas y no ser&aacute;n cedidos ni compartidos con empresas, entidades o particulares ajenos; salvo obligaci&oacute;n legal. Igualmente, deseo informarle que podr&aacute; ejercer los derechos de acceso, rectificaci&oacute;n, supresi&oacute;n, cancelaci&oacute;n, oposici&oacute;n, limitaci&oacute;n y portabilidad enviando un correo electr&oacute;nico a comercial@winmotor.net o en nuestra sede, sito en Glorieta Fernando Qui&ntilde;ones, Edificio Centris, Planta 1, M&oacute;dulo 7, 41940 Tomares, Sevilla.</p>
<p style='FONT-SIZE: 12px; MARGIN-BOTTOM: 1em; FONT-FAMILY: arial, helvetica, sans-serif; MARGIN-TOP: 0px; COLOR: #4a6082; TEXT-ALIGN: center; LINE-HEIGHT: 15px; BACKGROUND-COLOR: transparent; mso-line-height-rule: exactly' align='center'>This message is private and confidential; only the person to whom it is addressed has access to its content. If you have received this message by mistake, you must not reveal, copy, distribute or use it in anyway. We kindly ask you to notify the sender and delete this message and any other attached document that may contain. There is no waiver of the right to confidentiality or any privilege due to erroneous transmission or malfunction. In compliance with the provisions of L.O. 3/2018 of Protection of Personal Data and Regulation (EU) 679/2016, we inform you that your personal data are subject to treatment by SOFTWARE WINMOTOR SL, in order to enable communications with different contacts that this keep in the exercise of your activity and send you information about our activities and events. All the data collected is stored under the confidentiality and security measures legally established and will not be transferred or shared with companies, entities or individuals from outside; except legal obligation. Likewise, I wish to inform you that you may exercise the rights of access, rectification, deletion, cancellation, opposition, limitation and portability by sending an email to comercial@winmotor.net or at our headquarters, located in Glorieta Fernando Qui&ntilde;ones, Centris Building, Floor 1, Module 7, 41940 Tomares, Seville.</p>
</th>
</tr>
</table>
</th>
</tr>
</table>
</td>
</tr>
<tr>
<td style='FONT-SIZE: 0px; HEIGHT: 8px; LINE-HEIGHT: 0'>&nbsp;</td>
</tr>
</table>
<!-- Created with MailStyler 2.5.6.100 -->
</body>
</html>
"
```
{% endcode %}

\*\*\* Conforme vayan surgiendo dudas, ampliaremos la información aquí disponible incluso con ejemplos prácticos. Por ello no dudéis en consultarnos por email los detalles que os faltan para configurar correctamente este importante apartado del programa a fin de añadirlos.

