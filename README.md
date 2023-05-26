# Enhancing Nanohinge Functionality: Self-Assembly of a Repeatable DNA Hinge System Supporting Higher Order Structure Formation

### Primary Contributors/Contact for Inquiries
| Name | Description/Contribution | Contact |
| ---- | ------------------------ | ------- | 
|UBC BIOMOD| Team email - for general project related inquiries | ubcbiomod@gmail.com | 
| Fumiya Inaba | Primary contributor to [caDNAno Design Validation Tool](https://github.com/ubcbiomod/caDNAno-Design-Validation-Tool-Nanoval), design team co-lead of this project | fumiy@student.ubc.ca | 
| Charlie Sushams | Provided guidance on MATLAB usage/integration into pipeline, code reviewer, design team co-lead of this project | charliesushams@gmail.com |
| Ethan Rajkumar | Primary contributor to Kinetic_trap_detection and Sandwich_strand_detection Jupyter notebooks | ethanrajkumar2001@gmail.com | 

## Description
This repository contains code which was used in the project <i>Enhancing Nanohinge Functionality: Self-Assembly of a Repeatable DNA Hinge System Supporting Higher Order Structure Formation</i>. A cleaner packaged version of this code is available in the [nanoval repo](https://github.com/ubcbiomod/caDNAno-Design-Validation-Tool-Nanoval) as a command-line interface application.   

## Kinetic Trap Detection 
### Overview:
To optimize the folding of H1 and H2 hinges, python scripts were made to assess the presence of kinetic traps in cadnano outputs. 
### Background:
Kinetic traps result from excess mechanical strain which refers to the energy stored in bent or twisted structures programmed (internal energy) to occur by engineering staple crossovers at certain helix locations. We need to ensure that a structure is the one with the most minimal Gibbs Free Energy. This is not so easy with DNA origami structures. The structure can be caught in smaller energy minima as it seeks to minimize its internal energy and maximize its entropy. Kinetic traps are an issue because if a scaffold strand bends to make a crossover, a staple strand will have to circumvent or bend around the scaffold to ensure that the crossover occurs. Additionally, there is an “angular strain” on the staple strand and a “steric clash” between the staple and the scaffold strands.  This is shown in the figure below in which is a kinetic trap shown from the cross-section of the crossover’s point of view. Overall, the “tight bending” and “angular strain” cause issues when binding.

## Sandwich Strand Dectection
