# Enhancing Nanohinge Functionality: Self-Assembly of a Repeatable DNA Hinge System Supporting Higher Order Structure Formation

### Primary Contributors/Contact for Inquiries
| Name | Description/Contribution | Contact |
| ---- | ------------------------ | ------- | 
|UBC BIOMOD| Team email - for general project related inquiries | ubcbiomod@gmail.com | 
| Fumiya Inaba | Primary contributor to [caDNAno Design Validation Tool](https://github.com/ubcbiomod/caDNAno-Design-Validation-Tool-Nanoval), design team co-lead of this project | fumiy@student.ubc.ca | 
| Charlie Sushams | Provided guidance on MATLAB usage/integration into pipeline, code reviewer, design team co-lead of this project | charliesushams@gmail.com |
| Ethan Rajkumar | Primary contributor to Kinetic_trap_detection and Sandwich_strand_detection Jupyter notebooks and secondary contributor to [caDNAno Design Validation Tool](https://github.com/ubcbiomod/caDNAno-Design-Validation-Tool-Nanoval) | ethanrajkumar2001@gmail.com | 

## Description
This repository contains code which was used in the project <i>Enhancing Nanohinge Functionality: Self-Assembly of a Repeatable DNA Hinge System Supporting Higher Order Structure Formation</i>. A cleaner packaged version of this code is available in the [nanoval repo](https://github.com/ubcbiomod/caDNAno-Design-Validation-Tool-Nanoval) as a command-line interface application.   

## Kinetic Trap Detection 
### Overview:
To optimize the folding of H1 and H2 hinges, python scripts were made to assess the presence of kinetic traps in cadnano outputs. 
### Background:

Kinetic traps arise from the presence of excessive mechanical strain - energy contained within twisted or bent structures which have been deliberately engineered to occur at specific locations along a helix. This is especially relevant to DNA origami structures, where we aim to achieve the structure with the least possible Gibbs Free Energy.
However, the process isn't straightforward. As the structure tries to reduce its internal energy while increasing its entropy, it can get caught in minor energy pockets, known as kinetic traps. These traps can create problems due to the bending and maneuvering required by the staple strand to facilitate a crossover with the scaffold strand.
Furthermore, this interaction imposes "angular strain" on the staple strand and leads to a "steric clash" or physical interference between the staple and scaffold strands. This scenario is depicted from the perspective of a cross-section at the crossover point, highlighting the kinetic trap. Ultimately, this "tight bending" and "angular strain" pose challenges during the binding process.

## Sandwich Strand Dectection
### Overview:
To ensure proper annealing of staple strands to the H2 and H1 strands, python scripts were created that interpreted cadnano inputs and identified coordinates in the helices. 

### Background:
Sandwich strands are the result of the comparative length of staple strands that are either bound to multiple domains on the scaffold or interconnected through crossovers linking numerous helices. These strands are typically categorized as either type 1 or type 2 sandwich strands, as depicted in Figure 1.

![image](https://github.com/ubcbiomod/Higher-Order-Nanohinge-Systems/assets/61441923/2a1f8b68-f495-4204-887b-9d10dfae485d)

Type 1 sandwich strands pose a structural challenge due to the need for the staple DNA and the scaffold DNA to intertwine and form a double helix. If a longer binding domain connects first, it's difficult for the shorter binding domain to subsequently bind due to the necessity for shorter staple strand sequences to wrap around a smaller segment of the scaffold, followed by a larger stretch. In other words, if the two longer binding domains are the first to bind in a thermocycler, it becomes kinetically improbable for the shorter binding domain to bind correctly.

Type 2 sandwich strands are also problematic because they don't permit the sequential binding of the staple to the scaffold. The simultaneous binding of both binding domains is statistically unlikely. These complications surrounding sandwich strands can cause frustration because they often result in the scaffold adopting a shape that deviates from the intended structure.
