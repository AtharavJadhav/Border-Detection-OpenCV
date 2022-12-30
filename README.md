# Border-Detection-OpenCV
To develop a basic OpenCV Python script that draws an object’s outline using Rembg library &amp; OpenCV Image processing


## Detection of Preffered Zone and cropping it
OpenCV was used for selection of ROI i.e. Region of Interest. The imporant thing to note is, ROI selects the tupple based on (x1, y1, width, height) of the image, where x1 and y1 are the coordinates of the points which start the process of selection with mouse.

## Selecting only external contours (Borders)
This step was especially hard as it took most of the time removing the internal borders too, and the simple EXTRENAL function of CV library doesnt function well in this case. The image NEEDS to be stored in JPEG format and then converted to PNG as the contours only be accessed and saved in JPEG format, whereas PNG format is required for the transparent background of the cropped image (JPEG gives a black background).

## Displaying the cut portion at the exact same location
This step required the data of the images to be stored in a XLSX file so that we could access it later on.

