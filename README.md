# Grad_mix : GradMix for nuclei segmentation and classification in imbalanced pathology image datasets
by Tan Nhu Nhat Doan, Kyungeun Kim2, Boram Song, and Jin Tae Kwak

## Introduction
This repository is for our MICCAI 2022 paper [GradMix for nuclei segmentation and classification in imbalanced pathology image datasets]
(https://link.springer.com/chapter/10.1007/978-3-031-16434-7_17).

![Grad_mix](./data/grad_mix.png)
GradMix takes a pair of a major-class nucleus and a rare-class nucleus, creates a customized mixing mask, and combines them using the mask to generate a new rare-class nucleus. As it combines two nuclei,
GradMix considers both nuclei and the neighboring environment by using the customized mixing mask. This allows us to generate realistic rare-class nuclei with varying environments.
## Requirements
-   python 3.6.1
-   torch 1.1.0
-   torch-geometric 1.2.1
-   Other packages in requirements.txt

## Usage
Prerequisite: dataset images and cell/nuclei instance masks 
1. Clone the repository and set up the folders in the following structure:
```
