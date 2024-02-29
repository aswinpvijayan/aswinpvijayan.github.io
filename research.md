---
layout: page
title: Research
---

I am interested in working at the interface of theoretical modelling and observations, seeking to refine our understanding through an apples-to-apples comparison by forward modeling simulations.

Below you will find some of the research that I have been involved with. If you are interested, feel free to [get in touch](../contact)

<!-- <h2>First Light And Reionisation Simulations (<span style="font-variant: small-caps;">Flares</span>)</h2> -->
<details>
<summary><b><u><font size="+3">First Light And Reionisation Simulations (<span style="font-variant: small-caps;">Flares</span>)</font></u></b></summary>
The <span style="font-variant: small-caps;">Flare</span> simulations (<a href="https://flaresimulations.github.io/"><span style="font-variant: small-caps;">Flares</span></a>) are a suite of high-resolution hydrodynamic simulations of galaxy formation and evolution using the <span style="font-variant: small-caps;">Eagle</span> physics. The suite consists 40 zoom resimulations of spherical regions selected at z=5 from a 3.2 cGpc a side, parent dark matter-only box. We select a range of overdensities in order to study the environmental effect on high-redshift galaxy evolution. We also combine these resimulations in order to produce composite distribution functions, signficantly extending the dynamic range of the model over smaller volume, periodic simulations. The introductory papers can be found at <a href="https://ui.adsabs.harvard.edu/abs/2021MNRAS.500.2127L/abstract">Lovell et al. (2021)</a> and <a href="https://ui.adsabs.harvard.edu/abs/2021MNRAS.501.3289V/abstract">Vijayan et al. (2021)</a>.  

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

<details>
<summary><b><font size="+2"><span style="font-variant: small-caps;">Flares</span> Line-of-sight dust modelling</font></b></summary>
We use a line-of-sight (LOS) dust extinction model to model the photometric properties of the galaxies in the simulation. This is done by assuming that the dust optical depth along the line of sight is proportional to the LOS dust column density. We convert the LOS metal density for each star particle to a dust density based on the dust-to-metal ratio fitting function presented in <a href="https://ui.adsabs.harvard.edu/abs/2019MNRAS.489.4072V/abstract">Vijayan et al. (2019)</a>. We calibrate the proportionality constant based on the luminosity function at z=5 presented in <a href="https://ui.adsabs.harvard.edu/abs/2015ApJ...803...34B/abstract">Bouwens et al. 2015</a> as well as the UV-continuum slope from <a href="https://ui.adsabs.harvard.edu/abs/2014ApJ...793..115B/abstract">Bouwens et. al (2014)</a> at z=5 and the [OIII] doublet EW measurements at z=8 from <a href="https://ui.adsabs.harvard.edu/abs/2019MNRAS.489.2355D/abstract">deBarros et al. (2019)</a>.

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
</details>

<details>
<summary><b><font size="+2"><span style="font-variant: small-caps;">Flares</span>-<span style="font-variant: small-caps;">skirt</span> modelling</font></b></summary>
<!-- <h3><span style="font-variant: small-caps;">Flares</span>-<span style="font-variant: small-caps;">skirt</span> modelling</h3> -->
We modelled the full SED of the galaxy in post-processing using the radiative transfer code [<span style="font-variant: small-caps;">skirt</span>](https://skirt.ugent.be/) in <a href="https://ui.adsabs.harvard.edu/abs/2022MNRAS.511.4999V/abstract">Vijayan et al. (2022)</a>. The modelling assumptions builds upon previous <span style="font-variant: small-caps;">Eagle</span>-<span style="font-variant: small-caps;">skirt</span> work done in <a href="https://ui.adsabs.harvard.edu/abs/2016MNRAS.462.1057C/abstract">Camps et al. (2016)</a> and <a href="https://ui.adsabs.harvard.edu/abs/2017MNRAS.470..771T/abstract">Trayford et al. (2017)</a>. We look at the infrared luminosity function, the infrared excess (IRX) and the light-weighted dust temperatures of the most massive galaxies in <span style="font-variant: small-caps;">Flares</span> in the redshift range 5-10.

We find that the IR LF is underpredicted at bright IR luminosities compared to current observational results. We see that the <span style="font-variant: small-caps;">Flares</span> IRX-&beta; relation mainly follows the local starburst relation. We also see an evolution of the light-weighted dust temperatures towards higher values with increasing redshift.

<p align = "center">
<img src = "/images/IRX_beta_sSFR.png">
<font size="-0.5">The IRX-&beta; relation of <span style="font-variant: small-caps;">Flares</span> galaxies at z=5-10 coloured by their specific star formation rate. Also shown is some observational and theoretical data at these redshifts.</font>
</p>

<p align = "center">
<img src = "/images/Tdust_z_variation.png" width="50%">
<font size="-0.5">The redshift evolution of the light-weighted dust temperatures of the <span style="font-variant: small-caps;">Flares</span> galaxies at z=5-10. T<sub>peak</sub> is the wavelength at which the IR flux density peaks, T<sub>SED</sub> is the dust temperature obtained from fitting a mid-IR powerlaw + modified MBB to the IR SED while T<sub>SED,RJ</sub> is the temperature from an optically-thin MBB. Also shown is some observational and theoretical data at these redshifts.</font>
</p>
</details>
</details>

<details>
<summary><b><u><font size="+3">Dust Modelling in L-Galaxies Semi-Analytical Model</font></u></b></summary>
<!-- <h2>Dust Modelling in L-Galaxies Semi-Analytical Model</h2> -->
L-Galaxies is a semi-analytical model (SAM), implemented on the Millennium (<a href="https://ui.adsabs.harvard.edu/abs/2005Natur.435..629S/abstract">Springel et al. 2005</a>) and Millennium-II (<a href="https://ui.adsabs.harvard.edu/abs/2009MNRAS.398.1150B/abstract">Boylan-Kolchin et al. 2009</a>) simulation merger trees. The model has been developed over the years to include the relevant processes required for galaxy evolution. The model has been really successful in matching many of the observational results like the galaxy stellar mass function across redshifts (Henriques et al., <a href="https://ui.adsabs.harvard.edu/abs/2015MNRAS.451.2663H/abstract">2015</a>), (<a href="https://ui.adsabs.harvard.edu/abs/2020MNRAS.491.5795H/abstract">2020</a>), the high redshift ( z ≥ 4 ) UV luminosity function (<a href="https://ui.adsabs.harvard.edu/abs/2015MNRAS.451.2692C/abstract">Clay et al., 2015</a>). A self-consistent model of dust formation and evolution has been incorporated in the L-Galaxies' SAM, which is built on top of the  (<a href="https://ui.adsabs.harvard.edu/abs/2015MNRAS.451.2663H/abstract">Henriques et al. 2015</a>) model.

<p align = "center">
<img src = "/images/DTM_met_MR_MRII_full.png">
<font size="-0.5">The dust-to-metal ratio as a function of their metallicity from z = 0-8. The orange line shows the median result from galaxies in our model, with the dashed lines denoting the 84 and 16 percentiles. Green blue and red points show the observational constraints from Rémy-Ruyer et al. (2015), De Cia et al. (2016) and Wiseman et al. (2017) respectively.</font>
</p>

<p align = "center">
<img src = "/images/DTM_stellar_MR_MRII_full_age.png">
<font size="-0.5">The dust-to-metal ratio as a function of stellar mass from z = 0 − 8, with galaxies coloured according to their mass-weighted stellar age in Gyrs. Green points show the observational constraints from Rémy-Ruyer et al. (2015).</font>
</p>

The novel features in this work compared to similar efforts that have been published for semi-analytic and hydrodynamic models (e.g. <a href="https://ui.adsabs.harvard.edu/abs/2017MNRAS.471.3152P/abstract">Popping et al., 2017</a>; <a href="https://ui.adsabs.harvard.edu/abs/2017MNRAS.468.1505M/abstract">McKinnon et al., 2017</a>) are (i) the more accurate consideration of the impact of molecular cloud chemistry on grain growth in dense molecular clouds (by separate tracking of dust in molecular and diffuse gas) and (ii) incorporating information on the critical metals in the main dust species as well as dust depletion fractions. The former results in the diverse distribution of the dust-to-metal ratio seen in the high-redshift Universe in the model and the latter to the non-saturation of metal depletion onto dust. The model also predicts grain growth to be the significant dust production mechanism for z ≤ 8. We see an evolution across redshifts in the DTM ratio from low to high values, the former corresponding to dust injection from type II supernovae, and the other to maximal, saturated dust production occurring via dust growth on grains. The latter dominates at redshifts below z~4. We also see a significantly populated transition region at z = 6. We also provide a fitting function for the DTM ratio from our model, as a function of the gas-phase metallicity and the age of the galaxy stellar population, which provides a useful tool for simulators and observers alike.

The DTM fitting function is expressed as below:
<center>DTM<sub>fit</sub> = D<sub>0</sub>  + (D<sub>1</sub> -D<sub>0</sub> )(1-exp(-&alpha;Z<sup>&beta;</sup>(Age/&tau;)<sup>&tau;</sup>)),
</center>
where D<sub>0</sub> and D<sub>1</sub> represent the initial type-II SNe dust injection and the saturation value, respectively, Z is the metallicity of the interstellar medium, Age is the mass-weighted age of the stellar population, and &tau;=&tau;<sub>acc,0</sub>/D<sub>0</sub> Z is an estimate of the initial dust growth timescale after dust injection from type-II supernovae but prior to the initiation of dust growth on grains. We fix the values of D<sub>0</sub> and D<sub>1</sub> by reference to the figure showing the relationship between the DTM ratio and stellar mass. The parameter values are as follows: D<sub>0</sub> = 0.008, D<sub>1</sub> = 0.329, &alpha; = 0.017, &beta; = -1.337 and &gamma; = 2.122.
</details>
