---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VI
chapter_title: Systèmes de racines
section: 1
section_title: Systèmes de racines
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0141-0172, 0222-0225
extraction: ocr
subsections:
    - "no": 1
      title: Définition d’un système de racines
      page: 0
      pdf_page: 141
    - "no": 2
      title: Somme directe de systèmes de racines
      page: 0
      pdf_page: 145
    - "no": 3
      title: Relations entre deux racines
      page: 0
      pdf_page: 146
    - "no": 4
      title: Systèmes de racines réduits
      page: 0
      pdf_page: 150
    - "no": 5
      title: Chambres et bases d’un système de racines
      page: 0
      pdf_page: 152
    - "no": 6
      title: Racines positives
      page: 0
      pdf_page: 154
    - "no": 7
      title: Ensembles clos de racines
      page: 0
      pdf_page: 159
    - "no": 8
      title: Plus grande racine
      page: 0
      pdf_page: 164
    - "no": 9
      title: Poids, poids radiciels
      page: 0
      pdf_page: 165
    - "no": 10
      title: Poids fondamentaux, poids dominants
      page: 0
      pdf_page: 166
    - "no": 11
      title: Transformation de Coxeter
      page: 0
      pdf_page: 168
    - "no": 12
      title: Forme bilinéaire canonique
      page: 0
      pdf_page: 170
statements: 76
exercises: 24
content_sha256: f589f9c66d5dc049157fadfb4cab1add595be84cdcf4c16c98f7600c5f84106f
---

## § 1. Systèmes de racines

Dans ce paragraphe, $k$ désigne un corps de caractéristique zéro. À partir du n° 3, on suppose que $k = \mathbf{R}$.

### 1. Définition d’un système de racines

#### Lemme 1 {#lie-vi-s1-lem-1 .statement}

Soient $V$ un espace vectoriel sur $k$, $R$ une partie finie de $V$ engendrant $V$. Pour tout $\alpha \in \mathbf{R}$ tel que $\alpha \neq 0$, il existe au plus une réflexion $s$ de $V$ telle que $s(\alpha) = -\alpha$ et $s(R) = R$.

Soit $G$ le groupe des automorphismes de $V$ qui laissent $R$ stable. Comme $R$ engendre $V$, $G$ est isomorphe à un sous-groupe du groupe symétrique de $R$, donc est fini. Soient $s, s'$ deux réflexions de $V$ telles que $s(\alpha) = s'(\alpha) = -\alpha$, $s(R) = R$, $s'(R) = R$. Alors $t = ss'$ appartient à $G$, donc est d’ordre fini $m$. D’autre part, on a :

$$
t(\alpha) = \alpha \quad \text{et} \quad t(x) \equiv x \mod. k\alpha \quad \text{pour tout } x \in V.
$$

Il existe donc une forme linéaire $f$ sur $V$ telle que

$$
t(x) = x + f(x)\alpha \quad \text{pour tout } x \in V,
$$

et l’on a $f(\alpha) = 0$. Par récurrence sur $n$, on en déduit que

$$
t^n(x) = x + nf(x)\alpha \quad \text{pour tout } x \in V.
$$

En prenant $n$ égal à $m$, on voit que $mf(x) = 0$ pour tout $x \in V$, d’où $f = 0$, $t = 1$, et $s = s'$.

#### Définition 1 {#lie-vi-s1-def-1 .statement}

Soient $V$ un espace vectoriel sur $k$, et $R$ une partie de $V$. On dit que $R$ est un système de racines dans $V$ si les conditions suivantes sont vérifiées :
(SR_I) $R$ est fini, ne contient pas $0$, et engendre $V$.
(SR_{II}) Pour tout $\alpha \in R$, il existe un élément $\alpha^\vee$ du dual $V^*$ de $V$ tel que $\langle \alpha, \alpha^\vee \rangle = 2$ et que la réflexion $s_{\alpha, \alpha^\vee}$ (cf. chap. V, § 2) laisse stable $R$.
(SR_{III}) Pour tout $\alpha \in R$, on a $\alpha^\vee(R) \subset \mathbf{Z}$.

n° 1.1.

SYSTÈMES DE RACINES

D’après le lemme 1, la réflexion $s_{\alpha, \alpha^\vee}$ (donc aussi la forme linéaire $\alpha^\vee$) est déterminée de manière unique par $\alpha$, ce qui donne un sens à (SR_{III}). On posera $s_{\alpha, \alpha^\vee} = s_\alpha$. On a $s_\alpha(x) = x - \langle \alpha^\vee, x \rangle$ pour tout $x \in V$.

Les éléments de $\mathbf{R}$ sont appelés les racines (du système considéré). La dimension de $V$ s’appelle le rang du système.

Les automorphismes de $V$ qui laissent stable $R$ s’appellent les automorphismes de $R$. Ils forment un groupe fini noté $A(R)$. Le sous-groupe de $A(R)$ engendré par les $s_\alpha$ s’appelle le groupe de Weyl de $R$ et se note $W(R)$, ou simplement $W$.

Remarque 1). — Soit $k'$ une extension de $k$. Identifions canoniquement $V$ à un sous-ensemble de $V \otimes k'$ et $V^*$ à un sous-ensemble de $V^* \otimes k' = (V \otimes k')^*$. Alors, $R$ est un système de racines dans $V \otimes k'$, et les $\alpha^\vee$ sont les mêmes que précédemment.

#### Lemme 2 {#lie-vi-s1-lem-2 .statement}

Soit $R$ un système de racines dans $V$. Soit $(x|y)$ une forme bilinéaire symétrique sur $V$, non dégénérée, invariante par $W(R)$. Identifions $V$ à $V^*$ grâce à cette forme. Si $\alpha \in R$, $\alpha$ est non isotrope et

$$
\alpha^\vee = \frac{2\alpha}{(\alpha|\alpha)}.
$$

Cela résulte de la formule (4) du Chap. V, § 2, n° 3.

#### Proposition 1 {#lie-vi-s1-prop-1 .statement}

Soit $V_Q$ (resp. $V_Q^*$) le sous-$\mathbf{Q}$-espace vectoriel de $V$ (resp.$V^*$) engendré par les $\alpha$ (resp. les $\alpha^\vee$). Alors $V_Q$ (resp. $V_Q^*$) est une $\mathbf{Q}$-structure sur $V$ (resp. $V^*$) (Alg., chap. II, 3e éd., § 8, n° 1). La restriction à $V_Q \times V_Q^*$ de la forme bilinéaire canonique de $V \times V^*$ permet d’identifier chacun des espaces $V_Q, V_Q^*$ au dual de l’autre. L’ensemble $R$ est un système de racines dans $V_Q$.

Si $k = \mathbf{R}$, il existe un produit scalaire sur $V$ invariant par $W(R)$ (Intégr., chap. VII, § 3, n° 1, prop. 1); le lemme 2 prouve alors que les $\alpha^\vee$ engendrent $V^*$. D’après la Remarque 1, les $\alpha^\vee$ engendrent encore $V^*$ si $k = \mathbf{Q}$. Arrivons au cas général. Posons $E = V_Q$. D’après (SR_{III}), chaque $\alpha^\vee$ applique $E$ dans $\mathbf{Q}$, donc définit un élément $\tilde{\alpha}$ de $E^*$. Il est immédiat que $R$ est un système de racines dans $E$, et que l’élément correspondant à $\alpha$ dans $E^*$ est $\tilde{\alpha}$. D’après ce qui précède, les $\tilde{\alpha}$ engendrent l’espace vectoriel $E^*$. Considérons l’homomorphisme canonique $i : E \otimes_Q k \to V$, et son transposé $t_i : V^* \to E^* \otimes_Q k$. Puisque $R$ engendre $V$, $i$ est surjectif, donc $t_i$ est injectif; mais l’image de $t_i$ contient les $\tilde{\alpha}$, donc $t_i$ est surjectif. On en conclut finalement que $i$ et $t_i$ sont des isomorphismes. On peut identifier $V$ à $E \otimes k$, $V^*$ à $E^* \otimes k$, $\alpha^\vee$ à $\tilde{\alpha}$ et $V_Q^*$ à $E^*$. Ainsi $V_Q$ (resp. $V_Q^*$) est une $\mathbf{Q}$-structure sur $V$ (resp. $V^*$). La restriction à $V_Q \times V_Q^*$ de la forme bilinéaire canonique de $V \times V^*$ s’identifie à la forme bilinéaire canonique sur $E \times E^*$, d’où la proposition.

Remarques 2). — Grâce à la prop. 1, on peut ramener l’étude des systèmes de racines au cas où $k = \mathbf{Q}$. La Remarque 1 permet ensuite de se ramener à un système de racines de l’espace vectoriel réel $V_R = V_Q \otimes_Q \mathbf{R}$. Les groupes de Weyl associés à ces différents systèmes s’identifient canoniquement.

3) Puisque les $\alpha^\vee$ engendrent $V^*$, le groupe $W(R)$, considéré comme sous-groupe de $\mathbf{GL}(V_R)$, est essentiel (chap. V, § 3, n° 7). De plus, le cor. du th. 1 du chap. V, § 3, n° 2 montre que les seules réflexions appartenant à $W(R)$ sont les $s_\alpha$.

#### Proposition 2 {#lie-vi-s1-prop-2 .statement}

*Les $\alpha^\vee$ forment un système de racines dans $V^*$, et on a $\alpha^{\vee\vee} = \alpha$ pour tout $\alpha \in R$.*

Les $\alpha^\vee$ vérifient (SR_I) d’après la prop. 1. Puisque $s_{\alpha, \alpha^\vee}$ est un automorphisme de l’espace vectoriel $V$ muni du sous-ensemble $R$, $t(s_{\alpha, \alpha^\vee})^{-1}$ laisse stable l’ensemble $R^\vee$ des $\alpha^\vee$; or $t(s_{\alpha, \alpha^\vee})^{-1} = s_{\alpha^\vee, \alpha}$, ce qui prouve que $R^\vee$ vérifie (SR_{II}) et que $\alpha^{\vee\vee} = \alpha$. Enfin, on a $\langle \alpha^\vee, \beta \rangle \in \mathbf{Z}$ quels que soient $\alpha^\vee \in R$ et $\beta \in R$, donc $R^\vee$ vérifie (SR_{III}).

On dit que $R^\vee$ est le *système de racines inverse de* $R$. On voit que l’application $\alpha \mapsto \alpha^\vee$ est une bijection de $R$ sur $R^\vee$ appelée *bijection canonique de* $R$ *sur* $R^\vee$. On prendra garde que, si $\alpha, \beta$ sont des éléments de $R$ tels que $\alpha + \beta \in R$, alors $(\alpha + \beta)^\vee \neq \alpha^\vee + \beta^\vee$ en général.

Comme $s_\alpha(\alpha) = -\alpha$, l’axiome (SR_{II}) montre que $-R = R$. On a évidemment $(-\alpha)^\vee = -\alpha^\vee$ et $-1 \in A(R)$ (mais on n’a pas toujours $-1 \in W(R)$).

L’égalité $t(s_{\alpha, \alpha^\vee})^{-1} = s_{\alpha^\vee, \alpha}$ prouve que l’application $u \mapsto t_u^{-1}$ est un isomorphisme du groupe $W(R)$ sur le groupe $W(R^\vee)$. On identifie ces deux groupes par cet isomorphisme; autrement dit, on considère $W(R)$ comme opérant dans $V$ et dans $V^*$. De même pour $A(R)$.

#### Proposition 3 {#lie-vi-s1-prop-3 .statement}

*Pour $x, y \in V$, posons*
$$
(x|y) = \sum_{\alpha \in R} \langle \alpha^\vee, x \rangle \langle \alpha^\vee, y \rangle.
$$
*Alors* $(x|y)$ *est une forme bilinéaire symétrique non dégénérée sur* $V$, *invariante par* $A(R)$. *Pour* $x, y \in V_Q$, *on a* $(x|y) \in \mathbf{Q}$. *L’extension canonique de* $(x|y)$ *à*
$$
V_R = V_Q \otimes_Q \mathbf{R}
$$
*est positive non dégénérée*.

Il est clair que $(x|y)$ est une forme bilinéaire symétrique sur $V$. Si $g \in A(R)$, on a
$$
(g(x)|g(y)) = \sum_{\alpha \in R} \langle t_g(\alpha^\vee), x \rangle \langle t_g(\alpha^\vee), y \rangle = (x|y)
$$
puisque $(t_g)(R^\vee) = R^\vee$. Si $x, y \in V_Q$, on a $(x|y) \in \mathbf{Q}$ d’après (SR_{III}). Si $z \in V_R$, on a $(z|z) = \sum_{\alpha \in R} \langle \alpha^\vee, z \rangle^2 \geq 0$, et $(z|z) > 0$ si $z \neq 0$ d’après la prop. 1, donc l’extension canonique de $(x|y)$ à $V_R$ positive est non dégénérée. La restriction de $(x|y)$ à $V_Q$ est donc non dégénérée, et par suite la forme $(x|y)$ sur $V$ est non dégénérée.

n° 1.1.

#### Proposition 4 {#lie-vi-s1-prop-4 .statement}

(i) Soit $X$ une partie de $\mathbf{R}$, soit $V_X$ le sous-espace vectoriel de $V$ engendré par $X$, et soit $V'_X$ le sous-espace vectoriel de $V^*$ engendré par les $\alpha^\vee$, où $\alpha \in X$. Alors $V$ est somme directe de $V_X$ et du sous-espace orthogonal à $V'_X$, $V^*$ est somme directe de $V'_X$ et du sous-espace orthogonal à $V_X$, et $V'_X$ s’identifie au dual de $V_X$.

(ii) $R \cap V_X$ est un système de racines dans $V_X$, et la bijection canonique de $R \cap V_X$ sur le système inverse s’identifie à l’application $\alpha \mapsto \alpha^\vee$ restreinte à $R \cap V_X$.

Grâce à la remarque 2, on peut supposer que $k = \mathbf{R}$. Identifions $V$ à $V^*$ grâce à la forme bilinéaire symétrique de la prop. 3. On a $\alpha^\vee = \frac{2\alpha}{(\alpha|\alpha)}$ pour tout $\alpha \in \mathbf{R}$ (lemme 2). Tout sous-espace vectoriel de $V$ est non isotrope, et la proposition est alors évidente.

#### Corollaire {#lie-vi-s1-n1-cor-1 .statement}

Soit $V_1$ un sous-espace vectoriel de $V$, et soit $V_2$ le sous-espace vectoriel engendré par $R \cap V_1$. Alors $R \cap V_1$ est un système de racines dans $V_2$.

Cela résulte de (ii), appliqué à $X = R \cap V_1$.

Pour $\alpha \in \mathbf{R}$ et $\beta \in \mathbf{R}$, on pose :

(1) $$ \langle \alpha, \beta^\vee \rangle = n(\alpha, \beta). $$

On a donc :

(2) $$ n(\alpha, \alpha) = 2 $$
(3) $$ n(-\alpha, \beta) = n(\alpha, -\beta) = -n(\alpha, \beta). $$

D’après (SR_{III}),

(4) $$ n(\alpha, \beta) \in \mathbf{Z}. $$

Par définition même de $n(\alpha, \beta)$,

(5) $$ s_\beta(\alpha) = \alpha - n(\alpha, \beta)\beta. $$

La formule (1) et la prop. 2 entraînent

(6) $$ n(\alpha, \beta) = n(\beta^\vee, \alpha^\vee). $$

Soit $(x|y)$ une forme bilinéaire symétrique sur $V$, non dégénérée et invariante par $W(\mathbf{R})$ (prop. 3). On a, d’après le lemme 2,

(7) $$ n(\alpha, \beta) = \frac{2(\alpha|\beta)}{(\beta|\beta)}. $$

On en déduit que

(8) $$ n(\alpha, \beta) = 0 \iff n(\beta, \alpha) = 0 \iff (\alpha|\beta) = 0 $$
$$ \iff s_\alpha \text{ et } s_\beta \text{ sont permutables.} $$

(9) Si $(\alpha|\beta) \neq 0$, on a $$ \frac{n(\beta, \alpha)}{n(\alpha, \beta)} = \frac{(\beta|\beta)}{(\alpha|\alpha)}. $$

### 2. Somme directe de systèmes de racines

Soit V un espace vectoriel sur k, somme directe d’une famille $(V_i)_{1 \leq i \leq r}$ de sous-espaces vectoriels. Identifions $V^*$ à la somme directe des $V_i^*$. Pour tout $i$, soit $R_i$ un système de racines dans $V_i$. Alors $R = \bigcup_i R_i$ est un système de racines dans V dont le système inverse est $R^\vee = \bigcup_i R_i^\vee$; la bijection canonique de R sur $R^\vee$ prolonge, pour tout $i$, la bijection canonique de $R_i$ sur $R_i^\vee$. On dit que R est le *système de racines somme directe des* $R_i$. Soit $\alpha \in R_i$. Si $j \neq i$, le noyau de $\alpha^\vee$ contient $V_j$, donc $s_\alpha$ induit l’identité dans $V_j$; d’autre part, $k\alpha \subset V_i$, donc $s_\alpha$ laisse stable $V_i$. Ces remarques prouvent que $W(R)$ s’identifie à $\prod_{i=1}^r W(R_i)$.

On dit qu’un système de racines R est *irréductible* si $R \neq \emptyset$ et si R n’est pas somme directe de deux systèmes de racines non vides.

#### Proposition 5 {#lie-vi-s1-prop-5 .statement}

*Soit V un espace vectoriel sur k, somme directe de sous-espaces vectoriels $V_1, \ldots, V_r$. Soit R un système de racines dans V. Posons $R_i = R \cap V_i$. Les trois conditions suivantes sont équivalentes*:
(i) les $V_i$ sont stables par $W(R)$;
(ii) $R \subset V_1 \cup V_2 \cup \cdots \cup V_r$;
(iii) *pour tout i, $R_i$ est un système de racines dans $V_i$, et R est somme directe des* $R_i$.

(iii) $\Longrightarrow$ (i): ceci résulte de ce qu’on a dit au début de ce numéro.
(i) $\Longrightarrow$ (ii): supposons les $V_i$ stables par $W(R)$. Soit $\alpha \in R$, et soit H le noyau de $\alpha^\vee$. D’après la prop. 3 du chap. V, § 2, no 2, chaque $V_i$ est somme d’un sous-espace de H et d’un sous-espace de $k\alpha$. Donc l’un des $V_i$ contient $k\alpha$, d’où $\alpha \in V_1 \cup V_2 \cup \cdots \cup V_r$.
(ii) $\Longrightarrow$ (iii): si la condition (ii) est remplie, $R_i$ engendre $V_i$ pour tout $i$, donc $R_i$ est un système de racines dans $V_i$ (prop. 4). Il est clair que R est la somme directe des $R_i$.

#### Corollaire {#lie-vi-s1-n2-cor-1 .statement}

*Soit R un système de racines dans V. Les conditions suivantes sont équivalentes*:
(i) R est irréductible;
(ii) le $W(R)$-module V est simple;
(iii) le $W(R)$-module V est absolument simple.
(ii) $\Longleftrightarrow$ (i): cela résulte de la prop. 5 et du th. de Maschke (chap. V, Annexe, prop. 2).
(iii) $\Longleftrightarrow$ (ii): cela résulte de la prop. 1 du chap. V, § 2, no 1.

#### Proposition 6 {#lie-vi-s1-prop-6 .statement}

*Tout système de racines R dans V est somme directe d’une famille $(R_i)_{i \in I}$ de systèmes de racines irréductibles, qui est bien déterminée à une bijection près sur l’ensemble d’indices.*

L’existence des $R_i$ se démontre par récurrence sur Card $R$: si $R$ est non vide et non irréductible, $R$ est somme directe de deux systèmes de racines $R'$, $R''$ tels que Card $R' <$ Card $R$, Card $R'' <$ Card $R$, et l’on applique l’hypothèse de récurrence à $R'$ et $R''$. Pour prouver l’unicité, il suffit de prouver que, si $R$ est somme directe de $R'$ et $R''$, tout $R_i$ est nécessairement contenu dans $R'$ ou dans $R''$. Soient $V', V'', V'_i, V''_i$ les sous-espaces vectoriels de $V$ engendrés par $R', R'', R' \cap R_i, R'' \cap R_i$. Puisque la somme $V' + V''$ est directe, la somme $V'_i + V''_i$ est directe. On a $R_i \subset R' \cup R''$, donc $R_i$ est somme directe des systèmes de racines $R' \cap R_i$ et $R'' \cap R_i$; d’où $R' \cap R_i = \emptyset$ ou $R'' \cap R_i = \emptyset$, ce qui établit notre assertion.

On dit que les $R_i$ sont les composants irréductibles de $R$. Quels que soient les scalaires $\lambda_i$ non nuls, la réunion des $\lambda_i R_i$ est un système de racines dans $V$, dont le système inverse est la réunion des $\lambda_i^{-1} R_i$, et dont le groupe de Weyl est $W(R)$.

#### Proposition 7 {#lie-vi-s1-prop-7 .statement}

*Soient $R$ un système de racines dans $V$, $(R_i)$ la famille de ses composants irréductibles, $V_i$ le sous-espace vectoriel de $V$ engendré par $R_i$, B la forme bilinéaire symétrique définie dans la prop. 3, $B'$ une forme bilinéaire symétrique sur $V$ invariante par $W(R)$. Alors les $V_i$ sont deux à deux orthogonaux pour $B'$, et, pour tout $i$, les restrictions de $B$ et $B'$ à $V_i$ sont proportionnelles.*

Si $v_i \in V_i, v_j \in V_j, i \neq j$, et si $w \in W(R_j)$, on a
$$
B'(v_i, w(v_j)) = B'(v_i, v_j),
$$
ce qui montre que $w(v_j) - v_j$ est orthogonal à $v_i$ pour $B'$. Comme $V_j$ est irréductible pour $W(R_j)$, il est engendré par les $w(v_j) - v_j$, et il est donc orthogonal à $V_i$.

Le fait que les restrictions de $B$ et $B'$ à chacun des $V_i$ soient proportionnelles résulte de la prop. 1 du chap. V, § 2, no 1.

#### Remarque {#lie-vi-s1-n2-rem-1 .statement}

Choisissons un produit scalaire sur $V_R$ invariant par $W(R)$. Cela permet de parler de la *longueur* d’une racine et de l’*angle* de deux racines. La prop. 7 montre que cet angle est indépendant du choix du produit scalaire, et qu’il en est de même du rapport des longueurs de deux racines, pourvu que celles-ci appartiennent à la *même* composante irréductible de $R$.

### 3. Relations entre deux racines

Rappelons que *l’on suppose désormais $k = \mathbf{R}$*. (Nous laissons au lecteur le soin d’étendre définitions et résultats au cas général, par la méthode indiquée dans la *Remarque 2* du no 1.)

Dans tout ce qui suit, $R$ désigne un système de racines dans un espace vectoriel $V$; on munit $V$ d’un produit scalaire $(x, y) \mapsto (x|y)$ invariant par $W(R)$, cf. prop. 3.

Soient $\alpha, \beta \in \mathbf{R}$. D’après la formule (7) du n° 1, on a

$$
n(\alpha, \beta)n(\beta, \alpha) = 4 \cos^2 (\widehat{\alpha, \beta}) \leq 4.
$$

L’entier $n(\alpha, \beta)n(\beta, \alpha)$ ne peut donc prendre que les valeurs 0, 1, 2, 3, 4. Compte tenu du chap. V, § 2, n° 5, cor. de la prop. 6, et de la note de bas de page du chap. V, § 4, n° 8, on voit que les seules possibilités sont les suivantes, à l’échange près de $\alpha$ et $\beta$:

1) $n(\alpha, \beta) = n(\beta, \alpha) = 0; \quad \widehat{(\alpha, \beta)} = \frac{\pi}{2}; \quad s_{\alpha}s_{\beta}$ d’ordre 2;

2) $n(\alpha, \beta) = n(\beta, \alpha) = 1; \quad \widehat{(\alpha, \beta)} = \frac{\pi}{3}; ||\alpha|| = ||\beta||; \quad s_{\alpha}s_{\beta}$ d’ordre 3;

3) $n(\alpha, \beta) = n(\beta, \alpha) = -1; \quad \widehat{(\alpha, \beta)} = \frac{2\pi}{3}; ||\alpha|| = ||\beta||; \quad s_{\alpha}s_{\beta}$ d’ordre 3;

4) $n(\alpha, \beta) = 1, \quad n(\beta, \alpha) = 2; \quad \widehat{(\alpha, \beta)} = \frac{\pi}{4}; ||\beta|| = \sqrt{2}||\alpha||; s_{\alpha}s_{\beta}$ d’ordre 4;

5) $n(\alpha, \beta) = -1, n(\beta, \alpha) = -2; \widehat{(\alpha, \beta)} = \frac{3\pi}{4}; ||\beta|| = \sqrt{2}||\alpha||; s_{\alpha}s_{\beta}$ d’ordre 4;

6) $n(\alpha, \beta) = 1, \quad n(\beta, \alpha) = 3; \quad \widehat{(\alpha, \beta)} = \frac{\pi}{6}; ||\beta|| = \sqrt{3}||\alpha||; s_{\alpha}s_{\beta}$ d’ordre 6;

7) $n(\alpha, \beta) = -1, n(\beta, \alpha) = -3; \widehat{(\alpha, \beta)} = \frac{5\pi}{6}; ||\beta|| = \sqrt{3}||\alpha||; s_{\alpha}s_{\beta}$ d’ordre 6;

8) $n(\alpha, \beta) = n(\beta, \alpha) = 2; \quad \alpha = \beta;$

9) $n(\alpha, \beta) = n(\beta, \alpha) = -2; \quad \alpha = -\beta;$

10) $n(\alpha, \beta) = 1, \quad n(\beta, \alpha) = 4; \quad \beta = 2\alpha;$

11) $n(\alpha, \beta) = -1, n(\beta, \alpha) = -4; \quad \beta = -2\alpha.$

En particulier :

#### Proposition 8 {#lie-vi-s1-prop-8 .statement}

(i) *Si deux racines sont proportionnelles, le facteur de proportionalité ne peut être que $\pm 1, \pm \frac{1}{2}, \pm 2$.*

(ii) *Si $\alpha, \beta$ sont deux racines non proportionnelles, et si $||\alpha|| \leq ||\beta||$, alors $n(\alpha, \beta)$ prend l’une des valeurs 0, 1, —1.

Si une racine $\alpha \in \mathbf{R}$ est telle que $\frac{1}{2}\alpha \in \mathbf{R}$, on dit que $\alpha$ est une racine *indivisible*.

#### Théorème 1 {#lie-vi-s1-thm-1 .statement}

*Soient $\alpha, \beta$ deux racines.*
(i) *Si $n(\alpha, \beta) > 0$, $\alpha - \beta$ est une racine sauf si $\alpha = \beta$.*
(ii) *Si $n(\alpha, \beta) < 0$, $\alpha + \beta$ est une racine sauf si $\alpha = -\beta$.*
Si $n(\alpha, \beta) > 0$, les possibilités, d’après la liste ci-dessus, sont les suivantes :
1) $n(\alpha, \beta) = 1$; alors $\alpha - \beta = s_{\beta}(\alpha) \in \mathbf{R}$;
2) $n(\beta, \alpha) = 1$; alors $\beta - \alpha = s_{\alpha}(\beta) \in \mathbf{R}$, donc $\alpha - \beta \in \mathbf{R}$;
3) $\beta = \alpha$.

Ceci prouve (i), et (ii) s’en déduit en changeant $\beta$ en $-\beta$.

n° 1.3.

#### Corollaire {#lie-vi-s1-n3-cor-1 .statement}

Soient $\alpha$ et $\beta$ deux racines.
    (i) Si $(\alpha|\beta) > 0$, $\alpha - \beta$ est une racine sauf si $\alpha = \beta$.
    (ii) Si $(\alpha|\beta) < 0$, $\alpha + \beta$ est une racine sauf si $\alpha = -\beta$.
    (iii) Si $\alpha - \beta \in \mathbf{R} \cup \{0\}$ et $\alpha + \beta \in \mathbf{R} \cup \{0\}$, on a $(\alpha|\beta) = 0$.

Les assertions (i) et (ii) résultent du th. 1 et de la formule (7) du n° 1. L’assertion (iii) résulte de (i) et (ii).

Il peut se faire que $\alpha + \beta \in \mathbf{R}$, $(\alpha|\beta) = 0$ (cf. planche X, système $B_2$). Lorsque $\alpha - \beta \in \mathbf{R} \cup \{0\}$ et $\alpha + \beta \in \mathbf{R} \cup \{0\}$, on dit que les racines $\alpha$ et $\beta$ sont fortement orthogonales.

#### Proposition 9 {#lie-vi-s1-prop-9 .statement}

Soient $\alpha$ et $\beta$ deux racines non proportionnelles.
    (i) L’ensemble $I$ des entiers rationnels $j$ tels que $\beta + j\alpha$ soit une racine est un intervalle $(-q, p)$ de $\mathbf{Z}$ contenant 0.
    (ii) Soit $S$ l’ensemble des $\beta + j\alpha$ pour $j \in I$. Alors
        $$
        s_\alpha(S) = S \quad \text{et} \quad s_\alpha(\beta + p\alpha) = \beta - q\alpha.
        $$
    (iii) On a $p - q = -n(\beta, \alpha)$.

Il est clair que $0 \in I$. Soit $p$ (resp. $-q$) le plus grand (resp. le plus petit) élément de $I$. Si tous les entiers de $(-q, p)$ n’appartiennent pas à $I$, il existe deux entiers $r, s$ dans $(-q, p)$ possédant les propriétés suivantes : $s > r + 1$, $s \in I$, $r \in I$, $r + k \in I$ pour $1 \leq k \leq s - r - 1$. Avec les notations du cor. du th. 1, on a $(\alpha|\beta + s\alpha) \leq 0$, $(\alpha|\beta + r\alpha) \geq 0$, ce qui est absurde car
$$
(\alpha|\beta + s\alpha) > (\alpha|\beta + r\alpha).
$$
Ceci prouve (i).

On a $s_\alpha(\beta + j\alpha) = \beta - n(\beta, \alpha)\alpha - j\alpha = \beta + j'\alpha$ avec $j' = -j - n(\beta, \alpha)$. Donc $s_\alpha(S) \subset S$ et par suite $s_\alpha(S) = S$. En outre on voit que l’application $j \mapsto -j - n(\beta, \alpha)$ est une bijection décroissante de $I$ sur $I$. On en déduit que, pour $j = p$, on a $j' = -q$, de sorte que $-q = -p - n(\beta, \alpha)$. Ceci prouve (ii) et (iii).

On dit que $S$ est la $\alpha$-chaîne de racines définie par $\beta$, que $\beta - q\alpha$ est l’origine de la chaîne et $\beta + p\alpha$ son extrémité, et que $p + q$ est sa longueur.

#### Corollaire {#lie-vi-s1-n3-cor-2 .statement}

Soient $S$ une $\alpha$-chaîne de racines, $\gamma$ l’origine de $S$. La longueur de $S$ est $-n(\gamma, \alpha)$; elle est égale à 0, 1, 2 ou 3.

La première assertion résulte de la prop. 9, (iii), appliquée à $\beta = \gamma$, compte tenu de ce que $p = 0$.

D’autre part, comme $\gamma$ n’est pas proportionnelle à $\alpha$, la liste donnée au début de ce n° montre que $|n(\gamma, \alpha)| \leq 3$, d’où le corollaire.

#### Remarque {#lie-vi-s1-n3-rem-1 .statement}

Gardons les notations du corollaire ci-dessus. Alors :
    1) Si la longueur de $S$ est 0, on a $(\alpha|\gamma) = 0$.

2) Si la longueur de S est 1, on a $n(\gamma, \alpha) = -1$, d’où trois cas :

$$
n(\alpha, \gamma) = -1, \quad (\alpha|\alpha) = (\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{1}{2} (\alpha|\alpha), \quad (\widehat{\alpha, \gamma}) = \frac{2\pi}{3}
$$
$$
n(\alpha, \gamma) = -2, \quad (\alpha|\alpha) = 2(\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{1}{2} (\alpha|\alpha), \quad (\widehat{\alpha, \gamma}) = \frac{3\pi}{4}
$$
$$
n(\alpha, \gamma) = -3, \quad (\alpha|\alpha) = 3(\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{1}{2} (\alpha|\alpha), \quad (\widehat{\alpha, \gamma}) = \frac{5\pi}{6}
$$

![Diagram showing branching with angles π/3, π/4, 2π/3, and π/6](../images/chapter_6/systemes_racines_1.png)

3) Si la longueur de S est 2, on a $n(\gamma, \alpha) = -2$, d’où
$$
n(\alpha, \gamma) = -1, \quad (\alpha|\alpha) = \frac{1}{2} (\gamma|\gamma), \quad (\alpha|\gamma) = -(\alpha|\alpha), \quad (\widehat{\alpha, \gamma}) = \frac{3\pi}{4}.
$$

![Diagram showing branching with angles π/4, π/4, and π/4](../images/chapter_6/systemes_racines_2.png)

4) Si la longueur de S est 3, on a $n(\gamma, \alpha) = -3$, d’où
$$
n(\alpha, \gamma) = -1, \quad (\alpha|\alpha) = \frac{1}{3} (\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{3}{2} (\alpha|\alpha), \quad (\widehat{\alpha, \gamma}) = \frac{5\pi}{6}.
$$

![Diagram showing branching with angles π/6, π/3, π/6, and π/6](../images/chapter_6/systemes_racines_3.png)

Nous verrons (plancher X, systèmes A_2, B_2, G_2) que tous ces cas peuvent effectivement se présenter.

#### Proposition 10 {#lie-vi-s1-prop-10 .statement}

Soient $\alpha, \beta$ deux racines non proportionnelles telles que $\beta + \alpha$ soit une racine. Soient $p, q$ les entiers de la prop. 9. On a
$$
\frac{(\beta + \alpha|\beta + \alpha)}{(\beta|\beta)} = \frac{q + 1}{p}.
$$

Soient S la $\alpha$-chaîne définie par $\beta$, $\gamma$ son origine; sa longueur $l$ est $\geqslant 1$ puisque $\beta + \alpha$ est une racine. On peut avoir les cas suivants :

1) $l = 1$; alors $\beta = \gamma$, $q = 0$, $p = 1$, $(\beta + \alpha|\beta + \alpha) = (\beta|\beta)$.
2) $l = 2$, $\beta = \gamma$; alors $q = 0$, $p = 2$, $(\beta + \alpha|\beta + \alpha) = \frac{1}{2} (\beta|\beta)$.
3) $l = 2$, $\beta = \gamma + \alpha$; alors $q = 1$, $p = 1$, $(\beta + \alpha|\beta + \alpha) = 2(\beta|\beta)$.
4) $l = 3$, $\beta = \gamma$; alors $q = 0$, $p = 3$, $(\beta + \alpha|\beta + \alpha) = \frac{1}{3} (\beta|\beta)$.

n° 1.4.

5) $l = 3,\ \beta = \gamma + \alpha;$ alors $q = 1,\ p = 2,\ (\beta + \alpha|\beta + \alpha) = (\beta|\beta).$

6) $l = 3,\ \beta = \gamma + 2\alpha;$ alors $q = 2,\ p = 1,\ (\beta + \alpha|\beta + \alpha) = 3(\beta|\beta).$

Dans tous les cas, la formule à établir est vérifiée.

#### Proposition 11 {#lie-vi-s1-prop-11 .statement}

Supposons R irréductible. Soient $\alpha$ et $\beta$ deux racines telles que $||\alpha|| = ||\beta||$. Il existe $g \in W(R)$ tel que $g(\alpha) = \beta$.

Les transformés de $\alpha$ par $W(R)$ engendrent V (n° 2, cor. de la prop. 5). Il existe donc $g \in W(R)$ tel que $(g(\alpha)|\beta) \neq 0$. On peut ainsi supposer désormais que $(\alpha|\beta) \neq 0$. D’après la formule (9) du n° 1, $n(\alpha, \beta) = n(\beta, \alpha)$. Remplaçant éventuellement $\beta$ par $s_\beta(\beta) = -\beta$, on peut supposer $n(\alpha, \beta) > 0$. Alors, d’après la liste du début du n° 3, ou bien $\alpha = \beta$ (auquel cas la proposition est évidente), ou bien $n(\alpha, \beta) = n(\beta, \alpha) = 1$; dans ce cas

$$
(s_\alpha s_\beta s_\alpha)(\beta) = s_\alpha s_\beta(\beta - \alpha) = s_\alpha(-\beta - \alpha + \beta) = \alpha.
$$

### 4. Systèmes de racines réduits

On dit qu’un système de racines est réduit si toute racine du système est indivisible (n° 3).

#### Proposition 12 {#lie-vi-s1-prop-12 .statement}

Supposons R irréductible et réduit.

(i) Le rapport $\frac{(\beta|\beta)}{(\alpha|\alpha)}$ pour $\alpha \in R,\ \beta \in R$ ne peut prendre que les valeurs 1, 2, $\frac{1}{2}$, 3, $\frac{1}{3}$.

(ii) L’ensemble des $(\alpha|\alpha)$ pour $\alpha \in R$ a au plus deux éléments.

Comme R est irréductible, les transformés d’une racine par $W(R)$ engendrent V (n° 2, cor. de la prop. 5). Quelles que soient les racines $\alpha, \beta$, il existe donc une racine $\beta'$ telle que $(\alpha|\beta') \neq 0$ et $(\beta'| \beta') = (\beta|\beta)$. D’après la formule (9) du n° 1 et la liste du n° 3, $\frac{(\beta'| \beta')}{(\alpha|\alpha)}$ prend l’une des valeurs 1, 2, $\frac{1}{2}$, 3, $\frac{1}{3}$ (rappelons que le système est supposé réduit). En multipliant $(x|y)$ par un scalaire convenable, on peut supposer que $(\alpha|\alpha) = 1$ pour certaines racines et que les autres valeurs possibles de $(\beta|\beta)$ pour $\beta \in R$ sont 2 et 3. Les valeurs 2 et 3 ne peuvent être atteintes toutes les deux, car il existerait $\beta \in R,\ \gamma \in R$ tels que $\frac{(\gamma|\gamma)}{(\beta|\beta)} = \frac{3}{2}$, contrairement à ce qu’on a vu plus haut.

#### Proposition 13 {#lie-vi-s1-prop-13 .statement}

Supposons R irréductible, non réduit et de rang $\geq 2$.

(i) L’ensemble $R_0$ des racines indivisibles est un système de racines dans V ; ce système est irréductible et réduit ; on a $W(R_0) = W(R)$.

(ii) Soit A l’ensemble des racines $\alpha$ pour lesquelles $(\alpha|\alpha)$ prend la plus petite valeur $\lambda$. Alors deux éléments non proportionnels de A sont orthogonaux.

(iii) Soit B l’ensemble des $\beta \in \mathbf{R}$ tels que $(\beta|\beta) = 2\lambda$. On a $B \neq \varnothing$, $R_0 = A \cup B$, $R = A \cup B \cup 2A$.

Si $\alpha \in \mathbf{R} - R_0$, on a $\frac{1}{2} \alpha \in \mathbf{R}$, mais $\frac{1}{2} (\frac{1}{2} \alpha) \in \mathbf{R}$ (prop. 8), donc $\frac{1}{2} \alpha \in R_0$.

Ceci prouve que $R_0$ vérifie (SR_I). Il est clair que, pour tout $\alpha \in \mathbf{R}$, on a $s_{\alpha, \alpha^\vee}(R_0) = R_0$, donc $R_0$ vérifie (SR_{II}) et (SR_{III}). Comme $\alpha \in \mathbf{R} - R_0$ implique $\frac{1}{2} \alpha \in R_0$ et que $s_\alpha = s_{\alpha/2}$, on a $W(R) = W(R_0)$. Donc $R_0$ est irréductible (cor. de la prop. 5), et est évidemment réduit.

Comme $R$ est non réduit, il existe $\alpha \in R_0$ tel que $2\alpha \in \mathbf{R}$. Comme $R_0$ est irréductible et que dim $V \geq 2$, il n’est pas possible que $\alpha$ soit proportionnel ou orthogonal à toute racine. Soit $\beta \in R_0$ tel que $n(\beta, \alpha) \neq 0$ et que $\beta$ soit non proportionnel à $\alpha$. En changeant $\beta$ en $-\beta$, on peut supposer $n(\beta, \alpha) > 0$.

On a $\frac{1}{2} n(\beta, \alpha) = n(\beta, 2\alpha) \in \mathbf{Z}$, donc $n(\beta, \alpha) \in 2\mathbf{Z}$. D’après la liste du no 3, on a $n(\beta, \alpha) = 2$, $(\beta|\beta) = 2(\alpha|\alpha)$. Comme $R_0$ est réduit, la prop. 12 montre que, pour tout $\gamma \in R_0$, on a $(\gamma|\gamma) = (\alpha|\alpha)$ ou $(\gamma|\gamma) = 2(\alpha|\alpha)$. Et ce qui précède montre que, pour tout $\gamma \in \mathbf{R} - R_0$, le vecteur $\frac{1}{2} \gamma$ est un élément de $R_0$ tel que $(\frac{1}{2} \gamma | \frac{1}{2} \gamma) = (\alpha|\alpha)$. Ainsi, $\lambda = (\alpha|\alpha)$, $B \neq \varnothing$, $R_0 = A \cup B$, et $R \subset A \cup B \cup 2A$; d’autre part, si $\gamma \in A$, il existe $g \in W(R)$ tel que $\gamma = g(\alpha)$ (prop. 11), d’où $2\gamma = g(2\alpha) \in \mathbf{R}$; donc $2A \subset R$ et $R = A \cup B \cup 2A$. Enfin, soient $\gamma, \gamma'$ deux éléments non proportionnels de $A$. On a

$$
n(2\gamma, \gamma') = 2n(\gamma, \gamma') = 4n(\gamma, 2\gamma') \in 4\mathbf{Z}, \quad \text{et} \quad |n(\gamma, \gamma')| \leq 1
$$

puisque $\gamma$ et $\gamma'$ ont même longueur, d’où $n(\gamma, \gamma') = 0$ et $(\gamma|\gamma') = 0$.

#### Proposition 14 {#lie-vi-s1-prop-14 .statement}

Supposons que $R$ soit irréductible et réduit, et que $(\alpha|\alpha)$ prenne les valeurs $\lambda$ et $2\lambda$ pour $\alpha \in \mathbf{R}$. Soit $A$ l’ensemble des racines $\alpha$ telles que $(\alpha|\alpha) = \lambda$. On suppose que deux éléments de $A$ non proportionnels sont orthogonaux. Alors $R_1 = R \cup 2A$ est un système de racines irréductible non réduit et $R$ est l’ensemble des racines indivisibles de $R_1$.

Il est clair que $R_1$ vérifie (SR_I) et (SR_{II}). Soient $\alpha, \beta \in R_1$ et montrons que $\langle \alpha^\vee, \beta \rangle \in \mathbf{Z}$. C’est évident si $\alpha, \beta \in \mathbf{R}$. Comme $(2\alpha)^\vee = \frac{1}{2} \alpha^\vee$ pour $\alpha \in A$, c’est encore immédiat si $\alpha, \beta \in 2A$. Enfin, supposons $\beta \in \mathbf{R}$ et $\alpha = 2\gamma$ avec $\gamma \in A$.

1) Si $\gamma = \pm \beta$, on a $\langle \alpha^\vee, \beta \rangle = \pm \frac{1}{2} \langle \gamma^\vee, \gamma \rangle = \pm 1$.

2) Si $\gamma$ est non proportionnel à $\beta$ et si $\beta \in A$, l’hypothèse faite sur $A$ entraîne que $\langle \gamma^\vee, \beta \rangle = 0$, d’où $\langle \alpha^\vee, \beta \rangle = 0$.

3) Si $\beta \in \mathbf{R} - A$, on a $(\beta|\beta) = 2\lambda = 2(\gamma|\gamma)$, donc $\langle \beta, \gamma^\vee \rangle$ est égal soit à 0, soit à 2, soit à $-2$ d’après la liste du no 3. Donc $\langle \beta, \alpha^\vee \rangle = \frac{1}{2} \langle \beta, \gamma^\vee \rangle \in \mathbf{Z}$.

n° 1.5.

Ainsi, $R_1$ est un système de racines dans $V$, et les autres assertions sont évidentes.

### 5. Chambres et bases d’un système de racines

Pour tout $\alpha \in \mathbf{R}$, soit $L_\alpha$ l’hyperplan de $V$ formé des points invariants par $s_\alpha$. Les chambres déterminées dans $V$ par l’ensemble des $L_\alpha$ (chap. V, § 1, n° 3) s’appellent les *chambres* de $R$. La bijection $V \to V^*$ définie par le produit scalaire $(x|y)$ transforme $\alpha$ en $\frac{2\alpha^\vee}{(\alpha^\vee|\alpha^\vee)}$ pour $\alpha \in \mathbf{R}$, donc $L_\alpha$ en $L_{\alpha^\vee}$, donc les chambres de $R$ en celles de $R^\vee$. Si $C$ est une chambre de $R$, nous noterons $C^\vee$ la chambre correspondante de $R^\vee$. D’après la prop. 7 du n° 2, $C^\vee$ dépend uniquement de $C$, et non du choix de $(x|y)$.

#### Théorème 2 {#lie-vi-s1-thm-2 .statement}

(i) *Le groupe* $W(R)$ *opère de façon simplement transitive sur l’ensemble des chambres*.

(ii) *Soit* $C$ *une chambre. Alors* $\overline{C}$ *est un domaine fondamental pour* $W(R)$.

(iii) $C$ *est un cône simplicial ouvert* (chap. V, § 1, n° 6).

(iv) *Soient* $L_1, L_2, \ldots, L_l$ *les murs de* $C$. *Pour tout* $i$, *il existe une racine indivisible* $\alpha_i$ *et une seule telle que* $L_i = L_{\alpha_i}$ *et telle que* $\alpha_i$ *soit du même côté de* $L_i$ *que* $C$.

(v) *L’ensemble* $B(C) = \{\alpha_1, \ldots, \alpha_l\}$ *est une base de* $V$.

(vi) $C$ *est l’ensemble des* $x \in V$ *tels que* $\langle \alpha_i^\vee, x \rangle > 0$ *pour tout* $i$ *(ou, ce qui revient au même, l’ensemble des* $x \in V$ *tels que* $(x|\alpha_i) > 0$ *pour tout* $i$).

(vii) *Soit* $S$ *l’ensemble des* $s_{\alpha_i}$. *Le couple* $(W(R), S)$ *est un système de Coxeter* (chap. IV, § 1, n° 3).

Les assertions (i) et (vii) résultent du chap. V, § 3, n° 2, th. 1. L’assertion (ii) résulte du chap. V, § 3, n° 3, th. 2. L’assertion (iv) est évidente. La racine $\alpha_i$ est orthogonale à $L_i$, et $\alpha_i^\vee$ s’identifie à $2\alpha_i/(\alpha_i|\alpha_i)$. Comme $W(R)$ est essentiel (n° 1, *Remarque* 3), les assertions (iii), (v), (vi) résultent du chap. V, § 3, n° 9, prop. 7.

#### Remarque 1 {#lie-vi-s1-n5-rem-1 .statement}

L’assertion (vii) montre en particulier que $W(R)$ est *engendré* par les réflexions $s_{\alpha_i}$.

#### Remarque 2 {#lie-vi-s1-n5-rem-2 .statement}

Si $x, y \in C$, on a $(x|y) < 0$ (chap. V, § 3, n° 5, lemme 6), autrement dit l’angle $(\widehat{x, y})$ est *aigu*.

#### Remarque 3 {#lie-vi-s1-n5-rem-3 .statement}

Soit $m(\alpha, \beta)$ l’ordre de $s_\alpha s_\beta$ ($\alpha, \beta \in B(C)$). La matrice $(m(\alpha, \beta))$ s’identifie à la *matrice de Coxeter* (chap. IV, § 1, n° 9) de $(W, S)$. Si $\alpha \neq \beta$, la prop. 3 du chap. V, § 3, n° 4, montre que l’angle $(\widehat{\alpha, \beta})$ est égal à $\pi - \frac{\pi}{m(\alpha, \beta)}$; en particulier, cet angle est obtus ou droit, et l’on a $(\alpha|\beta) \leqslant 0$. En utilisant la liste du n° 3, *on voit que* $m(\alpha, \beta)$ *est égal à* 2, 3, 4 *ou* 6.

#### Définition 2 {#lie-vi-s1-def-2 .statement}

*Une partie* $B$ *de* $R$ *est appelée une base de* $R$ *s’il existe une chambre* $C$ *de* $R$ *telle que* $B = B(C)$. *Si* $C$ *est une chambre, on dit que* $B(C)$ *est la base de* $R$ *définie par* $C$.

#### Remarque 4 {#lie-vi-s1-n5-rem-4 .statement}

L’assertion (vi) du th. 2 montre que l’application $C \longmapsto B(C)$ est une bijection de l’ensemble des chambres sur l’ensemble des bases. Par suite, $W(R)$ opère de manière simplement transitive sur l’ensemble des bases.

#### Remarque 5 {#lie-vi-s1-n5-rem-5 .statement}

Soit $C$ une chambre de $R$, et soit $B$ la base correspondante. Si $\alpha \in B$, posons $\varphi(\alpha) = \alpha^\vee$ si $2\alpha \notin R$ et $\varphi(\alpha) = \frac{1}{2} \alpha^\vee$ si $2\alpha \in R$. Alors $\varphi(B)$ est la base de $R^\vee$ définie par $C^\vee$; cela résulte du fait que les murs de $C^\vee$ sont les $L_{\alpha^\vee}$, pour $\alpha \in B$.

#### Définition 3 {#lie-vi-s1-def-3 .statement}

Soit $B$ une base de $R$. On appelle matrice de Cartan de $R$ (relativement à $B$) la matrice $(n(\alpha, \beta))_{\alpha, \beta \in B}$.

On a $n(\alpha, \alpha) = 2$ pour tout $\alpha \in B$. Pour $\alpha, \beta \in B$, on a
$$
n(\alpha, \beta) = 2 \frac{(\alpha|\beta)}{(\beta|\beta)} = -2 \frac{\|\alpha\|}{\|\beta\|} \cos \frac{\pi}{m(\alpha, \beta)},
$$
où $m(\alpha, \beta)$ désigne comme précédemment l’ordre de $s_\alpha s_\beta$. Si $\alpha \neq \beta$, on a $n(\alpha, \beta) = 0, -1, -2$ ou $-3$ (cf. no 3).

#### Remarque 6 {#lie-vi-s1-n5-rem-6 .statement}

On ne confondra pas la matrice de Cartan $(n(\alpha, \beta))$ et la matrice de Coxeter $(m(\alpha, \beta))$. Noter d’ailleurs que la matrice de Cartan n’est pas nécessairement symétrique.

#### Remarque 7 {#lie-vi-s1-n5-rem-7 .statement}

Indexations canoniques. Si $B$ et $B'$ sont deux bases de $R$, il existe un unique élément $w \in W$ tel que $w(B) = B'$. On a
$$
n(w(\alpha), w(\beta)) = n(\alpha, \beta) \quad \text{et} \quad m(w(\alpha), w(\beta)) = m(\alpha, \beta)
$$
pour $\alpha, \beta \in B$. Par suite, les matrices de Cartan et de Coxeter associées à $B$ se déduisent de celles associées à $B'$ par composition avec la bijection
$$
\alpha \longmapsto w(\alpha)
$$
de $B$ sur $B'$.

On peut d’ailleurs définir des matrices de Cartan et de Coxeter canoniques de la manière suivante. Soit $X$ l’ensemble des couples $(B, \alpha)$, où $B$ est une base de $R$ et où $\alpha \in B$. Le groupe $W$ opère de manière évidente sur $X$ et une orbite de $W$ dans $X$ rencontre chacun des ensembles $\{B\} \times B$ en un point et un seul. Si $I$ est l’ensemble de ces orbites, chaque base $B$ admet donc une indexation canonique $(\alpha_i)_{i \in I}$. De plus, il existe une matrice $N = (n_{ij})$ (resp. $M = (m_{ij})$) et une seule, de type $I \times I$, telle que pour toute base $B$, la matrice de Cartan (resp. de Coxeter) associée à $B$ se déduise de $N$ (resp. $M$) par composition avec l’indexation canonique de $B$; on l’appelle la matrice de Cartan (resp. de Coxeter) canonique de $R$.

#### Proposition 15 {#lie-vi-s1-prop-15 .statement}

Soient $B$ une base de $R$ et $\alpha$ une racine indivisible. Il existe $\beta \in B$ et $w \in W(R)$ tels que $\alpha = w(\beta)$.

n° 1.6.

Soit C la chambre telle que $B = B(C)$. L’hyperplan $L_\alpha$ est mur d’une chambre $C'$ de $R$, et il existe un élément de $W(R)$ qui transforme $C'$ en $C$. On est donc ramené au cas où $L_\alpha$ est mur de $C$. Alors $\alpha$ est proportionnel à un élément $\beta$ de $B$. Comme $\alpha$ et $\beta$ sont indivisibles, on a $\alpha = \pm \beta$. Si $\alpha = -\beta$, on a $\alpha = s_\beta(\beta)$, d’où la proposition.

#### Corollaire {#lie-vi-s1-n5-cor-1 .statement}

Soient $R_1$ et $R_2$ deux systèmes de racines réduits dans des espaces vectoriels $V_1$ et $V_2$, et soient $B_1$ et $B_2$ des bases de $R_1$ et $R_2$. Soit $f : B_1 \to B_2$ une bijection qui transforme la matrice de Cartan de $R_1$ en celle de $R_2$. Il existe alors un isomorphisme $F : V_1 \to V_2$ qui transforme $R_1$ en $R_2$ et $\alpha$ en $f(\alpha)$ pour tout $\alpha \in B_1$.

Soit $F$ l’isomorphisme de $V_1$ sur $V_2$ qui transforme $\alpha$ en $f(\alpha)$ pour tout $\alpha \in B_1$. Alors $F$ transforme $s_\alpha$ en $s_{f(\alpha)}$, donc $W(R_1)$ en $W(R_2)$ (th. 2), donc $R_1$ en $R_2$ (prop. 15).

#### Proposition 16 {#lie-vi-s1-prop-16 .statement}

Soient $B$ une base de $R$, et $G$ le sous-groupe de $A(R)$ formé des éléments laissant stable $B$. Alors $W(R)$ est un sous-groupe distingué de $A(R)$ et $A(R)$ est produit semi-direct de $G$ et $W(R)$.

Si $\alpha \in R$ et $t \in A(R)$, on a $ts_\alpha t^{-1} = s_{t(\alpha)}$; comme $W(R)$ est engendré par les $s_\alpha$, on voit que $W(R)$ est un sous-groupe distingué de $A(R)$. Par transport de structure, $A(R)$ transforme une base de $R$ en une base de $R$. Comme $W(R)$ opère de façon simplement transitive sur l’ensemble des bases, tout élément de $A(R)$ s’écrit de manière unique sous la forme $g_1 g_2$, où $g_1 \in W(R)$ et $g_2 \in G$.

#### Remarque 8 {#lie-vi-s1-n5-rem-8 .statement}

Soient $R_1, \ldots, R_p$ des systèmes de racines dans les espaces vectoriels $V_1, \ldots, V_p$, $R$ la somme directe des $R_i$ dans $V = \prod_i V_i$, $C_i$ une chambre de $R_i$, $B_i = B(C_i)$. Il est immédiat que $C = \prod_i C_i$ est une chambre de $R$ et que $B(C) = \bigcup_i B_i$. Il résulte du th. 2 que les chambres et les bases de $R$ sont toutes obtenues par ce procédé.

### 6. Racines positives

Soit $C$ une chambre de $R$, et soit $B(C) = \{\alpha_1, \ldots, \alpha_l\}$ la base de $R$ correspondante. On appelle relation d’ordre définie par $C$ dans $V$ (resp. $V^*$) la relation d’ordre compatible avec la structure d’espace vectoriel de $V$ (resp. $V^*$) pour laquelle les éléments $\geqslant 0$ sont les combinaisons linéaires des $\alpha_i$ (resp. des $\alpha_i^\vee$) à coefficients $\geqslant 0$. On dira qu’un élément positif pour l’une de ces relations d’ordre est positif pour $C$, ou positif pour la base $B(C)$. Ces relations d’ordre sont aussi définies par $C^\vee$, comme on le voit en identifiant $V$ à $V^*$ à l’aide d’un produit scalaire invariant par $W(R)$. Compte tenu du th. 2, n° 5, un élément de $V^*$ est $\geqslant 0$ si et seulement si ses valeurs sur $C$ sont $\geqslant 0$. Un élément $x$ de $V$ est $\geqslant 0$ si et seulement si ses valeurs sur $C^\vee$ sont $\geqslant 0$, ou, ce qui revient au même, si $(x|y) \geqslant 0$ pour tout $y \in C$.

Les éléments de $\overline{C}$ sont $\geqslant 0$ pour $C$ d’après le lemme 6 du chap. V, § 3, n° 5. Mais l’ensemble des éléments $\geqslant 0$ pour $C$ est en général distinct de $\overline{C}$ (cf. planche X, systèmes $A_2, B_2, G_2$).

#### Théorème 3 {#lie-vi-s1-thm-3 .statement}

*Toute racine est combinaison linéaire à coefficients entiers de même signe d’éléments de $B(C)$*. *En particulier, toute racine est, soit positive, soit négative, pour $C$*.

Si $\alpha \in \mathbf{R}$, le noyau $L_\alpha$ de $\alpha$ ne rencontre pas $C^\vee$, donc $\alpha$ est, soit $> 0$ sur $C^\vee$ tout entier, soit $< 0$ sur $C^\vee$ tout entier, d’où la deuxième assertion. Il reste à prouver que $\alpha$ est contenu dans le *sous-groupe* $P$ de $V$ engendré par $B(C)$; on peut supposer $\alpha$ indivisible. Or le groupe $P$ est évidemment stable par les $s_\gamma$, pour $\gamma \in B(C)$, donc aussi par $W(\mathbf{R})$ d’après le th. 2. Comme $\alpha$ est de la forme $w(\beta)$, avec $w \in W(\mathbf{R})$ et $\beta \in B(C)$ (cf. prop. 15), on a bien $\alpha \in P$. C.Q.F.D.

On notera $R_+(C)$ l’ensemble des racines positives pour $C$. Ainsi,

$$
R = R_+(C) \cup (-R_+(C))
$$

est une partition de $R$.

#### Corollaire {#lie-vi-s1-n6-cor-1 .statement}

*Soient $\gamma$ une combinaison linéaire de racines à coefficients entiers, et $\alpha$ une racine indivisible. Si $\gamma$ est proportionnelle à $\alpha$, alors $\gamma \in \mathbf{Z}\alpha$*.

D’après la prop. 15 du n° 5, on peut choisir $C$ de telle sorte que $\alpha \in B(C)$. D’après le th. 3, on a :

$$
\gamma = \sum_{\beta \in B(C)} n_\beta \beta, \quad \text{avec} \quad n_\beta \in \mathbf{Z}.
$$

Si $\gamma$ est proportionnel à $\alpha$, on a donc $\gamma = n_\alpha \alpha$, ce qui démontre le corollaire.

Soit maintenant $S$ l’ensemble des réflexions $s_\alpha$ pour $\alpha \in B(C)$ et soit $T$ la réunion des conjugués de $S$ dans $W$. Pour $\alpha \in B(C)$ et $w \in W$, l’élément $t = ws_\alpha w^{-1}$ de $T$ est la réflexion orthogonale $s_\beta$ associée à la racine $\beta = w(\alpha)$; réciproquement, pour toute racine indivisible $\beta$, il existe un élément $w \in W$ tel que $\alpha = w^{-1}(\beta) \in B(C)$ (prop. 15) et on a $s_\beta = ws_\alpha w^{-1} \in T$. Il en résulte que l’on obtient une *bijection* $\psi$ de l’ensemble des racines indivisibles sur $\{ \pm 1 \} \times T$ en associant à une racine indivisible $\beta$ le couple $(\varepsilon, s_\beta)$, où $\varepsilon = +1$ si $\beta$ est positive et $\varepsilon = -1$ si $\beta$ est négative.

D’autre part, $(W, S)$ est un système de Coxeter (th. 2) et on peut lui appliquer les résultats du chap. IV, § 1, n° 4. Nous avons vu que, si $w$ est un élément de $W$ de longueur (par rapport à $S$) égale à $q$, il existe une partie $T_w$ de $T$, à $q$ éléments, telle que, si $w = s_1 \ldots s_q$ avec $s_i \in S$ et si l’on pose

$$
t_i = s_1 \ldots s_{i-1} s_i s_{i-1} \ldots s_1
$$

(pour $1 \leq i \leq q$), alors $T_w = \{ t_1, \ldots, t_q \}$. Rappelons que l’on a également défini au n° 4 du § 1 du chap. IV un nombre $\eta(w, t)$ (pour $w \in W$ et $t \in T$) égal à $+1$ si $t \notin T_w$ et à $-1$ si $t \in T_w$. Enfin, rappelons que, si l’on définit n° 1.6.

l’application $U_w$ de l’ensemble $\{ \pm 1 \} \times T$ dans lui-même par la formule
$$
U_w(\varepsilon, t) = (\varepsilon \eta(w^{-1}, t), wtw^{-1}),
$$
l’application $w \mapsto U_w$ est un *homomorphisme* de $W$ dans le groupe des permutations de l’ensemble $\{ \pm 1 \} \times T$ (chap. IV, § 1, n° 4, lemme 1).

#### Proposition 17 {#lie-vi-s1-prop-17 .statement}

*Supposons R réduit et soient $w \in W$ et $\alpha \in R$.*
(i) *On a $\psi(w(\alpha)) = U_w(\psi(\alpha))$.*
(ii) *Supposons $\alpha$ positive. La racine $w(\alpha)$ est négative si et seulement si*
$$
\eta(w^{-1}, s_\alpha) = -1,
$$
*autrement dit si $s_\alpha \in T_{w^{-1}}$.*
(iii) *On a $\eta(w, s_\alpha) = -1$ si et seulement si les chambres $C$ et $w(C)$ sont de part et d’autre de l’hyperplan $L_\alpha$. Autrement dit, l’ensemble $T_w$ se compose des réflexions par rapport aux murs séparant $C$ et $w(C)$.*
Soit $\beta \in B(C)$ et posons $s = s_\beta$. On a évidemment $T_s = \{ s \}$ et par suite :
$$
U_s(\varepsilon, t) = \begin{cases}
(\varepsilon, s t s^{-1}) & \text{si } t \neq s \\
(-\varepsilon, s) & \text{si } t = s.
\end{cases}
$$
(12)
D’autre part, soit $\rho = \sum_{\gamma \in B(C)} n_\gamma(\rho) \gamma$ une racine positive. Posons
$$
s(\rho) = \sum_{\gamma \in B(C)} n_\gamma(s(\rho)) \gamma.
$$
Si $\rho \neq \beta$, il existe un élément $\gamma \in B(C)$ avec $\gamma \neq \beta$, tel que $n_\gamma(\rho) > 0$, et l’on a $n_\gamma(s(\rho)) = n_\gamma(\rho) > 0$ (n° 1, formule (5)). Par suite $s(\rho)$ est *positive*. On en déduit aussitôt que :
$$
\psi(s(\varepsilon, \rho)) = \begin{cases}
(\varepsilon, ss_\rho s^{-1}) & \text{si } \rho \neq \beta \\
(-\varepsilon, s) & \text{si } \rho = \beta.
\end{cases}
$$
(13)
La comparaison de (12) et de (13) montre alors que $U_s(\psi(\gamma)) = \psi(s(\gamma))$ pour toute racine $\gamma$ et tout $s \in S$. Comme $S$ engendre $W$, on en déduit (i).
D’autre part, dire que $w(\alpha)$ est négative équivaut à dire que
$$
\psi(w(\alpha)) = (-1, ws_\alpha w^{-1}),
$$
ou encore d’après (i), que $U_w(\psi(\alpha)) = (-1, ws_\alpha w^{-1})$. Si de plus $\alpha$ est positive, on a $\psi(\alpha) = (+1, s_\alpha)$ et $U_w(\psi(\alpha)) = (\eta(w^{-1}, s_\alpha), ws_\alpha w^{-1})$, d’où (ii).
Enfin, on a, d’après (ii), $\eta(w, s_\alpha) = -1$ si et seulement si les racines $\alpha$ et $w^{-1}(\alpha)$ sont l’une positive et l’autre négative. Ceci équivaut à dire que $(\alpha|x).(w^{-1}(\alpha)|x) = (\alpha|x).(|\alpha|w(x)) < 0$ pour tout $x \in C$, d’où la première assertion de (iii). La seconde assertion de (iii) en résulte immédiatement.

#### Corollaire 1 {#lie-vi-s1-prop-17-cor-1 .statement}

*Soient $\beta \in B(C)$. La réflexion $s_\beta$ permutent entre elles les racines positives non proportionnelles à $\beta$.*

On se ramène aussitôt au cas où R est réduit. Dans ce cas, notre assertion résulte de (ii) et du fait que $T_{s_\beta} = \{ s_\beta \}$.

#### Corollaire 2 {#lie-vi-s1-prop-17-cor-2 .statement}

Supposons R réduit. Soit $w \in W$, soit q la longueur de w par rapport à S (chap. IV, § 1, n° 1), et soit $w = s_1 \ldots s_q$ une décomposition réduite de w. Soient $\alpha_1, \ldots, \alpha_q$ les éléments de B(C) correspondant à $s_1, \ldots, s_q$. Posons :

$$
\theta_i = s_q s_{q-1} \ldots s_{i+1}(\alpha_i), \quad i = 1, \ldots, q.
$$

Les racines $\theta_i$ sont $> 0$, deux à deux distinctes, on a $w(\theta_i) < 0$, et toute racine $\alpha > 0$ telle que $w(\alpha) < 0$ est égale à l’une des $\theta_i$.

Soit X l’ensemble des racines $\alpha > 0$ telles que $w(\alpha) < 0$. D’après (ii), on a

$$
\text{Card } (X) = \text{Card } (T_{w^{-1}}) = l(w^{-1}) = l(w) = q.
$$

D’autre part, si $\alpha \in X$, il est clair qu’il existe $i \in \{ 1, q \}$ tel que

$$
s_{i+1} \ldots s_q(\alpha) > 0 \quad \text{et} \quad s_i s_{i+1} \ldots s_q(\alpha) < 0.
$$

D’après le cor. 1, cela entraîne $s_{i+1} \ldots s_q(\alpha) = \alpha_i$, d’où $\alpha = \theta_i$. L’ensemble X est donc contenu dans l’ensemble des $\theta_i$. Puisque Card (X) = q, ceci n’est possible que si X est égal à l’ensemble des $\theta_i$, et si ceux-ci sont deux à deux distincts. D’où le corollaire.

#### Corollaire 3 {#lie-vi-s1-prop-17-cor-3 .statement}

Supposons R réduit. Il existe dans W un unique élément $w_0$ de plus grande longueur. Sa longueur est égale au nombre des racines positives et $w_0$ transforme la chambre C en — C. On a $w_0^2 = 1$ et $l(w w_0) = l(w_0) - l(w)$ pour tout $w \in W$.

Il est clair que — C est une chambre. Il existe donc un unique élément $w_0$ de W qui transforme C en — C. On a alors $w_0(\alpha) < 0$ pour toute racine positive $\alpha$ et les deux premières assertions du cor. 3 sont des conséquences immédiates du cor. 2. On a $w_0^2(C) = C$, d’où $w_0^2 = 1$. Enfin, si $w \in W$, la longueur $l(w)$ (resp. $l(w w_0)$) est égale, d’après la prop. 17 (iii), au nombre de murs séparant C et $w(C)$ (resp. $w w_0(C) = -w(C)$). Comme $w(C)$ et $-w(C)$ sont de part et d’autre de n’importe quel mur, la somme $l(w) + l(w w_0)$ est égale au nombre total de murs, c’est-à-dire à $l(w_0)$.

#### Proposition 18 {#lie-vi-s1-prop-18 .statement}

Soit $x \in V$. Les trois propriétés suivantes sont équivalentes :

(i) $x \in \overline{C}$.
(ii) $x \geq s_\alpha(x)$ pour tout $\alpha \in B(C)$ (au sens de la relation d’ordre définie par C).
(iii) $x \geq w(x)$ pour tout $w \in W$.

Comme $s_\alpha(x) = x - \langle x, \alpha^\vee \rangle \alpha$ et que $\overline{C}$ est l’ensemble des éléments $x \in V$ tels que $\langle x, \alpha^\vee \rangle \geq 0$ pour tout $\alpha \in B(C)$, l’équivalence de (i) et (ii) est évidente. D’autre part, il est clair que (iii) $\Longrightarrow$ (ii). Montrons que (i) $\Longrightarrow$ (iii). Soit $x \in \overline{C}$, et soit $w \in W$. Raisonnons par récurrence sur la longueur $l(w)$ de $w$. Le cas $l(w) = 0$ est trivial. Si $l(w) \geq 1$, on peut écrire $w$ sous la forme $w = w' s_\alpha$, n° 1.6.

avec $\alpha \in B(\mathbf{C})$ et $l(w') = l(w) - 1$. On a alors
$$
x - w(x) = x - w'(x) + w'(x - s_\alpha(x)).
$$
L’hypothèse de récurrence montre que $x - w'(x)$ est positif. D’autre part, on a
$$
w'(x - s_\alpha(x)) = w(s_\alpha(x) - x) = - \langle x, \alpha^\vee \rangle w(\alpha).
$$
Or $s_\alpha \in T_{w^{-1}}$, et la prop. 17, (ii) montre que $w(\alpha) < 0$. D’où le résultat.

#### Corollaire {#lie-vi-s1-n6-cor-2 .statement}

Pour que $x \in \mathbf{C}$, il faut et il suffit que $x > w(x)$ pour tout $w \in W$ tel que $w \neq 1$.

#### Proposition 19 {#lie-vi-s1-prop-19 .statement}

Soit $(\beta_i)_{1 \leq i \leq n}$ une suite de racines positives pour la chambre $C$ telle que $\beta_1 + \beta_2 + \cdots + \beta_n$ soit une racine. Il existe alors une permutation $\pi \in S_n$ telle que, pour tout $i \in \{1, 2, \ldots, n\}$, $\beta_{\pi(1)} + \beta_{\pi(2)} + \cdots + \beta_{\pi(i)}$ soit une racine.

Raisonnons par récurrence sur $n$, la proposition étant évidente pour $n \leq 2$. Posons $\beta = \beta_1 + \cdots + \beta_n$. On a $\sum_{i=1}^n (\beta|\beta_i) = (\beta|\beta) > 0$, donc il existe un indice $k$ tel que $(\beta|\beta_k) > 0$. Si $\beta = \beta_k$, on a $n = 1$ puisque $\beta_i > 0$ pour tout $i$. Sinon, $\beta - \beta_k$ est une racine (n° 3, cor. du th. 1); il suffit alors d’appliquer l’hypothèse de récurrence à $\beta - \beta_k = \sum_{i \neq k} \beta_i$.

#### Corollaire 1 {#lie-vi-s1-prop-19-cor-1 .statement}

Soit $\alpha \in R_+(\mathbf{C})$. Pour que $\alpha \notin B(\mathbf{C})$, il faut et il suffit que $\alpha$ soit somme de deux racines positives.

Si $\alpha$ est somme de deux racines positives, le th. 3 montre que $\alpha \notin B(\mathbf{C})$. Si $\alpha \notin B(\mathbf{C})$, le th. 3 montre que $\alpha = \sum_{k=1}^n \beta_k$ avec $\beta_k \in B(\mathbf{C})$ pour tout $k$ et $n \geq 2$. En permutant les $\beta_k$, on peut supposer que $\sum_{k=1}^{n-1} \beta_k$ est une racine (prop. 19), donc $\alpha$ est somme des racines positives $\sum_{k=1}^{n-1} \beta_k$ et $\beta_n$.

#### Corollaire 2 {#lie-vi-s1-prop-19-cor-2 .statement}

Soit $\varphi$ une application de $\mathbf{R}$ dans un groupe commutatif $\Gamma$ possédant les propriétés suivantes :
1) $\varphi(-\alpha) = -\varphi(\alpha)$ pour $\alpha \in \mathbf{R}$;
2) si $\alpha \in \mathbf{R}$, $\beta \in \mathbf{R}$ sont tels que $\alpha + \beta \in \mathbf{R}$, on a $\varphi(\alpha + \beta) = \varphi(\alpha) + \varphi(\beta)$.
Soit $Q$ le sous-groupe de $V$ engendré par $R$. Alors $\varphi$ se prolonge en un homomorphisme de $Q$ dans $\Gamma$.

Soit $B$ une base de $R$. Soit $\psi$ l’unique homomorphisme de $Q$ dans $\Gamma$ qui coïncide avec $\varphi$ sur $B$. Il suffit de montrer que $\psi(\alpha) = \varphi(\alpha)$ quand $\alpha$ est une racine positive pour $B$. On a $\alpha = \beta_1 + \cdots + \beta_m$ avec $\beta_i \in B$ pour tout $i$, et $\beta_1 + \cdots + \beta_h \in R$ pour tout $h$ (prop. 19). Montrons que $\psi(\alpha) = \varphi(\alpha)$ par récurrence sur $m$. C’est évident si $m = 1$. L’hypothèse de récurrence donne
$$
\psi(\beta_1 + \cdots + \beta_{m-1}) = \varphi(\beta_1 + \cdots + \beta_{m-1}),
$$
et on a $\psi(\beta_m) = \varphi(\beta_m)$, d’où $\psi(\alpha) = \varphi(\alpha)$, ce qui démontre le corollaire.

Pour toute racine $\alpha = \sum_{\beta \in B(C)} n_\beta \beta$ de $R$, notons $Y(\alpha)$ l’ensemble des $\beta \in B(C)$ tels que $n_\beta \neq 0$. Observons d’autre part que $B(C)$ s’identifie à l’ensemble des sommets du graphe du système de Coxeter formé par $W(R)$ et les $s_{x_i}$ (cf. chap. IV, § 1, no 9 et chap. V, § 3, no 2).

#### Corollaire 3 {#lie-vi-s1-prop-19-cor-3 .statement}

a) Soit $\alpha \in R$. Alors $Y(\alpha)$ est une partie connexe de $B(C)$ (chap. IV, Annexe).

b) Soit $Y$ une partie connexe non vide de $B(C)$. Alors $\sum_{\beta \in Y} \beta$ appartient à $R$.

Pour prouver a), on peut supposer $\alpha$ positive. Raisonnons par récurrence sur Card ($Y(\alpha)$), l’assertion étant triviale si Card ($Y(\alpha)$)$= 1$. D’après la prop. 19, il existe $\beta \in B(C)$ tel que $\alpha - \beta \in R$. Soit $p$ le plus grand entier $\geqslant 0$ tel que $\gamma = \alpha - p\beta \in R$. Comme $\gamma - \beta \in R$ et $\gamma + p\beta \in R$, on a $(\gamma|\beta) \neq 0$ (prop. 9); $\beta$ est donc liée à au moins un élément de $Y(\gamma)$. Mais $Y(\alpha) = Y(\gamma) \cup \{\beta\}$, et $Y(\gamma)$ est connexe d’après l’hypothèse de récurrence. Donc $Y(\alpha)$ est connexe, ce qui prouve a).

Soit maintenant $Y$ une partie connexe non vide de $B(C)$ et montrons par récurrence sur Card ($Y$) que $\sum_{\beta \in Y} \beta$ est une racine. Le cas où Card ($Y$)$\leqslant 1$ est trivial. Supposons que Card ($Y$)$\geqslant 2$. Comme $X$ est une forêt (chap. V, § 4, no 8, prop. 8), $Y$ est un arbre et possède un sommet terminal $\beta$ (chap. IV, Annexe). L’ensemble $Y - \{\beta\}$ est connexe, et un de ses éléments est lié à $\beta$. Vu l’hypothèse de récurrence, on a $\alpha = \sum_{\gamma \in Y - \{\beta\}} \gamma \in R$, et comme $(\alpha|\beta) < 0$, on a bien $\alpha + \beta \in R$ (th. 1).

C.Q.F.D.

### 7. Ensembles clos de racines

#### Définition 4 {#lie-vi-s1-def-4 .statement}

Soit $P$ un sous-ensemble de $R$.
(i) On dit que $P$ est clos si les conditions $\alpha \in P, \beta \in P, \alpha + \beta \in R$ impliquent $\alpha + \beta \in P$.
(ii) On dit que $P$ est parabolique si $P$ est clos et si $P \cup (-P) = R$.
(iii) On dit que $P$ est symétrique si $P = -P$.

#### Lemme 3 {#lie-vi-s1-lem-3 .statement}

Soient $C$ une chambre de $R$ et $P$ un sous-ensemble clos de $R$ contenant $R_+(C)$ (notation du no 6). Soient $\Sigma = B(C) \cap (-P)$, et $Q$ l’ensemble des racines combinaisons linéaires à coefficients entiers $\leqslant 0$ des éléments de $\Sigma$. Alors $P = R_+(C) \cup Q$.

Il s’agit de montrer que $P \cap (-R_+(C)) = Q$. Soit $-\alpha \in Q$. Alors $\alpha$ est somme de $n$ éléments de $\Sigma$. Montrons que $-\alpha \in P$, par récurrence sur $n$. C’est évident si $n = 1$. Si $n > 1$, on peut écrire, d’après la prop. 19 du no 6, $\alpha = \beta + \gamma$ avec $\gamma \in \Sigma$ et $\beta$ somme de $n - 1$ éléments de $\Sigma$. D’après l’hypothèse de récurrence, on a $-\beta \in P$; comme $-\gamma \in P$ et que $P$ est clos, on a $-\alpha \in P$. Donc $Q \subset P \cap (-R_+(C))$. Réciproquement, soit $-\alpha \in P \cap (-R_+(C))$. Alors $\alpha$ est somme de $p$ éléments de $B(C)$. Montrons que $-\alpha \in Q$, par récurrence sur $p$. C’est évident si $p = 1$. Si $p > 1$, on peut écrire, d’après la prop. 19, $\alpha = \beta + \gamma$ avec $\gamma \in B(C)$ et $\beta$ racine somme de $p - 1$ éléments de $B(C)$. Comme $-\gamma = \beta + (-\alpha)$ et que $P$ est clos, on a $-\gamma \in P$, donc $\gamma \in \Sigma$. D’autre part, $-\beta = \gamma + (-\alpha)$ donc $-\beta \in P$ parce que $P$ est clos. D’après l’hypothèse de récurrence, on a $-\beta \in Q$, donc $-\alpha = -\beta - \gamma \in Q$. Donc $P \cap (-R_+(C)) \subset Q$.

#### Proposition 20 {#lie-vi-s1-prop-20 .statement}

Soit $P$ un sous-ensemble de $R$. Les conditions suivantes sont équivalentes :
(i) $P$ est parabolique ;
(ii) $P$ est clos et il existe une chambre $C$ de $R$ telle que $P \supset R_+(C)$;
(iii) il existe une chambre $C$ de $R$ et une partie $\Sigma$ de $B(C)$ telle que $P$ soit la réunion de $R_+(C)$ et de l’ensemble $Q$ des racines combinaisons linéaires à coefficients entiers $\leq 0$ des éléments de $\Sigma$.

(ii) $\Longrightarrow$ (iii) : ceci résulte du lemme 3.
(iii) $\Longrightarrow$ (i) : adoptons les hypothèses et les notations de (iii). Il est clair que $P \cup (-P) = R$. Soient $\alpha, \beta \in P$ tels que $\alpha + \beta \in R$, et montrons que $\alpha + \beta \in P$. C’est évident si la racine $\alpha + \beta$ est positive. Supposons $\alpha + \beta$ négative. On a donc $\alpha + \beta = \sum_{\gamma \in B(C)} n_\gamma \gamma$, avec $n_\gamma \leq 0$. Mais le coefficient de tout élément $\gamma$ de $B(C) - \Sigma$ dans $\alpha$ ou $\beta$ est $\geq 0$; on a donc $n_\gamma = 0$ si $\gamma \in B(C) - \Sigma$, d’où $\alpha + \beta \in Q \subset P$.

(i) $\Longrightarrow$ (ii) : supposons $P$ parabolique. Soit $C$ une chambre telle que Card $(P \cap R_+(C))$ soit le plus grand possible. Soit $\alpha \in B(C)$ et supposons que $\alpha \notin P$, donc que $-\alpha \in P$. Pour tout $\beta \in P \cap R_+(C)$, $\beta$ est non proportionnel à $\alpha$ (car l’hypothèse $\beta = 2\alpha$ entraînerait $\alpha = 2\alpha + (-\alpha) \in P$ puisque $P$ est clos). Donc $s_\alpha(\beta) \in R_+(C)$ (n° 6, cor. 1 de la prop. 17). Si on pose $C' = s_\alpha(C)$, on a donc $\beta = s_\alpha(s_\alpha(\beta)) \in s_\alpha(R_+(C)) = R_+(C')$. Ainsi, $P \cap R_+(C) \subset P \cap R_+(C')$. Par ailleurs, $-\alpha = s_\alpha(\alpha) \in s_\alpha(R_+(C)) = R_+(C')$, donc $-\alpha \in P \cap R_+(C')$, donc Card $(P \cap R_+(C')) >$ Card $(P \cap R_+(C))$. Ceci est absurde, donc $\alpha \in P$. Donc $B(C) \subset P$, et par suite $R_+(C) \subset P$ d’après la prop. 19 et le fait que $P$ est clos.

#### Corollaire 1 {#lie-vi-s1-prop-20-cor-1 .statement}

Soit $P$ un sous-ensemble de $R$. Les conditions suivantes sont équivalentes :
(i) il existe une chambre $C$ telle que $P = R_+(C)$;
(ii) $P$ est clos, et $\{P, -P\}$ est une partition de $R$.
La chambre $C$ telle que $P = R_+(C)$ est alors unique.
(i) $\Longrightarrow$ (ii) : ceci résulte du th. 3 (n° 6).
(ii) $\Longrightarrow$ (i) : ceci résulte de l’implication (i) $\Longrightarrow$ (ii) de la prop. 20.
Si $P = R_+(C)$, $C^\vee$ est l’ensemble des $x^* \in V^*$ tels que $\langle x^*, x \rangle > 0$ pour tout $x \in P$, d’où l’unicité de $C$.

#### Corollaire 2 {#lie-vi-s1-prop-20-cor-2 .statement}

Supposons $V$ muni d’une structure d’espace vectoriel ordonné telle que, pour cette structure, toute racine de $R$ soit positive ou négative. Soit $P$ l’ensemble des racines positives pour cette structure. Alors il existe une chambre C de R et une seule telle que P = R_+(C).

En effet, P vérifie la condition (ii) du cor. 1.
Ce corollaire s’applique en particulier lorsque l’ordre considéré est total, la condition sur R étant alors automatiquement remplie. Rappelons qu’on obtient par exemple un tel ordre en choisissant une base (e_i)_{1 \leq i \leq n} dans V et en prenant sur V l’ordre lexicographique, où $x = \sum_i \xi_i e_i$ est $\geq 0$ si tous les $\xi_i$ sont 0, ou si $\xi_i > 0$ pour le plus petit indice i tel que $\xi_i \neq 0$.

#### Corollaire 3 {#lie-vi-s1-prop-20-cor-3 .statement}

Pour qu’une partie B de R soit une base de R, il faut et il suffit que les conditions suivantes soient remplies :

(i) les éléments de B sont linéairement indépendants ;
(ii) toute racine de R est combinaison linéaire d’éléments de B à coefficients tous positifs ou tous négatifs ;
(iii) toute racine de B est indivisible.

On sait déjà que les conditions sont nécessaires (n° 5, th. 2, et n° 6, th. 3). Supposons les conditions (i), (ii), (iii) vérifiées. Soit P l’ensemble des racines qui sont combinaisons linéaires à coefficients $\geq 0$ des éléments de B. Puisque P vérifie la condition (ii) du cor. 1, il existe une chambre C telle que P = R_+(C); soit B' = B(C), et soient X et X' les cônes convexes engendrés par B et B'.
On a
$$
B \subset P \subset X \quad \text{et} \quad B' \subset P \subset X',
$$
ce qui montre que X et X' sont tous deux engendrés par P, donc coïncident. Mais les demi-droites engendrées par les éléments de B (resp. de B') sont les génératrices extrémales de X (resp. de X'); comme une telle demi-droite ne contient qu’une seule racine indivisible, on a donc B = B'.

#### Corollaire 4 {#lie-vi-s1-prop-20-cor-4 .statement}

Soient B une base de R, B' une partie de B, V' le sous-espace vectoriel de V engendré par B', et R' = R \cap V'. Alors B' est une base du système de racines R'.

Ceci résulte aussitôt du cor. 3, et du cor. de la prop. 4.

On dit que R' est le système de racines engendré par B'.

#### Corollaire 5 {#lie-vi-s1-prop-20-cor-5 .statement}

Soient B une base de R, A_1, A_2, ..., A_r des parties de B deux à deux orthogonales, et A = A_1 \cup A_2 \cup ... \cup A_r. Alors toute racine $\alpha$ qui est combinaison linéaire d’éléments de A est déjà combinaison linéaire des éléments d’un des A_i. En particulier, si R est irréductible, il n’existe pas de partition de B(C) en deux ensembles orthogonaux.

Soient E_1, ..., E_r, E les sous-espaces vectoriels de V engendrés respectivement par A_1, ..., A_r, A. Grâce au cor. 4, on peut supposer que E = V. Alors, d’après le th. 2 (vii) du n° 5, les E_i sont stables par W(R), donc R est réunion des R \cap E_i (n° 2, prop. 5).

n° 1.7.

#### Corollaire 6 {#lie-vi-s1-prop-20-cor-6 .statement}

Adoptons les hypothèses et les notations de la prop. 20. Soit $V_1$ le sous-espace vectoriel de $V$ engendré par $\Sigma$. Alors $P \cap (-P) = Q \cup (-Q) = V_1 \cap R$ est un système de racines dans $V_1$ de base $\Sigma$.

On a $P \cap (-P) = (R_+(C) \cup Q) \cap ((--R_+(C)) \cup (--Q)) = Q \cup (--Q)$. Le th. 3 prouve que $Q \cup (--Q) = V_1 \cap R$. Enfin, $\Sigma$ est base du système de racines $V_1 \cap R$ d’après le cor. 4.

#### Proposition 21 {#lie-vi-s1-prop-21 .statement}

Soient $C$ (resp. $C'$) une chambre de $R$, $\Sigma$ (resp. $\Sigma'$) une partie de $B(C)$ (resp. $B(C')$), $Q$ (resp. $Q'$) l’ensemble des racines combinaisons linéaires à coefficients entiers négatifs des éléments de $\Sigma$ (resp. $\Sigma'$), et $P = Q \cup R_+(C)$ (resp. $P' = Q' \cup R_+(C')$). S’il existe un élément du groupe de Weyl transformant $P$ en $P'$, il existe un élément du groupe de Weyl transformant $C$ en $C'$ et $\Sigma$ en $\Sigma'$.

On se ramène aussitôt au cas où $P = P'$. Soit $V_1$ le sous-espace vectoriel de $V$ engendré par $P \cap (-P)$. Alors $\Sigma$ et $\Sigma'$ sont deux bases du système de racines $R_1 = P \cap (-P)$ dans $V_1$ (cor. 6 de la prop. 20). Il existe donc $g_1 \in W(R_1)$ tel que $g_1(\Sigma) = \Sigma'$. Il est clair que $g_1$ est induit par un élément $g$ de $W(R)$ qui est un produit de symétries $s_\sigma$, avec $\sigma \in \Sigma$. Soit $\gamma = \sum_{\beta \in B(C)} c_\beta \beta$ un élément de $P - R_1$. On a $c_\beta > 0$ pour au moins un $\beta \in B(C) - \Sigma$. D’autre part, si $\sigma \in \Sigma$, on a $s_\sigma(\gamma) - \gamma \in V_1$, donc $s_\sigma(\gamma)$ admet au moins une coordonnée $> 0$ par rapport à $B(C)$ (n° 1, formule (5)), d’où $s_\sigma(\gamma) \in R_+(C)$ et finalement $s_\sigma(\gamma) \in P - R_1$. Il en résulte que $P - R_1$ est stable par les $s_\sigma, \sigma \in \Sigma$, donc par $g$, et l’on a $g(P) = P$. On est ainsi ramené à prouver la proposition lorsque $P = P'$ et $\Sigma = \Sigma'$. Dans ce cas, on a $Q = Q'$, donc $R_+(C) = P - Q = P - Q' = R_+(C')$, donc $C = C'$ (cor. 1 de la prop. 20).

#### Corollaire {#lie-vi-s1-n7-cor-1 .statement}

Soient $P, P'$ deux sous-ensembles paraboliques de $R$ transformés l’un de l’autre par un élément du groupe de Weyl. S’il existe une chambre $C$ de $R$ telle que $R_+(C) \subset P$ et $R_+(C) \subset P'$, on a $P = P'$.

Ceci résulte du lemme 3 et de la prop. 21 puisque le seul élément de $W(R)$ transformant $C$ en $C$ est 1, cf. n° 5, th. 2.

#### Proposition 22 {#lie-vi-s1-prop-22 .statement}

Soit $P$ un sous-ensemble clos de $R$ tel que $P \cap (-P) = \varnothing$. Il existe alors une chambre $C$ de $R$ telle que $P \subset R_+(C)$.

1) Compte tenu du cor. du th. 1, n° 3, les hypothèses $\alpha \in P, \beta \in P, (\alpha|\beta) < 0$ impliquent $\alpha + \beta \in P$.

2) Montrons qu’aucune somme $\alpha_1 + \cdots + \alpha_q (q \geqslant 1)$ d’éléments de $P$ n’est nulle. On procède par récurrence sur $q$. L’assertion étant évidente pour $q = 1$, supposons $q \geqslant 2$. Si $\alpha_1 + \cdots + \alpha_q = 0$, alors

$$
-\alpha_1 = \alpha_2 + \cdots + \alpha_q,
$$

donc $(-\alpha_1|\alpha_2 + \cdots + \alpha_q) > 0$, d’où l’existence d’un $j \in [2, q]$ tel que $(\alpha_1|\alpha_j) < 0$. D’après la partie 1) de la démonstration, on a $\alpha_1 + \alpha_j \in P$, et la relation $(\alpha_1 + \alpha_j) + \sum_{i \neq 1, j} \alpha_i = 0$ contredit l’hypothèse de récurrence.

3) Montrons qu’il existe un élément γ non nul dans V tel que $(\gamma|\alpha) \geqslant 0$ pour tout $\alpha \in P$. Dans le cas contraire, le résultat de 1) prouverait qu’on peut trouver une suite infinie $\alpha_1, \alpha_2, \ldots$ d’éléments de P tels que

$$
\beta_i = \alpha_1 + \cdots + \alpha_i \in P
$$

pour tout i; il existerait deux entiers distincts $i, j$ tels que $\beta_i = \beta_j$, ce qui contredirait le résultat de 2).

4) Pour démontrer la proposition, il suffit (cor. 2 de la prop. 20) de montrer qu’il existe une base $(\alpha_k)_{1 \leq k \leq l}$ de V telle que, pour la relation d’ordre lexicographique définie par cette base, tout élément de P soit > 0. Procédons par récurrence sur $l = \dim V$, en supposant la proposition établie pour les dimensions < l. Soit $\gamma \in V$ tel que $\gamma \neq 0$ et $(\gamma|\alpha) \geqslant 0$ pour tout $\alpha \in P$ (cf. 3)). Soient L l’hyperplan orthogonal à $\gamma$, et $V'$ le sous-espace de L engendré par $R \cap L$. Alors $R \cap L$ est un système de racines dans $V'$ et $P \cap L$ est clos dans $R \cap L$. D’après l’hypothèse de récurrence, il existe une base $(\beta_1, \ldots, \beta_{l'})$ de $V'$ telle que les éléments de $P \cap L$ soient > 0 pour l’ordre lexicographique défini par cette base. Alors toute base de V dont les $l' + 1$ premiers éléments sont $\gamma, \beta_1, \beta_2, \ldots, \beta_{l'}$ et dont les éléments suivants sont dans L possède la propriété requise.

#### Proposition 23 {#lie-vi-s1-prop-23 .statement}

*Soient P un sous-ensemble de R et V₁ (resp. Γ) le sous-espace vectoriel (resp. le sous-groupe) de V engendré par P. Les conditions suivantes sont équivalentes* :

(i) *P est clos et symétrique*;
(ii) *P est clos, et P est un système de racines dans V₁*;
(iii) $\Gamma \cap R = P$.

*Supposons qu’il en soit ainsi. Pour tout $\alpha \in P$, soit $\alpha_1^\vee$ la restriction de $\alpha^\vee$ à $V_1$. Alors l’application $\alpha \mapsto \alpha_1^\vee$ est la bijection canonique du système de racines P sur $P^\vee$*.

(iii) $\Longrightarrow$ (i) : évident.

(i) $\Longrightarrow$ (ii) : supposons P clos et symétrique. D’abord P vérifie (SR₁) dans $V_1$. Soient $\alpha, \beta \in P$, et montrons que $s_\alpha(\beta) \in P$. C’est évident si $\alpha$ et $\beta$ sont proportionnels. Sinon, on a $s_\alpha(\beta) = \beta - n(\beta, \alpha)\alpha$ et $\beta - p\alpha \in R$ pour tout entier rationnel $p$ compris entre 0 et $n(\beta, \alpha)$ (prop. 9, no 3), donc

$$
\beta - n(\beta, \alpha)\alpha \in P
$$

puisque P est clos et symétrique. Ainsi, $s_{\alpha, \alpha_1^\vee}(P) = P$, et P vérifie (SR₂). Il est clair que P vérifie (SR₃). Donc P vérifie (ii), et on a en même temps prouvé la dernière assertion de la proposition.

(ii) $\Longrightarrow$ (iii) : supposons vérifiée la condition (ii), et prouvons que $\Gamma \cap R = P$. Il est clair que $P \subset \Gamma \cap R$. Soit $\beta \in \Gamma \cap R$. Puisque $\beta \in \Gamma$ et que $P = -P$, on a $\beta = \alpha_1 + \alpha_2 + \cdots + \alpha_k$ avec $\alpha_1, \ldots, \alpha_k \in P$. Nous allons prouver que $\beta \in P$.

n° 1.8.

C’est évident si $k = 1$. Raisonnons par récurrence sur $k$. On a

$$
0 < (\beta|\beta) = \sum_{i=1}^{k} (\beta|\alpha_i),
$$

donc $(\beta|\alpha_i) > 0$ pour un indice $i$. Si $\beta = \alpha_i$, on a $\beta \in P$. Sinon, on a $\beta - \alpha_i \in \mathbf{R}$ (cor. du th. 1, n° 3), donc $\beta - \alpha_i \in P$ d’après l’hypothèse de récurrence, donc $\beta \in P$ puisque $P$ est clos.

Les conditions de la prop. 23 peuvent être réalisées avec $V_1 = V$ et pourtant $P \neq \mathbf{R}$. Par exemple, il peut arriver que $\mathbf{R}$ soit un système de type $G_2$ et $P$ un système de type $A_2$; cf. planche X.

#### Proposition 24 {#lie-vi-s1-prop-24 .statement}

*Soit $R'$ l’intersection de $R$ avec un sous-espace vectoriel de $V$, de sorte que $R'$ est un système de racines dans le sous-espace vectoriel $V'$ qu’il engendre* (cf. cor. de la prop. 4, n° 1). *Soit $B'$ une base de $R'$*.

(i) *Il existe une base de $R$ contenant $B'$*.

(ii) *$R'$ est l’ensemble des éléments de $R$ qui sont combinaisons linéaires des éléments de $B'$*.

L’assertion (ii) est évidente. Prouvons (i). Soit $(\varepsilon_1, \varepsilon_2, \ldots, \varepsilon_l)$ une base de $V$ telle que $B' = (\varepsilon_{p+1}, \varepsilon_{p+2}, \ldots, \varepsilon_l)$. L’ordre lexicographique sur $V$ correspondant à cette base définit une chambre $C$ de $R$. Il est clair que tout élément de $B'$ est minimal dans $R_+(C)$. Donc $B' \subset B(C)$.

### 8. Plus grande racine

#### Proposition 25 {#lie-vi-s1-prop-25 .statement}

*Supposons $R$ irréductible. Soit $C$ une chambre de $R$, et soit $B(C) = \{\alpha_1, \ldots, \alpha_l\}$ la base correspondante*.

(i) *Il existe une racine $\tilde{\alpha} = \sum_{i=1}^{l} n_i \alpha_i$ telle que, pour toute racine $\sum_{i=1}^{l} p_i \alpha_i$, on ait $n_1 \geq p_1, n_2 \geq p_2, \ldots, n_l \geq p_l$. En d’autres termes, $R$ possède un plus grand élément $\tilde{\alpha}$ pour la relation d’ordre définie par $C$*.

(ii) *On a $\tilde{\alpha} \in \overline{C}$*.

(iii) *On a $(\tilde{\alpha}|\tilde{\alpha}) \geq (\alpha'|\alpha')$ pour toute racine $\alpha'$*.

(iv) *Pour toute racine positive $\alpha'$ non proportionnelle à $\tilde{\alpha}$, on a $n(\alpha', \tilde{\alpha}) = 0$ ou 1*.

1) Soient $\alpha = \sum_{i=1}^{l} n_i \alpha_i, \beta = \sum_{i=1}^{l} p_i \alpha_i$ deux racines maximales pour l’ordre défini par $C$. On va prouver que $\alpha = \beta$, ce qui établira (i).

2) Si on avait $(\alpha|\alpha_i) < 0$ pour un indice $i$, on en déduirait que $\alpha + \alpha_i \in \mathbf{R}$ ou $\alpha = -\alpha_i$ (cor. du th. 1, n° 3), et ces deux éventualités sont absurdes d’après la maximalité de $\alpha$. Donc $(\alpha|\alpha_i) \geq 0$ pour tout $i$.

3) Si $\alpha < 0$, on a $\alpha < -\alpha$, ce qui est absurde. Donc $n_i \geq 0$ pour tout $i$. Soit $J$ l’ensemble des $i$ tels que $n_i > 0$, et $J'$ le complémentaire de $J$ dans $\{1, 2, \ldots, l\}$. On a $J \neq \varnothing$. Si $J'$ était non vide, il existerait un $i \in J$ et un i' \in J' tels que $(\alpha_i|\alpha_{i'}) < 0$ (cor. 5 de la prop. 20, n° 7); on aurait
$$
(\alpha|\alpha_{i'}) = \sum_{i \in J} n_i (\alpha_i|\alpha_{i'}) < 0
$$
puisque $(\alpha_j|\alpha_k) \leq 0$ quels que soient $j$ et $k$ distincts, et ceci contredirait 2). Donc $J' = \varnothing$ et $n_i > 0$ pour tout $i$.

4) On a $(\beta|\alpha_i) \geq 0$ pour tout $i$ d’après 2). On ne peut avoir $(\beta|\alpha_i) = 0$ pour tout $i$ puisque $\beta \neq 0$. On conclut alors de 3) que
$$
(\beta|\alpha) = \sum_i n_i (\beta|\alpha_i) > 0.
$$
Si $\gamma = \alpha - \beta \in \mathbf{R}$, on a $\alpha > \beta$ ou $\beta > \alpha$ (th. 3, n° 6), ce qui contredit la maximalité de $\alpha$ et $\beta$. Donc $\alpha = \beta$ (cor. du th. 1, n° 3).

5) D’après 2), on a $\tilde{\alpha} \in \overline{C}$. Soit $\alpha' \in \mathbf{R}$, et prouvons que $(\alpha'|\alpha') \leq (\tilde{\alpha}|\tilde{\alpha})$. Puisque $\overline{C}$ est un domaine fondamental pour $W(\mathbf{R})$, on peut supposer que $\alpha' \in \overline{C}$. On a $\tilde{\alpha} - \alpha' \geq 0$, donc $(\tilde{\alpha} - \alpha'|x) \geq 0$ pour tout $x \in \overline{C}$. En particulier $(\tilde{\alpha} - \alpha'|\tilde{\alpha}) \geq 0$ et $(\tilde{\alpha} - \alpha'|\alpha') \geq 0$, d’où $(\tilde{\alpha}|\tilde{\alpha}) \geq (\alpha'|\tilde{\alpha}) \geq (\alpha'|\alpha')$. Donc $n(\alpha', \tilde{\alpha})$ vaut 0 ou 1 ou — 1 (prop. 8, n° 3) si $\alpha'$ est non proportionnel à $\tilde{\alpha}$. Si $\alpha' \geq 0$, on a $(\tilde{\alpha}|\alpha') \geq 0$ d’après 2), donc $n(\alpha', \tilde{\alpha}) \geq 0$, donc $n(\alpha', \tilde{\alpha})$ vaut 0 ou 1.

C.Q.F.D.

#### Remarque {#lie-vi-s1-n8-rem-1 .statement}

On dit que la racine
$$
\tilde{\alpha} = \sum_i n_i \alpha_i
$$
de (i) est la plus grande racine de $\mathbf{R}$ (vis-à-vis de $\mathbf{C}$). On notera que, d’après (i), on a $n_i \geq 1$ pour tout $i$.

### 9. Poids, poids radiciels

Soit $l = \dim V$. On note $Q(R)$ le sous-groupe de $V$ engendré par $R$; les éléments de $Q(R)$ s’appellent les poids radiciels de $R$. D’après le th. 3 du n° 6, $Q(R)$ est un sous-groupe discret de rang $l$ de $V$, et toute base de $R$ est une base de $Q(R)$.
De même, le groupe $Q(R^\vee)$ est un sous-groupe discret de rang $l$ de $V^*$.

#### Proposition 26 {#lie-vi-s1-prop-26 .statement}

L’ensemble des $x \in V$ tels que $\langle x, y^* \rangle \in \mathbf{Z}$ pour tout $y^* \in Q(R^\vee)$ (ou, ce qui revient au même, pour tout $y^* \in R^\vee$) est un sous-groupe discret $G$ de $V$ contenant $Q(R)$. Si $B'$ est une base de $R^\vee$, la base duale de $B'$ dans $V$ est une base de $G$.
Soit $x \in V$. Les trois propriétés suivantes sont équivalentes :
(i) $\langle x, y^* \rangle \in \mathbf{Z}$ pour tout $y^* \in Q(R^\vee)$;
(ii) $\langle x, y^* \rangle \in \mathbf{Z}$ pour tout $y^* \in B'$;
(iii) les coordonnées de $x$ par rapport à la base duale de $B'$ sont dans $\mathbf{Z}$.

On en conclut que la base duale de $B'$ est une base de $G$. D’autre part, (SR_{III}) prouve que $R \subset G$, d’où $Q(R) \subset G$.

Le groupe $G$ de la prop. 26 se note $P(R)$, et ses éléments s’appellent les *poids* de $R$. On peut considérer aussi le groupe $P(R^\vee)$ des poids de $R^\vee$.

D’après *Alg.*, chap. VII, 2e éd., § 4, no 8, les groupes

$$
P(R)/Q(R), \quad P(R^\vee)/Q(R^\vee)
$$

sont des groupes finis en dualité sur $\mathbf{Q}/\mathbf{Z}$, donc isomorphes. L’ordre commun de ces deux groupes s’appelle l'*indice de connexion* de $R$ (ou de $R^\vee$).

Si $R$ est somme directe de systèmes de racines $R_i$, le groupe $Q(R)$ (resp. $P(R)$) s’identifie canoniquement à la somme directe des $Q(R_i)$ (resp. $P(R_i)$).

#### Proposition 27 {#lie-vi-s1-prop-27 .statement}

*Soient* $R_1$ *une partie de* $R$, $Q_1$ *le sous-groupe de* $Q(R)$ *engendré par* $R_1$, *et* $W_1$ *le sous-groupe de* $W(R)$ *engendré par les* $s_\alpha$ ($\alpha \in R_1$). *Si* $p \in P(R)$ *et* $w \in W_1$, *on a* $p - w(p) \in Q_1$.

*Si* $w = s_\alpha$ *avec* $\alpha \in R_1$, *on a*

$$
p - w(p) = \langle p, \alpha^\vee \rangle \alpha \in \mathbf{Z}\alpha \subset Q_1.
$$

*Si* $w = s_{\alpha_1} s_{\alpha_2} \ldots s_{\alpha_r}$ *avec* $\alpha_1, \ldots, \alpha_r \in R_1$, *on a donc encore* $p - w(p) \in Q_1$ *comme on le voit par récurrence sur* $r$.

Le groupe $A(R)$ laisse invariants $P(R)$ et $Q(R)$, donc opère dans le groupe quotient $P(R)/Q(R)$. D’après la prop. 27, le groupe $W(R)$ opère trivialement dans $P(R)/Q(R)$. Par passage au quotient, on voit que *le groupe quotient* $A(R)/W(R)$ (cf. prop. 16, no 5) *opère canoniquement dans* $P(R)/Q(R)$.

### 10. Poids fondamentaux, poids dominants

Supposons $R$ *réduit*. Soit $C$ une chambre de $R$, et soit $B$ la base de $R$ correspondante. Comme $R$ est réduit, $B^\vee = \{\alpha^\vee\}_{\alpha \in B}$ est une base de $R^\vee$. La *base duale* $(\overline{\omega}_\alpha)_{\alpha \in B}$ de $B^\vee$ est donc une base du groupe des poids; ses éléments s’appellent les *poids fondamentaux* (relativement à $B$, ou à $C$); lorsque les éléments de $B$ sont numérotés $(\alpha_1, \ldots, \alpha_l)$, on note $(\overline{\omega}_1, \ldots, \overline{\omega}_l)$ les poids fondamentaux correspondants.

Soit $x \in V$. Pour que $x \in C$, il faut et il suffit que $\langle x, \alpha^\vee \rangle > 0$ pour tout $\alpha \in B$. Il s’ensuit que $C$ est l’ensemble des combinaisons linéaires des $\overline{\omega}_\alpha$ à coefficients $> 0$, et $\overline{C}$ l’ensemble des combinaisons linéaires des $\overline{\omega}_\alpha$ à coefficients $\geqslant 0$.

Les éléments $n(\alpha, \beta) = \langle \alpha, \beta^\vee \rangle$ de la matrice de Cartan sont, pour $\alpha$ fixé, les coordonnées de $\alpha$ par rapport à la base $(\overline{\omega}_\beta)_{\beta \in B}$:

$$
\alpha = \sum_{\beta \in B} n(\alpha, \beta) \overline{\omega}_\beta.
$$

La matrice de Cartan est donc la transposée de la matrice de l’injection canonique

$$
\mathbf{Q}(R) \to \mathbf{P}(R)
$$

par rapport aux bases $B$ et $(\varpi_\alpha)_{\alpha \in B}$ des $\mathbf{Z}$-modules $\mathbf{Q}(R)$ et $\mathbf{P}(R)$.

Un poids $\varpi$ est dit dominant s’il appartient à $\overline{C}$, autrement dit si ses coordonnées par rapport à $(\varpi_\alpha)_{\alpha \in B}$ sont des entiers $\geqslant 0$, ou encore si $g(\varpi) \leqslant \varpi$ pour tout $g \in W(R)$ (n° 6, prop. 18). Puisque $\overline{C}$ est un domaine fondamental pour $W(R)$ (th. 2), il existe, pour tout poids $\varpi$, un poids dominant $\varpi'$ et un seul tel que $\varpi'$ soit transformé de $\varpi$ par $W(R)$.

On a

$$
\langle \varpi_\alpha, \beta^\vee \rangle = (\varpi_\alpha | \frac{2\beta}{|\beta|}) = \delta_{\alpha \beta}
$$

pour $\alpha, \beta \in B$ ($\delta_{\alpha \beta}$ désignant le symbole de Kronecker), d’où

$$
s_\beta(\varpi_\alpha) = \varpi_\alpha - \delta_{\alpha \beta} \beta \quad \text{et} \quad (\varpi_\alpha | \beta) = \frac{1}{2} (\beta | \beta) \delta_{\alpha \beta}.
$$

Autrement dit, $\varpi_\alpha$ est orthogonal à $\beta$ pour $\beta \neq \alpha$, et sa projection orthogonale sur $R \alpha$ est $\frac{1}{2} \alpha$. Puisque $\varpi_\alpha \in \overline{C}$, on a $(\varpi_\alpha | \varpi_\beta) \geqslant 0$ pour $\alpha, \beta \in B$, i.e. l’angle $(\overline{\varpi_\alpha}, \overline{\varpi_\beta})$ est aigu ou droit. Les poids dominants sont les $\varpi \in V$ tels que $2(\varpi | \alpha)/(|\alpha|)$ soit un entier $\geqslant 0$ pour tout $\alpha \in B$.

#### Proposition 28 {#lie-vi-s1-prop-28 .statement}

*Soient B une base de R, B' une partie de B, V' le sous-espace vectoriel de V engendré par B', R' = R ∩ V' (qui est un système de racines dans V'), R'∨ le système de racines inverse (qui s’identifie à l’image canonique de R' dans R∨), V_1 l’orthogonal de R'∨ dans V, et p le projecteur de V sur V' parallèlement à V_1. Alors, Q(R') = Q(R) ∩ V', P(R') = p(P(R)). L’ensemble des poids dominants de R' est l’image par p de l’ensemble des poids dominants de R.*

En effet, $\mathbf{Q}(R)$ est le sous-groupe de $V$ de base $B$, $\mathbf{Q}(R')$ est le sous-groupe de $V$ de base $B'$ (n° 7, cor. 4 de la prop. 20) d’où aussitôt $\mathbf{Q}(R') = \mathbf{Q}(R) \cap V'$. Si $\varpi \in \mathbf{P}(R)$ et $\alpha \in R'$, on a $\langle p(\varpi), \alpha^\vee \rangle = \langle \varpi, \alpha^\vee \rangle \in \mathbf{Z}$, donc $p(\varpi) \in \mathbf{P}(R')$, donc $p(\mathbf{P}(R)) \subset \mathbf{P}(R')$. Si $\varpi' \in \mathbf{P}(R')$, $\varpi'$ se prolonge en une forme linéaire $\varpi$ sur $V^*$ nulle sur $(B - B')^\vee$; on a $\langle \varpi, \alpha^\vee \rangle \in \mathbf{Z}$ pour tout $\alpha \in B$, donc $\varpi \in \mathbf{P}(R)$, et $\varpi' = p(\varpi)$; donc $\mathbf{P}(R') \subset p(\mathbf{P}(R))$. Ainsi $\mathbf{P}(R') = p(\mathbf{P}(R))$, et l’assertion relative aux poids dominants se démontre de la même façon.

#### Proposition 29 {#lie-vi-s1-prop-29 .statement}

*Soit $\rho$ la demi-somme des racines > 0.

(i) *On a $\rho = \sum_{\alpha \in B} \varpi_\alpha$; c’est un élément de C.*
(ii) $s_\alpha(\rho) = \rho - \alpha$ pour tout $\alpha \in B$.
(iii) *On a $(2\rho | \alpha) = (\alpha | \alpha)$ pour tout $\alpha \in B$.*

n° 1.11.

Comme R est réduit, on a $s_\alpha(\mathbf{R}_+(\mathbf{C}) - \{\alpha\}) = \mathbf{R}_+(\mathbf{C}) - \{\alpha\}$ et $s_\alpha(\alpha) = -\alpha$ pour $\alpha \in B$ (n° 6, cor. 1 de la prop. 17), d’où $s_\alpha(2\rho) = 2\rho - 2\alpha$. Comme $s_\alpha(\rho) = \rho - \langle \rho, \alpha^\vee \rangle \alpha$, on voit que
$$
\langle \rho, \alpha^\vee \rangle = 1 = \langle \sum_{\beta \in B} \varpi_\beta, \alpha^\vee \rangle.
$$
D’où $\rho = \sum_{\beta} \varpi_\beta$, et par suite $\rho \in \mathbf{C}$. Enfin (iii) équivaut à $\langle \rho, \alpha^\vee \rangle = 1$.

#### Corollaire {#lie-vi-s1-n10-cor-1 .statement}

*Soit $\sigma$ la demi-somme des éléments > 0 de $\mathbf{R}^\vee$ (pour $\mathbf{B}^\vee$). Pour tout $\alpha \in V$, la somme des coordonnées de $\alpha$ par rapport à la base $B$ est $\langle \alpha, \sigma \rangle$. Si $\alpha \in \mathbf{R}$, cette somme est aussi égale à $\frac{1}{2} \sum_{\beta \in \mathbf{R}_+(\mathbf{C})} n(\alpha, \beta)$.*

Échangeant les rôles de R et $\mathbf{R}^\vee$ dans ce qui précède, on a $\langle \alpha, \sigma \rangle = 1$ pour tout $\alpha \in B$, d’où le corollaire.

### 11. Transformation de Coxeter

Soit C une chambre de R, soit $\{\alpha_1, \ldots, \alpha_l\}$ la base de R correspondante, et soit $c = s_{x_1} \ldots s_{x_l}$. L’élément c de W s’appelle la *transformation de Coxeter* de W définie par C et la bijection $i \mapsto \alpha_i$ (chap. V, § 6, n° 1). Son ordre h est appelé le *nombre de Coxeter* de W (ou de R).

#### Proposition 30 {#lie-vi-s1-prop-30 .statement}

*Supposons R irréductible. Soit m un entier compris entre 1 et h—1, et étranger à h. Alors $\exp(\frac{2i\pi m}{h})$ est une valeur propre de c de multiplicité 1.*

(En particulier, m est un *exposant* de W, cf. chap. V, § 6, n° 2).
Démontrons d’abord un lemme:

#### Lemme 3 {#lie-vi-s1-lem-3-bis .statement}

*Pour tout $w \in W$, le polynôme caractéristique de w est à coefficients entiers.*
On sait (n° 6, th. 3) que le sous-groupe Q(R) de V engendré par R a pour base $\{\alpha_1, \ldots, \alpha_l\}$. Comme w laisse stable Q(R), sa matrice par rapport à $\{\alpha_1, \ldots, \alpha_l\}$ est à coefficients entiers; il en est donc de même de son polynôme caractéristique.
Soit P le polynôme caractéristique de c. Le lemme ci-dessus montre que les coefficients de P sont entiers. D’après le chap. V, § 6, n° 2, cor. 2 de la prop. 3, la racine primitive h-ème de l’unité $z = \exp(\frac{2i\pi}{h})$ est une racine simple de P. Tout *conjugué* de z sur Q est donc aussi racine simple de P. Mais on sait (*) que toutes les racines primitives h-èmes de l’unité sont conjuguées sur Q. Elles sont donc toutes racines simples de P, ce qui démontre la proposition.

#### Proposition 31 {#lie-vi-s1-prop-31 .statement}

*Supposons R irréductible et réduit, et soit $\beta = n_1 \alpha_1 + \cdots + n_l \alpha_l$ la plus grande racine de R* (cf. n° 8). *On a alors $n_1 + \cdots + n_l = h — 1$*.

(*) Ce résultat figurera dans un chapitre d’Alg. comm. en préparation. En attendant, le lecteur pourra se reporter à D. Hilbert, Die Theorie der algebraischen Zahlkörper, § 97 (Gesamm. Abh., I, p. 63-363).

Soit $R_+$ l’ensemble des racines positives relativement à $C$. On a (n° 10, cor. de la prop. 29):

$$
n_1 + \cdots + n_l = \frac{1}{2} \sum_{\alpha \in R_+} n(\beta, \alpha)
$$
$$
= 1 + \frac{1}{2} \sum_{\alpha \in R_+, \alpha \neq \beta} n(\beta, \alpha) = 1 + \sum_{\alpha \in R_+, \alpha \neq \beta} \frac{(\alpha|\beta)}{(\alpha|\alpha)}.
$$

D’après le n° 8, prop. 25 (iv), on a, pour $\alpha \in R_+$ et $\alpha \neq \beta$, $n(\alpha, \beta) = 0$ ou $1$, donc $n(\alpha, \beta)^2 = n(\alpha, \beta)$, c’est-à-dire $\frac{4(\alpha|\beta)^2}{(\beta|\beta)^2} = \frac{2(\alpha|\beta)}{(\beta|\beta)}$. D’où :

$$
n_1 + \cdots + n_l + 1 = 2 + 2 \sum_{\alpha \in R_+, \alpha \neq \beta} \frac{(\alpha|\beta)^2}{(\beta|\beta)(\alpha|\alpha)}
$$
$$
= 2 \sum_{\alpha \in R_+} \frac{(\alpha|\beta)^2}{(\beta|\beta)(\alpha|\alpha)} = (\beta|\beta)^{-1} \sum_{\alpha \in R} \left( \frac{\alpha}{\|\alpha\|} |\beta \right)^2.
$$

D’après le chap. V, § 6, n° 2, cor. du th. 1, on a :

$$
\sum_{\alpha \in R} \left( \frac{\alpha}{\|\alpha\|} |\beta \right)^2 = h(\beta|\beta)
$$

d’où $n_1 + \cdots + n_l + 1 = h$.

#### Proposition 32 {#lie-vi-s1-prop-32 .statement}

*Supposons que R soit irréductible, et que toutes les racines aient même longueur. Soit $\alpha \in R$. Le nombre d’éléments de R non orthogonaux à $\alpha$ est $4h - 6$.*

Soit $R'$ l’ensemble des racines non proportionnelles et non orthogonales à $\alpha$. D’après le chap. V, § 6, n° 2, cor. du th. 1, on a

$$
(\alpha|\alpha)^2 + (\alpha|- \alpha)^2 + \sum_{\beta \in R'} (\alpha|\beta)^2 = h(\alpha|\alpha)^2,
$$

c’est-à-dire

$$
\sum_{\beta \in R'} (\alpha|\beta)^2 = (h - 2)(\alpha|\alpha)^2.
$$

Si $\beta \in R'$, on a $(\alpha|\beta) = \pm \frac{1}{2} (\alpha|\alpha)$ d’après la liste du n° 3. Donc

$$
\frac{1}{4} \operatorname{Card} R' = h - 2, \quad \operatorname{Card} R' = 4h - 8,
$$

et le nombre de racines non orthogonales à $\alpha$ est $\operatorname{Card} R' + 2 = 4h - 6$.

#### Proposition 33 {#lie-vi-s1-prop-33 .statement}

*Supposons R irréductible et réduit. Posons $s_{\alpha_i} = s_i$, et soit $\Gamma$ le sous-groupe de W engendré par $c = s_1 \ldots s_l$.*
(i) *Soit $\theta_i = s_i s_{i-1} \ldots s_{i+1}(\alpha_i)$ ($i = 1, \ldots, l$). On a $\theta_i > 0$, $c(\theta_i) < 0$.*
(ii) *Si $\alpha$ est une racine $> 0$ telle que $c(\alpha) < 0$, $\alpha$ est égale à l’une des $\theta_i$.*
(iii) *La famille $(\theta_i)_{1 \leq i \leq l}$ est une base de $Q(R)$.*
(iv) *Soit $\Omega_i$ l’orbite de $\theta_i$ pour $\Gamma$. Les ensembles $\Omega_i$ sont deux à deux disjoints, constituent toutes les orbites de $\Gamma$ dans $R$, et ont chacun $h$ éléments.*

n° 1.12.

Observons d’abord que $(s_1, \ldots, s_l)$ est une décomposition réduite de $c$ (chap. IV, § 1, n° 1) par rapport à l’ensemble $S$ des $s_i$. En effet, sinon, il existerait une partie $X = S - \{j\}$ à $l-1$ éléments de $S$ telle que $c \in W_X$; on aurait alors $s_j \in W_X$, ce qui contredirait le cor. 2 de la prop. 7 du chap. IV, § 1, n° 8.

En appliquant à $c = s_1 \ldots s_l$ le cor. 2 de la prop. 17 du n° 6, on obtient les assertions (i) et (ii).

Soit $Q_i$ le sous-groupe de $Q(\mathbf{R})$ engendré par les $\alpha_j, j > i$. On vérifie immédiatement que $Q_i$ est stable par les $s_j, j > i$, et que $s_j(\alpha_i) \equiv \alpha_i \mod Q_i$ pour $j > i$. On a donc:

$$
\theta_i = s_l \ldots s_{i+1}(\alpha_i) \equiv \alpha_i \mod Q_i.
$$

En d’autres termes, il existe des entiers $c_{ij}$ tels que:

$$
\theta_i = \alpha_i + \sum_{j > i} c_{ij} \alpha_j.
$$

D’où aussitôt (iii).

Enfin, soit $\alpha$ une racine. L’élément $\sum_{k=0}^{h-1} c^k(\alpha)$ est invariant par $c$, donc nul (chap. V, § 6, n° 2). Les $c^k(\alpha)$ ne peuvent donc pas être toutes de même signe, et il existe un $k$ tel que $c^k(\alpha) > 0$ et $c^{k+1}(\alpha) < 0$. D’après (ii), $c^k(\alpha)$ est l’un des $\theta_i$. Donc toute orbite de $\Gamma$ dans $\mathbf{R}$ est l’une des $\Omega_i$. Prolongeons alors $(x|y)$ en une forme hermitienne sur $V \otimes \mathbf{C}$. D’après la Remarque du chap. V, § 6, n° 2, il existe un élément $z \in V \otimes \mathbf{C}$ tel que $c(z) = \exp\left(\frac{2i\pi}{h}\right) z$ et que $(\gamma|z) \neq 0$ pour tout $\gamma \in \mathbf{R}$. Si $c^p(\alpha) = \alpha$, on a

$$
(z|\alpha) = (z|c^p(\alpha)) = (c^{-p}(z)|\alpha) = \exp\left(-\frac{2i\pi p}{h}\right)(z|\alpha),
$$

d’où $\exp\left(-\frac{2i\pi p}{h}\right) = 1$, et $p \equiv 0 \mod h$. Cela prouve que l’orbite de $\alpha$ possède $h$ éléments. D’après le th. 1 (ii) du chap. V, § 6, n° 2, le nombre total d’orbites de $\Gamma$ dans $\mathbf{R}$ est donc $\frac{hl}{h} = l$. Il en résulte que les $\Omega_i$ sont deux à deux disjointes, ce qui achève de prouver (iv).

### 12. Forme bilinéaire canonique

On a vu (n° 1, prop. 3) que la forme bilinéaire symétrique

$$
(x, y) \mapsto B_R(x, y) = \sum_{\alpha \in R} \langle \alpha^\vee, x \rangle \langle \alpha^\vee, y \rangle
$$

sur $V$ est non dégénérée et invariante par $A(R)$. Échangeant les rôles de $R$ et $R^\vee$, on voit que la forme bilinéaire symétrique $(x^*, y^*) \mapsto B_{R^\vee}(x^*, y^*) = \sum_{\alpha \in R} \langle \alpha, x^* \rangle \langle \alpha, y^* \rangle$ sur $V^*$ est non dégénérée et invariante par $A(R)$.

La forme inverse de $B_{R^\vee}$ (resp. $B_R$) sur $V$ (resp. $V^*$) sera appelée la *forme bilinéaire canonique* sur $V$ (resp. $V^*$) et notée $\Phi_R$ (resp. $\Phi_{R^\vee}$). Elle est non dégénérée et invariante par $A(R)$. Soit $\sigma$ l’isomorphisme de $V$ sur $V^*$ défini par $B_{R^\vee}$. On a, pour $x \in V$ et $y \in V$ :

$$
\Phi_R(x, y) = B_{R^\vee}(\sigma(x), \sigma(y)) = \sum_{\alpha \in R} \langle \alpha, \sigma(x) \rangle \langle \alpha, \sigma(y) \rangle.
$$

Mais $\langle \alpha, \sigma(x) \rangle = B_{R^\vee}(\sigma(\alpha), \sigma(x)) = \Phi_R(\alpha, x)$. D’où

$$
\Phi_R(x, y) = \sum_{\alpha \in R} \Phi_R(\alpha, x) \Phi_R(\alpha, y).
$$

Compte tenu de la prop. 7 du n° 2, $\Phi_R$ est la seule forme bilinéaire symétrique invariante par $W(R)$ et non nulle qui vérifie l’identité (16).

Pour $\beta \in R$, (16) donne

$$
\Phi_R(\beta, \beta) = \sum_{\alpha \in R} \Phi_R(\alpha, \beta)^2 = \frac{1}{4} \Phi_R(\beta, \beta)^2 \sum_{\alpha \in R} n(\alpha, \beta)^2
$$

d’où

$$
4 \Phi_R(\beta, \beta)^{-1} = \sum_{\alpha \in R} n(\alpha, \beta)^2.
$$

Par ailleurs, d’après le lemme 2 du n° 1, on a, pour $x, y \in V$ :

$$
B_R(x, y) = \sum_{\alpha \in R} \Phi_R\left( \frac{2\alpha}{\Phi_R(\alpha, \alpha)}, x \right) \Phi_R\left( \frac{2\alpha}{\Phi_R(\alpha, \alpha)}, y \right)
= 4 \sum_{\alpha \in R} \Phi_R(\alpha, x) \Phi_R(\alpha, y) \Phi_R(\alpha, \alpha)^{-2}.
$$

Si $R$ est *irréductible*, il existe donc une constante $\gamma(R) > 0$ telle que

$$
\sum_{\alpha \in R} \Phi_R(\alpha, x) \Phi_R(\alpha, y) \Phi_R(\alpha, \alpha)^{-2} = \gamma(R) \Phi_R(x, y).
$$

Par définition de $\gamma(R)$, on a $B_R(x, y) = 4 \gamma(R) \Phi_R(x, y)$, donc

$$
\Phi_{R^\vee}(x^*, y^*) = (4 \gamma(R))^{-1} B_{R^\vee}(x^*, y^*)
$$

pour $x^*, y^* \in V^*$. Ceci prouve d’abord que $\gamma(R) = \gamma(R^\vee)$. D’autre part, pour $\beta \in R$,

$$
\Phi_{R^\vee}(\beta^\vee, \beta^\vee) = (4 \gamma(R))^{-1} \sum_{\alpha \in R} \langle \beta^\vee, \alpha \rangle^2
= \gamma(R)^{-1} \sum_{\alpha \in R} \frac{\Phi_R(\alpha, \beta)^2}{\Phi_R(\beta, \beta)^2}
$$

soit, d’après (16)

$$
\Phi_{R^\vee}(\beta^\vee, \beta^\vee) = \gamma(R)^{-1} \Phi_R(\beta, \beta)^{-2} \Phi_R(\beta, \beta)
$$

ou finalement

$$
\Phi_R(\beta, \beta) \Phi_{R^\vee}(\beta^\vee, \beta^\vee) = \gamma(R)^{-1}.
$$

Si en outre toutes les racines de $R$ ont la même longueur $\lambda$ pour $\Phi_R$, (16) et (18) montrent que

$$
\gamma(R) = \lambda^{-4}.
$$

n° 2.1.

GROUPE DE WEYL AFFINE

De plus, si $h$ est le nombre de Coxeter de W, le cor. du th. 1 du chap. V, § 6, n° 2 montre que :

$$
h \Phi_R(x, x) = \sum_{\alpha \in R} \Phi_R(x, \frac{\alpha}{\lambda})^2 \quad \text{pour tout } x \in V.
$$

En comparant avec (16), on en déduit :

(21)
$$
\lambda = h^{-1/2} \quad \text{et} \quad \gamma(R) = h^2.
$$

Enfin, la formule (19) montre que les racines de $R^\vee$ ont la longueur $\lambda$ pour $\Phi_{R^\vee}$.

## EXERCICES {#lie-vi-s1-exercises}

Tous les systèmes de racines considérés ci-dessous sont relatifs à des espaces vectoriels réels. On désigne par $(x|y)$ un produit scalaire invariant par le groupe de Weyl (cf. n° 3).

See the [exercises for § 1](exercises/s1/).
