## About
Last Updated *[06/04/2019]*   
Created by [OSU Maps and Spatial Data](https://info.library.okstate.edu/map-room)

![img example](images/OSULogo.png)

## Table of Contents
- Introduction 
- *Georeferencing with ArcPro*
- - Starting a New Project
- - Adding Files
- - Control Points
- - Transforming the Image
- - Saving the Project
- Conclusion
- Further Reading/Resources

## Introduction

Georeferencing is the process of adding geographic information to a raster (or should I just say image?) (i.e. maps, satelite images and aerial photographs) so mapping software can place the image in its real world location. This is done by assigning geographic coordinates to the raster's pixels. 

## *Georeferencing with ArcPro*

#### Starting a New Project

1. To begin a new project, open ArcGIS on your desktop.
2. Click "Map" under "New Blank Templates".
    
![New Project](images/NewProject.PNG)

3. Name your project and choose a location that will be easy to access (fix wording). Then click "OK". A new screen should open. 

#### Adding Files
Now that a new project has been created, a folder connection must be added in order to import data. 
1. To do this, click "Add Folder" under the "Insert" tab of the Toolbar to create a folder connection.

![Folder Connection](images/FolderConnection.PNG)

2. Select the desired folder and click "OK".
3. The folder connection should appear under "Folders" in the Catalog pane. 

![Catalog Connection](images/CatalogConnection.PNG)

4. Locate desired data. Right click the file and click "Add to Current Map". The selected file is now added to the project and should appear in the contents pane. (It is okay if the raster is not displayed on the map as long as the file is visible in the Contents pane.)

![Added File](images/AddedFile.PNG)

Note: For georeferencing, JPGs are the preferred file type. 

#### Georeferencing

Once a file has been added to the project, the georeferencing process can begin. 

1. In order to start georeferencing, you must select the desired file in the contents pane.
2. Click Georeference under the Imagery tab of the Toolbar. A new Georeference tab should appear on the Toolbar. 

![Georeference](images/Georeference.PNG)

3. Click "Fit to Display" under the Georeference tab. If the raster image was not visible before, it should now appear on the map. The size of the image can be adjusted by zooming in or out and clicking "Fit to Display" as needed. (The image does not need to be the exact size of the geographical area it covers. This will be corrected during the georeferencing process.)

![Fit to Display](images/FittoDisplay.PNG)

 ##### Adding Control Points
 Control points are used to align pixels on the raster image with real life coordinates. 
 
 1. To add control points, click "Add Control Points" in the "Adjust" column of the "Georeference" tab.
 
 ![Add Control Points](images/AddControlPoints.PNG)
 
 2. For maps, locate the point of an intersecting latitude and longitude line on the raster image and click. A red box should appear, indicating the selection on the map
 Note: It can be helpful to click intersections of lines divisible by 5. 
 3. Turn off the raster layer by clicking the check box next to its name in the Contents pane. 
 4. Find the corresponding coordinates on the original world map and click. It is best to be as precise as possible to ensure minimal error. 
 5. Once this is done, a control point is added. 
 6. Continue this step until enough control points are added for the desired transformation. The more control points that are added, the more precise the transformation will be. It is also best to have the control points spaced out instead of clumped together to avoid skewing the image. 
 Note: Spline is the preferred transformation for accuracy and requires 10 or more control points, but there are other transformations when fewer control points are possible. 

#### Transforming the Image

#### Saving the Project

## Conclusion

## Further Reading/Resources


[Return to Top](#about)
