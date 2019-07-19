# Reacting Wall Module
This module was developed by [ATA Engineering](http://www.ata-e.com) as an 
add-on to the Loci/CHEM computational fluid dynamics (CFD) solver. The module 
augments the **viscousWall** boundary condition in Loci/CHEM by implementing a 
two surface reaction carbon oxidation model. The module follows the process 
outlined in [1] and [2]. The two oxidation reactions modeled are shown below.

O + C -> CO  
O2 + 2C -> 2CO

The module will allow O and O2 to exit the fluid domain through a 
**viscousWall** boundary, and allow CO to enter the domain through the same 
boundary. Currently the boundary remains fixed and is not recessed to account 
for ablation.

# Dependencies
This module depends on both Loci and CHEM being installed. Loci is an open
source framework developed at Mississippi State University (MSU) by Dr. Ed 
Luke. The framework provides a rule-based programming model and can take 
advantage of massively parallel high performance computing systems. CHEM is a 
full featured open source CFD code with finite-rate chemistry built on the Loci 
framework. CHEM is export controlled under the International Traffic In Arms 
Regulations (ITAR). Both Loci and CHEM can be obtained from the 
[SimSys Software Forum](http://www.simcenter.msstate.edu) hosted by MSU.

# Obtaining The Module
The source code for the module is freely available to a restricted set of users.
For more information and to request a copy please contact mnucci@ata-e.com.

# References
[1] Driver, D. M., et al. "Understanding High Recession Rates of Carbon Ablators
Seen in Shear Tests in an Arc Jet". 48th AIAA Aerospace Sciences Meeting. 
January 4-7, 2010.

[2] Driver, D. M. and MacLean, M. "Improved Predictions of PICA Recession in Arc
Jet Shear Tests". 49th AIAA Aerospace Sciences Meeting. January 4-7, 2011.