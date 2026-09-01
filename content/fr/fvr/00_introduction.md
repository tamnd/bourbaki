---
book: fvr
book_title: Functions of a Real Variable
chapter: ""
chapter_title: ""
section: 0
section_title: INTRODUCTION
kind: introduction
lang: fr
source: fvr-i-vii-fr
pdf_pages: 0007-0008
extraction: ocr
statements: 0
exercises: 0
content_sha256: df62367d771cea1ad5ed9a002672052784f6061f8383cf945428d1827c42fb99
---

## INTRODUCTION

L’objet de ce Livre est l’étude élémentaire des propriétés infinitésimales des fonctions d’une variable réelle; l’extension de ces propriétés aux fonctions de plusieurs variables réelles, ou, à plus forte raison, à des fonctions définies dans des espaces plus généraux, ne pourra être traitée que dans des Livres ultérieurs.

Les propriétés que nous démontrerons sont surtout utilisées lorsqu’elles se rapportent à des fonctions numériques (finies) d’une variable réelle; mais la plupart s’étendent sans nouveau raisonnement aux fonctions d’une variable réelle prenant leurs valeurs dans un espace vectoriel de dimension finie sur le corps $\mathbf{R}$, et plus généralement à des fonctions prenant leurs valeurs dans un espace vectoriel topologique sur $\mathbf{R}$ (voir ci-dessous); comme ces fonctions interviennent fréquemment en Analyse, c’est pour elles que nous énoncerons toutes les propriétés qui ne sont pas spéciales aux fonctions numériques.

La notion d’espace vectoriel topologique, dont nous venons de parler, est définie et étudiée en détail au Livre V de ce Traité; mais dans le présent Livre, nous n’aurons besoin d’aucun des résultats du Livre V; seules interviendront quelques définitions que nous allons reproduire ci-dessous pour la commodité du lecteur.

Nous ne reviendrons pas sur la définition d’une espace vectoriel sur un corps commutatif $\mathbf{K}$ (A, II, p. 3).¹ Un espace vectoriel topologique $E$ sur un corps topologique $K$.

¹ Les éléments (ou vecteurs) d’un espace vectoriel $E$ sur un corps commutatif $K$ seront notés d’ordinaire dans ce chapitre par des minuscules grasses, les scalaires par des minuscules latines; le plus souvent, nous noterons à droite le scalaire $t$ dans le produit par $t$ d’un vecteur $x$, produit qui s’écrira donc $xt$; éventuellement, nous nous permettrons toutefois d’utiliser la notation à gauche $tx$ dans certains cas où elle sera plus commode; nous écrirons aussi parfois le produit du scalaire $1/t$ ($t \neq 0$) et du vecteur $x$ sous la forme $x/t$.

est un espace vectoriel sur K muni d’une topologie telle que les fonctions x + y et xt soient continues dans E × E et dans E × K respectivement; une telle topologie est en particulier compatible avec la structure de groupe additif de E. Lorsque le groupe topologique E est complet, on dit que l’espace vectoriel topologique E est complet. Tout espace vectoriel normé sur un corps valué K (TG, IX, p. 31)¹ est un espace vectoriel topologique sur K.

Soit E un espace vectoriel (muni ou non d’une topologie) sur le corps R des nombres réels; si x, y sont deux points quelconques de E, on appelle segment fermé d’extrémités x, y l’ensemble des points xt + y(1 − t) lorsque t parcourt l’intervalle fermé [0, 1] de R. On dit qu’une partie A de E est convexe si, quels que soient les points x, y de A, le segment fermé d’extrémités x et y est contenu dans A. Par exemple, une variété linéaire affine est convexe; il en est de même d’un segment fermé; dans R^n, un parallélétope (TG, VI, p. 3) est convexe. Toute intersection d’ensembles convexes est un ensemble convexe.

On dit qu’un espace vectoriel topologique E sur le corps R est localement convexe si l’origine (et par suite tout point de E) possède un système fondamental de voisinages convexes. Tout espace normé E sur R est localement convexe; en effet, les boules \|x\| \leq r (r > 0) forment un système fondamental de voisinages de 0 dans E, et chacune d’elles est un ensemble convexe, car les relations \|x\| \leq r, \|y\| \leq r entraînent

$$
\|xt + y(1 - t)\| \leq \|x\|t + \|y\|(1 - t) \leq r
$$

pour $0 \leq t \leq 1$. En particulier, les espaces numériques R^n sont localement convexes.

Enfin, une algèbre topologique A sur un corps topologique (commutatif) K est une algèbre sur K munie d’une topologie telle que les fonctions x + y, xy et xt soient continues dans A × A, A × A et A × K respectivement; lorsqu’on munit seulement A de sa topologie et de sa structure d’espace vectoriel sur K, A est donc un espace vectoriel topologique. Toute algèbre normée sur un corps valué K (TG, IX, p. 37) est une algèbre topologique sur K.

¹ On rappelle qu’une norme sur E est une fonction numérique \|x\| définie dans E, à valeurs finies et $\geq 0$, telle que la relation \|x\| = 0 soit équivalente à x = 0 et qu’on ait

$$
\|x + y\| < \|x\| + \|y\| \text{ et } \|xt\| = \|x\|\cdot|t|
$$

pour tout $t \in K$ ($|t|$ étant la valeur absolue de t dans K).
