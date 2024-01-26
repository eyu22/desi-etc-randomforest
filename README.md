# desi-etc-randomforest
This is an exploration of finding ways to optimize the exposure time calculator (ETC) on the [Dark Energy Spectroscopic Instrument (DESI)](https://www.desi.lbl.gov/) with random forests trained on telemetry data from exposures-daily.fits. More detail can be found on the [Improving DESI Exposure Time Calculator Slideshow](https://docs.google.com/presentation/d/109zAjj5-1mi8YDfl0rRxocYNSrqs1EfgzJUCy6p96B0/edit?usp=sharing) presented at a DESI instrumentation telecon in July 2023.

The scripts are organized into predictions for bright-time and dark-time. The goal of each random forest is to predict the ratio of `'EFFTIME_SPEC'/'EFFTIME_ETC'` for a given night based on its telemetry data (seeing, airmass, EBV, etc...). `'EFFTIME_SPEC'` is the telescope's spectroscopic (offline) effective time and `'EFFTIME_ETC'` is the actual exposure time. Using the random forest predictions to impose corrections, the overall spread of these ratios were reduced. This opens the possibility of improving exposure time calculations in the future to avoid underexposed and overexposed data. Shown below is one of these results for bright-time:

![]()
