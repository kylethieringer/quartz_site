---
paper_title:
  - Functional Maps of Mechanosensory Features in the Drosophila Brain
title: Patella.Wilson2018
year: "2018"
authors: Paola Patella, Rachel I. Wilson
type: literature note
note date: 2023-10-07
modified: 
summary: unsupervised clustering of response types in the JONs, AMMC, and WED reveals a spatially organized map of mechanical feature stimuli
tags:
  - 📚
status: true
publish: "true"
timestamp: 2023-12-11 09:35
---

# Functional Maps of Mechanosensory Features in the Drosophila Brain
**authors**: *Paola Patella, Rachel I. Wilson*
**doi**: 10.1016/j.cub.2018.02.074
**zotero link**: [Full Text](zotero://select/groups/5209539/items/ERB8L8JZ)

> [!INFO] CITATION
> Patella, P., & Wilson, R. I. (2018). Functional Maps of Mechanosensory Features in the Drosophila Brain. _Current Biology_, _28_(8), 1189-1203.e5. [https://doi.org/10.1016/j.cub.2018.02.074](https://doi.org/10.1016/j.cub.2018.02.074)

> [!NOTE] ABSTRACT
> Johnston’s organ is the largest mechanosensory organ in Drosophila. It contributes to hearing, touch, vestibular sensing, proprioception, and wind sensing. In this study, we used in vivo 2-photon calcium imaging and unsupervised image segmentation to map the tuning properties of Johnston’s organ neurons (JONs) at the site where their axons enter the brain. We then applied the same methodology to study two key brain regions that process signals from JONs: the antennal mechanosensory and motor center (AMMC) and the wedge, which is downstream of the AMMC. First, we identified a diversity of JON response types that tile frequency space and form a rough tonotopic map. Some JON response types are direction selective; others are specialized to encode amplitude modulations over a specific range (dynamic range fractionation). Next, we discovered that both the AMMC and the wedge contain a tonotopic map, with a significant increase in tonotopy—and a narrowing of frequency tuning—at the level of the wedge. Whereas the AMMC tonotopic map is unilateral, the wedge tonotopic map is bilateral. Finally, we identified a subregion of the AMMC/wedge that responds preferentially to the coherent rotation of the two mechanical organs in the same angular direction, indicative of oriented steady air flow (directional wind). Together, these maps reveal the broad organization of the primary and secondary mechanosensory regions of the brain. They provide a framework for future efforts to identify the specific cell types and mechanisms that underlie the hierarchical re-mapping of mechanosensory information in this system.

## notes
[[tonotopy of the auditory system acts as an array of bandpass filters]]
[[unsupervised clustering of calcium imaging data]]

- Tonotopy allows co tuned neurons to interact with each other using minimal expenditure of "wire" - this maximizes speed and minimizes metabolic costs
## fleeting notes

- [[Johnston's organ neurons]] - largest mechanosensory organ in Drosophila
	- hearing, touch, vestibular sensing, proprioception, and wind
- JONs project to [[antennal mechanosensory and motor center|AMMC]] (antennal mechanosensory and motor center) and the [[wedge]]
- [[wedge|WED]] - wedge is downstream of the AMMC

- AMMC and the wedge contain a tonotopic map
- the wedge tonotopy is significantly higher and narrow frequency tuning
- AMMC tonotopic map is unilateral
- wedge tonotopic map is bilateral

- tonotopic maps reveal broad organization of primary and secondary mechanosensory regions

- experimental methods
	- head rotated 180 degrees with proboscis removed and imaging ventral side up. 
	- piezoelectric motor used to mechanically stimulate the arista
		- waveforms with frequency modulated sweeps (0-600 Hz)
		- narrowband vibrations - tones
		- sustained displacement
		- courtship song
	- imaging JON axons where they enter the brain and terminate on the AMMC
		- JON axons instead of soma in order to compare spatial maps of JON response to spatial maps of AMMC
		- GCaMP6f in pan JON driver (nan-Gal4) and subsets of JONs using splits

- pipeline
	- pull out single pixel responses in the imaging plane
	- discard unresponsive pixels
	- pool pixels across z-planes, brains, and genotypes
	- discard uncorrelated pixels because they contain noise
	- define functional clusters from the 102,669 x 3549 matrix (pixels x time) based on the response types
	- apply functional cluster labels to pixels
- make no assumptions about what stimulus features define the functional differences
- types defined in functional terms not spatial
- use cross brain similarity as a check on the plausibility of the algorithm output

- identified 10 JON types
	- because there were 10 response types
	- the pan JON imaging and the sparse lines had consistent response types but the sparse lines only responded to maybe 1 or 2 stimuli
- courtship song recruits all JON types
	- there is no specialized courtship song detector at the JONs
- JON types had a range of amplitudes they were sensitive to. 
	- type x responded to low frequency but increasing amplitude didnt increase response linearly so it was already saturated at the low amplitude
- JON types had different adaptation properties
	- some showed adaptations to sustained frequencies, some showed no adaptation

- Jons act as a parallel array of bandpass filters with center frequencies ranging from direct current to less than 600 Hz
	- some are directionally tuned 
	- some carry amplitude info

- Tonotopic map of JONs
	- steady displacement (DC) most medial edge
	- high frequency located more laterally

- found 19 response types in the CNS using the same pipeline
	- some represented in both the AMMC and the WED
	- no response types were exclusive to the AMMC

- why were there repeats in the CNS functional types like 3 different sections that respond to 75hz but their responses look the same in Fig5?????

- AMMC had over representation of low frequencies??
- WED had an over representation of extreme requencies
	- individual tuning of each response type was narrower in the WED than in the AMMC or JONs
	- individual WED neurons are more narrowly tuned than AMMC or JONs or they are more systematically positioned according to frequency
	- tonotopic representation was more orderly in the WED

- AMMC reponded mainly to ipsilateral antenna whereas WED had responses to both antenna

- most of the drosophila brain is neuropil
- most somata are excluded from the neuropil and are found in a thin rind around teh neuropil
- neuropil imaging - measuring signals from groups of neurons not single neurons
- calcium imaging has limited temporal resolution


#🐛 | #📚 
%% Import Date: 2023-10-07T19:06:23.714-04:00 %%
