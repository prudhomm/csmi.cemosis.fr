---
layout: project_item
name: Cartographie
title: 
date: 2015-08-17
author: 
fullname: 
categories: interdisciplinary-bio-project
tags: cemosis-project
abstract: Ce projet a pour but d'étudier les méthodes de déformation de carte géographique afin d'étudier la répartition d'un phénomène sur une surface.
img: /img/project/bio-medical/F3.large.jpg
---

Ce projet a pour but d'étudier les méthodes de déformation de carte géographique afin d'étudier la répartition d'un phénomène sur une surface.

<h5>Problématique:</h5>

Traditionnellement, les cartes géographiques sont découpés suivant des critères administratifs.
Lors de l'étude de l'occurrence d'un fait - le nombre d'accident de la route par exemple - on pourra représenter par un code couleur sur la carte le nombre d'accident par zone administratives. On comprend intuitivement que les informations donnés pour le département de Paris n'auront pas du tout la même signification que celles données pour la Creuse. Ainsi, le premier traitement consiste à normaliser la densité d'accident par la densité de population afin de produire une carte: "accident pour 100 habitants" par exemple.

Mais faire ainsi cache une partie de la réalité qui pourrait être rendue présente au lecteur par un découpage plus pertinent de la carte: c'est la question qui est posée dans ce projet.
L'idée de base est la suivante: chaque zone administrative dispose d'une densité à étudier. En appliquant une équation de diffusion, il est possible de générer un champ de vitesse déformant avec lui la carte, jusqu'à équilibre. l'application ainsi décrite forme une bijection. Chaque zone de la carte déformée à alors la même densité que les autres. Un découpage régulier de la carte déformée et l'utilisation de l'inverse de la bijection permet de fournir un découpage plus cohérent de la carte initiale, permettant au lecteur de disposer d'une carte découpée suivant le phénomène étudiée. Intuitivement, on imagine que Paris sera découpée en surfaces bien plus petite que la Creuse pour notre exemple.

<h5>Objectifs:</h5>

La première étape du projet consiste à reproduire l'état de l'art [1] afin de disposer d'un outil permettant de déformer une carte en fonction.

<center>
<img src="/img/project/bio-medical/F3.large.jpg" height="300" width="400">
</center>

<h5>Première étape :</h5>

La première étape du projet est maintenant achevée.
Grâce aux librairies shaplib et mapnik, nous disposons d'un cartogramme parallèle permettant de générer des cartes détaillées suffisamment rapidement.

<center>
<p><b>Avancée du projet MAP</b></p>

<iframe width="420" height="315" src="https://www.youtube.com/embed/UTRK0NudTs4" frameborder="0" allowfullscreen></iframe>

<br/>
<p><img src="/img/project/bio-medical/c_sh68.png" height="400" width="240">
<img src="/img/project/bio-medical/c_sh68_deformed_2005.png" height="400" width="240"></p>
<p>Haut-Rhin et déformation du Haut-Rhin en fonction d'une densité initiale.</p>
</center>

La deuxième étape sera d'appliquer la bijection inverse au découpage sur la carte déformée.
Une fois ces outils à disposition, nous serons en mesure de découper une carte géographique en fonction des données d'entrée, les suites à donner à ce projet seront alors légion.

[1] Diffusion-based method for producing density-equalizing maps
PNAS 2004 101 (20) 7499-7504; published ahead of print May 10, 2004,doi:10.1073/pnas.0400280101

<i class="fa fa-picture-o"></i> [c_sh68.png](/img/project/bio-medical/c_sh68.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_1988.png](/img/project/bio-medical/c_sh68_deformed_1988.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_1991.png](/img/project/bio-medical/c_sh68_deformed_1991.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_1992.png](/img/project/bio-medical/c_sh68_deformed_1992.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_1993.png](/img/project/bio-medical/c_sh68_deformed_1993.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_1994.png](/img/project/bio-medical/c_sh68_deformed_1994.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_1995.png](/img/project/bio-medical/c_sh68_deformed_1995.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_1996.png](/img/project/bio-medical/c_sh68_deformed_1996.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_1997.png](/img/project/bio-medical/c_sh68_deformed_1997.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_1998.png](/img/project/bio-medical/c_sh68_deformed_1998.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_1999.png](/img/project/bio-medical/c_sh68_deformed_1999.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_2001.png](/img/project/bio-medical/c_sh68_deformed_2001.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_2002.png](/img/project/bio-medical/c_sh68_deformed_2002.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_2003.png](/img/project/bio-medical/c_sh68_deformed_2003.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_2004.png](/img/project/bio-medical/c_sh68_deformed_2004.png)

<i class="fa fa-picture-o"></i> [c_sh68_deformed_2005.png](/img/project/bio-medical
/c_sh68_deformed_2005.png)