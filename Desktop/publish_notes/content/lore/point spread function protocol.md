---
title: point spread function protocol
publish: "true"
timestamp: 2023-12-11 09:36
tags:
  - 🐛
---
Slide prep: ([https://www.nature.com/articles/nprot.2011.407](https://urldefense.com/v3/__https://www.nature.com/articles/nprot.2011.407__;!!K-Hz7m0Vt54!jjYNR4MHelynhLVeFrFuJMTHvWQVwoYPEVKsbYmglcFu5S_qnHVSwvnRsIbum1RQ0D5KZ9VAQl_O$))
1. Wash no. 1.5 cover slips by placing them in a small beaker filled with 70% (vol/vol) ethanol. Lift them out of the beaker with pointed forceps and flame them with a Bunsen burner. This will create a hydrophilic surface on the glass, thus allowing the microsphere droplets to spread and create an even distribution of microspheres on the glass. Set this glass slide aside
2. Add some distilled water (or EtOH) in clean beaker
3. Grab pipetter that can take up 0.1-0.5 uL and 10-50 uL
4. Pipette 60 uL of water (70% EtOH also works, probably 100% as well) and ~0.5 uL of beads into a mixing tube and mix
5. Vortex or sonicate for 20-30 min
6. Pipette mixture onto glass slide and let it dry in fume hood

Imaging with Insight (imaging) protocol
1. Position grin lens under objective and level
2. Use stage with adjustable Z to elevate slide with beads underneath the GRIN lens aroun 200 um away or as close as possible by eye
3. Move slide or agar around relative to lens in X/Y and watch epicam for when beads comes into view. May be difficult to see - they are very small

4. Switch to scope and PMTs
5. Adjust bead position relative to GRIN lens bottom as desired by alternating back and forth imaging with PMT and opening up the enclosure
6. Zoom into bead around 7x
7. Perform z stack with 0.2 um resolution

Bruker protocol
1. Make a fluorescent micro-bead slide for testing
	1. Pipette 500uL ethanol into a microcentrifuge tube
	2. Vortex a vial of premixed fluorescent micro-bead concentration
	3. pipette 1-2 uL of the bead concentrate into the microcentrifuge tube
	4. Vortex the microcentrifuge tube
	5. Using the pipette, apply the ethanol/bead mixture to microscope slides
	6. let the slide dry for a few minutes
	7. rinse the slides to free any beads not stuck to the surface - gently drop some tap water on the slide and flick the water off
	8. let the slide dry before use. Keep in a light proof container at all times
2. Using an api-light source and a GFP emission cube, find the beads using the eyepieces
3. Image the beads using 820nm 2P beam on a green imaging channel
	- Use a calibrated 40x objective
	- apply 4-8x optical zoom to find the beads
	- apply 16x optical zoom once the beads are in the field of view
4. perform a Z-series from above the bead to below the bead at .2um increments
5. Open the Z-series in ImageJ > Plugins > input-output > Prairie Reader
6. select a square region around one bead and crop the image to only display one bead
7. go to ImageJ > Plugins > MetroloJ > Generate PSF Report
	- the psf report will be saved as a pdf document in the image folder it was generated from

#🐛  | [[⨳ how to]]
## references
---
[[charles zhou]] shared this with me