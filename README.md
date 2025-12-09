# Biodiversity Intactness Index Change
## Investigating the impacts of urban expansion in Maricopa County in Phoenix, AZ.
Repository containing all code and output for the final project in class EDS 220 of the [Master of Environmental Data Scienct (MEDS) program](https://bren.ucsb.edu/masters-programs/master-environmental-data-science) - Working with Environmental Datasets. 

![](https://upload.wikimedia.org/wikipedia/commons/3/38/BLM_Winter_Bucket_List_-25-_Agua_Fria_National_Monument%2C_Arizona%2C_for_a_Natural_and_Historic_Getaway_near_Superbowl_49_%2816335859491%29.jpg) 
Credit: Bureau of Land Management

# About
The biodiversity intactness index (BII) is a measure of a region's average remaining natural biodiversity. Its measured using data on plants, fungi and animals. Scientists can use BII to assess an environmental's community to various human pressures. In this study, we will the area of Maricopa county in Arizona, home to the Phoenix metropolitan area, as it is regarded as a county with significant increase in developed land since 2001. 

## Highlights
1. Access and manipulate `STAC` data.
2. Clip and filter `xarray.DataArray` according to conditions.
3. Calculate BII statistics using `xarray.DataArray`
4. Map BII loss.

# Data
BII data were sourced from the [Microsoft Planetary Computer](https://planetarycomputer.microsoft.com/dataset/io-biodiversity). These data are housed in a public catalog of many collections, and we will access the io-biodiversity catalog for our area of interest.
Data access: Data for this project were accessed on 12/01/2025. These data can be accessed in-code without downloading and storing any data using `pystac_client` and `planetary_computer`.

Shapefiles for the area of Maricopa county in Arizone were sourced from [U.S. Census Bureau Topologically Integrated Geographic Encoding and Referencing (MAF/TIGER) Database (MTDB)](https://catalog.data.gov/dataset/tiger-line-shapefile-2023-county-maricopa-county-az-topological-faces-polygons-with-all-geocode/resource/ddb9186b-11a1-484b-98e0-7fbcb3f8cbe2). These data contain polygons for every county subdivision in Arizona, which we will subset for our area of interest. 
Data access: Data for this project were accessed on 12/01/2025. Data can be downloaded from the link above as a zip. Unzip into local repository using the following data structure (note: data are not pushed to github due to size constraints. It is recommended to hide data with `.gitignore`: 

# Content
```bash 
repository
│   README.md: contains README code.
|   bii_change.ipnyb: The project code and output.
Data are not pushed to github, this is the recommended file structure:
|   .gitignore
|   └── data folder
        │   data-shapefiles
```
# Citations
Z. Levitt and J. Eng, “Where America’s developed areas are growing: ‘Way off into the horizon’,” The Washington Post, Aug. 2021, Available: https://www.washingtonpost.com/nation/interactive/2021/land-development-urban-growth-maps/. [Accessed: Nov. 22, 2024]

Microsoft Planetary Computer. (2024). Microsoft.com. https://planetarycomputer.microsoft.com/dataset/io-biodiversity

Data.gov. (2023). Data.gov. https://catalog.data.gov/dataset/tiger-line-shapefile-2023-county-maricopa-county-az-topological-faces-polygons-with-all-geocode/resource/ddb9186b-11a1-484b-98e0-7fbcb3f8cbe2

# Acknowledgments
This work was done by Leela Dixit, with support from Carmen Galaz García, Annie Adams, and classmates from the MEDS [EDS 220](https://bren.ucsb.edu/courses/eds-220) UCSB course. 
