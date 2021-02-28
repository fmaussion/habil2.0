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

But this alone won't guarantee that OGGM continues to be useful in the future.
In the following, I briefly discuss my personal opinions about the directions that the OGGM project might follow.
What other research groups will do with OGGM is not under my control, and I'm sure that I'll be up for some surprises.

**Surface mass balance and model calibration**

One of the major changes in the past few years has been the publication of geodetic mass balance estimates at the 
regional and (very soon) global scale. We now have a mass balance estimate for almost every single glacier of the world.
This is a tremendous opportunity for glacier models, opening new avenues of research based on these observations. 
It will raise very important questions with respect to model calibration and validation (since all models will likely 
be matching the same reference products during the observational period), and with respect to the added value of 
physical parameterisations versus 
parameter calibration (since out-of-sample validation will be more difficult, how do we estimate added value?).

With OGGM, we are now getting ready for these new products (albeit a bit late). In a recently started PhD project (led by 
Lilian Schuster), we attempt to address the question of the added value of physical complexity in mass balance models
by implementing a suite of parameterizations of varying complexity. We will include combinations of surface processes
(refreezing, snow cover properties, debris cover...) in order to study the impact of these model physics on glacier projections. 
This project will provide a new generation of mass balance models to OGGM users and, hopefully, open the door for an 
automated and systematic procedure to deal with model uncertainties.

**Ice dynamics and distributed vs flowline approaches**

A new generation of models currently in development are aiming for distributed (2D/3D) modelling of surface mass balance
and ice dynamics. I am aware of at least three independent efforts: Johannes 
Fürst (EU Starting grant at Uni Erlangen), Harry Zekollary (TU Delft / ETH Zürich), and Bert Wouters / Jordi Bolibar
(Universiteit Utrecht). Distributed approaches are more elegant, less parameterized, and physically more sensible than
the current approach used by OGGM. I welcome these new developments, and the OGGM framework will
be ready to provide boundary conditions for these models if they need them (for example, OGGM will be used to provide
some ot the products delivered with the future version of the RGI, and we will make sure to address the new needs of these
projects).

I, personally, still believe that OGGM's flowline model will still be very useful in the future. Included in OGGM
only a few years ago, it allowed the representation of much more realistic dynamic feedbacks than parameterized or
"delta h" approaches. It will certainly be the subject of scientific debate in the near future, but I believe that the quality
of our observations, boundary conditions, and estimates of ice thickness will not allow to use the 
full potential of distributed modelling (at least not at the global scale).

Personally (and I might be wrong), I am putting most of my thoughts and energy on improving our statistical  
methods for uncertainty estimation. The Bayesian model ensemble strategies and the inverse models we are implementing will be 
very hungry in computational resources, and the speed and robustness of the flowline model will be a central requirement
for these applications. Furthermore, I also think that one of the largest remaining issue of global models (frontal ablation)
will be more likely to be addressed by flowline than distributed models at first.

**Frontal ablation**

46% of the area of the world's mountain glaciers belong to water terminating glaciers (marine-, shelf-, and lake-terminating).
As discussed in this thesis, frontal ablations strongly impacts the dynamic response of glaciers in many ways, and raises 
new challenges for model calibration. I believe that frontal ablation is the most important challenge that the global-scale 
glacier modelling community needs to address.

It is a very difficult problem, requiring new collaborations with ice-sheet and ocean scientists, modelling  and remote
sensing specialists. Over the past few years, we have opened the door to such collaborations and hope that OGGM will 
be useful for such endeavors.

**Inverse methods for ice thickness estimation**

One of the main assumptions behind


**Modular framework and model structure**

