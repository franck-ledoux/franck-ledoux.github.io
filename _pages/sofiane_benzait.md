#### Sofiane BENZAIT (PhD from 07/2020 to 09/2023)

__Generation and Adaptation for hybrid meshes using oriented metrics__

_Supervision: F. Ledoux and A. Loseille (Gamma3, INRIA Paris-Saclay)_

_PhD defended on September 5, 2023_

Today, fully tetrahedral mesh generation is a solved problem, but hexahedral mesh generation is not. 
The generation of hexahedral meshes is an important area of research in numerical simulation. 
Hexahedral meshes save time in numerical simulations compared with the same tetrahedral meshes. In 
addition to the possible time savings, hexahedral meshes can be used to study numerical solutions in 
certain imposed directions in a simpler way than with tetrahedral meshes. Given the difficulty of 
generating an entirely hexahedral mesh, one choice that can be made is to combine hexahedra and 
tetrahedra to generate mixed meshes. This solution makes it possible to have hexahedra in the areas 
of interest in the numerical simulation and tetrahedra in the rest of the mesh. The work in this 
thesis has led to the creation of a technique for generating mixed meshes using an orientation field 
and an imposed metric field as constraints. We chose a frontal approach for creating the vertices 
that form the mixed elements of the mesh and the cavity operator for modifying the initial 
tetrahedral mesh. Frontal generation is used to generate the curves, then the surfaces and finally 
the volume of the mesh. The generated vertices are then inserted into the initial mesh using the 
cavity operator, then the initial vertices of the mesh are removed using the cavity operator. The 
last step consists of reconstructing the hexahedra that could not be created by frontal generation 
by combining the tetrahedra to generate hexahedra. This last step is controlled by a pre-imposed 
quality factor.

- Link to the PhD. description on the *theses.fr* website:  [https://theses.fr/2023IPPAX070](https://theses.fr/2023IPPAX070)

- Link to the PhD. manuscript (in French): [<i class="fa-solid fa-file-pdf"></i>](https://theses.hal.science/tel-04525333v1/document)