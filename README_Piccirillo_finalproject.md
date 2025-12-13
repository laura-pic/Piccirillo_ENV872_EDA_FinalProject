# Piccirillo_ENV872_EDA_FinalProject

## Summary

Repository for ENV872 final project by Laura Piccirillo, focused on selenium concentrations in the Eastern Tropical Pacific Ocean. The seawater samples included in this analysis were collected with Go-FLO trace-metal clean bottles in 2013 on the U.S. GEOTRACES East Pacific Zonal Transect (GP16) cruise from Peru to Tahiti. 

Selenium (Se) is a trace element and exists in various oxidation states throughout the water column (selenate, selenite, elemental Se, selenide). The marine biogeochemical cycling of Se is not well constrained, and these concentration measurements of the various forms of Se are helpful to better understand its cycling. Here, concentrations of selenite, selenate, and organic selenide were compared to depth and dissolved oxygen concentrations using multiple regression analyses across this cruise transect.

This project was carried out in December 2025.

## Investigators

Laura Piccirillo, PhD Student at Duke University, [laura.piccirillo\@duke.edu](mailto:laura.piccirillo@duke.edu)

## Keywords

Selenium, trace elements, GEOTRACES, Pacific Ocean

## Database Information

Two data files were used in this project.

The first data file was accessed on November 14, 2025 from the "Biological and Chemical Oceanography Data Management Office" (BCO-DMO) website: https://www.bco-dmo.org/

Link to the dataset webpage: https://www.bco-dmo.org/dataset/647606

Citation for the dataset: Cutter, G. A. (2017) Arsenate, iodide, and selenium concentrations collected from Go-FLO bottles during the R/V Thomas G. Thompson cruise TN303 from Peru to Tahiti in 2013 (U.S. GEOTRACES EPZT project). Biological and Chemical Oceanography Data Management Office (BCO-DMO). (Version 1) Version Date 2017-01-03. http://lod.bco-dmo.org/id/dataset/647606

The second data file was accessed on December 2, 2025 from the "Biological and Chemical Oceanography Data Management Office" (BCO-DMO) website: https://www.bco-dmo.org/

Link to the dataset webpage: https://www.bco-dmo.org/dataset/522668

Citation for the dataset: Moffett, J. W., Cutter, G. A., German, C. R. (2014). GTC shipboard CTD data along the US GEOTRACES East Pacific Zonal Transect from the R/V Thomas G. Thompson TN303 cruise in the tropical Pacific from Peru to Tahiti during 2013 (U.S. GEOTRACES EPZT project). Biological and Chemical Oceanography Data Management Office (BCO-DMO). (Version 30 October 2014) Version Date 2014-10-30. http://lod.bco-dmo.org/id/dataset/522668

The two data files were eventually merged in this project by matching latitude and longitude (rounded to 3 decimal points) and depth (rounded to 0 decimal points).

## Folder structure, file formats, and naming conventions

Folders for code, data, and output are present. 

Code folder: Three Rmarkdown documents for the data exploration, processing, and analysis, which were named as such.

Data folder (Raw): CSV files for raw data downloaded from http://lod.bco-dmo.org/id/dataset/647606 and https://www.bco-dmo.org/dataset/522668. File names remained in original form from download.

Data folder (Processed): CSV files for the explored and processed datasets. Explored datasets kept the naming conventions from the original download. Processed datasets were named for what they contained (Se data with oxygen vs. OMZ data only).

Output folder: Contains the final Rmarkdown used for the project report, rendered to HTML.

## Metadata
Additional information on parameters can be found on dataset webpages linked above.

Data (Raw):

As_Se_IO_BOTTLE.csv

Column names with descriptions, class, units: 

CASTNO: GEOTRACES cast number for that station.

STNNBR: Station number.	

GEOTRC_EVENTNO: GEOTRACES event number.

GEOTRC_SAMPNO: GEOTRACES sample number.

EVENT_LON: Longitude according to event log; West is negative, decimal degrees	

EVENT_LAT: Latitude at the start of event, according to log, decimal degrees	

BTMDEPTH: bottom Depth, meters	

DEPTH: depth of sample, meters	

SAMPNO: Bottle sample number

BTLNBR: Bottle number

PI_DATE: PI-supplied date in format YYYYMMDD

PI_TIME: PI-supplied time in format HHMM

As_III_D_CONC_BOTTLE: dissolved Arsenite concentration from a bottle sample, 
nanomoles per liter	

As_V_D_CONC_BOTTLE: dissolved Arsenate concentration from a bottle sample
nanomoles per liter	

Se_TD_CONC_BOTTLE: total dissolved Selenium concentration from a bottle sample
nanomoles per liter	

Se_IV_D_CONC_BOTTLE: dissolved Selenite concentration from a bottle sample
nanomoles per liter	

Se_VI_D_CONC_BOTTLE: dissolved Selenate concentration from a bottle sample
nanomoles per liter	

Org_Se_II_CONC_BOTTLE: organic Selenide concentration from a bottle sample
nanomoles per liter	

IODIDE_D_CONC_BOTTLE: dissolved iodide concentration from a bottle sample
nanomoles per liter	

IO3_D_CONC_BOTTLE: dissolved iodate concentration from a bottle sample
nanomoles per liter	

ISO_DATETIME_UTC_START_EVENT: Date and time (UTC) at start of the event according to the event log. Format is ISO 8601 standard YYYY-mm-ddTHH:MM:SS.xxZ. Values were added from the intermediate US GEOTRACES master file (see Processing Description).

BTL_DATE: Date when the bottle was fired; according to the bottle file. Format yyyymmdd.

BTL_TIME: Time when the bottle was fired; according to the bottle file. Format HHMM.

BTL_LAT: Latitude of bottle firing; north is positive, decimal degrees	

BTL_LON: Longitude of bottle firing; east is positive. decimal degrees	

SECT_ID: Transect identifier for GEOTRACES Eastern Pacific Zonal Transect (EPZT)


GT-C_SBE_CTD_Proc_v30Oct2014.csv

DATASET_ID: CTD Dataset Identifier

EXPOCODE: expedition code assigned by the CCHDO: NODCShipCodeYearMonthDay

SECT_ID: cruise section identification number

GEOTRC_EVENTNO: GEOTRACES Event Number (dimensionless	event)

DATE: Station Date (GMT) format YYYYMMDD

TIME: Station Time (GMT) HHMM	

LATITUDE: Station Latitude (South is negative), decimal degrees	

LONGITUDE: Station Longitude (West is negative), decimal degrees	

PrDM: Pressure Digiquartz, dbar

T090C: Temperature ITS-90, degrees celsius

T190C: Temperature 2 ITS-90, degrees celsius	

C0S: Conductivity, S/m	

C1S: Conductivity 2, S/m	

Sbeox0V: Oxygen raw SBE 43, volts	

Xmiss: Beam Transmission Chelsea/Seatech, percentage	

FlSP: Fluorescence Seapoint, nd

SeaTurbMtr: Turbidity Seapoint, FTU	

DepSM: Depth salt water  lat = -12.0057, meters	

Sal00: Salinity Practical, PSU	

Sal11: Salinity 2 Practical, PSU	

Density00: Density (density), kg/m^3	

Density11: Density 2 (density), kg/m^3	

Sigma_e00: Density sigma-theta, kg/m^3	

Sigma_e11: Density 2 sigma-theta, kg/m^3	

Sbeox0: Oxygen SBE 43  WS = 2, umol/kg

Flag: Flag

ISO_DATE_TIME: Date/Time (ISO formatted), YYYY-MM-DDTHH:MM:SS[.xx]Z


Data (Processed):
As_Se_IO_BOTTLE_Explored.csv: same parameters as As_Se_IO_BOTTLE.csv listed above.

GT-C_SBE_CTD_Proc_v30Oct2014_Explored.csv: same parameters as GT-C_SBE_CTD_Proc_v30Oct2014.csv listed above.


se_oxygen_processed.csv

EVENT_LAT: Station Latitude (South is negative), decimal degrees	

EVENT_LON: Station Longitude (West is negative), decimal degrees

PI_DATE: YYYYMMDD

depth: water depth, meters

Se_IV_D_CONC_BOTTLE: selenite concentration, nmol/L

Se_VI_D: selenate concentration, nmol/L

Org_Se_II_CONC_BOTTLE: organic selenide concentration, nmol/L

meanOxygen: oxygen averaged for matching latitude/longitude/depth points, umol/kg


OMZ_data_processed.csv

EVENT_LAT: Station Latitude (South is negative), decimal degrees

EVENT_LON: Station Longitude (West is negative), decimal degrees

PI_DATE: YYYYMMDD

depth: water depth, meters

Se_IV_D_CONC_BOTTLE: selenite concentration, nmol/L

Se_VI_D: selenate concentration, nmol/L

Org_Se_II_CONC_BOTTLE: organic selenide concentration, nmol/L

DATE: YYYYMMDD

Sbeox0: Processed oxygen onboard, umol/kg
