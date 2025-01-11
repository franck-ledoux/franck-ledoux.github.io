#### Sébastien MESTRALLET (PhD from 10/2021 to 11/2024)

__Robust polycubes for block-structured hexahedral mesh__

_Supervision: F. Ledoux and C. Bourcier (SGLS, Université Paris-Saclay, CEA)_

_PhD defended on November 28, 2024_

In order to make computations on discrete models, hexahedral meshes are often needed because:
- some computation codes can only manage hexahedral elements (or these codes are only qualified for hexahedral elements)
- hexahedral elements allow to get a mesh with less number of elements in shapes with small thickness
- hexahedral elements obtained by block splitting have in general good aspect ratio, allowing a better convergence and a better quality of the result of the simulation.

The current hexahedral meshing algorithms (using octree method or cartesian grid) do not always 
allow to have a mesh with a good enough quality to be usable as the input of a numerical simulation. 
Some cells are too distorted near curved faces and refinement areas. As a result, our colleagues 
often have to make a manual block splitting of the geometry in hexahedral blocks, which is tedious 
and takes a long human time (from several days to several months), and is sometimes impossible. 
Some new automatic methods like polycubes or field frames are being developed in the academic world 
but they are not robust enough to guarantee a good-quality mesh on every geometry. Hence, this is 
an open problem. The aim of this thesis is to find iterative/evolutionary algorithms that can be 
applied to robust and good quality hexahedral mesh generation.

- Link to the PhD. description on the *theses.fr* website:  [https://theses.fr/2024UPASG087](https://theses.fr/2024UPASG087)
