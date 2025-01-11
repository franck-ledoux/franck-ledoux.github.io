#### Hubert HIRTZ (PhD from 12/2020 to 12/2023)

__Mesh partitioning for load balancing multiphysics simulations__

_Supervision: F. Ledoux, C. Chevalier (LIHPC, CEA) and S. Morais (LIHPC, CEA)_

_PhD defended on December 12, 2023_

This study aims to improve the performance of large-scale, distributed, mesh-based simulations. 
More specifically, we take an interest in improving the balance between the load on each computation 
unit on which the simulations execute. Load balancing mesh-based simulations generally involve both 
the load of each mesh cell and the data transfers between computation units. State-of-the-art tools 
most commonly solve this problem in one way, which is not always the most optimal for a given 
simulation, because their scope is broader than that of mesh partitioning and load-balancing. Our 
study aims to fill this gap and implement a new partitioning tool dedicated to meshes and 
load-balancing. After an in-depth presentation of the context and issues related to balancing the 
load of distributed, mesh-based simulations, as well as the definition of common 
mesh-partitioning-related problems and associated, state-of-the-art algorithms to solve each of 
these problems, we present a new method to partition meshes, which involves carefully chaining 
algorithms to optimise given mesh partition metrics. We then develop this method in two ways: 

- first, we expand the number partitioning algorithm called VNBest so that it can balance load against target weights. 
- Second, we adapt the geometric algorithm called RCB for cartesian meshes, to improve its performance on such meshes. 

We implement the algorithm chaining method and its extensions in a new partitioning tool and describe 
its design thoroughly. We show our tool can compute partitions with better load-balance than 
state-of-the-art tools Scotch and Metis. However, the edgecut is not as optimised as in 
state-of-the-art. We present the scaling of our parallel implementation of partitioning algorithms.

- Link to the PhD. description on the *theses.fr* website:  [https://theses.fr/2023UPASG096](https://theses.fr/2023UPASG096)

- Link to the PhD. manuscript (in French): [<i class="fa-solid fa-file-pdf"></i>](https://theses.hal.science/tel-04400786v1/document)