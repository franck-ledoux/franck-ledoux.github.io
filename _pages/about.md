---
layout: about
title: about
permalink: /
subtitle: <a href='#'>Affiliations</a>. LIHPC, CEA, Université Paris-Saclay.

profile:
  align: right
  image: franck_ledoux.jpg
  image_circular: true # crops the image to make it circular
  more_info: >
    <p> LiHPC, Teratec</p> 
    <p> 2 Rue de la Piquetterie</p>
    <p> 91680 Bruyères-le-Châtel</p>

news: false # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page
---

I am member of the [LIHPC](https://www-lihpc.cea.fr/en/index.html) research lab and director of research at CEA, France. I work on designing and providing meshing algorithms and software for the purpose of numerical simulations. My main research interests are about: quadrilateral and hexahedral mesh generation, mesh adaptation and mesh partitioning.

In our team, we produce quadrilateral and hexahedral mesh generation for the purpose of hydrodynamics and areodynamics codes. In this context, preferred meshes are said **block-structured**. It is my main research topic. Today, I consider that _frame-field based global parameterizations_, including _Polycube_, are the option to follow. As a complement, with researchers of [IBISC](https://www.ibisc.univ-evry.fr/en/), we investigate how to update block structures using reinforcement learning techniques.

Generating meshes for numerical simulation codes raises the question of getting the "_right_" mesh. Trying to answer leads to investigate how to **generate/adapt a mesh considering data provided by the simulation code itself**. It means to adapt the mesh to numerical fields and not only to a geometrical shape.

The last component of my research is **mesh partitioning**. It is a key feature for running HPC simulation codes efficiently. Our specificity is that we partition meshes and not graphs and we deal both with architecture constraints (MPI process, CPU threads, GPU threads) and code requirements (multi-stages physics, load balancing on the fly).