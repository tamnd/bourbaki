---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 3
section_title: Modules simples
lang: fr
source: alg-viii-fr
book_pages: A VIII.41-A VIII.50
pdf_pages: 0052-0061
extraction: native
subsections:
    - "no": 1
      title: Modules simples
      page: 41
      pdf_page: 52
    - "no": 2
      title: Le lemme de Schur
      page: 43
      pdf_page: 54
    - "no": 3
      title: Sous-modules maximaux
      page: 44
      pdf_page: 55
    - "no": 4
      title: Modules simples sur un anneau artinien
      page: 46
      pdf_page: 57
    - "no": 5
      title: Classes de modules simples
      page: 47
      pdf_page: 58
statements: 23
exercises: 10
content_sha256: 7219d389af874cf7c041e423756b7d57af7b0b896e19508b9716dbecb9d09434
---

## § 3. MODULES SIMPLES

### 1. Modules simples

Rappelons la définition suivante (II, p. 21) :

#### Définition 1 {#alg-viii-s3-def-1 .statement tag=0035}

Soit A un anneau. Un A-module M est dit simple s’il n’est pas nul et ne contient pas d’autre sous-module que 0 et M.

Pour qu’un A-module M soit simple, il faut et il suffit que M soit un module simple sur l’anneau $A_M$ de ses homothéties. Tout module simple est indécomposable, de longueur 1, donc primordial (VIII, p. 28, prop. 4 b)).

#### Exemple 1 {#alg-viii-s3-n1-exa-1 .statement tag=0036}

Pour que $A_s$ soit un A-module simple, il faut et il suffit que A soit un corps (I, p. 109, th. 1). Les A-modules simples sont alors les espaces vectoriels de dimension 1 sur le corps A.

#### Exemple 2 {#alg-viii-s3-n1-exa-2 .statement tag=0037}

Soit A un anneau principal (VII, p. 1, déf. 1) qui n’est pas un corps. Pour tout élément extrémal $\pi$ de A, le A-module $A_s/(\pi )$ est simple, et tout A-module simple est isomorphe à un tel module (VII, p. 25, remarque 4). Pour $n\geqslant 2$, le A-module $A_s/(\pi^n)$ est indécomposable (VII, p. 23, prop. 8), mais n’est pas simple.

#### Exemple 3 {#alg-viii-s3-n1-exa-3 .statement tag=0038}

Soient K un corps, V un espace vectoriel à droite non nul sur le corps K et A un sous-anneau de l’anneau End$_K(V)$ qui contient les endomorphismes de rang fini de V (par exemple A = End$_K(V))$. Démontrons que V est un A-module simple : soient W un sous-A-module non nul de V et $x$ un élément non nul de W ; il existe une forme linéaire $\varphi$ sur V telle que $\varphi (x)\not= 0$ (II, p. 103, th. 6). Pour tout $y$ dans V, l’application $z\rightarrow y\varphi (z)$, linéaire de rang $\leqslant 1$, appartient à A ; on a donc $Ax= V$, d’où a fortiori W = V, ce qui prouve que V est un A-module simple.

#### Proposition 1 {#alg-viii-s3-prop-1 .statement tag=00QZ}

Soit A un anneau.

a) Soit $\mathfrak{m}$ un idéal à gauche de A. Pour que le A-module $A_s/\mathfrak{m}$ soit simple, il faut et il suffit que $\mathfrak{m}$ soit un idéal à gauche maximal.

b) Soit M un A-module simple et soit $x$ un élément non nul de M. On a l’égalité $M = Ax$, l’annulateur $\mathfrak{m}$ de $x$ est un idéal à gauche maximal de A, et l’application $a\rightarrow ax$ définit par passage au quotient un isomorphisme de $A_s/\mathfrak{m}$ sur M.

c) Soit M un A-module non nul. Si l’on a $M = Ax$ pour tout élément non nul $x$ de M, alors M est simple.

Les sous-modules de $A_s/\mathfrak{m}$ sont de la forme $\mathfrak{n}/\mathfrak{m}$, où $\mathfrak{n}$ est un idéal à gauche de A contenant $\mathfrak{m}$ (I, p. 39, th. 4) ; par suite le A-module $A_s/\mathfrak{m}$ est simple si et seulement si l’on a $\mathfrak{m}\not= A$ et tout idéal à gauche $\mathfrak{n}$ de A contenant $\mathfrak{m}$ satisfait à $\mathfrak{n}/\mathfrak{m}= 0$ ou $\mathfrak{n}/\mathfrak{m}= A_s/\mathfrak{m}$, c’est-à-dire à $\mathfrak{n}=\mathfrak{m}$ ou $\mathfrak{n}= A$. Ceci prouve a).

Sous les hypothèses de b), $Ax$ est un sous-module non nul de M, donc égal à M. Par suite, l’application $a\rightarrow ax$ définit par passage au quotient un isomorphisme de $A_s/\mathfrak{m}$ sur M ; le A-module $A_s/\mathfrak{m}$ est donc simple et l’idéal à gauche $\mathfrak{m}$ est maximal d’après a). Ceci prouve b).

Sous les hypothèses de c), soit N un sous-module non nul de M. Si $x$ est un élément non nul de N, on a $Ax\subset N$ et $Ax= M$, d’où M = N. Donc M est simple.

#### Corollaire 1 {#alg-viii-s3-prop-1-cor-1 .statement tag=0039}

Si l’anneau A n’est pas réduit à 0, il existe des A-modules simples.

En effet, il existe d’après le théorème de Krull (I, p. 99, th. 1) des idéaux à gauche maximaux de A.

#### Corollaire 2 {#alg-viii-s3-prop-1-cor-2 .statement tag=003A}

Soient A un anneau local (VIII, p. 24, déf. 1) et $\mathfrak{r}$ son idéal maximal. Le A-module $A_s/\mathfrak{r}$ est simple et tout A-module simple est isomorphe à $A_s/\mathfrak{r}$.

#### Remarque 1 {#alg-viii-s3-n1-rem-1 .statement tag=003B}

Soient A un anneau commutatif, et $\mathfrak{m}$ un idéal de A. Alors $\mathfrak{m}$ est l’annulateur (II, p. 28, déf. 11) du A-module $A_s/\mathfrak{m}$. Ainsi, si $\mathfrak{m}$ et $\mathfrak{m}'$ sont des idéaux de A distincts, les A-modules $A_s/\mathfrak{m}$ et $A_s/\mathfrak{m}'$ ne sont pas isomorphes. Pour qu’il existe un A-module simple et fidèle (II, p. 28), il faut et il suffit que (0) soit un idéal maximal de A, c’est-à-dire que A soit un corps.

#### Remarque 2 {#alg-viii-s3-n1-rem-2 .statement tag=003C}

On peut donner un exemple d’anneau non commutatif A et de deux idéaux à gauche maximaux distincts $\mathfrak{m}$ et $\mathfrak{m}'$ de A tels que les A-modules $A_s/\mathfrak{m}$ et $A_s/\mathfrak{m}'$ soient isomorphes (VIII, p. 48, exerc. 3).

### 2. Le lemme de Schur

#### Proposition 2 {#alg-viii-s3-prop-2 .statement tag=003D}

Soient A un anneau, M et N deux A-modules et $f$ un homomorphisme non nul de M dans N.

a) Si M est simple, $f$ est injectif.

b) Si N est simple, $f$ est surjectif.

c) Si M et N sont simples, $f$ est un isomorphisme.

Le noyau de $f$ est un sous-module de M distinct de M, et l’image de $f$ est un sous-module non nul de N.

a) Si M est simple, on a Ker($f$) $= 0$, donc $f$ est injectif.

b) Si N est simple, on a Im($f$) $= N$, donc $f$ est surjectif.

c) Si M et N sont simples, $f$ est à la fois injectif et surjectif.

#### Corollaire {#alg-viii-s3-n2-cor-1 .statement tag=00RZ}

L’anneau des endomorphismes d’un module simple est un corps.

Si M est un A-module simple, tout élément non nul de l’anneau non nul End$_A(M)$ est inversible (prop. 2, c)), donc End$_A(M)$ est un corps.

#### Théorème 1 {#alg-viii-s3-thm-1 .statement tag=003E}

Soient K un corps commutatif algébriquement clos, A une K-algèbre et M un A-module simple. On suppose que la dimension de M comme espace vectoriel sur K est finie, ou plus généralement strictement inférieure au cardinal de K. Alors l’anneau des endomorphismes du A-module M se compose des homothéties $\alpha_M$ avec $\alpha \in K$.

Soit E l’anneau des endomorphismes du A-module M ; c’est un corps d’après le cor. de la prop. 2, et une algèbre sur le corps K. Si l’on considère M comme un espace vectoriel à gauche sur le corps E, on a dim$_KM =$ (dim$_EM)[E : K]$ d’après la prop. 25 de II, p. 31, donc dim$_KM\geqslant [E : K]$. Comme dim$_KM<$ Card(K) par hypothèse, l’égalité $E = K\cdot 1_M$ résulte alors du lemme suivant :

#### Lemme 1 {#alg-viii-s3-lem-1 .statement tag=003F}

Soient E un corps et K un sous-corps du centre de E, distinct de E. Si le corps K est algébriquement clos, on a $[E : K]\geqslant$ Card(K).

Soient $x$ un élément de E K et L le sous-corps (commutatif) de E engendré par $K\cup  \{x\}$. Comme K est algébriquement clos, $x$ est transcendant sur K. D’après VII, p. 10, th. 2 et p. 11, les éléments $(x-\alpha )^{-1}$ de L, où $\alpha$ parcourt K, sont linéairement indépendants sur K. On a donc $[E : K]\geqslant [L : K]\geqslant$ Card(K).

#### Exemple {#alg-viii-s3-n2-exa-1 .statement tag=003G}

$*$Soit A une $\mathbf{C}$-algèbre engendrée par une famille dénombrable d’éléments ; elle est de dimension dénombrable sur $\mathbf{C}$. Soit M un A-module simple ; il est monogène, donc admet une base dénombrable sur $\mathbf{C}$. Puisque le corps $\mathbf{C}$n’est pas dénombrable (TG, IV, p. 44), on a $[M : \mathbf{C}]<$ Card($\mathbf{C}$). Donc les endomorphismes du A-module M sont les homothéties $\alpha_M$, avec $\alpha \in \mathbf{C}$. Ceci s’applique en particulier lorsque A est l’algèbre enveloppante d’une algèbre de Lie de dimension finie sur $\mathbf{C}$ (LIE, I, corollaire 3, p. $33).*$

#### Corollaire 1 {#alg-viii-s3-lem-1-cor-1 .statement tag=003H}

Conservons les hypothèses du théorème 1, et supposons de plus l’algèbre A commutative. Alors M est de dimension 1 sur K.

Comme l’anneau A est commutatif, $a_M$ est un endomorphisme du A-module M pour tout $a\in A$. D’après le th. 1, on a donc $A_M= K\cdot 1_M$ et M est un K-module simple, c’est-à-dire un espace vectoriel de dimension 1 sur le corps K.

#### Corollaire 2 {#alg-viii-s3-lem-1-cor-2 .statement tag=003I}

Soient K un corps commutatif, A une K-algèbre et M un A-module. On suppose que pour toute extension L de K, le $A_{(L)}$-module $M_{(L)}$ est simple. Alors l’anneau des endomorphismes de M se compose des homothéties $\alpha_M$ avec $\alpha \in K$.

Soit I un ensemble de cardinal strictement supérieur à la dimension de M sur K (par exemple l’ensemble des parties de M). Soit L une clôture algébrique du corps $K((X_i)_{i\in I})$ (V, p. 22, th. 2). Choisissons une forme K-linéaire $\varphi$ sur L telle que $\varphi (1) = 1$ et notons $v: M_{(L)}\rightarrow M$ l’application K-linéaire caractérisée par $v(\alpha \otimes m) =\varphi (\alpha )m$. Soit $u$ un endomorphisme de M. La dimension de $M_{(L)}$ sur L est égale à celle de M sur K et est strictement inférieure au cardinal de L. D’après le th. 1, l’endomorphisme $1_L\otimes u$ du $A_{(L)}$-module $M_{(L)}$ est de la forme $\lambda \otimes 1_M$, avec $\lambda \in L$. Pour tout $x\in M$, on a

$$
u(x) =v(1\otimes u(x))=v((1_L\otimes u)(1\otimes x))
$$

$$
=v((\lambda \otimes 1_M)(1\otimes x))=v(\lambda \otimes x) =\varphi (\lambda )x
$$

de sorte que $u$ est l’homothétie $\varphi (\lambda )_M$.

### 3. Sous-modules maximaux

#### Définition 2 {#alg-viii-s3-def-2 .statement tag=003J}

Soient A un anneau et M un A-module. On appelle sous-module maximal de M un élément maximal, pour la relation d’inclusion, de l’ensemble des sous-modules de M distincts de M.

Un sous-module maximal de $A_s$ n’est autre qu’un idéal maximal à gauche de A.

Soit N un sous-module de M. Les sous-modules de $M/N$ sont de la forme $P/N$ où P est un sous-module de M contenant N (I, p. 39, th. 4). Par suite, N est un sous-module maximal de M si et seulement si le module $M/N$ est simple.

#### Proposition 3 {#alg-viii-s3-prop-3 .statement tag=003K}

Soit M un A-module de type fini. Tout sous-module de M distinct de M est contenu dans un sous-module maximal.

Soit N un sous-module de M, distinct de M. Notons $\mathscr{S}$ l’ensemble des sous-modules de M distincts de M et contenant N ordonné par la relation d’inclusion ; démontrons que $\mathscr{S}$ est inductif. Soit $\mathscr{F}$ une partie totalement ordonnée de $\mathscr{S}$. Si $\mathscr{F}$ est vide, N est un majorant de $\mathscr{F}$ dans $\mathscr{S}$. Dans le cas contraire, notons Q la réunion des éléments de $\mathscr{F}$. Alors Q est un sous-module de M. Soit F une partie génératrice finie de M. Si Q était égal à M, F serait contenue dans un sous-module $P\in \mathscr{F}$, ce qui entraînerait P = M, contrairement à la définition de $\mathscr{F}$. On a donc $Q\in \mathscr{S}$, ce qui prouve que $\mathscr{S}$ est inductif. La prop. 3 résulte alors du cor. 1 de E, III, p. 21.

#### Corollaire 1 {#alg-viii-s3-prop-3-cor-1 .statement tag=003L}

Soit M un A-module de type fini non nul. Il existe un idéal bilatère $\mathfrak{a}$ de A, annulateur d’un A-module simple, tel que $\mathfrak{a}M$soit distinct de M.

Soit N un sous-module maximal de M (prop. 3) et soit $\mathfrak{a}$ l’annulateur du A-module simple $M/N$; c’est un idéal bilatère de A et l’on a $\mathfrak{a}(M/N) = 0$, d’où $\mathfrak{a}M\subset N$ et par suite $\mathfrak{a}M\not= M$.

#### Corollaire 2 {#alg-viii-s3-prop-3-cor-2 .statement tag=003M}

Soient A un anneau commutatif et B une A-algèbre. Soit M un B-module simple qui est un A-module de type fini et soit $\mathfrak{m}$ l’annulateur du A-module M. Alors $\mathfrak{m}$ est un idéal maximal de A et M est un espace vectoriel de dimension finie sur le corps $A/\mathfrak{m}$.

Comme l’anneau A est commutatif, l’annulateur d’un A-module simple est un idéal maximal de A (VIII, p. 42, prop. 1). D’après le corollaire 1 appliqué au A-module M, il existe un idéal maximal $\mathfrak{a}$ de A tel que $\mathfrak{a}M\not= M$. Mais $\mathfrak{a}M$ est un sous-module du B-module simple M ; on a donc $\mathfrak{a}M = 0$, d’où $\mathfrak{a}\subset \mathfrak{m}$. Comme l’idéal $\mathfrak{m}$ est distinct de A, il est égal à $\mathfrak{a}$, de sorte que $\mathfrak{m}$ est maximal. Le module M est un module de type fini sur le corps $A/\mathfrak{m}$, d’où la dernière assertion.

### 4. Modules simples sur un anneau artinien

Soit A un anneau. On dit par abus de langage qu’un idéal à gauche $\mathfrak{a}$ est un idéal à gauche minimal de A si c’est un élément minimal de l’ensemble des idéaux à gauche non nuls de A, ordonné par la relation d’inclusion. On définit de manière analogue les idéaux à droite minimaux et les idéaux bilatères minimaux.

Soit $\mathfrak{a}$ un idéal à gauche de A. Pour que $\mathfrak{a}$ soit un A-module simple, il faut et il suffit que ce soit un idéal à gauche minimal de A.

Tout idéal à gauche non nul d’un anneau artinien à gauche (VIII, p. 1, déf. 1) contient un idéal à gauche minimal.

#### Proposition 4 {#alg-viii-s3-prop-4 .statement tag=003N}

Soit A un anneau possédant un idéal à gauche minimal $\mathfrak{a}$. Tout A-module simple et fidèle est isomorphe au A-module $\mathfrak{a}$.

Soit M un A-module simple et fidèle. Soit $\alpha$ un élément non nul de $\mathfrak{a}$. Comme le A-module M est fidèle, il existe un élément $x$ de M tel que $\alpha x\not= 0$. L’homomorphisme $a\rightarrow ax$ de $\mathfrak{a}$ dans M est alors non nul ; c’est donc un isomorphisme d’après la prop. 2 de VIII, p. 43.

#### Proposition 5 {#alg-viii-s3-prop-5 .statement tag=003O}

Soient A un anneau artinien à gauche et M un A-module fidèle.

a) Il existe un entier naturel $m$ et un isomorphisme de $A_s$ sur un sous-module de $M^m$.

b) Si M possède une suite de Jordan-Hölder $(M_i)_{0\leqslant i\leqslant n}$, tout A-module simple est isomorphe à l’un des quotients $M_i/M_{i+1}$.

D’après VIII, p. 2 appliqué au A-module $A_s$ et aux annulateurs des éléments de M, il existe des éléments $x_1, . . . , x_m$ de M tels que l’annulateur de M soit l’intersection des annulateurs des $x_i$. Comme le A-module M est fidèle, l’application A-linéaire $a\rightarrow (ax_1, . . . , ax_m)$ de $A_s$ dans $M^m$ est injective, d’où a).

Sous les hypothèses de b), tout quotient simple de $A_s$ est isomorphe à un quotient d’une suite de Jordan-Hölder de $M^m$ (I, p. 41, cor.), donc à l’un des modules $M_i/M_{i+1}$ (I, p. 41, th. 6). Enfin, tout A-module simple est isomorphe à un quotient de $A_s$.

#### Remarque {#alg-viii-s3-n4-rem-1 .statement tag=003P}

La proposition 5 s’applique en particulier dans les deux cas suivants :

a) Soit A une algèbre sur un corps commutatif K et soit M un module fidèle de dimension finie sur K. Alors M est un A-module de longueur finie et le contremodule de M est de type fini. L’anneau A est artinien à gauche (VIII, p. 8, prop. 6). Il existe une suite de Jordan-Hölder $(M_i)_{0\leqslant i\leqslant n}$ du A-module M, et tout A-module simple est isomorphe à l’un des modules $M_i/M_{i+1}$ pour $0\leqslant i\leqslant n-1$.

b) Soit A un anneau artinien à gauche. Le module $A_s$ est de longueur finie (VIII, p. 5, th. 1). Comme le A-module $A_s$ est de longueur finie, il existe une suite décroissante $(\mathfrak{a}_i)_{0\leqslant i\leqslant n}$ d’idéaux à gauche de A, telle que $\mathfrak{a}_0= A,\mathfrak{a}_n= 0$ et que les A-modules $S_i=\mathfrak{a}_{i-1}/\mathfrak{a}_i$ soient simples pour $1\leqslant i\leqslant n$. Alors tout A-module simple est isomorphe à l’un des modules $S_1, . . . ,S_n$.

### 5. Classes de modules simples

Notons Is$_A(X,Y)$ la relation

« A est un anneau et $X,Y$ sont des A-modules isomorphes ».

C’est une relation d’équivalence par rapport à X et Y. Si X est un A-module, on note cl(X), et on appelle classe du A-module X, la classe d’objets équivalents à X pour Is$_A$ (E, II, p. 47). Par définition, cl(X) est un A-module isomorphe à X ; de plus, deux A-modules X et Y sont isomorphes si et seulement si l’on a cl(X) = cl(Y).

Soit A un anneau. La relation

« $\lambda$ est une classe de A-modules de type fini »

est collectivisante en $\lambda$ (E, II, p. 3). En effet, tout A-module de type fini est isomorphe à un A-module de la forme $A^n_s/R$, où $n$ est un entier naturel et R un sous-module de $A^n_s$, de sorte que notre assertion résulte de E, II, p. 47.

On notera $\mathscr{F}(A)$ l’ensemble des classes de A-modules de type fini. Tout A-module simple est monogène (VIII, p. 42, prop. 1), et par suite les classes des A-modules simples forment un sous-ensemble de $\mathscr{F}$(A), noté dans la suite $\mathscr{S}(A)$ (ou simplement $\mathscr{S})$. Lorsque l’anneau A est commutatif, l’application $\mathfrak{m}\rightarrow$ cl(A$/\mathfrak{m})$ est une bijection de l’ensemble des idéaux maximaux de A sur l’ensemble $\mathscr{S}(A)$ (loc. cit. et VIII, p. 42, remarque 1). Lorsque A est artinien à gauche, l’ensemble $\mathscr{S}(A)$ est fini (VIII, p. 47, remarque b)).

## EXERCICES {#alg-viii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
