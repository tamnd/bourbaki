---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 4
section_title: Perturbations dans les espaces de Banach
lang: fr
source: ts-iii-v-fr
book_pages: TS III.55-TS III.70, TS III.123-TS III.124
pdf_pages: 0069-0084, 0137-0138
extraction: native
subsections:
    - "no": 1
      title: Morphismes directs
      page: 55
      pdf_page: 69
    - "no": 2
      title: Perturbation des applications de Fredholm
      page: 58
      pdf_page: 72
    - "no": 3
      title: Perturbation des endomorphismes de Riesz
      page: 59
      pdf_page: 73
    - "no": 4
      title: Conorme d’une application linéaire continue
      page: 61
      pdf_page: 75
    - "no": 5
      title: Sous-espaces vectoriels de dimension finie d’un espace normé
      page: 64
      pdf_page: 78
    - "no": 6
      title: Perturbations des applications linéaires continues injectives ou surjectives
      page: 67
      pdf_page: 81
statements: 30
exercises: 9
content_sha256: 0639defbb25ee13675790dcd9d8ab04b2e73b080a6a0283ed9c065af1acacc79
---

## § 4. PERTURBATIONS DANS LES ESPACES DE BANACH

### 1. Morphismes directs

#### Définition 1 {#ts-iii-s4-def-1 .statement tag=02SH}

Soit E un espace vectoriel topologique. On dit qu’un sous-espace vectoriel de E est direct s’il admet un supplémentaire topologique.

Pour qu’un sous-espace vectoriel F de E soit direct, il faut et il suffit qu’il existe dans $\mathscr{L}(E)$ un projecteur d’image F. Si $p$ est un tel projecteur, E est somme directe topologique de F et du noyau de $p$. Le noyau de $1_E-p$ est F ; si E est séparé, F est donc fermé.

Soient F un sous-espace vectoriel direct de E et $E_1$ un sous-espace vectoriel de E contenant F ; alors F est un sous-espace vectoriel direct de $E_1$.

Tout sous-espace vectoriel fermé de codimension finie de E est direct (EVT, I, p. 15, prop. 3), et tout sous-espace vectoriel F de E contenu dans l’adhérence de $\{0\}$ est direct (en effet, il existe un projecteur d’image F et un tel projecteur est nécessairement continu).

#### Proposition 1 {#ts-iii-s4-prop-1 .statement tag=02SI}

Soit E un espace localement convexe. Tout sous-espace vectoriel de dimension finie de E est direct.

Soit F un sous-espace vectoriel de dimension finie de E. Notons S un supplémentaire topologique de l’adhérence de $\{0\}$ dans F, qui est un sous-espace direct de E. L’espace $F_2= F\cap S$ est séparé et de dimension finie ; il existe donc un entier $n\geqslant 0$ tel que $F_2$ soit isomorphe à $K^n$ (EVT, I, p. 14, th. 2). Il existe alors une application linéaire continue $p: S\rightarrow F_2$ prolongeant l’application identique de $F_2$ (EVT, II, p. 26, remarque). Le noyau de $p$ est un supplémentaire topologique de $F_2$ dans S, et aussi de F dans E.

#### Définition 2 {#ts-iii-s4-def-2 .statement tag=02SJ}

Soient E et F des espaces localement convexes et soit $u$ une application linéaire continue de E dans F. On dit que $u$ est un morphisme direct si $u$ est un morphisme strict dont le noyau est un sous-espace vectoriel direct de E et l’image un sous-espace vectoriel direct de F.

Soit $u\in \mathscr{L}(E; F)$. Pour que le noyau et l’image de $u$ soient des sous-espaces vectoriels directs de E et F respectivement, il faut et il suffit qu’il existe des décompositions $E = E_1\oplus E_2$ et $F = F_1\oplus F_2$ en sommes directes topologiques telles que $u$ soit représenté par une matrice $\begin{pmatrix} u_1 & 0 \\ 0 & 0 \end{pmatrix}$ où $u_1\in \mathscr{L}(E_1; F_1)$ est bijectif. Comme le noyau de $u$ est alors $E_2$, que l’application linéaire canonique de $E_1$ sur $E/E_2$ est un isomorphisme, et que l’image de $u$ est $F_1$, on voit que $u$ est un morphisme strict si et seulement si $u_1$ est un isomorphisme de $E_1$ sur $F_1$. Notons $v$ l’élément de $\mathscr{L}(F; E)$ représenté par la matrice $\begin{pmatrix} u_1^{-1} & 0 \\ 0 & 0 \end{pmatrix}$ . Alors l’application linéaire $u\circ v$ est le projecteur dans F de noyau $F_2$ et d’image $F_1$, l’application linéaire $v\circ u$ est le projecteur dans E de noyau $E_2$ et d’image $E_1$, et l’on a $u\circ v\circ u=u$.

Réciproquement, on a le résultat suivant :

#### Proposition 2 {#ts-iii-s4-prop-2 .statement tag=02SK}

Soient E et F des espaces localement convexes, soient $u\in \mathscr{L}(E; F)$ et $v\in \mathscr{L}(F; E)$. On suppose que $u=u\circ v\circ u$. Alors $u$ est un morphisme direct. De plus, $v\circ u$ est un projecteur continu dans E de noyau Ker($u$) et $u\circ v$ est un projecteur continu dans F d’image Im($u$).

Posons $p=v\circ u$ et $q=u\circ v$. On a

$$
p^2=v\circ (u\circ v\circ u) =v\circ u=p ,q^2= (u\circ v\circ u)\circ v=u\circ v=q
$$

donc $p$ et $q$ sont des projecteurs. Ils sont continus. Soient $E_1$ et $E_2$ l’image et le noyau de $p$, et soient $F_1$ et $F_2$ l’image et le noyau de $q$. Puisque $u\circ v\circ u=u$, on a

Ker($u$)$\subset$ Ker($v\circ u$)$\subset$ Ker($u\circ v\circ u$) $=$ Ker($u$),

donc Ker($u$) $=$ Ker($v\circ u$) $=$ Ker($p$) $= E_2$. Similairement, on déduit des inclusions

Im($u$)$\supset$ Im($u\circ v$)$\supset$ Im($u\circ v\circ u$) $=$ Im($u$)

que l’image de $u$ est $F_1$. Les espaces $E_2$ et $F_1$ sont des sous-espaces vectoriels directs de E et F respectivement.

L’espace vectoriel E est somme directe topologique de $E_1$ et $E_2$, et $u$ définit par restriction une application linéaire bijective $u_1$ de $E_1$ sur $F_1$. Pour tout $x\in E_1$, on a $v(u(x)) =p(x) =x$, et l’application $u^{-1}_1$ de $F_1$ sur $E_1$ coïncide avec $v$ sur $F_1$. Par conséquent, $u_1$ est un isomorphisme de $E_1$ sur $F_1$ et $u$ est un morphisme strict de E dans F.

Soient E et F des espaces localement convexes et $u\in \mathscr{L}(E; F)$. Pour que $u$ soit un morphisme direct injectif (resp. surjectif), il faut et il suffit qu’il existe $v$ dans $\mathscr{L}(F; E)$ tel que $v\circ u= 1_E$ (resp. $u\circ v= 1_F$) (cf. TG, III, p. 47 et 48).

#### Proposition 3 {#ts-iii-s4-prop-3 .statement tag=02SL}

Soient E et F des espaces de Banach. Les ensembles suivants sont des parties ouvertes de l’espace de Banach $\mathscr{L}(E; F):$

a) L’ensemble $\mathscr{I}(E; F)$ des isomorphismes de E sur F ;

b) L’ensemble $\mathscr{M} \mathscr{D}(E; F)$ des morphismes directs injectifs de E dans F, et plus précisément, pour tout sous-espace vectoriel fermé $F_1$ de F, l’ensemble $\mathscr{M}_{F_1}(E; F)$ des éléments de $\mathscr{M} \mathscr{D}(E; F)$ dont l’image est un supplémentaire topologique de $F_1$;

c) L’ensemble $\mathscr{E} \mathscr{D}(E; F)$ des morphismes directs surjectifs de E dans F, et plus précisément, pour tout sous-espace vectoriel fermé $E_1$ de E, l’ensemble $\mathscr{E}_{E_1}(E; F)$ des éléments de $\mathscr{E} \mathscr{D}(E; F)$ dont le noyau est un supplémentaire topologique de $E_1$.

De plus, l’application $u\mapsto u^{-1}$ de $\mathscr{I}(E; F)$ sur $\mathscr{I}(F; E)$ est analytique.

Par définition, $\mathscr{I}(E; E)$ est l’ensemble des éléments inversibles de l’algèbre normée complète $\mathscr{L}(E)$. D’après TG, IX, p. 40, prop. 14, c’est une partie ouverte de $\mathscr{L}(E)$. L’application $u\mapsto u^{-1}$ de $\mathscr{I}(E; E)$ dans $\mathscr{I}(E; E)$ est analytique (LIE, III, § 1, n$^o1$, exemple 2).

Si l’ensemble $\mathscr{I}(E; F)$ est vide, il est ouvert. Sinon, soit $u_0$ un isomorphisme de E sur F. L’application $v\mapsto u_0\circ v$ est alors un isomorphisme de $\mathscr{L}(E)$ sur $\mathscr{L}(E; F)$ qui transforme $\mathscr{I}(E; E)$ en $\mathscr{I}(E; F)$. L’ensemble $\mathscr{I}(E; F)$ est donc ouvert dans $\mathscr{L}(E; F)$. De plus, si $u=u_0\circ v$ est un élément de $\mathscr{I}(E; F)$, on a $u^{-1}=v^{-1}\circ u^{-1}_0$, et l’application $u\mapsto u^{-1}$ de $\mathscr{I}(E; F)$ sur $\mathscr{I}(F; E)$ est donc analytique.

Soit $F_1$ un sous-espace vectoriel fermé de F. Pour tout $u\in \mathscr{L}(E; F)$, soit $\overline{u}$ l’élément de $\mathscr{L}(E\times F_1; F)$ défini par $\overline{u}(x, y) =u(x) +y$. L’application $u\mapsto \overline{u}$ de $\mathscr{L}(E; F)$ dans $\mathscr{L}(E\times F_1; F)$ est continue, et $\mathscr{M}_{F_1}(E; F)$ est l’ensemble des éléments $u$ de $\mathscr{L}(E; F)$ tels que $\overline{u}$ appartienne à $\mathscr{I}(E\times F_1; F)$. Comme $\mathscr{I}(E\times F_1; F)$ est ouvert dans $\mathscr{L}(E\times F_1; F)$ d’après ce qui précède, l’ensemble $\mathscr{M}_{F_1}(E; F)$ est ouvert dans $\mathscr{L}(E; F)$. Il en est de même de $\mathscr{M} \mathscr{D}(E; F)$, qui est la réunion des $\mathscr{M}_{F_1}(E; F)$ lorsque $F_1$ parcourt l’ensemble des sous-espaces vectoriels fermés de F.

Soit $E_1$ un sous-espace vectoriel fermé de E, et soit $p$ l’application canonique de E sur l’espace de Banach quotient $E/E_1$. Pour qu’un élément $u$ de $\mathscr{L}(E; F)$ appartienne à $\mathscr{E}_{E_1}(E; F)$, il faut et il suffit que l’application $(u, p)$ de E dans $F\times E/E_1$ appartienne à $\mathscr{I}(E; F\times E/E_1)$. Comme précédemment, on en déduit que $\mathscr{E}_{E_1}(E; F)$ est ouvert dans $\mathscr{L}(E; F)$; il en est de même de $\mathscr{E} \mathscr{D}(E; F)$, qui est la réunion des $\mathscr{E}_{E_1}(E; F)$.

### 2. Perturbation des applications de Fredholm

#### Théorème 1 {#ts-iii-s4-thm-1 .statement tag=02SM}

Soient E et F des espaces de Banach. L’ensemble $\mathscr{F}(E; F)$ des applications de Fredholm de E dans F est ouvert dans l’espace de Banach $\mathscr{L}(E; F)$, et l’application $u\mapsto$ ind($u$) de $\mathscr{F}(E; F)$ dans $\mathbf{Z}$ est localement constante.

Le théorème résulte de l’énoncé plus précis suivant :

#### Proposition 4 {#ts-iii-s4-prop-4 .statement tag=02SN}

Soient E et F des espaces de Banach, $u_0: E\rightarrow F$ une application de Fredholm et $v_0$ un quasi-inverse de $u_0$. Il existe un voisinage ouvert U de $u_0$ dans $\mathscr{L}(E; F)$ et une application analytique $\varphi : U\rightarrow \mathscr{L}(F; E)$ telle que

(i) On a $\varphi (u_0) =v_0$;

(ii) Pour tout $u$ dans U, l’application $\varphi (u)$ est un quasi-inverse de $u$, et en particulier $u$ est une application de Fredholm ;

(iii) Pour tout $u$ dans U, on a ind($u$) $=$ ind($u_0$).

D’après la prop. 2 de III, p. 42, (ii), il existe des décompositions en somme directe topologique $E = E_1\oplus E_2$ et $F = F_1\oplus F_2$, et il existe $\alpha_0\in \mathscr{I}(E_1; F_1)$, tels que $E_2$ et $F_2$ soient de dimension finie et que $u_0$ soit représentée par la matrice $\begin{pmatrix} \alpha_0 & 0 \\ 0 & 0 \end{pmatrix}$ relativement à ces décompositions.

Soit U l’ensemble des éléments $u$ de $\mathscr{L}(E; F)$ tels que, dans la représentation matricielle $\begin{pmatrix} \alpha & \beta \\ \gamma & \delta \end{pmatrix}$ de $u$ par rapport à ces décompositions, on a $\alpha \in \mathscr{I}(E_1; F_1)$. Comme $\mathscr{I}(E_1; F_1)$ est ouvert dans $\mathscr{L}(E_1; F_1)$ (prop. 3 de III, p. 57), U est un voisinage ouvert de $u_0$ dans $\mathscr{L}(E; F)$. Pour $u=\begin{pmatrix} \alpha & \beta \\ \gamma & \delta \end{pmatrix}$ dans U, posons

$$
\varphi (u) =v_0+\begin{pmatrix} \alpha^{-1}-\alpha_0^{-1} & 0 \\ 0 & 0 \end{pmatrix} \tag{1}
$$

On a $\varphi (u_0) =v_0$ et l’application $\varphi$ est analytique (loc. cit.). Modulo les applications linéaires continues de rang fini, on a les congruences

$$
u\equiv \begin{pmatrix} \alpha & 0 \\ 0 & 0 \end{pmatrix},v_0\equiv \begin{pmatrix} \alpha_0^{-1} & 0 \\ 0 & 0 \end{pmatrix},\varphi (u)\equiv \begin{pmatrix} \alpha^{-1} & 0 \\ 0 & 0 \end{pmatrix}
$$

Par suite, $\varphi (u)$ est un quasi-inverse de $u$. Tout élément $u$ de U définit par restriction un isomorphisme de $E_1$ sur un supplémentaire topologique de $F_2$ dans F. D’après la prop. 3 de III, p. 44, on a donc

ind($u$) $=$ codim$_F(u(E_1))-$ codim$_E(E_1)$

= dim(F$_2$)$-$ dim(E$_2$) $=$ ind($u_0$),

ce qui conclut la démonstration.

### 3. Perturbation des endomorphismes de Riesz

#### Lemme 1 {#ts-iii-s4-lem-1 .statement tag=02SO}

Soit E un espace de Banach. Soient $p$ et $q$ des projecteurs continus de E tels que $\|q-p\|<1$. Alors $p$ induit un isomorphisme de Im($q$) sur Im($p$), et $1_E-p$ induit un isomorphisme de Ker($q$) sur Ker($p$).

Considérons les applications linéaires continues $u:x\mapsto p(x)$ de Im($q$) dans Im($p$) et $v:y\mapsto q(y)$ de Im($p$) dans Im($q$). Pour tout $x\in$ Im($q$), on a $x=q(x)$, d’où

$$
(q-p)^2(x) =q^2(x)-q(p(x))-p(q(x)) +p^2(x)
$$

$$
=x-q(p(x)) =x-v(u(x))
$$

Il en résulte que l’on a $\|1_E-v\circ u\|\leqslant \|q-p\|^2<1$. D’après le cor. 1 de I, p. 22$,v\circ u$ est un automorphisme de Im($q$). On démontre de même que $u\circ v$ est un automorphisme de Im($p$). Cela implique que $u$ est un isomorphisme de Im($q$) sur Im($p$), d’où la première assertion du lemme. La seconde s’en déduit en remplaçant $p$ et $q$ par $1_E-p$ et $1_E-q$ respectivement.

#### Théorème 2 {#ts-iii-s4-thm-2 .statement tag=02SP}

Soit E un espace de Banach. L’ensemble $\mathscr{R}(E)$ des endomorphismes de Riesz de E est ouvert dans $\mathscr{L}(E)$. L’application qui à un élément de $\mathscr{R}(E)$ associe la dimension de son nilespace est semi-continue supérieurement sur $\mathscr{L}(E)$.

Le théorème résulte de l’énoncé plus précis suivant :

#### Proposition 5 {#ts-iii-s4-prop-5 .statement tag=02SQ}

Soient E un espace de Banach et $u_0$ un endomorphisme de Riesz de E. Soit N (resp. I) le nilespace (resp. le conilespace) de $u_0$. Notons $d$ la dimension de N. Il existe un voisinage ouvert U de $u_0$ dans $\mathscr{L}(E)$ et une application analytique $\pi : U\rightarrow \mathscr{L}(E)$ telle que

(i) L’endomorphisme $\pi (u_0)$ est le projecteur d’image N et de noyau I ;

(ii) Pour tout $u\in U$, l’application linéaire $\pi (u)$ est un projecteur de rang $d$ qui appartient au bicommutant de $u$ et, en particulier, qui commute à $u$. De plus, $u$ induit un automorphisme de Ker($\pi (u)$);

(iii) Tout élément de U est un endomorphisme de Riesz dont le nilespace est de dimension $\leqslant d$.

Si K = $\mathbf{C}$, notons Sp($u_0$) le spectre de $u_0$ relativement à l’algèbre $\mathscr{L}(E)$. Lorsque K = $\mathbf{R}$, notons Sp($u_0$) le spectre complexe Sp$_{\mathscr{L}(E_{(\mathbf{C})})}((u_0)_{(\mathbf{C})})$ de $u_0($I, p. 85, n$^o13$). D’après la prop. 14 de III, p. 54, le point 0 est isolé dans $\{0\} \cup$ Sp($u_0$). Soit $r >0$ un nombre réel tel que tout élément de Sp($u_0$)$-\{0\}$ soit de module $> r$. Notons V l’ouvert dans $\mathbf{C}$ formé des nombres complexes de valeur absolue $\not =r$; soit $f$ la fonction holomorphe sur V définie par $f(z) = 0$ si $|z|> r$ et $f(z) = 1$ si $|z|< r$. Si $K =\mathbf{C}$ (resp. $K =\mathbf{R}$), notons $U'$ l’ensemble des éléments $u$ de $\mathscr{L}(E)$ dont le spectre (resp. dont le spectre complexe) est contenu dans V. L’ensemble $U'$ est un voisinage ouvert de $u_0$ dans $\mathscr{L}(E)$ et l’application $u\mapsto f(u)$ de $U'$ dans $\mathscr{L}(E)$ est holomorphe (I, p. 76, prop. 10 et I, p. 85, n$^o13$).

Soit $u\in U'$. L’endomorphisme $f(u)$ est le projecteur spectral $e_0(u)$; il commute à $u$, et $u$ induit par passage aux sous-espaces un automorphisme de Ker($e_0(u)$) $($cf. III, p. 53, n$^o6$).

Le projecteur $e_0(u_0)$ a pour image N et pour noyau I (III, p. 54, prop. 14) ; son rang est $d$. D’après le lemme 1, l’ensemble U des éléments $u\in U'$ tels que $e_0(u)$ soit de rang $d$ est un voisinage ouvert de $u_0$. L’ensemble U et l’application $\pi :u\mapsto e_0(u)$ de U dans $\mathscr{L}(E)$ satisfont aux conditions (i) et (ii) de la proposition.

Soit $u\in U$. Puisque $u$ induit un automorphisme de Ker($e_0(u)$), qui est un sous-espace vectoriel fermé de codimension finie de E, l’endomorphisme $u$ est un endomorphisme de Riesz de E (III, p. 48, prop. 8), le nilespace de $u$ est contenu dans l’image de $\pi (u) =e_0(u)$, et est de dimension $\leqslant d$.

### 4. Conorme d’une application linéaire continue

Soient E et F des espaces normés, $u: E\rightarrow F$ une application linéaire continue, N le noyau de $u$ et I son image. Notons $p$ la surjection canonique de E sur $E/N$ et $i$ l’injection canonique de I dans F. Soit $\widetilde{u}$ l’application linéaire bijective de $E/N$ sur I telle que $u=i\circ \widetilde{u}\circ p$. L’espace vectoriel $E/N$ est muni de la norme quotient, c’est-à-dire que

(2) $\|y\|=$ inf$_{x\in\overset{-1}{p}(y)}\|x\|$

pour tout $y\in E/N$. L’application $\widetilde{u}$ est continue et $\|u\|=\|\widetilde{u}\|$, d’où (3) $\|u\|=$ sup$_{y\in E/N}\frac{\|\widetilde{u}(y)\|}{\|y\|}$,

$y\not =0$

la borne supérieure étant prise dans $\overline{\mathbf{R}}_+$. On appelle conorme de $u$ le nombre

(4) $((u)) =$ inf$_{y\in E/N}\frac{\|\widetilde{u}(y)\|}{\|y\|}$,

$y\not =0$

la borne inférieure étant prise dans $\overline{\mathbf{R}}_+$. On a donc

$$
((u))\|y\|\leqslant \|\widetilde{u}(y)\|\leqslant \|u\| \|y\| \tag{5}
$$

pour tout élément $y$ de $E/N$. Posons $v=i\circ \widetilde{u}$. On a $u=v\circ p$ et

(6) $((u)) =$ inf$_{y\in E/N}\frac{\|v(y)\|}{\|y\|}=$ inf$_{y\in E/N}\|v(y)\|$.

$y\not =0\|y\|=1$

Lorsque $u$ est l’application nulle, l’espace $E/N$ est réduit à 0 et l’on a $((u)) = +\infty$ et $\|u\|= 0$. Lorsque $u\not = 0$, on déduit de (3) et (4) les inégalités

$$
0\leqslant ((u))\leqslant \|u\|<+\infty \tag{7}
$$

Lorsque $u$ est injectif, on a

(8) $((u)) =$ inf$_{xx\in\not=0E}\frac{\|u(x)\|}{\|x\|}$,

et, pour tout $x\in E$, on a

$$
((u))\|x\|\leqslant \|u(x)\|\leqslant \|u\| \|x\| \tag{9}
$$

Notons $j$ l’injection canonique de l’espace normé F dans son complété $\widehat{F}$. On a $((u)) = ((j\circ u))$.

#### Remarque {#ts-iii-s4-n4-rem-1 .statement tag=02SR}

Par définition, pour que l’on ait $((u))>0$, il faut et il suffit que l’application linéaire bijective $\widetilde{u}$ soit bicontinue, c’est-à-dire que $u$ soit un morphisme strict (TG, III, p. 16). On a alors

$$
((u)) =\|\widetilde{u}^{-1}\|^{-1} \tag{10}
$$

#### Lemme 2 {#ts-iii-s4-lem-2 .statement tag=02SS}

Soit $c$ un nombre réel. Si $c <((u))$, alors pour tout élément $z\in$ Im($u$), il existe un élément $x$ de E tel que $u(x) =z$ et $c\|x\|\leqslant \|z\|$. Réciproquement, si pour tout $z\in$ Im($u$) il existe $x\in E$ tel que $u(x) =z$ et $c\|x\|\leqslant \|z\|$, alors $c\leqslant ((u))$.

C’est une conséquence des formules (2) et (5) et de la définition de la conorme de $u$.

#### Proposition 6 {#ts-iii-s4-prop-6 .statement tag=02ST}

Soient E et F des espaces normés et $u\in \mathscr{L}(E; F)$. Notons B l’ensemble des éléments de E de norme $<1$. Posons

$P =u(E)-u(B),Q =u(E)$ - $(\overline{u(B)}\cap u(E))$.

La conorme de $u$ est égale à la distance de 0 à P dans F. Si l’espace normé E est complet ou si $u$ est un morphisme strict, la conorme de $u$ est égale à la distance de 0 à Q dans F.

Soit N le noyau de $u$; soit $p: E\rightarrow E/N$ la surjection canonique et soit $v: E/N\rightarrow F$ l’application déduite de $u$ par passage au quotient. L’ensemble $p(B)$ est l’ensemble des éléments de $E/N$ de norme $<1$. On a

$$
P =u(E)-u(B) =v(E/N)-v(p(B)) =v((E/N)-p(B))
$$

puisque l’application $v$ est injective. En d’autres termes, P se compose des éléments de F de la forme $v(y)$ avec $y\in E/N$ et $\|y\|\geqslant 1$. Notons $d_P$ la distance de 0 à P dans F. On a

$d_P=$ inf$_{y\|\in yE\|\geqslant/N1}\|v(y)\|=$ inf$_{y\|\in yE\|=1/N}\|v(y)\|= ((u))$ d’après (6).

Supposons que $u$ soit un morphisme strict. Soit $\varepsilon  >0$. L’ensemble $\varepsilon u(B)$ est un voisinage de 0 dans $u(E)$. L’adhérence de $u(B)$ dans $u(E)$ est égale à $\overline{u(B)}\cap u(E)$. Elle est contenue dans l’ensemble $u(B) +\varepsilon u(B)$ qui est égal à $(1 +\varepsilon )u(B)$ puisque $u(B)$ est convexe. On a par suite $(1 +\varepsilon )P\subset Q\subset P$ et la distance $d_Q$ de 0 à Q dans F satisfait aux inégalités $d_P\leqslant d_Q\leqslant (1 +\varepsilon )d_P$. Puisque ceci a lieu pour tout $\varepsilon  >0$, on a $d_Q=d_P= ((u))$.

Supposons que $u$ ne soit pas un morphisme strict, mais que l’espace normé E soit complet. On a alors $((u)) = 0$ (remarque ci-dessus). L’adhérence de $u(B)$ dans $u$(E), qui est égale à $\overline{u(B)}\cap u$(E), n’est pas un voisinage de 0 dans $u(E)$ (EVT, I, p. 17, th. 1). Il existe alors des points de Q arbitrairement proches de 0, d’où $d_Q= 0 = ((u))$.

#### Proposition 7 {#ts-iii-s4-prop-7 .statement tag=02SU}

Soient E un espace de Banach et F un espace normé. L’application $u\mapsto ((u))$ de $\mathscr{L}(E; F)$ dans $\overline{\mathbf{R}}$ est semi-continue supérieurement.

Soit $u\in \mathscr{L}(E; F)$. Il s’agit de prouver que pour tout nombre réel $c >((u))$, l’ensemble des éléments $v\in \mathscr{L}(E; F)$ tels que $((v))< c$ est un voisinage de $u$. Notons B l’ensemble des éléments de E de norme $<1$. D’après la prop. 6, il existe $y\in E$ tel que $u(y)\notin u(B)$ et $\|u(y)\|< c$. La distance $d$ de $u(y)$ à l’ensemble fermé $u(B)$ est strictement positive. L’ensemble V des éléments $v$ de $\mathscr{L}(E; F)$ vérifiant les relations $\|v(y)\|< c$ et $\|u-v\|(1 +\|y\|)< d$ est un voisinage de $u$ dans $\mathscr{L}(E; F)$. Soit $v\in V$. Pour tout $x\in B$, on a

$$
d\leqslant \|u(y)-u(x)\|\leqslant \|v(y)-v(x)\|+\|u-v\|(\|y\|+\|x\|)
$$

$$
<\|v(y)-v(x)\|+d
$$

Par conséquent $v(y)$ n’appartient pas à $v$(B), et l’on a $((v))\leqslant \|v(y)\|< c$ d’après la prop. 6.

#### Proposition 8 {#ts-iii-s4-prop-8 .statement tag=02SV}

Soient E un espace de Banach, F un espace normé. Pour tout $u\in \mathscr{L}(E; F)$, on a $((u)) = ((^tu))$.

Notons $j$ l’injection canonique de l’espace normé F dans son complété $\widehat{F}$. On a $((u)) = ((j\circ u))$. Comme l’application linéaire $^tj: (\widehat{F})'\rightarrow F'$ est bijective et isométrique, on a également $((^tu)) = ((^t(j\circ u)))$. Il suffit donc de démontrer la proposition lorsque l’espace normé F est complet, ce que nous supposons dans la suite de la démonstration.

Si $u$ est nul, on a $((u)) = ((^tu)) = +\infty$. Si $u$ n’est pas un morphisme strict, alors $^tu$ n’en est pas un (EVT, IV, p. 29, cor. 3), et l’on a $((u)) = ((^tu)) = 0$.

Supposons désormais que $u$ est un morphisme strict non nul. Notons N le noyau de $u$ et I son image, et considérons la décomposition canonique de $u:$

$$
E\overset{p}{\longrightarrow}E/N\longrightarrow^vI\longrightarrow^iF
$$

Le noyau de $^tu$ est l’orthogonal $I^{\circ}$ de I dans $F'$ (EVT, IV, p. 27, prop. 2), et $^ti$ définit par passage au quotient une isométrie $\iota$ de $F'/I^{\circ}$ sur $I'$ (EVT, IV, p. 9, prop. 10). Par ailleurs, $^tp$ définit une isométrie $\pi$ de $(E/N)'$ sur l’orthogonal $N^{\circ}$ de N dans $E'$ (EVT, IV, p. 8, prop. 9). La décomposition canonique de $^tu$ est donc

$$
F'\longrightarrow F'/I^{\circ}\longrightarrow^{v'}N^{\circ}\longrightarrow E'
$$

où $v'=\pi \circ^tv\circ \iota$. On a alors

$$
\|(v')^{-1}\|=\|(^tv)^{-1}\|=\|^t(v^{-1})\|=\|v^{-1}\|
$$

(EVT, IV, p. 7, prop. 8) d’où $((u)) = ((^tu))$ d’après la formule (10).

### 5. Sous-espaces vectoriels de dimension finie d’un espace normé

L’énoncé suivant sera démontré dans TA, à paraître, comme corollaire du théorème de Borsuk–Ulam.

#### Théorème 3 {#ts-iii-s4-thm-3 .statement tag=02SW}

Soient $n$ un entier positif, V un espace vectoriel normé réel de dimension $n+ 1$ et W un sous-espace vectoriel de V de dimension $n$. Soit S la sphère unité de V. Il n’existe pas d’application continue $f: S\rightarrow W$ telle que $\|f(x)-x)\|<1$ pour tout $x\in S$.

#### Théorème 4 (Krein, Krasnoselskii, Milman) {#ts-iii-s4-thm-4 .statement tag=02SX}

Soit E un espace normé, et soient F et G des sous-espaces vectoriels de E. Supposons que la dimension de G soit finie et strictement inférieure à celle de F. Il existe un élément de F de norme 1 dont la distance à G est égale à 1.

Il suffit de traiter le cas où le corps K est égal à $\mathbf{R}$. Soit $n$ la dimension de G. En remplaçant F par un sous-espace vectoriel de F de dimension $n+ 1$ contenant G, on se ramène au cas où dim(F) $=n+ 1$. Raisonnons par l’absurde en supposant que la conclusion du théorème n’est pas satisfaite. Soit S la sphère unité de F. Pour tout $x\in S$, la distance de $x$ à G est alors strictement inférieure à $\|x\|= 1$, et l’on peut choisir un élément $y(x)$ de G pour lequel on a $\|x-y(x)\|<1$. Notons $V_x$ l’ensemble des éléments $z$ de S tels que $\|z-y(x)\|<1$; c’est un voisinage ouvert de $x$ dans S. Il existe une partition continue localement finie de l’unité $(\varphi_x)_{x\in S}$ sur S subordonnée au recouvrement $(V_x)_{x\in S}$ de S (TG, IX, p. 46, prop. 3 et p. 51, prop. 6). Soit $f: S\rightarrow G$ l’application continue donnée par

$$
f(z) =\sum_{x\in S}\varphi_x(z)y(x)
$$

pour tout $z\in S$. Soit $z\in S$. On a $\varphi_x(z)\geqslant 0$ pour tout $x\in S$, et il existe $x\in S$ tel que $\varphi_x(z)>0$, puisque $\sum_{x\in S}\varphi_x(z) = 1$, donc

$$
\|z-f(z)\|=\|\sum_{x\in S}\varphi_x(z)(z-y(x))\|\leqslant \sum_{x\in S}\varphi_x(z)\|z-y(x)\|
$$

$$
<\sum_{x\in S}\varphi_x(z) = 1
$$

Cette propriété de $f$ contredit le théorème 3.

#### Proposition 9 {#ts-iii-s4-prop-9 .statement tag=02SY}

Soient E et F des espaces normés, $n\in \mathbf{N}$ et $u$ une application linéaire continue de E dans F dont le noyau est de dimension $n$. La conorme de $u$ est égale à la distance $d$ de $u$ à l’ensemble des applications $v\in \mathscr{L}(E; F)$ dont le noyau est de dimension au moins $n+ 1$.

Lorsque $u= 0$, on a $((u)) = +\infty$ et dim(E) $=n$, d’où $d= +\infty$. Supposons désormais $u$ non nulle, et donc $((u))<+\infty$. Soit $v$ un élément de $\mathscr{L}(E; F)$ tel que $\|u-v\|<((u))$ et démontrons que son noyau est de dimension $\leqslant n$. Soient $x$ un élément de norme 1 de Ker($v$) et $y$ son image dans $E/$ Ker($u$). On a (formule (5) de III, p. 61)

$$
((u))\|y\|\leqslant \|u(x)\|=\|(u-v)(x)\|\leqslant \|u-v\|<((u))
$$

d’où $\|y\|<1$. Or $\|y\|$ est la distance de $x$ à Ker($u$). Le théorème 4 implique alors que l’on a dim Ker($v$)$\leqslant$ dim Ker($u$) $=n$. Cela prouve l’inégalité $((u))\leqslant d$. L’inégalité réciproque $d\leqslant ((u))$ résulte du lemme plus précis qui suit.

#### Lemme 3 {#ts-iii-s4-lem-3 .statement tag=02SZ}

Soit $c$ un nombre réel tel que $c >((u))$. Il existe une application linéaire continue $h: E\rightarrow F$, de rang 1 et de norme $< c$ telle que le noyau de $u+h$ contienne celui de $u$ et soit de dimension $n+ 1$.

Notons $p$ l’application canonique de E sur $E/$ Ker($u$). Il existe $a\in E$ tel que $\|p(a)\|= 1$ et $\|u(a)\|< c$ (formule (6) de III, p. 61). D’après le théorème de Hahn–Banach (EVT, II, p. 24, cor. 2), il existe une forme linéaire continue $f$ sur l’espace normé $E/$ Ker($u$) telle que $f(p(a)) = 1$ et $\|f\|= 1$. L’application linéaire $h:x\mapsto  -(f\circ p)(x)u(a)$ de E dans F est continue, de rang 1, et l’on a $\|h\|\leqslant \|f\| \|p\| \|u(a)\|< c$. Le noyau de l’application $u+h$ contient celui de $u$ et $a$; comme $a\not \in$ Ker($u$), sa dimension est donc au moins $n+ 1$. D’autre part, l’application linéaire $u$ induit, par passage aux sous-espaces, une application linéaire de Ker($u+h$) dans Im($h$) de noyau Ker($u$)$\cap$ Ker($u+h$), de sorte que dim(Ker($u+h$))$\leqslant$ dim(Ker($u$)) $+ 1$. La conclusion en résulte.

#### Corollaire 1 {#ts-iii-s4-lem-3-cor-1 .statement tag=02T0}

Soient E et F des espaces normés, et soient $u,v$ des applications linéaires continues non nulles de E dans F dont les noyaux ont une même dimension finie. On a alors

$$
|((u))-((v))|\leqslant \|u-v\|
$$

Notons $n$ la dimension commune des noyaux de $u$ et $v$. Soit A l’ensemble des applications linéaires continues de E dans F dont le noyau est de dimension $\geqslant n+ 1$. Comme $u\not = 0$, on a dim(E) $> n$ et l’ensemble A contient 0. D’après la proposition 9, $((u))$ et $((v))$ sont respectivement les distances de $u$ et de $v$ à l’ensemble A dans $\mathscr{L}(E; F)$. Il suffit alors d’appliquer la formule $|d(u,A)-d(v,A)|\leqslant \|u-v\|($cf. TG, IX, p. 13).

#### Corollaire 2 {#ts-iii-s4-lem-3-cor-2 .statement tag=02T1}

Soient E et F des espaces de Banach et soient $u$ et $v$ des applications linéaires continues non nulles de E dans F dont les images ont une même codimension finie dans F. On a alors

$$
|((u))-((v))|\leqslant \|u-v\|
$$

Le morphisme $u$ est strict (III, p. 52, lemme 6). Le noyau de l’application linéaire continue $^tu$ est l’orthogonal (Im($u$))$^{\circ}$ de Im($u$) (EVT, IV, p. 27, prop. 2), donc dim(Ker($^tu$)) $=$ codim$_F$(Im($u$)), et de même dim(Ker($^tv$)) $=$ codim$_F$(Im($v$)). Les noyaux de $^tu$ et $^tv$ ont par suite une même dimension finie. Comme

$$
\|^tu-^tv\|=\|u-v\|,((^tu)) = ((u)),((^tv)) = ((v))
$$

(EVT, IV, p. 7, prop. 8 et prop. 8 de III, p. 63), l’assertion résulte du corollaire 1, appliqué à $^tu$ et $^tv$.

### 6. Perturbations des applications linéaires continues injectives ou surjectives

Dans ce numéro, on adopte les conventions suivantes : si E est un espace vectoriel de dimension finie, dim(E) désigne sa dimension ; si E est un espace vectoriel de dimension infinie, on pose dim(E) $= +\infty  \in \overline{\mathbf{R}}$. Si $u$ est une application linéaire dont le noyau ou le conoyau est de dimension finie, on pose ind($u$) $=$ dim Coker($u$)$-$ dim Ker($u$), le calcul étant effectué dans $\overline{\mathbf{R}}$.

Soient E et F des espaces normés. On note $\mathscr{M}(E; F)$ l’ensemble des morphismes stricts injectifs de E dans F, et $\mathscr{Q}\mathscr{M}(E; F)$ l’ensemble des morphismes stricts de E dans F dont le noyau est de dimension finie.

#### Proposition 10 {#ts-iii-s4-prop-10 .statement tag=02T2}

Soient E et F des espaces normés. L’ensemble $\mathscr{M}(E; F)$ est ouvert dans $\mathscr{L}(E; F)$. C’est l’intérieur de l’ensemble des applications de $\mathscr{L}(E; F)$ qui sont injectives.

Soit A l’ensemble des applications linéaires continues injectives de E dans F. Pour qu’une application $u\in A$ soit un morphisme strict, il faut et il suffit que sa conorme $((u))$ soit strictement positive (III, p. 62, remarque). Or $((u))$ est la distance de $u$ au complémentaire de A dans $\mathscr{L}(E; F)$(III, p. 65, prop. 9). La proposition en résulte.

#### Proposition 11 {#ts-iii-s4-prop-11 .statement tag=02T3}

Soient E et F des espaces de Banach. L’ensemble $\mathscr{Q}\mathscr{M}(E; F)$ est ouvert dans $\mathscr{L}(E; F)$. C’est l’intérieur de l’ensemble des applications de $\mathscr{L}(E; F)$ dont le noyau est de dimension finie.

Soit A l’ensemble des applications linéaires continues de E dans F dont le noyau est de dimension finie.

Soit $u$ un élément de $\mathscr{Q}\mathscr{M}(E; F)$. On a alors $((u))>0$(III, p. 62, remarque). Tout élément $v\in \mathscr{L}(E; F)$ dont la distance à $u$ est $<((u))$ appartient alors à A (III, p. 65, prop. 9), de sorte que $u$ est un point intérieur de A.

Réciproquement, soit $u$ un élément de A qui n’est pas un morphisme strict. On a $((u)) = 0 ($III, p. 62, remarque). Soit $v$ un élément de $\mathscr{L}(E; F)$ qui diffère de $u$ par une application linéaire de rang fini ; d’après le corollaire 1 de III, p. 40, le morphisme $v$ ne peut être strict d’image fermée ; comme un morphisme strict de E dans F a une image fermée dans F (EVT, IV, p. 28, th. 1), cela signifie que $v$ n’est pas un morphisme strict. On a donc $((v)) = 0$. Soit $\varepsilon$ un nombre réel $>0$. D’après ce qui précède, le lemme 3 de III, p. 66 permet de construire par récurrence une suite $(u_m)_{m\in\mathbf{N}}$ d’éléments de $\mathscr{L}(E; F)$ satisfaisant aux conditions suivantes :

(i) On a $u_0=u$;

(ii) Pour tout $m\geqslant 0,u_{m+1}-u_m$ est une application linéaire continue de rang 1 et de norme $\leqslant 2^{-m-1}\varepsilon$;

(iii) Pour tout $m\geqslant 0$, le noyau de $u_m$ est de dimension $n+m$ et est contenu dans celui de $u_{m+1}$.

La suite $(u_m)$ est une suite de Cauchy dans l’espace de Banach $\mathscr{L}(E; F)$. Soit $u'$ sa limite. Le noyau de $u'$ contient celui de $u_m$ pour tout $m\geqslant 0$; il est de dimension infinie. Comme

$$
\|u'-u\|\leqslant \sum_{m=0}^{\infty}\|u_{m+1}-u_m\|\leqslant \varepsilon \sum_{m=0}^{\infty}2^{-m-1}=\varepsilon
$$

la distance de $u$ au complémentaire de A est inférieure à $\varepsilon$. Ceci ayant lieu pour tout $\varepsilon  >0$, on conclut que $u$ n’est pas un point intérieur de A.

#### Proposition 12 {#ts-iii-s4-prop-12 .statement tag=02T4}

Soient E et F des espaces de Banach et $u$ un élément de $\mathscr{Q}\mathscr{M}(E; F)$. Tout $v\in \mathscr{L}(E; F)$ tel que $\|v-u\|<((u))$ appartient à $\mathscr{Q}\mathscr{M}(E; F)$ et satisfait les relations

dim Ker($v$)$\leqslant$ dim Ker($u$),

dim Coker($v$)$\leqslant$ dim Coker($u$),

ind($v$) $=$ ind($u$).

Comme $u$ est strict, on a $((u))>0$. Notons B la boule ouverte de centre $v$ et de rayon $((u))$ dans $\mathscr{L}(E; F)$. Pour tout $v\in$ B, on a dim Ker($v$)$\leqslant$ dim Ker($u$)(III, p. 65, prop. 9) et $v\in \mathscr{Q}\mathscr{M}(E; F)$ (prop. 11).

Pour $r\in \mathbf{Z}\cup  \{+\infty \}$, notons $B_r$ l’ensemble des éléments $v\in B$ tels que ind($v$) $=r$. Si $r\in \mathbf{Z}$, l’ensemble $B_r$ est l’ensemble des applications de Fredholm de E dans F d’indice $r$ qui appartiennent à B (III, p. 52, prop. 11) ; il est ouvert dans B d’après le th. 1 de III, p. 58.

Démontrons que les ensembles $B_r$ sont fermés dans B. Soit $v\in B$ un point adhérent à $B_r$. Comme les ensembles $B_s$, pour $s\in \mathbf{Z}$, sont ouverts dans B et deux à deux disjoints, on a $v\in B_r$ ou $v\in B_{+\infty}$.

Supposons $v\in B_{+\infty}$. Notons $n$ la dimension de Ker($u$). Choisissons un sous-espace vectoriel T de F de dimension $r+ 2n+ 1$ dont l’intersection avec Im($v$) soit réduite à 0 et un supplémentaire topologique S de Ker($v$) dans E (III, p. 55, prop. 1). Considérons l’application linéaire continue $f: (s, t)\mapsto v(s) +t$ de $S\times T$ dans F. Elle est injective. L’application linéaire $v$ est un morphisme strict puisque $v$ appartient à $B\subset \mathscr{Q}\mathscr{M}(E; F)$. L’image de $v$ est donc fermée (EVT, IV, p. 28, th. 1). D’après la prop. 1 de III, p. 39, la restriction de $v$ à S est un morphisme strict d’image fermée de S dans F, et $f$ est un morphisme strict d’image fermée de $S\times T$ dans F.

D’après la prop. 10, il existe un voisinage U de $v$ dans B tel que, pour tout $w\in U$, l’application linéaire $(s, t)\mapsto w(s) +t$ de $S\times T$ dans F est injective. Soit $w$ un élément de U. On a alors Ker($w$)$\cap S =\{0\}$ donc $w$ définit par restriction et passage au quotient une application linéaire injective de Ker($w$) dans $E/S$, ce qui implique que Ker($w$) est de dimension au plus $n$. On a également $w(S)\cap T =\{0\}$, donc

codim$_F$(Im($w$))$\geqslant$ dim(T) $-$ codim$_E(S) =r+n+ 1$,

cela entraîne ind($w$)$\geqslant r+ 1$ et contredit l’hypothèse que $v$ est adhérent à $B_r$.

Si $r$ est un élément de $\mathbf{Z}$ tel que $B_r$ soit non vide, on a $B_r= B$ puisque $B_r$ est ouvert et fermé dans B et B est connexe. Si $B_r$ est vide pour tout $r\in \mathbf{Z}$, on a ind($v$) $= +\infty$ pour tout $v\in B$. L’application $v\mapsto$ ind($v$) est donc constante sur B. Enfin, pour tout $v\in B$, on a

dim Coker($v$) $=$ ind($v$) $+$ dim Ker($v$)

$\leqslant$ ind($u$) $+$ dim Ker($u$) $=$ dim Coker($u$).

Cela conclut la démonstration.

#### Corollaire 1 {#ts-iii-s4-prop-12-cor-1 .statement tag=02T5}

Les fonctions définies par $u\mapsto$ dim Ker($u$) et par $u\mapsto$ dim Coker($u$) sur $\mathscr{Q}\mathscr{M}(E; F)$ sont semi-continues supérieurement. La fonction $u\mapsto$ ind($u$) est localement constante sur $\mathscr{Q}\mathscr{M}(E; F)$.

#### Corollaire 2 {#ts-iii-s4-prop-12-cor-2 .statement tag=02T6}

La fonction $u\mapsto$ dim Coker($u$) est localement constante sur l’ensemble $\mathscr{M}(E; F)$ des morphismes stricts injectifs de E dans F.

En effet, on a dim Coker($u$) $=$ ind($u$) pour $u\in \mathscr{M}(E; F)$.

#### Lemme 4 {#ts-iii-s4-lem-4 .statement tag=02T7}

Soient E et F des espaces de Banach. Pour qu’un élément $u$ de $\mathscr{L}(E; F)$ soit un morphisme strict de E dans F, il faut et il suffit que $^tu$ soit un morphisme strict de $F'$ dans $E'$. Dans ce cas, on a dim Coker($^tu$) $=$ dim Ker($u$) et dim Ker($^tu$) $=$ dim Coker($u$).

Pour que $u$ soit un morphisme strict, il faut et il suffit que $^tu$ en soit un (EVT, IV, p. 29, cor. 3) ; dans ce cas, l’image de $u$ est fermée (EVT, IV, p. 28, th. 1) et l’espace vectoriel Ker($^tu$) (resp. Coker($^tu$)) est canoniquement isomorphe au dual de l’espace normé Coker($u$) (resp. Ker($u$)) d’après EVT, IV, p. 27, prop. 2. Le lemme en résulte.

Soient E et F des espaces de Banach. On note $\mathscr{E}(E; F)$ l’ensemble des applications linéaires continues surjectives de E dans F et $\mathscr{Q}\mathscr{E}(E; F)$ l’ensemble des applications linéaires continues de E dans F dont l’image est de codimension finie. Tout élément de $\mathscr{Q}\mathscr{E}(E; F)$ est un morphisme strict d’image fermée (III, p. 52, lemme 6). Il résulte du lemme 4 que $\mathscr{E}(E; F)$ et $\mathscr{Q}\mathscr{E}(E; F)$ sont les images réciproques respectives de $\mathscr{M}(F'; E')$ et $\mathscr{Q}\mathscr{M}(F'; E')$ par l’application continue $u\mapsto^tu$ de $\mathscr{L}(E; F)$ dans $\mathscr{L}(F'; E')$.

#### Proposition 13 {#ts-iii-s4-prop-13 .statement tag=02T8}

Soient E et F des espaces de Banach. Les ensembles $\mathscr{E}(E; F)$ et $\mathscr{Q}\mathscr{E}(E; F)$ sont ouverts dans $\mathscr{L}(E; F)$. Plus précisément, si $u$ est un élément de $\mathscr{Q}\mathscr{E}(E; F)$ et $v$ un élément de $\mathscr{L}(E; F)$ tel que $\|v-u\|<((u))$, on a $v\in \mathscr{Q}\mathscr{E}(E; F)$ et

dim Ker($v$)$\leqslant$ dim Ker($u$), dim Coker($v$)$\leqslant$ dim Coker($u$),

ind($v$) $=$ ind($u$).

On a vu ci-dessus que $^tu\in \mathscr{Q}\mathscr{M}(F'; E')$. De plus, pour tout élément $v$ de $\mathscr{L}(E; F)$, on a $\|^tv-^tu\|=\|v-u\|$ et $((^tu)) = ((u))$ (EVT, IV, p. 7, prop. 8 et III, p. 63, prop. 8). D’après la prop. 12, il résulte de ces relations que si $\|v-u\|<((u))$, alors $^tv$ appartient à $\mathscr{Q}\mathscr{M}(F'; E')$ et qu’on a les inégalités

dim Ker($^tv$)$\leqslant$ dim Ker($^tu$), dim Coker($^tv$)$\leqslant$ dim Coker($^tu$)

ainsi que l’égalité ind($^tv$) $=$ ind($^tu$). La proposition résulte alors du lemme 4.

#### Corollaire 1 {#ts-iii-s4-prop-13-cor-1 .statement tag=02T9}

Les fonctions définies par $u\mapsto$ dim Ker($u$) et par $u\mapsto$ dim Coker($u$) sur $\mathscr{Q}\mathscr{E}(E; F)$ sont semi-continues supérieurement. La fonction $u\mapsto$ ind($u$) est localement constante sur $\mathscr{Q}\mathscr{E}(E; F)$.

#### Corollaire 2 {#ts-iii-s4-prop-13-cor-2 .statement tag=02TA}

La fonction définie par $u\mapsto$ dim Ker($u$) est localement constante sur $\mathscr{E}(E; F)$.

En effet, on a dim Ker($u$) $=-$ ind($u$) pour tout $u\in \mathscr{E}(E; F)$.

## EXERCICES {#ts-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
