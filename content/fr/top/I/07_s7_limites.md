---
book: top
book_title: General Topology
chapter: I
chapter_title: STRUCTURES TOPOLOGIQUES
section: 7
section_title: Limites
lang: fr
source: top-i-iv-fr
book_pages: TG I.46-TG I.51, TG I.99-TG I.100
pdf_pages: 0058-0063, 0111-0112
extraction: ocr
subsections:
    - "no": 1
      title: Limite d’un filtre
      page: 46
      pdf_page: 58
    - "no": 2
      title: Point adhérent à une base de filtre
      page: 0
      pdf_page: 59
    - "no": 3
      title: Valeur limite et valeur d’adhérence d’une fonction
      page: 48
      pdf_page: 60
    - "no": 4
      title: Limites et continuité
      page: 49
      pdf_page: 61
    - "no": 5
      title: Limites relativement à un sous-espace
      page: 50
      pdf_page: 62
    - "no": 6
      title: Limites dans les espaces produits et les espaces quotients
      page: 51
      pdf_page: 63
statements: 21
exercises: 7
content_sha256: cfb7b68d0a94a5786dfb0d7f7800cab6f6dec47b1b9010ba7043c5d6d12a9484
---

## § 7. LIMITES

### 1. Limite d’un filtre

#### Définition 1 {#top-i-s7-def-1 .statement}

Soient $X$ un espace topologique, $\mathcal{F}$ un filtre sur $X$. On dit qu’un point $x \in X$ est point limite (ou simplement limite) de $\mathcal{F}$, si $\mathcal{F}$ est plus fin que le filtre $\mathcal{V}(x)$ des voisinages de $x$; on dit aussi alors que $\mathcal{F}$ converge (ou est convergent) vers $x$. On dit que $x$ est limite d’une base de filtre $\mathcal{B}$ sur $X$ (ou que $\mathcal{B}$ converge vers $x$) si le filtre de base $\mathcal{B}$ converge vers $x$.

Cette définition et la prop. 4 de I, p. 38, donnent le critère suivant:

#### Proposition 1 {#top-i-s7-prop-1 .statement}

Pour qu’une base de filtre $\mathcal{B}$ sur un espace topologique $X$ converge vers $x \in X$, il faut et il suffit que tout ensemble d’un système fondamental de voisinages de $x$ contienne un ensemble de $\mathcal{B}$.

En accord avec la terminologie introduite dans I, p. 3, on peut énoncer la prop. 1 de la façon suivante: pour que $\mathcal{B}$ converge vers $x$, il faut et il suffit qu’il existe des ensembles des $\mathcal{B}$ aussi voisins qu’on veut de $x$.

Si un filtre $\mathcal{F}$ converge vers $x$, tout filtre plus fin que $\mathcal{F}$ converge aussi vers $x$, en vertu de la déf. 1. De même, si on remplace la topologie de $X$ par une topologie moins fine, le filtre des voisinages de $x$ est remplacé par un filtre moins fin (I, p. 11, prop. 3), donc $\mathcal{F}$ converge encore vers $x$ pour cette nouvelle topologie.

De façon imagée, on peut donc dire que, plus une topologie est fine, moins il y a de filtres convergents pour cette topologie. En particulier, pour la topologie discrète, les seuls filtres convergents sont les filtres de voisinages, car ces derniers sont les ultrafiltres triviaux sur $X$ (I, p. 40).

Soit $\Phi$ un ensemble de filtres sur $X$, qui convergent tous vers un même point $x$; le filtre des voisinages $\mathcal{V}(x)$ est moins fin que tous les filtres de $\Phi$, donc aussi moins fin que le filtre intersection $\mathfrak{J}$ des filtres de $\Phi$; autrement dit, $\mathfrak{J}$ converge aussi vers $x$.

LIMITES

#### Proposition 2 {#top-i-s7-prop-2 .statement}

Pour qu’un filtre $\mathcal{F}$ sur un espace topologique $X$ converge vers un point $x$, il faut et il suffit que tout ultrafiltre plus fin que $\mathcal{F}$ converge vers $x$.

Cela résulte aussitôt de ce qui précède et de la prop. 7 de I, p. 39.

On notera qu’en général un filtre peut avoir plusieurs points limites distincts ; nous reviendrons sur cette question dans I, p. 52.

### 2. Point adhérent à une base de filtre

#### Définition 2 {#top-i-s7-def-2 .statement}

Dans un espace topologique $X$, on dit qu’un point $x$ est adhérent à une base de filtre $\mathcal{B}$ sur $X$, s’il est adhérent à tous les ensembles de $\mathcal{B}$.

Si $x$ est adhérent à une base de filtre $\mathcal{B}$, il est aussi adhérent à toute base de filtre équivalente à $\mathcal{B}$ en vertu de I, p. 38, corollaire, et en particulier au filtre de base $\mathcal{B}$.

#### Proposition 3 {#top-i-s7-prop-3 .statement}

Pour qu’un point $x$ soit adhérent à une base de filtre $\mathcal{B}$, il faut et il suffit que tout ensemble d’un système fondamental de voisinages de $x$ rencontre chacun des ensembles de $\mathcal{B}$.

Cela résulte immédiatement des définitions.

Cette proposition et le cor. 1 de I, p. 37 montrent que la propriété « $x$ est adhérent au filtre $\mathcal{F}$ » est équivalente à la propriété « il existe un filtre plus fin que $\mathcal{F}$ et que le filtre des voisinages de $x$ ». Autrement dit :
PROPOSITION 4. — Pour qu’un point $x$ soit adhérent à un filtre $\mathcal{F}$, il faut et il suffit qu’il existe un filtre plus fin que $\mathcal{F}$ et qui converge vers $x$.

En particulier, tout point limite d’un filtre $\mathcal{F}$ est un point adhérent à $\mathcal{F}$.

#### Corollaire {#top-i-s7-n2-cor-1 .statement}

Pour qu’un ultrafiltre $\mathcal{U}$ soit convergent vers un point $x$, il faut et il suffit que $x$ soit adhérent à $\mathcal{U}$.

Si $x$ est adhérent à un filtre $\mathcal{F}$, il est aussi adhérent à tout filtre moins fin que $\mathcal{F}$; de même, si on remplace la topologie de $X$ par une topologie moins fine, $x$ reste adhérent à $\mathcal{F}$ pour cette topologie.

L’ensemble des points adhérents à une base de filtre $\mathcal{B}$ sur $X$ est par définition l’ensemble $\bigcap_{M \in \mathcal{B}} \overline{M}$; d’où :

#### Proposition 5 {#top-i-s7-prop-5 .statement}

L’ensemble des points adhérents à une base de filtre sur un espace topologique $X$ est fermé dans $X$.

#### Proposition 6 {#top-i-s7-prop-6 .statement}

Soit $\mathcal{B}$ une base de filtre sur une partie $A$ d’un espace topologique $X$. Tout point adhérent à $\mathcal{B}$ dans $X$ appartient à $\overline{A}$. Inversement, tout point de $\overline{A}$ est limite dans $X$ d’un filtre sur $A$.

La première assertion est évidente. D’autre part, si $x \in \overline{A}$, la trace sur $A$ du filtre des voisinages de $x$ dans $X$ est un filtre sur $A$ qui converge évidemment vers $x$.

#### Remarque {#top-i-s7-n2-rem-1 .statement}

Un filtre sur un espace topologique n’a pas nécessairement de point adhérent (ni a fortiori de point limite) : par exemple, sur un espace discret infini, le filtre des complémentaires des parties finies n’a pas de point adhérent. Les espaces dans lesquels tout filtre admet un point adhérent jouent un rôle très important en Mathématique ; nous les étudierons au § 9.

### 3. Valeur limite et valeur d’adhérence d’une fonction

#### Définition 3 {#top-i-s7-def-3 .statement}

Soit f une application d’un ensemble X dans un espace topologique Y, et soit 𝔅 un filtre sur X ; on dit qu’un point y ∈ Y est valeur limite (ou simplement limite) de f suivant le filtre 𝔅 si la base de filtre f(𝔅) converge vers y. On dit que y est valeur d’adhérence de f suivant le filtre 𝔅 si y est un point adhérent à la base de filtre f(𝔅).

La relation « y est limite de f suivant le filtre 𝔅 » s’écrit aussi lim₃₈f = y, ou limₓ₃₈f(x) = y, ou même limₓf(x) = y lorsqu’aucune confusion n’en résulte.

De la déf. 3 et des prop. 1 (I, p. 46) et 3 (I, p. 47) on déduit les critères suivants :

#### Proposition 7 {#top-i-s7-prop-7 .statement}

Pour que y ∈ Y soit limite de f suivant le filtre 𝔅, il faut et il suffit que, pour tout voisinage V de y dans Y, il existe un ensemble M ∈ 𝔅 tel que f(M) ⊂ V (ou encore, que $f^{-1}(V) \in 𝔅$ pour tout voisinage V de y).

Pour que y soit valeur d’adhérence de f suivant 𝔅, il faut et il suffit que pour tout voisinage V de y et tout ensemble M ∈ 𝔅, il existe x ∈ M tel que f(x) ∈ V.

#### Exemple 1 {#top-i-s7-n3-exa-1 .statement}

Une suite de points $(x_n)_{n \in \mathbf{N}}$ d’un espace topologique X est une application $n \mapsto x_n$ de $\mathbf{N}$ dans X. On a souvent à considérer, en Analyse, la notion de valeur limite ou de valeur d’adhérence d’une telle application suivant le filtre de Fréchet (I, p. 36) sur $\mathbf{N}$; si y est limite de $n \mapsto x_n$ suivant le filtre de Fréchet, on dit que y est limite de la suite $(x_n)$ lorsque n croît indéfiniment (ou que $x_n$ tend vers y lorsque n croît indéfiniment) et l’on écrit $\lim_{n \to \infty} x_n = y$. On appelle de même valeur d’adhérence de la suite $(x_n)$ toute valeur d’adhérence de l’application $n \mapsto x_n$ suivant le filtre de Fréchet.

On peut encore dire que $y \in X$ est valeur limite (resp. valeur d’adhérence) d’une suite $(x_n)$ de points de X s’il est point limite du filtre élémentaire associé à $(x_n)$ (I, p. 42) (resp. point adhérent à ce filtre).

Pour que y soit limite d’une suite $(x_n)$ dans X, il faut et il suffit que, pour tout voisinage V de y dans X, tous les termes de la suite $(x_n)$ à l’exception d’un nombre fini appartiennent à V, autrement dit qu’il existe un entier $n_0$ tel que $x_n \in V$ pour $n \geq n_0$. De même pour que y soit valeur d’adhérence de la suite $(x_n)$, il faut et il suffit que pour tout voisinage V de y et tout entier $n_0$, il existe un entier $n \geq n_0$ tel que $x_n \in V$.

Il importe de distinguer soigneusement la notion de valeur d’adhérence d’une suite de celle de point adhérent à l’ensemble des points de la suite ; toute valeur d’adhérence est un point adhérent à l’ensemble des points de la suite, mais la réciproque est inexacte.

#### Exemple 2 {#top-i-s7-n3-exa-2 .statement}

Plus généralement, soit $f$ une application d’un ensemble filtrant $A$ dans un espace topologique $X$. Si $x \in X$ est valeur limite (resp. valeur d’adhérence) de $f$ suivant le filtre des sections de $A$ (I, p. 38), on dit que $x$ est limite (resp. valeur d’adhérence) de $f$ suivant l’ensemble filtrant $A$, et on écrit $x = \lim_{z \in A} f(z)$.

Si $y$ est valeur limite (resp. valeur d’adhérence) d’une application $f : X \to Y$ suivant un filtre $\mathcal{F}$ sur $X$, $y$ reste valeur limite (resp. valeur d’adhérence) de $f$ suivant $\mathcal{F}$ quand on remplace la topologie de $Y$ par une topologie moins fine.

De même, si $y$ est limite (resp. valeur d’adhérence) de $f$ suivant le filtre $\mathcal{F}$, $y$ est encore limite (resp. valeur d’adhérence) de $f$ suivant tout filtre plus fin (resp. moins fin) que $\mathcal{F}$.

#### Proposition 8 {#top-i-s7-prop-8 .statement}

Soit $f$ une application d’un ensemble $X$ dans un espace topologique $Y$; pour que $y \in Y$ soit valeur d’adhérence de $f$ suivant $\mathcal{F}$, il faut et il suffit qu’il existe sur $X$ un filtre $\mathcal{G}$ plus fin que $\mathcal{F}$ et tel que $y$ soit limite de $f$ suivant $\mathcal{G}$.

En effet, si $y$ est valeur d’adhérence de $f$ suivant $\mathcal{F}$, et si $\mathcal{V}$ est le filtre des voisinages de $y$, $f^{-1}(\mathcal{V})$ est une base de filtre sur $X$ puisque tout ensemble de $f^{-1}(\mathcal{V})$ rencontre tout ensemble de $\mathcal{F}$ (I, p. 41). Cette remarque montre en outre qu’il existe sur $X$ un filtre $\mathcal{G}$ plus fin que $\mathcal{F}$ et que le filtre de base $f^{-1}(\mathcal{V})$ (I, p. 37, cor. 1), donc $y$ est valeur limite de $f$ suivant $\mathcal{G}$.

Notons enfin que si $f$ est une application d’un ensemble $X$ dans un espace topologique $Y$, l’ensemble des valeurs d’adhérence de $f$ suivant un filtre $\mathcal{F}$ sur $X$ est fermé dans $Y$ (I, p. 47, prop. 5) (et éventuellement vide).

#### Remarque {#top-i-s7-n3-rem-1 .statement}

Si $y \in Y$ est limite (resp. valeur d’adhérence) d’une application $f : X \to Y$ suivant un filtre $\mathcal{F}$ sur $X$, $y$ est aussi limite (resp. valeur d’adhérence) de toute fonction $g : X \to Y$ ayant même germe suivant $\mathcal{F}$ (I, p. 44); on dit aussi que $y$ est limite (resp. valeur d’adhérence) du germe $\tilde{f}$ de $f$ suivant $\mathcal{F}$.

### 4. Limites et continuité

Soient $X, Y$ deux espaces topologiques, $f$ une application de $X$ dans $Y$, $\mathcal{V}$ le filtre des voisinages dans $X$ d’un point $a \in X$. Au lieu de dire que $y \in Y$ est limite de $f$ suivant le filtre $\mathcal{V}$ et d’écrire $y = \lim_{\mathcal{V}} f$, on utilise la notation particulière

$$
y = \lim_{x \to a} f(x)
$$

et on dit que $y$ est limite de $f$ au point $a$ ou que $f(x)$ tend vers $y$ lorsque $x$ tend vers $a$. De même, au lieu de dire que $y$ est valeur d’adhérence de $f$ suivant $\mathcal{V}$, on dit que $y$ est valeur d’adhérence de $f$ au point $a$.

Compte tenu de la définition de la continuité (I, p. 8, déf. 1), la prop. 7 de I, p. 48 montre que:
**Proposition 9.** — *Pour qu’une application f d’un espace topologique X dans un espace topologique Y soit continue en un point a ∈ X, il faut et il suffit que* $\lim_{x \to a} f(x) = f(a)$.

#### Corollaire 1 {#top-i-s7-prop-8-cor-1 .statement}

*Soient X, Y deux espaces topologiques, f une application de X dans Y. Supposons f continue en un point a ∈ X; alors, pour toute base de filtre B sur X qui converge vers a, la base de filtre f(B) converge vers f(a). Inversement, si, pour tout ultrafiltre U sur X qui converge vers a, la base d’ultrafiltre f(U) converge vers f(a), f est continue au point a.*

La première assertion est une conséquence immédiate de la prop. 9. Pour démontrer la seconde, supposons que f ne soit pas continue au point a; il existe alors un voisinage W de f(a) dans Y tel que $f^{-1}(W)$ n’appartienne pas au filtre $\mathcal{V}$ des voisinages de a dans X. Alors (I, p. 39, prop. 7) il existe un ultrafiltre U plus fin que $\mathcal{V}$ et ne contenant pas $f^{-1}(W)$, donc contenant son complémentaire $A = X - f^{-1}(W)$ (I, p. 39, prop. 5); comme $f(A) \cap W = \varnothing, f(U)$ ne converge pas vers $f(a)$.

#### Corollaire 2 {#top-i-s7-prop-8-cor-2 .statement}

*Soit g une application d’un ensemble Z dans un espace topologique X, admettant une limite a suivant un filtre $\mathcal{F}$ sur Z; si l’application f : X → Y est continue au point a, la fonction composée f ∘ g admet la limite f(a) suivant le filtre $\mathcal{F}$.*

### 5. Limites relativement à un sous-espace

Soient X, Y deux espaces topologiques, A une partie de X, a un point de X adhérent à A (mais n’appartenant pas nécessairement à A). Soit $\mathcal{F}$ la trace sur A du filtre des voisinages de a dans X. Si f est une application de A dans Y, au lieu de dire que $y \in Y$ est limite de f suivant $\mathcal{F}$ et d’écrire $y = \lim_{\mathcal{F}} f$, on écrit

$$
y = \lim_{x \to a, x \in A} f(x)
$$

et on dit que y est *limite de f au point a, relativement au sous-espace* A, ou que $f(x)$ tend vers y lorsque x tend vers a en restant dans A. On remarquera que l’on a alors $y \in \overline{f(A)}$.

Lorsque $A = \mathbf{C}\{a\}$, où a est un point non isolé de X, au lieu d’écrire $y = \lim_{x \to a, x \in A} f(x)$, on écrit aussi $y = \lim_{x \to a, x \neq a} f(x)$.

On a des définitions analogues pour les valeurs d’adhérence.

Si f est la restriction à A d’une application g : X → Y, on dit que g a une limite (resp. valeur d’adhérence) y, relativement à A, en un point $a \in \overline{A}$, si y est limite (resp. valeur d’adhérence) de f au point a, relativement à A.

Soient B une partie de A, $a \in X$ un point adhérent à B; si y est limite au point a, relativement à A, d’une application $f : A \to Y$, y est aussi limite de f au point a, relativement à B; la réciproque est inexacte. Mais si V est un voisinage dans X d’un point $a \in \overline{A}$, et si $f$ a une limite $y$ au point $a$, relativement à $V \cap A$, $y$ est encore limite de $f$ au point $a$, relativement à $A$.

Soit $a$ un point de $X$ non isolé, donc adhérent à $C\{a\}$. Pour qu’une application $f : X \to Y$ soit continue au point $a$, il faut et il suffit que l’on ait $f(a) = \lim_{x \to a, x \neq a} f(x)$, comme il résulte aussitôt des définitions.

### 6. Limites dans les espaces produits et les espaces quotients

#### Proposition 10 {#top-i-s7-prop-10 .statement}

Soient $X$ un ensemble, $(Y_i)_{i \in I}$ une famille d’espaces topologiques, et pour chaque $i \in I$, soit $f_i$ une application de $X$ dans $Y_i$. On munit $X$ de la topologie $\mathcal{T}$ la moins fine rendant continues les $f_i$. Pour qu’un filtre $\mathcal{F}$ sur $X$ converge vers $a \in X$, il faut et il suffit que pour tout $i \in I$, la base de filtre $f_i(\mathcal{F})$ converge vers $f_i(a)$ dans $Y_i$.

La condition est nécessaire puisque les $f_i$ sont continues (I, p. 50, cor. 1). Inversement, supposons-la vérifiée, et soit $V$ un voisinage ouvert de $a$ dans $X$. Par définition de $\mathcal{T}$ (I, p. 12, prop. 4), il existe une partie finie $J$ de $I$ et, pour chaque $i \in J$, une partie ouverte $U_i$ de $Y_i$, telle que $f_i(a) \in U_i$ pour $i \in J$ et que $V$ contienne l’ensemble $\bigcap_{i \in J} f_i^{-1}(U_i)$. L’hypothèse entraîne que $f_i^{-1}(U_i) \in \mathcal{F}$ (I, p. 48, prop. 7); comme $J$ est fini, $M = \bigcap_{i \in J} f_i^{-1}(U_i)$ appartient à $\mathcal{F}$, et on a $M \subset V$, ce qui achève la démonstration.

#### Corollaire 1 {#top-i-s7-prop-10-cor-1 .statement}

Pour qu’un filtre $\mathcal{F}$ sur un espace produit $X = \prod_{i \in I} X_i$ converge vers un point $x$, il faut et il suffit que, pour tout $i \in I$, la base de filtre $\operatorname{pr}_i(\mathcal{F})$ converge vers $\operatorname{pr}_i x$.

#### Corollaire 2 {#top-i-s7-prop-10-cor-2 .statement}

Soit $f = (f_i)$ une application d’un ensemble $X$ dans un espace produit $Y = \prod_{i \in I} Y_i$. Pour que $f$ ait une limite $y = (y_i)$ suivant un filtre $\mathcal{F}$ sur $X$, il faut et il suffit que, pour tout $i \in I$, $f_i$ ait pour limite $y_i$ suivant $\mathcal{F}$.

#### Proposition 11 {#top-i-s7-prop-11 .statement}

Soient $R$ une relation d’équivalence ouverte dans un espace topologique $X$, $\varphi$ l’application canonique $X \to X/R$. Pour tout $x \in X$ et toute base de filtre $\mathcal{B}'$ sur $X/R$ qui converge vers $\varphi(x)$, il existe une base de filtre $\mathcal{B}$ sur $X$ qui converge vers $x$ et est telle que $\varphi(\mathcal{B})$ soit équivalente à $\mathcal{B}'$.

En effet, pour tout voisinage $U$ de $x$ dans $X$, $\varphi(U)$ est un voisinage de $\varphi(x)$ dans $X/R$ (I, p. 33, prop. 5), donc il existe un ensemble $M' \in \mathcal{B}'$ tel que $M' \subset \varphi(U)$; si on pose $M = U \cap \varphi^{-1}(M')$, on a $M' = \varphi(M)$. Cela montre que lorsque $M'$ parcourt $\mathcal{B}'$ et $U$ le filtre des voisinages de $x$, les ensembles $U \cap \varphi^{-1}(M')$ forment une base de filtre $\mathcal{B}$ sur $X$, qui converge évidemment vers $x$ et est telle que $\varphi(\mathcal{B})$ soit équivalente à $\mathcal{B}'$.

## EXERCICES {#top-i-s7-exercises}

See the [exercises for § 7](exercises/s7/).
