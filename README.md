# GSSA-of-QDs
Matlab program for the application of the Generalized Single Slice Approach for simulating TEM images of QDs

AUTHOR: Lionel C Gontard 2020
REFERENCE:  
Gontard, L. C., Barroso-Bogeat, A., Dunin-Borkowski, R. E., & Calvino, J. J. (2018). A single slice approach for simulating two-beam electron diffraction of nanocrystals. Ultramicroscopy, 195, 171-188. https://doi.org/10.1016/j.ultramic.2018.09.004

FILES: 
GSSA.m is the main function
CTF.m  contrast transfer function
MODELS:
Rx component x of the displacement field
Ry component y of the displacement field
Rz component z of the displacement field
composition  model of the structure and the distirbution of Indium of an In(Ga)As quantum dot (QD).

The main function is GSSA.m that loads the models, performs calculations and also the visualization.
GSSA.m  calls to the function CTF.m which models the Contrast Transfer Function of a transmission electron microscope. 

USAGE OF THE FUNCTION GSSA.m:

DEFINITIONS:
%def defocus value of the objective lens
%DF_BF=10 for simulation of DF TEM image 
%DF_BF=01 for simulation of BF TEM image
%hkl indexes of reflection, e.g., 200 or 222
%Cs spherical aberration in mm
%k value for adjusting the F200 in BF

EXAMPLES:
Example 1: GSSA(55,01,200,1,0) calculates a BF image of 200 with a defocus of 55 nm and spherical aberration of 1 mm
Example 2: GSSA(-35,10,202,1,0) calculates a DF image of 202 with a defocus of -35 nm and spherical aberration of 1 mm
