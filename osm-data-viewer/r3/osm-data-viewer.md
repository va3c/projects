[vA3C Projects]( ../../index.html ) &raquo;
[vA3C<br>OSM Data Viewer R3]( osm-data-viewer-hackette.html "Hi, Dan!" )
===
<span id=msg1 ></span>
## Options (open)

Sample files:
<select id=selFile onchange=loadFile(); >
	<option>Hotel Large STD2010 San Francisco</option>
	<option>Hotel Large STD2013 San Francisco</option>
	<option>medium office</option>
	<option>secondary school</option>
	<option>small hotel doe</option>
	<option selected>small office</option>
	<option>small office pre 1980</option>
</select>

Open a file on you computer:
<input type=file id=inpFile onchange=ifr.contentWindow.readFile(); /> 

<button onclick=ifr.contentWindow.saveFile(); >Save Model to JSON File</button>

Opacity:<input type=range id=inpOpacity min=0.05 max=1.0 step=0.05 value=0.85 onmousemove=updateOpacity(); /><small id=opac >0.85</small>  
Camera near:<input type=range id=inpCameraNear min=1 max=100 step=1 value=1.0 onmousemove=updateCameraCutOff(); /><small id=near >1</small>


## OSM Source
The text area below contains the full contents of the selected OSM file.
<textarea id=txtArea1 style=font-size:9pt;height:200px;width:100%; ></textarea>

## Three.js Interpreted Data
The text area below contains the parameters that have been read from the OSM file and used to create the model as shown here.
<textarea id=txtArea2 style=font-size:9pt;height:200px;width:100%; ></textarea>

## About
OpenStudio is a cross-platform collection of software tools to support whole building energy modeling using EnergyPlus and advanced daylight analysis using Radiance. 
<https://www.openstudio.net/>

This vA3C script reads [Open Studio]( https://github.com/NREL/OpenStudio ) [OSM files]( https://github.com/NREL/OpenStudio-Prototype-Buildings/ ) and displays their contents in 3D.

Thank you [Dan Macumber]( http://www.nrel.gov/buildings/commercial_staff.html#macumber ) of [NREL]( http://www.nrel.gov/ ) for bringing the awesomeness of OSM to light.

[Source Code on GitHub]( https://github.com/va3c/projects/tree/gh-pages/osm-data-viewer )  
[Read Me]( #../readme.md# )

### Copyright and License
Copyright &copy; 2015 vA3C authors  
All work herein is under the [MIT License]( http://opensource.org/licenses/MIT )



