This is a "map" (model, really) of several snapshots of the retreat of glacial ice in the Connecticut Valley, CT & MA, USA, and the fluctuating levels of Glacial Lake Hitchcock as an ice-marginal and sediment dammed glacial lake.

Each layer shows the extent of glacial ice in light grey / white and Glacial Lake Hitchcock in blue. The glacial ice extent is <em>*extremely*</em> inferred due to there being precious little published geologic data to draw from, nor high-resolution map sources for ice-margin boundaries in Massachusetts.  The extent of the glacial lake is also inferred-- see below for more discussion on that matter.

This is also a very, very simple and inefficiant implementation of <a href = "http://leafletjs.com">Leaflet.js</a> to display geological map layers.

Right now, I am pre-loading the GeoJSON layers as scripts in the html-- this is horrendously inefficiant and leads to a very long page-load.

There are better ways to do this, namely, using <a href="https://mapzen.com/products/tangram/">Tangram.js</a> by MapZen, which automatically tiles vector GeoJSON layers/objects.  I was unable to succesfully implement it this time around due to needing to do more research on the GeoJSON format and how Tangram.js's .yaml format interacts with GeoJSON... I suspect the GeoJSON files I was producing weren't structured properly for it to work.

Data Sources:

Glacial Ice: 

 - <a href="https://pubs.usgs.gov/sim/2005/2784/">Quaternary Geologic Map of Connecticut</a> for ice margin positions in Connecticut
 - Ridge, et al., 2012, <a href="http://www.ajsonline.org/content/312/7/685.abstract">The new North American Varve Chronology...</a> American Journal of Science Vol 312, P 685-722
 
Extent of Glacial Lake Hitchcock:
  - <a href="https://pubs.usgs.gov/sim/2005/2784/">Quaternary Geologic Map of Connecticut</a> for Connecticut
  - Correcting a USGS National Elevation Dataset DEM for isostatic rebound, determined from contours published in the <a href="http://www2.newpaltz.edu/fop/pdf/FOP2015Guide.pdf">2015 Friends of the Pleistocene Guidbook (Stone et al.)</a> and "filling" the Connecticut Valley to Glacial Lake levels as described in that article.  I could go into more detail.
  
These maps should be considered informed conceptual models more than anything else for public outreach due to the vagaries of GIS and geologic interpretation, and not accurate maps of the extent-- see the USGS's great surficial geologic maps for that.
