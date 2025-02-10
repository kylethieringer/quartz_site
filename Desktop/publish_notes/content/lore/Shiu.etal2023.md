---
paper_title:
  - A leaky integrate-and-fire computational model based on the connectome of the entire adult <i>Drosophila</i> brain reveals insights into sensorimotor processing
title: Shiu.etal2023
year: "2023"
authors: Philip K. Shiu, Gabriella R. Sterne, Nico Spiller, Romain Franconville, Andrea Sandoval, Joie Zhou, Neha Simha, Chan Hyuk Kang, Seongbong Yu, Jinseop S. Kim, Sven Dorkenwald, Arie Matsliah, Philipp Schlegel, Szi-chieh Yu, Claire E. McKellar, Amy Sterling, Marta Costa, Katharina Eichler, Gregory S.X.E. Jefferis, Mala Murthy, Alexander Shakeel Bates, Nils Eckstein, Jan Funke, Salil S. Bidaye, Stefanie Hampel, Andrew M. Seeds, Kristin Scott
type: literature note
note date: 2023-11-06
modified: 
summary: 
tags:
  - 📚
status: 
publish: "true"
timestamp: 2023-12-11 09:36
---

# A leaky integrate-and-fire computational model based on the connectome of the entire adult <i>Drosophila</i> brain reveals insights into sensorimotor processing
**authors**: *Philip K. Shiu, Gabriella R. Sterne, Nico Spiller, Romain Franconville, Andrea Sandoval, Joie Zhou, Neha Simha, Chan Hyuk Kang, Seongbong Yu, Jinseop S. Kim, Sven Dorkenwald, Arie Matsliah, Philipp Schlegel, Szi-chieh Yu, Claire E. McKellar, Amy Sterling, Marta Costa, Katharina Eichler, Gregory S.X.E. Jefferis, Mala Murthy, Alexander Shakeel Bates, Nils Eckstein, Jan Funke, Salil S. Bidaye, Stefanie Hampel, Andrew M. Seeds, Kristin Scott*
**doi**: https://doi.org/10.1101/2023.05.02.539144

> [!INFO] CITATION
> Shiu, P. K., Sterne, G. R., Spiller, N., Franconville, R., Sandoval, A., Zhou, J., Simha, N., Kang, C. H., Yu, S., Kim, J. S., Dorkenwald, S., Matsliah, A., Schlegel, P., Yu, S., McKellar, C. E., Sterling, A., Costa, M., Eichler, K., Jefferis, G. S. X. E., … Scott, K. (2023). _A leaky integrate-and-fire computational model based on the connectome of the entire adult Drosophila brain reveals insights into sensorimotor processing_ [Preprint]. Neuroscience. [https://doi.org/10.1101/2023.05.02.539144](https://doi.org/10.1101/2023.05.02.539144)

> [!NOTE] ABSTRACT
>Abstract
>The forthcoming assembly of the adult Drosophila melanogaster central brain connectome, containing over 125,000 neurons and 50 million synaptic connections, provides a template for examining sensory processing throughout the brain. Here, we create a leaky integrate-and-fire computational model of the entire Drosophila brain, based on neural connectivity and neurotransmitter identity, to study circuit properties of feeding and grooming behaviors. We show that activation of sugar-sensing or water-sensing gustatory neurons in the computational model accurately predicts neurons that respond to tastes and are required for feeding initiation. Computational activation of neurons in the feeding region of the Drosophila brain predicts those that elicit motor neuron firing, a testable hypothesis that we validate by optogenetic activation and behavioral studies. Moreover, computational activation of different classes of gustatory neurons makes accurate predictions of how multiple taste modalities interact, providing circuit-level insight into aversive and appetitive taste processing. Our computational model predicts that the sugar and water pathways form a partially shared appetitive feeding initiation pathway, which our calcium imaging and behavioral experiments confirm. Additionally, we applied this model to mechanosensory circuits and found that computational activation of mechanosensory neurons predicts activation of a small set of neurons comprising the antennal grooming circuit that do not overlap with gustatory circuits, and accurately describes the circuit response upon activation of different mechanosensory subtypes. Our results demonstrate that modeling brain circuits purely from connectivity and predicted neurotransmitter identity generates experimentally testable hypotheses and can accurately describe complete sensorimotor transformations. 


### fleeting notes
---

- 125,000 neurons and 50 million synapses in the drosophila central brain connectome
- a single neuron can have hundreds of downstream neurons

- leaky integrate and fire model using the connection weights from the connectome and NT predictions
	- spiking of a neuron alters membrane potential of downstream neurons in proportion to the connectivity from the upstream neuron
	- if downstream neuron reaches threshold, that neuron fires
	- baseline firing in model is 0 Hz
- examined feeding initiation and antennal grooming with the model



feeding initiation
- appetitive substances results in proboscis extension
- gustatory receptor neurons on the body surface respond to tastants and project to the SEZ
- focused on Ir94e - neurons responds to sugar, water, bitter and low salt
- activation of GRNs results in activation of motor neuron 9 (MN9)
- unilateral sugar GRN activation more strongly activates contralateral MN9
- these results were consistent in behavior and the model

- examined netowrk activity upon GRN activation ranging from 10-200hz
	- increasing GRN firing rate increases activity of MN9
- computationally stimulated top 200 responding neurons in the network to identify which drive activity in MN9
- then silenced top 200 neurons and activated sugar GRNs to see which were required for MN9 firing
	- found 44 neurons that drive MN9 but only 14 that are required

- 10 neuron classes that respond to sugar
	- 8 are correctly predicted to activate MN9 in the model
- 5 are required for sugar feeding
	- 3 of the 5 are predicted by the model
- this discrepency might be because the basal firing rate of the neurons in the model is set to 0

- to behaviorally confirm model, they did a screen activating 138 cell types with split gal4 lines
	- this labels a third of SEZ neurons
	- identified  106 cell types in flywire
	- 11 are predicted to activate MN9 and 10 actually do
	- model performs better that 90% accuracy

- Ir94e - mediate attraction to low salt concentration
- Ir94e GRNs inhibit MN9 firing in the model
- optogenetic activation inhibits proboscis extension

- noticed differences in Ir94e and bitter responses in the model. 
	- bitter activation eliminated consumption of 1M sucrose but Ir94e did not

- activation of water GRNs activates neurons also activated by sugar stimulation

- also tested grooming circuits
	- activation of mechanosensory neurons in antenna (JONs) elicits grooming
	- synapse onto 2 interneurons -- aBN1 and aBN2
	- these synapse onto aDN1 and aDN2
- computational model identified aBN1, aBN2, aDN1, and aDN2 respond to JON activation
- used activity of the aDN1 and DN2 as a proxy for grooming
- model predicts the correct nodes of the grooming circuit

- JO-C and JO-E and JO-F respond to antennal vibrations
	- JO-CE and JO-F drive grooming, both synapse onto aBN1
- model predicts JO-CE elicits aBN1 activity but JO-F does not
	- this holds up experimentally as well

