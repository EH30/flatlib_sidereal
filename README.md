# flatlib_sidereal

Flatlib is a python library for Traditional Astrology.  
flatlib_sidereal was made possible by: joaoventura    
this README was edited by EH30 to give some code examples because there are not many code examples for flatlib_sidereal.

# Example
```
from flatlib.datetime import Datetime
from flatlib.geopos import GeoPos
from flatlib.chart import Chart, const

# Date: 2005-6-27 Time: 6:45 AM UTC: +5:30
date = Datetime([2005, 6, 27], ['+',6,45,0], "+05:30")
pos = GeoPos(19.0760, 72.8777)
print("lat: ", pos.lat, "lng: ", pos.lon)


# Using Ayan Lahiri   
chart = Chart(date, pos, mode=const.AY_LAHIRI)
print(chart.get(const.ASC))
# output: 
# lat:  19.076 lng:  72.8777
# <Asc Gemini +20:04:01>
```   
## Installation
download flatlibe_sidereal      
run powershell as an Administrator and cd to the flatlib_sidereal folder.   
``` 
python setup.py install
```   

## Documentation

Flatlib's documentation is available at [http://flatlib.readthedocs.org/](http://flatlib.readthedocs.org/).



