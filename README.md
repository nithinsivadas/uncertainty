# Monte-carlo simulation of uncertainty in solar wind measurements
Uncertainty in measurement time of a system's input can lead to a misinterpretation of a system's response. Applying this in space physics, leads to an explanation of the polar-cap potential saturation as merely being a perception caused by uncertainty in solar wind measurements. 

If you use the code here, please cite as follows: 
Sivadas, N. (2021). Measurement uncertainty leads to non-linear bias in regression function (Version 1.0.0) [Computer software]. https://doi.org/10.5281/zenodo.5559102

## Contents
**Code1_Monte_Carlo_Simulation_of_Solar_Wind_Uncertainty.mlx**: contains the code that processes Data from data folder, runs a monte-carlo simulation of a solar wind error model, and plots outputs. 
The corresponding .html can be used to view the code and the results for those who do not have access to MATLAB 2021. 

**Code2_Analytical_derivation_of_time_uncertainty.mlx**: contains the code that carries out a numerical integration that reveals how uncertainty in the measurement times of an input variable can lead to bias in the regression function of the output given input. 
The corresponding .html can be used to view the code and the results for those who do not have access to MATLAB 2021. 

**Data.zip** contains the following data files: 

  The WIND spacecraft measurements of the solar wind parameters propagated to the bow shock: https://spdf.gsfc.nasa.gov/pub/data/omni/high_res_omni/sc_specific/.

  The polar cap index values from https://pcindex.org/archive. 

  The auroral electrojet indices were downloaded from the superMag database: https://supermag.jhuapl.edu/indices/. 


## Instructions
Both codes require MATLAB 2021 to run. 

To run Code1 successfully please do the followign: 
  1. Unzip Data.zip within the local repository itself. 
  2. In Code1_Monte_Carlo_Simulation_of_Solar_Wind_Uncertainty.mlx provide the correct path of the Data folder inside the variable "DataDir".

Code2 can be executed without any external input or data. 

## Acknowledgements

Code:

1) Stephen Lienhard (2021). Multivariate Lognormal Simulation with Correlation (https://www.mathworks.com/matlabcentral/fileexchange/6426-multivariate-lognormal-simulation-with-correlation), MATLAB Central File Exchange. Retrieved October 7, 2021.

2) Zdravko Botev (2021). kernel density estimation (https://www.mathworks.com/matlabcentral/fileexchange/17204-kernel-density-estimation), MATLAB Central File Exchange. Retrieved October 7, 2021.

Data:

3) We thank GSFC/SPDF OMNIWeb service for the WIND spacecraft measurements. The WIND spacecraft measurements of the solar wind propagated to the bow shock can be accessed from https://spdf.gsfc.nasa.gov/pub/data/omni/high_res_omni/sc_specific/. 

4) The polar cap index values PCN and PCS were downloaded from https://pcindex.org/archive. We thank Dr. Oleg Troshichev of the Arctic and Antarctic Research Institute for this data (https://pcindex.org/contacts). 

5) The auroral electrojet indices were downloaded from the SuperMAG database https://supermag.jhuapl.edu/indices/. For this we gratefully acknowledge the SuperMAG collaborators (https://supermag.jhuapl.edu/info/?page=acknowledgement). 
