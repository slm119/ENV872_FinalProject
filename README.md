# ENV872_FinalProject


## Summary

This repository contains code and analysis for a time series investigation of heavy metal concentrations in Mytilus edulis (blue mussels) using environmental monitoring data from several European countries collected between 1979 to 2018. Mytilus edulis are commonly used for coastal biomonitoring efforts due to their wide habitat range and their tendency to filter and collect aquatic pollutants, including heavy metals. Monitoring pollutant concentrations in Mylius edulis can help provide an indication of overall ecosystem health. Additionally, these bivalves are an important commercially harvested species and so high levels of heavy metals can also be a threat to human health. In the current study, statistical analyses were conducted to determine how concentrations of lead and cadmium in Mytilus edulis have changed over the study period from 1979 to 2018. 

## Investigators

Data and anlaysis were prepared by Sena McCrory, a masters student at the Nicholas School of the Environment, Duke University. 

Contact information: sena.mccrory@duke.edu


## Keywords

ICES, marine contaminants, heavy metals, cadmium, biomonitoring, lead, Mytilus edulis, blue mussel

## Database Information

Existing publically available databases were used for all analyses. 

Biological Contaminants Data:
Data for contaminants in biota was dowloaded from the International Council for the Exploration of the Sea (ICES) DOME database on Feb 26, 2020. This data portal holds a collection of marine related monitoring data sourced from several regional European monitoring groups including ICES, OSPAR, HELCOM, AMAP, and Expert Groups. Data for all metal and metalloid concentrations in biota were downloaded and then filtered for just Mytilus edulis species and the specific heavy metals of interest for this study.The ICES DOME data portal can be accessed here:http://dome.ices.dk/views/ContaminantsBiota.aspx. Geographic locations are given in decimal degrees (WGS84). 

Global Coastline Data: 
Global Self-consistent Hierarchical High-resolution Geography (GSHHG) coastline data was downloaded from the National Oceanographic and Atmospheric Administration's (NOAA) National Center for Environmental Information (NCEI) online data portal located here: https://www.ngdc.noaa.gov/mgg/shorelines/. L1 resolution shapefile was used for study sampling maps in this analysis. Geographic reference system is WGS84 (decimal degrees). 


## Folder structure, file formats, and naming conventions 

* Code: contains all data processing and analysis code
* Data: contains folders for metadata, raw data (tables only), processed data, and spatial data.
* Resources: contains publications and reference materials related to the analysis
* Output: contains any saved figures, tables, created durign analysis, as well as the final report in Rmarkdown format. 

File types used in this repository include Rmarkdown documents, .csv, .pdf, and spatial data are stored as ESRI shapefiles, .shp. 

Naming conventions -
* Raw data files have their original names as they were downloads.
* Processed datasets are named as follows "DataSource_Species_contaminant.csv"
* Other files use self explanatory names such as "DataAnalysis" or "DataProcessing" where the first letter of each word is capitolized.

## Metadata

Processed data file "ICES_Mytilusedulis_Cd_Pb_Hg_Cu.csv" column names are described in detail in the metadata file located in /Data/Metadata/DOMEdata/'Contaminants and effects of contaminants in biota.pdf'.

## Scripts and code

Main repository folder contains three additional scripts:
* 'README' (this document)
* 'LICENSE' describing the GNU General Pubilic License
* '.gitignore' which contains and files which were not synced to the github repository due to file size constraints. 

## Quality assurance/quality control

ICES DOME data QA/QC: All data flagged as "suspect" data quality were excluded from the analysis. After all necessary filtering was completed, only a few obvious outliers remained in the data. These outliers were retained in the data for statistical analysis, but may not be shown in the visual representations of the data due to scaling issues. 
