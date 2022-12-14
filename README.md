Dataset used in this work is from USGS Landsat-8 satellite. See the source here https://earthexplorer.usgs.gov/

<!-- <img align="right" width="200" height="100" src="https://raw.githubusercontent.com/cengizhunter/Change-Detection/main/logo/ITUlogo.png"> -->

# Change-Detection

This code calculates difference from NDTI images. It can be used for change detection on the images with different dates.
It can be easily modified for other indices.

## Libraries that are used in jupyter notebook on python 3.8.5

Using a conda enviroment with jupyternotebook for this code could be helpful.

- rasterio 1.3.2
- numpy 1.23.3
- matplotlib 3.4.3
- gdal 3.4.3
- scipy 1.9.1

## Input Bands for landsat8

- Band6 (SWIR1)
- Band7 (SWIR2)

## Output Images

- NDTI Images
- NDTI difference
- NDTI threshold Image
- NDTI threshold removed noise Image

2019 RGB Image Kocaeli             |  2014 RGB Image Kocaeli
:-------------------------:|:-------------------------:
![](https://github.com/cengizhunter/Change-Detection/blob/main/images/2019_RGBI.jpg)  |  ![](https://github.com/cengizhunter/Change-Detection/blob/main/images/2014_RGBI.jpg)


2019 NDTI Image Kocaeli             |  2014 NDTI Image Kocaeli
:-------------------------:|:-------------------------:
![Solarized dark](https://github.com/cengizhunter/Change-Detection/blob/main/images/2019_NDTI.jpg)  |  ![](https://github.com/cengizhunter/Change-Detection/blob/main/images/2014_NDTI.jpg)

NDTI difference Threshold square image             |  After 3x3 Mode Filter
:-------------------------:|:-------------------------:
![Solarized dark](https://github.com/cengizhunter/Change-Detection/blob/main/Output/threshold_square_ndtidif.png)  |  ![](https://github.com/cengizhunter/Change-Detection/blob/main/Output/mode_threshold_square_ndtidif.png)


 ## References
- [Separating Built-Up Areas article (Osgouei et al. 2018)]
- [Change Detection between NDVI Images by Thales Sehn Körting]
- [NDVI Index calculation by Hatari Labs]
 
[Change Detection between NDVI Images by Thales Sehn Körting]: https://github.com/tkorting/youtube/tree/master/basic-change-detection-in-rs
[NDVI Index calculation by Hatari Labs]: https://www.hatarilabs.com/ih-en/ndvi-calculation-from-landsat8-images-with-python-3-and-rasterio-tutorial
[Separating Built-Up Areas article (Osgouei et al. 2018)]: https://www.mdpi.com/2072-4292/11/3/345

