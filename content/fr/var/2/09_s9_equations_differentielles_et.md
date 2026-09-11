---
book: var
book_title: Variétés différentielles et analytiques
chapter: "2"
chapter_title: VARIÉTÉS DIFFÉRENTIELLES ET ANALYTIQUES, FASCICULE DE RÉSULTATS
section: 9
section_title: Equations différentielles et feuilletages
lang: fr
source: var-fr
pdf_pages: 0116-0125
extraction: ocr
subsections:
    - "no": 1
      title: Courbes intégrales
      page: 0
      pdf_page: 116
    - "no": 2
      title: Feuilletages
      page: 0
      pdf_page: 119
    - "no": 3
      title: Sous-fibrés intégrables
      page: 0
      pdf_page: 121
    - "no": 4
      title: Fibrés intégrables en caractéristique p ≠ 0
      page: 0
      pdf_page: 124
statements: 2
exercises: 0
content_sha256: a65d2285e0ec3b5e8e51427bcedc796fffee8d546e725662827c97e254fda4a1
---

## § 9. Equations différentielles et feuilletages

Dans les n$^{\mathrm{os}}$ 9.1, 9.2 et 9.3, on suppose K de caractéristique 0. Dans le n$^\circ$ 9.4, on suppose K de caractéristique $p \ne 0$.

### 9.1. Courbes intégrales

Dans ce n$^\circ$, X désigne une variété de classe $C^r$ et $\xi$ un champ de vecteurs de classe $C^s$ sur X, avec $r$, $s$ dans $\mathbf{N}_K$, $s \leq r - 1$.

9.1.1. Soit I un ouvert de K, et soit $f : I \to X$ une application de classe $C^k$ ($k \in \mathbf{N}_K$, $k \leq r$) de I dans X. Pour $t \in I$, on note $f'(t)$ le vecteur $T_t(f)(1) \in T_{f(t)}(X)$; ce vecteur est parfois appelé vitesse de $f$ à l’instant $t$. Lorsque X est un espace de Banach, $f'(t)$ est la dérivée de $f$ en $t$.

On dit que $f$ est une courbe intégrale de $\xi$ si l’on a

$$(1)\qquad f'(t)=\xi(f(t))$$

pour tout $t \in I$. Une telle courbe est de classe $C^{s+1}$.

Si $x$ est un point de X, on appelle courbe intégrale de $\xi$ d’origine $x$ une courbe intégrale $f : I \to X$ de $\xi$ telle que $0 \in I$ et $f(0)=x$; pour tout $x \in X$, il existe une courbe intégrale de $\xi$ d’origine $x$, définie dans un voisinage ouvert convenable de 0 dans K.

Si $f : I \to X$ est une courbe intégrale de $\xi$ et si $a \in K$, l’application $t \mapsto f(t-a)$ de $I+a$ dans X est une courbe intégrale de $\xi$.

Soient $f_1 : I_1 \to X$ et $f_2 : I_2 \to X$ deux courbes intégrales de $\xi$, et $t \in I_1 \cap I_2$. Si $f_1(t)=f_2(t)$, les applications $f_1$ et $f_2$ coïncident dans un voisinage de $t$.

9.1.2 (« Flots »). Soit W un ouvert de $X \times K$. Pour tout $x \in X$, notons $W_x$ l’ensemble des $t \in K$ tels que $(x,t) \in W$. On appelle flot intégral de $\xi$ de domaine W une application $f$ de classe $C^k$ ($k \leq r$) de W dans X telle que, pour tout $x \in X$, l’application $f_x : W_x \to X$ définie par $f_x(t)=f(x,t)$ soit une courbe intégrale de $\xi$, et que pour $(x,0) \in W$ on ait $f(x,0)=x$.

Pour tout point $x \in X$, il existe un flot intégral de $\xi$ de classe $C^s$ dont le domaine est un voisinage de $(x,0)$ dans $X \times K$. Deux flots intégralux de $\xi$ définis au voisinage de $(x,0)$ coïncident sur un voisinage de $(x,0)$.

Soit $x \in X$ et soit $f$ un flot intégral de $\xi$ dont le domaine W est un voisinage de (x, 0). Il existe un voisinage V de (x, 0, 0) dans X × K × K tel que, si (x, t_1, t_2) ∈ V, on ait
$$(x, t_1) \in W,\quad (f(x, t_1), t_2) \in W,\quad (x, t_1 + t_2) \in W$$
et
(2)
$$f(f(x, t_1), t_2) = f(x, t_1 + t_2).$$
Si X est paracompacte, ou si X est séparée et K = R ou C, il existe un flot intégral de $\xi$ dont le domaine est un voisinage de X × {0}.

9.1.3 (« Le cas réel »). On suppose que K = R et que X est séparée. On appelle *arc intégral* de $\xi$ toute courbe intégrale de $\xi$ dont le domaine est un intervalle ouvert de R. Deux arcs intégraux $f_1$ et $f_2$ de $\xi$, définis dans des intervalles $I_1$ et $I_2$, et coïncidant en un point de $I_1 \cap I_2$, coïncident dans $I_1 \cap I_2$.

Pour tout point $x \in X$, il existe un arc intégral d’origine x et un seul $f_x : I_x \to X$ tel que, pour tout arc intégral $f : I \to X$ d’origine x, on ait $I \subset I_x$ et $f = f_x|I$. L’arc $f_x$ est appelé *l’arc intégral maximal* de $\xi$ d’origine x, et son domaine $I_x$ est parfois appelé *l’intervalle de vie* du point x pour le champ $\xi$.

Si $I_x = ] -a_-, a_+ [$ et si $a_+$ est fini, la restriction de $f_x$ à l’intervalle $[0, a_+ [$ est une application propre de $[0, a_+ [$ dans X. En particulier, $f(t)$ n’a pas de limite lorsque t tend vers $a_+$.

9.1.4. Avec les notations et les hypothèses de 9.1.3, l’ensemble $\Omega$ des couples $(x, t) \in X \times \mathbf{R}$ tels que $t \in I_x$ est ouvert dans $X \times \mathbf{R}$ et l’application $f : \Omega \to X$ définie par $f(x, t) = f_x(t)$ est de classe $C^s$; c’est un flot intégral de $\xi$ de domaine $\Omega$.

Les fonctions $\alpha_+$ et $\alpha_- : X \to ]0, +\infty]$ définies par $I_x = ] -\alpha_-(x), \alpha_+(x)[$ sont semi-continues inférieurement. Pour $(x, t) \in \Omega$ et $y = f(x, t)$, on a $\alpha_+(y) = \alpha_+(x) - t$ et $\alpha_-(y) = \alpha_-(x) + t$.

Si $t_1 \in I_x$ et si $t_2 \in I_{f(x, t_1)}$, on a $t_1 + t_2 \in I_x$ et
(3)
$$f(f(x, t_1), t_2) = f(x, t_1 + t_2).$$

Si la fonction $\alpha_+$ (resp. $\alpha_-$) est minorée sur X par une constante > 0, elle est constante et égale à $+\infty$.

On a $\alpha_+ = \alpha_- = +\infty$ (autrement dit, on a $\Omega = X \times \mathbf{R}$) dans chacun des cas suivants:

(i) le champ $\xi$ est à support compact (par exemple si X est compacte);
(ii) il existe un groupe d’automorphismes de X, transitif, et préservant $\xi$;
*(iii) il existe sur X une structure riemannienne pour laquelle X soit complète et $\xi$ borné.*

Si $\Omega = X \times \mathbf{R}$, l’application $f : X \times \mathbf{R} \to X$ est une loi d’opération à droite de classe $C^s$ de la variété de groupe $\mathbf{R}$ dans la variété X, cf. 5.12.5.

9.1.5 (« Le cas complexe »). On suppose que K = C et que X est séparée. Pour tout $a \in ]0, +\infty]$, notons $D_a$ le disque ouvert de centre 0 et de rayon a dans C. Pour tout $x \in X$, il existe un nombre $\rho(x) \in ]0, +\infty]$ et un seul, une courbe intégrale $f_x : D_{\rho(x)} \to X$ d’origine $x$ et une seule telle que, pour tout $a \in ]0, +\infty]$ et toute courbe intégrale $f : D_a \to X$ d’origine $x$, on ait $a \leq \rho(x)$ et $f = f_x|D_a$.

Pour tout $\lambda \in \mathbf{C}$, soit $\alpha_\lambda(x)$ la borne supérieure de l’intervalle de vie de $x$ pour le champ de vecteurs $\lambda \xi$ sur la variété réelle déduite de $X$ par restriction des scalaires. On a $\rho(x) = \inf_{|\lambda|=1} \alpha_\lambda(x)$.

L’ensemble $\Delta$ des couples $(x, t) \in X \times \mathbf{C}$ tels que $t \in D_{\rho(x)}$ est ouvert dans $X \times \mathbf{C}$ et l’application $f$ de $\Delta$ dans $X$ définie par $f(x, t) = f_x(t)$ est un flot intégral de $\xi$. La fonction $\rho : X \to ]0, +\infty]$ est semi-continue inférieurement. Pour $(x, t) \in \Delta$ et $y = f(x, t)$, on a $\rho(y) \geq \rho(x) - |t|$. Si $\rho$ est minorée sur $X$ par une constante $> 0$, on a $\rho = +\infty$ et $\Delta = X \times \mathbf{C}$.

Lorsque $\Delta = X \times \mathbf{C}$, l’application $f : X \times \mathbf{C} \to X$ est une loi d’opération à droite de la variété de groupe $\mathbf{C}$ dans la variété $X$.

9.1.6. Soient $\varphi : X \to Y$ un morphisme de variétés et $\eta$ un champ de vecteurs sur $Y$ tels que $\xi$ soit $\varphi$-lié à $\eta$ (cf. 8.2.6). Si $f : I \to X$ est une courbe intégrale de $\xi$, l’application $\varphi \circ f : I \to Y$ est une courbe intégrale de $\eta$. Si $K = \mathbf{R}$ et si $X$ et $Y$ sont séparées, pour tout $x \in X$, l’intervalle de vie de $x$ pour $\xi$ est contenu dans l’intervalle de vie de $\varphi(x)$ pour $\eta$. Si de plus $\varphi$ est propre, ces intervalles sont égaux.

9.1.7 (« Équations dépendant du temps »). Soit $W$ un ouvert de $X \times K$ et soit $\Xi : W \to T(X)$ un relèvement de classe $C^s$ de $\mathrm{pr}_1 : W \to X$, c’est-à-dire une application de classe $C^s$ de $W$ dans $T(X)$ telle que $\Xi(x, t)$ appartienne à $T_x(X)$ pour tout $(x, t) \in W$. On appelle courbe intégrale de $\Xi$ une application $f$ de classe $C^k$ (avec $k \in \mathbf{N}_K$ et $k \leq r$), d’un ouvert $I$ de $K$ dans $X$ telle que, pour tout $t \in I$, on ait

$$
(f(t), t) \in W \text{ et } f'(t) = \Xi(f(t), t).
$$

Soit $\eta$ le champ de vecteurs de classe $C^s$ sur $W$ défini par $\eta(x, t) = (\Xi(x, t), (t, 1))$. Pour qu’une application $f$ d’un ouvert $I$ de $K$ dans $X$ soit une courbe intégrale de $\Xi$, il faut et il suffit que $t \mapsto (f(t), t)$ soit une courbe intégrale de $\eta$ au sens de 9.1.1.

Soient $g : I \to W$ une courbe intégrale de $\eta$ et $t_0$ un point de $I$ tel que $\mathrm{pr}_2(g(t_0)) = t_0$. L’ensemble des éléments $t \in I$ tels que $\mathrm{pr}_2(g(t)) = t$ est un voisinage de $t_0$ qui coïncide avec $I$ si $I$ est connexe.

9.1.8 (« Paramètres et conditions initiales »). Soit $Z$ une variété de classe $C^r$, soit $W$ un ouvert de $X \times K \times Z$, et soit $\Xi$ un relèvement de classe $C^s$ de $\mathrm{pr}_1 : W \to X$ (8.6.1). Si $z \in Z$, on note $W_z$ l’ensemble des $(x, t) \in X \times K$ tels que $(x, t, z) \in W$, et on note $\Xi_z$ l’application $(x, t) \mapsto \Xi(x, t, z)$ de $W_z$ dans $T(X)$.

Soit $(x_0, t_0, z_0)$ un point de $W$. Il existe alors un voisinage ouvert $X_1 \times I_1 \times Z_1$ de $(x_0, t_0, z_0)$ dans $W$ et une application de classe $C^s$

$$
f : X_1 \times I_1 \times I_1 \times Z_1 \to X
$$

tels que, quel que soit $(x_1, t_1, z_1) \in X_1 \times I_1 \times Z_1$, l’application $t \mapsto f(x_1, t_1, t, z_1)$ soit une courbe intégrale de $\Xi_{z_1}$ (au sens de 9.1.7) vérifiant la relation $f(x_1, t_1, t_1, z_1) = x_1$.

Deux applications

$$
f_1 : X_1 \times I_1 \times I_1 \times Z_1 \to X \quad \text{et} \quad f_2 : X_2 \times I_2 \times I_2 \times Z_2 \to X
$$

satisfaisant aux conditions ci-dessus coïncident dans un voisinage de $(x_0, t_0, t_0, z_0)$.

### 9.2. Feuilletages

Dans ce n°, X désigne une variété de classe $C^r$, avec $r \in \mathbf{N}_K$. Sauf mention du contraire, toutes les variétés et tous les morphismes considérés sont supposés de classe $C^r$.

9.2.1. Soit S une variété, et soit $p : X \to S$ une submersion. Pour tout $s \in S$, munissons $X_s = p^{-1}(s)$ de la structure de variété induite par celle de X (5.10.5); l’ensemble X est réunion disjointe des $X_s$. Notons $X_p$ la structure de variété sur X obtenue par recollement des $X_s$, pour $s \in S$ (5.2.4); c’est l’unique structure de variété sur X pour laquelle les $X_s$ soient des sous-variétés ouvertes. L’espace topologique $X_p$ est somme des espaces $X_s$.

Soient V une variété et $f$ une application de V dans X. Pour que $f$ soit un morphisme de V dans $X_p$, il faut et il suffit que $f$ soit un morphisme de V dans X et que $p \circ f$ soit localement constante.

9.2.2. On appelle feuilletage de X une variété Y ayant même ensemble sous-jacent que X et satisfaisant à la condition suivante:

(F) Pour tout $x \in X$, il existe une sous-variété ouverte U de X contenant x, une variété S et une submersion $p : U \to S$ telles que la variété $U_p$ soit une sous-variété ouverte de Y.

On dit aussi que le couple (X, Y) est une variété feuilletée. Si (X, Y) et (X', Y') sont des variétés feuilletées, on appelle morphisme de (X, Y) dans (X', Y') toute application $f : X \to X'$ qui est à la fois un morphisme de la variété X dans la variété X' et un morphisme de la variété Y dans la variété Y'.

Soit (X, Y) une variété feuilletée. L’application identique $Y \to X$ est une immersion bijective. Une partie U de X est appelée une feuille si c’est un ouvert de Y; dans ce cas, on munit U de la structure topologique et de la structure de variété induites par celles de Y; par exemple, on dit que U est une feuille connexe si c’est une partie ouverte et connexe de Y. Les feuilles qui sont des sous-variétés de X forment une base de la topologie de Y. Lorsque $K = \mathbf{R}$ ou $\mathbf{C}$, les composantes connexes de Y sont des feuilles, appelées feuilles connexes maximales de (X, Y).

9.2.3. Si $s \in \mathbf{N}_K, s \leq r$, on appelle feuilletage de classe $C^s$ de X un feuilletage de la variété de classe $C^s$ sous-jacente à X.

9.2.4. Exemples

a) La variété X est un feuilletage de X, appelé le feuilletage grossier de X.

b) Si $p : X \to S$ est une submersion, $X_p$ est un feuilletage de X, appelé le feuilletage de X défini par p. Le feuilletage de X défini par l’application identique est l’ensemble X muni de sa structure de variété pure de dimension 0 (5.2.1); on l’appelle le feuilletage discret de X.

c) Soient E un espace de Banach, F un sous-espace vectoriel fermé de E admettant un supplémentaire topologique, et $p$ la projection canonique $E \to E/F$. Le feuilletage $E_p$ de E est appelé le feuilletage de E défini par F.

d) Soit $\Gamma$ un groupe discret opérant proprement et librement sur l’espace topologique $X$ (TG, III, § 4, n° 4). Soit $Y$ un feuilletage de $X$, et supposons que, pour tout $s \in \Gamma$, l’application $x \mapsto sx$ soit un automorphisme de $(X, Y)$. La relation d’équivalence sur $X$ (resp. $Y$) dont les classes sont les orbites de $\Gamma$ est régulière (5.9.5). Si l’on note $X/\Gamma$ (resp. $Y/\Gamma$) la variété quotient correspondante, le couple $(X/\Gamma, Y/\Gamma)$ est une variété feuilletée, dite quotient de $(X, Y)$ par $\Gamma$.

9.2.5. Soient $Y$ un feuilletage de $X$ et $U$ un ouvert de $X$. Alors $U$ est ouvert dans $Y$ et $U$, muni de la structure de variété induite par celle de $Y$, est un feuilletage de $X$, appelé le feuilletage induit par $Y$.

Plus généralement, soit $f : X' \to X$ un morphisme tel que $f$ et l’application identique $Y \to X$ forment un couple transversal (5.11.1). Le produit fibré $Y' = X' \times_X Y$ s’identifie canoniquement à un feuilletage de $X'$ appelé le feuilletage image réciproque de $Y$ par $f$.

9.2.6. Soient $p : X \to S$ et $p' : X' \to S'$ deux submersions, et soit $f$ un morphisme de $X$ dans $X'$. Pour que $f$ soit un morphisme de $X_p$ dans $X_{p'}$, il faut et il suffit que, pour tout $x \in X$, il existe un voisinage ouvert $U$ de $x$ dans $X$ et un morphisme $g$ de $p(U)$ dans $S'$ tel que $g \circ p = p' \circ f$ sur $U$.

9.2.7. Soit $Y$ un feuilletage de $X$. On appelle carte feuilletante de $(X, Y)$ un quadruplet $(U, \varphi, E, F)$ tel que $(U, \varphi, E)$ soit une carte de $X$, que $F$ soit un sous-espace vectoriel fermé de l’espace de Banach $E$ admettant un supplémentaire topologique et que $\varphi$ soit un isomorphisme du feuilletage de $U$ induit par $Y$ sur le feuilletage de $\varphi(U)$ défini par l’application canonique de $E$ sur $E/F$. Pour tout point $x \in X$, il existe une carte feuilletante $(U, \varphi, E, F)$ de $(X, Y)$ telle que $x \in U$. Soit $n = \dim_x X$ et soit $m = \dim_x Y$. Si $n$ est fini, il existe un voisinage ouvert $U$ de $x$ et un système de coordonnées $\zeta^1, \ldots, \zeta^n$ de $X$ sur $U$ tel que le feuilletage de $U$ induit par $Y$ coïncide avec le feuilletage défini par l’application $(\zeta^{m+1}, \ldots, \zeta^n)$ de $U$ dans $K^{n-m}$.

9.2.8. Soit $Y$ un feuilletage de $X$. Lorsque $x$ parcourt $X$, les espaces $T_x(Y)$ sont les fibres d’un sous-fibré vectoriel de classe $C^{r-1}$ de $T(X)$ que l’on appelle le sous-fibré de $T(X)$ tangent au feuilletage $Y$ et que l’on note $T(X, Y)$. Si le feuilletage $Y$ est défini par une submersion $p : X \to S$, alors $T(X, Y) = \mathrm{Ker}\, T(p)$ est le fibré tangent relatif $T(X/S)$ de $X$ sur $S$ (8.1.3).

Soient $(X, Y)$ et $(X', Y')$ deux variétés feuilletées, et soit $f$ un morphisme de $X$ dans $X'$. Pour que $f$ soit un morphisme de variétés feuilletées, il faut et il suffit que $T(f)$ applique $T(X, Y)$ dans $T(X', Y')$. En particulier, soit $f : Z \to X$ un morphisme de variétés ; pour que $f$ soit un morphisme de $Z$ dans $Y$, il faut et il suffit que $T(f)$ applique $T(Z)$ dans $T(X, Y)$. Pour qu’une sous-variété $Z$ de $X$ soit une feuille de $(X, Y)$, il faut et il suffit que l’on ait

$$
T_z(Z) = T_z(X, Y) \quad \text{pour tout } z \in Z.
$$

Soit $Y$ un feuilletage de $X$ et soit $U$ une feuille de $Y$, admettant une base dénombrable d’ouverts. Soient $Z$ une variété et $f$ une application de $Z$ dans $U$. Pour que $f$ soit un morphisme de variétés de Z dans U, il faut et il suffit que le composé de f et de l’injection canonique de U dans X soit un morphisme de variétés de Z dans X. Si X est localement compact et dénombrable à l’infini, toute feuille connexe de (X, Y) admet une base dénombrable d’ouverts (cf. TG, I, 3e éd., §11, n° 7, cor. 2 du th. 1).

9.2.9. Supposons que K = R ou C. Soit Y un feuilletage de X. Les conditions suivantes sont équivalentes:

a) Il existe une variété S et une submersion $p : X \to S$ telles que $Y = X_p$.

b) Pour tout $x \in X$, il existe une sous-variété $S_x$ de X possédant les deux propriétés suivantes:
   b₁) L’espace tangent $T_x(S_x)$ à $S_x$ en $x$ est un supplémentaire topologique de $T_x(X, Y)$ dans $T_x(X)$.
   b₂) Toute feuille connexe de (X, Y) rencontre $S_x$ en au plus un point.

Supposons ces conditions vérifiées et soit $R \{x, y\}$ la relation sur X « x et y appartiennent à une même feuille connexe »; alors R est une relation d’équivalence régulière (5.9.5) sur X, et, si p désigne la projection canonique $X \to X/R$, on a $Y = X_p$.

#### Exemple {#var-2-s9-n2-exa-1 .statement}

Prenons $K = R$ et $X = R^2$. Faisons opérer le groupe discret $\Gamma = Z^2$ sur X par translations. Soit $m \in R$ et soit $(X, Y_m)$ le feuilletage défini par la submersion $p : (x_1, x_2) \mapsto x_2 - mx_1$ de X sur R. Posons $X' = X/\Gamma$ et $Y'_m = Y_m/\Gamma$; alors $Y'_m$ est un feuilletage du tore $X'$ (cf. 9.2.4, exemple d)). Si m est rationnel, il existe une submersion $p'$ de $X'$ sur $R/Z$ telle que $Y'_m = X'_{p'}$. Si m est irrationnel, toute feuille connexe maximale de $(X', Y'_m)$ est dense dans $X'$, et il n’existe pas de submersion $p'$ de $X'$ dans une variété S telle que $Y'_m = X'_{p'}$.

9.2.10. Soit Y un feuilletage de X, et soit $\pi : X \to S$ un morphisme de variétés tel que le composé $Y \to X \xrightarrow{\pi} S$ soit étale. Si S’ est un ouvert de S, une section $\sigma : S' \to X$ de $\pi$ au-dessus de S’ est dite horizontale (par rapport au feuilletage Y) si c’est un morphisme de S’ dans Y ; il revient au même de dire que $\sigma(S')$ est une feuille de (X, Y), ou encore que $T(\sigma)$ applique $T(S')$ dans $T(X, Y)$. Pour tout $s_0 \in S$ et pour tout $x_0 \in \pi^{-1}(s_0)$, il existe une section horizontale définie au voisinage de $s_0$ et prenant la valeur $x_0$ en $s_0$; deux telles sections coïncident sur un voisinage de $s_0$.

Plus généralement, soit $s_0 \in S$, soit T une variété, soit f un morphisme de T dans la sous-variété $\pi^{-1}(s_0)$ de X, et soit $t_0 \in T$. Il existe alors un voisinage ouvert T’ (resp. S’) de $t_0$ dans T (resp. de $s_0$ dans S), et un morphisme
$$
F : S' \times T' \to X
$$
vérifiant la condition suivante: pour tout $t \in T'$, l’application $s \mapsto F(s, t)$ est une section horizontale de $\pi$ au-dessus de S’ prenant la valeur $f(t)$ au point $s_0$. Deux telles applications F coïncident sur un voisinage de $(s_0, t_0)$.

### 9.3. Sous-fibrés intégrables

Dans ce n°, X désigne une variété de classe $C^r$ et F un sous-fibré vectoriel de classe $C^s$ de $T(X)$, avec $r, s$ dans $N_K, s \leq r - 1$.

9.3.1. Soit V une variété de classe $C^k$ ($k \in \mathbf{N}_K, k \leq r$) et soit $f$ un morphisme de classe $C^k$ de V dans X. On dit que $f$ est une intégrale de F si $T(f)$ applique $T(V)$ dans F.

Une sous-variété Z de classe $C^k$ de X est appelée une sous-variété intégrale de F si l’injection $Z \to X$ est une intégrale de F au sens ci-dessus, i.e. si l’on a $T_x(Z) \subset F_x$ pour tout $x \in Z$.

Soit $x \in X$. Si $Z_1$ et $Z_2$ sont deux sous-variétés intégrales de X contenant $x$ et si $T_x(Z_1) = F_x$, il existe un voisinage U de $x$ tel que $U \cap Z_2 \subset Z_1$. Si en outre $T_x(Z_2) = F_x$, les germes de $Z_1$ et $Z_2$ en $x$ coïncident.

9.3.2. On dit que F est intégrable s’il existe un feuilletage Y de X de classe $C^s$ tel que $F = T(X, Y)$ (9.2.8). Un tel feuilletage est alors unique; on l’appelle le feuilletage intégral de F. Pour qu’un morphisme $f : V \to X$ de classe $C^s$ soit une intégrale de F, il faut et il suffit que $f$ soit un morphisme de V dans Y.

#### Exemple {#var-2-s9-n3-exa-1 .statement}

Si F est de rang 1 en tout point, F est intégrable, et définit sur X un feuilletage pur de dimension 1. Supposons en outre que $K = \mathbf{R}$, que X soit séparée, et que F admette pour repère un champ de vecteurs $\xi$ partout non nul. Alors, pour tout $x \in X$, la feuille connexe maximale contenant $x$ est l’image de l’arc intégral maximal de $\xi$ d’origine $x$ (9.1.3).

9.3.3 (« Critères d’intégrabilité »). Les conditions suivantes sont équivalentes:

(i) Le sous-fibré vectoriel F de $T(X)$ est intégrable.

(ii) Pout tout $x \in X$, il existe une sous-variété intégrale Z de classe $C^s$ de F telle que $x \in Z$ et $T_x(Z) = F_x$.

(iii) Quels que soient l’ouvert U de X et les champs de vecteurs $\xi$ et $\eta$ appartenant à $\mathscr{J}_F^s(U)$ (7.4.1), on a $[\xi, \eta] \in \mathscr{J}_F^{s-1}(U)$.

Soit $(\xi_i)_{i \in I}$ une famille de sections de F de classe $C^s$ telle que, pour tout $x \in X$, l’ensemble des $\xi_i(x)$ soit un sous-ensemble total de l’espace de Banach $F_x$ (EVT, I, § 2, n° 1). Les conditions (i), (ii), (iii) sont alors équivalentes à:

(iv) pour tout couple $(i, j)$ d’éléments de I, et tout $x \in X$, on a $[\xi_i, \xi_j](x) \in F_x$.

Lorsque I est fini, et que la famille $(\xi_i)$ est un repère de F, les conditions précédentes équivalent encore à:

(v) il existe une famille $(c_{ij}^k)_{(i, j, k) \in I \times I \times I}$ de fonctions sur X à valeurs dans K telles que $[\xi_i, \xi_j] = \sum_k c_{ij}^k \xi_k$ quels que soient $i, j$ dans I.

(Si tel est le cas, les fonctions $c_{i,j}^k$ sont de classe $C^{s-1}$.)

9.3.4. Soit $s' \in \mathbf{N}_K$, avec $s' \leq s$, et soit $F'$ le fibré vectoriel de classe $C^{s'}$ déduit de F par affaiblissement de structure (8.7.1). Pour que F soit intégrable, il faut et il suffit que $F'$ le soit. Dans ce cas, le feuilletage intégral de $F'$ se déduit de celui de F par affaiblissement de structure.

9.3.5. Soient E un espace de Banach et $p$ un entier $\geq 0$. Pour tout $x \in X$, notons

N(p, E)_x le sous-espace vectoriel de Alt^p(T_x(X); E) formé des éléments u tels que $u(v_1, \ldots, v_p) = 0$ pour $v_1, \ldots, v_p$ dans $F_x$. Les espaces N(p, E)_x, pour $x \in X$, sont les fibres d’un sous-fibré vectoriel de classe C^s de Alt^p(T(X); E). Notons-le N(p, E). Si F est intégrable, on a:

(vi) pour tout ouvert U de X et toute forme $\omega \in \mathscr{S}_{N(p, E)}^s(U)$, on a $d\omega \in \mathscr{S}_{N(p+1, E)}^{s-1}(U)$.

Inversement, si (vi) est vérifiée pour $p = 1$ et pour tout espace de Banach E, le fibré F est intégrable; lorsque K = R ou C, il suffit même de vérifier (vi) pour $p = 1$ et E = K.

Supposons que le dual de T(X)/F admette un repère $(\omega_1, \ldots, \omega_n)$. L’intégrabilité de F est alors équivalente à la condition suivante:

(vii) $d\omega_i \wedge \omega_1 \wedge \cdots \wedge \omega_n = 0$ pour $1 \leq i \leq n$.

S’il existe en outre un sous-fibré vectoriel G de classe C^s de T(X) tel que T(X) soit somme directe de F et de G, la condition (vii) équivaut à:

(viii) il existe des formes différentielles $\alpha_i^j$ (i, j dans I) de degré 1 sur X, de classe C^{s-1}, telles que $d\omega_i = \sum_j \alpha_i^j \wedge \omega_j$ pour tout $i \in I$.

9.3.6. Soit L un espace de Banach et soit $\omega$ une forme différentielle de degré 1 sur X à valeurs dans L, de classe C^s. On fait les deux hypothèses suivantes:

a) pour tout $x \in X$, $\omega_x$ est un homomorphisme surjectif de $T_x(X)$ dans L, et le noyau de $\omega_x$ est $F_x$;
b) il existe un sous-fibré vectoriel G de T(X) tel que T(X) soit somme directe de F et de G.

L’intégrabilité de F est alors équivalente à:

(ix) il existe une forme différentielle $\alpha$ de degré 1 sur X à valeurs dans End(L) telle que $d\omega = \alpha \wedge \omega$, le produit extérieur étant défini par l’accouplement canonique End(L) $\times$ L $\to$ L (7.8.2 et 8.3.2).

9.3.7 (« Équations aux différentielles totales »). On suppose que X est le produit de deux variétés A et B de classe C^r; on note $p_1 : X \to A$ et $p_2 : X \to B$ les deux projections. Soit f un morphisme de classe C^s de $p_1^*T(A)$ dans $p_2^*T(B)$. Les graphes des applications $f_{(a, b)} : T_a(A) \to T_b(B)$ sont les fibres d’un sous-fibré vectoriel de classe C^s de T(X); notons-le F^f.

Soit A’ un ouvert de A, et soit $\varphi : A' \to B$ un morphisme de classe C^k ($k \in \mathbf{N}_K, k \leq r$). On dit que $\varphi$ est une intégrale de f si, pour tout $a \in A'$, on a $T_a(\varphi) = f_{a, \varphi(a)}$; cela équivaut à dire que l’application $a \mapsto (a, \varphi(a))$ de A’ dans X est une intégrale de F^f (9.3.1). Une telle application est de classe C^{s+1}. Si $\varphi_1$ et $\varphi_2$ sont deux intégrales de f et prennent la même valeur en un point $a \in A$, elles coïncident dans un voisinage de a.

Plus généralement, soit Z une variété de classe C^k, soit A’ un ouvert de A, soit $a \in A'$ et soient $\Phi_1, \Phi_2$ des morphismes de classe C^k de Z $\times$ A’ dans B. Supposons que

Φ₁ et Φ₂ coïncident sur Z × {a} et que, pour tout z ∈ Z, les morphismes
$$
a \mapsto \Phi_1(z, a) \quad \text{et} \quad a \mapsto \Phi_2(z, a)
$$
soient des intégrales de f. Alors Φ₁ et Φ₂ coïncident dans un voisinage de Z × {a}.

Supposons que F^f soit intégrable. Soient Z une variété de classe C^k (k ∈ N_K, k ≤ s), (z₀, a₀) un point de Z × A, et ρ un morphisme de classe C^k de Z dans B. Il existe un voisinage ouvert Z' × A' de (z₀, a₀) dans Z × A et un morphisme Φ : Z' × A' → B de classe C^k tels que, pour tout z ∈ Z', l’application a ↦ Φ(z, a) de A' dans B admette f pour application tangente et prenne la valeur ρ(z) au point a₀.

9.3.8. Conservons les hypothèses et notations de 9.3.7 et supposons que A (resp. B) soit une sous-variété ouverte d’un espace de Banach E (resp. M). L’application f s’identifie alors à un morphisme de classe C^s de X = A × B dans l’espace de Banach $\mathscr{L}(E; M)$. Notons D₁f (resp. D₂f) la première (resp. seconde) dérivée partielle de f (1.6.2); c’est un morphisme de classe C^{s-1} de X dans $\mathscr{L}(E; \mathscr{L}(E; M))$ (resp. dans $\mathscr{L}(M; \mathscr{L}(E; M))$), espace que l’on identifie de façon évidente à $\mathscr{L}_2(E; M)$ (resp. à $\mathscr{L}(M, E; M)$). Pour que F soit intégrable, il faut et il suffit que, pour tout x ∈ X, l’application bilinéaire
$$
\Delta_x : (h_1, h_2) \mapsto D_1f(x)(h_1, h_2) + D_2f(x)(f(x)h_1, h_2)
$$
de E × E dans M soit symétrique. Sous cette condition, si φ est une intégrale de f définie dans un ouvert A' de A, la dérivée seconde de φ en un point a de A' est $\Delta_{(a, \varphi(a))}$.

Si E = K^n, et si l’on note (x¹, ..., xⁿ) les fonctions coordonnées sur K^n, l’application f est définie par une famille (f₁, ..., fₙ) d’applications de A × B dans M, et la condition d’intégrabilité s’écrit:
$$
\frac{\partial f_i}{\partial x^j} + (D_2f_i) \cdot f_j = \frac{\partial f_j}{\partial x^i} + (D_2f_j) \cdot f_i
$$
quels que soient les entiers i, j dans {1, n}. Une application φ d’un ouvert A' de A dans B est une intégrale de f si et seulement si l’on a
$$
\frac{\partial \varphi}{\partial x^i} = f_i(x, \varphi(x)) \quad \text{pour tout } x \in A' \text{ et tout } i \in \{1, n\},
$$
autrement dit, si l’on a
$$
d\varphi = \sum_{1 \leq i \leq n} f_i(x, \varphi(x)) \, dx^i.
$$

### 9.4. Fibrés intégrables en caractéristique p ≠ 0

Dans ce n°, on suppose K de caractéristique p ≠ 0. On note X une variété K-analytique localement de dimension finie.

9.4.1 (« Puissances p-ièmes »). Soit ξ un champ de vecteurs sur un ouvert U de X. Il existe un champ de vecteurs ξ^p et un seul sur U tel que l’on ait
$$
D_{\xi^p}(f) = (D_\xi)^p(f) = \underbrace{D_\xi(D_\xi(\ldots(D_\xi(f))\ldots))}_{p \text{ fois}}
$$
pour toute fonction analytique f définie dans un ouvert de U.

Si $\varphi$ est une fonction analytique sur $U$, on a
$$
(\varphi \xi)^p = \varphi^p \xi^p + (\mathrm{D}_{\varphi \xi})^{p-1}(\varphi) \cdot \xi
$$
et si $\eta$ est un champ de vecteurs sur $U$, on a
$$
[\xi^p, \eta] = \mathrm{ad}(\xi)^p(\eta) = [\xi, [\xi, \ldots, [\xi, \eta]\ldots]].
$$

9.4.2 (« Identité de Jacobson »). Soit $L$ la $F_p$-algèbre de Lie libre (LIE, II, § 2, n° 2) sur un ensemble $\{x, y\}$ à deux éléments. Il existe un élément et un seul $\Lambda_p(x, y)$ de $L$ tel que l’on ait
$$
(x + y)^p = x^p + y^p + \Lambda_p(x, y)
$$
dans l’algèbre enveloppante de $L$. Exemples:
$$
\Lambda_2(x, y) = [x, y]; \quad \Lambda_3(x, y) = [x, [x, y]] - [y, [x, y]].
$$
Si $\xi$ et $\eta$ sont des champs de vecteurs sur $X$, on a
$$
(\xi + \eta)^p = \xi^p + \eta^p + \Lambda_p(\xi, \eta).
$$

9.4.3. *Exemple.* — Prenons $X = K$ (resp. $K^*$) et notons $x$ l’application canonique $X \to K$. Soit $\xi$ (resp. $\eta$) le champ de vecteurs $\partial / \partial x$ (resp. $x \cdot \partial / \partial x$); il est invariant par les translations du groupe additif (resp. multiplicatif) $X$. On a
$$
\xi^p = 0 \quad \text{et} \quad \eta^p = \eta.
$$

9.4.4 (« Fibrés intégrables »). Soit $F$ un sous-fibré vectoriel de $T(X)$. On dit que $F$ est *intégrable* si, pour tout $x \in X$, il existe un système de coordonnées $(\zeta^1, \ldots, \zeta^n)$ de $X$ en $x$ et un entier $m \leq n$ tels que $(\partial / \partial \zeta^1, \ldots, \partial / \partial \zeta^m)$ soit un repère de $F$ au voisinage de $x$.
Pour que $F$ soit intégrable, il faut et suffit qu’il vérifie la condition suivante:
*Pour tout ouvert $U$ de $X$, $\mathscr{S}_F^\omega(U)$ est une sous-algèbre de Lie de $\mathscr{S}_{T(X)}^\omega(U)$ stable par l’opération $\xi \mapsto \xi^p$.*
