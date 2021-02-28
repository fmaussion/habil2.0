(content:outlook)=
# Perspectives for the OGGM project

The OGGM global glacier modelling framework is now well established in the landscape of 
glacier models. It is the only global-scale model that is open source, which has
attracted many users and contributors from external institutions. It forms the basis of this thesis, 
several research publications and PhD theses, and is the backbone of current research projects and 
proposals.

Very few global models reach a similar level of physical complexity. At present, only the model by
Huss and Hock (2015) {cite}`Huss2015` and Zekollari et al. (2019) {cite}`Zekollari2019` aims for similar complexity and has
been a driver for many advances in global scale glaciology in recent years. A new model (PyGEM, {cite}`Rounce2020`) 
became open source recently: focussed on simulating the surface mass balance and its uncertainty with Bayesian
methods, PyGEM is arguably one of the best mass balance models available. Thanks to a recent collaboration, PyGEM is now 
relying on OGGM for its pre-processing and ice dynamics components, making it the first external application 
of OGGM's "framework" structure: PyGEM remains independent while still using some elements
of the OGGM workflow, opening the way for future model intercomparison studies. 

Additional unpublished models are currently in development (see below), but OGGM is still probably one of the most 
modern and complete global glacier models available. It is unprecedented in terms of open development, modular 
structure and testing practices.

This alone won't guarantee that OGGM continues to be useful in the future.

In the following, I briefly discuss my personal opinions about the directions that the OGGM project might follow.
What other research groups will do with OGGM is not under my control, and I'm sure that I'll be up for some surprises.

**Surface mass balance and model calibration**

One of the major recent advances for global glacier studies has been the publication of geodetic mass balance estimates at the 
regional and (very soon) global scale. We now have a mass balance estimate for almost every single glacier of the world.
This is a tremendous opportunity for glacier models, opening new avenues of research. 
It will raise very important questions with respect to model calibration and validation (since all models will 
be matching the same reference products, how to compare their performance?), and with respect to the added value of 
physical parameterisations (since out-of-sample validation will be more difficult, how do we estimate added value?).

We are now preparing OGGM to ingest these new products. In a recently started PhD project 
(Lilian Schuster), we attempt to address the question of the added value of physical processes in mass balance models
by implementing a suite of parameterizations of varying complexity. We will include combinations of surface processes
(refreezing, snow cover properties, debris cover...) and study the impact of these model physics on glacier projections. 
This project will provide a new generation of mass balance models to the OGGM framework and, hopefully, open the door for an 
automated and systematic model uncertainty quantification.

**Ice dynamics: distributed and flowline approaches**

A new generation of models currently in development are aiming for distributed (2D/3D) modelling of surface mass balance
and ice dynamics. I am aware of at least three independent efforts: Johannes 
Fürst (EU Starting grant at Universität Erlangen), Harry Zekollary (TU Delft / ETH Zürich), and Bert Wouters / Jordi Bolibar
(Universiteit Utrecht). Distributed approaches are more elegant, less parameterized, and physically more sensible than
the current approach used by OGGM. I welcome these new developments, and the OGGM framework will
be ready to provide boundary conditions for these models if they need them (for example, OGGM will be used to provide
the glacier attributes delivered with the future version of the RGI, and we will make sure to address the needs of these
new projects as well).

I, personally, still believe that OGGM's flowline model will continue to be useful in the future. Included in OGGM
only a few years ago, it allowed the representation of much more realistic dynamic feedbacks than parameterized or
"delta h" approaches. This will certainly be the subject of scientific debate in the near future, 
but I believe that the quality of our observations, boundary conditions, and estimates of ice thickness will not yet 
allow to use the full potential of distributed modelling (at least not at the global scale), and the use of distributed
models will come with its own set of challenges and uncertainties.

Personally (and I might be mistaken), I am investing most of my thoughts and energy on improving OGGM as it is now,
in particular in the domain of statistical methods for uncertainty estimation. The Bayesian model ensemble strategies 
and the inverse models we are planning to use will be very hungry in computational resources, and the efficiency and 
robustness of the flowline model will be a central requirement for these new applications. 
Furthermore, I also think that one of the largest remaining challenges for global models (frontal ablation)
will be more likely to be tackled by flowline than distributed models, at least in a first step.

**Frontal ablation**

46% of the area of the world's mountain glaciers eventually flows directly into water (marine-, shelf-, and 
lake-terminating glaciers). As discussed in this thesis, frontal ablation strongly impacts the dynamic response of 
glaciers, and raises new challenges for model calibration and ice thickness estimation. 
I believe that frontal ablation is the most important source of biases in current global-scale glacie change projections, 
and a problem that the glacier modelling community needs to address urgently.

It is a very difficult problem, requiring collaborations with ice-sheet and ocean experts, modelling  and remote
sensing specialists. Over the past few years, we have opened the door to such collaborations by implementing parameterizations
in the framework. Because of lack of testing in real-world global applications they are, however, switched off 
per default at the moment. With these first building blocks in place, we hope that OGGM will 
be useful to the research groups that are interested in such an endeavor.

**Inverse methods for ice thickness estimation**

The mass-conservation method used by OGGM to estimate the ice thickness relies on an important and problematic 
assumption: that glaciers are in dynamical equilibrium with a given mass-balance profile. To release this 
assumption, I have worked with two master students on a completely new approach based on cost optimisation:
[COMBINE](https://github.com/OGGM/combine) (COst Minimization Bed INvErsion model for glaciers and ice caps).

This new approach relies on the OGGM distributed or flowline model as a forward operator, and uses automatic 
differentiation to iteratively minimize the mismatch with observable variables such as surface height or 
ice thickness observations. COMBINE will allow to ingest much more information into the inversion process,
such as past climate data and past glacier outlines, hereby releasing the equilibrium assumption. It will 
also lead to improved present day glacier states and reduce the "initialisation shock" that happens in the 
first few years of an OGGM simulation. 

A research project proposal based on COMBINE is currently in the making.
