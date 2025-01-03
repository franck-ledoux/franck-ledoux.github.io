---
layout: page
title: Claire Roche
description: Generation of hexahedral meshes for atmospheric reentry, 2021-2024
img:
importance: 2
related_publications: false
category: Alumni
---

**Advisors:** F. Ledoux, J. Breil, and T. Hocquellet (CEA, DAM, CESTA)

**Team:** LIHPC, Université Paris-Saclay

_PhD thesis defended in October, 1, 2024_

### Subject

Numerical simulation codes in fluid mechanics fall into two main classes. The two classes correspond to the type of mesh
used for simulations, structured meshes and unstructured meshes. These two types of mesh each have advantages and
disadvantages.

Structured hexahedral meshes are equivalent to regular grids. In this case, numerous calculation optimizations are
possible, for example it is possible to know in advance the bandwidth of the sparse matrices. Likewise, the simplified
topology of the structured meshes allows almost zero information storage. Finally, it is easier to control the mesh
thicknesses, in the vicinity of the walls of the domain for example.

For complex geometries, it is often not possible to use
globally structured meshes, but it is sometimes possible to reduce oneself to structured meshes by blocks, for which
these optimizations can be applied by block. This remark does not apply to all hexahedral meshes, but the sub-category
of structured meshes (by blocks) is very interesting for high performance applications.

Another advantage often put forward of hexahedral meshes is that they can be aligned with the edge of 3D models, which
often also corresponds to the peculiarities of solution fields. For example in a simulation of fluid mechanics, the
fluid will flow along the edges of the domain. It is then possible to build layers of very anisotropic hexahedral
elements along the edges. This makes it possible to efficiently capture the large variations of the fields in the
boundary layers of problems with fluid-structure interaction.

It is also interesting to note that hexahedral meshes need less elements than tetrahedral meshes to cover the same
volume.
For example, it takes at least five tetrahedra to mesh a unit cube. Likewise, there are fewer edges and interior faces
in hexahedral meshes.

The generation of hexahedral meshes remains a difficult problem with significant industrial challenges. Therefore, it
has been the subject of much research over the past two decades. The use of fields of directions which make it possible
to guide the mesh inside the field, so that it is aligned with the edges makes it possible to treat complex geometrical
configurations. The techniques by direction fields are notably covered by the state of the art of the thesis of N.
Kowalski [Kow13]. One of the objectives of this thesis will be to be able to generate meshes automatically for
aerodynamic applications.
