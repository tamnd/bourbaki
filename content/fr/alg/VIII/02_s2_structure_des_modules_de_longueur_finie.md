---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 2
section_title: Structure des modules de longueur finie
lang: fr
source: alg-viii-fr
book_pages: A VIII.23-A VIII.40
pdf_pages: 0034-0051
extraction: native
subsections:
    - "no": 1
      title: Anneaux locaux
      page: 23
      pdf_page: 34
    - "no": 2
      title: Décomposition de Weyr-Fitting
      page: 25
      pdf_page: 36
    - "no": 3
      title: Modules indécomposables et modules primordiaux
      page: 27
      pdf_page: 38
    - "no": 4
      title: Modules semi-primordiaux
      page: 29
      pdf_page: 40
    - "no": 5
      title: Structure des modules de longueur finie
      page: 34
      pdf_page: 45
statements: 37
exercises: 19
content_sha256: bf71cdddea883d082ffabb1e855bc076eda1f524b11c3a6f13d4a05725c66fce
---

## § 2. STRUCTURE DES MODULES DE LONGUEUR FINIE

### 1. Anneaux locaux

#### Proposition 1 {#alg-viii-s2-prop-1 .statement tag=001P}

Soit A un anneau non nul et soit $\mathfrak{r}$ l’ensemble des éléments non inversibles de A. Les propriétés suivantes sont équivalentes :

(i) L’ensemble $\mathfrak{r}$ est un idéal bilatère de A ;

(ii) L’ensemble $\mathfrak{r}$ est stable par addition ;

(iii) L’anneau A possède un unique idéal à gauche maximal ;

(iv) Quel que soit $a\in A$, l’un des éléments $a$ ou $1-a$ est inversible ;

(v) Quel que soit $a\in A$, l’un des éléments $a$ ou $1-a$ est inversible à gauche.

L’implication (i) $=\Rightarrow$ (ii) résulte de la définition d’un idéal. Comme 1 n’appartient pas à $\mathfrak{r}$, on a (ii) $=\Rightarrow$ (iv).

On a $\mathfrak{r}\not= A$, et l’ensemble $\mathfrak{r}$ contient tout idéal à gauche de A distinct de A. Si $\mathfrak{r}$ est un idéal à gauche de A, c’est donc l’unique idéal à gauche maximal de A. Cela prouve que (i) entraîne (iii).

Supposons que A possède un unique idéal à gauche maximal $\mathfrak{m}$. Soit $b\in A-\mathfrak{m}$. L’idéal à gauche $Ab$ n’est contenu dans aucun idéal à gauche maximal de A, donc est égal à A (I, p. 99, th. 1) et $b$ est inversible à gauche. Quel que soit $a\in A$, l’un des éléments $a$ ou $1-a$ appartient à A $-\mathfrak{m}$, car $\mathfrak{m}$ est un idéal qui ne contient pas 1. Ainsi (iii) implique (v).

Supposons la propriété (v) satisfaite. Soit $b$ un élément de A inversible à gauche. Soit $c\in A$ tel que $cb= 1$. On a $(1-bc)b= 0$ et $b\not= 0$, donc $1-bc$ n’est pas inversible à gauche. D’après la propriété (v), $bc$ est inversible à gauche et, a fortiori, $c$ est inversible à gauche. Mais alors $c$ est inversible, $b$ est son inverse, de sorte que $b$ est inversible. Il en résulte que (v) entraîne (iv).

Il reste à prouver que (iv) implique (i). Supposons (iv) satisfaite. Alors $\mathfrak{r}$ est un idéal bilatère de A d’après les assertions a) à d) suivantes :

a) On a $0\in \mathfrak{r}$ puisque l’anneau A n’est pas nul.

b) Le produit de deux éléments de A dont l’un appartient à $\mathfrak{r}$ et l’autre à A$-\mathfrak{r}$ appartient à $\mathfrak{r}$.

c) L’ensemble $\mathfrak{r}$ est stable par addition.

Soient en effet $a$ et $b$ des éléments de $\mathfrak{r}$ tels que $s=a+b$ soit inversible. D’après b), les éléments $s^{-1}a$ et $s^{-1}b$ de A appartiennent à $\mathfrak{r}$; comme $s^{-1}b= 1-s^{-1}a$, cela contredit l’hypothèse (iv).

d) L’ensemble $\mathfrak{r}$ est stable par multiplication.

Soient en effet $a$ et $b$ deux éléments de $\mathfrak{r}$. L’élément $a'=-a(1-b)$ appartient à $\mathfrak{r}$ d’après b) de sorte que l’élément $ab$, qui est égal à $a+a'$, appartient à $\mathfrak{r}$ d’après c), d’où d).

#### Définition 1 {#alg-viii-s2-def-1 .statement tag=001Q}

On appelle anneau local un anneau non nul satisfaisant aux conditions équivalentes de la proposition 1.

Un anneau A est local si et seulement si l’anneau opposé $A^o$ est local.

Si A est un anneau local, l’ensemble $\mathfrak{r}$ des éléments de A non inversibles est un idéal bilatère de A ; il contient tout idéal à gauche ou à droite de A distinct de A. L’anneau $A/\mathfrak{r}$ est donc un corps qu’on appelle corps résiduel de A. L’ensemble $\mathfrak{r}$ est l’unique idéal à gauche (resp. à droite, resp. bilatère) maximal de A ; on dit simplement que $\mathfrak{r}$ est l’idéal maximal de A.

#### Exemple 1 {#alg-viii-s2-n1-exa-1 .statement tag=001R}

Tout corps est un anneau local.

#### Exemple 2 {#alg-viii-s2-n1-exa-2 .statement tag=001S}

Soit A un anneau non nul dans lequel tout élément est inversible ou nilpotent. Alors A est un anneau local. En effet, si $a\in A$ n’est pas inversible, il existe par hypothèse un entier $n\geqslant 0$ tel que $a^{n+1}= 0$, et $1-a$ admet pour inverse $1+a+\cdots +a^n$.

#### Exemple 3 {#alg-viii-s2-n1-exa-3 .statement tag=001T}

Soient X une variété de classe $C_r$ (VAR, R, 5.1.5) et $x$ un point de X. Soit $\mathscr{O}_x$ l’anneau des germes en $x$ de fonctions de classe $C^r$ à valeurs dans le corps des scalaires K. Alors $\mathscr{O}_x$ est un anneau local commutatif et son idéal maximal se compose des germes des fonctions s’annulant en $x.*$

#### Exemple 4 {#alg-viii-s2-n1-exa-4 .statement tag=001U}

Soient A un anneau local commutatif et $B = A[[X_i]]_{i\in I}$ une algèbre de séries formelles à coefficients dans A (III, p. 28). D’après la prop. 6 de IV, p. 28, l’anneau B est local et son idéal maximal se compose des séries formelles dont le terme constant appartient à l’idéal maximal de A. En particulier, si A est un corps, l’idéal maximal de $A[[X_i]]_{i\in I}$ se compose des séries formelles de terme constant nul.

#### Exemple 5 {#alg-viii-s2-n1-exa-5 .statement tag=001V}

Soit $p$ un nombre premier. Notons $\mathbf{Z}_{(p)}$ le sous-anneau du corps $\mathbf{Q}$des nombres rationnels constitué par les fractions $a/b$ avec $a\in \mathbf{Z},b\in \mathbf{Z}$et $b$ non divisible par $p*($cf. AC, II, p. $79)*$. Alors $\mathbf{Z}_{(p)}$ est un anneau local commutatif, d’idéal maximal

$p\mathbf{Z}_{(p)}$. L’anneau $\mathbf{Z}_p$ des entiers $p$-adiques (V, p. 92) est un anneau local commutatif, d’idéal maximal $p\mathbf{Z}_p$ (VIII, p. 37, exerc. 9).

#### Exemple 6 {#alg-viii-s2-n1-exa-6 .statement tag=001W}

Soient K un corps commutatif de caractéristique $p >0$ et G un $p$-groupe (I, p. 72, déf. 9). L’algèbre K[G] du groupe G sur K (III, p. 19) est un anneau local ; son idéal maximal est l’ensemble des éléments $(a_g)_{g\in G}$ de K[G] tels que $\sum_{g\in G}a_g= 0$ (VIII, p. 38, exerc. 10).

### 2. Décomposition de Weyr-Fitting

Soient A un anneau, M un A-module et $u$ un endomorphisme de M. Pour tout entier $p\geqslant 0$, on note $N_p$ le noyau de $u^p$. La suite des sous-modules $N_p$ est croissante et sa réunion est un sous-module $N_{\infty}$ de M stable par $u$. Pour tout entier $p\geqslant 0$, on a $N_{p+1}=^-u^1(N_p)$ et la relation $N_p= N_{p+1}$ entraîne donc $N_{p+1}= N_{p+2}$. Par suite, ou bien la suite $(N_p)$ est strictement croissante, ou bien il existe un entier $p\geqslant 0$ tel que $N_0, . . . ,N_p$ soient distincts et $N_p= N_{\infty}$.

Pour tout entier $q\geqslant 0$, notons $I_q$ l’image de $u^q$. La suite des sous-modules $I_q$ est décroissante et son intersection est un sous-module $I_{\infty}$ de M stable par $u$. Pour tout entier $q\geqslant 0$, on a $u(I_q) = I_{q+1}$ et la relation $I_q= I_{q+1}$ entraîne donc $I_{q+1}= I_{q+2}$. Par suite, ou bien la suite $(I_q)$ est strictement décroissante, ou bien il existe un entier $q\geqslant 0$ tel que $I_0, . . . ,I_q$ soient distincts et $I_q= I_{\infty}$.

#### Proposition 2 {#alg-viii-s2-prop-2 .statement tag=001X}

a) Supposons que la suite $(N_p)$est stationnaire. Alors on a $N_{\infty}\cap I_{\infty}= 0$, la restriction de $u$ à $I_{\infty}$ est injective et $u$ induit un endomorphisme nilpotent de $N_{\infty}$.

b) Supposons la suite $(I_p)$stationnaire. Alors on a $M = N_{\infty}+I_{\infty}$ et $u(I_{\infty}) = I_{\infty}$.

c) (« Décomposition de Weyr-Fitting ») Supposons que les suites $(N_p)$et $(I_p)$ soient stationnaires. Alors M est somme directe des sous-modules $N_{\infty}$ et $I_{\infty}$ qui sont stables par $u$ et $u$ induit un endomorphisme nilpotent de $N_{\infty}$ et un automorphisme de $I_{\infty}$.

Soit $p$ un entier positif tel que $N_p= N_{\infty}$ et soit $v=u^p$. Par construction, $v$ et $v^2$ ont le même noyau $N_{\infty}$ et $I_p$ est l’image de $v$. Pour $x$ dans $N_{\infty}\cap I_p$, il existe $y\in M$ tel que $x=v(y)$, d’où $v^2(y) =v(x) = 0$; on a donc $y\in N_{\infty}$, d’où $x= 0$. On a en particulier $N_{\infty}\cap I_{\infty}= 0$. Comme le noyau $N_1$ de $u$ est contenu dans $N_{\infty}$, la restriction de $u$ à $I_{\infty}$ est injective ; d’autre part, on a $u^p(N_{\infty}) = 0$. Ceci prouve a).

Soit $q$ un entier positif tel que $I_q= I_{\infty}$ et soit $w=u^q$. Alors $w$ et $w^2$ ont la même image $I_{\infty}$, et $N_q$ est le noyau de $w$. Soit $x\in M$. On a $w(x)\in I_{\infty}$, donc il existe $y\in M$ tel que $w(x) =w^2(y)$; on a alors $x-w(y)\in N_q$, d’où $M = N_q+ I_{\infty}$, et a fortiori $M = N_{\infty}+ I_{\infty}$. On a $u(I_{\infty}) =u(I_q) = I_{q+1}= I_{\infty}$. Ceci prouve b).

L’assertion c) est conséquence immédiate de a) et b).

#### Remarque 1 {#alg-viii-s2-n2-rem-1 .statement tag=001Y}

Soit $p$ un entier tel que $N_p= N_{p+1}$; la démonstration ci-dessus montre que $N_{\infty}\cap I_p= 0$, et la restriction de $u$ à $I_p$ est injective. De même, soit $q$ un entier tel que $I_q= I_{q+1}$; alors on a $N_q+ I_{\infty}= M$ et l’endomorphisme de $M/N_q$ déduit de $u$ par passage aux quotients est surjectif.

#### Remarque 2 {#alg-viii-s2-n2-rem-2 .statement tag=001Z}

Supposons que M soit somme directe de deux sous-modules N et I, stables par $u$, et que $u$ induise un endomorphisme nilpotent $u_N$ de N et un automorphisme de I. On a alors $N_{\infty}= N$ et $I_{\infty}= I$ et les suites $(N_p)$ et $(I_p)$ sont stationnaires. De plus, les entiers suivants sont égaux :

$\alpha )$ le plus petit entier $p\geqslant 0$ tel que $N_p= N_{\infty}$;

$\beta )$ le plus petit entier $q\geqslant 0$ tel que $I_q= I_{\infty}$;

$\gamma )$ le plus petit entier $r\geqslant 0$ tel que $(u_N)^r= 0$.

#### Remarque 3 {#alg-viii-s2-n2-rem-3 .statement tag=0020}

L’hypothèse de l’assertion a) est vérifiée si le A-module M est noethérien, l’hypothèse de l’assertion b) est vérifiée si M est artinien ; d’après la prop. 1 de VIII, p. 2, l’hypothèse de l’assertion c) est vérifiée si M est de longueur finie.

#### Corollaire 1 {#alg-viii-s2-prop-2-cor-1 .statement tag=0021}

Soit A un anneau et soit M un A-module.

a) Si le module M est noethérien, tout endomorphisme surjectif de M est bijectif.

b) Si le module M est artinien, tout endomorphisme injectif de M est bijectif.

c) Si le module M est de longueur finie, tout endomorphisme injectif ou surjectif de M est bijectif.

d) Si l’anneau A est commutatif et le A-module M de type fini, tout endomorphisme surjectif de M est bijectif.

Soit $u$ un endomorphisme du A-module M. Adoptons les notations introduites au début de ce numéro. Si l’endomorphisme $u$ est surjectif, on a $I_{\infty}= M$. L’assertion a) résulte alors de la prop. 2, a) et de la remarque 3. De même si l’endomorphisme $u$ est injectif, on a $N_{\infty}= 0$. L’assertion b) résulte donc de la prop. 2, b) et de la remarque 3. L’assertion c) découle aussitôt de a) et b).

Supposons maintenant l’anneau A commutatif, le A-module M de type fini et l’endomorphisme $u$ surjectif. Démontrons que $u$ est injectif. Soit $x$ un élément de M tel que $u(x) = 0$. Choisissons une famille génératrice finie $(x_i)_{i\in I}$ du A-module M et, pour tout $i\in I$, un élément $y_i$ de M tel que $u(y_i) =x_i$. Il existe des familles $(a_i)_{i\in I}$, $(b_{ij})_{(i,j)\in I\times I}$ et $(c_{ij})_{(i,j)\in I\times I}$ d’éléments de A telles que l’on ait

$$
x=\sum_{i\in I}a_ix_i,y_j=\sum_{i\in I}b_{ij}x_i,u(x_j) =\sum_{i\in I}c_{ij}x_i
$$

pour tout $j\in I$. Soit $A'$ un sous-anneau noethérien de A contenant les éléments $a_i$, $b_{ij}$ et $c_{ij}$ (VIII, p. 12, cor. 3). Soit $M'$ le sous-A$'$-module de M engendré par la famille $(x_i)_{i\in I}$. On a $u(x_j)\in M',y_j\in M'$, et $u(y_j) =x_j$ pour tout $j\in I$, donc $u$ définit par restriction un endomorphisme surjectif $u'$ du $A'$-module $M'$. Comme l’anneau $A'$ est noethérien, le $A'$-module de type fini $M'$ est noethérien (VIII, p. 7, prop. 4 a)). D’après a), l’endomorphisme $u'$ de $M'$ est bijectif. Par construction, $x$ appartient à $M'$, et l’on a $u'(x) =u(x) = 0$. On a donc $x= 0$, ce qui prouve d).

#### Corollaire 2 {#alg-viii-s2-prop-2-cor-2 .statement tag=0022}

Dans un anneau noethérien à gauche, tout élément inversible à droite ou à gauche est inversible.

Considérons en effet des éléments $x, y$ d’un anneau noethérien à gauche A tels que $xy= 1$. Notons $\boldsymbol{\delta }(x)$ et $\boldsymbol{\delta }(y)$ les endomorphismes $a\rightarrow ax$ et $a\rightarrow ay$ du A-module $A_s$. On a $\boldsymbol{\delta }(y)\circ \boldsymbol{\delta }(x) = 1_{A_s}$, donc $\boldsymbol{\delta }(y)$ est surjectif. D’après le cor. 1, a), $\boldsymbol{\delta }(y)$ est bijectif. L’endomorphisme $\boldsymbol{\delta }(x)$ est alors la bijection réciproque de $\boldsymbol{\delta }(y)$, et l’on a $yx= (\boldsymbol{\delta }(x)\circ \boldsymbol{\delta }(y))(1) = 1$, d’où le corollaire.

### 3. Modules indécomposables et modules primordiaux

Soit A un anneau. Rappelons la définition suivante (VII, p. 23, déf. 3) :

#### Définition 2 {#alg-viii-s2-def-2 .statement tag=0023}

On dit qu’un A-module M est indécomposable s’il n’est pas somme directe d’une famille de sous-modules distincts de 0 et de M.

Compte tenu du corollaire de II, p. 19, les conditions suivantes sont équivalentes :

a) Le A-module M est indécomposable ;

b) Le A-module M n’est pas nul et tout sous-module facteur direct de M est égal à 0 ou M ;

c) Le A-module M n’est pas nul et l’anneau End$_A(M)$ ne contient pas d’élément idempotent distinct de 0 et $1_M$;

En particulier, comme l’anneau des endomorphismes du A-module $A_s$ est isomorphe à l’anneau opposé de A, on voit que le A-module $A_s$ est indécomposable si et seulement si l’anneau A n’est pas nul, et que ses seuls éléments idempotents sont 0 et 1.

#### Exemple {#alg-viii-s2-n3-exa-1 .statement tag=0024}

Supposons l’anneau A principal. Les A-modules de type fini indécomposables sont les A-modules isomorphes soit à A, soit à $A/p^nA$, où $p$ est un élément extrémal de A et $n$ un entier $>0$ (VII, p. 23, prop. 8).

#### Proposition 3 {#alg-viii-s2-prop-3 .statement tag=0025}

Un A-module M noethérien ou artinien est somme directe d’une famille finie de sous-modules indécomposables.

Démontrons d’abord que tout sous-module non nul P de M possède un facteur direct indécomposable. Dans le cas contraire, tout sous-module facteur direct de P serait décomposable ; procédant par récurrence, on construirait pour tout $n\in \mathbf{N}$des sous-modules non nuls $N'_n$ et $N''_n$ de P tels que $P = N'_0\oplus N''_0$ et $N'_{n-1}= N'_n\oplus N''_n$ pour $n\geqslant 1$. Mais alors la suite des sous-modules $N''_0+\cdots + N''_n$ serait strictement croissante, et celle des sous-modules $N'_n$ serait strictement décroissante. Le module M ne serait ni noethérien, ni artinien, contrairement à l’hypothèse faite.

Supposons maintenant que M ne soit pas somme directe d’une famille finie de sous-modules indécomposables. On peut construire par récurrence des sous-modules indécomposables $P''_n$ de M et des sous-modules non nuls $P'_n$ de M pour tout $n\in \mathbf{N}$ tels que $M = P'_0\oplus P''_0$ et $P'_{n-1}= P'_n\oplus P''_n$ pour $n\geqslant 1$. En effet, M n’est pas nul et la première partie de la démonstration fournit $P'_0$ et $P''_0$. Les modules $P'_k$ et $P''_k$ étant définis pour $k < n$, il existe d’après la première partie de la démonstration des sous-modules $P'_n$ et $P''_n$ tels que $P'_{n-1}= P'_n\oplus P''_n$ avec $P''_n$ indécomposable. La relation $M = P'_n\oplus P''_0\oplus  \cdots  \oplus P''_n$ entraîne alors que $P'_n\not= 0$, car M n’est pas somme directe d’une famille finie de modules indécomposables.

La suite de sous-modules $P''_0+. . .P''_n$ est strictement croissante et la suite de sous-modules $P'_n$ strictement décroissante. Ceci contredit l’hypothèse que M est noethérien ou artinien.

La question de l’unicité de la décomposition d’un module en somme directe de sous-modules indécomposables sera étudiée au numéro suivant.

#### Définition 3 {#alg-viii-s2-def-3 .statement tag=0026}

On dit qu’un module est primordial si l’anneau de ses endomorphismes est local.

Par définition, un anneau local n’est pas réduit à 0 ; par suite, un module primordial n’est pas nul. De plus, le A-module $A_s$ est primordial si et seulement si l’anneau A est local.

#### Proposition 4 {#alg-viii-s2-prop-4 .statement tag=0027}

a) Un module primordial est indécomposable.

b) Un module indécomposable de longueur finie est primordial.

Soit M un A-module. Supposons M primordial ; soit $e$ un idempotent de l’anneau local End$_A(M)$. Comme $e^2=e$, ou bien $e$ est inversible et l’on a $e= 1$, ou bien $1-e$ est inversible et l’on a $e= 0$. Ceci prouve que M est indécomposable (VIII, p. 27).

Supposons maintenant que M soit indécomposable et de longueur finie. D’après la prop. 2, c) de VIII, p. 25, tout endomorphisme de M est inversible ou nilpotent ; l’anneau End$_A(M)$ est donc local d’après l’exemple 2 de VIII, p. 24.

Le $\mathbf{Z}$-module $\mathbf{Z}$est indécomposable, noethérien, mais non artinien. L’anneau de ses endomorphismes est isomorphe à $\mathbf{Z}$, donc n’est pas local. Par suite, $\mathbf{Z}$n’est pas un $\mathbf{Z}$-module primordial.

$*$ Soit $p$ un nombre premier. L’anneau des endomorphismes du $\mathbf{Z}$-module $\mathbf{Q}_p/\mathbf{Z}_p$ est isomorphe à l’anneau local $\mathbf{Z}_p$ (cf. VII, p. 62, exercice 13) ; c’est donc un $\mathbf{Z}$-module primordial.

Un module injectif est indécomposable si et seulement s’il est primordial (X, p. 21, prop. $14).*$

### 4. Modules semi-primordiaux

#### Définition 4 {#alg-viii-s2-def-4 .statement tag=0028}

On dit qu’un module est semi-primordial s’il est somme directe d’une famille de sous-modules primordiaux.

#### Exemple 1 {#alg-viii-s2-n4-exa-1 .statement tag=00SE}

$*$Tout module simple est primordial (VIII, p. 41) ; tout module semi-simple est donc semi-primordial (VIII, p. 51, déf 1).

#### Exemple 2 {#alg-viii-s2-n4-exa-2 .statement tag=01L7}

Si A est un anneau noethérien à gauche, tout A-module injectif est semi-primordial (X, p. 21, prop. 14 et p. 22, th. 3, b)). $*$

#### Théorème 1 {#alg-viii-s2-thm-1 .statement tag=00RX}

Soient A un anneau, L un A-module primordial et M un A-module semi-primordial. Il existe un unique cardinal, noté [M : L], possédant la propriété suivante :

Pour toute décomposition $M =\bigoplus_{i\in I}M_i$ de M en somme directe de modules primordiaux, l’ensemble des indices $i\in I$tels que $M_i$ soit isomorphe à L a pour cardinal [M : L].

La démonstration repose sur les quatre lemmes suivants.

#### Lemme 1 {#alg-viii-s2-lem-1 .statement tag=0029}

Soient M un A-module, $M'$ un sous-module primordial de M et $M''$ un sous-module de M supplémentaire de $M'$. Soit $u$ un endomorphisme de M. Alors $u$ ou $1_M-u$ induit un isomorphisme de $M'$ sur un sous-module de M supplémentaire de $M''$.

Soit $p$ la projection de M sur $M'$ de noyau $M''$ et soit $v$ la restriction de $p\circ u$ à $M'$. Supposons d’abord que $v$ soit un automorphisme de $M'$. Comme $v$ est injectif, la restriction de $u$ à $M'$ est injective et l’on a $u(M')\cap M''= 0$. Comme $v$ est surjectif, on a $u(M')\oplus M''= M$. Par suite, $u$ induit un isomorphisme de $M'$ sur un sous-module supplémentaire de $M''$ dans M. Supposons maintenant que $v$ ne soit pas un automorphisme de $M'$. Alors $1_{M'}-v$ est un automorphisme de $M'$, puisque $M'$ est primordial. Or $1_{M'}-v$ est la restriction à $M'$ de $p\circ (1_M-u)$. Le raisonnement précédent démontre que $1_M-u$ induit un isomorphisme de $M'$ sur un sous-module de M supplémentaire de $M''$.

#### Lemme 2 {#alg-viii-s2-lem-2 .statement tag=002A}

Soit M un A-module, somme directe d’une famille $(M_i)_{i\in I}$ de sous-modules primordiaux, et soit $u$ un endomorphisme de M. Posons $v= 1_M-u$ et $M_J=\bigoplus_{i\in J}M_i$ pour toute partie J de I. Alors l’une des deux propriétés suivantes est satisfaite :

a) Il existe un indice $i\in I$tel que $u$ induise un isomorphisme de $M_i$ sur un sous-module facteur direct de M.

b) Pour toute partie finie J de I$,v$ induit un isomorphisme de $M_J$ sur un sous-module supplémentaire de $M_{I-J}$.

Si la propriété b) est satisfaite, $v$ est injectif.

Supposons que la propriété a) soit fausse et établissons la propriété b) par récurrence sur le cardinal de J. Il n’y a rien à prouver si $J =\emptyset$. Supposons donc J non vide, choisissons un élément $i$ de J et posons $J'= J-\{i\}$. Par l’hypothèse de récurrence, $v$ induit un isomorphisme de $M_{J'}$ sur un sous-module de M supplémentaire de $M_{I-J'}= M_{I-J}\oplus M_i$; par suite, le sous-module $M''=v(M_{J'})\oplus M_{I-J}$ est supplémentaire de $M_i$. D’après le lemme 1 et l’hypothèse faite sur $u$, l’endomorphisme $v$ induit un isomorphisme de $M_i$ sur un sous-module de M supplémentaire de $M''$; par suite, $v$ induit un isomorphisme de $M_J= M_i\oplus M_{J'}$ sur un sous-module supplémentaire de $M_{I-J}$.

La dernière assertion résulte de ce que M est réunion des sous-modules $M_J$, où J parcourt l’ensemble des parties finies de I.

#### Lemme 3 {#alg-viii-s2-lem-3 .statement tag=002B}

Soient M un A-module, somme directe d’une famille $(M_i)_{i\in I}$ de sous-modules primordiaux, et $p$ un projecteur non nul de M. Il existe un indice $i\in I$tel que $p$ induise un isomorphisme de $M_i$ sur un sous-module facteur direct de $p(M)$.

Comme $p$ n’est pas nul, $1_M-p$ n’est pas injectif. D’après le lemme 2, il existe un indice $i\in I$ tel que $p$ induise un isomorphisme de $M_i$ sur un sous-module facteur direct de M. Tout projecteur de M d’image $p(M_i)$ définit par restriction un projecteur de $p(M)$ d’image $p(M_i)$, donc $p(M_i)$ est un sous-module facteur direct de $p(M)$.

#### Lemme 4 {#alg-viii-s2-lem-4 .statement tag=002C}

Soient M un A-module, somme directe d’une famille $(M_i)_{i\in I}$ de sous-modules primordiaux, L un A-module primordial et N un sous-module facteur direct de M. On suppose que N est somme directe d’une famille $(N_j)_{j\in J}$ de sous-modules isomorphes à L et l’on note $I_L$ l’ensemble des indices $i\in I$tels que $M_i$ soit isomorphe à L. On a alors

(1) Card(J) $\leqslant$ Card(I$_L)$.

Soit $N_0$ un sous-module de M supplémentaire de N. Le module M est somme directe de $N_0$ et de la famille $(N_j)_{j\in J}$. Pour tout $j\in J$, notons $p_j$ le projecteur de M d’image $N_j$ associé à cette décomposition (II, p. 18, prop. 12). Pour tout $i\in I$, notons $J(i)$ l’ensemble des indices $j\in J$ tels que $p_j$ induise un isomorphisme de $M_i$ sur $N_j$. Cet ensemble est fini : en effet, si $x$ est un élément non nul de $M_i$ et K une partie finie de J telle que $x$ appartienne à $N_0+\sum_{k\in K}N_k$, on a $p_j(x) = 0$ pour $j\in J$ - K, de sorte que $J(i)$ est contenu dans K.

Soit $j\in J$. D’après le lemme 3, il existe un indice $i\in I$ tel que $p_j$ induise un isomorphisme de $M_i$ sur un sous-module facteur direct de $N_j$. Comme $M_i$ n’est pas nul et que $N_j$ est primordial, donc indécomposable (VIII, p. 28, prop. 4), on a $p_j(M_i) = N_j$, et $j$ appartient à $J(i)$. Comme le module $M_i$ est isomorphe à $N_j$, donc à L, l’indice $i$ appartient à $I_L$. Cela démontre que J est réunion de la famille d’ensembles finis $(J(i))_{i\in I_L}$. Si l’ensemble J est infini, l’ensemble $I_L$ est infini, et l’on a (E, III, p. 49, cor. 3)

Card(J) $\leqslant \sum_{i\in I_L}$ Card(J($i$))$\leqslant$ Card(I$_L)$.

Supposons maintenant l’ensemble J fini, et démontrons le lemme par récurrence sur le cardinal de J. Si J est vide, il n’y a rien à prouver. Supposons donc J non vide et choisissons un élément $j$ de J. D’après ce qui précède, il existe un indice $i\in I_L$ tel que $p_j$ induise un isomorphisme de $M_i$ sur $N_j$. Posons $I'= I-\{i\}$ et $J'= J-\{j\}$. Le module M est somme directe de $M_i$ et du noyau de $p_j$. Il est aussi somme directe de $M_i$ et du sous-module $M'=\oplus_{i'\in I'}M_{i'}$. Il existe donc (II, p. 20, cor. de la prop. 13) un$(\sum)$ isomorphisme $\varphi$ de Ker$p_j= N_0\oplus_{j'\in J'}N_{j'}$ sur $M'$. Posons $N'=\varphi_{j'\in J'}N_{j'}$. Le sous-module $N'$ est facteur direct de $M'$ et est somme directe de la famille $(\varphi (N_{j'}))_{j'\in J'}$ de sous-modules primordiaux isomorphes à L. Appliquons l’hypothèse de récurrence à $M'$ et $N':$ on a Card(J$')\leqslant$ Card(I$_L-\{i\})$, d’où l’inégalité (1).

Prouvons le théorème 1. Soient $(M_i)_{i\in I}$ et $(N_j)_{j\in J}$ deux familles de sous-modules primordiaux dont M soit la somme directe. Soit $I_L$ (resp. $J_L)$ l’ensemble des $i\in I$ (resp. $j\in J)$ tels que $M_i$ (resp. $N_j)$ soit isomorphe à L. On a Card(J$_L)\leqslant$ Card(I$_L)$ d’après le lemme 4. En échangeant les rôles de I et J on obtient l’inégalité opposée, d’où le théorème.

Le cardinal [M : L] défini dans la théorème 1 est appelé multiplicité primordiale de L dans M.

#### Corollaire 1 {#alg-viii-s2-lem-4-cor-1 .statement tag=002D}

Soient M et N des modules semi-primordiaux. Pour que M et N soient isomorphes, il faut et il suffit que l’on ait [M : L] = [N : L] pour tout module primordial L.

#### Corollaire 2 {#alg-viii-s2-lem-4-cor-2 .statement tag=00QY}

Soit M un module semi-primordial. Soient $(M_i)_{i\in I}$ et $(M'_j)_{j\in J}$ des familles de sous-modules primordiaux de M telles que

$$
M =\bigoplus_{i\in I}M_i=\bigoplus_{j\in J}M'_j
$$

Il existe alors un automorphisme $u$ de M et une bijection $\varphi$ de I sur J tels que l’on ait $u(M_i) = M'_{\varphi(i)}$ pour tout $i\in I$.

Pour tout module primordial L, soit $I_L$ (resp. $J_L)$ l’ensemble des indices $i\in I$ (resp. $j\in J)$ tels que $M_i$ (resp. $M'_j)$ soit isomorphe à L. Les ensembles non vides de la forme $I_L$ (resp. $J_L)$ forment une partition de I (resp. J) et l’on a, pour tout L

Card(I$_L) =$ Card(J$_L) = [M : L]$,

d’où le cor. 2.

#### Corollaire 3 {#alg-viii-s2-lem-4-cor-3 .statement tag=002E}

Soient M, N et P des modules semi-primordiaux. On suppose que $M\oplus P$est isomorphe à $N\oplus P$, et que [P : L] est fini pour tout module primordial L. Alors M et N sont isomorphes.

On a par hypothèse

[M : L] + [P : L] = [N : L] + [P : L]

pour tout module primordial L. Comme [P : L] est fini, il résulte par récurrence de (E, III, p. 28, prop. 8) qu’on a [M : L] = [N : L] pour tout module primordial L. Les modules M et N sont donc isomorphes d’après le corollaire 1.

#### Corollaire 4 {#alg-viii-s2-lem-4-cor-4 .statement tag=002F}

Soient M et N des modules semi-primordiaux. On suppose qu’il existe un entier $d >0$tel que $M^d$ soit isomorphe à $N^d$. Alors les modules M et N sont isomorphes.

Soit L un module primordial. Par hypothèse, on a

$$
d[M : L] =d[N : L]
$$

On en déduit l’égalité [M : L] = [N : L] : en effet, on a $d\mathfrak{a}=\mathfrak{a}$ pour tout cardinal infini $\mathfrak{a}$ (E, III, p. 49, cor. 4). Les modules M et N sont alors isomorphes d’après le cor. 1.

#### Corollaire 5 {#alg-viii-s2-lem-4-cor-5 .statement tag=002G}

Soit M un module semi-primordial, somme directe d’une famille finie $(M_i)_{i\in I}$ de sous-modules primordiaux. Pour toute partie J de I, notons $M_J=$ $\bigoplus_{i\in J}M_i$. Soit N un sous-module facteur direct de M.

a) Il existe une partie J de I telle que $M_J$ soit un sous-module supplémentaire de N.

b) Soit J une partie de I. Si $M_J$ est un supplémentaire de N, alors le module N est isomorphe à $M_{I-J}$ et est semi-primordial.

Notons K l’ensemble des indices $i\in I$ tels que $N\cap M_i= 0$ et raisonnons par récurrence sur le cardinal de K. Le corollaire est clair si M = N . Supposons $M\not= N$. Soit $p$ un projecteur de M de noyau N. Notons P son image. Elle n’est pas nulle, et d’après le lemme 3, il existe $j\in I$ tel que $p$ induise un isomorphisme de $M_j$ sur un sous-module facteur direct de P. On a $N\cap M_j= 0$. Posons $N'= N\oplus M_j$. On a $N'= N\oplus p(M_j)$. Un sous-module supplémentaire de $p(M_j)$ dans P est aussi supplémentaire de $N'$ dans M, de sorte que $N'$ est un sous-module facteur direct de M. L’ensemble des indices $i\in I$ tels que $N'\cap M_i= 0$ est contenu dans K$-\{j\}$. D’après l’hypothèse de récurrence, il existe une partie $J'$ de I telle que $M_{J'}$ soit un sous-module supplémentaire de $N'$ dans M. Posons $J = J'\cup  \{j\}$. Alors $M_J$ est un sous-module supplémentaire de N dans M.

Soit J une partie de I telle que $M_J$ soit un sous-module supplémentaire de M dans N. Comme $M_J$ est également supplémentaire de $M_{I-J}$, les modules N et $M_{I-J}$ sont isomorphes et N est semi-primordial.

#### Corollaire 6 {#alg-viii-s2-lem-4-cor-6 .statement tag=002H}

Tout module projectif de type fini sur un anneau local est libre[^1].

Soit A un anneau local. Le A-module $A_s$ est primordial (VIII, p. 28). Si M est un A-module projectif de type fini, il existe un A-module N et un entier positif $n$ tel que $M\oplus N$ soit isomorphe à $A^n_s$ (II, p. 40, cor. 1). Il résulte du corollaire 5 que le module M est lui-même isomorphe à $A^m_s$ pour un entier $m$ tel que $0\leqslant m\leqslant n$, donc est libre.

#### Remarque {#alg-viii-s2-n4-rem-1 .statement tag=002I}

Soient M et $M'$ des A-modules semi-primordiaux. Il résulte aussitôt du lemme 4 de VIII, p. 31 que $M'$ est isomorphe à un sous-module facteur direct de M si et seulement si l’on a $[M': L]\leqslant [M : L]$ pour tout A-module primordial L. En particulier, si L est un A-module primordial, [M : L] est le plus grand des cardinaux $\mathfrak{a}$ pour lesquels il existe un sous-module facteur direct de M isomorphe à $L^{(\mathfrak{a})}$.

☡ La relation [M : L] = 0 signifie donc qu’il n’existe aucun sous-module facteur direct de M isomorphe à L. Ceci n’exclut pas qu’il existe un sous-module de M isomorphe à L ; il suffit de considérer l’exemple où $A = \mathbf{Z}, L = \mathbf{Z}/2\mathbf{Z}$et $M = \mathbf{Z}/4\mathbf{Z} :$ les $\mathbf{Z}$-modules L et M sont primordiaux, non isomorphes, d’où [M : L] = 0 et L est isomorphe au sous-module $2\mathbf{Z}/4\mathbf{Z}$de M.

### 5. Structure des modules de longueur finie

#### Théorème 2 {#alg-viii-s2-thm-2 .statement tag=00RY}

Soient A un anneau et M un A-module de longueur finie.

a) Il existe une famille finie $(M_i)_{i\in I}$ de sous-modules indécomposables de M telle que $M =\bigoplus_{i\in I}M_i$ et le module M est semi-primordial.

b) Soient $(M_i)_{i\in I}$ et $(M'_j)_{j\in J}$ deux familles finies de sous-modules indécomposables de M telles que $M =\bigoplus_{i\in I}M_i=\bigoplus_{j\in J}M'_j$. Il existe une bijection $\sigma$ de I sur J et un automorphisme $u$ de M tels que l’on ait $u(M_i) = M'_{\sigma(i)}$ pour tout $i\in I$.

c) Soit N un sous-module facteur direct de M et soit $(M_i)_{i\in I}$ une famille finie de sous-modules indécomposables de M dont M soit somme directe. Il existe une partie J de I telle que $\bigoplus_{i\in I-J}M_i$ soit un supplémentaire de N. Le module N est isomorphe à $\bigoplus_{j\in J}M_j$.

d) Soit N un A-module. S’il existe un entier $d >0$tel que les modules $M^d$ et $N^d$ soient isomorphes, alors les modules M et N sont isomorphes.

e) Soient N et P des A-modules de longueur finie. Si les modules $M\oplus P$et $N\oplus P$ sont isomorphes, alors M et N sont isomorphes.

Un module de longueur finie est à la fois artinien et noethérien (VIII, p. 2, prop. 1). De plus, pour un module de longueur finie, il revient au même d’être indécomposable ou primordial (VIII, p. 28, prop. 4). L’assertion a) résulte alors de la prop. 3 de VIII, p. 28. Les assertions b), c) et e) découlent respectivement des corollaires 2, 5 et 3 du th. 1 de VIII, p. 29. Enfin, l’assertion d) résulte du cor. 4 de VIII, p. 32, puisque sous les hypothèses de d) le module N est de longueur finie et donc semi-primordial par a).

#### Théorème 3 {#alg-viii-s2-thm-3 .statement tag=002J}

Soient K un corps commutatif, A une K-algèbre, M et N des A-modules de longueur finie. Soit $K'$ une K-algèbre commutative non nulle telle que les $A_{(K')}$-modules $M_{(K')}$ et $N_{(K')}$ soient isomorphes. Alors les A-modules M et N sont isomorphes.

a) Supposons d’abord que l’algèbre $K'$ soit de degré fini $d$ sur K. Alors le A-module $M_{(K')}$ est isomorphe à $M^d$ et le A-module $N_{(K')}$ à $N^d$, de sorte que les A-modules $M^d$ et $N^d$ sont isomorphes. D’après le th. 2, d) , les A-modules M et N sont isomorphes.

b) Supposons maintenant que la K-algèbre $K'$ soit engendrée par un nombre fini d’éléments. Choisissons un idéal maximal $\mathfrak{m}$ de $K'$ et posons $K''= K'/\mathfrak{m}$. En vertu du théorème des zéros de Hilbert (VIII, p. 451, cor. 1 du th. 1), $K''$ est une extension de degré fini de K. Par extension des scalaires de $K'$ à $K''$, on déduit de l’isomorphisme $A_{(K')}$-linéaire $M_{(K')}\rightarrow N_{(K')}$ un isomorphisme $A_{(K'')}$-linéaire $M_{(K'')}\rightarrow N_{(K'')}$. D’après la partie a) de la démonstration, les A-modules M et N sont isomorphes.

c) Traitons enfin le cas général. Soient $u: M_{(K')}\rightarrow N_{(K')}$ un isomorphisme de $A_{(K')}$-modules et $v: N_{(K')}\rightarrow M_{(K')}$ l’isomorphisme réciproque. Notons $\mathscr{E}$ l’ensemble des sous-K-algèbres de $K'$ qui sont engendrées par un nombre fini d’éléments. Si E est une telle sous-algèbre, $A_{(E)}$ s’identifie à un sous-anneau de $A_{(K')}$ et $M_{(E)}, N_{(E)}$ à des sous-A$_{(E)}$-modules de $M_{(K')}$ et $N_{(K')}$ (II, p. 108) ; de plus, $M_{(K')}$ et $N_{(K')}$ sont réunions des familles filtrantes croissantes $(M_{(E)})_{E\in\mathscr{E}}$ et $(N_{(E)})_{E\in\mathscr{E}}$ respectivement. Les A-modules M et N sont de longueur finie, donc de type fini ; soient S une partie génératrice finie du A-module M et T une partie génératrice finie du A-module N. Il existe une K-algèbre $E\in \mathscr{E}$ telle que l’on ait $u(1\otimes s)\in N_{(E)}$ pour tout $s\in S$ et $v(1\otimes t)\in M_{(E)}$ pour tout $t\in T$. Il en résulte par linéarité que l’on a $u(M_{(E)})\subset N_{(E)}$ et $v(N_{(E)})\subset M_{(E)}$. Les applications $u$ et $v$ induisent alors des bijections réciproques l’une de l’autre de $M_{(E)}$ dans $N_{(E)}$, et de $N_{(E)}$ dans $M_{(E)}$. Ces bijections sont clairement $A_{(E)}$-linéaires. Ainsi les $A_{(E)}$-modules $M_{(E)}$ et $N_{(E)}$ sont isomorphes. D’après la partie b) de la démonstration, les A-modules M et N sont isomorphes.

#### Remarque {#alg-viii-s2-n5-rem-1 .statement tag=002K}

Soient E et F deux espaces vectoriels de dimension finie sur un corps commutatif K et soit $K'$ une extension de K. Soient $u$ un endomorphisme de $E,v$ un endomorphisme de $F,u_{(K')}$ et $v_{(K')}$ les endomorphismes de $E_{(K')}$ et $F_{(K')}$ qu’on en déduit par extension des scalaires. Il résulte des corollaires 1 et 2 de VII, p. 32 que les endomorphismes $u$ et $v$ sont semblables si et seulement si les endomorphismes $u_{(K')}$ et $v_{(K')}$ le sont. Cela résulte aussi du théorème 3 ci-dessus, appliqué à l’algèbre A = K[X] et aux A-modules $M = E_u$ et $N = F_v$ (VII, p. 28).

## EXERCICES {#alg-viii-s2-exercises}

See the [exercises for § 2](exercises/s2/).

[^1]: On peut démontrer que tout module projectif sur un anneau local est libre (VIII, p.39, exerc. 18).
