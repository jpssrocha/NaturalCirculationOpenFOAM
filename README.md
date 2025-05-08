# OpenFOAM - Natural Circulation Loop

This case simulate a natural circulation loop implemented on top of the
BernardCell example from the heatTransfer tutorials on OpenFOAM, on the 
buoyantBoussinesqPimpleFoam solver.

It was changed to:

- Use the material properties from water (at `constant/transportProperties`)
- Have the geometry of a square circuit (set at `system/blockMeshDict`)
- To be isolated at all walls but at the top and bottom lids which are set to $T_1$ and $T_2$ (set at `0`)
- To have no turbulence modeling (set at `constant/turbulenceProperties`)
