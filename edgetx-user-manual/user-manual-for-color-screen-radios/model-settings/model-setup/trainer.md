# Trainer

<figure><img src="../../../../.gitbook/assets/trainer1.png" alt=""><figcaption><p>Pantalla modo instructor (Trainer)</p></figcaption></figure>

 En la pantalla**Trainer** se puede configurar el modo de transferencia de las señales CPPM (CPPM es una señal que combina la información de todos los canales en una sola señal que puede transmitirse mediante un único cable). Cuando este modo está habilitado, las señales CPPM pueden transferirse desde una radio que esté en modo esclavo _**Slave**_ a otra radio en que esté en modo maestro _**Master**_. Esta última, podrá tranferir a su vez estas señales, al modelo que esté controlando. La transferencia CPPM puede usarse para varias aplicaciones, tales como: Conexión de un rastreador de cabeza (head tracker), modo de entrenamiento Instructor / Estudiante, control de modelos complejos que requieren mas palancas de mando de las disponibles en los transmisores comunes.&#x20;

**Master mode (modo Maestro)** - Modo para la radio enlazada con el modelo. Esta radio, también deberá tener configurada la función global especial **Trainer (Instructor)** para activar el modo de transferencia. Cuando el modo de transferencia esté activado, las señales CCPM provenientes de la radio en modo esclavo _**Slave mode (modo esclavo)**_ serán enviadas al modelo controlado.

**Slave mode (modo esclavo)** - Este es el modo en que debe estar la radio que enviará sus señales CPPM a la radio en _**Master mode (modo Maestro)**_ la cual enviará estas señales al modelo.

Opciones de configuración:

* **Off (desactivado)** - No se usará el modo instructor (Trainer) para este modelo.&#x20;
* **Master / Jack** - Modo maestro (Master) usando un cable de conexión.
* **Slave / Jack** - Modo esclavo (Slave) usando un cable de conexión.
  * **Channel Range (rango de canales)** - Este es el número de canales que serán enviados a la radio maestra (Master). Se recomienda que el canal 10 sea el último canal usado.
  * **PPM Frame** - El primer campo es la duración de la secuencia de señales PPM. El segundo campo es el retardo entre pulsos. El tercer campo selecciona la polaridad de la señal. Al cambiar la cantidad de canales enviados, se ajusta automáticamente la duración del tren de pulsos a su valor correcto. Sin embargo, este valor puede ajustarse manualmente. _**Nota**: En la mayoría de los casos, _no es necesario cambiar el valor asignado por defecto._
* **Master / Bluetooth** - Modo Maestro (Master) usando una conexión Bluetooth. Si la radio cuenta con Bluetooth.
* **Slave / Bluetooth** - Modo esclavo (Slave) usando una conexión Bluetooth. Si la radio cuenta con Bluetooth.
* **Master / Multi** - Modo maestro (Master) usando un módulo Multi-protocol. Ver mas información en[set-up-wireless-trainer-with-mpm.md](../../../../edgetx-how-to/set-up-wireless-trainer-with-mpm.md "mention")

{% hint style="info" %}
Puede encontrarse mas información en la configuración del modo entrenador en [trainer.md](../../radio-settings/trainer.md "mention")
{% endhint %}

