Leaflet Copy Coordinates Control
===========================
Works with Leaflet to capture mouseclicks on a map and display the associated coordinates with an easy way to copy them.

Derived from [original work by zimmicz](https://github.com/zimmicz/Leaflet-Coordinates-Control). Forked mainly to provide npm functionality.

Demo
----

See demo [here](https://tinjaw.github.io/Leaflet-Copy-Coordinates-Control/).

How to use
----------
	var c = new L.Control.Coordinates(); # you can send options to the constructor if you want to, otherwise default values are used

	c.addTo(map);

	map.on('click', function(e) {
		c.setCoordinates(e);
	});