# ESP8266 Espresso Shot Timer

An espresso shot timer based on gyroscope measurements.
To be used with espresso machines using a vibration pump.

## Parts needed

- Wemos D1 Mini
- OLED Display (e.g. AZ-delivery 0.91 inch OLED I2C)
- Gyroscope sensor (e.g. AZ-delivery GY-521 MPU-6050)

## How it works

The gyroscope measures the vibrations of the pump to start a timer that is being displayed on the OLED display.
The vibrations of the three axis are added together and squared to strenghten small vibrations.
Using a rolling interval, multiple measurements are taken into account to evaluate the current strength of vibration.
If the strength passes the threshold the timer is started / stopped.
