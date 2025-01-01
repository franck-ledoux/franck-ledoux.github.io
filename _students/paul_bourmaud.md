---
layout: page
title: Paul Bourmaud
description: MCTS for hex blocking
img:  
importance: 4
related_publications: false
category: Phd
---

**Advisors:** Franck Ledoux and Jean-Christophe Janodet (IBISC, Université d'Evry Val d'Esssone, Paris-Saclay)

**Team:**  LIHPC, Université Paris-Saclay 

*Phd thesis started October, 3, 2022*

### Subject

Preparing high-fidelity simulations that requires block-structured hexahedral meshes is extremely time consuming. Highly skilled engineers have to manually decompose CAD models into a set of hex-meshable structured blocks. This manual process, called *blocking* stage,  is a bottleneck for incremental design and sensitivity analysis.  At CEA DAM, the blocking stage is performed using **MGX**, an interactive software dedicated to hexahedral block-structured mesh generation. **MGX** provides several basic features - creating or erasing a single block, cutting a set of blocks along a direction - and more advanced ones - putting an O-Grid structure with escaping faces on a set of selected blocks, performing 2D block rotations around an axis, etc. For realistic studies, the generation of the adequate block structure can require several weeks for an engineer. All the MGX operations for handling geometry, blocks and meshes,  can be launched through its own GUI or using a high-level Python API.

Current approaches to solve the hex blocking problem fail to propose an automatic solution to any 3D shapes. All of them model the hex blocking as a continuous optimization problem or a combinatorial problem, that works on the topological structure,  but fail to combine both aspects into a mixed optimization function. As engineers  are able to create such meshes using interactive tools, we strongly believe that machine learning techniques deserve to be studied. More specifically, we propose to develop Reinforcement Learning framework dedicated to decompose a CAD model into ready-to-use hex-meshable blocks. 


In the context of hexahedral meshing, and more specifically of block-structured hexahedral meshing, we cannot rely on a large dataset of blocking examples to train a supervised or unsupervised machine learning algorithm. We focus so on  reinforcement learning (RL) techniques that requires less data. As an **environment**, we consider the block structure and the CAD Model we want to discretize. The **agent** we want to program corresponds to the engineer that uses MGX operations to create the expected block-structure. At each stage, the **agent** observes the **state** of the **environment** and chooses an **action**, i.e. a MGX blocking operation, to apply. This action will change the block structure, and this process is repeated until getting the expected block structure. The set of blocking operations will be limited to  splitting a series of block along an edge, deleting a block, contracting and expanding column of blocks. A main difficulty of this work is that this small set quickly induces a huge set of potential actions to apply at each stage of the process.  In the context of reinforcement learning, the hex blocking problem is:
- **observable** -- At each stage, the whole CAD model and block structures are known and visible;
- **deterministic** -- Each action, derived from applying a blocking operation on a specific block, will always produces the same result;
- **sequential** -- An action modifies the environment, then another action is applied on the resulting environment and so on ;
- **known** -- the agent knows the objectives (getting a hex blocking structure that discretizes the CAD model) and the rules to follows (set of operations);

Training an algorithm to solve this problem is challenging and means to consider long-term rewards -- *do we have finally generated a valid or an invalid block structure ?*-- and a huge set of actions to apply at each stage. The objective of the Phd is to provide a first reinforcement learning algorithm that generates a MGX program that corresponds to build a hexahedral block structure for a given CAD shape.
 