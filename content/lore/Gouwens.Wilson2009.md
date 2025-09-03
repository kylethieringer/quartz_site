---
paper_title: Signal Propagation in <i>Drosophila</i> Central Neurons
year: "2009"
authors: Nathan W. Gouwens, Rachel I. Wilson
type: literature note
note date: 2025-04-27
modified: 
summary: 
tags: 
status: 
title: Gouwens.Wilson2009
publish: "true"
timestamp: 2025-06-01 15:51
---
# Signal Propagation in <i>Drosophila</i> Central Neurons
**authors**: *Nathan W. Gouwens, Rachel I. Wilson*
**doi**: 10.1523/JNEUROSCI.0764-09.2009

> [!INFO] CITATION
> Gouwens, N. W., & Wilson, R. I. (2009). Signal Propagation in _Drosophila_ Central Neurons. _The Journal of Neuroscience_, _29_(19), 6239–6249. [https://doi.org/10.1523/JNEUROSCI.0764-09.2009](https://doi.org/10.1523/JNEUROSCI.0764-09.2009)

> [!NOTE] ABSTRACT
>Drosophila is an important model organism for investigating neural development, neural morphology, neurophysiology, and neural correlates of behaviors. However, almost nothing is known about how electrical signals propagate in Drosophila neurons. Here, we address these issues in antennal lobe projection neurons, one of the most well studied classes of Drosophila neurons. We use morphological and electrophysiological data to deduce the passive membrane properties of these neurons and to build a compartmental model of their electrotonic structure. We find that these neurons are electrotonically extensive and that a somatic recording electrode can only imperfectly control the voltage in the rest of the cell. Simulations predict that action potentials initiate at a location distant from the soma, in the proximal portion of the axon. Simulated synaptic input to a single dendritic branch propagates poorly to the rest of the cell and cannot match the size of real unitary synaptic events, but we can obtain a good fit to data when we model unitary input synapses as dozens of release sites distributed across many dendritic branches. We also show that the true resting potential of these neurons is more hyperpolarized than previously thought, attributable to the experimental error introduced by the electrode seal conductance. A leak sodium conductance also contributes to the resting potential. Together, these findings have fundamental implications for how these neurons integrate their synaptic inputs. Our results also have important consequences for the design and interpretation of experiments aimed at understanding Drosophila neurons and neural circuits. 
>  
## fleeting notes
---
%% begin notes %% 
almost nothing is known about how electrical signals propagate in flies
investigate antennal lobe PNs

find the passive membrane properties of neurons and build compartmental model

recording from soma is imperfect in controlling the rest of the cell

action potentials initiate away from soma

insect neuron morphology
- soma separated from rest of cell by long neck of membrane
- action potentials traveling to spike initiation zone bypass the soma - signals often propagate poorly from the dendrites

the resting potential sets the driving force for synaptic currents 
- controls the activation of voltage gated conductances

focusing on understanding the electrical properties of antennal lobe PNs because they have been studied extensively for development and morphology and connectivity
- recordings can be made from functionally equivalent PNs in different experiments with GFP

use a model to predict membrane voltage at inaccessible locations 
Questions:
1) how effectively can a somatic electrode control the voltage throughout the cell? 
2) where in the cell do spikes initiate? 
3) how well do synaptic events propagate from the dendrite

the soma is the only location on a cell that can be patched
action potentials recorded at the soma are only 5-15mV
- action potentials are usually more than 40mV so this suggests that spikes are not initiated near the soma
- hyperpolarizing soma below -70mV does not suppress spontaneous firing -- suggesting that soma is distant from spike initiation

created a model of one of the PNs with varying dendritic densities
determined membrane parameters using electrophys - brife square pulses of current and recording membrane potential responses
adjusted model params to fit these data

injected white noise to see how cell would respond to different frequencies of current injection
- model accurately predicted responses to white noise

how does signal propagate?
- using model found that voltage changes at soma do propagate to dendrite and axon but attenuated
- most of this happens at primary neurite
- recorded from 3 neurons and fit 3 models. then looked at signal propagation in these three cells. they were all different but physiologically possible. All showed most attenuation at neurite
- changing dendrite density did not change propagation

[[the initial segment of a fly neuron is located where the primary neurite splits]]

where is the SIZ?
- modeled neuron and found that the best fit of clamping membrane potential at different sites was when spike initiated near start of axon where the primary neurite splits into axon and dendritic branches

[[synaptic connections between neurons span many dendritic branches]]

modeled unitary synapses potentials are insufficient to drive unitary EPSP that match data at the soma
- this suggests that synaptic connections between neurons are on multiple dendritic branches
- modeled single input neuron distributing release sites onto multiple branches and this fit data well
- EPSPs do no cause substantial voltage changes in axon terminals - action potentials are necessary for synaptic output

what is resting membrane potential of fly neurons
- measured firing rate in cell attached (tight seal but not rupturing membrane) and in whole cell (tight seal then break into cell)
- rupturing membrane caused increased spiking rate - indicating this depolarizes cell

- had to hyperpolarize the membrane about 10mV to recapitulate cell attached firing rate

why does cell depolarize when you break in?
- change happens very fast - so probably not dialysis from pipette solution

drosophila neurons are small and have high input resistances
- as input resistance approaches seal resistance, current flow through seal resistance has proportionately larger effect

resting potential is very depolarized compared to potassium reversal potential
- used slow voltage clamp commands to estimate resting potential by finding when there was zero net current flowing
- lowering external sodium concentration hyperpolarized resting potential by 10mV
	- suggests that there is resting sodium curerent
%% end notes %% 
## highlights
---
"==almost nothing is known about how electrical signals propagate in Drosophila neurons==”[Page ](zotero://open-pdf/library/items/2IYJ2UIB?page=&annotation=ZDTX4XJV) 
 
"==electrotonically extensive and that a somatic recording electrode can only imperfectly control the voltage in the rest of the cell==”[Page ](zotero://open-pdf/library/items/2IYJ2UIB?page=&annotation=UHNSDPSE) 
 
"==action potentials initiate at a location distant from the soma, in the proximal portion of the axon.==”[Page ](zotero://open-pdf/library/items/2IYJ2UIB?page=&annotation=D64TT5MW) 
 
"==We also show that the true resting potential of these neurons is more hyperpolarized than previously thought==”[Page ](zotero://open-pdf/library/items/2IYJ2UIB?page=&annotation=BY3A3INI) 
 
"==Our results also have important consequences for the design and interpretation of experiments aimed at understanding Drosophila neurons and neural circuits.==”[Page ](zotero://open-pdf/library/items/2IYJ2UIB?page=&annotation=YFHR4ZLK) 
 
"==The resting potential sets the driving force for synaptic currents and controls the activation of voltage-gated conductances.==”[Page ](zotero://open-pdf/library/items/2IYJ2UIB?page=&annotation=IAVXLKHH) 
 
"==First, how effectively can a somatic electrode control the voltage throughout the cell? Second, where in the cell do spikes initiate? Third, how well do synaptic events propagate from the dendrite==”[Page ](zotero://open-pdf/library/items/2IYJ2UIB?page=&annotation=JH3WDX6D) 
 
"==Assuming that action potentials are 40 mV at the spike initiation zone, this observation suggests that spikes are not initiated near the soma==”[Page 3](zotero://open-pdf/library/items/2IYJ2UIB?page=3&annotation=NC8LIZPY) 
 
"==Hyperpolarizing the soma below 70 mV typically does not completely suppress spontaneous firing==”[Page 3](zotero://open-pdf/library/items/2IYJ2UIB?page=3&annotation=DURKTC63) 
 
"==Together, these observations imply that the relationship between the soma and the other compartments of the cell is different from the arrangement in most vertebrate neurons.==”[Page 3](zotero://open-pdf/library/items/2IYJ2UIB?page=3&annotation=9GIXSVDF) 
 
"==injected an approximate white-noise current which fluctuated at many frequencies==”[Page 4](zotero://open-pdf/library/items/2IYJ2UIB?page=4&annotation=WJQWTNM2) 
 
"==the white-noise stimulus has a mean value of zero, it also ensures that the membrane potential does not deviate from rest for more than a few milliseconds and thereby helps prevent activation of voltage-dependent conductances==”[Page 4](zotero://open-pdf/library/items/2IYJ2UIB?page=4&annotation=QVB6LENE) 
 
"==We found that the somatic voltage change can propagate to the dendritic tuft and the axonal arbor. However, it is substantially attenuated in the dendrite and severely attenuated in the axon==”[Page 5](zotero://open-pdf/library/items/2IYJ2UIB?page=5&annotation=AY5AXFUG) 
 
"==Clamping the membrane potential at different sites (Fig. 5A) produced varying degrees of attenuation in the soma==”[Page 6](zotero://open-pdf/library/items/2IYJ2UIB?page=6&annotation=F3S9B9ZV) 
 
"==Placing the clamp in the soma or primary neurite produced an action potential in the soma that was larger and faster than those observed experimentally==”[Page 6](zotero://open-pdf/library/items/2IYJ2UIB?page=6&annotation=M2ZQFRKV) 
 
"==The best fit was obtained when the spike initiated near the start of the axon, just distal to the location where the primary neurite bifurcates into the axonal and dendritic branches. This suggests that the SIZ lies near this site. Because all spikes recorded in the same PN have a similar size, it seems probable that spikes initiate from only one location, unlike in some other insect neurons==”[Page 6](zotero://open-pdf/library/items/2IYJ2UIB?page=6&annotation=V9NXTLGY) 
 
"==how large must these EPSPs be in the dendrite to produce the large EPSPs we record in the soma==”[Page 6](zotero://open-pdf/library/items/2IYJ2UIB?page=6&annotation=H6P9T728) 
 
"==This result argues that a single ORN axon distributes release sites onto multiple dendritic branches of each postsynaptic PN.==”[Page 6](zotero://open-pdf/library/items/2IYJ2UIB?page=6&annotation=PVV9Z3YX) 
 
"==Nevertheless, EPSPs still did not cause substantial voltage changes at the axon terminals, implying that action potentials are indeed necessary for synaptic output in PNs.==”[Page 6](zotero://open-pdf/library/items/2IYJ2UIB?page=6&annotation=CKE9TVUW) 
 
"==PN firing rates generally increased immediately after rupturing the membrane patch beneath the pipette (Fig. 7A,B), implying that the resting potential measured in whole-cell mode is somewhat more depolarized than the resting potential in intact neurons.==”[Page 7](zotero://open-pdf/library/items/2IYJ2UIB?page=7&annotation=JKTK93FK) 
 
"==On average, we had to hyperpolarize the membrane from 47.8 1.6 mV to 57.8 1.5 mV to recapitulate the cell-attached firing rate==”[Page 7](zotero://open-pdf/library/items/2IYJ2UIB?page=7&annotation=CMKE7KFU) 
 
"==Because somatic voltage changes are attenuated in the rest of the cell, the SIZ and dendrite are likely to sit closer to their true resting potential during a whole-cell recording than the soma does.==”[Page 7](zotero://open-pdf/library/items/2IYJ2UIB?page=7&annotation=UG9HQH42) 
 
"==A more likely scenario is that breaking into the cell introduces current flow through the cell membrane adjacent to the pipette (the seal)==”[Page 7](zotero://open-pdf/library/items/2IYJ2UIB?page=7&annotation=AUC942AS) 
 
"==Drosophila neurons are extremely small and have high input resistances==”[Page 7](zotero://open-pdf/library/items/2IYJ2UIB?page=7&annotation=6NTWFBT4) 
 
"==We, therefore, considered how the seal resistance would affect the measured resting potential using a simple equivalent circuit model==”[Page 7](zotero://open-pdf/library/items/2IYJ2UIB?page=7&annotation=HEYQRCEL) 
 
"==the transition to a whole-cell configuration will depolarize a PN by several millivolts, with the exact magnitude of this effect depending on the input resistance and the level of ongoing synaptic input to the cell==”[Page 7](zotero://open-pdf/library/items/2IYJ2UIB?page=7&annotation=U5ZWSBGZ) 
 
"==Therefore, unlike many other cells, they probably do not perform dendritic computations that rely on the specific spatial locations of synaptic inputs==”[Page 8](zotero://open-pdf/library/items/2IYJ2UIB?page=8&annotation=LR5QKRH3) 
 
"==Nevertheless, it is likely that the effective value of the seal resistance varied across recordings, and this may be one reason why data from different electrophysiological recordings yielded somewhat different best-fit models.==”[Page 9](zotero://open-pdf/library/items/2IYJ2UIB?page=9&annotation=UI9JS79S) 
 
#📚 

%% Import Date: 2025-04-27T17:28:25.416-07:00 %%
