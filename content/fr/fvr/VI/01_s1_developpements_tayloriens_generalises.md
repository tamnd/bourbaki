---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: DÉVELOPPEMENTS TAYLORIENS GÉNÉRALISÉS. FORMULE SOMMATOIRE D’EULER–MACLAURIN
section: 1
section_title: Développements tayloriens généralisés
lang: fr
source: fvr-i-vii-fr
pdf_pages: 0261-0275, 0282-0282
extraction: ocr
subsections:
    - "no": 1
      title: Opérateurs de composition dans une algèbre de polynômes
      page: 0
      pdf_page: 261
    - "no": 2
      title: Polynômes d’Appell attachés à un opérateur de composition
      page: 5
      pdf_page: 265
    - "no": 3
      title: Série génératrice des polynômes d’Appell
      page: 6
      pdf_page: 266
    - "no": 4
      title: Polynômes de Bernoulli
      page: 7
      pdf_page: 267
    - "no": 5
      title: Opérateurs de composition sur les fonctions d’une variable réelle
      page: 9
      pdf_page: 269
    - "no": 6
      title: Indicatrice d’un opérateur de composition
      page: 10
      pdf_page: 270
    - "no": 7
      title: La formule sommatoire d’Euler-Maclaurin
      page: 14
      pdf_page: 274
statements: 22
exercises: 3
content_sha256: 1c3e00ab266cbc56b3245739da74a342e47944ab91c846c5650f7ce7098a4940
---

## § 1. DÉVELOPPEMENTS TAYLORIENS GÉNÉRALISÉS

### 1. Opérateurs de composition dans une algèbre de polynômes

Soient K un corps commutatif de caractéristique 0, K[X] l’algèbre des polynômes à une indéterminée sur K (A, IV, § 1, n° 1); dans tout ce paragraphe, nous désignerons sous le nom d’opérateur dans K[X] toute application linéaire U de l’espace vectoriel K[X] (par rapport à K) dans lui-même; comme les monômes X^n (n ≥ 0) forment une base de cet espace, U est déterminé par la donnée des polynômes U(X^n); de façon précise, si f(X) = $\sum_{k=0}^{\infty} \lambda_k X^k$ avec $\lambda_k \in K$, on a
$$ U(f) = \sum_{k=0}^{\infty} \lambda_k U(X^k). $$

Si G est une algèbre commutative sur K, ayant un élément unité, le G-module G[X] s’obtient par extension à G du corps des scalaires K de l’espace vectoriel K[X]; tout opérateur U dans K[X] se prolonge donc d’une seule manière en une application linéaire du G-module G[X] dans lui-même, que nous noterons encore U (A, II, p. 82); pour tout élément g(X) = $\sum_{k=0}^{\infty} \gamma_k X^k$, avec $\gamma_k \in G$, on a $U(g) = \sum_{k=0}^{\infty} \gamma_k U(X^k)$.

Considérons en particulier le cas où G = K[Y]; G[X] est donc l’anneau K[X, Y] des polynômes à deux indéterminées sur K; pour éviter toute confusion, on notera $U_X$ le prolongement de U à G[X]. Pour tout polynôme $g(X, Y) = \sum_{k=0}^{\infty} \gamma_k(Y) X^k$, où $\gamma_k(Y) \in K[Y]$ on a donc $U_X(g) = \sum_{k=0}^{\infty} \gamma_k(Y) U(X^k)$. Comme $U_X$ est linéaire, on voit que si on écrit $g(X, Y) = \sum_{h=0}^{\infty} \beta_h(X) Y^h$, on a aussi
$$ U_X(g) = \sum_{h=0}^{\infty} U(\beta_h) Y^h. $$

Par l’isomorphisme canonique de K[X] sur K[Y] qui à X fait correspondre Y, l’opérateur U se transforme en un opérateur dans K[Y] que nous noterons $U_Y$ pour éviter toute confusion, $U_Y(f(Y))$ étant donc le polynôme obtenu en remplaçant X par Y dans le polynôme $U(f(X)) = U_X(f(X))$. Cet opérateur $U_Y$ peut à son tour être prolongé en un opérateur (noté encore $U_Y$) dans K[X, Y]:

si $g(X, Y) = \sum_{h=0}^\infty \beta_h(X)Y^h$, on a donc ici $U_Y(g(X, Y)) = \sum_{h=0}^\infty \beta_h(X)\ U_Y(Y^h)$.

Comme exemple de ces prolongements, citons l’opérateur de *dérivation* D dans K[X] (A, IV, § 4), qui donne dans K[X, Y] les opérateurs de dérivation partielle $D_X$ et $D_Y$.

Pour tout polynôme $f \in K[X]$, nous désignerons par $T_Y(f)$ le polynôme $f(X + Y)$ de K[X, Y]; l’application $T_Y$ est une application K-linéaire de K[X] dans K[X, Y], dite *opérateur de translation*.

#### Définition 1 {#fvr-vi-s1-def-1 .statement}

*On dit qu’un opérateur U dans K[X] est un opérateur de composition s’il est permutable avec l’opérateur de translation, c’est-à-dire si $U_X T_Y = T_Y U$.*

En d’autres termes, si $f$ est un polynôme quelconque de K[X], et si $g = U(f)$, on doit avoir $g(X + Y) = V_X(f(X + Y))$.

Il résulte aussitôt de cette définition que, pour tout polynôme $f(X) \in K[X]$, on a, avec les notations introduites ci-dessus,

$$
U_X(f(X + Y)) = U_Y(f(X + Y)).
$$

#### Exemple 1 {#fvr-vi-s1-n1-exa-1 .statement}

Pour tout $\lambda \in K$, l’opérateur qui, à tout polynôme $f(X)$, fait correspondre le polynôme $f(X + \lambda)$, est un opérateur de composition.

#### Exemple 2 {#fvr-vi-s1-n1-exa-2 .statement}

La *dérivation* D dans K[X] est un opérateur de composition (cf. prop. 1).

#### Remarque {#fvr-vi-s1-n1-rem-1 .statement}

Comme K est un corps infini, pour que l’opérateur U dans K[X] soit un opérateur de composition, il faut et il suffit que pour tout polynôme $f \in K[X]$ et tout élément $\alpha \in K$, on ait, en posant $g = U(f)$, $g(X + \alpha) = U(f(X + \alpha))$. (A, IV, § 2, n° 4).

Il est clair que toute combinaison linéaire d’opérateurs de composition, à coefficients dans K, est un opérateur de composition; il en est de même du composé de deux opérateurs de composition. En d’autres termes, les opérateurs de composition forment une *sous-algèbre* $\Gamma$ de l’algèbre des endomorphismes de l’espace vectoriel K[X].

#### Proposition 1 {#fvr-vi-s1-prop-1 .statement}

*Pour qu’un opérateur U dans K[X] soit un opérateur de composition il faut et il suffit qu’il soit permutable avec la dérivation D dans K[X].*

En effet, la formule de Taylor montre que, pour tout polynôme $f \in K[X]$, on a

$$
U_X(f(X + Y)) = U_X \left( \sum_{k=0}^\infty \frac{1}{k!}\ Y^k D^k f(X) \right) = \sum_{k=0}^\infty \frac{1}{k!}\ Y^k U(D^k f(X));
$$

si on pose $g = U(f)$, on a

$$
g(X + Y) = \sum_{k=0}^\infty \frac{1}{k!}\ Y^k D^k g(X) = \sum_{k=0}^\infty \frac{1}{k!}\ Y^k D^k(U(f(X)));
$$

pour que $U$ soit un opérateur de composition, on doit donc avoir $UD^k = D^kU$ pour tout entier $k \geqslant 1$, et en particulier $UD = DU$. Inversement, si cette relation est vérifiée, elle entraîne $UD^k = D^kU$ pour tout entier $k \geqslant 1$, par récurrence sur $k$; la formule de Taylor montre alors que $g(X + Y) = U_x(f(X + Y))$.

Pour tout polynôme $f \in K[X, Y]$, nous désignerons par $U_0(f)$ le terme indépendant de $X$ dans le polynôme $U_X(f)$; en particulier, si $f \in K[X]$, $U_0(f)$ est le terme constant de $U(f)$, et $U_0$ est une forme linéaire sur $K[X]$. Pour tout polynôme $f \in K[X]$, soit $g = U(f)$; on a, en vertu de la déf. 1 de VI, p. 2,

$$
g(X + Y) = V_X(f(X + Y)) = U_X \left( \sum_{k=0}^{\infty} \frac{1}{k!} X^k D^k f(Y) \right) = \sum_{k=0}^{\infty} \frac{1}{k!} U(X^k) D^k f(Y)
$$

et si, dans cette formule, on remplace $X$ par 0, on obtient

$$
g(Y) = \sum_{k=0}^{\infty} \frac{1}{k!} U_0(X^k) D^k f(Y).
$$

On voit donc qu’on a

$$
U(f(X)) = \sum_{k=0}^{\infty} \frac{1}{k!} \mu_k D^k f(X)
$$

où $\mu_k$ est le terme constant du polynôme $U(X^k)$.

Cette formule montre que la donnée des $\mu_k$ détermine complètement l’opérateur de composition $U$; inversement, si $(\mu_n)$ est une suite arbitraire d’éléments de $K$, la formule (2) définit un opérateur $U$ qui est évidemment permutable avec $D$, et par suite (VI, p. 2, prop. 1) un opérateur de composition. Nous écrirons désormais la formule (2) sous la forme

$$
U = \sum_{k=0}^{\infty} \frac{1}{k!} \mu_k D^k.
$$

Cette formule peut s’interpréter en langage topologique de la façon suivante: si on considère sur $K[X]$ la topologie discrète, et sur l’algèbre $\mathrm{End}(K[X])$ des endomorphismes de $K[X]$, la topologie de la convergence simple dans $K[X]$ (TG, X, p. 4), la série de terme général $\frac{1}{k!} \mu_k D^k$ est commutativement convergente dans $\mathrm{End}(K[X])$ et a pour somme $U$ (TG, III, p. 44).

La formule (3) montre qu’à toute série formelle $u(S) = \sum_{k=0}^{\infty} \alpha_k S^k$ à une indéterminée sur $K$ (A, IV, § 5), on peut faire correspondre l’opérateur de composition $U = \sum_{k=0}^{\infty} \alpha_k D^k$, que nous noterons désormais $u(D)$. Cette remarque peut être précisée de la façon suivante:

#### Théorème 1 {#fvr-vi-s1-thm-1 .statement}

L’application qui, à toute série formelle $u(S) = \sum_{k=0}^\infty \alpha_k S^k$ à une indéterminée sur $K$, fait correspondre l’opérateur de composition $u(D) = \sum_{k=0}^\infty \alpha_k D^k$ dans $K[X]$, est un isomorphisme de l’algèbre $K[[S]]$ des séries formelles sur l’algèbre $\Gamma$ des opérateurs de composition.

On vérifie aussitôt que cette application est un homomorphisme. Tout revient donc à voir qu’elle est injective, autrement dit, que la relation $\sum_{k=0}^\infty \alpha_k D^k = 0$ entraîne $\alpha_k = 0$ pour tout $k$; or, $h! \alpha_h$ est le terme constant du polynôme obtenu en appliquant $\sum_{k=0}^\infty \alpha_k D^k$ à $X^h$, d’où le théorème.

#### Corollaire {#fvr-vi-s1-n1-cor-1 .statement}

L’algèbre $\Gamma$ des opérateurs de composition dans $K[X]$ est commutative.

#### Exemple {#fvr-vi-s1-n1-exa-3 .statement}

Si $U$ est l’opérateur qui, à tout polynôme $f(X)$, fait correspondre $f(X + \lambda)$ (où $\lambda \in K$), on a $U_0(X^k) = \lambda^k$, et par suite $U = \sum_{k=0}^\infty \frac{1}{k!} (\lambda D)^k$. Par analogie avec le développement en série de $e^x$ (III, p. 15), nous désignerons par $e^S$ ou $\exp(S)$ le série formelle $\sum_{n=0}^\infty \frac{1}{n!} S^n$ dans l’anneau $K[[S]]$; on peut donc écrire $U = e^{\lambda D}$. En remplaçant dans ce raisonnement le corps $K$ par le corps de fractions rationnelles $K(Y)$, on voit de même que l’opérateur de translation $T_Y$ peut s’écrire $e^{YD}$.

On notera d’ailleurs que, dans l’anneau $K[[S, T]]$ des séries formelles sur $K$ à deux indéterminées, on a

$$
(\exp S)(\exp T) = \sum_{p, q} \frac{S^p T^q}{p! q!}
$$
$$
= \sum_{n=0}^\infty \frac{1}{n!} \left( \binom{n}{0} S^n + \binom{n}{1} S^{n-1} T + \cdots + \binom{n}{n} T^n \right) = \exp (S + T)
$$

et en particulier

$$(\exp S)(\exp (-S)) = 1$$

ce qui justifie la notation introduite.

#### Scholie {#fvr-vi-s1-n1-sch-1 .statement}

L’isomorphie de l’algèbre $K[[S]]$ des séries formelles et de l’algèbre $\Gamma$ des opérateurs de composition dans $K[X]$, permet parfois de démontrer plus simplement des propositions relatives à des séries formelles, en les démontrant pour les opérateurs de composition qui leur correspondent (cf. VI, p. 6, prop. 6).

### 2. Polynômes d’Appell attachés à un opérateur de composition

Étant donné un opérateur de composition $U = \sum_{k=0}^{\infty} \alpha_k D^k \neq 0$, soit $p$ le plus petit des entiers $k$ tels que $\alpha_k \neq 0$; nous dirons que $p$ est l’ordre de l’opérateur $U$.

#### Proposition 2 {#fvr-vi-s1-prop-2 .statement}

*Tout opérateur de composition d’ordre 0 est inversible dans l’algèbre $\Gamma$ des opérateurs de composition dans $\mathbf{K}[X]$.*

En effet, une série formelle $\sum_{k=0}^{\infty} \alpha_k S^k$ telle que $\alpha_0 \neq 0$ est *inversible* dans l’anneau $\mathbf{K}[[S]]$ (A, IV, § 5); la proposition résulte donc du th. 1 de VI, p. 4.

#### Proposition 3 {#fvr-vi-s1-prop-3 .statement}

*Soit $U$ un opérateur de composition d’ordre $p$; pour tout polynôme $f$ de degré $< p$, $U(f) = 0$; pour tout polynôme $f \neq 0$ de degré $n \geq p$, $U(f)$ est un polynôme $\neq 0$ de degré $n - p$.*

C’est une conséquence immédiate de la formule (2) de VI, p. 2 et de la définition de l’ordre de $U$.

Il est clair que tout opérateur $U$ d’ordre $p$ peut s’écrire d’une seule manière $U = D^p V = V D^p$, où $V$ est un opérateur d’ordre 0 (donc inversible).

#### Définition 2 {#fvr-vi-s1-def-2 .statement}

*Soit $U = D^p V$ un opérateur de composition d’ordre $p$ dans $\mathbf{K}[X]$. On appelle polynôme d’Appell d’indice $n$ attaché à l’opérateur $U$ le polynôme $u_n(X) = V^{-1}(X^n)$.*

Si $V^{-1} = \sum_{k=0}^{\infty} \frac{1}{k!} \beta_k D^k$ (avec $\beta_0 \neq 0$) on a donc

$$
u_n(X) = \sum_{k=0}^{n} \binom{n}{k} \beta_k X^{n-k}.
$$

On vérifie ainsi que $u_n$ est un polynôme de degré $n$ (prop. 3); on a en outre

$$
u_n(0) = \beta_n.
$$

#### Proposition 4 {#fvr-vi-s1-prop-4 .statement}

*Les polynômes d’Appell attachés à $U$ satisfont aux relations*

$$
\frac{du_n}{dX} = n \cdot u_{n-1}
$$
$$
u_n(X + Y) = \sum_{k=0}^{n} \binom{n}{k} u_{n-k}(X) Y^k
$$
$$
U(u_n(X)) = \frac{n!}{(n-p)!} X^{n-p}.
$$

Ces formules sont en effet respectivement équivalentes aux relations suivantes (compte tenu de la déf. 2):

(10) $DV^{-1} = V^{-1}D$
(11) $(\exp(\mathrm{YD}_X))\ V_X^{-1} = V_X^{-1}\exp(\mathrm{YD}_X)$
(12) $UV^{-1} = D^p.$

#### Proposition 5 {#fvr-vi-s1-prop-5 .statement}

*Pour tout polynôme* $f \in \mathbf{K}[X]$ *et tout opérateur de composition U d’ordre p, on a*

$$
f^{(p)}(X + Y) = \sum_{k=0}^{\infty} \frac{1}{k!}\ U(f^{(k)}(X))u_k(Y)
$$

*(développement taylorien généralisé)*.

En effet, si on pose $U = D^pV = VD^p$, on a (VI, p. 2, formule (1))

$$
V_X^{-1}(f(X + Y)) = V_Y^{-1}(f(X + Y)) = \sum_{k=0}^{\infty} \frac{1}{k!}\ f^{(k)}(X)u_k(Y)
$$

en raison de la formule de Taylor et de la déf. 2 de VI, p. 5; il suffit d’appliquer l’opérateur $U_X$ aux deux membres extrêmes de la formule (14) pour obtenir (13).

### 3. Série génératrice des polynômes d’Appell

Soit E l’anneau des *séries formelles* à une indéterminée S, à coefficients dans l’anneau de polynômes $\mathbf{K}[X]$ (A, IV, § 5) autrement dit, l’anneau des séries formelles $g(X, S) = \sum_{n=0}^{\infty} \alpha_n(X)S^n$, où les $\alpha_n$ appartiennent à $\mathbf{K}[X]$. Pour tout opérateur U dans $\mathbf{K}[X]$, on définit une application $U_X$ de E dans lui-même en posant $U_X(g(X, S)) = \sum_{n=0}^{\infty} U(\alpha_n)S^n$. Il est clair que E est un module sur l’anneau $\mathbf{K}[[S]]$ des séries formelles en S à coefficients dans $\mathbf{K}$; en raison de la linéarité de U dans $\mathbf{K}[X]$, on vérifie aussitôt que pour tout élément $\theta \in \mathbf{K}[[S]]$ et tout $g \in E$, on a $U_X(\theta g) = \theta U_X(g)$; autrement dit, $U_X$ est une application *linéaire* du module E dans lui-même.

#### Proposition 6 {#fvr-vi-s1-prop-6 .statement}

*Soit* $U = D^pV = u(D)$ *un opérateur de composition d’ordre p dans* $\mathbf{K}[X]$, *u(S) étant une série d’ordre formelle p dans* $\mathbf{K}[[S]]$. *On a alors les formules*

$$
U_X(\exp(XS)) = u(S).\exp(XS)
$$
$$
\frac{S^p}{u(S)}\exp(XS) = \sum_{n=0}^{\infty} \frac{1}{n!}\ u_n(X)S^n
$$

$u_n$ *étant le polynôme d’Appell d’indice n attaché à U.*

D’après le scholie du th. 1 (VI, p. 4), pour établir la formule (15), il suffit de démontrer que, pour tout polynôme $f(Y) \in K[Y]$, on a
$$
U_X(\exp(XD_Y)(f(Y))) = u(D_Y)(\exp(XD_Y)(f(Y))).
$$
Or, le premier membre de (17) est $U_X(f(X + Y))$, et comme $U = u(D)$, le second membre de (17) est $U_Y(f(X + Y))$, si bien que l’identité (17) se réduit à (1) (VI, p. 2).

Il suffit ensuite d’appliquer (15) à l’opérateur de composition $V^{-1} = D^n/u(D)$ pour obtenir (16), puisque, par définition, on a
$$
V^{-1}(\exp(XS)) = \sum_{n=0}^{\infty} \frac{1}{n!} u_n(X) S^n.
$$
On notera que la formule (16) s’obtient aussi en multipliant les séries formelles $S^n/u(S)$ et $\exp(XS)$, compte tenu de (6).

On dit que la série formelle (16) est la série génératrice des polynômes d’Appell attachés à $U$.

### 4. Polynômes de Bernoulli

Considérons l’opérateur de composition $U$ défini par
$$
U(f(X)) = f(X + 1) - f(X);
$$
on peut l’écrire $U = e^D - 1$ (VI, p. 2, Exemple 1); c’est un opérateur d’ordre 1, et si on pose $U = DV$, on a $V^{-1} = \frac{D}{e^D - 1}$. Le polynôme d’Appell de degré $n$ correspondant à l’opérateur $U$ s’appelle polynôme de Bernoulli de degré $n$ et se note $B_n(X)$; si on pose $b_n = B_n(0)$, on a les formules
$$
B_n(X) = \sum_{k=0}^{n} \binom{n}{k} b_{n-k} X^k
$$
$$
\frac{Se^{XS}}{e^S - 1} = \sum_{n=0}^{\infty} \frac{1}{n!} B_n(X) S^n
$$
et en particulier
$$
\frac{S}{e^S - 1} = \sum_{n=0}^{\infty} \frac{1}{n!} b_n S^n.
$$
Les formules (7) et (9) de VI p. 5, donnent, pour les polynômes de Bernoulli, les relations
$$
\frac{dB_n}{dX} = n B_{n-1}(X)
$$
$$
B_n(X + 1) - B_n(X) = n X^{n-1}.
$$

En particulier, on a $B_n(1) - B_n(0) = 0$ pour $n > 1$, ce qui, compte tenu de (18), donne la relation de récurrence

$$
\sum_{m=0}^{n-1} \binom{n}{m} b_m = 0 \quad (\text{pour } n > 1)
$$

qui permet de calculer de proche en proche les $b_n$. Ces nombres sont évidemment rationnels; comme on peut écrire

$$
\frac{S}{e^s - 1} = -\frac{S}{2} + \frac{S}{2} \frac{e^s + 1}{e^s - 1}
$$

et que l’on a (VI, p. 4, formule (5))

$$
\frac{e^{-s} + 1}{e^{-s} - 1} = -\frac{e^s + 1}{e^s - 1}
$$

on voit que, dans la série formelle $\frac{S}{2} \frac{e^s + 1}{e^s - 1}$, tous les termes de degré impair ont un coefficient nul; on a donc

$$
b_0 = 1, \quad b_1 = -\frac{1}{2}, \quad b_{2n-1} = 0 \quad \text{pour } n > 1.
$$

Les nombres rationnels $b_{2n}$ ($n \geq 1$) sont appelés nombres de Bernoulli; nous verrons (VI, p. 19) que $b_{2n}$ a le signe de $(-1)^{n-1}$. La formule (23) donne, pour les premières valeurs de $n$,

$$
\begin{align*}
b_2 &= \frac{1}{6}, & b_4 &= -\frac{1}{30}, & b_6 &= \frac{1}{42}, & b_8 &= -\frac{1}{30}, \\
b_{10} &= \frac{5}{66}, & b_{12} &= -\frac{691}{2730}, & b_{14} &= \frac{7}{6}, \\
b_{16} &= -\frac{3617}{510}, & b_{18} &= \frac{43867}{798}, & b_{20} &= -\frac{174611}{330}, & b_{22} &= \frac{854513}{138}, \\
b_{24} &= -\frac{236364091}{2730}, & b_{26} &= \frac{8553103}{6}, & b_{28} &= -\frac{23749461029}{870}.
\end{align*}
$$

On notera que les numérateurs 691, 3617, 43867 sont premiers; les autres ont pour factorisations

$$
\begin{align*}
174611 &= 283 \times 617 \\
854513 &= 11 \times 131 \times 593 \\
236364091 &= 103 \times 2294797 \\
8553103 &= 13 \times 657931 \\
23749461029 &= 7 \times 9349 \times 362903
\end{align*}
$$

tous les facteurs des seconds membres étant premiers.

On en déduit pour expression des premiers polynômes de Bernoulli

$$
B_0(X) = 1, \quad B_1(X) = X - \frac{1}{2}, \quad B_2(X) = X^2 - X + \frac{1}{6},
$$
$$
B_3(X) = X^3 - \frac{3}{2}X^2 + \frac{1}{2}X, \quad B_4(X) = X^4 - 2X^3 + X^2 - \frac{1}{30}.
$$

### 5. Opérateurs de composition sur les fonctions d’une variable réelle

Soit I un intervalle de $\mathbf{R}$ contenant l’intervalle $\mathbf{R}_+ = (0, +\infty[$; soit E un espace vectoriel sur le corps $\mathbf{C}$, formé de fonctions d’une variable réelle à valeurs complexes, définies dans I. Nous supposerons que, pour tout $a \geqslant 0$ et toute fonction $f \in E$, la fonction $x \mapsto f(x + a)$ appartient à E; en outre, nous supposerons que E contient les restrictions à I des polynômes à coefficients complexes et des exponentielles $e^{\lambda x}$, où $\lambda$ est un nombre complexe quelconque. Nous appellerons opérateur dans E toute application linéaire $U$ de E dans l’espace de toutes les applications de I dans le corps $\mathbf{C}$ des nombres complexes; si $f \in E$ et $g = U(f)$, il sera commode d’utiliser la notation

$$
g(x) = U_{\xi}(f(\xi))
$$

$\xi$ étant donc une variable muette dans le symbole fonctionnel du second membre (cf. II, p. 9). Pour tout $a \geqslant 0$, l’opérateur qui, à toute fonction $f \in E$, associe la restriction à I de la fonction $x \mapsto f(x + a)$, est appelé l’opérateur de translation par a.

#### Définition 3 {#fvr-vi-s1-def-3 .statement}

On dit qu’un opérateur $U$ dans E est un opérateur de composition si, pour tout $a \geqslant 0$, il est permutable avec l’opérateur de translation par a.

Avec la notation introduite ci-dessus, cette définition se traduit par l’identité en $x$ et $a$ ($x \in I, a \geqslant 0$)

$$
U_{\xi + a}(f(\xi)) = U_{\xi}(f(\xi + a)).
$$

Dans cette identité, on peut échanger les rôles de $x$ et $a$ si $x \geqslant 0$, puis faire $a = 0$; on obtient ainsi, pour tout $x \geqslant 0$.

$$
U_{\xi}(f(\xi)) = U_{0}(f(\xi + x))
$$

$U_0$ étant la forme linéaire sur E qui, à toute fonction $f \in E$, fait correspondre la valeur $g(0)$ de $g = U(f)$.

Si $f$ est un polynôme, on a $f(\xi + x) = \sum_{k=0}^{s} \frac{1}{k!} f^{(k)}(\xi)x^k$, et la formule (26) montre donc que $U(f)$ est un polynôme; restreint à l’ensemble des polynômes en $x$, à coefficients dans $\mathbf{C}$ (ensemble qu’on peut identifier à l’algèbre $\mathbf{C}[X]$), l’opérateur $U$ est donc un opérateur de composition au sens de la déf. 1 de VI, p. 2, et tous les résultats des numéros précédents lui sont applicables.

Nous désignerons encore par $u_n$ les polynômes d’Appell attachés à l’opérateur $U$. Au développement taylorien généralisé d’un polynôme (VI, p. 6, formule (13)) correspond, pour des fonctions plus générales, le résultat suivant:

#### Théorème 2 {#fvr-vi-s1-thm-2 .statement}

Soit $f$ une fonction admettant une dérivée $(n+1)$-ème continue dans $I$, et appartenant à $E$ ainsi que toutes ses dérivées $f^{(m)}$ pour $1 \leq m \leq n$. Si $U$ est un opérateur de composition d’ordre $p \leq n$ dans $E$, on $a$, pour $x \geq 0$ et $h \geq 0$

$$
f^{(p)}(x + h) = \sum_{m=0}^n \frac{1}{m!} u_m(x) \ U_h^{\xi}(f^{(m)}(\xi)) + R_n(x, h)
$$

avec

$$
R_n(x, h) = - U_h^{\xi} \left( \int_0^{\xi-x-h} \frac{1}{n!} u_n(x+\eta) f^{(n+1)}(\xi-\eta) d\eta \right)
$$

(développement taylorien généralisé).

Considérons l’intégrale $\int_0^{\xi-x-h} \frac{1}{n!} u_n(x+\eta) f^{(n+1)}(\xi-\eta) d\eta$, définie pour tout $\xi \in I$, et appliquons-lui la formule d’intégration par parties d’ordre $n$ (II, p. 10, formule (11)); en tenant compte des relations

$$
u_n^{(k)} = n(n-1) \ldots (n-k+1) u_{n-k}
$$

déduites de (7) (VI, p. 5) par récurrence, il vient

$$
\int_0^{\xi-x-h} \frac{1}{n!} u_n(x+\eta) f^{(n+1)}(\xi-\eta) d\eta
$$
$$
= \sum_{m=0}^n \frac{1}{m!} u_m(x) f^{(m)}(\xi) - \sum_{m=0}^n \frac{1}{m!} u_m(\xi-h) f^{(m)}(x+h).
$$

Appliquons l’opérateur $U$ aux deux membres de la formule (29), considérés comme fonctions de $\xi$, puis prenons la valeur de la fonction obtenue pour la valeur $h$ de la variable $\xi$; en remarquant que, d’après les formules (26) (VI, p. 9) et (9) (VI, p. 5), on a

$$
U_h^{\xi}(u_m(\xi-h)) = U_0^{\xi}(u_m(\xi)) = \begin{cases} 0 & \text{pour } m \neq p \\ p! & \text{pour } m = p \end{cases}
$$

on obtient finalement la formule (27).

### 6. Indicatrice d’un opérateur de composition

Les hypothèses étant les mêmes que dans le no 5, la formule (26) de VI, p. 9, appliquée à la fonction $e^{\lambda x}$, donne

$$
U_x^{\xi}(e^{\lambda x}) = U_0^{\xi}(e^{\lambda x} e^{\lambda \xi}) = e^{\lambda x} U_0^{\xi}(e^{\lambda \xi}) = u(\lambda) e^{\lambda x}
$$

en posant $u(\lambda) = U_0^x(e^{\lambda x})$. On dit que la fonction $u(\lambda)$, définie dans $\mathbf{C}$ et à valeurs complexes, est l’indicatrice de l’opérateur de composition $U$. On notera que, si la restriction de $U$ à l’anneau $\mathbf{C}[X]$ des polynômes est égale à la série
$$
D^p \sum_{n=0}^\infty \alpha_n D^n
$$
(VI, p. 4, th. 1) (que nous avons notée $u(D)$ dans VI, p. 4), la série à termes complexes dont le terme général est $\alpha_n \lambda^{n+p}$ n’est pas nécessairement convergente pour $\lambda \neq 0$, et que, même si elle converge pour certaines valeurs de $\lambda$, sa somme n’est pas nécessairement égale à l’indicatrice $u(\lambda)$ de $U$ (VI, p. 22, exerc. 2). Nous dirons que l’opérateur de composition $U$ est régulier s’il existe un voisinage de $0$ dans $\mathbf{C}$-tel-que la série de terme général $\alpha_n \lambda^{n+p}$ soit absolument convergente et ait une somme égale à l’indicatrice $u(\lambda)$ dans ce voisinage¹.

Appliquons la formule (27) de VI, p. 10, à la fonction $e^{\lambda x}$, en faisant $h = 0$; comme $D^m(e^{\lambda x}) = \lambda^m e^{\lambda x}$, on a $U_0^x(D^n(e^{\lambda x})) = \lambda^n u(\lambda)$; il vient donc, pour tout $\lambda$ complexe tel que $u(\lambda) \neq 0$
$$
\frac{\lambda^p e^{\lambda x}}{u(\lambda)} = \sum_{m=0}^n u_m(x) \frac{\lambda^m}{m!} - \frac{\lambda^{n+1}}{u(\lambda)} U_0^x \left( \int_0^{\xi-x} \frac{1}{n!} u_n(x+\eta) e^{\lambda(x-\eta)} d\eta \right)
$$
et en particulier, pour $x = 0$
$$
\frac{\lambda^p}{u(\lambda)} = \sum_{m=0}^n \beta_m \frac{\lambda^m}{m!} - \frac{\lambda^{n+1}}{u(\lambda)} \cdot U_0^x \left( \int_0^{\xi} \frac{1}{n!} u_n(\eta) e^{\lambda(\xi-\eta)} d\eta \right)
$$
avec $\beta_m = u_m(0)$.

Si $U$ est un opérateur régulier, pour tout $\lambda \in \mathbf{C}$ tel que les séries entières $u(\lambda) = \sum_{n=0}^\infty \alpha_n \lambda^{n+p}$ et $\sum_{n=0}^\infty \beta_n \frac{\lambda^n}{n!}$ soient absolument convergentes², il résulte-de-la formule (16) et de la formule donnant le produit de deux séries absolument convergentes (TG, VIII, p. 16, prop. 1) que l’on a
$$
\frac{\lambda^p}{u(\lambda)} = \sum_{n=0}^\infty \beta_n \frac{\lambda^n}{n!}.
$$
De même, puisque le développement en série de Taylor de $e^{\lambda x}$ est absolument convergent pour tout $\lambda \in \mathbf{C}$ et tout $x \in \mathbf{C}$ (III, p. 15) on a aussi (formules (6) (VI, p. 5) et (16) (VI, p. 6), pour toutes les valeurs considérées et pour tout $x \in \mathbf{C}$
$$
\frac{\lambda^p e^{\lambda x}}{u(\lambda)} = \sum_{n=0}^\infty u_n(x) \frac{\lambda^n}{n!}
$$

¹ Nous ferons plus tard l’étude des séries dont le terme général est de la forme $c_n z^n$ ($c_n \in \mathbf{C}, z \in \mathbf{C}$), qu’on appelle séries entières; on verra en particulier que lorsqu’une telle série est absolument convergente pour $z = z_0$, elle est normalement convergente pour $|z| \leq |z_0|$.

² Il résulte de la théorie des séries entières que lorsque l’une de ces séries est absolument convergente dans un voisinage $V$ de $0$, l’autre est absolument convergente dans un voisinage $W \subset V$ de $0$.

#### Remarque {#fvr-vi-s1-n6-rem-1 .statement}

On peut utiliser la formule (33) (resp. (34)) pour le calcul des $\beta_n$ (resp. des $u_n(x)$) en utilisant le lemme suivant de la théorie des séries entières:

#### Lemme {#fvr-vi-s1-n6-lem-1 .statement}

Si deux séries entières $\sum_{n=0}^\infty c_n \lambda^n \sum_{n=0}^\infty d_n \lambda^n$ sont absolument convergentes pour tout $\lambda$ dans un voisinage de 0, et si on a $\sum_{n=0}^\infty c_n \lambda^n = \sum_{n=0}^\infty d_n \lambda^n$ pour ces valeurs de $\lambda$, alors $c_n = d_n$ pour tout entier $n \geqslant 0$.

Si, par un procédé quelconque, on peut obtenir une série entière convergente égale à $\lambda^n / u(\lambda)$ dans un voisinage de 0, les coefficients de cette série sont nécessairement égaux aux $\beta_n$. C’est ce procédé que nous allons appliquer dans les exemples qui suivent.

#### Exemple 1 {#fvr-vi-s1-n6-exa-1 .statement}

Si $U$ est l’application identique, on a $u(\lambda) = 1$, et l’opérateur $U$ est évidemment régulier; comme $u_n(x) = x^n$, la formule (27) de VI, p. 10, s’écrit, en posant $t = \xi - \eta$

$$
f(x + h) = \sum_{m=0}^n \frac{1}{m!} f^{(m)}(h)x^m + \int_h^{x+h} f^{(n+1)}(t) \frac{(x + h - t)^n}{n!} dt
$$

c’est-à-dire se réduit à la formule de Taylor (II, p. 12).

#### Exemple 2 {#fvr-vi-s1-n6-exa-2 .statement}

Prenons pour $U$ l’opérateur de composition qui, à toute fonction $f$ définie dans $\mathbf{R}_+$, fait correspondre la fonction $x \mapsto f(x + 1) - f(x)$; on a donc

$$
U_\xi^{\eta}(f(\xi)) = f(x + 1) - f(x);
$$

nous avons vu (VI, p. 7) que la restriction de $U$ à $\mathbf{C}[X]$ est égale à $e^D - 1$. Comme d’autre part $u(\lambda) = e^\lambda - 1$, l’opérateur $U$ est régulier; nous verrons (VI, p. 19) comment on peut déterminer les nombres de Bernoulli $b_n$ en calculant un développement en série entière convergente de $\frac{\lambda}{e^\lambda - 1}$. En appliquant la formule (27) de VI, p. 10, à une primitive de la fonction $f$, il vient

$$
f(x + h) = \int_h^{h+1} f(t) dt \\
+ \sum_{m=1}^n \frac{1}{m!} B_m(x)(f^{(m-1)})(h + 1) - f^{(m-1)}(h)) + R_n(x, h)
$$

avec

$$
R_n(x, h) = - \int_0^{1-x} \frac{B_n(x + \eta)}{n!} f^{(n)}(h + 1 - \eta) d\eta \\
+ \int_0^{-x} \frac{B_n(x + \eta)}{n!} f^{(n)}(h - \eta) d\eta.
$$

1 Ce lemme est un cas particulier d’un résultat général que nous démontrerons plus tard; en voici la démonstration. Si une série entière $\sum_{n=0}^\infty c_n \lambda^n$ est absolument convergente pour $\lambda = \lambda_0$, pour tout entier $k \geqslant 0$ la série $\sum_{n=0}^\infty c_{n+k} \lambda^n$ est normalement convergente pour $|\lambda| \leqslant |\lambda_0|$, donc est continue dans ce disque (TG, X, p. 10); on en conclut que $\sum_{n=k+1}^\infty c_n \lambda^n = o(\lambda^k)$ au voisinage de 0. Le lemme résulte alors de l’unicité des coefficients du développement asymptotique d’une fonction suivant les $\lambda^n$ (V, p. 12).

#### Exemple 3 {#fvr-vi-s1-n6-exa-3 .statement}

Soit E l’espace vectoriel des fonctions f définies et continues dans $\mathbf{R}$, telles en outre que l’intégrale $\int_{-\infty}^{+\infty} f(x + \xi)e^{-\xi^2/2}\ d\xi$ soit convergente pour tout $x \geqslant 0$. L’opérateur U défini par

$$
U_0^x(f(\xi)) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} f(x + \xi)d\xi
$$

est donc défini dans E et est évidemment un opérateur de composition. L’espace E contient toutes les exponentielles $e^{\lambda x}$ ($\lambda$ complexe quelconque), et on a

$$
u(\lambda) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-(\xi^2/2) + \lambda \xi}\ d\xi = \frac{1}{\sqrt{2\pi}} e^{\lambda^2/2} \int_{-\infty}^{+\infty} e^{-(\xi - \lambda)^2/2}d\xi = e^{\lambda^2/2}
$$

(cf. III, p. 28, exerc. 24, et VII, p. 9, formule (22)). On a $n! \alpha_n = U_0^n(\xi^n) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} \xi^n d\xi$. Pour tout entier n, on peut écrire

$$
\sum_{k=0}^n \int_{-\infty}^{+\infty} \frac{|\lambda \xi|^k}{k!} e^{-\xi^2/2} d\xi \leqslant 2 \int_0^{+\infty} e^{-(\xi^2/2) + |\lambda| \xi} d\xi.
$$

La série $\sum_{n=0}^{\infty} e^{-\xi^2/2} \frac{(\lambda \xi)^n}{n!}$ peut donc être intégrée terme à terme dans $\mathbf{R}$ (II, p. 22) cor. 1), ce qui prouve que la série $\sum_{n=0}^{\infty} \alpha_n \lambda^n$ converge absolument pour tout $\lambda \in \mathbf{C}$, et a une somme égale à $u(\lambda) = e^{\lambda^2/2} = \sum_{n=0}^{\infty} \frac{\lambda^{2n}}{2^n n!}$; l’opérateur U est donc régulier. L’application du lemme énoncé ci-dessus montre que $\alpha_{2n} = 1/2^n n!$, $\alpha_{2n+1} = 0$ pour tout $n \geqslant 0$; l’opérateur U est donc d’ordre 0. On a

$$
1/u(\lambda) = e^{-\lambda^2/2} = \sum_{n=0}^{\infty} \frac{(-1)^n \lambda^{2n}}{2^n n!},
$$

la série étant absolument convergente pour tout $\lambda \in \mathbf{C}$; une nouvelle application du lemme montre que $\beta_{2n} = \frac{(-1)^n (2n)!}{2^n n!}$, $\beta_{2n+1} = 0$; en outre, la série $\sum_{n=0}^{\infty} \frac{\lambda^n}{n!} u_n(x)$ est absolument convergente pour tout $\lambda \in \mathbf{C}$ et tout $x \in \mathbf{R}$, et on a

$$
\sum_{n=0}^{\infty} \frac{\lambda^n}{n!} u_n(x) = \exp \left( -\frac{\lambda^2}{2} + \lambda x \right) = \exp \left( \frac{x^2}{2} \right) \exp \left( -\frac{1}{2}(\lambda - x)^2 \right).
$$

En appliquant la formule de Taylor à la fonction $\exp \left( -x^{2/2} \right)$, on obtient donc l’expression suivante des polynômes $u_n(x)$;

$$
u_n(x) = (-1)^n e^{x^{2/2}} \frac{d^n}{dx^n} (e^{-x^{2/2}}).
$$

Ce polynôme est appelé *polynôme d’Hermite* de degré n, et se note le plus souvent $H_n(x)$. Les formules (7), (8) et (9) de VI, p. 5, donnent ici

$$
\frac{dH_n}{dx} = nH_{n-1}(x)
$$
$$
H_n(x + y) = \sum_{k=0}^n \binom{n}{k} H_{n-k}(x) y^k
$$
$$
\frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} H_n(x + \xi)d\xi = x^n
$$

et la formule (27) de VI, p. 10, devient, pour $h = 0$

$$
\sqrt{2\pi} f(x) = \sum_{m=0}^{n} \left( \int_{-\infty}^{+\infty} e^{-\xi^2/2} f^{(m)}(\xi) d\xi \right) \frac{H_m(x)}{m!}
- \int_{-\infty}^{+\infty} d\xi \int_0^x \frac{H_n(x+\eta)}{n!} e^{-(\xi+x)^2/2} f^{(n+1)}(x+\xi-\eta) d\eta.
$$

### 7. La formule sommatoire d’Euler-Maclaurin

Dans la formule (35) de VI, p. 12, remplaçons $x$ par $0$, et $h$ par $x$; comme $B_m(0) = b_m$, il résulte des relations (24) de VI, p. 8, qu’on peut écrire, pour tout entier $p > 0$

$$
f(x) = \int_x^{x+1} f(t) \, dt - \frac{1}{2}(f(x+1) - f(x))
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} (f^{(2k-1)}(x+1) - f^{(2k-1)}(x)) + R_p(x)
$$
avec
$$
R_p(x) = -\frac{1}{(2p+1)!} \int_0^1 B_{2p+1}(t) f^{(2p+1)}(x+1-t) \, dt.
$$

Dans cette formule, remplaçons successivement $x$ par $x+1, x+2, \ldots, x+n$, et ajoutons les formules obtenues membre à membre; il vient
$$
\begin{cases}
f(x) + f(x+1) + \cdots + f(x+n) \\
= \int_x^{x+n+1} f(t) \, dt - \frac{1}{2} (f(x+n+1) - f(x)) \\
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} (f^{(2k-1)}(x+n+1) - f^{(2k-1)}(x)) + T_p(x, n)
\end{cases}
$$
avec
$$
T_p(x, n) = -\frac{1}{(2p+1)!} \int_0^1 B_{2p+1}(t) \left( \sum_{k=0}^n f^{(2p+1)}(x+k+1-t) \right) dt.
$$

Le reste $T_p(x, n)$ de cette formule peut encore s’écrire de la façon suivante: désignons par $\overline{B}_{2p+1}(t)$ la fonction périodique de période 1, égale à $B_{2p+1}(t)$ dans l’intervalle $(0, 1[$. On a alors
$$
\int_0^1 B_{2p+1}(t) f^{(2p+1)}(x+k+1-t) dt = \int_k^{k+1} \overline{B}_{2p+1}(1-s) f^{(2p+1)}(x+s) ds
$$
et par suite
$$
T_p(x, n) = -\frac{1}{(2p+1)!} \int_0^{n+1} \overline{B}_{2p+1}(1-s) f^{(2p+1)}(x+s) ds.
$$

La formule (39) est dite *formule sommatoire d’Euler-Maclaurin*; elle est applicable à toute fonction complexe ayant une dérivée $(2p+1)$-ème continue dans un intervalle $\{x_0, +\infty\}$, pour tout $x \geq x_0$. Nous verrons (VI, p. 20) comment on peut majorer le *reste* $T_p(x, n)$ de cette formule.

## EXERCICES {#fvr-vi-s1-exercises}

See the [exercises for § 1](exercises/s1/).
