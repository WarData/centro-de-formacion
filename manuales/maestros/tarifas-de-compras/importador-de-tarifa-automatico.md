---
description: Automatismo de importación y actualización de tarifas de proveedor
---

# Importador de Tarifa automático

Se ha implementado un automatismo para la importación y actualización de tarifas de artículos. Este mecanismo permite mantener actualizados los precios y datos de los artículos de forma periódica y desatendida, según la configuración establecida en cada automatismo.

{% hint style="info" %}
La funcionalidad está disponible en:

_Maestros > Tarifas de artículos > Importador tarifa > Automatismos > Nueva_
{% endhint %}

## 1. Acceso y Configuración del Automatismo

<figure><img src="../../../.gitbook/assets/image (722).png" alt=""><figcaption></figcaption></figure>

### 1.1. Campos principales

<table data-header-hidden><thead><tr><th valign="top">Campo</th><th valign="top">Descripción</th></tr></thead><tbody><tr><td valign="top">Campo</td><td valign="top">Descripción</td></tr><tr><td valign="top">Código</td><td valign="top">Identificador numérico del automatismo. (Se asigna automáticamente)</td></tr><tr><td valign="top">Proveedor</td><td valign="top">Proveedor asociado a la tarifa.</td></tr><tr><td valign="top">Nombre</td><td valign="top">Nombre descriptivo del automatismo.</td></tr><tr><td valign="top">Sistema de conexión</td><td valign="top">Sistema origen de la tarifa.</td></tr><tr><td valign="top">Activa</td><td valign="top">Indica si el automatismo está habilitado.</td></tr></tbody></table>

<figure><img src="../../../.gitbook/assets/image (723).png" alt=""><figcaption></figcaption></figure>

### 1.2. Pestaña Conexión

Contiene los parámetros de vinculación con la fuente de datos:

<table data-header-hidden><thead><tr><th valign="top">Parámetro</th><th valign="top">Descripción</th></tr></thead><tbody><tr><td valign="top">Parámetro</td><td valign="top">Descripción</td></tr><tr><td valign="top">Estructura importación</td><td valign="top">Identificador y nombre de la estructura de importación creada previamente en el importador de tarifas.</td></tr><tr><td valign="top">Tipo de tarea (T o C)</td><td valign="top">Debe configurarse como T (Tarifa) o C (descarga de compras).</td></tr><tr><td valign="top">Tipo de actualización</td><td valign="top"><p>Define el alcance de la actualización. Valores </p><p>posibles: S, A o T</p></td></tr></tbody></table>

<figure><img src="../../../.gitbook/assets/image (724).png" alt=""><figcaption></figcaption></figure>

### 1.3. Planificación de ejecución

<table data-header-hidden><thead><tr><th valign="top">Parámetro</th><th valign="top">Descripción</th></tr></thead><tbody><tr><td valign="top">Parámetro</td><td valign="top">Descripción</td></tr><tr><td valign="top">Periodicidad</td><td valign="top">Intervalo de ejecución en horas (Mínimo 1 hora).</td></tr><tr><td valign="top">Última</td><td valign="top">Fecha y hora de la última ejecución realizada.</td></tr><tr><td valign="top">Próxima</td><td valign="top">Fecha y hora de la próxima ejecución programada.</td></tr></tbody></table>

<figure><img src="../../../.gitbook/assets/image (725).png" alt=""><figcaption></figcaption></figure>

## 2. Tipos de Actualización (campo S, A o T)

El campo Tarifas: tipo actualización determina el alcance de los cambios aplicados durante la importación:

* S – Solo actualizar tarifa: Únicamente se actualizan los precios de la tarifa existente. No se modifican los artículos.
* A – Actualizar tarifa y artículos: Se actualiza la tarifa y también se actualizan los datos de los artículos que ya existen en el programa.
* T – Actualizar tarifa, artículos y crear nuevos: Se actualiza la tarifa, se actualizan los artículos existentes y, además, se crean aquellos artículos que aún no existan en el programa.

## 3. Criterios de Actualización de Artículos

Durante el proceso de importación se aplican las siguientes reglas sobre los datos de cada artículo:

* Tipo de artículo: Si el artículo ya tiene asignado un tipo de artículo, se respeta el valor existente y no se sobrescribe.
* Familia: Se actualiza siempre con el valor indicado en la tarifa importada.
* Nombre del artículo: Se respeta siempre el nombre que ya tenga el artículo en el programa; no se modifica con el de la tarifa.

### 3.1. Tarifas de compra

* Tarifa secundaria: Si la referencia del artículo se localiza como tarifa de compra secundaria, se actualizan sus datos.
* Tarifa preferente: Se marca automáticamente la tarifa de este proveedor como preferente para el artículo.

## 4. Comportamiento según Configuración de Empresa

<table data-header-hidden><thead><tr><th valign="top">Configuración</th><th valign="top">Comportamiento</th></tr></thead><tbody><tr><td valign="top">Configuración</td><td valign="top">Comportamiento</td></tr><tr><td valign="top">Empresa multicentro</td><td valign="top">La tarifa importada se aplica sobre todos los centros de la empresa.</td></tr><tr><td valign="top">Empresa monocéntrico</td><td valign="top">La tarifa se aplica directamente sobre la empresa.</td></tr></tbody></table>

{% hint style="info" %}
_En ambos casos, las tarifas de compra del proveedor se marcan como preferentes en todos los centros con más de uno._
{% endhint %}
