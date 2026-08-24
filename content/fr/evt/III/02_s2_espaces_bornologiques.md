---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: ESPACES D’APPLICATIONS LINÉAIRES CONTINUES
section: 2
section_title: Espaces bornologiques
lang: fr
source: evt-i-v-fr
book_pages: EVT III.11-EVT III.13, EVT III.41-EVT III.42
pdf_pages: 0146-0148, 0176-0177
extraction: ocr
statements: 7
exercises: 4
content_sha256: dbe72fe42844e76b16c4733d97f80a7bdc97378d5a552921a91626f089aa4b8a
---

## § 2. ESPACES BORNOLOGIQUES

Dans ce paragraphe, E désigne un espace localement convexe, et $ \mathcal{B} $ sa bornologie canonique (III, p. 3, déf. 5).

#### Lemme 1 {#evt-iii-s2-lem-1 .statement}

Soient G un espace semi-normé, p sa semi-norme, et soit u une application linéaire de G dans E. Les conditions suivantes sont équivalentes :

(i) u est continue ;
(ii) l’image par u de la boule unité de G est bornée dans E ;
(iii) pour toute suite $ (x_n) $ de points de G tendant vers 0, la suite $ (u(x_n)) $ est bornée dans E.

Il est immédiat que (i) entraîne (ii) (III, p. 4, cor. 1) et que (ii) entraîne (iii). Soit maintenant V un voisinage de 0 dans E ; si $ u^{-1}(V) $ n’est pas un voisinage de 0 dans G, il existe une suite $ (y_n) $ de points de G – $ u^{-1}(V) $ telle que $ p(y_n) \leqslant \frac{1}{n^2} $. Alors la suite des $ x_n = ny_n $ tend vers 0 dans G et $ u(x_n) \notin nV $, ce qui entraîne que la suite $ (u(x_n)) $ n’est pas bornée. Par suite (iii) entraîne (i).

#### Proposition 1 {#evt-iii-s2-prop-1 .statement}

Les conditions suivantes sont équivalentes :

(i) Toute semi-norme sur E qui est bornée sur les parties bornées de E est continue.
(i bis) Toute partie convexe équilibrée de E qui absorbe les parties bornées de E (I, p. 7, déf. 4) est un voisinage de 0 dans E.
(ii) E est limite inductive des espaces semi-normés $ E_A $ quand A décrit l’ensemble filtrant croissant des parties convexes, équilibrées, fermées et bornées de E.
(ii bis) Il existe une famille $ (E_i)_{i \in I} $ d’espaces semi-normés et, pour chaque $ i \in I $, une application linéaire $ u_i : E_i \to E $ telles que la topologie de E soit la topologie localement convexe la plus fine rendant les $ u_i $ continues.
(iii) Quel que soit l’espace localement convexe F, une application linéaire $ u : E \to F $ est continue si et seulement si pour toute suite $ (x_n) $ de points de E tendant vers 0, la suite $ (u(x_n)) $ est bornée dans F.

(iii bis) Quel que soit l’espace semi-normé F, une application linéaire u : E → F est continue si et seulement si u(X) est borné dans F pour tout ensemble X borné dans E.

Il est immédiat que (i) et (i bis) sont équivalentes, vu la correspondance entre semi-normes et parties convexes équilibrées absorbantes (II, p. 22). Si p est une semi-norme sur E, continue sur chaque E_A, alors p est bornée sur les parties bornées de E ; donc (i) entraîne (ii) (II, p. 29, prop. 5). Il est clair que (ii) entraîne (ii bis).

Soit maintenant (E_i, u_i)_{i \in I} comme dans (ii bis), et soit u une application linéaire de E dans un espace localement convexe F, telle que (u(x_n)) soit bornée dans F pour toute suite (x_n) de points de E tendant vers 0. Il résulte du lemme 1 de III, p. 11 que l’application linéaire u o u_i : E_i → F est continue quelle que soit i ∈ I ; donc, si la topologie de E est la topologie localement convexe la plus fine rendant les u_i continues, u est continue (II, p. 29, prop. 5). Ceci montre que (ii bis) entraîne (iii).

Il est immédiat que (iii) entraîne (iii bis) (III, p. 3, corollaire). Enfin, si p est une semi-norme sur E, bornée sur les parties bornées de E, la condition (iii bis) affirme que l’application identique est continue de E dans l’espace semi-normé (E, p) ; autrement dit p est continue. Ceci montre que (iii bis) entraîne (i).

#### Définition 1 {#evt-iii-s2-def-1 .statement}

On dit qu’un espace localement convexe est bornologique s’il satisfait aux conditions équivalentes de la prop. 1.

#### Exemple 1 {#evt-iii-s2-exa-1 .statement}

Tout espace semi-normé est bornologique.
2) En particulier, tout espace localement convexe de dimension finie est bornologique.
3) Compte tenu de la transitivité des topologies localement convexes finales (II, p. 30, cor. 2), on déduit aussitôt de la condition (ii bis) que si (E_i)_{i \in I} est une famille d’espaces localement convexes bornologiques et si E est muni de la topologie localement convexe la plus fine rendant continues des applications linéaires u_i : E_i → E (pour i ∈ I), alors E est bornologique. En particulier, une limite inductive, une somme directe, un espace quotient d’espaces bornologiques sont des espaces bornologiques.

Par contre, un sous-espace fermé d’un espace bornologique n’est pas nécessairement bornologique (IV, p. 63, exerc. 8).

#### Corollaire {#evt-iii-s2-n0-cor-1 .statement}

Tout espace bornologique séparé et semi-complet est limite inductive d’espaces de Banach.

En effet, les espaces E_A où A est borné et fermé sont alors des espaces de Banach (III, p. 8, corollaire).

#### Proposition 2 {#evt-iii-s2-prop-2 .statement}

Un espace localement convexe métrisable est bornologique.

Supposons E métrisable, et soit p une semi-norme sur E, bornée sur les parties bornées de E. Supposons que p ne soit pas continue et soit A l’ensemble des x ∈ E tels que p(x) < 1. Soit (V_n)_{n \geq 1} une suite décroissante formant un système fondamental de voisinages de 0 dans E. Comme p n’est pas continue, A n’est pas un voisinage de 0 ; pour tout $ n > 0 $, on a donc $ A \not\supseteq n^{-1}V_n $ et il existe un point $ x_n $ de $ V_n $ tel que $ n^{-1}x_n \notin A $, c’est-à-dire $ p(x_n) \geq n $. La suite $ (x_n) $ tend vers 0, donc est bornée (III, p. 3, corollaire) ; ceci contredit l’hypothèse sur $ p $.

#### Corollaire {#evt-iii-s2-n0-cor-2 .statement}

*Tout espace de Fréchet* (II, p. 26) *est limite inductive d’espaces de Banach*.

## EXERCICES {#evt-iii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
