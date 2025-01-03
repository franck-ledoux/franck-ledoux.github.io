---
layout: page
title: Sébastien Mestrallet
description: Robust polycubes for block-structured hexahedral mesh, 2021-2024
img:
importance: 1
related_publications: false
category: Alumni
---

**Advisors:** F. Ledoux and C. Bourcier (CEA, DES)

**Team:** LIHPC, Université Paris-Saclay

_Phd thesis defended on November, 26, 2024_

### Subject

In order to make computations on discrete models, hexahedral meshes are often needed because: some numerical simulation
codes can only manage hexahedral elements (or these codes are only qualified for such elements); hexahedral elements
allow to get a mesh with less number of elements in shapes with small thickness; hexahedral elements obtained by block
splitting have in general good aspect ratio, allowing a better convergence and a better quality of the simulation
result. The current hexahedral meshing algorithms (using octree-based method or Cartesian grid) do not always generate a
mesh with a good enough quality to be usable as the input of a numerical simulation. Some elements are too distorted
near curved faces and refinement areas. As a result, users often have to make a manual block splitting of the geometry
into hexahedral blocks, which is tedious and very time-consuming (from several days to several months), and is sometimes
impossible. Some new automatic methods based on polycubes or frame fields are being developed in the academic world but
they are not robust enough to guarantee a good-quality mesh on every geometry. Hence, this is an open problem. The aim
of this thesis is to find iterative/evolutionary algorithms that can be applied to robust and good quality hexahedral
mesh generation.
