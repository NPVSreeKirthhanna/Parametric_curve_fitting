# Parametric Curve Fitting

## Final Estimated Parameters

 θ (radians) = 0.488133
 θ (degrees) = 27.967978
 M = 0.0205016
 X = 54.66619

## Final Latex Expression

\left(t*\cos(0.488133)-e^{0.020502\left|t\right|}\cdot\sin(0.3t)\sin(0.488133)+54.666195,42+t*\sin(0.488133)+e^{0.020502\left|t\right|}\cdot\sin(0.3t)\cos(0.488133)\right)

Domain: 6 ≤ t ≤ 60



## Approach

1. Loaded given xy_data.csv.
2. Since parameter 't' was not provided, reconstructed t using arc-length based reparameterization and mapped it into [6,60].
3. Implemented the given parametric model in Python.
4. Defined L1 error metric exactly as assignment scoring criteria.
5. Performed bounded parameter optimization:
   - Differential Evolution for global search within allowed ranges.
   - Nelder Mead local refinement for final precision.
6. Selected parameters which minimized L1 error.
7. Verified visually using Desmos.

L1 loss (observed): 37923.93  
L1 approx: 13932.83


## Visualization (Desmos)

Desmos Link: *(https://www.desmos.com/calculator/vihqiawf8q)*


