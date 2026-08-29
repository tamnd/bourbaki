---
book: top
book_title: General Topology
chapter: IV
chapter_title: NOMBRES RÉELS
section: 6
section_title: Fonctions numériques continues et fonctions numériques semi-continues
lang: fr
source: top-i-iv-fr
book_pages: TG IV.27-TG IV.31, TG IV.55-TG IV.58
pdf_pages: 0298-0302, 0326-0329
extraction: ocr
subsections:
    - "no": 1
      title: Fonctions numériques continues
      page: 27
      pdf_page: 298
    - "no": 2
      title: Fonctions semi-continues
      page: 28
      pdf_page: 299
statements: 15
exercises: 16
content_sha256: f7a41b4d735f549c22bac960df620992dc601aaa0a74c22e9a97bf836dde103d
---

## § 6. FONCTIONS NUMÉRIQUES CONTINUES ET FONCTIONS NUMÉRIQUES SEMI-CONTINUES

### 1. Fonctions numériques continues

En dehors des propriétés générales des fonctions continues à valeurs dans un espace topologique quelconque (I, p. 8), les fonctions numériques continues possèdent les deux propriétés fondamentales suivantes:

**Théorème 1** (Weierstrass). — *Soit f une fonction numérique définie et continue dans un* espace quasi-compact non vide E. Il existe au moins un point $a \in E$ tel que $f(a) = \sup_{x \in E} f(x)$, et au moins un point $b \in E$ tel que $f(b) = \inf_{x \in E} f(x)$.

En effet, $f(E)$ est compact (I, p. 62, th. 2), donc fermé dans $\overline{\mathbf{R}}$; par suite $f(E)$ contient ses bornes.

On énonce souvent ce théorème en disant qu’une fonction numérique continue dans un espace quasi-compact non vide y atteint ses bornes.

#### Corollaire {#top-iv-s6-n1-cor-1 .statement}

Si une fonction numérique $f$, définie dans un espace quasi-compact non vide E, est continue et finie dans E, elle est bornée dans E.

#### Théorème 2 (Bolzano) {#top-iv-s6-thm-2 .statement}

Soit $f$ une fonction numérique définie et continue dans un espace connexe E. Si $a$ et $b$ sont deux points quelconques de E, et $\alpha$ un nombre réel appartenant à l’intervalle fermé de bornes $f(a)$ et $f(b)$, il existe au moins un point $x \in E$ tel que $f(x) = \alpha$.

En effet, $f(E)$, qui est connexe (I, p. 82, prop. 4), est un intervalle de $\overline{\mathbf{R}}$ (IV, p. 15, prop. 5), et par suite contient l’intervalle fermé de bornes $f(a)$ et $f(b)$.

On exprime souvent cette propriété en disant qu’une fonction numérique continue dans un espace connexe ne peut passer d’une valeur à une autre sans passer par toutes les valeurs intermédiaires.

Cette propriété n’est d’ailleurs nullement caractéristique des fonctions continues; on peut donner des exemples de fonctions définies dans un espace connexe, discontinues en tout point, et qui la possèdent (IV, p. 55, exerc. 2).

### 2. Fonctions semi-continues

Soit $f$ une fonction numérique définie dans un espace topologique E; pour que $f$ soit continue en un point $a \in E$, il faut et il suffit que: 1° quel que soit le nombre réel $h$ tel que $h < f(a)$, il existe un voisinage V de $a$ tel qu’en tout point $x \in V$, on ait $h < f(x)$; 2° quel que soit le nombre réel $k$ tel que $k > f(a)$, il existe un voisinage W de $a$ tel qu’en tout point $x \in W$, on ait $k > f(x)$.

Les fonctions pour lesquelles une seule des deux conditions ci-dessus est remplie jouent un rôle important en Analyse. De façon précise, nous poserons la définition suivante:

#### Définition 1 {#top-iv-s6-def-1 .statement}

Une fonction numérique $f$, définie dans un espace topologique E, est dite semi-continue inférieurement (resp. semi-continue supérieurement) en un point $a \in E$, si quel que soit $h < f(a)$ (resp. $k > f(a)$), il existe un voisinage V de $a$ tel que $h < f(x)$ (resp. $k > f(x)$) pour tout $x \in V$.

Une fonction numérique est dite semi-continue inférieurement (resp. semi-continue supérieurement) dans E, si elle est semi-continue inférieurement (resp. supérieurement) en tout point de E.

Pour qu’une fonction numérique $f$ soit continue en un point $a$, il faut et il suffit donc qu’elle soit à la fois semi-continue supérieurement et semi-continue inférieurement au point $a$.

Si $f$ est semi-continue inférieurement en un point, $-f$ est semi-continue supérieurement en ce point, et réciproquement; aussi nous bornerons-nous, dans ce qui suit, à considérer les propriétés des fonctions semi-continues inférieurement.

Il est clair qu’une fonction semi-continue inférieurement dans $E$, est semi-continue inférieurement dans tout sous-espace de $E$.

#### Exemple 1 {#top-iv-s6-n2-exa-1 .statement}

Si en un point $a$, $f$ admet un minimum relatif, c’est-à-dire s’il existe un voisinage $V$ de $a$ tel que, pour tout $x \in V, f(a) \leq f(x)$, $f$ est semi-continue inférieurement au point $a$. En particulier, si $f(a) = -\infty$, $f$ est semi-continue inférieurement au point $a$.

#### Exemple 2 {#top-iv-s6-n2-exa-2 .statement}

Définissons une fonction numérique $f$ dans $\mathbf{R}$, en posant $f(x) = 0$ si $x$ est irrationnel, $f(x) = 1/q$ si $x$ est rationnel et égal à la fraction irréductible $p/q$ ($q > 0$). Pour tout $n$ entier $> 0$, l’ensemble des nombres rationnels $p/q$ tels que $q < n$ est fermé et ses points sont isolés; pour tout $x$ irrationnel, il existe donc un voisinage $V$ de $x$ tel que $f(y) \leq 1/n$ pour tout $y \in V$, ce qui prouve que $f$ est continue au point $x$; et d’autre part, $f$ admet un maximum relatif en tout point rationnel $x$, donc $f$ est semi-continue supérieurement dans $\mathbf{R}$.

La condition pour que $f$ soit semi-continue inférieurement au point $a$ peut encore s’exprimer en disant que, pour tout $h < f(a), \overline{f}([h, +\infty])$ doit être un voisinage de $a$.

Il suffit d’ailleurs de supposer cette condition vérifiée seulement pour une suite croissante $(h_n)$ de nombres réels $< f(a)$ et tendant vers $f(a)$.

Munissons $\overline{\mathbf{R}}$ de la topologie dont les ensembles ouverts sont $\varnothing$ et les intervalles ouverts illimités à droite de $\overline{\mathbf{R}}$ (c’est-à-dire les intervalles $]a, +\infty]$ pour $a$ fini, et l’intervalle $(-\infty, +\infty) = \overline{\mathbf{R}}$). Pour que la fonction numérique $f$ soit semi-continue inférieurement au point $a$, il faut et il suffit qu’elle soit continue en ce point, lorsqu’on la considère comme une application dans $\overline{\mathbf{R}}$ muni de la topologie précédente.

#### Proposition 1 {#top-iv-s6-prop-1 .statement}

*Pour qu’une fonction numérique $f$ soit semi-continue inférieurement dans un espace topologique $E$, il faut et il suffit que, pour tout nombre fini $k, \overline{f}([k, +\infty])$* (ensemble des $x \in E$ tels que $f(x) > k$) *soit un ensemble ouvert dans $E$* (ou, ce qui revient au même, que $\overline{f}([-\infty, k])$ *soit un ensemble fermé dans $E$*).

En effet, cette condition exprime que $\overline{f}([k, +\infty])$ est un voisinage de chacun de ses points.

Pour que $f$ soit semi-continue inférieurement dans $E$, il suffit que $\overline{f}([k, +\infty])$ soit un ensemble ouvert dans $E$, pour tous les nombres réels $k$ appartenant à un ensemble partout dense dans $\mathbf{R}$.

#### Corollaire {#top-iv-s6-n2-cor-1 .statement}

*Pour qu’une partie $A$ d’un espace topologique $E$ soit un ensemble ouvert (resp. fermé) dans $E$, il faut et il suffit que sa fonction caractéristique*¹ $\varphi_A$ *soit semi-continue inférieurement (resp. supérieurement) dans $E$*.

¹ Rappelons (E, III, p. 38) que la fonction caractéristique $\varphi_A$ d’une partie $A$ d’un ensemble $E$, est la fonction définie dans $E$, telle que $\varphi_A(x) = 1$ pour tout $x \in A$, et $\varphi_A(x) = 0$ pour tout $x \in \mathbf{C}A$.

En effet, $\varphi_A^{-1}(k, +\infty])$ est égal à $\varnothing$ pour $k \geqslant 1$, à $A$ pour $0 \leqslant k < 1$ et à $E$ pour $k < 0$.

#### Théorème 3 {#top-iv-s6-thm-3 .statement}

*Soit f une fonction semi-continue inférieurement dans un espace quasi-compact non vide E ; il existe au moins un point $a \in E$ tel que $f(a) = \inf_{x \in E} f(x)$* (autrement dit, *f atteint sa borne inférieure dans E*).

En effet, pour tout $k \in f(E)$, considérons l’ensemble $A_k = f^{-1}((-\infty, k])$; ces ensembles sont non vides et forment une *base de filtre* sur $E$; comme ils sont *fermés* d’après la prop. 1, ils ont au moins un point commun $a$ (axiome (C'') des espaces quasi-compacts (I, p. 59)). Pour tout $x \in E$, on a donc $f(a) \leqslant f(x)$, d’où le théorème.

#### Corollaire {#top-iv-s6-n2-cor-2 .statement}

*Soit f une fonction semi-continue inférieurement dans un espace quasi-compact non vide E ; si $f(x) > -\infty$ pour tout $x \in E$, f est minorée dans E.*

On remarquera que ce théorème, et le théorème correspondant pour les fonctions semi-continues supérieurement redonnent comme cas particulier le théorème de Weierstrass (IV, p. 27, th. 1).

#### Proposition 2 {#top-iv-s6-prop-2 .statement}

*Soient f et g deux fonctions numériques semi-continues inférieurement en un point $a \in E$. Les fonctions $\inf(f, g)$ et $\sup(f, g)$ sont semi-continues inférieurement au point a. Il en est de même de $f + g$ si cette fonction est définie, et de $fg$ si $f$ et $g$ sont $\geqslant 0$ et si le produit $fg$ est défini.*

Faisons par exemple la démonstration pour $f + g$; les raisonnements sont analogues dans les autres cas. La proposition est évidente si $f(a)$ ou $g(a)$ est égal à $-\infty$; sinon, on a $f(a) + g(a) > -\infty$. Tout nombre fini $h < f(a) + g(a)$ peut s’écrire $h = r + s$, où $r < f(a)$ et $s < g(a)$ sont finis (il suffit de prendre $s$ tel que $h - f(a) < s < g(a)$); par hypothèse, il existe un voisinage $V$ de $a$ tel que, pour tout $x \in V$, on ait $r < f(x)$, et un voisinage $W$ tel que, pour tout $x \in W$, $s < g(x)$; il en résulte que $h = r + s < f(x) + g(x)$ pour tout point $x$ du voisinage $V \cap W$.

On voit de même que, si $f$ est semi-continue inférieurement en un point $a$, et si $f \geqslant 0$, $1/f$ est semi-continue supérieurement au point $a$.

#### Théorème 4 {#top-iv-s6-thm-4 .statement}

*L’enveloppe supérieure d’une famille $(f_i)$ de fonctions semi-continues inférieurement en un point $a \in E$, est semi-continue inférieurement au point a.*

En effet, soit $g$ cette enveloppe supérieure; quel que soit $h < g(a)$, il existe un indice $i$ tel que $h < f_i(a) \leqslant g(a)$, puis un voisinage $V$ de $a$ tel que $h < f_i(x)$ pour tout $x \in V$, d’où *a fortiori* $h < g(x)$ pour tout $x \in V$.

D’après la prop. 2, l’enveloppe *inférieure* d’un nombre *fini* de fonctions semi-continues inférieurement, est encore semi-continue inférieurement; mais il n’en est pas de même en général de l’enveloppe inférieure d’une famille *infinie* de fonctions semi-continues inférieurement. Par exemple, pour tout nombre rationnel $r$, désignons par $f_r$ la fonction égale à 0 au point $r$, à 1 pour tout nombre réel $x \neq r$; l’enveloppe inférieure des $f_r$ est la fonction $g$ égale à 0 pour tout nombre rationnel, à 1 pour tout nombre irrationnel (*fonction de Dirichlet*); elle n’est donc pas semi-continue inférieurement aux points irrationnels.

#### Corollaire {#top-iv-s6-n2-cor-3 .statement}

L’enveloppe supérieure d’une famille de fonctions numériques continues dans un espace E est semi-continue inférieurement dans E.

Dans IX, §1, n° 7, prop. 7, nous montrerons que la réciproque de cette proposition est vraie si E est uniformisable (et dans ce cas seulement); toute fonction semi-continue inférieurement dans un espace uniformisable est l’enveloppe supérieure d’une famille de fonctions continues.

#### Proposition 3 {#top-iv-s6-prop-3 .statement}

Soient E un espace topologique, f une fonction numérique $\geq 0$ définie dans E et semi-continue inférieurement; alors f est limite d’une suite croissante $(f_n)_{n \geq 1}$ de fonctions semi-continues inférieurement dans E, telle que chaque $f_n$ soit combinaison linéaire, à coefficients $\geq 0$; de fonctions caractéristiques d’ensembles ouverts dans E.

Etant donnés deux entiers $k \geq 1$ et $n \geq 1$, notons $v_{kn}$ la fonction caractéristique de l’intervalle $[k/2^n, +\infty)$ de $\overline{\mathbf{R}}$. Pour tout $x \in \overline{\mathbf{R}}_+$, posons $u_n(x) = 2^{-n} \sum_{k=1}^{n.2^n} v_{kn}(x)$; il est immédiat que la suite $(u_n(x))_{n \geq 1}$ est croissante et admet x pour limite dans $\overline{\mathbf{R}}$. La suite des fonctions $f_n = u_n \circ f$ est donc croissante et converge vers f, et l’on a $f_n = 2^{-n} \sum_{k=1}^{n.2^n} \varphi_{U(k,n)}$, où U(k, n) est l’ensemble ouvert $-1$($k/2^n, +\infty$) de E (IV, p. 29, prop. 1).

#### Proposition 4 {#top-iv-s6-prop-4 .statement}

Pour qu’une fonction numérique f, définie dans un espace topologique E, soit semi-continue inférieurement en un point $a \in E$, il faut et il suffit que $\liminf_{x \to a} f(x) = f(a)$ (ou, ce qui revient au même, que $\liminf_{x \to a} f(x) \geq f(a)$).

La condition est nécessaire. En effet, quel que soit $h < f(a)$, il existe un voisinage V de a tel que $h < f(x)$ quel que soit $x \in V$, donc $h \leq \inf_{x \in V} f(x) \leq \liminf_{x \to a} f(x)$ (IV, p. 23, formules (12)), et par suite $f(a) \leq \liminf_{x \to a} f(x)$. La condition est suffisante; en effet, si elle est vérifiée, pour tout $h < f(a)$, il existe un voisinage V de a tel que $h \leq \inf_{x \in V} f(x)$, donc f est semi-continue inférieurement au point a.

#### Proposition 5 {#top-iv-s6-prop-5 .statement}

Soit f une fonction numérique quelconque, définie dans une partie partout dense A d’un espace topologique E; si, pour tout $x \in E$, on pose $g(x) = \liminf_{y \to x, y \in A} f(y)$, g est semi-continue inférieurement dans E.

En effet, quel que soit $h < g(x)$, il existe un voisinage ouvert V de x tel que, pour tout $z \in V \cap A$, $h < f(z)$; or V est un voisinage d’un quelconque de ses points y; on a donc $\liminf_{z \to y, z \in A} f(z) = g(y) \geq h$ quel que soit $y \in V$, d’où la proposition.

On dit que g est la fonction régularisée semi-continue inférieurement de f. On définit de même la régularisée semi-continue supérieurement de f.

On peut encore définir g comme la plus grande des fonctions $\varphi$ semi-continues inférieurement dans E, et telles que $\varphi(x) \leq f(x)$ quel que soit $x \in A$. Si f est semi-continue inférieurement dans A, g est un prolongement de f à E, d’après la prop. 3.

## EXERCICES {#top-iv-s6-exercises}

See the [exercises for § 6](exercises/s6/).
