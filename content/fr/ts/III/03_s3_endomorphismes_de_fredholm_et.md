---
book: ts
book_title: Théories spectrales
chapter: III
chapter_title: APPLICATIONS LINÉAIRES COMPACTES ET PERTURBATIONS
section: 3
section_title: Endomorphismes de Fredholm et endomorphismes de Riesz
lang: fr
source: ts-iii-v-fr
book_pages: A III.39-A III.55, A III.120-A III.122
pdf_pages: 0053-0069, 0134-0136
extraction: native
subsections:
    - "no": 1
      title: Morphismes stricts et applications linéaires de rang fini
      page: 39
      pdf_page: 53
    - "no": 2
      title: Applications de Fredholm
      page: 40
      pdf_page: 54
    - "no": 3
      title: Indice d’une application de Fredholm
      page: 43
      pdf_page: 57
    - "no": 4
      title: Endomorphismes de Riesz
      page: 45
      pdf_page: 59
    - "no": 5
      title: Applications de Fredholm et applications de Riesz entre espaces de Fréchet
      page: 52
      pdf_page: 66
    - "no": 6
      title: Caractérisation spectrale des endomorphismes de Riesz
      page: 53
      pdf_page: 67
statements: 31
exercises: 8
content_sha256: da78f50f34ac477662f0f04ab1566e3cf22beac9e03267e8963f646d15b9c528
---

## § 3. ENDOMORPHISMES DE FREDHOLM ET ENDOMORPHISMES DE RIESZ

### 1. Morphismes stricts et applications linéaires de rang fini

#### Proposition 1 {#ts-iii-s3-prop-1 .statement tag=02RE}

Soient E et F des espaces localement convexes, $E_1$ un sous-espace fermé de codimension finie de E et $u$ une application linéaire continue de E dans F. Pour que $u$ soit un morphisme strict d’image fermée, il faut et il suffit que $u|E_1$ en soit un.

Supposons d’abord que l’application linéaire $u|E_1$ est injective. On a alors $E_1\cap$ Ker($u$) $=\{0\}$, si bien que Ker($u$) est de dimension finie. Soit S un sous-espace vectoriel de E supplémentaire de $E_1+$ Ker($u$). L’espace E est somme directe topologique de $E_1$, Ker($u$) et S (EVT, I, p. 15, cor. 4 et prop. 3). Si $u$ est un morphisme strict d’image fermée, il définit par restriction un isomorphisme de $E_1\oplus S$ sur un sous-espace vectoriel fermé de F, et a fortiori un isomorphisme de $E_1$ sur un sous-espace vectoriel fermé de F. Inversement, supposons que $u$ définisse par restriction un isomorphisme de $E_1$ sur $u(E_1)$ et que $u(E_1)$ soit fermé dans F. On a $u(E) =u(E_1)\oplus u(S)$. Il en résulte que $u(E)$ est somme directe topologique de $u(E_1)$ et $u$(S), et est fermé dans F (loc. cit.). Puisque $u(E_1)$ est fermé et que l’on a $u(E_1)\cap u(S) =\{0\}$, l’espace $u(S)$ est séparé et $u$ définit par restriction un isomorphisme de S sur $u(S)$ (EVT, I, p. 15, cor. de la prop. 3), donc aussi de $E_1\oplus S$ sur $u(E)$. Cela prouve que $u$ est un morphisme strict d’image fermée.

Passons au cas général. Posons $N = E_1\cap$ Ker($u$) et $G = E/N$. L’espace localement convexe $E_1/N$ s’identifie à un sous-espace vectoriel fermé de codimension finie $G_1$ de G. Notons $v: G\rightarrow F$ l’application linéaire continue déduite de $u$ par passage au quotient. Pour que $u$ (resp. $u|E_1)$ soit un morphisme strict d’image fermée, il faut et il suffit que $v$ (resp. $v|G_1)$ en soit un. Cela nous ramène au cas déjà traité.

#### Corollaire 1 {#ts-iii-s3-prop-1-cor-1 .statement tag=02RF}

Supposons F séparé. Soit $v\in \mathscr{L}^f(E; F)$. Si $u$ est un morphisme strict d’image fermée de E dans F, alors il en est de même de $u+v$.

Comme F est séparé, le noyau de $v$ est un sous-espace vectoriel fermé de E ; il est de codimension finie dans E et $u+v$ a même restriction que $u$ à Ker($v$). Le corollaire découle ainsi de la proposition.

#### Corollaire 2 {#ts-iii-s3-prop-1-cor-2 .statement tag=02RG}

Soit T un sous-espace vectoriel séparé de dimension finie de F. Notons $\pi : F\rightarrow F/T$ la surjection canonique. Pour que $u$ soit un morphisme strict d’image fermée, il faut et il suffit que $\pi \circ u$ en soit un.

L’application identique de T sur lui-même se prolonge en une application continue $q: F\rightarrow T$ (EVT, II, p. 26, remarque). Le noyau S de $q$ est un supplémentaire topologique fermé de T. Soit $p: F\rightarrow F$ le projecteur d’image S associé à la décomposition $F = T\oplus S$. Pour que $\pi \circ u$ soit un morphisme strict d’image fermée, il faut et il suffit que $p\circ u$ en soit un. Or $p\circ u$ et $u$ ont même restriction à $^-u^1$(S), qui est un sous-espace vectoriel fermé de codimension finie de E, et l’assertion résulte de la proposition.

### 2. Applications de Fredholm

Soient E et F des espaces localement convexes. Dans ce numéro, on note $u\equiv v$ la congruence modulo $\mathscr{L}^f(E; F)$ des éléments $u$ et $v$ de $\mathscr{L}(E; F)$.

Si G est un espace localement convexe, et si $u'$ et $v'$ sont des éléments de $\mathscr{L}(F; G)$, les relations $u\equiv v$ et $u'\equiv v'$ entraînent la relation $u'\circ u\equiv v'\circ v$.

On dit qu’un élément $w$ de $\mathscr{L}(F; E)$ est un quasi-inverse de l’élément $u$ de $\mathscr{L}(E; F)$ si l’on a $w\circ u\equiv 1_E$ et $u\circ w\equiv 1_F$.

Supposons que $w$ soit un quasi-inverse de $u$. Si $u_1$ est un élément de $\mathscr{L}(E; F)$ et $w_1$ est un élément de $\mathscr{L}(F; E)$ tels que $u_1\equiv u$ et $w_1\equiv w$, alors $w_1$ est un quasi-inverse de $u_1$ puisque $w\circ u\equiv w_1\circ u_1$ et $u\circ w\equiv u_1\circ w_1$.

Si $w$ et $w_1$ sont des quasi-inverses de $u$, alors $w_1\equiv w$ puisque

$$
w_1= 1_E\circ w_1\equiv w\circ u\circ w_1\equiv w\circ 1_F=w
$$

#### Définition 1 {#ts-iii-s3-def-1 .statement tag=02RH}

Soient E et F des espaces localement convexes. On dit qu’un élément $u$ de $\mathscr{L}(E; F)$ est une application de Fredholm[^1] s’il possède un quasi-inverse. Une application de Fredholm de E dans E s’appelle un endomorphisme de Fredholm de E.

On notera $\mathscr{F}(E; F)$ l’ensemble des applications de Fredholm de E dans F, et $\mathscr{F}(E)$ l’ensemble des endomorphismes de Fredholm de E.

#### Remarque {#ts-iii-s3-n2-rem-1 .statement tag=02RI}

Soient E, F et G des espaces localement convexes, $u: E\rightarrow F$ et $v: F\rightarrow G$ des applications linéaires continues.

1) Supposons que $u$ soit une application de Fredholm et notons $u_1$ un quasi-inverse de $u$. Comme $u$ est un quasi-inverse de $u_1$, l’application $u_1$ est une application de Fredholm.

2) Supposons que $u$ et $v$ soient des applications de Fredholm, et soit $u_1$ (resp. $v_1)$ un quasi-inverse de $u$ (resp. $v)$. Alors $v\circ u$ est une application de Fredholm de E dans G et $u_1\circ v_1$ est un quasi-inverse de $v\circ u$. En effet, on calcule

$$
(u_1\circ v_1)\circ (v\circ u) =u_1\circ (v_1\circ v)\circ u\equiv u_1\circ 1_F\circ u=u_1\circ u\equiv 1_E
$$

$$
(v\circ u)\circ (u_1\circ v_1) =v\circ (u\circ u_1)\circ v_1\equiv v\circ 1_F\circ v_1=v\circ v_1\equiv 1_G
$$

3) Supposons que $u$ et $v\circ u$ soient des applications de Fredholm, et soit $w_1$ un quasi-inverse de $v\circ u$. Alors $v$ est une application de Fredholm et $u\circ w_1$ est un quasi-inverse de $v$.

En effet, $w_1$ est une application de Fredholm d’après la première remarque. Soit $u_1$ un quasi-inverse de $u$; d’après la seconde remarque, $u\circ w_1$ est une application de Fredholm et $(v\circ u)\circ u_1$ en est un quasi-inverse. On a $u\circ u_1\equiv 1_F$, d’où $v\circ u\circ u_1\equiv v$; ceci prouve l’assertion.

4) Supposons que $v$ et $v\circ u$ soient des applications de Fredholm, et soit $w_1$ un quasi-inverse de $v\circ u$. Alors $u$ est une application de Fredholm et $w_1\circ v$ est un quasi-inverse de $u$.

La démonstration est analogue à celle de la remarque précédente.

#### Lemme 1 {#ts-iii-s3-lem-1 .statement tag=02RJ}

Soient E et F des espaces localement convexes et $u$ une application de Fredholm de E dans F. Le noyau et le conoyau de $u$ sont de dimension finie.

Soit $v: F\rightarrow E$ un quasi-inverse de $u$. Le noyau de $u$ est contenu dans l’image de l’application linéaire de rang fini $1_E-v\circ u$, donc est de dimension finie. L’image de $u$ contient le noyau de l’application linéaire de rang fini $1_F-u\circ v$, donc est de codimension finie dans F.

#### Proposition 2 {#ts-iii-s3-prop-2 .statement tag=02RK}

Soient E et F des espaces localement convexes séparés et $u$ un élément de $\mathscr{L}(E; F)$. Les propriétés suivantes sont équivalentes :

(i) L’application $u$ est une application de Fredholm;

(ii) L’application $u$ est un morphisme strict, son noyau est de dimension finie, son image est fermée et de codimension finie dans F ;

(iii) Il existe des sous-espaces vectoriels fermés de codimension finie $E_1$ de E et $F_1$ de F tels que $u$ définisse par passage aux sous-espaces un isomorphisme de $E_1$ sur $F_1$;

(iv) Il existe des décompositions en somme directe topologique $E = E_1\oplus E_2$ et $F = F_1\oplus F_2$ telles que $E_2$ et $F_2$ soient de dimension finie, que $u$ s’annule sur $E_2$ et définisse par passage aux sous-espaces un isomorphisme de $E_1$ sur $F_1$.

(i) $=\Rightarrow$ (iii) : Soient $v$ un quasi-inverse de $u, E_1$ le noyau de $1_E-v\circ u$ et $F_1$ celui de $1_F-u\circ v$. Comme les applications linéaires $1_E-v\circ u$ et $1_F-u\circ v$ sont continues et de rang fini, $E_1$ et $F_1$ sont des sous-espaces vectoriels fermés de codimension finie de E et F respectivement. Soit $x\in E_1$. On a

$$
(1_F-u\circ v)(u(x)) =u((1_E-v\circ u)(x)) =u(0) = 0
$$

d’où $u(x)\in F_1$. On a donc $u(E_1)\subset F_1$; on a de même $v(F_1)\subset E_1$. Les applications linéaires continues $u_1: E_1\rightarrow F_1$ et $v_1: F_1\rightarrow E_1$ déduites de $u$ et $v$ sont alors des isomorphismes réciproques l’un de l’autre, puisque $v\circ u$ et $1_E$ (resp. $u\circ v$ et $1_F)$ coïncident sur $E_1$ (resp. sur $F_1)$.

(iii) $=\Rightarrow$ (ii) : Soient $E_1$ et $F_1$ vérifiant l’hypothèse de (iii). On a $E_1\cap$ Ker($u$) $=\{0\}$ et $F_1\subset$ Im($u$), donc Ker($u$) est de dimension finie et Im($u$) est fermé et de codimension finie dans F. Il résulte de la prop. 1 de III, p. 39 que l’application $u$ est un morphisme strict.

(ii) $=\Rightarrow$ (iv) : Supposons la condition (ii) satisfaite. Le sous-espace vectoriel fermé $E_2=$ Ker($u$) de E est de dimension finie, et il existe un sous-espace vectoriel $E_1$ de E supplémentaire topologique de $E_2$ (EVT, II, p. 27, cor. 2). Le sous-espace vectoriel $F_1=$ Im($u$) de F est fermé et de codimension finie, et il admet un supplémentaire topologique $F_2$ dans F. D’après la prop. 1 de III, p. 39, l’application $u|E_1$ est un morphisme strict, donc $u$ induit un isomorphisme de $E_1$ sur $F_1$.

(iv) $=\Rightarrow$ (i) : Sous les hypothèses de (iv), l’application linéaire de F dans E qui coïncide avec $u^{-1}_1$ sur $F_1$ et est nulle sur $F_2$ est un quasi-inverse de $u$.

#### Remarque 5 {#ts-iii-s3-n2-rem-5 .statement tag=02RL}

Soient E, F des espaces localement convexes séparés et $u: E\rightarrow F$ une application de Fredholm. Si $u$ est bijectif, alors $u$ est un isomorphisme (en effet, $u$ est un morphisme strict d’après la prop. 2, (ii)).

### 3. Indice d’une application de Fredholm

Soient E, F et G des espaces localement convexes.

Soit $u: E\rightarrow F$ une application de Fredholm. Les espaces vectoriels Ker($u$) et Coker($u$) sont de dimension finie (lemme 1 de III, p. 41). Rappelons que le nombre entier

(1) dim Coker($u$)$-$ dim Ker($u$) $=$ codim$_F$ Im($u$)$-$ dim Ker($u$)

s’appelle l’indice de $u$ et est noté ind($u$) (A, V, p. 126).

Si $u: E\rightarrow F$ et $v: F\rightarrow G$ sont des applications de Fredholm, il en est de même de $v\circ u($III, p. 41, remarque 2), et l’on a (A, V, p. 127, lemme 2)

(2) ind($v\circ u$) $=$ ind($v$) $+$ ind($u$).

Supposons E et F séparés et soit $u: E\rightarrow$ F une application de Fredholm ; adoptons les notations de la condition (iv) de la prop. 2 de III, p. 42. On a alors ind($u$) $=$ dim(F$_2)-$ dim(E$_2)$. Munissons le dual de chacun de ces espaces de la topologie faible (resp. de la topologie compacte, de la convergence bornée). Alors $E'$ s’identifie à la somme directe topologique de $E'_1$ et $E'_2$, et $F'$ à celle de $F'_1$ et $F'_2$, et $^tu$ induit un isomorphisme de $F'_1$ sur $E'_1$ et s’annule sur $F'_2$. Donc la transposée $^tu: F'\rightarrow E'$ est une application de Fredholm (loc. cit.). Le noyau de $^tu$ est $F'_2$, et sa dimension est celle de $F_2$, c’est-à-dire celle du conoyau de $u$. Donc

(3) ind($u$) $=$ dim Ker($^tu$)$-$ dim Ker($u$). De plus, l’image de $^tu$ est $E'_1$, et la dimension du conoyau de $^tu$ est donc égale à la dimension de $E'_2$, qui est celle du noyau $E_2$ de $u$. On en déduit

(4) ind($^tu$) $=-$ ind($u$).

Supposons E et F séparés et soit $u: E\rightarrow$ F une application de Fredholm d’indice 0. Alors $u$ est un morphisme strict d’après la prop. 2 de III, p. 42. Comme dim Ker($u$) $=$ codim$_F$ Im($u$), l’application $u$ est un isomorphisme dès qu’elle est injective ou surjective.

#### Proposition 3 {#ts-iii-s3-prop-3 .statement tag=02RM}

Soient E et F des espaces localement convexes et $u\in \mathscr{L}(E; F)$. Soit $E_1($resp. $F_1)$ un sous-espace fermé de codimension finie de E (resp. F). On suppose que $u$ applique $E_1$ dans $F_1$ et l’on note $u_1\in \mathscr{L}(E_1; F_1)$ l’application qui coïncide avec $u$ sur $E_1$. Pour que $u$ soit une application de Fredholm, il faut et il suffit que $u_1$ en soit une. On a alors

(5) ind($u$)$-$ ind($u_1$) $=$ codim$_F(F_1)-$ codim$_E(E_1)$.

Soient $i: E_1\rightarrow E$ et $j: F_1\rightarrow F$ les injections canoniques. Ce sont des applications de Fredholm, et l’on a

ind($i$) $=$ codim$_E(E_1)$, ind($j$) $=$ codim$_F(F_1)$.

Comme $j\circ u_1=u\circ i$, on voit que $u$ est une application de Fredholm si et seulement si $u_1$ en est une (remarques 3 et 4 de III, p. 41). S’il en est ainsi, on a

ind($j$) $+$ ind($u_1$) $=$ ind($j\circ u_1$) $=$ ind($u\circ i$) $=$ ind($u$) $+$ ind($i$),

d’où la formule (5).

#### Proposition 4 {#ts-iii-s3-prop-4 .statement tag=02RN}

Soient E et F des espaces localement convexes séparés, $u: E\rightarrow F$ une application de Fredholm, et $\widehat{u}:\widehat{E}\rightarrow \widehat{F}$ le prolongement de $u$ aux complétés. Alors $\widehat{u}$ est une application de Fredholm et l’on a Ker($\widehat{u}$) $=$ Ker($u$) et ind($\widehat{u}$) $=$ ind($u$).

Adoptons les notations de la condition (iv) de la prop. 2 de III, p. 42. Comme les espaces vectoriels $E_2$ et $F_2$ sont de dimension finie, ils sont complets. Le complété de $E_1$ (resp. $F_1)$ s’identifie à l’adhérence de $E_1$ dans $\widehat{E}$ (resp. de $F_1$ dans $\widehat{F})$, et $\widehat{E}$ (resp. $\widehat{F})$ est somme directe topologique de $\widehat{E}_1$ et $E_2$ (resp. $\widehat{F}_1$ et $F_2)$. L’application linéaire $\widehat{u}$ définit par restriction un isomorphisme de $\widehat{E}_1$ sur $\widehat{F}_1$ et s’annule sur $E_2$. La proposition résulte alors de l’implication (iv)$\Rightarrow$(i) de loc. cit.

### 4. Endomorphismes de Riesz

Soit E un espace vectoriel et soit $u$ un endomorphisme de E.

La suite (Ker($u^n$))$_{n\in\mathbf{N}}$ de sous-espaces vectoriels de E est croissante ; leur réunion est un sous-espace de E stable par $u$ qu’on appelle nilespace de $u$.

La suite (Im($u^n$))$_{n\in\mathbf{N}}$ de sous-espaces vectoriels de E est décroissante ; leur intersection est un sous-espace de E stable par $u$ qu’on appelle conilespace de $u$.

#### Lemme 2 {#ts-iii-s3-lem-2 .statement tag=02RO}

Soit E un espace vectoriel et soit $u$ un endomorphisme de E qui possède un indice (A, V, p. 126).

Si deux des propriétés suivantes sont satisfaites, il en est de même de la troisième :

(i) L’endomorphisme $u$ est d’indice 0 ;

(ii) Le nilespace N de $u$ est de dimension finie ;

(iii) Le conilespace I de $u$ est de codimension finie.

Pour tout entier $n\geqslant 0$, l’endomorphisme $u^n$ possède un indice, égal à $n$ ind($u$) (A, V, p. 127, lemme 2). La suite (dim(Ker($u^n$)))$_{n\in\mathbf{N}}$ d’entiers naturels est croissante ; pour qu’elle soit stationnaire, il faut et il suffit que le nilespace de $u$ soit de dimension finie. La suite (codim$_E$(Im($u^n$)))$_{n\in\mathbf{N}}$ d’entiers naturels est croissante ; pour qu’elle soit stationnaire, il faut et il suffit que le conilespace de $u$ soit de dimension finie. Supposons la condition (i) satisfaite ; la relation

dim(Ker($u^n$))$-$ codim$_E$(Im($u^n$)) $=$ ind($u^n$) $=n$ ind($u$) $= 0$

entraîne alors l’équivalence des condition (ii) et (iii). Inversement, si les conditions (ii) et (iii) sont satisfaites, cette formule entraîne que la suite $(n$ ind($u$))$_{n\in\mathbf{N}}$ est stationnaire, donc $u$ est d’indice nul.

#### Lemme 3 {#ts-iii-s3-lem-3 .statement tag=02RP}

Soit E un espace vectoriel et soit $u$ un endomorphisme de E qui possède un indice. Supposons que l’indice de $u$ est nul. Soit N le nilespace de $u$ et I son conilespace.

a) L’espace E est alors somme directe des sous-espaces N et I (décomposition de Weyr–Fitting, cf. A, VIII, §2, n$^o2$, p. 25).

b) L’endomorphisme $u$ induit, par passage aux sous-espaces, un endomorphisme nilpotent de N et un automorphisme $u_I$ de I.

c) Notons $v$ l’endomorphisme de E qui est nul sur N et qui coïncide avec $u^{-1}_I$ sur I. On a $u\circ v=v\circ u$ et l’endomorphisme $1_E-u\circ v$ est le projecteur d’image N et de noyau I.

d) Tout endomorphisme de E qui commute à $u$ stabilise N et I, et commute à $v$.

L’endomorphisme $u$ vérifie les propriétés du lemme précédent.

Soit $n\in \mathbf{N}$ tel que Ker($u^n$) $= N$. Alors Ker($u^m$) $=$ Ker($u^n$) pour tout entier $m\geqslant n$; comme ind($u^m$) $=m$ ind($u$) $= 0$, cela entraîne Im($u^m$) $=$ Im($u^n$) pour $m\geqslant n$, donc I = Im($u^n$). Il résulte de A, VIII, p. 25, prop. 2 que les assertions a) et b) sont satisfaites.

Pour tout $x\in N$, on a $v(x) = 0$ et $u(x)\in N$, donc $u(v(x)) = 0$ et $v(u(x)) = 0$. Pour tout $x\in I$, on a $u(v(x)) =v(u(x)) =x$. Cela entraîne que $u\circ v=v\circ u$ et que $1_E-u\circ v$ est le projecteur d’image N et de noyau I.

Soit $w$ un endomorphisme de E qui commute à $u$. Soit $n\in \mathbf{N}$ tel que N = Ker($u^n$) et I = Im($u^n$). Soit $x\in N$; on a $u^n(w(x)) =w(u^n(x)) = 0$, donc $w(x)\in N$. Soit $x\in I$; il existe $y\in E$ tel que $x=u^n(y)$; alors, $w(x) =w(u^n(y)) =u^n(w(y))\in I$. Cela prouve que $w$ stabilise N et I.

Prouvons enfin que $w$ et $v$ sont permutables. Pour tout $x$ dans N, on a $v(w(x)) = 0 =w(v(x))$. Soit $x\in I$; les éléments $v(w(x))$ et $w(v(x))$ de E appartiennent à I et leurs images par $u$ sont toutes deux égales à $w(x)$, donc ils sont égaux. Par linéarité, cela entraîne que $v$ et $w$ commutent.

#### Remarque {#ts-iii-s3-n4-rem-1 .statement tag=02RQ}

Supposons qu’il existe un entier $n\geqslant 0$ tel que Ker($u^n$) $=$ Ker($u^{n+1}$) (resp. Im($u^n$) $=$ Im($u^{n+1}$)); on a alors Ker($u^m$) $=$ Ker($u^n$) (resp. Im($u^m$) $=$ Im($u^n$)) pour tout entier $m\geqslant n$.

Supposons $u$ d’indice nul. Pour tout entier $n\geqslant 0$, on a

$n$ ind($u$) $=$ ind($u^n$) $=$ codim$_E$(Im($u^n$))$-$ dim(Ker($u^n$)).

Les conditions Ker($u^n$) $=$ Ker($u^{n+1}$) et Im($u^n$) $=$ Im($u^{n+1}$) sont donc équivalentes. Lorsqu’elles sont satisfaites, l’espace vectoriel E est somme directe de Ker($u^n$) et de Im($u^n$) (A, VIII, p. 25, prop. 2), l’espace Ker($u^n$) est de dimension finie, et $u$ induit par passage aux sous-espace un automorphisme de Im($u^n$).

#### Définition 2 {#ts-iii-s3-def-2 .statement tag=02RR}

Soit E un espace localement convexe séparé. On appelle endomorphisme de Riesz de E tout endomorphisme de Fredholm de E dont le nilespace est de dimension finie et le conilespace est de codimension finie.

#### Proposition 5 {#ts-iii-s3-prop-5 .statement tag=02RS}

Soit E un espace localement convexe séparé. Tout endomorphisme de Riesz de E est d’indice zéro.

Cela résulte de la définition et du lemme 2.

#### Exemple 1 {#ts-iii-s3-n4-exa-1 .statement tag=02RT}

Tout automorphisme de E est un endomorphisme de Riesz de E. Si E est de dimension finie, tout élément de $\mathscr{L}(E)$ est un endomorphisme de Riesz de E.

#### Exemple 2 {#ts-iii-s3-n4-exa-2 .statement tag=02RU}

Si $(E_i)_{i\in I}$ est une famille finie d’espaces localement convexes séparés et $u_i$ un élément de $\mathscr{L}(E_i)$ pour tout $i$ dans I, l’endomorphisme $u=\bigoplus_{i\in I}u_i$ de l’espace localement convexe $\bigoplus_{i\in I}E_i$ est un endomorphisme de Riesz si et seulement $u_i$ en est un pour tout $i$.

#### Exemple 3 {#ts-iii-s3-n4-exa-3 .statement tag=02RV}

Soit E un espace localement convexe séparé sur $\mathbf{R}$, et soit $E_{(\mathbf{C})}$ son complexifié. Soit $u$ un endomorphisme de E. Pour que $u$ soit un endomorphisme de Riesz, il faut et il suffit que son complexifié $u_{(\mathbf{C})}$ soit un endomorphisme de Riesz de $E_{(\mathbf{C})}$.

#### Proposition 6 {#ts-iii-s3-prop-6 .statement tag=02RW}

Soit E un espace localement convexe séparé et soit $u$ un endomorphisme de Riesz de E. Notons N le nilespace de $u$ et I son conilespace.

a) Les sous-espaces N et I de E sont fermés et stables par $u$, et l’espace E est leur somme directe topologique ;

b) L’endomorphisme $u$ définit par restriction un automorphisme $u_I$ de I ;

c) L’espace vectoriel N est de dimension finie et $u$ définit par restriction un endomorphisme nilpotent $u_N$ de N ;

d) Soit $v$ l’élément de $\mathscr{L}(E)$ qui est nul sur N et coïncide avec $u^{-1}_I$ sur I. C’est un endomorphisme de Riesz de E et un quasi-inverse de $u$ qui commute à $u$. L’endomorphisme $1_E-u\circ v$ de E est le projecteur d’image N et de noyau I. Tout élément de $\mathscr{L}(E)$ qui commute à $u$ stabilise N et I, et commute à $v$.

Soit $n$ un entier naturel tel que Ker($u^n$) $= N$ et Im($u^n$) $= I$. Comme E est séparé et $u$ est continu, N = Ker($u^n$) est fermé dans E. Comme $u$ est un endomorphisme de Fredholm, il en est de même de $u^n$, et I = Im($u^n$) est fermé (III, p. 42, prop. 2). D’après le lemme 2, l’espace E est somme directe de N et I et l’assertion a) résulte alors de la prop. 3 de EVT, I, p. 15.

Comme I est fermé, de codimension finie dans E et stable par $u$, l’application $u_I: I\rightarrow I$ déduite de $u$ est un endomorphisme de Fredholm (III, p. 44, prop. 3) ; elle est aussi bijective, donc c’est un automorphisme de I (III, p. 42, prop. 2). Cela prouve b) et les assertions restantes découlent du lemme 2.

L’endomorphisme $v$ défini dans l’assertion d) de la proposition est un quasi-inverse de $u$, que l’on appelle le quasi-inverse canonique de $u$.

Les endomorphismes de Riesz jouissent de certaines des propriétés de stabilité des applications de Fredholm.

#### Proposition 7 {#ts-iii-s3-prop-7 .statement tag=02RX}

Soit E un espace localement convexe séparé et soit $u$ un endomorphisme de E.

a) Soit $E_1$ un sous-espace fermé de codimension finie de E, stable par $u$. Notons $u_1$ l’élément de $\mathscr{L}(E_1)$ qui coïncide avec $u$ sur $E_1$. Alors $u$ est un endomorphisme de Riesz si et seulement si $u_1$ en est un ;

b) Supposons que $u$ est un endomorphisme de Fredholm d’indice 0. Soit $\widehat{E}$ le complété de E et soit $\widehat{u}\in \mathscr{L}(\widehat{E})$ le prolongement par continuité de $u$. Alors $u$ est un endomorphisme de Riesz si et seulement si $\widehat{u}$ en est un ;

c) Munissons le dual $E'$ de E de la topologie de la convergence bornée, de la topologie de la convergence compacte, ou de la topologie faible. Si $u$ est un endomorphisme de Riesz de E, alors $^tu$ est un endomorphisme de Riesz de $E'$.

a) Pour que $u$ soit un endomorphisme de Fredholm d’indice nul, il faut et il suffit que $u_1$ en soit un (III, p. 44, prop. 3). D’autre part, pour tout $n\in \mathbf{N}$, on a Ker($u^n_1$) $= E_1\cap$ Ker($u^n$), d’où

dim Ker($u^n_1$)$\leqslant$ dim Ker($u^n$)$\leqslant$ dim Ker($u^n_1$) $+$ codim$_E(E_1)$,

donc la suite (dim Ker($u^n$))$_{n\in\mathbf{N}}$ est bornée si et seulement si la suite (dim Ker($u^n_1$))$_{n\in\mathbf{N}}$ l’est. Par suite, $u$ est un endomorphisme de Riesz de E si et seulement si $u_1$ est un endomorphisme de Riesz de $E_1$ (lemme 2).

b) D’après la prop. 4 de III, p. 44, pour tout $n\in \mathbf{N}$, l’application $\widehat{u}^n$ est un endomorphisme de Fredholm de $\widehat{E}$ tel que Ker($\widehat{u}^n$) $=$ Ker($u^n$) et ind($\widehat{u}^n$) $=$ ind($u^n$) $=n$ ind($u$). Par suite, $u$ est un endomorphisme de Riesz si et seulement si $\widehat{u}$ est un endomorphisme de Riesz.

c) La transposée $^tu$ est un endomorphisme de Fredholm d’indice 0 de $E'($III, p. 43, n$^o3$). Comme le noyau de $(^tu)^n$ est l’orthogonal de l’image de $u^n$ (EVT, IV, p. 27, prop. 2), la suite (Ker($^tu$)$^n)_n$ est stationnaire. Cela prouve que $^tu$ est un endomorphisme de Riesz de $E'$.

#### Proposition 8 {#ts-iii-s3-prop-8 .statement tag=02RY}

Soient E un espace localement convexe séparé et $u$ un endomorphisme de E. Les conditions suivantes sont équivalentes :

(i) $u$ est un endomorphisme de Riesz de E ;

(ii) Il existe un quasi-inverse $v$ de $u$ qui commute à $u$;

(iii) Il existe un sous-espace vectoriel fermé $E_1$ de E, de codimension finie, stable par $u$, tel que $u$ induise un automorphisme de $E_1$.

L’implication (i) $=\Rightarrow$ (ii) résulte de la prop. 6, d).

Supposons que $u$ possède un quasi-inverse $v$ qui est permutable à $u$. Le noyau $E_1$ de $1_E-u\circ v$ est un sous-espace vectoriel fermé de E, de codimension finie, stable par $u$ et $v$. Comme on a $u(v(x)) =v(u(x)) =x$ pour tout $x\in E_1$, les applications $u$ et $v$ induisent des automorphismes de $E_1$ réciproques l’un de l’autre. Donc (ii) implique (iii).

Enfin, l’implication (iii) $=\Rightarrow$ (i) résulte de l’assertion a) de la prop. 7 et du fait qu’un automorphisme est un endomorphisme de Riesz.

#### Proposition 9 {#ts-iii-s3-prop-9 .statement tag=02RZ}

Soit E un espace localement convexe séparé et soient $u,v$ des éléments permutables de $\mathscr{L}(E)$. Les conditions suivantes sont équivalentes :

(i) Les endomorphismes $u$ et $v$ sont des endomorphismes de Riesz ;

(ii) L’endomorphisme $u\circ v$ est un endomorphisme de Riesz.

Supposons que $u$ et $v$ soient des endomorphismes de Riesz ; notons $u'$ et $v'$ leurs quasi-inverses canoniques. Les endomorphismes $u,v,u'$ et $v'$ de E commutent (prop. 6, d)). L’endomorphisme $v'\circ u'$ est un quasi-inverse de $u\circ v$ qui commute à $u\circ v$, donc $u\circ v$ est un endomorphisme de Riesz (prop. 8).

Supposons inversement que $u\circ v$ est un endomorphisme de Riesz, et soit $w$ son quasi-inverse canonique. Puisque $u$ commute à $u\circ v$, les endomorphismes $u$ et $w$ commutent d’après la prop. 6, d). De même $v$ et $w$ commutent. Donc les endomorphismes $u,v$ et $w$ de E commutent ; il en découle que l’endomorphisme $v\circ w$ de E est un quasi-inverse de $u$ et que $w\circ u$ est un quasi-inverse de $v$. D’après la prop. 8$,u$ et $v$ sont des endomorphismes de Riesz.

Soit $u$ un endomorphisme de Riesz de E. Si $v$ est un automorphisme de E, l’endomorphisme $u\circ v$ de E n’est pas nécessairement un endomorphisme de Riesz de E, même si $u\circ v-v\circ u$ est de rang fini. Si $h$ est un endomorphisme de rang fini de E, l’endomorphisme $u+h$ n’est pas nécessairement un endomorphisme de Riesz (cf. III, p. 120, exercice 3).

#### Proposition 10 {#ts-iii-s3-prop-10 .statement tag=02S0}

Soient E et F des espaces localement convexes, $p\in \mathscr{L}(E; F)$ et $q\in \mathscr{L}(F; E)$. Posons $u= 1_E-q\circ p$ et $v= 1_F-p\circ q$.

a) Soit $n\in \mathbf{N}$. L’application $p$ définit par restriction un isomorphisme d’espaces vectoriels topologiques de Ker($u^n$) sur Ker($v^n$) et définit par passage aux quotients un isomorphisme d’espaces vectoriels topologiques de Coker($u^n$) sur Coker($v^n$);

b) Si l’image de $u$ est fermée dans E, celle de $v$ est fermée dans F ;

c) Si Ker($u$) possède un supplémentaire topologique dans E, alors Ker($v$) en possède un dans F. Si Im($u$) possède un supplémentaire topologique dans E, alors Im($v$) en possède un dans F ;

d) Si $u$ est un morphisme strict, alors $v$ est un morphisme strict ;

e) Si $u$ est un automorphisme de E, alors $v$ est un automorphisme de F ;

f) Si $u$ est un endomorphisme de Fredholm de E, alors $v$ est un endomorphisme de Fredholm de F, et l’on a ind($u$) $=$ ind($v$);

g) Supposons E et F séparés. Si $u$ est un endomorphisme de Riesz de E, alors $v$ est un endomorphisme de Riesz de F.

Remarquons tout d’abord les formules

$$
q\circ v=u\circ q,v\circ p=p\circ u \tag{6}
$$

Démontrons alors deux lemmes.

#### Lemme 4 {#ts-iii-s3-lem-4 .statement tag=02S1}

Soit $n\in \mathbf{N}$. Posons

$ni-1(n)i-1$

$q_n=\sum(-1)q\circ (p\circ q)$.

$$
i
$$

$i=1$

On a $u^n= 1_E-q_n\circ p$ et $v^n= 1_F-p\circ q_n$.

On a $(q\circ p)^i=q\circ (p\circ q)^{i-1}\circ p$ pour tout entier $i\geqslant 1$. On calcule alors

$nnni-1(n)i$

$u= (1_E-q\circ p)= 1_E-\sum(-1)(q\circ p)= 1_E-q_n\circ p$

$$
i
$$

$$
i=1
$$

$nnni-1(n)i$

$v= (1_F-p\circ q)= 1_F-\sum(-1)(p\circ q)= 1_F-p\circ q_n$,

$$
i
$$

$i=1$

d’où le résultat.

#### Lemme 5 {#ts-iii-s3-lem-5 .statement tag=02S2}

Soit $u'$ un élément de $\mathscr{L}(E)$. Posons $v'= 1_F+p\circ u'\circ q$. Si $u'$ est un inverse de $u$, alors $v'$ est un inverse de $v$. Si $u'$ est un quasi-inverse de $u$, alors $v'$ est un quasi-inverse de $v$. Si $u'$ commute à $u$, alors $v'$ commute à $v$.

En utilisant les formules (6), on calcule

$$
v-v'\circ v=-p\circ u'\circ q\circ v=-p\circ u'\circ u\circ q
$$

$$
v-v\circ v'=-v\circ p\circ u'\circ q=-p\circ u\circ u'\circ q
$$

d’où

$$
1_F-v'\circ v=p\circ (1_E-u'\circ u)\circ q
$$

$$
1_F-v\circ v'=p\circ (1_E-u\circ u')\circ q
$$

ce qui démontre le lemme.

Démontrons la prop. 10. Compte tenu du lemme 4, il suffit de démontrer l’assertion a) pour $n= 1$. D’après les formules (6), les applications $p$ et $q$ définissent par passage aux sous-espaces des applications linéaires continues $p':$ Ker($u$)$\rightarrow$ Ker($v$) et $q':$ Ker($v$)$\rightarrow$ Ker($u$), et par passage aux quotients des applications linéaires continues $p'':$ Coker($u$)$\rightarrow$ Coker($v$) et $q'':$ Coker($v$)$\rightarrow$ Coker($u$).

Puisque $1_E-u=q\circ p$ et $1_F-v=p\circ q$, les applications $p'$ et $q'$ d’une part, $p''$ et $q''$ d’autre part, sont des isomorphismes réciproques l’un de l’autre. Cela prouve a).

Pour que l’image d’une application linéaire continue soit fermée, il faut et il suffit que le conoyau de cette application soit un espace séparé. Ainsi b) résulte de a).

Notons $i: Ker(u)\rightarrow E$ et $j:$ Ker($v$)$\rightarrow F$ les injections canoniques. Supposons que Ker($u$) possède un supplémentaire topologique dans E, et soit $r: E\rightarrow$ Ker($u$) une rétraction linéaire continue de $i$. Posons $r'=p'\circ r\circ q$. On a $r'\in \mathscr{L}(F$; Ker($v$)) et

$$
r'\circ j=p'\circ r\circ q\circ j=p'\circ r\circ i\circ q'=p'\circ q'= 1_{Ker(v)}
$$

donc $r'$ est une rétraction linéaire continue de $j$ et Ker($v$) possède un supplémentaire topologique dans F. Cela démontre la première assertion de c). La seconde se démontre de manière analogue, en remarquant que si $s:$ Coker($u$)$\rightarrow E$ est une section linéaire continue de la surjection canonique de E sur Coker($u$), alors $p\circ s\circ q''$ en est une de la surjection canonique de F sur Coker($v$).

Notons $u: E/$ Ker($u$)$\rightarrow$ Im($u$) et $v: F/$ Ker($v$)$\rightarrow$ Im($v$) les applications linéaires continues bijectives déduites de $u$ et $v$. D’après les formules (6), l’application $p$ définit par passage aux quotients une application linéaire continue $p_1: E/$ Ker($u$)$\rightarrow F/$ Ker($v$), et $p,q$ définissent par passage aux sous-espaces des applications linéaires continues $p_0:$ Im($u$)$\rightarrow$ Im($v$) et $q_0:$ Im($v$)$\rightarrow$ Im($u$).

Notons $t:$ Im($v$)$\rightarrow F/$ Ker($v$) l’application composée de l’injection canonique Im($v$)$\rightarrow F$ et de la surjection canonique $F\rightarrow F/$ Ker($v$); elle est continue. On a $v\circ t= 1_{Im(v)}-p_0\circ q_0$ et $v\circ p_1=p_0\circ u$, d’où

$$
v\circ (t+p_1\circ u^{-1}\circ q_0) =v\circ t+p_0\circ q_0= 1_{Im(v)}
$$

Cela prouve que $t+p_1\circ u^{-1}\circ q_0$ est la bijection réciproque de $v$. Si $u$ est stricte, l’application $u^{-1}$ est continue, et il en est de même de $v^{-1}$, ce qui prouve que $v$ est stricte. Cela démontre d).

D’après le lemme 5, si $u$ est un automorphisme de E, alors $v$ en est un de F. De même, si $u$ est un endomorphisme de Fredholm de E, alors $v$ en est un de F, et l’on a alors ind($u$) $=$ ind($v$) d’après a). Ceci démontre e) et f). Enfin, si E et F sont séparés et que $u$ est un endomorphisme de Riesz de E, alors $v$ en est un de F d’après le lemme 5 et la condition (ii) de la prop. 8 ; c’est l’assertion g).

### 5. Applications de Fredholm et applications de Riesz entre espaces de Fréchet

#### Proposition 11 {#ts-iii-s3-prop-11 .statement tag=02S3}

Soient E et F des espaces de Fréchet. Pour qu’une application linéaire continue $u$ de E dans F soit une application de Fredholm, il faut et il suffit que son noyau et son conoyau soient de dimension finie.

Cela résulte de la caractérisation des applications de Fredholm donnée par la condition (ii) de la prop. 2 de III, p. 42 et du lemme suivant :

#### Lemme 6 {#ts-iii-s3-lem-6 .statement tag=02S4}

Soient E et F des espaces de Fréchet et $u\in \mathscr{L}(E; F)$. On suppose que l’image de $u$ est de codimension finie dans F. Alors l’image de $u$ est fermée dans F et $u$ est un morphisme strict.

Soit G un sous-espace vectoriel de F supplémentaire de Im($u$); le sous-espace G est fermé (EVT, I, p. 14, cor. 1), donc l’espace quotient $F/G$ est un espace de Fréchet (TG, IX, p. 25, prop. 4). Soit $\pi : F\rightarrow F/G$ la surjection canonique. L’application $\pi \circ u$ est surjective, donc stricte (EVT, I, p. 19, cor. 3). L’assertion résulte alors du cor. 2 de III, p. 40.

#### Proposition 12 {#ts-iii-s3-prop-12 .statement tag=02S5}

Soient E et F des espaces de Fréchet. Munissons leurs duals $E'$ et $F'$ de la topologie faible, de la topologie de la convergence compacte, ou de la topologie de la convergence bornée. Soit $u\in \mathscr{L}(E; F)$. Pour que $u$ soit une application de Fredholm de E dans F, il faut et il suffit que $^tu$ soit une application de Fredholm de $F'$ dans $E'$.

La condition est nécessaire (III, p. 43, n$^o3$). Démontrons qu’elle est suffisante. Si $^tu$ est une application de Fredholm, c’est un morphisme strict (III, p. 42, prop. 2), donc $u$ est un morphisme strict d’image fermée (EVT, IV, p. 28, th. 1 et p. 29, cor. 3). Compte tenu des isomorphismes canoniques Coker($^tu$)$\rightarrow$ Ker($u$)$'$ et Ker($^tu$)$\rightarrow$ Coker($u$)$'$ (EVT, IV, p. 27, prop. 2), les espaces vectoriels Ker($u$) et Coker($u$) sont de dimension finie et $u$ est une application de Fredholm (prop. 2 de III, p. 42).

#### Proposition 13 {#ts-iii-s3-prop-13 .statement tag=02S6}

Soient E un espace de Fréchet et $u\in \mathscr{L}(E)$.

a) L’endomorphisme $u$ est un endomorphisme de Riesz si et seulement si son nilespace N est de dimension finie et son conilespace I est de codimension finie ;

b) Munissons $E'$ de la topologie de la convergence bornée, de la topologie de la convergence compacte, ou de la topologie faible. Si $^tu$ est un endomorphisme de Riesz de $E'$, alors $u$ est un endomorphisme de Riesz de E.

a) Supposons que le nilespace N est de dimension finie et que le conilespace I est de codimension finie. Comme Ker($u$)$\subset N$ et $I\subset$ Im($u$), le noyau de $u$ est de dimension finie et l’image de $u$ est de codimension finie. D’après la définition et la proposition 11, l’application $u$ est un endomorphisme de Riesz. La réciproque découle de la définition.

b) D’après la proposition 12, l’hypothèse implique que $u$ est un endomorphisme de Fredholm d’indice ind($^tu$) $=-$ ind($u$) $= 0$ (n$^o3$, formule (4)). Soit $n\in \mathbf{N}$. Comme l’image de $u^n$ est fermée et a pour orthogonal le noyau de $^tu^n$ (EVT, IV, p. 27, prop. 2), la suite (Im($u^n$)) est stationnaire, et $u$ est donc un endomorphisme de Riesz.

### 6. Caractérisation spectrale des endomorphismes de Riesz

Soient E un espace de Banach complexe et $u$ un endomorphisme de E. Rappelons que l’on note Sp($u$) le spectre de $u$ relativement à l’algèbre de Banach unifère $\mathscr{L}(E) ($cf. § 7 de I, p. 127).

Supposons que 0 est un point isolé de Sp($u$); rappelons qu’on note alors $e_0(u)$ le projecteur spectral associé à $u$ et à la partie ouverte et fermée $\{0\}$ du spectre de $u($cf. n$^o3$ de I, p. 131). On a $e_0(u) =f(u)$ pour tout germe de fonction holomorphe $f$ au voisinage de Sp($u$) qui est égal à 1 au voisinage de 0 et nul au voisinage de Sp($u$)$-\{0\}$.

Par passage aux sous-espaces, l’endomorphisme $u$ induit un endomorphisme quasi-nilpotent de l’image de $e_0(u)$, dont le spectre est réduit à $\{0\}$, et un automorphisme du noyau de $e_0(u)$, dont le spectre est Sp($u$)$-\{0\}($loc. cit.).

#### Proposition 14 {#ts-iii-s3-prop-14 .statement tag=02S7}

Soit E un espace de Banach complexe. Pour qu’un élément $u$ de $\mathscr{L}(E)$ soit un endomorphisme de Riesz de E, il faut et il suffit que l’une des deux conditions suivantes, qui s’excluent mutuellement, soit satisfaite :

(i) L’endomorphisme $u$ de E est un automorphisme de E ;

(ii) Le point 0 est un point isolé de Sp($u$) et le projecteur $e_0(u)$ est de rang fini.

Lorsque la condition (ii) est satisfaite, l’image de $e_0(u)$ est le nilespace de $u$ et le noyau de $e_0(u)$ est le conilespace de $u$.

Tout automorphisme de E est un endomorphisme de Riesz de E (III, p. 47, remarque 1). Si $u$ satisfait à la condition (ii), le noyau F de $e_0(u)$ est un sous-espace vectoriel fermé de codimension finie de E, stable par $u$. Soit $u_F$ l’endomorphisme de F déduit de $u$. Son spectre est contenu dans $\mathbf{C}-\{0\}$ (n$^o3$ de I, p. 131), donc $u_F$ est un automorphisme de F. Il en résulte que $u$ est un endomorphisme de Riesz de E (III, p. 48, prop. 8).

Inversement, soit $u$ un endomorphisme de Riesz de E. Notons N son nilespace et I son conilespace. D’après la prop. 6 de III, p. 47, l’espace E est somme directe topologique de N et I, et l’application $u$ définit par passage aux sous-espaces un endomorphisme nilpotent $u_N$ de N et un automorphisme $u_I$ de I. En particulier, on a Sp($u_N$)$\subset  \{0\}$ et $0\not \in$ Sp($u_I$). Si N est nul, alors I = E et $u$ est un automorphisme de E. Sinon, 0 est un point isolé de Sp($u$) et $e_0(u)$ est le projecteur d’image N et de noyau I (prop. 2 de I, p. 129) ; en particulier, il est de rang fini.

#### Remarque {#ts-iii-s3-n6-rem-1 .statement tag=02S8}

Soit E un espace de Banach réel et soit $u$ un endomorphisme de E. Supposons que 0 soit un point isolé du spectre complexe de $u$, c’est-à-dire du spectre de l’endomorphisme $1\otimes u$ de l’espace normable complet complexifié $E_{(\mathbf{C})}$ de E (I, p. 85, n$^o13$). La partie $\{0\}$ du spectre complexe de $u$ est ouverte et fermée, et invariante par conjugaison ; notons $e_0(u)\in \mathscr{L}(E)$ le projecteur spectral qui lui est associé (n$^o13$ de I, p. 85). La proposition 14 vaut mutatis mutandis dans ce cadre.

## EXERCICES {#ts-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).

[^1]: Certains auteurs disent aussi « opérateur à indice » ou « quasi-isomorphisme ».
