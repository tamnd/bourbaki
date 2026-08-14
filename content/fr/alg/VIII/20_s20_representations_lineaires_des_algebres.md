---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 20
section_title: Représentations linéaires des algèbres
lang: fr
source: alg-viii-fr
book_pages: A VIII.365-A VIII.386
pdf_pages: 0367-0388
extraction: native
subsections:
    - "no": 1
      title: Représentations linéaires des algèbres
      page: 365
      pdf_page: 367
    - "no": 2
      title: Dual restreint d’une algèbre
      page: 367
      pdf_page: 369
    - "no": 3
      title: Coefficients d’un module
      page: 368
      pdf_page: 370
    - "no": 4
      title: Dual restreint et coefficients matriciels
      page: 371
      pdf_page: 373
    - "no": 5
      title: Dual d’une algèbre semi-simple
      page: 371
      pdf_page: 373
    - "no": 6
      title: Caractère d’une représentation
      page: 374
      pdf_page: 376
    - "no": 7
      title: Coefficients d’un ensemble de classes de modules
      page: 379
      pdf_page: 381
    - "no": 8
      title: Structure de cogèbre sur le dual restreint
      page: 380
      pdf_page: 382
statements: 31
exercises: 6
content_sha256: 7108f6bd4c3b6c681b554709f31ce438c5f5fbdef631046cd35b996d3ddfe841
---

## § 20. REPRÉSENTATIONS LINÉAIRES DES ALGÈBRES

Dans ce paragraphe, on note K un anneau commutatif et A une K-algèbre. À partir du n$^o2$, on suppose que K est un corps, et l’on note $A^*$ le dual de l’espace vectoriel A sur K ; la notation $A^*$ ne désignera jamais le groupe multiplicatif de l’anneau A.

### 1. Représentations linéaires des algèbres

#### Définition 1 {#alg-viii-s20-def-1 .statement tag=00MD}

Soit M un K-module. On appelle représentation linéaire de l’algèbre A dans M un K-homomorphisme $\pi$ de A dans l’algèbre End$_K(M)$.

On dit aussi que le couple $(M, \pi )$ est une représentation linéaire de l’algèbre A. Lorsque M est un K-module libre, la dimension de M est appelée le degré (ou la dimension) de $\pi$.

Soit $\pi$ une représentation linéaire de A dans M. La loi additive sur M et la loi d’action $(a, x)\rightarrow \pi (a)(x)$ définissent sur M une structure de A-module à gauche, que l’on note $M_{\pi}$. On dit que $M_{\pi}$ est le module de la représentation $\pi$. La structure de K-module sur M est obtenue par restriction des scalaires à partir de la structure de A-module sur $M_{\pi}$.

Réciproquement, soit E un A-module à gauche. Soit M le K-module déduit de E par restriction des scalaires de A à K et soit $\pi$ l’homomorphisme $a\rightarrow a_E$ de A dans End$_K(M)$. Alors $\pi$ est une représentation de A dans M et l’on a $E = M_{\pi}$. On dit que $\pi$ est la représentation linéaire associée au A-module E.

Il revient au même d’étudier les A-modules ou les représentations linéaires de A. Nous allons traduire en langage de représentations linéaires certaines définitions relatives aux modules.

Soit $\pi$ une représentation linéaire de A dans M. Le noyau de l’homomorphisme$\pi$ est un idéal bilatère de A, qui n’est autre que l’annulateur du A-module $M_{\pi}$. L’homomorphisme $\pi$ est injectif si et seulement si le A-module $M_{\pi}$ est fidèle ; on dit alors que $\pi$ est une représentation fidèle de A.

Soient $(M, \pi )$ et $(M', \pi ')$ des représentations linéaires de A. Une application A-linéaire de $M_{\pi}$ dans $M'_{\pi'}$ est une application K-linéaire $u: M\rightarrow M'$ qui satisfait à la relation

$$
\pi '(a)\circ u=u\circ \pi (a) \tag{1}
$$

pour $a\in A$. Un isomorphisme de $M_{\pi}$ sur $M'_{\pi'}$ est un isomorphisme de K-modules $u: M\rightarrow M'$ satisfaisant à la condition

$$
\pi '(a) =u\circ \pi (a)\circ u^{-1} \tag{2}
$$

pour $a\in A$. On dit que $\pi$ et $\pi '$ sont isomorphes si les A-modules $M_{\pi}$ et $M'_{\pi'}$ sont isomorphes. On dit que $\pi$ est une sous-représentation (resp. une représentation quotient) de $\pi '$ si $M_{\pi}$ est un sous-module (resp. un module quotient) de $M'_{\pi'}$.

Supposons donnée une famille $(M_i, \pi_i)$ de représentations linéaires de A. Soit M le K-module somme directe des $M_i$; pour tout $a\in A$, soit $\pi (a)$ l’endomorphisme $(x_i)_{i\in I}\rightarrow (\pi_i(a)(x_i))_{i\in I}$ de M. Alors $\pi$ est une représentation linéaire de A dans M. Le A-module $M_{\pi}$ est somme directe de la famille des A-modules $(M_i)_{\pi_i}(i\in I)$; on dit que $\pi$ est la somme directe des $\pi_i$, et l’on écrit $\pi =\bigoplus\pi_i$.

On dit que la représentation $\pi$ de A dans M est simple ou irréductible si le A-module $M_{\pi}$ est simple ; on dit que la représentation $\pi$ de A dans M est semi-simple, ou complètement réductible, si le A-module $M_{\pi}$ est semi-simple.

Soit $\pi$ une représentation linéaire de A dans M. Soit $M^*$ le K-module dual de M. L’application $a\rightarrow^t(\pi (a))$ de $A^o$ dans End$_K(M^*)$ est la représentation transposée de $\pi$.

Soit L une K-algèbre commutative et soit $(M, \pi )$ une représentation linéaire de la K-algèbre A. L’homomorphisme $\pi_{(L)}: A_{(L)}\rightarrow$ End$_L(M_{(L)})$ correspondant à la structure de $A_{(L)}$-module de $M_{(L)}$ est une représentation linéaire de la L-algèbre $A_{(L)}$. On dit que $\pi_{(L)}$ est la représentation linéaire de l’algèbre $A_{(L)}$ déduite de la représentation $\pi$ par extension à L de l’anneau K des scalaires.

Supposons que K soit un corps et que L soit une K-algèbre commutative non nulle. Soient $\pi$ et $\pi '$ des représentations linéaires de l’algèbre A. Il résulte de VIII, p. 34, th. 3 que les représentations $\pi$ et $\pi '$ sont isomorphes si et seulement si $\pi_{(L)}$ et $\pi_{(L)}'$ le sont.

Supposons que K soit un corps. Soit L une extension de K. Considérons le groupe de Grothendieck $R_K(A)$ (resp. $R_L(A_{(L)}))$ des A-modules de dimension finie sur K (resp. des $A_{(L)}$-modules de dimension finie sur L). Nous avons vu que l’homomorphisme de groupes

$$
u: R_K(A)\longrightarrow R_L(A_{(L)})
$$

défini par l’extension des scalaires est injectif ; en outre, un élément $\xi \in R_K(A)$ est effectif si et seulement si $u(\xi )$ l’est (VIII, p. 191, th. 1).

### 2. Dual restreint d’une algèbre

On suppose désormais que K est un corps.

Pour $a\in A$, notons $\boldsymbol{\gamma }(a)$ l’application $x\rightarrow ax$ et $\boldsymbol{\delta }(a)$ l’application $x\rightarrow xa$ de A dans A. Alors $\boldsymbol{\gamma }$ est une représentation linéaire de A dans A, appelée représentation régulière gauche ; de même, $\boldsymbol{\delta }$ est une représentation linéaire de $A^o$ dans A, appelée (par abus de langage) la représentation régulière droite de A. Par transposition, on déduit de $\boldsymbol{\delta }$ et $\boldsymbol{\gamma }$ des représentations linéaires des algèbres A et $A^o$ dans l’espace vectoriel $A^*$ qui définissent sur $A^*$ une structure de A-module à gauche, et une structure de $A^o$-module à gauche. Ces deux structures correspondent à une structure de $(A$, A)-bimodule sur $A^*$ dont les lois d’action sont définies par les formules

$$
\langle af, b\rangle =\langle f, ba\rangle \tag{3}
$$

$$
\langle f a, b\rangle =\langle f, ab\rangle \tag{4}
$$

pour $a, b\in A$ et $f\in A^*$.

On rappelle (II, p. 42, déf. 4) que si E est un sous-espace vectoriel de A, son orthogonal $E'$ dans $A^*$ est l’ensemble des formes linéaires sur A dont la restriction à E est nulle. De même l’orthogonal $F'$ dans A d’un sous-espace vectoriel F de $A^*$ est l’intersection des noyaux des formes linéaires appartenant à F.

On sait (II, p. 104, th. 7) que l’application $\varphi : E\rightarrow E'$ est une bijection de l’ensemble des sous-espaces vectoriels de codimension finie de A sur l’ensemble des sous-espaces vectoriels de dimension finie de $A^*$. L’application réciproque $\varphi^{-1}$ associe à chaque sous-espace F de dimension finie de $A^*$ son orthogonal $F'$ dans A.

#### Proposition 1 {#alg-viii-s20-prop-1 .statement tag=00ME}

a) L’application $\varphi$ induit une bijection de l’ensemble des idéaux à gauche (resp. à droite, resp. bilatères) de A, de codimension finie, sur l’ensemble des sous-A-modules à droite (resp. des sous-A-modules à gauche, resp. des sous-bimodules) de $A^*$, de dimension finie sur K.

b) Tout idéal à gauche ou à droite de A, de codimension finie, contient un idéal bilatère de codimension finie.

Les formules (3) et (4) démontrent que si E est un idéal à gauche de A, alors $E'$ est un sous-A-module à droite de $A^*$; si V est un sous-A-module à droite de $A^*$, alors $V'$ est un idéal à gauche de A. Le cas des idéaux à droite et celui des idéaux bilatères se traitent de manière analogue. Ceci démontre a).

Soit $\mathfrak{a}$ un idéal à gauche de A, de codimension finie. Le A-module à gauche $E = A_s/\mathfrak{a}$ est de dimension finie sur K et il en est de même de End$_K(E)$. Le noyau de l’homomorphisme $a\rightarrow a_E$ de A dans End$_K(E)$ est donc un idéal bilatère de codimension finie de A, contenu dans $\mathfrak{a}$. Passant à l’anneau opposé $A^o$, on voit que tout idéal à droite, de codimension finie dans A, contient un idéal bilatère de codimension finie.

#### Définition 2 {#alg-viii-s20-def-2 .statement tag=00MF}

On appelle dual restreint de la K-algèbre A, et l’on note Θ(A), la réunion dans $A^*$ des orthogonaux des idéaux bilatères de codimension finie de A.

D’après la prop. 1, on peut donner les caractérisations suivantes de Θ(A) ; c’est au choix :

– la réunion des orthogonaux des idéaux à gauche de codimension finie de A ;

– la réunion des orthogonaux des idéaux à droite de codimension finie de A ;

– la réunion des orthogonaux des idéaux bilatères de codimension finie de A ;

– la réunion des sous-A-modules à gauche de $A^*$ de dimension finie sur K ;

– la réunion des sous-A-modules à droite de $A^*$ de dimension finie sur K ;

– la réunion des sous-(A, A)-bimodules de $A^*$ de dimension finie sur K.

On a $\Theta (A) = \Theta (A^o)$, et $\Theta (A) = A^*$ si A est de degré fini sur K. Soit $f\in A^*$; pour que $f$ appartienne à Θ(A), il faut et il suffit que $Af$ (resp. $fA$, resp. $AfA)$ soit un sous-espace vectoriel de $A^*$ de dimension finie sur K.

La somme de deux sous-(A, A)-bimodules de $A^*$ de dimension finie sur K est de dimension finie sur K. Il en résulte que Θ(A) est un sous-(A, A)-bimodule de $A^*$.

### 3. Coefficients d’un module

Soit E un A-module à gauche. Soit $E^*$ le dual de l’espace vectoriel E sur K ; on le munit de sa structure naturelle de A-module à droite. Étant donnés des éléments $x$ de E et $x^*$ de $E^*$, on note $c_E(x, x^*)$ la forme linéaire

$$
c_E(x, x^*) :a\rightarrow  \langle x^*, ax\rangle \tag{5}
$$

sur A. Ces formes linéaires s’appellent les coefficient de E. Le sous-espace de $A^*$ engendré par les coefficients de E se note $\Theta_E(A)$. Il est non nul si E est non nul.

Si F est un A-module isomorphe à E, alors E et F ont mêmes coefficients et l’on a $\Theta_F(A) = \Theta_E(A)$. Considérons $E^*$ comme un $A^o$-module à gauche, un coefficient de E est un coefficient de $E^*$ et $\Theta_E(A)\subset \Theta_{E^*}(A^o)$. Par suite, si E est de dimension finie sur K, alors E et $E^*$ ont mêmes coefficients et l’on a $\Theta_E(A) = \Theta_{E^*}(A^o)$.

Soit $(M, \pi )$ une représentation linéaire de l’algèbre A. Les coefficients du A-module $M_{\pi}$ sont aussi appelés les coefficients de la représentation $\pi$. Le coefficient $c_{M_{\pi}}(x, x^*)$, pour $x\in M$ et et $x^*\in M^*$, se note aussi $c_{\pi}(x, x^*)$; l’espace vectoriel $\Theta_{M_{\pi}}(A)$ est aussi noté $\Theta_{\pi}(A)$.

#### Remarque 1 {#alg-viii-s20-n3-rem-1 .statement tag=00MG}

Supposons que M soit de dimension finie sur K ; Soit $(e_1, . . . , e_n)$ une base de V et soit $(e^*_1, . . . , e^*_n)$ sa base duale. Notons $(\pi_{ij}(a))$ la matrice de $\pi (a)$ par rapport à la base $(e_1, . . . , e_n)$ de V ; on a $\pi_{ij}=c_{\pi}(e_j, e^*_i)$. L’application $a\rightarrow (\pi_{ij}(a))$ est un homomorphisme de A dans $\mathbf{M}_n(K)$; un tel homomorphisme est parfois appelé représentation matricielle de l’algèbre A.

#### Remarque 2 {#alg-viii-s20-n3-rem-2 .statement tag=00MH}

Soit E un A-module et soit $E'$ un sous-module de E. Par le cor. du th. 5 de II, p. 102, on a $\Theta_{E'}(A)\subset \Theta_E(A)$ et $\Theta_{E/E'}(A)\subset \Theta_E(A)$.

Soit $\gamma_E$ l’unique application K-linéaire de $E\otimes_KE^*$ dans $A^*$ qui à $x\otimes x^*$ associe $c_E(x, x^*)$. Elle est $(A$, A)-bilinéaire et son image est $\Theta_E(A)$. On en déduit des applications A-linéaires $c'_E: E\rightarrow$ Hom$_A(E^*,A^*)$ et $c''_E: E^*\rightarrow$ Hom$_A(E,A^*)$ telles que

$$
c'_E(x)(x^*) =c_E(x, x^*) =c''_E(x^*)(x)
$$

Notons $\theta_E$ l’application K-linéaire $\theta_E: E\otimes E^*\rightarrow$ End$_K(E)$ caractérisée par la relation

$$
\theta_E(x\otimes x^*)(y) =\langle x^*, y\rangle x
$$

pour $x, y\in E$ et $x^*\in E^*$. Son image est l’ensemble End$^f_K(E)$ des endomorphismes de rang fini de E (VIII, p. 453). Par définition de la trace (loc. cit.), on a

Tr($\theta_E(x\otimes x^*)$) $=\langle x^*, x\rangle$

pour $x\in E$ et $x^*\in E^*$; on a donc

$\langle \gamma_E(x\otimes x^*), a\rangle =\langle x^*, ax\rangle =$ Tr($\theta_E(ax\otimes x^*)$) $=$ Tr($\theta_E(x\otimes x^*)a$).

On en déduit la relation

$\langle \gamma_E(h), a\rangle =$ Tr($\theta_E(h)\circ a_E$) pour $a\in A$ et $h\in E\otimes_KE^*$. Ceci démontre que $\Theta_E(A)$ est l’ensemble des formes linéaires $a\rightarrow$ Tr($u\circ a_E$) sur A, où $u$ parcourt End$^f_K(E)$.

#### Lemme 1 {#alg-viii-s20-lem-1 .statement tag=00MI}

L’application $c''_E$ est bijective. Si E est de dimension finie, il en est de même de $c'_E$.

Si F est un A-module à droite et G un K-espace vectoriel, on a défini en II, p. 74, prop. 1 a), un isomorphisme $\gamma$ de K-espaces vectoriels de Hom$_K(F\otimes_AE,G)$ sur Hom$_A(E$, Hom$_K(F,G))$. Cet isomorphisme associe à $\varphi : F\otimes_AE\rightarrow G$ l’homomorphisme $e\rightarrow (f\rightarrow \varphi (f\otimes e))$. Compte tenu de l’isomorphisme canonique de $A_d\otimes_AE$ avec E (II, p. $56),\gamma$ s’identifie à $c''_E$ dans le cas où $F = A_d, G = K$.

De manière analogue, l’isomorphisme$\beta$ défini en II, p. 74, prop. 1 b) se spécialise en un isomorphisme $\beta$ de Hom$_K(E^*\otimes_AA_s,K)$ sur Hom$_A(E^*$, Hom$_K(A_s,K))$. Lorsque E est de dimension finie, E s’identifie canonique à Hom$_K(E^*,K)$ et $E^*$ à $E^*\otimes_AA_s$, l’homomorphisme $\beta$ s’identifie alors à $c'_E$.

#### Proposition 2 {#alg-viii-s20-prop-2 .statement tag=00MJ}

Soit E un A-module à gauche.

a) L’ensemble des coefficients de E est la réunion des images des applications A-linéaires de E dans $A^*$.

b) Supposons en outre que E soit de dimension finie $n$ sur K. Alors le A-module à gauche $\Theta_E(A)$est isomorphe à un quotient de $E^n$, le A-module E est isomorphe à un sous-module de $\Theta_E(A)^n$ et tout élément de $\Theta_E(A)$est un coefficient de $E^n$.

L’assertion a) résulte de la surjectivité de $c''_E$.

Démontrons b). Soit $(e^*_1, . . . , e^*_n)$ une base de $E^*$ sur K. Comme $\Theta_E(A)$ est engendré par les coefficients de E, l’application A-linéaire

$$
(x_1, . . . , x_n)\rightarrow \sum_{i=1}^nc_E(x_i, e^*_i)
$$

de $E^n$ dans $\Theta_E(A)$ est surjective. D’après a), tout élément de $\Theta_E(A)$ est un coefficient de $E^n$. Par ailleurs, l’application A-linéaire

$$
x\rightarrow (c_E(x, e^*_1), . . . , c_E(x, e^*_n))
$$

de E dans $\Theta_E(A)^n$ est injective, d’où b).

#### Remarque 3 {#alg-viii-s20-n3-rem-3 .statement tag=00MK}

Soit E un sous-A-module à gauche de $A^*$. Soit $\varepsilon$ la forme linéaire $y\rightarrow y(1)$ sur E. Pour tout $x$ dans E, on a $x=c_E(x, \varepsilon )$, donc E est un sous-A-module de $\Theta_E(A)$.

### 4. Dual restreint et coefficients matriciels

#### Proposition 3 {#alg-viii-s20-prop-3 .statement tag=00ML}

Soit $(V, \pi )$une représentation linéaire de dimension finie de l’algèbre A. Le noyau $\mathfrak{a}$ de $\pi$ est un idéal bilatère de codimension finie de A, et $\Theta_{\pi}(A)$ est l’orthogonal de $\mathfrak{a}$ dans $A^*$. L’application transposée de $\pi$ définit un isomorphisme du dual du K-espace vectoriel $\pi (A)$sur $\Theta_{\pi}(A)$.

Comme End$_K(V)$ est de dimension finie sur $K,\mathfrak{a}$ est un idéal bilatère de codimension finie de A. L’espace vectoriel $\Theta_{\pi}(A)$ est un sous-espace de dimension finie de $A^*$ et son orthogonal dans A est égal à $\mathfrak{a}$; d’après le th. 7 de II, p. 104, l’espace $\Theta_{\pi}(A)$ est donc l’orthogonal de $\mathfrak{a}$ dans $A^*$. De plus, comme $\mathfrak{a}$ est le noyau de $\pi$, l’application transposée de $\pi$ définit un isomorphisme du dual de $\pi (A)$ sur l’orthogonal de $\mathfrak{a}$ dans $A^*$ (II, p. 102, cor. du th. 5).

#### Corollaire {#alg-viii-s20-n4-cor-1 .statement tag=00MM}

Le dual restreint Θ(A) de A est l’ensemble des coefficients des représentations linéaires de dimension finie de A.

Par définition, Θ(A) est la réunion des orthogonaux des idéaux bilatères de codimension finie de A. On a donc $\Theta_{\pi}(A)\subset \Theta (A)$ pour toute représentation linéaire de dimension finie $\pi$ de A. Réciproquement, soit $f$ un élément de Θ(A) et soit $\mathfrak{a}$ un idéal bilatère de codimension finie, contenu dans le noyau de $f$ (VIII, p. 368, déf. 2). Notons $\pi$ la représentation linéaire de A dans $A/\mathfrak{a}$ déduite par passage au quotient de la représentation régulière gauche dans A ; soit $x$ la classe de 1 (mod. $\mathfrak{a})$, et $x^*$ la forme linéaire sur $A/\mathfrak{a}$ déduite de $f$. On a $f=c_{\pi}(x, x^*)$, de sorte que $f$ est un coefficient de $\pi$.

☡ On prendra garde que si $(V, \pi )$ est une représentation linéaire de A qui n’est pas de dimension finie sur K, l’espace $\Theta_{\pi}(A)$ n’est pas nécessairement contenu dans Θ(A).

### 5. Dual d’une algèbre semi-simple

Soit $\Theta^{ss}(A)$ le socle du A-module à gauche Θ(A), c’est-à-dire (VIII, p. 61) le plus grand sous-module semi-simple de Θ(A). On note $\mathscr{S}_K$ l’ensemble des classes des A-modules (à gauche) simples qui sont de dimension finie sur K. Lorsque A est une algèbre semi-simple de degré fini sur K, on a $A^*= \Theta (A) = \Theta^{ss}(A)$ puisque tout A-module à gauche est semi-simple (VIII, p. 134, prop. 4).

#### Théorème 1 {#alg-viii-s20-thm-1 .statement tag=00MN}

a) L’ensemble $\Theta^{ss}(A)$se compose des coefficients des représentations semi-simples de dimension finie de A. C’est un sous-$(A,A)$-bimodule de $A^*$.

b) Pour tout $S\in \mathscr{S}_K$, le composant isotypique de type S de Θ(A) est égal à $\Theta_S(A)$;le A-module à gauche $\Theta^{ss}(A)$est somme directe des sous-modules $\Theta_S(A)$, où S parcourt $\mathscr{S}_K$.

c) Pour tout S dans $\mathscr{S}_K$, le A-module à droite $S^*$ est simple et $\Theta_S(A)$est le composant isotypique de type $S^*$ du A-module à droite Θ(A). L’application qui à S associe cl(S$^*)$est une bijection de $\mathscr{S}_K$ sur l’ensemble des classes de $A^o$-modules simples de dimension finie sur K.

d) Considéré comme A-module à droite, Θ(A) a pour socle $\Theta^{ss}(A)$.

Soit E un A-module semi-simple de dimension finie sur K. Tout coefficient de E appartient à l’image d’une application A-linéaire de E dans $A^*$ (VIII, p. 370, prop. 2) donc appartient à $\Theta^{ss}(A)$. Inversement soit $f\in \Theta^{ss}(A)$. Alors le A-module $Af$ est de dimension finie sur K et est semi-simple. Par la remarque VIII, p. 358$,f$ est un coefficient de $Af$.

Pour tout S dans $\mathscr{S}_K$, le composant isotypique de type S de Θ(A) est engendré par les images des applications A-linéaires de S dans $A^*$; il est donc égal à $\Theta_S(A)$ d’après la prop. 2, a) de VIII, p. 370. D’autre part, si S est un A-module simple qui n’est pas de dimension finie sur K, le composant isotypique de type S de Θ(A) est nul : en effet, tout sous-module simple de Θ(A) est monogène, donc de dimension finie sur K. Comme le socle de Θ(A) est somme directe de ses composants isotypiques (VIII, p. 61, prop. 4), cela démontre b).

Soit S un A-module simple, de dimension finie sur K. Comme le K-espace vectoriel S n’est pas réduit à 0, il en est de même de $S^*$. Soit E un sous-module du A-module à droite $S^*$; son orthogonal $E'$ dans S est un sous-A-module de S ; comme S est simple, on a ou bien $E'= 0$, d’où $E = S^*$, ou bien $E'= S$, d’où E = 0. Donc $S^*$ est un A-module à droite simple.

On a $\Theta (A^o) = \Theta (A)$ (VIII, p. 368) ; on identifie A-modules à droite et $A^o$-modules à gauche. Comme tout espace vectoriel de dimension finie sur K est isomorphe à son bidual, ce qui précède démontre que l’application $S\rightarrow$ cl(S$^*)$ est une bijection de $\mathscr{S}_K$ sur l’ensemble des classes de $A^o$-modules simples de dimension finie sur K. Or, pour S dans $\mathscr{S}_K$, le composant isotypique de type $S^*$ de $\Theta (A^o)$ est égal à $\Theta_{S^*}(A^o)$ d’après l’assertion b) du th. 1 appliquée à l’algèbre $A^o$, et l’on a $\Theta_{S^*}(A^o) = \Theta_S(A)$. Les assertions c) et d) résultent aussitôt de là.

#### Corollaire 1 {#alg-viii-s20-thm-1-cor-1 .statement tag=00MO}

Toute A-module simple de dimension finie sur K est isomorphe à un sous-A-module de Θ(A).

Cela résulte du th. 1, b) car on a $\Theta_E(A)\not= 0$ pour tout A-module non nul E.

#### Corollaire 2 {#alg-viii-s20-thm-1-cor-2 .statement tag=00MP}

Si deux A-modules simples de dimension finie de A ont un même coefficient non nul, ils sont isomorphes.

Soient $S_1$ et $S_2$ des A-modules simples de dimension finie sur K ayant un même coefficient non nul. On a alors $\Theta_{S_1}(A)\cap \Theta_{S_2}(A)\not= 0$. Or $\Theta_{S_1}(A)$ est isotypique de type $S_1$ et $\Theta_{S_2}(A)$ de type $S_2$. Donc $S_1$ est isomorphe à $S_2$.

D’après le théorème 1, $\Theta^{ss}(A)$ est un sous-(A, A)-bimodule de $A^*$, somme directe des $(A$, A)-bimodules $\Theta_S(A)$ pour S parcourant $\mathscr{S}_K$; ces bimodules sont deux à deux non isomorphes, puisqu’ils sont déjà non isomorphes comme A-modules à gauche.

Fixons S dans $\mathscr{S}_K$. Notons D le corps opposé de End$_A$(S), et considérons S comme D-module à droite et $S^*$ comme un D-module à gauche. Avec ces conventions, S est un $(A$, D)-bimodule, $S^*$ est un $(D$, A)-bimodule, et $S\otimes_DS^*$ est un $(A,A)$-bimodule.

#### Proposition 4 {#alg-viii-s20-prop-4 .statement tag=00MQ}

a) Il existe un homomorphisme de groupes $\lambda_S$ de $S\otimes_DS^*$ dans $\Theta_S(A)$, caractérisé par

$$
\lambda_S(x\otimes x^*) =c_S(x, x^*) \tag{6}
$$

pour $x\in S$et $x^*\in S^*$. Cette application est un isomorphisme de $(A,A)$-bimodules.

b) Le $(A,A)$-bimodule $\Theta_S(A)$est simple.

L’application $\gamma_S: S\otimes_KS^*\rightarrow \Theta_S(A)$ caractérisée par la formule $\gamma_S(x\otimes x^*) =$ $c_S(x, x^*)$ est $(A$, A)-linéaire et surjective et satisfait à $\gamma_S(xd\otimes x^*) =\gamma_S(x\otimes dx^*)$ pour $x\in S,x^*\in S^*$ et $d\in D$. Elle définit donc une application $(A$, A)-linéaire surjective $\lambda_S: S\otimes_DS^*\rightarrow \Theta_S(A)$ caractérisée par la formule (6).

Prouvons que $S\otimes_DS^*$ est un $(A$, A)-bimodule simple. D’après le cor. 2 de VIII, p. 59, tout sous-(A, A)-bimodule de $S\otimes_DS^*$ est de la forme $S\otimes_DH$, où H est un sous$(D$, A)-bimodule de $S^*$. Comme $S^*$ est un A-module à droite simple (VIII, p. 371, th. 1, c)), on a H = 0 ou $H = S^*$, d’où notre assertion.

L’homomorphisme $\lambda_S$ est $(A$, A)-linéaire et non nul ; comme $S\otimes_DS^*$ est un bimodule simple, $\lambda_S$ est injectif (VIII, p. 43, prop. 2, a)).

#### Remarque {#alg-viii-s20-n5-rem-1 .statement tag=00MR}

Lorsque le corps K est algébriquement clos, on a D = K d’après le th. 1 de VIII, p. 43 et $\lambda_S$ est un isomorphisme de $(A$, A)-bimodules de $S\otimes_KS^*$ sur $\Theta_S(A)$.

### 6. Caractère d’une représentation

Soit E est un A-module à gauche, de dimension finie sur K. On appelle caractère de E ou trace de E, et l’on note Tr$_E$, la forme linéaire $a\rightarrow$ Tr($a_E$). Soient $(e_1, . . . , e_n)$ une base de E et $(e^*_1, . . . , e^*_n)$ sa base duale. Par définition, on a la relation

(7) Tr$_E=\sum_{i=1}^nc_E(e_i, e^*_i)$.

La forme linéaire Tr$_E$ appartient à $\Theta_E(A)$. On a Tr$_E=$ Tr$_{E'}$ si E et $E'$ sont deux A-modules isomorphes. Ainsi Tr$_E$ ne dépend que de la classe d’isomorphisme de E.

Soit $\pi$ une représentation linéaire de A dans un espace vectoriel V de dimension finie sur K. On appelle trace de $\pi$, ou parfois caractère de $\pi$, le caractère du A-module $V_{\pi}$. On le note Tr$_{\pi}$. Si $(e_1, . . . , e_n)$ est une base de V sur K et si $(\pi_{ij}(a))$ est la matrice de $\pi (a)$ par rapport à cette base, on a

(8) Tr$_{\pi}(a) =\sum_{i=1}^n\pi_{ii}(a)$.

La forme linéaire Tr$_{\pi}$ appartient à $\Theta_{\pi}(A)$.

#### Proposition 5 {#alg-viii-s20-prop-5 .statement tag=00MS}

Soit S un A-module simple de dimension finie sur K, soit D le corps opposé du commutant de S et soit Z le centre de D. Les conditions suivantes sont équivalentes :

(i) Le caractère Tr$_S$ de S n’est pas nul ;

(ii) Il existe un élément $d\in D$tel que Tr$_{D/K}(d)\not= 0$;

(iii) L’extension Z de K est séparable et la caractéristique $p$ de K ne divise pas le degré [D : Z].

Le D-espace vectoriel à droite S est de dimension finie. Soit $(e_1, . . . , e_n)$ une base de S sur D et soit $u$ un élément de End$_D(S)$. Soit $(d_{ij})$ la matrice de $u$ par rapport à la base $(e_1, . . . , e_n)$. On a $u(e_j) =\sum^n_{i=1}e_id_{ij}$ pour $j\in [1, n]$. Notons $u_K$ l’application $u$, considérée comme endomorphisme du K-espace vectoriel S, et $(u_{ij})$ la matrice de $u_K$ par rapport à la décomposition $(e_iD)$ du K-espace vectoriel S en somme directe (II, p, 146). On a Tr($u_K$) $=\sum_i$ Tr($u_{ii}$). De plus, $u_{ii}$ est l’endomorphisme du K-espace vectoriel $e_iD$ défini par $u_{ii}(e_id) =e_id_{ii}d$ pour $d\in D$, donc sa trace est égale à Tr$_{D/K}(d_{ii})$. Nous avons ainsi démontré l’égalité

(9) Tr($u_K$) $=$ Tr$_{D/K}(\sum_id_{ii})$.

D’après le théorème de Burnside (VIII, p. 79, cor. 1 de la prop. 4), l’application $a\rightarrow a_S$ de A dans End$_D(S)$ est surjective. L’équivalence des conditions (i) et (ii) résulte ainsi de la formule (9).

Si l’extension Z de K est séparable, il existe un élément $d\in$ Z tel que Tr$_{Z/K}(d)\not= 0$ (V, p. 48, cor. de la prop. 1). De plus, on a Tr$_{D/K}(d) = [D : Z]$ Tr$_{Z/K}(d)$ (III, p. 114, cor.) ; par conséquent, si $p$ ne divise pas [D : Z], on a Tr$_{D/K}(d)\not= 0$. Cela prouve que (iii) entraîne (ii).

Si l’extension Z de K n’est pas séparable, on a Tr$_{Z/K}(x) = 0$ pour tout $x\in Z$, d’où Tr$_{D/K}(d) =$ Tr$_{Z/K}$(Tr$_{D/Z}(d)) = 0$ pour tout $d\in D$.

Supposons maintenant que $p$ divise le degré [D : Z]. Il divise alors le degré réduit de D sur Z. Pour tout $d\in D$, on Tr$_{D/Z}(d) = 0$ (VIII, p. 337, remarque), d’où Tr$_{D/K}(d) =$ Tr$_{Z/K}$(Tr$_{D/Z}(d)) = 0$. Cela termine la démonstration de l’implication (ii) $=\Rightarrow$ (iii).

#### Corollaire {#alg-viii-s20-n6-cor-1 .statement tag=00MT}

Si le corps K est parfait, les conditions (i) à (iii) sont satisfaites.

Le corps étant parfait, l’extension Z de K est séparable (V, p. 119, th. 3). La condition (iii) résulte alors du cor. 3 de VIII, p. 318.

#### Proposition 6 {#alg-viii-s20-prop-6 .statement tag=00MU}

Soit $\mathscr{S}_0$ l’ensemble des classes de A-modules simples de dimension finie sur K, dont les traces ne sont pas nulles. La famille de formes linéaires (Tr$_S)_{S\in\mathscr{S}_0}$ est libre sur K.

Soit F une partie finie de $\mathscr{S}_0$ et soit S un élément de F. Par hypothèse, il existe un élément $a\in A$ tel que Tr$_S(a)\not= 0$. D’après le cor. 1 de la prop. 4 (VIII, p. 79) il existe un élément $b\in A$ tel que $b_S=a_S$ et $b_T= 0$ pour tout $T\in F-\{S\}$. On a Tr$_S(b)\not= 0$ et Tr$_T(b) = 0$ pour $T\in F-\{S\}$. La famille (Tr$_S)_{S\in F}$ est donc libre et la proposition 6 en résulte.

#### Remarque {#alg-viii-s20-n6-rem-1 .statement tag=00RR}

Soit $\mathscr{S}_K$ l’ensemble des classes de A-modules simples qui sont de dimension finie sur K. La prop. 6 résulte aussi du fait que la somme des $\Theta_S$(A), pour S parcourant $\mathscr{S}_K$, est directe.

Soit

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

une suite exacte de A-modules, tous de dimension finie sur K. D’après la prop. 1 de III, p. 109, on a Tr$_E=$ Tr$_{E'}+$ Tr$_{E''}$. D’après la définition du groupe de Grothendieck $R_K(A)$ (VIII, p. 189) et sa propriété universelle (VIII, p. 182, prop. 4), il existe un homomorphisme de groupes additifs $\theta$ de $R_K(A)$ dans $A^*$ caractérisé par la relation $\theta ([E]) =$ Tr$_E$ pour tout A-module E de dimension finie sur K. En particulier la trace d’un semi-simplifié de E est égale à celle de E. On déduit de $\theta$ une application K-linéaire $\theta_K: K\otimes_{\mathbf{Z}}R_K(A)\rightarrow A^*$.

#### Corollaire {#alg-viii-s20-n6-cor-2 .statement tag=00MV}

a) Supposons le corps K de caractéristique 0. Les homomorphismes $\theta$ et $\theta_K$ sont injectifs. Pour que deux A-modules, semi-simples et de dimension finie sur K, soient isomorphes, il faut et il suffit que leurs caractères soient égaux.

b) Supposons le corps K parfait de caractéristique $p$ non nulle. Alors l’homomorphisme $\theta_K$ est injectif et le noyau de $\theta$ est $pR_K(A)$. Soit E un A-module semi-simple et de dimension finie sur K. Pour que la forme linéaire Tr$_E$ soit nulle, il faut et il suffit qu’il existe un A-module F tel que E soit isomorphe à $F^p$.

Soit $\mathscr{S}_K$ l’ensemble des classes de A-modules simples qui sont de dimension finie sur K. Les éléments [S], où S parcourt $\mathscr{S}_K$, forment une base du $\mathbf{Z}$-module $R_K$(A), donc les éléments $1\otimes [S]$ forment une base du K-espace vectoriel $K\otimes_{\mathbf{Z}}R_K(A)$ (VIII, p. 191).

Supposons le corps K parfait. D’après la prop. 6 et le cor. de VIII, p. 375 les éléments $\theta ([S]) =\theta_K(1\otimes [S]) =$ Tr$_S$ de $A^*$ sont linéairement indépendants sur K. Il en résulte que l’homomorphisme $\theta_K$ est injectif et que le noyau de l’homomorphisme $\theta$ est composé des éléments $\sum_{S\in\mathscr{S}_K}n_S[S]$ de $R_K(A)$ tels que $n_S\cdot 1_K= 0$ pour tout $S\in \mathscr{S}_K$. Le noyau de $\theta$ est donc égal à $pR_K$(A), où $p$ est la caractéristique de K. En particulier, si K est de caractéristique 0, l’homomorphisme $\theta$ est injectif.

La dernière assertion de a) résulte du cor. de VIII, p. 186.

Plaçons-nous maintenant sous les hypothèses de b), et soit E un A-module semi-simple et de dimension finie sur K. S’il existe un A-module F tel que E soit somme directe de $p$ sous-modules isomorphes à F, le module F est semi-simple et de dimension finie sur K et l’on a Tr$_E=p$ Tr$_F= 0$. Inversement, supposons que Tr$_E= 0$. On a $[E]\in pR_K$(A), donc la multiplicité de tout module simple $S\in \mathscr{S}_K$ dans E est multiple de $p$ (VIII, p. 186, prop. 7) ; on peut l’écrire $p n_S$ avec $n_S\in \mathbf{N}$. La famille $(n_S)$ est à support fini. Posons $F =\oplus_{S\in\mathscr{S}_K}S^{n_S}$. On a alors $[E] = [F^p]$, de sorte que E et $F^p$ sont isomorphes (VIII, p. 186, cor.).

Soit E un A-module de dimension finie sur K. Soit $a\in A$. Notons $\chi_E(a; T)$ le déterminant de l’endomorphisme $1_E+ Ta_E$ du K[T]-module $E[T] = K[T]\otimes_KE$ (III, p. 107). On a la relation

(10) $\chi_E(a; T)\equiv 1 +$ Tr$_E(a)T$ (mod. $T^2K[T])$ (loc. cit., formule (49)). Comme ce polynôme a un terme constant égal à 1, c’est une série formelle inversible (IV, p. 28). De plus, si

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

est une suite exacte de A-modules, tous de dimension finie sur K, on a $\chi_E(a; T) =$ $\chi_{E'}(a; T)\chi_{E''}(a,T)$ (III, p. 101, formule (31)). D’après la définition du groupe de Grothendieck $R_K(A)$ (VIII, p. 189) et sa propriété universelle (VIII, p. 182, prop. 4), il existe un unique homomorphisme $\chi_a$ du groupe $R_K(A)$ dans le groupe multiplicatif 1 + TK[[T]] tel que $\chi_a([E]) =\chi_E(a; T)$ pour tout A-module E de dimension finie sur K. Il résulte de la formule (10) la relation

(11) $\chi_a(x)\equiv 1 +\theta (x)(a)T$ (mod. $T^2K[[T]])$,

tout élément $x\in R_K(A)$ et tout élément $a\in A$.

Si E et $E'$ sont deux A-modules, de dimension finie sur K, ayant des semisimplifiés isomorphes, on a $\chi_E(a; T) =\chi_{E'}(a; T)$.

#### Théorème 2 {#alg-viii-s20-thm-2 .statement tag=00MW}

Soit $\mathscr{A}$ une partie génératrice du K-espace vectoriel A. L’homomorphisme $\chi_{\mathscr{A}}: R_K(A)\rightarrow (1 +$ TK[[T]])$^{\mathscr{A}}$ défini par $\chi_{\mathscr{A}}(x) = (\chi_a(x))_{a\in\mathscr{A}}$ est injectif.

Soit $x$ un élément de $R_K(A)$ tel que $\chi_{\mathscr{A}}(x) = 1$. D’après (11), on a $\theta (x)(a) = 0$ pour tout $a\in \mathscr{A}$, d’où$\theta (x) = 0$ puisque $\theta (x)$ est une forme K-linéaire sur A et que $\mathscr{A}$ engendre le K-espace vectoriel A. Si la caractéristique de K est nulle, cela entraîne $x= 0$ (VIII, p. 376, cor. de la prop. 6), d’où le résultat dans ce cas. Supposons désormais que la caractéristique $p$ de K soit non nulle.

Traitons d’abord le cas où K est algébriquement clos. D’après ce qui précède et loc. cit., on a alors $x\in pR_K(A)$. Soit $y\in R_K(A)$ tel que $x=py$. Pour tout élément $a$ de $\mathscr{A}$, on a $\chi_a(y)^p=\chi_a(py) =\chi_a(x) = 1$. On a donc $(\chi_a(y)-1)^p= 0$, d’où $\chi_a(y) = 1$ puisque l’anneau K[[T]] est intègre. Ainsi, $y$ appartient au noyau de l’endomorphisme $\chi_{\mathscr{A}}$. Il en résulte par récurrence que $x$ appartient à $p^nR_K(A)$ pour tout entier $n\geqslant 1$. Comme $R_K(A)$ est un $\mathbf{Z}$-module libre, cela entraîne $x= 0$, d’où l’injectivité de $\chi_{\mathscr{A}}$ dans ce cas.

Si K n’est plus supposé algébriquement clos, on choisit une clôture algébrique K de K et on considère le diagramme de groupes et d’homomorphismes de groupes

$R_K(A)^{\chi_{\mathscr{A}}}$ // (1 + TK[[T]])$^{\mathscr{A}}$

$$
ui \tag{12}
$$

$R_K(A_{(K)})^{\chi_{\mathscr{A}}}/$/ (1 + TK[[T]])$^{\mathscr{A}}$ où $u$ est l’homomorphisme déduit de l’extension des scalaires de K à K (VIII, p. 190), $i$ l’injection canonique et $\chi_{\mathscr{A}}$ l’homomorphisme $z\rightarrow (\chi_{1\otimes a}(z))_{a\in\mathscr{A}}$. D’après la formule (12) de III, p. 108, le diagramme (12) est commutatif. D’après ce qui précède, l’homomorphisme $\chi_{\mathscr{A}}$ est injectif. Comme $u$ est injectif (VIII, p. 191, th. 1), l’homomorphisme $\chi_{\mathscr{A}}$ est injectif.

#### Corollaire 1 {#alg-viii-s20-thm-2-cor-1 .statement tag=00MX}

Soient E et F des A-modules semi-simples de dimension finie sur K et soit $\mathscr{A}$ une partie génératrice du K-espace vectoriel A. Supposons que pour tout $a\in \mathscr{A}$, les polynômes caractéristiques des endomorphismes $a_E$ et $a_F$ des K-espaces vectoriels E et F soient égaux. Alors les A-modules E et F sont isomorphes.

Soit $a$ un élément de $\mathscr{A}$. Les polynômes caractéristiques de $a_E$ et $a_F$ ont le même degré, donc la dimension de E est égale à celle de F ; notons-la $n$. Soit Pc$_E(a; T)$ le polynôme caractéristique de $a_E$. On a dans K(T) les égalités

$$
()-_n(-1-)-_n(-1)
$$

$\chi_E(a; T) =$ det $1 +a_ET$ = ( T) det $a_E$ = ( T) Pc$_Ea$;

T T

et $\chi_F(a; T)$ est donné par une formule analogue. Vu les hypothèses faites, on a $\chi_E(a; T) =\chi_F(a; T)$. D’après le th. 2, on a [E] = [F] et cela implique que E et F sont isomorphes (VIII, p. 186, cor. de la prop. 7).

#### Corollaire 2 {#alg-viii-s20-thm-2-cor-2 .statement tag=00MY}

Soit A une algèbre centrale, simple et de degré fini sur K. Soit B une K-algèbre semi-simple, soient $f, g$ des homomorphismes d’algèbres de B dans A et soit $\mathscr{B}$ une partie génératrice du K-espace vectoriel B. Les conditions suivantes sont équivalentes :

(i) Il existe un automorphisme intérieur $\theta$ de A tel que $g=\theta \circ f$;

(ii) Pour tout $b\in \mathscr{B}$, on a Pc$_{A/K}(f(b); X) =$ Pc$_{A/K}(g(b); X)$.

Lorsque K est de caractéristique nulle, ces conditions équivalent à la suivante :

(iii) Pour tout $b\in \mathscr{B}$, on a Tr$_{A/K}(f(b)) =$ Tr$_{A/K}(g(b))$.

Notons M et N les B-modules à gauche obtenus en munissant le groupe additif de A des lois d’actions $(b, a)\rightarrow f(b)a$ et $(b, a)\rightarrow g(b)a$ respectivement. D’après la prop. 1 de VIII, p. 253, la propriété (i) équivaut au fait que les B-modules M et N sont isomorphes. Par construction, l’homothétie $b_M$ associée à un élément $b$ de B est la multiplication à gauche par $f(b)$ dans A ; par suite, on a les relations

Pc$_M(b; X) =$ Pc$_{A/K}(f(b); X)$

Tr$_M(b) =$ Tr$_{A/K}(f(b))$

et deux relations analogues où l’on remplace M par N et $f$ par $g$. On sait (VIII, p. 378, cor. 1) que les B-modules M et N sont isomorphes si et seulement si l’on a Pc$_M(b; X) =$ Pc$_N(b; X)$ pour tout $b\in \mathscr{B}$; lorsque le corps K est de caractéristique 0, cette relation équivaut encore à Tr$_M(b) =$ Tr$_N(b)$ pour tout $b\in \mathscr{B}$ (VIII, p. 376, cor. de la prop. 6). L’équivalence des propriétés (i) et (ii), et aussi (i) et (iii) lorsque K est de caractéristique 0, résulte de là.

### 7. Coefficients d’un ensemble de classes de modules

Soit $\mathscr{C}$ un ensemble héréditaire de classes de A-modules (VIII, p. 179, déf. 1). On suppose que tout A-module de type $\mathscr{C}$ est de dimension finie sur K, et l’on note $\Theta_{\mathscr{C}}(A)$ l’ensemble des coefficients des A-modules de type $\mathscr{C}$. D’après la prop. 2 de VIII, p. 370, $\Theta_{\mathscr{C}}(A)$ est également la réunion des images des applications A-linéaires $u: E\rightarrow A^*$, où E parcourt $\mathscr{C}$; c’est aussi la réunion des sous-espaces $\Theta_E(A)$ de $A^*$, où E parcourt $\mathscr{C}($loc. cit.). La famille de sous-(A, A)-bimodules $(\Theta_E(A))_{E\in\mathscr{C}}$ de $A^*$ est filtrante, donc sa réunion $\Theta_{\mathscr{C}}(A)$ est un sous-(A, A)-bimodule de $A^*$.

#### Proposition 7 {#alg-viii-s20-prop-7 .statement tag=00MZ}

Un sous-A-module à gauche de $A^*$, de dimension finie sur K est contenu dans $\Theta_{\mathscr{C}}(A)$si et seulement s’il est de type $\mathscr{C}$.

Soit V un sous-A-module à gauche de $A^*$ de dimension finie sur K. On a vu en VIII, p. 370, remarque 3, qu’on a $V\subset \Theta_V(A)$. Si V est de type $\mathscr{C}$, on a $\Theta_V(A)\subset$ $\Theta_{\mathscr{C}}$(A), donc V est contenu dans $\Theta_{\mathscr{C}}(A)$. Réciproquement, supposons que V soit contenu dans $\Theta_{\mathscr{C}}(A)$. Comme $\Theta_{\mathscr{C}}(A)$ est réunion de la famille filtrante $(\Theta_E(A))_{E\in\mathscr{C}}$ et que V est de dimension finie sur K, il existe un module E de type $\mathscr{C}$ tel que V soit contenu dans $\Theta_E(A)$. Or il existe un entier naturel $n$ tel que $\Theta_E(A)$ soit isomorphe à un quotient de $E^n$ (VIII, p. 370, prop. 2). Comme $\mathscr{C}$ est héréditaire, V est de type $\mathscr{C}$.

#### Corollaire {#alg-viii-s20-n7-cor-1 .statement tag=00N0}

Soit E un A-module de dimension finie sur K. Pour que E soit de type $\mathscr{C}$, il faut et il suffit que $\Theta_E(A)$soit contenu dans $\Theta_{\mathscr{C}}(A)$.

La condition énoncée est évidemment nécessaire.

Réciproquement, supposons que $\Theta_{\mathscr{C}}(A)$ contienne $\Theta_E(A)$. Le A-module $\Theta_E(A)$ est de dimension finie sur K (VIII, p. 370, prop. 2), donc il est de type $\mathscr{C}$, d’après la prop. 7. Or il existe un entier $n\geqslant 0$ tel que E soit isomorphe à un sous-A-module de $\Theta_E(A)^n$ (VIII, p. 370, prop. 2). Comme $\mathscr{C}$ est héréditaire, E est de type $\mathscr{C}$.

### 8. Structure de cogèbre sur le dual restreint

Pour tout $a$ dans A, on note$\eta (a)$ la forme linéaire $f\rightarrow f(a)$ sur Θ(A) ; on définit ainsi une application K-linéaire $\eta$ de A dans le dual $\Theta (A)^*$ de l’espace vectoriel Θ(A). On pose $\varepsilon =\eta (1)$.

#### Proposition 8 {#alg-viii-s20-prop-8 .statement tag=00N1}

Sur l’espace vectoriel Θ(A), il existe une unique structure de cogèbre (III, p. 138) telle que l’application $\eta : A\rightarrow \Theta (A)^*$ soit un homomorphisme de A dans l’algèbre duale (III, p. 143) de Θ(A). La cogèbre Θ(A) est coassociative et admet $\varepsilon$ pour coünité.

Pour tout entier $n\geqslant 1$, considérons l’application K-linéaire $j_n$ de $\Theta (A)^{\otimes n}$ dans le dual de $A^{\otimes n}$ caractérisée par la formule

$$
\langle j_n(f_1\otimes  \cdots  \otimes f_n), a_1\otimes  \cdots  \otimes a_n\rangle =\prod_{i=1}^n\langle f_i, a_i\rangle \tag{13}
$$

pour $(a_i)$ dans $A^n$ et $(f_i)$ dans $\Theta (A)^n$. D’après la prop. 16, (ii) de II, p. 110, l’application $j_n$ est injective. Notons $m_K: K\otimes K\rightarrow K$ et $m_A: A\otimes A\rightarrow A$ les applications déduites de la multiplication de K et A respectivement. Pour $f, g\in \Theta (A)$ et $a, b\in A$, on a

$$
\langle j_2(f\otimes g), a\otimes b\rangle =m_K\circ (\eta (a)\otimes \eta (b))(f\otimes g)
$$

On a donc

$$
\langle j_2(t), a\otimes b\rangle =m_K\circ (\eta (a)\otimes \eta (b))(t) \tag{14}
$$

pour tout $t\in \Theta (A)\otimes \Theta (A)$.

#### Lemme 2 {#alg-viii-s20-lem-2 .statement tag=00RS}

Soit $c: \Theta (A)\rightarrow \Theta (A)\otimes \Theta (A)$une application K-linéaire. Pour que $\eta$ soit un homomorphisme de A dans l’algèbre duale de la cogèbre $(\Theta (A), c)$, il faut et il suffit que le diagramme

Θ(A) $^c$ // $\Theta (A)\otimes \Theta (A)$

$$
j_{_1}j_{_2} \tag{15}
$$

$A^{*^tm_A}$ // $(A\otimes A)^*$

soit commutatif.

En effet, pour que $\eta$ soit un homomorphisme de A dans l’algèbre duale de la cogèbre $(\Theta (A), c)$, il faut et il suffit que l’on ait $\eta (ab) =m_K\circ (\eta (a)\otimes \eta (b))\circ c$ pour tous $a, b\in A$, c’est-à-dire

$$
\eta (ab)(f) =m_K\circ (\eta (a)\otimes \eta (b))(c(f))
$$

pour $a, b\in A$ et $f\in \Theta (A)$. Or on a

$$
\eta (ab)(f) =f(ab) =\langle^tm_A(j_1(f)), a\otimes b\rangle
$$

et, d’après (14)

$$
m_K\circ (\eta (a)\otimes \eta (b))(c(f)) =\langle j_2(c(f)), a\otimes b\rangle
$$

pour tous $a, b\in A$ et tout $f\in \Theta (A)$, d’où le lemme.

Comme $j_2$ est injective, il existe au plus une application linéaire $c$ rendant commutatif le diagramme précédent. Pour en prouver l’existence, il s’agit de démontrer que l’image de $^tm\circ j_1$ est contenue dans celle de $j_2$; autrement dit, il s’agit de prouver qu’il existe, pour tout élément $f$ de Θ(A), un entier naturel $n$ et des éléments $f_1', . . . , f_n', f_1'', . . . , f_n''$ de Θ(A) satisfaisant aux relations

$$
f(ab) =\sum_{i=1}^nf_i'(a)f_i''(b) \tag{16}
$$

pour $a, b\in A$. On aura alors

$$
c(f) =\sum_{i=1}^nf_i'\otimes f_i'' \tag{17}
$$

D’après le cor. de VIII, p. 371, il existe un A-module à gauche E, de dimension finie sur K, dont $f$ est un coefficient. Soient $(e_1, . . . , e_n)$ une base de $E, (e^*_1, . . . , e^*_n)$ la base duale, $x$ un élément de E et $x^*$ un élément de $E^*$ tels que $f=c_E(x, x^*)$. Posons $f_i'=c_E(e_i, x^*)$ et $f_i''=c_E(x, e^*_i)$ pour $i\in [1, n]$; pour $a, b$ dans A, on a

$$
f(ab) =\langle x^*, abx\rangle =\langle x^*a, bx\rangle
$$

$$
=\sum_i\langle x^*a, e_i\rangle \langle e^*_i, bx\rangle =\sum_i\langle x^*, ae_i\rangle \langle e^*_i, bx\rangle =\sum_if_i'(a)f_i''(b)
$$

d’où (16).

Prouvons la coassociativité de $c$. Pour cela, considérons les applications K-linéaires

$c'=(c\otimes 1_{\Theta (A)})\circ c$ et $c''=(1_{\Theta (A)}\otimes c)\circ c$

de Θ(A) dans $\Theta (A)^{\otimes 3}$. On a les relations

$$
\langle j_3(f\otimes c(g)), a\otimes b\otimes c\rangle =\langle f, a\rangle \langle j_2\circ c(g), b\otimes c\rangle
$$

$$
=\langle f, a\rangle \langle g, bc\rangle
$$

$$
=\langle j_2(f\otimes g), a\otimes bc\rangle
$$

$=\langle^t$(Id$_A\otimes m_A)\circ j_2(f\otimes g), a\otimes b\otimes c\rangle$, pour $f, g\in \Theta (A)$ et $a, b, c\in A$. On en déduit la commutativité du diagramme suivant :

$\Theta (A)\otimes \Theta (A)^{Id_{\Theta (A)}\otimes c}/$/ $\Theta (A)\otimes \Theta (A)\otimes \Theta (A)$

(18)

$j_2j_3$

$(A\otimes A)^{*^t(Id_A\otimes m_A)}$ // $(A\otimes A\otimes A)^*$

Compte tenu de la commutativité de ce diagramme et de celle du diagramme (15) de VIII, p. 380, pour $f\in \Theta (A)$, et $a,a',a''\in A$, on a

$$
\langle j_3\circ c'(f), a\otimes a'\otimes a''\rangle =\langle f,(aa')a''\rangle
$$

on montre de même la relation

$$
\langle j_3\circ c''(f), a\otimes a'\otimes a''\rangle =\langle f, a(a'a'')\rangle
$$

Comme la multiplication dans A est associative, on a $j_3\circ c'=j_3\circ c''$, d’où $c'=c''$ puisque $j_3$ est injective.

Enfin, les formules (16) et (17) entraînent que Θ(A) admet $\varepsilon$ comme coünité.

#### Remarque 1 {#alg-viii-s20-n8-rem-1 .statement tag=00N2}

Soit $(V, \pi )$ une représentation linéaire de dimension finie de l’algèbre A. Introduisons une base $(e_1, . . . , e_n)$ de V et la base duale $(e^*_1, . . . , e^*_n)$ de $V^*$. D’après la démonstration précédente, on a la relation

$$
c(c_{\pi}(x, x^*)) =\sum_{k=1}^nc_{\pi}(e_k, x^*)\otimes c_{\pi}(x, e^*_k) \tag{19}
$$

pour $x\in V$ et $x^*\in V^*$. En particulier, posons $\pi_{ij}=c_{\pi}(e_j, e^*_i)$, de sorte que pour tout $a\in A$, la matrice de $\pi (a)$ par rapport à la base $(e_1, . . . , e_n)$ de V est égale à $(\pi_{ij}(a))$. On a alors, pour $1\leqslant i\leqslant n$ et $1\leqslant j\leqslant n$,

$$
c(\pi_{ij}) =\sum_{k=1}^n\pi_{ik}\otimes \pi_{kj} \tag{20}
$$

#### Définition 3 {#alg-viii-s20-def-3 .statement tag=00N3}

Soient C une cogèbre sur le corps K et $c$ son coproduit. On appelle sous-cogèbre de C tout sous-espace vectoriel $C_1$ de C tel que $c(C_1)$soit contenu dans l’image canonique de $C_1\otimes_KC_1$ dans $C\otimes_KC$.

Soit $j$ l’injection canonique de $C_1$ dans C. D’après cette définition, il existe une unique application linéaire $c_1: C_1\rightarrow C_1\otimes_KC_1$ telle que l’on ait

$$
c\circ j= (j\otimes j)\circ c_1 \tag{21}
$$

cette relation signifie que $j$ est un morphisme de cogèbres de $(C_1, c_1)$ dans $(C, c)$ (III, p. 138).

Si C est coassociative, alors $C_1$ est coassociative. Si C est cocommutative, alors il en est de même de $C_1$. Si C a une coünité $\varepsilon$, alors la restriction de $\varepsilon$ à $C_1$ est une coünité de $C_1$.

#### Proposition 9 {#alg-viii-s20-prop-9 .statement tag=00N4}

Soit Θ un sous-espace vectoriel de Θ(A). Les conditions suivantes sont équivalentes :

(i) Θ est un sous-$(A,A)$-bimodule de Θ(A) ;

(ii) Θ est une sous-cogèbre de Θ(A) ;

(iii) il existe un ensemble héréditaire $\mathscr{C}$ de classes de A-modules de dimension finie sur K tel que $\Theta  = \Theta_{\mathscr{C}}(A)$.

Lorsque ces conditions sont satisfaites, l’ensemble $\mathscr{C}$ mentionné en (iii) est uniquement déterminé.

La dernière assertion résulte du cor. de VIII, p. 379 : l’ensemble $\mathscr{C}$ se compose des classes des A-modules E de dimension finie sur K tels que $\Theta_E(A)$ soit contenu dans Θ.

(iii) $=\Rightarrow$ (ii) : Soit $\mathscr{C}$ un ensemble héréditaire de classes de A-modules de dimension finie sur K. Alors $\Theta_{\mathscr{C}}(A)$ est la réunion de la famille filtrante $(\Theta_E(A))_{E\in\mathscr{C}}$. Comme $\Theta_E(A)$ est une sous-cogèbre de Θ(A) pour tout $E\in \mathscr{C}$ (VIII, p. 382, formule (19)), il en est de même de $\Theta_{\mathscr{C}}(A)$.

(ii) $=\Rightarrow$ (i) : Soit $f\in \Theta (A)$. Soient $f_1', . . . , f_n', f_1'', . . . , f_n''$ des éléments de Θ(A) satisfaisant à $c(f) =\sum f_i'\otimes f_i''$. Pour $a,b$ dans A, on a $f(ab) =\sum f_i'(a)f_i''(b)$, d’où

$$
bf=\sum_{i=1}^nf_i''(b)f_i',f a=\sum_{i=1}^nf_i'(a)f_i''
$$

(VIII, p. 367, formules (3) et (4)). Par suite, une sous-cogèbre de Θ(A) en est un sous-(A, A)-bimodule.

(i) $=\Rightarrow$ (iii) : Supposons que Θ soit un sous-(A, A)-bimodule de Θ(A) ; soit $\mathscr{C}$ l’ensemble des classes des A-modules E de dimension finie sur K tels que $\Theta_E(A)$ soit contenu dans Θ. L’ensemble $\mathscr{C}$ est héréditaire (VIII, p. 369, remarque 2) et l’on a $\Theta_{\mathscr{C}}(A)\subset \Theta$ par construction. Soient $f\in \Theta$ et $E = Af$. Alors E est de dimension finie sur K. Par suite, toute forme linéaire sur E est de la forme $u_a:g\rightarrow g(a)$ avec $a$ dans A (II, p. 105, cor. 2). Or, pour $a, b, x\in A$, on a

$$
c_E(af, u_b)(x) =\langle u_b, xaf\rangle =f(bxa) =af b(x)
$$

d’où $c_E(af, u_b) =af b$. On a donc $\Theta_E(A)\subset \Theta$. Par suite, le A-module E est de type $\mathscr{C}$ et $f$ est l’un de ses coefficients. On a donc $\Theta \subset \Theta_{\mathscr{C}}(A)$ et finalement $\Theta  = \Theta_{\mathscr{C}}(A)$.

#### Remarque 2 {#alg-viii-s20-n8-rem-2 .statement tag=00N5}

Soit Θ une sous-cogèbre de Θ(A). Munissons K de la topologie discrète et l’algèbre A de la topologie la moins fine rendant continues les applications $f: A\rightarrow K$ pour $f$ parcourant Θ (TG I, p. 12). Cette topologie munit A d’une structure de K-module topologique. Un idéal bilatère de $\mathfrak{a}$ de A est ouvert si et seulement s’il est de codimension finie et que son orthogonal $\mathfrak{a}'$ est contenu dans Θ. D’après la prop. 3 de VIII, p. 371, les idéaux bilatères ouverts de A forment un système fondamental de voisinage de 0 dans A. La topologie de A est donc compatible avec sa structure d’anneau.

Soit $\mathscr{C}$ l’ensemble héréditaire de classes de A-modules de dimension finie sur K tel que $\Theta  = \Theta_{\mathscr{C}}$ (VIII, p. 383, prop. 9). Soit E un A-module à gauche, de dimension finie sur K. Munissons-le de la topologie discrète. Les conditions suivantes sont équivalentes :

(i) Le A-module E est de type $\mathscr{C}$;

(ii) L’annulateur du A-module E est ouvert dans A ;

(iii) L’application $(a, x)\rightarrow ax$ de $A\times E$ dans E est continue.

Cette dernière propriété signifie que E est un A-module topologique.

Soit $\Theta^*$ l’algèbre duale de la cogèbre Θ. On munit $\Theta^*$ de la topologie la moins fine rendant continues les applications $\varphi \rightarrow \varphi (u)$ de $\Theta^*$ dans K, pour $u$ parcourant Θ. La topologie sur l’algèbre $\Theta^*$ est compatible avec la structure de groupe additif de $\Theta^*$. Un système fondamental de voisinage de 0 est formé par les orthogonaux dans $\Theta^*$ des ensembles de la forme $\Theta_E(A)$ où E est un A-module de type $\mathscr{C}$. Or un tel ensemble est une sous-cogèbre de Θ, donc son orthogonal est un idéal de $\Theta^*$. La topologie de $\Theta^*$ est donc compatible avec sa structure d’anneau. L’homomorphisme canonique d’algèbres $\eta : A\rightarrow \Theta^*$ (qui à $a\in A$ associe la forme linéaire $f\rightarrow f(a)$ sur Θ) définit un isomorphisme de l’espace séparé complété $\widehat{A}$ de A (TG II, p. 23) sur $\Theta^*$.

## EXERCICES {#alg-viii-s20-exercises}

See the [exercises for § 20](exercises/s20/).
