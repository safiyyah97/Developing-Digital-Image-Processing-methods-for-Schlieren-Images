# Developing-Digital-Image-Processing-methods-for-Schlieren-Images: Quantification of internal and interfacial convection
Authors: Safiyyah Moos

This repository contains algorithms used analyse the contribution of fingers (interfacial convection) and streamers (internal convection) to the desaliantion of sea ice in a quasi-2D Hele-Shaw cell.  

## Necessary libraries:

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the necessary libraries, such as cv2, fnmatch, PIL, pandas, time, os, csv, numpy, matplotlib.pyplot, datetime

## Brief description
This collection of scripts that is used to analyse the raw Schlieren images obtained from a quasi-2D Hele-Shaw cell using DIP methods. The main image processing techniques in this algorithm involves pre-processing via image division and segmentation via edge detection methods and conncected component labelling/region detection to refine the combining and segmenting of objects within the image. 

## Workflow 
The workflow is divided into the streamer/finger analysis, ice interface analysis and tracking of individual streamers/fingers. The scripts are written in a notebook with each section performing a different operation, which is outlined below. The oeprations must be performed sequentially. 

### Streamer, finger and interface isolation 
1. Converting raw Schlieren image to segmented image.
2. Isolating the ice-water interface.
3. Tracking the ice-water interface and determining ice thickness. 
4. Applying connected component labelling to track expulsions and determine characteristics. 
5. Adding the scale bar and timestamp.
6. Converting the images to a video file. 

### Streamer tracking 
1. Crop a single streamer from segmented image.
2. Ensure image is binary.
3. Detect regions within image.
4. Match the regions based on characteristics (centroids).
5. Track the matched regions.

## Data sources 
- The raw Schlieren images for experiments 1, 2 and 3 can be found at ****. 
- The segmented images for experiments 1, 2 and 3 can be found at ***.
- The isolated ice-water interface can be found at ***.
- The final segmented image can be found at ***. 
