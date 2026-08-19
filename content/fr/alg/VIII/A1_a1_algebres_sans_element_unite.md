---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 1
section_title: Algèbres sans élément unité
appendix: true
lang: fr
source: alg-viii-fr
book_pages: A VIII.425-A VIII.436
pdf_pages: 0427-0438
extraction: native
subsections:
    - "no": 1
      title: Idéaux réguliers
      page: 425
      pdf_page: 427
    - "no": 2
      title: Adjonction d’un élément unité
      page: 427
      pdf_page: 429
    - "no": 3
      title: Radical d’une algèbre
      page: 429
      pdf_page: 431
    - "no": 4
      title: Théorème de densité
      page: 431
      pdf_page: 433
statements: 20
exercises: 15
content_sha256: 737dd3f8a42a9f905011149a420c6322acab9083235b98beb184aa04a02de142
---

### APPENDICE 1 ALGÈBRES SANS ÉLÉMENT UNITÉ

Dans cet appendice, la lettre $k$ désigne un anneau commutatif ; les $k$-algèbres sont supposées associatives mais non nécessairement unifères.

### 1. Idéaux réguliers

Soit A une $k$-algèbre. Rappelons (III, p. 4) qu’on appelle idéal à gauche de A un sous-$k$-module $\mathfrak{a}$ de A tel que les relations $a\in A, x\in \mathfrak{a}$ entraînent $ax\in \mathfrak{a}$. On définit de façon similaire les notions d’idéal à droite et d’idéal bilatère. Si A est une $k$-algèbre et $\mathfrak{a}$ un idéal bilatère de A, la multiplication de A définit par passage aux quotients une structure de $k$-algèbre sur le $k$-module $A/\mathfrak{a}($loc. cit.).

On dit qu’un idéal à gauche de A est maximal si c’est un élément maximal de l’ensemble des idéaux à gauche de A distincts de A pour la relation d’inclusion.

#### Définition 1 {#alg-viii-a1-def-1 .statement tag=00P4}

Soient A une $k$-algèbre et $\mathfrak{a}$ un idéal à gauche de A. Un élément $u$ de A tel que $au-a$ appartienne à $\mathfrak{a}$ pour tout $a\in A$s’appelle une unité à droite modulo $\mathfrak{a}$. On dit que l’idéal $\mathfrak{a}$ est régulier s’il existe une unité à droite modulo $\mathfrak{a}$.

On dit de même qu’un idéal à droite $\mathfrak{b}$ de A est régulier si A possède une unité à gauche modulo $\mathfrak{b}$, c’est-à-dire un élément $v$ tel que $va-a\in \mathfrak{b}$ pour tout $a\in A$. Lorsqu’un idéal est bilatère on veillera à préciser s’il est régulier en tant qu’idéal à gauche ou en tant qu’idéal à droite.

Lorsque l’algèbre A est unifère, l’élément unité de A est une unité à droite modulo $\mathfrak{a}$ pour tout idéal à gauche $\mathfrak{a}$ de A ; dans ce cas, tout idéal à gauche (ou à droite) de A est régulier. Par contre, si A est une $k$-algèbre dont tout élément est nilpotent, A est le seul idéal (à gauche ou à droite) de A qui soit régulier.

Soient $\mathfrak{a}$ un idéal à gauche régulier de A et $u$ une unité à droite modulo $\mathfrak{a}$. Si $\mathfrak{b}$ est un idéal à gauche de A contenant $\mathfrak{a},u$ est une unité à droite modulo $\mathfrak{b}$, donc $\mathfrak{b}$ est régulier. Ainsi les idéaux à gauche de A qui sont maximaux et réguliers sont les éléments maximaux de l’ensemble des idéaux à gauche réguliers de A distincts de A. De plus, pour qu’un idéal à gauche $\mathfrak{b}$ de A contenant $\mathfrak{a}$ soit distinct de A, il faut et il suffit que $u$ n’appartienne pas à $\mathfrak{b}$. L’ensemble des idéaux à gauche $\mathfrak{b}$ de A contenant $\mathfrak{a}$ et distincts de A, ordonné par inclusion, est donc inductif. Le théorème 2 de E, III, p. 20, appliqué à cet ensemble entraîne le résultat suivant :

#### Proposition 1 {#alg-viii-a1-prop-1 .statement tag=00P5}

Tout idéal à gauche (resp. à droite) de A, qui est régulier et distinct de A, est contenu dans un idéal à gauche (resp. à droite) maximal régulier.

#### Proposition 2 {#alg-viii-a1-prop-2 .statement tag=00P6}

Soient A une $k$-algèbre commutative. Pour qu’un idéal $\mathfrak{a}$ de A soit maximal régulier, il faut et il suffit que le pseudo-anneau $A/\mathfrak{a}$ (I, p. 93) soit un corps.

Pour qu’un élément $u$ de A soit une unité (à droite ou à gauche) modulo $\mathfrak{a}$, il faut et il suffit que l’image canonique de $u$ dans $A/\mathfrak{a}$ soit un élément unité de l’algèbre $A/\mathfrak{a}$. Pour que l’idéal $\mathfrak{a}$ soit régulier il faut et il suffit donc que l’algèbre $A/\mathfrak{a}$ soit unifère. Supposons ces conditions satisfaites.

L’application $\mathfrak{b}\rightarrow \mathfrak{b}/\mathfrak{a}$ est une bijection de l’ensemble des idéaux de l’algèbre A contenant $\mathfrak{a}$ sur l’ensemble des idéaux de l’algèbre $A/\mathfrak{a}$. Ceux-ci sont les idéaux de l’anneau $A/\mathfrak{a}$ puisque cette algèbre est unifère. Enfin, d’après le th. 1 de I, p. 109, l’anneau $A/\mathfrak{a}$ est un corps si et seulement s’il n’est pas nul et que ses seuls idéaux sont 0 et lui-même. La proposition résulte de là.

#### Exemple 1 {#alg-viii-a1-n1-exa-1 .statement tag=00P7}

Soit V un espace vectoriel de dimension infinie sur un corps commutatif K. Soit End$^f_K(V)$ la sous-K-algèbre de End$_K(V)$ formée des endomorphismes de rang fini. Soit W un sous-espace vectoriel de V et soit $\mathfrak{a}_W$ l’ensemble des éléments de End$^f_K(V)$ dont le noyau contient W ; c’est un idéal à gauche de End$^f_K(V)$. Un élément $u$ de End$^f_K(V)$ est une unité à droite modulo $\mathfrak{a}_W$ si et seulement si l’on a $u(x) =x$ pour tout $x\in W$. Pour qu’un tel élément $u$ existe, c’est-à-dire pour que $\mathfrak{a}_W$ soit régulier, il faut et il suffit que W soit de dimension finie. Pour que $\mathfrak{a}_W$ soit maximal et régulier, il faut et il suffit que W soit de dimension 1.

#### Exemple 2 {#alg-viii-a1-n1-exa-2 .statement tag=00P8}

Soit T un espace localement compact et soit $\mathscr{C}_0(T)$ la $\mathbf{C}$-algèbre commutative

des applications continues de T dans $\mathbf{C}$, tendant vers 0 à l’infini (TG, X, p. 40) ; elle est unifère si et seulement si T est compact. Soit F une partie fermée de T, et soit $\mathfrak{a}_F$ l’ensemble des éléments de $\mathscr{C}_0(T)$ dont la restriction à F est la fonction nulle ; c’est un idéal de $\mathscr{C}_0(T)$. Un élément $u$ de $\mathscr{C}_0(T)$ est une unité modulo $\mathfrak{a}_F$ si et seulement si l’on a $u(t) = 1$ pour tout $t\in F$. Pour qu’un tel élément $u$ existe, c’est-à-dire pour que $\mathfrak{a}_F$ soit régulier, il faut et il suffit que F soit compact. L’application $t\rightarrow \mathfrak{a}_{\{t\}}$ est une bijection de T sur l’ensemble des idéaux maximaux réguliers de $\mathscr{C}_0(T)$ (TS, I, §3, n$^o1$ et 2). Supposons que T ne soit pas compact et notons $\mathfrak{a}$ la partie de $\mathscr{C}_0(T)$ formée des fonctions à support compact ; alors $\mathfrak{a}$ est un idéal de $\mathscr{C}_0(T)$ qui n’est contenu dans aucun idéal régulier de $\mathscr{C}_0(T)$.

#### Exemple 3 {#alg-viii-a1-n1-exa-3 .statement tag=00P9}

Soit $L^1(\mathbf{R})$ l’algèbre de convolution du groupe localement compact $\mathbf{R}$. Rappelons (INT, VIII, §4, n$^o5)$ que $L^1(\mathbf{R})$ est l’espace des classes de fonctions sur $\mathbf{R}$ intégrables pour la mesure de Lebesgue ; le produit des classes de deux fonctions $f$ et $g$ est la classe de la fonction $f*g$ définie pour presque tout $s\in \mathbf{R}$par la formule

$$
(f*g)(s) =\int_{-\infty}^{+\infty}f(t)g(s-t)dt
$$

L’algèbre $L^1(\mathbf{R})$ n’est pas unifère. Pour tout $a$ dans $\mathbf{R}$, notons $\mathfrak{m}_a$ l’ensemble des éléments $f$ de $L^1(\mathbf{R})$ satisfaisant à

$$
\int_{-\infty}^{+\infty}f(t)e^{-iat}dt= 0
$$

D’après TS, II, §3, n$^o$ 1, th. 1, l’application $a\rightarrow \mathfrak{m}_a$ est une bijection de $\mathbf{R}$sur l’ensemble des idéaux maximaux réguliers de l’algèbre $L^1(\mathbf{R}).*$

### 2. Adjonction d’un élément unité

Soit A une $k$-algèbre. On a défini en III, p. 5, l’algèbre unifère $\widetilde{A}$ déduite de A par adjonction d’un élément unité $e$. On identifie A à un idéal bilatère de $\widetilde{A}$. Le $k$-module $\widetilde{A}$ est somme directe des sous-modules $ke$ et A.

#### Proposition 3 {#alg-viii-a1-prop-3 .statement tag=00PA}

a) Soit $\widetilde{\mathfrak{a}}$ un idéal à gauche de $\widetilde{A}$ tel que $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$. On pose $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$. Il existe un élément $u$ de A tel que $u-e$ appartienne à $\widetilde{\mathfrak{a}}$. Si $u$ est un tel élément, c’est une unité à droite de A modulo $\mathfrak{a}$, et l’on a $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$;en particulier l’idéal $\mathfrak{a}$ est régulier.

b) Inversement, soient $\mathfrak{a}$ un idéal à gauche régulier de A et $u$ une unité à droite de A modulo $\mathfrak{a}$. Posons $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$. Alors $\widetilde{\mathfrak{a}}$ est un idéal à gauche de $\widetilde{A}$, tel que $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$, et l’on a $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$.

c) Si $k$ est un corps, la condition $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$équivaut à dire que $\widetilde{\mathfrak{a}}$ n’est pas contenu dans A.

Sous les hypothèses de a), l’élément $e$ de $\widetilde{A}$ s’écrit sous la forme $(e-u) +u$, avec $u\in A$ et $u-e\in \widetilde{\mathfrak{a}}$. Soit $x=\lambda e+a$ un élément de $\widetilde{A}$, avec $\lambda \in k$ et $a\in A$; si $x$ appartient à $\widetilde{\mathfrak{a}}$, l’élément $y=a+\lambda u=x+\lambda (u-e)$ de A appartient à $\mathfrak{a}$, et l’on a $x=y-\lambda (u-e)$; cela prouve l’égalité $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$. De plus, pour tout $a$ dans A, l’élément $au-a=a(u-e)$ de A appartient à $\mathfrak{a}$, donc $u$ est une unité à droite modulo $\mathfrak{a}$. Cela établit l’assertion a).

Plaçons-nous sous les hypothèses de b) ; comme $\widetilde{A}$ est somme directe de A et de $k(u-e)$, on a $\widetilde{\mathfrak{a}}+ A =\widetilde{A}$ et $\widetilde{\mathfrak{a}}\cap A =\mathfrak{a}$. Tout élément de $\widetilde{\mathfrak{a}}$ est de la forme $x+\lambda (u-e)$ avec $x\in \mathfrak{a}$ et $\lambda \in k$; pour tout $a\in A$, on a

$$
a(x+\lambda (u-e)) =ax+\lambda (au-a)
$$

Comme $u$ est une unité à droite de A modulo $\mathfrak{a},ax+\lambda (au-a)$ appartient à $\mathfrak{a}$, de sorte que $\widetilde{\mathfrak{a}}$ est un idéal à gauche de A. Cela prouve b).

Enfin si $k$ est un corps, A est un hyperplan dans $\widetilde{A}$, et $\widetilde{A}$ est somme de $\widetilde{\mathfrak{a}}$ et de A si et seulement si $\widetilde{\mathfrak{a}}$ n’est pas contenu dans A.

#### Corollaire {#alg-viii-a1-n2-cor-1 .statement tag=00PB}

Les idéaux à gauche réguliers de A sont les idéaux de la forme $A\cap \widetilde{\mathfrak{a}}$, où $\widetilde{\mathfrak{a}}$ est un idéal à gauche de $\widetilde{A}$ tel que $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$.

#### Proposition 4 {#alg-viii-a1-prop-4 .statement tag=00PC}

a) Soit $\mathfrak{a}$ un idéal à gauche maximal régulier de A. Il existe un unique idéal à gauche $\widetilde{\mathfrak{a}}$ de $\widetilde{A}$ tel que $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$et $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$. Cet idéal est maximal et ne contient pas A.

b) L’application $\widetilde{\mathfrak{a}}\rightarrow \widetilde{\mathfrak{a}}\cap A$est une bijection de l’ensemble des idéaux à gauche maximaux de $\widetilde{A}$ ne contenant pas A sur l’ensemble des idéaux à gauche maximaux réguliers de A.

Soit $\mathfrak{a}$ un idéal à gauche maximal régulier de A. D’après la prop. 3, a), les idéaux à gauche $\mathfrak{b}$ de $\widetilde{A}$ tels que $\mathfrak{b}+ A =\widetilde{A}$ et $\mathfrak{b}\cap A =\mathfrak{a}$ sont les idéaux $\mathfrak{a}+k(u-e)$, où $u$ est une unité à droite modulo $\mathfrak{a}$. Pour démontrer l’unicité de $\widetilde{\mathfrak{a}}$, il suffit donc de prouver que deux unités à droite $u$ et $u'$ de A modulo $\mathfrak{a}$ sont congrues modulo $\mathfrak{a}$. Raisonnons par l’absurde en supposant que $u-u'$ n’appartient pas à $\mathfrak{a}$. La formule $x(u-u') = (xu-x)-(xu'-x)$ montre qu’on a $A(u-u')\subset \mathfrak{a}$; il en résulte que $\mathfrak{a}+k(u-u')$ est un idéal à gauche de A, contenant $\mathfrak{a}$ et distinct de $\mathfrak{a}$. Puisque $\mathfrak{a}$ est maximal, on a donc $\mathfrak{a}+k(u-u') = A$, d’où AA $\subset \mathfrak{a}$. Pour tout $x\in A$, on a $x\equiv xu$ (mod $\mathfrak{a})$, d’où $x\in \mathfrak{a}$ par ce qui précède, ce qui contredit l’hypothèse $\mathfrak{a}\not= A$.

Il existe donc un unique idéal à gauche $\widetilde{\mathfrak{a}}$ de $\widetilde{A}$ tel que $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ et $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$. Soit $\mathfrak{b}$ un idéal à gauche de $\widetilde{A}$ contenant $\widetilde{\mathfrak{a}}$ et distinct de $\widetilde{A}$. Alors $\mathfrak{b}\cap A$ est un idéal à gauche de A, contenant $\mathfrak{a}$, et distinct de A. Il est donc égal à $\mathfrak{a}$ puisque $\mathfrak{a}$ est maximal, ce qui entraîne $\mathfrak{b}=\widetilde{\mathfrak{a}}$ par le lemme 2 de VIII, p. 3. Cela prouve que $\widetilde{\mathfrak{a}}$ est un idéal maximal de $\widetilde{A}$; pour un tel idéal, la condition $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ signifie que $\widetilde{\mathfrak{a}}$ ne contient pas A.

Il reste à prouver que si $\widetilde{\mathfrak{a}}$ est un idéal à gauche maximal de $\widetilde{A}$, ne contenant pas A, alors l’idéal à gauche $\mathfrak{a}= A\cap \widetilde{\mathfrak{a}}$ de A est maximal. Soit $\mathfrak{b}$ un idéal à gauche de A, distinct de A et contenant $\mathfrak{a}$. Soit $u$ une unité à droite modulo $\mathfrak{a}$ telle que $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$ (prop. 3 de VIII, p. 427). C’est aussi une unité à droite modulo $\mathfrak{b}$; notons $\widetilde{\mathfrak{b}}$ l’idéal $\mathfrak{b}+k(u-e)$ de $\widetilde{A}$. D’après la prop. 3, b), on a $\mathfrak{b}= A\cap \widetilde{\mathfrak{b}}$. L’idéal $\widetilde{\mathfrak{a}}$, égal à $\mathfrak{a}+k(u-e)$, est contenu dans $\widetilde{\mathfrak{b}}$, donc égal à $\widetilde{\mathfrak{b}}$ puisque $\widetilde{\mathfrak{b}}$ est distinct de $\widetilde{A}$ et que $\widetilde{\mathfrak{a}}$ est maximal. Par suite on a $\mathfrak{a}=\mathfrak{b}$, et $\mathfrak{a}$ est maximal.

On laisse au lecteur le soin de traduire les prop. 3 et 4 pour les idéaux à droite.

### 3. Radical d’une algèbre

Soit A une $k$-algèbre. On appelle pseudomodule à gauche sur A un $k$-module M muni d’une structure de pseudomodule à gauche sur le pseudo-anneau A (II, p. 177), tel qu’on ait $a(\lambda x) =\lambda (ax) = (\lambda a)x$ pour $\lambda \in k,a\in A,x\in M$. On définit de même les pseudomodules à droite sur A.

Soit M un pseudomodule à gauche sur A ; on définit une structure dite canonique de $\widetilde{A}$-module à gauche sur M en posant

$(\lambda e+a)x=\lambda x+ax$ pour $\lambda \in k, a\in A, x\in M$.

Inversement, tout $\widetilde{A}$-module à gauche est muni canoniquement, par restriction de l’anneau des opérateurs à $k$ et A, d’une structure de pseudomodule à gauche sur A. Ainsi les espèces de structure de pseudomodule à gauche sur A et de module sur $\widetilde{A}$ sont équivalentes (E, IV, p. 9).

Soit M un pseudomodule à gauche sur A et soit N un sous-$k$-module de M. Pour que N soit un sous-$\widetilde{A}$-module de M, il faut et il suffit qu’il soit stable par l’action de A ; on dit alors que N est un sous-pseudomodule de M.

Comme dans le cas des anneaux, on définit le pseudomodule à gauche $A_s$ sur A, et le pseudomodule à droite $A_d$. Les idéaux à gauche (resp. à droite) de A sont les sous-pseudomodules de $A_s$ (resp. $A_d)$.

Soient$\mathfrak{a}$ un idéal à gauche régulier de A et $u$ une unité à droite modulo $\mathfrak{a}$. Posons $M = A_s/\mathfrak{a}$ et notons $z$ l’image de $u$ dans M. On a $M = Az$ et $\mathfrak{a}$ est l’annulateur de $z$.

Réciproquement, soit M un pseudomodule à gauche sur A et soit $z$ un élément de M tel que $M = Az$. Il existe alors un élément $u$ de A tel que $z=uz$. Pour tout $a\in A$, on a $(au-a)z= 0$, donc $au-a$ appartient à l’annulateur $\mathfrak{a}$ de $z$. Par suite, $\mathfrak{a}$ est un idéal à gauche régulier de A, l’élément $u$ est une unité à droite modulo $\mathfrak{a}$ et l’application $a\rightarrow az$ définit par passage au quotient un isomorphisme de $A_s/\mathfrak{a}$ sur M.

#### Définition 2 {#alg-viii-a1-def-2 .statement tag=00PD}

On dit qu’un pseudomodule M sur A est simple si l’on a AM $\not= 0$ et si 0 et M sont les seuls sous-pseudomodules de M.

Cela revient à dire que le $\widetilde{A}$-module M est simple et que son annulateur ne contient pas A. Lorsque A est un anneau et M un A-module, on a AM = M et la définition 2 coïncide donc avec la définition 1 de VIII, p. 41.

#### Proposition 5 {#alg-viii-a1-prop-5 .statement tag=00PE}

a) Soit $\mathfrak{m}$ un idéal à gauche maximal régulier de A. Alors le pseudomodule $A_s/\mathfrak{m}$ est simple et il existe un élément non nul de $A_s/\mathfrak{m}$ dont l’annulateur est $\mathfrak{m}$.

b) Soit M un pseudomodule simple et soit $x$ un élément non nul de M. On a $M = Ax$, l’annulateur $\mathfrak{m}$ de $x$ est un idéal à gauche maximal régulier de A et l’application $a\rightarrow ax$ définit par passage au quotient un isomorphisme de $A_s/\mathfrak{m}$ sur M.

c) Soit M un pseudomodule non réduit à 0. Pour que M soit simple, il faut et il suffit que l’on ait $M = Ax$ pour tout élément non nul $x$ de M.

Soit $\mathfrak{m}$ un idéal à gauche maximal régulier de A. On a vu qu’il existe un élément non nul $z$ de $A_s/\mathfrak{m}$ dont l’annulateur est égal à $\mathfrak{m}$ et tel que $Az= A_s/\mathfrak{m}$; en particulier, on a $A(A_s/\mathfrak{m})\not= 0$. De plus, tout sous-pseudomodule de $A_s/\mathfrak{m}$ est de la forme $\mathfrak{n}/\mathfrak{m}$, où $\mathfrak{n}$ est un idéal à gauche de A contenant $\mathfrak{m}$. Comme $\mathfrak{m}$ est maximal, les seules possibilités sont $\mathfrak{n}=\mathfrak{m}$ et $\mathfrak{n}= A$, de sorte que le pseudomodule $A_s/\mathfrak{a}$ est simple. Cela prouve a).

Sous les hypothèses de b), l’ensemble des éléments $y$ de M tels que $Ay= 0$ est un sous-pseudomodule de M, distinct de M, donc réduit à 0. Par suite, $Ax$ est un sous-pseudomodule non nul de M, ce qui entraîne $M = Ax$. L’assertion b) résulte alors des remarques faites avant la définition 2.

Soit M un pseudomodule non nul. Supposons qu’on ait $Ax= M$ pour tout élément non nul $x$ de M. En particulier, on a AM $\not= 0$. Soit N un sous-pseudomodule non nul de M et soit $x$ un élément non nul de N ; on a $Ax= M$, d’où N = M. Donc M est simple. Réciproquement, si M est simple, on a $M = Ax$ pour tout $x\not= 0$ d’après b).

#### Définition 3 {#alg-viii-a1-def-3 .statement tag=00RT}

On appelle radical de la $k$-algèbre A, et on note $\Re (A)$, l’intersection des idéaux à gauche maximaux réguliers de A.

Lorsque A est un anneau, tout idéal à gauche de A est régulier, donc la définition du radical coïncide avec la définition 2 de VIII, p. 150.

#### Exemple 1 {#alg-viii-a1-n3-exa-1 .statement tag=00PF}

Le radical de la $k$-algèbre End$^f_k(V)$ est réduit à 0 (VIII, p. 426, exemple 1$).*$Il en est de même pour les algèbres $\mathscr{C}_0(T)$ et $L^1(\mathbf{R}).*$

#### Exemple 2 {#alg-viii-a1-n3-exa-2 .statement tag=00PG}

Soit A un pseudo-anneau dans lequel tout élément est nilpotent. Le radical de A est égal à A, puisque A est le seul idéal à gauche régulier.

La proposition 5 entraîne aussitôt le résultat suivant :

#### Proposition 6 {#alg-viii-a1-prop-6 .statement tag=00PH}

Le radical de l’algèbre A est l’intersection des annulateurs des pseudomodules simples. C’est en particulier un idéal bilatère de A.

#### Proposition 7 {#alg-viii-a1-prop-7 .statement tag=00PI}

Le radical de A est la trace sur A du radical de $\widetilde{A}$;il est aussi égal au radical de l’algèbre opposée $A^o($c’est-à-dire à l’intersection des idéaux à droite maximaux réguliers de A). Si l’anneau $k$ est sans radical, le radical de A est égal à celui de $\widetilde{A}$.

L’égalité $\Re (\widetilde{A})\cap A =\Re (A)$ résulte de la prop. 4 de VIII, p. 428, b). Comme $\widetilde{A}$ et $\widetilde{A}^o$ ont le même radical (VIII, p. 152, cor. 1), on en déduit l’égalité $\Re (A) =\Re (A^o)$. Si $k$ est sans radical, l’intersection des idéaux à gauche maximaux de $\widetilde{A}$ contenant A est égale à A ; par suite, $\Re (\widetilde{A})$ est contenu dans A, donc égal à $\Re (A)$.

#### Remarque {#alg-viii-a1-n3-rem-1 .statement tag=00PJ}

Soient $x$ et $y$ des éléments de A ; on dit que $x$ est adverse à gauche de $y$, ou que $y$ est adverse à droite de $x$, si, dans $\widetilde{A},x-e$ est inverse à gauche de $y-e$, autrement dit si l’on a $x+y=xy$. D’après la prop. 7 et le théorème de Jacobson (VIII, p. 151, th. 1), le radical de A se compose des éléments $x$ de A tels que $ux-e$ soit inversible à gauche dans $\widetilde{A}$ pour tout $u$ dans $\widetilde{A}$. Comme on a $(a+\lambda e)x-e=ax+\lambda x-e$ (pour $a\in A,\lambda \in k)$, le radical de A est l’ensemble des éléments $x$ de A tels que $ax+\lambda x$ ait un adverse à gauche dans A quels que soient $a\in A$ et $\lambda \in k$.

### 4. Théorème de densité

Soit A une $k$-algèbre. Un pseudomodule à gauche M est dit semi-simple s’il est somme directe d’une famille de pseudomodules à gauche simples.

#### Lemme 1 {#alg-viii-a1-lem-1 .statement tag=00PK}

Soit M un A-pseudomodule à gauche semi-simple. Soit B le bicommutant du $\widetilde{A}$-module M. Alors tout sous-A-pseudomodule de M est un sous-B-module de M.

Le $\widetilde{A}$-module M est semi-simple. Soit N un sous-A-pseudomodule de M. Alors N est un sous-$\widetilde{A}$-module de M. Par le cor. 2 de VIII, p. 52 il existe un projecteur $p$ du $\widetilde{A}$-module M d’image N. Comme on a la relation $pb=bp$ pour tout $b\in B$, on obtient que N est un sous-B-module de M.

#### Lemme 2 {#alg-viii-a1-lem-2 .statement tag=00PL}

Soit M un A-pseudomodule à gauche semi-simple et soit $x$ un élément de M. Il existe un élément $a\in A$tel que $ax=x$.

Soit N le A-pseudomodule à gauche $\widetilde{A}x/Ax$. Il vérifie AN $=\{0\}$. D’après le corollaire 3 de VIII, p. 52 appliqué aux $\widetilde{A}$-modules M et $\widetilde{A}x$, le A-pseudomodule N est semi-simple. Par définition, tout sous-pseudomodule simple S de N vérifie AS $\not=\{0\}$. Par conséquent, le pseudomodule N est nul et on obtient que $x\in Ax$.

#### Théorème 1 (Théorème de densité de Jacobson) {#alg-viii-a1-thm-1 .statement tag=00SD}

Soit M un A-pseudomodule à gauche semi-simple. Soit $b$ un élément du bicommutant du $\widetilde{A}$-module M. Soit $\{x_1, . . . , x_n\}$ une partie finie de M. Alors il existe un élément $a\in$ A tel que $bx_i=ax_i$ pour tout $i\in [1, n]$.

Soit B le bicommutant du $\widetilde{A}$-module M. Le A-pseudomodule $M^n$ est semi-simple. Soit $\boldsymbol{x}= (x_1, . . . , x_n)\in M^n$. Il résulte du lemme 2 que $\boldsymbol{x}\in A\boldsymbol{x}$. Le bicommutant du $\widetilde{A}$-module $M^n$ coïncide avec les homothéties du B-module $M^n$ (VIII, p. 75, prop. 2). Par le lemme 1, le sous-A-pseudomodule $A\boldsymbol{x}$ de $M^n$ est donc un sous-B-module de $M^n$. On en déduit l’inclusion $B\boldsymbol{x}\subset A\boldsymbol{x}$. Donc il existe $a\in A$ tel que $b\boldsymbol{x}=a\boldsymbol{x}$. Le résultat en découle.

## EXERCICES {#alg-viii-a1-exercises}

See the [exercises for Appendix 1](exercises/a1/).
