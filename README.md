# IEA-15-240-RWT-Jacket
This reponsitory contains files that can be used in OpenFAST to simulate a 3-legged jacket structure in 50m water depth. These files make reference to (and therefore require) some of the files found in the IEA-15-240-RWT and IEA-15-240-RWT-Monopile folders of the IEA-25-240-RWT repository.

## Main dimensions
The 3-legged jacket model has the following main characteristics:
![Main Jacket Dimensions](https://github.com/mmrocze2/IEA-15-240-RWT-Jacket/blob/main/images/jacketdimensions.JPG?raw=true)

## Member sizes
The 3-legged jacket model has the following member sizes:
![Leg Member Dimensions](https://github.com/mmrocze2/IEA-15-240-RWT-Jacket/blob/main/images/legmembers.JPG?raw=true)
![Brace Member Dimensions](https://github.com/mmrocze2/IEA-15-240-RWT-Jacket/blob/main/images/bracemembers.JPG?raw=true)

## Interface elevation
The interface elevation between jacket and turbine has been increased to +30m relative to still water level (compared to +15m in the monopile model). This was considered to be more reprentative for a jacket foundation in 50m water depth.  

## Soil structure interaction
The jacket nodes at mudline are modeled with 1GN/m soil springs in the vertical translation direction, while the other degrees of freedem are fixed.

## Natural frequency
The natural frequency of the global model (turbine and jacket) was determined using a free-decay test in OpenFAST. The natural frequency was approximately 0.221 Hz, which falls outside the 1P and 3P frequency range of the IEA 15MW RWT.
