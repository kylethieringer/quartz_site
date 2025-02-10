---
paper_title:
  - Theory of coupled neuronal-synaptic dynamics
title: Clark.Abbott2023
year: "2023"
authors: David G. Clark, L. F. Abbott
type: literature note
note date: 2023-09-28
modified: 
summary: theory of scale jumping, discussing how synaptic plasticity happens on multiple timescales for synapses and neurons and they act in a dynamical system. Offers a new framework of plasticity called freezable chaos.
tags:
  - 📚
status: true
publish: "true"
timestamp: 2023-12-11 01:13
---
# Theory of coupled neuronal-synaptic dynamics
**authors**: David G. Clark, L. F. Abbott
**doi**: 
**zotero link**: [arXiv Fulltext PDF](zotero://select/groups/5209539/items/EGD9BFXU)

> [!INFO] CITATION
> Clark, D. G., & Abbott, L. F. (2023). _Theory of coupled neuronal-synaptic dynamics_ (arXiv:2302.08985). arXiv. [http://arxiv.org/abs/2302.08985](http://arxiv.org/abs/2302.08985)

> [!NOTE] ABSTRACT
>In neural circuits, synapses influence neurons by shaping network dynamics, and neurons influence synapses through activity-dependent plasticity. Motivated by this fact, we study a network model in which neurons and synapses are mutually coupled dynamic variables. Model neurons obey dynamics shaped by synaptic couplings that fluctuate, in turn, about quenched random strengths in response to pre- and postsynaptic neuronal activity. Using dynamical mean-field theory, we compute the phase diagram of the combined neuronal-synaptic system, revealing several novel phases suggestive of computational function. In the regime in which the non-plastic system is chaotic, Hebbian plasticity slows chaos, while anti-Hebbian plasticity quickens chaos and generates an oscillatory component in neuronal activity. Deriving the spectrum of the joint neuronal-synaptic Jacobian reveals that these behaviors manifest as differential effects of eigenvalue repulsion. In the regime in which the non-plastic system is quiescent, Hebbian plasticity can induce chaos. In both regimes, sufficiently strong Hebbian plasticity creates exponentially many stable neuronal-synaptic fixed points that coexist with chaotic states. Finally, in chaotic states with sufficiently strong Hebbian plasticity, halting synaptic dynamics leaves a stable fixed point of neuronal dynamics, freezing the neuronal state. This phase of freezable chaos provides a novel mechanism of synaptic working memory in which a stable fixed point of neuronal dynamics is continuously destabilized through synaptic dynamics, allowing any neuronal state to be stored as a stable fixed point by halting synaptic plasticity. 


- computations in circuits are typically thought about in dynamics of neurons, where synapses just shape the dynamics of each neuron
	- however synapses have much more dynamic range on different timescales on their own
	- therefore we must think of neurons and synapses as coupled systems in circuits
- there are consequences however if we assume these are coupled systems without separate timescales

- machine learning models view networks in the view that synapses sculpt neurons
	- weight parameters are learned through gradient descent
	- allowing weights to change based on activity of artificial units is beneficial (like how plasticity in circuits work)

- machine learning models that use plasticity like weight dynamics often share features
	- weights are not fully plastic, but sum of static component, trained by backpropagation and a plastic component
	- plasticity is hebbian

- inclusion of fast timescale coupling dynamics in machine learning models
	- can have non intuitive implications on the network
	- dynamic phase that the authors call freezable chaos
		- a stable fixed point of neuronal dynamics is destabilized generating neuronal synaptic chaos, which can create a synaptic working memory by halting synaptic plasticity

- the model the authors use is an adaptation of a random network model of Sompolinsky et al but adds dynamic couplings

[[freezable chaos is a novel network model of plasticity]]
	- in the default state, the network produces unstructured and spontaneous activity (chaos)
	- plasticity's role in this model is to destabilize a neuronal fixed point which allows the state to remain dynamic
	- activity pattern is stored (working memory) by abruptly halting synaptic plasticity (freezing)

- Advantages of this model over traditional short term synaptic facilitation (STF) models
	- in STF based memory, static connections in predefined assemblies of neurons are sustained for period of time
		- in freezable chaos, any network state can be stored allowing for more flexibility
	- in STF, stored activity decays unless provided reactivation input
		- in freezable chaos, fixed point can be stored indefinitely
	- in STF, there is a forgetting timescale of plasticity
		- in freezable chaos, circuit returns to dynamical state whenever the plasticity is released which can allow for temporally flexible computations
- 

%% Import Date: 2023-09-28T11:34:12.353-07:00 %%
