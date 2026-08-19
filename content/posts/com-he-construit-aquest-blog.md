---
title: Com he construït aquest blog (i per què)
date: 2026-08-19
type: post
micro: false
description: Per què un blog estàtic propi, amb mentalitat IndieWeb, i com
  funciona la pila que el fa possible.
tags:
  - indieweb
  - blog
  - sobirania digital
draft: false
---
Aquest és el primer post del blog, així que començaré explicant què és això i per què existeix. Perquè darrere d'unes quantes pàgines en blanc i negre hi ha una decisió: **publicar al meu propi lloc, abans que a cap plataforma.**

![The Matrix](/images/the-matrix-1999.jpeg)

<!--more-->

## La idea: el teu lloc, el teu contingut

La web té un problema: publiquem cada cop més a llocs que no controlem. Xarxes socials, plataformes, serveis que poden canviar les regles, tancar o desaparèixer amb tot el que hi hem escrit. El moviment [IndieWeb](https://indieweb.org/) proposa justament el contrari: **publica al teu domini, al teu ritme, amb les teves eines** — i després, si vols, sindica a les xarxes (el que en diuen [POSSE](https://indieweb.org/POSSE): *publish on your own site, syndicate elsewhere*).

Aquest blog és això: un lloc propi, lleuger, ràpid i meu. El contingut és meu, viu en fitxers que puc llegir, copiar i moure on vulgui. Cap plataforma no me'l pot prendre.

## La pila

* **[Hugo](https://gohugo.io/)**: generador de llocs estàtics. Escrius en Markdown (text pla, que dura per sempre) i genera pàgines HTML que carreguen en mil·lèsimes.
* **Tema [Alpine](https://github.com/microdotblog/theme-alpine)**: Minimalista, llegible, amb microformats IndieWeb de sèrie (h-entry, h-card, dt-published…), que és el llenguatge que les màquines entenen per intercanviar contingut.
* **Escriptura**: un panell d'administració propi (Decap CMS) i Obsidian — al final, tot són fitxers `.md` en un repositori de Git.
* **[Git + GitHub](https://github.com/jsalvia/jordisalvia)**: control de versions i còpia de seguretat. Cada versió de cada post queda registrada.
* **[Cloudflare Pages](https://pages.cloudflare.com/)**: allotjament gratuït i desplegament automàtic. Cada cop que faig un canvi, el blog es regenera sol en un minut.

## El flux

Escric → clico "Publica" → Git guarda → Cloudflare compila i desplega. No hi ha servidors a mantenir, no hi ha bases de dades, no hi ha res a vigilar. El resultat: **un blog que és meu, que no em costa ni un euro i que funcionarà d'aquí a vint anys** (els fitxers Markdown es poden obrir amb qualsevol eina).
