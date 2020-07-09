### This file has ROUGH NOTES , steps i followed , errors logs etc .( REFER with a pinch of salt)  


<p align="center">
    <img src="https://github.com/DigitalCognition-GIS/spaceNet/blob/master/ScreenCaptures_QGIS_SpaceNet_etc/Screenshot%20from%202020-07-05%2017-18-10.png" width= "850px">
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



```
python code here --- Work in Progress
```


```
#rstats code here ( Thats actually R Code , im just abusing the #rstats hashtag Prof Hadley would be cross with me ) --- Work in Progress
```



<br/>



Rohit Dhankar - https://www.linkedin.com/in/rohitdhankar/




