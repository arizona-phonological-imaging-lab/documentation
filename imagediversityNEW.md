Image Diversity New Manual
===

>This script measures the distance from average for each image in the
	input set, and copies the specified number of highest scoring images
	to a new folder called 'diverse'. If ROI_config.txt is present in the
	same folder as the input images, the ROI in that file will be used to
	do the measurement. If not present, it will use a hard-coded default ROI.

+ Open [Image Diversity](../image_diversityNEW.py) by typing `python image_diversityNEW.py`

![Image Diversity](images/image_diversityNEW.png)

+ Click _open_ by the Select Files field
 >Note: this program filters so that only images can be selected, and once you click _open_ it may take a while.
+ It will then ask for corresponding traces to match the images
+ Hit _open_ once you have selected the corresponding traces
+ The main screen tells the number of images selected
+ Specify the number for training and testing
 >_training_ is the first time it runs through, and then the number you _test_ comes from the _training_ batch
+ specify the numer of _most diverse_ and _least diverse_
 > _most diverse_ will select images that vary greatly in their tongue contours, while _least diverse_ will select images that all have similar tongue contours

 + That will reduce the numbr of overall images based on your specifications
+ Select the ratio of _most diverse_ to _least diverse_
+ From this you can select a __test set__. It is recommended that you use a sample from your most diverse images for testing.
+ __batches for remaining__ is simply all of the images that you have not selected to train with, and they will go into a folderentitled __remaining__
 > Note: if an __error__ during this part of the process occurs then some settings may be missing
+ Save to your folder of choice
+ Click __OK__
+ From this a graph will open

![Image Diversity Graph](images/image_diversityNEWgraph.png)
 > This shows __Diversity Scores__ on the Y axis. Diversity scores will be higher if you have more diverse images and vice versa for least diverse. On the X axis it simply ranks the numbers based on their order.

 + You can save this graph if you would like or take a screenshot
>The program will close automatically when it is done running (T: may not be correct, program has not closed automatically for me yet)
+ Open the folder where you specified to have the images
 > Note: In this folder there will be several other new folders. __batch remaining__ is the folder discussed above. __diversity log__ is the record of what happened in the file move. __sorted results__ are the scores for each image.
