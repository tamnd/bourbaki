---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: GROUPES DE LIE
section: 7
section_title: Groupes de Lie sur un corps ultramétrique
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0212-0223, 0270-0272
extraction: ocr
subsections:
    - "no": 1
      title: Passage des algèbres de Lie aux groupes de Lie
      page: 0
      pdf_page: 212
    - "no": 2
      title: Applications exponentielles
      page: 0
      pdf_page: 214
    - "no": 3
      title: Groupes standard¹
      page: 0
      pdf_page: 214
    - "no": 4
      title: Filtration des groupes standard
      page: 0
      pdf_page: 216
    - "no": 5
      title: Puissances dans les groupes standard
      page: 0
      pdf_page: 217
    - "no": 6
      title: Application logarithme
      page: 0
      pdf_page: 219
statements: 26
exercises: 10
content_sha256: 0267354d0f0076d5e121f08b9c07f55051a80af3273931457acfca54c73ff5f2
---

## § 7. Groupes de Lie sur un corps ultramétrique

Dans ce paragraphe, le corps valué $K$ est supposé ultramétrique et de caractéristique 0. On note $A$ l’anneau de valuation de $K$, $m$ l’idéal maximal de $A$, $p$ la caractéristique du corps résiduel $A/m$. Si $K$ est localement compact, on a $p \neq 0$ (AC, VI, § 9, th. 1).

### 1. Passage des algèbres de Lie aux groupes de Lie

#### Proposition 1 {#lie-iii-s7-prop-1 .statement}

*Soit* $G$ *un groupuscule de Lie d’élément neutre* $e$. *Il existe un système fondamental de voisinages ouverts de* $e$ *dans* $G$ *formé des sous-groupes de Lie de* $G$.

#### Théorème 1 {#lie-iii-s7-thm-1 .statement}

*Soit $L$ une algèbre de Lie normable complète. Il existe un groupe de Lie $G$ tel que $L(G)$ soit isomorphe à $L$. Deux tels groupes sont localement isomorphes.*
La première assertion a été prouvée au § 4, no 2, lemme 3. La deuxième est un cas particulier du § 4, no 2, th. 2.

#### Théorème 2 {#lie-iii-s7-thm-2 .statement}

*Soient $G$ un groupe de Lie, $\mathfrak{h}$ une sous-algèbre de Lie de $L(G)$ admettant un supplémentaire topologique. Il existe un sous-groupe de Lie $H$ de $G$ tel que $L(H) = \mathfrak{h}$. Si $H_1$ et $H_2$ sont des sous-groupes de Lie de $G$ tels que $L(H_1) = L(H_2) = \mathfrak{h}$, alors $H_1 \cap H_2$ est ouvert dans $H_1$ et $H_2$.*
La première assertion résulte de la prop. 1, et du § 4, no 2, th. 3. La deuxième est un cas particulier du § 4, no 2, th. 3.

#### Théorème 3 {#lie-iii-s7-thm-3 .statement}

*Soient $G$ et $H$ des groupes de Lie, $\mathfrak{h}$ un morphisme continu de $L(G)$ dans $L(H)$.*
(i) *Il existe un sous-groupe ouvert $G'$ de $G$ et un morphisme de groupes de Lie $\varphi$ de $G'$ dans $H$ tel que $h = L(\varphi)$.*
(ii) *Soient $G_1, G_2$ des sous-groupes ouverts de $G$, et $\varphi_i$ un morphisme de $G_i$ dans $H$ tel que $h = L(\varphi_i)$. Alors $\varphi_1$ et $\varphi_2$ coïncident dans un sous-groupe ouvert de $G$.*
Compte tenu de la prop. 1, cela résulte du § 4, no 1, th. 1.

#### Proposition 2 {#lie-iii-s7-prop-2 .statement}

*Soient $G$ un groupe de Lie, $\mathfrak{h}$ une sous-algèbre de Lie de $L(G)$ admettant un supplémentaire topologique. Les conditions suivantes sont équivalentes:*
(i) *Il existe un sous-groupe ouvert $G'$ de $G$ et un sous-groupe de Lie distingué $H$ de $G'$ tels que $L(H) = \mathfrak{h}$.*
(ii) *$\mathfrak{h}$ est un idéal de $L(H)$.*
S’il existe $G'$ et $H$ ayant les propriétés de (i), on a $L(G') = L(G)$, et $L(H)$ est un idéal de $L(G')$ d’après le § 3, no 12, prop. 47.
Supposons que $\mathfrak{h}$ soit un idéal de $L(G)$. Il existe un groupe de Lie $F$ tel que $L(F) = L(G)/\mathfrak{h}$ (th. 1). Soit $h$ le morphisme canonique de $L(G)$ sur $L(F)$. D’après le th. 3 (i), il existe un sous-groupe ouvert $G'$ de $G$ et un morphisme de groupes de Lie $\varphi$ de $G'$ dans $F$ tel que $L(\varphi) = h$. D’après le § 3, no 8, le noyau $H$ de $\varphi$ est un sous-groupe de Lie de $G'$, et $L(H) = \mathrm{Ker}\ L(\varphi) = \mathrm{Ker}\ h = \mathfrak{h}$. Enfin, $H$ est distingué dans $G'$ puisque $H = \mathrm{Ker}\ \varphi$.

### 2. Applications exponentielles

#### Proposition 3 {#lie-iii-s7-prop-3 .statement}

Soit G un groupe de Lie. Il existe une application exponentielle φ de G ayant les propriétés suivantes:
(i) φ est définie dans un sous-groupe ouvert U du groupe additif L(G);
(ii) φ(U) est un sous-groupe ouvert de G, et φ est un isomorphisme de la variété analytique U sur la variété analytique φ(U);
(iii) φ(nx) = φ(x)^n pour tout x ∈ U et tout n ∈ \mathbf{Z}.

Munissons L(G) d’une norme compatible avec sa topologie et telle que $\| [x, y] \| \leq \| x \| \| y \|$ pour x, y dans L(G). Soit G_1 le groupe de Lie défini par L(G). Soit ψ = Id_{G_1}, qui est une application exponentielle de G_1. Pour tout μ > 0, soit L_μ l’ensemble des x ∈ L(G) tels que $\| x \| < μ$. Alors, pour μ assez petit, L_μ est un sous-groupe ouvert du groupe additif L(G), ψ(L_μ) est un sous-groupe ouvert de G_1 (\S 4, n° 2, lemme 3), ψ|L_μ est un isomorphisme de variétés analytiques de L_μ sur ψ(L_μ), et ψ(nx) = ψ(x)^n pour tout x ∈ L_μ et tout n ∈ \mathbf{Z}. Les L_μ forment un système fondamental de voisinages de 0 dans L(G). D’après le th. 1, il existe un μ et un sous-groupe ouvert G' de G tels que ψ(L_μ) et G' soient isomorphes, d’où la proposition.

#### Proposition 4 {#lie-iii-s7-prop-4 .statement}

Soient G un groupe de Lie, φ une application exponentielle injective de G. Supposons p > 0. Quels que soient x, y dans L(G), on a
(1)
$$
x + y = \lim_{n \to + \infty} p^{-n} \varphi^{-1}(\varphi(p^n x) \varphi(p^n y))
$$
(2)
$$
[x, y] = \lim_{n \to + \infty} p^{-2n} \varphi^{-1}(\varphi(p^n x) \varphi(p^n y) \varphi(-p^n x) \varphi(-p^n y)).
$$

Ce sont des cas particuliers de la prop. 4 du \S 4, n° 3.

### 3. Groupes standard¹

Si S(X_1, X_2, \ldots, X_n) est une série formelle à coefficients dans A, alors, quels que soient x_1, \ldots, x_r dans m, la série S(x_1, x_2, \ldots, x_r) est convergente. Plus précisément, m × m × \cdots × m est contenu dans le domaine de convergence stricte de S (VAR, R, 4.1.3).

#### Définition 1 {#lie-iii-s7-def-1 .statement}

Soit r un entier $\geq 0$. On appelle groupe standard de dimension r sur K un groupe de Lie G possédant les propriétés suivantes:
(i) la variété analytique sous-jacente de G est m × m × \cdots × m (r facteurs);
(ii) il existe une série formelle F en 2r variables, à coefficients dans A^r, sans terme constant, telle que x . y = F(x, y) quels que soient x, y dans G.

¹ Les résultats des n°s 3 et 4 et leurs démonstrations restent valables lorsque la caractéristique de K est > 0.

On a alors $0.0 = 0$, donc l’élément neutre de $G$ est l’origine de $m \times \cdots \times m$.

On identifiera $L(G)$ à $K^r$. D’après le § 5, formule (13), les constantes de structure de $L(G)$ par rapport à la base canonique appartiennent à $A$. Il nous arrivera, dans une même démonstration, de considérer les éléments de $m \times \cdots \times m$, tantôt comme des éléments de $G$, tantôt comme des éléments de $L(G)$.

#### Exemple {#lie-iii-s7-n3-exa-1 .statement}

Soit $G = 1 + \mathbf{M}_n(m)$, qui est une partie ouverte de $\mathbf{M}_n(K)$. Si $x \in G$, on a $\det x \in 1 + m$, donc $G \subset \mathbf{GL}(n, K)$. Il est clair que $GG \subset G$. Si $x = 1 + y$ avec $y \in \mathbf{M}_n(m)$, le calcul de l’inverse d’une matrice prouve d’abord que $x^{-1} \in \mathbf{M}_n(A)$; si l’on pose $x^{-1} = 1 + y'$, on a $y + y' + yy' = 0$, donc $y' \in \mathbf{M}_n(m)$, et par suite $x^{-1} \in G$. Ainsi, $G$ est un sous-groupe ouvert de $\mathbf{GL}(n, K)$. Identifions $G$ à $m^{n^2}$ grâce à l’application $(\delta_{ij} + y_{ij}) \mapsto (y_{ij})$. Il est clair que $G$ est un groupe standard.

#### Théorème 4 {#lie-iii-s7-thm-4 .statement}

*Soit $G$ un groupe de Lie de dimension finie. Il existe un sous-groupe ouvert de $G$ isomorphe à un groupe standard.*

En remplaçant $G$ par un groupe isomorphe à un sous-groupe ouvert de $G$, on se ramène au cas où $G$ est une partie ouverte de $K^r$, d’élément neutre $0$, et où les coordonnées du produit $x.y$ et de l’inverse $x^{[−1]}$ sont données par des formules

$$
(x.y)_i = x_i + y_i + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c_{\alpha \beta i} x^\alpha y^\beta \quad (i = 1, 2, \ldots, r)
$$

$$
(x^{[−1]})_i = -x_i + \sum_{|\alpha| > 1} d_{\alpha i} x^\alpha \quad (i = 2, 2, \ldots, r)
$$

les séries des seconds membres étant convergentes pour $x, y$ dans $G$ (\S 5, n° 1). Soit $\lambda \in K^*$, et transportons la loi de groupe de $G$ à $G' = \lambda G$ par l’homothétie de rapport $\lambda$. Pour $x', y'$ dans $G'$, le produit $x'.y'$ et l’inverse ${x'}^{[−1]}$ calculés dans $G'$ ont pour coordonnées

$$
(x'.y')_i = x'_i + y'_i + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c'_{\alpha \beta i} {x'}^\alpha {y'}^\beta \quad (i = 1, 2, \ldots, r)
$$

$$
({x'}^{[−1]})_i = -x'_i + \sum_{|\alpha| > 1} d'_{\alpha i} {x'}^\alpha \quad (i = 1, 2, \ldots, r)
$$

avec

$$
c'_{\alpha \beta i} = \lambda^{-|\alpha|-|\beta|+1} c_{\alpha \beta i}, \quad d'_{\alpha i} = \lambda^{-|\alpha|+1} d_{\alpha i}.
$$

Comme les séries (3) et (4) sont convergentes, on voit que, pour $|\lambda|$ assez grand, on a, quels que soient $\alpha, \beta, i$,

$$
|c'_{\alpha \beta i}| \leq 1, \quad |d'_{\alpha i}| \leq 1
$$

c’est-à-dire $c'_{\alpha \beta i} \in A$ et $d'_{\alpha i} \in A$; et d’autre part $G' \supset m \times m \times \cdots \times m$. Alors $m \times m \times \cdots \times m$ est un sous-groupe ouvert de $G'$, et est un groupe standard.

### 4. Filtration des groupes standard

On reprend les notations de la déf. 1. Choisissons un nombre $a > 1$ et une valuation réelle $v$ de $\mathbf{K}$ telle que $|x| = a^{-v(x)}$ pour tout $x \in \mathbf{K}$ (AC, VI, § 6, prop. 3). Si $a$ est un idéal non nul (donc ouvert) de $\mathbf{A}$ contenu dans $m$, on note $G(a)$ l’ensemble des éléments de $G$ dont les coordonnées appartiennent à $a$. Si $\lambda \in \mathbf{R}$, on note $a_\lambda$ (resp. $a_\lambda^+$) l’ensemble des $x \in \mathbf{K}$ tels que $v(x) \geq \lambda$ (resp. $v(x) > \lambda$) ; on a $a_0 = \mathbf{A}, a_0^+ = m$. Pour $x = (x_1, \ldots, x_r) \in G$, nous poserons
$$
\omega(x) = \inf (v(x_1), \ldots, v(x_r)).
$$

#### Proposition 5 {#lie-iii-s7-prop-5 .statement}

Soit $G$ un groupe standard.

(i) Si $a$ est un idéal non nul de $\mathbf{A}$ contenu dans $m$, $G(a)$ est un sous-groupe distingué ouvert de $G$.

(ii) Les $G(a_\lambda)$, pour $\lambda > 0$, forment un système fondamental de voisinages de $e$ dans $G$.

(iii) Supposons $a_\lambda \subset a$ pour $\lambda \geq \lambda_0$, et munissons les $G(a)/G(a_\lambda)$, pour $\lambda \geq \lambda_0$, de la topologie discrète. Alors le groupe topologique $G(a)$ est limite projective des groupes $G(a)/G(a_\lambda)$.

(iv) Soient $a, b$ des idéaux non nuls de $\mathbf{A}$ contenus dans $m$, tels que $a \supset b \supset a^2$. L’application $x \mapsto (x_1 \mod b, \ldots, x_r \mod b)$ de $G(a)$ dans $(a/b) \times \cdots \times (a/b)$ définit par passage au quotient un isomorphisme du groupe $G(a)/G(b)$ sur le groupe additif $(a/b) \times \cdots \times (a/b)$.

Si $x \in G$ et $y \in G(a)$, les coordonnées de $x$ et de $x.y$ sont égales modulo $a$. Donc, pour $x', x''$ dans $G$ et $y', y''$ dans $G(a)$, les coordonnées de $x'.x''$ et de $(x'.y').(x''.y'')$ sont égales modulo $a$. Cela prouve (i).

(ii) est évident.

(iii) résulte de ce qui précède et de TG, III, § 7, prop. 2.

Si $x \in G(a)$ et $y \in G(a)$, les coordonnées de $x.y$ sont congrues à celles de $x + y$ modulo $G(a^2)$ d’après la formule (4) du § 5. Cela prouve (iv).

#### Corollaire {#lie-iii-s7-n4-cor-1 .statement}

Supposons $\mathbf{K}$ localement compact et soit $q = \mathrm{Card} (\mathbf{A}/m)$.

(i) Si $a = m^a$ et $b = m^b$ avec $b \geq a \geq 1$, $G(a)/G(b)$ est un $p$-groupe de cardinal $q^{r(b-a)}$.

(ii) $G(a)$ est limite projective de $p$-groupes.

Le nombre d’éléments de $G(a)/G(b)$ est $(\mathrm{Card}(a/b))^r$; si $b = a + 1$, $a/b$ est un espace vectoriel de dimension 1 sur $\mathbf{A}/m$, d’où (i) dans ce cas; le cas général s’en déduit par récurrence sur $b - a$. L’assertion (ii) résulte de (i) et de la prop. 5 (iii).

#### Proposition 6 {#lie-iii-s7-prop-6 .statement}

Soient $a, b, c, c'$ des idéaux non nuls de $\mathbf{A}$ contenus dans $m$ tels que
$$
c' \subset c, \quad ab \subset c, \quad ab^2 \subset c', \quad a^2b \subset c'.
$$
Si $x \in G(a)$ et $y \in G(b)$, alors $x^{[-1]} . y^{[-1]} . x.y, \quad x.y . x^{[-1]} . y^{[-1]}, \quad [x, y]$ appartiennent à $G(c)$ et sont congrus modulo $G(c')$.

D’après le § 5, n° 2, prop. 1, il existe des $c_{\alpha \beta} \in A^r$ tels que
$$
x^{[-1]}.y^{[-1]}.x.y - [x,y] = \sum_{|\alpha| + |\beta| \geq 3} c_{\alpha \beta} x^{\alpha} y^{\beta}.
$$
Si $x = 0$, ou si $y = 0$, on a $x^{[-1]}.y^{[-1]}.x.y - [x,y] = 0$; donc $c_{0 \beta} = c_{\alpha 0} = 0$.
D’autre part, les conditions
$$
x \in G(a), \quad y \in G(b), \quad |\alpha| \geq 1, \quad |\beta| \geq 1, \quad |\alpha| + |\beta| \geq 3
$$
impliquent
$$
c_{\alpha \beta} x^{\alpha} y^{\beta} \in G(a^2 b + ab^2) \subset G(c')
$$
donc $x^{[-1]}.y^{[-1]}.x.y - [x,y] \in G(c')$. On voit de même que
$$
x.y.x^{[-1]}.y^{[-1]} - [x,y] \in G(c').
$$
Enfin, d’après le § 5, formule (13), on a $[x,y] \in G(ab) \subset G(c)$. C.Q.F.D.

#### Proposition 7 {#lie-iii-s7-prop-7 .statement}

(i) *La famille* $(G(a_{\lambda}))$ *est une filtration centrale sur* $G$ (chap. II, § 4, n° 4, déf. 2).
(ii) *Pour* $\lambda \in \mathbf{R}_+^*$, *on a* $G(a_{\lambda}) = \{ x \in G | \omega(x) \geq \lambda \}$, $G(a_{\lambda}^+) = \{ x \in G | \omega(x) > \lambda \}$.
(ii) est évident. Prouvons (i). Il est clair que $G(a_{\lambda}) = \bigcap_{\mu < \lambda} G(a_{\mu})$ et que $G = \bigcup_{\lambda > 0} G(a_{\lambda})$. D’autre part, si $x \in G(a_{\lambda})$ et $y \in G(a_{\mu})$, on a
$$
x^{[-1]}.y^{[-1]}.x.y \in G(a_{\lambda+\mu})
$$
d’après la prop. 6 appliquée avec $a = a_{\lambda}, b = a_{\mu}, c = c' = a_{\lambda+\mu}$.

D’après le chap. II, § 4, n° 4, on peut former le groupe gr(G) associé au groupe G muni de la filtration centrale $(G(a_{\lambda}))$. Posant $G_{\lambda} = G(a_{\lambda})/G(a_{\lambda}^+)$ pour tout $\lambda > 0$, on a $\mathrm{gr}(G) = \bigoplus_{\lambda > 0} G_{\lambda}$. Rappelons (*loc. cit.*, prop. 1) que le commutateur dans G permet de définir un crochet dans gr(G) pour lequel gr(G) est une algèbre de Lie, de la manière suivante: si $\bar{x} \in G_{\lambda}$ et $\bar{y} \in G_{\mu}$, on choisit un représentant $x$ de $\bar{x}$ dans $G(a_{\lambda})$ et un représentant $y$ de $\bar{y}$ dans $G(a_{\mu})$; alors $[\bar{x}, \bar{y}]$ est la classe de $x^{[-1]}.y^{[-1]}.x.y \in G(a_{\lambda+\mu})$ dans $G_{\lambda+\mu}$. D’après la prop. 6, appliquée avec $a = a_{\lambda}, b = a_{\mu}, c = a_{\lambda+\mu}, c' = a_{\lambda+\mu}^+$, on voit que $[\bar{x}, \bar{y}]$ est aussi la classe de $[x, y]$ dans $G_{\lambda+\mu}$. Ainsi, lorsqu’on considère G comme une sous-algèbre de Lie de $L(G) = K^r$, filtrée par les $G(a_{\lambda})$, l’algèbre de Lie graduée associée (chap. II, § 4, n° 3) est égale à gr(G).

### 5. Puissances dans les groupes standard

On conserve les notations du n° 4.

#### Proposition 8 {#lie-iii-s7-prop-8 .statement}

Soient $n \in \mathbf{Z}$, et $h_n$ l’application $x \mapsto x^n$ de G dans G. Soit $a$ un idéal non nul de A contenu dans m, tel que $n \notin a$. Alors $h_n|G(a)$ est un isomorphisme de la variété analytique $G(a)$ sur la variété analytique $G(na)$.

$$
h_n(x) = nx + \sum_{|\alpha| \geq 2} a_\alpha x^\alpha.
$$

Donc, pour $x \in G$, on a

$$
\begin{align*}
h_n(nx) &= n^2(x + \sum_{|\alpha| \geq 2} a_\alpha n^{|\alpha|-2} x^\alpha) \\
&= n^2 S(x)
\end{align*}
$$

en posant $S(x) = x + \sum_{|\alpha| \geq 2} a_\alpha n^{|\alpha|-2} x^\alpha$. Cette série $S(x)$ définit une application analytique, que nous noterons encore $S$, de $G$ dans $G$. D’après A, IV, § 6, prop. 8, il existe une série entière en $r$ variables à coefficients dans $A^r$ telle que $S'(S(X)) = S(S'(X)) = X$. Donc $S$ est un isomorphisme de la variété analytique $G$ sur elle-même, et, pour tout idéal non nul $b$ de $A$ contenu dans $m$, on a $S(G(b)) \subset G(b), S'(G(b)) \subset G(b)$, donc $S(G(b)) = G(b)$. Comme $h_n(y) = n^2 S\left(\frac{1}{n} y\right)$ pour $y \in nG$, on voit que $h_n|n G(b)$ est un isomorphisme de la variété analytique $n G(b)$ sur la variété analytique $n^2 G(b)$. Or, comme $n \notin a$, on a $|n| > |\lambda|$ pour tout $\lambda \in a$, donc $n^{-1}a \subset m$, donc $a$ est de la forme $nb$ où $b$ est un idéal non nul de $A$ contenu dans $m$.

#### Corollaire {#lie-iii-s7-n5-cor-1 .statement}

*Si $n$ est inversible dans $A$, $h_n$ est un isomorphisme de la variété analytique $G$ sur elle-même. Pour tout idéal non nul $a$ de $A$ contenu dans $m$, on a $h_n(G(a)) = G(a)$. Pour tout $x \in G$, on a $\omega(x^n) = \omega(x)$.*

Cela résulte aussitôt de la prop. 8.

#### Proposition 9 {#lie-iii-s7-prop-9 .statement}

*Supposons $p \neq 0$.
(i) Soient $a, b$ des idéaux non nuls de $A$ tels que $b \subset a \subset m$. Dans le groupe $G(a)/G(b)$, tout élément admet pour ordre une puissance de $p$.
(ii) Supposons $v(p) = 1$. Si $x \in G$ est tel que $\omega(x) > \frac{1}{p-1}$, on a
$$
\omega(x^p) = \omega(x) + 1.
$$
D’après le § 5, formule (4), on a, pour tout $x \in G$,
$$
x^p = px + \sum_{|\alpha| \geq 2} c_\alpha x^\alpha
$$
où $c_\alpha \in A^r$ pour tout $\alpha$. Même pour prouver (i), on peut supposer $v(p) = 1$. Alors si $\omega(x) \geq 1$, on en déduit $\omega(x^p) \geq \omega(x) + 1$, donc $\omega(x^{p^n})$ tend vers $+\infty$ quand n tend vers + ∞; cela prouve (i). Comme $\binom{p}{i}$ est divisible par $p$ pour $1 \leq i \leq p - 1$, la prop. 2 du § 5, n° 3, prouve que $c_\alpha \in pA^r$ pour $2 \leq |\alpha| \leq p - 1$, donc
$$
\omega(c_\alpha x^\alpha) > \omega(px) = \omega(x) + 1 \text{ pour } 2 \leq |\alpha| \leq p - 1.
$$
D’autre part, si $|\alpha| \geq p$, on a $\omega(c_\alpha x^\alpha) \geq p \omega(x)$, et $p \omega(x) > \omega(x) + 1$ si $\omega(x) > \frac{1}{p - 1}$. Cela prouve (ii).

### 6. Application logarithme

#### Lemme 1 {#lie-iii-s7-lem-1 .statement}

On suppose $p \neq 0$. Soient $G$ un groupe de Lie, $G_1$ un sous-groupe ouvert de $G$ qui soit isomorphe à un groupe standard, et $x \in G$. Les conditions suivantes sont équivalentes:
(i) il existe une puissance de $x$ qui appartient à $G_1$;
(ii) il existe une suite strictement croissante $(n_i)$ d’entiers tels que $x^{n_i}$ tende vers $e$ quand $i$ tend vers $+ \infty$.
(ii) $\Rightarrow$ (i): évident.
(i) $\Rightarrow$ (ii): supposons que $y = x^m \in G_1$. D’après la prop. 9 (i) du n° 5, $y^{p^n}$ tend vers $e$ quand $n$ tend vers $+ \infty$, autrement dit $x^{mp^n}$ tend vers $e$ quand $n$ tend vers $+ \infty$.

#### Proposition 10 {#lie-iii-s7-prop-10 .statement}

On suppose $p \neq 0$. Soit $G$ un groupe de Lie de dimension finie. Soit $G_f$ l’ensemble des $x \in G$ pour lesquels il existe une suite strictement croissante $(n_i)$ d’entiers tels que $x^{n_i}$ tende vers $e$ quand $i$ tend vers $+ \infty$.
(i) $G_f$ est ouvert dans $G$.
(ii) Il existe une application $\psi$ et une seule de $G_f$ dans $L(G)$ possédant les propriétés suivantes:
a) $\psi(x^n) = n \psi(x)$ pour tout $x \in G_f$ et tout $n \in \mathbf{Z}$;
b) il existe un voisinage ouvert $V$ de $e$ dans $G_f$ tel que $\psi|V$ soit l’application réciproque d’une application exponentielle injective.
(iii) L’application $\psi$ est analytique.
Il existe un sous-groupe ouvert de $G$ qui est isomorphe à un groupe standard (n° 3, th. 4). L’assertion (i) résulte alors du lemme 1.
Soient $U$ un sous-groupe ouvert de $L(G)$, et $\varphi : U \to \varphi(U)$ une application exponentielle de $G$ ayant les propriétés de la prop. 3 du n° 2. On peut supposer $U$ assez petit pour que $\varphi(U) \subset G_f$. Soit $x \in G_f$. Il existe $m \in \mathbf{Z} - \{0\}$ tel que $x^m \in \varphi(U)$. L’élément $\frac{1}{m} \varphi^{-1}(x^m)$ ne dépend pas du choix de $m$. En effet, soit $m' \in \mathbf{Z}$ tel que $x^{m'} \in \varphi(U)$. On a $x^{mm'} \in \varphi(U)$, et
$$
m' \varphi^{-1}(x^m) = \varphi^{-1}(x^{mm'}) = m \varphi^{-1}(x^{m'}),
$$

d’où notre assertion. Posons $\psi(x) = \frac{1}{m} \varphi^{-1}(x^m)$. On a $\psi|\varphi(\mathrm{U}) = \varphi^{-1}$. D’autre part, si $n \in \mathbf{Z}$, on a
$$
\psi(x^n) = \frac{1}{m} \varphi^{-1}(x^{nm}) = \frac{n}{m} \varphi^{-1}(x^m) = n \psi(x).
$$
Donc $\psi$ possède les propriétés a) et b) de la proposition. Au voisinage de $x$, $\psi$ est composée des applications $x \mapsto x^m, y \mapsto \varphi^{-1}(y)$ et $z \mapsto \frac{1}{m} z$; donc $\psi$ est analytique dans $G_f$.

Enfin, soient $\psi'$ une application de $G_f$ dans $\mathrm{L}(G)$, et $V'$ un voisinage de $e$ dans $G_f$, tels que $\psi'(x^n) = n \psi'(x)$ pour $x \in G_f$ et $n \in \mathbf{Z}$, et tels que $\psi'|V'$ soit l’application réciproque d’une application exponentielle injective. Alors $\psi$ et $\psi'$ coïncident dans un voisinage $W$ de $e$. Si $x \in G_f$, il existe $n \in \mathbf{Z}$ tel que $x^n \in W$. Alors
$$
n \psi'(x) = \psi'(x^n) = \psi(x^n) = n \psi(x)
$$
donc $\psi = \psi'$.

#### Définition 2 {#lie-iii-s7-def-2 .statement}

L’application $\psi$ de la prop. 10 s’appelle l’application logarithme de $G$, et se note $\log_G$ ou simplement $\log$.

#### Proposition 11 {#lie-iii-s7-prop-11 .statement}

Supposons $p \neq 0$. Soient $x, y$ deux éléments permutables de $G_f$. On a $xy \in G_f$ et $\log(xy) = \log x + \log y$.

Le fait que $xy \in G_f$ résulte du lemme 1. Soient $\mathrm{U}$ un sous-groupe ouvert du groupe additif $\mathrm{L}(G)$ et $\varphi : \mathrm{U} \to \varphi(\mathrm{U})$ une application exponentielle de $G$ ayant les propriétés de la prop. 3 du n° 2; on peut supposer $\mathrm{U}$ assez petit pour que $\log|\psi(\mathrm{U})|$ soit l’application réciproque de $\varphi$. Pour $n \in \mathbf{Z} - \{0\}$ bien choisi, on a $x^n \in \varphi(\mathrm{U}), y^n \in \varphi(\mathrm{U})$. Posons $u = \log x^n, v = \log y^n$, d’où $x^n = \varphi(u), y^n = \varphi(v)$. D’après la formule (2), on a $[u, v] = 0$. La formule de Hausdorff prouve alors que $\varphi(\lambda(u + v)) = \varphi(\lambda u)\varphi(\lambda v)$ pour $|\lambda|$ assez petit; donc, pour tout entier $i$ assez grand, on a
$$
\varphi(p^i(u + v)) = \varphi(p^i u)\varphi(p^i v)
$$
c’est-à-dire
$$
p^i (\log x^n + \log y^n) = \log(x^{np^i} y^{np^i})
$$
ou
$$
np^i (\log x + \log y) = np^i \log(xy).
$$

#### Proposition 12 {#lie-iii-s7-prop-12 .statement}

Supposons $p \neq 0$. Soit $x \in G_f$. Les conditions suivantes sont équivalentes:
(i) $\log x = 0$;
(ii) $x$ est d’ordre fini dans $G$.

S’il existe un entier $n > 0$ tel que $x^n = e$, on en déduit que
$$
n \log x = \log x^n = 0,
$$

d’où $\log x = 0$. Si $\log x = 0$, soit $V$ un voisinage de $e$ dans $G_f$ tel que $\log|V|$ soit l’application réciproque d’une application exponentielle injective. Il existe un entier $n > 0$ tel que $x^n \in V$; l’égalité $\log x^n = 0$ entraîne $x^n = e$.

#### Proposition 13 {#lie-iii-s7-prop-13 .statement}

*Supposons $p \neq 0$. Si $G$ est compact ou standard, on a $G_f = G$.*

Si $G$ est standard, il suffit d’utiliser le lemme 1. Supposons $G$ compact. Soient $x \in G$ et $V$ un voisinage de $e$ dans $G$. Soit $y$ une valeur d’adhérence de la suite $(x^n)_{n \geq 0}$. Quel que soit $n > 0$, il existe deux entiers $n_1, n_2$ tels que $n_1 \geq 2n_2 \geq n$ et $x^{n_1} \in y\, V, x^{n_2} \in y\, V$, d’où $x^{n_1 - n_2} \in V^{-1}V$ et $n_1 - n_2 \geq n$. Donc $x \in G_f$.

#### Corollaire {#lie-iii-s7-n6-cor-1 .statement}

*Supposons $K$ localement compact. Alors $G_f$ est la réunion des sous-groupes compacts de $G$.*

Soit $x \in G$. Si $x$ appartient à un sous-groupe compact de $G$, on a $x \in G_f$ (prop. 13). Supposons $x \in G_f$. Comme $K$ est localement compact, il existe un sous-groupe ouvert $G_1$ de $G$ qui est compact. Puis il existe un entier $m > 0$ tel que $x^m \in G_1$. Le sous-groupe fermé $G_2$ engendré par $x^m$ est contenu dans $G_1$, donc compact. Alors $x$ commute aux éléments de $G_2$, donc $G_2 \cup xG_2 \cup \cdots \cup x^{m-1}G_2$ est un sous-groupe compact de $G$, qui contient $x$.

#### Exemple {#lie-iii-s7-n6-exa-1 .statement}

Supposons $K$ localement compact. Soit $U$ l’ensemble des éléments inversibles de $A$; c’est un sous-groupe ouvert et compact du groupe de Lie $K^*$. On a $U \subset (K^*)_f$, d’après la prop. 13; d’autre part, si $x \in K^*$ est tel que $x \notin U$, ou bien $x^n$ tend vers 0 quand $n$ tend vers $+\infty$, ou bien $x^n$ tend vers 0 quand $n$ tend vers $-\infty$; donc $U = (K^*)_f$. La fonction $\log_{K^*}$ est définie et analytique dans $U$, à valeurs dans $L(K^*) = K$, et telle que $\log_{K^*}(xy) = \log_{K^*}(x) + \log_{K^*}(y)$ quels que soient $x, y$ dans $U$; les éléments $x$ de $U$ tels que $\log_{K^*}(x) = 0$ sont les racines de l’unité de $K$.

On reprend les notations des nos 3, 4, 5.

#### Proposition 14 {#lie-iii-s7-prop-14 .statement}

*On suppose que $p \neq 0$ et que $v$ est choisie de telle sorte que $v(p) = 1$. Soient $G$ un groupe standard, $E(X)$ (resp. $L(X)$) le développement en série entière en 0 d’une application exponentielle de $G$ (resp. de l’application logarithme de $G$).

(i) *Le domaine de convergence stricte* (VAR, R, 4.1.3) de $E$ contient l’ensemble $\Delta$ des $x \in G$ tels que $\omega(x) > \frac{1}{p-1}$. Notons $E'$ l’application définie dans $\Delta$ par cette série. Alors $E'$ est une application exponentielle de $G$, et est un isomorphisme de la variété $\Delta$ sur elle-même.

(ii) *Le domaine de convergence stricte de $L$ contient $G$*. Notons $L'$ l’application définie dans $G$ par cette série. Alors $L'$ est l’application logarithme de $G$, et la restriction de $L'$ à $\Delta$ est l’application réciproque de $E'$.

(iii) *L’application $E'$ est un isomorphisme de $\Delta$, muni de la loi de Hausdorff, sur le sous-groupe $\Delta$ de $G$.*

Reprenons les notations du § 5, n°s 3 et 4. On a $E = \sum_{m \geq 1} \frac{\psi_{m,m}}{m!}$ (§ 5, n° 4, prop. 3). Comme les coefficients $c_{\alpha \beta \gamma}$ appartiennent à $A$, on a $\| \psi_{m,m} \| \leq 1$ (VAR, R, Appendice ; on suppose $K'$ muni de la norme
$$
\| (\lambda_1, \ldots, \lambda_r ) \| = \sup ( | \lambda_1 |, \ldots, | \lambda_r | ).
$$
D’après le chap. II, § 8, n° 1, lemme 1, on a $v(m!) \leq \frac{m-1}{p-1}$. Si $\omega(x) > \frac{1}{p-1}$, on voit que $m \, \omega(x) - v(m!)$ tend vers $+ \infty$ avec $m$, d’où
$$
\left\| \frac{\psi_{m,m}}{m!} \right\| \| x \|^{m} \leq \frac{1}{|m!|} \| x \|^{m}
$$
qui tend vers 0 quand $m$ tend vers $+ \infty$
et
$$
\omega \left( \frac{\psi_{m,m}(x)}{m!} \right) > \frac{m}{p-1} - \frac{m-1}{p-1} = \frac{1}{p-1} \quad \text{pour } m \geq 1.
$$
Par suite, $\Delta$ est contenu dans le domaine de convergence stricte de $E$, et $E'(\Delta) \subset \Delta$. Il est clair que $E'$ est une application exponentielle.

Si $L_m$ désigne la composante homogène de degré $m$ de $L$, la prop. 3 du § 5, n° 4, prouve que chaque coefficient de $L_m$ est de la forme $a_1 + \frac{1}{2} a_2 + \cdots + \frac{1}{m} a_m$ avec $a_1, a_2, \ldots, a_m$ dans $A$; or
$$
\inf \left( v(1), v\left( \frac{1}{2} \right), \ldots, v\left( \frac{1}{m} \right) \right) = O(\log m) \quad \text{quand } m \text{ tend vers } + \infty
$$
et
$$
\inf \left( v(1), v\left( \frac{1}{2} \right), \ldots, v\left( \frac{1}{m} \right) \right) \geq v\left( \frac{1}{m!} \right) \geq - \frac{m-1}{p-1}.
$$
Par suite, si $\omega(x) > 0$, $\| L_m \| \cdot \| x \|^{m}$ tend vers 0 quand $m$ tend vers $+ \infty$, de sorte que $G$ est contenu dans le domaine de convergence stricte de $L$. D’autre part, si $\omega(x) > \frac{1}{p-1}$, on a $\omega(L_m(x)) > \frac{m}{p-1} - \frac{m-1}{p-1} = \frac{1}{p-1}$ pour $m \geq 1$, donc $L'(\Delta) \subset \Delta$.

Comme les séries formelles $L(E(X))$ et $E(L(X))$ sont égales à $X$, le n° 4.1.5 de VAR, R, prouve que $L'(E'(x)) = E'(L'(x)) = x$ pour $x \in \Delta$. Donc $E'$ est un isomorphisme de la variété $\Delta$ sur elle-même, et l’isomorphisme réciproque est la restriction de $L'$ à $\Delta$.

On a $L(X^{[n]}) = nL(X)$ pour $n$ entier $> 0$ (cf. § 5, n° 4). Comme $G$ est contenu dans le domaine de convergence stricte de $L$ et de $X^{[n]}$, on a donc $L'(x^n) = nL'(x)$ pour tout $x \in G$. La relation $L'|_{\Delta} = {E'}^{-1}$ entraîne que $L'(x^n) = \log x^n$ pour assez grand. Donc $L'(x) = \log x$. On a ainsi prouvé (i) et (ii).

Soient $H = \sum_{r,s \geq 0} H_{r,s}$ la série formelle de Hausdorff, et $h$ la fonction de

Hausdorff, relatives à $L(G)$. Le domaine de convergence strict de $\tilde{H}$ contient $\Delta \times \Delta$, et $h$ est définie dans $\Delta \times \Delta$ (chap. II, § 8, prop. 2). On a
$$
E'(x)E'(y) = E'(h(x, y))
$$
pour $x, y$ assez voisins de 0 ($\S 4$, th. 4 (v)). Donc, avec les notations du n° 3, déf. 1, les séries formelles $F(E(X), E(Y))$ et $E(H(X, Y))$ sont égales. Soient $x, y$ dans $\Delta$. On a
$$
\sup_m \left\| \frac{\psi_{m,m}}{m!} \right\| (\sup (\|x\|, \|y\|))^m < 1
$$
$$
\sup_{r,s} \|H_{r,s}\| \|x\|^r \|y\|^s < |p|^{1/(p-1)}
$$
d’après le chap. II, § 8, formule (14). D’après VAR, R, 4.1.5, $E'(x)E'(y)$ s’obtient en substituant $x$ à $X$ et $y$ à $Y$ dans $F(E(X), E(Y))$, et $E'(h(x, y))$ s’obtient en substituant $x$ à $X$ et $y$ à $Y$ dans $E(H(X, Y))$. Donc $E'(x)E'(y) = E'(h(x, y))$.

## EXERCICES {#lie-iii-s7-exercises}

See the [exercises for § 7](exercises/s7/).
