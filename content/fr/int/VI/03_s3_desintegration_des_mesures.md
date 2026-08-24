---
book: int
book_title: Integration
chapter: VI
chapter_title: Intégration vectorielle
section: 3
section_title: Désintégration des mesures
lang: fr
source: int-vi-fr
pdf_pages: 0057-0072, 0097-0099
extraction: ocr
subsections:
    - "no": 1
      title: Désintégration d'une mesure $ \mu $ relativement à une application $ \mu $-propre.
      page: 0
      pdf_page: 57
    - "no": 2
      title: Mesures pseudo-images.
      page: 0
      pdf_page: 63
    - "no": 3
      title: Désintégration d'une mesure $ \mu $ relative à une pseudo-image de $ \mu $.
      page: 0
      pdf_page: 64
    - "no": 4
      title: '*Relations d’équivalence mesurables*.'
      page: 0
      pdf_page: 66
    - "no": 5
      title: Désintégration d’une mesure par une relation d’équivalence mesurable.
      page: 0
      pdf_page: 70
statements: 17
exercises: 12
content_sha256: a18f7b8708e017adbdafd3c8abee8bb47acd6388206d22180e7b7044573f4abd
---

## § 3. Désintégration des mesures

### 1. Désintégration d'une mesure $ \mu $ relativement à une application $ \mu $-propre.

Soit T un espace localement compact ayant une base dénombrable (en d'autres termes un espace localement compact polonais (Top. gén., chap. IX, 2e éd., § 6, no 1)). On sait que pour toute mesure positive sur T, les notions d'intégrale et d'intégrale essentielle coïncident (chap. V, § 2, no 2, Remarque 1). D'autre part, on a les propriétés suivantes :

#### Lemme 1 {#int-vi-s3-lem-1 .statement}

Si Y est un espace localement compact ayant une base dénombrable, l'espace $ \mathcal{K}(Y) $ contient une partie dénombrable partout dense. Plus précisément, il existe dans $ \mathcal{K}(Y) $ une partie dénombrable S formée de fonctions $ \geq 0 $, telle que, pour toute fonction $ f \geq 0 $ de $ \mathcal{K}(Y) $, il existe une suite de fonctions $ f_n \in S $ ($ n \geqslant 0 $) qui converge uniformément vers $ f $ et est telle que $ f_n \leq f_0 $ pour tout $ n \geqslant 0 $.

En effet, Y est réunion d'une suite croissante $ (U_n) $ d'ensembles ouverts relativement compacts tels que $ \overline{U}_n \subset U_{n+1} $ pour tout $ n $ (Top. gén., chap. I, 2e éd., § 10, no 11, prop. 19); l'espace $ \mathcal{K}(Y) $ est réunion de la suite croissante des espaces de Banach $ \mathcal{K}(Y, \overline{U}_n) $, et on sait que chacun de ces derniers est de type dénombrable (Top. gén., chap. X, 2e éd., § 3, no 4, th. 1). Soient $ S'_n $ un ensemble dénombrable dense dans $ \mathcal{K}(Y, \overline{U}_n) $, $ S_n $ l'ensemble des fonctions $ \varphi^+ $ pour $ \varphi \in S'_n $, $ u_n $ une fonction de $ \mathcal{K}(Y, \overline{U}_{n+1}) $, à valeurs dans $ \{0,1\} $ et égale à 1 dans $ U_n $. Nous prendrons pour S la réunion des $ S_n $ et de l'ensemble des $ m u_n $ pour $ m $ et $ n $ entiers $ \geqslant 0 $. Pour toute fonction $ f \geqslant 0 $ de $ \mathcal{K}(Y) $, $ f $ a son support dans l'un des $ U_n $, donc est limite uniforme d'une suite de fonctions $ f_p \in S_n $ ($ p \geqslant 1 $). Ces fonctions $ f_p $ sont uniformément majorées par un entier positif $ m $, et il suffit de prendre $ f_0 = m u_n $.

#### Lemme 2 {#int-vi-s3-lem-2 .statement}

Si Y est un espace localement compact ayant une base dénombrable, l'espace de Banach $ \overline{\mathcal{K}(Y)} $ des fonctions numériques continues tendant vers 0 au point à l'infini est de type dénombrable.

Ce lemme n'est autre que le cor. du th. 1 de Top. gén., chap. X, 2e éd., § 3, no 4. On peut observer qu'il résulte aussi du lemme 1 et du fait que la topologie de la convergence uniforme sur $ \mathcal{K}(Y) $ est moins fine que la topologie limite inductive des topologies des sous-espaces $ \mathcal{K}(Y, \overline{U}_n) $.

#### Lemme 3 {#int-vi-s3-lem-3 .statement}

Soient T et X deux espaces localement compacts à bases dénombrables, $ \mu $ une mesure positive sur T, $ t \to \lambda_t $ une famille de mesures positives sur X. Si l'application $ t \to \lambda_t $ est scalairement $ \mu $-intégrable (pour la topologie $ \sigma(\mathcal{M}(X), \mathcal{K}(X)) $), alors la famille $ t \to \lambda_t $ est $ \mu $-adéquate (chap. V, § 3, no 1, déf. 1).

En effet, le lemme 1, appliqué à $ \mathcal{K}(X) $, montre que l'application $ t \to \lambda_t $ est vaguement $ \mu $-mesurable (§ 1, no 5, prop. 13).

#### Théorème 1 {#int-vi-s3-thm-1 .statement}

Soient T et B deux espaces localement compacts ayant des bases dénombrables, $ \mu $ une mesure positive sur T, $ p $ une application $ \mu $-propre (chap. V, § 6, no 1, déf. 1) de T dans B, et $ \nu = p(\mu) $ l’image de $ \mu $ par $ p $. Il existe alors une famille $ \nu $-adéquate (chap. V, § 3, no 1, déf. 1) $ b \to \lambda_b $ ($ b \in B $) de mesures positives sur T, ayant les propriétés suivantes :

a) $ \| \lambda_b \| = 1 $ pour tout $ b \in p(T) $ ;
b) $ \lambda_b $ est concentrée sur l’ensemble $ p^{-1}(b) $ (chap. V, § 5, no 7, déf. 4) pour tout $ b \in B $; en particulier, $ \lambda_b = 0 $ pour $ b \notin p(T) $ ;
c) on a $ \mu = \int \lambda_b d\nu(b) $.

En outre, si $ b \to \lambda'_b $ ($ b \in B $) est une seconde famille $ \nu $-adéquate de mesures positives sur T ayant les propriétés b) et c), on a $ \lambda'_b = \lambda_b $ presque partout dans B pour la mesure $ \nu $.

1) Unicité. Pour toute fonction $ f \in \mathcal{K}(B) $, $ f \circ p $ est $ \mu $-intégrable puisque $ p $ est $ \mu $-propre (chap. V, § 6, no 2, th. 1); pour toute fonction $ g \in \mathcal{K}(T) $, la fonction $ t \to g(t)f(p(t)) $ est donc $ \mu $-intégrable. Il en résulte (chap. V, § 3, no 4, th. 1) que, pour presque tout $ b \in B $, la fonction $ t \to g(t)f(p(t)) $ est $ \lambda_b $-intégrable et que l’on a

$$
\int g(t)f(p(t))d\mu(t) = \int d\nu(b) \int g(t)f(p(t))d\lambda_b(t).
$$

Mais puisque $ \lambda_b $ est concentrée sur $ p^{-1}(b) $, on a, pour tout $ b \in B $, $ f(p(t)) = f(b) $ presque partout pour $ \lambda_b $, donc le second membre de (1) est égal à $ \int f(b)\langle g, \lambda_b \rangle d\nu(b) $. On a une formule analogue pour $ \lambda'_b $; par suite $ \int f(b)\langle g, \lambda_b \rangle d\nu(b) = \int f(b)\langle g, \lambda'_b \rangle d\nu(b) $ pour toute $ f \in \mathcal{K}(B) $ et toute $ g \in \mathcal{K}(T) $. Autrement dit, les deux applications $ b \to \lambda_b $ et $ b \to \lambda'_b $ de B dans $ \mathcal{M}(T) $ sont égales scalairement localement presque partout pour $ \nu $, donc égales presque partout pour $ \nu $ (lemme 1 et § 1, no 1, Remarque 2).

2. Définition provisoire de la famille $ b \to \lambda_b $. Pour toute fonction $ f \in \mathcal{L}^1(\nu) $, $ f \circ p $ est $ \mu $-intégrable (chap. V, § 6, no 2, th. 1), donc $ (f \circ p)_\mu $ est une mesure bornée sur T et l’on a

$$
\|(f \circ p)_\mu\| = \int |f \circ p|\, d\mu = \int |f|\, d\nu = N_1(f)
$$

(chap. IV, § 4, n° 7, prop. 12 ; chap. V, § 5, n° 3, th. 1 et § 6, n° 2, th. 1). Il en résulte que $(f \circ p) . \mu$ ne dépend que de la classe $\tilde{f}$ de $f$ dans $L^1(\nu)$ et que $\tilde{f} \to (f \circ p) . \mu$ est une application linéaire *isométrique* de $L^1(\nu)$ dans l’espace de Banach $\mathcal{M}^1(T)$ des mesures bornées sur $T$, dual fort de l’espace de Banach $\overline{\mathcal{K}(T)}$, qui est de type dénombrable (lemme 2). D’après le th. de Dunford-Pettis ($§ 2$, n° 5, cor. 2 du th. 1) il existe une application $b \to \lambda_b$ de $B$ dans la boule unité de $\mathcal{M}^1(T)$, scalairement $\nu$-mesurable (pour la topologie $\sigma(\mathcal{M}^1(T), \overline{\mathcal{K}(T)})$ et telle que, pour toute fonction $f \in L^1(\nu)$, on ait

$$
(f \circ p) . \mu = \int f(b) \lambda_b d\nu(b)
$$

ce qui s’écrit encore, pour toute fonction $g \in \overline{\mathcal{K}(T)}$

$$
\int g(t) f(p(t)) d\mu(t) = \int f(b) d\nu(b) \int g(t) d\lambda_b(t).
$$

Si $f \geqslant 0$ et $g \geqslant 0$, le premier membre de (3) est $\geqslant 0$, ce qui prouve que pour toute fonction $g \geqslant 0$ de $\mathcal{K}(T)$, la mesure $\left( \int g(t) d\lambda_b(t) \right)_\nu$ est $\geqslant 0$, donc que $\int g(t) d\lambda_b(t) \geqslant 0$ sauf lorsque $b$ appartient à un ensemble $\nu$-négligeable $N(g)$ (chap. V, § 5, n° 4, cor. 3 de la prop. 4). Or, il existe une suite partout dense $(g_n)$ dans l’espace $\mathcal{K}_+(T)$ des fonctions $\geqslant 0$ de $\mathcal{K}(T)$ (lemme 1). La réunion $N$ des $N(g_n)$ est $\nu$-négligeable et pour $b \notin N$ on a $\int g_n(t) d\lambda_b(t) \geqslant 0$ pour tout $n$, donc $\int g(t) d\lambda_b(t) \geqslant 0$ pour toute fonction $g \in \mathcal{K}_+(T)$, autrement dit $\lambda_b \geqslant 0$.

Cela étant, on peut remplacer $\lambda_b$ par 0 pour tout $b \in N$ sans modifier la validité de (3) ; nous pouvons donc supposer cette modification faite, autrement dit que l’on a $\lambda_b \geqslant 0$ pour tout $b \in B$.

3) *Extensions de la formule (3)*.

$a)$ Pour toute fonction $f \in L^1(\nu)$, il résulte de (3) que l’application $b \to \lambda_b$ de $B$ dans $\mathcal{M}(T)$ est scalairement intégrable pour la mesure $|f . \nu|$ et pour la topologie $\sigma(\mathcal{M}(T), \mathcal{K}(T))$, donc (lemme 3) la famille $b \to \lambda_b$ est $|f . \nu|$-*adéquate*. Soit alors $g$ une fonction numérique définie dans T, intégrable pour la mesure $ |(f \circ p) \cdot \mu| $, c'est-à-dire (chap. V, § 5, no 3, th. 1) telle que $ t \to g(t)f(p(t)) $ soit $ \mu $-intégrable ; il résulte alors de (2), du th. 1 du chap. V, § 3, no 4 et du th. 1 du chap. V, § 5, no 3 que, pour presque tout $ b \in B $, $ g $ est intégrable pour $ \lambda_b $, que la fonction (définie presque partout)
$$
b \to \int g(t)d\lambda_b(t)
$$
est intégrable pour $ |f \cdot \nu| $ et que la formule (3) est encore valable.

$ \beta) $ Pour toute fonction $ g \in \mathcal{J}_i(T) $, il résulte de (3), appliquée à $ f \in \mathcal{J}_i(B) $, que l’application $ p $ est propre pour la mesure $ |g \cdot \mu| $ (chap. V, § 6, no 1, déf. 1) et que l’image par $ p $ de la mesure $ g \cdot \mu $ est la mesure de densité $ b \to \int g(t)d\lambda_b(t) $ par rapport à $ \nu $. Si alors on prend pour $ f $ une fonction telle que $ f \circ p $ soit intégrable pour la mesure $ |g \cdot \mu| $, c’est-à-dire telle que $ t \to g(t)f(p(t)) $ soit $ \mu $-intégrable (chap. V, § 5, no 3, th. 1), la formule (3) est encore valable (chap. V, § 6, no 2, th. 1).

4) *Propriétés de la famille* $ b \to \lambda_b $. D’après la propriété $ \beta) $, on peut appliquer la formule (3) en prenant $ f = 1 $, $ g \in \mathcal{J}_i(T) $; cela prouve que $ b \to \lambda_b $ est scalairement $ \nu $-intégrable (pour la topologie $ \sigma(\mathcal{M}(T), \mathcal{J}_i(T)) $), donc $ \nu $-*adéquate* (lemme 3) et que l’on a
$$
\mu = \int \lambda_b d\nu(b).
$$

Soit maintenant $ \psi $ une fonction quelconque de $ \mathcal{K}(B) $; les conditions de la propriété $ \alpha) $ sont remplies en prenant $ f \in \mathcal{K}(B) $ et $ g = \psi \circ p $, car la fonction $ \psi(p(t))f(p(t)) $ est $ \mu $-intégrable puisque $ f \psi $ appartient à $ \mathcal{J}_i(B) $ et que $ p $ est $ \mu $-propre. Alors, $ \psi \circ p $ est $ \lambda_b $-intégrable pour presque tout $ b \in B $ et on a
$$
\int f(p(t))\psi(p(t))d\mu(t) = \int f(b)d\nu(b) \int \psi(p(t))d\lambda_b(t);
$$
mais le premier membre est par définition $ \int f(b)\psi(b)d\nu(b) $. On voit donc que, pour toute fonction $ \psi \in \mathcal{K}(B) $, la mesure $ \psi \cdot \nu $ et la mesure de densité $ b \to \int \psi(p(t))d\lambda_b(t) $ sont identiques. Par suite (chap. V, § 5, n° 4, cor. de la prop. 4), il existe un ensemble ν-négligeable N'(ψ) tel que, pour tout b ∈ N'(ψ), la fonction ψ ∘ p soit λ_b-intégrable et que ψ(b) = $ \int \psi(p(t)) d\lambda_b(t) $.

Soit S un ensemble dénombrable de $ \mathcal{K}(B) $ possédant les propriétés énoncées au lemme 1 (avec Y = B), et soit N' l'ensemble ν-négligeable réunion des N'(ψ) pour ψ ∈ S. Toute fonction ψ ≥ 0 de $ \mathcal{K}(B) $ est limite uniforme d'une suite ($ \psi_n $) d'éléments de S avec $ \psi_n \leq \psi_0 $. Par suite, pour b ∈ N', le th. de Lebesgue montre que, d'une part ψ ∘ p est λ_b-intégrable, autrement dit que p est λ_b-propre, et d'autre part que ψ(b) = $ \int \psi(p(t)) d\lambda_b(t) $. En d'autres termes, les applications $ b \to \varepsilon_b $ et $ b \to p(\lambda_b) $ de B dans $ \mathcal{M}(B) $ (cette dernière définie presque partout) sont scalairement presque partout égales pour ν (et pour la topologie $ \sigma(\mathcal{M}(B), \mathcal{K}(B)) $) ; on en conclut que ces applications sont égales presque partout pour ν (lemme 1 et § 1, n° 1, Remarque 2). Enfin, si $ p(\lambda_b) = \varepsilon_b $, l'ensemble B − {b} est $ \varepsilon_b $-négligeable, donc l'ensemble T − $ p^{-1}(b) $ est $ \lambda_b $-négligeable (chap. V, § 6, n° 2, cor. de la prop. 2), autrement dit $ \lambda_b $ est concentrée sur $ p^{-1}(b) $; et d'autre part on a $ \| \lambda_b \| = \int d\lambda_b = \int d(p(\lambda_b)) = \| \varepsilon_b \| = 1 $ (chap. V, § 6, n° 2, th. 1).

5) Modifications finales de la famille $ b \to \lambda_b $. Nous avons donc défini une famille ν-adéquate $ b \to \lambda_b $ de mesures ≥ 0 sur T, vérifiant la condition c) de l'énoncé et telle que, pour presque tout b ∈ B, p soit λ_b-propre, $ \lambda_b $ soit concentrée sur $ p^{-1}(b) $ et de norme 1. Soit N'' l'ensemble ν-négligeable des points b ∈ B où l'une des trois dernières propriétés n'est pas vérifiée ; on peut alors modifier $ \lambda_b $ de la façon suivante. Si $ b \in B - p(T) $, on prend $ \lambda_b = 0 $; si $ b \in p(T) \cap N'' $, on prend $ \lambda_b = \varepsilon_{\xi(b)} $, où $ \xi(b) $ est un point quelconque de $ p^{-1}(b) $. Comme B − p(T) est ν-négligeable (chap. V, § 6, n° 2, cor. 3 de la prop. 2), on n'a modifié $ \lambda_b $ qu'aux points d'un ensemble négligeable et par suite la famille $ b \to \lambda_b $ est encore ν-adéquate et vérifie la propriété c) ; en outre, elle vérifie maintenant a) et b), ce qui termine la démonstration.

On dit que toute famille ν-adéquate $ b \to \lambda_b $ de mesures positives sur T, ayant les propriétés b) et c) du th. 1, est une désintégration de la mesure $ \mu $, relative à l’application $ \mu $-propre $ p $.

### 2. Mesures pseudo-images.

#### Définition 1 {#int-vi-s3-def-1 .statement}

Soient T et B deux espaces localement compacts, $ \mu $ une mesure positive sur T, $ p $ une application $ \mu $-mesurable de T dans B. On dit qu’une mesure positive $ \nu $ sur B est une mesure pseudo-image de $ \mu $ par $ p $ si elle vérifie la condition suivante : pour qu’une partie N de B soit localement $ \nu $-négligeable, il faut et il suffit que $ p^{-1}(N) $ soit localement $ \mu $-négligeable.

#### Exemple 1 {#int-vi-s3-n2-exa-1 .statement}

Si $ p $ est $ \mu $-propre et si $ \nu = p(\mu) $, $ \nu $ est pseudo-image de $ \mu $ par $ p $ (chap. V, § 6, no 2, cor. 2 de la prop. 2).

#### Exemple 2 {#int-vi-s3-n2-exa-2 .statement}

Soient B’ un espace localement compact, $ \nu’ $ une mesure positive sur B’ ; prenons pour T l’espace $ B \times B’ $ et pour $ \mu $ la mesure $ \nu \otimes \nu’ $ ; si $ p $ est la projection de T sur B, $ \nu $ est pseudo-image de $ \mu $ par $ p $ (chap. V, § 8, no 2, cor. 8 de la prop. 5 et no 1 , cor. de la prop. 2).

On notera que si $ \nu $ est une mesure pseudo-image de $ \mu $ par $ p $, $ \nu $ est portée par $ p(T) $.

Si $ \nu $ est pseudo-image de $ \mu $ par $ p $, l’ensemble des mesures pseudo-images de $ \mu $ par $ p $ est la classe des mesures positives équivalentes à $ \nu $, et toute mesure positive équivalente à $ \mu $ admet les mêmes mesures pseudo-images par $ p $. On dit que la classe de $ \nu $ est la classe pseudo-image de celle de $ \mu $ par $ p $.

#### Proposition 1 {#int-vi-s3-prop-1 .statement}

Soient T un espace localement compact dénombrable à l’infini, $ \mu $ une mesure positive sur T, $ p $ une application $ \mu $-mesurable de T dans un espace localement compact B. Il existe alors une mesure pseudo-image de $ \mu $ par $ p $.

En effet, il existe sur T une mesure bornée $ \mu’ $ équivalente à $ \mu $ (chap. V, § 6, no 5, prop. 11) ; $ p $ est alors $ \mu’ $-propre.

### 3. Désintégration d'une mesure $ \mu $ relative à une pseudo-image de $ \mu $.

#### Théorème 2 {#int-vi-s3-thm-2 .statement}

Soient $ T $ et $ B $ deux espaces localement compacts ayant des bases dénombrables, $ \mu $ une mesure positive sur $ T $, $ p $ une application $ \mu $-mesurable de $ T $ dans $ B $, $ \nu $ une mesure pseudo-image de $ \mu $ par $ p $. Il existe alors une famille $ \nu $-adéquate $ b \to \lambda_b $ ($ b \in B $) de mesures positives sur $ T $, ayant les propriétés suivantes :

a) $ \lambda_b \neq 0 $ pour $ b \in p(T) $ ;
b) $ \lambda_b $ est concentrée sur l'ensemble $ p^{-1}(b) $ pour tout $ b \in B $; en particulier $ \lambda_b = 0 $ pour $ b \notin p(T) $ ;
c) on a $ \mu = \int \lambda_b d\nu(b) $.

En outre, si $ \nu' = r.\nu $ est une seconde mesure pseudo-image de $ \mu $ par $ p $, et si $ b \to \lambda'_b $ est une famille $ \nu' $-adéquate de mesures positives sur $ T $, ayant les propriétés b) et c) par rapport à $ \nu' $, on a, presque partout dans $ B $ (pour $ \nu $ ou $ \nu' $), $ \lambda_b = r(b)\lambda'_b $.

En effet, il existe une fonction numérique continue et finie $ f $ définie dans $ T $, telle que $ f(t) > 0 $ pour tout $ t \in T $ et que $ \mu'' = f.\mu $ soit bornée (chap. V, § 5, no 6, prop. 11). Soit $ \nu'' = p(\mu'') $, qui est équivalente à $ \nu $, et posons $ \nu'' = g.\nu $, $ g $ étant finie et localement $ \nu $-intégrable ; on peut en outre supposer $ g(b) > 0 $ pour tout $ b \in B $ (chap. V, § 5, no 6, prop. 10). Le th. 1 du no 1, appliqué à $ \mu'' $ et $ \nu'' $, montre qu'il existe une famille $ \nu'' $-adéquate $ b \to \lambda''_b $ ($ b \in B $) de mesures positives sur $ T $, telles que : 1) $ \| \lambda''_b \| = 1 $ pour $ b \in p(T) $ ; 2) $ \lambda''_b $ est concentrée sur $ p^{-1}(b) $ pour tout $ b \in B $ ; 3) $ \mu'' = \int \lambda''_b d\nu''(b) $.

Pour tout $ b \in B $, définissons une mesure positive $ \lambda_b $ sur $ T $ par la formule $ \lambda_b = (1/f).(g(b)\lambda'_b) $. Il est clair que la famille $ b \to \lambda_b $ possède les propriétés a) et b) de l'énoncé. D'autre part, pour toute fonction $ h \in \mathcal{K}(T) $, $ h/f $ appartient à $ \mathcal{K}(T) $, donc on a

$$
\int h(t)d\mu(t) = \int (h(t)/f(t))d\mu''(t) = \int d\nu''(b) \int (h(t)/f(t))d\lambda''_b(t).
$$

Mais comme la fonction $ b \to \int (h(t)/f(t))d\lambda''_b(t) $ est $ \nu'' $-intégrable, la fonction $ b \to g(b) \int (h(t)/f(t))d\lambda''_b(t) $ est $ \nu $-intégrable (chap. V, § 5, n° 3, th. 1). Par définition de $ \lambda_b $, cette fonction est $ b \to \int h(t)d\lambda_b(t) $, d’où $ \int h(t)d\mu(t) = \int dv(b) \int h(t)d\lambda_b(t) $ (loc. cit.) ce qui prouve que $ \mu = \int \lambda_b dv(b) $.

Pour établir la seconde partie de l’énoncé, remarquons qu’on peut supposer $ r(b) > 0 $ pour tout $ b \in B $ (chap. V, § 5, n° 6, prop. 10); posons $ \lambda_b''' = f . ((r(b)/g(b))\lambda_b') $; comme ci-dessus, on montre que, pour toute fonction $ h \in \mathcal{K}(T) $, la relation

$$
\int h(t)d\mu(t) = \int dv'(b) \int h(t)d\lambda_b'(t)
$$

entraîne

$$
\int h(t)d\mu(t) = \int dv'(b) \int (h(t)/f(t))d\lambda_b'''(t).
$$

Le th. 1 du n° 1, appliqué à $ \mu'' $ et $ v'' $, entraîne donc, pour presque tout $ b \in B $, $ \lambda_b''' = \lambda_b'' $, d’où $ \lambda_b = r(b)\lambda_b' $.

#### Définition 2 {#int-vi-s3-def-2 .statement}

Soient T et B deux espaces localement compacts polonais. Etant données une mesure positive $ \mu $ sur T, une application $ \mu $-mesurable $ p $ de T dans B, une mesure pseudo-image $ \nu $ de $ \mu $ par $ p $, toute famille $ \nu $-adéquate $ b \to \lambda_b $ ($ b \in B $) de mesures positives sur T possédant les propriétés b) et c) du th. 2 est appelée une désintégration de $ \mu $ relative à $ \nu $.

Lorsque $ p $ est $ \mu $-propre et que $ \nu = p(\mu) $, la notion de désintégration relative à $ p $ coïncide donc avec la notion de désintégration relative à $ \nu $. Sous les hypothèses du th. 2, deux désintégrations de $ \mu $ relatives à la même mesure pseudo-image $ \nu $ sont égales presque partout pour $ \nu $.

#### Remarque {#int-vi-s3-n3-rem-1 .statement}

Le th. 1 du chap. V, § 3, n° 4, montre (compte tenu de ce que T et B ont des bases dénombrables) que pour toute fonction $ f $ définie dans T, à valeurs dans $ \overline{\mathbf{R}} $ ou dans un espace de Banach F et $ \mu $-intégrable, l’ensemble des $ b \in B $ tels que $ f $ ne soit pas $ \lambda_b $-intégrable est $ \nu $-négligeable, la fonction $ b \to \int f(t) d\lambda_b(t) $, définie presque partout, est $ \nu $-intégrable, et l’on a

$$
\int f(t) d\mu(t) = \int d\nu(b) \int f(t) d\lambda_b(t).
$$

On a un résultat analogue pour les fonctions scalairement $ \mu $-intégrables en appliquant la prop. 3 du § 1, no 1.

### 4. *Relations d’équivalence mesurables*.

Étant donné un espace topologique $ X $ et une relation d’équivalence $ R $ dans $ X $, nous dirons que $ R $ est séparée si l’espace quotient $ X/R $ est séparé.

Rappelons (*Top. gén.*, chap. I, 2e éd., § 9, no 9, th. 2) que si $ R $ est une relation d’équivalence *ouverte*, il revient au même de dire que le graphe de $ R $ dans $ X \times X $ est fermé.

Soit $ p $ une application de $ X $ dans un espace topologique séparé $ B $, et soit $ R $ la relation d’équivalence $ p(x) = p(y) $ dans $ X $; si $ K $ est une partie *compacte* de $ X $ telle que la restriction de $ p $ à $ K $ soit *continue*, la relation $ R_K $ induite par $ R $ sur $ K $ est séparée, car l’espace quotient $ K/R_K $ est homéomorphe à l’espace $ p(K) $, qui est compact (*Top. gén.*, chap. I, 2e éd., § 10, no 6, cor. 1 de la prop. 8). Si $ T $ est un espace localement compact, $ \mu $ une mesure positive sur $ T $, $ p $ une application $ \mu $-mesurable de $ T $ dans un espace topologique séparé $ B $, on voit donc que l’ensemble des parties compactes $ K $ de $ T $ telles que la relation $ R_K $ soit séparée, est $ \mu $-dense (chap. V, § 1, no 2.) On est donc conduit à poser la définition suivante :

#### Définition 3 {#int-vi-s3-def-3 .statement}

*Soient T un espace localement compact, $ \mu $ une mesure positive sur T. On dit qu’une relation d’équivalence R dans T est $ \mu $-mesurable si l’ensemble des parties compactes K de T, telles que $ R_K $ soit séparée, est $ \mu $-dense.*

Si $ R $ est séparée, $ R $ est $ \mu $-mesurable, car si $ \varphi $ est l’application canonique de $ T $ sur l’espace topologique séparé $ T/R $, $ \varphi $ est continue et $ R $ est équivalente à $ \varphi(x) = \varphi(y) $. De même, si $ R $ est telle que le saturé pour R de toute partie compacte de T soit fermé (et en particulier si R est une relation d'équivalence fermée), R est $ \mu $-mesurable, car pour toute partie compacte K de T, la relation $ R_K $ est fermée, donc séparée (*Top. gén.*, chap. I, 2e éd., § 10, no 6, prop. 8).

On notera que, si R est $ \mu $-mesurable, R est aussi mesurable pour toute mesure de base $ \mu $ sur T.

#### Proposition 2 {#int-vi-s3-prop-2 .statement}

*Soient T un espace localement compact dénombrable à l'infini, $ \mu $ une mesure positive sur T.*

1) *Pour toute relation d'équivalence $ \mu $-mesurable R sur T, il existe un espace localement compact B et une application $ \mu $-mesurable p de T dans B telle que R soit équivalente à la relation $ p(x) = p(y) $.*

2) *Si en outre T admet une base dénombrable, on peut supposer que B admet une base dénombrable.*

Comme T est dénombrable à l'infini, il existe une suite croissante $(K_n)_{n \geq 1}$ de parties compactes de T telles que T soit réunion des $K_n$ et d'un ensemble $ \mu $-négligeable N, et que chacune des relations $R_{K_n}$ soit séparée. Soit $B_n$ l'espace quotient $K_n / R_{K_n}$, qui est compact, et soit $B'_n$ l'espace compact somme topologique de $B_n$ et d'un point $a_n$. Soit $q_n$ l'application canonique de $K_n$ sur $B_n$; on prolonge $q_n$ en une application $p_n$ de T dans $B'_n$ de la façon suivante : si $x \in T$ est congru mod. R à un élément $y \in K_n$, on pose $p_n(x) = q_n(y)$; dans le cas contraire, on pose $p_n(x) = a_n$. Soit $B'$ l'espace produit $\prod_{n=1}^\infty B'_n$, qui est compact, et soit $p'$ l'application $x \to (p_n(x))$ de T dans $B'$. Montrons que $p'$ est $ \mu $-*mesurable* : il suffit (chap. IV, § 5, no 3, th. 1) de prouver que chacune des applications $p_n$ est mesurable, et pour cela il suffit que la restriction de $p_n$ à chaque $K_m$ soit mesurable. Or cela est évident si $m \leq n$; si au contraire $m > n$, soit $K_{nm}$ le saturé de $K_n$ pour $R_{K_m}$, qui est une partie compacte de $K_m$ (*Top. gén.*, chap. I, 2e éd., § 10, no 4, th. 2); comme $p_n$ est constant dans $K_m - K_{nm}$, il suffit de prouver que la restriction de $p_n$ à $K_{nm}$ est continue, ce qui est évident à cause de l'isomorphisme canonique entre $K_{nm}/R_{K_{nm}}$ et $K_n/R_{K_n}$ (*Top. gén.*, chap. I, § 10, no 6, cor. 2 de la prop. 8).

Soit A le saturé de $\bigcup_n K_n$ pour la relation R, et soit

N' = T - A ⊂ N. Nous allons voir que la relation $ p'(x) = p'(y) $ est équivalente à la relation « R $ \{ x, y \} $ ou $ (x, y) \in N' \times N' $ ». En effet, si on a R $ \{ x, y \} $, on a $ p_n(x) = p_n(y) $ quel que soit $ n $, donc $ p'(x) = p'(y) $; et si $ x \in N' $, $ y \in N' $, on a $ p_n(x) = p_n(y) = a_n $ quel que soit $ n $, donc $ p'(x) = p'(y) $. Si d'autre part $ x $ et $ y $ sont dans A et ne sont pas congrus mod. R, il existe un entier $ n $, un élément $ x' \in K_n $ (resp. $ y' \in K_n $) congru mod. R à $ x $ (resp. $ y $) tels que $ x' $ ne soit pas congru à $ y' $ mod. $ R_{K_n} $; on a donc $ p_n(x) \neq p_n(y) $ et par suite $ p'(x) \neq p'(y) $. Enfin, si $ x \in N' $ et $ y \in A $, on a $ p_n(y) \in B_n $ pour $ n $ assez grand et $ p_n(x) = a_n $ pour tout $ n $, donc $ p'(x) \neq p'(y) $, ce qui établit notre assertion.

Considérons alors l’ensemble quotient $ B_0 = N'/R_x $; soient $ q_0 $ l’application canonique de $ N' $ sur $ B_0 $, $ s_0 $ une section associée à $ q_0 $. Posons $ p_0(x) = s_0(q_0(x)) $ pour $ x \in N' $ et prolongeons $ p_0 $ à T en prenant $ p_0 $ constante dans A et égale à un élément de T. Alors $ p = (p', p_0) $ est une application $ \mu $-mesurable de T dans l’espace localement compact $ B = B' \times T $; il est immédiat que si $ x \in N' $, $ y \in N' $, la relation $ p_0(x) = p_0(y) $ entraîne R $ \{ x, y \} $; donc $ p $ répond à la question. En outre, si T admet une base dénombrable, il en est de même de chacun des espaces quotients $ B_n $ (Top. gén., chap. IX, 2e éd., § 2, no 10, prop. 17), donc B' admet une base dénombrable, et par suite aussi B.

#### Proposition 3 {#int-vi-s3-prop-3 .statement}

Soient T un espace localement compact polonais, $ \mu $ une mesure positive sur T, R une relation d’équivalence dans T. Les propriétés suivantes sont équivalentes :

a) R est $ \mu $-mesurable.

b) Il existe une suite d’applications $ p_n : T \to F_n $ dans des espaces topologiques séparés, telle que chaque $ p_n $ soit $ \mu $-mesurable et que la relation R $ \{ x, y \} $ soit équivalente à « quel que soit $ n $, $ p_n(x) = p_n(y) $ ».

c) Il existe une suite $ (A_n) $ d’ensembles $ \mu $-mesurables, saturés pour R, et tels que, pour tout $ x \in T $, la classe de x suivant R soit l’intersection de ceux des $ A_n $ qui contiennent x.

Avec les notations de l’énoncé de b), posons $ p(x) = (p_n(x)) $; la propriété b) signifie que l’application p de T dans l’espace produit $ \prod F_n $ est mesurable (chap. IV, § 5, no 3, th. 1) et que la relation $ \bigwedge^n R \{ x, y \} $ est équivalente à $ p(x) = p(y) $; donc b) entraîne a).

Montrons ensuite que c) entraîne b). Supposons c) vérifiée ; alors les fonctions caractéristiques $ \varphi_{A_n} $ sont $ \mu $-mesurables, et l’hypothèse c) signifie que la relation $ R \{ x, y \} $ est équivalente à « quel que soit $ n $, $ \varphi_{A_n}(x) = \varphi_{A_n}(y) $ ».

Enfin, montrons que a) entraîne c). En vertu de la prop. 2, il existe un espace localement compact à base dénombrable B et une application $ \mu $-mesurable $ p $ de T dans B telle que la relation $ R \{ x, y \} $ soit équivalente à $ p(x) = p(y) $. Soit $ (U_n) $ une base dénombrable de la topologie de B. Les ensembles $ A_n = p^{-1}(U_n) $ sont $ \mu $-mesurables (chap. IV, § 5, no 5, prop. 8) et saturés pour R ; et si $ x, y $ sont des points de T tels que $ p(x) \neq p(y) $, il existe un indice $ n $ tel que $ p(x) \in U_n $ et $ p(y) \notin U_n $, ce qui signifie que $ x \in A_n $ et $ y \notin A_n $.

#### Remarque {#int-vi-s3-n4-rem-1 .statement}

Si R est une relation d’équivalence $ \mu $-mesurable dans T, le saturé pour R d’une partie compacte de T n’est pas nécessairement $ \mu $-mesurable (exerc. 5).

#### Théorème 3 {#int-vi-s3-thm-3 .statement}

Soient T un espace localement compact ayant une base dénombrable, $ \mu $ une mesure positive sur T, R une relation d’équivalence $ \mu $-mesurable dans T. Il existe alors une partie $ \mu $-mesurable S de T qui rencontre toute classe suivant R en un point et un seul (« section mesurable » pour R).

On peut évidemment supposer que la mesure $ \mu $ est bornée et que $ \mu(T) \leq 1 $ (chap. V, § 5, no 6, prop. 11). Nous allons définir une suite $ (S_n) $ de parties boréliennes (Top. gén., chap. IX, 2e éd., § 6, no 3) telles que toute classe d’équivalence suivant R rencontre la réunion S’ des $ S_n $ en un point au plus, que pour tout $ n $ le saturé $ T_n $ de la réunion des $ S_p $ d’indice $ p \leq n $ soit $ \mu $-mesurable, et que l’on ait $ \mu(T - T_n) \leq 1/2^n $. Le saturé $ T' $ de S’ sera donc $ \mu $-mesurable et $ N = T - T' $ de mesure nulle. Si $ S'' $ est une section quelconque de N pour la relation $ R_N $, $ S = S' \cup S'' $ répondra à la question, car $ S' $, étant borélien, est $ \mu $-mesurable (Top. gén., chap. IX, 2e éd., § 6, no 9, th. 5, et no 3, prop. 11), et $ S'' $ est de mesure nulle.

En vertu de la prop. 2, $ R \{ x, y \} $ est équivalente à la relation $ p(x) = p(y) $, où $ p $ est une application $ \mu $-mesurable de T dans un espace localement compact F. Supposons les $ S_k $ définis pour $ k \leq n $. Comme $ T - T_n $ est $ \mu $-mesurable et de mesure $ \leq 1/2^n $, il existe dans

T – T_n une partie compacte K telle que $ \mu(T - (T_n \cup K)) \leq 1/2^{n+1} $ et que la restriction de $ p $ à K soit continue. Comme la relation induite $ R_K $ est fermée et que K est métrisable, on sait qu’il existe une partie borélienne $ S_{n+1} $ de K telle que, dans K, tout point soit congru (mod. R) à un point et un seul de $ S_{n+1} $ (Top. gén., chap. IX, 2e éd., § 6, no 8, th. 4). On a donc $ p(S_{n+1}) = p(K) $, ensemble qui est compact dans F ; le saturé de $ S_{n+1} $ pour R est l’image réciproque $ ^{-1}p(p(K)) $, qui est donc $ \mu $-mesurable (chap. IV, § 5, no 5, prop. 8) ; il est clair que cet ensemble contient K, donc la réunion $ T_{n+1} $ de $ T_n $ et de $ ^{-1}p(p(K)) $ est $ \mu $-mesurable, saturée pour R et telle que $ \mu(T - T_{n+1}) \leq 1/2^{n+1} $, ce qui achève la démonstration.

### 5. Désintégration d’une mesure par une relation d’équivalence mesurable.

Soient T un espace localement compact polonais, $ \mu $ une mesure positive sur T, R une relation d’équivalence $ \mu $-mesurable dans T. Il existe alors (no 4, prop. 2) un espace localement compact polonais B et une application $ \mu $-mesurable $ p $ de T dans B, tels que la relation $ p(x) = p(y) $ soit équivalente à $ R \{ x, y \} $. Toute mesure pseudo-image $ \nu $ de $ \mu $ par $ p $ (no 2) sera dite une mesure quotient de $ \mu $ par la relation R ; si $ b \to \lambda_b $ est une désintégration de $ \mu $ relative à la mesure $ \nu $, on dira que $ b \to \lambda_b $ est une désintégration de $ \mu $ par la relation R. En vertu des propriétés de $ p $ et des $ \lambda_b $, chacune des mesures $ \lambda_b $ est concentrée sur une classe d’équivalence suivant R, et si $ b \neq c $, les mesures $ \lambda_b $ et $ \lambda_c $ sont concentrées sur des classes distinctes.

L’espace B, l’application $ p $ et la mesure pseudo-image $ \nu $ sur B peuvent en général être choisis d’une infinité de façons. Toutefois les diverses désintégrations de $ \mu $ par R peuvent toutes se déduire de l’une d’entre elles, comme il résulte du théorème suivant :

#### Théorème 4 {#int-vi-s3-thm-4 .statement}

Soient T un espace localement compact polonais, $ \mu $ une mesure positive sur T, R une relation d’équivalence $ \mu $-mesurable dans T. Soient B, B’ deux espaces localement compacts polonais, $ p, p’ $ deux applications $ \mu $-mesurables de T dans B, B’ respectivement, tels que $ R \{ x, y \} $ soit équivalente à $ p(x) = p(y) $ et à p'(x) = p'(y). Soient $ \nu, \nu' $ des mesures pseudo-images de $ \mu $ par $ p, p' $ respectivement ; soient $ b \to \lambda_b, b' \to \lambda'_b $, des désintégrations de $ \mu $ relatives à $ \nu, \nu' $ respectivement.

Dans ces conditions, il existe dans B (resp. B') un ensemble N (resp. N') négligeable pour $ \nu $ (resp. $ \nu' $) et une bijection $ f $ de B - N sur $ B' - N' $, tels que l'on ait les propriétés suivantes :

a) L'application $ f $ (définie presque partout dans B) est $ \nu $-mesurable et son application réciproque $ f' $ est $ \nu' $-mesurable ; toute mesure pseudo-image de $ \nu $ (resp. $ \nu' $) par $ f $ (resp. $ f' $) est équivalente à $ \nu' $ (resp. $ \nu $).

b) Pour tout $ b \in B - N $, la mesure $ \lambda'_{f(b)} $ sur T est de la forme $ r(b)\lambda_b $, où $ r(b) \neq 0 $ et $ r $ est localement $ \nu $-intégrable.

Pour établir a), on peut se limiter au cas où $ \nu $ et $ \nu' $ sont des mesures bornées (chap. V, § 5, no 6, prop. 11). Soient $ N_0 = B - p(T) $, $ N'_0 = B' - p'(T) $; on sait que $ N_0 $ (resp. $ N'_0 $) est négligeable pour $ \nu $ (resp. $ \nu' $) (no 2). Il existe une bijection $ f $ de $ B - N_0 $ sur $ B' - N'_0 $ définie par $ f(p(t)) = p'(t) $ pour tout $ t \in T $; soit $ f' $ l'application réciproque de $ f $, telle que $ f'(p'(t)) = p(t) $. Pour toute partie M de B, la relation « M est $ \nu $-mesurable » équivaut à « $ p^{-1}(M) $ est $ \mu $-mesurable », c'est-à-dire à « $ p'^{-1}(f(M)) $ est $ \mu $-mesurable », donc enfin à « $ f(M) $ est $ \nu' $-mesurable » (chap. V, § 6, no 2, cor. de la prop. 3). On voit donc que $ f $ (resp. $ f' $) transforme tout ensemble $ \nu $-mesurable (resp. $ \nu' $-mesurable) en un ensemble $ \nu' $-mesurable (resp. $ \nu $-mesurable) ; comme B et B' sont métrisables et ont des bases dénombrables, on en déduit que $ f $ et $ f' $ sont mesurables (chap. IV, § 5, no 5, th. 4). En outre, si $ M \subset B $ est $ \nu $-négligeable, $ p^{-1}(M) = p'^{-1}(f(M)) $ est $ \mu $-négligeable, donc $ f(M) $ est $ \nu' $-négligeable (chap. V, § 6, no 2, cor. 2 de la prop. 2) ; de même $ f' $ transforme tout ensemble $ \nu' $-négligeable en un ensemble $ \nu $-négligeable. Par suite, l'image de $ \nu $ par $ f $ (qui est définie puisque $ \nu $ est bornée, ce qui entraîne que $ f $ est $ \nu $-propre) est équivalente à $ \nu' $ et l'image de $ \nu' $ par $ f' $ est équivalente à $ \nu $ (chap. V, § 5, no 6, prop. 10). Reste à montrer b). En vertu du th. 2 du no 3, on peut se limiter au cas où $ \nu' = f(\nu) $. Comme on a $ \mu = \int \lambda'_b d\nu'(b') $, on a, pour toute fonction $ h \in \mathcal{K}(T) $

$$
\int h(t)d\mu(t) = \int d\nu'(b') \int h(t)d\lambda'_b(t) = \int d\nu(b) \int h(t)d\lambda'_{f(b)}(t)
$$

(chap. V, § 3, n° 4, th. 1, et § 6, n° 2, th. 1) ; autrement dit, on a
$$
\mu = \int \lambda_{f(b)}' d\nu(b).
$$
Mais comme on a aussi $ \mu = \int \lambda_b d\nu(b) $ et que,
pour tout $ b \in B - N_0 $, $ \lambda_b $ et $ \lambda_{f(b)}' $ sont portées par $ p^{-1}(b) $, le th. 2 du n° 3 entraîne que $ \lambda_b = \lambda_{f(b)}' $ pour presque tout $ b \in B - N_0 $, et par suite pour presque tout $ b \in B $. Les conditions du th. 4 sont donc vérifiées en prenant pour $ N $ la réunion de $ N_0 $ et de l’ensemble des $ b \in B $ tels que $ \lambda_b \neq \lambda_{f(b)}' $.

## EXERCICES {#int-vi-s3-exercises}

See the [exercises for § 3](exercises/s3/).
