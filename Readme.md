# eixport
[![Travis-CI Build Status](https://travis-ci.org/atmoschem/eixport.svg?branch=master)](https://travis-ci.org/atmoschem/eixport)[![Build status](https://ci.appveyor.com/api/projects/status/frk36kmayf8yff70?svg=true)](https://ci.appveyor.com/project/Schuch666/eixport)

## Exporting emissions to other models

Emissions are mass that affects atmosphere in complex ways, not only physical, but also, in the health of humans, ecosystems, economically, etc.

There are several models whose inputs are emissions, such as [R-Line](https://www.cmascenter.org/r-line/) or [WRF-Chem](https://ruc.noaa.gov/wrf/wrf-chem/). Now experimental addition of inputs for running smoke and cmaq.

This R-Package provide functions to read emissions from [VEIN](https://github.com/ibarraespinosa/vein) and from other models
in different formats and export the emissions into the appropiate format suitable to other models.

The first case of this package will exporting VEIN emissions into the model R-Line.

some functions:

- to_rline: Export emissions to other formats
- to_wrf:	Combine total/spatial/temporal/split and write emission to file
- to_brams_spm:	inputs for SPM BRAMS
- wrf_profile: Create spatial profile for WRF-Chem
- wrf_create:	Create emission files to the WRF-Chem
- wrf_plot: simple plot for emissions
- wrf_get:	Read variables of emission files
- wrf_put:	Write variables in emission files


```{r eval=F}
# 0.2.9
devtools::install_github("atmoschem/eixport")
library(eixport)
?to_wrf
```

