fontawesome-markers
===================

An export of the fontawesome glyphs into named SVG Paths in javascript.

All glyphs have the same names as font-awesome, except they are capitalised, and underscored, eg "exclamation-sign" becomes "EXCLAMATION_SIGN"

You can use these paths, in products like Google Maps, for example:

```js
new google.maps.Marker({
    map: map,
    icon: {
        path: fontawesome.markers.EXCLAMATION,
        scale: 0.5,
        strokeWeight: 0.2,
        strokeColor: 'black',
        strokeOpacity: 1,
        fillColor: '#f8ae5f',
        fillOpacity: 0.7,
    },
    clickable: false,
    position: new google.maps.LatLng(lat, lng)
});
```

##Update

7th August 2014 - Updated to fontawesome 4.1.0, see https://github.com/FortAwesome/Font-Awesome/wiki/Upgrading-from-3.2.1-to-4 for the list of changed names.
26th September 2013 - Changed font extraction process - Glyph size is a much more manageable 64px now, and rotation / flip corrected.
