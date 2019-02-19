---
description: '*** Manual en fase de desarrollo ***'
---

# NOVEDAD: Nuevo Módulo Recursos Humanos

**Objetivo**

En este módulo se resuelve la gestión del personal de la empresa a efectos de controlar vacaciones, bajas, calendario laboral individual y el control presencial de cada trabajador.

Por otro lado, y partiendo del calendario laboral de cada trabajador se crean y gestionan las agendas de citas por persona y departamento.

**Gestión**

En este gráfico \(clic encima para ampliar\) se muestran las tablas que intervienen en la estructura del módulo:

![](../../.gitbook/assets/image%20%28157%29.png)

Vamos a definir las tablas que intervienen en el orden que hay que crearlas para poner en marcha el módulo y crear los calendarios laborales y las distintas agendas de citas:

1 – Horarios/Jornadas

![](../../.gitbook/assets/image%20%2829%29.png)

Haciendo doble clic en la rejilla que aparece con el título “HORARIOS” en el menú de recursos humanos podremos crear las distintas fichas.

Hay que definir los horarios para la empresa o el centro indicando el nombre del horario \(mañana en este caso\) y la hora de inicio y fin. El programa calculará los minutos y horas que comprenden, así como el código de la ficha que tampoco hay que rellenarlo.

Normalmente para una empresa o centro habrá por tanto que definir el horario de mañana, el de tarde y si hay algún otro especial para algún día \(por ejemplo, si se trabaja el sábado sólo de mañana y con un horario distinto crearemos una ficha específica para ese día con el horario de sábado\).

2 – Festivos

Desde la ficha del centro en caso de distribución multicentro o la de la empresa, entrando en la pestaña “Festivos” podremos definirlos.

![](file:///C:/Users/Alberto/AppData/Local/Temp/msohtmlclip1/01/clip_image002.png)

Para definir los días festivos a partir del calendario laboral de la ciudad en la que esté la empresa o el centro daremos de alta una ficha por cada día, definiendo el nombre de la festividad y la fecha. Para la fecha usaremos el botón que aparece remarcado y quedará registrada sin el año.

Por último, hay que definir si se trata de una festividad nacional o local. En caso de distribución multicentro hay que definir los días festivos por cada centro, pero podemos usar el botón “Importar” que aparece debajo de la rejilla para importar los días ya definidos para otro centro, pudiendo seleccionar si queremos importar todos los días ya definidos, los nacionales o los locales.

3 – Departamentos laborales

Partiendo de la ficha de empresa o de centro en caso de distribución multicentro y de un departamento o sección \(taller, comercial, recambios, boutique\) se crean los distintos departamentos laborales. Para tener claro el concepto un departamento laboral será por lo tanto una sección de una empresa o de un departamento de una empresa; es decir, podemos crear por ejemplo el departamento “Taller” de una tienda o en caso de que queramos manejar distintas agendas podemos crear “subdepartamentos” como podría ser “Taller– chapa” y “Taller-electrónica”.

Haciendo doble clic en la rejilla “DEPARTAMENTOS” del menú de recursos humanos aparecerá este formulario:

![](file:///C:/Users/Alberto/AppData/Local/Temp/msohtmlclip1/01/clip_image004.jpg)

En el primer campo definiremos el centro o empresa al que está asociado \(También se puede acceder a este formulario desde la pestaña “Departamentos” de las fichas de Empresas o centros de trabajo en cuyo caso este campo aparecerá relleno\).

En el siguiente campo “Subdepartamento” definiremos el departamento de empresa al que estará relacionado el departamento laboral \(normalmente “C”- Comercial o “T” - Taller por ejemplo\).  En el ejemplo que presentamos arriba vamos a montar un departamento laboral con subdepartamento, en este caso “Taller” – “Electrónica”: rellenaremos por lo tanto el nombre del subdepartamento y un código de tres dígitos para identificarlo. Es importante recalcar que este campo es opcional y sólo lo utilizaremos en caso de querer gestionar varias agendas dentro de un mismo departamento de empresa.

El campo nombre con fondo gris se rellenará automáticamente con los datos anteriormente grabados.

A continuación, se nos pide “Tiempo mínimo para una cita \(minutos\)”: tendremos que definir por lo tanto el tiempo mínimo para el que daremos una cita; en el ejemplo hemos definido 15 minutos. Esto no sólo implica que no podremos dar citas de menos de 15 minutos, sino que todas las citas que demos serán de un múltiplo de este tiempo: partiendo de esta cifra podremos dar citas de 15, 30 ,45...minutos.

El siguiente campo es para indicar al programa si permitiremos que se puedan calcular “citas partidas”:  imaginemos que tenemos para un día sólo dos huecos libres, de 11:00 a 11:30 y de 17:00 a 18:30, si un cliente nos solicita una cita de dos horas para este día sólo se la podremos asignar en caso de que este campo esté marcado. Es importante recalcar que luego en el formulario de la cita se podrá desmarcar el permiso puesto que no siempre es factible que una cita pueda partirse. Es decir, al marcar este campo cuando vayamos a dar una cita ésta por defecto también lo mantendrá marcado y podremos por lo tanto darle partida, pero en la cita se puede desmarcar con lo que el programa buscaría sólo citas continuas.

Una vez definidos los datos de cabecera hay que crear:

Jornadas- se define el horario que tendremos en cada día de la semana que sea laborable:

![](file:///C:/Users/Alberto/AppData/Local/Temp/msohtmlclip1/01/clip_image006.jpg)

Haciendo doble clic en la rejilla de Jornadas iremos definiendo estos datos por cada día:

![](file:///C:/Users/Alberto/AppData/Local/Temp/msohtmlclip1/01/clip_image007.png)

Aunque no tiene mucho sentido, el programa contempla que para un mismo día se puedan definir hasta cuatro horarios. Es fundamental entender que éstos no se pueden pisar, es decir, no podemos definir un horario de mañana que termine a las 14:00 y un horario de tarde que empiece a las 13:30.

