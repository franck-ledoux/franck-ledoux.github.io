#### Isaïe MURON (PhD started on January 22, 2024)

__Efficient mesh algorithms on massively parallel architecture__

*Supervision: F. Ledoux and C. Chevalier (LIHPC, CEA)*

High-fidelity simulation of complex phenomena is today an essential tool in many scientific fields. 
At CEA, we develop our own simulation software and environmental tools (meshing, visualization), 
capable of exploiting powerful computers equipped with hundreds of thousands of processors composed 
of heterogeneous calculation units ( CPU and GPU). To effectively operate such computers, it is 
necessary to specifically adapt the data structures and algorithms. In this thesis, we are 
interested in remeshing algorithms, which belong to the category of irregular problems, for which 
successive memory accesses affect non-contiguous areas, and this in an unpredictable manner. This 
characteristic makes efficient parallelization problematic on current and future processors. It is 
this problem that we wish to provide a solution to. More precisely, the objective of the thesis work 
is to define a data structure and a parallel programming paradigm for 3D remeshing within the gmds 
mesh library. Considering the case of simplicial and mixed meshes, the thesis work will consist of 
extending existing parallelization concepts to exploit any type of many-core architecture 
(including GPUs)

- Link to the PhD. description on the *theses.fr* website:  [https://theses.fr/s390775](https://theses.fr/s390775)
