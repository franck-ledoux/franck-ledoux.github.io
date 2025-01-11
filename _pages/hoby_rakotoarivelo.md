#### Hoby RAKOTOARIVELO (PhD from 11/2014 to 07/2018)

__A co-design approach of irregular kernels on manycore architectures : case of multi-scale anisotropic remeshing in 
computational fluid dynamics__

_Supervision: F. Pommereau (COSMO, IBISC, Université Evry, Paris-Saclay) and F. Ledoux_

_PhD defended on July 6, 2018_

Numerical simulations of complex flows such as turbulence or shockwave propagation often require a 
huge computational time to achieve an industrial accuracy level. To speedup these simulations, two 
alternatives may be combined : mesh adaptation to reduce the number of required points on one hand, 
and parallel processing to absorb the computation workload on the other hand. However efficiently 
porting adaptive kernels on massively parallel architectures is far from being trivial. Indeed each 
task related to a local vicintiy need to be propagated, and it may induce new conflictual tasks 
though. Furthermore, these tasks are characterized by a low arithmetic intensity and a low reuse 
rate of already cached data. Besides, new kind of accelerators have arised in high performance 
computing landscape, involving a number of algorithmic constraints. In a context of electrical power 
consumption reduction, they are characterized by numerous underclocked cores and a deep hierarchy 
memory involving asymmetric expensive memory accesses. Therefore, kernels must expose a high degree 
of concurrency and high cached-data reuse rate to maintain an optimal core efficiency. The real issue 
is how to structure these data-driven and data-intensive kernels to match these constraints ?In this 
work, we provide an approach which conciliates both locality constraints and convergence in terms of 
mesh error and quality. More than a parallelization, it relies on redesign of kernels guided by 
hardware constraints while preserving accuracy. In fact, we devise a set of locality-aware kernels 
for anisotropic adaptation of triangulated differential manifold, as well as a lock-free and 
massively multithread parallelization of irregular kernels. Although being complementary, those axes 
come from distinct research themes mixing informatics and applied mathematics. Here, we aim to show 
that our devised schemes are as efficient as the state-of-the-art for both axes.

- Link to the PhD. description on the *theses.fr* website:  [https://theses.fr/2018SACLE012](https://theses.fr/2018SACLE012)

- Link to the PhD. manuscript (in French): [<i class="fa-solid fa-file-pdf"></i>](https://www.biblio.univ-evry.fr/theses/2018/2018SACLE012.pdf)