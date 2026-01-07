🌫️ IoT Air Quality Monitor (ESP8266 + Blynk)
A compact Wi-Fi enabled air quality monitoring system built using NodeMCU ESP8266.
It continuously measures air pollution levels along with temperature and humidity, displays data locally on an OLED, and syncs everything to the Blynk IoT Cloud for remote monitoring and alerts.
Designed for homes, labs, server rooms, and indoor spaces where air safety matters.

✨ Features
📊 Real-time air quality monitoring (PPM)
🌡️ Temperature & humidity sensing
🖥️ Live OLED display (standalone operation)
📱 Remote monitoring via Blynk mobile app
🚨 Automatic visual & audio alerts
🔕 Manual siren mute using hardware button
🌐 Works over Wi-Fi (ESP8266)

🔧 Hardware Used
NodeMCU ESP8266
MQ135 Air Quality Sensor
DHT11 Temperature & Humidity Sensor
0.96" OLED Display (SSD1306, I2C)
Active Buzzer
Push Button
Status LEDs (Green / Yellow / Red)

🧠 How It Works
MQ135 detects harmful gases and outputs an analog signal.
DHT11 provides temperature and humidity data.
ESP8266 processes sensor values and estimates air quality in PPM.

System categorizes air quality into:
Safe
Moderate
Dangerous
Status is shown locally on an OLED display.
Data is sent to Blynk Cloud every few seconds.

When pollution exceeds safe limits:
Red LED turns ON
Buzzer activates
Mobile alert is triggered
A physical button allows muting the siren without disabling alerts.

🚦 Air Quality Levels
PPM Range
Status
Indication
< 150
Safe
Green LED
150 – 350
Moderate
Yellow LED
> 350
Dangerous
Red LED + Buzzer
> 
📲 Blynk Dashboard
The Blynk app provides:
Live AQI, temperature & humidity values
Visual indicators matching hardware LEDs
Remote access from anywhere
Push notifications during hazardous conditions
Works even when you’re not near the device.

🖥️ Local Display
The OLED shows:
Air quality value (PPM)
Temperature & humidity
System status (Wi-Fi & siren state)
This allows the device to function without a phone.

🧪 Calibration Note
MQ135 sensors require:
Warm-up / burn-in time
Baseline adjustment for stable readings
This project includes software offset correction to avoid false high values in clean air.
