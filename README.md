# Shell-and-Tube Heat Exchanger (STHX) numerical model

This code presents a numerical model to solve for the thermal and hydraulic performance of a shell-and-tube heat exchanger. Newly developed correlations makes the model capable of solving for flow over bare, disc-finned, and cylindrical pin-finned tube banks. The current version of the model incorporates U-shaped tubes. Both internal and external flow streams have supercritical carbon dioxide as the working fluid. The thermophysical properties of the working fluid is obtained using CoolProp and thus the flow streams can be modified to any fluid available on the CoolProp package (https://doi.org/10.1021/ie4033999) [1]. Nickel-based superalloy, Haynes282, is used as the solid material in this version and can be modified to your preference. 

Further details of the flow correlations and its development can be found in the following journal article (will be posted upon acceptance) [2]:
Insert article DOI

Further details of the STHX numerical model can be found in the following journal article (will be posted upon acceptance) [3]:
Insert article DOI

If you find the code useful, I would highly appreciate it if you cite it along with the published journal articles explaining the details of the model development. The DOI for the code is: (will be posted upon publication)

### References
[1] Bell, I. H., Wronski, J., Quoilin, S., & Lemort, V. (2014). Pure and pseudo-pure fluid thermophysical property evaluation and the open-source thermophysical property library CoolProp. Industrial & engineering chemistry research, 53(6), 2498-2508.
[2] Insert article citation upon publication
[3] Insert article citation upon publication
