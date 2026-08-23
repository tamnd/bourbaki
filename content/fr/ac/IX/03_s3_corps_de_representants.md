---
book: ac
book_title: Commutative Algebra
chapter: IX
chapter_title: ANNEAUX LOCAUX NOETHÉRIENS COMPLETS
section: 3
section_title: Corps de représentants
lang: fr
source: ac-viii-ix-fr
book_pages: AC IX.28-AC IX.30, AC IX.75-AC IX.78
pdf_pages: 0140-0142, 0187-0190
extraction: ocr
subsections:
    - "no": 1
      title: Anneaux locaux d’égales caractéristiques
      page: 28
      pdf_page: 140
    - "no": 2
      title: Un théorème de relèvement
      page: 28
      pdf_page: 140
    - "no": 3
      title: Corps de représentants
      page: 29
      pdf_page: 141
statements: 7
exercises: 9
content_sha256: cbaf8843cce087daaa3d3f5c5e6b6092542009e0c34be277f981ba660fa6393d
---

## § 3. Corps de représentants

### 1. Anneaux locaux d’égales caractéristiques

Soit A un anneau. Rappelons (A, V, p. 2) que la caractéristique de A est définie lorsque A contient un sous-corps. Elle est égale à 0 si et seulement si A contient un sous-corps isomorphe à $ \mathbf{Q} $; et égale à un nombre premier $ p $ si et seulement si on a $ p1_A = 0 $. Si la caractéristique de A est définie, et si $ f : A \to B $ est un homomorphisme non nul d’anneaux, la caractéristique de B est définie et elle est égale à celle de A.

Soit A un anneau local, d’idéal maximal $ m $, et de corps résiduel $ k $.

a) Supposons $ k $ de caractéristique 0. Alors A contient un corps et la caractéristique de A est égale à 0. En effet, l’homomorphisme canonique de $ \mathbf{Z} $ dans A est injectif, et pour tout entier $ n $ non nul, $ n1_A $ est inversible dans A, car il n’appartient pas à $ m $.

b) Supposons $ k $ de caractéristique $ p \neq 0 $. Alors A contient un corps si et seulement si $ p1_A = 0 $. Dans ce cas la caractéristique de A est égale à $ p $.

Supposons que A soit un anneau local intègre, de corps des fractions K et de corps résiduel $ k $.

a’) L’anneau A contient un sous-corps si et seulement si les caractéristiques de $ k $ et K sont égales. Dans ce cas, la caractéristique de A est égale à celle de $ k $ et de K, et on dit que A est un anneau local d’égales caractéristiques.

b’) Supposons que les corps $ k $ et K n’aient pas même caractéristique. Alors il existe un nombre premier $ p $ tel que $ k $ soit de caractéristique $ p $. Comme on a $ q1_A \neq 0 $ pour tout nombre premier $ q \neq p $, le corps K est de caractéristique 0. On dit alors que A est un anneau local d’inégales caractéristiques.

### 2. Un théorème de relèvement

#### Proposition 1 {#ac-ix-s3-prop-1 .statement}

Soient $ k_0 $ un corps, A une $ k_0 $-algèbre qui est un anneau local séparé et complet, K une sous-$ k_0 $-extension de $ \kappa_A $ qui possède une base de transcendance séparante $ (\xi_{\lambda})_{\lambda \in \Lambda} $ sur $ k_0 $ (A, V, p. 130, déf. 1). Pour tout $ \lambda \in \Lambda $, soit $ x_{\lambda} $ un représentant de $ \xi_{\lambda} $ dans A. Il existe un unique sous-corps L de A, contenant $ k_0 $ et les éléments $ x_{\lambda} $, et tel que l’homomorphisme canonique $ \pi $ de A sur $ \kappa_A $ induise un isomorphisme de L sur K.

Soit $ \varphi $ le $ k_0 $-homomorphisme de l’anneau de polynômes $ k_0[(X_{\lambda})_{\lambda \in \Lambda}] $ dans A qui applique $ X_{\lambda} $ sur $ x_{\lambda} $ pour tout $ \lambda \in \Lambda $. Soit $ u $ un élément non nul de $ k_0[(X_{\lambda})_{\lambda \in \Lambda}] $; on a $ \pi(\varphi(u)) \neq 0 $, car la famille $ (\xi_{\lambda})_{\lambda \in \Lambda} $ est algébriquement libre sur $ k_0 $ dans $ \kappa_A $; par suite, $ \varphi(u) $ est inversible dans l’anneau local A. Il en résulte que $ \varphi $ se prolonge en un homomorphisme $ \psi $ du corps $ k_1 = k_0((X_{\lambda})_{\lambda \in \Lambda}) $ dans A. Alors A est une $ k_1 $-algèbre, $ \kappa_A $ est une extension de $ k_1 $ et K une sous-extension de $ \kappa_A $ qui est algébrique et séparable sur $ k_1 $. Il s’agit de prouver qu’il existe un unique sous-corps L de A contenant $ \psi(k_1) $ et tel que $ \pi(L) = K $.

a) *Existence de L* : Soit S l’ensemble des sous-corps L de A, contenant $ \psi(k_1) $ et tels que $ \pi(L) \subset K $; il est inductif pour la relation d’inclusion. Soit L un élément maximal de S ; on considère K comme une extension (algébrique et séparable, d’après A, V, p. 40, prop. 9) de L. Soit $ \xi \in K $ et soit $ P \in L[X] $ son polynôme minimal sur L. Comme $ \xi $ est racine simple de P, le lemme de Hensel (III, § 4, no 5, cor. 1 du th. 2) assure l’existence d’un élément x de A tel que $ \pi(x) = \xi $ et $ P(x) = 0 $. Le sous-anneau $ L[X] $ de A appartient à S ; d’après le caractère maximal de L, on a donc $ x \in L $, d’où $ \xi \in \pi(L) $. Finalement on a $ \pi(L) = K $.

b) *Unicité de L* : Soient L et L’ deux sous-corps de A contenant $ \psi(k_1) $ et tels que $ \pi(L) = \pi(L') = K $. Soit $ \xi \in K $, et soient $ x \in L $ et $ x' \in L' $ les éléments tels que $ \pi(x) = \pi(x') = \xi $. Si $ P \in k_1[X] $ est le polynôme minimal de $ \xi $ sur $ k_1 $, alors $ \xi $ est racine simple de P, et l’on a $ P(x) = P(x') = 0 $. D’après le lemme de Hensel (*loc. cit.*) on a $ x = x' $. On a donc $ L = L' $.

#### Remarque {#ac-ix-s3-n2-rem-1 .statement}

\* La démonstration précédente s’applique plus généralement au cas où on suppose seulement que A est un anneau local hensélien*. La démonstration d’unicité utilise l’hypothèse que l’anneau local A est séparé, mais non qu’il est complet.

### 3. Corps de représentants

#### Définition 1 {#ac-ix-s3-def-1 .statement}

*Soit A un anneau local. On appelle corps de représentants de A tout sous-corps K de A tel que l’homomorphisme canonique de A sur $ \kappa_A $ induise un isomorphisme de K sur $ \kappa_A $ (autrement dit, tel que $ A = K + m_A $).*

Il ne peut exister de corps de représentants de A que si A admet une caractéristique. Cette condition est suffisante lorsque A est séparé et complet. Plus précisément, on a le théorème suivant :

#### Théorème 1 {#ac-ix-s3-thm-1 .statement}

*Soit A un anneau local séparé et complet de caractéristique p.*

a) *Supposons $ p = 0 $ et soit $ (x_\lambda)_{\lambda \in \Lambda} $ une famille d’éléments de A dont les classes modulo $ m_A $ forment une base de transcendance de $ \kappa_A $ sur $ \mathbf{Q} $. Il existe un unique corps de représentants de A contenant les éléments $ x_\lambda $.*

b) *Supposons $ p \neq 0 $. Soit $ (x_\lambda)_{\lambda \in \Lambda} $ une famille d’éléments de A dont les classes modulo $ m_A $ forment une p-base de $ \kappa_A $ (A, V, p. 95). Il existe un unique corps de représentants de A contenant les éléments $ x_\lambda $. C’est un sous-anneau de Cohen de A.*

Supposons qu’on ait $ p = 0 $ de sorte que A est une $ \mathbf{Q} $-algèbre. Toute base de transcendance de $ \kappa_A $ sur $ \mathbf{Q} $ étant séparante, l’assertion a) résulte de la prop. 1 du no 1 appliquée au cas $ k_0 = \mathbf{Q} $, $ K = \kappa_A $.

Supposons maintenant qu’on ait $ p \neq 0 $. Alors on a $ p1_A = 0 $, et tout sous-anneau de Cohen C de A satisfait à $ pC = 0 $. Autrement dit, il y a identité entre les notions de corps de représentants et de sous-anneau de Cohen de A. L’assertion b) résulte alors du § 2, no 2, th. 1.

#### Corollaire 1 {#ac-ix-s3-thm-1-cor-1 .statement}

Soit $ A $ un anneau local séparé et complet, dont le corps résiduel est une extension algébrique de $ \mathbf{Q} $. Il existe alors un unique corps de représentants de $ A $.
En effet l’anneau $ A $ est de caractéristique 0 (no 1).

#### Corollaire 2 {#ac-ix-s3-thm-1-cor-2 .statement}

Soit $ A $ un anneau local séparé et complet de caractéristique $ p \neq 0 $. Supposons que le corps résiduel $ \kappa_A $ soit parfait. Alors il existe un unique corps de représentants de $ A $, à savoir l’ensemble des représentants multiplicatifs.
Le cor. 2 résulte aussitôt du th. 1 et de la prop. 7 du § 2, no 4.

#### Théorème 2 {#ac-ix-s3-thm-2 .statement}

Soit $ A $ un anneau local noethérien complet de dimension $ d $ contenant un corps. Soit $ K $ un corps de représentants de $ A $, et soit $ m $ la dimension de l’espace vectoriel $ m_A/m_A^2 $ sur le corps $ K $.
a) Il existe un idéal $ a $ de $ K[[T_1, ..., T_m]] $ tel que la $ K $-algèbre $ A $ soit isomorphe à $ K[[T_1, ..., T_m]]/a $.
b) Il existe une sous-$ K $-algèbre $ A' $ de $ A $, isomorphe à $ K[[T_1, ..., T_d]] $ et telle que $ A $ soit une algèbre finie sur $ A' $.
c) Supposons que l’anneau local noethérien $ A $ soit régulier, i.e. $ d = m $. Alors il existe un $ K $-isomorphisme de $ A $ sur $ K[[T_1, ..., T_d]] $.
Soient $ t_1, ..., t_m $ des éléments de $ m_A $ dont les classes modulo $ m_A^2 $ engendrent le $ K $-espace vectoriel $ m_A/m_A^2 $. D’après le lemme 3 du § 2, no 5, il existe un $ K $-homomorphisme surjectif de $ K[[T_1, ..., T_m]] $ dans $ A $, transformant $ T_i $ en $ t_i $ pour $ 1 \leq i \leq m $. Ceci prouve $ a $.
De même, l’assertion $ b $ résulte du lemme 4 de loc. cit. et de l’existence d’une suite sécante maximale pour $ A $ (VIII, § 3, no 2, th. 1).
Enfin, l’assertion $ c $ n’est autre que le cor. 3 du th. 1 de VIII, § 5, no 2.

## EXERCICES {#ac-ix-s3-exercises}

See the [exercises for § 3](exercises/s3/).
