---
layout: post
title: "Slaying dragons"
description: ""
category: opinion
tags: [climate]
---
{% include JB/setup %}

# Slaying dragons using Python and Pandas

The black metal band Solefald has a track called [Sagateller](https://m.youtube.com/watch?v=F4Ki1xy55Vg) on the album Black for Death where one line of lyrics reads “Ignorance, the dragon never dies”.

The dragon Ignorance is very much alive and well today, and it rears it’s monstrous form everywhere. I have been debating climate on the internet the last week, and here i really feel that Ignorance (of the wilful kind that is) is present. Participating in these discussions really feels like attempting to kill a dragon that sprouts new heads every time one is cut off. The amount of ignorance present in arguments that are written in all sincerity by some people is simply baffling. 

## Remote Sensing System TLT trend analysis

I will go into one particular example, that I come across almost every time i involve myself in discussions about climate. The trend in global warming since 1998. The argument goes as follows: Since 1998 there has been almost no/very little/negative global warming, then a reference to a sattellite dataset with a trendline drawn from 1998 until today. Often the set is cropped to start in 1998 as well to undermine the perception of the long-term trend. A typical example is this one from [Climate Depot](http://www.climatedepot.com/2015/09/02/a-new-record-pause-length-satellite-data-no-global-warming-for-18-years-8-months/). My argument is that the trend from 1998 until today is not robust, a point that has probably been made many times, but that I wanted to make myself. 

I downloaded the Remote Sensing Systems (RSS) global mean lower troposphere temperature anomaly [dataset](http://data.remss.com/msu/graphics/TLT/time_series/RSS_TS_channel_TLT_Global_Land_And_Sea_v03_3.txt) (I wanted to use the UAH set, but I couldn’t get the site open that evening). Using Python and Pandas, I did a rudimentary trend analysis to see how robust the trend from 1998 until the end of the data set really is. The trend lines with different starting years are shown in Figure 1. 

A few things are immediately clear: The trend over the entire data set is 0.13 K/decade. The year 1998 was a clear outlier (it was a strong El Ñino year). Trends calculated based on 1998 or the years immidiately prior to it are significantly smaller than the long term trend. Having an outlier at the beginning of the data set really skews the entire trend line a lot, (having one at the end is impacting the trend a lot as well, but the reasonable choice is to calculate the trend until the end of the data set.) and choosing an outlier as the starting point of the trend analysis is a powerful way of getting the result you want.

![RSS trend lines](https://raw.githubusercontent.com/hansbrenna/RSS_trend_analysis/master/trendlines.png)
> Figure 1: The RSS global mean lower troposphere temperature (TLT) with trendlines calculated based on different starting times.

Figure 2 shows the trend in K/decade starting from every month in the data set on a logarithmic y-axis. The point of this figure is to show that as we get to 1998 as the starting point, the trend falls off precipitously by almost two orders of magnitude, while rebounding almost immediately afterwards. Of course, as we get towards the end of the data set, the trend becomes increasingly meaningless, but the dip around 1998 powerfully shows the disingeniousness of choosing this year as the starting point of any trend analysis. 

![RSS trend is not robust](https://raw.githubusercontent.com/hansbrenna/RSS_trend_analysis/master/trends.png)
> Figure 2: Decadal temperature trend bassed on each month in the RSS dataset. The trend calculated from 1998 is two orders of magnitude lower than the surrounding periods.

## In summary

The trend in sattellite measured temperatures since 1998 is a loved argument by climate change deniers. I think it is seriously misleading to use 1998 as the starting point, since using this year does not give robust trends. Finally, has global warming slowed in the new milennium? Trends calculated based on times after 1998 are a bit lower than the long term trend, but increase continued and there was no return to the previous normal temperatures in later years. Thus 1998 looks a step change in global mean lower tropospherer temperatures. What will be interesting to see is what will happen over the next 10 years, since 2015-2016 will be another ENSO-driven outlier from the new higher baseline. Will we see a return to the smooth increase of the period before 1998 or are we now in a regime where global warming comes in the form of step changes every few ENSO cycles? It will be interesting to see.

I made a GitHub repository for this analysis, and it contains the data set I used, the code and the outputs, so take a look over [there](https://github.com/hansbrenna/RSS_trend_analysis) if you want.
