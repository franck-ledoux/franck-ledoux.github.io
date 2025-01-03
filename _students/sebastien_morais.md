---
layout: page
title: Sébastien Morais
description: Study and obtention of exact, and approximation, algorithms and heuristics for a mesh partitioning problem under memory constraints
img:  
importance: 9
related_publications: false
category: Alumni
---

**Advisors:** Eric Angel, Franck Ledoux and Damien Regnault

**Team:**  IBISC, Université Paris-Saclay

*Phd thesis defended on November, 23, 2016*

### Subject

In many scientific areas, the size and the complexity of numerical simulations lead to make intensive use of massively
parallel runs on High Performance Computing (HPC) architectures. Such computers consist in a set of processing units (
PU) where memory is distributed. Distribution of simulation data is therefore crucial: it has to minimize the
computation time of the simulation while ensuring that the data allocated to every PU can be locally stored in memory.
For most of the numerical simulations, the physical and numerical data are based on a mesh. The computations are then
performed at the cell level (for example within triangles and quadrilaterals in 2D, or within tetrahedrons and
hexahedrons in 3D). More specifically, computing and memory cost can be associated to each cell. In our context, where
the mathematical methods used are finite elements or finite volumes, the realization of the computations associated with
a cell may require information carried by neighboring cells. The standard implementation relies to locally store useful
data of this neighborhood on the PU, even if cells of this neighborhood are not locally computed. Such non computed but
stored cells are called ghost cells, and can have a significant impact on the memory consumption of a PU. The problem to
solve is thus not only to partition a mesh on several parts by affecting each cell to one and only one part while
minimizing the computational load assigned to each part. It is also necessary to keep into account that the memory load
of both the cells where the computations are performed and their neighbors has to fit into PU memory. This leads to
partition the computations while the mesh is distributed with overlaps. Explicitly taking these data overlaps into
account is the problem that we propose to study.