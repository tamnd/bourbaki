---
book: ac
book_title: Commutative Algebra
chapter: IX
chapter_title: ANNEAUX LOCAUX NOETHÉRIENS COMPLETS
section: 2
section_title: Anneaux de Cohen
lang: fr
source: ac-viii-ix-fr
book_pages: AC IX.17-AC IX.27, AC IX.68-AC IX.75
pdf_pages: 0129-0139, 0180-0187
extraction: ocr
subsections:
    - "no": 1
      title: $p$-anneaux
      page: 17
      pdf_page: 129
    - "no": 2
      title: Anneaux de Cohen
      page: 20
      pdf_page: 132
    - "no": 3
      title: Existence et unicité des $p$-anneaux
      page: 22
      pdf_page: 134
    - "no": 4
      title: Représentants multiplicatifs
      page: 24
      pdf_page: 136
    - "no": 5
      title: Structure des anneaux locaux noethériens complets
      page: 0
      pdf_page: 138
statements: 30
exercises: 17
content_sha256: 55a245e21b3153aae0c2254426dfc0000c89fee4a5e3f77c1215285ee543c76f
---

## § 2. ANNEAUX DE COHEN

Dans tout ce paragraphe, $p$ désigne un nombre premier.

### 1. $p$-anneaux

#### Définition 1 {#ac-ix-s2-def-1 .statement}

On dit qu’un anneau $C$ est un $p$-anneau si l’idéal $pC$ de $C$ est maximal, et si $C$ est séparé et complet pour la topologie $pC$-adique.

Soit $C$ un anneau ; si $p1_C$ est nilpotent et si l’idéal $pC$ de $C$ est maximal, $C$ est un $p$-anneau, car la topologie $pC$-adique de $C$ est discrète. Plus particulièrement, tout corps de caractéristique $p$ est un $p$-anneau.

#### Proposition 1 {#ac-ix-s2-prop-1 .statement}

Soit $C$ un $p$-anneau.

a) L’anneau $C$ est local, d’idéal maximal $pC$.

b) Supposons $p1_C$ nilpotent. Soit $d$ le plus petit entier positif tel que $p^d1_C = 0$. Les idéaux de $C$ sont de la forme $p^kC$ avec $0 \leq k \leq d$ et l’on a $p^kC \neq p^lC$ lorsque $k$ et $l$ sont deux entiers distincts vérifiant $0 \leq k \leq d, 0 \leq l \leq d$. Le $C$-module $C$ est de longueur $d$.

c) Supposons que $p1_C$ ne soit pas nilpotent. Alors $C$ est un anneau de valuation discrète dont le corps résiduel est de caractéristique $p$, et le corps des fractions de caractéristique $0$. Les idéaux de la forme $p^nC$, avec $n \in \mathbf{N}$, sont deux à deux distincts ; ils forment tous les idéaux non nuls de $C$. Le $C$-module $C$ n’est pas de longueur finie.

L’assertion a) résulte de la prop. 19 de III, $§ 2$, no 13.

On a $\bigcap_{n \geqslant 0} p^n C = \{0\}$ par hypothèse. Soit $x \neq 0$ dans $C$; il existe un entier $n \geqslant 0$ tel que $x \in p^n C$, $x \notin p^{n+1} C$; il existe donc un élément $y$ de $C$ tel que $x = p^n y$; comme $y$ n’appartient pas à $pC$, $y$ est inversible.

Supposons que $p 1_C$ ne soit pas nilpotent. Si $x$ et $x'$ sont deux éléments non nuls de $C$, il existe deux entiers $n \geqslant 0$, $n' \geqslant 0$ et deux éléments inversibles $y$, $y'$ de $C$ tels que $x = p^n y$, $x' = p^{n'} y'$. On a alors $xx' = p^{n+n'} yy' \neq 0$, donc $C$ est intègre. Comme $C$ est un anneau local, mais n’est pas un corps et que l’idéal maximal $m_C = pC$ de $C$ est principal, $C$ est un anneau de valuation discrète (VI, $§ 3$, no 6, prop. 9). Les idéaux non nuls de $C$ sont alors de la forme $p^n C$ d’après *loc. cit.*, prop. 8, et sont deux à deux distincts. En particulier, l’anneau $C$ n’est pas artinien, donc le $C$-module $C$ n’est pas de longueur finie. Le corps résiduel $C/pC$ de $C$ est de caractéristique $p$. Soit $q$ la caractéristique du corps des fractions de $C$. On a $p 1_C \neq 0$, d’où $p \neq q$. Par ailleurs, si $q$ était non nulle, on aurait $q 1_C = 0$ donc $C/pC$ serait de caractéristique $q \neq p$, ce qui est absurde. Ceci prouve c).

Supposons que $p 1_C$ soit nilpotent. Soit $d$ le plus petit entier positif tel que $p^d 1_C = 0$. On a une suite d’idéaux

(E)
$$
C \supset pC \supset p^2 C \supset ... \supset p^{d-1} C \supset p^d C = \{0\} .
$$

Si $k$ est un entier tel que $0 \leqslant k < d$ et $p^k C = p^{k+1} C$, on en déduit

$$
p^{d-k-1} p^k C = p^{d-k-1} p^{k+1} C = \{0\}
$$

contrairement à l’hypothèse $p^{d-1} 1_C \neq 0$. Donc les éléments de la suite (E) sont deux à deux distincts. Soit $a$ un idéal de $C$ et soit $k$ le plus petit entier positif tel que $a \supset p^k C$. Soit $x$ un élément non nul de $a$; on a vu que $x$ est de la forme $p^m u$ avec $m \geqslant 0$ et $u$ inversible dans $C$. On a donc $p^m C \subset a$, d’où $m \geqslant k$, et finalement $x \in p^k C$. En conclusion, on a $a = p^k C$. La suite (E) est alors une suite de Jordan-Hölder du $C$-module $C$, qui est de longueur $d$.

#### Corollaire 1 {#ac-ix-s2-prop-1-cor-1 .statement}

Si le $p$-anneau $C$ est intègre, c’est un anneau de valuation discrète, ou un corps de caractéristique $p$.

Supposons $C$ intègre. Si $p 1_C$ est nilpotent, on a $p 1_C = 0$, et $\{0\}$ est un idéal maximal de $C$, donc $C$ est un corps de caractéristique $p$. Si $p 1_C$ n’est pas nilpotent, alors $C$ est un anneau de valuation discrète d’après la prop. 1, c).

#### Corollaire 2 {#ac-ix-s2-prop-1-cor-2 .statement}

Soient $C$ un $p$-anneau et $a$ un idéal de $C$ distinct de $C$. L’anneau $C/a$ est un $p$-anneau.

On peut supposer $a \neq \{0\}$. Il existe alors un entier $i \geqslant 1$ tel que $a = p^i C$; l’idéal $pC/a$ de $C/a$ est maximal et l’on a $p^i 1_{C/a} = 0$, donc $C/a$ est un $p$-anneau.

Soit $C$ un $p$-anneau. On appelle *longueur de* $C$, et l’on note $l(C)$, la borne supérieure dans $\overline{\mathbf{R}}$ de l’ensemble des entiers $n \geqslant 1$ tels que $p^{n-1} 1_C \neq 0$. Lorsque $l(C)$ est finie, c’est la longueur du $C$-module $C$, et lorsque $l(C)$ est égale à $+ \infty$, le $C$-module $C$ n’est pas de longueur finie (prop. 1).

#### Exemple 1 {#ac-ix-s2-n1-exa-1 .statement}

Pour tout entier $n \geqslant 1$, l’anneau $\mathbf{Z}/p^n\mathbf{Z}$ est un $p$-anneau de longueur $n$. L’anneau $\mathbf{Z}_p$ des entiers $p$-adiques est un $p$-anneau de longueur infinie.

#### Exemple 2 {#ac-ix-s2-n1-exa-2 .statement}

Soit $K$ un corps parfait de caractéristique $p$. D’après la prop. 8 du § 1, no 8, l’anneau $W(K)$ des vecteurs de Witt est un $p$-anneau de longueur infinie. L’application $(a_n)_{n \in \mathbf{N}} \mapsto a_0$ induit par passage au quotient un isomorphisme de $W(K)/pW(K)$ sur le corps $K$ (loc. cit., prop. 7). Pour tout entier $n \geqslant 1$, l’anneau
$$
W_n(K) = W(K)/p^nW(K)
$$
est un $p$-anneau de longueur $n$.

#### Proposition 2 {#ac-ix-s2-prop-2 .statement}

Soient $C$ et $C'$ deux $p$-anneaux et $u$ un homomorphisme de $C$ dans $C'$. Soit $v$ l’homomorphisme de $\kappa_C = C/pC$ dans $\kappa_{C'} = C'/pC'$ déduit de $u$ par passage aux quotients.

a) On a $l(C) \geqslant l(C')$ et $u$ est injectif si et seulement si l’on a $l(C) = l(C')$.

b) Pour que $u$ soit surjectif, il faut et il suffit que $v$ soit un isomorphisme.

c) Pour que $u$ soit un isomorphisme, il faut et il suffit que $v$ soit un isomorphisme et qu’on ait $l(C) = l(C')$.

Soit $n \geqslant 1$ un entier. On a $u(p^{n-1}1_C) = p^{n-1}1_{C'}$, donc la relation $p^{n-1}1_{C'} \neq 0$ entraîne $p^{n-1}1_C \neq 0$ et lui est équivalente si $u$ est injectif. On a donc $l(C') \leqslant l(C)$ avec égalité si $u$ est injectif. Si $u$ n’est pas injectif, il existe un entier $i < l(C)$ tel que le noyau de $u$ soit l’idéal $p^iC$ de $C$; on a alors $p^i1_{C'} = 0$, d’où $l(C') \leqslant i$. Ceci prouve a).

Comme $\kappa_C$ et $\kappa_{C'}$ sont des corps, l’homomorphisme $v$ est injectif. Si $u$ est surjectif, il en est de même de $v$ qui est donc un isomorphisme. Réciproquement, supposons $v$ surjectif. Alors pour tout entier $n \geqslant 0$, l’application $v_n : p^nC/p^{n+1}C \to p^nC'/p^{n+1}C'$ déduite de $u$ est surjective. Comme $C$ est complet pour la filtration $pC$-adique et $C'$ séparé pour la filtration $pC'$-adique, $u$ est surjectif d’après le cor. 2 du th. 1 de III, § 2, no 8. Ceci prouve b).

Enfin, c) résulte de a) et b).

#### Proposition 3 {#ac-ix-s2-prop-3 .statement}

Soit $(C_n, \pi_{n,m})$ un système projectif d’anneaux relatif à l’ensemble d’indices $\mathbf{N}$. On suppose que $C_n$ est un $p$-anneau pour tout $n \in \mathbf{N}$ et que les homomorphismes $\pi_{n,m}$ sont surjectifs. Alors $C = \varprojlim C_n$ est un $p$-anneau, et pour tout $n \in \mathbf{N}$, l’homomorphisme canonique $\pi_n : C \to C_n$ est surjectif et induit un isomorphisme de $\kappa_C$ sur $\kappa_{C_n}$.

Comme les applications $\pi_{n,m}$ sont surjectives, il en est de même des applications $\pi_n$ (E, III, p. 58, prop. 5). Montrons que $C$ est un $p$-anneau. Soit $d_n$ la longueur de $C_n$. D’après la prop. 2, a), la suite des éléments $d_n$ de $\mathbf{N} \cup \{ + \infty \}$ est croissante ; si elle est stationnaire, il existe un entier $n_0$ tel que $\pi_{n,m}$ soit un isomorphisme de $C_m$ sur $C_n$ lorsque $n_0 \leqslant n \leqslant m$, de sorte que $C$, isomorphe à $C_{n_0}$, est un $p$-anneau.

Il suffit donc de considérer le cas où chaque $d_n$ est fini, et où la suite $(d_n)$ tend vers $+ \infty$. Munissons l’anneau $C$ de la filtration triviale (III, § 2, no 1, exemple 5). Pour $n \in \mathbf{N}$, soit $I_n$ le noyau de $\pi_n$; posons $I_n = C$ si $n < 0$. Notons $E$ le $C$-module $C$ muni de la filtration $(I_n)_{n \in \mathbf{Z}}$. Il est séparé et complet, car la topologie $\mathcal{T}$ définie par la filtration $(I_n)_{n \in \mathbf{Z}}$ est la topologie limite projective des topologies discrètes sur les $C_n$.

Soit k un entier $\geqslant 1$. On a $p^k C \subset \varprojlim (p^k C_n)$ (E, III, p. 55, formule (9)). Réciproquement, si $x = (x_n)_{n \in \mathbf{N}} \in \varprojlim (p^k C_n)$ et si on pose $X_n = \{ y \in C | \pi_n(p^k y) = x_n \}$, la suite $(X_n)_{n \in \mathbf{N}}$ est une suite décroissante de parties affines fermées non vides de E. Comme $E/I_n$ est un C-module artinien, l’intersection des $X_n$ est non vide (III, § 2, no 7, prop. 7); pour tout $z \in \bigcap_{n \in \mathbf{N}} X_n$, on a $p^k z = x$. Nous avons donc prouvé qu’on a $p^k C = \varprojlim p^k C_n$ pour tout entier $k \geqslant 1$. En particulier l’idéal $p^k C$ de C est fermé pour la topologie $\mathcal{T}$. Sur C, la topologie $p$-adique est plus fine que la topologie $\mathcal{T}$ car on a $p^{d_n} C \subset I_n$. Il résulte alors de TG, III, p. 26, cor. 1 à la prop. 10, que C est séparé et complet pour la topologie $pC$-adique. En outre on a $pC = \varprojlim pC_n = \pi_0^{-1}(pC_0)$ et donc l’homomorphisme surjectif de $C/pC$ dans $C_0/pC_0$ déduit de $\pi_0$ est un isomorphisme. Ceci montre que l’idéal $pC$ de C est maximal et par suite que C est un $p$-anneau. La dernière assertion de la prop. 3 résulte de la prop. 2, b).

### 2. Anneaux de Cohen

#### Définition 2 {#ac-ix-s2-def-2 .statement}

Soit A un anneau local séparé et complet, dont le corps résiduel est de caractéristique p. On appelle sous-anneau de Cohen de A un sous-anneau C de A qui est un $p$-anneau tel que $A = m_A + C$ (i.e. $A/m_A = C/(m_A \cap C)$).

Si C est un sous-anneau de Cohen de A, l’idéal $m_A \cap C$ de C est maximal, donc égal à $pC$. L’application canonique de $\kappa_C = C/pC$ sur $\kappa_A = A/m_A$ est donc un isomorphisme de corps.

#### Exemple {#ac-ix-s2-n2-exa-1 .statement}

Soit C un $p$-anneau. L’anneau de séries formelles $A = C[[T_1, ..., T_n]]$ est un anneau noethérien, local, séparé et complet, dont l’idéal maximal est engendré par la suite $(p, T_1, ..., T_n)$. Il est immédiat que C est un sous-anneau de Cohen de A. Ceci s’applique en particulier lorsque C est égal à $\mathbf{Z}_p$, à $\mathbf{Z}/p^n \mathbf{Z}$ ou à un corps de caractéristique $p$.

#### Théorème 1 {#ac-ix-s2-thm-1 .statement}

Soit A un anneau local, séparé et complet, dont le corps résiduel k est de caractéristique p. Soit $\pi$ l’application canonique de A sur k, et soit S une partie de A, telle que $\pi$ induise une bijection de S sur une p-base de k (A, V, p. 95).
a) Il existe un sous-anneau de Cohen C de A contenant S, et un seul.
b) Le sous-anneau C de A est fermé, et la topologie $pC$-adique de C est induite par la topologie $m_A$-adique de A.
c) Tout sous-anneau fermé $A'$ de A, contenant S, et tel que $A = A' + m_A$, contient C.

A) Cas particulier : $m_A$ nilpotent

Soit n un entier positif tel que $m_A^{n+1} = \{0\}$. Si $\Phi_n$ est le n-ième polynôme de Witt ($§ 1$, no 1), l’application $u : [a_0, ..., a_n] \mapsto \Phi_n(a_0, ..., a_n)$ est un homomorphisme d’anneaux de $W_{n+1}(A)$ dans A ($§ 1$, no 7). Soit $B_n$ l’image de $u$ et soit $C_n$ le sous-anneau de A engendré par $B_n \cup S$.

#### Lemme 1 {#ac-ix-s2-lem-1 .statement}

Soit $A'$ un sous-anneau de $A$ contenant $S$. Pour que $A'$ contienne $C_n$, il faut et il suffit qu’on ait $A' + m_A = A$.

On a $pA \subset m_A$ et $B_n$ se compose des éléments de la forme $a_0^{p^n} + pa_1^{p^{n-1}} + \cdots + p^n a_n$ avec $a_0, ..., a_n$ dans $A$. Par suite, on a $\pi(B_n) = k^{p^n}$, d’où $\pi(C_n) = k^{p^n}[\pi(S)]$. Mais comme $\pi(S)$ est une $p$-base de $k$, on a $k = k^{p^n}[\pi(S)]$ (A, V, p. 96), d’où $\pi(C_n) = k$, c’est-à-dire $C_n + m_A = A$.

Soit $A'$ un sous-anneau de $A$ contenant $S$. Si $A'$ contient $C_n$, on a
$$
A' + m_A \supset C_n + m_A = A, \quad \text{d’où} \quad A' + m_A = A.
$$
Réciproquement, supposons qu’on ait $A' + m_A = A$. Soient $a_0, ..., a_n$ des éléments de $A$; il existe par hypothèse des éléments $a'_0, ..., a'_n$ de $A'$ tels que $a_i \equiv a'_i \mod m_A$ pour $0 \leq i \leq n$. D’après la prop. 1 du § 1, no 1 et l’hypothèse $m_A^{n+1} = \{0\}$, on a donc $\Phi_n(a_0, ..., a_n) = \Phi_n(a'_0, ..., a'_n) \in A'$, d’où $B_n \subset A'$. Comme $C_n$ est l’anneau engendré par $B_n \cup S$, on a $C_n \subset A'$.

Dans l’ensemble $S$ des sous-anneaux $A'$ de $A$ contenant $S$ et tels que $A' + m_A = A$, il existe d’après le lemme 1 un plus petit élément $C$, et l’on a $C_n = C$ pour tout entier $n \geq 0$ tel que $m_A^{n+1} = \{0\}$.

On a $C + m_A = A$ par construction et $p1_C$ est nilpotent. On a évidemment $pC \subset C \cap m_A$ et le lemme 2 qui suit montre donc que $pC$ est un idéal maximal de $C$ et par suite que $C$ est un sous-anneau de Cohen de $A$.

#### Lemme 2 {#ac-ix-s2-lem-2 .statement}

On a $C \cap m_A \subset pC$.

Choisissons un entier $m \geq 1$ tel que $m_A^m = \{0\}$, d’où $C = C_m = C_{m-1}$. Soit $\Lambda$ la partie de $\mathbf{N}^{(S)}$ formée des familles à support fini d’entiers $(\alpha_s)_{s \in S}$ satisfaisant à $0 \leq \alpha_s < p^m$ pour tout $s \in S$. Comme $B_m$ contient $s^{p^m} = \Phi_m(s, 0, ..., 0)$ pour tout $s \in S$, les monômes $Z_\alpha = \prod_{s \in S} s^{\alpha_s}$, où $\alpha$ parcourt $\Lambda$, engendrent $C_m$ comme $B_m$-module.

De plus, d’après la formule
$$
\Phi_m(a_0, ..., a_m) = a_0^{p^m} + p \Phi_{m-1}(a_1, ..., a_m),
$$
tout élément de $B_m$ est de la forme $a^{p^m} + pb$ avec $a \in A$ et $b \in B_{m-1}$. Par suite tout élément de $C = C_m$ est de la forme
$$
x = \sum_{\alpha \in \Lambda} c_\alpha^{p^m} Z_\alpha + py
$$
avec $c_\alpha \in A$ pour tout $\alpha \in \Lambda$, et $y \in C_{m-1} = C$. Si $x$ appartient à $C \cap m_A$, on a $\pi(x) = 0$ d’où $\sum_{\alpha \in \Lambda} \pi(c_\alpha)^{p^m} \pi(Z_\alpha) = 0$. Comme $\pi(S)$ est une $p$-base de $k$, on a $\pi(c_\alpha) = 0$ pour tout $\alpha \in \Lambda$ d’après A, V, p. 96. On a alors $c_\alpha \in m_A$, d’où $c_\alpha^m = 0$ et $a fortiori$ $c_\alpha^{p^m} = 0$. D’après (1), on a $x = py$, d’où le lemme 2.

On a $p^m C = m_A^m = \{0\}$ pour $m$ assez grand et l’assertion b) est donc triviale. L’assertion c) résulte du lemme 1. Si $C'$ est un sous-anneau de Cohen de $A$ contenant $S$, on a $C' \supset C$ d’après le lemme 1. Mais comme l’inclusion de $C$ dans $C'$ induit un isomorphisme de $\kappa_C$ sur $\kappa_{C'}$, on a $C = C'$ (no 1, prop. 2, b)), et ceci achève de prouver a).

B) *Cas général*

Pour tout entier $n \geqslant 0$, notons $A_n$ l’anneau local $A/m_A^{n+1}$, $m_n = m_A/m_A^{n+1}$ son idéal maximal et $\pi_n$ l’homomorphisme canonique de $A$ sur $A_n$. D’après A), il existe un unique sous-anneau de Cohen $C_n$ de $A_n$ contenant $\pi_n(S)$. Lorsque $0 \leqslant n \leqslant m$, on note $\pi_{n,m}$ l’homomorphisme canonique de $A_m$ sur $A_n$. D’après le cor. 2 de la prop. 1 du no 1, $\pi_{n,m}(C_m)$ est un $p$-anneau ; on a $\pi_{n,m}(C_m) + m_n = A_n$, donc $\pi_{n,m}(C_m)$ est égal au sous-anneau de Cohen $C_n$ de $A_n$. D’après la prop. 3 du no 1, le sous-anneau $\lim C_n$ de $\lim A_n$ est un $p$-anneau. Posons $C = \bigcap_{n \in \mathbf{N}} \pi_n^{-1}(C_n)$. Comme $C$ est l’image réciproque de $\lim C_n$ par l’isomorphisme $a \mapsto (\pi_n(a))_{n \in \mathbf{N}}$ de $A$ sur $\lim A_n$, c’est un sous-anneau fermé de $A$, et un $p$-anneau. On a $\pi_n(C) = C_n$ pour tout $n \in \mathbf{N}$ (no 1, prop. 3), et en particulier $\pi_0(C) = A_0$, c’est-à-dire $\pi(C) = k$. Donc $C$ est un sous-anneau de Cohen de $A$.

Pour tout entier $n \geqslant 0$, posons $J_n = C \cap m_A^n$. Comme l’anneau local $A$ est séparé, on a $\bigcap_{n \in \mathbf{N}} J_n = \{0\}$, et vu la structure des idéaux d’un $p$-anneau (no 1, prop. 1), tout idéal de $C$ de la forme $p^kC$ contient l’un des $J_n$. Réciproquement, $J_n$ contient $p^nC$. Par suite, la topologie $pC$-adique de $C$ est induite par la topologie $m_A$-adique de $A$. Ceci prouve b).

Soit $A'$ un sous-anneau fermé de $A$, contenant $S$ et tel que $A' + m_A = A$. Comme $A'$ est fermé, on a $A' = \bigcap_{n \in \mathbf{N}} \pi_n^{-1}(\pi_n(A'))$. On a $\pi_n(A') \supset \pi_n(S)$ et $\pi_n(A') + m_n = A_n$, d’où $\pi_n(A') \supset C_n$ d’après ce qu’on a vu en A). Finalement, on a $\pi_n^{-1}(\pi_n(A')) \supset \pi_n^{-1}(C_n)$ d’où $A' \supset C$. Ceci prouve c). On en déduit l’unicité d’un sous-anneau de Cohen comme en A).

#### Remarque {#ac-ix-s2-n2-rem-1 .statement}

Supposons que $p1_A$ ne soit pas nilpotent (ceci a lieu en particulier lorsque $A$ est un anneau intègre dont le corps des fractions est de caractéristique 0). Alors $C$ est un anneau de valuation discrète dont le corps des fractions est de caractéristique 0.

### 3. Existence et unicité des $p$-anneaux

#### Proposition 4 {#ac-ix-s2-prop-4 .statement}

*Soient $C$ et $C'$ deux $p$-anneaux tels que $l(C) \geqslant l(C')$, $\pi$ (resp. $\pi'$) l’homomorphisme canonique de $C$ (resp. $C'$) sur $\kappa_C$ (resp. $\kappa_{C'}$). Soit $(x_\lambda)_{\lambda \in \Lambda}$ (resp. $(x'_\lambda)_{\lambda \in \Lambda}$) une famille d’éléments de $C$ (resp. $C'$) dont l’image par $\pi$ (resp. $\pi'$) soit une $p$-base de $\kappa_C$ (resp. $\kappa_{C'}$). Soit $v$ un isomorphisme de $\kappa_C$ sur $\kappa_{C'}$ tel que $v(\pi(x_\lambda)) = \pi'(x'_\lambda)$ pour tout $\lambda \in \Lambda$. Il existe alors un unique homomorphisme $u$ de $C$ dans $C'$, tel que $v \circ \pi = \pi' \circ u$ et $u(x_\lambda) = x'_\lambda$ pour tout $\lambda \in \Lambda$. Il est surjectif. Si $l(C) = l(C')$, c’est un isomorphisme.*

Prouvons l’existence de $u$. Soit $A$ le sous-anneau de $C \times C'$ formé des couples $(x, x')$ tels que $v(\pi(x)) = \pi'(x')$. L’application $(x, x') \mapsto \pi(x)$ est un homomorphisme surjectif d’anneaux de A sur $\kappa_C$. Son noyau $m$, égal à $pC \times pC'$ est donc un idéal maximal de A. Le sous-espace topologique A de $C \times C'$ est fermé dans $C \times C'$, donc complet, et la topologie induite sur A par celle de $C \times C'$ est la topologie $m$-adique. Par suite A est un anneau local séparé et complet d’idéal maximal $m$ (III, § 2, no 13, prop. 19). Pour tout $\lambda \in \Lambda$, on a $(x_\lambda, x'_\lambda) \in A$ par hypothèse ; si $\xi_\lambda$ est la classe de $(x_\lambda, x'_\lambda)$ modulo $m$, la famille $(\xi_\lambda)_{\lambda \in \Lambda}$ est une $p$-base du corps $A/m$. D’après le th. 1 du no 2, il existe un sous-anneau de Cohen $C''$ de A, et un seul, contenant $(x_\lambda, x'_\lambda)$ pour tout $\lambda \in \Lambda$. On a $l(C'') = l(C) \geq l(C')$. La restriction à $C''$ de la projection de $C \times C'$ sur C est un homomorphisme $h : C'' \to C$ qui induit un isomorphisme de $\kappa_{C''}$ sur $\kappa_C$. D’après la prop. 2, c) du no 2, $h$ est un isomorphisme de $C''$ sur C. On voit de même que la restriction $h'$ à $C''$ de la projection de $C \times C'$ sur $C'$ est un homomorphisme surjectif de $C''$ dans $C'$. Par suite, $C''$ est le graphe d’un homomorphisme surjectif $u = h' \circ h^{-1}$ de C sur $C'$, et l’on a évidemment $v \circ \pi = \pi' \circ u$, $u(x_\lambda) = x'_\lambda$ pour tout $\lambda \in \Lambda$. En outre, si $l(C) = l(C')$, $u$ est un isomorphisme.

Prouvons l’unicité de $u$. Soit $u_1$ un homomorphisme de C dans $C'$ tel que $v \circ \pi = \pi' \circ u_1$ et $u_1(x_\lambda) = x'_\lambda$ pour tout $\lambda \in \Lambda$, et soit $C_1$ le graphe de $u_1$. Il est immédiat que $C_1$ est un sous-anneau de Cohen de A, contenant $(x_\lambda, x'_\lambda)$ pour tout $\lambda \in \Lambda$, d’où $C_1 = C''$ (th. 1 du no 2) et finalement $u_1 = u$.

#### Proposition 5 {#ac-ix-s2-prop-5 .statement}

Soit k un corps de caractéristique p, et soit n un entier $\geq 1$, ou $+ \infty$. Il existe un p-anneau de longueur n dont le corps résiduel est isomorphe à k.

L’anneau $W(k)$ des vecteurs de Witt à coefficients dans k est un anneau local intègre séparé et complet, dont le corps résiduel est isomorphe à k ($§ 1$, no 8, prop. 8), et on a $p \cdot 1_{W(k)} \neq 0$ (loc. cit., formule (52)). Soit C un sous-anneau de Cohen de $W(k)$ (no 2, th. 1). Alors C est un p-anneau de longueur $+ \infty$ dont le corps résiduel est isomorphe à k, et, si n est un entier $\geq 1$, le quotient $C/p^nC$ est un p-anneau de longueur n dont le corps résiduel est isomorphe à k.

#### Remarque 1 {#ac-ix-s2-n3-rem-1 .statement}

Soient n un entier $\geq 1$ et S une p-base de k. On peut montrer que le sous-anneau de $W_n(k)$ engendré par $W_n(k^{p^n})$ et par les éléments $[\xi, 0, ..., 0]$ ($\xi \in S$), est un p-anneau de longueur n dont le corps résiduel est isomorphe à k (cf. p. 72, exerc. 10).

#### Remarque 2 {#ac-ix-s2-n3-rem-2 .statement}

Le lecteur trouvera en Appendice une démonstration de la prop. 5 qui n’utilise ni les résultats du $§ 1$, ni le théorème d’existence de sous-anneaux de Cohen (no 2, th. 1).

#### Corollaire {#ac-ix-s2-n3-cor-1 .statement}

Soit C un p-anneau de longueur finie n. Il existe un p-anneau $C'$ de longueur infinie tel que C soit isomorphe à $C'/p^nC'$.

D’après la prop. 5, il existe un p-anneau $C'$ de longueur infinie tel que $\kappa_{C'}$ soit isomorphe à $\kappa_C$. Alors $C'/p^nC' = C'_n$ est un p-anneau de longueur n, et le corps $\kappa_{C'_n}$ est isomorphe à $\kappa_{C'}$, donc à $\kappa_C$. D’après la prop. 4, les anneaux C et $C'_n$ sont donc isomorphes.

### 4. Représentants multiplicatifs

#### Proposition 6 {#ac-ix-s2-prop-6 .statement}

Soit C un p-anneau, dont le corps résiduel k soit parfait. Supposons C de longueur finie n (resp. infinie). Il existe un unique isomorphisme $u : W_n(k) \to C$ (resp. $u : W(k) \to C$) qui induise par passage aux quotients l’application identique de k.

Comme $W_n(k)$ (resp. $W(k)$) est un p-anneau de corps résiduel k, et de longueur n (resp. de longueur infinie) (n° 1, exemple 2), et que $\varnothing$ est une p-base du corps parfait k, la prop. 6 est un cas particulier de la prop. 4 du n° 3.

#### Théorème 2 {#ac-ix-s2-thm-2 .statement}

Soient A un anneau local séparé et complet, k son corps résiduel et $\pi$ l’homomorphisme canonique de A sur k. On suppose que k est un corps parfait de caractéristique p.

a) Il existe un unique homomorphisme d’anneaux $u : W(k) \to A$ tel que $\pi(u(a)) = a_0$ pour $a = (a_n)_{n \in \mathbf{N}}$ dans W(k).

b) L’homomorphisme u est continu lorsqu’on munit W(k) de la topologie $pW(k)$-adique, et l’image de u est l’unique sous-anneau de Cohen de A.

D’après le th. 1 du n° 2, il existe un unique sous-anneau de Cohen de A ; notons-le C. Soit u un homomorphisme de W(k) dans A tel que $\pi(u(a)) = a_0$ pour tout $a = (a_n)_{n \in \mathbf{N}}$ dans W(k) ; il est immédiat que l’image de u est un sous-anneau de Cohen de A, donc égal à C. L’existence et l’unicité de u résultent alors de la prop. 6. La topologie $pC$-adique de C est induite par la topologie $m_A$-adique de A (n° 2, th. 1, b)), d’où la continuité de u.

Pour une construction directe de u, voir p. 70, exerc. 6.

#### Proposition 7 {#ac-ix-s2-prop-7 .statement}

Conservons les hypothèses et notations du th. 2. Il existe une unique partie multiplicative S de A telle que $\pi$ induise une bijection de S sur k. Pour qu’un élément a de A appartienne à S, il faut et il suffit que pour tout $n \in \mathbf{N}$, il existe un élément $a_n$ de A tel que $a = a_n^{p^n}$. L’ensemble S est l’ensemble des éléments de la forme $u(x, 0, 0, ...)$.

Prouvons tout d’abord l’unicité de S. Soit S une partie multiplicative de A, telle que $\pi$ induise une bijection de S sur k. Soit T l’ensemble des éléments de A qui sont des puissances $p^n$-ièmes pour tout $n \in \mathbf{N}$.

a) On a $S \subset T$ : Soient $a \in S$ et $n \in \mathbf{N}$; comme le corps k est parfait, il existe un élément $x_n$ de k tel que $x_n^{p^n} = \pi(a)$; comme on a $\pi(S) = k$, il existe un élément $a_n$ de S tel que $x_n = \pi(a_n)$. On a alors $\pi(a_n^{p^n}) = \pi(a)$ d’où $a_n^{p^n} = a$ puisque la restriction de $\pi$ à S est injective.

b) La restriction de $\pi$ à T est injective : soient a et b deux éléments de T tels que $\pi(a) = \pi(b)$. Soit $n \in \mathbf{N}$; il existe deux éléments $a_n$ et $b_n$ de A tels que $a = a_n^{p^n}, b = b_n^{p^n}$. On a alors $\pi(a_n)^{p^n} = \pi(b_n)^{p^n}$, d’où $\pi(a_n) = \pi(b_n)$, c’est-à-dire $a_n \equiv b_n$ mod. $m_A$. D’après le lemme 1 du § 1, n° 1, on a $a_n^{p^n} \equiv b_n^{p^n}$ mod. $m_A^{n+1}$ c’est-à-dire $a \equiv b$ mod. $m_A^{n+1}$. Comme n est arbitraire, on a $a = b$.

Les propriétés a) et b) ci-dessus, jointes à la formule $\pi(S) = k$, entraînent la relation $S = T$, d’où l’unicité.

Prouvons maintenant l’existence de S. Avec les notations du th. 2, posons $\varphi = u \circ \tau_k$, c’est-à-dire (§ 1, n° 6)

(2)
$$
\varphi(x) = u(x, 0, 0, ...)
$$
pour tout $x \in k$. D’après la prop. 4 de loc. cit., on a

(3)
$$
\varphi(1) = 1,\quad \varphi(xy) = \varphi(x) \varphi(y) \text{ pour } x, y \text{ dans } k.
$$

Il est clair que l’application $\pi \circ \varphi$ est l’application identique de $k$. Donc l’image S de $\varphi$ satisfait aux conditions de la prop. 7.

Les éléments de S sont souvent appelés les représentants multiplicatifs (ou de Teichmüller) de A.

#### Remarque 1 {#ac-ix-s2-n4-rem-1 .statement}

Conservons les hypothèses et notations précédentes. On a
$$
a = \sum_{n=0}^{\infty} p^n \tau_k(a_n^{p^{-n}}) \quad (a = (a_n)_{n \in \mathbf{N}} \in \mathbf{W}(k))
$$
d’après la prop. 7 du § 1, n° 8. On a donc
(4)
$$
u(a) = \sum_{n=0}^{\infty} p^n \varphi(a_n^{p^{-n}})
$$
pour tout $a = (a_n)_{n \in \mathbf{N}}$ dans $\mathbf{W}(k)$, car $u$ est continu (th. 2, b)). D’après la formule (4), l’unique sous-anneau de Cohen de A se compose des éléments de la forme $\sum_{n=0}^{\infty} p^n s_n$ avec $s_n \in S$ pour tout entier $n \geq 0$.

#### Remarque 2 {#ac-ix-s2-n4-rem-2 .statement}

Soient A un anneau local séparé et complet, $k$ son corps résiduel et $\pi$ l’homomorphisme canonique de A sur $k$. On peut montrer qu’il existe une partie multiplicative S de A (non unique en général) telle que $\pi$ induise une bijection de S sur $k$ (cf. p. 72, exerc. 11).

#### Exemple 1 {#ac-ix-s2-n4-exa-1 .statement}

Soit $k$ un corps parfait de caractéristique $p$. Les représentants multiplicatifs de l’anneau $\mathbf{W}(k)$ sont les vecteurs de Witt $\tau(x) = (x, 0, 0, ...)$ pour $x \in k$.

#### Exemple 2 {#ac-ix-s2-n4-exa-2 .statement}

Soit A un anneau local intègre, séparé et complet. On suppose que le corps résiduel $k$ de A est fini, à $q = p^f$ éléments, donc parfait de caractéristique $p$. On a $x^q = x$ pour tout $x \in k$, d’où $s^q = s$ pour tout représentant multiplicatif s. Il en résulte que l’ensemble des représentants multiplicatifs se compose de 0 et des $q - 1$ racines $(q - 1)$-ièmes de l’unité dans le corps des fractions de A. Si le corps des fractions de A est localement compact, l’existence des représentants multiplicatifs découle aussi de VI, § 9, n° 2, prop. 3 (cf. aussi VI, § 9, exerc. 5).

#### Exemple 3 {#ac-ix-s2-n4-exa-3 .statement}

Plus particulièrement, considérons le cas $A = \mathbf{Z}_p$. Alors les représentants multiplicatifs sont 0 et les racines $(p - 1)$-ièmes de l’unité dans le corps des fractions $\mathbf{Q}_p$ de $\mathbf{Z}_p$.

### 5. Structure des anneaux locaux noethériens complets

Soient $A$ et $C$ des anneaux locaux noethériens complets et soit $u$ un homomorphisme local de $C$ dans $A$, induisant par passage aux quotients un isomorphisme de $\kappa_C$ sur $\kappa_A$. Soit $(p_1, ..., p_m)$ une suite engendrant l’idéal $m_C$ de $C$, et soient $t_1, ..., t_n$ des éléments de $m_A$. Posons $B = C[[T_1, ..., T_n]]$.

#### Lemme 3 {#ac-ix-s2-lem-3 .statement}

a) Il existe un unique homomorphisme $v : B \to A$ qui prolonge $u$ et applique $T_i$ sur $t_i$ pour $1 \leq i \leq n$.

b) Pour que $v$ soit surjectif, il faut et il suffit que la suite $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ engendre l’idéal $m_A$ de $A$, ou encore que les classes de ces éléments modulo $m_A^2$ engendrent $m_A/m_A^2$ comme espace vectoriel sur le corps $\kappa_A$.

c) Pour que $v$ fasse de $A$ une $B$-algèbre finie, il faut et il suffit que la suite $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ engendre un idéal de définition de (la topologie $m_A$-adique de) $A$.

Notons $n$ l’idéal de l’anneau $B$ engendré par $T_1, ..., T_n$. Tout homomorphisme $v$ de $B$ dans $A$ qui prolonge $u$ et tel que $v(T_i) = t_i$ applique $n$ dans $m_A$, donc est continu lorsqu’on munit $B$ de la topologie $n$-adique. L’existence et l’unicité de $v$ résultent alors de A, IV, p. 26, prop. 4.

L’anneau $B = C[[T_1, ..., T_n]]$ est un anneau local noethérien complet (III, § 2, no 10, cor. 6 du th. 2 et no 6, prop. 6), dont l’idéal maximal $m_B$ est engendré par $p_1, ..., p_m, T_1, ..., T_n$. On a donc $v(m_B) \subset m_A$ et $v$ définit un homomorphisme gr$(v)$ de $\operatorname{gr}(B) = \bigoplus_{n=0}^\infty m_B^n/m_B^{n+1}$ dans $\operatorname{gr}(A) = \bigoplus_{n=0}^\infty m_A^n/m_A^{n+1}$. Or l’anneau $\operatorname{gr}(A)$ est engendré par $A/m_A = \kappa_A$ et $m_A/m_A^2$, gr$(v)$ induit un isomorphisme de $\kappa_B = \kappa_C$ sur $\kappa_A$, et les classes modulo $m_B^2$ des éléments $p_1, ..., p_m, T_1, ..., T_n$ engendrent $m_B/m_B^2$ comme espace vectoriel sur $\kappa_B$; de plus $v$ est surjectif si et seulement si gr$(v)$ est surjectif (III, § 2, no 8, cor. 2 du th. 1). Ceci prouve $b$.

L’idéal de $A$ engendré par la suite $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ n’est autre que $v(m_B)$ $A$. Puisque $m_A$ contient $v(m_B)$, $A$ est un anneau de Zariski pour la topologie $v(m_B)$ $A$-adique. L’anneau $A/v(m_B)$ $A$ est artinien si et seulement si sa longueur en tant que $A$-module est finie. Mais comme tout module simple sur $A$ est annulé par $m_A$ et que, par hypothèse, $A/m_A$ et $B/m_B$ sont isomorphes, cela se produit si et seulement si la dimension sur le corps $B/m_B$ de l’espace vectoriel $A/v(m_B)$ $A$ est finie. Par IV, § 2, no 5, cor. 2 de la prop. 9, on voit donc que $v(m_B)$ $A$ est un idéal de définition de $A$ si et seulement si la dimension de $A/v(m_B)$ $A$ sur $B/m_B$ est finie. C’est bien le cas si $A$ est une $B$-algèbre finie.

Supposons que $v(m_B)$ $A$ soit un idéal de définition de $A$. La topologie $m_B$-adique du $B$-module $A$ coïncide alors avec la topologie $m_A$-adique de l’anneau $A$, donc est séparée. Comme $A/v(m_B)$ $A$ est un module de type fini sur $B/m_B$, $A$ est un $B$-module de type fini (III, § 2, no 3, exemple 3 et no 9, cor. 1 de la prop. 12). Ceci prouve $c$.

#### Lemme 4 {#ac-ix-s2-lem-4 .statement}

Supposons que l’anneau local noethérien C soit régulier, et que $(p_1, ..., p_m)$ soit un système de coordonnées de C (VIII, § 5, no 1, déf. 1).

a) Si la suite $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ est sécante pour A (VIII, § 3, no 2, déf. 1), l’homomorphisme $v : B \to A$ est injectif.

b) Pour que v soit injectif et fasse de A une algèbre finie sur B, il faut et il suffit que $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ soit une suite sécante maximale pour A. Alors A est de dimension $m + n$.

Pour que la suite $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ soit une suite sécante maximale pour A, il faut et il suffit qu’elle engendre un idéal de définition de A, et que A soit de dimension $m + n$ (VIII, § 3, no 2, th. 1). D’après le lemme 3, c), il revient au même de dire que A est une B-algèbre finie, et un anneau de dimension $m + n$. Or C est un anneau intègre noethérien de dimension $m$, donc $B = C[[T_1, ..., T_n]]$ est un anneau intègre noethérien de dimension $m + n$ (VIII, § 3, no 4, cor. 3 de la prop. 8). Si A est une B-algèbre finie, et si $a$ est le noyau de $v$, on a $\dim(A) = \dim(B/a)$ (VIII, § 2, no 3, th. 1, c)) ; comme B est un anneau intègre de dimension finie, on a $\dim(B/a) < \dim(B)$ si $a \neq \{0\}$ (VIII, § 1, no 3, prop. 6, e)). Donc, si A est une B-algèbre finie, $v$ est injectif si et seulement si A est de dimension $m + n$. Ceci prouve b).

Supposons que la suite $(u(p_1), ..., u(p_m), t_1, ..., t_n)$ d’éléments de $m_A$ soit sécante. On peut lui adjoindre (VIII, § 3, no 2, th. 1) des éléments $t_{n+1}, ..., t_{n+r}$ de $m_A$ pour en faire une suite sécante maximale. D’après ce qui précède, il existe alors un homomorphisme injectif $w$ de $C[[T_1, ..., T_n, T_{n+1}, ..., T_{n+r}]] = B[[T_{n+1}, ..., T_{n+r}]]$ qui prolonge $v$ et applique $T_{n+j}$ sur $t_{n+j}$ pour $1 \leq j \leq r$. Donc $v$ est injectif. Ceci prouve a).

#### Théorème 3 {#ac-ix-s2-thm-3 .statement}

Soit A un anneau local, noethérien et complet dont le corps résiduel k soit de caractéristique p. Soit C un p-anneau de longueur infinie, dont le corps résiduel soit isomorphe à k (no 3, prop. 5).

a) Soit m la dimension de l’espace vectoriel $m_A/(m_A^2 + pA)$ sur le corps k. Il existe un idéal $a$ de l’anneau $C[[T_1, ..., T_m]]$ tel que A soit isomorphe à $C[[T_1, ..., T_m]]/a$.

b) Soit d la dimension de A. Supposons que $p1_A$ ne soit pas diviseur de 0 dans A. Alors il existe un sous-anneau $A'$ de A isomorphe à $C[[T_1, ..., T_{d-1}]]$ et tel que A soit une algèbre finie sur $A'$.

Soit C’ un sous-anneau de Cohen de A (no 2, th. 1). Comme C est de longueur infinie, il existe un homomorphisme de C sur C’ (no 3, prop. 4). Par suite, il existe un homomorphisme local $u : C \to A$. Choisissons des éléments $t_1, ..., t_m$ de $m_A$ dont les classes forment une base de l’espace vectoriel $m_A/(m_A^2 + pA)$ sur le corps k. On a $u(p1_C) = p1_A$, et le lemme 3, b) prouve l’existence d’un homomorphisme surjectif de $C[[T_1, ..., T_m]]$ dans A, prolongeant $u$ et appliquant $T_i$ sur $t_i$ pour $1 \leq i \leq m$. Ceci prouve a).

Supposons que $p1_A$ ne soit pas diviseur de 0 dans A donc sécant pour A (VIII, § 3, no 2, prop. 3). Il existe alors (VIII, § 3, no 2, th. 1) des éléments $t_1, ..., t_{d-1}$ de $m_A$ tels que la suite $(p1_A, t_1, ..., t_{d-1})$ soit sécante maximale pour A. L’anneau local noethérien C est régulier, et $(p1_C)$ est un système de coordonnées de C. L’assertion b) du th. 3 résulte alors du lemme 4, b).

## EXERCICES {#ac-ix-s2-exercises}

Dans les exercices du § 2, $p$ est un nombre premier fixé. Si $a$ est un idéal d’un anneau $A$, on note $a^p$ l’idéal engendré par les éléments $a^p$, où $a$ parcourt $a$.

See the [exercises for § 2](exercises/s2/).
