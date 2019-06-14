# ArduinoWifiRev2

For å koble Arduino Uno WIFI Rev2 til internett er det gunstig å koble til alt annet enn Eduroam. For eksempel internettdeling via mobildata eller et privat nettverk. 

En guide som kan brukes for å prøve å kommunisere med mikrokontrolleren finner man på [hjemmesiden](https://www.arduino.cc/en/Guide/ArduinoUnoWiFiRev2). [WoolseyWorkshop](https://www.woolseyworkshop.com/2018/12/07/controlling-an-arduino-uno-wifi-rev2-or-arduino-uno-with-wifi-shield-from-a-web-browser/) har også en bra guide for å kommunisere via en nettside.
# Problemer underveis

Underveis har det dukket opp en del problemer. Noen var enklere å løse enn andre og her vil det bli nevnt noen som har dukket opp. Det oppfordres til å søke på nettet om du støter på et problem:

- [arduino.stackexchange](https://arduino.stackexchange.com/)
- [forum.arduino](https://forum.arduino.cc/index.php?board=126.0)
- [google](www.google.com)

Problemer:
- **Serial.print()** skriver ikke ut det du forventer til **Serial monitor**:
  - Sørg for at koden faktisk kan kompileres. Deretter sørg for at baud rate i **Serial monitor** er lik det du har i **Serial.begin(*baud rate*)** under **setup()**.
- Kan ikke laste inn angitt IP-adresse fra **Serial monitor** i Chrome eller Firefox:
  - Sørg for at datamaskinen er koblet til samme nettverk som Arduinoen før du laster inn siden igjen.
