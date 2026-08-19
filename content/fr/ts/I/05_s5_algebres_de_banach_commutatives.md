---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 5
section_title: Algèbres de Banach commutatives régulières
lang: fr
source: ts-i-ii-fr
book_pages: TS I.88-TS I.95, TS I.178-TS I.180
pdf_pages: 0101-0108, 0191-0193
extraction: native
subsections:
    - "no": 1
      title: Définition
      page: 88
      pdf_page: 101
    - "no": 2
      title: Synthèse harmonique
      page: 91
      pdf_page: 104
statements: 16
exercises: 7
content_sha256: 3b8b45af0b54b3bf0b9093138e784b60c042ad9a881e2bc1d672c05060435ac9
---

## § 5. ALGÈBRES DE BANACH COMMUTATIVES RÉGULIÈRES

Dans cette section, le corps de base est $\mathbf{C}$.

### 1. Définition

#### Proposition 1 {#ts-i-s5-prop-1 .statement tag=02BV}

Soit A une algèbre de Banach commutative. Les conditions suivantes sont équivalentes :

(i) La topologie faible et la topologie de Jacobson sur $\mathsf{X}(A)$ coïn-cident ;

(ii) Pour tout $\chi \in \mathsf{X}(A)$ et toute partie faiblement fermée F de $\mathsf{X}(A)$ telle que $\chi \notin F$, il existe un $x\in A$ tel que $\mathscr{G}(x)$ soit égale à 1 en $\chi$ et à 0 sur F;

(iii) Pour toute partie faiblement compacte K et toute partie faiblement fermée F de $\mathsf{X}(A)$ telles que $K\cap F =\emptyset$, il existe un élément $x\in A$ tel que $\mathscr{G}(x)$ soit égale à 1 sur K et à 0 sur F.

Soit $M\subset \mathsf{X}(A)$. Dire que M est fermé pour la topologie de Jacobson signifie que, pour tout $\chi \in \mathsf{X}(A)$ - M, il existe un $x\in A$ tel que $\mathscr{G}(x)$ s’annule sur M mais pas en $\chi$ (lemme 2 de I, p. 39). La condition (ii) signifie donc que toute partie de $\mathsf{X}(A)$ faiblement fermée est fermée pour la topologie de Jacobson, ce qui montre que (ii) $=\Rightarrow$ (i). Par ailleurs (iii) $=\Rightarrow$ (ii) puisque la partie $\{\chi \}$ est faiblement compacte dans $\mathsf{X}(A)$. Enfin (i) $=\Rightarrow$ (iii) d’après le cor. de la prop. 15 de I, p. 81.

#### Définition 1 {#ts-i-s5-def-1 .statement tag=02BW}

Soit A une algèbre de Banach commutative. Elle est dite régulière si elle vérifie les conditions équivalentes de la proposition 1.

#### Remarque {#ts-i-s5-n1-rem-1 .statement tag=02BX}

Soit $\widetilde{A}$ l’algèbre de Banach déduite de A par adjonction d’un élément unité $e$. La condition (ii) de la prop. 1 montre que si $\widetilde{A}$ est régulière, alors A est régulière. Supposons A régulière et montrons que $\widetilde{A}$ est régulière. Considérons des parties F et $F'$ de $\mathsf{X}(\widetilde{A})$ qui sont disjointes et faiblement fermées (donc faiblement compactes) et construisons un $x\in \widetilde{A}$ tel que $\mathscr{G}(x)$ s’annule sur F, et soit égale à 1 sur $F'$. Soit $\chi_0\in \mathsf{X}(\widetilde{A})$ le caractère nul sur A. Si $\chi_0\notin F'$, il existe, d’après la condition (iii) de la prop. 1 et l’hypothèse sur A, un élément $x\in A$ tel que $\mathscr{G}(x)$ s’annule sur F et soit égale à 1 sur $F'$. Si $\chi_0\in F'$, on a $\chi_0\notin F$; il existe donc un élément $y\in A$ tel que $\mathscr{G}(y)$ s’annule sur $F'$ et soit égale à 1 sur F. L’élément $x=e-y$ de $\widetilde{A}$ a alors la propriété demandée.

#### Exemple {#ts-i-s5-n1-exa-1 .statement tag=02BY}

Reprenons les exemples du n$^o2$ de I, p. 17.

L’algèbre des fonctions continues à valeurs complexes tendant vers 0 à l’infini sur un espace localement compact X (exemple 3 de I, p. 17) est régulière (cf. I, p. 36, exemple 1).

L’algèbre des fonctions $n$ fois dérivables sur $[0,1]$ (exemple 4 de I, p. 18) est régulière (cf. I, p. 36, exemple 2).

Si G est un groupe localement compact commutatif et $\mu$ une mesure de Haar sur G, alors l’algèbre $L^1(G, \mu)$ (exemple 7 de I, p. 19) est régulière (cf. II, p. 219, cor. 2).

L’algèbre des fonctions qui sont continues dans le disque $|z|\leqslant 1$ et analytiques à l’intérieur (exemple 9 de I, p. 20) n’est pas régulière (cf. I, p. 193, exerc. 6).

#### Proposition 2 {#ts-i-s5-prop-2 .statement tag=02BZ}

Soit A une algèbre de Banach unifère commutative régulière. Soient $n\geqslant 1$ un entier et $(U_1, . . . ,U_n)$ un recouvrement ouvert de $\mathsf{X}(A)$. Il existe des éléments $x_1, . . . , x_n$ de A de somme 1 tels que Supp($\mathscr{G}(x_i)$)$\subset U_i$ pour $i= 1, . . . ,n$.

Démontrons la proposition par récurrence sur $n$. L’assertion est valide si $n= 1$. Supposons que $n\geqslant 2$ et que l’assertion est établie pour $n-1$.

Il existe un recouvrement ouvert $(V_1, . . . ,V_n)$ de $\mathsf{X}(A)$ tel que $\overline{V}_i\subset$ $U_i$ pour tout $i$. D’après l’hypothèse de récurrence, il existe des éléments $x, x_3, . . . , x_n\in A$ tels que $x+x_3+\cdots +x_n= 1$ et Supp($\mathscr{G}(x)$)$\subset V_1\cup V_2$, Supp($\mathscr{G}(x_i)$)$\subset V_i$ pour $i\geqslant 3$. Notons K = Supp($\mathscr{G}(x)$)$\subset V_1\cup V_2$. Soit $K_1$ (resp. $K_2$) l’ensemble des éléments de K qui n’appartiennent pas à $V_1$ (resp. $V_2$). Alors $K_1$ et $K_2$ sont des parties compactes disjointes de K. Puisque l’algèbre de Banach A est régulière, il existe donc $y\in A$ tel que $\mathscr{G}(y) = 1$ sur $K_1$ et $\mathscr{G}(y) = 0$ sur $K_2$. Alors $\mathscr{G}(xy)$ est nulle sur $\mathsf{X}(A)-K$ et sur $K_2$, donc Supp $\mathscr{G}(xy)\subset \overline{V}_2\subset U_2$. De même, $\mathscr{G}(x(1-y))$ est nulle sur $\mathsf{X}(A)$ - K et sur $K_1$, donc Supp $\mathscr{G}(x(1-y))\subset \overline{V}_1\subset U_1$. Les éléments $x_1=x(1-y),x_2=xy$, et $x_3, . . . ,x_n$ vérifient alors les propriétés de la proposition.

#### Corollaire 1 {#ts-i-s5-prop-2-cor-1 .statement tag=02C0}

Soit A une algèbre de Banach unifère commutative régulière, soit I un idéal de A et soit $f:\mathsf{X}(A)\rightarrow \mathbf{C}$ une fonction continue. On suppose que, pour tout $\chi \in \mathsf{X}(A)$, il existe un élément $y_{\chi}\in I$ tel que $f=\mathscr{G}(y_{\chi})$ au voisinage de $\chi$. Alors il existe un élément $y\in I$ tel que $f=\mathscr{G}(y)$.

Comme $\mathsf{X}(A)$ est compact, il existe un recouvrement ouvert fini $(U_1, . . . ,U_n)$ de $\mathsf{X}(A)$, et des éléments $y_1, . . . , y_n$ de I tels que $f=\mathscr{G}(y_i)$ sur $U_i$. D’après la prop. 2, il existe des éléments $x_1, . . . , x_n$ de A de somme 1 tels que Supp($\mathscr{G}(x_i)$)$\subset U_i$ pour tout $i$. Soit $y=x_1y_1+\cdots +$ $x_ny_n$. C’est un élément de I qui a la propriété demandée. En effet, soit $\chi \in \mathsf{X}(A)$. Pour $1\leqslant i\leqslant n$, on a $\mathscr{G}(x_i)(\chi )\mathscr{G}(y_i)(\chi ) =\mathscr{G}(x_i)(\chi )f(\chi )$ puisque $\mathscr{G}(y_i)(\chi ) =f(\chi )$ si $\chi \in U_i$, et $\mathscr{G}(x_i)(\chi ) = 0$ si $\chi  /\in U_i$. Il vient donc

$$
\mathscr{G}(y)(\chi ) =\sum_{i=1}^n\mathscr{G}(x_i)(\chi )\mathscr{G}(y_i)(\chi ) =f(\chi )\sum_{i=1}^n\mathscr{G}(x_i)(\chi ) =f(\chi )
$$

#### Corollaire 2 {#ts-i-s5-prop-2-cor-2 .statement tag=02C1}

Soient A une algèbre de Banach commutative régulière, I un idéal de A et $f:\mathsf{X}'(A)\rightarrow \mathbf{C}$ une fonction continue. On suppose que, pour tout $\chi \in \mathsf{X}'(A)$, il existe un élément $y_{\chi}\in I$ tel que $f=\mathscr{G}'(y_{\chi})$ au voisinage de $\chi$. Alors il existe un élément $y\in I$ tel que $f=\mathscr{G}'(y)$.

Soit $\widetilde{A}$ l’algèbre de Banach déduite de A par adjonction d’un élément unité. Alors $\widetilde{A}$ est régulière (remarque 1), et $\mathsf{X}'(A) =\mathsf{X}(\widetilde{A})$; il suffit donc d’appliquer le cor. 1 à $\widetilde{A}$ et à l’idéal I.

Si I est un idéal d’une algèbre de Banach commutative, rappelons (cf. I, p. 30) que nous notons V(I) l’ensemble des $\chi \in \mathsf{X}(A)$ dont le noyau contient I, autrement dit l’ensemble des $\chi \in \mathsf{X}(A)$ où s’annulent toutes les fonctions $\mathscr{G}(x)$ pour $x\in I$. C’est une partie de $\mathsf{X}(A)$ fermée pour la topologie de Jacobson.

#### Proposition 3 {#ts-i-s5-prop-3 .statement tag=02C2}

Soient A une algèbre de Banach commutative régulière, I un idéal de A et K une partie de $\mathsf{X}(A)$ compacte et disjointe de V(I). Il existe un élément $x\in I$ tel que $\mathscr{G}(x) = 1$ pour tout $x$ dans K.

C’est un cas particulier de la prop. 15 de I, p. 81 compte tenu du fait que la topologie de Jacobson coïncide avec la topologie faible sur $\mathsf{X}(A)$.

### 2. Synthèse harmonique

Soit A une algèbre de Banach commutative. Rappelons que si M est une partie de $\mathsf{X}(A)$, nous notons Υ(M) l’intersection des noyaux des éléments de M (cf. I, p. 30) ; c’est un idéal de A.

#### Proposition 4 {#ts-i-s5-prop-4 .statement tag=02C3}

Soit A une algèbre de Banach commutative régulière sans radical. Soit F une partie fermée de $\mathsf{X}(A)$. L’ensemble des idéaux I de A tels que V(I) = F, ordonné par l’inclusion, admet un plus grand élément, à savoir Υ(F), et un plus petit élément, à savoir l’ensemble J des $x\in A$ tels que $\mathscr{G}(x)$ soit à support compact disjoint de F.

Par construction, Υ(F) est un idéal de A tel que V(Υ(F)) contient F, et c’est le plus grand idéal de A ayant cette propriété. Puisque F est fermé, il existe un idéal I de A tel que V(I) = F ; on a donc $I\subset \Upsilon (F)$, d’où $V(\Upsilon (F))\subset V(I) = F$, si bien que V(Υ(F)) = F. Cela prouve la première assertion.

L’ensemble J est un idéal de A et V(J) contient F. Montrons que V(J) = F. Soit $\chi \in \mathsf{X}(A)$ n’appartenant pas à F. Soit U un voisinage compact de $\chi$ ne rencontrant pas F (TG, I, p. 65, cor. de la prop. 9). D’après l’assertion (ii) de la prop. 1 de I, p. 88, il existe $x\in A$ tel que $\mathscr{G}(x)$ soit égale à 1 en $\chi$ et à 0 hors de U. On a alors $x\in J$ et donc $\chi \notin V(J)$. Cela montre que $V(J)\subset F$ et donc V(J) = F.

Enfin, soit I un idéal de A tel que V(I) = F. Montrons que $J\subset I$. Soit $x\in J$ et soit C le support de $\mathscr{G}(x)$ ; la partie C est une partie compacte de $\mathsf{X}(A)$ disjointe de F. D’après la prop. 3, il existe un élément $u\in I$ tel que $\mathscr{G}(u) = 1$ sur C. On a alors $\mathscr{G}(x) =\mathscr{G}(ux)$, et donc $x=ux$ puisque A est sans radical (prop. 8 de I, p. 38). Par conséquent, on a $x\in I$, ce qui montre que $J\subset I$.

#### Corollaire 1 {#ts-i-s5-prop-4-cor-1 .statement tag=02C4}

Soit A une algèbre de Banach commutative régulière sans radical. Soit J l’ensemble des $x\in A$ tels que $\mathscr{G}(x)$ soit à support compact. On suppose que J = A. Alors tout idéal fermé de A et distinct de A est contenu dans un idéal maximal régulier.

Si I est un idéal fermé de A qui n’est contenu dans aucun idéal maximal régulier, alors $V(I) =\emptyset$, donc $I\supset J$ (prop. 4 appliquée à F = $\emptyset$ ), d’où $I\supset \overline{J}= A$.

#### Corollaire 2 {#ts-i-s5-prop-4-cor-2 .statement tag=02C5}

Soit A une algèbre de Banach commutative régulière sans radical. Soient $x, y\in A$. Si le support de $\mathscr{G}(x)$ est compact et contenu dans l’ensemble des caractères $\chi$ tels que $\mathscr{G}(y)(\chi )\not= 0$, alors $x$ est un multiple de $y$ dans A.

Soit I l’idéal $Ay$ de A. Alors V(I) est l’ensemble des zéros de $\mathscr{G}(y)$. Puisque le support F de $\mathscr{G}(x)$ est compact et disjoint de V(I), on a $x\in I$ (prop. 4 appliquée à F).

#### Définition 2 {#ts-i-s5-def-2 .statement tag=02C6}

Soit A une algèbre de Banach commutative.

Soient I un idéal de A$,x\in A$, et $\chi \in \mathsf{X}'(A)$. On dit que $x$ appartient à I au voisinage de $\chi$ s’il existe un élément $y\in I$ tel que $\mathscr{G}'(y)$ et $\mathscr{G}'(x)$ coïncident au voisinage de $\chi$.

On dit que A vérifie la condition de Ditkin si, pour tout $\chi \in \mathsf{X}'(A)$ et tout $x\in A$ tel que $\mathscr{G}'(x)$ s’annule en $\chi$, il existe une suite $(x_n)$ dans A telle que $x=$ lim$_{n\rightarrow \infty}x_nx$ et telle que chaque $\mathscr{G}'(x_n)$ s’annule dans un voisinage $V_n$ de $\chi$.

#### Remarque {#ts-i-s5-n2-rem-1 .statement tag=02C7}

Soit A une algèbre de Banach commutative.

1) Si $\chi$ est tel que $\mathscr{G}'(x)$ s’annule au voisinage de $\chi$, alors $x$ appartient à I au voisinage de $\chi$.

2) Si $x$ appartient à I au voisinage de $\chi$ et $y\in A$ est un élément quelconque, alors $xy$ appartient à I au voisinage de $\chi$.

3) L’ensemble des $\chi$ tels que $x$ appartient à I au voisinage de $\chi$ est ouvert dans $\mathsf{X}'(A)$.

4) Supposons que A est régulière et sans radical. Si $x$ appartient à I au voisinage de $\chi$ pour tout $\chi \in \mathsf{X}'(A)$, alors $x$ appartient à I (cor. 2 de I, p. 91 appliqué à la fonction $f=\mathscr{G}'(x)$ et prop. 8 de I, p. 38).

5) Supposons que A est régulière. Soient I un idéal de A et $\chi$ un élément de $\mathsf{X}(A)$ tel que $\chi \notin V(I)$. Alors tout élément $x$ de A appartient à I au voisinage de $\chi$. En effet, d’après la déf. 1 de I, p. 89, il existe un $z\in A$ tel que $\mathscr{G}'(z)$ soit égale à 1 au voisinage de $\chi$, et égale à 0 au voisinage de V(I). Le support de $\mathscr{G}(z)$ est compact et donc on a $z\in I$ (prop. 4 appliquée à V(I)), donc $xz\in I$, et $\mathscr{G}'(xz) =\mathscr{G}'(x)$ au voisinage de $\chi$.

Rappelons qu’un sous-espace K d’un espace topologique X est dit parfait s’il est fermé sans point isolé (TG, I, p. 8).

#### Lemme 1 {#ts-i-s5-lem-1 .statement tag=02C8}

Soit A une algèbre de Banach commutative régulière sans radical, vérifiant la condition de Ditkin. Soient I un idéal fermé de A et $x$ un élément de Υ(V(I)). Soit K l’ensemble des $\chi \in \mathsf{X}'(A)$ tels que $x$ n’appartienne pas à I au voisinage de $\chi$. Alors l’ensemble K est une partie parfaite de $\mathsf{X}'(A)$.

Notons G le complémentaire de K dans $\mathsf{X}'(A)$. L’ensemble G est ouvert dans $\mathsf{X}'(A)$ (remarque 3) donc K est fermé.

Procédons par contradiction, et supposons que K admette un point isolé $\chi_0$. Notons U un voisinage de $\chi_0$ tel que U $-\{\chi_0\} \subset G$. Comme $x$ n’appartient pas à I au voisinage de $\chi_0$, la remarque 5 démontre que $\chi_0\in V(I)$. En particulier, on a $\chi_0(x) = 0$ puisque $x\in \Upsilon (V(I))$.

Nous allons montrer qu’il existe un élément $y$ de A qui appartient à I au voisinage de tout point de $\mathsf{X}'(A)-\{\chi_0\}$, qui n’appartient pas à I au voisinage de $\chi_0$, et tel que $\chi_0(y) = 0$.

Supposons tout d’abord démontrée l’existence d’un tel élément $y$. Puisque A vérifie la condition de Ditkin, il existe alors une suite $(x_n)$ dans A telle que $x_ny$ tende vers $y$ et telle que chaque $\mathscr{G}'(x_n)$ s’annule dans un voisinage de $\chi_0$. Pour tout $n$, l’élément $x_ny$ appartient alors à I au voisinage de tout point de $\mathsf{X}'(A)$ (remarques 1 et 2) et donc $x_ny\in I$ (remarque 4). Puisque I est fermé, on en déduit que $y\in I$, ce qui contredit le fait que $y$ n’appartient pas à I au voisinage de $\chi_0$.

Il reste à démontrer l’existence de $y$. Si $\chi_0\not= 0$, d’après l’assertion (iii) de la prop. 1 de I, p. 88, il existe un $u\in A$ tel que $\mathscr{G}'(u)$ soit égale à 1 au voisinage de $\chi_0$ et égale à 0 au voisinage de $\mathsf{X}'(A)$ - U. Soit $y=ux$. Puisque $x$ appartient à I au voisinage de $\chi$ pour tout $\chi \in U-\{\chi_0\}$, il en est de même de $y$. De plus, si $\chi \in \mathsf{X}'(A)$ - U, alors $\mathscr{G}'(y)$ s’annule au voisinage de $\chi$. Donc (remarque 5) l’élément $y=ux$ appartient à I au voisinage de tout $\chi \not=\chi_0$. Comme $\mathscr{G}'(y)$ coïncide avec $\mathscr{G}'(x)$ au voisinage de $\chi_0$, le fait que $\chi_0$ appartienne à K implique que $y$ n’appartient pas à I au voisinage de $\chi_0$. Finalement, on a $\chi_0(y) =\chi_0(u)\chi_0(x) = 0$.

Si $\chi_0= 0$, il existe similairement un élément $v\in A$ tel que $\mathscr{G}'(v)$ soit nulle au voisinage de $\chi_0$ et égale à 1 au voisinage de $\mathsf{X}'(A)$- U ; comme précédemment, on en déduit que l’élément $y=x-vx$ appartient à I au voisinage de tout $\chi \not=\chi_0$, qu’il n’appartient pas à I au voisinage de $\chi_0$, et que $\chi_0(y) = 0$.

#### Lemme 2 {#ts-i-s5-lem-2 .statement tag=02C9}

Soit X un espace topologique. Soient F et D des sous-espaces de X disjoints tels que F soit fermé et D discret. Si F ne contient pas de sous-espace parfait non vide, il en est de même de $F\cup D$.

Supposons en effet que K est un sous-espace parfait non vide de $F\cup D$. Soit $x$ un point de K. Si $x$ appartient à D, il est isolé dans D, donc également dans $F\cup D$ puisque F est fermé. Donc $x$ est isolé dans K, ce qui contredit les hypothèses.

#### Proposition 5 {#ts-i-s5-prop-5 .statement tag=02CA}

Soit A une algèbre de Banach commutative régulière sans radical, vérifiant la condition de Ditkin. Soit I un idéal fermé de A tel que la frontière F de V(I) ne contienne aucun ensemble parfait non vide. Alors I = Υ(V(I)), c’est-à-dire que I est l’ensemble des $x\in A$ tels que $\mathscr{G}(x)$ s’annule sur V(I). En particulier, si V(I) se réduit à un point $\chi$, on a I = Ker($\chi$ ).

On a $I\subset \Upsilon (V(I))$. Soit maintenant $x\in \Upsilon (V(I))$. Soit G l’ensemble des caractères $\chi \in \mathsf{X}'(A)$ tels que $x$ appartienne à I au voisinage de $\chi$. Il est ouvert et son complémentaire K est parfait (lemme 1). Comme $\mathscr{G}'(x)$ est nulle sur V(I), l’ensemble G contient l’intérieur de $V(I)\cup  \{0\}$ (remarque 1). Il contient également $\mathsf{X}(A)$- V(I) d’après la remarque 5. Donc $K =\mathsf{X}'(A)$ - G est contenu dans la frontière $F_0$ de $V(I)\cup  \{0\}$. On a $F_0\subset F\cup  \{0\}$. L’hypothèse implique donc que $F_0$ ne contient pas d’ensemble parfait non vide (lemme 2). Il découle donc du lemme 1 que l’ensemble parfait K est vide. Donc $x$ appartient à I au voisinage de tout $\chi \in \mathsf{X}'(A)$, ce qui signifie que $x\in I$ (remarque 4). Ainsi $\Upsilon (V(I))\subset$ I, ce qui conclut la preuve.

## EXERCICES {#ts-i-s5-exercises}

Dans les exercices ci-dessous, toutes les algèbres considérées sont sur $\mathbf{C}$.

See the [exercises for § 5](exercises/s5/).
