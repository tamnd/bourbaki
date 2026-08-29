---
book: top
book_title: General Topology
chapter: III
chapter_title: GROUPES TOPOLOGIQUES
section: 7
section_title: Limites projectives de groupes et d’anneaux topologiques
lang: fr
source: top-i-iv-fr
book_pages: TG III.85-TG III.87
pdf_pages: 0240-0249, 0268-0270
extraction: ocr
subsections:
    - "no": 1
      title: Limites projectives de groupes topologiques et d’espaces à l’opérateurs
      page: 0
      pdf_page: 240
    - "no": 2
      title: Approximation des groupes topologiques
      page: 59
      pdf_page: 242
    - "no": 3
      title: Application aux limites projectives
      page: 64
      pdf_page: 247
statements: 16
exercises: 6
content_sha256: c7807319adb537d56b965861ed731b38f67148ba59ad9a2cabfad494d6ae1bea
---

## § 7. LIMITES PROJECTIVES DE GROUPES ET D’ANNEAUX TOPOLOGIQUES

Dans tout ce paragraphe, on désigne par I un ensemble préordonné filtrant à droite¹ et non vide, par $\alpha \leq \beta$ la relation de préordre dans I. Sauf mention expresse du contraire, tous les systèmes projectifs considérés ont pour ensemble d’indices I.

### 1. Limites projectives de groupes topologiques et d’espaces à l’opérateurs

Nous dirons qu’un système projectif $(G_\alpha, f_{\alpha\beta})$ est un système projectif de groupes topologiques si les $G_\alpha$ sont des groupes topologiques et les $f_{\alpha\beta}$ des homomorphismes continus. Alors $G = \lim_{\leftarrow} G_\alpha$ est un sous-groupe du groupe produit $\prod_\alpha G_\alpha$ (A, I, p. 113); lorsqu’on le munit de la structure de groupe topologique induite par celle de $\prod_\alpha G_\alpha$, on dit que le groupe topologique ainsi obtenu est limite projective du système projectif de groupes topologiques $(G_\alpha, f_{\alpha\beta})$. Si les $G_\alpha$ sont séparés (resp. séparés et complets), G est séparé et fermé dans $\prod_\alpha G_\alpha$ (resp. séparé et complet) (I, p. 55, cor. 2 et II, p. 17, corollaire).

Si $(G'_\alpha, f'_{\alpha\beta})$ est un second système projectif de groupes topologiques et si, pour tout $\alpha$, $u_\alpha : G_\alpha \to G'_\alpha$ est un homomorphisme continu, tel que les $u_\alpha$ forment un système projectif d’applications, alors $u = \lim_{\leftarrow} u_\alpha$ est un homomorphisme continu de G dans $G' = \lim_{\leftarrow} G'_\alpha$ (I, p. 28). Les mêmes résultats sont valables lorsqu’on remplace « groupe topologique » par « anneau topologique »; on laisse au lecteur le soin d’énoncer les résultats analogues pour les modules topologiques (III, p. 52).

Soient $(E_\alpha, g_{\alpha\beta})$ un système projectif d’espaces topologiques, $(G_\alpha, f_{\alpha\beta})$ un système projectif de groupes topologiques; supposons que chaque $G_\alpha$ opère continûment dans $E_\alpha$ (III, p. 9) et que l’on ait les relations

(1)
$$
g_{\alpha\beta}(s_\beta \cdot x_\beta) = f_{\alpha\beta}(s_\beta) \cdot g_{\alpha\beta}(x_\beta)
$$
pour $x_\beta \in E_\beta, s_\beta \in G_\beta, \alpha \leq \beta$. On sait (A, I, p. 114) que le groupe $G = \lim_{\leftarrow} G_\alpha$ opère dans $E = \lim_{\leftarrow} E_\alpha$; en outre G opère continûment dans E. En effet, si $g_\alpha$ (resp. $f_\alpha$) est l’application canonique $E \to E_\alpha$ (resp. $G \to G_\alpha$), on a par définition
$$
g_\alpha(s \cdot x) = f_\alpha(s) \cdot g_\alpha(x)
$$

¹ On notera que la définition de la limite projective d’un système projectif d’ensembles $(E_\alpha, f_{\alpha\beta})$ ne suppose pas que l’ensemble préordonné d’indices I soit filtrant (E, III, p. 52); le lecteur vérifiera sans peine que cette hypothèse n’intervient pas non plus dans la plupart des définitions et résultats de ce paragraphe, avant la prop. 1.

donc les applications $(s, x) \mapsto g_\alpha(s.x)$ sont continues dans $E \times G$, ce qui prouve la continuité de $(s, x) \mapsto s.x$ (I, p. 28).

L’application $h_\alpha : E/G \to E_\alpha/G_\alpha$ déduite de $f_\alpha$ et $g_\alpha$ est donc continue (III, p. 10), et il en est de même de l’application $h : E/G \to \lim_{\leftarrow} E_\alpha/G_\alpha$ déduite des $h_\alpha$ (I, p. 28).

#### Proposition 1 {#top-iii-s7-prop-1 .statement}

*Les $E_\alpha$ et $G_\alpha$ étant supposés vérifier les hypothèses précédentes*:

a) *Si, pour tout $\alpha \in I$, le stabilisateur de tout point de $E_\alpha$ est un sous-groupe compact de $G_\alpha$, alors le stabilisateur de tout point $x = (x_\alpha)$ de $E$ est un sous-groupe compact de $G$, l’orbite de $x$ (pour $G$) est canoniquement homéomorphe à la limite projective des orbites des $x_\alpha$ (pour les $G_\alpha$), et l’application canonique $h : E/G \to \lim_{\leftarrow} E_\alpha/G_\alpha$ est injective*.

b) *Si, pour tout $\alpha \in I$, toute orbite d’un point de $E_\alpha$ (pour $G_\alpha$) est compacte, alors toute orbite d’un point de $E$ (pour $G$) est relativement compacte, et $h$ est surjective. Si en outre $h$ est bijective, toute orbite d’un point de $E$ est compacte*.

Soit $x = (x_\alpha) \in E$, et pour tout $\alpha \in I$, soit $E'_\alpha = G_\alpha.x_\alpha$ l’orbite de $x_\alpha$. Pour $\alpha \leq \beta$, il résulte de (1) et de la relation $g_{\alpha\beta}(x_\beta) = x_\alpha$ que l’on a $g_{\alpha\beta}(E'_\beta) \subset E'_\alpha$, autrement dit, $(E'_\alpha)$ est un système projectif de parties des $E_\alpha$. Pour tout $\alpha \in I$, soit $u_\alpha : G_\alpha \to E'_\alpha$ l’application continue $s_\alpha \mapsto s_\alpha.x_\alpha$; les $u_\alpha$ forment un système projectif d’applications, et $u = \lim_{\leftarrow} u_\alpha$ est l’application continue $s \mapsto s.x$ de $G$ dans le sous-espace $E' = \lim_{\leftarrow} E'_\alpha$ de $E$. L’hypothèse de a) entraîne que $\overline{u_\alpha^{-1}}(y_\alpha)$ est compact pour tout $y_\alpha \in E'_\alpha$. Comme en outre $u_\alpha$ est surjectif, les conditions de I, p. 65, cor. 2, *a*) sont vérifiées, donc on en déduit les deux premières assertions de a). Ceci entraîne que si $x = (x_\alpha)$ et $y = (y_\alpha)$ sont tels que, pour tout $\alpha$, $x_\alpha$ et $y_\alpha$ appartiennent à la même orbite pour $G_\alpha$, alors $x$ et $y$ appartiennent à la même orbite pour $G$, ce qui prouve que $h$ est injective.

De même, l’hypothèse de b) entraîne que le système projectif des applications canoniques $v_\alpha : E_\alpha \to E_\alpha/G_\alpha$ vérifie les conditions de I, p. 65, cor. 2, *a*), donc sa limite projective $v = \lim_{\leftarrow} v_\alpha : E \to \lim_{\leftarrow} E_\alpha/G_\alpha$ est surjective et l’image réciproque par $v$ de tout point de $\lim_{\leftarrow} E_\alpha/G_\alpha$ est compacte. Comme $v$ se factorise en $E \xrightarrow{\psi} E/G \xrightarrow{h} \lim_{\leftarrow} E_\alpha/G_\alpha$, où $\psi$ est l’application canonique, on en déduit les assertions de b).

#### Corollaire 1 {#top-iii-s7-prop-1-cor-1 .statement}

*Si les $G_\alpha$ sont compacts et les $E_\alpha$ séparés, les conclusions de a) et de b) sont valables*.

En effet, les hypothèses de a) et b) sont vérifiées, tout sous-groupe fermé de $G_\alpha$ étant compact et $u_\alpha : s_\alpha \mapsto s_\alpha.x_\alpha$ étant une application continue d’un espace compact dans un espace séparé.

#### Corollaire 2 {#top-iii-s7-prop-1-cor-2 .statement}

*Si, pour tout $\alpha \in I$, le groupe $G_\alpha$ opère transitivement dans l’espace $E_\alpha$, et si le stabilisateur de tout point de $E_\alpha$ est un sous-groupe compact de $G_\alpha$, alors $G$ opère transitivement dans $E$ et le stabilisateur de tout point de $E$ est un sous-groupe compact de $G$*.

En effet, l’hypothèse de la prop. 1, a) est vérifiée, et $E'_\alpha = E_\alpha$ pour tout $\alpha$.

#### Corollaire 3 {#top-iii-s7-prop-1-cor-3 .statement}

*On suppose les $G_\alpha$ séparés. Pour tout $\alpha \in I$, soit $K_\alpha$ un sous-groupe compact de $G_\alpha$ et supposons que l’on ait $f_{\alpha \beta}(K_\beta) \subset K_\alpha$ pour $\alpha \leq \beta$. Alors, si $K = \lim_{\leftarrow} K_\alpha$, l’application canonique $h$ de l’espace homogène $G/K$ dans $\lim_{\leftarrow} G_\alpha / K_\alpha$ est un homéomorphisme.*

Avec les notations de la prop. 1, le fait que $h$ est bijective résulte du cor. 1 appliqué en remplaçant $E_\alpha$ par $G_\alpha$ et $G_\alpha$ par $K_\alpha$ opérant *à droite* par les translations (III, p. 11). Soit $\varphi$ l’application canonique $G \to G/K$, et pour tout $\alpha$, soit $f_\alpha$ l’application canonique $G \to G_\alpha$; lorsque, pour chaque $\alpha$, les $V_\alpha$ parcourent un système fondamental de voisinages ouverts de l’élément neutre $e_\alpha$ de $G_\alpha$, les ensembles $V = f^{-1}_\alpha(V_\alpha)$ ($\alpha$ et $V_\alpha$ variables) forment un système fondamental de voisinages de $e$ dans $G$ (I, p. 29, prop. 9), et les $\varphi(V.K)$ un système fondamental de voisinages de $\varphi(e)$ dans $G/K$. Il s’agit de prouver que l’image par $h$ de $\varphi(V.K)$ contient un voisinage de $h(\varphi(e))$, c’est-à-dire qu’il existe un $\beta \geq \alpha$ et un voisinage $W_\beta$ de $e_\beta$ dans $G_\beta$ tels que $f^{-1}_\beta(W_\beta.K_\beta) \subset V.K$. Or, la relation $x \in V.K$ équivaut à l’existence d’un $y \in K$ tel que $f_\alpha(xy^{-1}) \in V_\alpha$, ou encore $f_\alpha(x) \in V_\alpha.f_\alpha(K)$, autrement dit, on a $V.K = f^{-1}_\alpha(V_\alpha.f_\alpha(K))$. Soit $U_\alpha = V_\alpha.f_\alpha(K)$; nous allons voir qu’il existe $\beta \geq \alpha$ tel que si on pose $U_\beta = f^{-1}_{\alpha \beta}(U_\alpha)$, on ait $K_\beta \subset U_\beta$; il en résultera bien qu’il existe un voisinage $W_\beta$ de $e_\beta$ dans $G_\beta$ tel que $W_\beta.K_\beta \subset U_\beta$ (II, p. 31, corollaire), ce qui établira la relation cherchée $f^{-1}_\beta(W_\beta.K_\beta) \subset f^{-1}_\beta(U_\beta) = V.K$. Raisonnons par l’absurde, et posons, pour tout $\beta \geq \alpha$, $M_\beta = K_\beta \cap G U_\beta$; comme $f^{-1}_{\beta \gamma}(U_\beta) = U_\gamma$ pour $\alpha \leq \beta \leq \gamma$, les $M_\beta$ forment un système projectif de parties compactes des $G_\beta$ (pour $\beta \geq \alpha$); s’ils étaient tous non vides, il en serait de même de leur limite projective $M$ (I, p. 64, prop. 8). Il est clair que l’on a $M \subset K$ et $f_\alpha(M) \subset M_\alpha$; mais cela est absurde puisque $f_\alpha(K) \subset U_\alpha$, ce qui achève la démonstration.

### 2. Approximation des groupes topologiques

Soit $G$ un groupe et soit $(H_\alpha)_{\alpha \in I}$ une famille filtrante décroissante de sous-groupes distingués de $G$. Pour tout $\alpha \in I$, soit $G_\alpha = G/H_\alpha$, et pour $\alpha \leq \beta$, soit $f_{\alpha \beta}$ l’homomorphisme canonique $G/H_\beta \to G/H_\alpha$, qui fait donc correspondre à toute classe $T$ de $G$ mod. $H_\beta$ la classe $TH_\alpha$ de $G$ mod. $H_\alpha$ qui contient $T$. Il est clair que $(G_\alpha, f_{\alpha \beta})$ est un système projectif de groupes, les éléments de $\tilde{G} = \lim_{\leftarrow} G_\alpha$ étant les familles décroissantes $(T_\alpha)_{\alpha \in I}$, où $T_\alpha$ est une classe de $G$ mod. $H_\alpha$ pour tout $\alpha$. L’application $i : s \mapsto (sH_\alpha)$ de $G$ dans $\tilde{G}$, limite projective des homomorphismes canoniques $G \to G/H_\alpha$, est un homomorphisme de $G$ dans $\tilde{G}$, et l’image réciproque par $i$ d’un élément $(T_\alpha) \in \tilde{G}$ est égale à $\bigcap_{\alpha \in I} T_\alpha$. Le noyau de $i$ est donc $\bigcap_{\alpha \in I} H_\alpha$, et l’image de $i$ se compose des familles $(T_\alpha) \in \tilde{G}$ dont l’intersection est non vide.

Supposons maintenant que $G$ soit un groupe topologique ; si on munit $G_\alpha = G / H_\alpha$ de la topologie quotient, il est clair que $(G_\alpha, f_{\alpha \beta})$ est un système projectif de groupes topologiques, et que $i : G \to \tilde{G}$ est un homomorphisme continu.

#### Proposition 2 {#top-iii-s7-prop-2 .statement}

*Soient G un groupe topologique, $(H_\alpha)_{\alpha \in I}$ une famille filtrante décroissante de sous-groupes distingués de G vérifiant la condition suivante :

(AP) Pour tout $\alpha \in I$, $H_\alpha$ est fermé dans $G$ et tout voisinage de $e$ dans $G$ contient un des $H_\alpha$ (autrement dit, la base de filtre formée des $H_\alpha$ converge vers $e$).

Alors l’application $i : G \to \tilde{G} = \lim_{\leftarrow} G / H_\alpha$ est un morphisme strict de $G$ sur $i(G)$ ; $\tilde{G}$ est séparé et $i(G)$ est dense dans $\tilde{G}$ ; enfin le noyau de $i$ est l’adhérence de $\{e\}$ dans $G$. Si en outre un des $H_\alpha$ est complet, alors $i$ est surjective.

Il est clair que les $G_\alpha = G / H_\alpha$ sont séparés (III, p. 13, prop. 18), donc il en est de même de $\tilde{G}$, sous-espace de $\prod_{\alpha \in I} G_\alpha$. Le noyau $H$ de $i$ est l’intersection des $H_\alpha$, et est donc un sous-groupe fermé de $G$ ; comme tout voisinage de $e$ contient l’un des $H_\alpha$, il contient $H$, et par suite (III, p. 20, formule (1)) $H$ est l’adhérence de $\{e\}$. Montrons ensuite que $i(G)$ est dense dans $\tilde{G}$. Soit $f_\alpha$ l’application canonique $\tilde{G} \to G_\alpha$, restriction à $\tilde{G}$ de la projection $pr_\alpha$ ; $\varphi_\alpha = f_\alpha \circ i$ est l’application canonique $G \to G / H_\alpha$. Pour tout ensemble ouvert non vide $U$ de $\tilde{G}$, il existe un $\alpha \in I$ et un ensemble ouvert non vide $U_\alpha$ dans $G_\alpha$ tels que $f_\alpha^{-1}(U_\alpha) \subset U$ (I, p. 29, prop. 9), donc $i(U) \supset \varphi_\alpha^{-1}(U_\alpha)$ ; mais comme $\varphi_\alpha$ est surjective, $i(U)$ n’est pas vide, ce qui prouve qui $i(G) \cap U \neq \varnothing$.

Pour voir que $i$ est un morphisme strict sur $i(G)$, considérons un voisinage $V$ de $e$ dans $G$ ; il existe un voisinage $W$ de $e$ dans $G$ tel que $W^2 \subset V$, et un $\alpha \in I$ tel que $H_\alpha \subset W$ ; on en déduit que $V$ contient $WH_\alpha = \varphi_\alpha^{-1}(\varphi_\alpha(W)) = i(f_\alpha(\varphi_\alpha(W)))$ ; comme $f_\alpha(\varphi_\alpha(W))$ est un voisinage de l’élément neutre dans $\tilde{G}$, cela prouve notre assertion (III, p. 16, prop. 24).

Enfin, supposons qu’il existe un $\gamma \in I$ tel que $H_\gamma$ soit complet ; pour voir que $i$ est surjective, il suffit de prouver que toute famille décroissante $(T_\alpha) \in \tilde{G}$ a une intersection non vide. Comme $T_\gamma$ se déduit par translation de $H_\gamma$, c’est un sous-espace complet de $G$ (pour la structure uniforme droite et la structure uniforme gauche). De plus, comme tout voisinage $U$ de $e$ dans $G$ contient l’un des $H_\alpha$, l’ensemble $T_\alpha$ correspondant est petit d’ordre $U_d$ (ou $U_s$), autrement dit l’ensemble des $T_\alpha$ contenus dans $T_\gamma$ est une base de *filtre de Cauchy* ; elle converge donc dans $T_\gamma$, et comme les $T_\alpha$ sont fermés dans $G$ (étant déduits par translation des $H_\alpha$), leur intersection est non vide.

C.Q.F.D.

#### Corollaire 1 {#top-iii-s7-prop-2-cor-1 .statement}

Si la condition (AP) est vérifiée et si en outre les groupes (séparés) $G/H_\alpha$ sont complets, le groupe $G$ admet un groupe séparé complété, qui s’identifie à $\tilde{G}$, l’application $i : G \to \tilde{G}$ s’identifiant à l’application canonique (III, p. 25).

En effet, $\tilde{G}$ est alors complet (III, p. 57) et la prop. 2 montre que $i(G)$ est isomorphe au groupe séparé associé à $G$; comme il est dense dans $\tilde{G}$, on en déduit le corollaire (III, p. 25).

En particulier:

#### Corollaire 2 {#top-iii-s7-prop-2-cor-2 .statement}

Soient $G$ un groupe, $(H_\alpha)$ une famille filtrante décroissante de sous-groupes distingués de $G$. Si l’on munit $G$ de la topologie de groupe pour laquelle les $H_\alpha$ forment un système fondamental de voisinages de $e$ (III, p. 5, Exemple), le groupe séparé associé à $G$ est isomorphe à $G/(\bigcap_\alpha H_\alpha) = G_1$, $G_1$ admet un groupe complété et l’application canonique $G_1 \to \tilde{G} = \lim_{\leftarrow} G/H_\alpha$ se prolonge en un isomorphisme de $\hat{G} = \hat{G}_1$ sur $\tilde{G}$.

En effet, le sous-groupe $H_\alpha$ de $G$ étant ouvert, est aussi fermé (III, p. 7, corollaire) et $G/H_\alpha$ est discret (III, p. 13, prop. 18), donc les conditions du cor. 1 sont satisfaites.

#### Corollaire 3 {#top-iii-s7-prop-2-cor-3 .statement}

Soient $G$ un groupe, $G_0$ un sous-groupe de $G$, $(H_\alpha)$ une famille filtrante décroissante de sous-groupes distingués de $G_0$. On suppose que les $H_\alpha$ forment un système fondamental de voisinages de $e$ pour une topologie séparée sur $G$, compatible avec la structure de groupe de $G$. Alors le groupe topologique $G$ ainsi défini admet un groupe complété $\hat{G}$, et l’adhérence $\overline{G_0}$ de $G_0$ dans $\hat{G}$ est canoniquement isomorphe à $\lim_{\leftarrow} G_0/H_\alpha$.

En effet, $G_0$ est un sous-groupe ouvert de $G$; l’application $x \mapsto x^{-1}$ de $G_0$ dans $G$ est uniformément continue pour la structure uniforme droite de $G$, car les relations $x \in G_0,\ y \in G_0,\ xy^{-1} \in H_\alpha$ entraînent $yx^{-1} \in H_\alpha$, puis $x^{-1}y = x^{-1}(yx^{-1})x \in H_\alpha$ puisque $H_\alpha$ est un sous-groupe distingué de $G_0$. L’existence du groupe complété $\hat{G}$ résulte donc de III, p. 25, prop. 9; comme alors $\overline{G_0}$ s’identifie au groupe complété de $G_0$ (II, p. 26, cor. 1), la seconde assertion résulte du cor. 2.

Dans toute la fin de ce numéro, nous supposerons que $G$ est séparé et que $(H_\alpha)$ est une famille décroissante filtrante de sous-groupes distingués compacts vérifiant la condition (AP); en vertu de la prop. 2 (III, p. 60), l’application $i : G \to \tilde{G} = \lim_{\leftarrow} G/H_\alpha$ est alors un isomorphisme de groupes topologiques, permettant d’identifier $G$ et $\tilde{G}$; nous noterons $f_\alpha$ l’application canonique $G \to G/H_\alpha$.

#### Lemme 1 {#top-iii-s7-lem-1 .statement}

Sous les hypothèses de la prop. 2 (III, p. 60), pour toute partie fermée $E$ de $G$, on a $E = \bigcap_\alpha EH_\alpha$.

En effet, $E$ est l’intersection des ensembles $EV$, où $V$ parcourt le filtre des voisinages de $e$ (III, p. 20, formule (1)), et tout voisinage de $e$ contient un $H_\alpha$; d’où la conclusion puisque $E \subset EH_\alpha$.

#### Proposition 3 {#top-iii-s7-prop-3 .statement}

On suppose G séparé, les H_α compacts et vérifiant (AP).

a) Soit L un sous-groupe fermé de G ; alors, pour tout α ∈ I, le sous-groupe L_α = f_α(L) de G_α = G/H_α est fermé, et l’isomorphisme i de G sur lim ← G_α donne par restriction un isomorphisme de L sur lim ← L_α. Si de plus L est distingué dans G, alors L_α est distingué dans G_α pour tout α ∈ A, et par passage aux quotients, i donne un isomorphisme de G/L sur lim ← G_α/L_α.

b) Inversement, pour tout α ∈ I, soit L_α un sous-groupe fermé de G_α, et supposons que l’on ait L_α = f_{αβ}(L_β) pour α ≤ β. Il existe alors un sous-groupe fermé L de G et un seul tel que L_α = f_α(L) pour tout α ∈ I ; en outre, si pour tout α ∈ I, L_α est distingué dans G_α, alors L est distingué dans G.

a) Comme H_α est compact, LH_α est fermé dans G (III, p. 28, cor. 1), donc L_α est fermé dans G_α. Puisque i identifie les groupes topologiques G et lim ← G_α et que lim ← L_α s’identifie à un sous-groupe (topologique) de lim ← G_α, i identifie à lim ← L_α le sous-groupe ∩_α LH_α de G, et pour démontrer la première assertion, il suffit de remarquer que L = ∩_α LH_α en vertu du lemme 1. D’autre part, si L est distingué, alors, pour tout α ∈ I, l’application f_α′ : G/L → G_α/L_α déduite de f_α par passage aux quotients est un morphisme strict surjectif (III, p. 17, Remarque 3), dont le noyau est le sous-groupe distingué compact H_αL/L de G/L, image canonique du sous-groupe compact H_α de G. Comme les sous-groupes H_αL/L de G/L vérifient la condition (AP) (III, p. 16, prop. 24) et que G/L est séparé, la dernière assertion de a) résulte de la prop. 2 de III, p. 60.

b) Soit f_{αβ}′ la restriction de f_{αβ} à L_β pour α ≤ β ; (L_α, f_{αβ}′) est alors un système projectif de groupes topologiques, dont la limite projective L s’identifie au sous-groupe G ∩ ∏_α L_α de G. Par hypothèse f_{αβ}′ est surjective et son noyau est le sous-groupe compact f_β(H_α) ∩ L_β de L_β ; par suite (I, p. 64, cor. 1) on a L_α = f_α(L) pour tout α ∈ I. Si L′ est un second sous-groupe fermé de G tel que f_α(L′) = L_α pour tout α ∈ I, on a L′H_α = f_α^{-1}(L_α), d’où (lemme 1)

$$
L' = \bigcap_\alpha L'H_\alpha = \bigcap_\alpha f_\alpha^{-1}(L_\alpha) = L.
$$

Enfin, la dernière assertion de b) résulte de la formule L = ∩_α f_α^{-1}(L_α), les f_α^{-1}(L_α) étant alors distingués dans G.

#### Proposition 4 {#top-iii-s7-prop-4 .statement}

On suppose G séparé, les H_α compacts et vérifiant (AP). Si C_α est la composante neutre de G_α = G/H_α, la composante neutre C de G s’identifie à lim ← C_α et on a f_α(C) = C_α.

La proposition résultera du lemme suivant:

#### Lemme 2 {#top-iii-s7-lem-2 .statement}

Soient G un groupe topologique séparé, H un sous-groupe distingué compact de G, φ l’application canonique G → G/H. Si C est la composante neutre de G, φ(C) est la composante neutre de G' = G/H.

En effet, une fois ce lemme établi, on aura $f_\alpha(C) = C_\alpha$ pour tout $\alpha \in I$, et comme C est un sous-groupe fermé de G (III, p. 8, prop. 8), il suffira d’appliquer la prop. 3 a) de III, p. 62.

Pour démontrer le lemme 2, observons d’abord que si C’ est la composante connexe de l’élément neutre $e'$ dans G’, on a $\varphi(C) \subset C'$ puisque $\varphi(C)$ est connexe. Supposons que $\varphi(C) \neq C'$. Comme C est un sous-groupe distingué fermé de G (III, p. 8, prop. 8), $\varphi(C)$ est un sous-groupe distingué de G’; si $\psi$ est l’application canonique $G' \to G'/\varphi(C)$, $\psi(C')$ serait connexe et non réduit à l’élément neutre, donc la composante connexe de $G'/\varphi(C)$ serait distincte de l’élément neutre. Mais $G'/\varphi(C)$ est isomorphe à $(G/H)/(HC/H)$, donc à $G/HC$, et par suite aussi à $(G/C)/(HC/C)$ (III, p. 15, corollaire et III, p. 14, prop. 20). Or, G/C est séparé et totalement discontinu (I, p. 84, prop. 9), et HC/C, image canonique du sous-groupe distingué compact H de G, est un sous-groupe compact de G/C. On est donc ramené à démontrer le lemme 2 lorsque G est en outre supposé totalement discontinu, soit $C = \{e\}$.

Supposons alors que $C' \neq \{e'\}$; en remplaçant G par son sous-groupe $\overline{\varphi}^{-1}(C')$, qui est totalement discontinu et contient H, on peut supposer que G’ est connexe et non réduit à un point.

Soit $\mathfrak{M}$ l’ensemble des sous-groupes fermés L de G tels que LH = G; montrons que l’ensemble $\mathfrak{M}$, ordonné par la relation $\supset$, est inductif. En effet, si $\mathfrak{S}$ est une partie totalement ordonnée de $\mathfrak{M}$, alors, pour tout $x \in G$, l’ensemble des $xH \cap L$ pour $L \in \mathfrak{S}$ est une base de filtre composée d’ensembles fermés dans l’espace compact $xH$; l’intersection de ces ensembles est donc non vide, ce qui prouve que l’intersection des sous-groupes $L \in \mathfrak{S}$ appartient encore à $\mathfrak{M}$. Appliquant le th. de Zorn, on voit donc qu’il existe dans $\mathfrak{M}$ un élément minimal $L_0$. Comme H est compact, $G/H = L_0H/H$ est isomorphe à $L_0/(L_0 \cap H)$ (III, p. 28, cor. 3); comme $L_0$ est totalement discontinu et $L_0 \cap H$ compact, on voit qu’on peut remplacer G par $L_0$; autrement dit, on peut supposer en outre qu’il n’existe aucun sous-groupe fermé $L \neq G$ tel que LH = G.

Or, soit F l’intersection des voisinages à la fois ouverts et fermés de e dans G; montrons que F est un sous-groupe fermé de G. En effet, comme il est évident que F est fermé, il suffit de montrer que $F^{-1}.F \subset F$. Mais si $x \in F$ et si V est un voisinage ouvert et fermé de e dans G, il en est de même de $xV$: sans quoi, e appartiendrait au complémentaire W de $xV$ dans G, qui est encore ouvert et fermé, et on aurait $x \notin W$, donc par définition $x \notin F$ contrairement à l’hypothèse. On en conclut que $xF$, intersection des $xV$ pour les voisinages ouverts et fermés V de e, contient F, autrement dit $x^{-1}F \subset F$, ce qui prouve notre assertion. Puisque G est totalement discontinu et non réduit à e, on a $F \neq G$. Mais si V est un voisinage à la fois ouvert et fermé de e dans G, VH est aussi à la fois ouvert et fermé dans G (III, p. 28, cor. 1), donc $\varphi(V)$ est à la fois ouvert et fermé dans $G/H$, ce qui implique $\varphi(V) = G/H$ en vertu de l’hypothèse. On va en conclure que $FH = G$, ce qui impliquera contradiction, et démontrera donc le lemme. En effet, pour tout $x \in G$, $xH$ rencontre tout voisinage $V$ de $e$ à la fois ouvert et fermé, donc aussi l’intersection $F$ de ces voisinages, puisque les ensembles $V \cap xH$ forment une base de filtre composée d’ensembles fermés dans l’espace compact $xH$.

#### Remarque {#top-iii-s7-n2-rem-1 .statement}

Si le sous-groupe $H_\alpha$ est compact pour un $\alpha \in I$, alors $H_\beta$ est compact pour $\beta \geq \alpha$, puisque c’est un sous-groupe fermé de $H_\alpha$. Comme l’ensemble des $\beta \in I$ tels que $\beta \geq \alpha$ est cofinal à $I$, il revient essentiellement au même, pour l’étude du groupe $G$, de supposer un des $H_\alpha$ compact ou tous les $H_\alpha$ compacts.

### 3. Application aux limites projectives

#### Proposition 5 {#top-iii-s7-prop-5 .statement}

Soit $(G_\alpha, f_{\alpha\beta})$ un système projectif de groupes topologiques séparés, tel que les $f_{\alpha\beta}$ soient des morphismes stricts surjectifs, de noyaux compacts. Alors, pour tout $\alpha \in I$, l’application canonique $f_\alpha$ de $G = \lim_{\leftarrow} G_\alpha$ dans $G_\alpha$ est un morphisme strict surjectif, de noyau compact.

Le fait que $f_\alpha$ soit surjectif et de noyau compact est conséquence de I, p. 64, cor. 1. Reste à voir que $f_\alpha$ est un morphisme strict. Désignons par $e$ (resp. $e_\alpha$) l’élément neutre de $G$ (resp. $G_\alpha$). Tout voisinage $V$ de $e$ dans $G$ contient un ensemble de la forme $f_\beta^{-1}(V_\beta)$, où $V_\beta$ est un voisinage de $e_\beta$ dans $G_\beta$, et où l’on peut supposer $\beta \geq \alpha$; comme $f_{\alpha\beta}$ est un morphisme strict surjectif, $f_{\alpha\beta}(V_\beta)$ est un voisinage de $e_\alpha$ dans $G_\alpha$, et comme $f_\beta$ est surjectif, on a $V_\beta \subset f_\beta(V)$, d’où

$$
f_\alpha(V) = f_{\alpha\beta}(f_\beta(V)) \supset f_{\alpha\beta}(V_\beta),
$$

ce qui prouve que $f_\alpha(V)$ est un voisinage de $e_\alpha$ dans $G_\alpha$.

Si $H_\alpha = f_\alpha^{-1}(e_\alpha)$, les sous-groupes distingués compacts $H_\alpha$ de $G$ vérifient évidemment la condition (AP) de III, p. 60 et $G_\alpha$ s’identifie à $G/H_\alpha$. En particulier les prop. 3 (III, p. 62) et 4 (III, p. 62) s’appliquent à $G$ et aux $H_\alpha$.

#### Corollaire 1 {#top-iii-s7-prop-5-cor-1 .statement}

Soient $(G_\alpha, f_{\beta\alpha})$ un système projectif de groupes topologiques vérifiant les hypothèses de la prop. 5, $(G'_\alpha, f'_{\alpha\beta})$ un système projectif de groupes topologiques, et pour chaque $\alpha$, soit $u_\alpha : G_\alpha \to G'_\alpha$ un morphisme strict surjectif, de noyau compact, les $u_\alpha$ formant un système projectif d’applications. Alors $u = \lim_{\leftarrow} u_\alpha$ est un morphisme strict de $G = \lim_{\leftarrow} G_\alpha$ sur $G' = \lim_{\leftarrow} G'_\alpha$, de noyau compact.

Soit $N_\alpha$ le noyau de $u_\alpha$; $L_\alpha = f_\alpha^{-1}(N_\alpha)$ est alors le noyau du morphisme strict surjectif $v_\alpha = u_\alpha \circ f_\alpha : G \to G'_\alpha$; comme $L_\alpha / H_\alpha$ est isomorphe à $N_\alpha$ (III, p. 14, prop. 20), $L_\alpha$ est un sous-groupe distingué compact de $G$ (III, p. 28, cor. 2). Le noyau $L$ de $u$ est l’intersection des $L_\alpha$; désignons par $\varphi$ l’application canonique

G → G/L; on peut écrire $v_\alpha = w_\alpha \circ \varphi$, où $w_\alpha$ est un morphisme strict de $G/L$ sur $G'_\alpha$, de noyau $L_\alpha / L$. Comme l’intersection des $L_\alpha / L$ est l’élément neutre de $G/L$ et que les $L_\alpha / L$ forment une base de filtre et sont compacts, cette base de filtre converge vers l’élément neutre de $G/L$ (I, p. 60, corollaire). La prop. 2 de III, p. 60 montre alors que $w = \lim_{\leftarrow} w_\alpha$ est un isomorphisme de $G/L$ sur $G'$; on en conclut que $w \circ \varphi$ est un morphisme strict de $G$ sur $G'$, de noyau $L$; mais il est clair que $u = w \circ \varphi$, ce qui démontre le corollaire.

#### Corollaire 2 {#top-iii-s7-prop-5-cor-2 .statement}

Soit $(G_\alpha, f_{\alpha\beta})$ un système projectif de groupes topologiques vérifiant les conditions de la prop. 5, et soit $G'$ un groupe topologique dans lequel il existe un voisinage $V'$ de l’élément neutre $e'$ ne contenant aucun sous-groupe de $G'$ distinct de $\{e'\}$. Alors, pour tout homomorphisme continu $v : G \to G'$, il existe un indice $\alpha \in I$ et un homomorphisme continu $v_\alpha : G_\alpha \to G'$ tels que $v = v_\alpha \circ f_\alpha$.

En effet, comme $v(V')$ est un voisinage de $e$ dans $G$, il existe un indice $\alpha$ et un voisinage $V_\alpha$ de $e_\alpha$ dans $G_\alpha$ tels que $f_\alpha^{-1}(V_\alpha) \subset v^{-1}(V')$. On a donc $v(H_\alpha) \subset V'$, et comme $v(H_\alpha)$ est un sous-groupe de $G'$, $v(H_\alpha) = \{e'\}$. Comme $f_\alpha$ s’identifie à l’application canonique $G \to G/H_\alpha$, le corollaire résulte de la factorisation canonique d’un homomorphisme continu (III, p. 16).

Exercises

## EXERCICES {#top-iii-s7-exercises}

See the [exercises for § 7](exercises/s7/).
