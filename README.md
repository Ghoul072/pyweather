# PyWeather


## What is PyWeather
PyWeather is a Pythonic API for weather and geolocation, powered by [WeatherAPI](https://www.weatherapi.com/)


<!-- ## Installation

Use [pip](https://pip.pypa.io/en/stable/) package manager to install PyWeather.

```bash
pip install pyweather
``` -->
## Installation

WeatherAPI is available on [PyPI](https://pypi.org/) and can be installed by running the below command:
```
pip install weatherapi
```


## Usage

This package is designed to be as easy as possible to use. Simply create a client object using your API Key as shown below and all commands are available as methods under the newly created client object

```python
import pyweather

#create a PyWeather client using your API key from www.weatherapi.com
client = pyweather.Client("YOUR_KEY_HERE")
weather = client.current("London")  # checks and returns current weather
print(weather.condition)            # print current weather condition
print(weather.feelslike_c)          # print feelslike in celsius

# Check the location using an IP address
my_ip = client.ip_lookup("209.142.68.29")
print(my_ip.country_name)

```


## Contributing

Pull requests are welcome. For major changes, please open an [issue](https://github.com/Ghoul072/weather/issues) first
to discuss what you would like to change.


## License

MIT
