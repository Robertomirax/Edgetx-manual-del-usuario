# Preflight Checks

<figure><img src="../../../../.gitbook/assets/preflightchecks.png" alt=""><figcaption><p>Página de controles pre-vuelo</p></figcaption></figure>

Cada vez que se carga un modelo nuevo, EdgeTX realiza un control pre-vuelo basado en las verificaciones definidas en esta página. Si falla alguna de las verificaciones, EdgeTX le dará al usuario una advertencia visual y audible que debe ser admitida antes de seguir adelante. Se pueden configurar las siguientes opciones:

**Display checklist (mostrar lista de verificaciones)** - Cuando está seleccionada esta opción, se mostrarán en pantalla las notas del modelo cuando este sea cargado. Debe existir un archivo válido en la carpeta **Models** en la tarjeta SD. El archivo de notas debe ser un archivo de texto .txt y debe tener exactamente el mismo nombre que el modelo seleccionado. Por ejemplo: Mobula6.txt. El texto en el archivo depende del usuario.

**Throttle state (estado del acelerador)** - Cuando está seleccionada esta opción, la radio verificará que el acelerador esté en su valor mínimo para la fuente configurada como acelerador en la sección [Throttle (acelerador)](throttle.md).

**Custom Position?** -  When this option is selected, a number box will be shown that can be configured with a user-defined value for the throttle state check. &#x20;

**Switches** - The section displays all the switches that are configured on the radio and allows you to select which position is the correct position for the switch state check. Selecting the switch will cycle through the available switch positions or turn the check off for the switch completely. Yellow switches have the switch position check activated. White switches e de-activated.

**Pots & Sliders**- When activated, this option checks the position of the pots & sliders. There are three options - OFF, ON and AUTO. When ON or AUTO is selected from the drop-down menu, buttons for the available pots and sliders will appear.&#x20;

* **OFF** - Pot and slider positions are not checked.
* **ON** - Positions are checked against manually configured pot and slider positions that are set to active (yellow). To manually set the check position, select ON from the drop-down menu, put the pots and sliders into the desired position, and activate them by selecting them (yellow).
* **AUTO** - Positions are checked for activated pots and sliders and compared to the last automatically saved position before the radio was turned off or the model was changed.

**Center Beep** - Allows you to turn on / off the center beep function for the individual sticks, pots, and sliders by selecting them (yellow).&#x20;
