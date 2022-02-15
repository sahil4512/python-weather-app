# Python Weather App

Python Weather App Build with [Open Weather](https://openweathermap.org/current#geocoding) API.

## How to Use

- Create a new account on [Open Weather Sign Up](https://home.openweathermap.org/users/sign_up)
- Generate a new API Key
- Add key to Secrets.ini file 

```bash
[openweather]
api_key= <YOUR-OPENWEATHER-API-KEY>
```


## Usage

- Used ConfigParser to Fetch the API key from your configuration file
- Used argparse Handles the CLI user interactions

- shows weather for any city around the world (temperature, feels like , humidity)
- show temperature in celsius by default and you pass a parameter as -i for fahrenheit
- pass -h for help

```python
python weather.py -h

usage: weather.py [-h] [-i] city [city ...]

gets weather and temperature information for a city in any language !

positional arguments:
  city            enter the city name

optional arguments:
  -h, --help      show this help message and exit
  -i, --imperial  display the temperature in imperial units


# Example 
python weather.py city

python weather.py toronto

Toronto  💨   Overcast clouds (-10.61 °C) | Feels like (-13.49 ) °C | Humidity 65 🟠

python weather.py toronto -i 

Toronto 💨   Overcast clouds (12.83 °F) | Feels like (12.83 ) °F | Humidity 63 🟠
```
