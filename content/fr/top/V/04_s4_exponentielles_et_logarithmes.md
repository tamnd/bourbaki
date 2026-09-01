---
book: top
book_title: General Topology
chapter: V
chapter_title: GROUPES À UN PARAMÈTRE
section: 4
section_title: Exponentielles et logarithmes
lang: fr
source: top-v-x-fr
book_pages: TG V.18
pdf_pages: 0018-0022, 0025-0025
extraction: ocr
subsections:
    - "no": 1
      title: Définition de $a^x$ et de $\log_a x$
      page: 11
      pdf_page: 18
    - "no": 2
      title: Variation des fonctions $a^x$ et $\log_a x$
      page: 13
      pdf_page: 20
    - "no": 3
      title: Familles multipliables de nombres $> 0$
      page: 14
      pdf_page: 21
statements: 1
exercises: 3
content_sha256: 13c4d5874b69e07b73bba14aaa5be449e3a08c434da280bc51e59cfa0e546880
---

## § 4. EXPONENTIELLES ET LOGARITHMES

### 1. Définition de $a^x$ et de $\log_a x$

#### Théorème 1 {#top-v-s4-thm-1 .statement}

Le groupe multiplicatif $\mathbf{R}_+^*$ des nombres réels $> 0$ est un groupe topologique isomorphe au groupe additif $\mathbf{R}$ des nombres réels.

En effet, $\mathbf{R}_+^* = ]0, +\infty[$ est un intervalle ouvert de $\mathbf{R}$, donc est homéomorphe à $\mathbf{R}$ (IV, p. 13, prop. 1); d’après le th. 2 de V, p. 11, c’est donc un groupe topologique isomorphe à $\mathbf{R}$.

D’après le corollaire de V, p. 3, pour tout nombre $a > 0$, il existe un homomorphisme continu et un seul $f_a$ de $\mathbf{R}$ dans $\mathbf{R}_+^*$, tel que $f_a(1) = a$. Quels que soient $x \in \mathbf{R}$, $y \in \mathbf{R}$, on a donc

$$
f_a(x + y) = f_a(x)f_a(y), \quad f_a(-x) = \frac{1}{f_a(x)},
$$

d’où en particulier, pour tout entier $n \in \mathbf{Z}$,

$$
f_a(n) = a^n.
$$

En raison de cette relation, on note, pour tout $x \in \mathbf{R}$, $f_a(x) = a^x$; les fonctions $a^x$ (pour toutes les valeurs > 0 de a) sont dites fonctions exponentielles. On a $1^x = 1$ quel que soit $x \in \mathbf{R}$; pour $a \neq 1$, $a^x$ est un isomorphisme du groupe $\mathbf{R}$ sur le groupe $\mathbf{R}_+^*$.

Pour $a \neq 1$, l’isomorphisme de $\mathbf{R}_+^*$ sur $\mathbf{R}$, réciproque de $a^x$, s’appelle logarithme de base $a$, et sa valeur pour $x \in \mathbf{R}_+^*$ se note $\log_a x$. On a donc, avec ces notations,

(1) $$
a^{x+y} = a^x a^y \quad \text{pour } x \in \mathbf{R}, y \in \mathbf{R}, a > 0;
$$
(2) $$
a^{-x} = \frac{1}{a^x} \quad \text{pour } x \in \mathbf{R}, a > 0;
$$
(3) $$
\log_a 1 = 0, \quad \log_a a = 1 \quad \text{pour } a > 0 \text{ et } \neq 1;
$$
(4) $$
\log_a(xy) = \log_a x + \log_a y \quad \text{pour } x > 0, y > 0;
$$
(5) $$
\log_a \left( \frac{1}{x} \right) = -\log_a x \quad \text{pour } x > 0;
$$
(6) $$
a^{\log_a x} = x \quad \text{pour } x > 0;
$$
(7) $$
\log_a(a^x) = x \quad \text{pour } x \in \mathbf{R}.
$$

D’après la prop. 5 de V, p. 2, tout homomorphisme continu de $\mathbf{R}$ dans $\mathbf{R}_+^*$ est de la forme $y \mapsto a^{xy}$, où $x \in \mathbf{R}$; comme sa valeur pour $y = 1$ est $a^x$, on a identiquement

(8) $$
(a^x)^y = a^{xy} \quad \text{pour } x \in \mathbf{R}, y \in \mathbf{R}, a > 0
$$
ou, en changeant les notations,
(9) $$
x^y = a^{y \cdot \log_a x} \quad \text{pour } x > 0, y \in \mathbf{R}, a > 0 \text{ et } \neq 1.
$$

La formule (8) montre que pour tout entier $n > 0$, on a $(a^{1/n})^n = a$, donc $a^{1/n}$ est la racine $n$-ième $\sqrt[n]{a}$, définie dans IV, p. 12.

Les formules (7) et (9) montrent que
(10) $$
\log_a(x^y) = y \cdot \log_a x \quad \text{pour } x > 0 \text{ et } y \in \mathbf{R},
$$
ou, en changeant les notations,
(11) $$
\log_a x = \log_a b \cdot \log_b x \quad \text{pour } x > 0, a > 0, b > 0, a \neq 1, b \neq 1
$$
(formule dite « du changement de base »).

Cherchons enfin tous les homomorphismes continus du groupe topologique $\mathbf{R}_+^*$ dans lui-même; si $g$ est un tel homomorphisme, $\log_a(g(a^x))$ est un homomorphisme continu de $\mathbf{R}$ dans $\mathbf{R}$, donc (V, p. 2, prop. 5) il existe $\alpha \in \mathbf{R}$ tel que $\log_a(g(a^x)) = \alpha x$ quel que soit $x \in \mathbf{R}$; d’où on tire, en vertu de (8), l’identité $g(x) = x^\alpha$ quel que soit $x > 0$. On a donc identiquement
(12) $$
(xy)^\alpha = x^\alpha y^\alpha \quad \text{quels que soient } x > 0, y > 0, \alpha \in \mathbf{R}.
$$

En raison de la formule (4), qui ramène toute multiplication à une addition (seule opération à laquelle soit vraiment adapté le système de numération en usage), les logarithmes ont longtemps été un instrument indispensable pour le calcul numérique (voir la Note historique de ce chapitre).

Lorsqu’on les utilise à cette fin, on choisit la base $a = 10$; et il existe des tables donnant les valeurs de la fonction $\log_{10} x$ (avec une certaine approximation). En Analyse, on est conduit, comme nous le verrons ultérieurement (FVR, III, §1, n° 1), à un autre choix de la base, celle-ci (qu’on note $e$) étant prise telle qu’on ait
$$
\lim_{x \to 1, x \neq 1} \frac{\log_e x}{x - 1} = 1 \quad (\text{cf. V, p. 18, exerc. 1}).
$$

### 2. Variation des fonctions $a^x$ et $\log_a x$

D’après le th. 5 de IV, p. 9, pour $a \neq 1$, $x \mapsto a^x$ est une application strictement monotone de $\mathbf{R}$ sur l’intervalle $\mathbf{R}_+^* = ]0, +\infty[$. Si $a > 1$, $a^1 = a > 1 = a^0$, donc $a^x$ est strictement croissante; en outre, $\mathbf{R}_+^*$ n’étant pas borné supérieurement, $a^x$ n’est pas bornée supérieurement dans $\mathbf{R}$, donc
$$
\lim_{x \to +\infty} a^x = +\infty \qquad (a > 1)
$$
et, d’après (2) (V, p. 12),
$$
\lim_{x \to -\infty} a^x = 0 \qquad (a > 1).
$$
Au contraire, si $a < 1$, la fonction $a^x$ est strictement décroissante dans $\mathbf{R}$, tend vers 0 lorsque $x$ tend vers $+\infty$, vers $+\infty$ lorsque $x$ tend vers $-\infty$ (fig. 1).

![Figure 1](https://i.imgur.com/1.png)

Figure 1

![Figure 2](https://i.imgur.com/2.png)

Figure 2

De ces propriétés, et de (12), on déduit que si $0 < a < b$, on a $a^x < b^x$ pour $x > 0$, $a^x > b^x$ pour $x < 0$; cela revient en effet à constater que $(b/a)^x > 1$ pour $x > 0$, $(b/a)^x < 1$ pour $x < 0$.

La variation de $\log_a x$ dans $\mathbf{R}_+^*$ se déduit de celle de $a^x$ dans $\mathbf{R}$; si $a > 1$, la fonction $\log_a x$ est strictement croissante, tend vers $-\infty$ quand $x$ tend vers 0, vers $+\infty$ quand $x$ tend vers $+\infty$; si $a < 1$, la fonction $\log_a x$ est strictement décroissante, tend vers $+\infty$ quand $x$ tend vers $0$, vers $-\infty$ quand $x$ tend vers $+\infty$ (fig. 2).

La fonction $a^x$ (resp. $\log_a x$) étant considérée comme définie sur une partie de la droite achevée $\overline{\mathbf{R}}$ et prenant ses valeurs dans $\overline{\mathbf{R}}$, on peut la prolonger par continuité à $\overline{\mathbf{R}}$ (resp. à l’intervalle $[0, +\infty)$ de $\overline{\mathbf{R}}$), en lui donnant aux points $+\infty$ et $-\infty$ (resp. $0$ et $+\infty$) ses valeurs limites en ces points.

Plus généralement, la formule (9) (V, p. 12) montre que la fonction $x^y$ est continue dans le sous-espace $\mathbf{R}_+^* \times \mathbf{R}$ de $\overline{\mathbf{R}}^2$, et tend vers une limite lorsque $(x, y)$ tend vers un point $(a, b)$ de $\overline{\mathbf{R}}^2$ adhérent à $\mathbf{R}_+^* \times \mathbf{R}$, à l’exception des points $(0, 0)$, $(+\infty, 0)$, $(1, +\infty)$, $(1, -\infty)$. On peut donc encore prolonger par continuité $x^y$ aux points de $\overline{\mathbf{R}}^2$ où sa limite existe; d’après le principe de prolongement des identités (I, p. 53, cor. 1), les formules (1), (4) et (8) de V, p. 12 sont encore valables lorsque chacun des deux membres a un sens.

On notera que le prolongement par continuité de $x^y$ ne permet pas de retrouver la formule $0^0 = 1$ qui résultait des conventions faites en Algèbre (A, I, p. 13); il convient d’éviter toute confusion à cet égard.

On remarquera aussi que la définition de l’exponentielle permet de prolonger à $\mathbf{R}$ la fonction $n \mapsto a^n$ définie dans $\mathbf{Z}$, pour tout $a > 0$; mais nous n’obtenons ainsi aucun prolongement de cette fonction lorsque $a < 0$; un prolongement « naturel » de cette fonction ne pourra être défini qu’avec la théorie des fonctions analytiques.

### 3. Familles multipliables de nombres $> 0$

L’isomorphie des groupes topologiques $\mathbf{R}$ et $\mathbf{R}_+^*$ montre aussitôt que, pour qu’une famille $(x_i)$ de nombres réels finis et $> 0$ soit multipliable (IV, p. 35), il faut et il suffit que la famille $(\log_a x_i)$ soit sommable ($a$ étant un nombre quelconque $> 0$ et $\neq 1$); on a en outre

$$
\prod_i x_i = a^{\sum_{\log_a x_i}}
$$

De même, pour qu’un produit infini défini par une suite $(1 + u_n)$ de nombres finis et $> 0$ soit convergent (IV, p. 39), il faut et il suffit que la série de terme général $\log_a (1 + u_n)$ soit convergente, et on a

$$
\prod_{n=0}^{\infty} (1 + u_n) = a^{\sum_{n=0}^{\infty} \log_a (1 + u_n)}
$$

L’étude des produits infinis de nombres réels $> 0$ est donc ramenée à celle des sommes infinies de nombres réels, dont les termes se présentent sous forme de logarithmes; nous verrons plus tard comment les sommes de cette nature s’étudient au moyen des propriétés différentielles du logarithme (cf., par exemple, FVR, V, § 5, n° 3).

Exercises

## EXERCICES {#top-v-s4-exercises}

See the [exercises for § 4](exercises/s4/).
