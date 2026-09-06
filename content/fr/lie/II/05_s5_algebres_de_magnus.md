---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: II
chapter_title: ALGÈBRES DE LIE LIBRES
section: 5
section_title: Algèbres de Magnus
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0043-0049, 0082-0088
extraction: ocr
subsections:
    - "no": 1
      title: Algèbres de Magnus
      page: 0
      pdf_page: 43
    - "no": 2
      title: Groupe de Magnus
      page: 0
      pdf_page: 44
    - "no": 3
      title: Groupe de Magnus et groupe libre
      page: 0
      pdf_page: 44
    - "no": 4
      title: Suite centrale descendante d’un groupe libre
      page: 0
      pdf_page: 46
    - "no": 5
      title: $p$-filtration des groupes libres
      page: 0
      pdf_page: 48
statements: 14
exercises: 12
content_sha256: 6994d1fcef1279c0e7cff0c45ff4c40d2c5fa008b3fcaaed2d058d386707fb02
---

## § 5. Algèbres de Magnus

Dans ce paragraphe, on note $X$ un ensemble, $F(X)$ le groupe libre construit sur $X$ (A, I, p. 84, n° 5) et $A(X)$ l’algèbre associative libre construite sur $X$, munie de sa graduation totale $(A^n(X))_{n \geq 0}$ (cf. A, III, p. 31, Exemple 3). On identifie $X$ à ses images dans $F(X)$ et $A(X)$.

### 1. Algèbres de Magnus

Soit $\hat{A}(X)$ le module produit $\prod_{n \geq 0} A^n(X)$. Dans $\hat{A}(X)$ on définit une multiplication par la règle

$$
(a \cdot b)_n = \sum_{i=0}^n a_i \cdot b_{n-i}
$$

pour $a = (a_n)$ et $b = (b_n)$ dans $\hat{A}(X)$. On sait (AC, III, § 2, n° 12, Exemple 1) que $\hat{A}(X)$ est une algèbre associative et que $A(X)$ s’identifie à la sous-algèbre de $\hat{A}(X)$ formée des suites dont tous les termes sont nuls à l’exception d’un nombre fini.

On munit $\hat{A}(X)$ de la topologie produit des topologies discrètes des facteurs $A^n(X)$; cette topologie fait de $\hat{A}(X)$ une algèbre topologique séparée et complète, l’anneau $K$ étant muni de la topologie discrète, et $A(X)$ est dense dans $\hat{A}(X)$.

Soit $a = (a_n) \in \hat{A}(X)$; la famille $(a_n)_{n \geq 0}$ est sommable et $a = \sum_{n \geq 0} a_n$.

Pour tout entier $m \geq 0$, on note $\hat{A}_m(X)$ l’idéal formé des séries $a = \sum_{n \geq m} a_n$ telles que $a_n \in A^n(X)$ pour tout $n \geq m$. Cette suite d’idéaux est un système fondamental de voisinages de 0 dans $\hat{A}(X)$ et une filtration entière sur $\hat{A}(X)$. La fonction d’ordre associée à la filtration précédente est notée $\omega$; on a donc $\omega(0) = +\infty$ et $\omega(a) = m$ si $a = \sum_{n \geq m} a_n$ avec $a_n \in A^n(X)$ pour tout $n \geq m$ et $a_m \neq 0$ ($§ 4$, n°s 1 et 2).

On dit que $\hat{A}(X)$ est l’algèbre de Magnus de l’ensemble $X$ à coefficients dans $K$. Si une ambiguïté sur $K$ est possible on écrira $\hat{A}_K(X)$.

#### Proposition 1 {#lie-ii-s5-prop-1 .statement}

Soit $B$ une algèbre associative unifère, munie d’une filtration réelle $(B_\alpha)_{\alpha \in \mathbf{R}}$ pour laquelle $B$ est séparée et complète ($§ 4$, n°s 1 et 2). Soit $f$ une application de $X$ dans $B$, telle qu’il existe $\lambda > 0$ pour lequel $f(X) \subset B_\lambda$. Alors $f$ se prolonge d’une manière et d’une seule en un homomorphisme unifère continu $\hat{f}$ de $\hat{A}(X)$ dans $B$.

Soit $f'$ l’unique homomorphisme d’algèbre unifère de $\mathbf{A}(X)$ dans $B$ prolongeant $f$ (A, III, p. 22, prop. 7). Montrons que $f'$ est continu: en effet, on a $f'(\mathbf{A}^n(X)) \subset B_{n\lambda}$ d’où $f'(\hat{\mathbf{A}}_n(X) \cap \mathbf{A}(X)) \subset B_{n\lambda}$. Par suite, $f'$ se prolonge d’une manière et d’une seule par continuité en un homomorphisme $\hat{f}: \hat{\mathbf{A}}(X) \to B$.

Conservons les hypothèses et notations de la prop. 1 et soit $u \in \hat{\mathbf{A}}(X)$. L’élément $\hat{f}(u)$ se note $u((f(x))_{x \in X})$ et s’appelle le résultat de la substitution des $f(x)$ aux $x$ dans $u$. En particulier, on a $u((x)_{x \in X}) = u$. Soit maintenant $u = (u_y)_{y \in Y}$ une famille d’éléments de $\hat{\mathbf{A}}_1(X)$ et soit $v \in \hat{\mathbf{A}}(Y)$. Ce qui précède permet de définir l’élément $v((u_y)_{y \in Y}) \in \hat{\mathbf{A}}(X)$. On le note $v \circ u$. Comme $u_y((f(x))) \in B_\lambda$, on peut substituer les éléments $u_y((f(x)))$ aux $y$ dans $v$. Les applications $v \mapsto (v \circ u)((f(x)))$ et $v \mapsto v((u_y((f(x))))))$ sont alors deux homomorphismes continus d’algèbres unifères de $\hat{\mathbf{A}}(Y)$ dans $B$, et prennent la même valeur $u_y((f(x)))$ sur l’élément $y \in Y$. Par suite (prop. 1), on a

$$
(v \circ u)((f(x))) = v((u_y((f(x))))))
$$

pour tout $v \in \hat{\mathbf{A}}(Y)$.

### 2. Groupe de Magnus

Pour tout $a = (a_n)_{n \geq 0}$ dans $\hat{\mathbf{A}}(X)$, l’élément $a_0$ de $K$ sera appelé le terme constant de $a$, et noté $\varepsilon(a)$. La formule (1) montre que $\varepsilon$ est un homomorphisme d’algèbre de $\hat{\mathbf{A}}(X)$ dans $K$.

#### Lemme 1 {#lie-ii-s5-lem-1 .statement}

Pour qu’un élément $a$ de $\hat{\mathbf{A}}(X)$ soit inversible, il faut et il suffit que son terme constant soit inversible dans $K$.

Si $a$ est inversible dans $\hat{\mathbf{A}}(X)$, $\varepsilon(a)$ est inversible dans $K$. Inversement, si $\varepsilon(a)$ est inversible dans $K$, il existe $u \in \hat{\mathbf{A}}_1(X)$ tel que $a = \varepsilon(a)(1 - u)$; posons $b = \left( \sum_{n \geq 0} u^n \right) \varepsilon(a)^{-1}$. On a $ab = ba = 1$, et $a$ est inversible.

L’ensemble des éléments de $\hat{\mathbf{A}}(X)$ de terme constant 1 est donc un sous-groupe du monoïde multiplicatif $\hat{\mathbf{A}}(X)$, qu’on appelle le groupe de Magnus construit sur $X$ (relativement à $K$). Dans ce chapitre, on le notera $\Gamma(X)$, ou simplement $\Gamma$. Pour tout entier $n \geq 1$, on note $\Gamma_n$ l’ensemble des $a \in \Gamma$ tels que $\omega(a - 1) \geq n$. D’après la prop. 2 du § 4, n° 5, la suite $(\Gamma_n)_{n \geq 1}$ est une filtration centrale entière sur $\Gamma$.

### 3. Groupe de Magnus et groupe libre

#### Théorème 1 {#lie-ii-s5-thm-1 .statement}

Soit $r$ une application de $X$ dans $\hat{\mathbf{A}}(X)$ telle que $\omega(r(x)) \geq 2$ pour tout $x \in X$. L’unique homomorphisme $g$ du groupe libre $F(X)$ dans le groupe de Magnus $\Gamma(X)$, tel que $g(x) = 1 + x + r(x)$ pour tout $x \in X$, est injectif.

Démontrons d’abord trois lemmes.

#### Lemme 2 {#lie-ii-s5-lem-2 .statement}

Soit $n$ un entier rationnel non nul. Dans l’anneau de séries formelles $\mathbf{K}[[t]]$, on pose $(1 + t)^n = \sum_{j \geq 0} c_{j,n} t^j$. Il existe un entier $j \geq 1$ tel que $c_{j,n} \neq 0$.

Si $n > 0$, on a $c_{n,n} = 1$ d’après la formule du binôme.

Supposons $n < 0$ et posons $m = -n$. Si l’on avait $c_{j,n} = 0$ pour tout $j \geq 1$, on aurait $(1 + t)^n = 1$, d’où en prenant l’inverse, $(1 + t)^m = 1$, ce qui est contraire à la formule $c_{m,m} = 1$.

#### Lemme 3 {#lie-ii-s5-lem-3 .statement}

Soient $x_1, \ldots, x_s$ des éléments de $X$, tels que $s \geq 1$ et $x_i \neq x_{i+1}$ pour $1 \leq i \leq s-1$; soient $n_1, \ldots, n_s$ des entiers rationnels non nuls. Alors l’élément $\prod_{i=1}^s (1 + x_i)^{n_i}$ de $\hat{\mathbf{A}}(X)$ est $\neq 1$.

Soient $m$ un idéal maximal de $K$ et $k$ le corps $K/m$; soit $p : \hat{\mathbf{A}}_K(X) \to \hat{\mathbf{A}}_k(X)$ l’unique homomorphisme continu de $K$-algèbres unifères tel que $p(x) = x$ pour $x \in X$ (no 1, prop. 1). Il suffit de prouver que $p(\Pi(1 + x_i)^{n_i}) \neq 1$, et on est ramené au cas où $K$ est un corps.

Avec les notations du lemme 2, on a:

$$
\prod_{i=1}^s (1 + x_i)^{n_i} = \sum_{b_i \geq 0} c_{b_1,n_1} \cdots c_{b_s,n_s} x_1^{b_1} \cdots x_s^{b_s}.
$$

D’après le lemme 2, il existe des entiers $a_i > 0$ tels que $c_{a_i,n_i} \neq 0$ ($1 \leq i \leq s$). D’après A, I, p. 84, prop. 6, aucun monôme $x_1^{b_1} \cdots x_s^{b_s}$ tel que $b_i \geq 0$ et $(b_1, \ldots, b_s) \neq (a_1, \ldots, a_s)$ ne peut être égal à $x_1^{a_1} \cdots x_s^{a_s}$. Il s’ensuit que le coefficient de $x_1^{a_1} \cdots x_s^{a_s}$ dans $\prod_{i=1}^s (1 + x_i)^{n_i}$ est $c_{a_1,n_1} \cdots c_{a_s,n_s} \neq 0$, ce qui entraîne le résultat.

#### Lemme 4 {#lie-ii-s5-lem-4 .statement}

Soit $\sigma$ l’endomorphisme continu de $\hat{\mathbf{A}}(X)$ tel que $\sigma(x) = x + r(x)$ pour $x \in X$ (no 1, prop. 1). Alors $\sigma$ est un automorphisme et $\sigma(\hat{\mathbf{A}}_m(X)) = \hat{\mathbf{A}}_m(X)$ pour tout $m \in \mathbf{N}$.

On a $\sigma(x) \equiv x \mod \hat{\mathbf{A}}_2(X)$ pour $x \in X$, d’où, pour $n \geq 1$ et $x_1, \ldots, x_n$ dans $X$,

$$
\sigma(x_1) \cdots \sigma(x_n) \equiv x_1 \cdots x_n \quad \text{mod. } \hat{\mathbf{A}}_{n+1}(X);
$$

il en résulte par linéarité que $\sigma(a) \equiv a$ modulo $\hat{\mathbf{A}}_{n+1}(X)$ pour tout $a \in \mathbf{A}^n(X)$, et en particulier $\sigma(\mathbf{A}^n(X)) \subset \hat{\mathbf{A}}_n(X)$. On en déduit $\sigma(\mathbf{A}^m(X)) \subset \hat{\mathbf{A}}_n(X)$ pour $m \geq n$, d’où $\sigma(\hat{\mathbf{A}}_n(X)) \subset \hat{\mathbf{A}}_n(X)$. Autrement dit, $\sigma$ est compatible avec la filtration $(\hat{\mathbf{A}}_m(X))$ de $\mathbf{A}(X)$ et sa restriction au gradué associé est l’identité. Donc $\sigma$ est bijectif (AC, III, § 2, no 8, cor. 3 du th. 1).

Démontrons enfin le théorème 1. Soit $w \neq 1$ un élément de $F(X)$. D’après A, I, p. 84, prop. 7, il existe $x_1, \ldots, x_s$ dans $X$ et des entiers rationnels non nuls $n_1, \ldots, n_s$, tels que $s \geq 1$, $x_i \neq x_{i+1}$ ($1 \leq i \leq s-1$), et

$$
w = x_1^{n_1} \cdots x_s^{n_s}.
$$

Avec les notations du lemme 4, on a

$$
g(w) = \prod (1 + \sigma(x_i))^{n_i} = \sigma(\prod (1 + x_i)^{n_i}),
$$

donc $g(w) \neq 1$ d’après les lemmes 3 et 4.

### 4. Suite centrale descendante d’un groupe libre

Nous allons démontrer les deux théorèmes suivants:

#### Théorème 2 {#lie-ii-s5-thm-2 .statement}

On suppose que dans l’anneau K, la relation $n \cdot 1 = 0$ entraîne $n = 0$ pour tout entier $n$. Soit $r$ une application de $X$ dans $\hat{A}(X)$ telle que $\omega(r(x)) \geq 2$ pour $x \in X$, et soit $g$ l’homomorphisme de $F(X)$ dans le groupe de Magnus $\Gamma(X)$ tel que $g(x) = 1 + x + r(x)$ pour $x \in X$. Pour tout $n \geq 1$, $C^n F(X)$ est l’image réciproque par $g$ du sous-groupe $1 + \hat{A}_n(X)$ de $\Gamma(X)$.

#### Théorème 3 {#lie-ii-s5-thm-3 .statement}

Pour tout $x \in X$, soit $c(x)$ l’image canonique de $x$ dans $F(X)/(F(X), F(X))$. Soit $g$ la $\mathbf{Z}$-algèbre de Lie graduée associée à la filtration $(C^n F(X))_{n \geq 1}$ de $F(X)$ (§ 4, n° 6). L’unique homomorphisme de la $\mathbf{Z}$-algèbre de Lie libre $L_Z(X)$ dans $g$ qui prolonge $c$ est un isomorphisme.

En termes imagés, la $\mathbf{Z}$-algèbre de Lie graduée associée au groupe libre $F(X)$ (muni de la suite centrale descendante) est la $\mathbf{Z}$-algèbre de Lie libre $L_Z(X)$.

Posons $F(X) = F, \ \Gamma(X) = \Gamma, \ \hat{A}(X) = \hat{A}, \ \hat{A}_Z(X) = \hat{A}_Z, \ C^n F(X) = C^n, \ \Gamma_n = 1 + \hat{A}_n(X)$, et soit $\alpha : L_Z(X) \to g$ l’homomorphisme introduit dans l’énoncé du th. 3.

A) Réductions préliminaires.

Notons $\gamma$ l’homomorphisme de $F$ dans $\Gamma$ défini par $\gamma(x) = 1 + x$ pour $x \in X$. D’après le lemme 4, il existe un automorphisme $\sigma$ de l’algèbre $\hat{A}$ respectant la filtration de $\hat{A}$ et tel que $\sigma(1 + x) = g(x)$ pour tout $x \in X$; on a $\sigma(\Gamma_n) = \Gamma_n$ pour tout $n$. Comme les homomorphismes $g$ et $\sigma \circ \gamma$ de $F$ dans $\Gamma$ coïncident dans $X$, on a $g = \sigma \circ \gamma$, donc $g^{-1}(\Gamma_n) = \gamma^{-1}(\Gamma_n)$. Sous les hypothèses du th. 2, on peut identifier $\mathbf{Z}$ à un sous-anneau de $K$; l’algèbre de Magnus $\hat{A}_Z$ s’identifie donc à un sous-anneau de $\hat{A}$, la filtration de $\hat{A}_Z$ étant induite par celle de $\hat{A}$. Comme $\gamma$ applique $F$ dans $\hat{A}_Z$, on voit qu’il suffit de prouver les th. 2 et 3 sous les hypothèses supplémentaires $K = \mathbf{Z}$ et $r = 0$, donc $g = \gamma$, hypothèses que nous ferons désormais.

B) Surjectivité de $\alpha$.

Comme $X$ engendre le groupe $F = C^1$, l’ensemble $c(X)$ engendre le $\mathbf{Z}$-module $g^1 = C^1/C^2$. Or $g^1$ engendre la $\mathbf{Z}$-algèbre de Lie $g$ (§ 4, n° 6, prop. 5), donc $c(X)$ engendre $g$, ce qui prouve que $\alpha$ est surjectif.

C) Identifions l’algèbre graduée $\mathrm{gr}(\hat{A})$ à $A(X)$ par les isomorphismes canoniques $A^n(X) \to \hat{A}_n/\hat{A}_{n+1}$. Pour tout entier $n \geq 1$, posons $F^n = \gamma^{-1}(\Gamma_n)$; on sait (§ 4, n° 5) que $(F^n)_{n \geq 1}$ est une filtration centrale entière sur $F$. Notons $g'$ la $\mathbf{Z}$-algèbre de Lie graduée associée (§ 4, n° 4). Soit $f$ l’homomorphisme d’algèbres de Lie de $g'$ dans $A(X)$ associé à $\gamma$ (§ 4, n° 5, prop. 3). Or, on a $C^n \subset F^n$ pour tout entier $n \geq 1$ (§ 4, n° 6, prop. 4), d’où un homomorphisme canonique $\varepsilon$ de $g = \bigoplus_{n \geq 1} C^n/C^{n+1}$ dans $g' = \bigoplus_{n \geq 1} F^n/F^{n+1}$

$$
L_\mathbf{Z}(X) \xrightarrow{\alpha} g \xrightarrow{\varepsilon} g' \xrightarrow{f} A(X).
$$

On pose $\beta = f \circ \varepsilon$; on peut expliciter $\beta$ ainsi : si $u$ est la classe modulo $C^{n+1}$ d’un élément $w$ de $C^n$, alors $\gamma(w) - 1$ est d’ordre $\geq n$ dans $\hat{A}$ et $\beta(u)$ est la composante homogène de degré $n$ de $\gamma(w) - 1$. En particulier, on a

(3)
$$
\beta(c(x)) = x \quad \text{pour tout } x \in X.
$$

D) *Démonstration des théorèmes 2 et 3*.

L’homomorphisme d’algèbres de Lie $\beta \circ \alpha : L_\mathbf{Z}(X) \to A(X)$ a pour restriction à $X$ l’identité d’après (3), donc est l’*injection canonique* (§ 3, n° 1). Par suite, $\alpha$ est injectif, donc bijectif d’après B); ceci démontre le th. 3. Comme $\beta \circ \alpha = f \circ \varepsilon \circ \alpha$ est injectif et que $\alpha$ est bijectif, $\varepsilon$ est injectif. Pour tout $n \geq 1$,

$$
\varepsilon_n : C^n/C^{n+1} \to F^n/F^{n+1}
$$

est injectif, donc

$$
C^n \cap F^{n+1} = C^{n+1}.
$$

On a $C^1 = F = F^1$; si $C^n = F^n$, on a $C^n \cap F^{n+1} = F^{n+1}$ d’où $C^{n+1} = F^{n+1}$, ce qui démontre le th. 2 par récurrence sur $n \geq 1$.

#### Corollaire {#lie-ii-s5-n4-cor-1 .statement}

*On a*

$$
\bigcap_{n \geq 1} C^n F(X) = \{e\}.
$$

En effet, appliquant le th. 2 pour $K = \mathbf{Z}$ et $r = 0$, on a

$$
\bigcap_{n \geq 1} C^n F(X) = \bigcap_{n \geq 1} g^{-1}(1 + \hat{A}_n(X)) = g^{-1}\left(\bigcap_{n \geq 1} (1 + \hat{A}_n(X))\right) = g^{-1}(1) = \{e\}.
$$

#### Remarque {#lie-ii-s5-n4-rem-1 .statement}

Soit $H$ un ensemble de Hall relatif à $X$ (§ 2, n° 10). Soit $M$ le magma défini par la loi de composition $(x, y) \mapsto (x, y) = x^{-1}y^{-1}xy$ sur $F(X)$, et soit $\varphi$ l’homomorphisme de $M(X)$ dans $M$ dont la restriction à $X$ est l’identité. Les éléments de $\varphi(H)$ s’appellent les *commutateurs basiques* de $F(X)$ associés à l’ensemble de Hall $H$. Pour tout entier $n \geq 1$, soit $H_n$ la partie de $H$ formée des éléments de longueur $n$; on sait (§ 2, n° 11, th. 1) que l’application canonique de $H_n$ dans $L_\mathbf{Z}(X)$ est une base du groupe abélien $L^n_\mathbf{Z}(X)$. De plus, on a $\varphi(H_n) \subset C^n$; pour tout $m \in H_n$, notons $\varphi_n(m)$ la classe mod. $C^{n+1}$ de $\varphi(m) \in C^n$. Le th. 3 montre alors que $\varphi_n$ est une bijection de $H_n$ sur une base du groupe abélien $C^n/C^{n+1}$. On déduit aussitôt de là que, pour tout $w \in F(X)$, et tout $i \geq 1$, il existe un élément unique $\alpha_i$ de $\mathbf{Z}^{(H_i)}$ tel que, pour tout $n \geq 1$, on ait

$$
w = \prod_{i=1}^n \prod_{m \in H_i} \varphi(m)^{\alpha_i(m)} \mod C^{n+1},
$$

où le produit est calculé suivant l’ordre total donné sur $H$.

#### Exemple {#lie-ii-s5-n4-exa-1 .statement}

Supposons que $X$ soit un ensemble à deux éléments $x, y$ et prenons $H_1 = \{x, y\}, H_2 = \{xy\}$. Tout élément $w$ de $F(X)$ peut donc s’écrire

$$
w \equiv x^a y^b (x, y)^c \mod C^3 \quad \text{avec } a, b, c \text{ dans } \mathbf{Z}.
$$

Pour $w = (xy)^n$, on a $a = b = n$ et $c = n(1-n)/2$ (cf. exerc. 9), d’où

$$
(xy)^n \equiv x^n y^n (x, y)^{n(1-n)/2} \mod C^3.
$$

### 5. $p$-filtration des groupes libres

Dans ce $n^\circ$, on note $p$ un nombre premier et l’on suppose $K = \mathbf{F}_p$. Soit $\gamma$ l’homomorphisme de $F(X)$ dans $\Gamma(X)$ défini par $\gamma(x) = 1 + x$ pour $x$ dans $X$; posons $F_n^{(p)}(X) = \gamma^{-1}(1 + \hat{A}_n(X))$. La suite $(F_n^{(p)}(X))_{n \geq 1}$ est une filtration centrale entière sur $F(X)$, qui est séparée car $\gamma$ est injectif ($n^\circ 3$, th. 1). On l’appelle la $p$-filtration de $F(X)$.

#### Proposition 2 {#lie-ii-s5-prop-2 .statement}

*Supposons $X$ fini. Pour tout entier $n \geq 1$, le groupe $F(X)/F_n^{(p)}(X)$ est un $p$-groupe fini de classe de nilpotence $\leq n$.*

Raisonnant par récurrence sur $n$, il suffit de prouver que $F_n^{(p)}(X)/F_{n+1}^{(p)}(X)$ est un $p$-groupe commutatif fini pour tout $n \geq 1$. Pour tout $w \in F_n^{(p)}(X)$, l’élément $\gamma(w) - 1$ de $\hat{A}(X)$ est d’ordre $\geq n$; on note $\delta_n(w)$ la composante homogène de degré $n$ de $\gamma(w) - 1$. L’application $\delta_n : F_n^{(p)}(X) \to A^n(X)$ est un homomorphisme de noyau $F_{n+1}^{(p)}(X)$ ($§ 4$, $n^\circ 5$, prop. 3), donc $F_n^{(p)}(X)/F_{n+1}^{(p)}(X)$ est isomorphe à un sous-groupe de $A^n(X)$. Puisque $X$ est fini, $A^n(X)$ est un espace vectoriel de dimension finie sur $\mathbf{F}_p$, donc un $p$-groupe commutatif fini et il en est de même de $F_n^{(p)}(X)/F_{n+1}^{(p)}(X)$.

#### Proposition 3 {#lie-ii-s5-prop-3 .statement}

*Pour tout $w \neq 1$ dans $F(X)$, il existe un $p$-groupe fini $G$ et un homomorphisme $f$ de $F(X)$ dans $G$ tel que $f(w) \neq 1$.*

Il existe des éléments $x_1, \ldots, x_r$ de $X$ et des entiers $n_1, \ldots, n_r$ tels que $w = x_1^{n_1} \ldots x_r^{n_r}$. Soit $Y = \{x_1, \ldots, x_r\}$. L’injection canonique de $Y$ dans $X$ se prolonge en un homomorphisme $\alpha : F(Y) \to F(X)$; par ailleurs, soit $\beta$ l’homomorphisme de $F(X)$ dans $F(Y)$ dont la restriction à $Y$ est l’identité et qui applique $X - Y$ dans $\{1\}$. On a $\beta(\alpha(y)) = y$ pour $y \in Y$, donc $\beta \circ \alpha$ est l’automorphisme identique de $F(Y)$. Il existe évidemment $w'$ dans $F(Y)$ tel que $w = \alpha(w')$; alors $\beta(w) = w' \neq 1$; or on a $\bigcap_{n \geq 1} F_n^{(p)}(Y) = \{1\}$ et il existe donc un entier $n \geq 1$ tel que $\beta(w) \notin F_n^{(p)}(Y)$. D’après la prop. 2, le groupe $G = F(Y)/F_n^{(p)}(Y)$ est un $p$-groupe fini. Si $f$ est le composé de $\beta$ et de l’homomorphisme canonique de $F(Y)$ sur $G$, on a $f(w) \neq 1$.

#### Corollaire {#lie-ii-s5-n5-cor-1 .statement}

*L’intersection des sous-groupes distingués d’indice fini de $F(X)$ est réduite à $\{1\}$*.

## EXERCICES {#lie-ii-s5-exercises}

Dans les exercices ci-dessous, les hypothèses et notations sont celles du § 5. On note F le groupe libre $F(X)$, et g l’unique homomorphisme de F dans le groupe de Magnus $\Gamma(X)$ tel que $g(x) = 1 + x$ pour tout $x \in X$ (cf. th. 1).

See the [exercises for § 5](exercises/s5/).
