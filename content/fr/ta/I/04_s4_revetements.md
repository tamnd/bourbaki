---
book: ta
book_title: Topologie algébrique
chapter: I
chapter_title: REVÊTEMENTS
section: 4
section_title: Revêtements
lang: fr
source: ta-i-iv-fr
book_pages: TA I.68-TA I.90, TA I.145-TA I.147
pdf_pages: 0084-0106, 0161-0163
extraction: native
subsections:
    - "no": 1
      title: Espaces fibrés localement triviaux
      page: 68
      pdf_page: 84
    - "no": 2
      title: Revêtements
      page: 69
      pdf_page: 85
    - "no": 3
      title: Produits et produits fibrés
      page: 71
      pdf_page: 87
    - "no": 4
      title: Degré d’un revêtement
      page: 73
      pdf_page: 89
    - "no": 5
      title: Revêtements finis
      page: 75
      pdf_page: 91
    - "no": 6
      title: Revêtements des espaces localement connexes
      page: 79
      pdf_page: 95
    - "no": 7
      title: Revêtements d’un espace paracompact
      page: 84
      pdf_page: 100
    - "no": 8
      title: Faisceaux localement constants
      page: 86
      pdf_page: 102
    - "no": 9
      title: Produits de faisceaux localement constants
      page: 87
      pdf_page: 103
    - "no": 10
      title: Morphismes de faisceaux localement constants sur un espace localement connexe
      page: 89
      pdf_page: 105
statements: 50
exercises: 9
content_sha256: b223342ad6235f2feedc9185ea923d98d548abd3077ff7d001d2ae40063239a4
---

## § 4. REVÊTEMENTS

### 1. Espaces fibrés localement triviaux

Soit B un espace topologique. Si F est un espace topologique, on appelle B-espace fibré trivial de fibre-type F le B-espace $(B\times F$, pr$_1)$.

Soit E un B-espace. S’il existe un espace topologique F et un B-isomorphisme $u: E\rightarrow B\times F$, on dit que le B-espace E est un B-espace fibré trivialisable et que $u$ en est une trivialisation de fibre-type F.

#### Définition 1 {#ta-i-s4-def-1 .statement tag=01OR}

Soit B un espace topologique. Soit E un B-espace et soit $p$ sa projection. On dit que E est un B-espace fibré localement trivial si tout point de B possède un voisinage V tel que $(\overset{-1}{p}(V), p_V)$ soit un V-espace fibré trivialisable.

Au lieu de « B-espace fibré localement trivial », on dit également « espace fibré localement trivial de base B ». Si E est un B-espace fibré localement trivial, on dit parfois que $(E,B, p)$ est une fibration localement triviale, ou, par abus, que $p$ est une fibration localement triviale. On dit aussi qu’un B-espace $(E, p)$ est trivialisable au-dessus d’une partie A de B si le A-espace $E_A$ induit par $(E, p)$ au-dessus de A est un espace fibré trivialisable.

Soit E un B-espace fibré localement trivial ; notons $p$ sa projection.

L’ensemble des points $a$ de B tels que la fibre $\overset{-1}{p}(a)$ soit vide (resp. non vide) est ouvert. L’image de $p$ est donc une partie ouverte et fermée de B.

Soit F un espace topologique. Si toutes les fibres de E sont homéo-morphes à F, on dit que E est un B-espace fibré localement trivial de fibre-type F.

#### Remarque 1 {#ta-i-s4-n1-rem-1 .statement tag=01OS}

Soit $(E, p)$ un B-espace fibré localement trivial et soit A une partie de B. Le A-espace $E_A= (\overset{-1}{p}(A), p_A)$ déduit de E par passage aux sous-espaces est un espace fibré localement trivial. Si E est trivialisable, il en est de même de $E_A$.

En effet, pour tout point $a$ de A, il existe un voisinage ouvert U de $a$ dans B, un espace topologique F et un U-isomorphisme $g:\overset{-1}{p}(U)\rightarrow$ $U\times F$. L’application $f$ induit un $(A\cap U)$-isomorphisme de $p^{-1}_A(A\cap U)$ sur $(A\cap U)\times F$, ce qui prouve que $E_A$ est un A-espace fibré localement trivial.

#### Remarque 2 {#ta-i-s4-n1-rem-2 .statement tag=01OT}

Soit $(E, p)$ un B-espace et soit $(E_i)_{i\in I}$ une partition de E formée d’ouverts.

Si chacun des B-espaces $(E_i, p|E_i)$ est un espace fibré trivialisable, E est un B-espace fibré trivialisable. En effet, pour chaque $i\in I$, soit $F_i$ un espace topologique tel que les B-espaces $(E_i, p|E_i)$ et $(B\times F_i$, pr$_1)$ soient isomorphes. Alors le B-espace $(E, p)$ est isomorphe à $(B\times F$, pr$_1)$, où F est l’espace topologique somme de la famille $(F_i)_{i\in I}$.

Supposons l’ensemble I fini. Si chacun des B-espaces $(E_i, p|E_i)$ est un B-espace fibré localement trivial, il en est de même du B-espace E. En effet, puisque l’ensemble I est fini, chaque point de B possède un voisinage U au-dessus duquel les B-espaces fibrés $E_i$ sont tous trivialisables. D’après ce qui précède, le U-espace $(\overset{-1}{p}(U), p_U)$ est alors un espace fibré trivialisable.

### 2. Revêtements

#### Définition 2 {#ta-i-s4-def-2 .statement tag=01OU}

On appelle revêtement un espace fibré localement trivial dont toutes les fibres sont discrètes.

Au lieu de dire qu’un B-espace E est un revêtement, on dit aussi que E est un revêtement de B.

Soit E un B-espace, notons $p$ sa projection ; soit A une partie de B. Si E est un revêtement de B, les fibres de $p$ sont discrètes, donc celles de $p_A:\overset{-1}{p}(A)\rightarrow A$ aussi et le A-espace fibré localement trivial $(\overset{-1}{p}(A), p_A)$ est un revêtement.

#### Proposition 1 {#ta-i-s4-prop-1 .statement tag=01OV}

Soient B et E des espaces topologiques et soit $p: E\rightarrow B$ une application. Les conditions suivantes sont équivalentes :

(i) L’application $p$ est continue et le B-espace $(E, p)$ est un revêtement trivialisable ;

(ii) Il existe une partition $(V_i)_{i\in I}$ de E formée d’ensembles ouverts telle que, pour tout $i\in I$, l’application $p|V_i: V_i\rightarrow B$ soit un homéomorphisme.

Supposons que la condition (i) soit vérifiée et soit $g: E\rightarrow B\times F$ une trivialisation du B-espace $(E, p)$, de fibre-type F. Par suite, F est un espace topologique discret et, les ensembles $V_i=\overset{-1}{g}(B\times  \{i\})$, pour $i\in F$, forment une partition de E formée d’ensembles ouverts. Pour tout $i$, l’application $p|V_i: V_i\rightarrow B$ est un homéomorphisme, d’homéomorphisme réciproque l’application $x\mapsto g^{-1}(x, i)$, d’où la condition (ii).

Inversement, supposons que la condition (ii) soit satisfaite. L’application $p$ est alors continue. Considérons l’application de E dans $B\times I$ qui à $x\in E$ associe le couple $(p(x), i)$, où $i$ est l’unique élément de I telle que $x\in V_i$. Si I est muni de la topologie discrète, la condition (ii) signifie que cette application est un B-isomorphisme et le B-espace $(E, p)$ est un revêtement trivialisable.

#### Corollaire 1 {#ta-i-s4-prop-1-cor-1 .statement tag=01OW}

Soient B et E des espaces topologiques et soit $p: E\rightarrow B$ une application. Pour que E, muni de l’application $p$, soit un revêtement de B, il faut et il suffit que, pour tout point $a$ de B, il existe un voisinage ouvert U de $a$ et une partition $(V_i)_{i\in I}$ de $\overset{-1}{p}(U)$ formée d’ensembles ouverts de E telle que, pour tout $i\in I$, l’application $p$ induise un homéomorphisme de $V_i$ sur U.

#### Remarque {#ta-i-s4-n2-rem-1 .statement tag=01OX}

Soit B un espace topologique. Soit E un B-espace et soit $p$ sa projection. Si E est un revêtement de B, il résulte du corollaire 1 ci-dessus, que l’application $p$ est étale (I, p. 28, déf. 2) et séparée (I, p. 25, prop. 1, (iii)). Ces conditions ne suffisent cependant pas à assurer que E soit un revêtement. Considérons par exemple un ensemble ouvert U de B. L’injection canonique $i: U\rightarrow B$ est étale et séparée. Pour que le B-espace $(U, i)$ soit un revêtement, il faut et il suffit que l’ensemble ouvert U soit aussi fermé.

#### Corollaire 2 {#ta-i-s4-prop-1-cor-2 .statement tag=01OY}

Soit B un espace topologique, soit E un B-espace et soit $p$ sa projection. Supposons que $p$ soit étale et séparée et que l’espace B soit connexe. Pour que E soit un revêtement trivialisable de B, il faut et il suffit que, pour tout point $x$ de E, il existe une section continue $s: B\rightarrow E$ de $p$ telle que $s\circ p(x) =x$.

C’est évidemment nécessaire. Inversement, pour toute section continue $s$ de $p$, l’ensemble $s(B)$ est ouvert et l’application $p$ induit un homéomorphisme de $s(B)$ sur B (I, p. 30, cor. 3 de la prop. 6). En outre, lorsque $s$ parcourt l’ensemble $\mathscr{S}(B; E)$ des sections de $p$, les ensembles $s(B)$ sont deux à deux disjoints, car B est connexe (I, p. 34, cor. 1 de la prop. 11). Il résulte alors de la proposition 1 que si les ensembles $s(B)$ recouvrent E, l’espace E est un revêtement trivialisable de B.

### 3. Produits et produits fibrés

#### Proposition 2 {#ta-i-s4-prop-2 .statement tag=01OZ}

Soient B et $B'$ des espaces topologiques, soit $(E, p)$ un B-espace et soit $(E', p')$ un $B'$-espace. Supposons que E et $E'$ soient des espaces fibrés localement triviaux ( resp. des revêtements). L’espace $E\times E'$, muni de l’application $p\times p': E\times E'\rightarrow B\times B'$, est alors un espace fibré localement trivial ( resp. un revêtement) de base $B\times B'$. Si E et $E'$ sont trivialisables, il en est de même de $E\times E'$.

Supposons d’abord que le B-espace E et le $B'$-espace $E'$ admettent des trivialisations $g: E\rightarrow B\times F,g': E'\rightarrow B'\times F'$; l’application composée de l’homéomorphisme $g\times g'$ de $E\times E'$ sur $(B\times F)\times (B'\times F')$ et de l’homéomorphisme canonique de $(B\times F)\times (B'\times F')$ sur $(B\times B')\times (F\times F')$ est une trivialisation du $B\times B'$-espace $E\times E'$, de fibre-type $F\times F'$. Si F et $F'$ sont des espaces discrets, l’espace $F\times F'$ est aussi discret.

Dans le cas général, pour tout point $(a, a')$ de $B\times B'$, il existe un voisinage U de $a$ dans B et un voisinage $U'$ de $a'$ dans $B'$ tels que le U-espace $E_U$ et le $U'$-espace $E'_{U'}$ soient trivialisables. Il résulte de ce qui précède que le $B\times B'$-espace $E\times E'$ est trivialisable au-dessus de $U\times U'$. C’est donc un espace fibré localement trivial de base $B\times B'$. Ses fibres sont discrètes si E et $E'$ sont des revêtements, d’où la proposition.

On remarquera que, si $(p_i: E_i\rightarrow B_i)_{i\in I}$ est une famille d’espaces fibrés localement triviaux, ou même de revêtements, l’espace produit $\prod_{i\in I}E_i$ muni de l’application $(p_i)_{i\in I}$ n’est pas nécessairement un espace fibré localement trivial de base $\prod_{i\in I}B_i($I, p. 145, exerc. 3).

#### Corollaire 1 {#ta-i-s4-prop-2-cor-1 .statement tag=01P0}

Soient A un espace topologique, B, $B'$ des A-espaces. Soient E et $E'$ des espaces fibrés localement triviaux ( resp. des revêtements) de bases B et $B'$; notons $p$ et $p'$ leurs projections. Le $B\times_AB'$-espace $E\times_AE'$ déduit de $p\times p'$ par passage aux sous-espaces est alors un espace fibré localement trivial ( resp. un revêtement). Il est trivialisable si E et $E'$ le sont.

Puisque l’ensemble $E\times_AE'$ est l’image réciproque de $B\times_AB'$ par l’application $p\times p': E\times E'\rightarrow B\times B'$, le corollaire résulte de la proposition 2 et de la remarque 1 (I, p. 68).

#### Corollaire 2 {#ta-i-s4-prop-2-cor-2 .statement tag=01P1}

Soit

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

un carré cartésien. Si $(E, p)$ est un B-espace fibré localement trivial ( resp. un revêtement), alors $(E', p')$ est un espace fibré localement trivial ( resp. un revêtement) de base $B'$, trivialisable si $(E, p)$ l’est.

Cela résulte du corollaire 1, appliqué avec B = A et $E'= B'$.

#### Corollaire 3 {#ta-i-s4-prop-2-cor-3 .statement tag=01P2}

Soit B un espace topologique. Soient E et $E'$ des B-espaces fibrés localement triviaux ( resp. des revêtements). Alors $E\times_BE'$ est un B-espace fibré localement trivial ( resp. un revêtement de B). Il est trivialisable si E et $E'$ le sont.

Cela résulte du corollaire 1, appliqué au cas où A, B et $B'$ sont égaux.

#### Proposition 3 {#ta-i-s4-prop-3 .statement tag=01P3}

Soit

${E'}^{f'}$ E

$$
p'p \tag{1}
$$

${B'}^f$ B

un carré cartésien. Supposons qu’au voisinage de tout point de B, l’application $f$ possède une section continue. Alors, si $(E', p')$ est un $B'$-espace fibré localement trivial ( resp. un revêtement), le B-espace $(E, p)$ est un espace fibré localement trivial ( resp. un revêtement).

Il s’agit de démontrer que tout point $a$ de B possède un voisinage U tel que le U-espace induit par $(E, p)$ au-dessus de U soit un espace fibré localement trivial (resp. un revêtement). Prenons pour U un voisinage de $a$ au-dessus duquel il existe une section continue $s$ de $f$. Notons $i: U\rightarrow B$ et $j:\overset{-1}{p}(U)\rightarrow E$ les injections canoniques. Comme le carré (1) est cartésien, il existe une unique application continue $s':\overset{-1}{p}(U)\rightarrow E'$ telle que $f'\circ s'=j$ et $p'\circ s'=s\circ p_U$. Le carré

$$
\overset{-1}{p}(U)^{s'}E'
$$

$$
p_{_U}p' \tag{2}
$$

U $^sB'$

est ainsi commutatif et son composé avec le carré (1) est le carré cartésien

$\overset{-1}{p}(U)^j$ E

$p_Up$

U $^iB$.

D’après la proposition 7 de I, p. 15, le carré (2) est cartésien. Le corollaire 2 permet de conclure.

#### Remarque {#ta-i-s4-n3-rem-1 .statement tag=01P4}

Si dans la proposition 3, on affaiblit l’hypothèse sur l’application $f$ en la supposant seulement universellement stricte et surjective, et si $p'$ est un revêtement, l’application $p$ est étale (I, p. 31, prop. 8) et séparée (I, p. 27, prop. 4) mais E n’est pas nécessairement un revêtement de B. On peut trouver par exemple un espace topologique B et un recouvrement fermé localement fini $(A_i)_{i\in I}$ de B, un B-espace $(E, p)$ qui n’est pas un revêtement mais tel que, pour tout $i\in I$, le $A_i$-espace induit $E_{A_i}$ soit un revêtement de $A_i($I, p. 146, exerc. 5). Pour une condition suffisante, voir cependant le corollaire 4 de I, p. 77.

### 4. Degré d’un revêtement

Soit B un espace topologique, soit E un revêtement de B, notons $p$ sa projection. Notons C l’ensemble des cardinaux Card($\overset{-1}{p}(b)$), où $b$ parcourt B. L’application $b\mapsto$ Card($\overset{-1}{p}(b)$) est une application localement constante de B dans C. On dit que le revêtement E possède un degré si B n’est pas vide et si l’application $b\mapsto$ Card($\overset{-1}{p}(b)$) est constante. La valeur commune des cardinaux Card($\overset{-1}{p}(b)$), pour $b\in B$, est alors appelée le degré du revêtement E et est notée deg(E$, p)$, voire [E: B] s’il ne peut y avoir d’ambiguïté sur l’application $p$.

Si B n’est pas vide, le revêtement trivial de base B et de fibre-type F possède un degré qui est égal à Card(F).

Si B est connexe, la fonction $b\mapsto$ Card($\overset{-1}{p}(b)$) est constante. Par suite :

#### Proposition 4 {#ta-i-s4-prop-4 .statement tag=01P5}

Tout revêtement d’un espace connexe non vide possède un degré.

Soit G un espace topologique, soit $(F, g)$ un revêtement de G et soit $(E, f)$ un revêtement de F ; supposons que ces revêtements possèdent un degré. Si le G-espace $(E, g\circ f)$ est un revêtement, il possède alors un degré et l’on a deg(E$, g\circ f) =$ deg(F$, g)$ deg(E$, f)$, ce qu’on peut aussi écrire

$$
[E : G] = [E : F] [F : G]
$$

En effet, si $z$ est un point de G, toutes les fibres de l’application

$$
f_{\overset{-1}{g}(z)}:\overset{-1}{f}(\overset{-1}{g}(z))\rightarrow \overset{-1}{g}(z)
$$

ont pour cardinal deg(E$, f)$, et $\overset{-1}{g}(z)$ a pour cardinal deg(F$, g)$. L’assertion résulte donc du principe des bergers (E, III, p. 41, prop. 9).

Soient B et $B'$ des espaces topologiques, soit $(E, p)$ un revêtement de B et soit $(E', p')$ un revêtement de $B'$. Supposons que ces revêtements possèdent un degré ; alors, le revêtement $(E\times E', p\times p')$ de $B\times B'$ (I, p. 71, prop. 2) possède un degré et l’on a :

deg(E $\times E', p\times p') =$ deg(E$, p)$ deg(E$', p')$.

En effet, pour tout couple $(b, b')\in B\times B'$, la fibre $(E\times E')_{(b,b')}$ est le produit $E_b\times E'_{b'}$.

Soient B et $B'$ des espaces topologiques, $(E, p)$ un revêtement de B, $(E', p')$ un revêtement de $B'$ et soit

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

un carré cartésien. Si $B'$ n’est pas vide et si le revêtement $(E, p)$ possède un degré, alors le revêtement $(E', p')$ possède un degré, égal à celui de E, d’après I, p. 10, cor. de la prop. 4.

### 5. Revêtements finis

On dit qu’un revêtement est localement fini si les cardinaux de toutes ses fibres sont finis. On dit qu’un revêtement est fini si l’ensemble des cardinaux de ses fibres est majoré par un cardinal fini.

#### Théorème 1 {#ta-i-s4-thm-1 .statement tag=01P6}

Soient E, B des espaces topologiques et $p: E\rightarrow B$ une application. Les conditions suivantes sont équivalentes :

(i) L’espace E, muni de l’application $p$, est un revêtement localement fini de B ;

(ii) L’application $p$ est étale, propre et séparée ;

(iii) L’application $p$ est continue, ouverte et séparée, ses fibres sont finies et la fonction numérique $b\mapsto$ Card($\overset{-1}{p}(b)$) est semi-continue supérieurement sur B (TG, IV, p. 28).

Nous utiliserons dans la démonstration le lemme suivant :

#### Lemme {#ta-i-s4-n5-lem-1 .statement tag=01P7}

Soient X et Y des espaces topologiques. Pour qu’une application $f: X\rightarrow Y$ soit fermée, il faut et il suffit que pour tout point $y$ de Y et tout voisinage W de la fibre $\overset{-1}{f}(y)$, il existe un voisinage V

de $y$ tel que W contienne $\overset{-1}{f}(V)$.

Dans cet énoncé, on peut ne considérer que les voisinages W de $\overset{-1}{f}(y)$ qui sont ouverts. En notant F le complémentaire de W dans Y, on peut alors reformuler l’énoncé de la façon suivante : pour qu’une application $f: X\rightarrow Y$ soit fermée, il faut et il suffit que, pour toute partie fermée F de X, tout point $y$ de Y qui n’appartient pas à $f(F)$ possède un voisinage V disjoint de $f(F)$. Or cette assertion résulte immédiatement de la définition d’une application fermée (TG, I, p. 30, déf. 1).

Démontrons maintenant le théorème 1. Chacune des trois conditions implique que l’application $p$ est continue, ouverte et séparée, et aussi que les fibres de $p$ sont finies. C’est clair sous les hypothèses (i) et (iii) ; sous l’hypothèse (ii), les fibres de $p$ sont discrètes (I, p. 29, remarque 2) et quasi-compactes (TG, I, p. 75, th. 1) donc finies (TG, I, p. 60, exemple 1).

(i)$\Rightarrow$(ii) : il suffit de démontrer que $p$ est propre et, pour cela, que pour tout ouvert U au-dessus duquel le revêtement $(E, p)$ est trivialisable, l’application $p_U:\overset{-1}{p}(U)\rightarrow U$ est propre (TG, I, p. 72, prop. 3). Comme les fibres de $p_U$ sont finies, cette dernière assertion résulte du corollaire 5 de TG, I, p. 77.

(ii)$\Rightarrow$(iii) : soit $b$ un point de B et, pour tout $x\in \overset{-1}{p}(b)$, soit $W_x$ un voisinage ouvert de $x$ dans E tel que $p|W_x$ soit injectif. L’ensemble $W =\bigcup_{x\in\overset{-1}{p}(b)}W_x$ est un voisinage ouvert de $\overset{-1}{p}(b)$. Comme l’application $p$ est fermée, il existe d’après le lemme ci-dessus un voisinage ouvert U de $b$ tel que $\overset{-1}{p}(U)\subset W$. Pour tout $a\in U$, on a $\overset{-1}{p}(a)\subset W$ ; comme la restriction de $p$ à chaque $W_x$ est injective, il en résulte que Card($\overset{-1}{p}(a)$)$\leqslant$ Card($\overset{-1}{p}(b)$), ce qui prouve la semi-continuité supérieure de l’application $a\mapsto$ Card($\overset{-1}{p}(a)$).

(iii)$\Rightarrow$(i) : soit $b$ un point de B. Comme la fibre $E_b=\overset{-1}{p}(b)$ est finie et l’application $p$ séparée, on peut choisir, pour tout $x\in E_b$, un voisinage ouvert $V'_x$ de $x$ de telle sorte que les $V'_x$ soient deux à deux disjoints (I, p. 26, remarque 4). Comme l’application $p$ est ouverte et l’ensemble $E_b$ fini, l’ensemble $U'=\bigcap_{x\in E_b}p(V'_x)$ est un voisinage ouvert de $b$ dans B. Soit U un voisinage ouvert de $b$ dans B, contenu dans $U'$ et tel que pour tout $a\in U$, Card(E$_a)\leqslant$ Card(E$_b)$. Pour tout $x\in E_b$, posons $V_x= V'_x\cap \overset{-1}{p}(U)$. Soit $a$ un point de U ; les ensembles $E_a\cap V_x$, pour $x\in E_b$, sont non vides et deux à deux disjoints. Ces ensembles contiennent donc chacun un unique élément et forment une partition de $E_a$. Cela démontre que, pour tout $x\in E_b$, l’application $p|V_x$ est injective et que l’on a $\overset{-1}{p}(U) =\bigcup_{x\in E_b}V_x$. Comme l’application $p$ est ouverte, elle induit un homéomorphisme de $V_x$ sur U et par suite, $(E, p)$ est un revêtement de B (I, p. 70, cor. 1 de la prop. 1).

#### Remarque {#ta-i-s4-n5-rem-1 .statement tag=01P8}

Une application continue, séparée, ouverte, propre et à fibres finies n’est pas nécessairement un revêtement. C’est le cas de l’application $x\mapsto x^2$ de $\mathbf{R}$ dans $[0; +\infty [$.

#### Corollaire 1 {#ta-i-s4-thm-1-cor-1 .statement tag=01P9}

Soient E et B des espaces topologiques et soit $p: E\rightarrow B$ une application propre et séparée. L’ensemble U des points $b$ de B tels que $p$ soit étale en tout point de la fibre $E_b$ est ouvert dans B. Le U-espace induit par $(E, p)$ au-dessus de U est un revêtement localement fini.

L’ensemble F des points de E en lesquels l’application $p$ n’est pas étale est fermé dans E (I, p. 29, remarque 1). Son image $p(F)$ est fermée car l’application $p$ est propre ; le complémentaire U de $p(F)$ est donc ouvert. L’application $p_U$ est séparée (I, p. 27, prop. 4) et propre (TG, I, p. 72, prop. 3). Par construction, l’application $p_U$ est étale ; elle satisfait donc à la condition (ii) du théorème 1.

#### Corollaire 2 {#ta-i-s4-thm-1-cor-2 .statement tag=01PA}

Soit B un espace topologique séparé et soit E un B-espace. Supposons que E soit compact et que sa projection $p: E\rightarrow B$ soit étale. Alors, E est un revêtement fini de B.

L’application $p$ est séparée (I, p. 26, remarque 2) et propre (TG, I, p. 76, cor. 2). D’après le corollaire 1, E est donc un revêtement localement fini de B. Comme E est compact, $p(E)$ est une partie quasi-compacte de B; l’application de $p(E)$ dans $\mathbf{N}$ donnée par $b\mapsto$ Card $\overset{-1}{p}(b)$ étant localement constante, elle est majorée (TG, IV, p. 30, corollaire).

#### Corollaire 3 {#ta-i-s4-thm-1-cor-3 .statement tag=01PB}

Soit B un espace topologique, soient $(E, p)$ et $(E', p')$ des B-espaces et soit $f: E'\rightarrow E$ un B-morphisme. Supposons que $E'$ soit un revêtement localement fini de B.

a) Si l’application $p$ est étale et séparée, le E-espace $(E', f)$ est un revêtement.

b) Si l’application $f$ est surjective et fait de l’espace $E'$ un revêtement de E, alors E est un revêtement de B.

Sous l’hypothèse de a), les applications $p$ et $p'$ sont étales et séparées, et l’application $p'$ est propre (théorème 1). L’application $f$ est donc étale (I, p. 30, cor. 1 de la prop. 6), séparée (I, p. 25, prop. 2 b)) et propre (I, p. 28, prop. 5). D’après le théorème 1, $(E', f)$ est un revêtement de E.

Supposons maintenant que $f$ soit surjective et que $(E', f)$ soit un revêtement de E. Il est alors localement fini donc l’application $f$ est propre et surjective (th. 1). D’après I, p. 25, prop. 2, c), l’application $p$ est séparée, car $p'=p\circ f$ et $p'$ est séparée. L’application $p$ est étale (I, p. 29, prop. 6, d)), propre (TG, I, p. 73, prop. 5, b)) et ses fibres sont finies. D’après le th. 1, le B-espace $(E, p)$ est alors un revêtement de B.

#### Corollaire 4 {#ta-i-s4-thm-1-cor-4 .statement tag=01PC}

Soit

${E'}^{f'}$ E

$p'p$

${B'}^f$ B un carré cartésien. Supposons que $(E', p')$ soit un revêtement localement fini de $B'$ et que l’application $f$ soit universellement stricte et surjective. Alors $(E, p)$ est un revêtement localement fini de B.

En effet, l’application $p$ est étale (I, p. 31, prop. 8), propre (I, p. 21, prop. 11) et séparée (I, p. 27, prop. 4).

#### Corollaire 5 {#ta-i-s4-thm-1-cor-5 .statement tag=01PD}

Soit B un espace topologique connexe et soit $(E, p)$ un revêtement fini de B. L’espace E n’a qu’un nombre fini de composantes connexes et chacune d’entre elles est un revêtement de B.

Le résultat est vrai si B est vide ; on le suppose désormais non vide.

Si X est une partie ouverte et fermée de E, la restriction de $p$ à X est une application séparée (I, p. 25, prop. 2, a) et I, p. 26, remarque 1), étale et propre (TG, I, p. 74, corollaire 1) ; d’après le théorème 1, $(X, p)$ est un revêtement localement fini de B. Comme B est connexe, ce revêtement possède un degré fini. Si X est distinct de E, il existe un point $b\in B$ tel que $X_b(E_b$, d’où $[X : B]<[E : B]$ car B est connexe. On en déduit que toute suite décroissante d’ensembles ouverts et fermés dans E est stationnaire.

Soit $x\in E$; il existe alors une plus petite partie ouverte et fermée X de E contenant $x$ (E, III, p. 51, prop. 6). Un tel ensemble X est connexe ; c’est donc la composante connexe de $x$ dans E. Cela montre que les composantes connexes de E sont ouvertes et fermées et que chacune d’entre elles est un revêtement de B. Comme B est connexe, chaque composante connexe de E rencontre chaque fibre de $p$; les composantes connexes de E sont donc en nombre fini.

#### Proposition 5 {#ta-i-s4-prop-5 .statement tag=01PE}

Soit B un espace topologique, soient E et $E'$ des B-espaces et soit $f: E'\rightarrow E$ un B-morphisme. On suppose que E est un revêtement localement fini et que l’espace $E'$, muni de l’application $f$, est un E-espace fibré localement trivial ( resp. un revêtement). Alors, $E'$ est un B-espace fibré localement trivial ( resp. un revêtement).

Notons $p$ et $p'$ les projections respectives des B-espaces E et $E'$. Soit $b$ un point de B. Il existe un voisinage ouvert U de $b$ dans B et une partition finie $(V_i)_{i\in I}$ de $\overset{-1}{p}(U)$ formée d’ensembles ouverts de E telle que, pour tout $i\in I$, l’application $p$ induise un homéomorphisme de

$V_i$ sur U. Posons $V'_i=\overset{-1}{f}(V_i)$. Les ensembles $V'_i$ sont ouverts dans $E'$,

forment une partition de $(^-{p'}^1)(U)$ et l’application de $V'_i$ dans U déduite de $p'$ par passage aux sous-espaces fait de $V'_i$ un U-espace fibré localement trivial. Il en résulte que l’espace $(^-{p'}^1)(U)$, muni de l’application

$p'_U:(^-{p'}^1)(U)\rightarrow U$, est un U-espace fibré localement trivial (I, p. 69, remarque 2). Si $(E', f)$ est un revêtement de E, les fibres de $p'_U$ sont discrètes car leurs intersections avec chacun des ensembles ouverts $V'_i$ le sont. Cela termine la démonstration.

#### Remarque {#ta-i-s4-n5-rem-2 .statement tag=01PF}

Si $(E, p)$ est un revêtement de B et si $(E', f)$ est un revêtement de E, l’application $p\circ f$ est étale (I, p. 29, prop. 6, a)) et séparée (I, p. 25, prop. 2, a)). Mais il peut arriver, voir l’exercice 5, b) de I, p. 146, que l’espace $E'$, muni de l’application $p\circ f$, ne soit pas un revêtement de B. Voir cependant IV, p. 342, prop. 3.

### 6. Revêtements des espaces localement connexes

Soit B un espace topologique et soit E un B-espace. Supposons que sa projection $p$ soit une application étale et séparée.

Si l’espace B est localement connexe, l’espace E est localement connexe. Si l’espace E est localement connexe, la partie ouverte $p(E)$ de B (cf. I, p. 29, remarque 2) est localement connexe.

L’image $s(B)$ de toute section $s$ de $p$ est ouverte (I, p. 30, cor. 3) et fermée dans B (I, p. 27, prop. 3). Si B est connexe et non vide, c’est donc une composante connexe de E ; en général, c’est une réunion de composantes connexes de E.

Si B est localement connexe, la réunion des images des sections de $p$ est donc une partie ouverte et fermée de E (cf. TG, I, p. 85).

Supposons que E soit un revêtement trivialisable de B et soit $g: E\rightarrow B\times F$ une trivialisation. Si l’espace B est connexe, les ensembles $V_x=\overset{-1}{g}(B\times  \{x\})$, pour $x$ parcourant F, sont les composantes connexes de E (cf. prop. 1 de I, p. 69).

#### Proposition 6 {#ta-i-s4-prop-6 .statement tag=01PG}

Soit B un espace topologique et soit E un B-espace ; notons $p$ sa projection. Supposons que l’espace E soit localement connexe. Pour que E soit un revêtement de B, il faut et il suffit que tout point de B possède un voisinage ouvert U tel que l’application $p$ induise un homéomorphisme de toute composante connexe de $\overset{-1}{p}(U)$ sur U.

Soit $b$ un point de B. Si E est un revêtement de B, tout voisinage ouvert U de $b$ qui est connexe et au-dessus duquel le revêtement E est trivialisable remplit les conditions énoncées dans la proposition. Inversement, soit U un voisinage ouvert de $b$ remplissant ces conditions. L’ensemble $\overset{-1}{p}(U)$ est ouvert ; ses composantes connexes sont des parties ouvertes de E (TG, I, p. 85, prop. 11) et constituent une partition de $\overset{-1}{p}(U)$. La proposition résulte donc du corollaire 1 (I, p. 70) de la proposition 1.

#### Corollaire 1 {#ta-i-s4-prop-6-cor-1 .statement tag=01PH}

Soit B un espace topologique localement connexe, soit $(E, p)$ un revêtement de B et soit $E'$ une partie ouverte et fermée de E. Le B-espace $(E', p|E')$ est un revêtement et $p(E')$ est ouvert et fermé dans B.

Les espaces E et $E'$ sont localement connexes. Pour toute partie ouverte U de B, l’ensemble $E'\cap \overset{-1}{p}(U)$ est ouvert et fermé dans $\overset{-1}{p}(U)$, donc est réunion de composantes connexes de $\overset{-1}{p}(U)$. Les parties ouvertes U de B telles que $p$ induise un homéomorphisme de chaque composante connexe de $\overset{-1}{p}(U)$ sur U recouvrent B. D’après la proposition, $p|E'$ fait de $E'$ un revêtement de B. La deuxième assertion en résulte (cf. I, p. 68).

#### Corollaire 2 {#ta-i-s4-prop-6-cor-2 .statement tag=01PI}

Soit B un espace topologique localement connexe, soient $(E, p)$, $(E', p')$ des revêtements de B et soient $f, g: E'\rightarrow E$ des B-morphismes. Pour tout point $b$ de B, notons $f_b, g_b: E_b\rightarrow E'_b$ les applications déduites de $f$ et $g$ respectivement. L’ensemble des points $b$ de B tels que $f_b=g_b$ est ouvert et fermé dans B.

Soit X l’ensemble des points $x$ de $E'$ tels que $f(x) =g(x)$. C’est l’ensemble des points où coïncident les relèvements $f$ et $g$ de $p'$ à E ; donc X est ouvert et fermé dans $E'$ (prop. 11 de I, p. 34). Le complémentaire Y de X est aussi ouvert et fermé ; par suite $p(Y)$ est ouvert et fermé dans B (corollaire 1). Son complémentaire, qui est l’ensemble des points $b$ de B tels que $f_b=g_b$, l’est donc aussi.

#### Corollaire 3 {#ta-i-s4-prop-6-cor-3 .statement tag=01PJ}

Soit B un espace topologique connexe et localement connexe, soient $(E, p)$ et $(E', p')$ des revêtements de B. Pour tout point $b$ de B, l’application $f\mapsto f_b$ de $\mathscr{C}_B(E'; E)$ dans $\mathscr{C}(E'_b; E_b)$ est injective.

Soit $b$ un point de B. Soient $f$ et $g$ des B-morphismes de $E'$ dans E tels que $f_b=g_b$. L’ensemble des points $a$ de B tels que $f_a=g_a$ est ouvert et fermé dans B (corollaire 2) et contient $b$. Il est donc égal à B et $f$ est égal à $g$.

#### Corollaire 4 {#ta-i-s4-prop-6-cor-4 .statement tag=01PK}

Soit B un espace topologique connexe et localement connexe, soit $(E, p)$ un revêtement de B et soit $b$ un point de B. Pour que E soit un revêtement trivialisable, il faut et il suffit que tout point de la fibre $E_b$ appartienne à l’image d’une section continue de $p$.

La condition est nécessaire. Soit $E'$ la réunion des images des sections continues de $p$ et soit $E''$ son complémentaire dans E. L’ensemble $E'$ est ouvert et fermé dans E (cf. I, p. 79). Par suite, $(E', p|E')$ est un revêtement de B (corollaire 1), et ce revêtement est trivialisable en vertu du corollaire 2 (I, p. 70). Supposons que $E'$ contienne $E_b$ et démontrons que $E''$ est vide. Comme $E''$ est ouvert et fermé dans E, $p(E'')$ est ouvert et fermé dans B (corollaire 1). Puisque B est connexe et que $b$ n’appartient pas à $p(E''),p(E'') =\emptyset$, donc $E''=\emptyset$.

#### Corollaire 5 {#ta-i-s4-prop-6-cor-5 .statement tag=01PL}

Soit

${E'}^{f'}$ E

$p'p$

${B'}^f$ B

un carré cartésien. Supposons que le B-espace $(E, p)$ soit un revêtement et que l’espace $B'$ soit connexe et localement connexe. Soit $b'$ un point de $B'$. Pour que le $B'$-espace $(E', p')$ soit un revêtement trivialisable, il faut et il suffit que pour tout point $x$ de E tel que $p(x) =f(b')$, il existe un relèvement continu $g: B'\rightarrow E$ de $f$ tel que $g(b') =x$.

Rappelons que $(E', p')$ est un revêtement de $B'($I, p. 71, cor. 2) et que l’application $f'$ induit une bijection $E'_{b'}\rightarrow E_{f(b')}($I, p. 10, cor.). D’après la prop. 3 de I, p. 9, l’application $s\mapsto f'\circ s$ définit une bijection entre l’ensemble des sections continues de $p'$ et l’ensemble des relèvements continus de $f$ à E. Le corollaire résulte donc du corollaire 4.

#### Proposition 7 {#ta-i-s4-prop-7 .statement tag=01PM}

Soit B un espace topologique, soient E et $E'$ des B-espaces et soit $f: E'\rightarrow E$ un B-morphisme. On suppose que $E'$ est un revêtement de B et que l’espace B est localement connexe.

a) Si la projection du B-espace E est une application étale et séparée, $(E', f)$ est un revêtement de E.

b) Si $f$ est surjective, alors E est un revêtement de B.

Notons $p$ et $p'$ les projections des B-espaces E et $E'$ respectivement. Sous l’hypothèse de a$),f$ est étale (I, p. 29, prop. 6, c)). Sous l’hypothèse de b$),p$ est étale (loc. cit., d)). Par suite, sous l’une quelconque de ces deux hypothèses, E est localement connexe ; ses composantes connexes sont en particulier ouvertes et fermées dans E (TG, I, p. 85, prop. 11).

Nous allons d’abord démontrer la proposition 7 sous l’hypothèse supplémentaire que B est connexe, localement connexe, et que $E'$ est le revêtement trivial $(B\times F'$, pr$_1)$.

#### Lemme {#ta-i-s4-n6-lem-1 .statement tag=01PN}

Si U est une composante connexe de $E'$, la restriction de $f$ à U induit un homéomorphisme de U sur une composante connexe de E.

Soit $x\in F'$ tel que $U = B\times  \{x\}($cf. I, p. 79). L’application de B dans E qui à $b\in B$ associe $f(b, x)$ est une section continue de $p$. Son image X est donc connexe et ouverte dans E, car $p$ est étale (I, p. 30, cor. 3). Elle est de plus fermée sous l’hypothèse a), car $p$ est séparée (I, p. 27, prop. 3). Elle est aussi fermée sous l’hypothèse b) d’après le corollaire 1 de I, p. 80, car U est ouvert et fermé dans $E'$. Par suite, X est une composante connexe de E.

Comme $f|U: U\rightarrow X$ est bijective et ouverte, c’est un homéomorphisme sur son image, ce qui démontre le lemme.

Conservons les hypothèses précédant le lemme et démontrons maintenant l’assertion a). Soit V une composante connexe de E. C’est un

ensemble ouvert et fermé dans E et $\overset{-1}{f}(V)$ est réunion de composantes connexes de $E'$ que $f$ applique homéomorphiquement sur V d’après le lemme. Il résulte de la prop. 6 de I, p. 79 que $(E', f)$ est un revêtement.

Démontrons b). Comme $f$ est surjective, il résulte du lemme que toute composante connexe V de E est l’image homéomorphe d’une composante connexe $U = B\times \{x\}$ de $E'$. L’application $p$ induit alors un homéomorphisme de V sur B. D’après la prop. 6, E est un revêtement de B.

Cela démontre donc la proposition, sous l’hypothèse supplémentaire que B est connexe et $E'$ un revêtement trivialisable de B. Démontronsla dans le cas général.

Il existe un recouvrement $(U_i)_{i\in I}$ de B, formé d’ouverts connexes au-dessus desquels le revêtement $E'$ est trivialisable. Soit $i\in I$.

Démontrons a). Si l’application $p$ est étale et séparée, il en est de même de l’application $p_{U_i}: U_i\times_BE\rightarrow U_i$, pour $i\in I$, d’après les prop. 8 de I, p. 31 et 4 de I, p. 27. Il résulte donc du cas particulier traité que,

pour tout $i\in I$, le $U_i$-espace ($(^-{p'}^1)(U_i), f_{U_i}$) est un revêtement. Notons A l’espace somme des $U_i$ et $q: A\rightarrow B$ l’application canonique. Alors, l’espace $A\times_BE'$, muni de l’application $f_A: A\times_BE'\rightarrow A\times_BE$ est un revêtement de $A\times_BE$. L’application $q$ admet une section continue au voisinage de tout point de B et la prop. 3 de I, p. 72, appliquée au carré cartésien

$$
A\times_BE'E'
$$

$$
_{f_A}f
$$

$A\times_BE$ E

implique que $E'$ est un revêtement de E.

Démontrons b). Supposons que $f$ soit surjective. Alors, pour tout élément $i$ de I, l’application $f_{U_i}: U_i\times_BE'\rightarrow U_i\times_BE$ est surjective et l’espace $U_i\times_BE'$, muni de l’application $f_{U_i}$, est un revêtement de $U_i\times_BE$ (I, p. 71, cor. 2 de la prop. 2). Il résulte du cas particulier traité précédemment que le $U_i$-espace $(\overset{-1}{p}(U_i), p_{U_i})$ est un revêtement. Par conséquent, E est un revêtement de B.

Soit B un espace topologique, soient E et $E'$ des revêtements de B et soit $f: E\rightarrow E'$ un B-morphisme On a vu que $(E, f)$ est un revêtement sous chacune des deux hypothèses suivantes : 1) le revêtement E est localement de degré fini (I, p. 76, cor. 1) ; 2) l’espace B est localement connexe (I, p. 81, prop. 7). Ce phénomène peut s’expliquer comme suit.

Soient F et $F'$ des espaces topologiques discrets et soit $f: B\times F\rightarrow$ $B\times F'$ un B-morphisme. L’application $\widetilde{f}:a\mapsto$ pr$_2\circ f(b,\cdot )$ de B dans l’espace $\mathscr{C}_c(F; F')$ est continue (TG, X, p. 28, th. 3). Si U est un ouvert de B tel que l’application $\widetilde{f}$ soit constante sur U, l’application $f_U: U\times$ $F\rightarrow U\times F'$ déduite de $f$ est un revêtement trivialisable (I, p. 69, prop. 1).

L’espace $\mathscr{C}_c(F; F')$ n’est autre que l’ensemble $\mathscr{F}(F; F')$ des applications de F dans $F'$ muni de la topologie déduite de la topologie de l’espace produit $(F')^F$ par l’identification canonique. Pour cette topologie, l’espace $\mathscr{F}(F; F')$ est totalement discontinu (I, p. 84, prop. 10). Par suite, si l’espace B est connexe, l’application $\widetilde{f}$ est constante (I, p. 82, prop. 4) ; si l’espace B est localement connexe, l’application $\widetilde{f}$ est localement constante. Lorsque l’ensemble F est fini, l’espace $\mathscr{F}(F; F')$ est discret et l’application $\widetilde{f}$ est localement constante.

#### Remarque {#ta-i-s4-n6-rem-1 .statement tag=01PO}

Soit B un espace topologique, soient $(E, p)$ et $(E', p')$ des B-espaces et soit $f: E'\rightarrow E$ un B-morphisme.

a) Si E et $E'$ sont des revêtements de B, l’application $f$ est étale (I, p. 29, prop. 6) et séparée (I, p. 25, prop. 2). Mais il n’est pas vrai, en général, que $(E', f)$ soit un revêtement de E si l’espace B n’est pas localement connexe (I, p. 145, exerc. 4).

b) Si $(E', p')$ est un revêtement de B$,f$ est surjective et fait de $E'$ un revêtement de E, alors l’application $p$ est étale (I, p. 29, prop. 6). Mais il n’est pas vrai, en général, qu’elle soit séparée si l’espace B n’est pas localement connexe (I, p. 145, exerc. 4). En particulier, E n’est pas nécessairement un revêtement de B.

#### Corollaire {#ta-i-s4-n6-cor-1 .statement tag=01PP}

Soit B un espace topologique connexe et localement connexe. Soient E et $E'$ des revêtements de B. Soit $b$ un point de B. Soit $f: E'\rightarrow E$ un B-morphisme et soit $f_b: E'_b\rightarrow E_b$ l’application déduite de $f$ par restriction aux fibres. Si l’application $f_b$ est injective ( resp. surjective, resp. bijective), il en est de même de l’application $f$.

Notons $p$ la projection du B-espace E. D’après la proposition, $(E', f)$ est un revêtement de E ; son image $f(E')$ est ouverte et fermée dans E. Notons U le complémentaire de $f(E')$ dans E, de sorte que le B-espace $(U, p|U)$ est un revêtement de B (I, p. 80, corollaire 1). Si l’application $f_b$ est surjective, la fibre en $b$ de ce revêtement est vide. Comme B est un espace connexe, U est alors vide, donc $f$ est surjective.

L’ensemble V des points de E où la fibre de $f$ a exactement un élément est ouvert et fermé. Les B-espaces $(V, p|V)$ et $(f(E'), p|f(E'))$ sont des revêtements de B (loc. cit.) et l’application canonique $i: V\rightarrow$ $f(E')$ est un B-morphisme. Si l’application $f_b$ est injective, l’application $i_b$ est surjective, donc $i$ est surjective d’après ce qui précède et l’on a $V =f(E')$. Par suite, l’application $f$ est injective.

### 7. Revêtements d’un espace paracompact

#### Proposition 8 {#ta-i-s4-prop-8 .statement tag=01PQ}

Un revêtement d’un espace paracompact ( I, p. 69) est un espace paracompact.

Démontrons d’abord un lemme.

#### Lemme {#ta-i-s4-n7-lem-1 .statement tag=01PR}

Soit E un espace topologique séparé. Supposons que E possède un recouvrement ouvert localement fini $(V_i)_{i\in I}$ tel que, pour tout $i\in I,\overline{V_i}$ soit un espace paracompact. Alors, l’espace E est paracompact.

Soit $(W_j)_{j\in J}$ un recouvrement ouvert de E ; nous allons démontrer qu’il existe un recouvrement ouvert localement fini $(A_k)_{k\in K}$ de E qui est plus fin que le recouvrement $(W_j)_{j\in J}$. Pour tout $i\in I$, soit $(A'_{\ell})_{\ell\in K_i}$ un recouvrement localement fini de $\overline{V_i}$ par des ouverts de $\overline{V_i}$, plus fin que le recouvrement $(W_j\cap \overline{V_i})_{j\in J}$. Soit K la somme de la famille $(K_i)_{i\in I}$ (E, II, p. 30, déf. 8). Pour tout élément $k= (\ell , i)$ de K, posons $A_k= A'_{\ell}\cap V_i$. Alors $A_k$ est ouvert dans E et l’on a $\bigcup_{k\in K}A_k=\bigcup_{i\in I}V_i= E$ ; de plus, pour tout $k\in K$, il existe un indice $j\in J$ tel que $A_k\subset W_j$. Ainsi, la famille $(A_k)_{k\in K}$ est un recouvrement ouvert de E plus fin que $(W_j)_{j\in J}$. Il reste à démontrer que la famille $(A_k)_{k\in K}$ est localement finie. Soit $x\in E$ ; il existe un voisinage ouvert U de $x$ qui ne rencontre $V_i$ que pour $i$ appartenant à un sous-ensemble fini $I'$ de I. Pour tout $i\in I',x$ possède un voisinage ouvert $U_i\subset U$ qui ne rencontre qu’un nombre fini d’ouverts $A_k$, pour $k\in K_i\times \{i\}:$ c’est évident si $x$ n’appartient pas à $\overline{V_i}$, et si $x$ appartient à $\overline{V_i}$, cela résulte de la propriété de finitude locale du recouvrement $(A'_{\ell})_{\ell\in K_i}$ de $\overline{V_i}$. Par suite, $V'=\bigcap_{i\in I'}U_i$ est un voisinage ouvert de $x$ qui ne rencontre qu’un nombre fini des $A_k,k\in K$, et le recouvrement $(A_k)_{k\in K}$ est localement fini.

Démontrons la proposition. Soit E un revêtement de B, notons $p$ sa projection, et supposons que l’espace B soit paracompact. Soit $(A_i)_{i\in I}$ un recouvrement ouvert localement fini de B tel que, pour tout $i\in I$, le revêtement E soit trivialisable au-dessus de $A_i$. Pour tout $i\in I$, soit $F_i$ un espace topologique discret et soit $g_i:\overset{-1}{p}(A_i)\rightarrow A_i\times F_i$ une trivialisation de E au-dessus de $A_i$. Soit $(B_i)_{i\in I}$ un recouvrement ouvert de B tel que, pour tout $i\in I$, on ait $\overline{B_i}\subset A_i$ (TG, IX, p. 49, prop. 4 et p. 48, cor. 1). Pour tout $i\in I$, posons $V_i=\overset{-1}{p}(B_i)$ ; on a $\overline{V_i}\subset \overset{-1}{p}(B_i)\subset \overset{-1}{p}(A_i)$ et $V_i=\overset{-1}{g_{i}}(B_i\times F_i)$, d’où $\overline{V_i}\subset \overset{-1}{g_{i}}(B_i\times F_i)$. Comme B est paracompact, $\overline{B_i}$ est paracompact (TG, I, p. 69, prop. 16) et $\overline{B_i}\times F_i$ est paracompact (TG, I, p. 70, prop. 18). Par suite, $\overset{-1}{g_{i}}(B_i\times F_i)$ est paracompact, donc $\overline{V_i}$ aussi (TG, I, p. 69, prop. 16). La famille $(V_i)_{i\in I}$ est, par construction, un recouvrement ouvert localement fini de E. Enfin, l’espace E est séparé (I, p. 26, remarque 3). Il satisfait donc aux hypothèses du lemme, d’où la proposition.

#### Remarque {#ta-i-s4-n7-rem-1 .statement tag=01PS}

On peut démontrer qu’un revêtement d’un espace métrisable est métrisable (I, p. 145, exerc. 1) et qu’un revêtement connexe d’un espace localement compact dénombrable à l’infini est lui-même localement compact dénombrable à l’infini (I, p. 145, exerc. 2).

### 8. Faisceaux localement constants

Soient B un espace topologique et F un ensemble ; munissons F de la topologie discrète. On appelle faisceau constant sur B de tige-type F le faisceau sur B des applications localement constantes à valeurs dans F (I, p. 45, exemple 2). Ce faisceau est parfois noté F, lorsqu’aucune confusion sur l’espace B n’est à craindre. Il s’identifie au faisceau sur B des sections continues du B-espace étalé $(B\times F$, pr$_1)$ : la formule $i([U, s, a]) = (a, s(a))$ définit en effet un isomorphisme canonique $i$ de l’espace étalé associé à F sur $(B\times F$, pr$_1)$. Pour tout $a\in B$, l’application $[U, s, a]\mapsto s(a)$ est une bijection canonique de la tige $F_a$ de F en $a$ sur l’ensemble F.

Soit $\mathscr{P}= (\mathscr{P}(U), r_{UV})$ le préfaisceau sur B tel que $\mathscr{P}(U) = F$ pour tout ouvert U de B et $r_{UV}=$ Id$_F$ pour tout couple $(U,V)$ d’ouverts de B tels que $U\subset V$. Alors, le faisceau $\widetilde{\mathscr{P}}$ associé à $\mathscr{P}$ est canoniquement isomorphe au faisceau constant F (I, p. 52, exemple 1).

#### Définition 3 {#ta-i-s4-def-3 .statement tag=01PT}

On dit qu’un faisceau $\mathscr{F}$ sur un espace topologique B est localement constant si tout point de B possède un voisinage ouvert U tel que le faisceau induit $\mathscr{F}|U$ soit isomorphe à un faisceau constant sur U.

#### Proposition 9 {#ta-i-s4-prop-9 .statement tag=01PU}

Pour qu’un faisceau soit localement constant, il faut et il suffit que l’espace étalé associé soit un revêtement.

Soit B un espace topologique et soit $\mathscr{F}$ un faisceau sur B. Le faisceau $\mathscr{F}$ est constant si et seulement si l’espace étalé $E_{\mathscr{F}}$ est B-isomorphe à un revêtement trivial $(B\times F$, pr$_1)$, où F est un espace topologique discret. Si U est un ouvert de B, l’espace étalé associé au faisceau induit $\mathscr{F}|U$ s’identifie au U-espace étalé induit par $E_{\mathscr{F}}$ au-dessus de U (cf. I, p. 51). La proposition en résulte.

#### Corollaire {#ta-i-s4-n8-cor-1 .statement tag=01PV}

Pour qu’un B-espace étalé soit un revêtement, il faut et il suffit que le faisceau de ses sections soit localement constant.

Cela découle de la proposition et de l’exemple 2 de I, p. 52.

### 9. Produits de faisceaux localement constants

Soit B un espace topologique et soit $(\mathscr{F}_i)_{i\in I}$ une famille de faisceaux sur B. Notons $\mathscr{F}$ le faisceau produit $\prod_{i\in I}\mathscr{F}_i$ et, pour $i\in I$, soit pr$_i:\mathscr{F}\rightarrow \mathscr{F}_i$ le morphisme de projection d’indice $i($I, p. 46, exemple 7). Soient $(E, p)$ et $(E_i, p_i)$ les B-espaces étalés associés aux faisceaux $\mathscr{F}$ et $\mathscr{F}_i$ respectivement, et $\varphi_i: E\rightarrow E_i$ le B-morphisme associé à pr$_i($I, p. 50). Notons enfin $(E', p')$ le B-produit $\prod_BE_i$. D’après la propriété universelle du B-espace produit (I, p. 5), il existe un unique B-morphisme $\Phi : E\rightarrow E'$ tel que, pour tout $i\in I$, pr$_i\circ \Phi  =\varphi_i$.

#### Proposition 10 {#ta-i-s4-prop-10 .statement tag=01PW}

Si l’ensemble I est fini, le B-morphisme Φ est un isomorphisme.

D’après le corollaire de I, p. 32, le B-espace $E'$ est étalé et il suffit de démontrer que le B-morphisme Φ est bijectif ( I, p. 30, cor. 2). Pour tout point $b$ de B, la restriction $\Phi_b: E_b\rightarrow E'_b$ de Φ aux fibres en $b$ s’identifie à l’application canonique de lim$\longrightarrow \prod_{i\in I}\mathscr{F}_i(U)$ dans $\prod_{i\in I}$ lim$\longrightarrow \mathscr{F}_i(U)$, où U parcourt l’ensemble des ouverts de B qui contiennent $b($cf. I, p. 50). D’après la prop. 10 de E, III, p. 67, cette application est une bijection.

Considérons maintenant le cas des faisceaux localement constants sur un espace topologique B. Soit $(F_i)_{i\in I}$ une famille d’ensembles et posons $F =\prod_{i\in I}F_i$. On définit un morphisme canonique $\psi = (\psi_U)$ du faisceau constant F dans le produit $\prod_{i\in I}F_i$ des faisceaux constants $F_i$ en posant, pour tout ouvert U de B et toute fonction localement constante $f: U\rightarrow F,\psi_U(f) =$ (pr$_i\circ f)_{i\in I}$.

#### Proposition 11 {#ta-i-s4-prop-11 .statement tag=01PX}

Si l’ensemble I est fini, ou si l’espace B est localement connexe, le morphisme canonique $\psi : F\rightarrow \prod F_i$ est un isomorphisme.

Soit U un ouvert de B. Il est clair que l’application $\psi_U$ est injective. Montrons qu’elle est surjective. Il s’agit de prouver que pour toute famille $(f_i)_{i\in I}$ où $f_i$ est une application localement constante de U dans $F_i$, et tout point $a$ de U, il existe un voisinage V de $a$ dans U tel que pour tout $i\in I$, l’application $f_i|V$ soit constante. Lorsque l’ensemble I est fini, l’existence d’un tel voisinage est claire. Lorsque l’espace B est localement connexe, il suffit de prendre pour V un voisinage connexe de $a$ dans U. Cela prouve la proposition.

#### Corollaire 1 {#ta-i-s4-prop-11-cor-1 .statement tag=01PY}

Un produit fini de faisceaux localement constants est localement constant.

Soit $(\mathscr{F}_i)_{i\in I}$ une famille finie de faisceaux localement constants sur B. Tout point $a$ de B possède un voisinage ouvert U dans B tel que, pour tout $i\in I$, le faisceau $\mathscr{F}_i|U$ soit isomorphe à un faisceau constant. Il en est alors de même du faisceau $((\prod\mathscr{F}_i)|U$, qui est égal à $\prod ((\mathscr{F}_i|U)$.

#### Corollaire 2 {#ta-i-s4-prop-11-cor-2 .statement tag=01PZ}

Soit $(\mathscr{F}_i)_{i\in I}$ une famille de faisceaux sur B. Supposons que l’espace B soit localement connexe et que tout point de B possède un voisinage ouvert U tel que, pour tout $i\in I$, le faisceau $\mathscr{F}_i|U$ soit isomorphe à un faisceau constant. Alors, le faisceau produit $\prod\mathscr{F}_i$ est localement constant.

#### Remarque 1 {#ta-i-s4-n9-rem-1 .statement tag=01Q0}

Soit $(E_i, p_i)_{i\in I}$ une famille de revêtements de l’espace topologique B. Supposons que l’espace B soit localement connexe et qu’il existe un recouvrement ouvert $(U_j)_{j\in J}$ de B tel que, pour tout $j\in J$ et tout $i\in I$, le revêtement $E_i$ soit trivialisable au-dessus de $U_j$. Pour $i\in I$, soit $\mathscr{F}_i$ le faisceau localement constant des sections de $E_i$ et soit $\mathscr{F}$ le faisceau produit $\prod_i\mathscr{F}_i$. D’après le corollaire précédent, $\mathscr{F}$ est un faisceau localement constant et le B-espace étalé E qui lui est associé est donc un revêtement (I, p. 86, prop. 8). Pour $i\in I$, soit pr$_i: E\rightarrow E_i$ le B-morphisme induit par le morphisme de projection d’indice $i,\mathscr{F}\rightarrow \mathscr{F}_i$.

Considérons maintenant un revêtement $(Y, q)$ de B et, pour tout $i\in$ I, soit $f_i: Y\rightarrow E_i$ un B-morphisme. Si $\mathscr{G}$ désigne le faisceau localement constant des sections de $q$, les B-morphismes $f_i$ induisent des morphismes de faisceaux $\widetilde{f}_i:\mathscr{G}\rightarrow \mathscr{F}_i$. Soit $\widetilde{f}:\mathscr{G}\rightarrow \mathscr{F}$ l’unique morphisme de faisceaux tel que $\widetilde{f}_i=$ pr$_i\circ \widetilde{f}$ pour tout $i\in I$. Il existe alors un unique B-morphisme $f: Y\rightarrow E$ tel que $f_i$ = pr$_i\circ f$ pour tout $i:$ c’est le B-morphisme qui induit $\widetilde{f}$.

On dit parfois que E est le revêtement produit de la famille $(E_i)_{i\in I}$.

#### Remarque 2 {#ta-i-s4-n9-rem-2 .statement tag=01Q1}

Avec les notations précédentes, le B-morphisme canonique $\Phi : E\rightarrow \prod_BE_i$ est bijectif. La question est en effet de nature locale sur B et l’on peut supposer que, pour tout $i\in I$, le B-espace $E_i$ est isomorphe au B-espace $(B\times F_i$, pr$_1)$, où $F_i$ est un espace topologique discret, de sorte que le faisceau $\mathscr{F}_i$ est isomorphe au faisceau $F_i$. D’après la prop. 11, le faisceau $\mathscr{F}$ s’identifie au faisceau F, où F est l’ensemble $\prod F_i$, muni de la topologie discrète, et l’application Φ s’identifie à l’application canonique $B\times F\rightarrow B\times (\prod_iF_i)$ qui est bijective.

### 10. Morphismes de faisceaux localement constants sur un espace localement connexe

Soit B un espace topologique, soient $(E, p)$ et $(E', p')$ des B-espaces. Notons $\mathscr{M}$ = $\mathscr{M}$or$_B(E; E')$ le faisceau sur B des B-morphismes de $(E, p)$ dans $(E', p')$ (I, p. 45, exemple 4). Si U est un ouvert de B et $b$ un point de U, on notera $\theta_{b,U}:\mathscr{M}(U)\rightarrow \mathscr{C}(E_b; E'_b)$ l’application canonique obtenue par passage aux fibres en $b$. On note $\theta_b:\mathscr{M}_b\rightarrow$ $\mathscr{C}(E_b; E'_b)$ l’unique application telle que $\theta_{b,U}$ soit la composée de $\theta_b$ et de l’application canonique $\mathscr{M}(U)\rightarrow \mathscr{M}_b$ pour tout ouvert U de B contenant $b$ (E, III, p. 62).

Soit aussi $\mathscr{I}=\mathscr{I}$som$_B(E; E')$ le faisceau sur B des B-isomorphismes de $(E, p)$ dans $(E', p')$. Notons $i:\mathscr{I}\rightarrow \mathscr{M}$ le morphisme canonique. Pour tout $b\in B$, l’application $\theta_b\circ i_b$ induit une application $\theta '_b$ de $\mathscr{I}_b$ dans l’ensemble des bijections continues de $E_b$ sur $E'_b$.

#### Proposition 12 {#ta-i-s4-prop-12 .statement tag=01Q2}

Supposons que l’espace B soit localement connexe et que les B-espaces E et $E'$ soient des revêtements. Le faisceau $\mathscr{M}$or$_B(E; E')$ est alors localement constant et, pour tout $b\in B$, l’application $\theta_b$ est une bijection de sa tige en $b$ sur l’ensemble des applications de $E_b$ dans $E'_b$.

De même, le faisceau $\mathscr{I}$som$_B(E; E')$ est localement constant et, pour tout point $b$ de B, l’application $\theta '_b$ est une bijection de sa tige en $b$ sur l’ensemble des bijections de $E_b$ sur $E'_b$.

Nous noterons $\mathscr{M}=\mathscr{M}$or$_B(E; E')$ et $\mathscr{I}=\mathscr{I}$som$_B(E; E')$. Les assertions à démontrer sont de nature locale sur B ; nous pouvons donc supposer que $E = B\times F$ et $E'= B\times F'$ sont des revêtements triviaux, où F et $F'$ sont des espaces topologiques discrets.

Prouvons d’abord que, pour tout ouvert connexe U de B et tout point $b$ de U, l’application $\theta_{b,U}$ est une bijection. Soit $f: U\times F\rightarrow$ $U\times F'$ un morphisme de U-espaces ; alors, $\theta_{b,U}(f)$ est l’application $y\mapsto$ pr$_2(f(b, y))$ de F dans $F'$. Pour tout $y\in F$, l’application $x\mapsto$ pr$_2(f(x, y))$ est une application continue de l’espace connexe U dans l’espace discret $F'$, donc est constante, égale à pr$_2(f(b, y))$. On a ainsi $f(x, y) = (x, \theta_{b,U}(f)(y))$. Il en résulte que $\theta_{b,U}$ est une bijection ; sa bijection réciproque associe à toute application $\varphi : F\rightarrow F'$ le U-morphisme de $U\times F$ dans $U\times F'$ donné par $(x, y)\mapsto (x, \varphi (y))$.

Par hypothèse, tout point $b\in B$ admet une base de voisinages ouverts connexes ; l’application $\theta_b$ est donc une bijection. Les applications $\theta^{-1}_{b,U}$, pour U ouvert connexe non vide de B et $b$ un point quelconque de $b$, définissent un morphisme de préfaisceaux (relativement à la base des ouverts connexes de B) du faisceau constant de tige-type ${F'}^F$ dans le faisceau $\mathscr{M}$. D’après ce qui précède, ce morphisme induit une bijection sur les tiges ; c’est donc un isomorphisme.

Les assertions relatives au faisceau $\mathscr{I}$ se démontrent de même.

#### Corollaire 1 {#ta-i-s4-prop-12-cor-1 .statement tag=01Q3}

Soient B un espace topologique et A un sous-espace de B. On suppose que les espaces A et B sont localement connexes. Soient E et $E'$ des revêtements de B. Alors les morphismes canoniques $\psi :\mathscr{M}$or$_B(E; E')_A\rightarrow \mathscr{M}$or$_A(E_A; E'_A)$ et $\psi ':\mathscr{I}$som$_B(E; E')_A\rightarrow$ $\mathscr{I}$som$_A(E_A; E'_A)$ (I, p. 45, exemple 4) sont des isomorphismes.

Pour tout point $a\in A$, il résulte de la proposition précédente et de l’exemple 2 de I, p. 63, appliqué aux espaces $\{a\}$, A, B et aux injections canoniques, que le morphisme canonique $\psi$ induit par passage aux tiges l’identité de $E^{E'_a}_a$. C’est donc un isomorphisme. Le fait que $\psi '$ soit un isomorphisme se démontre de manière analogue.

#### Corollaire 2 {#ta-i-s4-prop-12-cor-2 .statement tag=01Q4}

Soient B un espace topologique et A un sous-espace de B. On suppose que les espaces A et B sont localement connexes et que le couple $(B,A)$ jouit de la propriété (PCV) de I, p. 37. Soient E et $E'$ des revêtements de B, notons $p$ et $p'$ leurs projections. Soit

$g:\overset{-1}{p}(A)\rightarrow (^-{p'}^1)(A)$ un A-morphisme ( resp. un A-isomorphisme). Il existe un voisinage U de A dans B et un U-morphisme ( resp. un

U-isomorphisme) $f:\overset{-1}{p}(U)\rightarrow (\overset{-1}{p}')(U)$ tel que $f_A=g$.

Conservons les notations du corollaire 1. D’après ce même corollaire, un A-morphisme $g: E_A\rightarrow E'_A$ s’identifie à une section $s_0$ au-dessus de A de l’espace étalé $E_{\mathscr{M}}$ associé à $\mathscr{M}$. D’après l’hypothèse faite sur le couple $(B,A)$ et le lemme 3 de I, p. 39, il existe un voisinage ouvert U de A dans B et une section continue $s$ de $E_{\mathscr{M}}$ au-dessus de U prolongeant $s_0$. Cette section $s$ s’identifie à un U-morphisme $f: E_U\rightarrow E'_U$ prolongeant $f$.

Le cas où $g$ est un A-isomorphisme se traite de manière analogue en considérant au lieu du faisceau $\mathscr{M}$ le faisceau $\mathscr{I}$.

## EXERCICES {#ta-i-s4-exercises}

See the [exercises for § 4](exercises/s4/).
