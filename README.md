This map can be viewed <a href="https://geojoek.github.io/PVMA_Map_Lake_Hitchcock/">here</a> on Github Pages or in its final form at <a href="https://www.dinotracksdiscovery.org/map/detail/">dinotrackdiscovery.org</a>. The latter site was produced in conjunction with the great folks at <a href="http://www.digitalgizmo.com">Digital Gizmo</a>.

This is a "map" (model, really) of several snapshots of the retreat of glacial ice in the Connecticut Valley, CT & MA, USA, and the fluctuating levels of Glacial Lake Hitchcock as an ice-marginal and sediment dammed glacial lake.

Each layer shows the extent of glacial ice in light grey / white and Glacial Lake Hitchcock in blue. The southern margin of glacial ice extent is <em>*extremely*</em> inferred and should not be considered accurate— This is due to there being precious little published geologic data to draw from, nor high-resolution map sources for ice-margin boundaries in Massachusetts.  The extent of the glacial lake is also inferred-- see below for more discussion on that matter.

<em>NOTE:</em> Only Glacial Lake Hitchcock is shown on this map. There were numerous other glacial lakes across southern New-England that co-existed with Glacial Lake Hitchcock, but they are not shown as they were beyond the scope of this project— perhaps another project!

This is also a very, very simple and inefficiant implementation of <a href = "http://leafletjs.com">Leaflet.js</a> to display geological map layers.

Right now, I am pre-loading the GeoJSON layers as scripts in the html-- this is horrendously inefficiant and leads to a very long page-load.

There are better ways to do this, namely, using <a href="https://mapzen.com/products/tangram/">Tangram.js</a> by MapZen, which automatically tiles vector GeoJSON layers/objects.  I was unable to succesfully implement it this time around due to needing to do more research on the GeoJSON format and how Tangram.js's .yaml format interacts with GeoJSON... I suspect the GeoJSON files I was producing weren't structured properly for it to work.

Data Sources:

Glacial Ice: 

 - <a href="https://pubs.usgs.gov/sim/2005/2784/">Quaternary Geologic Map of Connecticut</a> for ice margin positions in Connecticut
 - Ridge, et al., 2012, <a href="http://www.ajsonline.org/content/312/7/685.abstract">The new North American Varve Chronology...</a> American Journal of Science Vol 312, P 685-722
 - Ridge, J.C., 2003, The last deglaciation of the northeastern United States: A combined varve, paleomagnetic, and calibrated C <sup>14</sup> chronology: Chapter 3 in </em>Geoarchaeology of Landscapes in the Glaciated Northeast</em>, New York State Museum Bulletin 497.
 
Extent of Glacial Lake Hitchcock:
  - <a href="https://pubs.usgs.gov/sim/2005/2784/">Quaternary Geologic Map of Connecticut</a> for Connecticut
  - Correcting a USGS National Elevation Dataset DEM for isostatic rebound, determined from contours published in the <a href="http://www2.newpaltz.edu/fop/pdf/FOP2015Guide.pdf">2015 Friends of the Pleistocene Guidbook (Stone et al.)</a> and "filling" the Connecticut Valley to Glacial Lake levels as described in that article and referenced therein.  I could go into more detail.
  
These maps should be considered informed conceptual models, more than anything else, for public outreach and educational purposes due to the vagaries of GIS and geologic interpretation. These *are not* accurate maps of the extent of glacial ice or glacial lakes in Southern New England-- please see the USGS's great surficial geologic maps for that.

The ice sheet was cropped to a rectangle as it's the bounds of the project.  It covered the whole continent and had various lobes extending southward.

What the layers show:
<ul>
<li><em>15,600 years ago: </em> By this point the dam at Rocky Hill was breached due to the earth's crust, and local topography beginning to rebound and rise from being released from the weight of several kilometers of ice.  This caused the lake level to suddenly drop by about 5-6m and become unstable for the remainder of the history of the Lake as it began to drain. By this point large areas of former lake bottom were above water and exposed to air.  The Lake level is shown post-drop, so the Montague and Long Plain (Sunderland) deltas are shown to be above water in this view when they were underwater for a period of time while being deposited.</li>
<li><em>17,200 years ago:</em> This is in the middle of what geologist's called the "stable phase" of Glacial Lake Hitchcock, when lake levels were stable for several 100 to almost 1000 years.</li>
<li><em>17,900 years ago:</em> This is during the high-stand of Glacial Lake Hitchcock, what geologists call the "Connecticut Phase"</li>
<li><em>19,500 years ago:</em> Before Glacial Lake Hitchcock, after the ice sheet was at its full extent.  There was a small glacial lake off of the end of the ice sheet unrelated to Lake Hitchcock that is not shown here, as not to confuse folks. </li>
