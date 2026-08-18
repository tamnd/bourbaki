---
book: ts
book_title: Théories spectrales
chapter: I
chapter_title: ALGÈBRES NORMÉES
section: 6
section_title: Algèbres stellaires
lang: fr
source: ts-i-ii-fr
book_pages: TS I.95-TS I.127, TS I.180-TS I.187
pdf_pages: 0108-0140, 0193-0200
extraction: native
subsections:
    - "no": 1
      title: Involutions semi-linéaires
      page: 95
      pdf_page: 108
    - "no": 2
      title: Algèbres involutives
      page: 96
      pdf_page: 109
    - "no": 3
      title: Algèbres normées involutives
      page: 100
      pdf_page: 113
    - "no": 4
      title: Algèbres stellaires
      page: 102
      pdf_page: 115
    - "no": 5
      title: Algèbres stellaires commutatives
      page: 107
      pdf_page: 120
    - "no": 6
      title: Calcul fonctionnel dans les algèbres stellaires unifères
      page: 109
      pdf_page: 122
    - "no": 7
      title: Applications du calcul fonctionnel
      page: 112
      pdf_page: 125
    - "no": 8
      title: Calcul fonctionnel dans une algèbre non unifère
      page: 114
      pdf_page: 127
    - "no": 9
      title: Éléments positifs dans les algèbres stellaires
      page: 115
      pdf_page: 128
    - "no": 10
      title: Unités approchées dans les algèbres stellaires
      page: 120
      pdf_page: 133
    - "no": 11
      title: Quotient par un idéal bilatère fermé
      page: 122
      pdf_page: 135
    - "no": 12
      title: Algèbre stellaire enveloppante d’une algèbre de Banach involutive
      page: 123
      pdf_page: 136
    - "no": 13
      title: Algèbre stellaire d’un groupe localement compact
      page: 125
      pdf_page: 138
statements: 94
exercises: 32
content_sha256: 5e940fbc8c3e5ef356a38337e27dabf3b613bc4c7f6a5b5188ca811c50cafae6
---

## § 6. ALGÈBRES STELLAIRES

Dans ce paragraphe, le corps de base est $\mathbf{C}$.

### 1. Involutions semi-linéaires

Soit E un espace vectoriel complexe. Une involution semi-linéaire sur E est une application $\mathbf{R}$-linéaire de E dans E telle que $u\circ u=$ Id$_E$ et $u(\lambda x) =\lambda u(x)$ pour tout $\lambda \in \mathbf{C}$ et tout $x\in E$. On note alors $E^u$ le sous-espace vectoriel réel de E formé des éléments $x\in E$ tels que $u(x) =x$.

#### Lemme 1 {#ts-i-s6-lem-1 .statement tag=02CI}

Soient E un espace vectoriel complexe et $u$ une involution semi-linéaire sur E. Soit $x\in E$ ;posons

$$
x_1=\frac{1}{2}(x+u(x)),x_2=\frac{1}{2i}(x-u(x))
$$

Le couple $(x_1, x_2)$ est l’unique élément de $E^u\times E^u$ tel que $x=x_1+ix_2$.

Les éléments $x_1$ et $x_2$ vérifient $x_1+ix_2=x$ et appartiennent à $E^u$ puisque $u(u(x)) =x$. Inversement, si $y_1$ et $y_2$ dans $E^u$ vérifient $x=y_1+iy_2$, il vient $u(x) =u(y_1) +u(iy_2) =y_1-iy_2$, donc

$$
y_1=\frac{1}{2}(x+u(x)) =x_1,iy_2=\frac{1}{2}(x-u(x)) =ix_2
$$

#### Proposition 1 {#ts-i-s6-prop-1 .statement tag=02CJ}

Soient $E_1$ et $E_2$ des espaces vectoriels complexes, et soient $u_1$ et $u_2$ des involutions semi-linéaires sur $E_1$ et $E_2$ respectivement. Soit $f$ une application linéaire de $E_1$ dans $E_2$. Alors $f\circ u_1=u_2\circ f$ si et seulement si $f(E^{u_1}_1)\subset E^{u_2}_2$.

Si $f\circ u_1=u_2\circ f$, on obtient aussitôt $f(E^{u_1}_1)\subset E^{u_2}_2$. Inversement, supposons que cette condition est satisfaite. Soit $x\in$ E. Écrivons $x=x_1+ix_2$ avec $(x_1, x_2)\in E^{u_1}_1\times E^{u_1}_1$ (lemme ci-dessus). On a alors $f(u_1(x)) =f(x_1)-if(x_2)$ et $u_2(f(x)) =u_2(f(x_1))-iu_2(f(x_2)) =$ $f(x_1)-if(x_2) =f(u_1(x))$.

### 2. Algèbres involutives

#### Définition 1 {#ts-i-s6-def-1 .statement tag=02CK}

Soit A une algèbre sur $\mathbf{C}$. On appelle involution dans A une application $x\mapsto x^*$ de A dans A telle que :

$$
(x^*)^*=x,(x+y)^*=x^*+y^*,(\lambda x)^*=\lambda x^*
$$

$$
(xy)^*=y^*x^*
$$

quels que soient $x, y\in A$ et $\lambda \in \mathbf{C}$. Une algèbre sur $\mathbf{C}$ munie d’une involution est appelée une algèbre involutive.

Une involution sur A est en particulier un isomorphisme de l’anneau A sur l’anneau opposé $A^{\circ}$.

Soit A une algèbre involutive. On dit que $x^*$ est l’adjoint de $x$. Une partie de A stable pour l’involution est dite auto-adjointe. Si A possède un élément unité $e$, on a $e^*=e$; on dit que $(A, e)$ est une algèbre unifère involutive. Un élément $u$ d’une algèbre unifère involutive est dit unitaire si $uu^*=u^*u=e$, autrement dit si $u$ est inversible et si son inverse est $u^*$.

Un élément $x\in A$ est dit hermitien si $x=x^*$ et normal si $xx^*=$ $x^*x$. Cette terminologie généralise celle de A, IX, § 7, n$^o3$. Tout élément hermitien est normal, tout élément unitaire est normal. L’ensemble $A_h$ des éléments hermitiens de A est un sous-espace vectoriel réel de A. Si $x$ et $y$ sont hermitiens et permutables, on a $(xy)^*$ = $y^*x^*=yx=xy$, donc $xy$ est hermitien. Pour tout $x\in A$, les éléments $xx^*$ et $x^*x$ de A sont hermitiens.

Si $A =\mathbf{C}$ muni de l’involution $z\mapsto \overline{z}$, on a $A_h=\mathbf{R}$.

#### Lemme 2 {#ts-i-s6-lem-2 .statement tag=02CL}

Soient A une algèbre involutive et $x\in A$. Les éléments

$$
x_1=\frac{1}{2}(x+x^*),x_2=\frac{1}{2i}(x-x^*)
$$

sont hermitiens et vérifient $x=x_1+ix_2$. Si $x=y_1+iy_2$ avec $y_1$ et $y_2$ hermitiens, alors $x_1=y_1$ et $x_2=y_2$. De plus, l’élément $x$ est normal si et seulement si $x_1$ et $x_2$ sont permutables.

Les deux premières assertions résultent du lemme 1 de I, p. 95. On calcule que $xx^*-x^*x= 2i(x_2x_1-x_1x_2)$, donc $x$ est normal si et seulement si $x_1$ et $x_2$ sont permutables.

Soit A une algèbre unifère involutive. Pour que $x\in A$ soit inversible, il faut et il suffit que $x^*$ le soit, et on a alors $(x^*)^{-1}= (x^{-1})^*$. Comme (Sp$x_A-(x\lambda e)$.$)^*=x^*-\lambda e$ pour tout $\lambda \in \mathbf{C}$, on en déduit que Sp$_A(x^*) =$

Soient A une algèbre involutive et $\widetilde{A}$ l’algèbre déduite de A par adjonction d’un élément unité. Il existe dans $\widetilde{A}$ une unique involution prolongeant celle de A, donnée par $(\lambda , x)^*= (\lambda , x^*)$ pour $\lambda \in \mathbf{C}$ et $x\in A$. Si $x\in A$, on a Sp$'_A(x^*) =$ Sp$'_A(x)$.

Soient A et B des algèbres involutives. On appelle morphisme de A dans B un morphisme d’algèbres $\varphi$ de A dans B tel que $\varphi (x^*) =\varphi (x)^*$ quels que soient $x$ et $y$ dans A. L’application identique de A est un morphisme d’algèbres involutives. Si C est une algèbre involutive et $\pi : B\rightarrow C$ un morphisme d’algèbres involutives, alors $\pi \circ \varphi$ est un morphisme d’algèbres involutives. Si $\varphi$ est un isomorphisme d’algèbres, alors $\varphi^{-1}$ est un morphisme d’algèbres involutives, et on dit que $\varphi$ est un isomorphisme d’algèbres involutives.

D’après la prop. 1 de I, p. 95, si A et B sont des algèbres involutives, un morphisme d’algèbres $\varphi$ de A dans B est un morphisme d’algèbres involutives si et seulement si $\varphi (A_h)\subset B_h$. On appelle sous-algèbre involutive de A une sous-algèbre auto-adjointe. Le centre de A est une sous-algèbre involutive. Si $A_1$ est un idéal bilatère auto-adjoint de A, l’involution de A définit par passage au quotient une involution dans l’algèbre $A/A_1$, et l’application canonique de A sur $A/A_1$ est un morphisme d’algèbres involutives.

Soit A une algèbre involutive. Le radical de A est égal au radical de l’algèbre opposée (A, VIII, p. 431, prop. 7), et est donc auto-adjoint.

Soit A une algèbre involutive. Si $M\subset A$ est auto-adjoint, son commutant $M'$ est une sous-algèbre involutive de A. Si $x\in A$, le bicommutant de $\{x, x^*\}$ est une sous-algèbre involutive contenant $x$ et $x^*$, et cette sous-algèbre est commutative si et seulement si $x$ est normal (n$^o5$ de I, p. 5).

#### Remarque {#ts-i-s6-n2-rem-1 .statement tag=02CM}

Soient A une algèbre involutive et B une sous-algèbre involutive commutative maximale de A. Alors B est une sous-algèbre commutative maximale. En particulier, si A est unifère, alors l’algèbre B est pleine.

En effet, soit $x\in A$ un élément permutable à B. Alors $x^*$ est permutable à B. Écrivons $x=x_1+ix_2$ avec $x_1$ et $x_2$ hermitiens ; les éléments $x_1$ et $x_2$ sont permutables à B (lemme 2). La sous-algèbre de A engendrée par B et $x_1$ est donc commutative et involutive. Par conséquent, elle est égale à B, de sorte que $x_1\in B$. De même, on a $x_2\in B$, et donc finalement $x\in B$.

Soit A une algèbre involutive. Si $f$ est une forme linéaire sur A, l’application $x\mapsto \overline{f(x^*)}$ sur A est une forme linéaire sur A, que l’on note $f^*$. L’application $f\mapsto f^*$ est une involution semi-linéaire sur $A'$. On dit que $f$ est hermitienne si $f=f^*$. D’après le lemme 1 de I, p. 95, toute forme linéaire $f$ sur A a une unique représentation $f=f_1+if_2$ où $f_1$ et $f_2$ sont hermitiennes, à savoir $f_1=\frac{1}{2}(f+f^*)$ et $f_2=\frac{1}{2i}(f-f^*)$.

Pour qu’une forme linéaire $f$ soit hermitienne, il faut et il suffit que la restriction de $f$ à $A_h$ soit à valeurs réelles (proposition 1 de I, p. 95). L’application $f\mapsto f|A_h$ est un isomorphisme de l’espace vectoriel réel des formes hermitiennes sur l’espace vectoriel dual de l’espace vectoriel réel $A_h$.

En particulier, on notera $\mathsf{X}'(A)_h$ (resp. $\mathsf{X}(A)_h)$ l’ensemble des caractères hermitiens de A (resp. l’ensemble des caractères hermitiens non nuls de A). Un caractère est donc hermitien si sa restriction à $A_h$ est à valeurs réelles.

Si A est commutative et si $\chi$ est un caractère de A, alors $\chi^*$ est un caractère de A, et l’application $\chi \mapsto \chi^*$ est un homéomorphisme de $\mathsf{X}'(A)$ sur $\mathsf{X}'(A)$.

#### Lemme 3 {#ts-i-s6-lem-3 .statement tag=02CN}

Soit A une algèbre involutive commutative. La transformation de Gelfand de A dans $\mathscr{C}_0(\mathsf{X}(A))$ est un morphisme d’algèbres involutives si et seulement si tout caractère de A est hermitien.

En effet, dire que $\mathscr{G}_A$ est un morphisme d’algèbres involutives revient à dire que, pour tous $x\in A$ et $\chi \in \mathsf{X}(A)$, on a

$$
\chi (x^*) =\mathscr{G}_A(x^*)(\chi ) =\mathscr{G}_A(x)(\chi ) =\overline{\chi(x)}
$$

c’est-à-dire que tout $\chi$ est hermitien.

#### Exemple 1 {#ts-i-s6-n2-exa-1 .statement tag=02CO}

Soit A l’algèbre des fonctions à valeurs complexes sur un ensemble X. L’application $f\mapsto \overline{f}$ est une involution dans A. La sous-algèbre des fonctions bornées dans X est une sous-algèbre involutive de A. Si X est un espace topologique localement compact, les sous-algèbres $\mathscr{C}(X),\mathscr{C}_b(X),\mathscr{C}_0(X)$ et $\mathscr{K}(X)$ sont des sous-algèbres involutives de A.

#### Exemple 2 {#ts-i-s6-n2-exa-2 .statement tag=02CP}

Soient X un espace topologique localement compact et $\mu$ une mesure positive sur X. L’application $f\mapsto \overline{f}$ est une involution sur l’algèbre $\mathscr{L}^{\infty}(X, \mu)$ ; elle induit par passage au quotient une involution sur l’algèbre unifère $L^{\infty}(X, \mu)$.

#### Exemple 3 {#ts-i-s6-n2-exa-3 .statement tag=02CQ}

Soit E un espace hilbertien complexe. Sur l’algèbre de Banach $\mathscr{L}(E)$, l’application $x\mapsto x^*$ (EVT, V, p. 37, prop. 1) est une involution.

#### Exemple 4 {#ts-i-s6-n2-exa-4 .statement tag=02CR}

Soit G un groupe localement compact. Soit $\mathscr{M}^1(G)$ l’algèbre de Banach des mesures bornées complexes sur G (exemple 6 de I, p. 19).

L’application $x\mapsto x^{-1}$ de G sur G transforme toute mesure $\mu\in$ $\mathscr{M}^1(G)$ en une mesure $\check{\mu}\in \mathscr{M}^1(G)$ (INT, VII, p. 12, formule (13)). On note $\mu^*$ la mesure complexe conjuguée de $\check{\mu}$. L’application $\mu\mapsto \check{\mu}$ est un isomorphisme isométrique de l’algèbre de Banach $\mathscr{M}^1(G)$ sur l’algèbre de Banach $\mathscr{M}^1(G^{\circ})$ (INT, VIII, §3, n$^o1$, cor. de la prop. 7) donc $\mu\mapsto \mu^*$ est une involution isométrique de l’algèbre de Banach $\mathscr{M}^1(G)$.

L’ensemble A des mesures bornées admettant une densité par rapport à une mesure de Haar est une sous-algèbre fermée de $\mathscr{M}^1(G)$ stable par l’involution (cf. INT, VIII, §4, n$^o5)$; elle ne dépend pas du choix d’une mesure de Haar.

Soit $\nu$ une mesure de Haar à gauche sur G et notons Δ le module devolution$Gf$. On munit$\mapsto f^*=\widetilde{f}L\overset{1}{\cdot}(G\Delta^-, \nu^1$, où) du produit$\widetilde{f}(x) =\frac{(f, g)}{f(x^{-1})}\mapsto$pour tout$f*^{\nu}g$ et de l’in-$x\in G$. Alors l’application $f\mapsto f\cdot \nu$ est un isomorphisme de l’algèbre involutive $L^1(G, \nu )$ sur A. Cet isomorphisme est isométrique. En particulier, $L^1(G, \nu )$ s’identifie à une sous-algèbre involutive de $\mathscr{M}^1(G)$.

#### Exemple 5 {#ts-i-s6-n2-exa-5 .statement tag=02CS}

Soit U une partie ouverte de $\mathbf{C}$ stable par la conjugaison complexe. Considérons l’algèbre $\mathscr{O}(U)$ des fonctions holomorphes à valeurs complexes sur U. Pour toute fonction $f\in \mathscr{O}(U)$, l’application $f^*:z\mapsto f(\overline{z})$ est une fonction holomorphe sur U. L’application $f\mapsto f^*$ est une involution sur $\mathscr{O}(U)$.

Similairement, soit S une partie compacte de $\mathbf{C}$ stable par la conjugaison complexe. Considérons l’algèbre $\mathscr{O}(S)$ des germes de fonctions holomorphes à valeurs complexes au voisinage de S. L’application $f\mapsto f^*$ est une involution sur $\mathscr{O}(S)$.

La sous-algèbre $\mathscr{O}_{\mathbf{R}}(U)$ (resp. la sous-algèbre $\mathscr{O}_{\mathbf{R}}(S)$) définie dans le n$^o13$ de I, p. 85 est l’ensemble des éléments hermitiens de $\mathscr{O}(U)$ (resp. de $\mathscr{O}(S)$).

### 3. Algèbres normées involutives

#### Définition 2 {#ts-i-s6-def-2 .statement tag=02CT}

On appelle algèbre normée involutive une algèbre normée A munie d’une involution $x\mapsto x^*$ telle que $\|x^*\|=\|x\|$ pour tout $x$. Si A est une algèbre de Banach, on dit que A est une algèbre de Banach involutive.

#### Exemple 1 {#ts-i-s6-n3-exa-1 .statement tag=02CU}

Soit X un espace topologique localement compact. L’algèbre de Banach $\mathscr{C}_b(X)$ des fonctions complexes continues et bornées sur X, munie de la norme $\|f\|$ = sup$_{x\in X}|f(x)|$ et de l’involution $f\mapsto \overline{f}$, est une algèbre de Banach involutive. La sous-algèbre $\mathscr{C}_0(X)$ des fonctions continues tendant vers 0 à l’infini est une sous-algèbre involutive fermée de $\mathscr{C}_b(X)$.

#### Exemple 2 {#ts-i-s6-n3-exa-2 .statement tag=02CV}

Soient X un espace topologique localement compact et $\mu$ une mesure positive sur X. L’algèbre involutive $L^{\infty}(X, \mu)$ (exemple 2 de I, p. 99) est une algèbre de Banach involutive, puisque $|f|=|\overline{f}|$ pour tout élément $f\in L^{\infty}(X, \mu)$.

#### Exemple 3 {#ts-i-s6-n3-exa-3 .statement tag=02CW}

L’algèbre involutive $\mathscr{L}(E)$ des endomorphismes continus d’un espace hilbertien complexe E (I, p. 99, exemple 3), munie de la norme

$\|u\|=$ sup$_{\|xx\in\|\leqslant E1}\|u(x)\|$

(EVT, III, p. 14) est une algèbre de Banach involutive (EVT, V, p. 37, prop. 1).

#### Exemple 4 {#ts-i-s6-n3-exa-4 .statement tag=02CX}

L’algèbre involutive $\mathscr{M}^1(G)$ des mesures bornées sur un groupe localement compact (I, p. 99, exemple 4), munie de la norme usuelle (exemple 6 de I, p. 19), est une algèbre de Banach involutive. Soit $\nu$ une mesure de Haar à gauche sur G. L’algèbre de Banach involutive $L^1(G, \nu )$ s’identifie à une sous-algèbre fermée de $\mathscr{M}^1(G)$.

#### Exemple 5 {#ts-i-s6-n3-exa-5 .statement tag=02CY}

Soit $(A_i)$ une famille d’algèbres normées involutives. Soit A l’algèbre normée produit des $A_i$ (n$^o1$ de I, p. 15). L’algèbre A, munie de l’involution $(x_i)^*= (x^*_i)$, est une algèbre normée involutive. Si chacune des algèbres $A_i$ est une algèbre de Banach involutive, alors A est une algèbre de Banach involutive. On dit que A est l’algèbre normée involutive (resp. l’algèbre de Banach involutive) produit des $A_i$.

#### Exemple 6 {#ts-i-s6-n3-exa-6 .statement tag=02CZ}

Soit A une algèbre normée involutive et soit $\widetilde{A}$ l’algèbre normée déduite de A par adjonction d’un élément unité. Munie de l’involution définie au n$^o2$, l’algèbre $\widetilde{A}$ est une algèbre normée involutive. Si A est une algèbre de Banach involutive, alors $\widetilde{A}$ est également une algèbre de Banach involutive.

Si A est une algèbre normée involutive, l’adhérence d’une sous-algèbre involutive est une sous-algèbre involutive. Si $M\subset A$, la plus petite sous-algèbre fermée involutive contenant M est appelée la sous-algèbre fermée involutive engendrée par M ; c’est l’adhérence de la sous-algèbre engendrée par $M\cup M^*$. Si M se réduit à un élément normal, l’algèbre fermée involutive engendrée par M est commutative, et tous ses éléments sont normaux.

De même, si A est une algèbre normée involutive unifère et M un sous-ensemble de A, la plus petite sous-algèbre unifère fermée involutive contenant M est appelée la sous-algèbre unifère fermée involutive engendrée par M ; c’est l’adhérence de la sous-algèbre unifère engendrée par $M\cup M^*$. Si M se réduit à un élément normal, l’algèbre unifère fermée involutive engendrée par M est commutative, et tous ses éléments sont normaux.

Le quotient d’une algèbre normée involutive par un idéal bilatère fermé auto-adjoint, la complétée et l’opposée d’une algèbre normée involutive sont de façon naturelle des algèbres normées involutives.

Si A est une algèbre normée involutive, l’ensemble $A_h$ des éléments hermitiens de A est un espace vectoriel réel normé.

#### Lemme 4 {#ts-i-s6-lem-4 .statement tag=02D0}

Soit A une algèbre normée involutive. Pour toute forme linéaire $f$ continue sur A, on a $\|f^*\|=\|f\|$. Si de plus $f$ est hermitienne, alors $\|f\|=\|f|A_h\|$.

La première assertion découle des définitions. Pour la seconde, notons $g$ la restriction de $f$ à $A_h$. On a $\|f\|\geqslant \|g\|$. Montrons l’inégalité réciproque. Pour tout $\varepsilon  >$ 0, il existe $x\in$ A tel que $\|x\|\leqslant 1$ et $|f(x)|\geqslant \|f\| -\varepsilon$. En multipliant $x$ par un nombre complexe de module 1, on peut supposer $f(x)\geqslant 0$. Alors l’élément $\frac{1}{2}(x+x^*)$ appartient à $A_h$ et est de norme $\leqslant 1$. On a

$|(1_*)|$ 1 $*$

$$
g(x+x)|=|f(x) +f(x)|=f(x)\geqslant \|f\| -\varepsilon
$$

2 2

donc $\|g\|\geqslant \|f\| -\varepsilon$. On en déduit que $\|g\|\geqslant \|f\|$.

On identifiera dans la suite les formes linéaires continues hermitiennes sur A et les formes linéaires continues réelles sur $A_h$.

#### Lemme 5 {#ts-i-s6-lem-5 .statement tag=02D1}

Soit A une algèbre de Banach involutive.

a) Pour tout $x\in A$, on a exp($x$)$^*=$ exp($x^*$) ;

b) Soit $x\in A_h$ un élément hermitien. Alors exp($ix$) est unitaire.

En effet, puisque l’involution sur A est continue, on a

exp($x$)$^*=(\sum_{n=0}^{\infty}xn^n$! $)^*=\sum_{n=0}^{\infty}(x\overset{*}{n}$!$)^n=$ exp($x^*$)

pour tout $x\in A$ (formule (9) de I, p. 78). Si $x\in A_h$, il vient alors

exp($ix$)$^*=$ exp(($ix$)$^*) =$ exp($-ix$) $=$ exp($ix$)$^{-1}$

(formule (11) de I, p. 78).

### 4. Algèbres stellaires

#### Définition 3 {#ts-i-s6-def-3 .statement tag=02D2}

On appelle algèbre stellaire une algèbre de Banach involutive A telle que $\|x\|^2=\|x^*x\|$ pour tout $x\in A$.

Si A et B sont des algèbres stellaires, un morphisme, ou morphisme d’algèbres stellaires, de A dans B est un morphisme d’algèbres involutives de A dans B. Un isomorphisme de A dans B est un isomorphisme d’algèbres involutives de A dans B.

Certains auteurs parlent de « $C^*$-algèbre ».

Soit A une algèbre stellaire. Une sous-algèbre stellaire de A est une sous-algèbre involutive fermée de A.

#### Exemple 1 {#ts-i-s6-n4-exa-1 .statement tag=02D3}

L’algèbre de Banach involutive des endomorphismes continus d’un espace hilbertien complexe (exemple 3 de I, p. 100) est une algèbre stellaire (EVT, V, p. 39, prop. 2).

#### Exemple 2 {#ts-i-s6-n4-exa-2 .statement tag=02D4}

Soit X un espace topologique localement compact. L’algèbre de Banach involutive $\mathscr{C}_b(X)$ des fonctions continues et bornées à valeurs complexes sur X (exemple 1 de I, p. 100) est une algèbre stellaire. En effet, pour toute fonction $f\in \mathscr{C}_b(X)$, on a $f^*f=|f|^2$, et donc $\|f^*f\|=\||f|^2\|=\|f\|^2$.

Soit $A =\mathscr{C}_0(X)$ la sous-algèbre de Banach involutive des fonctions tendant vers 0 à l’infini. C’est une sous-algèbre stellaire de $\mathscr{C}_b(X)$. Pour toute fonction $f\in A$, on a $\|f\|=\varrho (f)$, puisque Sp$'_A(f) =f(X)\cup  \{0\}$.

Soient X et Y des espaces topologiques localement compacts. Pour toute application partielle propre $\varphi$ de X dans Y (déf. 1 de I, p. 33), le morphisme d’algèbres $\varphi^*$ de $\mathscr{C}_0(Y)$ dans $\mathscr{C}_0(X)$ (prop. 3 de I, p. 34) est un morphisme d’algèbres involutives. Réciproquement, tout morphisme d’algèbres stellaires $\pi :\mathscr{C}_0(Y)\rightarrow \mathscr{C}_0(X)$ est de cette forme (loc. cit.).

#### Exemple 3 {#ts-i-s6-n4-exa-3 .statement tag=02D5}

Soient X un espace topologique compact et $x_0\in X$ un élément fixé de X. La sous-algèbre $\mathscr{C}'(X)$ de $\mathscr{C}(X)$ des fonctions continues $f: X\rightarrow$ $\mathbf{C}$ telles que $f(x_0) = 0$ est une algèbre stellaire.

#### Exemple 4 {#ts-i-s6-n4-exa-4 .statement tag=02D6}

Soient X un espace topologique séparé et $\mu$ une mesure positive sur X. L’algèbre de Banach involutive $L^{\infty}(X, \mu)$ est une algèbre stellaire commutative unifère.

#### Exemple 5 {#ts-i-s6-n4-exa-5 .statement tag=02D7}

Soit $(A_i)$ une famille d’algèbres stellaires. L’algèbre de Banach involutive A produit des $A_i$ (exemple 5 de I, p. 101) est une algèbre stellaire, appelée algèbre stellaire produit des $A_i$.

#### Exemple 6 {#ts-i-s6-n4-exa-6 .statement tag=02D8}

Soit A une algèbre stellaire. Si B est une sous-algèbre involutive fermée de A, alors B est une algèbre stellaire. On verra (V, à paraître) que toute algèbre stellaire est isomorphe à une sous-algèbre involutive fermée de l’algèbre stellaire des endomorphismes d’un espace hilbertien (exemple 1).

#### Exemple 7 {#ts-i-s6-n4-exa-7 .statement tag=02D9}

Soit A une algèbre stellaire. Si $M\subset A$ est une partie quelconque, alors la sous-algèbre fermée involutive de A engendrée par M est une algèbre stellaire, appelée sous-algèbre stellaire de A engendrée par M. Si A est de plus unifère, alors la sous-algèbre unifère fermée involutive engendrée par M est une algèbre stellaire unifère, appelée sous-algèbre stellaire unifère de A engendrée par M.

#### Exemple 8 {#ts-i-s6-n4-exa-8 .statement tag=02DA}

En général, l’algèbre de Banach involutive $\mathscr{M}^1(G)$ (exemple 4 de I, p. 100) n’est pas une algèbre stellaire (I, p. 181, exerc. 8).

#### Lemme 6 {#ts-i-s6-lem-6 .statement tag=02DB}

Soit A une algèbre de Banach munie d’une involution vérifiant

$$
\|x\|^2\leqslant \|x^*x\| \tag{1}
$$

pour tout $x\in A$. Alors A est une algèbre stellaire.

Soit $x\in A$. On a alors $\|x\|^2\leqslant \|x^*\| \cdot  \|x\|$, d’où $\|x\|\leqslant \|x^*\|$. En échangeant le rôle de $x$ et $x^*$, on voit que $\|x\|=\|x^*\|$. Ainsi $\|x^*x\|\leqslant$ $\|x^*\|\|x\|\leqslant \|x\|^2$ et l’hypothèse implique l’égalité $\|x\|^2=\|x^*x\|$.

#### Lemme 7 {#ts-i-s6-lem-7 .statement tag=02DC}

Soit A une algèbre stellaire.

a) La représentation regulière $\boldsymbol{\gamma }$ de A (déf. 1 de I, p. 16) est isométrique, c’est-à-dire

$\|x\|=$ sup$_{\|y\|\leqslant 1}\|xy\|$,

pour tout $x\in A$ ;

b) Pour tout $x\in A_h$, on a

$$
\varrho (x) =\|x\| \tag{2}
$$

Soit $x\in A$. On a sup$_{\|y\|\leqslant 1}\|xy\|\leqslant \|x\|$. Pour prouver que $\|x\|\leqslant$ sup$_{\|y\|\leqslant 1}\|xy\|$, on peut supposer $\|x\|= 1$. Alors, l’élément $y$ = $x^*$ vérifie $\|y\|=\|x^*\|= 1$, et $\|xy\|=\|x\|^2= 1$, d’où l’assertion a).

Supposons que $x$ est hermitien. Il vient $\|x^2\|=\|x^*x\|=\|x\|^2$, d’où par récurrence $\|x^{2^n}\|^{2^{-n}}=\|x\|$ pour tout entier $n\geqslant 1$, d’où l’assertion b) d’après la prop. 1 de I, p. 20.

#### Remarque 1 {#ts-i-s6-n4-rem-1 .statement tag=02DD}

Soit A une algèbre stellaire unifère. On a

$$
\|1\|^2=\|1^*1\|=\|1\|
$$

donc la norme $\|1\|$ est nulle ou égale à 1. Si $A\not=\{0\}$, on en déduit $\|1\|= 1$. Par suite, pour tout élément unitaire $u$ de A, on a $\|u\|=$ $\|u^*u\|^{1/2}= 1$.

#### Remarque 2 {#ts-i-s6-n4-rem-2 .statement tag=02DE}

Soit A une algèbre normée involutive. Si $\|x\|^2=\|x^*x\|$ pour tout $x\in A$, la complétée $\widehat{A}$ de A est une algèbre stellaire.

#### Proposition 2 {#ts-i-s6-prop-2 .statement tag=02DF}

Soit A une algèbre de Banach involutive, soit B une algèbre stellaire et soit $\pi$ un morphisme d’algèbres involutives de A dans B. On a $\|\pi (x)\|\leqslant \|x\|$ pour tout $x\in A$, et en particulier $\pi$ est continu.

Pour tout $x\in A$, on a Sp$'_B(\pi (x))\subset$ Sp$'_A(x)$, donc $\varrho (\pi (x))\leqslant \varrho (x)\leqslant$ $\|x\|$. Comme $\pi (x^*x)\in B_h$, on a $\|\pi (x^*x)\|=\varrho (\pi (x^*x))$ (formule (2)), donc

$$
\|\pi (x)\|^2=\|\pi (x^*x)\|=\varrho (\pi (x^*x))\leqslant \|x^*x\|=\|x\|^2
$$

#### Proposition 3 {#ts-i-s6-prop-3 .statement tag=02DG}

Soit A une algèbre stellaire et soit $\widetilde{A}$ l’algèbre involutive déduite de A par adjonction d’un élément unité. Il existe une unique norme sur $\widetilde{A}$ prolongeant celle de A et faisant de $\widetilde{A}$ une algèbre stellaire.

L’unicité d’une telle norme résulte de la prop. 2. Montrons maintenant son existence. Notons $\widetilde{e}$ l’élément unité de $\widetilde{A}$.

Supposons d’abord que A possède un élément unité $e$. Le produit des algèbres normées involutives A et $\mathbf{C}(\widetilde{e}-e)$ s’identifie à $\widetilde{A}$ et est une algèbre stellaire (exemple 5). La norme sur $\widetilde{A}$ prolonge celle de A, d’où l’assertion.

Supposons désormais que A ne possède pas d’élément unité. Pour tout $x\in \widetilde{A}$, soit $\boldsymbol{\gamma }_x$ l’opérateur de multiplication $y\mapsto xy$ de A dans A, et posons $\|x\|_{\widetilde{A}}=\|\boldsymbol{\gamma }_x\|$. L’application $x\mapsto  \|x\|_{\widetilde{A}}$ est une semi-norme sur $\widetilde{A}$. Pour tous $x$ et $x'$ de $\widetilde{A}$, on a $\|xx'\|_{\widetilde{A}}\leqslant \|x\|_{\widetilde{A}}\|x'\|_{\widetilde{A}}$. De plus, d’après le lemme 7, on a $\|x\|_{\widetilde{A}}=\|x\|$ pour tout $x\in A$.

Montrons que l’application $x\mapsto  \|x\|_{\widetilde{A}}$ est une norme sur $\widetilde{A}$. Soient $\lambda \in \mathbf{C}$ et $x\in A$ tels que $\|\lambda \widetilde{e}+x\|_{\widetilde{A}}$ = 0. Si $\lambda \not= 0$, la condition $(\lambda \widetilde{e}+x)y= 0$ pour tout $y\in A$ implique que $-\lambda^{-1}x$ est un élément unité à gauche dans A. De même, l’élément $-\overline{\lambda}^{-1}x^*$ est un élément unité à droite. Ainsi, l’algèbre A possèderait alors un élément unité, contrairement à l’hypothèse. On a donc $\lambda = 0$. Mais alors $0 =\|x\|_{\widetilde{A}}=$ $\|x\|$, et donc $x= 0$.

Comme A est complet et de codimension 1 dans $\widetilde{A}$, l’espace $\widetilde{A}$ muni de la norme $x\mapsto  \|x\|_{\widetilde{A}}$ est complet. Pour conclure, il est donc suffisant de montrer que l’on a $\|x\|^2_{\widetilde{A}}\leqslant \|x^*x\|_{\widetilde{A}}$ pour tout $x\in \widetilde{A}$ (lemme 6). On peut supposer que $\|x\|_{\widetilde{A}}= 1$. Pour tout nombre réel $r <1$, il existe donc $y\in A$ tel que $\|y\|=\|y^*\|\leqslant 1$ et $\|xy\|^2\geqslant r$. Comme $xy\in A$, on a

$$
\|x^*x\|_{\widetilde{A}}\geqslant \|x^*xy\|\geqslant \|y^*(x^*x)y\|=\|(xy)^*(xy)\|=\|xy\|^2\geqslant r
$$

On en déduit que $\|x^*x\|_{\widetilde{A}}\geqslant 1$, et donc l’algèbre involutive $\widetilde{A}$ munie de la norme $x\mapsto  \|x\|_{\widetilde{A}}$ est une algèbre stellaire.

#### Définition 4 {#ts-i-s6-def-4 .statement tag=02DH}

On dit que $\widetilde{A}$, munie de la norme de la prop. 3, est l’algèbre stellaire déduite de A par adjonction d’un élément unité.

Lorsque $A\not=\{0\}$, la norme d’algèbre stellaire sur l’algèbre normée involutive $\widetilde{A}$ n’est pas celle considérée dans l’exemple 6 de I, p. 101 (cf. exercice 10 de I, p. 181).

#### Proposition 4 {#ts-i-s6-prop-4 .statement tag=02DI}

Soit A une algèbre stellaire.

a) Si A possède un élément unité et si $u$ est un élément unitaire de A, alors Sp($u$)$\subset \mathbf{U}$;

b) Si $h$ est un élément hermitien de A, alors Sp$'(h)\subset \mathbf{R}$.

On peut supposer que A est non nulle. Démontrons l’assertion a). Soit $u$ un élément unitaire de A. On a $\|u\|=\|u^{-1}\|= 1$ (remarque 1), donc Sp($u$)$\subset \mathbf{U}($I, p. 26, cor. 3). Pour démontrer b), on peut supposer que A est unifère (prop. 3). Soit $h$ un élément hermitien de A. Alors exp($ih$) est unitaire (lemme 5 de I, p. 102). Ainsi, d’après le cor. 2 de I, p. 67 et a), on a exp($i$ Sp($h$)) $=$ Sp(exp($ih$))$\subset \mathbf{U}$, ce qui signifie que Sp($h$)$\subset \mathbf{R}$.

#### Proposition 5 {#ts-i-s6-prop-5 .statement tag=02DJ}

Soient A une algèbre stellaire unifère et B une sous-algèbre stellaire de A contenant l’élément unité de A. Alors B est une sous-algèbre pleine de A. En particulier, on a Sp$_B(x) =$ Sp$_A(x)$ pour tout $x$ dans B.

Soit $x$ un élément hermitien de B. Comme Sp$_B(x)\subset \mathbf{R}$ (prop. 4), la prop. 6 de I, p. 28 montre que Sp$_B(x) =$ Sp$_A(x)$. En particulier, $x$ est inversible dans B si et seulement si il est inversible dans A.

Soit maintenant $x$ un élément quelconque dans B inversible dans A. Alors $x^*$ est inversible dans A, et $xx^*$ est inversible dans A. Comme $xx^*$ est hermitien, ce qui précède montre que $xx^*$ est inversible dans B. Cela implique que $x$ est inversible à droite dans B. De même, on vérifie que $x$ est inversible à gauche dans B, et par suite que $x$ est inversible dans B. Ainsi, B est une sous-algèbre pleine de A.

#### Corollaire {#ts-i-s6-n4-cor-1 .statement tag=02DK}

Soit A une algèbre stellaire et soit B une sous-algèbre stellaire de A. Alors on a Sp$'_B(x) =$ Sp$'_A(x)$ pour tout $x$ dans B.

Par adjonction d’un élément unité (prop. 3), cela résulte de la prop. 5.

Proposition 6 (Théorème de Fuglede–Putnam)

Soit A une algèbre stellaire unifère. Soient $a$ et $b$ des éléments normaux de A. Si $c\in A$ vérifie $ac=cb$, alors $a^*c=cb^*$.

L’hypothèse implique $(wa)^kc=c(wb)^k$ pour tout entier $k\geqslant 0$ et tout $w\in \mathbf{C}$, donc $e^{wa}c=ce^{wb}$ (formule (9) de I, p. 78). Considérons la fonction $f$ de $\mathbf{C}$ dans A définie par $z\mapsto e^{-za^*}ce^{zb^*}$. C’est une fonction holomorphe sur $\mathbf{C}$, dont la dérivée vérifie

$$
f'(z) =-a^*e^{-za^*}ce^{zb^*}+e^{-za^*}cb^*e^{zb^*}
$$

pour tout $z\in \mathbf{C}$. Puisque $c=e^{-za}ce^{zb}$, on peut écrire

$$
f(z) =e^{-za^*}e^{za}c e^{-zb}e^{zb^*}
$$

Puisque $a$ et $b$ sont normaux, les éléments $e^{-za^*}e^{za}=e^{-za^*+za}$ et $e^{-zb}e^{zb^*}=e^{-zb+zb^*}$ de A sont unitaires pour tout $z\in \mathbf{C}$ (lemme 5 de I, p. 102), donc de norme 1. Par conséquent, on a $\|f(z)\|\leqslant \|c\|$ pour tout $z\in \mathbf{C}$. La fonction $f$ est donc constante (VAR, R1, 3.3.6, p. 29), c’est-à-dire que $f(z) =f(0) =c$ pour tout $z\in \mathbf{C}$. Mais alors $-a^*c+cb^*=f'(0) = 0$.

#### Corollaire {#ts-i-s6-n4-cor-2 .statement tag=02DL}

Soit A une algèbre stellaire et $a$ un élément normal de A. Le commutant (resp. le bicommutant) de $\{a, a^*\}$ coïncide avec le commutant (resp. le bicommutant) de $a$.

Il suffit de prendre $b=a$ dans la proposition.

### 5. Algèbres stellaires commutatives

#### Lemme 8 {#ts-i-s6-lem-8 .statement tag=02DM}

Soient X et Y des espaces métriques, l’espace X étant complet. Soit $f$ une application de X dans Y telle que

$$
d(f(x), f(y))\geqslant d(x, y)
$$

pour tous $x$ et $y$ dans X et telle que le graphe de $f$ est fermé dans $X\times Y$. Alors $f$ est une application fermée.

Soit F une partie fermée de X et soit $(y_n)_{n\in\mathbf{N}}$ une suite dans $f(F)$ qui converge vers $y\in Y$. Pour tout $n\in \mathbf{N}$, soit $x_n\in F$ tel que $f(x_n) =y_n$. L’hypothèse implique que la suite $(x_n)_{n\in\mathbf{N}}$ est une suite de Cauchy ; soit $x\in X$ sa limite ; c’est un élément de F, car F est fermé. On a de plus $(x_n, f(x_n))\rightarrow (x, y)$ dans $X\times Y$. Comme le graphe de $f$ est fermé, il en découle que $y=f(x)$ appartient à $f(F)$.

#### Lemme 9 {#ts-i-s6-lem-9 .statement tag=02DN}

Soit A une algèbre stellaire commutative. Tout caractère de A est hermitien et la transformation de Gelfand est un morphisme d’algèbres stellaires de A dans $\mathscr{C}_0(\mathsf{X}(A))$.

Il suffit de démontrer la première assertion (proposition 7 de I, p. 38 et lemme 3 de I, p. 98). Soit $\chi$ un caractère de A. Pour tout élément hermitien $y$ de A, on a $\chi (y) =\mathscr{G}_A(y)(\chi )\in$ Sp$'(y)\subset \mathbf{R}$ (prop. 4 de I, p. 106). Par conséquent, le caractère $\chi$ est hermitien (prop. 1 de I, p. 95).

#### Théorème 1 {#ts-i-s6-thm-1 .statement tag=02DO}

Soit A une algèbre stellaire commutative. La transformation de Gelfand est un isomorphisme isométrique de l’algèbre stellaire A sur l’algèbre stellaire $\mathscr{C}_0(\mathsf{X}(A))$ des fonctions continues sur $\mathsf{X}(A)$ tendant vers 0 à l’infini.

La transformation de Gelfand est un morphisme d’algèbres involutives de A dans $\mathscr{C}_0(\mathsf{X}(A))$ (lemme 9). Soit B son image. C’est une sous-algèbre involutive de $\mathscr{C}_0(\mathsf{X}(A))$. Les éléments de B séparent les points de $\mathsf{X}(A)$ par définition. Soit $\chi \in \mathsf{X}(A)$. Il existe $x\in A$ tel que $\chi (x)\not= 0$, donc $f=\mathscr{G}(x)$ est un élément de B tel que $f(\chi )\not= 0$. D’après TG, X, p. 40, cor. 2, la sous-algèbre B est donc dense dans $\mathscr{C}_0(\mathsf{X}(A))$.

Pour tout élément hermitien $y$ de A, on a $\|\mathscr{G}(y)\|=\varrho (y) =\|y\|$ (prop. 7 de I, p. 38 et formule (2) de I, p. 104), d’où, pour tout $x\in A$, les égalités

$$
\|x\|^2=\|x^*x\|=\|\mathscr{G}(x^*x)\|=\|\overline{\mathscr{G} (x)}\cdot \mathscr{G}(x)\|=\|\mathscr{G}(x)\|^2
$$

Ainsi $\mathscr{G}$ est isométrique, et son image B est donc fermée (lemme 8). On conclut que $B =\mathscr{C}_0(\mathsf{X}(A))$.

#### Corollaire 1 {#ts-i-s6-thm-1-cor-1 .statement tag=02DP}

Soient A une algèbre stellaire et $x$ un élément normal de A. Alors $\|x\|=\varrho (x)$.

Comme la sous-algèbre stellaire de A engendrée par $x$ et $x^*$ est commutative, on peut supposer que A est commutative. Dans ce cas, le cor. résulte du th. 1, de l’exemple 2 de I, p. 102 et du th. 1 de I, p. 24.

#### Corollaire 2 {#ts-i-s6-thm-1-cor-2 .statement tag=02DQ}

Soit A une algèbre stellaire commutative.

a) Il existe un espace topologique localement compact X tel que A est isomorphe à l’algèbre stellaire $\mathscr{C}_0(X)$ ;

b) Soit B une algèbre stellaire commutative. L’application $\pi \mapsto$ $\mathsf{X}'(\pi )$ est une bijection de l’ensemble des morphismes d’algèbres stellaires de A dans B sur l’ensemble des applications partielles propres de $\mathsf{X}(B)$ dans $\mathsf{X}(A)$ (déf. 1 de I, p. 33).

Le théorème 1 établit la première assertion, et la seconde assertion découle de la prop. 3 de I, p. 34 et de l’exemple 2 de I, p. 102.

#### Corollaire 3 {#ts-i-s6-thm-1-cor-3 .statement tag=02DR}

Soit A une algèbre stellaire commutative unifère.

a) Il existe un espace topologique compact X tel que A est isomorphe à l’algèbre stellaire $\mathscr{C}(X)$;

b) Soit B une algèbre stellaire commutative unifère. L’application $\pi \mapsto \mathsf{X}(\pi )$ est une bijection de l’ensemble des morphismes unifères d’algèbres stellaires $A\rightarrow B$ dans l’ensemble des applications continues de $\mathsf{X}(B)$ dans $\mathsf{X}(A)$.

Cela découle de ce qui précède et de la prop. 4 de I, p. 35.

#### Remarque {#ts-i-s6-n5-rem-1 .statement tag=02DS}

*Soit $\mathbf{G}$ la catégorie dont les objets sont les espaces localement compacts et dont les morphismes sont les applications partielles propres (déf. 1 de I, p. 33), et soit $\mathbf{S}$ la catégorie des algèbres stellaires commutatives, dont les morphismes sont les morphismes d’algèbres involutives. Considérons le foncteur de $\mathbf{S}$ dans la catégorie opposée $\mathbf{G}^{\circ}$ qui associe à une algèbre stellaire commutative A l’espace localement compact $\mathsf{X}(A)$ des caractères non nuls de A, et à un morphisme $\varphi : A\rightarrow B$ d’algèbres stellaires commutatives l’application continue $\mathsf{X}'(\varphi )$. Le th. 1 et le cor. 2 signifient que ce foncteur est une équivalence de catégories, et qu’un quasi-inverse de ce foncteur est le foncteur qui associe à un espace topologique localement compact X l’algèbre stellaire commutative $\mathscr{C}_0(X)$.

De même, le corollaire 3 signifie que la catégorie opposée de la catégorie des espaces compacts est équivalente à la catégorie des algèbres stellaires commutatives unifères.*

### 6. Calcul fonctionnel dans les algèbres stellaires unifères

Dans ce numéro, A est une algèbre stellaire unifère et $x$ est un élément normal de A.

Soit B la sous-algèbre stellaire unifère de A engendrée par $x$; elle est commutative et contenue dans le bicommutant de $\{x, x^*\}$, donc dans le bicommutant de $x$ (cor. de la prop. 6 de I, p. 106). La transformation de Gelfand $\mathscr{G}_B: B\rightarrow \mathscr{C}(\mathsf{X}(B))$ est un isomorphisme d’algèbres stellaires (th. 1 de I, p. 108). On a Sp$_B(x) =$ Sp$_A(x)$ (prop. 5 de I, p. 106).

#### Lemme 10 {#ts-i-s6-lem-10 .statement tag=02DT}

L’application ev$_x:\chi \mapsto \chi (x)$ induit un homéomorphisme de $\mathsf{X}(B)$ sur Sp$_A(x)$.

L’application $x\mapsto \chi (x)$ de $\mathsf{X}(B)$ dans $\mathbf{C}$ est continue, et son image est égale à Sp$_B(x)$ d’après la prop. 6 de I, p. 37, donc à Sp$_A(x)$. Comme les caractères de B sont hermitiens (lemme 9 de I, p. 107), des caractères de B qui coïncident en $x$ sont également égaux en $x^*$, donc sont égaux sur la sous-algèbre stellaire unifère B engendrée par $x$. Cela prouve que l’application ev$_x$ est injective. Comme $\mathsf{X}(B)$ est compact et $\mathbf{C}$ est séparé, elle induit un homéomorphisme de $\mathsf{X}(B)$ sur son image, d’où le lemme.

On déduit du lemme un isomorphisme d’algèbres stellaires $\varphi_x:\mathscr{C}$(Sp$_A(x))\rightarrow \mathscr{C}(\mathsf{X}(B))$. Il applique une fonction $f\in \mathscr{C}$ (Sp$_A(x))$ sur la fonction $\chi \mapsto f(\chi (x))$. L’application $\mathscr{G}_B^{-1}\circ \varphi_x$ est un isomorphisme de l’algèbre stellaire $\mathscr{C}$(Sp$_A(x))$ sur B.

#### Définition 5 {#ts-i-s6-def-5 .statement tag=02DU}

Le morphisme involutif $f\mapsto (\mathscr{G}_B^{-1}\circ \varphi_x)(f)$ de $\mathscr{C}$(Sp$_A(x))$ dans A est appelé application de calcul fonctionnel continu de $x$ dans A. On le note $f\mapsto f(x)$.

#### Remarque {#ts-i-s6-n6-rem-1 .statement tag=02DV}

L’application $f\mapsto f(x)$ est isométrique ; son image est la sous-algèbre stellaire unifère B engendrée par $x$, qui est contenue dans le bicommutant de $x$.

Si $f$ est la restriction à Sp$_A(x)$ d’une fonction de la forme $z\mapsto$ $P(z, z)$, où $P\in \mathbf{C}[X,Y]$ est un polynôme, alors on a $f(x) = P(x, x^*)$ au sens algébrique usuel.

#### Exemple 1 {#ts-i-s6-n6-exa-1 .statement tag=02DW}

Supposons qu’il existe $\lambda \in \mathbf{C}$ tel que Sp$_A(x)$ est réduit à $\lambda$. On a alors $x=\lambda \cdot 1$. En effet, la fonction identique de Sp$_A(x)$ est égale à $\lambda$, donc son image par l’application de calcul fonctionnel, c’est-à-dire $x$, est égale à $\lambda \cdot 1$.

#### Exemple 2 {#ts-i-s6-n6-exa-2 .statement tag=02DX}

Pour que $x$ soit hermitien, il faut et il suffit que Sp$_A(x)$ soit contenu dans $\mathbf{R}$. En effet, soit $f$ l’application continue sur Sp$_A(x)$ donnée par $f(z) =z-\overline{z}$. Alors $x$ est hermitien si et seulement si $f(x) = 0$, c’est-à-dire si $f$ est nulle, c’est-à-dire si Sp$_A(x)$ est contenu dans $\mathbf{R}$.

#### Exemple 3 {#ts-i-s6-n6-exa-3 .statement tag=02DY}

Pour que $x$ soit unitaire, il faut et il suffit que son spectre soit contenu dans le cercle unité de $\mathbf{C}$. En effet, soit $f\in \mathscr{C}$ (Sp$_A(x))$ la fonction définie par $f(z) =zz-1$; l’élément $x$ est unitaire si et seulement si $f(x) = 0$, c’est-à-dire si $f$ est nulle.

#### Proposition 7 {#ts-i-s6-prop-7 .statement tag=02DZ}

L’application $f\mapsto f(x)$ est l’unique morphisme unifère d’algèbres involutives de $\mathscr{C}$ (Sp$_A(x))$ dans A tel que l’application identique $z$ de Sp$_A(x)$ ait pour image $x$.

En effet, la sous-algèbre unifère de $\mathscr{C}$ (Sp$_A(x))$ engendrée par les éléments $z$ et $\overline{z}$ de $\mathscr{C}$(Sp$_A(x))$ est dense dans $\mathscr{C}$ (Sp$_A(x))$ (TG, X, p. 40, cor. 1). Puisque tout morphisme d’algèbres involutives de $\mathscr{C}$ (Sp$_A(x))$ dans A est continu (I, p. 104, prop. 2), il existe au plus un morphisme d’algèbres involutives de $\mathscr{C}$(Sp$_A(x))$ dans A qui applique $z$ sur $x$.

Le corollaire suivant montre que lorsque $f$ est la restriction d’une fonction holomorphe au voisinage de Sp$_A(x)$, la définition de $f(x)$ coïn-cide avec celle du calcul fonctionnel holomorphe en une variable du numéro 9 de I, p. 74.

#### Corollaire 1 {#ts-i-s6-prop-7-cor-1 .statement tag=02E0}

Soit $f\in \mathscr{O}$(Sp$_A(x))$ un germe de fonction holomorphe au voisinage de Sp$_A(x)$ et soit $\widetilde{f}\in \mathscr{C}$(Sp$_A(x))$ la fonction continue sur Sp$_A(x)$ associée à $f$. On a $\widetilde{f}(x) =f(x)$, où $f(x)$ est l’élément de A donné par le calcul fonctionnel holomorphe.

En effet, l’application $f\mapsto \widetilde{f}(x)$ est un morphisme unifère continu de $\mathscr{O}$(Sp$_A(x))$ dans A qui applique le germe de la fonction identique au voisinage de Sp$_A(x)$ sur $x$. Le résultat est alors conséquence du th. 5 de I, p. 74.

#### Corollaire 2 {#ts-i-s6-prop-7-cor-2 .statement tag=02E1}

Soit $f\in \mathscr{C}$ (Sp$_A(x))$.

a) On a

Sp$_A(f(x)) =f$(Sp$_A(x))$ ;

b) Pour tout $g\in \mathscr{C}$ (Sp$_A(f(x)))$, on a $(g\circ f)(x) =g(f(x))$.

Comme $f(x)$ appartient à la sous-algèbre pleine B de A, on a Sp$_A(f(x)) =$ Sp$_B(f(x))$ (prop. 5 de I, p. 106). L’isomorphisme $f\mapsto f(x)$ de $\mathscr{C}$(Sp$_A(x))$ dans B préserve le spectre ; on a donc Sp$_B(f(x)) =$ Sp$_{\mathscr{C}(Sp_A(x))}(f) =f$(Sp$_A(x))$ (exemple 3 de I, p. 17). Cela démontre l’assertion a).

L’application $g\mapsto (g\circ f)(x)$ est un morphisme unifère d’algèbres involutives de $\mathscr{C}$(Sp$_A(f(x)))$ dans A qui transforme la fonction identique de Sp$_A(f(x))$ en $f(x)$. D’après la prop. 7, on a donc $(g\circ f)(x) =g(f(x))$ pour tout $g\in \mathscr{C}$ (Sp$_A(f(x)))$.

#### Exemple 4 {#ts-i-s6-n6-exa-4 .statement tag=02E2}

Soit X un espace localement compact et soit $A =\mathscr{C}_b(X)$ l’algèbre stellaire unifère commutative des fonctions continues et bornées sur X (exemple 2 de I, p. 102). Soit $g\in A$ ; son spectre S est l’adhérence dans $\mathbf{C}$ de l’ensemble $g(X)$ des valeurs de $g$ (exemple 3 de I, p. 17). L’application de calcul fonctionnel de $g$ est alors l’application $f\mapsto f\circ g$, pour $f\in \mathscr{C}(S)$. En effet, cette application est un morphisme unifère d’algèbres stellaires tel que l’application identique de S a pour image $g$.

Dans le cas où X est compact, on a $A =\mathscr{C}(X)$ et $S =g(X)$.

Soit $\pi : A\rightarrow A'$ un morphisme unifère d’algèbres stellaires unifères. L’élément $\pi (x)$ de $A'$ est normal et son spectre relativement à $A'$ est contenu dans Sp$_A(x)$. On a alors :

#### Proposition 8 {#ts-i-s6-prop-8 .statement tag=02E3}

Soit $f\in \mathscr{C}$(Sp$_A(x))$. Notant encore $f$ la restriction de $f$ à Sp$_{A'}(\pi (x))$, on a l’égalité $\pi (f(x)) =f(\pi (x))$. En particulier, pour tout $\chi \in \mathsf{X}(A)$, on a $\chi (f(x)) =f(\chi (x))$.

Soit $z$ l’application identique de Sp$_A(x)$. Les applications définies par $f\mapsto \pi (f(x))$ et $f\mapsto f(\pi (x))$ sont des morphismes unifères continus d’algèbres involutives de $\mathscr{C}$(Sp$_A(x))$ dans B qui appliquent $z$ sur $\pi (x)$. Ces morphismes coïncident donc sur la sous-algèbre involutive unifère de $\mathscr{C}$ (Sp$_A(x))$ engendrée par $z$. Comme celle-ci est dense dans $\mathscr{C}$(Sp$_A(x))$ (TG, X, p. 40, cor. 1), ces morphismes sont égaux.

#### Corollaire {#ts-i-s6-n6-cor-1 .statement tag=02E4}

Supposons que A est commutative. Pour tout $f\in$ $\mathscr{C}$(Sp$_A(x))$, on a $\mathscr{G}_A(f(x)) =f\circ \mathscr{G}_A(x)$.

Il suffit d’appliquer la prop. 8 à la transformation de Gelfand $\mathscr{G}_A$ de A dans $\mathscr{C}(\mathsf{X}(A))$ et de remarquer (exemple ci-dessus) que $f(\mathscr{G}_A(x)) =f\circ \mathscr{G}_A(x)$.

### 7. Applications du calcul fonctionnel

#### Proposition 9 {#ts-i-s6-prop-9 .statement tag=02E5}

Tout morphisme injectif d’algèbres stellaires est isométrique et, en particulier, d’image fermée.

Soient A et $A'$ des algèbres stellaires et soit $\pi : A\rightarrow A'$ un morphisme d’algèbres involutives de A dans $A'$.

Supposons d’abord que A et $A'$ sont unifères et que $\pi$ est unifère. On a $\|\pi \|\leqslant 1$ (prop. 2). Supposons qu’il existe $x$ dans A tel que $\|\pi (x)\|<\|x\|$. Soit $y=x^*x$; c’est un élément hermitien de A. Puisque A et $A'$ sont des algèbres stellaires, on a $\|\pi (y)\|=\|\pi (x)\|^2<\|x\|^2=$ $\|y\|$, c’est-à-dire $\varrho (\pi (y))< \varrho (y)$ (lemme 7 de I, p. 104). En particulier, Sp$_{A'}(\pi (y))$ est un sous-ensemble fermé de Sp$_A(y)$, distinct de Sp$_A(y)$ (remarque 6 de I, p. 3 et th. 1 de I, p. 24). Il existe alors une fonction non nulle $f\in \mathscr{C}$(Sp$_A(y))$ telle que $f|$ Sp$_{A'}(\pi (y)) = 0$ (TG, IX, p. 13, prop. 3). Soit $w=f(y)\in$ A. On a $w\not= 0$ puisque $f\not= 0$, mais $\pi (w) =\pi (f(y)) =f(\pi (y)) = 0$ puisque $f$ est nulle sur Sp$_{A'}(\pi (y))$ (prop. 8). Donc $\pi$ n’est pas injective.

Traitons maintenant le cas général. Soient $\widetilde{A}$ et $\widetilde{A}'$ les algèbres stellaires déduites de A et de $A'$ respectivement par adjonction d’un élément unité (déf. 4 de I, p. 106). Il existe un unique morphisme unifère d’algèbres involutives $\widetilde{\pi}:\widetilde{A}\rightarrow \widetilde{A}'$ prolongeant $\pi$. Ce morphisme est injectif, donc est isométrique d’après ce qui précède. Pour tout $x\in A$, on a alors $\|\pi (x)\|=\|\widetilde{\pi}(x)\|=\|x\|$.

#### Lemme 11 {#ts-i-s6-lem-11 .statement tag=02E6}

Soit X un espace topologique complètement régulier, c’est-à-dire uniformisable et séparé (TG, IX, p. 8, déf. 4), contenant au moins deux points. Il existe des fonctions continues non nulles $f$ et $g$ dans $\mathscr{C}(X)$ telles que $f g= 0$.

Soient $x\not=y$ des points distincts de X. Soient U et V des voisinages ouverts de $x$ et $y$, respectivement, tels que U et V sont disjoints. Puisque X est uniformisable, d’après TG, IX, p. 7, th. 2, il existe une fonction $f\in \mathscr{C}(X)$ telle que $f(x) = 1$ et $f|X$ - U = 0. De même, il existe $g\in \mathscr{C}(X)$ telle que $g(y) = 1$ et $g|X$ - V = 0. On a alors $f g= 0$.

#### Proposition 10 {#ts-i-s6-prop-10 .statement tag=02E7}

Soit A une algèbre stellaire unifère. On suppose que pour tout couple $(x, y)$ d’éléments permutables de A, la condition $xy= 0$ implique que $x= 0$ ou $y= 0$. Alors $A =\mathbf{C}\cdot 1$.

Si A n’est pas égale à $\mathbf{C}\cdot 1$, il existe un élément hermitien $x$ dans A qui n’appartient pas à $\mathbf{C}\cdot 1$ (lemme 2 de I, p. 96). Soit B la sous-algèbre stellaire unifère de A engendrée par $x$. Elle est commutative, et isomorphe à $\mathscr{C}$ (Sp$_A(x))$ (I, p. 110, remarque). Comme $x$ n’est pas scalaire, son spectre dans B n’est pas réduit à un seul élément (exemple 1 de I, p. 110). Il existe donc des fonctions continues et non nulles $f$ et $g$ sur Sp$_A(x)$ telles que $f g= 0$ (lemme 11). Les éléments $f(x)$ et $g(x)$ de A sont non nuls, permutables, et vérifient $f(x)g(x) = 0$ dans A.

#### Proposition 11 {#ts-i-s6-prop-11 .statement tag=02E8}

Soient A une algèbre stellaire unifère, $a,x$ et $y$ des éléments de A. On suppose que $x$ et $y$ sont normaux. Si $xa=$ $ay$, alors on a $f(x)a=af(y)$ pour toute fonction $f$ continue dans la réunion du spectre de $x$ et du spectre de $y$. En particulier, on a $f(aa^*)a=af(a^*a)$ pour toute fonction $f\in \mathscr{C}$ (Sp$'(a^*a))$.

Soit S = Sp($x$)$\cup$ Sp($y$). La proposition 6 de I, p. 106 implique que $x^*a=ay^*$. Par conséquent, il vient $f(x)a=af(y)$ pour toute fonction $f$ qui est de la forme $z\mapsto P(z, z)$, où $P\in \mathbf{C}[X,Y]$ est un polynôme. Puisque l’ensemble des fonctions $f\in \mathscr{C}(S)$ vérifiant $f(x)a=$ $af(y)$ est une sous-algèbre fermée de $\mathscr{C}(S)$, elle coïncide avec $\mathscr{C}(S)$ d’après TG, X, p. 40, cor. 1.

La seconde assertion est une conséquence de la première, appliquée aux éléments hermitiens $x=aa^*$ et $y=a^*a$, compte tenu du fait que Sp$'(a^*a) =$ Sp$'(aa^*)$ (prop. 1 de I, p. 5).

### 8. Calcul fonctionnel dans une algèbre non unifère

Soit A une algèbre stellaire et soit $\widetilde{A}$ l’algèbre stellaire unifère déduite de A par adjonction d’un élément unité $e$. Notons $\pi$ le caractère hermitien $x+\lambda e\mapsto \lambda$ de $\widetilde{A}$ dans $\mathbf{C}$; on a Ker($\pi$ ) $= A$.

Soit $x\in A$ un élément normal. Il est normal dans $\widetilde{A}$ et Sp$_{\widetilde{A}}(x) =$ Sp$'_A(x)$. Notons $\mathscr{C}'$(Sp$'_A(x))$ l’algèbre stellaire des fonctions continues $f$ sur Sp$'_A(x)$ telles que $f(0) = 0$.

Soit $f\in \mathscr{C}$ (Sp$'_A(x))$. Comme $\pi (f(x)) =f(\pi (x))$ (prop. 8 de I, p. 112), on a $f(x)\in A$ si et seulement si $f(0) = 0$. L’application $f\mapsto f(x)$ définit un morphisme d’algèbres involutives de l’algèbre stellaire $\mathscr{C}'$(Sp$'_A(x))$ dans A pour lequel l’image de l’application identique $z$ de Sp$'_A(x)$ est $x$. Ce morphisme est isométrique et son image est la sous-algèbre stellaire de A engendrée par $x$.

#### Proposition 12 {#ts-i-s6-prop-12 .statement tag=02E9}

L’application $f\mapsto f(x)$ est l’unique morphisme d’algèbres involutives de l’algèbre stellaire $\mathscr{C}'$(Sp$'_A(x))$ dans A tel que l’application identique $z$ de Sp$'_A(x)$ ait pour image $x$.

Les éléments $z$ et $\overline{z}$ de $\mathscr{C}'$(Sp$'_A(x))$ engendrent une sous-algèbre dense de $\mathscr{C}'$(Sp$'_A(x))$ (cf. TG, X, p. 40, cor. 2). Puisque tout morphisme d’algèbres involutives de l’algèbre stellaire $\mathscr{C}'$(Sp$'_A(x))$ dans l’algèbre stellaire A est continu (I, p. 104, prop. 2), le résultat en découle.

Les résultats du numéro précédent concernant le calcul fonctionnel s’étendent au cas général. Nous les énoncerons simplement et laisserons aux lecteurs le soin de compléter les démonstrations, mutatis mutandis.

#### Proposition 13 {#ts-i-s6-prop-13 .statement tag=02EA}

On a les propriétés suivantes :

a) Pour tout $f\in \mathscr{C}'$(Sp$'_A(x))$, on a Sp$'_A(f(x)) =f$(Sp$'_A(x))$ ;

b) Pour tout $f\in \mathscr{C}'$(Sp$'_A(x))$ et pour tout $g\in \mathscr{C}'$(Sp$'_A(f(x)))$, on a $(g\circ f)(x) =g(f(x))$ ;

c) Soit $A'$ une algèbre stellaire et soit $\pi$ un morphisme de A dans $A'$; alors $\pi (x)$ est normal dans $A'$, on a Sp$'_{A'}(\pi (x))\subset$ Sp$'_A(x)$ et $\pi (f(x)) =f(\pi (x))$ pour tout $f\in \mathscr{C}'$(Sp$'_A(x))$;

d) Si A est commutative, et si $f\in \mathscr{C}'$(Sp$'_A(x))$, alors $\mathscr{G}'_A(f(x)) =$ $f\circ \mathscr{G}'_A(x)$.

#### Remarque {#ts-i-s6-n8-rem-1 .statement tag=02EB}

Soit A une algèbre stellaire unifère et soit $\widetilde{A}$ l’algèbre stellaire unifère déduite de A par adjonction d’un élément unité $e$. Pour tout $x\in A$, on a Sp$'_A(x) =$ Sp$_A(x)\cup  \{0\}$. Soit $x$ un élément normal de A. C’est alors un élément normal de $\widetilde{A}$ et l’on dispose donc de deux applications de calcul fonctionnel dans A, la première définie sur $\mathscr{C}$ (Sp$_A(x))$ et la seconde sur $\mathscr{C}'$(Sp$'_A(x))$. Soit $f'\in \mathscr{C}'$(Sp$'_A(x))$; si l’on note $f$ sa restriction à Sp$_A(x)$, on a alors $f'(x) =f(x)$.

### 9. Éléments positifs dans les algèbres stellaires

#### Définition 6 {#ts-i-s6-def-6 .statement tag=02EC}

Soit A une algèbre stellaire. Un élément $x$ de A est dit positif s’il est hermitien et si Sp$'_A(x)\subset \mathbf{R}_+$. On note $A_+$ l’ensemble des éléments positifs de A. C’est un sous-ensemble de $A_h$.

On note $x\geqslant y$ si $x-y\in A_+$.

Si l’algèbre stellaire A est unifère, son élément unité est positif.

Si B est une sous-algèbre stellaire de A, on a $B_+= B\cap A_+$ (cor. de la prop. 5 de I, p. 106).

Si $\pi : A\rightarrow$ B est un morphisme d’algèbres stellaires, alors $\pi (A_+)\subset B_+$.

#### Exemple 1 {#ts-i-s6-n9-exa-1 .statement tag=02ED}

Soit X un espace localement compact. Dans l’algèbre stellaire $\mathscr{C}_0(X)$ des fonctions continues sur X et tendant vers 0 à l’infini, resp. dans l’algèbre stellaire $\mathscr{C}_b(X)$ des fonctions continues bornées sur X, une fonction $f$ est un élément positif si et seulement si elle est à valeurs réelles et si $f(x)\geqslant 0$ pour tout $x\in X$ (cf. exemple 3 de I, p. 17).

#### Exemple 2 {#ts-i-s6-n9-exa-2 .statement tag=02EE}

Soit A une algèbre stellaire commutative. Soit $a$ dans A. Puisque Sp$'_A(x)$ est la réunion de $\{0\}$ et de l’image de la transformée de Gelfand $\mathscr{G}(a)$ (prop. 6 de I, p. 37), l’élément $a$ est positif si, et seulement si, la transformée de Gelfand $\mathscr{G}(a)$ est une fonction positive.

#### Exemple 3 {#ts-i-s6-n9-exa-3 .statement tag=02EF}

Soit E un espace hilbertien complexe. Un élément $x$ de l’algèbre stellaire $\mathscr{L}(E)$ (exemple 1 de I, p. 102) est positif si et seulement si c’est un endomorphisme positif de E au sens de EVT, V, p. 45, déf. 6 (prop. 8 de I, p. 138).

#### Lemme 12 {#ts-i-s6-lem-12 .statement tag=02EG}

Soit A une algèbre stellaire unifère et soit $x\in A$ un élément hermitien.

a) L’élément $x$ est positif si et seulement si $\|\|x\| \cdot 1-x\|\leqslant \|x\|$;

b) Si $\|x\|\leqslant 1$, alors $x$ est positif si et seulement si $\|1-x\|\leqslant 1$ ;

c) Si $x$ est positif, alors $1-x$ est positif si et seulement si $\|x\|\leqslant 1$ ;

d) Si $x$ est positif et si $y\in A_+$ est permutable à $x$, alors $xy$ est positif.

L’élément $x$ est hermitien, donc normal. En considérant la sous-algèbre stellaire engendrée par $x$, qui est commutative, on se ramène au cas où l’algèbre A est commutative, c’est-à-dire au cas où A = $\mathscr{C}_0(X)$ pour un espace topologique localement compact X (th. 1 de I, p. 108). Les trois premières assertions découlent alors immédiatement de l’exemple 1 ci-dessus. De même, pour montrer l’assertion d), on peut considérer la sous-algèbre stellaire engendrée par $x$ et $y$, qui est commutative.

#### Proposition 14 {#ts-i-s6-prop-14 .statement tag=02EH}

Soit A une algèbre stellaire. L’ensemble $A_+$ est un cône convexe fermé pointé saillant dans l’espace de Banach réel $A_h$ (EVT, II, p. 11).

Soit $\widetilde{A}$ l’algèbre stellaire déduite de A par adjonction d’un élément unité. Puisque $A_+= A\cap \widetilde{A}_+$, il suffit de démontrer la proposition pour $\widetilde{A}$. On peut donc supposer que A possède un élément unité.

On a $0\in A_+$. Pour tout $\lambda \in \mathbf{R}_+^*$ et tout $x\in A$, on a Sp$'_A(\lambda x) =$ $\lambda$ Sp$'_A(x)$, ce qui implique que $A_+$ est un cône dans l’espace de Banach réel $A_h$.

Pour montrer que $A_+$ est convexe, il suffit de montrer que si $x$ et $y$ sont positifs, alors $x+y\geqslant 0$ (EVT, II, p. 11, prop. 10). Par homothétie, il suffit de démontrer que si $x\geqslant 0$ et $y\geqslant 0$ vérifient de plus $\|x\|\leqslant 1$, $\|y\|\leqslant 1$, alors l’élément $\frac{1}{2}(x+y)$ est positif. Or on a

$$
\|1-\frac{1}{2}(x+y)\|\leqslant \frac{1}{2}\|1-x\|+\frac{1}{2}\|1-y\|\leqslant 1
$$

d’après l’assertion b) du lemme 12, et cette même assertion montre alors que $\frac{1}{2}(x+y)$ est positif.

Enfin, l’assertion a) du lemme 12 implique également que $A_+$ est fermé.

Puisque $A_+$ est un cône pointé dans $A_h$, il est saillant si et seulement si $A_+\cap (-A_+)$ est réduit à 0. Mais si $x\in A_+\cap (-A_+)$, on a Sp$'_A(x) =$ $\{0\}$, donc $\varrho (x) = 0$, et $\|x\|= 0$ comme $x$ est hermitien (lemme 7, (2) de I, p. 104), d’où $x= 0$.

La proposition 14 signifie que la relation « $x\geqslant y$ » est une relation d’ordre sur $A_h$ (EVT, II, p. 13, prop. 13).

#### Proposition 15 {#ts-i-s6-prop-15 .statement tag=02EI}

Soit A une algèbre stellaire. Soit $x$ un élément normal de A.

a) Supposons que A soit unifère et soit $f$ une fonction continue de Sp$_A(x)$ dans $\mathbf{C}$. Pour que $f(x)$ soit positif, il faut et il suffit que l’image de $f$ soit contenue dans $\mathbf{R}_+$;

b) Soit $f$ une fonction continue de Sp$'_A(x)$ dans $\mathbf{C}$ telle que $f(0) =$ 0. Pour que $f(x)$ soit un élément positif de A, il faut et il suffit que l’image de $f$ soit contenue dans $\mathbf{R}_+$.

L’assertion a) découle de l’assertion a) du cor. 2 de I, p. 111, et l’assertion b) découle de la prop. 13 de I, p. 114.

Soit $x$ un élément hermitien de l’algèbre stellaire A. Son spectre est contenu dans $\mathbf{R}$ (prop. 4 de I, p. 106). Considérons les fonctions continues de Sp$'_A(x)$ dans $\mathbf{R}$ définies par

$f_1:t\mapsto$ sup($t,0$)$,f_2:t\mapsto$ sup($-t,0$)$,f_3:t\mapsto  |t|$.

On note

$$
x^+=f_1(x),x^-=f_2(x),|x|=f_3(x) \tag{3}
$$

Comme les fonctions $f_1,f_2,f_3$ sont à valeurs réelles positives et s’annulent en 0, les éléments $x^+,x^-$ et $|x|$ sont des éléments positifs de A (prop. 15, a)) qui appartiennent à la sous-algèbre stellaire de A engendrée par $x$.

On a $f_1(t)-f_2(t) =t$ pour tout $t\in \mathbf{R}$, ainsi que les relations $f_1+f_2=f_3$ et $f_1f_2= 0$. Il en découle les relations :

$$
x=x^+-x^-,|x|=x^++x^-,x^+x^-=x^-x^+= 0 \tag{4}
$$

Comme l’application de calcul fonctionnel est isométrique, on a

$$
\| |x| \|=\|x\|,\|x^+\|\leqslant \|x\|,\|x^-\|\leqslant \|x\|
$$

Soit $x$ un élément positif de A. Il est hermitien, donc normal. Soit $\alpha \in \mathbf{R}^*_+$, et soit $g$ la restriction à Sp$'_A(x)$ de la fonction $t\mapsto t^{\alpha}$; on note $x^{\alpha}=g(x)$. C’est un élément positif de la sous-algèbre stellaire de A engendrée par $x$. Soient $\alpha$ et $\beta$ dans $\mathbf{R}^*_+$. Comme l’application de calcul fonctionnel est un morphisme d’algèbres, et d’après la prop. 13 de I, p. 114, on a

$$
x^{\alpha}x^{\beta}=x^{\alpha+\beta}(x^{\alpha})^{\beta}=x^{\alpha \beta} \tag{5}
$$

$$
\surd_/
$$

On écrira aussi $\overline{x}=x^{12}$.

#### Proposition 16 {#ts-i-s6-prop-16 .statement tag=02EJ}

Soit $x$ un élément positif de A. Soit $\alpha \in \mathbf{R}^*_+$. Alors $x^{1/\alpha}$ est l’unique élément positif $y$ de A tel que $y^{\alpha}=x$.

On a vu ci-dessus que $x^{1/\alpha}$ vérifie les propriétés demandées. Inversement, soit $y$ un élément positif de A tel que $y^{\alpha}=x$. D’après la formule (5), on a $y= (y^{\alpha})^{1/\alpha}=x^{1/\alpha}$, ce qu’il fallait démontrer.

#### Lemme 13 {#ts-i-s6-lem-13 .statement tag=02EK}

Soit A une algèbre stellaire unifère. Tout élément de A est somme d’éléments unitaires.

D’après le lemmeOn aSoit$yx_*=$un élément hermitien de$_{1\overline{2}}x-i12\surd$,1c$-)$, on a$_{1\overline{4}}x_2$, donc$1-\frac{1}{4}Axyy$. Supposons d’abord que$^2_*\in = 1A_+$. Soitet $xy==y\frac{1}{2}+xy+_*i$est somme$\surd\|1x-\|\leqslant^1_{\overline{4}}x2^2$..

de deux éléments unitaires. Dans le cas général, soit $k$ un entier tel que $\|\frac{1}{k}x\|\leqslant 2$ ; l’élément $x$ est alors somme de $2k$ éléments unitaires. D’après le lemme 2 de I, p. 96, le lemme en résulte.

#### Théorème 2 {#ts-i-s6-thm-2 .statement tag=02EL}

Soit A une algèbre stellaire. Un élément $x$ de A est positif si et seulement s’il existe $y\in A$ tel que $x=y^*y$.

Supposons que $x$ soit positif. Soit $y=x^{1/2}$; c’est un élément hermitien de A et on a $y^*y=y^2=x$.

Réciproquement, soit $y$ un élément de A et posons $x=y^*y$. C’est un élément hermitien de A. Montrons que $x$ est positif. Notons pour cela $z=x^-$ et posons $w=yz$. On a alors

$$
w^*w=z^*y^*yz=zxz=z(x^+-z)z=-z^3
$$

Comme $z\geqslant 0$, on a $z^3\geqslant 0$, et on en déduit que Sp$'_A(w^*w)\subset \mathbf{R}_-$. Écrivons par ailleurs $w=w_1+iw_2$ où $w_1$ et $w_2$ sont hermitiens (lemme 2 de I, p. 96). Les éléments $w^2_1$ et $w_2^2$ sont positifs. On a $ww^*+w^*w=$ $2w^2_1+ 2w_2^2$, et la prop. 14 montre donc que $ww^*= 2w_1^2+ 2w^2_2+ (-w^*w)$ est positif. Comme Sp$'_A(ww^*) =$ Sp$'_A(w^*w)$ (I, p. 5, prop. 1), qui est contenu dans $\mathbf{R}_-$, on conclut que Sp$'_A(w^*w) =\{0\}$. Puisque $w^*w$ est hermitien, cela implique (cor. 1 de I, p. 108) que $\|w^*w\|=\varrho (w^*w) = 0$, donc que $z^3= 0$. Puisque $z$ est hermitien, on a $z= 0$. Ainsi, $x=x^+$ est positif.

#### Remarque {#ts-i-s6-n9-rem-1 .statement tag=02EM}

Soit A une algèbre stellaire et soit $x\in A$. L’élément $x^*x$ de A est positif ; on pose alors $|x|= (x^*x)^{1/2}$. On a $\|x\|^2=\|x^*x\|=$ $\||x|^2\|=\||x|\|^2$, donc $\|x\|=\||x|\|$.

Lorsque $x$ est normal, on a également $|x|=f(x)$, où $f$ est l’application de $\mathbf{C}$ dans $\mathbf{C}$, nulle en 0, donnée par $f(z) =|z|$. En particulier, lorsque $x$ est hermitien, $|x|$ coïncide avec l’élément défini par la formule (3).

Supposons de plus que A soit unifère et que $x$ soit inversible. Alors $|x|$ est également inversible, l’élément $u=x|x|^{-1}$ est unitaire et l’on a $x=u|x|$ (« décomposition polaire » ; voir aussi I, p. 139, n$^o8$ pour le cas des endomorphismes des espaces hilbertiens).

#### Lemme 14 {#ts-i-s6-lem-14 .statement tag=02EN}

Soit A une algèbre stellaire, et soient $x$ et $y$ des éléments hermitiens de A.

a) Si $x\leqslant y$, alors pour tout élément $w$ de A, on a $w^*xw\leqslant w^*yw$. En particulier, si $y\geqslant 0$, on a $w^*yw\geqslant 0$;

b) Supposons que A est unifère. Si $0\leqslant x\leqslant y$ et si $x$ est inversible, alors $y$ est inversible et $y^{-1}\leqslant x^{-1}$;

c) Si $0\leqslant x\leqslant y$ alors $\|x\|\leqslant \|y\|$.

Soit $u= (y-x)^{1/2}$. On a $w^*yw-w^*xw=w^*u^2w= (uw)^*(uw)$, et l’assertion a) résulte du th. 2.

Démontrons l’assertion b). Supposons d’abord que $x= 1$. Soit B la sous-algèbre stellaire unifère engendrée par $y$. Par l’isomorphisme de Gelfand, $y$ correspond à une fonction continue $\geqslant 1$ sur l’espace compact $\mathsf{X}(B)$. Cette fonction est donc inversible et son inverse est $\leqslant 1$. Ceci implique que $y$ est inversible et $y^{-1}\leqslant 1 =x^{-1}$. Dans le cas général, on observe que $0\leqslant 1\leqslant x^{-1/2}yx^{-1/2}$ d’après a), donc le cas précédent implique que $z=x^{-1/2}yx^{-1/2}$ est inversible et $z^{-1}\leqslant 1$. Ainsi, $y$ est inversible et $y^{-1}\leqslant x^{-1}$ d’après a) encore.

Pour démontrer l’assertion c), on peut supposer que A est unifère (prop. 3 de I, p. 105). Supposons d’abord que $y$ est inversible. Notons

$$
\surd -_{1-1}
$$

$b=y$. D’après a), les conditions $0\leqslant x\leqslant y$ impliquent $0\leqslant bxb\leqslant$ $b^{-1}yb^{-1}= 1$, donc $\|b^{-1}xb^{-1}\|\leqslant 1$ par le lemme 12, c) de I, p. 116. On a alors

$$
\|x\|=\|b(b^{-1}xb^{-1})b\|\leqslant \|b\|\|b^{-1}xb^{-1}\|\|b\|\leqslant \|b\|^2=\|b^2\|=\|y\|
$$

Dans le cas général, pour tout réel $\varepsilon  >0$, l’élément $y+\varepsilon$ est inversible et $0\leqslant x\leqslant y+\varepsilon$. D’après ce qui précède, on a donc $\|x\|\leqslant \|y+\varepsilon \|$ pour tout nombre réel $\varepsilon  >0$, d’où le résultat.

#### Remarque {#ts-i-s6-n9-rem-2 .statement tag=02EO}

En général, si $x$ et $y$ sont des éléments positifs d’une algèbre stellaire A, la condition $0\leqslant x\leqslant y$ n’implique pas $x^2\leqslant y^2($cf. exercice 15 de I, p. 182).

### 10. Unités approchées dans les algèbres stellaires

#### Définition 7 {#ts-i-s6-def-7 .statement tag=02EP}

Soit A une algèbre normée. Une unité approchée de A est une base de filtre $\mathfrak{F}$ sur la boule unité de A telle que, pour tout $x$ dans A, les bases de filtre $x\mathfrak{F}$ et $\mathfrak{F}x$ sur A convergent vers $x$, autrement dit :

lim$_{f,\mathfrak{F}}f x=$ lim$_{f,\mathfrak{F}}xf=x$.

Si A est une algèbre stellaire, une unité approchée $\mathfrak{F}$ est dite croissante si $\mathfrak{F}$ est une base de filtre sur $A_+$.

Soit A une algèbre stellaire. On note $A^{\leqslant 1}_+$ (resp. $A^{<1}_+)$ l’ensemble des éléments positifs de A de norme $\leqslant 1$ (resp. de norme $<1$) ; ce sont les éléments hermitiens de A dont le spectre est contenu dans $[0,1]$ (resp. dans $[0,1[$).

#### Proposition 17 {#ts-i-s6-prop-17 .statement tag=02EQ}

Soit A une algèbre stellaire, soit $\mathfrak{F}$ une base de filtre sur $A^{\leqslant 1}_+$. Pour que $\mathfrak{F}$ soit une unité approchée croissante de A, il faut et il suffit que l’on ait

lim$_{f,\mathfrak{F}}f x=x$

pour tout élément positif $x$ de A.

La condition est évidemment nécessaire ; démontrons qu’elle est suffisante. Soit $\widetilde{A}$ l’algèbre stellaire déduite de A par adjonction d’un élément unité. Soit $x$ un élément de A et soit $f\in A^{\leqslant 1}_+$. On a

$$
\|f x-x\|^2=\|(f x-x)(f x-x)^*\|=\|(f-1)xx^*(f-1)\|
$$

$$
\leqslant \|(f-1)xx^*\|
$$

car $\|f-1\|\leqslant 1$ (lemme 12, c) de I, p. 116). On a donc

lim sup$_{f,\mathfrak{F}}\|f x-x\|^2\leqslant$ lim sup$_{f,\mathfrak{F}}\|f xx^*-xx^*\|$. Comme $xx^*$ est positif (th. 2 de I, p. 118), l’hypothèse implique que

lim sup$_{f,\mathfrak{F}}\|f x-x\|^2\leqslant \|xx^*-xx^*\|= 0$,

de sorte que

lim$_{f,\mathfrak{F}}f x=x$.

Comme l’involution de A est continue et comme $\mathfrak{F}$ est une base de filtre sur $A_h$, il vient

lim$_{f,\mathfrak{F}}xf=$ lim$_{f,\mathfrak{F}}(f^*x^*)^*=$ lim$_{f,\mathfrak{F}}(f x^*)^*= (x^*)^*=x$.

La proposition en résulte.

#### Proposition 18 {#ts-i-s6-prop-18 .statement tag=02ER}

Soit A une algèbre stellaire. L’ensemble ordonné $A^{<1}_+$ est filtrant à droite (E, III, p. 12, déf. 7) et le filtre de ses sections (TG, I, p. 38, exemple 2) est une unité approchée croissante de A.

Soit $\widetilde{A}$ l’algèbre stellaire déduite de A par adjonction d’un élément unité noté 1 (déf. 4 de I, p. 106).

Soit $g$ la fonction de $[0,1[$ dans $\mathbf{R}_+$ définie par $g(t) =t(1-t)^{-1}$. C’est une bijection continue croissante, sa bijection réciproque étant donnée par $t\mapsto 1-(1 +t)^{-1}$.

Démontrons que l’ensemble ordonné $A^{<1}_+$ est filtrant à droite. Soient $x$ et $y$ des éléments de $A^{<1}_+$. Puisque $g(0) = 0$ et puisque Sp$'_A(x)$ et Sp$'_A(y)$ sont contenus dans $[0,1[$, les éléments $g(x)$ et $g(y)$ sont définis ; ils sont positifs, de sorte que $g(x) +g(y)\geqslant 0$. On peut donc former l’élément $z=g^{-1}(g(x) +g(y))$ de A. On a Sp$'_A(z)\subset [0,1[$, et donc $z\in A^{<1}_+$.

On a $0\leqslant g(x)\leqslant g(z)$, d’où $1\leqslant 1+g(x)\leqslant 1+g(z)$. L’assertion b) du lemme 14 de I, p. 119 implique que $1 +g(x)$ et $1 +g(z)$ sont inversibles et que $(1 +g(z))^{-1}\leqslant (1 +g(x))^{-1}$. Par suite, $z= 1-(1 +g(z))^{-1}\geqslant$ $1-(1 +g(x))^{-1}=x$. De même, on a $z\geqslant y$. En conséquence, $z$ majore $x$ et $y$ dans $A^{<1}_+$. L’ensemble ordonné $A^{<1}_+$ est donc filtrant à droite. Notons $\mathfrak{F}$ le filtre de ses sections

Soit $x$ un élément positif de A. Pour tout entier $n\geqslant 1$, soit $e_n=$ $g^{-1}(nx)$ ; on a $e_n\in A^{<1}_+$. Soit $h_n$ la fonction continue sur $\mathbf{R}_+$ définie pour tout $t\in \mathbf{R}_+$ par $h_n(t) =t^2(1-g^{-1}(nt)) =t^2/(1 +nt)$. On a $|h_n(t)|\leqslant t/n$ pour tout $t\geqslant 0$, et donc $\|x(1-e_n)x\|=\|h_n(x)\|\leqslant$ $\|x\|/n$. En particulier, $x(1-e_n)x$ tend vers 0 quand $n$ tend vers l’infini.

Soit $\varepsilon  >0$ un nombre réel. Soit $n$ un entier tel que $\|x(1-e_n)x\|< \varepsilon$. Pour tout $f\in A^{<1}_+$ tel que $f\geqslant e_n$, on a alors

$$
\|x-f x\|^2=\|(1-f)x\|^2=\|((1-f)x)^*(1-f)x\|=\|x^*(1-f)^2x\|
$$

$$
=\|x(1-f)^2x\|
$$

Par ailleurs, puisque $0\leqslant f\leqslant 1$, il vient $(1-f)-(1-f)^2= (1-f)f\geqslant 0$ (lemme 12, d) de I, p. 116), donc $(1-f)^2\leqslant 1-f$. Comme $1-f\leqslant 1-e_n$, il vient $0\leqslant (1-f)^2\leqslant 1-e_n$. D’après le lemme 14, a) et c) de I, p. 119, il s’ensuit

$$
\|x-f x\|^2=\|x(1-f)^2x\|\leqslant \|x(1-e_n)x\|< \varepsilon
$$

On a donc lim$_{f,\mathfrak{F}}f x=x$ pour tout $x\in A_+$. Le filtre $\mathfrak{F}$ est donc une unité approchée de A d’après la proposition 17.

### 11. Quotient par un idéal bilatère fermé

#### Lemme 15 {#ts-i-s6-lem-15 .statement tag=02ES}

Soit A une algèbre stellaire et soit I un idéal bilatère fermé de A. Alors I est auto-adjoint.

Soit $J = I\cap I^*$. L’ensemble J est un idéal bilatère auto-adjoint de A, qui contient $I^*I$. En particulier, J est une algèbre stellaire. Soit $\mathfrak{F}$ une unité approchée croissante de J (prop. 18 de I, p. 121). Pour tout $x\in I$ et tout $f\in J^{\leqslant 1}_+$, on a

$$
\|xf-x\|^2=\|(xf-x)^*(xf-x)\|=\|f(x^*xf-x^*x)-(x^*xf-x^*x)\|
$$

$$
\leqslant 2\|x^*xf-x^*x\|
$$

Comme $x^*x\in J$, on a donc

lim$_{f,\mathfrak{F}}\|xf-x\|^2= 0$.

Comme $xf\in J$ pour tout $f\in J^{\leqslant 1}_+$ et comme J est fermé, cela implique que $x\in J$. Donc I = J, et l’idéal I est auto-adjoint.

#### Proposition 19 {#ts-i-s6-prop-19 .statement tag=02ET}

Soit A une algèbre stellaire et soit I un idéal bilatère fermé de A. Alors l’algèbre de Banach involutive quotient $A/I$ est une algèbre stellaire.

L’idéal I est auto-adjoint (lemme 15). On considère l’algèbre stellaire $\widetilde{A}$ déduite de A par adjonction d’un élément unité (déf. 4 de I, p. 106). Dans cette algèbre, l’ensemble I est un idéal bilatère auto-adjoint fermé, et $A/I$ s’identifie à une sous-algèbre involutive fermée de $\widetilde{A}/I$. On peut donc supposer que A est unifère.

L’algèbre de Banach $A/I$ est involutive. Soit $\pi : A\rightarrow A/I$ la projection canonique. L’idéal bilatère auto-adjoint I est une sous-algèbre stellaire de A. Soit $\mathfrak{F}$ une unité approchée croissante de I (prop. 18 de I, p. 121). Montrons d’abord que pour tout $x\in A$, on a

(6) $\|\pi (x)\|_{A/I}=$ lim$_{f,\mathfrak{F}}\|x-xf\|$.

D’une part, comme $xf\in I$ pour tout $f\in I^{\leqslant 1}_+$, on a

$\|\pi (x)\|_{A/I}=$ inf$_{a\in I}\|x-a\|\leqslant$ lim inf$_{f,\mathfrak{F}}\|x-xf\|$.

D’autre part, pour tout $a\in I$, on a

$$
\|x-xf\|\leqslant \|(x-a)-(x-a)f\|+\|a-af\|
$$

$$
=\|(x-a)(1-f)\|+\|a-af\|
$$

et donc, puisque $\|1-f\|\leqslant 1$ (lemme 12 de I, p. 116) et $a\in I$, on en déduit

lim sup$_{f,\mathfrak{F}}\|x-xf\|\leqslant \|x-a\|$.

Ainsi, il vient lim sup$_{f,\mathfrak{F}}\|x-xf\|\leqslant \|\pi (x)\|_{A/I}$ puisque $a$ est arbitraire dans I. La formule (6) est donc démontrée.

Soit maintenant $x$ un élément de A. D’après la formule (6), on a

$\|\pi (x)\|^2_{A/I}=$ lim$_{f,\mathfrak{F}}\|x-xf\|^2=$ lim$_{f,\mathfrak{F}}\|x(1-f)\|^2$

= lim$_{f,\mathfrak{F}}\|(1-f)x^*x(1-f)\|\leqslant$ lim$_{f,\mathfrak{F}}\|x^*x(1-f)\|=\|\pi (x^*x)\|_{A/I}$.

Le lemme 6 de I, p. 103 entraîne alors que l’algèbre de Banach involutive $A/I$ est une algèbre stellaire.

### 12. Algèbre stellaire enveloppante d’une algèbre de Banach involutive

#### Lemme 16 {#ts-i-s6-lem-16 .statement tag=02EU}

Soit A une algèbre involutive et soit $p$ une semi-norme sur A. Les conditions suivantes sont équivalentes :

(i) On a $p(xy)\leqslant p(x)p(y),p(x^*) =p(x)$ et $p(x)^2=p(x^*x)$ quels que soient $x, y\in A$ ;

(ii) L’ensemble R des éléments $x$ de A tels que $p(x) = 0$ est un idéal bilatère auto-adjoint de A, et la semi-norme sur $A/R$ déduite de $p$ fait de $A/R$ une algèbre normée involutive dont la complétée est une algèbre stellaire;

(iii) Il existe une algèbre stellaire B et un morphisme d’algèbres involutives $\varphi$ de A dans B tel que $p(x) =\|\varphi (x)\|$ pour tout $x\in A$.

Les implications (i)$=\Rightarrow$ (ii)$=\Rightarrow$ (iii)$=\Rightarrow$ (i) sont toutes élémentaires.

Une semi-norme satisfaisant aux conditions du lemme 16 sera appelée une semi-norme stellaire sur l’algèbre involutive A.

Soit A une algèbre normée involutive et soit S l’ensemble des semi-normes stellaires sur A. On a $p(x)\leqslant \|x\|$ pour tout $x\in A$ et tout $p\in S$ (I, p. 104, prop. 2). L’application $x\mapsto  \|x\|_*=$ sup$_{p\in S}p(x)$ est une

semi-norme stellaire sur A. C’est la plus grande semi-norme stellaire sur A.

Soit R l’ensemble des $x\in A$ tels que $\|x\|_*= 0$. C’est un idéal bilatère fermé de A. On note Stell(A) l’algèbre stellaire complétée de $A/R$ pour la norme déduite de $x\mapsto  \|x\|_*$ (lemme 16, (ii)). L’application canonique de A dans Stell(A) est continue, son image est dense dans Stell(A) et son noyau est égal à R.

#### Définition 8 {#ts-i-s6-def-8 .statement tag=02EV}

L’algèbre stellaire Stell(A) est appelée l’algèbre stellaire enveloppante de l’algèbre normée involutive A.

Si A est commutative, alors Stell(A) est commutative ; si A est unifère, alors Stell(A) est unifère.

#### Proposition 20 {#ts-i-s6-prop-20 .statement tag=02EW}

Soit A une algèbre normée involutive et soit $j$ le morphisme canonique de A dans Stell(A). Pour toute algèbre stellaire B et pour tout morphisme $\varphi$ d’algèbres involutives de A dans B, il existe un unique morphisme $\varphi '$ d’algèbres stellaires de Stell(A) dans B tel que $\varphi =\varphi '\circ j$.

Notons $x\mapsto  \|x\|_*$ la norme sur Stell(A). Soit R le noyau de $j$. L’application $x\mapsto  \|\varphi (x)\|$ est une semi-norme stellaire sur A. On a donc $\|\varphi (x)\|\leqslant \|x\|_*$ pour tout $x\in A$. Le morphisme $\varphi$ définit donc par passage au quotient un morphisme continu de $A/R$ dans B, qui se prolonge par continuité en un morphisme $\varphi '$ de Stell(A) dans B vérifiant $\varphi =\varphi '\circ j$. L’unicité de $\varphi '$ résulte de ce que l’image de $j$ est dense dans Stell(A).

#### Corollaire {#ts-i-s6-n12-cor-1 .statement tag=02EX}

Soient A une algèbre de Banach involutive commutative et $j$ le morphisme canonique de A dans Stell(A). L’application $\mathsf{X}(j)$ est un homéomorphisme de $\mathsf{X}$(Stell(A)) sur le sous-espace $\mathsf{X}(A)_h$ de $\mathsf{X}(A)$ formé des caractères hermitiens de A.

Les caractères hermitiens de A sont les morphismes d’algèbres involutives de A dans l’algèbre stellaire $\mathbf{C}$. La prop. 20 entraîne donc que $\mathsf{X}(j)$ est une bijection de $\mathsf{X}$(Stell(A)) sur $\mathsf{X}(A)_h$. Comme $\mathsf{X}(j)$ est un homéomorphisme sur son image (cf. I, p. 10), le corollaire en résulte.

On identifie $\mathsf{X}$(Stell(A)) à $\mathsf{X}(A)_h$ par l’application $\mathsf{X}(j)$. Pour tout $x\in$ A, l’application $\mathscr{G}_{Stell(A)}(j(x))$ n’est autre que la restriction à $\mathsf{X}(A)_h$ de $\mathscr{G}_A(x)$.

#### Proposition 21 {#ts-i-s6-prop-21 .statement tag=02EY}

Soient A une algèbre de Banach involutive et $j$ le morphisme canonique de A dans Stell(A). Le radical de A est contenu dans le noyau de $j$.

Soit $x$ un élément du radical de A. Alors $x^*x$ appartient au radical de A, et donc Sp$'_A(x^*x) =\{0\}($I, p. 5, remarque 3). Puisque Sp$'_{Stell(A)}(j(x^*x))\subset$ Sp$'_A(x^*x)$, on a donc Sp$'_{Stell(A)}(j(x)^*j(x)) =\{0\}$, d’où $\|j(x)\|^2=\|j(x)^*j(x)\|=\varrho (j(x)^*j(x)) = 0$ (formule (2) de I, p. 104), et donc $j(x) = 0$.

### 13. Algèbre stellaire d’un groupe localement compact

#### Définition 9 {#ts-i-s6-def-9 .statement tag=02EZ}

Soit G un groupe localement compact et soit A l’algèbre de Banach involutive des mesures bornées sur G admettant une densité par rapport à une mesure de Haar sur G (exemple 4 de I, p. 99). On appelle algèbre stellaire de G l’algèbre stellaire enveloppante de l’algèbre de Banach involutive A. On la note Stell(G).

#### Remarque {#ts-i-s6-n13-rem-1 .statement tag=02F0}

Soit $\nu$ une mesure de Haar à gauche sur G et soit Δ son module. L’application $f\mapsto f\cdot \nu$ est un isomorphisme isométrique de l’algèbre $L^1(G, \nu )$ sur A (loc. cit.). On peut donc aussi définir Stell(G) comme l’algèbre stellaire enveloppante de l’algèbre normée involutive $L^1(G, \nu )$.

Soit G un groupe localement compact et soit $\nu$ une mesure de Haar à gauche sur G. Pour $\mu\in \mathscr{M}^1(G)$ et $f\in L^2(G, \nu )$, on a $\mu*f\in L^2(G, \nu )$ (INT, VIII, §4, prop. 6). Notons alors $\boldsymbol{\gamma }(\mu)$ l’endomorphisme $f\mapsto \mu*f$ de $L^2(G, \nu )$. L’application $\mu\mapsto \boldsymbol{\gamma }(\mu)$ est une représentation de l’algèbre $\mathscr{M}^1(G)$ dans l’algèbre de Banach $\mathscr{L}(L^2(G, \nu ))$ des endomorphismes continus de $L^2(G, \nu )$ (INT, VIII, §4, cor. de la prop. 6). D’autre part, $\boldsymbol{\gamma }(\check{\mu})$ est la transposée de l’endomorphisme $\boldsymbol{\gamma }(\mu)$ (INT, VIII, §4, n$^o3$, prop. 8). Il en résulte que $\boldsymbol{\gamma }(\mu^*)$ est l’endomorphisme adjoint de $\boldsymbol{\gamma }(\mu)$, et donc que l’application $\boldsymbol{\gamma }:\mu\mapsto \boldsymbol{\gamma }(\mu)$ est un morphisme d’algèbres involutives de $\mathscr{M}^1(G)$ dans l’algèbre stellaire $\mathscr{L}(L^2(G, \nu ))$, appelé la représentation régulière gauche de $\mathscr{M}^1(G)$ dans $L^2(G, \nu )$. D’après INT, VIII, §4, n$^o7$, prop. 19, cette représentation est fidèle.

Soit $j$ l’application canonique de $L^1(G, \nu )$ dans Stell(G). Par restriction à $L^1(G, \nu )$, la représentation régulière $\boldsymbol{\gamma }$ définit un morphisme injectif d’algèbres involutives de $L^1(G, \nu )$ dans $\mathscr{L}(L^2(G, \nu ))$, appelé représentation régulière gauche de $L^1(G)$ dans $L^2(G)$. D’après la prop. 20, il existe un unique morphisme $\boldsymbol{\gamma }':$ Stell(G) $\rightarrow \mathscr{L}(L^2(G, \nu ))$ tel que $\boldsymbol{\gamma }=\boldsymbol{\gamma }'\circ j$. On dit que $\boldsymbol{\gamma }'$ est la représentation régulière gauche de Stell(G) dans $L^2(G, \nu )$. Par abus de notation, nous noterons encore

$$
\boldsymbol{\gamma }'(\varphi )(f) =\varphi *f \tag{7}
$$

pour $f\in L^2(G, \nu )$ et $\varphi \in$ Stell(G). On a

$$
\|\varphi *f\|_2\leqslant \|\varphi \|_*\|f\|_2 \tag{8}
$$

#### Remarque {#ts-i-s6-n13-rem-2 .statement tag=02F1}

En général, la représentation régulière gauche $\boldsymbol{\gamma }'$ de Stell(G) dans $L^2(G, \nu )$ n’est pas fidèle. On peut démontrer qu’elle l’est si et seulement si il existe sur $L^{\infty}_{\mathbf{R}}(G)$ une forme linéaire positive $f$ telle que $f(1) = 1$ et $f(\boldsymbol{\gamma }(g)x) =f(x)$ pour tout $(g, x)\in G\times G$ (on dit alors que le groupe G est moyennable, cf. EVT, IV, p. 73, exercice 4).

#### Proposition 22 {#ts-i-s6-prop-22 .statement tag=02F2}

L’application canonique $j$ de $L^1(G, \nu )$ dans Stell(G) est injective et d’image dense.

L’image de $j$ est dense par définition de l’algèbre stellaire enveloppante d’une algèbre normée involutive. Puisque la représentation régulière gauche $\boldsymbol{\gamma }$ est fidèle, l’injectivité de $j$ résulte de l’égalité $\boldsymbol{\gamma }=\boldsymbol{\gamma }'\circ j$.

#### Corollaire {#ts-i-s6-n13-cor-1 .statement tag=02F3}

L’algèbre $L^1(G, \nu )$ est sans radical.

Ceci résulte de la prop. 21 de I, p. 125 et de la prop. 22.

On peut donc identifier $L^1(G, \nu )$ à une sous-algèbre involutive dense de Stell(G), et l’injection canonique de $L^1(G, \nu )$ dans Stell(G) est alors continue.

Supposons maintenant que le groupe G soit unimodulaire (INT, VII, §1, n$^o3$, déf. 3). On peut alors répéter les mêmes arguments à partir de la représentation régulière droite $(f, \mu)\mapsto \boldsymbol{\delta }(\mu)(f) =f*\check{\mu}$ de $L^2(G, \nu )\times \mathscr{M}^1(G)$ dans $L^2(G, \nu )$. On définit alors un morphisme $\boldsymbol{\delta }'$ de Stell(G) dans $\mathscr{L}(L^2(G, \nu ))$ tel que $\boldsymbol{\delta }=\boldsymbol{\delta }'\circ j$, et on note $\boldsymbol{\delta }'(\varphi )(f) =f*\varphi$ pour $f\in L^2(G, \nu )$ et $\varphi \in$ Stell(G).

Pour $\varphi , \psi \in$ Stell(G), on a $\boldsymbol{\delta }'(\psi )\circ \boldsymbol{\gamma }'(\varphi ) =\boldsymbol{\gamma }'(\psi )\circ \boldsymbol{\delta }'(\varphi )$, c’est-à-dire

$$
(\varphi *f)*\psi =\varphi *(f*\psi ) \tag{9}
$$

pour tout $f\in L^2(G, \nu )$. En effet, cette formule est vraie pour $\varphi , \psi \in$ $L^1(G, \nu )$, et les applications $(\varphi , \psi )\mapsto (\varphi *f)*\psi$ et $(\varphi , \psi )\mapsto \varphi *(f*\psi )$ sont des applications bilinéaires continues de Stell(G) $\times$ Stell(G) dans $L^2(G, \nu )$.

## EXERCICES {#ts-i-s6-exercises}

See the [exercises for § 6](exercises/s6/).
