OSM Data Viewer Read Me
===

[OSM Data Viewer latest]( http://va3c.github.io/projects/osm-data-viewer/latest/ )  
<a href=https://github.com/va3c/projects/tree/gh-pages/osm-data-viewer >OSM Data Viewer source code</a>

## Concept

### Mission
Read and display in 3D the data contained in Open Studio OSM files

### Vision
Make the data contained in OSM files available to a larger audience in a greater variety of ways

* Including on tablets and phones

## Current Status

The code currently just reads surface data. Hopefully, each new release will add further parameters.

There is no intermediate format. 
The script reads the vertices in the OSM file and directly creates meshes and assigns data to the mesh's userData area.

The script uses three files:

* osm-data-viewer.html
	* A typical Three.js file
	* Adds the ability to open and read OSM files and create Three.js geometry
	* Works as a standalone or within an iframe
* osm-data-viewer-hackette.html
	* Creates the user-interface
	* loads osm-data-viewer.html in an iframe
* osm-data-viewer.md
	* Source code for user interface in Markdown format
	* Used by osm-data-viewer-hackette.html

You will also note that there is no standard HTML area and no style sheets.
It's 100% JavaScript (and Markdown).

Yes, this is a very idiosyncratic way of writing code. On the other hand, the important bits are all in the main Three.js files.
The user interface files are quite separate and may easily be replace by jQuery files or whatever.

The idea, or the hope anyway, is to write code that's easy to read - code that you can use to write scripts in your style.


## Issues /Bugs

* Subsurface edges helpers not coplanar with subsurface
* Code currently has many items commented out / needs a clean-up
* Setting/'hamburger' button do not initiate menu slide on Android 
* Selected surfaces do not de-highlight properly
* IE: surfaces do not have assigned colors

### Road Map

* Add first person camera
* Add exploded view 
* Add terrain viewer
* Add real-time updates: changes to OSM can be viewed in real-time

### Change Log

2015-03-05 ~ Theo

* Add version and space parameters
* Add the beginning of a translate on axis feature so that subsurfaces sit just a bit proud of the underlying surface
	* Face normals helpers were added
	* Helpers show that normals seem to consistently face the outside of the model

* Views are beginning to look quite bizarre with all the helpers
* Will clean up eventually, but makes things fun to look at for now


2015-03-02 ~ Theo

* Opacity and camera cut-off update while you move slider ( onmousemove instead of onchange ). This can cause issues. Please monitor.
* Adds save model to JSON 4 capability. 
	* Note: Open File button currently only reads OSM files. Open JSON files TBD!
	* In meantime, see [vA3C Cookbook]( https://github.com/va3c/viewer/tree/gh-pages/cookbook ) or [Three.js Editor]( http://mrdoob.github.io/three.js/editor/ ) < remember to add lights
* Partial fix to Outside Boundary Condition
* Add read OS Site parameters
* Started adding sub surfaces

2015-03-01 ~ Theo

* R2
