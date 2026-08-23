---
book: ac
book_title: Commutative Algebra
chapter: V
chapter_title: Entiers
section: 1
section_title: Notion d’élément entier
lang: fr
source: ac-v-vii-fr
pdf_pages: 0005-0030, 0066-0073
extraction: ocr
subsections:
    - "no": 1
      title: Éléments entiers sur un anneau
      page: 0
      pdf_page: 5
    - "no": 2
      title: Fermeture intégrale d’un anneau. Anneaux intégralement clos
      page: 0
      pdf_page: 11
    - "no": 3
      title: Exemples d’anneaux intégralement clos
      page: 0
      pdf_page: 13
    - "no": 4
      title: Anneaux complètement intégralement clos
      page: 0
      pdf_page: 16
    - "no": 5
      title: Fermeture intégrale d’un anneau de fractions
      page: 0
      pdf_page: 18
    - "no": 6
      title: Normes et traces d’entiers
      page: 0
      pdf_page: 20
    - "no": 7
      title: Extension des scalaires dans une algèbre intégralement close
      page: 0
      pdf_page: 23
    - "no": 8
      title: '*Entiers sur un anneau gradué*'
      page: 0
      pdf_page: 25
    - "no": 9
      title: 'Application : invariants d’un groupe d’automorphismes d’une algèbre'
      page: 0
      pdf_page: 28
statements: 51
exercises: 19
content_sha256: 21feca5b44a18f4455d238751be0eb3a286059b83dcd196e3ef8f3297109515a
---

## § 1. Notion d’élément entier.

### 1. Éléments entiers sur un anneau

#### Théorème 1 {#ac-v-s1-thm-1 .statement}

Soient $ A $ un anneau (commutatif), $ R $ une algèbre sur $ A $ (non nécessairement commutative), $ x $ un élément de $ R $. Les propriétés suivantes sont équivalentes :
$ (E_I) $ $ x $ est racine d’un polynôme unitaire de l’anneau de polynômes $ A[X] $.
$ (E_{II}) $ La sous-algèbre $ A[x] $ de $ R $ est un $ A $-module de type fini.
$ (E_{III}) $ Il existe un module fidèle sur l’anneau $ A[x] $ qui est un $ A $-module de type fini.

Montrons d’abord que $ (E_I) $ entraîne $ (E_{II}) $. Soit
$$
X^n + a_1 X^{n-1} + \cdots + a_n
$$
un polynôme unitaire de $ A[X] $ ayant $ x $ pour racine; pour tout entier $ q \geqslant 0 $, soit $ M_q $ le sous-$ A $-module de $ R $ engendré par $ 1, x, \ldots, x^{n+q} $. On a
$$
x^{n+q} = -a_1 x^{n+q-1} - \cdots - a_n x^q \in M_{q-1}
$$

pour tout $ q \geqslant 1 $, d’où, par récurrence sur $ q $,
$$
M_q = M_{q-1} = \cdots = M_0.
$$
On en conclut que $ A[x] $ est égal à $ M_0 $ et est donc un $ A $-module de type fini.

Comme l’anneau commutatif $ A[x] $ est un module fidèle sur lui-même, $ (\mathrm{E}_{\mathrm{II}}) $ entraîne $ (\mathrm{E}_{\mathrm{III}}) $.

Enfin, le fait que $ (\mathrm{E}_{\mathrm{III}}) $ entraîne $ (\mathrm{E}_1) $ résultera du lemme plus précis suivant :

#### Lemme 1 {#ac-v-s1-lem-1 .statement}

*Soient $ A $ un anneau, $ R $ une algèbre (non nécessairement commutative) sur $ A $, $ x $ un élément de $ R $. Soit $ M $ un module fidèle sur $ A[x] $ qui soit un $ A $-module de type fini. Si $ q $ est un idéal de $ A $ tel que $ xM \subset qM $, alors $ x $ est racine d’un polynôme unitaire à coefficients dans $ A $, dont tous les coefficients autres que le coefficient dominant appartiennent à $ q $.

En effet, soit $ (u_i)_{1 \leq i \leq n} $ une famille finie d’éléments de $ M $ telle que $ M = \sum_{i=1}^n Au_i $. Pour tout $ i $, il existe par hypothèse une famille finie $ (q_{ij})_{1 \leq j \leq n} $ d’éléments de $ q $ telle que
$$
xu_i = \sum_{j=1}^n q_{ij}u_j \quad \text{pour} \quad 1 \leq i \leq n.
$$

Par suite (*Alg.*, chap. III, 3e éd., § 8), si $ d $ est le déterminant de la matrice $ (q_{ij} - \delta_{ij}x) $ à éléments dans $ A[x] $ ($ \delta_{ij} $ désignant l’indice de Kronecker), on a $ du_i = 0 $ pour tout $ i $, donc $ dM = 0 $; comme $ M $ est supposé être un $ A[x] $-module fidèle, on a nécessairement $ d = 0 $. Cela signifie que $ x $ est racine du polynôme $ \det(q_{ij} - \delta_{ij}X) $ de $ A[X] $ qui, au signe près, est un polynôme unitaire dont les coefficients autres que le coefficient dominant appartiennent à $ q $.

#### Définition 1 {#ac-v-s1-def-1 .statement}

*Soient $ A $ un anneau, $ R $ une $ A $-algèbre (non nécessairement commutative). On dit qu’un élément $ x \in R $ est entier sur $ A $ s’il vérifie les propriétés équivalentes $ (\mathrm{E}_1) $, $ (\mathrm{E}_{\mathrm{II}}) $, $ (\mathrm{E}_{\mathrm{III}}) $ du th. 1.

Une relation de la forme $ P(x) = 0 $, où $ P $ est un polynôme unitaire de $ A[X] $, est encore appelée *équation de dépendance intégrale* à coefficients dans $ A $.

#### Exemple 1 {#ac-v-s1-n1-exa-1 .statement}

Soient $ K $ un corps (commutatif), $ R $ une $ K $-algèbre; dire qu’un élément $ x \in R $ est entier sur $ K $ équivaut

#### Exemple 2 {#ac-v-s1-n1-exa-2 .statement}

Les éléments de $ \mathbf{Q}(i) $ entiers sur l’anneau $ \mathbf{Z} $ sont les éléments de la forme $ a + ib $ avec $ a \in \mathbf{Z} $ et $ b \in \mathbf{Z} $ (« entiers de Gauss »); les éléments de $ \mathbf{Q}(\sqrt{5}) $ entiers sur $ \mathbf{Z} $ sont les éléments de la forme $ (a + b\sqrt{5})/2 $, où $ a $ et $ b $ appartiennent à $ \mathbf{Z} $ et sont tous deux pairs ou tous deux impairs (pour ces deux exemples, voir exerc. 1).*

#### Exemple 3 {#ac-v-s1-n1-exa-3 .statement}

Les nombres complexes entiers sur $ \mathbf{Z} $ sont encore appelés entiers algébriques.

#### Remarque 1 {#ac-v-s1-n1-rem-1 .statement}

Soit $ A' $ le sous-anneau de $ R $ (contenu dans le centre de $ R $) image de $ A $ par l’homomorphisme d’anneaux $ A \to R $ qui définit la structure de $ A $-algèbre de $ R $. Il est clair qu’il est équivalent de dire qu’un élément de $ R $ est entier sur $ A $ ou qu’il est entier sur $ A' $.

#### Remarque 2 {#ac-v-s1-n1-rem-2 .statement}

Soit $ R' $ une sous-$ A $-algèbre de $ R $; les éléments de $ R' $ qui sont entiers sur $ A $ ne sont autres que les éléments de $ R $ qui sont entiers sur $ A $ et appartiennent à $ R' $; ceci permet souvent de ne pas spécifier l’algèbre à laquelle appartient un élément entier sur $ A $, lorsqu’il n’en résulte pas de confusion.

#### Proposition 1 {#ac-v-s1-prop-1 .statement}

Soient $ A $ un anneau, $ R $ une algèbre sur $ A $ (non nécessairement commutative), $ x $ un élément de $ R $. Pour que $ x $ soit entier sur $ A $, il faut et il suffit que $ A[x] $ soit contenu dans une sous-algèbre $ R' $ de $ R $ qui soit un $ A $-module de type fini.

La condition est évidemment nécessaire en vertu de la propriété (E_{II}); elle est suffisante en vertu de (E_{III}), car $ R' $ est un $ A[x] $-module fidèle (puisque’il contient l’élément unité de $ R $).

#### Corollaire {#ac-v-s1-n1-cor-1 .statement}

Soient $ A $ un anneau noethérien, $ R $ une $ A $-algèbre (non nécessairement commutative), $ x $ un élément de $ R $. Pour que $ x $ soit entier sur $ A $, il faut et il suffit qu’il existe un sous-$ A $-module de type fini de $ R $ contenant $ A[x] $.

En effet, la condition est nécessaire en vertu de (E_{II}); elle est suffisante, car si $ A[x] $ est un sous-$ A $-module d’un $ A $-module de type fini, il est lui-même un $ A $-module de type fini (Alg., chap. VIII, § 2, no 3, prop. 7).

On ne peut dans cet énoncé omettre l’hypothèse que $ A $ est noethérien (exerc. 2).

#### Définition 2 {#ac-v-s1-def-2 .statement}

Soit $ A $ un anneau. On dit qu’une $ A $-algèbre $ R $ (non nécessairement commutative) est entière sur $ A $ si tout élément de $ R $ est entier sur $ A $. On dit que $ R $ est finie sur $ A $ si $ R $ est un $ A $-module de type fini.

Il résulte de la prop. 1 que toute $ A $-algèbre finie est entière; lorsque $ R $ est commutative et est une $ A $-algèbre finie, $ R $ est évidemment une $ A $-algèbre de type fini, la réciproque étant inexacte.

#### Exemple 4 {#ac-v-s1-n1-exa-4 .statement}

Si $ M $ est un $ A $-module de type fini, l’algèbre $ \mathrm{End}_A(M) $ des endomorphismes de $ M $ est entière sur $ A $ en vertu de ($ E_{\mathrm{III}} $); en particulier, pour tout entier $ n $, l’algèbre de matrices $ \mathbf{M}_n(A) = \mathrm{End}_A(A^n) $ est entière (et même finie) sur $ A $.

#### Proposition 2 {#ac-v-s1-prop-2 .statement}

Soient $ A, A' $ deux anneaux, $ R $ une $ A $-algèbre, $ R' $ une $ A' $-algèbre (non nécessairement commutatives), $ f : A \to A' $ et $ g : R \to R' $ deux homomorphismes d’anneaux tels que le diagramme

$$
\begin{array}{ccc}
A & \xrightarrow{f} & A' \\
\downarrow & & \downarrow \\
R & \xrightarrow{g} & R'
\end{array}
$$

soit commutatif. Si un élément $ x \in R $ est entier sur $ A $, alors $ g(x) $ est entier sur $ A' $.

En effet, si l’on a $ x^n + a_1 x^{n-1} + \cdots + a_n = 0 $ avec $ a_i \in A $ pour $ 1 \leq i \leq n $, on en déduit que

$$
(g(x))^n + f(a_1)(g(x))^{n-1} + \cdots + f(a_n) = 0.
$$

#### Corollaire 1 {#ac-v-s1-prop-2-cor-1 .statement}

Soient $ A $ un anneau, $ B $ une $ A $-algèbre (commutative), $ C $ une $ B $-algèbre (non nécessairement commutative). Alors tout élément $ x \in C $ qui est entier sur $ A $ est entier sur $ B $.

#### Corollaire 2 {#ac-v-s1-prop-2-cor-2 .statement}

Soient $ K $ un corps, $ L $ une extension de $ K $, $ x, x' $ deux éléments de $ L $ conjugués sur $ K $ (Alg., chap. V, § 6, no 2). Si $ A $ est un sous-anneau de $ K $ et si $ x $ est entier sur $ A $, $ x' $ est aussi entier sur $ A $.

En effet, il existe un $ K $-isomorphisme $ f $ de $ K(x) $ sur $ K(x') $ tel que $ f(x) = x' $, et les éléments de $ A $ sont invariants par $ f $.

#### Corollaire 3 {#ac-v-s1-prop-2-cor-3 .statement}

Soient $ A $ un anneau, $ B $ une $ A $-algèbre (commutative), $ C $ une $ B $-algèbre (non nécessairement commutative). Si $ C $ est entière sur $ A $, $ C $ est entière sur $ B $.

#### Proposition 3 {#ac-v-s1-prop-3 .statement}

Soit $ (R_i)_{1 \leq i \leq n} $ une famille finie de $ A $-algèbres (non nécessairement commutatives) et soit $ R = \prod_{i=1}^n R_i $ leur produit. Pour qu’un élément $ x = (x_i)_{1 \leq i \leq n} $ de $ R $ soit entier sur $ A $, il faut et il suffit que chacun des $ x_i $ soit entier sur $ A $. Pour que $ R $ soit entière sur $ A $, il faut et il suffit que chacune des $ R_i $ soit entière sur $ A $.

Il suffit évidemment de prouver la première assertion. La condition est nécessaire en vertu de la prop. 2. Inversement, si chacun des $ x_i $ est entier sur $ A $, la sous-algèbre $ A[x_i] $ de $ R_i $ est un $ A $-module de type fini, donc il en est de même de la sous-algèbre $ \prod_{i=1}^n A[x_i] $ de $ R $; comme $ A[x] $ est contenue dans cette sous-algèbre, $ x $ est entier sur $ A $ en vertu de la prop. 1.

#### Proposition 4 {#ac-v-s1-prop-4 .statement}

Soient $ A $ un anneau, $ R $ une $ A $-algèbre (non nécessairement commutative), $ (x_i)_{1 \leq i \leq n} $ une famille finie d’éléments de $ R $, deux à deux permutables. Si, pour tout $ i $, $ x_i $ est entier sur $ A[x_1, \ldots, x_{i-1}] $ (et en particulier si tous les $ x_i $ sont entiers sur $ A $), alors la sous-algèbre $ A[x_1, \ldots, x_n] $ de $ R $ est un $ A $-module de type fini.

Raisonnons par récurrence sur $ n $, la proposition n’étant autre que $ (\mathrm{E}_{\mathrm{II}}) $ pour $ n = 1 $. L’hypothèse de récurrence entraîne que $ B = A[x_1, \ldots, x_{n-1}] $ est un $ A $-module de type fini; comme $ x_n $ est entier sur $ B $, $ B[x_n] = A[x_1, \ldots, x_n] $ est un $ B $-module de type fini, donc aussi un $ A $-module de type fini (*Alg.*, chap. II, 3e éd., § 1, no 13, prop. 25).

#### Corollaire 1 {#ac-v-s1-prop-4-cor-1 .statement}

Soient $ A $ un anneau, $ R $ une $ A $-algèbre (commutative). L’ensemble des éléments de $ R $ entiers sur $ A $ est une sous-algèbre de $ R $.

En effet, si $ x, y $ sont deux éléments de $ R $ entiers sur $ A $, il résulte de la prop. 4 que $ A[x, y] $ est un $ A $-module de type fini; comme il contient $ x + y $ et $ xy $, le corollaire résulte de la prop. 1.

Dans une algèbre non commutative, la somme et le produit de deux éléments entiers sur $ A $ ne sont pas nécessairement entiers sur $ A $ (exerc. 4).

COROLLAIRE 2. — Soient $ A $ un anneau, $ R $ une $ A $-algèbre (non nécessairement commutative), $ E $ un ensemble d’éléments de $ R $, deux à deux permutables et entiers sur $ A $. Alors la sous-$ A $-algèbre $ B $ de $ R $ engendrée par $ E $ est entière sur $ A $.

En effet, tout élément de $ B $ appartient à une sous-$ A $-algèbre de $ B $ engendrée par une partie finie de $ E $.

#### Remarque 3 {#ac-v-s1-n1-rem-3 .statement}

Il résulte de la prop. 4 que toute $ A $-algèbre commutative entière sur $ A $ est réunion d’une famille filtrante croissante de sous-algèbres finies sur $ A $.

PROPOSITION 5. — Soient $ A $ un anneau, $ A' $ et $ R $ deux $ A $-algèbres (commutatives). Si $ R $ est entière sur $ A $, $ R \otimes_A A' $ est entière sur $ A' $.

Considérons en effet un élément quelconque $ x' = \sum_{i=1}^n x_i \otimes a'_i $ de $ R \otimes_A A' $, où les $ x_i $ appartiennent à $ R $ et les $ a'_i $ à $ A' $; comme $ x_i \otimes a'_i = (x_i \otimes 1)a'_i $, et que les $ x_i \otimes 1 $ sont entiers sur $ A' $ (prop. 2), il en est de même de $ x $.

COROLLAIRE. — Soient $ R $ un anneau, $ A, B, C $ des sous-anneaux de $ R $ tels que $ A \subset B $. Si $ B $ est entier sur $ A $, $ C[B] $ est entier sur $ C[A] $.

En effet, $ B \otimes_A C[A] $ est entier sur $ C[A] $ en vertu de la prop. 5, donc il en est de même de l’image canonique $ C[B] $ de $ B \otimes_A C[A] $ dans $ R $ (considéré comme $ A $-algèbre) en vertu de la prop. 2.

PROPOSITION 6. — Soient $ A $ un anneau, $ B $ une $ A $-algèbre (commutative), $ C $ une $ B $-algèbre (non nécessairement commutative). Si $ B $ est entière sur $ A $ et si $ C $ est entière sur $ B $, alors $ C $ est entière sur $ A $.

Il suffit de voir que tout $ x \in C $ est entier sur $ A $. Par hypothèse, il existe un polynôme unitaire $ X^n + b_1 X^{n-1} + \cdots + b_n $ à coefficients dans $ B $, ayant $ x $ pour racine; alors $ x $ est entier sur $ B' = A[b_1, \ldots, b_n] $ et $ B'[x] $ est donc un $ B' $-module de type fini. Mais comme $ B $ est entière sur $ A $, $ B' $ est un $ A $-module de type fini (prop. 4); on en conclut que $ B'[x] $ est aussi un $ A $-module de type fini (\emph{Alg.}, chap. II, 3e éd., § 1, no 13, prop. 25), et par suite $ x $ est entier sur $ A $.

COROLLAIRE. — Soient $ A $ un anneau, $ R, R' $ deux $ A $-algèbres (commutatives) entières sur $ A $. Alors $ R \otimes_A R' $ est entière sur $ A $.

En effet, $ R \otimes_A R' $ est entière sur $ R' $ (prop. 5), donc la conclusion résulte de la prop. 6.

### 2. Fermeture intégrale d’un anneau. Anneaux intégralement clos

#### Définition 3 {#ac-v-s1-def-3 .statement}

Soient $ A $ un anneau, $ R $ une $ A $-algèbre (commutative). La sous-$ A $-algèbre $ A' $ de $ R $ formée des éléments de $ R $ entiers sur $ A $ (no 1, cor. 1 de la prop. 4) est appelée la fermeture intégrale de $ A $ dans $ R $. Si $ A' $ est égale à l’image canonique de $ A $ dans $ R $, on dit que $ A $ est intégralement fermé dans $ R $.

#### Remarque 1 {#ac-v-s1-n2-rem-1 .statement}

Si $ h : A \to R $ est l’homomorphisme d’anneaux définissant la structure de $ A $-algèbre de $ R $, la fermeture intégrale de $ A $ dans $ R $ est aussi celle de $ h(A) $ dans $ R $. D’autre part, si $ R' $ est une sous-algèbre de $ R $, la fermeture intégrale de $ A $ dans $ R' $ est $ A' \cap R' $.

#### Remarque 2 {#ac-v-s1-n2-rem-2 .statement}

Si $ A $ est un corps, la fermeture intégrale $ A' $ de $ A $ dans $ R $ est formée des éléments de $ R $ algébriques sur $ A $ (no 1, Exemple 1); généralisant la terminologie en usage pour les extensions de corps (Alg., chap. V, § 3, no 3), on dit encore alors que $ A' $ est la fermeture algébrique du corps $ A $ dans l’algèbre $ R $, et que $ A $ est algébriquement fermé dans $ R $ si $ A' = A $.

#### Définition 4 {#ac-v-s1-def-4 .statement}

Si $ A $ est un anneau intègre, on appelle clôture intégrale de $ A $ la fermeture intégrale de $ A $ dans son corps des fractions. On dit qu’un anneau est intégralement clos s’il est intègre et égal à sa clôture intégrale.

On notera qu’un anneau intégralement clos n’est pas nécessairement intégralement fermé dans un anneau qui le contient, comme le montre l’exemple d’un corps non algébriquement clos.

#### Proposition 7 {#ac-v-s1-prop-7 .statement}

Soient $ A $ un anneau, $ R $ une $ A $-algèbre. La fermeture intégrale $ A' $ de $ A $ dans $ R $ est un sous-anneau intégralement fermé dans $ R $.

En effet, la fermeture intégrale de $ A' $ dans $ R $ est entière sur $ A $ en vertu du no 1, prop. 6; elle est donc égale à $ A' $.

#### Corollaire {#ac-v-s1-n2-cor-1 .statement}

La clôture intégrale d’un anneau intègre $ A $ est un anneau intégralement clos.

En effet, soient K le corps des fractions de A, B la clôture intégrale de A. Il est clair que K est le corps des fractions de B, et il suffit d’appliquer la prop. 7 à R = K.

#### Proposition 8 {#ac-v-s1-prop-8 .statement}

Soient R un anneau, (B_\lambda)_{\lambda \in L} une famille de sous-anneaux de R et pour chaque \lambda \in L, soit A_\lambda un sous-anneau de B_\lambda. Si chaque A_\lambda est intégralement fermé dans B_\lambda, alors $ A = \bigcap_{\lambda \in L} A_\lambda $ est intégralement fermé dans $ B = \bigcap_{\lambda \in L} B_\lambda $.

Cela résulte aussitôt de la déf. 3 et du n° 1, cor. 1 de la prop. 2.

#### Corollaire {#ac-v-s1-n2-cor-2 .statement}

Toute intersection d’une famille non vide de sous-anneaux intégralement clos d’un anneau intègre est un anneau intégralement clos.

Soit A l’intersection d’une telle famille $(A_\lambda)_{\lambda \in L}$ de sous-anneaux d’un anneau intègre C. D’après la prop. 8, appliquée en prenant pour R (resp. B_\lambda) le corps des fractions de C (resp. de A_\lambda), A est intégralement fermé dans le corps $ B = \bigcap_{\lambda \in L} B_\lambda $ et *a fortiori* est intégralement clos.

#### Proposition 9 {#ac-v-s1-prop-9 .statement}

Soient A un anneau, $(R_i)_{1 \leq i \leq n}$ une famille finie de A-algèbres, $A'_i$ la fermeture intégrale de A dans $R_i$ ($1 \leq i \leq n$). Alors la fermeture intégrale de A dans $R = \prod_{i=1}^n R_i$ est égale à $\prod_{i=1}^n A'_i$.

C’est une conséquence immédiate du n° 1, prop. 3.

#### Corollaire 1 {#ac-v-s1-prop-9-cor-1 .statement}

Soient A un anneau noethérien réduit, $p_i$ ($1 \leq i \leq n$) ses idéaux premiers minimaux distincts, $K_i$ le corps des fractions de l’anneau intègre $A/p_i$ (canoniquement isomorphe à l’anneau local $A_{p_i}$ (chap. IV, § 2, n° 5, prop. 10)), $A'_i$ la fermeture intégrale de A dans $K_i$ ($1 \leq i \leq n$). Alors l’isomorphisme canonique de l’anneau total des fractions B de A sur $\prod_{i=1}^n K_i$ (loc. cit.) applique la fermeture intégrale de A dans B sur l’anneau produit $\prod_{i=1}^n A'_i$.

#### Corollaire 2 {#ac-v-s1-prop-9-cor-2 .statement}

Pour qu’un anneau noethérien réduit soit intégralement fermé dans son anneau total des fractions il faut et il suffit qu’il soit composé direct d’anneaux (noethériens) intégralement clos (donc intègres).

### 3. Exemples d’anneaux intégralement clos

#### Proposition 10 {#ac-v-s1-prop-10 .statement}

Tout anneau principal est intégralement clos.

Soient A un anneau principal, K son corps des fractions, x un élément de K. Il existe deux éléments étrangers a, b de A tels que $ x = ab^{-1} $ (Alg., chap. VII, § 1, no 2, prop. 1 et chap. VI, § 1, no 11, prop. 9 (DIV)). Si x est entier sur A, il est racine d’un polynôme $ X^n + c_1 X^{n-1} + \cdots + c_n $ de A[X]. On a alors $ a^n = b(-c_1 a^{n-1} - \cdots - c_n b^{n-1}) $, ce qui prouve que b divise $ a^n $. Puisque a et b sont étrangers, cela implique que b est inversible dans A (Alg., chap. VI, § 1, no 12, cor. 1 de la prop. 11 (DIV)); donc $ x \in A $.

#### Lemme 2 {#ac-v-s1-lem-2 .statement}

Soient R un anneau, P un polynôme unitaire dans R[X]. Il existe un anneau R’ contenant R tel que, dans l’anneau de polynômes R'[X], le polynôme P soit produit de polynômes unitaires de degré 1.

Procédons par récurrence sur le degré n de P, le lemme étant évident pour $ n = 0 $ et $ n = 1 $. Supposons donc $ n > 1 $. Soit a l’idéal de R[X] engendré par P, et soit f l’homomorphisme canonique de R[X] sur B = R[X]/a. Puisque P est unitaire, on a, pour tout polynôme Q $ \in R[X] $, $ \deg(PQ) = \deg(P) + \deg(Q) $, d’où $ a \cap R = 0 $; la restriction de f à R est donc injective. Identifiant R au sous-anneau $ f(R) $ de B au moyen de f, et posant $ b = f(X) $, on voit que b est une racine de P dans B, P étant considéré comme un polynôme de B[X]. Il existe donc un polynôme unitaire Q de B[X], de degré $ n-1 $, tel que $ P(X) = (X-b)Q(X) $ (Alg., chap. IV, § 1, no 4, prop. 5). En vertu de l’hypothèse de récurrence, il existe un anneau R’ ⊃ B tel que, dans R'[X], le polynôme Q soit un produit de polynômes unitaires de degré 1; il est clair que dans R'[X], P est alors produit de polynômes unitaires de degré 1.

#### Proposition 11 {#ac-v-s1-prop-11 .statement}

Soient A un anneau, R une A-algèbre, P et Q deux polynômes unitaires dans R[X]. Si les coefficients de PQ sont entiers sur A, les coefficients de P et de Q sont entiers sur A.

Par double application du lemme 2, on voit qu’il existe un anneau R’ contenant R et des familles d’éléments $ (a_i)_{1 \leq i \leq m} $, (b_j)_{1 \leq j \leq n} de R' telles que, dans R'[X], on ait P[X] = \prod_{i=1}^{m} (X - a_i), Q(X) = \prod_{j=1}^{n} (X - b_j); les coefficients de PQ appartiennent à la fermeture intégrale A' de A dans R', donc (no 2, prop. 7) les éléments $ a_i (1 \leq i \leq m) $ et $ b_j (1 \leq j \leq n) $ appartiennent à A'. Il en résulte que les coefficients de P et Q sont entiers sur A (no 1, cor. 1 de la prop. 4).

Soient A un anneau intègre, K son corps des fractions, K' une K-algèbre (non nécessairement commutative). Étant donné un élément $ x \in K' $ algébrique sur K, les polynômes $ P \in K[X] $ tels que $ P(x) = 0 $ forment un idéal $ a \neq 0 $ de $ K[X] $, nécessairement principal (Alg., chap. IV, § 1, no 5, prop. 7). Il existe un polynôme unitaire et un seul qui engendre a; généralisant la terminologie introduite en Alg., chap. V, § 3, no 1, déf. 3, nous dirons que ce polynôme unitaire est le polynôme minimal de $ x $ sur K.

COROLLAIRE. — Soient A un anneau intègre, K son corps des fractions, x un élément d’une K-algèbre K' (non nécessairement commutative). Si x est entier sur A, les coefficients du polynôme minimal P de x sur K sont entiers sur A (et ils appartiennent donc à A si A est intégralement clos).

Il existe par hypothèse (no 1, th. 1) un polynôme unitaire $ Q \in A[X] $ tel que $ Q(x) = 0 $. Comme P divise Q dans $ K[X] $, il résulte de la prop. 11 que les coefficients de P sont entiers sur A.

Soient A un anneau, R une A-algèbre (commutative); l’homomorphisme $ \varphi : A \to R $ définissant la structure de A-algèbre de R se prolonge d’une seule manière en un homomorphisme $ A[X] \to R[X] $ des anneaux de polynômes sur A et R, laissant X invariant, donc $ R[X] $ est canoniquement muni d’une structure de $ A[X] $-algèbre.

PROPOSITION 12. — Soient A un anneau, R une A-algèbre, P un polynôme dans $ R[X_1, \ldots, X_n] $. Pour que P soit entier sur $ A[X_1, \ldots, X_n] $, il faut et il suffit que les coefficients de P soient entiers sur A.

En considérant les polynômes de $ R[X_1, \ldots, X_n] $ comme des polynômes en $ X_n $, à coefficients dans $ R[X_1, \ldots, X_{n-1}] $, on voit aussitôt qu’on est ramené à démontrer la proposition pour $ n = 1 $. Soit donc P un polynôme de $ R[X] $; il résulte aussitôt du no 1, prop. 5 que si les coefficients de P sont dans la fermeture intégrale B de A dans R, l’élément P, qui appartient à B[X] = B ⊗_A A[X], est entier sur A[X]. Inversement, supposons que P soit entier sur A[X], et soit

$$
Q(Y) = Y^m + F_1 Y^{m-1} + \cdots + F_m
$$

un polynôme unitaire à coefficients $ F_i \in A[X] $ admettant P pour racine. Soit $ r $ un entier strictement supérieur à tous les degrés des polynômes P et $ F_i (1 \leq i \leq m) $, et posons

$$
P_1(X) = P(X) - X^r.
$$

Alors $ P_1 $ est racine du polynôme

$$
Q_1(Y) = Q(Y + X^r) = Y^m + G_1 Y^{m-1} + \cdots + G_m
$$

à coefficients dans $ A[X] $; on peut donc écrire

(1)
$$
- P_1(P_1^{m-1} + G_1 P_1^{m-2} + \cdots + G_{m-1}) = G_m.
$$

Or le choix de $ r $ implique que — $ P_1 $ est un polynôme *unitaire* de $ R[X] $ et il en est de même de $ G_m(X) = Q(X^r) $, les degrés des polynômes $ F_k(X) X^{r(m-k)} $ étant tous $ < rm $ pour $ k \geq 1 $. On en conclut tout d’abord que le polynôme

$$
P_1^{m-1} + G_1 P_1^{m-2} + \cdots + G_{m-1}
$$

de $ R[X] $ est aussi unitaire; en outre, comme les coefficients de $ G_m $ appartiennent à A, la prop. 11 montre que $ P_1 $ a ses coefficients entiers sur A, et les coefficients de P sont donc bien entiers sur A.

#### Proposition 13 {#ac-v-s1-prop-13 .statement}

*Soient A un anneau, R une A-algèbre, A' la fermeture intégrale de A dans R. Alors la fermeture intégrale de A[X_1, ..., X_n] dans R[X_1, ..., X_n] est égale à A'[X_1, ..., X_n].*
Cela résulte de la prop. 12 et de la déf. 3 du no 2.

#### Corollaire 1 {#ac-v-s1-prop-13-cor-1 .statement}

*Soient A un anneau intègre, A' sa clôture intégrale. Alors la clôture intégrale de l’anneau de polynômes A[X_1, ..., X_n] est A'[X_1, ..., X_n].*

En raisonnant par récurrence sur $ n $, on est aussitôt ramené au cas $ n = 1 $. Soit K le corps des fractions de A, qui est aussi celui de $ A' $; si un élément P du corps des fractions K(X) de A[X] est entier sur A[X], il appartient à l’anneau de polynômes K[X], car ce dernier est principal (*Alg.*, chap. IV, § 1, no 5, prop. 7), donc intégralement clos (prop. 10); le corollaire résulte donc de la prop. 13 appliquée à $ R = K $.

COROLLAIRE 2. — Soit $ A $ un anneau intègre. Pour que l’anneau de polynômes $ A[X_1, \ldots, X_n] $ soit intégralement clos, il faut et il suffit que $ A $ soit intégralement clos.

COROLLAIRE 3. — Si $ K $ est un corps, toute algèbre de polynômes $ K[X_1, \ldots, X_n] $ est un anneau intégralement clos.

### 4. Anneaux complètement intégralement clos

DÉFINITION 5. — On dit qu’un anneau $ A $ est complètement intégralement clos s’il est intègre, et si la condition suivante est vérifiée : tout élément $ x $ du corps des fractions $ K $ de $ A $ tel que toutes les puissances $ x^n $ ($ n \geqslant 0 $) soient contenues dans un sous-A-module de type fini de $ K $, appartient à $ A $.

On notera que l’hypothèse que les $ x^n $ sont contenus dans un sous-A-module de type fini de $ K $ s’exprime encore en disant qu’il existe un élément non nul $ d \in A $ tel que $ dx^n \in A $ pour tout $ n \geqslant 0 $; en effet, cette dernière condition signifie que $ x^n \in Ad^{-1} $; et inversement, si $ (b_i)_{1 \leqslant i \leqslant m} $ est une suite finie d’éléments de $ K $, il existe $ d \in A $ tel que $ db_i \in A $ pour $ 1 \leqslant i \leqslant m $, d’où $ dM \subset A $ pour le sous-A-module $ M $ de $ K $ engendré par les $ b_i $.

Il est clair qu’un anneau complètement intégralement clos est intégralement clos; inversement, le cor. de la prop. 1 du no 1 montre qu’un anneau noethérien intégralement clos est complètement intégralement clos. *Par contre, un anneau de valuation de hauteur $ \geqslant 2 $ (chap. VI, § 4, no 4) est intégralement clos mais non complètement intégralement clos.* Si $ (A_i) $ est une famille d’anneaux complètement intégralement clos ayant même corps des fractions $ K $, $ A = \bigcap_i A_i $ est complètement intégralement clos.
En effet, si $ x \in K $ est tel que, pour un $ d $ non nul dans $ A $, $ dx^n $ appartienne à $ A $ pour tout $ n > 0 $, l’hypothèse entraîne que $ x \in A_i $ pour tout $ i $, donc $ x \in A $.

PROPOSITION 14. — Soit $ A $ un anneau complètement intégralement clos. Alors tout anneau de polynômes $ A[X_1, \ldots, X_n] $ (resp. tout anneau de séries formelles $ A[[X_1, \ldots, X_n]] $) est complètement intégralement clos.

Par récurrence sur $ n $, il suffit de prouver que $ A[X] $ (resp. $ A[[X]] $) est complètement intégralement clos. Soit donc $ P $ un élément du corps des fractions de $ A[X] $ (resp. $ A[[X]] $) et supposons

C.Q.F.D.

#### Proposition 15 {#ac-v-s1-prop-15 .statement}

Soit $ A $ un anneau filtré dont la filtration est exhaustive, et tel que tout idéal principal de $ A $ soit fermé pour la topologie définie par la filtration. Si l’anneau gradué associé $ \mathrm{gr}(A) $ (chap. III, § 2, no 3) est complètement intégralement clos, alors $ A $ est complètement intégralement clos.

Soit $ (A_n)_{n \in \mathbf{Z}} $ la filtration de $ A $; comme $ \bigcap_{n \in \mathbf{Z}} A_n $ est l’adhérence de l’idéal (0) (chap. III, § 2, no 5), l’hypothèse implique d’abord que la filtration $ (A_n) $ est séparée, et comme $ \mathrm{gr}(A) $ est intègre, il en est donc de même de $ A $ (chap. III, § 2, no 3, cor. de la prop. 1). Soit $ x = b/a $ un élément du corps des fractions $ K $ de $ A $ ($ a \in A, b \in A $) pour lequel il existe un élément $ d \neq 0 $ de $ A $ tel que $ dx^n \in A $ pour tout $ n \geqslant 0 $. Il s’agit de prouver que $ b \in Aa $, et comme par hypothèse l’idéal $ Aa $ est fermé, il suffit de montrer que pour tout $ n \in \mathbf{Z} $ on a $ b \in Aa + A_n $. Comme la filtration de $ A $ est exhaustive, il existe un entier $ q \in \mathbf{Z} $ tel que $ b \in Aa + A_q $. Il suffira donc de prouver que la relation $ b \in Aa + A_m $ implique $ b \in Aa + A_{m+1} $.

Supposons donc que $ b = ay + z $ avec $ y \in A, z \in A_m $. On a par hypothèse $ dx^n \in A $ pour tout $ n \geqslant 0 $, d’où on tire aussitôt

C.Q.F.D.

### 5. Fermeture intégrale d’un anneau de fractions

Soient A un anneau, R une A-algèbre, S une partie multiplicative de A. Rappelons (chap. II, § 2, no 8) que S^{-1}R est canoniquement muni d’une structure de S^{-1}A-algèbre.

PROPOSITION 16. — Soient A un anneau, R une A-algèbre, A' la fermeture intégrale de A dans R, S une partie multiplicative de A. Alors la fermeture intégrale de S^{-1}A dans S^{-1}R est S^{-1}A'.

Soit b/s un élément de S^{-1}A' (s \in S, b \in A'). Puisque le diagramme

$$
\begin{array}{ccc}
A & \xrightarrow{i_A^S} & S^{-1}A \\
h \downarrow & & \downarrow S^{-1}h \\
R & \xrightarrow{i_R^S} & S^{-1}R
\end{array}
$$

est commutatif, b/1 est entier sur S^{-1}A (no 1, prop. 2). Comme 1/s \in S^{-1}A, b/s = (b/1)(1/s) est entier sur S^{-1}A.

Inversement, soit r/t (r \in R, t \in S) un élément de S^{-1}R entier sur S^{-1}A; alors r/1 = (t/1)(r/t) est entier sur S^{-1}A. On a par suite une relation de la forme

$$(r/1)^n + (a_1/s)(r/1)^{n-1} + \cdots + (a_n/s) = 0,$$

avec $ a_i \in A $ ($ 1 \leq i \leq n $) et $ s \in S $. Cette relation s’écrit aussi
$$
(sr^n + a_1 r^{n-1} + \cdots + a_n)/s = 0
$$
et par suite il existe $ s' \in S $ tel que $ s'(sr^n + a_1 r^{n-1} + \ldots + a_n) = 0 $; on en déduit que $ (s'sr)^n + s'a_1(s'sr)^{n-1} + \cdots + s'^n s^{n-1} a_n = 0 $. Par définition, on a donc $ s'sr \in A' $, d’où $ r/1 \in S^{-1}A' $ et $ r/t \in S^{-1}A' $.

#### Corollaire 1 {#ac-v-s1-prop-15-cor-1 .statement}

*Soient A un anneau intègre, A' sa clôture intégrale, S une partie multiplicative de A telle que $ 0 \notin S $. Alors la clôture intégrale de $ S^{-1}A $ est $ S^{-1}A' $.*

En effet, le corps des fractions R de A est aussi le corps des fractions de $ S^{-1}A $ puisque $ 0 \notin S $ (chap. II, § 1, no 1, Remarque 7); on applique à R la prop. 16.

#### Corollaire 2 {#ac-v-s1-prop-15-cor-2 .statement}

*Soient A un anneau intègre, K son corps des fractions, R une algèbre sur K, B la fermeture intégrale de A dans R. Les éléments de R algébriques sur K (no 1, Exemple 1) sont les éléments de la forme $ a^{-1} b $ où $ b \in B $ et $ a \in A $, $ a \neq 0 $; si L est la fermeture algébrique de K dans R, il existe une base de L sur K contenue dans B.*

La première assertion résulte de la prop. 16 appliquée au cas où $ S = A - \{0\} $. Si $ (x_i)_{i \in I} $ est une base de L sur K, il existe donc pour tout $ i \in I $ un élément $ a_i \neq 0 $ de A tel que $ a_i x_i \in B $; alors $ (a_i x_i)_{i \in I} $ est aussi une base de L sur K.

#### Corollaire 3 {#ac-v-s1-prop-15-cor-3 .statement}

*Soient A un anneau intègre, $ \Omega $ l’ensemble des idéaux maximaux de A. Pour que A soit intégralement clos, il faut et il suffit que, pour tout $ m \in \Omega $, $ A_m $ soit intégralement clos.*

Il résulte du cor. 1 que la condition est nécessaire. La condition est suffisante, car on a $ A = \bigcap_{m \in \Omega} A_m $ (chap. II, § 3, no 3, formule (2)), et il suffit d’appliquer le cor. de la prop. 8 du no 2.

#### Corollaire 4 {#ac-v-s1-prop-15-cor-4 .statement}

*Soient A un anneau intègre, K son corps des fractions, S une partie multiplicative de A telle que $ 0 \notin S $.*
(i) *Soient B un sous-anneau de K entier sur A, et soit $ f $ l’annulateur du A-module B/A. Alors $ S^{-1}f $ est contenu dans l’annulateur du $ (S^{-1}A)$-module $ S^{-1}B/S^{-1}A $, et est égal à cet annulateur lorsque B est un A-module de type fini.*
(ii) *Soit A' la clôture intégrale de A. Pour que $ S^{-1}A $ soit intégralement clos, il suffit que l’annulateur $ f $ du A-module $ A'/A $ rencontre S. Cette condition est aussi nécessaire lorsque A' est un A-module de type fini.*

(ii) En vertu du cor. 1, $ S^{-1}A' $ est la clôture intégrale de $ S^{-1}A $. Comme les relations $ f \cap S \neq \emptyset $ et $ S^{-1}f = S^{-1}A $ sont équivalentes (chap. II, § 2, no 5, Remarque) (ii) est une conséquence immédiate de (i).

Lorsque $ B $ est un sous-anneau de $ K $ entier sur $ A $, on dit parfois que l’annulateur $ f $ de $ B/A $ (égal par définition au transporteur $ A:B $ (chap. I, § 2, no 10)) est le conducteur de $ B $ dans $ A $.

COROLLAIRE 5. — Soient $ A $ un anneau intègre, $ A' $ sa clôture intégrale, et $ f $ l’annulateur du $ A $-module $ A'/A $. Supposons que $ A' $ soit un $ A $-module de type fini. Les idéaux premiers $ \mathfrak{p} $ de $ A $ tels que $ A_{\mathfrak{p}} $ ne soit pas intégralement clos sont ceux qui contiennent $ f $. Cela résulte aussitôt du cor. 4, (ii) appliqué à $ S = A - \mathfrak{p} $.

On notera que sous les hypothèses du cor. 5, on a $ f \neq 0 $, puisque $ A' $ est un $ A $-module de type fini et que tout élément de $ K/A $ ($ K $ corps des fractions de $ A $) a un annulateur $ \neq 0 $.

*En géométrie algébrique, le cor. 5 et la remarque précédente montrent que les points où une variété affine $ V $ n’est pas normale forment un ensemble fermé distinct de $ V_* $*

### 6. Normes et traces d’entiers

PROPOSITION 17. — Soient $ A $ un anneau, $ B $ une $ A $-algèbre (commutative), $ X $ une matrice carrée d’ordre $ n $ sur $ B $; les propriétés suivantes sont équivalentes:

a) $ X $ est entière sur $ A $.

b) Il existe un sous-$ A $-module de type fini $ M $ de $ B^n $, tel que $ X.x \in M $ pour tout $ x \in M $ et que $ M $ soit un système de générateurs du $ B $-module $ B^n $.

c) Les coefficients du polynôme caractéristique de $ X $ sont entiers sur $ A $.

Si $ \chi(T) = \det(T.1 - X) $ est le polynôme caractéristique de $ X $, le th. de Hamilton-Cayley montre que $ \chi(X) = 0 $ (Alg., chap. VII, § 5, no 4, Remarque 1) et comme $ \chi $ est un polynôme unitaire, c) implique a) en vertu du no 1, prop. 6.

Supposons en second lieu $a)$ vérifiée. Si $(e_i)_{1 \leq i \leq n}$ est la base canonique de $B^n$, le sous-A-module $M$ de $B$ engendré par les $X^k.e_i$ $(1 \leq i \leq n, k \geq 0)$ est un $A$-module de type fini, puisque la $A$-algèbre $A[X]$ est un $A$-module de type fini (no 1, th. 1); comme $M$ contient les $e_i$, on voit que $a)$ implique $b)$; la réciproque est une conséquence du no 1, th. 1, condition $(E_{III})$.

Prouvons enfin que $a)$ implique $c)$; comme $X$ est entière sur $A$, et $a$ fortiori sur l’anneau de polynômes $A[T]$, T.1 — $X$ est aussi entier sur $A[T]$, et en vertu du no 3, prop. 12, on voit qu’on est ramené (en remplaçant $X$ par T.1 — $X$ et $A$ par $A[T]$) à prouver que si $X$ est entière sur $A$, $d = \det(X)$ est un élément de $B$ entier sur $A$. Or, on a vu ci-dessus que l’endomorphisme $u$ de $B^n$ défini par $X$ laisse stable un sous-A-module $M$ de type fini contenant les $e_i$; les $n$-vecteurs $x_1 \wedge x_2 \wedge \cdots \wedge x_n$, où $x_i \in M$ pour $1 \leq i \leq n$, engendrent donc dans $\bigwedge^n(B^n)$ un sous-A-module de type fini contenant $e_1 \wedge e_2 \wedge \ldots \wedge e_n$, et qui est stable par $\bigwedge^n u$, autrement dit par l’homothétie de rapport $d$; comme l’annulateur de
$$
e_1 \wedge e_2 \wedge \cdots \wedge e_n
$$
dans $B$ est réduit à 0, la condition $(E_{III})$ du no 1, th. 1 prouve que $d$ est entier sur $A$.

C.Q.F.D.

COROLLAIRE 1. — Soient $A$ un anneau intègre, $K$ son corps des fractions, $K'$ une $K$-algèbre de dimension finie (non nécessairement commutative). Si $x \in K'$ est entier sur $A$, les coefficients du polynôme caractéristique $Pc_{K'/K}(x;X)$ (Alg., chap. VIII, § 12, no 2) sont entiers sur $A$.

En effet, si $z \to M(z)$ est la représentation régulière de l’algèbre $K'$ (considérée comme représentation matricielle; cf. Alg., chap. VIII, § 13) $Pc_{K'/K}(x;X)$ est par définition le polynôme caractéristique de la matrice $M(x)$; si $x$ est entier sur $A$, la matrice $M(x)$ est entière sur $A$ (no 1, prop. 2), et il suffit d’appliquer la prop. 17.

COROLLAIRE 2. — Avec les mêmes hypothèses et notations que dans le cor. 1, $Tr_{K'/K}(x)$ et $N_{K'/K}(x)$ sont entiers sur $A$.

En effet, $Tr_{K'/K}(x)$ et $N_{K'/K}(x)$ sont, au signe près, des coefficients de $Pc_{K'/K}(x;X)$ (Alg., chap. VIII, § 12, no 1, formules (4)), donc sont entiers.

PROPOSITION 18. — Soient $ A $ un anneau intégralement clos, $ K $ son corps des fractions, $ K' $ une $ K $-algèbre commutative séparable (A, V, p. 114) de dimension finie, $ A' $ la fermeture intégrale de $ A $ dans $ K' $. Alors $ A' $ est contenu dans un $ A $-module de type fini.
La proposition résultera du lemme plus précis suivant :

#### Lemme 3 {#ac-v-s1-lem-3 .statement}

Sous les hypothèses de la prop. 18, soit $ (\omega_1, \ldots, \omega_n) $ une base de $ K' $ sur $ K $, contenue dans $ A' $ (n° 5, cor. 2 de la prop. 16); il y a alors une base unique $ (\omega_1^*, \ldots, \omega_n^*) $ de $ K' $ sur $ K $ pour laquelle on a $ \mathrm{Tr}_{K'/K}(\omega_i \omega_j^*) = \delta_{ij} $ (indice de Kronecker); si $ d = D_{K'/K}(\omega_1, \ldots, \omega_n) $ est le discriminant de la base $ (\omega_1, \ldots, \omega_n) $ (Alg., chap. IX, § 2), on a $ d \neq 0 $ et

$$
\sum_{i=1}^n A \omega_i \subset A' \subset \sum_{i=1}^n A \omega_i^* \subset d^{-1} \left( \sum_{i=1}^n A \omega_i \right).
$$

En particulier, si $ d $ est un élément inversible de $ A $, $ A' $ est un $ A $-module libre de base $ (\omega_1, \ldots, \omega_n) $.

Comme $ K' $ est une $ K $-algèbre séparable, on a $ d \neq 0 $ (Alg., chap. IX, § 2, prop. 5) et la forme $ K $-bilinéaire

$$(x, y) \to \mathrm{Tr}_{K'/K}(xy)$$

sur $ K' $ est donc non dégénérée (loc. cit., prop. 4); ceci démontre l’existence et l’unicité de la base $ (\omega_i^*)_{1 \leq i \leq n} $ (Alg., chap. IX, § 1, n° 6, cor. de la prop. 6). Cela étant, la première inclusion de (2) est évidente. Soit $ x $ un élément de $ A' $; posons $ x = \sum_{i=1}^n \xi_i \omega_i^* $ avec $ \xi_i \in K $; pour tout $ i $, on a $ \xi_i = \mathrm{Tr}_{K'/K}(x \omega_i) $, donc $ \xi_i $ est entier sur $ A $ (cor. 2 de la prop. 17), et comme $ A $ est intégralement clos, on a $ \xi_i \in A $ pour $ 1 \leq i \leq n $; ceci démontre la seconde inclusion (2). Enfin, posons $ \omega_j^* = \sum_{i=1}^n \alpha_{ji} \omega_i $ avec $ \alpha_{ji} \in K $; on a alors $ \sum_{i=1}^n \alpha_{ji} \mathrm{Tr}_{K'/K}(\omega_i \omega_k) = \delta_{jk} $ quels que soient $ j $ et $ k $; les formules de Cramer montrent que les $ \alpha_{ji} $ appartiennent à $ d^{-1}A $, d’où la troisième inclusion (2). La dernière assertion résulte aussitôt de (2), qui donne dans ce cas $ A' = \sum_{i=1}^{n} A w_i $.

Dans les deux corollaires qui suivent, les hypothèses et notations sont celles de la prop. 18.

COROLLAIRE 1. — Si $ A $ est un anneau noethérien, le $ A $-module $ A' $ est de type fini, et en particulier l’anneau $ A' $ est noethérien.
En effet $ A' $ est un sous-module d’un $ A $-module de type fini.

COROLLAIRE 2. — Si $ A $ est un anneau principal, $ A' $ est un $ A $-module libre de rang $ n $.
En effet, tout sous-module d’un $ A $-module libre est alors libre (Alg., chap. VII, § 3, th. 1).

COROLLAIRE 3. — Soit $ E $ une extension de degré $ n $ du corps $ \mathbf{Q} $ des nombres rationnels. Le groupe additif de la fermeture intégrale dans $ E $ de l’anneau $ \mathbf{Z} $ des entiers rationnels est un groupe commutatif libre de rang $ n $.
En effet, $ \mathbf{Z} $ est intégralement clos (no 3, prop. 10) et $ E $ est séparable puisque $ \mathbf{Q} $ est de caractéristique 0. On peut donc appliquer le cor. 2 au cas où $ A = \mathbf{Z}, K = \mathbf{Q} $ et $ K' = E $.

#### Remarque 2 {#ac-v-s1-n6-rem-2 .statement}

Les conclusions du cor. 1 ne sont pas nécessairement vraies si on ne suppose pas $ K' $ séparable sur $ K $, même si $ K' $ est un surcorps de $ K $ (exerc. 20). Par contre, lorsque $ A $ est une $ K_0 $-algèbre intègre de type fini, où $ K_0 $ est un corps, la fermeture intégrale de $ A $ dans toute extension de degré fini du corps des fractions de $ A $ est un $ A $-module de type fini et un anneau noethérien, comme nous le verrons au § 3, no 2, th. 2.

### 7. Extension des scalaires dans une algèbre intégralement close

PROPOSITION 19. — Soient $ k $ un corps, $ L $ une extension séparable de $ k $, $ R $ une $ k $-algèbre intégralement close. Si l’anneau $ L \otimes_k R $ est intègre, il est intégralement clos.
Soit $ K $ le corps des fractions de $ R $; comme $ k $ est un corps, $ L \otimes_k R $ s’identifie canoniquement à une sous-$ k $-algèbre de $ L \otimes_k K $ et $ L $ et $ R $ à des sous-$ k $-algèbres de $ L \otimes_k R $. En outre, un élément $ s \neq 0 $ de $ R $ étant non diviseur de 0 dans $ R $, $ 1 \otimes s $ est non diviseur de zéro dans $ L \otimes_k R $ puisque $ L $ est plat sur $ k $ (chap. I,

1° Supposons d’abord que $ L $ soit une extension de degré fini de $ k $; alors $ L \otimes_k K $ est une algèbre de rang fini sur $ K $ et par hypothèse n’a pas de diviseur de 0; donc c’est un corps (Alg., chap. V, § 2, n° 1, prop. 1), et par suite c’est dans ce cas le corps des fractions $ \Omega $ de $ L \otimes_k R $. Soit $ (\omega_1, \ldots, \omega_n) $ une base de $ L $ sur $ k $, qui est donc aussi une base de $ L \otimes_k K $ sur $ K $. Il existe une base $ (\omega_1^*, \ldots, \omega_n^*) $ de $ L $ telle que $ \mathrm{Tr}_{L/k}(\omega_i \omega_j^*) = \delta_{ij} $ (n° 6, lemme 3); tout $ z \in L \otimes_k K $ s’écrit d’une seule manière $ z = \sum_{i=1}^n a_i \omega_i $ avec $ a_i \in K $; on a donc $ \mathrm{Tr}_{(L \otimes K)/K}(z \omega_j^*) = \sum_{i=1}^n a_i \mathrm{Tr}_{(L \otimes K)/K}(\omega_i \omega_j^*) $ et comme dans $ L $ les traces $ \mathrm{Tr}_{(L \otimes K)/K} $ et $ \mathrm{Tr}_{L/k} $ coïncident (Alg., chap. VIII, § 12, n° 2, formule (13)), on a finalement $ \mathrm{Tr}_{(L \otimes K)/K}(z \omega_j^*) = a_j $ pour $ 1 \leq j \leq n $. Notons d’autre part que les éléments de $ L $ sont entiers sur $ k $, donc aussi sur $ R $ (n° 1, cor. 1 de la prop. 2); par suite (n° 1, prop. 5) $ L \otimes_k R $ est entière sur $ R $. Cela étant, supposons $ z \in L \otimes_k K $ entier sur $ L \otimes_k R $; alors $ z $ est aussi entier sur $ R $ (n° 1, prop. 6), donc il en est de même de $ z \omega_j^* $ et par suite aussi de $ a_j = \mathrm{Tr}_{(L \otimes K)/K}(z \omega_j^*) $ pour $ 1 \leq j \leq n $ (n° 6, cor. 2 de la prop. 17). Comme $ R $ est intégralement clos, on a $ a_j \in R $ pour tout $ j $, donc $ z \in L \otimes_k R $, ce qui démontre la proposition dans ce cas.

2° Supposons maintenant que $ L $ soit une extension séparable de type fini de $ k $; alors il existe une base de transcendance séparante $ (x_1, \ldots, x_d) $ de $ L $ sur $ k $ (Alg., chap. V, § 9, n° 3, th. 2); comme $ L $ et $ K $ sont algébriquement disjointes sur $ k $ dans le corps $ \Omega $ (Alg., chap. V, § 5, n° 4), les $ x_i $ sont algébriquement indépendants sur $ K $; donc $ R[x_1, \ldots, x_d] $ est intégralement clos (n° 3, cor. 2 de la prop. 13). Soit $ T $ l’ensemble des éléments $ \neq 0 $ de l’anneau $ A = k[x_1, \ldots, x_d] \subset L $, de sorte que le corps $ k_1 = k(x_1, \ldots, x_d) \subset L $ est égal à $ T^{-1}k[x_1, \ldots, x_d] $; on a
$$
k_1 \otimes_k R = (T^{-1}A) \otimes_k R = T^{-1}A \otimes_A (A \otimes_k R)
= T^{-1}(A \otimes_k R) = T^{-1}R[x_1, \ldots, x_d]
$$
par associativité du produit tensoriel, donc cet anneau est intégralement clos (n° 5, cor. 1 de la prop. 16). Mais $ L \otimes_k R $ s’identifie à $ L \otimes_{k_1}(k_1 \otimes_k R) $ et par définition $ L $ est une extension séparable de degré fini de $ k_1 $; il résulte donc de 1° que $ L \otimes_k R $ est intégralement clos.

3° *Cas général.* Si $ z $ est un élément de $ \Omega $ entier sur $ L \otimes_k R $, il vérifie une relation de la forme $ z^m + b_1 z^{m-1} + \cdots + b_m = 0 $, où les $ b_i $ appartiennent à $ L \otimes_k R $; il existe donc une sous-extension $ L' $ de $ L $, de type fini sur $ k $, telle que les $ b_i $ appartiennent à $ L' \otimes_k R $ pour $ 1 \leq i \leq m $, et $ z $ à $ L' \otimes_k K $. Il résulte alors de 2° que l’on a $ z \in L' \otimes_k R $, donc $ L \otimes_k R $ est intégralement clos.

C.Q.F.D.

*Soient $ V $ une variété algébrique irréductible affine, $ k $ un corps de définition de $ V $, $ R $ l’anneau des fonctions régulières sur $ V $ définies sur $ k $; lorsque $ R $ est intégralement clos, on dit que $ V $ est *normale sur* $ k $; la prop. 19 montre que si $ V $ est normale sur $ k $, elle reste normale sur toute extension séparable $ L $ de $ k_*$

COROLLAIRE. — *Soient $ k $ un corps, $ R $ et $ S $ deux $ k $-algèbres intégralement closes. On suppose que l’anneau $ R \otimes_k S $ est intègre et que les corps des fractions $ K $ et $ L $ de $ R $ et $ S $ respectivement sont séparables sur $ k $. Alors l’anneau $ R \otimes_k S $ est intégralement clos.*

En effet, comme $ R $ et $ S $ s’identifient à des sous-algèbres de $ R \otimes_k S $, $ K $ et $ L $ s’identifient à des sous-corps du corps des fractions $ \Omega $ de $ R \otimes_k S $, linéairement disjoints sur $ k $ (*Alg.*, chap. V, § 2, no 3, prop. 5). Il résulte alors de la prop. 19 que $ R \otimes_k L $ et $ K \otimes_k S $ sont intégralement clos; comme leur intersection est $ R \otimes_k S $ (chap. I, § 2, no 6, prop. 7), $ R \otimes_k S $ est intégralement clos (no 2, cor. de la prop. 8).

\* Étant données deux variétés affines irréductibles $ V $, $ W $ définies sur $ k $, leur produit $ V \times W $ est une variété affine, et l’anneau des fonctions régulières sur $ V \times W $ s’identifie au produit tensoriel sur $ k $ de l’anneau des fonctions régulières sur $ V $ et de l’anneau des fonctions régulières sur $ W $. Le cor. de la prop. 19 montre que si $ V $ et $ W $ sont normales sur $ k $, alors $ V \times W $ est normale sur $ k_*$

### 8. *Entiers sur un anneau gradué*

*Toutes les graduations envisagées dans ce no sont de type $ \mathbf{Z} $; si $ A $ est un anneau gradué et si $ i \in \mathbf{Z} $, on note $ A_i $ l’ensemble des éléments homogènes de degré $ i $ de l’anneau $ A $.*

Soient $ A $ un anneau gradué et $ B $ une $ A $-algèbre graduée. Soit $ x $ un élément *homogène* de $ B $ qui soit entier sur $ A $; on a donc une relation

$$
x^n + a_1 x^{n-1} + \cdots + a_n = 0 \quad \text{avec } a_i \in A \text{ pour } 1 \leq i \leq n.
$$

Soit $ m = \deg(x) $ et soit $ a'_i $ la composante homogène de degré $ mi $ de $ a_i $ ($ 1 \leq i \leq n $); on a évidemment

$$
x^n + a'_1 x^{n-1} + \cdots + a'_n = 0
$$

autrement dit $ x $ vérifie une équation de dépendance intégrale à coefficients *homogènes*.

Désignons par $ A[X, X^{-1}] $ l’anneau de fractions $ S^{-1}A[X] $ de l’anneau de polynômes $ A[X] $ en une indéterminée, $ S $ étant la partie multiplicative de $ A[X] $ formée des puissances $ X^n $ de $ X $ ($ n \geq 0 $); comme $ X $ est non diviseur de $ 0 $ dans $ A[X] $ il est immédiat que les $ X^i $ ($ i \in \mathbf{Z} $) forment une *base* sur $ A $ du $ A $-module $ A[X, X^{-1}] $. Pour tout élément $ a \in A $, de composantes homogènes $ a_i $ ($ i \in \mathbf{Z} $), on posera

$$
j_A(a) = \sum_{i \in \mathbf{Z}} a_i X^i \in A[X, X^{-1}]
$$

il est immédiat que $ j_A : A \to A[X, X^{-1}] $ est un homomorphisme injectif d’anneaux.

#### Proposition 20 {#ac-v-s1-prop-20 .statement}

*Soient* $ A = \bigoplus_{i \in \mathbf{Z}} A_i $ *un anneau gradué* et $ B $ *une* $ A $*-algèbre graduée (commutative)*. L’ensemble $ A' $ des éléments de $ B $ entiers sur $ A $ *est une sous-algèbre graduée de* $ B $. *Si* $ A_i = 0 $ *pour* $ i < 0 $ *et si* $ B $ *est un anneau réduit*, *on a* $ A'_i = 0 $ *pour* $ i < 0 $.

Le diagramme

$$
\begin{array}{ccc}
A & \xrightarrow{\rho} & B \\
j_A \downarrow & & \downarrow j_B \\
A[X, X^{-1}] & \xrightarrow{\rho'} & B[X, X^{-1}]
\end{array}
$$

(où $ \rho $ est l’homomorphisme définissant la structure de $ A $-algèbre de $ B $ et $ \rho' $ l’homomorphisme qui s’en déduit canoniquement) est commutatif, comme on le vérifie aussitôt sur la définition (5). Soit $ x $ un élément de $ B $ entier sur $ A $; alors $ j_B(x) $ est entier sur $ A[X, X^{-1}] $ (no 1, prop. 2) et il résulte donc du no 5, prop. 16 qu’il existe un entier $ m > 0 $ tel que $ X^m j_B(x) $ soit un élément de

B[X] entier sur A[X]. On déduit alors du no 3, prop. 12, que les coefficients du polynôme $ X^m j_B(x) $ sont entiers sur A; comme ces coefficients sont par définition les composantes homogènes de $ x $, on voit que celles-ci sont entières sur A, ce qui prouve que $ A' $ est une sous-algèbre graduée de B.

Supposons maintenant que $ x \in A'_i $ avec $ i < 0 $; la remarque du début de ce no montre que $ x $ vérifie une équation de la forme (4) avec $ a_k' \in A_{ki} $ pour $ 1 \leq k \leq n $. Si $ A_j = 0 $ pour tout $ j < 0 $, on a donc $ x^n = 0 $ et si B est un anneau réduit on en conclut que $ x = 0 $, donc $ A'_i = 0 $ pour tout $ i < 0 $ dans ce cas.

Rappelons (chap. II, § 2, no 9) que si $ A = \bigoplus_{i \in \mathbf{Z}} A_i $ est un anneau gradué et S une partie multiplicative de A formée d’éléments homogènes, on définit sur $ S^{-1}A $ une structure d’anneau gradué en prenant pour ensemble $ (S^{-1}A)_i $ d’éléments homogènes de degré $ i $ l’ensemble des éléments de la forme $ a/s $, où $ a \in A $ et $ s \in S $ sont homogènes et tels que $ \deg(a) - \deg(s) = i $.

#### Lemme 4 {#ac-v-s1-lem-4 .statement}

*Soient $ A = \bigoplus_{i \in \mathbf{Z}} A_i $ un anneau gradué intègre, S l’ensemble des éléments homogènes $ \neq 0 $ de A.*

(i) *Tout élément homogène $ \neq 0 $ de $ S^{-1}A $ est inversible, l’anneau $ K_0 = (S^{-1}A)_0 $ est un corps et l’ensemble des $ i \in \mathbf{Z} $ tels que $ (S^{-1}A)_i \neq 0 $ est un sous-groupe $ q\mathbf{Z} $ de $ \mathbf{Z} $ (avec $ q \geq 0 $).

(ii) *Supposons que $ q \geq 1 $ et soit t un élément non nul de $ (S^{-1}A)_q $. Alors le $ K_0 $-homomorphisme $ f $ de l’anneau de polynômes $ K_0[X] $ dans $ S^{-1}A $ qui transforme X en t se prolonge en un isomorphisme de $ K_0[X, X^{-1}] $ sur $ S^{-1}A $, et $ S^{-1}A $ est intégralement clos.*

Les assertions de (i) découlent immédiatement des définitions et de l’hypothèse que A est intègre, car si $ a/s $ et $ a'/s' $ sont deux éléments homogènes $ \neq 0 $ de $ S^{-1}A $, de degrés $ i $ et $ i' $, $ aa'/ss' $ est un élément homogène $ \neq 0 $ et de degré $ i + i' $. Pour démontrer (ii), notons que puisque $ t $ est inversible dans $ S^{-1}A $, l’homomorphisme $ f $ se prolonge d’une seule manière en un homomorphisme $ \bar{f} : K_0[X, X^{-1}] \to S^{-1}A $ et l’on a nécessairement $ \bar{f}(X^{-1}) = t^{-1} $. D’autre part, par définition de $ q $, tout élément homogène $ \neq 0 $ de $ S^{-1}A $ est de degré $ qn $ ($ n \in \mathbf{Z} $), donc peut s’écrire d’une seule manière sous la forme $ \lambda t^n $ avec $ \lambda \in K_0 $ (puisque $ S^{-1}A $ est intègre); donc $ \bar{f} $ est bijectif. Enfin, on sait que $ K_0[X] $ est intégralement clos (no 3, prop. 10), donc il en est de même de $ K_0[X, X^{-1}] $ (no 5, cor. 1 de la prop. 16), ce qui achève de prouver le lemme.

PROPOSITION 21. — Soient $ A = \bigoplus_{i \in \mathbf{Z}} A_i $ un anneau gradué intègre, S l’ensemble des éléments homogènes $ \neq 0 $ de A. La clôture intégrale $ A' $ de A est alors un sous-anneau gradué de $ S^{-1}A $. Si en outre $ A_i = 0 $ pour $ i < 0 $, on a $ A'_i = 0 $ pour $ i < 0 $.

Si $ A = A_0 $, la proposition est triviale. Sinon, on peut appliquer le lemme 4; l’anneau $ S^{-1}A $ est intégralement clos et par suite $ A' \subset S^{-1}A $; comme $ S^{-1}A $ est gradué, il en est de même de $ A' $ en vertu de la prop. 20; la dernière assertion résulte aussi de la prop. 20.

COROLLAIRE 1. — Les hypothèses et notations étant celles de la prop. 21, si tout élément homogène de $ S^{-1}A $ qui est entier sur A appartient à A, alors A est intégralement clos.

En effet on a, alors $ A'_i \subset A $ pour tout $ i \in \mathbf{Z} $, donc $ A' = A $.

COROLLAIRE 2. — Si $ A = \bigoplus_{i \in \mathbf{Z}} A_i $ est un anneau gradué intégralement clos, l’anneau $ A_0 $ est intégralement clos.

En effet, le corps des fractions $ K_0 $ de $ A_0 $ s’identifie (avec les notations de la prop. 21) à un sous-anneau de l’anneau des éléments homogènes de degré 0 de $ S^{-1}A $; tout élément de $ K_0 $ entier sur $ A_0 $ (et a fortiori sur A) appartient donc par hypothèse à $ A_0 $.

COROLLAIRE 3. — Soit $ A = \bigoplus_{i \in \mathbf{Z}} A_i $ un anneau gradué intégralement clos. Alors, pour tout entier $ d > 0 $, l’anneau $ A^{(d)} $ (chap. III, § 1, no 3) est intégralement clos.

Soit U l’ensemble des éléments homogènes $ \neq 0 $ de $ A^{(d)} $, et soit x un élément homogène de $ U^{-1}A^{(d)} $ entier sur $ A^{(d)} $, donc sur A; comme $ x \in S^{-1}A $, x appartient à A par hypothèse; comme son degré est divisible par d, il appartient à $ A^{(d)} $, et il résulte donc du cor. 1 que $ A^{(d)} $ est intégralement clos.

### 9. Application : invariants d’un groupe d’automorphismes d’une algèbre

Étant donnés un anneau K, une K-algèbre A, et un groupe $ G_j $, nous dirons que $ G_j $ opère sur A si : 1° l’ensemble A est muni du groupe d’opérateurs $ G_j $ (Alg., chap. I, § 7, no 2); 2° pour tout $ \sigma \in G_j $, l’application $ x \to \sigma.x $ est un endomorphisme de la K-algèbre

A (et par suite un automorphisme puisqu’elle est bijective (loc. cit.)). Nous noterons $ A^G_g $ l’ensemble des éléments de A invariants par $ G $; il est clair que c’est une sous-K-algèbre de A.

Nous dirons que $ G $ est un groupe d’opérateurs localement fini sur A si toute orbite de $ G $ dans A (Alg., chap. I, 3e éd., Rectifications au fasc. IV) est finie.

#### Proposition 22 {#ac-v-s1-prop-22 .statement}

Soient A une K-algèbre (commutative), $ G $ un groupe d’opérateurs localement fini sur A. Alors A est entière sur la sous-algèbre $ A^G_g $.

En effet, pour tout $ x \in A $, soient $ x_i (1 \leq i \leq n) $ les éléments distincts de l’orbite de $ x $ pour $ G $; pour tout $ \sigma \in G $, il existe une permutation $ \pi_\sigma $ de l’ensemble $ \{1, 2, \ldots, n\} $ telle que $ \sigma.x_i = x_{\pi_\sigma(i)} $ pour $ 1 \leq i \leq n $; par suite les fonctions symétriques élémentaires des $ x_i $ sont des éléments de A invariants par $ G $, autrement dit des éléments de $ A^G_g $. Comme $ x $ est racine du polynôme unitaire $ \prod_{i=1}^n (X - x_i) $ et que les coefficients de ce polynôme appartiennent à $ A^G_g $, $ x $ est entier sur $ A^G_g $.

#### Théorème 2 {#ac-v-s1-thm-2 .statement}

Soient A une K-algèbre de type fini, $ G $ un groupe d’opérateurs localement fini sur A. Alors A est un $ A^G_g $-module de type fini; si de plus K est noethérien, $ A^G_g $ est une K-algèbre de type fini.

Soit $ (a_j)_{1 \leq j \leq m} $ un système de générateurs de la K-algèbre A; comme on a a fortiori $ A = A^G_g[a_1, \ldots, a_m] $ et que les $ a_j $ sont entiers sur $ A^G_g $ en vertu de la prop. 22, la première assertion résulte du no 1, prop. 4. La seconde est conséquence du lemme suivant:

#### Lemme 5 {#ac-v-s1-lem-5 .statement}

Soient K un anneau noethérien, B une K-algèbre de type fini, C une sous-K-algèbre de B telle que B soit entière sur C. Alors C est une K-algèbre de type fini.

Soit $ (x_i)_{1 \leq i \leq n} $ un système fini de générateurs de la K-algèbre B. Pour tout $ i $, il existe par hypothèse un polynôme unitaire $ P_i \in \mathbf{C}[X] $ tel que $ P_i(x_i) = 0 $. Soit $ C' $ la sous-K-algèbre de C engendrée par les coefficients des $ P_i (1 \leq i \leq n) $; il est clair que les $ x_i $ sont entiers sur $ C' $ et que l’on a $ B = C'[x_1, \ldots, x_n] $; donc B est un $ C' $-module de type fini (no 1, prop. 4). D’autre part,

#### Remarque {#ac-v-s1-n9-rem-1 .statement}

L’ensemble des $ \sigma \in \mathcal{G} $ tels que $ \sigma a_j = a_j $ pour $ 1 \leq j \leq m $ laisse évidemment invariant tout élément de A. Le sous-groupe distingué $ \mathcal{H} $ de $ \mathcal{G} $ laissant invariant tout élément de A est donc d’indice fini dans $ \mathcal{G} $ et on peut considérer que A est muni du groupe d’opérateurs fini $ \mathcal{G}/\mathcal{H} $; on a évidemment $ A_{\mathcal{G}/\mathcal{H}} = A_{\mathcal{G}} $.

Soient S une partie multiplicative d’un anneau A, $ \mathcal{G} $ un groupe opérant sur A et pour lequel S est stable; alors, pour tout $ \sigma \in \mathcal{G} $, il existe un endomorphisme et un seul $ z \to \sigma.z $ de l’anneau $ S^{-1}A $ tel que $ \sigma.(a/1) = (\sigma.a)/1 $ pour tout $ a \in A $; il est donné par la formule $ \sigma.(a/s) = (\sigma.a)/(\sigma.s) $ pour $ a \in A $ et $ s \in S $ (chap. II, § 2, no 1, prop. 2); si $ \tau $ est un second élément de $ \mathcal{G} $, il est clair que $ \sigma.(\tau.z) = (\sigma\tau).z $ pour tout $ z \in S^{-1}A $, donc le groupe $ \mathcal{G} $ opère sur l’anneau $ S^{-1}A $.

#### Proposition 23 {#ac-v-s1-prop-23 .statement}

Soient A une K-algèbre, $ \mathcal{G} $ un groupe d’opérateurs localement fini sur A, S une partie multiplicative de A stable pour $ \mathcal{G} $, $ S_{\mathcal{G}} $ l’ensemble $ S \cap A_{\mathcal{G}} $. Alors l’application canonique de $ (S_{\mathcal{G}})^{-1}A $ dans $ S^{-1}A $ (chap. II, § 2, no 1, cor. 2 de la prop. 2) est un isomorphisme, qui transforme $ (S_{\mathcal{G}})^{-1}A_{\mathcal{G}} $ en $ (S^{-1}A)_{\mathcal{G}} $.

En effet, pour tout $ s \in S $, soient $ s, s_1, \ldots, s_q $ les éléments distincts de l’orbite de s pour $ \mathcal{G} $; comme $ ss_1 \ldots s_q \in S_{\mathcal{G}} $, la première assertion résulte du chap. II, § 2, no 3, prop. 8. Identifiant canoniquement $ (S_{\mathcal{G}})^{-1}A $ et $ S^{-1}A $, il est clair que tout élément de $ (S_{\mathcal{G}})^{-1}A_{\mathcal{G}} $ est invariant par $ \mathcal{G} $. Réciproquement, soit $ a/t $ un élément de $ (S_{\mathcal{G}})^{-1}A $ invariant par $ \mathcal{G} $ ($ a \in A, t \in S_{\mathcal{G}} $); si $ a_j (1 \leq j \leq m) $ sont les éléments distincts de l’orbite de a pour $ \mathcal{G} $, on a donc $ a_j/t = a/t $ pour $ 1 \leq j \leq m $, et par suite il existe $ s \in S_{\mathcal{G}} $ tel que $ s(a_j - a) = 0 $ pour $ 1 \leq j \leq m $; autrement dit, sa est invariant par $ \mathcal{G} $ et comme $ a/t = (sa)/(st) $, on a bien $ a/t \in (S_{\mathcal{G}})^{-1}A_{\mathcal{G}} $.

#### Corollaire {#ac-v-s1-n9-cor-1 .statement}

Soient A un anneau intègre, K son corps des fractions, $ \mathcal{G} $ un groupe d’opérateurs localement fini sur A. Alors $ \mathcal{G} $ opère sur K et $ K_{\mathcal{G}} $ est le corps des fractions de $ A_{\mathcal{G}} $.

En effet, $ A - \{0\} $ est stable pour $ \mathcal{G} $.

## EXERCICES {#ac-v-s1-exercises}

See the [exercises for § 1](exercises/s1/).
