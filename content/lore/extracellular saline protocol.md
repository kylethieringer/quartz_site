---
title: extracellular saline protocol
publish: "true"
timestamp: 2023-12-11 01:14
---
*protocol adapted from live demo by anne s. in the tuthill lab*
## recipes
- there are many recipes for chemistry of the saline. there may be pros and cons depending on the type of experiment you are doing (calcium imaging vs ephys for example)
- refer to [this excel sheet](https://docs.google.com/spreadsheets/d/1vWe8J5_-i8QxzKrDN3vg3G9fAIiUefn7QrT-BBnXkXo/edit#gid=0) for some tried and true recipes
- Here is the first recipe on the google sheet:

| ingredient     | MW        | mOsm | 6L  (g) | 1L (g) | 2L (g) | 
| -------------- | --------- | ---- | ------- | ------ | ------ |
| base readings  | --        | 117  |         |        |        |
| NaCl           | 58.443    | 103  | 36.12   | 6.02   | 12.04  |
| KCl            | 74.5513   | 3    | 1.34    | 0.22   | 0.45   |
| TES            | 229.24    | 5    | 6.88    | 1.15   | 2.29   |
| trehalose 2H20 | 378.3     | 8    | 18.16   | 3.03   | 6.05   |
| glucose        | 180.16    | 10   | 10.81   | 1.80   | 3.60   |
| NaHCO3         | 84.007    | 26   | 13.11   | 2.18   | 4.37   |
| NaH2PO4        | 137.99247 | 1    | 0.83    | 0.14   | 0.28   |
| MgCl2          | 203.3034  | 4    | 4.88    | 0.81   | 1.63   |
| CaCl2          | 147.0154  | 1.5  | 1.32    | 0.22   | 0.44   |

**final osmolarity you are shooting for with this recipe:** 270-275

the mOsm shows the contribution of each ingredient to the total osmolarity reading. the columns for 6L, 1L, and 2L describe how many grams of each ingredient (in grams) to add for each total quantity of saline batch you are making. 

## procedure
1. gather clean glassware
	- if making a 6L batch then you need a 6L flask, then 6 x 1L bottles to aliquot into at the end.
	- "clean" at the very least means that the glassware has been rinsed thoroughly with filtered water and then swished with ethanol and let dry. it doesn't hurt to autoclave glassware to be as sterile as possible but not necessary.
		- ephys experiments are sensitive to soap so be very careful cleaning glassware and try not to use detergents or rinse super well if you do
2. fill large beaker with filtered water, but much less than you need
	- if making 6L, then fill ~5.5L. this lets us dial in the final osmolarity at the end by adding water, since we know it will be too high.
	- the water should not come just straight from the tap. it should be filtered through a water purification system
3. place the large beaker on a stir plate, add a stir bar and begin stirring (~ level 3)
4. arrange the ingredients on the bench in the order listed in the table above
	- this way you can put the chemical away after you've added it to keep track of which step you are on
5. place a weigh boat on a scale and tare it
6. using a spatula, weigh out the correct amount of the ingredient to the hundredths place. 
	- try to be as exact as possible. some ingredients absorb more water than others and tend to clump (like the MgCl2) so you just have to do your best.
	- if you overshoot the weight, just scoop out and either place in a "waste" weigh boat on the side to be disposed of later, or back into original container (see note below about contamination)
7. add the ingredient to the large beaker. 
	- if you don't get all of it into the beaker, don't fret. if you weigh into the same weigh boat and tare it each time, you can wash the trace chemicals into the beaker at the end
8. continue to weigh out the chemicals and add them one at a time to the large beaker
9. once all ingredients are added, use more filtered water to wash the walls of the flask and the weigh boat to get anything not mixed in yet into solution
	- you can use a piece of parafilm to cap off the flask and shake it around to help get everything into solution
10. let the saline solution mix for a couple of minutes while you setup the osmometer
11. find a standard solution for the osmometer with a target number as close as possible to your expected osmolarity reading. 
	- if doing a full calibration, you will need standards for the low, middle, and high ranges. but this is not necessary to check each time
12. using the pipette designed to work with the osmometer, attached with a new clean tip, draw up the standard
	- you do not want a meniscus on the pipette tip. to get rid of it, hold the pipette out away from you in one hand, and a kimwipe out loosely in the other hand. using the kimwipe lightly brush the kimwipe over the pipette tip once or twice
13. take the cleaner out of the osmometer and give it a couple of twists in the process
14. insert the pipette into the osmometer and press start
	- it will go through a process of cooling and heating the sample in order to calculate the osmolarity. there will be loud obnoxious noises, that is normal
	- if the reading is off by >1 or 2, you will need to recalibrate the osmometer. refer to the operation manual of the machine to do this.
15. take the pipette out of the osmometer and quickly replace it with a fresh cleaner and twist it around a few times, then flip it around and put the cleaner back in while you prepare the next sample
16. if the osmometer reading for the standard is good, then with a new clean tip, draw up some of the saline solution and place it in the osmometer.
	- the first reading should be extremely high because we added too little water
17. if the osmolarity is too high, add a little bit of water, let it mix for a couple of minutes and then take another reading. 
	- there is a little bit of an art to knowing how much water too add. always err on the side of caution because its easier to keep adding more water than to add too much water and have to figure out what to do from there...
18. once you reach the target osmolarity, aliquot into smaller containers
19. store saline in the fridge, until ready to be used

## sources of contamination to be mindful of
---
- if glassware is not autoclaved, there may be trace amounts of alien life
- we are not a chemistry lab, and the only use for these chemicals will most likely be for making this saline. you can use the same spatula across all ingredients as long as you are mindful of this fact. if the chemicals will be used for multiple purposes, then use a clean, new spatula for each ingredient.
- there is sugar in the solution so there is always a risk of alien life forms appearing. keep in the fridge to minimize this risk. make a new batch if saline has been sitting for a while.
	- **decide on a cutoff for oldest saline we will use in the lab** - for consistency and to maintain highest quality of science!
- **current recipe does not include a sterile filtering step (like a [steritop](https://www.emdmillipore.com/US/en/product/Steritop-Filter-Units,MM_NF-C3239))** - should we add this in?
## waste disposal and cleanup
---
- none of the ingredients are toxic, so they can be disposed of in the regular trash, but maybe throw in biohazard trash just to be safe
	- **confirm with sama / ehs?? **
- dispose of the pipette tips in the sharps container just to be safe, but they are not technically a sharp
- wash out used beakers & flasks with filtered water. the waste water can go down the regular sink drain

#🐛 | [[⨳ how to]]
## references
---
[[anne sustar]]