### Telemetry parameters trained on:

'AIRMASS','EBV', 'TRANSPARENCY_GFA', 'SEEING_GFA', 'FIBER_FRACFLUX_GFA', 'SKY_MAG_AB_GFA','SKY_MAG_G_SPEC','SKY_MAG_R_SPEC','G-R','SKY_MAG_Z_SPEC','EFFTIME_GFA'

### BrightRandomForest.ipynb

- uses random forest trained on telemetry parameters of the current night (e.g. Night 1) to predict the ET ratio for the current night (e.g. Night 1)
- the random forest prediction is then used to reduce outliers and spread by dividing the current ET ratios by the random forest predicted ones such that a perfect prediction would result in a corrected value of 1

### BrightPrevNightCorrections.ipynb

- this script imposes corrections by dividing the ET ratio of each night (e.g. Night 2) by the ET ratio of the previous night (e.g. Night 1) with the assumption that the previous night's ET ratio will be similar to the current night's ET ratio, creating a corrected ratio closer to 1
- these corrections only apply to nights that have telemetry data from the night before, any pairs of data taken more than a day apart were discarded
