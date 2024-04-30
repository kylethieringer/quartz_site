---
title: § population constraints on individuals
publish: "true"
timestamp: 2023-12-20 16:40
tags:
  - 🐛
---
## project overview

Canonically, when approaching systems neuroscience questions, we often take a bottom up approach. This approach considers a single player and positioning it within the rest of the population. Consider a flock of starlings that display beautiful murmurs:

(https://youtu.be/UVko9jyAkQg?t=57)
![video](https://youtu.be/UVko9jyAkQg?t=57)

We can model the behavior of these flocks fairly well with very few parameters ([[Bialek.etal2012]]), using just the interaction of one bird with its neighboring birds, to explain much of the spontaneity of this system. What these models lack, however, is the explanation of how the flock constrains the flight of any given bird. On a completely different scale, we can activate [[descending neurons]] in a fly to drive behaviors or silence the neurons to test necessity of the neuron for that behavior ([[Cande.etal2018]]). However there is variability in response to these single neuron perturbations ([[Zacarias.etal2018]]) which indicates something more broadly constrains the outcome of one individual's effect on the population. On the synaptic level, we can consider the duality of interactions on different scales through the separate but coupled dynamic range of activity between neurons and synapses ([[Clark.Abbott2023]]).

To begin studying population constraints on individuals, I will use the auditory system in the fly. There has been a tremendous amount of work characterizing responses of JONs and second order neurons to both mechano stimuli and auditory stimuli ([[Baker.etal2022]]). the auditory network in the fly brain is densely connected and highly recurrent. this offers a unique opportunity to ask how the auditory population of neurons constrains any individual neuron in the network. 

the initial approach is to activate a candidate auditory neuron while recording calcium activity in the rest of the brain. we expect to see a mix of responses, some neurons don't respond, some respond very strongly, and others may have a variable response. this last group may be the most interesting to understand what parameters of the network dictate the faculty of the candidate neuron. we can represent the network in a low dimensional space and look at the trajectory of activity ([[Kato.etal2015]]). how does changing the network change the trajectory in this low dimensional space? we can disrupt population dynamics through neuromodulation, knocking down specific receptors or manipulating important enzymes in intercellular signaling pathways. we can study increased population activity during locomotion or other "internal states" (in quotation marks because I think this is a neuroscience buzz word). we may expect a number of outcomes when looking at the trajectory in this low dimensional space. Maybe there is no change in trajectory, and the network is deterministic. Or, maybe by changing the population, we change the parameters that constrain the individual and the trajectories are driven to one specific place in the low dimensional space. By answering these questions we gain more comprehensive understanding at the fundamental mechanisms and parameters of neural systems that ultimately drive the complexity of animal behaviors.


#🐛 | [[⨳ projects]]