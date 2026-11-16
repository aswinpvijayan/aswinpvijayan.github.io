---
layout: page
title: Research
---

I am interested in working at the interface of theoretical modelling and observations, seeking to refine our understanding through an apples-to-apples comparison by forward modelling simulations.

My current focus is on modelling the spectral energy distributions (SEDs) of the broad and narrow line regions of active galactic nuclei (AGN) in <span class="sc">Synthesizer</span>, and on forward modelling publicly available, state-of-the-art cosmological simulations.

Below you will find some of the research that I have been involved with. If you are interested, feel free to [get in touch](../contact).

<details>
<summary class="summary-main"><span class="sc">Synthesizer</span></summary>
<a href="https://synthesizer-project.github.io/"><span class="sc">Synthesizer</span></a> is an open-source Python package for forward modelling synthetic astronomical observables, of which I am one of the co-PIs. It is designed to be fast, modular and flexible, allowing the user to generate spectra, photometry, images and spectral data cubes from both parametric models of galaxies and the outputs of cosmological hydrodynamical simulations and semi-analytic models. <span class="sc">Synthesizer</span> works with pre-computed grids of stellar population synthesis and AGN models, which can be post-processed with photoionisation codes such as <span class="sc">Cloudy</span> to include nebular line and continuum emission, and combined with models for dust attenuation and emission. This makes it easy to explore how different modelling choices change predicted observables, enabling like-for-like comparisons between theory and observations. The code is available on <a href="https://github.com/synthesizer-project/synthesizer">GitHub</a>, and the introductory paper can be found at <a href="https://ui.adsabs.harvard.edu/abs/2025arXiv250803888L/abstract">Lovell, Roper, Vijayan, Wilkins et al. (2025)</a> and the JOSS paper at <a href="https://joss.theoj.org/papers/10.21105/joss.09436">Roper, Lovell, Vijayan, Wilkins et al. (2026)</a>, with the stellar photoionisation modelling described in <a href="https://ui.adsabs.harvard.edu/abs/2026arXiv260727467V/abstract">Vijayan et al. (2026)</a>.

In <a href="https://ui.adsabs.harvard.edu/abs/2026arXiv260727467V/abstract">Vijayan et al. (2026)</a> we describe how emission from photoionised gas is incorporated into <span class="sc">Synthesizer</span>, and quantify how modelling choices such as the stellar population synthesis model, initial mass function, ionisation parameter, gas density, geometry, elemental abundances, depletion onto dust grains and dust itself affect commonly used spectral diagnostics. We also demonstrate how these models can be applied to everything from simple toy models to large cosmological simulations.

<figure class="figure">
<a href="/images/synthesizer_parametric.png"><img src="/images/synthesizer_parametric.png" alt="Two-panel plot: synthetic spectrum of a stellar population from 1000 to 10000 Angstrom showing incident, nebular continuum, transmitted, escaped and intrinsic components, with equivalent widths of labelled emission lines above."></a>
<figcaption>Spectra of a parametric stellar population generated with <span class="sc">Synthesizer</span>. The bottom panel shows the different spectral components (incident, nebular continuum, transmitted, escaped and intrinsic), while the top panel shows the equivalent widths of prominent emission lines, coloured by element. From <a href="https://ui.adsabs.harvard.edu/abs/2026arXiv260727467V/abstract">Vijayan et al. (2026)</a>.</figcaption>
</figure>
</details>

<details>
<summary class="summary-main">Dust in the <span class="sc">Colibre</span> simulations</summary>
<span class="sc">Colibre</span> is a new suite of cosmological hydrodynamical simulations of galaxy formation that models the cold interstellar medium and follows the formation and evolution of dust grains during the simulation (<a href="https://academic.oup.com/mnras/article/548/1/stag375/8650959">Schaye et al. 2026</a>; <a href="https://academic.oup.com/mnras/article/548/1/stag300/8650960">Chaikin et al. 2026</a>). In <a href="https://ui.adsabs.harvard.edu/abs/2026arXiv260726058V/abstract">Vijayan et al. (2026)</a> we study how galaxy dust scaling relations evolve over 0 &le; z &le; 15, using volumes of up to (400 cMpc)<sup>3</sup> at three different mass resolutions. We present predictions for the dust mass function, the cosmic dust mass density and dust scaling relations such as the dust-to-metal and dust-to-gas ratios.

We find that silicates dominate the dust mass at all epochs. The model broadly reproduces most observed dust scaling relations across cosmic time, although it overpredicts the cosmic dust mass density at z &lt; 1 and underpredicts the number of bright submillimetre galaxies at z &ge; 2. The scaling relations are only sensitive to numerical resolution for low-mass galaxies at low redshift.

<figure class="figure">
<img src="/images/DTM_met_colibre.png" alt="Nine-panel plot of the dust-to-metal ratio against gas-phase oxygen abundance from redshift 0 to 15, comparing three COLIBRE resolutions with observational data.">
<figcaption>The dust-to-metal ratio as a function of gas-phase metallicity in <span class="sc">Colibre</span> from z = 0 to 15, for three different resolutions (m5, m6 and m7). The dashed line shows the z = 0 relation from the L200m6 volume for reference. Also shown are observational constraints at these redshifts.</figcaption>
</figure>
</details>

<details>
<summary class="summary-main">Interpreting nebular emission lines at high redshift</summary>
JWST now routinely measures nebular emission lines from galaxies in the first billion years, and these are used to infer quantities such as the star formation rate, the ionising photon production efficiency and the gas-phase oxygen abundance. In <a href="https://ui.adsabs.harvard.edu/abs/2025arXiv250720190V/abstract">Vijayan et al. (2025)</a> we test how reliable these diagnostics are at z &ge; 5, focusing on dust corrections based on the V-band attenuation (A<sub>V</sub>) and the Balmer decrement. Using both toy models and galaxies from <span class="sc">Flares</span>, we show that the clumpy structure of galaxies biases the inferred properties, and that no single dust-correction method gives unbiased results for all of these quantities.
</details>

<details>
<summary class="summary-main">First Light And Reionisation Epoch Simulations (<span class="sc">Flares</span>)</summary>
<a href="https://flaresimulations.github.io/"><span class="sc">Flares</span></a> is a suite of high-resolution hydrodynamic simulations of galaxy formation and evolution using the <span class="sc">Eagle</span> physics. The suite consists of 40 zoom resimulations of spherical regions selected at z=5 from a 3.2 cGpc a side, parent dark matter-only box. We select a range of overdensities in order to study the environmental effect on high-redshift galaxy evolution. We also combine these resimulations in order to produce composite distribution functions, significantly extending the dynamic range of the model over smaller volume, periodic simulations. The introductory papers can be found at <a href="https://ui.adsabs.harvard.edu/abs/2021MNRAS.500.2127L/abstract">Lovell et al. (2021)</a> and <a href="https://ui.adsabs.harvard.edu/abs/2021MNRAS.501.3289V/abstract">Vijayan et al. (2021)</a>.  

<figure class="figure">
<img src="/images/overdensities.png" alt="Dark matter density maps of eleven spherical FLARES regions, ranging from the most overdense (delta = 0.97) to underdense regions (delta = -0.48).">
<figcaption>DM visualisation of a few selected regions in <span class="sc">Flares</span>.</figcaption>
</figure>

<figure class="figure">
<img src="/images/cdf.png" alt="Plot of cumulative galaxy number counts against stellar mass, comparing the combined FLARES regions with the EAGLE Reference volume.">
<figcaption>Combined cumulative galaxy number counts of <span class="sc">Flares</span> compared to the <span class="sc">Eagle</span> Reference simulation volume. <span class="sc">Flares</span> has ~20 times more galaxies with stellar mass greater than 10<sup>10</sup> M<sub>&odot;.</sub></figcaption>
</figure>

The increased dynamic range probed by <span class="sc">Flares</span> allows us to make predictions for a number of large area surveys that will probe the EoR in coming years, such as Euclid and Nancy Grace Roman Space Telescope as well as JWST.  As can be seen from the cumulative galaxy mass function plot above, the mass range has been significantly extended compared to the <span class="sc">Eagle</span> reference volume. Also <span class="sc">Flares</span> has access to a much larger sample of galaxies, thus providing a useful statistical sample of galaxies accessible to upcoming facilities.

<figure class="figure">
<img src="/images/gsmf_multi_both.png" alt="Plot of the galaxy stellar mass function at redshifts 5 to 10, comparing FLARES with observations and other models.">
<figcaption>Stellar mass function of the <span class="sc">Flares</span> galaxies in z=5-10, observations and model values are plotted alongside.</figcaption>
</figure>

<figure class="figure">
<img src="/images/team_meating.png" alt="Seven members of the FLARES team sitting around a table in a pub in Brighton.">
<figcaption>A past <span class="sc">Flares</span> team meeting in Brighton.</figcaption>
</figure>

<details>
<summary class="summary-sub"><span class="sc">Flares</span> Line-of-sight dust modelling</summary>
We use a line-of-sight (LOS) dust extinction model to model the photometric properties of the galaxies in the simulation. This is done by assuming that the dust optical depth along the line of sight is proportional to the LOS dust column density. We convert the LOS metal density for each star particle to a dust density based on the dust-to-metal ratio fitting function presented in <a href="https://ui.adsabs.harvard.edu/abs/2019MNRAS.489.4072V/abstract">Vijayan et al. (2019)</a>. We calibrate the proportionality constant based on the luminosity function at z=5 presented in <a href="https://ui.adsabs.harvard.edu/abs/2015ApJ...803...34B/abstract">Bouwens et al. (2015)</a> as well as the UV-continuum slope from <a href="https://ui.adsabs.harvard.edu/abs/2014ApJ...793..115B/abstract">Bouwens et al. (2014)</a> at z=5 and the [OIII] doublet EW measurements at z=8 from <a href="https://ui.adsabs.harvard.edu/abs/2019MNRAS.489.2355D/abstract">De Barros et al. (2019)</a>.

<figure class="figure">
<img src="/images/LF_FUV_z5_10_Observations+Models.png" alt="Plot of the far-UV luminosity function at redshifts 5 to 10, comparing FLARES with observations and other models.">
<figcaption>UV luminosity function of the <span class="sc">Flares</span> galaxies in the range z=5-10. Also shown are data points from observations and models. The <span class="sc">Flares</span> galaxies extend the UV luminosity function to brighter luminosities.</figcaption>
</figure>

<figure class="figure narrow">
<img src="/images/sfrd.png" alt="Plot of star formation rate density against redshift in FLARES, split into obscured and unobscured contributions.">
<figcaption>The star formation rate density evolution as probed by <span class="sc">Flares</span>.</figcaption>
</figure>

We find no environmental dependence on the shape of the UV luminosity function. Another interesting observation is that the obscured star formation rate density (SFRD) is almost equal to the unobscured SFRD by z~6 and starts to dominate at lower redshifts.
</details>

<details>
<summary class="summary-sub"><span class="sc">Flares</span>-<span class="sc">skirt</span> modelling</summary>
We modelled the full SED of the galaxy in post-processing using the radiative transfer code <a href="https://skirt.ugent.be/"><span class="sc">skirt</span></a> in <a href="https://ui.adsabs.harvard.edu/abs/2022MNRAS.511.4999V/abstract">Vijayan et al. (2022)</a>. The modelling assumptions build upon previous <span class="sc">Eagle</span>-<span class="sc">skirt</span> work done in <a href="https://ui.adsabs.harvard.edu/abs/2016MNRAS.462.1057C/abstract">Camps et al. (2016)</a> and <a href="https://ui.adsabs.harvard.edu/abs/2017MNRAS.470..771T/abstract">Trayford et al. (2017)</a>. We look at the infrared luminosity function, the infrared excess (IRX) and the light-weighted dust temperatures of the most massive galaxies in <span class="sc">Flares</span> in the redshift range 5-10.

We find that the IR LF is underpredicted at bright IR luminosities compared to current observational results. We see that the <span class="sc">Flares</span> IRX-&beta; relation mainly follows the local starburst relation. We also see an evolution of the light-weighted dust temperatures towards higher values with increasing redshift.

<figure class="figure">
<img src="/images/IRX_beta_sSFR.png" alt="Plot of infrared excess against UV continuum slope for FLARES galaxies at redshifts 5 to 10, coloured by specific star formation rate.">
<figcaption>The IRX-&beta; relation of <span class="sc">Flares</span> galaxies at z=5-10 coloured by their specific star formation rate. Also shown are some observational and theoretical data at these redshifts.</figcaption>
</figure>

<figure class="figure narrow">
<img src="/images/Tdust_z_variation.png" alt="Plot of light-weighted dust temperature against redshift for FLARES galaxies, comparing three temperature definitions with observational and theoretical data.">
<figcaption>The redshift evolution of the light-weighted dust temperatures of the <span class="sc">Flares</span> galaxies at z=5-10. T<sub>peak</sub> is the temperature derived from the wavelength at which the IR flux density peaks, T<sub>SED</sub> is the dust temperature obtained from fitting a mid-IR power law + modified blackbody (MBB) to the IR SED, while T<sub>SED,RJ</sub> is the temperature from an optically-thin MBB. Also shown are some observational and theoretical data at these redshifts.</figcaption>
</figure>
</details>

<details>
<summary class="summary-sub">Sizes of massive dusty galaxies from the UV to the IR</summary>
In <a href="https://ui.adsabs.harvard.edu/abs/2025A%26A...696A.234P/abstract">Punyasheel et al. (2025)</a>, led by my student Paurush Punyasheel, we study the UV and far-infrared sizes of massive (M<sub>&#8902;</sub> &gtrsim; 10<sup>9</sup> M<sub>&odot;</sub>) <span class="sc">Flares</span> galaxies at 5 &le; z &le; 10, using the <span class="sc">skirt</span> radiative transfer models and mock JWST NIRCam and ALMA observations. We find that dust makes galaxies appear smaller in the UV, that their far-infrared sizes do not evolve with redshift, and that noise and the instrumental PSF strongly affect the measured sizes. The predicted evolution of UV sizes broadly agrees with observations.

<figure class="figure">
<img src="/images/NIRCAM_ALMA_Punyasheel.png" alt="Two rows of six image cut-outs of simulated galaxies at redshifts 5 to 10: JWST NIRCam colour images on top and ALMA dust-continuum maps below, each labelled with stellar mass and UV luminosity.">
<figcaption>Mock JWST NIRCam (top) and ALMA (bottom) images of massive <span class="sc">Flares</span> galaxies from z = 5 to 10, labelled with their stellar masses and UV luminosities.</figcaption>
</figure>
</details>

<details>
<summary class="summary-sub">Offsets between UV and dust emission</summary>
In <a href="https://ui.adsabs.harvard.edu/abs/2026arXiv260527370P/abstract">Punyasheel et al. (2026)</a>, also led by Paurush Punyasheel, we measure the spatial offsets between the UV and far-infrared emission of 6890 massive <span class="sc">Flares</span> galaxies at 5 &le; z &le; 10, using mock JWST NIRCam and ALMA observations. About 16% of galaxies show offsets of at least 2.5 kpc. These offsets do not correlate with stellar mass, luminosity, size, AGN feedback, environment or merger history, but the offset galaxies have bluer UV slopes and formed their stars earlier.
</details>
</details>

<details>
<summary class="summary-main">Dust Modelling in L-Galaxies Semi-Analytical Model</summary>
L-Galaxies is a semi-analytical model (SAM), implemented on the Millennium (<a href="https://ui.adsabs.harvard.edu/abs/2005Natur.435..629S/abstract">Springel et al. 2005</a>) and Millennium-II (<a href="https://ui.adsabs.harvard.edu/abs/2009MNRAS.398.1150B/abstract">Boylan-Kolchin et al. 2009</a>) simulation merger trees. The model has been developed over the years to include the relevant processes required for galaxy evolution. The model has been successful in matching many of the observational results like the galaxy stellar mass function across redshifts (Henriques et al. <a href="https://ui.adsabs.harvard.edu/abs/2015MNRAS.451.2663H/abstract">2015</a>, <a href="https://ui.adsabs.harvard.edu/abs/2020MNRAS.491.5795H/abstract">2020</a>), the high redshift ( z ≥ 4 ) UV luminosity function (<a href="https://ui.adsabs.harvard.edu/abs/2015MNRAS.451.2692C/abstract">Clay et al., 2015</a>). A self-consistent model of dust formation and evolution has been incorporated in the L-Galaxies' SAM, which is built on top of the <a href="https://ui.adsabs.harvard.edu/abs/2015MNRAS.451.2663H/abstract">Henriques et al. (2015)</a> model.

<figure class="figure">
<img src="/images/DTM_met_MR_MRII_full.png" alt="Plot of dust-to-metal ratio against metallicity at redshifts 0 to 8 from the L-Galaxies dust model, with observational constraints.">
<figcaption>The dust-to-metal ratio as a function of their metallicity from z = 0-8. The orange line shows the median result from galaxies in our model, with the dashed lines denoting the 84 and 16 percentiles. Green, blue and red points show the observational constraints from Rémy-Ruyer et al. (2015), De Cia et al. (2016) and Wiseman et al. (2017) respectively.</figcaption>
</figure>

<figure class="figure">
<img src="/images/DTM_stellar_MR_MRII_full_age.png" alt="Plot of dust-to-metal ratio against stellar mass at redshifts 0 to 8, with galaxies coloured by mass-weighted stellar age.">
<figcaption>The dust-to-metal ratio as a function of stellar mass from z = 0 − 8, with galaxies coloured according to their mass-weighted stellar age in Gyr. Green points show the observational constraints from Rémy-Ruyer et al. (2015).</figcaption>
</figure>

The novel features in this work, compared to similar efforts that have been published for semi-analytic and hydrodynamic models (e.g. <a href="https://ui.adsabs.harvard.edu/abs/2017MNRAS.471.3152P/abstract">Popping et al., 2017</a>; <a href="https://ui.adsabs.harvard.edu/abs/2017MNRAS.468.1505M/abstract">McKinnon et al., 2017</a>), are (i) the more accurate consideration of the impact of molecular cloud chemistry on grain growth in dense molecular clouds (by separate tracking of dust in molecular and diffuse gas) and (ii) incorporating information on the critical metals in the main dust species as well as dust depletion fractions. The former results in the diverse distribution of the dust-to-metal ratio seen in the high-redshift Universe in the model and the latter to the non-saturation of metal depletion onto dust. The model also predicts grain growth to be the dominant dust production mechanism for z ≤ 8. We see an evolution across redshifts in the dust-to-metal (DTM) ratio from low to high values, the former corresponding to dust injection from type II supernovae, and the other to maximal, saturated dust production occurring via dust growth on grains. The latter dominates at redshifts below z~4. We also see a significantly populated transition region at z = 6. We also provide a fitting function for the DTM ratio from our model, as a function of the gas-phase metallicity and the age of the galaxy stellar population, which provides a useful tool for simulators and observers alike.

The DTM fitting function is expressed as below:
<p class="equation">DTM<sub>fit</sub> = D<sub>0</sub>  + (D<sub>1</sub> -D<sub>0</sub> )(1-exp(-&alpha;Z<sup>&beta;</sup>(Age/&tau;)<sup>&gamma;</sup>)),</p>
where D<sub>0</sub> and D<sub>1</sub> represent the initial type-II SNe dust injection and the saturation value, respectively, Z is the metallicity of the interstellar medium, Age is the mass-weighted age of the stellar population, and &tau;=&tau;<sub>acc,0</sub>/(D<sub>0</sub>Z) is an estimate of the initial dust growth timescale after dust injection from type-II supernovae but prior to the initiation of dust growth on grains. We fix the values of D<sub>0</sub> and D<sub>1</sub> by reference to the figure showing the relationship between the DTM ratio and stellar mass. The parameter values are as follows: D<sub>0</sub> = 0.008, D<sub>1</sub> = 0.329, &alpha; = 0.017, &beta; = -1.337 and &gamma; = 2.122.
</details>
