---
layout: post
title: "CMIP5 HadCRUT4 comparison"
description: ""
category: analysis
tags: [temperatures, climate]
---
{% include JB/setup %}

# [Comparing the CMIP5 model temperatures to HadCRUT4](http://hansbrenna.github.io/analysis/2016/04/29/cmip5-hadcrut4-comparison)
Often, I see the claim that the models used in the Coupled Model Intercomparison Project phase 5 (CMIP5) are overestimating global temperatures compared to what is observed. I wanted to check this myself, so I downloaded the [CMIP5 global temperatures from 42 models](https://dl.dropboxusercontent.com/u/96723180/CMIP5%20Models%20Air%20Temp%20One%20Member.xlsx) and the [HadCRUT4 global mean temperatures](https://dl.dropboxusercontent.com/u/96723180/HadCRUT%20Absolute%20Temps.csv) from the beacon of sound climate science [www.wattsupwiththat.com](http://www.wattsupwiththat.com) and got to work. The HadCRUT4 data I downloaded are missing the last year. Maybe I'll be bothered to go back and fix it later. I used pandas to open the excel data, and did some pre-processing. First I did a five-year rolling mean both data sets, then I subtracted the 20th century mean value of the HadCRUT data from bot datasets. The next step was to calculate the multimodel mean and standard deviation of the 42 CMIP5 time series.

Figure 1 shows the HadCRUT4 temperatures together with the mean and standard deviation of the CMIP5 data compared to the HadCRUT4 global mean surface temperature from the beginning of the data until 2005 relative to the 20th centure HadCRUT4 mean value. For the entire period, the HadCRUT4 is well within one standard deviation of the CMIP multimodel mean, which I would interpret to mean that the CMIP5 ensemble of models, on average, is able to simulate the temperature evolution reasonably well. 

![CMIP5 and HadCRUT4 comparison](https://raw.githubusercontent.com/hansbrenna/cmip4_hadcrut4_comparison/master/hadcrut_cmip_comparison.png)
<br>
>Figure 1: HadCRUT4 global mean surfacce temperature compared to 42 CMIP5 models.

What happens after 2005? In 2005 the CMIP5 historical runs end, and that means the forcings driving the temperature evolution changes from historical forcing to one of the RCP scenarios, in this case RCP4.5. Whta this means is that the forcings driving the models after 2005 lack all of the random to semi-random events with climate impacts happening from time to time, for instance large and small volcanic eruptions are not accounted for after 2005. While the last decades have been relatively quiescent, the stratospheric aerosol layer has grown over this period caused by smaller volcanic eruptions and human emissions of sulfur (Solomon et al, 2012; Ridley et al, 2014).

In addition, as we get further away from 2005, the cyces of oscillations in the models, for instance ENSO, come out of phase with their real world counterparts. These two effects in combination can make the difference between models and observations large over shorter periods from months to decadal scales.

The code used to do this analysis is available from the GitHub repository [cmip5_hadcrut4_comparison](https://github.com/hansbrenna/cmip4_hadcrut4_comparison)

## References
Ridley, D. A., Solomon, S., Barnes, J. E., Burlakov, V. D., Deshler, T., Dolgii, S. I., ... & Ritter, C. (2014). Total volcanic stratospheric aerosol optical depths and implications for global climate change. Geophysical Research Letters, 41(22), 7763-7769.

Solomon, S., Daniel, J. S., Neely, R. R., Vernier, J. P., Dutton, E. G., & Thomason, L. W. (2011). The persistently variable “background” stratospheric aerosol layer and global climate change. Science, 333(6044), 866-870.
