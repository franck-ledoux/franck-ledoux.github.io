---
layout: page
title: Nicolas Kowalski
description: Domain partitioning using frame fields - applications to quadrilateral and hexahedral meshing
img:
importance: 10
related_publications: false
category: Alumni
---

**Advisors:** Pascal Frey and Franck Ledoux

**Team:** Laboratoire Jacques Louis Lions, Université Paris 6

_Phd thesis defended in 2013_

### Subject

In this work, we describe a method to partition domains adapted to the generation of quadrilateral and hexahedral
meshes. Given a domain D, the proposed approach proceeds in two steps: first, a frame field is defined on a background
simplicial mesh of D. Then, singular elements of this field are extracted to create a skeleton that partitions D. The
key element of this approach is the use of frames: at a point P of D, a frame allows to orient the quadrilateral or the
hexahedral. Thus, we propose a complete study of frames and frame fields. We describe the proposed method both in
dimension two and three. The main difference between the two is in the way frame fields are generated. In dimension 2,
we solve a non-linear PDE, while in 2D, a heuristic is applied that uses initially an advancing front algorithm that
takes the stability of the field into account, before using a smoothing algorithm. In both cases, a skeleton is
extracted from the frame field. In dimension two, this skeleton always leads to a partition of D into
quadrilateral-shaped blocks, and singularities are all of degree three and five. In dimension three, the obtained frame
field leads to a partition allowing for hexahedral meshing in numerous cases. Many examples are showcased and compared
to results obtained by existing methods.
