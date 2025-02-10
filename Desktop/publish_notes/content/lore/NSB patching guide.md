---
title: NSB patching guide
publish: "true"
timestamp: 2024-04-15 10:33
---
1. setup amplifier
	- in voltage clamp dial in holding voltage to ~-50mV
	- turn switch to off -- which switch??
	- turn on seal test
2. fill patch electrode with internal saline ??
	- make sure not clogged or have any bubbles in tip
3. put electrode in bath
	- make sure pipette resistance is acceptable (8-12 mega Ohms)
	- apply positive pressure before it hits the bath!
4. slowly lower pipette toward cell of interest
5. once close to cell set speed to 5
6. switch to mouth pressure
7. approach cell with pipette
	- position pipette tip over cell
	- slowly lower tip
	- cell should dimple from positive pressure
	- release positive pressure
	- cell should rebound up to the pipette
8. oscilloscope should change from steps to transients as seal is formed
9. wait about a minute to make sure the seal is stable and that the pipette isnt drifting
10. cancel capacitance transients with fast pipette capacitance
11. set oscilloscope scale to 100mV to dial in compensation??
12. turn on voltage command by flipping the switch from off to negative
13. break into the cell with snappy suctions that slowly increase in intensity
14. you have broken into cell when capacitance transients come back
15. acquire trace for records - tells you how good access is
16. turn off seal test and flip to I=0 mode
17. aquire another trace
	- this gives good sense of overall quality of recording
	- ideally sitting at hyperpolarized potential (-30-55 is good for most cells)
	- spontaneous behavior shouldnt be too crazy
	- if things look off, hyperpolarizing current injection might fix everything
18. remove all voltage dialed in before starting experiment
	- turn holding command knob to 0
19. flip to current clamp normal 
20. dial in a bit of holding current to help cell sit at a measureable potential
	- most cells need a few pA of negative current
21. acquire a few more traces
22. begin experiment

#🥚 
## references
---
typed up version of hand written notes in tuthill lab documents
[google doc scan of original](https://drive.google.com/file/d/1vC7koAInrY_FguJsb6vziq22b1s9DbGZ/view?usp=sharing)