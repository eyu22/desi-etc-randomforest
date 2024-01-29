# Dark-time Predictions

### [ETCparametersonly.ipynb](https://github.com/eyu22/desi-etc-randomforest/blob/main/dark_time/ETCparametersonly.ipynb)
- uses a random forest to predict the ET ratio using only the ETC data available on the mountain as training features
- features trained on are: 'EBV', 'TRANSPARENCY_GFA', 'SEEING_GFA','SKY_MAG_R_SPEC','SKY_MAG_G_SPEC' - 'SKY_MAG_R_SPEC'

### [top3RandomForestCorrections.ipynb](https://github.com/eyu22/desi-etc-randomforest/blob/main/dark_time/top3RandomForestCorrections.ipynb)
- uses a random forest to predict the ET ratio using only the top 3 most important features according to their permutation importance and mean decrease in impurity (MDI) importance
- features trained on are: 'EBV', 'SEEING_GFA', 'SKY_MAG_G_SPEC' - 'SKY_MAG_R_SPEC'

### [ETCCrossValidatedPolyRandForestComparison.ipynb](https://github.com/eyu22/desi-etc-randomforest/blob/main/dark_time/ETCCrossValidatedPolyRandForestComparison.ipynb)
- compares a 2nd and 3rd order polynomial fit to the random forest predictions for ET ratio
- features trained on are: 'AIRMASS','EBV', 'TRANSPARENCY_GFA', 'SEEING_GFA', 'FIBER_FRACFLUX_GFA', 'SKY_MAG_AB_GFA','SKY_MAG_G_SPEC','SKY_MAG_R_SPEC','G-R','SKY_MAG_Z_SPEC','EFFTIME_GFA'
