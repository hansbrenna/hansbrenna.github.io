---
layout: post
title: "From climate forecast to carbon budgets – Unfounded probabilities at the heart of climate science."
description: ""
category: commentary
tags: [commentary, carbon budgets, climate modeling, interpretation, probabilistic prediction]
---
{% include JB/setup %}

# [From climate forecast to carbon budgets – Unfounded probabilities at the heart of climate science.](http://hansbrenna.github.io/commentary/2017/01/25/From-climate-forecast-to-carbon-budgets)

The stated goal of world climate policy is to avoid dangerous levels of global warming. This point is often, somewhat arbitrarily, defined as 2°C above preindustrial temperatures. In the context of the Paris agreement, the ambition is 1.5°C. No matter what the limit is, we need some way of knowing if we’re going to exceed the warming limit or not. The answer in the last years has been whats called cumulative carbon emission budgets or, often, just carbon budgets.

Cumulative carbon emission budgets are one of the most important and policy relevant results that come out of attempts to quantify future climate change. A carbon budget is an attempt to give information about how much greenhouse gases human society can emit without exceeding some target temperature (e.g. 2°C) to some accepted likelihood (e.g. 33%). This is a multi-faceted problem and there is no one correct way of making a budget, nor is there a single accepted target temperature or exceedance likelihood. 

The free parameters when making a budget are: Which forcing agents to include in addition to CO2, which type of budget to make, which target warming to aim for at which time with which probability. All of these choices impact significantly on the size of the allowed budget.

To inform policy based on emission budgets, the general approach is to derive emission scenarios that are deemed societally possible and compatible with the budget. Here, another complication emerges: If the budget is exceeded to a moderate extent, the nature of the climate system’s response to CO2 makes it possible to remove excess CO2 after it was emitted and still hit the target temperatures. This makes the range of specific emission scenarios that are compatible with a given budget very large, and the choice of how to limit the scenarios considered plausible is important when giving policy advice based on emission budgets.

The freedom inherent in the process of formulating emission budgets combined with their seeming simplicity and ease of comparison to reserves of fossil fuels have made many groups see the potential of emission budgets as strategic communication tools, and there is potential for misuse with the aim of cynically subvert policy action. This means that when seeing emission budgets used in public discourse, a certain amount of skepticism is in order. 

This is a serious problem in itself, but a more fundamental problem with the emission budget concept seems to be more-or-less unexplored: Do cumulative carbon emission budgets have a sound scientific foundation?

In this essay, I will explore an argument with the goal of showing that a specific type of carbon budgets derived in the IPCC 5th assessment report (AR5) (IPCC, 2013)⁠  are scientifically unfounded and that this argument also applies to other types of budgets. I will then briefly explore what this means for the scientific content of the carbon budgets and if different ways of making cumulative budgets can salvage the concept. 

## 1. From climate forecast to emission budget

There is a straight-forward way to derive a useful type of carbon budget directly from a model forecast of future climate. I will go through the required steps in some detail.

A climate forecast consists of a set of forcings and a set of climate models. The forcings consist of the external parameters that drive the state of the climate system and would, for the future, consist of educated guesses. The most important factors are anthropogenic emissions of greenhouse gases, land use changes and emissions of aerosols. For model forecasts, natural forcings are usually considered constant due to lack of foreknowledge. Figure 1a illustrates some forcing scenarios expressed in radiative forcing.

By applying the set of forcings to the set of climate models, the result is a range of climate scenarios, generally called projections. These are our best guesses of how the climate would change if the corresponding forcing scenario became true. Figure 1b illustrates the  range of modeled change given the scenarios in Figure 1a.

One of the major efforts for the fifth IPCC AR5 was the Coupled Model Intercomparison Project phase 5 (CMIP5) (Collins et al., 2013)⁠. This project used a compiled set of emission and forcing scenarios called the Representative Concentration Pathways (RCP) to drive a group of the most complex climate available, so-called Atmosphere Ocean General Circulation Models. These models are developed by several groups around the world and share a complicated family tree of model development. The forcings and model simulations of the future are together called the CMIP5 ensemble and are what is shown in Figure 1a and b.

As Figure 1c shows there is an approximately linear relationship between total cumulative carbon emissions and the resulting warming. The exact relationship is weakly dependent on the actual emission scenario simulated and strongly dependent on the specific model, resulting in a large modeled range, but small differences between the multi model means from the different emission scenarios. 

![Illustration of how threshold exceedance budgets can be made from climate model output](https://raw.githubusercontent.com/hansbrenna/hansbrenna.github.io/master/assets/img/CMIP5_illustration.png)
*Figure 1: a) The four RCP scenarios, developed for the AR5, expressed in radiative forcing. b) The evolution of the global average surface tempereture to the RCP scenarios in the CMIP5 ensemble (figure TS.15 in (Stocker et al., 2013)⁠.) c) Global warming as function of cumulative CO2 emissions. The dashed line represents cumulative emissions in 2010. The solid black lines represent a simple estimate of a cumulative carbon budget for 2C warming (Modified from Figure 2.3 from  (IPCC, 2014)⁠).*

If we were certain that the ensemble mean warming represents the real climate systemt we could read out from figure 1c at which cumulative carbon emission we could expect to cross this threshold. But we cannot be sure that the ensemble mean represents the true warming. By  interpreting the model ensemble probabilistically we can make an emission budget to a given probability and the simplest way to do this is to treat each model as an equally reasonable representation. 

Armed with our model ensemble projection, a temperature limit (2°C), exceedance likelihood (33%) and our “one model, one vote” ensemble interpretation, we find the cumulative carbon emission where approximately 33% of our modeled realizations have warmed more than 2°C. In Figure 1c, a quick estimate of this value is marked by the intersection of the black lines. By this estimate, somewhat more than 1000 Gt of additional CO2 can be emitted after 2010 before crossing the 2°C threshold with 33% probability. This type of budget is called a Threshold Exceedance Budget (TEB) and the number we found is in close agreement with the more detailed analysis considered in the IPCC AR5 (Collins et al., 2013)⁠. 

We have derived a cumulative emission budget that tells us at which cumulative emissions we exceed our accepted likelihood of crossing 2°C warming. A policy response to this budget could be to find pathways for limiting global cumulative emissions below about 1000 GtCO2 in the period 2010-2100. 

If this budget was unanimously accepted as the guiding principle of global climate policy and stringent action was taken to limit emissions to 1000 GtCO2, could we be reasonably certain that warming would be limited below 2°C? Alas, to this question, we must answer: No.

## 2. Fundamental soundness of threshold exceedance budgets

The central assumption behind the TEB  we have found is the probabilistic interpretation of the CMIP5 ensemble. Let’s explore this interpretation in more detail. 

Interpreting multi model ensemble climate forecasts has been studied in both the climate scientific literature (Stainforth et al., 2005; McWilliams, 2007; Knutti, 2008; Collins et al., 2013)⁠and the literature on the philosophy of computer simulation (Parker, 2006, 2010, Betz, 2009a, 2009b, 2010, 2015; Katzav, 2013)⁠. Why do we have so many climate models in the first place? Climate models suffer from the related problems of structural uncertainty and parametric uncertainty. When designing a climate model, the modeler has to make many choices. Often there is more than one way of representing am important process, and choosing which one to incorporate usually involves  trade-offs, or even a level of scientific arbitrariness (1). The results is called structural uncertainty in the models (McWilliams, 2007; Parker, 2010)⁠. Even when the representation of all included processes is decided the models include many parameters that are only weakly constrained by other data, meaning there is parametric uncertainty (2) (McWilliams, 2007; Betz, 2009a; Parker, 2010; Katzav, 2013)⁠. It is generally possible to fit every plausibly formulated model, and even different versions of the same model, equally well to the observed climate of the past and present. The consequence of these problems is that there is no objective way of ranking the climate models from best to worst and every climate model should be treated as equally plausible. Does this justify our “one model one vote” interpretation?

The CMIP5 ensemble does not span the space of either parametric uncertainty or structural uncertainty in a thorough or strategic way; it is an ensemble of opportunity. Based on model data alone, we cannot assign a probability to even being in the modeled range at a given time in the future, and by extension we cannot assign probabilities to individual realizations. Each climate simulation is only a statement about what is possibly true in the real climate system and even though we can do no better than treating the models equally, they can not be interpreted probabilistically (Betz, 2009a; Parker, 2010)⁠. This is a well known problem, and the IPCC AR5 acknowledges it several times (Collins et al., 2013; Stocker et al., 2013)⁠. Still this unfounded probabilistic interpretation is at the heart of making threshold exceedance budgets.

Is there a way to salvage the TEB concept? We could, of course, use other knowledge about the climate system to rule out evolutions that are inconsistent with our background knowledge, but, at best this gives us upper and lower limits. On the interpretation of the CMIP5 ensemble, the IPCC states that the CMIP5 5-95% range is considered the likely (66%)(3) range of future warming (Collins et al., 2013)⁠. Thus the upper and lower limits provided by other knowledge does not really constrain our modeled range. Even if we were able to constrain the ensemble range, the remaining plausible range could still not be interpreted probabilistically. 

The question then is: What is the new scientific content in the CMIP5 ensemble simulations compared to the rest of our knowledge about the climate system? Concerning global scale temperature change the answer must be: Very little.(4) We can not assign probabilities to being within the model range or to any individual projection. Any upper or lower limits come from other sources of knowledge. Thus the CMIP5 ensemble data is empty of scientific content at the global scale, any emission budget derived from this data is equally empty, and, it seems, the TEB concept is dead.

## 3. Is it possible to salvage emission budgets?

There are two other main types of emission budgets called Threshold Avoidance Budgets (TAB) and CO2-only budgets. Threshold Avoidance Budgets estimates the cumulative emissions that leads to peak warming lower than the threshold to a given probability (Rogelj et al., 2016)⁠. These budgets give the lowest estimates of allowed emissions and are the simplest to convert into policy advice, but they suffer from the same problem of probabilistic interpretation as TEBs since they are dependent on simple climate models with uncertainty ranges calibrated to the CMIP5 ensemble.

The CO2-only budget is represented in Figure 1c by the gray shaded area, and is on a stronger scientific foundation since the upper and lower limits of the warming can be estimated from background knowledge (Rogelj et al., 2016)⁠. Still, if we attempt to derive probabilistic budgets from this data we immediately run into the same problems again. In addition, the CO2-only budget is of limited policy value since it by definition neglects many important forcing agents and is expected to significantly underestimate the warming. 

In summary, all presently used carbon budget methodologies are based on a severely flawed interpretation of ensemble climate forecasts, and I see no way of salvaging the concept as it is presently understood. 

## 4. Carbon budgets as pure communications tools

A significant amount of energy is expended on making emission budgets, arguing about them and designing policy pathways consistent with them. For most scientists, activists, decision makers and people in general I believe this is because they sincerely believe that emission budgets are scientifically sound. But the value of cumulative emission budgets as strategic communications tools has been recognized by many groups. One example is the organization Oil Change International which argues that most remaining fossil fuel reserves has to be left in the ground to keep below 2°C on the basis of cumulative emission budgets (Oil Change International, 2016)⁠. Another is the Norwegian Oil and Gas Association arguing that oil and gas will be an important energy source after 2050 on the basis of another budget consistent with 2°C (KonKraft, 2016, p. 15)⁠. These two examples differ in their exceedance/avoidance probability (33% vs. 50%) and their use of technologically achieved net removal of CO2 from the atmosphere after 2050. 

Thus it seems almost every point of view can be argued based on a strategically formulated carbon budget, and the main value of the budgets are as communication tools, giving views with widely different and incompatible policy implications a similar standing in the public discourse. When discussing climate policy in the public sphere it is very hard to communicate the caveats associated with each emission budget, even if assuming that the budgets are scientifically sound. 

## 5. Summary and conclusions

I have attempted to establish that emission budgets of the policy relevant type are scientifically unsound, and I believe the argument is successful. My opinion is that probabilistically formulated budgets should be discarded by groups advocating action on carbon emissions. The risk of continuing to base the argumentation on emission budgets is that they communicate a false certainty to society and policy makers leading to policies that seem to be based on scientifically derived probabilities, but are really just statements about what is possibly true. It is not certain that present emission budgets overestimate allowed emissions, but the chance of this can not be probabilistically quantified. 

In the present, if formulating emission limits for policy advice, we should avoid the use of probabilistic language and we should use background knowledge to specify an upper limit of cumulative emissions which is compatible with almost certainly keeping warming below 2°C (or 1.5°C in the framework of the Paris Agreement). For the near future the uncertainty in climate prediction justifies choosing polices that guide us towards net negative emissions as quickly as possible and the stabilization of atmospheric greenhouse gases at levels significantly lower than today.(5)

A main focus for climate science in the coming years should be to use whatever methods are available to try to limit the range of uncertainties in key climate variables like the climate sensitivity and transient climate response. The use of physical arguments to rule out regions of parameter space looks particularly promising, but it’s important to be careful not to introduce new unfounded probabilities (Stevens et al., 2016)⁠.

## Notes

When designing the Norwegian Earth System Model (NorESM), instead of starting from scratch, the modeling groups took the atmosphere model (called CAM) from the climate model called CESM, an ocean model originating from the MICOM model and the carbon cycle model HAMOCC from Germany. The atmosphere model is significantly modified with respect to CAM regarding which processes to include to what detail.

For a spectacular illustration of parametric uncertainty, see the climateprediction.net project. Here thousands of different plausible parameter values for the same climate model were simulated. The resulting range of climate sensitivity spanned more than 10C.

Whether or not this probability is well founded or not is outside the scope of this essay.

On sub-global scales the answer is not so pessimistic, since the only way to get specific knowledge about regional and local scales is to self-consistently simulate the climate system at these scales. The CMIP5 ensemble can say something about changes and consequences on these scales that can not be derived from our general background knowledge. Still, assigning probabilities to these statements is unfounded.

As long as global climate policy is supposed to be based on the precautionary principle, this is the only justifiable course of action in my opinion.

## References
Betz, G. (2009a) ‘Underdetermination, model-ensembles and surprises: On the epistemology of scenario-analysis in climatology’, Journal for General Philosophy of Science. Springer Netherlands, 40(1), pp. 3–21. doi: 10.1007/s10838-009-9083-3.

Betz, G. (2009b) ‘What range of future scenarios should climate policy be based on? Modal falsificationism and its limitations’, Philosophia Naturalis, 46(1), pp. 133–158. doi: 10.3196/003180209791291918.

Betz, G. (2010) ‘What’s the Worst Case? The Methodology of Possibilistic Prediction’, Analyse & Kritik, 32(1), pp. 87–106. doi: 10.1515/auk-2010-0105.

Betz, G. (2015) ‘Are climate models credible worlds? Prospects and limitations of possibilistic climate prediction’, European Journal for Philosophy of Science. Springer Netherlands, 5(2), pp. 191–215. doi: 10.1007/s13194-015-0108-y.

Collins, M., Knutti, R., Arblaster, J., Dufresne, J.-L., Fichefet, T., Friedlingstein, P., Gao, X., Gutowski, W. J., Johns, T., Krinner, G., Shongwe, M., Tebaldi, C., Weaver, A. J. and Wehner, M. (2013) ‘Long-term Climate Change: Projections, Commitments and Irreversibility’, in Climate Change 2013: The Physical Science Basis. Contribution of Working Group I to the Fifth Assessment Report of the Intergovernmental Panel on Climate Change, pp. 1029–1136. doi: 10.1017/CBO9781107415324.024.

IPCC (2013) Climate Change 2013: The Physical Science Basis. Contribution of Working Group I to the Fifth Assessment Report of IPCC the Intergovernmental Panel on Climate Change. Edited by T. F. Stocker, D. Qin, G.-K. Plattner, M. M. B. Tignor, S. K. Allen, J. Boschung, A. Nauels, Y. Xia, V. Bex, and P. M. Midgley. Cambridge University Press.

IPCC (2014) Climate Change 2014: Synthesis Report. Contribution of Working Groups I, II and III to the Fifth Assessment Report of the Intergovernmental Panel on Climate Change. Edited by Intergovernmental Panel on Climate Change. Cambridge: Cambridge University Press. doi: 10.1017/CBO9781107415324.

Katzav, J. (2013) ‘Hybrid models, climate models, and inference to the best explanation’, British Journal for the Philosophy of Science, 64(1), pp. 107–129. doi: 10.1093/bjps/axs002.

Knutti, R. (2008) ‘Should we believe model predictions of future climate change?’, Philosophical transactions. Series A, Mathematical, physical, and engineering sciences, 366(1885), pp. 4647–4664. doi: 10.1098/rsta.2008.0169.

KonKraft (2016) Klima - norsk sokkel i endring. Available at: https://www.norskoljeoggass.no/Global/2016 dokumenter/Klima norsk sokkel i endring.pdf.

McWilliams, J. C. (2007) ‘Irreducible imprecision in atmospheric and oceanic simulations’, Proceedings of the National Academy of Sciences. National Academy of Sciences, 104(21), pp. 8709–8713. doi: 10.1073/pnas.0702971104.

Oil Change International (2016) The sky’s limit. Available at: http://priceofoil.org/content/uploads/2016/09/OCI_the_skys_limit_2016_FINAL_2.pdf.

Parker, W. S. (2006) ‘Understanding pluralism in climate modeling’, Foundations of Science, 11(4), pp. 349–368. doi: 10.1007/s10699-005-3196-x.

Parker, W. S. (2010) ‘Predicting weather and climate: Uncertainty, ensembles and probability’, Studies in History and Philosophy of Science Part B - Studies in History and Philosophy of Modern Physics. Elsevier, 41(3), pp. 263–272. doi: 10.1016/j.shpsb.2010.07.006.

Rogelj, J., Schaeffer, M., Friedlingstein, P., Gillett, N. P., van Vuuren, D. P., Riahi, K., Allen, M. and Knutti, R. (2016) ‘Differences between carbon budget estimates unravelled’, Nature Climate Change. Nature Research, 6(3), pp. 245–252. doi: 10.1038/nclimate2868.

Stainforth, D. A., Aina, T., Christensen, C., Collins, M., Faull, N., Frame, D. J., Kettleborough, J. A., Knight, S., Martin, A., Murphy, J. M., Piani, C., Sexton, D., Smith, L. A., Spicer, R. A., Thorpe, A. J. and Allen, M. R. (2005) ‘Uncertainty in predictions of the climate response to rising levels of greenhouse gases.’, Nature. Nature Publishing Group, 433(7024), pp. 403–6. doi: 10.1038/nature03301.

Stevens, B., Sherwood, S. C., Bony, S. and Webb, M. J. (2016) ‘Prospects for narrowing bounds on Earth’s equilibrium climate sensitivity’, Earth’s Future. Wiley Periodicals, Inc. doi: 10.1002/2016EF000376.

Stocker, T. F., Dahe, Q., Plattner, G.-K., Alexander, L. V., Allen, S. K., Bindoff, N. L., Bréon, F.-M., Church, J. A., Cubash, U., Emori, S., Forster, P., Friedlingstein, P., Talley, L. D., Vaughan, D. G. and Xie, S.-P. (2013) ‘Technical Summary’, Climate Change 2013: The Physical Science Basis. Contribution of Working Group I to the Fifth Assessment Report of the Intergovernmental Panel on Climate Change, pp. 33–115. doi: 10.1017/ CBO9781107415324.005.