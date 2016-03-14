---
layout: post
title: "Slaying dragons"
description: ""
category: opinion
tags: [climate]
---
{% include JB/setup %}

# Slaying dragons

The black metal band Solefald has a song called [Sagateller](https://m.youtube.com/watch?v=F4Ki1xy55Vg) on the album Black for Death where one line of lyrics reads “Ignorance, the dragon never dies”. “In the Midgard of men they call you sagateller. In the Asgard of gods they call you dragonkiller” Ignorance is likened to an immortal dragon and the skald, the keeper and transmitter of knowledge and wisdom, as the hero attempting to remove the threat of ignorance to society.

The dragon Ignorance is very much alive and well today, and it rears it’s monstrous hydra-headed form everywhere. If this all sound very dramatic, I have a rather more prosaic point to make. I have been debating climate on the internet the last week, and here i really feel that the dragon Ignorance (of the wilful kind that is) is present. The amount of ignorant arguments that are written in all sincerity by some people is simply baffling. 

I will go into one particular example, that I come across almost every time i involve myself in discussions about climate. The trend in global warming since 1998. The argument goes as follows: Since 1998 there has been almost no/very little/negative global warming, then a reference to a sattellite dataset with a trendline drawn from 1998 until today. Often the set is cropped to start in 1998 as well to undermine the perception of the long-term trend. A typical example is this one from [Climate Depot](http://www.climatedepot.com/2015/09/02/a-new-record-pause-length-satellite-data-no-global-warming-for-18-years-8-months/). My argument is that the trend from 1998 until today is not robust, a point that has probably been made many times, but that I wanted to make myself. 

I downloaded the Remote Sensing Systems (RSS) global mean lower troposphere temperature anomaly [dataset](http://data.remss.com/msu/graphics/TLT/time_series/RSS_TS_channel_TLT_Global_Land_And_Sea_v03_3.txt) (I wanted to use the UAH set, but I couldn’t get the site open that evening). Using Python and Pandas, I did a rudimentary trend analysis to see how robust the trend from 1998 until the end of the data set really is. The trend lines with different starting years are shown in 

![RSS trend lines](https://raw.githubusercontent.com/hansbrenna/RSS_trend_analysis/master/trendlines.png)
> Figure 1: The RSS global mean lower troposphere temperature (TLT) with trendlines calculated based on different starting times.


![RSS trend is not robust](https://raw.githubusercontent.com/hansbrenna/RSS_trend_analysis/master/trends.png)
