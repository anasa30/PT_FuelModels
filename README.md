# FUMOD: Updated FUel MODels gridded dataset

This repository contains the fuel maps of fuel models for Portugal and the raw datasets used to develop them. 

Package: FUMOD
Version: V1
Data: December 2022
Product: Fuel Models Map
Study area: Mainland Portugal
Properties: Geotiff gridded datasets with pixel size of 100-m; UTM-29 projection


The generation of maps of fuel models in Portugal follows the methodology described in Sá et al. 2023 (DOI) and is summarized in the figure below.

![workflow_v1](https://user-images.githubusercontent.com/117373204/210095096-28f13635-88f8-47c6-94e6-a526cf376ab4.png)

The dataset contains the layers identified with letters in the figure, namely:
- DATASET_A: Land cover (cos2018)
- DATASET_B: Corine land cover (2018)
- DATASET_C: National fire atlas
- DATASET_D: Satellite vegetation indexes
- DATASET_E: Copernicus tree density cover (2018)
- DATASET_F: Fieldwork
- DATASET_G: Land cover and fuel management operations
- DATASET_H: Bioclimatic and lithological classification
- Final map of fuel models

A comprehensive description of the fuel models developed for Portugal with in situ photographies can be found [here](https://github.com/anasa30/PT_FuelModels/blob/main/Documents/Table_FM_description.pdf).

## Download the database file
The database file can be easily downloaded as a a geodatabase from GitHub by using Download Directory or DownGit, or by simply accessing to:
- https://download-directory.github.io/?url=https%3A%2F%2Fgithub.com%2Fanasa30%2FPT_FuelModels%2Ftree%2Fmain%2FFUMOD%2FDatasets
- https://downgit.github.io/#/home?url=https://github.com/anasa30/PT_FuelModels/tree/main/FUMOD/Datasets/DATASET.gdb

## Community Feedback
If you have any sugestion on how to improve the map of fuel models in Portugal or if you encounter any issue when downloading or using the dataset, please open a new [issue](https://github.com/anasa30/PT_FuelModels/issues).

## Frequency of data updates
The map of fuel models is updated once per year, before the starting of a new fire season in Portugal (around late spring). After an update, all the hyperlinks redirecting to the data download are also updated and older versions moved to the corresponding folder in [Fuel Models](https://github.com/anasa30/PT_FuelModels/tree/main/Fuel%20Models). The base layers that are used to generate the map of fuel models (e.g. land cover, national fire atlas, etc.) are available at the [Models](https://github.com/anasa30/PT_FuelModels/tree/main/FUMOD/Models) folder.

If you wish to download past versions you can use the [Download Directory](https://download-directory.github.io/) or [DownGit](https://downgit.github.io/) and paste de hyperlink to the folder you wish to download. For example, to download the models of 2021 from DownGit simply paste the path to the folder (https://github.com/anasa30/PT_FuelModels/tree/main/FUMOD/Models/SubModels_2021.gdb) in the mainpage of DownGit [DownGit](https://downgit.github.io/)

## Citation
Please use the following citation when refering to this dataset:
Sá, A.C.L., Benali, A., Bruni, C., Mota, C., Aparicio, B.A., Pereira, J.M.C., Fernandes, P.M. (subm.) A method to produce a flexible and customized fuel models dataset
