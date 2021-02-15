# OSSWorkflowForAllignIRImages

The tests carried out showed how the alignment phase of the images shotted by UAV is influenced by the different lighting conditions, depending to the different flight times. None of the commercial photogrammetry software is capable of aligning images taken before sunrise or after sunset. 
These workflows made it possible to merge RGB and IR images into 4-channel TIFF images, allowing the photogrammetry software to construct an orthophoto from which thermal information can be extracted.

The steps illustrate the design and development of the UAV-based OSS workflow:

Step 1: The GNU-Octave software has been used for steps 1 and 2.

Write the function to convert in grayscale and resize the Infrared images (from 640x480 to 3840x2880);
Write the function to crop the RGB images (from 4056x3040 to 3840x2880.

Step 2:
Merge the IR and RGB images in 4-band TIFF image.

Step 3:
The OSS Open Drone Map (ODM) has been used for the photogrammetry and stitching algorithms to elaborate the point cloud and then the orthophoto.


Step 4:
Extract the IR band from the orthophoto. Quantum GIS or Multispec have been used to achieve this aim.

The next phase would be to test different open source photogrammetry solutions to improve processing time and develop a stand-alone open source application (e.g., Python QGis plugin) that includes all phases of the work.


