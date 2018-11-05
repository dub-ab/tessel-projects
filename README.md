# tessel-projects
a sandbox for all projects created at https://bocoup.com/blog/say-hello-world-with-johnny-five-on-tessel-2

[//]: # (To view in Preview Mode: Ctrl+Shift+V)

# Monitor Project
The goal of the monitor project is to display various web service and localized sensor data on a connected TFT LCD display.

## Hardware

The hardware for this project is:

- 1 x WeMos Mini D1
    - Approximately cost $5.00.
- 1 x 1.8 Inch TFT LCD Display Module
    - Approximate cost $6.00.
- 1 x DHT22/AM2302 Digital Temperature And Humidity Sensor
    - Approximately cost $5.00.

Wiring as follows:

| TFT           | WEMOS (PIN)   | Color     |
| :------------ |:-------------:| ---------:|
| Vcc           | 5v            |  brown    |
| GND           | GND           |    red    |
| 3             |               |           |
| 4             |               |           |
| 5             |               |           |
| 6             |               |           |
| 7             |               |           |
| 3v3           |      3v3      |     grey  |

## Software
- Upon power up, if connection details have been saved previously the device will connect to the local WiFi network.
- If no connection details are saved it will function as an access-point, allowing you to specify the appropriate WiFi network.
- The device will fetch the date & time via NTP.
- The device will fetch weather-details from openweathermap.org.
- The device will fetch stock details from alphavantage.co
- The TFT LCD screen will alternate between three displays:
    - The current date & time.
    - The current weather conditions.
    - Current intraday time series data.
- The web browser display data as well as allow configuration of settings.

This project requires a **free** API-key from the [OpenWeatherMap](https://openweathermap.org/appid) service and a **free** API-key from [Alpha Vantage](https://www.alphavantage.co/support/#api-key).


## License
[MIT](https://choosealicense.com/licenses/mit/) dub-ab 
