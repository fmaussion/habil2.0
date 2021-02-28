# Paper 11: Testing the consistency between changes in simulated climate and Alpine glacier length over the past millennium

```{admonition} Citation
Goosse, H., Barriat, P.-Y., Dalaiden, Q., Klein, F., Marzeion, B., **Maussion, F.**, Pelucchi, P. and Vlug, A.: Testing the consistency between changes in simulated climate and Alpine glacier length over the past millennium, Clim. Past, 14(8), 1119–1133, [doi:10.5194/cp-14-1119-2018](https://doi.org/10.5194/cp-14-1119-2018), 2018.
```

Past glacier extents have been used as proxy measures of past climates for decades.
Glacier models can help to provide imperfect but quantitative 
information about the climate conditions (temperature, precipitation) that might have led the observed extents.

In this innovative study led by Hugues Goosse (paleoclimatologist at UC Louvain, Belgium), the idea
of using glaciers as "sensors" of  past climate variability is taken a step further: can glaciers also be 
used as a "validation metric" for past climate simulations?

We drove OGGM with a suite of centennial scale climate simulations on 71 glaciers in the European Alps.
The length fluctuations simulated by OGGM are then compared to directly to glacier length records, 
effectively evaluating the forcing climate models "from the glacier perspective".
The results are more sensitive to model choices (i.e. the glacier model adds a layer of uncertainty), 
but in the absence of available temperature records at the timescales studied here, this method allows
a new kind of model validation without the use of any inverse method.
Indeed, the uncertain step of converting proxies (such as tree 
rings or glacier length) back to the observable variable (such as temperature) is avoided here
thanks to the use of OGGM as a forward model.

This original application of OGGM rewarded the difficult task
of developing the model's ability to simulate past glacier lengths. Of course, 
this pilot study also opened new questions: there are now being investigated in a research project at UC Louvain
and led to a recent follow-up publication at the global scale {cite}`Parkes2020`, this time without 
involvement from the OGGM core team.

I contributed to this paper by providing support with OGGM. I also helped to interpret the glacier 
length changes in the analysis of the simulation results, and did a minor contribution to the writing.

[Link to the paper](https://doi.org/10.5194/cp-14-1119-2018) (open-access)
