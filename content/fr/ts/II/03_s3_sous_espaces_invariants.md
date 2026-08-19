---
book: ts
book_title: Théories spectrales
chapter: II
chapter_title: GROUPES LOCALEMENT COMPACTS COMMUTATIFS
section: 3
section_title: Sous-espaces invariants
lang: fr
source: ts-i-ii-fr
book_pages: TS II.250-TS II.261, TS II.308-TS II.318
pdf_pages: 0262-0273, 0320-0330
extraction: native
subsections:
    - "no": 1
      title: Le cas de l’espace hilbertien $L^2(G)$
      page: 251
      pdf_page: 263
    - "no": 2
      title: Idéaux fermés de $L^1(G)$
      page: 251
      pdf_page: 263
    - "no": 3
      title: Sous-espaces invariants faiblement fermés de $L^{\infty}(G)$
      page: 257
      pdf_page: 269
statements: 12
exercises: 19
content_sha256: 53b9dd4c4ef649cd2bc5283995540b3c864a2e7f5144d3f97d442f0fa2bfffc2
---

## § 3. SOUS-ESPACES INVARIANTS

L’objectif de ce numéro est l’étude de certains sous-espaces invariants par translation dans les espaces $L^1(G)$, $L^2(G)$ et $L^{\infty}(G)$.

### 1. Le cas de l’espace hilbertien $L^2(G)$

Pour toute partie mesurable M de $\widehat{G}$, on note $E_M$ l’ensemble des $f\in$ $L^2(G)$ telles que la transformation de Fourier $\mathscr{F}_G(f)$ est nulle presque partout sur $\widehat{G}$. Soit $\varphi_M$ la fonction caractéristique de M. L’espace $E_M$ est le noyau de l’application linéaire continue $f\mapsto \varphi_M\mathscr{F}_G(f)$ de $L^2(G)$ dans $L^2(\widehat{G})$, et c’est donc un sous-espace fermé de $L^2(G)$.

#### Proposition 1 {#ts-ii-s3-prop-1 .statement tag=02N3}

a) Soit M une partie mesurable de $\widehat{G}$. Pour tout $x\in G$, l’espace $E_M$ est stable par l’application $f\mapsto \varepsilon_x*f$;

b) Soient M et N des parties mesurables de $\widehat{G}$. On a $E_M= E_N$ si et seulement si M et N sont égales à un ensemble localement négligeable près;

c) Tout sous-espace de $L^2(G)$ stable par les applications $f\mapsto \varepsilon_x*f$ pour tout $x\in G$ est de la forme $E_M$ pour une partie mesurable M de $\widehat{G}$.

Ce résultat sera démontré ultérieurement (cf. V, à paraître).

### 2. Idéaux fermés de $L^1(G)$

La cotransformation de Fourier sur l’algèbre de Banach $L^1(G)$ s’identifie avec la transformation de Gelfand de $L^1(G)$ (II, p. 209). Avec cette identification, rappelons que si I est un idéal de $L^1(G)$, on note V(I) l’ensemble fermé dans $\widehat{G}$ des caractères $\chi \in \widehat{G}$ tels que, pour toute fonction $f\in I$, la cotransformation de Fourier de $f$ s’annule en $\chi ($cf. I, p. 30). Pour toute partie M de $\widehat{G}$, on note Υ(M) l’idéal fermé des $f\in L^1(G)$ telles que $\overline{\mathscr{F}}_G(f)$ s’annule sur M (I, p. 30).

D’après la prop. 2 de II, p. 219, l’algèbre de Banach $L^1(G)$ est régulière. D’après § 5 de I, p. 88 on en déduit donc les propriétés suivantes de la transformation et de la cotransformation de Fourier :

1) Si F est une partie fermée de $\widehat{G}$ et K une partie compacte de $\widehat{G}$ telles que $F\cap K =\emptyset$, il existe une fonction $f\in L^1(G)$ telle que $\mathscr{F}_G(f)$ soit égale à 0 sur F et à 1 sur K (I, p. 88, prop. 1 ; pour ce fait et les suivants, on passe de la cotransformation de Fourier à la transformation de Fourier par le biais de la formule (8) de II, p. 207).

2) Soit M une partie fermée de $\widehat{G}$. L’ensemble des idéaux I de $L^1(G)$ tels que V(I) = M a pour plus grand élément Υ(M) et pour plus petit élément l’ensemble des $f\in L^1(G)$ dont la cotransformation de Fourier est à support compact disjoint de M (I, p. 91, prop. 4).

3) Soient I un idéal de $L^1(G)$, et $g:\widehat{G}\rightarrow \mathbf{C}$ une fonction continue. On suppose que pour tout $\chi \in \widehat{G}$, il existe une fonction $f_{\chi}\in I$ telle que $g$ soit égale à $\mathscr{F}_G(f_{\chi})$ au voisinage de $\chi$. On suppose en outre qu’il existe une fonction $f_{\infty}\in I$ telle que $g$ soit égale à $\mathscr{F}_G(f_{\infty})$ dans le complémentaire d’une partie compacte de $\widehat{G}$, cette dernière condition étant toujours satisfaite si G est discret. Alors il existe une fonction $f\in I$ telle que $g=\mathscr{F}_G(f)$ (I, p. 91, cor. 2).

#### Lemme 1 {#ts-ii-s3-lem-1 .statement tag=02N4}

L’espace des fonctions de $L^1(G)$ dont la transformée de Fourier est à support compact est dense dans $L^1(G)$.

Comme $\mathscr{K}(\widehat{G})$ est dense dans $L^2(\widehat{G})$ et que la transformation de Fourier de $L^2(G)$ est une isométrie sur $L^2(\widehat{G})$ (th. 1 de II, p. 215), le sous-espace V de $L^2(G)$ formé des $f\in L^2(G)$ telles que $\mathscr{F}_G(f)\in \mathscr{K}(\widehat{G})$ est dense dans $L^2(G)$.

Soit $g\in L^1(G)$. Il existe $g_1, g_2\in L^2(G)$ telles que $g=g_1g_2$ (on peut par exemple prendre $g_1=|g|^{1/2}$, et $g_2(x) = 0$ si $g(x) = 0,g_2(x) =$ $g(x)/g_1(x)$ sinon). On déduit donc de ce qui précède que $g$ est limite d’une suite de fonctions de la forme $h_1h_2$, où $h_1$ et $h_2$ appartiennent à V. Or $\mathscr{F}_G(h_1h_2) =\mathscr{F}_G(h_1)*\mathscr{F}_G(h_2)$ (II, p. 223, prop. 14), et $\mathscr{F}_G(h_1)*$ $\mathscr{F}_G(h_2)$ appartient à $\mathscr{K}(G)$. Le lemme en résulte.

#### Proposition 2 {#ts-ii-s3-prop-2 .statement tag=02N5}

Soit I un idéal fermé de $L^1(G)$, et soit $f\in L^1(G)$. Si $\overline{\mathscr{F}}_G(f)$ s’annule sur un voisinage de V(I), alors $f$ appartient à I.

Soit $\varepsilon  >0$. Il existe une fonction $g\in L^1(G)$ telle que $\|f-f*g\|_1<$ $\varepsilon$ (prop. 8 de II, p. 211 (iv)). Soit $h\in L^1(G)$ tel que le support de $\overline{\mathscr{F}}_G(h)$ est compact et $\|f\|_1\|g-h\|_1< \varepsilon$ (lemme 1). On a

$$
\|f-f*h\|_1\leqslant \|f-f*g\|_1+\|f*(g-h)\|_1<2\varepsilon
$$

D’après l’hypothèse sur $f$, la fonction $\overline{\mathscr{F}}_G(f*h) =\overline{\mathscr{F}}_G(f)\overline{\mathscr{F}}_G(h)$ est à support compact disjoint de V(I), ce qui implique que $f*h\in I$ (remarque 2 ci-dessus). Comme $\varepsilon$ est arbitrairement petit, on a $f\in$ I = I.

#### Théorème 1 {#ts-ii-s3-thm-1 .statement tag=02N6}

Soit I un idéal fermé de $L^1(G)$ distinct de $L^1(G)$. Il existe un caractère $\widehat{x}\in \widehat{G}$ tel que $\mathscr{F}_G(f)(\widehat{x}) = 0$ pour toute $f\in I$.

Comme l’algèbre $L^1(G)$ est régulière (prop. 2 de II, p. 219) et sans radical (cor. de la prop. 22 de I, p. 126), et que l’ensemble des fonctions dont la cotransformée de Fourier est à support compact est dense dans $L^1(G)$ (lemme 1), le cor. 1 de I, p. 92 montre que l’idéal I est contenu dans un idéal maximal régulier de $L^1(G)$, c’est-à-dire dans le noyau d’un caractère $\widehat{y}$ de $L^1(G)$ (th. 2 de I, p. 30) ; on peut alors prendre $\widehat{x}=\widehat{y}^{-1}($cf. formule (8) de II, p. 207).

Corollaire 1 (Théorème taubérien de Wiener)

Soit $f\in L^1(G)$. Si la transformée de Fourier de $f$ ne s’annule pas, les fonctions $f*\varepsilon_x:g\mapsto f(gx^{-1})$, où $x$ parcourt G, forment un ensemble total dans $L^1(G)$ (EVT, I, p. 12, déf. 1).

Soit V le sous-espace vectoriel fermé de $L^1(G)$ engendré par les $f*\varepsilon_x$. D’après INT, VIII, §4, cor. de la prop. 20, l’espace V est un idéal fermé de $L^1(G)$. D’après le th. 1 on a $V = L^1(G)$.

#### Définition 1 {#ts-ii-s3-def-1 .statement tag=02N7}

Soit $g$ une fonction complexe sur G et soit Φ un filtre sur G. On dit que $g$ est lentement oscillante suivant Φ si, pour tout $\varepsilon  >0$, il existe un ensemble $M\in \Phi$ et un voisinage V de $e$ dans G tels que

$x\in M$ et $y\in V=\Rightarrow |g(xy)-g(x)|\leqslant \varepsilon$.

#### Corollaire 2 {#ts-ii-s3-def-1-cor-2 .statement tag=02N8}

Soit Φ un filtre sur G invariant par translation. Soit $f\in L^1(G)$ telle que la transformée de Fourier de $f$ ne s’annule pas et telle que $\int_Gf(x)dx= 1$. Soit $g\in L^{\infty}(G)$. On suppose que $f*g$ a une limite finie $\alpha$ suivant Φ.

a) Pour toute fonction $h\in L^1(G)$ telle que $\int_Gh(x)dx= 1$, la limite de $h*g$ suivant Φ est égale à $\alpha$;

b) Supposons de plus que $g$ soit lentement oscillante suivant Φ. Alors $g$ tend vers $\alpha$ suivant Φ.

En remplaçant $g$ par $g-\alpha$, on se ramène au cas où $\alpha = 0$. Soit I l’ensemble des fonctions $h\in L^1(G)$ telles que $h*g$ tende vers 0 suivant Φ. L’ensemble I est un sous-espace vectoriel de $L^1(G)$ invariant par translation. C’est un espace fermé. En effet, soit $h\in \overline{I}$. Pour toute fonction $h_0\in L^1(G)$ et tout $x\in G$, on a

$$
|(h*g)(x)|\leqslant |((h-h_0)*g)(x)|+|(h_0*g)(x)|
$$

$$
\leqslant \|h-h_0\|_1\|g\|_{\infty}+|(h_0*g)(x)|
$$

Pour tout $\varepsilon  >0$, il existe $h_0\in I$ telle que $\|h-h_0\|_1\|g\|_{\infty}< \varepsilon$. Soit $M\in$ Φ tel que $|(h_0*g)(x)|< \varepsilon$ pour tout $x\in M$. On a alors $|(h*g)(x)|<2\varepsilon$ pour tout $x\in M$, donc $h*g$ converge vers 0 suivant Φ. Cela montre que $h\in I$.

L’espace I est donc un idéal fermé de $L^1(G)$. On a $f\in I$ par hypothèse, donc $I = L^1(G)$ d’après le th. 1 puisque la transformée de Fourier de $f$ ne s’annule pas. Ceci implique a).

Plaçons-nous dans les hypothèses de b). Soit $\varepsilon  >0$. Puisque $g$ est lentement oscillante suivant Φ, il existe $M\in \Phi$ et un voisinage compact V de $e$ tels que

$x\in M$ et $y\in V =\Rightarrow  |g(y^{-1}x)-g(x)|\leqslant \varepsilon$.

Soient $\varphi$ la fonction caractéristique de V et $\mu=\int\varphi (x)dx$. Pour tout $x\in G$, on a

$$
\frac{1}{\mu}(\varphi *g)(x) =\frac{1}{\mu}\int_Vg(y^{-1}x)dy=g(x) +\frac{1}{\mu}\int_V(g(y^{-1}x)-g(x))dy
$$

Donc pour tout $x\in M$, on a

$$
|\frac{1}{\mu}(\varphi *g)(x)-g(x)|\leqslant \varepsilon
$$

Comme, d’après a), la limite de $\varphi *g$ selon Φ est nulle, on a lim sup$_{\Phi}|g|\leqslant \varepsilon$. Puisque $\varepsilon$ est arbitraire, on conclut que la limite de $g$ selon Φ est nulle, ce qui prouve b).

#### Lemme 2 {#ts-ii-s3-lem-2 .statement tag=02N9}

Soit K une partie compacte de G. Pour tout $\eta  >0$, il existe une fonction $j\in L^1(G)$ telle que :

$$
\surd
$$

a) $\|j\|_1\leqslant$ 2 ;

b) la fonction $\mathscr{F}_G(j)$ est égale à 1 au voisinage de l’élément neutre de $\widehat{G}$;

c) pour tout $x\in K$, on a $\|j-j*\varepsilon_x\|_1\leqslant \eta$.

L’ensemble $U_1$ des éléments $\widehat{x}\in \widehat{G}$ tels que

$$
|\langle \widehat{x}, x\rangle  -1|\leqslant \frac{\eta}{4}
$$

pour tout $x\in$ K est un voisinage de $e$ dans $\widehat{G}$. Soit U $\subset U_1$ un voisinage ouvert, symétrique, et intégrable pour la mesure de Haar $m=d\widehat{x}$ de $\widehat{G}$ duale de la mesure $dx$. Soit $V\subset U$ un voisinage compact symétrique de $e$ tel que $m(V)\geqslant \frac{1}{2}m(U)$. Notons $\varphi_U$ (resp. $\varphi_V$) la fonction caractéristique de U (resp. de V). Puisque $\varphi_U$ appartient à $L^2(G)$, il existe $u\in L^2(G)$ telle que $\varphi_U=\mathscr{F}_G(u)$ (th. 1 de II, p. 215). De même, il existe une fonction $v\in L^2(G)$ telle que $\varphi_V=\mathscr{F}_G(v)$. Nous allons montrer que la fonction $j=\frac{1}{m(V)}uv$ vérifie les propriétés demandées. On a $j\in L^1(G)$.

a) D’après le théorème de Plancherel et la condition $m(V)\geqslant \frac{1}{2}m(U)$, on a

$$
\|j\|_1\leqslant \frac{\|u\|_2\|v\|_2}{m(V)}=\frac{\|\mathscr{F}_G(u)\|_2\|\mathscr{F}_G(v)\|_2}{m(V)}=\surd\overline{mm(U)(V)m(V)}\leqslant \surd \overline{2}
$$

b) Il existe un voisinage W de $e$ dans $\widehat{G}$ tel que WV $\subset U$ (TG, II, p. 31, prop. 4). Pour tout $\widehat{x}\in W$, on a $\widehat{x}V\subset U$, et la prop. 14 de II, p. 223 implique

$$
\mathscr{F}_G(j)(\widehat{x}) =\frac{1}{m(V)}(\mathscr{F}_G(u)*\mathscr{F}_G(v))(\widehat{x})
$$

$$
=\frac{1}{m(V)}\int_{\widehat{G}}\varphi_U(\widehat{y})\varphi_V(\widehat{y}^{-1}\widehat{x})dm(\widehat{y})
$$

$$
=\frac{m(U \cap\widehat{x}V^{-1})}{m(V)}=\frac{m(\widehat{x}V)}{m(V)}= 1
$$

puisque V est symétrique.

c) Si $x\in K$, on a

$$
\|u-u*\varepsilon_x\|^2_2=\int_{\widehat{G}}|\mathscr{F}_G(u)(\widehat{x})(1- \langle x,\widehat{x}\rangle )||^2dm(\widehat{x})\leqslant m(U)(\frac{\eta}{4})^2
$$

puisque $U\subset U_1$, et de même $\|v-v*\varepsilon_x\|^2_2\leqslant m(V)(\frac{\eta}{4})^2$. Donc

$$
\|j-j*\varepsilon_x\|_1=\frac{1}{m(V)}\|u(v-v*\varepsilon_x) + (v*\varepsilon_x)(u-u*\varepsilon_x)\|_1
$$

$$
\leqslant \frac{\eta}{4m(V)}(\|u\|_2\surd m(V) +\|v\|_2\surd\overline{m(U)})
$$

$$
=\eta \surd\overline{m2m(U)(V)m(V)}< \eta
$$

#### Proposition 3 {#ts-ii-s3-prop-3 .statement tag=02NA}

L’algèbre $L^1(G)$ vérifie la condition de Ditkin (I, p. 92, déf. 2).

Soit $\chi$ un caractère de $L^1(G)$. Distinguons deux cas suivant que $\chi$ est nul ou non. Si $\chi$ est nul, il faut vérifier que pour toute fonction $f\in L^1(G)$, il existe une suite $(f_n)_{n\geqslant 1}$ dans $L^1(G)$ telle que $\mathscr{F}(f_n)$ s’annule hors d’une partie compacte de $\widehat{G}$ et telle que $f_n*f$ tende vers $f$ dans $L^1(G)$. L’existence d’une telle suite résulte du lemme 1 ci-dessus et de la prop. 8 de II, p. 211.

Supposons maintenant que $\chi$ est non nul, donc $\chi \in \mathsf{X}(L^1(G)) =\widehat{G}$ (prop. 1 de II, p. 202). Soit $f\in L^1(G)$ telle que $\mathscr{G}_{L^1(G)}(f)(\chi ) =$ $\overline{\mathscr{F}}(f)(\chi ) = 0$. Il s’agit de prouver l’existence d’une suite $(f_n)_{n\geqslant 1}$ dans $L^1(G)$ telle que $f*f_n$ converge vers $f$ dans $L^1(G)$ et telle que $\overline{\mathscr{F}}(f_n)$ s’annule au voisinage de $\chi$. On peut supposer que $\|f\|_1= 1$. Par translation dans $\widehat{G}$, on se ramène au cas où $\chi =e$.

Soit $K_n$ une partie compacte de G telle que

$$
\int_{G-K_n}|f(x)|dx\leqslant \frac{1}{n}
$$

Soit $u_n\in L^1(G)$ une fonction $\geqslant 0$ telle que $\|u_n\|_1= 1$ et

$$
\|f-f*u_n\|_1\leqslant \frac{1}{n}
$$

(cf. prop. 8 de II, p. 211, (iii)). D’après le lemme$\surd$ 2, il existe une fonction $j_n$ dans $L^1(G)$ telle que $\|j_n\|_1\leqslant \overline{2}$, dont la cotransformée de Fourier vaut 1 au voisinage de $e$, et de plus telle que $\|j_n-j_n*\varepsilon_x\|_1\leqslant n^{-1}$ pour tout $x\in K_n$. On pose

$$
f_n=u_n-j_n*u_n
$$

Nous allons montrer que la suite $(f_n)_{n\geqslant 1}$ possède les propriétés requises. Tout d’abord, on a

$$
\mathscr{F}(f_n) =\mathscr{F}(u_n)-\mathscr{F}(j_n)\mathscr{F}(u_n) = (1-\mathscr{F}(j_n))\mathscr{F}(u_n)
$$

donc la transformée de Fourier de $f_n$ s’annule au voisinage de $\chi =e$. D’autre part,

1

$$
\|f*f_n-f\|_1\leqslant \|f*u_n-f\|_1+\|f*j_n\|_1\|u_n\|_1\leqslant +\|f*j_n\|_1
$$

$$
n
$$

Or, pour presque tout $y\in G$, on a

$$
(f*j_n)(y) =\int_Gf(x)j_n(x^{-1}y)dx=\int_Gf(x)(j_n(x^{-1}y)-j_n(y))dx
$$

puisque, par hypothèse, on a $\mathscr{F}(f)(e) =\int_Gf(x)dx= 0$. D’où

$$
\|f*j_n\|_1\leqslant \int_G|f(x)| \|j_n*\varepsilon_x-j_n\|_1dx
$$

$$
=\int|f(x)| \|j_n*\varepsilon_x-j_n\|_1dx
$$

$$
+\int^{K_n}|f(x)| \|j_n*\varepsilon_x-j_n\|_1dx
$$

$G-K_n$

$1\int\int$ 5 $\leqslant |f(x)|dx+ 4|f(x)|dx\leqslant$.

$n_{K_n}G-K_{_n}n$

Finalement, $\|f*f_n-f\|_1\leqslant 6n^{-1}$ et donc $f*f_n$ converge dans $f$ dans $L^1(G)$, comme désiré.

Appliquant la prop. 5, on obtient alors le résultat suivant :

#### Théorème 2 {#ts-ii-s3-thm-2 .statement tag=02NB}

Soit I un idéal fermé de $L^1(G)$ tel que la frontière de V(I) ne contienne aucun ensemble parfait non vide. Alors I est l’ensemble des fonctions $f\in L^1(G)$ telles que $\mathscr{F}(f)$ s’annule sur V(I).

Pour un idéal fermé quelconque de $L^1(G)$, la conclusion du th. 2 est en général inexacte (cf. exerc. 12 de II, p. 314). Plus précisément, on peut montrer que, si G est non compact, il existe un idéal fermé de $L^1(G)$ qui n’est pas auto-adjoint (voir par exemple W. Rudin, Fourier analysis on groups, Interscience tracts in pure and applied mathematics, theorem 7.7.1.)

#### Corollaire {#ts-ii-s3-n2-cor-1 .statement tag=02NC}

Si un idéal fermé I de $L^1(G)$ est contenu dans un seul idéal régulier maximal, alors I est lui-même régulier maximal.

### 3. Sous-espaces invariants faiblement fermés de $L^{\infty}(G)$

Dans ce numéro, on identifie $L^{\infty}(G)$ au dual de $L^1(G)$, et on le munit de la topologie faible $\sigma (L^{\infty}(G),L^1(G))$. On note $(f, g)\mapsto  \langle f, g\rangle$ l’application bilinéaire définissant cette dualité pour $f\in L^1(G)$ et $g\in L^{\infty}(G)$.

L’application $W\mapsto W^{\circ}$ est une bijection de l’ensemble des sous-espaces vectoriels faiblement fermés de $L^{\infty}(G)$ sur l’ensemble des sous-espaces vectoriels fermés de $L^1(G)$ (EVT, II, p. 55, prop. 10).

D’autre part, si $f\in L^1(G)$ et $x\in G$, l’endomorphisme $g\mapsto f*g$ (resp. $g\mapsto \varepsilon_x*g$) de l’espace de Banach $L^1(G)$ a pour transposé l’endomorphisme $h\mapsto \check{f}*h$ (resp. $h\mapsto \varepsilon_{x^{-1}}*h$) de l’espace de Banach $L^{\infty}(G)$ (INT, VIII, §4, n$^o3$, exemple 6). Pour qu’un sous-espace vectoriel fermé de $L^1(G)$ soit un idéal de $L^1(G)$, il faut et il suffit qu’il soit invariant par les translations de G. Donc, pour qu’un sous-espace vectoriel faiblement fermé de $L^{\infty}(G)$ soit stable par convolution avec les éléments de $L^1(G)$, il faut et il suffit qu’il soit invariant par les translations de G.

Soit W un sous-espace vectoriel faiblement fermé de $L^{\infty}(G)$. Supposons W (donc aussi $W^{\circ}$) invariant par les translations de G. Soit $f\in$ $L^1(G)$. Pour tout $g\in L^{\infty}(G)$, on a $(\check{f}*g)(x) =\langle \varepsilon_x*f, g\rangle =\langle f, \varepsilon_{x^{-1}}*g\rangle$. Donc, pour que $f$ appartienne à $W^{\circ}$, il faut et il suffit que $\check{f}*g= 0$ pour tout $g\in W$.

Si W est un sous-espace vectoriel de $L^{\infty}(G)$ faiblement fermé et invariant par translation, nous noterons A(W) l’ensemble des caractères $\chi \in \widehat{G}$ qui appartiennent à W. C’est une partie fermée de $\widehat{G}$. Si F est une partie fermée de $\widehat{G}$, nous noterons Y(F) le sous-espace vectoriel faiblement fermé de $L^{\infty}(G)$ engendré par les éléments de F; comme toute translation de G transforme chaque caractère en une fonction proportionnelle à ce caractère, l’espace Y(F) est invariant par translation.

Soit W un sous-espace faiblement fermé de $L^{\infty}(G)$ invariant par les translations de G. D’après le théorème des bipolaires (EVT, II, p. 48, th. 1), un caractère $\chi$ appartient à W si et seulement si il appartient à $(W^{\circ})^{\circ}$; ce dernier espace est l’ensemble des fonctions $g\in L^{\infty}(G)$ telles que $\langle f, g\rangle = 0$ pour $f\in W^{\circ}$. On a $\langle f, \chi \rangle =\overline{\mathscr{F}}(f)(\chi )$, et donc

$$
A(W) = V(W^{\circ})
$$

Similairement, une fonction $f\in L^1(G)$ appartient à $Y(F)^{\circ}$ si et seulement $\langle f, \chi \rangle = 0$ pour tout $\chi \in F$, ce qui équivaut à $\overline{\mathscr{F}}(f)(\chi ) = 0$ pour $\chi \in F$, c’est-à-dire à $f\in \Upsilon (F)$. Donc (loc. cit.) on a

$$
Y(F) = \Upsilon (F)^{\circ}
$$

Les relations V(Υ(F)) = F (I, p. 13 et I, p. 30) et $\Upsilon (V(I))\supset I$, combinées avec le théorème des bipolaires (EVT, II, p. 48, th. 1), entraînent alors

$$
A(Y(F)) = F,Y(A(W))\subset W
$$

#### Proposition 4 {#ts-ii-s3-prop-4 .statement tag=02ND}

Soit W un sous-espace vectoriel faiblement fermé de $L^{\infty}(G)$ invariant par translation et non nul. Alors W contient au moins un caractère de G.

On a vu que $A(W) = V(W^{\circ})$. Comme $W\not= 0$, on a $W^{\circ}\not= L^1(G)$, et alors $V(W^{\circ})$ est non vide d’après le th. 1 de II, p. 252.

#### Proposition 5 {#ts-ii-s3-prop-5 .statement tag=02NE}

Soit W un sous-espace vectoriel faiblement fermé de $L^{\infty}(G)$ invariant par translation.

a) Quel que soit le voisinage U de A(W) dans $\widehat{G}$, toute fonction de W est limite faible de combinaisons linéaires de caractères appartenant à U ;

b) Si la frontière de A(W) ne contient aucun ensemble parfait non vide, toute fonction de W est limite faible de combinaisons linéaires de caractères appartenant à W.

Pour prouver a), il suffit par le théorème des bipolaires de montrer que si $f$ est une fonction de $L^1(G)$ orthogonale aux éléments de U, alors $f$ est orthogonale à W. Or, la cotransformée de Fourier $\overline{\mathscr{F}}(f)$ s’annule alors sur le voisinage U de $A(W) = V(W^{\circ})$, de sorte que la prop. 2 de II, p. 252 montre effectivement que $f\in W^{\circ}$. L’assertion b) s’établit de manière analogue, en employant le th. 2 de II, p. 257 au lieu de la prop. 2 de II, p. 252.

# Exercices

Dans tous les exercices du chapitre II, on identifie le dual de $\mathbf{R}^n$ (resp. de $(\mathbf{R}/\mathbf{Z})^n$, de $\mathbf{Z}^n$) avec $\mathbf{R}^n$ (resp. avec $\mathbf{Z}^n$, avec $(\mathbf{R}/\mathbf{Z})^n$) suivant le corollaire 3 de II, p. 236. Pour $x$ et $y$ dans $\mathbf{R}^n$, on note $x\cdot y=\sum_ix_iy_i$. On note $\mathbf{T}=\mathbf{R}/\mathbf{Z}$, et on munit $\mathbf{T}$ de sa structure de groupe de Lie réel (LIE, III, p. 105, prop. 11). On notera souvent $\widehat{f}$ la transformée de Fourier d’une fonction $f$.

Pour tout nombre réel $t$ non nul, on note s($t$) $=t/|t|$, et on pose s(0) = 0 (fonction signe).

Si E est un espace vectoriel topologique et $(x_h)_{h\in\mathbf{Z}}$ une famille d’éléments de E, on dit que la série de terme général $x_h$ converge symétriquement dans E vers $x\in E$ si la suite $(s_n)_{n\geqslant 1}$ définie par

$$
s_n=\sum_{-n\leqslant h\leqslant n}x_h
$$

converge vers $x$ dans E.

On appelle mesure de probabilité sur un espace topologique localement compact X une mesure positive de masse totale 1. On note $\mathscr{P}(X)$ l’ensemble des mesures de probabilité sur X.

Sauf mention du contraire, G désigne un groupe topologique localement compact commutatif.

## EXERCICES {#ts-ii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
