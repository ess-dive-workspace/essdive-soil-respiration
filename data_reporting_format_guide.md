# ESS-DIVE Soil Respiration Data Reporting Format

Here you will find proposed guidelines for formatting soil respiration data

---

## Soil Respiration Data Reporting Format - Link to More Details

[CHAMBER_ID](#chamber_id) | [TIMESTAMP_BEGIN](#timestamp_begin) | [TIMESTAMP_END](#timestamp_end) 

[DRY_CO2](#dry_co2) | [DRY_CH4](#dry_ch4) | [FLUX_CO2](#flux_co2) 

[FLUX_CH4](#flux_ch4) |[FLUX_SE_CO2](#flux_se_co2) |[FLUX_SE_CH4](#flux_se_ch4) 

[CRVFIT_CO2](#crvfit_co2) | [CRVFIT_CH4](#crvfit_ch4) |[R2_CO2](#r2_co2) 

[R2_CH4](#r2_ch4) | [ERROR](#error) | [CO2_AMB](#co2_amb) 

[CH4_AMB](#ch4_amb) | [TAIR_AMB](#tair_amb) | [TAIR](#tair) 

[PAR](#par) | [RH](#rh) | [PAR_AMB](#par_amb) 

[VPD_AMB](#vpd_amb) | [PRECIP_AMB](#precip_amb) | [Tx](#tx) 

[SMx](#smx) | [SOIL_O2](#soil_o2) | [WTD](#wtd) 

[RECORD](#record) | [NOTES](#notes) 

---

### CHAMBER_ID
|**field name**|CHAMBER_ID|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|required|
|**description**|Unique chamber label; must appear in chamber data table as well|
|**format**|character|
|**units**||

### TIMESTAMP_BEGIN
|**field name**|TIMESTAMP_BEGIN|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|required|
|**description**|ISO timestamp begin of averaging period (up to a 12-digit integer as specified by the data's temporal resolution)|
|**format**|integer|
|**units**|YYYYMMDDHHMM|

### TIMESTAMP_END
|**field name**|TIMESTAMP_END|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|required|
|**description**|ISO timestamp END of averaging period (up to a 12-digit integer as specified by the data's temporal resolution)|
|**format**|integer|
|**units**|YYYYMMDDHHMM|

### DRY_CO2
|**field name**|DRY_CO2|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Mean chamber CO2 concentration during measurement period|
|**format**|numeric|
|**units**|ppmv|

### DRY_CH4
|**field name**|DRY_CH4|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Mean chamber CH4 concentration during measurement period|
|**format**|numeric|
|**units**|ppbv|

### FLUX_CO2
|**field name**|FLUX_CO2|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|required|
|**description**|CO2 flux (positive = to atmosphere)|
|**format**|numeric|
|**units**|&#181;mol CO2/m2/s|

### FLUX_CH4
|**field name**|FLUX_CH4|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|CH4 flux (positive = to atmosphere)|
|**format**|numeric|
|**units**|nmol CH4/m2/s|

### FLUX_SE_CO2
|**field name**|FLUX_SE_CO2|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Standard error of CO2 flux computation|
|**format**|numeric|
|**units**|&#181;mol CO2/m2/s|

### FLUX_SE_CH4
|**field name**|FLUX_SE_CH4|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Standard error of CH4 flux computation|
|**format**|numeric|
|**units**|nmol CH4/m2/s|

### CRVFIT_CO2
|**field name**|CRVFIT_CO2|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|CO2 flux computation method ("Lin" or "Exp" for linear and exponential)|
|**format**|character|
|**units**||

### CRVFIT_CH4
|**field name**|CRVFIT_CH4|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|CH4 flux computation method ("Lin" or "Exp" for linear and exponential)|
|**format**|character|
|**units**||

### R2_CO2
|**field name**|R2_CO2|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|R2 of CO2 flux computation|
|**format**|numeric|
|**units**|fraction|

### R2_CH4
|**field name**|R2_CH4|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|R2 of CH4 flux computation|
|**format**|numeric|
|**units**|fraction|
 
### ERROR
|**field name**|ERROR|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Error generated by analyzer or during import|
|**format**|logical|
|**units**||

### CO2_AMB
|**field name**|CO2_AMB|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Ambient CO2 concentration at measurement location|
|**format**|numeric|
|**units**|ppmv|

### CH4_AMB
|field name|CH4_AMB|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement_level|optional|
|description|Ambient CH4 concentration at measurement location|
|format|numeric|
|units|ppbv|

### TAIR_AMB
|field name|TAIR_AMB|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement_level|optional|
|description|Ambient air temperature at measurement location|
|format|numeric|
|units|&#8451;|

### TAIR
|field name|TAIR|
|:----------------------------------------------------|:----------------------------------------------------|
|requirement_level|optional|
|**description|Air temperature inside measurement chamber|
|**format|numeric|
|**units**|&#8451;|

### PAR
|**field name**|PAR|
|:----------------------------------------------------|:----------------------------------------------------|
|**equirement_level**|optional|
|**description**|Photosynthetically active radiation inside measurement chamber|
|**format**|numeric|
|**units**|&#181;mol photons/m2/s|

### RH
|**field name**|RH|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Relative humidity inside measurement chamber|
|**format**|numeric|
|**units**|%|

### PAR_AMB
|**field name**|PAR_AMB|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Photosynthetically active radiation outside measurement chamber|
|**format**|numeric|
|**units**|&#181;mol photons/m2/s|

### VPD_AMB
|**field name**|VPD_AMB|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Vapor pressure deficit at measurement location|
|**format**|numeric|
|**units**|Pa|

### PRECIP_AMB
|**field name**|PRECIP_AMB|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Precipitation at measurement location|
|**format**|numeric|
|**units**|mm|

### Tx
|**field name**|Tx|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Soil temperature at x cm (for additional "Tx" fields, follow same format, e.g. T5, T15)|
|**format**|numeric|
|**units**|&#8451;|

### SMx
|**field name**|SMx|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Volumetric soil moisture at x cm depth (for additional "SMx" fields, follow the same format, e.g. SM5, SM15)|
|**format**|numeric|
|**units**|m3/m3|

### SOIL_O2
|**field name**|SOIL_O2|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Soil oxygen level at measurement chamber|
|**format**|numeric|
|**units**|%|

### WTD
|**field name**|WTD|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Water table depth at measurement location, positive numbers are depth|
|**format**|numeric|
|**units**|cm|

### RECORD
|**field name**|RECORD|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Record number within file|
|**format**|integer|
|**units**||

### NOTES
|**field name**|NOTES|
|:----------------------------------------------------|:----------------------------------------------------|
|**requirement_level**|optional|
|**description**|Additional information about this measurement|
|**format**|character|
|**units**||
