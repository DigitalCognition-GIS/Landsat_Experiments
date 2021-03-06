### This file has ROUGH NOTES , steps i followed , errors logs etc .( REFER with a pinch of salt)  


<p align="center">
    <img src="https://github.com/DigitalCognition-GIS/Landsat_Experiments/blob/master/ScreenCaptures/Landsat_8.jpg" width= "850px">
</p>

<h1 align="center">LANDSAT Experiments - </h1>

> This repository will contain both code and additional reading material refrences for analytics and pseudo-projects done with the LANDSAT Data. (LANDSAT -8 Mostly) **- LANDSAT 2020**
 
> If you are a GIS developer or a GeoSpatial Scientist - kindly feel free to contribute. 


<br/>


### Table of Contents of this repository

- [X] `A-- Intro to LANDSAT group of satellites` 
- [X] `B-- Download and Preprocess LANDSAT -7&8 Data` 
- [X] `C-- Further explorations with LANDSAT -7&8 Data` 
- [X] `D-- Global Food Security Support Analysis Data (GFSAD)` 
- [X] `Work in Progress` 
- [X] `Work in Progress` 
- [X] `Work in Progress` 


<br/>

### References - Always an ongoing effort - Work in Progress

### LANDSAT - 8 ( Features and Facts )

- Source URL - https://www.usgs.gov/land-resources/nli/landsat/landsat-8?qt-science_support_page_related_con=0#qt-science_support_page_related_con   


> The Landsat 8 satellite orbits the the Earth in a sun-synchronous, near-polar orbit, at an altitude of 705 km (438 mi), inclined at 98.2 degrees, and circles the Earth every 99 minutes.  The satellite has a 16-day repeat cycle with an equatorial crossing time: 10:00 a.m. +/- 15 minutes.    
Landsat 8 aquires about 740 scenes a day on the Worldwide Reference System-2 (WRS-2) path/row system, with a swath overlap (or sidelap) varying from 7 percent at the Equator to a maximum of approximately 85 percent at extreme latitudes. The scene size is 185 km x 180 km (114 mi x 112 mi). Data products created from over 1.6 million Landsat 8 OLI/TIRS scenes are available to download from EarthExplorer, GloVis, and the LandsatLook Viewer. 

 
#### Landsat 8 Instruments

> Operational Land Imager (OLI)  -  Built by Ball Aerospace & Technologies Corporation

    Nine spectral bands, including a pan band:
        Band 1 Visible (0.43 - 0.45 µm) 30 m
        Band 2 Visible (0.450 - 0.51 µm) 30 m
        Band 3 Visible (0.53 - 0.59 µm) 30 m
        Band 4 Red (0.64 - 0.67 µm) 30 m
        Band 5 Near-Infrared (0.85 - 0.88 µm) 30 m
        Band 6 SWIR 1(1.57 - 1.65 µm) 30 m
        Band 7 SWIR 2 (2.11 - 2.29 µm) 30 m
        Band 8 Panchromatic (PAN) (0.50 - 0.68 µm) 15 m
        Band 9 Cirrus (1.36 - 1.38 µm) 30 m

> OLI captures data with improved radiometic precision over a 12-bit dynamic range, which improves overall signal to noise ratio. This translates into 4096 potential grey levels, compared with only 256 grey levels in Landsat 1-7 8-bit instruments. Improved signal to noise performance enables improved characterization of land cover state and condition.  

The 12-bit data are scaled to 16-bit integers and delivered in the Level-1 data products. Products are scaled to 55,000 grey levels, and can be rescaled to the Top of Atmosphere (TOA) reflectance and/or radiance using radiometric rescaling coefficients provided in the product metadata file (MTL file).

Thermal Infrared Sensor (TIRS)  -  Built by NASA Goddard  Space Flight Center 

    Two spectral bands:
        Band 10 TIRS 1 (10.6 - 11.19 µm) 100 m
        Band 11 TIRS 2 (11.5 - 12.51 µm) 100 m

### Download Landsat Data directly within QGIS -- Semi-Automatic Classification Plugin (SCP)

- Source URL - https://readthedocs.org/projects/semiautomaticclassificationmanual/downloads/pdf/latest/
- Source URL - https://fromgistors.blogspot.com/p/user-manual.html

> Semi-Automatic Classification Plugin - The Semi-Automatic Classification Plugin (SCP) allows for the supervised classification of remote sensing images, providing tools for the download, the preprocessing and postprocessing of images.   
Developed by Luca Congedo, the Semi-Automatic Classification Plugin (SCP) allows for the supervised classification of remote sensing images, providing tools for the download, the preprocessing and postprocessing of images. Search and download is available for ASTER, Landsat, MODIS, Sentinel-2, and Sentinel-3 images. Several algorithms are available for the land cover classification. This plugin requires the installation of GDAL, OGR, Numpy, SciPy, and Matplotlib. For more information please visit https://fromgistors.blogspot.com .  



### Global Croplands Data 

- Source URL - https://www.croplands.org/app/data/search?page=1&page_size=200

> The Global Croplands data . The NASA and related agencies effort towards Global Food Security . Part of the answer lies in understanding global croplands, both rainfed and irrigated, how they are used, their extents and how they can be better managed, particularly since they account for nearly 80% of all freshwater abstractions. Here technologies such as remote sensing will play an increasingly critical role – providing new spatial information to help manage croplands in a more productive and sustainable way.   


### Global Food Security Support Analysis Data (GFSAD)

- Source URL - https://lpdaac.usgs.gov/documents/168/GFSAD30SEACE_User_Guide_V1.pdf  

> This study conducted by NASA and associated agencies has collected data from both MODIS and LANDSAT-7&8. The basic introductory guide is - NASA_CropLand_LU-LC_GFSAD30SEACE_User_Guide_V1.pdf , this file was downloaded on 9th JUL 2020 from - ```Source URL sited above``` File also available in this repository at DIR -    


### US LANDSAT Analysis Ready Data 

- Source URL -- 

> Analysis Ready Data (ARD) , Data Format Control Book (DFCB) , ```LSDS-1873_US_Landsat_C1_ARD_DFCB-v6``` , this file was downloaded on 9th JUL 2020 from - ```Source URL sited above``` File also available in this repository at DIR -    


### LANDSAT Pixel Quality Assessment Band 

- Source URL - https://landsat.usgs.gov/sites/default/files/documents/landsat_QA_tools_userguide.pdf

> Relevant quote from the PDF ( source cited above ) - The bit-packed information in aQA band is adecimal translation of binary strings. Forexample, the decimal value “1” translates to the binary value “0001.” The binary value “0001” has 4 bits(0, 1, 2, and 3),written right to left as bits 0 (“1”), 1 (“0”), 2 (“0”), and 3 (“0”). Each of the bits 0-3 represents a condition that can affect the calculation of a physical value. Bit 0 may be used to identify fill values, bit 1 may be used to identify a cloud, bit 2 may be used to indicate water, and bit 3 may be used identify snow. If the condition is true, the bit is set to “1,” and “0” if false.    

> Used effectively, QA bits improve the integrity of science investigations by indicating which pixels might be affected by instrument artifacts or subject to cloudcontamination. For example, NDVI calculated over pixels containing clouds will show anomalous values. If such pixels were included in a phenology study, the results might not show the true characteristics of seasonal vegetation growth. Cloud contaminated pixels will lower NDVI values, and measures like the timing of ‘green up’ or peak maturity would appear later than they actually occurred. A worse consequence would be that the reported reduction of vegetation growth would be taken as an indicator of environmental change, potentially prompting unnecessary land management policies or practices   

<br/>

- Source URL - https://github.com/USGS-EROS/landsat-ldope-tools/tree/master/src

> The USGS-EROS/landsat-ldope-tools , GitHub repo is archived as on date


<br/>

- Source URL - https://www.usgs.gov/land-resources/nli/landsat/landsat-level-1-quality-assessment-tools?qt-science_support_page_related_con=2#qt-science_support_page_related_con

> The Landsat Level-1 QA bands are 16-bit files in GeoTIFF format which require robust image processing software.

To simplify the "unpacking" of the QA band information, the USGS developed the Landsat QA Tools, which were derived from the Moderate Resolution Imaging Spectroradiometer (MODIS) Land Data Operational Product Evaluation (LDOPE) Toolbox.   

The Landsat QA Tools originally supported Landsat data in Hierarchical Data Format (HDF), similar to MODIS data. However, the USGS has moved away from Landsat HDF data delivery and toward using GeoTIFF as the standard Landsat data product delivery format, and the Landsat QA Tools needed to be changed accordingly.   


- Source URL - https://openweather.co.uk/about

> Free Weather pre-processed data from - OpenWeather.co.uk   
The Quoted text below is an as is transcript from the - OpenWeather.co.uk - site , source sited above.    
Fortunately, global meteorological companies such as NOAA, MetOffice, Environment Canada, ECMWF, etc. share our belief that weather data should be open. They supply us with enormous data feeds including data from radars, weather satellites and weather stations. They also provide a lot of more specialised products such as road alerts, road risks and marine weather.  

Before weather data can find its way to businesses, it has to pass through the hands of developers, and they have to come to us. Our weather products are based on open data and open technologies. With our convolutional neural networks and ML technologies, we significantly enhance fundamental global forecast models with radar-based nowcasts, weather satellite data and the vast network of weather stations (82,000), rain gauges, and other weather sensors. Developers access these vast amounts of data via our light-speed, elegant APIs.  

With our APIs, you get data for any location on the globe: minute forecast (currently the US), hourly forecast, current weather, history, with vast range of meteorological parameters. All these remarkable products are available for free with up to 1,000,000 calls per month. For those who are looking for bigger service we provide several paid subscriptions and a range of historical products.  


- Source URL pySTEPS - NowCasting weather (in-place of ForeCasting ) - https://pysteps.readthedocs.io/en/latest/user_guide/index.html

> Work in Progress  


- Source URL - Sentinel-HUB Blog - https://medium.com/sentinel-hub/landsat-tweaks-panchromatic-and-thermal-bands-ddaf5a98d7f

> Pan-sharpening - Panchromatic sharpening (pan-sharpening) is a technique that merges high-resolution panchromatic data with medium-resolution multispectral data to create a multispectral image with higher-resolution features. Basically, it means using a panchromatic (single band) image to “sharpen” a multispectral image. In this sense, to “sharpen” means to increase the spatial resolution of a multispectral image.   


- Source URL -SURVIVAL GUIDE TO LANDSAT PRE-PROCESSING -  https://esajournals.onlinelibrary.wiley.com/doi/pdf/10.1002/ecy.1730


> Landsat data are increasingly used for ecological monitoring and research. These data  often  require  preprocessing  prior  to  analysis  to  account  for  sensor,  solar,  atmospheric,  and topographic effects. However, ecologists using these data are faced with a literature con-taining  inconsistent  terminology,  outdated  methods,  and  a  vast  number  of  approaches  with  contradictory recommendations. These issues can, at best, make determining the correct pre-processing  workflow  a  difficult  and  time-  consuming  task  and,  at  worst,  lead  to  erroneous  results. We address these problems by providing a concise overview of the Landsat missions and  sensors  and  by  clarifying  frequently  conflated  terms  and  methods.   


- Source URL Official USGS -- LANDSAT Collections , how they are processed and categorised - https://www.usgs.gov/land-resources/nli/landsat/landsat-collection-1?qt-science_support_page_related_con=1#qt-science_support_page_related_con

> Landsat scenes with the highest available data quality are placed into Tier 1 and are considered suitable for time-series analysis. Tier 1 includes Level-1 Precision and Terrain (L1TP) corrected data that have well-characterized radiometry and are inter-calibrated across the different Landsat instruments. The georegistration of Tier 1 scenes is consistent and within prescribed image-to-image tolerances of ≦ 12-meter radial root mean square error (RMSE).   



```
python code here --- Work in Progress
```


```
#rstats code here ( Thats actually R Code , im just abusing the #rstats hashtag Prof Hadley would be cross with me ) --- Work in Progress
```



<br/>



Rohit Dhankar - https://www.linkedin.com/in/rohitdhankar/




