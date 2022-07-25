# Land Cover Change Detection using Multispectral Satellite Images


## Prerequisites

1. Python3
2. QGIS

## Getting Started

### Installation
 - Clone this repo:

    git clone https://github.com/gallayagnesh/landcover_change_detection_using_multispectral_satellite_images
 - Install Python Depedencies
     - For pip users, please type the command 	```pip install -r requirements.txt```
 - Install QGIS Application from https://www.qgis.org/en/site/forusers/download.html and also install Semi-Classification Plugin(SCP) in QGIS.
 
 ### Data Collection
  - Download Landsat-8 Collection-1 Level-1 Bands images, MTL and XML files from USGS Website of two different timelines.
  
### Image Preprocessing
  - Add band images of one timeline in the Layers and crop the selected area in *Crop Raster* which is available in SCP dropdown.
  - Apply reflectance to the band images and make sure that you select the landsat-8 collection in the reflectance tab.
  - Download the required band composition by adjusting the bands combination.
  - Classify the stacked image by giving the Region of Interests(ROI) polygons as training inputs and download the classified image.
  - Repeat the same process for the other timeline image.
  for more info, [watch this video](https://www.youtube.com/watch?v=HKNS-wsc7lo) 
  
### Change Detection
 Given Python notebook file takes two image files as inputs. Run the blocks of code accordingly to see the reults. After the generating the erode image, shape that image for the evalution.
