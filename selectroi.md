Select ROI
---
 >This script is designed to help the user select a region of interest
	to use with the set of images selected by the user. The boundaries
	can be set either by clicking and dragging, or with the text entry
	boxes. When this script is run, it will look for a config file called
	ROI_config.txt that specifies the region of interest. If no such file
	exists, it will be created when the user presses 'Save'. Saving will
	overwrite any previous information in ROI_config.txt.
	ROI_config.txt will be used by other scripts, such as image_diversity.py,
	Autotrace.py, and TrainNetwork.py.

+ Open __Select ROI__
+ To do this open the __terminal__
+ Open a new tab within the __terminal__
+ Change to the Autotrace directory (ex.`cd /path/to/Autotrace/old`)

+ Start [SelectROI.py](../SelectROI.py) by typing `python SelectROI.py`
+ The terminal will open followed by an __Open Image Files__ screen.
![Image1SR](images/Image1SR.png)
+ Select the images by boxing them or shift-clicking to make sure that they are all highlighted and click __open__
+ Once the window is open, box the area you are interested in investigating, select the machine you are using, and click __save__.
+ Then select a location to put the ROI_config.txt and click __save__.
+ When finished, click __Exit Program__
