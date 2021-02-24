# Paper 04: Impact of frontal ablation on the ice thickness estimation of marine-terminating glaciers in Alaska

```{admonition} Citation
Recinos, B., **Maussion, F.**, Rothenpieler, T. and Marzeion, B.: Impact of frontal ablation on the ice thickness estimation of marine-terminating glaciers in Alaska, Cryosph., 13(10), 2657–2672, [doi:10.5194/tc-13-2657-2019](https://doi.org/10.5194/tc-13-2657-2019), 2019.
```

This paper is the first of two papers led by Beatriz Recinos during her PhD Thesis ([link to the PDF](https://media.suub.uni-bremen.de/handle/elib/4637)).
In this work, we studied the influence of frontal ablation on the OGGM ice thickness estimation of marine-terminating glaciers.

OGGM's ice thickness model belongs to the type of "mass-conservation models", which rely on the computation of an ice flux through the glacier. Using this flux value, surface properties and the physics of ice flow, OGGM estimates the ice thickness along the flowline. In this paper, we discuss (for the first time in a regional modelling context) the importance of frontal ablation on the estimation of this mass flux and therefore on the volume of marine-terminating glaciers.

We implemented an existing parameterization {cite}`Oerlemans2005b` in OGGM to estimate frontal ablation flux from three simple variables (ice thickness, water depth, and glacier width) and one tuning parameter. Relying on the assumption that this flux needs to be equal to the flux by ice deformation at the terminus, we could solve for the ice thickness at the terminus and  provide this new boundary condition to the mass-balance model calibration routine.

This publication led to the operational implementation of this parameterization in OGGM, and paved the way for further investigation. While we still relied on an external frontal ablation dataset to calibrate model parameters, in a follow-up study (Recinos et al, in review for J. Glac.), we could make use of observations of ice velocity to better calibrate the model.

I contributed to this paper in several ways: I provided technical support to Beatriz in the implementation of the new parameterization, and I helped with the OGGM integration. I also provided support and supervision during the paper writing and duing the review process.

[Link to the paper](https://doi.org/10.5194/tc-13-2657-2019) (open access)
