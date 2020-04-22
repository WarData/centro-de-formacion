---
description: >-
  La clave de este módulo es que se puede configurar cualquier departamento de
  la empresa. Para el desarrollo de este manual nos hemos basado en el Taller.
---

# Configuración Módulo Recursos Humanos

![](../../.gitbook/assets/image%20%28411%29.png)

**Objetivo**

En este módulo se resuelve la gestión del personal de la empresa a efectos de controlar vacaciones, bajas, calendario laboral individual y el control presencial de cada trabajador.

Por otro lado, y partiendo del calendario laboral de cada trabajador se crean y gestionan las agendas de citas por persona y departamento.

**Gestión**

En este gráfico \(clic encima para ampliar\) se muestran las tablas que intervienen en la estructura del módulo:

![](../../.gitbook/assets/image%20%28414%29.png)

Vamos a definir las tablas que intervienen en el orden que hay que crearlas para poner en marcha el módulo y crear los calendarios laborales y las distintas agendas de citas:

1 – Horarios/Jornadas

![](../../.gitbook/assets/image%20%28392%29.png)

Haciendo doble clic en la rejilla que aparece con el título “HORARIOS” en el menú de recursos humanos podremos crear las distintas fichas.

Hay que definir los horarios para la empresa o el centro indicando el nombre del horario \(mañana en este caso\) y la hora de inicio y fin. El programa calculará los minutos y horas que comprenden, así como el código de la ficha que tampoco hay que rellenarlo.

Normalmente para una empresa o centro habrá por tanto que definir el horario de mañana, el de tarde y si hay algún otro especial para algún día \(por ejemplo, si se trabaja el sábado sólo de mañana y con un horario distinto crearemos una ficha específica para ese día con el horario de sábado\).

2 – Festivos

Desde la ficha del centro en caso de distribución multicentro o la de la empresa, entrando en la pestaña “Festivos” podremos definirlos.

![](../../.gitbook/assets/image%20%28218%29.png)

Para definir los días festivos a partir del calendario laboral de la ciudad en la que esté la empresa o el centro daremos de alta una ficha por cada día, definiendo el nombre de la festividad y la fecha. Para la fecha usaremos el botón que aparece remarcado y quedará registrada sin el año.

Por último, hay que definir si se trata de una festividad nacional o local. En caso de distribución multicentro hay que definir los días festivos por cada centro, pero podemos usar el botón “Importar” que aparece debajo de la rejilla para importar los días ya definidos para otro centro, pudiendo seleccionar si queremos importar todos los días ya definidos, los nacionales o los locales.

3 – Departamentos laborales

Partiendo de la ficha de empresa o de centro en caso de distribución multicentro y de un departamento o sección \(taller, comercial, recambios, boutique\) se crean los distintos departamentos laborales. Para tener claro el concepto un departamento laboral, será por lo tanto una sección de una empresa o de un departamento de una empresa; es decir, podemos crear por ejemplo el departamento “Taller” de una tienda o en caso de que queramos manejar distintas agendas podemos crear “subdepartamentos” como podría ser “Taller– chapa” y “Taller-electrónica”.

Haciendo doble clic en la rejilla “DEPARTAMENTOS” del menú de recursos humanos aparecerá este formulario:

![](../../.gitbook/assets/image%20%28501%29.png)

En el primer campo definiremos el centro o empresa al que está asociado \(También se puede acceder a este formulario desde la pestaña “Departamentos” de las fichas de Empresas o centros de trabajo en cuyo caso este campo aparecerá relleno\).

En el siguiente campo “Subdepartamento” definiremos el departamento de empresa al que estará relacionado el departamento laboral \(normalmente “C”- Comercial o “T” - Taller por ejemplo\).  En el ejemplo que presentamos arriba vamos a montar un departamento laboral con subdepartamento, en este caso “Taller” – “Electrónica”: rellenaremos por lo tanto el nombre del subdepartamento y un código de tres dígitos para identificarlo. Es importante recalcar que este campo es opcional y sólo lo utilizaremos en caso de querer gestionar varias agendas dentro de un mismo departamento de empresa.

El campo nombre con fondo gris se rellenará automáticamente con los datos anteriormente grabados.

A continuación, se nos pide “Tiempo mínimo para una cita \(minutos\)”: tendremos que definir por lo tanto el tiempo mínimo para el que daremos una cita; en el ejemplo hemos definido 15 minutos. Esto no sólo implica que no podremos dar citas de menos de 15 minutos, sino que todas las citas que demos serán de un múltiplo de este tiempo: partiendo de esta cifra podremos dar citas de 15, 30 ,45...minutos.

El siguiente campo es para indicar al programa si permitiremos que se puedan calcular “citas partidas”:  imaginemos que tenemos para un día sólo dos huecos libres, de 11:00 a 11:30 y de 17:00 a 18:30, si un cliente nos solicita una cita de dos horas para este día sólo se la podremos asignar en caso de que este campo esté marcado. Es importante recalcar que luego en el formulario de la cita se podrá desmarcar el permiso puesto que no siempre es factible que una cita pueda partirse. Es decir, al marcar este campo cuando vayamos a dar una cita ésta por defecto también lo mantendrá marcado y podremos por lo tanto darle partida, pero en la cita se puede desmarcar con lo que el programa buscaría sólo citas continuas.

Una vez definidos los datos de cabecera hay que crear:

**Jornadas** - se define el horario que tendremos en cada día de la semana que sea laborable:

![](../../.gitbook/assets/image%20%28142%29.png)

Haciendo doble clic en la rejilla de Jornadas iremos definiendo estos datos por cada día:

![](../../.gitbook/assets/image%20%2869%29.png)

Aunque no tiene mucho sentido, el programa contempla que para un mismo día se puedan definir hasta cuatro horarios. Es fundamental entender que éstos no se pueden pisar, es decir, no podemos definir un horario de mañana que termine a las 14:00 y un horario de tarde que empiece a las 13:30.

**Operarios** - Se asignan al departamento laboral de los disponibles según el tipo de entidad. Aquellas entidades marcadas como "operarios" se podrán asignar a cualquiera de los departamentos creados entrando en la pestaña de la propia entidad "Operario" e introduciendo el código del departamento.

Dicho código se corresponde con "empresa-departamento" como por ejemplo 1-T. Una vez asignado al departamento el operario, se deberá asignar la jornada \(es posible que tenga horarios distintos a otros operarios\). 

\*\*\* Es requisito imprescindible que el módulo RRHH esté activado por nuestros técnicos \(Win ERP\).

![](../../.gitbook/assets/image%20%28285%29.png)

**Administradores** - Son aquellas entidades "usuario" que tienen acceso al alta / borrado / modificación / lectura de las características del módulo de RRHH\*\*\* \(departamentos laborales, jornadas, etc...\) y al panel de citas con sus diversas visualizaciones.

\*\*\* Si tienen el acceso activado también en su perfil de usuario

![](../../.gitbook/assets/image%20%28493%29.png)

**Una vez finalizada la configuración debemos ir a "Configuración" &gt; Listar ejercicios &gt; entrar en el ejercico actual y pulsar en el botón "Crear Calendarios". Este proceso tarda unos minutos en finalizar.** 

Finalizado el proceso anterior, al pulsar en la opción RRHH obtenemos este panel de configuración de Recursos Humanos completo, a nivel administrador, en el que podremos visualizar citas por día, mes, año, operario, disponibilidad y un largo etcétera que iremos viendo a lo largo de este manual:

![](../../.gitbook/assets/image%20%28361%29.png)

**Completada la configuración, el usuario que gestione la agenda del departamento laboral podrá acceder a ella desde la opción "Taller" &gt; "Agenda de Taller" \***

**\* Es muy importante revisar la configuración de usuario y activar un modo de visualización de la nueva agenda \(Configuración &gt; Listar Usuarios &gt; seleccionar usuario que va a usar el planning de taller &gt; Pestaña "Configuración de usuario &gt; al final "Recursos Humanos" y tener activada una "Vista de Panel" &gt; semana / mes / año\), en caso contrario la Agenda de Taller no abrirá el Planning.**

![](../../.gitbook/assets/image%20%28202%29.png)

Para usuarios de Winmotor que únicamente gestionen el planning para dar citas, cambiarlas, etc...su perfil debe tener, como mínimo para dicha acción, **"Recursos Humanos" y "Gestión de Citas" activados** en alta / baja / modificación y consulta:

![](../../.gitbook/assets/image%20%28316%29.png)

Y añadir a dichos usuarios a Administradores del departamento dentro de la opcíon RRHH según la siguiente imagen:

![&#xDA;nicamente WINMOTOR podr&#xED;a gestionar el planning en este caso](../../.gitbook/assets/image%20%28504%29.png)

Como configuración añadida a la anterior, seleccionando Departamento y luego un operario, podemos en su vista mensual definir **vacaciones, bajas o eventos\*\*\*** \(cursos por ejemplo\):

![](../../.gitbook/assets/image%20%2843%29.png)

\*\*\* Requisito imprescindible: activar en el perfil **"Administración de Calendarios"**

En los botones inferiores \(los 3 de la izquierda\) accedemos a definir:

* Vacaciones:

![](../../.gitbook/assets/image%20%28402%29.png)

* Bajas:

![](../../.gitbook/assets/image%20%28487%29.png)

* Eventos:

![](../../.gitbook/assets/image%20%28442%29.png)

En todos los casos, al pulsar en "Revisar", el sistema comprueba si entra en algún conflicto con una o más citas durante ese periodo para cambiarlas de operario si es posible.

![](../../.gitbook/assets/image%20%28329%29.png)

En la vista del mes podemos ver vacaciones en azul claro, eventos a determinadas horas en azul oscuro y baja en rojo. Estos elementos se alternan con las citas del departamento cada día, mostrando el porcentaje de ocupación, en este caso de un único operario.

