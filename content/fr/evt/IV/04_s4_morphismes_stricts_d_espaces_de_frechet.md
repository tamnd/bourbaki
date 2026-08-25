---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: LA DUALITÉ DANS LES ESPACES VECTORIELS TOPOLOGIQUES
section: 4
section_title: Morphismes stricts d’espaces de Fréchet
lang: fr
source: evt-i-v-fr
book_pages: EVT IV.26-EVT IV.31, EVT IV.62-EVT IV.67
pdf_pages: 0212-0217, 0248-0253
extraction: ocr
subsections:
    - "no": 1
      title: Caractérisations des morphismes stricts
      page: 26
      pdf_page: 212
    - "no": 2
      title: Morphismes stricts d’espaces de Fréchet
      page: 28
      pdf_page: 214
    - "no": 3
      title: Critères de surjectivité
      page: 30
      pdf_page: 216
statements: 13
exercises: 23
content_sha256: b9998a7b218f6ef8780fed9ae6996d5d7de396981f85e4de36f4ce106816fd85
---

## § 4. MORPHISMES STRICTS D’ESPACES DE FRÉCHET

Pour tout espace localement convexe $E$, on note $S(E)$ l’ensemble des semi-normes continues sur $E$. Pour tout $p \in S(E)$, on note $H_p$ l’ensemble des formes linéaires $f$ sur $E$ telles que $|f| \leq p$. La famille $(H_p)_{p \in S(E)}$ est une base de la bornologie formée des parties équicontinues de $E'$.

### 1. Caractérisations des morphismes stricts

#### Proposition 1 {#evt-iv-s4-prop-1 .statement}

Soient $E$ et $F$ deux espaces localement convexes et $u$ une application linéaire continue de $E$ dans $F$. Pour que $u$ soit un morphisme strict, il faut et il suffit que la condition suivante soit satisfaite :

(MS) Pour toute semi-norme $p \in S(E)$, nulle sur le noyau de $u$, il existe $q$ dans $S(F)$ telle que $p \leq q \circ u$.

Soient $N$ le noyau et $M$ l’image de $u$; introduisons la décomposition canonique de $u$, soit
$$
E \xrightarrow{\pi} E/N \xrightarrow{\tilde{u}} M \to F .
$$
Les semi-normes continues sur $E$, nulles sur $N$, sont les semi-normes $p_1 \circ \pi$ où $p_1$ parcourt $S(E/N)$; de même $S(M)$ se compose des semi-normes $q_1$ pour lesquelles il existe $q \in S(F)$ avec $q_1 \leq q|F$. Enfin, $u$ est un morphisme strict si et seulement si l’application linéaire bijective continue $\tilde{u}$ a un inverse continu ; ceci signifie aussi que toute semi-norme dans $S(E/N)$ est de la forme $q_1 \circ \tilde{u}$ avec $q_1$ dans $S(M)$. La prop. 1 résulte aussitôt de ces remarques.

#### Proposition 2 {#evt-iv-s4-prop-2 .statement}

Soient E et F des espaces localement convexes séparés et u une application linéaire continue de E dans F. Pour que u soit un morphisme strict, il faut et il suffit que sa transposée $^t u : F' \to E'$ satisfasse aux conditions suivantes :

a) L’image de $^t u$ est fermée dans $E'$ pour $\sigma(E', E)$.

b) Toute partie équicontinue de $E'$, contenue dans l’image de $^t u$, est image par $^t u$ d’une partie équicontinue de $F'$.

S’il en est ainsi, on a $\mathrm{Ker}\ ^t u = (\mathrm{Im}\ u)^{\circ}$ et $\mathrm{Im}\ ^t u = (\mathrm{Ker}\ u)^{\circ}$, et il existe des isomorphismes canoniques de $\mathrm{Coker}\ ^t u$ sur le dual de $\mathrm{Ker}\ u$ et de $\mathrm{Ker}\ ^t u$ sur le dual de $\mathrm{Coker}\ u$.

Soient N le noyau et I l’image de u. D’après le cor. 2 de II, p. 51, le noyau de $^t u$ est l’orthogonal de I, et l’adhérence de l’image de $^t u$ pour $\sigma(E', E)$ est l’orthogonal $N^{\circ}$ de N. La conjonction de a) et b) équivaut donc à la condition suivante :

b') Toute partie équicontinue de $E'$ contenue dans $N^{\circ}$ est l’image par $^t u$ d’une partie équicontinue de $F'$.

Comme $N^{\circ}$ s’identifie au dual de $E/N$, la prop. 9, (i) de IV, p. 8 montre que les parties équicontinues de $E'$ contenues dans $N^{\circ}$ sont les ensembles contenus dans un ensemble de la forme $H_p$, où $p$ est une semi-norme continue sur E, nulle sur N. La condition b') signifie donc que, pour toute semi-norme $p \in S(E)$ nulle sur N, il existe $q \in S(F)$ telle que $H_p \subset ^t u(H_q)$. D’après le th. de Hahn-Banach (II, p. 24, cor. 1 et 2, et p. 67, th. 1 et cor. 1), on a $^t u(H_q) = H_{q_{ou}}$, et les relations $H_p \subset H_{p'}$ et $p \leq p'$ sont équivalentes quelles que soient les semi-normes $p$ et $p'$ dans $S(E)$. Par suite, la relation $H_p \subset ^t u(H_q)$ équivaut à la relation $p \leq q \circ u$. D’après la prop. 1, la propriété b') signifie donc que u est un morphisme strict.

Supposons que u soit un morphisme strict. On a déjà vu que le noyau de $^t u$ est l’orthogonal de I et que l’image de $^t u$ est l’orthogonal de N. Le conoyau de u est l’espace F/I et son dual s’identifie à $I^{\circ} = \mathrm{Ker}\ ^t u$. De même, le dual de $N = \mathrm{Ker}\ u$ s’identifie à $E'/N^{\circ}$ (IV, p. 8), c’est-à-dire au conoyau de $^t u$ puisque $N^{\circ}$ est l’image de $^t u$.

#### Remarque {#evt-iv-s4-n1-rem-1 .statement}

Avec les notations de la prop. 2, la propriété a) signifie encore que u est un morphisme strict pour les topologies affaiblies (II, p. 52, cor. 3).

#### Proposition 3 {#evt-iv-s4-prop-3 .statement}

Soient E et F deux espaces localement convexes et u une application linéaire continue de E dans F. On suppose E séparé et F métrisable. Pour que u soit un morphisme strict, il faut et il suffit que l’image de $^t u$ soit fermée dans $E'$ pour la topologie faible $\sigma(E', E)$.

La nécessité résulte de la prop. 2.

Supposons réciproquement l’image de $^t u$ fermée pour $\sigma(E', E)$ et introduisons la décomposition canonique de u comme dans la démonstration de la prop. 1. D’après la remarque ci-dessus, l’application réciproque $\tilde{u}^{-1}$ de $\tilde{u}$ est continue pour les topologies affaiblies. Or le sous-espace $M = u(E)$ de F est métrisable, donc bornologique (III, p. 12, prop. 2); par suite (IV, p. 7, prop. 7, (ii)), $\tilde{u}^{-1}$ est continue, donc u est un morphisme strict.

### 2. Morphismes stricts d’espaces de Fréchet

#### Théorème 1 {#evt-iv-s4-thm-1 .statement}

Soient E et F deux espaces de Fréchet et u une application linéaire continue de E dans F. Les conditions suivantes sont équivalentes :

a) u est un morphisme strict.
b) u est un morphisme strict pour les topologies affaiblies.
c) L’image de u est fermée dans F.
d) $'u$ est un morphisme strict de F’ dans E’ pour les topologies faibles.
e) L’image de $'u$ est fermée dans E’ pour la topologie faible $\sigma(E', E)$.
f) L’image de $'u$ est fermée dans E’ pour la topologie forte $\beta(E', E)$.
g) $'u$ est un morphisme strict de $F'_c$ dans $E'_c$ (duals munis de la topologie de la convergence compacte).

L’équivalence de a), b) et e) résulte de la prop. 3 de IV, p. 27, et de la remarque qui la précède. Celle de a) et c) n’est autre que le cor. 3 de I, p. 19. La remarque de IV, p. 27, montre aussi que d) équivaut au fait que l’image de u est fermée pour la topologie affaiblie $\sigma(F, F')$ de F ; l’équivalence de c) et d) résulte donc de la prop. 2 de IV, p. 4.

Prouvons l’équivalence de e) et f). Il suffit de prouver que f) implique e). Supposons donc que l’image de $'u$ soit fermée pour $\beta(E', E)$ dans E’. Compte tenu du th. de Banach-Dieudonné (IV, p. 25, cor. 2), il suffit de prouver que, pour tout voisinage convexe équilibré U de 0 dans E, l’intersection $B = 'u(F') \cap U^\circ$ est compacte pour $\sigma(E', E)$. Le dual fort $E'_b$ de l’espace de Fréchet E est complet (IV, p. 21, prop. 2), donc la partie fermée B de $E'_b$ est complète, et l’espace normé $E'_B$ est complet (III, p. 8, corollaire). Soit $(V_n)$ une suite décroissante formant un système fondamental de voisinages de 0 dans F. Alors F’ est réunion des ensembles $C_n = V_n^\circ$ qui sont compacts pour $\sigma(F', F)$, d’où $E'_B = \bigcup B_n$, avec $B_n = E'_B \cap 'u(C_n)$.

Comme $E'_B$ est un espace de Baire, et que chacun des ensembles $B_n$ est convexe, équilibré et fermé, il existe un nombre réel $r > 0$ et un entier $n$ tels que $B \subset r.B_n$. On a alors $B = U^\circ \cap 'u(r.C_n)$; comme les ensembles $U^\circ$ et $r.C_n$ sont compacts et $'u$ continue pour les topologies faibles, B est compact pour $\sigma(E', E)$. Ceci achève la démonstration de l’équivalence de e) et f).

Enfin, l’équivalence de g) et des conditions précédentes résulte de la prop. 18 de TG, IX, p. 22, et du lemme suivant :

#### Lemme 1 {#evt-iv-s4-lem-1 .statement}

Soient E et F deux espaces localement convexes séparés quasi-complets et u une application linéaire continue de E dans F. Pour que $'u$ soit un morphisme strict de $F'_c$ dans $E'_c$, il faut et il suffit que l’image $u(E)$ de u soit fermée, et que toute partie compacte de $u(E)$ soit l’image par u d’une partie compacte de E.

D’après le th. de Mackey (IV, p. 2, th. 1) et le fait que sur E’ (resp. F’) la topologie de la convergence compacte coïncide avec celle de la convergence convexe compacte (IV, p. 4), on peut identifier E (resp. F) au dual de $E'_c$ (resp. $F'_c$). Alors $u$ est la transposée de $'u$, et les parties équicontinues de E (resp. F) sont les ensembles relativement compacts. Le lemme 1 résulte alors de la prop. 2 (IV, p. 27), car $u(E)$ est fermé dans F si et seulement s’il l’est pour la topologie affaiblie $\sigma(F, F')$ (IV, p. 4, prop. 2).

#### Corollaire 1 {#evt-iv-s4-lem-1-cor-1 .statement}

Sous les hypothèses du th. 1, les conditions suivantes sont équivalentes :
(i) $u$ est un morphisme strict injectif ;
(ii) $^t u$ est un morphisme strict surjectif pour les topologies faibles ;
(iii) $^t u$ est surjectif.
L’implication (i) $\Rightarrow$ (ii) résulte aussitôt de l’équivalence des conditions $a), d)$ et $e)$ du th. 1 et de IV, p. 6, prop. 5. Il est clair que (ii) entraîne (iii). Montrons enfin que (iii) entraîne (i) : si $^t u$ est surjectif, $u$ est un morphisme strict d’après l’équivalence de $a)$ et $e)$ dans le th. 1 ; que $u$ soit injectif résulte de la prop. 5 de IV, p. 6.

#### Corollaire 2 {#evt-iv-s4-lem-1-cor-2 .statement}

Sous les hypothèses du th. 1, les conditions suivantes sont équivalentes :
(i) $u$ est surjectif ;
(ii) $u$ est un morphisme strict surjectif ;
(iii) $^t u$ est un morphisme strict injectif pour les topologies faibles.
L’équivalence de (i) et (ii) résulte du th. de Banach (I, p. 17, th. 1).
D’après l’équivalence de $a)$ et $c)$ dans le th. 1, la condition (ii) signifie que $u$ est un morphisme strict et que son image est dense dans F pour $\sigma(F, F')$. L’équivalence de (ii) et (iii) résulte alors de l’équivalence de $a)$ et $d)$ dans le th. 1 et de la prop. 5 de IV, p. 6.

Si $u : E \to F$ est un morphisme strict d’espaces de Fréchet, la transposée $^t u$ n’est pas nécessairement un morphisme strict de $F'_b$ dans $E'_b$ (IV, p. 62, exerc. 3). On a cependant le résultat partiel suivant :

#### Corollaire 3 {#evt-iv-s4-lem-1-cor-3 .statement}

Sous les hypothèses du th. 1, les propriétés a) à g) sont entraînées par la suivante :
h) $^t u$ est un morphisme strict de $F'_b$ dans $E'_b$.
Lorsque E et F sont tous deux des espaces de Banach, ou tous deux des espaces de Montel, la propriété h) est équivalente aux propriétés a) à g) du th. 1.
Supposons que $^t u$ soit un morphisme strict de $F'_b$ dans $E'_b$. Nous allons prouver que l’image H de $^t u$ est fermée dans $E'_b$, d’où la première assertion du cor. 3.
Soit G l’adhérence de l’image de $u$ dans F ; muni de la topologie induite par celle de F, c’est un espace de Fréchet. L’application $u : E \to F$ se factorise en $u = j \circ v$ où $j$ est l’injection canonique de G dans F et où $v \in \mathcal{L}(E; G)$. On a alors $^t u = ^t v \circ ^t j$, où $^t j$ est surjective d’après le th. de Hahn-Banach (II, p. 26, prop. 2) ; de plus, $^t v$ est injective puisque $v(E)$ est dense dans G (IV, p. 6, prop. 5). Par hypothèse, l’application $^t u$ de $F'_b$ sur H est ouverte ; comme $^t j$ est surjective et continue, l’application $^t v$ induit un homéomorphisme de $G'_b$ sur H. Or le dual $G'_b$ de l’espace de Fréchet G est complet (IV, p. 21, prop. 2) ; par suite, H est complet, donc fermé dans $E'_b$.

Si E et F sont des espaces de Montel, la topologie forte sur E' (resp. F') coïncide avec la topologie de la convergence compacte, et h) n’est qu’une reformulation de g).

Si E et F sont des espaces de Banach, il en est de même de E'_b et F'_b, et la condition h) équivaut à f) d’après l’équivalence de a) et c) appliquée à 'u : F'_b → E'_b.

#### Corollaire 4 {#evt-iv-s4-lem-1-cor-4 .statement}

Supposons que E et F soient des espaces de Banach. Pour que 'u soit surjective, il faut et il suffit qu’il existe un nombre réel r > 0 tel que $\|x\| \leq r \cdot \|u(x)\|$ pour tout $x \in E$.

Cela ne fait que traduire l’équivalence des conditions (i) et (iii) du cor. 1.

#### Corollaire 5 {#evt-iv-s4-lem-1-cor-5 .statement}

Soient E et F des espaces de Fréchet et u une application linéaire continue de E dans F. Les conditions suivantes sont équivalentes :

a) u est un isomorphisme de E sur F.
b) u est un isomorphisme de E sur F pour les topologies affaiblies.
c) 'u est un isomorphisme de F' sur E' pour les topologies faibles.
d) 'u est un isomorphisme de F' sur E' pour les topologies fortes.
e) 'u est un isomorphisme de F'_c sur E'_c.

Comme un isomorphisme n’est autre qu’un morphisme strict bijectif, l’équivalence de a) et b) résulte de l’équivalence des conditions a) et b) du th. 1.

Il est clair que a) entraîne chacune des conditions c), d) et e).

Réciproquement, supposons que l’une des conditions c), d) ou e) soit satisfaite. Il résulte du th. 1 et de son cor. 3 que u est un morphisme strict de E dans F, et 'u est évidemment bijectif. Soit N (resp. I) le noyau (resp. l’image) de u. Comme 'u est bijectif, on a Im 'u = E' et Ker 'u = {0}, d’où N° = E' et I° = {0} d’après la prop. 2 de IV, p. 27. Or N (resp. I) est un sous-espace vectoriel fermé de E (resp. F), et le th. des bipolaires (II, p. 49) entraîne donc N = {0} et I = F, donc u est bijectif. On a donc prouvé que u est un isomorphisme.

### 3. Critères de surjectivité

#### Proposition 4 {#evt-iv-s4-prop-4 .statement}

Soient E et F deux espaces de Fréchet, et u une application linéaire continue de E dans F. Les conditions suivantes sont équivalentes :

(i) u est surjective.
(ii) Pour toute semi-norme $p \in S(E)$, il existe $q \in S(F)$ telle que l’on ait $|f| \leq q$ pour toute forme linéaire $f \in F'$ satisfaisant à $|f \circ u| \leq p$.
(iii) Pour toute semi-norme $p \in S(E)$, il existe $q \in S(F)$ ayant la propriété suivante : si une forme linéaire $f \in F'$ satisfait à $|f \circ u| \leq p$, alors f s’annule aux points où q s’annule et pour $y \in F$, $r \in S(F)$, il existe $x \in E$ avec $r(u(x) - y) = 0$.
(iv) Pour toute semi-norme $p \in S(E)$, on a

(1)
$$
\sup_{\substack{f \in F' \\ |f \circ u| \leq p}} |f(y)| < + \infty \quad \text{pour tout } y \in F .
$$

Nous ferons la démonstration selon le schéma logique

(i)   (ii)   (iii)   (iv)

Si $u$ est surjective, c’est un morphisme strict (IV, p. 28, th. 1); il existe donc, pour toute semi-norme $p \in S(E)$, une semi-norme $q \in S(F)$ telle que, pour tout $y \in F$ vérifiant $q(y) \leq 1$, il existe $x \in E$ vérifiant $p(x) \leq 1$ et $u(x) = y$. On en déduit aussitôt que (i) entraîne (ii) et (iii). Il est clair que (ii) entraîne (iv).

Montrons que (iii) entraîne (iv). Soient $p$ et $q$ comme dans (iii). Soit $y$ dans $F$; d’après (iii), il existe $x$ dans $E$ tel que $q(u(x) - y) = 0$. Si $f \in F'$ satisfait à $|f \circ u| \leq p$, alors on a $f(u(x) - y) = 0$, d’où

$$
|f(y)| = |f(u(x))| \leq p(x)
$$

et la relation (1) est satisfaite.

Montrons enfin que (iv) entraîne (i). Soient $p \in S(E)$ et $q$ l’enveloppe supérieure des fonctions $|f|$ pour $f \in F'$ satisfaisant à $|f \circ u| \leq p$. D’après (iv), $q$ est fini sur $F$, et c’est évidemment une semi-norme semi-continue inférieurement sur $F$; comme $F$ est tonnelé (III, p. 25, corollaire), on a $q \in S(F)$. Notons $B_p$ (resp. $B_q$) l’ensemble des $x \in E$ (resp. $y \in F$) tels que $p(x) \leq 1$ (resp. $q(y) \leq 1$). On a $q \circ u \leq p$, d’où $u(B_p) \subset B_q$. Le polaire de $u(B_p)$ dans $F'$ se compose des formes linéaires $f \in F'$ telles que $|f \circ u| \leq p$, d’où $|f| \leq q$; autrement dit, on a $u(B_p)^{\circ} \subset B_q^{\circ}$, d’où finalement $\overline{u(B_p)} = B_q$ d’après le th. des bipolaires (II, p. 49, cor. 3). Si $U$ est un voisinage de 0 dans $E$, il existe $p \in S(E)$ telle que $B_p \subset U$, donc $u(U)$ contient le voisinage $B_q$ de 0 dans $F$. Ceci entraîne que $u$ est surjective (I, p. 17, th. 1).

#### Corollaire {#evt-iv-s4-n3-cor-1 .statement}

*Supposons que E et F soient des espaces de Banach. Les conditions suivantes sont équivalentes* :

(i) *u est surjective*.
(ii) *Il existe un nombre réel r > 0 tel que l’on ait \|f\| \leq r.\|u(f)\| pour tout f \in F'*.
(iii) *Pour tout y \in F, on a \sup_{\substack{f \in F' \\ \|f \circ u\| \leq 1}} |f(y)| < + \infty*.

En effet, les conditions (ii) et (iii) ne sont autres que les formulations, pour les espaces de Banach, des conditions (ii) et (iv) de la prop. 4.

## EXERCICES {#evt-iv-s4-exercises}

See the [exercises for § 4](exercises/s4/).
