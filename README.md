# Shell-and-Tube Heat Exchanger (STHX) numerical model

This code presents a numerical model coded in Julia programming language to solve for the thermal and hydraulic performance of a shell-and-tube heat exchanger [[1]](#1). 

## Numerical model summary

- Newly developed correlations enables the model to solve for flow over bare, disc-finned, and cylindrical pin-finned tube banks. 
- The current version of the model incorporates U-shaped tubes. 
- Both internal and external flow streams utilize supercritical carbon dioxide as the working fluid. 
- The thermophysical properties of the working fluid are obtained using CoolProp and thus the flow streams can be modified to any fluid available on the CoolProp package (https://doi.org/10.1021/ie4033999) [[2]](#2). 
- Nickel-based superalloy, Haynes282, is used as the solid material in this version and can be modified to your preference. 
- The code writes the key geometric parameters and performance outputs to a CSV file titled "HXTestData.csv" located in the same directory as the Jupyter Notebook in your local device.

## Documentation and citation information

Further details of the flow correlations and its development can be found in the following journal article (will be posted upon acceptance) [[3]](#3): 
Insert article DOI

Further details of the STHX numerical model can be found in the following journal article (will be posted upon acceptance) [[4]](#4): 
Insert article DOI

If you find the code useful, I would highly appreciate it if you cite the code along with the published journal articles explaining the details of the model development (references [[1]](#1),[[3]](#3), and [[4]](#4)). 
The DOI for the code is: (will be posted upon publication)

## References
<a id="1">[1]</a> 
Insert code citation upon publication

<a id="2">[2]</a> 
Bell, I. H., Wronski, J., Quoilin, S., & Lemort, V. (2014). 
Pure and pseudo-pure fluid thermophysical property evaluation and the open-source thermophysical property library CoolProp. 
Industrial & engineering chemistry research, 53(6), 2498-2508. 
https://doi.org/10.1021/ie4033999

<a id="3">[3]</a> 
Insert article citation upon publication

<a id="4">[4]</a> 
Insert article citation upon publication
