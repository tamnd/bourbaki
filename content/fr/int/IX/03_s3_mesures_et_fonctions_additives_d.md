---
book: int
book_title: Integration
chapter: IX
chapter_title: MESURES SUR LES ESPACES TOPOLOGIQUES SÉPARÉS
section: 3
section_title: Mesures et fonctions additives d’ensemble
lang: fr
source: int-ix-fr
pdf_pages: 0040-0048, 0100-0104
extraction: ocr
subsections:
    - "no": 1
      title: Mesures et fonctions additives de compacts
      page: 0
      pdf_page: 41
    - "no": 2
      title: Fonctions d’ensemble intérieurement régulières
      page: 0
      pdf_page: 43
    - "no": 3
      title: Espaces radoniens
      page: 0
      pdf_page: 45
statements: 17
exercises: 18
content_sha256: 79962b3e97f40794f6e08612fe66145bf080ed2de4e4dcb997acfe88f292418b
---

## § 3. Mesures et fonctions additives d'ensemble

Dans ce paragraphe, on désignera respectivement par $\mathfrak{A}(T)$ et par $\mathfrak{B}(T)$ l'ensemble des parties compactes d'un espace topologique séparé $T$, et la tribu borélienne de $T$.

### 1. Mesures et fonctions additives de compacts

#### Théorème 1 {#int-ix-s3-thm-1 .statement}

Soient T un espace topologique, et I une application de $\mathfrak{K}(T)$ dans $\mathbf{R}_+$. Pour qu’il existe une mesure $\mu$ sur T telle que $I(K) = \mu^*(K)$ pour tout $K \in \mathfrak{K}(T)$, il faut et il suffit que I satisfasse aux conditions suivantes:

1) Si K et L sont des parties compactes de T telles que $K \subset L$, on a $I(K) \leq I(L)$ (« I est croissante »).

2) Si K et L sont des parties compactes de T, on a $I(K \cup L) \leq I(K) + I(L)$.

3) Si K et L sont des compacts disjoints de T, on a $I(K \cup L) = I(K) + I(L)$ (« I est additive »).

4) Pour toute famille filtrante décroissante $(K_\alpha)_{\alpha \in A}$ de parties compactes de T, on a $I(\bigcap_{\alpha \in A} K_\alpha) = \inf_{\alpha \in A} I(K_\alpha)$.

5) Pour tout $x \in T$, il existe un voisinage V de x tel que
$$
\sup_{\substack{K \in \mathfrak{K}(T) \\ K \subset V}} I(K) < +\infty \quad (\text{« I est localement bornée »}).
$$

La mesure $\mu$ est alors unique.

L’unicité de $\mu$ résulte du cor. de la prop. 2 du § 1, n° 2. Les conditions ci-dessus sont nécessaires, les trois premières de façon évidente, la dernière du fait que $\mu^*$ est un encombrement localement borné, et la condition 4) d’après le cor. de la prop. 5 du § 1, n° 6.

Pour montrer que ces conditions sont suffisantes, nous commencerons par traiter le cas où T est compact.

#### Lemme 1 {#int-ix-s3-lem-1 .statement}

Supposons que T soit compact, et posons $I(T) = l$. Pour tout $A \subset T$, posons
$$
J(A) = \sup_{\substack{K \in \mathfrak{K}(T) \\ K \subset A}} I(K)
$$
et soit $\Phi$ l’ensemble des $A \subset T$ tels que $J(A) + J(\complement A) = l$. L’ensemble $\Phi$ est alors un clan qui contient $\mathfrak{K}(T)$, et la fonction J sur $\Phi$ est croissante et additive.

Il est clair que J est une fonction d’ensemble croissante, qui prolonge I, et que l’on a $J(A) + J(\complement A) \leq l$ pour tout $A \subset T$.

Soient K et S deux ensembles compacts dans T ; nous allons montrer d’abord que l’on a:
$$
J(K \cap S) + J(\complement K \cap S) = J(S).
$$

En considérant les restrictions de I à $\mathfrak{K}(S)$ et de J à $\mathfrak{P}(S)$, on se ramène aussitôt au cas où $S = T$. Comme T est normal, K est l’intersection de la famille filtrante décroissante de ses voisinages compacts, et la condition 4) entraîne l’existence, pour tout $\varepsilon > 0$, d’un voisinage compact H de K tel que $I(H) \leq I(K) + \varepsilon$. Soit L l’adhérence de $T - H$; L est compact, on a $L \cap K = \varnothing$, et $H \cup L = T$, donc $l = I(H \cup L) \leq I(H) + I(L) \leq I(K) + I(L) + \varepsilon$ (condition 2)), d’où la relation $J(K) + J(\mathcal{C}K) \geq I(K) + I(L) \geq l - \varepsilon$. Comme $\varepsilon$ est arbitraire, on a $J(K) + J(\mathcal{C}K) = l$. Cela prouve la formule (2), ainsi que l’inclusion $\mathfrak{A}(T) \subset \Phi$.

Prouvons maintenant que $\Phi$ est un clan. Comme $\Phi$ est évidemment stable par passage au complémentaire, il suffit de montrer que si $A_1$ et $A_2$ désignent des éléments de $\Phi$, on a $A_1 \cup A_2 \in \Phi$, ou encore que l’on a

$$
J(A_1 \cup A_2) + J(\mathcal{C}(A_1 \cup A_2)) \geq l.
$$

Désignons par $\varepsilon$ un nombre $> 0$, et, pour $i = 1, 2$, soient $K_i$ un compact contenu dans $A_i$, $L_i$ un compact contenu dans $\mathcal{C}A_i$, tels que

$$
I(K_i) \geq J(A_i) - \varepsilon, \quad I(L_i) \geq J(\mathcal{C}A_i) - \varepsilon.
$$

Posons $M_1 = K_1 \cup L_1$; les relations $l = J(M_1) + J(\mathcal{C}M_1)$, $J(M_1) = I(K_1) + I(L_1) \geq J(A_1) + J(\mathcal{C}A_1) - 2\varepsilon = l - 2\varepsilon$, entraînent $J(\mathcal{C}M_1) \leq 2\varepsilon$. Alors, si $S$ est une partie compacte de $T$, la relation (2) (appliquée à $K = M_1$) entraîne $J(S) \leq J(M_1 \cap S) + 2\varepsilon$, d’où

$$
J(S) \leq J(K_1 \cap S) + J(L_1 \cap S) + 2\varepsilon.
$$

Ajoutons les inégalités obtenues en faisant $S = K_2$ et $S = L_2$ et tenons compte de l’inégalité $J(K_2) + J(L_2) \geq l - 2\varepsilon$, et du fait que $K_1 \cap K_2, L_1 \cap K_2$ et $K_1 \cap L_2$ sont trois compacts disjoints contenus dans $A_1 \cup A_2$. Il vient, en désignant par $C$ la réunion de ces trois compacts

$$
l - 2\varepsilon \leq J(K_2) + J(L_2) \leq J(C) + J(L_1 \cap L_2) + 4\varepsilon \\
\leq J(A_1 \cup A_2) + J(\mathcal{C}(A_1 \cup A_2)) + 4\varepsilon
$$

d’où aussitôt la formule (3) cherchée vu l’arbitraire de $\varepsilon$. Ceci étant acquis, les inégalités précédentes entraînent $J(C) \geq J(A_1 \cup A_2) - 6\varepsilon$; si $A_1$ et $A_2$ sont disjoints, $C$ est réunion de $K_1 \cap L_2 \subset A_1$ et de $K_2 \cap L_1 \subset A_2$, et on en déduit $J(A_1 \cup A_2) \leq J(A_1) + J(A_2)$. L’inégalité inverse étant évidente, $J$ est bien additive sur $\Phi$, et le lemme est établi.

Achevons la démonstration du théorème dans le cas où $T$ est compact. Soit $\mathscr{E}(\Phi)$ l’espace vectoriel des fonctions $\Phi$-étagées sur $T$ muni de la convergence uniforme (chap. IV, 2e éd., § 4, n° 9, déf. 4); nous désignerons encore par $J$ la forme linéaire positive sur $\mathscr{E}(\Phi)$ associée à la fonction additive $J$ (loc. cit., prop. 18). Comme $J(T) = l$, $J$ est continue et de norme $l$. Soit alors $\mathscr{H}$ l’adhérence de $\mathscr{E}(\Phi)$ pour la topologie de la convergence uniforme; on vérifie aussitôt que $J$ se prolonge par continuité en une forme linéaire *positive* sur $\mathscr{H}$, encore notée $J$. Comme $\mathscr{H}$ contient $\mathscr{C}(T)$ (loc. cit., n° 10, prop. 19) la restriction de $J$ à $\mathscr{C}(T)$ est une mesure positive $\mu$. Il nous reste à montrer que l’on a $\mu^\bullet(K) = I(K)$ pour toute partie compacte $K$ de $T$. Or nous avons $\mu^\bullet(K) = \inf_{f \in S_K} \mu^\bullet(f)$, où $S_K$ désigne l’ensemble des éléments de $\mathscr{C}(T)$ qui majorent $\varphi_K$ (§ 1, n° 6, prop. 5). Comme $J(f) = \mu^\bullet(f)$ pour $f \in \mathscr{C}(T)$, il suffit évidemment de montrer que $J(K) \geq \inf_{f \in S_K} J(f)$. Or soit $H$, comme dans la démonstration du lemme 1, un voisinage compact de K tel que $J(H) \leq J(K) + \varepsilon$, et soit $f$ une fonction continue dans T, comprise entre 0 et 1, égale à 1 sur K et à 0 hors de H ($Top. gén.$, chap. IX, 3e éd., § 4, n° 1, prop. 1). On a
$$
J(f) \leq J(H) \leq J(K) + \varepsilon;
$$
$\varepsilon$ étant arbitraire, l’inégalité demandée est prouvée, et le théorème est donc établi lorsque T est compact.

Passons maintenant au cas général. Pour tout ensemble compact L dans T, soit $I_L$ la restriction de I à $\mathfrak{A}(L)$. D’après le cas particulier qui vient d’être traité, il existe une mesure $\mu_L$ sur L, unique, telle que $\mu_L(K) = I_L(K)$ pour tout ensemble compact $K \subset L$. Soit alors $L'$ un compact contenu dans L; on a $(\mu_L)_{L'}(K) = \mu_{L'}(K) = \mu_{L'}(K)$ pour tout compact $K \subset L'$, donc $\mu_{L'} = (\mu_L)_{L'}$; l’application $\mu : L \mapsto \mu_L$ est une prémesure. La condition 5) exprime que $\mu$ est une mesure, et la relation $I(K) = \mu^*(K)$ pour tout compact $K \subset T$ est évidente.

#### Remarque 1 {#int-ix-s3-n1-rem-1 .statement}

La condition 4) peut être remplacée, dans l’énoncé du théorème 1, par la condition suivante (« continuité à droite »):
4') *Pour tout $K \in \mathfrak{A}(T)$ et tout $\varepsilon > 0$, il existe un ensemble ouvert U contenant K, tel que $I(H) \leq I(K) + \varepsilon$ pour tout compact $H \subset U$*.

Si $\mu$ est une mesure, la fonction $I : K \mapsto \mu^*(K)$ satisfait en effet à 4') ($§ 1$, n° 9, prop. 13). Inversement, supposons que I satisfasse à 1) et 4'); montrons que I satisfait alors à 4). Avec les notations de l’énoncé du théorème 1, choisissons $\varepsilon > 0$ et un ensemble ouvert U contenant l’ensemble compact $K = \bigcap_{\alpha \in A} K_\alpha$, et tels que 4') soit vérifiée. Il existe alors un indice $\beta \in A$ tel que $K_\beta \subset U$, et cela entraîne
$$
\inf_{\alpha \in A} I(K_\alpha) \leq I(K_\beta) \leq I(K) + \varepsilon
$$
et 4) est bien vérifiée.

#### Remarque 2 {#int-ix-s3-n1-rem-2 .statement}

L’ensemble des conditions 2) et 3) peut être remplacé, dans l’énoncé du th. 1, par la condition suivante:
*Si K et L sont des compacts de T, on a*
$$
I(K \cup L) + I(K \cap L) = I(K) + I(L).
$$
Cette condition entraîne en effet 2) et 3), et d’autre part, on a
$$
\mu^*(K \cup L) + \mu^*(K \cap L) = \mu^*(K) + \mu^*(L)
$$
pour toute mesure $\mu$, en vertu de la relation $\varphi_{K \cup L} + \varphi_{K \cap L} = \varphi_K + \varphi_L$ entre les fonctions caractéristiques.

### 2. Fonctions d’ensemble intérieurement régulières

#### Définition 1 {#int-ix-s3-def-1 .statement}

*Soit T un espace topologique, et soit $\mathcal{B}(T)$ la tribu borélienne de T; soit I une application de $\mathcal{B}(T)$ dans $\overline{\mathbf{R}}_+$.
a) On dit que I est dénombrablement additive si, pour toute suite $(A_n)$ d’éléments de $\mathcal{B}(T)$ deux à deux disjoints, on a*
$$
I(\bigcup_n A_n) = \sum_n I(A_n).
$$

b) On dit que I est intérieurement régulière si, pour tout ensemble $A \in \mathcal{B}(T)$, on a
$$
(5) \quad I(A) = \sup_K I(K),
$$
$K$ parcourant l’ensemble des parties compactes de $A$.

c) On dit que I est bornée (resp. localement bornée) si $I(T) < +\infty$ (resp. si tout point $x \in T$ admet un voisinage ouvert $V$ tel que $I(V) < +\infty$).

#### Remarque 1 {#int-ix-s3-n2-rem-1 .statement}

La condition a) entraîne évidemment que I est une application croissante de $\mathcal{B}(T)$ (ordonné par inclusion) dans $\overline{\mathbf{R}}_+$.

#### Remarque 2 {#int-ix-s3-n2-rem-2 .statement}

Supposons que I soit dénombrablement additive; soit $(A_n)_{n \in \mathbf{N}}$ une suite croissante d’ensembles boréliens, et soit $A = \bigcup_{n \in \mathbf{N}} A_n$. Les ensembles $D_0 = A_0, D_n = A_n - A_{n-1}$ étant deux à deux disjoints, et leur réunion étant $A$, on a $I(A) = \sum_n I(D_n) = \lim_{n \to \infty} I(A_n)$. De même, si $(B_n)$ est une suite décroissante d’ensembles boréliens, et si $I(B_0) < +\infty$, on a $I(\bigcap_n B_n) = \lim_{n \to \infty} I(B_n)$: il suffit d’appliquer ce qui précède aux ensembles $A_n = B_0 - B_n$.

#### Remarque 3 {#int-ix-s3-n2-rem-3 .statement}

Soit $(A_n)$ une suite quelconque de parties boréliennes de $T$. Si I est dénombrablement additive, on a $I(\bigcup_n A_n) \leq \sum_n I(A_n)$. D’après la remarque précédente, il suffit d’établir cette inégalité pour une suite finie. On se ramène alors aussitôt au cas de deux ensembles $A_1$ et $A_2$; mais la relation (4) entraîne que
$$
I(A_1 \cup A_2) = I(A_1) + I(A_2 - (A_1 \cap A_2)) \leq I(A_1) + I(A_2).
$$
L’inégalité cherchée en résulte immédiatement.

#### Remarque 4 {#int-ix-s3-n2-rem-4 .statement}

Si I est une fonction dénombrablement additive et localement bornée, la remarque précédente entraîne aussitôt que $I(K) < +\infty$ pour tout compact $K \subset T$.

#### Remarque 5 {#int-ix-s3-n2-rem-5 .statement}

On peut montrer que si I est additive, c’est-à-dire satisfait à (4) pour les suites finies, et si I est intérieurement régulière, alors I est dénombrablement additive (exerc. 7). Le lecteur pourra d’ailleurs constater que seule l’additivité et la régularité intérieure sont utilisées dans la démonstration du th. 2 ci-dessous.

#### Théorème 2 {#int-ix-s3-thm-2 .statement}

Soit T un espace topologique, et soit I une fonction définie sur $\mathcal{B}(T)$, à valeurs dans $\overline{\mathbf{R}}_+$. Pour qu’il existe une mesure $\mu$ sur T, telle que $\mu^*(A) = I(A)$ pour tout $A \in \mathcal{B}(T)$, il faut et il suffit que I soit dénombrablement additive, localement bornée et intérieurement régulière. La mesure $\mu$ est alors unique.

Ces trois conditions sont nécessaires : l’application $A \mapsto \mu^*(A)$ sur $\mathcal{B}(T)$ est en effet dénombrablement additive (§ 1, n° 5, cor. de la prop. 4), localement bornée d’après la définition des mesures (§ 1, n° 2, déf. 5) et intérieurement régulière d’après la Remarque 3 du § 1, n° 2.

Passons à l’existence. Il est clair que la restriction de I à $\mathfrak{A}(T)$ satisfait aux conditions 1), 2), 3) et 5) de l’énoncé du th. 1; montrons que 4) est également satisfaite. Soit K une partie compacte de T, intersection d’une famille filtrante décroissante $(K_\alpha)_{\alpha \in A}$ d’ensembles compacts, et soit $\varepsilon$ un nombre $> 0$; I étant localement bornée, il existe un voisinage ouvert (donc borélien) V de K tel que $I(V) < +\infty$, et il existe alors un indice $\alpha$ tel que $K_\alpha \subset V$; quitte à changer de notation, nous pouvons supposer que $K_\alpha \subset V$ pour tout $\alpha \in A$. D’après la régularité intérieure de I, il existe un ensemble compact $L \subset V - K$ tel que

I(L) ≥ I(V − K) − ε; comme L ne rencontre pas K, il existe un indice α tel que L ∩ K_α = ∅, et on a alors I(V − K_α) ≥ I(L) ≥ I(V − K) − ε. Comme on a K_α ⊂ V, il en résulte I(K_α) ≤ I(K) + ε et la condition 4) est vérifiée.

D’après le th. 1, il existe une mesure μ telle que μ^•(K) = I(K) pour tout K ∈ 𝔽(T). La régularité intérieure des fonctions d’ensembles μ^• et I sur 𝔽(T) entraîne alors μ^•(A) = I(A) pour tout A ∈ 𝔽(T) et l’existence est prouvée. L’unicité de μ résulte de l’assertion d’unicité du th. 1.

### 3. Espaces radoniens

#### Définition 2 {#int-ix-s3-def-2 .statement}

Soit T un espace topologique. On dit que T est un espace radonien (resp. fortement radonien) si T est séparé et si toute fonction définie sur la tribu borélienne 𝔽(T) de T, à valeurs dans $\overline{\mathbf{R}}_+$, dénombrablement additive et bornée (resp. localement bornée) est intérieurement régulière.

Par exemple, nous verrons plus loin (prop. 3) que tout espace polonais est fortement radonien. En particulier, tout espace localement compact à base dénombrable est fortement radonien.

Il existe des espaces radoniens qui ne sont pas fortement radoniens.

#### Proposition 1 {#int-ix-s3-prop-1 .statement}

Tout espace de Lindelöf (1) radonien est fortement radonien.

Soit T un espace de Lindelöf radonien, et soit I une fonction d’ensemble, positive, dénombrablement additive et localement bornée, sur la tribu 𝔽(T). Les ensembles ouverts V tels que I(V) < +∞ forment un recouvrement de T, dont on peut extraire un recouvrement dénombrable $(V_n)_{n \in \mathbf{N}}$. Posons $G_n = V_0 \cup V_1 \cup \ldots \cup V_n$ pour tout $n \in \mathbf{N}$; posons $H_0 = G_0$ et $H_n = G_n - G_{n-1}$ pour $n \geq 1$; désignons enfin par $I_n$ la fonction d’ensemble $A \mapsto I(A \cap H_n)$ sur 𝔽(T), qui est évidemment dénombrablement additive et bornée. Les ensembles $H_n$ formant une partition de T, on a $I = \sum_n I_n$. L’espace T étant radonien, il existe pour chaque $n \in \mathbf{N}$ une mesure bornée $\mu_n$ sur T telle qu’on ait $\mu_n^•(A) = I_n(A)$ pour tout $A \in \mathcal{B}(T)$; on a donc aussi $\sum_n \mu_n^•(A) = I(A)$. Comme I est localement bornée, la famille $(\mu_n)$ est sommable (§ 1, n° 7, prop. 7); si $μ$ désigne $\sum_n \mu_n$, on a $μ^•(A) = I(A)$ pour tout $A \in \mathcal{B}(T)$, et il en résulte que I est intérieurement régulière. Autrement dit, T est fortement radonien.

Rappelons qu’une partie A d’un espace topologique T est dite universellement mesurable si A est $μ$-mesurable pour toute mesure $μ$ sur T. Cela revient à dire que A est $μ$-mesurable pour toute mesure $μ$ sur T à support compact (§ 1, n° 8, prop. 9).

(1) Rappelons (Top. gén. chap. IX, Appendice I) qu’on appelle espace de Lindelöf tout espace topologique T tel que de tout recouvrement ouvert de T, on puisse extraire un recouvrement dénombrable.

#### Proposition 2 {#int-ix-s3-prop-2 .statement}

Soient $X$ un espace topologique et $T$ un sous-espace de $X$.

a) Supposons que $T$ soit radonien. Pour toute fonction $I$ définie sur $\mathcal{B}(X)$, positive, dénombrablement additive et bornée, on a alors

$$
\sup_{\substack{K \text{ compact} \\ K \subset T}} I(K) = \inf_{\substack{B \in \mathcal{B}(X) \\ B \supset T}} I(B).
$$

De plus, $T$ est universellement mesurable dans $X$.

b) Inversement, supposons que $X$ soit radonien, et que $T$ soit universellement mesurable dans $X$; alors $T$ est radonien.

Démontrons a). Désignons par $\alpha$ le second membre de (6); pour tout $n \in \mathbf{N}$, il existe un ensemble $C_n \in \mathcal{B}(X)$ contenant $T$, et tel que $I(C_n) \leq \alpha + 2^{-n}$. Si l’on pose $C = \bigcap_n C_n$, on a alors $T \subset C$, $I(C) = \alpha$. Si $A \in \mathcal{B}(T)$, choisissons une partie borélienne $B$ de $X$ telle que $A = B \cap T$ (*Top. gén.*, chap. IX, 3e éd., § 6, n° 3) et posons $J(A) = I(B \cap C)$. Ce nombre ne dépend pas du choix de $B$, car si $B'$ est un second ensemble, borélien dans $X$, tel que $A = B' \cap T$, alors $B \cap C$ et $B' \cap C$ ne diffèrent que par un ensemble borélien $M$ contenu dans $C - T$, et on a $I(M) = 0$ d’après la construction de $C$. On a évidemment $J(K) = I(K)$ pour tout ensemble compact $K \subset T$. Soit $(A_n)$ une suite de parties boréliennes de $T$, deux à deux disjointes, et, pour chaque $n$, soit $B_n$ une partie borélienne de $X$ telle que $B_n \cap T = A_n$. Quitte à remplacer $B_n$ par $B_n - (\bigcup_{k < n} B_k)$, on peut supposer que les ensembles $B_n$ sont deux à deux disjoints. Posons $A = \bigcup_n A_n$ et $B = \bigcup_n B_n$; on a $J(A) = I(B \cap C) = \sum_n I(B_n \cap C) = \sum_n J(A_n)$; $J$ est donc une fonction dénombrablement additive et bornée sur $\mathcal{B}(T)$. Comme $T$ est radonien par hypothèse, il existe une mesure bornée $\mu$ sur $T$ telle que $J(A) = \mu^*(A)$ pour tout $A \in \mathcal{B}(T)$; on a par conséquent $\alpha = J(T) = \mu^*(T) = \sup_K \mu^*(K) = \sup_K J(K)$, par définition de $\mu^*$. La formule (6) est donc établie.

Montrons que $T$ est universellement mesurable. Soit $\lambda$ une mesure bornée sur $X$; le raisonnement précédent s’applique à la fonction d’ensemble $I : A \mapsto \lambda^*(A)$ sur $\mathcal{B}(X)$, et il existe donc une suite $(K_n)$ de parties compactes de $T$ telles que l’on ait (avec les notations ci-dessus)

$$
\sup_n \lambda^*(K_n) = J(T) = \lambda^*(C).
$$

Posons $K' = \bigcup_{n \in \mathbf{N}} K_n$; $K'$ est borélien dans $X$, on a $K' \subset T \subset C$, $\lambda^*(K') = \lambda^*(C)$, donc ces trois ensembles ne diffèrent que par des ensembles $\lambda$-négligeables, et $T$ est $\lambda$-mesurable. Cela achève la démonstration de a).

Passons à b). Supposons que $X$ soit radonien, et que $T$ soit universellement mesurable dans $X$. Soit $I$ une fonction positive, dénombrablement additive et bornée sur $\mathcal{B}(T)$; la fonction $A \mapsto I(A \cap T)$ sur $\mathcal{B}(X)$ est alors positive, dénombrablement additive et bornée, et il existe donc une mesure bornée $\nu$ sur $X$ telle que $I(A \cap T) = v^*(A)$ pour tout $A \in \mathfrak{B}(X)$. Or $T$ est $v$-mesurable; la relation précédente montre que $v^*(K) = 0$ pour tout compact $K$ de $X$ disjoint de $T$, et $v$ est donc concentrée sur $T$. Par conséquent, pour tout ensemble borélien $A$ de $X$, on a $I(A \cap T) = v^*(A \cap T) = \mu^*(A \cap T)$, où $\mu$ est la mesure induite par $v$ sur $T$. Il en résulte enfin que $I(B) = \mu^*(B)$ pour tout ensemble $B \in \mathfrak{B}(T)$ (\emph{Top. gén.}, chap. IX, 3\textsuperscript{e} éd., § 6, no 3, *Remarque*), et $I$ est bien intérieurement régulière.

#### Corollaire {#int-ix-s3-n3-cor-1 .statement}

*Si $X$ est un espace radonien, tout sous-ensemble borélien $T$ de $X$ est radonien.*

En effet, $T$ est universellement mesurable dans $X$.

#### Proposition 3 {#int-ix-s3-prop-3 .statement}

*Tout espace souslinien (en particulier tout espace polonais ou lusinien) est fortement radonien.*

Soit $T$ un espace souslinien; $T$ étant un espace de Lindelöf (*Top. gén.*, chap. IX, 3\textsuperscript{e} éd., Appendice I, cor. de la prop. 1), il suffit de montrer que $T$ est radonien (prop. 1). Soit $I$ une fonction définie sur $\mathfrak{B}(T)$, positive, dénombrablement additive et bornée. Nous prolongerons $I$ à $\mathfrak{P}(T)$ en posant, pour toute partie $A$ de $T$

$$
I(A) = \inf_{\substack{B \in \mathfrak{B}(T) \\ B \supseteq A}} I(B).
$$

Montrons que ce prolongement est une *capacité* sur $T$ (*Top. Gén.*, chap. IX, 3\textsuperscript{e} éd., § 6, no 9). Il est clair que la relation $A \subset A'$ entraîne $I(A) \leq I(A')$. Soit $(A_n)$ une suite croissante de parties de $T$, et soit $A = \bigcup_n A_n$. L’ensemble des parties boréliennes qui contiennent $A_n$ étant stable pour les intersections dénombrables, il existe pour chaque $n$ un ensemble borélien $B_n$ tel que $A_n \subset B_n$ et $I(A_n) = I(B_n)$ (cf. démonstration de la prop. 2). Posons $C_n = \bigcap_{p \geq n} B_p$; $C_n$ est borélien, et on a $A_n \subset C_n \subset B_n$, donc $I(A_n) = I(C_n)$. D’autre part, la suite $(C_n)$ est croissante. Soit $C = \bigcup_n C_n$: la relation $A \subset C$ entraîne $I(A) \leq I(C) = \lim_n I(C_n) = \lim_n I(A_n)$ d’où aussitôt l’égalité $I(A) = \lim_n I(A_n)$. Par suite, $I$ est une capacité.

Si $(H_n)$ est une suite décroissante d’ensembles fermés dans $T$, on a évidemment $I(\bigcap_n H_n) = \inf_n I(H_n)$. Il en résulte que tout sous-ensemble souslinien $F$ de $T$ est capacitable pour $I$ (*Top. gén.*, chap. IX, 3\textsuperscript{e} éd., § 4, no 9, prop. 15). En particulier, tout sous-ensemble borélien $A$ de $T$ est capacitable (*loc. cit.*, no 3, prop. 10). Autrement, dit, on a

$$
I(A) = \sup_K I(K),
$$

$K$ parcourant l’ensemble des compacts contenus dans $A$; on a prouvé que $I$ est intérieurement régulière.

#### Remarque {#int-ix-s3-n3-rem-1 .statement}

Soient $X$ un espace lusinien (en particulier un espace polonais), et $f$ une application continue bijective de $X$ dans un espace (régulier) $Y$. On sait (*Top. gén.*, chap. IX, 3e éd., § 6, n° 7, prop. 14) que l’application $B \mapsto f^{-1}(B)$ est une bijection de la tribu borélienne de $Y$ sur la tribu borélienne de $X$. Les espaces $X$ et $Y$ sont lusiniens, donc fortement radoniens (prop. 3). Il en résulte immédiatement que l’application $\mu \mapsto f(\mu)$ est une bijection de l’ensemble des mesures bornées sur $X$ sur l’ensemble des mesures bornées sur $Y$.

## EXERCICES {#int-ix-s3-exercises}

See the [exercises for § 3](exercises/s3/).
