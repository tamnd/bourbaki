---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: Valuations
section: 4
section_title: Hauteur d’une valuation
lang: fr
source: ac-v-vii-fr
pdf_pages: 0106-0113, 0171-0176
extraction: ocr
subsections:
    - "no": 1
      title: Inclusion des anneaux de valuation d’un même corps
      page: 0
      pdf_page: 106
    - "no": 2
      title: Sous-groupes isolés d’un groupe ordonné
      page: 0
      pdf_page: 108
    - "no": 3
      title: Comparaison des valuations
      page: 0
      pdf_page: 109
    - "no": 4
      title: Hauteur d’une valuation
      page: 0
      pdf_page: 110
    - "no": 5
      title: Valuations de hauteur 1
      page: 0
      pdf_page: 111
statements: 21
exercises: 5
content_sha256: b183165ffbef744b18bb24fd033dc8b81bbf2f8dd70c28bdec14b9f83e6eb755
---

## § 4. Hauteur d’une valuation.

### 1. Inclusion des anneaux de valuation d’un même corps

#### Proposition 1 {#ac-vi-s4-prop-1 .statement}

Soient $\mathbf{K}$ un corps, et $\mathbf{A}$ un anneau de valuation pour $\mathbf{K}$. Alors:
a) Tout anneau $\mathbf{B}$ tel que $\mathbf{A} \subset \mathbf{B} \subset \mathbf{K}$ est un anneau de valuation pour $\mathbf{K}$;
b) L’idéal maximal $m(\mathbf{B})$ d’un tel anneau est contenu dans $\mathbf{A}$, et c’est un idéal premier de $\mathbf{A}$;
c) L’application $\mathfrak{p} \to \mathbf{A}_{\mathfrak{p}}$ est une bijection décroissante de l’ensemble des idéaux premiers de $\mathbf{A}$ sur l’ensemble des anneaux $\mathbf{B}$ tels que $\mathbf{A} \subset \mathbf{B} \subset \mathbf{K}$; sa bijection réciproque est l’application $\mathbf{B} \to m(\mathbf{B})$.

Si $\mathbf{B}$ est un anneau tel que $\mathbf{A} \subset \mathbf{B} \subset \mathbf{K}$, et si $x \in \mathbf{K} - \mathbf{B}$,

#### Corollaire {#ac-vi-s4-n1-cor-1 .statement}

*L’ensemble des sous-anneaux de* $K$ *contenant* $A$ *est totalement ordonné par inclusion*.

En effet, l’ensemble des idéaux premiers de $A$ est totalement ordonné par inclusion ($§ 1$, no 2, th. 1 e)), et l’application $\mathfrak{p} \to A_{\mathfrak{p}}$ renverse les relations d’inclusion.

#### Proposition 2 {#ac-vi-s4-prop-2 .statement}

*Soient* $K$ *un corps*, $B$ *un anneau de valuation pour* $K$, *et* $h_B$ *la place de* $K$ *associée à* $B$ *(à valeurs dans* $\kappa(B)$). *Alors l’application* $A \to h_B(A)$ *définit une bijection de l’ensemble* $\mathcal{A}$ *des anneaux de valuation pour* $K$ *contenus dans* $B$, *sur l’ensemble* $\mathcal{A}'$ *des anneaux de valuation pour* $\kappa(B)$.

Si $A \in \mathcal{A}$, on a $h_B(A) \in \mathcal{A}'$: en effet, si $x' = h_B(x)$ (où $x \in B$) est un élément de $\kappa(B) - h_B(A)$, on a $x \notin A$, donc $x^{-1} \in A$ et $h_B(x)^{-1} \in h_B(A)$. D’autre part, pour $A \in \mathcal{A}$, on a $A \supset m(B)$ (prop. 1, $b$)), donc l’application $A \to h_B(A)$ est injective. Enfin, soient $A' \in \mathcal{A}'$ et $A = \overline{h_B}(A') \subset B$; on va montrer, ce qui achèvera la démonstration, que $A \in \mathcal{A}$; en effet, si $x \in K - A$, on a, soit $x \notin B$, soit $x \in B$; si $x \notin B$, on a $x^{-1} \in m(B) \subset A$; si $x \in B$, on a $h_B(x) \in \kappa(B)$ et $h_B(x) \notin A'$, donc $h_B(x^{-1}) \in A'$, et on en conclut encore que $x^{-1} \in A$; donc $A \in \mathcal{A}$.

#### Corollaire {#ac-vi-s4-n1-cor-2 .statement}

*Soient* $A$ *et* $B$ *deux anneaux de valuation pour* $K$, *avec* $A \subset B$; *posons* $A' = h_B(A)$, *qui est un anneau de valuation pour* $\kappa(B)$. *Le corps résiduel* $\kappa(A')$ *de* $A'$ *est canoniquement isomorphe au corps résiduel* $\kappa(A)$ *de* $A$, *et la place* $h_A$ *associée à* $A$ *est la composée* $h_{A'} \circ h_B$ *des places associées à* $A'$ *et* $B$.

En effet, puisque l’anneau local $A'$ est un quotient de l’anneau local $A$, leurs corps résiduels sont canoniquement isomorphes, et l’égalité $h_A(x) = h_{A'}(h_B(x))$ est vraie pour $x \in A$. D’autre part, si $x \in B - A$, on a $h_B(x) \notin A'$, et les deux membres de l’égalité sont égaux à $\infty$; il en est de même si $x \in K - B$.

#### Remarque {#ac-vi-s4-n1-rem-1 .statement}

Réciproquement, soient $f$ une place de $K$ à valeurs dans $K'$, et $f'$ une place de $K'$ à valeurs dans $K''$. Alors $f' \circ f$ est une place de $K$ dont l’anneau est contenu dans l’anneau de la place $f$.

### 2. Sous-groupes isolés d’un groupe ordonné

Pour étudier la situation du n° 1 du point de vue des valuations, nous aurons besoin de la déf. 1 et de la prop. 3 ci-dessous.

#### Définition 1 {#ac-vi-s4-def-1 .statement}

Un sous-groupe $H$ d’un groupe ordonné $G$ est dit isolé si les relations $0 \leq y \leq x$ et $x \in H$ entraînent $y \in H$.

#### Exemple 1 {#ac-vi-s4-n2-exa-1 .statement}

Soient $A$ et $B$ deux groupes ordonnés ; munissons $A \times B$ de l’ordre lexicographique (i.e. « $(a, b) \leq (a', b')$ » équivaut à « $(a < a')$ ou $(a = a'$ et $b \leq b'$) »). Le deuxième facteur $B$ de $A \times B$ est alors, comme on le voit aussitôt, un sous-groupe isolé de $A \times B$.

#### Proposition 3 {#ac-vi-s4-prop-3 .statement}

Soient $G$ un groupe ordonné, et $P$ l’ensemble de ses éléments positifs.

a) Le noyau d’un homomorphisme croissant de $G$ dans un groupe ordonné est un sous-groupe isolé de $G$.

b) Réciproquement, soient $H$ un sous-groupe isolé de $G$, et $g$ l’homomorphisme canonique de $G$ sur $G/H$. Alors $g(P)$ est l’ensemble des éléments positifs pour une structure de groupe ordonné sur $G/H$. En outre, si $G$ est totalement ordonné, il en est de même de $G/H$.

a) Soit $f$ un homomorphisme croissant de $G$ dans un groupe ordonné ; notons $H$ le noyau de $f$. Si $0 \leq y \leq x$ et $x \in H$, on a $0 \leq f(y) \leq f(x) = 0$, d’où $f(y) = 0$, c’est-à-dire $y \in H$. Donc $H$ est isolé.

b) Soient $H$ un sous-groupe isolé de $G$ et $g : G \to G/H$. Posons $P' = g(P)$. Il est clair que $P' + P' \subset P'$. On a

$$
P' \cap (-P') = \{0\},
$$

car, si $x$ et $y$ sont des éléments de $P$ tels que $g(x) = -g(y)$, on a $x + y \in H$, d’où $x \in H$ et $y \in H$ puisque $H$ est isolé ; donc $g(x) = g(y) = 0$. Ainsi $P'$ est l’ensemble des éléments positifs pour une structure de groupe ordonné sur $G/H$ (Alg. chap. VI, § 1, n° 3, prop. 3). Enfin, si $G$ est totalement ordonné, on a $P \cup (-P) = G$, d’où $P' \cup (-P') = G/H$, donc $G/H$ est totalement ordonné (*loc. cit.*).

#### Exemple 2 {#ac-vi-s4-n2-exa-2 .statement}

Si nous reprenons l’exemple où $G$ est un produit lexicographique $A \times B$ et où $H = B$, le groupe ordonné $G/H$ s’identifie canoniquement à $A$.

### 3. Comparaison des valuations

Soient $K$ un corps, et $A$ un anneau de valuation pour $K$. Pour tout sous-anneau $B$ de $K$ contenant $A$, on a $U(A) \subset U(B)$. On a donc un homomorphisme canonique $\lambda$ de $\Gamma_A = K^*/U(A)$ sur $\Gamma_B = K^*/U(B)$, dont le noyau est $U(B)/U(A)$. Notant $\varphi_A$ et $\varphi_B$ les valuations canoniques de $K$ définies par $A$ et $B$ (§ 3, no 2), on a donc

$$
\varphi_B = \lambda \circ \varphi_A.
$$

Comme $A \subset B$, $\lambda$ transforme les éléments positifs de $\Gamma_A$ en éléments positifs de $\Gamma_B$, donc est croissant. Par suite (prop. 3), le noyau $H_B$ de $\lambda$ est un sous-groupe isolé de $\Gamma_A$, et $\lambda$ se factorise en $\Gamma_A \to \Gamma_A/H_B \xrightarrow{\mu} \Gamma_B$, où $\mu$ est un homomorphisme bijectif et croissant, donc un *isomorphisme* de groupes totalement ordonnés; donc $\Gamma_B$ s’identifie au groupe totalement ordonné quotient $\Gamma_A/H_B$.

#### Proposition 4 {#ac-vi-s4-prop-4 .statement}

*L’application* $B \to H_B$ *est une bijection croissante de l’ensemble des sous-anneaux de K contenant A sur l’ensemble des sous-groupes isolés de $\Gamma_A$*.

En effet, la donnée de $H_B$ définit $\varphi_B$ à une équivalence près, donc détermine $B$ sans ambiguïté. D’autre part, soit $H$ un sous-groupe isolé de $\Gamma_A$; considérant $\Gamma_A/H$ comme un groupe totalement ordonné (prop. 3), l’application composée

$$
K^* \xrightarrow{\varphi_A} \Gamma_A \to \Gamma_A/H
$$

est une valuation de $K$ dont l’anneau contient $A$.

#### Remarque {#ac-vi-s4-n3-rem-1 .statement}

Avec les hypothèses précédentes, notons $f$ l’homomorphisme canonique de $B$ sur $\kappa(B)$, et posons $A' = f(A)$; c’est un anneau de valuation pour $\kappa(B)$ (prop. 2, no 1). On a $\overline{f(\kappa(B))^*} = U(B), \overline{f(A')} = A, \overline{f(m(A'))} = m(A)$, donc

$$
\overline{f(U(A'))} = U(A).
$$

Il en résulte un isomorphisme canonique de $U(B)/U(A)$ sur $\kappa(B)^*/U(A') = \Gamma_{A'}$. La suite exacte

$$
0 \to U(B)/U(A) \to \Gamma_A \to \Gamma_B \to 0
$$

donne donc une suite exacte

$$
0 \to \Gamma_{A'} \to \Gamma_A \to \Gamma_B \to 0.
$$

#### Exemple {#ac-vi-s4-n3-exa-1 .statement}

Soient $k$ un corps,

$$
E = k(X) \quad \text{et} \quad K = k(X, Y) = E(Y)
$$

$(X, Y$ indéterminées). Soit $B = E[Y]_{(Y)}$ l’anneau de valuation pour $K$ défini par l’élément extrémal $Y$ de l’anneau principal $E[Y]$ (§ 1, no 4, prop. 3). Le corps résiduel $\kappa(B)$ s’identifie canoniquement à $E[Y]/(Y) = E$. Soit, de même, $A' = k[X]_{(X)}$ l’anneau de valuation pour $E = k(X)$ défini par l’élément extrémal $X$ de $k[X]$. En désignant par $h_B$ la place de $E$ associée à $B$, et en posant $A = \overline{h_B}(A')$, on définit un anneau de valuation $A$ pour $K$ contenu dans $B$, et l’on a $\kappa(A) = \kappa(A') = k$. La place canonique $h_A : K \to k$ peut se décrire ainsi : si $f(X, Y)$ est un élément de $K$, on fait d’abord $Y = 0$ dans $f$ (ce qui donne un élément de $\widetilde{E} = k(X)$), puis $X = 0$ dans le résultat obtenu. Les groupes $\Gamma_{A'}$ et $\Gamma_B$ sont canoniquement isomorphes à $\mathbf{Z}$ (§ 3, no 4, Exemple 4).

*On montre sans difficulté (cf. § 10, no 2, lemme 2) que le groupe $\Gamma_A$ est isomorphe au produit lexicographique $\mathbf{Z} \times \mathbf{Z}$, et que la valuation $\varphi_A$ est équivalente à la valuation définie au § 3, no 4, fin de l’Exemple 6.*

### 4. Hauteur d’une valuation

Soit $G$ un groupe totalement ordonné. Étant donnés deux sous-groupes isolés $H$ et $H'$ de $G$, l’un d’eux est contenu dans l’autre : en effet, dans le cas contraire, il existerait un élément positif $x$ de $H$ n’appartenant pas à $H'$ et un élément positif $x'$ de $H'$ n’appartenant pas à $H$; soit, par exemple, $x \geqslant x'$; comme $H$ est isolé, on obtient $x' \in H$, d’où contradiction.

Ceci résulte aussi de la prop. 4 du no 3 et du cor. de la prop. 1 du no 1, en tenant compte du fait que tout groupe totalement ordonné est le groupe des ordres d’une valuation (§ 3, no 4, Exemple 6).

#### Définition 2 {#ac-vi-s4-def-2 .statement}

Soit G un groupe totalement ordonné. Si le nombre des sous-groupes isolés de G distincts de G est fini et égal à n, on dit que G est de hauteur n. Si ce nombre est infini, on dit que G est de hauteur infinie.

#### Exemple 1 {#ac-vi-s4-n4-exa-1 .statement}

La hauteur du groupe G = {0} est 0.
2) Les groupes $\mathbf{Z}$ et $\mathbf{R}$ sont de hauteur 1.
3) Soient G un groupe totalement ordonné et H un sous-groupe isolé de G. Si l’on désigne par $h(H)$ et $h(G/H)$ les hauteurs des groupes totalement ordonnés H et G/H, on a
$$
h(G) = h(H) + h(G/H),
$$
puisque l’ensemble des sous-groupes isolés de G est totalement ordonné par inclusion. En particulier, si G est le produit lexicographique de deux groupes totalement ordonnés H et H', on a
$$
h(G) = h(H) + h(H')
$$
(cf. no 2, Exemple 2); ainsi le produit lexicographique $\mathbf{Z} \times \mathbf{Z}$ est de hauteur 2.

Par contre la hauteur de $\mathbf{Z} \times \mathbf{Z}$, ordonné par plongement dans $\mathbf{R}$ (cf. § 3, no 4, fin de l’Exemple 6) est égale à 1 (cf. prop. 8 ci-dessous).

#### Définition 3 {#ac-vi-s4-def-3 .statement}

On appelle hauteur d’une valuation la hauteur du groupe des ordres de cette valuation.

Par exemple une valuation discrète est de hauteur 1. Seules les valuations impropres sont de hauteur 0. Les prop. 1 et 4 entraînent :

#### Proposition 5 {#ac-vi-s4-prop-5 .statement}

La hauteur d’une valuation est égale au nombre des idéaux premiers non nuls de son anneau.

### 5. Valuations de hauteur 1

#### Proposition 6 {#ac-vi-s4-prop-6 .statement}

Soient K un corps, A un sous-anneau de K. Supposons que A ne soit pas un corps. Alors les conditions suivantes sont équivalentes :
a) A est l’anneau d’une valuation de hauteur 1 de K ;
b) A est un anneau de valuation pour K, et n’a d’autres idéaux premiers que (0) et m(A) ;
c) A est maximal parmi les sous-anneaux de K distincts de K.

La prop. 5 du n° 4 montre que a) implique b), et la prop. 1 du n° 1 montre que b) implique c). Reste à montrer que c) implique a). Supposons $A$ maximal parmi les sous-anneaux de $K$ distincts de $K$. Soient $m$ un idéal maximal de $A$, et $V$ un anneau de valuation pour $K$ dominant $A_m$ ($§ 1$, n° 2, cor. du th. 2); comme $m(V) \cap A = m$ et que $m \neq (0)$ (puisque $A$ n’est pas un corps), on a $V \neq K$, d’où $V = A$, ce qui montre que $A$ est l’anneau d’une valuation $\nu$ de $K$. Ceci étant, $\nu$ est de hauteur 1 d’après les prop. 1 (n° 1) et 5 (n° 4).

#### Proposition 7 {#ac-vi-s4-prop-7 .statement}

*Pour qu’une valuation d’un corps soit de hauteur 1, il faut et il suffit que son groupe des ordres soit isomorphe à un sous-groupe ordonné non nul de $\mathbf{R}$*.

Cela résulte en effet de la proposition suivante :

#### Proposition 8 {#ac-vi-s4-prop-8 .statement}

*Soit $G$ un groupe totalement ordonné non réduit à 0. Les conditions suivantes sont équivalentes :
a) $G$ est de hauteur 1 ;
b) quels que soient $x > 0$ et $y \geqslant 0$ dans $G$, il existe un entier $n \geqslant 0$ tel que $y \leqslant nx$ ;
c) $G$ est isomorphe à un sous-groupe non réduit à 0 du groupe additif ordonné $\mathbf{R}$*.

Soit $x$ un élément positif de $G$, et soit $H_x$ l’ensemble des $y \in G$ tels qu’il existe un entier $n \geqslant 0$ vérifiant $|y| \leqslant nx$. On vérifie aisément que $H_x$ est un sous-groupe isolé de $G$, et que tout sous-groupe isolé de $G$ contenant $x$ contient $H_x$. La condition a) équivaut donc à « $H_x = G$ pour tout $x > 0$ », c’est-à-dire à la condition b).

Il est clair que c) implique b). Réciproquement, supposons vérifiée la condition b), et notons $Q$ l’ensemble des éléments $> 0$ de $G$. Supposons d’abord que $Q$ ait un plus petit élément $x$; pour tout $y \in Q$, soit $n$ le plus petit entier tel que $y \leqslant nx$; si l’on avait $y < nx$, on aurait aussi $nx - y \geqslant x$, d’où $y \leqslant (n - 1)x$ contrairement au choix de $n$; on a donc $y = nx$, ce qui montre que $G = \mathbf{Z}x$ est isomorphe à $\mathbf{Z} \subset \mathbf{R}$. Supposons maintenant que $Q$ n’ait pas de plus petit élément; appliquons à l’ensemble ordonné $P = Q \cup \{0\}$ la prop. 1 de *Top. Gén.*, chap. V, § 2 (ce qui est possible, puisque la condition $b$) n’est autre que « l’axiome d’Archimède »); on voit qu’il existe une application strictement croissante $f$ de $P$ dans $\mathbf{R}_+$ telle que

$$
f(x + y) = f(x) + f(y)
$$

pour $x \in P$ et $y \in P$; par linéarité $f$ se prolonge en un isomorphisme de $G$ sur un sous-groupe de $\mathbf{R}$, ce qui prouve que b) implique c).

#### Proposition 9 {#ac-vi-s4-prop-9 .statement}

Soient $K$ un corps, $\nu$ une valuation non impropre de $K$, et $A$ l’anneau de $\nu$. Pour que $A$ soit complètement intégralement clos (chap. V, § 1, n° 4, déf. 5), il faut et il suffit que $\nu$ soit de hauteur 1.

Supposons $\nu$ de hauteur 1. Soit $x \in K$ tel que les $x^n (n \geq 0)$ soient tous contenus dans un sous-A-module de type fini de $K$. Il existe $d \in A - \{0\}$ tel que $dx^n \in A$ pour tout $n \geq 0$. On a donc $\nu(d) + n \nu(x) \geq 0$, c’est-à-dire $n(-\nu(x)) \leq \nu(d)$ pour tout $n \geq 0$, d’où $-\nu(x) \leq 0$ (prop. 8, $b$)) et $x \in A$. Ainsi $A$ est complètement intégralement clos.

Supposons maintenant que $\nu$ ne soit pas de hauteur 1. Il existe alors $y \in m(A)$ et $t \in A$ tels que $n \nu(y) < \nu(t)$ pour tout $n \geq 0$ (prop. 8, $b$)). On a donc $ty^{-n} \in A$ pour tout $n \geq 0$, mais $y^{-1} \notin A$. Donc $A$ n’est pas complètement intégralement clos.

#### Corollaire {#ac-vi-s4-n5-cor-1 .statement}

Soient $K$ un corps, $(\nu_\alpha)_{\alpha \in I}$ une famille de valuations de hauteur 1 de $K$, et $A$ l’intersection des anneaux des $\nu_\alpha$. Alors $A$ est complètement intégralement clos.

Un anneau complètement intégralement clos n’est pas toujours intersection d’anneaux de valuations de hauteur 1 (exerc. 6).

## EXERCICES {#ac-vi-s4-exercises}

See the [exercises for § 4](exercises/s4/).
