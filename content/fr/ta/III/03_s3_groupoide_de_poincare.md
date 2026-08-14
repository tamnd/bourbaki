---
book: ta
book_title: Topologie algébrique
chapter: III
chapter_title: HOMOTOPIE ET GROUPOÏDE DE POINCARÉ
section: 3
section_title: Groupoïde de Poincaré
lang: fr
source: ta-i-iv-fr
book_pages: A III.289-A III.300
pdf_pages: 0305-0316
extraction: native
subsections:
    - "no": 1
      title: Groupoïde de Poincaré
      page: 289
      pdf_page: 305
    - "no": 2
      title: Fonctorialité du groupoïde de Poincaré
      page: 293
      pdf_page: 309
    - "no": 3
      title: Lacets librement homotopes
      page: 299
      pdf_page: 315
statements: 27
exercises: 0
content_sha256: 8ae9f3b618ebca68a814b8db68dc1f380d756c9ac56c880f36553601d75c8f9c
---

## § 3. GROUPOÏDE DE POINCARÉ

### 1. Groupoïde de Poincaré

#### Définition 1 {#ta-iii-s3-def-1 .statement tag=01YE}

Soit X un espace topologique, soient $c_0$ et $c_1$ des chemins dans X et $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow X$ une homotopie reliant $c_0$ à $c_1$. On dit que $\sigma$ est une homotopie stricte si les applications $s\mapsto \sigma (0, s)$ et $s\mapsto \sigma (1, s)$ sont constantes.

On dit que des chemins $c_0$ et $c_1$ dans X sont strictement homotopes s’il existe une homotopie stricte reliant $c_0$ à $c_1$.

Deux chemins strictement homotopes ont même origine et même terme.

#### Exemple {#ta-iii-s3-n1-exa-1 .statement tag=01YF}

Soit $c$ un chemin dans X et soit $\varphi :\mathbf{I}\rightarrow \mathbf{I}$ une application continue telle que $\varphi (0) = 0$ et $\varphi (1) = 1$. Les chemins $c$ et $c\circ \varphi$ sont strictement homotopes. En effet, l’application $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow X$ définie par $\sigma (t, s) =c((1-s)t+s\varphi (t))$ est une homotopie stricte reliant $c$ à $c\circ \varphi$.

Soit X un espace topologique. Rappelons (cf. III, p. 257) que Λ(X) désigne l’espace topologique $\mathscr{C}_c(\mathbf{I}; X)$ des chemins de X et que pour $x$, $y\in X$, $\Lambda_{x,y}(X)$ est le sous-espace de Λ(X) formé des chemins d’origine $x$ et de terme $y$. La famille des ensembles $\Lambda_{x,y}(X)$, pour $x,y\in X$, est une partition de l’espace des chemins de X. Par la bijection canonique (III, p. 257, remarque 2) de $\mathscr{C}(\mathbf{I}\times \mathbf{I}; X)$ sur $\mathscr{C}(\mathbf{I}; \Lambda (X))$, les homotopies strictes correspondent aux chemins $c:\mathbf{I}\rightarrow \Lambda (X)$ dont l’image est contenue dans un sous-espace de la forme $\Lambda_{x,y}(X)$. La relation « les chemins $c_0$ et $c_1$ sont strictement homotopes » est donc une relation d’équivalence dans Λ(X) (III, p. 259, prop. 5) et les classes d’équivalence pour cette relation sont les composantes connexes par arcs des sous-espaces $\Lambda_{x,y}(X)$ de l’espace des chemins de X. On note $\varpi_{x,y}(X)$ l’ensemble $\pi_0(\Lambda_{x,y}(X))$ et on appelle classe de chemins reliant $x$ à $y$ tout élément de $\varpi_{x,y}(X)$.

#### Définition 2 {#ta-iii-s3-def-2 .statement tag=01YG}

On appelle espace des lacets de X, et on note Ω(X),le sous-espace de Λ(X) constitué des lacets (III, p. 256, déf. 1) dans X.

On note $\Omega_x(X)$ l’ensemble $\Lambda_{x,x}(X)$. Les éléments de $\Omega_x(X)$ sont appelés les lacets dans X en $x$ et les éléments de $\varpi_{x,x}(X)$ sont appelés classes de lacets dans X en $x$. L’application $e_x:\mathbf{I}\rightarrow X$ constante d’image $x$ est un lacet, appelé le lacet constant en $x$; sa classe d’homotopie stricte est notée $\varepsilon_x$. L’application $x\mapsto e_x$ de X dans Λ(X) est continue (III, p. 257, prop. 1).

Soit X un espace topologique et soient $x,y,z$ des points de X. Par passage aux composantes connexes par arcs, on déduit de l’application continue $c\mapsto \overline{c}$ de $\Lambda_{x,y}(X)$ dans $\Lambda_{y,x}(X)$ (III, p. 258, corollaire) une application de $\varpi_{x,y}(X)$ dans $\varpi_{y,x}(X)$ que l’on note $\gamma \mapsto \overline{\gamma}$. Si $\gamma \in$ $\varpi_{x,y}(X),\overline{\gamma}$ s’appelle l’inverse de la classe de chemins $\gamma$.

De même, si l’on identifie les ensembles $\pi_0(\Lambda_{x,y}(X))\times \pi_0(\Lambda_{y,z}(X))$ et $\pi_0(\Lambda_{x,y}(X)\times \Lambda_{y,z}(X))$ (III, p. 260, prop. 6), on déduit de l’application continue $(c, d)\mapsto c*d$ de $\Lambda_{x,y}(X)\times \Lambda_{y,z}(X)$ dans $\Lambda_{x,z}(X)$ (III, p. 258, corollaire), par passage aux composantes connexes par arcs, une application $C_{x,y,z}:\varpi_{x,y}(X)\times \varpi_{y,z}(X)\rightarrow \varpi_{x,z}(X)$. Pour $\gamma \in \varpi_{x,y}(X)$ et $\delta \in \varpi_{y,z}(X)$, on note $\gamma \delta$ la classe d’homotopie stricte $C_{x,y,z}(\gamma , \delta )$. On l’appelle la composée des classes de chemins juxtaposables $\gamma$ et $\delta$.

On a $\overline{\overline{\gamma}}=\gamma$ et $\overline{\gamma \delta}=\delta  \gamma$.

#### Proposition 1 {#ta-iii-s3-prop-1 .statement tag=01YH}

Soit X un espace topologique, soient $x,y,z,u$ des points de X et soient $\gamma_1\in \varpi_{x,y}(X),\gamma_2\in \varpi_{y,z}(X),\gamma_3\in \varpi_{z,u}(X)$ des classes de chemins. On a

$$
\varepsilon_x\gamma_1=\gamma_1\varepsilon_y=\gamma_1 \tag{1}
$$

$$
\gamma_1\overline{\gamma}_1=\varepsilon_x,\overline{\gamma}_1\gamma_1=\varepsilon_y \tag{2}
$$

$$
(\gamma_1\gamma_2)\gamma_3=\gamma_1(\gamma_2\gamma_3) \tag{3}
$$

Soient $c_1\in \Lambda_{x,y}(X),c_2\in \Lambda_{y,z}(X),c_3\in \Lambda_{z,u}(X)$ des représentants de $\gamma_1,\gamma_2$ et $\gamma_3$ respectivement. Soit $\varphi :\mathbf{I}\rightarrow \mathbf{I}$ la fonction définie par

$t/2$ pour $0\leqslant t\leqslant 1/2$,

(4) $\varphi (t) =t-1/4$ pour $1/2\leqslant t\leqslant 3/4$,

$2t-1$ pour $3/4\leqslant t\leqslant 1$.

La fonction $\varphi$ est affine sur chacun des trois intervalles $[0,1/2]$, $[1/2,3/4]$ et $[3/4,1]$; elle est donc continue. On a $\varphi (0) = 0$ et $\varphi (1) = 1$. Il résulte de la formule (1) de III, p. 256 définissant la juxtaposition des chemins que

$$
c_1*(c_2*c_3) = ((c_1*c_2)*c_3)\circ \varphi
$$

D’après l’exemple de III, p. 289, les chemins $c_1*(c_2*c_3)$ et $(c_1*c_2)*c_3$ sont strictement homotopes, d’où l’égalité (3).

De même, la fonction $\psi :\mathbf{I}\rightarrow \mathbf{I}$ définie par

$2t$ pour $0\leqslant t\leqslant 1/2$,

$$
\psi (t) = \tag{5}
$$

1 pour $1/2\leqslant t\leqslant 1$

est continue et vérifie $\psi (0) = 0,\psi (1) = 1$. L’égalité $\gamma_1\varepsilon_y=\gamma_1$ résulte alors de ce que

$$
c_1*e_y=c_1\circ \psi
$$

et l’égalité $\varepsilon_x\gamma_1=\gamma_1$ se démontre de même, d’où (1).

L’application $\sigma :\mathbf{I}\times \mathbf{I}\rightarrow X$ définie par

$c_1(2ts)$ pour $0\leqslant t\leqslant 1/2$,

$$
\sigma (t, s) = \tag{6}
$$

$c_1(2(1-t)s)$ pour $1/2\leqslant t\leqslant 1$

est continue ; c’est une homotopie stricte reliant le chemin $e_x$ au chemin $c_1*\overline{c_1}$, d’où la première égalité de (2). La seconde résulte de la première et du fait que, pour tout chemin $c$, on a $c=\overline{\overline{c}}$.

#### Remarque 1 {#ta-iii-s3-n1-rem-1 .statement tag=01YI}

Soit X un espace topologique. Soit $n$ un entier $\geqslant 1$ et soit $(c_1, . . . , c_n)$ une suite de chemins dans X telle que $c_i$ et $c_{i+1}$ soient juxtaposables pour $1\leqslant i\leqslant n-1$ (une telle suite est appelée suite de chemins juxtaposables). Notons $c$ le chemin

$$
c_1*(c_2*(\cdots  *(c_{n-1}*c_n). . .))
$$

et $c'$ le chemin défini par $c'(t) =c_i(nt-i+ 1)$ pour $1\leqslant i\leqslant n$ et $t\in [\frac{i-1}{n},\frac{i}{n}]$. Les chemins $c$ et $c'$ ont même image et sont strictement homotopes : l’un est le composé de l’autre avec un homéomorphisme de $\mathbf{I}$ laissant fixes 0 et 1 (cf. III, p. 289, exemple). On notera parfois $c_1*c_2* \cdots  *c_n$ le chemin $c'$.

Il existe un unique graphe orienté $\varpi (X)$ dont l’ensemble des sommets est X et dont l’ensemble des flèches reliant un point $x$ à un point $y$ est $\varpi_{x,y}(X)$, et dans lequel les applications $C_{x,y,z}$ définissent une loi de composition. D’après la proposition $1,\varpi (X)$ est un groupoïde (II, p. 162, déf. 4). Pour tout $x\in X$, l’élément neutre en le sommet $x$ de ce groupoïde est la classe du lacet constant d’image $x$. L’inverse d’une flèche $\gamma$ est la flèche $\overline{\gamma}$ que nous noterons aussi $\gamma^{-1}$. En particulier, la loi de composition $C_{x,x,x}$ munit, pour tout $x\in X$, l’ensemble $\varpi_{x,x}(X)$ d’une structure de groupe ; on note ce groupe $\pi_1(X, x)$.

#### Définition 3 {#ta-iii-s3-def-3 .statement tag=01YJ}

Soit X un espace topologique. Le groupoïde $\varpi (X)$ est appelé groupoïde de Poincaré, ou groupoïde fondamental, de l’espace X. Soit $x$ un point de X ; le groupe $\pi_1(X, x)$ des classes de lacets en $x$ est appelé groupe de Poincaré, ou groupe fondamental, de l’espace X au point $x$.

Soit $\mathscr{U}$ un ensemble de parties de X dont les intérieurs recouvrent X. Les classes de chemins dans X dont l’image est contenue dans une des parties appartenant à $\mathscr{U}$ engendrent le groupoïde $\varpi (X)$ (lemme 4 de III, p. 272).

Les orbites du groupoïde $\varpi (X)$ (II, p. 162) coïncident avec les composantes connexes par arcs de l’espace X. En particulier (loc. cit.), on a :

#### Proposition 2 {#ta-iii-s3-prop-2 .statement tag=01YK}

Soit X un espace topologique.

a) Si l’espace X est connexe par arcs, les groupes $\pi_1(X, x)$ et $\pi_1(X, y)$ sont isomorphes pour tous points $x$ et $y$ de X.

b) Soit $x$ un point de X ; les conditions suivantes sont équivalentes :

(i) Le groupe $\pi_1(X, x)$ est trivial ;

(ii) Deux chemins d’origine $x$ dans X qui ont le même terme

sont strictement homotopes ;

(iii) Tout lacet d’origine $x$ dans X est strictement homotope

au lacet constant d’image $x$.

Plus précisément, soit X un espace topologique connexe par arcs et soient $x$ et $y$ des points de X. Pour tout élément $\delta$ de $\varpi_{x,y}(X)$, l’application $u_{\delta}:\gamma \mapsto \delta \gamma \delta^{-1}$ de $\pi_1(X, y)$ dans $\pi_1(X, x)$ est un isomorphisme de groupes dont l’isomorphisme réciproque est $u_{\delta^{-1}}$. Pour $\delta \in \varpi_{x,y}(X)$ et $\gamma \in \pi_1(X, y)$, on pose $^{\delta}\gamma =u_{\delta}(\gamma )$. Lorsque $x=y$, on a $^{\delta}\gamma =$ Int($\delta$ )$(\gamma )$, i.e. $u_{\delta}=$ Int($\delta$ ).

Soient $x,y,z$ des points de X. Pour $\delta \in \varpi_{x,y}(X)$ et $\eta \in \varpi_{y,z}(X)$, on a $u_{\delta \eta}=u_{\delta}\circ u_{\eta}$, ce qui s’écrit aussi $^{\delta \eta}\gamma =^{\delta}(^{\eta}\gamma )$ pour $\gamma \in \pi_1(X, z)$.

Soient $x,y$ des points de X et soient $\delta ,\delta '$ des éléments de $\varpi_{x,y}(X)$. On a

(7) $u_{\delta'}=u_{\delta}\circ$ Int($\delta^{-1}\delta '$) $=$ Int($\delta '\delta^{-1}$)$\circ u_{\delta}$.

#### Remarque 2 {#ta-iii-s3-n1-rem-2 .statement tag=01YL}

Soit X un espace topologique et soit C une composante connexe par arcs de X. Si $x$ et $y$ sont des points de C, l’espace topologique $\Lambda_{x,y}(C)$ s’identifie à l’espace topologique $\Lambda_{x,y}(X)$, de sorte que l’ensemble $\varpi_{x,y}(C)$ s’identifie à l’ensemble $\varpi_{x,y}(X)$. Ainsi, le groupoïde fondamental $\varpi (C)$ s’identifie au sous-groupoïde plein de $\varpi (X)$ ayant C pour ensemble de points. En particulier, pour tout point $x$ de C, le groupe $\pi_1(C, x)$ s’identifie au groupe $\pi_1(X, x)$.

#### Remarque 3 {#ta-iii-s3-n1-rem-3 .statement tag=01YM}

Soit X un espace topologique et soient $x,y,z$ des points de X. L’application $(c, d)\mapstochar \rightarrow c*d$ de $\Lambda_{x,y}(X)\times \Lambda_{y,z}(X)$ dans $\Lambda_{x,z}(X)$ est continue (III, p. 258, corollaire de la prop. 2). On prendra garde que l’application de composition $\varpi_{x,y}(X)\times \varpi_{y,z}(X)\rightarrow \varpi_{x,z}(X)$ qui s’en déduit n’est pas nécessairement continue lorsqu’on munit les ensembles $\varpi_{x,y}(X),\varpi_{y,z}(X)$ et $\varpi_{x,z}(X)$ des topologies quotient (cf. TG, I, p. 35 et III, p. 259). Cependant, pour tout $\gamma_0\in \varpi_{x,y}(X)$ et tout $\delta_0\in \varpi_{y,z}(X)$, les applications partielles $\gamma \mapsto \gamma \delta_0$ de $\varpi_{x,y}(X)$ dans $\varpi_{x,z}(X)$ et $\delta \mapsto \gamma_0\delta$ de $\varpi_{y,z}(X)$ dans $\varpi_{x,z}(X)$ sont des homéomorphismes. En effet, soit $c_0\in \Lambda_{x,y}(X)$ un chemin de classe $\gamma_0$. L’application $d\mapsto c_0*d$ est une application continue de $\Lambda_{y,z}(X)$ dans $\Lambda_{x,z}(X)$. L’application $\delta \mapsto \gamma_0\delta$ s’en déduit par passage aux quotients, donc est continue. Il en est de même de l’application $\delta '\mapsto \gamma_0^{-1}\delta '$ de $\varpi_{x,z}(X)$ dans $\varpi_{y,z}(X)$. Ces deux applications étant réciproques l’une de l’autre, ce sont des homéomorphismes. On raisonne de façon analogue pour l’application $\gamma \mapsto \gamma \delta_0$. Voir aussi IV, p. 374.

### 2. Fonctorialité du groupoïde de Poincaré

Soient X, Y des espaces topologiques et soit $f: X\rightarrow Y$ une application continue. L’application $c\mapsto f\circ c$ est une application continue, notée $\Lambda (f)$, de Λ(X) = $\mathscr{C}_c(\mathbf{I}; X)$ dans Λ(Y) = $\mathscr{C}_c(\mathbf{I}; Y)$ (I, p. 132, lemme). Elle définit par passage aux sous-ensembles des applications continues

$$
\Lambda_x(f): \Lambda_x(X)\rightarrow \Lambda_{f(x)}(Y)
$$

pour $x\in X$,

$$
\Lambda_{x,y}(f): \Lambda_{x,y}(X)\rightarrow \Lambda_{f(x),f(y)}(Y)
$$

pour $x,y\in X$ et

$$
\Omega (f): \Omega (X)\rightarrow \Omega (Y)
$$

Pour $x\in X$, l’application $\Lambda_{x,x}(f)$ est aussi notée $\Omega_x(f)$. Par passage aux composantes connexes par arcs (III, p. 290), on déduit de l’application $\Lambda_{x,y}(f)$ une application

$$
\varpi_{x,y}(f):\varpi_{x,y}(X)\rightarrow \varpi_{f(x),f(y)}(Y)
$$

Soient $x,y,z$ des points de X et soient $c\in \Lambda_{x,y}(X),d\in \Lambda_{y,z}(X)$ des chemins ; par définition de la juxtaposition des chemins, on a

$$
f\circ (c*d) = (f\circ c)*(f\circ d)
$$

Par passage aux classes d’homotopie stricte, il en résulte la relation

$$
\varpi_{x,z}(f)(\gamma \delta ) = (\varpi_{x,y}(f)(\gamma ))(\varpi_{y,z}(f)(\delta ))
$$

pour tout $\gamma \in \varpi_{x,y}(X)$ et tout $\delta \in \varpi_{y,z}(X)$. Ainsi, l’application continue $f$ et les applications $\varpi_{x,y}(f)$, pour $x$ et $y\in$ X, définissent un morphisme du groupoïde $\varpi (X)$ dans le groupoïde $\varpi (Y)$ (II, p. 161, déf. 3). On le note $\varpi (f)$ et on l’appelle le morphisme de groupoïdes de Poincaré déduit de l’application continue $f$. En particulier, si $x$ est un point de X, l’application $\varpi_{x,x}(f)$ est un homomorphisme du groupe $\pi_1(X, x)$ dans le groupe $\pi_1(X, f(x))$ ; cet homomorphisme se note aussi $\pi_1(f, x)$.

#### Remarque 1 {#ta-iii-s3-n2-rem-1 .statement tag=01YN}

L’homomorphisme $\varpi_{x,y}(f)$ est continu si l’on munit les ensembles $\varpi_{x,y}(X)$ et $\varpi_{f(x),f(y)}(Y)$ de la topologie quotient de la topologie de la convergence compacte sur $\mathscr{C}_c(\mathbf{I}; X)$ et $\mathscr{C}_c(\mathbf{I}; Y)$.

Pour simplifier l’écriture, si $x,y\in X$ et $\gamma \in \varpi_{x,y}(X)$, on écrira parfois $f_*(\gamma )$ l’élément $\varpi_{x,y}(f)(\gamma )$ de $\varpi_{f(x),f(y)}(Y)$.

Soient X, Y, Z des espaces topologiques, soient $f: X\rightarrow Y,g: Y\rightarrow Z$ des applications continues. Pour tout chemin $c$ dans X, on a $(g\circ f)\circ c=$ $g\circ (f\circ c)$. Il en résulte que l’on a

$$
\varpi (g\circ f) =\varpi (g)\circ \varpi (f)
$$

Soient X et Y des espaces topologiques, soient $f_0$ et $f_1$ des applications continues de X dans Y et soit $\sigma : X\times \mathbf{I}\rightarrow Y$ une homotopie reliant $f_0$ à $f_1$. L’application $(c, t)\mapsto c(t)$ de $\mathscr{C}_c(\mathbf{I}; X)\times \mathbf{I}$ dans X (III, p. 257, prop. 1) étant continue, il en est de même de l’application de $\mathscr{C}_c(\mathbf{I}; X)\times \mathbf{I}\times \mathbf{I}$ dans Y donnée par $(c, t, s)\mapsto \sigma (c(t), s)$. Par suite, l’application $\Sigma : (c, s)\mapsto \sigma (c(\cdot ), s)$ est une application continue de $\mathscr{C}_c(\mathbf{I}; X)\times \mathbf{I}$ dans $\mathscr{C}_c(\mathbf{I}; Y)$ (loc. cit.). L’application Σ est une homotopie reliant l’application $\Lambda (f_0)$ à l’application $\Lambda (f_1)$. Par restriction aux espaces de lacets, l’application Σ induit une homotopie $\Omega (X)\times \mathbf{I}\rightarrow \Omega (Y)$ reliant $\Omega (f_0)$ à $\Omega (f_1)$. Soit $x$ un point de X ; supposons que l’homotopie $\sigma$ soit une homotopie pointée en $x$ et posons $y=f_0(x) =f_1(x)$. L’application Σ induit alors une application continue de $\Omega_x(X)\times \mathbf{I}$ dans $\Omega_y(Y)$ qui est une homotopie pointée en $e_x$, reliant l’application $\Omega_x(f_0)$ à l’application $\Omega_x(f_1)$.

#### Proposition 3 {#ta-iii-s3-prop-3 .statement tag=01YO}

Soient X et Y des espaces topologiques, $f_0$ et $f_1$ des applications continues de X dans Y et soit $\sigma : X\times \mathbf{I}\rightarrow$ Y une homotopie reliant $f_0$ à $f_1$. Soit $x$ un point de X ; posons $y_0=f_0(x)$, $y_1=f_1(x)$ et notons $\delta \in \varpi_{y_0,y_1}(Y)$ la classe du chemin $d$ défini par $d(t) =\sigma (x, t)$ pour $t\in \mathbf{I}$. Pour tout $\gamma \in \pi_1(X, x)$, on a $(f_1)_*(\gamma ) =$ $\delta^{-1}(f_0)_*(\gamma )\delta$.

Soit $c$ un lacet de X en $x$ et soit $\gamma$ sa classe d’homotopie stricte. Posons $\gamma_0= (f_0)_*(\gamma )$ et $\gamma_1= (f_1)_*(\gamma )$ ; ce sont les classes d’homotopie stricte de $f_0\circ c$ et $f_1\circ c$. Pour $(t, s)\in \mathbf{I}\times \mathbf{I}$, posons $\varphi (t, s) =\sigma (c(t), s)$. Pour tout $t\in \mathbf{I}$, on a $\varphi (t,0) = (f_0\circ c)(t),\varphi (t,1) = (f_1\circ c)(t)$ et $\varphi (0, t) =\varphi (1, t) =d(t)$. La relation $\gamma_0\delta =\delta \gamma_1$ résulte donc du lemme suivant.

#### Lemme 1 {#ta-iii-s3-lem-1 .statement tag=01YP}

Soit Y un espace topologique et soit $\varphi :\mathbf{I}\times \mathbf{I}\rightarrow Y$ une application continue. Pour $t\in \mathbf{I}$, posons $c_0(t) =\varphi (t,0),c_1(t) =\varphi (t,1)$, $d_0(t) =\varphi (0, t)$ et $d_1(t) =\varphi (1, t)$. Les chemins $c_0*d_1$ et $d_0*c_1$ sont strictement homotopes.

Notons $c$ le chemin dans $\mathbf{I}\times \mathbf{I}$ obtenu en juxtaposant les chemins $t\mapsto (t,0)$ et $t\mapsto (1, t)$ ; notons $d$ le chemin dans $\mathbf{I}\times \mathbf{I}$ obtenu en juxtaposant les chemins $t\mapsto (0, t)$ et $t\mapsto (t,1)$. Les chemins $c$ et $d$ ont même origine $(0,0)$ et même terme $(1,1)$. L’application $(t, s)\mapsto$ $(1-s)c(t)+sd(t)$ de $\mathbf{I}\times \mathbf{I}$ dans $\mathbf{I}\times \mathbf{I}$ est une homotopie stricte reliant $c$ à $d$. On a $c_0*d_1=\varphi \circ c$ et $d_0*c_1=\varphi \circ d$; ces deux chemins sont donc strictement homotopes.

#### Corollaire 1 {#ta-iii-s3-lem-1-cor-1 .statement tag=01YQ}

Soient X et Y des espaces topologiques et soit $x$ un point de X. Soient $f_0$ et $f_1$ des applications continues de X dans Y. S’il existe une homotopie pointée en $x$ reliant $f_0$ à $f_1$, on a $\pi_1(f_0, x) =$ $\pi_1(f_1, x)$.

Soit $\sigma$ une homotopie pointée en $x$ reliant $f_0$ à $f_1$. Avec les notations de la prop. $3,\delta$ est la classe d’un chemin constant d’image $f_0(x) =$ $f_1(x)$. L’assertion en résulte.

#### Corollaire 2 {#ta-iii-s3-lem-1-cor-2 .statement tag=01YR}

Soient X et Y des espaces topologiques et soit $f: X\rightarrow$ Y une homéotopie. Pour tout point $x$ de X, l’homomorphisme

$$
\pi_1(f, x):\pi_1(X, x)\rightarrow \pi_1(Y, f(x))
$$

est un isomorphisme.

Soit $g$ une application continue de Y dans X, réciproque à homotopie près de $f$. Soit $x$ un point de X. Il résulte de la prop. 3 appliquée aux applications homotopes Id$_X$ et $g\circ f: X\rightarrow X$ que l’application $\pi_1(g\circ f, x)$ est un isomorphisme du groupe $\pi_1(X, x)$ sur le groupe $\pi_1(X, g\circ f(x))$. Puisque

$$
\pi_1(g\circ f, x) =\pi_1(g, f(x))\circ \pi_1(f, x)
$$

l’homomorphisme $\pi_1(f, x)$ est injectif et l’homomorphisme $\pi_1(g, f(x))$ est surjectif. Comme l’application $g$ est aussi une homéotopie, l’homomorphisme $\pi_1(g, f(x))$ est injectif ; c’est donc un isomorphisme. Par suite, $\pi_1(f, x)$ est un isomorphisme.

#### Exemple {#ta-iii-s3-n2-exa-1 .statement tag=01YS}

Soit G un groupe topologique, soit $e$ son élément neutre. Pour tout point $g$ de G, les translations à gauche et à droite, $x\mapsto gx$ et $x\mapsto xg$, sont des homéomorphismes de G sur lui-même (TG, III, p. 2) qui appliquent $e$ sur $g$. D’après le corollaire 2, elles induisent des isomorphismes de $\pi_1(G, e)$ sur $\pi_1(G, g)$. Ces isomorphismes ne sont pas nécessairement égaux (IV, p. 459, exerc. 1).

#### Corollaire 3 {#ta-iii-s3-lem-1-cor-3 .statement tag=01YT}

Soit X un espace topologique homéotope à un point. Pour tout point $x$ de X, le groupe $\pi_1(X, x)$ est réduit à l’élément neutre.

Le cor. 3 s’applique en particulier quand X est l’espace numérique à $n$ dimensions $\mathbf{R}^n$ et plus généralement quand X est une partie de l’espace $\mathbf{R}^n$ qui est étoilée (III, p. 234) par rapport à un de ses points.

#### Proposition 4 {#ta-iii-s3-prop-4 .statement tag=01YU}

Soit X l’espace produit d’une famille $(X_j)_{j\in J}$ d’espaces topologiques. Le morphisme du groupoïde $\varpi (X)$ dans le produit des groupoïdes $\varpi (X_j)$, pour $j\in J$, défini par la famille de morphismes $(\varpi$(pr$_j))_{j\in J}$ est un isomorphisme.

Notons $\varphi$ ce morphisme de groupoïdes. L’application qui s’en déduit par passage aux sommets est l’application identique $X\rightarrow \prod_jX_j$. Soient $x= (x_j)$ et $y= (y_j)$ deux points de X. Notons $\varphi_{x,y}$ l’application de $\varpi_{x,y}(X)$ dans $\prod_j\varpi_{x_j,y_j}(X_j)$ déduite de $\varphi$. Si pour tout $j\in J,c_j:\mathbf{I}\rightarrow$ $X_j$ est un chemin reliant $x_j$ à $y_j$, l’application $t\mapsto (c_j(t))$ est un chemin dans X reliant $x$ à $y$ (TG, I, p. 25, prop. 1). Cela prouve que $\varphi_{x,y}$ est surjective. Soient $c$ et $d$ deux chemins dans X reliant $x$ à $y$. Supposons qu’il existe pour tout $j\in J$ une homotopie stricte $\sigma_j:\mathbf{I}\times \mathbf{I}\rightarrow X_j$ reliant pr$_j\circ c$ à pr$_j\circ d$. Alors, l’application $(t, s)\mapsto (\sigma_j(t, s))$ de $\mathbf{I}\times \mathbf{I}$ dans X est une homotopie stricte reliant $c$ à $d($loc. cit.). Cela prouve que $\varphi_{x,y}$ est injective.

#### Corollaire {#ta-iii-s3-n2-cor-1 .statement tag=01YV}

Soit $x= (x_j)_{j\in J}$ un point de X. L’application

$$
\pi_1(X, x)\rightarrow \prod_{j\in J}\pi_1(X_j, x_j)
$$

déduite des applications $\pi_1$(pr$_j, x_j)$ est un isomorphisme de groupes.

Cet isomorphisme est dit canonique. Dans la suite, nous identifierons souvent $\pi_1(X, x)$ à $\prod_{j\in J}\pi_1(X_j, x_j)$ au moyen de cet isomorphisme.

#### Remarque 2 {#ta-iii-s3-n2-rem-2 .statement tag=01YW}

Soit $(X_j)_{j\in J}$ une famille d’espaces topologiques. Notons X l’espace topologique produit $\prod_{j\in J}X_j$ et soit $x= (x_j)$ un point de X.

Pour tout $i\in J$, soit $u_i: X_i\rightarrow X$ l’application telle que, pour $z\in X_i$, pr$_i\circ u_i(z) =z$ et, pour tout $j\in J$ distinct de $i$, pr$_j\circ u_i(z) =$ $x_j$. L’application $u_i$ est continue et l’application $\pi_1(u_i, x_i)$ s’identifie à l’injection canonique du facteur $\pi_1(X_i, x_i)$ dans le groupe produit de la famille $(\pi_1(X_j, x_j))_{j\in J}($cf. A, I, p. 45).

Supposons que l’ensemble J soit fini et, pour tout $j\in J$, soit $\gamma_j$ un élément de $\pi_1(X_j, x_j)$. L’élément $(\gamma_j)$ de $\pi_1(X, x)$ est le composé des classes de lacets $(u_j)_*(\gamma_j),j\in J$, ces classes étant deux à deux permutables.

#### Remarque 3 {#ta-iii-s3-n2-rem-3 .statement tag=01YX}

Soit $(X_j)_{j\in J}$ une famille d’espaces topologiques. Notons X l’espace topologique produit $\prod_{j\in J}X_j$ et soit $x= (x_j)$ un point de X.

Munissons les ensembles $\pi_1(X, x)$ et $\pi_1(X_j, x_j)$ de la topologie quotient de la topologie de la convergence compacte sur les espaces $\Lambda_x(X)$ et $\Lambda_{x_j}(X_j)$. L’isomorphisme $\pi_1(X, x)\rightarrow \prod_{j\in J}\pi_1(X_j, x_j)$ est alors un homéomorphisme. Il est continu (III, p. 294, remarque 1). La topologie de la convergence compacte sur Λ(X) est engendrée par les parties de la forme $\mathbf{T}(K,U)$, où K est une partie compacte de $\mathbf{I}$ et U un ouvert de X. Pour $j\in J$, soit $U_j$ un ouvert de $X_j$, tels que $\prod_{j\in J}U_j\subset U$. Alors (pr$_j)_*(\mathbf{T}(K,U))$ contient $\mathbf{T}(K,U_j)$. Cela montre que les applications (pr$_j)_*: \Lambda_x(X)\rightarrow \Lambda_{x_j}(X_j)$ sont ouvertes, et les applications $\pi_1$(pr$_j, x_j)$ sont aussi ouvertes. Comme elles sont surjectives, l’application $\pi_1(X, x)\rightarrow \prod_{j\in J}\pi_1(X_j, x_j)$ est ouverte (TG, I, p. 34, prop. 8). Étant continue et bijective, c’est un homéomorphisme (TG, I, p. 30, exemple 2).

#### Proposition 5 {#ta-iii-s3-prop-5 .statement tag=01YY}

Soit X un espace topologique et soit $(A_i)_{i\in I}$ une famille croissante de parties de X, indexée par un ensemble ordonné filtrant I, telle que toute partie quasi-compacte de X soit contenue dans l’un des $A_i$. Le morphisme de groupoïdes canonique

$\rho :$ lim$\longrightarrow \varpi (A_i)\rightarrow \varpi (X)$,

$i\in I$

déduit des injections canoniques de $A_i$ dans X, est un isomorphisme.

Si $i\leqslant j$, notons $\rho_{j,i}$ le morphisme de groupoïdes $\varpi (A_i)\rightarrow \varpi (A_j)$ déduit de l’injection de $A_i$ dans $A_j$. Comme l’application déduite de $\rho_{j,i}$ par passage aux sommets est l’injection $A_i\rightarrow A_j$ et que les $A_i$ recouvrent X, l’application déduite de $\rho$ par passage aux sommets est bijective.

Soient $a$ et $b$ des points de X et soit $c$ un chemin reliant $a$ à $b$ dans X. L’image de $c$ est une partie quasi-compacte de X (TG, I, p. 62, th. 2), car $\mathbf{I}$ est compact. Il existe donc un élément $i\in I$ tel que l’image de $c$ soit contenue dans $A_i$. Par suite, l’application déduite de $\rho$ par passage aux ensembles de flèches est surjective.

Soit $i\in I$, soient $a$ et $b$ des points de $A_i$, soient $c,c'$ des chemins reliant $a$ à $b$ dans $A_i$; soit $h$ une homotopie stricte reliant $c$ à $c'$ dans X. Comme $\mathbf{I}\times \mathbf{I}$ est compact, $h(\mathbf{I}\times \mathbf{I})$ est une partie quasi-compacte de X (loc. cit.) et il existe un élément $i\in I$ tel que l’image de $h$ soit contenue dans $A_i$. Les chemins $c$ et $c'$ sont strictement homotopes dans $A_i$; a fortiori, les classes de chemins $[c]$ et $[c']$ ont même image dans lim$\longrightarrow \varpi (A_i)$. Par suite, $\rho$ est injectif.

#### Corollaire {#ta-iii-s3-n2-cor-2 .statement tag=01YZ}

Soit $a$ un point de X et soit J l’ensemble des $i\in I$ tels que $a\in A_i$. L’homomorphisme canonique

lim$\longrightarrow \pi_1(A_i, a)\rightarrow \pi_1(X, a)$

$i\in J$

est bijectif.

#### Remarque 4 {#ta-iii-s3-n2-rem-4 .statement tag=01Z0}

La proposition et son corollaire s’appliquent en particulier lorsque $(A_i)_{i\in I}$ est une famille croissante de parties de X indexée par un ensemble ordonné filtrant I telle que les intérieurs des $A_i$ recouvrent X.

### 3. Lacets librement homotopes

#### Définition 4 {#ta-iii-s3-def-4 .statement tag=01Z1}

Soit X un espace topologique et soient $c$ et $c'$ deux lacets dans X. On appelle homotopie libre reliant $c$ à $c'$ une homotopie $\sigma$ reliant $c$ à $c'$ telle que $\sigma (0, s) =\sigma (1, s)$ pour tout $s\in \mathbf{I}$. On dit que $c$ est librement homotope à $c'$ s’il existe une homotopie libre reliant $c$ à $c'$.

Les homotopies libres reliant $c$ à $c'$ correspondent aux chemins reliant $c$ à $c'$ dans l’espace Ω(X) des lacets de X. Par suite, la relation « $c$ est librement homotope à $c'$ » est une relation d’équivalence dans Ω(X) dont les classes d’équivalence sont les composantes connexes par arcs de Ω(X).

#### Remarque {#ta-iii-s3-n3-rem-1 .statement tag=01Z2}

Soit $\varphi$ l’application canonique de $\mathbf{R}$ sur $\mathbf{T}=\mathbf{R}/\mathbf{Z}$ (TG, V, p. 2). L’application $f\mapsto f\circ \varphi |\mathbf{I}$ est un homéomorphisme de $\mathscr{C}_c(\mathbf{T}; X)$ sur Ω(X), d’où, par passage aux composantes connexes par arcs, une bijection de l’ensemble $[\mathbf{T}; X]$ (III, p. 230) sur l’ensemble des classes d’homotopie libre de lacets dans X.

#### Proposition 6 {#ta-iii-s3-prop-6 .statement tag=01Z3}

Soit X un espace topologique connexe par arcs et soit $x$ un point de X.

a) Tout lacet dans X est librement homotope à un lacet en $x$. Plus précisément, si $c$ est un lacet en $y$ et $d$ un chemin d’origine $y$ et de terme $x,c$ est librement homotope au lacet $(\overline{d}*c)*d$ en $x$.

b) Deux lacets dans X en $x$ sont librement homotopes si et seulement si leurs classes d’homotopie stricte sont conjuguées dans le groupe $\pi_1(X, x)$.

Démontrons a). Pour tout $s\in [0,1]$, notons $d_s$ le chemin dans X défini par $d_s(t) =d(st)$ pour $t\in \mathbf{I}$; son origine est $y$. Comme l’application $(s, t)\mapsto d(st)$ est continue, l’application $s\mapsto d_s$ de $\mathbf{I}$ dans $\mathscr{C}_c(\mathbf{I}; X)$ est continue (III, p. 257, prop. 1). L’application $s\mapsto (\overline{d_s}*c)*d_s$ est alors un chemin dans Ω(X) (III, p. 257, prop. 2) reliant $(e_y*c)*e_y$ à $(\overline{d}*c)*d$, d’où a).

Soient $c$ et $c'$ deux lacets dans X en $x$. Si leurs classes d’homotopie stricte sont conjuguées dans $\pi_1(X, x)$, il existe un lacet $d$ en $x$ tel que $c'$ soit strictement homotope au lacet $(\overline{d}*c)*d$. Il résulte de a) que $c$ et $c'$ sont librement homotopes. Réciproquement, supposons qu’il existe une homotopie libre $\varphi$ reliant $c$ à $c'$. Posons $d(t) =\varphi (0, t)$, on a aussi $d(t) =\varphi (1, t)$ et $d$ est un lacet en $x$. D’après le lemme 1 de III, p. 295, les lacets $c*d$ et $d*c'$ sont strictement homotopes. Les classes d’homotopie stricte de $c$ et $c'$ sont donc conjuguées dans $\pi_1(X, x)$.

#### Scholie {#ta-iii-s3-n3-sch-1 .statement tag=01Z4}

Soit X un espace topologique connexe par arcs et soit $x$ un point de X. La proposition 6 permet de définir une bijection canonique de l’ensemble des classes d’homotopie libre de lacets dans X sur l’ensemble des classes de conjugaison dans $\pi_1(X, x)$.
