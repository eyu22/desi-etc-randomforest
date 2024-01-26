### Telemetry parameters trained on:

'AIRMASS','EBV', 'TRANSPARENCY_GFA', 'SEEING_GFA', 'FIBER_FRACFLUX_GFA', 'SKY_MAG_AB_GFA','SKY_MAG_G_SPEC','SKY_MAG_R_SPEC','G-R','SKY_MAG_Z_SPEC','EFFTIME_GFA'

### CurrentNightBright.ipynb

- random forest trained on telemetry parameters of the current night (e.g. Night 1) to predict the ETC ratio for the current night (e.g. Night 1).

### PrevNightsBright.ipynb

-  random forest is trained on telemtry parameters of the previous night (e.g. Night 0) to predict the ETC ratio for the current night (e.g. Night 1).
