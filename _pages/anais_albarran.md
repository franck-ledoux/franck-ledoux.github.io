#### Anaïs ALBARRAN (PhD started on October 2, 2025)

__Boundary layer meshing for hypersonic flows simulation__

_Supervision: F. Ledoux, J. Breil, and F. NAULEAU (CEA CESTA)_

At CEA DAM, an important area of research concerns the atmospheric reentry of hypersonic vehicles. While simulating this type of flow requires the development of accurate and robust numerical models, an essential preliminary step is mesh generation. Here, we are interested in generating block-structured hexahedral meshes as automatically as possible. To this end, we aim to provide innovative solutions for generating the boundary layer mesh, which is the area where the most intense physical phenomena occur. It is important to note that this research is part of a more comprehensive and ambitious program to accelerate numerical simulation. This requires enabling a physicist-designer to conduct as many comparative studies as possible in the shortest possible time. In our context, this means that mesh generation must consume as little engineering time as possible.
To generate and then adapt block-structured meshes along the wall of a hypersonic vehicle during computation, we propose to provide innovative solutions for the three main steps of the following pipeline:
1. First, the generation of a curved quadrangular mesh of the hypersonic vehicle wall. Starting from any CAD geometry, this curved mesh must best adapt to the surface of the geometry, potentially crossing poorly connected surface patches.
2. The second step will consist of extruding the generated quadrangular meshes along the wall to obtain hexahedral blocks of the boundary layer. The curved blocks
3. Finally, the final mesh will be obtained by generating a grid of meshes for each hexahedral block and adopting geometric relaxation techniques to obtain meshes of adequate sizes and orientations relative to the needs of the numerical model. Curved quadrilateral and hexahedral blocks will be represented using NURBS elements and manipulated within the framework of bloom theory. Mesh adaptation during computation will be studied through the manipulation of the control polyhedron of NURBS elements.
   
%- Link to the PhD. description on the *theses.fr* website:  [https://theses.fr/s404849](https://theses.fr/s404849)
