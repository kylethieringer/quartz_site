---
title: a maximum entropy model predicts behavior without assumptions or free parameters
tags:
  - 🥚
  - 🌱
publish: "true"
timestamp: 2023-12-11 01:12
---

the maximum entropy model is constructed by finding the individual characteristic in a group, for example, velocity of each bird. It is then normalized (like z-scoring?). the normalized values can all be drawn from the probability distribution of the entire group (all of the possible values an individual can have). then measure the correlations between the normalized values of each individual in the group. there will be infinite possibilities of distributions that can make up that correlation (by definition I think?). However only one distribution is the "most random" that still matches the experimental data, which can then be used to test hypotheses. [[maximum entropy model lacks free parameters]] so you dont need to fit the model, just predict

see the paper for a better description of this model...

[[example implementation of maximum entropy model]]


#🥚 | #🌱
## references
---
[[Bialek.etal2012]]