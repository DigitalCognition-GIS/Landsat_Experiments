### This file has ROUGH NOTES , steps i followed , errors logs etc .( REFER with a pinch of salt)  


<p align="center">
    <img src="https://github.com/DigitalCognition-GIS/spaceNet/blob/master/ScreenCaptures_QGIS_SpaceNet_etc/Screenshot%20from%202020-07-05%2017-18-10.png" width= "850px">
</p>

<h1 align="center">LANDSAT Experiments - </h1>

> This repository will contain both code and additional reading material refrences for analytics and pseudo-projects done with the LANDSAT Data. (LANDSAT -8 Mostly) **- LANDSAT 2020**
 
> If you are a GIS developer or a GeoSpatial Scientist - kindly feel free to contribute. 


<br/>


### Table of Contents of this repository

- [X] `Intro to LANDSAT group of satellites` 
- [X] `Download and Preprocess LANDSAT -8 Data` 
- [X] `Further explorations with LANDSAT -8 Data` 
- [X] `Work in Progress` 
- [X] `Work in Progress` 
- [X] `Work in Progress` 
- [X] `Work in Progress` 


<br/>

### References - Always an ongoing effort - Work in Progress

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




