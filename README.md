# Geog458-MapTiles

This project contains four raster tilesets for efficiently rendering web maps. Tilesets are displayed as toggleable layers on the [web map](https://maxjayne-1860279.github.io/Geog458-MapTiles/). Each tileset is centered on Seattle, Washington and contains zoom levels from 0-14, allowing the map layers to acccurately and efficiently render the area surrounding Seattle, though accuracy drops off near the state borders.

![A plain basemap](/imgs/layer1.png)

This first layer is a simple basemap for displaying basic geographic context. It can be overlaid with a thematic layer to illustrate data over it's given geo context. This map was developed using MapBox's Monochrome basemap, with minor color adjustments to a more paper-esque feel, and minor changes to text lables.

![A map layer displaying Seattle affordable housing zones](/imgs/layer2.png)

This thematic layer displays affordable housing zones in Seattle (known as MHA zones) in which constructed multi-unit apartments must lease out a certain percentage of total units at affordable housing prices, or opt to instead pay a fee to the citys affordable housing program. This layer uses data sourced from Seattle City GIS, hosted by ArcGIS.

![A combined layer of basemap and housing zones](/imgs/layer3.png)

This layer combines the two previous layers, taking the basemap from the first, and overlaying the Seattle affordable housing zone thematic layer on top. This basemap allows for geographic context to be applied to the thematic layer (Note: the affordable housing layer by itself is also rendered over a basemap).

![A custom basemap for roadway analysis](/imgs/layer4.png)

The final layer is a custom basemap also developed from MapBox's Monochrome basemap. This basemap is designed for roadway analysis and as such uses a dark palette for land and water features. Streets on the other hand are highlighted in purple so as to be easily seen. Road labels are adjusted to appear brighter than other labels for further ease of analysis.

## Credits

Each tileset was created using QGIS and QMetaTiles. Data for the thematic layer sourced from Seattle City GIS hosted by ArcGIS. Basemaps created and web hosted via MapBox-gl. Lab developed by Bo Zhao.