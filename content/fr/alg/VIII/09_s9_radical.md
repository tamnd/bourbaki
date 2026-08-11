---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 9
section_title: Radical
lang: fr
source: alg-viii-fr
book_pages: A VIII.147-A VIII.168
pdf_pages: 0153-0174
extraction: native
subsections:
    - "no": 1
      title: Radical d’un module
      page: 147
      pdf_page: 153
    - "no": 2
      title: Radical d’un anneau
      page: 150
      pdf_page: 156
    - "no": 3
      title: Lemme de Nakayama
      page: 154
      pdf_page: 160
    - "no": 4
      title: Relèvements d’idempotents
      page: 155
      pdf_page: 161
    - "no": 5
      title: Couverture projective d’un module
      page: 156
      pdf_page: 162
statements: 49
exercises: 31
content_sha256: f3c97e654802cccd8632d6d02e163804fad39b61872da01b17c741181871e5f0
---

## § 9. RADICAL

### 1. Radical d’un module

#### Définition 1 {#alg-viii-s9-def-1 .statement tag=00A1}

Soit A un anneau. On appelle radical d’un A-module M le sous-module intersection des sous-modules maximaux de M (VIII, p. 44, déf. 2) ou, ce qui revient au même, l’ensemble des éléments de M annulés par tout homomorphisme de M dans un A-module simple.

Dans la suite de ce chapitre, on notera $\mathfrak{R}_A$(M), ou simplement $\mathfrak{R}$(M), le radical d’un A-module M.

Soit A un anneau. Pour que le radical d’un A-module M soit réduit à 0 (auquel cas on dit, par abus de langage, que M est sans radical), il faut et il suffit qu’il existe une famille $(S_i)_{i\in I}$ de A-modules simples et une famille $(f_i)_{i\in I}$ d’applications A-linéaires $f_i: M\rightarrow S_i$, telles que l’on ait $\cap_{i\in I}$ Ker($f_i$) $= 0$. Il revient au même de dire que M est isomorphe à un sous-module d’un produit de A-modules simples.

#### Exemple 1 {#alg-viii-s9-n1-exa-1 .statement tag=00A2}

Soit $\mathfrak{a}$ un idéal à gauche de A. Le radical du A-module $A_s/\mathfrak{a}$ est égal à $\mathfrak{a}'/\mathfrak{a}$ où $\mathfrak{a}'$ est l’intersection des idéaux à gauche maximaux de A contenant $\mathfrak{a}$. En particulier, le radical du $\mathbf{Z}$-module $\mathbf{Z}$est réduit à 0, et celui du $\mathbf{Z}$-module $\mathbf{Z}/p^n\mathbf{Z}$ est égal à $p\mathbf{Z}/p^n\mathbf{Z}$pour tout nombre premier $p$ et tout nombre entier $n\geqslant 1$.

#### Exemple 2 {#alg-viii-s9-n1-exa-2 .statement tag=00A3}

Soit A un anneau principal qui n’est pas un corps et soit K son corps des fractions. Comme K-module, K est sans radical. Démontrons que le radical de K, considéré comme A-module, est égal à K, ou, ce qui revient au même, que toute application A-linéaire $f$ de K dans un A-module simple S est nulle. D’après VII, p. 25, on peut supposer S égal à $A()/(\pi ()$, où$)\pi$ est un élément extrémal de A ; pour tout $x\in K$, on a $f(x) =f\pi_{\pi}^x=\pi f^x_{\pi}$ = 0 puisque $\pi S = 0$, d’où le résultat.

#### Proposition 1 {#alg-viii-s9-prop-1 .statement tag=00A4}

Soient M et N des A-modules et $f$ un homomorphisme de M dans N. On a $f(\mathfrak{R}(M))\subset \mathfrak{R}(N)$, et l’on a même égalité si $f$ est surjectif et que le noyau de $f$ est contenu dans le radical de M.

Soit $g$ un homomorphisme de N dans un A-module simple ; alors $\mathfrak{R}(M)$ est contenu dans le noyau de $g\circ f$, de sorte que $f(\mathfrak{R}(M))$ est contenu dans le noyau de $g$. On a donc $f(\mathfrak{R}(M))\subset \mathfrak{R}(N)$. Supposons maintenant que $f$ soit surjectif, et que son noyau soit contenu dans $\mathfrak{R}(M)$. Soit $y$ un élément de $\mathfrak{R}(N)$ et soit $x$ un antécédent de $y$. Si $g$ est un homomorphisme de M dans un A-module simple S, son noyau contient le radical de M, donc le noyau de $f$; l’homomorphisme $f$ étant surjectif, il existe un homomorphisme $h$ de N dans S tel que $g=h\circ f$. Comme $y=f(x)$ appartient à $\mathfrak{R}$(N), on a $h(f(x)) = 0$, c’est-à-dire $g(x) = 0$; ainsi $x$ appartient à $\mathfrak{R}$(M), ce qui prouve l’inclusion $\mathfrak{R}(N)\subset f(\mathfrak{R}(M))$.

#### Corollaire 1 {#alg-viii-s9-prop-1-cor-1 .statement tag=00A5}

Soient M un A-module et N un sous-module de M.

a) On a $\mathfrak{R}(N)\subset \mathfrak{R}(M)\cap N$.

b) On a $(\mathfrak{R}(M) + N)/N\subset \mathfrak{R}(M/N)$. Si N est contenu dans $\mathfrak{R}(M)$, on a l’égalité $\mathfrak{R}(M/N) =\mathfrak{R}(M)/N$.

c) Le module $M/\mathfrak{R}(M)$est sans radical. Si le module $M/N$est sans radical, on a $\mathfrak{R}(M)\subset N$.

L’assertion a) résulte de la prop. 1 appliquée à l’injection canonique de N dans M, et l’assertion b) de la prop. 1 appliquée à l’application canonique de M sur $M/N$. De b), on déduit que $M/N$ est sans radical si $N =\mathfrak{R}(M)$ et que l’on a $\mathfrak{R}(M)\subset N$ si $M/N$ est sans radical.

$\dbend$ Il résulte de l’exemple 1 de VIII, p. 147 qu’il peut exister des sous-modules N contenant $\mathfrak{R}(M)$ et tels que le radical de $M/N$ ne soit pas nul.

#### Corollaire 2 {#alg-viii-s9-prop-1-cor-2 .statement tag=00A6}

Soient $(M_i)_{i\in I}$ une famille de A-modules, P son produit et S sa somme directe. On a $\mathfrak{R}(P)\subset \prod_{i\in I}\mathfrak{R}(M_i)$et $\mathfrak{R}(S) =\bigoplus_{i\in I}\mathfrak{R}(M_i)$.

Pour tout $i\in I$, soit $\pi_i$ la projection d’indice $i$ de P dans $M_i$; d’après la prop. 1, on a $\pi_i(\mathfrak{R}(P))\subset \mathfrak{R}(M_i)$ pour tout $i\in I$, d’où la première assertion. On a $S\subset P$, d’où

$$
\mathfrak{R}(S)\subset S\cap \mathfrak{R}(P)\subset S\cap \prod_{i\in I}\mathfrak{R}(M_i) =\bigoplus_{i\in I}\mathfrak{R}(M_i)
$$

par ailleurs, pour tout $i\in I$, on a $M_i\subset S$, d’où $\mathfrak{R}(M_i)\subset \mathfrak{R}$(S), et finalement $\oplus_{i\in I}\mathfrak{R}(M_i)\subset \mathfrak{R}(S)$.

Il existe des familles de modules dont le radical du produit n’est pas isomorphe au produit des radicaux (exerc. 3 de VIII, p. 161).

#### Proposition 2 {#alg-viii-s9-prop-2 .statement tag=00A7}

Soit M un A-module de type fini.

a) Si M n’est pas réduit à 0, on a $\mathfrak{R}(M)\not= M$.

b) Si N est un sous-module de M tel que $N +\mathfrak{R}(M) = M$, on a N = M.

Soit N un sous-module de M, distinct de M. D’après la prop. 3 de VIII, p. 45, il existe un sous-module maximal L de M contenant N. On a $N +\mathfrak{R}(M)\subset L$, et a fortiori $N+\mathfrak{R}(M)\not= M$. Cela prouve b) ; le cas particulier N = 0 établit l’assertion a).

#### Corollaire {#alg-viii-s9-n1-cor-1 .statement tag=00A8}

Soient M un A-module, $(x_i)_{i\in I}$ une famille génératrice de M et $x$ un élément de M. Les conditions suivantes sont équivalentes :

(i) On a $x\in \mathfrak{R}(M)$;

(ii) Tout sous-module N de M tel que $N + Ax= M$est égal à M ;

(iii) Pour toute famille $(a_i)_{i\in I}$ d’éléments de A, la famille $(x_i+a_ix)_{i\in I}$ engendre le A-module M.

(i) $=\Rightarrow$ (ii) : Supposons que $x$ appartienne à $\mathfrak{R}(M)$. Soit N un sous-module de M tel que $N+Ax= M$. On a $N+\mathfrak{R}(M) = M$, de sorte que le A-module $M/N$ est égal à son radical (cor. 1, b) de la prop. 1). Comme il est monogène, il est nul (prop. 2) et l’on a M = N.

(ii) $=\Rightarrow$ (iii) : Soit $(a_i)_{i\in I}$ une famille d’éléments de A. Notons N le sous-module de M engendré par la famille $(x_i+a_ix)_{i\in I}$. On a $x_i\in N + Ax$ pour tout $i\in I$, d’où $N + Ax= M$. Si la condition (ii) est satisfaite, N est égal à M.

(iii) $=\Rightarrow$ (i) : Supposons que $x$ n’appartienne pas à $\mathfrak{R}(M)$. Il existe alors un sous-module maximal N de M qui ne contient pas $x$. Comme N est maximal, on a $N + Ax= M$; chacun des éléments $x_i$ peut donc s’écrire sous la forme $y_i-a_ix$, avec $y_i\in N$ et $a_i\in A$. La famille $(x_i+a_ix)_{i\in I}$ est contenue dans N, donc n’engendre pas M.

#### Proposition 3 {#alg-viii-s9-prop-3 .statement tag=00A9}

a) Un module semi-simple est sans radical.

b) Pour qu’un module soit semi-simple et de type fini, il faut et il suffit qu’il soit sans radical et artinien.

Par définition, le radical d’un module simple est réduit à 0. Si le module M est semi-simple, il est somme directe d’une famille $(S_i)_{i\in I}$ de sous-modules simples, et l’on a $\mathfrak{R}(M) =\bigoplus_{i\in I}\mathfrak{R}(S_i)$ d’après le cor. 2 ci-dessus, d’où $\mathfrak{R}(M) = 0$.

Si de plus M est de type fini, il est artinien d’après la prop. 10 de VIII, p. 67.

Réciproquement, supposons que M soit sans radical et artinien. D’après VIII, p. 2, appliqué à l’ensemble des sous-modules maximaux de M, il existe une famille finie $(N_i)_{i\in I}$ de sous-modules maximaux de M dont l’intersection est réduite à 0. Alors M est isomorphe à un sous-module de $\bigoplus_{i\in I}(M/N_i)$; il est donc semi-simple et de longueur finie, et a fortiori de type fini.

### 2. Radical d’un anneau

#### Définition 2 {#alg-viii-s9-def-2 .statement tag=00AA}

On appelle radical de Jacobson (ou simplement radical) d’un anneau A, et l’on note $\mathfrak{R}(A)$, le radical du A-module $A_s$, c’est-à-dire l’intersection des idéaux à gauche maximaux de A.

On dit, par abus de langage, que l’anneau A est sans radical si l’on a $\mathfrak{R}(A) = 0$.

#### Proposition 4 {#alg-viii-s9-prop-4 .statement tag=00AB}

Pour qu’un anneau A soit semi-simple, il faut et il suffit qu’il soit artinien à gauche et sans radical.

Cela résulte de la prop. 3, b) appliquée au A-module $A_s$.

#### Exemple 1 {#alg-viii-s9-n2-exa-1 .statement tag=00AC}

Si A est un anneau local, il possède un unique idéal à gauche maximal $\mathfrak{r}$, formé des éléments non inversibles de A (VIII, p. 23, prop. 1) ; donc $\mathfrak{r}$ est le radical de A. En particulier, un corps est sans radical.

#### Exemple 2 {#alg-viii-s9-n2-exa-2 .statement tag=00AD}

Soient K un corps commutatif et E l’algèbre $K[[X_i]]_{i\in I}$ des séries formelles par rapport aux indéterminées $X_i$ à coefficients dans K. D’après l’exemple précédent et l’exemple 4 de VIII, p. 24, le radical de E se compose des séries formelles $\dbend$ de terme constant nul. On notera que l’anneau E est intègre et que son radical n’est pas réduit à 0, bien que E soit un sous-anneau de son corps des fractions qui est sans radical.

#### Exemple 3 {#alg-viii-s9-n2-exa-3 .statement tag=00AE}

Supposons que A soit un anneau principal et soit P un système représentatif d’éléments extrémaux (VII, p. 3). Si A est un corps, il est sans radical d’après l’exemple 1 ; si l’ensemble P est infini, l’intersection des idéaux maximaux $Ap$ de A est réduite à 0, donc A est sans radical ; mais si P est fini et non vide, et si l’on pose $x=\prod_{p\in P}p$, le radical de A est égal à $\cap_{p\in P}Ap= Ax$ (VII, p. 3, prop. 4), donc n’est pas réduit à zéro.

Soit $y$ un élément non nul de A ; écrivons-le sous la forme $y=up^i_{1^1}. . . p^i_{r^r}$, où $u$ est inversible dans $A,p_1, . . . , p_r$ sont des éléments de P deux à deux distincts et $i_1, . . . , i_r$ des entiers strictement positifs. Les idéaux maximaux de l’anneau $A/Ay$ sont les idéaux $Ap_1/Ay, . . . ,Ap_r/Ay$; le radical de l’anneau $A/Ay$ est donc l’idéal $Ap_1. . . p_r/Ay$. En particulier, l’anneau $A/Ay$ est sans radical si et seulement si l’on a $i_1=\cdots =i_r= 1$; on dit dans ce cas que $y$ est sans facteur multiple.

#### Proposition 5 {#alg-viii-s9-prop-5 .statement tag=00AF}

a) Le radical d’un anneau A est l’intersection des annulateurs des A-modules simples, et aussi le plus petit des annulateurs des A-modules semi-simples. C’est en particulier un idéal bilatère de A. Si A n’est pas réduit à 0, le radical de A est distinct de A.

b) Soit $\mathfrak{a}$ un idéal bilatère de A. On a $(\mathfrak{R}(A) +\mathfrak{a})/\mathfrak{a}\subset \mathfrak{R}(A/\mathfrak{a})$. Si $\mathfrak{a}$ est contenu dans $\mathfrak{R}(A)$, on a $\mathfrak{R}(A/\mathfrak{a}) =\mathfrak{R}(A)/\mathfrak{a}$.

c) L’anneau $A/\mathfrak{R}(A)$est sans radical ; réciproquement, tout idéal bilatère $\mathfrak{a}$ de A tel que $A/\mathfrak{a}$ soit sans radical contient $\mathfrak{R}(A)$.

d) Le radical de A est contenu dans l’intersection des idéaux bilatères maximaux de A.

Soit $x\in A$. Dire que $x$ appartient à l’annulateur de tout A-module simple revient à dire que $x$ appartient à l’annulateur de tout élément de tout A-module simple, autrement dit (VIII, p. 42, prop. 1) à tout idéal à gauche maximal de A.

Soit M un A-module semi-simple. Son annulateur est l’intersection des annulateurs des sous-modules simples de M, donc il contient $\mathfrak{R}(A)$. Par ailleurs, si $\mathscr{S}$ est l’ensemble des classes de A-modules simples (VIII, p. 47), la somme directe $\oplus_{\lambda\in\mathscr{S}}\lambda$ est un A-module semi-simple, dont l’annulateur est $\mathfrak{R}(A)$. Supposons A non réduit à 0 ; la relation $\mathfrak{R}(A)\not= A$ résulte de la prop. 2, a) de VIII, p. 149, appliquée au A-module $A_s$. On a prouvé a).

Soit $\mathfrak{a}$ un idéal bilatère de A. Les idéaux à gauche maximaux de $A/\mathfrak{a}$ sont les idéaux de la forme $\mathfrak{m}/\mathfrak{a}$, où $\mathfrak{m}$ est un idéal à gauche maximal de A contenant $\mathfrak{a}$. Par suite, le radical de l’anneau $A/\mathfrak{a}$ est égal au radical du A-module $A_s/\mathfrak{a}$. Les assertions b) et c) résultent donc du cor. 1 de VIII, p. 148.

Soit $\mathfrak{a}$ un idéal bilatère maximal de A. Dans l’anneau $A/\mathfrak{a}$, les seuls idéaux bilatères sont 0 et $A/\mathfrak{a}$. Comme l’anneau $A/\mathfrak{a}$ n’est pas réduit à 0, son radical n’est pas égal à $A/\mathfrak{a}$. L’anneau $A/\mathfrak{a}$ est donc sans radical, et l’on a $\mathfrak{R}(A)\subset \mathfrak{a}$ d’après c). Cela prouve d).

On dit qu’un idéal à gauche (ou à droite) de A est un nilidéal s’il se compose d’éléments nilpotents. On dit qu’un idéal bilatère $\mathfrak{a}$ de A est nilpotent s’il existe un entier $n\geqslant 1$ tel que $\mathfrak{a}^n= 0$, c’est-à-dire (I, p. 102) tel que l’on ait $x_1. . . x_n= 0$ pour $\dbend$ toute suite $(x_1, . . . , x_n)$ d’éléments de $\mathfrak{a}$. Tout idéal bilatère nilpotent est un nilidéal, mais il peut exister des nilidéaux qui ne sont pas contenus dans un idéal bilatère nilpotent (VIII, p. 162, exerc. 9).

#### Théorème 1 {#alg-viii-s9-thm-1 .statement tag=00S5}

Le radical d’un anneau A se compose des éléments $x\in A$tels que $1 +ax$ soit inversible à gauche (I, p. 15) pour tout $a\in A$. C’est aussi le plus grand des idéaux bilatères $\mathfrak{a}$ tels que $1 +x$ soit inversible pour tout $x\in \mathfrak{a}$. Le radical de A contient tout nilidéal à gauche de A.

L’élément 1 engendre le A-module $A_s$, et $1 +ax$ est inversible à gauche si et seulement s’il engendre le A-module $A_s$. La première assertion du théorème 1 est donc un cas particulier du corollaire de la prop. 2 (VIII, p. 149).

Soit $x\in \mathfrak{R}(A)$. D’après ce qui précède, $1 +x$ est inversible à gauche ; soit $y$ un élément de A tel que $y(1 +x) = 1$. On a alors $1-y=yx$, donc $1-y$ appartient à $\mathfrak{R}(A)$; par suite $y$ est inversible à gauche. Comme $y$ est aussi inversible à droite, il est inversible (I, p. 16, prop. 3) et il en est de même de son inverse à droite $1 +x$.

Soit $\mathfrak{a}$ un idéal à gauche de A tel que $1 +x$ soit inversible pour tout $x\in \mathfrak{a}$; ceci a lieu par exemple si $\mathfrak{a}$ est un nilidéal, puisque la relation $x^n= 0$ entraîne que $1-x+\cdots + (-x)^{n-1}$ est l’inverse de $1 +x$. Soit $x\in \mathfrak{a}$; pour tout $a\in A$, on a $ax\in \mathfrak{a}$, donc $1 +ax$ est inversible, de sorte qu’on a $x\in \mathfrak{R}(A)$. On en déduit que $\mathfrak{a}$ est contenu dans $\mathfrak{R}$(A), d’où le théorème 1.

#### Corollaire 1 {#alg-viii-s9-thm-1-cor-1 .statement tag=00AG}

Le radical de A est égal au radical de l’anneau opposé $A^o$, c’està-dire à l’intersection des idéaux à droite maximaux de A.

Pour tout $x\in \mathfrak{R}$(A), $1 +x$ est inversible dans l’anneau A, donc dans l’anneau $A^o$; comme $\mathfrak{R}(A)$ est un idéal bilatère de $A^o$, on a $\mathfrak{R}(A)\subset \mathfrak{R}(A^o)$, d’où l’égalité en échangeant les rôles de A et $A^o$.

#### Corollaire 2 {#alg-viii-s9-thm-1-cor-2 .statement tag=00AH}

Pour qu’un élément de A soit inversible, il faut et il suffit que son image canonique dans l’anneau $A/\mathfrak{R}(A)$soit inversible.

La condition est évidemment nécessaire. Démontrons qu’elle est suffisante. Soit $x$ un élément de A dont l’image canonique dans l’anneau $A/\mathfrak{R}(A)$ soit inversible. Il existe alors un élément $y$ de A tel que $xy$ appartienne à $1 +\mathfrak{R}(A)$. D’après le th. 1, $xy$ est inversible, de sorte que $x$ est inversible à droite. On démontre de même que $x$ est inversible à gauche.

#### Corollaire 3 {#alg-viii-s9-thm-1-cor-3 .statement tag=00AI}

Le radical du produit d’une famille $(A_i)_{i\in I}$ d’anneaux est le produit des $\mathfrak{R}(A_i)$.

Soit $x= (x_i)_{i\in I}$ un élément de $\prod_{i\in I}A_i$. Pour tout élément $a= (a_i)_{i\in I}$ de $\prod_{i\in I}A_i$, l’élément $1 +ax$ est inversible à gauche si et seulement si $1 +a_ix_i$ est inversible à gauche dans $A_i$ pour tout $i\in I$, d’où le corollaire 3.

#### Corollaire 4 {#alg-viii-s9-thm-1-cor-4 .statement tag=00AJ}

Pour que l’anneau A soit local, il faut et il suffit que l’anneau $A/\mathfrak{R}(A)$soit un corps. Dans ce cas, $\mathfrak{R}(A)$est l’ensemble des éléments non inversibles de A.

Notons $\mathfrak{r}$ l’ensemble des éléments non inversibles de A. Si l’anneau A est local, son radical est égal à $\mathfrak{r}$ (VIII, p. 150, exemple 1) et l’anneau $A/\mathfrak{r}$ est un corps (VIII, p. 24). Inversement, supposons que l’anneau $A/\mathfrak{R}(A)$ soit un corps. D’après le corollaire 2, on a $\mathfrak{r}=\mathfrak{R}$(A), donc $\mathfrak{r}$ est un idéal bilatère de A. Il en résulte que l’anneau A est local (VIII, p. 24, déf. 1).

#### Exemple 4 {#alg-viii-s9-n2-exa-4 .statement tag=00AK}

Soient K un anneau intègre, I un ensemble non vide et A l’anneau de polynômes $K[X_i]_{i\in I}$. Démontrons que l’anneau A est sans radical. Les seuls éléments inversibles de A sont ceux de K (IV, p. 9, cor. 2). Soit $f\in \mathfrak{R}(A)$. Choisissons un élément $i\in I$. Alors $1 +fX_i$ est inversible (th. 1), ce qui implique $f= 0$.

$\dbend$ Remarquons que lorsque K est un corps commutatif, l’anneau $A = K[X_i]_{i\in I}$ est un sous-anneau de $B = K[[X_i]]_{i\in I}$, et qu’on a $\mathfrak{R}(A) = 0$ et $A\cap \mathfrak{R}(B)\not= 0 ($cf. VIII, p. 150, exemple 2).

#### Exemple 5 {#alg-viii-s9-n2-exa-5 .statement tag=00AL}

Soit $\mathfrak{a}$ un idéal bilatère de A. La topologie sur A, compatible avec la structure d’anneau de A, pour laquelle les idéaux $\mathfrak{a}^n$ (pour $n\geqslant 1)$ forment un système fondamental de voisinages de 0 (TG, III, p. 49, exemple 3) s’appelle la topologie $\mathfrak{a}$-adique. Supposons que l’anneau A soit séparé et complet (TG, III, p. 50) pour cette topologie : c’est le cas par exemple lorsque l’idéal $\mathfrak{a}$ est nilpotent. Pour tout $x\in \mathfrak{a}$, la série $\sum^{\infty}_{n=0}(-x)^n$ est alors convergente (TG, III, p. 44, remarque). Soit $y$ sa somme. On a $y-1 =\sum^{\infty}_{n=1}(-x)^n=-xy$, d’où $(1 +x)y= 1$ et on a de même $y(1 +x) = 1$, de sorte que $1 +x$ est inversible. Il en résulte d’après le th. 1 que l’idéal $\mathfrak{a}$ est contenu dans le radical de A.

#### Remarque 1 {#alg-viii-s9-n2-rem-1 .statement tag=00AM}

D’après le théorème 1, tout nilidéal à gauche d’un anneau A est

contenu dans son radical. Soit $x$ un élément nilpotent et central de A ; alors $Ax$ $\dbend$ est un nilidéal de A, donc $x$ appartient au radical de A. Il se peut cependant qu’il existe dans A des éléments nilpotents non nuls, mais que A soit sans radical : par exemple, pour tout entier $n\geqslant 2$, l’anneau de matrices $\mathbf{M}_n(K)$ sur un corps K est simple, donc sans radical (VIII, p. 150, prop. 4) et il contient des éléments nilpotents, par exemple les unités matricielles $E_{ij}$ avec $i\not=j$.

#### Remarque 2 {#alg-viii-s9-n2-rem-2 .statement tag=00AN}

Soit A un anneau commutatif. L’ensemble des éléments nilpotents de A est un idéal $\mathfrak{N}(A)$ de A, qu’on appelle le nilradical de A ; c’est l’intersection des idéaux premiers de A (V, p. 113, prop. 2). On a $\mathfrak{N}(A)\subset \mathfrak{R}(A) ;*$il y a égalité

si A est un anneau artinien (VIII, p. 169, cor. 2), ou bien une algèbre commutative de type fini sur un corps commutatif (AC, V, § 3, n$^{\circ}4$, th. $3)*$. On peut fort bien avoir $\mathfrak{N}(A)\not=\mathfrak{R}(A) :$ c’est le cas lorsque A est l’anneau K[[X]], où K est un corps commutatif : on a $\mathfrak{N}(A) = 0$ et $\mathfrak{R}(A) =$ AX (VIII, p. 150, exemple 2).

### 3. Lemme de Nakayama

#### Proposition 6 {#alg-viii-s9-prop-6 .statement tag=00AO}

Pour tout A-module M, on a $\mathfrak{R}(A)M\subset \mathfrak{R}(M)$et on a égalité si le A-module M est projectif.

Soit P un sous-module maximal de M ; le A-module $M/P$ est simple, donc il est annulé par $\mathfrak{R}(A)$ d’après la prop. 5 de VIII, p. 150. On a donc $\mathfrak{R}(A)M\subset P$ pour tout sous-module maximal P de M, d’où $\mathfrak{R}(A)M\subset \mathfrak{R}(M)$.

On a évidemment $\mathfrak{R}(A_s) =\mathfrak{R}(A)A_s$. Si le A-module M est projectif, il existe un A-module N tel que $M\oplus N$ soit libre, c’est-à-dire somme directe d’une famille $(L_i)_{i\in I}$ de modules isomorphes à $A(\bigoplus)_s$. D’après le cor. 2 de VIII, p. 148, on a $\mathfrak{R}(M\oplus N) =$ $\mathfrak{R}(M)\oplus \mathfrak{R}(N)$ et $\mathfrak{R}_{i\in I}L_i=\bigoplus_{i\in I}\mathfrak{R}(L_i)$; de l’égalité $\mathfrak{R}(L_i) =\mathfrak{R}(A)L_i$, on déduit alors l’égalité $\mathfrak{R}(M) =\mathfrak{R}(A)M$.

#### Théorème 2 {#alg-viii-s9-thm-2 .statement tag=00S6}

Soient M un A-module et $\mathfrak{a}$ un idéal bilatère de A. Supposons satisfaite l’une des deux hypothèses suivantes :

(i) Le A-module M est de type fini et $\mathfrak{a}$ est contenu dans le radical de A ;

(ii) L’idéal $\mathfrak{a}$ est nilpotent.

Si N est un sous-module de M tel que $M = N +\mathfrak{a}M$, on a N = M. En particulier, si le module M n’est pas nul, on a $M\not=\mathfrak{a}M$.

Supposons que M soit de type fini et qu’on ait $\mathfrak{a}\subset \mathfrak{R}(A)$. Soit N un sous-module de M tel que $M = N +\mathfrak{a}M$. D’après la prop. 6, on a $M = N +\mathfrak{R}$(M), d’où M = N d’après la prop. 2, b) de VIII, p. 149.

Supposons maintenant que $\mathfrak{a}$ soit nilpotent, et soit N un sous-module de M tel que $M = N +\mathfrak{a}M$. Par récurrence sur l’entier $n\geqslant 0$, on établit la relation $M = N +\mathfrak{a}^nM$; par hypothèse, il existe un entier $n\geqslant 0$ tel que $\mathfrak{a}^n= 0$, d’où M = N.

La dernière assertion du théorème se déduit de ce qui précède en prenant N égal à 0.

#### Corollaire 1 {#alg-viii-s9-thm-2-cor-1 .statement tag=00R9}

Conservons les hypothèses du théorème 2. Soit $(x_i)_{i\in I}$ une famille d’éléments de M, et soit $x_i$ l’image canonique de $x_i$ dans $M/\mathfrak{a}M$. Si la famille $(x_i)_{i\in I}$ engendre le $(A/\mathfrak{a})$-module $M/\mathfrak{a}M$, la famille $(x_i)_{i\in I}$ engendre le A-module M.

Cela résulte du th. 2 appliqué au sous-module N de M engendré par la famille $(x_i)_{i\in I}$.

#### Corollaire 2 {#alg-viii-s9-thm-2-cor-2 .statement tag=00AP}

Conservons les hypothèses du théorème 2. Soient par ailleurs $M'$ un A-module et $u: M'\rightarrow M$un homomorphisme. Si l’homomorphisme $u$ de $M'/\mathfrak{a}M'$ dans $M/\mathfrak{a}M$déduit de $u$ par passage aux quotients est surjectif, l’homomorphisme $u$ est surjectif.

Il suffit d’appliquer le th. 2 à l’image N de $u:$ en effet, l’image de $u$ est $(N +\mathfrak{a}M)/\mathfrak{a}M$, donc $u$ est surjectif si et seulement si on a $N +\mathfrak{a}M = M$.

### 4. Relèvements d’idempotents

#### Lemme 1 {#alg-viii-s9-lem-1 .statement tag=00AQ}

Soit $a$ un élément d’un anneau A tel que $a-a^2$ soit nilpotent. Il existe un polynôme P appartenant à $X + (X-X^2)\mathbf{Z}[X]$tel que $P(a)$soit idempotent dans A.

Soit $n$ un entier strictement positif tel que $(a-a^2)^n= 0$. Posons P(X) = $1-(1-X^n)^n$. Le polynôme P(X) est multiple de $X^n$ et le polynôme $1-P(X)$ est multiple de $(1-X)^n$, donc $P(X)-P(X)^2$ est multiple de $(X-X^2)^n$ et l’on a $P(a) = P(a)^2$. Par ailleurs $X-P(X)$ est multiple de X et de $1-X$, donc de $X-X^2$.

#### Proposition 7 {#alg-viii-s9-prop-7 .statement tag=00AR}

Soit $\mathfrak{a}$ un nilidéal bilatère de A et soit $e$ un élément idempotent de l’anneau $A/\mathfrak{a}$. Il existe un élément idempotent $e$ de A dont l’image canonique dans $A/\mathfrak{a}$ est égale à $e$.

Soit $a$ un représentant quelconque de $e$ dans A. L’élément $a-a^2$ de A est nilpotent puisqu’il appartient à $\mathfrak{a}$. Choisissons un polynôme $P\in \mathbf{Z}[X]$ satisfaisant aux conditions du lemme 1. On a que $a-P(a)\in A(a-a^2)$ et l’élément $e= P(a)$ de A convient.

$\dbend$ Supposons que $e$ appartienne au centre de l’anneau $A/\mathfrak{a}$. Il n’existe pas nécessairement d’idempotent $e$ dans le centre Z de A, relevant $e$ (VIII, p. 167, exerc. 31) ; cependant, si $e$ appartient à l’image de Z dans $A/\mathfrak{a}$, il se relève en un idempotent de Z puisque $Z\cap \mathfrak{a}$ est un nilidéal de Z.

#### Corollaire 1 {#alg-viii-s9-prop-7-cor-1 .statement tag=00AS}

Soient M et P des A-modules et $u$ une application A-linéaire surjective de P dans M. On suppose que P est projectif et qu’il existe un idéal bilatère nilpotent $\mathfrak{a}$ de A tel que le noyau N de $u$ soit contenu dans $\mathfrak{a}P$. Soient $M'$ et $M''$ des sous-modules de M, tels que M soit somme directe de $M'$ et $M''$. Alors P est somme directe de sous-modules $P'$ et $P''$ tels que $u(P') = M'$ et $u(P'') = M''$.

Notons B le sous-anneau de End$_A(P)$ formé des endomorphismes $f$ de P tels que $f(N)\subset N$. Soit B l’anneau des endomorphismes de M. Pour tout $f\in B$, notons $f$ l’unique endomorphisme de M tel que $f\circ u=u\circ f$. L’application $f\rightarrow f$ est un homomorphisme d’anneaux de B dans B. Comme le module P est projectif, cet homomorphisme est surjectif ; son noyau $\mathfrak{b}$ se compose des endomorphismes $f\in B$ tels que $f(P)\subset N$. Soit $n$ un entier positif tel que $\mathfrak{a}^n= 0$. On a

$$
P =\mathfrak{a}^0P\supset \mathfrak{a}^1P\supset  \cdots  \supset \mathfrak{a}^{n-1}P\supset \mathfrak{a}^nP = 0
$$

et, pour tout $f\in \mathfrak{b}$ et tout entier $j\geqslant 0$,

$$
f(\mathfrak{a}^jP) =\mathfrak{a}^jf(P)\subset \mathfrak{a}^jN\subset \mathfrak{a}^{j+1}P
$$

puisque $N\subset \mathfrak{a}P$ par hypothèse. Pour tout entier naturel $j$ et tout $f\in \mathfrak{b}^j$, on a donc $f(P)\subset \mathfrak{a}^jP$. En particulier, on a $\mathfrak{b}^n= 0$.

Soit $\varepsilon '$ le projecteur de M d’image $M'$ et de noyau $M''$. D’après la prop. 7 appliquée à l’anneau B et à l’idéal bilatère nilpotent $\mathfrak{b}$, il existe un élément idempotent $e'$ de B tel que $e'=\varepsilon '$, c’est-à-dire $\varepsilon '\circ u=u\circ e'$. Posons $e''= 1-e',\varepsilon ''=e''$, $P'=e'$(P), $P''=e''(P)$. Alors P est somme directe des sous-modules de $P'$ et $P''$ et l’on a

$$
u(P') =u(e'(P)) =\varepsilon '(u(P)) =\varepsilon '(M) = M'
$$

l’égalité $u(P'') = M''$ se démontre de manière analogue.

#### Corollaire 2 {#alg-viii-s9-prop-7-cor-2 .statement tag=00AT}

Soit A un anneau et soit $\mathfrak{a}$ un idéal bilatère nilpotent de A. Si P est un A-module projectif, alors $P/\mathfrak{a}P$est un module projectif sur $A/\mathfrak{a}$ et pour que le A-module P soit indécomposable il faut et il suffit que le $A/\mathfrak{a}$-module $P/\mathfrak{a}P$le soit.

Soit P un A-module projectif et soit P le $A/\mathfrak{a}$-module $P/\mathfrak{a}P$. Le A-module P est nul si et seulement si P l’est (th. 2 de VIII, p. 154). On suppose maintenant $P\not= 0$. Comme le $A/\mathfrak{a}$-module P est isomorphe à $A\otimes_AP$, il est projectif (II, p. 84, cor.). Si P est indécomposable, il en est de même de P d’après le cor. 1. Inversement, supposons que P soit décomposable et non nul, et soient $P'$ et $P''$ deux sous-modules non nuls de P tels que $P = P'\oplus P''$. D’après le lemme de Nakayama (VIII, p. 154, th. 2), on a $P'+\mathfrak{a}P\not= P$ et $P''+\mathfrak{a}P\not= P$; si $P'$ et $P''$ sont les images canoniques de $P'$ et $P''$ dans P, on a $P'\not= P, P''\not= P$ et $P = P'\oplus P''$. Cela prouve que P est décomposable.

### 5. Couverture projective d’un module

#### Définition 3 {#alg-viii-s9-def-3 .statement tag=00AU}

Soit A un anneau et soit M un A-module. On appelle couverture projective de M un couple $(P, u)$, où P est un A-module projectif et $u$ un homomorphisme surjectif de P dans M, tel que l’on ait $u(P')\not= M$pour tout sous-A-module $P'$ de P distinct de P.

#### Remarque 1 {#alg-viii-s9-n5-rem-1 .statement tag=00AV}

Pour tout A-module projectif M, le couple $(M,1_M)$ est une couverture projective de M.

#### Remarque 2 {#alg-viii-s9-n5-rem-2 .statement tag=00AW}

Supposons que $(P, u)$ soit une couverture projective du A-module M. Soit $(x_i)_{i\in I}$ une famille d’éléments de P et soit $P'$ le sous-module de P qu’elle engendre ; alors $u(P')$ est engendré par la famille $(u(x_i))_{i\in I}$. Par conséquent, la famille $(x_i)_{i\in I}$ engendre le A-module P si et seulement si la famille $(u(x_i))_{i\in I}$ engendre le A-module M. En particulier, P est de type fini si et seulement si M est de type fini.

#### Proposition 8 {#alg-viii-s9-prop-8 .statement tag=00AX}

Soient M et $M'$ des A-modules, $(P, u)$et $(P', u')$des couvertures projectives de M et $M'$ respectivement et $g: M\rightarrow M'$ une application A-linéaire.

a) Il existe une application A-linéaire $f: P\rightarrow P'$ telle que $u'\circ f=g\circ u$.

b) Soit $f$ une telle application. Si $g$ est surjective (resp. bijective), alors $f$ est surjective (resp. bijective). Si $g$ est injective et que son image est un facteur direct de $M',f$ est injective et son image est un facteur direct de $P'$.

Par hypothèse, le A-module P est projectif et l’application $u'$ est surjective. Par suite, il existe une application A-linéaire $f: P\rightarrow P'$ telle que $g\circ u=u'\circ f$ (II, p. 39, prop. 4), d’où a).

Soit $f$ une telle application. Supposons $g$ surjective. Comme $u$ est surjective, on a $M'=g(u(P)) =u'(f(P))$. Comme $(P', u')$ est une couverture projective de $M'$, on a $f(P) = P'$, donc $f$ est surjective. D’après loc. cit., le noyau de $f$ admet un sous-module supplémentaire $P_1$, d’où $f(P_1) = P'$. Supposons maintenant $g$ bijective. On a $g(u(P_1)) =u'(f(P_1)) =u'(P') = M'$, d’où $u(P_1) = M$. Comme $(P, u)$ est une couverture projective de M, on a $P_1= P$, d’où Ker($f$) $= 0$. Donc $f$ est injective ; comme on sait déjà que $f$ est surjective, $f$ est bijective.

Pour finir, supposons que $g$ soit injective et que son image soit un facteur direct de $M'$. Il existe alors une application A-linéaire $g': M'\rightarrow M$ telle que $g'\circ g= 1_M$. D’après a), il existe une application A-linéaire $f': P'\rightarrow P$ telle que $u\circ f'=g'\circ u'$. On a $u\circ (f'\circ f) =g'\circ u'\circ f= (g'\circ g)\circ u$; d’après l’alinéa précédent, l’application $f'\circ f$ est bijective. Notons $h$ la bijection réciproque ; on a $(h\circ f')\circ f= 1_P$, donc $f$ est injective et son image est un facteur direct de $P'$ (II, p. 21, cor. 2).

#### Corollaire 1 {#alg-viii-s9-prop-8-cor-1 .statement tag=00AY}

Soit M un A-module. Soient $(P, u)$et $(P', u')$des couvertures projectives de M. Il existe un isomorphisme $f$ de P sur $P'$ tel que $u=u'\circ f$.

$\dbend$ On notera que $f$ n’est pas nécessairement déterminé de manière unique par la relation $u=u'\circ f$ (VIII, p. 165, exerc. 21).

#### Corollaire 2 {#alg-viii-s9-prop-8-cor-2 .statement tag=00AZ}

Soit $(P, u)$une couverture projective du A-module M. Si Q est un A-module projectif et $g: Q\rightarrow M$une application linéaire surjective, il existe une application linéaire surjective $f: Q\rightarrow P$telle que $g=u\circ f$.

#### Proposition 9 {#alg-viii-s9-prop-9 .statement tag=00B0}

Soient M un A-module et $(P, u)$une couverture projective de M. Notons $\mathfrak{r}$ le radical de l’anneau A. L’homomorphisme $u: P/\mathfrak{r}P\rightarrow M/\mathfrak{r}M$déduit de $u$ par passage aux quotients est un isomorphisme.

L’homomorphisme $u$ est surjectif par définition, donc $u$ est surjectif. Notons N le noyau de $u$. On a $u^{-1}(\mathfrak{r}M) = N+\mathfrak{r}P$. Démontrons que l’on a $N\subset \mathfrak{r}P$, ce qui entraînera l’injectivité de $u$. Pour tout sous-module maximal $P'$ de P, on a $u(P')\not= M$, d’où $P'+ N\not= P$; comme $P'$ est maximal, on a $N\subset P'$. Le sous-module N de P est donc contenu dans le radical de P ; or celui-ci est égal à $\mathfrak{r}P$ d’après la prop. 6 de VIII, p. 154.

#### Corollaire {#alg-viii-s9-n5-cor-1 .statement tag=00B1}

Pour qu’un A-module M possède une couverture projective, il faut que le $A/\mathfrak{r}$-module $M/\mathfrak{r}M$soit projectif.

En effet, si $(P, u)$ est une couverture projective de M, le $(A/\mathfrak{r}$)-module $M/\mathfrak{r}M$ est isomorphe à $P/\mathfrak{r}P$ (prop. 9) ; comme le A-module P est projectif, le $(A/\mathfrak{r}$)-module $P/\mathfrak{r}P$ est aussi projectif.

#### Remarque 3 {#alg-viii-s9-n5-rem-3 .statement tag=00B2}

Supposons que l’anneau A soit sans radical. D’après la prop. 9, $(P, u)$ est une couverture projective d’un A-module M si et seulement si $u$ est un isomorphisme. Ainsi seuls les A-modules projectifs ont une couverture projective.

L’anneau $\mathbf{Z}$est sans radical (VIII, p. 150, exemple 3). Soit $n\geqslant 2$ un entier. Le $\mathbf{Z}$-module $\mathbf{Z}/n\mathbf{Z}$n’est pas projectif et il n’admet donc pas de couverture projective.

#### Remarque 4 {#alg-viii-s9-n5-rem-4 .statement tag=00B3}

Supposons que tout A-module de type fini possède une couverture projective ; alors le quotient $A'$ de A par son radical est semi-simple. En effet, tout module de type fini sur l’anneau $A'$ est projectif d’après le corollaire. En particulier, pour tout idéal à gauche $\mathfrak{a}$ de $A'$, le $A'$-module $A'_s/\mathfrak{a}$ est projectif. Notre assertion résulte alors de la prop. 4 de VIII, p. 134.

On peut donner un exemple d’un anneau commutatif A pour lequel $A/\mathfrak{r}$ est semi-simple et d’un A-module M de type fini qui n’admet pas de couverture projective (VIII, p. 165, exerc. 22).

#### Proposition 10 {#alg-viii-s9-prop-10 .statement tag=00B4}

Soient M un A-module, P un A-module projectif et $u: P\rightarrow M$ une application linéaire. Soit $\mathfrak{a}$ un idéal bilatère de A . On suppose que l’application linéaire $u: P/\mathfrak{a}P\rightarrow M/\mathfrak{a}M$déduite de $u$ par passage aux quotients est bijective et que l’une des deux hypothèses suivantes est satisfaite :

(i) Les A-modules M et P sont de type fini et $\mathfrak{a}$ est contenu dans le radical de A ;

(ii) L’idéal $\mathfrak{a}$ est nilpotent.

Alors $(P, u)$est une couverture projective de M.

Sous les hypothèses faites, l’homomorphisme $u$ est surjectif (VIII, p. 154, cor. 2), et son noyau N est contenu dans $\mathfrak{a}P$. Soit $P'$ un sous-module de P, distinct de P. D’après le lemme de Nakayama (VIII, p. 154, th. 2), on a $P'+\mathfrak{a}P\not= P$ et donc $u(P')\not= M$. Donc $(P, u)$ est une couverture projective de M.

#### Corollaire 1 {#alg-viii-s9-prop-10-cor-1 .statement tag=00B5}

Soit P un A-module projectif. On suppose que P est de type fini ou que le radical $\mathfrak{r}$ de A est un idéal bilatère nilpotent. Notons $u$ l’application canonique de P sur $P/\mathfrak{r}P$. Alors $(P, u)$est une couverture projective de $P/\mathfrak{r}P$.

#### Corollaire 2 {#alg-viii-s9-prop-10-cor-2 .statement tag=00B6}

Soient $\mathfrak{a}$ un idéal bilatère de A et M un A-module tel que le $(A/\mathfrak{a})$-module $M/\mathfrak{a}M$soit libre. Supposons satisfaite l’une des deux conditions suivantes :

(i) Le module M est de type fini et $\mathfrak{a}$ est contenu dans le radical de A ;

(ii) L’idéal $\mathfrak{a}$ est nilpotent.

Alors M possède une couverture projective.

Plus précisément, soient P un A-module libre, $(e_i)_{i\in I}$ une base de P et $u: P\rightarrow M$ un homomorphisme tel que les images canoniques des éléments $u(e_i)$dans $M/\mathfrak{a}M$ forment une base du $(A/\mathfrak{a})$-module $M/\mathfrak{a}M$. Alors $(P, u)$est une couverture projective de M.

En effet, le $(A/\mathfrak{a}$)-module $P/\mathfrak{a}P$ est libre et l’homomorphisme $u$ de $P/\mathfrak{a}P$ dans $M/\mathfrak{a}M$ déduit de $u$ par passage aux quotients transforme une base de $P/\mathfrak{a}P$ en une base de $M/\mathfrak{a}M$, donc est bijectif.

Si $\mathfrak{a}$ est nilpotent, il suffit alors d’appliquer la prop. 10. Supposons maintenant que l’anneau A est non nul et que le A-module M est de type fini ; il en est alors de même du $(A/\mathfrak{a}$)-module $M/\mathfrak{a}M$, et par conséquent du $(A/\mathfrak{a}$)-module $P/\mathfrak{a}P$. Toute base de $P/\mathfrak{a}P$ est alors finie. Il en résulte que l’ensemble I est fini et que le A-module P est de type fini. On applique alors à nouveau la prop. 10.

#### Corollaire 3 {#alg-viii-s9-prop-10-cor-3 .statement tag=00B7}

Tout module de type fini sur un anneau local possède une couverture projective.

Soient A un anneau local et $\mathfrak{r}$ son radical. C’est un idéal bilatère de A (VIII, p. 150, prop. 5, a)) et l’anneau $A/\mathfrak{r}$ est un corps (VIII, p. 152, cor. 4). Si M est un A-module, $M/\mathfrak{r}M$ est un espace vectoriel sur le corps $A/\mathfrak{r}$, donc un $(A/\mathfrak{r}$)-module libre. Il suffit alors d’appliquer le cor. 2.

#### Remarque 5 {#alg-viii-s9-n5-rem-5 .statement tag=00B8}

Soient A un anneau local et $\mathfrak{r}$ son radical. Soient M un A-module de type fini, P un A-module projectif de type fini et $u: P\rightarrow M$ un homomorphisme. D’après le cor. 6 de VIII, p. 33, le A-module P est libre. Choisissons-en une base $(e_i)_{i\in I}$. Posons $x_i=u(e_i)$ et notons $x_i$ l’image canonique de $x_i$ dans $M/\mathfrak{r}M$. Les conditions suivantes sont équivalentes :

(i) Le couple $(P, u)$ est une couverture projective de M ;

(ii) La famille $(x_i)_{i\in I}$ est une famille génératrice minimale du A-module M ;

(iii) La famille $(x_i)_{i\in I}$ est une base de l’espace vectoriel $M/\mathfrak{r}M$ sur le corps $A/\mathfrak{r}$. On a en effet (i) $=\Rightarrow$ (ii) d’après la remarque 2 de VIII, p. 157 et (iii) $=\Rightarrow$ (i) d’après le cor. 2. Par ailleurs, si la famille $(x_i)$ est une famille génératrice minimale du A-module M, la famille $(x_i)$ est une famille génératrice minimale, c’est-à-dire une base, de l’espace vectoriel $M/\mathfrak{r}M$ sur $A/\mathfrak{r}$ (VIII, p. 154, cor. 1).

#### Proposition 11 {#alg-viii-s9-prop-11 .statement tag=00B9}

Soient A un anneau et $\mathfrak{a}$ un idéal bilatère nilpotent de A. Soit M un $A/\mathfrak{a}$-module projectif. Il existe un A-module projectif P et une application A-linéaire surjective $u: P\rightarrow M$, de noyau $\mathfrak{a}P$.

Un tel couple $(P, u)$est une couverture projective de M considéré comme A-module.

Il existe un $A/\mathfrak{a}$-module $M'$ tel que $M\oplus M'$ soit un $A/\mathfrak{a}$-module libre. Choisissons un A-module libre L et une application A-linéaire surjective $v: L\rightarrow M\oplus M'$ de noyau $\mathfrak{a}L$. D’après le cor. 1 de la prop. 7 (VIII, p. 155), il existe une décomposition en somme directe $L = P\oplus P'$ telle que $v(P) = M$ et $v(P') = M'$. Le A-module P est projectif et l’application A-linéaire $u$ de P dans M qui coïncide avec $v$ sur P est surjective, de noyau $\mathfrak{a}P$. La première assertion en résulte.

Soient P un A-module projectif, et $u$ un homomorphisme de P sur M, de noyau $\mathfrak{a}P$. D’après la prop. 10, $(P, u)$ est une couverture projective de M.

#### Corollaire {#alg-viii-s9-n5-cor-2 .statement tag=00RA}

Soient P et $P'$ des A-modules projectifs. Si les modules $P/\mathfrak{a}P$et $P'/\mathfrak{a}P'$ sont isomorphes, alors P et $P'$ sont isomorphes.

Comme $P/\mathfrak{a}P$ et $P'/\mathfrak{a}P'$ sont projectifs, le corollaire résulte de la prop. 11 et de l’unicité de la couverture projective (VIII, p. 157, cor. 1).

## EXERCICES {#alg-viii-s9-exercises}

See the [exercises for § 9](exercises/s9/).
