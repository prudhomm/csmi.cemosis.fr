---
layout: project_item
name: HiFiMagnet
title: Modélisation multi physique d'aimants à haut champ
date: 2015-08-17
author: 
fullname: 
categories: [interdisciplinary-physics-project]
tags: [cemosis-project]
abstract: Le Laboratoire National des Champs Magnétiques Intenses (LNCMI) est un Très Grand Equipement du CNRS permettant aux chercheurs de réaliser des expériences sous champ magnétique intense (ie. supérieur au champ pouvant être produit par des aimants supraconducteurs, soit 24 T).
img: /img/project/physics/temperature_M1_I16000_ws.png
---

<center>
<p><img src="/img/project/physics/LJK_logo-small.png"> Collaboration : <a href="http://lncmi.cnrs.fr/">LNCMI</a>, <a href="http://www-ljk.imag.fr/">LJK (UJF)</a>, CeMoSiS <img src="/img/project/physics/LNCMI-logo-small.png">
</p>
</center>

<img src="/img/project/physics/Magnet_3D_Ouvert.png" height="200" width="150" style="float:left;display:inline;margin:5px 0px 0px 10px">
Le Laboratoire National des Champs Magnétiques Intenses (LNCMI) est un Très Grand Equipement du CNRS permettant aux chercheurs de réaliser des expériences sous champ magnétique intense (ie. supérieur au champ pouvant être produit par des aimants supraconducteurs, soit 24 T). Actuellement, les aimants du LNCMI peuvent produire jusqu'a 35 T en champ statique, produit par des aimants résistifs alimentés grâce à une installation électrique de 24 MW. Ces aimants sont mis à la disposition de la communauté scientifique via des appels à projets deux fois par an, et répondent à un large spectre d'applications allant de la physique du solide à la supraconductivité ou encore la magnétoscience.

Dans un contexte de compétition internationale entre les laboratoires champs intenses, le LNCMI doit sans cesse repousser les limites des technologies utilisées pour la conceptions des aimants, en terme de matériaux et de design.
<div style="clear:left"></div>

<p style="color:#666666;"><i>Image : Aimant polyhélice. Les hélices sont des tubes de cuivre découpés en spires par électro-érosion. L'isolation électrique entre les spires est assurée, soit en introduisant de la colle epoxy dans les fentes (hélices dites "longitudinales"), soit grâce à des isolants disposés régulièrement entre les spires (hélices dites "radiales"). Ces aimants sont refroidis par circulation d'eau entre les hélices, et entre les spires pour les hélices radiales.</i></p>

<img src="/img/project/physics/temperature_M1_I16000_ws.png" height="320" width="160" style="float:left;display:inline;margin:5px 20px 0px 0px">
D'un point de vue ingéniérie, la conception de tels aimants nécéssite des modèles multi-physique non-linéaires réprésentatifs des phénomènes physiques mis en jeu (électromagnétisme, thermique, mécanique, hydraulique, …). 
Ces modèles doivent être validés et certifiés pour garantir les spécifications, par exemple l’homogénéité du champ pour les applications RMN. Ils doivent s’adapter facilement à tout type de géométrie et de matériaux. Enfin, les incertitudes sur les propriétés des matériaux, les conditions de fonctionnement de l'aimant ainsi que les tolérances géométriques liées au montage des aimants doivent aussi être évaluées pour fiabiliser le design tout en gardant des temps de calcul raisonnable.

Ces modèles doivent donc répondre à des conditions de généricité, d'efficacité, de prise en compte des incertitudes et de contrôle de l'erreur.

Le projet HiFiMagnet a pour objectif de proposer différents outils pour répondre à ces défis : 

- des techniques d'adaptation de maillage et d'estimation d'erreur a posteriori ont d'ores et déjà été mises en place pour controler les erreurs d’approximation numérique
- des méthodes de réduction d'ordre ont été plus récemment utilisées pour les études paramétriques et les analyses de sensibilité
- une implémentation en parallèle de ces méthodes a été réalisée et des tests de passage à l’échelle sont actuellement en cours (Projet Prace Feel++  HPC)

<div style="clear:left"></div>

J. Nadarasa a soutenu son stage de Master 2 sur ce sujet (Coupled modeling and simulation of electromagnets in stationary and instationary modes (axisymmetric and 3D) ) ce 22/08/2013.

<p style="color:#666666;"><i>Image : Comportement de la température dans un hélice radiale en fonctionnement (modèle electrothermique couplé non linéaire).</i></p>

<h5>Contacts :</h5> 

- C. Prud'homme (christophe.prudhomme@cemosis.fr),
- C.Trophime (christophe.trophime@lncmi.cnrs.fr),
- C. Daversin (cecile.daversin@lncmi.cnrs.fr)