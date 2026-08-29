---
book: alg
book_title: Algebra
chapter: VII
chapter_title: Modules sur les anneaux principaux
section: 3
section_title: MODULES LIBRES SUR UN ANNEAU PRINCIPAL
lang: fr
source: alg-iv-vii-fr
book_pages: A VII.14-A VII.15, A VII.58-A VII.60
pdf_pages: 0347-0348, 0391-0393
extraction: ocr
statements: 8
exercises: 11
content_sha256: 632af2a4cecdfd0dde79ecc8af75dba08c5be8fd7baaf23be89443f94cb3aa3f
---

## § 3. MODULES LIBRES SUR UN ANNEAU PRINCIPAL

#### Théorème 1 {#alg-vii-s3-thm-1 .statement}

Soit $A$ un anneau tel que tout idéal à gauche de $A$ soit un $A$-module projectif (II, p. 39, déf. 1). Tout sous-module $M$ d’un $A$-module à gauche libre $L$ est somme directe de modules isomorphes à des idéaux de $A$.

Soit $(e_i)_{i \in I}$ une base de $L$, et soient $p_i$ les fonctions coordonnées relatives à cette base. Munissons $I$ d’une structure d’ensemble bien ordonné (E, III, p. 20, th. 1), et désignons par $L_i$ le sous-module engendré par les $e_\lambda$ pour $\lambda \leq i$; nous poserons $M_i = M \cap L_i$. La fonction coordonnée $p_i$ applique $M_i$ sur un idéal $a_i$ de $A$; puisque $a_i$ est un $A$-module projectif, il existe (II, p. 39, prop. 4) un sous-module $N_i$ de $M_i$ tel que l’application $x \mapsto p_i(x)$ de $N_i$ dans $a_i$ soit bijective. Soit $M'_i$ le sous-module de $L$ engendré par les $N_\lambda$ pour $\lambda \leq i$; nous allons montrer que $M'_i = M_i$ pour tout $i$, ce qui impliquera que $M$ est engendré par la famille $(N_i)_{i \in I}$. Supposons en effet que l’on ait $M'_\lambda = M_\lambda$ pour tout $\lambda < i$; alors, pour tout $x \in M_i$, on a $p_i(x) \in a_i$; il existe donc $y \in N_i$ tel que $x - y$ soit combinaison linéaire d’un nombre fini d’éléments $e_\lambda$ avec $\lambda < i$; autrement dit, $x - y$ est élément d’un $M_\lambda$ avec $\lambda < i$; l’hypothèse de récurrence montre que $x - y \in M'_\lambda \subset M'_i$ c’est-à-dire $x \in M'_i$, d’où $M'_i = M_i$. Reste à montrer que la somme des $N_i$ est directe ; or, supposons qu’il existe une relation linéaire $\sum_i a_i = 0$, avec $a_i \in N_i$ où les $a_i$ (nuls sauf un nombre fini d’entre eux) ne sont pas tous nuls. Soit $\mu$ le plus grand des indices $i$ tels que $a_i \neq 0$; comme $p_\mu(a_\lambda) = 0$ pour $\lambda < \mu$, on a $p_\mu(a_\mu) = p_\mu(\sum_i a_i) = 0$ donc $a_\mu = 0$, ce qui est contraire à l’hypothèse.

#### Corollaire 1 {#alg-vii-s3-thm-1-cor-1 .statement}

Si tout idéal à gauche de $A$ est projectif, tout sous-module d’un $A$-module à gauche projectif est projectif.

En effet, tout $A$-module projectif est isomorphe à un sous-module d’un module libre (II, p. 39, prop. 4) et on applique le th. 1.

#### Corollaire 2 {#alg-vii-s3-thm-1-cor-2 .statement}

Sur un anneau principal, tout sous-module d’un module libre est libre.

Tous les idéaux d’un anneau principal étant des modules libres, cela résulte directement du th. 1.

#### Corollaire 3 {#alg-vii-s3-thm-1-cor-3 .statement}

Tout module projectif sur un anneau principal est libre.

#### Remarque {#alg-vii-s3-n0-rem-1 .statement}

La démonstration du th. 1 montre que tout sous-module de $A^{(I)}$ est isomorphe à une somme directe $\bigoplus_{i \in I} a_i$, où chaque $a_i$ est un idéal de $A$.

#### Proposition 1 {#alg-vii-s3-prop-1 .statement}

Si $L$ est un module libre de rang fini $n$ sur un anneau principal $A$, tout sous-module $M$ de $L$ est un module libre de rang $\leq n$.

En effet, $M$ est un module libre d’après le cor. 2 au th. 1, et il est de rang $\leq n$ d’après la remarque précédente ou le lemme suivant :

#### Lemme 1 {#alg-vii-s3-lem-1 .statement}

Soient L un module sur un anneau commutatif A, ayant un système générateur de n éléments, et M un sous-module libre de L ; alors M est de rang $\leq n$.

Supposons tout d’abord L libre. Notons i l’injection canonique de M dans L. D’après III, p. 88, cor., l’homomorphisme $\Lambda^{n+1}i : \Lambda^{n+1}M \to \Lambda^{n+1}L$ est injectif ; d’après III, p. 80, prop. 6, $\Lambda^{n+1}L = \{0\}$, donc $\Lambda^{n+1}M = \{0\}$; il en résulte que M est de rang $\leq n$ (III, p. 87, cor. 1). Passons maintenant au cas général ; L est un quotient d’un module libre L’ de rang n. Il existe un sous-module M’ de L’ isomorphe à M (II, p. 27, prop. 21). D’après la première partie du raisonnement, M’ est de rang $\leq n$, d’où le résultat.

#### Corollaire {#alg-vii-s3-n0-cor-1 .statement}

Soit E un module sur un anneau principal A, engendré par n éléments. Tout sous-module F de E admet un système générateur ayant au plus n éléments.

Il existe en effet un homomorphisme f de $A^n$ sur E (II, p. 25, cor. 3), et $\bar{f}(F)$, qui est un module libre de rang $m \leq n$, est engendré par m éléments ; les images de ceux-ci par f engendrent F.

## EXERCICES {#alg-vii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
