
The codes in this folder are selected from the (long) seismic analysis process.

1. 0_subtractData.cpp

    This file first create the S and ScS empirical source wavelet from data by stacking (event by event).
    Then stretch/shrink the ScS ESW to S ESW (event by event).
    Finally subtract the modified ScS ESW from records from each event.


2. 0_subtractModels.cpp

    This file do the same as "0_subtractData.cpp", but this time, on synthetics.
    Multi-threading are needed because there are so many models.


3. 1_Binning.cpp

    This code do the geographic binning.
    

4. 2_subtractBinStack.cpp

    This file is in charge of the modeling process.
    For each bin, each model, a data stack and a synthetic stack are calculated.
    Then the two stacks are compared using the function defined in "CalculateCQ.hpp".


5. 3_Figure2_Subtract.cpp

    This file call the GMT package, which will plot Figure 2 in the paper.
    

6. CPP-Library-Headers

    This folder contains all the functions needed for this project. Most heavy liftings happen here.

