# How to write post for CSMI, Feelpp and Cemosis website

## Use `tags: website-name` in the Front Matter

This repository contains all the news of three websites above.
To write a post for a specific website, be sure to use right `tags` in the `Front Matter` of every markdown file.

Two examples for two websites:

A news for CSMI website:

```yaml
---
layout: news_item
title: tile
date: 2015-07-17
author: Admin
categories: [website]
tags: [csmi]
---
```

A news for Feelpp website:
```yaml
---
layout: news_item
title:  Hp-Feel++ selected by Prace 10th call
date: 2015-03-10
author: prudhomm
fullname: Christophe Prud'homme
categories: [project]
project: [HP-Feel++]
tags: [feelpp]
---
```

## News for several websites

If you want to display a news in several websites, just add one or two more website names in the `tags:`. Close `tags` and `categories` in square brackets to avoid parsing issue.

```yaml
---
layout: news_item
title:  Hp-Feel++ selected by Prace 10th call
date: 2015-03-10
author: prudhomm
fullname: Christophe Prud'homme
categories: [project]
project: [HP-Feel++]
tags: [feelpp, cemosis, csmi]
---
```

### Be sure the `categories:` that you write exists and is correct.


# Webhook for 3 websites

To setup news webhook for feelpp.org, csmi.unistra.fr and www.cemosis.fr add a webhook that send to http://hostname:8080/hooks/news/master. Then destination machine will execute script to pull changes from news repository and push commits into their own repositories. 

## Write post as project for www.cemosis.fr

```yaml
---
layout: project_item
name: Chorus
title: "Méthodes de Réduction d'Ordre en Aérothermie: Application aux systèmes d'air conditionné de cabine d'avion"
date: 2015-08-17
author: 
fullname: 
categories: [entreprise-project]
tags: [cemosis-project]
abstract: Dans ce projet nous nous intéressons à des méthodes de réduction d'ordre pour des problèmes d'aérothermie.
img: /img/project/cabin.png
collaborator: 
---
```

Actually there are 3 types of project for cemosis website: `[interdisciplinary-bio-project]`, `[entreprise-project]` and `[interdisciplinary-physics-project]`. They are all under the same tags: `[cemosis-project]`.
