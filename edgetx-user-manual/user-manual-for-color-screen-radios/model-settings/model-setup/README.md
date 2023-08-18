---
description: Ajustes generales del modelo
---

# Model Setup

<div align="center">

<figure><img src="../../../../.gitbook/assets/modelsetup.png" alt=""><figcaption><p>Pestaña de ajustes en la pantalla de configuración</p></figcaption></figure>

</div>

La página **model setup (ajustes del modelo)** es la página por defecto que aparece en la pantalla de configuración del modelo. Es el inicio de la configuración. Contiene los siguientes ajustes:

#### Model name (nombre del modelo)

Se ingresa el nombre del modelo con un máximo de 15 caracteres.

#### Labels (etiquetas)

Aquí es posible asignarle al modelo, una etiqueta de las que se encuentran en la lista de etiquetas ya definida. Por defecto aparece asignada la etiqueta **Unlabeled. (sin etiqueta)** Para más información sobre la creación de etiquetas, ver [select-model.md](../../select-model.md "mention") .

#### Model image (imagen)

Mediante este botón se puede seleccionar una imagen para el modelo, de la lista de imágenes que se encuentra en la carpeta "images" de la tarjeta SD.

{% hint style="info" %}
Para evitar problemas de rendimiento. La imagen no debe exceder, 192 X 114 pixeles. Para más información sobre los requerimientos de la imagen, ver por favor la parte **Images** de la sección [SD Card (tarjeta SD)](../../radio-settings/sd-card.md).
{% endhint %}

{% hint style="info" %}
[https://www.skyraccoon.com/](https://www.skyraccoon.com/) Contiene un gran repositorio de imágenes de libre uso que pueden utilizarse en EdgeTX.
{% endhint %}

#### Use global functions (funciones globales)

Habilita o no, el uso de las funciones globales en este modelo.

{% hint style="info" %}
_Global functions_ (Funciones globales)_ son funciones especiales que pueden ser aplicadas a todos los modelos. Ver [Special _Functions_(funciones especiales)](../special-functions.md) para mas información sobre su configuración.
{% endhint %}

#### ADC Filter

Enables/disables the ADC filter for this model. The _**global**_ option will take the value designated in the radio settings, which is _on_ by default.

{% hint style="info" %}
The ADC filter is a filter for the proportional channels (sticks, pots, sliders), smoothing out smaller fast movements that occur due to noise in the system electronics. Normally, this filter should be _disabled_ for models with flight controllers.
{% endhint %}



