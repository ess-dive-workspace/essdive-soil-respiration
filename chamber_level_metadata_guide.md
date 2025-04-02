# Chamber Level Metadata Guide

Here you will find proposed guidelines for standardizing chamber level soil respiration data

## Chamber Level Metadata Content - Link to More Details

[Chamber ID](chamber_level_metadata_guide.md#chamber-id) | [Measurement Variable](chamber_level_metadata_guide.md#measurement-variable) |[Treatment](chamber_level_metadata_guide.md#treatment)

[Opaque](chamber_level_metadata_guide.md#opaque) | [Plants Removed](chamber_level_metadata_guide.md#plants-removed) | [Instrument](chamber_level_metadata_guide.md#instrument)

[Longitude](chamber_level_metadata_guide.md#longitude) | [Latitude](chamber_level_metadata_guide.md#latitude) | [Area](chamber_level_metadata_guide.md#area)

[Volume](chamber_level_metadata_guide.md#volume) | [Observation Count](chamber_level_metadata_guide.md#observation-count) | [Collar Depth](chamber_level_metadata_guide.md#collar-depth)

[Fan](chamber_level_metadata_guide.md#fan) | [Species](chamber_level_metadata_guide.md#species)

[Sensor Depths](chamber_level_metadata_guide.md#sensor-depths) | [Notes](chamber_level_metadata_guide.md#notes)

### Chamber ID

| **field name**        | Chamber\_ID                                                  |
| --------------------- | ------------------------------------------------------------ |
| **requirement level** | required                                                     |
| **description**       | Unique chamber label; must appear in flux data table as well |
| **format**            | character                                                    |
| **units**             |                                                              |

### Measurement variable

| **field name**        | Msmt\_Var                                                                                                                                                                            |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **requirement level** | required                                                                                                                                                                             |
| **description**       | Flux should be interpreted as: "Rs" (soil respiration, whether CO2 or CH4), "Rh" (heterotrophic respiration only), "Reco" (ecosystem respiration), or "NEE" (net ecosystem exchange) |
| **format**            | character                                                                                                                                                                            |
| **units**             |                                                                                                                                                                                      |

### Treatment

| **field name**        | Treatment                                                                      |
| --------------------- | ------------------------------------------------------------------------------ |
| **requirement level** | required                                                                       |
| **description**       | Soil or ecosystem treatment applied at measurement location; default is "None" |
| **format**            | character                                                                      |
| **units**             |                                                                                |

### Opaque

| **field name**        | Opaque          |
| --------------------- | --------------- |
| **requirement level** | required        |
| **description**       | Opaque chamber? |
| **format**            | logical         |
| **units**             |                 |

### Plants removed

| **field name**        | Plants\_Removed                    |
| --------------------- | ---------------------------------- |
| **requirement level** | required                           |
| **description**       | Plants removed from inside collar? |
| **format**            | logical                            |
| **units**             |                                    |

### Instrument

| **field name**         | Instrument                          |
| ---------------------- | ----------------------------------- |
| **requirement\_level** | required                            |
| **description**        | Measurement instrument (i.e. model) |
| **format**             | character                           |
| **units**              |                                     |

### Longitude

| **field name**        | Longitude                                                  |
| --------------------- | ---------------------------------------------------------- |
| **requirement level** | optional                                                   |
| **description**       | Decimal longitude of measurement location, positive = east |
| **format**            | numeric                                                    |
| **units**             | degrees                                                    |

### Latitude

| **field name**        | Latitude                                                   |
| --------------------- | ---------------------------------------------------------- |
| **requirement level** | optional                                                   |
| **description**       | Decimal latitude of measurement location, positive = north |
| **format**            | numeric                                                    |
| **units**             | degrees                                                    |

### Area

| **field name**        | Area                          |
| --------------------- | ----------------------------- |
| **requirement level** | optional                      |
| **description**       | Soil surface measurement area |
| **format**            | numeric                       |
| **units**             | cm2                           |

### Volume

| **field name**        | Volume                        |
| --------------------- | ----------------------------- |
| **requirement level** | optional                      |
| **description**       | Volume of measurement chamber |
| **format**            | numeric                       |
| **units**             | cm3                           |

### Observation Count

| **field name**        | Obs\_Count                                                                                               |
| --------------------- | -------------------------------------------------------------------------------------------------------- |
| **requirement level** | optional                                                                                                 |
| **description**       | Observation count representing how many measurement cycles were completed and used to calculate the flux |
| **format**            | numeric                                                                                                  |
| **units**             |                                                                                                          |

### Collar depth

| **field name**        | Collar\_Depth             |
| --------------------- | ------------------------- |
| **requirement level** | optional                  |
| **description**       | Depth of collar insertion |
| **format**            | numeric                   |
| **units**             | cm                        |

### Fan

| **field name**        | Fan                    |
| --------------------- | ---------------------- |
| **requirement level** | optional               |
| **description**       | Mixing fan in chamber? |
| **format**            | logical                |
| **units**             |                        |

### Species

| **field name**        | Species                                                          |
| --------------------- | ---------------------------------------------------------------- |
| **requirement level** | optional                                                         |
| **description**       | Comma-separated list of dominant species at measurement location |
| **format**            | character                                                        |
| **units**             |                                                                  |

### Sensor depths

| **field name**        | Sensor\_Depths                                                      |
| --------------------- | ------------------------------------------------------------------- |
| **requirement level** | optional                                                            |
| **description**       | Comma-separated depths of solid-state sensors, gradient method only |
| **format**            | character                                                           |
| **units**             | cm                                                                  |

### Notes

| **field name**         | Notes                                                  |
| ---------------------- | ------------------------------------------------------ |
| **requirement\_level** | optional                                               |
| **description**        | Additional information about this measurement location |
| **format**             | character                                              |
| **units**              |                                                        |
