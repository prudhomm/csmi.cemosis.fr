---
layout: project_item
name: Écoulements Sanguins
title: "De l'IRM réelle à l'IRM virtuelle : modéliser les flux sanguins dans le cerveau humain"
date: 2015-08-17
author:
fullname:
categories: [interdisciplinary-bio-project]
tags: [cemosis-project]
abstract: Le but du projet ANR [Vivabrain](http://www.vivabrain.fr/) consiste à développer un protocole complet pour la création d’angiographies virtuelles des réseaux vasculaires cérébraux. Il s’agit d’un travail à l’interface entre informatique (traitement, analyse, synthèse d’image, génération de maillages) et mathématiques appliquées (mécanique des fluides, interaction fluides/structures).
img: /img/project/bio-medical/MesoChallengeStreamlinesV30.png
collaborator: Cemosis, LJK, LIPHY
---

<p style="color:red">Résumé</p>
Le but du projet ANR [Vivabrain](http://www.vivabrain.fr/) consiste à développer un protocole complet pour la création d’angiographies virtuelles des réseaux vasculaires cérébraux. Il s’agit d’un travail à l’interface entre informatique (traitement, analyse, synthèse d’image, génération de maillages) et mathématiques appliquées (mécanique des fluides, interaction fluides/structures).

Un tel protocole requiert l’acquisition d’angiographies (IRM ou scanner X), leur segmentation, l’extraction de modèles anatomiques fiables, la simulation de flux artériels et veineux dans ces modèles, et enfin la simulation de l’acquisition radiographique de tels flux par des mécanismes d’IRM ou de scanner X. L’intérêt de telles angiographies virtuelles (encore inexistantes à ce jour) serait dans un premier temps de calibrer les modèles numériques utilisés et ensuite de valider les résultats ainsi obtenus. Après, elles pourraient fournir à la communauté informatique médicale, des vérités-terrain réalistes (et complexes) pour le développement et la validation de techniques d’analyse d’images vasculaires.

<table style="border: 1px solid black;">
 <tr>
  <td style="border: 1px solid black;"><img src="/img/project/bio-medical/MesoChallengeStreamlinesV30.png">Lignes de courant coloriées avec la magnitude de la vitesse mm/s à t=0.5 s.<br/>Paramètres : viscosité dynamique 3.4815e-6 kg/(mm.s^2) , densité 1.055e-6 kg/mm^3, vitesse constante en entrée de 30 mm/s, modèle Navier-Stokes incompressible. Résultats en sortie des deux veines jugulaires : débit 5784 mm^3/s, vitesse moyenne 155 mm/s.</td>
  <td style="border: 1px solid black;"><img src="/img/project/bio-medical/MesoChallengeStreamlines2.png" height="246" width="320">Lignes de courant coloriées avec la magnitude de la vitesse mm/s à t=0.5 s.<br/>Paramètres : viscosité dynamique 3.4815e-6 kg/(mm.s^2) , densité 1.055e-6 kg/mm^3, vitesse constante en entrée de 50 mm/s, modèle de Navier-Stokes incompressible. Résultats en sortie des deux veines jugulaires : débit 9641 mm^3/s, vitesse moyenne 257 mm/s.</td>
  <td style="border: 1px solid black;"><img src="/img/project/bio-medical/MesoChallengePressure3.png" height="246" width="320">Champ de pression kg/(mm.s^2) à t=0.5 s.<br/>Paramètres : viscosité dynamique 3.4815e-6 kg/(mm.s^2), densité 1.055e-6 kg/mm^3, vitesse constante en entrée de 50 mm/s, modèle de Navier-Stokes incompressible. Résultats en sortie des deux veines jugulaires : débit 9641 mm^3/s, vitesse moyenne 257 mm/s.</td>
 </tr>
</table>
<br/>
<p style="color:red">Équipe</p>

- Vincent Chabannes (UJF, vincent.chabannes@imag.fr)
- Mourad Ismail (UJF, mourad.ismail@ujf-grenoble.fr)
- Christophe Prud'homme (christophe.prudhomme@cemosis.fr, prudhomme@unistra.fr)
- Ranine Tarabay (UNISTRA, CeMoSiS)
- Marcela Szopos (szopos@math.unistra.fr)

<p style="color:red">Contacts</p>

- Marcela Szopos (szopos@math.unistra.fr)
- Christophe Prud'homme (christophe.prudhomme@cemosis.fr, prudhomme@unistra.fr)
