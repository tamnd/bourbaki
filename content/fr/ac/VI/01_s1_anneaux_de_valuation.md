---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: Valuations
section: 1
section_title: Anneaux de valuation
lang: fr
source: ac-v-vii-fr
pdf_pages: 0084-0091, 0164-0167
extraction: ocr
subsections:
    - "no": 1
      title: Relation de domination entre anneaux locaux
      page: 0
      pdf_page: 84
    - "no": 2
      title: Anneaux de valuation
      page: 0
      pdf_page: 85
    - "no": 3
      title: Caractérisation des éléments entiers
      page: 0
      pdf_page: 88
    - "no": 4
      title: Exemples d’anneaux de valuation
      page: 0
      pdf_page: 89
statements: 15
exercises: 8
content_sha256: 29cb15898721c3be9bccdf2016512aa6a79e9992ad47c59e809ddc412de5f25c
---

## § 1. Anneaux de valuation.

### 1. Relation de domination entre anneaux locaux

#### Définition 1 {#ac-vi-s1-def-1 .statement}

Soient A et B deux anneaux locaux. On dit que B domine A si A est un sous-anneau de B et si $ m(A) = A \cap m(B) $.

#### Proposition 1 {#ac-vi-s1-prop-1 .statement}

Soient A et B des anneaux locaux tels que A soit un sous-anneau de B. Les conditions suivantes sont équivalentes :

a) on a $ m(A) \subset m(B) $;
b) B domine A;
c) l’idéal $ Bm(A) $ engendré par $ m(A) $ dans B ne contient pas 1.

Si $ m(A) \subset m(B) $, $ m(B) \cap A $ est un idéal de A qui ne contient pas 1 et qui contient l’idéal maximal $ m(A) $; il lui est par suite égal, et $a)$ implique $b$. Si $B$ domine $A$, l’idéal $B_m(A)$ est contenu dans $m(B)$, donc ne contient pas 1; ainsi $b)$ implique $c$. Si $c)$ est satisfaite, $B_m(A)$ est contenu dans l’unique idéal maximal $m(B)$ de $B$, d’où $a$.

On notera que, si $K$ est un anneau, la relation « $B$ domine $A$ » est une *relation d’ordre* dans l’ensemble des sous-anneaux locaux de $K$.

Soient $A$ et $B$ deux anneaux locaux tels que $B$ domine $A$. L’injection canonique $A \to B$ définit, par passage aux quotients, un isomorphisme du corps $\kappa(A)$ sur un sous-corps de $\kappa(B)$; cet isomorphisme permet d’identifier $\kappa(A)$ à un sous-corps de $\kappa(B)$.

#### Exemple 1 {#ac-vi-s1-n1-exa-1 .statement}

Soient $A$ un anneau local noethérien, $\hat{A}$ son complété; l’anneau local $\hat{A}$ domine alors $A$ (Chap. III, § 3, no 5, prop. 9).

#### Exemple 2 {#ac-vi-s1-n1-exa-2 .statement}

Soient $B$ un anneau intègre, $A$ un sous-anneau de $B$, $\mathfrak{p}'$ un idéal premier de $B$, et $\mathfrak{p} = A \cap \mathfrak{p}'$. On a $\mathfrak{p}A_{\mathfrak{p}} \subset \mathfrak{p}'B_{\mathfrak{p}'}$, de sorte que $B_{\mathfrak{p}'}$ domine $A_{\mathfrak{p}}$.

### 2. Anneaux de valuation

#### Théorème 1 {#ac-vi-s1-thm-1 .statement}

*Soient $K$ un corps, et $V$ un sous-anneau de $K$. Les conditions suivantes sont équivalentes*:

$a)$ $V$ est un élément maximal de l’ensemble des sous-anneaux locaux de $K$, cet ensemble étant ordonné par la relation « $B$ domine $A$ » entre $A$ et $B$.

$b)$ *Il existe un corps algébriquement clos $L$, et un homomorphisme $h$ de $V$ dans $L$ qui est maximal dans l’ensemble des homomorphismes de sous-anneaux de $K$ dans $L$, ordonné par la relation « $g$ est un prolongement de $f$ » entre $f$ et $g$*.

$c)$ *Si $x \in K - V$, alors $x^{-1} \in V$*.

$d)$ *Le corps des fractions de $V$ est $K$, et l’ensemble des idéaux principaux de $V$ est totalement ordonné par la relation d’inclusion*.

$e)$ *Le corps des fractions de $V$ est $K$, et l’ensemble des idéaux de $V$ est totalement ordonné par la relation d’inclusion*.

Nous démontrerons le théorème suivant le schéma logique

$$
a) \implies b) \implies c) \implies d) \implies e) \implies a).
$$

Supposons $a)$ satisfaite. Alors $V$ est un anneau local. Soient $L$ une clôture algébrique du corps résiduel $\kappa(V)$, et $h$ l’homomorphisme canonique de V dans L. Soient V' un sous-anneau de K contenant V, et h' un homomorphisme de V' dans L prolongeant h. Si $ \mathfrak{p}' $ est le noyau de h', on a $ \mathfrak{p}' \cap V = m(V) $; donc (no 1, Exemple 2) $ V_{\mathfrak{p}'} $ domine V, ce qui entraîne $ V_{\mathfrak{p}'} = V $ et $ V' = V $. Ainsi b) est satisfaite.

Supposons b) satisfaite. Soient L un corps algébriquement clos, h un homomorphisme de V dans L; supposons h maximal dans l’ensemble des homomorphismes de sous-anneaux de K dans L; soit $ \mathfrak{p} $ le noyau de h. Les éléments de $ h(V - \mathfrak{p}) $ étant inversibles dans L, h se prolonge en un homomorphisme de $ V_{\mathfrak{p}} $ dans L (Chap. II, § 2, no 1, prop. 1); donc $ V = V_{\mathfrak{p}} $, ce qui montre que V est un anneau local, et que $ \mathfrak{p} $ est son idéal maximal. Soit x un élément non nul de K; il nous faut montrer que l’un au moins des éléments $ x, x^{-1} $ appartient à V, c’est-à-dire, en vertu du caractère maximal de h, que h peut être prolongé à $ V[x] $ ou à $ V[x^{-1}] $. Si x est entier sur V, ceci résulte du Chap. V, § 2, no 1, cor. 4 du th. 1. Si x n’est pas entier sur V, nous utiliserons le lemme suivant:

#### Lemme 1 {#ac-vi-s1-lem-1 .statement}

Soient A un sous-anneau d’un anneau B, x un élément de B non entier sur A; alors l’anneau de fractions $ B_x $ (chap. II, § 5, no 1) n’est pas réduit à 0, et il existe dans le sous-anneau $ A[1/x] $ de $ B_x $ des idéaux maximaux contenant $ 1/x $; en outre, si $ \mathfrak{M} $ est un quelconque de ces idéaux maximaux, l’image réciproque de $ \mathfrak{M} $ dans A est un idéal maximal.

Comme x n’est pas entier sur A, il n’est pas nilpotent et on a donc $ B_x \neq 0 $; en outre, on a $ x/1 \notin A[1/x] $, sans quoi on aurait une relation de la forme $ x/1 = a_0/1 + a_1/x + \cdots + a_n/x^n $ pour un $ n \geqslant 0 $ (avec $ a_i \in A $ pour $ 0 \leqslant i \leqslant n $), ce qui équivaut à

$$
x^{n+h} - a_0 x^{n+h-1} - a_1 x^{n+h-2} - \cdots - a_n x^{h-1} = 0
$$

pour un $ h \geqslant 1 $ convenable; mais une telle relation entraînerait que x est entier sur A, contrairement à l’hypothèse. L’existence d’un idéal maximal de $ A[1/x] $ contenant $ 1/x $ résulte donc de ce que $ 1/x $ n’est pas inversible dans $ A[1/x] $ (Alg., chap. I, § 8, no 7, th. 2).

Soit alors $ \mathfrak{M} $ un idéal maximal de $ A[1/x] $ contenant $ 1/x $; soient $ \varphi : A \to A[1/x] $, $ p : A[1/x] \to A[1/x]/\mathfrak{M} $ les homomorphismes canoniques; on a $ p(A[1/x]) = p(\varphi(A))[p(1/x)] = p(\varphi(A)) $ puisque $ p(1/x) = 0 $; cela prouve que $ p(\varphi(A)) $ est un corps, donc l’image réciproque $ \overline{\varphi}^{-1}(\mathfrak{M}) $ est un idéal maximal de A.

Appliquons ce lemme pour $ A = V $ et $ B = K $; il y a donc un idéal maximal $ \mathfrak{M} $ de $ V[x^{-1}] $ contenant $ x^{-1} $, et $ \mathfrak{M} \cap V $ est un idéal maximal de $ V $; on a $ \mathfrak{M} \cap V = \mathfrak{p} $ puisque $ V $ est local; notant $ f $ l’homomorphisme canonique de $ V[x^{-1}] $ sur $ V[x^{-1}]/\mathfrak{M} $, on a $ f(x^{-1}) = 0 $, d’où $ V/\mathfrak{p} = f(V) = f(V[x^{-1}]) $; comme $ h $ définit par passage au quotient un homomorphisme injectif $ \bar{h} $ de $ V/\mathfrak{p} $ dans $ L $, $ \bar{h} \circ f $ est un homomorphisme de $ V[x^{-1}] $ dans $ L $ prolongeant $ h $. Donc c) est satisfaite.

Supposons maintenant c) satisfaite. Il est clair que $ K $ est le corps des fractions de $ V $. Soient $ a $ et $ b $ des éléments de $ V $ tels que $ Va \not\subset Vb $; montrons que $ Vb \subset Va $. C’est vrai si $ b = 0 $; sinon la relation $ a \notin Vb $ entraîne $ b^{-1}a \notin V $, d’où, en vertu de c), $ a^{-1}b \in V $, et par suite $ Vb \subset Va $. Donc d) est satisfaite.

Supposons d) satisfaite. Soient $ a $ et $ b $ des idéaux de $ V $ tels que $ a \not\subset b $. Il existe $ a \in a $ tel que $ a \notin b $. Pour tout $ b \in b $ on a $ a \notin Vb $, d’où $ Va \not\subset Vb $, et par suite $ Vb \subset Va \subset a $ (d’après c)), et $ b \in a $. On a donc $ b \subset a $, ce qui montre que la condition e) est satisfaite.

Supposons enfin e) satisfaite. Comme $ V $ possède un idéal maximal, il n’en possède qu’un seul, et est donc un anneau local. Soit $ V' $ un sous-anneau local de $ K $ dominant $ V $, et soit $ x $ un élément non nul de $ V' $; posons $ x = ab^{-1} $ avec $ a \in V, \ b \in V $. L’un des idéaux $ Va, \ Vb $ est contenu dans l’autre. Si $ Va \subset Vb $, on a $ x \in V $. Si $ Vb \subset Va $, on a $ x^{-1} \in V $; comme l’idéal $ V'm(V) $ ne contient pas 1 (no 1, prop. 1), on a $ x^{-1} \notin m(V) $, d’où de nouveau $ x \in V $ puisque $ V $ est local. Tout élément de $ V' $ appartient donc à $ V $; on en conclut que a) est satisfaite.

#### Définition 2 {#ac-vi-s1-def-2 .statement}

Les notations étant celles du th. 1, on dit que $ V $ est un anneau de valuation pour le corps $ K $ si les conditions équivalentes a), b), c), d), e) sont satisfaites. On dit qu’un anneau est un anneau de valuation s’il est intègre et si c’est un anneau de valuation pour son corps des fractions.

#### Théorème 2 {#ac-vi-s1-thm-2 .statement}

Soient $ K $ un corps, et $ h $ un homomorphisme d’un sous-anneau $ A $ de $ K $ dans un corps algébriquement clos $ L $. Il existe alors un anneau de valuation $ V $ pour $ K $ et un homomorphisme $ h' $ de $ V $ dans $ L $ tels que $ V $ contienne $ A $, que $ h' $ prolonge $ h $ et que $ h'^{-1}(0) = m(V) $.

Soit $ \mathcal{H} $ l’ensemble des homomorphismes de sous-anneaux de $ K $ dans $ L $, ordonné par la relation de prolongement. Cet ensemble est inductif; en effet, si $ (h_\alpha)_{\alpha \in I} $ est une famille totalement ordonnée

#### Corollaire {#ac-vi-s1-n2-cor-1 .statement}

*Tout sous-anneau local A d’un corps K est dominé par au moins un anneau de valuation pour K.*

On applique le th. 2 à l’homomorphisme canonique $ h $ de $ A $ dans une clôture algébrique $ L $ de $ A/m(A) $.

### 3. Caractérisation des éléments entiers

#### Théorème 3 {#ac-vi-s1-thm-3 .statement}

*Soit A un sous-anneau d’un corps K. La fermeture intégrale $ A' $ de A dans K est l’intersection des anneaux de valuation pour K qui contiennent A; si A est local, $ A' $ est l’intersection des anneaux de valuation pour K qui dominent A.*

Soient $ x $ un élément de $ A' $, et $ V $ un anneau de valuation pour $ K $ contenant $ A $; comme $ x $ est entier sur $ V $, il existe un idéal premier $ \mathfrak{p}' $ de $ V[x] $ tel que $ \mathfrak{p}' \cap V = m(V) $ (Chap. V, § 2, n° 1, th. 1); il est clair qu’alors l’anneau local $ (V[x])_{\mathfrak{p}'} $ domine $ V $, donc lui est égal; d’où $ x \in V $. Inversement soit $ y $ un élément de $ K $ qui ne soit pas entier sur $ A $; il existe alors un idéal maximal $ \mathfrak{M} $ de $ A[y^{-1}] $ qui contient $ y^{-1} $ (n° 2, lemme 1); il existe aussi un anneau de valuation $ V $ pour $ K $ qui domine $ (A[y^{-1}])_{\mathfrak{M}} $ (n° 2, cor. du th. 2); comme $ y^{-1} \in m(V) $, on a $ y \notin V $. De plus $ \mathfrak{M} \cap A $ est un idéal maximal de $ A $ (n° 2, lemme 1); donc, si $ A $ est local, on a $ \mathfrak{M} \cap A = m(A) $, et $ V $ domine $ A $. C.Q.F.D.

#### Corollaire 1 {#ac-vi-s1-thm-3-cor-1 .statement}

*Tout anneau de valuation est intégralement clos.*

#### Corollaire 2 {#ac-vi-s1-thm-3-cor-2 .statement}

*Pour qu’un anneau intègre soit intégralement clos, il faut et il suffit qu’il soit l’intersection d’une famille d’anneaux de valuation pour son corps des fractions.*

COROLLAIRE 3. — Soient K un corps, K’ une extension de K, et A un anneau de valuation pour K. La fermeture intégrale de A dans K’ est l’intersection des anneaux de valuation V’ pour K’ tels que V’ ∩ K = A.

En effet le th. 1, c) montre que, si V’ est un anneau de valuation pour K’, V’ ∩ K est un anneau de valuation pour K, et V’ domine V’ ∩ K. Pour que V’ domine A, il est nécessaire et suffisant que V’ ∩ K domine A, donc lui soit égal.

### 4. Exemples d’anneaux de valuation

1) Tout corps est un anneau de valuation.

2) Si V’ est un anneau de valuation pour un corps K’, et si K est un sous-corps de K’, V’ ∩ K est, d’après le no 2, th. 1, c), un anneau de valuation pour K.

3) La proposition suivante fournit de nombreux exemples d’anneaux de valuation :

PROPOSITION 2. — Soit A un anneau local dont l’idéal maximal soit un idéal principal Ap. Si $ \bigcap_{n=1}^{\infty} Ap^n = (0) $ (par exemple si A est noethérien, cf. chap. III, § 3, no 2, cor. de la prop. 5), les seuls idéaux de A sont (0) et les Ap^n; alors, ou bien p est nilpotent, ou bien A est un anneau de valuation.

Filtrons en effet A par les Ap^n, et notons $ \nu $ la fonction d’ordre correspondante (chap. III, § 2, no 2). Comme

$$
\bigcap_{n=1}^{\infty} Ap^n = (0),
$$

la relation $ \nu(x) = + \infty $ implique $ x = 0 $. Soient $ a $ un idéal $ \neq (0) $ de A, et $ a $ un élément de $ a $ pour lequel $ \nu $ prenne sa plus petite valeur; posons $ \nu(a) = s $ ($ s \neq + \infty $). On a $ a \subset Ap^s $. En particulier, il existe $ u \in A $ tel que $ a = up^s $; comme $ a \notin Ap^{s+1} $, on a $ u \notin Ap $; donc $ u $ est inversible et l’on a $ p^s \in Aa \subset a $. Il en résulte que $ a = Ap^s $, d’où notre première assertion. On voit aussi que tout élément $ a \neq 0 $ de A s’écrit sous la forme $ a = up^{\nu(a)} $ avec $ u $ inversible. Si $ a' = u'p^{\nu(a')} $ ($ u' $ inversible) est un autre élément non nul de A, on a $ aa' = uu'p^{\nu(a)+\nu(a')} $; donc, si $ p $ n’est pas nilpotent, on a $ aa' \neq 0 $, et $ A $ est intègre. Alors, comme l’ensemble des idéaux de $ A $ est totalement ordonné par inclusion, on en conclut que $ A $ est un anneau de valuation (th. 1, e)).

C.Q.F.D.

Par exemple, si $ p $ est un nombre premier, l’anneau local $ \mathbf{Z}_{(p)} $ est un anneau de valuation. Soit $ B = K[X_1, \ldots, X_n] $ l’anneau des polynômes en $ n $ lettres sur un corps $ K $; l’idéal $ BX_1 $ est premier, puisque $ B/BX_1 $ est isomorphe à $ K[X_2, \ldots, X_n] $; donc $ B_{BX_1} $ est un anneau de valuation; il se compose des fractions rationnelles $ PQ^{-1} $, où $ P $ et $ Q $ sont des polynômes et où $ Q(0, X_2, \ldots, X_n) \neq 0 $.

\* Plus généralement, on verra que, si $ F $ est un élément extrémal de $ B = K[X_1, \ldots, X_n] $, $ B_{BF} $ est un anneau de valuation (cf. Chap. VII, § 3, no 5).*

L’anneau de séries formelles $ K[[T]] $ en une indéterminée sur un corps $ K $ est un anneau local intègre et noethérien dont l’idéal maximal est principal; c’est donc un anneau de valuation. Par contre l’anneau $ K[[T_1, T_2]] $ des séries formelles en deux indéterminées, qui est un anneau local intègre et noethérien, n’est pas un anneau de valuation, car aucun des éléments $ T_1, T_2 $ n’y est multiple de l’autre.

#### Proposition 3 {#ac-vi-s1-prop-3 .statement}

*Soient $ A $ un anneau principal et $ K $ son corps des fractions. Les anneaux de valuation pour $ K $ contenant $ A $ et distincts de $ K $ sont les anneaux de la forme $ A_{Ap} $, où $ p $ est un élément extrémal de $ A $.*

Il est clair que $ A_{Ap} $ ($ p $ extrémal) est un anneau de valuation contenant $ A $ et distinct de $ K $ (prop. 2). Inversement, soit $ V $ un anneau de valuation distinct de $ K $ et contenant $ A $. Comme $ V \neq K $, $ m(V) $ contient un élément $ x \neq 0 $; écrivant $ x = a/b $ avec $ a \in A $ et $ b \in A $ on voit que $ A \cap m(V) $ contient l’élément non nul $ a $. Comme $ A \cap m(V) $ est premier, il est de la forme $ Ap $ avec $ p $ extrémal dans $ A $. On a alors $ A_{Ap} \subset V $, $ pA_{Ap} \subset m(V) $, de sorte que $ V $ domine $ A_{Ap} $; comme $ A_{Ap} $ est un anneau de valuation pour $ K $ (prop. 2), on a $ V = A_{Ap} $.

#### Corollaire 1 {#ac-vi-s1-prop-3-cor-1 .statement}

*Tout anneau de valuation pour le corps $ \mathbf{Q} $ et distinct de $ \mathbf{Q} $ est de la forme $ \mathbf{Z}_{(p)} $ où $ p $ est un nombre premier.*

En effet tout sous-anneau de $ \mathbf{Q} $ contient $ \mathbf{Z} $.

#### Corollaire 2 {#ac-vi-s1-prop-3-cor-2 .statement}

*Soient $ K $ un corps, $ K(X) $ le corps des fractions rationnelles en une indéterminée sur $ K $, et $ V $ un anneau de valuation pour $ K(X) $ contenant $ K $ et distinct de $ K(X) $. Si $ X \in V $, il existe un polynôme irréductible $ P \in K[X] $ tel que $ V = (K[X])_{(P)} $; sinon $ V $ est l’anneau local de $ K[X^{-1}] $ en l’idéal premier $ X^{-1}K[X^{-1}] $ (autrement dit $ V $ se compose des fractions $ A/B $, où $ A \in K[X] $ et $ B \in K[X] $, telles que $ \deg(A) \leq \deg(B) $).

Si $ X \in V $, on a $ K[X] \subset V $, et l’assertion faite résulte de la prop. 3. Si $ X \notin V $, on a $ X^{-1} \in V $, d’où $ K[X^{-1}] \subset V $; alors $ V $ est l’anneau local de $ K[X^{-1}] $ en un idéal premier $ \mathfrak{p} $ (prop. 3), et cet idéal contient $ X^{-1} $ puisque $ X^{-1} $ n’est pas inversible dans $ V $; on a donc $ \mathfrak{p} = X^{-1}K[X^{-1}] $ puisque ce dernier idéal est maximal. Enfin considérons une fraction rationnelle $ A(X)/B(X) $, où $ A $ et $ B $ sont des polynômes, de degrés respectifs $ a $ et $ b $; on a $ A(X) = X^a A'(X^{-1}) $ et $ B(X) = X^b B'(X^{-1}) $, où $ A' $ et $ B' $ sont des polynômes tels que $ A'(0) \neq 0 $ et $ B'(0) \neq 0 $; donc, pour que $ A(X)/B(X) $ appartienne à l’anneau local de $ K[X^{-1}] $ en $ X^{-1}K[X^{-1}] $, il faut et il suffit qu’on ait $ a \leq b $.

## EXERCICES {#ac-vi-s1-exercises}

See the [exercises for § 1](exercises/s1/).
