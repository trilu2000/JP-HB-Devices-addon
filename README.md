# JP-HB-Devices-addon [![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/) [![Github All Releases](https://img.shields.io/github/downloads/jp112sdl/JP-HB-Devices-addon/total.svg)](https://github.com/jp112sdl/JP-HB-Devices-addon/releases) [![GitHub issues](https://img.shields.io/github/issues/jp112sdl/JP-HB-Devices-addon.svg)](https://github.com/jp112sdl/JP-HB-Devices-addon/issues)

**:heavy_check_mark: lauffähig unter CCU / RaspberryMatic Firmware 2.31.x - 2.45.6 | 3.37.x - 3.45.7**<br/>

Die jeweils aktuellste Version ist bei den [Releases](https://github.com/jp112sdl/JP-HB-Devices-addon/releases/latest) zu finden.

**Das Wichtigste vorweg:**<br/>
Dieses Addon integriert die unten aufgelisteten HomeBrew Projekte in die CCU-Firmware.</font><br/>
Ich stelle es 
* kostenfrei 
* ohne jeglichen Anspruch auf vollständige Funktion 
* auf eigene Gefahr (z.B. unerwünschte Nebeneffekte in der CCU-Firmware)

zur Verfügung.<br/>
Da es sich um ein reines Hobby-Projekt handelt, kann ich **weder (umfangreichen) Support** leisten, **noch auf individuelle Wünsche eingehen** oder **zeitnah die neueste CCU-Firmware unterstützen**!<br/>
Es sollte klar sein, dass mit (m)einer eventuellen Aufgabe dieses Hobbys, mittel-/langfristig (teilweise) keine Verwendung u.g. Geräte mehr möglich ist. _Jedoch steht es jedem frei, sich an den Quellen zu bedienen und das Addon weiterzuentwickeln._

Nach der Installation wird ein Neustart der Zentrale durchgeführt.<br/>
Die eigentliche Installation des Addons erfolgt nach diesem Neustart.<br/>
Währenddessen werden ReGa und der RFD gestoppt, so dass es im Browser zu der Meldung<br/>`Eine Komponente der Homematic Zentrale reagiert nicht mehr.` kommen kann.<br/>
_Bitte etwas Geduld haben - je nach Geschwindigkeit der SD Karte kann die Installation u.U. mehrere Minuten in Anspruch nehmen!_<br/><br/>

Dieses Addon wird benötigt, um die Kompatibilität der folgenden HomeMatic Selbstbaugeräte herzustellen:

|  | Name | Beschreibung | 🔋Batterie-/<br/>⚡️Netzbetrieb |
|--------|--------|--------|:--------:|
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-cap-moist_thumb.png" width=25/> | [HB-UNI-Sen-CAP-MOIST](https://github.com/jp112sdl/HB-UNI-Sen-CAP-MOIST) | kapazitiver Bodenfeuchtesensor | 🔋 |
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-cap-moist-t_thumb.png" width=25/> | [HB-UNI-Sen-CAP-MOIST-T](https://github.com/jp112sdl/HB-UNI-Sen-CAP-MOIST-T) | kapazitiver Bodenfeuchtesensor<br/>mit DS18B20 Temperatursensor| 🔋 |
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-dist-tof_thumb.png" width=25/> | [HB-UNI-Sen-DIST-TOF](https://github.com/jp112sdl/HB-UNI-Sen-DIST-TOF) | Time-of-Flight Abstandsensor | 🔋 |
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-dist-us_thumb.png" width=25/> | [HB-UNI-Sen-DIST-US](https://github.com/jp112sdl/HB-UNI-Sen-DIST-US) | Ultraschall Abstandsensor | 🔋 |
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-lev-tof_thumb.png" width=25/> | [HB-UNI-Sen-LEV-TOF](https://github.com/jp112sdl/HB-UNI-Sen-LEV-TOF) | Time-of-Flight Füllstandsensor | 🔋 |
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-lev-us_thumb.png" width=25/> | [HB-UNI-Sen-LEV-US](https://github.com/jp112sdl/HB-UNI-Sen-LEV-US) | Ultraschall Füllstandsensor | 🔋 |
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-press_thumb.png" width=25/> | [HB-UNI-Sen-PRESS](https://github.com/jp112sdl/HB-UNI-Sen-PRESS) | Drucksensor | ⚡️ |
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-temp-ds18b20_thumb.png" width=25/> | [HB-UNI-Sen-TEMP-DS18B20](https://github.com/jp112sdl/HB-UNI-Sen-TEMP-DS18B20) | 1..8fach DS18B20 Temperatursensor | ⚡️ / 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-wea_thumb.png" width=25/> | [HB-UNI-Sen-WEA](https://github.com/jp112sdl/HB-UNI-Sen-WEA) | Wetterstation | ⚡️ | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-senact-4-4_thumb.png" width=25/> | <strike>[HB-UNI-SenAct-4-4](https://github.com/jp112sdl/HB-UNI-SenAct-4-4)</strike> | <strike>4fach - Sender & - Aktor</strike> | ⚡️ / 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-senact-8-8_thumb.png" width=25/> |  <strike>[HB-UNI-SenAct-8-8](https://github.com/jp112sdl/HB-UNI-SenAct-8-8) <strike> | <strike>8fach - Sender & - Aktor</strike> | ⚡️ / 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-rgb-led-ctrl_thumb.png" width=25/> | [HB-UNI-RGB-LED-CTRL](https://github.com/jp112sdl/HB-UNI-RGB-LED-CTRL) | RGB Controller für WS28xx / Neopixel / etc. | ⚡️ / 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-temp-ir_thumb.png" width=25/> | [HB-UNI-Sen-TEMP-IR](https://github.com/jp112sdl/HB-UNI-Sen-TEMP-IR) | MLX90614 Infrarot Temperatursensor | 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-dummy-beacon_thumb.png" width=25/> | [HB-UNI-Sen-DUMMY-BEACON](https://github.com/jp112sdl/HB-UNI-Sen-DUMMY-BEACON) | Dummy-Device zum Simulieren<br/>zyklischer Statusmeldungen sowie Ack-Nachrichten | ⚡️ / 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-volt_thumb.png" width=25/> | [HB-UNI-Sen-VOLT](https://github.com/jp112sdl/HB-UNI-Sen-VOLT) | universeller Spannungssensor (Template) | 🔋 |  
|<img src="https://github.com/eq-3/occu/blob/master/WebUI/www/config/img/devices/50/PushButton-2ch-wm_thumb.png" width=25/> | [HB-LC-Sw1PBU-FM](https://github.com/jp112sdl/Beispiel_AskSinPP/tree/master/examples/HB-LC-Sw1PBU-FM) | alternative Firmware für den<br/>HM-LC-Sw1PBU-FM (getrennte Taster-/Relais-Kanäle) | ⚡️ | 
|<img src="https://github.com/eq-3/occu/blob/master/WebUI/www/config/img/devices/50/PushButton-2ch-wm_thumb.png" width=25/> | [HB-LC-Sw2PBU-FM](https://github.com/jp112sdl/Beispiel_AskSinPP/tree/master/examples/HB-LC-Sw2PBU-FM) | alternative Firmware für den<br/>HM-LC-Sw2PBU-FM (getrennte Taster-/Relais-Kanäle) | ⚡️ | 
|<img src="https://github.com/eq-3/occu/blob/master/WebUI/www/config/img/devices/50/PushButton-2ch-wm_thumb.png" width=25/> | [HB-LC-Bl1PBU-FM](https://github.com/jp112sdl/Beispiel_AskSinPP/tree/master/examples/HB-LC-Bl1PBU-FM) | alternative Firmware für den<br/>HM-LC-Bl1PBU-FM (getrennte Taster-/Relais-Kanäle) | ⚡️ | 
|<img src="https://github.com/eq-3/occu/blob/master/WebUI/www/config/img/devices/50/5_hm-lc-sw2-fm_thumb.png" width=25/> | [HB-LC-Sw2-FM](https://github.com/stan23/HB-LC-Sw2-FM) | alternative Firmware für den<br/>HB-LC-Sw2-FM (getrennte Taster-/Relais-Kanäle) special thx to [stan23](https://github.com/stan23)! | ⚡️ | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-dmx-master_thumb.png" width=25/> | [HB-UNI-DMX-Master](https://github.com/jp112sdl/HB-UNI-DMX-Master) | (sehr) einfacher DMX Master Controller | ⚡️ |  
|<img src="src/addon/www/config/img/devices/50/hb-dis-ep-42bw_thumb.png" width=25/> | [HB-Dis-EP-42BW](https://github.com/jp112sdl/HB-Dis-EP-42BW) | 4.2" ePaper Display | 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-rfid-rc_thumb.png" width=25/> | [HB-UNI-Sen-RFID-RC](https://github.com/jp112sdl/HB-UNI-Sen-RFID-RC) | RFID-Reader als Sender (Tasterschnittstelle) | ⚡️ | 
|<img src="src/addon/www/config/img/devices/50/hb-ibut-8_thumb.png" width=25/> | [HB-IBUT-8](https://github.com/pa-pa/AskSinPP/tree/master/examples/custom/HB-IBUT-8) | iButton Sender Taster/Schließer | ⚡️ | 
|<img src="src/addon/www/config/img/devices/50/hb-ou-mp3-led_thumb.png" width=25/> | <strike>[HB-OU-MP3-LED](https://github.com/jp112sdl/HB-OU-MP3-LED)</strike> | <strike>MP3-Player mit LED</strike> | ⚡️ | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-weight_thumb.png" width=25/> | [HB-UNI-Sen-WEIGHT](https://github.com/jp112sdl/HB-UNI-Sen-WEIGHT) | universeller Wägesensor | 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-uni-sen-iaq_thumb.png" width=25/> | [HB-UNI-Sen-IAQ](https://github.com/jp112sdl/HB-UNI-Sen-IAQ) | universeller Luftgütesensor _(temporarily discontinued)_ [(see HM-Forum)](https://homematic-forum.de/forum/viewtopic.php?f=76&t=49422)| 🔋 | 
|<img src="src/addon/www/config/img/devices/50/hb-rc-12-ep-bw_thumb.png" width=25/> | [HB-RC-12-EP](https://github.com/jp112sdl/HB-RC-12-EP) | 12 Kanal Fernbedienung mit Farb- oder Schwarz/Weiß-ePaper-Display | 🔋 | 

Zu diesem Zweck ist die [aktuellste Version](https://github.com/jp112sdl/JP-HB-Devices-addon/releases/latest) des Addons herunterzuladen und wie gewohnt in der WebUI über "Einstellungen"->"Systemsteuerung"->"Zusatzsoftware" zu installieren.
<br>_Wie immer bei Addons der Hinweis:<br>Die heruntergeladene Datei mit der Endung `.tgz` darf nicht entpackt werden!_

**Hinweis, falls bereits die früheren einzelnen Addons aus den jeweiligen Projekten genutzt werden:**<br>
Die Addons **müssen zuerst deinstalliert** werden.<br>
Anschließend muss das JP-HB-Devices-addon installiert werden.<br>
Zwischenzeitlich darf **kein Reboot** erfolgen! _(Es erfolgt nach der Installation ohnehin automatisch ein Neustart.)_<br>
Achtung: Bereits angelernte Selbstbaugeräte sind nach dem Neustart u.U. im Posteingang wiederzufinden!

**Info:** Bisher verwendete IDs der Device Model meiner HB-Geräte

| Device Model | Gerät |
|--------|--------|
|E9 01 | HB-UNI-Sen-PRESS |
|E9 02 | HB-UNI-Sen-PRESS-SC |
|F1 D0 | HB-UNI-Sen-WEA |
|F1 D1 | HB-UNI-Sen-IAQ |
|F2 06 | HB-IBUT-8 |
|F3 11 | HB-UNI-Sen-CAP-MOIST |
|F3 12 | HB-UNI-Sen-CAP-MOIST-T |
|F3 01 | HB-UNI-Sen-TEMP-DS18B20 |
|F3 08 | HB-UNI-Sen-TEMP-IR |
|F3 20 | HB-LC-SW12-FM |
|<strike>F3 31</strike> | <strike>HB-UNI-SenAct-4-4-SC</strike>|
|<strike>F3 32</strike> | <strike>HB-UNI-SenAct-4-4-RC</strike>|
|<strike>F3 33</strike> | <strike>HB-UNI-SenAct-4-4-SC-BAT</strike>|
|<strike>F3 34</strike> | <strike>HB-UNI-SenAct-4-4-RC-BAT</strike>|
|F3 35 | HB-LC-Sw1PBU-FM|
|F3 36 | HB-LC-Sw2PBU-FM|
|F3 37 | HB-LC-Bl1PBU-FM|
|<strike>F3 38</strike> | <strike>HB-UNI-SenAct-8-8-RC</strike>|
|<strike>F3 39</strike> | <strike>HB-UNI-SenAct-8-8-RC-BAT</strike>|
|<strike>F3 3A</strike> | <strike>HB-UNI-SenAct-8-8-SC</strike>|
|<strike>F3 3B</strike> | <strike>HB-UNI-SenAct-8-8-SC-BAT</strike>|
|F3 3C | HB-UNI-Sen-RFID-RC|
|F3 41 | HB-UNI-RGB-LED-CTRL |
|F3 42 | HB-UNI-DMX-MASTER |
|F3 43 | HB-DIS-EP-42BW |
|<strike>F3 44</strike> | <strike>HB-OU-MP3-LED</strike> |
|F3 45 | HB-RC-12-EP-29C |
|F3 46 | HB-RC-12-EP-29BW |
|F3 4A | HB-UNI-Sen-VOLT |
|F3 4B | HB-UNI-Sen-WEIGHT |
|F3 53 | HB-DIS-EP-42BW-MAINS |
|F3 FF | HB-UNI-Sen-DUMMY-BEACON |
|F5 01 | HB-LC-Sw2-FM |
|F9 D6 | HB-UNI-Sen-DIST-US |
|F9 D7 | HB-UNI-Sen-DIST-TOF |
|F9 D2 | HB-UNI-Sen-LEV-US |
|F9 D3 | HB-UNI-Sen-LEV-TOF |


<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons Lizenzvertrag" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />Dieses Werk ist lizenziert unter einer <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Namensnennung - Nicht-kommerziell - Weitergabe unter gleichen Bedingungen 4.0 International Lizenz</a>.

Die verwendeten Icons sind "free for non-commercial use" von
 - https://www.flaticon.com/authors/popcic from www.flaticon.com 
 - http://icons8.com 
