2018 Kīlauea Lower Puna Eruption

![image](https://user-images.githubusercontent.com/77478277/111932791-4856ac80-8a62-11eb-802f-7b09e8739e5b.png)
![image](https://user-images.githubusercontent.com/77478277/111932758-38d76380-8a62-11eb-9896-3a29224ff97c.png)
These two images show how with the time slider you can see the continuity of lava flow. I thought this particular location was interesting because even though there is a hill upslope, the lava was able to encroach upon this area because of the landscape depressions.

https://elana-shi.github.io/elana-shi-web/Lab%202%20Interactive%20Mapping/index.html

<b> Reliance on other resources </b> </br>
Code was modified from MapBox Docs: Create a Time Slider and MapBox Docs: Add 3D Terrain to a Map </br>
https://docs.mapbox.com/mapbox-gl-js/example/timeline-animation/ </br>
https://docs.mapbox.com/mapbox-gl-js/example/add-terrain/ </br>
Instead of mapping points with different radii like in the example, I modified the code to map a series of polygons based on the date. I modified the lava data in QGIS (merging and adding appropriate fields) so that the code could draw data from it. I also asked you (Luke) to help me debug an issue I had with displaying the polygons through the slider filter. I accidentally didn’t save the code you helped me with, so I had to figure it out again by myself although I did remember the direction you pointed me in initially. That was a good way of testing out whether I understood what I was doing… it worked out.
I asked my peers to help critique my color choices, but they generally agreed that the red was an alright choice.

<b> Reflective Analysis </b> </br>
This map visualizes the extent to which lava moved over the lower Puna landscape throughout the 2018 eruptions on Hawaii Island. 
The map highlights not only the destruction to the built habitat, but also how lava flow responds to topography, which is visualized through contours, 
hill shades, and a 3D terrain. The latter is an important factor in residential zoning; if we can predict how lava will flow over a landscape based on 
historical evidence, then we can better evaluate the risks of placing houses in certain areas in the future. If zoomed in enough, you can see a row of 
fissures surrounded by whole neighborhood of houses. I would venture to say that it was poor planning to place people’s homes downhill of an active volcano. 
Those downhill of the fissures that weren’t affected were often also downhill of some obstacle (hill) that helped redirect the lava elsewhere. </br> </br>
The time component is there so help visualize the flow over time. The data only shows newly surveyed lava, as opposed to new extent plus past extent. 
This makes sense because there is a lot of overlap in lava flow that couldn’t be documented otherwise, however it makes it hard for a viewer to understand 
the continuity of certain flows. The slider makes up for this by allowing the viewer to flip between consecutive surveys. 
To improve this map, I would want to have an opaque layer of the previous few polygons to help the user visualize continuity better. </br> </br>
I am quite satisfied with the overall aesthetic of this map, as I felt like the color choices resonated with the theme of volcanos. 
The black landscape is meant to represent lava rock, which the islands are composed of. The orange of the lava polygons is self-explanatory. 
For the houses, I differentiated the houses affected by the lava flow (via a quick intersect selection in QGIS) from those that weren’t impacted. 
I had a bit of trouble with the color scheme, but I decided to make the affected houses a deep red, which is bright enough to stand out from the 
black but dark enough to stand out from the orange. It also helped that the houses were 3D and rose above the flat lava polygon. I made the map have 
a 3D terrain because topography is an important driver of lava movement. By holding the left and right mouse buttons, the user can adjust the pitch and 
bearing to see the hills and divets in the landscape created by previous volcanic activity, and where the houses are situated in relation to these landscape features.

<b> Data Citation </b> </br>
Hawaiian Volcano Observatory staff, 2018, Preliminary map of the 2018 lower East Rift Zone eruption of Kīlauea Volcano, Island of Hawai‘i: U.S. Geological Survey, https://doi.org/10.5066/P994OGY8. </br>
Microsoft, 2020, USBuildingFootprints
