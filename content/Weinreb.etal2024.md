---
paper_title: "Keypoint-MoSeq: parsing behavior by linking point tracking to pose dynamics"
year: '2024'
authors: "Caleb Weinreb, Jonah E. Pearl, Sherry Lin, Mohammed Abdal Monium Osman, Libby Zhang, Sidharth Annapragada, Eli Conlin, Red Hoffmann, Sofia Makowska, Winthrop F. Gillis, Maya Jay, Shaokai Ye, Alexander Mathis, Mackenzie W. Mathis, Talmo Pereira, Scott W. Linderman, Sandeep Robert Datta"
type: literature note
note date: '2025-04-25'
modified: 
summary: 
tags: []
status:
---
# Keypoint-MoSeq: parsing behavior by linking point tracking to pose dynamics
**authors**: *Caleb Weinreb, Jonah E. Pearl, Sherry Lin, Mohammed Abdal Monium Osman, Libby Zhang, Sidharth Annapragada, Eli Conlin, Red Hoffmann, Sofia Makowska, Winthrop F. Gillis, Maya Jay, Shaokai Ye, Alexander Mathis, Mackenzie W. Mathis, Talmo Pereira, Scott W. Linderman, Sandeep Robert Datta*
**doi**: 10.1038/s41592-024-02318-2

> [!INFO] CITATION
> Weinreb, C., Pearl, J. E., Lin, S., Osman, M. A. M., Zhang, L., Annapragada, S., Conlin, E., Hoffmann, R., Makowska, S., Gillis, W. F., Jay, M., Ye, S., Mathis, A., Mathis, M. W., Pereira, T., Linderman, S. W., & Datta, S. R. (2024). Keypoint-MoSeq: Parsing behavior by linking point tracking to pose dynamics. _Nature Methods_, _21_(7), 1329–1339. [https://doi.org/10.1038/s41592-024-02318-2](https://doi.org/10.1038/s41592-024-02318-2)

> [!NOTE] ABSTRACT
>Abstract Keypoint tracking algorithms can flexibly quantify animal movement from videos obtained in a wide variety of settings. However, it remains unclear how to parse continuous keypoint data into discrete actions. This challenge is particularly acute because keypoint data are susceptible to high-frequency jitter that clustering algorithms can mistake for transitions between actions. Here we present keypoint-MoSeq, a machine learning-based platform for identifying behavioral modules (‘syllables’) from keypoint data without human supervision. Keypoint-MoSeq uses a generative model to distinguish keypoint noise from behavior, enabling it to identify syllables whose boundaries correspond to natural sub-second discontinuities in pose dynamics. Keypoint-MoSeq outperforms commonly used alternative clustering methods at identifying these transitions, at capturing correlations between neural activity and behavior and at classifying either solitary or social behaviors in accordance with human annotations. Keypoint-MoSeq also works in multiple species and generalizes beyond the syllable timescale, identifying fast sniff-aligned movements in mice and a spectrum of oscillatory behaviors in fruit flies. Keypoint-MoSeq, therefore, renders accessible the modular structure of behavior through standard video recordings. 
>  
## fleeting notes
---
%% begin notes %% 

keypoint data is susceptible to high frequency jitter that clustering algorithms mistake for transitions

kepoint moseq finds syllables from keypoint data - unsupervised

uses a generative model to distinguish noise from behavior

MoSeq
- uses unsupervised classificaiton of 3D videos (depth vids) into motifs
- to find syllables - it finds discontinuities in behavior at timescale set by user
- influences the frequency that syllabels can transition
- in mice - sub second and second timscale is good for boundaries
- depth cameras are difficult to use!
- using keypoints as inputs has been tricky because of the jitter in estimates which gets mistaken for transitions

redeveloped the moseq model to capture behavioral syllables at mulitple timescales 

similar sub second discontinuities were present in depth and keypoint models

keypoint model used on moseq had a ton of high frequency fluctuations from tracking artifacts
- smoothing did not get rid of this. it blurred true transitions and made it difficult to detect syllable boundaries
- 

keypoint moseq produces different syllables each time it runs
- so run multiple interations and fit a likelihood metric

unsupervised classification of behavior - learn how the brain generates self motivated behaviors
- boundaries serve as timestamps for alignment
- found that dopamine dynamics increased at onset of syllables defined by moseq
	- this suggests that moseq syllables could be used as landmarks for neural data analysis

keypoint moseq generalized across experimental setups and species

keypoint moseq handles tracking errors for behavioral classification
- infers noise from learned patterns of animal motion

%% end notes %% 
## highlights
---
#📚 

%% Import Date: 2025-04-25T14:46:21.358-07:00 %%
