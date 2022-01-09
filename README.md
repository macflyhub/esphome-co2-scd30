# esphome-co2-scd30
  
Using ESPHOME with Home Assistant and a Sensirion SCD30 CO2 Sensor with a ESP32 (Don't use ESP8266)  
Link: https://www.sensirion.com/en/environmental-sensors/carbon-dioxide-sensors/carbon-dioxide-sensors-scd30/  
Datasheet: https://www.sensirion.com/fileadmin/user_upload/customers/sensirion/Dokumente/9.5_CO2/Sensirion_CO2_Sensors_SCD30_Datasheet.pdf  
ESPHome SCD30: https://esphome.io/components/sensor/scd30.html  
  
This is a really good sensor with great accuracy and highly recommended.  
  
A big thank you to the amazing team working on Home Assistant and ESPHome.  
This has to be the best smart home solution in the world and exceeds all of the commercial systems out there.  
  
NOTE: The SCD30 CO2 Sensor does NOT work [currently] with ESPHome when using a ESP8266 for some reason, you will need an ESP32 to get this working.  
  
The YAML example code is simply a working version (edit your passwords in) of the code required to get your project started.  
  
ESP32 PINOUT  
ESP PIN D21 to SCD30 SCA  
ESP PIN D22 to SCD30 SCL  
ESP PIN 3.3V to SCD30 VIN  
ESP PIN GND to SCD30 GND  
ESP PIN GND to SCD30 SEL  
  
As per the PIN instructions above the SEL on the SCD30 is grounded to enable I2C  
  
It takes 5 days for Auto calibration or you can manually tweak the settings.  
My unit was about 200 units above true reading to start with.  

Update: Added "automatic_self_calibration: true" as the documentation said "true" was the default but it turned out not to work.
