---
title: how to find labeled neurons in the connectome
publish: "true"
timestamp: 2025-03-17 23:28
---
finding neurons in the connectome can range in difficulty, especially between datasets. there are a few [[connectome datasets]] and the process is a little different for each. 
## flywire
if you know the cell type, the first thing i would try is to search [codex](https://codex.flywire.ai) and use different identifiers to try to find the cell of interest. you can then sift through the different search results and use community annotations to help narrow down your search. 

if you dont know the cell type, and only know the gal4 driver line name, then i would go through neuron bridge (see below)
## manc
similar to flywire, if you know the cell type or the name of the neuron, i would start searching in [neuprint](https://neuprint.janelia.org/?dataset=manc:v1.2.1&qt=findneurons)

if that doesnt work then i'd move on to neuron bridge (see below)
## fanc
working in fanc is a little different because we do not have the same infrastructure as flywire or neuprint. one option is to query the dataset using python. there are a number of cave tables with annotations of neurons that may help narrow down a cell type. 

if that does not work, you can then also try to match the gal4 driver to manc neurons using neuron bridge and then using [braincircuits.io](https://braincircuits.io) to find those neurons in fanc. i havent tried this so that might be challenging
## neuron bridge
[neuron bridge](https://neuronbridge.janelia.org) makes it relatively easy to find candidate neurons in the connectome from a light microscopy image of a genetic driver line.

just search for the driver line name and then scan through the results of **color depth search results** and try to find cell IDs that match up as best as possible. pay specific attention to different morphological traits of the neurons

#🥚 
## references
---
