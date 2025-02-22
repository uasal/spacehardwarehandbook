# High-Contrast Lab Contamination Control Plan

Based on the DeMi CubeSat contamination control plan by MIT STAR Lab team members Ewan Douglas and Rachel Morgan (MIT) 

NASA source document: [NASA Marshall Contamination Control of Space Optical Systems](attachments/PD-ED-1263.pdf) (also from https://extapps.ksc.nasa.gov/Reliability/Documents/Preferred_Practices/1263.pdf)

Examples: [Hanford Contamination Control Update 2](https://dcc.ligo.org/LIGO-G1400378/public)

References: Morzinski, Katie M., Andrew P. Norton, Julia W. Evans, Layra Reza, Scott A. Severson, Daren Dillon, Marc Reinig, Donald T. Gavel, Steven Cornelissen, and Bruce A. Macintosh. 2012. “MEMS Practice: From the Lab to the Telescope.” In SPIE MOEMS-MEMS, 825304–825304. http://proceedings.spiedigitallibrary.org/proceeding.aspx?articleid=1344856.

Gushwa, K. E., & Torrie, C. I. (2014). Coming clean: understanding and mitigating optical contamination and laser induced damage in advanced LIGO. In G. J. Exarhos, V. E. Gruzdev, J. A. Menapace, D. Ristau, & M. Soileau (Eds.) (p. 923702). Presented at the SPIE Laser Damage, Boulder, Colorado, United States. https://doi.org/10.1117/12.2066909


## Cleanliness
MEMS devices and optical components are particularly susceptible to contamination, thus:

* payload assembly will occur in a class 100,000 or better cleanroom 
* installation and removal operations on an exposed MEMS device will occur under a class 1000 or better flow bench
* do not use alcohol to clean aluminum mirrors* [it reacts with the Al](Cleaning%20Optics-%20Choosing%20the%20Best%20Meth...ptical%20components%20%7C%20Photonics%20Handbook.pdf) and they have been cleaned at the factory.
* Only low-out-gassing (per https://outgassing.nasa.gov) lubricants (e.g. Bray-Coat) and adhesives (e.g. 2216 A/B Gray) will be used in the payload
* guided by NASA STD 8739-1 (WORKMANSHIP STANDARD FOR STAKING AND CONFORMAL COATING OF PRINTED WIRING BOARDS AND ELECTRONIC ASSEMBLIES, https://snebulos.mit.edu/projects/reference/NASA-Generic/NASA-STD-8739-1.pdf) Electrical components will be cleaned as appropriate and conformal coated where possible (e.g. wirebonds cannot be coated)

### Cleaning plan
* Machined and 3D printed parts in view of payload optical components will be ultrasonically cleaned in 4 steps:
   1. wipe down
   1. solvent  - acetone or dilute simple green (1 part to 10 parts distilled water) ([darthmouth method](Dartmouth%20Lynch%20Aurora%20Lab%20Ultrasonic%20Cleaning%20Procedure.pdf))
      - [Contrex AL](CONTREX%20AL%20Tech%20Sheet.pdf) (purchased from Fisher Scientific) is preferred as it has much less odor than Simple Green.  1 part to 20 parts distilled water quasi-arbitrarily. 
   1. distilled water
   1. isopropyl alcohol
* **do not put flammables in an ultrasonic cleaning tank directly, they must be in a glass container in a water bath**

### Removing dust from previously cleaned parts

**With DM removed** the pass the part under the air knife at TBD PSI TBD times or until dust is removed
to run air knife:
1. check that the tube is connected to the nitrogen tank in SSL
2. open silver top  rightmost knob (amount doesn't really matter)
3. open pressure regulator knob to between 200-500 psi (middle knob, rightmost dial)
4. open valve to 25 kPa slowly (leftmost valve, left dial)
to shut off: 
close silver rightmost knob, wait for dials to go down to zero, close those valves

### Transport

* Spacecraft and payload transport will be by white glove or hand carry
* assembled spacecraft will be sealed with low-ESD polyimide (Kapton) tape to prevent contamination during handling and transport outside of cleanrooms.


### Humidity and Electrostatic Discharge

The payload is extremely  sensitive to the conflicting hazards of electrostatic discharge and high humidity, requiring

* humidity monitoring of the spacecraft during integration
* MEMS de operation limited to humidities  between 25  \%RH and 40  \%RH (25-30 \%RH preferred)  
* technician payload handling of the powered off payload at $>40$\%RH is preferred for ESD hazard reduction.
* Payload and technician grounding at all times
* Daily testing of grounding equipment
* Static dissipative lab coats warn at all times

The above humidity operational requirements can be met with a dry air purge, and low humidity ESD risks during assembly can be mitigated with a benchtop ionizer. 
