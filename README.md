# GZ CEERS: bar fractions

This repo contains the data presented in Géron+2025.


## Description Tables

#### geron25_sample
This table contains all the information of the galaxies in the parent and volume-limited sample of Géron+2025.

`gz_ceers_id`: The CEERS ID of this galaxy.  
`candels_id`: The CANDELS ID of this galaxy.  
`ra`: The right ascension of this galaxy. In degrees.  
`dec`: The declination of this galaxy. In degrees.  
`z_candels`: The redshift of this galaxy, reported by CANDELS. It is a combination of photometric and spectroscopic redshifts. Corresponds to their `z_best` column.  
`bar_type`: Description of the bar strength of this galaxy. Either 'strong', 'weak' or 'no'.   
`vollim_flag`: A flag that corresponds to whether this galaxy is in the volume-limited sample.   


    
#### geron25_bar_fractions
This table contains the bar fractions. Corresponds to Table 2 of Géron+2025.  

`z_low`: The lower limit of this redshift bin.  
`z_high`: The upper limit of this redshift bin.  
`z_med`: The median value of the redshifts of all galaxies in this redshift bin.  
`z_p25`: The 25th percentile of the redshifts of all galaxies in this redshift bin.  
`z_p75`: The 75th percentile of the redshifts of all galaxies in this redshift bin.  

`fbar_raw`: The raw, uncorrected bar fraction. Corresponds to $f_{\rm bar, raw}$ in the paper.    
`fbar_fd`: The bar fraction, accounting for featureless discs in the denominator. Corresponds to $f_{\rm bar, FD}$ in the paper.  
`fbar_zcorr`: The bar fraction, corrected for redshift. Corresponds to $f_{\rm bar, z-corr}$ in the paper.  
`fbar_fd_zcorr`: The bar fraction, accounting for featureless discs and corrected for redshift. Recommended to use this value. Corresponds to $f_{\rm bar, fd, z-corr}$ in the paper.   
The columns with the `_ll` and `_ul` suffixes for every bar fraction correspond to the lower and upper limits calculated using the beta distribution quantile technique. 

`sample_size`: The sample size of this redshift bin.  
`n_bars`: The number of bars in this redshift bin.  
`n_strong_bars`: The number of strong bars in this redshift bin.  
`n_weak_bars`: The number of weak bars in this redshift bin.  

`fd_corr_factor`: The correction factor used to account for featureless discs.  
`z_corr_factor`: The correction factor used to correct for redshift.  
`tot_corr_factor`: The total correction factor.   
