---
book: ac
book_title: Commutative Algebra
chapter: V
chapter_title: Entiers
section: 2
section_title: Relèvement des idéaux premiers
lang: fr
source: ac-v-vii-fr
pdf_pages: 0031-0053, 0073-0080
extraction: ocr
subsections:
    - "no": 1
      title: Le premier théorème d’existence
      page: 0
      pdf_page: 31
    - "no": 2
      title: Groupe de décomposition et groupe d’inertie
      page: 0
      pdf_page: 36
    - "no": 3
      title: Décomposition et inertie pour les anneaux intégralement clos
      page: 0
      pdf_page: 45
    - "no": 4
      title: Deuxième théorème d’existence
      page: 0
      pdf_page: 52
statements: 46
exercises: 12
content_sha256: 625739294eceba5ec4f58481795e89c52180e856a0a1e0ef6e59a1daa88008f8
---

## § 2. Relèvement des idéaux premiers.

### 1. Le premier théorème d’existence

#### Définition 1 {#ac-v-s2-def-1 .statement}

Soient $ A, A' $ deux anneaux, $ h : A \to A' $ un homomorphisme d’anneaux. On dit qu’un idéal $ a' $ de $ A' $ est au-dessus d’un idéal $ a $ de $ A $ si $ a = h^{-1}(a') $.

Dire qu’un idéal premier $ \mathfrak{p}' $ de $ A' $ est au-dessus d’un idéal premier $ \mathfrak{p} $ de $ A $ signifie donc que $ \mathfrak{p} $ est l’image de $ \mathfrak{p}' $ par l’application continue $ ^ah : \mathrm{Spec}(A') \to \mathrm{Spec}(A) $ associée à $ h $ (chap. II, § 4, no 3).

On notera que pour qu’il existe un idéal de $ A' $ au-dessus de l’idéal (0) de $ A $, il faut et il suffit que $ h : A \to A' $ soit injective.

Soit $ a $ un idéal de $ A $; par passage aux quotients, l’homomorphisme $ h $ donne un homomorphisme $ h_1 : A/a \to A'/aA' $; dire que $ a' $ est un idéal de $ A' $ au-dessus de $ a $ équivaut à dire que $ aA' \subset a' $ et que $ a'/aA' $ est un idéal de $ A'/aA' $ au-dessus de (0).

#### Lemme 1 {#ac-v-s2-lem-1 .statement}

Soient $ h : A \to A' $ un homomorphisme d’anneaux, $ S $ une partie multiplicative de $ A $, $ i = i_A^S : A \to S^{-1}A $, $ i' = i_{A'}^{h(S)} : A' \to S^{-1}A' = (h(S))^{-1}A' $ les homomorphismes canoniques, $ h_1 = S^{-1}h : S^{-1}A \to S^{-1}A' $, de sorte que l’on a un diagramme commutatif

$$
\begin{array}{ccc}
A & \xrightarrow{h} & A' \\
i \downarrow & & \downarrow i' \\
S^{-1}A & \xrightarrow{h_1} & S^{-1}A'
\end{array}
$$

Soit $ \mathfrak{p} $ un idéal premier de $ A $ tel que $ \mathfrak{p} \cap S = \emptyset $. Alors $ a' \to S^{-1}a' $ est une application surjective de l’ensemble $ \mathcal{F} $ des idéaux de $ A' $ au-dessus de $ \mathfrak{p} $ sur l’ensemble $ \mathcal{F}_1 $ des idéaux de $ S^{-1}A' $ au-dessus de $ S^{-1}\mathfrak{p} $, et l’application $ a'_1 \to i'^{-1}(a'_1) $ est une bijection de $ \mathcal{F}_1 $ sur l’ensemble des idéaux appartenant à $ \mathcal{F} $ et saturés pour $ h(S) $; en particulier $ \mathfrak{p}' \to S^{-1}\mathfrak{p}' $ est une bijection de l’ensemble des idéaux premiers de $ A' $ au-dessus de $ \mathfrak{p} $ sur l’ensemble des idéaux premiers de $ S^{-1}A' $ au-dessus de $ S^{-1}\mathfrak{p} $.

On sait que $ S^{-1}\mathfrak{p} $ est un idéal premier de $ S^{-1}A $ et que $ i^{-1}(S^{-1}\mathfrak{p}) = \mathfrak{p} $ (chap. II, § 2, no 5, prop. 11); s’il existe un idéal $ \mathfrak{b}' $ de $ S^{-1}A' $ au-dessus de $ S^{-1}\mathfrak{p} $, on a donc $ h^{-1}(i'^{-1}(\mathfrak{b}')) = i^{-1}(h_1^{-1}(\mathfrak{b}')) = \mathfrak{p} $; comme $ S^{-1}.i'^{-1}(\mathfrak{b}') = \mathfrak{b}' $ (loc. cit.), cela montre déjà que l’image de $ \mathcal{F} $ par l’application $ a' \to S^{-1}a' $ contient $ \mathcal{F}_1 $. D’autre part, si $ a' \in \mathcal{F} $, $ a \in A $ et $ s \in S $, on a les équivalences suivantes

$$
h_1(a/s) \in S^{-1}a' \iff h(a)/h(s) \in S^{-1}a'
$$
$$
\iff \text{il existe } t \in S \text{ tel que } h(t)h(a) \in a'
$$
$$
\iff \text{il existe } t \in S \text{ tel que } ta \in \mathfrak{p}
$$
$$
\iff a/z \in S^{-1}\mathfrak{p}.
$$

Donc on a $ h_1^{-1}(S^{-1}a') = S^{-1}\mathfrak{p} $, ce qui achève de prouver que l’image de $ \mathcal{F} $ par l’application $ a' \to S^{-1}a' $ est égale à $ \mathcal{F}_1 $; les autres assertions résultent du chap. II, § 2, no 5, prop. 11.

#### Proposition 1 {#ac-v-s2-prop-1 .statement}

*Soient* $ h : A \to A' $ *un homomorphisme d’anneaux tel que* $ A' $ *soit entier sur* $ A $, $ \mathfrak{p}' $ *un idéal premier de* $ A' $, *et* $ \mathfrak{p} = h^{-1}(\mathfrak{p}') $. *Pour que* $ \mathfrak{p} $ *soit maximal, il faut et il suffit que* $ \mathfrak{p}' $ *le soit*.

Posons en effet $ B = A/\mathfrak{p} $, $ B' = A'/\mathfrak{p}' $ et soit $ h_1 : B \to B' $ l’homomorphisme déduit de $ h $ par passage aux quotients; $ B $ et $ B' $ sont intègres et $ B' $ est entier sur $ B $ (\S 1, no 1, prop. 2). Dire que $ \mathfrak{p} $ (resp. $ \mathfrak{p}' $) est maximal signifie que $ B $ (resp. $ B' $) est un corps. La proposition résulte donc du lemme suivant:

#### Lemme 2 {#ac-v-s2-lem-2 .statement}

*Soient* $ B $ *un anneau intègre, A un sous-anneau de* $ B $ *tel que* $ B $ *soit entier sur* $ A $. *Pour que* $ B $ *soit un corps, il faut et il suffit que* $ A $ *soit un corps*.

Si $ A $ est un corps, alors, pour tout $ y \neq 0 $ dans $ B $, $ A[y] $ est par hypothèse (\S 1, th. 1) un $ A $-module de type fini; comme $ A[y] $ est intègre, c’est un corps (*Alg.*, chap. V, § 2, no 1, prop. 1), et *a fortiori* $ y $ est inversible dans $ B $, donc $ B $ est un corps. Inversement, supposons que $ B $ soit un corps, et soit $ z \neq 0 $ dans $ A $; comme $ z^{-1} \in B, z^{-1} $ est entier sur $ A $, autrement dit on a une équation de dépendance intégrale

$$
z^{-n} + a_1 z^{-(n-1)} + \cdots + a_n = 0
$$

où les $ a_i \in A $; or cette relation montre que l’on a

$$
-z^{-1} = a_1 + a_2 z + \cdots + a_n z^{n-1} \in A
$$

donc $ A $ est bien un corps.

#### Corollaire 1 {#ac-v-s2-lem-2-cor-1 .statement}

*Soient* $ h : A \to A' $ *un homomorphisme d’anneaux tel que* $ A' $ *soit entier sur* $ A $, $ \mathfrak{p} $ *un idéal premier de* $ A $, $ \mathfrak{p}' $ *et* $ a' $ *deux idéaux de* $ A' $ *au-dessus de* $ \mathfrak{p} $ *tels que* $ \mathfrak{p}' \subset a' $. *Si* $ \mathfrak{p}' $ *est premier, on a* $ a' = \mathfrak{p}' $.

Posons $ S = A - \mathfrak{p} $; alors $ S^{-1}A' $ est entier sur $ S^{-1}A $ ($ \S 1 $, n° 5, prop. 16), $ S^{-1}\mathfrak{p} $ est un idéal maximal de $ S^{-1}A $ (chap. II, $ \S 2 $, n° 5, prop. 11), $ S^{-1}\mathfrak{a}' $ et $ S^{-1}\mathfrak{p}' $ sont des idéaux de $ S^{-1}A' $ au-dessus de $ S^{-1}\mathfrak{p} $ (lemme 1) et l’on a $ S^{-1}\mathfrak{a}' \supset S^{-1}\mathfrak{p}' $. Comme $ S^{-1}\mathfrak{p}' $ est premier, il est maximal en vertu de la prop. 1, donc $ S^{-1}\mathfrak{p}' = S^{-1}\mathfrak{a}' $; par suite $ \mathfrak{a}' $ est contenu dans le saturé de $ \mathfrak{p}' $ pour $ h(S) $, qui est égal à $ \mathfrak{p}' $ (chap. II, $ \S 2 $, n° 5, prop. 11).

#### Corollaire 2 {#ac-v-s2-lem-2-cor-2 .statement}

Soient $ A' $ un anneau intègre, $ A $ un sous-anneau de $ A' $ tel que $ A' $ soit entier sur $ A $, $ f $ un homomorphisme de $ A' $ dans un anneau $ B $. Si la restriction de $ f $ à $ A $ est injective, $ f $ est injectif.

En effet, si $ \mathfrak{a}' $ est le noyau de $ f $, l’hypothèse signifie que $ \mathfrak{a}' \cap A = (0) $; comme $ A' $ est intègre, on peut appliquer le cor. 1 en prenant pour $ \mathfrak{p} $ et $ \mathfrak{p}' $ l’idéal (0) de $ A $ et l’idéal (0) de $ A' $ respectivement, d’où $ \mathfrak{a}' = (0) $.

#### Corollaire 3 {#ac-v-s2-lem-2-cor-3 .statement}

Soient $ h : A \to A' $ un homomorphisme d’anneaux tel que $ A' $ soit entier sur $ A $, $ m $ un idéal maximal de $ A $, et supposons qu’il n’y ait dans $ A' $ qu’un nombre fini d’idéaux maximaux distincts $ m'_j $ ($ 1 \leq j \leq n $) au-dessus de $ m $. Soit $ q'_j $ le saturé de $ mA' $ pour $ m'_j $ (chap. II, $ \S 2 $, n° 4). Alors :

(i) Dans l’anneau $ A'/q'_j $, les diviseurs de zéro sont les éléments de $ m'_j/q'_j $ et ils sont nilpotents ($ 1 \leq j \leq n $).

(ii) On $ a \ mA' = \bigcap_j q'_j = \prod_j q'_j $.

(iii) L’homomorphisme canonique $ A'/mA' \to \prod_j (A'/q'_j) $ est bijectif.

Pour qu’un idéal premier de $ A' $ contienne $ mA' $, il faut et il suffit que son image réciproque par $ h $ contienne $ m $, donc qu’il soit au-dessus de $ m $, puisque $ m $ est maximal dans $ A $; les $ m'_j $ sont donc les seuls idéaux premiers de $ A' $ contenant $ mA' $ (prop. 1), et par suite $ r' = \bigcap_j m'_j $ est la racine de $ mA' $ (chap. II, $ \S 2 $, n° 6, cor. 1 de la prop. 13). Par définition de $ q'_j $, la classe mod. $ q'_j $ d’un élément de $ A' - m'_j $ n’est pas diviseur de 0 dans $ A'/q'_j $; d’autre part, comme les $ m'_j $ sont des idéaux maximaux distincts, pour tout indice $ j $ il existe un élément $ a'_j $ appartenant à $ \bigcap_{i \neq j} m'_j $ et non à $ m'_j $ (chap. II, $ \S 1 $, n° 1, prop. 4); pour tout $ x \in m'_j $, on a alors $ a'_j x \in r' $, donc la classe mod. $ q'_j $ de $ a'_j x $ est nilpotente, et comme celle de $ a'_j $ n’est pas diviseur de 0, on en conclut que la classe de $ x $ est nilpotente;

#### Remarque 1 {#ac-v-s2-n1-rem-1 .statement}

Si $ A' $ est noethérien, il résulte de (i) et (ii) que $ (q_j')_{1 \leq j \leq n} $ est l’unique décomposition primaire de $ mA' $ (chap. IV, § 2, no 3).

#### Théorème 1 {#ac-v-s2-thm-1 .statement}

Soient $ h : A \to A' $ un homomorphisme injectif d’anneaux, tel que $ A' $ soit entier sur $ A $, $ \mathfrak{p} $ un idéal premier de $ A $. Il existe un idéal premier $ \mathfrak{p}' $ de $ A' $ au-dessus de $ \mathfrak{p} $.

Supposons d’abord que $ A $ soit un anneau local et $ \mathfrak{p} $ l’idéal maximal de $ A $; alors, pour tout idéal maximal $ m' $ de $ A' $, $ h^{-1}(m') $ est un idéal maximal de $ A $ (prop. 1), donc est égal à $ \mathfrak{p} $, ce qui démontre le théorème dans ce cas (puisque $ A' $ contient $ A $ par hypothèse, et n’est donc pas réduit à 0). Dans le cas général, posons $ S = A - \mathfrak{p} $; alors $ S^{-1}A $ est un anneau local dont $ S^{-1}\mathfrak{p} $ est l’idéal maximal (chap. II, § 2, no 5, prop. 11), $ S^{-1}h : S^{-1}A \to S^{-1}A' $ est injectif (chap. II, § 2, no 4, th. 1) et $ S^{-1}A' $ est entier sur $ S^{-1}A $ (§ 1, no 5, prop. 16); il existe donc un idéal premier $ q' $ de $ S^{-1}A' $ au-dessus de $ S^{-1}\mathfrak{p} $, et on sait que $ q' = S^{-1}\mathfrak{p}' $, où $ \mathfrak{p}' $ est un idéal premier de $ A' $ au-dessus de $ \mathfrak{p} $ (lemme 1).

Si $ h : A \to A' $ n’est pas injectif, le th. 1 n’est plus nécessairement exact, comme le montre l’exemple de l’homomorphisme $ \mathbf{Z} \to \mathbf{Z}/n\mathbf{Z} \ (n > 1) $. On peut toutefois appliquer le th. 1 à l’injection canonique $ h(A) \to A' $; autrement dit, l’énoncé du th. 1 est valable pour les idéaux premiers $ \mathfrak{p} $ contenant $ \mathrm{Ker}(h) $.

#### Corollaire 1 {#ac-v-s2-thm-1-cor-1 .statement}

Avec les hypothèses et notations du th. 1, on a $ h^{-1}(\mathfrak{p}A') = \mathfrak{p} $.

En effet, on a $ \mathfrak{p}A' \subset \mathfrak{p}' $ et $ h^{-1}(\mathfrak{p}') = \mathfrak{p} $.

#### Corollaire 2 {#ac-v-s2-thm-1-cor-2 .statement}

Soient $ h : A \to A' $ un homomorphisme d’anneaux tel que $ A' $ soit entier sur $ A $, $ a $ et $ \mathfrak{p} $ deux idéaux de $ A $ tels que $ a \subset \mathfrak{p} $, $ a' $ un idéal de $ A' $ au-dessus de $ a $. On suppose $ \mathfrak{p} $ premier. Il existe alors un idéal premier $ \mathfrak{p}' $ de $ A' $ au-dessus de $ \mathfrak{p} $ et contenant $ a' $.

Si $ h_1 : A/a \to A'/a' $ est l’homomorphisme déduit de $ h $ par passage aux quotients, $ h_1 $ est injectif par hypothèse et $ A'/a' $ est entier sur $ A/a $ ($ \S 1 $, n° 1, prop. 2); il existe donc un idéal premier $ \mathfrak{p}'/a' $ de $ A'/a' $ ($ \mathfrak{p}' $ premier dans $ A' $) au-dessus de $ \mathfrak{p}/a $ (th. 1), et $ \mathfrak{p}' $ répond à la question.

#### Corollaire 3 {#ac-v-s2-thm-1-cor-3 .statement}

Soient $ A $ un anneau, $ A' $ un anneau contenant $ A $ et entier sur $ A $. Si $ \mathfrak{R}' $ est le radical de $ A' $, $ \mathfrak{R}' \cap A $ est le radical de $ A $.

Soit $ \mathfrak{R} $ le radical de $ A $. Pour tout idéal maximal $ m' $ de $ A' $, $ m' \cap A $ est un idéal maximal de $ A $ (prop. 1), donc $ \mathfrak{R} \subset m' \cap A $ et par suite $ \mathfrak{R} \subset \mathfrak{R}' \cap A $ (*Alg.*, chap. VIII, § 5, n° 3, déf. 3). Inversement, soit $ x \in \mathfrak{R}' \cap A $; pour tout idéal maximal $ m $ de $ A $, il existe un idéal premier de $ A' $ au-dessus de $ m $ (th. 1) et cet idéal $ m' $ est nécessairement maximal (prop. 1), donc on a $ x \in m' \cap A = m $ et par suite $ x \in \mathfrak{R} $.

#### Corollaire 4 {#ac-v-s2-thm-1-cor-4 .statement}

Soient $ A $ un anneau, $ A' $ un anneau contenant $ A $ et entier sur $ A $, et $ f $ un homomorphisme de $ A $ dans un corps algébriquement clos $ L $. Alors $ f $ se prolonge en un homomorphisme de $ A' $ dans $ L $.

En effet, soit $ \mathfrak{p} $ le noyau de $ f $, qui est un idéal premier puisque $ f(A) \subset L $ est intègre; soit $ \mathfrak{p}' $ un idéal premier de $ A' $ au-dessus de $ \mathfrak{p} $ (th. 1). Alors $ A/\mathfrak{p} $ s’identifie canoniquement à un sous-anneau de $ A'/\mathfrak{p}' $ et $ A'/\mathfrak{p}' $ est entier sur $ A/\mathfrak{p} $ ($ \S 1 $, n° 1, prop. 2). L’homomorphisme $ f $ définit, par passage au quotient, un isomorphisme de $ A/\mathfrak{p} $ sur le sous-anneau $ f(A) $ de $ L $, qui se prolonge en un isomorphisme $ g $ du corps des fractions $ K $ de $ A/\mathfrak{p} $ sur un sous-corps de $ L $. Comme le corps des fractions $ K' $ de $ A'/\mathfrak{p}' $ est algébrique sur $ K $, $ g $ se prolonge en un isomorphisme $ g' $ de $ K' $ sur un sous-corps de $ L $ (*Alg.*, chap. V, § 4, n° 2, cor. du th. 1); si $ \pi' : A' \to A'/\mathfrak{p}' $ est l’homomorphisme canonique, $ g' \circ \pi' $ est un homomorphisme de $ A' $ dans $ L $ prolongeant $ f $.

#### Remarque 2 {#ac-v-s2-n1-rem-2 .statement}

Soit $ h : A \to A' $ un homomorphisme d’anneaux tel que $ A' $ soit entier sur $ A $; alors l’application continue associée $ ^ah : \mathrm{Spec}(A') \to \mathrm{Spec}(A) $ est *fermée*. En effet, pour tout idéal $ a' $ de $ A' $, $ A'/a' $ est entier sur $ A' $, donc aussi sur $ A $ ($ \S 1 $, n° 1, prop. 6) et $ \mathrm{Spec}(A'/a') $ s’identifie au sous-espace fermé $ V(a') $ de $ \mathrm{Spec}(A') $; pour montrer que $ ^ah $ est fermée, on voit donc (en remplaçant $ A' $ par $ A'/a' $) qu’il suffit de prouver que l’image de $ \mathrm{Spec}(A') $ par $ ^ah $ est une partie *fermée* de $ \mathrm{Spec}(A) $; or il résulte du th. 1 que cette image n’est autre que l’ensemble des idéaux premiers de $ A $ contenant l’idéal $ \mathrm{Ker}(h) $, et cet ensemble est fermé par définition de la topologie de $ \mathrm{Spec}(A) $.

#### Proposition 2 {#ac-v-s2-prop-2 .statement}

*Soient* $ h : A \to A' $ *un homomorphisme d’anneaux tel que* $ A' $ *soit entier sur* $ A $, $ \mathfrak{p} $ *un idéal premier de* $ A $, $ S = A - \mathfrak{p} $, $ (\mathfrak{p}'_i)_{i \in I} $ *la famille de tous les idéaux premiers de* $ A' $ *au-dessus de* $ \mathfrak{p} $, $ S' = \bigcap_{i \in I} (A' - \mathfrak{p}'_i) $; *alors on a* $ S^{-1}A' = S'^{-1}A' $.

En effet, par définition on a $ h(S) \subset S' $, et comme
$$
h(S)^{-1}A' = S^{-1}A',
$$
il suffit de prouver, en vertu du chap. II, § 2, n° 3, prop. 8, que si un idéal premier $ q' $ de $ A' $ ne rencontre pas $ h(S) $, il ne rencontre pas non plus $ S' $. Or, supposons que $ q' \cap h(S) = \emptyset $, et soit $ q = h^{-1}(q') $; on a donc $ q \cap S = \emptyset $, autrement dit $ q \subset \mathfrak{p} $. Comme $ q' $ est au-dessus de $ q $ par définition, il résulte du cor. 2 du th. 1 qu’il y a un indice $ i $ tel que $ q' \subset \mathfrak{p}'_i $, donc $ q' \cap S' = \emptyset $, ce qui achève la démonstration.

#### Proposition 3 {#ac-v-s2-prop-3 .statement}

*Soit* $ h : A \to A' $ *un homomorphisme d’anneaux tel que* $ A' $ *soit un* $ A $*-module de type fini; alors, pour tout idéal premier* $ \mathfrak{p} $ *de* $ A $, *l’ensemble des idéaux premiers de* $ A' $ *au-dessus de* $ \mathfrak{p} $ *est fini*.

Soit $ S = A - \mathfrak{p} $; en vertu du lemme 1, on peut remplacer $ A $ par $ S^{-1}A $, $ A' $ par $ S^{-1}A' $ (qui est un $ S^{-1}A $-module de type fini) et $ \mathfrak{p} $ par $ S^{-1}\mathfrak{p} $; autrement dit, on peut supposer que $ A $ est un anneau *local* et $ \mathfrak{p} $ son idéal maximal. On peut ensuite (d’après la remarque faite au début de ce n°) remplacer $ A $ par $ A/\mathfrak{p} $, $ A' $ par $ A'/\mathfrak{p}A' $ et $ \mathfrak{p} $ par $ (0) $, car $ A'/\mathfrak{p}A' = (A/\mathfrak{p}) \otimes_A A' $ est un $ (A/\mathfrak{p}) $-module de type fini. On est donc finalement ramené à démontrer la proposition lorsque $ A $ est un *corps* et $ \mathfrak{p} = (0) $; $ A' $ est alors une $ A $-algèbre de rang fini, donc *artinienne*, et on sait que dans une telle algèbre il n’y a qu’un nombre *fini* d’idéaux premiers (chap. IV, § 2, n° 5, prop. 9).

### 2. Groupe de décomposition et groupe d’inertie

#### Définition 2 {#ac-v-s2-def-2 .statement}

*Soient* $ A' $ *un anneau,* $ \mathcal{G} $ *un groupe opérant sur* $ A' $ *(§ 1, n° 9)*. *Étant donné un idéal premier* $ \mathfrak{p}' $ *de* $ A' $, *le sous-groupe des éléments* $ \sigma \in \mathcal{G} $ *tels que* $ \sigma.\mathfrak{p}' = \mathfrak{p}' $ *s’appelle le groupe de décomposition de* $ \mathfrak{p}' $ *(par rapport à* $ \mathcal{G} $) *et se note* $ \mathcal{G}^Z(\mathfrak{p}') $. *L’anneau* des éléments de $ A' $ invariants par $ G^z(p') $ s’appelle l’anneau de décomposition de $ p' $ (par rapport à $ G $) et se note $ A^z(p') $ (*).

On écrit souvent $ G^z $ et $ A^z $ au lieu de $ G^z(p') $ et $ A^z(p') $ respectivement, lorsqu’aucune confusion n’est à craindre.

Pour tout $ \sigma \in G^z(p') $, nous désignerons encore par $ z \to \sigma.z $ l’endomorphisme de l’anneau $ A'/p' $ déduit de l’endomorphisme $ x \to \sigma.x $ de $ A' $ en passant aux quotients; il est clair que le groupe $ G^z(p') $ opère ainsi sur l’anneau $ A'/p' $.

#### Définition 3 {#ac-v-s2-def-3 .statement}

Avec les notations de la déf. 2, le sous-groupe de $ G^z(p') $ formé des $ \sigma $ tels que l’endomorphisme $ z \to \sigma.z $ de $ A'/p' $ soit l’identité, s’appelle le groupe d’inertie de $ p' $ (par rapport à $ G $) et se note $ G^T(p') $ (ou $ G^T $). L’anneau des éléments de $ A' $ invariants par $ G^T(p') $ s’appelle l’anneau d’inertie de $ p' $ (par rapport à $ G $) et se note $ A^T(p') $ (ou $ A^T $) (**).

Si $ A $ est le sous-anneau de $ A' $ formé des invariants de $ G $, il est clair que l’on a

(1)
$$
A \subset A^z(p') \subset A^T(p') \subset A'.
$$

Il résulte des déf. 2 et 3 que pour tout $ \rho \in G $, on a

(2)
$$
G^z(\rho.p') = \rho G^z(p') \rho^{-1}, \quad G^T(\rho.p') = \rho G^T(p') \rho^{-1}.
$$

Si, pour tout $ \sigma \in G^z(p') $, $ \bar{\sigma} $ est l’automorphisme $ z \to \sigma.z $ de $ A'/p' $, $ \sigma \to \bar{\sigma} $ est un homomorphisme (dit canonique) de $ G^z $ dans le groupe $ \Gamma_0 $ des automorphismes de $ A'/p' $ laissant invariants les éléments de $ A^z/(p' \cap A^z) $ (identifié canoniquement à un sous-anneau de $ A'/p' $) et par définition $ G^T(p') $ est le noyau de cet homomorphisme canonique; $ G^T $ est donc un sous-groupe distingué de $ G^z $. Si $ k' $ est le corps des fractions de $ A'/p' $, tout automorphisme de $ A'/p' $ se prolonge d’une seule manière en un automorphisme de $ k' $, si bien que l’on peut aussi considérer $ z \to \bar{\sigma} $ comme un homomorphisme de $ G^z(p') $ dans le groupe des automorphismes de $ k' $. On notera enfin que puisque $ G^T $ est distingué dans $ G^z $, $ A^T $ est stable pour $ G^z $.

#### Lemme 3 {#ac-v-s2-lem-3 .statement}

Soient $ A' $ un anneau, $ G $ un groupe opérant sur $ A' $, $ A $ l’anneau des invariants de $ G $, $ p' $ un idéal premier de $ A' $,

(*) La lettre Z est l’initiale du mot allemand « Zerlegung » qui signifie « décomposition ».
(**) La lettre T est l’initiale du mot allemand « Trägheit » qui signifie « inertie ».

S une partie multiplicative de $ A $ ne rencontrant pas $ \mathfrak{p}' $. Alors on a $ \mathcal{G}^z(S^{-1}\mathfrak{p}') = \mathcal{G}^z(\mathfrak{p}') $, $ \mathcal{G}^T(S^{-1}\mathfrak{p}') = \mathcal{G}^T(\mathfrak{p}') $ et, si $ \mathcal{G} $ est localement fini, $ S^{-1}A^z(\mathfrak{p}') = A^z(S^{-1}\mathfrak{p}') $, $ S^{-1}A^T(\mathfrak{p}') = A^T(S^{-1}\mathfrak{p}') $.

Comme les éléments de $ S $ sont invariants par $ \mathcal{G} $, il est clair que si $ \sigma.\mathfrak{p}' = \mathfrak{p}' $, on a aussi $ \sigma.(S^{-1}\mathfrak{p}') = S^{-1}\mathfrak{p}' $. Inversement, supposons que $ \sigma \in \mathcal{G} $ soit tel que $ \sigma.(S^{-1}\mathfrak{p}') = S^{-1}\mathfrak{p}' $; alors, si $ x \in \mathfrak{p}' $, on a $ (\sigma.x)/1 \in S^{-1}\mathfrak{p}' $ et il existe par suite $ s \in S $ tel que $ s(\sigma.x) \in \mathfrak{p}' $, d’où $ \sigma.x \in \mathfrak{p}' $ puisque $ \mathfrak{p}' $ est premier et $ s \notin \mathfrak{p}' $; ceci prouve que $ \sigma.\mathfrak{p}' \subset \mathfrak{p}' $ et on montre de même que $ \sigma^{-1}.\mathfrak{p}' \subset \mathfrak{p}' $, donc $ \sigma.\mathfrak{p}' = \mathfrak{p}' $ et $ \sigma \in \mathcal{G}^z(\mathfrak{p}') $. Si $ \sigma \in \mathcal{G}^T(\mathfrak{p}') $, on a $ \sigma.x - x \in \mathfrak{p}' $ pour tout $ x \in A' $, donc aussi, pour tout $ s \in S $, $ \sigma.(x/s) - (x/s) = (\sigma.x - x)/s \in S^{-1}\mathfrak{p}' $, et par suite $ \sigma \in \mathcal{G}^T(S^{-1}\mathfrak{p}') $. Inversement, supposons que $ \sigma \in \mathcal{G}^T(S^{-1}\mathfrak{p}') $; pour tout $ x \in A' $ on a alors $ \sigma.(x/1) - (x/1) \in S^{-1}\mathfrak{p}' $, et par suite il existe $ s \in S $ tel que $ s(\sigma.x - x) \in \mathfrak{p}' $, d’où comme plus haut $ \sigma.x - x \in \mathfrak{p}' $, ce qui montre que $ \sigma \in \mathcal{G}^T(\mathfrak{p}') $. Les dernières assertions résultent du § 1, no 9, prop. 23.

#### Théorème 2 {#ac-v-s2-thm-2 .statement}

Soient $ A' $ un anneau, $ \mathcal{G} $ un groupe fini opérant sur $ A' $, $ A $ l’anneau des invariants de $ \mathcal{G} $, de sorte que $ A' $ est entier sur $ A $ (§ 1, no 9, prop. 22).

(i) Étant donnés deux idéaux premiers $ \mathfrak{p}', \mathfrak{q}' $ de $ A' $ au-dessus d’un même idéal premier $ \mathfrak{p} $ de $ A $, il existe $ \sigma \in \mathcal{G} $ tel que $ \mathfrak{q}' = \sigma.\mathfrak{p}' $; autrement dit, $ \mathcal{G} $ opère transitiivement dans l’ensemble des idéaux premiers de $ A' $ au-dessus de $ \mathfrak{p} $.

(ii) Soient $ \mathfrak{p}' $ un idéal premier de $ A' $, $ \mathfrak{p} = \mathfrak{p}' \cap A $, $ k $ (resp. $ k' $) le corps des fractions de $ A/\mathfrak{p} $ (resp. $ A'/\mathfrak{p}' $). Alors $ k' $ est une extension quasi-galoisienne (*) de $ k $, et l’homomorphisme canonique $ \sigma \to \overline{\sigma} $ de $ \mathcal{G}^z(\mathfrak{p}') $ dans le groupe $ \Gamma $ des $ k $-automorphismes de $ k' $ définit, par passage au quotient, un isomorphisme de $ \mathcal{G}^z(\mathfrak{p}')/\mathcal{G}^T(\mathfrak{p}') $ sur $ \Gamma $.

(i) Si $ x \in \mathfrak{q}' $, on a $ \prod_{\sigma \in \mathcal{G}} \sigma.x \in \mathfrak{q}' \cap A = \mathfrak{p} \subset \mathfrak{p}' $; donc il existe $ \sigma \in \mathcal{G} $ tel que $ \sigma.x \in \mathfrak{p}' $, c’est-à-dire $ x \in \sigma^{-1}.\mathfrak{p}' $. On en conclut que $ \mathfrak{q}' \subset \bigcup_{\sigma \in \mathcal{G}} \sigma.\mathfrak{p}' $, donc (comme $ \mathcal{G} $ est fini et les $ \sigma.\mathfrak{p}' $ premiers) il existe $ \sigma \in \mathcal{G} $ tel que $ \mathfrak{q}' \subset \sigma.\mathfrak{p}' $ (chap. II, § 1, no 1, prop. 2); comme $ \mathfrak{q}' $ et $ \sigma.\mathfrak{p}' $ sont tous deux au-dessus de $ \mathfrak{p} $, on a $ \mathfrak{q}' = \sigma.\mathfrak{p}' $ (no 1, cor. 1 de la prop. 1).

(*) Afin d’éviter des confusions avec d’autres sens du mot « normal », nous emploierons désormais les termes « extension quasi-galoisienne » comme synonymes des termes « extension normale » définis en Alg., chap. V, § 6, no 2, déf. 2.

Il est clair que pour tout $ \sigma \in \mathcal{G}^z $, $ \bar{\sigma} $ est un $ k $-automorphisme de $ k' $; il reste à voir que $ \sigma \to \bar{\sigma} $ applique $ \mathcal{G}^z $ sur le groupe de tous les $ k $-automorphismes de $ k' $. Posons $ S = A - \mathfrak{p} $; on ne change pas $ k $ et $ k' $ en remplaçant $ A' $ et $ \mathfrak{p}' $ par $ S^{-1}A' $ et $ S^{-1}\mathfrak{p}' $ respectivement, en vertu du § 1, no 9, prop. 23 et de la relation $ S^{-1}\mathfrak{p}' \cap S^{-1}A = S^{-1}(A \cap \mathfrak{p}') = S^{-1}\mathfrak{p} $ (chap. II, § 2, no 4); il résulte du lemme 3 que l’on ne change pas ainsi non plus $ \mathcal{G}^z $ ni la façon dont opère $ \mathcal{G}^z $ sur $ k' $; on peut par suite se borner au cas où $ \mathfrak{p} $ est maximal, auquel cas on sait qu’il en est de même de $ \mathfrak{p}' $ (no 1, prop. 1), et tout élément de $ k' $ est donc de la forme $ \pi'(x) $ pour un $ x \in A' $; on a vu ci-dessus qu’un tel élément est racine d’un polynôme de $ k[X] $ de degré $ \leqslant \mathrm{Card}(\mathcal{G}) $. Comme toute extension séparable de degré fini de $ k $ admet un élément primitif ($ Alg. $, chap. V, § 7, no 7, prop. 12 et § 11, no 4, prop. 4), on voit que toute extension séparable de degré fini de $ k $ contenue dans $ k' $ est de degré $ \leqslant \mathrm{Card}(\mathcal{G}) $, d’où résulte que la plus grande extension séparable $ k'_s $ de $ k $ contenue dans $ k' $ ($ Alg. $, chap. V, § 7, no 6, prop. 11) est de degré $ \leqslant \mathrm{Card}(\mathcal{G}) $ ($ Alg. $, chap. V, § 3, no 2, Remarque 2). Soit $ y \in A' $ un élément tel que $ \pi'(y) $ soit élément primitif de $ k'_s $. Les idéaux $ \sigma.\mathfrak{p}' $ pour $ \sigma \in \mathcal{G} - \mathcal{G}^z $ sont maximaux et distincts de $ \mathfrak{p}' $ par définition; il existe par suite $ x \in A' $ tel que $ x \equiv y \pmod{\mathfrak{p}'} $ et $ x \in \sigma^{-1}\mathfrak{p}' $ pour $ \sigma \in \mathcal{G} - \mathcal{G}^z $ (chap. II, § 1, no 2, prop. 5). Cela étant, soit $ u $ un $ k $-automorphisme de $ k' $ et soit $ P(X) = \prod_{\sigma \in \mathcal{G}} (X - \pi'(\sigma.x)) $; comme $ \pi'(x) $ est racine de $ P $ et que $ P \in k[X] $, $ u(\pi'(x)) $ est aussi racine de $ P $ dans $ k' $, donc il existe $ \tau \in \mathcal{G} $ tel que
$$
u(\pi'(x)) = \pi'(\tau.x);
$$
mais on a $ u(\pi'(x)) \neq 0 $ et pour $ \sigma \in \mathcal{G} - \mathcal{G}^z $ on a $ \sigma.x \in \mathfrak{p}' $, donc π′(σ.x) = 0; on en conclut que l’on a nécessairement τ ∈ G_f^z. Mais comme u et τ ont même valeur pour l’élément primitif π′(y) = π′(x) de k_s′, ils coïncident dans k_s′, et comme k′ est une extension radicielle de k_s′, ils coincident dans k′. C.Q.F.D.

#### Corollaire {#ac-v-s2-n2-cor-1 .statement}

Les hypothèses et les notations étant celles du th. 2, soient f_1, f_2 deux homomorphismes de A′ dans un corps L, ayant même restriction à A. Alors il existe σ ∈ G_f tel que

$$ f_2(x) = f_1(σ.x) $$

pour tout x ∈ A′.

Soit p_i′ le noyau de f_i (i = 1, 2) qui est un idéal premier de A′; par hypothèse on a p_1′ ∩ A = p_2′ ∩ A et cette intersection est un idéal premier p de A; il existe par suite τ ∈ G_f tel que τ.p_2′ = p_1′ (th. 2, (i)); remplaçant f_1 par l’homomorphisme x → f_1(τ.x), on peut donc supposer que p_2′ = p_1′ (idéal que nous noterons p′). Par passage au quotient, on déduit alors de f_1 et f_2 deux homomorphismes injectifs f_1′, f_2′ de A′/p′ dans L qui se prolongent donc en deux homomorphismes injectifs f_1″, f_2″ du corps des fractions k′ de A′/p′ dans L. Comme k′ est une extension quasi-galoisienne de k, il en est de même de k_1″ = f_1″(k′) et k_2″ = f_2″(k′) (k étant identifié à un sous-corps de L), et comme il y a un k-isomorphisme de k_1″ sur k_2″, on a k_1″ = k_2″ (Alg., chap. V, § 6, prop. 6). Ainsi f_1″^{-1} o f_2″ est un k-automorphisme de k′; en vertu du th. 2, (ii), il est donc de la forme $ \overline{σ} $, où σ ∈ G_f^z(p′). En particulier, pour tout x ∈ A′ les éléments f_2(x) et f_1(σ.x) sont égaux.

#### Remarque 1 {#ac-v-s2-n2-rem-1 .statement}

On notera que sous les hypothèses du th. 2, il se peut que k′ soit de degré infini sur k lorsque k′ n’est pas séparable sur k (exerc. 9).

#### Remarque 2 {#ac-v-s2-n2-rem-2 .statement}

Il est clair que k′ est une extension galoisienne de k lorsque le corps k est parfait. Elle est alors de degré fini sur k.

#### Proposition 4 {#ac-v-s2-prop-4 .statement}

Soient A′ un anneau, G_f un groupe fini opérant sur A′, H un sous-groupe de G_f, A et B les anneaux d’invariants de G_f et H respectivement, p′ un idéal premier de A′; posons p = A ∩ p′, p(B) = B ∩ p′.

(i) Pour que H soit contenu dans le groupe de décomposition G_f^z(p′), il faut et il suffit que p′ soit le seul idéal premier de A au-dessus de p(B).

(ii) Si H contient G_f^z(p′), les conditions suivantes sont satisfaites:

a) Les anneaux A/p et B/p(B) ont même corps des fractions.

b) L’idéal maximal de l’anneau local $ B_{\mathfrak{p}(B)} $ est égal à $ \mathfrak{p}B_{\mathfrak{p}(B)} $.

(iii) Supposons de plus que $ A' $ soit intègre et que l’on ait $ \bigcap_{n \geq 0} \mathfrak{p}^n A'_{\mathfrak{p}'} = 0 $; alors les conditions a) et b) de (ii) entraînent que $ G^z(\mathfrak{p}') $ laisse invariants les éléments de $ B $.

(i) Il résulte du th. 2, (i) que les idéaux premiers de $ A' $ au-dessus de $ \mathfrak{p}(B) $ sont les idéaux de la forme $ \sigma.\mathfrak{p}' $, où $ \sigma \in \mathcal{H} $; d’où aussitôt (i).

(ii) Posons $ S = A - \mathfrak{p} $; on sait que les anneaux d’invariants de $ G $ et $ \mathcal{H} $ dans $ S^{-1}A' $ sont respectivement $ S^{-1}A $ et $ S^{-1}B $ (\$ 1, no 9, prop. 23) et l’on a $ G^z(S^{-1}\mathfrak{p}') = G^z(\mathfrak{p}') $ (lemme 3); enfin on a $ S^{-1}\mathfrak{p}(B) = S^{-1}\mathfrak{p}' \cap S^{-1}B $ (chap. II, § 2, no 4), l’anneau local de l’idéal premier $ S^{-1}\mathfrak{p}(B) $ de l’anneau $ S^{-1}B $ est canoniquement isomorphe à $ B_{\mathfrak{p}(B)} $ et son corps résiduel est isomorphe au corps des fractions de $ B/\mathfrak{p}(B) $ (chap. II, § 2, no 5, prop. 11). On peut donc, pour démontrer (ii), se borner au cas où $ \mathfrak{p} $ est maximal. Pour établir a), il nous suffira de prouver que l’on a

(3)
$$
B = A + \mathfrak{p}(B)
$$
car cela montrera que les corps $ A/\mathfrak{p} $ et $ B/\mathfrak{p}(B) $ sont canoniquement isomorphes. En vertu du th. 2, il n’y a qu’un nombre fini d’idéaux premiers de $ A' $ au-dessus de $ \mathfrak{p} $, et en vertu du th. 1 du no 1, il y a au moins un idéal premier de $ A' $ au-dessus de tout idéal premier de $ B $; cela entraîne qu’il n’y a qu’un nombre fini d’idéaux premiers de $ B $ au-dessus de $ \mathfrak{p} $; désignons par $ n_j (1 \leq j \leq r) $ ceux de ces idéaux qui sont $ \neq \mathfrak{p}(B) $. Soit $ x $ un élément de $ B $; comme les idéaux $ \mathfrak{p}(B) $ et $ n_j $ sont maximaux (no 1, prop. 1), il existe $ y \in B $ tel que $ y \equiv x $ (mod. $ \mathfrak{p}(B) $) et $ y \in n_j $ pour $ 1 \leq j \leq r $ (chap. II, § 1, no 2, prop. 5). Soient $ y_1 = y, y_2, \ldots, y_q $ les éléments distincts de l’orbite de $ y $ pour $ G $; il est clair que
$$
z = y_1 + y_2 + \cdots + y_q \in A,
$$
et pour établir (3), il suffira de montrer que l’on a $ y_i \in \mathfrak{p}' $ pour $ i \geq 2 $, car alors on en déduira que $ z - y \in \mathfrak{p}' \cap B = \mathfrak{p}(B) $, d’où $ x \in A + \mathfrak{p}(B) $ puisque $ x \equiv y $ (mod. $ \mathfrak{p}(B) $). Soit donc $ i \geq 2 $ et soit $ \sigma \in G $ tel que $ \sigma.y = y_i $; montrons que $ \sigma^{-1}.\mathfrak{p}' $ n’est pas au-dessus de $ \mathfrak{p}(B) $. Sinon, en effet, il existerait $ \tau \in \mathcal{H} $ tel que $ \sigma^{-1}.\mathfrak{p}' = \tau.\mathfrak{p}' $ (th. 2, (i)), d’où $ (\tau^{-1}\sigma^{-1}).\mathfrak{p}' = \mathfrak{p}' $, autrement dit $ \tau^{-1}\sigma^{-1} \in G^z \subset \mathcal{H} $ par hypothèse, d’où $ \sigma \in \mathcal{H} $; mais comme $ y \in B $ et $ \sigma.y \neq y $, cela est absurde. On en conclut que $ \sigma^{-1}.\mathfrak{p}' $ est au-dessus d’un des idéaux $ n_j $, et comme $ y \in n_j $ par construction, on a bien $ y \in \sigma^{-1}.\mathfrak{p}' $, ou $ y_i = \sigma.y \in \mathfrak{p}' $.

$$(4)$$
$$
\mathfrak{p}(B) \subset q \cup n_1 \cup \cdots \cup n_r
$$

en vertu du chap. II, § 1, no 1, prop. 2. Pour cela, considérons un élément $ u \in \mathfrak{p}(B) $ n’appartenant à aucun des $ n_j $ ($ 1 \leq j \leq r $) (chap. II, § 1, no 1, prop. 2); soient $ u_1 = u, u_2, \ldots, u_m $ les éléments distincts de l’orbite de $ u $ pour $ \mathcal{G} $; posons $ w = u_1 u_2 \ldots u_m, v = u_2 \ldots u_m $; il est clair que l’on a $ w \in A $; d’autre part, si $ \tau \in \mathcal{H} $, on a $ \tau.u = u $, donc nécessairement $ \tau.u_i \neq u $ pour $ i \geq 2 $, ce qui montre que $ \tau.v = v $, donc $ v \in B $. On montre comme dans la démonstration de $ a) $ que si $ \sigma \in \mathcal{G} $ est tel que $ \sigma.u = u_i $ avec $ i \geq 2 $, $ \sigma^{-1}.\mathfrak{p}' $ est au-dessus de l’un des $ n_j $, et comme $ u \notin n_j $ on a aussi $ u \notin \sigma^{-1}.\mathfrak{p}' $, autrement dit $ u_i \notin \mathfrak{p}' $. On en conclut que $ v \notin \mathfrak{p}' $, et par suite $ v \notin \mathfrak{p}(B) $. Par ailleurs il est clair que $ w \in \mathfrak{p}' \cap A = \mathfrak{p} $, et la relation $ w = uv $ montre que $ u $ est dans le saturé de $ \mathfrak{p}B $ pour $ \mathfrak{p}(B) $, donc établit (4).

(iii) Supposons que $ A' $ soit intègre, que $ \bigcap_{n \geq 0} \mathfrak{p}^n A'_{\mathfrak{p}'} = 0 $ et que les conditions $ a) $ et $ b) $ de (ii) soient vérifiées. Avec les mêmes notations que dans (ii), il est clair que $ S^{-1}A' $ est intègre et $ S^{-1}A'_{\mathfrak{p}'} = A'_{\mathfrak{p}'} $; on peut donc remplacer $ A' $ et $ \mathfrak{p}' $ par $ S^{-1}A' $ et $ S^{-1}\mathfrak{p}' $, autrement dit, supposer encore que l’idéal $ \mathfrak{p} $ est maximal. Les hypothèses $ a) $ et $ b) $ entraînent alors que

$$(5)$$
$$
B_{\mathfrak{p}(B)} = A + \mathfrak{p}B_{\mathfrak{p}(B)}
$$

Par récurrence sur $ n $, on en déduit que $ B_{\mathfrak{p}(B)} = A + \mathfrak{p}^n B_{\mathfrak{p}(B)} $ pour tout $ n > 0 $. Soient alors $ \sigma $ un élément de $ \mathcal{G}^z $ et $ x $ un élément de $ B $. Pour tout $ n > 0 $, il existe $ a_n \in A $ tel que $ x - a_n \in \mathfrak{p}^n B_{\mathfrak{p}(B)} \subset \mathfrak{p}^n A'_{\mathfrak{p}'} $; comme $ \sigma.a_n = a_n $ et $ \sigma.\mathfrak{p}' = \mathfrak{p}' $, on en déduit que $ \sigma.x - x \in \mathfrak{p}^n A'_{\mathfrak{p}'} $. Cette relation ayant lieu pour tout $ n $, on conclut de l’hypothèse que $ \sigma.x = x $.

#### Remarque 3 {#ac-v-s2-n2-rem-3 .statement}

Si $ A' $ est intègre et noethérien, la condition $ \bigcap_{n \geq 1} \mathfrak{p}^n A'_{\mathfrak{p}'} = 0 $ est toujours vérifiée (chap. III, § 3, no 2, cor. de la prop. 5). On peut montrer que cette condition est aussi satisfaite si on suppose que $ A' $ est intègre et $ A $ noethérien.

#### Remarque 4 {#ac-v-s2-n2-rem-4 .statement}

Lorsque $ \mathfrak{p} $ n’est pas un idéal maximal de $ A $, on n’a pas nécessairement la relation (3) sous les hypothèses de (ii) et par suite $ A/\mathfrak{p} $ et $ B/\mathfrak{p}(B) $ ne sont pas nécessairement isomorphes, même lorsque l’on prend $ \mathcal{H} = \mathcal{G}^z $, d’où $ B = Az $ (exerc. 10).

#### Corollaire 1 {#ac-v-s2-prop-4-cor-1 .statement}

Sous les hypothèses du th. 2, les anneaux $ A/\mathfrak{p} $ et $ A^z/(\mathfrak{p}' \cap A^z) $ ont même corps de fractions, et l’idéal maximal de l’anneau local $ (A^z)_{\mathfrak{p}' \cap A^z} $ est engendré par $ \mathfrak{p} $.

#### Corollaire 2 {#ac-v-s2-prop-4-cor-2 .statement}

Soient $ A' $ un anneau intègre, $ G $ un groupe fini opérant sur $ A' $, $ A $ l’anneau des invariants de $ G $, $ \mathfrak{p}' $ un idéal premier de $ A' $; soient $ K, K^z $ et $ K' $ les corps des fractions de $ A, A^z $ et $ A' $ respectivement. Alors $ K' $ est extension galoisienne de $ K $, et les sous-corps $ L $ de $ K' $ contenant $ K $ et tels que $ \mathfrak{p}' $ soit le seul idéal premier de $ A' $ au-dessus de l’idéal $ \mathfrak{p}' \cap L $ de $ A' \cap L $, ne sont autres que ceux qui contiennent $ K^z $.

En effet, $ G $ opère sur $ K' $ et $ K $ est le corps des invariants de $ G $ dans $ K' $ (\$ 1, no 9, prop. 23 appliquée à $ S = A - \{0\} $), et de même $ K^z $ est le corps des invariants de $ G^z $; par définition $ K' $ est donc extension galoisienne de $ K $. Si $ \mathcal{H} $ est le sous-groupe de $ G $ formé des $ \sigma \in G $ laissant invariants les éléments de $ L $, dire que $ L $ contient $ K^z $ signifie que $ \mathcal{H} $ est contenu dans $ G^z $ (Alg., chap. V, § 10, no 5, th. 3), et comme $ L $ est le corps des invariants de $ \mathcal{H} $ dans $ K' $, $ A' \cap L $ est l’anneau des invariants de $ \mathcal{H} $ dans $ A' $; la seconde assertion résulte donc de la prop. 4, (i).

#### Définition 4 {#ac-v-s2-def-4 .statement}

Les hypothèses et notations étant celles du cor. 2 de la prop. 4, on dit qu’un idéal premier $ \mathfrak{p} $ de $ A $ se décompose complètement dans $ K' $ si le nombre des idéaux premiers de $ A' $ au-dessus de $ \mathfrak{p} $ est égal à $ [K':K] $.

Il revient au même de dire que, pour un idéal premier $ \mathfrak{p}' $ de $ A' $ au-dessus de $ \mathfrak{p} $, le sous-groupe $ G^z(\mathfrak{p}') $ est égal au sous-groupe $ \mathcal{H} $ laissant invariants tous les éléments de $ A' $, ou que $ A^z(\mathfrak{p}') = A' $, ou que $ G/\mathcal{H} $ opère fidèlement dans l’ensemble des idéaux premiers de $ A' $ au-dessus de $ \mathfrak{p} $.

#### Corollaire 3 {#ac-v-s2-def-4-cor-3 .statement}

Soient $ A' $ un anneau intègre, $ G $ un groupe commutatif fini opérant sur $ A' $, $ A $ l’anneau des invariants de $ G $, $ \mathfrak{p} $ un idéal premier de $ A $, $ K $ et $ K' $ les corps des fractions de $ A $ et $ A' $ respectivement. Alors les idéaux premiers de $ A' $ au-dessus de $ \mathfrak{p} $ ont tous même anneau de décomposition $ A^z $, et le corps des fractions $ K^z $ de $ A^z $ est le plus grand corps intermédiaire entre $ K $ et $ K' $ dans lequel $ \mathfrak{p} $ se décompose complètement.

Si $ \mathfrak{p}' $ est un idéal premier de $ A' $ au-dessus de $ \mathfrak{p} $, on a $ G^z(\sigma.\mathfrak{p}') = G^z(\mathfrak{p}') $ puisque $ G $ est commutatif (formule (2)), donc (th. 2, (i)) tous les idéaux premiers de $ A' $ au-dessus de $ \mathfrak{p} $ ont même groupe de décomposition $ \mathcal{G}^z $, et par suite même anneau de décomposition $ A^z $; leur nombre est $ (\mathcal{G} : \mathcal{G}^z) $. Soit $ L $ un corps intermédiaire entre $ K $ et $ K' $ et soit $ \mathcal{H} $ le sous-groupe de $ \mathcal{G} $ laissant invariants les éléments de $ L $; le groupe de décomposition de $ \mathfrak{p}' $ par rapport à $ \mathcal{H} $ est $ \mathcal{G}^z \cap \mathcal{H} $; comme $ A' \cap L $ est l’anneau des invariants de $ \mathcal{H} $ dans $ A' $, le nombre d’idéaux premiers de $ A' $ au-dessus de $ \mathfrak{p}' \cap L $ est $ (\mathcal{H} : (\mathcal{G}^z \cap \mathcal{H})) = (\mathcal{H}\mathcal{G}^z : \mathcal{G}^z) $ (puisque $ \mathcal{G} $ est commutatif). Le nombre d’idéaux premiers de $ A' \cap L $ au-dessus de $ \mathfrak{p} $ est donc $ (\mathcal{G} : \mathcal{H}\mathcal{G}^z) $. Pour que $ \mathfrak{p} $ se décompose complètement dans $ L $, il faut et il suffit donc que l’on ait $ (\mathcal{G} : \mathcal{H}\mathcal{G}^z) = [L : K] = (\mathcal{G} : \mathcal{H}) $, et comme $ \mathcal{H} \subset \mathcal{H}\mathcal{G}^z $, cela équivaut à $ \mathcal{H}\mathcal{G}^z = \mathcal{H} $, ou encore à $ \mathcal{G}^z \subset \mathcal{H} $, et finalement à $ L \subset K^z $.

#### Proposition 5 {#ac-v-s2-prop-5 .statement}

*Les hypothèses et notations étant celles du th. 2, le corps des fractions $ k^T $ de $ A^T / (\mathfrak{p}' \cap A^T) $ est égal à la plus grande extension séparable $ k'_s $ de $ k $ contenue dans $ k' $.

Comme dans la prop. 4, on peut se ramener au cas où $ \mathfrak{p} $ est un idéal maximal de $ A $, ce qui entraîne que $ \mathfrak{p}' $, $ \mathfrak{p}' \cap A^z $ et $ \mathfrak{p}' \cap A^T $ sont maximaux dans $ A' $, $ A^z $ et $ A^T $ respectivement (n° 1, prop. 1).

Pour tout $ x \in A' $, le polynôme $ P(X) = \prod_{\sigma \in \mathcal{G}^T} (X - \sigma.x) $ a ses coefficients dans l’anneau d’inertie $ A^T $, et par définition de $ \mathcal{G}^T $, toutes ses racines dans $ A' $ sont congrues mod. $ \mathfrak{p}' $; le polynôme $ \pi'(P) $ sur $ A^T / (\mathfrak{p}' \cap A^T) $ dont les coefficients sont les images canoniques de ceux de $ P $ par l’homomorphisme $ \pi' : A' \to A'/\mathfrak{p}' $ a donc toutes ses racines dans $ A'/\mathfrak{p}' $ égales à l’image de $ x $, ce qui montre que $ k' $ est une extension *radicielle* de $ k^T $; d’où $ k'_s \subset k^T $, puisque tout élément de $ k'_s $ est séparable sur $ k $, et *a fortiori* sur $ k^T $.

On sait que $ k'_s $ est une extension galoisienne de $ k $ (*Alg.*, chap. V, § 10, n° 9, prop. 14) et il résulte du th. 2 que son groupe de Galois est isomorphe à $ \mathcal{G}' = \mathcal{G}^z / \mathcal{G}^T $. Comme $ k^T $ est une extension radicielle de $ k'_s $, $ k^T $ est une extension quasi-galoisienne de $ k $, et le facteur séparable du degré de $ k^T $ sur $ k $ est $ q = (\mathcal{G}^z : \mathcal{G}^T) $. Il reste à voir que $ k^T $ est une extension séparable de $ k $. Nous avons vu plus haut que $ \mathcal{G}' $ s’identifie à un groupe d’automorphismes de $ A^T $, et que $ A^z $ est l’anneau des invariants de $ \mathcal{G}' $. Si $ x \in A^T $, le polynôme $ Q(X) = \prod_{\sigma' \in \mathcal{G}'} (X - \sigma'(x)) $ a donc ses coefficients dans $ A^z $; le polynôme sur $ A^z / (\mathfrak{p}' \cap A^z) $ dont les coefficients sont les images de ceux de $ Q $ par $ \pi' $ est de degré $ q $ et a pour racine π'(x) ∈ A^T/(p' ∩ A^T). Comme A^Z/(p' ∩ A^Z) = k en vertu de la prop. 4, (ii), on voit que tout élément de k^T est de degré $ \leq q $ sur k.

Cela étant, soit $ k_1 $ le corps des invariants du groupe des k-automorphismes de l’extension quasi-galoisienne $ k^T $ de k; on a $[k^T : k_1] = q$ (Alg., chap. V, § 10, no 9, prop. 14). Soit u un élément primitif de $ k^T $ sur $ k_1 $; comme il est de degré q sur $ k_1 $ et de degré $ \leq q $ sur k, il est de degré q sur k et son polynôme minimal sur $ k_1 $ a ses coefficients dans k; ceci montre que u est séparable sur k. D’autre part, pour tout $ v \in k_1 $, il existe une puissance $ p^f $ de l’exposant caractéristique p telle que $ v^{p^f} \in k $. On en conclut que $ k(u - v) $, qui contient

$$(u - v)^{p^f} = u^{p^f} - v^{p^f},$$

contient $ u^{p^f} $ et par conséquent $ k(u^{p^f}) $. Mais comme u est séparable sur k, on a $ k(u) = k(u^{p^f}) $ (Alg., chap. V, § 8, no 3, prop. 4), d’où $ k(u) \subset k(u - v) $. Comme u est de degré q sur k et $ u - v $ de degré $ \leq q $, il en résulte que $ k(u) = k(u - v) $, d’où $ v \in k(u) $. Ceci montre que v est séparable sur k, donc $ k_1 = k $ et $ k^T $ est séparable sur k.

C.Q.F.D.

#### Corollaire {#ac-v-s2-n2-cor-2 .statement}

Si l’ordre du groupe d’inertie $ G^T(p') $ est étranger à l’exposant caractéristique p de k, le corps $ k' $ est une extension galoisienne de k.

En effet, avec les notations de la démonstration de la prop. 5, le polynôme $ \pi'(P) $ a ses coefficients dans $ k^T = k'_s $ et toutes ses racines égales à $ \pi'(x) $; on en déduit aussitôt que $ \pi'(P) $ est une puissance du polynôme minimal de $ \pi'(x) $ sur $ k'_s $; mais ce dernier a un degré égal à une puissance de p, donc, comme le degré de $ \pi'(P) $ est égal à l’ordre de $ G^T $, l’hypothèse entraîne que $ \pi'(x) \in k'_s $, autrement dit $ k'_s = k' $.

### 3. Décomposition et inertie pour les anneaux intégralement clos

#### Lemme 4 {#ac-v-s2-lem-4 .statement}

Soient A un anneau intégralement clos, K son corps des fractions, p l’exposant caractéristique de K, K’ une extension radicielle de K et A’ un sous-anneau de K’ contenant A et entier sur A. Pour tout idéal premier $ \mathfrak{p} $ de A, il existe un idéal premier $ \mathfrak{p}' $ et un seul de A’ au-dessus de $ \mathfrak{p} $ et $ \mathfrak{p}' $ est l’ensemble des $ x \in A' $ tels qu’il existe un entier $ m \geq 0 $ pour lequel $ x^{p^m} \in \mathfrak{p} $.

L’existence de $ \mathfrak{p}' $ résulte du n° 1, th. 1. Si $ x \in \mathfrak{p}' $, il existe $ m \geqslant 0 $ tel que $ x^{p^m} \in K $, d’où $ x^{p^m} \in A $ puisque $ A $ est intégralement clos, donc $ x^{p^m} \in \mathfrak{p}' \cap A = \mathfrak{p} $. Inversement, si $ x \in A' $ est tel que $ x^{p^m} \in \mathfrak{p} \subset \mathfrak{p}' $, on a $ x \in \mathfrak{p}' $ puisque $ \mathfrak{p}' $ est premier.

#### Remarque 1 {#ac-v-s2-n3-rem-1 .statement}

Il résulte du § 1, n° 3, cor. de la prop. 11 que la fermeture intégrale de $ A $ dans $ K' $ est l’ensemble des $ x \in K' $ tels qu’il existe $ m \geqslant 0 $ pour lequel $ x^{p^m} \in A $ (Alg., chap. V, § 8, n° 1, prop. 1).

#### Proposition 6 {#ac-v-s2-prop-6 .statement}

Soient $ A $ un anneau intégralement clos, $ K $ son corps des fractions, $ K' $ une extension quasi-galoisienne de $ K $, $ A' $ la fermeture intégrale de $ A $ dans $ K' $. Alors :
(i) Pour tout idéal premier $ \mathfrak{p} $ de $ A $, le groupe $ G $ des $ K $-automorphismes de $ K' $ opère transitivement dans l’ensemble des idéaux premiers de $ A' $ au-dessus de $ \mathfrak{p} $.
(ii) Pour tout idéal premier $ \mathfrak{p}' $ de $ A' $, le corps des fractions $ k' $ de $ A'/\mathfrak{p}' $ est une extension quasi-galoisienne du corps des fractions $ k $ de $ A/(A \cap \mathfrak{p}') $, et l’homomorphisme canonique $ \sigma \to \bar{\sigma} $ de $ G^z(\mathfrak{p}') $ dans le groupe $ \Gamma $ des $ k $-automorphismes de $ k' $ définit, par passage au quotient, une bijection de $ G^z(\mathfrak{p}')/G^\Gamma(\mathfrak{p}') $ sur $ \Gamma $.

A) Supposons d’abord que $ K' $ soit une extension galoisienne de degré fini de $ K $. On a $ A = A' \cap K $ puisque $ A $ est intégralement clos, et $ A $ est donc l’anneau des invariants de $ G $ dans $ A' $. Comme $ G $ est fini, la proposition résulte dans ce cas du n° 2, th. 2.

B) Supposons en second lieu que $ K' $ soit une extension galoisienne quelconque de $ K $. Alors $ K' $ est une réunion d’une famille filtrante croissante $ (K_\alpha)_{\alpha \in I} $ d’extensions galoisiennes de degré fini de $ K $. Pour démontrer (i), considérons deux idéaux premiers $ \mathfrak{p}', q' $ de $ A' $ au-dessus de $ \mathfrak{p} $. Pour tout $ \alpha \in I $, $ \mathfrak{p}' \cap K_\alpha $ et $ q' \cap K_\alpha $ sont deux idéaux premiers de $ A' \cap K_\alpha $ au-dessus de $ \mathfrak{p} $. Puisque $ A' \cap K_\alpha $ est la fermeture intégrale de $ A $ dans $ K_\alpha $ et que les restrictions à $ K_\alpha $ des éléments de $ G $ forment le groupe des $ K $-automorphismes de $ K_\alpha $, il résulte du cas A) qu’il existe $ \sigma \in G $ tel que $ \sigma.(\mathfrak{p}' \cap K_\alpha) = q' \cap K_\alpha $. Soit $ E_\alpha $ l’ensemble des $ \sigma \in G $ qui possèdent cette dernière propriété. Soit $ \sigma \in G - E_\alpha $; alors, pour tout $ \tau \in G $ laissant invariants les éléments de $ K_\alpha $, on a $ (\sigma \tau).(\mathfrak{p}' \cap K_\alpha) = \sigma.(\mathfrak{p}' \cap K_\alpha) \neq q' \cap K_\alpha $, donc $ \sigma \tau \in G - E_\alpha $. Il en résulte que $ E_\alpha $ est fermé dans le groupe de Galois topologique $ G $ (Alg., chap. V, App. II, n° 1), et il est clair que la famille (ε_α)_{α∈I} est filtrante décroissante. Comme $ G $ est compact (*loc. cit.*, n° 2, prop. 3) et les $ ε_α $ non vides, l’intersection $ ε $ de la famille $ (ε_α) $ est non vide, et on a $ σ.p' = q' $ pour tout $ σ ∈ ε $, d’où (i).

Pour démontrer (ii), notons que $ k' $ est réunion de la famille filtrante croissante $ (k_α)_{α∈I} $, où $ k_α $ est le corps des fractions de $ (A' ∩ K_α)/(p' ∩ K_α) $. Comme chaque $ k_α $ est extension quasi-galoisienne de $ k $ en vertu de A), il en est de même de $ k' $ (*Alg.*, chap. V, § 6, n° 3, prop. 8). D’autre part, soit $ u $ un $ k $-automorphisme de $ k' $, et soit $ π': A' → A'/p' $ l’homomorphisme canonique. En vertu du n° 2, th. 2 appliqué à $ A' ∩ K_α $, il existe, pour tout $ α $, un ensemble non vide $ F_α $ d’éléments $ σ ∈ G $ tels que $ σ.(p' ∩ K_α) = p' ∩ K_α $ et $ u(π'(x)) = π'(σ.x) $ pour tout $ x ∈ A' ∩ K_α $. On voit comme ci-dessus que $ F_α $ est fermé dans $ G $, et comme $ (F_α) $ est une famille filtrante décroissante, son intersection $ F $ est non vide. Il est clair que pour $ σ ∈ F $, on a $ σ ∈ G^z(p') $ et $ \overline{σ} = u $, ce qui achève de prouver (ii) dans ce cas.

C) *Cas général.* — Le corps des invariants $ K_1 $ de $ G $ est une extension radicielle de $ K $ (*Alg.*, chap. V, § 10, n° 9, prop. 14); il existe donc un seul idéal premier $ p_1 $ de $ A_1 = A' ∩ K_1 $ au-dessus de $ p $ (lemme 4). Si $ p' $ et $ q' $ sont deux idéaux premiers de $ A' $ au-dessus de $ p $, ils sont par suite au-dessus de $ p_1 $; comme $ K' $ est une extension galoisienne de $ K_1 $ et que $ A' ∩ K_1 $ est intégralement clos (\$ 1, n° 2, prop. 7 et cor. de la prop. 8), il résulte de B) qu’il existe $ σ ∈ G $ tel que $ σ.p' = q' $; d’où (i). D’autre part, il est clair que le corps des fractions $ k_1 $ de $ A_1/p_1 $ est extension radicielle de $ k $ (A étant intégralement clos); comme $ k' $ est extension quasi-galoisienne de $ k_1 $ d’après B), $ k' $ est extension quasi-galoisienne de $ k $, tout $ k $-isomorphisme de $ k' $ dans une extension algébriquement close de $ k' $ étant un $ k_1 $-isomorphisme. Cette dernière remarque montre aussi, compte tenu de B), que tout $ k $-automorphisme de $ k' $ est de la forme $ \overline{σ} $ où $ σ ∈ G^z(p') $, ce qui achève de démontrer (ii).

C.Q.F.D.

#### Remarque 2 {#ac-v-s2-n3-rem-2 .statement}

Supposons que $ K' $ soit une extension *galoisienne* de $ K $ et gardons les notations de la démonstration de la prop. 6; pour tout $ α $, soit $ G^z_{α} $ (resp. $ G^T_{α} $) le sous-groupe de $ G $ formé des $ σ $ dont la restriction à $ A' ∩ K_α $ appartient à $ G^z(p' ∩ K_α) $ (resp. à $ G^T(p' ∩ K_α) $). La démonstration de la prop. 6 montre que ces sous-groupes sont *fermés* dans $ G $, et que

$$
G^z(p') = \bigcap_{α} G^z_{α} \quad \text{et} \quad G^T(p') = \bigcap_{α} G^T_{α}.
$$

En outre, l’ensemble des restrictions à $ A' \cap K_\alpha $ des éléments de $ G_z^\alpha $ (resp. $ G_T^\alpha $) est le groupe $ G_z(p' \cap K_\alpha) $ (resp. $ G_T(p' \cap K_\alpha) $) tout entier, tout K-automorphisme de $ K_\alpha $ se prolongeant en un élément de $ G $.

Sous les mêmes hypothèses, l’anneau $ A^z(p') $ (resp. $ A^T(p') $) est réunion de la famille filtrante des $ A^z(p' \cap K_\alpha) $ (resp. $ A^T(p' \cap K_\alpha) $) : en effet, tout $ x \in A^z(p') $ (resp. tout $ x \in A^T(p') $) appartient à un des $ K_\alpha $, et d’après ce qui précède, il existe un $ \beta $ tel que $ K_\alpha \subset K_\beta $ et que les restrictions à $ A' \cap K_\alpha $ des éléments de $ G_z(p') $ (resp. $ G_T(p') $) soient les mêmes que les restrictions à $ A' \cap K_\alpha $ des éléments de $ G_z(p' \cap K_\beta) $ (resp. $ G_T(p' \cap K_\beta) $), les groupes $ G_z(p' \cap K_\alpha) $ et $ G_T(p' \cap K_\beta) $ étant finis ; donc $ x $ appartient à $ A^z(p' \cap K_\beta) $ (resp. $ A^T(p' \cap K_\beta) $).

#### Corollaire 1 {#ac-v-s2-prop-6-cor-1 .statement}

Les hypothèses étant celles de la prop. 6, soient $ f $ un homomorphisme de $ A $ dans un corps $ L $, $ g_1, g_2 $ deux homomorphismes de $ A' $ dans $ L $ qui prolongent $ f $. Il existe alors un K-automorphisme $ \sigma $ de $ K' $ tel que $ g_1 = g_2 \circ \sigma $.

La démonstration à partir de la prop. 6 est la même que celle du cor. du th. 2 à partir de ce dernier.

#### Corollaire 2 {#ac-v-s2-prop-6-cor-2 .statement}

Soient $ A $ un anneau intégralement clos, $ K $ son corps des fractions, $ K' $ une extension algébrique de degré fini de $ K $, $ A' $ un sous-anneau de $ K' $ contenant $ A $ et entier sur $ A $.

(i) Pour tout idéal premier $ p $ de $ A $, l’ensemble des idéaux premiers de $ A' $ au-dessus de $ p $ est fini.

(ii) Si $ p' $ est un idéal premier de $ A' $ au-dessus de $ p $, tout élément de $ A'/p' $ est de degré $ \leq [K':K] $ sur le corps des fractions de $ A/p $.

(i) Soient $ K'' $ l’extension quasi-galoisienne de $ K $ engendrée par $ K' $ dans une clôture algébrique de $ K' $, $ A'' $ la fermeture intégrale de $ A $ dans $ K'' $. Le corps $ K'' $ est une extension de $ K $ de degré fini ($ Alg. $, chap. V, § 6, no 3, cor. 1 de la prop. 9), donc son groupe de K-automorphismes est fini ; il en résulte que l’ensemble des idéaux premiers de $ A'' $ au-dessus de $ p $ est fini (prop. 6, (i)). D’autre part, comme $ A'' $ est entier sur $ A' $, l’application $ p'' \to p'' \cap A' $ de l’ensemble des idéaux premiers de $ A'' $ au-dessus de $ p $ dans l’ensemble des idéaux premiers de $ A' $ au-dessus de $ x $ est surjective (no 1, th. 1).

(ii) Les coefficients du polynôme minimal (sur $ K $) d’un élément quelconque $ x' \in A' $ appartiennent à $ A $ ($ § 1 $, no 3, cor. de la prop. 10); en appliquant aux coefficients de ce polynôme l’homomorphisme canonique $ \pi': A' \to A'/p' $, on obtient pour la classe mod. $ \mathfrak{p}' $ de $ x $ une équation de dépendance intégrale à coefficients dans $ A/\mathfrak{p} $ et de degré $ \leq [K': K] $; d’où la conclusion.

#### Corollaire 3 {#ac-v-s2-prop-6-cor-3 .statement}

Les hypothèses et notations étant celles du cor. 2, si $ A $ est semi-local, il en est de même de $ A' $.

En effet, pour tout idéal maximal $ m' $ de $ A' $, $ m' \cap A $ est un idéal maximal de $ A $ (no 1, prop. 1); le corollaire résulte donc du cor. 2, puisque par hypothèse l’ensemble des idéaux maximaux de $ A $ est fini.

#### Corollaire 4 {#ac-v-s2-prop-6-cor-4 .statement}

Soient $ A $ un anneau intégralement clos, $ K $ son corps des fractions, $ K' $ une extension galoisienne de $ K $, $ A' $ la fermeture intégrale de $ A $ dans $ K' $, $ \mathfrak{p}' $ un idéal premier de $ A' $, $ \mathfrak{p} = A \cap \mathfrak{p}' $, $ k $ et $ k' $ les corps des fractions de $ A/\mathfrak{p} $ et $ A'/\mathfrak{p}' $ respectivement. Alors :

(i) Le corps des fractions de $ A^Z/(\mathfrak{p}' \cap A^Z) $ est égal à $ k $, et l’idéal maximal de l’anneau local de $ A^Z $ relatif à $ \mathfrak{p}' \cap A^Z $ est engendré par $ \mathfrak{p} $.

(ii) Le corps des fractions $ k^T $ de $ A^T/(\mathfrak{p}' \cap A^T) $ est la plus grande extension séparable de $ k $ contenue dans $ k' $.

L’anneau $ A $ est l’anneau des invariants dans $ A' $ du groupe de Galois de $ K' $ sur $ K $; lorsque $ K' $ est de degré fini sur $ K $, le corollaire résulte donc des prop. 4 et 5 du no 2. Considérons maintenant le cas général, $ K' $ étant donc réunion d’une famille filtrante croissante $ (K_\alpha) $ d’extensions galoisiennes de degré fini de $ K $. Alors :

(i) Si $ x, y $ sont deux éléments de $ A^Z $, avec $ y \in \mathfrak{p}' $, il y a un indice $ \alpha $ tel que $ x $ et $ y $ appartiennent à $ A^Z(\mathfrak{p}' \cap K_\alpha) $ (Remarque 2); en vertu de la prop. 4 du no 2, il y a $ x_0, y_0 $ dans $ A $, avec $ y_0 \in \mathfrak{p}' $, tels que $ xy_0 - x_0y \in \mathfrak{p}' $, ce qui prouve la première assertion de (i); si en outre $ x \in \mathfrak{p}' $, on peut supposer $ y_0 $ tel que

$$
xy_0 \in \mathfrak{p}A^Z(\mathfrak{p}' \cap K_\alpha) \subset \mathfrak{p}A^Z(\mathfrak{p}')
$$

ce qui démontre la seconde assertion de (i).

(ii) Supposons maintenant que $ x \in A^T $; il existe $ \alpha $ tel que $ x \in A^T(\mathfrak{p}' \cap K_\alpha) $ (Remarque 2) et la prop. 5 du no 2 montre que la classe $ \overline{x} $ de $ x $ mod. $ (\mathfrak{p}' \cap K_\alpha \cap A^T) $ est algébrique séparable sur $ k $; $ a fortiori $ la classe mod. $ (\mathfrak{p}' \cap A^T) $ de $ x $ est séparable sur $ k $; pour achever de prouver le corollaire, il suffit de montrer que $ k' $ est une extension radicielle de $ k^T $. Or, $ k' $ est réunion de la famille filtrante croissante des corps des fractions $ k_\alpha $ des anneaux $(A' \cap K_\alpha)/(p' \cap K_\alpha)$. Il résulte donc de la prop. 5 que si un élément de $ k' $ appartient à $ k_\alpha $, il est radiciel sur le corps des fractions de

$$
A^T(p' \cap K_\alpha)/(p' \cap A^T(p' \cap K_\alpha))
$$

et *a fortiori* sur $ k^T $ (en vertu de la *Remarque 2*).

#### Définition 5 {#ac-v-s2-def-5 .statement}

*Les hypothèses et notations étant celles de la prop. 6, le corps des invariants $ K^z(p') $ (resp. $ K^T(p') $) du groupe $ G^z(p') $ (resp. $ G^T(p') $) dans le corps $ K' $ s’appelle le corps de décomposition (resp. corps d’inertie) de $ p' $ par rapport à $ K $.

On écrit aussi $ K^z $ (resp. $ K^T $) au lieu de $ K^z(p') $ (resp. $ K^T(p') $). Il résulte du § 1, no 9, prop. 23 que $ K^z $ (resp. $ K^T $) est le *corps des fractions* de l’anneau $ A^z $ (resp. $ A^T $); $ A^z $ (resp. $ A^T $) est la fermeture intégrale de $ A $ dans $ K^z $ (resp. $ K^T $).

#### Remarque 3 {#ac-v-s2-n3-rem-3 .statement}

Sous les conditions du cor. 4 de la prop. 6, et en supposant $[K':K]\ fini$, le nombre des idéaux premiers distincts au-dessus de $ p $ est $[K^z:K]$, ce degré étant égal à l’indice $(G:G^z)$ en vertu de la théorie de Galois; en outre, il résulte de la théorie de Galois que l’on a

(6)
$$
[K^T:K^z] = (G^z:G^T) = [k^T:k].
$$

#### Remarque 4 {#ac-v-s2-n3-rem-4 .statement}

Soient $ A $ un anneau intégralement clos, $ K $ son corps des fractions, $ K' $ une extension algébrique de degré *fini* de $ K $, $ A' $ la fermeture intégrale de $ A $ dans $ K' $. Alors, pour tout idéal premier $ p $ de $ A $, *le nombre d’idéaux premiers de $ A' $ au-dessus de $ p $ est au plus* $[K':K]_s$ (facteur séparable du degré de $ K' $ sur $ K $). En effet, on peut d’abord se borner au cas où $ K' $ est une extension séparable de $ K $, car en général $ K' $ est extension radicielle de la plus grande extension séparable $ K_0 $ de $ K $ contenue dans $ K' $, on a $[K':K]_s = [K_0:K]$ par définition, et si $ A_0 $ est la fermeture intégrale de $ A $ dans $ K_0 $, les idéaux premiers de $ A_0 $ et de $ A' $ se correspondent biunivoquement (lemme 4). Supposons donc $ K' $ séparable sur $ K $, et soient $ N $ l’extension galoisienne de $ K $ engendrée par $ K' $ dans une clôture algébrique de $ K $, $ G $ son groupe de Galois, $ B $ la fermeture intégrale de $ A $ dans $ N $, $ \mathfrak{P} $ un idéal premier de $ B $ au-dessus de $ p $. Soient $ \mathcal{H} $ le groupe de Galois de $ N $ sur $ K' $, $ G^z $ le groupe de décomposition de $ \mathfrak{P} $; les idéaux premiers de $ B $ au-dessus de $ p $ sont les $ s.\mathfrak{P} $ pour $ s \in \mathcal{G} $ (no 2, th. 2), et la relation $ s.\mathfrak{P} = s'.\mathfrak{P} $ signifie que $ s' = sg $ où $ g \in \mathcal{G}^z $. D’autre part, pour que $ s.\mathfrak{P} \cap K' = s'.\mathfrak{P} \cap K' $, il faut et il suffit que $ s'.\mathfrak{P} = ts.\mathfrak{P} $, où $ t \in \mathcal{H} $ (no 2, th. 2), d’où finalement $ s' = tsg $ avec $ t \in \mathcal{H} $ et $ g \in \mathcal{G}^z $. Le nombre des idéaux premiers de $ A' $ au-dessus de $ \mathfrak{p} $ est donc égal au *nombre de classes de $ \mathcal{G} $ pour la relation d’équivalence* « *il existe* $ t \in \mathcal{H} $ *et* $ g \in \mathcal{G}^z $ *tels que* $ s' = tsg $ *entre* $ s $ *et* $ s' $; il est clair que ce nombre est au plus égal à l’indice $ (\mathcal{G} : \mathcal{H}) $, nombre de classes à droite de $ \mathcal{G} $ suivant $ \mathcal{H} $, et l’on a $ (\mathcal{G} : \mathcal{H}) = [K' : K] $ par la théorie de Galois.

#### Proposition 7 {#ac-v-s2-prop-7 .statement}

*Soient* $ A $ *un anneau intégralement clos*, $ K $ *son corps des fractions*, $ K' $ *une extension galoisienne de* $ K $, $ \mathcal{G} $ *son groupe de Galois*, $ A' $ *la fermeture intégrale de* $ A $ *dans* $ K' $, $ \mathfrak{p}' $ *un idéal premier de* $ A' $, $ \mathfrak{p} = A \cap \mathfrak{p}' $. *Enfin, soit* $ L $ *un sous-corps de* $ K' $ *contenant* $ K $, *et soit* $ \mathfrak{p}(L) = \mathfrak{p}' \cap L $.

(i) *Le corps de décomposition* (resp. *d’inertie*) *de* $ \mathfrak{p}' $ *par rapport à* $ L $ *est* $ L(K^z) $ (resp. $ L(K^T) $); *si en outre* $ L $ *est une extension galoisienne de* $ K $, *le corps de décomposition de* $ \mathfrak{p}(L) $ *par rapport à* $ K $ *est* $ L \cap K^z $.

(ii) *Si* $ L $ *est contenu dans* $ K^z $, $ A/\mathfrak{p} $ *et* $ (A' \cap L)/\mathfrak{p}(L) $ *ont même corps des fractions*, *et dans l’anneau local de* $ A' \cap L $ *correspondant à l’idéal premier* $ \mathfrak{p}(L) $, *l’idéal maximal est engendré par* $ \mathfrak{p} $. *Réciproquement, si ces deux conditions sont vérifiées, et si en outre* $ \bigcap_{n \geq 0} \mathfrak{p}^n A'_\mathfrak{p}' = 0 $, *L est contenu dans* $ K^z $.

(i) Si $ \mathcal{H} $ *est le sous-groupe de* $ \mathcal{G} $ *laissant invariants les éléments de* $ L $, *il est clair que le groupe de décomposition* (resp. *d’inertie*) *de* $ \mathfrak{p}' $ *par rapport à* $ L $ *est* $ \mathcal{G}^z \cap \mathcal{H} $ (resp. $ \mathcal{G}^T \cap \mathcal{H} $), *et la première assertion résulte de la théorie de Galois lorsque* $ K' $ *est une extension galoisienne* *finie* *de* $ K $ (*Alg.*, chap. V, § 10, no 6, cor. 1 du th. 3); *dans le cas général, elle découle de ce que* $ A^z $ (resp. $ A^T $) *est réunion des* $ A^z(\mathfrak{p}' \cap K_\alpha) $ (resp. $ A^T(\mathfrak{p}' \cap K_\alpha) $) *avec les notations de la Remarque 2*: tout élément $ x \in K' $ appartient à un $ K_\alpha $ *et s’il est invariant par* $ \mathcal{G}^z(\mathfrak{p}') \cap \mathcal{H} $ (resp. $ \mathcal{G}^T(\mathfrak{p}') \cap \mathcal{H} $) *il l’est aussi par* $ \mathcal{G}^z(\mathfrak{p}' \cap K_\beta) \cap \mathcal{H} $ (resp. $ \mathcal{G}^T(\mathfrak{p}' \cap K_\beta) \cap \mathcal{H} $) *pour un* $ \beta $ *convenable; donc il appartient d’après le début du raisonnement à* $ L(K^z(\mathfrak{p}' \cap K_\beta)) \subset L(K^z) $ (resp. à $ L(K^T(\mathfrak{p}' \cap K_\beta)) \subset L(K^T) $). *Supposons maintenant que* $ L $ *soit une extension galoisienne de* $ K $; *la restriction à* $ L $ *de tout* $ \sigma \in \mathcal{G}^z $ *laisse alors invariant* $ \mathfrak{p}(L) = \mathfrak{p}' \cap L $, *donc appartient au groupe de décomposition de* $ \mathfrak{p}(L) $ *par rapport à* $ K $. *Réciproquement, soit* $ \tau $ *un automorphisme de* $ L $ *appartenant à ce groupe, et soit* $ \sigma $ *un prolongement de* $ \tau $ *en un* $ K $*-automorphisme de* $ K' $;

posons $ q' = \sigma.p' $. Comme $ p' $ et $ q' $ sont tous deux au-dessus de $ \mathfrak{p}(L) $, il existe un automorphisme $ \rho \in \mathcal{H} $ tel que $ q' = \rho.p' $, d’où $ \rho^{-1}\sigma \in G^z $, et $ \tau $ est restriction de $ \rho^{-1}\sigma $ à $ L $; autrement dit, le groupe de décomposition de $ \mathfrak{p}(L) $ par rapport à $ K $ est identique au groupe des restrictions à $ L $ des automorphismes $ \sigma \in G^z $, ce qui démontre la seconde assertion.

(ii) Dire que $ L \subset K^z $ signifie que $ \mathcal{H} > G^z $, et les assertions de (ii) sont donc des cas particuliers du no 2, prop. 4, (ii) et (iii) lorsque $[K':K]$ est fini. Dans le cas général, on raisonne comme dans la démonstration de la prop. 6.

### 4. Deuxième théorème d’existence

#### Théorème 3 {#ac-v-s2-thm-3 .statement}

*Soient A un anneau intégralement clos, A' un anneau contenant A et entier sur A. On suppose que 0 est le seul élément de A qui soit diviseur de 0 dans A'. Soient p, q deux idéaux premiers de A tels que q ⊃ p, et q' un idéal premier de A' au-dessus de q. Alors il existe un idéal premier p' de A' au-dessus de p et tel que q' ⊃ p'*.

Supposons d’abord A' *intègre*. Soient K, K' les corps des fractions de A et A' respectivement; soient K'' la clôture algébrique de K' et A'' la fermeture intégrale de A dans K''; on a $ A \subset A' \subset A'' $. Soient $ p'' $ un idéal premier de A'' au-dessus de $ p $ (no 1, th. 1), $ q'' $ un idéal premier de A'' au-dessus de $ q $ et tel que $ p'' \subset q'' $ (no 1, cor. 2 du th. 1), enfin $ q'_1 $ un idéal premier de A'' au-dessus de $ q' $ (no 1, th. 1). En vertu du no 3, prop. 6, (i), il existe un K-automorphisme $ \sigma $ de K'' tel que $ \sigma.q'' = q'_1 $. Alors $ \sigma.p'' $ est un idéal premier de A'' au-dessus de $ p $ tel que $ \sigma.p'' \subset q'_1 $, donc $ p' = A' \cap \sigma.p'' $ est un idéal premier de A' au-dessus de $ p $ et contenu dans $ A' \cap q'_1 = q' $.

Passons au cas général. Comme A est intègre et $ q' $ premier, les parties $ A - \{0\} $ et $ A' - q' $ de A' sont multiplicatives; donc leur produit $ S = (A - \{0\})(A' - q') $ est une partie multiplicative de A', qui ne contient pas 0 puisque les éléments non nuls de A ne sont pas diviseurs de 0 dans A'. Il existe alors (chap. II, § 2, no 5, cor. 2 de la prop. 11) un idéal premier $ m' $ de A' disjoint de S, autrement dit tel que $ m' \subset q' $ et $ m' \cap A = 0 $. Soit $ h $ l’homomorphisme canonique $ A' \to A'/m' $. La restriction de $ h $ à A est injective, donc $ h(A) $ est intégralement clos. Comme $ m' \subset q' $, $ h(q') $ est un idéal premier de $ A'/m' $ au-dessus de $ h(q) $;

puisque $ A'/m' $ est intègre, la première partie de la démonstration prouve qu’il existe un idéal premier $ n' $ de $ A'/m' $ tel que $ n' \cap h(A) = h(p) $ et $ h(q') \supset n' $. L’idéal $ p' = h^{-1}(n') $ est un idéal premier de $ A' $, et on a $ q' \supset p' $, puisque $ q' $ contient le noyau de $ h $. Comme $ n' \supset h(p) $, on a $ p' \supset p $. Enfin, pour $ x \in p' \cap A $, on a $ h(x) \in n' \cap h(A) = h(p) $, donc $ x \in p $ puisque la restriction de $ h $ à $ A $ est injective; donc $ p' \cap A = p $.

C.Q.F.D.

#### Corollaire {#ac-v-s2-n4-cor-1 .statement}

Les hypothèses sur $ A $ et $ A' $ étant celles du th. 3, soit $ p $ un idéal premier de $ A $. Les idéaux premiers de $ A' $ au-dessus de $ p $ sont les éléments minimaux de l’ensemble $ \mathcal{E} $ des idéaux premiers de $ A' $ contenant $ pA' $.

En effet, un idéal premier de $ A' $ au-dessus de $ p $ est minimal dans $ \mathcal{E} $, en vertu du no 1, cor. 1 de la prop. 1. Inversement, soit $ q' $ un élément minimal de $ \mathcal{E} $. Comme $ q' \cap A \supset p $, le th. 3 montre qu’il existe un idéal premier $ p' $ de $ A' $ au-dessus de $ p $ tel que $ q' \supset p' $. Comme $ p' $ contient $ pA' $, l’hypothèse faite sur $ q' $ entraîne que $ q' = p' $, donc $ q' $ est au-dessus de $ p $.

\* Soient $ V, V' $ deux variétés algébriques affines, $ f $ un morphisme de $ V' $ dans $ V $ tel que $ f(V') $ soit dense dans $ V $. Soit $ A $ (resp. $ A' $) l’anneau des fonctions régulières sur $ V $ (resp. $ V' $); la donnée de $ f $ permet d’identifier $ A $ à un sous-anneau de $ A' $; supposons que $ A' $ soit entier sur $ A $. Le th. 1 du no 1 montre que pour toute sous-variété irréductible $ W $ de $ V $, il existe une sous-variété irréductible $ W' $ de $ V' $ telle que $ f(W') $ soit une partie dense de $ W $; en particulier tout point de $ V $ est l’image d’une sous-variété irréductible de $ V' $, ce qui montre que $ f $ est surjective. De même, la restriction de $ f $ à toute sous-variété irréductible $ W' $ de $ V' $ applique $ W' $ sur une sous-variété irréductible de $ V $. Le cor. 2 du th. 1, no 1, montre que si $ W $ et $ X $ sont deux sous-variétés irréductibles de $ V $ telles que $ W \supset X $, et si $ W' $ est une sous-variété irréductible de $ V' $ telle que $ f(W') = W $, alors il existe une sous-variété irréductible $ X' $ de $ V' $ contenue dans $ W' $ et telle que $ f(X') = X $.

Lorsque $ A $ est intégralement clos, on dit que $ V $ est normale. Le th. 3 montre que si $ V $ est normale, si $ W $ et $ X $ sont des sous-variétés irréductibles de $ V $ telles que $ W \supset X $, et si $ X' $ est une sous-variété irréductible de $ V' $ telle que $ f(X') = X $, alors il existe une sous-variété $ W' $ de $ V' $ contenant $ X' $ et telle que $ f(W') = W $. Enfin, le cor. du th. 3 montre que si $ V $ est normale et si $ W $ est une sous-variété irréductible de $ V $, les sous-variétés irréductibles $ W' $ de $ V' $ telles que $ f(W') = W $ ne sont autres que les composantes irréductibles de $ f^{-1}(W) $.*

## EXERCICES {#ac-v-s2-exercises}

See the [exercises for § 2](exercises/s2/).
