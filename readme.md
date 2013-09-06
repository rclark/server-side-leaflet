# server-side-leaflet

Use [Leaflet](http://leafletjs.com/) on the server with help from [jsdom](https://github.com/tmpvar/jsdom).

All this does is 

- spoof the `window` and DOM with jsdom, 
- fix the size of the map to 1024x1024, 
- set `L.Icon.Default.imagePath` to some nonsense,
- and then let Leaflet do the rest.

I concatenated [Leaflet.markercluster]() here, in order to use it to do clustering server-side. See [the example](clustering.js).