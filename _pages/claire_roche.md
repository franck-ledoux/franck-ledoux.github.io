#### Claire ROCHE (PhD from 10/2021 to 10/2024)

__Hexahedral curved block-structured mesh generation for atmospheric re-entry__

_Supervision: F. Ledoux, J. Breil (CEA, CESTA) and T. Hocquellet (CESTA, CEA)_

_PhD defended on October 1st, 2024_

The French Alternative Energies and Atomic Energy Commission (CEA) studies Computational Fluid 
Dynamics (CFD) in the case of supersonic and hypersonic flows. To do so, a dedicated code is 
developed. To deal with strong constraints, this code only performs on block-structured meshes. 
This specific type of mesh is complicated to generate, and this generation is usually handled by 
hand using dedicated interactive software. In the case of industrial complex geometries, the mesh 
generation is highly time-consuming. Currently, automatic hexahedral mesh generation is a complex 
open research field.In this thesis work, we propose a method to generate block-structured hexahedral 
meshes on curved blocks of the fluid domain around vehicles, dedicated for the problems of interest. 
This method is first proposed in 2D and then extended to 3D. Here, it is presented in the generic nD 
case. This method is composed of several steps. First, a linear block structure is extruded from a 
first vehicle surface discretization. This work is an extension of the previous work of Ruiz-Girones 
et al.. Once this linear block structure is generated, we propose two different methods to curve the 
block structure to improve the vehicle surface representation and limit the smoothing on the final 
mesh. The first method is through an algorithm of mesh adaptation at fixed topology by solving an 
optimization problem to which a penalty term is added to align certain mesh edges to an implicit 
interface. Our global approach uses this method to align the block structure to the vehicle surface. 
This method remains time-consuming in 3D, so we proposed a second method to curve our block structure 
through polynomial Bézier curves. Considering our blocks as Bézier blocks, we apply geometric and 
local operations to align the high-order block structure to the vehicle surface. Then, considering 
we curved the block structure using Bézier elements, we generate a mesh on the curved blocks under 
constraints. Finally, the generated mesh quality is evaluated in two ways. The first one is through 
purely geometrical criteria analysis. The second one is through numerical simulations of flows around 
vehicles on our meshes, comparing the simulation results to experimental data, analytical results, 
and reference simulations.

- Link to the PhD. description on the *theses.fr* website:  [https://theses.fr/2024UPASG053](https://theses.fr/2024UPASG053)

- Link to the PhD. manuscript (in English): [<i class="fa-solid fa-file-pdf"></i>](https://www.biblio.univ-evry.fr/theses/2024/2024UPASG053.pdf)