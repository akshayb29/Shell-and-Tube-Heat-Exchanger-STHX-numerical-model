# Shell-and-Tube Heat Exchanger (STHX) numerical model

This code presents a numerical model coded in Julia programming language to solve for the thermal and hydraulic performance of a shell-and-tube heat exchanger [[1]](#1). 

<p align="center">
  <img width="460" height="300" src="https://user-images.githubusercontent.com/57877963/116480097-90bd7300-a835-11eb-9150-f6dfdb0890ea.png">
</p>
<h4 align="center" style="margin-top: 0px;"><b>Figure 1.</b> Schematic of the counterflow shell-and-tube heat exchanger modelled in the numerical model</h4>


## Numerical model summary

- Newly developed correlations enable the model to solve for flow over bare, disc-finned, and cylindrical pin-finned tube banks. 
- The current version of the model incorporates U-shaped tubes. 
- Both internal and external flow streams utilize supercritical carbon dioxide as the working fluid. 
- The thermophysical properties of the working fluid are obtained using CoolProp and thus the flow streams can be modified to any fluid available on the CoolProp package (https://doi.org/10.1021/ie4033999) [[2]](#2). 
- Nickel-based superalloy, Haynes282, is used as the solid material in this version and can be modified to your preference. 
- The code writes the key geometric parameters and performance outputs to a CSV file titled "HXTestData.csv" located in the same directory as the Jupyter Notebook in your local device.

## Outputs from the code

Apart from the key performance parameters, the code outputs the front and top views of the temperature contours as shown in <b><i>Fig. 2</i></b>.

<p align="center">
  <img width="850" height="250" src="https://user-images.githubusercontent.com/57877963/117217168-d342fa80-adb5-11eb-9a33-03678743e4e0.png">
</p>
<p align="center">
  <img width="850" height="250" src="https://user-images.githubusercontent.com/57877963/117217226-e5249d80-adb5-11eb-8c0a-137129089f09.png">
</p>
<h4 align="center" style="margin-top: 0px;"><b>Figure 2.</b> Temperature contours of a sample STHX test case</h4>

The code also outputs the pressure profiles for both the external and internal flow streams as shown in <b><i>Fig. 3</i></b>.

<p align="center">
  <img width="850" height="350" src="https://user-images.githubusercontent.com/57877963/137968161-e3cd6cae-07ad-4f54-ac0c-4ed30cbb0c8e.png">
</p>
<p align="center">
  <img width="850" height="350" src="https://user-images.githubusercontent.com/57877963/137967381-b4ff6dd0-40c0-4636-a5a8-e8371f36e4cd.png">
</p>
<h4 align="center" style="margin-top: 0px;"><b>Figure 3.</b> (a) External and (b) Internal pressure profiles of a sample STHX test case</h4>

## Documentation and citation information

Further details of the flow correlations and its development can be found in the following journal article (will be posted upon acceptance) [[3]](#3): 
Insert article DOI

Further details of the STHX numerical model can be found in the following journal article (will be posted upon acceptance) [[4]](#4): 
Insert article DOI

If you find the code useful, I would highly appreciate it if you cite the code along with the published journal articles explaining the details of the model development (references [[1]](#1),[[3]](#3), and [[4]](#4)). 
The DOI for the code is: https://doi.org/10.5281/ZENODO.5117860.

## References

<a id="1">[1]</a> 
Krishna, A. B., Jin, K., Ayyaswamy, P. S., Catton, I., and Fisher, T. S. (2021).
Akshayb29/Shell-and-Tube-Heat-Exchanger-STHX-Numerical-Model: Shell-and-Tube Heat Exchanger Numerical Model.
https://doi.org/10.5281/ZENODO.5117860.

<a id="2">[2]</a> 
Bell, I. H., Wronski, J., Quoilin, S., & Lemort, V. (2014). 
Pure and pseudo-pure fluid thermophysical property evaluation and the open-source thermophysical property library CoolProp. 
Industrial & engineering chemistry research, 53(6), 2498-2508. 
https://doi.org/10.1021/ie4033999

<a id="3">[3]</a> 
Krishna, A. B., Jin, K., Ayyaswamy, P. S., Catton, I., and Fisher, T. S. (2021)
Modeling of supercritical CO2 shell-and-tube heat exchangers at extreme temperatures and pressures. Part 1: Correlation development.
Under review.

<a id="4">[4]</a> 
Modeling of supercritical CO2 shell-and-tube heat exchangers at extreme temperatures and pressures. Part 2: Heat exchanger numerical model.
Under Review.

## Funding

The information, data, or work presented herein was funded in part by the Advanced Research Projects Agency-Energy (ARPA-E), US Dept. of Energy, under Award Number DE-AR0001131, in collaboration with Honeywell Aerospace. The information, data, or work presented herein was funded in part by an agency of the United States Government. Neither the United States Government nor any agency thereof, nor any of their employees, makes any warranty, express or implied, or assumes any legal liability or responsibility for the accuracy, completeness, or usefulness of any information, apparatus, product, or process disclosed, or represents that its use would not infringe privately owned rights. Reference herein to any specific commercial product, process, or service by trade name, trademark, manufacturer, or otherwise does not necessarily constitute or imply its endorsement, recommendation, or favoring by the United States Government or any agency thereof. The views and opinions of authors expressed herein do not necessarily state or reflect those of the United States Government or any agency thereof.
