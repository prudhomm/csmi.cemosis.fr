# How to write post for CSMI, Feelpp and Cemosis website

## Use `tags: website-name` in the Front Matter

This repository contains all the news of three websites above.
To write a post for a specific website, be sure to use right `tag` in the `Front Matter` of every markdown file.

Two examples for two websites:

A news for CSMI website:

```yaml
---
layout: news_item
title: tile
date: 2015-07-17
author: Admin
categories: website
tags: csmi
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
tags: feelpp
---
```

## News for several websites

If you want to display a news in several websites, just add one or two more website names in the `tags:`.

```yaml
---
layout: news_item
title:  Hp-Feel++ selected by Prace 10th call
date: 2015-03-10
author: prudhomm
fullname: Christophe Prud'homme
categories: [project]
project: [HP-Feel++]
tags: feelpp, cemosis, csmi
---
```

## Be sure the `categories:` that you write exists and is correct.


# Webhook for 3 websites

To setup webhook for feelpp.org csmi.unistra.fr and www.cemosis.fr, add a webhook that send to http://hostname:8080/hooks/news/master. Then destination machine will execute script to pull changes from news repository and push commits into their own repositories.

## setup git push.default

git config --global push.default simple

## setup git authentification to avoid account/passwd

Generate ssh key and copy it to github settings.

