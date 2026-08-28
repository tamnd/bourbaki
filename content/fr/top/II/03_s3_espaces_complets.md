---
book: top
book_title: General Topology
chapter: II
chapter_title: STRUCTURES UNIFORMES
section: 3
section_title: Espaces complets
lang: fr
source: top-i-iv-fr
book_pages: TG II.12-TG II.26, TG II.35-TG II.36
pdf_pages: 0151-0165, 0174-0175
extraction: ocr
subsections:
    - "no": 1
      title: Filtres de Cauchy
      page: 12
      pdf_page: 151
    - "no": 2
      title: Filtres de Cauchy minimaux
      page: 14
      pdf_page: 153
    - "no": 3
      title: Espaces complets
      page: 15
      pdf_page: 154
    - "no": 4
      title: Sous-espaces des espaces complets
      page: 16
      pdf_page: 155
    - "no": 5
      title: Produits et limites projectives d’espaces complets
      page: 17
      pdf_page: 156
    - "no": 6
      title: Prolongement des fonctions uniformément continues
      page: 20
      pdf_page: 159
    - "no": 7
      title: La complétion d’un espace uniforme
      page: 21
      pdf_page: 160
    - "no": 8
      title: Espace uniforme séparé associé à un espace uniforme
      page: 24
      pdf_page: 163
    - "no": 9
      title: Complétion des sous-espaces et des espaces produits
      page: 26
      pdf_page: 165
statements: 47
exercises: 7
content_sha256: 7b3962f40687de1412eac7b21507079e0cc5f58948a2fab1fecfc3ae3fc562cc
---

## § 3. ESPACES COMPLETS

### 1. Filtres de Cauchy

Lorsqu’on a muni un ensemble $X$ d’une structure uniforme, on peut définir ce qu’on entend par un sous-ensemble « petit » dans $X$ (relativement à cette structure): ce sera un ensemble dont tous les points sont « très voisins » deux à deux. De façon précise:

#### Définition 1 {#top-ii-s3-def-1 .statement}

Étant donné un espace uniforme $X$, et un entourage $V$ de $X$, on dit qu’une partie $A$ de $X$ est un ensemble petit d’ordre $V$ lorsque deux quelconques des points de $A$ sont voisins d’ordre $V$ (ce qui revient à dire que $A \times A \subset V$).

#### Proposition 1 {#top-ii-s3-prop-1 .statement}

Dans un espace uniforme $X$, si deux ensembles $A$ et $B$ sont petits d’ordre $V$ et se rencontrent, leur réunion $A \cup B$ est un ensemble petit d’ordre $\overline{V}^2$.

En effet, soient $x, y$ deux points de $A \cup B$, et $z$ un point de $A \cap B$; on a par hypothèse $(x, z) \in V$ et $(z, y) \in V$, donc $(x, y) \in \overline{V}^2$.

#### Définition 2 {#top-ii-s3-def-2 .statement}

*On dit qu’un filtre $\mathcal{F}$ sur un espace uniforme $X$ est un filtre de Cauchy si, pour tout entourage $V$ de $X$, il existe un ensemble petit d’ordre $V$ et appartenant à $\mathcal{F}$.*

Ici encore, on peut rendre le langage plus imagé en utilisant les expressions « ensemble assez petit » et « ensemble aussi petit qu’on veut »; par exemple, la déf. 2 peut encore s’exprimer en disant qu’un filtre de Cauchy est un filtre qui *contient des ensembles arbitrairement petits*.

On dit qu’une suite infinie $(u_n)$ de points d’un espace uniforme $X$ est une *suite de Cauchy* si le filtre élémentaire associé à cette suite est un filtre de Cauchy. Il revient au même de dire que pour tout entourage $V$ de $X$, il existe $n_0$ tel que, quels que soient $m \geq n_0$ et $n \geq n_0$, on ait $(u_m, u_n) \in V$.

#### Proposition 2 {#top-ii-s3-prop-2 .statement}

*Sur un espace uniforme $X$, tout filtre convergent est un filtre de Cauchy.*

En effet, pour tout $x \in X$, et tout entourage symétrique $V$ de $X$, le voisinage $V(x)$ de $x$ est petit d’ordre $\overline{V}^2$; si $\mathcal{F}$ est un filtre convergent vers $x$, il existe un ensemble de $\mathcal{F}$ contenu dans $V(x)$, donc petit d’ordre $\overline{V}^2$.

Il est clair que tout filtre *plus fin* qu’un filtre de Cauchy est un filtre de Cauchy.

#### Proposition 3 {#top-ii-s3-prop-3 .statement}

*Soit $f : X \to X'$ une application uniformément continue. L’image par $f$ d’une base de filtre de Cauchy sur $X$ est une base de filtre de Cauchy sur $X'$.*

Soit en effet $g = f \times f$; si $V'$ est un entourage de $X'$, $\overline{g^{-1}(V')}$ est un entourage de $X$, et l’image par $f$ d’un ensemble petit d’ordre $\overline{g^{-1}(V')}$ est un ensemble petit d’ordre $V'$; d’où la proposition.

Il en résulte en particulier que si on remplace la structure uniforme d’un espace uniforme $X$ par une structure uniforme *moins fine*, tout filtre de Cauchy pour la structure uniforme initialement donnée reste filtre de Cauchy pour la nouvelle structure uniforme.

On retiendra aisément ce fait sous la forme suivante: *plus une structure uniforme est fine, moins il y a de filtres de Cauchy*.

#### Proposition 4 {#top-ii-s3-prop-4 .statement}

*Soient $X$ un ensemble, $(Y_\iota)_{\iota \in I}$ une famille d’espaces uniformes, et pour chaque $\iota \in I$, soit $f_\iota$ une application de $X$ dans $Y_\iota$. On munit $X$ de la structure uniforme $\mathcal{U}$ la moins fine rendant uniformément continues les $f_\iota$. Pour qu’une base de filtre $\mathcal{B}$ sur $X$ soit une base de filtre de Cauchy, il faut et il suffit que, pour tout $\iota \in I$, $f_\iota(\mathcal{B})$ soit une base de filtre de Cauchy sur $Y_\iota$.*

La condition est nécessaire en vertu de la prop. 3. Inversement, supposons-la vérifiée, et soit $U(V_{\iota_1}, \ldots, V_{\iota_n})$ un entourage de la structure uniforme $\mathcal{U}$ (II, p. 8, formule (1)). Par hypothèse, pour tout indice $k$, il existe un ensemble $M_k \in \mathfrak{B}$ tel que $f_{\iota_k}(M_k)$ soit petit d’ordre $V_{\iota_k}$ ($1 \leq k \leq n$); soit $M$ un ensemble de $\mathfrak{B}$ contenu dans $M_{k}$ pour $1 \leq k \leq n$; pour tout couple de points, $x, x'$ de $M$, on a $(f_{t_{k}}(x), f_{t_{k}}(x')) \in V_{t_{k}}$ pour $1 \leq k \leq n$, donc $(x, x') \in U(V_{t_{1}}, \ldots, V_{t_{n}})$ ce qui démontre la proposition.

#### Corollaire 1 {#top-ii-s3-prop-4-cor-1 .statement}

Si un filtre de Cauchy sur un espace uniforme $X$ induit un filtre sur une partie $A$ de $X$, ce filtre est un filtre de Cauchy sur le sous-espace uniforme $A$.

#### Corollaire 2 {#top-ii-s3-prop-4-cor-2 .statement}

Pour qu’une base de filtre $\mathcal{B}$ sur un produit $\prod_{i \in I} X_{i}$ d’espaces uniformes soit une base de filtre de Cauchy, il faut et il suffit que, pour tout $i \in I$, $\mathrm{pr}_{i}(\mathcal{B})$ soit une base de filtre de Cauchy sur $X_{i}$.

### 2. Filtres de Cauchy minimaux

Les éléments minimaux (pour la relation d’inclusion) de l’ensemble des filtres de Cauchy sur un espace uniforme $X$ sont appelés *filtres de Cauchy minimaux* sur $X$.

#### Proposition 5 {#top-ii-s3-prop-5 .statement}

Soit $X$ un espace uniforme. Pour tout filtre de Cauchy $\mathcal{F}$ sur $X$, il existe un et un seul filtre de Cauchy minimal $\mathcal{F}_{0}$ moins fin que $\mathcal{F}$; si $\mathcal{B}$ est une base de $\mathcal{F}$, $\mathcal{G}$ un système fondamental d’entourages symétriques de $X$, les ensembles $V(M)$ ($M \in \mathcal{B}, V \in \mathcal{G}$) forment une base de $\mathcal{F}_{0}$.

Si $M, M'$ sont dans $\mathcal{B}$, $V, V'$ dans $\mathcal{G}$, il existe dans $\mathcal{B}$ (resp. $\mathcal{G}$) un ensemble $M''$ (resp. $V''$) tel que $M'' \subset M \cap M'$ (resp. $V'' \subset V \cap V'$), d’où
$$
V''(M'') \subset V(M) \cap V'(M');
$$
les ensembles $V(M)$ (pour $M \in \mathcal{B}, V \in \mathcal{G}$) forment donc bien une base d’un filtre $\mathcal{F}_{0}$ sur $X$. En outre, si $M$ est petit d’ordre $V$, $V(M)$ est petit d’ordre $V^{3}$, donc $\mathcal{F}_{0}$ est un filtre de Cauchy sur $X$, évidemment moins fin que $\mathcal{F}$. Pour achever la démonstration, il suffit de prouver que si $\mathcal{G}$ est un filtre de Cauchy moins fin que $\mathcal{F}$, $\mathcal{G}$ est plus fin que $\mathcal{F}_{0}$; en effet, pour tout $M \in \mathcal{B}$ et tout $V \in \mathcal{G}$, il existe un ensemble $N \in \mathcal{G}$ petit d’ordre $V$, et comme $N \in \mathcal{F}$, $N$ rencontre $M$, donc $N \subset V(M)$ et $V(M) \in \mathcal{G}$.

#### Corollaire 1 {#top-ii-s3-prop-5-cor-1 .statement}

Pour tout $x \in X$, le filtre $\mathcal{B}(x)$ des voisinages de $x$ dans $X$ est un filtre de Cauchy minimal.

Il suffit, dans la prop. 5, de prendre pour $\mathcal{F}$ le filtre de toutes les parties contenant $x$, et pour $\mathcal{B}$ l’ensemble de parties réduit à l’unique élément $\{x\}$.

#### Corollaire 2 {#top-ii-s3-prop-5-cor-2 .statement}

Tout point $x$ adhérent à un filtre de Cauchy $\mathcal{F}$ est point limite de $\mathcal{F}$.

En effet, il existe un filtre $\mathcal{G}$ plus fin que $\mathcal{F}$ et que $\mathcal{B}(x)$ (I, p. 47, prop. 4); comme $\mathcal{F}$ est un filtre de Cauchy, il en est de même de $\mathcal{G}$. Si $\mathcal{F}_{0}$ est l’unique filtre de Cauchy minimal moins fin que $\mathcal{F}$, $\mathcal{F}_{0}$ et $\mathcal{B}(x)$ sont deux filtres de Cauchy minimaux moins fins que $\mathcal{G}$, donc $\mathcal{F}_{0} = \mathcal{B}(x)$, ce qui prouve que $\mathcal{F}$ converge vers $x$.

#### Corollaire 3 {#top-ii-s3-prop-5-cor-3 .statement}

Toute filtre de Cauchy moins fin qu’un filtre convergent vers un point x converge aussi vers x.

C’est un conséquence du cor 2.

#### Corollaire 4 {#top-ii-s3-prop-5-cor-4 .statement}

Si $\mathcal{F}$ est un filtre de Cauchy minimal, tout ensemble de $\mathcal{F}$ a un intérieur non vide, qui appartient à $\mathcal{F}$ (en d’autres termes il existe une base de $\mathcal{F}$ formée d’ensembles ouverts).

En effet, pour tout entourage V de X, il existe un entourage ouvert U $\subset$ V (II, p. 5, cor. 2) et pour toute partie M de X, U(M) est alors ouvert et contenu dans V(M); d’où le corollaire, compte tenu de la prop. 5.

### 3. Espaces complets

Sur un espace uniforme X, un filtre de Cauchy n’a pas nécessairement de point limite.

#### Exemple 1 {#top-ii-s3-n3-exa-1 .statement}

Considérons, sur la droite rationnelle $\mathbf{Q}$, la suite $(u_n)$ définie par
$$
u_n = \sum_{p=0}^{n} 2^{-p(p+1)/2}; \text{ si } m > n, \text{ on a}
$$
$$
|u_m - u_n| \leq 2^{-n(n+3)/2}
$$
donc $(u_n)$ est une suite de Cauchy. Mais cette suite n’a pas de limite dans $\mathbf{Q}$: en effet, si le nombre rationnel $a/b$ était limite de $(u_n)$, on aurait d’après (1), quel que soit $n$
$$
|a/b - h_n/2^{n(n+1)/2}| \leq (\frac{1}{2})^{n(n+3)/2}
$$
où $h_n$ est un entier (dépendant de $n$); ou encore
$$
|a.2^{n(n+1)/2} - b h_n| \leq b.2^{-n}
$$
quel que soit $n$; or, comme le premier membre de cette inégalité est un entier quel que soit $n$, il serait nul pour tout entier $n$ supérieur à un entier $n_0$ tel que $b < 2^{n_0}$; on aurait alors $a/b = u_n$ quel que soit $n > n_0$, ce qui est absurde.

#### Exemple 2 {#top-ii-s3-n3-exa-2 .statement}

Soit X un ensemble infini, et considérons sur X la structure uniforme des partitions finies (II, p. 7, Remarque 1); tout ultrafiltre $\mathcal{F}$ sur X est un filtre de Cauchy pour cette structure. En effet, si $(A_i)$ est une partition finie de X, $V = \bigcup_i (A_i \times A_i)$ l’entourage correspondant, il existe un des $A_i$ qui appartient à $\mathcal{F}$ (I, p. 39, corollaire) et il est petit d’ordre V. Mais d’autre part, X est un espace discret infini, donc non compact, et par suite il existe des ultrafiltres sur X qui ne convergent pas.

#### Définition 3 {#top-ii-s3-def-3 .statement}

On appelle espace complet un espace uniforme tel que tout filtre de Cauchy sur cet espace soit convergent.

Dans un espace complet, toute suite de Cauchy (II, p. 13, n° 1) est donc convergente.

#### Exemple {#top-ii-s3-n3-exa-3 .statement}

Sur un espace uniforme discret X, un filtre de Cauchy est un ultrafiltre trivial (I, p. 39), donc convergent, et par suite X est complet.

Des déf. 2 (II, p. 13) et 3 et de la prop. 2 de II, p. 13, on déduit aussitôt la proposition suivante, connue sous le nom de critère de Cauchy:

#### Proposition 6 {#top-ii-s3-prop-6 .statement}

Soit $\mathcal{F}$ un filtre sur un ensemble X, et soit f une application de X dans un espace uniforme complet X'; pour que f admette une limite suivant $\mathcal{F}$, il faut et il suffit que l’image de $\mathcal{F}$ par f soit une base de filtre de Cauchy.

On voit par là l’intérêt que présentent les espaces complets dans toutes les questions où intervient la notion de limite; si une fonction prend ses valeurs dans espace complet, on pourra démontrer l’existence de sa limite, sans connaître au préalable la valeur de cette limite, ce qui serait impossible si on ne disposait, comme critère de convergence, que de la définition de la limite.

Une structure uniforme plus fine qu’une structure uniforme d’espace complet n’est pas nécessairement une structure uniforme d’espace complet (II, p. 36, exerc. 2 du § 3); mais on a la proposition suivante:

#### Proposition 7 {#top-ii-s3-prop-7 .statement}

Soient $\mathcal{U}_1, \mathcal{U}_2$ deux structures uniformes sur un ensemble $X$, $\mathcal{T}_1, \mathcal{T}_2$ les topologies déduites respectivement de ces structures uniformes. On suppose que $\mathcal{U}_1$ est plus fine que $\mathcal{U}_2$, et en outre qu’il existe un système fondamental d’entourages pour $\mathcal{U}_1$ qui sont fermés dans $X \times X$ pour la topologie produit de $\mathcal{T}_2$ par elle-même. Alors, pour qu’un filtre $\mathfrak{F}$ sur $X$ converge pour $\mathcal{T}_1$, il faut et il suffit qu’il soit un filtre de Cauchy pour $\mathcal{U}_1$ et qu’il converge pour $\mathcal{T}_2$.

Les conditions sont évidemment nécessaires, puisque $\mathcal{T}_2$ est moins fine que $\mathcal{T}_1$; prouvons qu’elles sont suffisantes. Soit $x$ un point limite de $\mathfrak{F}$ pour $\mathcal{T}_2$; montrons que $x$ est limite de $\mathfrak{F}$ pour $\mathcal{T}_1$. En effet, soit $V$ un entourage symétrique de $\mathcal{U}_1$, fermé pour la topologie produit de $\mathcal{T}_2$ par elle-même. Par hypothèse, $\mathfrak{F}$ contient un ensemble $M$ petit d’ordre $V$; si $x' \in M$, on a donc $M \subset V(x')$. Mais $V(x')$ est fermé pour $\mathcal{T}_2$, donc $x$, qui est adhérent à $M$ pour $\mathcal{T}_2$, appartient à $V(x')$; on en conclut que $M \subset \overline{V}(x)$, ce qui démontre la proposition.

#### Corollaire {#top-ii-s3-n3-cor-1 .statement}

On suppose vérifiées les hypothèses de la prop. 7. Si en outre $\mathcal{U}_2$ est une structure uniforme d’espace complet, il en est de même de $\mathcal{U}_1$.

En effet, tout filtre de Cauchy pour $\mathcal{U}_1$ est alors filtre de Cauchy pour $\mathcal{U}_2$, donc converge pour $\mathcal{T}_2$ par hypothèse.

On notera que les hypothèses du cor. de la prop. 7 sont remplies lorsque $\mathcal{T}_1 = \mathcal{T}_2$ (II, p. 5, cor. 2).

### 4. Sous-espaces des espaces complets

#### Proposition 8 {#top-ii-s3-prop-8 .statement}

Tout sous-espace fermé d’un espace complet est complet; tout sous-espace complet d’un espace uniforme séparé (complet ou non) est fermé.

En effet, soient $X$ un espace complet, $A$ un sous-espace fermé de $X$. Si $\mathfrak{F}$ est un filtre de Cauchy sur $A$, c’est une base de filtre de Cauchy sur $X$ (II, p. 13, prop. 3), qui converge donc vers un point $x \in X$; mais comme $A$ est fermé, on a $x \in A$, ce qui prouve que dans le sous-espace $A$, $\mathfrak{F}$ est convergent.

Soient maintenant $A$ un ensemble non fermé dans un espace uniforme séparé $X$, et soit $b \in \overline{A} - A$; la trace $\mathfrak{V}_A$ sur $A$ du filtre $\mathfrak{V}$ des voisinages de $b$ dans $X$ est un filtre de Cauchy sur $A$; il ne peut converger vers un point $c \in A$, car alors $c$ serait point limite de $\mathfrak{V}$ (II, p. 15, cor. 3) ce qui est absurde puisque $b \neq c$ et que $X$ est séparé.

#### Proposition 9 {#top-ii-s3-prop-9 .statement}

*Soient $X$ un espace uniforme, $A$ une partie partout dense de $X$ telle que toute base de filtre de Cauchy sur $A$ soit convergente dans $X$; dans ces conditions, $X$ est complet.*

Il suffit de montrer qu’un filtre de Cauchy *minimal* $\mathcal{F}$ sur $X$ est convergent. Comme $A$ est partout dense et que tout ensemble de $\mathcal{F}$ a un intérieur non vide (II, p. 15, cor. 4), la trace $\mathcal{F}_A$ de $\mathcal{F}$ sur $A$ est un filtre de Cauchy sur $A$, donc converge vers un point $x_0 \in X$; comme $\mathcal{F}$ est moins fin que le filtre sur $X$ engendré par $\mathcal{F}_A$, on en conclut que $\mathcal{F}$ converge vers $x_0$ (II, p. 15, cor. 3).

### 5. Produits et limites projectives d’espaces complets

#### Proposition 10 {#top-ii-s3-prop-10 .statement}

*Tout produit d’espaces uniformes complets est complet. Réciproquement, si un produit d’espaces uniformes non vides est complet, chacun des espaces uniformes facteurs est complet.*

La première assertion résulte de la caractérisation des filtres de Cauchy et des filtres convergents sur un espace produit (II, p. 14, cor. 2 de la prop. 4 et I, p. 51, cor. 1). Inversement, supposons $X = \prod_{\iota \in I} X_\iota$ complet (les $X_\iota$ étant non vides) et soit $\mathcal{F}_k$ un filtre de Cauchy sur $X_k$; pour tout $\iota \neq k$, soit $\mathcal{F}_\iota$ un filtre de Cauchy sur $X_\iota$, et considérons le filtre produit (I, p. 42) $\mathcal{F} = \prod_{\iota \in I} \mathcal{F}_\iota$ sur $X$; $\mathcal{F}$ est un filtre de Cauchy (II, p. 14, cor. 2 de la prop. 4), donc est convergent, et il en est par suite de même de $\operatorname{pr}_k \mathcal{F} = \mathcal{F}_k$ (I, p. 51, cor. 1).

#### Corollaire {#top-ii-s3-n5-cor-1 .statement}

*Soit $(X_\alpha, f_{\alpha\beta})$ un système projectif d’espaces uniformes. Si les $X_\alpha$ sont séparés et complets, il en est de même de $X = \lim_{\leftarrow} X_\alpha$.*

On sait en effet que $X$ est séparé et s’identifie à un sous-espace fermé de $\prod_\alpha X_\alpha$ (I, p. 55, cor. 2); le corollaire résulte donc de la prop. 10 et de la prop. 8 (II, p. 16).

Une limite projective d’espaces uniformes séparés et complets $X_\alpha$ peut être *vide*, même si les $X_\alpha$ sont non vides et les $f_{\alpha\beta}$ surjectifs, comme le montre le cas des espaces discrets (E, III, p. 94, exerc. 4). Mais on a le théorème suivant:

**Théorème 1** (Mittag-Leffler). — *Soit $(X_\alpha, f_{\alpha\beta})$ un système projectif d’espaces uniformes séparés et complets, relatif à un ensemble d’indices préordonné filtrant $I$ qui admet un sous-ensemble cofinal dénombrable; on suppose en outre que, pour tout $\alpha \in I$, $X_\alpha$ possède un système fondamental dénombrable d’entourages.\footnote{Cette condition signifie que l’espace uniforme séparé $X_\alpha$ est métrisable; cf. IX, § 2, n°4, th. 1.*} Enfin, on suppose que pour tout $\alpha \in I$, il existe un $\beta \geq \alpha$ vérifiant la condition suivante:

(ML_{\alpha,\beta}) Pour tout $\gamma \geq \beta$, $f_{\alpha\gamma}(X_\gamma)$ est dense dans $f_{\alpha\beta}(X_\beta)$.

Soient alors $X = \lim_{\leftarrow} X_\alpha$, $f_\alpha$ l’application canonique $X \to X_\alpha$; pour tout $\alpha \in I$ et tout $\beta \geq \alpha$ vérifiant (ML_{\alpha,\beta}), $f_\alpha(X)$ est dense dans $f_{\alpha\beta}(X_\beta)$ (et par suite $X$ est non vide si les $X_\alpha$ sont tous non vides).

Soit $(\lambda_n)$ une suite d’indices cofinale à I. Partons d’un $\alpha_0 \in I$, et définissons par récurrence une suite croissante $(\alpha_n)$ telle que $\alpha_n \geq \lambda_n$ et que (ML_{\alpha_n,\alpha_{n+1}}) soit vérifiée; il est clair que la suite $(\alpha_n)$ est cofinale à I. Nous écrirons $f_{mn}$ au lieu de $f_{\alpha_m\alpha_n}$ pour $m \leq n$, et nous poserons $f_{n,n+1}(X_{\alpha_{n+1}}) = Y_n$. Alors, pour $m \leq n$, $f_{mn}(Y_n)$ est dense dans $Y_m$: en effet, par définition, $f_{m,n+1}(X_{\alpha_{n+1}})$ est dense dans $f_{m,m+1}(X_{\alpha_{m+1}}) = Y_m$, et comme $f_{m,n+1}(X_{\alpha_{n+1}}) = f_{mn}(f_{n,n+1}(X_{\alpha_{n+1}})) = f_{mn}(Y_n)$, cela établit notre assertion.

Par récurrence sur $n$ et $k$, on peut, pour chaque $n$, définir un système fondamental $(V_{kn})_{k \in \mathbf{N}}$ d’entourages symétriques fermés de $X_{\alpha_n}$ tel que

(2)
$$
\overline{V}_{k+1,n} \subset V_{kn}
$$

(3)
$$
(f_{n,n+1} \times f_{n,n+1})(V_{k,n+1}) \subset V_{kn}.
$$

Soit en effet $(U_{kn})_{k \in \mathbf{N}}$ un système fondamental d’entourages de $X_{\alpha_n}$. Si on suppose les $V_{kn}$ définis pour un $n$ donné et pour tout $k \in \mathbf{N}$, on peut, puisque $f_{n,n+1}$ est uniformément continue, définir par récurrence sur $k$ l’entourage $V_{k,n+1}$ de sorte que (3) soit vérifié et que l’on ait en outre

$$
\overline{V}_{k+1,n+1} \subset V_{k,n+1} \cap U_{k+1,n+1},
$$

d’où notre assertion.

Cela étant, soit $x_0 \in Y_0$. Nous allons prouver que, pour tout entier $k > 0$, il existe $z \in X$ tel que $(x_0, f_{\alpha_0}(z)) \in V_{k-1,0}$, ce qui démontrera le théorème. Comme $f_{n,n+1}(Y_{n+1})$ est dense dans $Y_n$, on peut définir par récurrence une suite de points $x_n \in Y_n$ tels que

(4)
$$
(x_n, f_{n,n+1}(x_{n+1})) \in V_{k+n,n}.
$$

En vertu de (3), on en déduit que, pour tout $m \leq n$,

(5)
$$
(f_{mn}(x_n), f_{m,n+1}(x_{n+1})) \in V_{k+n,m}.
$$

On conclut de là que, pour $m$ fixe, la suite $(f_{mn}(x_n))_{n \geq m}$ est une suite de Cauchy dans $X_{\alpha_m}$, et converge par suite vers un point $z_m$; en effet, par récurrence, on déduit de (5) que pour tout couple d’entiers $p \geq m, q > 0$, on a

(6)
$$
(f_{mp}(x_p), f_{m,p+q}(x_{p+q})) \in V_{k+p+q-1,m} \circ V_{k+p+q-2,m} \circ \cdots \circ V_{k+p,m}
$$

et en vertu de (2), il est immédiat que le second membre de (6) est contenu dans $V_{k+p-1,m}$; faisant croître $q$ indéfiniment, on en tire en particulier, pour $m = p = 0$, que $(x_0, z_0) \in V_{k-1,0}$, puisque $V_{k-1,0}$ est fermé. D’autre part, des relations z_m = \lim_{n \to \infty} f_{mn}(x_n) et de la continuité de $f_{m,m+1}$, on déduit que $f_{m,m+1}(z_{m+1}) = z_m$ pour tout $m \geqslant 0$. Pour tout $\gamma \in I$, il y a au moins un entier $n$ tel que $\alpha_n \geqslant \gamma$; si on pose $z_\gamma = f_{\gamma,\alpha_n}(z_n)$, on vérifie aussitôt que $z_\gamma$ ne dépend pas de la valeur de $n$ telle que $\alpha_n \geqslant \gamma$, et que la famille $(z_\alpha)_{\alpha \in I}$ ainsi définie est un point $z$ de $X = \lim_{\leftarrow} X_\alpha$; comme $f_{\alpha_0}(z) = z_0$, cela termine la démonstration.

#### Corollaire 1 {#top-ii-s3-prop-10-cor-1 .statement}

*Soit* $(X_\alpha, f_{\alpha\beta})$ *un système projectif d’ensembles tel que* $I$ *soit filtrant et admette un sous-ensemble cofinal dénombrable, et que les* $f_{\alpha\beta}$ *soient surjectives; si* $X = \lim_{\leftarrow} X_\alpha$, *l’application canonique* $f_\alpha : X \to X_\alpha$ *est surjective pour tout* $\alpha \in I$.

Il suffit en effet de munir les $X_\alpha$ de la structure uniforme discrète.

#### Corollaire 2 {#top-ii-s3-prop-10-cor-2 .statement}

*Soit* $I$ *un ensemble préordonné filtrant ayant un ensemble cofinal dénombrable. Soient* $(X_\alpha, f_{\alpha\beta}), (X'_\alpha, f'_{\alpha\beta})$ *deux systèmes projectifs d’ensembles relatifs à* $I$, *et pour tout* $\alpha \in I$, *soit* $u_\alpha : X_\alpha \to X'_\alpha$ *une application telle que les* $u_\alpha$ *forment un système projectif d’applications; posons* $u = \lim_{\leftarrow} u_\alpha$. *Soit* $x' = (x'_\alpha)$ *un élément de* $X' = \lim_{\leftarrow} X'_\alpha$ *vérifiant la condition suivante: pour tout* $\alpha \in I$, *il existe* $\beta \geqslant \alpha$ *tel que, pour tout* $\gamma \geqslant \beta$, *on ait* $f_{\alpha\gamma}(\overline{u}_\gamma(x'_\gamma)) = f_{\alpha\beta}(\overline{u}_\beta(x'_\beta))$; *alors il existe* $x \in X = \lim_{\leftarrow} X_\alpha$ *tel que* $u(x) = x'$.

Il suffit d’appliquer le th. 1 au système projectif des ensembles $\overline{u}_\alpha^{-1}(x'_\alpha)$, munis de la structure uniforme discrète (cf. E, III, p. 58, prop. 5).

#### Exemple {#top-ii-s3-n5-exa-1 .statement}

Supposons donnés, dans $\mathbf{C}$: 1° une suite $(a_n)$ de points distincts tels que la suite $(|a_n|)$ soit croissante et tende vers $+\infty$; 2° pour chaque $n$, une fonction rationnelle $z \mapsto R_n(z)$ définie dans $\mathbf{C} - \{a_n\}$ et ayant un pôle au point $a_n$; 3° une suite strictement croissante $(B_n)$ de boules ouvertes de centre 0, de réunion $\mathbf{C}$, telle qu’aucun des $a_k$ ne soit sur la frontière d’une des boules $B_n$. Pour chaque $n$, désignons par $B'_n$ l’intersection de $\overline{B}_n$ et du complémentaire dans $\mathbf{C}$ de l’ensemble des $a_m$; soit $X_n$ l’ensemble des applications $z \mapsto S(z) = P(z) + \sum_{a_k \in B'_n} R_k(z)$ de $B'_n$ dans $\mathbf{C}$, où $P$ est la restriction à $B'_n$ d’une fonction continue dans $\overline{B}_n$ et holomorphe dans $B_n$. On définit une distance dans $X_n$ en posant $d_n(S_1, S_2) = \sup_{z \in B'_n} |S_1(z) - S_2(z)|$. On vérifie aisément que pour cette distance, $X_n$ est *complet*. Enfin, pour $n \leqslant m$, on définit une application $f_{nm} : X_m \to X_n$ en faisant correspondre à $S \in X_m$ sa *restriction* à $B'_n$; il est clair que les $f_{nm}$ sont *uniformément continues* et que $(X_n, f_{nm})$ est un système projectif d’espaces uniformes. Cela étant, il est clair qu’un élément de la *limite projective* $X = \lim_{\leftarrow} X_n$ s’identifie canoniquement à une *fonction méromorphe* $F$ dans $\mathbf{C}$, dont les seuls pôles sont les points $a_n$, et qui est telle que pour tout $n$, $F(z) - R_n(z)$ est *holomorphe au point* $a_n$. Le théorème classique de Mittag–Leffler affirme que $X$ *n’est pas vide*; en vertu du th. 1, il suffit pour le démontrer de vérifier la condition $(\mathrm{ML}_{n,n+1})$ pour tout $n$. Or, soit $S_{n+1} = P_{n+1} + \sum_{a_k \in B_{n+1}} R_k$ un élément de $X_{n+1}$, où $P_{n+1}$ est continue dans $\overline{B}_{n+1}$ et holomorphe dans $B_{n+1}$; pour tout $m \geqslant n+1$, soit $Q_{mn}$ la restriction à $B'_m$ de $\sum_{a_h \in B_m - B_{n+1}} R_h$; cette dernière somme est une fonction holomorphe dans un voisinage de $\overline{B}_n$, donc (par le développement de Taylor), pour tout $\varepsilon > 0$, il y a un polynôme $P_{mn}$ tel que $|P_{n+1}(z) - Q_{mn}(z) - P_{mn}(z)| \leqslant \varepsilon$ dans $B_n$; si $S_m$ est la restriction à $B'_m$ de $P_{mn} + \sum_{a_h \in B_m} R_h$ on a $S_m \in X_m$ et $|S_m(z) - S_{n+1}(z)| \leqslant \varepsilon$ dans $B'_n$, ce qui achève la démonstration.*

### 6. Prolongement des fonctions uniformément continues

Il est possible d’apporter d’importants compléments au théorème de prolongement par continuité (I, p. 57, th. 1) lorsqu’il s’agit de fonctions prenant leurs valeurs dans un espace uniforme séparé et complet.

#### Proposition 11 {#top-ii-s3-prop-11 .statement}

Soient $A$ une partie partout dense d’un espace topologique $X$, et $f$ une application de $A$ dans un espace uniforme séparé et complet $X'$. Pour que $f$ puisse être prolongée par continuité dans $X$, il faut et il suffit que, pour tout $x \in X$, l’image par $f$ de la trace sur $A$ du filtre des voisinages de $x$ dans $X$ soit une base de filtre de Cauchy sur $X'$.

Cela résulte du th. de prolongement par continuité (loc. cit.), puisque $X'$ est régulier (II, p. 5, prop. 3) et qu’il y a identité entre filtres convergents et filtres de Cauchy sur $X'$.

Lorsque $X$ est lui-même un espace uniforme, on a de plus le théorème suivant:

#### Théorème 2 {#top-ii-s3-thm-2 .statement}

Soit $f$ une fonction définie dans un sous-espace partout dense $A$ d’un espace uniforme $X$, prenant ses valeurs dans un espace uniforme séparé et complet $X'$, et uniformément continue dans $A$. Alors $f$ peut être prolongée par continuité à $X$ tout entier, et la fonction prolongée $\bar{f}$ est uniformément continue.

L’existence de $\bar{f}$ est une conséquence immédiate des prop. 3 (II, p. 13) et 11. Montrons que $\bar{f}$ est uniformément continue. Soit $V'$ un entourage symétrique fermé de $X'$, et soit $V$ un entourage de $X$ tel que, lorsque $x, y$ sont dans $A$ et voisins d’ordre $V$, $f(x)$ et $f(y)$ soient voisins d’ordre $V'$. On peut supposer que $V$ est l’adhérence dans $X \times X$ d’un entourage $W$ de $A$ (II, p. 10, prop. 6). On a $(\bar{f}(x), \bar{f}(y)) \in V'$ pour $(x, y) \in W$; comme $\bar{f} \times \bar{f}$ est continue dans $X \times X$ (I, p. 25, prop. 1), on a aussi $(\bar{f}(x), \bar{f}(y)) \in V'$ pour $(x, y) \in V = \overline{W}$ puisque $V'$ est fermé (I, p. 9, th. 1).

C.Q.F.D.

#### Corollaire {#top-ii-s3-n6-cor-1 .statement}

Soient $X_1, X_2$ deux espaces uniformes séparés et complets, $Y_1, Y_2$ des sous-espaces partout denses de $X_1, X_2$ respectivement. Tout isomorphisme $f$ de $Y_1$ sur $Y_2$ se prolonge en un isomorphisme de $X_1$ sur $X_2$.

En effet, $f$ est uniformément continue dans $Y_1$, donc (th. 2) se prolonge en une application uniformément continue $\bar{f}: X_1 \to X_2$; de même l’application réciproque $g$ de $f$ se prolonge en une application uniformément continue $\bar{g}: X_1 \to X_2$. La fonction $\bar{g} \circ \bar{f}$ est alors une application continue de $X_1$ dans lui-même qui coïncide dans $Y_1$ avec l’application identique; en vertu du principe de prolongement des identités (I, p. 53, cor. 1), $\bar{g} \circ \bar{f}$ est donc l’application identique de $X_1$; de même $\bar{f} \circ \bar{g}$ est l’application identique de $X_2$. Par suite (E, II, p. 18, corollaire) $\bar{f}$ et $\bar{g}$ sont deux bijections réciproques l’une de l’autre; comme elles sont uniformément continues, ce sont des isomorphismes (II, p. 6, prop. 2).

On notera que si $f$ est une application uniformément continue bijective de $Y_1$ sur $Y_2$, son prolongement par continuité $\bar{f}$ n’est pas nécessairement injectif ni surjectif (II, p. 36, exerc. 3).

### 7. La complétion d’un espace uniforme

#### Théorème 3 {#top-ii-s3-thm-3 .statement}

Soit X un espace uniforme. Il existe un espace uniforme séparé et complet $\hat{X}$, et une application uniformément continue $i : X \to \hat{X}$, ayant la propriété suivante:

(P) Pour toute application uniformément continue $f$ de X dans un espace uniforme séparé et complet Y, il existe une application uniformément continue $g : \hat{X} \to Y$ et une seule telle que $f = g \circ i$.

Si $(i_1, X_1)$ est un second couple formé d’un espace uniforme séparé et complet $X_1$ et d’une application uniformément continue $i_1 : X \to X_1$, possédant la propriété (P), alors il existe un isomorphisme $\varphi : \hat{X} \to X_1$ et un seul tel que $i_1 = \varphi \circ i$.

La première assertion de l’énoncé signifie encore que le couple $(i, \hat{X})$ est solution du problème d’application universelle (E, IV, p. 23) dans lequel on prend pour $\Sigma$-ensembles les espaces uniformes séparés et complets, pour $\sigma$-morphismes les applications uniformément continues et pour $\alpha$-applications les applications uniformément continues de X dans un espace uniforme séparé et complet. L’unicité du couple $(i, \hat{X})$ à un isomorphisme unique près résulte donc des propriétés générales des solutions de problèmes d’application universelle (loc. cit.). Reste à prouver l’existence du couple $(i, \hat{X})$.

1) Définition de $\hat{X}$. Soit $\hat{X}$ l’ensemble des filtres de Cauchy minimaux (II, p. 14) sur X. Nous allons définir sur $\hat{X}$ une structure uniforme. Pour cela, pour tout entourage symétrique V de X, désignons par $\tilde{V}$ l’ensemble des couples $(\mathcal{X}, \mathcal{Y})$ de filtres de Cauchy minimaux ayant en commun un ensemble petit d’ordre V : montrons que les ensembles $\tilde{V}$ forment un système fondamental d’entourages d’une structure uniforme sur $\hat{X}$. En effet:

1° Comme tout $\mathcal{X} \in \hat{X}$ est un filtre de Cauchy, on a par définition $(\mathcal{X}, \mathcal{X}) \in \tilde{V}$ pour tout entourage symétrique V de X, donc $(U'_I)$ est vérifié.

2° Si V, V’ sont deux entourages symétriques de X, $W = V \cap V'$ est un entourage symétrique, et tout ensemble petit d’ordre W est petit d’ordre V et d’ordre V’ ; donc on a $\tilde{W} \subset \tilde{V} \cap \tilde{V}'$, ce qui prouve $(B_I)$.

3° Les ensembles $\tilde{V}$ sont symétriques par définition, donc $(U''_{II})$ est vérifié.

4° Étant donné un entourage symétrique V de X, soit W un entourage symétrique tel que $\tilde{W} \subset V$. Considérons trois filtres de Cauchy minimaux $\mathcal{X}, \mathcal{Y}, \mathcal{Z}$ tels que $(\mathcal{X}, \mathcal{Y}) \in \tilde{W}$ et $(\mathcal{Y}, \mathcal{Z}) \in \tilde{W}$; il existe donc deux ensembles M, N, petits d’ordre W et tels que $M \in \mathcal{X} \cap \mathcal{Y}, N \in \mathcal{Y} \cap \mathcal{Z}$. Comme M et N appartiennent à $\mathcal{Y}$, $M \cap N$ n’est pas vide, donc (II, p. 12, prop. 1), $M \cup N$ est petit d’ordre $\tilde{W} \subset V$; comme $M \cup N$ appartient à $\mathcal{X}$ et à $\mathcal{Z}$, on a $\tilde{W} \subset \tilde{V}$; d’où $(U'''_{III})$.

Montrons en outre que l’espace uniforme $\hat{X}$ est séparé. En effet, soient $\mathcal{X}, \mathcal{Y}$ deux filtres de Cauchy minimaux sur X tels que $(\mathcal{X}, \mathcal{Y}) \in \tilde{V}$ pour tout entourage symétrique V de X. Il est immédiat que les ensembles $M \cup N$, où $M \in \mathcal{X}, N \in \mathcal{Y}$ forment la base d’un filtre $\mathcal{Z}$ moins fin que $\mathcal{X}$ et que $\mathcal{Y}$. Or, $\mathcal{Z}$ est un filtre de Cauchy, car pour tout entourage symétrique V de X, il y a par hypothèse un ensemble P petit d’ordre V et appartenant à la fois à $\mathcal{X}$ et à $\mathcal{Y}$, donc $P \in \mathcal{S}$. Par définition des filtres de Cauchy minimaux, on a $\mathcal{X} = \mathcal{S} = \mathcal{Y}$, et cela achève de montrer que $\hat{X}$ est séparé.

2) *Définition de i ; la structure uniforme de X est image réciproque de celle de $\hat{X}$ par i.* On sait que, pour tout $x \in X$, le filtre des voisinages $\mathfrak{V}(x)$ de $x$ dans $X$ est un filtre de Cauchy minimal (II, p. 14, cor. 1 de la prop. 5); nous prendrons $i(x) = \mathfrak{V}(x)$. Soit $j = i \times i$; nous allons montrer que pour tout entourage symétrique $V$ de $X$, on a $j^{-1}(\tilde{V}) \subset V \subset j^{-1}(\tilde{V})^3$, ce qui prouvera notre assertion (II, p. 9). Or, si $(i(x), i(y)) \in \tilde{V}$, il y a un ensemble $M$ petit d’ordre $V$ et qui est à la fois voisinage de $x$ et de $y$, donc $(x, y) \in V$. Inversement, si $(x, y) \in V$, il est immédiat que l’ensemble $V(x) \cup V(y)$ est petit d’ordre $\tilde{V}$ et est à la fois voisinage de $x$ et de $y$.

3) $\hat{X}$ est complet et $i(X)$ dense dans $\hat{X}$. Cherchons la trace sur $i(X)$ d’un voisinage $\tilde{V}(\mathcal{X})$ d’un point $\mathcal{X} \in \hat{X}$; c’est l’ensemble des $i(x)$ tels que $(\mathcal{X}, i(x)) \in \tilde{V}$. Cette relation signifie qu’il existe un voisinage de $x$ dans $X$, petit d’ordre $V$ et appartenant à $\mathcal{X}$, ou encore que $x$ est *intérieur à un ensemble de $\mathcal{X}$ petit d’ordre* $V$. Soit $M$ la réunion dans $X$ des intérieurs des ensembles de $\mathcal{X}$ qui sont petits d’ordre $V$; $M$ appartient à $\mathcal{X}$ (II, p. 15, cor. 4) et ce qui précède montre que $\tilde{V}(\mathcal{X}) \cap i(X) = i(M)$; on en conclut que:
1° $\tilde{V}(\mathcal{X}) \cap i(X)$ n’est pas vide, donc $i(X)$ est *dense* dans $\hat{X}$;
2° La trace sur $i(X)$ de $\tilde{V}(\mathcal{X})$ appartient à la *base de filtre* $i(\mathcal{X})$ sur $\hat{X}$, donc cette base de filtre converge dans $\hat{X}$ vers le *point* $\mathcal{X}$.

Soit alors $\mathcal{F}$ un filtre de Cauchy sur $i(X)$; d’après ce qu’on a vu dans 2) et la prop. 4 de II, p. 13, $i^{-1}(\mathcal{F})$ est une base d’un filtre de Cauchy $\mathcal{G}$ sur $X$; soit $\mathcal{X}$ un filtre de Cauchy minimal moins fin que $\mathcal{G}$ (II, p. 14, prop. 5); $i(\mathcal{X})$ est alors une base d’un filtre de Cauchy sur $i(X)$ (II, p. 13, prop. 3) et $\mathcal{F} = i^{-1}(i(\mathcal{F}))$ est plus fin que le filtre de base $i(\mathcal{X})$. Comme ce dernier converge dans $\hat{X}$, il en est de même de $\mathcal{F}$, et la prop. 9 de II, p. 17 montre alors que $\hat{X}$ est *complet*.

4) *Vérification de la propriété* (P). Soit $f$ une application uniformément continue de $X$ dans un espace uniforme *séparé* et *complet* $Y$. Montrons d’abord qu’il existe une application uniformément continue $g_0 : i(X) \to Y$ et une seule telle que $f = g_0 \circ i$. En effet, comme $f$ est continue, on a nécessairement $f(x) = \lim f(\mathfrak{V}(x))$, donc si on pose $g_0(i(x)) = \lim f(\mathfrak{V}(x))$, on a bien $f = g_0 \circ i$; tout revient à voir que $g_0$ est *uniformément continue* dans $i(X)$. Or, soit $U$ un entourage de $Y$ et soit $V$ un entourage symétrique de $X$ tel que la relation $(x, x') \in V$ entraîne $(f(x), f(x')) \in U$; on a vu dans 2) que la relation $(i(x), i(x')) \in \tilde{V}$ entraîne $(x, x') \in V$, donc aussi $(g_0(i(x)), g_0(i(x')))) \in U$, ce qui établit notre assertion.

Cela étant, soit $g$ le prolongement par continuité de $g_0$ à $\hat{X}$ (II, p. 20, th. 2); on peut aussi écrire $f = g \circ i$, et il est clair que $g$ est l’unique application continue de $\hat{X}$ dans $Y$ vérifiant la relation précédente puisque $i(X)$ est dense dans $\hat{X}$ (I, p. 53, cor. 1).

C.Q.F.D.

#### Définition 4 {#top-ii-s3-def-4 .statement}

On dit que l’espace uniforme séparé et complet $\hat{X}$ défini dans la démonstration du th. 3 est l’espace séparé complété de $X$ et que l’application $i : X \to \hat{X}$ est l’application canonique de $X$ dans son séparé complété.

Notons en outre les propriétés suivantes:

#### Proposition 12 {#top-ii-s3-prop-12 .statement}

1° Le sous-espace $i(X)$ est dense dans $\hat{X}$.
    2° Le graphe de la relation d’équivalence $i(x) = i(x')$ est l’intersection des entourages de $X$.
    3° La structure uniforme de $X$ est l’image réciproque par $i$ de celle de $\hat{X}$ (ou de celle du sous-espace $i(X)$).
    4° Les entourages de $i(X)$ sont les images par $i \times i$ des entourages de $X$, et les adhérences dans $\hat{X} \times \hat{X}$ des entourages de $i(X)$ forment un système fondamental d’entourages de $\hat{X}$.

En effet, 1° et 3° ont été prouvées au cours de la démonstration du th. 3; 4° est conséquence de 1° et 3° en vertu de propriétés générale vues antérieurement (II, p. 9, Remarque et II, p. 10, prop. 6). Enfin, la relation $i(x) = i(x')$ signifie par définition que les filtres de voisinages de $x$ et de $x'$ sont les mêmes. Mais cela entraîne par définition que $(x, x') \in V$ pour tout entourage $V$ de $X$, et la réciproque est évidente.

#### Corollaire {#top-ii-s3-n7-cor-1 .statement}

Si $X$ est un espace uniforme séparé, l’application canonique $i : X \to \hat{X}$ est un isomorphisme de $X$ sur un sous-espace partout dense de $\hat{X}$.

Lorsque $X$ est séparé, on dit que $X$ est l’espace complété (ou plus brièvement le complété) de $X$, et on identifie le plus souvent $X$ à un sous-espace partout dense de $\hat{X}$ au moyen de $i$.

#### Remarque {#top-ii-s3-n7-rem-1 .statement}

Lorsqu’on fait cette identification, les filtres de Cauchy minimaux de $X$ ne sont autres que les traces sur $X$ des filtres de voisinages des points de $\hat{X}$, comme il résulte de la démonstration du th. 3 (II, p. 21).

Le cor. de la prop. 12 caractérise le complété d’un espace uniforme séparé:

#### Proposition 13 {#top-ii-s3-prop-13 .statement}

Si $Y$ est un espace séparé et complet, $X$ un sous-espace partout dense de $Y$, l’injection canonique $X \to Y$ se prolonge en un isomorphisme de $\hat{X}$ sur $Y$.

En effet, toute application uniformément continue de $X$ dans un espace uniforme séparé et complet $Z$ se prolonge d’une seule manière en une application uniformément continue de $Y$ dans $Z$ en vertu de II, p. 20, th. 2.

#### Proposition 14 {#top-ii-s3-prop-14 .statement}

Soient $X$ un espace uniforme séparé et complet, $\mathcal{U}$ sa structure uniforme, $Z$ un sous-espace partout dense dans $X$. Si $\mathcal{U}'$ est une structure uniforme sur $X$, moins fine que $\mathcal{U}$ et induisant sur $Z$ la même structure uniforme que $\mathcal{U}$, on a $\mathcal{U}' = \mathcal{U}$.

Désignons par $X'$ l’ensemble $X$ muni de la structure uniforme $\mathcal{U}'$; la composée de l’application canonique $X' \to \hat{X}'$ et de l’application identique $X \to X'$, qui est uniformément continue, peut être considérée comme une application uniformément continue $\varphi : X \to \hat{X}'$; comme $Z$ est séparé pour la structure uniforme induite par $\mathcal{U}'$, la restriction de $\varphi$ à $Z$ est par hypothèse un isomorphisme de $Z$ sur le sous-espace partout dense $\varphi(Z)$ de $\hat{X}'$; il en résulte (II, p. 20, corollaire) que $\varphi$ lui-même est un isomorphisme de $X$ sur $\hat{X}'$, donc $X' = \hat{X}'$ et $\mathcal{U}' = \mathcal{U}$.

#### Proposition 15 {#top-ii-s3-prop-15 .statement}

*Soient $X, X'$ deux espaces uniformes; pour toute application uniformément continue $f : X \to X'$, il existe une application uniformément continue et une seule $\hat{f} : \hat{X} \to \hat{X}'$ rendant commutatif¹ le diagramme*

$$
\begin{array}{ccc}
X & \xrightarrow{f} & X' \\
i \downarrow & & i' \downarrow \\
\hat{X} & \xrightarrow{\hat{f}} & \hat{X}'
\end{array}
$$

*où $i : X \to \hat{X}$ et $i' : X' \to \hat{X}'$ sont les applications canoniques.*

Il suffit d’appliquer le th. 3 (II, p. 21) à la fonction $i' \circ f : X \to \hat{X}'$.

#### Corollaire {#top-ii-s3-n7-cor-2 .statement}

*Soient $f : X \to X'$ et $g : X' \to X''$ deux applications uniformément continues; si $h = g \circ f$, on a $\hat{h} = \hat{g} \circ \hat{f}$.*
Cela résulte aussitôt de la propriété d’unicité de la prop. 15.

### 8. Espace uniforme séparé associé à un espace uniforme

#### Proposition 16 {#top-ii-s3-prop-16 .statement}

*Soient $X$ un espace uniforme, i l’application canonique de $X$ dans son séparé complété $\hat{X}$. Pour toute application uniformément continue $f$ de $X$ dans un espace uniforme séparé $Y$, il existe une application uniformément continue et une seule $h : i(X) \to Y$ telle que $f = h \circ i$.*

En effet (II, p. 23, corollaire) on peut identifier $Y$ à un sous-espace de son complété $\hat{Y}$, et $f$ peut alors être considérée comme une application uniformément continue de $X$ dans $\hat{Y}$. En vertu du th. 3 (II, p. 21), elle s’écrit donc $f = g \circ i$, où $g$ est une application uniformément continue de $\hat{X}$ dans $\hat{Y}$; si $h$ est la restriction de $g$ à $i(X)$, on a évidemment $f = h \circ i$, et $h$ applique $i(X)$ dans $Y$; l’unicité de $h$ est triviale.

Le couple $(i, i(X))$ est donc solution du *problème d’application universelle* (E, IV, p. 23) où cette fois on prend comme $\Sigma$-ensembles les espaces uniformes *séparés*, pour $\sigma$-morphismes (resp. $\alpha$-applications) les applications uniformément continues (resp. les applications uniformément continues de $X$ dans un espace uniforme séparé).

#### Définition 5 {#top-ii-s3-def-5 .statement}

*On dit que l’espace uniforme séparé $i(X)$ défini dans la démonstration du th. 3 (II, p. 21) est l’espace uniforme séparé associé à $X$.*

¹ Autrement dit $i' \circ f = \hat{f} \circ i$.

Par suite, le séparé complété de X n’est autre que le complété de l’espace séparé associé à X. Si X est complet, il résulte de la définition de $\hat{X}$ (II, p. 21, th. 3) que l’application $i : X \to \hat{X}$ est surjective, donc l’espace séparé associé à X est égal à l’espace séparé complété de X réciproquement, s’il en est ainsi, X est complet (II, p. 23, prop. 12 et II, p. 15, déf. 3).

#### Corollaire {#top-ii-s3-n8-cor-1 .statement}

Soient X, Y deux espaces uniformes, $X', Y'$ les espaces séparés associés; pour toute application uniformément continue $f : X \to Y$, il existe une application uniformément continue et une seule $f' : X' \to Y'$ rendant commutatif le diagramme

$$
\begin{array}{ccc}
X & \xrightarrow{f} & Y \\
i \downarrow & & \downarrow i' \\
X' & \xrightarrow{f'} & Y'
\end{array}
$$

où i et $i'$ sont les applications canoniques.

On applique la prop. 16 à $i' \circ f : X \to Y'$.

L’espace séparé associé à un espace uniforme peut encore se caractériser par la propriété suivante:

#### Proposition 17 {#top-ii-s3-prop-17 .statement}

Soient X un espace uniforme, $i(X)$ son espace séparé associé, f une application de X sur un espace uniforme séparé $X'$, telle que la structure uniforme de X soit l’image réciproque par f de celle de $X'$. Alors l’application $g : i(X) \to X'$ telle que $f = g \circ i$ est un isomorphisme.

On sait que g est uniformément continue (II, p. 24, prop. 16); g est évidemment surjective, et elle est aussi injective puisque la relation $f(x) = f(y)$ entraîne par définition que $(x, y)$ appartient à tous les entourages de X, donc que $i(x) = i(y)$ (II, p. 23, prop. 12). Enfin, les entourages de $X'$ sont les images par $f \times f$ des entourages de X (II, p. 9, Remarque), donc aussi les images par $g \times g$ des entourages de $i(X)$ (II, p. 23, prop. 12), d’où la proposition.

#### Remarque {#top-ii-s3-n8-rem-1 .statement}

Soit R la relation d’équivalence $i(x) = i(x')$ dans X; on a vu (II, p. 23, prop. 12) que son graphe C est l’intersection des entourages de X. Il est clair que tout ensemble ouvert (et par suite aussi tout ensemble fermé) dans X est saturé pour R; compte tenu de la définition de l’image réciproque d’une topologie, on en conclut que la bijection canonique de l’espace topologique quotient $X/R$ sur $i(X)$ déduite de i est un homéomorphisme; l’espace séparé associé à X peut donc s’identifier en tant qu’espace topologique à $X/R$. L’application canonique $i : X \to i(X)$ est ouverte et fermée, et même propre (I, p. 77, Exemple).

Soient $X'$ un second espace uniforme, $C'$ l’intersection des entourages de $X'$, $R'$ la relation d’équivalence de graphe $C'$. Soit $f : X \to X'$ une application continue: comme l’image réciproque par f de tout voisinage de $f(x)$ est un voisinage de x, l’image réciproque par f de $C'(f(x))$ contient $C(x)$, donc f est compatible avec R et $R'$, et donne par passage aux quotients une application continue $X/R \to X'/R'$ (I, p. 21, corollaire); ceci généralise le cor. de la prop. 16.

### 9. Complétion des sous-espaces et des espaces produits

#### Proposition 18 {#top-ii-s3-prop-18 .statement}

Soient $X$ un ensemble, $(Y_\lambda)_{\lambda \in L}$ une famille d’espaces uniformes, et pour chaque $\lambda \in L$, soit $f_\lambda$ une application de $X$ dans $Y_\lambda$; on munit $X$ de la structure uniforme la moins fine $\mathcal{U}$ rendant uniformément continues les $f_\lambda$. Alors la structure uniforme de l’espace séparé complété $\hat{X}$ de $X$ est la moins fine rendant uniformément continues les applications $f_\lambda : \hat{X} \to \hat{Y}_\lambda$ ($\lambda \in L$) (II, p. 24, prop. 15). En outre, si $j_\lambda$ est l’application canonique de $Y_\lambda$ dans $\hat{Y}_\lambda$, et si $g_\lambda = j_\lambda \circ f_\lambda$, $\hat{X}$ s’identifie à l’adhérence dans $\prod_{\lambda \in L} \hat{Y}_\lambda$ de l’image de $X$ par l’application $x \mapsto (g_\lambda(x))$.

Soit $X'$ (resp. $Y'_\lambda$) l’espace uniforme séparé associé à $X$ (resp. $Y_\lambda$), et soit $f'_\lambda : X' \to Y'_\lambda$ l’application uniformément continue rendant commutatif le diagramme

$$
\begin{array}{ccc}
X & \xrightarrow{f_\lambda} & Y_\lambda \\
\downarrow & & \downarrow j_\lambda \\
X' & \xrightarrow{f'_\lambda} & Y'_\lambda
\end{array}
$$

où $i$ est l’application canonique.

La transitivité des structures uniformes initiales (II, p. 8, prop. 5) montre d’une part que $\mathcal{U}$ est la structure uniforme la moins fine rendant uniformément continues les applications $j_\lambda \circ f_\lambda : X \to Y'_\lambda$, et d’autre part que $\mathcal{U}$ est aussi l’image réciproque par $i$ de la structure uniforme $\mathcal{U}'$ la moins fine sur l’ensemble $X'$ rendant uniformément continues les $f'_\lambda$. Or $\mathcal{U}'$ est séparée, car si $x_1, x_2$ sont deux points de $X$ tels que $j_\lambda(f_\lambda(x_1)) = j_\lambda(f_\lambda(x_2))$ pour tout $\lambda \in L$, $(x_1, x_2)$ appartient à tous les entourages de $\mathcal{U}$, et par suite $i(x_1) = i(x_2)$. La prop. 17 (II, p. 25) montre donc que $\mathcal{U}'$ est la structure uniforme de l’espace séparé $X'$ associé à $X$.

Cela étant, $X'$ s’identifie par la bijection $x' \mapsto (f'_\lambda(x'))$ à un sous-espace uniforme de l’espace uniforme produit $\prod_\lambda Y'_\lambda$ (II, p. 11, prop. 8). Comme les $Y'_\lambda$ sont séparés, on peut identifier chacun des $Y'_\lambda$ à un sous-espace partout dense de son complété $\hat{Y}_\lambda$, donc $\prod_\lambda Y'_\lambda$ à un sous-espace partout dense de $\prod_\lambda \hat{Y}_\lambda$ (I, p. 27, prop. 7). Mais $\prod_\lambda \hat{Y}_\lambda$ est séparé et complet (II, p. 17, prop. 10); l’adhérence $\overline{X'}$ de $X'$ dans $\prod_\lambda \hat{Y}_\lambda$ est donc un sous-espace séparé et complet (II, p. 16, prop. 8), qui s’identifie par suite au séparé complété $\hat{X}$ de $X$, les applications $f'_\lambda$ s’identifiant aux projections sur les $\hat{X}_\lambda$; d’où la proposition.

#### Corollaire 1 {#top-ii-s3-prop-18-cor-1 .statement}

Soient $X$ un espace uniforme, $i$ l’application canonique de $X$ dans son séparé complété $\hat{X}$; si $A$ est un sous-espace de $X$, $j : A \to X$ l’injection canonique, alors $\hat{j} : \hat{A} \to \hat{X}$ est un isomorphisme de $\hat{A}$ sur l’adhérence de $i(A)$ dans $\hat{X}$.

#### Corollaire 2 {#top-ii-s3-prop-18-cor-2 .statement}

Soit $(Y_\lambda)_{\lambda \in L}$ une famille d’espaces uniformes. Le séparé complété de l’espace produit $\prod_{\lambda \in L} Y_\lambda$ est canoniquement isomorphe au produit $\prod_{\lambda \in L} \hat{Y}_\lambda$.

## EXERCICES {#top-ii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
