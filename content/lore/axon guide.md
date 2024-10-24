---
paper_title: axon guide
year: "2012"
authors: molecular devices
type: literature note
note date: 2024-03-26
modified: 
summary: 
tags: 
status: 
title: axon guide
publish: "true"
timestamp: 2024-04-15 10:34
---
# axon guide third edition
**authors**: *Molecular Devices*

## Chapter I: bioloelectricity

- electric properties of cells come from the properties of the membrane
	- membrane gets properties from lipids and proteins like ion channels
- the electrical potential difference is between the interior and exterior of the cell
	- an ion loses energy as it moves down its gradient
- units of volts
- transmembrane potentials are generated by difference across the membrane established by pumps
	- usually less than 0.1 V in animal cells (less than 100mV)

- electrical current is the flow of charge 
	- units of amperes 
- currents always flow in complete circuits
	- can flow through capacitors, resistors, ion channels, amplifiers, electrodes, etc but must be in complete circuit
- current is conserved at branch points
	- if current $I_{total}$ splits into $I_{1}$ and $I_{2}$ then $I_{total} = I_{1} + I_{2}$  

- resistors = barrier to current flow
- conductors = pathway for flow

- resistance is the inverse of conductance in Ohms law
- parallel conductances sum
	- for example with ion channels, when multiple are open simultaneously, the total conductance is the sum of the individual open channels
- the reversal potential of a channel equals the nernst potential for the permeant ion

- Ohm's law
	- the potential difference between two points linked by a current path with a conductance and current is
		- $\Delta V = IR = I/G$ 
- in extracellular recording - current is what flows between parts of a cell through external resistance produces the change in voltage. as the impulse propagates, current changes and so does the voltage
- in voltage clamp experiment - the driving force = membrane potential minus reversal potential which produces a current. As channels open and close, the conductance changes which changes the current. voltage clamp current is proportional to the number of open channels at any given time
	- each channel can change conductance incrementally
- when two resistors are connected in series, the same current passes through each of them so the voltage across each = the potential difference provided by a battery
	- potential difference is divided in proportino to 2 resistance values

- ephys recordings should:
	- accurately measure parameter of interest
	- should produce no perturbation of the parameter

- best way to measure electrical potential difference is to use voltmeter with infinite resistance
	- the best way to measure current is to open the path and insert an ammeter. if the ammeter has zero resistance it will not perturb the circuit.

- Ohms law is a linear relation between potential difference and current flow
	- applies to aqueous ionic solutions
- current is carried by anions and cations (at least one of each usually more)
- current must be transformed smoothly from a flow of electrons in the copper wire to a flow of ions in solution. 
	- most common electrode is a silver/silver chloride

- electrical field is a property of each point in space proportional to the force experienced by a charge placed at that point
	- the greater the potential difference the greater the electrical field
- the cell membrane is important for understanding concept of electrical fields
	- the transmembrane resting potential is huge but typical ephys equipment cannot measure these fields
	- instead we assume that voltage gating domains of ion channels as a proxy of the electrical excitability because it will change the conductance when channels are open or closed. 
	- the membrane is thick and a good capacitor - ability to store charge

- charge is stored in a capacitor only when there is a change in voltage across the capacitor. 
	- current flowing through is proportional to the voltage change with time
	- as long as voltage is constant, you can ignore membrane capacitance on currents
	- any change in the voltage across the membrane is accompanied by a change in the stored charge. 
		- new current first satisfies requirement for charging membrane capacitance, then it changes membrane voltage
	- the charging time constant increases when the membrane capacitance or resistance increases

- current clamp 
	- apply a known constant or time varying current and measure change in membrane potential 
	- mimics current produced by synaptic input
- voltage clamp
	- control membrane voltage and measure current required to maintain that voltage
	- does not mimic nature... but
	- it eliminates capacitive current
	- currents that flow are proportional only to membrane conductance and to number of open channels
	- channel gating is determined by transmembrane voltage alone, so voltage clamp allows you to determine the opening and closing of ion channels
- patch clamp
	- type of voltage clamp that allows one to resolve currents flowing through single ion channels
	- currents measured are very small (picoamps in single channel to nanoamps in whole cell)

- glass microelectrodes and tight seals
	- currents through the seal do not distort measured voltage or current but they do add to noise



#📚 