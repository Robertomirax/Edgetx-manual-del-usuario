# Internal / External RF

Las configuraciones del módulo de RF interno y del externo trabajan de la misma forma. La única diferencia es que la sección **Internal RF** Es para configurar el módulo de RF interno que viene con la radio y la sección **External RF** es para configurar el módulo que se puede instalar en forma externa.

Si el botón es de color amarillo, significa que el módulo correspondiente, se encuentra activo. Si es de color blanco, el módulo está inactivo.

<div>

<figure><img src="../../../../.gitbook/assets/internalrf.png" alt=""><figcaption><p>Módulo multiprotocolo seleccionado en la configuración interna. "Internal RF"</p></figcaption></figure>

 

<figure><img src="../../../../.gitbook/assets/externalrf.png" alt=""><figcaption><p>Módulo CRSF seleccionado en la configuración externa. "External RF"</p></figcaption></figure>

</div>

#### Receiver ID (Número de receptor)

El número de receptor (Receiver ID) es un número asignado por el usuario, que es enviado al receptor, durante el enlace. Cada modelo, debe tener un único número de receptor. Solo pueden tener el mismo número, si los receptores usan protocolos distintos. Aparecerá un aviso, para informar si el número es único o si está previamente usado en otro modelo.

{% hint style="warning" %}
Si se usa la radio como mando de juegos conectado a un computador. Deben deshabilitarse tanto el módulo de RF interno como el externo. Esto mejorará el rendimiento.&#x20;
{% endhint %}

#### Mode Options (modo)

* **Off** - No se usa el módulo de RF
* **PPM** - Modulación por posición de pulso. Se usa en muchos módulos genéricos, compatibles con JR.
  * **Telemetry** - Sin telemetria o MLink
  * **Channel Range** - Canales que serán usados.
  * **PPM Frame** – Duración de la secuencia de pulsos, duración del pulso, y polaridad de la señal PPM. La duración de la secuencia de pulsos, se ajusta automáticamente, cuando cambia el número de canales transmitido. Sin embargo, este valor asignado automáticamente, puede cambiarse de forma manual.
* **XJT** -&#x20;
  * **Protocol**- D16, B8, LR2
  * **Channel Range** - Canales que serán usados.
  * **Failsafe Mode (señal perdida)** - Disponible en protocolo D16. El receptor usará esta configuración, cuando pierda la señal del transmisor.
    * **Not Set** - No está definido el modo de failsafe (señal perdida).&#x20;
    * **Hold** – El receptor mantiene último valor recibido para cada canal luego de perder la señal del transmisor.
    * **No pulses** – El receptor no genera pulsos PWM en sus salidas.
    * **Receiver** – Se ejecuata la configuración de failsafe, que tenga definida el receptor. Ver las instrucciones que vienen con el receptor.
    * **Custom** – El receptor cambia los valores de cada canal a aquellos definidos por el usuario.
      * **Custom Set** – Cada canal puede tener su propia configuración. Las opciones son: un valor, mantener el último valor o no generar pulsos.
  * **Receiver Number** - Un valor asignado por el usuario para cada modelo que es enviado al receptor durante el enlace.
  * **Bind** - Esto coloca el transmisor en modo de enlace con el receptor. En este modo, el transmisor produce un chirrido cada 2,5 segundos.
  * **Range** . Esto coloca el transmisor en el modo de verificación de rango de alcance. Se mostrará el valor de RSSI (indicador de fuerza de la señal recibida, RSSI por las siglas del inglés Received Signal Strength Indicator), y se emitirá un sonido cada 5 segundos.
* **DSM2**
  * **Protocol** - LP45, DSM2, DSMX
  * **Channel Range** - Canales que serán usados.
  * **Receiver Number** -  Un valor asignado por el usuario para cada modelo que es enviado al receptor durante el enlace.
  * **Bind** - Esto coloca el transmisor en modo de enlace con el receptor. En este modo, el transmisor produce un chirrido cada 2,5 segundos.
  * **Range** . Esto coloca el transmisor en el modo de verificación de rango de alcance. Se mostrará el valor de RSSI (indicador de fuerza de la señal recibida, RSSI por las siglas del inglés Received Signal Strength Indicator), y se emitirá un sonido cada 5 segundos.
* **CRSF**
  * **Baud Rate** - Velocidad a la que se establece la comunicación entre la radio y el módulo.
  * **Status** - Muestra la configuración de la transmisión, en el módulo RF.
  * **Channel Range** - Canales que serán usados.
  * **Receiver Number** -  Un valor asignado por el usuario para cada modelo que es enviado al receptor durante el enlace.
* **Multi** - Módulo multiprotocolo. Las opciones de configuración, son únicas para cada protocolo seleccionado. Se describen aqui:  [https://www.multi-module.org/using-the-module/protocol-options](https://www.multi-module.org/using-the-module/protocol-options)
* **R9M**
  * **Mode**- FCC, EU, 868MHz, 915 MHZ
  * **Failsafe Mode (señal perdida)** - Disponible en protocolo D16. El receptor usará esta configuración, cuando pierda la señal del transmisor.
    * **Not Set** - No está definido el modo de failsafe (señal perdida).&#x20;
    * **Hold** – El receptor mantiene último valor recibido para cada canal luego de perder la señal del transmisor.
    * **No pulses** – El receptor no genera pulsos PWM en sus salidas.
    * **Receiver** – Se ejecuata la configuración de failsafe, que tenga definida el receptor. Ver las instrucciones que vienen con el receptor.
    * **Custom** – El receptor cambia los valores de cada canal a aquellos definidos por el usuario.
      * **Custom Set** – Cada canal puede tener su propia configuración. Las opciones son: un valor dado, mantener el último valor o no generar pulsos.
  * **Receiver Number** -  Un valor asignado por el usuario para cada modelo que es enviado al receptor durante el enlace.
  * **Bind** - Esto coloca el transmisor en modo de enlace con el receptor. En este modo, el transmisor produce un chirrido cada 2,5 segundos.
  * **Range** . Esto coloca el transmisor en el modo de verificación de rango de alcance. Se mostrará el valor de RSSI (indicador de fuerza de la señal recibida, RSSI por las siglas del inglés Received Signal Strength Indicator), y se emitirá un sonido cada 5 segundos.
  * **RF Power** - Indica la potencia de salida del módulo transmisor. Las opciones cambian de acuerdo al modo seleccionado.
* **R9M Access    Note:** In order for the mode **R9M ACCESS** to be visible in the mode dropdown**,** the AUX1 or AUX2 serial port must be configured to **External Module** on the [Hardware](../../radio-settings/hardware.md) page.&#x20;
  * **Channel Range** - Channels that will be used.
  * **Failsafe Mode** - The receiver will use this setting when the transmitter signal is not being received (signal loss).
    * **Not Set** - failsafe mode is not set.&#x20;
      * **Hold** – The receiver keeps channel values at their last received state from the transmitter.
      * **No pulses** – No PWM pulses are output.
      * **Receiver** – Follows the fail-safe settings configured on the receiver. Follow the instructions that come with the receiver.
      * **Custom** – The receiver changes the channel values to the custom set values.
        * **Custom Set** – Each channel can have its own setting. The options are a value, hold and no pulses
  * **Module -** _Please refer to FrSky documentation for these configuration settings_
    * Register
      * Range
      * Options
  * **Receiver No (Number)** -  a user-assigned number for a model that is sent to the receiver when bound
  * **Bind** - This puts the transmitter into bind mode. When in this mode the transmitter will make a chirp sound every 2.5 seconds.
* **GHST** - ImmersionRC Ghost
  * **Channel Range** - Channels that will be used.
  * **Raw 12 bits** - enable 12bit mode
* **SBUS**&#x20;
  * **Channel Range** - Channels that will be used.
  * **Refresh Rate** - Rate of refresh in milliseconds
    * **Inversion** - Normal, Non-inverted
* **FLYSKY**&#x20;
  * **Protocol** - AFHDS3, AFHDS2A
  * **Module Status** - Status of the module
  * **Type** - _Please refer to FLYSKY documentation for these configuration settings_
    * **Module Options**- _Please refer to FLYSKY documentation for these configuration settings_
  * **Channel Range** - Channels that will be used.
  * **Failsafe Mode** - The receiver will use this setting when the transmitter signal is not being received (signal loss).
    * **Not Set** - failsafe mode is not set.&#x20;
    * **Hold** – The receiver keeps channel values at their last received state from the transmitter.
    * **No pulses** – No PWM pulses are output.
    * **Receiver** – Follows the fail-safe settings configured on the receiver. Follow the instructions that come with the receiver.
    * **Custom** – The receiver changes the channel values to the custom set values.
      * **Custom Set** – Each channel can have its own setting. The options are a value, hold and no pulses.
  * **Receiver (number)** -  a user-assigned number for a model that is sent to the receiver when bound
  * **Bind** - This puts the transmitter into bind mode. When in this mode the transmitter will make a chirp sound every 2.5 seconds.
* **LemonRx DSMP**
  * **Channel Range** - Channels that will be used.
  * **Bind** - This puts the transmitter into bind mode. When in this mode the transmitter will make a chirp sound every 2.5 seconds.
  * **Range** . This puts the transmitter into range check mode. When in this mode, the RSSI value is displayed and a sound is made every 5 seconds.
