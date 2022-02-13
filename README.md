Dia-NN singularity recipe
====================================================
DIA-NN - a universal software for data-independent acquisition (DIA) proteomics data processing by Demichev, Ralser and Lilley labs. In 2018

Table of Contents
=================

  * Using Dia-NN singularity image
    * [Build Singularity image from recipe](#singularity-build)
    * [Run container](#singularity-run)

<a name="singularity-build">Build Dia-NN image from recipe</a>
----------------------------------------------------
```console
sudo singularity build -F DiaNN.sif Singularity
```

<a name="singularity-run">Run DiaNN</a>
----------------------------------------------------
To run DiaNN from the Singularity image simply run the container followed by all arguments you wish to pass to Dia-NN. More information on how to run DiaNN can be found [here](https://github.com/vdemichev/DiaNN)
```console
sudo singularity run DiaNN.sif --cfg diann_config.cfg
```