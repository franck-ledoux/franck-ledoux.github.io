---
layout: page
title: Nicolas Le Goff
description: Construction of a conformal hexahedral mesh from volume fractions - theory and applications
img:  
importance: 7
related_publications: false
category: Alumni
---

**Advisors:** Jean-Christophe Janodet and Franck Ledoux

**Team:**  IBISC, Université Paris-Saclay 

*Phd thesis defended in  December, 17, 2020*

### Subject
This thesis addresses the problem of the automatic generation of purely hexahedral meshes for simulation codes when having a mesh carrying volume fraction data as an input, meaning that there can be several materials inside one cell. The proposed approach should create an hexahedral mesh where each cell corresponds to a single material, and where interfaces between materials form smooth surfaces. From a theoretical standpoint, we aim at adapting and extending state-of-the-art techniques and we apply them on examples, some classically issued from CAD models (and imprinted onto a mesh to obtain volume fractions), some procedurally generated cases and others in an intercode capacity where we take the results of a first simulation code to be our inputs. We first define a metric that allows the evaluation of our (or others') results and a method to improve those; we then introduce a discrete material interface reconstruction method inspired from the scientific visualization field and finally we present an algorithmic pipeline, called {sc ELG}, that offers a guarantee on the mesh quality by performing geometrical and topological mesh adaptation.