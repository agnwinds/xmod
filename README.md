## Description of Extra Models for use with the MCRT Code Python

Python contains a number of simple models, e.g a BB spectrum, to simulate
the radiation generated by external radiation sources such as a central star
or disk.  In addition, however, one can read in models that provide a more accurate
representation of these data sources.

The number of possible models can be large, and that can be fairly voluminous in 
in terms of the amount of space they require.  Rather than incorporaate them into
the main Python data repository, they are offered as a separate repository.


### Disk/Stellar Models

To use put data/masterfile.ls in your parameter file, e.g. xmod/model_kurucz91. 

Users should be aware that some of the stellar spectra are calculated using stellar 
atmospheres that were not very sophisticated, and better models may be available today.

* kurucz91.ls: Kurucz model atmospheres. Grid goes to 50,000K and log(g) = 5
* kurucz_d14.ls: Kurucz model atmospheres run through Synspec. Grid goes to 50,000K and log(g) = 5
* tlusty_d14.ls: TLUSTY model atmospheres. Grid goes to 130,000K and log(g) = 9
* kur_tlusty_hybrid.ls: Kurucz + TLUSTY hybrid model atmosphere's. Current benchmark SA grid for accretion disk.
* disk06.ls: Disk 06 models
* lejeune.ls: A set of stellar models from lejeune.  Not yet used. Their advantage is that they go further into the IR than kurucz

**Folders:** Masterfiles have same names as folders, except for the d14 and kur_tlusty_hybrid models which are contained in disk14 folder.
