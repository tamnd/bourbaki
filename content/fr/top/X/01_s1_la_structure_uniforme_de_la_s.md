---
book: top
book_title: General Topology
chapter: X
chapter_title: ESPACES FONCTIONNELS
section: 1
section_title: La structure uniforme de la S-convergence
lang: fr
source: top-v-x-fr
pdf_pages: 0250-0259, 0290-0292
extraction: ocr
subsections:
    - "no": 1
      title: La structure de la convergence uniforme
      page: 0
      pdf_page: 250
    - "no": 2
      title: La $\mathfrak{S}$-convergence
      page: 2
      pdf_page: 251
    - "no": 3
      title: Exemples de $\mathfrak{S}$-convergence
      page: 4
      pdf_page: 253
    - "no": 4
      title: Propriétés des espaces $\mathcal{F}_\mathfrak{S}(X; Y)$
      page: 5
      pdf_page: 254
    - "no": 5
      title: Parties complètes de $\mathcal{F}_{\mathcal{S}}(X; Y)$
      page: 6
      pdf_page: 255
    - "no": 6
      title: La $\mathfrak{S}$-convergence dans les espaces d’applications continues
      page: 7
      pdf_page: 256
statements: 36
exercises: 12
content_sha256: 401857c8b74031e4527e1497431b3e91bb1924d8c4e983fb5eee3c05fd3867c8
---

## § 1. LA STRUCTURE UNIFORME DE LA $\mathfrak{S}$-CONVERGENCE

Notations. — Étant donnés deux ensembles $X, Y$, rappelons que l’on désigne par $\mathcal{F}(X; Y)$ l’ensemble de toutes les applications de $X$ dans $Y$, qui s’identifie à l’ensemble produit $Y^X$ (E, II, p. 31). Pour toute partie $H$ de $\mathcal{F}(X; Y)$, et tout $x \in X$, nous désignerons par $H(x)$ l’ensemble des $u(x) \in Y$ lorsque $u$ parcourt $H$. Si $\Phi$ est une base de filtre sur $\mathcal{F}(X; Y)$, nous désignerons par $\Phi(x)$ la base de filtre sur $Y$ formée des $H(x)$, où $H$ parcourt $\Phi$. Enfin, rappelons que, pour tout $u \in \mathcal{F}(X; Y)$ et toute partie $A$ de $X$, $u | A$ désigne la restriction de $u$ à $A$, application de $A$ dans $Y$; si $H$ est une partie de $\mathcal{F}(X; Y)$, $H | A$ désignera l’ensemble des restrictions $u | A$ pour $u \in H$.

### 1. La structure de la convergence uniforme

Soient $X$ un ensemble, $Y$ un espace uniforme. Pour tout entourage $V$ de $Y$, désignons par $W(V)$ l’ensemble des couples $(u, v)$ d’applications de $X$ dans $Y$ tels que l’on ait $(u(x), v(x)) \in V$ pour tout $x \in X$. Lorsque $V$ parcourt l’ensemble des entourages de $Y$, les ensembles $W(V)$ forment un système fondamental d’entourages d’une structure uniforme sur $\mathcal{F}(X; Y)$. En effet, ils satisfont de façon évidente à l’axiome $(\mathrm{U}_1')$ (II, p. 2); si $V, V'$ sont deux entourages de $Y$ tels que $V \subset V'$, on a $W(V) \subset W(V')$, donc les ensembles $W(V)$ vérifient $(\mathrm{B}_1)$ (I, p. 38); on a $\widehat{W(V)} = W(V)^{-1}$, donc $(\mathrm{U}_{\mathrm{II}}')$ est vérifié; enfin, les relations « quel que soit $x \in X,\ (u(x), v(x)) \in V$ et « quel que soit $x \in X,\ (v(x), w(x)) \in V$ » entraînent la relation « quel que soit $x \in X,\ (u(x), w(x)) \in \overset{2}{V}$ », autrement dit on a

$$
\widehat{W(V)}^2 \subset W(V)^2,
$$

ce qui démontre ($U'_{III}$).

#### Définition 1 {#top-x-s1-def-1 .statement}

On dit que la structure uniforme sur l’ensemble $\mathcal{F}(X; Y)$ ayant pour système fondamental d’entourages l’ensemble des $W(V)$, où $V$ parcourt l’ensemble des entourages de $Y$, est la structure de la convergence uniforme ; la topologie déduite de cette structure uniforme est appelée topologie de la convergence uniforme. Si un filtre $\Phi$ sur $\mathcal{F}(X; Y)$ converge vers un élément $u_0$ pour cette topologie, on dit qu’il converge uniformément vers $u_0$.

On notera que la topologie de la convergence uniforme sur $\mathcal{F}(X; Y)$ dépend de la structure uniforme de $Y$ et non seulement de la topologie de $Y$ (X, p. 41, exerc. 4).

L’espace uniforme obtenu en munissant $\mathcal{F}(X; Y)$ de la structure de la convergence uniforme se note $\mathcal{F}_u(X; Y)$.

### 2. La $\mathfrak{S}$-convergence

#### Définition 2 {#top-x-s1-def-2 .statement}

Soient $X$ un ensemble, $Y$ un espace uniforme, $\mathfrak{S}$ un ensemble de parties de $X$. On appelle structure uniforme de la convergence uniforme dans les ensembles de $\mathfrak{S}$, ou simplement structure uniforme de la $\mathfrak{S}$-convergence, la structure uniforme la moins fine sur $\mathcal{F}(X; Y)$ rendant uniformément continues les applications de restriction $u \mapsto u|A$ de $\mathcal{F}(X; Y)$ dans les espaces uniformes $\mathcal{F}_u(A; Y)$, où $A$ parcourt $\mathfrak{S}$. On note $\mathcal{F}_{\mathfrak{S}}(X; Y)$ l’espace uniforme obtenu en munissant $\mathcal{F}(X; Y)$ de la structure uniforme de la $\mathfrak{S}$-convergence.

La topologie déduite de la structure uniforme de la $\mathfrak{S}$-convergence s’appelle la topologie de la $\mathfrak{S}$-convergence ; c’est la moins fine rendant continues les applications $u \mapsto u|A$ de $\mathcal{F}(X; Y)$ (pour $A \in \mathfrak{S}$) dans les espaces $\mathcal{F}_u(A; Y)$ (II, p. 8, corollaire).

Pour qu’un filtre $\Phi$ sur $\mathcal{F}(X; Y)$ converge vers $u_0$ pour la topologie de la $\mathfrak{S}$-convergence, il faut et il suffit que pour tout $A \in \mathfrak{S}$, $u|A$ converge uniformément vers $u_0|A$ suivant le filtre $\Phi$ (I, p. 51, prop. 10) ; aussi dit-on que $\Phi$ converge uniformément vers $u_0$ dans les ensembles de $\mathfrak{S}$.

De même, pour qu’une base de filtre $\Phi$ sur $\mathcal{F}_{\mathfrak{S}}(X; Y)$ soit une base de filtre de Cauchy, il faut et il suffit que, pour tout $A \in \mathfrak{S}$, l’image de $\Phi$ par l’application $u \mapsto u|A$ soit une base de filtre de Cauchy dans $\mathcal{F}_u(A; Y)$ (II, p. 13, prop. 4).

Soit $f$ une application d’un espace topologique (resp. d’un espace uniforme) $Z$ dans $\mathcal{F}_{\mathfrak{S}}(X; Y)$. Pour que $f$ soit continue (resp. uniformément continue), il faut et il suffit que, pour tout $A \in \mathfrak{S}$, l’application $z \mapsto f(z)|A$ de $Z$ dans $\mathcal{F}_u(A; Y)$ soit continue (resp. uniformément continue) (I, p. 12, prop. 4 et II, p. 8, prop. 4).

Enfin, soit $M$ une partie de $\mathcal{F}_\mathfrak{S}(X; Y)$; pour que $M$ soit précompacte il faut et il suffit que, pour tout $A \in \mathfrak{S}$, l’ensemble des restrictions $u \mid A$ pour $u \in M$ soit une partie précompacte de $\mathcal{F}_u(A; Y)$ (II, p. 31, prop. 3).

#### Remarque 1 {#top-x-s1-n2-rem-1 .statement}

La définition générale des entourages d’une structure uniforme initiale (II, p. 8, prop. 4) montre qu’on obtient un système fondamental d’entourages de $\mathcal{F}_\mathfrak{S}(X; Y)$ de la façon suivante: pour tout $A \in \mathfrak{S}$ et tout entourage $V$ d’un système fondamental $\mathfrak{B}$ d’entourages de $Y$, soit $W(A, V)$ l’ensemble des couples $(u, v)$ d’applications de $X$ dans $Y$ tels que $(u(x), v(x)) \in V$ pour tout $x \in A$; lorsque $A$ parcourt $\mathfrak{S}$ et que $V$ parcourt $\mathfrak{B}$, les intersections finies des $W(A, V)$ forment un système fondamental d’entourages de $\mathcal{F}_\mathfrak{S}(X, Y)$.

Cette description montre aussitôt que, si $\mathfrak{S}, \mathfrak{S}'$ sont deux ensembles de parties de $X$ telles que $\mathfrak{S} \subset \mathfrak{S}'$, la structure uniforme de la $\mathfrak{S}'$-convergence est plus fine que celle de la $\mathfrak{S}$-convergence.

#### Remarque 2 {#top-x-s1-n2-rem-2 .statement}

Toutefois, on ne change pas la structure uniforme de la $\mathfrak{S}$-convergence en remplaçant $\mathfrak{S}$ par l’ensemble $\mathfrak{S}'$ des parties de $X$ dont chacune est contenue dans la réunion d’un nombre fini d’ensembles appartenant à $\mathfrak{S}$. Dans l’étude de la $\mathfrak{S}$-convergence, on peut donc toujours se limiter au cas où l’ensemble $\mathfrak{S}$ satisfait aux deux conditions suivantes:

$(F'_I)$ Toute partie d’un ensemble de $\mathfrak{S}$ appartient à $\mathfrak{S}$.
$(F'_II)$ Toute réunion finie d’ensembles de $\mathfrak{S}$ appartient à $\mathfrak{S}$.

Lorsque $(F'_II)$ est vérifiée, on obtient un système fondamental d’entourages de $\mathcal{F}_\mathfrak{S}(X; Y)$ en prenant tous les ensembles $W(A, V)$, $A$ parcourant $\mathfrak{S}$ et $V$ un système fondamental d’entourages de $Y$.

#### Remarque 3 {#top-x-s1-n2-rem-3 .statement}

La structure uniforme de la $\mathfrak{S}$-convergence est l’image réciproque, par l’application $u \mapsto (u \mid A)_{A \in \mathfrak{S}}$ de $\mathcal{F}(X; Y)$ dans $\prod_{A \in \mathfrak{S}} \mathcal{F}_u(A; Y)$, de la structure uniforme de cet espace produit (II, p. 11, prop. 8). Lorsque $\mathfrak{S}$ est un recouvrement de $X$, cette application est injective, et $\mathcal{F}_\mathfrak{S}(X; Y)$ est donc isomorphe au sous-espace uniforme de $\prod_{A \in \mathfrak{S}} \mathcal{F}_u(A; Y)$, image de cette application.

#### Proposition 1 {#top-x-s1-prop-1 .statement}

Si $Y$ est séparé et si $\mathfrak{S}$ est un recouvrement de $X$, l’espace $\mathcal{F}_\mathfrak{S}(X; Y)$ est séparé.

En effet, soient $u, v$ deux éléments de $\mathcal{F}(X; Y)$ tels que $(u, v) \in W(A, V)$ pour tout entourage $V$ de $F$ et tout $A \in \mathfrak{S}$; comme $Y$ est séparé, on en déduit d’abord que $u$ et $v$ coïncident dans chaque ensemble $A \in \mathfrak{S}$, et comme $\mathfrak{S}$ est un recouvrement de $X$, $u = v$.

#### Remarque 4 {#top-x-s1-n2-rem-4 .statement}

Soit $H$ une partie de $\mathcal{F}(X; Y)$; par abus de langage, on appelle structure uniforme (resp. topologie) de la $\mathfrak{S}$-convergence sur l’ensemble $H$, la structure uniforme (resp. la topologie) induite sur $H$ par la structure uniforme (resp. la topologie) de la $\mathfrak{S}$-convergence sur $\mathcal{F}(X; Y)$.

#### Remarque 5 {#top-x-s1-n2-rem-5 .statement}

Si $\lambda \mapsto u_\lambda$ est une application, dans $\mathcal{F}_\mathfrak{S}(X; Y)$, d’un ensemble $L$ filtré par un filtre $\mathfrak{S}$, et si cette application admet une limite suivant $\mathfrak{S}$, on dit encore que, suivant le filtre $\mathfrak{S}$, les applications $u_\lambda$ de $X$ dans $Y$ convergent uniformément vers $v$ (ou que la famille $(u_\lambda)$ est uniformément convergente vers $v$) dans tout ensemble de $\mathfrak{S}$; on omet la mention du filtre $\mathfrak{S}$ lorsque $L = \mathbf{N}$ et que $\mathfrak{S}$ est le filtre de Fréchet.

Plus particulièrement, supposons définie dans $Y$ une loi de composition commutative et associative, notée additivement. Pour toute suite $(u_n)$ d’applications de $X$ dans $Y$, désignons par $v_n$ l’application $x \mapsto \sum_{k=0}^n u_k(x)$ ($n \in \mathbf{N}$); on dira que la série de terme général $u_n$ est uniformément convergente dans tout ensemble de $\mathfrak{S}$ si la suite $(v_n)$ est uniformément convergente dans tout ensemble de $\mathfrak{S}$. On définit de même une famille uniformément sommable $(u_\lambda)_{\lambda \in L}$ d’applications de $X$ dans $Y$, en considérant les applications $x \mapsto \sum_{\lambda \in J} u_\lambda(x)$ pour toutes les parties finies $J$ de $L$, et la limite de ces applications dans $\mathcal{F}_\mathfrak{S}(X; Y)$ suivant l’ensemble ordonné filtrant des parties finies de $L$ (III, p. 37).

#### Remarque 6 {#top-x-s1-n2-rem-6 .statement}

Les déf. 1 et 2 (X, p. 2) entraînent aussitôt que pour tout $x \in \bigcup_{A \in \mathfrak{S}} A$, l’application $u \mapsto u(x)$ de $\mathcal{F}_\mathfrak{S}(X; Y)$ dans $Y$ est uniformément continue. Il en résulte en particulier que, si on désigne par $\overline{H}$ l’adhérence dans $\mathcal{F}_\mathfrak{S}(X; Y)$ d’une partie $H$ de cet espace, on a, pour tout $x \in \bigcup_{A \in \mathfrak{S}} A$, $\overline{H}(x) \subset \overline{H(x)}$ (I, p. 9, th. 1).

### 3. Exemples de $\mathfrak{S}$-convergence

I. Convergence uniforme dans une partie de $X$. — Soient $A$ une partie de $X$, $\mathfrak{S} = \{A\}$. La structure uniforme (resp. la topologie) de la $\mathfrak{S}$-convergence s’appelle aussi alors la structure uniforme (resp. la topologie) de la convergence uniforme dans $A$; si un filtre $\Phi$ sur $\mathcal{F}_\mathfrak{S}(X; Y)$ converge vers $u_0$, on dit qu’il converge vers $u_0$ uniformément dans $A$. Lorsque $A = X$, on retrouve la structure de la convergence uniforme définie dans $X$, p. 2.

II. Convergence simple dans une partie de $X$. — Soit $A$ une partie de $X$, et prenons pour $\mathfrak{S}$ l’ensemble des parties de $X$ qui se réduisent à un seul point de $A$ (ou, ce qui revient au même en vertu de $X$, p. 3, Remarque 2, l’ensemble des parties finies de $A$). On dit alors que la structure uniforme (resp. la topologie) de la $\mathfrak{S}$-convergence est la structure uniforme (resp. la topologie) de la convergence simple dans $A$; si un filtre $\Phi$ sur $\mathcal{F}_\mathfrak{S}(X; Y)$ converge vers $u_0$, on dit qu’il converge simplement vers $u_0$ dans $A$; il revient au même de dire que, pour tout $x \in A$, $u_0(x)$ est limite de $u(x)$ suivant le filtre $\Phi$.

En particulier, lorsque $A = X$, la structure uniforme (resp. la topologie) de la convergence simple dans $X$ est aussi appelée structure uniforme (resp. topologie) de la convergence simple et l’espace uniforme obtenu en munissant $\mathcal{F}(X; Y)$ de cette structure se note $\mathcal{F}_s(X; Y)$. On notera que la topologie de la convergence simple n’est autre que la topologie produit sur $Y^X$; elle ne dépend donc que de la topologie de $Y$ et non de sa structure uniforme, contrairement à ce qui a lieu en général.

III. Convergence compacte. — Supposons que $X$ soit un espace topologique, et prenons pour $\mathfrak{S}$ l’ensemble des parties compactes de $X$. La structure uniforme (resp. la topologie) de la $\mathfrak{S}$-convergence est alors appelée structure uniforme (resp. topologie) de la convergence compacte; l’espace uniforme obtenu en munissant $\mathcal{F}(X; Y)$ de cette structure se note $\mathcal{F}_c(X; Y)$. La structure de la convergence compacte est moins fine que celle de la convergence uniforme, et lui est identique si $X$ est compact; elle est plus fine que la structure de la convergence simple, et lui est identique si $X$ est discret.

Lorsque $X$ est un espace uniforme, on définit de même sur $\mathcal{F}(X; Y)$ la structure uniforme de la convergence précompacte en prenant pour $\mathfrak{S}$ l’ensemble des parties précompactes de $X$. De même, si $X$ est un espace métrique, on peut prendre pour $\mathfrak{S}$ l’ensemble des parties bornées de $X$; la structure de la $\mathfrak{S}$-convergence prend alors le nom de structure uniforme de la convergence bornée.

### 4. Propriétés des espaces $\mathcal{F}_\mathfrak{S}(X; Y)$

#### Proposition 2 {#top-x-s1-prop-2 .statement}

Soient $X_1, X_2$ deux ensembles, $Y$ un espace uniforme, $\mathfrak{S}_i$ un ensemble de parties de $X_i$ ($i = 1, 2$), $\mathfrak{S}_1 \times \mathfrak{S}_2$ l’ensemble des parties de la forme $A_1 \times A_2$ de $X_1 \times X_2$, avec $A_i \in \mathfrak{S}_i, i = 1, 2$. Alors la bijection canonique.

$$
\mathcal{F}(X_1 \times X_2; Y) \to \mathcal{F}(X_1; \mathcal{F}(X_2, Y))
$$

(E, II, p. 31) est un isomorphisme de l’espace uniforme $\mathcal{F}_{\mathfrak{S}_1 \times \mathfrak{S}_2}(X_1 \times X_2; Y)$ sur l’espace uniforme $\mathcal{F}_{\mathfrak{S}_1}(X_1; \mathcal{F}_{\mathfrak{S}_2}(X_2; Y))$.

En effet, soient $V$ un entourage de $Y$, $A_i$ un élément de $\mathfrak{S}_i$ ($i = 1, 2$); il résulte aussitôt des définitions que $W(A_1 \times A_2, V)$ s’identifie à $W(A_1, W(A_2, V))$ par la bijection canonique, d’où la proposition.

#### Proposition 3 {#top-x-s1-prop-3 .statement}

a) Soient $X$ un ensemble, $\mathfrak{S}$ un ensemble de parties de $X$, $Y, Y'$ deux espaces uniformes, $f : Y \to Y'$ une application uniformément continue. Alors l’application $u \mapsto f \circ u$ de $\mathcal{F}_\mathfrak{S}(X; Y)$ dans $\mathcal{F}_\mathfrak{S}(X; Y')$ est uniformément continue.

b) Soient $X, X'$ deux ensembles, $\mathfrak{S}$ (resp. $\mathfrak{S}'$) un ensemble de parties de $X$ (resp. $X'$), $Y$ un espace uniforme, $g : X' \to X$ une application telle que, pour tout $A' \in \mathfrak{S}'$, $g(A')$ soit contenu dans une réunion finie d’ensembles de $\mathfrak{S}$. Alors l’application $u \mapsto u \circ g$ de $\mathcal{F}_\mathfrak{S}(X; Y)$ dans $\mathcal{F}_{\mathfrak{S}'}(X'; Y)$ est uniformément continue.

#### Proposition 4 {#top-x-s1-prop-4 .statement}

Soient $X, Y$ deux ensembles, $(X_\lambda)_{\lambda \in L}$ une famille d’ensembles, $(Y_\mu)_{\mu \in M}$ une famille d’espaces uniformes. Pour tout $\lambda \in L$, soit $\mathfrak{S}_\lambda$ un ensemble de parties de $X_\lambda$, soit $g_\lambda$ une application de $X_\lambda$ dans $X$, et soit $\mathfrak{S}$ l’ensemble de parties de $X$, réunion des $g_\lambda(\mathfrak{S}_\lambda)$. Pour tout $\mu \in M$, soit $f_\mu$ une application de $Y$ dans $Y_\mu$; on munit $Y$ de la structure uniforme la moins fine rendant uniformément continues les $f_\mu$. Alors la structure uniforme de la $\mathfrak{S}$-convergence sur $\mathcal{F}(X; Y)$ est la moins fine rendant uniformément continues les applications $u \mapsto f_\mu \circ u \circ g_\lambda$ de $\mathcal{F}(X; Y)$ dans les $\mathcal{F}_{\mathfrak{S}_\lambda}(X_\lambda; Y_\mu)$.

Ces propositions résultent immédiatement de la description d’un système fondamental d’entourages pour la structure uniforme de la $\mathfrak{S}$-convergence, donnée dans X, p. 3, Remarque 1; nous laissons les détails des démonstrations au lecteur.

#### Corollaire 1 {#top-x-s1-prop-4-cor-1 .statement}

Soient X un ensemble, $(Y_i)_{i \in I}$ une famille d’espaces uniformes, $\mathcal{S}$ un ensemble de parties de X. Si on munit $\prod_{i \in I} Y_i$ de la structure uniforme produit, la bijection canonique de l’espace uniforme $\mathcal{F}_{\mathcal{S}}(X, \prod_{i \in I} Y_i)$ sur l’espace uniforme produit $\prod_{i \in I} \mathcal{F}_{\mathcal{S}}(X; Y_i)$ (E, II, p. 39) est un isomorphisme.

Cela résulte de la prop. 4.

#### Corollaire 2 {#top-x-s1-prop-4-cor-2 .statement}

Soient X un ensemble, $\mathcal{S}$ un ensemble de parties de X et G un groupe topologique. Supposons que les structures uniformes droite et gauche (III, p. 19) de G soient identiques. Alors la topologie de la $\mathcal{S}$-convergence sur $\mathcal{F}(X, G)$ est compatible avec la structure de groupe de $\mathcal{F}(X, G)$ déduite de l’identification à $G^X$ (A, I, p. 43).

Soient $\mu : G \times G \to G$ et $\tilde{\mu} : \mathcal{F}_{\mathcal{S}}(X, G) \times \mathcal{F}_{\mathcal{S}}(X, G) \to \mathcal{F}_{\mathcal{S}}(X, G)$ les applications définies respectivement par $\mu(x, y) = xy^{-1}$ et $\tilde{\mu}(u, v) = u \cdot v^{-1}$. L’application $\mu$ est uniformément continue; soient en effet $x, x', y, y' \in G$ et V un voisinage de l’élément neutre $e$ de G; il existe un voisinage W de $e$ tel que, si $z, z' \in W^2$, alors $z'z \in V$. Si ${x'}^{-1}x \in W$ et $y^{-1}y' \in W$, alors ${x'}^{-1}xy^{-1}y' \in W^2$, donc $\mu(x', y')^{-1}\mu(x, y) \in V$. L’application $\tilde{\mu}$ est la composée de deux applications uniformément continues: la bijection canonique

$$
\mathcal{F}_{\mathcal{S}}(X, G) \times \mathcal{F}_{\mathcal{S}}(X, G) \to \mathcal{F}_{\mathcal{S}}(X, G \times G)
$$

(cor. 1) et l’application $w \mapsto \mu \circ w$ de $\mathcal{F}_{\mathcal{S}}(X, G \times G)$ dans $\mathcal{F}_{\mathcal{S}}(X, G)$ (prop. 4). D’où la continuité de $\tilde{\mu}$ et le corollaire d’après (III, p. 1).

#### Remarque 1 {#top-x-s1-n4-rem-1 .statement}

L’hypothèse du corollaire est satisfaite si G est commutatif ou compact.

#### Remarque 2 {#top-x-s1-n4-rem-2 .statement}

Pour tout partie $A \in \mathcal{S}$ et tout voisinage V de $e$ dans G, notons $L_0(A, V)$ l’ensemble des $u \in \mathcal{F}(X, G)$ tels que $u(A) \subset V$. Sous l’hypothèse du cor. 2, il résulte des définitions que, pour tout $u_0 \in \mathcal{F}(X, G)$, les ensembles $L_0(A, V) \cdot u_0$ (resp. $u_0 \cdot L_0(A, V)$) engendrent le filtre des voisinages de $u_0$ pour la topologie de la $\mathcal{S}$-convergence. En particulier, la structure uniforme de la $\mathcal{S}$-convergence et les structures uniformes droite et gauche du groupe topologique $\mathcal{F}(X, G)$ sont identiques.

### 5. Parties complètes de $\mathcal{F}_{\mathcal{S}}(X; Y)$

#### Proposition 5 {#top-x-s1-prop-5 .statement}

Soient X un ensemble, Y un espace uniforme, $\mathcal{S}$ un ensemble de parties de X. Pour qu’un filtre $\Phi$ sur $\mathcal{F}_{\mathcal{S}}(X; Y)$ converge vers $u_0$, il faut et il suffit que $\Phi$ soit un filtre de Cauchy pour la structure uniforme de la $\mathcal{S}$-convergence, et qu’il converge simplement vers $u_0$ dans $B = \bigcup_{A \in \mathcal{S}} A$.

Comme la structure de la convergence simple dans B est moins fine que celle de la $\mathcal{S}$-convergence, tout revient à démontrer que pour tout $A \in \mathcal{S}$ et tout entourage fermé V de Y, $W(A, V)$ est fermé pour la topologie de la convergence simple dans B (II, p. 16, prop. 7). Or, $W(A, V)$ est l’intersection des images réciproques de V par les applications $(u, v) \mapsto (u(x), v(x))$ ($x$ parcourant A), et ces dernières sont continues pour la topologie de la convergence simple (X, p. 4, Remarque 6), d’où la conclusion.

#### Corollaire 1 {#top-x-s1-prop-5-cor-1 .statement}

Pour qu’un sous-espace H de $\mathcal{F}_\mathfrak{S}(X; Y)$ soit complet, il faut et il suffit que, pour tout filtre de Cauchy $\Phi$ sur H, il existe $u_0 \in H$ tel que $\Phi$ converge simplement vers $u_0$ dans $B = \bigcup_{A \in \mathfrak{S}} A$.

Cela résulte aussitôt de la prop. 5.

#### Corollaire 2 {#top-x-s1-prop-5-cor-2 .statement}

Soient $\mathfrak{S}_1, \mathfrak{S}_2$ deux ensembles de parties de X ayant même réunion et tels que $\mathfrak{S}_1 \subset \mathfrak{S}_2$, et soit H une partie de $\mathcal{F}(X; Y)$; si H est complet pour la $\mathfrak{S}_1$-convergence, il est complet pour la $\mathfrak{S}_2$-convergence.

En effet, tout filtre de Cauchy pour la $\mathfrak{S}_2$-convergence est un filtre de Cauchy pour la $\mathfrak{S}_1$-convergence, et on peut appliquer le cor. 1.

#### Corollaire 3 {#top-x-s1-prop-5-cor-3 .statement}

Soit H une partie de $\mathcal{F}(X; Y)$ telle que, pour tout $x \in B = \bigcup_{A \in \mathfrak{S}} A$, l’adhérence de $H(x)$ dans Y soit un sous-espace complet. Alors l’adhérence $\overline{H}$ de H dans $\mathcal{F}_\mathfrak{S}(X; Y)$ est un sous-espace complet.

Soit $\Phi$ un filtre de Cauchy sur $\overline{H}$; définissons une application $v$ de X dans Y de la façon suivante. Si $x \in B$, $\Phi(x)$ est un filtre de Cauchy sur $\overline{H(x)}$ (X, p. 4, Remarque 6), donc a par hypothèse au moins un point limite; nous prendrons pour $v(x)$ un de ces points limites; si $x \notin B$, nous prendrons pour $v(x)$ un point quelconque de Y. Avec cette définition, il est clair que $\Phi$ converge simplement vers $v$ dans B, et $v$ est donc limite de $\Phi$ dans $\mathcal{F}_\mathfrak{S}(X; Y)$ en vertu de la prop. 5.

En particulier, si Y est complet, l’hypothèse du cor. 3 de la prop. 5 est vérifiée pour tout $H \subset \mathcal{F}(X; Y)$, d’où:

#### Théorème 1 {#top-x-s1-thm-1 .statement}

Soient X un ensemble, $\mathfrak{S}$ un ensemble de parties de X, Y un espace uniforme complet; alors l’espace uniforme $\mathcal{F}_\mathfrak{S}(X; Y)$ est complet.

### 6. La $\mathfrak{S}$-convergence dans les espaces d’applications continues

Soient X, Y deux espaces topologiques; on désigne par $\mathcal{C}(X; Y)$ l’ensemble des applications continues de X dans Y. Si $\mathfrak{S}$ est un ensemble de parties de X, et si Y est un espace uniforme, on désigne par $\mathcal{C}_\mathfrak{S}(X; Y)$ l’ensemble $\mathcal{C}(X; Y)$ muni de la structure uniforme de la $\mathfrak{S}$-convergence. En particulier, $\mathcal{C}_s(X; Y), \mathcal{C}_c(X; Y), \mathcal{C}_u(X; Y)$ désignent l’ensemble $\mathcal{C}(X; Y)$ muni respectivement de la structure uniforme de la convergence simple, de la convergence compacte et de la convergence uniforme.

#### Proposition 6 {#top-x-s1-prop-6 .statement}

Soient X un espace topologique, Y un espace uniforme, $\mathfrak{S}$ un ensemble de parties de X. Pour tout $A \in \mathfrak{S}$ et tout entourage fermé $V$ de $Y$, les traces sur $C(X; Y) \times C(X; Y)$ de $W(A, V)$ et de $W(\overline{A}, V)$ sont les mêmes.

En effet, si $u$ et $v$ sont des applications continues de $X$ dans $Y$, l’application $x \mapsto (u(x), v(x))$ de $X$ dans $Y \times Y$ est continue, et l’hypothèse que $(u(x), v(x)) \in V$ pour $x \in A$ entraîne donc $(u(x), v(x)) \in \nabla = V$ pour $x \in \overline{A}$ (I, p. 9, th. 1).

Si $\overline{\mathfrak{S}}$ désigne l’ensemble des adhérences dans $X$ des ensembles de $\mathfrak{S}$, la prop. 6 montre que, sur $C(X; Y)$, les structures de la $\mathfrak{S}$-convergence et de la $\overline{\mathfrak{S}}$-convergence sont les mêmes.

#### Corollaire {#top-x-s1-n6-cor-1 .statement}

Soit $B$ une partie partout dense de $X$; sur $C(X; Y)$, la structure de la convergence uniforme est identique à la structure de la convergence uniforme dans $B$.

#### Proposition 7 {#top-x-s1-prop-7 .statement}

Soient $X$ un espace topologique, $\mathfrak{S}$ un ensemble de parties de $X$, $Y$ un espace uniforme. Si $Y$ est séparé et si la réunion $B$ des ensembles de $\mathfrak{S}$ est dense dans $X$, alors $C_{\mathfrak{S}}(X; Y)$ est séparé.

En effet, si $u$ et $v$ appartiennent à tous les $W(A, V)$ ($A \in \mathfrak{S}$, $V$ entourage de $Y$), l’hypothèse que $Y$ est séparé entraîne $u(x) = v(x)$ pour tout $x \in B$; si $u$ et $v$ sont continues, on en conclut $u = v$ par le principe de prolongement des identités (I, p. 53, cor. 1).

En particulier, sur $C(X; Y)$, la topologie de la convergence simple dans un ensemble dense dans $X$ est séparée si $Y$ est séparé.

#### Proposition 8 {#top-x-s1-prop-8 .statement}

Soient $X$ un ensemble, $\mathcal{F}$ un filtre sur $X$, $Y$ un espace uniforme. L’ensemble $H$ des applications $u : X \to Y$ telles que $u(\mathcal{F})$ soit une base de filtre de Cauchy sur $Y$ est fermé dans $F_u(X; Y)$.

En effet, soit $u_0$ une application de $X$ dans $Y$ adhérente à $H$ dans $F_u(X; Y)$. Pour tout entourage symétrique $V$ de $Y$, il existe une application $u \in H$ telle que $(u_0(x), u(x)) \in V$ pour tout $x \in X$; d’autre part, il existe par hypothèse un ensemble $M \in \mathcal{F}$ tel que pour tout couple d’éléments $x, x'$ de $M$, on ait $(u(x), u(x')) \in V$. Comme on a $(u_0(x), u(x)) \in V$ et $(u_0(x'), u(x')) \in V$, on en déduit que $(u_0(x), u_0(x')) \in \overline{V}$ pour tout couple d’éléments $x, x'$ de $M$, d’où la proposition.

#### Corollaire 1 {#top-x-s1-prop-8-cor-1 .statement}

Soient $X$ un espace topologique, $Y$ un espace uniforme. L’ensemble des applications de $X$ dans $Y$, continues en un point $x_0 \in X$, est fermé dans $F_u(X; Y)$.

En effet, si $\mathcal{B}$ est le filtre des voisinages de $x_0$ dans $X$, $u(x_0)$ est un point adhérent à $u(\mathcal{B})$; donc, pour que $u$ soit continue au point $x_0$, il faut et il suffit que $u(\mathcal{B})$ soit une base de filtre de Cauchy sur $Y$ (II, p. 14, cor. 2).

#### Corollaire 2 {#top-x-s1-prop-8-cor-2 .statement}

Soient $X, L$ deux ensembles filtrés par des filtres $\mathcal{F}, \mathfrak{S}$ respectivement, et soit $Y$ un espace uniforme complet. Pour tout $\lambda \in L$, soit $u_\lambda$ une application de $X$ dans $Y$. On suppose que : 1° suivant le filtre $\mathfrak{S}$, la famille $(u_\lambda)_{\lambda \in L}$ converge uniformément dans $X$ vers une application $v$ de $X$ dans $Y$; 2° pour tout $\lambda \in L$, $u_\lambda$ a une limite $y_\lambda$ suivant le filtre $\mathcal{F}$. Dans ces conditions, $v$ a une limite suivant le filtre $\mathcal{F}$, et toute limite de $v$ suivant $\mathcal{F}$ est limite de la famille $(y_\lambda)_{\lambda \in L}$ suivant $\mathfrak{S}$.

En effet, $v$ est adhérente à l’ensemble des $u_\lambda$ dans $\mathcal{F}_u(X; Y)$, donc $v(\mathcal{F})$ est une base filtre de Cauchy sur $Y$ en vertu de la prop. 8, ce qui prouve que $v$ admet une limite $y$ suivant $\mathcal{F}$ puisque $Y$ est complet. Soit $X' = X \cup \{\omega\}$ l’espace topologique associé au filtre $\mathcal{F}$ (I, p. 40) et prolongeons $u_\lambda$ (resp. $v$) en une application $\bar{u}_\lambda$ (resp. $\bar{v}$) de $X'$ dans $Y$ en posant $\bar{u}_\lambda(\omega) = y_\lambda$ (resp. $\bar{v}(\omega) = y$). Alors les $\bar{v}_\lambda$ et $\bar{v}$ sont continues dans $X'$, et $\bar{u}_\lambda$ converge uniformément dans $X$ vers $\bar{v}$ suivant $\mathfrak{S}$; comme $X$ est dense dans $X'$, il résulte de X, p. 8, corollaire, que $\bar{u}_\lambda$ converge uniformément dans $X'$ vers $\bar{v}$, et en particulier que $y = \lim_{\mathfrak{S}} y_\lambda$.

#### Théorème 2 {#top-x-s1-thm-2 .statement}

Soient $X$ un espace topologique, $Y$ un espace uniforme. Alors l’ensemble $C(X; Y)$ des applications continues de $X$ dans $Y$ est une partie fermée de $\mathcal{F}(X; Y)$ muni de la topologie de la convergence uniforme.

En effet, pour tout $x \in X$, l’ensemble des applications de $X$ dans $Y$ qui sont continues au point $x$ est fermé dans $\mathcal{F}_u(X; Y)$ (X, p. 8, cor. 1), donc l’intersection $C(X; Y)$ de ces ensembles est aussi fermé.

On exprime encore ce résultat en disant que toute limite uniforme de fonctions continues est continue.

#### Corollaire 1 {#top-x-s1-thm-2-cor-1 .statement}

Si $Y$ est un espace uniforme complet, $C_u(X; Y)$ est complet.

En effet, en vertu du th. 2, $C_u(X; Y)$ est un sous-espace uniforme fermé de l’espace uniforme $\mathcal{F}_u(X; Y)$, qui est complet en vertu de X, p. 7, th. 1.

#### Corollaire 2 {#top-x-s1-thm-2-cor-2 .statement}

Soient $X$ un espace topologique, $\mathfrak{S}$ un ensemble de parties de $X$, $Y$ un espace uniforme ; on désigne par $\tilde{C}_\mathfrak{S}(X; Y)$ l’ensemble des applications de $X$ dans $Y$ dont la restriction à tout ensemble de $\mathfrak{S}$ est continue. Alors $\tilde{C}_\mathfrak{S}(X; Y)$ est fermé dans l’espace uniforme $\mathcal{F}_\mathfrak{S}(X; Y)$ et est un sous-espace uniforme complet lorsque $Y$ est complet.

En effet, supposons que $u$ soit adhérente à $\tilde{C}_\mathfrak{S}(X; Y)$ dans $\mathcal{F}_\mathfrak{S}(X; Y)$ alors (X, p. 2), pour tout $A \in \mathfrak{S}$, $u|_A$ est adhérente à $C(A; Y)$ dans $\mathcal{F}_u(A; Y)$, donc est continue en vertu du th. 2.

#### Corollaire 3 {#top-x-s1-thm-2-cor-3 .statement}

Soient $X$ un espace topologique métrisable ou localement compact, $Y$ un espace uniforme. Alors $C(X; Y)$ est fermé dans l’espace $\mathcal{F}_c(X; Y)$; si en outre $Y$ est complet, l’espace uniforme $C_c(X; Y)$ est complet.

En vertu du cor. 2, tout revient à voir que, si on prend pour $\mathfrak{S}$ l’ensemble des parties compactes de $X$, on a $\tilde{C}_\mathfrak{S}(X; Y) = C(X; Y)$ dans les deux cas envisagés. C’est évident si $X$ est localement compact ; si $X$ est métrisable, l’hypothèse que la restriction de $u : X \to Y$ à toute partie compacte de $X$ est continue entraîne en particulier que pour tout $x \in X$ et toute suite $(z_n)$ de points de $X$ qui converge vers $x$, on a $u(x) = \lim_{n \to \infty} u(z_n)$; donc $u$ est continue en $x$ (IX, p. 17, prop. 10).

On notera que le raisonnement précédent s’applique généralement lorsque tout point de X possède un système fondamental dénombrable de voisinages.

#### Remarque 1 {#top-x-s1-n6-rem-1 .statement}

En général, l’ensemble $\mathcal{C}(X; Y)$ n’est pas fermé dans $\mathcal{F}(X; Y)$ muni de la topologie de la convergence simple; en d’autres termes, une limite simple de fonctions continues n’est pas nécessairement continue (X, p. 42, exerc. 5a)).

#### Remarque 2 {#top-x-s1-n6-rem-2 .statement}

Un filtre sur $\mathcal{C}(X; Y)$ peut converger simplement vers une fonction continue sans converger uniformément vers cette fonction.

Par exemple, dans l’intervalle $I = [0, 1]$, soit $u_n$ la fonction numérique égale à 0 pour $x = 0$ et pour $2/n \leq x \leq 1$, égale à 1 pour $x = 1/n$, et linéaire dans chacun des intervalles $[0, 1/n]$ et $[1/n, 2/n]$; la suite $(u_n)$ converge simplement vers 0, mais ne converge pas uniformément vers 0 dans I (cf. X, p. 42, exerc. 6).

#### Remarque 3 {#top-x-s1-n6-rem-3 .statement}

Si X est un espace uniforme, un raisonnement tout à fait analogue à celui de X, p. 8, prop. 8 montre que l’ensemble des applications uniformément continues de X dans Y est fermé dans $\mathcal{F}_u(X; Y)$.

#### Remarque 4 {#top-x-s1-n6-rem-4 .statement}

Supposons que l’espace uniforme Y soit muni d’une loi de composition associative et commutative, notée additivement, et telle que l’application $(y, y') \mapsto y + y'$ soit continue dans $Y \times Y$. Alors, si $(u_n)$ est une suite d’applications continues de X dans Y telle que la série de terme générale $u_n$ soit uniformément convergente dans X, la somme de cette série est continue dans X.

Nous laissons au lecteur le soin d’énoncer le résultat correspondant pour les familles uniformément sommables (X, p. 3, Remarque 5) d’applications continues.

#### Proposition 9 {#top-x-s1-prop-9 .statement}

Soient X un espace topologique, Y un espace uniforme. Alors l’application $(f, x) \mapsto f(x)$ de $C_u(X; Y) \times X$ dans Y est continue.

En effet, soient $f_0$ une application continue de X dans Y, $x_0$ un point de X, V un entourage symétrique de Y. L’ensemble T des applications continues $f : X \to Y$ telles que $(f(x), f_0(x)) \in V$ pour tout $x \in X$ est un voisinage de $f_0$ dans $\mathcal{C}_u(X; Y)$. D’autre part, comme $f_0$ est continue, il existe un voisinage U de $x_0$ dans X tel que $(f_0(x), f_0(x_0)) \in V$ pour tout $x \in U$. On a par suite $(f(x), f_0(x_0)) \in \overline{V}^2$ pour $(f, x) \in T \times U$, ce qui démontre la proposition.

## EXERCICES {#top-x-s1-exercises}

See the [exercises for § 1](exercises/s1/).
