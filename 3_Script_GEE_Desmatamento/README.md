
<!-- GETTING STARTED -->
## Getting Started

This is an example of how setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

All necessary prerequisites are already installed in docker container

### Usage

1. Get access for Google Earth Engine (GEE) at [signup](https://earthengine.google.com/signup/)
2. Inside the container previously created, run this command to authenticate your account:
```sh
earthengine authenticate
```
3. (Optional if want to regenerate table of alerts) First, download shapefile alerts from mapbiomas in https://plataforma.alerta.mapbiomas.org/downloads. Copy the shapefile files to **OLACEFS_DAM/3_Script_GEE_Desmatamento/EarthEngine** and run:
```sh
python shp_file.py
```
5. After that, in the same folder, run:
```sh
python earth_engine.py
```

<!-- Examples of Downloaded Images -->
## Examples of Downloaded Images

Example of a deforestation alert SAR images extract from the mapbiomas webset, with a temporal resolution of 3 months.


![](https://github.com/edemir-matcomp/OLACEFS_DAM/blob/master/3_Script_GEE_Desmatamento/mapbiomas_example.png)


<!-- References -->
## References



_For more examples, please refer to the Google Earth Engine [Documentation](https://developers.google.com/earth-engine)


