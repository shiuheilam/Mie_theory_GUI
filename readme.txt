Mie_theory Executable

1. Prerequisites for Deployment 

Verify that version 9.8 (R2020a) of the MATLAB Runtime is installed.   
If not, you can run the MATLAB Runtime installer.
To find its location, enter
  
    >>mcrinstaller
      
at the MATLAB prompt.
NOTE: You will need administrator rights to run the MATLAB Runtime installer. 

Alternatively, download and install the Windows version of the MATLAB Runtime for R2020a 
from the following link on the MathWorks website:

    https://www.mathworks.com/products/compiler/mcr/index.html
   
For more information about the MATLAB Runtime and the MATLAB Runtime installer, see 
"Distribute Applications" in the MATLAB Compiler documentation  
in the MathWorks Documentation Center.

2. Files to Deploy and Package

Files to Package for Standalone 
================================
-Mie_theory.exe
-MCRInstaller.exe 
    Note: if end users are unable to download the MATLAB Runtime using the
    instructions in the previous section, include it when building your 
    component by clicking the "Runtime included in package" link in the
    Deployment Tool.
-This readme file 



3. Definitions

For information on deployment terminology, go to
https://www.mathworks.com/help and select MATLAB Compiler >
Getting Started > About Application Deployment >
Deployment Product Terms in the MathWorks Documentation
Center.


4. Descriptions

Calculating the scattering spectrum of customized dielectric functions 
using the Mie theory. Resolving their electric dipole (E1), magnetic dipole 
(M1), electric quadrupole (E2) and magnetic quadrupole (M2) contributions. 
Constant function, Drude model, Drude-Lorentz model, Lorentz model with two
oscillators and data point import are available.

To import dielectric function data, enter a path of a .mat file containing 
the dielectric function. It should be given in two (n x 2) matrice named "Re"
and "Im", where the first row is the wavelength in nanometer, and the second
row is the real part or imaginary part of the dielectric function, 
respectively. An example, "PANI.mat" is provided.


5. Acknowledge

The GUI is written based on the Mie theory code provided by 2008 Eric Le Ru 
and Pablo Etchegoin.

Reference:
E. C. Le Ru and P. G. Etchegoin, Principles of Surface-Enhanced
Raman Spectroscopy and Related Plasmonic Effects
(Elsevier, Amsterdam, 2009).
