---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Algèbres de Lie
section: 5
section_title: Algèbres de Lie résolubles
lang: fr
source: lie-i-fr
pdf_pages: 0059-0068, 0123-0126
extraction: ocr
subsections:
    - "no": 1
      title: Définition des algèbres de Lie résolubles
      page: 0
      pdf_page: 60
    - "no": 2
      title: Radical d’une algèbre de Lie
      page: 0
      pdf_page: 61
    - "no": 3
      title: Radical nilpotent d’une algèbre de Lie
      page: 0
      pdf_page: 62
    - "no": 4
      title: Un critère de résolvabilité
      page: 0
      pdf_page: 65
    - "no": 5
      title: Nouvelles propriétés du radical
      page: 0
      pdf_page: 67
    - "no": 6
      title: Extension du corps de base
      page: 0
      pdf_page: 68
statements: 31
exercises: 17
content_sha256: 92c59100943c2827b9f36c287d8bb5cf7fb9727029ae0476849c7530ba5db090
---

## § 5. Algèbres de Lie résolubles

On rappelle que K désigne désormais un corps de caractéristique 0 et que toutes les algèbres de Lie sont supposées de dimension finie sur K.¹

¹ Le lecteur remarquera que l’hypothèse sur la caractéristique de K n’est pas employée dans les numéros 1 et 2 du présent paragraphe.

### 1. Définition des algèbres de Lie résolubles

#### Définition 1 {#lie-i-s5-def-1 .statement}

Une algèbre de Lie g est dite résoluble si sa k-ième algèbre dérivée $\mathcal{D}^k g$ est nulle pour k assez grand.

Une algèbre de Lie nilpotente est résoluble.

#### Proposition 1 {#lie-i-s5-prop-1 .statement}

Une sous-algèbre, une algèbre quotient d’une algèbre de Lie résoluble sont résolubles. Toute extension d’une algèbre résoluble par une algèbre résoluble est résoluble. Tout produit fini d’algèbres résolubles est résoluble.

Soient g une algèbre de Lie, g' une sous-algèbre, h un idéal de g, $\mathfrak{k} = g/h$, et $\varphi$ l’application canonique de g sur $\mathfrak{k}$. Si g est résoluble, on a $\mathcal{D}^k g = \{0\}$ pour un entier k, donc $\mathcal{D}^k g' \subset \mathcal{D}^k g = \{0\}$, et $\mathcal{D}^k \mathfrak{k} = \varphi(\mathcal{D}^k g) = \{0\}$, donc g' et $\mathfrak{k}$ sont résolubles. Si h et $\mathfrak{k}$ sont résolubles, il existe des entiers s, t tels que $\mathcal{D}^s h = \mathcal{D}^t \mathfrak{k} = \{0\}$; on a alors $\mathcal{D}^t g \subset h$, donc $\mathcal{D}^{s+t} g = \mathcal{D}^s (\mathcal{D}^t g) \subset \mathcal{D}^s h = \{0\}$, et g est résoluble. La dernière assertion résulte de la deuxième par récurrence sur le nombre des facteurs.

#### Proposition 2 {#lie-i-s5-prop-2 .statement}

Soit g une algèbre de Lie. Les conditions suivantes sont équivalentes :

a) g est résoluble ;
b) il existe une suite décroissante $g = g_0 \supset g_1 \supset \cdots \supset g_n = \{0\}$ d’idéaux de g tels que les algèbres $g_i / g_{i+1}$ soient commutatives ($i = 0, 1, \ldots, n-1$) ;
c) il existe une suite décroissante $g = g'_0 \supset g'_1 \supset \cdots \supset g'_p = \{0\}$ de sous-algèbres de g telles que $g'_{i+1}$ soit un idéal dans $g'_i$ et que $g'_i / g'_{i+1}$ soit commutative ($i = 0, 1, \ldots, p-1$).
d) Il existe une suite décroissante $g = g''_0 \supset g''_1 \supset \cdots \supset g''_q = \{0\}$ de sous-algèbres de g telles que $g''_{i+1}$ soit un idéal de codimension 1 dans $g''_i$ ($i = 0, 1, \ldots, q-1$).

a) $\Rightarrow$ b) : il suffit de considérer la suite des idéaux dérivés de g.
b) $\Rightarrow$ c) : c’est évident.
c) $\Rightarrow$ d) : supposons la condition c) satisfaite ; tout sous-espace vectoriel de $g'_i$ contenant $g'_{i+1}$ est un idéal de $g'_i$, d’où aussitôt d).
d) $\Rightarrow$ a) ; ceci résulte du fait qu’une extension d’une algèbre résoluble par une algèbre résoluble est résoluble.

Exemples d’algèbres de Lie résolubles.

I. Soient g un espace vectoriel de dimension 2 sur K, $(e_1, e_2)$ une base de g. Il existe une multiplication bilinéaire alternée $(x, y) \mapsto [x, y]$ et une seule sur g telle que $[e_1, e_2] = e_2$. On vérifie facilement que g est ainsi muni d’une structure d’algèbre de Lie résoluble. Maintenant, soit $h$ une algèbre de Lie non commutative de dimension 2 sur K. On va montrer que $h$ est isomorphe à g. Soit $(f_1, f_2)$ une base de h. L’élément $[f_1, f_2]$ n’est pas nul (sinon h serait commutative), donc il engendre un sous-espace $f$ de dimension 1 de h. On a $[h, h] = f$. Soit $(e'_1, e'_2)$ une base de h telle que $e'_2 \in f$. On a $[e'_1, e'_2] = \lambda e'_2$ avec $\lambda \neq 0$. Remplaçant $e'_1$ par $\lambda^{-1} e_1$, on voit qu’on peut supposer $\lambda = 1$, d’où notre assertion.

II. Les formules (5) du § 1 prouvent que $\mathcal{O}t(n, K) = n(n, K)$. Comme $n(n, K)$ est nilpotente donc résoluble, $t(n, K)$ est résoluble. Par suite, $st(n, K)$ est résoluble. En particulier, $st(2, K)$ est isomorphe à l’algèbre de l’exemple I.

### 2. Radical d’une algèbre de Lie

Soient a, b deux idéaux résolubles d’une algèbre de Lie g. L’algèbre $(a + b)/b$ est isomorphe à $a/(a \cap b)$, donc est résoluble, et $a + b$, qui est extension de $(a + b)/b$ par b, l’est aussi (prop. 1). Il s’ensuit qu’un idéal résoluble maximal de g contient tout idéal résoluble de g, donc que g possède un plus grand idéal résoluble. Ceci légitime la définition suivante :

#### Définition 2 {#lie-i-s5-def-2 .statement}

On appelle radical d’une algèbre de Lie son plus grand idéal résoluble.

#### Proposition 3 {#lie-i-s5-prop-3 .statement}

Le radical r d’une algèbre de Lie g est le plus petit idéal de g tel que $g/r$ ait pour radical $\{0\}$.

Soient a un idéal de g, et $\varphi$ l’application canonique de g sur $g/a$. Si le radical de $g/a$ est nul, alors $\varphi(r)$, qui est un idéal résoluble de $g/a$, est nul ; donc $r \subset a$. D’autre part, l’image réciproque $\varphi^{-1}(r')$ du radical $r'$ de $g/r$ est un idéal de g qui est résoluble d’après la prop. 1, donc est égal à r ; par suite $r' = \{0\}$.

#### Proposition 4 {#lie-i-s5-prop-4 .statement}

Soient $g_1, \ldots, g_n$ des algèbres de Lie. Le radical $r$ du produit des $g_i$ est le produit des radicaux $r_i$ des $g_i$.

Le produit $r'$ des $r_i$ est un idéal résoluble (prop. 1), donc $r' \subset r$. L’image canonique de $r$ dans $g_i$ est un idéal résoluble de $g_i$, donc est contenue dans $r_i$; donc $r \subset r'$.

### 3. Radical nilpotent d’une algèbre de Lie

#### Définition 3 {#lie-i-s5-def-3 .statement}

Soit $g$ une algèbre de Lie. On appelle radical nilpotent de $g$ l’intersection des noyaux des représentations simples de dimension finie de $g$.

#### Remarque 1 {#lie-i-s5-n3-rem-1 .statement}

Soit $s$ le radical nilpotent de $g$. Comme tout suite décroissante de sous-espaces vectoriels de $g$ est stationnaire, il existe un nombre fini de représentations simples de dimension finie de $g$ dont les noyaux ont pour intersection $s$. La somme directe de ces représentations est semi-simple et a pour noyau $s$. Il en résulte que l’ensemble des noyaux des représentations semi-simples de dimension finie de $g$ a un plus petit élément, à savoir $s$.

#### Remarque 2 {#lie-i-s5-n3-rem-2 .statement}

Compte tenu de la prop. 4 c) du § 4, n° 3, $s$ est aussi l’intersection des plus grands idéaux de nilpotence des représentations de dimension finie de $g$. En particulier, $s$ est contenu dans le plus grand idéal nilpotent de $g$, donc est un idéal nilpotent de $g$.

#### Remarque 3 {#lie-i-s5-n3-rem-3 .statement}

Toute forme linéaire $\lambda$ sur $g$ qui est nulle sur $\mathcal{O}g$ est une représentation simple (d’espace $K$) de $g$, d’où $\lambda(s) = \{0\}$. Il en résulte que $s \subset \mathcal{O}g$. Par ailleurs, $s$ est contenu dans le radical $r$ de $g$ d’après la remarque 2. Nous allons démontrer que $s = r \cap \mathcal{O}g$.

#### Lemme 1 {#lie-i-s5-lem-1 .statement}

Soient $V$ un espace vectoriel de dimension finie sur $K$, $g$ une sous-algèbre de $\mathrm{gl}(V)$ telle que $V$ soit un $g$-module simple, $a$ un idéal commutatif de $g$. On a alors $a \cap \mathcal{O}g = \{0\}$.

Soit $(V_i)_{0 \leq i \leq r}$ une suite de Jordan-Hölder du $a$-module $V$. Soit $S$ la sous-algèbre de $\mathcal{L}(V)$ engendrée par $1$ et $a$.

Si $b$ est un idéal de $g$ contenu dans $a$ et tel que l’on ait $\mathrm{Tr}\, bs = 0$ pour tout $b \in b$ et tout $s \in S$, on a en particulier, par définition de $S$, $\mathrm{Tr}\,(b^n) = 0$ pour tout entier $n > 0$, donc $b$ est nilpotent

#### Théorème 1 {#lie-i-s5-thm-1 .statement}

Soient g une algèbre de Lie, r son radical, et s son radical nilpotent. On a alors s = $\mathcal{O}g \cap r$.

On sait déjà que s ⊂ $\mathcal{O}g \cap r$. Il suffira donc de montrer que, si ρ est une représentation simple de dimension finie de g, on a $\rho(\mathcal{O}g \cap r) = \{0\}$. Soit k le plus petit entier ≥ 0 tel que $\rho(\mathcal{O}^{k+1}r) = \{0\}$; posons $g' = \rho(g)$, $a' = \rho(\mathcal{O}^k r)$; comme $\mathcal{O}^k r$ est un idéal de g, $a'$ est un idéal de $g'$; cet idéal est commutatif puisque $\rho(\mathcal{O}^{k+1}r) = \{0\}$. Si V est l’espace de ρ, on a $g' \subset \mathrm{gl}(V)$ et V est un $g'$-module simple. Alors, $\rho(\mathcal{O}g \cap \mathcal{O}^k r) \subset \mathcal{O}g' \cap a' = \{0\}$. Si on avait $k > 0$, on aurait $\mathcal{O}^k r \subset \mathcal{O}g$, $\rho(\mathcal{O}^k r) = \{0\}$, contrairement à la définition de k. Donc $k = 0$, c’est-à-dire que $\rho(\mathcal{O}g \cap r) = \{0\}$.

#### Corollaire 1 {#lie-i-s5-thm-1-cor-1 .statement}

Soit g une algèbre de Lie résoluble. Le radical nilpotent de g est $\mathcal{O}g$. Si ρ est une représentation simple de dimension finie de g, $\rho(g)$ est commutative, et l’algèbre associative L engendrée par 1 et $\rho(g)$ est un corps de degré fini sur K.

On a ici r = g, d’où s = $\mathcal{O}g$. Donc $\rho(\mathcal{O}g) = \{0\}$, ce qui montre que $g' = \rho(g)$ est commutative. Tout élément ≠ 0 de L est invér-sible en vertu du lemme de Schur ; L est donc un corps.

#### Corollaire 2 (théorème de Lie) {#lie-i-s5-thm-1-cor-2 .statement}

Soit g une algèbre de Lie résoluble ; supposons K algébriquement clos. Soit M un g-module de dimension finie sur K, et soit $(M_i)_{0 \leq i \leq r}$ une suite de Jordan-Hölder de M. Alors, $M_{i-1}/M_i$ est de dimension 1 sur K pour $1 \leq i \leq r$, et, pour tout $x \in g$, on a $x_{M_{i-1}/M_i} = \lambda_i(x) \cdot 1$, $\lambda_i$ étant une forme linéaire sur g nulle sur $\mathcal{O}g$. En particulier, tout g-module simple de dimension finie sur K est en fait de dimension 1.

Soit $\rho_i$ la représentation de $g$ dans $M_{i-1}/M_i$. L’algèbre associative $L_i$ engendrée par 1 et $\rho_i(g)$ est un corps, extension de degré fini de $K$, donc égal à $K$; et $M_{i-1}/M_i$ est un $L_i$-module simple, d’où $\dim M_{i-1}/M_i = 1$. Le reste du corollaire est évident.

#### Remarque 4 {#lie-i-s5-n3-rem-4 .statement}

Si on remplace $(M_i)_{0 \leq i \leq r}$ par une autre suite de Jordan-Hölder de $M$, la suite $(\lambda_1, \ldots, \lambda_r)$ est remplacée par une suite de la forme $(\lambda_{\pi(1)}, \ldots, \lambda_{\pi(r)})$, où $\pi$ est une permutation de $\{1, \ldots, r\}$, comme il résulte du théorème de Jordan-Hölder.

#### Remarque 5 {#lie-i-s5-n3-rem-5 .statement}

Soit $(e_1, \ldots, e_r)$ une base de $M$ telle que $e_i \in M_{i-1},\ e_i \notin M_i$ $(1 \leq i \leq r)$. Si $x \in g$, l’endomorphisme de $M$ qui correspond à $x$ est représenté par rapport à cette base par une matrice triangulaire dont les coefficients diagonaux sont $\lambda_1(x), \ldots, \lambda_r(x)$.

#### Corollaire 3 {#lie-i-s5-thm-1-cor-3 .statement}

Supposons $K$ algébriquement clos. Si $g$ est une algèbre de Lie résoluble de dimension $r$, tout idéal de $g$ est un terme d’une suite décroissante d’idéaux de dimensions $r, r-1, \ldots, 0$.

En effet, tout idéal fait partie d’une suite de Jordan-Hölder de $g$, considéré comme espace de la représentation adjointe (Alg., chap. I, § 6, no 14, cor. du th. 8) ; il suffit alors d’appliquer le cor. 2.

#### Corollaire 4 {#lie-i-s5-thm-1-cor-4 .statement}

Supposons que $K = \mathbf{R}$. Soit $g$ une algèbre de Lie résoluble. Toute représentation simple de $g$ est de dimension $\leq 2$. Tout idéal de $g$ est un terme d’une suite décroissante $(g_i)_{0 \leq i \leq m}$ d’idéaux telle que $g_0 = g, g_m = \{0\}, \dim g_{i-1}/g_i \leq 2$ $(1 \leq i \leq m)$.

Cela se démontre de la même manière que les cor. 2 et 3, tenant compte de ce que toute extension algébrique de $\mathbf{R}$ est de degré $\leq 2$.

#### Corollaire 5 {#lie-i-s5-thm-1-cor-5 .statement}

Pour qu’une algèbre de Lie $g$ soit résoluble, il faut et suffit que $\mathcal{O}g$ soit nilpotente.

La condition est nécessaire en vertu du cor. 1. Elle est suffisante puisque $g/\mathcal{O}g$ est commutative.

#### Corollaire 6 {#lie-i-s5-thm-1-cor-6 .statement}

Soit $\rho$ une représentation de dimension finie d’une algèbre de Lie $g$. Soit $r$ le radical de $g$. Tout élément $x \in r$ tel que $\rho(x)$ soit nilpotent appartient au plus grand idéal de nilpotence $n$ de $\rho$.

Soit V l’espace de ρ ; soit (V_i)_{0 \leq i \leq r} une suite de Jordan-Hölder pour la structure de r-module de V, et soit ρ_i la représentation de r d’espace V_i/V_{i-1} (1 \leq i \leq r). Si ρ(x) est nilpotent, il en est de même des ρ_i(x) ; comme, pour tout i, l’algèbre engendrée par ρ_i(r) est un corps, on a ρ_i(x) = 0. Réciproquement, si ρ_i(x) = 0 pour tout i, ρ(x) = 0. Ceci montre que l’ensemble a des x \in r tels que ρ(x) soit nilpotent est un idéal de r. D’autre part, [g, a] \subset \mathfrak{g} \cap r \subset n \cap r \subset a, donc a est un idéal de g. Ceci prouve que a \subset n.

#### Corollaire 7 {#lie-i-s5-thm-1-cor-7 .statement}

Soient g une algèbre de Lie, r son radical. Les quatre ensembles suivants sont identiques : a) le plus grand idéal nilpotent de g ; b) le plus grand idéal nilpotent de r ; c) l’ensemble des x \in r tels que ad_g x soit nilpotent ; d) l’ensemble des x \in r tels que ad_r x soit nilpotent.

Désignons par a, b, c, d ces quatre ensembles. Les inclusions a \subset b \subset d \subset c sont claires. On a c \subset a d’après le cor. 6 appliqué à la représentation adjointe de g.

### 4. Un critère de résolvabilité

#### Lemme 2 {#lie-i-s5-lem-2 .statement}

Soient x un endomorphisme d’un espace vectoriel V de dimension finie, et s (resp. n) sa composante semi-simple (resp. nilpotente) (cf. Alg., chap. VIII, § 9, no 4, déf. 4). Soient ad x, ad s, ad n les images respectives de x, s, n dans la représentation adjointe de gl(V). Alors ad s (resp. ad n) est la composante semi-simple (resp. nilpotente) de ad x, et est égal à un polynôme en ad x, à coefficients dans K, sans terme constant.

On a ad x = ad s + ad n, [ad s, ad n] = 0, et ad n est nilpotent (§ 4, lemme 1). Montrons que ad s est semi-simple. Il suffit de le faire pour K algébriquement clos (cf. Alg., chap. VIII, § 9, no 2, prop. 3). Soit alors (e_i)_{1 \leq i \leq n} une base de V telle que s(e_i) = \lambda_i e_i (\lambda_i \in K). Soit (E_{ij}) la base canonique de \mathbf{M}_n(K) = gl(V). D’après les formules (5) du § 1, on a (ad s).E_{ij} = (\lambda_i - \lambda_j)E_{ij}, donc ad s est semi-simple. La dernière assertion du lemme résulte d’Alg., chap. VIII, § 9, no 4, prop. 8.

#### Lemme 3 {#lie-i-s5-lem-3 .statement}

Soient M un espace vectoriel de dimension finie, A et B deux sous-espaces vectoriels de gl(M) tels que B ⊂ A et T l’ensemble des t ∈ gl(M) tels que [t, A] ⊂ B. Si z ∈ T est tel que Tr (zu) = 0 pour tout u ∈ T, alors z est nilpotent.

Il suffit de faire la démonstration lorsque K est algébriquement clos, ce que nous supposerons désormais. Soient s et n les composantes semi-simple et nilpotente de z, et soit (e_i) une base de M telle que s(e_i) = λ_i e_i (λ_i ∈ K). Soit V ⊂ K l’espace vectoriel sur Q engendré par les λ_i. Il s’agit de montrer que V = {0}. Soit f une forme Q-linéaire sur V, et soit t l’endomorphisme de M tel que te_i = f(λ_i)e_i. Si (E_{ij}) est la base canonique de gl(M) définie par E_{ij}e_k = δ_{jk}e_i, on a

$$
(\mathrm{ad}\, s)E_{ij} = (\lambda_i - \lambda_j)E_{ij}
$$
$$
(\mathrm{ad}\, t)E_{ij} = (f(\lambda_i) - f(\lambda_j))E_{ij}.
$$

Il existe un polynôme P, sans terme constant, à coefficients dans K, tel que P(λ_i - λ_j) = f(λ_i) - f(λ_j) quels que soient i et j (car, si λ_i - λ_j = λ_h - λ_k, on a f(λ_i) - f(λ_j) = f(λ_h) - f(λ_k), et, si λ_i - λ_j = 0, f(λ_i) - f(λ_j) = 0). Alors, ad t = P(ad s). D’autre part, ad s est un polynôme sans terme constant en ad z. Or (ad z)(A) ⊂ B, d’où aussi (ad t)(A) ⊂ B. Vu l’hypothèse, on a 0 = Tr (zt) = Σλ_i f(λ_i), d’où 0 = f(Tr (zt)) = Σ f(λ_i)^2. Puisque les f(λ_i) sont des nombres rationnels, f = 0, ce qui achève la démonstration.

#### Théorème 2 (critère de Cartan) {#lie-i-s5-thm-2 .statement}

Soient g une algèbre de Lie, M un espace vectoriel de dimension finie, ρ une représentation de g dans M, et β la forme bilinéaire sur g associée à ρ. Alors, ρ(g) est résoluble si et seulement si O_g est orthogonal à g pour β.

On peut évidemment se ramener au cas où g est une sous-algèbre de Lie de gl(M) et où ρ est l’application identique. Si g est résoluble, O_g est contenu dans le plus grand idéal de nilpotence de la représentation identique de g (th. 1), donc est orthogonal à g pour β (§ 4, prop. 4 d)). Supposons O_g orthogonal à g pour β, et prouvons que g est résoluble. Soit T l’ensemble des t ∈ gl(M) tels que [t, g] ⊂ O_g. Si t ∈ T et si x, y appartiennent à g, on a [t, x] ∈ O_g, donc

$$
\mathrm{Tr}\,(t[x, y]) = \beta([t, x], y) = 0
$$

d’où par linéarité $\operatorname{Tr}(tu) = 0$ pour tout $u \in \mathcal{O}g$. Par ailleurs, il est clair que $\mathcal{O}g \subset T$. Donc (lemme 3) tout élément de $\mathcal{O}g$ est nilpotent. Il est résulte que $\mathcal{O}g$ est nilpotente ($§ 4$, cor. 3 du th. 1), donc que $g$ est résoluble (no 3, cor. 5 du th. 1).

### 5. Nouvelles propriétés du radical

#### Proposition 5 {#lie-i-s5-prop-5 .statement}

Soient $g$ une algèbre de Lie, $r$ son radical.
a) Si $\rho$ est une représentation de dimension finie de $g$, et si $\beta$ est la forme bilinéaire associée, $r$ et $\mathcal{O}g$ sont orthogonaux pour $\beta$.
b) $r$ est l’orthogonal de $\mathcal{O}g$ pour la forme de Killing.
Soient $x, y$ dans $g, z \in r$. On a $[y, z] \in \mathcal{O}g \cap r$, donc $\beta([x, y], z) = \beta(x, [y, z]) = 0$ (th. 1). D’où a).
Soit $r'$ l’orthogonal de $\mathcal{O}g$ pour la forme de Killing. C’est un idéal de $g$ ($§ 3$, no 6, prop. 7 a)) qui contient $r$ d’après ce qui précède. D’autre part, l’image $s$ de $r'$ par la représentation adjointe de $g$ est résoluble (th. 2), donc $r'$ est résoluble comme extension centrale de $s$. Donc $r' \subset r$.

#### Corollaire 1 {#lie-i-s5-prop-5-cor-1 .statement}

Soit $g$ une algèbre de Lie. Alors, $g$ est résoluble si et seulement si $\mathcal{O}g$ est orthogonal à $g$ pour la forme de Killing.
C’est une conséquence immédiate de la prop. 5 b).

#### Corollaire 2 {#lie-i-s5-prop-5-cor-2 .statement}

Le radical $r$ d’une algèbre de Lie $g$ est un idéal caractéristique.
En effet, $\mathcal{O}g$ est un idéal caractéristique, et la forme de Killing est complètement invariante ($§ 3$, no 6, prop. 10). Donc l’orthogonal de $\mathcal{O}g$ pour la forme de Killing est un idéal caractéristique ($§ 3$, no 6, prop. 7 b)).

#### Corollaire 3 {#lie-i-s5-prop-5-cor-3 .statement}

Soient $g$ une algèbre de Lie, $r$ son radical, $a$ un idéal de $g$. Alors, le radical de $a$ est égal à $r \cap a$.
En effet, $r \cap a$ est un idéal résoluble de $a$, donc est contenu dans le radical $r'$ de $a$. Réciproquement, $r'$ est un idéal de $g$ (cor. 2, et $§ 1$, no 4, prop. 2), donc $r' \subset r$.

Le cor. 2 peut être précisé de la manière suivante :

#### Proposition 6 {#lie-i-s5-prop-6 .statement}

Soient g une algèbre de Lie, r son radical, n son plus grand idéal nilpotent. Toute dérivation de g applique r dans n.

Soit D une dérivation de g. Soit g' = g + Kx_0 une algèbre de Lie dans laquelle g est un idéal de codimension 1, telle que Dx = [x_0, x] pour tout x ∈ g (§ 1, n° 8, exemple 1). D’après le cor. 3 de la prop. 5, r est contenu dans le radical r' de g'. On a D(r) = [x_0, r] ⊂ [g', g'] ∩ r' = s'. Pour tout x ∈ s', ad_{g'} x est nilpotent (th. 1). Donc, pour tout x ∈ s' ∩ g, ad_g x est nilpotent. Donc D(r) est contenu dans l’idéal nilpotent s' ∩ g de g.

#### Corollaire {#lie-i-s5-n5-cor-1 .statement}

Le plus grand idéal nilpotent d’une algèbre de Lie est un idéal caractéristique.

#### Remarque {#lie-i-s5-n5-rem-1 .statement}

Pour résumer certains des résultats antérieurs, notons que, si on désigne respectivement par r, n, s, f, le radical de g, le plus grand idéal nilpotent de g, le radical nilpotent de g, et l’orthogonal de g pour la forme de Killing, on a

r ⊃ f ⊃ n ⊃ s.

L’inclusion r ⊃ f résulte de la prop. 5 b). L’inclusion f ⊃ n résulte du § 4, n° 4, prop. 6 b). L’inclusion n ⊃ s a été signalée à la remarque 2 du n° 3.

### 6. Extension du corps de base

Soient g une K-algèbre de Lie, et K_1 une extension de K. Il est clair que g_{(K_1)} est résoluble si et seulement si g est résoluble, puisque $\mathcal{O}^n(g_{(K_1)}) = (\mathcal{O}^n g)_{(K_1)}$.

Soit r le radical de g. Alors, r_{(K_1)} est le radical de g_{(K_1)}. En effet, soit β la forme de Killing de g. Comme r est l’orthogonal de $\mathcal{O}g$ pour β (prop. 5 b)), r_{(K_1)} est l’orthogonal de $(\mathcal{O}g)_{(K_1)} = \mathcal{O}(g_{(K_1)})$ pour la forme déduite de β par extension de K à K_1, c’est-à-dire pour la forme de Killing de g_{(K_1)} (§ 3, n° 8). Notre assertion résulte alors d’une nouvelle application de la prop. 5 b).

## EXERCICES {#lie-i-s5-exercises}

Les conventions du § 5 restent valables, sauf mention du contraire.

See the [exercises for § 5](exercises/s5/).
