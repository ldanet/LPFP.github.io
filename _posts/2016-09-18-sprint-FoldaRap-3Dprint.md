---
layout: post
title:  "Sprint LPFP - imprimantes 3D"
date:   2016-09-18 19:42:42
img: sprint20160918.png
comments: true
poster: remi
---

# LPFP sprint imprimantes 3D FoldaRap
La FoldaRap avait la buse de bouché accompagner d'un problème de surchauffe du moteur de l'axe X.

## Prise en main

* Démontage de la buse
* Débouchage avec une aiguille chauffé à blanc.
* Resserrage de la poulie qui actionne l'envoi du fil PLA devenu glissante.
* Changenement de la pièce 3D haute du charriot qui déroule le fil PLA.
* modifiaction de la vitesse du moteur de l'axe X.
* modifiaction de la vitesse du moteur de l'extrudeur.

![potentiometres](http://reprap.org/mediawiki/images/thumb/e/e9/Potentiometers_FoldaRap2-5_2.jpg/400px-Potentiometers_FoldaRap2-5_2.jpg)

---

La buse à bien été débouché, de gros résidus ont été enlevés au niveau de la tête d'impression et sur les parois.
Nous avons ajustés la vitesse du moteur de l'axe X, d'1/4 de tour pour diminuer le problème thermique.

Le PLA a beaucoup de mal à descendre au niveau de la bloc chauffant ou de la buse voir même au niveau du radiateur. Il se peut qu'il y ait un problème de tension dans la courbure de la gaine ou "tube PTFE".

>En faisant un repère sur le PLA on a constaté qu'il manquait ~ 1cm pour aller au fond de la buse.

En poussant fort le PLA (sans le tube PTFE) au fond de la buse, on a réussi a obtenir une fusion du PLA et à avoir un extrusion à 195°C stable et de couleur non dégradé.

![rac](http://reprap.org/mediawiki/images/thumb/0/0b/Mondrian3-0_196.JPG/400px-Mondrian3-0_196.JPG)
Il faudrait peut-être modifier la hauteur du raccord pneumatique et faire passer le tube PTFE dans le radiateur. Comme sur la photo du wiki-reprap ci-dessus.

Il se peut que le problème soit aussi dût au mauvais réglages du moteur du charriot.

La friction au niveau de la poulie d'envoi du PLA est aussi incertaine.
Le fil PLA fond moins vite qu'il n'avance.
Ce qui donne un effet de fil PLA qui s'accumule entre la buse et le chariot lorsqu'on on teste l'extrudeur.
