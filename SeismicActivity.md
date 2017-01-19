# Seismic activity in Italy
Albert Blanchart  
January 19, 2017  



## The News of the week

During this week Italy has been striken by a series of earthquakes which have spread around the areas of Perugia, Viso and Rome. CNN has a dedicated video about this in its [webpage](http://edition.cnn.com/2016/10/31/europe/italy-earthquake-norcia-explainer/). So in this short markdown document we will be ploting the region of Italy and pointing out just a few of the earthquakes that took place on thursday the 19th nof Januari. Actually there has been registered up to 186 earthquakes in the regions of L'Aquila, Rieti, Perugia and Rome. More detailed information can be obtained in the [Volcano Discovery Webpage](https://www.volcanodiscovery.com/earthquakes/italy.html) where all seisms are registrered lived!

## The necessary packages to perform a nice plot
Well as you all know this peer-graded assignment is all about Leaflet (Since R Markdown has been covered in opther courses and just a few more details were revealed in this session). We all love leaflet, it does awesome things with the maps, so lets going to load in R:

```r
library(leaflet)
library(dplyr)
```
And now we will start building our map:
<!--html_preserve--><div id="htmlwidget-ea182ce3ef63c800f241" style="width:672px;height:480px;" class="leaflet html-widget"></div>
<script type="application/json" data-for="htmlwidget-ea182ce3ef63c800f241">{"x":{"calls":[{"method":"addTiles","args":["http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",null,null,{"minZoom":0,"maxZoom":18,"maxNativeZoom":null,"tileSize":256,"subdomains":"abc","errorTileUrl":"","tms":false,"continuousWorld":false,"noWrap":false,"zoomOffset":0,"zoomReverse":false,"opacity":1,"zIndex":null,"unloadInvisibleTiles":null,"updateWhenIdle":null,"detectRetina":false,"reuseTiles":false,"attribution":"&copy; <a href=\"http://openstreetmap.org\">OpenStreetMap\u003c/a> contributors, <a href=\"http://creativecommons.org/licenses/by-sa/2.0/\">CC-BY-SA\u003c/a>"}]},{"method":"addMarkers","args":[[42.5252,42.5685,42.5793,42.59,42.5793,42.8337,43.0252,42.9017],[13.3118,13.2728,13.3018,13.3,13.2893,12.9652,13.0358,13.1917],null,null,null,{"clickable":true,"draggable":false,"keyboard":true,"title":"","alt":"","zIndexOffset":0,"opacity":1,"riseOnHover":false,"riseOffset":250},["magnitude: 2","magnitude: 2.1","magnitude: 2","magnitude: 3.4","magnitude: 2.5","magnitude: 2.2","magnitude: 2.8","magnitude: 2.8"],null,null]},{"method":"addCircles","args":[[42.5252,42.5685,42.5793,42.59,42.5793,42.8337,43.0252,42.9017],[13.3118,13.2728,13.3018,13.3,13.2893,12.9652,13.0358,13.1917],[4760,6320,5320,4000,4120,4680,3400,3880],null,null,{"lineCap":null,"lineJoin":null,"clickable":true,"pointerEvents":null,"className":"","stroke":true,"color":["red","red","blue","green","blue","orange","purple","orange"],"weight":5,"opacity":0.5,"fill":true,"fillColor":["red","red","blue","green","blue","orange","purple","orange"],"fillOpacity":0.2,"dashArray":null},null]},{"method":"addLegend","args":[{"colors":["red","blue","green","orange","purple"],"labels":["L`Aquila","Rieti","Rome","Macerata","Perugia"],"na_color":null,"na_label":"NA","opacity":0.5,"position":"topright","type":"unknown","title":null,"extra":null,"layerId":null,"className":"info legend"}]}],"limits":{"lat":[42.5252,43.0252],"lng":[12.9652,13.3118]}},"evals":[],"jsHooks":[]}</script><!--/html_preserve-->

So the different regions have been colored and the popups show the magnitude of the seisms, moreover the radius of each circle shows the Depth. Note that in order to visualize the radius I just multiply the original value by 400 so all the circles are visibles in the whole region, *values of 10 Km are not visible in such a broad area :>*.

For those interested in see the code you can find the .Rmd, .md and htlm files in my git repository:

[(https://github.com/Changomazo/Seismic-activity)]
