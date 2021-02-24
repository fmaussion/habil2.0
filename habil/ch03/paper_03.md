# Paper 03: A consensus estimate for the ice thickness distribution of all glaciers on Earth

```{admonition} Citation
Farinotti, D., Huss, M., Fürst, J. J., Landmann, J., Machguth, H., **Maussion, F.** and Pandit, A.: A consensus estimate for the ice thickness distribution of all glaciers on Earth, Nat. Geosci., 12(3), 168–173, [doi:10.1038/s41561-019-0300-3](https://doi.org/10.1038/s41561-019-0300-3), 2019.
```

This paper is the second contribution of the IACS working group on Ice thickness estimation. After the completion of ITMIX experiment phase I ([Paper 02](paper_02)), all modelling groups able to simulate a large number of glaciers (> 1000) were invited to contribute to the first global, multi-model estimate of the distributed ice thickness of the world's glaciers. This was a very timely endeavor, for various reasons:

- the only previous global estimate of distributed glacier ice thickness {cite}`Huss2012` was based on a single model and on an older version of the RGI glacier inventory
- other glacier volume estimates (i.e. without distributed thickness) were based on scaling relationships, and were widely different from another {cite}`Radic2010,Marzeion2012,Grinsted2013`
- there was an increasing demand from the community for a freely available, RGI based ice thickness product.

Similarly to ITMIX phase I, the call for participation was open to anyone, and the boundary conditions (topography, ice thickness observations) were standardized and provided to all participants. Importantly, the modellers were asked to conduct a cross-validation experiment, in which the training and validation samples were rotated to allow an independent model validation. The final weight given to each model contribution would depend on its out-of-sample validation score.

The main outcome of this study certainly is the openly available ice-thickness dataset, which is now advertised as an extended product of the RGI version 6. Similarly to ITMIX phase I, the study also reveals large discrepancies between models, indicating that further improvements will be necessary (I will discuss this point in [chapter 07](content:outlook)).

I contributed to this paper in several ways:
- OGGM was one of the five models contributing to the final product. This contribution led to several improvements in the OGGM codebase itself.
- I argued in favor of runnning a cross-validation experiment and helped designing it.
- I also participated with an additional model contribution (a simple statistical model), which was later discarded because it was previously unpublished.  
- I participated in the analysis of the results, and, to a smaller extent, to the writing of the paper.

[Link to the paper](https://doi.org/10.1038/s41561-019-0300-3) (non open-access)

[Link to the ice thickness dataset](https://doi.org/10.3929/ethz-b-000315707) (open-access)
