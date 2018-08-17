# map-conversion
Converting a Google Map from My Maps to a leaflet.js Open Street Map for a more customisable map

This is a project made for http://thecarlsarecoming.com
It's probably horribly inefficient

## What it does
The page fetches the data from your My Maps project as a KML file and parses it and butchers it until it gets the coordinates, the title and the description. It then adds the coordinates as new markers on the Leaflet Open Street Map and adds a custom marker image.

## Requirements
You'll need Leaflet, get it here: https://leafletjs.com/
Don't forget to replace the addresses in the code for leaflet.css and leaflet.js to the path of your downloaded Leaflet files.

You'll also want to replace the map with your own map from My Maps. To do that, go to your map, and in the options, click "Download KML". Choose which part of the map you want to export, activate both checkboxes ("Keep data up to date with network link KML (only usable online)." will give you the link, "Export to a .KML file (for full icon support, use .KMZ)." will make sure you will get the human readable KML instead of the KMZ) and download the file. Then look for the address in the KML and copy it from there
Or you can just change the MID in the address. That's probably easier.

Also change the address in changeMarkerImage with your own marker. Or delete it if you don't need it. You can always change the original image files anyway.
