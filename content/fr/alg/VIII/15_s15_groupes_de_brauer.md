---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 15
section_title: Groupes de Brauer
lang: fr
source: alg-viii-fr
book_pages: A VIII.273-A VIII.280
pdf_pages: 0276-0283
extraction: native
subsections:
    - "no": 1
      title: Classes d’algèbres
      page: 273
      pdf_page: 276
    - "no": 2
      title: Définition du groupe de Brauer
      page: 274
      pdf_page: 277
    - "no": 3
      title: Changement de corps
      page: 276
      pdf_page: 279
    - "no": 4
      title: Exemples de groupes de Brauer
      page: 279
      pdf_page: 282
statements: 12
exercises: 2
content_sha256: 31c7c5c563c0e9fa5d6f809acc1899275f9c821ac5577480e6394ffe2c1f4cef
---

## § 15. GROUPES DE BRAUER

Dans ce paragraphe, la lettre K désigne un corps commutatif.

### 1. Classes d’algèbres

Notons Iso$_K(A,B)$ la relation

« A et B sont des K-algèbres de degré fini isomorphes. »

C’est une relation d’équivalence par rapport à A et B. Soit A une K-algèbre de degré fini ; on appelle classe de A et l’on note cl(A) (ou parfois cl$_K$(A)), la classe d’objets équivalents à A pour la relation Iso$_K$ (E, II, p. 47). Par définition, cl(A) est une K-algèbre isomorphe à A ; pour que deux K-algèbres de degré fini aient la même classe, il faut et il suffit qu’elles soient isomorphes.

Notons $\mathscr{A}$ l’ensemble des couples $(W, \mu )$, où W est un sous-espace vectoriel de $K^{(\mathbf{N})}$, de dimension finie sur K, et $\mu$ une application K-bilinéaire de $W\times W$ dans W, qui fait de W une K-algèbre (associative et unifère). Toute K-algèbre de degré fini est isomorphe à une telle algèbre. D’après loc. cit., la relation

« $\alpha$ est une classe de K-algèbres de degré fini »

est donc collectivisante en $\alpha$ (E, II, p. 3). On note $\mathscr{C}_K$ l’ensemble des classes des K-algèbres de degré fini.

#### Proposition 1 {#alg-viii-s15-prop-1 .statement tag=00HV}

L’ensemble $\mathscr{C}_K$, muni de la loi de composition donnée par $(\alpha , \beta )\rightarrow$ cl($\alpha \otimes_K\beta$ ), est un monoïde commutatif. L’élément neutre de $\mathscr{C}_K$ est la classe $\varepsilon$ de la K-algèbre K. De plus, si A et B sont des K-algèbres de degré fini, on a la relation

(1) cl(A $\otimes_KB) =$ cl(A) cl(B).

Soient A, B et C des K-algèbres de degré fini, de classes respectives $\alpha ,\beta$ et $\gamma$. Les K-algèbres A et $\alpha$ sont isomorphes, ainsi que B et $\beta$; donc les K-algèbres $A\otimes_KB$ et $\alpha \otimes_K\beta$ sont isomorphes et l’on a cl(A $\otimes_KB) =$ cl($\alpha \otimes_K\beta$ ), d’où la formule (1). Il en résulte que $(\alpha \beta )\gamma$ est la classe de la K-algèbre $(A\otimes_KB)\otimes_KC$, et $\alpha (\beta \gamma )$ celle de la K-algèbre $A\otimes_K(B\otimes_KC)$. Or ces K-algèbres sont isomorphes (III, p. 34), d’où l’égalité $(\alpha \beta )\gamma =\alpha (\beta \gamma )$. De manière analogue, la relation $\alpha \varepsilon =\varepsilon \alpha =\alpha$ résulte de ce que les K-algèbres $A\otimes_KK, K\otimes_KA$ et A sont isomorphes, et la relation $\alpha \beta =\beta \alpha$ de ce que les algèbres $A\otimes_KB$ et $B\otimes_KA$ sont isomorphes.

Dans l’ensemble $\mathscr{C}_K$, la relation « $\alpha$ et $\beta$ sont des algèbres équivalentes au sens de Morita » est une relation d’équivalence (VIII, p. 96) ; elle est compatible avec la loi de composition de $\mathscr{C}_K$ d’après la prop. 13, d) de VIII, p. 107. On note $\mathscr{M}_K$ le monoïde quotient de $\mathscr{C}_K$ par cette relation d’équivalence et $\varphi$ l’homomorphisme canonique de $\mathscr{C}_K$ sur $\mathscr{M}_K$. Pour toute K-algèbre A de degré fini, on note [A] l’image de cl(A) par $\varphi$. Si A et B sont des K-algèbres de degré fini, on a [A] = [B] si et seulement si les K-algèbres A et B sont équivalentes au sens de Morita ; de plus, on a la relation

$$
[A\otimes_KB] = [A][B] \tag{2}
$$

dans le monoïde $\mathscr{M}_K$.

#### Lemme 1 {#alg-viii-s15-lem-1 .statement tag=00HW}

Soient A une K-algèbre de degré fini et D un corps de degré fini sur K. Pour que l’on ait [A] = [D] dans $\mathscr{M}_K$, il faut et il suffit qu’il existe un entier $n\geqslant 1$ tel que A soit isomorphe à $\mathbf{M}_n(D)$.

Par définition, on a [A] = [D] si et seulement s’il existe un $(A$, D)-bimodule inversible, c’est-à-dire (VIII, p. 97, th. 1) un espace vectoriel à droite V de dimension finie non nulle sur D muni d’un isomorphisme de K-algèbres $A\rightarrow$ End$_D(V)$. Le lemme 1 résulte de là.

### 2. Définition du groupe de Brauer

On note Br(K) l’ensemble des éléments de $\mathscr{M}_K$ de la forme [A], où A est une algèbre centrale, simple et de degré fini sur K.

#### Proposition 2 {#alg-viii-s15-prop-2 .statement tag=00HX}

L’ensemble Br(K) est l’ensemble des éléments inversibles de $\mathscr{M}_K$, l’inverse d’un élément [A] de Br(K) étant $[A^o]$. Par suite, la loi de composition du monoïde $\mathscr{M}_K$ munit Br(K) d’une structure de groupe commutatif.

Soit A une algèbre centrale, simple et de degré fini sur K. L’algèbre $A^o$ est centrale, simple et de degré fini sur K (VIII, p. 247). L’algèbre $A\otimes_KA^o$ est isomorphe à une algèbre de matrices $\mathbf{M}_n(K)$ où $n^2=$ dim(A) (VIII, p. 248, th. 1). On a donc $[A][A^o] = [A\otimes_KA^o] = [K]$ (lemme 1), ce qui démontre que [A] est inversible, d’inverse $[A^o]$.

Inversement, soit A une K-algèbre de degré fini. Si [A] est inversible dans $\mathscr{M}_K$, il existe une K-algèbre B de degré fini telle que [A][B] = [K] ; d’après la formule (2) et le lemme 1, cela signifie que la K-algèbre $A\otimes_KB$ est isomorphe à une algèbre de matrices $\mathbf{M}_n$(K), avec $n\geqslant 1$. D’après la remarque 1 de VIII, p. 247, l’algèbre A est alors centrale et simple.

#### Définition 1 {#alg-viii-s15-def-1 .statement tag=00HY}

Le groupe commutatif Br(K) est appelé le groupe de Brauer du corps K.

#### Lemme 2 {#alg-viii-s15-lem-2 .statement tag=00HZ}

Soient I et J des ensembles finis, $k$ un anneau commutatif, A et B des $k$-algèbres. Notons $\mathbf{M}_I(A)$la $k$-algèbre des matrices carrées de type $(I,I)$à éléments dans A et définissons de manière analogue les $k$-algèbres $\mathbf{M}_J(B)$et $\mathbf{M}_{I\times J}(A\otimes_KB)$. Il existe un unique isomorphisme de $k$-algèbres

$$
\varphi : \mathbf{M}_I(A)\otimes_k\mathbf{M}_J(B)\longrightarrow \mathbf{M}_{I\times J}(A\otimes_kB)
$$

tel que $\varphi ((a_{ii'})\otimes (b_{jj'}))$ soit la matrice dont l’élément d’indice $((i, j),(i', j'))$est $a_{ii'}\otimes b_{jj'}$.

L’existence d’une bijection $k$-linéaire $\varphi$ satisfaisant à la condition de l’énoncé résulte de la compatibilité du produit tensoriel aux sommes directes (II, p. 61, prop. 7) ; le fait que $\varphi$ est un homomorphisme d’algèbres résulte de la définition du produit matriciel.

#### Proposition 3 {#alg-viii-s15-prop-3 .statement tag=00I0}

Soient A et B des K-algèbres centrales, simples et de degré fini. Les propriétés suivantes sont équivalentes :

(i) On a [A] = [B] dans le groupe de Brauer Br(K) ;

(ii) Il existe un entier $t\geqslant 1$tel que la K-algèbre $A\otimes_KB^o$ soit isomorphe à l’algèbre de matrices $\mathbf{M}_t(K)$;

(iii) Il existe des entiers strictement positifs $r$ et $s$ tels que les K-algèbres $A\otimes_K\mathbf{M}_r(K)$et $B\otimes_K\mathbf{M}_s(K)$soient isomorphes ;

(iv) Il existe un corps D contenant K et des entiers $m\geqslant 1$et $n\geqslant 1$tels que A soit isomorphe à $\mathbf{M}_m(D)$et B à $\mathbf{M}_n(D)$.

Supposons que l’on ait [A] = [B]. Comme $[B^o]$ est l’inverse de [B] dans le groupe de Brauer, on a $[K] = [B][B^o] = [A][B^o] = [A\otimes_KB^o]$. D’après le lemme 1, il existe un entier $t\geqslant 1$ tel que les algèbres $A\otimes_KB^o$ et $\mathbf{M}_t(K)$ soient isomorphes. Donc (i) entraîne (ii).

Supposons (ii) satisfaite. Comme $B^o\otimes_KB$ est isomorphe à une algèbre de matrices $\mathbf{M}_s(K)$ avec $s\geqslant 1$ (VIII, p. 248, th. 1) l’algèbre $A\otimes_KB^o\otimes_KB$ est isomorphe d’une part à $A\otimes_K\mathbf{M}_s(K)$ et de l’autre à $\mathbf{M}_t(K)\otimes_KB$. Ainsi l’assertion (ii) entraîne l’assertion (iii).

Supposons (iii) satisfaite. D’après le théorème de Wedderburn (VIII, p. 116, th. 1), il existe des entiers $m\geqslant 1$ et $n\geqslant 1$ et des corps D et $D'$ de centre K et de degré fini sur K, tels que A soit isomorphe à $\mathbf{M}_m(D)$ et B à $\mathbf{M}_n(D')$. Alors l’algèbre $A\otimes_K\mathbf{M}_r(K)$ est isomorphe à $\mathbf{M}_{mr}(D)$ et $B\otimes_K\mathbf{M}_{r'}(K)$ est isomorphe à $\mathbf{M}_{nr'}(D')$ (lemme 2) ; d’après le cor. 2 de VIII, p. 117, les K-algèbres D et $D'$ sont isomorphes. Donc (iii) entraîne (iv).

Enfin, supposons (iv) satisfaite. Les algèbres A et D d’une part, B et D de l’autre, sont équivalentes au sens de Morita (VIII, p. 109, exemple 2). On a donc [A] = [B], de sorte que (iv) entraîne (i).

Lorsque les conditions équivalentes de la proposition sont satisfaites, on dit que les algèbres A et B sont semblables.

#### Corollaire {#alg-viii-s15-n2-cor-1 .statement tag=00I1}

Soient A et B des algèbres centrales, simples et de degré fini sur K. Pour que A et B soient isomorphes, il faut et il suffit qu’elles soient semblables et de même degré.

Cela résulte de l’équivalence des propriétés (i) et (iv) de la prop. 3 et du fait que dim$_K(\mathbf{M}_n(D)) =$ dim$_K(D)\times n^2$.

#### Proposition 4 {#alg-viii-s15-prop-4 .statement tag=00I2}

Soit $\mathscr{K}_K$ l’ensemble des classes de K-algèbres centrales de degré fini qui sont des corps. L’application $D\rightarrow [D]$de $\mathscr{K}_K$ dans Br(K) est bijective.

Cela résulte du lemme 1 de VIII, p. 274 et du théorème de Wedderburn (VIII, p. 116, th. 1).

### 3. Changement de corps

Soit L une extension du corps K. Soient A et B des K-algèbres de degré fini, les L-algèbres $A_{(L)}$ et $B_{(L)}$ sont de degré fini. Les L-algèbres $A_{(L)}\otimes_LB_{(L)}$ et $(A\otimes_KB)_{(L)}$ sont isomorphes (III, p. 35, prop. 3). La L-algèbre $K_{(L)}$ est isomorphe à L. Il existe donc un unique homomorphisme de monoïdes $\rho_{L/K}$ de $\mathscr{C}_K$ dans $\mathscr{C}_L$ tel que

(3) $\rho_{L/K}$(cl(A)) = cl(A$_{(L)})$

pour toute K-algèbre A de degré fini.

Si les K-algèbres A et B sont équivalentes au sens de Morita, il en est de même des L-algèbres $A_{(L)}$ et $B_{(L)}$ (VIII, p. 107, prop. 13 e)). Si la K-algèbre A est centrale, simple et de degré fini, il en est de même de la L-algèbre $A_{(L)}$ (VIII, p. 247, remarque 2). On déduit donc de $\rho_{L/K}$ un homomorphisme de groupes $r_{L/K}$ de Br(K) dans Br(L), tel que

$$
r_{L/K}([A]) = [A_{(L)}] \tag{4}
$$

pour toute K-algèbre A centrale, simple et de degré fini.

Soit M une extension du corps L. Compte tenu de la transitivité de l’extension des scalaires (III, p. 8), on a la relation

$$
r_{M/K}=r_{M/L}\circ r_{L/K} \tag{5}
$$

Soit A une K-algèbre centrale, simple et de degré fini et soit L une extension de K. On dit que L déploie A (ou neutralise A) si la L-algèbre $A_{(L)}$ est isomorphe à une algèbre de matrices $\mathbf{M}_n$(L), pour un entier $n\geqslant 1$. Avec les notations précédentes, il revient au même de dire que la classe de A dans Br(K) appartient au noyau de l’homomorphisme $r_{L/K}:$ Br(K) $\rightarrow$ Br(L).

Si B est semblable à A, alors A est déployée sur L si et seulement si B l’est.

Si A est déployée par L, elle est déployée par toute extension de L. D’après le th. 1 de VIII, p. 248, il existe une extension galoisienne de degré fini de K qui déploie A et toute clôture séparable de K déploie A.

#### Proposition 5 {#alg-viii-s15-prop-5 .statement tag=00I3}

Soit A une K-algèbre centrale, simple et de degré fini et soit L une extension de degré fini de K. Les conditions suivantes sont équivalentes :

(i) L’extension L déploie A ;

(ii) Il existe une K-algèbre centrale, simple, de degré fini, semblable à A, contenant une sous-algèbre commutative maximale isomorphe à L.

Prouvons que (ii) entraîne (i) ; il suffit de traiter le cas où L est une sous-algèbre commutative maximale de A. Soit $\psi : A\otimes_KA^o\rightarrow$ End$_K(A)$ l’isomorphisme canonique qui applique $a\otimes a'$ sur l’application K-linéaire $x\rightarrow axa'$ (VIII, p. 248, th. 1). Considérons A comme un espace vectoriel à droite sur L ; alors $\psi$ applique $A\otimes_KL$ dans le sous-espace End$_L(A)$ de End$_K(A)$ et induit par restriction un homomorphisme injectif de L-algèbres $\psi ': A\otimes_KL\rightarrow$ End$_L(A)$. Posons $n= [L : K]$. D’après VIII, p. 258, prop. 3, on a $[A : L] =n$ d’où $[A\otimes_KL : L] = [A : K] =n^2$ et [End$_L(A) : L] =n^2$. Par conséquent $\psi '$ est un isomorphisme, ce qui prouve (i).

La réciproque résulte du lemme suivant.

#### Lemme 3 {#alg-viii-s15-lem-3 .statement tag=00I4}

Soit A une K-algèbre centrale, simple et de degré fini et soit L une extension de degré fini de K qui déploie A. Soit V un $A_{(L)}$ module simple, si bien que le morphisme naturel $\varphi : A_{(L)}\rightarrow$ End$_L(V)$est un isomorphisme. Soit C l’anneau End$_A(V)$. Alors C est semblable à $A^o$ et l’image de $L\otimes 1\subset A_{(L)}$ est une sous-algèbre commutative maximale de C.

Identifions A à un sous-anneau de $A_{(L)}$. Considérons V comme un K-espace vectoriel. L’anneau C est le commutant de $\varphi (A)$ dans End$_K(V)$. C’est une K-algèbre centrale, simple et de degré fini, et l’homomorphisme $a\otimes c\rightarrow ac$ de $A\otimes_KC$ dans End$_K(V)$ est un isomorphisme (VIII, p. 256, th. 6 a)). Par suite les K-algèbres A et $C^o$ sont semblables (VIII, p. 275, prop. 3).

Soit $L_V$ l’anneau des homothéties du L-espace vectoriel V ; c’est le commutant de End$_L(V)$ dans End$_K(V)$ (VIII, p. 78, cor. 1). Or la K-algèbre End$_L(V)$ est engendrée par $\varphi (A)$ et $L_V$; on a donc dans End$_K(V)$

$L_V=$ End$_L(V)'=\varphi (A)'\cap L'_V= C\cap L'_V$,

où pour toute partie B de End$_K$(V), le commutant de B dans End$_K(V)$ est noté $B'$. Ainsi $L_V$ est une sous-algèbre commutative maximale de C (VIII, p. 257, lemme 3), et donc aussi de $C^o$. L’application $\lambda \rightarrow \lambda_V$ est un isomorphisme de K-algèbres de L sur $L_V$; cela prouve le lemme.

#### Corollaire 1 {#alg-viii-s15-lem-3-cor-1 .statement tag=00I5}

Soient A une K-algèbre centrale, simple et de degré fini, et L une extension de degré fini de K. Supposons que $[A : K] = [L : K]^2$. Pour que L déploie A, il faut et il suffit que A contienne une sous-algèbre isomorphe à L.

Supposons qu’il existe un morphisme $\varphi$ de L dans A. Soit M une sous-algèbre commutative semi-simple maximale contenant $\varphi (L)$. Par la prop. 3 de VIII, p. 258, on a $[A : K] = [M : K]^2$, donc [M : K] = [L : K] et $M =\varphi (L)$. D’après la prop. 5, L déploie A. Inversement supposons que l’extension L déploie A, alors elle est isomorphe à une sous-algèbre commutative maximale d’une K-algèbre B centrale, simple et semblable à A (prop. 5). On a $[B : K] = [L : K]^2$ (VIII, p. 258, prop. 3), d’où [B : K] = [A : K] ; par suite B est isomorphe à A (VIII, p. 276, cor.), d’où le corollaire 1.

#### Corollaire 2 {#alg-viii-s15-lem-3-cor-2 .statement tag=00I6}

Soient D un corps de centre K et de degré fini sur K, et L une extension de degré fini de K déployant D. Le degré réduit de D divise [L : K].

Notons $r$ le degré réduit de D (VIII, p. 249) ; par définition, $[D : K] =r^2$. D’après la prop. 5, il existe une K-algèbre B centrale simple semblable à D dont L est une sous-algèbre commutative maximale. Comme B est isomorphe à une algèbre de matrices $\mathbf{M}_n(D)$ (VIII, p. 274, lemme 1), on a [B : K] = $n^2r^2$, et par suite $[L : K] =nr$ (VIII, p. 258, prop. 3).

### 4. Exemples de groupes de Brauer

Le groupe de Brauer Br(K) est réduit à l’élément neutre dans les trois cas suivants :

a) K est séparablement clos (VIII, p. 249, cor. 1).

$*$b) K est un corps fini (VIII, p. 349, cor. 2).

c) K satisfait à la propriété $(C_1)$ (VIII, p. 349, remarque 2).

Supposons que K soit un corps ordonné maximal (VI, p. 24). Le groupe de Brauer de K est alors cyclique d’ordre 2 ; ses éléments sont la classe de K et la classe de la K-algèbre de quaternions de type $(-1,0,-1)$ (III, p. 18 et VIII, p. 359, th. 1).

Supposons que K soit un corps topologique localement compact, non discret et commutatif. Si K n’est pas connexe c’est un corps complet pour une valuation discrète, de corps résiduel fini (AC, VI, p. 154, th. 1), il existe un isomorphisme de Br(K) sur $\mathbf{Q}/\mathbf{Z}$(VIII, p. 327, exerc. 17). Si K est connexe, il est isomorphe à $\mathbf{R}$ou $\mathbf{C}$. Le groupe de Brauer du corps $\mathbf{R}$est cyclique d’ordre 2. Son élément non trivial est la classe de l’algèbre $\mathbf{H}$des quaternions de Hamilton (TG VII, p. 4) ; le groupe de Brauer de $\mathbf{C}$est d’ordre $1.*$

## EXERCICES {#alg-viii-s15-exercises}

See the [exercises for § 15](exercises/s15/).
