# FUMOD: Updated FUel MODels gridded dataset

This repository contains the fuel maps of fuel models for Portugal and the raw datasets used to develop them. 

**Package:** FUMOD

**Version:** V1

**Date:** December 2022

**Product:** Fuel Models Map

**Study area:** Mainland Portugal

**Properties:** Geotiff gridded datasets with pixel size of 100-m; UTM-29 projection

## Description
This package is built using ModelBuilder/ArcGis toolbox, developed to produce an updated Fuel Models Map (FMM), based on the overlap of several intermediate fuel models maps (SM) for a reference year. The updated FMM is obtained by running SM from 1 to 10. The algorithms developed to produce SM8 and SM9 are either confidential or rely on provisory data, respectively. Each SM is dependent on different datasets, all organized in a geodatabase. The FUMOD toolbox contains the SM toolsets, inside each there are the developed codes to geoprocess the models. Next figure guides the sequence of steps and datasets needed to produce the updated FMM. 


## Method overview

The flowchart below represents the proposed model (FUMOD) composed by a sequence of the 10 sub-models (SM) and eight datasets (labeled from A to H) to produce the updated fuel models map (FMM).

![workflow_v1](https://user-images.githubusercontent.com/117373204/210095096-28f13635-88f8-47c6-94e6-a526cf376ab4.png)

## Technical steps and considerations
1. Copy the toolbox FUMOD to your working folder.
2. Copy the input GEODATABASE to the previously created folder. It includes DATASETS (from A to H) the Industrial properties fuel maps (SM8) and the pre- main fire season burned areas for the reference years (SM9). The reference year is the year for which the fuel models map is being produced. This folder will be also used to save the OUTPUT geodatabase (see next point); the output database for each reference year and the updated Fuel Models Maps (FMM).
3. Create a new geodatabase (OUTPUT) where the output maps from running the sub-models 1 to 6 (SM) will be saved. Notice that sub-models SM8 and SM9 are not shown either because the first uses confidential data and the second used provisory data.
4. Define the Workspace in the Environment Settings of ArcMap, with the full path to the previously created database (point 2).
5. Some sub-models (SM5 and SM7) include two intermediate models; each begin with a number that indicates the order that should be run. These models are used to check for errors. The full model integrates the intermediate models.
6. Only the first three sub-models (SM1 to SM3) are static, i.e., they all are used in each reference year (In the study, from 2019 to 2022).
7. For example, SM4 (fuel models in burned areas) depends on time since last fire variable (TSLF) which corresponds to DATASET_C_year, where “year” ranges from 2019 to 2022.
8. Some SM have different output datasets that are used to traceline and check fore rrors. These are the SM5, SM7 and SM10.
9. For example, the SM5 outputs two intermediate datasets: 1) the map of fuel models in burned shrublands; and 2) an update of the previous map using SAVI spectral index from June of the reference year.
10. In the SM10 it is necessary to set a new workspace folder where the final FMM will be saved in the geotiff format.
11. SM10 produces the final updated FMM in the shrubland areas according to the classification of Atlantic versus Mediterranean types (DATASET_H) for the reference year


## Download large volume of files (e.g. geodatabase)
A large volume of files can be downloaded at once by using the [Download Directory](https://download-directory.github.io/) or [DownGit](https://downgit.github.io/). To download any folder simply paste the hyperlink to the folder you wish to download. For example, to download the submodels of 2021 from DownGit simply paste the path to the folder (https://github.com/anasa30/PT_FuelModels/tree/main/FUMOD/SubModelsOutputs/SubModels_2021.gdb) in the mainpage of [DownGit](https://downgit.github.io/); to download the same data from [Download Directory](https://download-directory.github.io/) paste the path to the precedent folder you wish to download (https://github.com/anasa30/PT_FuelModels/tree/main/FUMOD/SubModelsOutputs)


## Community Feedback
If you have any sugestion on how to improve the map of fuel models in Portugal or if you encounter any issue when downloading or using the dataset, please open a new [issue](https://github.com/anasa30/PT_FuelModels/issues).


## Frequency of data updates
The map of fuel models is updated once per year, before the starting of a new fire season in Portugal (around late spring). After an update, a new folder corresponding to the present year is created in [Fuel Models](https://github.com/anasa30/PT_FuelModels/tree/main/Fuel%20Models). The layers used to create the fuel map are also updated every year. If you wish to download past versions of submodels or any other layer used to create the fuel model map, please contact the authors at anasa30@gmail.com

## Reference
Sá, A.C.L., Benali, A., Aparicio, B.A., Bruni, C., Mota, C., Pereira, J.M.C. and Fernandes, P.M. A method to produce a flexible and customized fuel models dataset. MethodsX. Submitted (December 2022)


**Author contact:** anasa30@gmail.com
