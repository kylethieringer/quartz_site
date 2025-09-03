---
paper_title: Modularity and robustness of frontal cortical networks
year: "2021"
authors: Guang Chen, Byungwoo Kang, Jack Lindsey, Shaul Druckmann, Nuo Li
type: literature note
note date: 2025-05-03
modified: 
summary: 
tags: 
status: 
title: Chen.etal2021b
publish: "true"
timestamp: 2025-06-01 15:50
---
# Modularity and robustness of frontal cortical networks
**authors**: *Guang Chen, Byungwoo Kang, Jack Lindsey, Shaul Druckmann, Nuo Li*
**doi**: 10.1016/j.cell.2021.05.026

> [!INFO] CITATION
> Chen, G., Kang, B., Lindsey, J., Druckmann, S., & Li, N. (2021). Modularity and robustness of frontal cortical networks. _Cell_, _184_(14), 3717-3730.e24. [https://doi.org/10.1016/j.cell.2021.05.026](https://doi.org/10.1016/j.cell.2021.05.026)

> [!NOTE] ABSTRACT
> 
> 
## fleeting notes
---
%% begin notes %% 

it is unknown how brain regions interact for persistent activity and having robustness

recorded population activity to see how regions interact
each hemisphere had persistent activity when other hemisphere was perturbed to prevent spreading... what does spreading mean?

persistent activity bridges past and future - supports short term memory

corrupt info in one brain region can be compensated for by redundant information in other regions
- these parallel representations need to be separate so that corrupt info cant propagate

ALM neurons have persistent activity and instructs choice. 
- choice is not affected when one hemisphere is perturbed. recovery of choice info depends on other hemisphere

ALM hemispheres are highly coordinated and have parallel representations of choice

some mice had modular organization other mice did not. modular organization was more robust

there is a challenge in the brain: 
- two hemispheres must be independent to prevent spread of corrupted info
- however they need to be connected to recover information

modeling suggests that there is activity state gating of interactions to achieve both of these things
- better gating == better short term memory

Task:
- delayed response task
- tactile stimulus of whisker and reported object location with licking
- delay of 1.7s to make sure mice use short term memory

recorded from both hemispheres and had similar neurons numbers on each side
- different neurons were selective for left or right lick trials

choice selective neurons have similar activity profile in each hemisphere. but stimulus selective cells are different. 
- this shows that there is redundant choice selection

built a linear decoder to detect choice from the activity in the delay epoch
- monitored choice in population activity through the decoder activity
- left and right sides had highly correlated choice activity

each hemisphere contains redundant choice information

silenced neurons in the ALM during early delay epoch. this abolished choice selectivity
- and activity became less correlated
- correlated activity is not explained by movements or eternal input. so it means they interact with each other for choice info

recorded from 39 mice! holyyy

did unilateral silencing but bilateral recording
- in some mice, choice selectivity remained in the contralateral hemisphere showing compatmentalized representation
- in other mice, activity was asymmetric

modularity correlated with choice detection probability and showed 
- but modularity varied across individuals

the side of the tactile stimulus rather than the sensorimotor contingency drove the shift in interhemispheric asymmetry

trials also varied in variability. and showed different degrees of robustness to perturbations

how does the brain maintain modularity between hemispheres and recover information after pertubration?

trained a model to predict single trial dynamics from activity of hemispheres
- performance improved when adding contralateral hemisphere activity
	- but both hemispheres were very correlated

state dependence - how strong is the selectivity (essentially confidence?) 
- if less selective then it allows for influence from the other hemisphere

modularity was inversely correlated with strength of interhemispheric influence

used an RNN to explore how the network solves robust solutions to perturbations
- networks were robust if:
	- they were initialized into modules before training
	- they were trained as modules - internal weights of modules were trained but not between module weights
	- if there were nonlinear dynamics
- without these conditions - the networks showed attractor dynamics

asymmetry of hemisphere dynamics depended on the strength of sensory input to each hemisphre

%% end notes %% 
## highlights
---
"==Neural activity underlying short-term memory is maintained by interconnected networks of brain regions==”[Page 2](zotero://open-pdf/library/items/TC3SL5XB?page=2&annotation=4VIW7W6K) 
 
"==nknown how brain regions interact to maintain persistent activity while exhibiting robustness==”[Page 2](zotero://open-pdf/library/items/TC3SL5XB?page=2&annotation=YI76PI4G) 
 
"==we uncovered individual variability in the organization of frontal cortical networks.==”[Page 2](zotero://open-pdf/library/items/TC3SL5XB?page=2&annotation=FG3ISF87) 
 
"==each hemisphere retained persistent activity during perturbations of the other hemisphere, thus preventing local perturbations from spreading.==”[Page 2](zotero://open-pdf/library/items/TC3SL5XB?page=2&annotation=5IUTJ2JS) 
 
"==robust short-term memory is mediated by redundant modular representations across brain regions==”[Page 2](zotero://open-pdf/library/items/TC3SL5XB?page=2&annotation=2GH6NWH6) 
 
"==Redundant modular representations naturally emerge in neural network models that learned robust dynamics==”[Page 2](zotero://open-pdf/library/items/TC3SL5XB?page=2&annotation=SSL8C4TJ) 
 
"==whereby corrupt information in one brain region can be compensated for by redundant information in other regions==”[Page 2](zotero://open-pdf/library/items/TC3SL5XB?page=2&annotation=9ZLY92KC) 
 
"==multiple parallel representations must be compartmentalized such that perturbations in one representation do not propagate into another==”[Page 2](zotero://open-pdf/library/items/TC3SL5XB?page=2&annotation=A9MP4PPG) 
 
"==Neurons in mouse anterior lateral motor cortex (ALM) exhibit persistent activity that instructs future choice==”[Page 2](zotero://open-pdf/library/items/TC3SL5XB?page=2&annotation=KLX2WALW) 
 
"==Choice information is robust to transient perturbations of ALM activity in one hemisphere, and the recovery of choice information is dependent on input from the contralateral hemisphere==”[Page 2](zotero://open-pdf/library/items/TC3SL5XB?page=2&annotation=V2Q24KTI) 
 
"==Perturbation revealed unexpected variability in the organization of frontal cortical networks across a population of mice.==”[Page 2](zotero://open-pdf/library/items/TC3SL5XB?page=2&annotation=UXHQ67CH) 
 
"==Conceptually, the two hemispheres must be independent to retain choice information during unilateral perturbations. At the same time, the hemispheres must communicate to coordinate coherent information and recover information after perturbations. Theoretical analysis of the neural data and modeling suggests that the interhemispheric interaction was dynamically gated by the activity state to simultaneously meet these two conflicting requirements==”[Page 4](zotero://open-pdf/library/items/TC3SL5XB?page=4&annotation=QHBN5A5A) 
 
"==Mice with more potent gating showed superior short-term memory behavior even in the absence of external perturbations. Our results show that robust persistent activity is maintained by redundant modular representations distributed across multiple brain regions.==”[Page 4](zotero://open-pdf/library/items/TC3SL5XB?page=4&annotation=P4C8P7ZP) 
 
"==Choice selectivity arose during the late sample epoch, ramped up through the delay, and reached a maximum during movement initiation==”[Page 4](zotero://open-pdf/library/items/TC3SL5XB?page=4&annotation=N8UUDKBU) 
 
"==These results show that the two ALM hemispheres have parallel representations of choice information during the delay epoch.==”[Page 4](zotero://open-pdf/library/items/TC3SL5XB?page=4&annotation=CCUXHNKV) 
 
"==Trajectory endpoints were highly correlated across trials==”[Page 4](zotero://open-pdf/library/items/TC3SL5XB?page=4&annotation=9N5KYUHQ) 
 
"==Thus, the two hemispheres have coherent choice encoding, and each hemisphere contains redundant choice information.==”[Page 4](zotero://open-pdf/library/items/TC3SL5XB?page=4&annotation=SYDUV858) 
 
"==that activity reflecting ongoing movements was not the primary driver of the correlation between hemispheres.==”[Page 6](zotero://open-pdf/library/items/TC3SL5XB?page=6&annotation=RGSA5SIX) 
 
"==We silenced activity in both hemispheres during the early delay epoch using 4 laser spots on each hemisphere that covered the entire ALM and surrounding regions==”[Page 6](zotero://open-pdf/library/items/TC3SL5XB?page=6&annotation=J87AIZJ5) 
 
"==The modularity of each hemisphere varied along a continuum across individual sessions==”[Page 6](zotero://open-pdf/library/items/TC3SL5XB?page=6&annotation=U4A2W92B) 
 
"==Further systematic task manipulations showed that the side of the tactile stimulus, rather than the sensorimotor contingency, drove the shift in interhemispheric asymmetry==”[Page 7](zotero://open-pdf/library/items/TC3SL5XB?page=7&annotation=EDA6I4C2) 
 
"==Thus, different sessions exhibited different degrees of robustness to perturbations==”[Page 7](zotero://open-pdf/library/items/TC3SL5XB?page=7&annotation=CGCQIRSM) 
 
"==how hemispheres maintain modular representations and recover choice information after perturbations.==”[Page 7](zotero://open-pdf/library/items/TC3SL5XB?page=7&annotation=PA446K6X) 
 
"==To have both properties at the same time, interaction strength between the hemispheres needs to be modulated in a state-dependent way.==”[Page 7](zotero://open-pdf/library/items/TC3SL5XB?page=7&annotation=W825DSI6) 
 
"==ALM activity on held-out control trials (Figures 5C and S6A). Importantly, for nearly every session, adding the influence of the other hemisphere significantly improved model prediction==”[Page 9](zotero://open-pdf/library/items/TC3SL5XB?page=9&annotation=8JCEXJHE) 
 
"==Importantly, the modulation was consistent with a state-dependent gating mechanism: the influence of the other hemisphere was weaker when choice encoding was strong within a hemisphere==”[Page 9](zotero://open-pdf/library/items/TC3SL5XB?page=9&annotation=NUFE7STQ) 
 
"==In trials where the unperturbed hemisphere exhibited weak choice encoding, its selectivity was strongly affected by contralateral photoinhibition==”[Page 9](zotero://open-pdf/library/items/TC3SL5XB?page=9&annotation=NA8PUGN9) 
 
"==In contrast, when the unperturbed hemisphere exhibited strong choice encoding, its selectivity was less affected (==”[Page 9](zotero://open-pdf/library/items/TC3SL5XB?page=9&annotation=S2SX7JLI) 
 
"==In asymmetric sessions, the hemisphere with low modularity (driven hemisphere) showed strong influence from the other hemisphere (little gating, Figure 6A). In modular sessions, the same hemisphere showed little influence from the other hemisphere (strong gating==”[Page 10](zotero://open-pdf/library/items/TC3SL5XB?page=10&annotation=KIGET8NK) 
 
"==modularity of a hemisphere (revealed by photoinhibition) could be explained by the gating of interhemispheric influence inferred from control trials==”[Page 10](zotero://open-pdf/library/items/TC3SL5XB?page=10&annotation=DIBKPIP8) 
 
"==the strength of interhemispheric influence in the weakly selective state predicted the recovery of choice information following photoinhibition==”[Page 10](zotero://open-pdf/library/items/TC3SL5XB?page=10&annotation=5CRDNDJ6) 
 
"==This suggests that the ability of the two hemispheres to dynamically gate influence and maintain modular representations might help better maintain choice information during normal behavior, possibly by increasing robustness to internal perturbations such as noise.==”[Page 11](zotero://open-pdf/library/items/TC3SL5XB?page=11&annotation=6R5THB8R) 
 
"==We next examined more generally what interhemispheric interactions might arise in highly connected networks required to perform the delayed response task with minimal additional assumptions. We chose recurrent neural networks (RNNs) due to their ability to generate models that are constrained to solve a task without enforcing their solutions==”[Page 11](zotero://open-pdf/library/items/TC3SL5XB?page=11&annotation=JW8HTCQK) 
 
"==Learned networks were robust to perturbations without experiencing perturbations during training when three conditions were met (Figures S7A and S7B): (1) modular initialization—networks were partitioned into modules before training, in which the initial between-module connection weights were smaller than the within-module connection weights; (2) modular training—the internal weights of each module were trained while keeping the between-module weights frozen; (3) nonlinearity—units within the RNN had nonlinear input-output functions (==”[Page 11](zotero://open-pdf/library/items/TC3SL5XB?page=11&annotation=EN2J5FK4) 
 
"==Remarkably, even though we did not build in any state-dependent gating mechanisms, the interhemispheric influences of the robust RNNs were modulated such that the influence of the other hemisphere was smaller when a hemisphere was highly selective and greater when it was weakly selective==”[Page 11](zotero://open-pdf/library/items/TC3SL5XB?page=11&annotation=K9SE6IYK) 
 
"==Consistent with our hypothesis, interhemispheric influence in these RNNs developed an asymmetry that was dependent on the relative strength of sensory input to each hemisphere==”[Page 12](zotero://open-pdf/library/items/TC3SL5XB?page=12&annotation=7EYZRZWJ) 
 
"==ur study provides evidence for modular organization in frontal cortical networks that maintain persistent activity.==”[Page 12](zotero://open-pdf/library/items/TC3SL5XB?page=12&annotation=REMH6REE) 
 
"==Modular organization is required for the robustness of persistent activity to perturbations==”[Page 12](zotero://open-pdf/library/items/TC3SL5XB?page=12&annotation=53MSSXGI) 
 
"==Future experiments tracking the activity of both hemispheres in the same animal across learning will shed light on the underlying mechanisms.==”[Page 13](zotero://open-pdf/library/items/TC3SL5XB?page=13&annotation=C6NVW23X) 
 
"==This type of modulation makes sense from a normative point of view: if a representation has accurate information, then receiving outside influence could be detrimental, but a representation that has poor information would likely benefit from influence.==”[Page 13](zotero://open-pdf/library/items/TC3SL5XB?page=13&annotation=4VTXV945) 
 
#📚 

%% Import Date: 2025-05-03T12:21:32.257-07:00 %%
