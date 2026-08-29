---
book: top
book_title: General Topology
chapter: I
chapter_title: STRUCTURES TOPOLOGIQUES
section: 9
section_title: Espaces compacts et espaces localement compacts
lang: fr
source: top-i-iv-fr
book_pages: TG I.59-TG I.71
pdf_pages: 0071-0083, 0117-0123
extraction: ocr
subsections:
    - "no": 1
      title: Espaces quasi-compacts et espaces compacts
      page: 59
      pdf_page: 71
    - "no": 2
      title: Régularité d’un espace compact
      page: 60
      pdf_page: 72
    - "no": 3
      title: Ensembles quasi-compacts; ensembles compacts; ensembles relativement compacts
      page: 61
      pdf_page: 73
    - "no": 4
      title: Image d’un espace compact par une application continue
      page: 62
      pdf_page: 74
    - "no": 5
      title: Produit d’espaces compacts
      page: 63
      pdf_page: 75
    - "no": 6
      title: Limites projectives d’espaces compacts
      page: 64
      pdf_page: 76
    - "no": 7
      title: Espaces localement compacts
      page: 65
      pdf_page: 77
    - "no": 8
      title: Immersion d’un espace localement compact dans un espace compact
      page: 67
      pdf_page: 79
    - "no": 9
      title: Espaces localement compacts dénombrables à l’infini
      page: 68
      pdf_page: 80
    - "no": 10
      title: Espaces paracompacts
      page: 69
      pdf_page: 81
statements: 48
exercises: 31
content_sha256: 3860aec594aa68b86a44725b56f6eb22a136dac4a050301c0019ce468b15b289
---

## § 9. ESPACES COMPACTS ET ESPACES LOCALEMENT COMPACTS

### 1. Espaces quasi-compacts et espaces compacts

#### Définition 1 {#top-i-s9-def-1 .statement}

On dit qu’un espace topologique X est quasi-compact s’il vérifie l’axiome suivant:
(C) Tout filtre sur X possède au moins un point adhérent.
On dit qu’un espace topologique est compact s’il est quasi-compact et séparé.

On déduit aussitôt de cet axiome que si f est une application d’un ensemble Z dans une espace quasi-compact X, et F un filtre quelconque sur Z, f a au moins une valeur d’adhérence suivant F. En particulier, toute suite de points d’un espace compact a au moins une valeur d’adhérence, mais cette condition n’est pas équivalente à (C) (I, p. 106, exerc. 12).

Nous énoncerons trois axiomes équivalents à l’axiome (C):
(C’) Tout ultrafiltre sur X est convergent.
(C’) entraîne (C): car soit F un filtre sur X; il existe un ultrafiltre plus fin que F (I, p. 39, th. 1); comme cet ultrafiltre est convergent vers un point x, x est adhérent à F.
(C) entraîne (C’): car si un ultrafiltre a un point adhérent, il converge vers ce point (I, p. 47, corollaire).

Si f est une application d’un ensemble Z dans un espace quasi-compact X, et U un ultrafiltre sur Z, f a donc au moins une limite suivant U (I, p. 41, prop. 10).

(C'') Toute famille d’ensembles fermés dans X, dont l’intersection est vide, contient une sous-famille finie, dont l’intersection est vide.
(C) entraîne (C''): car soit G une famille d’ensembles fermés dans X dont l’intersection soit vide; si l’intersection d’une sous-famille finie quelconque de G n’était pas vide, G engendrerait un filtre (I, p. 37, prop. 1) qui aurait un point adhérent d’après (C). Mais ce point appartiendrait à tous les ensembles de G, ces derniers étant fermés; ce qui est contraire à l’hypothèse.
Inversement, la négation de (C) entraîne celle de (C''): car si F est un filtre sans point adhérent, les adhérences des ensembles de F forment une famille d’ensembles fermés contredisant (C'').
(C''') (axiome de Borel–Lebesgue). Tout recouvrement ouvert de X contient un recouvrement ouvert fini de X.
(C''') se déduit de (C'') par passage aux complémentaires, et lui est donc équivalent.

Si X est quasi-compact, tout recouvrement localement fini R de X est fini, car il existe alors en vertu de (C''') un recouvrement de X formé d’un nombre fini d’ensembles ouverts, dont chacun ne rencontre qu’un nombre fini d’ensembles de $\mathfrak{R}$.

#### Exemple 1 {#top-i-s9-n1-exa-1 .statement}

Tout espace *fini* est *quasi-compact* et plus généralement tout espace dans lequel il n’y a qu’un nombre fini d’ensembles ouverts est quasi-compact; pour qu’un espace fini soit compact, il faut et il suffit qu’il soit *discret*, puisqu’un espace fini séparé est discret (I, p. 53, corollaire). Réciproquement, *tout espace discret compact est fini*, car dans un tel espace tout ensemble réduit à un point est ouvert, donc l’espace est fini en vertu de (C''').

#### Exemple 2 {#top-i-s9-n1-exa-2 .statement}

Soit X un ensemble; munissons X de la topologie pour laquelle les parties fermées sont X et les parties *finies* de X (cet ensemble de parties vérifiant de façon évidente les axiomes (O_I') et (O_{II}') de I, p. 5). L’espace topologique X ainsi défini est *quasi-compact*; montrons en effet qu’il vérifie l’axiome (C''). Si $(F_\alpha)_{\alpha \in I}$ est une famille de parties fermées de X dont l’intersection est vide, il y a un $\alpha \in I$ tel que $F_\alpha$ soit fini; si $a_k$ ($1 \leq k \leq n$) sont ses éléments, il existe par hypothèse pour chaque indice $k$ un indice $\iota_k \in I$ tel que $a_k \notin F_{\iota_k}$; l’intersection des $F_{\iota_k}$ ($1 \leq k \leq n$) et de $F_\alpha$ est alors vide. Si X est infini, il n’est pas séparé.

#### Remarque {#top-i-s9-n1-rem-1 .statement}

Les espaces quasi-compacts non séparés sont surtout utiles dans les applications de la Topologie à la Géométrie algébrique, mais n’interviennent guère dans les autres théories mathématiques, où par contre les espaces compacts jouent un rôle prépondérant.

#### Théorème 1 {#top-i-s9-thm-1 .statement}

*Soit $\mathcal{F}$ un filtre sur un espace quasi-compact X, et soit A l’ensemble des points adhérents à $\mathcal{F}$. Tout voisinage de A appartient alors à $\mathcal{F}$.*

En effet, soit V un voisinage de A; raisonnons par l’absurde, en supposant que tout ensemble de $\mathcal{F}$ rencontre $\mathcal{G}V$. Les traces sur $\mathcal{G}V$ des ensembles de $\mathcal{F}$ forment alors une base d’un filtre $\mathcal{G}$ sur X; comme X est quasi-compact, $\mathcal{G}$ a au moins un point adhérent $y$, qui n’appartient pas à A, puisque le voisinage V de A a une intersection vide avec certains de ensembles de $\mathcal{G}$. Mais, comme $\mathcal{G}$ est *plus fin* que $\mathcal{F}$, $y$ est aussi adhérent à $\mathcal{F}$, ce qui est contraire à l’hypothèse.

#### Corollaire {#top-i-s9-n1-cor-1 .statement}

*Pour qu’un filtre sur un espace compact soit convergent il faut et il suffit qu’il ait un seul point adhérent.*

La condition est nécessaire en vertu de I, p. 52, prop. 1; elle est suffisante en vertu du th. 1.

### 2. Régularité d’un espace compact

#### Proposition 1 {#top-i-s9-prop-1 .statement}

*Soient X un espace compact, x un point de X. Pour qu’une base de filtre $\mathcal{B}$ formée de voisinages fermés de x soit un système fondamental de voisinages de x, il faut et il suffit que l’intersection des ensembles de $\mathcal{B}$ se réduise au point x.*

La condition est nécessaire puisque X est séparé (I, p. 52, prop. 1). Elle est suffisante, car elle signifie que x est le seul point adhérent à $\mathcal{B}$, donc $\mathcal{B}$ converge vers x d’après le cor. du th. 1.

#### Corollaire {#top-i-s9-n2-cor-1 .statement}

*Tout espace compact est régulier.*
En effet, il résulte de l’axiome (Hi) (I, p. 52, prop. 1) que la base de filtre formée de *tous* les voisinages fermés d’un point quelconque de l’espace satisfait à la condition de la prop. 1.

On notera que l’espace quasi-compact non séparé X de l’*Exemple* 2 de I, p. 60 ne vérifie pas l’axiome (O$_{\text{III}}$), car l’intersection de deux ensembles ouverts non vides dans cet espace n’est jamais vide.

### 3. Ensembles quasi-compacts; ensembles compacts; ensembles relativement compacts

#### Définition 2 {#top-i-s9-def-2 .statement}

*On dit qu’une partie* A *d’un espace topologique* X *est un ensemble quasi-compact* (resp. *compact*) *si le sous-espace* A *est quasi-compact* (resp. *compact*).

Pour qu’une partie A d’un espace topologique X soit un ensemble quasi-compact, il faut et il suffit que tout recouvrement de A par des ensembles *ouverts dans* X contienne un recouvrement *fini* de A, comme il résulte de l’axiome (C'"). Dans un espace *séparé*, les notions d’ensemble quasi-compact et d’ensemble compact coïncident, puisque tout sous-espace est séparé.

#### Exemple 1 {#top-i-s9-n3-exa-1 .statement}

Dans un espace topologique X, tout ensemble fini est quasi-compact; l’ensemble vide et tout ensemble réduit à un point sont compacts.
2) Dans un espace topologique X, soit $(x_n)_{n \in \mathbf{N}}$ une suite infinie de points qui *converge* vers un point a. L’ensemble A formé des $x_n$ ($n \in \mathbf{N}$) et de a est *quasi-compact*. En effet, si $(U_i)$ est un recouvrement de A par des ensembles ouverts de X, il existe un indice $\kappa$ tel que $a \in U_\kappa$; comme $U_\kappa$ est un voisinage de a, il n’existe qu’un nombre fini d’indices $n_k$ tels que $x_{n_k} \notin U_\kappa$; si, pour chaque indice $k$, $\iota_k$ est un indice tel que $x_{n_k} \in U_{\iota_k}$, $U_\kappa$ et les $U_{\iota_k}$ forment un recouvrement ouvert fini de A.

#### Proposition 2 {#top-i-s9-prop-2 .statement}

*Dans un espace quasi-compact* (resp. *compact*), *tout ensemble fermé est quasi-compact* (resp. *compact*).

Il suffit d’appliquer l’axiome (C''), en remarquant que si A est fermé dans un espace X, tout ensemble fermé dans A est fermé dans X.

#### Proposition 3 {#top-i-s9-prop-3 .statement}

*Soient* X *un espace séparé*, A *et* B *deux parties compactes de* X *sans point commun. Alors il existe un voisinage* V *de* A *et un voisinage* W *de* B *qui ne se rencontrent pas*.

Montrons d’abord que pour tout $x \in A$, il existe un voisinage T$(x)$ de x dans X et un voisinage U$(x)$ de B dans X qui ne se rencontrent pas. En effet, pour tout $y \in B$, il existe un voisinage T$(x, y)$ de x et un voisinage U$(x, y)$ de y qui ne se rencontrent pas; comme B est compact, il y a un nombre fini de points $y_j$ de B tels que les U$(x, y_j)$ forment un recouvrement de B. Il suffit de prendre pour U$(x)$ la réunion des U$(x, y_j)$ et pour T$(x)$ l’intersection des T$(x, y_j)$. Comme A est compact, il y a un nombre fini de points $x_i \in A$ tels que les T$(x_i)$ forment un recouvrement de A. On répond alors à la question en prenant pour V la réunion des T$(x_i)$ et pour W l’intersection des U$(x_i)$.

#### Proposition 4 {#top-i-s9-prop-4 .statement}

Dans un espace séparé, tout ensemble compact est fermé.

En effet, si A est une partie compacte d’un espace séparé X et x un point de $\mathcal{C}A$, il résulte de la prop. 3 qu’il y a un voisinage de x ne rencontrant pas A, puisque $\{x\}$ est fermé (I, p. 54, prop. 4); donc $\mathcal{C}A$ est ouvert.

#### Corollaire {#top-i-s9-n3-cor-1 .statement}

Dans un espace compact X, pour qu’un ensemble A soit compact, il faut et il suffit qu’il soit fermé dans X.

#### Proposition 5 {#top-i-s9-prop-5 .statement}

Dans un espace topologique, la réunion d’une famille finie d’ensembles quasi-compacts est un ensemble quasi-compact.

Il suffit de montrer que la réunion de deux ensembles quasi-compacts A, B dans un espace topologique X est quasi-compacte. Soit $\mathfrak{R}$ un recouvrement ouvert de $A \cup B$; c’est un recouvrement de A et un recouvrement de B, donc il contient un recouvrement fini $\mathfrak{R}_1$ de A et un recouvrement fini $\mathfrak{R}_2$ de B; $\mathfrak{R}_1 \cup \mathfrak{R}_2$ est donc un recouvrement fini de $A \cup B$ contenu dans $\mathfrak{R}$, d’où la proposition.

#### Définition 3 {#top-i-s9-def-3 .statement}

On dit qu’une partie A d’un espace topologique X est relativement quasi-compacte (resp. relativement compacte) dans X si A est contenue dans une partie quasi-compacte (resp. compacte) de X.

De façon abrégée, on dit aussi que A est un « ensemble relativement quasi-compact » (resp. « relativement compact ») lorsqu’il n’y a pas d’équivoque sur X. Dans un espace séparé, les notions d’ensemble relativement quasi-compact et d’ensemble relativement compact sont identiques.

#### Proposition 6 {#top-i-s9-prop-6 .statement}

Dans un espace séparé X, pour qu’un ensemble A soit relativement compact, il faut et il suffit que A soit compact.

C’est évidemment suffisant, et c’est nécessaire en vertu de la prop. 4 et de son corollaire.

#### Proposition 7 {#top-i-s9-prop-7 .statement}

Si A est un ensemble relativement quasi-compact dans un espace topologique X, toute base de filtre sur A possède au moins un point adhérent dans X.

En effet, si $A \subset K$, où K est une partie quasi-compacte de X, toute base de filtre sur A admet un point adhérent dans K.

La réciproque de cette proposition n’est valable que moyennant des conditions supplémentaires sur X (I, p. 109, exerc. 23).

#### Remarque {#top-i-s9-n3-rem-1 .statement}

Dans un espace non séparé, un ensemble compact n’est pas nécessairement fermé, et son adhérence n’est pas nécessairement quasi-compacte (I, p. 105, exerc. 5); l’intersection de deux ensembles compacts n’est pas nécessairement quasi-compacte (I, p. 105, exerc. 5); la réunion de deux ensembles compacts n’est pas nécessairement compacte (I, p. 105, exerc. 5).

### 4. Image d’un espace compact par une application continue

#### Théorème 2 {#top-i-s9-thm-2 .statement}

Si f est une application continue d’un espace quasi-compact X dans un espace topologique $X'$, l’ensemble $f(X)$ est quasi-compact.

En effet, soit $\mathfrak{R}$ un recouvrement de $f(X)$ par des ensembles ouverts de $X'$; $f^{-1}(\mathfrak{R})$ est un recouvrement ouvert de $X$ (I, p. 9, th. 1), donc il y a une partie finie $\mathcal{G}$ de $\mathfrak{R}$ telle que $f^{-1}(\mathcal{G})$ soit un recouvrement de $X$; mais alors $\mathcal{G}$ est un recouvrement de $f(X)$, d’où le théorème.

#### Corollaire 1 {#top-i-s9-thm-2-cor-1 .statement}

Soit $f$ une application continue d’un espace topologique $X$ dans un espace séparé $X'$; l’image par $f$ de tout ensemble quasi-compact (resp. relativement quasi-compact) dans $X$ est un ensemble compact (resp. relativement compact) dans $X'$.

#### Corollaire 2 {#top-i-s9-thm-2-cor-2 .statement}

Toute application continue $f$ d’un espace quasi-compact $X$ dans un espace séparé $X'$ est fermée; si en outre $f$ est bijective, $f$ est un homéomorphisme.
Cela résulte aussitôt du cor. 1 et de I, p. 62, prop. 4.

En particulier:
COROLLAIRE 3. — Une topologie séparée moins fine qu’une topologie d’espace quasi-compact lui est nécessairement identique.

#### Corollaire 4 {#top-i-s9-thm-2-cor-4 .statement}

Soient $X$ un espace topologique, $R$ une relation d’équivalence séparée dans $X$.
a) S’il existe dans $X$ un ensemble quasi-compact $K$ tel que toute classe d’équivalence suivant $R$ rencontre $K$, $X/R$ est compact et l’application canonique de $K/R_K$ sur $X/R$ est un homéomorphisme.
b) Si en outre toute classe suivant $R$ ne rencontre $K$ qu’en un seul point, $K$ est une section continue pour la relation $R$ (I, p. 22).
En effet, soit $f$ la restriction à $K$ de l’application canonique $X \to X/R$; comme $X/R$ est séparé, $X/R$ est compact (cor. 1) et $f$ est une application fermée (cor. 2), donc la bijection $K/R_K \to X/R$ associée à $f$ est un homéomorphisme (I, p. 32, prop. 3); ceci démontre l’assertion a); l’assertion b) en résulte aussitôt, puisqu’alors $K/R_K = K$.

### 5. Produit d’espaces compacts

#### Théorème 3 (Tychonoff) {#top-i-s9-thm-3 .statement}

Tout produit d’espaces quasi-compacts (resp. compacts) est quasi-compact (resp. compact). Réciproquement, si un produit d’espaces non vides est quasi-compact (resp. compact), chacun des espaces facteurs est quasi-compact (resp. compact).
Vu la caractérisation des espaces produits séparés (I, p. 54, prop. 7), tout revient à démontrer les assertions relatives aux espaces quasi-compacts. Si $X = \prod_{i \in I} X_i$ est quasi-compact et non vide, on a $X_i = \mathrm{pr}_i(X)$ pour tout $i$, donc $X_i$ est quasi-compact en vertu du th. 2 de I, p. 62. Inversement, supposons les $X_i$ quasi-compacts et soit $\mathcal{U}$ un ultrafiltre sur $X$; pour tout $i \in I$, $\mathrm{pr}_i(\mathcal{U})$ est une base d’ultrafiltre sur $X_i$ (I, p. 41, prop. 10), qui converge donc en vertu de l’axiome (C'); par suite $\mathcal{U}$ est convergent (I, p. 51, cor. 1), ce qui achève la démonstration.

#### Corollaire {#top-i-s9-n5-cor-1 .statement}

Pour qu’une partie d’un produit d’espaces topologiques soit relativement quasi-compacte, il faut et il suffit que chacune de ses projections soit relativement quasi-compacte dans l’espace facteur correspondant.

La condition est nécessaire d’après le th. 2 de I, p. 62. Elle est suffisante, car si A est une partie de $\prod_i X_i$ telle que pour tout $i$, $\mathrm{pr}_i(A)$ soit contenu dans une partie quasi-compacte $K_i$ de $X_i$, A est contenu dans la partie quasi-compacte $\prod_i K_i$ de $\prod_i X_i$.

### 6. Limites projectives d’espaces compacts

#### Proposition 8 {#top-i-s9-prop-8 .statement}

Soient $(X_\alpha, f_{\alpha\beta})$ un système projectif d’espaces compacts relatif à un ensemble d’indices filtrant I, tel que $f_{\alpha\alpha}$ soit l’application identique pour tout $\alpha \in I$, $X = \lim_{\leftarrow} X_\alpha$ sa limite projective, $f_\alpha$ l’application canonique $X \to X_\alpha$ (I, p. 28). Alors:

$1^\circ$ $X$ est compact, et pour tout $\alpha$, on a

(1)
$$
f_\alpha(X) = \bigcap_{\beta \geq \alpha} f_{\alpha\beta}(X_\beta).
$$

$2^\circ$ Si les $X_\alpha$ sont non vides, $X$ est non vide.

En effet, $X$ est un sous-espace fermé de $\prod_\alpha X_\alpha$ (I, p. 55, cor. 2), donc il est compact en vertu du th. 3 de I, p. 63 et de la prop. 2 de I, p. 61. Les autres assertions résultent de E, III, p. 58, th. 1 : en effet, on peut appliquer ce théorème en prenant pour $S_\alpha$ l’ensemble des parties fermées de $X_\alpha$; les conditions (i) et (ii) ne sont autres que les axiomes (O'_I) et (C'"); la propriété (iii) résulte de ce que $\{ x_\alpha \}$ est fermé et $f_{\alpha\beta}$ continue (I, p. 9, th. 1); enfin la propriété (iv) résulte du cor. 2 de I, p. 63.

#### Corollaire 1 {#top-i-s9-prop-8-cor-1 .statement}

Soit $(X_\alpha, f_{\alpha\beta})$ un système projectif d’espaces topologiques relatif à un ensemble d’indices filtrant, tel que, pour tout couple d’indices $\alpha, \beta$ tels que $\alpha \leq \beta$, et pour tout $x_\alpha \in X_\alpha, f_{\alpha\beta}^{-1}(x_\alpha)$ soit compact. Alors on a la relation (1) et, pour tout $x_\alpha \in X_\alpha, f_\alpha^{-1}(x_\alpha)$ est compact.

En effet, pour tout $x_\alpha \in \bigcap_{\beta \geq \alpha} f_{\alpha\beta}(X_\beta)$ et tout $\beta \geq \alpha$, posons $L_\beta = f_{\alpha\beta}^{-1}(x_\alpha)$. Pour $\alpha \leq \beta \leq \gamma$, on a $f_{\beta\gamma}(L_\gamma) \subset L_\beta$ et l’ensemble des $\beta \geq \alpha$ est cofinal à l’ensemble I. Il est immédiat que les $L_\beta$ ($\beta \geq \alpha$) forment un système projectif d’espaces topologiques (pour les restrictions des $f_{\beta\gamma}$), dont la limite projective L est homéomorphe à $f_\alpha^{-1}(x_\alpha)$. Comme les $L_\beta$ sont par hypothèse compacts et non vides, le corollaire résulte de la prop. 8.

#### Corollaire 2 {#top-i-s9-prop-8-cor-2 .statement}

Soient $(X_\alpha, f_{\alpha\beta}), (X'_\alpha, f'_{\alpha\beta})$ deux systèmes projectifs d’espaces topologiques relatifs au même ensemble d’indices filtrant $I$, et soit $(u_\alpha)$ un système projectif d’applications $u'_\alpha : X_\alpha \to X'_\alpha$. Posons $X = \lim \leftarrow X_\alpha, X' = \lim \leftarrow X'_\alpha, u = \lim \leftarrow u_\alpha$.

a) Si, pour un $x' = (x'_\alpha) \in X'$, $\bar{u}_\alpha^{-1}(x'_\alpha)$ est compact et non vide pour tout $\alpha \in I$, alors $-1$
$u(x')$ est compact et non vide.

b) Si les $X_\alpha$ sont compacts, les $X'_\alpha$ séparés et les $u_\alpha$ surjectives et continues, alors $u$ est surjective.

Posons $L_\alpha = \bar{u}_\alpha^{-1}(x'_\alpha)$; il est immédiat que les $L_\alpha$ forment un système projectif d’espaces topologiques (pour les restrictions des $f_{\alpha\beta}$) et que $-1$
$u(x') = L$ est limite projective des $L_\alpha$; l’assertion a) résulte donc de la prop. 8. L’assertion b) en est une conséquence immédiate, compte tenu de la prop. 2 de I, p. 61.

### 7. Espaces localement compacts

#### Définition 4 {#top-i-s9-def-4 .statement}

On dit qu’un espace topologique $X$ est localement compact s’il est séparé et si tout point de $X$ possède un voisinage compact.

Il est clair que tout espace compact est localement compact, mais la réciproque est inexacte; par exemple, tout espace discret est localement compact, mais non compact s’il est infini.

*Comme nous le verrons dans IV, p. 7, la droite numérique $\mathbf{R}$ est un espace localement compact, mais non compact.*

#### Proposition 9 {#top-i-s9-prop-9 .statement}

Tout espace localement compact est régulier.

En effet, tout point $x$ d’un espace localement compact $X$ possède un voisinage compact $V$; comme $X$ est séparé, $V$ est fermé (I, p. 62, prop. 4); d’autre part, $V$ est un sous-espace régulier (I, p. 61, corollaire), donc $X$ est régulier (I, p. 57, prop. 13).

#### Corollaire {#top-i-s9-n7-cor-1 .statement}

Dans un espace localement compact, tout point admet un système fondamental de voisinages compacts.

En effet, l’intersection d’un voisinage fermé de $x$ et d’un voisinage compact de $x$ est un voisinage compact de $x$ (I, p. 61, prop. 2).

On notera qu’il existe des espaces topologiques non séparés dans lesquels tout point a un système fondamental de voisinages compacts (I, p. 105, exerc. 5).

Le cor. de la prop. 9 se généralise comme suit:

#### Proposition 10 {#top-i-s9-prop-10 .statement}

Dans un espace localement compact $X$, tout ensemble compact $K$ admet un système fondamental de voisinages compacts.

En effet, soit $U$ un voisinage quelconque de $K$; pour tout $x \in K$, il existe un voisinage compact $W(x)$ de $x$ contenu dans $U$. Les intérieurs des ensembles $W(x)$ forment un recouvrement ouvert de $K$ lorsque $x$ parcourt $K$, donc il existe un nombre fini de points $x_i \in K$ ($1 \leq i \leq n$) tels que les intérieurs des $W(x_i)$ forment un recouvrement de $K$; la réunion $V$ des $W(x_i)$ est alors un voisinage compact de $K$ contenu dans $U$ (I, p. 62, prop. 5).

#### Proposition 11 {#top-i-s9-prop-11 .statement}

*Dans un espace localement compact $X$, soit $F$ un ensemble tel que pour toute partie compacte $K$ de $X$, $F \cap K$ soit compact; alors $F$ est fermé dans $X$.*
Compte tenu de la prop. 4 de I, p. 62, cela résulte de la prop. 3 a) de I, p. 18.

#### Proposition 12 {#top-i-s9-prop-12 .statement}

*Dans un espace séparé $X$, tout sous-espace localement compact $A$ est localement fermé.*
En effet, pour tout $x \in A$, il y a par hypothèse un voisinage $V$ de $x$ dans $X$ tel que $V \cap A$ soit compact, et par suite fermé dans $V$ (I, p. 62, prop. 4).

#### Proposition 13 {#top-i-s9-prop-13 .statement}

*Dans un espace localement compact $X$, tout sous-espace localement fermé est localement compact.*
En effet, supposons $A$ localement fermé dans $X$; pour tout $x \in A$ il existe un voisinage $U$ de $x$ dans $X$ tel que $U \cap A$ soit fermé dans $U$. Soit $V \subset U$ un voisinage compact de $x$ dans $X$; $V \cap A = (U \cap A) \cap V$ est fermé dans $V$, donc compact (I, p. 61, prop. 2), et comme c’est un voisinage de $x$ dans $A$, cela démontre la proposition (A étant évidemment séparé).

Le th. 1 (I, p. 60) et le cor. 2 de I, p. 63 ne s’étendent pas aux espaces localement compacts non compacts.

Par exemple, dans un espace discret infini, le filtre des ensembles contenant un point $x$ et dont le complémentaire est fini, admet le point $x$ comme seul point adhérent, mais ne converge pas vers $x$. Une application quelconque d’un espace discret infini $X$ dans un espace séparé $X'$ étant continue, l’image par cette application d’une partie quelconque de $X$ (qui est fermée dans $X$) ne sera pas en général une partie fermée de $X'$.

La proposition correspondant au th. 3 (I, p. 63) est la suivante:

#### Proposition 14 {#top-i-s9-prop-14 .statement}

a) *Soit $(X_t)_{t \in I}$ une famille d’espaces localement compacts, telle que $X_t$ soit compact sauf pour un nombre fini d’indices. Alors l’espace produit $X = \prod_{t \in I} X_t$ est localement compact.*
b) *Réciproquement, si le produit d’une famille $(X_t)_{t \in I}$ d’espaces topologiques non vides est localement compact, les $X_t$ sont compacts sauf pour un nombre fini d’indices, et les facteurs non compacts sont localement compacts.*
a) Soit $x = (x_t)$ un point de $X$; pour chacun des indices $t$ tels que $X_t$ soit localement compact et non compact, soit $V_t$ un voisinage compact de $x_t$ dans $X_t$; pour les autres indices $t$, posons $V_t = X_t$; alors $\prod_t V_t$ est un voisinage compact de $x$ dans $X$ (I, p. 63, th. 3). On sait par ailleurs (I, p. 54, prop. 7) que $X$ est séparé, donc $X$ est localement compact.

b) Si $X = \prod_{i \in I} X_i$ est localement compact et les $X_i$ non vides, chacun des $X_i$ est homéomorphe à un sous-espace fermé de $X$ (I, p. 26, prop. 4 et I, p. 27, corollaire). D’autre part, soit $a = (a_i)$ un point de $X$, $V$ un voisinage compact de $a$; comme on a $\mathrm{pr}_i V = X_i$ sauf pour un nombre fini d’indices $i$ (I, p. 24), il résulte de I, p. 63, cor. 1 que les $X_i$ sont compacts sauf pour un nombre fini d’indices.

### 8. Immersion d’un espace localement compact dans un espace compact

#### Théorème 4 (Alexandroff) {#top-i-s9-thm-4 .statement}

Pour tout espace localement compact $X$, il existe un espace compact $X'$ et un homéomorphisme $f$ de $X$ sur le complémentaire d’un point de $X'$. En outre, si $X'_1$ est un second espace compact tel qu’il existe un homéomorphisme $f_1$ de $X$ sur le complémentaire d’un point de $X'_1$, il existe un homéomorphisme et un seul $g$ de $X'$ sur $X'_1$ tel que $f_1 = g \circ f$.

Démontrons d’abord la seconde assertion, et soient $f(X) = X' - \{ \omega \}$, $f_1(X) = X'_1 - \{ \omega_1 \}$; si l’homéomorphisme $g$ existe, son unicité est évidente, car on doit avoir par définition $g(x') = f_1(f^{-1}(x'))$ pour $x' \neq \omega$ et par suite $g(\omega) = \omega_1$. Reste à montrer que la bijection $g : X' \to X'_1$ définie par ces formules est bi-continue, et comme $X'$ et $X'_1$ jouent le même rôle, il suffit de montrer que l’image par $g$ d’un voisinage d’un point $x' \in X'$ est un voisinage de $g(x')$ dans $X'_1$. Or, cela est évident par définition si $x' \neq \omega$; d’autre part, si $V'$ est un voisinage ouvert de $\omega$ dans $X'$, $X' - V' = K$ est fermé dans $X'$, donc compact (I, p. 61, prop. 2) et contenu dans $f(X)$, et par suite $g(K) = f_1(f^{-1}(K))$ est compact (I, p. 63, cor. 1). Il en résulte que $g(V') = X'_1 - g(K)$ est un voisinage ouvert de $\omega_1$ (I, p. 62, prop 4), ce qui achève de prouver que $g$ est un homéomorphisme.

Prouvons maintenant la première assertion du théorème. Soit $X'$ un ensemble somme de $X$ et d’un ensemble réduit à un élément $\omega$, $X$ étant identifié au complémentaire de $\{ \omega \}$ dans $X'$. Définissons sur $X'$ une topologie en prenant pour ensemble $\mathcal{O}$ des parties ouvertes de $X'$ l’ensemble formé des parties ouvertes de $X$ et des parties de la forme $(X - K) \cup \{ \omega \}$, où $K$ est une partie compacte de $X$. Comme toute intersection de parties compactes de $X$ est compacte (I, p. 61, prop. 2 et I, p. 62, 4) et que toute partie fermée d’un ensemble compact est compacte (I, p. 61, prop. 2), $\mathcal{O}$ vérifie l’axiome $(O_I)$; comme toute réunion finie de parties compactes de $X$ est compacte (I, p. 62, prop. 5), $\mathcal{O}$ vérifie aussi l’axiome $(O_{II})$. Puisque toute partie compacte de $X$ est fermée dans $X$ (I, p. 62, prop. 4), la topologie induite sur $X$ par celle de $X'$ est la topologie initialement donnée sur $X$. Pour établir la première assertion, il reste à prouver que $X'$ est compact. En premier lieu $X'$ est séparé: en effet, si $x, y$ sont deux points distincts de $X$, il existe dans $X$ deux voisinages ouverts $V, W$ de $x$ et $y$ respectivement qui sont sans point commun, et $V$ et $W$ sont aussi ouverts dans $X'$; d’autre part, pour tout $x \in X$, il existe dans $X$ un voisinage compact $K$ de $x$, qui est aussi un voisinage de $x$ dans

X', et U = (X - K) ∪ {ω} est alors un voisinage de ω dans X' tel que U ∩ K = ∅. Enfin X' est quasi-compact : soit en effet (U_λ)_{λ ∈ L} un recouvrement ouvert de X' ; il y a au moins un indice μ ∈ L tel que U_μ = (X - K_μ) ∪ {ω}, où K_μ est une partie compacte de X ; il y a donc une partie finie H de L telle que les U_λ pour λ ∈ H forment un recouvrement de K_μ ; posant J = H ∪ {μ}, (U_λ)_{λ ∈ J} est un recouvrement de X', ce qui achève de prouver que X' est compact.

C.Q.F.D.

On observera que si X est déjà compact, le point ω est isolé dans l’espace compact X', et X' est par suite somme (I, p. 15, Exemple III) de X et de l’espace {ω}.

Lorsqu’on a ainsi défini un espace compact X' à partir d’un espace localement compact X par adjonction d’un élément ω, on dit souvent que ω est le « point à l’infini » de X', et que X' résulte de X par adjonction d’un point à l’infini ; on dit aussi que X' est le compactifié d’Aleksandroff de l’espace localement compact X.

*Exemple. — Si on applique le th. d’Aleksandroff au plan numérique R², on obtient un espace compact, dont on peut définir comme suit un homéomorphisme sur la sphère S₂ d’équation x₁² + x₂² + x₃² = 1 dans l’espace R³ : au point ω qu’on a adjoint à R² (point à l’infini), on fait correspondre le point (0, 0, 1) de S₂ ; et à tout point (x₁, x₂) de R² on fait correspondre le point où la droite joignant les points (0, 0, 1) et (x₁, x₂, 0) recoupe S₂. Cet homéomorphisme est connu sous le nom de projection stéréographique (voir A, IX, § 10, exerc. 14 et VI, §2, N° 4).*

### 9. Espaces localement compacts dénombrables à l’infini

#### Définition 5 {#top-i-s9-def-5 .statement}

On dit qu’un espace localement compact X est dénombrable à l’infini s’il est réunion dénombrable d’ensembles compacts.

#### Exemple 1 {#top-i-s9-n9-exa-1 .statement}

Pour qu’un espace discret soit dénombrable à l’infini, il faut et il suffit qu’il soit dénombrable.
*2) La droite numérique R est un espace localement compact dénombrable à l’infini, car elle est réunion des intervalles compacts {−n, +n} pour n ∈ N.*

#### Remarque {#top-i-s9-n9-rem-1 .statement}

Un espace topologique séparé peut être réunion dénombrable de sous-espaces compacts sans être localement compact. *Il en est ainsi par exemple de l’espace de Hilbert muni de la topologie faible, comme nous le démontrerons plus tard (EVT, I, § 1, n° 6, th. 4).*

#### Proposition 15 {#top-i-s9-prop-15 .statement}

Si X est un espace localement compact dénombrable à l’infini, il existe une suite (U_n) d’ensembles ouverts relativement compacts dans X, formant un recouvrement de X et tels que $\overline{U}_n \subset U_{n+1}$ pour tout n.

En effet, X est réunion d’une suite (K_n) d’ensembles compacts. Soit U₁ un voisinage ouvert relativement compact de K₁ (I, p. 65, prop. 10) et définissons par récurrence U_n pour n > 1 comme un voisinage ouvert relativement compact de $\overline{U}_{n-1} \cup K_n$ (I, p. 62, prop. 5 et I, p. 65, prop. 10) ; il est clair que les U_n répondent à la question.

#### Corollaire 1 {#top-i-s9-prop-15-cor-1 .statement}

Avec les notations de la prop. 15, pour toute partie compacte K de X, il existe un entier n tel que K ⊂ U_n.

En effet, il y a un nombre fini des $U_k$ qui recouvrent K (axiome de Borel-Lebesgue).

#### Corollaire 2 {#top-i-s9-prop-15-cor-2 .statement}

Soient $X$ un espace localement compact, $X'$ l’espace compact obtenu en adjoignant à $X$ un point à l’infini $\omega$ (I, p. 68). Pour que $X$ soit dénombrable à l’infini, il faut et il suffit que, dans $X'$, le point $\omega$ possède un système fondamental dénombrable de voisinages.

La condition est suffisante puisque les complémentaires des voisinages ouverts de $\omega$ sont compacts dans $X$. Elle est nécessaire, car si les $U_n \subset X$ ont les propriétés énoncées dans la prop. 15, les voisinages $X' - \overline{U}_n$ de $\omega$ dans $X$ forment un système fondamental de voisinages de $\omega$ en vertu du cor. 1.

Il est clair que tout sous-espace fermé d’un espace localement compact dénombrable à l’infini est un espace localement compact dénombrable à l’infini. De même, tout produit fini d’espaces localement compacts dénombrables à l’infini est dénombrable à l’infini.

On notera par contre qu’un sous-espace ouvert d’un espace compact n’est pas nécessairement dénombrable à l’infini, comme le montre le th. d’Alexandroff (I, p. 67, th. 4).

### 10. Espaces paracompacts

#### Définition 6 {#top-i-s9-def-6 .statement}

Un espace topologique $X$ est dit paracompact s’il est séparé, et s’il vérifie l’axiome suivant:
(PC) Pour tout recouvrement ouvert $\mathcal{R}$ de $X$, il existe un recouvrement ouvert localement fini $\mathcal{R}'$ de $X$, plus fin que $\mathcal{R}$ (E, II, p. 27, déf. 5).

Il est clair que tout espace compact est paracompact. Tout espace discret $X$ est paracompact, car le recouvrement ouvert formé de tous les ensembles réduits à un point est localement fini et plus fin que tout recouvrement ouvert de $X$.

#### Proposition 16 {#top-i-s9-prop-16 .statement}

Dans un espace paracompact $X$, tout sous-espace fermé $F$ est paracompact.

En effet, $F$ est séparé; d’autre part, si $(V_t)$ est un recouvrement ouvert dans le sous-espace $F$, tout $V_t$ est de la forme $V_t = U_t \cap F$, où $U_t$ est ouvert dans $X$. Considérons le recouvrement ouvert $\mathcal{R}$ de $X$ formé de $CF$ et des $U_t$; il existe un recouvrement ouvert localement fini $\mathcal{R}'$ de $X$ plus fin que $\mathcal{R}$, et les traces sur $F$ des ensembles de $\mathcal{R}'$ forment un recouvrement ouvert localement fini de $F$, plus fin que le recouvrement donné $(V_t)$.

Par contre, un sous-espace ouvert d’un espace compact n’est pas nécessairement paracompact (I, p. 105, exerc. 12).

#### Proposition 17 {#top-i-s9-prop-17 .statement}

*Le produit d’un espace paracompact et d’un espace compact est paracompact.*

Soient $X$ un espace paracompact, $Y$ un espace compact, $\mathfrak{R}$ un recouvrement ouvert de $X \times Y$. Pour tout point $(x, y) \in X \times Y$, il existe un voisinage ouvert $V(x, y)$ de $x$ dans $X$ et un voisinage ouvert $W(x, y)$ de $y$ dans $Y$ tels que $V(x, y) \times W(x, y)$ soit contenu dans un ensemble de $\mathfrak{R}$. Pour tout $x \in X$, les $W(x, y)$, où $y$ parcourt $Y$, forment un recouvrement ouvert de $Y$, donc il existe un nombre fini de points $y_i$ ($1 \leq i \leq n(x)$) de $Y$ tels que les $W(x, y_i)$ forment un recouvrement ouvert de $Y$. Posons $U(x) = \bigcap_{i=1}^{n(x)} V(x, y_i)$; chacun des ensembles ouverts $U(x) \times W(x, y_i)$ est contenu dans un ensemble de $\mathfrak{R}$. Soit alors $(T_\iota)_{\iota \in I}$ un recouvrement ouvert localement fini de $X$ plus fin que le recouvrement formé par les $U(x)$ ($x \in X$). Pour tout $\iota \in I$, soit $x_\iota$ un point de $X$ tel que $T_\iota \subset U(x_\iota)$, et désignons par $S_{\iota, k}$ les ensembles $W(x_\iota, y_k)$ correspondant à ce point ($1 \leq k \leq n(x_\iota)$). Il est clair que les ensembles $T_\iota \times S_{\iota, k}$ ($\iota \in I, 1 \leq k \leq n(x_\iota)$ pour tout $\iota \in I$) forment un recouvrement ouvert de $X \times Y$, plus fin que $\mathfrak{R}$; montrons que ce recouvrement est localement fini. En effet, pour tout $(x, y) \in X \times Y$, il existe un voisinage $Q$ de $x$ ne rencontrant qu’un nombre fini d’ensembles $T_\iota$; *a fortiori* le voisinage $Q \times Y$ de $(x, y)$ ne rencontre qu’un nombre fini d’ensembles de la forme $T_\iota \times S_{\iota, k}$.

Par contre, le produit de deux espaces paracompacts n’est pas nécessairement paracompact (voir IX, §5, exerc. 15).

#### Proposition 18 {#top-i-s9-prop-18 .statement}

*Un espace $X$ somme* (I, p. 15, *Exemple III*) *d’une famille* $(X_\iota)_{\iota \in I}$ *d’espaces paracompacts est paracompact.*

Soit en effet $(V_\lambda)_{\lambda \in L}$ un recouvrement ouvert de $X$; le recouvrement formé des ensembles ouverts $X_\iota \cap V_\lambda$ est plus fin que $(V_\lambda)$; si pour chaque $\iota \in I$, $(U_{\iota, \mu})_{\mu \in M_\iota}$ est un recouvrement ouvert localement fini de $X_\iota$ plus fin que $(V_\lambda \cap X_\iota)_{\lambda \in L}$, le recouvrement ouvert de $X$ formé des $U_{\iota, \mu}$ ($\iota \in I, \mu \in M_\iota$ pour chaque $\iota \in I$) est localement fini et plus fin que $(V_\lambda)$.

#### Théorème 5 {#top-i-s9-thm-5 .statement}

*Pour qu’un espace localement compact $X$ soit paracompact il, faut et il suffit qu’il soit somme d’une famille d’espaces localement compacts dénombrables à l’infini.*

Montrons d’abord que la condition est nécessaire. Supposons $X$ paracompact, et pour tout $x \in X$, soit $V_x$ un voisinage ouvert relativement compact de $x$ dans $X$. Il existe par hypothèse un recouvrement ouvert localement fini $(U(\alpha))_{\alpha \in A}$ de $X$ plus fin que le recouvrement formé des $V_x$ (où $x \in X$); les $U(\alpha)$ sont donc relativement compacts. Toute partie compacte $K$ de $X$ ne rencontre qu’un nombre fini d’ensembles $U(\alpha)$: en effet, les ensembles $U(\alpha) \cap K$ non vides forment un recouvrement ouvert localement fini de l’espace compact $K$, donc ce recouvrement est nécessairement fini (I, p. 59). Cela étant, soit $R$ la relation suivante entre deux points $x, y$ de $X$: « il existe une suite finie $(\alpha_i)_{1 \leq i \leq n}$ d’indices dans $A$ telle que $x \in U(\alpha_1),\ y \in U(\alpha_n)$ et $U(\alpha_i) \cap U(\alpha_{i+1}) \neq \varnothing$ pour $1 \leq i \leq n - 1$. On vérifie aussitôt que $R$ est une *relation d’équivalence*; en outre, toute classe d’équivalence suivant $R$ est un ensemble *ouvert* dans $X$, comme il résulte aussitôt de la définition de $R$ et du fait que les $U(\alpha)$ sont ouverts. L’espace $X$ est donc *somme* des sous-espaces localement compacts (I, p. 66, prop. 13) formés des classes d’équivalence suivant $R$; tout revient à prouver que chacun de ces sous-espaces est réunion d’une sous-famille *dénombrable* de la famille $(U(\alpha))$.

Or, soit $x$ un point quelconque de $X$; définissons par récurrence sur $n$ une suite $(C_n)$ d’ensembles ouverts relativement compacts dans $X$, de la façon suivante: $C_1$ est la réunion des ensembles $U(\alpha)$ qui contiennent $x$, et pour tout $n > 1$, $C_n$ est la réunion des ensembles $U(\alpha)$ qui rencontrent $C_{n-1}$. Il est immédiat, par récurrence sur $n$, que chacun des $C_n$ est relativement compact et réunion d’un nombre *fini* d’ensembles $U(\alpha)$. Montrons alors que la classe de $x$ suivant $R$ est la *réunion* des $C_n$: en effet, si $(\alpha_i)_{1 \leq i \leq n}$ est une suite d’indices telle que $x \in U(\alpha_1)$ et $U(\alpha_i) \cap U(\alpha_{i+1}) \neq \varnothing$ pour $1 \leq i \leq n - 1$, on a, par récurrence sur $i$, $U(\alpha_i) \subset C_i$ pour $1 \leq i \leq n$, ce qui achève de démontrer la première partie du théorème.

Montrons maintenant que la condition de l’énoncé est *suffisante*. En vertu de la prop. 18, on peut se borner au cas où $X$ est *dénombrable à l’infini*. Soit $\mathcal{R} = (G_\lambda)_{\lambda \in L}$ un recouvrement ouvert quelconque de $X$. Soit d’autre part $(U_n)$ une suite d’ensembles ouverts relativement compacts de $X$ ayant les propriétés énoncées dans la prop. 15 de I, p. 68; nous désignerons par $K_n$ l’ensemble compact $\overline{U_n} - U_{n-1}$ (en convenant de poser $U_n = \varnothing$ pour $n \leq 0$). L’ensemble ouvert $U_{n+1} - \overline{U}_{n-2}$ est un voisinage de $K_n$ par construction; pour tout $x \in K_n$, il existe donc un voisinage $W_x$ de $x$ contenu dans un des ensembles $G_\lambda$ et contenu aussi dans $U_{n+1} - \overline{U}_{n-2}$. Comme $K_n$ est compact, il existe un nombre fini d’ensembles de la forme $W_x$ formant un recouvrement de $K_n$; soient $H_{ni}$ $(1 \leq i \leq p_n)$ ces ensembles. Il est clair que la famille $\mathcal{R}'$ des ensembles $H_{nt}$ $(n \geq 1,\ 1 \leq i \leq p_n$ pour tout n) est un recouvrement ouvert de $X$ plus fin que $\mathcal{R}$; montrons que $\mathcal{R}'$ est *localement fini*. Soient $z$ un point quelconque de $X$, $n$ le plus petit entier tel que $z \in U_n$; comme $z \notin U_{n-1}$ il existe un voisinage $T$ de $z$ contenu dans $U_n$ et ne rencontrant pas $\overline{U}_{n-2}$; par suite, $T$ ne peut rencontrer que les ensembles $H_{mi}$ pour lesquels $n - 2 \leq m \leq n + 1$, et ces derniers sont en nombre fini.

C.Q.F.D.

Au cours de la démonstration, nous avons en outre prouvé ce qui suit:
COROLLAIRE. — *Soit $X$ un espace localement compact et paracompact; pour tout recouvrement ouvert $\mathcal{R}$ de $X$, il existe un recouvrement ouvert localement fini $\mathcal{R}'$ de $X$ plus fin que $\mathcal{R}$ et formé d’ensembles relativement compacts. Si $X$ est dénombrable à l’infini, on peut en outre supposer que $\mathcal{R}'$ est dénombrable.*

## EXERCICES {#top-i-s9-exercises}

See the [exercises for § 9](exercises/s9/).
