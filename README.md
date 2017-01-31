# ConvRadio
![badge-img](https://img.shields.io/badge/Made%20at-%23AstroHackWeek-8063d5.svg?style=flat)
Neural Networks with 21cm Radio Data
====================================

This package implements a neural network on visibility data (radio astronomy data sets).

This project was carried out at Astro Hack Week 2016 at the University of California Berkeley, in collaboration with Zaki Ali (PhD student @ Berkeley) 

Goal
====
The goal of this package is to determine bad antennas from interferometric data sets typically used in radio astronomy. 

Methodology
=====
The Hydrogen Epoch of Reionization Array (HERA) is a radio telescope dedicated to observing large scale structure during and prior to the epoch of reionization.  HERA is a second generation instrument which combines efforts and lessons learned from the Murchison Widefield Array (MWA) and the Donald C. Backer Precision Array for Probing the Epoch of Reionization (PAPER). The array is a large grid of 14 meter (42 ft) diameter non-tracking dishes packed into a hexagonal grid 300 m (900ft)  across. This substantial collecting area increase gives an order of magnitude more sensitivity than first generation instruments and be capable of robust statistical characterization and has the sensitivity to enable first images of large scale HI structure. (http://reionization.org/)

Radio telescope clusters like the HERA are not able to detect in real time if one of the antenna has 'gone bad', this can be understood only after a lot of data processing, which requires both time and resources. Furthermore as the data is cross corelated all of the recorded data is deemed unusable. We are using Deep Learning to predict in real time if any one of the antenna belonging to the cluster are 'bad'. 

We were inspired by the Kaggle competition where whale sounds were encoded into images and a convolution net was used for classification. We use a similar approach and encode the data into images and use a deep convolution neural network for classification and prediction.

Please refer to the (main.ipynb) jupeter notebook for the detailed methodology of the implementation and testing.

