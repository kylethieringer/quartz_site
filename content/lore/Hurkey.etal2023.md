---
paper_title: Gap junctions desynchronize a neural circuit to stabilize insect flight
year: "2023"
authors: Silvan Hürkey, Nelson Niemeyer, Jan-Hendrik Schleimer, Stefanie Ryglewski, Susanne Schreiber, Carsten Duch
type: literature note
note date: 2025-04-20
modified: 
summary: 
tags: 
status: 
title: Hurkey.etal2023
publish: "true"
timestamp: 2025-04-20 11:31
---
# Gap junctions desynchronize a neural circuit to stabilize insect flight
**authors**: *Silvan Hürkey, Nelson Niemeyer, Jan-Hendrik Schleimer, Stefanie Ryglewski, Susanne Schreiber, Carsten Duch*
**doi**: 10.1038/s41586-023-06099-0

> [!INFO] CITATION
> Hürkey, S., Niemeyer, N., Schleimer, J.-H., Ryglewski, S., Schreiber, S., & Duch, C. (2023). Gap junctions desynchronize a neural circuit to stabilize insect flight. _Nature_, _618_(7963), 118–125. [https://doi.org/10.1038/s41586-023-06099-0](https://doi.org/10.1038/s41586-023-06099-0)

> [!NOTE] ABSTRACT
>Abstract Insect asynchronous flight is one of the most prevalent forms of animal locomotion used by more than 600,000 species. Despite profound insights into the motor patterns 1 , biomechanics 2,3 and aerodynamics underlying asynchronous flight 4,5 , the architecture and function of the central-pattern-generating (CPG) neural network remain unclear. Here, on the basis of an experiment–theory approach including electrophysiology, optophysiology, Drosophila genetics and mathematical modelling, we identify a miniaturized circuit solution with unexpected properties. The CPG network consists of motoneurons interconnected by electrical synapses that, in contrast to doctrine, produce network activity splayed out in time instead of synchronized across neurons. Experimental and mathematical evidence support a generic mechanism for network desynchronization that relies on weak electrical synapses and specific excitability dynamics of the coupled neurons. In small networks, electrical synapses can synchronize or desynchronize network activity, depending on the neuron-intrinsic dynamics and ion channel composition. In the asynchronous flight CPG, this mechanism translates unpatterned premotor input into stereotyped neuronal firing with fixed sequences of cell activation that ensure stable wingbeat power and, as we show, is conserved across multiple species. Our findings prove a wider functional versatility of electrical synapses in the dynamic control of neural circuits and highlight the relevance of detecting electrical synapses in connectomics. 
>  
## fleeting notes
---
%% begin notes %% 

the CPG neural network for asynchronous flight remains unclear. 

here, there is a splayed out pattern of activity in motor neurons connected by electrical synapses that are asynchronous with each other

they claim that their model demonstrates how unpatterned premotor input translates to fixed sequences of cell activation for stable wingbeat power

asynchronous flight has evolved 7-10 times in evolution!

flight MNs fire at lower frequencies than the muscles - not cycle to cycle basis. power output is regulated by MN firing frequencies

CPG architecture / principles for MN output is not identified. 

used DLM MNs 1-5 to study CPG output

DLM provides the force for wing downstroke
- 6 muscle fibers 
- MN1-4 target one of the four most ventral DLM fibers ipsilateral to soma
- MN5 innervates fiber 5-6 on contralateral side to soma

all DLMn fire at the same frequency within animals


MN1-5 control muscular tension and stretch activatability by adjusting myoplasmic calcium levels
- for further reading about calcium and mechanical power:
	- Gordon, S. & Dickinson, M. H. Role of calcium in the regulation of mechanical power in insect flight. Proc. Natl Acad. Sci. USA 103, 4311–4315 (2006).
	- Wang, Q., Zhao, C. & Swank, D. M. Calcium and stretch activation modulate power generation in Drosophila flight muscle. Biophys. J. 101, 2207–2213 (2011).

[[DLMn activity drives linear changes in wing beat frequency]]

MN1-5 linearly translate synaptic input into tonic firing

MN1-5 spikes are splayed out in time. 
- sequence of firing can change but the CPG slides back into one of the preferred splay states
- same splay states preferred across animals
	- 1423 and 1324 are the most common
	- firing of MN pairs is not phase locked

the timing and pattern of MN activation during locomotion relies on networks of premotor neurons. however, here it is by interactions between MNs themselves

[[the DLMns compose a minimal flight CPG]]
	the MNs themselves constitute a minimal CPG themselves

receptors for inhibitory transmitters :
- GABA A receptors
- glutamate gated chloride channels (GluCl)

lateral inhibition through chemical synapses is not required for pattern generation

[[weak electrical coupling between DLMns favors splayed firing pattern]]
**weak** electrical coupling creates the splay state
- knockdown using RNAi of connexins (shakB) creates random firing patterns (but frequency is conserved)
- over expression of connexins (shakB) causes synchronization

the electrical synapses are weak, bidirectional and non-rectifying

[[the DLMn gap junctions are nonrectifying]]

mathematical model:
- bifurcation analysis 
- out of phase firing is preferred through a homoclinic spike onset near the saddle node loop bifurcation
	- i think this is saying that they used a dynamical systems approach. homoclinic is saying that the system returns back to a fixed point and the onset is 
- there are three spike onset bifurcations..?
	- subcritical Hopf
	- saddle-node-on-an-invariant cycle SNIC
	- saddle homoclinic orbit (HOM)

shab channels are around 50% of the delayed rectifier currents in the MNs

shab overexpression results in near synchronization

[[splayed DLMn firing stabilizes wingbeat frequency]]
synchronized MN firing causes large oscillations in WBF rather than more stable WBF

there is heterogeneous electrical coupling between MN1-5

each MN causes an increase in calcium in the muscle fiber. there is a long delay time constant so the splay state firing keeps a relatively stable calcium concentration in the muscle 

%% end notes %% 
## highlights
---
"==Insect asynchronous flight is one of the most prevalent forms of animal locomotion used by more than 600,000 species==”[Page ](zotero://open-pdf/library/items/HNFY4DSD?page=&annotation=D8UPVV6F) 
 
"==the architecture and function of the central-patterngenerating (CPG) neural network remain unclear==”[Page ](zotero://open-pdf/library/items/HNFY4DSD?page=&annotation=LZSZQMEW) 
 
"==The CPG network consists of motoneurons interconnected by electrical synapses that, in contrast to doctrine, produce network activity splayed out in time instead of synchronized across neurons==”[Page ](zotero://open-pdf/library/items/HNFY4DSD?page=&annotation=GUMB3FX2) 
 
"==In small networks, electrical synapses can synchronize or desynchronize network activity, depending on the neuron-intrinsic dynamics and ion channel composition==”[Page ](zotero://open-pdf/library/items/HNFY4DSD?page=&annotation=SSUFSHR4) 
 
"==n the asynchronous flight CPG, this mechanism translates unpatterned premotor input into stereotyped neuronal firing with fixed sequences of cell activation that ensure stable wingbeat power and, as we show, is conserved across multiple species==”[Page ](zotero://open-pdf/library/items/HNFY4DSD?page=&annotation=K8G4VUVK) 
 
"==In 75% of all flying insect species, highly specialized, indirect, asynchronous flight muscles form an oscillatory system that generates wingbeat frequencies of 100–1,000 Hz by reciprocal stretch activation of antagonistic wing muscles to ensure forward propulsion at low Reynolds numbers==”[Page ](zotero://open-pdf/library/items/HNFY4DSD?page=&annotation=8R2AL9AG) 
 
"==The flight motoneurons (MNs) that innervate asynchronous flight muscles fire at much lower frequencies, therefore not activating the muscles on a cycle-to-cycle basis==”[Page ](zotero://open-pdf/library/items/HNFY4DSD?page=&annotation=75H63MMU) 
 
"==output is regulated by a CPG network in the central nervous system that controls MN firing frequencies to adjust the myoplasmic calcium levels that, in turn, regulate wingbeat frequency and amplitude==”[Page ](zotero://open-pdf/library/items/HNFY4DSD?page=&annotation=YMTVKA6E) 
 
"==asynchronous flight has emerged independently 7–10 times during evolution==”[Page ](zotero://open-pdf/library/items/HNFY4DSD?page=&annotation=BJQPHTU4) 
 
"==lthough the firing frequencies of MN1–5 can vary between animals and are adjusted on demand1,15,16, within a given animal and power demand, all five MNs always fire at the same frequencies==”[Page ](zotero://open-pdf/library/items/HNFY4DSD?page=&annotation=6MXDH2BW) 
 
"==MN1–5 firing frequencies directly control muscular tension and stretch activatability by adjusting myoplasmic calcium levels and, therefore, wingbeat frequency and stroke amplitude==”[Page 2](zotero://open-pdf/library/items/HNFY4DSD?page=2&annotation=N9HN4DLL) 
 
"==A linear relationship between average MN firing and average wingbeat frequency==”[Page 2](zotero://open-pdf/library/items/HNFY4DSD?page=2&annotation=G2EIBY8S) 
 
"==he central nervous system controls asynchronous flight muscle power output neither by the recruitment of different motor units, nor on the scale of single wingbeats, but the frequency of MN1–5 population firing is the key regulator of wing power production==”[Page 2](zotero://open-pdf/library/items/HNFY4DSD?page=2&annotation=VWFD5LZN) 
 
"==their spikes are splayed-out in time with firing phases across neurons dispersed approximately equidistantly, resulting in stereotyped preferred sequences of MN1–5 spiking==”[Page 2](zotero://open-pdf/library/items/HNFY4DSD?page=2&annotation=NHY3GT66) 
 
"==A network splay state means that each individual cell in a network of N neurons fires regularly, yet with a constant, non-zero phase relationship with respect to the firing of each other neuron==”[Page 2](zotero://open-pdf/library/items/HNFY4DSD?page=2&annotation=FW9W6WBU) 
 
"==he sequence of MN1–5 firing can change intermittently, but the CPG robustly slides back into one or two of the most preferred splay states==”[Page 2](zotero://open-pdf/library/items/HNFY4DSD?page=2&annotation=GSBBDZEU) 
 
![[attachments/Hurkey.etal2023_image-2-x380-y564.png]][Page 2](zotero://open-pdf/library/items/HNFY4DSD?page=2&annotation=42QKXQ7R) 
 
"==the timing and pattern of MN activation during locomotion typically rely on networks of premotor interneurons==”[Page 3](zotero://open-pdf/library/items/HNFY4DSD?page=3&annotation=XXWC47CH) 
 
"==that splayed-out MN1–5 firing is generated by interactions between the MNs themselves==”[Page 3](zotero://open-pdf/library/items/HNFY4DSD?page=3&annotation=EWDYPZ6Z) 
 
"==and that all MNs share common synaptic input==”[Page 3](zotero://open-pdf/library/items/HNFY4DSD?page=3&annotation=LSCECP3I) 
 
"==ommon excitatory synaptic drive to MN1–5, as induced by optogenetic stimulation, is therefore transformed into out-of-phase MN1–5 firing==”[Page 3](zotero://open-pdf/library/items/HNFY4DSD?page=3&annotation=AW62V37H) 
 
"==unpatterned, tonic, optogenetic stimulation of the five MNs (see Extended Data Fig. 5a,b for selective expression of transgenes in MN1–5) during flight increases their firing frequency and, therefore, wingbeat power, but it does not change phase relationships between MNs, as exemplified by the same characteristic gap around phase 0 for the MN4–MN5 pair==”[Page 3](zotero://open-pdf/library/items/HNFY4DSD?page=3&annotation=R3E737BK) 
 
"==However, neither trans-synaptic mapping nor genetic markers for central output synapses from MN1–5 provide evidence for postsynaptic partners in the ventral nerve cord==”[Page 3](zotero://open-pdf/library/items/HNFY4DSD?page=3&annotation=BWDQRJZF) 
 
"==hus, the in vivo data indicate that weak electrical synapses cause firing desynchronization, but stronger coupling synchronizes firing.==”[Page 3](zotero://open-pdf/library/items/HNFY4DSD?page=3&annotation=UMURQL8F) 
 
"==Dual in situ patch-clamp recordings of MN pairs confirm electrical coupling and demonstrate that the electrical synapses are weak, bidirectional and non-rectifying==”[Page 3](zotero://open-pdf/library/items/HNFY4DSD?page=3&annotation=6MD8JVAD) 
 
"==we found that the AHP of MN spikes is transmitted more effectively (CC, 0.042 ± 0.04) through ShakB-mediated electrical synapses than the brief spike overshoot==”[Page 4](zotero://open-pdf/library/items/HNFY4DSD?page=4&annotation=3IMQGXAX) 
 
"==iring of one MN can depress firing of the other during and shortly after the AHP==”[Page 4](zotero://open-pdf/library/items/HNFY4DSD?page=4&annotation=8N5J52MJ) 
 
![[attachments/Hurkey.etal2023_image-4-x96-y548.png]][Page 4](zotero://open-pdf/library/items/HNFY4DSD?page=4&annotation=T8GEG69U) 
 
"==Indeed, five identically, weakly electrically coupled MNs with cellular dynamics near the SNL point robustly exhibit a desynchronized splay state==”[Page 5](zotero://open-pdf/library/items/HNFY4DSD?page=5&annotation=8DUFFX9V) 
 
"==Thus, weak electrical coupling is required for network desynchronization.==”[Page 6](zotero://open-pdf/library/items/HNFY4DSD?page=6&annotation=E5ZK2JT3) 
 
"==Mathematically, these correspond to three distinct spike-onset bifurcations: the subcritical Hopf, the saddle-node-on-an-invariant cycle (SNIC) and the saddle homoclinic orbit (HOM) bifurcations==”[Page 6](zotero://open-pdf/library/items/HNFY4DSD?page=6&annotation=I5Z5ZMPS) 
 
"==Shab potassium channels constitute around 50% of the delayed rectifier current in these MNs==”[Page 6](zotero://open-pdf/library/items/HNFY4DSD?page=6&annotation=ZAKCI3BV) 
 
"==verexpression of Shab in MN1–5 causes a near doubling of Shab delayed rectifier current==”[Page 6](zotero://open-pdf/library/items/HNFY4DSD?page=6&annotation=DBWAQVL5) 
 
"==By contrast, heterogenous electrical coupling between MN1–5 (Fig. 3i) as observed in situ (Fig. 2f) produces the same preferred splay states with similar sequence statistics==”[Page 6](zotero://open-pdf/library/items/HNFY4DSD?page=6&annotation=QPWSE9R5) 
 
"==nvivo, synchronous MN firing causes 8× higher wingbeat frequency fluctuations over time compared with firing in splay state==”[Page 6](zotero://open-pdf/library/items/HNFY4DSD?page=6&annotation=JB8EG66G) 
 
"==An MN spike causes a rapid depolarization of the DLM fibre membrane==”[Page 7](zotero://open-pdf/library/items/HNFY4DSD?page=7&annotation=UMN8ZQT5) 
 
"==ollowed by a myoplasmic calcium signal with a rise time constant of around 6 ms and a decay time constant of about 80 ms==”[Page 7](zotero://open-pdf/library/items/HNFY4DSD?page=7&annotation=4Z6SKRQD) 
 
"==changes in wingbeat frequency during simultaneous MN firing should follow the same time course as changes in myoplasmic calcium across all six DLM fibres.==”[Page 7](zotero://open-pdf/library/items/HNFY4DSD?page=7&annotation=PQ3QA5T5) 
 
"==Given that each DLM fibre is innervated by one MN only (Fig. 1a), MN firing in splay state causes splayed-out calcium signals across the different muscle fibres (Fig. 4d (top)), each peaking around 6 ms after the respective MN spike and declining with a time==”[Page 7](zotero://open-pdf/library/items/HNFY4DSD?page=7&annotation=AXBHCVGL) 
 
"==By contrast, during synchronous firing of MN1–5, the calcium signals in all DLM fibres are time locked, which results in much larger calcium fluctuations across DLM fibres==”[Page 7](zotero://open-pdf/library/items/HNFY4DSD?page=7&annotation=S8ADS8JP) 
 
"==Thus, the splay state serves to minimize wing power fluctuations==”[Page 7](zotero://open-pdf/library/items/HNFY4DSD?page=7&annotation=IJFLUQY4) 
 
![[attachments/Hurkey.etal2023_image-7-x40-y554.png]][Page 7](zotero://open-pdf/library/items/HNFY4DSD?page=7&annotation=6C5WZZ24) 
 
![[attachments/Hurkey.etal2023_image-7-x360-y552.png]][Page 7](zotero://open-pdf/library/items/HNFY4DSD?page=7&annotation=8QFIP79B) 
 
![[attachments/Hurkey.etal2023_image-18-x148-y610.png]][Page 18](zotero://open-pdf/library/items/HNFY4DSD?page=18&annotation=E6L6PN6L) 
 
#📚 

%% Import Date: 2025-04-20T11:17:10.192-07:00 %%
