---
paper_title: Flight cessation and modulation control of coleopteran employing wireless miniature muscular stimulators
year: "2022"
authors: Yongchang Jiang, Bo Yang, Ye Jiang, Wenhao Zhao, Xin Guo
type: literature note
note date: 2024-09-05
modified: 
summary: 
tags: 
status: 
title: Jiang.etal2022
publish: "true"
timestamp: 2024-09-05 11:44
---
# Flight cessation and modulation control of coleopteran employing wireless miniature muscular stimulators
**authors**: *Yongchang Jiang, Bo Yang, Ye Jiang, Wenhao Zhao, Xin Guo*
**doi**: 10.1177/00202940221098047

> [!INFO] CITATION
> Jiang, Y., Yang, B., Jiang, Y., Zhao, W., & Guo, X. (2022). Flight cessation and modulation control of coleopteran employing wireless miniature muscular stimulators. _Measurement and Control_, _55_(7–8), 821–829. [https://doi.org/10.1177/00202940221098047](https://doi.org/10.1177/00202940221098047)

> [!NOTE] ABSTRACT
>
> Recently, the combination of electronic devices with living insects has been explored to manipulate their crawling or flying, similar to manipulable biological actuators. However, the investigations of controlled flight cessation or flight modulation of the coleopteran characterized by the strong payload capacity have rarely been reported thus far. On the basis of anatomy, this study proposed and validated two separate muscular electrical stimulation protocols to stop and modulate the flight of coleopteran, respectively. The experiment results demonstrated that the suggested cessation protocol realized flight cessation control with a success rate of 83% and a short response time. Meanwhile, the flight modulation stimulation protocol was able to increase the flapping frequency by an average of 7.3%. Finally, we designed a wireless miniature backpack weighing 1 gram to actuate the flight cessation and modulation of coleopteran in free-flying through the remote command transmission. The proposed method has potential applications in the development of the insect-cyborg micro air vehicle.  

## fleeting notes
---
%% begin notes %% 

references to check out:
- https://doi.org/10.1242/jeb.037465
- https://iopscience.iop.org/article/10.1088/1748-3190/aa934b/meta
- http://dx.doi.org/10.1109/TBME.2009.2022551

- coleopteran = beetles
- insect machine interface - IMI - directly manipulates insects movements

- underlying motivation of study is to control where the insect lands by stopping flight

landing flight cessation studies:
- Evangelista C, Kraft P, Dacke M, et al. The moment before touchdown: landing manoeuvres of the honeybee Apis mellifera. J Exp Biol 2010; 213(2): 262–270. https://doi.org/10.1242/jeb.037465
- Shen C and Sun M. Wing and body kinematics measurement and force analyses of landing in fruit flies. Bioinspiration & Biomimetics 2017; 13(1): 016004 https://iopscience.iop.org/article/10.1088/1748-3190/aa934b/meta

[[bio robotic research coarsely demonstrate flight cessation with implanted neural stimulations in large insects]]

flight cessation by stimulating antennal lobe in manduca sexta (tobacco hornworm)
- Bozkurt A, Gilmour RF and Lal A. Balloon-assisted flight of radio-controlled insect biobots. IEEE Trans Biomed Eng 2009; 56(9): 2304–2307. http://dx.doi.org/10.1109/TBME.2009.2022551
flight cessation by stimulating beetle optic lobes, central complex, or ventral nerve cord
- Sato H, Berry CW, Maharbiz MM. Flight control of 10 gram insects by implanted neural stimulators. 2008 Solid-State, Actuators, and Microsystems Workshop, 2008, 90–91 
- Van Truong T, Byun D, Lavine LC, et al. Flight behavior of the rhinoceros beetle Trypoxylus dichotomus during electrical nerve stimulation. Bioinspir Biomim 2012; 7(3): 036021.
biobots - flight cessation:
- Chung AJ, Cordovez B, Jasuja N, et al. Implantable microfluidic and electronic systems for insect flight manipulation. Microfluidics and Nanofluidics 2012; 13(2): 345–352

used a cutoff of flight cessation of 2s as successful trial, otherwise a failed trial

inserted electrodes into the DLMs and DVMs and injected a pulse train at 50Hz 50% duty cycle 1 s duration to stop flight - varied the intensity to obtain flight cessation

[[coordinated activity of the flight power muscles are critical for flight]]

when stimulating the DLM and DVMs - they saw wings flapping angle decrease, and the forelegs and middle legs fell underneath the thorax

stimulus injection disrupted the oscillating muscles of the DLMs and DVMs by activating both muscles together rather than how they naturally alternate
- induced a tetanic contraction state

-  **this could be a good possible mechanism for inducing flight cessation in flies -- changing the timing of muscle contraction as opposed to muscle inhibition**
	- one circuit mechanism (that seems maybe less likely) is that there are two complimentary circuits for each muscle group and flight cessation is the activation of the complimentary circuit during the each stage of the wingstroke - so inhibition through muscle activation???

- insects modulate wingbeat frequency by tensioning their thorax (changing stiffness) through the pleurosternal muscle 
	- Machin KE and Pringle JWS. The physiology of insect fibrillar muscle-ii mechanical properties of a beetle flight muscle. Proc R Soc Lond Ser B Biol Sci 1959; 151(943): 204–225.
	- Dickinson MH and Tu MS. The function of dipteran flight muscle. Comp Biochem Physiol A: Physiol 1997; 116(3): 223–238.

[[the pleurosternal muscle tensions the thorax]]
- are there any pleurosternal muscle motor neurons in the connectome?
%% end notes %% 
## highlights
---
"==In most insects, such as bees and fruit flies, the flapping stops immediately after touchdown==”[Page 1](zotero://open-pdf/library/items/ZKTWX2GC?page=1&annotation=7PCDG68Q) 

 
"==Researchers have demonstrated several controllable flight cessation in insects through a wide spectrum of neural actuation mechanisms.==”[Page 1](zotero://open-pdf/library/items/ZKTWX2GC?page=1&annotation=4NYC5E2B) 

 
"==Similarly, the same cessation behavior could be realized in Manduca sexta through stimulating the antennal lobe.15 The stimulus on the beetle’s optic lobes16 or simultaneously on the brain central complex and ventral nerve cords17 could also stop its flying behavior. Nevertheless, the optic lobe stimulation will inevitably impair the photoreception of the beetles and thereby cause flight discontinuity.==”[Page 1](zotero://open-pdf/library/items/ZKTWX2GC?page=1&annotation=LDD289ZM) 

 
"==medication injections to paralyze the dorsoventral muscles (DVMs) and the dorsal longitudinal muscles (DLMs) as these two muscles are responsible for powering the wing beat.==”[Page 2](zotero://open-pdf/library/items/ZKTWX2GC?page=2&annotation=M49H57F6) 

 
"==he potential of those muscles (DLM and DVM) on flight cessation has not been explored thus far.==”[Page 2](zotero://open-pdf/library/items/ZKTWX2GC?page=2&annotation=WNPF54R4) 

 
"==If the beetle stopped flapping within 2 s, we recorded it as a successful trial, otherwise as a failed trial==”[Page 4](zotero://open-pdf/library/items/ZKTWX2GC?page=4&annotation=IKNUARWR) 

 
"==Notably, the flapping angle decreased rapidly, and forelegs and middle legs fell underneath the thorax after the DLM-DVM combined stimulation.==”[Page 5](zotero://open-pdf/library/items/ZKTWX2GC?page=5&annotation=DI9Y4UD8) 

 
![[attachments/Jiang.etal2022_image-6-x271-y620.png]][Page 6](zotero://open-pdf/library/items/ZKTWX2GC?page=6&annotation=TUYQ2IBF) 

 
"==the stimulus decoupled the oscillation state established by the alternate contraction of the DVMs and DLMs. The electrical stimulation activated two muscles together, which induced the muscles in a tetanic contractions state.==”[Page 7](zotero://open-pdf/library/items/ZKTWX2GC?page=7&annotation=FPTN48YF) 

 
"==Previous articles have suggested that insects modulated their wingbeat frequency by tensioning their thorax (increasing the stiffness) via pleurosternal muscle contraction==”[Page 7](zotero://open-pdf/library/items/ZKTWX2GC?page=7&annotation=DEGYATFS) 

 
#📚 

%% Import Date: 2024-09-05T11:33:16.092-07:00 %%
