# Data Guide

Here you will find proposed guidelines for formatting soil respiration data

## Soil Respiration Data Reporting Format - Link to More Details

[Chamber ID](data_reporting_format_guide.md#chamber_id) | [Timestamp Begin](data_reporting_format_guide.md#timestamp_begin) | [Timestamp End](data_reporting_format_guide.md#timestamp_end)

[CO2 Flux](data_reporting_format_guide.md#flux_co2) | [Dry CO2](data_reporting_format_guide.md#dry_co2) | [CO2 Flux Standard Error](data_reporting_format_guide.md#flux_se_co2)

[CO2 Curve Fit](data_reporting_format_guide.md#crvfit_co2) | [CO2 R2](data_reporting_format_guide.md#r2_co2) | [Error](data_reporting_format_guide.md#error)

[Ambient CO2](data_reporting_format_guide.md#co2_amb) | [Ambient Tair](data_reporting_format_guide.md#tair_amb) | [Tair](data_reporting_format_guide.md#tair)

[PAR](data_reporting_format_guide.md#par) | [RH](data_reporting_format_guide.md#rh) | [Ambient PAR](data_reporting_format_guide.md#par_amb)

[Ambient VPD](data_reporting_format_guide.md#vpd_amb) | [Ambient Precip](data_reporting_format_guide.md#precip_amb) | [Tx](data_reporting_format_guide.md#tx)

[SMx](data_reporting_format_guide.md#smx) | [Soil O2](data_reporting_format_guide.md#soil_o2) | [WTD](data_reporting_format_guide.md#wtd)

[Record](data_reporting_format_guide.md#record) | [Notes](data_reporting_format_guide.md#notes)

### Chamber\_ID

| **field name**         | Chamber\_ID                                                     |
| ---------------------- | --------------------------------------------------------------- |
| **requirement\_level** | required                                                        |
| **description**        | Unique chamber label; must appear in chamber data table as well |
| **format**             | character                                                       |
| **units**              |                                                                 |

### Timestamp\_Begin

| **field name**         | Timestamp\_Begin                                                                                                  |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------- |
| **requirement\_level** | required                                                                                                          |
| **description**        | ISO timestamp begin of averaging period (up to a 12-digit integer as specified by the data's temporal resolution) |
| **format**             | integer                                                                                                           |
| **units**              | YYYYMMDDHHMM                                                                                                      |

### Timestamp\_End

| **field name**         | Timestamp\_End                                                                                                  |
| ---------------------- | --------------------------------------------------------------------------------------------------------------- |
| **requirement\_level** | required                                                                                                        |
| **description**        | ISO timestamp END of averaging period (up to a 12-digit integer as specified by the data's temporal resolution) |
| **format**             | integer                                                                                                         |
| **units**              | YYYYMMDDHHMM                                                                                                    |

### Flux\_CO2

| **field name**         | Flux\_CO2                                                                |
| ---------------------- | ------------------------------------------------------------------------ |
| **requirement\_level** | required                                                                 |
| **description**        | CO2 flux (positive = to atmosphere); negative values are also acceptable |
| **format**             | numeric                                                                  |
| **units**              | µmol CO2 m-2 s-1                                                         |

### Dry\_CO2

| **field name**         | Dry\_CO2                                                 |
| ---------------------- | -------------------------------------------------------- |
| **requirement\_level** | optional                                                 |
| **description**        | Mean chamber CO2 concentration during measurement period |
| **format**             | numeric                                                  |
| **units**              | ppmv                                                     |

### Flux\_SE\_CO2

| **field name**         | Flux\_SE\_CO2                          |
| ---------------------- | -------------------------------------- |
| **requirement\_level** | optional                               |
| **description**        | Standard error of CO2 flux computation |
| **format**             | numeric                                |
| **units**              | µmol CO2 m-2 s-1                       |

### CrvFit\_CO2

| **field name**         | CrvFit\_CO2                                                             |
| ---------------------- | ----------------------------------------------------------------------- |
| **requirement\_level** | optional                                                                |
| **description**        | CO2 flux computation method ("Lin" or "Exp" for linear and exponential) |
| **format**             | character                                                               |
| **units**              |                                                                         |

### R2\_CO2

| **field name**         | R2\_CO2                    |
| ---------------------- | -------------------------- |
| **requirement\_level** | optional                   |
| **description**        | R2 of CO2 flux computation |
| **format**             | numeric                    |
| **units**              | fraction                   |

### Error

| **field name**         | Error                                        |
| ---------------------- | -------------------------------------------- |
| **requirement\_level** | optional                                     |
| **description**        | Error generated by analyzer or during import |
| **format**             | logical                                      |
| **units**              |                                              |

### CO2\_Amb

| **field name**         | CO2\_Amb                                          |
| ---------------------- | ------------------------------------------------- |
| **requirement\_level** | optional                                          |
| **description**        | Ambient CO2 concentration at measurement location |
| **format**             | numeric                                           |
| **units**              | ppmv                                              |

### Tair\_Amb

| **field name**         | Tair\_Amb                                       |
| ---------------------- | ----------------------------------------------- |
| **requirement\_level** | optional                                        |
| **description**        | Ambient air temperature at measurement location |
| **format**             | numeric                                         |
| **units**              | ℃                                               |

### Tair

| **field name**         | Tair                                       |
| ---------------------- | ------------------------------------------ |
| **requirement\_level** | optional                                   |
| **description**        | Air temperature inside measurement chamber |
| **format**             | numeric                                    |
| **units**              | ℃                                          |

### PAR

| **field name**         | PAR                                                            |
| ---------------------- | -------------------------------------------------------------- |
| **requirement\_level** | optional                                                       |
| **description**        | Photosynthetically active radiation inside measurement chamber |
| **format**             | numeric                                                        |
| **units**              | µmol photons m-2 s-1                                           |

### RH

| **field name**         | RH                                           |
| ---------------------- | -------------------------------------------- |
| **requirement\_level** | optional                                     |
| **description**        | Relative humidity inside measurement chamber |
| **format**             | numeric                                      |
| **units**              | %                                            |

### PAR\_Amb

| **field name**         | PAR\_AMB                                                        |
| ---------------------- | --------------------------------------------------------------- |
| **requirement\_level** | optional                                                        |
| **description**        | Photosynthetically active radiation outside measurement chamber |
| **format**             | numeric                                                         |
| **units**              | µmol photons m-2 s-1                                            |

### VPD\_AMB

| **field name**         | VPD\_AMB                                       |
| ---------------------- | ---------------------------------------------- |
| **requirement\_level** | optional                                       |
| **description**        | Vapor pressure deficit at measurement location |
| **format**             | numeric                                        |
| **units**              | Pa                                             |

### Precip\_Amb

| **field name**         | Precip\_Amb                           |
| ---------------------- | ------------------------------------- |
| **requirement\_level** | optional                              |
| **description**        | Precipitation at measurement location |
| **format**             | numeric                               |
| **units**              | mm                                    |

### Tx

| **field name**         | Tx                                                                                      |
| ---------------------- | --------------------------------------------------------------------------------------- |
| **requirement\_level** | optional                                                                                |
| **description**        | Soil temperature at x cm (for additional "Tx" fields, follow same format, e.g. T5, T15) |
| **format**             | numeric                                                                                 |
| **units**              | ℃                                                                                       |

### SMx

| **field name**         | SMx                                                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------ |
| **requirement\_level** | optional                                                                                                     |
| **description**        | Volumetric soil moisture at x cm depth (for additional "SMx" fields, follow the same format, e.g. SM5, SM15) |
| **format**             | numeric                                                                                                      |
| **units**              | m3 m-3                                                                                                       |

### Soil\_O2

| **field name**         | Soil\_O2                                 |
| ---------------------- | ---------------------------------------- |
| **requirement\_level** | optional                                 |
| **description**        | Soil oxygen level at measurement chamber |
| **format**             | numeric                                  |
| **units**              | %                                        |

### WTD

| **field name**         | WTD                                                                   |
| ---------------------- | --------------------------------------------------------------------- |
| **requirement\_level** | optional                                                              |
| **description**        | Water table depth at measurement location, positive numbers are depth |
| **format**             | numeric                                                               |
| **units**              | cm                                                                    |

### Record

| **field name**         | Record                    |
| ---------------------- | ------------------------- |
| **requirement\_level** | optional                  |
| **description**        | Record number within file |
| **format**             | integer                   |
| **units**              |                           |

### Notes

| **field name**         | Notes                                         |
| ---------------------- | --------------------------------------------- |
| **requirement\_level** | optional                                      |
| **description**        | Additional information about this measurement |
| **format**             | character                                     |
| **units**              |                                               |
