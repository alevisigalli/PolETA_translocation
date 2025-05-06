# Pol η Translocation – Input and Output Files

This repository contains input and output files used in the molecular dynamics and enhanced sampling simulations of DNA translocation by polymerase η (Pol η). These data support the analyses presented in our study, including the definition of a multi-task collective variable (CV) and the reconstruction of the free energy landscape.

## Structure files (PDB)

The following structures correspond to the centroids of the most populated clusters obtained via k-medoids clustering of the MD trajectories:

- `Pre_translocation.pdb` – Centroid structure of the pre-translocation state  
- `Post_translocation.pdb` – Centroid structure of the post-translocation state  
- `Intermediate1.pdb` – Centroid structure of the first intermediate (INT1)  
- `Intermediate2.pdb` – Centroid structure of the second intermediate (INT2)  

## Input files

These files were used for the enhanced sampling simulations involving the 2D collective variable (multi-task CV):

- `plumed.dat` – Main PLUMED input file for enhanced sampling simulations  
- `plumed_descriptors.dat` – DNA•protein distances used as descriptors for enhanced sampling simulations  
- `plumed_rst.dat` – Restraint parameters to maintain hydrogen bonds between the DNA bases during the simulations  

## Output files

These are the output files generated from the enhanced sampling simulations with the 2D collective variable (CV):

- `COLVAR` – OPES parameters used for the enhanced sampling simulations  
- `DIST` – DNA•protein distances used as descriptors for the machine-learning CV calculated over the biased trajectory  
- `FES.dat` – Free energy surface (FES) derived from enhanced sampling simulations  
