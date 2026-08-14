---
book: ts
book_title: Théories spectrales
chapter: II
chapter_title: GROUPES LOCALEMENT COMPACTS COMMUTATIFS
section: 1
section_title: Transformation de Fourier
lang: fr
source: ts-i-ii-fr
book_pages: A II.201-A II.243, A II.262-A II.304
pdf_pages: 0213-0255, 0274-0316
extraction: native
subsections:
    - "no": 1
      title: Caractères unitaires d’un groupe localement compact commutatif
      page: 201
      pdf_page: 213
    - "no": 2
      title: Définition de la transformation de Fourier
      page: 206
      pdf_page: 218
    - "no": 3
      title: Le théorème de Plancherel
      page: 210
      pdf_page: 222
    - "no": 4
      title: La formule d’inversion de Fourier
      page: 217
      pdf_page: 229
    - "no": 5
      title: Le théorème de dualité de Pontryagin
      page: 220
      pdf_page: 232
    - "no": 6
      title: Propriétés fonctorielles de la dualité
      page: 224
      pdf_page: 236
    - "no": 7
      title: La formule de Poisson
      page: 229
      pdf_page: 241
    - "no": 8
      title: Exemples de dualité
      page: 232
      pdf_page: 244
    - "no": 9
      title: Transformée de Fourier euclidienne et séries de Fourier
      page: 237
      pdf_page: 249
statements: 95
exercises: 68
content_sha256: 2f7dbed03b68b20aa52adad677b2a1449b233a466fd9ee2ef9d56e087bebcebb
---

## § 1. TRANSFORMATION DE FOURIER

### 1. Caractères unitaires d’un groupe localement compact commutatif

#### Définition 1 {#ts-ii-s1-def-1 .statement tag=02HQ}

On appelle caractère unitaire de G un homomorphisme continu de G dans le groupe multiplicatif $\mathbf{U}$ des nombres complexes de module 1.

Autrement dit, un caractère unitaire est une fonction continue $\chi$ sur G, à valeurs complexes, telle que :

$$
\chi (xy) =\chi (x)\chi (y),|\chi (x)|= 1(x, y\in G)
$$

Dans ce chapitre, on dira souvent simplement « caractère » au lieu de « caractère unitaire ».

Soit E un espace hilbertien de dimension 1, et soit $\chi$ un caractère unitaire de G. L’application qui à $x\in G$ fait correspondre l’homothétie de rapport $\chi (x)$ dans E est une représentation linéaire continue isométrique de G dans E. Réciproquement, toute représentation linéaire continue bornée de G dans E est obtenue par ce procédé, et en particulier est unitaire.

Il est immédiat que le produit de deux caractères unitaires, l’inverse d’un caractère unitaire, et la fonction constante égale à 1 sont des caractères unitaires. Par suite, l’ensemble $\widehat{G}$ des caractères unitaires de G est un groupe pour la multiplication. Ce groupe est commutatif. D’autre part, l’application $(\chi_1, \chi_2)\mapsto \chi_1\chi^{-1}_2=\chi_1\chi_2$ est continue pour la topologie de la convergence compacte et $\widehat{G}$ muni de la topologie de la convergence compacte est un groupe topologique (TG, X, p. 6, corollaire 2 et remarque 1).

#### Définition 2 {#ts-ii-s1-def-2 .statement tag=02HR}

Le groupe topologique $\widehat{G}$ est appelé le groupe dual de G.

Puisque G est localement compact, l’application $(x, \chi )\mapsto \chi (x)$ est continue sur $G\times \widehat{G}$ (TG, X, p. 28, th. 3).

Rappelons que $\mathscr{M}^1(G)$ désigne l’algèbre de Banach involutive unifère des mesures complexes bornées sur G (exemple 4 de I, p. 99). Pour toute mesure complexe bornée $\mu\in \mathscr{M}^1(G)$ et tout $\chi \in \widehat{G}$, on note

$$
\chi (\mu) =\int_G\chi (x)d\mu(x) \tag{1}
$$

(cf. INT, VIII, §2, n$^o6)$.

#### Lemme 1 {#ts-ii-s1-lem-1 .statement tag=02HS}

Pour tout $\chi \in \widehat{G}$, l’application $\mu\mapsto \chi (\mu)$ est un caractère hermitien de l’algèbre de Banach involutive $\mathscr{M}^1(G)$.

D’après INT, VIII, §3, n$^o3$, prop. 11, l’application $\mu\mapsto \chi (\mu)$ est un caractère de l’algèbre de Banach involutive $\mathscr{M}^1(G)$. De plus, on a :

$$
\chi (\mu^*) =\int_G\chi (x^{-1})d\mu(x) =\int_G\chi (x)d\mu(x) =\chi (\mu)
$$

et ce caractère est donc hermitien.

On a ainsi défini une application de $\widehat{G}$ dans $\mathsf{X}(\mathscr{M}^1(G))$ ; on la qualifiera de canonique.

Soit $\chi \in \widehat{G}$. La restriction de $\mu\mapsto \chi (\mu)$ à $L^1(G)$ est non nulle (cf. INT, VIII, §2, n$^o7$, prop. 10). Par restriction à la sous-algèbre de Banach involutive $L^1(G)$, on obtient donc une application de $\widehat{G}$ dans $\mathsf{X}(L^1(G))$, dite canonique. Elle associe à $\chi \in \widehat{G}$ le caractère hermitien

$$
f\mapsto \chi (f) =\chi (f\cdot dx) =\int_Gf(x)\chi (x)dx(f\in L^1(G)) \tag{2}
$$

de $L^1(G)$.

#### Proposition 1 {#ts-ii-s1-prop-1 .statement tag=02HT}

L’application canonique de $\widehat{G}$ dans $\mathsf{X}(L^1(G))$ est un homéomorphisme.

Notons ev cette application canonique et, pour $\chi \in \widehat{G}$, notons ev$_{\chi}$ l’image du caractère $\chi$ par ev, c’est-à-dire le caractère hermitien $f\mapsto \chi (f)$ de $L^1(G)$. Considérée comme une application de $\widehat{G}$ dans le dual de $L^1(G)$, l’application ev est la composée de l’injection de $\widehat{G}$ dans $L^{\infty}(G)$, muni de la topologie faible $\sigma (L^{\infty}(G),L^1(G))$, et de l’injection de $L^{\infty}(G)$ dans le dual de $L^1(G)$, muni de la topologie de la convergence simple. Comme $\widehat{G}$ est une partie bornée de $L^{\infty}(G)$, la première application est continue d’après le théorème de Lebesgue (INT, IV, §3, n$^o7$, th. 6). La seconde est également continue, par définition. Ceci démontre que l’application ev est continue.

Si $\chi \in \widehat{G}$ et si $f\in L^1(G)$, on a ev$_{\chi}(\varepsilon_x*f) =\chi (x$)ev$_{\chi}(f)$. En prenant $f$ telle que ev$_{\chi}(f)\not= 0$, on en déduit que l’application ev est injective.

Soit $\zeta \in \mathsf{X}(L^1(G))$ et soit $f\in L^1(G)$ telle que $\zeta (f)\not= 0$. Définissons une application $\chi : G\rightarrow \mathbf{C}$ en posant, pour $x\in G$ :

$$
\zeta (\varepsilon_x*f)
$$

$$
\chi (x) = \tag{3}
$$

$$
\zeta (f)
$$

On a $\chi (e) = 1$. Comme l’application $x\mapsto \varepsilon_x*f=\boldsymbol{\gamma }(x)(f)$ de G dans $L^1(G)$ est continue (INT, VIII, §2, n$^o5$, prop. 8), l’application $\chi$ est continue. Elle est bornée car, pour tout $x\in G$, on a

$$
\|\varepsilon_x*f\|\|f\|
$$

$|\chi (x)|\leqslant$ =

$$
|\zeta (f)||\zeta (f)|
$$

(th. 1 de I, p. 29 et INT, VIII, loc. cit.).

Soit maintenant $\mathfrak{B}$ une base du filtre des voisinages de $e$ formée de voisinages compacts. Pour tout $V\in \mathfrak{B}$, soit $g_V$ une fonction continue positive, nulle en dehors de V et d’intégrale égale à 1 (lemme 1 de II, p. 200). Pour toute fonction $h\in L^1(G)$, on a alors

$\varepsilon_x*h=$ lim$(\varepsilon_x*h)*g_V=$ lim$(\varepsilon_x*g_V*h)$,

$V,\mathfrak{B}V,\mathfrak{B}$

dans $L^1(G)$, la limite étant prise suivant le filtre des sections de $\mathfrak{B}$ (INT, VIII, §4, n$^o7$, prop. 20). En particulier, comme $\zeta (\varepsilon_x*g_V*f) =$ $\zeta (\varepsilon_x*g_V)\zeta (f)$, on en déduit que

$\chi (x) =$ lim $\zeta (\varepsilon_x*g_V)$.

$V,\mathfrak{B}$

Pour tout $h\in L^1(G)$, on obtient

$\zeta (\varepsilon_x*h) =$ lim $\zeta (\varepsilon_x*g_V*h) =\zeta (h)$ lim $\zeta (\varepsilon_x*g_V) =\chi (x)\zeta (h)$.

$V,\mathfrak{B}V,\mathfrak{B}$

Par suite, on a pour $x, y\in G$ :

$$
\zeta (\varepsilon_x*\varepsilon_y*f)\chi (x)\zeta (\varepsilon_y*f)
$$

$\chi (xy) =$ = $=\chi (x)\chi (y)$,

$$
\zeta (f)\zeta (f)
$$

ce qui démontre que $\chi$ est un homomorphisme de G dans $\mathbf{C}^*$. Comme $\chi$ est borné et continu, c’est un caractère unitaire de G. De plus, si $g\in L^1(G)$, on a

$$
g*f=\int_G(\varepsilon_x*f)g(x)dx
$$

dans $L^1(G)$ (INT, VIII, §1, n$^o5$, prop. 7), d’où

$$
\zeta (g)\zeta (f) =\zeta (g*f) =\int_G\zeta (\varepsilon_x*f)g(x)dx
$$

$=\zeta (f)\int_G\chi (x)g(x)dx=$ ev$_{\chi}(g)\zeta (f)$ (INT, VI, §1, n$^o1$, prop. 1) ce qui montre que $\zeta =$ ev$_{\chi}$. Par suite, ev est surjective, donc bijective.

Montrons finalement que l’application réciproque ev$^{-1}$ est continue. Soit $\zeta \in \mathsf{X}(L^1(G))$. Soit $f\in L^1(G)$ une fonction telle que $\zeta (f)\not= 0$. L’ensemble W des $\xi \in \mathsf{X}(L^1(G))$ tels que $\xi (f)\not= 0$ est un voisinage ouvert de $\zeta$ dans $\mathsf{X}(L^1(G))$. Pour tout $\xi \in W$, ce qui précède montre que ev$^{-1}(\xi )$ est le caractère

$$
\xi (\varepsilon_x*f)
$$

$$
x\mapsto
$$

$$
\xi (f)
$$

Soit $\mathfrak{F}$ un filtre sur $W\subset \mathsf{X}(L^1(G))$ convergeant vers $\zeta$. Puisque l’ensemble $\mathsf{X}(L^1(G))$ est borné, donc équicontinu, dans $L^{\infty}(G)$, la structure uniforme de la convergence simple coïncide avec la structure uniforme de la convergence compacte (TG, X, p. 16, th. 1). Soit K une partie compacte de G. L’ensemble des $\varepsilon_x*f$ pour $x\in K$ est compact dans $L^1(G)$ (INT, VIII, §2, n$^o5$, prop. 8). On a donc

lim $\xi (\varepsilon_x*f) =\zeta (\varepsilon_x*f)$

$\xi ,\mathfrak{F}$

uniformément pour $x\in K$. On en déduit que

lim$_{\xi ,\mathfrak{F}}$ ev$^{-1}(\xi ) =$ ev$^{-1}(\zeta )$,

donc ev$^{-1}$ est continue en $\zeta$. Ceci achève la démonstration de la proposition.

Nous identifierons désormais un caractère unitaire $\chi$ de G au caractère $f\mapsto \int_Gf(x)\chi (x)dx$ de $L^1(G)$.

#### Remarque 1 {#ts-ii-s1-n1-rem-1 .statement tag=02HU}

*La bijectivité de l’application de $\widehat{G}$ dans $\mathsf{X}(L^1(G))$ de la prop. 1 est un cas particulier de la correspondance entre représentations continues d’un groupe localement compact H (non nécessairement commutatif) et représentations continues de l’algèbre $L^1(H)$.*

#### Remarque 2 {#ts-ii-s1-n1-rem-2 .statement tag=02HV}

L’application canonique de $\widehat{G}$ dans $\mathsf{X}(\mathscr{M}^1(G))$ n’est pas surjective en général (II, p. 308, exerc. 14).

#### Corollaire 1 {#ts-ii-s1-prop-1-cor-1 .statement tag=02HW}

Tout caractère de $L^1(G)$ est hermitien. L’application canonique de $\mathsf{X}$(Stell(G)) (déf. 9 de I, p. 125) dans $\mathsf{X}(L^1(G))$ est un homéomorphisme.

La première assertion résulte de la proposition 1 et du lemme 1 en restriction à $L^1(G)$. La seconde résulte de la première et du cor. de la prop. 20 de I, p. 124.

#### Corollaire 2 {#ts-ii-s1-prop-1-cor-2 .statement tag=02HX}

Le groupe topologique $\widehat{G}$ est localement compact.

En effet, $\mathsf{X}(L^1(G))$ est localement compact (corollaire du théorème 1 de I, p. 29).

Nous identifierons $\widehat{G}$ avec $\mathsf{X}(L^1(G))$ et $\mathsf{X}$(Stell(G)). Pour $x\in G$ et $\chi \in \widehat{G}$, nous noterons $\langle \chi , x\rangle$ le nombre complexe $\chi (x)$, qui appartient à $\mathbf{U}$.

On dit que $x$ et $\chi$ sont orthogonaux si $\langle \chi , x\rangle = 1$. Soit A une partie de G (resp. de $\widehat{G})$; l’ensemble des éléments de $\widehat{G}$ (resp. de G) orthogonaux à A est un sous-groupe fermé de $\widehat{G}$ (resp. de G) qu’on appelle orthogonal de A et qu’on note $A^{\bot}$. L’orthogonal de G est réduit à $e$.

Pour $x\in G$, notons $\eta (x)$ l’application de $\widehat{G}$ dans $\mathbf{U}$ définie par $\chi \mapsto$ $\langle \chi , x\rangle$. Par définition de la multiplication dans $\widehat{G}$, l’application $\eta (x)$ est un homomorphisme de groupes. Elle est continue puisque l’application $(x, \chi )\mapsto  \langle \chi , x\rangle$ de $G\times \widehat{G}$ dans $\mathbf{U}$ est continue (TG, X, p. 28, th. 3). Nous avons ainsi défini une application $\eta$, dite canonique, de G dans le groupe bidual $\widehat{\widehat{G}}$; c’est un homomorphisme de groupes. De plus, l’application $\eta$ est continue (TG, X, p. 28, th. 3). Nous démontrerons plus loin (II, p. 220, th. 2) que $\eta$ est un isomorphisme de groupes topologiques de G sur $\widehat{\widehat{G}}$.

Soient G et H des groupes localement compacts commutatifs, et $\varphi : G\rightarrow H$ un morphisme de groupes topologiques. Pour tout $\chi \in \widehat{H}$, l’application $\chi \circ \varphi$ est un caractère de G noté $\widehat{\varphi}(\chi )$. Cette définition se traduit par la formule

$$
\langle \chi , \varphi (x)\rangle =\langle \widehat{\varphi}(\chi ), x\rangle \tag{4}
$$

quels que soient $\chi \in \widehat{H}$ et $x\in G$. On en déduit que $\widehat{\varphi}$ est un morphisme du groupe topologique $\widehat{H}$ dans le groupe topologique $\widehat{G}$; on dit que $\widehat{\varphi}$ est le dual du morphisme $\varphi$.

Soient K un groupe localement compact commutatif et $\psi : H\rightarrow K$ un morphisme de groupes topologiques. La définition montre que $\widehat{\psi}\circ \varphi =\widehat{\varphi}\circ \widehat{\psi}$. Si $\varphi$ est l’application identique de G, alors $\widehat{\varphi}$ est l’application identique de $\widehat{G}$. En particulier, si $\varphi$ est un isomorphisme de groupes topologiques, il en est de même de $\widehat{\varphi}$, et $\widehat{\varphi}^{-1}$ est le dual de $\varphi^{-1}$.

#### Lemme 2 {#ts-ii-s1-lem-2 .statement tag=02HY}

Soient G et H des groupes localement compacts commutatifs et soit $f: H\rightarrow G$ un morphisme de groupes topologiques. Le noyau de $\widehat{f}$ est l’orthogonal de l’image de $f$.

Par définition, on a $\chi \in$ Ker($\widehat{f}$) si et seulement si la restriction de $\chi$ à l’image de $f$ est triviale.

#### Proposition 2 {#ts-ii-s1-prop-2 .statement tag=02HZ}

Soit $n\geqslant 0$ un entier et soient $G_1, . . . ,G_n$ des groupes commutatifs localement compacts. Soit G le groupe produit des groupes $G_j$ pour $1\leqslant j\leqslant n$. Pour $1\leqslant j\leqslant n$, soit $\lambda_j$ l’injection de $G_j$ dans G qui associe à $x\in G_j$ l’élément $(x_k)$ tel que $x_k=e$ si $k\not=j$ et $x_j=x$. L’application

$$
(\widehat{\lambda}_j)_{1\leqslant j\leqslant n}:\widehat{G}\rightarrow \prod_{1\leqslant j\leqslant n}\widehat{G}_j
$$

est un isomorphisme de groupes topologiques.

Soit $m$ l’application produit de $\widehat{G}^n$ dans $\widehat{G}$, et pour tout $j$ tel que $1\leqslant j\leqslant n$, soit $\pi_j$ la projection de G sur $G_j$. Soit $\mu$ le morphisme de groupes topologiques $m\circ (\widehat{\pi}_j)_j$ de $\prod\widehat{G}_j$ dans $\widehat{G}$, de sorte que

$$
\langle \mu((\chi_j)),(x_j)\rangle =\prod_{j=1}^n\langle \chi_j, x_j\rangle
$$

L’application $\mu$ est continue, et on vérifie que $\mu$ et $(\widehat{\lambda}_j)$ sont des bijections réciproques l’une de l’autre. La proposition en résulte.

#### Remarque {#ts-ii-s1-n1-rem-3 .statement tag=02I0}

Le calcul du groupe dual d’un produit infini de groupes compacts commutatifs est l’objet du corollaire 4 de II, p. 234 ci-dessous. Le cas d’un groupe localement compact commutatif qui est un produit quelconque de groupes localement compacts découle de ces deux énoncés, puisque dans un tel produit, tous les facteurs sauf un nombre fini sont compacts (TG, I, p. 66, prop. 14, b)).

### 2. Définition de la transformation de Fourier

#### Définition 3 {#ts-ii-s1-def-3 .statement tag=02I1}

Soit $\mu\in \mathscr{M}^1(G)$ une mesure complexe bornée sur G. On appelle transformée de Fourier de $\mu$ la fonction $\mathscr{F}_G(\mu)$ sur $\widehat{G}$ définie par

$$
\mathscr{F}_G(\mu)(\widehat{x}) =\int_G\langle \widehat{x}, x\rangle d\mu(x) \tag{5}
$$

On appelle cotransformée de Fourier de $\mu$ la fonction $\mathscr{F}_G(\mu)$ sur $\widehat{G}$ definie par

$$
\mathscr{F}_G(\mu)(\widehat{x}) =\int_G\langle \widehat{x}, x\rangle d\mu(x) \tag{6}
$$

Lorsque il n’y a pas d’ambiguïté concernant le groupe G considéré, on écrira aussi $\mathscr{F}(\mu)$ et $\mathscr{F}(\mu)$. On note aussi parfois $\widehat{\mu}=\mathscr{F}_G(\mu)$.

#### Proposition 3 {#ts-ii-s1-prop-3 .statement tag=02I2}

Pour toute mesure $\mu\in \mathscr{M}^1(G)$, les fonctions $\mathscr{F}_G(\mu)$ et $\mathscr{F}_G(\mu)$ sont continues et bornées. Les applications $\mathscr{F}_G:\mu\mapsto$ $\mathscr{F}_G(\mu)$ et $\mathscr{F}_G:\mu\mapsto \mathscr{F}_G(\mu)$ sont des morphismes continus de l’algèbre involutive $\mathscr{M}^1(G)$ dans l’algèbre involutive des fonctions continues bornées sur $\widehat{G}$ (exemple 1 de I, p. 99).

Soit $\mu\in \mathscr{M}^1(G)$. Pour tout $\chi \in \widehat{G}$, on a

$$
|\mathscr{F}(\mu)(\chi )|=\int_G\langle \chi , x\rangle d\mu(x)\leqslant \|\mu\|_1 \tag{7}
$$

donc la transformée de Fourier de $\mu$ est bornée. Similairement, on vérifie que $\mathscr{F}(\mu)$ est bornée.

Si $\chi$ tend vers $\chi_0$ dans $\widehat{G}$, la fonction $\chi$ sur G tend vers $\chi_0$ uniformément sur tout compact en restant bornée par la fonction constante 1 qui appartient à $L^1(G, \mu)$. D’après le théorème de Lebesgue (INT, IV, §3, n$^o7$, th. 6), il en résulte que $\mathscr{F}(\mu)(\chi )$ tend vers $\mathscr{F}(\mu)(\chi_0)$. Donc $\mathscr{F}(\mu)$ est continue. Il en est de même de $\mathscr{F}(\mu)$.

Pour tout $\chi \in \widehat{G}$, l’application $\mu\mapsto \chi (\mu) =\int\langle \chi , x\rangle d\mu(x)$ est un caractère hermitien de $\mathscr{M}^1(G)$ (lemme 1 de II, p. 202). Cela entraîne que $\mathscr{F}$ et $\mathscr{F}$ sont des morphismes d’algèbres involutives de $\mathscr{M}^1(G)$ dans l’algèbre involutive des fonctions continues bornées sur $\widehat{G}$. L’inégalité (7) démontre que ces morphismes sont continus.

La transformation de Fourier de G (resp. la cotransformation de Fourier de G) est l’application $\mu\mapsto \mathscr{F}_G(\mu)$ (resp. l’application $\mu\mapsto$ $\mathscr{F}_G(\mu)$) de $\mathscr{M}^1(G)$ dans $\mathscr{C}_b(\widehat{G})$.

Notons quelques formules utiles pour $\mu\in \mathscr{M}^1(G),x\in G$ et $\chi \in \widehat{G}:$

$$
\mathscr{F}(\mu)(\chi ) =\mathscr{F}(\mu)(\chi^{-1}) =\mathscr{F}(\mu)(\chi ) \tag{8}
$$

$$
\|\mathscr{F}(\mu)\|_{\infty}=\|\mathscr{F}(\mu)\|_{\infty}\leqslant \|\mu\|_1 \tag{9}
$$

$$
\mathscr{F}(\varepsilon_x)(\chi ) =\langle \chi , x\rangle
$$

(10)

$$
\mathscr{F}(\varepsilon_x)(\chi ) =\langle \chi , x\rangle
$$

(en particulier $\mathscr{F}(\varepsilon_e) =\mathscr{F}(\varepsilon_e) = 1$),

$$
\mathscr{F}(\varepsilon_x*\mu)(\chi ) =\langle \chi , x\rangle \mathscr{F}(\mu)(\chi )
$$

(11)

$$
\mathscr{F}(\varepsilon_x*\mu)(\chi ) =\langle \chi , x\rangle \mathscr{F}(\mu)(\chi )
$$

$$
\mathscr{F}(\chi \cdot \mu) =\varepsilon_{\chi}*\mathscr{F}(\mu)
$$

(12)

$$
\mathscr{F}(\chi \cdot \mu) =\varepsilon_{\chi^{-1}}*\mathscr{F}(\mu)
$$

Les formules (8), (9), (10) et (11) découlent des définitions. Démontrons la première des formules (12), la seconde étant analogue. On a pour tout $\xi$ dans $\widehat{G}$ les égalités

$$
\mathscr{F}(\chi \cdot \mu)(\xi ) =\int_G\langle \xi , x\rangle \langle \chi , x\rangle d\mu(x) =\int_G\langle \xi \chi^{-1}, x\rangle d\mu(x)
$$

$$
=\mathscr{F}(\mu)(\xi \chi^{-1}) = (\varepsilon_{\chi}*\mathscr{F}(\mu))(\xi )
$$

Notons par ailleurs que pour tout $\chi \in \widehat{G}$ et toutes mesures $\mu$ et $\nu$ dans $\mathscr{M}^1(G)$, on a

$$
(\varepsilon_{\chi}*\mathscr{F}(\mu))(\varepsilon_{\chi}*\mathscr{F}(\nu )) =\varepsilon_{\chi}*(\mathscr{F}(\mu)\mathscr{F}(\nu )) \tag{13}
$$

puisque les deux membres de cette égalité sont des fonctions sur $\widehat{G}$ dont la valeur en $\xi \in \widehat{G}$ est

$$
\mathscr{F}(\mu)(\xi \chi^{-1})\mathscr{F}(\nu )(\xi \chi^{-1})
$$

Soit H un groupe localement compact commutatif et soit $\varphi : G\rightarrow H$ un morphisme continu. Soit $\mu\in \mathscr{M}^1(G)$. La mesure image $\varphi (\mu)$ est définie (INT, V, §6, n$^o1$, remarque 1), et il vient $\mathscr{F}_H(\varphi (\mu)) =\mathscr{F}_G(\mu)\circ$ $\widehat{\varphi}($cf. INT, V, §6, n$^o4$, prop. 7).

Par restriction à la sous-algèbre $L^1(G)$ de $\mathscr{M}^1(G)$, on obtient la définition de la transformation de Fourier et de la cotransformation de Fourier sur $L^1(G)$. On a donc pour $f\in L^1(G)$ et $\chi \in \widehat{G}:$

$$
(14)\mathscr{F}_G(f)(\chi ) =\int_G\langle \chi , x\rangle f(x)dx,\mathscr{F}_G(f)(\chi ) =\int_G\langle \chi , x\rangle f(x)dx
$$

En particulier, $\mathscr{F}_G(f) =\mathscr{F}_G(f)$. On a aussi

$$
\mathscr{F}(f)(\chi ) =\chi (f) \tag{15}
$$

pour tout $f\in L^1(G)$ et tout $\chi \in \widehat{G}$.

Soient $\sigma$ un automorphisme de G et Δ le module de $\sigma$ (INT, VII, §1, n$^o4$, déf. 4). Pour $f\in L^1(G)$, on a

$$
\mathscr{F}(f\circ \sigma ) = \Delta^{-1}\mathscr{F}(f)\circ \widehat{\sigma}^{-1} \tag{16}
$$

(cf. loc. cit., formule (31)).

Si l’on identifie $\widehat{G}$ et $\mathsf{X}(L^1(G))$ (prop. 1 de II, p. 202), la cotransformation de Fourier n’est autre que la transformation de Gelfand de l’algèbre de Banach $L^1(G)$ (I, p. 7, déf. 5).

#### Proposition 4 {#ts-ii-s1-prop-4 .statement tag=02I3}

La transformation de Fourier et la cotransformation de Fourier sont des morphismes injectifs d’algèbres involutives de $L^1(G)$ dans l’algèbre $\mathscr{C}_0(\widehat{G})$ des fonctions continues nulles à l’infini sur $\widehat{G}$.

La cotransformation de Fourier est un morphisme d’algèbres involutives de $L^1(G)$ dans l’algèbre des fonctions continues bornées sur $\widehat{G}$ (prop. 3). Comme elle s’identifie à la transformation de Gelfand, son image est contenue dans $\mathscr{C}_0(\widehat{G})$ (I, p. 37, prop. 5), et son noyau est le radical de $L^1(G)$ (prop. 8 de I, p. 38), qui est nul (cor. de la prop. 22 de I, p. 126).

Nous verrons ultérieurement (corollaire de la proposition 13 de II, p. 221) que la cotransformation de Fourier sur $\mathscr{M}^1(G)$ est également injective.

#### Remarque {#ts-ii-s1-n2-rem-1 .statement tag=02I4}

La transformation de Fourier sur l’espace $L^1(G)$ dépend du choix de la mesure de Haar $dx$, contrairement à la transformation de Fourier sur $\mathscr{M}^1(G)$. Si l’on remplace $dx$ par la mesure $a\cdot dx$ (avec $a >0$), alors pour toute fonction $f$ intégrable sur G, la transformée de Fourier de $f$ est $a\widehat{f}$, où $\widehat{f}$ est la transformée de Fourier définie relativement à la mesure $dx$.

Considérons l’algèbre stellaire Stell(G) du groupe G (déf. 9 de I, p. 125), et identifions $L^1(G)$ à une sous-algèbre dense de Stell(G) (prop. 22 de I, p. 126).

#### Proposition 5 {#ts-ii-s1-prop-5 .statement tag=02I5}

Par continuité, la transformation de Fourier et la cotransformation de Fourier se prolongent de manière unique en des isomorphismes d’algèbres stellaires de Stell(G) sur $\mathscr{C}_0(\widehat{G})$.

La cotransformation de Fourier se prolonge par continuité en un morphisme d’algèbres stellaires de Stell(G) dans $\mathscr{C}_0(\widehat{G})$. Si l’on identifie $\widehat{G}$ avec $\mathsf{X}$(Stell(G)) (cor. 1 de II, p. 204 et prop. 1 de II, p. 202), ce prolongement est la transformation de Gelfand de Stell(G). D’après le th. 1 de I, p. 108, c’est un isomorphisme. L’assertion concernant la transformation de Fourier en découle.

On notera toujours $\mathscr{F}$ et $\mathscr{F}$ les isomorphismes de la prop. 5.

#### Corollaire {#ts-ii-s1-n2-cor-1 .statement tag=02I6}

L’image de $L^1(G)$ par la transformation de Fourier de G est dense dans $\mathscr{C}_0(\widehat{G})$.

Puisque $L^1(G)$ est dense dans Stell(G), cela découle de la proposition 5.

#### Proposition 6 {#ts-ii-s1-prop-6 .statement tag=02I7}

Supposons que G est compact. La mesure de Haar normalisée $dx$ appartient à $\mathscr{M}^1(G)$, et sa transformée de Fourier est $\varphi_e$, la fonction caractéristique de $\{e\}$.

Soit $\chi \in \widehat{G}$. Puisque $\varepsilon_y*dx=dx$ pour tout $y\in G$, on a

$$
\mathscr{F}(dx)(\chi ) =\langle \chi , y\rangle \mathscr{F}(dx)(\chi )
$$

d’après la formule (11). Si $\chi \not= 1$, il existe $y\in G$ tel que $\langle \chi , y\rangle  \not= 1$, donc $\mathscr{F}(dx)(\chi ) = 0$. Si $\chi = 1$, alors $\mathscr{F}(dx)(\chi ) =\int_Gdx= 1$ puisque la mesure $dx$ est normalisée.

### 3. Le théorème de Plancherel

On note A(G) le sous-espace vectoriel de $L^1(G)$ engendré par les fonctions $f*g$ pour $f, g\in L^1(G)\cap L^2(G)$.

#### Proposition 7 {#ts-ii-s1-prop-7 .statement tag=02I8}

L’espace A(G) est un idéal auto-adjoint de $L^1(G)$. Il est contenu dans $L^1(G)\cap L^2(G)$, et dans l’image de $\mathscr{C}(G)$ dans $L^1(G)$.

Soit $f\in L^1(G)$. Pour tout $g\in L^2(G)$, on a $f*g\in L^1(G)$ (INT, VIII, §4, n$^o5$, prop. 12). Par conséquent, l’espace $L^1(G)\cap L^2(G)$ est un idéal de $L^1(G)$, et il en est de même de l’espace A(G). L’idéal A(G) est auto-adjoint.

Soient $f$ et $g$ dans $L^2(G)$. Le produit de convolution $f*g$ est alors la classe de la fonction continue donnée par

$$
y\mapsto \int_Gf(yx^{-1})g(x)dx
$$

(INT, VIII, §4, n$^o5$, prop. 15). La seconde assertion en résulte.

Comme $\chi (f*g) = (\chi f)*(\chi g)$ pour $\chi \in \widehat{G},f\in L^1(G)$ et $g\in L^1(G)$ (INT, VIII, §3, n$^o1$, prop. 6), on a $\chi h\in A(G)$ pour tout $h\in A(G)$ et $\chi \in \widehat{G}$. Comme $\varepsilon_x*f=\boldsymbol{\gamma }(x)f$ et la représentation linéaire $\boldsymbol{\gamma }$ est isométrique sur $L^p(G)$ pour tout $p$ (INT, VIII, §2, n$^o5$, prop. 8), on a $\varepsilon_x*f\in A(G)$ pour tous $x\in G$ et $f\in A(G)$.

On note $\widehat{A}(G)$ l’image de A(G) par la transformation de Fourier. C’est un sous-espace de $\mathscr{C}_0(\widehat{G})$.

#### Proposition 8 {#ts-ii-s1-prop-8 .statement tag=02I9}

Il existe une base de filtre $\mathfrak{B}$ sur $A(G)\cap \mathscr{K}_+(G)$ telle que les conditions suivantes soient vérifiées :

(i) Pour tout élément $\varphi$ d’un ensemble de $\mathfrak{B}$, on a $\|\varphi \|_1= 1$ et $\|\mathscr{F}(\varphi )\|_{\infty}\leqslant 1$ ;

(ii) On a

lim $\varphi \cdot dx=\varepsilon_e$

$\varphi ,\mathfrak{B}$

dans l’espace $\mathscr{C}'(G)$ des mesures à support compact sur G muni de la topologie de la convergence uniforme sur les parties compactes de $\mathscr{C}(G)$ ;

(iii) On a

lim$_{\varphi ,\mathfrak{B}}\mathscr{F}(\varphi ) = 1$

pour la topologie de la convergence compacte sur $\widehat{G}$;

(iv) Pour $p= 1$ ou $p= 2$, et pour tout $f\in L^p(G)$, on a $\varphi *f\in$ A(G) pour tout $\varphi$ appartenant à un ensemble de $\mathfrak{B}$ et

lim $\varphi *f=f$

$\varphi ,\mathfrak{B}$

dans $L^p(G)$.

Soit $K_0$ un voisinage compact fixé de $e$ dans G. Soit $\mathfrak{B}_0$ une base du filtre des voisinages de $e$ dans G formée de voisinages compacts symétriques contenus dans $K_0$ (cf. TG, III, p. 4). Pour K $\in \mathfrak{B}_0$, soit $X'_K$ l’ensemble des fonctions $\psi \in \mathscr{K}_+(G)$ telles que Supp$(\psi )\subset K$ et $\int\psi (x)dx= 1$ ; il est non vide (lemme 1 de II, p. 200). Soit $X_K$ l’ensemble des fonctions $\psi *\psi$ pour $\psi \in X'_K$. Il est non vide et contenu dans $A(G)\cap \mathscr{K}_+(G)$. L’ensemble $\mathfrak{B}$ dont les éléments sont les ensembles $X_K$ pour K variant dans $\mathfrak{B}_0$ est une base de filtre sur $A(G)\cap \mathscr{K}_+(G)$. Démontrons que $\mathfrak{B}$ vérifie les propriétés demandées.

Si $X\in \mathfrak{B}$ et $\varphi \in X$, on a $\|\varphi \|_1=\int_G\varphi (x)dx= 1$, donc $\|\mathscr{F}(\varphi )\|_{\infty}\leqslant 1$, ce qui établit la propriété (i).

La propriété (ii) résulte de INT, VIII, § 2, n$^o7$, corollaire 1 du lemme 4. Une partie compacte de $\widehat{G}$ est une partie compacte de $\mathscr{C}(G)$, donc (ii) entraîne lim$_{\varphi ,\mathfrak{B}}\mathscr{F}(\varphi ) = 1$ pour la topologie de la convergence

compacte sur $\widehat{G}$, c’est-à-dire (iii).

Finalement, soit $p= 1$ ou $p= 2$. Soit $f\in L^p(G)$. On a $\varphi *f\rightarrow f$ dans $L^p(G)$ selon le filtre $\mathfrak{B}$ (INT, VIII, §4, n$^o7$, prop. 20). De plus, pour tout K dans $\mathfrak{B}_0$ et $\varphi \in X_K$, il existe $\psi \in X_K'$ tel que $\varphi =\psi *\psi$, d’où $\varphi *f=\psi *(\psi *f)$. On a $\psi \in L^1(G)\cap L^2(G)$ et $\psi *f\in L^1(G)\cap L^2(G)$, donc $\varphi *f\in A(G)$.

#### Corollaire 1 {#ts-ii-s1-prop-8-cor-1 .statement tag=02IA}

L’espace A(G) est dense dans $L^1(G)$ et dans $L^2(G)$. Il est également dense dans Stell(G), et son image $\widehat{A}(G)$ par la transformation de Fourier est dense dans $\mathscr{C}_0(\widehat{G})$.

L’assertion (iv) de la proposition fournit la première assertion. Puisque $L^1(G)$ est dense dans Stell(G), la seconde en résulte, et la dernière découle alors de la prop. 5 de II, p. 209.

#### Corollaire 2 {#ts-ii-s1-prop-8-cor-2 .statement tag=02IB}

Pour $f\in A(G)$, soit $\Omega_f$ l’ensemble des $\chi \in \widehat{G}$ tels que $\mathscr{F}(f)(\chi )\not= 0$. Les ensembles $\Omega_f$ forment un recouvrement ouvert de $\widehat{G}$.

Cela découle du corollaire précédent puisque, pour tout $\chi \in \widehat{G}$, l’application $f\mapsto \mathscr{F}(f)(\chi )$ est un caractère non nul de $L^1(G)$.

Rappelons que la représentation régulière gauche $\boldsymbol{\gamma }$ de Stell(G) sur $L^2(G)$ (cf. I, p. 125, n$^o13$) est notée $\boldsymbol{\gamma }(\varphi )f$ = $\varphi *f$ pour $\varphi \in$ Stell(G) et $f\in L^2(G)$.

#### Lemme 3 {#ts-ii-s1-lem-3 .statement tag=02IC}

Pour tout $f\in A(G)$, il existe une unique mesure bornée $\mu_f$ sur $\widehat{G}$ telle que

$$
(\varphi *f)(e) =\int_{\widehat{G}}\mathscr{F}(\varphi )d\mu_f \tag{17}
$$

quel que soit $\varphi \in$ Stell(G).

De plus, pour tous $f$ et $g$ dans A(G), on a l’égalité

$$
\mathscr{F}(f)\cdot \mu_g=\mathscr{F}(g)\cdot \mu_f \tag{18}
$$

entre la mesure de densité $\mathscr{F}(f)$ par rapport à $\mu_g$ et la mesure de densité $\mathscr{F}(g)$ par rapport à $\mu_f$.

Soient $f,g$ des éléments de $L^1(G)\cap L^2(G)$. Pour tout $\varphi \in$ Stell(G), on a $\varphi *f\in L^2(G)$ et $\|\varphi *f\|_2\leqslant \|\varphi \|_*\|f\|_2($I, p. 126, formule (8)). De plus, on a $\varphi *(f*g) = (\varphi *f)*g($loc. cit., formule (9)). Cette dernière fonction appartient à l’adhérence $\mathscr{C}_0(G)$ de $\mathscr{K}(G)$ dans $\mathscr{C}(G)$ (INT, VIII, §4, n$^o5$, prop. 15). De plus, on a

$$
\|\varphi *(f*g)\|_{\infty}\leqslant \|\varphi *f\|_2\|g\|_2\leqslant \|\varphi \|_*\|f\|_2\|g\|_2
$$

Puisque les fonctions $f*g$ pour $f$ et $g$ dans $L^1(G)\cap L^2(G)$ engendrent A(G), on en déduit que $\varphi *f\in \mathscr{C}_0(G)$ pour tous $f\in A(G)$ et $\varphi \in$ Stell(G), et que l’application $\varphi \mapsto (\varphi *f)(e)$ est une forme linéaire continue sur Stell(G). Comme $\mathscr{F}$ est un isomorphisme de Stell(G) sur $\mathscr{C}_0(\widehat{G})$ (prop. 5 de II, p. 209), la première assertion en résulte.

Soient maintenant $f$ et $g$ dans A(G). Pour $\varphi \in L^1(G)$, on a

$$
\mathscr{F}(f)\cdot \mu_g(\mathscr{F}(\varphi )) =\int_{\widehat{G}}\mathscr{F}(\varphi )\mathscr{F}(f)d\mu_g=\int_{\widehat{G}}\mathscr{F}(\varphi *f)d\mu_g
$$

$$
= ((\varphi *f)*g)(e) \tag{19}
$$

Comme $(\varphi *f)*g= (\varphi *g)*f$ et comme l’image de $L^1(G)$ par la transformation de Fourier est dense dans $\mathscr{C}_0(\widehat{G})$ (cor. de II, p. 210), on déduit de la formule (19) que la formule (18) est satisfaite pour tous $f$ et $g$ dans A(G).

#### Lemme 4 {#ts-ii-s1-lem-4 .statement tag=02ID}

Il existe une unique mesure $\nu$ sur $\widehat{G}$ telle que

$$
\mu_f=\mathscr{F}(f)\cdot \nu
$$

pour tout $f\in A(G)$. Pour $f\in A(G)$, on a $\mathscr{F}(f)\in L^1(\widehat{G}, \nu )\cap L^2(\widehat{G}, \nu )$.

Soit $f\in A(G)$. Notons $\Omega_f$ l’ensemble ouvert dans $\widehat{G}$ formé des $\chi \in \widehat{G}$ tels que $\mathscr{F}(f)(\chi )\not= 0$. Soit $\varphi$ la fonction caractéristique de $\widehat{G}-\Omega_f$. Pour tout $g\in A(G)$, on a alors

$$
\int_{\widehat{G}}\mathscr{F}(g)d(\varphi \cdot \mu_f) =\int_{\widehat{G}}\varphi \mathscr{F}(f)d\mu_g= 0
$$

compte tenu de la formule (18).

D’après le corollaire 1 de II, p. 212, l’image $\widehat{A}(G)$ de A(G) par la transformation de Fourier est dense dans $\mathscr{C}_0(\widehat{G})$. On déduit alors de la formule précédente que $\varphi \cdot \mu_f= 0$, donc que $\mu_f$ est concentrée sur $\Omega_f$ (INT, IV, §4, n$^o7$, déf. 4). Soit $\nu_f$ la mesure sur $\Omega_f$ de densité $\mathscr{F}(f)^{-1}$ par rapport à $\mu_f|\Omega_f$.

Les ensembles $\Omega_f$, pour $f\in A(G)$, forment un recouvrement ouvert de $\widehat{G}$ (cor. 2). Pour tous $f$ et $g$ dans A(G), la formule (18) démontre que $\nu_f|(\Omega_f\cap \Omega_g) =\nu_g|(\Omega_f\cap \Omega_g)$. Par suite, il existe une unique mesure $\nu$ sur $\widehat{G}$ telle que l’on ait $\nu_f=\nu |\Omega_f$ pour tout $f\in A(G)$ (INT, III, §2, n$^o1$, prop. 1).

Si $f\in A(G)$, les mesures $\mu_f$ et $\mathscr{F}(f)\cdot \nu$ sont concentrées sur $\Omega_f$, et leurs restrictions à $\Omega_f$ sont égales à $\mathscr{F}(f)\cdot \nu_f$; ces mesures sont donc égales.

Puisque $\mu_f$ est une mesure bornée, la transformée de Fourier $\mathscr{F}(f)$ appartient à l’espace $L^1(\widehat{G}, \nu )$. Comme, de plus, $\mathscr{F}(f)$ appartient à $\mathscr{C}_0(\widehat{G})$, on a aussi $\mathscr{F}(f)\in L^2(\widehat{G}, \nu )$.

La formule (17) s’écrit maintenant, pour $\varphi \in$ Stell(G) et $f\in A(G)$ : (20) $(\varphi *f)(e) =\int_{\widehat{G}}\mathscr{F}(\varphi )\mathscr{F}(f)d\nu$.

En particulier, pour $f$ et $g$ dans A(G), on a

$$
\int_{\widehat{G}}\mathscr{F}(f)\mathscr{F}(g)d\nu = (f*g)(e) =\int_Gf(x)g(x^{-1})dx \tag{21}
$$

#### Proposition 9 {#ts-ii-s1-prop-9 .statement tag=02IE}

La mesure $\nu$ caractérisée par le lemme 4 est une mesure de Haar sur $\widehat{G}$.

Soit $\chi \in \widehat{G}$. Pour $f$ et $g$ dans A(G), appliquons la formule (21) à $\chi  f$ et $\chi  g$. Le membre de droite est inchangé, d’où

$$
\nu (\mathscr{F}(f)\mathscr{F}(g)) =\nu (\mathscr{F}(\chi  f)\mathscr{F}(\chi  g))
$$

D’après les formules (12) de II, p. 208 et (13) de II, p. 208, il vient

$$
\nu (\mathscr{F}(f)\mathscr{F}(g)) =\nu (\varepsilon_{\chi}*(\mathscr{F}(f)\mathscr{F}(g)))
$$

On déduit alors de INT, VIII, §4, n$^o3$, prop. 7 que

$$
\nu (\mathscr{F}(f)\mathscr{F}(g)) = (\varepsilon_{\chi^{-1}}*\nu )(\mathscr{F}(f)\mathscr{F}(g))
$$

c’est-à-dire

$$
(\mathscr{F}(f)\cdot \nu )(\mathscr{F}(g)) = (\mathscr{F}(f)\cdot (\varepsilon_{\chi^{-1}}*\nu ))(\mathscr{F}(g))
$$

Comme l’espace $\widehat{A}(G)$ est dense dans $\mathscr{C}_0(\widehat{G})$ (cor. 1), il en résulte l’égalité

$$
\mathscr{F}(f)\cdot \nu =\mathscr{F}(f)\cdot (\varepsilon_{\chi^{-1}}*\nu )
$$

Les mesures $\nu$ et $\varepsilon_{\chi^{-1}}*\nu$ coïncident donc sur l’ouvert $\Omega_f$ où $\mathscr{F}(f)$ est non nulle. D’après le corollaire 2 et INT, III, §2, n$^o1$, cor. de la prop. 1, ces mesures sont donc égales.

Ceci montre que la mesure $\nu$ est proportionnelle à une mesure de Haar sur $\widehat{G}$. Soit $f\in A(G)$. Prenons $g=\widetilde{f}$ dans la formule (21). Elle s’écrit alors

$$
\int_{\widehat{G}}|\mathscr{F}(f)|^2d\nu =\int_G|f|^2dx \tag{22}
$$

ce qui démontre que la mesure $\nu$ n’est pas nulle. La mesure $\nu$ est donc une mesure de Haar sur $\widehat{G}$.

#### Définition 4 {#ts-ii-s1-def-4 .statement tag=02IF}

La mesure de Haar $\nu$ sur $\widehat{G}$ de la proposition 9 est dite mesure duale de la mesure de Haar $dx$ donnée sur G.

Nous noterons souvent $d\chi$ ou $d\widehat{x}$ la mesure de Haar sur $\widehat{G}$ qui est duale de la mesure de Haar $dx$.

#### Remarque {#ts-ii-s1-n3-rem-3 .statement tag=02IG}

Soit $a$ un nombre réel $>0$. Si l’on remplace $dx$ par la mesure $a\cdot dx$, le produit de convolution des fonctions $f$ et $g\in L^1(G)$ est remplacé par $a(f*g)$. Nous avons vu (II, p. 209, remarque) que $\mathscr{F}(f)$ est remplacée par $a\mathscr{F}(f)$. Donc $\mu_f$ est inchangée et $\nu$ est remplacée par $a^{-1}\cdot \nu$. En particulier, la mesure $dx\otimes d\widehat{x}$ sur $G\times \widehat{G}$ est indépendante du choix de la mesure de Haar sur G.

#### Lemme 5 {#ts-ii-s1-lem-5 .statement tag=02IH}

L’espace $A(\widehat{G})$ est dense dans $L^2(\widehat{G})$.

Soit $h$ un élément de $L^2(\widehat{G})$ orthogonal à $\widehat{A}(G)$. Pour $f$ et $g$ dans A(G), on a $\mathscr{F}(f)\cdot \mathscr{F}(g) =\mathscr{F}(f*g)\in \widehat{A}(G)$, donc $h\cdot \mathscr{F}(f)$ est orthogonal à $\mathscr{F}(g)$. Ainsi, pour tout $f\in A(G)$, la fonction $h\cdot \mathscr{F}(f)$ est orthogonale à $\widehat{A}(G)$. Mais $h\cdot \mathscr{F}(f)\in L^1(\widehat{G})$, et $\widehat{A}(G)$ est dense dans $\mathscr{C}_0(\widehat{G})$, donc la mesure $h\mathscr{F}(f)\cdot \nu$ est nulle, c’est-à-dire que $h\mathscr{F}(f)$ est $\nu$-localement négligeable (INT, V, §5, n$^o3$, cor. 2 de la prop. 3). En particulier, $h$ est $\nu$-localement négligeable sur l’ensemble $\Omega_f$ des caractères $\chi$ tels que $\mathscr{F}(f)(\chi )\not= 0$. D’après le corollaire 2, on en déduit que $h$ est $\nu$-localement négligeable, donc nulle puisque $h$ appartient à $L^2(\widehat{G})$. Cela conclut la preuve.

#### Théorème 1 (Plancherel) {#ts-ii-s1-thm-1 .statement tag=02II}

La restriction de la transformation de Fourier au sous-espace A(G) de $L^2(G)$ se prolonge de manière unique en une isométrie Φ de $L^2(G)$ sur $L^2(\widehat{G})$.

De plus, si $f\in L^1(G)\cap L^2(G)$, sa transformée de Fourier appartient à $L^2(\widehat{G})$ et coïncide dans $L^2(\widehat{G})$ avec $\Phi (f)$.

D’après la formule (22), la restriction de $\mathscr{F}$ à A(G) est une isométrie du sous-espace A(G) de $L^2(G)$ sur le sous-espace $\widehat{A}(G)$ de $L^2(\widehat{G})$. Comme A(G) est dense dans $L^2(G)$ (cor. 1 de II, p. 212), la transformation de Fourier se prolonge de manière unique en une isométrie Φ de $L^2(G)$ sur un sous-espace fermé de $L^2(\widehat{G})$. Mais puisque son image contient $\widehat{A}(G)$, qui est dense dans $L^2(\widehat{G})$ (lemme 5), l’application Φ est surjective.

Soit maintenant $f\in L^1(G)\cap L^2(G)$; démontrons que sa transformée de Fourier appartient à $L^2(\widehat{G})$. D’après la prop. 8, (iv) de II, p. 211, et le fait que A(G) est un idéal de $L^1(G)$, il existe une base de filtre $\mathfrak{B}$ sur A(G) qui converge vers $f$ à la fois dans $L^1(G)$ et dans $L^2(G)$. On a alors

$\Phi (f) =$ lim$_{g,\mathfrak{B}}\Phi (g) =$ lim$_{g,\mathfrak{B}}\mathscr{F}(g)$ dans $L^2(\widehat{G})$ et $\mathscr{F}(f) =$ lim$_{g,\mathfrak{B}}\mathscr{F}(g)$ dans $\mathscr{C}_0(\widehat{G})$. Il existe donc une

suite $(g_n)$ dans A(G) telle que $\mathscr{F}(g_n)$ converge vers $\Phi (f)$ dans $L^2(\widehat{G})$ et vers $\mathscr{F}(f)$ dans $\mathscr{C}_0(\widehat{G})$. D’après INT, IV, §3, n$^o4$, th. 3 et cor. 1, on a $\mathscr{F}(f) = \Phi (f)$, et en particulier $\mathscr{F}(f)\in L^2(\widehat{G})$. Ceci achève de prouver le théorème.

On note encore $\mathscr{F}$ l’isométrie de $L^2(G)$ sur $L^2(\widehat{G})$ définie dans le théorème 1, et on l’appelle la transformation de Fourier dans $L^2(G)$. De même, la cotransformation de Fourier admet un unique prolongement isométrique à $L^2(G)$, encore appelé cotransformation de Fourier et noté $\mathscr{F}$.

#### Corollaire {#ts-ii-s1-n3-cor-1 .statement tag=02IJ}

Supposons que G est compact et que $dx$ est la mesure de Haar normalisée sur G. Alors la famille des caractères unitaires de G est une base orthonormale de $L^2(G)$.

Puisque G est compact, les caractères de G appartiennent à $L^2(G)$. Pour $\chi$ et $\xi$ dans $\widehat{G}$, on a

$$
\int_G\langle \chi , x\rangle \langle \xi , x\rangle dx=\mathscr{F}_G(dx)(\chi \xi^{-1})
$$

donc la famille des caractères de G est orthonormale (prop. 6 de II, p. 210). Elle est de plus totale car le produit scalaire de $\chi \in \widehat{G}$ et de $f\in L^2(G)$ est égal à $\mathscr{F}_G(f)(\chi )$, et donc $f$ est orthogonale à $\widehat{G}$ si et seulement si $\mathscr{F}_G(f)$ est nulle dans $L^2(\widehat{G})$, si et seulement si $f$ est nulle (th. 1).

#### Remarque 1 {#ts-ii-s1-n3-rem-1 .statement tag=02IK}

Certaines des formules concernant la transformation de Fourier sur $L^1(G)$ s’étendent à la transformation de Fourier sur $L^2(G)$. En particulier, pour $f\in L^2(G)$ et $\chi \in \widehat{G}$, on a

$$
\mathscr{F}(f) = (\chi \mapsto \mathscr{F}(f)(\chi^{-1})) =\mathscr{F}(f)
$$

$$
\mathscr{F}(\varepsilon_x*f) =\eta (x^{-1})\mathscr{F}(f),\mathscr{F}(\varepsilon_x*f) =\eta (x)\mathscr{F}(f)
$$

$$
\mathscr{F}(\chi  f) =\varepsilon_{\chi}*\mathscr{F}(f),\mathscr{F}(\chi  f) =\varepsilon_{\chi}*\mathscr{F}(f)
$$

Si $\sigma$ est un automorphisme de G et Δ le module de $\sigma$ (INT, VII, §1, n$^o4$, déf. 4), alors pour $f\in L^2(G)$, on a

$$
\mathscr{F}(f\circ \sigma ) = \Delta^{-1}\mathscr{F}(f)\circ \widehat{\sigma}^{-1}
$$

dans $L^2(G)$.

#### Remarque 2 {#ts-ii-s1-n3-rem-2 .statement tag=02IL}

Les formules

$$
\|\mathscr{F}(f)\|^2=\|f\|^2 \tag{23}
$$

pour $f\in L^2(G)$, ou bien

$$
\int_Gf(x)g(x)dx=\int_{\widehat{G}}\mathscr{F}(f)(\chi )\mathscr{F}(g)(\chi )d\chi \tag{24}
$$

pour $f$ et $g$ dans $L^2(G)$, sont appelées « formules de Plancherel ».

#### Proposition 10 {#ts-ii-s1-prop-10 .statement tag=02IM}

Soit $n\geqslant 0$ un entier et soient $G_1,\cdots ,G_n$ des groupes commutatifs localement compacts. Soient $\mu_j$, pour $1\leqslant j\leqslant n$, des mesures de Haar sur $G_j$. Soit G le groupe produit des groupes $G_j$ pour $1\leqslant j\leqslant n$. Soit $\beta$ l’isomorphisme de $\widehat{G}$ sur $\prod\widehat{G}_j$ de la prop. 2 de II, p. 206. La mesure de Haar sur $\widehat{G}$ duale de la mesure de Haar produit $\mu=\mu_1\otimes  \cdots  \otimes \mu_n$ sur G s’identifie au produit des mesures de Haar $\widehat{\mu}_j$.

En effet, pour toute famille $(f_j)$ d’éléments non nuls de $\mathscr{L}^2(G_j)$, la fonction $f$ sur G définie par $(x_j)\mapsto \prod f_j(x_j)$ appartient à $\mathscr{L}^2(G)$, et vérifie

$$
\int_G|f|^2d\mu=\prod_j\int_{G_j}|f_j|^2d\mu_j=\prod_j\int_{\widehat{G}_j}|\mathscr{F}_{G_j}(f)|^2d\widehat{\mu}_j
$$

d’après la formule de Plancherel, ce qui démontre que la mesure de Haar produit des $\widehat{\mu}_j$ s’identifie à la mesure de Haar duale de $\mu$.

### 4. La formule d’inversion de Fourier

Rappelons que tout élément $f$ de A(G) est la classe d’une unique fonction continue (prop. 7, b) de II, p. 210). Pour $x\in G$, on notera $f(x)$ la valeur de cette fonction en $x$.

#### Proposition 11 {#ts-ii-s1-prop-11 .statement tag=02IN}

Soit $f\in A(G)$. Alors $\mathscr{F}(f)\in L^1(\widehat{G})$ et, pour tout $x\in G$, on a

$$
f(x) =\int_{\widehat{G}}\langle \widehat{x}, x\rangle \mathscr{F}(f)(\widehat{x})d\widehat{x} \tag{25}
$$

Autrement dit, pour $f\in A(G)$, on a

$$
f=\mathscr{F}_{\widehat{G}}(\mathscr{F}_G(f))\circ \eta \tag{26}
$$

où $\eta$ désigne l’application canonique de G dans le groupe bidual $\widehat{\widehat{G}}$.

D’après le lemme 4 de II, p. 213 et la proposition 9 de II, p. 214, on a $\mathscr{F}(f)\in L^1(\widehat{G})$ pour toute fonction $f\in A(G)$. D’après la formule de Plancherel (24), pour $f$ et $g$ dans $L^2(G)$, on a

$$
(f*\widetilde{g})(e) =\int_{\widehat{G}}\mathscr{F}(f)(\chi )\mathscr{F}(g)(\chi )d\widehat{x}(\chi ) \tag{27}
$$

Soient $f$ et $g$ dans $L^1(G)\cap L^2(G)$ et $h=f*\widetilde{g}\in A(G)$. Puisque la transformation de Fourier est un morphisme involutif, la formule (27) est l’assertion (25) pour la fonction $h$ au point $x=e$. Par linéarité, on en déduit que la formule (25) est valide au point $x=e$ pour toute fonction $h\in A(G)$.

Soient $x\in G$ et $h\in A(G)$. Soit $h_1=\varepsilon_{x^{-1}}*h$. Alors $h_1\in A(G)$ et $h_1(e) =h(x)$. Comme de plus $\mathscr{F}(h_1)(\chi ) =\langle \chi , x\rangle \mathscr{F}(f)(\chi )$ pour tout $\chi \in \widehat{G}($cf. formule (11) de II, p. 208), la formule (25) pour la fonction $h_1$ au point $e$ implique la formule (25) pour $h$ au point $x$.

#### Lemme 6 {#ts-ii-s1-lem-6 .statement tag=02IO}

Soit $\varphi \in L^1(\widehat{G})\cap L^2(\widehat{G})$. Alors $f=\mathscr{F}_{\widehat{G}}(\varphi )\circ \eta$ appartient à $L^2(G)$ et $\mathscr{F}_G(f) =\varphi$ dans $L^2(\widehat{G})$.

La fonction $f$ est continue et bornée sur G car $\varphi \in L^1(\widehat{G})$. Pour toute fonction $g\in L^1(G)\cap L^2(G)$, on a

$$
\int_Gg(x)f(x)dx=\int_Gg(x)\int_{\widehat{G}}\langle \chi , x\rangle \varphi (\chi )d\widehat{x}(\chi )dx
$$

$$
=\int_{\widehat{G}}\mathscr{F}_G(g)(\chi )\varphi (\chi )d\widehat{x}(\chi ) \tag{28}
$$

en appliquant le théorème de Lebesgue-Fubini (INT, V, §8, n$^o4$, th. 1, a)) à la fonction $(x, \chi )\mapsto g(x)\varphi (\chi )\langle \chi , x\rangle$ qui est intégrable sur $G\times \widehat{G}$ par rapport à la mesure produit $dx\otimes d\widehat{x}$. On en déduit que

$$
\int_Gg(x)f(x)dx\leqslant \|\mathscr{F}_G(g)\|_2\|\varphi \|_2=\|g\|_2\|\varphi \|_2
$$

d’après la formule de Plancherel. La forme linéaire $g\mapsto \int_Gf g$ est donc continue sur $L^1(G)\cap L^2(G)$, et comme $L^1(G)\cap L^2(G)$ est dense dans l’espace hilbertien $L^2(G)$, on en déduit que $f$ appartient à $L^2(G)$.

En appliquant alors le th. 1 de II, p. 215, on obtient d’autre part

$$
\int_Gg(x)f(x)dx=\int_{\widehat{G}}\mathscr{F}_G(g)(\chi )\mathscr{F}_G(f)(\chi )d\widehat{x}(\chi )
$$

$$
=\int_{\widehat{G}}\mathscr{F}_G(g)(\chi )\mathscr{F}_G(f)(\chi )d\widehat{x}(\chi )
$$

pour tout $g\in L^2(G)$. Comparant avec (28), on conclut que $\varphi =\mathscr{F}_G(f)$ dans $L^2(\widehat{G})$, puisque A(G) est contenu dans $L^1(G)\cap L^2(G)$ et que $\widehat{A}(G)$ est dense dans $L^2(\widehat{G})$ (lemme 5 de II, p. 215).

Proposition 12 (Formule d’inversion de Fourier)

Soit $f\in L^2(G)$ telle que $\mathscr{F}_G(f)\in L^1(\widehat{G})$. Alors on a $f$ = $\mathscr{F}_G(\mathscr{F}_G(f))\circ \eta$ dans $L^2(G)$. Autrement dit, pour presque tout $x\in G$, on a

$$
f(x) =\int_{\widehat{G}}\langle \widehat{x}, x\rangle \mathscr{F}_G(f)(\widehat{x})d\widehat{x}
$$

La fonction $\varphi =\mathscr{F}_G(f)$ appartient à $L^1(\widehat{G})\cap L^2(\widehat{G})$, et on obtient la formule désirée en appliquant le lemme.

#### Corollaire 1 {#ts-ii-s1-lem-6-cor-1 .statement tag=02IP}

Pour tout sous-ensemble fermé P de $\widehat{G}$ et tout $\chi \in \widehat{G}$ n’appartenant pas à P, il existe une fonction $f\in L^1(G)$ telle que $\mathscr{F}(f)$ soit nulle sur P et non nulle en $\chi$.

Comme, d’après (12), on a $\mathscr{F}(\chi f) =\varepsilon_{\chi}*\mathscr{F}(f)$ pour tout $\chi \in \widehat{G}$, il suffit de considérer le cas où $\chi$ est l’élément neutre de $\widehat{G}$.

Soit U un voisinage compact symétrique de $e\in \widehat{G}$ tel que $U^2\cap P =\emptyset$. Soit $\varphi$ une fonction continue positive sur $\widehat{G}$, nulle en dehors de U et telle que $\varphi (e) = 1$. La fonction $\varphi_1=\varphi *\varphi$ est alors nulle sur P et $\varphi_1(e)>0$. Il suffit donc de démontrer que $\varphi_1$ appartient à l’image de la transformation de Fourier sur $L^1(G)$. Or $\varphi$ et $\varphi_1$ appartiennent à $L^1(\widehat{G})\cap L^2(\widehat{G})$. Posons $f=\mathscr{F}(\varphi )\circ \eta$ et $f_1=\mathscr{F}(\varphi_1)\circ \eta$. Le lemme 6 implique que $f$ et $f_1$ appartiennent à $L^2(G)$ et vérifient $\varphi =\mathscr{F}(f)$ et $\varphi_1=\mathscr{F}(f_1)$. De plus

$$
f_1=\mathscr{F}(\varphi *\varphi )\circ \eta = (\mathscr{F}(\varphi )\circ \eta )^2=f^2
$$

et donc $f_1\in L^1(G)$. Ainsi $\varphi_1=\mathscr{F}(f_1)$ est bien dans l’image de $L^1(G)$ par la transformation de Fourier.

#### Corollaire 2 {#ts-ii-s1-lem-6-cor-2 .statement tag=02IQ}

L’algèbre de Banach $L^1(G)$ est régulière (I, p. 89, déf. 1).

D’après la prop. 1 de I, p. 88 et l’identification de la transformation de Gelfand de $L^1(G)$ et de la cotransformation de Fourier de G, cela découle du corollaire précédent.

### 5. Le théorème de dualité de Pontryagin

#### Théorème 2 (Pontryagin) {#ts-ii-s1-thm-2 .statement tag=02IR}

L’application canonique $\eta$ de G dans $\widehat{\widehat{G}}$ est un isomorphisme de groupes topologiques. Il transforme la mesure de Haar $dx$ en la mesure de Haar biduale $d\widehat{\widehat{x}}$.

Démontrons d’abord que $\eta$ est injective et stricte. Il suffit pour cela de montrer que pour tout voisinage U de $e$ dans G, il existe un voisinage W de $e$ dans $\widehat{\widehat{G}}$ tel que $^-\eta^1(W)\subset U$ (lemme 2 de II, p. 200). Or soit V un voisinage compact symétrique de $e$ dans G tel que $V^2\subset U$, soit $f$ une fonction continue positive sur G, à support contenu dans V, et telle que $f(e)>0$. Soit $g=\widetilde{f}*f$. Alors $g$ appartient à A(G), son support est contenu dans U et $g(e)>0$. De plus, $\mathscr{F}_G(g)\in L^1(\widehat{G})$ d’après la prop. 11 de II, p. 217. L’ensemble W des $\xi$ dans $\widehat{\widehat{G}}$ tels que

$$
\mathscr{F}_G(\mathscr{F}_G(g))(\xi )-\mathscr{F}_G(\mathscr{F}_G(g))(e)<1g(e)
$$

2

est un voisinage de $e$ dans $\widehat{\widehat{G}}$ puisque la fonction $\mathscr{F}_{\widehat{G}}(\mathscr{F}_G(g))$ est continue sur $\widehat{\widehat{G}}$. Soit $x\in^-\eta^1(W)$. D’après la formule (26), on a

$$
\mathscr{F}_{\widehat{G}}(\mathscr{F}_G(g))(\eta (x)) =g(x)
$$

et donc $|g(x)-g(e)|<^1_2g(e)$. Cela implique $g(x)\not= 0$ et donc $x\in U$, puisque le support de $g$ est contenu dans U. Ainsi $^-\eta^1(W)\subset U$.

Démontrons que l’application $\eta$ est surjective. Comme cette application est un homéomorphisme sur son image, le groupe $\eta (G)$ est un sous-groupe localement compact de $\widehat{\widehat{G}}$. Il est donc fermé dans $\widehat{\widehat{G}}$ (TG, III, p. 22, cor. 2). Raisonnons par l’absurde et supposons qu’il existe un caractère $\xi \in \widehat{\widehat{G}}$ tel que $\xi \notin \eta (G)$. Il existe alors (corollaire 1 de II, p. 219) un élément $f$ non nul de $L^1(\widehat{G})$ tel que $\mathscr{F}_{\widehat{G}}(f)$ soit nulle sur $\eta (G)$. Soit $g\in L^1(G)$. La fonction $(x, \chi )\mapsto g(x)f(\chi )\langle \chi , x\rangle$ appartient à $L^1(G\times \widehat{G})$. D’après le th. de Lebesgue-Fubini (INT, V, §8, n$^o4$, th. 1, a)), il vient donc

$$
\int_{\widehat{G}}f(\chi )\mathscr{F}_G(g)(\chi )d\chi =\int_Gg(x)\int_{\widehat{G}}f(\chi )\langle \chi , x\rangle d\chi dx
$$

$$
=\int_Gg(x)\mathscr{F}_{\widehat{G}}(f)(\eta (x))dx= 0
$$

Puisque l’image de la transformation de Fourier est dense dans $\mathscr{C}_0(\widehat{G})$ (cor. de la prop 5 de II, p. 209), il en résulte que la mesure $f\cdot d\chi$ est nulle. Cela contredit le fait que $f\not= 0$ dans $L^1(\widehat{G})$, et démontre que $\eta$ est surjective.

La mesure image $\eta (dx)$ et la mesure $\nu$ duale de la mesure $d\chi$ sont des mesures de Haar sur $\widehat{\widehat{G}}$. Soit $f$ un élément non nul de A(G) ; en particulier $f\in L^2(G)$. D’après la prop. 12 de II, p. 219$,\mathscr{F}_G(f)\in L^1(\widehat{G})$ et l’on a

$\int$ 2 $\int\int$ 2

$\mathscr{F}_G(\mathscr{F}_G(f))\eta (dx) =|f|^2dx=\mathscr{F}_G(\mathscr{F}_G(f))d\nu$,

$\widehat{\widehat{G}}$ G $\widehat{\widehat{G}}$

où la deuxième égalité suit de deux applications de la formule de Plancherel, donc la mesure de Haar duale de $d\chi$ est la mesure $\eta (dx)$.

Nous identifierons dorénavant G et $\widehat{\widehat{G}}$ par l’isomorphisme $\eta$. On a alors :

#### Corollaire {#ts-ii-s1-n5-cor-1 .statement tag=02IS}

La cotransformation de Fourier de $L^2(\widehat{G})$ sur $L^2(G)$ et la transformation de Fourier de $L^2(G)$ sur $L^2(\widehat{G})$ sont des isométries réciproques l’une de l’autre.

#### Remarque {#ts-ii-s1-n5-rem-1 .statement tag=02IT}

Soient $f\in L^2(G)$ et $g\in L^2(\widehat{G})$. En appliquant la formule de Plancherel (24) à $f$ et $\mathscr{F}_{\widehat{G}}(g)$, on obtient la formule

$$
\int_Gf(x)\mathscr{F}_{\widehat{G}}(g)(x)dx=\int_{\widehat{G}}\mathscr{F}_G(f)(\chi )g(\chi )d\widehat{x}(\chi ) \tag{29}
$$

puisque l’on a $\mathscr{F}_G(\mathscr{F}_{\widehat{G}}(g)) =\mathscr{F}_G(\mathscr{F}_{\widehat{G}}(g)) =g$.

La transformation et la cotransformation de Fourier définies sur $\mathscr{M}^1(\widehat{G})$ sont à valeurs dans l’espace des fonctions continues bornées sur G. Pour $\beta \in \mathscr{M}^1(\widehat{G})$ et $x\in G$, on a

$$
\mathscr{F}_{\widehat{G}}(\beta )(x) =\int_{\widehat{G}}\langle \chi , x\rangle d\beta (\chi ),\mathscr{F}_{\widehat{G}}(\beta )(x) =\int_{\widehat{G}}\langle \chi , x\rangle d\beta (\chi )
$$

Les transformations de Fourier de G et $\widehat{G}$ sont également transposées l’une de l’autre. Plus précisément :

#### Proposition 13 {#ts-ii-s1-prop-13 .statement tag=02IU}

Soient $\alpha \in \mathscr{M}^1(G)$ et $\beta \in \mathscr{M}^1(\widehat{G})$. On a alors (30) $\mathscr{F}_G(\mathscr{F}_{\widehat{G}}(\beta )\cdot \alpha ) =\beta *\mathscr{F}_G(\alpha )$

et en particulier

$$
\int_G\mathscr{F}_{\widehat{G}}(\beta )(x)d\alpha (x) =\int_{\widehat{G}}\mathscr{F}_G(\alpha )(\chi )d\beta (\chi ) \tag{31}
$$

La formule (30) implique la formule (31) en évaluant les deux côtés de l’identité en $\chi = 1$. Démontrons (30). Soit $\chi \in \widehat{G}$. Il vient

$$
(\mathscr{F}_G(\mathscr{F}_{\widehat{G}}(\beta )\cdot \alpha ))(\chi ) =\int_G\langle \chi , x\rangle \mathscr{F}_{\widehat{G}}(\beta )(x)d\alpha (x)
$$

$$
=\int_G\langle \chi , x\rangle \int_{\widehat{G}}\langle \xi , x\rangle d\beta (\xi )d\alpha (x)
$$

La fonction $(x, \xi )\mapsto  \langle \chi , x\rangle \langle \xi , x\rangle$ est continue et bornée, donc intégrable sur $G\times \widehat{G}$ par rapport à la mesure $\alpha \otimes \beta$. D’après le théorème de Lebesgue-Fubini (INT, V, §8, n$^o4$, th. 1, a)), on obtient

$$
(\mathscr{F}_G(\mathscr{F}_{\widehat{G}}(\beta )\cdot \alpha ))(\chi ) =\int_{\widehat{G}}\int_G\langle \chi \xi^{-1}, x\rangle d\alpha (x)d\beta (\xi )
$$

$$
=\int_{\widehat{G}}\mathscr{F}_G(\alpha )(\chi \xi^{-1})d\beta (\xi ) = (\beta *\mathscr{F}_G(\alpha ))(\chi )
$$

comme désiré.

#### Corollaire {#ts-ii-s1-n5-cor-2 .statement tag=02IV}

La transformation de Fourier $\mathscr{F}_G$ est injective sur $\mathscr{M}^1(G)$.

En effet, si $\alpha \in \mathscr{M}^1(G)$ vérifie $\mathscr{F}_G(\alpha ) = 0$, on déduit de (31) que $\alpha (\mathscr{F}_G(f)) = 0$ pour toute $f\in L^1(\widehat{G})$ ; comme l’image de $L^1(\widehat{G})$ par la tran$\widehat{s}$formation de Fourier est dense dans $\mathscr{C}_0(G)$ (cor. de la prop. 5 de II, p. 209), on a donc $\alpha = 0$.

Il existe des espaces fonctionnels sur G et $\widehat{G}$, autres que $L^2(G)$ et $L^2(\widehat{G})$, sur lesquels $\mathscr{F}$ et $\mathscr{F}$ sont des isomorphismes inverses l’un de l’autre. Le théorème suivant en donne un exemple. On note B(G) le sous-espace vectoriel de $L^1(G)$ formé des éléments $f\in L^1(G)$ tels que $\mathscr{F}_G(f)\in L^1(\widehat{G})$. C’est une sous-algèbre de $L^1(G)$. En effet, soient $f$ et $g$ dans B(G). On a $f*g\in L^1(G)$ et $\mathscr{F}_G(f*g) =\mathscr{F}_G(f)\mathscr{F}_G(g)\in L^1(\widehat{G})$, puisque $\mathscr{F}_G(f)\in L^1(\widehat{G})$ et $\mathscr{F}_G(g)\in \mathscr{C}_0(\widehat{G})$.

#### Théorème 3 {#ts-ii-s1-thm-3 .statement tag=02IW}

La restriction de la transformation de Fourier à B(G) induit un isomorphisme d’espaces vectoriels de B(G) sur $B(\widehat{G})$, dont la réciproque est induite par la restriction à $B(\widehat{G})$ de la cotransformation de Fourier.

Soit $f\in B(G)$. Notons $g=\mathscr{F}_G(f)$. On a $g\in L^1(\widehat{G})\cap \mathscr{C}_0(\widehat{G})\subset$ $L^1(\widehat{G})\cap L^2(\widehat{G})$. Posons $f_1=\mathscr{F}_{\widehat{G}}(g)\in L^2(G)$. Pour toute fonction continue à support compact $h\in \mathscr{K}(\widehat{G})$, on a $h\in L^1(\widehat{G})\cap L^2(\widehat{G})$ et

$$
\int_Gf_1(x)\mathscr{F}_{\widehat{G}}(h)(x)dx=\int_G\mathscr{F}_{\widehat{G}}(g)(x)\mathscr{F}_{\widehat{G}}(h)(x)dx
$$

$$
=\int_{\widehat{G}}g(\chi )h(\chi )d\widehat{x}(\chi )
$$

$$
=\int_{\widehat{G}}\mathscr{F}_G(f)(\chi )h(\chi )d\widehat{x}(\chi ) =\int_Gf(x)\mathscr{F}_{\widehat{G}}(h)(x)dx
$$

en utilisant le théorème de Plancherel et la formule (31). Puisque $\mathscr{K}(\widehat{G})$ est dense dans $L^2(\widehat{G})$, son image par la transformation de Fourier est dense dans $L^2(G)$. Par conséquent, on a $f_1=f$ dans $L^1(G)$ ; cela démontre que $g\in B(\widehat{G})$.

La formule $f_1=f$ signifie que la restriction à B(G) de la composition $\mathscr{F}_{\widehat{G}}\circ \mathscr{F}_G$ est l’application identique de B(G). En échangeant les rôles de G et $\widehat{G}$, on constate que $\mathscr{F}_G\circ \mathscr{F}_{\widehat{G}}$ est l’application identique de $B(\widehat{G})$, ce qui achève la preuve du théorème.

#### Corollaire 1 {#ts-ii-s1-thm-3-cor-1 .statement tag=02IX}

Soit $f\in L^1(G)$. Alors $f\in B(G)$ si et seulement si $f$ appartient à l’image de la transformation de Fourier $\mathscr{F}_{\widehat{G}}$ sur $L^1(\widehat{G})$. En particulier, on a $A(G)\subset B(G)$.

Le théorème 3 prouve que si $f\in B(G)$, alors $f=\mathscr{F}_{\widehat{G}}(\mathscr{F}_G(f))$, où $\mathscr{F}_G(f)$ appartient à $L^1(\widehat{G})$. Réciproquement, si $f=\mathscr{F}_{\widehat{G}}(g)$, où $g\in L^1(\widehat{G})$, alors on a $g\in B(\widehat{G})$ et donc $f\in B(G)$ d’après le théorème. La dernière assertion résulte alors de la prop. 11 de II, p. 217.

#### Corollaire 2 {#ts-ii-s1-thm-3-cor-2 .statement tag=02IY}

L’espace vectoriel B(G) est une algèbre à la fois pour la multiplication et pour la convolution. La transformation de Fourier échange convolution et multiplication dans B(G) et $B(\widehat{G})$.

On a déjà vu que B(G) est une sous-algèbre de $L^1(G)$. D’autre part, si $f$ et $g$ appartiennent à B(G), alors $f g\in L^1(G)$ puisque $f\in L^1(G)$ et $g$ appartient à l’image de la transformation de Fourier sur $L^1(\widehat{G})$ (corollaire 1). Comme il existe $f_1$ et $g_1$ dans $L^1(\widehat{G})$ telles que $f$ = $\mathscr{F}_{\widehat{G}}(f_1)$ et $g=\mathscr{F}_{\widehat{G}}(g_1)$ (loc. cit.), on a $f g=\mathscr{F}_{\widehat{G}}(f_1*g_1)$, et donc $f g\in B(G)$ de nouveau par le corollaire précédent.

#### Proposition 14 {#ts-ii-s1-prop-14 .statement tag=02IZ}

Soient $f$ et $g$ dans $L^2(G)$. Alors $\mathscr{F}_G(f g) =$ $\mathscr{F}_G(f)*\mathscr{F}_G(g)$.

L’égalité est vraie si $f$ et $g$ appartiennent à B(G) (corollaire 2), et en particulier si $f$ et $g$ appartiennent à A(G) puisque $A(G)\subset B(G)$ (cor. 1). Comme A(G) est dense dans $L^2(G)$ (cor. 1 de II, p. 212), il suffit de démontrer que les deux membres de l’égalité sont des fonctions continues de $(f, g)\in L^2(G)\times L^2(G)$ à valeurs dans $\mathscr{C}_0(\widehat{G})$. Or l’application $(f, g)\mapsto \mathscr{F}_G(f g)$ s’obtient en composant l’application continue $(f, g)\mapsto f g$ de $L^2(G)\times L^2(G)$ dans $L^1(G)$ et la transformation de Fourier $\mathscr{F}_G$ de $L^1(G)$ dans $\mathscr{C}_0(\widehat{G})$, qui est également continue. De même, l’application $(f, g)\mapsto \mathscr{F}_G(f)*\mathscr{F}_G(g)$ s’obtient en composant les applications continues $(f, g)\mapsto (\mathscr{F}_G(f),\mathscr{F}_G(g))$ de $L^2(G)\times L^2(G)$ dans $L^2(\widehat{G})\times L^2(\widehat{G})$ et $(h_1, h_2)\mapsto h_1*h_2$ de $L^2(\widehat{G})\times L^2(\widehat{G})$ dans $\mathscr{C}_0(\widehat{G})$ (INT, VIII, §4, n$^o5$, prop. 15).

#### Remarque {#ts-ii-s1-n5-rem-2 .statement tag=02J0}

Voir le n$^o9$ et les exercices 22 de II, p. 270 et 31 de II, p. 275 pour d’autres exemples d’espaces fonctionnels sur lesquels la transformation de Fourier est un isomorphisme, dans le cas de groupes G particuliers.

### 6. Propriétés fonctorielles de la dualité

Soient G et H des groupes localement compacts commutatifs. Rappelons que si $\varphi : G\rightarrow H$ est un morphisme de groupes topologiques, le morphisme dual $\widehat{\varphi}:\widehat{H}\rightarrow \widehat{G}$ est défini par $\langle \chi , \varphi (x)\rangle =\langle \widehat{\varphi}(\chi ), x\rangle$ quels que soient $\chi \in \widehat{H}$ et $x\in G$. Cette définition montre que $\widehat{\widehat{\varphi}}=\varphi$ avec les identifications de G (resp. H) et $\widehat{\widehat{G}}$ (resp. $\widehat{\widehat{H}})$ du théorème 2 de II, p. 220.

Soit $\theta$ une application de $G\times H$ dans $\mathbf{U}$. Pour tout $x\in G$ (resp. tout $y\in H$), soit $\theta_x$ (resp. $\theta^y)$ la fonction de G dans $\mathbf{U}$ définie par $y\mapsto$ $\theta (x, y)$ (resp. la fonction de H dans $\mathbf{U}$ définie par $x\mapsto \theta (x, y)$). Supposons que l’application $\alpha :x\mapsto \theta_x$ soit un isomorphisme du groupe topologique G sur le groupe topologique $\widehat{H}$. Pour tout $y\in H$ et $x\in G$, on a

$$
\theta^y(x) =\theta (x, y) =\langle \alpha (x), y\rangle =\langle x,\widehat{\alpha}(y)\rangle
$$

c’est-à-dire $\theta^y=\widehat{\alpha}(y)$. D’après le th. 2 de II, p. 220, l’application $\beta :y\mapsto \theta^y$ est donc un isomorphisme du groupe topologique H sur le groupe topologique $\widehat{G}$. Dans ces conditions, nous dirons que $\theta$ met G et H en dualité, ou que G et H sont en dualité relativement à $\theta$. Nous identifierons alors chacun des groupes G et H au dual de l’autre. On appellera mesure duale de la mesure de Haar $dx$ la mesure de Haar sur H obtenue par transport de structure à partir de la mesure duale de $dx$.

#### Lemme 7 {#ts-ii-s1-lem-7 .statement tag=02J1}

Soient $(G_i)_{i\in I}$ et $(H_i)_{i\in I}$ des familles finies de groupes topologiques localement compacts. Pour $i\in I$, soit $\theta_i: G_i\times H_i\rightarrow \mathbf{U}$ une application qui met les groupes $G_i$ et $H_i$ en dualité. L’application $\theta$ définie par

$$
\theta ((g_i),(h_i)) =\prod_{i\in I}\theta_i(g_i, h_i)
$$

met les groupes $\prod G_i$ et $\prod H_i$ en dualité.

Cela résulte de la prop. 2 de II, p. 206 et de la définition qui précède.

#### Définition 5 {#ts-ii-s1-def-5 .statement tag=02J2}

Soient G, H et K des groupes topologiques. Soient $f: H\rightarrow G$ et $g: G\rightarrow K$ des morphismes de groupes topologiques. On dit que le couple $(f, g)$ est une suite exacte de groupes topologiques, si c’est une suite exacte de groupes (A, II, p. 10, remarque 5) et si $f$ et $g$ sont des morphismes stricts.

On représentera une suite exacte par le diagramme

$$
H\longrightarrow^fG\longrightarrow^gK
$$

et on dira qu’un diagramme

$$
G_1\longrightarrow^{f_1}G_2\longrightarrow^{f_2}G_3\rightarrow  \cdots  \rightarrow G_n\longrightarrow^{f_n}G_{n+1}
$$

est exact si chaque couple $(f_i, f_{i+1})$ pour $1\leqslant i\leqslant n-1$ est exact.

Une suite

$$
1\rightarrow H\longrightarrow^fG\longrightarrow^gK\rightarrow 1
$$

est exacte si et seulement si $f$ est un morphisme injectif strict, $g$ est un morphisme surjectif strict, et le noyau de $g$ est égal à l’image de $f$. Si K est séparé, l’image de $f$ est un sous-groupe fermé de G.

#### Exemple 1 {#ts-ii-s1-n6-exa-1 .statement tag=02J3}

Soit $f: H\rightarrow$ G un morphisme injectif strict dont l’image est un sous-groupe distingué. La suite

$$
1\rightarrow H\longrightarrow^fG\longrightarrow^pG/f(H)\rightarrow 1
$$

où $p$ est la projection canonique, est exacte. En particulier, si H est un sous-groupe fermé et distingué de G, la suite de groupes topologiques

$$
1\rightarrow H\longrightarrow^jG\longrightarrow^pG/H\rightarrow 1
$$

où $j$ est l’inclusion et $p$ la projection canonique, est exacte.

#### Exemple 2 {#ts-ii-s1-n6-exa-2 .statement tag=02J4}

Soit $g: G\rightarrow K$ un morphisme surjectif strict. La suite

$1\rightarrow$ Ker($g$)$\longrightarrow^jG\longrightarrow^gK\rightarrow 1$,

où $j$ est l’inclusion, est exacte

#### Théorème 4 {#ts-ii-s1-thm-4 .statement tag=02J5}

Une suite

$H\longrightarrow^fG\longrightarrow^g$ K

de groupes topologiques localement compacts commutatifs est exacte si, et seulement si, la suite duale

$$
\widehat{K}\widehat{\longrightarrow}^g\widehat{G}\widehat{\longrightarrow}^f\widehat{H}
$$

est exacte.

Nous commencerons par démontrer quelques lemmes. On notera que chacun d’entre eux est par ailleurs une conséquence facile de l’assertion du th. 4.

#### Lemme 8 {#ts-ii-s1-lem-8 .statement tag=02J6}

Soit $g: G\rightarrow K$ un morphisme de groupes topologiques localement compacts commutatifs. Si le morphisme $g$ est surjectif et strict, alors $\widehat{g}$ est injectif et strict.

Puisque $g$ est surjectif, le morphisme $\widehat{g}$ est injectif (lemme 2 de II, p. 205). Pour démontrer que $\widehat{g}$ est un morphisme strict, il suffit de démontrer que pour tout voisinage U de $e$ dans $\widehat{K}$, il existe un voisinage V de $e$ dans $\widehat{G}$ tel que $^-\widehat{g}^1(V)\subset U$ (lemme 2 de II, p. 200). Soit U un tel voisinage de $e$ dans $\widehat{K}$. Par définition de la topologie de $\widehat{K}$, il existe une partie compacte X de K et un nombre $\varepsilon  >0$ tels que U contienne l’ensemble des $\widehat{z}\in \widehat{K}$ qui, pour tout $z\in X$, vérifient $|\langle \widehat{z}, z\rangle  -1|< \varepsilon$. Puisque $g$ est strict et surjectif, il existe, d’après TG, I, p. 80, prop. 10, une partie compacte $X_0$ de G telle que $g(X_0) = X$. Soit V le voisinage de $e$ dans $\widehat{G}$ formé des éléments $\chi \in \widehat{G}$ tels que,

pour tout $x\in X_0$, on ait $|\langle \chi , x\rangle  -1|< \varepsilon$. On a alors $^-\widehat{g}^1(V)\subset U$. Cela démontre l’assertion.

#### Lemme 9 {#ts-ii-s1-lem-9 .statement tag=02J7}

Soit $f: H\rightarrow G$ un morphisme de groupes topologiques localement compacts. Si le morphisme $f$ est injectif et strict, alors $\widehat{f}$ est surjectif et strict.

Supposons que $f$ est injectif et strict. Le morphisme $\widehat{f}$ induit par passage au quotient un morphisme $q:\widehat{G}/$ Ker($\widehat{f}$)$\rightarrow \widehat{H}$. Il s’agit de démontrer que c’est un isomorphisme de groupes topologiques ; par dualité, il suffit pour cela de démontrer que son dual $\widehat{q}$ est un isomorphisme.

Notons L le groupe dual de $\widehat{G}/$ Ker($\widehat{f}$) et $p:\widehat{G}\rightarrow \widehat{G}/$ Ker($\widehat{f}$) la projection canonique. Nous allons d’abord démontrer que $\widehat{p}$ induit, par passage aux sous-espaces, un isomorphisme de L sur $f(H)$.

On a $q\circ p=\widehat{f}$, d’où $\widehat{p}\circ \widehat{q}=f$. L’image de $\widehat{p}$ contient donc $f(H)$.

Comme $f$ est strict, son image $f(H)$ est un sous-groupe localement compact de G, et est donc fermé (TG, III, p. 22, cor. 2). Soit K = $G/f(H)$ et considérons la suite exacte

$$
1\rightarrow H\longrightarrow^fG\longrightarrow^gK\rightarrow 1
$$

associée (exemple 1). Par dualité, le morphisme $\widehat{f}\circ \widehat{g}$ est trivial et donc l’image de $\widehat{g}$ est contenue dans Ker($\widehat{f}$) $=$ Ker($p$). Ainsi $p\circ \widehat{g}$ est le morphisme trivial et, à nouveau par dualité, $g\circ \widehat{p}$ est aussi trivial. Il en résulte que l’image de $\widehat{p}$ est contenue dans le noyau de $g$, qui est égal à $f(H)$. On conclut que l’image de $\widehat{p}$ est égale à $f(H)$.

Par ailleurs, puisque $p$ est un morphisme surjectif et strict, le morphisme dual $\widehat{p}$ est un morphisme injectif strict de L dans G (lemme 8). Il en résulte que $\widehat{p}$ induit un isomorphisme de groupes topologiques de L sur $f(H)$. Puisque $\widehat{p}\circ \widehat{q}=f$, et que $f$ induit un isomorphisme de H sur son image $f(H)$, le morphisme $\widehat{q}$ est un isomorphisme.

#### Lemme 10 {#ts-ii-s1-lem-10 .statement tag=02J8}

Soit

$H\longrightarrow^fG\longrightarrow^g$ K

une suite exacte de groupes localement compacts commutatifs. Le noyau de $\widehat{f}$ est égal à l’image de $\widehat{g}$.

L’homomorphisme $\widehat{f}\circ \widehat{g}$ est trivial par dualité, donc l’image de $\widehat{g}$ est contenue dans le noyau de $\widehat{f}$. Réciproquement, soit $\chi$ dans le noyau de $\widehat{f}$. Cela signifie que Im($f$) $=$ Ker($g$) est contenu dans le noyau de $\chi$, donc qu’il existe un caractère $\eta$ de Im($g$) tel que $\eta \circ g=\chi$. Puisque l’inclusion de Im($g$) dans K est stricte, l’application duale de restriction des caractères de K à Im($g$) est surjective (lemme 9). Il existe donc un caractère $\beta$ de K tel que $\eta$ est la restriction de $\beta$, et il vient $\chi =\beta \circ g=\widehat{g}(\beta )$. On en conclut que le noyau de $\widehat{f}$ est contenu dans l’image de $\widehat{g}$.

Démontrons maintenant le théorème 4. Il suffit par dualité de démontrer que la suite $\widehat{K}\widehat{\longrightarrow}^g\widehat{G}\widehat{\longrightarrow}^f\widehat{H}$ est exacte lorsque la suite $H\longrightarrow^fG\longrightarrow^g$ K l’est. Or, d’après les lemmes 8 et 9, les morphismes $\widehat{f}$ et $\widehat{g}$ sont stricts et d’après le lemme 10, le noyau de $\widehat{f}$ est égal à l’image de $\widehat{g}$.

#### Corollaire 1 {#ts-ii-s1-lem-10-cor-1 .statement tag=02J9}

Soit

$$
1\rightarrow H\longrightarrow^fG\longrightarrow^gK\rightarrow 1
$$

une suite exacte de groupes topologiques localement compacts commutatifs. Le morphisme $\widehat{g}$ induit un isomorphisme entre $\widehat{K}$ et $f(H)^{\bot}$, et $\widehat{f}$ induit par passage au quotient un isomorphisme entre $\widehat{G}/f(H)^{\bot}$ et $\widehat{H}$.

D’après le théorème 4, la suite

$$
1\rightarrow \widehat{K}\widehat{\longrightarrow}^g\widehat{G}\widehat{\longrightarrow}^f\widehat{H}\rightarrow 1 \tag{32}
$$

est exacte. Le morphisme $\widehat{g}$ induit donc un isomorphisme de $\widehat{K}$ sur Ker($\widehat{f}$) $=f(H)^{\bot}$ (lemme 2 de II, p. 205), et $\widehat{f}$ induit par passage au quotient un isomorphisme de $\widehat{G}/Ker(\widehat{f}) =\widehat{G}/f(H)^{\bot}$ sur $\widehat{H}($loc. cit.).

#### Corollaire 2 {#ts-ii-s1-lem-10-cor-2 .statement tag=02JA}

Soit $f: G\rightarrow H$ un morphisme de groupes topologiques localement compacts commutatifs. Le morphisme $f$ est strict si et seulement si $\widehat{f}$ est strict.

D’après la décomposition canonique (E, II, p. 44) d’un morphisme strict, cela résulte des lemmes 8 et 9.

#### Corollaire 3 {#ts-ii-s1-lem-10-cor-3 .statement tag=02JB}

Soit H un sous-groupe de G. On a $(H^{\bot})^{\bot}= H$.

Puisque $H^{\bot}= H^{\bot}$, on peut supposer que H est fermé. Soit $f: H\rightarrow G$ l’injection canonique et $p: G\rightarrow G/H$ la projection canonique. On a $H^{\bot}=$ Ker($\widehat{f}$) (lemme 10). Soit $k$ l’injection canonique de $H^{\bot}$ dans $\widehat{G}$. D’après le théorème 4, le morphisme $\widehat{p}$ induit un isomorphisme $\widehat{p}_H:\widehat{G}/H\rightarrow H^{\bot}$ de groupes topologiques et on a $k\circ \widehat{p}_H=\widehat{p}$. Par conséquent (corollaire 1), il vient

$(H^{\bot})^{\bot}=$ Ker($\widehat{k}$) $=$ Ker( $\widehat{\widehat{p}}_H\circ \widehat{k}) =$ Ker($p$) $= H$.

#### Corollaire 4 {#ts-ii-s1-lem-10-cor-4 .statement tag=02JC}

Soit I un ensemble et soit $(H_i)_{i\in I}$ une famille de sous-groupes fermés de G. L’orthogonal du sous-groupe fermé engendré par les $H_i$ est $\bigcap_{i\in I}H^{\bot}_i$. L’orthogonal de $\bigcap_iH_i$ est le sous-groupe fermé engendré par les sous-groupes $H^{\bot}_i$.

La première assertion découle de la définition de l’orthogonal. En appliquant ce résultat et le cor. 3 à la famille de sous-groupes fermés $(H^{\bot}_i)_{i\in I}$ de $\widehat{G}$, on voit que $\bigcap_iH_i$ est l’orthogonal du sous-groupe fermé engendré par les sous-groupes $H^{\bot}_i$, et la seconde assertion est alors obtenue par dualité.

#### Corollaire 5 {#ts-ii-s1-lem-10-cor-5 .statement tag=02JD}

Soit $\varphi : G\rightarrow H$ un morphisme de groupes localement compacts commutatifs. Alors le sous-groupe Im($\varphi$ ) de H et le sous-groupe Ker($\widehat{\varphi}$) de $\widehat{H}$ sont l’orthogonal l’un de l’autre. En particulier, pour que $\widehat{\varphi}$ soit injectif, il faut et il suffit que l’image de $\varphi$ soit dense dans H.

On a Ker($\widehat{\varphi}$) $=\varphi (G)^{\bot}$ (lemme 2 de II, p. 205), d’où le résultat d’après le cor. 3.

#### Corollaire 6 {#ts-ii-s1-lem-10-cor-6 .statement tag=02JE}

Soit $k\in \mathbf{Z}$. Alors le noyau de l’homomorphisme $x\mapsto x^k$ de G dans G et l’adhérence de l’image du morphisme $\chi \mapsto \chi^k$ de $\widehat{G}$ dans $\widehat{G}$ sont l’orthogonal l’un de l’autre.

Cela résulte du corollaire précédent puisque les morphismes $x\mapsto x^k$ de G dans G et $\chi \mapsto \chi^k$ de $\widehat{G}$ dans $\widehat{G}$ sont duaux l’un de l’autre.

Rappelons (A, X, p. 17) qu’un groupe commutatif A est divisible si, pour tout $n\in \mathbf{Z}$ non nul, l’application $a\mapsto a^n$ de A dans A est surjective.

#### Corollaire 7 {#ts-ii-s1-lem-10-cor-7 .statement tag=02JF}

Soit G un groupe localement compact commutatif.

a) Si G est divisible, alors le groupe dual $\widehat{G}$ est sans torsion ;

b) Si le groupe dual $\widehat{G}$ est sans torsion, et si $k\in \mathbf{Z}$ est non nul, alors l’image de l’homomorphisme $x\mapsto x^k$ de G dans G est dense dans G ;

c) Supposons G discret ou compact. Pour que G soit divisible il faut et il suffit que $\widehat{G}$ soit sans torsion.

Les assertions a) et b) résultent du cor. 6. Si G est discret ou compact, l’image du morphisme $x\mapsto x^k$ de G dans G est fermée, et c) résulte de a) et b).

#### Remarque {#ts-ii-s1-n6-rem-1 .statement tag=02JG}

Il existe des groupes localement compacts commutatifs G qui ne sont pas divisibles et tels que $\widehat{G}$ est sans torsion (exercice 63 de II, p. 299).

### 7. La formule de Poisson

Dans ce numéro, on considère un sous-groupe fermé H de G. On note $\beta =dx$ la mesure de Haar sur G et $\widehat{\beta}$ la mesure de Haar duale sur $\widehat{G}$. On note $\alpha$ une mesure de Haar sur H et $\widehat{\alpha}$ la mesure de Haar duale sur le groupe dual $\widehat{H}$, que l’on identifie à $\widehat{G}/H^{\bot}$ (théorème 4 de II, p. 226). On identifie aussi $\widehat{G}/H$ à $H^{\bot}$ par l’application duale de la projection canonique $G\rightarrow G/H$ (loc. cit.).

On désignera par $\dot{x}$ l’image canonique d’un élément $x$ de G dans $G/H$ et par $\dot{\chi}$ l’image canonique d’un élément $\chi$ de $\widehat{G}$ dans $\widehat{G}/H^{\bot}$.

On note $\gamma$ la mesure de Haar $\beta /\alpha$ sur $G/H$ (INT, VII, §2, n$^o2$, déf. 1 et n$^o7$, prop. 10), et $\widehat{\gamma}$ la mesure de Haar duale sur $H^{\bot}$. Rappelons (INT, VII, §2, n$^o3$, prop. 5, c)) que la mesure $\gamma$ est caractérisée par la propriété suivante : pour toute $f\in \mathscr{L}^1(G)$, la fonction $y\mapsto f(xy)$ sur H est $\alpha$-intégrable pour $\beta$-presque tout $x\in G$ ; son intégrale ne dépend que de $\dot{x}$ et la fonction définie $\gamma$-presque partout sur $G/H$ par

$$
f^{\flat}: \dot{x}\mapsto \int_Hf(xh)d\alpha (h)
$$

appartient à $L^1(G/H, \gamma )$ et vérifie

$$
\int_{G/H}f^{\flat}d\gamma =\int_Gf d\beta \tag{33}
$$

#### Proposition 15 {#ts-ii-s1-prop-15 .statement tag=02JH}

Soit $f\in L^1(G)$ telle que la restriction à $H^{\bot}$ de la fonction continue $\mathscr{F}_G(f)$ est intégrable relativement à $\widehat{\gamma}$. Alors, pour presque tout $x\in G$, la fonction $y\mapsto f(xy)$ sur H est $\alpha$-intégrable, et l’on a :

$$
\int_Hf(xy)d\alpha (y) =\int_{H^{\bot}}\langle \chi , x\rangle \mathscr{F}_G(f)(\chi )d\widehat{\gamma}(\chi )
$$

D’après ce qui précède, la fonction $f^{\flat}$ définie presque partout sur $G/H$ par

$$
f^{\flat}( \dot{x}) =\int_Hf(xy)d\alpha (y)
$$

appartient à $L^1(G/H)$. La transformée de Fourier de $f^{\flat}$ s’identifie à la fonction sur $H^{\bot}=\widehat{G}/H$ donnée pour $\chi \in H^{\bot}$ par

$$
\mathscr{F}_{G/H}(f^{\flat})(\chi ) =\int_{G/H}\langle \chi ,\dot{x}\rangle f^{\flat}( \dot{x})d\gamma ( \dot{x})
$$

$$
=\int_G\langle \chi , x\rangle f(x)d\beta (x) =\mathscr{F}_G(f)(\chi )
$$

d’après la formule (33), appliquée à la fonction intégrable $x\mapsto$ $\langle \chi , x\rangle f(x)$. Par hypothèse, la fonction $\mathscr{F}(f)|H^{\bot}=\mathscr{F}_{G/H}(f^{\flat})$ appartient à $L^1(H^{\bot})$, et donc la fonction $f^{\flat}$ appartient à l’espace $B(G/H)$. Il en résulte (th. 3 de II, p. 222) que $f^{\flat}$ coïncide presque partout avec $\mathscr{F}_{\widehat{G}/H}(\mathscr{F}_{G/H}(f^{\flat}))$. Pour presque tout $\dot{x}\in G/H$, on a donc

$$
f^{\flat}( \dot{x}) =\int_{H^{\bot}}\langle \chi , x\rangle \mathscr{F}_{G/H}(f^{\flat})(\chi )d\widehat{\gamma}(\chi ) =\int_{H^{\bot}}\langle \chi , x\rangle \mathscr{F}_G(f)(\chi )d\widehat{\gamma}(\chi )
$$

Cela conclut la preuve.

#### Corollaire (Formule de Poisson) {#ts-ii-s1-n7-cor-1 .statement tag=02JI}

Soit $f\in \mathscr{L}^1(G)$. On suppose que les conditions suivantes sont vérifiées :

(i) La restriction de $\mathscr{F}_G(f)$ à $H^{\bot}$ est intégrable ;

(ii) Pour tout $x\in G$, la fonction $y\mapsto f(xy)$ sur H est intégrable ;

(iii) L’application $x\mapsto \int_Hf(xy)d\alpha (y)$ est continue sur G.

Alors on a

$$
\int_Hf(y)d\alpha (y) =\int_{H^{\bot}}\mathscr{F}_G(f)(\chi )d\widehat{\gamma}(\chi ) \tag{34}
$$

En effet, reprenant les notations de la preuve de la proposition précédente, les fonctions $f^{\flat}$ et $\mathscr{F}_{\widehat{G}/H}(\mathscr{F}_{G/H}(f^{\flat}))$ sur $G/H$ sont continues et égales presque partout. Elle sont donc égales partout et en particulier en $e$, ce qui donne la formule (34).

#### Proposition 16 {#ts-ii-s1-prop-16 .statement tag=02JJ}

La mesure $\widehat{\alpha}$ sur $\widehat{H} =\widehat{G}/H^{\bot}$ est égale à $\widehat{\beta /}\widehat{\gamma}$.

Fixons $f\in \mathscr{K}(G)$ non nulle. Pour $x\in G$ et $\chi \in \widehat{G}$, posons

$$
\varphi (x, \chi ) =\int_Hf(xy)\langle \chi , y\rangle d\alpha (y)
$$

La fonction $\varphi$ est continue sur $G\times \widehat{G}$ (INT, IV, §4, n$^o3$, cor. 1 du th. 2). Pour $x$ fixé, $\varphi (x, \chi )$ ne dépend que de la classe de $\chi$ dans $\widehat{G}/H^{\bot}=\widehat{H}$. Pour $\chi$ fixé, $\langle \chi , x\rangle \varphi (x, \chi )$ ne dépend que de la classe de $x$ dans $G/H$, et la fonction $\dot{x}\mapsto  \langle \chi , x\rangle \varphi (x, \chi )$ sur $G/H$ est à support compact.

Soit $x\in G$. La fonction $\dot{\chi}\mapsto \varphi (x, \chi )$ sur $\widehat{H}$ est la cotransformée de Fourier de la fonction $y\mapsto f(xy)$ sur H. Celle-ci est de carré intégrable, donc d’après la formule de Plancherel (23) de II, p. 217, on a

$$
\int_{\widehat{G}/H^{\bot}}|\varphi (x, \chi )|^2d\widehat{\alpha}( \dot{\chi}) =\int_H|f(xy)|^2d\alpha (y) \tag{35}
$$

Soit $\chi \in \widehat{G}$. La fonction $\dot{x}\mapsto  \langle \chi , x\rangle \varphi (x, \chi )$ appartient à $\mathscr{K}(G/H)$, donc à $L^1(G/H)$. Sa cotransformée de Fourier est la fonction sur $H^{\bot}$ dont la valeur en $\xi \in H^{\bot}$ est

$$
\int_{G/H}\langle \xi ,\dot{x}\rangle \langle \chi , x\rangle \varphi (x, \chi )d\gamma ( \dot{x}) =\int_{G/H}\int_H\langle \chi \xi , xy\rangle f(xy)d\alpha (y)d\gamma ( \dot{x})
$$

$$
=\int_G\langle \chi \xi , x\rangle f(x)d\beta (x) =\mathscr{F}_G(f)(\chi \xi )
$$

d’après la formule (33). Donc

$$
\int_{G/H}|\varphi (x, \chi )|^2d\gamma ( \dot{x}) =\int_{H^{\bot}}|\mathscr{F}_G(f)(\chi \xi )|^2d\widehat{\gamma}(\xi ) \tag{36}
$$

par la formule de Plancherel de nouveau.

On calcule alors finalement

$\int_{\widehat{G}}|\mathscr{F}_G(f)|^2d\widehat{\beta}=\int_G|f|^2d\beta$ (par (23))

$=\int_{G/H}d\gamma ( \dot{x})\int_H|f(xy)|^2d\alpha (y)$ (par (33))

$=\int_{G/H}d\gamma ( \dot{x})\int_{\widehat{G}/H^{\bot}}|\varphi (x, \chi )|^2d\widehat{\alpha}( \dot{\chi})$ (par (35))

$$
=\int_{\widehat{G}/H^{\bot}}d\widehat{\alpha}( \dot{\chi})\int_{G/H}|\varphi (x, \chi )|^2d\gamma ( \dot{x})
$$

$=\int_{\widehat{G}/H^{\bot}}d\widehat{\alpha}( \dot{\chi})\int_{H^{\bot}}|\mathscr{F}_G(f)(\chi \xi )|^2d\widehat{\gamma}(\xi )$ (par (36)$)$,

où on a appliqué INT, V, §8, n$^o3$, prop. 5 à la fonction continue positive $( \dot{x},\dot{\chi})\mapsto  |\varphi (x, \chi )|^2$ sur $G/H\times \widehat{G}/H^{\bot}$.

En comparant cette égalité avec la formule d’intégration (33) pour le groupe $\widehat{G}$, on conclut alors que les mesures de Haar $\widehat{\alpha}$ et $\widehat{\beta /}\widehat{\gamma}$ coïncident.

### 8. Exemples de dualité

#### Proposition 17 {#ts-ii-s1-prop-17 .statement tag=02JK}

Soit $n\geqslant 1$ un entier. Notons $\boldsymbol{\mu}_n$ le groupe des racines $n$-ièmes de l’unité dans $\mathbf{C}$. Les groupes $\mathbf{Z}/n\mathbf{Z}$ et $\boldsymbol{\mu}_n$ sont en dualité relativement à l’application induite par passage au quotient de l’application $\mathbf{Z}\times \boldsymbol{\mu}_n\rightarrow \mathbf{U}$ définie par $(m, z)\mapsto z^m$.

Le groupe $\mathbf{Z}\widehat{/n}\mathbf{Z}$ coïncide avec l’ensemble des homomorphismes $\chi$ de $\mathbf{Z}/n\mathbf{Z}$ dans $\mathbf{U}$. Ceux-ci sont de la forme $m\mapsto \chi (1)^m$ où $\chi (1)$ est un élément quelconque de $\mathbf{U}$ tel que $\chi (1)^n= 1$, d’où le résultat.

#### Corollaire 1 {#ts-ii-s1-prop-17-cor-1 .statement tag=02JL}

Soit G un groupe fini commutatif. Le groupe dual $\widehat{G}$ est isomorphe à G.

Le groupe G est isomorphe à un produit fini de groupes cycliques (A, VII, p. 22, th. 3), et son groupe dual est isomorphe au produit des groupes duaux de ceux-ci (prop. 2 de II, p. 206). On est donc ramené au cas où G est cyclique, qui relève de la proposition 17 puisque le groupe $\boldsymbol{\mu}_n$ est cyclique d’ordre $n$ (A, V, p. 75, th. 1).

#### Corollaire 2 {#ts-ii-s1-prop-17-cor-2 .statement tag=02JM}

Soit G un groupe localement compact commutatif. Le groupe G est fini si et seulement si $\widehat{G}$ est fini. Un sous-groupe fermé H de G est d’indice fini si et seulement si son orthogonal est fini.

Par dualité, la première assertion découle du fait que le dual d’un groupe fini est fini (corollaire 1). La seconde en résulte, puisque $\widehat{G}/H$ s’identifie à $H^{\bot}$ (th. 4 de II, p. 226).

#### Proposition 18 {#ts-ii-s1-prop-18 .statement tag=02JN}

Pour que $\widehat{G}$ soit compact, il faut et il suffit que G soit discret. Si G est discret, la mesure duale de la mesure de comptage sur G est la mesure de Haar normalisée sur $\widehat{G}$. Si G est compact, la mesure duale de la mesure de Haar normalisée est la mesure de comptage sur $\widehat{G}$.

Supposons G discret, et soit $\alpha$ la mesure de comptage sur G. Soit $\varphi$ la fonction caractéristique de $e\in G$. On a $\mathscr{F}_G(\varphi ) = 1$ sur $\widehat{G}$. Comme $\mathscr{F}_G(\varphi )$ tend vers 0 à l’infini, le groupe $\widehat{G}$ est compact.

En outre, pour la mesure duale $\widehat{\alpha}$ de $\alpha$, la fonction $\mathscr{F}_G(\varphi )$ doit être d’intégrale $\varphi (e) = 1$ (prop. 12 de II, p. 219). Donc $\widehat{\alpha}(\widehat{G}) = 1$.

Supposons G compact. Alors la mesure de Haar $dx$ appartient à $\mathscr{M}^1(G)$. Sa transformée de Fourier est strictement positive en $\chi =e$ et nulle pour $\chi \not= 0$ (prop. 6 de II, p. 210). Puisque elle est continue sur $\widehat{G}$, le groupe $\widehat{G}$ est discret. Si la mesure de G est 1, on déduit par dualité du cas précédent que la mesure duale de la mesure $dx$ est la mesure de comptage sur $\widehat{G}$.

#### Corollaire 1 (Relations d’orthogonalité) {#ts-ii-s1-prop-18-cor-1 .statement tag=02JO}

Supposons G discret et muni de la mesure de comptage. Pour $x$ et $y$ dans G, on a

$\int$ 0 si $x\not=y$

$$
\chi (x)\chi (y)d\chi =
$$

$_{\widehat{G}}$ 1 si $x=y$.

Cela résulte du cor. du théo. 1 de II, p. 215 et de la dualité.

#### Corollaire 2 {#ts-ii-s1-prop-18-cor-2 .statement tag=02JP}

Soit H un sous-groupe fermé de G.

a) Pour que H soit compact, il faut et il suffit que $H^{\bot}$ soit ouvert dans $\widehat{G}$ ;

b) Pour que H soit ouvert, il faut et il suffit que $H^{\bot}$ soit compact dans $\widehat{G}$.

a) Dire que $H^{\bot}$ est ouvert revient à dire que $\widehat{G}/H^{\bot}$ est discret, or $\widehat{G}/H^{\bot}$ est isomorphe à $\widehat{H}$ (th. 4 de II, p. 226) ; l’assertion découle donc de la prop. 18. L’assertion b) résulte par dualité de l’assertion a) appliquée à $H^{\bot}$.

#### Corollaire 3 {#ts-ii-s1-prop-18-cor-3 .statement tag=02JQ}

Soit $(H_i)_{i\in I}$ une famille filtrante décroissante de sous-groupes compacts de G. Pour que G s’identifie à la limite projective des groupes $G/H_i$, il faut et il suffit que $\widehat{G}$ soit réunion des sous-groupes ouverts $H^{\bot}_i$.

Dire que G s’identifie à la limite projective des $G/H_i$ revient à dire que $\bigcap_iH_i=\{e\}$ (TG, III, p. 60, prop. 2), c’est-à-dire que $\bigcup_iH^{\bot}_i$ est dense dans $\widehat{G}$ (cor. 4 du th. 4 de II, p. 226). Or $\bigcup_iH^{\bot}_i$ est un sous-groupe ouvert, donc fermé, de $\widehat{G}$.

#### Corollaire 4 {#ts-ii-s1-prop-18-cor-4 .statement tag=02JR}

Soit I un ensemble et soit $(H_i)_{i\in I}$ une famille de groupes compacts. Le dual du groupe produit des $H_i$ est le groupe discret somme directe des groupes $\widehat{H}_i$.

C’est un cas particulier du cor. 3.

#### Proposition 19 {#ts-ii-s1-prop-19 .statement tag=02JS}

Soit K un corps localement compact non discret, non nécessairement commutatif, et soit G le groupe additif de K, dont la loi de groupe est notée additivement. Soit $\chi$ un caractère unitaire de G distinct de 1. Pour $x, y\in G$, posons $\theta (x, y) =\chi (xy)$. Alors G est en dualité avec lui-même relativement à $\theta$.

Pour $y\in G$, soit $\chi_y$ l’application de G dans $\mathbf{U}$ telle que $\chi_y(x) =$ $\chi (xy)$. On a $\chi_y\in \widehat{G}$, et il faut démontrer que $\beta :y\mapsto \chi_y$ est un isomorphisme de groupes topologiques de G dans $\widehat{G}$.

L’application $\beta$ est un homomorphisme injectif de G dans $\widehat{G}$; elle est continue (TG, X, p. 28, th. 3 appliqué à l’application continue $\theta$ de $G\times G$ dans $\mathbf{C})$. Démontrons que $\theta$ est un homéomorphisme sur son image. Il suffit (lemme 2 de II, p. 200) de démontrer que pour tout voisinage U de 0 dans K, il existe un voisinage V de $e$ dans $\widehat{G}$

$-1$

tel que $\beta (V)\subset U$. Soit $x\mapsto  |x|$ une valeur absolue sur K définissant la topologie de K (AC, VI, §9, n$^o1$, prop. 1), et soit $x_0\in K$ tel que $\chi (x_0)\not= 1$ ; notons $\eta =|\chi (x_0)-1|>0$. Soit U un voisinage de 0 dans K. Il existe $\delta  >0$ tel que U contienne l’ensemble des $y\in K$ tels que $|y|< \delta$. Soit V l’ensemble des caractères $\xi \in \widehat{G}$ tels que $|\langle \xi , x\rangle  -1|< \eta$ pour tout élément $x\in K$ vérifiant $|x|\leqslant |x_0|/\delta$. C’est un voisinage de $e$ dans $\widehat{G}$. Si $y\not= 0$ est tel que $\beta (y)$ appartient à V, on a donc $|\chi (xy)-1|<|\chi (x_0)-1|$ pour tout $x$ tel que $|x|\leqslant |x_0|/\delta$. Par conséquent, on a $|x_0y^{-1}|>|x_0|/\delta$, et donc $|y|< \delta$, de sorte que $y\in U$.

Puisque $\beta$ est un homéomorphisme sur son image, celle-ci est fermée dans $\widehat{G}$ (TG, III, p. 22, cor. 2). Mais par ailleurs l’orthogonal de l’image de $\beta$ est l’ensemble des éléments $x$ de G tel que $\chi (xy) = 1$ pour tout $y\in G$, et est donc réduit à $\{0\}$. L’image de $\beta$ est donc dense dans $\widehat{G}$ (corollaire 3 de II, p. 228). On conclut que $\beta$ est surjective.

#### Corollaire 1 {#ts-ii-s1-prop-19-cor-1 .statement tag=02JT}

Soient K un corps localement compact non discret non nécessairement commutatif et $\chi$ un caractère unitaire non trivial du groupe additif de K. Soit E un espace vectoriel topologique de dimension finie sur K. L’application $\theta$ de $E\times E'$ dans $\mathbf{U}$ définie par $\theta (x, \lambda ) =\chi (\langle \lambda , x\rangle )$ pour $(\lambda , x)\in E'\times E$ met les groupes topologiques E et $E'$ en dualité.

Soient $n$ la dimension de E et $(e_1, . . . , e_n)$ une base de E. Elle permet d’identifier E et $K^n$ (EVT, I, p. 14, th. 2). Le résultat découle alors de la prop. 19 et de la prop. 2 de II, p. 206.

On note $\mathbf{T}$ le groupe $\mathbf{R}/\mathbf{Z}$.

#### Corollaire 2 {#ts-ii-s1-prop-19-cor-2 .statement tag=02JU}

a) Le groupe $\mathbf{R}$ est en dualité avec lui-même relativement à l’application $(x, y)\mapsto$ exp(2$i\pi xy)$, et la mesure duale de la mesure de Lebesgue est la mesure de Lebesgue ;

b) Les groupes $\mathbf{Z}$ et $\mathbf{T}$ sont en dualité relativement à l’application obtenue par passage au quotient à partir de l’application de $\mathbf{Z}\times \mathbf{R}$ dans $\mathbf{U}$ telle que $(n, x)\mapsto$ exp(2$i\pi nx)$. La mesure de Haar duale de la mesure de comptage sur $\mathbf{Z}$ est la mesure de Haar normalisée sur $\mathbf{R}/\mathbf{Z}$.

Le groupe $\mathbf{R}$ est en dualité avec lui-même relativement à l’application $(x, y)\mapsto$ exp(2$i\pi xy)$ d’après la prop. 19. Identifions $\widehat{\mathbf{R}}$ à $\mathbf{R}$. L’orthogonal de $\mathbf{Z}$ dans $\widehat{\mathbf{R}}=\mathbf{R}$ est alors $\mathbf{Z}$, et b) résulte du th. 4 de II, p. 226.

Soient $\alpha$ la mesure de comptage sur $\mathbf{Z}$ et $\gamma$ la mesure de Haar normalisée sur $\mathbf{T}$. Si $\beta$ désigne la mesure de Lebesgue sur $\mathbf{R}$, on a $\gamma =\beta /\alpha$, puisque ces deux mesures de Haar sur $\mathbf{R}/\mathbf{Z}$ sont de masse 1. La mesure de Haar $\widehat{\alpha}$ sur $\widehat{\mathbf{Z}}=\mathbf{T}$ est la mesure de Haar normalisée (prop. 18), et la mesure de Haar $\widehat{\gamma}$ est la mesure de comptage sur $\mathbf{Z}($loc. cit.). D’après la prop. 16 de II, p. 231, la mesure duale de $\beta$ est donc la mesure $\beta$.

#### Remarque {#ts-ii-s1-n8-rem-1 .statement tag=02JV}

On retrouve en particulier la détermination de $\mathsf{X}(L^1(\mathbf{Z}))$ faite à l’exemple 4 de I, p. 36.

Pour tout entier $n\geqslant 0$ et $(x, y)\in \mathbf{R}^n\times \mathbf{R}^n$, on note

$$
x\cdot y=\sum_{j=1}^nx_jy_j
$$

#### Corollaire 3 {#ts-ii-s1-prop-19-cor-3 .statement tag=02JW}

Soit $n\geqslant 1$ un entier. Le groupe $\mathbf{R}^n$ est en dualité avec lui-même relativement à l’application $(x, y)\mapsto$ exp(2$i\pi  x\cdot y)$ et la mesure duale de la mesure de Lebesgue sur $\mathbf{R}^n$ est la mesure de Lebesgue. Les groupes $\mathbf{Z}^n$ et $\mathbf{T}^n=\mathbf{R}^n/\mathbf{Z}^n$ sont en dualité relativement à l’application obtenue par passage au quotient à partir de l’application $(n, x)\mapsto$ exp(2$i\pi  x\cdot y)$, et la mesure de Haar duale de la mesure de comptage sur $\mathbf{Z}^n$ est la mesure de Haar normalisée sur $(\mathbf{R}/\mathbf{Z})^n$.

Ceci résulte du lemme 7 de II, p. 225, de la proposition 10 de II, p. 217 et du corollaire 2.

#### Remarque {#ts-ii-s1-n8-rem-2 .statement tag=02JX}

Étant donné un sous-groupe H de $\mathbf{R}^n$, il lui correspond donc son orthogonal $H^{\bot}$, un sous-groupe de $\widehat{\mathbf{R}}^n=\mathbf{R}^n$, qui n’est autre que le sous-groupe associé à H défini en TG, VII, p. 6, n$^o3$.

Dans la suite, on identifiera le dual de $\mathbf{R}^n$ (resp. de $\mathbf{T}^n)$ avec $\mathbf{R}^n$ (resp. avec $\mathbf{Z}^n)$ par la dualité du corollaire. En particulier, pour $f\in L^1(\mathbf{R}^n)$, sa transformée de Fourier s’identifie à la fonction de $\mathbf{R}^n$ dans $\mathbf{C}$ qui à $y\in \mathbf{R}^n$ associe

$\mathscr{F}(f)(y) =\int_{\mathbf{R}^n}f(x)$ exp($-2i\pi  x\cdot y$)$dx$.

#### Corollaire 4 {#ts-ii-s1-prop-19-cor-4 .statement tag=02JY}

Le groupe $\mathbf{R}^*$ est en dualité avec le groupe $\{-1,1\} \times \mathbf{R}$ par l’application $(x,(\sigma , t))\mapsto \sigma (x/|x|)|x|^{it}$. Le groupe $\mathbf{R}^*_+$ est en dualité avec $\mathbf{R}$ par l’application $(x, t)\mapsto x^{it}$.

En effet, l’application $x\mapsto (x/|x|$, log($|x|$)) est un isomorphisme de groupes topologiques de $\mathbf{R}^*$ sur $\{-1,1\} \times \mathbf{R}$. L’assertion résulte alors du lemme 7 de II, p. 225, du corollaire 2 et du fait que les caractères unitaires de $\{-1,1\}$ sont 1 et $x\mapsto x$.

Soit $p$ un nombre premier. Le corps $\mathbf{Q}_p$ des nombres $p$-adiques est le complété de $\mathbf{Q}$ pour la valuation $p$-adique (INT, VII, § 1, n$^o6$, exemple, et AC, VI, § 3, n$^o4$, exemple 4). Pour tout $x\in \mathbf{Q}_p$, il existe un unique entier $\nu \geqslant 0$ et un unique entier $q$ vérifiant $0\leqslant q < p^{\nu}$ tels que $qp^{-\nu}-x\in \mathbf{Z}_p$ (A, VII, p. 10, th. 2, appliqué à l’anneau principal $\mathbf{Z}_p$ et à l’ensemble $R_p$ des entiers $j$ tels que $0\leqslant j < p)$. On note $\lambda (x) =qp^{-\nu}$.

#### Proposition 20 {#ts-ii-s1-prop-20 .statement tag=02JZ}

L’application $x\mapsto$ exp(2$i\pi \lambda (x))$ est un caractère unitaire de $\mathbf{Q}_p$ dont le noyau est $\mathbf{Z}_p$.

Pour $x_1$ et $x_2$ dans $\mathbf{Q}_p$, on a par définition $\lambda (x_1+x_2)-\lambda (x_1)-\lambda (x_2)\in$ $\mathbf{Z}_p\cap \mathbf{Q}=\mathbf{Z}$. L’application $\lambda$ est de plus localement constante puisque $\lambda (x+y) =\lambda (x)$ si $y\in \mathbf{Z}_p$. Il en découle alors que $x\mapsto$ exp(2$i\pi \lambda (x))$ est un caractère unitaire de $\mathbf{Q}_p$. Comme $\lambda (x)\in \mathbf{Z}$ si et seulement si $x\in \mathbf{Z}_p$, le noyau de ce caractère est $\mathbf{Z}_p$.

On rappelle qu’on appelle mesure de Haar normalisée sur le groupe additif de $\mathbf{Q}_p$ l’unique mesure de Haar $\mu$ telle que $\mu(\mathbf{Z}_p) = 1$ (INT, VII, §1, n$^o6$, exemple).

#### Corollaire {#ts-ii-s1-n8-cor-1 .statement tag=02K0}

a) Le groupe $\mathbf{Q}_p$ est en dualité avec lui-même relativement à l’application $(x, y)\mapsto$ exp(2$i\pi \lambda (xy))$. La mesure de Haar normalisée sur $\mathbf{Q}_p$ est alors sa propre duale ;

b) Les groupes $\mathbf{Z}_p$ et $\mathbf{Q}_p/\mathbf{Z}_p$ sont en dualité relativement à l’application obtenue par passage au quotient à partir de l’application définie par $(z, x)\mapsto$ exp(2$i\pi \lambda (zx))$, et la mesure duale de la mesure de Haar normalisée sur $\mathbf{Z}_p$ est la mesure de comptage sur $\mathbf{Q}_p/\mathbf{Z}_p$.

La démonstration suit pas à pas celle du cor. 2 de la prop. 19.

### 9. Transformée de Fourier euclidienne et séries de Fourier

$*$ Soit $n\in \mathbf{N}$. On identifie $\mathbf{R}_n$ et son dual comme dans le cor. 3 de II, p. 236. La mesure duale de la mesure de Lebesgue est alors la mesure de Lebesgue. On munit $\mathbf{R}^n$ de la norme euclidienne. Pour tout multi-indice $\alpha \in \mathbf{N}^n$, et tout $x= (x_1, . . . , x_n)\in \mathbf{R}^n$, on notera $x^{\alpha}=x^{\alpha}_{1^1}\cdots x^{\alpha}_{n^n}$, et on note $X^{\alpha}$ la fonction $x\mapsto x^{\alpha}$ sur $\mathbf{R}^n$.

Soit $m\in \mathbf{R}^m$. Tout morphisme continu de groupes commutatifs de $\mathbf{R}^m$ dans $\mathbf{R}^n$ est une application linéaire $\sigma \in \mathscr{L}(\mathbf{R}^n,\mathbf{R}^m)$ (TG, VII, p. 11, prop. 1). Le morphisme dual $\widehat{\sigma}$ s’identifie à l’application linéaire $^t\sigma$.

La transformation de Fourier dans $\mathbf{R}^n$ prend une forme particulièrement pratique dans le cadre de l’espace des fonctions de Schwartz et de son dual (IV, à paraître). Nous en résumons ici les résultats principaux.

Soit $\mathscr{S}(\mathbf{R}^n)$ l’espace des fonctions indéfiniment dérivables $\varphi$ sur $\mathbf{R}^n$, à valeurs complexes, telles que, pour tout multi-indice $\alpha \in \mathbf{N}^n$ et tout entier $k\in \mathbf{N}$, la fonction

$$
x\mapsto  \|x\|^k\partial^{\alpha}\varphi (x)
$$

est bornée sur $\mathbf{R}^n$. On munit $\mathscr{S}(\mathbf{R}^n)$ de la topologie localement convexe définie par les semi-normes

$p_{k,\alpha}:\varphi \mapsto$ sup $\|x\|^k|\partial^{\alpha}\varphi (x)|$.

$x\in \mathbf{R}^n$

On dit que $\mathscr{S}(\mathbf{R}^n)$ est l’espace des fonctions de Schwartz sur $\mathbf{R}^n$.

Pour tout $\alpha \in \mathbf{N}^n$, les applications $\varphi \mapsto \partial^{\alpha}\varphi$ et $\varphi \mapsto X^{\alpha}\varphi$ sont continues de $\mathscr{S}(\mathbf{R}^n)$ dans lui-même. L’espace $\mathscr{S}(\mathbf{R}^n)$ est une algèbre topologique ; c’est un espace de Fréchet et un espace de Montel (EVT IV, p. 18, déf. 4). Pour tout $p\in [1,+\infty ]$, l’espace $\mathscr{S}(\mathbf{R}^n)$ est contenu dans $\mathscr{L}^p(\mathbf{R}^n)$ et l’injection canonique de $\mathscr{S}(\mathbf{R}^n)$ dans $\mathscr{L}^p(\mathbf{R}^n)$ est continue. L’image de $\mathscr{S}(\mathbf{R}^n)$ dans $L^p(\mathbf{R}^n)$ est dense si $p\not= +\infty$.

Comme toute fonction de Schwartz $\varphi$ est intégrable sur $\mathbf{R}^n$, elle admet une transformée de Fourier notée $\widehat{\varphi}$ qui s’identifie à la fonction continue sur $\mathbf{R}^n$ définie par

$y\mapsto \int_{\mathbf{R}^n}\varphi (x)$ exp($-2i\pi  x\cdot y$)$dx$.

La cotransformée de Fourier de $\varphi$ s’identifie, quand à elle, à la fonction continue définie par

$y\mapsto \int_{\mathbf{R}^n}\varphi (x)$ exp(2$i\pi  x\cdot y)dx$.

Soit $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Soit $\alpha \in \mathbf{N}^n$ un multi-indice. On a

$$
\mathscr{F}(\partial^{\alpha}\varphi ) = (2i\pi )^{|\alpha|}X^{\alpha}\mathscr{F}(\varphi )
$$

$$
\mathscr{F}(X^{\alpha}\varphi ) = (-2i\pi )^{-|\alpha|}\partial^{\alpha}(\mathscr{F}(\varphi ))
$$

#### Proposition 21 {#ts-ii-s1-prop-21 .statement tag=02K1}

La restriction à $\mathscr{S}(\mathbf{R}^n)$ de la transformation de Fourier est un automorphisme d’espaces vectoriels topologiques dont l’inverse est la restriction de la cotransformation de Fourier.

Soit $\Lambda \subset \mathbf{R}^n$ un réseau (TG, VII, p. 4), et soit $\Lambda^*\subset \mathbf{R}^n$ le réseau associé (TG, VII, p. 6), aussi parfois appelé réseau dual.

On appelle covolume du réseau Λ, et on note V(Λ), la mesure de $\mathbf{R}^n/\Lambda$ pour la mesure de Haar induite par la mesure de Lebesgue sur $\mathbf{R}^n($cf. INT, VIII, §5, n$^o5$, exemple). Pour toute fonction $f\in$ $\mathscr{S}(\mathbf{R}^n)$ et tout $y\in \mathbf{R}^n$, on a la formule de Poisson

1

$\sum f(x+y) =\sum\widehat{f}(z)$ exp(2$i\pi  y\cdot z)$.

V(Λ) $_*$

$x\in \Lambda z\in \Lambda$

#### Remarque 1 {#ts-ii-s1-n9-rem-1 .statement tag=02K2}

Plus généralement, d’après le corollaire de la proposition 15 de II, p. 230, cette formule vaut pour toute fonction complexe intégrable sur $\mathbf{R}^n$ telle que

$$
\sum_{x\in\Lambda}|f(x+y)|<+\infty
$$

pour tout $y\in \mathbf{R}^n$ et telle que la fonction sur $\mathbf{T}^n$ définie par

$$
y\mapsto \sum_{x\in\Lambda}f(x+y)
$$

est continue et admet une série de Fourier (cf. ci-dessous) absolument convergente.

#### Remarque 2 {#ts-ii-s1-n9-rem-2 .statement tag=02K3}

Il existe des fonctions $f\in B(\mathbf{R})$ telles que la série $\sum_{n\in\mathbf{Z}}f(n)$ diverge (exercice 4 de II, p. 263).

#### Exemple {#ts-ii-s1-n9-exa-1 .statement tag=02K4}

Soit Q une forme quadratique définie positive sur $\mathbf{R}^n$. La fonction définie par $\varphi (x) =$ exp($-\pi Q(x)$) appartient à $\mathscr{S}(\mathbf{R}^n)$. Il existe $\sigma \in$ GL($n,\mathbf{R}$) tel que $Q(x) =\|\sigma (x)\|^2$ pour tout $x\in \mathbf{R}^n$. La transformée de Fourier de $\varphi$ est donnée pour tout $y\in \mathbf{R}^n$ par

1 $*$

$\widehat{\varphi}(y) =$ exp($-\pi Q(y)$)

$|$det($\sigma$ )$|$

où $Q^*(y) =\|^t\sigma^{-1}(y)\|^2($cf. INT, IX, §6, n$^o$ 4–5 et exercice 1, c) de II, p. 262).

#### Définition 6 {#ts-ii-s1-def-6 .statement tag=02K5}

On appelle espace des distributions tempérées sur $\mathbf{R}^n$ l’espace dual de $\mathscr{S}(\mathbf{R}^n)$ muni de la topologie de la convergence bornée. On le note $\mathscr{S}'(\mathbf{R}^n)$.

Puisque $\mathscr{S}(\mathbf{R}^n)$ est bornologique, l’espace $\mathscr{S}'(\mathbf{R}^n)$ est complet et bornologique (EVT, III, p. 24, cor. 1 et 2). Comme $\mathscr{S}(\mathbf{R}^n)$ est un espace de Montel, il en est de même de $\mathscr{S}'(\mathbf{R}^n)$ (EVT, IV, p. 19, prop. 9).

Soit $\alpha \in \mathbf{N}^n$. On note encore $f\mapsto X^{\alpha}f$ la transposée de l’endomorphisme $\varphi \mapsto X^{\alpha}\varphi$ de $\mathscr{S}(\mathbf{R}^n)$, et on note $f\mapsto \partial^{\alpha}f$ l’endomorphisme de $\mathscr{S}'(\mathbf{R}^n)$ défini par

$$
\langle \partial^{\alpha}f, \varphi \rangle = (-1)^{|\alpha|}\langle f, \partial^{\alpha}\varphi \rangle
$$

pour $f\in \mathscr{S}'(\mathbf{R}^n)$ et $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

Soit $f$ une application linéaire de $\mathscr{S}(\mathbf{R}^n)$ dans $\mathbf{C}$. Alors $f$ est une distribution tempérée si, et seulement si, pour toute famille $(M_{k,\alpha})_{(k,\alpha)\in\mathbf{N}\times\mathbf{N}^n}$ dans $\mathbf{R}_+$, la forme linéaire $f$ est bornée sur l’ensemble des fonctions $\varphi \in \mathscr{S}(\mathbf{R}^n)$ telles que pour tout $(k, \alpha )\in \mathbf{N}\times \mathbf{N}^n$, on a $p_{k,\alpha}(\varphi )\leqslant M_{k,\alpha}$.

Une suite $(f_m)_{m\in\mathbf{N}}$ de distributions tempérées converge vers une distribution tempérée $f$ si, et seulement si, on a $\langle f_m, \varphi \rangle  \rightarrow  \langle f, \varphi \rangle$ pour tout $\varphi \in \mathscr{S}(\mathbf{R}^n)$.

#### Exemple {#ts-ii-s1-n9-exa-2 .statement tag=02K6}

Une mesure $\nu$ sur $\mathbf{R}^n$ est dite tempérée s’il existe un entier positif $r$ tel que l’application continue $x\mapsto (1+\|x\|)^{-r}$ est $\nu$-intégrable sur $\mathbf{R}^n$. La restriction de $\nu$ à $\mathscr{S}(\mathbf{R}^n)$ est une distribution tempérée. Elle est nulle si et seulement si la mesure $\nu$ est nulle.

Soit $p\in [1,+\infty ]$ et $f\in \mathscr{L}^p(\mathbf{R}^n)$. Alors la mesure $f\cdot dx$ de densité $f$ par rapport à la mesure de Lebesgue est tempérée. En particulier, la mesure de Lebesgue $\mu$ sur $\mathbf{R}^n$ est tempérée, et toute mesure bornée sur $\mathbf{R}^n$ est tempérée.

Pour tout $p\in [1,+\infty ]$, on peut identifier $L^p(\mathbf{R}^n)$ à un sous-espace de $\mathscr{S}'(\mathbf{R}^n)$ par l’application linéaire $f\mapsto f\cdot dx$; cette application est continue.

#### Définition 7 {#ts-ii-s1-def-7 .statement tag=02K7}

On appelle transformation de Fourier sur $\mathscr{S}'(\mathbf{R}^n)$, et on note $\mathscr{F}$ (resp. on appelle cotransformation de Fourier, et on note $\mathscr{F})$ la transposée de la transformation de Fourier sur $\mathscr{S}(\mathbf{R}^n)$ (resp. de la cotransformation de Fourier).

Pour $f\in \mathscr{S}'(\mathbf{R}^n)$, la distribution tempérée $\mathscr{F}(f)$ (resp. $\mathscr{F}(f)$) est définie par $\varphi \mapsto  \langle f,\mathscr{F}(\varphi )\rangle$ pour $\varphi \in \mathscr{S}(\mathbf{R}^n)$ (resp. par $\varphi \mapsto$ $\langle f,\mathscr{F}(\varphi )\rangle )$.

La transformation de Fourier sur $\mathscr{S}'(\mathbf{R}^n)$ est un automorphisme d’espaces vectoriels topologiques dont l’inverse est la cotransformation de Fourier $\mathscr{F}$.

#### Proposition 22 {#ts-ii-s1-prop-22 .statement tag=02K8}

Soit $f$ une distribution tempérée appartenant à $\mathscr{M}^1(\mathbf{R}^n)$ (resp. à $L^2(\mathbf{R}^n)$). La transformée de Fourier de $f$ dans $\mathscr{S}'(\mathbf{R}^n)$ est la distribution tempérée associée à la transformée de Fourier de $f$ dans $\mathscr{C}_0(\mathbf{R}^n)$ (resp. dans $L^2(\mathbf{R}^n)$). Il en est de même pour la cotransformation de Fourier.

#### Remarque {#ts-ii-s1-n9-rem-3 .statement tag=02K9}

Les formules élémentaires concernant la transformation de Fourier des mesures restent valides pour la transformation de Fourier des distributions tempérées.

Ainsi, si $\alpha \in \mathbf{N}^n$ et $f\in \mathscr{S}'(\mathbf{R}^n)$, on a

$$
\mathscr{F}(\partial^{\alpha}f) = (2i\pi )^{|\alpha|}X^{\alpha}\mathscr{F}(f)
$$

$$
\mathscr{F}(X^{\alpha}f) = (-2i\pi )^{-|\alpha|}\partial^{\alpha}(\mathscr{F}(f))
$$

Soit $y\in \mathbf{R}^n$. Notons $\boldsymbol{\gamma }(y)$ l’endomorphisme de $\mathscr{S}'(\mathbf{R}^n)$ défini par

$$
\langle \boldsymbol{\gamma }(y)f, \varphi \rangle =\langle f,\boldsymbol{\gamma }(-y)\varphi \rangle
$$

pour $f\in \mathscr{S}'(\mathbf{R}^n)$ et $\varphi \in \mathscr{S}(\mathbf{R}^n)$. Notons $e_y$ le caractère de $\mathbf{R}^n$ tel que $e_y(x) =$ exp(2$i\pi x\cdot y)$. Alors $e_y\in \mathscr{S}'(\mathbf{R}^n)$. On a $\mathscr{F}(e_y) =\varepsilon_y$, et plus généralement

$$
\mathscr{F}(e_yf) =\boldsymbol{\gamma }(y)\mathscr{F}(f)
$$

pour tout $f\in \mathscr{S}'(\mathbf{R}^n).*$

Soient $n\geqslant 1$ un entier et $G =\mathbf{T}^n$, muni de la mesure de Haar normalisée. Le groupe dual de G s’identifie à $\mathbf{Z}^n$ par l’application $h\mapsto \chi_h$, où $\chi_h$ est le caractère unitaire de $\mathbf{T}^n$ obtenu par passage au quotient à partir du caractère $x\mapsto$ exp(2$i\pi h\cdot x)$ de $\mathbf{R}^n$ (corollaire 3 de II, p. 236). La transformée de Fourier d’une mesure $\mu$ sur $\mathbf{T}^n$ s’identifie à la famille $(\widehat{\mu}(h))_{h\in\mathbf{Z}^n}$ où

$$
\widehat{\mu}(h) =\int_{\mathbf{T}^n}e^{-2i\pi h\cdot x}d\mu(x)
$$

La série

$$
\sum_{h\in\mathbf{Z}^n}\widehat{\mu}(h)\chi_h
$$

est appelée la série de Fourier de $\mu$.

Si $f\in L^1(\mathbf{T}^n)$ est telle que sa série de Fourier converge absolument dans $L^1(\mathbf{Z}^n)$, on a alors $f\in \mathscr{C}(\mathbf{T}^n)$ et

$$
f(x) =\sum_{h\in\mathbf{Z}^n}\widehat{f}(h)e^{2i\pi h\cdot x}
$$

pour tout $x\in \mathbf{T}^n$ (théorème 3 de II, p. 222), où

$$
\widehat{f}(h) =\int_{\mathbf{T}^n}f(x)e^{-2i\pi h\cdot x}dx,h\in \mathbf{Z}^n
$$

Pour $f\in L^2(\mathbf{T}^n)$, la formule d’inversion de Fourier (prop. 12 de II, p. 219) dit que, si la série de terme général $\widehat{f}(h)$ converge absolument, on a

$$
f(x) =\sum_{h\in\mathbf{Z}^n}\widehat{f}(h)e^{2i\pi h\cdot x}
$$

pour presque tout $x$ dans $\mathbf{T}^n$.

Cependant, même si $f$ est continue, la série de Fourier de $f$ ne converge en général pas vers $f(x)$ pour tout $x$ (exerc. 30 de II, p. 274). Le résultat suivant est d’autant plus utile.

#### Proposition 23 (Théorème de Fejér) {#ts-ii-s1-prop-23 .statement tag=02KA}

Soit $n\geqslant 1$ un entier. Pour tout $h= (h_i)\in \mathbf{Z}^n$, on note $|h|=$ sup$_i|h_i|$. Soit $f\in \mathscr{C}(\mathbf{T}^n)$. Pour tout entier $N\geqslant 1$, notons $f_N$ la fonction sur $\mathbf{T}^n$ telle que

$$
f_N(x) =\sum_{\substack{h\in\mathbf{Z}^n\\|h|\leqslant N}}\widehat{f}(h)e^{2i\pi h\cdot x}\prod_{j=1}^n\left(1-\frac{|h_j|}{N}\right)
$$

pour $x\in \mathbf{T}^n$. Alors $f_N$ converge vers $f$ dans $\mathscr{C}(\mathbf{T}^n)$.

#### Lemme 11 {#ts-ii-s1-lem-11 .statement tag=02KB}

Pour tout $N\geqslant 1$, soit $\mu_N$ la mesure sur $\mathbf{T}^n$ de densité l’application continue

$$
F_N:x\mapsto \sum_{\substack{h\in\mathbf{Z}^n\\|h|\leqslant N}}e^{2i\pi h\cdot x}\prod_{j=1}^n\left(1-\frac{|h_j|}{N}\right).
$$

La suite des mesures $(\mu_N)_{N\geqslant 1}$ converge vers $\varepsilon_0$ dans l’espace $\mathscr{M}^1(\mathbf{T}^n)$ muni de la topologie de la convergence compacte dans $\mathscr{C}(\mathbf{T}^n)$.

On se ramène au cas $n= 1$ en notant que $\mu_N$ est le produit de mesures du même type pour $n= 1$. Il suffit alors de vérifier que la suite $(\mu_N)$ satisfait aux hypothèses du lemme 4 de INT, VIII, §2, n$^o7$ avec $a= 0$.

Pour cela, notons tout d’abord que $F_N$ est la cotransformée de Fourier de l’application $\varphi_N:h\mapsto (1- |h|/N)$ sur $\mathbf{Z}$. Celle-ci s’écrit $\varphi_N=$ $N^{-1}\psi_N*\widetilde{\psi}_N$, où $\psi_N$ est la fonction caractéristique de l’ensemble défini par $-N/2<|h|\leqslant N/2$. Par conséquent, $F_N= N^{-1}|\mathscr{F}(\psi_N)|^2\geqslant 0$. Ainsi, $\mu_N$ est une mesure positive ; on a $\mu_N(\mathbf{T}) = 1$, ce qui démontre (i) et (iii) dans loc. cit.

Démontrons la condition (ii) de loc. cit. Soit U un voisinage ouvert de 0 dans $\mathbf{T}$. Il suffit de démontrer que $\mu_N(U)\rightarrow 1$ quand $N\rightarrow +\infty$. Soient K un voisinage compact symétrique de 0 tel que $K^2\subset U$ et $\psi$ la fonction caractéristique de K. Posons $\varphi =\psi *\psi$. C’est un élément de $A(\mathbf{T})$ à support contenu dans U. Le nombre réel $m=\varphi (0)$ est la mesure de l’ensemble K et donc $m >0$. De plus, il vient $0\leqslant \varphi \leqslant m$ puisque $\varphi (x)$ est la mesure de l’ensemble $K\cap xK$. On a

$\mu_N(U)\geqslant 1\int\varphi (x)\mu_N(x) =$ 1 $\sum\mathscr{F}(\varphi )(h)\varphi_N(h)$

$$
m_{\mathbf{T}}m
$$

$h\in \mathbf{Z}$

d’après les propriétés de transposition de la transformation de Fourier (prop. 13 de II, p. 221). Puisque $\varphi \in A(\mathbf{T})$, sa transformée de Fourier appartient à $L^1(\mathbf{Z})$ et $\varphi$ vérifie la formule d’inversion de Fourier (prop. 11 de II, p. 217). Comme $\varphi_N(h)\rightarrow 1$ pour tout $h\in \mathbf{Z}$ et $|\varphi_N(h)|\leqslant 1$, le théorème de Lebesgue (INT, IV, §3, n$^o7$, th. 6) et la formule d’inversion de Fourier impliquent que

lim inf $\mu_N(U)\geqslant$ 1 lim $\sum\mathscr{F}(\varphi )(h)\varphi_N(h) =$

$N\rightarrow +\infty mN\rightarrow +\infty h\in \mathbf{Z}$

1 $\sum\mathscr{F}(\varphi )(h) =1\varphi (0) = 1$.

$$
m_{h\in\mathbf{Z}}m
$$

Démontrons la proposition. On a $f*F_N=f_N$ pour $N\geqslant 1$. La représentation régulière $\boldsymbol{\gamma }$ de $\mathbf{T}^n$ dans $\mathscr{C}(\mathbf{T}^n)$ (INT, VIII, §2, n$^o3)$ est continue et vérifie $f*F_N=\boldsymbol{\gamma }(\mu_N)f$ (INT, VIII, §4, n$^o5$, prop. 5 (iv)). L’application $\mu\mapsto \boldsymbol{\gamma }(\mu)f$ est continue de $\mathscr{M}^1(\mathbf{T}^n)$ dans $\mathscr{C}(\mathbf{T}^n)$ (INT, VI, §1, n$^o6$, prop. 14). D’après le lemme, on a donc

$_{N\rightarrow}$lim$_{+\infty}f_N=_{N\rightarrow}$lim$_{+\infty}f*F_N=_{N\rightarrow}$lim$_{+\infty}\boldsymbol{\gamma }(\mu_N)f=\boldsymbol{\gamma }(\varepsilon_0)(f) =f$

dans $\mathscr{C}(\mathbf{T}^n)$.

#### Remarque {#ts-ii-s1-n9-rem-4 .statement tag=02KC}

Il existe des fonctions $f\in L^1(\mathbf{T})$ dont la série de Fourier diverge en tout point $x\in \mathbf{T}$ (théorème de Kolmogorov, cf. exercice 51 de II, p. 289).

Un théorème de Carleson[^1] démontre que les sommes partielles symétriques de la série de Fourier de $f$ convergent vers $f(x)$ pour presque tout $x\in \mathbf{T}$ si $f\in \mathscr{L}^2(\mathbf{T})$.

## EXERCICES {#ts-ii-s1-exercises}

See the [exercises for § 1](exercises/s1/).

[^1]: L. Carleson, On convergence and growth of partial sums of Fourier series, Acta Mathematica 116 (1), 1966, p. 135–157.
