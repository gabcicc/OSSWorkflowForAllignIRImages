# OSSWorkflowForAllignIRImages
An open source software workflow to align the thermal photos shotted by UAV.

The steps illustrate the design and development of the UAV-based OSS workflow:

Step 1:
Write the function to convert in grayscale and resize the Infrared images (from 640x480 to 3840x2880);
Write the function to crop the RGB images (from 4056x3040 to 3840x2880.


Step 2:
Merge the IR and RGB images in 4-band TIFF image.

Step 3:
The OSS Open Drone Map (ODM) has been used for the photogrammetry and stitching algorithms to elaborate the point cloud and then the orthophoto.


Step 4:
Extract the IR band from the orthophoto. Quantum GIS or Multispec have been used to achieve this aim.

