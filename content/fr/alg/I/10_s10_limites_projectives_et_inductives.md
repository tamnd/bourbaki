---
book: alg
book_title: Algebra
chapter: I
chapter_title: STRUCTURES ALGÉBRIQUES
section: 10
section_title: Limites projectives et inductives
lang: fr
source: alg-i-iii-fr
book_pages: A I.157
pdf_pages: 0122-0128, 0167-0167
extraction: ocr
subsections:
    - "no": 1
      title: Systèmes projectifs de magmas
      page: 0
      pdf_page: 122
    - "no": 2
      title: Limites projectives d’actions
      page: 113
      pdf_page: 123
    - "no": 3
      title: Systèmes inductifs de magmas
      page: 114
      pdf_page: 124
    - "no": 4
      title: Limite inductive d’actions
      page: 117
      pdf_page: 127
statements: 5
exercises: 2
content_sha256: cd4ebcd580756750a371bafeb1a9e2b804c75724354b5aa0193b9a1b9afda980
---

## § 10. LIMITES PROJECTIVES ET INDUCTIVES

Dans tout ce paragraphe, on désigne par $I$ un ensemble préordonné non vide, par $\alpha \leqslant \beta$ la relation de préordre dans $I$. La notion de système projectif (resp. inductif) d’ensembles relatif à l’ensemble d’indices $I$ est définie en E, III, p. 52 (resp. E, III, p. 61, sous l’hypothèse que $I$ est filtrant à droite).

### 1. Systèmes projectifs de magmas

#### Définition 1 {#alg-i-s10-def-1 .statement}

*On appelle système projectif de magmas relatif à l’ensemble d’indices $I$ un système projectif d’ensembles* $(\mathbf{E}_\alpha, f_{\alpha\beta})$ *relatif à $I$, chaque* $\mathbf{E}_\alpha$ *étant muni d’une structure de magma et chaque* $f_{\alpha\beta}$ *étant un homomorphisme de magmas*.

Soit $(\mathbf{E}_\alpha, f_{\alpha\beta})$ un système projectif de magmas dont les lois sont notées multiplicativement. L’ensemble limite projective $\mathbf{E} = \lim_{\leftarrow} \mathbf{E}_\alpha$ est le sous-ensemble du magma produit $\prod_{\alpha \in I} \mathbf{E}_\alpha$ formé des familles $(x_\alpha)_{\alpha \in I}$ telles que $x_\alpha = f_{\alpha\beta}(x_\beta)$ pour α ≤ β. Si $(x_\alpha)$ et $(y_\alpha)$ appartiennent à E, on a, pour $\alpha \leq \beta$, $x_\alpha = f_{\alpha \beta}(x_\beta)$ et $y_\alpha = f_{\alpha \beta}(y_\beta)$, d’où $x_\alpha y_\alpha = f_{\alpha \beta}(x_\beta)f_{\alpha \beta}(y_\beta) = f_{\alpha \beta}(x_\beta y_\beta)$; donc E est un sous-magma de $\prod_{\alpha \in I} E_\alpha$. On munira E de la loi induite par celle de $\prod_{\alpha \in I} E_\alpha$; le magma obtenu s’appelle le *magma limite projective des magmas* $E_\alpha$. Il jouit de la propriété universelle suivante:

a) Pour tout $\alpha \in I$, l’application canonique $f_\alpha$ de E dans $E_\alpha$ est un homomorphisme de magmas de E dans $E_\alpha$. On a $f_\alpha = f_{\alpha \beta} \circ f_\beta$ pour $\alpha \leq \beta$.

b) Supposons donnés un magma F et des homomorphismes $u_\alpha : F \to E_\alpha$ tels que $u_\alpha = f_{\alpha \beta} \circ u_\beta$ pour $\alpha \leq \beta$. Il existe un homomorphisme $u : F \to E$ et un seul tel que $u_\alpha = f_\alpha \circ u$ pour tout $\alpha \in I$ (à savoir $x \mapsto u(x) = (u_\alpha(x))_{\alpha \in I}$).

Si les magmas $E_\alpha$ sont associatifs (resp. commutatifs), il en est de même de E. Supposons que chaque magma $E_\alpha$ admette un élément neutre $e_\alpha$ et que les homomorphismes $f_{\alpha \beta}$ soient unifères. Alors $e = (e_\alpha)_{\alpha \in I}$ appartient à E, car $e_\alpha = f_{\alpha \beta}(e_\beta)$ pour $\alpha \leq \beta$, et c’est un élément neutre du magma E; avec les notations précédentes, les homomorphismes $f_\alpha$ sont unifères, et si les $u_\alpha$ sont unifères, alors $u$ est unifère. De plus un élément $x = (x_\alpha)_{\alpha \in I}$ de E est inversible si et seulement si chacun des $x_\alpha$ est inversible dans le magma $E_\alpha$ correspondant, et l’on a $x^{-1} = (x_\alpha^{-1})_{\alpha \in I}$: cela résulte de la formule $f_{\alpha \beta}(x_\beta^{-1}) = f_{\alpha \beta}(x_\beta)^{-1} = x_\alpha^{-1}$ pour $\alpha \leq \beta$.

On déduit de ces remarques que si les magmas $E_\alpha$ sont des monoïdes (resp. des groupes) et les $f_{\alpha \beta}$ des homomorphismes de monoïdes, alors le magma E est un monoïde (resp. un groupe). On parlera dans ce cas de système projectif de monoïdes (resp. de groupes). La propriété universelle se transpose immédiatement à ce cas.

On laisse au lecteur le soin de définir un système projectif d’anneaux $(E_\alpha, f_{\alpha \beta})$ et de vérifier que $E = \lim_{\leftarrow} E_\alpha$ est un sous-anneau de l’anneau produit $\prod_{\alpha \in I} E_\alpha$ appelé *anneau limite projective des anneaux* $E_\alpha$; on vérifie que la propriété universelle s’étend à ce cas.

Soient $\mathfrak{E} = (E_\alpha, f_{\alpha \beta})$ et $\mathfrak{E}' = (E'_\alpha, f'_{\alpha \beta})$ deux systèmes projectifs de magmas (resp. de monoïdes, de groupes, d’anneaux) relatifs au même ensemble d’indices. Un homomorphisme de $\mathfrak{E}$ dans $\mathfrak{E}'$ est un système projectif $(u_\alpha)_{\alpha \in I}$ d’applications $u_\alpha : E_\alpha \to E'_\alpha$ tel que chaque $u_\alpha$ soit un homomorphisme. Dans ces conditions, l’application $u = \lim_{\leftarrow} u_\alpha$ de $\lim_{\leftarrow} E_\alpha$ dans $\lim_{\leftarrow} E'_\alpha$ est un homomorphisme (cf. E, III, p. 54).

### 2. Limites projectives d’actions

Supposons donnés deux systèmes projectifs d’ensembles $(\Omega_\alpha, \varphi_{\alpha \beta})$ et $(E_\alpha, f_{\alpha \beta})$ relatifs au même ensemble d’indices I. Supposons donnée pour tout $\alpha \in I$ une action de $\Omega_\alpha$ sur $E_\alpha$ de sorte que l’on ait

$$
f_{\alpha \beta}(\omega_\beta x_\beta) = \varphi_{\alpha \beta}(\omega_\beta) \cdot f_{\alpha \beta}(x_\beta)
$$

pour $\alpha \leq \beta$, $x_\beta \in E_\beta$, $\omega_\beta \in \Omega_\beta$. On dit alors que la famille d’actions considérée est un système projectif d’actions. Posons $\Omega = \lim_{\leftarrow} \Omega_\alpha$ et $E = \lim_{\leftarrow} E_\alpha$; si $x = (x_\alpha)_{\alpha \in I}$ appartient à $E$ et $\omega = (\omega_\alpha)_{\alpha \in I}$ appartient à $\Omega$, alors $\omega \cdot x = (\omega_\alpha \cdot x_\alpha)_{\alpha \in I}$ appartient à $E$ d’après (1). On définit ainsi une action de $\Omega$ sur $E$, appelée limite projective des actions des $\Omega_\alpha$ sur les $E_\alpha$.

Ce qui précède s’applique surtout au cas où les $\Omega_\alpha$ sont des monoïdes, et où chaque action de $\Omega_\alpha$ sur $E_\alpha$ est une opération. Alors, la limite projective de ces opérations est une opération du monoïde $\Omega$ sur $E$.

On laisse au lecteur le soin de définir la limite projective d’un système projectif de groupes à opérateurs, et de vérifier que cette limite est un groupe à opérateurs.

### 3. Systèmes inductifs de magmas

Dans ce n° et le suivant, on suppose I filtrant à droite.

#### Définition 2 {#alg-i-s10-def-2 .statement}

On appelle système inductif de magmas relatif à l’ensemble d’indices I un système inductif d’ensembles $(E_\alpha, f_{\beta \alpha})$ relatif à I, chaque $E_\alpha$ étant muni d’une structure de magma et chaque $f_{\beta \alpha}$ étant un homomorphisme de magmas.

Soit $(E_\alpha, f_{\beta \alpha})$ un système inductif de magmas. On notera E l’ensemble limite inductive $\lim_{\longrightarrow} E_\alpha$ et $f_\alpha$ l’application canonique de $E_\alpha$ dans E. On rappelle que l’on a

$$
f_\beta \circ f_{\beta \alpha} = f_\alpha \quad \text{pour } \alpha \leq \beta,
$$
$$
E = \bigcup_{\alpha \in \Lambda} f_\alpha(E_\alpha).
$$

D’après (2), on a aussi

$$
f_\alpha(E_\alpha) \subset f_\beta(E_\beta) \quad \text{pour } \alpha \leq \beta.
$$

Si $x_\alpha, y_\alpha$ dans $E_\alpha$ sont tels que $f_\alpha(x_\alpha) = f_\alpha(y_\alpha)$, il existe un $\beta \geq \alpha$ tel que $f_{\beta \alpha}(x_\alpha) = f_{\beta \alpha}(y_\alpha)$.

#### Proposition 1 {#alg-i-s10-prop-1 .statement}

Il existe sur E une structure de magma et une seule pour laquelle les applications $f_\alpha : E_\alpha \to E$ sont des homomorphismes. Si les magmas $E_\alpha$ sont associatifs (resp. commutatifs), il en est de même de E. Si les magmas $E_\alpha$ et les homomorphismes $f_{\beta \alpha}$ sont unifères, il en est de même du magma E et des homomorphismes $f_\alpha$.

On notera multiplicativement les magmas $E_\alpha$.

Soient $x, y$ dans E. Il existe $\alpha$ dans I et $x_\alpha, y_\alpha$ dans $E_\alpha$ tels que $x = f_\alpha(x_\alpha)$ et y = f_\alpha(y_\alpha). S’il existe une structure de magma sur E pour laquelle $f_\alpha$ soit un homomorphisme, on aura $x.y = f_\alpha(x_\alpha y_\alpha)$, d’où l’unicité de cette structure de magma.

Pour démontrer son existence, nous devons prouver que pour $\alpha, \beta$ dans I, $x_\alpha, y_\alpha$ dans $E_\alpha$ et $x'_\beta, y'_\beta$ dans $E_\beta$, les relations
$$
f_\alpha(x_\alpha) = f_\beta(x'_\beta), \quad f_\alpha(y_\alpha) = f_\beta(y'_\beta)
$$
entraînent $f_\alpha(x_\alpha y_\alpha) = f_\beta(x'_\beta y'_\beta)$. Pour $\gamma \geq \alpha$ et $\gamma \geq \beta$, posons $x_\gamma = f_{\gamma \alpha}(x_\alpha)$, $y_\gamma = f_{\gamma \alpha}(y_\alpha)$, $x'_\gamma = f_{\gamma \beta}(x'_\beta)$, $y'_\gamma = f_{\gamma \beta}(y'_\beta)$. D’après la définition de la limite inductive, il existe $\gamma$ dans I tels que $\gamma \geq \alpha, \gamma \geq \beta$, $x_\gamma = x'_\gamma, y_\gamma = y'_\gamma$. Alors
$$
f_\alpha(x_\alpha y_\alpha) = f_\gamma(f_{\gamma \alpha}(x_\alpha y_\alpha)) = f_\gamma(x_\gamma y_\gamma) = f_\gamma(x'_\gamma y'_\gamma) = f_\gamma(f_{\gamma \beta}(x'_\beta y'_\beta)) = f_\beta(x'_\beta y'_\beta).
$$

Supposons les magmas $E_\alpha$ associatifs. Soient $x, y, z$ dans E. Il existe $\alpha \in I$ et des éléments $x_\alpha, y_\alpha, z_\alpha$ de $E_\alpha$ tels que
$$
x = f_\alpha(x_\alpha), \quad y = f_\alpha(y_\alpha), \quad z = f_\alpha(z_\alpha).
$$
On a alors $xy = f_\alpha(x_\alpha y_\alpha)$, d’où $(xy)z = f_\alpha((x_\alpha y_\alpha)z_\alpha)$; de même, on a $x(yz) = f_\alpha(x_\alpha(y_\alpha z_\alpha))$, d’où $(xy)z = x(yz)$ car $(x_\alpha y_\alpha)z_\alpha = x_\alpha(y_\alpha z_\alpha)$. Le cas des magmas commutatifs se traite de manière analogue.

Supposons enfin que chaque magma $E_\alpha$ ait un élément neutre $e_\alpha$ et qu’on ait $f_{\beta \alpha}(e_\alpha) = e_\beta$ pour $\alpha \leq \beta$. Pour $\alpha, \beta$ dans I, il existe $\gamma$ dans I tel que $\gamma \geq \alpha$ et $\gamma \geq \beta$, d’où
$$
f_\alpha(e_\alpha) = f_\gamma(f_{\gamma \alpha}(e_\alpha)) = f_\gamma(e_\gamma) = f_\gamma(f_{\gamma \beta}(e_\beta)) = f_\beta(e_\beta)
$$
et il existe donc un élément $e$ de E tel que $f_\alpha(e_\alpha) = e$ pour tout $\alpha \in I$. Soit $x \in E$; soient $\alpha \in I$ et $x_\alpha \in E_\alpha$ tels que $x = f_\alpha(x_\alpha)$. On a alors
$$
ex = f_\alpha(e_\alpha) \cdot f_\alpha(x_\alpha) = f_\alpha(e_\alpha \cdot x_\alpha) = f_\alpha(x_\alpha) = x
$$
et de même $xe = x$, donc $e$ est élément neutre de E.

C. Q. F. D.

On dit que le magma E est la limite inductive des magmas $E_\alpha$.

#### Proposition 2 {#alg-i-s10-prop-2 .statement}

*Soit* $(E_\alpha, f_{\beta \alpha})$ *un système inductif de magmas et soient* E *sa limite inductive*, $f_\alpha : E_\alpha \to E$ *les homomorphismes canoniques*. *On suppose donnés un magma* F *et une famille d’homomorphismes* $u_\alpha : E_\alpha \to F$ *tels que* $u_\alpha = u_\beta \circ f_{\beta \alpha}$ *pour* $\alpha \leq \beta$. *Il existe un homomorphisme* $u : E \to F$ *et un seul tel que* $u_\alpha = u \circ f_\alpha$ *pour tout* $\alpha \in I$. *Si les magmas* $E_\alpha$ *et* F *et les homomorphismes* $f_{\beta \alpha}$ *et* $u_\alpha$ *sont unifères, l’homomorphisme* u *est unifère*.

On sait (E, III, p. 62, prop. 6) qu’il existe une application $u : E \to F$ et une seule telle que $u_\alpha = u \circ f_\alpha$ pour tout $\alpha \in I$. Vérifions que $u$ est un homomorphisme; soient $x, y$ dans E, $\alpha$ dans I et $x_\alpha, y_\alpha$ dans $E_\alpha$ tels que $x = f_\alpha(x_\alpha)$ et $y = f_\alpha(y_\alpha)$. On a $xy = f_\alpha(x_\alpha y_\alpha)$, d’où
$$
u(xy) = u(f_\alpha(x_\alpha y_\alpha)) = u_\alpha(x_\alpha y_\alpha) = u_\alpha(x_\alpha)u_\alpha(y_\alpha)
$$
$$
= u(f_\alpha(x_\alpha))u(f_\alpha(y_\alpha)) = u(x)u(y).
$$

Plaçons-nous maintenant dans le cas unifère et notons $e_\alpha$ l’élément unité de $E_\alpha$, $e$ celui de $E$ et $e'$ celui de $F$. Soit $\alpha \in I$; on a $e = f_\alpha(e_\alpha)$, d’où
$$
u(e) = u(f_\alpha(e_\alpha)) = u_\alpha(e_\alpha) = e'
$$
car $u_\alpha$ est unifère. Donc $u$ est unifère.

C. Q. F. D.

Par analogie avec la notion de système inductif de magmas, on peut formuler celle de système inductif de monoïdes ou de groupes. La prop. 1 (I, p. 114) montre que le magma $E$ limite d’un système inductif de monoïdes $(E_\alpha, f_{\beta\alpha})$ est un monoïde. Montrons que $E$ est un groupe si les $E_\alpha$ sont des groupes; soient $x \in E$, $\alpha \in I$ et $x_\alpha \in E_\alpha$ tels que $x = f_\alpha(x_\alpha)$; l’élément $y = f_\alpha(x_\alpha^{-1})$ de $E$ est inverse de $x$ (I, p. 15). La propriété universelle de la prop. 2 (I, p. 115) se traduit immédiatement dans le cas d’un système inductif de monoïdes ou de groupes.

Nous laissons au lecteur le soin de définir un système inductif d’anneaux. Soit $(A_\alpha, f_{\beta\alpha})$ un tel système inductif; soient $A = \lim_{\longrightarrow} A_\alpha$ et $f_\alpha : A_\alpha \to A$ les homomorphismes canoniques. Il existe (I, p. 115, prop. 2) sur $A$ une addition et une multiplication caractérisées par $x + y = f_\alpha(x_\alpha + y_\alpha)$, $xy = f_\alpha(x_\alpha y_\alpha)$ pour $\alpha$ dans $I$, $x_\alpha, y_\alpha$ dans $A_\alpha$ et $x = f_\alpha(x_\alpha), y = f_\alpha(y_\alpha)$. Pour l’addition, $A$ est un groupe commutatif, et la multiplication est associative et admet un élément unité. Enfin, pour $x, y, z$ dans $A$, soient $\alpha$ dans $I$ et $x_\alpha, y_\alpha, z_\alpha$ dans $A_\alpha$ tels que
$$
x = f_\alpha(x_\alpha), \quad y = f_\alpha(y_\alpha), \quad \text{et} \quad z = f_\alpha(z_\alpha).
$$
On a
$$
(x + y)z = f_\alpha(x_\alpha + y_\alpha)f_\alpha(z_\alpha) = f_\alpha((x_\alpha + y_\alpha)z_\alpha)
= f_\alpha(x_\alpha z_\alpha + y_\alpha z_\alpha) = f_\alpha(x_\alpha z_\alpha) + f_\alpha(y_\alpha z_\alpha) = xz + yz
$$
et de manière analogue, on prouve la relation $x(y + z) = xy + xz$. Autrement dit, $A$ est muni d’une structure d’anneau, caractérisée par le fait que $f_\alpha$ est un homomorphisme d’anneaux pour tout $\alpha \in I$.

On dit que l’anneau $A$ est limite inductive des anneaux $A_\alpha$. La prop. 2 (I, p. 115) s’étend immédiatement au cas des anneaux.

#### Proposition 3 {#alg-i-s10-prop-3 .statement}

a) Si les $A_\alpha$ sont non nuls, $A$ est non nul.
b) Si les $A_\alpha$ sont intègres, $A$ est intègre.
c) Si les $A_\alpha$ sont des corps, $A$ est un corps.

Soient $0_\alpha, 1_\alpha$ le zéro et l’unité de $A_\alpha$, et $0, 1$ le zéro et l’unité de $A$. Il existe $\alpha \in I$ tel que $f_\alpha(0_\alpha) = 0, f_\alpha(1_\alpha) = 1$. Si $0 = 1$, il existe $\beta \geq \alpha$ tel que $f_{\beta\alpha}(0_\alpha) = f_{\beta\alpha}(1_\alpha)$, c’est-à-dire $0_\beta = 1_\beta$. Ceci prouve a).

Supposons les $A_\alpha$ intègres. Alors $A$ est commutatif, et non nul d’après a). Soient $x, y$ des éléments de $A$ tels que $xy = 0$. Il existe $\alpha \in I$ et $x_\alpha, y_\alpha$ dans $A_\alpha$ tels que $x = f_\alpha(x_\alpha), y = f_\alpha(y_\alpha)$. Alors $f_\alpha(x_\alpha y_\alpha) = xy = 0 = f_\alpha(0_\alpha)$. Donc il existe $\beta \geq \alpha$ tel que $f_{\beta\alpha}(x_\alpha y_\alpha) = f_{\beta\alpha}(0_\alpha)$. Comme $A_\beta$ est intègre, on en conclut que $f_{\beta\alpha}(x_\alpha) = 0_\beta$ ou $f_{\beta\alpha}(y_\alpha) = 0_\beta$, donc $x = 0$ ou $y = 0$. Ceci prouve b).

Supposons que les $A_\alpha$ soient des corps. Alors $A \neq \{0\}$ d’après a). Soit $x$ un élément non nul de $A$. Il existe $\alpha \in I$ et $x_\alpha \in A_\alpha$ tel que $x = f_\alpha(x_\alpha)$. Alors $x_\alpha \neq 0$ et $f_\alpha(x_\alpha^{-1})$ est inverse de $x$ dans $A$. Ceci prouve c).

Soient $\mathfrak{E} = (E_\alpha, f_{\beta \alpha})$ et $\mathfrak{E}' = (E'_\alpha, f'_{\beta \alpha})$ deux systèmes inductifs de magmas (resp. monoïdes, groupes, anneaux). Un homomorphisme de $\mathfrak{E}$ dans $\mathfrak{E}'$ est un système inductif $(u_\alpha)_{\alpha \in I}$ d’applications $u_\alpha : E_\alpha \to E'_\alpha$ tel que chaque $u_\alpha$ soit un homomorphisme. Dans ces conditions, l’application $u = \lim u_\alpha$ de $E = \lim E_\alpha$ dans $E' = \lim E'_\alpha$ est un homomorphisme (cf. E, III, p. 63).

### 4. Limite inductive d’actions

Supposons donnés deux systèmes inductifs d’ensembles $(\Omega_\alpha, \varphi_{\beta \alpha})$ et $(E_\alpha, f_{\beta \alpha})$ relatifs au même ensemble d’indices $I$, et, pour chaque $\alpha \in I$, une action de $\Omega_\alpha$ sur $E_\alpha$. On suppose que l’on a

$$
f_{\beta \alpha}(\omega_\alpha \cdot x_\alpha) = \varphi_{\beta \alpha}(\omega_\alpha) \cdot f_{\beta \alpha}(x_\alpha)
$$

pour $\alpha \leq \beta$, $\omega_\alpha \in \Omega_\alpha$ et $x_\alpha \in E_\alpha$. On dit alors que la famille d’actions considérée est un *système inductif d’actions*. On vérifie facilement comme dans la prop. 2 (I, p. 115) qu’il existe une action $h$ de $\Omega = \lim \Omega_\alpha$ sur $E = \lim E_\alpha$ qui se décrit ainsi : soient $\omega \in \Omega$ et $x \in E$; soient $\alpha \in I$ et $\omega_\alpha \in \Omega_\alpha$, $x_\alpha \in E_\alpha$ tels que $\omega = \varphi_\alpha(\omega_\alpha)$ et $x = f_\alpha(x_\alpha)$ (on note $\varphi_\alpha : \Omega_\alpha \to \Omega$ et $f_\alpha : E_\alpha \to E$ les applications canoniques); on a alors $\omega \cdot x = f_\alpha(\omega_\alpha \cdot x_\alpha)$. On dit que l’action de $\Omega$ sur $E$ est la *limite inductive des actions* des $\Omega_\alpha$ sur les $E_\alpha$.

Si les $\Omega_\alpha$ sont des monoïdes et si chaque action de $\Omega_\alpha$ sur $E_\alpha$ est une opération, l’action limite inductive est une opération.

On laisse au lecteur le soin de définir la limite inductive d’un système inductif de groupes à opérateurs, et de vérifier que cette limite est un groupe à opérateurs.

Exercises

## EXERCICES {#alg-i-s10-exercises}

See the [exercises for § 10](exercises/s10/).
