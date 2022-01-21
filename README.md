# Reference Evapotranspiration Estimation in Ege Region, Turkey

## Table of Content
* [Overview](#overview)
* [Motivation](#motivation)
* [Structure](#structure)
* [References](#references)

<img src="https://raw.githubusercontent.com/YZouzou/evapotranspiration/main/part_3/img/result_analysis.png" width="700" height="300">

## Overview
This repository contains a project conducted on weather data collected from stations in the Ege region in Turkey to estimate reference evapotranspiration using limited climatic variables.

## Motivation
Evapotranspiration is the total loss of water from land, constituted from evaporation and transpiration. Measuring evapotranspiration allows for efficient irrigation scheduling that provides the exact water requirements of the crops. However, measuring evapotranspiration directly is time consuming and not practical to be done on a regular basis. The Food and Agricultural Organization recommends the use of the Penman Monteith equation to estimate reference evapotranspiration (Eq. 1) [1]. Reference evapotranspiration is the evapotranspiration from a surface of previously determined properties (reference surface), which can then be adjusted to other types of surfaces.

<img src="https://render.githubusercontent.com/render/math?math=ET_0 = \frac{0.408 \Delta \cdot \left( R_n - G \right) + \gamma \cdot \frac{900}{T + 273} \cdot u_2 \cdot \left(e_s - e_a \right)}{\Delta + \gamma \cdot \left( 1 + 0.34 \cdot u_2 \right)} ">




The previous equation, however, requires several climatic measurements that may not always be available on site. Therefore, several equations to compute ET0 from a smaller set of climatic variables have been suggested [2]. With the emergence of machine learning (ML), numerous researches were conducted on estimating reference evapotranspiration from a subset of climatic variables using ML algorithms. The project presented here is a small part of a larger study on this subject, which is to be published in the future.

## Structure
The project is divided into three parts:
* **Part 1:** Reference evapotranspiration computation from raw climatic data using the Fao 56 PM equation (Eq. 1).
* **Part 2:** Exploratory data analysis of the climatic data.
* **Part 3:** Application of machine learning algorithms to estimate ET0 from limited climatic variables. This part also includes an analysis and commentary on the prediction results.

The notebooks used and saved data to a local machine, therefore, to run the codes, download this repository and define the relevant paths in each notebook. All notebooks have a *"Define paths"* section where the paths used in that notebook should be defined.

## References

[1] Allen, R. G., L. S. Pereira, Raes, D., and Smith, M., Crop evapotraspiration guidelines for computing crop water requirements. 1998.

[2] G. H. Hargreaves and Z. A. Samani, “Reference Crop Evapotranspiration From Temperature.,” American Society of Agricultural Engineers, pp. 96–99, 1985.