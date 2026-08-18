---
book: ta
book_title: Topologie algébrique
chapter: II
chapter_title: GROUPOÏDES
section: 4
section_title: Homotopies
lang: fr
source: ta-i-iv-fr
book_pages: TA II.180-TA II.196
pdf_pages: 0196-0212
extraction: native
subsections:
    - "no": 1
      title: Définition des homotopies
      page: 180
      pdf_page: 196
    - "no": 2
      title: Homotopismes de groupoïdes
      page: 181
      pdf_page: 197
    - "no": 3
      title: Cohomotopeur
      page: 184
      pdf_page: 200
    - "no": 4
      title: Comparaison de deux cohomotopeurs
      page: 187
      pdf_page: 203
    - "no": 5
      title: Groupes d’isotropie d’un cohomotopeur
      page: 192
      pdf_page: 208
statements: 15
exercises: 0
content_sha256: 42b6b15a8d35c52c77c4cdd11ec65007ecd0a759eb51efe44e28c26290c10d75
---

## § 4. HOMOTOPIES

### 1. Définition des homotopies

#### Définition 1 {#ta-ii-s4-def-1 .statement tag=01U3}

Soient G un groupoïde, H un carquois, $\varphi$ et $\varphi '$ des morphismes de carquois de H dans G. Une homotopie reliant $\varphi$ à $\varphi '$ est une application $h$ de l’ensemble des sommets de H dans l’ensemble des flèches de G possédant les propriétés suivantes :

(i) Pour tout sommet $a$ de H, la flèche $h(a)$ a pour origine $\varphi (a)$ et pour terme $\varphi '(a)$ ;

(ii) Pour toute flèche $f$ de H, d’origine $a$ et de terme $b$, on a $\varphi (f)h(b) =h(a)\varphi '(f)$.

On dit que $\varphi$ et $\varphi '$ sont homotopes s’il existe une homotopie reliant $\varphi$ à $\varphi '$.

Soit G un groupoïde, soit H un carquois et soient $\varphi ,\varphi ',\varphi ''$ des morphismes de carquois de H dans G. L’application $a\mapsto e_{\varphi(a)}$ est une homotopie reliant $\varphi$ à $\varphi$. Si $h$ est une homotopie reliant $\varphi$ à $\varphi '$, l’application $a\mapsto h(a)^{-1}$ est une homotopie reliant $\varphi '$ à $\varphi$. Soient $h$ et $h'$ des homotopies reliant $\varphi$ à $\varphi '$ et $\varphi '$ à $\varphi ''$ respectivement. Pour tout sommet $a$ de H, les flèches $h(a)$ et $h'(a)$ sont composables. L’application $a\mapsto h(a)h'(a)$ est une homotopie reliant $\varphi$ à $\varphi ''$.

Il en résulte que la relation « $\varphi$ est homotope à $\varphi '$ » est une relation d’équivalence dans l’ensemble des morphismes de carquois de H dans G.

Soient G un groupoïde, H un carquois et $\varphi ,\varphi '$ des morphismes de carquois de H dans G qui sont homotopes. D’après la condition (i) de la définition 1, pour tout sommet $a$ de H, les sommets $\varphi (a)$ et $\varphi '(a)$ appartiennent à une même orbite de G.

Supposons de plus que H soit un groupoïde et soit $h$ une homotopie reliant $\varphi$ à $\varphi '$. Les applications Orb($\varphi$ ) et Orb($\varphi '$) déduites de $\varphi$ et $\varphi '$ par passage aux orbites sont donc égales. Pour tout sommet $a$ de H et toute flèche $f\in H_a$, on a $\varphi (f) =h(a)\varphi '(f)h(a)^{-1}=$ Int($h(a)$)$(\varphi '(f))$, d’après la condition (ii) de la définition 1. Autrement dit, l’homomorphisme $\varphi_a$ est égal à Int($h(a)$)$\circ \varphi '_a$. En particulier, si l’homomorphisme $\varphi_a$ est injectif (resp. bijectif, resp. surjectif), il en est de même de l’homomorphisme $\varphi '_a$.

#### Remarque 1 {#ta-ii-s4-n1-rem-1 .statement tag=01U4}

Soient G, $G'$ des groupoïdes, H, $H'$ des carquois, soient $u: H'\rightarrow H$ un morphisme de carquois et $v: G\rightarrow G'$ un morphisme de groupoïdes. Si des morphismes de carquois $\varphi ,\varphi '$ de H dans G sont homotopes, les morphismes de carquois $v\circ \varphi \circ u$ et $v\circ \varphi '\circ u$ de $H'$ dans $G'$ sont homotopes. Plus précisément, si $h$ est une homotopie reliant $\varphi$ à $\varphi '$, l’application Fl($v$)$\circ h\circ$ Som($u$) est une homotopie reliant $v\circ \varphi \circ u$ à $v\circ \varphi '\circ u$.

#### Remarque 2 {#ta-ii-s4-n1-rem-2 .statement tag=01U5}

Soit G un groupoïde, soit H un carquois et soient $\varphi , \psi$ des morphismes de carquois de H dans G. Notons $j$ le morphisme canonique de H dans Grp(H), soient $\overline{\varphi}$ et $\overline{\psi}$ les morphismes de groupoïdes de Grp(H) dans G tels que $\overline{\varphi}\circ j=\varphi$ et $\overline{\psi}\circ j=\psi$.

Rappelons que Som(H) = Som(Grp(H)).

Une homotopie $h:$ Som(H) $\rightarrow$ Fl(G) reliant $\varphi$ à $\psi$ est une homotopie reliant $\overline{\varphi}$ à $\overline{\psi}$.

### 2. Homotopismes de groupoïdes

Dans ce n$^o$, nous utiliserons la notation $u\sim v$ pour exprimer que deux morphismes de groupoïdes $u$ et $v$ sont homotopes.

#### Définition 2 {#ta-ii-s4-def-2 .statement tag=01U6}

Soient G, $G'$ des groupoïdes et soit $\varphi$ un morphisme de G dans $G'$. On appelle inverse à homotopie près de $\varphi$ un morphisme de groupoïdes $\psi$ de $G'$ dans G tel que les morphismes $\psi \circ \varphi$ et $\varphi \circ \psi$ soient respectivement homotopes à Id$_G$ et à Id$_{G'}$. On dit que $\varphi$ est un homotopisme s’il existe un inverse de $\varphi$ à homotopie près.

Un isomorphisme de groupoïdes est un homotopisme.

Soient G et $G'$ des groupoïdes. Soient $\varphi ,\varphi '$ des morphismes de groupoïdes de G dans $G'$ qui sont homotopes. Si $\varphi$ est un homotopisme, il en est de même de $\varphi '$. En effet, si $\psi$ désigne un inverse de $\varphi$ à homotopie près, on a $\psi \circ \varphi '\sim \psi \circ \varphi \sim$ Id$_G$ et $\varphi '\circ \psi \sim \varphi \circ \psi \sim$ Id$_{G'}$, ce qui démontre que $\psi$ est inverse à homotopie près de $\varphi '$.

Soient G, $G',G''$ des groupoïdes et soient $\varphi : G\rightarrow G',\varphi ': G'\rightarrow G''$, $\psi : G'\rightarrow G,\psi ': G''\rightarrow G'$ des morphismes de groupoïdes. Alors, des conditions suivantes :

(i) $\psi$ est inverse à homotopie près de $\varphi$;

(ii) $\psi '$ est inverse à homotopie près de $\varphi '$;

(iii) $\psi \circ \psi '$ est inverse à homotopie près de $\varphi '\circ \varphi$; deux quelconques entraînent la troisième. En effet, supposons d’abord que (i) et (ii) soient satisfaites ; on a alors

$\psi \circ \psi '\circ \varphi '\circ \varphi \sim \psi \circ$ Id$_{G'}\circ \varphi \sim \psi \circ \varphi \sim$ Id$_G$

et, de même, $\varphi '\circ \varphi \circ \psi \circ \psi '\sim$ Id$_{G'}$, d’où (iii). Si (i) et (iii) sont satisfaites,

$\varphi '\circ \psi '\sim \varphi '\circ \varphi \circ \psi \circ \psi '\sim$ Id$_{G''}$

et

$\psi '\circ \varphi '\sim (\varphi \circ \psi )\circ \psi '\circ \varphi '\circ (\varphi \circ \psi )\sim \varphi \circ \psi \sim$ Id$_{G'}$,

d’où la condition (ii). La démonstration que les conditions (ii) et (iii) entraînent la condition (i) est analogue.

En particulier, si deux des morphismes $\varphi ,\varphi ',\varphi '\circ \varphi$ sont des homotopismes, il en est de même du troisième.

#### Proposition 1 {#ta-ii-s4-prop-1 .statement tag=01U7}

Soient G, $G'$ des groupoïdes, soit $\varphi$ un morphisme de G dans $G'$, et soit A une partie de l’ensemble des sommets de G qui rencontre chaque orbite de G. Pour que $\varphi$ soit un homotopisme, il faut et il suffit que les conditions suivantes soient satisfaites :

(i) l’application Orb($\varphi$ ) de Orb(G) dans Orb(G$')$, déduite de $\varphi$ par passage aux orbites, est bijective ;

(ii) pour tout $a\in A$, l’homomorphisme $\varphi_a: G_a\rightarrow G'_{\varphi(a)}$ est bijectif.

Supposons d’abord que $\varphi$ soit un homotopisme et soit $\psi$ un inverse de $\varphi$ à homotopie près. Alors,

Orb($\psi$ )$\circ$ Orb($\varphi$ ) $=$ Orb($\psi \circ \varphi$ ) $=$ Orb(Id$_G) =$ Id$_{Orb(G)}$,

car deux morphismes de groupoïdes homotopes induisent la même application par passage aux orbites. De même, Orb($\varphi$ )$\circ$ Orb($\psi$ ) $=$ Id$_{Orb(G')}$. L’application Orb($\varphi$ ) est donc bijective, d’où l’assertion (i). On a aussi, pour tout sommet $a$ de G,

$$
\psi_{\varphi(a)}\circ \varphi_a= (\psi \circ \varphi )_a
$$

comme $\psi \circ \varphi$ est homotope à Id$_G$, l’homomorphisme $(\psi \circ \varphi )_a$ est bijectif (cf. p. 180), si bien que $\varphi_a$ est injectif et $\psi_{\varphi(a)}$ est surjectif. En échangeant les rôles de $\varphi$ et $\psi$, on voit que $\varphi_a$ est aussi surjectif, d’où la condition (ii).

Supposons maintenant que les conditions (i) et (ii) soient satisfaites et démontrons que $\varphi$ est un homotopisme.

Traitons d’abord le cas où chaque orbite de $G'$ est réduite à un point.

Pour chaque sommet $b$ de $G'$, choisissons un sommet $u(b)$ de G appartenant à A et dont l’image par $\varphi$ soit $b$. C’est possible car l’application Orb($\varphi$ ) est surjective et que A rencontre chaque orbite de G. Soit $f$ une flèche de $G'$; on a $o(f) =t(f)$ par hypothèse ; posons $b=o(f)$ et $a=u(b)$. D’après la condition (ii), il existe une unique flèche $v(f)\in G_a$ dont l’image par $\varphi$ soit $f$. Le couple $\psi = (u, v)$ est un morphisme de groupoïdes de $G'$ dans G. Démontrons que $\psi$ est inverse de $\varphi$ à homotopie près. On a déjà $\varphi \circ \psi =$ Id$_{G'}$ par construction de $\psi$.

Soit $x$ un sommet de G. Posons $a=\psi (\varphi (x))$; c’est un élément de A tel que $\varphi (a) =\varphi (x)$. Puisque Orb($\varphi$ ) est injectif, $a$ appartient à l’orbite de $x$ dans G et il existe une flèche $f$ dans G reliant $a$ à $x$. La flèche $h(x) =\psi (\varphi (f))^{-1}f$ relie alors $a$ à $x$ et l’on a $\varphi (h(x)) =e_{\varphi(a)}$.

Montrons que l’application $h:$ Som(G) $\rightarrow$ Fl(G) ainsi définie est une homotopie qui relie $\psi \circ \varphi$ à Id$_G$. La condition (i) de la définition 1 est satisfaite, par construction. Soient $f$ une flèche de G$,x$ son origine et $y$ son terme. On a $\varphi (x) =\varphi (y)$ ; posons $a=\psi (\varphi (x)) =\psi (\varphi (y))$. Les flèches $h(x)f h(y)^{-1}$ et $\psi \circ \varphi (f)$ appartiennent à $G_a$ et ont toutes deux pour image $\varphi (f)$ dans $G'_{\varphi(a)}$. Comme l’application $\varphi_a$ est injective, on a $h(x)f h(y)^{-1}=\psi \circ \varphi (f)$. La condition (ii) de la définition 1 est ainsi satisfaite.

Démontrons maintenant la proposition 1 dans le cas général. Soit X une forêt orientée maximale de $G'($II, p. 157, prop. 1). Soit $G''$ le groupoïde déduit de $G'$ par contraction des flèches de X et soit $\varphi ': G'\rightarrow G''$ le morphisme canonique. Le morphisme $\varphi '$ satisfait aux conditions de la prop. 1 (II, p. 170, remarque 1 et p. 178, cor. 2), et il en est donc de même du morphisme $\varphi '\circ \varphi$.

Comme les orbites de $G''$ sont réduites à des points, il résulte du cas particulier déjà démontré que $\varphi '$ et $\varphi '\circ \varphi$ sont des homotopismes, si bien que $\varphi$ en est un également. Cela termine la démonstration de la proposition.

#### Corollaire 1 {#ta-ii-s4-prop-1-cor-1 .statement tag=01U8}

Soit G un groupoïde, soit A un ensemble et soit $f: A\rightarrow$ Som(G) une application. Si l’image de $f$ rencontre chaque orbite de G, le morphisme de groupoïdes canonique $\varphi$ de $f^*G$ dans G est un homotopisme.

Par définition du groupoïde image réciproque (II, p. 166, exemple 4), A est l’ensemble des sommets du groupoïde $f^*G$ et l’on a Fl$_{a,b}(f^*G) =$ Fl$_{f(a),f(b)}(G)$ pour tout couple $(a, b)$ d’éléments de A. Par ailleurs, on a Som($\varphi$ ) $=f$ et Fl($\varphi$ ) induit l’application identique de Fl$_{a,b}(f^*G)$ dans Fl$_{f(a),f(b)}(G)$. Par suite, l’application Orb($\varphi$ ) est bijective et l’homomorphisme $\varphi_a: (f^*G)_a\rightarrow G_{f(a)}$ est un isomorphisme, pour tout $a\in A$. Les hypothèses de la proposition 1 sont donc vérifiées.

#### Corollaire 2 {#ta-ii-s4-prop-1-cor-2 .statement tag=01U9}

Soit G un groupoïde, soit X une forêt orientée de G, soit $G'$ le groupoïde déduit de G par contraction des flèches de X. Le morphisme canonique de G dans $G'$ est un homotopisme.

Il résulte en effet de la remarque 1 de II, p. 170 et du corollaire 2 de II, p. 178 que les hypothèses de la proposition 1 sont vérifiées.

### 3. Cohomotopeur

Soit H un carquois, soit G un groupoïde et soient $\varphi$ et $\psi$ des morphismes de carquois de H dans G.

Notons $G_1$ le carquois défini de la façon suivante : les sommets de $G_1$ sont ceux de G ; les flèches de $G_1$ sont les éléments de l’ensemble somme des ensembles Fl(G) et Som(H) ; l’application origine de $G_1$ coïncide avec celle de G dans Fl(G) et avec Som($\varphi$ ) dans Som(H) ; l’application terme de $G_1$ coïncide avec celle de G dans Fl(G) et avec Som($\psi$ ) dans Som(H). Notons $\alpha_1$ le morphisme de carquois de G dans $G_1$ défini par l’application identique de Som(G) et par l’injection canonique de Fl(G) dans Fl(G$_1)$. Notons $h_1$ l’injection canonique Som(H) $\rightarrow$ Fl(G$_1)$.

Considérons le groupoïde libre Grp(G$_1)$ construit sur $G_1($II, p. 174, déf. 9) et notons $\theta_1$ le morphisme canonique de carquois de $G_1$ dans Grp(G$_1)$. Désignons enfin par Coh($\varphi , \psi$ ) le groupoïde déduit de Grp(G$_1)$ par contraction des lacets (en l’origine de $x)$

$$
\alpha_1(x)\alpha_1(y)\alpha_1(xy)^{-1} \tag{1}
$$

pour tout couple $(x, y)$ de flèches composables de G, ainsi que des lacets (en $\varphi (a)$)

$$
\alpha_1(\varphi (f))h_1(b)\alpha_1(\psi (f))^{-1}h_1(a)^{-1} \tag{2}
$$

pour $a,b$ dans Som(H) et $f\in$ Fl$_{ab}(H)$. Notons $\pi :$ Grp(G$_1)\rightarrow$ Coh($\varphi , \psi$ ) le morphisme canonique ; posons $\alpha$ = $\pi \circ \theta_1\circ \alpha_1$ et $h=$ Fl($\pi \circ \theta_1$)$\circ h_1$.

#### Proposition 2 {#ta-ii-s4-prop-2 .statement tag=01UA}

Le groupoïde Coh($\varphi , \psi$ ) est engendré par le sous-carquois dont l’ensemble des sommets est Som(G) et celui des flèches est la réunion des images des applications Fl($\alpha$ ) et $h$.

Ce sous-carquois étant l’image du carquois $G_1$ par le morphisme de carquois $\pi \circ \theta_1$, la proposition résulte aussitôt de la construction de Coh($\varphi , \psi$ ).

#### Proposition 3 {#ta-ii-s4-prop-3 .statement tag=01UB}

Le morphisme de carquois $\alpha$ est un morphisme de groupoïdes de G dans Coh($\varphi , \psi$ ) et l’application $h$ est une homotopie reliant $\alpha \circ \varphi$ à $\alpha \circ \psi$.

Le triplet (Coh($\varphi , \psi$ )$, \alpha , h)$ possède la propriété universelle suivante : si $G'$ est un groupoïde, $\alpha '$ un morphisme de groupoïdes de G dans $G'$ et $h':$ Som(H) $\rightarrow$ Fl(G$')$ une homotopie reliant $\alpha '\circ \varphi$ à $\alpha '\circ \psi$, il existe un unique morphisme de groupoïdes $\eta :$ Coh($\varphi , \psi$ )$\rightarrow G'$ tel que

(3) $\alpha '=\eta \circ \alpha$ et $h'=$ Fl($\eta$ )$\circ h$.

Compte tenu de la définition du groupoïde déduit par contraction de flèches, la contraction des lacets (1) entraîne que $\alpha$ est un morphisme de groupoïdes, la contraction des lacets (2) que $h$ est une homotopie reliant $\alpha \circ \varphi$ à $\alpha \circ \psi$.

Soient $G',\alpha ',h'$ comme dans l’énoncé. Soit $\eta_1$ le morphisme de carquois de $G_1$ dans $G'$ tel que Som($\eta_1$) soit égal à Som($\alpha '$) et tel que Fl($\eta_1$) coïncide avec Fl($\alpha '$) dans Fl(G) et avec $h'$ dans Som(H). Il existe un unique morphisme de groupoïdes $\eta_2:$ Grp(G$_1)\rightarrow G'$ tel que $\eta_1=\eta_2\circ \theta_1$. Comme $\alpha '$ est un morphisme de groupoïdes et $h'$ est une homotopie reliant $\alpha '\circ \varphi$ à $\alpha '\circ \psi ,\eta_2$ définit par passage au quotient un morphisme de groupoïdes $\eta$ de Coh($\varphi , \psi$ ) dans $G'($II, p. 170, prop. 3). Ce morphisme satisfait aux relations (3) et c’est le seul (II, p. 185, prop. 2).

#### Définition 3 {#ta-ii-s4-def-3 .statement tag=01UC}

Le groupoïde Coh($\varphi , \psi$ ) s’appelle le cohomotopeur du couple $(\varphi , \psi )$. On dit que $\alpha$ est le morphisme canonique de G dans Coh($\varphi , \psi$ ) et que $h$ est l’homotopie canonique reliant $\alpha \circ \varphi$ à $\alpha \circ \psi$.

On appelle armature du couple $(\varphi , \psi )$ le carquois dont l’ensemble des sommets est l’ensemble des orbites de G, l’ensemble des flèches est l’ensemble des composantes connexes de H et dont les applications origine et terme sont déduites de $\varphi$ et $\psi$ par passage aux quotients.

#### Proposition 4 {#ta-ii-s4-prop-4 .statement tag=01UD}

L’application Orb($\alpha$ )$:$ Orb(G) $\rightarrow$ Orb(Coh($\varphi , \psi$ )) est surjective, ses fibres sont les composantes connexes de l’armature du couple $(\varphi , \psi )$.

Le morphisme $\alpha$ est le composé des morphismes $\alpha_1: G\rightarrow G_1$, $\theta_1: G_1\rightarrow$ Grp(G$_1)$ et $\pi :$ Grp(G$_1)\rightarrow$ Coh($\varphi , \psi$ ). L’application $\theta_1$ induit une bijection de l’ensemble des composantes connexes du carquois $G_1$ sur l’ensemble des orbites de Grp(G$_1)$ et l’application Orb($\pi$ )$:$ Orb(Grp(G$_1))\rightarrow$ Orb(Coh($\varphi , \psi$ )) est bijective (II, p. 170, remarque 1). Il suffit donc de démontrer que l’application de Orb(G) dans $\pi_0(G_1)$ déduite de $\alpha_1$ est surjective et que ses fibres sont les composantes connexes de l’armature du couple $(\varphi , \psi )$. La surjectivité résulte de ce que l’application Som($\alpha_1$) est l’application identique. La relation d’équivalence dans Som(G) donnée par « $a$ et $b$ sont dans la même composante connexe de $G_1$ » est engendrée par les relations « il existe une flèche de G reliant $a$ à $b$ » et « il existe un sommet $h$ de H tel que $\varphi (h) =a$ et $\psi (h) =b$ ». Cette relation d’équivalence est compatible avec l’application de Som(G) dans Orb(G) et la relation qui s’en déduit dans Orb(G) est engendrée par la relation « il existe une orbite $\eta$ de H telle que Orb($\varphi$ )$(\eta ) =\alpha$ et Orb($\psi$ )$(\eta ) =\beta$ ». C’est donc la relation « $\alpha$ et $\beta$ sont dans la même composante connexe de l’armature du couple $(\alpha , \beta )$ ».

#### Proposition 5 {#ta-ii-s4-prop-5 .statement tag=01UE}

Soit $G'$ un groupoïde, soient $\eta ,\eta '$ des morphismes de groupoïdes de Coh($\varphi , \psi$ ) dans $G'$ et soit $k$ une application de Som(G) dans Fl(G$')$. Pour que $k$ soit une homotopie reliant $\eta$ à $\eta '$, il faut et il suffit que les deux conditions suivantes soient satisfaites :

(i) L’application $k$ est une homotopie reliant $\eta \circ \alpha$ à $\eta '\circ \alpha$;

(ii) Pour tout sommet $a$ de H, on a

$$
\eta (h(a))k(\psi (a)) =k(\varphi (a))\eta '(h(a))
$$

Par définition, pour que $k$ soit une homotopie reliant $\eta$ à $\eta '$, il faut et il suffit que les deux conditions suivantes soient réalisées (rappelons que Som(G) = Som(Coh($\varphi , \psi$ ))) :

a) Pour tout sommet $x$ de Coh($\varphi , \psi$ )$,k(x)$ relie $\eta (x)$ à $\eta '(x)$ ;

b) Pour tout couple $(x, y)$ de sommets de Coh($\varphi , \psi$ ) et toute flèche $f\in$ Fl$_{x,y}$(Coh($\varphi , \psi$ )), on a $\eta (f)k(y) =k(x)\eta '(f)$.

D’après la prop. 2, il suffit de vérifier la condition b) lorsque $f$ appartient à l’image de Fl($\alpha$ ) ou à celle de $h$, de sorte que b) équivaut à la conjonction des deux conditions c) et d) ci-dessous :

c) Pour $x\in$ Som(G), $y\in$ Som(G) et $g\in$ Fl$_{x,y}(G)$, on a $\eta (\alpha (g))k(y) =k(x)\eta '(\alpha (g))$;

d) Pour tout $a\in$ Som(H), on a $\eta (h(a))k(\psi (a)) =k(\varphi (a))\eta '(h(a))$. La condition (i) équivaut à la conjonction de a) et c), et la condition (ii) est la condition d), d’où le corollaire.

### 4. Comparaison de deux cohomotopeurs

Considérons un diagramme

H $^{\varphi}$ G

$$
u^{\psi}_v \tag{4}
$$

$$
{H'}^{\varphi'}_{\psi'}G'
$$

où H, $H'$, G, $G'$ sont des groupoïdes et $u,v,\varphi ,\psi ,\varphi ',\psi '$ des morphismes de groupoïdes tels que $v\circ \varphi =\varphi '\circ u$ et $v\circ \psi =\psi '\circ u$.

Notons $\alpha$ le morphisme canonique de G dans le cohomotopeur Coh($\varphi , \psi$ ) et $h$ l’homotopie canonique reliant $\alpha \circ \varphi$ à $\alpha \circ \psi$; définissons de façon analogue $\alpha '$ et $h'$. Alors, $\alpha '\circ v$ est un morphisme de groupoïdes de G dans Coh($\varphi ', \psi '$) et $h'\circ$ Som($u$) est une homotopie reliant $\alpha '\circ \varphi '\circ u$ à $\alpha '\circ \psi '\circ u$, c’est-à-dire $\alpha '\circ v\circ \varphi$ à $\alpha '\circ v\circ \psi$. D’après la propriété universelle des cohomotopeurs (II, p. 185, prop. 3), il existe un unique morphisme de groupoïdes $w$ de Coh($\varphi , \psi$ ) dans Coh($\varphi ', \psi '$) tel que $w\circ \alpha =\alpha '\circ v$ et Fl($w$)$\circ h=h'\circ$ Som($u$). Nous avons en particulier étendu le diagramme (4) en un diagramme

H $^{\varphi}$ G $^{\alpha}$ Coh($\varphi , \psi$ )

$$
u^{\psi}_vw \tag{5}
$$

${H'}^{\varphi'}_{\psi'}{G'}^{\alpha'}$ Coh($\varphi ', \psi '$)

dans lequel le second carré est commutatif.

#### Théorème 1 {#ta-ii-s4-thm-1 .statement tag=01UF}

Faisons les hypothèses suivantes :

(i) le morphisme de groupoïdes $v$ est un homotopisme ;

(ii) l’application Orb($u$)$:$ Orb(H) $\rightarrow$ Orb(H$')$, déduite de $u$ par passage aux orbites, est bijective ;

(iii) il existe dans chaque orbite de H un point $a$ tel que l’homomorphisme $u_a: H_a\rightarrow H'_{u(a)}$ soit surjectif.

Alors, le morphisme de groupoïdes $w:$ Coh($\varphi , \psi$ )$\rightarrow$ Coh($\varphi ', \psi '$) est un homotopisme.

Soit $G''$ le groupoïde déduit de $G'$ par contraction des flèches d’une forêt orientée maximale. Le morphisme canonique $v': G'\rightarrow G''$ est un homotopisme (II, p. 184, corollaire 2 de la prop. 1). Les deux diagrammes

H $^{\varphi}$ G ${H'}^{\varphi'}G'$

$u\psi v'\circ v$ et Id$_{H'}\psi 'v'$

$$
H'vv''\circ \circ \psi \varphi ''G'H'vv''\circ \circ \psi \varphi ''G''
$$

donnent lieu à des morphismes de groupoïdes $w'_1:$ Coh($\varphi , \psi$ )$\rightarrow$ Coh($v'\circ \varphi ', v'\circ \psi '$) et $w'_2:$ Coh($\varphi ', \psi '$)$\rightarrow$ Coh($v'\circ \varphi ', v'\circ \psi '$) ; on a $w'_1=w'_2\circ w$. Il suffit donc de démontrer que $w'_1$ et $w'_2$ sont des homotopismes. Comme les applications Som($v'\circ v$)$:$ Som(G) $\rightarrow$ Som(G$'')$ et Som($v'$)$:$ Som(G$')\rightarrow$ Som(G$'')$ sont surjectives, il suffit par conséquent de démontrer le théorème sous l’hypothèse supplémentaire que l’application Som($v$) est surjective, hypothèse que nous ferons dans toute la suite de la démonstration.

Démontrons successivement les assertions suivantes :

– L’application Orb($w$) est bijective ;

– Pour tout sommet $a$ de G, l’homomorphisme $w_a$ est surjectif ;

– Pour tout sommet $a$ de G, l’homomorphisme $w_a$ est injectif.

a) Par hypothèse, l’application Orb($u$) est bijective ; il en est de même de l’application Orb($v$) d’après II, p. 182, prop. 1, car $v$ est un homotopisme. Le morphisme de carquois de l’armature du couple $(\varphi , \psi )$ sur celle du couple $(\varphi ', \psi ')$ défini par les applications Orb($u$) et Orb($v$) est donc un isomorphisme. En particulier, l’application qui s’en déduit par passage aux composantes connexes est bijective. La prop. 4 de II, p. 185 implique alors que l’application Orb($w$) est bijective.

b) Soit $f'$ une flèche de $G'$, notons $a'$ son origine et $b'$ son terme. Comme l’application Som($v$) est surjective, il existe des sommets $a$ et $b$ dans G tels que $a'=v(a)$ et $b'=v(b)$. Comme le morphisme $v$ est un homotopisme, il existe une flèche $f$ de G reliant $a$ à $b$ ainsi qu’un élément $g\in G_a$ tel que $v(g) =f'v(f)^{-1}($II, p. 182, prop. 1), d’où $f'=v(gf)$. Cela démontre que l’application Fl($v$) est surjective.

Démontrons alors que l’application Fl($w$) est surjective. Son image contient celle de Fl($\alpha '$), car l’on a $\alpha '\circ v=w\circ \alpha$ et l’application Fl($v$) est surjective. Soit $b$ un sommet de $H'$; soit $a$ un sommet de H tel que $b$ et $u(a)$ soient dans la même orbite de $H'$ et soit $f$ une flèche de $H'$ reliant $u(a)$ à $b$. Alors,

$$
h'(u(a))\cdot (\alpha '\circ \psi ')(f) = (\alpha '\circ \varphi ')(f)\cdot h'(b)
$$

car $h'$ est une homotopie reliant $\alpha '\circ \varphi '$ à $\alpha '\circ \psi '$. La flèche $h'(u(a)) =$ $w(h(a))$ appartient à l’image de Fl($w$), de même que les deux flèches $\alpha '(\psi '(f))$ et $\alpha '(\varphi '(f))$ d’après ce qui précède. Il en résulte que la flèche $h'(b)$ appartient à l’image de Fl($w$), ce qui démontre que l’image de Fl($w$) contient celle de $h'$. D’après la prop. 2 de II, p. 185, l’application Fl($w$) est surjective.

Soit $g'\in$ Coh($\varphi ', \psi '$)$_{u(a)}$. Soit $g$ une flèche de Coh($\varphi , \psi$ ) telle que $w(g) =g'$. Notons $x$ et $y$ l’origine et le terme de $g$; on a $u(x) =$ $u(y) =u(a)$. Soit $g_1$ (resp. $g_2)$ une flèche de G reliant $a$ à $x$ (resp. $a$ à $y)$ dont l’image par $v$ est $e_{u(a)}$. Alors, $\alpha (g_1)g\alpha (g_2)^{-1}$ est un élément de Coh($\varphi , \psi$ )$_a$ dont l’image par $w_a$ est $g'$. Par suite, pour tout sommet $a$ de G, l’homomorphisme $w_a$ est surjectif.

c) Démontrons que, pour tout sommet $a$ de G, l’homomorphisme $w_a$ est injectif. En considérant successivement les diagrammes

H $^{\varphi}$ G H $^{v\circ\varphi}G'$

Id$_H\psi v$ et $uv\circ \psi$ Id$_{G'}$

H $^v_{v\circ}^{\circ\varphi}_{\psi}G'{H'}^{\varphi'}_{\psi'}G'$

on est alors ramené à traiter les deux cas suivants : 1) On a $H'= H$ et $u=$ Id$_H; 2)$ On a $G'= G$ et $v=$ Id$_G$.

1) Supposons que l’on a $H'= H$ et $u=$ Id$_H$.

Considérons un morphisme de groupoïdes $v': G'\rightarrow G$ qui est inverse de $v$ à homotopie près et une homotopie $k:$ Som(G) $\rightarrow$ Fl(G) reliant $v'\circ v$ à Id$_G$. D’après la remarque 1 de II, p. 181, les applications $\alpha \circ k\circ \varphi$ et $\alpha \circ k\circ \psi$ sont des homotopies reliant respectivement $\alpha \circ v'\circ \varphi '$ à $\alpha \circ \varphi$ et $\alpha \circ v'\circ \psi '$ à $\alpha \circ \psi$. Par suite (cf. II, p. 180), l’application

$h_1:$ Som(H) $\rightarrow$ Fl(Coh($\varphi , \psi$ )),

$$
x\mapsto (\alpha \circ k\circ \varphi )(x)\cdot h(x)\cdot ((\alpha \circ k\circ \psi )(x))^{-1}
$$

est une homotopie reliant $\alpha \circ v'\circ \varphi '$ à $\alpha \circ v'\circ \psi '$. D’après la propriété universelle des cohomotopeurs (II, p. 185, prop. 3), il existe un unique morphisme de groupoïdes $w':$ Coh($\varphi ', \psi '$)$\rightarrow$ Coh($\varphi , \psi$ ) tel que $\alpha \circ v'=$ $w'\circ \alpha '$ et $h_1=$ Fl($w'$)$\circ h'$.

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ )

Id$_Hvw$

H $^{\varphi'}_{\psi'}{G'}^{\alpha'}$ Coh($\varphi ', \psi '$)

Id$_Hv'w'$

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ ) .

On a en particulier

$$
\alpha \circ v'\circ v=w'\circ \alpha '\circ v=w'\circ w\circ \alpha
$$

Comme $k$ est une homotopie reliant $v'\circ v$ à Id$_G,\alpha \circ k$ est une homotopie reliant $w'\circ w\circ \alpha$ à $\alpha$. Comme Fl($w'\circ w$)$\circ h=$ Fl($w'$)$\circ h'=h_1$, on a, pour tout sommet $x$ de H,

Fl($w'\circ w$)$\circ h(x)\cdot (\alpha \circ k\circ \psi )(x) =h_1(x)\cdot (\alpha \circ k\circ \psi )(x) = (\alpha \circ k\circ \varphi )(x)\cdot h(x)$,

par définition de $h_1$. D’après la prop. 5 de II, p. 186, appliquée aux morphismes de groupoïdes $w'\circ w$ et Id$_{Coh(\varphi ,\psi)}$, l’application $\alpha \circ k$ est une homotopie reliant $w'\circ w$ à Id$_G$. En particulier, $w'\circ w$ est un homotopisme.

Pour tout sommet $a$ de G, l’homomorphisme de groupes $(w'\circ w)_a$ est donc bijectif (II, p. 182, prop. 1). Il en résulte que l’homomorphisme $w_a$ est injectif, d’où le résultat dans le cas A).

2) Supposons que l’on a $G'= G$ et $v=$ Id$_G$.

Soit $x$ un sommet de $H'$. L’application Orb($u$) étant surjective, il existe un sommet $a$ de H et une flèche $f$ de $H'$ reliant $u(a)$ à $x$. Les flèches $\alpha (\varphi '(f))^{-1},h(a)$ et $\alpha (\psi '(f))$ relient respectivement $\varphi '(x)$ à $\varphi '(u(a)) =\varphi (a),\varphi (a)$ à $\psi (a)$ et $\psi '(u(a)) =\psi (a)$ à $\psi '(x)$, donc sont composables dans Coh($\varphi , \psi$ ). Posons

$$
h_2(x) =\alpha (\varphi '(f))^{-1}\cdot h(a)\cdot \alpha (\psi '(f))
$$

Vérifions que la flèche $h_2(x)$ ainsi définie ne dépend pas des éléments $a$ et $f$ choisis. Soit $a'$ un sommet de H et soit $f'$ une flèche de $H'$ reliant $u(a')$ à $x$. Puisque l’application Orb($u$) est injective, les sommets $a$ et $a'$ de H appartiennent à la même orbite et il existe une flèche $c\in$ Fl(H) reliant $a$ à $a'$. Alors, $u(c)f'f^{-1}$ est un lacet en $u(a)$ dans $H'$. D’après l’hypothèse (iii), il existe un sommet $b$ de H tel que l’homomorphisme $u_b$ soit surjectif et une flèche $c'$ de H reliant $b$ à $a$; alors, Int($u(c')$)$(u(c)f'f^{-1})$ est un lacet en $u(b)$ dans H, c’est donc l’image par $u_b$ d’un lacet $c''$ en $b$. Par conséquent, la flèche $g= (c'c)^{-1}c''c'$ de H relie le sommet $a'$ au sommet $a$ et vérifie $f'=u(g)f$. On a alors

$$
\alpha (\varphi '(f'))^{-1}h(a')\alpha (\psi '(f'))
$$

$$
=\alpha (\varphi '(f))^{-1}\alpha (\varphi '(u(g)))^{-1}h(a')\alpha (\psi '(u(g)))\alpha (\psi '(f))
$$

$$
=\alpha (\varphi '(f))^{-1}\alpha (\varphi (g))^{-1}h(a')\alpha (\psi (g))\alpha (\psi '(f))
$$

$$
=\alpha (\varphi '(f))^{-1}\cdot h(a)\cdot \alpha (\psi '(f))
$$

puisque $h$ est une homotopie reliant $\alpha \circ \varphi$ à $\alpha \circ \psi$. Cela démontre l’indépendance annoncée.

Par construction, on a $h_2(u(x)) =h(x)$ pour tout $x\in$ Som(H). Nous avons ainsi défini une application $h_2$ de Som(H$')$ dans Fl(Coh($\varphi , \psi$ )). Soit $c$ une flèche de $H'$, notons $x$ son origine et $y$ son terme. Soit $a$ un sommet de H et $f$ une flèche de $H'$ reliant $u(a)$ à $x$. Alors, $f c$ est une flèche de $H'$ qui relie $u(a)$ à $y$. Par définition de $h_2$, on a ainsi

$$
h_2(x)\alpha (\psi '(c)) =\alpha (\varphi '(f))^{-1}h(a)\alpha (\psi '(f))\alpha (\psi '(c))
$$

$$
=\alpha (\varphi '(c))\alpha (\varphi '(f c))^{-1}h(a)\alpha (\psi '(f c))
$$

$$
=\alpha (\varphi '(c))h_2(y)
$$

Cela prouve que $h_2$ est une homotopie qui relie $\alpha \circ \varphi '$ à $\alpha \circ \psi '$.

D’après la propriété universelle des cohomotopeurs, il existe un unique morphisme de groupoïdes $w':$ Coh($\varphi ', \psi '$)$\rightarrow$ Coh($\varphi , \psi$ ) tel que $w'\circ \alpha '=\alpha$ et $h_2$ = Fl($w'$)$\circ h'$. On a $w'\circ w\circ \alpha =w'\circ \alpha '=\alpha$ et Fl($w'\circ w$)$\circ h=$ Fl($w'$)$\circ h'\circ$ Som($u$) $=h_2\circ u=h$ par définition de $h_2$. D’après la propriété universelle des cohomotopeurs, cela implique que l’on a $w'\circ w=$ Id$_{Coh(\varphi ,\psi)}$. En particulier, pour tout $a\in$ Som(G), l’homomorphisme $w_a$ est injectif.

Il résulte alors de la prop. 1 de II, p. 182 que le morphisme $w$ est un homotopisme, d’où le théorème.

### 5. Groupes d’isotropie d’un cohomotopeur

Soient G et H des groupoïdes et soient $\varphi ,\psi$ des morphismes de groupoïdes de H dans G. Le but de ce n$^o$ est de calculer les groupes d’isotropie du cohomotopeur Coh($\varphi , \psi$ ). On reprend les notations $G_1, h_1, \theta_1, \alpha , h$ du n$^o3$.

Notons $\Gamma_0$ l’armature du couple $(\varphi , \psi )$ ; rappelons (II, p. 185, déf. 3) qu’il s’agit du carquois (Orb(G), Orb(H)$, \varphi_0, \psi_0)$, où $\varphi_0$ et $\psi_0$ sont les applications de Orb(H) dans Orb(G) déduites des applications $\varphi$ et $\psi$ par passage aux orbites.

Dans toute la suite de ce n$^o$, nous supposerons en outre que le carquois $\Gamma_0$ est connexe et non vide ; d’après II, p. 185, prop. 4, cela revient à supposer que le groupoïde Coh($\varphi , \psi$ ) est transitif, ou encore que le carquois $G_1$ est connexe et non vide (II, p. 185, prop. 2).

#### Définition 4 {#ta-ii-s4-def-4 .statement tag=01UG}

On appelle équipement de base du couple $(\varphi , \psi )$ la donnée :

(i) Pour tout $i\in$ Orb(G), d’un sommet $a(i)$ dans l’orbite $i$ de G;

(ii) Pour tout $j\in$ Orb(H), d’un sommet $b(j)$ dans l’orbite $j$ de H ;

(iii) Pour tout $j\in$ Orb(H), de flèches $c_1(j)$ et $c_2(j)$ de G reliant respectivement $\varphi (b(j))$ à $a(\varphi_0(j))$ et $\psi (b(j))$ à $a(\psi_0(j))$ ;

(iv) D’un sous-carquois T de l’armature $\Gamma_0$ dont le graphe associé est un arbre maximal du graphe $\widetilde{\Gamma}_0$;

(v) D’une orbite $i_0$ de G.

Choisissons un équipement de base $(a, b, c_1, c_2,T, i_0)$ du couple $(\varphi , \psi )$. On définit un morphisme de carquois $\tau_1$ de $\Gamma_0$ dans Grp(G$_1)$ en posant $\tau_1(i) =a(i)$ pour $i\in$ Som(Γ$_0) =$ Orb(G) et

$$
\tau_1(j) =c_1(j)^{-1}\cdot h_1(b(j))\cdot c_2(j)
$$

pour $j\in$ Fl(Γ$_0) =$ Orb(H). Nous noterons $\tau_0$ le composé de $\tau_1$ et du morphisme canonique $\theta_1$ de Grp(G$_1)$ dans Coh($\varphi , \psi$ ) ; c’est un morphisme de carquois de $\Gamma_0$ dans Coh($\varphi , \psi$ ).

Pour $i\in$ Orb(G), notons $\alpha_i: G_{a(i)}\rightarrow$ Coh($\varphi , \psi$ )$_{a(i)}$ l’homomorphisme de groupes déduit du morphisme $\alpha : G\rightarrow$ Coh($\varphi , \psi$ ) par restriction aux groupes d’isotropie en $a(i)$.

Pour $j\in$ Orb(H), notons

$\varphi_j=$ Int($c_1(j)$)$^{-1}\circ \varphi_{b(j)}: H_{b(j)}\rightarrow G_{a(\varphi_0(j))}$

et

$\psi_j=$ Int($c_2(j)$)$^{-1}\circ \psi_{b(j)}: H_{b(j)}\rightarrow G_{a(\psi_0(j))}$,

de sorte que l’on a, pour tout élément $f$ de $H_{b(j)}$,

(6) $\varphi_j(f) =c_1(j)^{-1}\varphi (f)c_1(j)$ et $\psi_j(f) =c_2(j)^{-1}\psi (f)c_2(j)$.

Pour tout sommet $i$ de $\Gamma_0$, notons encore $d_i$ l’unique classe de chemins reliant $i_0$ à $i$ dans l’arbre $\widetilde{T}$; on la considère comme une flèche de Grp(Γ$_0)$. Notons alors $\delta_i$ la flèche de Coh($\varphi , \psi$ ) image de $d_i$ par le morphisme canonique de Grp(Γ$_0)$ dans Coh($\varphi , \psi$ ) déduit de $\tau_0$; l’origine de $\delta_i$ est $a(i_0)$, son terme est $a(i)$.

Le morphisme de carquois $\tau_0$, les homomorphismes de groupes $\alpha_i$ (pour $i\in$ Orb(G)$),\varphi_j$ et $\psi_j$ (pour $j\in$ Orb(H)), et les flèches $\delta_i$ dans Coh($\varphi , \psi$ ) (pour $i\in$ Orb(G)) seront dits déduits de l’équipement de base.

Si $(G_i)_{i\in I}$ est une famille de groupes, on note $_i*_{\in I}G_i$ leur produit libre ; l’image d’un élément $g\in G_i$ par l’application canonique de $G_i$ dans $_i*_{\in I}G_i$ sera notée $[g]$, voire $g$ s’il n’y a pas de confusion possible. Si S est un ensemble, on note F(S) le groupe libre construit sur S (A, I, p. 84).

#### Proposition 6 {#ta-ii-s4-prop-6 .statement tag=01UH}

Il existe un unique homomorphisme de groupes

Λ: $*G_{a(i)}*$ F(Orb(H)) $\rightarrow$ Coh($\varphi , \psi$ )$_{a(i_0)}$

$i\in$Orb(G)

tel que

(7) $\Lambda (f) =\delta_i\alpha_i(f)\delta_i^{-1}$ pour $i\in$ Orb(G) et $f\in G_{a(i)}$,

(8) $\Lambda (j) =\delta_{\varphi_0(j)}\tau_0(j)\delta^{-1}_{\psi_0(j)}$ pour $j\in$ Orb(H).

L’homomorphisme Λ est surjectif ; son noyau est le plus petit sous-groupe distingué de $(*_iG_{a(i)})*$ F(Orb(H)) contenant les éléments $j$ de Fl(T) et les éléments $\varphi_j(f)j\psi_j(f)^{-1}j^{-1}$, pour $j\in$ Orb(H) et $f\in H_{b(j)}$.

L’existence et l’unicité de l’homomorphisme Λ résulte de la propriété universelle des produits libres et des groupes libres (A, I, p. 85, prop. 8).

Notons A l’ensemble des $a(i)$ pour $i\in$ Orb(G) et $G_A$ le sous-groupoïde plein de G dont l’ensemble des sommets est A. Pour tout $x\in$ Som(G), notons $\overline{x}$ l’orbite de $x$ dans G et choisissons une flèche $d_x$ de G reliant $x$ à $a(\overline{x})$. Le couple $v$ formé de l’application $x\mapsto a(\overline{x})$ de Som(G) dans A et de l’application qui à $f\in$ Fl$_{x,y}(G)$ associe l’élément $d^{-1}_xf d_y$ de Fl$_{a(\overline{x}),a(\overline{y})}(G_A)$ est un morphisme de groupoïdes. Il résulte de la prop. 1 de II, p. 182 que $v$ est un homotopisme. Notons $\varphi '=v\circ \varphi$ et $\psi '=v\circ \psi$, puis $w$ le morphisme canonique de Coh($\varphi , \psi$ ) dans Coh($\varphi ', \psi '$) ; c’est un homotopisme (II, p. 187, théorème 1).

Les orbites de $G_A$ sont les ensembles $\{a\}$, pour $a\in A$, et l’injection $G_A\rightarrow G$ induit une bijection de Orb(G$_A)$ sur Orb(G) par laquelle nous identifierons ces deux ensembles. On définit un équipement de base $(a', b', \beta '_1, \beta '_2,T', i_0)$ du couple $(\varphi ', \psi ')$ en posant $a'(i) =a(i)$ pour $i\in$ Orb(G)$,b'(j) =b(j),\beta '_1(j) =v(c_1(j)),\beta '_2(j) =v(c_2(j))$ pour $j\in$ Orb(H) et $T'= T$. Les homomorphismes de groupes $\varphi '_j$ et $\psi '_j$ (pour $j\in$ Orb(H)), le morphisme de carquois $\tau '_0$, les flèches $\delta '_i$ (pour $i\in$ Orb(G)), et donc l’homomorphisme de groupes $\Lambda '$, déduits de cet équipement de base sont les composés avec $w$ des homomorphismes correspondants $\varphi_j,\psi_j$, du morphisme de carquois $\tau_0$, des flèches correspondantes $\delta_i$ et de l’homomorphisme Λ.

Soit B l’ensemble des $b(j)$ pour $j\in$ Orb(H), soit $H_B$ le sous-groupoïde plein de H d’ensemble de sommets B ; notons $u: H_B\rightarrow H$ l’injection canonique ; posons $\varphi ''=\varphi '\circ u$ et $\psi ''=\psi '\circ u$. Le morphisme $u$ induit une bijection B $\rightarrow$ Orb(H) par laquelle nous identifierons ces deux ensembles. On déduit encore du théorème 1 de II, p. 187 un homotopisme canonique $w':$ Coh($\varphi '', \psi ''$)$\rightarrow$ Coh($\varphi ', \psi '$). En outre, le couple $(\varphi '', \psi '')$ est muni d’un équipement de base $(a'', b'', \beta ''_1, \beta ''_2,T'', i_0)$, de sorte que $\Lambda ', \varphi '_j, \psi '_j, \tau '_0, \delta '_i(i, i'\in$ Orb(G), $j\in$ Orb(H)) soient les composés avec $w'$ de $\Lambda '', \varphi ''_j, \psi ''_j, \tau ''_0, \delta ''_i$.

On résume par le diagramme suivant les divers morphismes de groupoïdes introduits :

$H_{B\psi''}^{\varphi''}G_A^{\alpha''}$ Coh($\varphi '', \psi ''$)

$w'$

(9) H $^{\varphi'}G_A^{\alpha'}$ Coh($\varphi '', \psi ''$)

$\psi '$

$$
vw
$$

H $^{\varphi}_{\psi}$ G $^{\alpha}$ Coh($\varphi , \psi$ ) .

Pour démontrer la proposition, on peut donc supposer que A = Som(G) et B = Som(H), autrement dit que les applications canoniques Som(G) $\rightarrow$ Orb(G) et Som(H) $\rightarrow$ Orb(H) sont bijectives, hypothèses sous lesquelles nous nous placerons dans la suite de la démonstration.

Le carquois $G_1$ a alors pour ensemble de sommets A et pour flèches l’ensemble somme des ensembles $G_a,a\in A$, et de l’ensemble B. Les flèches de $G_a$ sont des lacets en $a$; si $b\in B$, la flèche $b$ relie $\varphi (b)$ à $\psi (b)$, les flèches $c_1(b)$ et $c_2(b)$ sont des lacets respectivement en $\varphi (b)$ et $\psi (b)$. Le carquois T sera identifié à un arbre orienté de $G_1$; c’en est un arbre orienté maximal car l’ensemble de ses sommets est égal à l’ensemble des sommets de $G_1($II, p. 157, prop. 1). On posera $a_0=a(i_0)$. L’ensemble des flèches de l’armature $\Gamma_0$ du couple $(\varphi , \psi )$ étant identifié à B, le morphisme de carquois $\tau_1: \Gamma_0\rightarrow$ Grp(G$_1)$ associe à la flèche $b$ la classe de chemins $c_1(b)^{-1}bc_2(b)$ dans le graphe $\widetilde{G}_1$.

Rappelons que $\theta_1$ désigne le morphisme canonique de carquois de $G_1$ dans Grp(G$_1)$. Notons

$\lambda :_a*_{\in A}F(G_a)*F(B)\rightarrow$ Grp(G$_1)_{a_0}$

l’unique homomorphisme de groupes tel que l’on ait

$\lambda (f) =\tau_1(d_a)\theta_1(f)\tau_1(d_a)^{-1}$ si $a\in A$ et $f\in G_a$;

$\lambda (b) =\tau_1(d_{\varphi(b)})\tau_1(b)\tau_1(d_{\psi(b)})^{-1}$ si $b\in B$.

On a ainsi $\lambda =\lambda '\circ \varepsilon$, où $\lambda '$ désigne l’homomorphisme de groupes canonique de $_a*_{\in A}F(G_a)*F(B)$ dans Grp(G$_1)_{a_0}$ défini par l’arbre orienté maximal T (II, p. 179, prop. 9) et où $\varepsilon$ est l’unique automorphisme du groupe $_a*_{\in A}F(G_a)*F(B)$ tel que $\varepsilon (f) =f$ pour $a\in A$ et $f\in G_a$, et $\varepsilon (b) =c_1(b)^{-1}h_1(b)c_2(b)$ pour $b\in B$. D’après la remarque 2 de II, p. 179, l’homomorphisme $\lambda$ est surjectif et que son noyau est le plus petit sous-groupe distingué de $_a*_{\in A}F(G_a)*F(B)$ qui contient les flèches de T.

Notons $\pi :$ Grp(G$_1)\rightarrow$ Coh($\varphi , \psi$ ) le morphisme de groupoïdes canonique. D’après II, p. 177, cor. 1 de la prop. 8, le morphisme de groupes $\pi_{a_0}$ de Grp(G$_1)_{a_0}$ dans Coh($\varphi , \psi$ )$_{a_0}$ est surjectif, et son noyau est le plus petit sous-groupe distingué de Grp(G$_1)_{a_0}$ qui contient les lacets Int($\tau_1(d_a)$)$(\alpha_1(f)\alpha_1(g)\alpha_1(f g)^{-1})$, pour $a\in A$ et $f,g\in G_a$, et les lacets Int($\tau_1(d_{\varphi(b)})$)$(\varphi (f)b\psi (f)^{-1}b^{-1})$, pour $b\in B$ et $f\in H_b$.

Si $p: F(\bigcup G_a\cup B)\rightarrow_a*_{\in A}G_a*F(B)$ désigne l’homomorphisme surjectif canonique, on a ainsi $\Lambda \circ p=\pi_{a_0}\circ \lambda$. Cette formule entraîne que l’homomorphisme Λ est surjectif ; il reste à déterminer son noyau.

Pour $a\in A$ et $f\in G_a$, on note $[f]$ l’image de $f\in F(G_a)$ dans le groupe $_a*_{\in A}F(G_a)*F(B)$. Pour $a\in A,f, g\in G_a$, on a alors

Int($\tau_1(d_a)$)$(\alpha_1(f)\alpha_1(g)\alpha_1(f g)^{-1}) =\lambda ([f][g][f g]^{-1})$.

De même, pour $b\in B$ et $f\in H_b$, la définition des homomorphismes $\varphi_b$ et $\psi_b$ (formule (6) de II, p. 193) entraîne que l’on a

Int($\tau_1(d_{\varphi(b)})$)$(\varphi (f)h_1(b)\psi (f)^{-1}h_1(b)^{-1})$

$$
=\tau_1(d_{\varphi(b)})\varphi (f)c_1(b)\tau_1(b)c_2(b)^{-1}\psi (f)^{-1}
$$

$$
c_2(b)\tau_1(b)^{-1}c_1(b)^{-1}\tau_1(d_{\varphi(b)})^{-1}
$$

$$
=\tau_1(d_{\varphi(b)})c_1(b)\varphi_b(f)\tau_1(b)\psi_b(f)^{-1}\tau_1(b)^{-1}c_1(b)^{-1}\tau_1(d_{\varphi(b)})^{-1}
$$

$$
=\lambda (c_1(b))\lambda (\varphi_b(f)[b]\psi_b(f)^{-1}[b]^{-1})\lambda (c_1(b))^{-1}
$$

Par suite, le noyau de l’homomorphisme $\pi_{a_0}\circ \lambda$ est le plus petit sous-groupe distingué de $_a*_{\in A}F(G_a)*F(B)$ qui contient les éléments $[f][g][f g]^{-1}$ pour $a\in A$ et $f,g\in G_a$, les éléments $\varphi_b(f)[b]\psi_b(f)^{-1}[b]^{-1}$ pour $b\in B$ et $f\in H_b$, et les éléments $[b]$, pour $b\in$ Fl(T).

Finalement, le noyau de l’homomorphisme Λ est le plus petit sous-groupe distingué de $(_a*_{\in A}G_a)*F(B)$ qui contient les images par $p$ des éléments précédents, autrement dit, les éléments $[b]$, pour $b\in$ Fl(T), et les éléments $\varphi_b(f)[b]\psi_b(f)[b]^{-1}$, pour $b\in B$ et $f\in H_b$. La proposition est ainsi démontrée.
