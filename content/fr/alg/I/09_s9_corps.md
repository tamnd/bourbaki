---
book: alg
book_title: Algebra
chapter: I
chapter_title: STRUCTURES ALGÉBRIQUES
section: 9
section_title: Corps
lang: fr
source: alg-i-iii-fr
book_pages: A I.153-A I.157
pdf_pages: 0118-0122, 0163-0167
extraction: ocr
subsections:
    - "no": 1
      title: Corps
      page: 108
      pdf_page: 118
    - "no": 2
      title: Anneaux intègres
      page: 110
      pdf_page: 120
    - "no": 3
      title: Idéaux premiers
      page: 111
      pdf_page: 121
    - "no": 4
      title: Le corps des nombres rationnels
      page: 111
      pdf_page: 121
statements: 19
exercises: 21
content_sha256: aa763e5c5e122e0d1bb887dc16f744bf1f662066917ba969fce719596e5f648a
---

## § 9. CORPS

### 1. Corps

#### Définition 1 {#alg-i-s9-def-1 .statement}

On dit qu’un anneau K est un corps s’il n’est pas réduit à 0 et si tout élément non nul de K est inversible.

L’ensemble des éléments non nuls du corps K, muni de la multiplication, est un groupe, qui n’est autre que le groupe multiplicatif $K^*$ de l’anneau K (I, p. 93). L’anneau opposé d’un corps est un corps. On dit qu’un corps est commutatif si sa multiplication est commutative; un tel corps est identique à son opposé. Un corps non commutatif est parfois appelé corps gauche.

#### Exemple 1 {#alg-i-s9-n1-exa-1 .statement}

Nous définirons au n° 4 le corps des nombres rationnels; on définira en Topologie Générale le corps des nombres réels (TG, IV, § 1, n° 3), celui des nombres complexes (TG, VIII, § 1, n° 1) et celui des quaternions (TG, VIII, § 1, n° 4). Ces corps sont commutatifs, à l’exception du corps des quaternions.*

#### Exemple 2 {#alg-i-s9-n1-exa-2 .statement}

L’anneau $\mathbf{Z}/2\mathbf{Z}$ est évidemment un corps.

Soit K un corps. On appelle sous-corps de K tout sous-anneau L de K qui est un corps et on dit alors que K est un surcorps de L; il revient au même de dire que L est un sous-anneau de K et que l’on a $x^{-1} \in L$ pour tout élément non nul x de L. Si $(L_i)_{i \in I}$ est une famille de sous-corps de K, alors $\bigcap_{i=1}^n L_i$ est un sous-corps de K; pour toute partie X de K, il existe donc un plus petit sous-corps de K contenant X; on dit qu’il est engendré par X.

#### Proposition 1 {#alg-i-s9-prop-1 .statement}

Soit K un corps. Pour toute partie X de K, le commutant (I, p. 98, Exemple 3) X' de X est un sous-corps de K.

On sait (loc. cit.) que X' est un sous-anneau de K. D’autre part, si x ≠ 0 est permutable avec z ∈ X, il en est de même de x^{-1} (I, p. 16, prop. 5), donc X' contient l’inverse de tout élément non nul de X'.

#### Corollaire {#alg-i-s9-n1-cor-1 .statement}

Le centre d’un corps K est un sous-corps (commutatif) de K.

#### Théorème 1 {#alg-i-s9-thm-1 .statement}

Soit A un anneau. Les conditions suivantes sont équivalentes:
a) A est un corps;
b) A est non réduit à 0, et les seuls idéaux à gauche de A sont 0 et A.

Supposons que A soit un corps. Alors A est non réduit à 0. Soit a un idéal à gauche de A distinct de 0. Il existe un a non nul appartenant à a. Pour tout x ∈ A, on a x = (xa^{-1})a ∈ a; donc a = A.

Supposons que A vérifie la condition b). Soit x ≠ 0 dans A. Il s’agit de prouver que x est inversible. L’idéal à gauche Ax contient x donc n’est pas nul, d’où Ax = A. Il existe donc x' ∈ A tel que x'x = 1. On a x' ≠ 0 puisque 1 ≠ 0. Appliquons le résultat précédent à x'; on voit qu’il existe x'' ∈ A tel que x''x' = 1. On a x'' = x''. 1 = x''x'x = 1.x = x, donc xx' = 1. Finalement, x' est inverse de x.

#### Remarque {#alg-i-s9-n1-rem-1 .statement}

On peut, dans le th. 1, remplacer les idéaux à gauche par les idéaux à droite. Au chap. VIII, § 5, no 2, nous étudierons des anneaux non nuls A qui n’ont aucun idéal bilatère distinct de 0 et A; de tels anneaux (dits quasi-simples) ne sont pas nécessairement des corps *(par exemple, l’anneau M_2(\mathbf{Q}) des matrices carrées d’ordre 2 à coefficients rationnels est quasi-simple mais n’est pas un corps)*.

#### Corollaire 1 {#alg-i-s9-thm-1-cor-1 .statement}

Soient A un anneau et a un idéal bilatère de A. Pour que l’anneau A/a soit un corps, il faut et il suffit que a soit un idéal à gauche maximal de A.

Les idéaux à gauche de A/a sont de la forme b/a où b est un idéal à gauche de A contenant a (I, p. 102, corollaire). Dire que A/a ≠ {0} signifie que a ≠ A. Sous cette hypothèse, A/a est un corps si et seulement si les seuls idéaux à gauche de A contenant a sont a et A (th. 1), d’où le corollaire.

#### Corollaire 2 {#alg-i-s9-thm-1-cor-2 .statement}

Soit A un anneau commutatif non réduit à 0. Il existe un homomorphisme de A sur un corps commutatif.

D’après le th. de Krull (I, p. 99, th. 1), il existe dans A un idéal maximal a. Alors A/a est un corps (cor. 1).

#### Corollaire 3 {#alg-i-s9-thm-1-cor-3 .statement}

Soit a un entier ≥ 0. Pour que l’anneau \mathbf{Z}/a\mathbf{Z} soit un corps, il faut et il suffit que a soit premier.

Cela résulte du cor. 1, et de I, p. 106.

Pour p premier, le corps \mathbf{Z}/p\mathbf{Z} se note \mathbf{F}_p.

#### Théorème 2 {#alg-i-s9-thm-2 .statement}

Soient $K$ un corps et $A$ un anneau non réduit à 0. Si $f$ est un homomorphisme de $K$ dans $A$, alors le sous-anneau $f(K)$ de $A$ est un corps et $f$ définit un isomorphisme de $K$ sur $f(K)$.

Soit $\alpha$ le noyau de $f$. On a $1 \notin \alpha$ car $f(1) = 1 \neq 0$ dans $A$, et comme $\alpha$ est un idéal à gauche de $K$, on a $\alpha = \{0\}$ d’après le th. 1. Par suite, $f$ est injective, donc un isomorphisme de $K$ sur le sous-anneau $f(K)$ de $A$; ce dernier anneau est donc un corps.

### 2. Anneaux intègres

#### Définition 2 {#alg-i-s9-def-2 .statement}

On dit qu’un anneau $A$ est intégre (ou que $A$ est un anneau d’intégrité) s’il est commutatif, non réduit à 0, et si le produit de deux éléments non nuls de $A$ est non nul.

L’anneau $\mathbf{Z}$ des entiers rationnels est intégre: il est commutatif, non réduit à 0; le produit de deux entiers $> 0$ est non nul; tout entier non nul est de la forme $a$ ou $-a$ avec $a > 0$, et l’on a $(-a)b = -ab, (-a)(-b) = ab$ pour $a > 0, b > 0$, d’où notre assertion.

Tout corps commutatif est un anneau intégre. Un sous-anneau d’un anneau intégre est intégre. En particulier, un sous-anneau d’un corps commutatif est intégre. Nous allons montrer que réciproquement tout anneau intégre $A$ est isomorphe à un sous-anneau d’un corps commutatif. Rappelons (I, p. 108) que l’on a identifié $A$ à un sous-anneau de son anneau total des fractions. Notre assertion résulte alors de la proposition suivante:

#### Proposition 2 {#alg-i-s9-prop-2 .statement}

Si $A$ est un anneau intégre, l’anneau total des fractions $K$ de $A$ est un corps commutatif.

L’anneau $K$ est commutatif. Il est non réduit à 0 puisque $A \neq \{0\}$. Comme $A$ est intégre, tout élément non nul de $A$ est simplifiable, et $K$ se compose des fractions $a/b$ avec $b \neq 0$. Or $a/b \neq 0$ entraîne $a \neq 0$, et la fraction $b/a$ est alors inverse de $a/b$.

L’anneau total des fractions d’un anneau intégre s’appelle son corps des fractions. On identifie un tel anneau à son image dans son corps des fractions.

#### Proposition 3 {#alg-i-s9-prop-3 .statement}

Soient $B$ un anneau non réduit à 0, $A$ un sous-anneau commutatif de $B$ tel que tout élément non nul de $A$ soit inversible dans $B$.

a) $A$ est intégre.

b) Soit $A'$ le corps des fractions de $A$. L’injection canonique de $A$ dans $B$ se prolonge de manière unique en un isomorphisme $f$ de $A'$ sur un sous-corps de $B$.

c) Les éléments de $f(A')$ sont les $xy^{-1}$ où $x \in A, y \in A, y \neq 0$.

L’assertion a) est évidente. L’injection canonique de $A$ dans $B$ se prolonge de manière unique en un homomorphisme $f$ de $A'$ dans $B$ (I, p. 108, th. 5). L’assertion b) résulte alors du th. 2. Les éléments de $A'$ sont les fractions $x/y$ avec $x \in A, y \in A, y \neq 0$, et $f(x/y) = xy^{-1}$, d’où c).

### 3. Idéaux premiers

#### Proposition 4 {#alg-i-s9-prop-4 .statement}

Soient $A$ un anneau commutatif, $p$ un idéal de $A$. Les conditions suivantes sont équivalentes :
a) l’anneau $A/p$ est intègre ;
b) $A \neq p$, et, si $x \in A - p$ et $y \in A - p$, on a $xy \in A - p$;
c) $p$ est le noyau d’un homomorphisme de $A$ dans un corps.
Les implications c) $\Rightarrow$ b) $\Rightarrow$ a) sont évidentes. Si $A/p$ est intègre, soient $f$ l’injection canonique de $A/p$ dans son corps des fractions et $g$ l’homomorphisme canonique de $A$ sur $A/p$; alors $p$ est le noyau de $f \circ g$, d’où l’implication a) $\Rightarrow$ c).

#### Définition 3 {#alg-i-s9-def-3 .statement}

Dans un anneau commutatif $A$, on appelle idéal premier un idéal $p$ vérifiant les conditions de la prop. 4.

#### Exemple 1 {#alg-i-s9-n3-exa-1 .statement}

Soit $A$ un anneau commutatif. Si $m$ est un idéal maximal de $A$, $m$ est premier; en effet, l’anneau $A/m$ est un corps (I, p. 109, cor. 1).

#### Exemple 2 {#alg-i-s9-n3-exa-2 .statement}

Si $A$ est un anneau intègre, l’idéal $\{0\}$ de $A$ est premier (mais non maximal en général, comme le prouve l’exemple de l’anneau $\mathbf{Z}$).

### 4. Le corps des nombres rationnels

#### Définition 4 {#alg-i-s9-def-4 .statement}

On appelle corps des nombres rationnels, et l’on désigne par $\mathbf{Q}$, le corps des fractions de l’anneau $\mathbf{Z}$ des entiers rationnels. Les éléments de $\mathbf{Q}$ sont appelés nombres rationnels.

Tout nombre rationnel est donc une fraction de la forme $a/b$ où $a$ et $b$ sont des entiers rationnels avec $b \neq 0$ (et même $b > 0$ comme le prouve la relation $a/b = (-a)/(-b)$). On note $\mathbf{Q}_+$ l’ensemble des nombres rationnels de la forme $a/b$ avec $a \in \mathbf{N}$ et $b \in \mathbf{N}^*$.
On a les relations:

(1) $\mathbf{Q}_+ + \mathbf{Q}_+ = \mathbf{Q}_+$
(2) $\mathbf{Q}_+ \cdot \mathbf{Q}_+ = \mathbf{Q}_+$
(3) $\mathbf{Q}_+ \cap (-\mathbf{Q}_+) = \{0\}$
(4) $\mathbf{Q}_+ \cup (-\mathbf{Q}_+) = \mathbf{Q}$
(5) $\mathbf{Q}_+ \cap \mathbf{Z} = \mathbf{N}$.

Les deux premières résultent des formules $a/b + a'/b' = (ab' + ba')/bb'$, $(a/b)(a'/b') = aa'/bb'$, $0 \in \mathbf{Q}_+$, $1 \in \mathbf{Q}_+$, et de ce que $\mathbf{N}$ est stable par addition et multiplication et $\mathbf{N}^*$ stable par multiplication. Comme $0 \in \mathbf{Q}_+$, on a $0 \in (-\mathbf{Q}_+)$; soit $x$ dans $\mathbf{Q}_+ \cap (-\mathbf{Q}_+)$; il existe donc des entiers positifs $a, b, a', b'$ avec $b \neq 0$, $b' \neq 0$ et $x = a/b = -a'/b'$; on en déduit $ab' + ba' = 0$ d’où $ab' = 0$ (car $ab' \geqslant 0$ et $ba' \geqslant 0$), donc $a = 0$ car $b' \neq 0$; autrement dit, on a $x = 0$. Enfin, on a évidemment $\mathbf{N} \subset \mathbf{Z}$ et $\mathbf{N} \subset \mathbf{Q}_+$. Inversement, si $x$ appartient à $\mathbf{Z} \cap \mathbf{Q}_+$, c’est un entier rationnel; il existe deux entiers rationnels $a$ et $b$ tels que $a \geqslant 0,\ b > 0$ et $x = a/b$ d’où $a = bx$; si l’on avait $x \notin \mathbf{N}$, on aurait $-x > 0$ d’où $-a = b(-x) > 0$ et par conséquent $a < 0$ contrairement à l’hypothèse.

Etant donnés deux nombres rationnels $x$ et $y$, on écrit $x \leqslant y$ si l’on a $y - x \in \mathbf{Q}_+$. On déduit facilement des formules (1), (3) et (4) que $x \leqslant y$ est une relation d’ordre totale sur $\mathbf{Q}$, de (5) que cette relation induit la relation d’ordre usuelle sur $\mathbf{Z}$. Enfin de (1) on déduit que les relations $x \leqslant y$ et $x' \leqslant y'$ entraînent $x + x' \leqslant y + y'$ et de (2) que la relation $x \leqslant y$ entraîne $xz \leqslant yz$ pour tout $z \geqslant 0$ et $xz \geqslant yz$ pour $z \leqslant 0$ (cf. VI, § 2, n° 1).

Soit $x$ un nombre rationnel. On dit que $x$ est *positif* si $x \geqslant 0$, *strictement positif* si $x > 0$, *négatif* si $x \leqslant 0$ et *strictement négatif* si $x < 0$.\footnote{Nous nous écartons de la terminologie courante, où positif signifie $> 0$.} L’ensemble des nombres rationnels positifs est $\mathbf{Q}_+$ et celui des nombres négatifs est $-\mathbf{Q}_+$. Si l’on note $\mathbf{Q}^*$ l’ensemble des nombres rationnels non nuls, l’ensemble $\mathbf{Q}_+^*$ des nombres strictement positifs est égal à $\mathbf{Q}^* \cap \mathbf{Q}_+$ et $-\mathbf{Q}_+^*$ est l’ensemble des nombres strictement négatifs.

Les ensembles $\mathbf{Q}_+^*$ et $\{1, -1\}$ sont des sous-groupes du groupe multiplicatif $\mathbf{Q}^*$. Tout nombre rationnel $x \neq 0$ se met d’une manière et d’une seule sous l’une des formes $1.y,\ (-1).y$, où $y > 0$; donc le groupe multiplicatif $\mathbf{Q}^*$ est produit des sous-groupes $\mathbf{Q}_+^*$ et $\{1, -1\}$; le composant de $x$ dans $\mathbf{Q}_+^*$ s’appelle la *valeur absolue* de $x$, et se note $|x|$; le composant de $x$ dans $\{-1, 1\}$ (égal à 1 si $x > 0$, à $-1$ si $x < 0$) s’appelle *signe* de $x$, et se note $\operatorname{sgn}\, x$.

On prolonge d’ordinaire ces deux fonctions à $\mathbf{Q}$ tout entier en posant $|0| = 0$, et $\operatorname{sgn}\, 0 = 0$.

## EXERCICES {#alg-i-s9-exercises}

See the [exercises for § 9](exercises/s9/).
