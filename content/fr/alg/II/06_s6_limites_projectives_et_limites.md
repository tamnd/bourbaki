---
book: alg
book_title: Algebra
chapter: II
chapter_title: ALGÈBRE LINÉAIRE
section: 6
section_title: Limites projectives et limites inductives de modules
lang: fr
source: alg-i-iii-fr
book_pages: A II.88-A II.95
pdf_pages: 0265-0272, 0369-0369
extraction: ocr
subsections:
    - "no": 1
      title: Limites projectives de modules
      page: 88
      pdf_page: 265
    - "no": 2
      title: Limites inductives de modules
      page: 90
      pdf_page: 267
    - "no": 3
      title: Produit tensoriel de limites inductives
      page: 93
      pdf_page: 270
statements: 17
exercises: 4
content_sha256: e406895b1625ad7fa5ffe7186d3e518cff1a0f1317ac962efb162f7003c8aba6
---

## § 6. LIMITES PROJECTIVES ET LIMITES INDUCTIVES DE MODULES

Dans tout ce paragraphe, on désigne par $I$ un ensemble préordonné non vide, par $\alpha \leq \beta$ la relation de préordre dans $I$. Sauf mention expresse du contraire, les systèmes projectifs et inductifs considérés ont pour ensemble d’indices $I$.

### 1. Limites projectives de modules

Soient $(A_\alpha, \varphi_{\alpha\beta})$ un système projectif d’anneaux (I, p. 133), $(E_\alpha, f_{\alpha\beta})$ un système projectif de groupes commutatifs (notés additivement) (I, p. 113), et supposons chaque $E_\alpha$ muni d’une structure de $A_\alpha$-module à gauche; en outre supposons que pour $\alpha \leq \beta$, $(f_{\alpha \beta}, \varphi_{\alpha \beta})$ soit un dimorphisme de $E_\beta$ dans $E_\alpha$ (II, p. 32), autrement dit que l’on ait

(1)
$$
f_{\alpha \beta}(\lambda_\beta x_\beta) = \varphi_{\alpha \beta}(\lambda_\beta) f_{\alpha \beta}(x_\beta),
$$
pour $x_\beta \in E_\beta, \lambda_\beta \in A_\beta$; alors il résulte de I, p. 114 que $E = \lim_{\leftarrow} E_\alpha$ est muni d’une structure de module à gauche sur $A = \lim_{\leftarrow} A_\alpha$. Pour tout $\alpha \in I$, soient $f_\alpha : E \to E_\alpha$, $\varphi_\alpha : A \to A_\alpha$ les applications canoniques; alors $(f_\alpha, \varphi_\alpha)$ est un dimorphisme de $E$ dans $E_\alpha$. Nous dirons que $(E_\alpha, f_{\alpha \beta})$ est un système projectif de $A_\alpha$-modules à gauche, et que le $A$-module $E$ est sa limite projective.

Soit $(E'_\alpha, f'_{\alpha \beta})$ un second système projectif de $A_\alpha$-modules à gauche, et pour tout $\alpha$, soit $u_\alpha : E'_\alpha \to E_\alpha$ une application $A_\alpha$-linéaire, ces applications formant un système projectif; alors $u = \lim_{\leftarrow} u_\alpha$ est une application $A$-linéaire de $\lim_{\leftarrow} E'_\alpha$ dans $\lim_{\leftarrow} E_\alpha$.

En outre:

#### Proposition 1 {#alg-ii-s6-prop-1 .statement}

*Soient* $(E_\alpha, f_{\alpha \beta}), (E'_\alpha, f'_{\alpha \beta}), (E''_\alpha, f''_{\alpha \beta})$ *trois systèmes projectifs de* $A_\alpha$*-modules*, $(u_\alpha), (v_\alpha)$ *deux systèmes projectifs d’applications* $A_\alpha$*-linéaires tels que les suites*
$$
0 \longrightarrow E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha
$$
*soient exactes pour tout* $\alpha$. *Alors, si on pose* $u = \lim_{\leftarrow} u_\alpha, v = \lim_{\leftarrow} v_\alpha$, *la suite*
$$
0 \longrightarrow \lim_{\leftarrow} E'_\alpha \xrightarrow{u} \lim_{\leftarrow} E_\alpha \xrightarrow{v} \lim_{\leftarrow} E''_\alpha
$$
*est exacte*.

En effet, comme $\overline{u}_\alpha^1(0) = \{0\}$ pour tout $\alpha$, il résulte de E, III, p. 54, prop. 2 que $\overline{u}_\alpha^1(0) = \{0\}$, donc $u$ est injectif; en outre, les $u_\alpha(E'_\alpha)$ forment un système projectif de parties des $E_\alpha$ et l’on a $u(\lim_{\leftarrow} E'_\alpha) = \lim_{\leftarrow} u_\alpha(E'_\alpha)$. Comme $u_\alpha(E'_\alpha) = \overline{v}_\alpha^1(0)$ par hypothèse, on a $\overline{v}_\alpha^1(0) = \lim_{\leftarrow} u_\alpha(E'_\alpha) = u(\lim_{\leftarrow} E'_\alpha)$ (E, III, p. 54, prop. 2), ce qui achève la démonstration.

#### Remarque 1 {#alg-ii-s6-n1-rem-1 .statement}

La prop. 1 et sa démonstration sont valables pour des groupes quelconques, au changement de notation près.

#### Remarque 2 {#alg-ii-s6-n1-rem-2 .statement}

On notera que si l’on a des suites exactes
$$
0 \longrightarrow E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha \longrightarrow 0
$$
*il n’en résulte pas nécessairement* que la suite
$$
0 \longrightarrow \lim_{\leftarrow} E'_\alpha \xrightarrow{u} \lim_{\leftarrow} E_\alpha \xrightarrow{v} \lim_{\leftarrow} E''_\alpha \longrightarrow 0
$$
soit exacte; autrement dit, la limite projective d’un système projectif d’applications linéaires surjectives n’est pas nécessairement surjective (cf. II, p. 192, exerc. 1).

Supposons maintenant que tous les $A_\alpha$ soient égaux à un même anneau $A$ et les $\varphi_{\alpha \beta}$ à $1_A$; alors pour tout système projectif $(E_\alpha, f_{\alpha \beta})$ de $A$-modules, $E = \lim_{\leftarrow} E_\alpha$ est un $A$-module. Soit $F$ un $A$-module, et pour tout $\alpha$, soit $u_\alpha : F \to E_\alpha$ une applica-

tion A-linéaire telle que $(u_\alpha)$ soit un système projectif d’applications; alors $u = \lim_{\leftarrow} u_\alpha$ est une application A-linéaire de F dans $\lim_{\leftarrow} E_\alpha$. Inversement, pour toute application A-linéaire $v : F \to \lim_{\leftarrow} E_\alpha$, la famille des $v_\alpha = f_\alpha \circ v$ est un système projectif d’applications A-linéaires tel que $v = \lim_{\leftarrow} v_\alpha$. Notons d’autre part que pour $\alpha \leq \beta$, l’application
$$
\operatorname{Hom}(1_F, f_{\alpha \beta}) = \bar{f}_{\alpha \beta} : \operatorname{Hom}_A(F, E_\beta) \to \operatorname{Hom}_A(F, E_\alpha)
$$
est un homomorphisme de $\mathbf{Z}$-modules tel que $(\operatorname{Hom}_A(F, E_\alpha), \bar{f}_{\alpha \beta})$ soit un système projectif de $\mathbf{Z}$-modules; comme $\bar{f}_{\alpha \beta}(v_\beta) = f_{\alpha \beta} \circ v_\beta$, les remarques précédentes peuvent donc s’exprimer de la façon suivante:
**Proposition 2.** — *Pour tout système projectif* $(E_\alpha, f_{\alpha \beta})$ *de A-modules et tout A-module F, l’application canonique* $u \mapsto (f_\alpha \circ u)$ *est un isomorphisme de* $\mathbf{Z}$*-modules*
(2)
$$
l_F : \operatorname{Hom}_A(F, \lim_{\leftarrow} E_\alpha) \to \lim_{\leftarrow} \operatorname{Hom}_A(F, E_\alpha).
$$

#### Corollaire {#alg-ii-s6-n1-cor-1 .statement}

*Pour tout homomorphisme* $v : F \to F'$ *de A-modules, les* $\bar{v}_\alpha = \operatorname{Hom}(v, 1_{E_\alpha}) : \operatorname{Hom}(F', E_\alpha) \to \operatorname{Hom}(F, E_\alpha)$ *forment un système projectif d’applications* $\mathbf{Z}$*-linéaires, et le diagramme*
(3)
$$
\begin{array}{ccc}
\operatorname{Hom}(F', \lim_{\leftarrow} E_\alpha) & \xrightarrow{l_{F'}} & \lim_{\leftarrow} \operatorname{Hom}(F', E_\alpha) \\
\operatorname{Hom}(v, 1_E) \downarrow & & \downarrow \lim_{\leftarrow} \bar{v}_\alpha \\
\operatorname{Hom}(F, \lim_{\leftarrow} E_\alpha) & \xrightarrow{l_F} & \lim_{\leftarrow} \operatorname{Hom}(F, E_\alpha)
\end{array}
$$
*est commutatif*.
Pour tout $u \in \operatorname{Hom}(F', \lim_{\leftarrow} E_\alpha)$, on a en effet $l_F(u \circ v) = (f_\alpha \circ u \circ v)$ et la commutativité du diagramme (3) résulte alors aussitôt des définitions.

### 2. Limites inductives de modules

*On suppose désormais I filtrant à droite.*

Soient $(A_\alpha, \varphi_{\beta \alpha})$ un système inductif d’anneaux (I, p. 116), $(E_\alpha, f_{\beta \alpha})$ un système inductif de groupes commutatifs (notés additivement) (I, p. 116), et supposons chaque $E_\alpha$ muni d’une structure de $A_\alpha$-module *à gauche*; en outre, supposons que pour $\alpha \leq \beta$, $(f_{\beta \alpha}, \varphi_{\beta \alpha})$ soit un *dimorphisme* de $E_\alpha$ dans $E_\beta$ (II, p. 32), autrement dit que l’on ait
(4)
$$
f_{\beta \alpha}(\lambda_\alpha x_\alpha) = \varphi_{\beta \alpha}(\lambda_\alpha) f_{\beta \alpha}(x_\alpha)
$$
pour $x_\alpha \in E_\alpha, \lambda_\alpha \in A_\alpha$; alors $E = \lim_{\longrightarrow} E_\alpha$ est muni d’une structure de *module à gauche* sur $A = \lim_{\longrightarrow} A_\alpha$ (I, p. 117). Pour tout $\alpha \in I$, soient $f_\alpha : E_\alpha \to E, \varphi_\alpha : A_\alpha \to A$ les applications canoniques; alors $(f_\alpha, \varphi_\alpha)$ est un *dimorphisme* de $E_\alpha$ dans $E$. Nous dirons que $(E_\alpha, f_{\beta \alpha})$ est un *système inductif de* $A_\alpha$*-modules à gauche*, et que le A-module $E$ est sa *limite inductive*.
Soit $(E'_\alpha, f'_{\beta \alpha})$ un second système inductif de $A_\alpha$-modules à gauche, et pour tout $\alpha$, soit $u_\alpha : E'_\alpha \to E_\alpha$ une application $A_\alpha$-linéaire, ces applications formant un système inductif; alors $u = \lim u_\alpha$ est une application $A$-linéaire de $\lim E'_\alpha$ dans $\lim E_\alpha$. En outre:

#### Proposition 3 {#alg-ii-s6-prop-3 .statement}

*Soient* $(E_\alpha, f_{\beta \alpha}), (E'_\alpha, f'_{\beta \alpha}), (E''_\alpha, f''_{\beta \alpha})$ *trois systèmes inductifs de* $A_\alpha$*-modules*, $(u_\alpha), (v_\alpha)$ *deux systèmes inductifs d’applications* $A_\alpha$*-linéaires tels que les suites*

$$
E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha
$$

*soient exactes pour tout* $\alpha$. *Alors, si on pose* $u = \lim u_\alpha, v = \lim v_\alpha$, *la suite*

$$
\lim E'_\alpha \xrightarrow{u} \lim E_\alpha \xrightarrow{v} \lim E''_\alpha
$$

*est exacte*.

En effet, on a $u(\lim E'_\alpha) = \lim u_\alpha(E'_\alpha)$ et $\overline{v}^1(0) = \lim \overline{v}_\alpha^1(0)$ (E, III, p. 64, corollaire).

De façon imagée, on exprime encore la prop. 3 en disant que *le passage à la limite inductive préserve l’exactitude*.

#### Proposition 4 {#alg-ii-s6-prop-4 .statement}

*Soient* $(E_\alpha, f_{\beta \alpha})$ *un système inductif de* $A_\alpha$*-modules*, $E = \lim E_\alpha$ *sa limite inductive*, $\varphi_\alpha : A_\alpha \to A$ *et* $f_\alpha : E_\alpha \to E$ *les applications canoniques pour tout* $\alpha \in I$. *Si, pour tout* $\alpha \in I$, $S_\alpha$ *est un système générateur de* $E_\alpha$, *alors* $S = \bigcup_{\alpha \in I} f_\alpha(S_\alpha)$ *est un système générateur de* $E$.

En effet, tout $x \in E$ est de la forme $f_\alpha(x_\alpha)$ pour un $\alpha \in I$ et un $x_\alpha \in E_\alpha$, et par hypothèse $x_\alpha = \sum_i \lambda^{(i)}_\alpha y^{(i)}_\alpha$, où $\lambda^{(i)}_\alpha \in A_\alpha$ et $y^{(i)}_\alpha \in S_\alpha$; si on pose $\lambda^{(i)} = \varphi_\alpha(\lambda^{(i)}_\alpha)$, $y^{(i)} = f_\alpha(y^{(i)}_\alpha)$, on a $x = \sum_i \lambda^{(i)} y^{(i)}$.

#### Proposition 5 {#alg-ii-s6-prop-5 .statement}

*Les hypothèses et notations étant celles de la prop. 4, on suppose que pour tout* $\alpha \in I$, $E_\alpha$ *soit somme directe d’une famille* $(M^\lambda_\alpha)_{\lambda \in L}$ *de sous-modules* (l’ensemble d’indices $L$ *étant indépendant de* $\alpha$) *et que l’on ait* $f_{\beta \alpha}(M^\lambda_\alpha) \subset M^\lambda_\beta$ *pour* $\alpha \leq \beta$ *et pour tout* $\lambda \in L$. *Alors* $E$ *est somme directe de la famille des sous-modules* $M^\lambda = \lim M^\lambda_\alpha$ ($\lambda \in L$).

Il résulte de la prop. 4 que $E$ est somme des $M^\lambda$. Soit $(y^\lambda)_{\lambda \in L}$ une famille telle que $y^\lambda \in M^\lambda$ pour tout $\lambda \in L$, dont le support est fini, et supposons que $\sum_\lambda y^\lambda = 0$. En vertu de E, III, p. 62, lemme 1, il existe un $\alpha \in I$ et une famille $(x^\lambda_\alpha)_{\lambda \in L}$, de support fini, formée d’éléments de $E_\alpha$ tels que $x^\lambda_\alpha \in M^\lambda_\alpha$ et $y^\lambda = f_\alpha(x^\lambda_\alpha)$ pour tout $\lambda \in L$. La relation $f_\alpha \left( \sum_{\lambda \in L} x^\lambda_\alpha \right) = 0$ entraîne l’existence d’un $\beta \geq \alpha$ tel que $f_{\beta \alpha} \left( \sum_{\lambda \in L} x^\lambda_\alpha \right) = 0$ (E, III, p. 62, lemme 1) ce qui s’écrit $\sum_{\lambda \in L} x^\lambda_\beta = 0$, où $x^\lambda_\beta = f_{\beta \alpha}(x^\lambda_\alpha) \in M^\lambda_\beta$ par hypothèse; on a donc $x^\lambda_\beta = 0$ pour tout $\lambda \in L$, et par suite $y^\lambda = f_\beta(x^\lambda_\beta) = 0$ pour tout $\lambda \in L$, ce qui prouve que la somme des $M^\lambda$ est directe.

#### Corollaire {#alg-ii-s6-n2-cor-1 .statement}

Soit $(P_\alpha)$ un système inductif de parties des $E_\alpha$, et soit $P = \lim P_\alpha$. Si pour tout $\alpha \in I$, $P_\alpha$ est une partie libre (resp. une base) de $E_\alpha$, alors $P$ est une partie libre (resp. une base) de $E$.

La seconde assertion résulte aussitôt de la première et de la prop. 4. Il suffit donc de prouver que si les $P_\alpha$ sont libres, toute partie $\{y^{(i)}\}_{1 \leq i \leq n}$ formée d’éléments de $P$ deux à deux distincts, est libre. Il existe un $\alpha \in I$ et des éléments $x_\alpha^{(i)} \in P_\alpha$ tels que $y^{(i)} = f_\alpha(x_\alpha^{(i)})$ pour $1 \leq i \leq n$ (E, III, p. 62, lemme 1); si $\sum_i \lambda^{(i)} y^{(i)} = 0$, on peut supposer que $\lambda^{(i)} = \varphi_\alpha(\lambda_\alpha^{(i)})$ pour $1 \leq i \leq n$, donc on a $f_\alpha(\sum_i \lambda_\alpha^{(i)} x_\alpha^{(i)}) = 0$; cela entraîne $\sum_i \lambda_\beta^{(i)} x_\beta^{(i)} = 0$ pour un $\beta \geq \alpha$, avec $\lambda_\beta^{(i)} = \varphi_{\beta \alpha}(\lambda_\alpha^{(i)})$, $x_\beta^{(i)} = f_{\beta \alpha}(x_\alpha^{(i)})$, et les $x_\beta^{(i)}$ appartiennent à $P_\beta$ et sont deux à deux distincts, puisque $y^{(i)} = f_\beta(x_\beta^{(i)})$; on a donc $\lambda_\beta^{(i)} = 0$ pour $1 \leq i \leq n$, d’où $\lambda^{(i)} = \varphi_\beta(\lambda_\beta^{(i)}) = 0$ pour $1 \leq i \leq n$.

Supposons maintenant que tous les anneaux $A_\alpha$ soient égaux à un même anneau $A$ et les $\varphi_{\beta \alpha}$ à $1_A$; alors, pour tout système inductif $(E_\alpha, f_{\beta \alpha})$ de $A$-modules, $E = \lim E_\alpha$ est un $A$-module. Soit $F$ un $A$-module et pour tout $\alpha$, soit $u_\alpha : E_\alpha \to F$ une application $A$-linéaire telle que $(u_\alpha)$ soit un système inductif d’applications; alors $u = \lim u_\alpha$ est une application $A$-linéaire de $E$ dans $F$. Inversement, pour toute application $A$-linéaire $v : \lim E_\alpha \to F$, la famille des $v_\alpha = v \circ f_\alpha$ est un système inductif d’applications $A$-linéaires tel que $v = \lim v_\alpha$. Notons d’autre part que pour $\alpha \leq \beta$, l’application

$$
\operatorname{Hom}(f_{\beta \alpha}, 1_F) = \bar{f}_{\alpha \beta} : \operatorname{Hom}_A(E_\beta, F) \to \operatorname{Hom}_A(E_\alpha, F)
$$

est un homomorphisme de $\mathbf{Z}$-modules tel que $(\operatorname{Hom}_A(E_\alpha, F), \bar{f}_{\alpha \beta})$ soit un système projectif de $\mathbf{Z}$-modules; comme $\bar{f}_{\alpha \beta}(v_\beta) = v_\beta \circ f_{\beta \alpha}$, les remarques précédentes peuvent s’exprimer comme suit:

#### Proposition 6 {#alg-ii-s6-prop-6 .statement}

Pour tout système inductif $(E_\alpha, f_{\beta \alpha})$ de $A$-modules et tout $A$-module $F$, l’application canonique $u \mapsto (u \circ f_\alpha)$ est un isomorphisme de $\mathbf{Z}$-modules

$$(5)$$
$$
d_F : \operatorname{Hom}_A(\lim E_\alpha, F) \to \lim \operatorname{Hom}_A(E_\alpha, F).
$$

#### Corollaire 1 {#alg-ii-s6-prop-6-cor-1 .statement}

Pour tout homomorphisme $v : F \to F'$ de $A$-modules, les $\bar{v}_\alpha = \operatorname{Hom}(1_{E_\alpha}, v) : \operatorname{Hom}(E_\alpha, F) \to \operatorname{Hom}(E_\alpha, F')$ forment un système projectif d’applications $\mathbf{Z}$-linéaires, et le diagramme

$$(6)$$
$$
\begin{array}{ccc}
\operatorname{Hom}(\lim E_\alpha, F) & \xrightarrow{d_F} & \lim \operatorname{Hom}(E_\alpha, F) \\
\operatorname{Hom}(1_{E_\alpha}, v) \downarrow & & \downarrow \lim \bar{v}_\alpha \\
\operatorname{Hom}(\lim E_\alpha, F') & \xrightarrow{d_{F'}} & \lim \operatorname{Hom}(E_\alpha, F')
\end{array}
$$

est commutatif.

Pour tout $u \in \mathrm{Hom}(\lim_{\longrightarrow} E_\alpha, F)$, on a en effet $d_F(v \circ u) = (v \circ u \circ f_\alpha)$, et la commutativité du diagramme (6) résulte alors aussitôt des définitions.

#### Corollaire 2 {#alg-ii-s6-prop-6-cor-2 .statement}

Si $(E_\alpha, f_{\beta \alpha})$ est un système inductif de $A$-modules à gauche et $E = \lim_{\longrightarrow} E_\alpha$, $(E^*_\alpha, t f_{\beta \alpha})$ est un système projectif de $A$-modules à droite, et $\lim_{\longleftarrow} E^*_\alpha$ est canoniquement isomorphe à $E^*$.

#### Remarque {#alg-ii-s6-n2-rem-1 .statement}

Soient $E$ un $A$-module, $(M_\alpha)_{\alpha \in I}$ une famille croissante de sous-modules de $E$ telle que $E$ soit réunion des $M_\alpha$; si $j_{\beta \alpha} : M_\alpha \to M_\beta$ (pour $\alpha \leq \beta$) et $j_\alpha : M_\alpha \to E$ sont les injections canoniques, il est immédiat que $j = \lim_{\longrightarrow} j_\alpha$ est un isomorphisme de $\lim_{\longrightarrow} M_\alpha$ sur $E$ (E, III, p. 63, Remarque 1). En particulier, tout $A$-module est limite inductive de la famille filtrante croissante de ses sous-modules de type fini.

### 3. Produit tensoriel de limites inductives

Soient $(A_\alpha, \rho_{\beta \alpha})$ un système inductif d’anneaux, $(E_\alpha, f_{\beta \alpha})$ (resp. $(F_\alpha, g_{\beta \alpha})$) un système inductif de $A_\alpha$-modules à droite (resp. à gauche). Pour $\alpha \leq \beta$, on a un homomorphisme de $\mathbf{Z}$-modules

$$
f_{\beta \alpha} \otimes g_{\beta \alpha} : E_\alpha \otimes_{A_\alpha} F_\alpha \to (E_\beta)_{[A_\alpha]} \otimes_{A_\alpha} (F_\beta)_{[A_\alpha]}
$$

et d’autre part, on a un homomorphisme canonique de $\mathbf{Z}$-modules

$$
(E_\beta)_{[A_\alpha]} \otimes_{A_\alpha} (F_\beta)_{[A_\alpha]} \to E_\beta \otimes_{A_\beta} F_\beta
$$

correspondant à l’homomorphisme d’anneaux $\rho_{\beta \alpha}$ (II, p. 53, prop. 2); d’où, par composition, un homomorphisme de $\mathbf{Z}$-modules

$$
h_{\beta \alpha} : E_\alpha \otimes_{A_\alpha} F_\alpha \to E_\beta \otimes_{A_\beta} F_\beta
$$

qui, à tout produit tensoriel $x_\alpha \otimes y_\alpha$, fait correspondre $f_{\beta \alpha}(x_\alpha) \otimes g_{\beta \alpha}(y_\alpha)$. Il est clair que $(E_\alpha \otimes_{A_\alpha} F_\alpha, h_{\beta \alpha})$ est un système inductif de $\mathbf{Z}$-modules. Soient $A = \lim_{\longrightarrow} A_\alpha$, $E = \lim_{\longrightarrow} E_\alpha$, $F = \lim_{\longrightarrow} F_\alpha$, et soient $\rho_\alpha : A_\alpha \to A$, $f_\alpha : E_\alpha \to E$, $g_\alpha : F_\alpha \to F$ les applications canoniques. On définit comme ci-dessus une application $\mathbf{Z}$-linéaire $\pi_\alpha : E_\alpha \otimes_{A_\alpha} F_\alpha \to E \otimes_A F$ qui, à tout produit tensoriel $x_\alpha \otimes y_\alpha$, fait correspondre $f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)$, et il est immédiat que ces applications forment un système inductif. On en déduit une application $\mathbf{Z}$-linéaire

(7)
$$
\pi = \lim_{\longrightarrow} \pi_\alpha : \lim_{\longrightarrow} (E_\alpha \otimes_{A_\alpha} F_\alpha) \to E \otimes_A F.
$$

#### Proposition 7 {#alg-ii-s6-prop-7 .statement}

L’application $\mathbf{Z}$-linéaire (7) est bijective.

Posons $P = \lim_{\longrightarrow} (E_\alpha \otimes_{A_\alpha} F_\alpha)$ et, pour tout $\alpha \in I$, soit $h_\alpha : E_\alpha \otimes_{A_\alpha} F_\alpha \to P$ l’application canonique. Soit d’autre part, pour tout $\alpha \in I$,

$$
t_\alpha : E_\alpha \times F_\alpha \to E_\alpha \otimes_{A_\alpha} F_\alpha
$$

l’application $\mathbf{Z}$-bilinéaire canonique; pour $\alpha \leq \beta$, on a $t_\beta(f_{\beta \alpha}(x_\alpha), g_{\beta \alpha}(y_\alpha)) =$ f_{\beta \alpha}(x_\alpha) \otimes g_{\beta \alpha}(y_\alpha) = h_{\beta \alpha}(t_\alpha(x_\alpha, y_\alpha)), donc $(t_\alpha)$ est un système inductif d’applications. Identifiant canoniquement $\lim \rightarrow (E_\alpha \times F_\alpha)$ à $E \times F$ (E, III, p. 67, prop. 10), on en déduit une application $t = \lim \rightarrow t_\alpha : E \times F \to P$, telle que $t(f_\alpha(x_\alpha), g_\alpha(y_\alpha)) = h_\alpha(t_\alpha(x_\alpha, y_\alpha)) = h_\alpha(x_\alpha \otimes y_\alpha)$. Tenant compte du lemme 1 de E, III, p. 62, on voit aussitôt que $t$ est $\mathbf{Z}$-bilinéaire; en outre, pour $x \in E, y \in F, \lambda \in A$, il existe $\alpha \in I$ tel que $x = f_\alpha(x_\alpha), y = g_\alpha(y_\alpha), \lambda = \rho_\alpha(\lambda_\alpha)$ avec $\lambda_\alpha \in A_\alpha, x_\alpha \in E_\alpha, y_\alpha \in F_\alpha$ (E, III, p. 62, lemme 1); d’où $t(x\lambda, y) = h_\alpha((x_\alpha \lambda_\alpha) \otimes y_\alpha) = h_\alpha(x_\alpha \otimes (\lambda_\alpha y_\alpha)) = t(x, \lambda y)$. Il existe donc une application $\mathbf{Z}$-linéaire et une seule $\pi' : E \otimes_A F \to P$ telle que $\pi'(x \otimes y) = t(x, y)$ (II, p. 51, prop. 1). En outre, on a par définition

$$
\pi'(\pi(h_\alpha(x_\alpha \otimes y_\alpha))) = \pi'(f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)) = h_\alpha(x_\alpha \otimes y_\alpha)
$$
$$
\pi(\pi'(f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha))) = \pi(h_\alpha(x_\alpha \otimes y_\alpha)) = f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)
$$

et comme les éléments de la forme $f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)$ (resp. $h_\alpha(x_\alpha \otimes y_\alpha)$) engendrent le $\mathbf{Z}$-module $E \otimes_A F$ (resp. $P$), $\pi' \circ \pi$ et $\pi \circ \pi'$ sont les applications identiques.

C. Q. F. D.

De façon imagée, on exprime la prop. 7 en disant que le produit tensoriel commute avec les limites inductives, et l’on identifie d’ordinaire les deux membres de (7) au moyen de l’isomorphisme $\pi$.

#### Corollaire 1 {#alg-ii-s6-prop-7-cor-1 .statement}

Soit $(E'_\alpha, f'_{\beta \alpha})$ (resp. $(F'_\alpha, g'_{\beta \alpha})$) un second système inductif de $A_\alpha$-modules à droite (resp. à gauche); pour tout $\alpha \in I$, soit $u_\alpha : E_\alpha \to E'_\alpha$ (resp. $v_\alpha : F_\alpha \to F'_\alpha$) une application $A_\alpha$-linéaire, telle que $(u_\alpha)$ (resp. $(v_\alpha)$) soit un système inductif. Alors $(u_\alpha \otimes v_\alpha)$ est un système inductif d’applications $\mathbf{Z}$-linéaires, et le diagramme

$$
\begin{array}{ccc}
\lim \rightarrow (E_\alpha \otimes_{A_\alpha} F_\alpha) & \longrightarrow & (\lim \rightarrow E_\alpha) \otimes_A (\lim \rightarrow F_\alpha) \\
\downarrow & & \downarrow \\
\lim \rightarrow (E'_\alpha \otimes_{A_\alpha} F'_\alpha) & \longrightarrow & (\lim \rightarrow E'_\alpha) \otimes_A (\lim \rightarrow F'_\alpha)
\end{array}
$$

est commutatif.

La vérification est immédiate.

Soit $(A'_\alpha, \rho'_{\beta \alpha})$ un second système inductif d’anneaux, et supposons que chaque $E_\alpha$ soit un $(A'_\alpha, A_\alpha)$-bimodule, les $f_{\beta \alpha}$ étant $(A'_\alpha, A_\alpha)$-linéaires pour $\alpha \leq \beta$. Alors, si on pose $A' = \lim \rightarrow A'_\alpha$, l’isomorphisme (7) (II, p. 93) est linéaire pour les structures de $A'$-modules à gauche des deux membres en vertu du cor. 1. On généralise immédiatement à des multimodules quelconques.

En particulier, si les $A_\alpha$ sont commutatifs, $A = \lim \rightarrow A_\alpha$ est commutatif et l’isomorphisme (7) est un isomorphisme de $A$-modules.

#### Corollaire 2 {#alg-ii-s6-prop-7-cor-2 .statement}

Soit $(E_\alpha, f_{\beta \alpha})$ un système inductif de $A_\alpha$-modules à droite et soit $E'_\alpha = E_\alpha \otimes_{A_\alpha} A$ le $A$-module obtenu par extension à $A = \lim \rightarrow A_\alpha$ de l’anneau des scalaires au moyen de l’homomorphisme canonique $\rho_\alpha : A_\alpha \to A$. Alors $(E'_\alpha, f_{\beta\alpha} \otimes 1_A)$ est un système inductif de $A$-modules à droite, dont la limite inductive est canoniquement isomorphe à $\varprojlim E_\alpha$.

Il suffit d’appliquer la prop. 7 (II, p. 93) en prenant pour $F_\alpha$ l’anneau $A$ considéré comme $(A_\alpha, A)$-bimodule au moyen de $\rho_\alpha$.

#### Corollaire 3 {#alg-ii-s6-prop-7-cor-3 .statement}

*Soient $A$ un anneau, $(E_\alpha, f_{\beta\alpha})$ un système inductif de $A$-modules à droite, $F$ un $A$-module à gauche. Alors les $\mathbf{Z}$-modules $\varprojlim (E_\alpha \otimes_A F)$ et $(\varprojlim E_\alpha) \otimes_A F$ sont canoniquement isomorphes.*

Il suffit de faire $A_\alpha = A$ et $F_\alpha = F$ pour tout $\alpha \in I$ dans la prop. 7 (II, p. 93).

En particulier, si $\rho : A \to B$ est un homomorphisme d’anneaux, $\varprojlim \rho^*(E_\alpha)$ et $\rho^*(\varprojlim E_\alpha)$ sont canoniquement isomorphes.

#### Corollaire 4 {#alg-ii-s6-prop-7-cor-4 .statement}

*Soient $M$ un $A$-module à droite, $N$ un $A$ module à gauche, $(x_i)_{1 \leq i \leq n}$ une famille d’éléments de $M$, $(y_i)_{1 \leq i \leq n}$ une famille d’éléments de $N$, telles que $\sum_i (x_i \otimes y_i) = 0$ dans $M \otimes_A N$. Il existe alors un sous-module de type fini $M_1$ (resp. $N_1$) de $M$ (resp. $N$), contenant les $x_i$ (resp. les $y_i$), et tel que l’on ait $\sum_i (x_i \otimes y_i) = 0$ dans $M_1 \otimes_A N_1$.

En effet, $M$ (resp. $N$) s’identifie canoniquement à la limite inductive de la famille filtrante de ses sous-modules de type fini contenant les $x_i$ (resp. les $y_i$), et il suffit d’appliquer E, III, p. 62, lemme 1.

## EXERCICES {#alg-ii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
