---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: GROUPES DE LIE RÉELS COMPACTS
section: 8
section_title: Transformation de Fourier
lang: fr
source: lie-ix-fr
book_pages: LIE IX.78-LIE IX.87, LIE IX.127-LIE IX.128
pdf_pages: 0081-0090, 0130-0131
extraction: ocr
subsections:
    - "no": 1
      title: Transformées de Fourier des fonctions intégrables
      page: 78
      pdf_page: 81
    - "no": 2
      title: Transformées de Fourier des fonctions indéfiniment dérivables
      page: 81
      pdf_page: 84
    - "no": 3
      title: Transformées de Fourier des fonctions centrales
      page: 84
      pdf_page: 87
    - "no": 4
      title: Fonctions centrales sur G et fonctions sur T
      page: 87
      pdf_page: 90
statements: 9
exercises: 6
content_sha256: d0265b4788235766af102893705b0c165e3e11646e7de504a0891a78f8058d69
---

## § 8. TRANSFORMATION DE FOURIER

On conserve les notations et conventions du paragraphe précédent.

### 1. Transformées de Fourier des fonctions intégrables

Dans ce numéro, on rappelle des définitions et résultats de TS $ ^2 $.
Notons $ \hat{G} $ l’ensemble des classes de représentations irréductibles de G (dans des espaces vectoriels complexes de dimension finie). Pour tout $ u \in \hat{G} $, notons $ E_u $ l’espace

$ ^1 $ La démonstration de loc. cit., qui n’est énoncée que pour les algèbres de Lie semi-simples déployées, est valable directement dans le cas des algèbres réductives déployées.
$ ^2 $ Voir note $ ^1 $, § 7, p. 66.

de $ u $ et $ d(u) $ sa dimension. Il existe des formes hermitiennes positives séparantes sur $ E_u $ invariantes pour $ u $, et deux telles formes sont proportionnelles. On note $ A^* $ (resp. $ \|A\|_\infty $) l’adjoint (resp. la norme) d’un élément $ A $ de $ \mathrm{End}(E_u) $ relativement à l’une quelconque de ces formes ; pour tout $ g \in G $, on a $ u(g)^* = u(g)^{-1} = u(g^{-1}) $ et $ \|u(g)\|_\infty = 1 $; pour tout $ x \in g $, on a $ u(x)^* = -u(x) = u(-x) $.

On munit $ \mathrm{End}(E_u) $ de la structure d’espace hilbertien pour laquelle le produit scalaire est

(1)
$$
\langle A|B \rangle = d(u) \operatorname{Tr}(A^*B) = d(u) \operatorname{Tr}(BA^*) ,
$$
et on pose

(2)
$$
\|A\|_2 = \langle A|A \rangle^{1/2} = (d(u) \operatorname{Tr}(A^*A))^{1/2} .
$$

On a

(3)
$$
\sqrt{d(u)} \|A\|_\infty \leq \|A\|_2 \leq d(u) \|A\|_\infty ,
$$
donc

(4)
$$
|\langle A|B \rangle| \leq d(u)^2 \|A\|_\infty \|B\|_\infty .
$$

Pour tout $ g \in G $, on a $ \|u(g)\|_2 = d(u) $.

Notons $ F(\hat{G}) $ l’algèbre $ \prod_{u \in \hat{G}} \mathrm{End}(E_u) $. On note $ L^2(\hat{G}) $ la somme hilbertienne des espaces hilbertiens $ \mathrm{End}(E_u) $; c’est l’espace des familles $ A = (A_u) \in F(\hat{G}) $ telles que $ \sum_u \|A_u\|_2^2 < \infty $, muni du produit scalaire

(5)
$$
\langle A|B \rangle = \sum_{u \in \hat{G}} \langle A_u|B_u \rangle = \sum_{u \in \hat{G}} d(u) \operatorname{Tr}(A_u^*B_u) .
$$

On note encore $ \| \cdot \|_2 $ la norme hilbertienne sur $ L^2(\hat{G}) $, de sorte qu’on a $ \|A\|_2^2 = \sum_{u \in \hat{G}} \|A_u\|_2^2 $ pour $ A \in L^2(\hat{G}) $.

Si $ f $ est une fonction complexe intégrable sur $ G $, on pose pour tout $ u \in \hat{G} $,

(6)
$$
u(f) = \int_G f(g) u(g) dg \in \mathrm{End}(E_u) .
$$

On a $ \|u(f)\|_\infty \leq \int_G |f(g)| dg = \|f\|_1 $. On appelle cotransformée de Fourier de $ f $ et on note $ \overline{\mathcal{F}}(f) $ la famille $ (u(f))_{u \in \hat{G}} \in F(\hat{G}) $. Si $ f \in L^2(G) $, on a
$$
\|f\|_2^2 = \sum_{u \in \hat{G}} \langle u(f)|u(f) \rangle = \|\overline{\mathcal{F}}(f)\|_2^2 ,
$$
de sorte que $ \overline{\mathcal{F}} $ induit une application linéaire isométrique de l’espace hilbertien $ L^2(G) $ dans l’espace hilbertien $ L^2(\hat{G}) $ : autrement dit pour $ f $ et $ f' $ dans $ L^2(G) $, on a

(7)
$$
\int_G \overline{f(g)} f'(g) dg = \langle \overline{\mathcal{F}}(f)|\overline{\mathcal{F}}(f') \rangle = \sum_{u \in \hat{G}} d(u) \operatorname{Tr}(u(f)^*u(f')) .
$$

Pour $ f $ et $ f' $ dans $ L^1(G) $, le produit de convolution $ f * f' $ de $ f $ et $ f' $ est défini par

$$
(f * f')(h) = \int_G f(hg^{-1}) f'(g) \, dg = \int_G f(g) f'(g^{-1}h) \, dg
$$

(l'intégrale ayant un sens pour presque tout $ h \in G $).

On a $ f * f' \in L^1(G) $ et, pour tout $ u \in \hat{G} $, $ u(f * f') = u(f) u(f') $, donc

(8)
$$
\overline{\mathcal{F}}(f * f') = \overline{\mathcal{F}}(f) \cdot \overline{\mathcal{F}}(f')
$$

Inversement, soit $ A = (A_u)_{u \in \hat{G}} $ un élément de $ F(\hat{G}) $; pour tout $ u \in \hat{G} $, soit $ \mathcal{F}_u A $ la fonction (analytique) sur $ G $ définie par

(9)
$$
(\mathcal{F}_u A)(g) = \langle u(g)|A_u \rangle = d(u) \operatorname{Tr}(A_u u(g)^{-1})
$$

Si $ A \in L^2(\hat{G}) $, la famille $ (\mathcal{F}_u A)_{u \in \hat{G}} $ est sommable dans $ L^2(G) $; on appelle alors transformée de Fourier de $ A $, et on note $ \mathcal{F}(A) $, la somme de cette famille. Les applications $ \overline{\mathcal{F}} $ et $ \mathcal{F} $ sont des isomorphismes réciproques entre les espaces hilbertiens $ L^2(G) $ et $ L^2(\hat{G}) $.

En d'autres termes :

#### Proposition 1 {#lie-ix-s8-prop-1 .statement tag=01GZ}

Toute fonction complexe $ f $ de carré intégrable sur $ G $ est somme dans l'espace hilbertien $ L^2(G) $ de la famille $ (f_u)_{u \in \hat{G}} $, où pour tout $ h \in G $ et tout $ u \in \hat{G} $, on a

(10)
$$
f_u(h) = \langle u(h)|u(f) \rangle = d(u) \int_G f(g) \operatorname{Tr}(u(gh^{-1})) \, dg = d(u) \int_G f(gh) \operatorname{Tr}(u(g)) \, dg .
$$

Choisissons pour tout $ u \in \hat{G} $ une base orthonormale $ B_u $ de $ E_u $, et notons $ (u_{ij}(g)) $ la matrice de $ u(g) $ dans cette base. La prop. 1 signifie aussi que la famille des fonctions $ \sqrt{d(u)} \, u_{ij} $, pour $ u $ dans $ \hat{G} $ et $ i, j $ dans $ B_u $, est une base orthonormale de l'espace $ L^2(G) $.

Si $ f $ est une fonction intégrable sur $ G $ telle que la famille $ (f_u) $ soit uniformément sommable, alors la somme de cette famille est une fonction continue, qui coïncide presque partout avec $ f $; en d'autres termes, si on suppose en outre $ f $ continue, on a pour tout $ h \in G $

(11)
$$
f(h) = \sum_{u \in \hat{G}} d(u) \int_G f(gh) \operatorname{Tr}(u(g)) \, dg .
$$

Inversement, soit $ A \in F(\hat{G}) $; si la famille $ (\mathcal{F}_u A)_{u \in \hat{G}} $ est uniformément sommable, alors la fonction
$$
g \mapsto \sum_{u \in \hat{G}} (\mathcal{F}_u A)(g) = \sum_{u \in \hat{G}} d(u) \operatorname{Tr}(A_u u(g)^{-1})
$$
est une fonction continue sur $ G $, dont $ A $ est la cotransformée de Fourier.

Soit $ f $ une fonction intégrable sur $ G $, et soit $ s \in G $. Notons $ \gamma(s)\ f $ et $ \delta(s)\ f $ les fonctions sur $ G $ définies par $ \gamma(s)\ f = \varepsilon_s * f,\quad \delta(s)\ f = f * \varepsilon_{s^{-1}} $, c'est-à-dire

$$
(\gamma(s)\ f)(g) = f(s^{-1}\ g),\quad (\delta(s)\ f)(g) = f(gs) \text{ pour } g \in G ,
$$

(III, § 3, no 4 et INT, VII, § 1, no 1). On a

$$
u(\gamma(s)\ f) = \int_G f(s^{-1}g)\ u(g)\ dg = \int_G f(g)\ u(sg)\ dg ,
$$

donc

$$(12)\qquad u(\gamma(s)\ f) = u(s)\ u(f) ,$$

et de même,

$$(13)\qquad u(\delta(s^{-1})\ f) = u(f)\ u(s) .$$

Lorsque $ G $ est commutatif, $ \hat{G} $ est l'ensemble sous-jacent au groupe dual de $ G $ (TS, II, § 1, no 1), on a $ d(u) = 1 $ pour tout $ u \in \hat{G} $, et on retrouve les définitions de la transformation de Fourier données en TS, II.

### 2. Transformées de Fourier des fonctions indéfiniment dérivables

Rappelons (III, § 3, no 1, déf. 2) qu'on note $ U(G) $ l'algèbre des distributions sur $ G $ à support contenu dans $ \{e\} $. L'injection canonique de $ g $ dans $ U(G) $ se prolonge en un isomorphisme de l'algèbre enveloppante de l'algèbre de Lie $ g $ sur $ U(G) $ (*loc. cit.*, no 7, prop. 25); nous identifierons dans la suite ces deux algèbres par cet isomorphisme. Si $ f $ est une fonction complexe indéfiniment dérivable sur $ G $ et si $ t \in U(G) $, on note $ L_t f $ et $ R_t f $ les fonctions sur $ G $ définies par

$$
L_t f(g) = \langle \varepsilon_g * t, f \rangle ,\quad R_t f(g) = \langle t * \varepsilon_g, f \rangle
$$

(*cf. loc. cit.*, no 6). On a pour tout $ g \in G $,

$$
L_t \circ \gamma(g) = \gamma(g) \circ L_t ,\quad R_t \circ \delta(g) = \delta(g) \circ R_t .
$$

Soit $ u \in \hat{G} $; notons $ E_u $ l'espace de $ u $. Le morphisme de groupes de Lie $ u : G \to \mathbf{GL}(E_u) $ donne par dérivation un homomorphisme d'algèbres de Lie (réelles) $ g \to \mathrm{End}(E_u) $, d'où un homomorphisme d'algèbres, encore noté $ u $, de $ U(G) $ dans $ \mathrm{End}(E_u) $. Si $ t \in U(G) $ et si $ f $ est une fonction indéfiniment dérivable sur $ G $, on a

$$(14)\qquad u(L_t f) = u(f)\ u(t^\vee) ,\quad u(R_t f) = u(t^\vee)\ u(f) ,$$

où $ t^\vee $ désigne l'image de $ t $ par l'anti-automorphisme principal de $ U(G) $ (I, § 2, no 4); en effet il suffit de le vérifier pour $ t \in g $, auquel cas cela résulte par dérivation des formules (12) et (13) (*cf. III, § 3, no 7, prop. 27).

Pour tout $ u \in \hat{G} $, notons $ \lambda(u) $ le plus grand poids de $ u $ (\S 7, n° 2, th. 1), de sorte que $ u \mapsto \lambda(u) $ est une application bijective de $ \hat{G} $ dans l’ensemble $ X_{++} $ des éléments dominants de $ X(T) $.

Soit $ \Gamma \in U(G) $ un élément de Casimir de $ G $ (\S 7, n° 6); pour tout $ u \in \hat{G} $, l’endomorphisme $ u(\Gamma) $ de $ E_u $ est une homothétie, dont nous noterons $ \tilde{\Gamma}(u) $ le rapport, d’où une application $ u \mapsto \tilde{\Gamma}(u) $ de $ \hat{G} $ dans $ \mathbf{C} $.

Si $ \varphi $ et $ \psi $ sont deux fonctions à valeurs réelles positives sur $ \hat{G} $, on note « $ \varphi \preccurlyeq \psi $ » ou « $ \varphi(u) \preccurlyeq \psi(u) $ » la relation « il existe $ M > 0 $ tel que $ \varphi(u) \leq M \psi(u) $ pour tout $ u \in \hat{G} $ »; c’est une relation de préordre sur l’ensemble des fonctions sur $ \hat{G} $ à valeurs réelles positives.

#### Proposition 2 {#lie-ix-s8-prop-2 .statement tag=01H0}

*Soient* $ m \mapsto \|m\| $ *une norme sur le* $ \mathbf{R}$-*espace vectoriel* $ \mathbf{R} \otimes X(T) $ *et* $ \Gamma $ *un élément de Casimir de* $ G $. *Soit* $ \varphi $ *une fonction sur* $ \hat{G} $ *à valeurs réelles positives.*

a) *Les conditions suivantes sont équivalentes :*

(i) *Il existe un entier* $ n > 0 $ *tel que* $ \varphi(u) \preccurlyeq (\|\lambda(u)\| + 1)^n $ *(resp. pour tout entier* $ n > 0 $, *on a* $ \varphi(u) \preccurlyeq (\|\lambda(u)\| + 1)^{-n} $).

(ii) *Il existe un entier* $ n > 0 $ *tel que* $ \varphi(u) \preccurlyeq (\tilde{\Gamma}(u) + 1)^n $ *(resp. pour tout entier* $ n > 0 $, *on a* $ \varphi(u) \preccurlyeq (\tilde{\Gamma}(u) + 1)^{-n} $).

b) *Si* $ G $ *est semi-simple, les conditions* (i) *et* (ii) *ci-dessus équivalent aussi à :*

(iii) *Il existe un entier* $ n > 0 $ *tel que* $ \varphi(u) \preccurlyeq d(u)^n $ *(resp. pour tout entier* $ n > 0 $, *on a* $ \varphi(u) \preccurlyeq d(u)^{-n} $).

Notons d’abord que la condition (i) est évidemment indépendante de la norme choisie. On peut donc prendre pour norme celle qui est définie par la forme quadratique $ Q_\Gamma $ associée à $ \Gamma $ (\S 7, n° 6, prop. 4). On a alors

$$
0 \leq \tilde{\Gamma}(u) = \|\lambda(u) + \rho\|^2 - \|\rho\|^2,
$$

donc $ \tilde{\Gamma}(u) + 1 \preccurlyeq (\|\lambda(u)\| + 1)^2 \preccurlyeq \tilde{\Gamma}(u) + 1 $, d’où a).

Par ailleurs, si $ G $ est semi-simple, on a (\S 7, n° 5, cor. 1 au th. 3)

$$
\|\lambda(u) + \rho\| \preccurlyeq d(u) \preccurlyeq \|\lambda(u) + \rho\|^N,\quad \text{où } N = 1/2\ (\dim G - \dim T),
$$

donc $ \|\lambda(u)\| + 1 \preccurlyeq d(u) \preccurlyeq (\|\lambda(u)\| + 1)^N $, d’où b).

Il résulte de la prop. 2 que la condition (i) est indépendante du tore maximal, de la chambre, et de la norme choisie, et que la condition (ii) est indépendante de l’élément de Casimir choisi. Une fonction $ \varphi $ satisfaisant aux conditions (i) et (ii) est dite à *croissance modérée* (resp. à *décroissance rapide*). Le produit de deux fonctions à croissance modérée est à croissance modérée ; le produit d’une fonction à croissance modérée par une fonction à décroissance rapide est à décroissance rapide. Si $ \varphi $ est à décroissance rapide, la famille $ (\varphi(u))_{u \in \hat{G}} $ est sommable.

#### Exemple {#lie-ix-s8-n2-exa-1 .statement tag=01H1}

La fonction $ u \mapsto d(u) $ est à croissance modérée (\S 7, n° 5, cor. 1 au th. 3); pour toute norme $ \| $ sur $ \mathbf{R} \otimes X(T) $, la fonction $ u \mapsto \|\lambda(u)\| $ est à croissance modérée. Pour tout élément de Casimir $ \Gamma $, la fonction $ u \mapsto \tilde{\Gamma}(u) $ est à croissance modérée ; plus généralement :

#### Proposition 3 {#lie-ix-s8-prop-3 .statement tag=01H2}

Pour tout $ t \in \mathrm{U}(G) $, les fonctions $ u \mapsto \|u(t)\|_{\infty} $ et $ u \mapsto \|u(t)\|_2 $ sont à croissance modérée sur $ \hat{G} $.

Puisque le produit de deux fonctions à croissance modérée est à croissance modérée, il suffit de le démontrer lorsque $ t \in g $; dans ce cas l’assertion résulte de la remarque du § 7, no 6 et de l’inégalité

$$
\|u(t)\|_2 \leq d(u) \|u(t)\|_{\infty}.
$$

#### Théorème 1 {#lie-ix-s8-thm-1 .statement tag=01H3}

a) Soit $ f $ une fonction complexe indéfiniment dérivable sur $ G $. Alors la famille $ (f_u)_{u \in \hat{G}} $, où $ f_u(g) = \langle u(g)|u(f) \rangle $, est uniformément sommable sur $ G $, et on a pour tout $ h \in G $

$$
f(h) = \sum_{u \in \hat{G}} \langle u(h)|u(f) \rangle = \sum_{u \in \hat{G}} d(u) \int_G f(g) \operatorname{Tr}(u(gh^{-1})) \, dg.
$$

b) Soit $ f $ une fonction intégrable sur $ G $; pour que $ f $ soit presque partout égale à une fonction indéfiniment dérivable, il faut et il suffit que la fonction $ u \mapsto \|u(f)\|_{\infty} $ soit à décroissance rapide sur $ \hat{G} $.

Soit $ f $ une fonction indéfiniment dérivable sur $ G $, et soit $ \Gamma $ un élément de Casimir pour $ G $; d’après la formule (14), on a pour tout entier $ n \geq 0 $

$$
\tilde{\Gamma}(u)^n u(f) = u(f) u(\Gamma)^n = u((L_{\Gamma})^n f),
$$

et par conséquent

$$
\tilde{\Gamma}(u)^n \|u(f)\|_{\infty} \leq \|(L_{\Gamma})^n f\|_1 \leq \sup_{g \in G} |((L_{\Gamma})^n f)(g)|;
$$

la fonction $ u \mapsto \|u(f)\|_{\infty} $ est donc bien à décroissance rapide.

Inversement, soit $ A = (A_u)_{u \in \hat{G}} $ un élément de $ F(\hat{G}) $ tel que la fonction $ u \mapsto \|A_u\|_{\infty} $ soit à décroissance rapide. Posons $ f_u(g) = \langle u(g)|A_u \rangle $; la fonction $ g \mapsto f_u(g) $ est analytique, donc indéfiniment dérivable. Pour tout $ x \in g $, on a d’après III, § 3, no 7, prop. 27 :

$$
(L_x f_u)(g) = \langle u(g) \, u(x)|A_u \rangle.
$$

Soit $ t \in \mathrm{U}(G) $; d’après la formule précédente, on a

$$
(L_t f_u)(g) = \langle u(g) \, u(t)|A_u \rangle
$$

et par suite

$$
|(L_t f_u)(g)| = |\langle u(g) \, u(t)|A_u \rangle| \leq d(u)^2 \|u(t)\|_{\infty} \|u(g)\|_{\infty} \|A_u\|_{\infty} = d(u)^2 \|u(t)\|_{\infty} \|A_u\|_{\infty}.
$$

La fonction $ u \mapsto \sup_g |(L_t f_u)(g)| $ est donc à décroissance rapide, puisque $ d(u) $ et $ \|u(t)\|_{\infty} $ sont à croissance modérée (prop. 3) et $ \|A_u\|_{\infty} $ à décroissance rapide ; la famille

(L_{t}f_{u})_{u\in\hat{G}} est donc uniformément sommable. On en déduit $ ^1 $ que la somme de la famille $(f_{u})$ est une fonction indéfiniment dérivable sur $ G $, dont la cotransformée de Fourier est $(A_{u})$, d'où le théorème.

Notons $ \mathcal{S}(\hat{G}) $ le sous-espace vectoriel de $ L^{2}(\hat{G}) $ formé des familles $ A = (A_{u})_{u\in\hat{G}} $ telles que la fonction $ u \mapsto \|A_{u}\|_{\infty} $ soit à décroissance rapide sur $ \hat{G} $. Il résulte du théorème que les applications $ \overline{\mathcal{F}} : f \mapsto (u(f))_{u\in\hat{G}} $ et $ \mathcal{F} : A \mapsto \sum_{u\in\hat{G}} \langle u(g)|A_{u} \rangle $ induisent des isomorphismes réciproques entre les espaces vectoriels complexes $ \mathcal{C}^{\infty}(G ; \mathbf{C}) $ et $ \mathcal{S}(\hat{G}) $. Munissons l'espace $ \mathcal{C}^{\infty}(G ; \mathbf{C}) $ de la topologie de la $ C^{\infty} $-convergence uniforme ($ \S 6 $, n° 4) qui peut être définie par la famille des semi-normes $ f \mapsto \sup_{g\in G} |L_{t}f(g)| $ pour $ t \in U(G) $, et l'espace $ \mathcal{S}(\hat{G}) $ de la topologie définie par la suite des semi-normes $ p_{n} : A \mapsto \sup_{u\in\hat{G}} (\tilde{\Gamma}(u) + 1)^{n} \|A_{u}\|_{\infty} $. La formule (15) de la démonstration précédente entraîne que $ \overline{\mathcal{F}} $ est continue. Soient $ t \in U(G) $, $ A = (A_{u})_{u\in\hat{G}} $ un élément de $ \mathcal{S}(\hat{G}) $; posons $ f_{u}(g) = \langle u(g)|A_{u} \rangle $. Soit $ p $ un entier tel que $ \sum_{u\in\hat{G}} \tilde{\Gamma}(u)^{-p} = M < \infty $. D'après la démonstration précédente, il existe un entier positif $ m $ tel qu'on ait, pour tout $ g \in G $,

$$
|(L_{t}f_{u})(g)| \leq d(u)^{2} \|u(t)\|_{\infty} \|A_{u}\|_{\infty} \leq m.(1 + \tilde{\Gamma}(u))^{m} \tilde{\Gamma}(u)^{-p} \|A_{u}\|_{\infty}
$$

d'où $ |(L_{t}\mathcal{F}(A))(g)| \leq mM_{p_{m}}(A) $; ceci prouve que $ \mathcal{F} $ est continue. Par conséquent :

#### Corollaire {#lie-ix-s8-n2-cor-1 .statement tag=01H4}

Les applications $ \overline{\mathcal{F}} : f \mapsto (u(f))_{u\in\hat{G}} $ et $ \mathcal{F} : A \mapsto \sum_{u\in\hat{G}} \langle u(g)|A_{u} \rangle $ induisent des isomorphismes réciproques entre les espaces vectoriels topologiques $ \mathcal{C}^{\infty}(G ; \mathbf{C}) $ et $ \mathcal{S}(\hat{G}) $.

### 3. Transformées de Fourier des fonctions centrales

Pour tout $ u \in \hat{G} $, notons $ \chi_{u} $ le caractère de $ u $; on a donc

$$(16)$$
$$
\chi_{u}(g) = \operatorname{Tr}(u(g)), \quad (g \in G).
$$

Rappelons (TS) les formules

$$(17)$$
$$
\chi_{u} * \chi_{v} = 0 \qquad (u, v \in \hat{G}, u \neq v)
$$

$$(18)$$
$$
\chi_{u} * \chi_{u} = \frac{1}{d(u)} \chi_{u} \quad (u \in \hat{G}).
$$

$ ^1 $ Cela résulte de ce que l'espace $ \mathcal{C}^{\infty}(G ; \mathbf{C}) $, muni de la topologie de la $ C^{\infty} $-convergence uniforme ($ \S 6 $, n° 4), est complet.

Pour tout $ u \in \hat{G} $, notons $ \varepsilon_u $ l’application identique de $ E_u $. Rappelons (\S 7, n° 4) qu’on note $ ZL^2(G) $ le sous-espace de $ L^2(G) $ formé des classes de fonctions $ f $ qui sont centrales, c’est-à-dire telles que $ f \circ \mathrm{Int}\ s = f $ pour tout $ s \in G $, ou de manière équivalente $ \gamma(s)\ f = \delta(s^{-1})\ f $ pour tout $ s \in G $.

#### Proposition 4 {#lie-ix-s8-prop-4 .statement tag=01H5}

*Soit $ f \in L^2(G) $. Pour que $ f $ soit centrale, il faut et il suffit que $ u(f) $ soit une homothétie pour tout $ u \in \hat{G} $. On a alors*

$$
u(f) = \frac{\varepsilon_u}{d(u)} \int_G f(g) \chi_u(g) \, dg .
$$

D’après la prop. 1 (n° 1), dire que $ f $ est centrale signifie qu’on a $ u(\gamma(s)\ f) = u(\delta(s^{-1})f) $ pour tout $ s \in G $ et tout $ u \in \hat{G} $; mais cela s’écrit aussi $ u(s)\ u(f) = u(f)\ u(s) $ pour tout $ s \in G $ et tout $ u \in \hat{G} $ (formules (12) et (13)), d’où la première assertion de la prop. 4 (lemme de Schur). Si $ u(f) $ est une homothétie, on a $ u(f) = \lambda_u \varepsilon_u $ avec

$$
\lambda_u = \frac{1}{d(u)} \mathrm{Tr}\,(u(f)) = \frac{1}{d(u)} \int_G f(g) \mathrm{Tr}\,(u(g)) \, dg = \frac{1}{d(u)} \int_G f(g) \chi_u(g) \, dg .
$$

Pour $ f \in ZL^2(G) $, on a par conséquent

$$
u(f) = \langle \overline{\chi_u}|f\rangle \frac{\varepsilon_u}{d(u)} ,
$$

donc

$$
\overline{\mathcal{F}}(f) = \left( \langle \overline{\chi_u}|f\rangle \frac{\varepsilon_u}{d(u)} \right)_{u \in \hat{G}} .
$$

avec

$$
\| \overline{\mathcal{F}}(f) \|_2^2 = \sum_u \left\| \langle \overline{\chi_u}|f\rangle \frac{\varepsilon_u}{d(u)} \right\|_2^2 = \sum_u | \langle \overline{\chi_u}|f\rangle |^2 .
$$

Inversement, si $ \varphi $ est une fonction complexe de carré intégrable sur $ \hat{G} $, alors l’élément $ \left( \frac{\varphi(u)}{d(u)} \varepsilon_u \right)_{u \in \hat{G}} $ de $ F(\hat{G}) $ appartient à $ L^2(\hat{G}) $, et on a (formule (9))

$$
\left( \mathcal{F}_u \left( \frac{\varphi(u)}{d(u)} \varepsilon_u \right) \right)(g) = d(u) \mathrm{Tr} \left( \frac{\varphi(u)}{d(u)} \varepsilon_u u(g)^{-1} \right) = \varphi(u) \overline{\chi_u}(g) ,
$$

donc

$$
\mathcal{F} \left( \left( \frac{\varphi(u)}{d(u)} \varepsilon_u \right) \right) = \sum_{u \in \hat{G}} \varphi(u) \overline{\chi_u} .
$$

Notons que les formules (20) et (21) donnent en particulier pour $ u, v $ dans $ \hat{G} $

$$
u(\overline{\chi}_v) = 0 \quad \text{si} \quad u \neq v,
$$
$$
u(\overline{\chi}_u) = \frac{\varepsilon_u}{d(u)} \in \mathrm{End}(E_u),
$$
$$
\overline{F}(\chi_u) = \frac{\varepsilon_u}{d(u)} \in \mathrm{End}(E_u) \subset F(\hat{G}) . \tag{25}
$$

#### Proposition 5 {#lie-ix-s8-prop-5 .statement tag=01H6}

*Soit $ f $ une fonction continue centrale sur $ G $. Pour que $ f $ soit indéfiniment dérivable, il faut et il suffit que la fonction $ u \mapsto |\langle \chi_u | f \rangle| $ soit à décroissance rapide sur $ \hat{G} $; on a alors pour tout $ g \in G $*

$$
f(g) = \sum_{u \in \hat{G}} \langle \chi_u | f \rangle \chi_u(g) .
$$

D’après le th. 1, *b)*, la fonction $ \overline{f} $ est indéfiniment dérivable si et seulement si la fonction $ u \mapsto \| u(\overline{f}) \|_\infty $ est à décroissance rapide ; mais d’après (20), on a

$$
\| u(\overline{f}) \|_\infty = \frac{1}{d(u)} |\langle \chi_u | f \rangle| ,
$$

d’où la première assertion, puisque les fonctions $ d(u) $ et $ \frac{1}{d(u)} $ sont à croissance modérée.

Supposons $ f $ indéfiniment dérivable ; alors d’après le th. 1, *a)*, on a pour tout $ g \in G $,

$$
f_u(g) = \langle u(g) | u(f) \rangle = d(u) \operatorname{Tr}(u(g)^{-1} \cdot u(f)) = d(u) \operatorname{Tr}\left( u(g)^{-1} \langle \overline{\chi}_u | f \rangle \frac{\varepsilon_u}{d(u)} \right)
$$
$$
= \langle \overline{\chi}_u | f \rangle \operatorname{Tr}(u(g)^{-1}) = \langle \overline{\chi}_u | f \rangle \overline{\chi}_u(g) .
$$

Donc $ f(g) = \sum_{u \in \hat{G}} \langle \overline{\chi}_u | f \rangle \overline{\chi}_u(g) $; mais, pour tout $ u \in \hat{G} $, la représentation contragrédiente $ u' $ de $ u $ satisfait à $ \overline{\chi}_u = \chi_{u'} $ et l’application $ u \mapsto u' $ est une permutation de $ \hat{G} $; on a donc aussi $ f(g) = \sum_{u \in \hat{G}} \langle \chi_u | f \rangle \chi_u(g) $, d’où la proposition.

#### Corollaire {#lie-ix-s8-n3-cor-1 .statement tag=01H7}

*Soit $ f $ une fonction continue centrale sur $ G $. Pour que $ f $ soit indéfiniment dérivable, il faut et il suffit que la restriction de $ f $ à $ T $ soit indéfiniment dérivable.*

En effet, d’après le cor. 4 du § 7, n° 4, on a

$$
\langle \chi_u | f \rangle = \int_G \overline{\lambda(u)(t)} \varphi(t) \, dt , \quad \text{où} \quad \varphi(t) = \prod_{\alpha > 0} (1 - \alpha(t)^{-1}) f(t) .
$$

1. On plonge $ \mathrm{End}(E_u) $ dans le produit $ F(\hat{G}) = \prod_{v \in \hat{G}} \mathrm{End}(E_v) $ en associant à tout $ A \in \mathrm{End}(E_u) $ la famille $ (A_v)_{v \in \hat{G}} $ telle que $ A_u = A $ et $ A_v = 0 $ pour $ v \neq u $.

Si $ f|T $ est indéfiniment dérivable, $ \varphi $ l’est aussi ; d’après la prop. 5, appliquée au groupe T, la fonction $ \mu \mapsto \int_T \overline{\mu(t)}\, \varphi(t)\, dt $ sur $ \hat{T} = X(T) $ est alors à décroissance rapide, et il en est de même de la fonction $ u \mapsto \langle \chi_u | f \rangle $; la fonction $ f $ est donc indéfiniment dérivable (prop. 5). La réciproque est évidente.

### 4. Fonctions centrales sur G et fonctions sur T

Notons $ \mathcal{C}(G) $ l’espace des fonctions continues complexes sur G et $ \mathcal{C}^\infty(G) $ le sous-espace des fonctions indéfiniment dérivables. On a donc une suite d’inclusions

$$
\Theta(G) \subset \mathcal{C}^\infty(G) \subset \mathcal{C}(G) \subset L^2(G).
$$

Notons $ Z\Theta(G), Z\mathcal{C}^\infty(G), Z\mathcal{C}(G), ZL^2(G) $ respectivement les sous-espaces formés des fonctions centrales dans ces divers espaces. Introduisons de même les espaces $ \Theta(T), \mathcal{C}^\infty(T), \mathcal{C}(T) $ et $ L^2(T) $; pour tout espace E de cette liste, notons $ E^W $ (resp. $ E^{-W} $) le sous-espace formé des éléments invariants (resp. anti-invariants) pour l’action du groupe W. On a un diagramme commutatif

$$
\begin{array}{ccc}
Z\mathcal{C}(G) & \xrightarrow{a_c} & \mathcal{C}(T)^W \\
& & \\
Z\mathcal{C}^\infty(G) & \xrightarrow{a_\infty} & \mathcal{C}^\infty(T)^W \\
& & \\
Z\Theta(G) & \xrightarrow{a_\Theta} & \Theta(T)^W
\end{array}
$$

où les flèches verticales représentent les injections canoniques, et où les applications $ a_c, a_\infty, a_\Theta $ sont induites par l’application de restriction de $ \mathcal{C}(G) $ dans $ \mathcal{C}(T) $.

Les applications $ a_c, a_\infty, a_\Theta $ sont *bijectives* (\S 2, no 5, cor. 1 à la prop. 5, \S 8, no 3, cor. à la prop. 5, et \S 7, no 3, cor. à la prop. 2).

Supposons maintenant que la demi-somme $ \rho $ des racines positives appartienne à $ X(T) $ et considérons l’application $ b $ qui à chaque fonction continue $ \varphi $ sur T associe $ \varphi . J(\rho) $. On a un diagramme commutatif

$$
\begin{array}{cccccc}
ZL^2(G) & \xrightarrow{u} & L^2(T)^{-W} \\
& & \\
Z\mathcal{C}(G) & \xrightarrow{a_c} & \mathcal{C}(T)^W & \xrightarrow{b_c} & \mathcal{C}(T)^{-W} \\
& & \\
Z\mathcal{C}^\infty(G) & \xrightarrow{a_\infty} & \mathcal{C}^\infty(T)^W & \xrightarrow{b_\infty} & \mathcal{C}^\infty(T)^{-W} \\
& & \\
Z\Theta(G) & \xrightarrow{a_\Theta} & \Theta(T)^W & \xrightarrow{b_\Theta} & \Theta(T)^{-W}
\end{array}
$$

où les flèches verticales sont les inclusions canoniques, les applications $ b_c, b_\infty, b_\Theta $ sont induites par $ b $, et où $ u $ prolonge $ b_c \circ a_c $ par continuité (\S 7, no 4, cor. 3 au th. 2). Les applications $ u $ et $ b_\Theta $ sont *bijectives* (*loc. cit.*); il en est de même pour $ b_\infty $ (exerc. 5); en revanche, $ b_c $ n’est pas en général surjective (exerc. 6).

## EXERCICES {#lie-ix-s8-exercises}

See the [exercises for § 8](exercises/s8/).
