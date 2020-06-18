
Because of repository dependencies, to download this repository, do:
```
$ git clone --recursive https://github.com/UHVZ-CentralAmerica/Results.git
```

If `--recursive` is not added, the dependencies in Codes will not be downloaded.



1. "BinStacks"

    The files in this folder are weighted bin stack signals.
    For each bin, there are two files, representing the data stack and the synthetic stack when modeling against the bin's best-fit model.

    Each file is 2-column time series text file.
    The first column represent time relative to ScS peak, in second.
    The second column represent the amplitude relative to original ScS peak (before subtract).

    These files can be used to create Extended Data Fig. 6.

2. "TableData"

    Files in this folder are text files.
    The data are pulled from calculations.

3. "Codes"

    Selected primary C++ codes used for the seismic analysis part.
    Dependencies are: SAC, MariaDB, GMT, fftw3
