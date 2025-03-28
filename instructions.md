# Soil respiration reporting format instructions

A data package containing soil respiration data must include, at a minimum: 

1. Assemble the data table by downloading and filling in the data template in [XLSX](templates/data_reportingformat_template.xlsx) or [CSV](templates/data_reportingformat_template.csv) format. These serve as a guide for how the table should be structured. See our [data format guide](/data_reporting_format_guide.md) for descriptions and instructions for each data field.

2. Assemble the metadata table by downloading and filling in the chamber-level metadata template in [XLSX](templates/chammetadata_reportingformat_template.xlsx) or [CSV](templates/chammetadata_reportingformat_template.csv) formats. See our [chamber-level metadata format guide](chamber_level_metadata_guide.md) for descriptions and instructions for each field.

3. Ensure that all _required_ data types are included for each table (see required data tables below) and save each file as a `.csv`

4. Within the FLMD file, the [standard](https://github.com/ess-dive-workspace/essdive-file-level-metadata/blob/main/flmd_quick_guide.md#standard) for each soil respiration reporting format related file should be **ESS-DIVE Soil Respiration v1**. If submitting your dataset to ESS-DIVE, include the keyword **ESS-DIVE Soil Respiration Reporting Format** in the package-level metadata. 

| Required Data Variables                                                                        |
|:-----------------------------------------------------------------------------------------------|
| Chamber_ID                                                                                     |
| Timestamp_Begin                                                                                |
| Timestamp_End                                                                                  |
| Flux_CO2                                                                                        |

| Required Metadata Variables                                                                    |
|:-----------------------------------------------------------------------------------------------|
| Chamber_ID                                                                                     |
| Msmt_Var                                                                                       |
| Treatment                                                                                      |
| Opaque                                                                                         |
| Plants_Removed                                                                                 |
| Instrument                                                                                     |

## Additional information

Defined variables should be used where available. For **variables not yet covered** by this reporting format documentation, data contributors should use machine readable variable names that are in common use and follow ESS-DIVE data dictionary format guidelines as described [here](https://github.com/ess-dive-workspace/essdive-file-level-metadata/blob/master/CSV_dd/CSV_dd_instructions.md). 

Inclusion of additional related datasets with soil respiration data is encouraged. This can include measurements made inline, such as soil moisture or temperature, or subsequent analysis of chemical composition or physical properties. Related data should be linked by using common sample identifiers. 

We will continue to work with the ESS researchers to improve data and metadata reporting formats for soil respiration data. Please [contribute](contribute.md) by submitting issues, using our issue templates, or contact ess-dive-support@lbl.gov to provide any feedback on the process of formatting data or specific metadata fields.
