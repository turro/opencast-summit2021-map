# Opencast Summit 2021 – Map

This is the repository for [ocsummit2021.map.opencast.org](https://ocsummit2021.map.opencast.org).
The map shows locations of some Opencast summit 2021 attendees.

## Add yourself to the map

If you would like to appear on the map, just create a [pull request](https://github.com/opencast/opencast-summit2021-map/pulls) in which you add your data to the file [adopters.geojson](adopters.geojson).
To do so, add this object with your data as a new line `features`-list in said file:

```json
{"type": "Feature", "properties": {"institution": "YOUR_INSTITUTION"}, "geometry": {"type": "Point", "coordinates": [0.0, 0.0]}}
```

Replace `YOUR_INSTITUION` and `[0.0, 0.0]` with your `lon` and `lat` coordinates, respectively, and your good to go.


If you have problems with creating a pull request, you can also open an issue instead and include name and location.
We will pick that up and then add it to the map for you.


### How to get your Coordinates

You can use the tool [nominatim](https://nominatim.openstreetmap.org) to look up an address and get its coordinates.
Alternatively, you can right click on a location in google maps and you will be shown the coordinates in the menu.
Note that in both of these ways, you will have to invert the order of the coordinates (which you will get in `lat/lon`) for this map (where it is `lon/lat`).
