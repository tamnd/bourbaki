---
book: alg
book_title: Algebra
chapter: V
chapter_title: Corps commutatifs
section: 1
section_title: CORPS PREMIERS. CARACTÉRISTIQUE
lang: fr
source: alg-iv-vii-fr
pdf_pages: 0105-0112, 0243-0244
extraction: ocr
subsections:
    - "no": 1
      title: Corps premiers
      page: 0
      pdf_page: 105
    - "no": 2
      title: Caractéristique d’un anneau et d’un corps
      page: 2
      pdf_page: 106
    - "no": 3
      title: Anneaux commutatifs de caractéristique $p$
      page: 3
      pdf_page: 107
    - "no": 4
      title: Anneaux parfaits de caractéristique $p$
      page: 5
      pdf_page: 109
    - "no": 5
      title: Exposant caractéristique d’un corps. Corps parfaits
      page: 6
      pdf_page: 110
    - "no": 6
      title: Caractérisation des polynômes à différentielle nulle
      page: 7
      pdf_page: 111
statements: 23
exercises: 5
content_sha256: ccabb795b6367ecb44790665aeebfb201ca49fe627c8152ddc6c60376751cafb
---

## § 1. CORPS PREMIERS. CARACTÉRISTIQUE

### 1. Corps premiers

Le corps des fractions de l’anneau $\mathbf{Z}$ des entiers rationnels s’appelle le corps des nombres rationnels et se note $\mathbf{Q}$ (I, p. 111). Pour tout nombre premier $p$, l’anneau quotient $\mathbf{Z}/(p)$ est un corps fini $^1$ à $p$ éléments, noté $\mathbf{F}_p$ dans la suite. Le corps $\mathbf{Q}$ est infini car il contient $\mathbf{Z}$, et n’est donc isomorphe à aucun des corps $\mathbf{F}_p$. Si $p$ et $p'$ sont deux nombres premiers distincts, les corps $\mathbf{F}_p$ et $\mathbf{F}_{p'}$ ont des cardinaux distincts, et ne sont donc pas isomorphes.

#### Définition 1 {#alg-v-s1-def-1 .statement}

On dit qu’un corps est premier s’il est isomorphe, soit à $\mathbf{Q}$, soit à l’un des corps $\mathbf{F}_p$.

Tout sous-corps de $\mathbf{Q}$ contient l’anneau $\mathbf{Z}$, donc le corps des fractions $\mathbf{Q}$ de $\mathbf{Z}$; tout sous-anneau de $\mathbf{F}_p$ est nécessairement égal à $\mathbf{F}_p$. Par suite, tout sous-corps d’un corps premier lui est nécessairement égal (cf. cor. 2 du th. 1 ci-dessous). Soient P un corps premier et A un anneau ; si $f$ et $f'$ sont deux homomorphismes de P

$^1$ On dit par abus de langage qu’un anneau ou un corps est fini si l’ensemble sous-jacent est fini.

dans $A$, l’ensemble des $x \in P$ tels que $f(x) = f'(x)$ est un sous-corps de $P$; on a donc $f = f'$ d’après ce qui précède. En particulier, le seul endomorphisme d’un corps premier est l’application identique.

#### Théorème 1 {#alg-v-s1-thm-1 .statement}

*Soit $A$ un anneau ; on suppose qu’il existe un sous-corps de $A$. Alors $A$ possède un unique sous-corps $P$ qui soit un corps premier. De plus, $P$ est contenu dans le centre de $A$ et dans tout sous-corps de $A$.

Soient $K$ un sous-corps de $A$, $C$ le centre de $A$. Posons $K' = K \cap C$; alors $K'$ est un sous-corps de $A$. Soient $f$ l’unique homomorphisme de $\mathbf{Z}$ dans $A$ et $p$ son noyau. Tout sous-anneau de $A$, et en particulier $K'$, contient $f(\mathbf{Z})$; par suite, l’idéal $p$ est premier (I, p. 111). Si $p = (0)$, l’homomorphisme $f$ de $\mathbf{Z}$ dans $K'$ est injectif ; il se prolonge donc (I, p. 110) en un isomorphisme $\bar{f}$ de $\mathbf{Q}$ sur un sous-corps $P$ de $K'$. Si $p \neq (0)$, il existe un entier strictement positif $p$ tel que $p = (p)$ (I, p. 106) ; si l’on avait $p = ab$ avec $a > 1$ et $b > 1$, on aurait $a \notin p$, $b \notin p$ et $ab \in p$ contrairement au fait que $p$ est premier. Le nombre $p$ est donc premier et $f$ définit par passage au quotient un isomorphisme $\bar{f}$ du corps $F_p = \mathbf{Z}/p$ sur un sous-corps $P$ de $K'$. Dans les deux cas, $P$ est un sous-corps de $A$ contenu dans le centre $C$ de $A$, et c’est un corps premier. Soit $L$ un sous-corps de $A$; alors $P \cap L$ est un sous-corps de $P$, et comme $P$ est premier, on a $P \cap L = P$, d’où $P \subset L$. Si $P'$ est un sous-corps de $A$ et un corps premier, on a $P \subset P'$ par ce qui précède, d’où $P = P'$ car $P'$ est premier.

#### Corollaire 1 {#alg-v-s1-thm-1-cor-1 .statement}

*Soit $K$ un corps. Il existe un unique sous-corps de $K$ qui soit un corps premier. C’est le plus petit des sous-corps de $K$.

#### Corollaire 2 {#alg-v-s1-thm-1-cor-2 .statement}

*Pour qu’un corps soit premier, il faut et il suffit qu’il ne contienne aucun sous-corps distinct de lui-même.

### 2. Caractéristique d’un anneau et d’un corps

Nous ne définirons la caractéristique d’un anneau $A$ que lorsque $A$ possède un sous-corps. S’il en est ainsi, soit $f$ l’unique homomorphisme d’anneaux de $\mathbf{Z}$ dans $A$, et soit $n$ l’unique entier positif engendrant l’idéal de $\mathbf{Z}$ noyau de $f$ (I, p. 106) ; l’entier $n$ s’appelle alors la *caractéristique de $A$*.

Soit $A$ un anneau dont la caractéristique est définie. Alors $A$ n’est pas réduit à 0. D’après le théorème 1, il existe un unique sous-corps $P$ de $A$ qui soit un corps premier ; on l’appelle le *sous-corps premier de $A$*. D’après la démonstration du théorème 1, on a les deux possibilités suivantes :

a) la caractéristique de $A$ est 0, et $P$ est isomorphe à $\mathbf{Q}$;
b) la caractéristique de $A$ est un nombre premier $p$, et $P$ est isomorphe à $\mathbf{F}_p$.

Si la caractéristique de $A$ est égale à 0, il existe un unique homomorphisme d’anneaux de $\mathbf{Q}$ dans $A$; son image est le sous-corps premier de $A$, contenu dans le centre de $A$. Il existe par conséquent une unique structure de $\mathbf{Q}$-algèbre sur $A$ compatible avec sa structure d’anneau. Lorsque la caractéristique de $A$ est un nombre premier $p$, on a des propriétés analogues où l’on remplace le corps $\overline{\mathbf{Q}}$ par le corps $\mathbf{F}_p$.

#### Proposition 1 {#alg-v-s1-prop-1 .statement}

*Soit A un anneau non réduit à 0.*

a) *Pour que A soit de caractéristique 0, il faut et il suffit que l’application $x \mapsto n.x$ de A dans A soit bijective pour tout entier $n \neq 0$.*

b) *Soit p un nombre premier. Pour que A soit de caractéristique p, il faut et il suffit que l’on ait $p.x = 0$ pour tout $x \in A$.*

Soit $f$ l’unique homomorphisme de $\mathbf{Z}$ dans A ; on a $n.x = f(n)\ x$ pour tout entier $n$ et tout $x$ dans A. Pour que A soit de caractéristique 0, il faut et il suffit que $f$ se prolonge en un homomorphisme de $\mathbf{Q}$ dans A, c’est-à-dire que $f(n)$ soit inversible dans A pour tout $n \neq 0$ (I, p. 108) ; ceci prouve a). De même, pour que A soit de caractéristique $p$, il faut et il suffit que $f$ annule $p\mathbf{Z}$, c’est-à-dire qu’on ait $f(p) = 0$, ou encore $p.x = 0$ pour tout $x \in A$ ; ceci prouve b).

Prenons pour A un corps *non nécessairement commutatif*. Le centre de A est un corps (commutatif). Par suite, la caractéristique et le sous-corps premier de A sont définis.

#### Remarque 1 {#alg-v-s1-n2-rem-1 .statement}

Soient A et A’ deux anneaux non réduits à 0. On suppose que la caractéristique de A est définie, et qu’il existe un homomorphisme $u$ de A dans A’. L’image par $u$ du sous-corps premier P de A est un sous-corps P’ de A’, isomorphe à P, donc premier. Par suite, la caractéristique de A’ est définie, et elle est égale à celle de A. Si A et A’ sont de caractéristique 0 (resp. $p \neq 0$), l’application $u$ est un homomorphisme d’algèbres sur le corps $\mathbf{Q}$ (resp. $\mathbf{F}_p$).

#### Remarque 2 {#alg-v-s1-n2-rem-2 .statement}

La remarque 1 montre que si A est un anneau de caractéristique 0 (resp. $p \neq 0$), il en est de même de tout anneau A’ contenant A comme sous-anneau, ou du quotient de A par un idéal bilatère $a \neq A$. En particulier, si K est un corps, tout sous-corps de K et tout surcorps de K ont la même caractéristique que K.

#### Remarque 3 {#alg-v-s1-n2-rem-3 .statement}

Soit A une algèbre non réduite à 0 sur un corps K. Comme l’application $\lambda \mapsto \lambda .1$ de K dans A est un homomorphisme d’anneaux, la remarque 1 montre que la caractéristique de A est définie et qu’elle est égale à celle de K.

#### Remarque 4 {#alg-v-s1-n2-rem-4 .statement}

Le corps $\mathbf{Q}$ étant infini, tout anneau de caractéristique 0 est infini ; par suite tout corps fini a une caractéristique non nulle.

#### Remarque 5 {#alg-v-s1-n2-rem-5 .statement}

Soit A un anneau non réduit à 0, dont le groupe additif soit un $\mathbf{Z}$-module sans torsion, et posons $B = \mathbf{Q} \otimes_{\mathbf{Z}} A$. L’application $x \mapsto 1 \otimes x$ de A dans B est injective (II, p. 116), donc A est isomorphe à un sous-anneau d’un anneau de caractéristique 0.

### 3. Anneaux commutatifs de caractéristique $p$

*Dans ce numéro et le suivant, on note p un nombre premier.*

#### Théorème 2 {#alg-v-s1-thm-2 .statement}

*Soit A un anneau commutatif de caractéristique p. L’application $a \mapsto a^p$ est un endomorphisme de l’anneau A, c’est-à-dire qu’on a les relations*

(1) $$(a + b)^p = a^p + b^p$$

(2) $$(ab)^p = a^p b^p$$

*pour a, b dans A.*

La formule (2) résulte de la commutativité de A. Pour prouver (1), nous utiliserons la formule du binôme $(a + b)^p = a^p + b^p + \sum_{i=1}^{p-1} \binom{p}{i} a^i b^{p-i}$; comme on a $p.x = 0$ pour tout $x \in A$, il suffit d’établir le lemme suivant :

#### Lemme 1 {#alg-v-s1-lem-1 .statement}

Soient $p$ un nombre premier et $i$ un entier compris entre 1 et $p - 1$. Le coefficient binômial $\binom{p}{i}$ est un entier divisible par $p$.

Raisonnons par récurrence sur $i$, le cas $i = 1$ résultant de la formule $\binom{p}{1} = p$.

Supposons qu’on ait $2 \leq i \leq p - 1$ et que $\binom{p}{i-1}$ soit divisible par $p$. Alors, l’entier $i \binom{p}{i} = (p - i + 1) \binom{p}{i-1}$ appartient à l’idéal premier $p \mathbf{Z}$ de $\mathbf{Z}$; comme on a $i \notin p \mathbf{Z}$, on a $\binom{p}{i} \in p \mathbf{Z}$, d’où le lemme.

Soient A un anneau commutatif de caractéristique $p$, et $f$ un entier $\geq 0$. On déduit du théorème 2, par récurrence sur $f$, que l’application $a \mapsto a^{p^f}$ est un endomorphisme de l’anneau A. En particulier, on a la relation

$$
(a_1 + \cdots + a_n)^{p^f} = a_1^{p^f} + \cdots + a_n^{p^f}
$$

quels que soient $a_1, \ldots, a_n$ dans A. L’application $a \mapsto a^p$ s’appelle parfois l’endomorphisme de Frobenius de A. Prenant $A = \mathbf{F}_p$ et $a_i = 1$, on tire de (3) la relation :

$$
n^{p^f} \equiv n \mod p \quad (n \in \mathbf{Z}, f \in \mathbf{N})
$$

Pour toute partie S de A, on note $S^{p^f}$ l’ensemble des éléments de A de la forme $x^{p^f}$ avec $x \in S$¹. En particulier, si K est un sous-anneau de A, l’ensemble $K^{p^f}$ est un sous-anneau de A. Si K est un sous-anneau de A et S une partie de A, on note K[S] le sous-anneau de A engendré par $K \cup S$; lorsque A est un corps, on note K(S) le corps des fractions de K[S], c’est-à-dire le sous-corps de A engendré par K \cup S.

#### Proposition 2 {#alg-v-s1-prop-2 .statement}

Soient A un anneau commutatif de caractéristique $p$, K un sous-anneau de A, S une partie de A, et $f$ un entier positif.
a) On a $K[S]^{p^f} = K^{p^f}[S^{p^f}]$, et si A est un corps, on a $K(S)^{p^f} = K^{p^f}(S^{p^f})$.
b) Si le K-module K[S] est engendré par une famille $(a_i)_{i \in I}$ d’éléments de A, alors le K-module $K[S^{p^f}]$ est engendré par la famille $(a_i^{p^f})_{i \in I}$.

Comme K[S] est le sous-anneau de A engendré par $K \cup S$, son image $K[S]^{p^f}$ par l’endomorphisme $\pi : a \mapsto a^{p^f}$ de l’anneau A est le sous-anneau de A engendré

¹ Bien entendu, on ne confondra l’ensemble $S^{p^f}$ ni avec l’ensemble produit de $p^f$ ensembles égaux à S, ni avec l’ensemble des produits de $p^f$ éléments appartenant à S.

par l’image $K^{p^f} \cup S^{p^f}$ de $K \cup S$ par $\pi$, d’où $K[S]^{p^f} = K^{p^f}[S^{p^f}]$. Le cas des corps se traite de manière analogue. Ceci prouve a).

Il est clair que la famille $(a_i^{p^f})_{i \in I}$ engendre le $K^{p^f}$-module $K[S]^{p^f}$. Le $K$-module $K[S^{p^f}]$ est engendré par les produits de la forme $x_1^{p^f} \ldots x_n^{p^f} = (x_1 \ldots x_n)^{p^f}$ avec $x_1, \ldots, x_n$ arbitraires dans $S$, donc aussi par l’ensemble $K[S]^{p^f}$. L’assertion b) résulte immédiatement de là.

### 4. Anneaux parfaits de caractéristique $p$

#### Définition 2 {#alg-v-s1-def-2 .statement}

On dit qu’un anneau $A$ de caractéristique $p \neq 0$ est parfait s’il est commutatif et si l’application $a \mapsto a^p$ est bijective.

Si l’anneau $A$ est parfait de caractéristique $p$, l’application $a \mapsto a^{p^f}$ est un automorphisme de l’anneau $A$ pour tout entier $f \geqslant 0$; l’automorphisme réciproque se note $a \mapsto a^{1/p^f}$ ou $a \mapsto a^{p^{-f}}$ et l’image d’une partie $S$ de $A$ par cet automorphisme se note $S^{1/p^f}$ ou $S^{p^{-f}}$. Il est clair que l’on a $(a^{p^e})^{p^f} = a^{p^{e+f}}$ pour tout $a \in A$, quels que soient les entiers $e$ et $f$ (de signe quelconque).

Soit $A$ un anneau commutatif de caractéristique $p$. Pour tout entier $f \geqslant 0$, notons $n_f$ le noyau de l’endomorphisme $a \mapsto a^{p^f}$ de l’anneau $A$. Alors $(n_f)_{f \geqslant 0}$ est une suite croissante d’idéaux de $A$; comme tout entier positif est majoré par une puissance de $p$, l’idéal $n = \bigcup_{f \geqslant 0} n_f$ se compose des éléments nilpotents de $A$. En particulier, si $A$ est parfait, tout élément nilpotent de $A$ est nul.

#### Définition 3 {#alg-v-s1-def-3 .statement}

Soit $A$ un anneau commutatif de caractéristique $p \neq 0$. On appelle clôture parfaite de $A$ un couple $(\hat{A}, u)$ où $\hat{A}$ est un anneau parfait de caractéristique $p$ et $u$ un homomorphisme de $A$ dans $\hat{A}$ satisfaisant à la propriété universelle suivante :

(CP) Si $B$ est un anneau parfait de caractéristique $p$ et $v$ un homomorphisme de $A$ dans $B$, il existe un homomorphisme $h$ de $\hat{A}$ dans $B$, et un seul, tel que $v = h \circ u$.

La propriété universelle (CP) entraîne aussitôt l’unicité de la clôture parfaite au sens suivant : si $(\hat{A}, u)$ et $(\hat{A}', u')$ sont deux clôtures parfaites de $A$, il existe un isomorphisme $h$ de $\hat{A}$ sur $\hat{A}'$, et un seul, tel que $u' = h \circ u$ (cf. E, IV, p. 23). Nous démontrons maintenant l’existence d’une clôture parfaite :

#### Théorème 3 {#alg-v-s1-thm-3 .statement}

Soit $A$ un anneau commutatif de caractéristique $p \neq 0$. Il existe une clôture parfaite $(\hat{A}, u)$ de $A$. De plus, le noyau de $u$ est l’ensemble des éléments nilpotents de $A$, et pour tout $x \in \hat{A}$, il existe un entier $n \geqslant 0$ tel que $x^{p^n} \in u(A)$.

Pour tout entier $n \geqslant 0$, posons $A_n = A$; lorsque $m \geqslant n$, on définit un homomorphisme $\pi_{m,n}$ de $A_n$ dans $A_m$ par $\pi_{m,n}(a) = a^{p^{m-n}}$. On définit ainsi un système inductif d’anneaux $(A_n, \pi_{m,n})$ (I, p. 116); soient $\hat{A}$ la limite inductive de ce système et $u_n$ l’homomorphisme canonique de $A_n = A$ dans $\hat{A}$; on pose aussi $u = u_0$. Par construction de la limite inductive, le noyau $n$ de $u$ est la réunion des noyaux des homomorphismes $\pi_{n,0}: a \mapsto a^{p^n}$ de $A$ dans $A$, donc se compose des éléments nilpotents de $A$. L’anneau $\hat{A}$ est commutatif de caractéristique $p$ d’après la remarque 1 de V, p. 3.

L’anneau $\hat{A}$ est réunion de la suite croissante $(u_n(A))_{n \geq 0}$ de sous-anneaux. On a $u_n(A)^{p^n} = u(A)$; par suite, pour tout $x \in \hat{A}$, il existe un entier $n \geq 0$ tel que $x^{p^n} \in u(A)$. On a aussi $u_n(A) = u_{n+1}(A)^p$, d’où $\hat{A}^p = \hat{A}$. Soit $x \in \hat{A}$ tel que $x^p = 0$; choisissons un entier $n \geq 1$ et un élément $a$ de $A$ tels que $x = u_n(a)$. On a alors $u_{n-1}(a) = u_n(a)^p = 0$; par définition de la limite inductive, il existe un entier $m \geq n$ tel que $\pi_{m-1,n-1}(a) = 0$, c’est-à-dire $a^{p^{m-n}} = 0$. On a alors $\pi_{m,n}(a) = 0$, d’où $u_n(a) = 0$, c’est-à-dire $x = 0$. Par suite, l’anneau $\hat{A}$ est parfait de caractéristique $p$.

Soit $v$ un homomorphisme de $A$ dans un anneau parfait $B$ de caractéristique $p$. Pour tout entier $n \geq 0$, l’application $b \mapsto b^{p^n}$ est un automorphisme de $B$, et il existe donc un homomorphisme $v_n$ de $A_n = A$ dans $B$ caractérisé par $v(a) = v_n(a)^{p^n}$. On a alors $v_m \circ \pi_{m,n} = v_n$ pour $m \geq n \geq 0$; par définition de la limite inductive, il existe un homomorphisme $h$ de $\hat{A}$ dans $B$ tel que $v_n = h \circ u_n$ pour tout $n \geq 0$; en particulier, on a $v = v_0 = h \circ u_0 = h \circ u$. Soit enfin $h'$ un homomorphisme de $\hat{A}$ dans $B$ tel que $h' \circ u = v$. Soit $x \in \hat{A}$; on a vu qu’il existe un entier $n \geq 0$ et un élément $a \in A$ tels que $x^{p^n} = u(a)$. On a alors
$$
h(x)^{p^n} = h(u(a)) = v(a) = h'(u(a)) = h'(x)^{p^n},
$$
et comme $B$ est parfait, on a $h(x) = h'(x)$. On a donc $h' = h$, et ceci achève de prouver que $(\hat{A}, u)$ est une clôture parfaite de $A$.

#### Proposition 3 {#alg-v-s1-prop-3 .statement}

*Soient B un anneau parfait de caractéristique p et A un sous-anneau de B. Posons $A^{p^{-\infty}} = \bigcup_{f \geq 0} A^{p^{-f}}$ et notons j l’injection canonique de A dans $A^{p^{-\infty}}$. Alors $A^{p^{-\infty}}$ est le plus petit sous-anneau parfait de B contenant A, et $(A^{p^{-\infty}}, j)$ est une clôture parfaite de A.*

Pour tout entier $f \in \mathbf{Z}$, on note $\pi_f$ l’automorphisme $b \mapsto b^{p^f}$ de $B$. La suite des sous-anneaux $\pi_{-f}(A)$ de $B$ (pour $f \geq 0$) est croissante, et sa réunion $A^{p^{-\infty}}$ est donc un sous-anneau de $B$. On a $\pi_1(A^{p^{-\gamma}}) = \bigcup_{f \geq 0} \pi_{-(f-1)}(A) = A^{p^{-\gamma}}$, donc $A^{p^{-\infty}}$ est un sous-anneau parfait de $B$. Enfin, soit $B_0$ un sous-anneau parfait de $B$ contenant $A$; pour tout entier $f \geq 0$, on a $\pi_{-f}(A) \subset \pi_{-f}(B_0) = B_0$, d’où $A^{p^{-\infty}} \subset B_0$.

Soit $v$ un homomorphisme de $A$ dans un anneau parfait $B'$ de caractéristique $p$. Pour tout entier $f \geq 0$, on définit un homomorphisme $h_f$ de $\pi_{-f}(A)$ dans $B'$ par $h_f(\pi_{-f}(a)) = v(a)^{p^{-f}}$ pour tout $a \in A$. On voit immédiatement que $h_{f+1}$ coïncide avec $h_f$ sur $\pi_{-f}(A)$; il existe donc un homomorphisme $h$ de $A^{p^{-\infty}}$ dans $B'$ qui induit $h_f$ sur $\pi_{-f}(A)$ pour tout $f \geq 0$, et en particulier, $h$ prolonge $h_0 = v$. Si $h'$ est un autre prolongement de $v$ en un homomorphisme de $A^{p^{-\infty}}$ dans $B$, on prouve l’égalité $h' = h$ comme dans la démonstration du théorème 3.

### 5. Exposant caractéristique d’un corps. Corps parfaits

Soit K un corps. On appelle *exposant caractéristique* de K l’entier égal à 1 si K est de caractéristique 0, et à la caractéristique de K si celle-ci est non nulle.

#### Proposition 4 {#alg-v-s1-prop-4 .statement}

*Soit K un corps d’exposant caractéristique q. Pour tout entier* f \geqslant 0, l’application x \mapsto x^{q^f} est un isomorphisme de K sur un de ses sous-corps (noté K^{q^f}).

Cela résulte du th. 2 lorsque q \neq 1 et c’est trivial lorsque q = 1.

On étend de même la prop. 2 au cas où A est un corps d’exposant caractéristique q, le cas q = 1 étant trivial.

#### Définition 4 {#alg-v-s1-def-4 .statement}

On dit qu’un corps K d’exposant caractéristique q est parfait si l’on a K^q = K. On dit que K est imparfait si l’on a K^q \neq K.

D’après cette définition, un corps est parfait s’il est de caractéristique 0, ou si c’est un anneau parfait de caractéristique p \neq 0 au sens de la définition 2. Soit K un corps de caractéristique p \neq 0, et soit (\hat{K}, u) une clôture parfaite de K. Alors \hat{K} est un corps, d’après la proposition 3 (V, p. 6), et u est un isomorphisme de K sur un sous-corps de \hat{K}. On identifie le plus souvent K à son image par u dans \hat{K}, de sorte qu’on a \hat{K} = K^{p^{-\infty}} (prop. 3).

Soit K un corps de caractéristique 0 ; l’exposant caractéristique q de K est égal à 1. Par convention, les notations x^{q^{-f}} et S^{q^{-f}} désignent respectivement x et S (pour un élément x de K et une partie S de K). En particulier, on pose K^{q^{-\infty}} = K, et l’on convient que la clôture parfaite de K est K.

#### Proposition 5 {#alg-v-s1-prop-5 .statement}

Si K est un corps de caractéristique 0, ou fini, \* ou algébriquement clos *, il est parfait. En particulier, tout corps premier est parfait.

Supposons K de caractéristique p \neq 0. Si K est fini, le sous-corps K^p de K a même cardinal que K, d’où K^p = K. \* Si K est algébriquement clos, le polynôme X^p - a a une racine x dans K pour tout a \in K (V, p. 19, déf. 1) d’où x^p = a et finalement K^p = 'K. \* Enfin, un corps premier est de caractéristique 0, ou fini.

Soient K_0 un corps de caractéristique p \neq 0 et K = K_0(X) le corps des fractions rationnelles à une indéterminée X sur K_0. Alors K est imparfait : en effet, il n’existe aucun élément u(X)/v(X) de K (u et v polynômes de K_0[X]) tel que (u(X)/v(X))^p = X ; cela se voit en écrivant cette relation sous la forme u(X)^p = X . v(X)^p et en comparant les degrés des deux membres.

### 6. Caractérisation des polynômes à différentielle nulle

#### Proposition 6 {#alg-v-s1-prop-6 .statement}

Soient K un anneau commutatif, A l’algèbre de polynômes K[X_i]_{i \in I} et S l’ensemble des éléments F de A tels que dF = 0.
a) Si K est un anneau de caractéristique 0, on a S = K.
b) Si K est un anneau de caractéristique p \neq 0, on a S = K[X_i^p]_{i \in I} ; si de plus K est parfait, on a S = A^p.

L’application F \mapsto dF de A dans le module \Omega_K(A) des K-différentielles de A est K-linéaire et satisfait à la relation

d(FF') = F . dF' + F' . dF

(III, p. 134). Par suite, S est une sous-algèbre de A.

Lorsque $K$ est de caractéristique $p \neq 0$, posons $T = K[X_i^p]_{i \in I}$; on a donc $T = A^p$ si $K$ est parfait (V, p. 4, prop. 2); de plus, on a $d(X_i^p) = pX_i^{p-1} \cdot dX_i = 0$ pour tout $i \in I$, donc la sous-algèbre $S$ de $A$ contient $T$. Si $K$ est de caractéristique 0, posons $T = K$, d’où encore $T \subset S$. Il nous reste à prouver que $S$ est contenu dans $T$.

Pour toute partie finie $J$ de $I$, soit $A_J$ la sous-algèbre de $A$ engendrée par la famille $(X_j)_{j \in J}$. On a $A_\varnothing = K$ et $A = \bigcup_{J \subset I} A_J$; il suffit donc de prouver la relation $S \cap A_J \subset T$, ce que nous ferons par récurrence sur le cardinal de $J$. Soient donc $J$ une partie finie de $I$ telle que $S \cap A_J \subset T$, $i$ un élément de $I - J$ et $J' = J \cup \{i\}$. Tout élément $F$ de $A_J$ s’écrit de manière unique sous la forme

$$
F = \sum_{n=0}^\infty F_n \cdot X_i^n,
$$

avec $F_n \in A_J$ pour tout $n \geq 0$, et l’on a alors

$$
dF = \sum_{n=0}^\infty X_i^n \cdot dF_n + \sum_{n=0}^\infty nX_i^{n-1} F_n \cdot dX_i.
$$

Supposons que $F$ appartienne à $S$; la famille $(dX_r)_{r \in I}$ est une base du $A$-module $\Omega_K(A)$ (III, p. 134) et $dF_n$ est combinaison linéaire des différentielles $dX_j$ pour $j \in J$ puisque l’on a $F_n \in A_J = K[X_j]_{j \in J}$. D’après (6), on a alors $dF_n = 0$ et $nF_n = 0$ pour tout entier $n \geq 0$. D’après l’hypothèse de récurrence on a $F_n \in T$ pour tout $n \geq 0$ puisque $dF_n = 0$.

a) Si $K$ est de caractéristique 0, on a $nF_n = 0$ pour tout $n \geq 1$ d’où $F_n = 0$ d’après la prop. 1 (V, p. 3); on a alors $F = F_0$, d’où $F \in T$.

b) Si $K$ est de caractéristique $p \neq 0$, alors $A$ est une algèbre sur le corps $F_p$, et la relation $nF_n = 0$ entraîne $F_n = 0$ pour tout entier $n$ non divisible par $p$. On a donc $F = \sum_{m=0}^\infty F_{mp} X_i^{mp}$, d’où $F \in T$.

#### Remarque {#alg-v-s1-n6-rem-1 .statement}

On a encore $S = K$ si le groupe additif de $K$ est sans torsion ; cela résulte de la démonstration donnée ci-dessus ou de la remarque 5 de V, p. 3.

#### Corollaire {#alg-v-s1-n6-cor-1 .statement}

Soient $K$ un corps et $F(X)$ un polynôme à coefficients dans $K$, dont la dérivée $F'(X)$ soit nulle.

a) Si $K$ est de caractéristique 0, on a $F \in K$.

b) Si $K$ est de caractéristique $p \neq 0$, il existe un polynôme $G(X)$ tel que l’on ait $F(X) = G(X^p)$.

En effet, on a $dF = F'.dX = 0$.

## EXERCICES {#alg-v-s1-exercises}

See the [exercises for § 1](exercises/s1/).
