# Map of Fuel Models for Portugal

This repository contains the fuel maps of fuel models for Portugal and the raw datasets used to develop them. The generation of maps of fuel models in Portugal follows the methodology described in Sá et al. 2023 (DOI) and is summarized in the figure below.

![flowchart](https://user-images.githubusercontent.com/117373204/209812230-83abfc4d-a6cb-4f6e-9608-bc2955f29311.png)

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

A comprehensive description of the fuel models developed for Portugal with in situ photographies can be found [here](https://github.com/anasa30/PT_FuelModels/blob/main/Table_FM_description.pdf).

## Download the database file
The database file can be easily downloaded as a a geodatabase from GitHub by using Download Directory or DownGit, or by simply accessing to:
- https://download-directory.github.io/?url=https%3A%2F%2Fgithub.com%2Fanasa30%2FPT_FuelModels%2Ftree%2Fmain%2Fdatasets 
- https://downgit.github.io/#/home?url=https://github.com/anasa30/PT_FuelModels/tree/main/datasets/DATASETS.gdb

## Community Feedback
If you have any sugestion on how to improve the map of fuel models in Portugal or if you encounter any issue when downloading or using the dataset, please open a new [issue](https://github.com/anasa30/PT_FuelModels/issues).

## Frequency of data updates
The map of fuel models is updated once per year, before the starting of a new fire season in Portugal (around late spring). After an update, all the hyperlinks redirecting to the data download are also updated and older versions moved to [past versions](https://github.com/anasa30/PT_FuelModels/tree/main/past%20versions). The base layers that are used to generate the map of fuel models (e.g. land cover, national fire atlas, etc.) are also updated once per year around late spring, depending on the availability of updated data.

If you wish to download past versions you can use the [Download Directory](https://download-directory.github.io/) or [DownGit](https://downgit.github.io/) and paste de hyperlink to the folder you wish to download. For example, to download the data of 2021 from DownGit simply paste the path to the folder (https://github.com/anasa30/PT_FuelModels/tree/main/past%20versions/2021) in the mainpage of DownGit [DownGit](https://downgit.github.io/)

## Citation
Please use the following citation when refering to this dataset:
Sá, A.C.L., Benali, A., Bruni, C., Mota, C., Aparicio, B.A., Pereira, J.M.C., Fernandes, P.M. (subm.) A customized method to produce adaptable fuel models dataset.
