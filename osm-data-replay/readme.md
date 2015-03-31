Open Studio Data Display Read Me
===

[Open Studio Data Display latest]( http://va3c.github.io/projects/osm-data-replay/latest/ )
[Open Studio Data Display source code]( https://github.com/va3c/projects/tree/gh-pages/osm-data-replay )

R2 adds three new things

1. Edges helpers are added. This helps with visualizing the different walls. A future release will add the ability to toggle the display of edges helpers

2. Material opacity is added. A slider allows you to update the opacity of materials for the entire building.  A readout is provided to see the current setting. Again this is just one of many tools that may be used - in conjunction with others - to add insight as  what is happening in and around a structure

3. A Camera Near feature is added - controlled by a slider and feedback provided by a readout. This is very much of a trick feature - a handy one-liner. Nevertheless there are situations where adjusting the camera cut-off parameters may be highly beneficial

Camera Near: general usage: in this demo, slide the pointer to about a value of 45 then using the pointing device twirl the building. Notice that whatever part of the structure is directly facing the camera is truncated and you are able to see what is inside.

Generally
The code could use a big clean up. It will eventually get to be shorter, tighter simpler.

A lot depends on the ways we agree for reading Open Studio data.

Future
Add more camera controls to enable building fly-throughs

Enable Boolean operations so as to cut fixed sections through structures.

### Road Map

* Add Orbit/first person camera toggle
* Add show edges checkbox
* Add file open capability


### Change Log

2015-02-25 ~ Theo

* Add R2
* Adds Opacity update, slider and readout
* Adds Camera near update, slider and readout
* Adds edges helpers

2015-02-20 ~ Theo

* First commit R1