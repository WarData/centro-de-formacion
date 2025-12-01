# WhatsApp

Introducción

Este manual describe cómo utilizar el nuevo módulo WhatsApp integrado en la aplicación Winmotor. El módulo permite gestionar comunicaciones con clientes de forma automática y manual, optimizando el servicio de atención y seguimiento en todo el flujo de su negocio.

### 1. Acceso al módulo WhatsApp

#### 1.1 Ubicación del módulo

Una vez que el módulo WhatsApp esté activado en su aplicación, encontrará una nueva opción al final del menú principal que le permitirá acceder al panel de control de WhatsApp (contacte con [comercial@winmotor.com](mailto:comercial@winmotor.com) para solicitar información y presupuesto)

#### 1.2 Pantalla principal del módulo

La interfaz de WhatsApp en Winmotor presenta una ventaja respecto a la versión de teléfono: **muestra simultáneamente la lista de contactos en el lado izquierdo y los mensajes del contacto seleccionado en el lado derecho**, permitiendo una gestión más eficiente de las conversaciones.

### 2. Contactos y comunicación

#### 2.1 Gestión de contactos

El módulo WhatsApp funciona con los contactos propios de su empresa:

* Winmotor genera automáticamente un contacto para cada entidad creada en la aplicación.
* **Requisito**: La entidad debe tener el teléfono móvil completamente rellenado.
* Los contactos existentes aparecerán en la lista disponible para comunicación.

#### 2.2 Primera comunicación: obligatoriedad de plantillas

Para iniciar una conversación con un contacto **debe hacerlo obligatoriamente a través de una plantilla preestablecida**.

Características de las plantillas:

* Winmotor entrega una colección de plantillas base para cada caso de uso.
* Las plantillas están prediseñadas y optimizadas para diferentes situaciones.
* Solo después de que el contacto responda puede enviar mensajes libres.

{% hint style="info" %}
Nota importante: En la pestaña de envío (cuando se envía desde documentos) aparecerá automáticamente la conversación relacionada con el documento, permitiendo un seguimiento completo.
{% endhint %}

### 3. Tipos de mensajes

#### 3.1 Mensajes automáticos

Ciertos eventos en el programa generan automáticamente mensajes WhatsApp que se envían a través de plantillas predefinidas:

* Presupuestos
* Citas de taller
* Fin de reparación
* Material recibido

#### 3.2 Mensajes manuales

Los mensajes manuales se originan directamente desde el panel de WhatsApp, permitiendo comunicación personalizada con clientes.

#### 3.3 Mensajes desde documentos

Desde los siguientes documentos y módulos puede enviar WhatsApp mediante la pestaña habilitada:

* Presupuestos
* Órdenes de Reparación (ORs)
* Pedidos
* Facturas de venta
* Operaciones comerciales

### 4. Reglas de comunicación

#### 4.1 Ventana de 24 Horas

Restricción después de enviar plantilla:

* Después de enviar una plantilla a un contacto **no podrá enviar mensajes libres** hasta que el contacto responda.
* Una vez ha respondido el contacto, tiene **hasta veinticuatro horas** para enviar un mensaje libre.
* Pasadas las 24 horas desde la respuesta, deberá enviar una nueva plantilla.

#### 4.2 Mensajes desde el contacto

* El contacto **puede enviarle mensajes libres en cualquier momento** sin restricciones.
* El contacto no verá a su empresa en su WhatsApp hasta que **le haya enviado una plantilla como primer contacto**.

### 5. Configuración de usuarios y departamentos

#### 5.1 Requisito obligatorio

Si activa el módulo WhatsApp, **todos los usuarios finales de la aplicación deben tener definido su "Departamento Interno"** en su ficha de usuario.

#### 5.2 Acceso según departamento

* Cada usuario verá exclusivamente los mensajes relativos a su departamento.
* Los usuarios no ven mensajes personales sino todos los del departamento al que pertenecen.
* Esto funciona como un sistema de empresa, no como comunicación personal.

#### 5.3 Configuración multicentro

Si la empresa es **multicentro**, los departamentos están separados por centros, manteniendo la estructura organizativa de la empresa.

#### 5.4 Permisos de supervisor

Los usuarios definidos como **supervisores** tienen permisos especiales:

* Pueden ver los mensajes de **todos los departamentos**.
* Por defecto, ven primero los mensajes de su propio departamento.
* Su departamento interno también debe estar definido en su ficha de usuario.

### 6. Flujo de trabajo típico

{% stepper %}
{% step %}
#### Acceso y selección de contacto

* Acceda al módulo WhatsApp desde el menú principal.
* Seleccione un contacto de la lista o busque el contacto deseado.
{% endstep %}

{% step %}
#### Iniciar comunicación con plantilla

* Para iniciar comunicación, seleccione la plantilla apropiada según el caso:
  * Presupuesto: use plantilla de presupuesto
  * Cita de taller: use plantilla de cita
  * Fin de reparación: use plantilla de finalización
  * Material recibido: use plantilla de recepción
* El mensaje se envía automáticamente al contacto.
{% endstep %}

{% step %}
#### Respuesta y mensajes libres

* Espere la respuesta del contacto.
* Una vez respondido, puede enviar mensajes libres durante 24 horas.
* Después de 24 horas, deberá enviar una nueva plantilla para continuar.
{% endstep %}
{% endstepper %}

### Flujo desde documentos del sistema

{% stepper %}
{% step %}
#### Abrir documento relacionado

* Abra el documento (presupuesto, OR, pedido, factura, operación comercial).
* Localice la pestaña de WhatsApp habilitada.
{% endstep %}

{% step %}
#### Seleccionar contacto y plantilla

* El sistema mostrará los contactos disponibles.
* Seleccione el contacto y la plantilla apropiada.
{% endstep %}

{% step %}
#### Visualizar historial y enviar

* El historial de conversación relacionada aparecerá en la misma pestaña.
* Envíe la plantilla; el envío quedará ligado al documento.
{% endstep %}
{% endstepper %}

### 7. Casos de uso comunes

#### 7.1 Envío de Presupuesto

{% stepper %}
{% step %}
Acceda al presupuesto en el sistema.
{% endstep %}

{% step %}
En la pestaña WhatsApp, seleccione el cliente.
{% endstep %}

{% step %}
Elija la plantilla de presupuesto.
{% endstep %}

{% step %}
Se enviará automáticamente con la información del presupuesto.
{% endstep %}

{% step %}
El cliente puede responder directamente desde WhatsApp.
{% endstep %}
{% endstepper %}

#### 7.2 Confirmación de cita de taller

{% stepper %}
{% step %}
Cree la cita en el sistema.
{% endstep %}

{% step %}
Vaya a la pestaña WhatsApp de la cita.
{% endstep %}

{% step %}
Envíe la plantilla de confirmación de cita.
{% endstep %}

{% step %}
El cliente recibirá la cita y su horario.
{% endstep %}
{% endstepper %}

#### 7.3 Notificación de fin de reparación

{% stepper %}
{% step %}
Cuando finalice la reparación, acceda a la OR.
{% endstep %}

{% step %}
En la pestaña WhatsApp, envíe la plantilla de fin de reparación.
{% endstep %}

{% step %}
El cliente será notificado automáticamente.
{% endstep %}

{% step %}
Podrá responder consultas sobre la reparación durante 24 horas.
{% endstep %}
{% endstepper %}

#### 7.4 Confirmación de material recibido

{% stepper %}
{% step %}
Registre el material recibido en el sistema.
{% endstep %}

{% step %}
Acceda a la sección correspondiente.
{% endstep %}

{% step %}
Envíe la plantilla de material recibido.
{% endstep %}

{% step %}
El cliente será notificado del estado de su pedido.
{% endstep %}
{% endstepper %}

### 8. Recomendaciones importantes

#### 8.1 Buenas prácticas

* Verifique que todos los contactos tengan teléfono móvil registrado antes de usar el módulo.
* Asegúrese de que todos los usuarios finales tengan su departamento interno configurado.
* Use las plantillas prediseñadas para garantizar comunicación profesional.
* Realice seguimiento de conversaciones en la pestaña WhatsApp de cada documento.
* Responda dentro de las 24 horas después de que un cliente responda.

#### 8.2 Restricciones a considerar

* No podrá enviar mensajes libres sin que el cliente haya respondido primero.
* Cada nueva iniciativa de contacto requiere una plantilla.
* La ventana de 24 horas es estricta; después vencerá sin posibilidad de enviar mensajes libres.
* Solo verá mensajes de su departamento (salvo si es supervisor).
* El módulo requiere que esté completamente configurado para todos los usuarios.

### 9. Solución de problemas

<details>

<summary>No veo mensajes de otros departamentos</summary>

Causa: Su usuario no tiene permisos de supervisor.

Solución: Solicite a su administrador que defina su usuario como supervisor.

</details>

<details>

<summary>No puedo enviar mensajes libres</summary>

Causa: El contacto no ha respondido aún a la plantilla.

Solución: Espere a que el contacto responda o envíe una nueva plantilla.

</details>

<details>

<summary>El contacto no aparece en la lista</summary>

Causa: La entidad no tiene teléfono móvil registrado.

Solución: Edite la entidad y complete el campo de teléfono móvil.

</details>

<details>

<summary>Falta Departamento Interno</summary>

Causa: Su usuario no tiene departamento definido.

Solución: Contacte a su administrador para que asigne su departamento interno.

</details>

### 10. Conclusión

El módulo WhatsApp de Winmotor optimiza la comunicación con clientes mediante una integración completa en el flujo de trabajo empresarial. Siguiendo este manual, podrá:

* Gestionar comunicaciones de forma ordenada y profesional.
* Automatizar notificaciones sobre presupuestos, citas y reparaciones.
* Mantener un historial completo de conversaciones ligadas a documentos.
* Respetar las reglas de comunicación de WhatsApp Business.

Para consultas adicionales o soporte técnico, contacte a [programacion@winmotor.com](mailto:programacion@winmotor.com)
