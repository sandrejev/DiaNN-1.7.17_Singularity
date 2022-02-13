Dia-NN singularity recipe
====================================================
Dia-NN - a universal software for data-independent acquisition (DIA) proteomics data processing by Demichev, Ralser and Lilley labs. In 2018

Table of Contents
=================

  * Using Dia-NN singularity image
    * [Download Dia-NN recipe from github](#singularity-download)
    * [Build Dia-NN image from recipe](#singularity-build)
    * [Run Dia-NN](#singularity-run)
    * 
<a name="singularity-download">Download Dia-NN recipe from github</a>
----------------------------------------------------
```console
git clone git@github.com:sandrejev/DiaNN-1.7.17_Singularity.git
```

<a name="singularity-build">Build Dia-NN image from recipe</a>
----------------------------------------------------
```console
sudo singularity build -F DiaNN.sif Singularity
```

<a name="singularity-run">Run Dia-NN</a>
----------------------------------------------------
To run Dia-NN from the Singularity image simply run the container followed by all arguments you wish to pass to Dia-NN. More information on how to run Dia-NN can be found [here](https://github.com/vdemichev/DiaNN)
```console
sudo singularity run DiaNN.sif --cfg diann_config.cfg
```