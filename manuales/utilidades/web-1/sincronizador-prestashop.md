---
description: Explicación, detalles a tener en cuenta y configuración para su puesta a punto
---

# Sincronizador Prestashop

Con el sincronizador se podrá hacer la comunicación entre la web de Prestashop y Winmotor.

Con el sincronizador mediante cron se podrán hacer las sincronizaciones de forma automática en ambos sentidos.

En la sincronización existen las siguientes opciones:

* Winmotor a Prestashop:
  * Sincronizar las categorías (familias en Winmotor).
  * Sincronizar los productos (artículos) tanto los nuevos creados.
  * Sincronizar TODOS los productos (artículos).
* Prestashop a Winmotor:
  * Sincronizar los clientes solo de hoy.
  * Sincronizar los pedidos solo de hoy.
  * Sincronizar TODOS los clientes.
  * Sincronizar TODOS los pedidos.

Para la configuración del CRON habrá que crear un nuevo trabajo de cron en cPanel o el similar del hosting.

Por tanto, habrá que copiar y pegar el siguiente comando en un nuevo cron job de su hosting. Ejemplo:

* /_usr/bin/curl --user-agent cPanel-Cron "_[_https://DOMINIO\_WEB/WinSync/exec.php?userKey=CODE\&mode=cron"_](https://phpstack-1004645-4311096.cloudwaysapps.com/WinSync\_f/exec.php?userKey=a%C3%B1sopdjfje900sdawredia\&mode=cron%22)

Los valores para minuto, hora, día y día de la semana habrá que especificarlo pudiendo ser una vez al día, dos veces al día o cada hora. El valor mínimo será de cada hora y en esa sincronización sincronizará todos los puntos mencionados anteriormente.
