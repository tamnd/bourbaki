---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ENSEMBLES ORDONNÉS, CARDINAUX, NOMBRES ENTIERS
section: 7
section_title: Limites projectives et limites inductives
lang: fr
source: ens-i-iv-fr
source_edition: 2006, Springer
book_pages: E III.94-E III.96
pdf_pages: 0155-0173, 0198-0200
extraction: ocr
subsections:
    - "no": 1
      title: Limites projectives
      page: 51
      pdf_page: 155
    - "no": 2
      title: Systèmes projectifs d’applications
      page: 52
      pdf_page: 156
    - "no": 3
      title: Double limite projective
      page: 56
      pdf_page: 160
    - "no": 4
      title: Conditions pour qu’une limite projective soit non vide
      page: 57
      pdf_page: 161
    - "no": 5
      title: Limites inductives
      page: 60
      pdf_page: 164
    - "no": 6
      title: Systèmes inductifs d’applications
      page: 62
      pdf_page: 166
    - "no": 7
      title: Double limite inductive. Produit de limites inductives
      page: 66
      pdf_page: 170
statements: 26
exercises: 10
content_sha256: 8c30384cc85751bc4198f0143b858784f0b5074aaeb93001f72b9ed872738c39
---

## § 7. LIMITES PROJECTIVES ET LIMITES INDUCTIVES

### 1. Limites projectives

Soient I un ensemble préordonné, $(E_\alpha)_{\alpha \in I}$ une famille d’ensembles ayant I pour ensemble d’indices. Pour tout couple $(\alpha, \beta)$ d’indices de I tels que $\alpha \leq \beta$, soit $f_{\alpha \beta}$ une application de $E_\beta$ dans $E_\alpha$. On suppose que les $f_{\alpha \beta}$ vérifient les conditions suivantes:

(LP_I) Les relations $\alpha \leq \beta \leq \gamma$ entraînent $f_{\alpha \gamma} = f_{\alpha \beta} \circ f_{\beta \gamma}$.
(LP_{II}) Pour tout $\alpha \in I$, $f_{\alpha \alpha}$ est l’application identique de $E_\alpha$.

Soit $G = \prod_{\alpha \in I} E_\alpha$ l’ensemble *produit* de la famille d’ensembles $(E_\alpha)_{\alpha \in I}$, et désignons par $E$ la partie de $G$ formée des éléments $x$ satisfaisant à *chacune* des relations
(1)
$$
\mathrm{pr}_\alpha x = f_{\alpha \beta}(\mathrm{pr}_\beta x)
$$
pour tout couple d’indices $(\alpha, \beta)$ tel que $\alpha \leq \beta$. On dit que $E$ est *la limite projective de la famille* $(E_\alpha)_{\alpha \in I}$ *pour la famille d’applications* $(f_{\alpha \beta})$, et on écrit $E = \lim_{\leftarrow} (E_\alpha, f_{\alpha \beta})$ ou simplement $E = \lim_{\leftarrow} E_\alpha$ si aucune confusion n’en résulte. Par abus de langage, on dira que le couple $((E_\alpha), (f_{\alpha \beta}))$ (que l’on notera aussi $(E_\alpha, f_{\alpha \beta})$) est un *système projectif d’ensembles*, relatif à l’ensemble d’indices $I$. On dit que la *restriction* $f_\alpha$ à $E$ de la projection $\mathrm{pr}_\alpha$ est l’*application canonique* de $E$ dans $E_\alpha$; on a la relation
(2)
$$
f_\alpha = f_{\alpha \beta} \circ f_\beta
$$
pour $\alpha \leq \beta$, ce qui ne fait que traduire les relations (1) définissant $E$.

#### Exemple 1 {#ens-iii-s7-n1-exa-1 .statement tag=03TF}

Supposons que la relation de préordre dans $I$ soit la relation d’égalité. Alors les seuls couples $(\alpha, \beta)$ tels que $\alpha \leq \beta$ sont les couples $(\alpha, \alpha)$ pour $\alpha \in I$, et comme $f_{\alpha \alpha}$ est l’application identique, la relation (1) est vérifiée pour *tout* $x \in G$; autrement dit, $\lim_{\leftarrow} E_\alpha$ est alors le *produit* $\prod_{\alpha \in I} E_\alpha$.

#### Exemple 2 {#ens-iii-s7-n1-exa-2 .statement tag=03TG}

Supposons que $I$ soit *filtrant à droite*, que pour tout $\alpha \in I$, $E_\alpha$ soit égal à un même ensemble $F$ et que pour $\alpha \leq \beta$, $f_{\alpha \beta}$ soit l’application identique de $F$ sur lui-même. Alors $E = \lim_{\leftarrow} E_\alpha$ n’est autre que la *diagonale* $\Delta$ du produit $G = \prod_{\alpha \in I} E_\alpha = F^I$. En effet, il est clair que tout $x \in \Delta$ vérifie les relations (1). Inversement, soit $x$ un élément de $E$ et montrons que pour tout couple d’indices $(\alpha, \beta)$ dans $I$, on a $\mathrm{pr}_\alpha x = \mathrm{pr}_\beta x$. En effet, il existe par hypothèse $\gamma \in I$ tel que $\alpha \leq \gamma$ et $\beta \leq \gamma$, donc on déduit de (1) que $\mathrm{pr}_\alpha x = f_{\alpha \gamma}(\mathrm{pr}_\gamma x) = \mathrm{pr}_\gamma x$ et de même $\mathrm{pr}_\beta x = \mathrm{pr}_\gamma x$, d’où notre assertion.

On notera que $E = \lim_{\leftarrow} E_\alpha$ peut être *vide* même lorsque les $E_\alpha$ sont tous *non vides* et que chacune des applications $f_{\alpha \beta}$ est *surjective* (III, p. 94, exerc. 4; voir III, p. 57–60).

Il est clair que pour toute partie $J$ de $I$, le couple formé de la sous-famille $(E_\alpha)_{\alpha \in J}$ et de la famille $(f_{\alpha \beta})$ où $\alpha \in J, \beta \in J$ et $\alpha \leq \beta$, est encore un système projectif d’ensembles, relatif à $J$; on dira qu’il est obtenu par *restriction* à $J$ de l’ensemble d’indices. Notons $E$ et $E'$ les limites projectives des familles $(E_\alpha)_{\alpha \in I}$ et $(E_\alpha)_{\alpha \in J}$ respectivement; pour tout $x \in E$, l’élément
(3)
$$
g(x) = (f_\alpha(x))_{\alpha \in J}
$$
appartient à $E'$ en vertu de (2); l’application $g : E \to E'$ ainsi définie est dite *canonique*. Si $J'$ est une partie de $J$, $E''$ la limite projective de la famille $(E_\alpha)_{\alpha \in J'}$, $g' : E' \to E''$ et $g'' : E \to E''$ les applications canoniques, on a, par définition,
(4)
$$
g'' = g' \circ g.
$$

### 2. Systèmes projectifs d’applications

#### Proposition 1 {#ens-iii-s7-prop-1 .statement tag=03OC}

*Soient I un ensemble préordonné,* $(E_\alpha, f_{\alpha \beta})$ *un système projectif d’ensembles relativ à I,* $E = \lim_{\leftarrow} E_\alpha$ *sa limite projective,* et *pour tout* $\alpha \in I$, *soit* $f_\alpha : E \to E_\alpha$ l’application canonique. Pour tout $\alpha \in \mathbf{I}$, soit $u_\alpha$ une application d’un ensemble $F$ dans $E_\alpha$ telle que l’on ait
$$
f_{\alpha \beta} \circ u_\beta = u_\alpha \tag{5}
$$
pour $\alpha \leq \beta$.

Dans ces conditions :
1° Il existe une application et une seule $u$ de $F$ dans $E$ telle que
$$
u_\alpha = f_\alpha \circ u \tag{6}
$$
pour tout $\alpha \in \mathbf{I}$.

2° Pour que $u$ soit injective, il faut et il suffit que pour tout couple d’éléments distincts $y, z$ de $F$, il existe $\alpha \in \mathbf{I}$ tel que $u_\alpha(y) \neq u_\alpha(z)$.

En effet, la relation $u_\alpha = f_\alpha \circ u$ signifie que pour tout $y \in F$, on a $\mathrm{pr}_\alpha(u(y)) = u_\alpha(y)$; l’élément $u(y) \in \prod_{\alpha \in \mathbf{I}} E_\alpha$ est déterminé de façon unique par $u(y) = (u_\alpha(y))_{\alpha \in \mathbf{I}}$.
Reste à voir que $u(y) \in E$ pour tout $y \in F$, autrement dit que l’on a
$$
\mathrm{pr}_\alpha(u(y)) = f_{\alpha \beta}(\mathrm{pr}_\beta(u(y)))
$$
pour $\alpha \leq \beta$; mais cela s’écrit $u_\alpha(y) = f_{\alpha \beta}(u_\beta(y))$ et résulte donc de (5). La seconde partie de la proposition découle aussitôt des définitions.

#### Corollaire 1 {#ens-iii-s7-prop-1-cor-1 .statement tag=03RN}

Soient $(E_\alpha, f_{\alpha \beta})$ et $(F_\alpha, g_{\alpha \beta})$ deux systèmes projectifs d’ensembles relatifs à un même ensemble d’indices $\mathbf{I}$; soient $E = \lim_{\leftarrow} E_\alpha$, $F = \lim_{\leftarrow} F_\alpha$, et pour tout $\alpha \in \mathbf{I}$, soit $f_\alpha$ (resp. $g_\alpha$) l’application canonique de $E$ dans $E_\alpha$ (resp. de $F$ dans $F_\alpha$). Pour tout $\alpha \in \mathbf{I}$, soit $u_\alpha$ une application de $E_\alpha$ dans $F_\alpha$ telle que, pour $\alpha \leq \beta$, le diagramme
$$
\begin{array}{ccc}
E_\beta & \xrightarrow{u_\beta} & F_\beta \\
f_{\alpha \beta} \downarrow & & g_{\alpha \beta} \downarrow \\
E_\alpha & \xrightarrow{u_\alpha} & F_\alpha
\end{array}
$$
soit commutatif.\footnote{Cela signifie que l’on a $u_\alpha \circ f_{\alpha \beta} = g_{\alpha \beta} \circ u_\beta$.} Il existe alors une application $u : E \to F$ et une seule telle que, pour tout $\alpha \in \mathbf{I}$, le diagramme
$$
\begin{array}{ccc}
E & \xrightarrow{u} & F \\
f_\alpha \downarrow & & g_\alpha \downarrow \\
E_\alpha & \xrightarrow{u_\alpha} & F_\alpha
\end{array}
$$
soit commutatif.

Posons $v_\alpha = u_\alpha \circ f_\alpha$. Pour $\alpha \leq \beta$, on a, d’après (2)
$$
g_{\alpha \beta} \circ v_\beta = g_{\alpha \beta} \circ u_\beta \circ f_\beta = u_\alpha \circ f_{\alpha \beta} \circ f_\beta = u_\alpha \circ f_\alpha = v_\alpha
$$
et on peut donc appliquer la prop. 1 aux $v_\alpha$; d’où l’existence et l’unicité d’une application $u : E \to F$ telle que
$$
g_\alpha \circ u = v_\alpha = u_\alpha \circ f_\alpha
$$
pour tout $\alpha \in \mathbf{I}$.

On dit qu'une famille d'applications $u_\alpha : E_\alpha \to F_\alpha$ satisfaisant aux conditions du cor. 1 est un système projectif d'applications de $(E_\alpha, f_{\alpha\beta})$ dans $(F_\alpha, g_{\alpha\beta})$; l'application $u$ définie dans le cor. 1 est appelée la limite projective de la famille $(u_\alpha)$ et se note $u = \lim \leftarrow u_\alpha$ lorsque aucune confusion n'est à craindre.

#### Corollaire 2 {#ens-iii-s7-prop-1-cor-2 .statement tag=03RO}

Soient $(E_\alpha, f_{\alpha\beta}), (F_\alpha, g_{\alpha\beta}), (G_\alpha, h_{\alpha\beta})$ trois systèmes projectifs d'ensembles relatifs à $I$; soient $E = \lim \leftarrow E_\alpha, F = \lim \leftarrow F_\alpha, G = \lim \leftarrow G_\alpha$, et soit $f_\alpha$ (resp. $g_\alpha, h_\alpha$) l'application canonique de $E$ (resp. $F, G$) dans $E_\alpha$ (resp. $F_\alpha, G_\alpha$). Si $(u_\alpha)$ et $(v_\alpha)$ sont deux systèmes projectifs d'applications, $u_\alpha : E_\alpha \to F_\alpha,\ v_\alpha : F_\alpha \to G_\alpha$, alors les $v_\alpha \circ u_\alpha : E_\alpha \to G_\alpha$ forment un système projectif d'applications, et l'on a

$$
\lim \leftarrow (v_\alpha \circ u_\alpha) = (\lim \leftarrow v_\alpha) \circ (\lim \leftarrow u_\alpha).
$$

En effet, si on pose $w_\alpha = v_\alpha \circ u_\alpha$, on a, pour $\alpha \leq \beta$

$$
w_\alpha \circ f_{\alpha\beta} = v_\alpha \circ (u_\alpha \circ f_{\alpha\beta}) = v_\alpha \circ (g_{\alpha\beta} \circ u_\beta) = (h_{\alpha\beta} \circ v_\beta) \circ u_\beta = h_{\alpha\beta} \circ w_\beta
$$

ce qui montre que $(w_\alpha)$ est un système projectif d'applications. En outre, si on pose $u = \lim \leftarrow u_\alpha,\ v = \lim \leftarrow v_\alpha$, on a, pour tout $\alpha \in I$

$$
h_\alpha \circ (v \circ u) = (v_\alpha \circ g_\alpha) \circ u = (v_\alpha \circ u_\alpha) \circ f_\alpha
$$

et en raison de l'unicité de la limite projective, on a $v \circ u = \lim \leftarrow w_\alpha$.

Soit $(E_\alpha, f_{\alpha\beta})$ un système projectif d'ensembles, et pour tout $\alpha \in I$, soit $M_\alpha$ une partie de $E_\alpha$. Si l'on a $f_{\alpha\beta}(M_\beta) \subset M_\alpha$ pour $\alpha \leq \beta$, on dit que les $M_\alpha$ forment un système projectif de parties des $E_\alpha$. Soit $g_{\alpha\beta}$ l'application de $M_\beta$ dans $M_\alpha$ (pour $\alpha \leq \beta$) ayant même graphe que la restriction de $f_{\alpha\beta}$ à $M_\beta$; il est clair que $(M_\alpha, g_{\alpha\beta})$ est un système projectif d'ensembles, et l'on a

$$
\lim \leftarrow M_\alpha = (\lim \leftarrow E_\alpha) \cap \prod_{\alpha \in I} M_\alpha.
$$

#### Proposition 2 {#ens-iii-s7-prop-2 .statement tag=03RP}

Soient $(E_\alpha, f_{\alpha\beta}), (E'_\alpha, f'_{\alpha\beta})$ deux systèmes projectifs d'ensembles relatifs à $I$, et pour chaque $\alpha \in I$, soit $u_\alpha$ une application de $E_\alpha$ dans $E'_\alpha$, les $u_\alpha$ formant un système projectif d'applications. Soit $u = \lim \leftarrow u_\alpha$. Pour tout $x' = (x'_\alpha) \in E' = \lim \leftarrow E'_\alpha$, les $\bar{u}_\alpha^{-1}(x'_\alpha)$ forment un système projectif de parties des $E_\alpha$, et l'on a $\bar{u}^{-1}(x') = \lim \leftarrow \bar{u}_\alpha^{-1}(x'_\alpha)$.

En effet, si $\alpha \leq \beta$ et $x_\beta \in \bar{u}_\beta^{-1}(x'_\beta)$, on a

$$
u_\alpha(f_{\alpha\beta}(x_\beta)) = f'_{\alpha\beta}(u_\beta(x_\beta)) = f'_{\alpha\beta}(x'_\beta) = x'_\alpha,
$$

d'où la première assertion; et dire que $x = (x_\alpha) \in E = \lim \leftarrow E_\alpha$ est tel que $u(x) = x'$ signifie par définition que $u_\alpha(x_\alpha) = x'_\alpha$ pour tout $\alpha \in I$.

#### Corollaire {#ens-iii-s7-n2-cor-1 .statement tag=03OD}

Si $u_\alpha$ est injective (resp. bijective) pour tout $\alpha \in I$, $u$ est injective (resp. bijective).

On notera qu’avec les notations de la prop. 2, les images $u_\alpha(E_\alpha)$ forment aussi un système projectif de parties des $E'_\alpha$ et l’on a
$$
u(E) \subset \lim_{\leftarrow} u_\alpha(E_\alpha)
$$
mais les deux membres de cette relation ne sont pas nécessairement égaux (III, p. 94, exerc. 4).

#### Proposition 3 {#ens-iii-s7-prop-3 .statement tag=03OE}

*Soient I un ensemble préordonné, $(E_\alpha, f_{\alpha\beta})$ un système projectif d’ensembles relatif à I, $E = \lim_{\leftarrow} E_\alpha$ sa limite projective. Soient J une partie cofinale de I, filtrante à droite, $E'$ la limite projective du système projectif d’ensembles obtenu à partir de $(E_\alpha, f_{\alpha\beta})$ par restriction à J de l’ensemble d’indices. Alors l’application canonique g de E dans $E'$ (III, p. 52, formule (3)) est bijective.*

Pour tout $\alpha \in J$, soit $f'_\alpha$ l’application canonique $E' \to E_\alpha$; alors, compte tenu de (2) et (5), g est l’unique application de E dans $E'$ telle que $f_\alpha = f'_\alpha \circ g$ pour tout $\alpha \in J$ (III, p. 52, prop. 1). Vérifions le critère de la prop. 1 pour voir que g est injective: si $x, y$ sont deux éléments distincts de E, il existe par définition un $\alpha \in I$ tel que $f_\alpha(x) \neq f_\alpha(y)$; comme J est cofinal dans I, il existe $\lambda \in I$ tel que $\alpha \leq \lambda$; comme $f_{\alpha\lambda}(f_\lambda(x)) \neq f_{\alpha\lambda}(f_\lambda(y))$, on a bien $f_\lambda(x) \neq f_\lambda(y)$. Montrons ensuite que g est surjective. Soit $x' = (x'_\lambda)_{\lambda \in J}$ un élément de $E'$. Pour tout $\alpha \in I$, il existe $\lambda \in I$ tel que $\alpha \leq \lambda$; montrons que l’élément $f_{\alpha\lambda}(x'_\lambda)$ ne dépend pas de l’indice $\lambda \in J$ tel que $\alpha \leq \lambda$. En effet si $\mu \in J$ est tel que $\alpha \leq \mu$, il existe $\nu \in J$ tel que $\lambda \leq \nu$ et $\mu \leq \nu$, donc $f_{\alpha\lambda}(x'_\lambda) = f_{\alpha\lambda}(f_{\lambda\nu}(x'_\nu)) = f_{\alpha\nu}(x'_\nu)$, et de même $f_{\alpha\mu}(x'_\mu) = f_{\alpha\nu}(x'_\nu)$, d’où notre assertion. Soit $x_\alpha$ la valeur commune des $f_{\alpha\lambda}(x'_\lambda)$ pour les $\lambda \in J$ tels que $\alpha \leq \lambda$, et posons $x = (x_\alpha)_{\alpha \in I}$. L’élément x appartient à E, car si $\alpha \leq \beta$ et si $\lambda \in J$ est tel que $\beta \leq \lambda$, on a $f_{\alpha\beta}(x_\beta) = f_{\alpha\beta}(f_{\beta\lambda}(x'_\lambda)) = f_{\alpha\lambda}(x'_\lambda) = x_\alpha$. Enfin, on a $x'_\lambda = f_{\lambda\lambda}(x'_\lambda)$ pour tout $\lambda \in J$, donc $x_\lambda = x'_\lambda$ pour tout $\lambda \in J$, autrement dit $f_\lambda(x) = x'_\lambda$, d’où $g(x) = x'$, ce qui achève la démonstration.

En particulier, si I admet un *plus grand élément* $\omega$, on peut prendre $J = \{\omega\}$, et on voit que $\lim_{\leftarrow} E_\alpha$ s’identifie canoniquement à $E_\omega$.

*Remarques*

1) Pour tout $\alpha \in I$, posons $E'_\alpha = f_\alpha(E)$; les $E'_\alpha$ forment un *système projectif de parties* des $E_\alpha$ en vertu de (2), et il est immédiat que l’on a $\lim_{\leftarrow} E'_\alpha = E = \lim_{\leftarrow} E_\alpha$; on notera que l’application $f'_{\alpha\beta} : E'_\beta \to E'_\alpha$ (pour $\alpha \leq \beta$) ayant même graphe que la restriction de $f_{\alpha\beta}$ à $E'_\beta$ est *surjective*; en outre, on a
$$
E'_\alpha = f_\alpha(E) \subset \bigcap_{\beta \geq \alpha} f_{\alpha\beta}(E_\beta)
$$
pour tout $\alpha \in I$.

2) Soient I un ensemble préordonné *filtrant à droite*, $(E_\alpha, f_{\alpha\beta})$ un système projectif d’ensembles relatif à I, et pour tout $\alpha \in I$, soit $u_\alpha : F \to E_\alpha$ une application, telle que la famille $(u_\alpha)$ vérifie (5). Considérons le système projectif $(F_\alpha, i_{\alpha\beta})$ relatif à I, où $F_\alpha = F$ pour tout $\alpha \in I$ et $i_{\alpha\beta}$ est l’application identique de F. On sait alors

(III, p. 52, Exemple 2) que F s’identifie canoniquement à $\lim_{\leftarrow} F_\alpha$. Si on considère $u_\alpha$ comme application de $F_\alpha$ dans $E_\alpha$, $(u_\alpha)$ est un système projectif d’applications, et l’application $u : F \to E$ définie par (6) s’identifie à la limite projective de ce système d’applications. Aussi écrit-on alors par abus de langage $u = \lim_{\leftarrow} u_\alpha$.

3) Soient I un ensemble ordonné, $(E_\alpha, f_{\alpha\beta})$ un système projectif d’ensembles relatif à I. Pour toute partie finie J de I, soit $F_J$ la limite projective du système projectif (fini) obtenu à partir de $(E_\alpha, f_{\alpha\beta})$ par restriction à J de l’ensemble d’indices. Pour deux parties finies J, K de I telles que $J \subset K$, soit $g_{JK}$ l’application canonique (3) de $F_K$ dans $F_J$; la relation (4) montre que $(F_J, g_{KJ})$ est un système projectif d’ensembles relatif à l’ensemble ordonné filtrant (pour la relation $\subset$) $\mathfrak{F}(I)$ des parties finies de I. D’autre part, pour tout $J \in \mathfrak{F}(I)$, soit $h_J : E \to F_J$ l’application canonique (3); en vertu de (4) (et avec l’abus de langage signalé dans la Remarque 2), $(h_J)$ est un système projectif d’applications; posons $h = \lim_{\leftarrow} h_J : E \to F = \lim_{\leftarrow} F_J$, et montrons que $h$ est une bijection (dite canonique). En effet, soit $y = (y_J)$ un élément de F; on a par définition $y_J = (x_{\alpha, J})_{\alpha \in J}$ avec $x_{\alpha, J} \in E_\alpha$ pour tout $\alpha \in J$; si $J \subset K$, on a, par définition des $g_{JK}$ et en raison de la relation $y_J = g_{JK}(y_K)$, $x_{\alpha, J} = x_{\alpha, K}$ pour tout $\alpha \in J$. Pour un $\alpha \in I$, il y a donc un unique élément $x_\alpha \in E_\alpha$ tel que $x_\alpha = x_{\alpha, J}$ pour tout J fini contenant $\alpha$. Si $\alpha \leq \beta$, il y a une partie finie J de I contenant à la fois $\alpha$ et $\beta$, donc $x_\alpha = f_{\alpha\beta}(x_\beta)$ par définition; on en conclut que $x = (x_\alpha)$ est l’unique élément de E tel que $h(x) = y$.

### 3. Double limite projective

Soient I, L deux ensembles préordonnés, $I \times L$ leur produit (III, p. 7). Considérons un système projectif d’ensembles $(E^\lambda_\alpha, f^{\lambda\mu}_{\alpha\beta})$ relatif à l’ensemble d’indices $I \times L$; on a donc

$$
f^{\lambda\nu}_{\alpha\gamma} = f^{\lambda\mu}_{\alpha\beta} \circ f^{\mu\nu}_{\beta\gamma} \quad \text{pour } \alpha \leq \beta \leq \gamma \text{ et } \lambda \leq \mu \leq \nu.
$$

Désignons par E ou $\lim_{\leftarrow, \lambda} E^\lambda_\alpha$ la limite projective de ce système projectif.

Pour tout $\lambda \in L$, posons $g^\lambda_{\alpha\beta} = f^{\lambda\lambda}_{\alpha\beta} : E^\lambda_\beta \to E^\lambda_\alpha$; il résulte de (11) que l’on a

$$
g^\lambda_{\alpha\gamma} = g^\lambda_{\alpha\beta} \circ g^\lambda_{\beta\gamma} \quad \text{pour } \alpha \leq \beta \leq \gamma,
$$

autrement dit $(E^\lambda_\alpha, g^\lambda_{\alpha\beta})$ est un système projectif d’ensembles relatif à I; notons $F^\lambda = \lim_{\leftarrow} E^\lambda_\alpha$ sa limite projective. D’autre part, pour $\lambda \leq \mu$ fixés dans L, il résulte de (11) que les $h^{\lambda\mu}_{\alpha} = f^{\lambda\mu}_{\alpha\alpha} : E^\mu_\alpha \to E^\lambda_\alpha$ forment un système projectif d’applications; nous noterons $h^{\lambda\mu} = \lim_{\leftarrow} h^{\lambda\mu}_{\alpha} : F^\mu \to F^\lambda$ sa limite projective. Pour $\lambda \leq \mu \leq \nu$ dans L, on a

$$
h^{\lambda\nu} = h^{\lambda\mu} \circ h^{\mu\nu}
$$

(III, p. 54, cor. 2); donc $(F^\lambda, h^{\lambda\mu})$ est un système projectif d’ensembles relatif à L. Soit $F = \lim_{\leftarrow} F^\lambda$ sa limite projective; nous allons définir une bijection canonique $F \to E$. Remarquons pour cela que F est, par définition, une partie de $\prod_{\lambda \in L} F^\lambda$, et

F^λ une partie de $\prod_{\alpha \in I} E_\alpha^\lambda$; donc F s’identifie canoniquement à une partie de $\prod_{(\alpha, \lambda) \in I \times L} E_\alpha^\lambda = G$ (II, p. 35, prop. 7). Pour tout $z \in G$, soit $\mathrm{pr}^\lambda(z)$ l’élément $(\mathrm{pr}_\alpha^\lambda(z))_{\alpha \in I}$ de $\prod_{\alpha \in I} E_\alpha^\lambda$; dire que $z \in F$ signifie que l’on a
(14)
$$
\mathrm{pr}^\lambda(z) = h^{\lambda \mu}(\mathrm{pr}^\mu(z)) \quad \text{pour } \lambda \leq \mu \text{ dans } L
$$
et que $\mathrm{pr}^\lambda(z) \in F^\lambda$ pour tout $\lambda \in L$, c’est-à-dire que pour $\alpha \leq \beta$ dans I on a
(15)
$$
\mathrm{pr}_\alpha^\lambda(z) = f_{\alpha \beta}^{\lambda \lambda}(\mathrm{pr}_\beta^\lambda(z)).
$$
Mais on a $h^{\lambda \mu}(\mathrm{pr}^\mu(z)) = (f_{\alpha \alpha}^{\lambda \mu}(\mathrm{pr}_\alpha^\mu(z)))_{\alpha \in I}$; on déduit donc de (14) et (15) que pour $\alpha \leq \beta$ et $\lambda \leq \mu$, on a
$$
\mathrm{pr}_\alpha^\lambda(z) = f_{\alpha \alpha}^{\lambda \mu}(f_{\alpha \beta}^{\mu \mu}(\mathrm{pr}_\beta^\mu(z))) = f_{\alpha \beta}^{\lambda \mu}(\mathrm{pr}_\beta^\mu(z))
$$
ce qui signifie que $z \in E$; la réciproque est immédiate. Autrement dit:

#### Proposition 4 {#ens-iii-s7-prop-4 .statement tag=03OF}

Si $(E_\alpha^\lambda, f_{\alpha \beta}^{\lambda \mu})$ est un système projectif d’ensembles relatif à un produit $I \times L$ d’ensembles préordonnés, on a, à une bijection canonique près
(16)
$$
\lim_{\leftarrow \alpha, \lambda} E_\alpha^\lambda = \lim_{\leftarrow \lambda} (\lim_{\leftarrow \alpha} E_\alpha^\lambda).
$$

#### Corollaire 1 {#ens-iii-s7-prop-4-cor-1 .statement tag=03OG}

Soit $(E_\alpha^{'\lambda}, f_{\alpha \beta}^{'\lambda \mu})$ un second système projectif d’ensembles relatif à $I \times L$, et, pour tout $(\alpha, \lambda) \in I \times L$, soit $u_\alpha^\lambda$ une application de $E_\alpha^\lambda$ dans $E_\alpha^{'\lambda}$, les $u_\alpha^\lambda$ formant un système projectif d’applications. On a alors
(17)
$$
\lim_{\leftarrow \alpha, \lambda} u_\alpha^\lambda = \lim_{\leftarrow \lambda} (\lim_{\leftarrow \alpha} u_\alpha^\lambda).
$$
La vérification est analogue.

#### Corollaire 2 {#ens-iii-s7-prop-4-cor-2 .statement tag=03OH}

Soit $(E_\alpha^\lambda, f_{\alpha \beta}^\lambda)_{\lambda \in L}$ une famille de systèmes projectifs relatifs à I. Alors, si on note $\prod_{\lambda \in L} f_{\alpha \beta}^\lambda$ l’extension aux produits de la famille d’applications $(f_{\alpha \beta}^\lambda)_{\lambda \in L}$ (II, p. 38, déf. 2), $(\prod_{\lambda \in L} E_\alpha^\lambda, \prod_{\lambda \in L} f_{\alpha \beta}^\lambda)$ est un système projectif d’ensembles relatif à I, et on a, à une bijection canonique près
(18)
$$
\lim_{\leftarrow \alpha} \prod_{\lambda \in L} E_\alpha^\lambda = \prod_{\lambda \in L} (\lim_{\leftarrow \alpha} E_\alpha^\lambda).
$$
Il suffit de considérer le système projectif $(E_\alpha^\lambda, g_{\alpha \beta}^{\lambda \mu})$ relatif à $I \times L$ où la relation d’ordre sur L est l’égalité (III, p. 52, Exemple 1) et où $g_{\alpha \beta}^{\lambda \mu} = f_{\alpha \beta}^\lambda$ pour $\lambda = \mu$, et de lui appliquer la prop. 4.

### 4. Conditions pour qu’une limite projective soit non vide

Nous allons dans ce n° donner les deux conditions suffisantes pour qu’une limite projective soit non vide, qui sont le plus souvent utilisées (voir aussi III, p. 94, exerc. 5).

#### Proposition 5 {#ens-iii-s7-prop-5 .statement tag=03OI}

Soit $(E_\alpha, f_{\alpha\beta})$ un système projectif d'ensembles relatif à un ensemble préordonné filtrant $I$, qui admet une partie cofinale dénombrable; supposons en outre que les $f_{\alpha\beta}$ soient surjectives. Alors, si $E = \lim_{\leftarrow} E_\alpha$, l'application canonique $f_\alpha : E \to E_\alpha$ est surjective pour tout $\alpha \in I$ (et a fortiori, $E$ n'est pas vide si aucun des $E_\alpha$ n'est vide).

Soit $(\alpha_n)$ une suite d'éléments de $I$ formant une partie cofinale de $I$. Comme $I$ est filtrant, on peut définir par récurrence une suite $(\beta_n)$ par les conditions $\beta_0 = \alpha_0$, $\beta_n \geq \beta_i$ pour $i < n$ et $\beta_n \geq \alpha_n$; il est clair que la suite $(\beta_n)$ est croissante et forme une partie cofinale de $I$; tenant compte de III, p. 52, prop. 1 et des relations $f_\alpha = f_{\alpha\beta_n} \circ f_{\beta_n}$ pour $\alpha \leq \beta_n$, on voit qu'on est ramené à prouver la proposition lorsque $I = \mathbf{N}$. En outre, il est clair qu'il suffit de prouver que $f_0$ est surjective. Soit donc $x_0 \in E_0$; on définit par récurrence $x_n \in E_n$ pour $n \geq 1$ comme un élément de $f_{n-1,n}^{-1}(x_{n-1})$, ce qui est possible puisque ce dernier ensemble n'est pas vide par hypothèse. On prouve alors par récurrence sur $n - m$ que pour $m \leq n$, on a $x_m = f_{mn}(x_n)$, donc $x = (x_n)$ appartient à $E$.

Le second critère concerne les systèmes projectifs $(E_\alpha, f_{\alpha\beta})$ relatifs à un ensemble d'indices $I$, tels que pour tout $\alpha \in I$ on se soit donné un ensemble $\mathcal{S}_\alpha$ de parties de $E_\alpha$, vérifiant les conditions suivantes:

(i) Toute intersection d'ensembles de $\mathcal{S}_\alpha$ appartient à $\mathcal{S}_\alpha$.

Il résulte en particulier de cette condition (en considérant l'intersection de la famille vide) que $E_\alpha \in \mathcal{S}_\alpha$.

(ii) Si un ensemble de parties $\mathfrak{F} \subset \mathcal{S}_\alpha$ est tel que toute intersection finie d'ensembles appartenant à $\mathfrak{F}$ soit non vide, alors $\bigcap_{M \in \mathfrak{F}} M$ est non vide.

Il est clair, compte tenu de (i), que (ii) est équivalente à la condition suivante:

(ii') Si $\mathfrak{G} \subset \mathcal{S}_\alpha$ est un ensemble filtrant décroissant dont les éléments sont non vides, alors $\bigcap_{M \in \mathfrak{G}} M$ est non vide.

#### Théorème 1 {#ens-iii-s7-thm-1 .statement tag=03RQ}

On suppose que $I$ est filtrant, que les $\mathcal{S}_\alpha$ satisfont aux conditions (i) et (ii), et en outre que le système projectif $(E_\alpha, f_{\alpha\beta})$ possède les propriétés suivantes:

(iii) Pour tout couple d'indices $\alpha, \beta$ tels que $\alpha \leq \beta$, et tout $x_\alpha \in E_\alpha$, on a $f_{\alpha\beta}^{-1}(x_\alpha) \in \mathcal{S}_\beta$.

(iv) Pour tout couple d'indices $\alpha, \beta$ tels que $\alpha \leq \beta$ et tout $M_\beta \in \mathcal{S}_\beta$, on a $f_{\alpha\beta}(M_\beta) \in \mathcal{S}_\alpha$.

Soit $E = \lim_{\leftarrow} E_\alpha$, et pour tout $\alpha \in I$, soit $f_\alpha : E \to E_\alpha$ l'application canonique. Alors:

a) Pour tout $\alpha \in I$, on a

$$
f_\alpha(E) = \bigcap_{\beta \geq \alpha} f_{\alpha\beta}(E_\beta).
$$

b) Si, pour tout $\alpha \in I$, $E_\alpha$ est non vide, alors $E$ est non vide.

Soit $\Sigma$ l'ensemble des familles $\mathfrak{A} = (A_\alpha)_{\alpha \in I}$ vérifiant les conditions:

$$
A_\alpha \neq \varnothing \quad \text{et} \quad A_\alpha \in \mathcal{S}_\alpha \quad \text{pour tout} \quad \alpha \in I;
$$

$$
f_{\alpha\beta}(A_\beta) \subset A_\alpha \quad \text{pour} \quad \alpha \leq \beta.
$$

Pour deux éléments $\mathfrak{A} = (A_\alpha)$, $\mathfrak{A}' = (A'_\alpha)$ de $\Sigma$, la relation $\mathfrak{A} \leq \mathfrak{A}'$ signifiera que $A_\alpha \supset A'_\alpha$ pour tout $\alpha$; il est clair que $\Sigma$ est ordonné par cette relation.

1° Prouvons d’abord que l’ensemble ordonné $\Sigma$ est *inductif*. Soient $L$ un ensemble totalement ordonné, $\lambda \mapsto \mathfrak{A}^\lambda = (A^\lambda_\alpha)_{\alpha \in I}$ une application strictement croissante de $L$ dans $\Sigma$. Pour tout $\alpha \in I$, posons $B_\alpha = \bigcap_{\lambda \in L} A^\lambda_\alpha$; il est immédiat que la famille $\mathfrak{B} = (B_\alpha)_{\alpha \in I}$ vérifie (21); en vertu de (i) et (ii'), elle vérifie aussi (20), donc $\mathfrak{B} \in \Sigma$, et il est clair que $\mathfrak{B}$ majore l’ensemble des $\mathfrak{A}^\lambda$.

2° Soit $\mathfrak{A} = (A_\alpha)$ un élément *maximal* de $\Sigma$; montrons que l’on a alors $A_\alpha = f_{\alpha \beta}(A_\beta)$ pour $\alpha \leq \beta$. En effet, soit $A'_\alpha = \bigcap_{\beta \geq \alpha} f_{\alpha \beta}(A_\beta)$ pour tout $\alpha \in I$; montrons que $\mathfrak{A}' = (A'_\alpha)$ appartient à $\Sigma$. Notons d’abord que pour $\alpha \leq \beta \leq \gamma$ on a $f_{\alpha \gamma}(A_\gamma) = f_{\alpha \beta}(f_{\beta \gamma}(A_\gamma)) \subset f_{\alpha \beta}(A_\beta)$ en vertu de (21); en outre on a $f_{\alpha \beta}(A_\beta) \in \mathcal{S}_\alpha$ d’après (iv), et $f_{\alpha \beta}(A_\beta) \neq \varnothing$ par (20); les conditions (i) et (ii) montrent alors que $\mathfrak{A}'$ vérifie (20). Enfin $\mathfrak{A}'$ vérifie aussi (21): en effet, si $\alpha \leq \beta$, on a

$$
f_{\alpha \beta}(A'_\beta) \subset \bigcap_{\gamma \geq \beta} f_{\alpha \beta}(f_{\beta \gamma}(A_\gamma)) = \bigcap_{\gamma \geq \beta} f_{\alpha \gamma}(A_\gamma);
$$

d’autre part, pour tout $\delta \geq \alpha$, il existe un $\gamma \in I$ tel que $\gamma \geq \delta$ et $\gamma \geq \beta$, donc $f_{\alpha \gamma}(A_\gamma) \subset f_{\alpha \delta}(A_\delta)$, et par suite $\bigcap_{\gamma \geq \beta} f_{\alpha \gamma}(A_\gamma) = \bigcap_{\delta \geq \alpha} f_{\alpha \delta}(A_\delta) = A'_\alpha$, ce qui achève d’établir que $\mathfrak{A}' \in \Sigma$. Comme $A'_\alpha \subset A_\alpha$ pour tout $\alpha$, l’hypothèse que $\mathfrak{A}$ est maximal dans $\Sigma$ entraîne $\mathfrak{A}' = \mathfrak{A}$, ce qui prouve notre assertion.

3° Montrons maintenant que si $\mathfrak{A} = (A_\alpha)$ est un élément *maximal* de $\Sigma$, chacun des $A_\alpha$ est *réduit à un élément*. Soit $x_\alpha \in A_\alpha$. Pour tout $\beta \geq \alpha$, posons $B_\beta = A_\beta \cap f^{-1}_{\alpha \beta}(x_\alpha)$; si l’on n’a pas $\beta \geq \alpha$, posons $B_\beta = A_\beta$; nous allons voir que $\mathfrak{B} = (B_\beta)$ appartient à $\Sigma$. Si l’on n’a pas $\beta \geq \alpha$, la relation $\beta \leq \gamma$ entraîne

$$
f_{\beta \gamma}(B_\gamma) \subset f_{\beta \gamma}(A_\gamma) \subset A_\beta = B_\beta; \text{ si au contraire } \alpha \leq \beta \leq \gamma, \text{ comme } f^{-1}_{\alpha \gamma}(x_\alpha) = f^{-1}_{\beta \gamma}(f_{\alpha \beta}(x_\alpha)), \text{ on a } f_{\beta \gamma}(f^{-1}_{\alpha \gamma}(x_\alpha)) \subset f^{-1}_{\alpha \beta}(x_\alpha), \text{ et comme } f_{\beta \gamma}(A_\gamma) \subset A_\beta, \text{ on a encore } f_{\beta \gamma}(B_\gamma) \subset B_\beta; \text{ la famille } \mathfrak{B} \text{ vérifie donc (21)}. $$

Comme $A_\alpha = f_{\alpha \beta}(A_\beta)$ pour $\alpha \leq \beta$ d’après 2°, il est clair que $B_\beta \neq \varnothing$ pour tout $\beta \in I$; enfin, en vertu de (i) et (iii), on a $B_\beta \in \mathcal{S}_\beta$ pour tout $\beta \in I$, ce qui achève de montrer que $\mathfrak{B} \in \Sigma$. Comme $B_\beta \subset A_\beta$ pour tout $\beta \in I$, l’hypothèse que $\mathfrak{A}$ est maximal entraîne $B_\beta = A_\beta$ pour tout $\beta$, et en particulier $A_\alpha = \{x_\alpha\}$.

4° Nous pouvons maintenant démontrer le th. 1. Prouvons d’abord *a)*. On sait que $f_\alpha(E) \subset \bigcap_{\beta \geq \alpha} f_{\alpha \beta}(E_\beta)$. Inversement, soit $x_\alpha \in \bigcap_{\beta \geq \alpha} f_{\alpha \beta}(E_\beta)$. Posons $B_\beta = f_{\alpha \beta}(x_\alpha)$ si $\beta \geq \alpha$, $B_\beta = E_\beta$ dans le cas contraire; par définition de $x_\alpha$, les $B_\beta$ ne sont pas vides et l’on a $B_\beta \in \mathcal{S}_\beta$ pour tout $\beta \in I$ en vertu de (iii) et de (i); en outre il est immédiat que $f_{\beta \gamma}(B_\gamma) \subset B_\beta$ pour $\beta \leq \gamma$. On a donc $\mathfrak{B} = (B_\beta) \in \Sigma$; soit $\mathfrak{A} = (A_\beta)$ un élément maximal de $\Sigma$ tel que $\mathfrak{A} \geq \mathfrak{B}$, élément dont l’existence résulte de 1° et de III, p. 21, cor. 1; comme, d’après 3°, $A_\beta$ est de la forme $\{y_\beta\}$ pour tout $\beta \in I$, $y = (y_\beta)$ appartient à $E$, et $f_\alpha(y) = y_\alpha = x_\alpha$ par définition.

Prouvons enfin que $a)$ entraîne $b)$. On peut en effet supposer $I$ non vide (sans quoi il n'y a rien à démontrer); l'hypothèse que les $E_\alpha$ sont non vides entraîne $f_{\alpha \beta}(E_\beta) \neq \varnothing$ pour $\beta \geq \alpha$; comme les $f_{\alpha \beta}(E_\beta)$, pour $\alpha$ fixé et $\beta \geq \alpha$, forment un ensemble filtrant décroissant de parties de $E_\alpha$ appartenant à $\mathfrak{S}_\alpha$, la condition (ii') prouve que $\bigcap_{\beta \geq \alpha} f_{\alpha \beta}(E_\beta) \neq \varnothing$. On a donc $f_\alpha(E) \neq \varnothing$ d'après $a)$, et $a$ fortiori $E \neq \varnothing$.

C.Q.F.D.

#### Remarque 1 {#ens-iii-s7-n4-rem-1 .statement tag=03OJ}

Supposons que dans l'énoncé du th. 1, on remplace la condition (iii) par la condition plus faible suivante:

(iii') *Pour tout $\alpha \in I$, et tout ensemble non vide $M_\alpha \in \mathfrak{S}_\alpha$, il existe $x_\alpha \in M_\alpha$ tel que $f_{\alpha \beta}^{-1}(x_\alpha) \in \mathfrak{S}_\beta$ pour tout $\beta \geq \alpha$.*

Alors la conclusion $b)$ du th. 1 est encore valable. En effet, les démonstrations des parties 1° et 2° du th. 1 sont inchangées; la démonstration de la partie 3° reste valable en ayant soin de prendre $x_\alpha \in A_\alpha$ tel que $f_{\alpha \beta}^{-1}(x_\alpha)$ appartienne à $\mathfrak{S}_\beta$ pour $\beta \geq \alpha$. Enfin, le raisonnement de 4° montre que si $\bigcap_{\beta \geq \alpha} f_{\alpha \beta}(E_\beta) \neq \varnothing$ et si on prend dans cet ensemble un $x_\alpha$ tel que $f_{\alpha \beta}^{-1}(x_\alpha) \in \mathfrak{S}_\beta$ pour $\beta \geq \alpha$, il existe $y \in E$ tel que $f_\alpha(y) = x_\alpha$, ce qui établit notre assertion.

Exemples

I) Si les $E_\alpha$ sont des ensembles *finis*, on peut appliquer le th. 1 en prenant pour $\mathfrak{S}_\alpha$ l'ensemble de *toutes* les parties de $E_\alpha$. *Cet exemple sera généralisé en Topologie générale au cas où les $E_\alpha$ sont des espaces *compacts*, les $f_{\alpha \beta}$ des applications *continues*, et $\mathfrak{S}_\alpha$ l'ensemble des parties *fermées* de $E_\alpha$ (TG, I, § 9, n° 6).*

*II) Soient $A$ un anneau, et pour chaque $\alpha \in I$, soit $T_\alpha$ un $A$-module à gauche *artinien* (A, VIII, § 2, n° 1); soit $E_\alpha$ un *espace homogène* sur $T_\alpha$ dans lequel $T_\alpha$ opère fidèlement (de sorte que l'on peut dire que $E_\alpha$ est un *espace affine* attaché à $T_\alpha$ (A, II, § 9, n° 1)). Pour $\beta \geq \alpha$, supposons que $f_{\alpha \beta}: E_\beta \to E_\alpha$ soit une *application affine* (A, II, § 9, n° 4). Prenons pour $\mathfrak{S}_\alpha$ l'ensemble formé de la partie vide et des *variétés linéaires affines* de $E_\alpha$ (A, II, § 9, n° 3). Alors la condition (i) est trivialement vérifiée, et la condition (ii) résulte de ce que $T_\alpha$ est artinien: cela entraîne en effet l'existence d'un élément minimal parmi les intersections finies d'ensembles $M \in \mathfrak{F}$, et cet élément est nécessairement égal à $\bigcap_{M \in \mathfrak{F}} M$. Enfin, comme $f_{\alpha \beta}$ est affine, les conditions (iii) et (iv) sont trivialement vérifiées.*

### 5. Limites inductives

Soient $I$ un ensemble préordonné *filtrant à droite*, $(E_\alpha)_{\alpha \in I}$ une famille d'ensembles ayant $I$ pour ensemble d'indices. Pour tout couple $(\alpha, \beta)$ d'indices de $I$ tels que α ≤ β, soit $f_{βα}$ une application de $E_α$ dans $E_β$. On suppose que les $f_{βα}$ vérifient les conditions suivantes:
(LI_I) Les relations $α ≤ β ≤ γ$ entraînent $f_{γα} = f_{γβ} \circ f_{βα}$.
(LI_II) Pour tout $α ∈ I$, $f_{αα}$ est l’application identique de $E_α$.

Soit G l’ensemble somme de la famille d’ensembles $(E_α)_{α ∈ I}$ (II, p. 30); par abus de langage, nous identifierons les $E_α$ aux parties de G qui en sont les images canoniques, et forment une partition de G; pour tout $x ∈ G$, nous désignerons par $λ(x)$ l’unique indice $α ∈ I$ tel que $x ∈ E_α$. Soir $R\{x, y\}$ la relation suivante entre deux éléments $x, y$ de G:
« il existe un élément $γ ∈ I$ tel que $γ ≥ α = λ(x)$ et $γ ≥ β = λ(y)$, et pour lequel on a $f_{γα}(x) = f_{γβ}(y)$ »;
montrons que R est une relation d’équivalence dans G. Il est évident que R est symétrique et réflexive dans G; reste à voir qu’elle est transitive. Or, soient $x ∈ E_α$, $y ∈ E_β$, $z ∈ E_γ$; supposons qu’il existe $λ ∈ I$ tel que $λ ≥ α$, $λ ≥ β$, et $f_{λα}(x) = f_{λβ}(y)$, et $μ ∈ I$ tel que $μ ≥ β$, $μ ≥ γ$ et $f_{μβ}(y) = f_{μγ}(z)$. Comme I est filtrant, il existe $ν ∈ I$ tel que $ν ≥ λ$ et $ν ≥ μ$; en vertu de (LI_I), on a alors
$$
f_{να}(x) = f_{νλ}(f_{λα}(x)) = f_{νλ}(f_{λβ}(y)) = f_{νβ}(y)
= f_{νμ}(f_{μβ}(y)) = f_{νμ}(f_{μγ}(z)) = f_{νγ}(z)
$$
ce qui établit notre assertion.

On dit que l’ensemble quotient $E = G/R$ est la limite inductive de la famille $(E_α)_{α ∈ I}$ pour la famille d’applications $(f_{βα})$, et on écrit $E = \lim \rightarrow (E_α, f_{βα})$, ou simplement $E = \lim \rightarrow E_α$ si aucune confusion n’en résulte. Par abus de langage, on dira que le couple $((E_α), (f_{βα}))$ (que l’on notera aussi $(E_α, f_{βα})$) est un système inductif d’ensembles, relatif à l’ensemble filtrant I.

Il est clair que E n’est pas vide si un au moins des $E_α$ n’est pas vide. Nous désignerons par $f_α$ la restriction à $E_α$ de l’application canonique $f$ de G sur $E = G/R$, et nous dirons que $f_α$ est l’application canonique de $E_α$ dans E. Pour $α ≤ β$, on a la relation
(22)
$$
f_β \circ f_{βα} = f_α ;
$$
en effet, pour tout $x ∈ E_α$, on a $f_{ββ}(f_{βα}(x)) = f_{βα}(x)$ en vertu de (LI_I), donc les éléments $x ∈ E_α$ et $f_{βα}(x) ∈ E_β$ sont congrus mod. R, ce qui démontre (22).

#### Exemple 1 {#ens-iii-s7-n5-exa-1 .statement tag=03TM}

Soient A, B deux ensembles, $(V_α)_{α ∈ I}$ une famille de parties de A, dont l’ensemble d’indices I est filtrant à droite, telle que la relation $α ≤ β$ entraîne $V_β ⊂ V_α$. Désignons par $E_α$ l’ensemble des applications de $V_α$ dans B; pour tout couple d’indices $α, β$ tels que $α ≤ β$, soit $f_{βα}$ l’application de $E_α$ dans $E_β$ qui à toute fonction $u ∈ E_α$ fait correspondre sa restriction $f_{βα}(u)$ à $V_β$. Il est immédiat que les conditions (LI_I) et (LI_II) sont vérifiées; on dit que l’ensemble $E = \lim \rightarrow E_α$ est l’ensemble des germes d’applications des $V_α$ dans B. *Le cas le plus fréquent est celui où $(V_α)$ est la famille des voisinages d’une partie d’un espace topologique A (TG, I, § 6, n° 10).*
2) Supposons que pour tout $α ∈ I$, $E_α$ soit égal à un ensemble F et que pour $α ≤ β$, $g_{βα}$ soit l’application identique de F sur lui-même. Alors il existe une bijection canonique de $\lim$ $E_\alpha$ sur $F$: en effet, pour définir $\lim$ $E_\alpha$, on doit former l’ensemble $G$ somme de la famille $(E_\alpha)$; $G$ est donc réunion d’une famille $(G_\alpha)$ d’ensembles deux à deux disjoints, et pour tout $\alpha \in I$, il y a une bijection canonique $h_\alpha : F \to G_\alpha$. On doit ensuite considérer la relation d’équivalence $R$ dans $G$, correspondant à la partition $(P_y)_{y \in F}$, où $P_y$ est l’ensemble des $h_\alpha(y)$ lorsque $\alpha$ parcourt $I$. Il est clair que $y \mapsto P_y$ est une bijection, dont la bijection réciproque est la bijection cherchée; on identifiera $F$ à $\lim$ $E_\alpha$ au moyen de cette bijection canonique.

#### Lemme 1 {#ens-iii-s7-lem-1 .statement tag=03OK}

Soient $(E_\alpha, f_{\beta \alpha})$ un système inductif d’ensembles, $E = \lim$ $E_\alpha$ sa limite inductive, et pour tout $\alpha \in I$, soit $f_\alpha : E_\alpha \to E$ l’application canonique.

(i) Soit $(x^{(i)})_{1 \leq i \leq n}$ un système fini d’éléments de $E$. Il existe un $\alpha \in I$ et un système fini $(x_\alpha^{(i)})_{1 \leq i \leq n}$ d’éléments de $E_\alpha$ tels que $x^{(i)} = f_\alpha(x_\alpha^{(i)})$ pour $1 \leq i \leq n$.

(ii) Soit $(y_\alpha^{(i)})_{1 \leq i \leq n}$ un système fini d’éléments d’un $E_\alpha$; si $f_\alpha(y_\alpha^{(i)}) = f_\alpha(y_\alpha^{(j)})$ pour tout couple d’indices $(i, j)$, il existe un $\beta \geq \alpha$ tel que $f_{\beta \alpha}(y_\alpha^{(i)}) = f_{\beta \alpha}(y_\alpha^{(j)})$ pour tout couple $(i, j)$.

(i) Par définition de $E$, il existe pour chaque $i$ un $\beta_i \in I$ et un élément $z_{\beta_i} \in E_{\beta_i}$ tel que $x^{(i)} = f_{\beta_i}(z_{\beta_i})$; il suffit de prendre $\alpha$ tel que $\alpha \geq \beta_i$ pour $1 \leq i \leq n$, et $x_\alpha^{(i)} = f_{\alpha \beta_i}(z_{\beta_i})$.

(ii) Par définition de $E$, pour tout couple $(i, j)$ il existe $\gamma_{ij} \in I$ tel que $\gamma_{ij} \geq \alpha$ et que $f_{\gamma_{ij} \alpha}(y_\alpha^{(i)}) = f_{\gamma_{ij} \alpha}(y_\alpha^{(j)})$; il suffit de prendre $\beta$ tel que $\beta \geq \gamma_{ij}$ pour tous les couples $(i, j)$, et d’utiliser les relations $f_{\beta \alpha} = f_{\beta \gamma_{ij}} \circ f_{\gamma_{ij} \alpha}$.

### 6. Systèmes inductifs d’applications

#### Proposition 6 {#ens-iii-s7-prop-6 .statement tag=03RR}

Soient $I$ un ensemble préordonné filtrant à droite, $(E_\alpha, f_{\beta \alpha})$ un système inductif d’ensembles, $E = \lim$ $E_\alpha$ sa limite inductive, et pour tout $\alpha \in I$, soit $f_\alpha : E_\alpha \to E$ l’application canonique. Pour tout $\alpha \in I$, soit $u_\alpha$ une application de $E_\alpha$ dans un ensemble $F$ telle que l’on ait

$$
u_\beta \circ f_{\beta \alpha} = u_\alpha \tag{23}
$$

pour $\alpha \leq \beta$.

Dans ces conditions:

1° Il existe une application $u$ et une seule de $E$ dans $F$ telle que

$$
u_\alpha = u \circ f_\alpha \tag{24}
$$

pour tout $\alpha \in I$.

2° Pour que $u$ soit surjective, il faut et il suffit que $F$ soit réunion des $u_\alpha(E_\alpha)$.

3° Pour que $u$ soit injective, il faut et suffit que, pour tout $\alpha \in I$, les relations $x \in E_\alpha, y \in E_\alpha, u_\alpha(x) = u_\alpha(y)$ entraînent qu’il existe $\beta \geq \alpha$ pour lequel $f_{\beta \alpha}(x) = f_{\beta \alpha}(y)$.

1° Avec les notations du no 5, soit $v$ l’application de l’ensemble somme $G$ dans $F$ qui coïncide avec $u_\alpha$ dans chaque $E_\alpha$ (II, p. 29, prop. 8). L’hypothèse entraîne que $v$ est compatible avec la relation d’équivalence $R$ (II, p. 44); donc il existe une application $u$ et une seule de $E = G/R$ dans $F$ telle que $v = u \circ f$ (loc. cit.).

2° Comme $E$ est réunion des $f_\alpha(E_\alpha)$, la relation $F = \bigcup_{\alpha \in I} u_\alpha(E_\alpha)$ est évidemment nécessaire et suffisante pour que $u$ soit surjective.

3° En vertu du lemme 1 (III, p. 62), deux éléments quelconques de E peuvent toujours s’écrire sous la forme $f_\alpha(x)$ et $f_\alpha(y)$, où $x \in E_\alpha$ et $y \in E_\alpha$, pour un $\alpha \in I$ convenable; il résulte aussi de ce lemme que la relation $f_\alpha(x) = f_\alpha(y)$ est équivalente à l’existence de $\beta \geq \alpha$ tel que $f_{\beta \alpha}(x) = f_{\beta \alpha}(y)$; comme $u_\alpha(x) = u(f_\alpha(x))$ et $u_\alpha(y) = u(f_\alpha(y))$, cela achève la démonstration.

Lorsque l’application $u$ est *bijective*, on dit parfois, par abus de langage, que F est la limite inductive de la famille $(E_\alpha)$.

*Remarque 1).* — Supposons que chacune des applications $f_{\beta \alpha}$ soit *injective*; alors chacune des applications $f_\alpha$ est *injective* en vertu de la définition de la relation R. On identifie alors en général $E_\alpha$ et $f_\alpha(E_\alpha)$, et on considère donc E comme la *réunion* des $E_\alpha$. Inversement, soit $(F_\alpha)_{\alpha \in I}$ une famille croissante de parties d’un ensemble F, et supposons que F soit *réunion* de cette famille; si $j_{\beta \alpha}$ désigne l’injection canonique de $F_\alpha$ dans $F_\beta$ pour $\alpha \leq \beta$, il résulte de la prop. 6 que l’on peut identifier F à la limite inductive de la famille $(F_\alpha)$ pour la famille d’applications $(j_{\beta \alpha})$, et les applications canoniques des $F_\alpha$ dans $\lim \rightarrow F_\alpha$ aux injections canoniques des $F_\alpha$ dans F.

#### Corollaire 1 {#ens-iii-s7-prop-6-cor-1 .statement tag=03RS}

*Soient* $(E_\alpha, f_{\beta \alpha})$ *et* $(F_\alpha, g_{\beta \alpha})$ *deux systèmes inductifs d’ensembles relatifs à un même ensemble d’indices I; soient* $E = \lim \rightarrow E_\alpha$, $F = \lim \rightarrow F_\alpha$, *et pour tout* $\alpha \in I$, *soit* $f_\alpha$ *(resp. $g_\alpha$)* *l’application canonique de* $E_\alpha$ *dans* E *(resp. de* $F_\alpha$ *dans* F*).* *Pour tout* $\alpha \in I$, *soit* $u_\alpha$ *une application de* $E_\alpha$ *dans* $F_\alpha$ *telle que, pour* $\alpha \leq \beta$, *le diagramme*

$$
\begin{array}{ccc}
E_\alpha & \xrightarrow{u_\alpha} & F_\alpha \\
f_{\beta \alpha} \downarrow & & g_{\beta \alpha} \downarrow \\
E_\beta & \xrightarrow{u_\beta} & F_\beta
\end{array}
$$

*soit commutatif.* *Il existe alors une application* $u : E \to F$ *et une seule telle que, pour tout* $\alpha \in I$, *le diagramme*

$$
\begin{array}{ccc}
E_\alpha & \xrightarrow{u_\alpha} & F_\alpha \\
f_\alpha \downarrow & & g_\alpha \downarrow \\
E & \xrightarrow{u} & F
\end{array}
$$

*soit commutatif.*

Posons $v_\alpha = g_\alpha \circ u_\alpha$. Pour $\alpha \leq \beta$, on a, d’après (22),

$$
v_\beta \circ f_{\beta \alpha} = g_\beta \circ u_\beta \circ f_{\beta \alpha} = g_\beta \circ g_{\beta \alpha} \circ u_\alpha = g_\alpha \circ u_\alpha = v_\alpha.
$$

On peut donc appliquer la prop. 6 aux $v_\alpha$, d’où l’existence et l’unicité d’une application $u : E \to F$ telle que

$$
u \circ f_\alpha = v_\alpha = g_\alpha \circ u_\alpha
$$

pour tout $\alpha \in I$.

On dit qu’une famille d’applications $u_\alpha : E_\alpha \to F_\alpha$ satisfaisant aux conditions du cor. 1 est un *système inductif d’applications* de $(E_\alpha, f_{\beta \alpha})$ dans $(F_\alpha, g_{\beta \alpha})$; l’application définie dans le cor. 1 est appelée la *limite inductive* de la famille $(u_\alpha)$ et se note $u = \lim \rightarrow u_\alpha$ lorsque aucune confusion n’est à craindre.

#### Corollaire 2 {#ens-iii-s7-prop-6-cor-2 .statement tag=03RT}

Soient $(E_\alpha, f_{\beta\alpha})$, $(F_\alpha, g_{\beta\alpha})$, $(G_\alpha, h_{\beta\alpha})$ trois systèmes inductifs d’ensembles relatifs à $I$; soient $E = \lim E_\alpha$, $F = \lim F_\alpha$, $G = \lim G_\alpha$, et soit $f_\alpha$ (resp. $g_\alpha, h_\alpha$) l’application canonique de $E_\alpha$ (resp. $F_\alpha, G_\alpha$) dans $E$ (resp. $F, G$). Si $(u_\alpha)$ et $(v_\alpha)$ sont deux systèmes inductifs d’applications $u_\alpha : E_\alpha \to F_\alpha$, $v_\alpha : F_\alpha \to G_\alpha$, alors les $v_\alpha \circ u_\alpha : E_\alpha \to G_\alpha$ forment un système inductif d’applications, et on a

$$
\lim (v_\alpha \circ u_\alpha) = (\lim v_\alpha) \circ (\lim u_\alpha).
$$

En effet, si on pose $w_\alpha = v_\alpha \circ u_\alpha$, on a pour $\alpha \leq \beta$

$$
h_{\beta\alpha} \circ w_\alpha = (h_{\beta\alpha} \circ v_\alpha) \circ u_\alpha = (v_\beta \circ g_{\beta\alpha}) \circ u_\alpha = v_\beta \circ (u_\beta \circ f_{\beta\alpha}) = w_\beta \circ f_{\beta\alpha}
$$

ce qui montre que $(w_\alpha)$ est un système inductif d’applications. En outre, si on pose $u = \lim u_\alpha$, $v = \lim v_\alpha$, on a, pour tout $\alpha \in I$,

$$
(v \circ u) \circ f_\alpha = v \circ (g_\alpha \circ u_\alpha) = h_\alpha \circ (v_\alpha \circ u_\alpha)
$$

et en raison de l’unicité de la limite inductive, on a $v \circ u = \lim w_\alpha$.

#### Proposition 7 {#ens-iii-s7-prop-7 .statement tag=03RU}

Soient $(E_\alpha, f_{\beta\alpha})$, $(E'_\alpha, f'_{\beta\alpha})$ deux systèmes inductifs d’ensembles relatifs à $I$, et pour chaque $\alpha \in I$, soit $u_\alpha$ une application de $E_\alpha$ dans $E'_\alpha$, les $u_\alpha$ formant un système inductif d’applications. Soit $u = \lim u_\alpha$. Si chacune des $u_\alpha$ est injective (resp. surjective), alors $u$ est injective (resp. surjective).

Soient $E = \lim E_\alpha$, $E' = \lim E'_\alpha$, et $f_\alpha : E_\alpha \to E$, $f'_\alpha : E'_\alpha \to E'$ les applications canoniques. Supposons les $u_\alpha$ injectives; pour vérifier que $u$ est injective, il suffit (III, p. 62, prop. 6) de vérifier que si $x \in E_\alpha$, $y \in E_\alpha$ sont tels que $f'_\alpha(u_\alpha(x)) = f'_\alpha(u_\alpha(y))$, alors il existe $\beta \geq \alpha$ tel que $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$. Or l’hypothèse implique (III, p. 62, lemme 1) qu’il existe $\beta \geq \alpha$ tel que $f'_{\beta\alpha}(u_\alpha(x)) = f'_{\beta\alpha}(u_\alpha(y))$, ce qui s’écrit aussi $u_\beta(f_{\beta\alpha}(x)) = u_\beta(f_{\beta\alpha}(y))$, et entraîne donc $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$ puisque $u_\beta$ est injective.

Supposons maintenant les $u_\alpha$ surjectives; on a alors

$$
E' = \bigcup_\alpha f'_\alpha(E'_\alpha) = \bigcup_\alpha f'_\alpha(u_\alpha(E_\alpha))
= \bigcup_\alpha u(f_\alpha(E_\alpha)) = u(\bigcup_\alpha f_\alpha(E_\alpha)) = u(E).
$$

Avec les notations de la prop. 7, soit, pour tout $\alpha \in I$, $M_\alpha$ une partie de $E_\alpha$; si l’on a $f_{\beta\alpha}(M_\alpha) \subset M_\beta$ pour $\alpha \leq \beta$, on dit que $(M_\alpha)_{\alpha \in I}$ est un système inductif de parties des $E_\alpha$. Soit $g_{\beta\alpha}$ l’application de $M_\alpha$ dans $M_\beta$ (pour $\alpha \leq \beta$) ayant même graphe que la restriction de $f_{\beta\alpha}$ à $M_\alpha$; il est clair que $(M_\alpha, g_{\beta\alpha})$ est un système inductif d’ensembles, et la prop. 7, appliquée aux injections canoniques $j_\alpha : M_\alpha \to E_\alpha$, permet d’identifier $M = \lim M_\alpha$ à une partie de $E$ au moyen de l’injection $j = \lim j_\alpha$.

#### Corollaire {#ens-iii-s7-n6-cor-1 .statement tag=03ON}

Soient $(E_\alpha, f_{\beta\alpha})$, $(E'_\alpha, f'_{\beta\alpha})$ deux systèmes inductifs d’ensembles, $(u_\alpha)$ un système inductif d’applications $u_\alpha : E_\alpha \to E'_\alpha$, et soit $u = \lim u_\alpha$.

(i) Soit $(M_\alpha)$ un système inductif de parties des $E_\alpha$. Alors $(u_\alpha(M_\alpha))$ est un système inductif de parties des $E'_\alpha$, et on a
$$
\lim u_\alpha(M_\alpha) = u(\lim M_\alpha).
$$
(ii) Soit $(a'_\alpha)_{\alpha \in I}$ une famille telle que l’on ait $a'_\alpha \in E'_\alpha$ pour tout $\alpha \in I$ et $f'_{\beta \alpha}(a'_\alpha) = a'_\beta$ pour $\alpha \leq \beta$. Alors les ensembles $\bar{u}_\alpha^{-1}(a'_\alpha)$ forment un système inductif de parties des $E_\alpha$, et l’on a
$$
\lim \bar{u}_\alpha^{-1}(a'_\alpha) = \bar{u}^{-1}(a')
$$
en désignant par $a'$ l’unique élément de $\lim E'_\alpha$ image canonique de $a'_\alpha$ pour tout $\alpha \in I$.

(i) Il est immédiat que les $u_\alpha(M_\alpha)$ forment un système inductif de parties des $E'_\alpha$, et on peut écrire $u_\alpha(M_\alpha) = v_\alpha(M_\alpha)$, où $v_\alpha$ est l’application de $M_\alpha$ sur $u_\alpha(M_\alpha)$ dont le graphe coïncide avec celui de la restriction de $u_\alpha$ à $M_\alpha$. La relation (26) résulte alors de la prop. 7, puisque les $v_\alpha$ sont surjectives.

(ii) Soit $N_\alpha = u_\alpha^{-1}(a'_\alpha)$; si $\alpha \leq \beta$ et si $x_\alpha \in N_\alpha$, on a $u_\beta(f_{\beta \alpha}(x_\alpha)) = f'_{\beta \alpha}(u_\alpha(x_\alpha)) = f'_{\beta \alpha}(a'_\alpha) = a'_\beta$, donc $f_{\beta \alpha}(x_\alpha) \in N_\beta$, et les $N_\alpha$ forment un système inductif de parties des $E_\alpha$. Avec les notations de la démonstration de la prop. 7, considérons un élément $x \in \lim N_\alpha$; il existe donc un $\alpha \in I$ et un $x_\alpha \in N_\alpha$ tels que $x = f_\alpha(x_\alpha)$, d’où $u(x) = u(f_\alpha(x_\alpha)) = f'_\alpha(u_\alpha(x_\alpha)) = f'_\alpha(a'_\alpha) = a'$. Réciproquement, si $x \in \bar{u}^{-1}(a')$ et si $x = f_\alpha(x_\alpha)$ pour un $\alpha \in I$ et un $x_\alpha \in E_\alpha$, on a $f'_\alpha(a'_\alpha) = a' = u(f_\alpha(x_\alpha)) = f'_\alpha(u_\alpha(x_\alpha))$; donc (III, p. 62, lemme 1), il existe $\beta \geq \alpha$ tel que $f'_{\beta \alpha}(u_\alpha(x_\alpha)) = f'_{\beta \alpha}(a'_\alpha) = a'_\beta$; ceci s’écrit aussi $u_\beta(f_{\beta \alpha}(x_\alpha)) = a'_\beta$, donc $f_{\beta \alpha}(x_\alpha) \in N_\beta$; comme $x = f_\beta(f_{\beta \alpha}(x_\alpha))$, on a bien $x \in \lim N_\alpha$.

Remarque 2). — Supposons que pour tout $\alpha \in I$, $u_\alpha : E_\alpha \to E'$ soit une application telle que la famille $(u_\alpha)$ vérifie (23). Considérons le système inductif $(E'_\alpha, i_{\beta \alpha})$ relatif à $I$, où $E'_\alpha = E'$ pour tout $\alpha \in I$ et $i_{\beta \alpha}$ est l’application identique de $E'$. On sait alors (III, p. 61, Exemple 2) que $E'$ s’identifie canoniquement à $\lim E_\alpha$. Si on considère $u_\alpha$ comme application de $E_\alpha$ dans $E'$, $(u_\alpha)$ est un système inductif d’applications, et l’application $u : E \to E'$ définie par (24) s’identifie à la limite inductive de ce système d’applications. Aussi écrit-on alors par abus de langage $u = \lim u_\alpha$.

Pour toute partie $J$ de $I$, filtrante à droite (pour le préordre induit), il est clair que le couple formé de la sous-famille $(E_\alpha)_{\alpha \in J}$ et de la famille $(f_{\beta \alpha})$, où $\alpha \leq \beta$, $\alpha \in J$ et $\beta \in J$, est encore un système inductif d’ensembles, relatif à $J$; on dira qu’il est obtenu par restriction à $J$ de l’ensemble d’indices. Notons par $E$ et $E'$ les limites inductives des familles $(E_\alpha)_{\alpha \in I}$ et $(E_\alpha)_{\alpha \in J}$ respectivement, et pour tout $\alpha \in I$, soit $f_\alpha : E_\alpha \to E$ l’application canonique; alors $(f_\alpha)_{\alpha \in J}$ est un système inductif d’applications, et par suite $g = \lim f_\alpha$ est un application $E' \to E$, dite canonique.

En outre, si $J'$ est une partie filtrante de $J$, $E''$ la limite inductive de la famille $(E_\alpha)_{\alpha \in J''}$, $g': E'' \to E'$ et $g'': E'' \to E$ les applications canoniques, il résulte aussitôt de la prop. 6 que l’on a

$$
g'' = g \circ g'.
$$

#### Proposition 8 {#ens-iii-s7-prop-8 .statement tag=03OP}

*Soient I un ensemble préordonné filtrant à droite, $(E_\alpha, f_{\beta \alpha})$ un système inductif d’ensembles relatif à I, $E = \lim_{\longrightarrow} E_\alpha$ sa limite inductive. Soient J une partie cofinale de I, $E'$ la limite inductive du système inductif d’ensembles obtenu à partir de $(E_\alpha, f_{\beta \alpha})$ par restriction à J de l’ensemble d’indices. Alors l’application canonique de $E'$ dans $E$ est bijective.*

On sait que J est nécessairement filtrant à droite (III, p. 13). Vérifions les critères de la prop. 6 (III, p. 62) pour montrer que g est bijective. La condition d’injectivité découle aussitôt de la définition et du lemme 1 (III, p. 62). Pour voir que g est surjective, remarquons que pour tout $\alpha \in J$, on a $g(E_\alpha) = f_\alpha(E_\alpha)$. Or, pour tout $\beta \in I$, il existe $\gamma \in J$ tel que $\beta \leq \gamma$, d’où on conclut que $g(E_\gamma) \supset g(f_{\gamma \beta}(E_\beta)) = f_\beta(E_\beta)$; E est donc bien réunion des $g(E_\alpha)$ lorsque $\alpha$ parcourt J.

### 7. Double limite inductive. Produit de limites inductives

Soient I, L deux ensembles préordonnés filtrants à droite, $I \times L$ leur produit (III, p. 7) qui est filtrant à droite. Considérons un système inductif d’ensembles $(E^\lambda_\alpha, f^{\mu \lambda}_{\beta \alpha})$ relatif à $I \times L$; on a donc

$$
f^{\nu \lambda}_{\gamma \alpha} = f^{\nu \mu}_{\gamma \beta} \circ f^{\mu \lambda}_{\beta \alpha} \quad \text{pour } \alpha \leq \beta \leq \gamma \text{ et } \lambda \leq \mu \leq \nu.
$$

Désignons par E ou $\lim_{\longrightarrow} E^\lambda_\alpha$ la limite inductive de ce système inductif. Pour tout $\lambda \in L$, posons $g^{\lambda}_{\beta \alpha} = f^{\lambda \lambda}_{\beta \alpha}: E^\lambda_\alpha \to E^\lambda_\beta$; il résulte de (29) que l’on a

$$
g^{\lambda}_{\gamma \alpha} = g^{\lambda}_{\gamma \beta} \circ g^{\lambda}_{\beta \alpha} \quad \text{pour } \alpha \leq \beta \leq \gamma;
$$
autrement dit, $(E^\lambda_\alpha, g^{\lambda}_{\beta \alpha})$ est un système inductif d’ensembles relatif à I; notons $F^\lambda = \lim_{\longrightarrow} E^\lambda_\alpha$ sa limite inductive. D’autre part, pour $\lambda \leq \mu$ fixés dans L, il résulte de (29) que les $h^{\mu \lambda}_{\alpha} = f^{\mu \lambda}_{\alpha \alpha}: E^\lambda_\alpha \to E^\mu_\alpha$ forment un système inductif d’applications; nous noterons $h^{\mu \lambda} = \lim_{\longrightarrow} h^{\mu \lambda}_{\alpha}: F^\lambda \to F^\mu$ sa limite inductive. Pour $\lambda \leq \mu \leq \nu$ dans L, on a alors

$$
h^{\nu \lambda} = h^{\nu \mu} \circ h^{\mu \lambda}
$$
(III, p. 64, cor. 2); donc $(F^\lambda, h^{\mu \lambda})$ est un système inductif d’ensembles relatif à L. Soit $F = \lim_{\longrightarrow} F^\lambda$ sa limite inductive; nous allons définir une *bijection canonique* $E \to F$. Notons $g^\lambda_\alpha$ l’application canonique $E^\lambda_\alpha \to F^\lambda$, et $h^\lambda$ l’application canonique $F^\lambda \to F$, et posons $u^\lambda_\alpha = h^\lambda \circ g^\lambda_\alpha$. Pour $\alpha \leq \beta$ et $\lambda \leq \mu$, on a

$$
u^\mu_\beta \circ f^{\mu \lambda}_{\beta \alpha} = h^\mu \circ g^\mu_\beta \circ f^{\mu \lambda}_{\beta \alpha} = h^\mu \circ g^\mu_\beta \circ f^{\mu \mu}_{\beta \alpha} \circ f^{\mu \lambda}_{\alpha \alpha} = h^\mu \circ g^\mu_\alpha \circ f^{\mu \lambda}_{\alpha \alpha}
$$
$$
= h^\mu \circ h^{\mu \lambda} \circ g^\lambda_\alpha = h^\lambda \circ g^\lambda_\alpha = u^\lambda_\alpha
$$

en vertu de (29) et de la définition de $h^{\mu\lambda}$; les $u_\alpha^\lambda$ forment donc un système inductif d'applications relatif à $I \times L$. Posons $u = \lim_{\alpha, \lambda} u_\alpha^\lambda : E \to F$, et montrons que $u$ est bijective en appliquant les critères de III, p. 62, prop. 6. En premier lieu, $F$ est réunion des $h^\lambda(F^\lambda)$, et chaque $F^\lambda$ est réunion des $g_\alpha^\lambda(E_\alpha^\lambda)$; donc $F$ est réunion des $h^\lambda(g_\alpha^\lambda(E_\alpha^\lambda)) = u_\alpha^\lambda(E_\alpha^\lambda)$. D'autre part, soient $x, y$ deux éléments de $E_\alpha^\lambda$ tels que $u_\alpha^\lambda(x) = u_\alpha^\lambda(y)$, autrement dit $h^\lambda(g_\alpha^\lambda(x)) = h^\lambda(g_\alpha^\lambda(y))$; il existe alors un $\mu \geq \lambda$ tel que $h^{\mu\lambda}(g_\alpha^\lambda(x)) = h^{\mu\lambda}(g_\alpha^\lambda(y))$ (III, p. 62, lemme 1), c'est-à-dire $g_\alpha^\mu(f_{\alpha\alpha}^{\mu\lambda}(x)) = g_\alpha^\mu(f_{\alpha\alpha}^{\mu\lambda}(y))$; de même il existe $\beta \geq \alpha$ tel que $g_{\beta\alpha}^\mu(f_{\alpha\alpha}^{\mu\lambda}(x)) = g_{\beta\alpha}^\mu(f_{\alpha\alpha}^{\mu\lambda}(y))$ (III, p. 62, lemme 1), c'est-à-dire $f_{\beta\alpha}^{\mu\lambda}(x) = f_{\beta\alpha}^{\mu\lambda}(y)$; cela montre (III, p. 62, prop. 6) que $u$ est injective. Nous avons donc démontré la proposition suivante:

#### Proposition 9 {#ens-iii-s7-prop-9 .statement tag=03RV}

*Si* $(E_\alpha^\lambda, f_{\beta\alpha}^{\mu\lambda})$ *est un système inductif d'ensembles relatif à un produit* $I \times L$ *de deux ensembles préordonnés filtrants à droite, on a, à une bijection canonique près,* (32)
$$
\lim_{\alpha, \lambda} E_\alpha^\lambda = \lim_{\lambda} (\lim_{\alpha} E_\alpha^\lambda).
$$

#### Corollaire {#ens-iii-s7-n7-cor-1 .statement tag=03OQ}

*Soit* $(E'_\alpha, {f'}_{\beta\alpha}^{\mu\lambda})$ *un second système inductif d'ensembles relatif à* $I \times L$, *et, pour chaque* $(\alpha, \lambda)$ *soit* $u_\alpha^\lambda$ *une application de* $E_\alpha^\lambda$ *dans* $E'_\alpha$, *les* $u_\alpha^\lambda$ *formant un système inductif d'applications. On a alors*
(33)
$$
\lim_{\alpha, \lambda} u_\alpha^\lambda = \lim_{\lambda} (\lim_{\alpha} u_\alpha^\lambda).
$$
Nous laissons la vérification au lecteur.

#### Proposition 10 {#ens-iii-s7-prop-10 .statement tag=03RW}

*Soient* $(E_\alpha, f_{\beta\alpha}), (E'_\alpha, f'_{\beta\alpha})$ *deux systèmes inductifs d'ensembles relatifs à un même ensemble d'indices préordonné filtrant à droite* $I$; *soient* $E = \lim_{\longrightarrow} E_\alpha$, $E' = \lim_{\longrightarrow} E'_\alpha$, *et désignons par* $f_\alpha : E_\alpha \to E$ *et* $f'_\alpha : E'_\alpha \to E'$ *(pour* $\alpha \in I$) *les applications canoniques.* *Alors* $(E_\alpha \times E'_\alpha, f_{\beta\alpha} \times f'_{\beta\alpha})$ *est un système inductif d'ensembles*, $(f_\alpha \times f'_\alpha)$ *est un système inductif d'applications, et* $\lim_{\longrightarrow} (f_\alpha \times f'_\alpha)$ *est un bijection*
(34)
$$
\lim_{\longrightarrow} (E_\alpha \times E'_\alpha) \to (\lim_{\longrightarrow} E_\alpha) \times (\lim_{\longrightarrow} E'_\alpha).
$$
La vérification des deux premières assertions est immédiate, et pour voir que $g = \lim_{\longrightarrow} (f_\alpha \times f'_\alpha)$ est bijective, nous allons appliquer la prop. 6 de III, p. 62. Il est clair que $E \times E'$ est réunion des $f_\alpha(E_\alpha) \times f'_\alpha(E'_\alpha)$, donc $g$ est surjective. D'autre part, si $(x, x')$ et $(y, y')$ sont deux éléments de $E_\alpha \times E'_\alpha$ tels que $f_\alpha(x) = f_\alpha(y)$ et $f'_\alpha(x') = f'_\alpha(y')$, il existe (III, p. 62, lemme 1) deux éléments $\beta \geq \alpha$, $\gamma \geq \alpha$ de $I$ tels que $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$ et $f'_{\gamma\alpha}(x') = f'_{\gamma\alpha}(y')$; comme $I$ est filtrant, il existe un $\delta \in I$ tel que $\delta \geq \beta$ et $\delta \geq \gamma$, d'où $f_{\delta\alpha}(x) = f_{\delta\alpha}(y)$ et $f'_{\delta\alpha}(x') = f'_{\delta\alpha}(y')$, ce qui achève la démonstration.

On dit que la bijection $g$ est *canonique*.

#### Corollaire {#ens-iii-s7-n7-cor-2 .statement tag=03RX}

Soient $(\mathbf{F}_\alpha, g_{\beta\alpha}), (\mathbf{F}'_\alpha, g'_{\beta\alpha})$ deux systèmes inductifs d’ensembles relatifs à $I$, et pour tout $\alpha \in I$, soient $u_\alpha : E_\alpha \to \mathbf{F}_\alpha$, $u'_\alpha : E'_\alpha \to \mathbf{F}'_\alpha$ des applications formant deux systèmes inductifs. Alors $(u_\alpha \times u'_\alpha)$ est un système inductif d’applications, et l’on a, à des bijections canoniques près

$$
\lim \left( u_\alpha \times u'_\alpha \right) = \left( \lim u_\alpha \right) \times \left( \lim u'_\alpha \right).
$$

La vérification est laissée au lecteur.

Exercises

## EXERCICES {#ens-iii-s7-exercises}

See the [exercises for § 7](exercises/s7/).
