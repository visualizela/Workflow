---
sectionid: Merge
sectionclass: h1
is-parent: yes
title: Merge
number: 6
---
This step is only necessary if the map you have created was composed of a series of individual maps that has been stiched up together such as with this particular map. If you have a single map then you can skip this part.

The purpose of merging files together within this project is so that the areas being documented are easily distinguishable/connected to each other so that when they are clicked on, no matter where they are clicked on, the information from the binders comes through.

At the taskbar go to Raster - Miscellaneous - Merge.
Picture.

In the input layers section click the button with … on it and select all the layers you are trying to merge.
In the merged area click the … button and save the file to the desktop as Geomerge.
Picture

Once this is concluded there will likely be a black border that obscures a significant amount of the map.
Picture

Click on the information icon (the blue circle with an i in it) and click on the black border.
Picture

Take the number from that and go to the raster file Geomerge, open it.
In the transparency page you are going to put the number you found in the No Data Value - Additional no data value area, which will remove the black.
Picture

It will also shift the colors of the map to be brighter to go to the symbology page and mess around with the color rendering. For this map I changed the blending mode, brightness, and contrast. This might be very different depending on the maps that you have. There is also the option to convert the raster from PCT to RGB by going to Raster - Conversion - PCT to RGB… and inputting the correct layer. I didn’t use this method because it kept giving errors to my files but it is apparently a viable method for color correction.
Picture
