# Reference Evapotranspiration Estimation in Turkey

## Table of Content
* [Overview](#overview)


## Overview
This repository contains a study conducted on weather data collected from stations in Turkey to estimate reference evapotranspiration using limited climatic variables.

## Motivation
Evapotranspiration is the total loss of water from land, constituted from evaporation and transpiration. Measuring evapotranspiration allows for efficient irrigation scheduling that provides the exact water requirements of the crops. However, measuring evapotranspiration directly is time consuming and not practical to be done on a regular basis. The Food and Agricultural Organization recommends the use of the Penman Monteith equation to estimate reference evapotranspiration (Eq. 1). Reference evapotranspiration is the evapotranspiration from a surface of previously determined properties (reference surface), which can then be adjusted to other types of surfaces.

$$ ET_0 = \frac{0.408 \Delta \cdot \left( R_n - G \right) + \gamma \cdot \frac{900}{T + 273} \cdot u_2 \cdot \left(e_s - e_a \right)}{\Delta + \gamma \cdot \left( 1 + 0.34 \cdot u_2 \right)} $$

Where:

* $ET_0$ reference evapotranspiration ($mm \cdot day^{-1}$)
* $R_n$ net radiation ($MJ \cdot m^{-2} \cdot day^{-1}$)
* $G$ soil heat flux density ($MJ \cdot m^{-2} \cdot day^{-1}$)
* $T$ mean daily air temperature at 2 m height (°C) **calculated as the mean between max and min temperatures**
* $u_2$ wind speed at 2 m height ($m \cdot s^{-1}$)
* $e_s$ saturation vapour pressure ($kPa$)
* $e_a$ actual vapour pressure ($kPa$)
* $\Delta$ slope vapour pressure deficit ($kPa \cdot °C^{-1}$)
* $\gamma$ psychometric constant ($kPa \cdot °C^{-1}$)