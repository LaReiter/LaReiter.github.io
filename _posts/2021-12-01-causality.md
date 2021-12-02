---
title: "Behind every smart machine, is a smart human"
mathjax: true
layout: post
categories: media
---

![ML](/assets/ml.png)

In 2008, Google launched a spectacular project called Google Flu Trends (GFT). The program was devised to collect search queries from users of their search engine, in order to predict the outbreaks of flu.
It was a tremendous success, until it wasn’t anymore. From its birth in 2003 and up till the year of 2009 GFT had accurately predicted the outbreak of Flu several days in advance. 
You could almost hear the apostles of big data chant in unison: “The era of the machine has begun”.

Then came the swine flu in the spring 2009, and GFT was beaten. But why?

We know that Google trained the program between 2003 and up to 2008, in order to narrow down the search queries (45 was found) which correlated with the flu outbreak over this period. What was also the case in this 7 year period, was that flu outbreaks (in the U.S. where the program was trained) always started in the winter.
One has to wonder, if GFT in fact was a ingenious model to predict the coming of winter. 
After its failure in 2009, GFT was updated, but failed once again in 2012-2013 with a heavy overestimation of the flu outbreaks. In 2015 GFT was ended. Also in 2009, Google had introduced its suggested query function. It is speculated that this function could potentially boost the queries for flu-related searches, hence resulting in a overly optimistic (or pessimistic) flu prediction.

![SQ](/assets/sq.png)

There are many speculations as to why GFT ended as a fallen star. But what seems to be beyond discussion, is that causation is at the core of the problem. 
We simply, do not know enough about the causal structure behind the search pattern of individuals. 
In particular, we do not know if correlations are in fact causations, and if the past correlations are only ‘by chance’, such that future realizations will not promote the same set of search queries as predictors.

## Big data. Deep learning. Artificial intelligence.

These are words that can spark up enthusiastic conversations. And for good reason, the possibilities are endless: Self-driving vehicles. Image segmentation for locating pathologies, including cancer. Automatization across sectors. And so much more.
In fact, the possibilities are so enormous, that if we are not careful, we might not even see the limitations. As the GFT example showed.
One of the issues to be addressed in machine learning, is the intrinsic ‘black-box’ nature of algorithms, or as I like to call it “fitting incomplete pieces”-paradigm, stretching our lack of knowledge w.r.t. Causality.

## Making decision from incomplete or biased data
> "If you feed your machine garbage data, it will give you garbage results"

In supervised learning, a machine (program) is trained to make good predictions. In order to train the machine, we collect real world data and use (a subset of) the data to validate the performance.
In the background of this learning process is a key assumption, namely that the data needs to be i.i.d (= Independent and identically distributed). It means that, any instance of our data needs to follow the same probability distribution and be non-influenced by previous observations. In reality this is not the case. 
For uncountable many reasons, new data can be corrupted, resulting in non-identical data (compared to the training data). If we have knowledge about the corruption, it is possible that it can enter our model as a ‘feature’ which will alleviate the problem, since it now enters into the distribution of our data.
But in practice, there are too many ways that external factors could influence the distribution.  
As another example, say you are training a missile program to recognize a military vehicle based on a million military vehicles in broad daylight. When satisfied with its performance, you are ready to apply it during a night-time mission. The result is catastrophical, and the missile does not hit its intended target. What happens, is that during day-time, the pixel pattern of vehicle images follows one distribution, whereas night-time adds corruption (blurred images), hence the pattern of vehicles in night-time follows another distribution. Thus we train our machine on data from one distribution, and inputs data from another distribution on the mission, using a prediction-rule based on the training data, resulting in a rogue missile.

## Can we fix it?

One would argue that we just need to expand our feature set, or equivalently sample more different data. In the example above, this would certainly help. But the issue arise, when we don’t know a priori what data is meaningful in the context of the machine learning problem. Such as with the GFT example.
Can we fix it? This is one of the hot topics within data science, and a active field of research. Integrating causality, implies the possibility of adaption to new settings. For instance, a machine which could recognize the influence of “night-time”, even though it has not been explicitly served with data from this distribution. 
We humans make causal reasoning all the time, and it is in part what makes us conscious and intelligent. The perspective of a machine with the same rational state, is something that I believe would make even the most skeptical of us chant with the big data apostles.

