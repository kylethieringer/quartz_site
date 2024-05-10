---
paper_title: Neural Coding of Leg Proprioception in Drosophila
year: "2018"
authors: Akira Mamiya, Pralaksha Gurung, John C. Tuthill
type: literature note
note date: 2024-05-03
modified: 
summary: 
tags: 
status: 
title: Mamiya.etal2018
publish: "true"
timestamp: 2024-05-10 11:14
---
# Neural Coding of Leg Proprioception in Drosophila
**authors**: *Akira Mamiya, Pralaksha Gurung, John C. Tuthill*
**doi**: 10.1016/j.neuron.2018.09.009

> [!INFO] CITATION
> Mamiya, A., Gurung, P., & Tuthill, J. C. (2018). Neural Coding of Leg Proprioception in Drosophila. _Neuron_, _100_(3), 636-650.e6. [https://doi.org/10.1016/j.neuron.2018.09.009](https://doi.org/10.1016/j.neuron.2018.09.009)

> [!NOTE] ABSTRACT
> 
> 

## fleeting notes
---
%% begin notes %% 


- 2p calcium imaging of proprioceptive sensory neurons during controlled movements of the fly tibia
- axons are organized into distinct functional projections containing topographic representations of kinematic features -- does this just mean movement?
- one group = tibia position (flexion and extension)
- one group = tibia movement direction
- one group = tibia bidirectional movement and vibration frequency

- "proprioceptive stimuli from single leg joint are encoded by diverse population of sensory neurons and how proprioceptive feedback signals are used by motor circuits to coordinate body"

- [[proprioception]]

- Femoral chordotonal organ - FeCO
- population imaging from proprioceptive neurons labeled by iav-gal4

- chose to control leg kinematics with a magnetic bar that moved the joint angle


- calculated pairwise correlations between calcium signal in each pixel in order to cluster activity then performed kmeans clustering on the correlation matrix
	- this revealed spatially separated groups of axons that encode distinct proprioceptive stim features

- to find the functional organization of FeCO axons
	- first clustered trial to trial from four regions of interest
	- combined responses from same region in different flies
	- then grouped again using kmeans clustering

- 5 basic subclasses of responses in FeCO axons
	- two tonic non adapting 
	- 3 phasic adapting

- tonic response - increase activity when tibia extends or flexes
- phasic response - transient increase during movement phase of swing
	- one responded to either direction
	- 2 responded only to one direction

- different projections of proprioceptive axons have different tuning and are organized similarly across flies

- club - labels axons that run laterally through center of leg (R64C04-Gal4)
	- terminate near midline. some toward brain or other segments
- claw - shaped like a claw. projections split into 3 smaller branches. X,Y,Z branches. (R73D10-Gal4)
- hook - projections run along Z branch of the claw and extend a longer arborization toward midline (R21D21-Gal4)

- [[proprioceptor driver lines]]

- claw neurons tonically increase activity in response to flexion or extension of tibia
- club neurons phasically increase activity in response to flexion or extension
- hook neurons active more during flexion

- ramp and hold stimulus to explore position dependent tuning of proprioceptor subclasses
	- claw neurons responded with tonic increases during flexion or extension
		- activity of extension tuned pixels increased when tibia was between 90 and 180 degrees
		- flexion tuned pixels increased when tibia was less than 90 degrees
		- none active during middle of range
		- linear tuning of femur tibia joint angle
	- club neurons respond phasically to each tibia movement regardless of direction across all joint angles
	- hook neurons phasically increase activity during flexion not extension. slightly weaker when fully extended
- used a piezoelectric chip to vibrate magnet attached to leg at different frequencies (100-2000 hz)
- club neurons have large response to tibia vibration
- claw and hook do not respond to vibration

- spatial organization of responses in club neurons in response to frequency range
	- a frequency map
- single club neurons are tuned to different frequencies

- single claw neurons are tuned to have peak responses at different femur tibia angles

claw neurons encode the position of the tibia
- 

%% end notes %% 
## highlights
---
#📚 

%% Import Date: 2024-05-03T22:49:44.840-07:00 %%
