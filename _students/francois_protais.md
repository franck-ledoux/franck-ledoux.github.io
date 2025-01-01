---
layout: page
title: François Protais
description: Polycube-dominant meshing, 2019-2022
img: 
importance: 6
related_publications: false
category: Alumni
---

**Advisors:** Dmitry Sokolov (Université de Lorraine) and Franck Ledoux

**Team:**  LORIA - Laboratoire Lorrain de Recherche en Informatique et ses Applications

*Phd thesis defended in  October 21, 2022*

### Subject  

The general context is generation of hexahedral meshes, which is a very active field in research for the past 40 years. In this PhD thesis, we are interested in studying a sub-problem, more precisely, polycube generation.
A polycube is an orthogonal Polyhedron, that is to say a polyhedron where all the faces are oriented following one of the axes X, Y and Z. We want a one-to-one function that map our domain to a polycube. The polycube must keep the topological characteristics of the original domain, and the map must be of minimum distortion.
The usual approach [1] is to start from a tetrahedral mesh that we can generate with meshing software such as Tetgen or GMSH. The idea of the algorithm is then, for each face of the boundary, to define if this face will be aligned with X, Y or Z. Then, we progressively deform the meshing, trying to follow the prescribed flagging, and finally, we project it onto a polycube. There exists several issues with this approach. If we start with a given flagging, it is possible that a big part of the model will be collapsed, so it might be necessary to review the flagging.
As it appears to be very complex to be sure that a flagging is valid, we will study how to generate models that are polycube-dominant with a flagging that will not be completely coherent. We can start by detecting problematic parts, and remove them from the model, that produce a polycube on the rest. We will therefore obtain hexahedron everywhere except on the boundary of the removed parts.
We will be able to fill those part with existing algorithm from the team [2], and we obtain a polycube-dominant mesh.
The polycube approach allows to have a solid start without having to deal with singularities inside of the hexahedral mesh, to focus on problems linked to boundaries constraints. The approach allows us to focus on those parts, this will be very beneficial to meshes generated with those method. We will then be able to transpose this knowledge directly to global parametrization, which are more generals.
[1] J. Gregson, A. Sheffer and E. Zhang, All-Hex Mesh Generation via Volumetric PolyCube Deformation, SGP 2011
[2] Nicolas Ray, Dmitry Sokolov, Franck Ledoux, Bruno Lévy, Hexahedral Meshing: Mind the Gap!, SPM 2018