---
layout: project_item
name: Rhéologie Sanguine
title: 
date: 2015-08-17
author: 
fullname: 
categories: interdisciplinary-bio-project
tags: cemosis-project
abstract: Contrairement aux liquides ordinaires et aux solides élastiques, les fluides complexes présentent plusieurs comportements étranges qui dépendent essentiellement de structures sous-jacentes qui composent ces fluides.
img: /img/project/bio-medical/bloodrheol1-fe20d.png
---

<img src="/img/project/bio-medical/bloodrheol2-3d963.png" style="display:inline;float:left;margin: 0px 5px 0px 0px">
<img src="/img/project/bio-medical/bloodrheol1-fe20d.png" style="display:inline;float: right;margin: 5px 5px 0px 0px;">
Contrairement aux liquides ordinaires et aux solides élastiques, les fluides complexes présentent plusieurs comportements étranges qui dépendent essentiellement de structures sous-jacentes qui composent ces fluides. En effet, de nombreux fluides complexes sont constituées d’entités microscopiques (comme des particules rigides ou déformables, des cellules biologiques, des macromolécules etc ..) qui sont en suspension dans le liquide, et dont les individus et les comportements collectifs ont un impact sur l’ensemble des propriétés rhéologiques du fluide à l’échelle macro. C’est cette rétroaction de l’échelle micro à l’échelle macro qui confère ce comportement complexe à ces fluides et qui continue de poser un formidable défi pour la modélisation théorique. Des exemples typiques de ces fluides complexes sont par exemple des suspensions (particules rigides en suspension dans un fluide newtonien), des émulsions (gouttelettes en suspension dans un fluide newtonien), du sang (globules rouges en suspension dans le plasma), et ainsi de suite. Les fluides complexes sont la règle dans les mondes industriels et biologiques, conférant ainsi à ce sujet un intérêt important dans des domaines variés allant du fondamental au technologique.
Un défi important dans les fluides complexes réside dans la compréhension de (i) l’interaction fluide / structure au niveau des particules et (ii) l’organisation spatio-temporelle des entités (c’est à dire leurs comportements collectifs, la formation de bandes ...) qui composent le fluide complexe.
<div style="clear:both"></div>

<i>Images : Cytosquelette d’une globule rouge et forme biconcave d’une globule rouge</i>

Au cours des dernières années, nous avons développé des méthodes numériques, des modèles et une plate-forme logicielle ([Feel ++](http://www.feelpp.org/)) pour la simulation numérique de la rhéologie du sang dans le système vasculaire : Le but de ce projet est de simuler des suspensions d’un grand nombre de vésicules --- agissant en tant que modèles pour les cellules du sang---. Il a en effet été démontré qu’il y a plusieurs similitudes entre les vésicules et les globules rouges (GR) en particulier du point de vue mécanique. Par exemple, comme les GR, les vésicules sous écoulement de cisaillement présentent des dynamiques différentes : le tank threading et le tumbling. En 5 ans, nous prévoyons être en mesure de simuler des dizaines de vésicules déformables (GR) dans les flux 3D dans les artères avec le déplacement des frontières sur des centaines de processeurs et dans les 10 ans des centaines de vésicules déformables en flux 3D dans les artères avec des frontières mobiles. La portée est d’étudier le flux sanguin pulsé dans les moyennes et petites artères. Dans ce contexte de grands déplacements de la membrane (plus de 10% du rayon) des artères cohabitent avec le confinement du flux sanguin. Notre travail actuellement consiste à construire quatre ingrédients :

- de méthodes d’ordre élévé de discrétisation en l’espace, temps et géométrie appliquée à des écoulements en domaine mobiles, 
- des méthodes leveset et des méthodes de domaine fictif, 
- des méthodes de décomposition de domaine et des stratégies de resolution parallèle 
- l’utilisation efficace des architectures informatiques CHP --- par exemple distribués, le calcul parallèle et le GPU.

Ce travail est réalisé en collaboration avec des physiciens de Grenoble ([LIPHY](http://www-lsp.ujf-grenoble.fr/)) et est financé à l’heure actuelle par le ministère de l’Enseignement Supérieur et de la Recherche, la Région Rhône-Alpes (2009-2012), le [projet ANR HAMM](http://www.google.fr/url?sa=t&rct=j&q=anr%20hamm&source=web&cd=1&ved=0CB8QFjAA&url=http%3A%2F%2Fwww.agence-nationale-recherche.fr%2Ffileadmin%2Fuser_upload%2Fdocuments%2Faap%2F2010%2Ffinance%2Fcosinus-financement-2010.pdf&ei=WwXBTobnFo7DtAbgoaXKAw&usg=AFQjCNFjhu0rneo7Zo0Zvuwcxecmr5zDgA) (2010-2014) et le [projet ANR VIVABRAIN](http://icube-vivabrain.unistra.fr/) (2013-2017)