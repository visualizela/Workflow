---
sectionid: QGIS
sectionclass: h1
is-parent: yes
title: QGIS
number: 5000
---

The process of adapting these files for QGIS in order to georeference them is the longest step within this entire project.
First you are going to want to download every single PDF file that you just documented and place it into a folder created on the desktop.
In this folder you are also going to create individual folders for each file and their outputs. Don’t put anything in them yet as that will make accessing the files in QGIS slightly more time consuming. These folders will carry the output rasters from QGIS and separate them into specific areas. Name them after the ID number e.g. 00032
Moving back to the files they  are going to be switched from .pdf files into .tiff files to do this you will need to open up the application automator, which should be available on a Mac computer.
Once opened find and drag “Get Specified Finder Items,” “Render PDF Pages as Images,” and “Copy Finder Items” into the main area.
Your interface should look like this (make sure that you change the resolution to 600 dots per inch to resemble the digitized file):
![](img/Automater.png)

In the “Get Specified Finder Items” box, add the files you wish to convert and press run.
The files should show up in the Desktop as converted .tiff files.
After this is done you are going to crop the files so that the white space of the maps is limited, you can do this easily in preview with the crop button but for some of the more oddly shaped maps it is best to manually eliminate the white space in a photo editing application such as in photoshop. 
Keep in mind, if you crop the photos before you convert them the cropping won’t be transferred, so it is better to do it after.
From there you are going to open up QGIS and open up a standard OSM map.
To do this go to the task bar on the top of the computer where it says web click on it, scroll down to QuickMapServices, scroll to OSM, and open OSM Standard like so:
**Picture here**

This should present a map of the world upon the main user interface which will be used as our base for georeferencing.
For this purpose you should zoom in on the area that is being georeferenced (in this case Los Angeles).
From here you will go back to the taskbar and click on Raster and then click on Georeferencer like so:
**Picture here**

This will open up a new window where you will be uploading your .tiff files and creating points that will connect them to the OSM map on the original page.
Within this window you are going to click the open raster button on the top left which is a button that looks like a blue and black checkerboard with a small green square with a white plus in it on the bottom right.
**Picture here**

From there you are going to open up a .tiff file into this window.
Before you begin to georeference click on the yellow gear in the window, it will say “transformation settings” and open a new window like so:
**Picture here**

Leave everything as is except change the Output raster name so instead of it ending with _modified, have it end with _geo. Save this output to the correct folder on the desktop e.g. save planning_00032 to the folder 000032
Click OK
At this point you will begin georeferencing which uses three buttons on the top of the window.
**Picture here**

The Add Point button on the left adds points, the Delete Point button in the middle deletes points, and the Move GCP point button moves the points.
From here, using the map you are going to connect points from one window to the other. In the case of Los Angeles, the easiest points to find were street intersections. To do this you will click on a point from the .tiff map which will open a new window labeled Enter Map Coordinates like so:
**Picture here**

From there click on the “From Map Canvas” button. This will bring you to the OSM map.
Once there you will locate the same point on the street as you clicked on for the .tiff file.
This will bring you back to the Enter Map Coordinates window with the X/East and Y/North areas filled in.
Click OK and the point will be placed on both maps.
Do this until you have at least six points placed on the map as that is the lowest amount allowed for QGIS. For this project the numbers ranged but the more points you put on the map the more accurate the georeference is going to be.
Once you have put enough points on the map click the green Start Georeferencing button. This will transform your map and project it onto the OSM form.
If the map looks distorted, go back to the Georeferencer tool and add more points in areas that didn’t have them previously. If it continues to look distorted after multiple back and forths then edit the map outside of the program to remove more white space.
Save the GCP points to the file that is named after the ID.
Repeat this process until all of the maps have been georeferenced, it should look similar to the large pullout map that is included at the back of most binders.
