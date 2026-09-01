---
book: int
book_title: Integration
chapter: IX
chapter_title: MESURES SUR LES ESPACES TOPOLOGIQUES SÉPARÉS
section: 4
section_title: Limites projectives de mesures
lang: fr
source: int-ix-fr
pdf_pages: 0048-0053, 0104-0104
extraction: ocr
subsections:
    - "no": 1
      title: Compléments sur les espaces compacts et les limites projectives
      page: 0
      pdf_page: 48
    - "no": 2
      title: Systèmes projectifs de mesures
      page: 0
      pdf_page: 49
    - "no": 3
      title: Cas des systèmes projectifs dénombrables
      page: 0
      pdf_page: 51
statements: 7
exercises: 2
content_sha256: 3f704416f3acfabd112831848a0a9daa10e262eae898fd3efdc042174b2adef4
---

## § 4. Limites projectives de mesures

Dans tout ce paragraphe, on note $I$ un ensemble non vide, muni d’une relation de préordre, notée $i \leq j$, et filtrant pour cette relation. Rappelons (Top. gén., 4e éd., chap. I, § 4, n° 4) qu’un système projectif d’espaces topologiques indexé par $I$ est une famille $(T_i, p_{ij})$ où $T_i$ est un espace topologique et $p_{ij}$ une application continue de $T_j$ dans $T_i$ pour $i \leq j$, où $p_{ii}$ est l’application identique de $T_i$ et où l’on a $p_{ik} = p_{ij} \circ p_{jk}$ pour $i \leq j \leq k$. Soient $T$ un espace topologique et $(p_i)_{i \in I}$ une famille d’applications continues $p_i : T \to T_i$. On dit que la famille $(p_i)_{i \in I}$ est cohérente si l’on a $p_i = p_{ij} \circ p_j$ pour $i \leq j$, et qu’elle est séparante si pour $x, y$ distincts dans $T$, il existe $i \in I$ tel que $p_i(x) \neq p_i(y)$. Lorsque $T = \lim_{\leftarrow} T_i$ et que $p_i$ est l’application canonique de $T$ dans $T_i$, la famille $(p_i)_{i \in I}$ est cohérente et séparante.

### 1. Compléments sur les espaces compacts et les limites projectives

#### Proposition 1 {#int-ix-s4-prop-1 .statement}

Soient $X$ et $Y$ deux espaces topologiques et $f$ une application continue de $X$ dans $Y$. Soit $(K_\alpha)_{\alpha \in A}$ une famille filtrante décroissante de parties compactes de $X$, d’intersection $K$. On a alors $f(K) = \bigcap_{\alpha \in A} f(K_\alpha)$.

En effet, soit $y$ un point de $\bigcap_{\alpha \in A} f(K_\alpha)$; pour tout $\alpha \in A$, l’ensemble $L_\alpha = K_\alpha \cap f^{-1}(y)$ est compact et non vide. La famille $(L_\alpha)_{\alpha \in A}$ est filtrante décroissante, donc son intersection $L$ est non vide. Or on a $L = K \cap f^{-1}(y)$, d’où $y \in f(K)$. On a donc prouvé l’inclusion $f(K) \supset \bigcap_{\alpha \in A} f(K_\alpha)$ et l’inclusion inverse est évidente.

#### Proposition 2 {#int-ix-s4-prop-2 .statement}

Soient donnés un système projectif $(T_i, p_{ij})$ d’espaces topologiques indexé par $I$, un espace topologique $T$ et une famille cohérente et séparante d’applications continues $p_i : T \to T_i$. Alors :

a) Pour toute partie compacte $K$ de $T$, on a $K = \bigcap_{i \in I} p_i^{-1}(p_i(K))$.

b) Soient $K$ et $L$ deux parties compactes disjointes de $T$. Il existe $i \in I$ tel que $p_j(K)$ et $p_j(L)$ soient disjoints pour $j \geq i$.

a) Soit $x$ un point de $\bigcap_{i \in I} p_i^{-1}(p_i(K))$; pour tout $i \in I$, l’ensemble $K_i$ formé des points $y$ de $K$ tels que $p_i(y) = p_i(x)$ est une partie fermée non vide de $K$. Pour $i \leq j$, on a $K_i \supset K_j$, et comme $K$ est compact, l’ensemble $\bigcap_{i \in I} K_i$ est donc non vide. Soit $y$ un point de $\bigcap_{i \in I} K_i$; on a $y \in K$ et $p_i(y) = p_i(x)$ pour tout $i \in I$, d’où $y = x$; finalement, on a $x \in K$, ce qui démontre l’inclusion $K \supset \bigcap_{i \in I} p_i^{-1}(p_i(K))$; l’inclusion opposée est évidente.

n° 4.2.

b) Pour tout $i \in I$, posons $M_i = p_i^{-1}(p_i(K)) \cap L$; c'est une partie fermée de l'espace compact $L$, on a $M_i \supset M_j$ pour $i \leq j$ et, d'après a), on a $\bigcap_{i \in I} M_i = K \cap L = \varnothing$. Par suite, il existe un indice $i$ tel que $M_i = \varnothing$. Pour $j \geq i$, on a $p_j^{-1}(p_j(K)) \cap L = M_j \subset M_i = \varnothing$, d'où $p_j(K) \cap p_j(L) = \varnothing$.

### 2. Systèmes projectifs de mesures

#### Définition 1 {#int-ix-s4-def-1 .statement}

Soit $\mathcal{T} = (T_i, p_{ij})$ un système projectif d'espaces topologiques indexé par $I$. On appelle système projectif (resp. système sous-projectif) de mesures sur $\mathcal{T}$ une famille $(\mu_i)_{i \in I}$ où $\mu_i$ est une mesure bornée sur $T_i$ pour tout $i \in I$, et où l'on a $\mu_i = p_{ij}(\mu_j)$ (resp. $\mu_i \geq p_{ij}(\mu_j)$) pour $i \leq j$.

#### Proposition 3 {#int-ix-s4-prop-3 .statement}

Soient donnés un système projectif d'espaces topologiques $\mathcal{T} = (T_i, p_{ij})$ indexé par $I$, un espace topologique $T$, une famille cohérente et séparante d'applications continues $p_i : T \to T_i$ (pour $i \in I$) et un système sous-projectif $(\mu_i)_{i \in I}$ de mesures sur $\mathcal{T}$. Pour toute partie compacte $K$ de $T$, on pose

$$
J(K) = \inf_{i \in I} \mu_i^*(p_i(K)).
$$

Il existe alors une mesure bornée $\pi$ sur $T$, et une seule, telle que $\pi^*(K) = J(K)$ pour tout compact $K$ de $T$. On a $\mu_i \geq p_i(\pi)$ pour tout $i \in I$ et $\pi$ est la plus grande des mesures sur $T$ satisfaisant à cette condition.

Prouvons d'abord que $J(K)$ est la limite de $\mu_i(p_i(K))$ selon le filtre des sections $\mathfrak{F}$ de l'ensemble préordonné filtrant $I$: il suffit pour cela (Top. gén., chap. IV, 3e éd., § 5, n° 2, th. 2) de montrer que l'on a $\mu_i^*(p_i(K)) \geq \mu_j^*(p_j(K))$ pour $i \leq j$; or, si l'on pose $\mu_{ij}' = p_{ij}(\mu_j)$, on a $\mu_{ij}' \leq \mu_i$ et $p_j(K) \subset p_{ij}^{-1}(p_i(K))$, d'où

$$
\mu_j^*(p_j(K)) \leq \mu_j^*(p_{ij}^{-1}(p_i(K))) = (\mu_{ij}')^*(p_i(K)) \leq \mu_i^*(p_i(K)).
$$

Passons maintenant à l'étude des propriétés de la fonction $J$:
1) Il est clair que l'on a $J(K) \leq J(L)$ lorsque $K \subset L$.
2) Soient $K$ et $L$ deux parties compactes de $T$. Pour tout $i \in I$, on a $p_i(K \cup L) \subset p_i(K) \cup p_i(L)$, d'où

$$
\mu_i^*(p_i(K \cup L)) \leq \mu_i^*(p_i(K)) + \mu_i^*(p_i(L));
$$

passant à la limite selon le filtre $\mathfrak{F}$, on obtient $J(K \cup L) \leq J(K) + J(L)$.
3) Supposons les compacts $K$ et $L$ disjoints. D'après la prop. 2 du n° 1, il existe $i \in I$ tel que $p_j(K) \cap p_j(L) = \varnothing$ pour $j \geq i$. Pour $j \geq i$, on a donc

$$
\mu_j^*(p_j(K \cup L)) = \mu_j^*(p_j(K)) + \mu_j^*(p_j(L)),
$$

d'où $J(K \cup L) = J(K) + J(L)$ en passant à la limite selon le filtre $\mathfrak{F}$.
4) Soit $(K_\alpha)_{\alpha \in A}$ une famille filtrante décroissante de parties compactes de $T$, d'intersection $K$. D'après la prop. 1 du n° 1, on a $p_i(K) = \bigcap_{\alpha \in A} p_i(K_\alpha)$ et par suite μ_i^*(p_i(K)) = \inf_{\alpha \in A} \mu_i^*(p_i(K_\alpha)) pour tout i \in I (§ 1, n° 6, cor. de la prop. 5). On en déduit

$$
J(K) = \inf_{i \in I} \mu_i^*(p_i(K)) = \inf_{i \in I} \inf_{\alpha \in A} \mu_i^*(p_i(K_\alpha))
= \inf_{\alpha \in A} \inf_{i \in I} \mu_i^*(p_i(K_\alpha)) = \inf_{\alpha \in A} J(K_\alpha).
$$

5) Choisissons i dans I et posons c = μ_i^*(T_i). Alors c est fini et l’on a J(K) ≤ μ_i^*(p_i(K)) ≤ μ_i^*(T_i), soit J(K) ≤ c pour tout compact K de T.

Les propriétés précédentes permettent d’appliquer le th. 1 du § 3, n° 1; on en conclut qu’il existe une mesure bornée π sur T, et une seule, telle que π^*(K) = J(K) pour toute partie compacte K de T. Pour tout i ∈ I, notons ν_i la mesure sur T_i image de π par p_i. Soient i ∈ I, A une partie compacte de T_i et Ω l’ensemble des parties compactes de p_i^{-1}(A). D’après la Remarque 3 du § 1, n° 2, on a π^*(p_i^{-1}(A)) = \sup_{K \in \Omega} π^*(K); on a par ailleurs ν_i^*(A) = π^*(p_i^{-1}(A)) et J(K) = π^*(K) pour K ∈ Ω, d’où ν_i^*(A) = \sup_{K \in \Omega} J(K). Pour K ∈ Ω, on a p_i(K) ⊂ A, d’où J(K) ≤ μ_i^*(p_i(K)) ≤ μ_i^*(A) et finalement ν_i^*(A) ≤ μ_i^*(A). Comme A est un ensemble compact arbitraire dans T_i, on en conclut ν_i ≤ μ_i.

C.Q.F.D.

#### Théorème 1 (Prokhorov) {#int-ix-s4-thm-1 .statement}

Soient $\mathcal{T} = (T_i, p_{ij})$ un système projectif d’espaces topologiques indexé par I, T un espace topologique et $(p_i)_{i \in I}$ une famille cohérente et séparante d’applications continues $p_i : T \to T_i$. Enfin soit $(\mu_i)_{i \in I}$ un système projectif de mesures sur $\mathcal{T}$.

Pour qu’il existe une mesure bornée μ sur T telle que $p_i(\mu) = \mu_i$ pour tout $i \in I$, il faut et il suffit que soit vérifiée la condition suivante:
(P) pour tout $\varepsilon > 0$, il existe une partie compacte K de T telle que $\mu_i^*(T_i - p_i(K)) \leq \varepsilon$ pour tout $i \in I$.

S’il en est ainsi, la mesure μ est déterminée de manière unique et l’on a

(2)
$$
\mu^*(K) = \inf_i \mu_i^*(p_i(K))
$$
pour tout ensemble compact K dans T.

Démontrons d’abord l’unicité de μ. Soit μ une mesure bornée sur T telle que $p_i(\mu) = \mu_i$ pour tout $i \in I$. Soit K une partie compacte de T; d’après la prop. 2 du n° 1, l’ensemble K est intersection de la famille filtrante décroissante $(p_i^{-1}(p_i(K)))_{i \in I}$ de parties fermées de T. D’après le cor. de la prop. 5 du § 1, n° 6, on a donc
$$
\mu^*(K) = \inf_{i \in I} \mu^*(p_i^{-1}(p_i(K))) = \inf_{i \in I} \mu_i^*(p_i(K)),
$$
ce qui établit la formule (2). Comme deux mesures qui coïncident sur l’ensemble des compacts sont égales (§ 1, n° 2, cor. de la prop. 2), on en déduit l’unicité de μ.

D’après la prop. 3, il existe sur T une mesure bornée π telle que $\pi^*(K) = \inf_{i \in I} \mu_i^*(p_i(K))$ pour toute partie compacte K de T. D’après la formule (2), l’existence d’une mesure bornée $\mu$ sur $T$ telle que $p_i(\mu) = \mu_i$ pour tout $i \in I$ équivaut donc à la relation:

(P') *On a* $p_i(\pi) = \mu_i$ pour tout $i \in I$.

Pour $i \leq j$, on a $\mu_i = p_{ij}(\mu_j)$, d’où $\mu_i^*(T_i) = \mu_j^*(T_j)$; comme $I$ est filtrant, il existe un nombre fini $c \geq 0$ tel que $\mu_i^*(T_i) = c$ pour tout $i \in I$. D’après la prop. 3, la mesure $\mu_i - p_i(\pi)$ est positive, donc est nulle si et seulement si sa masse totale est nulle, c’est-à-dire si $\mu_i(T_i) = p_i(\pi)^*(T_i)$. Comme on a $p_i(\pi)^*(T_i) = \pi^*(T)$, la condition (P') équivaut donc à $\pi^*(T) = c$, c’est-à-dire ($§ 1$, n° 2, *Remarque 3*) à la propriété:

(P'') *On a* $\sup_{K \in \mathfrak{K}} \pi^*(K) = c$, où $\mathfrak{K}$ est l’ensemble des *parties compactes* de $T$.

Or, pour $K \in \mathfrak{K}$, on a
$$
\pi^*(K) = \inf_{i \in I} \mu_i^*(p_i(K)) = c - \sup_{i \in I} \mu_i^*(T_i - p_i(K))
$$
et cette formule entraîne immédiatement l’équivalence de (P) et (P'').

C.Q.F.D.

Soit $(T_i, p_{ij})$ un système projectif d’espaces topologiques. Posons $T = \lim_{\leftarrow} T_i$ et notons $p_i$ l’application canonique de $T$ dans $T_i$. Généralisant la déf. 2 du chap. III, $§ 4$, n° 5, on dira qu’une mesure bornée $\mu$ sur $T$ est *limite projective d’un système projectif* $(\mu_i)_{i \in I}$ *de mesures* si l’on a $\mu_i = p_i(\mu)$ pour tout $i \in I$. Le th. 1 fournit un critère d’existence des limites projectives de mesures. Lorsque les espaces $T_i$ sont *compacts*, et les applications $p_{ij}$ surjectives, $T$ est compact et l’on a $p_i(T) = T_i$ pour tout $i \in I$; la condition (P) est donc remplie, et l’on retrouve dans ce cas la prop. 8, (iv) du chap. III, $§ 4$, n° 5.

#### Remarque {#int-ix-s4-n2-rem-1 .statement}

Soit $(\mu_i)_{i \in I}$ un système projectif de mesures sur le système projectif d’espaces $\mathcal{T} = (T_i, p_{ij})$. On suppose donné un espace topologique $T'$ et des applications continues $p'_i : T' \to T_i$; on suppose que la famille $(p'_i)_{i \in I}$ est cohérente, mais non nécessairement séparante. *Si la condition de Prokhorov (P) est satisfaite par la famille* $(p'_i)_{i \in I}$, *il existe une mesure* $\mu'$ (*non nécessairement unique*) *sur* $T'$ *avec* $p'_i(\mu') = \mu_i$ *pour tout* $i \in I$.

Posons $T = \lim_{\leftarrow} T_i$ et $p' = (p'_i)_{i \in I}$, et notons $p_i$ l’application canonique de $T$ dans $T_i$; la condition de Prokhorov est satisfaite par $T$ et les $p_i$, car on a $p_i(p'(K')) = p'_i(K')$ et $p'(K')$ est compact dans $T$ pour toute partie compacte $K'$ de $T'$. D’après le th. 1, il existe une mesure bornée $\mu$ sur $T$ telle que $p_i(\mu) = \mu_i$ pour tout $i \in I$. Soit $K'$ un ensemble compact dans $T'$; on a $\mu^*(p'(K')) = \inf_{i \in I} \mu_i^*(p'_i(K'))$, d’où
$$
\mu^*(T - p'(K')) = \sup_{i \in I} \mu_i^*(T_i - p'_i(K')) .
$$
Soit $\varepsilon > 0$; comme la condition de Prokhorov (P) est satisfaite par les $p'_i$, on peut donc trouver un compact $K'$ de $T'$ tel que $\mu^*(T - p'(K')) \leq \varepsilon$. La prop. 8 du $§ 2$, n° 4 établit alors l’existence d’une mesure bornée $\mu'$ sur $T'$ avec $\mu = p'(\mu')$, d’où $\mu_i = p_i(\mu) = p_i(p'(\mu')) = p'_i(\mu')$ pour tout $i \in I$.

### 3. Cas des systèmes projectifs dénombrables

#### Théorème 2 {#int-ix-s4-thm-2 .statement}

*On suppose que l’ensemble préordonné filtrant* $I$ *possède une partie cofinale* dénombrable. *Soient* $\mathcal{T} = (T_i, p_{ij})$ *un système projectif d’espaces topologiques,*

T = \lim_{\leftarrow} T_i et p_i l'application canonique de T dans T_i. Tout système projectif (\mu_i)_{i \in I} de mesures sur \mathcal{T} admet alors une limite projective.

Nous traiterons d'abord le cas où I = \mathbf{N} et nous poserons q_n = p_{n, n+1}. Soit \varepsilon > 0. Par récurrence, on définit une suite d'ensembles compacts L_n \subset T_n comme suit; L_0 est une partie compacte de T_0 telle que \mu_0^\bullet(T_0 - L_0) \leq \varepsilon/2, et pour n \geq 0, l'ensemble compact L_{n+1} est contenu dans q_n^{-1}(L_n) et tel que
$$
\mu_{n+1}^\bullet(q_n^{-1}(L_n) - L_{n+1}) \leq \varepsilon/2^{n+2}.
$$
Cette construction est possible en vertu de la Remarque 3 du § 1, n° 2. On a
$$
\begin{align*}
\mu_{n+1}^\bullet(T_{n+1} - L_{n+1}) &= \mu_{n+1}^\bullet(T_{n+1} - q_n^{-1}(L_n)) + \mu_{n+1}^\bullet(q_n^{-1}(L_n) - L_{n+1}) \\
&\leq \mu_{n+1}^\bullet(T_{n+1} - q_n^{-1}(L_n)) + \varepsilon/2^{n+2} \\
&= \mu_n^\bullet(T_n - L_n) + \varepsilon/2^{n+2}
\end{align*}
$$
car \mu_n = q_n(\mu_{n+1}); par récurrence sur p, on en déduit
$$
\mu_p^\bullet(T_p - L_p) \leq \varepsilon(1 - 1/2^{p+1}) \leq \varepsilon.
$$
Comme T est un sous-espace fermé de \prod_{n \in \mathbf{N}} T_n et que l'espace produit \prod_{n \in \mathbf{N}} L_n est compact, la partie L = T \cap \prod_{n \in \mathbf{N}} L_n = \bigcap_{n \in \mathbf{N}} p_n^{-1}(L_n) de T est compacte. Soit n \in \mathbf{N}; on a p_n(L) = \bigcap_{m \geq n} p_{nm}(L_m) (Top. gén., chap. I, 4e éd., § 9, n° 6, prop. 8) et p_{nm}(L_m) \supset p_{nm'}(L_{m'}) pour m' \geq m \geq n, d'où
$$
\mu_n^\bullet(T_n - p_n(L)) = \lim_{m \to \infty} \mu_n^\bullet(T_n - p_{nm}(L_m)).
$$
Mais, pour m \geq n, la mesure \mu_n est image de \mu_m par p_{nm}, d'où
$$
\mu_n^\bullet(T_n - p_{nm}(L_m)) = \mu_m^\bullet(T_m - p_{nm}^{-1}(p_{nm}(L_m))) \leq \mu_m^\bullet(T_m - L_m) \leq \varepsilon;
$$
en passant à la limite sur m, on obtient \mu_n^\bullet(T_n - p_n(L)) \leq \varepsilon. Autrement dit, la condition de Prokhorov (P) est satisfaite, et il existe une mesure bornée \mu sur T telle que \mu_n = p_n(\mu) pour tout n \in \mathbf{N} (n° 2, th. 1).

Passons au cas général: il existe dans I une suite cofinale croissante (i_n)_{n \in \mathbf{N}}. L'application t \mapsto (p_{i_n}(t))_{n \in \mathbf{N}} est un homéomorphisme de T sur la limite projective du système projectif (T_{i_n}, p_{i_n i_m}) (Top. gén., chap. I, 4e éd., § 4, n° 4). D'après la première partie de la démonstration, il existe donc une mesure bornée \mu sur T telle que \mu_{i_n} = p_{i_n}(\mu) pour tout n \in \mathbf{N}. Soit i \in I; il existe n \in \mathbf{N} avec i \leq i_n, d'où
$$
p_i(\mu) = p_{i i_n}(p_{i_n}(\mu)) = p_{i i_n}(\mu_{i_n}) = \mu_i.
$$
C.Q.F.D.

Le théorème 2 est souvent utilisé dans la situation suivante: soient D un ensemble dénombrable et (X_t)_{t \in D} une famille d'espaces topologiques. Soit \mathfrak{F} l'ensemble des parties finies de D, ordonné par inclusion. Pour J dans \mathfrak{F}, posons

X_J = \prod_{t \in J} X_t, et pour J \subset J', soit $p_{JJ'}$ la projection canonique de $X_{J'}$ sur le produit partiel $X_J$. On pose aussi $X = \prod_{t \in D} X_t$ et l'on note $p_J$ la projection canonique de $X$ sur le produit partiel $X_J$. On montre facilement (cf Ens., chap. III, 2e éd., § 7, n° 2, Remarque 3) que la famille $(p_J)_{J \in \mathfrak{g}}$ définit un homéomorphisme de $X$ sur $\lim_{\leftarrow} X_J$. Un système projectif de mesures $\mu$ est alors une famille de mesures bornées $\mu_J$ sur $X_J$ telles que $\mu_J = p_{JJ'}(\mu_{J'})$ pour $J \subset J'$. Il existe une mesure bornée $\mu$ sur $X$ et une seule telle que $\mu_J = p_J(\mu)$ pour toute partie finie $J$ de $D$ (« Théorème de Kolmogoroff »). On dit parfois que $\mu$ est la mesure sur $\prod_{t \in D} X_t$ admettant les marges $\mu_J$.

En particulier, supposons donnée, pour tout $t \in D$, une mesure $\nu_t$ de masse totale 1 sur $X_t$. Posons $\mu_J = \bigotimes_{t \in J} \nu_t$ pour toute partie finie $J$ de $D$. Soient $J \subset J'$ deux parties finies de $D$ et $K = J' - J$; si l'on identifie $X_{J'}$ à $X_J \times X_K$, on a $\mu_{J'} = \mu_J \otimes \mu_K$, et comme la mesure $\mu_K$ est de masse totale 1, la projection de $\mu_J \otimes \mu_K$ sur $X_J$ est égale à $\mu_J$. La mesure sur $X$ admettant les marges $\mu_J$ se note $\bigotimes_{t \in D} \nu_t$ et s'appelle le *produit de la famille* $(\nu_t)_{t \in D}$. Lorsque les espaces $X_t$ sont compacts, on retrouve la construction du chap. III, 2e éd., § 4, n° 6.

## EXERCICES {#int-ix-s4-exercises}

See the [exercises for § 4](exercises/s4/).
