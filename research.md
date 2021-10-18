---
layout: page
title: Research
---

<h2>First Light And Reionisation Simulations (<span style="font-variant: small-caps;">Flares</span>)</h2>
The <span style="font-variant: small-caps;">Flare</span> simulations are a suite of high-resolution hydrodynamic simulations of galaxy formation and evolution using the <span style="font-variant: small-caps;">Eagle</span> physics. The suite consists 40 zoom resimulations of spherical regions selected at z=5 from a 3.2 cGpc a side, parent dark matter-only box. We select a range of overdensities in order to study the environmental effect on high-redshift galaxy evolution. We also combine these resimulations in order to produce composite distribution functions, signficantly extending the dynamic range of the model over smaller volume, periodic simulations. The introductory papers can be found at [Lovell et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021MNRAS.500.2127L/abstract) and [Vijayan et al. (2021)](https://ui.adsabs.harvard.edu/abs/2021MNRAS.501.3289V/abstract).  

<p align = "center">
<img src = "/images/overdensities.png">
</p>
<p align = "center">
<font size="-0.5">DM visualisation of a few selected regions in <span style="font-variant: small-caps;">Flares</span>.</font>
</p>

<p align = "center">
<img src = "/images/cdf.png">
</p>
<p align = "center">
<font size="-0.5">Combined cumulative galaxy number counts of <span style="font-variant: small-caps;">Flares</span> compared to the <span style="font-variant: small-caps;">Eagle</span> Reference simulation volume. <span style="font-variant: small-caps;">Flares</span> has more than ~20 times galaxies with stellar mass greater than 10<sup>10</sup> M<sub>&odot;.</sub></font>
</p>

The increased dynamic range probed by <span style="font-variant: small-caps;">Flares</span> allows us to make predictions for a number of large area surveys that will probe the EoR in coming years, such as Euclid and Nancy Grace Roman Space Telescope as well as JWST.  As can be seen from the cumulative galaxy mass function plot above, the mass range has been significantly extended compared to the <span style="font-variant: small-caps;">Eagle</span> reference volume. Also <span style="font-variant: small-caps;">Flares</span> has access to a much larger sample of galaxies, thus providing a useful statistical sample of galaxies accessible to upcoming facilities. 

<p align = "center">
<img src = "/images/gsmf_multi_both.png">
</p>
<p align = "center">
<font size="-0.5">Stellar mass function of the <span style="font-variant: small-caps;">Flares</span> galaxies in z=5-10, observations and model values are plotted alongside.</font>
</p>

We use a line-of-sight (LOS) dust extinction model to model the photometric properties of the galaxies in the simulation. This is done by assuming that the dust optical depth along the line of sight is proportional to the LOS dust column density. We convert the LOS metal density for each star particle to a dust density based on the dust-to-metal ratio fitting function presented in [Vijayan et al. (2019)](https://ui.adsabs.harvard.edu/abs/2019MNRAS.489.4072V/abstract). We calibrate the proportionality constant based on the luminosity function at z=5 presented in [Bouwens et al. 2015](https://ui.adsabs.harvard.edu/abs/2015ApJ...803...34B/abstract) as well as the UV-continuum slope from [Bouwens et. al (2014)](https://ui.adsabs.harvard.edu/abs/2014ApJ...793..115B/abstract) at z=5 and the [OIII] doublet EW measurements at z=8 from [deBarros et al. (2019)](https://ui.adsabs.harvard.edu/abs/2019MNRAS.489.2355D/abstract).

<p align = "center">
<img src = "/images/LF_FUV_z5_10_Observations+Models.png">
</p>
<p align = "center">
<font size="-0.5">UV luminosity function of the <span style="font-variant: small-caps;">Flares</span> galaxies in the range z=5-10. Also shown are data points from observations and models. The <span style="font-variant: small-caps;">Flares</span> galaxies extends the UV luminosity function to the very brighter regime.</font>
</p>

<p align = "center">
<img src = "/images/sfrd.png" width="45%">
<font size="-0.5">The star formation rate density evolution as probed by <span style="font-variant: small-caps;">Flares</span>.</font>
</p>

We find no environmental dependence on the shape of the UV luminosity function. Another interesting observation is that the obscured star formation density (SFRD) is almost equal to the unobscured SFRD by z~6 and starts to dominates below.

<h2>Dust Modelling in L-Galaxies Semi-Analytical Model</h2>
L-Galaxies is a semi-analytical model (SAM), implemented on the Millennium ([Springel et al. 2005](https://ui.adsabs.harvard.edu/abs/2005Natur.435..629S/abstract)) and Millennium-II ([Boylan-Kolchin et al. 2009](https://ui.adsabs.harvard.edu/abs/2009MNRAS.398.1150B/abstract)) simulation merger trees. The model has been developed over the years to include the relevant processes required for galaxy evolution. The model has been really successful in matching many of the observational results like the galaxy stellar mass function across redshifts (Henriques et al., [2015](https://ui.adsabs.harvard.edu/abs/2015MNRAS.451.2663H/abstract), [2020](https://ui.adsabs.harvard.edu/abs/2020MNRAS.491.5795H/abstract)), the high redshift ( z ≥ 4 ) UV luminosity function (Clay et al., 2015). A self-consistent model of dust formation and evolution has been incorporated in the L-Galaxies' SAM, which is built on top of the  [Henriques et al., 2015](https://ui.adsabs.harvard.edu/abs/2015MNRAS.451.2663H/abstract) model. 

<p align = "center">
<img src = "/images/DTM_met_MR_MRII_full.png">
<font size="-0.5">The dust-to-metal ratio as a function of their metallicity from z = 0-8. The orange line shows the median result from galaxies in our model, with the dashed lines denoting the 84 and 16 percentiles. Green blue and red points show the observational constraints from Rémy-Ruyer et al. (2015), De Cia et al. (2016) and Wiseman et al. (2017) respectively.</font>
</p>

<p align = "center">
<img src = "/images/DTM_stellar_MR_MRII_full_age.png">
<font size="-0.5">The dust-to-metal ratio as a function of stellar mass from z = 0 − 8, with galaxies coloured according to their mass-weighted stellar age in Gyrs. Green points show the observational constraints from Rémy-Ruyer et al. (2015).</font>
</p>

The novel features in this work compared to similar efforts that have been published for semi-analytic and hydrodynamic models (e.g. Popping et al., 2017; McKinnon et al., 2017) are (i) the more accurate consideration of the impact of molecular cloud chemistry on grain growth in dense molecular clouds (by separate tracking of dust in molecular and diffuse gas) and (ii) incorporating information on the critical metals in the main dust species as well as dust depletion fractions. The former results in the diverse distribution of the dust-to-metal ratio seen in the high-redshift Universe in the model and the latter to the non-saturation of metal depletion onto dust. The model also predicts grain growth to be the significant dust production mechanism for z ≤ 8. We see an evolution across redshifts in the DTM ratio from low to high values, the former corresponding to dust injection from type II supernovae, and the other to maximal, saturated dust production occurring via dust growth on grains. The latter dominates at redshifts below z~4. We also see a significantly populated transition region at z = 6. We also provide a fitting function for the DTM ratio from our model, as a function of the gas-phase metallicity and the age of the galaxy stellar population, which provides a useful tool for simulators and observers alike.

The DTM fitting function is expressed as below:
<center>DTM<sub>fit</sub> = D<sub>0</sub>  + (D<sub>1</sub> -D<sub>0</sub> )(1-exp(-&alpha;Z<sup>&beta;</sup>(Age/&tau;)<sup>&tau;</sup>)),
</center>
where D<sub>0</sub> and D<sub>1</sub> represent the initial type-II SNe dust injection and the saturation value, respectively, Z is the metallicity of the interstellar medium, Age is the mass-weighted age of the stellar population, and &tau;=&tau;<sub>acc,0</sub>/D<sub>0</sub> Z is an estimate of the initial dust growth timescale after dust injection from type-II supernovae but prior to the initiation of dust growth on grains. We fix the values of D<sub>0</sub> and D<sub>1</sub> by reference to the figure showing the relationship between the DTM ratio and stellar mass. The parameter values are as follows: D<sub>0</sub> = 0.008, D<sub>1</sub> = 0.329, &alpha; = 0.017, &beta; = -1.337 and &gamma; = 2.122.
