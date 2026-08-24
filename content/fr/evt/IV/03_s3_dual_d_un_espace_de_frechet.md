---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: LA DUALITÉ DANS LES ESPACES VECTORIELS TOPOLOGIQUES
section: 3
section_title: Dual d’un espace de Fréchet
lang: fr
source: evt-i-v-fr
book_pages: EVT IV.20-EVT IV.26, EVT IV.58-EVT IV.62
pdf_pages: 0206-0212, 0244-0248
extraction: ocr
subsections:
    - "no": 1
      title: Espaces semi-tonnelés
      page: 20
      pdf_page: 206
    - "no": 2
      title: Dual d’un espace localement convexe métrisable
      page: 21
      pdf_page: 207
    - "no": 3
      title: Bidual d’un espace localement convexe métrisable
      page: 22
      pdf_page: 208
    - "no": 4
      title: Dual d’un espace de Fréchet réflexif
      page: 23
      pdf_page: 209
    - "no": 5
      title: La topologie de la convergence compacte sur le dual d’un espace de Fréchet
      page: 24
      pdf_page: 210
    - "no": 6
      title: Applications bilinéaires séparément continues
      page: 25
      pdf_page: 211
statements: 15
exercises: 18
content_sha256: 74d314526bdd3197a2777453c0ca689467f92f3f044106de47c5445cd9e83e63
---

## § 3. DUAL D’UN ESPACE DE FRÉCHET

### 1. Espaces semi-tonnelés

#### Proposition 1 {#evt-iv-s3-prop-1 .statement}

Soit $E$ un espace localement convexe. Les conditions suivantes sont équivalentes :
(i) Soit $U$ une partie de $E$, qui absorbe toute partie bornée de $E$, et qui est intersection d’une suite de voisinages convexes, équilibrés et fermés de 0 dans $E$. Alors $U$ est un voisinage de 0 dans $E$.

(ii) Pour tout espace localement convexe F, toute partie bornée de $ \mathcal{L}_b(E; F) $, qui est réunion d’une famille dénombrable de parties équicontinues, est équicontinue.

(iii) Dans le dual fort $ E'_b $ de E, toute partie bornée qui est réunion d’une famille dénombrable de parties équicontinues, est équicontinue.

Il est clair que (iii) est un cas particulier de (ii).

(i) $ \Rightarrow $ (ii) : soit H une partie bornée de $ \mathcal{L}_b(E; F) $, et soit $ (H_n) $ une suite de parties équicontinues de $ \mathcal{L}_b(E; F) $ telle que $ H = \bigcup_n H_n $. Soit V un voisinage convexe, équilibré et fermé de 0 dans F. Pour tout n, l’ensemble $ W_n = \bigcap_{u \in H_n} u^{-1}(V) $ est un voisinage convexe, équilibré et fermé de 0 dans E puisque $ H_n $ est équicontinue. L’ensemble $ W = \bigcap_{u \in H} u^{-1}(V) $ absorbe toute partie bornée de E, puisque H est borné dans $ \mathcal{L}_b(E; F) $ (III, p. 22), et l’on a $ W = \bigcap_n W_n $. Si E satisfait à (i), l’ensemble W est un voisinage de 0 dans E, donc H est équicontinu.

(iii) $ \Rightarrow $ (i) : soit $ (U_n) $ une suite de voisinages convexes, équilibrés et fermés de 0 dans E. On suppose que l’ensemble $ U = \bigcap_n U_n $ absorbe toute partie bornée de E, donc que son polaire $ U^\circ $ est borné dans $ E'_b $. Alors l’ensemble $ B = \bigcup_n U_n^\circ $ est contenu dans $ U^\circ $, donc est borné dans $ E'_b $. Si E satisfait à (iii), l’ensemble B est équicontinu dans $ E' $; par suite, le polaire $ B^\circ = \bigcap_n (U_n^\circ)^\circ = \bigcap_n U_n = U $ de B dans E est un voisinage de 0 dans E.

#### Définition 1 {#evt-iv-s3-def-1 .statement}

On dit qu’un espace localement convexe E est semi-tonnelé s’il satisfait aux conditions équivalentes de la prop. 1.

Tout espace tonnelé est semi-tonnelé. Il en est de même de tout espace bornologique (III, p. 22, prop. 10).

### 2. Dual d’un espace localement convexe métrisable

#### Proposition 2 {#evt-iv-s3-prop-2 .statement}

Soient E un espace localement convexe métrisable et F son dual fort. L’espace F est complet, semi-tonnelé et satisfait à la condition suivante :

(DB) Il existe une suite $ (A_n)_{n \in \mathbf{N}} $ de parties bornées de F telle que toute partie bornée de F soit contenue dans l’une des $ A_n $.

L’espace E est bornologique (III, p. 12, prop. 2), donc son dual fort est complet (III, p. 24, cor. 1).

Soit $ (V_n)_{n \in \mathbf{N}} $ une suite décroissante de voisinages de 0 dans E, telle que tout voisinage de 0 dans E contienne l’un des $ V_n $. Soit $ A_n $ le polaire de $ V_n $ dans F. Comme E est bornologique, toute partie bornée de F est équicontinue (III, p. 22, prop. 10), donc contenue dans l’un des $ A_n $. Autrement dit, l’espace F satisfait à la condition (DB).

Montrons que F est semi-tonnelé. Soit $ (U_n)_{n \in \mathbf{N}} $ une suite de voisinages convexes, équilibrés et fermés de 0 dans F. On suppose que l’ensemble $ U = \bigcap_n U_n $ absorbe toute partie bornée de F. Il s’agit de démontrer que U est un voisinage de 0 dans F. Nous allons construire, par récurrence sur l’entier $ n \geqslant 0 $, des nombres réels $ \lambda_n > 0 $

et des voisinages convexes et équilibrés $ W_n $ de 0 dans F, fermés pour $ \sigma(F, E) $, et satisfaisant aux relations
(1)
$$
\lambda_n A_n \subset \frac{1}{2} U \cap (\bigcap_{0 \leq i < n} W_i)
$$
(2)
$$
\bigcup_{0 \leq i \leq n} \lambda_i A_i \subset W_n \subset U_n .
$$

Supposons construits les nombres $ \lambda_i $ et les ensembles $ W_i $ pour $ 0 \leq i < n $. Par hypothèse, l’ensemble U absorbe les parties bornées de F ; de plus, pour $ 0 \leq i < n $, $ W_i $ est un voisinage de 0 dans F, donc absorbe les parties bornées de F. On peut donc trouver un nombre $ \lambda_n > 0 $ satisfaisant à (1). Notons C l’enveloppe fermée convexe équilibrée, pour $ \sigma(F, E) $, de $ \bigcup_{0 \leq i \leq n} \lambda_i A_i $; l’ensemble C est équicontinu, donc compact pour $ \sigma(F, E) $ (III, p. 17, cor. 2). Comme $ U_n $ est un voisinage de 0 dans F, il existe une partie bornée B de E telle que $ B^\circ \subset \frac{1}{2} U_n $. Posons $ W_n = C + B^\circ $. Comme $ B^\circ $ est un voisinage de 0 dans F, on voit que $ W_n $ est un voisinage convexe et équilibré de 0 dans F. De plus, C est compact et $ B^\circ $ fermé pour $ \sigma(F, E) $; d’après le cor. 1 de TG, III, p. 28, $ W_n $ est fermé pour $ \sigma(F, E) $. Enfin, on a $ C \subset \frac{1}{2} U \subset \frac{1}{2} U_n $ et $ B^\circ \subset \frac{1}{2} U_n $, donc $ W_n \subset U_n $ puisque $ U_n $ est convexe. On a donc établi (2).

Posons $ W = \bigcap^n W_n $, d’où $ W \subset U $. D’après (1) et (2), on a $ \lambda_i A_i \subset W_j $ quels que soient $ i $ et $ j $ dans $ \mathbf{N} $, d’où $ \lambda_i A_i \subset W $ pour tout $ i \in \mathbf{N} $. En particulier, W est absorbant, donc c’est un tonneau pour $ \sigma(F, E) $. D’après la remarque 3 de IV, p. 4, W est un voisinage de 0 dans F. *A fortiori*, U est un voisinage de 0 dans F, et F est semi-tonnelé.

Le corollaire suivant étend le th. de Banach-Steinhaus au dual d’un espace de Fréchet (*cf.* III, p. 26, cor. 2).

#### Corollaire {#evt-iv-s3-n2-cor-1 .statement}

*Soit G un espace localement convexe séparé, et soit* $ (u_n) $ *une suite d’applications linéaires de F dans G, convergeant simplement vers une application u de F dans G. Alors u est continue, et la suite* $ (u_n) $ *converge vers u uniformément sur toute partie précompacte de F.*

Comme F est complet, l’ensemble des $ u_n $, qui est borné pour la topologie de la convergence simple, est borné dans $ \mathscr{L}_b(F; G) $ (III, p. 27, cor. 1). Comme l’espace F est semi-tonnelé (prop. 2), toute partie dénombrable et bornée de $ \mathscr{L}_b(F; G) $ est équi-continue d’après la prop. 1 de IV, p. 20. L’ensemble des $ u_n $ est donc équicontinu, et le corollaire résulte alors de III, p. 18, corollaire.

### 3. Bidual d’un espace localement convexe métrisable

#### Proposition 3 {#evt-iv-s3-prop-3 .statement}

*Soient E un espace localement convexe métrisable, $ E'_b $ son dual fort et G un espace de Fréchet. L’espace $ \mathscr{L}_b(E'_b; G) $ est un espace de Fréchet.*

D’après la prop. 2 (IV, p. 21), il existe une suite $ (A_n) $ de parties bornées de $ E'_b $ telle que toute partie bornée de $ E'_b $ soit contenue dans l’une des $ A_n $. Soit $ (V_n) $ un système fondamental dénombrable de voisinages de 0 dans G. Soit $ H_{mn} $ l’ensemble des applications linéaires $ u $ de $ E'_b $ dans G telles que $ u(A_m) \subset V_n $. Alors $ (H_{mn}) $ est un système fondamental de voisinages de 0 dans $ \mathcal{L}_b(E'_b ; G) $, et ce dernier espace est donc métrisable.

Pour montrer que $ \mathcal{L}_b(E'_b ; G) $ est complet, il suffit de prouver que toute suite de Cauchy $ (u_n) $ dans cet espace est convergente ; comme G est complet, il existe une application linéaire $ u : E'_b \to G $ telle que $ (u_n) $ converge simplement vers $ u $. D’après IV, p. 22, corollaire, on a $ u \in \mathcal{L}(E'_b ; G) $. Il résulte alors de la prop. 5 de TG, X, p. 6, que $ (u_n) $ converge vers $ u $ dans $ \mathcal{L}_b(E'_b ; G) $.

#### Corollaire {#evt-iv-s3-n3-cor-1 .statement}

*Le bidual d’un espace localement convexe métrisable est un espace de Fréchet.*

### 4. Dual d’un espace de Fréchet réflexif

#### Proposition 4 {#evt-iv-s3-prop-4 .statement}

*Soit E un espace de Fréchet réflexif. Le dual fort $ E'_b $ de E est limite inductive d’une suite d’espaces de Banach.*

Soit $ (V_n)_{n \in \mathbf{N}} $ une suite décroissante de voisinages convexes, équilibrés et fermés de 0 dans E, telle que tout voisinage de 0 dans E contienne l’un des $ V_n $. Soit $ A_n $ le polaire de $ V_n $ dans $ E' $. Alors $ A_n $ est convexe, équilibré, et compact pour $ \sigma(E', E) $; d’après III, p. 8, corollaire, l’espace $ E'_{A_n} $ est un espace de Banach. Nous allons prouver que $ E'_b $ est limite inductive des espaces $ E'_{A_n} $, autrement dit que *toute partie convexe et équilibrée U de $ E' $ qui absorbe chacun des $ A_n $ est un voisinage de 0 dans $ E'_b $*. Pour tout $ n \in \mathbf{N} $, choisissons un nombre réel $ \lambda_n > 0 $ tel que $ \lambda_n A_n \subset U $. Soit $ B_n $ l’enveloppe convexe de l’ensemble $ \bigcup_{0 \leq i \leq n} \lambda_i A_i $; posons $ V = \bigcup_n B_n $, d’où $ V \subset U $. Pour tout $ n \in \mathbf{N} $, l’ensemble $ B_n $ est convexe, équilibré et compact pour $ \sigma(E', E) $ (II, p. 14, prop. 15).

Montrons que l’on a $ \frac{1}{2} V^{oo} \subset V $. Soit $ x \in E'_b - V $; pour tout $ n \in \mathbf{N} $, on a $ x \notin B_n $, et comme $ B_n $ est fermée pour $ \sigma(E', E) $, il existe un élément $ y_n $ de $ B_n^o $ tel que $ \langle y_n, x \rangle = 1 $ (II, p. 41, prop. 4). Comme E est réflexif, toute partie bornée de E est relativement compacte pour $ \sigma(E, E') $ (IV, p. 16, th. 2). D’après la définition de $ B_n $, on a

$$
\lambda_i y_n \in V_i \quad \text{pour tout } n \geq i,
$$

donc la suite $ (y_n) $ est bornée. Soit $ y $ une valeur d’adhérence de $ (y_n) $ pour la topologie $ \sigma(E, E') $. On a $ y \in V^o = \bigcap_n B_n^o $ et $ \langle y, x \rangle = 1 $. On a donc $ x \notin \frac{1}{2} V^{oo} $, d’où l’inclusion $ \frac{1}{2} V^{oo} \subset V $ et *a fortiori* $ \frac{1}{2} V^{oo} \subset U $.

Comme toute partie bornée de $ E'_b $ est contenue dans l’un des ensembles $ A_n $, l’ensemble $ V = \bigcup_n B_n $ absorbe toute partie bornée de $ E'_b $. Par suite, $ V^o $ est borné dans E, donc $ \frac{1}{2} V^{oo} $ est un voisinage de 0 dans $ E'_b $. *A fortiori* U est un voisinage de 0 dans $ E'_b $.

#### Corollaire {#evt-iv-s3-n4-cor-1 .statement}

*Le dual fort d’un espace de Fréchet réflexif est bornologique et tonnelé.*

Une limite inductive d’espaces de Banach est bornologique par définition. Par ailleurs, un espace de Banach est tonnelé (III, p. 25, corollaire) et toute limite inductive d’espaces tonnelés est un espace tonnelé (III, p. 25, cor. 3).

### 5. La topologie de la convergence compacte sur le dual d’un espace de Fréchet

#### Théorème 1 (Banach-Dieudonné) {#evt-iv-s3-thm-1 .statement}

Soit E un espace localement convexe métrisable. Sur le dual E' de E, les topologies suivantes coïncident :
a) la topologie $ \mathcal{T}_{\mathfrak{N}} $ de la $ \mathfrak{N} $-convergence, où $ \mathfrak{N} $ est l’ensemble des parties de E dont chacune est formée des points d’une suite convergeant vers 0 ;
b) la topologie $ \mathcal{T}_c $ de la convergence uniforme sur les parties compactes de E ;
c) la topologie $ \mathcal{T}_{pc} $ de la convergence uniforme sur les parties précompactes de E ;
d) la topologie $ \mathcal{T}_f $ la plus fine induisant la même topologie que $ \sigma(E', E) $ sur toute partie équicontinue de E'.

Remarquons d’abord qu’une partie A de E' est fermée pour $ \mathcal{T}_f $ si et seulement si $ A \cap H $ est fermé pour $ \sigma(E', E) $ quelle que soit la partie H de E', équicontinue et fermée pour $ \sigma(E', E) $. Sur toute partie équicontinue de E', la topologie faible $ \sigma(E', E) $ et $ \mathcal{T}_{pc} $ induisent la même topologie (III, p. 17, prop. 5). Par suite, chacune des topologies $ \mathcal{T}_{\mathfrak{N}}, \mathcal{T}_c, \mathcal{T}_{pc}, \mathcal{T}_f $ est moins fine que la suivante. Il suffit donc de prouver que $ \mathcal{T}_{\mathfrak{N}} $ est plus fine que $ \mathcal{T}_f $. De plus, toute translation dans E' est un homéomorphisme pour $ \mathcal{T}_f $. Il suffit donc de prouver que, si F est une partie de E' fermée pour $ \mathcal{T}_f $, ne contenant pas 0, il existe un ensemble $ S \in \mathfrak{N} $ tel que $ S^\circ \cap F = \varnothing $.

Soit $ (U_n)_{n \geq 0} $ une suite décroissante de voisinages de 0 dans E, formant un système fondamental de voisinages de 0. Nous allons construire, par récurrence sur $ n \geq 0 $, des ensembles finis $ X_n $ tels que l’on ait

(4)
$$
X_n \subset U_n
$$
(5)
$$
(\bigcup_{0 \leq p \leq n} X_p)^\circ \cap U_{n+1}^\circ \cap F = \varnothing
$$

pour tout entier $ n \geq 0 $. Soit $ m \geq 0 $ un entier tel que $ X_n $ soit déjà construit pour $ 0 \leq n < m $ et satisfasse à (4) et (5) pour $ 0 \leq n < m $. Pour tout $ x \in U_m $, posons
$$
F_x = (\bigcup_{0 \leq p < m} X_p)^\circ \cap \{x\}^\circ \cap U_{m+1}^\circ \cap F.
$$

La formule (5), où l’on fait $ n = m - 1 $ entraîne $ \bigcap_{x \in U_m} F_x = \varnothing $. Par ailleurs, l’ensemble $ U_{m+1}^\circ $ est équicontinu, et compact pour $ \sigma(E', E) $. Vu la définition de $ \mathcal{T}_f $, chacun des ensembles $ F_x $ est compact pour $ \sigma(E', E) $; il existe donc une partie finie $ X_m $ de $ U_m $ telle que $ \bigcap_{x \in X_m} F_x = \varnothing $, c’est-à-dire que la relation (5) est satisfaite pour $ n = m $.

Posons $ S = \bigcup_{n \geq 0} X_n $. On a $ X_n \subset U_p $ pour $ n \geq p $, donc S est l’ensemble des points d’une suite qui converge vers 0 dans E. De (5), on déduit $ S^\circ \cap U_{n+1}^\circ \cap F = \varnothing $, d’où $ S^\circ \cap F = \varnothing $ car E' est réunion de la suite des ensembles $ U_{n+1}^\circ $.

#### Corollaire 1 {#evt-iv-s3-thm-1-cor-1 .statement}

Soit E un espace localement convexe métrisable. Toute partie précompacte de E est contenue dans l’enveloppe fermée convexe équilibrée de l’ensemble des points d’une suite convergeant vers 0.

Cela résulte de l’identité des topologies $ \mathcal{T}_{pc} $ et $ \mathcal{T}_\mathfrak{K} $, compte tenu de la prop. 2 de III, p. 15.

#### Corollaire 2 {#evt-iv-s3-thm-1-cor-2 .statement}

*Soit E un espace de Fréchet. Pour qu’une partie convexe A du dual E’ de E soit fermée pour $ \sigma(E', E) $, il faut et il suffit que $ A \cap U^\circ $ soit fermé pour $ \sigma(E', E) $ quel que soit le voisinage U de 0 dans E.*

Puisque E est complet, la topologie $ \mathcal{T}_c $ sur E’ est compatible avec la dualité entre E’ et E (IV, p. 3, Exemple); par suite les parties convexes fermées dans E’ sont les mêmes pour $ \mathcal{T}_c $ et $ \sigma(E', E) $ (IV, p. 1, prop. 1). Le corollaire résulte alors de l’identité des topologies $ \mathcal{T}_c $ et $ \mathcal{T}_f $.

Rappelons (I, p. 13) que les hyperplans de E’ fermés pour $ \sigma(E', E) $ sont les noyaux des formes linéaires sur E’ associées aux éléments de E. Le cor. 2 fournit donc une autre démonstration (pour les espaces de Fréchet) du cor. 1 de III, p. 21.

#### Corollaire 3 {#evt-iv-s3-thm-1-cor-3 .statement}

*Soient E un espace de Banach et M un sous-espace vectoriel du dual E’ de E. Pour que M soit fermé pour la topologie faible $ \sigma(E', E) $, il faut et il suffit que son intersection avec la boule unité (fermée) dans E’ soit fermée pour $ \sigma(E', E) $.*

#### Exemple {#evt-iv-s3-n5-exa-1 .statement}

*Soit H un espace hilbertien de type dénombrable; on note $ H_\sigma $ l’espace H muni de la topologie affaiblie. Soit $ \mathcal{L}^1(H) $ l’espace de Banach des endomorphismes nucléaires de H (V, p. 50, et TS, V); la norme dans $ \mathcal{L}^1(H) $ est définie par $ \|u\|_1 = \operatorname{Tr}((u^*u)^{1/2}) $. On peut identifier $ \mathcal{L}(H) $ au dual de l’espace de Banach $ \mathcal{L}^1(H) $ en associant à tout $ u \in \mathcal{L}(H) $ la forme linéaire $ \varphi_u : v \mapsto \operatorname{Tr}(uv) $ sur $ \mathcal{L}^1(H) $. Soit A une sous-algèbre de $ \mathcal{L}(H) $, contenant 1 et stable par $ u \mapsto u^* $; c’est une algèbre de von Neumann si et seulement si elle est fermée dans $ \mathcal{L}(H) $ pour la topologie faible $ \sigma(\mathcal{L}(H), \mathcal{L}^1(H)) $. On déduit du cor. 3 le critère suivant : pour que A soit une algèbre de von Neumann, il faut et il suffit que pour toute suite $ (u_n) $ d’éléments de norme $ \leqslant 1 $ de A admettant une limite u dans l’espace $ \mathcal{L}_s(H ; H_\sigma) $, u appartienne à A. \*

### 6. Applications bilinéaires séparément continues

#### Lemme 1 {#evt-iv-s3-lem-1 .statement}

*Soient E et F deux espaces localement convexes métrisables, et u une application linéaire continue de $ E'_b $ dans F. Il existe un voisinage U de 0 dans $ E'_b $ dont l’image par u est bornée dans F.*

Soit $ (U_n)_{n \in \mathbf{N}} $ (resp. $ (V_n)_{n \in \mathbf{N}} $) un système fondamental de voisinages de 0 dans E (resp. F). On suppose que les ensembles $ U_n $ sont équilibrés et forment une suite décroissante. Comme u est continue, il existe pour tout $ n \in \mathbf{N} $ un ensemble borné $ B_n $ dans E tel que $ u(B_n^\circ) \subset V_n $. Comme $ B_n $ est borné, il existe un nombre réel $ \lambda_n > 0 $ tel que $ \lambda_n B_n \subset U_n $. Posons $ B = \bigcup_{n \in \mathbf{N}} \lambda_n B_n $.

Nous allons prouver que l’ensemble B est borné dans E, autrement dit que pour tout entier $ m \geqslant 0 $, il existe un nombre réel $ \mu > 0 $ tel que $ \mu B \subset U_m $. Comme les ensembles $ B_n $ sont bornés, il existe un nombre réel $ \mu $ tel que $ 0 < \mu \leqslant 1 $ et que $ \mu (\lambda_n B_n) \subset U_m $ pour $ 0 \leqslant n \leqslant m $; on a par ailleurs $ \lambda_n B_n \subset U_n \subset U_m $ si $ n > m $, d’où $ \mu B \subset U_m $ puisque $ U_m $ est équilibré.

Soit U le polaire de B dans $ E'_b $. C’est un voisinage de 0 dans $ E'_b $ et l’on a $ \lambda_n B^\circ \subset B_n^\circ $, d’où $ \lambda_n u(U) \subset V_n $ pour tout $ n \in \mathbf{N} $. Par suite $ u(U) $ est borné dans F.

#### Théorème 2 {#evt-iv-s3-thm-2 .statement}

Soient $ E_1 $ et $ E_2 $ deux espaces de Fréchet réflexifs, et $ G $ un espace localement convexe séparé. Pour $ i = 1, 2 $, soit $ F_i $ le dual fort de $ E_i $. Alors toute application bilinéaire séparément continue $ u : F_1 \times F_2 \to G $ est continue.

L’espace $ G $ est isomorphe à un sous-espace d’un produit d’espaces de Banach (II, p. 5, prop. 3). Il suffit donc de prouver le théorème sous l’hypothèse supplémentaire que $ G $ est un espace de Banach. Or $ F_1 $ est tonnelé et $ F_2 $ bornologique (IV, p. 23, corollaire), et $ \mathcal{L}_b(F_2 ; G) $ est un espace de Fréchet (IV, p. 22, prop. 3). Notons $ v $ l’application linéaire de $ F_1 $ dans $ \mathcal{L}_b(F_2 ; G) $ associée à $ u $ par la relation
$$
u(x_1, x_2) = v(x_1)(x_2) \quad (x_1 \in F_1, x_2 \in F_2).
$$
Comme $ F_1 $ est tonnelé et $ u $ séparément continue, $ v $ est continue (III, p. 32, prop. 6).

Comme $ v $ est continue, le lemme 1 entraîne l’existence d’un voisinage $ U_1 $ de 0 dans $ F_1 $ dont l’image par $ v $ soit bornée dans $ \mathcal{L}_b(F_2 ; G) $. Autrement dit, pour tout ensemble borné $ B_2 $ dans $ F_2 $, l’ensemble $ u(U_1 \times B_2) $ est borné dans l’espace de Banach $ G $. Soit $ U_2 $ l’ensemble des $ x_2 \in F_2 $ tels que l’on ait $ \|u(x_1, x_2)\| \leq 1 $ pour tout $ x_1 \in U_1 $. L’ensemble $ U_2 $ absorbe donc tout ensemble borné ; comme $ F_2 $ est bornologique, $ U_2 $ est donc un voisinage de 0 dans $ F_2 $, ce qui prouve que $ u $ est continue.

## EXERCICES {#evt-iv-s3-exercises}

See the [exercises for § 3](exercises/s3/).
