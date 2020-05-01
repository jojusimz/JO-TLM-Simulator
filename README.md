# GEMINI: A TIME DOMAIN TLM ELECTROMAGNETIC FIELD SOLVER DEVELOPED IN C++

This repository hosts a C++ TLM electromagnetic field solver suitable for simulating E and H field interactions in prescribed 2D and 3D cubic geometries discretized with a uniform mesh. 

This software was developed to facilitate my PhD research. Through it I implemented formulations of novel PML algorithms and benchmarked these against existing published methods. I have now decided to release the source code as it may be useful to any researcher interested in simulating similar geometries or wanting to build on the existing work. 
The implementation and approach taken to mesh and solve are simple and can be easily understood my researchers familiar with the TLM/Finite difference methods. The novelty however is the stable PML algorithms implemented the details of which are published in my journal papers  (See reference list [1]-[5]).


## The TLM Method:

## How GEMINI Works: 

![image](https://user-images.githubusercontent.com/60849864/80803483-5087ce00-8baa-11ea-938f-0d0b2f270edc.png)

## Features:

## Source Code Features:

## Geometry Features:

## Getting Setup:
 
  ### Building GEMINI from source on Linux / Windows ( MSYS )
  
  Compilation Instructions
  
  1. **Checklist**
  
   * Msys terminal ( Mandatory for Windows )
   * g++ compiler ( Mandatory )
   * MATLAB or Python to run Analytic scripts on Results ( Mandatory )
  
  2.  **START** BASH (Linux) / MSYS shell ( Windows )
    
  3.  **NAVIGATE** to project folder and **CLONE** GEMINI repository to
  
      ```cd folder/to/clone-into/```
      
      ```git clone https://github.com/jojusimz/GEMINI.git```
  
  4.  **NAVIGATE** to GEMINI source code directory and **CREATE a results directory 
  
       ```cd src```
       
       ```mkdir GEMINI_results```
  
  5.  **BUILD** the source code to executable software 
    
      ``` make ```
      
  6.  **RUN** the executable
  
      ``` .\simulate_GEMINI ```
  
## Reference List featuring GEMINI:
1.	_J. Odeyemi, A. Vukovic, T. Benson, P. Sewell, “An improved PML implementation in the transmission line method,” IET 10th International Conference on Computational Electromagnetics, June 2019._ 

2.	_J. Odeyemi, A. Vukovic, T. Benson, P. Sewell, “Stretched-Coordinate PML in 2D TLM simulations,” IET Science, Measurement and Technology, vol.14, no.3, pp. 272-277, 2020._

3.  _J. Odeyemi, A. Vukovic, T. Benson, P. Sewell, “A complex domain mapping of the SCN for an effective PML implementation in TLM,” IEEE Open Journal of Antenna and Propagation, to be published DOI: 10.1109/OJAP.2020.2986293._

4.  _J. Odeyemi, C. Smartt, A. Vukovic, T. Benson, P. Sewell, “ PML Effectiveness in the Transmission Line Modelling Method for Radiation and Scattering Applications,”  European Conference on Antennas and Propagation, Copenhagen, 2020 (to be published)._

5.	_J. Odeyemi, M. Panitz, A. Vukovic, T. Benson, P. Sewell, “An Effective Stretched Coordinate TLM-PML Suitable for Analyzing Planar Periodic Structures,” IEEE Microwave and Wireless Components Letters (submitted and under review)._

