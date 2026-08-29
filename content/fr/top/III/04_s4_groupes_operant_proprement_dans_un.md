---
book: top
book_title: General Topology
chapter: III
chapter_title: GROUPES TOPOLOGIQUES
section: 4
section_title: Groupes opérant proprement dans un espace topologique. Compacité dans les groupes topologiques et les espaces à opérateurs
lang: fr
source: top-i-iv-fr
book_pages: TG III.27-TG III.36, TG III.74-TG III.78
pdf_pages: 0210-0219, 0257-0261
extraction: ocr
subsections:
    - "no": 1
      title: Groupes opérant proprement dans un espace topologique
      page: 27
      pdf_page: 210
    - "no": 2
      title: Propriétés des groupes opérant proprement
      page: 29
      pdf_page: 212
    - "no": 3
      title: Groupes opérant librement dans un espace topologique
      page: 30
      pdf_page: 213
    - "no": 4
      title: Groupes localement compacts opérant proprement
      page: 31
      pdf_page: 214
    - "no": 5
      title: Groupes opérant continûment dans un espace localement compact
      page: 33
      pdf_page: 216
    - "no": 6
      title: Espaces homogènes localement compacts
      page: 35
      pdf_page: 218
statements: 33
exercises: 25
content_sha256: 8f8e406c4f43a7ad7c78f10282c1fa4ef54b3c6d5a8681180780e2f6a40e23d2
---

## § 4. GROUPES OPÉRANT PROPREMENT DANS UN ESPACE TOPOLOGIQUE. COMPACITÉ DANS LES GROUPES TOPOLOGIQUES ET LES ESPACES À OPÉRATEURS

### 1. Groupes opérant proprement dans un espace topologique

#### Définition 1 {#top-iii-s4-def-1 .statement}

Soit $G$ un groupe topologique opérant continûment dans un espace topologique $E$. On dit que $G$ opère proprement dans $E$ si l’application $\theta : (s, x) \mapsto (x, s.x)$ de $G \times E$ dans $E \times E$ est propre (I, p. 72, déf. 1).

Soit $\Gamma \subset G \times E \times E$ le graphe de l’application $\rho : (s, x) \mapsto s.x$; puisque $\rho$ est continue, l’application $\sigma : (s, x) \mapsto (s, x, s.x)$ est un homéomorphisme de $G \times E$ sur $\Gamma$; l’application composée $G \times E \xrightarrow{\sigma} \Gamma \xrightarrow{\mathrm{pr}_{23}} E \times E$ n’est autre que $\theta$. La déf. 1 revient donc à dire que la restriction de $\mathrm{pr}_{23}$ à $\Gamma$ est une application propre de $\Gamma$ dans $E \times E$.

Le th. 1 de I, p. 75, montre que $G$ opère proprement dans $E$ si et seulement si la condition suivante est vérifiée:

Pour tout ensemble $A$ filtré par un ultrafiltre $\mathfrak{F}$ et toute application $\alpha \mapsto (s_\alpha, x_\alpha)$ de $A$ dans $G \times E$, si l’application $\alpha \mapsto (s_\alpha.x_\alpha, x_\alpha)$ a une limite $(b, a)$ suivant $\mathfrak{F}$, alors $\alpha \mapsto s_\alpha$ a une limite $t \in G$ suivant $\mathfrak{F}$, telle que $t.a = b$.

#### Exemple 1 {#top-iii-s4-n1-exa-1 .statement}

Soit $H$ un sous-groupe fermé d’un groupe topologique $G$. Si $G$ opère proprement dans $E$, il en est de même de $H$, puisque $H \times E$ est fermé dans $G \times E$ (I, p. 74, cor. 1). Si l’on prend par exemple $E = G$, $G$ opérant dans lui-même par translation à gauche, l’application $\theta : G \times E \to E \times E$ est un homéomorphisme, donc est propre, et l’on voit donc que $H$ opère proprement dans $G$ par translation à gauche.

#### Exemple 2 {#top-iii-s4-n1-exa-2 .statement}

Si $G$ opère proprement dans $E$, il opère proprement dans tout sous-espace $E'$ de $E$ réunion d’orbites de points de $E$ (autrement dit, saturé pour la relation d’équivalence définie par $G$). En effet, l’image réciproque de $E' \times E'$ dans $G \times E$ est $G \times E'$, et il suffit d’appliquer la prop. 3 de I, p. 72.

#### Proposition 1 {#top-iii-s4-prop-1 .statement}

Soient G un groupe topologique opérant continûment dans un espace topologique E, K une partie quasi-compacte de G. L’application $\rho : (s, x) \mapsto s.x$ de $K \times E$ dans E est propre.

En effet, $\rho$ se factorise en $K \times E \xrightarrow{\alpha} K \times E \xrightarrow{\mathrm{pr}_2} E$, où $\alpha(s, x) = (s, s.x)$. L’application $\alpha$ est un homéomorphisme, car $\alpha^{-1}(s, y) = (s, s^{-1}.y)$ est continue; puisque K est quasi-compact, $\mathrm{pr}_2$ est propre (I, p. 77, cor. 5); donc $\rho$ est propre (I, p. 73, prop. 5).

#### Corollaire 1 {#top-iii-s4-prop-1-cor-1 .statement}

Si A est une partie fermée (resp. compacte) de E, alors K.A est fermé dans E (resp. compact si E est séparé). En particulier, si F est une partie fermée et K une partie quasi-compacte de G, KF est fermé dans G.

L’assertion relative aux parties fermées résulte de la prop. 1 et de ce qu’une application propre est fermée (I, p. 72, prop. 1); l’assertion relative aux parties compactes est triviale.

On notera que si L est une partie compacte de E, F une partie fermée de G, F.L n’est pas nécessairement fermé dans E (III, p. 72, exerc. 29; cf. III, p. 35, corollaire).

#### Corollaire 2 {#top-iii-s4-prop-1-cor-2 .statement}

Si K est un sous-groupe quasi-compact d’un groupe topologique G, la relation d’équivalence $x^{-1}y \in K$ est fermée, et l’application canonique $\varphi : G \to G/K$ est propre.

La première assertion résulte du cor. 1; la seconde résulte alors du I, p. 75, th. 1.

#### Corollaire 3 {#top-iii-s4-prop-1-cor-3 .statement}

Soient K un sous-groupe distingué quasi-compact d’un groupe topologique G, $\varphi$ l’application canonique $G \to G/K$. Pour tout sous-groupe fermé A de G, la bijection canonique de $A/(A \cap K)$ sur $\varphi(A)$ est un isomorphisme de groupes topologiques.

En effet, comme $x^{-1}y \in K$ est une relation d’équivalence fermée (cor. 2), le corollaire résulte de I, p. 32, prop. 4.

#### Proposition 2 {#top-iii-s4-prop-2 .statement}

Soit K un groupe compact opérant continûment dans un espace séparé E. Alors:

a) K opère proprement dans E.
b) L’application $(s, x) \mapsto s.x$ de $K \times E$ dans E est propre.
c) L’application canonique de E sur $E/K$ est propre.

En effet, b) résulte de la prop. 1. D’autre part, comme K est compact, $\mathrm{pr}_2 : (s, x) \mapsto x$ est propre (I, p. 77, cor. 5); donc, comme E est séparé, $(s, x) \mapsto (x, s.x)$ est propre (I, p. 74, cor. 3), ce qui prouve a). En vertu du cor. 1 de la prop. 1, l’application canonique $\varphi : E \to E/K$ est fermée; pour tout espace topologique Z, si on fait opérer trivialement K dans Z, K opère continûment dans $E \times Z$, donc l’application canonique $E \times Z \to (E \times Z)/K$ est fermée d’après ce qui précède; mais $(E \times Z)/K$ s’identifie canoniquement à $(E/K) \times Z$ (III, p. 10, lemme 2 et I, p. 34, cor. de la prop. 8). Donc l’application canonique $E \times Z \to (E \times Z)/K$ s’identifie à $\varphi \times \mathrm{Id}_Z$, et dire qu’elle est fermée pour tout Z signifie que $\varphi$ est propre.

#### Corollaire 1 {#top-iii-s4-prop-2-cor-1 .statement}

Les hypothèses étant celles de la prop. 2, pour que E soit compact (resp. localement compact), il faut et il suffit que E/K le soit.
Cela résulte de ce que l’application canonique E → E/K est propre, compte tenu de I, p. 79, corollaire.

#### Corollaire 2 {#top-iii-s4-prop-2-cor-2 .statement}

Soient G un groupe topologique séparé, K un sous-groupe compact de G. Pour que G soit compact (resp. localement compact) il faut et il suffit que G/K soit compact (resp. localement compact).
En effet, il suffit d’appliquer le cor. 1 à K opérant dans G par translation à droite.

### 2. Propriétés des groupes opérant proprement

#### Proposition 3 {#top-iii-s4-prop-3 .statement}

Si un groupe topologique G opère proprement dans un espace topologique E, l’espace des orbites E/G est séparé. Si de plus G est séparé, alors E est séparé.
Soit C ⊂ E × E le graphe de la relation d’équivalence R définie par G dans E; c’est l’image de G × E par l’application θ: (s, x) ↦ (x, s.x). Comme θ est propre, C est fermé dans E × E (I, p. 72, prop. 1). Comme la relation R est ouverte (III, p. 10, lemme 2), on en conclut que E/G est séparé (I, p. 55, prop. 8).
Supposons maintenant G séparé; l’application x ↦ (e, x) de E dans G × E est un homéomorphisme sur une partie fermée de G × E, donc est propre (I, p. 72, prop. 2); si on compose avec cette application l’application (s, x) ↦ (x, s.x) de G × E dans E × E, qui est propre par hypothèse, on obtient une application propre de E dans E × E (I, p. 73, prop. 5) qui n’est autre que l’application diagonale x ↦ (x, x); donc la diagonale de E × E est fermée (I, p. 72, prop. 1), ce qui démontre que E est séparé (I, p. 52, prop. 1).

#### Proposition 4 {#top-iii-s4-prop-4 .statement}

Soit G un groupe topologique opérant proprement dans un espace topologique E, et soit x un point de E. Désignons par G.x l’orbite de x, par K_x le stabilisateur de x. Alors:
a) L’application s ↦ s.x est une application propre de G dans E.
b) K_x est quasi-compact.
c) L’application canonique de G/K_x sur G.x est un homéomorphisme.
d) L’orbite G.x est fermée dans E.
L’image réciproque par θ: (s, x) ↦ (x, s.x) de {x} × E est G × {x}; la prop. 3 de I, p. 72, montre que la restriction de θ à G × {x} est une application propre de G × {x} dans {x} × E, d’où a). Comme K_x est l’image réciproque de x par s ↦ s.x, b) résulte de I, p. 75, th. 1. Le fait que l’application canonique G/K_x ↦ G.x soit un homéomorphisme et le fait que G.x soit fermé dans E sont conséquences de a) (I, p. 72, prop. 2 et p. 73, prop. 5 b)).

#### Proposition 5 {#top-iii-s4-prop-5 .statement}

Soit G (resp. G’) un groupe topologique opérant continûment dans un espace topologique E (resp. E'). Soient $\varphi$ un homomorphisme continu de G dans G', $\psi$ une application continue de E dans E' telles que $\varphi$ et $\psi$ soient compatibles (III, p. 10).

(i) Si $\varphi$ est surjectif, $\psi$ surjective et propre, et si G opère proprement dans E, alors G' opère proprement dans E'.

(ii) Si $\varphi$ est propre, si G' opère proprement dans E' et si E est séparé, alors le groupe G opère proprement dans E.

Pour démontrer (i), on considère le diagramme commutatif

$$
\begin{array}{ccc}
G \times E & \xrightarrow{\theta} & E \times E \\
\alpha \downarrow & & \downarrow \beta \\
G' \times E' & \xrightarrow{\theta'} & E' \times E'
\end{array}
$$

où $\alpha = \varphi \times \psi, \beta = \psi \times \psi$. Par hypothèse, $\theta$ est propre et il en est de même de $\beta$ (I, p. 73, prop. 4 a)); donc $\beta \circ \theta = \theta' \circ \alpha$ est propre (I, p. 73, prop. 5 a)); comme $\alpha$ est surjective, on en déduit que $\theta'$ est propre (I, p. 73, prop. 5 b)).

Pour démontrer (ii), considérons un ultrafiltre $\mathcal{U}$ sur $G \times E$, tel que $(s, x) \mapsto s.x$ et $(s, x) \mapsto x$ convergent suivant $\mathcal{U}$ vers $y_0$ et $x_0$ respectivement. On en conclut que $(s, x) \mapsto \varphi(s).\psi(x)$ et $(s, x) \mapsto \psi(x)$ convergent suivant $\mathcal{U}$. Puisque G' opère proprement dans E', cela entraîne (III, p. 27) que $(s, x) \mapsto \varphi(s)$ converge suivant $\mathcal{U}$ vers un point $s'_0 \in G'$; comme $\varphi$ est propre, on en conclut (I, p. 75, th. 1) que $(s, x) \mapsto s$ converge suivant $\mathcal{U}$ vers un point $s_0 \in G$. L’unicité de la limite dans E montre alors que $y_0 = s_0.x_0$, ce qui montre que G opère proprement dans E (I, p. 75, th. 1).

#### Corollaire {#top-iii-s4-n2-cor-1 .statement}

Soient G un groupe topologique, K un sous-groupe de G. Pour que G opère proprement dans $G/K$, il faut et il suffit que K soit quasi-compact.

La nécessité de la condition résulte de la prop. 4 b) de III, p. 29. Pour montrer que la condition est suffisante, observons d’abord que G opère proprement dans lui-même par translation à gauche (III, p. 27, Exemple 1) et d’autre part l’application canonique $\psi : G \to G/K$ est propre (III, p. 28, cor. 2). Il suffit alors d’appliquer la prop. 5, (i) en y faisant $G, \varphi = \mathrm{Id}_G, E = G, E' = G/K, \psi$ étant l’application canonique.

### 3. Groupes opérant librement dans un espace topologique

Rappelons la définition suivante (A, I, p. 54):

#### Définition 2 {#top-iii-s4-def-2 .statement}

Soit G un groupe opérant dans un ensemble E. On dit que G opère librement dans E si le stabilisateur de tout point de E est réduit à e, autrement dit si les relations $s.x = x, x \in E, s \in G$ entraînent $s = e$.

#### Exemple {#top-iii-s4-n3-exa-1 .statement}

Soit G un groupe et soit H un sous-groupe de G. Le groupe H opère librement par translations (à droite ou à gauche) dans G.

Soient G un groupe opérant librement dans un ensemble E, R la relation d’équivalence dans E définie par G, C ⊂ E × E le graphe de R. Si (x, y) ∈ C, il existe un s ∈ G tel que s.x = y ; de plus cet élément est unique, car si s.x = s'.x, on a s'⁻¹s.x = x, d’où s'⁻¹s = e, puisque G opère librement. Si l’on fait correspondre au couple (x, y) ∈ C l’unique élément s ∈ G tel que s.x = y, on définit une application φ : C → G, que nous appellerons l’application canonique de C dans G. Avec ces notations :

#### Proposition 6 {#top-iii-s4-prop-6 .statement}

Soit G un groupe topologique opérant continûment dans un espace topologique E. On suppose que G opère librement dans E. Alors, pour que G opère proprement, il faut et il suffit que l’on ait :
(FP) Le graphe C de la relation d’équivalence définie par G est fermé dans E × E, et l’application canonique φ : C → G est continue.

L’ensemble C est l’image de l’application θ : (s, x) ↦ (x, s.x) de G × E dans E × E. On sait (I, p. 72, prop. 2) que pour que θ soit propre, il faut et il suffit que C soit fermé dans E × E et que si on désigne par θ' l’application θ considérée comme application de G × E dans C, θ' soit un homéomorphisme. Or l’hypothèse entraîne que θ' est bijective et que son application réciproque est (x, y) ↦ (φ(x, y), x); pour que θ' soit un homéomorphisme, il faut et il suffit donc que φ soit continue.

### 4. Groupes localement compacts opérant proprement

#### Proposition 7 {#top-iii-s4-prop-7 .statement}

Soit G un groupe localement compact opérant continûment dans un espace séparé E. Pour que G opère proprement, il faut et il suffit que, pour tout couple de points x, y de E, il existe un voisinage V_x de x et un voisinage V_y de y tels que l’ensemble K des s ∈ G pour lesquels s.V_x ∩ V_y ≠ ∅ soit relativement compact dans G.

Soit F l’espace compact obtenu en adjoignant à G un point à l’infini ω et soit Γ le graphe de ρ : (s, x) ↦ s.x considéré comme partie de F × E × E; montrons que si la restriction à Γ de pr_{23} est propre, Γ est fermé dans F × E × E. En effet, l’hypothèse entraîne que l’application u : (t, s, x, y) ↦ (t, x, y) de F × Γ dans F × E × E est fermée. Si Γ' est l’ensemble des points (s, s) dans F × G pour s ∈ G, Γ' est fermé dans F × G, étant le graphe de l’injection canonique G → F (I, p. 53, cor. 2); l’intersection (Γ' × E × E) ∩ (F × Γ) est donc une partie fermée de F × Γ, et il est immédiat que son image par u est l’ensemble Γ considéré comme partie de F × E × E, d’où notre assertion. Or, on a ((ω) × E × E) ∩ Γ = ∅. Par définition de F, pour tout (x, y) ∈ E × E, il existe donc un voisinage W de (x, y) dans E × E et une partie compacte K de G tels que ((G − K) × W) ∩ Γ = ∅ ; comme on peut prendre pour W un voisinage de la forme V_x × V_y, où V_x et V_y sont des voisinages de x et y respectivement, la relation ((G − K) × W) ∩ Γ = ∅ se traduit par « s ∉ K entraîne s.V_x ∩ V_y = ∅ », et nous avons démontré la nécessité de la condition de l’énoncé. Inversement, supposons cette condition vérifiée; soit $A$ un ensemble filtré par un ultrafiltre $\mathcal{F}$ et soit $\alpha \mapsto (s_\alpha, x_\alpha)$ une application de $A$ dans $G \times E$ telle que $\lim_{\mathcal{F}} x_\alpha = x$, $\lim_{\mathcal{F}} s_\alpha \cdot x_\alpha = y$. Supposons que $K, V_x$ et $V_y$ vérifient la condition de l’énoncé. Par hypothèse, il existe un ensemble $M \in \mathcal{F}$ tel que pour $\alpha \in M$, on ait $x_\alpha \in V_x$ et $s_\alpha \cdot x_\alpha \in V_y$, donc $s_\alpha \in K$, ce qui prouve que $\alpha \mapsto s_\alpha$ converge suivant $\mathcal{F}$ et achève la démonstration.

Lorsque $G$ est compact, la condition de l’énoncé de la prop. 7 est trivialement vérifiée, et on retrouve ainsi la prop. 2 a) de III, p. 28.

La prop. 7 montre en particulier qu’un groupe discret $G$ opérant continûment dans un espace séparé $E$ opère proprement dans $E$ si et seulement si, pour tout couple $(x, y)$ de points de $E$, il existe un voisinage $V_x$ de $x$ et un voisinage $V_y$ de $y$ tels que l’ensemble des $s \in G$ pour lesquels $s \cdot V_x \cap V_y \neq \varnothing$ soit fini.

#### Proposition 8 {#top-iii-s4-prop-8 .statement}

*Soit $G$ un groupe discret opérant proprement dans un espace séparé $E$. Soit $x$ un point de $E$ et soit $K_x$ le stabilisateur de $x$.

a) *Le sous-groupe $K_x$ est fini*.

b) *Il existe un voisinage ouvert $U$ de $x$ dans $E$ possédant les propriétés suivantes*:
   (i) $U$ est stable *par* $K_x$;
   (ii) *la relation d’équivalence induite dans $U$ par la relation définie par $G$ est la relation définie par $K_x$*;
   (iii) *pour tout $s \in G - K_x$, on a $U \cap s \cdot U = \varnothing$*.

c) *L’application canonique $U/K_x \to E/G$ est un homéomorphisme de $U/K_x$ sur un voisinage ouvert de la classe de $x$ dans $E/G$*.

En vertu de la prop. 7, $K_x$ est fini. Pour construire un ensemble ouvert $U$ vérifiant les conditions requises, notons d’abord qu’il existe, d’après la prop. 7, un ensemble ouvert $U_0$ contenant $x$ et tel que l’ensemble $K$ des $s \in G$ pour lesquels $s \cdot U_0 \cap U_0 \neq \varnothing$ soit fini. On a évidemment $K_x \subset K$; soient $s_1, \ldots, s_n$ les éléments de $K - K_x$. Si l’on pose $x_i = s_i \cdot x$ ($1 \leq i \leq n$), on a $x_i \neq x$ pour tout $i$; puisque $E$ est séparé, il existe pour chaque indice $i$ un voisinage ouvert $V_i$ de $x$ et un voisinage ouvert $V'_i$ de $s_i \cdot x$ tels que $V_i \cap V'_i = \varnothing$; posons $U_i = V_i \cap s_i^{-1} \cdot V'_i$. Il est clair que $U_i$ est ouvert et contient $x$, et l’on a $U_i \cap s_i \cdot U_i \subset V_i \cap V'_i = \varnothing$. Soit $U' = U_0 \cap U_1 \cap \cdots \cap U_n$; $U'$ est ouvert, contient $x$ et est tel que $U' \cap s \cdot U' = \varnothing$ pour $s \notin K_x$; en posant $U = \bigcap_{t \in K_x} t \cdot U'$ on obtient un ensemble ouvert stable pour $K_x$, contenant $x$ et tel que $U \cap s \cdot U = \varnothing$ pour $s \notin K_x$; c’est l’ensemble ouvert cherché.

Le fait que l’application canonique $U/K_x \to E/G$ soit un homéomorphisme de $U/K_x$ sur un ensemble ouvert dans $E/G$ résulte de I, p. 32, prop. 4, puisque $U$ est ouvert et la relation d’équivalence définie par $G$ ouverte (III, p. 10, lemme 2).

#### Corollaire {#top-iii-s4-n4-cor-1 .statement}

*Si l’on suppose en outre que $K_x = \{ e \}$, le point $x$ possède un voisinage ouvert $U$ tel que $U \cap s \cdot U = \varnothing$ pour tout $s \neq e$ dans $G$, et que la restriction à $U$ de l’application canonique $E \to E/G$ soit un homéomorphisme de $U$ sur une partie ouverte de $E/G$.

### 5. Groupes opérant continûment dans un espace localement compact

#### Proposition 9 {#top-iii-s4-prop-9 .statement}

Soit $G$ un groupe topologique opérant continûment dans un espace localement compact $E$. Si $E/G$ est séparé, il est localement compact.

En effet, comme la relation d’équivalence dans $E$ définie par $G$ est ouverte (III, p. 10, lemme 2), la proposition résulte de I, p. 80, prop. 10.

#### Proposition 10 {#top-iii-s4-prop-10 .statement}

Soit $G$ un groupe topologique opérant continûment dans un espace localement compact $E$, et supposons $E/G$ séparé; soit $\varphi$ l’application canonique de $E$ sur $E/G$. Pour toute partie compacte $K'$ de $E/G$, il existe une partie compacte $K$ de $E$ telle que $\varphi(K) = K'$.

Comme la relation d’équivalence définie par $G$ est ouverte (III, p. 10, lemme 2), la proposition est un cas particulier de la prop. 10 de I, p. 80.

#### Proposition 11 {#top-iii-s4-prop-11 .statement}

Soit $G$ un groupe topologique séparé opérant proprement dans un espace non vide $E$. Si $E$ est compact (resp. localement compact), il en est de même de $G$ et de $E/G$.

Par hypothèse, l’application $\theta : (s, x) \mapsto (x, s.x)$ de $G \times E$ dans $E \times E$ est propre; si $E \times E$ est compact (resp. localement compact) le corollaire de I, p. 79 montre qu’il en est de même de $G \times E$, donc de $G$ puisque $E \neq \emptyset$. Comme $E/G$ est séparé (III, p. 29, prop. 3) on sait que si $E$ est compact (resp. localement compact), $E/G$ est compact (I, p. 78, prop. 8) (resp. localement compact (prop. 9)) (voir III, p. 72, exerc. 29).

Nous allons maintenant donner des critères permettant d’affirmer qu’un groupe topologique séparé $G$ opère proprement dans un espace localement compact $E$. Pour tout couple de parties $K, L$ de $E$, nous noterons $P(K, L)$ l’ensemble des $s \in G$ tels que $s.K \cap L \neq \emptyset$.

#### Théorème 1 {#top-iii-s4-thm-1 .statement}

Soit $G$ un groupe topologique séparé, opérant continûment dans un espace topologique $E$. Soient $K$ une partie compacte de $E$, $L$ une partie fermée de $E$. Alors:
a) L’ensemble $P(K, L)$ est fermé dans $G$.
b) Si $G$ opère proprement dans $E$, et si $L$ est compact, $P(K, L)$ est compact.
c) Réciproquement, si $E$ est localement compact, et si, pour tout couple de parties compactes $K, L$ de $E$, $P(K, L)$ est relativement compact dans $G$ (donc compact d’après a)), alors $G$ opère proprement dans $E$ (et si $E$ est non vide, $G$ est localement compact d’après la prop. 11).

L’application $(s, x) \mapsto s.x$ de $G \times K$ dans $E$ est continue; l’image réciproque $L'$ de $L$ par cette application est donc fermée. Comme $K$ est compact, la projection $\mathrm{pr}_1 : G \times K \to G$ est propre (I, p. 77, cor. 5) et l’image de $L'$ par $\mathrm{pr}_1$ est fermée (I, p. 72, prop. 1). Comme cette image est $P(K, L)$, ceci démontre a).

Démontrons b). Notons que E est séparé (III, p. 29, prop. 3). Par hypothèse l’application $\theta : (s, x) \mapsto (x, s.x)$ de $G \times E$ dans $E \times E$ est propre; comme $K \times L$ est compact, $\overline{\theta}(K \times L)$ est compact, E étant séparé (I, p. 77, prop. 6); la projection $P(K, L)$ de $\overline{\theta}(K \times L)$ dans $G$ est donc un ensemble compact.

Démontrons c). Comme $K \times L$ est fermé dans $E \times E$, $\overline{\theta}(K \times L)$ est une partie fermée de $P(K, L) \times K$, donc est un ensemble compact sous les hypothèses de c). Comme toute partie compacte de $E \times E$ est contenue dans un ensemble compact de la forme $K \times L$, on en conclut que l’image réciproque par $\theta$ d’une partie compacte quelconque de $E \times E$ est compacte, et puisque $E \times E$ est localement compact, ceci prouve que $\theta$ est propre (I, p. 77, prop. 7) (voir IV, p. 46, exerc. 4 c)).

#### Remarque {#top-iii-s4-n5-rem-1 .statement}

On a évidemment $P(K, L) \subset P(K \cup L, K \cup L)$; donc, pour que G opère proprement dans un espace localement compact E, il suffit que pour toute partie compacte K de E, l’ensemble $P(K, K)$ soit relativement compact dans G. En particulier, pour qu’un groupe discret G opère proprement dans un espace localement compact E, il faut et il suffit que, pour toute partie compacte K de E, l’ensemble des $s \in G$ tels que $s.K \cap K \neq \varnothing$ soit fini.

#### Exemple {#top-iii-s4-n5-exa-1 .statement}

*Soit X une variété analytique complexe, analytiquement isomorphe à une partie ouverte bornée de $\mathbf{C}^n$, et soit G le groupe des automorphismes analytiques de X; la topologie de la convergence compacte est compatible avec la structure de groupe de G, et on peut montrer que G opère proprement dans X. En particulier, tout sous-groupe discret de G opère proprement dans X.

Prenons par exemple pour X le demi-plan $\mathcal{J}(z) > 0$, analytiquement isomorphe à un disque ouvert dans $\mathbf{C}$; le groupe G est le groupe des transformations $z \mapsto (az + b)/(cz + d)$, avec $a, b, c, d$ réels et $ad - bc \neq 0$. Le sous-groupe H de G formé des transformations pour lesquelles $a, b, c, d$ sont entiers et $ad - bc = 1$, est un sous-groupe discret de G, appelé groupe modulaire. En vertu de ce qui précède, il opère proprement dans le demi-plan $\mathcal{J}(z) > 0$.*

#### Proposition 12 {#top-iii-s4-prop-12 .statement}

Soit G un groupe topologique séparé opérant continûment dans un espace topologique E. Soit K une partie compacte de E, et soit $\rho_K$ l’application $(s, x) \mapsto s.x$ de $G \times K$ dans E. Alors:
a) Si G opère proprement dans E, $\rho_K$ est une application propre.
b) Si E est localement compact, et si $\rho_K$ est propre pour toute partie compacte K de E, G opère proprement dans E.

L’application $\rho_K$ se factorise en $G \times K \xrightarrow{\theta_K} K \times E \xrightarrow{\mathrm{pr}_2} E$, où $\theta_K$ est la restriction à $G \times K$ de l’application $\theta : (s, x) \mapsto (x, s.x)$ de $G \times E$ dans $E \times E$. Comme $\overline{\theta}(K \times E) = G \times K$, $\theta_K$ est propre si $\theta$ l’est (I, p. 72, prop. 3). D’autre part, comme K est compact, la projection $\mathrm{pr}_2$ de $K \times E$ sur E est propre (I, p. 77, cor. 5) donc $\rho_K$ est propre (I, p. 73, prop. 5).

Supposons inversement que pour toute partie compacte K de E, $\rho_K$ soit propre; si L est une partie compacte de E, $\overline{\rho_K}(L)$ est une partie compacte de

G × K, dont la projection dans G est P(K, L); donc P(K, L) est compact, et si E est localement compact, on en conclut que G opère proprement dans G, en vertu du th. 1 de III, p. 33.

#### Corollaire {#top-iii-s4-n5-cor-1 .statement}

Soit G un groupe topologique séparé opérant proprement dans un espace topologique E. Pour toute partie compacte K de E et toute partie fermée F de G, F.K est une partie fermée de E.
    Cela résulte de la prop. 12 et de I, p. 72, prop. 1.

### 6. Espaces homogènes localement compacts

#### Proposition 13 {#top-iii-s4-prop-13 .statement}

Soient G un groupe localement compact, H un sous-groupe fermé de G. L’espace homogène G/H est localement compact et paracompact.
    Comme G/H est séparé (III, p. 12, prop. 13), il est localement compact en vertu de III, p. 33, prop. 9, appliquée à H opérant à droite dans G. Reste donc à montrer que G/H est paracompact. Soit V un voisinage compact symétrique de e dans G, et soit G_0 = V^\infty le sous-groupe de G engendré par V, qui est ouvert (III, p. 7, corollaire). Le groupe G_0 opère continûment dans G/H (III, p. 12, prop. 12); montrons que chacune des orbites G_0 . z (pour z ∈ G/H) est une partie ouverte de G/H, réunion dénombrable d’ensembles compacts; il en résultera que G/H est somme topologique des orbites distinctes G_0 . z, et par suite est paracompact (I, p. 70, th. 5). Le fait que G_0 . z soit ouvert dans G/H résulte de ce que G_0 est ouvert dans G, et la relation d’équivalence x^{-1}y ∈ H ouverte dans G (III, p. 10, lemme 2). D’autre part, G_0 . z est réunion des V^n . z (n ≥ 1), et comme V^n est compact dans G et G/H séparé, V^n . z est compact, ce qui achève la démonstration.

#### Proposition 14 {#top-iii-s4-prop-14 .statement}

Dans un groupe localement compact G, la composante neutre C est l’intersection des sous-groupes ouverts de G.
    Comme C est un sous-groupe distingué fermé de G (III, p. 8, prop. 8), G/C est un groupe localement compact (prop. 13) qui est totalement discontinu (I, p. 84, prop. 9). Comme l’image réciproque, par l’application canonique de G sur G/C, d’un sous-groupe ouvert de G/C, est un sous-groupe ouvert de G contenant C, on voit qu’on peut se borner à démontrer la proposition pour le groupe G/C; autrement dit, on est ramené au cas où G est totalement discontinu. On sait alors (II, p. 32, corollaire) que tout voisinage compact V de e contient un voisinage U de e, à la fois ouvert et fermé. Comme U est compact, et B = CU fermé, il existe un voisinage ouvert symétrique W de e tel que W ⊂ U et UW ∩ BW = ∅ (III, p. 20 et II, p. 31, prop. 4), et a fortiori UW ⊂ U. Par récurrence sur n, on en déduit W^n ⊂ U pour tout entier n > 0; le sous-groupe W^\infty = \bigcup_{n > 0} W^n de G engendré par W, qui est ouvert (III, p. 7, corollaire), est donc contenu dans U, ce qui démontre la proposition.

Nous avons en outre prouvé:

#### Corollaire 1 {#top-iii-s4-prop-14-cor-1 .statement}

Si G est un groupe localement compact totalement discontinu, tout voisinage de e dans G contient un sous-groupe ouvert de G.

#### Corollaire 2 {#top-iii-s4-prop-14-cor-2 .statement}

Un groupe localement compact qui est engendré par chacun des voisinages de l’élément neutre est connexe.

#### Corollaire 3 {#top-iii-s4-prop-14-cor-3 .statement}

Soient G un groupe localement compact, H un sous-groupe fermé de G, φ l’application canonique de G sur G/H. Les composantes connexes de G/H sont les adhérences des images par φ des composantes connexes de G.

Soit C la composante neutre de G. Les composantes connexes de G sont les ensembles sC, où s ∈ G (III, p. 8, prop. 8); il est clair que φ(sC) est connexe, donc aussi $\overline{\varphi(sC)}$ (I, p. 81, prop. 1). Mais $\varphi(sC) = \varphi(sCH)$ et comme sCH est saturé pour la relation d’équivalence définie par H, et que cette relation est ouverte (III, p. 10, lemme 2), on a $\overline{\varphi(sCH)} = \varphi(\overline{sCH}) = \varphi(s.\overline{CH})$ (I, p. 33, prop. 7).

Posons L = $\overline{CH}$; L est un sous-groupe fermé de G contenant C et H; pour prouver que les ensembles $\varphi(s.L) = s.\varphi(L)$ sont les composantes connexes de G/H, il suffit de montrer que l’espace quotient de G/H par la relation d’équivalence dont les ensembles s.φ(L) sont les classes est totalement discontinu. Or, cet espace quotient est homéomorphe à l’espace homogène G/L (I, p. 21, prop. 7); on est ainsi ramené à prouver que lorsque C ⊂ H, G/H est totalement discontinu. Comme G/H s’identifie alors à (G/C)/(H/C) (III, p. 15, prop. 22), on peut supposer que G est lui-même totalement discontinu. Tout voisinage de φ(e) dans G/H contient un voisinage de la forme φ(V), où V est un voisinage de e dans G, et par suite (cor. 1) il contient un voisinage de la forme φ(K), où K est un sous-groupe ouvert et compact de G; φ(K) est alors ouvert et fermé dans G/H, ce qui montre que la composante connexe de φ(e) dans G/H est réduite à ce point; par translation, il en est de même de la composante connexe de tout point de G/H, ce qui achève de démontrer le corollaire.

## EXERCICES {#top-iii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
