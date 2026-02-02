# DEM imputation

[Konstantin A. Maslov](https://people.utwente.nl/k.a.maslov), [Thomas Schellenberger](https://www.mn.uio.no/geo/english/people/aca/geohyd/thosche/), [Claudio Persello](https://people.utwente.nl/c.persello), [Alfred Stein](https://people.utwente.nl/a.stein)

<br/>

The repository implements DEM imputation logic used for GlaUnTI glacier surface mass balance model (see [https://github.com/konstantin-a-maslov/glaunti](https://github.com/konstantin-a-maslov/glaunti)). 
The algorithm imputes [Hugonnet et al. (2021)](https://doi.org/10.1038/s41586-021-03436-z) elevations based on Cop30DEM (or any other DEM) features using an approximation of the RBF kernel regression. 

<br/>


## Getting started

We recommend using the [Anaconda](https://www.anaconda.com/download) or [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/) Python distributions. 
After installing one of them, one can use the `conda` package manager to install the required libraries in a new environment called `demimputation` and activate it by running
```
conda env create -f env.yml
conda activate demimputation
```

<br/>

After the installation is complete, data for imputation should be prepared. 
For brevity, we uploaded only a subset of three glaciers presented in the original study to this repository. 
The data format can be copied from there. 
Make sure to reproject Cop30DEM to the Hugonnet et al. grid before imputation.

<br/>

To calibrate and run the imputation models, please follow the instructions in [`main.ipynb`](main.ipynb). 


## License

This software is licensed under the [GNU General Public License v2](LICENSE).


## Citing

To cite the repository, please use the following bib entry. 
```
@article{
  ...
}
```
