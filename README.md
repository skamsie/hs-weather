# hs-weather

Weather menubar app for [hammerspoon](http://www.hammerspoon.org) users.

### Setup

1. Copy the repo to your hammerspoon folder. 
```cp -r hs-weather ~/.hammerspoon```
2. Add this to your init.lua
```
local weather = require("hs-weather")
weather.start()
```
3. Modify config.json to suit your needs  
  - ```geolocation: true``` => if hammerspoon has location services enabled, will get weather for current location and the ```location``` parameter will be ignored

Now the weather should be shown in the menu bar.

[![Screen Shot 2016-08-21 at 2.37.41 PM.png](https://s10.postimg.org/e9djfzq6x/Screen_Shot_2016_08_21_at_2_37_41_PM.png)](https://postimg.org/image/rdj3soi8l/)

**NOTES**
- click updates weather
- hover shows last yahoo update for the location
- if right after opening hammerspoon it shows N/A, just click to retry (this happens because sometimes yahoo returns an empty response for the location)
- Config can also be passed as an argument to weather.start() e.g.
```
local weather = require("hs-weather")
weather.start({
  geolocation = true,
  units = 'F'
})
```
- Default refresh is 5 minutes
- Disable by calling ```weather.stop()```

### Credits

Weather data: [Yahoo Weather API](https://developer.yahoo.com/weather/). It does not require an api key.  
Icons by RNS, Freepik, Vectors Market, Yannick at http://www.flaticon.com
