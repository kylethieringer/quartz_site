---
paper_title: Mapping model units to visual neurons reveals population code for social behaviour
year: "2024"
authors: Benjamin R. Cowley, Adam J. Calhoun, Nivedita Rangarajan, Elise Ireland, Maxwell H. Turner, Jonathan W. Pillow, Mala Murthy
type: literature note
note date: 2025-04-22
modified: 
summary: 
tags: 
status: 
title: Cowley.etal2024
publish: "true"
timestamp: 2025-04-22 12:44
---
# Mapping model units to visual neurons reveals population code for social behaviour
**authors**: *Benjamin R. Cowley, Adam J. Calhoun, Nivedita Rangarajan, Elise Ireland, Maxwell H. Turner, Jonathan W. Pillow, Mala Murthy*
**doi**: 10.1038/s41586-024-07451-8

> [!INFO] CITATION
> Cowley, B. R., Calhoun, A. J., Rangarajan, N., Ireland, E., Turner, M. H., Pillow, J. W., & Murthy, M. (2024). Mapping model units to visual neurons reveals population code for social behaviour. _Nature_, _629_(8014), 1100–1108. [https://doi.org/10.1038/s41586-024-07451-8](https://doi.org/10.1038/s41586-024-07451-8)

> [!NOTE] ABSTRACT
>Abstract The rich variety of behaviours observed in animals arises through the interplay between sensory processing and motor control. To understand these sensorimotor transformations, it is useful to build models that predict not only neural responses to sensory input 1–5 but also how each neuron causally contributes to behaviour 6,7 . Here we demonstrate a novel modelling approach to identify a one-to-one mapping between internal units in a deep neural network and real neurons by predicting the behavioural changes that arise from systematic perturbations of more than a dozen neuronal cell types. A key ingredient that we introduce is ‘knockout training’, which involves perturbing the network during training to match the perturbations of the real neurons during behavioural experiments. We apply this approach to model the sensorimotor transformations of Drosophila melanogaster males during a complex, visually guided social behaviour 8–11 . The visual projection neurons at the interface between the optic lobe and central brain form a set of discrete channels 12 , and prior work indicates that each channel encodes a specific visual feature to drive a particular behaviour 13,14 . Our model reaches a different conclusion: combinations of visual projection neurons, including those involved in non-social behaviours, drive male interactions with the female, forming a rich population code for behaviour. Overall, our framework consolidates behavioural effects elicited from various neural perturbations into a single, unified model, providing a map from stimulus to neuronal cell type to behaviour, and enabling future incorporation of wiring diagrams of the brain 15 into the model. 
>  
## fleeting notes
---
%% begin notes %% 

want to build a model that predicts neural responses to sensory input and also how each neuron contributes to behavior

one-to-one mapping between internal units of a deep neural network and real neurons by predicting behavior that arises from silencing cells

population of visual neurons drive social interactions

use a new method called knockout training - to show how each internal unit of a DNN can prdict behavior of an animal that has a similar perturbation

the model infers neural activity from behavior alone

the visual system has a bottleneck - visual projectino neurons
- there are 200 cell types
- 57 LC types identified so far

DNN model
- convolutional vision network
- bottleneck layer of LC units - each LC unit represents the summed activity of neurons of the same LC type (activity of an optic glomerulus)
- a decision netowrk with dense connections that map LC responses to behavior

did not put biological constraints on the model to improve predictability. wanted to explain LC function

collected natural courtship data from LC silenced males
- then trained model. setting LC unit in model to zero for each particular LC silenced cell type

trained model with inputs of visual input to the male during courtship. output of male movement and song production

the 1-to-1 network estimated male behavior from visual input alone

then looked at neural responses. chose a subset that had the largest effects on behavior during silencing

the network was able to predict LC responses just from behavior of both naturalistic and artificial stimuli

population of model LC units all respond to female position size and rotation and no model LC unit encoded a single visual parameter

almost all units encoded some nonlinear interaction among three visual parameters

model LC units encode visual stimuli in a distributed way - each stimulus feature is encoded by mulitple LC units

multiple LC units contributed to each behavior of the male fly
- LC contributions may change with context

[[distributed LC neurons cooperate to encode visual stimuli]]

%% end notes %% 
## highlights
---
"==combinations of visual projection neurons, including those involved in non-social behaviours, drive male interactions with the female, forming a rich population code for behaviour.==”[Page ](zotero://open-pdf/library/items/G6TNPMW2?page=&annotation=IRFZHWWU) 
 
"==Here we overcome this drawback by perturbing the internal units of a DNN model while predicting the behaviour of animals whose neurons have also been perturbed, a method that we call knockout training. This approach places a strong constraint on the model: each model unit must contribute to behaviour in a way that matches the causal contribution of the corresponding real neuron to behaviour.==”[Page ](zotero://open-pdf/library/items/G6TNPMW2?page=&annotation=RZMHHQEL) 
 
"==The primary cell types of this bottleneck (Fig. 1a) are the 57 lobula columnar (LC) and lobula plate (LPLC) neuron types identified so far (we use ‘LC types’ to refer both to LC and LPLC neuron types), making up about 3.5% of all neurons in the brain==”[Page ](zotero://open-pdf/library/items/G6TNPMW2?page=&annotation=D6X3IH2M) 
 
"==Neurons of a single LC type innervate only one optic glomerulus in the posterior lateral protocerebrum==”[Page ](zotero://open-pdf/library/items/G6TNPMW2?page=&annotation=EZYM9WK6) 
 
"==we explored whether the representation of the female during courtship might be distributed across the LC population, and similarly whether multiple LC types might be required to drive behaviour==”[Page 2](zotero://open-pdf/library/items/G6TNPMW2?page=2&annotation=IMP4LUQM) 
 
"==he DNN model has three components: (1) a front-end convolutional vision network that reflects processing in the optic lobe;  (2) a bottleneck layer of LC units in which each model LC unit represents the summed activity of neurons of the same LC type (that is, the overall activity level of an optic glomerulus); and (3) a decision network with dense connections that maps LC responses to behaviour, reflecting downstream processing in the central brain and ventral nerve cord==”[Page 2](zotero://open-pdf/library/items/G6TNPMW2?page=2&annotation=ZWW99FG3) 
 
"==ur goal was to identify a one-to-one mapping between model LC units and LC neuron types.==”[Page 2](zotero://open-pdf/library/items/G6TNPMW2?page=2&annotation=XKSM4H78) 
 
"==silencing LC10a neurons resulted in failures to initiate chasing, as male-to-female distances remained large over time==”[Page 3](zotero://open-pdf/library/items/G6TNPMW2?page=3&annotation=VG7VIUV2) 
 
"==silencing LC6 and LC26 neurons resulted in stronger and more persistent chasing==”[Page 3](zotero://open-pdf/library/items/G6TNPMW2?page=3&annotation=7DXS7VP3) 
 
"==the silencing of any single LC type did not match the behavioural deficits of blind flies==”[Page 3](zotero://open-pdf/library/items/G6TNPMW2?page=3&annotation=CGK62LHK) 
 
"==The model inputs were videos of the visual input of the male fly during natural courtship==”[Page 3](zotero://open-pdf/library/items/G6TNPMW2?page=3&annotation=ADIJVTH8) 
 
"==omprised the male movements==”[Page 3](zotero://open-pdf/library/items/G6TNPMW2?page=3&annotation=LJM6FVK7) 
 
"==nd song production==”[Page 3](zotero://open-pdf/library/items/G6TNPMW2?page=3&annotation=YXCNMSTN) 
 
"==The 1-to-1 network reliably predicted these behavioural variables in held-out data==”[Page 3](zotero://open-pdf/library/items/G6TNPMW2?page=3&annotation=KZPXNNJF) 
 
"==he 1-to-1 network reliably estimated the behaviour of the male from visual input alone, even for male flies with a silenced LC type==”[Page 3](zotero://open-pdf/library/items/G6TNPMW2?page=3&annotation=M94BFQCX) 
 
"==We found that the recorded LC neurons responded to many of these naturalistic stimulus sequence==”[Page 3](zotero://open-pdf/library/items/G6TNPMW2?page=3&annotation=4J3NJ6H5) 
 
"==The prediction performance of the 1-to-1 network was consistent with our expectations—exact matches were unlikely owing to differences in behavioural state during courtship (on which the 1-to-1 network was trained) and during imaging==”[Page 3](zotero://open-pdf/library/items/G6TNPMW2?page=3&annotation=6Q9APNUF) 
 
"==The 1-to-1 network was the most consistent in its neural predictions (across ten different random initializations) compared with other training procedures (Extended Data Fig.6), suggesting that knockout training converges to a similar solution despite a different initialization==”[Page 3](zotero://open-pdf/library/items/G6TNPMW2?page=3&annotation=REF9QBEA) 
 
"==We found that the majority of model LC units in the 1-to-1 network responded to changes in female position, size and rotation (Fig. 3a). Moreover, almost no model LC unit directly encoded any single visual parameter==”[Page 3](zotero://open-pdf/library/items/G6TNPMW2?page=3&annotation=GXCIRTCY) 
 
"==Most model LC units encoded changes in female position (Fig. 3e, orange bars), roughly half encoded female size (Fig. 3e, blue bars), and female rotation was weakly encoded (Fig. 3e, green bars are small). However, almost all model LC units encoded some nonlinear interaction among the three visual parameters==”[Page 4](zotero://open-pdf/library/items/G6TNPMW2?page=4&annotation=WAQTTTJI) 
 
"==hat most model LC units encode some aspect of female size, position and rotation==”[Page 4](zotero://open-pdf/library/items/G6TNPMW2?page=4&annotation=SYS3KIH5) 
 
"==the model LC units encode visual stimuli in a distributed way: each visual stimulus feature is encoded by multiple model LC units==”[Page 4](zotero://open-pdf/library/items/G6TNPMW2?page=4&annotation=KNKIYM4M) 
 
"==The inactivated model LC units that led to the largest drops in performance were the strongest contributors to each behaviour==”[Page 5](zotero://open-pdf/library/items/G6TNPMW2?page=5&annotation=BGTF5M82) 
 
"==most model LC units contributed to multiple behavioural outputs==”[Page 5](zotero://open-pdf/library/items/G6TNPMW2?page=5&annotation=7K2G28VG) 
 
"==each behavioural output was driven by multiple LC units==”[Page 5](zotero://open-pdf/library/items/G6TNPMW2?page=5&annotation=9I7GIHGF) 
 
"==multiple LC units contributed to each behaviour==”[Page 6](zotero://open-pdf/library/items/G6TNPMW2?page=6&annotation=M9Q23VWB) 
 
"==LC contributions change with context.==”[Page 6](zotero://open-pdf/library/items/G6TNPMW2?page=6&annotation=W6XEAVJG) 
 
"==model LC units encode multiple visual features of the female (Fig. 5a, left connections) and contribute to multiple behavioural outputs==”[Page 6](zotero://open-pdf/library/items/G6TNPMW2?page=6&annotation=A6Y74FPP) 
 
"==A key prediction of our 1-to-1 network is that LC neuron types share common inputs in the optic lobe (creating shared feature tuning across the LC population) and converge onto shared downstream targets to drive behaviour.==”[Page 6](zotero://open-pdf/library/items/G6TNPMW2?page=6&annotation=X7PBJ4T2) 
 
![[attachments/Cowley.etal2024_image-6-x273-y448.png]][Page 6](zotero://open-pdf/library/items/G6TNPMW2?page=6&annotation=MSZMK3HI) 
 
"==The 1-to-1 network is the first large-scale hypothesis of how the LC types work together to encode stimuli==”[Page 7](zotero://open-pdf/library/items/G6TNPMW2?page=7&annotation=SM5P8LVE) 
 
"==Future experiments are needed to understand how the same LC cell type can contribute to different behaviours in different contexts==”[Page 8](zotero://open-pdf/library/items/G6TNPMW2?page=8&annotation=9VXTNGY9) 
 
"==n intriguing future direction is to apply this framework to other bottlenecks within the Drosophila brain, such as the descending and ascending neurons that link the brain and nerve cord==”[Page 8](zotero://open-pdf/library/items/G6TNPMW2?page=8&annotation=5A4URXKM) 
 
#📚 

%% Import Date: 2025-04-22T11:56:27.151-07:00 %%
