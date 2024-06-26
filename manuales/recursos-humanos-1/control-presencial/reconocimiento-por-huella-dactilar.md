---
description: Módulo opcional
---

# Reconocimiento por huella dactilar

1.- Realizada la activación del módulo de reconocimiento de huellas por parte de Winmotor, se añadirá la grabación y borrado de huella existente a los usuarios, accediendo a la entidad > Datos Trabajador > Control Huella:

<figure><img src="../../../.gitbook/assets/imagen (2) (1) (3) (1).png" alt=""><figcaption></figcaption></figure>

* Al pulsar en el botón "Grabar huella" mostrará la ventana de grabación de huellas del lector y tendremos que añadir el mismo dedo 3 veces, levantándolo cada vez que reconozca la huella y darle a grabar una vez haya finalizado:

<figure><img src="../../../.gitbook/assets/imagen (8) (1) (2) (1) (1).png" alt=""><figcaption></figcaption></figure>

* Se mostrarán 4 confirmaciones de huella como 1, 2, 3 y 4 para generar y guardar la huella en formato XML.

2.- Además añade el botón "Huella" en el menú del control presencial a fin de realizar la lectura por huella cuando se pulsa o permitiendo el acceso mediante el carné usando el lector de códigos de barras:

<figure><img src="../../../.gitbook/assets/imagen (1) (1) (2) (2) (1).png" alt=""><figcaption></figcaption></figure>

* Mientras no se pulse en el botón "Huella" el control presencial funcionará en modo lector de códigos de barras
* Cuando se pulsa "Huella" mostrará la ventana del lector de huellas para pulsar y leer, reconociendo al usuario que tenga la huella guardada:

<figure><img src="../../../.gitbook/assets/imagen (3) (5) (1) (1).png" alt=""><figcaption></figcaption></figure>

* Panel con entradas y salidas de usuarios usando el reconocimiento de huellas:

<figure><img src="../../../.gitbook/assets/imagen (6) (1) (4).png" alt=""><figcaption></figcaption></figure>

3.- Solución de fallos (Error -17):

<figure><img src="../../../.gitbook/assets/5572d4f2-e197-4854-8b1f-610efb466eb6.png" alt=""><figcaption></figcaption></figure>

* Para grabar la huella en la entidad del usuario debe estar cerrado el control presencial (si lo tienen abierto en un vClient independiente) y si se realiza en una pestaña directamente en el control presencial también cerrarlo.
  * Una vez grabada la huella abrir el vClient con el control presencial o una pestaña en el mismo vClient.
* Si sigue dando error comprobar si la entidad que no puede dar de alta la entrada/salida en el control presencial es una entidad normal o también es una entidad usuario. Si no es un usuario hacer que esa entidad también sea usuario.
