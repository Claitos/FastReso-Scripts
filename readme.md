## Usefull Scripts for handling FastReso resonance lists



Contains scrpits for mainly three different functionality:


- parser.py conatins a parser to manipulate the data inside the Azhydro resonance data files for the FastReso package. It saves the data inside two pandas dataframes for manipulation and allows to save them again to a file which has the exact same structure as the original data file.
The parser also has a built in functionality to score the resonances in the data file regarding their contribution to a certain particle spectra. The default is for pions.
- pdg_lib.py features a libary to call the api of the PDG to get uncertainties for values of the resonances in the data files. Currently supported are uncertainties for Masses, Decay widths and Branching ratios of the resonances and their decay modes.
- It also contains a script to sample values of the resonance parameters according to the parameter uncertainties. It features functionality of changing uncertainties manually to do an edge study and features rejection sampling and a MCMC sampler. (sampler_lib.py) 
- This repository also provides a small script the reverse the output data files. This reversed file can be needed for FastReso to run. (reverser.py)


The notebooks explain and use the functionalities that are implemented in the scripts.

This repository is mainly used in my ongoing master thesis regarding the influence of resonance parameter uncertainties on the low transverse momentum pion excess.