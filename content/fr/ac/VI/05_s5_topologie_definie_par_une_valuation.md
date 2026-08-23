---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: Valuations
section: 5
section_title: Topologie définie par une valuation
lang: fr
source: ac-v-vii-fr
pdf_pages: 0113-0118, 0177-0181
extraction: ocr
subsections:
    - "no": 1
      title: Topologie définie par une valuation
      page: 0
      pdf_page: 113
    - "no": 2
      title: Espaces vectoriels topologiques sur un corps muni d’une valuation
      page: 0
      pdf_page: 116
    - "no": 3
      title: Complétion d’un corps muni d’une valuation
      page: 0
      pdf_page: 117
statements: 10
exercises: 3
content_sha256: 9da475c8328abc8e702dddf5ac788695f90cfd018418adb11c27c75545d4daa4
---

## § 5. Topologie définie par une valuation.

### 1. Topologie définie par une valuation

Soient $ K $ un corps non nécessairement commutatif, $ \nu $ une valuation de $ K $, et $ G $ le groupe totalement ordonné $ \nu(K^*) $. Pour tout $ \alpha \in G $, soit $ V_\alpha $ l’ensemble des $ x \in K $ tels que $ \nu(x) > \alpha $; cet ensemble est un sous-groupe additif de $ K $ (§ 3, n° 1). Il existe une topologie $ \mathcal{T}_\nu $ et une seule sur $ K $, compatible avec la structure de groupe additif de $ K $, pour laquelle les $ V_\alpha $ forment un système fondamental de voisinages de 0 (*Top. Gén.*, chap. III, § 1, n° 2, Exemple). Pour que $ \nu $ soit impropre, il faut et il suffit que $ \mathcal{T}_\nu $ soit la topologie discrète.

#### Lemme 1 {#ac-vi-s5-lem-1 .statement}

Soient $ x \in K^*, y \in K^*, $ et $ \alpha \in G. $ Si
$$
v(x - y) > \sup(\alpha + 2v(y), v(y)),
$$
on a $ v(x^{-1} - y^{-1}) > \alpha. $
En effet on a $ x^{-1} - y^{-1} = x^{-1}(y - x)y^{-1}, $ donc
$$
v(x^{-1} - y^{-1}) = v(x - y) - v(x) - v(y).
$$
Si $ v(x - y) > v(y), $ la prop. 1 du § 3, n° 1 entraîne que $ v(x) = v(y), $ puisque $ x = y + (x - y). $ En outre, si $ v(x - y) > \alpha + 2v(y), $ on a $ v(x^{-1} - y^{-1}) > \alpha + 2v(y) - 2v(y) = \alpha. $

#### Proposition 1 {#ac-vi-s5-prop-1 .statement}

La topologie $ \mathcal{T}_v $ est séparée et compatible avec la structure de corps de $ K. $ L’application $ v : K^* \to G $ est continue si l’on munit $ G $ de la topologie discrète.
Soient $ x \in K^* $ et $ \alpha = v(x); $ on a $ x \notin V_\alpha, $ ce qui montre que $ \mathcal{T}_v $ est séparée. Quels que soient $ x_0 \in K $ et $ \alpha \in G, $ il existe $ \beta \in G $ tel que $ x_0 V_\beta \subset V_\alpha $ et $ V_\beta x_0 \subset V_\alpha $ (il suffit de prendre $ \beta \geq \alpha - v(x_0) $). D’autre part, si $ \alpha \geq 0, $ on a $ V_\alpha V_\alpha \subset V_\alpha. $ Les axiomes (AV_I) et (AV_{II}) de Top. gén., chap. III, 3e éd., § 6, n° 3, étant ainsi satisfaits, $ \mathcal{T}_v $ est compatible avec la structure d’anneau de $ K. $ Soit $ x_0 \in K^*; $ si $ x \in K^* $ vérifie $ v(x - x_0) > \sup(\alpha + 2v(x_0), v(x_0)), $ on a $ v(x^{-1} - x_0^{-1}) > \alpha $ (lemme 1), ce qui montre que $ x \to x^{-1} $ est continue, et que $ \mathcal{T}_v $ est donc compatible avec la structure de corps de $ K. $ Enfin, la seule condition $ v(x - x_0) > v(x_0) $ entraîne $ v(x) = v(x_0) $ ($ § 3, $ n° 1, prop. 1), donc l’application $ v : K^* \to G $ est continue si l’on munit $ G $ de la topologie discrète. C.Q.F.D.

Soient $ \alpha \in G, $ et $ V'_\alpha $ l’ensemble des $ x \in K $ tels que $ v(x) \geq \alpha. $ Si $ \beta < \alpha, $ on a $ V_\beta \supset V'_\alpha \supset V_\alpha. $ Si $ v $ n’est pas impropre, on voit donc que les $ V'_\alpha $ forment un système fondamental de voisinages de 0 pour $ \mathcal{T}_v. $
Les $ V_\alpha $ et les $ V'_\alpha $ sont des sous-groupes additifs ouverts, donc fermés de $ K, $ donc le corps topologique $ K $ est totalement discontinu. Comme tout idéal non nul de l’anneau de $ v $ contient un $ V_\alpha, $ il est ouvert et fermé dans $ K. $ La topologie quotient du corps résiduel de $ v $ est donc discrète.
Soit $ A $ l’anneau de $ v. $ Si $ v $ est discrète, la prop. 8 du § 3, n° 6, montre que la topologie induite par $ \mathcal{T}_v $ sur $ A $ est la topologie $ m(A)$-adique. Il n’en est pas de même en général (exerc. 4).

#### Proposition 2 {#ac-vi-s5-prop-2 .statement}

Soient $ K $ un corps non nécessairement commutatif, $ v $ une valuation non impropre de $ K, $ A l’anneau de $ \nu $, m l’idéal de $ \nu $. Pour que K, muni de la topologie $ \mathcal{T}_\nu $, soit localement compact, il faut et il suffit que les conditions suivantes soient satisfaites :

(i) K est complet;
(ii) $ \nu $ est discrète;
(iii) le corps résiduel $ \kappa(A) $ est fini.
S’il en est ainsi, A est compact.

Supposons K localement compact. Il est alors complet (Top. gén., chap. III, 3e éd., § 3, no 3, cor. 1 de la prop. 4); de plus il existe un voisinage compact de 0, qui contient un voisinage $ V'_\alpha $, où $ \alpha $ appartient au groupe des valeurs de $ \nu $; autrement dit, il existe $ a \neq 0 $ dans $ K^* $ tel que $ A.a $ soit compact, et il en résulte que $ A = (A.a)a^{-1} $ est compact. Comme tout idéal $ b \neq (0) $ de A est ouvert, $ A/b $ est compact et discret (Top. gén., chap. III, 3e éd., § 2, no 5, prop. 14), donc fini, et en particulier $ \kappa(A) = A/m $ est fini. En outre, pour $ y \neq 0 $ dans m, l’anneau $ A/Ay $ étant fini, il n’y a qu’un nombre fini d’idéaux de A contenant $ Ay $, et l’ensemble P des éléments de la forme $ \nu(x) $ tels que

$$
0 < \nu(x) \leq \nu(y)
$$

est fini; comme $ \nu(K^*) $ est totalement ordonné, P a un plus petit élément $ \gamma $. Pour tout $ x \in A $ tel que $ \nu(x) > 0 $, on a donc, soit $ \nu(x) > \nu(y) \geq \gamma $, soit $ \nu(x) \leq \nu(y) $ et alors $ \nu(x) \geq \gamma $ par définition, si bien que $ \gamma $ est le plus petit des éléments $ > 0 $ de $ \nu(K^*) $. Comme P est fini, il y a un plus grand entier $ m \geq 0 $ tel que $ m\gamma \in P $, d’où $ m\gamma \leq \nu(y) < (m+1)\gamma $. On en déduit $ 0 \leq \nu(y) - m\gamma < \gamma $, et par définition de $ \gamma $, cela entraîne $ \nu(y) = m\gamma $. On a donc $ \nu(K^*) = \mathbf{Z}.\gamma $ et la valuation $ \nu $ est discrète.

Réciproquement, supposons les conditions (i), (ii), (iii) vérifiées. On peut se borner au cas où $ \nu $ est normée; soit u une uniformisante pour $ \nu $. On a $ \kappa(A) = A/Au $, donc $ A/Au $ est fini. Comme $ x \to xu^n $ définit par passage aux quotients un isomorphisme de groupe additif de $ A/Au $ sur $ Au^n/Au^{n+1} $, $ A/Auj $ est fini pour tout $ j \geq 0 $. Comme A est fermé dans K, il est complet, donc isomorphe à la limite projective des $ A/Auj $ (Top. Gén., chap. III, 3e éd., § 7, no 3, prop. 2), et par conséquent compact. Puisque A est ouvert dans K, on voit donc que K est localement compact.

#### Remarque {#ac-vi-s5-n1-rem-1 .statement}

On notera qu’il suffit dans cette démonstration de supposer que A est complet.

### 2. Espaces vectoriels topologiques sur un corps muni d’une valuation

Soient toujours K un corps (non nécessairement commutatif), $ \nu $ une valuation de K, et G son groupe des ordres. On munit K de la topologie $ \mathcal{T}_\nu $.

#### Proposition 3 {#ac-vi-s5-prop-3 .statement}

Soit E un espace vectoriel topologique à gauche sur K, séparé et de dimension 1. On suppose $ \nu $ non impropre. Pour tout $ x_0 \neq 0 $ dans E, l’application $ a \to ax_0 $ de $ K_s $ sur E est un isomorphisme topologique.

Cette application est un isomorphisme algébrique continu. Il suffit de montrer qu’elle est bicontinue. Soit $ \alpha \in G $. Il s’agit de montrer qu’il existe un voisinage V de 0 dans E tel que la relation $ ax_0 \in V $ entraîne $ \nu(a) > \alpha $. Soit $ a_0 \in K^* $ tel que $ \nu(a_0) = \alpha $. Comme E est séparé, il existe un voisinage W de 0 dans E tel que $ a_0x_0 \notin W $. Comme $ \nu $ n’est pas impropre, il existe un voisinage $ W' $ de 0 dans E et un élément $ \beta $ de G tels que les relations $ y \in W', \ \nu(a) \geq \beta $ entraînent $ ay \in W $. Soit $ a_1 \in K^* $ tel que $ \nu(a_1) = -\beta $. Les relations $ ax_0 \in a_1^{-1}W' $ et $ \nu(a) \leq \alpha $ entraînent $ a_1ax_0 \in W' $ et $ \nu(a_0a^{-1}a_1^{-1}) = \alpha + \beta - \nu(a) \geq \beta $, donc $ a_0x_0 = a_0a^{-1}a_1^{-1}(a_1ax_0) \in W $, ce qui est absurde; autrement dit, la relation $ ax_0 \in a_1^{-1}W' $ entraîne $ \nu(a) > \alpha $.

#### Corollaire {#ac-vi-s5-n2-cor-1 .statement}

Soient E un espace vectoriel topologique à gauche sur K, H un hyperplan fermé de E, et D un sous-espace vectoriel de dimension 1 de E supplémentaire algébrique de H. On suppose $ \nu $ non impropre. Alors D est un supplémentaire topologique de H.

Compte tenu des prop. 1 et 3, la démonstration est la même que celle d’Esp. Vect. Top., chap. I, § 2, cor. 2 du th. 1.

#### Proposition 4 {#ac-vi-s5-prop-4 .statement}

On suppose $ \nu $ non impropre et K complet. Soit E un espace vectoriel topologique à gauche sur K, séparé et de dimension finie n. Pour toute base $ (e_i)_{1 \leq i \leq n} $ de E sur K, l’application $ (a_i) \to \sum_{i=1}^n a_i e_i $ de $ K_s^n $ sur E est un isomorphisme d’espaces vectoriels topologiques.

#### Corollaire {#ac-vi-s5-n2-cor-2 .statement}

On suppose $ \varphi $ non impropre et K complet. Soient E un espace vectoriel topologique séparé sur K, et F un sous-espace vectoriel de dimension finie de E. Alors F est fermé.
En effet, F est complet.

### 3. Complétion d’un corps muni d’une valuation

#### Proposition 5 {#ac-vi-s5-prop-5 .statement}

Soient K un corps non nécessairement commutatif, $ \varphi $ une valuation de K, et G le groupe $ \varphi(K^*) $ muni de la topologie discrète.

a) L’anneau complété $ \hat{K} $ de K (muni de $ \mathcal{T}_\varphi $) est un corps topologique.

b) L’application $ \varphi : K^* \to G $ se prolonge de manière unique en une application continue $ \hat{\varphi} : \hat{K}^* \to G $. L’application $ \hat{\varphi} $ (prolongée par $ \hat{\varphi}(0) = +\infty $) est une valuation de $ \hat{K} $ et $ \hat{\varphi}(\hat{K}^*) = \varphi(K^*) $.

c) La topologie de $ \hat{K} $ est la topologie définie par la valuation $ \hat{\varphi} $.

d) Pour tout $ \alpha \in G $, soient $ V_\alpha, V'_\alpha $ les sous-groupes de K définis par les conditions $ \varphi(x) > \alpha, \varphi(x) \geq \alpha $. Alors les adhérences $ \overline{V_\alpha}, \overline{V'_\alpha} $ de $ V_\alpha, V'_\alpha $ dans $ \hat{K} $ sont définies par les conditions $ \hat{\varphi}(x) > \alpha, \hat{\varphi}(x) \geq \alpha $ respectivement.

e) L’anneau de $ \hat{\varphi} $ est le complété $ \hat{A} $ de l’anneau A de $ \varphi $; l’idéal de $ \hat{\varphi} $ est le complété $ \hat{m} $ de l’idéal m de $ \varphi $.

f) On a $ \hat{A} = A + \hat{m} $; le corps résiduel de $ \hat{\varphi} $ s’identifie canoniquement à celui de $ \varphi $.

Pour prouver a), il suffit (Top. gén., chap. III, 3e éd., § 6, no 8, prop. 7) de démontrer ceci : soit $ \mathfrak{F} $ un filtre de Cauchy (pour la structure uniforme additive) sur $ K^* $ auquel 0 n’est pas adhérent; alors l’image de $ \mathfrak{F} $ par la bijection $ x \to x^{-1} $ est un filtre de Cauchy (pour la structure uniforme additive). En effet, puisque 0 n’est pas adhérent à $ \mathfrak{F} $, il existe $ M \in \mathfrak{F} $ et $ \beta \in G $ tels que $ \beta $ soit un majorant de $ \varphi(M) $. Soit $ \alpha \in G $. Si $ M' $ est un élément de $ \mathfrak{F} $ contenu dans M et tel que $ \varphi(x - y) > \sup (\alpha + 2\beta, \beta) $ pour $ x \in M' $ et $ y \in M' $, on a $ \varphi(x^{-1} - y^{-1}) > \alpha $ pour $ x \in M' $ et $ y \in M' $ (no 1, lemme 1). D’où a).

D’après la prop. 1 du no 1, $ \varphi|K^* $ est une représentation continue de $ K^* $ dans $ G $, donc se prolonge de manière unique en une représentation continue $ \hat{\nu} $ de $ \hat{K}^* $ dans $ G $. La relation
$$
\hat{\nu}(x + y) \geq \inf (\hat{\nu}(x), \hat{\nu}(y))
$$
est vraie dans $ K^* $, donc reste vraie dans $ \hat{K}^* $ par continuité. Ainsi $ \hat{\nu} $ (prolongée par $ \hat{\nu}(0) = +\infty $) est une valuation de $ \hat{K} $, et $ b) $ est démontré.

Démontrons $ d) $. Soient $ \alpha \in G $ et $ x \in \overline{V}_\alpha - \{0\} $. Pour $ y $ dans $ V_\alpha $ assez voisin de $ x $, on a $ \hat{\nu}(x) = \hat{\nu}(y) = \nu(y) $, donc $ \hat{\nu}(x) > \alpha $. Réciproquement, soit $ x \in \hat{K}^* $ tel que $ \hat{\nu}(x) > \alpha $; pour $ y $ dans $ K^* $ assez voisin de $ x $, on a $ \nu(y) = \hat{\nu}(y) = \hat{\nu}(x) $, donc $ y \in V_\alpha $, d’où $ x \in \overline{V}_\alpha $. Ainsi $ \overline{V}_\alpha $ est l’ensemble des $ x \in \hat{K} $ tels que $ \hat{\nu}(x) > \alpha $. On raisonne de façon analogue pour $ V'_\alpha $. Ceci prouve $ d) $.

Compte tenu de la prop. 7 de Top. gén., chap. III, 3e éd., § 3, no 4, l’assertion $ c) $ est une conséquence de $ d) $. L’assertion $ e) $ est un cas particulier de $ d) $. Enfin, soit $ x \in \hat{A} $; il existe $ y \in A $ tel que $ \hat{\nu}(x - y) > 0 $; alors $ z = x - y \in \hat{m} $, donc $ x = y + z \in A + \hat{m} $; ainsi $ \hat{A} = A + \hat{m} $, ce qui démontre $ f) $.

#### Remarque {#ac-vi-s5-n3-rem-1 .statement}

Pour tout $ x \in \hat{K} $ n’appartenant pas à $ \hat{A} $, il existe $ x_0 \in K $ tel que $ \hat{\nu}(x - x_0) > 0 $, $ \hat{\nu}(x) = \hat{\nu}(x_0) = \nu(x_0) < 0 $; on a donc $ x_0^{-1} x \in \hat{A} $, et comme $ x_0^{-1} \in A $, on voit que si l’on pose $ S = A - \{0\} $, on peut écrire $ \hat{K} = S^{-1} \hat{A} $.

## EXERCICES {#ac-vi-s5-exercises}

**Q 1)** Soient $ A $ un anneau intègre, $ K $ son corps des fractions, $ \mathcal{T} $ une topologie linéaire sur $ A $ (chap. III, § 2, exerc. 21).

$ a) $ Pour que les voisinages de $ 0 $ pour $ \mathcal{T} $ constituent un système fondamental de voisinages de $ 0 $ pour une topologie $ \mathcal{T}_K $ compatible avec la structure d’anneau de $ K $, il faut et il suffit que $ \mathcal{T} $ soit la topologie $ \mathcal{T}_u(A) $ (chap. III, § 2, exerc. 24); alors $ A $ est une partie bornée pour $ \mathcal{T}_K $ et $ \mathcal{T}_K $ est une topologie séparée localement bornée ($ Top. gén. $, chap. III, 3e éd., § 6, exerc. 12 et 20 e)). Pour que $ K $ soit complet (resp. linéairement compact, resp. strictement linéairement compact (chap. III, § 2, exerc. 21)) pour $ \mathcal{T}_K $, il faut et il suffit que $ A $ le soit pour $ \mathcal{T} $.

$ b) $ Pour que la topologie $ \mathcal{T}_K $ (où $ \mathcal{T} = \mathcal{T}_u(A) $) soit compatible avec la structure de corps de $ K $, il faut et il suffit que le radical $ \mathfrak{R}(A) $ de $ A $ soit $ \neq 0 $.

**Q 2)** Soient $ K $ un corps (commutatif), $ \mathcal{T} $ une topologie séparée non discrète sur $ K $, compatible avec la structure d’anneau de $ K $. Pour que la topologie $ \mathcal{T} $ soit définie par une valuation de $ K $ ou une valeur absolue sur $ K $, il faut et il suffit que $ \mathcal{T} $ soit localement rétrobornée ($ Top. gén. $, chap. III, 3e éd., § 6, exerc. 22. S’il existe dans $ K $ des éléments topologiquement nilpotents, utiliser l’exerc. 22 d) de $ Top. gén. $, chap. III, 3e éd., § 6 et l’exerc. 13 de $ Top. gén. $, chap. IX, 2e éd., § 3. Dans le cas contraire, utiliser l’exerc. 22 f) de $ Top. gén. $, chap. III, 3e éd., § 6).

**Q 3)** Soient $ A $ un anneau noethérien intègre, $ K $ son corps des fractions, $ \mathcal{T}_u $ la topologie $ \mathcal{T}_u(A) $ sur $ A $, $ \mathcal{T}_K $ la topologie correspondante sur $ K $ (exerc.

See the [exercises for § 5](exercises/s5/).
