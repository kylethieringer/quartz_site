---
title: unsupervised clustering of calcium imaging data
publish: "true"
timestamp: 2023-12-11 09:37
tags:
  - 🐛
  - 🌱
---
1. pull out single pixel responses in each imaging plane (assuming there is structural registering first?)
2. discard unresponsive pixels
3. pool pixels across z-planes, and animals
4. discard uncorrelated pixels because they probably just contain a lot of noise
5. define functional clusters based on the correlation of responses of each pixel

Benefits of this method:
- no assumption about what stimulus features define the functional differences
- functional types are defined by the activity not by spatial location
- cross brain similarity can be used as a check that the clustering algorithm works


#🐛  | #🌱 
## references
---
[[Patella.Wilson2018]]