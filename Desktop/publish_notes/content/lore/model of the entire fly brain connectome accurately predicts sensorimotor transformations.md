---
title: model of the entire fly brain connectome accurately predicts sensorimotor transformations
publish: "true"
timestamp: 2023-12-11 09:35
tags:
  - 🌱
  - 🐛
---
using a leaky-integrate and fire model, with every neuron in the fly brain as input (~125,000 neurons), the pathway from sensory input to motor output is fairly accurately predicted. the results were replicated using both the sugar sensing to proboscis extension pathway and the antennal grooming pathway. Not only were the neurons identified but the necessity and sufficiency was also determined through activating and silencing individual neurons in the model, and confirmed later through behavioral experiments. 


> [!info] fig 4a,b,c
> ![[shiu_etal2023_fig4abc.png]]
> 

in their model, they activate all water or sugar GRNs then record the response individually of every other neuron. A shows top 200 responsive neurons. Then they activate all other neuron and measure activity of MN9 (motor neuron that drives proboscis extension) to see which are sufficient. then activating all water GRNs while individually silencing the top 200 other neurons to see which are necessary for MN9 activation.

#🐛 | #🌱 
## references
---
[[Shiu.etal2023]]