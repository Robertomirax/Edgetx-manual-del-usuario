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
Para evitar problemas de rendimiento. La imagen no debe exceder, 192 X 114 pixeles. Para más información sobre los requerimientos de la imagen, ver por favor la sección **Images** portion of the [SD Card (tarjeta SD)](../../radio-settings/sd-card.md) section.
{% endhint %}

{% hint style="info" %}
[https://www.skyraccoon.com/](https://www.skyraccoon.com/) has a large repository of free image files that can be used with EdgeTX.
{% endhint %}

#### Use global functions

When enabled, global functions programmed in the radio settings will apply to this model. When disabled, global functions will not apply to this model.

{% hint style="info" %}
_Global functions_ are _special functions_ that are applied across all models. Refer to [Special _Functions_](../special-functions.md) for information on configurable settings.
{% endhint %}

#### ADC Filter

Enables/disables the ADC filter for this model. The _**global**_ option will take the value designated in the radio settings, which is _on_ by default.

{% hint style="info" %}
The ADC filter is a filter for the proportional channels (sticks, pots, sliders), smoothing out smaller fast movements that occur due to noise in the system electronics. Normally, this filter should be _disabled_ for models with flight controllers.
{% endhint %}



