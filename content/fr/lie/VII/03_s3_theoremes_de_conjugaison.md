---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: Sous-algèbres de Cartan. Éléments réguliers
section: 3
section_title: Théorèmes de conjugaison
lang: fr
source: lie-vii-viii-fr
pdf_pages: 0020-0027, 0054-0057
extraction: ocr
subsections:
    - "no": 1
      title: Automorphismes élémentaires
      page: 0
      pdf_page: 20
    - "no": 2
      title: Conjugaison des sous-algèbres de Cartan
      page: 0
      pdf_page: 22
    - "no": 3
      title: Applications de la conjugaison
      page: 0
      pdf_page: 23
    - "no": 4
      title: Conjugaison des sous-algèbres de Cartan des algèbres de Lie résolubles
      page: 0
      pdf_page: 25
    - "no": 5
      title: Cas des groupes de Lie
      page: 0
      pdf_page: 26
statements: 17
exercises: 18
content_sha256: 42d5e6ec1bc68c2e4139ceaa466630284080c37badd58933afd6c420c57592d2
---

## § 3. Théorèmes de conjugaison

Dans ce paragraphe, le corps de base k est de caractéristique 0.

### 1. Automorphismes élémentaires

Soit g une algèbre de Lie. Nous noterons Aut(g) le groupe de ses automorphismes. Si $x \in g$ et si $\mathrm{ad}(x)$ est nilpotent, on a $e^{\mathrm{ad}\,x} \in \mathrm{Aut}(g)$ (I, § 6, n° 8).

#### Définition 1 {#lie-vii-s3-def-1 .statement tag=00V0}

On appelle automorphisme élémentaire de g tout produit fini d’automorphismes de g de la forme $e^{\mathrm{ad}\,x}$ avec ad x nilpotent. On note $\mathrm{Aut}_e(g)$ le groupe des automorphismes élémentaires de g.

Si $u \in \mathrm{Aut}(g)$, on a $ue^{\mathrm{ad}\,x}u^{-1} = e^{\mathrm{ad}\,u(x)}$. Il en résulte que $\mathrm{Aut}_e(g)$ est un sous-groupe distingué de $\mathrm{Aut}(g)$. Si $k = \mathbf{R}$ ou $\mathbf{C}$, $\mathrm{Aut}_e(g)$ est contenu dans le groupe Int(g) des automorphismes intérieurs de g (III, § 6, n° 2, déf. 2).

\* Dans le cas général, $\mathrm{Aut}_e(g)$ est contenu dans la composante neutre du groupe algébrique $\mathrm{Aut}(g)$.*

#### Lemme 1 {#lie-vii-s3-lem-1 .statement tag=00V1}

Soient V un espace vectoriel de dimension finie, n une sous-algèbre de Lie de $a = \mathfrak{gl}(V)$ formée d’éléments nilpotents.

(i) L’application $x \mapsto \exp x$ est une bijection de n sur un sous-groupe N de $\mathbf{GL}(V)$ formé d’éléments unipotents (II, § 6, n° 1, remarque 4). On a $n = \log(\exp n)$. L’application $f \mapsto f \circ \log$ est un isomorphisme de l’algèbre des fonctions polynomiales sur n sur l’algèbre des restrictions à N des fonctions polynomiales sur End(V).

(ii) Si $x \in n$ et $a \in a$, on a

$$
(\exp \mathrm{ad}_a x) \cdot a = (\exp x)a(\exp(-x)).
$$

(iii) Soient V’ un espace vectoriel de dimension finie, n’ une sous-algèbre de Lie de $\mathfrak{gl}(V')$ formée d’éléments nilpotents, $\varphi$ un homomorphisme de n dans n’. Soit $\pi$ l’application $\exp x \mapsto \exp \varphi(x)$ de $\exp n$ dans $\exp n'$. Alors $\pi$ est un homomorphisme de groupes.

D’après le th. d’Engel, on peut identifier V à $k^n$ de telle sorte que n soit une sous-algèbre de $n(n, k)$ (sous-algèbre de Lie de $\mathbf{M}_n(k)$ formée des matrices triangulaires inférieures de diagonale nulle). Pour $s \geqslant 0$, soit $n_s(n, k)$ l’ensemble des $(x_{ij})_{l \leq i, j \leq n} \in \mathbf{M}_n(k)$ telles que $x_{ij} = 0$ pour $i - j < s$. Alors

$$
[n_s(n, k), n_{s'}(n, k)] \subset n_{s+s'}(n, k)
$$

(II, § 4, n° 6, remarque), et la série de Hausdorff définit une application polynomiale $(a, b) \mapsto \mathbf{H}(a, b)$ de $n(n, k) \times n(n, k)$ dans $n(n, k)$ (II, § 6, n° 5, remarque 3); muni de cette application, $n(n, k)$ est un groupe (II, § 6, n° 5, prop. 4). D’après II, § 6, n° 1, remarque 4, les applications $x \mapsto \exp x$ de $n(n, k)$ dans $1 + n(n, k)$ et $y \mapsto \log y$ de $1 + n(n, k)$ dans $n(n, k)$ sont des bijections réciproques l’une de l’autre et sont polynomiales; d’après II, § 6, n° 5, prop. 3, ces bijections sont des isomorphismes de groupes si l’on munit $n(n, k)$ de la loi $(a, b) \mapsto \mathbf{H}(a, b)$ et si l’on considère $1 + n(n, k)$ comme sous-groupe de $\mathbf{GL}_n(k)$. Les assertions (i) et (iii) du lemme résultent de là. Soit $x \in n$. Notons $L_x, R_x$ les applications $u \mapsto xu, u \mapsto ux$ de $a$ dans $a$, qui sont permutables et nilpotentes. On a $\operatorname{ad}_a x = L_x - R_x$, donc, pour tout $a \in a$,

$$
\text{(1)} \quad (\exp \operatorname{ad}_a x)a = (\exp(L_x - R_x))a = (\exp L_x)(\exp R_{-x})a
$$
$$
= \sum_{i,j \geq 0} \frac{L_x^i}{i!} \frac{R_{-x}^j}{j!} a = (\exp x)a(\exp(-x)).
$$

Avec les notations du lemme 1, on dit que $\pi$ est la représentation linéaire de $\exp n$ compatible avec la représentation donnée $\rho$ de $n$ dans $V'$. Lorsque $k$ est $\mathbf{R}, \mathbf{C}$, ou un corps ultramétrique complet non discret, on a $\rho = L(\pi)$ d’après les propriétés des applications exponentielles (III, § 4, n° 4, cor. 2 à la prop. 8).

#### Proposition 1 {#lie-vii-s3-prop-1 .statement tag=00V2}

*Soient $g$ une algèbre de Lie, $n$ une sous-algèbre de $g$ telle que $\operatorname{ad}_g x$ soit nilpotent pour tout $x \in n$. Alors $e^{\operatorname{ad}_g n}$ est un sous-groupe de $\operatorname{Aut}_e(g)$*.

Cela résulte aussitôt du lemme 1 (i).

En particulier, si on prend pour $n$ le radical nilpotent de $g$, $e^{\operatorname{ad}_g n}$ est le groupe des automorphismes spéciaux de $g$ (I, § 6, n° 8, déf. 6).

#### Remarque 1 {#lie-vii-s3-n1-rem-1 .statement tag=00V3}

Soient $V$ un espace vectoriel de dimension finie, $g$ une sous-algèbre de Lie de $a = \mathfrak{gl}(V)$, $x$ un élément de $g$ tel que $\operatorname{ad}_g x$ soit nilpotent. Alors il existe un élément nilpotent $n$ de $a$ tel que $\operatorname{ad}_a n$ prolonge $\operatorname{ad}_g x$. En effet, soient $s, n$ les composantes semi-simple et nilpotente de $x$; alors $\operatorname{ad}_a s$ et $\operatorname{ad}_a n$ sont les composantes semi-simple et nilpotente de $\operatorname{ad}_a x$ (I, § 5, n° 4, lemme 2), donc $\operatorname{ad}_a s$ et $\operatorname{ad}_a n$ laissent stables $g$, et $\operatorname{ad}_a s|g, \operatorname{ad}_a n|g$ sont les composantes semi-simple et nilpotente de $\operatorname{ad}_g x$; par suite, $\operatorname{ad}_g x = \operatorname{ad}_a n|g$, ce qui prouve notre assertion. Compte tenu du lemme 1 (ii), on voit que tout automorphisme élémentaire de $g$ se prolonge en un automorphisme de $a$ de la forme $u \mapsto mum^{-1}$ où $m \in \mathbf{GL}(V)$.

#### Remarque 2 {#lie-vii-s3-n1-rem-2 .statement tag=00V4}

Soit $V$ un espace vectoriel de dimension finie. Pour tout $g \in \mathbf{SL}(V)$, notons $\varphi(g)$ l’automorphisme $x \mapsto gxg^{-1}$ de $\mathfrak{gl}(V)$. On a
$$
\operatorname{Aut}_e(\mathfrak{gl}(V)) = \varphi(\mathbf{SL}(V)).
$$
En effet, d’après (1), $\operatorname{Aut}_e(\mathfrak{gl}(V))$ est contenu dans $\varphi(\mathbf{SL}(V))$, et l’inclusion opposée résulte de A, III, p. 104, prop. 17 et de (1). Un argument analogue montre que Aut_e(\mathfrak{sl}(V)) est l’ensemble des restrictions à \mathfrak{sl}(V) des éléments de $\varphi(\mathbf{SL}(V))$.

### 2. Conjugaison des sous-algèbres de Cartan

Soient $g$ une algèbre de Lie, $h$ une sous-algèbre nilpotente de $g$ et $R$ l’ensemble des poids non nuls de $h$ dans $g$, autrement dit l’ensemble des formes linéaires $\lambda \neq 0$ sur $h$ telles que $g^\lambda(h) \neq 0$, cf. § 1, n° 3, prop. 9 (iii). Supposons que
$$
g = g^0(h) \oplus \sum_{\lambda \in R} g^\lambda(h),
$$
ce qui est le cas si $k$ est algébriquement clos ($§ 1$, n° 3, prop. 9 (i)). Pour $\lambda \in R$ et $x \in g^\lambda(h)$, ad $x$ est nilpotent ($§ 1$, n° 3, prop. 10 (iv)). On note $E(h)$ le sous-groupe de $\mathrm{Aut}_e(g)$ engendré par les $e^{\mathrm{ad}\,x}$ où $x$ est de la forme précédente. Si $u \in \mathrm{Aut}(g)$, on a aussitôt $uE(h)u^{-1} = E(u(h))$.

#### Lemme 2 {#lie-vii-s3-lem-2 .statement tag=00V5}

(i) Soit $h_r$ l’ensemble des $x \in h$ tels que $g^0(x) = g^0(h)$; c’est l’ensemble des $x \in h$ tels que $\lambda(x) \neq 0$ pour tout $\lambda \in R$, et $h_r$ est ouvert dense dans $h$ pour la topologie de Zariski.

(ii) Posons $R = \{ \lambda_1, \lambda_2, \ldots, \lambda_p \}$ où les $\lambda_i$ sont deux à deux distincts. Soit $F$ l’application de $g^0(h) \times g^{\lambda_1}(h) \times \cdots \times g^{\lambda_p}(h)$ dans $g$ définie par la formule
$$
F(h, x_1, \ldots, x_p) = e^{\mathrm{ad}\,x_1} \cdots e^{\mathrm{ad}\,x_p} h.
$$
Alors $F$ est une application polynomiale dominante (App. I).

L’assertion (i) est évidente. Prouvons (ii). Soit $n = \dim g$. Si $\lambda \in R$ et $x \in g^\lambda(h)$, on a $(\mathrm{ad}\,x)^n = 0$. Il en résulte que $(y, x) \mapsto e^{\mathrm{ad}\,x} y$ est une application polynomiale de $g \times g^\lambda(h)$ dans $g$; on en déduit par récurrence que $F$ est polynomiale. Soit $h_0 \in h_r$ et soit DF l’application linéaire tangente à $F$ en $(h_0, 0, \ldots, 0)$; montrons que DF est surjective. Pour $h \in g^0(h)$, on a $F(h_0 + h, 0, \ldots, 0) = h_0 + h$, donc $(\mathrm{DF})\ (h, 0, \ldots, 0) = h$ et $\mathrm{Im}(\mathrm{DF}) \supset g^0(h)$. D’autre part, pour $x \in g^{\lambda_1}(h)$, on a
$$
F(h_0, x, 0, \ldots, 0) = e^{\mathrm{ad}\,x} h_0 = h_0 + (\mathrm{ad}\,x).h_0 + \frac{(\mathrm{ad}\,x)^2}{2!} h_0 + \cdots
$$
donc $(\mathrm{DF})\ (0, x, 0, \ldots, 0) = (\mathrm{ad}\,x).h_0 = - (\mathrm{ad}\,h_0)x$; comme $\mathrm{ad}\,h_0$ induit un automorphisme de $g^{\lambda_1}(h)$, on a $\mathrm{Im}(\mathrm{DF}) \supset g^{\lambda_1}(h)$. On voit de même que
$$
\mathrm{Im}(\mathrm{DF}) \supset g^{\lambda_i}(h)
$$
pour tout $i$, d’où la surjectivité de DF. La prop. 4 de l’App. I montre alors que F est dominante.

#### Proposition 2 {#lie-vii-s3-prop-2 .statement tag=00V6}

Supposons $k$ algébriquement clos. Soient $g$ une algèbre de Lie, $h$ et $h'$ des sous-algèbres de Cartan de $g$. Il existe $u \in E(h)$ et $u' \in E(h')$ tels que $u(h) = u'(h')$.

Conservons les notations du lemme 2. Du fait que $\mathfrak{h}$ et $\mathfrak{h}'$ sont des sous-algèbres de Cartan, on a $g^0(\mathfrak{h}) = \mathfrak{h}$ et $g^0(\mathfrak{h}') = \mathfrak{h}'$. D’après le lemme 2 et la prop. 3 de l’App. I, $E(\mathfrak{h})_{\mathfrak{h}_r}$ et $E(\mathfrak{h}')_{\mathfrak{h}'_r}$ contiennent des parties de $g$ qui sont ouvertes et denses pour la topologie de Zariski. On a donc $E(\mathfrak{h})_{\mathfrak{h}_r} \cap E(\mathfrak{h}')_{\mathfrak{h}'_r} \neq \emptyset$. Autrement dit, il existe $u \in E(\mathfrak{h}), \ u' \in E(\mathfrak{h}'), \ h \in \mathfrak{h}_r, \ h' \in \mathfrak{h}'_r$ tels que $u(h) = u'(h')$; on a alors
$$
u(\mathfrak{h}) = u(g^0(\mathfrak{h})) = g^0(u(h)) = g^0(u'(h')) = u'(\mathfrak{h}').
$$

#### Corollaire {#lie-vii-s3-n2-cor-1 .statement tag=00V7}

*On a* $E(\mathfrak{h}) = E(\mathfrak{h}')$.

Soient $u, u'$ comme dans la prop. 2. On a
$$
E(\mathfrak{h}) = uE(\mathfrak{h})u^{-1} = E(u(\mathfrak{h})) = E(u'(\mathfrak{h}')) = u'E(\mathfrak{h}'){u'}^{-1} = E(\mathfrak{h}'),
$$
d’où le corollaire.

En raison de ce résultat, si $k$ est algébriquement clos, nous noterons simplement $E$ le groupe $E(\mathfrak{h})$, où $\mathfrak{h}$ est une sous-algèbre de Cartan de $g$.

En général, $\mathrm{Aut}_e(g) \neq E$ (par exemple, si $g$ est nilpotente, $E$ est réduit à l’élément neutre, tandis qu’il existe des automorphismes élémentaires non triviaux pourvu que $g$ soit non commutative). On peut montrer cependant (VIII, § 10, exerc. 5) que $\mathrm{Aut}_e(g) = E$ pour $g$ semi-simple.

#### Théorème 1 {#lie-vii-s3-thm-1 .statement tag=00V8}

*Supposons k algébriquement clos. Soit g une algèbre de Lie. Le groupe E est distingué dans Aut(g) et opère transitivement sur l’ensemble des sous-algèbres de Cartan de g.*

Soient $\mathfrak{h}$ une sous-algèbre de Cartan de $g$, et $v \in \mathrm{Aut}(g)$. On a
$$
vE(\mathfrak{h})v^{-1} = E(v(\mathfrak{h})) = E(\mathfrak{h}),
$$
donc $E(\mathfrak{h}) = E$ est distingué dans $\mathrm{Aut}(g)$. Si $\mathfrak{h}'$ est une autre sous-algèbre de Cartan de $g$, on a, avec les notations de la prop. 2, ${u'}^{-1}u(\mathfrak{h}) = \mathfrak{h}'$, et ${u'}^{-1}u \in E$.

### 3. Applications de la conjugaison

#### Théorème 2 {#lie-vii-s3-thm-2 .statement tag=00V9}

*Soit g une algèbre de Lie.*

(i) *Les sous-algèbres de Cartan de g ont même dimension, à savoir $\mathrm{rg}(g)$, et même classe de nilpotence.*

(ii) *Pour qu’un élément $x \in g$ soit régulier, il faut et il suffit que $g^0(x)$ soit une sous-algèbre de Cartan de g ; toute sous-algèbre de Cartan s’obtient de cette façon.*

Pour démontrer (i), on peut supposer $k$ algébriquement clos (cf. § 2, prop. 3 et prop. 6), auquel cas cela résulte du th. 1 du n° 2. L’assertion (ii) résulte de (i) et du § 2, th. 1, (i) et (iv).

#### Proposition 3 {#lie-vii-s3-prop-3 .statement tag=00VA}

*Soient g une algèbre de Lie, g’ une sous-algèbre de g. Les conditions suivantes sont équivalentes :*

(i) *g’ contient un élément régulier de g, et $\mathrm{rg}(g) = \mathrm{rg}(g')$;*

(ii) $g'$ contient une sous-algèbre de Cartan de $g$;
(iii) toute sous-algèbre de Cartan de $g'$ est une sous-algèbre de Cartan de $g$.
(i) $\Rightarrow$ (ii): Supposons que $\mathrm{rg}(g) = \mathrm{rg}(g')$, et qu’il existe $x \in g'$ régulier dans $g$. Posons $\mathfrak{h} = g^0(x)$, $\mathfrak{h}' = {g'}^0(x) = \mathfrak{h} \cap g'$. On a
$$
\mathrm{rg}(g') \leq \dim \mathfrak{h}' \leq \dim \mathfrak{h} = \mathrm{rg}(g) = \mathrm{rg}(g')
$$
donc $\mathfrak{h} = \mathfrak{h}' \subset g'$. Cela prouve (ii).

(ii) $\Rightarrow$ (iii): Supposons que $g'$ contienne une sous-algèbre de Cartan $\mathfrak{h}$ de $g$, et soit $\mathfrak{h}_1$ une sous-algèbre de Cartan de $g'$. Pour prouver que $\mathfrak{h}_1$ est une sous-algèbre de Cartan de $g$, on peut supposer $k$ algébriquement clos. Soient alors $E(\mathfrak{h})$ et $E'(\mathfrak{h})$ les groupes d’automorphismes de $g$ et $g'$ associés à $\mathfrak{h}$ (n° 2). D’après le th. 1, il existe $f \in E'(\mathfrak{h})$ tel que $f(\mathfrak{h}) = \mathfrak{h}_1$. Or tout élément de $E'(\mathfrak{h})$ est induit par un élément de $E(\mathfrak{h})$; en effet, il suffit de le vérifier pour $e^{\mathrm{ad}\, x}$, avec $x \in {g'}^\lambda(\mathfrak{h})$, $\lambda \neq 0$, auquel cas cela résulte de l’inclusion ${g'}^\lambda(\mathfrak{h}) \subset g^\lambda(\mathfrak{h})$. Donc $\mathfrak{h}_1$ est une sous-algèbre de Cartan de $g$.

(iii) $\Rightarrow$ (i): Supposons la condition (iii) vérifiée. Soit $\mathfrak{h}$ une sous-algèbre de Cartan de $g'$. Comme c’est une sous-algèbre de Cartan de $g$, elle contient un élément régulier de $g$ (th. 2 (ii)), et d’autre part $\mathrm{rg}(g) = \dim(\mathfrak{h}) = \mathrm{rg}(g')$.

#### Corollaire {#lie-vii-s3-n3-cor-1 .statement tag=00VB}

*Soit $\mathfrak{h}$ une sous-algèbre nilpotente de $g$. La sous-algèbre $g^0(\mathfrak{h})$ possède les propriétés (i), (ii), (iii) de la prop. 3.*
En effet, la prop. 11 du § 2, n° 3, montre que $g^0(\mathfrak{h})$ possède la propriété (ii).

#### Proposition 4 {#lie-vii-s3-prop-4 .statement tag=00VC}

*Soient $g$ une algèbre de Lie, $l$ le rang de $g$, $c$ la classe de nilpotence des sous-algèbres de Cartan de $g$, et $x \in g$. Il existe une sous-algèbre de $g$ de dimension $l$, dont la classe de nilpotence est $\leq c$, et qui contient $x$*.
Soit T une indéterminée. Soient $k' = k(T)$ et $g' = g \otimes_k k'$. Si $\mathfrak{h}$ est une sous-algèbre de Cartan de $g$, $\mathfrak{h} \otimes_k k'$ est une sous-algèbre de Cartan de $g'$, donc le rang de $g'$ est $l$ et la classe de nilpotence de toute sous-algèbre de Cartan de $g'$ est $c$.
Choisissons un élément régulier $y$ de $g$. Avec les notations du § 2, n° 2, on a $a_l(y) \neq 0$. Notons encore $a_l$ la fonction polynomiale sur $g'$ qui prolonge $a_l$. Alors l’élément $a_l(x + Ty)$ de $k[T]$ admet $a_l(y)$ pour coefficient dominant. En particulier, $x + Ty$ est régulier dans $g'$. Soit $\mathfrak{h}'$ le nilspace de $\mathrm{ad}(x + Ty)$ dans $g'$. Alors $\dim \mathfrak{h}' = l$ et la classe de nilpotence de $\mathfrak{h}'$ est $c$. Posons $\mathfrak{k} = \mathfrak{h}' \cap (g \otimes_k k[T])$; on a $\mathfrak{k} \otimes_{k[T]} k(T) = \mathfrak{h}'$.
Soit $\varphi$ l’homomorphisme de $k[T]$ sur $k$ tel que $\varphi(T) = 0$, et soit $\psi$ l’homomorphisme $1 \otimes \varphi$ de $g \otimes_k k[T]$ sur $g$. Alors $\psi(\mathfrak{k})$ est une sous-algèbre de $g$, dont la classe de nilpotence est $\leq c$, et qui contient $\psi(x + Ty) = x$.
Dans le $k[T]$-module libre $g \otimes_k k[T]$, $\mathfrak{k}$ est un sous-module de rang $l$, et $(g \otimes_k k[T])/\mathfrak{k}$ est sans torsion, de sorte que $\mathfrak{k}$ est un sous-module facteur direct dans $g \otimes_k k[T]$ (A, VII, § 4, n° 2, th. 1). Donc $\dim_k \psi(\mathfrak{k}) = l$, ce qui achève la démonstration.

### 4. Conjugaison des sous-algèbres de Cartan des algèbres de Lie résolubles

Soit $g$ une algèbre de Lie résoluble. Notons $\mathcal{C}^\infty(g)$ l’intersection des termes de la série centrale descendante de $g$ (I, § 1, n° 5). C’est un idéal caractéristique de $g$, et c’est le plus petit idéal $m$ de $g$ tel que $g/m$ soit nilpotente. Comme $\mathcal{C}^\infty(g) \subset [g, g]$, $\mathcal{C}^\infty(g)$ est un idéal nilpotent de $g$ (I, § 5, n° 3, cor. 5 au th. 1). D’après la prop. 1 du n° 1, l’ensemble des $e^{\mathrm{ad}\, x}$, pour $x \in \mathcal{C}^\infty(g)$, est un sous-groupe de $\mathrm{Aut}(g)$, contenu dans le groupe des automorphismes spéciaux (I, § 6, n° 8, déf. 6).

#### Théorème 3 {#lie-vii-s3-thm-3 .statement tag=00VD}

Soit $g$ une algèbre de Lie résoluble, et soient $h, h'$ des sous-algèbres de Cartan de $g$. Il existe $x \in \mathcal{C}^\infty(g)$ tel que $e^{\mathrm{ad}\, x}h = h'$.

Raisonnons par récurrence sur $\dim g$, le cas où $g = 0$ étant trivial. Soit $n$ un idéal commutatif non nul minimal de $g$. Soit $\varphi : g \to g/n$ le morphisme canonique. On a $\varphi(\mathcal{C}^\infty g) = \mathcal{C}^\infty(g/n)$ (I, § 1, n° 5, prop. 4). Puisque $\varphi(h)$ et $\varphi(h')$ sont des sous-algèbres de Cartan de $g/n$ ($§ 2$, n° 1, cor. 2 de la prop. 4), il existe, d’après l’hypothèse de récurrence, un $x \in \mathcal{C}^\infty(g)$ tel que $e^{\mathrm{ad}\, \varphi(x)}\varphi(h) = \varphi(h')$. Quitte à remplacer $h$ par $e^{\mathrm{ad}\, x}h$, on peut donc supposer $\varphi(h) = \varphi(h')$, c’est-à-dire

$$
h + n = h' + n.
$$

Alors $h$ et $h'$ sont des sous-algèbres de Cartan de $h + n$. Si $h + n \neq g$, l’assertion à démontrer résulte de l’hypothèse de récurrence. Nous supposerons donc désormais que $h + n = h' + n = g$.

D’après la minimalité de $n$, on a $[g, n] = \{0\}$ ou $[g, n] = n$. Si $[g, n] = \{0\}$, alors $n \subset h$ et $n \subset h'$ ($§ 2$, n° 1, prop. 5), donc $h = h + n = h' + n = h'$. Reste à considérer le cas où $[g, n] = n$, d’où $n \subset \mathcal{C}^\infty(g)$. L’idéal $n$ est un $g$-module simple; comme $g = h + n$, et que $[n, n] = \{0\}$, il en résulte que $n$ est un $h$-module simple. Si $h \cap n \neq \{0\}$, on a donc $n \subset h$, d’où $g = h$ et $h' = h$. Supposons maintenant que $h \cap n = \{0\}$. On a $g = h \oplus n$ et par suite $g = h' \oplus n$, puisque $h$ et $h'$ ont même dimension.

Pour tout $x \in h$, soit $f(x)$ l’unique élément de $n$ tel que $x - f(x) \in h'$; si $x, y \in h$, on a

$$
[x, y] - [x, f(y)] - [f(x), y] = [x - f(x), y - f(y)] \in h',
$$

donc $f([x, y]) = [x, f(y)] + [f(x), y]$. D’après le § 1, n° 3, cor. de la prop. 9, il existe $a \in n$ tel que $f(x) = [x, a]$ pour tout $x \in h$. On a $(\mathrm{ad}\, a)^2(g) \subset (\mathrm{ad}\, a)(n) = 0$, donc, pour tout $x \in h$,

$$
e^{\mathrm{ad}\, a}x = x + [a, x] = x - f(x).
$$

On voit que $e^{\mathrm{ad}\, a}(h) = h'$. Comme $a \in \mathcal{C}^\infty(g)$, cela achève la démonstration.

#### Lemme 3 {#lie-vii-s3-lem-3 .statement tag=00VE}

Soient $g$ une algèbre de Lie, $r$ son radical, $\varphi$ l’homomorphisme canonique de $g$ sur $g/r$, $v$ un automorphisme élémentaire de $g/r$. Il existe un automorphisme élémentaire $u$ de $g$ tel que $\varphi \circ u = v \circ \varphi$.

On peut supposer que $v$ est de la forme $e^{a d b}$, où $b \in g/r$ et $ad\ b$ est nilpotent. Soit $s$ une sous-algèbre de Levi de $g$ (I, § 6, n° 8, déf. 7) et soit $a$ l’élément de $s$ tel que $\varphi(a) = b$. Comme $ad_s\ a$ est nilpotent, $ad_g\ a$ est nilpotent (I, § 6, n° 3, cor. de la prop. 3), et $u = e^{ad_g\ a}$ est un automorphisme élémentaire de $g$ tel que $\varphi \circ u = v \circ \varphi$.

#### Proposition 5 {#lie-vii-s3-prop-5 .statement tag=00VF}

*Soient $g$ une algèbre de Lie, $r$ son radical, $h$ et $h'$ des sous-algèbres de Cartan de $g$, et $\varphi$ l’homomorphisme canonique de $g$ sur $g/r$. Les conditions suivantes sont équivalentes*:

(i) $h$ et $h'$ sont conjuguées par un automorphisme élémentaire de $g$;
(ii) $\varphi(h)$ et $\varphi(h')$ sont conjuguées par un automorphisme élémentaire de $g/r$.
(i) $\Rightarrow$ (ii): C’est évident.
(ii) $\Rightarrow$ (i): Supposons la condition (ii) vérifiée, et prouvons (i). Grâce au lemme 3, on se ramène au cas où $\varphi(h) = \varphi(h')$. Posons $k = h + r = h' + r$, qui est une sous-algèbre résoluble de $g$. Alors $h$ et $h'$ sont des sous-algèbres de Cartan de $k$, donc il existe $x \in \mathcal{C}^\infty(k)$ tel que $e^{ad_k\ x}h = h'$ (th. 3). Comme $k/r$ est nilpotente, on a $\mathcal{C}^\infty(k) \subset r$; d’autre part, $\mathcal{C}^\infty k \subset [k, k] \subset [g, g]$, d’où $x \in r \cap [g, g]$; d’après I, § 5, n° 3, th. 1, $ad_g\ x$ est nilpotent, donc $e^{ad_g\ x}$ est un automorphisme élémentaire de $g$ transformant $h$ en $h'$.

### 5. Cas des groupes de Lie

#### Proposition 6 {#lie-vii-s3-prop-6 .statement tag=00VG}

*Supposons que $k$ soit $\mathbf{R}$, ou $\mathbf{C}$, ou un corps ultramétrique complet non discret de caractéristique 0. Soient $G$ un groupe de Lie de dimension finie sur $k$, $e$ son élément neutre, $g$ son algèbre de Lie, $h$ une sous-algèbre de Cartan de $g$, $h_r$ l’ensemble des éléments réguliers de $g$ appartenant à $h$*.

(i) *Soient $s$ un sous-espace vectoriel supplémentaire de $h$ dans $g$, $s_0$ un voisinage de 0 dans $s$ dans lequel une application exponentielle est définie, et $h_0 \in h_r$. L’application $(s, h) \mapsto F(s, h) = (\exp ad\ s)\cdot h$ de $s_0 \times h$ dans $g$ est étale en $(0, h_0)$.
(ii) *L’application $(g, h) \mapsto F'(g, h) = (\mathrm{Ad}\ g)\cdot h$ de $G \times h_r$ dans $g$ est une submersion. En particulier, son image $\Omega$ est ouverte. Pour tout $x \in \Omega, g^0(x)$ est une sous-algèbre de Cartan de $g$ conjuguée de $h$ par $\mathrm{Ad}(G)$.
(iii) *Soit $h_0 \in h_r$. Pour tout voisinage $U$ de $e$ dans $G$, l’ensemble $\bigcup_{a \in U} (\mathrm{Ad}\ a)(h_r)$ est un voisinage de $h_0$ dans $g$.

Soient $h_0$ et $s$ comme dans (i). Soit $T$ l’application linéaire tangente à $F$ en $(0, h_0)$. On a $F(0, h) = h$ pour tout $h \in h$, donc $T(0, h) = h$ pour tout $h \in h$. D’autre part, pour $s_0$ assez petit, l’application $s \mapsto \exp ad\ s$ de $s_0$ dans $\mathrm{End}(g)$ a pour application tangente en 0 l’application $s \mapsto ad\ s$ de $s$ dans $\mathrm{End}(g)$. Donc $T(s, 0) = [s, h_0]$ pour tout $s \in s$. Or l’application de $g/h$ dans $g/h$ déduite de $ad\ h_0$ par passage au quotient est bijective. On en déduit que $T$ est bijective, d’où (i). Comme $\exp ad\ s = \mathrm{Ad}\ \exp s$ pour tout $s \in s$ assez voisin de 0, on en déduit (iii), et la première assertion de (ii). Tout $x \in \Omega$ est de la forme $(\mathrm{Ad}\, a)\,(h)$ avec $a \in G$ et $h \in \mathfrak{h}_r$, donc $g^0(x) = (\mathrm{Ad}\, a)(g^0(h)) = (\mathrm{Ad}\, a)\,(\mathfrak{h})$ est une sous-algèbre de $\mathfrak{g}$ conjuguée de $\mathfrak{h}$ par $\mathrm{Ad}(G)$.

## EXERCICES {#lie-vii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
