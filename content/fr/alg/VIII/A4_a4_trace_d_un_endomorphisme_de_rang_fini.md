---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 4
section_title: Trace d’un endomorphisme de rang fini
appendix: true
lang: fr
source: alg-viii-fr
book_pages: A VIII.453-A VIII.457
pdf_pages: 0454-0458
extraction: native
subsections:
    - "no": 1
      title: Applications linéaires de rang fini
      page: 453
      pdf_page: 454
    - "no": 2
      title: Trace d’un endomorphisme de rang fini
      page: 454
      pdf_page: 455
statements: 5
exercises: 2
content_sha256: 61723c841f5b4b121b1f809e79591cd5a8f85f6783252c80270eac319d22bc45
---

### APPENDICE 4 TRACE D’UN ENDOMORPHISME DE RANG FINI

### 1. Applications linéaires de rang fini

Soit A un anneau et soient E et F des A-modules. On note Hom$^f_A(E,F)$ l’ensemble des applications linéaires de E dans F dont l’image est contenue dans un sous-module de type fini de F. C’est un sous-groupe de Hom$_A(E,F)$. Lorsque A est un corps, c’est l’ensemble des applications linéaires de rang fini de E dans F (II, p. 101, déf. 3). On pose End$^f_A(E) =$ Hom$^f_A(E,E)$.

Soient $E,F,G$ des A-modules et soient $u: E\rightarrow F$ et $v: F\rightarrow G$ des applications A-linéaires. Si $u\in$ Hom$^f_A(E,F)$ ou $v\in$ Hom$^f_A(F,G)$, alors $v\circ u$ appartient à Hom$^f_A(E,G)$.

Notons $\theta$ l’homomorphisme de groupes canonique de $E^*\otimes_AF$ dans Hom$_A(E,F)$ (A, II, p. 77) ; il associe à un élément $x^*\otimes y$ de $E^*\otimes_AF$ l’application $x\rightarrow  \langle x, x^*\rangle y$ de E dans F.

#### Lemme 1 {#alg-viii-a4-lem-1 .statement tag=00QO}

Supposons que le A-module F soit projectif. L’homomorphisme de groupes $\theta$ est injectif et son image est Hom$^f_A(E,F)$.

D’après loc. cit., cor., l’homomorphisme $\theta$ est injectif. Son image est contenue dans Hom$^f_A(E,F)$. Soit $u\in$ Hom$^f_A(E,F)$; prouvons que $u$ appartient à l’image de $\theta$.

Supposons d’abord le A-module F libre. Soit $(f_i)_{i\in I}$ une base de F et soit $(f_i^*)_{i\in I}$ la base de $F^*$ duale de $(f_i)_{i\in I}$. Soit J une partie finie de I telle que l’image de $u$ soit contenue dans le sous-module de F engendré par les $f_j$ pour $j\in J$; on a

$$
u(x) =\sum_{j\in J}\langle u(x), f_j^*\rangle f_j=\sum_{j\in J}\langle x,^tu(f_j^*)\rangle f_j \tag{1}
$$

pour tout $x\in E$, d’où

$$
u=\theta (\sum_{j\in J}^tu(f_j^*)\otimes f_j) \tag{2}
$$

Dans le cas général, il existe un A-module libre L et des homomorphismes $i: F\rightarrow L$ et $p: L\rightarrow F$ tels que $p\circ i= 1_F$. L’homomorphisme $i\circ u$ appartient à Hom$^f_A(E,L)$. D’après ce qui précède, il existe un ensemble fini J et, pour tout $j\in J$, des éléments $x^*_j$ de $E^*$ et $y_j$ de L tels qu’on ait

$$
i(u(x)) =\sum_{j\in J}\langle x, x^*_j\rangle y_j
$$

pour tout $x\in E$. On a alors

$$
u(x) =p(i(u(x))) =\sum_{j\in J}\langle x, x^*_j\rangle p(y_j)
$$

pour tout $x\in E$, d’où $u=\theta (\sum_{j\in J}x^*_j\otimes p(y_j))$.

### 2. Trace d’un endomorphisme de rang fini

Dans ce numéro, A désigne un anneau commutatif. Soit E un A-module projectif. Alors End$^f_A(E)$ est un sous-A-module de End$_A(E)$ et l’application canonique $E^*\otimes_AE\rightarrow$ End$_A(E)$ définit un isomorphisme $\theta_E$ de A-modules de $E^*\otimes_AE$ sur End$^f_A(E)$ (lemme 1). Considérons la forme linéaire canonique $\tau : E^*\otimes_AE\rightarrow A$ (A, II, p. 78), caractérisée par la formule $\tau (x^*\otimes x) =\langle x, x^*\rangle$. Par composition avec l’isomorphisme $\theta^{-1}_E$, on en déduit une forme linéaire Tr : End$^f_A(E)\rightarrow A$, dite forme trace. Lorsque le A-module E est de type fini, on retrouve la définition de A, II, p. 78.

#### Proposition 1 {#alg-viii-a4-prop-1 .statement tag=00QP}

Soit E un A-module libre. Soit $(e_i)_{i\in I}$ une base de E et soit $(e^*_i)_{i\in I}$ sa base duale. Soit $u\in$ End$^f_A(E)$. La famille $(\langle u(e_i), e^*_i\rangle )_{i\in I}$ est à support fini et sa somme est égale à Tr( $u)$.

Il suffit de traiter le cas où $u$ est de la forme $\theta_E(x^*\otimes x)$ avec $x\in E$ et $x^*\in E^*$. La famille $(\langle x, e^*_i\rangle )_{i\in I}$ est alors à support fini et l’on a $x=\sum_{i\in I}\langle x, e^*_i\rangle e_i$. Par suite, la famille $(\langle x, e^*_i\rangle \langle e_i, x^*\rangle )_{i\in I}$ est aussi à support fini et l’on a $\langle x, x^*\rangle =\sum_{i\in I}\langle x, e^*_i\rangle \langle e_i, x^*\rangle$. Or on a $\langle u(e_i), e^*_i\rangle =\langle x, e^*_i\rangle \langle e_i, x^*\rangle$ pour tout $i\in I$. Cela démontre la proposition.

#### Proposition 2 {#alg-viii-a4-prop-2 .statement tag=00QQ}

Soient $E,F$des A-modules projectifs. Soient $u\in$ Hom$^f_A(E,F)$ et $v\in$ Hom$_A(F,E)$. On a la relation

(3) Tr($v\circ u$) $=$ Tr($u\circ v$).

Il suffit de démontrer la proposition lorsque $u$ est de la forme $\theta (x^*\otimes y)$, avec $x^*\in E^*$ et $y\in F$; or on a dans ce cas

$v\circ u=\theta_E(x^*\otimes v(y))$ et $u\circ v=\theta_F(^tv(x^*)\otimes y)$, d’où

Tr($v\circ u$) $=\langle v(y), x^*\rangle =\langle y,^tv(x^*)\rangle =$ Tr($u\circ v$).

#### Corollaire {#alg-viii-a4-n2-cor-1 .statement tag=00QR}

Soit E un A-module projectif, soit $u$ un élément de End$^f_A(E)$et soit F un sous-A-module projectif de E contenant Im $u$;notons $u_F$ l’endomorphisme de F induit par $u$. On a

(4) Tr($u$) $=$ Tr($u_F$).

Notons $i$ l’injection canonique de F dans E, et $v: E\rightarrow F$ l’homomorphisme déduit de $u$. On a $u_F=v\circ i$ et $u=i\circ v$, d’où le corollaire.

Soient E un A-module projectif et $u\in$ End$^f_A(E)$. Pour tout entier naturel $p$, le

A-module $\wedge^pE$ est projectif (III, p. 87, cor. 2), l’endomorphisme $\wedge^pu$ appartient à End$^f_A(\wedge^pE)$ (III, p. 80, prop. 6) et il est nul dès que $p$ est assez grand. L’en-

semble $1_E+$ End$^f_A(E)$ est stable par composition. On définit une application det de $1_E+$ End$^f_A(E)$ dans A en posant

det(1$_E+u) =\sum_{p\geqslant 0}$ Tr$\wedge^pu$,

pour tout $u\in$ End$^f_A(E)$.

Si E est libre de dimension finie, cette définition est cohérente avec celle de III, p. 90, en vertu du cor. de III, p. 97.

#### Proposition 3 {#alg-viii-a4-prop-3 .statement tag=00QS}

Soit E un A-module projectif.

a) Soit $u\in$ End$^f_A(E)$. Soit F un sous-A-module projectif de E, contenant Im $u$, et soit $u_F$ l’endomorphisme de F induit par $u$. On a

(5) det(1$_E+u) =$ det(1$_F+u_F)$.

b) Soient $u, v$ deux éléments de End$^f_A(E)$. On a

(6) det$((1_E+u)\circ (1_E+v))=$ det(1$_E+u)$ det(1$_E+v)$.

Prouvons a). Pour tout entier $p\geqslant 0$, le A-module projectif $\wedge^pF$ s’identifie à un sous-module de $\wedge^pE$ (III, p. 88, cor.). L’image de $\wedge^pu$ est contenue dans $\wedge^pF$, et l’endomorphisme de $\wedge^pF$ induit par $\wedge^pu$ est égal à $\wedge^pu_F$. On a donc Tr($\wedge^pu$) $=$ Tr($\wedge^pu_F$) en vertu du cor. de la prop. 2, d’où a).

Prouvons b). Soit G un A-module tel que le A-module $L = E\oplus G$ soit libre. Notons $u', v'$ les endomorphismes $u\oplus 0_G$ et $v\oplus 0_G$ de L. D’après a), on a les relations det(1$_L+u') =$ det(1$_E+u)$, det(1$_L+v') =$ det(1$_E+v)$ et

det(1$_L+u'+v'+u'\circ v') =$ det(1$_E+u+v+u\circ v)$; il suffit donc de prouver l’assertion b) lorsque le A-module E est libre. Il existe alors un sous-module libre de type fini F de E qui contient l’image de $u$ et celle de $v$. Posons $w=u+v+u\circ v$. L’image de $w$ est contenue dans F et l’on a $w_F=u_F+v_F+u_F\circ v_F$. On a donc, d’après (5), on a det(1$_E+u) =$ det(1$_F+u_F)$, det(1$_E+v) =$ det(1$_F+v_F)$

et $()$

det $(1_E+u)\circ (1_E+v)$ = det(1$_E+w) =$ det(1$_F+w_F) =$ det((1$_F+u_F)\circ (1_F+v_F))$. Comme F est un A-module libre de type fini, on a

det((1$_F+u_F)\circ (1_F+v_F)) =$ det(1$_F+u_F)$ det(1$_F+v_F) =$ det(1$_E+u)$ det(1$_E+v)$.

## EXERCICES {#alg-viii-a4-exercises}

See the [exercises for Appendix 4](exercises/a4/).
