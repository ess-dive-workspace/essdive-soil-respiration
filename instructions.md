# Soil respiration reporting format instructions

A data package containing soil respiration data must include, at a minimum: 

1. Assemble the data table by downloading and filling in the [data template](https://github.com/ess-dive-community/essdive-soil-respiration/blob/main/templates/data_reportingformat_template.xlsx). These serve as a guide for how the table should be structured. See our [data format guide](https://github.com/ess-dive-community/essdive-soil-respiration/blob/main/data_reporting_format_guide.md) for descriptions and instructions for each data field.

2. Assemble the metadata table by downloading and filling in the [chamber-level metadata template](https://github.com/ess-dive-community/essdive-soil-respiration/blob/main/templates/chammetadata_reportingformat_template.xlsx). See our [chamber-level metadata format guide](https://github.com/ess-dive-community/essdive-soil-respiration/blob/main/chamber_level_metadata_guide.md) for descriptions and instructions for each field.

4. Ensure that all _required_ data types are included for each table (see required data tables below) and save each file as a `.csv` 

| Required Data Variables                                                                        |
|:-----------------------------------------------------------------------------------------------|
| Chamber_ID                                                                                     |
| Timestamp_Begin                                                                                |
| Timestamp_End                                                                                  |
| Dry_CO2                                                                                        |

| Required Metadata Variables                                                                    |
|:-----------------------------------------------------------------------------------------------|
| Chamber_ID                                                                                     |
| Msmt_Var                                                                                       |
| Treatment                                                                                      |
| Opaque                                                                                         |
| Plants_Removed                                                                                 |
| Instrument                                                                                     |

## Additional information

Defined variables should be used where available. For **variables not yet covered** by this reporting format documentation, data contributors should use machine readable variable names that are in common use and follow ESS-DIVE data dictionary format guidelines as described [here](https://github.com/ess-dive-community/essdive-file-level-metadata/blob/master/CSV_dd/CSV_dd_instructions.md). 

Inclusion of additional related datasets with soil respiration data is encouraged. This can include measurements made inline, such as soil moisture or temperature, or subsequent analysis of chemical composition or physical properties. Related data should be linked by using common sample identifiers. 

We will continue to work with the ESS community to improve data and metadata reporting formats for soil respiration data. Please [contribute](contribute.md) by submitting issues, using our issue templates, or contact ess-dive-support@lbl.gov to provide any feedback on the process of formatting data or specific metadata fields.
