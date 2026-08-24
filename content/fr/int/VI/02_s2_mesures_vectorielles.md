---
book: int
book_title: Integration
chapter: VI
chapter_title: Intégration vectorielle
section: 2
section_title: Mesures vectorielles
lang: fr
source: int-vi-fr
pdf_pages: 0029-0057, 0087-0096
extraction: ocr
subsections:
    - "no": 1
      title: Définition d’une mesure vectorielle.
      page: 0
      pdf_page: 29
    - "no": 2
      title: Intégration par rapport à une mesure vectorielle.
      page: 0
      pdf_page: 31
    - "no": 3
      title: Mesures vectorielles majorables.
      page: 0
      pdf_page: 35
    - "no": 4
      title: Mesures vectorielles de base $ \mu $.
      page: 0
      pdf_page: 39
    - "no": 5
      title: Le théorème de Dunford-Pettis.
      page: 0
      pdf_page: 42
    - "no": 6
      title: Dual de l'espace $ L^1_F $ (F espace de Banach de type dénombrable).
      page: 0
      pdf_page: 47
    - "no": 7
      title: Intégration d'une fonction vectorielle par rapport à une mesure vectorielle.
      page: 0
      pdf_page: 48
    - "no": 8
      title: Mesures complexes.
      page: 0
      pdf_page: 50
    - "no": 9
      title: Mesures complexes bornées.
      page: 0
      pdf_page: 54
    - "no": 10
      title: Image d'une mesure complexe ; mesure complexe induite ; produit de mesures complexes.
      page: 0
      pdf_page: 55
statements: 46
exercises: 27
content_sha256: 11f3aa2aad7ad343645f025e01ca7cbfc405719bf3555a62abd1ff80cdfaf752
---

## § 2. Mesures vectorielles

### 1. Définition d’une mesure vectorielle.

La définition d’une mesure donnée au chap. III, § 2, n° 2 se généralise comme suit :

#### Définition 1 {#int-vi-s2-def-1 .statement}

Soit F un espace localement convexe séparé sur $ \mathbf{R} $. On appelle mesure vectorielle sur T à valeurs dans F toute application linéaire continue de l’espace $ \mathcal{K}(T) $ dans F.

La déf. 1 peut encore s’exprimer de la façon suivante : une mesure vectorielle sur T à valeurs dans F est une application linéaire $ m $ de $ \mathcal{K}(T) $ dans F telle que, pour toute partie compacte K de T, la restriction de $ m $ à $ \mathcal{K}(T, K) $ soit continue pour la topologie de la convergence uniforme. Si $ f \in \mathcal{K}(T) $, on écrit encore $ \int f d\mathbf{m} $ ou $ \int f(t) d\mathbf{m}(t) $ au lieu de $ m(f) $. Les mesures à valeurs dans $ \mathbf{R} $ (c’est-à-dire les mesures définies au chap. III, § 2, no 2) sont parfois appelées mesures réelles ou mesures scalaires sur T.

#### Exemple 1 {#int-vi-s2-n1-exa-1 .statement}

L’application identique de $ \mathcal{K}(T) $ est une mesure vectorielle sur T à valeurs dans $ \mathcal{K}(T) $.

#### Exemple 2 {#int-vi-s2-n1-exa-2 .statement}

*Soient H un espace hilbertien complexe, $ \mathcal{L}(H) $ l’algèbre normée des endomorphismes continus de H. Soit A une sous-algèbre de $ \mathcal{L}(H) $, commutative, fermée, autoadjointe et contenant l’identité ; on démontre qu’il existe un espace compact X et un isomorphisme de l’algèbre normée A sur l’algèbre $ \mathcal{K}_c(X) $ des fonctions complexes continues dans X, munie de la norme $ \|f\| = \sup_{x \in X} |f(x)| $. L’isomorphisme réciproque, restreint à $ \mathcal{K}(X) $, est une mesure $ m $ sur X, à valeurs dans $ \mathcal{L}(H) $, telle que $ m(fg) = m(f)m(g) $.*

#### Remarque 1 {#int-vi-s2-n1-rem-1 .statement}

Pour qu’une application linéaire $ m $ de $ \mathcal{K}(T) $ dans F soit une mesure vectorielle, il faut et il suffit que, pour toute partie compacte K de T, l’image par $ m $ de la boule unité $ \|f\| \leq 1 $ de $ \mathcal{K}(T, K) $ soit bornée dans F. La notion de mesure vectorielle à valeurs dans F est donc la même pour toutes les topologies localement convexes séparées sur F admettant les mêmes ensembles bornés, et en particulier pour toutes les topologies compatibles avec la dualité entre F et $ F' $ (Esp. vect. top., chap. IV, § 2, no 4, th. 3).

#### Remarque 2 {#int-vi-s2-n1-rem-2 .statement}

Soient $ T_1 $ un espace localement compact, $ F_1 $ un espace localement convexe séparé sur $ \mathbf{R} $, $ u $ une application linéaire continue de $ \mathfrak{J}_i(T_1) $ dans $ \mathfrak{J}_i(T) $, $ \varphi $ une application linéaire continue de $ F $ dans $ F_1 $. Si $ m $ est une mesure vectorielle sur $ T $ à valeurs dans $ F $, $ \varphi \circ m \circ u $ est une mesure vectorielle sur $ T_1 $ à valeurs dans $ F_1 $. En particulier, si $ g $ est une fonction numérique finie et continue dans $ T $, $ f \to m(gf) $ est une mesure vectorielle sur $ T $ à valeurs dans $ F $, que l’on note $ g.m $; si $ h $ est une seconde fonction numérique finie et continue dans $ T $, on a $ g.(h.m) = (gh).m $.

#### Remarque 3 {#int-vi-s2-n1-rem-3 .statement}

Comme l’espace $ \mathfrak{J}_i(T) $ est limite inductive des espaces de Banach $ \mathfrak{K}(T, K) $, et en particulier est tonnelé ($ Esp.\ vect.\ top. $, chap. III, § 1, no 1, cor. de la prop. 1 et no 2, prop. 2), pour qu’une application linéaire $ m $ de $ \mathfrak{J}_i(T) $ dans $ F $ soit une mesure vectorielle, il faut et il suffit que, pour tout $ z' \in F' $, $ z' \circ m $ soit une mesure scalaire sur $ T $ ($ Esp.\ vect.\ top. $, chap. IV, § 4, no 1, prop. 1 et no 2, cor. de la prop. 7).

#### Remarque 4 {#int-vi-s2-n1-rem-4 .statement}

Compte tenu de la remarque 1, la prop. 1 du chap. III, § 3, no 1 et sa démonstration sont encore valables pour les mesures vectorielles. On peut donc encore définir le support d’une mesure vectorielle $ m $ sur $ T $ comme le complémentaire du plus grand ensemble ouvert $ U \subset T $ tel que la restriction de $ m $ à $ U $ soit nulle.

### 2. Intégration par rapport à une mesure vectorielle.

Soit $ m $ une mesure vectorielle sur $ T $, à valeurs dans $ F $. Pour tout $ z' \in F' $, l’application $ z' \circ m $ est une mesure scalaire sur $ T $, dépendant linéairement de $ z' $. Si $ f $ est une fonction numérique définie dans $ T $, nous dirons, par abus de langage, que le couple $ (f, m) $ possède une propriété $ P $ si, pour tout $ z' \in F' $, le couple $ (f, |z' \circ m|) $ possède la propriété $ P $. Par exemple, on dira que $ f $ est essentiellement intégrable pour $ m $ si, pour tout $ z' \in F' $, la fonction $ f $ est essentiellement intégrable pour $ |z' \circ m| $. Il revient au même de dire que $ f $ est essentiellement intégrable pour chacune des mesures $ (z' \circ m)^+ $ et $ (z' \circ m)^- $ (chap. V, § 3, no 5, cor. 1 de la prop. 6).

#### Proposition 1 {#int-vi-s2-prop-1 .statement}

Soient $ m $ une mesure vectorielle sur $ T $ à valeurs dans $ F $, $ f $ une fonction numérique sur $ T $, essentiellement intégrable pour $ m $. L’application
$$
z' \to \int f d(z' \circ m)^+ - \int f d(z' \circ m)^-
$$
est une forme linéaire sur $ F' $.

Si on désigne cette application par $ \Phi $, il est immédiat que $ \Phi(\lambda z') = \lambda \Phi(z') $ pour tout $ \lambda \in \mathbf{R} $. Tout revient à voir que $ \Phi(y' + z') = \Phi(y') + \Phi(z') $. Posons $ \mu = |y' \circ m| + |z' \circ m| $; en vertu du th. de Lebesgue-Nikodym, on peut alors écrire $ y' \circ m = g \cdot \mu $ et $ z' \circ m = h \cdot \mu $, où $ g $ et $ h $ sont deux fonctions numériques localement $ \mu $-intégrables et bornées (chap. V, § 5, no 5, th. 2); en outre, on a $ (y' \circ m)^+ = g^+ \cdot \mu $ et $ (y' \circ m)^- = g^- \cdot \mu $, et les relations analogues lorsque $ y' $ est remplacé par $ z' $ (resp. $ y' + z' $) et $ g $ par $ h $ (resp. $ g + h $). Cela étant, il est immédiat que $ f $ est essentiellement $ \mu $-intégrable (chap. V, § 3, no 5, cor. 1 de la prop. 6), et la relation à démontrer se réduit à $ (g + h)^+ - (g + h)^- = (g^+ - g^-) + (h^+ - h^-) $, qui est évidente.

#### Définition 2 {#int-vi-s2-def-2 .statement}

Soient $ m $ une mesure vectorielle sur $ T $ à valeurs dans $ F $, $ f $ une fonction numérique sur $ T $, essentiellement intégrable pour $ m $. On appelle intégrale de $ f $ par rapport à $ m $ et on note $ m(f) $ ou $ \int f d|m| $ ou encore $ \int f(t) d|m|(t) $ l’élément de $ F' $* défini par

$$
\langle z', \int f d|m| \rangle = \int f d(z' \circ m)^+ - \int f d(z' \circ m)^-.
$$

Remarquons que si $ f \in \mathcal{K}(T) $, l’élément $ \int f d|m| $ ainsi défini coïncide avec l’élément noté de même au no 1, car le second membre de (1) est alors $ \int f d(z' \circ m) = z'(m(f)) $ par définition. En outre, si on applique en particulier la déf. 2 au cas où $ F = \mathbf{R} $, on voit que pour tout $ z' \in F' $, $ f $ est essentiellement intégrable pour la mesure réelle $ z' \circ m $, et que le second membre de (1) peut s’écrire $ \int f d(z' \circ m) $.

Supposons $ f $ essentiellement intégrable pour $ m $, et soit $ z' \in F' $. Posons $ \mu = |z' \circ m| $; en vertu du th. de Lebesgue-Nikodym, on peut écrire $ z' \circ m = g \cdot \mu $, où $ g $ est localement $ \mu $-intégrable et $ \|g\| \leq 1 $, et la démonstration de la prop. 1 montre que $ \int f d(z' \circ m) = \int f g d\mu $. On a par suite

$$
\left| \int f d(z' \circ m) \right| \leq \int |f| d|z' \circ m|.
$$

Il est clair que l’ensemble des fonctions numériques finies essentiellement intégrables pour $ m $ est un espace vectoriel sur $ \mathbf{R} $; nous désignerons par $ \mathcal{L}(m) $ cet espace muni de la topologie localement convexe la moins fine rendant continues toutes les formes linéaires $ f \to \int f d(z' \circ m) $, où $ z' $ parcourt $ F' $. On notera qu’en général l’espace localement convexe $ \mathcal{L}(m) $ est non séparé.

#### Exemple {#int-vi-s2-n2-exa-1 .statement}

Prenons pour $ m $ l’application identique de $ \mathcal{K}(T) $ sur lui-même. Comme le dual de $ \mathcal{K}(T) $ est l’espace $ \mathcal{M}(T) $ des mesures scalaires sur $ T $, les fonctions $ f \in \mathcal{L}(m) $ sont celles qui sont essentiellement intégrables pour toute mesure scalaire $ \mu $ (cf. exerc. 1), et l’intégrale $ \int f d\mathbf{m} $ est la forme linéaire $ \mu \to \int f d\mu $ sur $ \mathcal{M}(T) $. On ne peut avoir $ \int f d\mu = 0 $ pour toute mesure $ \mu \in \mathcal{M}(T) $ que si $ f = 0 $, comme on le voit en prenant $ \mu = \varepsilon_t $, où $ t $ est arbitraire dans $ T $; autrement dit l’application $ f \to \int f d\mathbf{m} $ est une injection de $ \mathcal{L}(m) $ dans le dual algébrique de $ \mathcal{K}(T) $, qui prolonge l’application identique de $ \mathcal{K}(T) $. La relation $ \int f d\mathbf{m} \in F = \mathcal{K}(T) $ est donc équivalente à $ f \in \mathcal{K}(T) $.

Soit $ u $ une application linéaire continue de $ F $ dans un espace localement convexe séparé $ G $, et notons encore $ u $ son prolongement par bitransposition en une application linéaire de $ F'^* $ dans $ G'^* $ (\$ 1, no 1). Avec cette convention :

#### Proposition 2 {#int-vi-s2-prop-2 .statement}

Toute fonction numérique $ f $ essentiellement intégrable pour $ m $ est essentiellement intégrable pour $ u \circ m $, et on a
$$
\int f d(u \circ m) = u \left( \int f d\mathbf{m} \right).
$$
La proposition est évidente, compte tenu de l’égalité $ y' \circ u \circ m = 'u(y') \circ m $ pour tout $ y' \in G' $.

En général, si $ f \in \mathcal{L}(m) $, l’intégrale $ \int f d\mathbf{m} $ appartient à $ F'^* $ mais non à $ F $ (voir Exemple ci-dessus). Cependant :

#### Proposition 3 {#int-vi-s2-prop-3 .statement}

Si l’image par $ m $ de l’ensemble des $ f \in \mathcal{K}(T) $ telles que $ \sup_{t \in T} |f(t)| \leq 1 $ est faiblement relativement compacte dans $ F $, alors on a $ \int f d\mathbf{m} \in F $ pour toute fonction numérique bornée $ f $ essentiellement intégrable pour $ m $.

Soit $ A $ l’ensemble des $ f \in \mathcal{L}(m) $ telles que $ \sup_{t \in T} |f(t)| \leq 1 $, et soit $ B = A \cap \mathcal{K}(T) $ : par hypothèse, $ m(B) $ est faiblement relativement compact dans $ F $, et il suffit donc de montrer que $ m(A) $ est contenu dans l’adhérence (dans $ F' \ast $) de $ m(B) $ pour la topologie $ \sigma(F', F') $; comme $ m(B) $ est convexe et équilibré, il suffit de prouver que le polaire de $ m(B) $ dans $ F' $ est contenu dans celui de $ m(A) $ ($ Esp.\ vect.\ top.\$$ ), chap. IV, § 1, no 3, prop. 3). Or, pour qu’une forme linéaire$  z' \in F' $ appartienne à $ (m(B))^0 $, il faut et il suffit que
$$
|\langle z', m(g) \rangle| = \left| \int g d(z' \circ m) \right| \leq 1 \text{ pour toute fonction } g \in B,
$$
qui signifie que la mesure scalaire $ |z' \circ m| $ est bornée et de norme $ \leq 1 $ (chap. III, § 2, no 6, prop. 3) ; mais d’après (2) cette dernière condition entraîne $ |\langle z', m(f) \rangle| \leq 1 $ pour toute fonction $ f \in A $, d’où $ z' \in (m(A))^0 $.

#### Corollaire 1 {#int-vi-s2-prop-3-cor-1 .statement}

Si, pour toute partie compacte $ K $ de $ T $, l’image par $ m $ de l’ensemble des $ f \in \mathcal{K}(T, K) $ telles que $ \sup_{t \in T} |f(t)| \leq 1 $ est relativement faiblement compacte dans $ F $, alors on a $ \int f d\mathbf{m} \in F $ pour toute fonction $ f \in \mathcal{L}(m) $ bornée et à support compact, et $ \int f d\mathbf{m} \in F'' $ pour toute fonction $ f \in \mathcal{L}(m) $.

La première assertion se déduit immédiatement de la prop. 3 : si $ f $ est bornée et à support compact, et si $ U $ est un voisinage ouvert relativement compact du support de $ f $, la restriction de $ m $ au sous-espace $ \mathcal{K}(U) $ est une mesure $ m_u $ sur $ U $ qui vérifie les conditions de la prop. 3, et on a $ \int f d\mathbf{m}_u = \int f d\mathbf{m} $ (chap. V, § 7, no 1, th. 1), donc $ \int f d\mathbf{m} \in F $.

Soit maintenant $ f $ quelconque dans $ \mathcal{L}(m) $; pour toute partie compacte $ K $ de $ T $ et tout entier $ n > 0 $, soit $ f_{n, K} $ la fonction numérique sur $ T $ définie comme suit : si $ t \notin K $, $ f_{n, K}(t) = 0 $; si $ t \in K $ et $ |f(t)| \leq n $, $ f_{n, K}(t) = f(t) $; enfin, si $ t \in K $ et $ |f(t)| > n $, $ f_{n, K}(t) = nf(t)/|f(t)| $. Il est clair que pour tout $ t \in T $, $ f(t) $ est limite de $ f_{n, K}(t) $ suivant le filtre produit du filtre de Fréchet par le filtre des sections de l’ensemble ordonné (filtrant croissant) des parties compactes de $ T $. Comme $ |f_{n, K}| \leq |f| $, il résulte du th. de Lebesgue et de la prop. 8 du chap. V, § 2, no 2, appliqués à chaque mesure scalaire $ |\mathbf{z}' \circ m| $, que $ f_{n, K} $ converge vers $ f $ dans $ \mathcal{L}(m) $ suivant le filtre précédent. Par suite, l’intégrale $ \int f d\mathbf{m} $ est adhérente dans $ F' * $ (pour la topologie $ \sigma(F', F') $) à l’ensemble $ M $ des $ m(f_{n, K}) $. Mais la première partie du corollaire montre que $ M \subset F $, et d’autre part, pour tout $ \mathbf{z}' \in F' $, on a $ |\langle \mathbf{z}', m(f_{n, K}) \rangle| \leq \int |f| d|\mathbf{z}' \circ m| $, ce qui montre que $ M $ est borné dans $ F_\sigma $, et par suite dans $ F $ (*Esp. vect. top.*, chap. IV, § 2, no 4, th. 3). Le lemme 1 du § 1, no 2 montre donc que $ \int f d\mathbf{m} \in F'' $.

#### Corollaire 2 {#int-vi-s2-prop-3-cor-2 .statement}

*Si F est semi-réflexif, on a* $ \int f d\mathbf{m} \in F $ *pour toute fonction numérique f essentiellement intégrable pour m.*

### 3. Mesures vectorielles majorables.

Soit $ q $ une semi-norme semi-continue inférieurement sur $ F $. Nous désignerons par $ A_q' $ l’ensemble des $ \mathbf{z}' \in F' $ tels que $ |\langle \mathbf{z}', \mathbf{x} \rangle| \leq q(\mathbf{x}) $ pour tout $ \mathbf{x} \in F $. C’est le polaire dans $ F' $ de l’ensemble des $ \mathbf{x} \in F $ tels que $ q(\mathbf{x}) \leq 1 $; pour tout $ \mathbf{x} \in F $, on a $ q(\mathbf{x}) = \sup_{\mathbf{z}' \in A_q'} |\langle \mathbf{x}, \mathbf{z}' \rangle| $.

#### Définition 3 {#int-vi-s2-def-3 .statement}

*Soit m une mesure vectorielle sur T à valeurs dans F. Si q est une semi-norme semi-continue inférieurement sur F, on dit que m est q-majorable s’il existe une mesure positive $ \mu $ telle que* $ |\mathbf{z}' \circ m| \leq \mu $ *pour tout* $ \mathbf{z}' \in A_q' $; *la borne supérieure des mesures* | $ z' \circ m $ | lorsque $ z' $ parcourt $ A_q' $ (chap. III, § 2, n° 4, th. 3) se note alors $ q(m) $. On dit que $ m $ est majorable si elle est $ q $-majorable pour toute semi-norme $ q $ continue sur $ F $.

Si $ m $ et $ m' $ sont toutes deux $ q $-majorables, il est immédiat que $ m + m' $ est aussi $ q $-majorable et que l'on a
$$
q(m + m') \leq q(m) + q(m').
$$

Lorsque $ F $ est un espace normé, dont la norme est notée $ |x| $, dire que $ m $ est majorable signifie donc que les mesures $ |z' \circ m| $, où $ |z'| \leq 1 $, sont majorées par une même mesure positive ; on note alors $ |m| $ la borne supérieure de cette famille de mesures.

Si $ F = \mathbf{R} $, la mesure $ |m| $, correspondant à la norme euclidienne $ |x| $ sur $ \mathbf{R} $, coïncide avec la mesure notée $ |m| $ au chap. III, § 2, n° 4.

#### Proposition 4 {#int-vi-s2-prop-4 .statement}

Soient $ (F_i)_{1 \leq i \leq n} $ une famille finie d'espaces localement convexes séparés, $ F = \prod_{i=1}^n F_i $ leur produit, $ q_i $ ($ 1 \leq i \leq n $) une semi-norme semi-continue inférieurement sur $ F_i $, $ q $ la semi-norme sur $ F $ définie par $ q(x_1, \ldots, x_n) = \sum_{i=1}^n q_i(x_i) $. Si $ m_i $ ($ 1 \leq i \leq n $) est une mesure vectorielle sur $ T $ à valeurs dans $ F_i $ et $ q_i $-majorable, la mesure $ m = (m_1, \ldots, m_n) $ à valeurs dans $ F $ est $ q $-majorable.

En effet, le dual $ F' $ s'identifie à $ \prod_{i=1}^n F_i' $, de façon que si $ x = (x_i) \in F $, $ z' = (z_i') \in F' $, on ait $ \langle x, z' \rangle = \sum_{i=1}^n \langle x_i, z_i' \rangle $. Si $ |\langle x, z' \rangle| \leq q(x) $ pour tout $ x \in F $, on a en particulier $ |\langle x_i, z_i' \rangle| \leq q_i(x_i) $ pour $ 1 \leq i \leq n $, et la réciproque est évidente, ce qui montre que l'ensemble $ A_q' $ est le produit des $ A_{q_i}' $. Comme par hypothèse on a $ |z_i' \circ m_i| \leq q_i(m_i) $ pour $ z_i' \in A_{q_i}' $, on en conclut que
$$
|z' \circ m| \leq \sum_{i=1}^n |z_i' \circ m_i| \leq \sum_{i=1}^n q_i(m_i)
$$
pour tout $ z' \in A_q' $, ce qui démontre la proposition.

#### Corollaire {#int-vi-s2-n3-cor-1 .statement}

Si l’espace F est de dimension finie, toute mesure vectorielle m à valeurs dans F est majorable. Pour qu’une fonction numérique soit essentiellement intégrable pour m, il faut et il suffit qu’elle soit essentiellement intégrable pour $ |\mathbf{m}|(|\mathbf{x}| $ désignant une norme quelconque sur F$)$.

#### Proposition 5 {#int-vi-s2-prop-5 .statement}

Soit q une semi-norme semi-continue inférieurement sur F. Soit m une mesure q-majorable, et soit f une fonction essentiellement intégrable pour m et telle que$  \int f d\mathbf{m} \in F $. Alors on a
$$
q\left( \int f d\mathbf{m} \right) \leq \int^* |f| dq(\mathbf{m}).
$$
En effet, on a
$$
q\left( \int f d\mathbf{m} \right) = \sup_{\mathbf{z}' \in \mathbb{A}_q'} |\langle \mathbf{z}', \int f d\mathbf{m} \rangle| \leq \sup_{\mathbf{z}' \in \mathbb{A}_q'} \int |f| d|\mathbf{z}' \circ \mathbf{m}| \leq \int^* |f| dq(\mathbf{m})
$$
en vertu de (1) et de la relation $ |\mathbf{z}' \circ \mathbf{m}| \leq q(\mathbf{m}) $ pour $ \mathbf{z}' \in \mathbb{A}_q' $.

#### Proposition 6 {#int-vi-s2-prop-6 .statement}

Soient F un espace localement convexe séparé quasi-complet, m une mesure majorable sur T à valeurs dans F. Si f est une fonction numérique essentiellement intégrable pour toutes les mesures q(m) (q parcourant l’ensemble des semi-normes continues sur F), alors f est essentiellement intégrable pour m, et l’on a $ \int f d\mathbf{m} \in F $.

Nous utiliserons le résultat auxiliaire suivant. Soit $ (\mu_i)_{i \in I} $ une famille filtrante croissante de mesures positives sur T. Désignons par $ \mathcal{L}^1((\mu_i)_{i \in I}) $ l’espace vectoriel des fonctions numériques finies sur T, essentiellement $ \mu_i $-intégrables pour tout $ i \in I $, muni de la topologie définie par les semi-normes $ f \to \mu_i(|f|) $ ($ i \in I $). Soit $ \mathcal{L}_0 $ le sous-espace vectoriel de $ \mathcal{L}^1((\mu_i)_{i \in I}) $ engendré par les produits $ g \varphi_K $ où g parcourt l’ensemble des fonctions numériques finies continues dans T et K l’ensemble des parties compactes de T.

#### Lemme 1 {#int-vi-s2-lem-1 .statement}

Lorsqu’on munit $ \mathcal{L}_0 $ et $ \mathfrak{K}(T) $ de la topologie induite par celle de $ \mathcal{L}^1((\mu_i)_{i \in I}) $ :
a) tout élément de $ \mathcal{L}_0 $ est adhérent à une partie bornée de $ \mathfrak{K}(T) $;

b) tout élément de $ \mathcal{L}^1((\mu_i)_{i \in I}) $ est adhérent à une partie bornée de $ \mathcal{L}_0 $.

Pour démontrer $ a) $, on peut se restreindre au cas d’un élément de la forme $ f = g \varphi_K $ ($ g \in C(T) $, K compact dans T). Il est immédiat (en vertu du th. d’Urysohn) que $ f $ est adhérente à l’ensemble B des fonctions de la forme $ gh $, où $ h $ décrit l’ensemble des applications continues de T dans $ [0, 1] $, égale à 1 dans K et à 0 dans le complémentaire d’un voisinage compact fixe H de K. De plus, l’ensemble B est borné, car $ \mu_i(|gh|) \leq \mu_i(|g \varphi_H|) $ pour toute fonction $ h $ ayant les propriétés précédentes.

Démontrons maintenant $ b) $ : on peut se restreindre au cas d’un élément $ f \geq 0 $ de $ \mathcal{L}^1((\mu_i)_{i \in I}) $. Pour tout $ i \in I $ et tout $ \varepsilon > 0 $, il existe une partie compacte $ K(i, \varepsilon) $ de T telle que la restriction de $ f $ à $ K(i, \varepsilon) $ soit continue et que $ \mu_i(|f - f \varphi_{K(i, \varepsilon)}|) \leq \varepsilon $. Il est clair que $ f $ est adhérente à l’ensemble C des $ f \varphi_{K(i, \varepsilon)} $ (où $ i \in I, \varepsilon > 0 $). En vertu du th. d’Urysohn, l’ensemble C est contenu dans $ \mathcal{L}_0 $; de plus, il est borné, car on a $ \mu_x(f \varphi_{K(i, \varepsilon)}) \leq \mu_x(f) $ quels que soient $ i \in I, x \in I $ et $ \varepsilon > 0 $.

Démontrons maintenant la prop. 6 : pour toute fonction $ g \in \mathcal{J}(T) $ et toute semi-norme continue $ q $ sur F, on a
$$
q\left( \int g d\mathbf{m} \right) \leq \int |g| \, d(q(\mathbf{m})) \quad \text{(prop. 5)},
$$
ce qui entraîne que l’application $ g \to \int g d\mathbf{m} $ de $ \mathcal{J}(T) $ dans F est continue lorsqu’on munit $ \mathcal{J}(T) $ de la topologie induite par celle de $ \mathcal{L}^1((q(\mathbf{m})))_{q \in Q} $ (Q ensemble des semi-normes continues sur F). Par suite, d’après le lemme précédent, et la prop. 8 de Esp. vect. top., chap. III, § 2, no 5, cette application se prolonge par continuité, tout d’abord en une application linéaire continue $ \varphi_0 $ de $ \mathcal{L}_0 $ dans F, puis en une application linéaire continue $ \varphi $ de $ \mathcal{L}^1((q(\mathbf{m})))_{q \in Q} $ dans F. En outre, pour tout $ z' \in F' $, la relation $ \langle z', \varphi(f) \rangle = \int f d(z' \circ \mathbf{m}) $ est vraie par définition de $ \varphi $ pour toute $ f \in \mathcal{J}(T) $; comme $ |z' \circ \mathbf{m}| \leq q(\mathbf{m}) $ pour $ q(z) = |\langle z', z \rangle| $, l’application $ f \to \int f d(z' \circ \mathbf{m}) $ est continue dans $ \mathcal{L}^1((q(\mathbf{m})))_{q \in Q} $, donc on a encore par continuité, la relation

$$
\langle \mathbf{z}', \varphi(f) \rangle = \int f d(\mathbf{z}' \circ \mathbf{m}) \text{ pour toute fonction } f \in \mathcal{L}^1((q(\mathbf{m}))_{q \in Q}). \text{ On en conclut } \varphi(f) = \int f d\mathbf{m}, \text{ ce qui achève la démonstration.}
$$

### 4. Mesures vectorielles de base $ \mu $.

#### Définition 4 {#int-vi-s2-def-4 .statement}

*Soit $ \mu $ une mesure positive sur $ T $. On dit qu'une mesure vectorielle $ \mathbf{m} $ sur $ T $, à valeurs dans $ F $, est une mesure de base $ \mu $ s'il existe une application $ \mathbf{f} $ de $ T $ dans $ F $, scalairement localement $ \mu $-intégrable et telle que $ \mathbf{m}(g) = \int g \mathbf{f} d\mu $ pour toute fonction $ g \in \mathcal{J}_i(T) $. On dit alors que $ \mathbf{f} $ est une densité de $ \mathbf{m} $ par rapport à $ \mu $, et on écrit $ \mathbf{m} = \mathbf{f} \cdot \mu $.*

Il est immédiat que si $ \mathbf{f}_1 $ et $ \mathbf{f}_2 $ sont deux densités de $ \mathbf{m} $ par rapport à $ \mu $, $ \mathbf{f}_1 - \mathbf{f}_2 $ est scalairement localement $ \mu $-négligeable (chap. V, § 5, no 4, cor. 2 de la prop. 5); rappelons que cela n'entraîne pas en général que $ \mathbf{f}_1 - \mathbf{f}_2 $ soit nulle localement presque partout (cf. § 1, exerc. 12 et no 1, Remarque 2).

Soit $ \mathbf{m} $ une mesure de base $ \mu $, de densité $ \mathbf{f} $. Pour qu'une fonction numérique $ g $ soit essentiellement intégrable pour $ \mathbf{m} $, il faut et il suffit que $ g \mathbf{f} $ soit scalairement essentiellement $ \mu $-intégrable (chap. V, § 3, no 5, th. 1).

#### Proposition 7 {#int-vi-s2-prop-7 .statement}

*Soit $ \mathbf{f} $ une application scalairement localement intégrable par rapport à une mesure positive $ \mu $ sur $ T $, telle que, pour toute fonction $ g \in \mathcal{J}_i(T) $, l'on ait $ \int g \mathbf{f} d\mu \in F $. Alors l'application $ g \to \int g \mathbf{f} d\mu $ de $ \mathcal{J}_i(T) $ dans $ F $ est une mesure vectorielle sur $ T $, de base $ \mu $ et de densité $ \mathbf{f} $ par rapport à $ \mu $.*

En effet (no 1, Remarque 3), il suffit de montrer que, si on pose $ \mathbf{m}(g) = \int g \mathbf{f} d\mu $, $ \mathbf{z}' \circ \mathbf{m} $ est une mesure scalaire pour tout $ \mathbf{z}' \in F' $. Mais comme $ \mathbf{z}'(\mathbf{m}(g)) = \int g \langle \mathbf{z}', \mathbf{f} \rangle d\mu $, on a $ \mathbf{z}' \circ \mathbf{m} = \langle \mathbf{z}', \mathbf{f} \rangle \cdot \mu $, d'où notre assertion.

#### Proposition 8 {#int-vi-s2-prop-8 .statement}

Soient $ \mu $ une mesure positive sur $ T $, $ m $ une mesure sur $ T $ à valeurs dans $ F $, de base $ \mu $ et de densité $ f $ par rapport à $ \mu $. Soit $ q $ une semi-norme semi-continue inférieurement sur $ F $.

a) Si, pour toute partie compacte $ K $ de $ T $, l'intégrale supérieure $ \int_K^{*} (q \circ f) d\mu $ est finie, alors $ m $ est $ q $-majorable.

b) Si $ m $ est $ q $-majorable, alors $ q(m) $ est de base $ \mu $; si de plus $ f $ est $ \mu $-mesurable en tant qu'application de $ T $ dans $ F_{\sigma} $, alors $ q \circ f $ est localement $ \mu $-intégrable, et on a $ q(m) = (q \circ f) \cdot \mu $.

a) Pour toute partie finie $ J $ de $ A'_q $, désignons par $ \lambda_J $ la borne supérieure des mesures $ |z' \circ m| $ où $ z' $ parcourt $ J $; si $ g_J = \sup_{z' \in J} |\langle z', f \rangle| $ on a $ \lambda_J = g_J \cdot \mu $ (chap. V, § 5, no 4, prop. 5).

Pour toute partie ouverte relativement compacte $ U $ de $ T $, soit $ \lambda_{J, U} $ la restriction de $ \lambda_J $ à $ U $; montrons d'abord que lorsque $ J $ parcourt l'ensemble filtrant $ \mathfrak{F} $ des parties finies de $ A'_q $, la famille $ (\lambda_{J, U}) $ est majorée dans $ \mathcal{M}(U) $. En effet, pour toute fonction $ h \geq 0 $ de $ \mathcal{H}(U) $, on a
$$
\int h d\lambda_{J, U} = \int h g_J d\mu \leq \int_K^{*} (q \circ f) h d\mu \leq \|h\| \int_U^{*} (q \circ f) d\mu
$$
d'où notre assertion (chap. II, § 2, no 2). Soit $ \nu_U $ la borne supérieure de cette famille de mesures dans $ \mathcal{M}(U) $. Si $ U' $ est une seconde partie ouverte relativement compacte de $ T $ telle que $ U \subset U' $, $ \nu_U $ est la restriction de $ \nu_{U'} $ à $ U $, comme il résulte aussitôt de l'expression de la borne supérieure d'un ensemble filtrant croissant de mesures (chap. II, § 2, no 2) et du fait que $ \lambda_{J, U} $ est la restriction à $ U $ de $ \lambda_{J, U'} $. Il y a donc une mesure positive $ \nu $ et une seule dont la restriction à chacun des $ U $ soit $ \nu_U $ (chap. III, § 3, no 1, prop. 1), et il est clair que $ \nu = q(m) $.

b) Comme les mesures $ \lambda_J $ sont de base $ \mu $, il en est de même de leur borne supérieure $ q(m) $ (chap. V, § 5, no 5, th. 2). Si $ f $ est $ \mu $-mesurable pour la topologie $ \sigma(F, F') $ sur $ F $, il résulte aussitôt des définitions que l'application $ t \to (g_J(t))_{J \in \mathfrak{F}} $ de $ T $ dans l'espace produit $ \mathbf{R}^{\mathfrak{F}} $ est $ \mu $-mesurable ; comme la famille $ (g_J) $ est filtrante croissante, $ q \circ f = \sup_{J \in \mathfrak{F}} g_J $ est $ \mu $-mesurable, et pour toute partie compacte $ K $ de $ T $, on a
$$
\int_K^{*} (q \circ f) d\mu = \sup_J \int_K g_J d\mu \leq \int_K dq(m)
$$

(chap. V, § 2, no 2, prop. 9). Mais cela prouve que $ q \circ f $ est localement $ \mu $-intégrable et que $ \lambda_J \leq (q \circ f) \cdot \mu \leq q(m) $ pour tout $ J \in \mathcal{F} $; d’où, par définition, $ q(m) = (q \circ f) \cdot \mu $.

#### Remarque {#int-vi-s2-n4-rem-1 .statement}

Supposons qu’il existe dans $ A_q' $ un ensemble dénombrable $ D $ dense pour $ \sigma(F', F) $; alors la fonction $ q \circ f $ est toujours $ \mu $-mesurable, car on a $ q(f(t)) = \sup_{z' \in D} |\langle z', f(t) \rangle| $ (chap. IV, § 5, no 4, cor. 1 du th. 2). On a alors, pour toute partie compacte $ K $ de $ T $,
$$
\int_K^* (q \circ f) d\mu = \sup_J \int_K g_J d\mu
$$
où $ J $ parcourt l’ensemble filtrant dénombrable des parties finies de $ D $ (chap. IV, § 1, no 1, cor. du th. 3); on voit donc que dans ce cas la condition $ \int_K^* (q \circ f) d\mu < +\infty $ pour toute partie compacte $ K $ de $ T $ est nécessaire et suffisante pour que $ m $ soit $ q $-majorable.

#### Proposition 9 {#int-vi-s2-prop-9 .statement}

Soit $ F $ un espace de Banach de dimension finie. Toute mesure $ m $ sur $ T $ à valeurs dans $ F $ est une mesure de base $ |m| $. Si $ m = f.|m| $, on a $ |f(t)| = 1 $ localement presque partout pour $ |m| $. Pour que $ m $ soit de base $ \mu $, il faut et il suffit que $ |m| $ soit de base $ \mu $, et si $ m = g.\mu $, on a $ |m| = |g|.\mu $.

Soient $ (e_i)_{1 \leq i \leq n} $ une base de $ F $ et $ (e'_i)_{1 \leq i \leq n} $ la base duale de $ F' $. Pour tout indice $ i $, on a $ |e'_i \circ m| \leq |m| $, donc (chap. V, § 5, no 5, th. 2) $ e'_i \circ m = h_i.|m| $, où $ h_i $ est bornée et $ |m| $-mesurable. Si on pose $ h = \sum_{i=1}^n h_i e_i $, on a donc $ m = h.|m| $. Si $ m = f.|m| $, la prop. 8 montre que $ |m| = |f|.|m| $, d’où $ |f(t)| = 1 $ localement presque partout pour $ |m| $ (chap. V, § 5, no 4, cor. 2 de la prop. 5). La dernière assertion résulte aussitôt de la prop. 8.

#### Remarque {#int-vi-s2-n4-rem-2 .statement}

Si $ z = \sum_{i=1}^n z_i e_i $, $ |z| = \psi(z_1, \ldots, z_n) $ est une fonction continue positivement homogène dans $ \mathbf{R}^n $. Si on pose $ \mu_i = e'_i \circ m = h_i.|m| $, on a, par définition (chap. V, § 5, no 9),
$$
\psi(\mu_1, \ldots, \mu_n) = \psi(h_1, \ldots, h_n).|m| = |h|.|m| = |m|.
$$

### 5. Le théorème de Dunford-Pettis.

Soit $ \mu $ une mesure positive sur T. On dit qu'une mesure vectorielle $ m $ sur T, à valeurs dans F, est scalairement de base $ \mu $ si, pour tout $ z' \in F' $, la mesure scalaire $ z' \circ m $ est de base $ \mu $. Si une mesure vectorielle $ m $ à valeurs dans F est de base $ \mu $, elle est scalairement de base $ \mu $ : en effet, si $ m = f \cdot \mu $, on a $ z' \circ m = \langle z', f \rangle \cdot \mu $ pour tout $ z' \in F' $. Mais il existe des mesures vectorielles qui sont scalairement de base $ \mu $ sans être de base $ \mu $ (exerc. 17), et d'autre part il existe des mesures vectorielles qui ne sont scalairement de base $ \nu $ pour aucune mesure positive $ \nu $; on notera toutefois que toute mesure $ m $ majorable à valeurs dans un espace normé est scalairement de base $ |m| $, en vertu du th. de Lebesgue-Nikodym.

#### Exemple {#int-vi-s2-n5-exa-1 .statement}

Prenons pour $ m $ l’application identique de $ \mathcal{K}(T) $. Dire que $ m $ est scalairement de base $ \mu $ signifie que toute mesure réelle sur T est de base $ \mu $. En particulier, la mesure ponctuelle $ \varepsilon_t (t \in T) $ doit être de base $ \mu $, ce qui exige que $ \mu(\{t\}) > 0 $ pour tout $ t \in T $, et entraîne en particulier que toute partie compacte de T est dénombrable.

Nous allons dans ce no démontrer un résultat qui généralise une des conséquences du th. de Lebesgue-Nikodym, à savoir que le dual de $ L^1(\mu) $ est $ L^\infty(\mu) $ (chap. V, § 5, no 8, th. 4), et qui donne une condition suffisante pour qu’une mesure vectorielle scalairement de base $ \mu $ soit de base $ \mu $.

Soit $ \pi $ l’application canonique de $ \mathcal{L}^\infty(\mu) $ sur $ L^\infty(\mu) $. Nous dirons qu’un sous-espace vectoriel G de $ L^\infty $ possède la propriété de relèvement s’il existe une application linéaire $ \rho $ de G dans $ \mathcal{L}^\infty(\mu) $ (dite relèvement de G) telle que $ \pi \circ \rho $ soit l’identité sur G et que $ |\rho(f)(t)| \leq N_\infty(f) $ pour tout $ t \in T $ et tout $ f \in G $.

On démontre que si $ \mu $ est la mesure de Lebesgue sur $ \mathbf{R}^n $, l’espace $ L^\infty(\mathbf{R}^n, \mu) $ tout entier possède la propriété de relèvement (exerc. 18).

#### Lemme 2 {#int-vi-s2-lem-2 .statement}

Tout sous-espace G de type dénombrable de l’espace de Banach $ L^\infty(T, \mu) $ possède la propriété de relèvement.

Par hypothèse il existe une partie dénombrable dense H de G, qui soit un sous-espace vectoriel sur le corps $ \mathbf{Q} $ des nombres rationnels ; soit $ (h_n) $ une base (dénombrable) de $ H $ sur $ \mathbf{Q} $. Pour tout entier $ n $, soit $ h'_n $ un élément de $ \mathcal{L}^\infty $ tel que $ \pi(h'_n) = h_n $, et soit $ \rho' $ l’application $ \mathbf{Q} $-linéaire de $ H $ dans $ \mathcal{L}^\infty $ définie par $ \rho'(h_n) = h'_n $; il est clair que $ \pi \circ \rho $ est l’identité sur $ H $. En outre, pour tout $ h \in H $, on a $ |\rho'(h)(t)| \leq N_\infty(h) $ sauf aux points $ t $ d’un ensemble localement négligeable $ A(h) $. Soit $ A $ la réunion des $ A(h) $ pour $ h \in H $, qui est encore localement négligeable. Pour tout $ h \in H $, désignons par $ \rho(h) $ la fonction $ h'' \in \mathcal{L}^\infty $ telle que $ h''(t) = \rho'(h)(t) $ si $ t \notin A $ et $ h''(t) = 0 $ si $ t \in A $. Il est clair que $ \rho $ est une application $ \mathbf{Q} $-linéaire de $ H $ dans $ \mathcal{L}^\infty $, telle que $ \pi \circ \rho $ soit l’identité sur $ H $ et que $ |\rho(h)(t)| \leq N_\infty(h) $ pour tout $ h \in H $ et tout $ t \in T $. Comme $ \mathcal{L}^\infty $ est un espace de Banach pour la norme $ \|f\| = \sup_{t \in T} |f(t)| $ (chap. IV, § 5, no 4, th. 2), $ \rho $ se prolonge en une application $ \mathbf{R} $-linéaire continue, notée encore $ \rho $, de $ G $ dans $ \mathcal{L}^\infty $, qui est évidemment un relèvement de $ G $.

#### Définition 5 {#int-vi-s2-def-5 .statement}

Soient $ F $ un espace localement convexe séparé, $ F'_s $ son dual muni de la topologie $ \sigma(F', F) $. On désigne par $ \mathcal{L}_{F'_s}^\infty $ l’espace vectoriel des applications $ f $ de $ T $ dans $ F'_s $, telles que $ f $ soit scalairement $ \mu $-mesurable et égale scalairement localement presque partout (pour $ \mu $) à une application de $ T $ dans une partie équicontinue de $ F' $. On désigne par $ L_{F'_s}^\infty $ l’espace quotient de $ \mathcal{L}_{F'_s}^\infty $ par l’espace des applications scalairement localement $ \mu $-négligeables de $ T $ dans $ F'_s $.

Lorsque $ F $ vérifie les hypothèses du § 1, no 5, prop. 13, les fonctions de $ \mathcal{L}_{F'_s}^\infty $ sont $ \mu $-mesurables pour la topologie faible $ \sigma(F', F) $, mais ne sont pas nécessairement mesurables pour la topologie forte sur $ F' $, même si $ F $ est un espace de Banach ($ \S 1 $, exerc. 17). Dans les mêmes conditions, les applications scalairement localement $ \mu $-négligeables de $ T $ dans $ F'_s $ sont identiques aux applications localement $ \mu $-négligeables de $ T $ dans $ F'_s $ ($ \S 1 $, no 1, Remarque 2).

Lorsque $ F $ est un espace normé de type dénombrable, les éléments de $ \mathcal{L}_{F'_s}^\infty $ sont les applications $ f $ de $ T $ dans $ F'_s $, telles que $ f $ soit scalairement $ \mu $-mesurable et que $ |f| $ soit bornée en mesure ; on peut alors définir sur l’espace $ L_{F'_s}^\infty $ une structure d’espace normé, en le munissant de la norme $ N_\infty $ (chap. IV, § 6, no 3).

#### Lemme 3 {#int-vi-s2-lem-3 .statement}

Soient F un espace localement convexe séparé, f un élément de $ \mathcal{L}_{\mathbf{F}_s}^\infty $. Pour tout $ z \in F $, on a $ \langle z, f \rangle \in \mathcal{L}^\infty $, et l’application linéaire $ z \to \pi(\langle z, f \rangle) $ de F dans $ L^\infty $ est continue ; si en outre F est un espace normé, on a $ N_\infty(\langle z, f \rangle) \leq |z| \cdot \sup_{t \in T} |f(t)| $.

Il est clair par définition que $ \langle z, f \rangle $ est $ \mu $-mesurable et bornée en mesure ; en remplaçant éventuellement f par une fonction appartenant à la même classe de $ \mathcal{L}_{\mathbf{F}_s}^\infty $, on peut supposer en outre que $ f(T) \subset V^0 $, où V est un voisinage convexe équilibré de 0 dans F (ce qui ne modifie $ \langle z, f \rangle $ que sur un ensemble localement négligeable, dépendant de z). Alors la relation $ z \in V $ entraîne $ |\langle z, f(t) \rangle| \leq 1 $ pour tout $ t \in T $, ce qui prouve la continuité de $ z \to \pi(\langle z, f \rangle) $. La dernière assertion est évidente.

#### Lemme 4 {#int-vi-s2-lem-4 .statement}

Soient F un espace localement convexe séparé, f un élément de $ \mathcal{L}_{\mathbf{F}_s}^\infty $. Pour toute fonction numérique $ g \in \bar{\mathcal{L}}^1 $, la fonction gf est scalairement essentiellement $ \mu $-intégrable et l’on a $ \int gf d\mu \in F' $.

En effet, pour tout $ z \in F $, $ \langle z, f \rangle $ appartient à $ \mathcal{L}^\infty $, d’où la première assertion. En outre, on peut supposer, sans modifier $ \int gf d\mu $, que $ f(T) \subset V^0 $, où V est un voisinage convexe équilibré de 0 dans F. Alors la relation $ z \in V $ entraîne $ |\langle z, f(t) \rangle| \leq 1 $ pour tout $ t \in T $, d’où $ |\langle z, \int gf d\mu \rangle| = \left| \int \langle z, f \rangle g d\mu \right| \leq \overline{N}_1(g) $, ce qui prouve que $ \int gf d\mu \in F' $.

#### Théorème 1 {#int-vi-s2-thm-1 .statement}

Soit F un espace localement convexe séparé, contenant une partie dénombrable partout dense. Pour toute fonction $ f \in \mathcal{L}_{\mathbf{F}_s}^\infty $ et tout $ z \in F $, soit $ v_1(z) = \pi(\langle z, f \rangle) \in L^\infty $ ; l’application $ f \to v_1 $ définit, par passage au quotient, une bijection linéaire de $ \mathcal{L}_{\mathbf{F}_s}^\infty $ sur l’espace $ \mathcal{L}(F; L^\infty) $ des applications linéaires continues de F dans $ L^\infty $. Si F est un espace normé, cette bijection est une isométrie.

Vu le lemme 3, la première assertion sera démontrée si l’on prouve que pour toute application continue u de F dans $ L^\infty $, il existe une fonction $ f \in \mathcal{L}_{\mathbf{F}_s}^\infty $, telle que $ \pi(\langle z, f \rangle) = u(z) $ pour tout z \in F, et que la classe de f dans L_{F_s}^\infty est déterminée de façon unique par cette condition. Le second point est immédiat, car si $ \pi(\langle z, f \rangle) = \pi(\langle z, f_1 \rangle) $ pour tout $ z \in F, f_1 - f $ est scalairement localement négligeable. D'autre part, il existe un relèvement $ \varphi $ de $ u(F) $ dans $ \mathcal{L}^\infty $ (lemme 2). Pour tout $ t \in T $, l'application $ z \to \varphi(u(z))(t) $ est une forme linéaire continue sur $ F $, c'est-à-dire un élément $ f(t) $ de $ F' $. La fonction $ f $ est scalairement $ \mu $-mesurable puisque $ \langle z, f \rangle = \varphi(u(z)) \in \mathcal{L}^\infty $ pour tout $ z \in F $; on a $ \pi(\langle z, f \rangle) = u(z) $; enfin, pour tout $ t \in T $ et tout $ z $ appartenant à l'image réciproque $ V $ par $ u $ de la boule unité de $ L^\infty $, on a

$$
|\langle z, f(t) \rangle| = |\varphi(u(z))(t)| \leq N_\infty(u(z)) \leq 1
$$

ce qui montre que $ f(t) \in V^0 $ pour tout $ t \in T $.

Si de plus $ F $ est un espace normé, ce qui précède montre que $ \sup_{t \in T} |f(t)| \leq \|u\| $. Mais d'autre part (lemme 3), on a

$$
N_\infty(u(z)) \leq |z| \cdot \sup_{t \in T} |f(t)|
$$

et cette inégalité subsiste lorsqu'on modifie arbitrairement $ f $ dans un ensemble localement négligeable. On en conclut que $ \|u\| = N_\infty(|f|) $.

#### Corollaire 1 {#int-vi-s2-thm-1-cor-1 .statement}

Soit $ F $ un espace localement convexe séparé contenant une partie dénombrable partout dense. Pour toute fonction $ f \in \mathcal{L}_{F_s}^\infty $, tout $ z \in F $ et toute fonction $ g \in \mathcal{L}^1 $, soit $ \Phi_f(z, \tilde{g}) = \int \langle z, f(t) \rangle g(t) d\mu(t) $. L'application $ f \to \Phi_f $ définit, par passage au quotient, une bijection linéaire de $ L_{F_s}^\infty $ sur l'espace $ \mathcal{B}(F, L^1) $ des formes bilinéaires continues dans $ F \times L^1 $. Si $ F $ est un espace normé, cette bijection est une isométrie.

En effet, on peut supposer que $ f(T) $ est une partie équicontinue de $ F' $. Il est clair alors que $ \Phi_f $ est séparément continue, et avec les notations du th. 1 et de l'Appendice, on a (compte tenu de ce que $ L^\infty $ est le dual de $ L^1 $ (chap. V, § 5, no 8, th. 4)) $ ^t\Phi_f = v_f $. Le corollaire résulte alors du th. 1 ci-dessus et de l'Appendice, no 1, prop. 1 et corollaire.

#### Corollaire 2 (théorème de Dunford-Pettis) {#int-vi-s2-thm-1-cor-2 .statement}

Soit F un espace localement convexe séparé contenant une partie dénombrable partout dense. Pour toute fonction $ f \in \mathcal{L}_{\mathbf{F}_s}^\infty $, et toute fonction $ g \in \mathcal{L}^1 $, soit $ \omega_f(\tilde{g}) = \int g f d\mu \in F' $ (lemme 4). L’application $ f \to \omega_f $ définit, par passage au quotient, une bijection linéaire de $ \mathcal{L}_{\mathbf{F}_s}^\infty $ sur l’espace $ \mathcal{R}(L^1, F') $ des applications linéaires $ u $ de $ L^1 $ dans $ F' $ telles que l’image par $ u $ de la boule unité de $ L^1 $ soit une partie équicontinue de $ F' $. Si F est un espace normé (auquel cas $ \mathcal{R}(L^1, F') $ est l’espace des applications linéaires continues de $ L^1 $ dans le dual fort de $ F $), la bijection $ f \to \omega_f $ est une isométrie.

Compte tenu de ce que $ L^\infty $ est le dual de $ L^1 $, cela résulte du corollaire précédent et de l’Appendice, n° 1, prop. 1 et corollaire.

#### Remarque {#int-vi-s2-n5-rem-1 .statement}

Il est clair que les applications $ u \in \mathcal{R}(L^1, F') $ sont continues pour toute $ \mathcal{S}$-topologie sur $ F' $ ($ \mathcal{S} $ recouvrement de F par des parties bornées). Réciproquement, si on suppose en outre F tonnelé, toute application linéaire continue de $ L^1 $ dans $ F' $ muni d’une $ \mathcal{S}$-topologie transforme la boule unité de $ L^1 $ en une partie bornée de $ F' $, qui est par suite équicontinue (*Esp. vect. top.*, chap. III, § 3, n° 6, th. 2).

#### Corollaire 3 {#int-vi-s2-thm-1-cor-3 .statement}

Soient F un espace localement convexe séparé contenant une partie dénombrable partout dense, m une mesure vectorielle sur T à valeurs dans le dual faible $ F' $ de F. Si l’image par m de l’ensemble B des fonctions g de $ \mathcal{K}(T) $ telles que $ \mu(|g|) \leq 1 $ est contenu dans une partie équicontinue convexe et fermée $ H' $ de $ F' $, alors m est de base $ \mu $ et il existe une densité f de m par rapport à $ \mu $ telle que $ f(t) \in H' $ pour tout $ t \in T $.

L’hypothèse entraîne que m est continue lorsqu’on munit $ \mathcal{K}(T) $ de la topologie induite par celle de $ \mathcal{L}^1(\mu) $ (définie par la semi-norme $ N_1 $) ; elle se prolonge donc en une application linéaire continue $ u $ de $ \mathcal{L}^1(\mu) $ dans le complété G du dual faible de F ; mais comme $ H' $ est une partie compacte de G et que l’image par $ u $ de l’ensemble B des $ f \in \mathcal{L}^1 $ tels que $ N_1(f) \leq 1 $ est contenue dans l’adhérence de $ H' $ dans G, on a $ u(B) \subset H' $, donc $ u $ applique $ \mathcal{L}^1 $ dans $ F' $. Comme la relation $ N_1(f) \leq \varepsilon $ entraîne $ u(f) \in \varepsilon H' $, on a $ u(g) = 0 $ si $ g $ est $ \mu $-négligeable, et on peut donc appliquer le cor. 2 à l’application de $ L^1 $ dans F' obtenue par passage au quotient à partir de u ; d'où le corollaire.

#### Corollaire 4 {#int-vi-s2-thm-1-cor-4 .statement}

Soient F un espace normé de type dénombrable, m une mesure sur T à valeurs dans le dual fort F', majo-
rable pour la norme de F'. Alors m est une mesure de base |m|, et si m = f.|m|, on a |f(t)| = 1 localement presque partout pour |m|.
En effet, par hypothèse, pour tout z ∈ F tel que |z| ≤ 1, on a
|\langle z, m(g) \rangle| \leq |m|(|g|) pour toute fonction g ∈ J(T), et par suite
|m(g)| \leq |m|(|g|) (Esp. vect. top., chap. IV, § 5, n° 2, prop. 4).
Comme toute boule dans F' est équicontinue, le cor. 3 s'applique et montre que m est de base |m| ; en outre, si m = f.|m|, f est |m|-mesurable pour σ(F', F) (§ 1, n° 5, prop. 13), et on a
|m| = |f|.|m| (n° 4, prop. 8), ce qui démontre le corollaire (chap. V, § 5, n° 4, cor. 2 de la prop. 5).

Si on applique ce corollaire au cas où F est de dimension finie, on retrouve comme cas particulier la première partie de la prop. 9.

### 6. Dual de l'espace $ L^1_F $ (F espace de Banach de type dénombrable).

#### Proposition 10 {#int-vi-s2-prop-10 .statement}

Soit F un espace de Banach de type dénombrable. Pour toute fonction $ f \in \overline{\mathcal{L}}^1_F $ et toute fonction $ g \in \mathcal{L}^\infty_{F_s'} $, la fonction numérique $ \langle f, g \rangle : t \to \langle f(t), g(t) \rangle $ est essentiellement µ-intégrable et on a
$$
\left| \int \langle f, g \rangle \, d\mu \right| \leq \overline{N}_1(f) N_\infty(g).
$$
Pour toute classe $ \dot{g} \in \mathcal{L}^\infty_{F_s'} $, soit $ \theta(\dot{g}) $ la forme linéaire continue sur $ L^1_F $ déduite par passage au quotient de la forme linéaire $ f \to \int \langle f, g \rangle \, d\mu $ sur $ \overline{\mathcal{L}}^1_F $; alors $ \theta $ est une isométrie linéaire de $ L^\infty_{F_s'} $, sur le dual fort $ (L^1_F)' $ de l'espace de Banach $ L^1_F $.

Pour toute partie compacte K de T et tout $ \varepsilon > 0 $, il existe une partie compacte K' de K telle que $ \mu(K - K') \leq \varepsilon $ et que la restriction de f (resp. g) à K' soit une application continue de K' dans F (resp. dans $ F_s' $) ; par suite $ g(K') $ est faiblement compact, donc équicontinu dans F' (Esp. vect. top., chap. IV, § 5, n° 1). Or, la restriction de la forme bilinéaire canonique sur F × F' au produit de F et d'une partie équicontinue de F' est continue pour la topologie produit de la topologie de F et de σ(F', F) (Top. gén., chap. X, 2e éd., § 2, n° 2, cor. 4 de la prop. 1); on en conclut que la restriction de $ \langle f, g \rangle $ à K' est continue, et par suite que $ \langle f, g \rangle $ est $ \mu $-mesurable. De plus, on a

$$
|\langle f(t), g(t) \rangle| \leq |f(t)| \cdot |g(t)| \leq |f(t)| N_\infty(g)
$$

localement presque partout, et par suite $ \langle f, g \rangle $ est essentiellement $ \mu $-intégrable et on a l'inégalité (3) (chap. IV, § 5, n° 6, th. 5 et chap. V, § 2, n° 2, prop. 5).

Reste à montrer que $ \theta $ est une isométrie surjective. Soit $ u $ une forme linéaire continue sur $ L^1_F $. L'application $ (\tilde{h}, z) \to u(\tilde{h}z) $ est une forme bilinéaire continue sur $ L^1 \times F $, car

$$
|u(\tilde{h}z)| \leq \|u\| \cdot N_1(hz) \leq \|u\| \cdot |z| \cdot N_1(h).
$$

D'après le cor. 1 du th. 1 du n° 5, il existe une application g de T dans F', appartenant à $ L^\infty_{F'} $, telle que $ |g(t)| \leq \|u\| $ pour tout $ t \in T $, et que $ u(\tilde{h}z) = \int \langle hz, g \rangle d\mu $ pour toute fonction $ h \in \mathcal{L}^1 $ de classe $ \tilde{h} $ dans $ L^1 $, et tout $ z \in F $. Autrement dit, les formes linéaires $ u $ et $ \theta(\dot{g}) $ coïncident sur le sous-espace de $ L^1_F $ engendré par les éléments de la forme $ \tilde{h}z $ ($ \tilde{h} \in L^1, z \in F $). Comme ce sous-espace est dense dans $ L^1_F $ (chap. IV, § 3, n° 5, prop. 10), on a donc $ u = \theta(\dot{g}) $, ce qui prouve déjà que $ \theta $ est surjective. On a en outre d'après (3) $ \|\theta(\dot{g})\| \leq N_\infty(g) \leq \|u\| = \|\theta(\dot{g})\| $, d'où $ \|\theta(\dot{g})\| = N_\infty(g) $, et ceci termine la démonstration.

### 7. Intégration d'une fonction vectorielle par rapport à une mesure vectorielle.

#### Proposition 11 {#int-vi-s2-prop-11 .statement}

Soient F, G, H trois espaces de Banach, $ \Phi $ une application bilinéaire continue de $ F \times G $ dans H. Soit m une mesure vectorielle majorable sur T, à valeurs dans G. Il existe alors une application linéaire continue et une seule $ I_{\Phi, m} $ de $ \bar{\varphi}_F^1(|m|) $ dans

H telle que, pour tout $ z \in F $ et pour toute fonction numérique $ h $ intégrable pour $ |\mathbf{m}| $, on ait $ I_{\Phi, \mathbf{m}}(hz) = \Phi\left(z, \int h d\mathbf{m}\right) $. En outre, on a

$$
|I_{\Phi, \mathbf{m}}(\mathbf{f})| \leq \| \Phi \| \int |\mathbf{f}| d|\mathbf{m}|,
$$

pour toute fonction $ \mathbf{f} \in \mathcal{L}_F^1(|\mathbf{m}|) $.

S’il existe une telle application, sa valeur pour une fonction étagée $ \mathbf{f} $ sur les ensembles $ |\mathbf{m}| $-intégrables est bien déterminée : on sait en effet qu’on peut écrire alors $ \mathbf{f} = \sum_i a_i \varphi_{X_i} $, où les $ X_i $ sont $ |\mathbf{m}| $-intégrables et disjoints, et les $ a_i \in F $ (chap. IV, § 4, no 8, lemme 1). La valeur de $ I_{\Phi, \mathbf{m}}(\mathbf{f}) $ doit donc être égale à $ \sum_i \Phi(a_i, \int \varphi_{X_i} d\mathbf{m}) $. Or, on a (no 3, prop. 6)

$$
|\sum_i \Phi(a_i, \int \varphi_{X_i} d\mathbf{m})| \leq \| \Phi \| \cdot \sum_i |a_i| \cdot |\mathbf{m}|(X_i) = \| \Phi \| \int |\mathbf{f}| d|\mathbf{m}|,
$$

ce qui montre d’abord que l’élément $ \sum_i \Phi(a_i, \int \varphi_{X_i} d\mathbf{m}) $ de $ H $ ne dépend pas de l’expression de $ \mathbf{f} $ sous la forme $ \sum_i a_i \varphi_{X_i} $, et par suite qu’on peut l’écrire $ I_{\Phi, \mathbf{m}}(\mathbf{f}) $. On vérifie aussitôt que l’application $ I_{\Phi, \mathbf{m}} $ ainsi définie est linéaire dans l’espace $ \mathcal{E}_F $ des fonctions étagées sur les ensembles $ |\mathbf{m}| $-intégrables : il suffit en effet d’écrire deux fonctions $ \mathbf{f}, g $ de $ \mathcal{E}_F $ sous la forme $ \mathbf{f} = \sum_i a_i \varphi_{X_i} $ et $ g = \sum_i b_i \varphi_{X_i} $ pour la même famille finie d’ensembles $ |\mathbf{m}| $-intégrables $ X_i $, deux à deux disjoints (ce qui est possible en vertu du lemme 1 du chap. IV, § 4, no 8). L’inégalité (5) montre alors que $ I_{\Phi, \mathbf{m}} $ est continue dans $ \mathcal{E}_F $, et comme ce sous-espace est partout dense dans $ \mathcal{L}_F^1 $ (chap. IV, § 4, no 9, cor. 1 de la prop. 16 et chap. V, § 2, no 2, prop. 6), on en déduit l’existence et l’unicité de $ I_{\Phi, \mathbf{m}} $ ainsi que l’inégalité (4).

On dit que $ I_{\Phi, \mathbf{m}}(\mathbf{f}) $ est l’intégrale de $ \mathbf{f} $ par rapport à $ \mathbf{m} $ (relativement à l’application bilinéaire $ \Phi $) ; lorsque l’on note $ xy $ la valeur de l’application bilinéaire $ \Phi $ au point $ (x, y) $, on écrira $ \int \mathbf{f} d\mathbf{m} $ au lieu de $ I_{\Phi, \mathbf{m}}(\mathbf{f}) $.

Bourbaki XXV.

Avec les notations du no 6, l'intégrale $ \int \langle f, g \rangle d\mu $ n'est autre que $ I_{\Phi, m}(f) $ avec $ \Phi(x, x') = \langle x, x' \rangle $ et $ m = g.\mu $.

#### Corollaire {#int-vi-s2-n7-cor-1 .statement}

*Si* $ m $ et $ m' $ sont deux mesures majorables sur $ T $, à valeurs dans $ G $, *on a* $ I_{\Phi, m + m'} = I_{\Phi, m} + I_{\Phi, m'} $ et $ I_{\Phi, \lambda m} = \lambda I_{\Phi, m} $ pour tout scalaire $ \lambda $.

La seconde assertion est immédiate. La première signifie que pour toute fonction $ f $ qui est à la fois $ |m| $-intégrable et $ |m'| $-intégrable, on a
$$
I_{\Phi, m + m'}(f) = I_{\Phi, m}(f) + I_{\Phi, m'}(f).
$$
La fonction $ f $ est alors ($ |m| + |m'| $)-intégrable (chap. V, § 3, prop. 6 et cor. 1), donc *a fortiori* ($ |m + m'| $)-intégrable, et le premier membre de (6) a bien un sens. Pour démontrer (6), il suffit de le faire lorsque $ f $ est une fonction étagée sur les ensembles ($ |m| + |m'| $)-intégrables, l'ensemble de ces fonctions étant dense dans $ \mathcal{L}_F^1(|m| + |m'|) $ et les deux membres de (6) étant continus dans ce dernier espace, en vertu de (4). Mais pour $ f = a \varphi_X $, où $ X $ est ($ |m| + |m'| $)-intégrable, les deux membres de (6) se réduisent à $ \Phi(a, \int \varphi_X dm) + \Phi(a, \int \varphi_X dm') $, d'où le corollaire.

#### Remarque {#int-vi-s2-n7-rem-1 .statement}

Lorsque $ m $ est de la forme $ b\mu $, où $ b \in G $ et $ \mu $ est une mesure réelle sur $ T $, on a
$$
I_{\Phi, m}(f) = \int \Phi(f(t), b) d\mu(t)
$$
pour toute fonction $ f \in \mathcal{L}_F^1(\mu) $, car les deux membres sont continus dans cet espace et coïncident lorsque $ f $ est étagée sur les ensembles $ |\mu| $-intégrables.

### 8. Mesures complexes.

#### Définition 5 {#int-vi-s2-def-5-bis .statement}

*On appelle mesure complexe sur* $ T $ *toute forme linéaire continue sur l'espace vectoriel complexe* $ \mathcal{K}_c(T) $.

L'espace $ \mathcal{M}_c(T) $ des mesures complexes sur $ T $ est donc le dual de l'espace localement convexe séparé $ \mathcal{J}_c(T) $.

Si $ m $ est une mesure complexe sur $ T $, sa restriction à $ \mathcal{H}(T) $ est une mesure vectorielle sur $ T $ à valeurs dans $ \mathbf{C} $ (considéré comme espace vectoriel sur $ \mathbf{R} $) ; $ m $ est déterminée par cette restriction, puisque si $ f = f_1 + i f_2 \in \mathcal{H}_\mathbf{C}(T) $, la partie réelle $ f_1 $ et la partie imaginaire $ f_2 $ de $ f $ sont dans $ \mathcal{H}(T) $, et $ m(f) = m(f_1) + i m(f_2) $. Inversement, pour toute mesure vectorielle $ m_0 $ sur $ T $ à valeurs dans $ \mathbf{C} $, la formule $ m(f) = m_0(f_1) + i m_0(f_2) $ définit une mesure complexe $ m $ et une seule dont la restriction à $ \mathcal{H}(T) $ soit $ m_0 $. Nous identifierons donc désormais une mesure complexe à sa restriction à $ \mathcal{H}(T) $ ; une telle mesure $ m $ est de la forme $ m = \mu_1 + i \mu_2 $, où $ \mu_1 $ et $ \mu_2 $ sont deux mesures réelles sur $ T $, qui sont appelées respectivement *partie réelle* et *partie imaginaire* de $ m $. Le support de $ m $ est l’adhérence de la réunion des supports de $ \mu_1 $ et $ \mu_2 $. On sait que $ m $ est majorable (no 3, cor. de la prop. 4) ; nous appellerons *valeur absolue* de $ m $ la mesure positive $ |m| $ correspondant à la valeur absolue $ |x_1 + i x_2| = \sqrt{x_1^2 + x_2^2} $ sur $ \mathbf{C} $. On a $ |m| = (\mu_1^2 + \mu_2^2)^{1/2} $ (no 4, Remarque suivant la prop. 9), et $ |\mu_1| \leq |m|,\ |\mu_2| \leq |m|,\ |m| \leq |\mu_1| + |\mu_2| $; en outre, $ m $ est une mesure de base $ |m| $, et on peut écrire $ m = h.|m| $, où $ h \in \mathcal{L}_\mathbf{C}^\infty(|m|) $ et $ |h(t)| = 1 $ localement presque partout pour $ |m| $ (no 4, prop. 9). Les supports de $ m $ et de $ |m| $ sont les mêmes.

Pour toute application $ \mathbf{f} $ de $ T $ dans un espace de Banach complexe $ F $, essentiellement intégrable par rapport à $ |m| $, on peut définir (no 7) l’intégrale de $ \mathbf{f} $ par rapport à $ m $ (correspondant à l’application $ \mathbf{R}$-bilinéaire $ (\mathbf{x}, \lambda) \to \lambda \mathbf{x} $ de $ F \times \mathbf{C} $ dans $ F $), qu’on notera $ \int \mathbf{f} dm $; il résulte aussitôt de la propriété d’unicité de la prop. 11 que l’on a (avec les notations précédentes)
$$
\int \mathbf{f} dm = \int \mathbf{f} d\mu_1 + i \int \mathbf{f} d\mu_2 = \int \mathbf{f} h d|m|.
$$
Pour $ f \in \mathcal{H}_\mathbf{C}(T) $, on a donc $ m(f) = \int f dm $. On dit que $ \mathbf{f} $ est essentiellement intégrable pour $ m $ si elle l’est pour $ |m| $; on définit de même les applications $ m $-intégrables, $ m $-mesurables, localement $ m $-intégrables, $ m $-négligeables, localement $ m $-négligeables. On écrit $ \mathcal{L}_F^p(T, m) $ (resp. $ \overline{\mathcal{L}}_F^p(T, m), L_F^p(T, m) $) au lieu de $ \mathcal{L}_F^p(T, |m|) $ (resp. $ \overline{\mathcal{L}}_F^p(T, |m|), L_F^p(T, |m|) $); ce sont des espaces vectoriels complexes.

Pour que $ \mathbf{f} $ soit $ m $-intégrable (resp. essentiellement $ m $-intégrable), il faut et il suffit que $ \mathbf{f} $ soit intégrable (resp. essentiellement intégrable) par rapport à chacune des quatre mesures $ \mu_1^+, \mu_1^-, \mu_2^+, \mu_2^- $, en vertu des inégalités entre $ |m|, |\mu_1|, |\mu_2| $ et des relations $ |\mu_k| = \mu_k^+ + \mu_k^- (k = 1, 2) $ (chap. V, § 3, no 5, cor. 1 de la prop. 6).

Si $ \mathbf{f} $ est essentiellement $ m $-intégrable (resp. $ m $-intégrable), $ |\mathbf{f}| $ est essentiellement $ |m| $-intégrable (resp. $ |m| $-intégrable), et il résulte de la prop. 11 que

$$
\left| \int \mathbf{f} dm \right| \leq \int |\mathbf{f}| d|m|.
$$

Soient F et G deux espaces de Banach complexes, $ u $ une application linéaire continue de F dans G. Si $ \mathbf{f} $ est une application essentiellement $ m $-intégrable (resp. $ m $-intégrable) de T dans F, $ u \circ \mathbf{f} $ est essentiellement $ m $-intégrable (resp. $ m $-intégrable) et on a
$$
\int (u \circ \mathbf{f}) dm = u \left( \int \mathbf{f} dm \right);
$$
cela résulte aussitôt de ce qui précède et de la proposition analogue pour les fonctions essentiellement $ |m| $-intégrables (chap. IV, § 4, no 2, th. 1 et chap. V, § 2, no 2, prop. 5).

Soient $ m $ une mesure complexe sur T et $ h $ une fonction complexe localement $ m $-intégrable. Pour toute fonction $ f \in \mathcal{H}_c(T) $, la fonction $ fh $ est $ m $-intégrable et l’application $ f \to \int fh dm $ est une mesure complexe notée $ h.m $ et appelée mesure de densité $ h $ par rapport à $ m $. Si $ m = g.|m| $, il est clair que $ h.m = hg.|m| $; comme en outre $ |g(t)| = 1 $ localement presque partout pour $ |m| $, pour que $ \mathbf{f} $ soit essentiellement intégrable pour $ n = h.m $, il faut et il suffit que $ \mathbf{f}h $ soit essentiellement $ m $-intégrable, et on a
$$
\int \mathbf{f} dn = \int (\mathbf{f}h) dm.
$$
De plus, on a $ |h.m| = |h|.|m| $. On dit encore que toute mesure de la forme $ h.m $ est une mesure complexe de base $ m $; deux mesures complexes $ m, m' $ sont dites équivalentes si chacune a une densité par rapport à l’autre, ou, ce qui revient au même, si $ m' = h.m $, où $ h $ est localement $ m $-intégrable et $ h(t) \neq 0 $ localement presque partout pour $ |m| $. Il est clair que $ m $ et $ |m| $ sont équivalentes, et que, pour que $ m $ et $ m' $ soient équivalentes, il faut et il suffit que $ |m| $ et $ |m'| $ le soient.

Si $ m $ et $ m' $ sont deux mesures complexes sur $ T $, $ f $ une fonction à valeurs dans un espace de Banach complexe $ F $, essentiellement intégrable (resp. intégrable) à la fois pour $ m $ et $ m' $, alors, quels que soient les nombres complexes $ \lambda $ et $ \lambda' $, $ f $ est essentiellement intégrable (resp. intégrable) pour $ \lambda m + \lambda' m' $, et on a

$$
\int f d(\lambda m + \lambda' m') = \lambda \int f dm + \lambda' \int f dm'.
$$

Cela résulte en effet du cor. de la prop. 11 du no 7.

Il résulte en outre des définitions que l’on a

$$
|\lambda m + \lambda' m'| \leq |\lambda| \cdot |m| + |\lambda'| \cdot |m'|.
$$

On appelle mesure conjuguée d’une mesure complexe $ m $ la mesure complexe $ m $ définie par $ \overline{m}(f) = \overline{m(f)} $ pour $ f \in \mathcal{K}_c(T) $. Si $ m = \mu_1 + i \mu_2 $, où $ \mu_1 $ et $ \mu_2 $ sont des mesures réelles, on a $ \overline{m} = \mu_1 - i \mu_2 $ et $ |\overline{m}| = |m| $; si $ m = h \cdot |m| $, on a $ \overline{m} = \overline{h} \cdot |m| $. Si $ f $ est une fonction essentiellement $ m $-intégrable (resp. $ m $-intégrable) à valeurs complexes, $ \overline{f} $ est essentiellement $ \overline{m} $-intégrable (resp. $ \overline{m} $-intégrable) et on a

$$
\int \overline{f} d\overline{m} = \int \overline{f} dm.
$$

#### Proposition 12 {#int-vi-s2-prop-12 .statement}

Soient $ m $ une mesure complexe sur $ T $, $ p $ et $ q $ des exposants conjugués (chap. IV, § 6, no 4). La forme bilinéaire $ (f, g) \to \int fg dm $ est définie et continue dans le produit $ \mathcal{L}_c^p(m) \times \mathcal{L}_c^q(m) $; on a $ \left| \int fg dm \right| \leq N_p(f) N_q(g) $, et $ N_q(g) $ est la norme de la forme linéaire continue sur $ L_c^p(m) $, déduite par passage au quotient de la forme linéaire $ f \to \int fg dm $.

En outre, si $ 1 \leq p < +\infty $, toute forme linéaire continue sur l’espace vectoriel complexe $ \mathcal{L}_c^p(m) $ est du type $ f \to \int fg dm $, où $ g $ est une fonction de $ \mathcal{L}_c^q(m) $, dont la classe dans $ L_c^q(m) $ est bien déterminée.

Comme $ m = h \cdot |m| $, où $ |h(t)| = 1 $ localement presque partout, la première assertion résulte aussitôt de l’inégalité de Hölder (chap. IV, § 6, n° 4, th. 2) ; la seconde découle de la prop. 3 du chap. IV, § 6, n° 4. Enfin, si u est une forme linéaire continue sur $ \mathcal{L}_c^p $, sa restriction au sous-espace (réel) $ \mathcal{L}^p $ de $ \mathcal{L}_c^p $ est une application $ \mathbf{R}$-linéaire continue de $ \mathcal{L}^p $ dans $ \mathbf{C} $; si $ 1 \leq p < +\infty $, elle est donc du type $ f \to \int fg_1 d|m| + i \int fg_2 d|m| $, où $ g_1 $ et $ g_2 $ appartiennent à $ \mathcal{L}^q $ (chap. V, § 5, n° 8, th. 4) ; d’où la dernière assertion en posant $ g = (g_1 + ig_2)h^{-1} $.

### 9. Mesures complexes bornées.

Pour toute mesure complexe $ m $ sur $ T $, on pose
$$
\| m \| = \sup_{\|f\| \leq 1, f \in \mathcal{K}_c(T)} |m(f)|.
$$
On dit que $ m $ est *bornée* si $ \| m \| < +\infty $; il revient au même de dire que $ m $ est continue sur $ \mathcal{K}_c(T) $ muni de la topologie de la convergence uniforme, donc se prolonge en une forme linéaire continue (de norme $ \| m \| $) sur l’espace de Banach $ \overline{\mathcal{J}_c}(T) $ des fonctions continues complexes tendant vers 0 à l’infini.

#### Lemme 5 {#int-vi-s2-lem-5 .statement}

*Soient m une mesure complexe sur T, f une fonction m-intégrable complexe. On a* $ \int |f| d|m| = \sup \left| \int fh dm \right| $, *lorsque h parcourt l’ensemble des fonctions de $ \mathcal{J}_c(T) $ telles que* $ |h(t)| \leq 1 $ *pour tout* $ t \in T $.

Si $ m = g.|m| $, on a $ \int |f| d|m| = \int |fg| d|m| $ et $ \int fh dm = \int fg hd|m| $. Posons $ \zeta(t) = 0 $ lorsque $ f(t)g(t) = 0 $, et
$$
\zeta(t) = f(t)g(t)/|f(t)g(t)|
$$
lorsque $ f(t)g(t) \neq 0 $; $ \zeta $ est $ |m| $-mesurable, et pour tout $ \varepsilon > 0 $, il existe donc une partie compacte K de T telle que $ \int_{T-K} |f| d|m| \leq \varepsilon $, que la restriction de $ \zeta $ à K soit continue et que $ |\zeta(t)| = 1 $ dans K. Il existe donc, en vertu du th. d’Urysohn, une fonction continue $ \zeta_1 $ à valeurs complexes, définie dans T, telle que $ \zeta_1 = \zeta $ dans K et que $ |\zeta_1(t)| \leq 2 $ et $ \zeta_1(t) \neq 0 $ pour tout $ t \in T $; si on pose $ h(t) = \zeta_1(t)/|\zeta_1(t)| $, on voit que $ h $ est continue dans $ T $, coïncide avec $ \zeta $ dans $ K $ et est telle que $ |h(t)| = 1 $ pour tout $ t \in T $. Soit enfin $ u $ une application continue de $ T $ dans $ [0,1] $, égale à 1 dans $ K $ et à support compact ; en posant $ h_1 = h^{-1}u $, on a

$$
\left| \int f h_1 dm - \int |f| d|m| \right| \leq 2 \int_{T-K} |f| d|m| \leq 2 \varepsilon
$$

ce qui démontre le lemme.

#### Proposition 13 {#int-vi-s2-prop-13 .statement}

*Soient m une mesure complexe, et $ \mu = |m| $. Pour que m soit bornée, il faut et il suffit que $ \mu $ soit bornée, et on a alors $ \|m\| = \|\mu\| $.*

On a $ m = g.\mu $, où $ g $ est $ \mu $-mesurable telle que $ |g(t)| = 1 $ pour tout $ t \in T $. Si $ \mu $ est bornée, on a, pour toute fonction $ g \in \mathcal{K}_c(T) $

$$
|m(f)| = \left| \int fg d\mu \right| \leq N_\infty(fg) \|\mu\| = \|f\| \cdot \|\mu\|
$$

donc $ m $ est bornée et $ \|m\| \leq \|\mu\| $. Si $ m $ est bornée, on a, pour toute $ f \in \mathcal{K}_c(T) $, et compte tenu du lemme 5

$$
|\mu(f)| \leq \|f\| \cdot \|m\|
$$

donc $ \mu $ est bornée et $ \|\mu\| \leq \|m\| $. D'où la proposition.

#### Corollaire {#int-vi-s2-n9-cor-1 .statement}

*Soit m une mesure complexe bornée. Toute fonction $ f \in \mathcal{L}_F^\infty(m) $ est alors m-intégrable, et on a* $ \left| \int f dm \right| \leq N_\infty(f) \|m\| $.

En effet, $ f $ est $ m $-mesurable, et en posant $ \mu = |m| $, on a

$$
\int^* |f| d\mu \leq N_\infty(f) \|\mu\| = N_\infty(f) \|m\|
$$

donc $ f $ est $ |m| $-intégrable (chap. IV, § 5, no 6, th. 5) et

$$
\left| \int f dm \right| \leq \int |f| d\mu \leq N_\infty(f) \|m\|.
$$

### 10. Image d'une mesure complexe ; mesure complexe induite ; produit de mesures complexes.

Soit $ m $ une mesure complexe sur $ T $, et soit $ \pi $ une application de $ T $ dans un espace localement compact $ X $. Nous dirons que $ \pi $ est m-propre si $ \pi $ est $ |m| $-propre (chap. V, § 6, n° 1, déf. 1); il est alors immédiat que pour toute fonction $ f \in \mathcal{K}_c(X) $, la fonction $ f \circ \pi $ est essentiellement $ m $-intégrable et que l’on a

$$
\left| \int (f \circ \pi) dm \right| \leq \int |f \circ \pi| d|m| = \int |f| d(\pi(|m|))
$$

donc l’application $ f \to \int (f \circ \pi) dm $ est continue dans $ \mathcal{K}_c(X) $, autrement dit c’est une mesure complexe sur $ X $, notée $ \pi(m) $ et appelée image de $ m $ par $ \pi $. En outre, il résulte de (8) que l’on a $ |\pi(m)| \leq \pi(|m|) $. Si $ m $ et $ m' $ sont deux mesures complexes sur $ T $ et si $ \pi $ est à la fois $ m $-propre et $ m' $-propre, alors $ \pi $ est $ (\lambda m + \lambda' m') $-propre quels que soient les scalaires complexes $ \lambda, \lambda' $, et on a $ \pi(\lambda m + \lambda' m') = \lambda \pi(m) + \lambda' \pi(m') $.

Soit $ Y $ un sous-espace localement compact de $ T $. Pour toute fonction $ f \in \mathcal{K}_c(Y) $, la fonction $ f' $ sur $ T $, définie par $ f'(t) = f(t) $ si $ t \in Y $ et $ f'(t) = 0 $ si $ t \notin Y $, est $ m $-intégrable (chap. V, § 1, n° 1); il est immédiat que l’application $ f \to \int f' dm $ est une mesure complexe sur $ Y $, appelée mesure induite sur $ Y $ par $ m $ et notée $ m_Y $. Si $ m = g.|m| $, il est clair que $ m_Y = g_Y.|m|_Y $, où $ g_Y $ est la restriction à $ Y $ de la fonction $ g $, qui est localement intégrable pour $ |m|_Y $ (chap. V, § 7, n° 1); en outre, comme $ |g_Y| = 1 $ localement presque partout pour $ |m|_Y $ (chap. V, § 7, n° 1, cor. 1 de la prop. 1), on a $ |m_Y| = |m|_Y $.

Soient $ T $ et $ T' $ deux espaces localement compacts, $ m $ (resp $ m' $) une mesure complexe sur $ T $ (resp. $ T' $). Posons $ m = g.|m| $ et $ m' = g'.|m'| $. La fonction $ g \otimes g' $ est localement intégrable sur $ T \times T' $ pour la mesure positive $ |m| \otimes |m'| $ (chap. V, § 8, n° 2, cor. 5 de la prop. 5), et on vérifie aussitôt que lorsqu’on remplace $ g $ (resp. $ g' $) par une fonction $ g_1 $ (resp. $ g_1 $) égale à $ g $ (resp. $ g' $) localement presque partout pour $ |m| $ (resp. $ |m'| $), $ g_1 \otimes g'_1 $ est égale à $ g \otimes g' $ localement presque partout pour $ |m| \otimes |m'| $. La mesure complexe $ (g \otimes g').(|m| \otimes |m'|) $ sur $ T \times T' $ ne dépend donc que de $ m $ et $ m' $; on la note $ m \otimes m' $ et on l’appelle la mesure produit de m et de m'. Comme $ |g \otimes g'| = 1 $ localement presque partout pour $ |m| \otimes |m'| $ (chap. V, § 8, no 2, cor. 8 de la prop. 5), on a $ |m \otimes m'| = |m| \otimes |m'| $.

Le lecteur vérifiera aisément que toutes les propositions démontrées au chap. V relativement à l'image d'une mesure positive, à la mesure induite par une mesure positive ou au produit de mesures positives, à l'exception de celles où interviennent des intégrales supérieures ou des intégrales supérieures essentielles, restent valables lorsqu'on remplace les mesures positives par des mesures complexes quelconques.

Enfin, on définit comme au § 1 la notion de fonction scalairement essentiellement m-intégrable pour une mesure complexe m ; pour qu'une fonction f ait cette propriété, il faut et il suffit que f soit scalairement essentiellement intégrable par rapport à $ |\mu_1| $ et à $ |\mu_2| $, où $ \mu_1 $ et $ \mu_2 $ sont les parties réelle et imaginaire de m, et on a alors $ \int f dm = \int f d\mu_1 + i \int f d\mu_2 $. Nous laissons au lecteur le soin de transcrire pour les mesures complexes les résultats du § 1.

## EXERCICES {#int-vi-s2-exercises}

See the [exercises for § 2](exercises/s2/).
