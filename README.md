Raspberry Pi LED Vezérlés – Telepítési Útmutató

Ez az útmutató bemutatja, hogyan telepítsd és futtasd a LED vezérlő projektet Raspberry Pi-n.
-   Másold fel a letöltött ZIP fájlt a Raspberry Pi-re (például scp segítségével).
-  Csomagold ki a ZIP fájlt: unzip raspi-led-control.zip.
-  Lépj be a projekt mappába: cd raspi-led-control.
-  Telepítsd a szükséges függőségeket: npm install.
-  Indítsd el a szervert (GPIO miatt sudo szükséges): sudo node server.js.
-  Nyisd meg a böngészőben a Raspberry Pi IP címét: http:///.
-  A webes felületen vezérelheted a LED-eket (Bekapcsol/Kikapcsol gombok).

Megjegyzés: A projekt a GPIO lábak vezérléséhez az rpio könyvtárat használja, ezért a futtatáshoz
rendszergazdai jogosultság szükséges
- scp -r raspi-led-control pi@<IP_CÍM>:/home/pi/
- unzip raspi-led-control.zip
- cd raspi-led-control
- npm install
- sudo node server.js
- http://<RaspberryPi_IP>/
