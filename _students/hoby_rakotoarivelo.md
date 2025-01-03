---
layout: page
title: Hoby Rakotoarivelo
description: Irregular kernels co-design on manycore architectures, application to multi-scale anisotropic mesh adaptation in computational fluid dynamics, 2014-2018
img: 
importance: 8
related_publications: false
category: Alumni
---

**Advisors:** Franck Pommereau (IBISC) and Franck Ledoux

**Team:**  IBISC - Informatique, BioInformatique, Systèmes Complexes, Université d'Evry, Paris-Saclay

*Phd thesis defended in July 6, 2018*

### Subject

Numerical simulations of complex flows such as turbulence or shockwave propagation often require a huge computational
time to achieve an industrial accuracy level. To speedup these simulations, two alternatives may be combined : mesh
adaptation to reduce the number of required points on one hand, and parallel processing to absorb the computation
workload on the other hand. However efficiently porting adaptive kernels on massively parallel architectures is far from
being trivial. Indeed each task related to a local vicintiy need to be propagated, and it may induce new conflictual
tasks though. Furthermore, these tasks are characterized by a low arithmetic intensity and a low reuse rate of already
cached data. Besides, new kind of accelerators have arised in high performance computing landscape, involving a number
of algorithmic constraints. In a context of electrical power consumption reduction, they are characterized by numerous
underclocked cores and a deep hierarchy memory involving asymmetric expensive memory accesses. Therefore, kernels must
expose a high degree of concurrency and high cached-data reuse rate to maintain an optimal core efficiency. The real
issue is how to structure these data-driven and data-intensive kernels to match these constraints ?In this work, we
provide an approach which conciliates both locality constraints and convergence in terms of mesh error and quality. More
than a parallelization, it relies on redesign of kernels guided by hardware constraints while preserving accuracy. In
fact, we devise a set of locality-aware kernels for anisotropic adaptation of triangulated differential manifold, as
well as a lock-free and massively multithread parallelization of irregular kernels. Although being complementary, those
axes come from distinct research themes mixing informatics and applied mathematics. Here, we aim to show that our
devised schemes are as efficient as the state-of-the-art for both axes.