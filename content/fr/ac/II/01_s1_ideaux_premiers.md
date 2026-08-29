---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: Localisation
section: 1
section_title: Idéaux premiers
lang: fr
source: ac-i-iv-fr
pdf_pages: 0067-0072, 0150-0152
extraction: ocr
subsections:
    - "no": 1
      title: Définition des idéaux premiers.
      page: 0
      pdf_page: 67
    - "no": 2
      title: Idéaux étrangers.
      page: 0
      pdf_page: 69
statements: 9
exercises: 11
content_sha256: 3f5986b3b0b9fc5bf46e08c855d7c25a7cdd2ae8e0bfc096ae2ca1109fc46ebc
---

## § 1. Idéaux premiers

### 1. Définition des idéaux premiers.

#### Définition 1 {#ac-ii-s1-def-1 .statement}

On dit qu’un idéal p d’un anneau A est premier si l’anneau A/p est intègre.

D’après cette définition, un idéal p d’un anneau A est premier si les deux conditions suivantes sont vérifiées :

1° p ≠ A ;
2° si x, y sont deux éléments de A tels que x ∈ p et y ∈ p, on a xy ∈ p.

Ces conditions peuvent encore s’exprimer en disant que le produit de toute famille finie d’éléments de C_p appartient à C_p, car en appliquant cette condition à la famille vide, cela implique que 1 ∈ p.

(*) A l’exception des énoncés placés entre deux astérisques : *...,*, les résultats de ce chapitre ne dépendent d’aucun autre Livre de la deuxième partie, ni du § 4 du chap. I.

Un idéal maximal $m$ de $A$ est premier, puisque $A/m$ est un corps ; il résulte donc du th. de Krull (Alg., chap. I, § 8, n° 7, th. 2) que tout idéal de $A$ distinct de $A$ est contenu dans un idéal premier au moins. En particulier, pour qu’il existe des idéaux premiers dans un anneau $A$, il faut et il suffit que $A$ ne soit pas réduit à 0.

Soit $f : A \to B$ un homomorphisme d’anneaux, et soit $q$ un idéal de $B$. Posons $p = \overline{f}(q)$; l’homomorphisme $\bar{f} : A/p \to B/q$ déduit de $f$ par passage aux quotients est injectif. Supposons $q$ premier ; comme l’anneau $B/q$ est intègre, il en est de même de $A/p$ qui est isomorphe à un sous-anneau de $B/q$; par conséquent l’idéal $p = \overline{f}(q)$ est premier. En particulier, soit $A$ un sous-anneau de $B$; pour tout idéal premier $q$ de $B$, $q \cap A$ est un idéal premier de $A$. Si $f$ est surjectif, $\bar{f}$ est un isomorphisme; les conditions «$p$ est premier » et «$q$ est premier » sont alors équivalentes. Donc, si $p$ et $a$ sont des idéaux de $A$ tels que $a \subset p$, une condition nécessaire et suffisante pour que $p$ soit premier est que $p/a$ soit premier dans $A/a$.

#### Proposition 1 {#ac-ii-s1-prop-1 .statement}

*Soient $A$ un anneau, $a_1, a_2, ..., a_n$ des idéaux de $A$, $p$ un idéal premier de $A$. Si $p$ contient le produit $a_1 a_2 ... a_n$, il contient l’un au moins des $a_i$.*

Supposons en effet que $p$ ne contienne aucun des $a_i$. Pour $1 \leq i \leq n$, il existe donc un élément $s_i \in a_i \cap \mathbf{C}p$; alors $s = s_1 s_2 ... s_n$ est contenu dans $a_1 a_2 ... a_n$ et n’est pas contenu dans $p$, ce qui est absurde.

#### Corollaire {#ac-ii-s1-n1-cor-1 .statement}

*Soit $m$ un idéal maximal de $A$; pour tout entier $n > 0$, le seul idéal premier contenant $m^n$ est $m$.*

En effet, un tel idéal $p$ doit contenir $m$ en vertu de la prop. 1 appliquée à $a_i = m$ pour $1 \leq i \leq n$; comme $m$ est maximal, on a $p = m$.

#### Proposition 2 {#ac-ii-s1-prop-2 .statement}

*Soient $A$ un anneau, $a$ un sous-ensemble non vide de $A$ stable par addition et multiplication, et $(p_i)_{i \in I}$ une famille finie non vide d’idéaux de $A$. On suppose que $a$ est contenu dans la réunion des $p_i$ et qu’il y a au plus deux des $p_i$ qui ne sont pas premiers. Alors $a$ est contenu dans un des $p_i$.*

Raisonnons par récurrence sur $n = \mathrm{Card} (I)$; la proposition est triviale si $n = 1$. Supposons $n \geqslant 2$; s’il existe un indice $j$ tel que $a \cap p_j \subset \bigcup_{i \neq j} p_i$, l’ensemble $a$, qui est la réunion des $a \cap p_i$ pour $i \in I$, est contenu dans $\bigcup_{i \neq j} p_i$, donc dans l’un des $p_i$ en vertu de l’hypothèse de récurrence. Supposons donc qu’il n’en soit pas ainsi ; pour tout $j \in I$, soit $y_j$ un élément de $a \cap p_j$ n’appartenant à aucun des $p_i$ tels que $i \neq j$. Soit $k$ un élément de $I$ choisi de telle manière que $p_k$ soit premier si $n > 2$, et choisi arbitrairement si $n = 2$; soit $z = y_k + \prod_{i \neq k} y_i$. On a $z \in a$, puisque $a$ est stable pour l’addition et la multiplication ; si $j \neq k$, $\prod_{i \neq k} y_i$ appartient à $p_j$, mais $y_k \notin p_j$, d’où $z \notin p_j$. D’autre part, $\prod_{i \neq k} y_i$ n’appartient pas à $p_k$, car aucun des facteurs $y_i$ ($i \neq k$) ne lui appartient, et $p_k$ est premier si $n - 1 > 1$; comme $y_k \in p_k$, $z$ n’appartient pas à $p_k$, et la proposition est établie.

### 2. Idéaux étrangers.

Soit $A$ un anneau ; on dit que deux idéaux $a, b$ de $A$ sont étrangers si $a + b = A$. Pour qu’il en soit ainsi, il faut et il suffit que $a + b$ ne soit contenu dans aucun idéal premier ($Alg.$, chap. I, § 8, no 7, th. 2), autrement dit qu’aucun idéal premier ne contienne à la fois $a$ et $b$. Deux idéaux maximaux distincts sont étrangers.

Lorsque $A$ est un anneau principal ($Alg.$, chap. VII, § 1), pour que deux éléments $a, b$ de $A$ soient étrangers, il faut et il suffit, en vertu de l’identité de Bezout ($loc. cit.$, no 2, th. 1), que les idéaux $Aa$ et $Ab$ soient étrangers.

#### Proposition 3 {#ac-ii-s1-prop-3 .statement}

Soient $a$ et $b$ deux idéaux étrangers d’un anneau $A$. Soient $a'$ et $b'$ deux idéaux de $A$ tels que tout élément de $a$ (resp. $b$) ait une puissance dans $a'$ (resp. $b'$). Alors $a'$ et $b'$ sont étrangers.

Vu l’hypothèse faite, tout idéal premier qui contient $a'$ contient $a$ et tout idéal premier qui contient $b'$ contient $b$. Si un idéal premier contient $a'$ et $b'$, il contient donc $a$ et $b$, ce qui est absurde puisque $a$ et $b$ sont étrangers ; donc $a'$ et $b'$ sont étrangers.

#### Proposition 4 {#ac-ii-s1-prop-4 .statement}

*Soient $a, b_1, ..., b_n$ des idéaux d’un anneau $A$. Si $a$ est étranger à chacun des $b_i$ ($1 \leq i \leq n$), il est étranger à $b_1 b_2 ... b_n$.

Soit $p$ un idéal premier de $A$. Si $p$ contient $a$ et $b_1 b_2 ... b_n$, il contient un des $b_i$ (no 1, prop. 1), ce qui est absurde puisque $a$ et $b_i$ sont étrangers.*

#### Proposition 5 {#ac-ii-s1-prop-5 .statement}

*Soit $(a_i)_{i \in I}$ une famille finie non vide d’idéaux d’un anneau $A$. Les propriétés suivantes sont équivalentes :
a) Pour $i \neq j$, $a_i$ et $a_j$ sont étrangers.
b) L’homomorphisme canonique $\varphi : A \to \prod_{i \in I} (A/a_i)$ (Alg., chap. II, 3e éd., § 1, no 7) est surjectif.
Lorsqu’il en est ainsi, l’intersection $a$ des $a_i$ est égale à leur produit, et l’homomorphisme canonique $\psi : A/a \to \prod_{i \in I} (A/a_i)$ (Alg., chap. II, 3e éd., § 1, no 7) est bijectif.

Raisonnons par récurrence sur le nombre $n$ d’éléments de $I$, le cas $n = 1$ étant trivial. Considérons d’abord le cas $n = 2$. L’équivalence de a) et b) résulte alors de l’exactitude de la suite

$$0 \to A/(a_1 \cap a_2) \xrightarrow{\psi} (A/a_1) \oplus (A/a_2) \to A/(a_1 + a_2) \to 0$$

*(Alg., chap. II, 3e éd., § 1, no 7, formule (30)). En outre, il existe $e_1 \in a_1$ et $e_2 \in a_2$ tels que $1 = e_1 + e_2$; pour tout $x \in a = a_1 \cap a_2$, on a donc $x = x e_1 + x e_2$; mais par définition on a $x e_1 \in a_1 a_2$ et $x e_2 \in a_1 a_2$, donc $x \in a_1 a_2$; d’où $a \subset a_1 a_2$, et l’inclusion opposée est évidente.

Passons au cas général. Supposons la condition a) satisfaite et soient $k$ un élément de $I$, $b_k = \bigcap_{i \neq k} a_i$; l’hypothèse de récurrence entraîne que $b_k = \prod_{i \neq k} a_i$, et il résulte de la prop. 4 que $a_k$ et $b_k$ sont étrangers; donc $a = \bigcap_{i \in I} a_i = a_k \cap b_k = a_k b_k = \prod_{i \in I} a_i$ par la première partie du raisonnement, et pour la même raison l’homomorphisme canonique $A/a \to (A/a_k) \times (A/b_k)$ est bijectif ; par l’hypothèse de récurrence l’homomorphisme canonique $A/b_k \to \prod_{i \neq k} (A/a_i)$ est bijectif, et il en est donc de même de l’homomorphisme composé

$$
A/a \to (A/a_k) \times (A/b_k) \to (A/a_k) \times \prod_{i \neq k} (A/a_i) = \prod_{i \in I} (A/a_i)
$$

qui n’est autre que $\psi$, ce qui démontre $b$). Inversement, supposons $b$) vérifiée et montrons que les $a_i$ sont nécessairement étrangers deux à deux. Dans le cas contraire, il existerait un idéal $c \neq A$ contenant $a_i$ et $a_j$ pour $i \neq j$. Posons $a'_h = a_h$ pour $h$ distinct de $i$ et de $j$, et $a'_i = a'_j = c$; l’homomorphisme canonique $\varphi' : A \to \prod_{i \in I} (A/a'_i)$ peut s’écrire comme le composé

$$
A \xrightarrow{\varphi} \prod_{i \in I} (A/a_i) \xrightarrow{f} \prod_{i \in I} (A/a'_i)
$$

$f$ étant le produit des homomorphismes canoniques $A/a_i \to A/a'_i$; il est clair que $\varphi'$ n’est pas surjectif, la projection de $\varphi'(A)$ sur $(A/a'_i) \times (A/a'_i)$ étant la diagonale du produit $(A/c) \times (A/c)$, qui est distincte de ce produit puisque $c \neq A$. Comme $f$ est surjectif, cela montre que $\varphi$ n’est pas surjectif.

C. Q. F. D.

#### Proposition 6 {#ac-ii-s1-prop-6 .statement}

*Soit* $(a_i)_{i \in I}$ *une famille finie non vide d’idéaux d’un anneau* $A$, *étrangers deux à deux* ; *soit* $a$ *l’intersection des* $a_i$. *Pour tout* $A$*-module* $M$, *l’application canonique* $M \to \prod_{i \in I} (M/a_iM)$ *est surjective*, *et son noyau est* $aM$.

Il est clair que l’application canonique de $M$ dans $\prod_{i \in I} (M/a_iM)$ s’annule dans $aM$; elle définit donc par passage au quotient un homomorphisme $\lambda : M/aM \to \prod_{i \in I} (M/a_iM)$. D’autre part, d’après la prop. 5, l’homomorphisme canonique $\psi : A/a \to \prod_{i \in I} (A/a_i)$ est bijectif. Il en est donc de même de $1_M \otimes \psi : M \otimes (A/a) \to M \otimes \prod_{i \in I} (A/a_i)$. Or $M \otimes (A/a)$ s’identifie à $M/aM$, et $M \otimes \prod_{i \in I} (A/a_i)$ s’identifie à $\prod_{i \in I} M \otimes (A/a_i)$, qui s’identifie lui-même à $\prod_{i \in I} (M/a_iM)$. On vérifie immédiatement que les identifications précédentes transforment $1_M \otimes \psi$ en $\lambda$, d’où la proposition.

#### Exemple {#ac-ii-s1-n2-exa-1 .statement}

Soient K un corps, $a_i (1 \leq i \leq m)$ des éléments deux à deux distincts de K, et pour chaque $i$, soit $g_i$ un polynôme dans $K[X]$; l’idéal principal $(X - a_i) = m_i$ est maximal dans $K[X]$, donc pour tout système $(n_i)_{1 \leq i \leq m}$ de m entiers $\geq 1$, les idéaux $m_i^{n_i}$ sont deux à deux étrangers. On déduit donc de la prop. 5 qu’il existe un polynôme $f \in K[X]$ tel que l’on ait $f(X) \equiv g_i(X)$ (mod. $(X - a_i)^{n_i}$) pour $1 \leq i \leq m$, la différence de deux tels polynômes étant divisible par $\omega(X) = \prod_{i=1}^m (X - a_i)^{n_i}$. Lorsqu’on prend tous les $n_i$ égaux à 1, on retrouve le problème résolu explicitement par la formule d’interpolation de Lagrange (Alg., chap. IV, § 2, no 4).

## EXERCICES {#ac-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
