# Group_fMRI_Analysis
 
We analyze the data from Smeets et al. (2013) composed by $29$ subjects passively looking to food and no-food images. The group analysis to explore the differences in BOLD response recorded under the two experimental conditions was performed using [FSL](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FSL). The registration step to standard space images was computed using FLIRT (Jenkinson and Smith, 2001) (Jenkinson et al., 2012), the motion correction using MCFLIRT (Jenkinson et al., 2002), the non-brain removal using BET (Smith, 2002) and spatial smoothing using a Gaussian Kernel FWHM (6mm). Finally, the intensity normalization of the entire 4D dataset was computed by a single multiplicative factor, and the high-pass temporal filtering (Gaussian-weighted least-squares straight-line fitting, with sigma=64.0s) was applied.

In the following figure, we can see how the values of the one-sample t-tests change applying different FSL approaches, i.e.:

1. Fixed Effects;
2. FLAME 1;
3. FLAME 12;
4. OLS.

<p align="center">
<img src="https://github.com/angeella/Group_fMRI_Analysis/Images/zstat_check_tot.png, width="400px" height="300px"/>
</p>

(TODO)




# References

SMEETS, P. A. M., M. KROESE, F. M., EVERS, C. and DE RIDDER, D. T. D. (2013). Allured or alarmed:
Counteractive control responses to food temptations in the brain. Behavioural Brain Research 248 41-45.
