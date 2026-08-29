---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: Sous-algèbres de Cartan. Éléments réguliers
section: 1
section_title: Décomposition primaire des représentations linéaires
lang: fr
source: lie-vii-viii-fr
pdf_pages: 0001-0012, 0049-0052
extraction: ocr
subsections:
    - "no": 1
      title: Décomposition d'une famille d'endomorphismes
      page: 0
      pdf_page: 1
    - "no": 2
      title: Cas d'une famille linéaire d'endomorphismes
      page: 0
      pdf_page: 6
    - "no": 3
      title: Décomposition des représentations d’une algèbre de Lie nilpotente
      page: 0
      pdf_page: 7
    - "no": 4
      title: Décomposition d’une algèbre de Lie relativement à un automorphisme
      page: 0
      pdf_page: 10
    - "no": 5
      title: Invariants d’une algèbre de Lie semi-simple relativement à une action semi-simple
      page: 0
      pdf_page: 11
statements: 25
exercises: 11
content_sha256: 93055c29b31ba278750646b090533b3f67516ae2208265d1bf0262d77022244c
---

## § 1. Décomposition primaire des représentations linéaires

### 1. Décomposition d'une famille d'endomorphismes

Soient V un espace vectoriel, S un ensemble, et r une application de S dans End(V). Notons P l'ensemble des applications de S dans k. Si $\lambda \in P$, on note $V_{\lambda}(S)$ (resp. $V^{\lambda}(S)$) l'ensemble des $v \in V$ tels que, pour tout $s \in S$, on ait $r(s)v = \lambda(s)v$ (resp. $(r(s) - \lambda(s))^nv = 0$ pour n assez grand). Les ensembles $V_{\lambda}(S)$ et $V^{\lambda}(S)$ sont des sous-espaces vectoriels de V, et l'on a $V_{\lambda}(S) \subset V^{\lambda}(S)$. On dit que $V_{\lambda}(S)$ est le sous-espace propre de V relatif à $\lambda$ (et à r), que $V^{\lambda}(S)$ est le sous-espace primaire de V relatif à $\lambda$ (et à r), que $V^{0}(S)$ est le nilespace de V (relatif à r). On dit que $\lambda$ est un poids de S dans V si $V^{\lambda}(S) \neq 0$.

En particulier, quand S est réduit à un seul élément s, P s'identifie à k; on emploie les notations $V_{\lambda(s)}(s)$ et $V^{\lambda(s)}(s)$, ou $V_{\lambda(s)}(r(s))$ et $V^{\lambda(s)}(r(s))$, au lieu des notations $V_{\lambda}(\{s\})$, $V^{\lambda}(\{s\})$; on parle des sous-espaces propres, des sous-espaces primaires, du nilespace de $r(s)$; un élément $v$ de $V_{\lambda(s)}(s)$ est appelé un vecteur propre de $r(s)$, et, si $v \neq 0$, $\lambda(s)$ est appelé la valeur propre correspondante (cf. A, VII, § 5).

On a aussitôt, pour tout $\lambda \in P$, les relations

(1)
$$
V^{\lambda}(S) = \bigcap_{s \in P} V^{\lambda(s)}(s),
$$

(2)
$$
V_{\lambda}(S) = \bigcap_{s \in P} V_{\lambda(s)}(s).
$$

Soit $k'$ une extension de k. L'application canonique de End(V) dans End(V $\otimes_k k'$), donne par composition avec r, une application $r': S \to \mathrm{End}(V \otimes_k k')$. De même, toute application $\lambda$ de S dans k définit canoniquement une application, notée encore $\lambda$, de S dans $k'$. Avec ces notations, on a la proposition suivante:

#### Proposition 1 {#lie-vii-s1-prop-1 .statement tag=00SJ}

Pour tout $\lambda \in P$, on a
$$
(V \otimes_k k')^{\lambda}(S) = V^{\lambda}(S) \otimes_k k' \quad \text{et} \quad (V \otimes_k k')_{\lambda}(S) = V_{\lambda}(S) \otimes_k k'.
$$

Soit $(a_i)$ une base du $k$-espace vectoriel $k'$. Si $v \in V \otimes_k k'$, $v$ se met de manière unique sous la forme $\sum v_i \otimes a_i$, où $(v_i)$ est une famille à support fini d’éléments de $V$. On a, pour tout $s \in S$,

$$(r'(s) - \lambda(s))^n(v) = \sum (r(s) - \lambda(s))^nv_i \otimes a_i.$$

Il s’ensuit que

$$
\begin{align*}
v \in (V \otimes_k k')^\lambda(S) &\Leftrightarrow v_i \in V^\lambda(S) \quad \text{pour tout } i, \\
v \in (V \otimes_k k')_\lambda(S) &\Leftrightarrow v_i \in V_\lambda(S) \quad \text{pour tout } i,
\end{align*}
$$

ce qui entraîne la proposition.

#### Proposition 2 {#lie-vii-s1-prop-2 .statement tag=00SK}

*Soient $V, V', W$ des espaces vectoriels. Soient $r : S \to \mathrm{End}(V)$, $r' : S \to \mathrm{End}(V')$ et $q : S \to \mathrm{End}(W)$ des applications.*

(i) *Soit $f : V \to W$ une application linéaire telle que $q(s)f(v) = f(r(s)v)$ pour $s \in S$ et $v \in V$. Alors, pour tout $\lambda \in P$, $f$ applique $V^\lambda(S)$ (resp. $V_\lambda(S)$) dans $W^\lambda(S)$ (resp. $W_\lambda(S)$).*

(ii) *Soit $B : V \times V' \to W$ une application bilinéaire telle que*

$$q(s)B(v, v') = B(r(s)v, v') + B(v, r'(s)v')$$

*pour $s \in S$, $v \in V$, $v' \in V'$. Alors, pour tous $\lambda, \mu \in P$, $B$ applique $V^\lambda(S) \times {V'}^\mu(S)$ (resp. $V_\lambda(S) \times V'_\mu(S)$) dans $W^{\lambda+\mu}(S)$ (resp. $W_{\lambda+\mu}(S)$).*

(iii) *Soit $B : V \times V' \to W$ une application bilinéaire telle que*

$$q(s)B(v, v') = B(r(s)v, r'(s)v')$$

*pour $s \in S$, $v \in V$, $v' \in V'$. Alors, pour tous $\lambda, \mu \in P$, $B$ applique $V^\lambda(S) \times {V'}^\mu(S)$ (resp. $V_\lambda(S) \times V'_\mu(S)$) dans $W^{\lambda\mu}(S)$ (resp. $W_{\lambda\mu}(S)$).*

Dans le cas (i), on a $(q(s) - \lambda(s))^nf(v) = f((r(s) - \lambda(s))^nv)$ pour $s \in S$ et $v \in V$, et l’on conclut aussitôt. Dans le cas (ii), on a

$$(q(s) - \lambda(s) - \mu(s))B(v, v') = B((r(s) - \lambda(s))v, v') + B(v, (r'(s) - \mu(s))v')$$

pour $s \in S$, $v \in V$, $v' \in V'$, d’où par récurrence sur $n$

$$(q(s) - \lambda(s) - \mu(s))^nB(v, v') = \sum_{i+j=n} \binom{n}{i} B((r(s) - \lambda(s))^iv, (r'(s) - \mu(s))^jv').$$

On en déduit immédiatement les assertions de (ii). Dans le cas (iii), on a

$$(q(s) - \lambda(s)\mu(s))B(v, v') = B((r(s) - \lambda(s))v, r'(s)v') + B(\lambda(s)v, (r'(s) - \mu(s))v')$$

pour $s \in S$, $v \in V$, $v' \in V'$, d’où par récurrence sur $n$

$$(q(s) - \lambda(s)\mu(s))^nB(v, v') = \sum_{i+j=n} \binom{n}{i} B(\lambda(s)^j(r(s) - \lambda(s))^iv, r'(s)^j(r'(s) - \mu(s))^jv').$$

On en déduit immédiatement les assertions de (iii).

#### Proposition 3 {#lie-vii-s1-prop-3 .statement tag=00SL}

La somme $\sum_{\lambda \in P} V^\lambda(S)$ est directe. La somme $\sum_{\lambda \in P} V_\lambda(S)$ est directe.

La seconde assertion est conséquence de la première; il suffit de prouver celle-ci. Distinguons plusieurs cas.

a) S est vide. L’assertion est triviale.

b) S est réduit à un élément s. Soient $\lambda_0, \lambda_1, \ldots, \lambda_n$ des éléments distincts de k. Pour $i = 0, 1, \ldots, n$, soit $v_i \in V^{\lambda_i}(s)$ et supposons que $v_0 = v_1 + \cdots + v_n$. Il s’agit de prouver que $v_0 = 0$. Pour $i = 0, \ldots, n$, il existe un entier $q_i > 0$ tel que $(r(s) - \lambda_i)^{q_i} v_i = 0$. Considérons les polynômes $P(X) = \prod_{i \geq 1} (X - \lambda_i)^{q_i}$ et $Q(X) = (X - \lambda_0)^{q_0}$. On a $Q(r(s))v_0 = 0$, et $P(r(s))v_0 = \sum_{i=1}^n P(r(s))v_i = 0$.

Comme P et Q sont premiers entre eux, l’identité de Bezout prouve que $v_0 = 0$.

c) S est fini non vide. Raisonnons par récurrence sur le cardinal de S. Soient $s \in S$ et $S' = S - \{s\}$. Soit $(v_\lambda)_{\lambda \in P}$ une famille à support fini d’éléments de V tels que $\sum_{\lambda \in P} v_\lambda = 0$ et $v_\lambda \in V^\lambda(S)$. Soit $\lambda_0 \in P$. Notons $P'$ l’ensemble des $\lambda \in P$ tels que $\lambda|S' = \lambda_0|S'$. D’après l’hypothèse de récurrence appliquée à $S'$, on a $\sum_{\lambda \in P'} v_\lambda = 0$.

Si $\lambda, \mu$ sont des éléments distincts de $P'$, on a $\lambda(s) \neq \mu(s)$. Comme la somme $\sum_{\alpha \in k} V^\alpha(s)$ est directe d’après b), et que $v_\lambda \in V^{\lambda(s)}(s)$, on a $v_\lambda = 0$ pour tout $\lambda \in P'$, et en particulier $v_{\lambda_0} = 0$, ce qu’il fallait démontrer.

d) Cas général. Soit $(v_\lambda)_{\lambda \in P}$ une famille à support fini d’éléments de V telle que $\sum_{\lambda \in P} v_\lambda = 0$ et $v_\lambda \in V^\lambda(S)$. Soit $P'$ l’ensemble fini des $\lambda \in P$ tels que $v_\lambda \neq 0$, et soit $S'$ une partie finie de S telle que les conditions $\lambda \in P', \mu \in P', \lambda|S' = \mu|S'$ entraînent $\lambda = \mu$. On a $v_\lambda \in V^{\lambda|S'}(S')$; appliquant c), on voit que $v_\lambda = 0$ pour $\lambda \in P'$, ce qui achève la démonstration.

Rappelons que, si $x \in \mathrm{End}(V)$, on note ad $x$ l’application $y \mapsto xy - yx = [x, y]$ de $\mathrm{End}(V)$ dans lui-même.

#### Lemme 1 {#lie-vii-s1-lem-1 .statement tag=00SM}

Soient $x, y \in \mathrm{End}(V)$.

(i) Supposons V de dimension finie. Pour que x soit trigonalisable, il faut et il suffit que $V = \sum_{a \in k} V^a(x)$.

(ii) S’il existe un entier n tel que $(\mathrm{ad}\ x)^n y = 0$, chaque $V^a(x)$ est stable par y.

(iii) Supposons V de dimension finie. Si $V = \sum_{a \in k} V^a(x)$ et si chaque $V^a(x)$ est stable par y, il existe un entier n tel que $(\mathrm{ad}\ x)^n y = 0$.

La partie (i) résulte de A, VII, § 5, n° 2, prop. 3.

Soit E = End(V). Soit B l’application bilinéaire $(u, v) \mapsto u(v)$ de E $\times$ V dans V. Par définition de ad $x$, on a

$$
x(B(u, v)) = B(u, x(v)) + B((\mathrm{ad}\ x)(u), v)
$$

pour $x \in E, u \in E, v \in V$. Faisons opérer $x$ sur $E$ par $\mathrm{ad}\,x$. D’après la prop. 2 (ii), on a $B(E^0(x), V^a(x)) \subset V^a(x)$ pour tout $a \in k$. Si $(\mathrm{ad}\,x)^n y = 0$, alors $y \in E^0(x)$, donc $y(V^a(x)) \subset V^a(x)$, ce qui prouve (ii).

Pour prouver (iii), on peut remplacer $V$ par $V^a(x)$, $x$ (resp. $y$) par sa restriction à $V^a(x)$. Quitte à remplacer $x$ par $x - a$, on peut donc supposer $x$ nilpotent. Alors $(\mathrm{ad}\,x)^{2\dim V - 1} = 0$ (I, § 4, n° 2), ce qui prouve (iii).

#### Remarque {#lie-vii-s1-n1-rem-1 .statement tag=00SN}

La démonstration prouve que, si $V$ est de dimension finie et s’il existe un entier $n$ tel que $(\mathrm{ad}\,x)^n y = 0$, alors $(\mathrm{ad}\,x)^{2\dim V - 1} y = 0$.

Dans la suite, nous dirons que l’application $r : S \to \mathrm{End}(V)$ satisfait à la condition (PC) (de « presque commutativité ») si l’on a:
(PC) *Pour tout couple* $(s, s')$ *d’éléments de S*, *il existe un entier n tel que*
$$
(\mathrm{ad}\,r(s))^n r(s') = 0.
$$

#### Théorème 1 {#lie-vii-s1-thm-1 .statement tag=00SO}

*Supposons V de dimension finie. Les conditions suivantes sont équivalentes* :
(i) *La condition* (PC) *est vérifiée et, pour tout s \in S, r(s) est trigonalisable*.
(ii) *Pour tout* $\lambda \in P$, $V^\lambda(S)$ *est stable par r(S), et l’on a* $V = \sum_{\lambda \in P} V^\lambda(S)$.

Si $V = \sum_{\lambda \in P} V^\lambda(S)$, on a $V = \sum_{a \in k} V^a(s)$ pour tout $s \in S$, et il résulte du lemme 1 que (ii) entraîne (i). Supposons la condition (i) vérifiée. Le lemme 1 et la formule (1) entraînent que chaque $V^\lambda(S)$ est stable par $r(S)$. Reste à prouver que $V = \sum_{\lambda \in P} V^\lambda(S)$. Nous raisonnons par récurrence sur $\dim V$. Distinguons deux cas.
a) Pour tout $s \in S$, $r(s)$ admet une seule valeur propre $\lambda(s)$. Alors $V = V^{\lambda(s)}(S)$.
b) Il existe $s \in S$ tel que $r(s)$ admette au moins deux valeurs propres distinctes. Alors $V$ est somme directe des $V^a(s)$ pour $a \in k$, et $\dim V^a(s) < \dim V$ pour tout $a$. Chaque $V^a(s)$ est stable par $r(S)$, et il suffit d’appliquer l’hypothèse de récurrence.

#### Corollaire 1 {#lie-vii-s1-thm-1-cor-1 .statement tag=00SP}

*Supposons V de dimension finie et la condition* (PC) *vérifiée. Soit k’ une extension de k. On suppose que, pour tout s \in S, l’endomorphisme r(s) \otimes 1 de V \otimes_k k’ est trigonalisable. Soit P’ l’ensemble des applications de S dans k’. Alors* $V \otimes_k k' = \sum_{\lambda' \in P'} (V \otimes_k k')^{\lambda'}(S)$.

Soit $r' : S \to \mathrm{End}(V \otimes_k k')$ l’application définie par $r$. Si $s_1, s_2 \in S$, il existe un entier $n$ tel que $(\mathrm{ad}\,r(s_1))^n r(s_2) = 0$, d’où $(\mathrm{ad}\,r'(s_1))^n r'(s_2) = 0$. Il suffit alors d’appliquer le th. 1.

#### Corollaire 2 {#lie-vii-s1-thm-1-cor-2 .statement tag=00SQ}

*Supposons V de dimension finie et la condition* (PC) *vérifiée. Notons* $V^+(S)$ *le sous-espace vectoriel* $\sum_{s \in S} \left( \bigcap_{i \geq 1} r(s)^i V \right)$. *Alors* :
(i) $V^0(S)$ *et* $V^+(S)$ *sont stables par r(S)*;

(ii) $V = V^0(S) \oplus V^+(S);$
(iii) *tout sous-espace vectoriel W de V, stable par r(S) et tel que W^0(S) = 0, est contenu dans V^+(S);*
(iv) *on a $\sum_{s \in S} r(s)V^+(S) = V^+(S).$*
En outre, $V^+(S)$ est le seul sous-espace vectoriel de V possédant les propriétés (i) et (ii).
Pour toute extension $k'$ de $k$, on a $(V \otimes_k k')^+(S) = V^+(S) \otimes_k k'$.

La dernière assertion est immédiate. Pour prouver les autres, on peut alors, compte tenu de la prop. 1, supposer $k$ algébriquement clos. On a, d’après le th. 1, $V = \sum_{\lambda \in P} V^\lambda(S)$, et les $V^\lambda(S)$ sont stables par $r(S)$. Si $s \in S$, le polynôme caractéristique de $r(s) | V^\lambda(S)$ est $(X - \lambda(s))^{dim\, V^\lambda(S)}$; il s’ensuit que $\bigcap_{i \geq 1} r(s)^i V^\lambda(s)$ est nul si $\lambda(s) = 0$ et égal à $V^\lambda(S)$ si $\lambda(s) \neq 0$; par conséquent
(3)
$$
V^+(S) = \sum_{\lambda \in P, \lambda \neq 0} V^\lambda(S),
$$
ce qui prouve (i), (ii) et (iv). Si $W$ est un sous-espace vectoriel de $V$ stable par $r(S)$, on a $W = \sum_{\lambda \in P} W^\lambda(S)$ et $W^\lambda(S) = W \cap V^\lambda(S)$. Si $W^0(S) = 0$, on voit que $W \subset V^+(S)$, ce qui prouve (iii).

Soit $V'$ un sous-espace vectoriel de $V$ stable par $r(S)$ et tel que $V' \cap V^0(S) = 0$. On a ${V'}^0(S) = 0$, donc $V' \subset V^+(S)$ d’après (iii). Si de plus $V = V^0(S) + V'$, on voit que $V' = V^+(S)$.

On dit parfois que $(V^0(S), V^+(S))$ est la *décomposition de Fitting* de $V$, ou de l’application $r : S \to \mathrm{End}(V)$. Si $S$ est réduit à un seul élément $s$, on écrit $V^+(s)$ ou $V^+(r(s))$ au lieu de $V^+(\{s\})$. On a $V = V^0(s) \oplus V^+(s)$, $V^0(s)$ et $V^+(s)$ sont stables par $r(s)$, $r(s) | V^0(s)$ est nilpotent et $r(s) | V^+(s)$ est bijectif.

#### Corollaire 3 {#lie-vii-s1-thm-1-cor-3 .statement tag=00SR}

Soient $V$ et $V'$ des espaces vectoriels de dimension finie, $r : S \to \mathrm{End}(V)$ et $r' : S \to \mathrm{End}(V')$ des applications vérifiant la condition (PC). Soit $f : V \to V'$ une application linéaire surjective telle que $f(r(s)v) = r'(s)f(v)$ pour $s \in S$ et $v \in V$. Alors $f(V^\lambda(S)) = {V'}^\lambda(S)$ pour tout $\lambda \in P$.

Grâce à la prop. 1, on se ramène au cas où $k$ est algébriquement clos. On a $V = \bigoplus_{\lambda \in P} V^\lambda(S)$, $V' = \bigoplus_{\lambda \in P} {V'}^\lambda(S)$ d’après le th. 1, et $V' = f(V) = \sum_{\lambda \in P} f(V^\lambda(S))$.
Enfin, $f(V^\lambda(S)) \subset {V'}^\lambda(S)$ d’après la prop. 2 (i), d’où le corollaire.

#### Proposition 4 {#lie-vii-s1-prop-4 .statement tag=00SS}

*Supposons k parfait.* Soient $V$ un espace vectoriel de dimension finie, $u$ un élément de $\mathrm{End}(V)$, $u_s, u_n$ les composantes semi-simple et nilpotente de $u$ (A, VII, § 5, n° 8).
(i) *Pour tout $\lambda \in k$, on a $V^\lambda(u) = V^\lambda(u_s) = V_\lambda(u_s)$.*
(ii) *Si V est muni d’une structure d’algèbre et si u est une dérivation de V, $u_s$ et $u_n$ sont des dérivations de V.*

(iii) Si V est muni d'une structure d'algèbre et si u est un automorphisme de V, alors $u_s$ et $1 + u_s^{-1}u_n$ sont des automorphismes de V.

Grâce à la prop. 1, on peut supposer k algébriquement clos, d'où
$$
V = \sum_{\lambda \in k} V^\lambda(u).
$$
La composante semi-simple de $u|V^\lambda(u)$ est l'homothétie de rapport $\lambda$ dans $V^\lambda(u)$. Cela prouve (i).

Supposons désormais V muni d'une structure d'algèbre. Soient $x \in V^\lambda(u)$, $y \in V^\mu(u)$.

Si u est une dérivation de V, on a $xy \in V^{\lambda+\mu}(u)$ (prop. 2 (ii)), donc
$$
u_s(xy) = (\lambda + \mu)(xy) = (\lambda x)y + x(\mu y) = (u_s x)y + x(u_s y).
$$
Cela prouve que $u_s$ est une dérivation de V. Alors $u_n = u - u_s$ est aussi une dérivation de V.

Si u est un automorphisme de V, on a $\mathrm{Ker}(u_s) = V^0(u) = 0$, donc $u_s$ est bijectif. D'autre part, $xy \in V^{\lambda\mu}(u)$ (prop. 2 (iii)), donc
$$
u_s(xy) = (\lambda \mu)(xy) = (\lambda x)(\mu y) = u_s(x) \cdot u_s(y).
$$
Cela prouve que $u_s$ est un automorphisme de V ; il en est de même de
$$
1 + u_s^{-1}u_n = u_s^{-1}u.
$$

### 2. Cas d'une famille linéaire d'endomorphismes

Nous supposons maintenant que S est muni d'une structure d'espace vectoriel, que l'application $r : S \to \mathrm{End}(V)$ est linéaire, et que V et S sont de dimension finie.

#### Proposition 5 {#lie-vii-s1-prop-5 .statement tag=00ST}

Supposons la condition (PC) vérifiée, et soit $\lambda : S \to k$ tel que $V^\lambda(S) \neq 0$. Si k est de caractéristique 0, l'application $\lambda$ est linéaire. Si k est de caractéristique $p \neq 0$, il existe une puissance q de p divisant $\dim V^\lambda(S)$, et une fonction polynomiale homogène $P : S \to k$ de degré q, telles que $\lambda(s)^q = P(s)$ pour tout $s \in S$.

Comme $V^\lambda(S)$ est stable par $r(S)$ (lemme 1 et formule (1) du n° 1), on peut supposer que $V = V^\lambda(S)$. Soit $n = \dim V$. Pour $s \in S$, on a alors
$$
\det(X - r(s)) = (X - \lambda(s))^n.
$$
D'autre part, le développement du déterminant prouve que
$$
\det(X - r(s)) = X^n + a_1(s)X^{n-1} + \cdots + a_i(s)X^{n-i} + \cdots
$$
où $a_i : S \to k$ est une fonction polynomiale homogène de degré i. Ecrivons $n = qm$ où q est une puissance de l'exposant caractéristique de k et où $(q, m) = 1$. On a alors $(X - \lambda(s))^n = (X^q - \lambda(s)^q)^m$; d'où $-m \lambda(s)^q = a_q(s)$, ce qui entraîne le résultat.

#### Proposition 6 {#lie-vii-s1-prop-6 .statement tag=00SU}

Supposons k infini et la condition (PC) vérifiée. Soit k' une extension de k. Posons V' = V $\otimes_k k'$, S' = S $\otimes_k k'$. Soit r': S' $\to$ End(V') l’application déduite de r par extension des scalaires. Alors

$$
V^0(S) \otimes_k k' = {V'}^0(S) = {V'}^0(S').
$$

La première égalité résulte de la prop. 1. Pour prouver la deuxième, on peut supposer V = V^0(S) d’où V' = V'^0(S). Soient (s_1, ..., s_m) une base de S et (e_1, ..., e_n) une base de V. Il existe des polynômes P_{ij}(X_1, ..., X_m) tels que

$$
r'(a_1 s_1 + \cdots + a_m s_m)^n e_j = \sum_{i=1}^n P_{ij}(a_1, ..., a_m) e_i
$$

pour $1 \leq j \leq n$ et $a'_1, ..., a'_m \in k'$. Par hypothèse, on a $r'(s)^n = 0$ pour tout $s \in S$, c’est-à-dire $P_{ij}(a_1, ..., a_m) = 0$ pour $1 \leq i, j \leq n$ et $a_1, ..., a_m \in k$. Comme k est infini, on a donc $P_{ij} = 0$. Par suite, tout élément de $r'(S')$ est nilpotent et $V' = {V'}^0(S')$.

#### Proposition 7 {#lie-vii-s1-prop-7 .statement tag=00SV}

Supposons k infini et la condition (PC) vérifiée. Soit $\tilde{S}$ l’ensemble des $s \in S$ tels que $V^0(s) = V^0(S)$. Si $s \in S$, soit $P(s)$ le déterminant de l’endomorphisme de $V/V^0(S)$ défini par $r(s)$ (n° 1, cor. 2 (i) au th. 1).

(i) La fonction $s \mapsto P(s)$ est polynomiale sur S. On a $\tilde{S} = \{ s \in S \mid P(s) \neq 0 \}$; c’est un ouvert de S pour la topologie de Zariski (App. I).

(ii) $\tilde{S}$ est non vide, et, pour tout $s \in \tilde{S}$, on a $V^+(s) = V^+(S)$.

Le fait que $s \mapsto P(s)$ soit polynomiale résulte de la linéarité de r. Si $s \in S$, on a $V^0(s) \supseteq V^0(S)$, avec égalité si et seulement si $r(s)$ définit un automorphisme de $V/V^0(S)$, d’où (i).

Soit maintenant $k'$ une clôture algébrique de k, et introduisons V', S', r' comme dans la prop. 6. Remarquons que S' vérifie la condition (PC) par prolongement de l’identité polynomiale $\operatorname{ad}(r(s_1))^{2 \dim V - 1} r(s_2) = 0$ valable pour $s_1, s_2 \in S$ (n° 1, remarque). Appliquant le th. 1, on en déduit une décomposition

$$
V' = {V'}^0(S') \oplus \sum_{i=1}^m {V'}^{\lambda_i}(S')
$$

avec $\lambda_i \neq 0$ pour $1 \leq i \leq m$. Pour $1 \leq i \leq m$, il existe une fonction polynomiale $P_i$ non nulle sur S' et un entier $q_i$ tels que $\lambda_i^{q_i} = P_i$ (prop. 5). Puisque k est infini, il existe $s \in S$ tel que $(P_1 ... P_m)(s) \neq 0$, cf. A, IV, § 2, n° 3, cor. 2 à la prop. 9. On a alors $\lambda_i(s) \neq 0$ pour tout $i$, d’où ${V'}^0(S') = {V'}^0(s)$ et par suite $V^0(S) = V^0(s)$ (prop. 6), ce qui montre que $\tilde{S} \neq \emptyset$. Si $s \in \tilde{S}$, le fait que $V^+(S)$ soit stable par $r(s)$ et supplémentaire de $V^0(s)$ dans V entraîne que $V^+(S) = V^+(s)$ (cor. 2 au th. 1).

### 3. Décomposition des représentations d’une algèbre de Lie nilpotente

Soient $\mathfrak{h}$ une algèbre de Lie et M un $\mathfrak{h}$-module. Pour toute application $\lambda$ de $\mathfrak{h}$ dans $k$, on a défini au n° 1 les sous-espaces vectoriels $M^\lambda(\mathfrak{h})$ et $M_\lambda(\mathfrak{h})$ de M. En particulier, si $g$ est une algèbre de Lie contenant $h$ comme sous-algèbre, et si $x \in g$, on emploiera souvent les notations $g^\lambda(h)$ et $g_\lambda(h)$ $g^\alpha(x)$ et $g_\alpha(x)$; il sera alors sous-entendu qu’on fait opérer $h$ dans $g$ par la représentation adjointe $\mathrm{ad}_g$.

#### Proposition 8 {#lie-vii-s1-prop-8 .statement tag=00SW}

*Soient $h$ une algèbre de Lie, et $L, M, N$ des $h$-modules. Notons $P$ l’ensemble des applications de $h$ dans $k$.*

(i) *La somme $\sum_{\lambda \in P} L^\lambda(h)$ est directe.*

(ii) *Si $f : L \to M$ est un homomorphisme de $h$-modules, on a $f(L^\lambda(h)) \subset M^\lambda(h)$ pour tout $\lambda \in P$.*

(iii) *Si $f : L \times M \to N$ est une application bilinéaire $h$-invariante, on a*
$$
f(L^\lambda(h) \times M^\mu(h)) \subset N^{\lambda + \mu}(h)
$$
*quels que soient $\lambda, \mu \in P$.*
Cela résulte des prop. 2 et 3.

#### Proposition 9 {#lie-vii-s1-prop-9 .statement tag=00SX}

*Soient $h$ une algèbre de Lie nilpotente et $M$ un $h$-module de dimension finie. Notons $P$ l’ensemble des applications de $h$ dans $k$.*

(i) *Chaque $M^\lambda(h)$ est un sous-$h$-module de $M$. Si, pour tout $x \in h$, $x_M$ est trigonalisable, alors $M = \sum_{\lambda \in P} M^\lambda(h)$.*

(ii) *Si $k$ est infini, il existe $x \in h$ tel que $M^0(x) = M^0(h)$.*

(iii) *Si $k$ est de caractéristique 0, et si $\lambda \in P$ est tel que $M^\lambda(h) \neq 0$, alors $\lambda$ est une forme linéaire sur $h$ nulle sur $[h, h]$, et $M_\lambda(h) \neq 0$.*

(iv) *Si $f : M \to N$ est un homomorphisme surjectif de $h$-modules de dimension finie, on a $f(M^\lambda(h)) = N^\lambda(h)$ pour tout $\lambda \in P$.*

(v) *Si $N$ est un $h$-module de dimension finie, et $B$ une forme bilinéaire sur $M \times N$ invariante par $h$, alors $M^\lambda(h)$ et $N^\mu(h)$ sont orthogonaux relativement à $B$ si $\lambda + \mu \neq 0$. Si, en outre, $B$ est non dégénérée, il en est de même de sa restriction à $M^\lambda(h) \times N^{-\lambda}(h)$ pour tout $\lambda \in P$.*

La partie (i) résulte du n° 1, lemme 1 et th. 1. La partie (ii) résulte du n° 2, prop. 7. La partie (iv) résulte du n° 1, cor. 3 du th. 1. Prouvons (iii). On peut supposer que $M = M^\lambda(h)$. Alors, pour tout $x \in h$, on a $\lambda(x) = (\dim V)^{-1} \mathrm{Tr}(x_M)$; cela prouve que $\lambda$ est linéaire (ce qui résulte aussi de la prop. 5) et que $\lambda$ s’annule sur $[h, h]$. Considérons l’application $\rho : h \to \mathrm{End}_k(M)$ définie par
$$
\rho(x) = x_M - \lambda(x)1_M;
$$
en vertu de ce qui précède, c’est une représentation de $h$ dans $M$, et $\rho(x)$ est nilpotent pour tout $x \in h$. D’après le th. d’Engel (I, § 4, n° 2, th. 1), il existe $m \neq 0$ dans $M$ tel que $\rho(x)m = 0$ pour tout $x \in h$, d’où $m \in M_\lambda(h)$.

La première assertion de (v) résulte du n° 1, prop. 2, (ii). Pour prouver la deuxième, on peut supposer $k$ algébriquement clos, vu la prop. 1 du n° 1; elle résulte alors de la première et du fait que $M = \sum_\lambda M^\lambda(h)$, $N = \sum_\mu N^\mu(h)$, cf. (i).

#### Remarque {#lie-vii-s1-n3-rem-1 .statement tag=00SY}

Supposons k parfait de caractéristique 2. Soient $\mathfrak{h} = \mathfrak{sl}(2, k)$, et M le $\mathfrak{h}$-module $k^2$ (pour l’application identique de $\mathfrak{h}$). Si $x = \begin{pmatrix} a & b \\ c & a \end{pmatrix}$ est un élément quelconque de $\mathfrak{h}$, notons $\lambda(x)$ l’unique $\lambda \in k$ tel que $\lambda^2 = a^2 + bc$. Alors $M = M^\lambda(\mathfrak{h})$ comme le montre un calcul immédiat; en revanche, $M_\lambda(\mathfrak{h}) = 0$ et $\lambda$ n’est ni linéaire, ni nulle sur $[\mathfrak{h}, \mathfrak{h}]$, bien que $\mathfrak{h}$ soit nilpotente.

#### Corollaire {#lie-vii-s1-n3-cor-1 .statement tag=00SZ}

Soient $\mathfrak{h}$ une algèbre de Lie nilpotente, et M un $\mathfrak{h}$-module de dimension finie tel que $M^0(\mathfrak{h}) = 0$. Soit $f : \mathfrak{h} \to M$ une application linéaire telle que
$$
f([x, y]) = x.f(y) - y.f(x) \quad \text{pour } x, y \in \mathfrak{h}.
$$
Il existe $a \in M$ tel que $f(x) = x.a$ pour tout $x \in \mathfrak{h}$.

Soit $N = M \times k$. Faisons opérer $\mathfrak{h}$ sur N par la formule
$$
x.(m, \lambda) = (xm - \lambda f(x), 0).
$$
L’identité vérifiée par $f$ entraîne que N est un $\mathfrak{h}$-module (I, § 1, no 8, exemple 2). L’application $(m, \lambda) \mapsto \lambda$ de N dans $k$ est un homomorphisme de N dans le $\mathfrak{h}$-module trivial $k$. D’après la prop. 9 (iv), il en résulte que $N^0(\mathfrak{h})$ contient un élément de la forme $(a, 1)$ où $a \in M$. Vu l’hypothèse faite sur M, on a
$$
(M \times 0) \cap N^0(\mathfrak{h}) = 0,
$$
donc $N^0(\mathfrak{h})$ est de dimension 1 et par suite est annulé par $\mathfrak{h}$. Ainsi, on a $xa - f(x) = 0$ pour tout $x \in \mathfrak{h}$, ce qui prouve le corollaire.

#### Proposition 10 {#lie-vii-s1-prop-10 .statement tag=00T0}

Soient $g$ une algèbre de Lie, $\mathfrak{h}$ une sous-algèbre nilpotente de $g$. Notons P l’ensemble des applications de $\mathfrak{h}$ dans $k$.

(i) Pour $\lambda, \mu \in P$, on a $[g^\lambda(\mathfrak{h}), g^\mu(\mathfrak{h})] \subset g^{\lambda+\mu}(\mathfrak{h})$; en particulier, $g^0(\mathfrak{h})$ est une sous-algèbre de Lie de $g$ contenant $\mathfrak{h}$, et les $g^\lambda(\mathfrak{h})$ sont stables par ad $g^0(\mathfrak{h})$. De plus, $g^0(\mathfrak{h})$ est son propre normalisateur dans $g$.

(ii) Si M est un $g$-module, on a $g^\lambda(\mathfrak{h})M^\mu(\mathfrak{h}) \subset M^{\lambda+\mu}(\mathfrak{h})$ pour $\lambda, \mu \in P$; en particulier, chaque $M^\lambda(\mathfrak{h})$ est un $g^0(\mathfrak{h})$-module.

(iii) Si B est une forme bilinéaire sur $g$ invariant par $\mathfrak{h}$, $g^\lambda(\mathfrak{h})$ et $g^\mu(\mathfrak{h})$ sont orthogonaux relativement à B pour $\lambda + \mu \neq 0$. Supposons B non dégénérée. Alors, pour tout $\lambda \in P$, la restriction de B à $g^\lambda(\mathfrak{h}) \times g^{-\lambda}(\mathfrak{h})$ est non dégénérée; en particulier, la restriction de B à $g^0(\mathfrak{h}) \times g^0(\mathfrak{h})$ est non dégénérée.

(iv) Supposons k de caractéristique 0. Alors, si $x \in g^\lambda(\mathfrak{h})$ avec $\lambda \neq 0$, ad $x$ est nilpotent.

L’application $(x, y) \mapsto [x, y]$ de $g \times g$ dans $g$ est $g$-invariante d’après l’identité de Jacobi, donc $\mathfrak{h}$-invariante. La première partie de (i) résulte alors de la prop. 2 (ii). On démontre (ii) de manière analogue.

Si $x$ appartient au normalisateur de $g^0(\mathfrak{h})$ dans $g$, on a, pour tout $y \in \mathfrak{h}$,
$$
(\operatorname{ad} y).x = -[x, y] \in g^0(\mathfrak{h}),
$$
donc $(\operatorname{ad} y)^n.x = 0$ pour $n$ assez grand. Cela prouve que $x \in g^0(\mathfrak{h})$. L’assertion (i) est ainsi entièrement établie.

L’assertion (iii) résulte de la prop. 9 (v).

Pour démontrer (iv), on peut supposer $k$ algébriquement clos. Soit $x \in g^\lambda(\mathfrak{h})$, avec $\lambda \neq 0$. Pour tout $\mu \in P$ et tout entier $n \geq 0$, on a $(\mathrm{ad}\,x)^n g^\mu(\mathfrak{h}) \subset g^{\mu+n\lambda}(\mathfrak{h})$; soit $P_1$ l’ensemble fini des $\mu \in P$ tels que $g^\mu(\mathfrak{h}) \neq 0$; si $k$ est de caractéristique 0 et $\lambda \neq 0$, on a $(P_1 + n\lambda) \cap P_1 = \emptyset$ pour $n$ assez grand, d’où $(\mathrm{ad}\,x)^n = 0$.

#### Lemme 2 {#lie-vii-s1-lem-2 .statement tag=00T1}

On suppose $k$ de caractéristique 0. Soient $g$ une algèbre de Lie semi-simple sur $k$, $B$ la forme de Killing de $g$, $m$ une sous-algèbre de $g$. On suppose que les conditions suivantes sont satisfaites:
1) la restriction de $B$ à $m$ est non dégénérée ;
2) si $x \in m$, les composantes semi-simple et nilpotente$^1$ de $x$ dans $g$ appartiennent à $m$.
Alors $m$ est réductive dans $g$ (I, § 6, no 6).

D’après I, § 6, no 4, prop. 5 d), $m$ est réductive. Soit $c$ le centre de $m$. Si $x \in c$ est nilpotent, alors $x = 0$; en effet, pour tout $y \in m$, $\mathrm{ad}\,x$ et $\mathrm{ad}\,y$ commutent, leur composé $\mathrm{ad}\,x \circ \mathrm{ad}\,y$ est nilpotent, et $B(x, y) = 0$, d’où $x = 0$. Soit maintenant $x$ un élément quelconque de $c$; soient $s$ et $n$ ses composantes semi-simple et nilpotente. On a $n \in m$. Comme $\mathrm{ad}\,n$ est de la forme $P(\mathrm{ad}\,x)$, où $P$ est un polynôme sans terme constant, on a $(\mathrm{ad}\,n).m = 0$, donc $n \in c$, et alors $n = 0$ d’après ce qui précède. Donc $\mathrm{ad}\,x$ est semi-simple. Par suite, la restriction à $m$ de la représentation adjointe de $g$ est semi-simple (I, § 6, no 5, th. 4 b)).

#### Proposition 11 {#lie-vii-s1-prop-11 .statement tag=00T2}

On suppose $k$ de caractéristique 0. Soient $g$ une algèbre de Lie semi-simple, $h$ une sous-algèbre nilpotente de $g$. L’algèbre $g^0(h)$ satisfait aux conditions (1) et (2) du lemme 2 ; elle est réductive dans $g$.

Soient $x, x' \in g$, $s$ et $s'$ leurs composantes semi-simples, $n$ et $n'$ leurs composantes nilpotentes. On a
$$
x' \in g^0(x) \Leftrightarrow (\mathrm{ad}\,s)(x') = 0 \quad \text{(prop. 4)}
\Leftrightarrow (\mathrm{ad}\,x')(s) = 0
\Rightarrow (\mathrm{ad}\,s')(s) = 0
\Leftrightarrow (\mathrm{ad}\,s)(s') = 0
\Leftrightarrow s' \in g^0(x) \quad \text{(prop. 4)}
$$
donc $x' \in g^0(x) \Rightarrow n' \in g^0(x)$ et l’on a prouvé (2). La forme de Killing de $g$ est non dégénérée, donc sa restriction à $g^0(h)$ est non dégénérée (prop. 10 (iii)). Le fait que $g^0(h)$ soit réductive dans $g$ résulte alors du lemme 2.

### 4. Décomposition d’une algèbre de Lie relativement à un automorphisme

#### Proposition 12 {#lie-vii-s1-prop-12 .statement tag=00T3}

Soient $g$ une algèbre de Lie, $a$ un automorphisme de $g$.
(i) Pour $\lambda, \mu \in k$, on a $[g^\lambda(a), g^\mu(a)] \subset g^{\lambda\mu}(a)$; en particulier, $g^1(a)$ est une sous-algèbre de $g$.

1 D’après I, § 6, no 3, th. 3, tout $x \in g$ s’écrit de manière unique comme somme d’un élément semi-simple $s$ et d’un élément nilpotent $n$ commutant entre eux ; l’élément $s$ (resp. $n$) s’appelle la composante semi-simple (resp. nilpotente) de $x$.

(ii) Si $B$ est une forme bilinéaire symétrique sur $g$ invariante par $a$, $g^\lambda(a)$ et $g^\mu(a)$ sont orthogonaux relativement à $B$ pour $\lambda \mu \neq 1$. Supposons $B$ non dégénérée. Alors, si $\lambda \neq 0$, la restriction de $B$ à $g^\lambda(a) \times g^{1/\lambda}(a)$ est non dégénérée.

L’assertion (i) et la première moitié de (ii) résultent de la prop. 2 (iii) appliquée à la loi de composition $g \times g \to g$ et à la forme bilinéaire $B$. Pour démontrer la seconde moitié de (ii), on peut supposer $k$ algébriquement clos. On a alors $g = \bigoplus_{v \in k} g^v(a)$. Vu ce qui précède, $g^\lambda(a)$ est orthogonal aux $g^v(a)$ si $\lambda v \neq 1$; comme $B$ est non dégénérée, il en résulte que sa restriction à $g^\lambda(a) \times g^{1/\lambda}(a)$ l’est aussi.

#### Corollaire {#lie-vii-s1-n4-cor-1 .statement tag=00T4}

Supposons $k$ de caractéristique zéro et $g$ semi-simple. Alors la sous-algèbre $g^1(a)$ satisfait aux conditions (1) et (2) du lemme 2; elle est réductive dans $g$.

La condition (1) résulte de la partie (ii) de la prop. 12; la condition (2) résulte de la prop. 4 du n° 1.

### 5. Invariants d’une algèbre de Lie semi-simple relativement à une action semi-simple

Dans ce n°, on suppose $k$ de caractéristique zéro.

#### Proposition 13 {#lie-vii-s1-prop-13 .statement tag=00T5}

Soient $g$ une algèbre de Lie semi-simple, $a$ une sous-algèbre de $g$ réductive dans $g$, et $m$ le commutant de $a$ dans $g$. La sous-algèbre $m$ satisfait aux conditions (1) et (2) du lemme 2 du n° 3; elle est réductive dans $g$.

D’après la prop. 6 de I, § 3, n° 5, appliquée au $a$-module $g$, on a $g = m \oplus [a, g]$. Soit $B$ la forme de Killing de $g$, et soient $x \in a, y \in m, z \in g$. On a
$$
B([z, x], y) = B(z, [x, y]) = 0 \quad \text{puisque } [x, y] = 0,
$$
ce qui montre que $m$ est orthogonal à $[a, g]$ relativement à $B$. Comme $B$ est non dégénérée, et que $g = m \oplus [a, g]$, cela entraîne que la restriction de $B$ à $m$ est non dégénérée; la condition (1) du lemme 2 est donc vérifiée.

Soit maintenant $x \in m$ et soient $s$ et $n$ ses composantes semi-simple et nilpotente. La composante semi-simple de $\operatorname{ad} x$ est $\operatorname{ad} s$, cf. I, § 6, n° 3. Comme $\operatorname{ad} x$ est nul sur $a$, il en est de même de $\operatorname{ad} s$, d’après la prop. 4 (i). On a donc $s \in m$, d’où $n = x - s \in m$, et la condition 2 du lemme 2 est satisfaite.

#### Remarque {#lie-vii-s1-n5-rem-1 .statement tag=00T6}

Le commutant de $m$ dans $g$ n’est pas nécessairement réduit à $a$, cf. Exerc. 4.

#### Proposition 14 {#lie-vii-s1-prop-14 .statement tag=00T7}

Soient $g$ une algèbre de Lie semi-simple, $A$ un groupe et $r$ un homomorphisme de $A$ dans $\operatorname{Aut}(g)$. Soit $m$ la sous-algèbre de $g$ formée des éléments invariants par $r(A)$. Supposons que la représentation linéaire $r$ soit semi-simple. Alors $m$ satisfait aux conditions (1) et (2) du lemme 2 du n° 3; elle est réductive dans $g$.

La démonstration est analogue à celle de la proposition précédente:

Soit $g^+$ le sous-espace vectoriel de $g$ engendré par les $r(a)x - x,\ a \in A,\ x \in g$. L’espace vectoriel $g' = m + g^+$ est stable par $r(A)$. Soit $n$ un supplémentaire de $g'$ dans $g$ stable par $r(A)$. Si $x \in n,\ a \in A$, on a $r(a)x - x \in n \cap g^+ = 0$, d’où $x \in m$ et $x = 0$ puisque $m \cap n = 0$. Ainsi, $g = g' = m + g^+$. Soit B la forme de Killing de $g$ et soient $y \in m,\ a \in A,\ x \in g$. On a

$$
\begin{align*}
B(y, r(a)x - x) &= B(y, r(a)x) - B(y, x) \\
&= B(r(a^{-1})y, x) - B(y, x) \\
&= B(y, x) - B(y, x) = 0.
\end{align*}
$$

Ainsi $m$ et $g^+$ sont orthogonaux relativement à B. Il en résulte que la restriction de B à $m$ est non dégénérée; d’où la condition (1) du lemme 2. La condition (2) est immédiate par transport de structure.

## EXERCICES {#lie-vii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
