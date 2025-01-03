---
layout: page
title: Hubert Hirtz
description: Mesh partitioning for multi-physics code load balancing , 2020-2023
img:
importance: 4
related_publications: false
category: Alumni
---

**Advisors:** Franck Ledoux, Cédric Chevalier and Sébastien Morais (CEA, LIHPC)

**Team:** LIHPC, Université Paris-Saclay

_Phd thesis defended in December, 10, 2023_

### Subject (in French)

Les logiciels de simulation numérique sont le plus souvent exécutés sur des machines parallèles. Une répartition
équilibrée des calculs est alors primordiale. Pour ce faire, on utilise généralement une approche statique qui consiste
à prédécouper le support de calcul. Dans notre cas, il s’agit de calculer un partitionnement de maillages, un maillage
étant une décomposition géométrique du support de calcul en éléments simples, les mailles. En dimension 3, les mailles
sont le plus souvent des tétraèdres et des hexaèdres et le maillage en comportera plusieurs dizaines ou centaines de
millions.
Ce problème de partitionnement de maillages peut être traité par différentes méthodes, qu’elles soient topologiques (
partitionnement de graphes) ou géométriques. La plupart des outils de partitionnement se focalisent sur le
partitionnement de graphes [Karypis G., 2013 ; Pellegrini F., 2008 ; Zoltan], oubliant certaines caractéristiques de
notre problème :
Le coût des mailles fantômes n’est pas pris en compte. En effet, lorsqu’on distribue le maillage sur différents
processeurs, au bord de chaque domaine des mailles virtuelles, représentant les mailles des processeurs distants, sont
créées. Ne pas les prendre en compte peut s’avérer problématique, particulièrement en 3D.
Ces outils se focalisent sur la minimisation d’une quantité appelée « coupe ». Cette quantité représente les
communications induites par la partition des mailles, mais ce modèle est hélas incorrect [Hendrickson B., 1999].
Dans nombre de nos simulations, la difficulté du problème de partitionnement vient d’abord de la distribution des coûts
de calculs. De plus, ces coûts sont souvent pluriels car correspondant à plusieurs phases de calcul différentes.
Deux thèses récentes au CEA/DAM ont permis des avancées significatives sur ces trois points. La
première [Morais S., 2016] propose une solution pour les deux premiers points, en utilisant un modèle de graphe biparti.
La seconde [Barat R., 2017] apporte des réponses au partitionnement de graphes multi-critères.

L’objectif de cette thèse est d’une part de proposer une réponse concrète au problème d’équilibrage de charges pour des
instances pratiques de simulation multi-physiques (sur des maillages de dizaines ou centaines de millions de mailles).
Pour cela, les techniques utilisées dans les thèses précédentes devront être étendues et adaptées.
D’autre part, l’implantation pratique des algorithmes sera effectuée dans le cadre du projet COUPE (COncUrrent
PartitionEr), écrit en Rust dans un contexte multi-threads. De bonnes connaissances en théorie des graphes mais aussi en
techniques d’optimisation discrète seront nécessaires pour mener à bien cette thèse.
