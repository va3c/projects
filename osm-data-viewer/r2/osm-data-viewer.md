[vA3C Projects]( ../../index.html ) &raquo;
[vA3C<br>OSM Data Viewer]( osm-data-viewer-hackette.html "Hi, Dan!" )
===

## Options (open)

Sample files:
<select id=selFile onchange=loadFile(); >
	<option>Hotel Large STD2010 San Francisco</option>
	<option>Hotel Large STD2013 San Francisco</option>
	<option>medium office</option>
	<option>secondary school/option>
	<option>small hotel doe</option>
	<option selected>small office</option>
	<option>small office pre 1980</option>
</select>

Open a file on you computer:
<input type=file id=inpFile onchange=ifr.contentWindow.readFile(); /> 

<button onclick=saveFile(); >Save File</button>

Opacity: <input type=range id=inpOpacity min=0.05 max=1.0 step=0.05 value=0.85 onchange=opac.innerHTML=this.value;ifr.contentWindow.findSurfaces(); /> <span id=opac >0.85</span>
Camera near: <input type=range id=inpCameraNear min=1 max=100 step=1 value=1.0 onchange=near.innerHTML=this.value;ifr.contentWindow.camera.near=parseFloat(this.value);ifr.contentWindow.camera.updateProjectionMatrix(); /> <span id=near >1</span>


## OSM Source
The text area below contains the full contents of the selected OSM file.
<textarea id=txtArea1 style=font-size:9pt;height:200px;width:100%; ></textarea>

## Three.js Interpretated Data
The text area below contains the parameters that have been read from the OSM file and used to create the model as shown here.
<textarea id=txtArea2 style=font-size:9pt;height:200px;width:100%; ></textarea>

## About

Thank you Dan Macumber of NREL for bringing the awesomeness of OSM to light

### Copyright and License
copyright &copy; 2015 vA3C authors ~ All work herein is under the [MIT License]()



