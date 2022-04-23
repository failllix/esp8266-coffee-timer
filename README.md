# ESP8266 espresso shot timer
An espresso shot timer based on gyroscope measurements. To be used with vibration pumps.

## Parts needed
- Wemos D1 Mini
- OLED Display (e.g. AZ-delivery 0.91 inch OLED I2C)
- Gyroscope sensor (e.g. AZ-delivery GY-521 MPU-6050)

## How it works
The gyroscope measures the vibrations of the pump to start a timer that is being displayed on the OLED display. The vibrations of the three axis are added together and squared to strenghten small vibrations. Afterwards during a certail interval multiple measurements are taken to evaluate the strength of vibration. If the strength passes a certain threshold the timer is started.
