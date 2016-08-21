# hs-weather

Weather menubar app for [hammerspoon](http://www.hammerspoon.org) users.

### Setup

1. Copy the repo to your hammerspoon folder. Must be in ~/.hammerspoon (it is there by default)  
```cp -r hs-weather ~/.hammerspoon```
2. Add this to your init.lua ```require("hs-weather.menuapp")```
3. Modify config.json to suit your needs  

Now the weather should be shown in the menu bar. It displays additional info on hover.

[![Screen Shot 2016-08-21 at 2.37.41 PM.png](https://s10.postimg.org/e9djfzq6x/Screen_Shot_2016_08_21_at_2_37_41_PM.png)](https://postimg.org/image/rdj3soi8l/)

### Credits

Weather based on the [Yahoo Weather API] (https://developer.yahoo.com/weather/). It does not require an api key.  
The ```json.lua``` file by Jeffrey Friedl http://regex.info/blog/lua/json  
Icons by RNS, Freepik, Vectors Market, Yannick at http://www.flaticon.com
