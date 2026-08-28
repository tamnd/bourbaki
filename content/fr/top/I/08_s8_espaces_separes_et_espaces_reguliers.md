---
book: top
book_title: General Topology
chapter: I
chapter_title: STRUCTURES TOPOLOGIQUES
section: 8
section_title: Espaces séparés et espaces réguliers
lang: fr
source: top-i-iv-fr
pdf_pages: 0064-0071, 0112-0117
extraction: ocr
subsections:
    - "no": 1
      title: Espaces séparés
      page: 0
      pdf_page: 64
    - "no": 2
      title: Sous-espaces et espaces produits d’espaces séparés
      page: 54
      pdf_page: 66
    - "no": 3
      title: Séparation d’un espace quotient
      page: 55
      pdf_page: 67
    - "no": 4
      title: Espaces réguliers
      page: 56
      pdf_page: 68
    - "no": 5
      title: Prolongement par continuité. Double limite
      page: 57
      pdf_page: 69
    - "no": 6
      title: Relations d’équivalence dans un espace régulier
      page: 58
      pdf_page: 70
statements: 28
exercises: 29
content_sha256: cce74d2df88a64d676300feacac6c04c83e3b53a68854d681394c7cf50a19e8d
---

## § 8. ESPACES SÉPARÉS ET ESPACES RÉGULIERS

### 1. Espaces séparés

#### Proposition 1 {#top-i-s8-prop-1 .statement}

Soit X un espace topologique. Les propositions suivantes sont équivalentes:

(H) Quels que soient les points distincts x, y de X, il existe un voisinage de x et un voisinage de y sans point commun.

(Hi) L’intersection des voisinages fermés d’un point quelconque de X est l’ensemble réduit à ce point.

(Hii) La diagonale Δ de l’espace produit X × X est un ensemble fermé.

(Hiii) Pour tout ensemble I, la diagonale Δ de l’espace produit Y = XI est fermée dans Y.

(Hiv) Un filtre sur X ne peut avoir plus d’un point limite.

(Hv) Si un filtre F sur X admet un point limite x, x est le seul point adhérent à F.

Nous démontrerons les implications

$$
H \Rightarrow Hi \Rightarrow Hv \Rightarrow Hiv \Rightarrow H
$$

et

$$
H \Rightarrow Hiii \Rightarrow Hii \Rightarrow H.
$$

(H) ⇒ (Hi): En effet, si x ≠ y, il y a alors un voisinage ouvert U de x et un voisinage ouvert V de y tels que U ∩ V = ∅ ; par suite y ∉ \overline{U}.

(Hi) ⇒ (Hv): Soit y ≠ x ; il y a un voisinage fermé V de x tel que y ∉ V, et par hypothèse il existe M ∈ F tel que M ⊂ V ; on en conclut que M ∩ CV = ∅ , et comme CV est un voisinage de y, y n’est pas adhérent à F.

(Hv) ⇒ (Hiv): C’est immédiat, puisque tout point limite d’un filtre est adhérent à ce filtre.

(Hiv) ⇒ (H): Si tout voisinage V de x et tout voisinage W de y se rencontrent, les ensembles V ∩ W forment une base de filtre, qui admet à la fois x et y comme points limites dans X. D’où la conclusion.

(H) ⇒ (Hiii): Soit x = (x_i) un point de XI n’appartenant pas à Δ. Il y a donc au moins deux indices λ, μ tels que x_λ ≠ x_μ. Soit V_λ (resp. V_μ) un voisinage de x_λ (resp. x_μ) dans X, tels que V_λ ∩ V_μ = ∅ ; alors l’ensemble

$$
W = V_λ \times V_μ \times \prod_{i \neq λ, μ} X_i
$$

(avec X_i = X pour i ≠ λ, μ) est un voisinage de x dans XI (I, p. 24) ne rencontrant pas Δ, ce qui prouve que Δ est fermé dans XI.

(Hiii) ⇒ (Hii): C’est évident.

(Hii) ⇒ (H): Si x ≠ y, le point (x, y) ∈ X × X n’appartient pas à la diagonale Δ, donc (I, p. 24) il existe un voisinage V de x et un voisinage W de y tels que (V × W) ∩ Δ = ∅ , ce qui signifie que V ∩ W = ∅ .

#### Définition 1 {#top-i-s8-def-1 .statement}

On dit qu’un espace topologique X qui vérifie les conditions de la prop. 1 est un espace séparé (ou un espace de Hausdorff); la topologie d’un tel espace est dite séparée (ou de Hausdorff).

L’axiome (H) est appelé axiome de Hausdorff.

#### Exemple {#top-i-s8-n1-exa-1 .statement}

Tout espace discret est séparé. La droite rationnelle $\mathbf{Q}$ est séparée, car si $x, y$ sont deux nombres rationnels tels que $x < y$, et $z$ un nombre rationnel tel que $x < z < y$, les voisinages respectifs $]\leftarrow, z[$ et $]z, \rightarrow[$ de $x$ et $y$ ne se rencontrent pas.
Un ensemble $X$ ayant au moins deux points et muni de la topologie la moins fine (I, p. 11) n’est pas un espace séparé.

Soit $f : X \to Y$ une application d’un ensemble $X$ dans un espace séparé $Y$; il résulte aussitôt de la prop. 1 que $f$ ne peut avoir qu’une seule limite suivant un filtre $\mathcal{F}$ sur $X$, et que si $f$ a une limite $y$ suivant $\mathcal{F}$, $y$ est la seule valeur d’adhérence de $f$ suivant $\mathcal{F}$.

#### Proposition 2 {#top-i-s8-prop-2 .statement}

Soient $f, g$ deux applications continues d’un espace topologique $X$ dans un espace séparé $Y$; alors l’ensemble des $x \in X$ tels que $f(x) = g(x)$ est fermé dans $X$.
En effet, cet ensemble est l’image réciproque de la diagonale de $Y \times Y$ par l’application $x \mapsto (f(x), g(x))$ de $X$ dans $Y \times Y$, qui est continue (I, p. 25, prop. 1); la conclusion résulte donc de (Hii) et de I, p. 9, th. 1.

#### Corollaire 1 (Principe de prolongement des identités) {#top-i-s8-prop-2-cor-1 .statement}

Soient $f, g$ deux applications continues d’un espace topologique $X$ dans un espace séparé $Y$. Si $f(x) = g(x)$ en tous les points d’une partie partout dense de $X$, on a $f = g$.

En d’autres termes, une application continue de $X$ dans $Y$ (séparé) est entièrement déterminée par ses valeurs aux points d’une partie partout dense de $X$.

#### Corollaire 2 {#top-i-s8-prop-2-cor-2 .statement}

Si $f$ est une application continue d’un espace topologique $X$ dans un espace séparé $Y$, le graphe de $f$ est fermé dans $X \times Y$.
En effet, ce graphe est l’ensemble des points $(x, y) \in X \times Y$ tels que $f(x) = y$, et les deux applications $(x, y) \mapsto y$ et $(x, y) \mapsto f(x)$ de $X \times Y$ dans $Y$ sont continues.

#### Proposition 3 {#top-i-s8-prop-3 .statement}

Dans un espace séparé $X$, soit $(x_i)_{1 \leq i \leq n}$ une famille finie de points distincts; il existe alors pour chaque indice $i$ un voisinage $V_i$ de $x_i$ dans $X$ tel que les $V_i$ ($1 \leq i \leq n$) soient deux à deux disjoints.
On raisonne par récurrence sur $n$, la proposition n’étant autre que l’axiome (H) pour $n = 2$. Soit donc $W_i$ ($1 \leq i \leq n - 1$) un voisinage de $x_i$ tel que les $W_i$ soient deux à deux disjoints. Pour $1 \leq i \leq n - 1$, il existe d’autre part un voisinage $T_i$ de $x_i$ et un voisinage $U_i$ de $x_n$ sans point commun. En prenant $V_i = W_i \cap T_i$ pour $1 \leq i \leq n - 1$ et $V_n = \bigcap_{i=1}^{n-1} U_i$, on répond à la question.

#### Corollaire {#top-i-s8-n1-cor-1 .statement}

Tout espace fini séparé est discret.

#### Proposition 4 {#top-i-s8-prop-4 .statement}

Dans un espace séparé, tout ensemble fini est fermé.

Il suffit en effet de remarquer que tout ensemble réduit à un point est fermé en vertu de l’axiome (H^i).

#### Proposition 5 {#top-i-s8-prop-5 .statement}

Si, pour tout couple de points distincts x, y d’un espace topologique X, il existe une application continue f de X dans un espace séparé X' telle que f(x) ≠ f(y), alors X est séparé.

En effet, soient V' et W' des voisinages disjoints de f(x) et f(y) respectivement dans X'; $f^{-1}(V')$ et $f^{-1}(W')$ sont des voisinages disjoints de x et y respectivement, d’où la conclusion.

#### Corollaire {#top-i-s8-n1-cor-2 .statement}

Toute topologie plus fine qu’une topologie séparée est séparée.

### 2. Sous-espaces et espaces produits d’espaces séparés

Un sous-espace A d’un espace séparé X est séparé : il suffit en effet d’appliquer la prop. 5 à l’injection canonique A → X.

Inversement :

#### Proposition 6 {#top-i-s8-prop-6 .statement}

Si, dans un espace topologique X, tout point possède un voisinage fermé qui soit un sous-espace séparé de X, X est séparé.

En effet, soit x un point de X, et soit V un voisinage fermé de x dans X qui soit un sous-espace séparé de X. Les voisinages fermés de x relativement à V ont pour intersection {x} par hypothèse (axiome (H^i)); comme ce sont des voisinages fermés de x dans X (I, p. 18), l’intersection de tous les voisinages fermés de x dans X est a fortiori réduite à x; donc X vérifie (H^i).

On peut donner des exemples d’espaces non séparés dans lesquels tout point admet un voisinage séparé (I, p. 101, exerc. 7).

#### Proposition 7 {#top-i-s8-prop-7 .statement}

Tout produit d’espaces séparés est séparé. Réciproquement, si un produit d’espaces non vides est séparé, chacun des espaces facteurs est séparé.

En effet, soit X = $\prod_{i \in I} X_i$ un produit d’espaces topologiques ; pour deux points distincts x, y de X, il existe i tel que pr_i x ≠ pr_i y, et la prop. 5 montre que X est séparé si les X_i le sont. Inversement, si X est séparé et les X_i non vides, chacun des X_i est homéomorphe à un sous-espace de X (I, p. 26, prop. 4), donc est séparé.

#### Corollaire 1 {#top-i-s8-prop-7-cor-1 .statement}

Soient X un ensemble, $(Y_i)_{i \in I}$ une famille d’espaces topologiques séparés, et pour chaque i ∈ I, soit f_i une application de X dans Y_i. On munit X de la topologie $\mathcal{T}$ la moins fine rendant continues les f_i. Pour que X soit séparé, il faut et il suffit que pour tout couple (x, y) de points distincts de X, il existe i ∈ I tel que f_i(x) ≠ f_i(y).

La condition est suffisante en vertu de la prop. 5 de I, p. 54. Inversement, pour prouver que la condition est nécessaire, on peut, en vertu de la prop. 7 de I, p. 54 et de la prop. 3 de I, p. 26, se ramener au cas où I est réduit à un seul élément, autrement dit au cas où $\mathcal{T}$ est l’image réciproque par $f : X \to Y$ d’une topologie séparée. Mais si $f(x) = f(y)$ pour deux points distincts $x, y$ de $X$, il est clair que tout ensemble ouvert (pour $\mathcal{T}$) qui contient $x$ contient aussi $y$, d’où notre assertion.

#### Corollaire 2 {#top-i-s8-prop-7-cor-2 .statement}

Soit $(X_\alpha, f_{\alpha\beta})$ un système projectif d’espaces topologiques. Si les $X_\alpha$ sont séparés, $X = \lim_{\leftarrow} X_\alpha$ est séparé et est un sous-espace fermé de $\prod_\alpha X_\alpha$.

La première assertion résulte aussitôt de ce que $X$ est un sous-espace de l’espace séparé $\prod_\alpha X_\alpha$ (I, p. 54, prop. 7). D’autre part, pour $\alpha \leq \beta$, soit $F_{\alpha\beta}$ la partie de $\prod_\alpha X_\alpha$ formée des $x$ tels que $\mathrm{pr}_\alpha x = f_{\alpha\beta}(\mathrm{pr}_\beta x)$; les $F_{\alpha\beta}$ sont fermés dans $\prod_\alpha X_\alpha$ (I, p. 53, prop. 2), donc aussi leur intersection $X$.

Il est immédiat que tout espace somme d’espaces séparés (I, p. 15, Exemple III) est séparé.

### 3. Séparation d’un espace quotient

Cherchons des conditions pour qu’un espace quotient $X/R$ soit séparé (auquel cas on dit que la relation d’équivalence $R$ est séparée). En premier lieu, si $X/R$ est séparé, les ensembles réduits à un point dans $X/R$ sont fermés (I, p. 54, prop. 4), donc toute classe d’équivalence suivant $R$ est fermée dans $X$. Cette condition nécessaire n’est pas suffisante; la définition des ensembles ouverts dans $X/R$ donne la condition nécessaire et suffisante suivante: pour que $X/R$ soit séparé, il faut et il suffit que deux classes d’équivalence distinctes dans $X$ soient respectivement contenues dans deux ensembles ouverts saturés sans point commun. Nous allons donner d’autres conditions plus maniables.

#### Proposition 8 {#top-i-s8-prop-8 .statement}

Pour qu’un espace quotient $X/R$ soit séparé, il est nécessaire que le graphe $C$ de $R$ soit fermé dans $X \times X$. Cette condition est suffisante lorsque la relation $R$ est ouverte.

Soit $\varphi : X \to X/R$ l’application canonique; $C$ est l’image réciproque par $\varphi \times \varphi : X \times X \to (X/R) \times (X/R)$ de la diagonale $\Delta$ de $(X/R) \times (X/R)$, donc la première assertion résulte de la continuité de $\varphi \times \varphi$, de $(\mathrm{H}^{ii})$ et de I, p. 9, th.1. Si $R$ est ouverte, $(X/R) \times (X/R)$ s’identifie à l’espace quotient $(X \times X)/(R \times R)$ (I, p. 34, cor. de la prop. 8), et $\Delta$ s’identifie donc à l’image canonique dans $(X \times X)/(R \times R)$ de l’ensemble $C$ saturé pour $R \times R$; d’où la seconde assertion.

Lorsque $R$ n’est pas ouverte, on peut donner des exemples où $C$ est fermé et $R$ non séparée (I, p. 101, exerc. 10 et I, p. 105, exerc. 28).

Pour démontrer que $X/R$ est séparé, on peut aussi faire usage de la prop. 5 de I, p. 54 : M et N étant deux classes d’équivalence distinctes suivant R il suffira de connaître une application continue $f$ d’une partie ouverte A de X, saturée pour R et contenant M et N, dans un espace séparé $X'$, de sorte que : 1° $f$ soit constante sur toute classe d’équivalence suivant R, contenue dans A ; 2° $f$ prenne des valeurs distinctes sur M et N. Comme $A/R_A$ peut être identifié à une partie ouverte de $X/R$ (I, p. 23, cor. 1), on pourra appliquer la prop. 5 de I, p. 54 à l’application $g : A/R \to X'$ deduite de $f$ par passage aux quotients, puisque cette application est continue (I, p. 21, prop. 6).

En particulier :

#### Proposition 9 {#top-i-s8-prop-9 .statement}

*Si $f$ est une application continue d’un espace topologique $X$ dans un espace séparé $X'$, et $R$ la relation d’équivalence $f(x) = f(y)$, l’espace quotient $X/R$ est séparé.*

#### Proposition 10 {#top-i-s8-prop-10 .statement}

*Si $X$ est un espace séparé, et s’il existe une section continue s de $X$ pour la relation $R$, $X/R$ est séparé et $s(X/R)$ est fermé dans $X$.*

En effet (I, p. 22) $X/R$ est homéomorphe au sous-espace $s(X/R)$ de $X$, qui est séparé. En outre $s(X/R)$ est l’ensemble des $x \in X$ tels que $s(\varphi(x)) = x$, où $\varphi : X \to X/R$ est l’application canonique ; la seconde assertion résulte donc de I, p. 53, prop. 2.

### 4. Espaces réguliers

#### Proposition 11 {#top-i-s8-prop-11 .statement}

*Dans un espace topologique $X$, les propriétés suivantes sont équivalentes :

(O_{III}) *L’ensemble des voisinages fermés d’un point quelconque de $X$ est un système fondamental de voisinages de ce point.*

(O’_{III}) *Pour toute partie fermée F de $X$ et tout point $x \notin F$, il existe un voisinage de $x$ et un voisinage de $F$ sans point commun.*

(O_{III}) $\Rightarrow$ (O’_{III}) : En effet, si F est fermé et $x \notin F$, il existe un voisinage fermé V de $x$ contenu dans le voisinage $\complement F$ de $x$; V et $\complement V$ sont alors des voisinages de $x$ et F respectivement, sans point commun.

(O’_{III}) $\Rightarrow$ (O_{III}) : En effet, si W est un voisinage ouvert d’un point $x \in X$, il existe alors un voisinage U de $x$ et un voisinage V de $\complement W$ sans point commun, ce qui montre que $\overline{U} \subset W$.

#### Définition 2 {#top-i-s8-def-2 .statement}

*On dit qu’un espace topologique est régulier s’il est séparé et vérifie l’axiome (O_{III}) ; sa topologie est alors dite régulière.*

Un espace discret est régulier. *Nous verrons au § 9 que tout espace localement compact (en particulier la droite numérique $\mathbf{R}$) est un espace régulier.*

#### Proposition 12 {#top-i-s8-prop-12 .statement}

*Tout sous-espace d’un espace régulier est régulier.*

En effet, soit A un sous-espace d’un espace régulier X. Comme X est séparé, A est séparé (I, p. 54) ; d’autre part, tout voisinage d’un point $x \in A$ par rapport à A est de la forme V ∩ A, où V est un voisinage de x dans X. Comme X est régulier, il existe un voisinage W de x dans X, fermé dans X et tel que W ⊂ V; W ∩ A est alors un voisinage de x dans A, fermé dans A et tel que W ∩ A ⊂ V ∩ A, d’où la proposition.

Inversement:

#### Proposition 13 {#top-i-s8-prop-13 .statement}

Si, dans un espace topologique X, tout point possède un voisinage fermé qui soit un sous-espace régulier de X, X est régulier.

En effet, X est séparé (I, p. 54, prop. 6). D’autre part, soit x un point quelconque de X et soit V un voisinage fermé de x dans X, qui soit un sous-espace régulier de X. Pour tout voisinage U de x dans X tel que U ⊂ V, U est un voisinage de x dans V, donc il existe par hypothèse un voisinage W de x dans V, fermé dans V et contenu dans U. Mais W est aussi un voisinage de x dans X puisque V est un voisinage de x dans X, et W est fermé dans X puisque V est fermé dans X.

#### Remarque 1 {#top-i-s8-n4-rem-1 .statement}

On peut donner des exemples d’espaces non séparés, dont tout point admet un voisinage régulier (I, p. 101, exerc. 7).
2) On peut donner des exemples d’espaces séparés non réguliers (I, p. 103, exerc. 20).
3) Une topologie plus fine qu’une topologie régulière n’est pas nécessairement régulière (I, p. 103, exerc. 20).

### 5. Prolongement par continuité. Double limite

#### Théorème 1 {#top-i-s8-thm-1 .statement}

Soient X un espace topologique, A une partie partout dense de X, f : A → Y une application de A dans un espace régulier Y. Pour qu’il existe une application continue $\tilde{f} : X \to Y$ prolongeant f, il faut et il suffit que pour tout $x \in X, f(y)$ tende vers une limite dans Y lorsque y tend vers x en restant dans A. Le prolongement continu $\tilde{f}$ de f à X est alors unique.

L’unicité de $\tilde{f}$ résulte du principe de prolongement des identités (I, p. 53, cor. 1). La nécessité de la condition est évidente, car si $\tilde{f}$ est continue dans X, on a, pour tout $x \in X, \tilde{f}(x) = \lim_{y \to x, y \in A} \tilde{f}(y) = \lim_{y \to x, y \in A} f(y)$ (I, p. 50). Inversement, supposons vérifiée la condition de l’énoncé et posons, pour tout $x \in X, \tilde{f}(x) = \lim_{y \to x, y \in A} f(y)$, élément bien déterminé de Y, puisque Y est séparé. Il reste à prouver que $\tilde{f}$ est continue en tout point $x \in X$. Soit $V'$ un voisinage fermé de $\tilde{f}(x)$ dans Y ; par hypothèse, il existe un voisinage V de x dans X, ouvert dans X et tel que $f(V \cap A) \subset V'$; comme V est un voisinage de chacun de ses points, pour tout $z \in V$, on a $\tilde{f}(z) = \lim_{y \to z, y \in V \cap A} f(y)$, ce qui entraîne $\tilde{f}(z) \in \overline{f(V \cap A)} \subset V'$, puisque $V'$ est fermé. La conclusion résulte donc de ce que les voisinages fermés de $f(x)$ forment un système fondamental de voisinages de $f(x)$ dans Y.

On dit que l’application $\tilde{f}$ s’obtient en prolongeant f par continuité à X.

On ne peut, dans l’énoncé du th. 1, remplacer l’hypothèse que Y est régulier par une condition moins restrictive, sans faire d’hypothèse supplémentaire sur X, A ou f (I, p. 102, exerc. 19).

#### Corollaire {#top-i-s8-n5-cor-1 .statement}

Soit $\mathfrak{F}_1 \times \mathfrak{F}_2$ le filtre produit (I, p. 42), sur un ensemble $X = X_1 \times X_2$, d’un filtre $\mathfrak{F}_1$ sur $X_1$ et d’un filtre $\mathfrak{F}_2$ sur $X_2$. Soit $f$ une application de $X$ dans un espace régulier $Y$. On suppose que:
a) $\lim_{\mathfrak{F}_1 \times \mathfrak{F}_2} f$ existe;
b) $\lim_{x_2, \mathfrak{F}_2} f(x_1, x_2) = g(x_1)$ existe quel que soit $x_1 \in X_1$.
Dans ces conditions, $\lim_{x_1, \mathfrak{F}_1} g(x_1)$ existe et est égale à $\lim_{\mathfrak{F}_1 \times \mathfrak{F}_2} f$.

Soit $X'_1 = X_1 \cup \{\omega_1\}$ (resp. $X'_2 = X_2 \cup \{\omega_2\}$) l’espace topologique associé au filtre $\mathfrak{F}_1$ (resp. $\mathfrak{F}_2$) (I, p. 40, Exemple). Dans l’espace produit $X' = X'_1 \times X'_2$, soit $X''$ la réunion des sous-espaces $X_1 \times X'_2$ et $\{(\omega_1, \omega_2)\}$; $X$ est évidemment un sous-espace partout dense de $X''$, et les hypothèses signifient que $f(y_1, y_2)$ tend vers une limite lorsque $(y_1, y_2)$ tend vers un point quelconque $(x_1, x_2)$ de $X''$ en restant dans $X$. L’existence du prolongement par continuité de $f$ à $X''$ résulte donc du th. 1. Comme en outre $(\omega_1, \omega_2)$ est adhérent dans $X''$ à l’ensemble $(X_1 \times \{\omega_2\})$, la conclusion du corollaire en résulte aussitôt (I, p. 50).

### 6. Relations d’équivalence dans un espace régulier

#### Proposition 14 {#top-i-s8-prop-14 .statement}

Soient $X$ un espace régulier, $R$ une relation d’équivalence fermée dans $X$; alors le graphe $C$ de $R$ dans $X \times X$ est fermé.

Soit $(a, b)$ un point de $X \times X$ adhérent à $C$, et soit $V$ (resp. $W$) un voisinage fermé de $a$ (resp. un voisinage de $b$) dans $X$; par hypothèse, il existe $(x, y) \in C \cap (V \times W)$. Comme $x \in V$, $y$ appartient au saturé $S$ de $V$ pour $R$; donc $W \cap S \neq \varnothing$ pour tout voisinage $W$ de $b$, et comme $S$ est fermé par hypothèse, on a $b \in S$. Soit alors $B$ le saturé de $\{b\}$ pour $R$; on a $V \cap B \neq \varnothing$ pour tout voisinage fermé $V$ de $a$; comme par hypothèse $B$ est fermé et $X$ régulier, on a $a \in B$, donc $(a, b) \in C$, ce qui achève la démonstration.

#### Corollaire {#top-i-s8-n6-cor-1 .statement}

Dans un espace régulier, toute relation d’équivalence à la fois ouverte et fermée est séparée.

Cela résulte de la prop. 14 et de I, p. 55, prop. 8.

#### Proposition 15 {#top-i-s8-prop-15 .statement}

Soient $X$ un espace régulier, $F$ une partie fermée non vide de $X$, $R$ la relation d’équivalence obtenue en identifiant entre eux tous les points de $F$ (autrement dit, la relation d’équivalence dont les classes sont $F$ et les ensembles $\{x\}$ pour $x \in CF$). Alors l’espace quotient $X/R$ est séparé.

En effet, soient $M$ et $N$ deux classes d’équivalence distinctes dans $X$. Si chacune d’elles se réduit à un point dans $CF$, il existe dans le sous-espace séparé $CF$ deux voisinage ouverts de $M$ et $N$ respectivement sans point commun, et ces voisinages sont des voisinages de $M$ et $N$ dans $X$, saturés pour $R$ et sans point commun. Si $M = F$ et $N = \{b\}$ où $b \notin F$, il existe par hypothèse un voisinage ouvert de $b$ et un voisinage ouvert de $F$ sans point commun, et ces voisinages sont saturés pour $R$, ce qui achève la démonstration.

On notera que l’espace quotient X/R n’est pas nécessairement régulier (IX, §4, exerc. 18).

## EXERCICES {#top-i-s8-exercises}

See the [exercises for § 8](exercises/s8/).
