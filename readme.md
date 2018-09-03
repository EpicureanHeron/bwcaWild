# 9/3/2018

## Currently working on 

* Improving the embedded iframe maps' layers functionality

* Expectations
    * Zooming in and out on a map causes the amount of icons rendered to dynamically adjust
    * As a user scrolls in, more detail is displayed in terms of icons rendered
    * Scrolling out causes fewer icons to be displayed 
    

## Working Examples

Looking at Gillis Lake as an example of how everything currently functions

* http://bwcawild.com/BWCA-Lakes/Gunflint-District/Gillis-Lake/Gillis-Lake.html

This has am embedded iFrame to the topographical map: 

* http://bwcawild.com/BWCA-Lakes/Gunflint-District/Gillis-Lake/Gillis-Lake-Topo-Map.html


Competitor website already has it implemented

* [Paddle Planner](http://www.paddleplanner.com/)

Navigating into the Chrome Dev Tools and selecting the "sources" tab exposes the public facing web files.

Drilling down into paddleplanner.com > js > leaflet > leafletcontrolloading is where I believe their implementation of Layers is, as the file there has 36 mentions of the term "layers"

However, this could exist elsewhere or interact with combo of other files.

## Leaflet

[Leaflet](https://leafletjs.com/) is the javascript library being used to power the maps on this website.

The feature which needs to be implemented is called "layers" 
* [documentation here](https://leafletjs.com/reference-1.3.2.html#layer)


