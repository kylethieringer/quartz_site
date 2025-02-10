---
title: neurons with stereotyped functions are still context dependent
publish: "true"
timestamp: 2023-12-11 09:35
tags:
  - 🥚
  - 🌱
---
when performing open loop optogenetic experiments, we often look at probability of a behavior around a stimulus onset. However, the current state of the animal, which behaviors it's performing, etc. all impact the stimulus effect. These confounds change whether neurons drive specific behaviors, even when neurons have accepted stereotypic functional roles for behavior.

For example, [[Cande.etal2018]] use [[mutual information]] as a metric to determine how much the behavior before an opto stimulus explains the behavior during the opto stimulus. (high mutual info = high context dependency). All of the neurons they tested (split gal4 descending neuron lines) show some amount of mutual information - meaning they all have some context dependency. And these are neurons widely accepted to drive stereotyped behavior!

fear : what are we missing in open loop opto experiments?
joy : behavior is complex and variable and I find this result more interesting than thinking about neural activity as binary readout of behavior

#🥚 | #🌱 
## references
---
[[Cande.etal2018]]