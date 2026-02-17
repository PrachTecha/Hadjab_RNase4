# Hadjab RNase4 core analysis

This repository holds the core code for the main analysis and plotting for "Ribonuclease 4 Functions in Nociceptor-Mediated Nerve Homeostasis" paper.

## Citation
```
Feng, X., Zhang, K., Techameena, P., Quadros, R., Adori, C., Murtazina, M., Adameyko, I., Biagini, S., Bayramlik, O., Lallemend, F., Gurumurthy, C., Hadjab, S. (2026). 
Ribonuclease 4 Functions in Nociceptor-Mediated Nerve Homeostasis.
Nature Communications.
```

## Contents
The core analysis can be found in [Notebook](Notebook) folder. Notebook [#1](Notebook/01_Neurons_DRG.ipynb), [#2](Notebook/02_Neurons_TG.ipynb), [#3](Notebook/03_Neurons_SGN.ipynb), and [#4](Notebook/04_Neurons_hDRG.ipynb) are mainly for analyzing the expression profile of RNase4 in mouse DRG, TG, SGN, and human DRG respectively. Notebook [#5](Notebook/05_Kinetics.ipynb) extracted the expression dynymics of RNase4 upon injury throughout time. The identification of co-expressing genes with RNase4 was done in Notebook [#6](Notebook/06_coexpression.ipynb). The analysis of snRNA-seq comparing BafCreRNase4 and WT can be found in Notebook [#7](Notebook/07_ss3_rnase_mut.ipynb). Notebook [#8](Notebook/08_behavior.ipynb) and [#9](Notebook/09_img_analysis.ipynb) are holding the code for behavior and image analysis respectively.

## Dependencies
To reproduce the results, please use `conda` or `mamba` to install all the dependencies from [environment.yml](environment.yml) file using:

```sh
mamba env create -f environment.yml
mamba activate rnase4
```

## Data availability
The count matrix of Smart-seq3xpress (cKO-BR) can be downloaded from [here](https://doi.org/10.6084/m9.figshare.28391387), while the count matrix from 10x platform (cKO-PR) can be downloaded from [GSE318231](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE318231).