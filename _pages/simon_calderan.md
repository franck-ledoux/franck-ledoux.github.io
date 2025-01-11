#### Simon CALDERAN (PhD from 10/2018 to 05/2022)

__Interactive generation of block-structured hexahedral meshes__

_Supervision: G. Hutzler (COSMO, IBISC, Université Evry, Paris-Saclay) and F. Ledoux_

_PhD defended on May 17, 2022_

The numerical simulation codes based on element and finite volume methods require discretizing the 
studied domain - for example a mechanical part such as a motor, an airplane wing, a turbine, 
etc. - using a mesh. In 3 dimensions, a mesh is a set composed of simple volumic elements, most 
often tetrahedrons or hexahedra, which partition the field of study. The choice of tetrahedrons or 
hexahedra is mainly dictated by the application (fluid-structure interaction, hydrodynamics, etc.). 
If the automatic generation of tetrahedral meshes is a relatively controlled process today, 
generating hexahedral meshes is still an open problem. This is problematic for applications that 
just imperatively require hexahedral meshes since their generation is done semi-automatically, 
which can take several weeks to several months of engineer time! While the time devoted to the 
digital simulation process itself tends to decrease due to the power of the machines used, the 
bottleneck is now in the preparation of the data, namely to obtain a CAD model adapted to the 
computation, then generate a mesh.It is in this context that we propose to develop a hybrid approach 
combining:1. The development of (semi) -automatic algorithms for generating and modifying 
block-structured hexahedral meshes;2. The implementation of an interactive graphic software 
dedicated to the manipulation of block structures. The interaction mechanisms will also be used to 
guide the algorithms in their decision-making, whether at initialization (criteria to be affixed to 
particular CAD entities) or in the course of an algorithm (decision between several options on 
which the algorithm cannot pronounce itself).The objective of this thesis is therefore not to 
provide a universal automatic solution, which seems unattainable at present, but rather to reduce 
the engineering time devoted to the generation of the mesh by providing more adapted tools. In this 
context, we propose to place the study as an extension of [LED10, KOW12, GAO15, GAO17], which 
considered the problem of simplification and enrichment of hexahedral meshes by insertion and 
removal of mesh layers. In all these works, the proposed algorithms are simple 'greedy' algorithms 
where the mesh is modified step by step to converge towards a final solution Ef: At each step Ei, 
one makes the hypothesis that the 'best' solution Ef will be obtained by making the 'optimal' 
choice for Ei. However, in operational research, such an approach is known to be perfectible since 
the problem of optimization treated is nonlinear. The idea is to use usual approaches in operational 
research and more specifically multi-agent systems, coupled to interactive tools, to allow the 
generation of block structures on complex CA0s

- Link to the PhD. description on the *theses.fr* website:  [https://theses.fr/2022UPASG049](https://theses.fr/2022UPASG049)

- Link to the PhD. manuscript (in French): [<i class="fa-solid fa-file-pdf"></i>](https://www.biblio.univ-evry.fr/theses/2022/2022UPASG049.pdf)