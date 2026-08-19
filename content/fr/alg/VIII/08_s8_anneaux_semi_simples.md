---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Modules et anneaux semi-simples
section: 8
section_title: Anneaux semi-simples
lang: fr
source: alg-viii-fr
book_pages: A VIII.131-A VIII.145
pdf_pages: 0138-0152
extraction: native
subsections:
    - "no": 1
      title: Anneaux semi-simples
      page: 131
      pdf_page: 138
    - "no": 2
      title: Modules sur un anneau semi-simple
      page: 134
      pdf_page: 141
    - "no": 3
      title: Facteurs d’un anneau semi-simple
      page: 136
      pdf_page: 143
    - "no": 4
      title: Idempotents et anneaux semi-simples
      page: 140
      pdf_page: 147
statements: 30
exercises: 6
content_sha256: d022b8b7bcc0df4ce265d5b13c85dd980b872df2a090b3cde80e39237c2e7d84
---

## § 8. ANNEAUX SEMI-SIMPLES

### 1. Anneaux semi-simples

#### Théorème 1 (Wedderburn) {#alg-viii-s8-thm-1 .statement tag=00S4}

Soit A un anneau. Les conditions suivantes sont équivalentes :

(i) Le A-module $A_s$ est semi-simple ;

(ii) Pour tout idéal à gauche $\mathfrak{a}$ de A, il existe un idéal à gauche $\mathfrak{b}$ de A tel que $A_s$ soit somme directe de $\mathfrak{a}$ et $\mathfrak{b}$;

(iii) L’anneau A est artinien à gauche et le $(A,A)$-bimodule $_sA_d$ est semi-simple ;

(iv) L’anneau A est isomorphe au produit d’une famille finie d’anneaux simples ;

(v) Il existe un entier $s\geqslant 0$, des corps $D_1, . . . ,D_s$ et des entiers $r_1\geqslant 1, . .$., $r_s\geqslant 1$tels que l’anneau A soit isomorphe au produit des anneaux de matrices $\mathbf{M}_{r_i}(D_i)$;

(vi) L’anneau A est artinien à gauche et il existe un A-module à gauche semi-simple et fidèle.

L’équivalence de (i) et (ii) résulte du cor. 2 de VIII, p. 52, et celle de (iv) et (v) résulte du th. 1 de VIII, p. 116.

Le A-module $A_s$ est de type fini. S’il est semi-simple, il est artinien à gauche (VIII, p. 67, prop. 10). Comme le A-module $A_s$ est fidèle, cela prouve que (i) entraîne (vi). Réciproquement, supposons la condition (vi) satisfaite ; soit M un A-module semi-simple fidèle. Il existe un entier $m\geqslant 1$ tel que $A_s$ soit isomorphe à un sous-module de $M^m$ (VIII, p. 46, prop. 5 a)) ; comme M est semi-simple, il en est de même de $A_s$. On a donc prouvé l’équivalence de (i) et (vi).

Démontrons que (i) entraîne (iii). Supposons que l’anneau A satisfasse à la propriété (i) ; on a déjà remarqué que A est alors artinien à gauche. Or les endomorphismes du A-module à gauche $A_s$ sont les multiplications à droite par les éléments de A. Que le $(A$, A)-bimodule $_sA_d$ soit semi-simple résulte alors de la prop. 6 de VIII, p. 81.

Montrons que (iii) entraîne (iv). Supposons que le $(A$, A)-bimodule $_sA_d$ soit semi-simple. Il est de type fini, donc il existe une famille finie $(\mathfrak{a}_i)_{i\in I}$ de sous-(A$,A$)-bimodules simples, dont $_sA_d$ soit la somme directe. Autrement dit, les $\mathfrak{a}_i$ sont des idéaux bilatères non nuls de A, le groupe additif de A est la somme directe des $\mathfrak{a}_i$ et, pour tout $i\in I$, tout idéal bilatère de A contenu dans $\mathfrak{a}_i$ est égal à 0 ou $\mathfrak{a}_i$. Posons $\mathfrak{b}_i=\sum_{j\not=i}\mathfrak{a}_j$ pour tout $i\in I$; c’est un idéal bilatère de A. L’application $a\rightarrow (a+\mathfrak{b}_i)_{i\in I}$ est un isomorphisme de l’anneau A sur le produit des anneaux $A/\mathfrak{b}_i$. Les $(A$, A)-bimodules $\mathfrak{a}_i$ et $A/\mathfrak{b}_i$ sont isomorphes, donc tout idéal bilatère de $A/\mathfrak{b}_i$ est égal à 0 ou $A/\mathfrak{b}_i$. Si l’anneau A est artinien à gauche, il en est de même des anneaux $A/\mathfrak{b}_i$, qui sont donc simples (VIII, p. 116, déf. 1).

Démontrons enfin que (iv) entraîne (i). Supposons que A soit le produit d’une famille finie $(A_i)_{i\in I}$ d’anneaux simples ; notons $\pi_i$ la projection d’indice $i$ de A dans $A_i$, et $M_i$ le A-module ayant $A_i$ pour groupe additif sous-jacent et la loi d’action $(a, x)\rightarrow \pi_i(a)x$. Comme l’anneau $A_i$ est simple, le $A_i$-module $(A_i)_s$ est semi-simple, donc le A-module $M_i$ est semi-simple. Comme le A-module $A_s$ n’est autre que le produit $\prod_{i\in I}M_i$, il est semi-simple.

#### Définition 1 {#alg-viii-s8-def-1 .statement tag=0093}

On dit que l’anneau A est semi-simple s’il satisfait aux conditions équivalentes (i) à (vi) du théorème 1. Une algèbre A sur un anneau commutatif $k$ est une algèbre semi-simple si l’anneau sous-jacent à A est semi-simple.

#### Proposition 1 {#alg-viii-s8-prop-1 .statement tag=0094}

Soit A un anneau semi-simple. Il existe une famille finie $(\mathfrak{m}_i)_{i\in I}$ d’idéaux à gauche minimaux de A telle que $A_s=\oplus_{i\in I}\mathfrak{m}_i$. Si $(\mathfrak{m}_i)_{i\in I}$ est une telle famille, tout A-module simple est isomorphe à l’un des $\mathfrak{m}_i$. L’ensemble des classes de A-modules simples est fini.

La première assertion résulte du fait que le A-module $A_s$ est semi-simple et de type fini. Tout module simple est isomorphe à un quotient de $A_s$ (VIII, p. 42, prop. 1) ; la deuxième assertion résulte alors du cor. 3 de VIII, p. 52, et la troisième s’en déduit aussitôt.

#### Exemple {#alg-viii-s8-n1-exa-1 .statement tag=0095}

Soient G un groupe fini et K un corps commutatif. $*$Nous verrons plus

loin (VIII, p. 391, cor. 1) que l’algèbre K[G] du groupe G sur le corps K est un anneau semi-simple si et seulement si l’exposant caractéristique de K est étranger à l’ordre de $G.*$

#### Remarque 1 {#alg-viii-s8-n1-rem-1 .statement tag=0096}

Soit K un corps commutatif et soit A une algèbre semi-simple sur K. Alors il existe des K-algèbres $D_1, . . . ,D_s$ qui sont des corps et des entiers $r_1\geqslant 1, . . . , r_s\geqslant 1$ tels que la K-algèbre A soit isomorphe au produit $\prod^s_{i=1}\mathbf{M}_{r_i}(D_i)$.

#### Remarque 2 {#alg-viii-s8-n1-rem-2 .statement tag=0097}

Soit K un corps algébriquement clos et soit A une algèbre de degré fini sur K. Compte tenu de la remarque 4 de VIII, p. 118, pour que l’algèbre A soit semi-simple, il faut et il suffit qu’il existe des entiers $n_1\geqslant 1, . . . , n_r\geqslant 1$ tels que A soit isomorphe à l’algèbre $B = \mathbf{M}_{n_1}(K)\times  \cdots  \times \mathbf{M}_{n_r}(K)$.

#### Proposition 2 {#alg-viii-s8-prop-2 .statement tag=0098}

a) Le centre d’un anneau semi-simple est semi-simple.

b) L’anneau opposé d’un anneau semi-simple est semi-simple.

c) Le quotient d’un anneau semi-simple par un idéal bilatère est un anneau semi-simple.

d) Le produit d’une famille finie d’anneaux semi-simples est un anneau semi-simple.

Soit A un anneau semi-simple. Il est isomorphe au produit d’une famille finie $(A_i)_{i\in I}$ d’anneaux simples. Le centre de A est isomorphe au produit des centres des $A_i$, et $A^o$ est isomorphe à l’anneau produit des $A^o_i$. Les assertions a) et b) résultent donc du cor. 1 de VIII, p. 117.

Soit $\mathfrak{a}$ un idéal bilatère de A. Le A-module $A_s/\mathfrak{a}$, quotient du A-module semi-simple $A_s$, est semi-simple. Le $(A/\mathfrak{a}$)-module $A_s/\mathfrak{a}$ est donc semi-simple, d’où c).

Pour qu’un anneau soit semi-simple, il faut et il suffit qu’il soit isomorphe au produit d’une famille finie d’anneaux simples ; l’assertion d) en résulte.

#### Proposition 3 {#alg-viii-s8-prop-3 .statement tag=0099}

Soit A un anneau commutatif. Les propriétés suivantes sont équivalentes :

(i) L’anneau A est semi-simple ;

(ii) L’anneau A est artinien et réduit (V, p. 33) ;

(iii) L’anneau A est isomorphe au produit d’une famille finie de corps commutatifs.

Les anneaux simples commutatifs sont les corps commutatifs (VIII, p. 116, remarque 1). Donc (i) équivaut à (iii).

Il est clair que (iii) entraîne (ii). Réciproquement, supposons l’anneau A artinien et réduit. L’intersection de l’ensemble des idéaux premiers de A se compose des éléments nilpotents de A (V, p. 113, prop. 2), donc est réduite à zéro puisque A est réduit ; compte tenu de VIII, p. 2, il existe alors des idéaux premiers distincts $\mathfrak{p}_1, . . . ,\mathfrak{p}_r$ de A, tels que l’on ait $\mathfrak{p}_1\cap \cdots \cap \mathfrak{p}_r= 0$. D’après le cor. de VIII, p. 8, chacun des idéaux premiers $\mathfrak{p}_i$ de l’anneau artinien A est maximal ; on a donc $\mathfrak{p}_i+\mathfrak{p}_j= A$ lorsque $i$ et $j$ sont distincts. D’après la prop. 9 de I, p. 104, l’homomorphisme canonique de A dans l’anneau $\prod^r_{i=1}(A/\mathfrak{p}_i)$ est un isomorphisme. Pour chaque $i$, l’anneau $A/\mathfrak{p}_i$ est un corps et (ii) entraîne donc (iii).

Une algèbre commutative de degré fini sur un corps est un anneau commutatif artinien. La proposition 3 généralise donc la prop. 5 de V, p. 33.

### 2. Modules sur un anneau semi-simple

#### Proposition 4 {#alg-viii-s8-prop-4 .statement tag=009A}

Soit A un anneau. Les propriétés suivantes sont équivalentes :

(i) L’anneau A est semi-simple ;

(ii) Tout A-module est semi-simple ;

(iii) Il existe un A-module semi-simple et générateur ;

(iv) Il existe un A-module semi-simple et fidèle dont le contremodule est de type fini ;

(v) Tout A-module est projectif ;

(vi) Tout A-module monogène est projectif.

$*$Pour d’autres caractérisations des anneaux semi-simples, voir la prop. 6 de X, p. $140.*$

Démontrons d’abord que (i) entraîne (ii) et (v). Supposons l’anneau A semi-simple et considérons un A-module à gauche M. Par hypothèse, le A-module $A_s$ est semi-simple, donc tout A-module libre est semi-simple. D’après la prop. 20 de II, p. 27, il existe un A-module libre L et une application A-linéaire surjective $u$ de L sur M. Soit N le noyau de $u$; comme le A-module L est semi-simple, il existe un sous-module $N'$ semi-simple supplémentaire de N dans L (VIII, p. 52, th. 1) ; le A-module $N'$ est projectif et $u$ induit un isomorphisme de $N'$ sur M. Par suite, M est semi-simple et projectif.

(ii) $=\Rightarrow$ (iii) : si tout A-module est semi-simple, le A-module $A_s$ est semi-simple ; d’autre part il est générateur.

(iii) $=\Rightarrow$ (iv) : en effet, si M est un A-module générateur, il est fidèle (VIII, p. 76, cor. du th. 1) et son contremodule est de type fini (VIII, p. 95, cor. 1).

(iv) $=\Rightarrow$ (i) : soit M un A-module semi-simple et fidèle dont le contremodule soit de type fini. D’après le lemme 4 de VIII, p. 8 il existe un entier positif $m$ tel que $A_s$ soit isomorphe à un sous-module de $M^m$; le A-module $M^m$ est semi-simple, et il en est donc de même de $A_s$.

L’implication (v) $=\Rightarrow$ (vi) est immédiate.

(vi) $=\Rightarrow$ (i) : supposons que tout A-module monogène soit projectif. Soit $\mathfrak{a}$ un idéal à gauche de A ; comme le A-module $A_s/\mathfrak{a}$ est projectif, il existe un idéal à gauche $\mathfrak{b}$ de A tel que $A_s$ soit somme directe de $\mathfrak{a}$ et $\mathfrak{b}$ (II, p. 39, prop. 4). Par suite l’anneau A est semi-simple (VIII, p. 131, th. 1).

#### Lemme 1 {#alg-viii-s8-lem-1 .statement tag=009B}

Soit A un anneau artinien à gauche et soit M un A-module simple, alors l’anneau $A_M$ est simple.

Comme l’anneau A est artinien à gauche, il en est de même de l’anneau $A_M$, d’après la prop. 5 de VIII, p. 7. Or M est un $A_M$-module simple et fidèle, donc l’anneau $A_M$ est simple (VIII, p. 115, prop. 1).

#### Proposition 5 {#alg-viii-s8-prop-5 .statement tag=009C}

Supposons l’anneau A semi-simple. Soit M un A-module à gauche. Le contremodule de M est de type fini et l’on a $A_M= A''_M$.

Considérons d’abord le cas où M est un A-module simple. Par le lemme 1, l’anneau $A_M$ est simple. La prop. 5 résulte alors du lemme 1 de VIII, p. 116.

Passons au cas général. L’ensemble $\mathscr{S}$ des classes de A-modules simples est fini (VIII, p. 132, prop. 1). Choisissons pour tout $\lambda \in \mathscr{S}$ un A-module $S_{\lambda}$ de classe $\lambda$, et notons $D_{\lambda}$ le corps opposé du commutant de $S_{\lambda}$. D’après le lemme 1 appliqué à l’anneau simple $A_{S_{\lambda}}, S_{\lambda}$ est un espace vectoriel de dimension finie sur le corps $D_{\lambda}$; notons $m(\lambda )$ cette dimension. Soit B l’anneau opposé de l’anneau des endomorphismes de M. On a vu en VIII, p. 80 qu’il existe des $(D_{\lambda}$, B)-bimodules $V_{\lambda}$, simples comme B-modules, et un isomorphisme de $(A$, B)-bimodules de M sur $\oplus_{\lambda\in\mathscr{S}}S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$. En tant que B-module, M est isomorphe à $\oplus_{\lambda\in\mathscr{S}}V^{m(\lambda)}_{\lambda}$. Comme $\mathscr{S}$ et les $m(\lambda )$ sont finis, M est un B-module de type fini.

Le A-module M est semi-simple et son contremodule est de type fini. On a donc $A_M= A''_M$ d’après la prop. 4 de VIII, p. 79.

#### Proposition 6 {#alg-viii-s8-prop-6 .statement tag=009D}

Soit M un A-module semi-simple de type fini. On note $\mathscr{S}_M$ son support (VIII, p. 62) et B l’anneau de ses endomorphismes. Pour tout $\lambda \in \mathscr{S}_M$, on choisit un A-module simple $S_{\lambda}$ de classe $\lambda$, et l’on note $V_{\lambda}$ le B-module à gauche Hom$_A(S_{\lambda},M)$.

a) L’anneau B est semi-simple.

b) L’application $\lambda \rightarrow$ cl(V$_{\lambda}$)est une bijection du support $\mathscr{S}_M$ de M sur l’ensemble des classes de B-modules simples.

c) Pour tout $\lambda \in \mathscr{S}_M$, le composant isotypique de type $\lambda$ du A-module M est égal au composant isotypique de type $V_{\lambda}$ du B-module M.

Considéré comme B-module, M est semi-simple (VIII, p. 80, prop. 5) et fidèle ; son contremodule est de type fini puisque l’on a $A_M\subset$ End$_B(M)$. Donc l’anneau B est semi-simple (VIII, p. 134, prop. 4). Si $(x_1, . . . , x_r)$ est une suite génératrice du A-module M, l’application $b\rightarrow (bx_1, . . . , bx_r)$ de $B_s$ dans $M^r$ est B-linéaire et injective. Tout B-module simple est isomorphe à un sous-module de $B_s$ (VIII, p. 132, prop. 1), donc à un sous-B-module de M. La proposition résulte alors aussitôt de la prop. 5 de VIII, p. 80.

#### Proposition 7 {#alg-viii-s8-prop-7 .statement tag=009E}

Soit A un anneau semi-simple.

a) Tout A-module de type fini est réflexif (II, p. 47).

b) Pour tout A-module à gauche simple S, le A-module à droite $S^*$ dual de S est simple, et l’application $\lambda \rightarrow$ cl($\lambda^*$)définit une bijection de l’ensemble des classes de A-modules simples sur celui des classes de A-modules à droite simples.

c) Soit M un A-module à gauche de type fini, le A-module à droite $M^*$ dual de M est de type fini et a même longueur que M. En outre, on a $[M : S] = [M^*: S^*]$ pour tout A-module simple S.

Soit M un A-module de type fini.

D’après la prop. 4 de VIII, p. 134, le A-module M est projectif de type fini ; il est donc réflexif d’après le cor. 4 de II, p. 47. En particulier, tout A-module simple est réflexif. Il en résulte également que deux modules à gauche de type fini sont isomorphes si et seulement si leurs duaux le sont.

Soit S un A-module à gauche simple. Soit $(T_i)_{i\in I}$ une famille de A-modules à droite simples, dont le dual $S^*$ de S soit somme directe. Comme S est réflexif, il est isomorphe à $(S^*)^*$ donc à $\prod_{i\in I}T^*_i$. Chacun des modules $T_i$ est réflexif ; en particulier, on a $T^*_i\not= 0$ pour tout $i\in I$. Comme le module simple S est isomorphe à $\prod_{i\in I}T^*_i$, l’ensemble I a un seul élément, donc $S^*$ est simple.

Comme M est semi-simple et de type fini, il est somme directe de sous-modules simples $S_1, . . . ,S_r$. Alors $M^*$ est isomorphe à la somme directe de la famille $S^*_1, . . . ,S^*_r$, et l’on vient de voir que les modules $S^*_i$ sont simples. L’assertion c) en résulte aussitôt.

### 3. Facteurs d’un anneau semi-simple

Dans ce numéro, on considère un anneau semi-simple A.

On note $\mathscr{S}$ l’ensemble des classes de A-modules à gauche simples (VIII, p. 47) ; il est fini (VIII, p. 132, prop. 1). Pour tout $\lambda \in \mathscr{S}$, on choisit un A-module simple $S_{\lambda}$ de classe $\lambda$; on note $\mathfrak{b}_{\lambda}$ son annulateur et $D_{\lambda}$ le corps opposé de son commutant End$_A(S_{\lambda})$.

#### Proposition 8 {#alg-viii-s8-prop-8 .statement tag=009F}

a) Pour tout $\lambda \in \mathscr{S}, S_{\lambda}$ est un espace vectoriel à droite de dimension finie sur le corps $D_{\lambda}$. L’application $a\rightarrow a_{S_{\lambda}}$ définit par passage au quotient un isomorphisme d’anneaux de $A/\mathfrak{b}_{\lambda}$ sur End$_{D_{\lambda}}(S_{\lambda})$.

b) Pour tout $\lambda \in \mathscr{S}$, l’anneau $A/\mathfrak{b}_{\lambda}$ est simple et l’homomorphisme canonique $\psi$ de A sur $\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$ est un isomorphisme d’anneaux.

L’anneau $A/\mathfrak{b}_{\lambda}$ est isomorphe à $A_{S_{\lambda}}$. Par le lemme 1 de VIII, p. 135, cet anneau est simple. L’application considérée de $A/\mathfrak{b}_{\lambda}$ dans End$_{D_{\lambda}}(S_{\lambda})$ s’identifie à l’application de $A_{S_{\lambda}}$ dans $A''_{S_{\lambda}}$. Par la prop. 5 de VIII, p. 135, c’est un isomorphisme.

Le A-module $A_s$ est semi-simple, fidèle et équilibré. L’homomorphisme $\psi$ s’identifie au morphisme du bicommutant de $A_s$ sur $\prod_{\lambda\in\mathscr{S}}$ End$_{D_{\lambda}}(S_{\lambda})$ qui est un isomorphisme (VIII, p. 81, prop. 7, c)).

L’anneau simple $A/\mathfrak{b}_{\lambda}$ est appelé le facteur simple de type $\lambda$ de A.

#### Exemple {#alg-viii-s8-n3-exa-1 .statement tag=009G}

Soit K un corps commutatif algébriquement clos et soit A une algèbre semi-simple de degré fini sur K. Soit $(V_i)_{i\in I}$ une famille de A-modules simples telle que tout A-module simple soit isomorphe à l’un des $V_i$ et un seul. Alors I est un ensemble fini (VIII, p. 132, prop. 1), les espaces vectoriels $V_i$ sont de dimension finie sur le corps K, le commutant de $V_i$ est égal à $K\cdot 1_{V_i}$ (VIII, p. 43, th. 1), et l’application $a\rightarrow (a_{V_i})_{i\in I}$ est un isomorphisme d’algèbres de A sur $\prod_{i\in I}$ End$_K(V_i)$ (prop. 8).

On a défini (VIII, p. 46) un idéal bilatère minimal comme un élément minimal de l’ensemble des idéaux bilatères non nuls, ordonné par inclusion. Autrement dit, un idéal bilatère minimal $\mathfrak{a}$ de A est un sous-(A, A)-bimodule simple de $_sA_d$. De manière analogue, on définit un idéal bilatère maximal de A comme un élément maximal de l’ensemble des idéaux bilatères distincts de A ; un idéal bilatère maximal $\mathfrak{a}$ de A n’est autre qu’un sous-(A, A)-bimodule maximal de $_sA_d$ (VIII, p. 44, définition 2). Si l’anneau A est simple, l’idéal 0 en est un idéal bilatère maximal et A un idéal bilatère minimal.

Pour tout $\lambda \in \mathscr{S}$, on note $\mathfrak{a}_{\lambda}$ le composant isotypique de type $\lambda$ du A-module $A_s$. Pour toute partie Λ de $\mathscr{S}$, posons $\mathfrak{a}_{\Lambda}=\sum_{\lambda\in\Lambda}\mathfrak{a}_{\lambda}$.

#### Proposition 9 {#alg-viii-s8-prop-9 .statement tag=009H}

a) Ordonnons par inclusion l’ensemble $\mathfrak{P}(\mathscr{S})$des parties de $\mathscr{S}$ et l’ensemble $\mathscr{B}_A$ des idéaux bilatères de A. L’application $\Lambda \rightarrow \mathfrak{a}_{\Lambda}$ est un isomorphisme d’ensembles ordonnés de $\mathfrak{P}(\mathscr{S})$sur $\mathscr{B}_A$.

b) Les idéaux bilatères minimaux de A sont les idéaux $\mathfrak{a}_{\lambda}$.

c) Pour tout $\lambda \in \mathscr{S}$, on a $\mathfrak{b}_{\lambda}=\mathfrak{a}_{\mathscr{S}-\{\lambda\}}$, et les idéaux $\mathfrak{b}_{\lambda}$ sont les idéaux bilatères maximaux de A.

d) Pour tout $\lambda \in \mathscr{S}$, l’application canonique de A sur $A/\mathfrak{b}_{\lambda}$ induit un isomorphisme de A-modules de $\mathfrak{a}_{\lambda}$ sur $A/\mathfrak{b}_{\lambda}$.

L’assertion a) résulte de la prop. 8, d) de VIII, p. 82 appliquée au A-module $A_s$. Il en résulte que les idéaux bilatères minimaux de A sont les $\mathfrak{a}_{\lambda}$ et que les idéaux bilatères maximaux sont les idéaux $\mathfrak{c}_{\lambda}=a_{\mathscr{S}-\lambda}$ (pour $\lambda \in \mathscr{S}$).

Il reste à établir, pour tout $\lambda \in \mathscr{S}$, l’égalité de $\mathfrak{b}_{\lambda}$ et $\mathfrak{c}_{\lambda}$. Soient $\lambda$ et $\mu$ distincts dans $\mathscr{S}$. Le sous-A-module $\mathfrak{a}_{\mu}S_{\lambda}$ de $S_{\lambda}$ est réunion des images des applications linéaires $a\rightarrow ax$ de $\mathfrak{a}_{\mu}$ dans $S_{\lambda}$, pour $x\in S_{\lambda}$. Par suite il est nul et l’on a $\mathfrak{a}_{\mu}\subset \mathfrak{b}_{\lambda}$. On en déduit $\mathfrak{c}_{\lambda}\subset \mathfrak{b}_{\lambda}$ et finalement $\mathfrak{c}_{\lambda}=\mathfrak{b}_{\lambda}$ puisque $\mathfrak{c}_{\lambda}$ est un idéal bilatère maximal de A et que $\mathfrak{b}_{\lambda}$ est distinct de A.

#### Corollaire {#alg-viii-s8-n3-cor-1 .statement tag=009I}

Soient $(A_i)_{i\in I}$ une famille finie d’anneaux simples et $f$ un isomorphisme de A sur $\prod_{i\in I}A_i$. Pour tout $i\in I$, il existe un unique élément $\varphi (i)$de $\mathscr{S}$ tel que le noyau de pr$_i\circ f$ soit $\mathfrak{b}_{\varphi(i)}$. L’application $\varphi$ est une bijection de I sur $\mathscr{S}$;pour tout $i\in I$, l’application pr$_i\circ f$ induit un isomorphisme $f_i$ de $A/\mathfrak{b}_{\varphi(i)}$ sur $A_i$.

Ainsi $f$ est composé de l’isomorphisme canonique de A sur $\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$ et de l’isomorphisme de $\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$ sur $\prod_{i\in I}A_i$ déduit des $f_i($« unicité de la décomposition d’un anneau semi-simple en produit d’anneaux simples »).

Démontrons le corollaire. Soit $i\in I$; notons $\mathfrak{b}'_i$ le noyau de pr$_i\circ f$. Comme l’anneau simple $A_i$ est isomorphe à $A/\mathfrak{b}'_i$, l’idéal bilatère $\mathfrak{b}'_i$ de A est maximal. D’après la prop. 8, c), il existe donc un unique élément $\varphi (i)$ de $\mathscr{S}$ tel que l’on ait $\mathfrak{b}'_i=\mathfrak{b}_{\varphi(i)}$. Alors pr$_i\circ f$ définit par passage au quotient un isomorphisme $f_i$ de $A/\mathfrak{b}_{\varphi(i)}$ sur $A_i$. Par ailleurs, on a $\mathfrak{b}'_i+\mathfrak{b}'_j= A$ si $i\not=j$ et $\cap_{i\in I}\mathfrak{b}'_i= 0 ($cf. I, p. 105, prop. 10). Il résulte de là et de la prop. 8, que $\varphi$ est une bijection de I sur $\mathscr{S}$.

#### Proposition 10 {#alg-viii-s8-prop-10 .statement tag=009J}

Notons Z le centre de A ; pour tout $\lambda \in \mathscr{S}$, soit $Z_{\lambda}$ le centre du corps $D_{\lambda}$.

a) L’application $z\rightarrow (z_{S_{\lambda}})_{\lambda\in\mathscr{S}}$ est un isomorphisme de l’anneau Z sur le produit $\prod_{\lambda\in\mathscr{S}}Z_{\lambda}$.

b) Ordonnons par inclusion l’ensemble $\mathscr{I}_Z$ des idéaux de Z et l’ensemble $\mathscr{B}_A$ des idéaux bilatères de A. L’application $\mathfrak{a}\rightarrow \mathfrak{a}A$est un isomorphisme d’ensembles ordonnés de $\mathscr{I}_Z$ sur $\mathscr{B}_A$. L’isomorphisme réciproque associe à un idéal bilatère $\mathfrak{b}$ de A l’idéal $\mathfrak{b}\cap Z$de Z.

Cette proposition résulte de la prop. 8 de VIII, p. 82 appliquée au A-module $A_s$, dont le bicommutant est A.

#### Corollaire {#alg-viii-s8-n3-cor-2 .statement tag=009K}

Soit B un anneau. Les conditions suivantes sont équivalentes :

(i) L’anneau B est simple ;

(ii) L’anneau B est semi-simple et son centre est un corps ;

(iii) L’anneau B est semi-simple et il existe une seule classe de B-modules simples.

#### Proposition 11 {#alg-viii-s8-prop-11 .statement tag=009L}

Soit $\lambda \in \mathscr{S}$. Le composant isotypique $\mathfrak{a}_{\lambda}$ de A est à la fois le composant isotypique de type $S_{\lambda}$ de $A_s$ et le composant isotypique de type $S^*_{\lambda}$ de $A_d$. De plus, on a

(1) $[A_s: S_{\lambda}] = [A_d: S^*_{\lambda}] =$ dim$_{D_{\lambda}}S_{\lambda}$

et

(2) long(A) = long(A$^o$) $=\sum_{\lambda\in\mathscr{S}}$ dim$_{D_{\lambda}}S_{\lambda}$.

La première assertion est le cas particulier $M = A_s$ de la prop. 6, c) de VIII, p. 135. L’égalité $[A_s: S_{\lambda}] = [A_d: S^*_{\lambda}]$ résulte de la prop. 7 de VIII, p. 136, puisque le dual du A-module à gauche $A_s$ est isomorphe au A-module à droite $A_d$. D’après les prop. 8, a) de VIII, p. 137 et 9, c) de VIII, p. 137, l’application $a\rightarrow a_{S_{\lambda}}$ définit un isomorphisme de A-modules à gauche de $\mathfrak{a}_{\lambda}$ sur End$_{D_{\lambda}}(S_{\lambda})$. Comme $[A_s: S_{\lambda}]$ est, par définition, la longueur du A-module à gauche $\mathfrak{a}_{\lambda}$, la relation $[A_s: S_{\lambda}] =$ dim$_{D_{\lambda}}S_{\lambda}$ résulte du lemme 2 de VIII, p. 117. Enfin, la formule (2) s’obtient à partir de (1) par sommation sur $\lambda$.

#### Scholie {#alg-viii-s8-n3-sch-1 .statement tag=009M}

Soient A un anneau semi-simple et Z son centre. Il existe des bijections canoniques entre les ensembles suivants :

a) l’ensemble $\mathscr{S}(A)$des classes de A-modules à gauche simples ;

b) l’ensemble $\mathscr{S}(A^o)$des classes de A-modules à droite simples ;

c) l’ensemble des idéaux bilatères minimaux de A ;

d) l’ensemble des idéaux bilatères maximaux de A ;

e) l’ensemble $\mathscr{S}(Z)$des classes de Z-modules simples ;

f) l’ensemble des idéaux minimaux de Z ;

g) l’ensemble des idéaux maximaux de Z.

À tout élément $\lambda$ de $\mathscr{S}(A)$ correspondent ainsi la classe $\lambda^*$ du A-module à droite simple $S^*_{\lambda}$ dual de $S_{\lambda}$, l’idéal bilatère minimal $\mathfrak{a}_{\lambda}$ (composant isotypique de type $\lambda$ de $A_s$), l’idéal bilatère maximal $\mathfrak{b}_{\lambda}$ de A (annulateur du module simple $S_{\lambda}$), la classe du Z-module simple $Z\cap \mathfrak{a}_{\lambda}$, l’idéal minimal $Z\cap \mathfrak{a}_{\lambda}$ de Z et l’idéal maximal $Z\cap \mathfrak{b}_{\lambda}$ de Z.

#### Proposition 12 {#alg-viii-s8-prop-12 .statement tag=009N}

Soient M un module sur l’anneau semi-simple A et $\mathscr{S}_M\subset \mathscr{S}$ le support de M. Alors l’annulateur Ann(M) de M est l’idéal bilatère $\sum_{\lambda\in\mathscr{S}-\mathscr{S}_M}\mathfrak{a}_{\lambda}$ et l’idéal trace $\tau (M)$de M est l’idéal bilatère $\sum_{\lambda\in\mathscr{S}_M}\mathfrak{a}_{\lambda}$. En particulier, A est somme directe de Ann(M) et $\tau (M)$.

Par définition (VIII, p. 80)$,\mathscr{S}_M$ se compose des classes des sous-modules simples de M. Comme le module M est semi-simple, l’annulateur de M est l’intersection des annulateurs $\mathfrak{b}_{\lambda}$ des modules de classe $\lambda$, pour $\lambda$ parcourant$\mathscr{S}_M$. Or on a $\mathfrak{b}_{\lambda}=\sum_{\mu\not=\lambda}\mathfrak{a}_{\mu}$ pour tout $\lambda \in \mathscr{S}$ (VIII, p. 137, prop. 9). Comme A est somme directe de la famille $(\mathfrak{a}_{\lambda})_{\lambda\in\mathscr{S}}$, l’annulateur de M est bien égal à $\sum_{\lambda\in\mathscr{S}-\mathscr{S}_M}\mathfrak{a}_{\lambda}$.

Par définition (VIII, p. 75), l’idéal trace $\tau (M)$ est le sous-A-module de $A_s$ engendré par les images des applications A-linéaires de M dans $A_s$. Il revient au même, puisque M est semi-simple, de dire que $\tau (M)$ est engendré par les sous-modules simples de $A_s$ dont la classe appartient à $\mathscr{S}_M$. On a donc $\tau (M) =\sum_{\lambda\in\mathscr{S}_M}\mathfrak{a}_{\lambda}$.

#### Corollaire {#alg-viii-s8-n3-cor-3 .statement tag=009O}

Soit M un module sur l’anneau semi-simple A. Les propriétés suivantes sont équivalentes :

(i) Le A-module M est fidèle ;

(ii) Le support de M est égal à $\mathscr{S}$;

(iii) Le A-module M est générateur.

En effet, dire que M est fidèle signifie que son annulateur est réduit à 0, et M est générateur si et seulement si sa trace est égale à A (VIII, p. 76, th. 1).

### 4. Idempotents et anneaux semi-simples

Soit A un anneau. Rappelons qu’un élément $e$ de A est dit idempotent (I, p. 7) si l’on a $e^2=e$; c’est alors également un élément idempotent de l’anneau $A^o$ opposé de A.

#### Proposition 13 {#alg-viii-s8-prop-13 .statement tag=009P}

a) Pour qu’un idéal à gauche $\mathfrak{a}$ de A admette un supplémentaire dans $A_s$, il faut et il suffit qu’il existe un élément idempotent $e$ de A tel que $\mathfrak{a}= Ae$. L’idéal $\mathfrak{a}$ se compose alors des éléments $x$ de A tels que $x=xe$.

b) Soient $e$ et $f$ des éléments idempotents de A. On a $Ae\subset Af$ si et seulement si l’on a la relation $ef=e$.

c) Soit M un A-module. Pour que M soit projectif et monogène, il faut et il suffit qu’il existe un élément idempotent $e$ de A tel que M soit isomorphe à $Ae$.

Les endomorphismes du A-module $A_s$ sont les multiplications à droite par les éléments de A ; les projecteurs dans le A-module $A_s$ sont donc les applications $x\rightarrow xe$ où $e$ est idempotent dans A. De plus, les sous-modules de $A_s$ sont les idéaux à gauche, et un tel sous-module admet un supplémentaire si et seulement s’il est l’image d’un projecteur (II, p. 20, prop. 14). L’assertion a) résulte de là.

La relation $Ae\subset Af$ équivaut à $e\in Af$; d’après a), elle équivaut donc à $e=ef$, d’où b).

Si le A-module M est monogène, il existe une application A-linéaire surjective $u: A_s\rightarrow M$; si de plus M est projectif, il existe un sous-module $\mathfrak{a}$ de $A_s$, supplémentaire du noyau de $u$. Alors $u$ induit un isomorphisme de $\mathfrak{a}$ sur M. Inversement, si M est isomorphe à un sous-module facteur direct de $A_s$, il est monogène et projectif. L’assertion c) résulte donc de a).

#### Remarque 1 {#alg-viii-s8-n4-rem-1 .statement tag=009Q}

Soit $\mathfrak{a}$ un idéal à gauche de A. D’après la démonstration ci-dessus et le corollaire de II, p. 19, l’application $e\rightarrow A(1-e)$ définit une bijection de l’ensemble des éléments idempotents $e$ de A tels que $\mathfrak{a}= Ae$ sur l’ensemble des idéaux à gauche $\mathfrak{b}$ de A tels que $A_s=\mathfrak{a}\oplus \mathfrak{b}$.

#### Remarque 2 {#alg-viii-s8-n4-rem-2 .statement tag=009R}

Soient $e$ et $f$ des éléments idempotents de A. D’après la prop. 13 b), on a $Ae= Af$ si et seulement si l’on a $ef=e$ et $f e=f$. Par conséquent, si l’anneau A est commutatif, la relation $Ae= Af$ équivaut à $e=f$. Il n’en est pas de même en général, comme le montre l’exemple $A = \mathbf{M}_2(\mathbf{Z}), e = \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix}$ et $f = \begin{pmatrix} 1 & 0 \\ 1 & 0 \end{pmatrix}$.

On dit que des éléments idempotents $e$ et $e'$ de l’anneau A sont orthogonaux si l’on a $ee'=e'e= 0$. Soit $(e_i)_{i\in I}$ une famille finie d’éléments idempotents de A, deux à deux orthogonaux. Comme on a

$$
(\sum_ie_i)^2=\sum_ie^2_i+\sum_{i\not=j}e_ie_j=\sum_ie_i
$$

l’élément $\sum_{i\in I}e_i$ de A est idempotent.

On appelle partition d’un élément idempotent $e$ de A toute famille finie $(e_i)_{i\in I}$ d’éléments idempotents de A, deux à deux orthogonaux, telle que $e=\sum_{i\in I}e_i$. On dit qu’un élément idempotent $e$ de A est décomposable s’il existe une partition de $e$ formée d’éléments idempotents distincts de 0 et de lui-même, deux à deux orthogonaux ; dans le cas contraire, on dit qu’il est indécomposable. On observera que 0 est un élément idempotent décomposable.

#### Proposition 14 {#alg-viii-s8-prop-14 .statement tag=009S}

Soit $e$ un élément idempotent de A.

a) Si $(e_i)_{i\in I}$ est une partition de $e$, le A-module $Ae$ est somme directe de la famille $(Ae_i)_{i\in I}$.

b) Soit $(\mathfrak{a}_i)_{i\in I}$ une famille finie d’idéaux à gauche de A, dont $Ae$ soit somme directe ; pour $i\in I$, notons $e_i$ le composant de $e$ dans $\mathfrak{a}_i$. Alors $(e_i)_{i\in I}$ est une partition de $e$ et l’on a $\mathfrak{a}_i= Ae_i$ pour tout $i\in I$.

c) Le A-module $Ae$ est indécomposable si et seulement si l’élément idempotent $e$ est indécomposable.

Soit $(e_i)_{i\in I}$ une partition de $e$. Pour tout $i\in I$, on a

$$
e_ie=\sum_je_ie_j=e^2_i+\sum_{j\not=i}e_ie_j=e_i
$$

d’où $Ae_i\subset Ae$. Pour tout $i\in I$, on définit un projecteur A-linéaire $p_i$ dans $Ae$ en posant $p_i(x) =xe_i$. On a $p_ip_j= 0$ si $i\not=j$, et pour tout $x$ dans $Ae$

$$
x=xe=\sum_ixe_i=\sum_ip_i(x)
$$

Par suite (II, p. 18, prop. $12$)$, Ae$ est somme directe des images des $p_i$. Or on a $ee_i=e_ie=e_i$, donc l’image de $p_i$ est $Ae_i$. Cela prouve a).

Prenons les notations et hypothèses de b). Soit $i\in I$; comme $e_i$ appartient à $Ae$, on a $e_i=e_ie=\sum_je_ie_j$; comme $Ae$ est somme directe des $\mathfrak{a}_j$ et que $e_ie_j$ appartient à $\mathfrak{a}_j$ pour tout $j$, on a $e_i=e_ie_i$ et $e_ie_j= 0$ pour $i\not=j$. Autrement dit, $(e_i)_{i\in I}$ est une partition de l’élément idempotent $e$. D’après a), $Ae$ est somme directe des $Ae_i$; par hypothèse, on a $Ae_i\subset \mathfrak{a}_i$ et $Ae$ est somme directe des $\mathfrak{a}_i$. On a donc $Ae_i=\mathfrak{a}_i$ pour tout $i\in I$, d’où b).

Enfin, c) résulte aussitôt de a) et b).

#### Remarque 3 {#alg-viii-s8-n4-rem-3 .statement tag=00R8}

En appliquant les résultats précédents à l’anneau opposé de A, on voit en particulier qu’un A-module à droite monogène M est projectif si et seulement s’il existe un élément idempotent $e$ dans A tel que M soit isomorphe à $eA$; de plus, $eA$ est un module à droite indécomposable si et seulement si $e$ est indécomposable.

Supposons maintenant l’anneau A semi-simple et notons $\mathscr{S}$ l’ensemble des classes de A-modules à gauche simples. Le A-module $A_s$ est semi-simple et tout sous-module de $A_s$ est facteur direct. Soit $\mathfrak{a}$ un idéal à gauche de A ; d’après ce qui précède, il existe un élément idempotent $e$ de A tel que $\mathfrak{a}= Ae$, et le A-module $\mathfrak{a}$ est simple si et seulement s’il est indécomposable, c’est-à-dire si et seulement si $e$ est indécomposable.

Soit $(\mathfrak{m}_i)_{i\in I}$ une famille d’idéaux à gauche minimaux de A, telle que l’on ait $A_s=\oplus_{i\in I}\mathfrak{m}_i$. D’après la prop. 14 (VIII, p. 141), il existe une partition $(\varepsilon_i)_{i\in I}$ de 1, formée d’éléments idempotents indécomposables et telle que $\mathfrak{m}_i= A\varepsilon_i$ pour tout $i\in I$.

Pour tout $\lambda \in \mathscr{S}$, notons $S_{\lambda}$ un A-module de classe $\lambda$ et $\mathfrak{a}_{\lambda}$ le composant isotypique de type $\lambda$ du A-module $A_s$. Comme A est somme directe de la famille $(\mathfrak{a}_{\lambda})_{\lambda\in\mathscr{S}}$, il existe une partition $(e_{\lambda})_{\lambda\in\mathscr{S}}$ de 1 telle que $\mathfrak{a}_{\lambda}= Ae_{\lambda}$ pour tout $\lambda \in \mathscr{S}$. Pour $\lambda \in \mathscr{S}$, notons $I(\lambda )$ l’ensemble des indices $i\in I$ tels que le A-module simple $\mathfrak{m}_i$ soit de type $\lambda$; d’après la prop. 4, b) de VIII, p. 61, on a

$$
\mathfrak{a}_{\lambda}=\bigoplus_{i\in I(\lambda)}\mathfrak{m}_i \tag{3}
$$

L’élément idempotent $e_{\lambda}$ est la composante de 1 dans $\mathfrak{a}_{\lambda}$, donc $e_{\lambda}=\sum_{i\in I(\lambda)}\varepsilon_i$.

#### Proposition 15 {#alg-viii-s8-prop-15 .statement tag=009T}

Supposons l’anneau A semi-simple.

a) Pour tout $\lambda \in \mathscr{S},e_{\lambda}$ est l’unique élément du centre Z de A satisfaisant à la relation $(e_{\lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$ et $(e_{\lambda})_{S_{\mu}}= 0$pour $\mu \not=\lambda$.

b) Les idempotents indécomposables de l’anneau Z sont les $e_{\lambda}$, et les idéaux minimaux de Z sont les $Ze_{\lambda}$ pour $\lambda \in \mathscr{S}$.

c) Soient M un A-module et $(M_{\lambda})_{\lambda\in\mathscr{S}}$ la famille de ses composants isotypiques. La famille de projecteurs associée à la décomposition de M en somme directe des $M_{\lambda}$ (VIII, p. 61) est $((e_{\lambda})_M)_{\lambda\in\mathscr{S}}$ et l’on a $M_{\lambda}=\mathfrak{a}_{\lambda}M$pour tout $\lambda \in \mathscr{S}$.

Soient $\lambda$ et $\mu$ distincts dans $\mathscr{S}$. On a $e_{\lambda}\in \mathfrak{a}_{\lambda}$ et $\mathfrak{a}_{\lambda}$ est contenu dans l’annulateur $\mathfrak{b}_{\mu}$ du A-module $S_{\mu}$ (VIII, p. 137, prop. 9) ; on a donc $(e_{\lambda})_{S_{\mu}}= 0$. La relation $(e_{\lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$ résulte de là puisqu’on a $1 =\sum_{\nu\in\mathscr{S}}e_{\nu}$. L’assertion a) découle alors de la prop. 8 de VIII, p. 137.

Soit $\lambda$ dans $\mathscr{S}$. L’idéal bilatère $\mathfrak{a}_{\lambda}$ de A se compose des éléments $x$ tels que $x=xe_{\lambda}$; on a donc $Z\cap \mathfrak{a}_{\lambda}= Ze_{\lambda}$, d’où b) d’après la prop. 10, b) de VIII, p. 138.

Prouvons c). Soit $x$ un élément de M. Pour tout $\lambda \in \mathscr{S}$, on a $e_{\lambda}\in \mathfrak{a}_{\lambda}$; comme l’application $a\rightarrow ax$ de $A_s$ dans M est A-linéaire, on a $\mathfrak{a}_{\lambda}x\subset M_{\lambda}$ (VIII, p. 62, prop. 5) et en particulier $e_{\lambda}x\in M_{\lambda}$. On a $1 =\sum_{\lambda\in\mathscr{S}}e_{\lambda}$, d’où $x=\sum_{\lambda\in\mathscr{S}}e_{\lambda}x$; par suite, $e_{\lambda}x$ est la composante de $x$ dans $M_{\lambda}$.

#### Remarque 4 {#alg-viii-s8-n4-rem-4 .statement tag=009U}

Supposons l’anneau A semi-simple. Soit $(e_i)_{i\in I}$ une partition de 1, formée d’éléments idempotents non nuls du centre Z de A ; si Card(I) = Card($\mathscr{S}$), les $e_i$ sont les idempotents indécomposables de Z.

## EXERCICES {#alg-viii-s8-exercises}

See the [exercises for § 8](exercises/s8/).
