---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: GROUPES DE LIE
section: 3
section_title: Passage d’un groupe de Lie à son algèbre de Lie
lang: fr
source: lie-ii-iii-fr
pdf_pages: 0123-0164, 0256-0259
extraction: ocr
subsections:
    - "no": 1
      title: Convolution des distributions ponctuelles sur un groupe de Lie
      page: 0
      pdf_page: 123
    - "no": 2
      title: Propriétés fonctorielles
      page: 0
      pdf_page: 125
    - "no": 3
      title: Cas d’un groupe opérant dans une variété
      page: 0
      pdf_page: 128
    - "no": 4
      title: Convolution des distributions ponctuelles et des fonctions
      page: 0
      pdf_page: 129
    - "no": 5
      title: Champs de distributions ponctuelles définis par l’action d’un groupe sur une variété
      page: 0
      pdf_page: 133
    - "no": 6
      title: Champs invariants de distributions ponctuelles sur un groupe de Lie
      page: 0
      pdf_page: 134
    - "no": 7
      title: Algèbre de Lie d’un groupe de Lie
      page: 0
      pdf_page: 136
    - "no": 8
      title: Propriétés fonctorielles de l’algèbre de Lie
      page: 0
      pdf_page: 139
    - "no": 9
      title: Algèbre de Lie du groupe des éléments inversibles d’une algèbre
      page: 0
      pdf_page: 141
    - "no": 10
      title: Algèbres de Lie de certains groupes linéaires
      page: 0
      pdf_page: 142
    - "no": 11
      title: Représentations linéaires
      page: 0
      pdf_page: 145
    - "no": 12
      title: Représentation adjointe
      page: 0
      pdf_page: 149
    - "no": 13
      title: Tenseurs et formes invariantes
      page: 0
      pdf_page: 153
    - "no": 14
      title: Formules de Maurer-Cartan
      page: 0
      pdf_page: 154
    - "no": 15
      title: Construction de formes différentielles invariantes
      page: 0
      pdf_page: 156
    - "no": 16
      title: Mesure de Haar sur un groupe de Lie
      page: 0
      pdf_page: 157
    - "no": 17
      title: Différentielle gauche
      page: 0
      pdf_page: 160
    - "no": 18
      title: Algèbre de Lie d’un groupuscule de Lie
      page: 0
      pdf_page: 161
statements: 111
exercises: 9
content_sha256: 10d475925bba6f8447e2caa7f660b8bf6a0a4cf578ab88234d2012cde55fecbe
---

## § 3. Passage d’un groupe de Lie à son algèbre de Lie

### 1. Convolution des distributions ponctuelles sur un groupe de Lie

#### Définition 1 {#lie-iii-s3-def-1 .statement}

Soient G un groupe de Lie, g et g' deux points de G, et soient t ∈ T^{(∞)}_g(G), t' ∈ T^{(∞)}_{g'}(G) deux distributions ponctuelles en g et g' sur G (VAR, R, 13.2.1). On appelle produit de convolution de t et t', et on note t \* t', l’image de t ⊗ t' par l’application (h, h') ↦ hh' de G × G dans G (VAR, R, 13.2.3).

#### Proposition 1 {#lie-iii-s3-prop-1 .statement}

(i) Si t ∈ T^{(s)}_g(G) et t' ∈ T^{(s')}_{g'}(G), on a t \* t' ∈ T^{(s + s')}_{gg'}(G).
(ii) Si t ou t' est sans terme constant, t \* t' est sans terme constant.
(iii) ε_g \* ε_{g'} = ε_{gg'}.
(iv) Soient t ∈ T^{(s)}_g(G), t' ∈ T^{(s')}_{g'}(G), et f une fonction de classe C^{s + s'} dans un voisinage ouvert de gg', à valeurs dans un espace polynormé séparé. On a
$$
\langle t * t', f \rangle = \langle t', h' \mapsto \langle t, h \mapsto f(hh') \rangle \rangle \\
= \langle t, h \mapsto \langle t', h' \mapsto f(hh') \rangle \rangle.
$$
Cela résulte de VAR, R, 13.4.1, 13.2.3 et 13.4.4.

Supposons K = R ou C, et G de dimension finie. Alors G est localement compact. Si t, t' sont des mesures ponctuelles, la définition de t \* t' concorde avec celle de INT, VIII, § 1. Nous verrons plus tard comment le produit de convolution des mesures et celui des distributions ponctuelles sont deux cas particuliers du produit de convolution de distributions non nécessairement ponctuelles.

Soit $\mathcal{T}^{(\infty)}(G)$ la somme directe des $T^{(\infty)}_g(G)$ pour $g \in G$ (cf. VAR, R, 13.6.1). On définit le produit de convolution dans $\mathcal{T}^{(\infty)}(G)$ comme l’application bilinéaire de $\mathcal{T}^{(\infty)}(G) \times \mathcal{T}^{(\infty)}(G)$ dans $\mathcal{T}^{(\infty)}(G)$ prolongeant le produit de convolution de la déf. 1. On le note encore *. Ainsi, $\mathcal{T}^{(\infty)}(G)$ est muni d’une structure d’algèbre, filtrée par les $\mathcal{T}^{(s)}(G)$. La sous-algèbre $\mathcal{T}^{(0)}(G) = \bigoplus_{g \in G} T^{(0)}_g(G)$ s’identifie à l’algèbre $K^{(G)}$ du groupe G sur K.

#### Proposition 2 {#lie-iii-s3-prop-2 .statement}

L’algèbre $\mathcal{T}^{(\infty)}(G)$ est associative. Elle est commutative si et seulement si G est commutatif.

Soient $t \in \mathcal{T}^{(\infty)}(G), t' \in \mathcal{T}^{(\infty)}(G), t'' \in \mathcal{T}^{(\infty)}(G)$. Alors $t * (t' * t'')$ est l’image de $t \otimes t' \otimes t''$ par l’application $(g, g', g'') \mapsto g(g'g'')$ de $G \times G \times G$ dans G, et $(t * t') * t''$ est l’image de $t \otimes t' \otimes t''$ par l’application $(g, g', g'') \mapsto (gg')g''$ de $G \times G \times G$ dans G. Donc $(t * t') * t'' = t * (t' * t'')$. On voit de même que, si G est commutatif, $t * t' = t' * t$. Si le produit de convolution est commutatif, G est commutatif d’après la prop. 1 (iii).

#### Proposition 3 {#lie-iii-s3-prop-3 .statement}

Si $t \in \mathcal{T}^{(\infty)}(G)$ et $g \in G$, on a $\gamma(g)_* t = \varepsilon_g * t, \delta(g)_* t = t * \varepsilon_{g^{-1}}, (\mathrm{Int}\, g)_* t = \varepsilon_g * t * \varepsilon_{g^{-1}}$. En particulier, $\varepsilon_e$ est élément unité de $\mathcal{T}^{(\infty)}(G)$.

Considérons le diagramme

$$
G \xrightarrow{\varphi} G \times G \xrightarrow{\psi} G
$$

où $\varphi$ est l’application $h \mapsto (g, h)$ et où $\psi$ est l’application $(h', h) \mapsto h'h$. On a $\gamma(g) = \psi \circ \varphi$, donc $\gamma(g)*t = \psi_*(\varphi_*(t))$. Or $\varphi_*(t) = \varepsilon_g \otimes t$, donc $\psi_*(\varphi_*(t)) = \varepsilon_g * t$. On raisonne de même pour $\delta(g)*t$. Enfin, $\mathrm{Int}\, g = \gamma(g) \circ \delta(g)$, donc $(\mathrm{Int}\, g)_* = \gamma(g)_* \circ \delta(g)_*$.

On voit donc que, pour $t \in T(G)$, $\varepsilon_g * t$ et $t * \varepsilon_g$ sont égaux à $gt$ et $tg$ calculés dans le groupe $T(G)$ (§ 2, n° 2). On prendra garde que, pour $t, t'$ dans $T(G)$, le produit $tt'$ au sens du § 2 est en général distinct de $t * t'$.

#### Définition 2 {#lie-iii-s3-def-2 .statement}

Soit $G$ un groupe de Lie. La sous-algèbre de $\mathcal{T}^{(\infty)}(G)$ formée des distributions à support contenu dans $\{e\}$ se note $U(G)$.

Cette algèbre est filtrée par les sous-espaces

$$
U_s(G) = U(G) \cap \mathcal{T}^{(s)}(G) = T_e^{(s)}(G).
$$

On pose $U^+(G) = T_e^{(\infty)+}(G)$, $U_s^+(G) = U^+(G) \cap U_s(G)$ (cf. VAR, R, 13.2.1). Rappelons que $U_0(G)$ s’identifie à $K$, et $U_1^+(G)$ à l’espace tangent $T_e(G)$. Dans $U(G)$, $U^+(G)$ est un idéal bilatère supplémentaire de $U_0(G)$.

#### Exemple {#lie-iii-s3-n1-exa-1 .statement}

Soit $E$ un espace normable complet, considéré comme groupe de Lie. Alors l’espace vectoriel $U(E)$ s’identifie canoniquement à l’espace vectoriel $TS(E)$ (VAR, R, 13.2.4). Soit $m : E \times E \to E$ l’addition dans $E$. Alors

$$
m_* : TS(E \times E) \to TS(E)
$$

est égal à $TS(m)$ (VAR, R, 13.2.4). Pour $t, t'$ dans $U(E) = TS(E)$, l’image $t * t'$ du produit tensoriel symétrique $t \otimes t'$ par $m_*$ est donc $TS(m)(t \otimes t')$. D’après A, IV, § 5, n° 6, prop. 7, n°elle édition, cette image n’est autre que le produit $tt'$ dans l’algèbre $TS(E)$. Ainsi, l’algèbre $U(E)$ s’identifie à l’algèbre $TS(E)$.

#### Proposition 4 {#lie-iii-s3-prop-4 .statement}

Considérons l’application bilinéaire $(u, v) \mapsto u * v$ (resp. $(u, v) \mapsto v * u$) de $U(G) \times K^{(G)}$ dans $\mathcal{T}^{(\infty)}(G)$. L’application linéaire correspondante de $U(G) \otimes K^{(G)}$ dans $\mathcal{T}^{(\infty)}(G)$ est un isomorphisme d’espaces vectoriels.

En effet, $K^{(G)}$ est somme directe des $K\varepsilon_x$ pour $x \in G$. D’autre part, l’application $u \mapsto u * \varepsilon_g$ (resp. $u \mapsto \varepsilon_g * u$) est un isomorphisme de l’espace vectoriel $U(G) = T_e^{(\infty)}(G)$ sur l’espace vectoriel $T_g^{(\infty)}(G)$ d’après la prop. 3. Enfin, $\mathcal{T}^{(\infty)}(G)$ est somme directe des $T_g^{(\infty)}(G)$ pour $g \in G$.

C.Q.F.D.

Soient $X$ une variété de classe $C^r$ ($r \geq \infty$) et $x \in X$. On a défini (VAR, R, 13.3.1) une filtration canonique sur l’espace vectoriel $T_x^{(\infty)}(X)$, et un isomorphisme canonique $i_{X,x}$ de l’espace vectoriel gradué associé sur l’espace vectoriel gradué

TS(T_x(X)). En particulier, posons T_e(G) = L; alors i_{G,e} est un isomorphisme de l’espace vectoriel gradué gr U(G) sur l’espace vectoriel gradué TS(L). Mais U(G) est une algèbre filtrée, d’où une structure d’algèbre graduée sur gr U(G).

#### Proposition 5 {#lie-iii-s3-prop-5 .statement}

L’isomorphisme $i_{G,e} : \mathrm{gr}\ U(G) \to \mathrm{TS}(L)$ est un isomorphisme d’algèbres.

Soit $p$ l’application $(t, t') \mapsto t \otimes t'$ de $U(G) \times U(G)$ dans $U(G \times G)$. Soit $c$ l’application $(t, t') \mapsto t * t'$ de $U(G) \times U(G)$ dans $U(G)$. Soit $m$ l’application $(g, g') \mapsto gg'$ de $G \times G$ dans $G$. On a d’après la déf. 1
$$
c = m_* \circ p.
$$
Considérons le diagramme

$$
\begin{array}{ccc}
\mathrm{gr}\ U(G) \times \mathrm{gr}\ U(G) & \xrightarrow{\mathrm{gr}(p)} & \mathrm{gr}\ U(G \times G) \xrightarrow{\mathrm{gr}(m_*)} \mathrm{gr}\ U(G) \\
\downarrow i_{G,e} \times i_{G,e} & & \downarrow i_{G \times G,e} \\
\mathrm{TS}(L) \times \mathrm{TS}(L) & \xrightarrow{q} & \mathrm{TS}(L \times L) \xrightarrow{\mathrm{TS}(T(m))} \mathrm{TS}(L)
\end{array}
$$

où $q$ est l’application déduite de l’isomorphisme canonique de $\mathrm{TS}(L) \otimes \mathrm{TS}(L)$ sur $\mathrm{TS}(L \times L)$. D’après VAR, R, 13.4.6 et 13.3.5, les deux carrés du diagramme sont commutatifs. Donc, compte tenu de (1), le diagramme

$$
\begin{array}{ccc}
\mathrm{gr}\ U(G) \times \mathrm{gr}\ U(G) & \xrightarrow{\mathrm{gr}(c)} & \mathrm{gr}\ U(G) \\
\downarrow i_{G,e} \times i_{G,e} & & \downarrow i_{G,e} \\
\mathrm{TS}(L) \times \mathrm{TS}(L) & \xrightarrow{\mathrm{TS}(T(m)) \circ q} & \mathrm{TS}(L)
\end{array}
$$

est commutatif. Or $T(m) : L \times L \to L$ transforme $(x, y)$ en $x + y$ (§ 2, n° 1, prop. 2 (ii)). D’après A, IV, § 5, n° 6, prop. 7, n^{elle} édition, $\mathrm{TS}(T(m)) \circ q$ est donc la multiplication de l’algèbre $\mathrm{TS}(L)$.

### 2. Propriétés fonctorielles

#### Proposition 6 {#lie-iii-s3-prop-6 .statement}

Soient $G, H$ des groupes de Lie, $\varphi$ un morphisme de $G$ dans $H$. Pour $t, t'$ dans $\mathcal{T}^{(\infty)}(G)$, on a $\varphi_*(t * t') = \varphi_*(t) * \varphi_*(t')$.

Considérons le diagramme

$$
\begin{array}{ccc}
G \times G & \xrightarrow{m} & G \\
\downarrow \varphi \times \varphi & & \downarrow \varphi \\
H \times H & \xrightarrow{n} & H
\end{array}
$$

où $m(g, g') = gg'$, $n(h, h') = hh'$. Ce diagramme est commutatif. Donc
$$
\varphi_*(t * t') = \varphi_*(m_*(t \otimes t')) = n_*((\varphi \times \varphi)_*(t \otimes t'))
= n_*(\varphi_*(t) \otimes \varphi_*(t')) = \varphi_*(t) * \varphi_*(t').
$$

Les groupes de Lie G et $G^\vee$ ont la même variété sous-jacente, donc les espaces vectoriels $\mathcal{T}^{(\infty)}(G)$ et $\mathcal{T}^{(\infty)}(G^\vee)$ sont les mêmes. Soit $\theta$ l’application $g \mapsto g^{-1}$, qui est un isomorphisme du groupe de Lie G sur le groupe de Lie $G^\vee$. Alors $\theta_*$ est un automorphisme de l’espace vectoriel $\mathcal{T}^{(\infty)}(G)$, automorphisme qu’on note $t \mapsto t^\vee$. On a $(\varepsilon_g)^\vee = \varepsilon_{g^{-1}}$. Si $t \in T_e(G)$, on a
$$
t^\vee = -t \quad (§ 2, \text{prop. } 2).
$$

#### Exemple {#lie-iii-s3-n2-exa-1 .statement}

Supposons que G soit le groupe de Lie défini par un espace normable complet E. Alors U(G) s’identifie à TS(E) et la restriction de $\theta_*$ à U(G) s’identifie à TS(T_e(\theta)) (VAR, R, 13.2.4). Par suite, si $t \in TS^s(E)$, on a $t^\vee = (-1)^s t$.

#### Proposition 7 {#lie-iii-s3-prop-7 .statement}

*Soit G un groupe de Lie. Soient t, t' dans $\mathcal{T}^{(\infty)}(G)$.*
(i) *Le produit t \* t' calculé relativement à $G^\vee$ est égal au produit t' \* t calculé relativement à G.*
(ii) *On a $(t * t')^\vee = {t'}^\vee * t^\vee$.*
Considérons le diagramme

$$
\begin{array}{ccc}
G \times G & \xrightarrow{s} & G \times G \\
& \searrow^n & \swarrow^m \\
& & G
\end{array}
$$

où $s(g, g') = (g', g)$, $m(g, g') = gg'$, $n(g, g') = g'g$ quels que soient $g, g'$ dans G. Ce diagramme est commutatif. Donc $n_*(t \otimes t') = m_*(s_*(t \otimes t')) = m_*(t' \otimes t)$. Cette égalité n’est autre que (i). L’assertion (ii) résulte de (i) et de la prop. 6.

#### Proposition 8 {#lie-iii-s3-prop-8 .statement}

*Soient G, H des groupes de Lie, $\varphi$ un morphisme de G dans H. Si $t \in \mathcal{T}^{(\infty)}(G)$, on a $\varphi_*(t^\vee) = (\varphi_*(t))^\vee$.*
Soit $\theta$ (resp. $\theta'$) l’application $g \mapsto g^{-1}$ de G dans G (resp. de H dans H). On a $\varphi \circ \theta = \theta' \circ \varphi$, d’où $\varphi_*(\theta_*(t)) = \theta'_*(\varphi_*(t))$.

#### Proposition 9 {#lie-iii-s3-prop-9 .statement}

*Soient $G_1, \ldots, G_n$ des groupes de Lie, et $G = G_1 \times \cdots \times G_n$. Si l’on identifie canoniquement les espaces vectoriels $\mathcal{T}^{(\infty)}(G)$ et $\mathcal{T}^{(\infty)}(G_1) \otimes \cdots \otimes \mathcal{T}^{(\infty)}(G_n)$, l’algèbre $\mathcal{T}^{(\infty)}(G)$ est produit tensoriel des algèbres $\mathcal{T}^{(\infty)}(G_1), \ldots, \mathcal{T}^{(\infty)}(G_n)$. Si $t_i \in \mathcal{T}^{(\infty)}(G_i)$ pour $i = 1, \ldots, n$, on a
$$
(t_1 \otimes \cdots \otimes t_n)^{\vee} = t_1^{\vee} \otimes \cdots \otimes t_n^{\vee}.
$$
Il suffit d’envisager le cas où $n = 2$. Soient $t_1, t_1'$ dans $\mathcal{T}^{(\infty)}(G_1)$, $t_2, t_2'$ dans $\mathcal{T}^{(\infty)}(G_2)$. Il s’agit de montrer que $(t_1 \otimes t_2) * (t_1' \otimes t_2') = (t_1 * t_1') \otimes (t_2 * t_2')$, et que $(t_1 \otimes t_2)^{\vee} = t_1^{\vee} \otimes t_2^{\vee}$. Considérons le diagramme

$$
\begin{array}{ccc}
(G_1 \times G_2) \times (G_1 \times G_2) & \xrightarrow{m} & G_1 \times G_2 \\
& \searrow^n & \nearrow^{p_1 \times p_2} \\
& & (G_1 \times G_1) \times (G_2 \times G_2)
\end{array}
$$

où $m((x_1, x_2), (x_1', x_2')) = (x_1 x_1', x_2 x_2')$, $n((x_1, x_2), (x_1', x_2')) = ((x_1, x_1'), (x_2, x_2'))$, $p_1(x_1, x_1') = x_1 x_1'$, $p_2(x_2, x_2') = x_2 x_2'$. Ce diagramme est commutatif. Donc
$$
m_*((t_1 \otimes t_2) \otimes (t_1' \otimes t_2')) = (p_1 \times p_2)_*(n_*((t_1 \otimes t_2) \otimes (t_1' \otimes t_2'))),
$$
c’est-à-dire
$$
\begin{align*}
(t_1 \otimes t_2) * (t_1' \otimes t_2') &= (p_1 \times p_2)_*((t_1 \otimes t_1') \otimes (t_2 \otimes t_2')) \\
&= p_1*(t_1 \otimes t_1') \otimes p_2*(t_2 \otimes t_2') \\
&= (t_1 * t_1') \otimes (t_2 * t_2').
\end{align*}
$$
On voit de façon analogue que $(t_1 \otimes t_2)^{\vee} = t_1^{\vee} \otimes t_2^{\vee}$.

#### Proposition 10 {#lie-iii-s3-prop-10 .statement}

Soient $H$ un sous-groupe de Lie de $G$, et $i : H \to G$ l’injection canonique. Alors $i_*$ est un homomorphisme injectif de l’algèbre $\mathcal{T}^{(\infty)}(H)$ dans l’algèbre $\mathcal{T}^{(\infty)}(G)$, et $i_*((t^{\vee})) = (i_*(t))^{\vee}$ pour tout $t \in \mathcal{T}^{(\infty)}(H)$.
Cela résulte des prop. 6, 8 et de VAR, R, 13.2.3.

On identifie $\mathcal{T}^{(\infty)}(H)$ à une sous-algèbre de $\mathcal{T}^{(\infty)}(G)$ grâce à l’isomorphisme de la prop. 10.

#### Remarque {#lie-iii-s3-n2-rem-1 .statement}

La prop. 10 reste valable si $H$ est un quasi-sous-groupe de Lie.

Rappelons (VAR, R, 13.5.1) que, si $V$ est une variété analytique sur $K$, $\mathcal{T}^{(\infty)}(V)$ est munie canoniquement d’une structure de cogèbre sur $K$, à coïunité; la coïunité est l’application linéaire de $\mathcal{T}^{(\infty)}(G)$ dans $K$ qui associe, à tout élément de $T_x^{(\infty)}(V)$, son terme constant.

#### Proposition 11 {#lie-iii-s3-prop-11 .statement}

Soit $G$ un groupe de Lie.
(i) La cogèbre $\mathcal{T}^{(\infty)}(G)$, munie de la convolution, est une bigèbre (A, III, p. 149).

(ii) Soit c le coproduit dans $\mathcal{T}^{(\infty)}(G)$. Soit $t \in \mathcal{T}^{(\infty)}(G)$, et posons $c(t) = \sum_{i=1}^n t_i \otimes t'_i$.
Alors $c(t^\vee) = \sum_{i=1}^n t_i^\vee \otimes t_{i'}^\vee$.

Prouvons (i). Dans la définition citée des bigèbres, la condition 1° résulte des prop. 2 et 3, la condition 2° résulte de VAR, R, 13.5.1. Soit d l’application $g \mapsto (g, g)$ de G dans $G \times G$. On a $c = d_*$, donc c est un morphisme d’algèbres (prop. 6 et 9), ce qui est la condition 3°. Soient $t \in T_g^{(\infty)}(G)$, $t' \in T_{g'}^{(\infty)}(G)$, sans termes constants et $\lambda, \lambda'$ dans K; alors $\varepsilon_g \otimes tt', t \otimes \varepsilon_{g'}, t \otimes t'$ sont sans termes constants (VAR, R, 13.4.1), donc le terme constant de $(\lambda \varepsilon_g + t) * (\lambda' \varepsilon_{g'} + t')$ est $\lambda \lambda'$; donc la condition 4° est vérifiée.

Prouvons (ii). D’après les prop. 8 et 9, on a
$$
c(t^\vee) = d_*(t^\vee) = (d_*(t))^\vee = \left( \sum_{i=1}^n t_i \otimes t_i' \right)^\vee = \sum_{i=1}^n t_i^\vee \otimes t_{i'}^\vee.
$$

#### Proposition 12 {#lie-iii-s3-prop-12 .statement}

Soient G, H deux groupes de Lie, $\varphi$ un morphisme de G dans H. Alors $\varphi_*$ est un morphisme de bigèbres de $\mathcal{T}^{(\infty)}(G)$ dans $\mathcal{T}^{(\infty)}(H)$.
Cela résulte de la prop. 6 et de VAR, R, 13.5.1.

Soit G un groupe de Lie. La restriction de la convolution et du coproduit à U(G) définissent sur U(G) une structure de bigèbre. On a $U(G)^\vee = U(G)$. Si $\varphi : G \to H$ est un morphisme de groupes de Lie, on note U($\varphi$) l’application $t \mapsto \varphi_*(t)$ de U(G) dans U(H); c’est un morphisme de bigèbres. Si $\psi : H \to L$ est un autre morphisme de groupes de Lie, on a $U(\psi \circ \varphi) = U(\psi) \circ U(\varphi)$. Si $\varphi$ est une immersion (resp. submersion), U($\varphi$) est injectif (resp. surjectif) d’après VAR, R, 13.2.3. En particulier, si H est un sous-groupe de Lie de G, U(H) s’identifie à une sous-algèbre de U(G), le coproduit de U(H) étant la restriction du coproduit de U(G). Si H est ouvert dans G, on a $U(H) = U(G)$. Si $G_1, G_2$ sont des groupes de Lie, $U(G_1 \times G_2)$ s’identifie à $U(G_1) \otimes U(G_2)$. Les éléments primitifs de U(G) sont ceux de $T_e(G)$ (VAR, R, 13.5.3).

Soit à nouveau $\varphi : G \to H$ un morphisme de groupes de Lie. Si l’on identifie gr U(G) à TS(T_e(G)) et gr U(H) à TS(T_e(H)), alors gr U($\varphi$) s’identifie à TS(T_e($\varphi$)) (VAR, R, 13.3.5). Appliquons cela à l’isomorphisme $g \mapsto g^{-1}$ de G sur $G^\vee$; alors $T_e(\varphi) = -1$, donc
$$
t \in U_s(G) \Rightarrow t^\vee \equiv (-1)^s t \mod. U_{s-1}(G).
$$

### 3. Cas d’un groupe opérant dans une variété

Soient G un groupe de Lie, X une variété de classe $C^r$, et f une loi d’opération à gauche de classe $C^r$ de G dans X. Si $t \in T_g^{(s)}(G)$ et $u \in T_x^{(s')}(X)$, et si $s + s' \leq r$, on note $t * u$ l’image de $t \otimes u$ par $f_*$. On prolonge le produit \* en une application bilinéaire, notée encore *, de $\mathcal{T}^{(s)}(G) \times \mathcal{T}^{(s')}(X)$ dans $\mathcal{T}^{(s+s')}(X)$. La prop. 1 du n° 1 s’étend, avec des modifications évidentes, à la présente situation.

Lorsqu’on fait opérer G à gauche dans lui-même par translations, on retrouve la déf. 1 du n° 1.

#### Proposition 13 {#lie-iii-s3-prop-13 .statement}

*Soient* $t \in \mathcal{T}^{(s)}(G)$, $t' \in \mathcal{T}^{(s')}(G)$, $u \in \mathcal{T}^{(s'')}(X)$, *tels que* $s + s' + s'' \leq r$. *On a* $(t * t') * u = t * (t' * u)$.

Cela se démontre comme la prop. 2 du n° 1.

En particulier, si $r \geq \infty$, l’espace vectoriel $\mathcal{T}^{(\infty)}(X)$ est un module à gauche sur l’algèbre $\mathcal{T}^{(\infty)}(G)$ pour le produit *.

#### Proposition 14 {#lie-iii-s3-prop-14 .statement}

(i) *Soient* $g_0 \in G$, et $\tau(g_0)$ l’application $x \mapsto f(g_0, x)$ de X dans X. *Si* $u \in \mathcal{T}^{(r)}(X)$, *on a* $\tau(g_0)*u = \varepsilon_{g_0}*u$.

(ii) *Soient* $x_0 \in X$, et $\rho(x_0)$ l’application $g \mapsto f(g, x_0)$ de G dans X. *Si* $t \in T^{(r)}(G)$, *on a* $\rho(x_0)*t = t * \varepsilon_{x_0}$.

Cela se démontre comme la prop. 3 du n° 1.

En particulier, si $u \in T(X)$ et $t \in T(G)$, $\varepsilon_{g_0}*u$ et $t * \varepsilon_{x_0}$ sont égaux aux produits $g_0u, tx_0$ définis au § 2, n° 2.

#### Proposition 15 {#lie-iii-s3-prop-15 .statement}

*Soient* G (resp. $G'$) *un groupe de Lie*, X (resp. $X'$) *une variété de classe* $C^r$. *On suppose donnée une loi d’opération à gauche de classe* $C^r$ *de G (resp. G’) dans X (resp. X’).* *Soient* $\varphi$ *un morphisme de G dans G’*, $\psi$ *un* $\varphi$-*morphisme de X dans X’*. *Soient* $t \in \mathcal{T}^{(s)}(G)$, $u \in \mathcal{T}^{(s')}(X)$, *tels que* $s + s' \leq r$. *Alors* $\psi_*(t * u) = \varphi_*(t) * \psi_*(u)$.

Cela se démontre comme la prop. 6 du n° 2.

#### Remarque {#lie-iii-s3-n3-rem-1 .statement}

Soit $f$ une loi d’opération à droite de classe $C^r$ de G dans X. Si $t \in \mathcal{T}^{(s)}(G)$ et $u \in \mathcal{T}^{(s')}(X)$, avec $s + s' \leq r$, on note $u * t$ l’image de $u \otimes t$ par $f_*$.
Les prop. 13, 14, 15 se transposent de manière évidente à cette situation.

#### Proposition 16 {#lie-iii-s3-prop-16 .statement}

*Soient* G, $G'$ *des groupes de Lie*, X *une variété de classe* $C^r$, *et supposons que* G (resp. $G'$) *opère à gauche (resp. à droite) dans X, avec* $(gx)g' = g(xg')$ *quels que soient* $x \in X$, $g \in G$, $g' \in G$. *Soient* $t \in \mathcal{T}^{(s)}(G)$, $t' \in \mathcal{T}^{(s')}(G')$, $t'' \in \mathcal{T}^{(s'')}(X)$ *avec* $s + s' + s'' \leq r$. *Alors*
$$
(t * t'') * t' = t * (t'' * t').
$$
En effet, $(t * t'') * t'$ (resp. $t * (t'' * t')$) est l’image de $t \otimes t'' \otimes t'$ par l’application $(g, x, g') \mapsto (gx)g'$ (resp. $g(xg')$) de $G \times X \times G'$ dans X.

### 4. Convolution des distributions ponctuelles et des fonctions

Soient G un groupe de Lie, X une variété de classe $C^r$, et $(g, x) \mapsto gx$ une loi d’opération à gauche de classe $C^r$ de G dans X. Pour tout $x \in X$, notons $\rho(x)$ l’application orbitale de x.

#### Définition 3 {#lie-iii-s3-def-3 .statement}

Soit $t \in \mathcal{T}^{(s)}(G)$ avec $s \leq r$. Soit $f : X \to F$ une fonction de classe $C^r$ à valeurs dans un espace polynormé séparé (par exemple $F = K$). On appelle convolée de $t$ et $f$, et l’on note $t * f$, la fonction sur $X$ à valeurs dans $F$ définie par
$$
(t * f)(x) = \langle t^\vee * \varepsilon_x, f \rangle.
$$
On a
$$
\begin{align*}
(t * f)(x) &= \langle \rho(x) * (t^\vee), f \rangle \quad (\text{n}^o 3, \text{prop. 14 (ii)}) \\
&= \langle t^\vee, f \circ \rho(x) \rangle \quad (\text{VAR, R, 13.2.3}) \\
&= \langle t, (f \circ \rho(x))^\vee \rangle \quad (\text{VAR, R, 13.2.3}).
\end{align*}
$$
Notons aussi que la déf. 3 s’écrit sous forme plus symétrique
$$
\langle \varepsilon_x, t * f \rangle = \langle t^\vee * \varepsilon_x, f \rangle.
$$
La fonction $(g, x) \mapsto f(gx) = (f \circ \rho(x))(g)$ sur $G \times X$ est de classe $C^r$. D’après VAR, R, 13.4.4, la fonction $x \mapsto \langle t^\vee, f \circ \rho(x) \rangle$ est donc de classe $C^{r-s}$ si $s < \infty$. Autrement dit, si $s < \infty$, $t * f$ est de classe $C^{r-s}$.
Il est clair que $t * f$ dépend linéairement de $t$ et de $f$.
La formule (4) entraîne en particulier, pour $g \in G$,
$$
(\varepsilon_g * f)(x) = f(g^{-1}x)
$$
c’est-à-dire
$$
\varepsilon_g * f = \gamma(g)f.
$$
Supposons $K = \mathbf{R}$ ou $\mathbf{C}$, $G$ et $X$ de dimension finie, et $X$ munie d’une mesure positive invariante par $G$. La définition de $\varepsilon_g * f$ est en accord avec celle de INT, VIII, § 4, n° 1 (cf. formule (2), loc. cit.).

#### Proposition 17 {#lie-iii-s3-prop-17 .statement}

Soient $t \in \mathcal{T}^{(s)}(G)$, $t' \in \mathcal{T}^{(s')}(X)$, et $f : X \to F$ une fonction de classe $C^r$, avec $s + s' \leq r$. On a
$$
\langle t', t * f \rangle = \langle t^\vee * t', f \rangle.
$$
En effet,
$$
\begin{align*}
\langle t', t * f \rangle &= \langle t', x \mapsto \langle t, g \mapsto f(g^{-1}x) \rangle \rangle \quad \text{d’après (4)} \\
&= \langle t \otimes t', (g, x) \mapsto f(g^{-1}x) \rangle \quad (\text{VAR, R, 13.4.4}) \\
&= \langle t^\vee \otimes t', (g, x) \mapsto f(gx) \rangle \quad (\text{VAR, R, 13.2.3}) \\
&= \langle t^\vee * t', f \rangle.
\end{align*}
$$

#### Proposition 18 {#lie-iii-s3-prop-18 .statement}

Soient $t \in \mathcal{T}^{(s)}(G)$, $t' \in \mathcal{T}^{(s')}(G)$, et $f : X \to F$ une fonction de classe $C^r$, tels que $s + s' \leq r$. On a
$$
(t * t') * f = t * (t' * f).
$$

En effet, pour tout $x \in X$, on a
$$
\langle \varepsilon_x, (t * t') * f \rangle = \langle ((t * t')^\vee * \varepsilon_x, f \rangle \quad \text{d'après (5)} \\
= \langle {t'}^\vee * (t^\vee * \varepsilon_x), f \rangle \quad \text{(prop. 2 et 7)} \\
= \langle t^\vee * \varepsilon_x, t' * f \rangle \quad \text{(prop. 17)} \\
= \langle \varepsilon_x, t * (t' * f) \rangle \quad \text{(prop. 17).}
$$
C.Q.F.D

Si $r \geq \infty$, on voit que l’ensemble des fonctions de classe $C^\infty$ sur $X$ à valeurs dans $F$ est un module à gauche sur l’algèbre $\mathcal{T}^{(\infty)}(G)$.

#### Proposition 19 {#lie-iii-s3-prop-19 .statement}

Soit $t \in \mathcal{T}^{(s)}(G)$, avec $s \leq r$. Soit $f$ (resp. $f'$) une fonction de classe $C^r$ sur $X$ à valeurs dans un espace polynormé séparé $F$ (resp. $F'$). Soit $(u, u') \mapsto uu'$ une application bilinéaire continue de $F \times F'$ dans un espace polynormé séparé $F''$, de sorte que $ff'$ est une fonction de classe $C^r$ sur $X$ à valeurs dans $F''$. Soit $\sum_{i=1}^n t_i \otimes t'_i$ l’image de $t$ dans $\mathcal{T}^{(s)}(G) \otimes \mathcal{T}^{(s)}(G)$ par le coproduit. On a
$$
t * (ff') = \sum_{i=1}^n (t_i * f)(t'_i * f').
$$

En effet, soit $x \in X$, et notons toujours $\rho(x)$ l’application orbitale de $x$. On a
$$
\langle \varepsilon_x, t * (ff') \rangle = \langle t', (ff') \circ \rho(x) \rangle \quad \text{d'après (4)} \\
= \langle t', (f \circ \rho(x))(f' \circ \rho(x)) \rangle \\
= \sum_{i=1}^n \langle t'_i, f \circ \rho(x) \rangle \langle t_i^\vee, f' \circ \rho(x) \rangle \quad \text{(VAR, R, 13.5.2)} \\
= \sum_{i=1}^n \langle \varepsilon_x, t_i * f \rangle \langle \varepsilon_x, t'_i * f' \rangle \quad \text{d'après (4).}
$$

#### Remarque 1 {#lie-iii-s3-n4-rem-1 .statement}

Soient $G$ un groupe de Lie, $X$ une variété de classe $C^r$, et $(x, g) \mapsto xg$ une loi d’opération à droite de classe $C^r$ de $G$ dans $X$. Si $t \in \mathcal{T}^{(s)}(G)$ avec $s \leq r$, et $f : X \to F$ est une fonction de classe $C^r$ sur $X$, on note $f * t$ la fonction sur $X$ définie par
$$
\langle \varepsilon_x, f * t \rangle = \langle \varepsilon_x * t^\vee, f \rangle \\
= \langle \rho(x) * (t^\vee), f \rangle \\
= \langle t^\vee, f \circ \rho(x) \rangle \\
= \langle t, (f \circ \rho(x))^\vee \rangle.
$$
En particulier
$$
(f * \varepsilon_g)(x) = f(xg^{-1})
$$

c’est-à-dire

(10) $$ f * \varepsilon_g = \delta(g)^{-1}f. $$

Les prop. 17, 18, 19 deviennent, avec des notations évidentes,

(11) $$ \langle t', f * t \rangle = \langle t' * t^\nu, f \rangle $$

(12) $$ f * (t * t') = (f * t) * t' $$

(13) $$ (ff') * t = \sum_{i=1}^n (f * t_i)(f' * t_i'). $$

#### Proposition 20 {#lie-iii-s3-prop-20 .statement}

*Soient G, G' des groupes de Lie, X une variété de classe C^r, et (g, x) \mapsto gx* (resp. (x, g') \mapsto xg') une loi d’opération à gauche (resp. à droite) de classe C^r de G (resp. G') dans X. Supposons que (gx)g' = g(xg') quels que soient x \in X, g \in G, g' \in G'. Soient t \in \mathcal{T}^{(s)}(G), t' \in \mathcal{T}^{(s')}(G'), et f : X \to F une fonction de classe C^r, tels que s + s' \leq r. Alors*

$$(t * f) * t' = t * (f * t').$$

En effet, pour tout x \in X, on a

$$
\begin{align*}
\langle \varepsilon_x, (t * f) * t' \rangle &= \langle \varepsilon_x * {t'}^\nu, t * f \rangle &\text{d'après (8)} \\
&= \langle {t'}^\nu * (\varepsilon_x * {t'}^\nu), f \rangle &\text{(prop. 17)} \\
&= \langle {t'}^\nu * \varepsilon_x, f * t' \rangle &\text{(prop. 2, et (11))} \\
&= \langle \varepsilon_x, t * (f * t') \rangle &\text{d'après (5).}
\end{align*}
$$

C.Q.F.D.

En particulier, considérons G comme opérant sur lui-même par les translations à gauche et à droite. Si f : G \to F est une fonction de classe C^r sur G, et si t \in \mathcal{T}^{(s)}(G) (avec s \leq r), t \* f et f \* t sont, si s < \infty, des fonctions de classe C^{r-s} sur G. Soit en outre t' \in \mathcal{T}^{(s')}(G), avec s + s' \leq r. Alors

(14) $$ (t * f) * t' = t * (f * t'). $$

En particulier, \mathscr{C}^\infty(G) est un (\mathcal{T}^{(\infty)}(G), \mathcal{T}^{(\infty)}(G))-bimodule. Les formules (5) et (8) admettent comme cas particuliers

(15) $$ \langle t, f \rangle = \langle \varepsilon_e, t^\nu * f \rangle = \langle \varepsilon_e, f * t^\nu \rangle. $$

#### Remarque 2 {#lie-iii-s3-n4-rem-2 .statement}

Soit (g, x) \mapsto gx une loi d’opération à gauche de classe C^r de G dans X. Soient t \in U_s(G) avec s \leq r, \Omega une partie ouverte de X, et f : \Omega \to F une fonction de classe C^r. On peut encore définir t \* f par les formules (4) ou (5); c’est une fonction définie sur \Omega, à valeurs dans F, de classe C^{r-s} si s < \infty. Les résultats de ce n° s’étendent de façon évidente à cette situation.

### 5. Champs de distributions ponctuelles définis par l’action d’un groupe sur une variété

Soit $(g, x) \mapsto \lambda(g, x) = gx$ une loi d’opération à gauche de classe $C^r$ de $G$ dans $X$. Soient $s \leq r$ et $t \in U_s(G)$. Pour tout $x \in X$, on a $t * \varepsilon_x \in T^{(s)}_x(X)$. L’application $x \mapsto t * \varepsilon_x$ s’appelle le champ de distributions ponctuelles défini par $t$ et par l’action de $G$ sur $X$, et se note parfois $D_t^\lambda$ ou simplement $D_t$. Soient $\Omega$ une partie ouverte de $X$ et $F$ un espace polynormé séparé. Si $f : \Omega \to F$ est de classe $C^r$ et si $s \leq r$, la fonction $t^y * f$ sur $\Omega$ se note aussi $D_t f$. On a donc

$$
(D_t f)(x) = \langle t * \varepsilon_x, f \rangle.
$$

Si $s < \infty$, on a $D_t f \in \mathcal{C}^{r-s}(\Omega, F)$ d’après le n° 4. Ainsi, $f \mapsto D_t f$ est une application de $\mathcal{C}^r(\Omega, F)$ dans $\mathcal{C}^{r-s}(\Omega, F)$ (notée souvent $D_t$ par abus de notation).

Si $t \in U_s(G)$, $t' \in U_{s'}(G)$, et $s + s' \leq r$, on a, d’après la prop. 18 du n° 4,

$$
D_{t*t'} f = D_{t'}(D_t f)
$$

donc, avec l’abus de notation signalé ci-dessus,

$$
D_{t*t'} = D_{t'} \circ D_t.
$$

Supposons $G$ et $X$ de dimension finie. L’application $(t, x) \mapsto t \otimes \varepsilon_x$ de $T^{(s)}(G) \times X$ dans le fibré vectoriel $T^{(s)}(G \times X)$ (cf. VAR, R, 13.2.5) est de classe $C^{r-s}$. Donc (VAR, R, 13.2.5), l’application $(t, x) \mapsto t * \varepsilon_x$ de $T^{(s)}(G) \times X$ dans le fibré vectoriel $T^{(s)}(X)$ est de classe $C^{r-s}$. En particulier, $D_t$ est un opérateur différentiel d’ordre $\leq s$ et de classe $C^{r-s}$ au sens de VAR, R, 14.1.6. D’après la formule (16), la fonction $D_t f$ est alors la transformée de $f$ par cet opérateur différentiel (VAR, R, 14.1.4).

Ne supposons plus $G$ et $X$ de dimension finie. Soient $\psi$ un automorphisme de la variété $X$, et $\Delta$ un champ de distributions ponctuelles sur $X$. Conformément aux définitions générales, on appelle transformé de $\Delta$ par $\psi$ le champ de distributions ponctuelles sur $X$ dont la valeur en $\psi(x)$ est $\psi_*(\Delta(x))$; on note $\psi(\Delta)$ cette application. Si $g \in G$, et si $\tau(g)$ désigne l’automorphisme $x \mapsto gx$ de $X$, le transformé de $\Delta$ par $\tau(g)$ s’appelle aussi le transformé de $\Delta$ par $g$.

#### Proposition 21 {#lie-iii-s3-prop-21 .statement}

Soit $\psi$ un automorphisme de $X$ commutant avec les opérations de $G$. Alors $D_t$ est invariant par $\psi$.

En effet, pour tout $x \in X$, on a

$$
\begin{align*}
(\psi(D_t))(\psi(x)) &= \psi_*(D_t(x)) = \psi_*(t * \varepsilon_x) \\
&= t * \psi_*(\varepsilon_x) & (\text{prop. 15}) \\
&= t * \varepsilon_{\psi(x)} = D_t(\psi(x)).
\end{align*}
$$

#### Proposition 22 {#lie-iii-s3-prop-22 .statement}

Si $g \in G$, le transformé de $D_t$ par $g$ est $D_{\varepsilon_g * t * \varepsilon_{g^{-1}}}$.

En effet, la valeur de ce transformé en $gx$ est
$$
\tau(g)_*(D_t(x)) = \tau(g)_*(t * \varepsilon_x)
= \varepsilon_g * (t * \varepsilon_x) \quad \text{(prop. 14 (i))}
= (\varepsilon_g * t * \varepsilon_{g^{-1}}) * \varepsilon_{gx} \quad \text{(prop. 1 et 2)}
= D_{\varepsilon_g * t * \varepsilon_{g^{-1}}}(gx).
$$
C.Q.F.D.

Soit $(x, g) \mapsto \mu(x, g) = xg$ une loi d’opération à droite de classe $C^r$ de $G$ dans $X$. Soient $s \leq r$ et $t \in U_s(G)$. Pour tout $x \in X$, on a $\varepsilon_x * t \in T^{(s)}_x(X)$. L’application $x \mapsto \varepsilon_x * t$ s’appelle le champ de distributions défini par $t$ et par l’action de $G$ sur $X$, et se note parfois $D_t^\mu$ ou simplement $D_t$. Soit $\Omega$ une partie ouverte de $X$. Si $f : \Omega \to F$ est de classe $C^r$, la fonction $f * t'$ se note $D_t f$. On a donc
$$(19)$$
$$(D_t f)(x) = \langle \varepsilon_x * t, f \rangle$$
et, avec des notations évidentes,
$$(20)$$
$$D_{t * t'} f = D_t(D_{t'} f)$$
$$(21)$$
$$D_{t * t'} = D_t \circ D_{t'}.$$
La prop. 21 reste valable. Soit $g \in G$. Le transformé de $D_t$ par $g$ (c’est-à-dire par l’automorphisme $x \mapsto xg$ de $X$) est $D_{\varepsilon_{g^{-1}} * t * \varepsilon_g}$.

### 6. Champs invariants de distributions ponctuelles sur un groupe de Lie

#### Définition 4 {#lie-iii-s3-def-4 .statement}

Soit $G$ un groupe de Lie. Un champ de distributions sur $G$ est dit invariant à gauche (resp. à droite) s’il est invariant par les translations à gauche (resp. à droite) de $G$.

Autrement dit, un champ de distributions $g \mapsto \Delta_g$ sur $G$ est invariant à gauche si
$$\Delta_{gg'} = \gamma(g)_*\Delta_{g'} \quad \text{pour } g, g' \text{ dans } G,$$
ou encore si
$$\Delta_{gg'} = \varepsilon_g * \Delta_{g'} \quad \text{pour } g, g' \text{ dans } G.$$
Il est invariant à droite si
$$\Delta_{gg'} = \delta({g'}^{-1})_*\Delta_g \quad \text{pour } g, g' \text{ dans } G,$$
ou encore si
$$\Delta_{gg'} = \Delta_g * \varepsilon_{g'} \quad \text{pour } g, g' \text{ dans } G.$$

#### Définition 5 {#lie-iii-s3-def-5 .statement}

Soient $G$ un groupe de Lie, et $t \in U(G)$. On note $L_t$ le champ de distributions $g \mapsto \varepsilon_g * t$ sur $G$, et $R_t$ le champ de distributions $g \mapsto t * \varepsilon_g$ sur $G$.

Autrement dit, $L_t$ (resp. $R_t$) est le champ de distributions défini par $t$ et par $G$ opérant à droite (resp. à gauche) dans $G$ grâce à l’application $(g, g') \mapsto gg'$. Soient $\Omega$ une partie ouverte de $G$ et $F$ un espace polynormé séparé ; si $f \in \mathcal{C}^\omega(\Omega, F)$, on a $L_t f = f * t^\nu \in \mathcal{C}^\omega(\Omega, F)$ et $R_t f = t^\nu * f \in \mathcal{C}^\omega(\Omega, F)$ (n° 5). Si $G$ est de dimension finie, les opérateurs différentiels $L_t$ et $R_t$ sont de classe $C^\omega$ (n° 5).

#### Proposition 23 {#lie-iii-s3-prop-23 .statement}

(i) *L’application* $t \mapsto L_t$ (resp. $t \mapsto R_t$) *est un isomorphisme de l’espace vectoriel* $U(G)$ *sur l’espace vectoriel des champs de distributions invariants à gauche* (resp. *à droite*) *sur* $G$.

(ii) *Pour* $t, t'$ *dans* $U(G)$, *on a* $L_{t*t'} = L_t \circ L_{t'}, \ R_{t*t'} = R_{t'} \circ R_t, \ L_t \circ R_{t'} = R_{t'} \circ L_t$ (*avec l’abus de notation du n° 5*).

(iii) *Si* $\theta$ *est l’application* $g \mapsto g^{-1}$ *de* $G$ *sur* $G$, *on a* $\theta(L_t) = R_{t^\nu}$.

(iv) *Si* $t \in U(G)$ *et* $g \in G$, *on a* $(L_t)_g = (R_{\varepsilon_g * t * \varepsilon_{g^{-1}}})_g$.

Dans $G$, toute translation à droite commute à toute translation à gauche. D’après la prop. 21 du n° 5, $L_t$ est donc invariant à gauche. Comme $(L_t)_e = t$, l’application $t \mapsto L_t$ est injective. Soit $\Delta$ un champ de distributions invariant à gauche sur $G$; soit $t = \Delta_e$; alors $\Delta$ et $L_t$ ont même valeur en $e$ et sont invariants à gauche, donc $\Delta = L_t$. Ceci prouve (i) pour $L_t$ et on raisonne de même pour $R_t$. Les formules $L_{t*t'} = L_t \circ L_{t'}, \ R_{t*t'} = R_{t'} \circ R_t$ résultent de (21) et (18). Soient $t \in U_s(G), \ t' \in U_{s'}(G), f \in \mathcal{C}^r(\Omega, F)$, où $\Omega$ est ouvert dans $G$ et où $s + s' \leq r$; on a
$$
L_t R_{t'} f = L_t ({t'}^\nu * f) = ({t'}^\nu * f) * t^\nu \\
= {t'}^\nu * (f * t^\nu) \tag{prop. 20} \\
= R_{t'} L_t f
$$
donc $L_t \circ R_{t'} = R_{t'} \circ L_t$. Comme $\theta$ est un isomorphisme de $G$ sur $G^\nu$, $\theta(L_t)$ est un champ de distributions invariant à droite sur $G$; sa valeur en $e$ est $\theta^*(t) = t^\nu$; donc $\theta(L_t) = R_{t^\nu}$. Enfin, on a
$$
(L_t)_g = \varepsilon_g * t = (\varepsilon_g * t * \varepsilon_{g^{-1}}) * \varepsilon_g = (R_{\varepsilon_g * t * \varepsilon_{g^{-1}}})_g.
$$

#### Remarque 1 {#lie-iii-s3-n6-rem-1 .statement}

C’est l’action de $G$ sur lui-même par translations *à droite* qui définit les champs de distributions invariants *à gauche*.

#### Remarque 2 {#lie-iii-s3-n6-rem-2 .statement}

Supposons $G$ de dimension finie. L’application
$$
(t, g) \mapsto (R_t)_g = t * \varepsilon_g
$$
de $U_s(G) \times G$ dans $T^{(s)}(G)$ est un isomorphisme de fibrés vectoriels analytiques ; en effet, cette application est bijective, linéaire sur chaque fibre, et analytique (n° 5) ; d’autre part, soit $\varphi : T^{(s)}(G) \to U_s(G) \times G$ la bijection réciproque ; si $t \in T_g^{(s)}(G)$, on a $\varphi(t) = (t * \varepsilon_{g^{-1}}, g)$, donc $\varphi$ est analytique. L’isomorphisme $\varphi$ s’appelle la trivialisation droite de $T^{(s)}(G)$. De même, considérons l’application $(t, g) \mapsto (L_t)_g = \varepsilon_g * t$ de $U_s(G) \times G$ dans $T^{(s)}(G)$ ; l’isomorphisme réciproque s’appelle la trivialisation gauche de $T^{(s)}(G)$. Par restriction, on retrouve les trivialisations droite et gauche de $T(G)$ (§ 2, n° 2).

### 7. Algèbre de Lie d’un groupe de Lie

Soit G un groupe de Lie. Dans U(G), comme dans toute algèbre associative, on pose $[t, t'] = t * t' - t' * t$. Comme $T_e(G)$ est l’ensemble des éléments primitifs de $U(G)$, on a $[T_e(G), T_e(G)] \subset T_e(G)$ (chap. II, § 1, n° 2, prop. 4). La restriction du crochet à $T_e(G)$ définit donc sur $T_e(G)$ une structure d’algèbre de Lie.

#### Lemme 1 {#lie-iii-s3-lem-1 .statement}

Soient X et $X'$ des espaces normables complets, $X_0$ un voisinage ouvert de 0 dans X, f une application analytique de $X_0$ dans $X'$ telle que $f(0) = 0$. Soit $f = f_1 + f_2 + f_3 + \cdots$ le développement en série entière de f en 0, où $f_i$ est un polynôme-continu homogène de degré i sur X à valeurs dans $X'$. Soit t un élément de $TS^2(X)$, considéré comme distribution ponctuelle sur X de support contenu dans {0}. Soit $t' = f_*(t) \in TS(X')$. La composante homogène de degré 1 de $t'$ est $\langle f_2, t \rangle$.

Notons $t'_1$ cette composante. On a, pour toute application linéaire continue u de $X'$ dans un espace polynormé,

$$
\begin{align*}
u(t'_1) &= \langle t', u \rangle & \text{parce que } u \text{ est linéaire continue} \\
&= \langle t, u \circ f \rangle & (\text{VAR, R, 13.2.3}) \\
&= \langle t, u \circ f_2 \rangle & \text{parce que } t \in TS^2(X) \\
&= u(\langle t, f_2 \rangle) & (\text{VAR, R, 13.2.2})
\end{align*}
$$

d’où le lemme.

#### Proposition 24 {#lie-iii-s3-prop-24 .statement}

Soient G un groupe de Lie, $(U, \varphi, E)$ une carte de G telle que $\varphi(e) = 0$. Soit V un voisinage ouvert de e tel que $V^2 \subset U$. Soit m l’application analytique $(a, b) \mapsto \varphi(\varphi^{-1}(a)\varphi^{-1}(b))$ de $\varphi(V) \times \varphi(V)$ dans E. Soit $m = \sum_{i,j \geq 0} m_{i,j}$ le développement en série entière de m en $(0, 0)$, où $m_{ij}$ est un polynôme-continu bihomogène de bidegré $(i, j)$ sur $E \times E$, à valeurs dans E.

(i) On a $m_{i,0} = m_{0,j} = 0$ quels que soient $i \neq 1$ et $j \neq 1$.
(ii) $m_{1,0}(a, b) = a$ et $m_{0,1}(a, b) = b$ quels que soient $a \in E$, $b \in E$.
(iii) Soit $\psi : T_e(G) \to E$ la différentielle de $\varphi$ en e. Quels que soient $u, v$ dans $T_e(G)$, on a
$$
\psi([u, v]) = m_{1,1}(\psi(u), \psi(v)) - m_{1,1}(\psi(v), \psi(u)).
$$
On a $m(a, 0) = a, m(0, b) = b$ quels que soient $a, b$ dans $\varphi(V)$, ce qui prouve (i) et (ii). Soient $u, v$ dans $T_e(G)$. Identifions $T_0(E)$ à E, donc $\psi$ à $T_e(\varphi)$. Les images de $u$ et $v$ par $T_e(\varphi)$ sont $\psi(u)$ et $\psi(v)$. La distribution ponctuelle produit tensoriel de ces images est le produit symétrique de $(\psi(u), 0)$ et de $(0, \psi(v))$ dans $TS(E \times E) = TS(E) \otimes TS(E)$, c’est-à-dire
$$
(\psi(u), 0) \otimes (0, \psi(v)) + (0, \psi(v)) \otimes (\psi(u), 0).
$$

Donc $\varphi_*(u * v)$ est l’image de l’élément précédent par l’application $m$ de $\varphi(V) \times \varphi(V)$ dans $E$. Sa composante de degré 1 dans $TS(E)$ est, d’après le lemme 1,
$$
x = \langle m_{1,1}, (\psi(u), 0) \otimes (0, \psi(v)) + (0, \psi(v)) \otimes (\psi(u), 0) \rangle.
$$
Définissons une application bilinéaire $n : (E \times E)^2 \to E$ par
$$
n((a, b), (a', b')) = m_{1,1}(a, b').
$$
On a $n((a, b), (a, b)) = m_{11}(a, b)$, donc
$$
x = \langle n, (\psi(u), 0) \otimes (0, \psi(v)) + (0, \psi(v)) \otimes (\psi(u), 0) \rangle \\
= m_{1,1}(\psi(u), \psi(v)) + m_{1,1}(0, 0) = m_{1,1}(\psi(u), \psi(v)).
$$
De même, $\varphi_*(v * u)$ admet $m_{1,1}(\psi(v), \psi(u))$ comme composante de degré 1 dans $TS(E)$. Comme $\psi([u, v])$ est de degré 1, cela prouve (iii).

#### Corollaire {#lie-iii-s3-n7-cor-1 .statement}

L’espace normable $T_e(G)$, muni du crochet, est une algèbre de Lie normable.

#### Définition 6 {#lie-iii-s3-def-6 .statement}

L’espace normable $T_e(G)$, muni du crochet, s’appelle l’algèbre de Lie normable de $G$, ou simplement l’algèbre de Lie de $G$, et se note $L(G)$.

#### Proposition 25 {#lie-iii-s3-prop-25 .statement}

Soient $G$ un groupe de Lie, $E(G)$ l’algèbre enveloppante de $L(G)$. L’injection canonique de $L(G)$ dans $U(G)$ définit un homomorphisme $\eta$ de l’algèbre $E(G)$ dans l’algèbre $U(G)$. Si $K$ est de caractéristique 0, $\eta$ est un isomorphisme de bigèbres.

En effet, la bigèbre $U(G)$ est cocommutative (VAR, R, 13.5.1) et la filtration $(U_s(G))$ est compatible avec la structure de bigèbre. L’ensemble des éléments primitifs de $U(G)$ est $L(G)$. Il suffit alors d’appliquer le chap. II, § 1, no 6, th. 1.

Lorsque $K$ est de caractéristique 0, nous identifions désormais $U(G)$ à l’algèbre enveloppante de $L(G)$. D’après (2) et la prop. 7 (ii), l’application $t \mapsto t^\nu$ de $U(G)$ dans $U(G)$ s’identifie alors à l’antiautomorphisme principal de $U(G)$ (chap. I, § 2, no 4).

#### Proposition 26 {#lie-iii-s3-prop-26 .statement}

Supposons $K$ de caractéristique $p > 0$. Pour tout $a \in L(G)$, on a $a^p \in L(G)$ et $\operatorname{ad}(a^p) = (\operatorname{ad} a)^p$ (la puissance $a^p$ étant calculée dans $U(G)$).

Si $a \in L(G)$, $a$ est primitif dans $U(G)$, donc $a^p$ est primitif dans $U(G)$ (chap. II, § 1, no 2, Remarque 1), donc $a^p \in L(G)$. Soit $\sigma_a$ (resp. $\tau_a$) l’application linéaire $x \mapsto a * x$ (resp. $x \mapsto x * a$) de $U(G)$ dans $U(G)$. Pour tout $x \in U(G)$, on a $(\operatorname{ad} a)(x) = (\sigma_a - \tau_a)(x)$, donc $(\operatorname{ad} a)^p = (\sigma_a - \tau_a)^p$. Mais $\sigma_a$ et $\tau_a$ commutent, et par suite $(\sigma_a - \tau_a)^p = (\sigma_a)^p - (\tau_a)^p = \sigma_{a^p} - \tau_{a^p}$, d’où la seconde assertion.

#### Définition 7 {#lie-iii-s3-def-7 .statement}

Soient $X$ une variété de classe $C^r$ ($r \geq 2$), $g$ une algèbre de Lie normable complète. On appelle loi d’opération infinitésimale à gauche (resp. à droite) de classe $C^{r-1}$ de $g$ dans $X$ une application $a \mapsto D_a$ de $g$ dans l’ensemble des champs de vecteurs sur $X$, possédant les propriétés suivantes:

a) l’application $(a, x) \mapsto D_a(x)$ est un morphisme de classe $C^{r-1}$ du fibré vectoriel trivial $g \times X$ dans le fibré vectoriel $T(X)$;
b) on a $[D_a, D_b] = -D_{[a,b]}$ (resp. $[D_a, D_b] = D_{[a,b]}$) quels que soient $a, b$ dans $g$.

En particulier, chaque champ de vecteurs $D_a$ est de classe $C^{r-1}$.

#### Remarque {#lie-iii-s3-n7-rem-1 .statement}

Soient $X$ une variété de classe $C^r$, $g$ une algèbre de Lie de dimension finie, $a \mapsto D_a$ une application linéaire de $g$ dans l’espace vectoriel des champs de vecteurs de classe $C^{r-1}$ sur $X$. Alors la condition a) de la déf. 7 est vérifiée. En effet, en considérant une base de $g$ et en appliquant VAR, R, 7.7.1, on se ramène au cas où $\dim g = 1$, et notre assertion est alors évidente.

#### Proposition 27 {#lie-iii-s3-prop-27 .statement}

Soient $G$ un groupe de Lie, $X$ une variété de classe $C^r$. Supposons donnée une loi d’opération à gauche (resp. à droite) de classe $C^r$ de $G$ dans $X$. Pour tout $a \in L(G)$, soit $D_a$ le champ de distributions ponctuelles défini par $a$ sur $X$.

(i) L’application $(a, x) \mapsto D_a(x)$ est un morphisme de classe $C^{r-1}$ du fibré vectoriel trivial $L(G) \times X$ dans le fibré vectoriel $T(X)$.

(ii) Soient $I$ une partie ouverte de $K$ contenant $0$, et $\gamma : I \to G$ une application de classe $C^r$ telle que $\gamma(0) = e$. Soit $a = T_0(\gamma)1 \in L(G)$. Si $f$ est une fonction de classe $C^r$ sur une partie ouverte de $X$, on a
$$
(D_a f)(x) = \lim_{k \in K^*, k \to 0} k^{-1}(f(\gamma(k)x) - f(x)) \quad \text{si } G \text{ opère à gauche},
$$
$$
(D_a f)(x) = \lim_{k \in K^*, k \to 0} k^{-1}(f(x\gamma(k)) - f(x)) \quad \text{si } G \text{ opère à droite}.
$$

(iii) Si $r \geq 2$, l’application $a \mapsto D_a$ est une loi d’opération infinitésimale à gauche (resp. à droite) de classe $C^{r-1}$ de $L(G)$ dans $X$.

Supposons que $G$ opère à gauche dans $X$. Soit $\varphi : G \times X \to X$ la loi d’opération. Alors $T(\varphi)$ est un $\varphi$-morphisme de classe $C^{r-1}$ du fibré vectoriel $T(G) \times T(X)$ dans le fibré vectoriel $T(X)$ (VAR, R, 8.1.2). Le fibré vectoriel induit $(T(G) \times T(X))|(\{e\} \times X)$ s’identifie à $E = L(G) \times T(X)$. Donc $T(\varphi)|E$ est un morphisme de classe $C^{r-1}$ de fibrés vectoriels. Pour $(a, x) \in L(G) \times X$, on a $T(\varphi)(a, x) = D_a(x)$, d’où (i).

La formule donnant $(D_a f)(x)$ résulte du § 2, fin du n° 2, et de VAR, R, 8.4.5.

Supposons $r \geq 2$. Soient $a, b$ dans $L(G)$ et $f$ une fonction de classe $C^r$ sur une partie ouverte de $X$. On a
$$
D_{[a,b]} f = D_b(D_a f) - D_a(D_b f) \quad \text{d’après (17)}
$$
$$
= [D_b, D_a] f \tag{VAR, R, 8.5.3}.
$$

Soit $x \in X$. En prenant pour $f$ une carte d’un voisinage ouvert de $x$, on en déduit que $D_{[a,b]}(x) = [D_b, D_a](x)$, d’où (iii). On raisonne de même si G opère à droite dans X.

C.Q.F.D.

Lorsque $r \geq 2$, l’application $a \mapsto D_a$ s’appelle la loi d’opération infinitésimale associée à la loi d’opération donnée.

### 8. Propriétés fonctorielles de l’algèbre de Lie

Soient G et H des groupes de Lie, $\varphi$ un morphisme de G dans H. La restriction de $U(\varphi)$ à $L(G)$, qui n’est autre que $T_e(\varphi)$, est un morphisme continu de $L(G)$ dans $L(H)$, qu’on note $L(\varphi)$. Si $\psi$ est un morphisme de H dans un groupe de Lie, on a $L(\psi \circ \varphi) = L(\psi) \circ L(\varphi)$.

Pour que $\varphi$ soit une immersion, il faut et il suffit que $L(\varphi)$ soit un isomorphisme de $L(G)$ sur une sous-algèbre de $L(H)$ admettant un supplémentaire topologique. En particulier, si G est un sous-groupe de Lie de H, et si $\varphi$ est l’injection canonique, on identifie $L(G)$ à une sous-algèbre de Lie de $L(H)$ grâce à $L(\varphi)$. Plus particulièrement, si G est un sous-groupe ouvert de H, on a $L(G) = L(H)$.

Si G est un quasi-sous-groupe de Lie de H, $L(G)$ s’identifie encore à une sous-algèbre de Lie fermée de $L(H)$.

Pour que $\varphi$ soit une submersion, il faut et il suffit que $L(\varphi)$ soit surjectif et que son noyau admette un supplémentaire topologique. Dans ce cas, le noyau N de $\varphi$ est un sous-groupe de Lie de G et $L(N) = \mathrm{Ker}\ L(\varphi)$. En particulier, si H est le groupe de Lie quotient de G par un sous-groupe de Lie distingué P, $L(P)$ est un idéal de $L(G)$, et, si $\varphi$ est la surjection canonique de G sur H, on identifie $L(G/P)$ à $L(G)/L(P)$ grâce au morphisme déduit de $L(\varphi)$ par passage au quotient.

Soient I un ensemble fini, $(G_i)_{i \in I}$ une famille de groupes de Lie, G leur produit, $p_i$ le morphisme canonique de G sur $G_i$. Alors $(L(p_i))_{i \in I}$ est un morphisme de l’algèbre de Lie $L(G)$ dans l’algèbre de Lie $\prod_{i \in I} L(G_i)$, et est un isomorphisme d’espaces normables. On identifie donc $L(G)$ à $\prod_{i \in I} L(G_i)$ grâce à $(L(p_i))_{i \in I}$.

#### Proposition 28 {#lie-iii-s3-prop-28 .statement}

Soient G et H des groupes de Lie, $\varphi$ un morphisme de G dans H. Supposons K de caractéristique 0 et H de dimension finie.

(i) Le noyau N de $\varphi$ est un sous-groupe de Lie de G, et $L(N) = \mathrm{Ker}\ L(\varphi)$.

(ii) Le morphisme $\psi$ de $G/N$ dans H déduit de $\varphi$ par passage au quotient est une immersion.

(iii) Si $\varphi(G)$ est fermé dans H et si la topologie de G a une base dénombrable, $\varphi(G)$ est un sous-groupe de Lie de H, $\psi$ est un isomorphisme du groupe de Lie $G/N$ sur le groupe de Lie $\varphi(G)$, et $L(\varphi(G)) = \mathrm{Im}\ L(\varphi)$.

Faisons opérer G à gauche dans H par l’application $(g, h) \mapsto \varphi(g)h$. Il suffit d’appliquer à l’orbite de e la prop. 14 du § 1, n° 7.

#### Proposition 29 {#lie-iii-s3-prop-29 .statement}

Soient G et H des groupes de Lie, φ un morphisme de G dans H. Supposons K de caractéristique 0 et H de dimension finie. Si H' est un sous-groupe de Lie de H, alors G' = φ^{-1}(H') est un sous-groupe de Lie de G, et L(G') = L(φ)^{-1}(L(H')).

Soit π l’application canonique de H dans l’espace homogène X = H/H'. Faisons opérer G à gauche dans X par l’application (g, x) ↦ φ(g)x. Le stabilisateur de π(e) est G', qui est donc un sous-groupe de Lie de G (§ 1, n° 7, prop. 14). L’application orbitale de π(e) est π ◦ φ. D’après la prop. 14 du § 1, L(G') est le noyau de L(π ◦ φ) = T_e(π) ◦ L(φ). Le noyau de T_e(π) est L(H') (§ 1, n° 6, prop. 11 (i)), donc Ker L(π ◦ φ) = L(φ)^{-1}(L(H')).

#### Corollaire 1 {#lie-iii-s3-prop-29-cor-1 .statement}

Soient G, H des groupes de Lie, φ_1 et φ_2 des morphismes de G dans H. Supposons K de caractéristique 0 et H de dimension finie. L’ensemble des g ∈ G tels que φ_1(g) = φ_2(g) est un sous-groupe de Lie G' de G, et L(G') est l’ensemble des x ∈ L(G) tels que L(φ_1)x = L(φ_2)x.

Posons φ(g) = (φ_1(g), φ_2(g)) pour tout g ∈ G, de sorte que φ est un morphisme de G dans H × H. Soit Δ le sous-groupe diagonal de H × H. Alors G' = φ^{-1}(Δ), et L(φ)x = (L(φ_1)x, L(φ_2)x) pour tout x ∈ L(G). Il suffit maintenant d’appliquer la prop. 29.

#### Corollaire 2 {#lie-iii-s3-prop-29-cor-2 .statement}

Soient G un groupe de Lie de dimension finie, G_1 et G_2 deux sous-groupes de Lie de G. On suppose K de caractéristique 0. Alors G_1 ∩ G_2 est un sous-groupe de Lie de G d’algèbre de Lie L(G_1) ∩ L(G_2).

On applique la prop. 29 à l’injection canonique de G_1 dans G et au sous-groupe G_2.

#### Corollaire 3 {#lie-iii-s3-prop-29-cor-3 .statement}

Soient G, G', H des groupes de Lie, φ : G → H et φ' : G' → H des morphismes de groupes de Lie. Supposons K de caractéristique 0 et H de dimension finie. Soit F l’ensemble des (g, g') ∈ G × G' tels que φ(g) = φ'(g'). Alors F est un sous-groupe de Lie de G × G', et L(F) est l’ensemble des (x, x') ∈ L(G) × L(G') tels que L(φ)x = L(φ')x'.

On applique le cor. 1 aux morphismes (g, g') ↦ φ(g) et (g, g') ↦ φ'(g') de G × G' dans H.

#### Proposition 30 {#lie-iii-s3-prop-30 .statement}

Soient G un groupe de Lie de dimension finie à base dénombrable, H et H' des sous-groupes de Lie de G. On suppose K de caractéristique 0, et HH' localement fermé dans G.

(i) HH' est une sous-variété de G, et T_e(HH') = L(H) + L(H').

(ii) Supposons tout élément de H permutable à tout élément de H'. Alors HH' est un sous-groupe de Lie de G. Soit φ l’application (h, h') ↦ hh' de H × H' sur HH'. Le noyau de φ est l’ensemble des (m, m^{-1}) où m ∈ H ∩ H', et le morphisme de (H × H')/Ker φ sur HH' déduit de φ par passage au quotient est un isomorphisme de groupes de Lie.

Faisons opérer $H \times H'$ à gauche dans $G$ par l’application $((h, h'), g) \mapsto hg{h'}^{-1}$. L’application orbitale $\rho$ de $e$ est $(h, h') \mapsto h{h'}^{-1}$. D’après la prop. 14 (iii) du § 1, n° 7, $HH'$ est une sous-variété de $G$, et $T_e(HH') = \operatorname{Im} T_e(\rho)$. Or
$$
T_e(\rho)(L(H) \times \{0\}) = L(H) \text{ et } T_e(\rho)(\{0\} \times L(H')) = L(H')
$$
donc $T_e(HH') = L(H) + L(H')$. Supposons tout élément de $H$ permutable à tout élément de $H'$. Alors $HH'$ est un sous-groupe de $G$. D’après (i), c’est un sous-groupe de Lie de $G$. Le reste de l’énoncé résulte de la prop. 28.

#### Proposition 31 {#lie-iii-s3-prop-31 .statement}

*Soient G un groupe de Lie de dimension finie à base dénombrable, H un sous-groupe de Lie distingué de G, A un sous-groupe de Lie de G. On suppose que K est de caractéristique 0 et que AH est fermé. Soit $\varphi$ le morphisme canonique de G sur G/H. Alors les applications canoniques*
$$
A/(H \cap A) \to \varphi(A), \qquad AH/H \to \varphi(A)
$$
*sont des isomorphismes de groupes de Lie*.

D’après la prop. 30, $AH$ est un sous-groupe de Lie de $G$. D’après le cor. 2 de la prop. 29, $H \cap A$ est un sous-groupe de Lie de $G$. On peut donc parler des groupes de Lie $AH/H$ et $A/(H \cap A)$. D’autre part, $\varphi(A)$, qui est l’image canonique de $AH$ dans $G/H$, est fermé, donc est un sous-groupe de Lie de $G/H$ (prop. 28 (iii)). La prop. 28, appliquée aux morphismes composés $A \to G \to G/H$ et $AH \to G \to G/H$, prouve que les applications canoniques de la proposition sont des isomorphismes de groupes de Lie.

#### Proposition 32 {#lie-iii-s3-prop-32 .statement}

*Soient G et H des groupes de Lie, k un sous-corps fermé non discret de K, et $\varphi$ un morphisme de G dans H pour les structures de groupes de Lie sur k. Supposons K de caractéristique 0. Si $L(\varphi)$ est K-linéaire, $\varphi$ est un morphisme pour les structures de groupes de Lie sur K*.

Pour tout $g \in G$, on a
$$
T_g(\varphi) = T_e(\gamma(\varphi(g))) \circ L(\varphi) \circ T_g(\gamma(g)^{-1})
$$
donc $T_g(\varphi)$ est K-linéaire. La proposition résulte alors de VAR, R, 5.14.6.

### 9. Algèbre de Lie du groupe des éléments inversibles d’une algèbre

Soit A une algèbre associative normable complète, ayant un élément unité $e$. Soit $A^*$ le groupe des éléments inversibles de A. On a vu ($\S$ 1, n° 1) que $A^*$ est une sous-variété ouverte de A, et est un groupe de Lie. Soient G un groupe de Lie, $f$ un morphisme du groupe de Lie G dans le groupe de Lie $A^*$. On peut considérer f comme une application analytique de G dans l’espace normable complet A. Donc, si $t \in \mathcal{T}^{(\infty)}(G)$, on peut former $\langle t, f \rangle$, qui est un élément de A.

#### Proposition 33 {#lie-iii-s3-prop-33 .statement}

*L’application* $t \mapsto \langle t, f \rangle$ *est un morphisme de l’algèbre* $\mathcal{T}^{(\infty)}(G)$ *dans l’algèbre* A.

Il suffit de vérifier que, si $t$ et $t'$ sont des distributions ponctuelles sur G, on a $\langle t * t', f \rangle = \langle t, f \rangle \langle t', f \rangle$. Or
$$
\begin{align*}
\langle t * t', f \rangle &= \langle t \otimes t', (g, g') \mapsto f(gg') \rangle \\
&= \langle t \otimes t', (g, g') \mapsto f(g)f(g') \rangle \\
&= \langle t, f \rangle \langle t', f \rangle \tag{VAR, R, 13.4.3}.
\end{align*}
$$
C.Q.F.D.

Le morphisme de la prop. 33 est dit *associé à* f.

Prenons pour G le groupe $A^*$ lui-même, et pour $f$ l’application identique $\iota$ de $A^*$. Nous obtenons un morphisme, dit *canonique*, de l’algèbre $\mathcal{T}^{(\infty)}(A^*)$ dans l’algèbre A. L’espace tangent $T_e(A^*)$ s’identifie canoniquement à A; et, si $t \in T_e(A^*)$, la définition de cette identification est telle que $\langle t, \iota \rangle = t$. Ceci posé, la prop. 33 entraîne le corollaire suivant:

#### Corollaire {#lie-iii-s3-n9-cor-1 .statement}

*L’application canonique* $\zeta$ *de* $L(A^*)$ *dans* A *est un isomorphisme de l’algèbre de Lie* $L(A^*)$ *sur l’algèbre de Lie* A. *Autrement dit, on a*
$$
\zeta([a, b]) = \zeta(a)\zeta(b) - \zeta(b)\zeta(a)
$$
*quels que soient* a, b *dans* $L(A^*)$. *Si* K *est de caractéristique* $p > 0$, *on a* $\zeta(a^p) = \zeta(a)^p$ *pour tout* $a \in L(A^*)$.

On identifie désormais $L(A^*)$ et A grâce à l’isomorphisme $\zeta$.

Le morphisme canonique de $\mathcal{T}^{(\infty)}(A^*)$ dans A a été obtenu comme cas particulier du morphisme de la prop. 33. Mais on peut procéder en sens inverse:

#### Proposition 34 {#lie-iii-s3-prop-34 .statement}

*Soient* H *un groupe de Lie, A une algèbre associative normable complète unifière, $\varphi : H \to A^*$ un morphisme de groupes de Lie. Le morphisme associé* $\varphi'$ *de* $\mathcal{T}^{(\infty)}(H)$ *dans* A *s’obtient en composant* $\varphi_*$ *et le morphisme canonique de* $\mathcal{T}^{(\infty)}(A^*)$ *dans* A. *En particulier, $\varphi'(x) = L(\varphi)(x)$ pour tout* $x \in L(H)$.

En effet, soit $i$ l’application identique de $A^*$ dans A. On a, pour tout $t \in \mathcal{T}^{(\infty)}(H)$,
$$
\varphi'(t) = \langle t, \varphi \rangle = \langle t, i \circ \varphi \rangle \\
= \langle \varphi_*(t), i \rangle \tag{VAR, R, 13.2.3}.
$$

### 10. Algèbres de Lie de certains groupes linéaires

Soit E un espace normable complet. Alors $\mathcal{L}(E)$ est une algèbre normable complète unifière, et $\mathbf{GL}(E)$ est un groupe de Lie. D’après le cor. de la prop. 33, n° 9,

#### Proposition 35 {#lie-iii-s3-prop-35 .statement}

*Soit E un espace vectoriel de dimension finie. Soit $\varphi$ le morphisme $g \mapsto \det g$ du groupe de Lie $\mathbf{GL}(E)$ dans le groupe de Lie $K^*$. L’application $L(\varphi)$ de $\mathcal{L}(E)$ dans $K$ est l’application $x \mapsto \operatorname{Tr} x$. Le noyau $\mathbf{SL}(E)$ de $\varphi$ est un sous-groupe de Lie de $\mathbf{GL}(E)$ d’algèbre de Lie $\mathfrak{sl}(E)$.

Choisissons une norme et une base dans E. Le développement du déterminant prouve que
$$
\det(1 + u) \in 1 + \operatorname{Tr} u + o(\|u\|)
$$
quand $u$ tend vers 0 dans $\mathcal{L}(E)$. Donc, compte tenu de la prop. 34, n° 9, on a, pour $x \in \mathcal{L}(E) = L(\mathbf{GL}(E))$:
$$
L(\varphi)(x) = \langle x, \varphi \rangle = \operatorname{Tr} x.
$$
Il en résulte que $\varphi$ est une submersion. Par suite, $\operatorname{Ker} \varphi = \mathbf{SL}(E)$ est un sous-groupe de Lie de $\mathbf{GL}(E)$ dont l’algèbre de Lie est $\operatorname{Ker} L(\varphi) = \mathfrak{sl}(E)$.

C.Q.F.D.

Soient $E_1, \ldots, E_n$ des espaces normables complets, E leur somme directe. Tout $x \in \mathcal{L}(E)$ se représente par une matrice $(x_{ij})_{1 \leq i, j \leq n}$, où $x_{ij} \in \mathcal{L}(E_i, E_j)$.

#### Proposition 36 {#lie-iii-s3-prop-36 .statement}

*Soient I une partie de $\{1, 2, \ldots, n\}$, G le sous-groupe de $\mathbf{GL}(E)$ formé des $g = (g_{ij})_{1 \leq i, j \leq n} \in \mathbf{GL}(E)$ tels que $g_{ij} = 0$ pour $i < j$ et $g_{ii} = 1$ pour $i \in I$. Alors G est un sous-groupe de Lie de $\mathbf{GL}(E)$, et $L(G)$ est l’ensemble des $x = (x_{ij})_{1 \leq i, j \leq n} \in \mathcal{L}(E)$ tels que $x_{ij} = 0$ pour $i < j$ et $x_{ii} = 0$ pour $i \in I$.

Soit S l’ensemble des $(x_{ij}) \in \mathcal{L}(E)$ tels que $x_{ij} = 0$ pour $i < j$ et $x_{ii} = 0$ pour $i \in I$. Alors G est l’intersection de $\mathbf{GL}(E)$ et du sous-espace affine $1 + S$ de $\mathcal{L}(E)$. Donc G est une sous-variété de $\mathbf{GL}(E)$, et l’espace tangent à G en 1 s’identifie à S.

C.Q.F.D

En particulier, dans $\mathbf{GL}(n, K)$, le sous-groupe trigonal large inférieur et le sous-groupe trigonal strict inférieur, définis comme dans INT, VII, § 3, n° 3, sont des sous-groupes de Lie d’algèbres de Lie $t(n, K)$ et $n(n, K)$ (chap. I, § 1, n° 2).

#### Proposition 37 {#lie-iii-s3-prop-37 .statement}

*Soient A une algèbre associative unifère normable complète, $x \mapsto x^t$ une application linéaire continue de A dans A telle que $(x^t)^t = x$, $(xy)^t = y^t x^t$ quels que soient $x, y$ dans A. Supposons K de caractéristique $\neq 2$. Soit G le sous-groupe de $A^*$ formé des $x \in A$ tels que $xx^t = x^t x = 1$. Alors G est un sous-groupe de Lie de $A^*$, et $L(G)$ est l’ensemble des $y \in A$ tels que $y^t = -y$.

Soit S (resp. S') l’ensemble des $y \in A$ tels que $y = y^i$ (resp. $y = -y^i$). Alors S, S' sont des sous-espaces vectoriels fermés de A. La formule

$$
y = \frac{1}{2}(y + y^i) + \frac{1}{2}(y - y^i)
$$

prouve que A est somme directe topologique de S et S'. Soit $f$ l’application de A dans S définie par $f(x) = xx^i$. Cette application est analytique. Pour tout $y \in A$, on a $f(1 + y) = 1 + y + y^i + yy^i$; choisissons une norme sur A compatible avec sa structure d’algèbre; alors

$$
f(1 + y) \in 1 + y + y^i + o(\|y\|) \quad \text{pour } y \text{ tendant vers } 0.
$$

Ainsi, $T_1(f)(y) = y + y^i$, de sorte que $f$ est une submersion en 1. Par suite, il existe un voisinage ouvert U de 1 dans A tel que $U \cap G$ soit une sous-variété de U. Donc (§ 1, n° 3, prop. 6), G est un sous-groupe de Lie de $A^*$. En outre, $L(G) = T_e(G) = \operatorname{Ker} T_1(f)$.

#### Corollaire 1 {#lie-iii-s3-prop-37-cor-1 .statement}

*Supposons K de caractéristique $\neq 2$. Soient E un espace vectoriel de dimension finie sur K, et $\varphi$ une forme bilinéaire symétrique (resp. alternée) non dégénérée sur E. Pour tout $u \in \mathcal{L}(E)$, soit $u^*$ l’adjoint de u relativement à $\varphi$. Soit G le groupe orthogonal (resp. symplectique) de $\varphi$. Alors G est un sous-groupe de Lie de $\mathbf{GL}(E)$, et $L(G)$ est l’ensemble des $x \in \mathcal{L}(E)$ tels que $x^* = -x$.

On applique la prop. 37 avec $A = \mathcal{L}(E)$ et $x^i = x^*$.

#### Remarque {#lie-iii-s3-n10-rem-1 .statement}

Soient B une base de E, et $J$ la matrice de $\varphi$ par rapport à B. Alors $L(G)$ est l’ensemble des éléments de $\mathcal{L}(E)$ dont la matrice $X$ par rapport à B vérifie l’égalité

$$
{}^tX = -J\, X\, J^{-1}.
$$

Ceci résulte de A, IX, § 1, formule (50).

#### Corollaire 2 {#lie-iii-s3-prop-37-cor-2 .statement}

*Soient E un espace hilbertien complexe (resp. réel), U le groupe unitaire de E. Alors U est un sous-groupe de Lie réel de $\mathbf{GL}(E)$, et $L(U)$ est l’ensemble des $x \in \mathcal{L}(E)$ tels que $x^* = -x$.

On applique la prop. 37 avec $A = \mathcal{L}(E)$ considérée comme algèbre sur $\mathbf{R}$, et $x^i = x^*$.

#### Corollaire 3 {#lie-iii-s3-prop-37-cor-3 .statement}

*Soient E un espace vectoriel complexe de dimension finie, $\varphi$ une forme sesquilinéaire hermitienne non dégénérée sur E, U le groupe unitaire de $\varphi$. Alors U est un sous-groupe de Lie réel de $\mathbf{GL}(E)$, et $L(U)$ est l’ensemble des $x \in \mathcal{L}(E)$ tels que ix soit hermitien.

Lorsque $E \neq \{0\}$, U n’est *pas* un sous-groupe de Lie du groupe de Lie complexe $\mathbf{GL}(E)$, car $L(U)$ n’est pas un sous-espace vectoriel complexe de $\mathcal{L}(E)$.

### 11. Représentations linéaires

Soient G un groupe de Lie, E un espace normable complet, π une représentation linéaire analytique de G dans E (§ 1, n° 2). Le morphisme associé $t \mapsto \langle t, \pi \rangle$ de $\mathcal{T}^{(\infty)}(G)$ dans $\mathcal{L}(E)$ est un morphisme d’algèbres (n° 9, prop. 33), et sa restriction à $L(G)$ est $L(\pi)$. Donc $L(\pi)$ est une représentation de $L(G)$ dans E (chap. I, § 3, déf. 1).

#### Proposition 38 {#lie-iii-s3-prop-38 .statement}

Considérons G comme opérant à gauche dans E par l’application $(g, x) \mapsto \pi(g)x$. Soient $b \in E$ et $\rho(b)$ son application orbitale. Identifions canoniquement $T_b(E)$ à E. Pour tout $t \in L(G)$, on a

$$
(L(\pi)t)(b) = \langle t, \rho(b) \rangle = \rho(b)_*t = t * \varepsilon_b.
$$

En particulier, le champ de vecteurs défini par t sur E est le champ $b \mapsto (L(\pi)t)(b)$.

On a $L(\pi)t = \langle t, \pi \rangle$ (n° 9, prop. 34). Comme l’application $A \mapsto Ab$ de $\mathcal{L}(E)$ dans E est linéaire continue, on en déduit que

$$
\begin{align*}
(L(\pi)t)(b) &= \langle t, g \mapsto \pi(g)b \rangle \\
&= \langle t, \mathrm{Id}_E \circ \rho(b) \rangle \\
&= \langle \rho(b)_*t, \mathrm{Id}_E \rangle \quad \text{(VAR, R, 13.2.3)} \\
&= \rho(b)_*t.
\end{align*}
$$

Enfin, $\rho(b)_*t = t * \varepsilon_b$ (n° 3, prop. 14 (ii)).

#### Proposition 39 {#lie-iii-s3-prop-39 .statement}

On suppose K de caractéristique 0. Soient G un groupe de Lie, E un espace vectoriel de dimension finie, π une représentation linéaire analytique de G dans E. Soient $E_1, E_2$ des sous-espaces vectoriels de E tels que $E_2 \subset E_1$. L’ensemble $G_1$ des $g \in G$ tels que $\pi(g)x \equiv x$ (mod. $E_2$) pour tout $x \in E_1$ est un sous-groupe de Lie de G, et $L(G_1)$ est l’ensemble des $a \in L(G)$ tels que $L(\pi)a$ applique $E_1$ dans $E_2$.

Cela résulte des prop. 29 (n° 8) et 36 (n° 10).

#### Corollaire 1 {#lie-iii-s3-prop-39-cor-1 .statement}

Les notations étant celles de la prop. 39, l’ensemble des $g \in G$ tels que $\pi(g)(E_1) \subset E_1$ est un sous-groupe de Lie de G, et son algèbre de Lie est l’ensemble des $a \in L(G)$ tels que $L(\pi)a$ applique $E_1$ dans $E_1$.

On applique la prop. 39 avec $E_1 = E_2$.

#### Corollaire 2 {#lie-iii-s3-prop-39-cor-2 .statement}

Soient G, E, π comme dans la prop. 39. Soit F une partie de E. L’ensemble des $g \in G$ tels que $\pi(g)x = x$ pour tout $x \in F$ est un sous-groupe de Lie de G, et son algèbre de Lie est l’ensemble des $a \in L(G)$ tels que $(L(\pi)a)(x) = 0$ pour tout $x \in F$.

On applique la prop. 39 avec $E_2 = \{0\}$, $E_1$ étant le sous-espace vectoriel de E engendré par F.

C.Q.F.D.

#### Proposition 40 {#lie-iii-s3-prop-40 .statement}

*Soient G un groupe de Lie, E un espace normable complet, $\pi$ une représentation linéaire analytique de G dans E, F un sous-espace vectoriel fermé de E stable par $\pi(G)$. On suppose K de caractéristique 0, ou bien F facteur direct de E.*

(i) *La sous-représentation $\pi_1$ et la représentation quotient $\pi_2$ de $\pi$ définies par F sont des représentations analytiques.*

(ii) *F est stable par $L(\pi)(L(G))$.*

(iii) *Soient $\rho_1$ et $\rho_2$ la sous-représentation et la représentation quotient de $L(\pi)$ définies par F. Alors $L(\pi_1) = \rho_1, L(\pi_2) = \rho_2$.*

Soit A l’ensemble des $u \in \mathcal{L}(E)$ tels que $u(F) \subset F$. Alors A est un sous-espace vectoriel fermé de $\mathcal{L}(E)$, et $\pi$ prend ses valeurs dans A. En vertu des hypothèses sur K et F, l’application $\pi' : G \to A$ de même graphe que $\pi$ est analytique (VAR, R, 5.8.5). Les applications canoniques $\theta_1 : A \to \mathcal{L}(F)$ et $\theta_2 : A \to \mathcal{L}(E/F)$ sont linéaires continues, donc analytiques. Cela prouve (i). Les applications $T_e(\pi)$ et $T_e(\pi')$ ont même graphe, donc $L(\pi)(L(G)) \subset A$, ce qui prouve (ii). On a

$$
T_e(\pi_1) = T_e(\theta_1 \circ \pi') = \theta_1 \circ T_e(\pi') = \rho_1 \\
T_e(\pi_2) = T_e(\theta_2 \circ \pi') = \theta_2 \circ T_e(\pi') = \rho_2.
$$

#### Proposition 41 {#lie-iii-s3-prop-41 .statement}

*Soient G un groupe de Lie, $\pi_1, \pi_2, \ldots, \pi_n, \pi$ des représentations linéaires analytiques de G dans des espaces normables complets $E_1, E_2, \ldots, E_n, E$. Soit $(x_1, x_2, \ldots, x_n) \mapsto x_1 x_2 \ldots x_n$ une application multilinéaire continue de $E_1 \times E_2 \times \cdots \times E_n$ dans E. Supposons que*

$$
\pi(g)(x_1 x_2 \ldots x_n) = (\pi_1(g)x_1)(\pi_2(g)x_2) \ldots (\pi_n(g)(x_n))
$$
*quels que soient $g \in G, x_1 \in E_1, \ldots, x_n \in E_n$. Alors*

$$
(L(\pi)a)(x_1 x_2 \ldots x_n) = \sum_{i=1}^n x_1 x_2 \ldots x_{i-1} ((L(\pi_i)a)x_i) x_{i+1} \ldots x_n
$$
*quels que soient $a \in L(G), x_1 \in E_1, \ldots, x_n \in E_n$.*

Faisons le calcul pour $n = 2$ par exemple. On a

$$
(L(\pi)a)(x_1 x_2) = \langle a, g \mapsto \pi(g)(x_1 x_2) \rangle \quad \text{(prop. 38)} \\
= \langle a, (g \mapsto \pi_1(g)x_1)(g \mapsto \pi_2(g)x_2) \rangle \\
= \langle a, g \mapsto \pi_1(g)x_1 \rangle . x_2 + x_1 . \langle a, g \mapsto \pi_2(g)x_2 \rangle \quad \text{(VAR, R, 5.5.6)} \\
= ((L(\pi_1)a)x_1) . x_2 + x_1 . ((L(\pi_2)a)x_2). \quad \text{(prop. 38)}
$$

$$
(\pi(g)u)(x_1, ..., x_n) = \pi_{n+1}(g)(u(\pi_1(g)^{-1}x_1, ..., \pi_n(g)^{-1}x_n)).
$$

Alors $\pi$ est une représentation linéaire analytique de G dans E, et

$$
((\mathbf{L}(\pi)a)u)(x_1, ..., x_n) = - \sum_{i=1}^n u(x_1, ..., x_{i-1}, (\mathbf{L}(\pi_i)a)x_i, x_{i+1}, ..., x_n)
$$
$$
+ (\mathbf{L}(\pi_{n+1})a)(u(x_1, ..., x_n))
$$

quels que soient $a \in \mathbf{L}(G)$, $u \in E$, $x_1 \in E_1, ..., x_n \in E_n$.

Tout élément $(A_1, ..., A_{n+1})$ de $\mathcal{L}(E_1) \times \cdots \times \mathcal{L}(E_{n+1})$ définit un endomorphisme continu $\theta(A_1, ..., A_{n+1})$ de E par la formule

$$
(\theta(A_1, ..., A_{n+1})u)(x_1, ..., x_n) = A_{n+1}(u(A_1x_1, ..., A_nx_n)).
$$

L’application $\theta$ de $\mathcal{L}(E_1) \times \cdots \times \mathcal{L}(E_{n+1})$ dans $\mathcal{L}(E)$ est multilinéaire continue. On a, pour tout $g \in G$,

$$
\pi(g) = \theta(\pi_1(g^{-1}), ..., \pi_n(g^{-1}), \pi_{n+1}(g))
$$

donc $\pi$ est analytique. Appliquons la prop. 41 à l’application

$$
(x_1, ..., x_n, u) \mapsto u(x_1, ..., x_n)
$$

de $E_1 \times \cdots \times E_n \times E$ dans $E_{n+1}$. On a bien

$$
\pi_{n+1}(g)(u(x_1, ..., x_n)) = (\pi(g)u)(\pi_1(g)x_1, ..., \pi_n(g)x_n)
$$

donc

$$
(\mathbf{L}(\pi_{n+1})a)(u(x_1, ..., x_n))
$$
$$
= \sum_{i=1}^n u(x_1, ..., (\mathbf{L}(\pi_i)a)x_i, ..., x_n) + ((\mathbf{L}(\pi)a)u)(x_1, ..., x_n).
$$

Lorsque les $E_i$ sont de dimension finie, la représentation $\mathbf{L}(\pi)$ de $\mathbf{L}(G)$ se déduit des représentations $\mathbf{L}(\pi_1), ..., \mathbf{L}(\pi_{n+1})$ par le procédé du chap. I, § 3, prop. 3.

#### Corollaire 2 {#lie-iii-s3-prop-41-cor-2 .statement}

Soient G un groupe de Lie, $\pi$ une représentation linéaire analytique de G dans un espace normable complet E. Alors $g \mapsto {}^t\pi(g)^{-1}$ est une représentation linéaire analytique $\rho$ de G dans l’espace normable complet $\mathcal{L}(E, K)$,¹ et $\mathbf{L}(\rho)a = -{}^t(\mathbf{L}(\pi)a)$ pour tout $a \in \mathbf{L}(G)$.

¹ Comme lorsque $K = \mathbf{R}$ ou $\mathbf{C}$, le transposé ${}^t\pi(g)$ envisagé ici est la restriction à $\mathcal{L}(E, K)$ du transposé de $\pi(g)$ au sens purement algébrique.

C’est un cas particulier du cor. 1.

On dit que $\rho$ est la représentation contragrédiente de $\pi$.

Lorsque E est de dimension finie, $L(\rho)$ est la représentation duale de $L(\pi)$ au sens du chap. I, § 3, n° 3.

#### Corollaire 3 {#lie-iii-s3-prop-41-cor-3 .statement}

Soient G un groupe de Lie, $\pi_1, \ldots, \pi_n$ des représentations linéaires analytiques de G dans des espaces vectoriels de dimension finie $E_1, \ldots, E_n$. Alors la représentation $\pi_1 \otimes \cdots \otimes \pi_n$ de G (Appendice) est analytique, et $L(\pi_1 \otimes \cdots \otimes \pi_n)$ est le produit tensoriel de $L(\pi_1), \ldots, L(\pi_n)$.

L’application $(A_1, \ldots, A_n) \mapsto A_1 \otimes \cdots \otimes A_n$ de $\mathcal{L}(E_1) \times \cdots \times \mathcal{L}(E_n)$ dans $\mathcal{L}(E_1 \otimes \cdots \otimes E_n)$ est multilinéaire, d’où le fait que $\pi$ est analytique. Considérons l’application $(x_1, \ldots, x_n) \mapsto x_1 \otimes \cdots \otimes x_n$ de $E_1 \times \cdots \times E_n$ dans $E_1 \otimes \cdots \otimes E_n$. D’après la prop. 41, on voit que

$$
(L(\pi)a)(x_1 \otimes \cdots \otimes x_n) = \sum_{i=1}^n x_1 \otimes \cdots \otimes (L(\pi_i)a)x_i \otimes \cdots \otimes x_n
$$

quels que soient $a \in L(G)$, $x_i \in E_i$ pour $1 \leq i \leq n$. Donc $L(\pi)$ est produit tensoriel des $L(\pi_i)$.

#### Corollaire 4 {#lie-iii-s3-prop-41-cor-4 .statement}

Soient G un groupe de Lie, $\pi$ une représentation linéaire analytique de G dans un espace vectoriel de dimension finie E. Alors les représentations $T^n(\pi)$, $S^n(\pi)$, $\wedge^n(\pi)$ de G (Appendice) sont analytiques, et l’on a

$$
L(T^n(\pi)) = T^n(L(\pi)), \quad L(S^n(\pi)) = S^n(L(\pi)), \quad L(\wedge^n(\pi)) = \wedge^n(L(\pi)).
$$

Cela résulte du cor. 3 et de la prop. 40.

#### Corollaire 5 {#lie-iii-s3-prop-41-cor-5 .statement}

Soit A une algèbre de dimension finie. On suppose K de caractéristique 0. Le groupe Aut(A) des automorphismes de A est un sous-groupe de Lie de $\mathbf{GL}(A)$, et $L(\mathrm{Aut}(A))$ est l’algèbre de Lie des dérivations de A.

Cela résulte du cor. 1 (appliqué à $E = \mathcal{L}(A, A; A)$), et du cor. 2 de la prop. 39 (appliqué à la partie de E réduite à la seule multiplication de A).

#### Remarque {#lie-iii-s3-n11-rem-1 .statement}

Appliquons le cor. 1 avec $G = \mathbf{GL}(F)$ (F, espace normable complet), $\pi_1 = \pi_2 = \mathrm{Id}_G$, $\pi_3$ étant la représentation triviale de G dans K. On obtient une représentation analytique $\pi$ de $\mathbf{GL}(F)$ dans $\mathcal{L}(F, F; K)$. Supposons F de dimension finie et K de caractéristique 0. Appliquant à $\pi$ le cor. 2 de la prop. 39 on retrouve en partie le cor. 1 de la prop. 37.

#### Proposition 42 {#lie-iii-s3-prop-42 .statement}

Soient G un groupe de Lie, X une variété analytique, $(g, x) \mapsto gx$ (resp. $xg$) une loi d’opération à gauche (resp. à droite) analytique de G dans X, $x_0$ un point de X invariant par G. Pour tout $g \in G$, soit $\tau(g)$ l’automorphisme $x \mapsto gx$ (resp. $xg$) de X, et soit $\pi(g)$ l’automorphisme de $T_{x_0}(X)$ tangent en $x_0$ à $\tau(g)$.

(i) $\pi$ est une représentation linéaire analytique de G (resp. $G^\vee$) dans $T_{x_0}(X)$.
(ii) Pour tout $a \in L(G)$ et tout $\xi_0 \in T_{x_0}(X)$, $L(\pi)a.\xi_0$ peut se calculer ainsi : soient

D_a le champ de vecteurs défini par a sur X, et $\xi$ un champ de vecteurs de classe $C^1$ dans un voisinage ouvert de $x_0$, tel que $\xi(x_0) = \xi_0$; alors

$$
L(\pi)a.\xi_0 = -[D_a, \xi](x_0).
$$

On a $\tau(gg') = \tau(g)\tau(g')$ (resp. $\tau(g')\tau(g)$), donc $\pi(gg') = \pi(g)\pi(g')$ (resp. $\pi(g')\pi(g)$). D’autre part, puisque TX est un G-fibré vectoriel de classe $C^\omega$ (§ 1, n° 8, prop. 16), $\pi$ est analytique, d’où (i).

Pour prouver (ii), supposons que G opère à gauche. Il existe un voisinage ouvert I de 0 dans K et une application analytique $\gamma$ de I dans G tels que $\gamma(0) = e$, $T_0(\gamma)1 = a$. Alors $D_a$ est le champ de vecteurs sur X défini par l’application $\varphi : (\lambda, x) \mapsto \gamma(\lambda)x$ de $I \times X$ dans X (§ 2, n° 2). Si l’on note $\varphi_\lambda$ la bijection $x \mapsto \gamma(\lambda)x$ de X dans X, on a

$$
[D_a, \xi](x_0) = \left( \frac{d}{d\lambda} (T_{\varphi_\lambda(x_0)}(\varphi_\lambda^{-1})\xi(\varphi_\lambda(x_0))) \right)_{\lambda=0} \tag{VAR, R, 8.4.5}
$$
$$
= \left( \frac{d}{d\lambda} (T_{x_0}(\varphi_\lambda^{-1})\xi_0) \right)_{\lambda=0}
$$
$$
= \left( \frac{d}{d\lambda} (\pi(\gamma(\lambda))^{-1}\xi_0) \right)_{\lambda=0}.
$$

Comme les applications $\lambda \mapsto \gamma(\lambda)^{-1}$ et $\lambda \mapsto \gamma(-\lambda)$ sont tangentes en 0, cela est encore égal à
$$
= -\left( \frac{d}{d\lambda} (\pi(\gamma(\lambda))\xi_0) \right)_{\lambda=0}
$$
$$
= -\left( \frac{d}{d\lambda} (\pi \circ \gamma)(\lambda) \right)_{\lambda=0} \xi_0
$$
$$
= -L(\pi)a.\xi_0.
$$

### 12. Représentation adjointe

Soit G un groupe de Lie. Considérons la loi d’opération à gauche analytique
$$
(g, g') \mapsto gg'g^{-1} = (\mathrm{Int}\, g)g'
$$
de G dans G. Cette loi d’opération définit, d’après le n° 3, une application bilinéaire de $\mathcal{T}^{(\infty)}(G) \times \mathcal{T}^{(\infty)}(G)$ dans $\mathcal{T}^{(\infty)}(G)$, que nous noterons $\top$ dans ce n°. D’après la prop. 13 du n° 3, on a
$$(22)$$
$$
(t * t') \top t'' = t \top (t' \top t'')
$$
quels que soient $t, t', t''$ dans $\mathcal{T}^{(\infty)}(G)$. D’après la prop. 14 (i) du n° 3, on a
$$(23)$$
$$
\varepsilon_g \top t = (\mathrm{Int}\, g)_* t
$$

quels que soient $g \in G$ et $t \in \mathcal{T}^{(\infty)}(G)$. En particulier, l’application $t \mapsto \varepsilon_g \top t$ de $\mathcal{T}^{(\infty)}(G)$ dans $\mathcal{T}^{(\infty)}(G)$ est un automorphisme de la bigèbre $\mathcal{T}^{(\infty)}(G)$. Ses restrictions à $U(G)$, $U_s(G)$, $L(G)$ se notent $\mathrm{Ad}_{U(G)}(g)$, $\mathrm{Ad}_{U_s(G)}(g)$, $\mathrm{Ad}_{L(G)}(g)$. On écrit souvent $\mathrm{Ad}(g)$ au lieu de $\mathrm{Ad}_{L(G)}(g)$ quand aucune confusion n’en résulte. D’après (23), $\mathrm{Ad}(g)$ est l’application tangente en $e$ à $\mathrm{Int}(g)$. C’est un automorphisme de l’algèbre de Lie normable $L(G)$. Pour $K$ de caractéristique 0, $\mathrm{Ad}_{U(G)}(g)$ est l’unique automorphisme de $U(G)$ prolongeant $\mathrm{Ad}(g)$.

Si $\varphi$ est un morphisme du groupe de Lie $G$ dans un groupe de Lie $H$, on a
$$
\varphi_*(t \top t') = \varphi_*(t) \top \varphi_*(t')
$$
quels que soient $t, t'$ dans $\mathcal{T}^{(\infty)}(G)$; cela résulte de la prop. 15 du no 3.

#### Proposition 43 {#lie-iii-s3-prop-43 .statement}

*Soient $t, u$ dans $\mathcal{T}^{(\infty)}(G)$. Soit $\sum_{i=1}^n t_i \otimes t'_i$ l’image de $t$ par le coproduit.* Alors
$$
t \top u = \sum_{i=1}^n t_i * u * t_{i'}^\vee.
$$
Par définition, $t \top u$ est l’image de $t \otimes u$ par l’application $(g, g') \mapsto gg'g^{-1}$ de $G \times G$ dans $G$. Or cette application s’obtient en composant les applications suivantes:
$$
\begin{align*}
\alpha : (g, g') &\mapsto (g, g, g') & \text{de } G \times G \text{ dans } G \times G \times G \\
\beta : (g, g', g'') &\mapsto (g, {g'}^{-1}, g'') & \text{de } G \times G \times G \text{ dans } G \times G \times G \\
\gamma : (g, g', g'') &\mapsto gg''g' & \text{de } G \times G \times G \text{ dans } G.
\end{align*}
$$
D’autre part:
$$
\alpha_* (t \otimes u) = \sum_{i=1}^n (t_i \otimes t'_i) \otimes u = \sum_{i=1}^n t_i \otimes t'_i \otimes u
$$
$$
\beta_* \left( \sum_{i=1}^n t_i \otimes t'_i \otimes u \right) = \sum_{i=1}^n t_i \otimes t_{i'}^\vee \otimes u
$$
$$
\gamma_* \left( \sum_{i=1}^n t_i \otimes t_{i'}^\vee \otimes u \right) = \sum_{i=1}^n t_i * u * t_{i'}^\vee.
$$

#### Corollaire 1 {#lie-iii-s3-prop-43-cor-1 .statement}

*Soient $u \in L(G)$, $u' \in \mathcal{T}^{(\infty)}(G)$. On a $u \top u' = u * u' - u' * u$.* En effet, l’image de $u$ par le coproduit est $u \otimes \varepsilon_e + \varepsilon_e \otimes u$, d’où
$$
u \top u' = u * u' * \varepsilon_e + \varepsilon_e * u' * u^\vee = u * u' - u' * u.
$$

#### Corollaire 2 {#lie-iii-s3-prop-43-cor-2 .statement}

*Soient $t \in \mathcal{T}^{(\infty)}(G)$ et $g \in G$. On a $\varepsilon_g \top t = \varepsilon_g * t * \varepsilon_{g^{-1}}$. Si $t \in L(G)$, on a $\varepsilon_g \top t = gtg^{-1}$ (ce dernier produit étant calculé dans le groupe $T(G)$).* En effet, l’image de $\varepsilon_g$ par le coproduit est $\varepsilon_g \otimes \varepsilon_g$.

#### Corollaire 3 {#lie-iii-s3-prop-43-cor-3 .statement}

Soit $a \in \mathbf{L}(G)$. Le champ de vecteurs défini par $a$ et par l’opération à gauche $g \mapsto \mathrm{Int}\,g$ de $G$ dans $G$ est le champ $R_a - L_a$.

En effet, la valeur de ce champ en $g$ est
$$
a \top \varepsilon_g = a * \varepsilon_g - \varepsilon_g * a \quad \text{(cor. 1)}
$$
$$
= (R_a)_g - (L_a)_g \quad \text{(déf. 5)}.
$$
C.Q.F.D.

Pour tout $g \in G$ et tout $t \in \mathbf{L}(G)$, on a
$$
(\mathrm{Ad}\,g)(t) = \varepsilon_g \top t = \varepsilon_g * t * \varepsilon_{g^{-1}} = gtg^{-1}.
$$
Puisque $\mathrm{Ad}\,g = T_e(\mathrm{Int}\,g)$, la prop. 42 du n° 11 prouve que $\mathrm{Ad}$ est une représentation linéaire analytique de $G$ dans l’espace normable $\mathbf{L}(G)$.

#### Définition 7 {#lie-iii-s3-def-7-bis .statement}

La représentation $\mathrm{Ad}$ de $G$ dans $\mathbf{L}(G)$ s’appelle la représentation adjointe de $G$.

#### Proposition 44 {#lie-iii-s3-prop-44 .statement}

Pour tout $a \in \mathbf{L}(G)$, on a
$$
(\mathbf{L}(\mathrm{Ad}))(a) = \mathrm{ad}_{\mathbf{L}(G)} a.
$$
Soit $b \in \mathbf{L}(G)$. D’après la prop. 42 (ii) du n° 11 et le cor. 3 de la prop. 43, on a
$$
(\mathbf{L}(\mathrm{Ad}))(a) . b = - [R_a - L_a, L_b](e).
$$
Or $R_a \circ L_b = L_b \circ R_a$ (n° 6, prop. 23 (ii)), d’où $[R_a, L_b] = 0$; compte tenu encore de la prop. 23 (ii), on a
$$
(\mathbf{L}(\mathrm{Ad}))(a) . b = [L_a, L_b](e) = L_{[a, b]}(e) = [a, b] = (\mathrm{ad}_{\mathbf{L}(G)} a) b.
$$

#### Proposition 45 {#lie-iii-s3-prop-45 .statement}

Supposons $G$ de dimension finie et $K$ de caractéristique 0. Soit $s$ un entier $\geqslant 0$. Alors l’application $\pi : g \mapsto \mathrm{Ad}_{U_s(G)}(g)$ est une représentation linéaire analytique de $G$ dans $U_s(G)$, et $\mathbf{L}(\pi)a = \mathrm{ad}_{U_s(G)} a$ pour tout $a \in \mathbf{L}(G)$.

La représentation linéaire $\pi$ est un quotient de $\bigoplus_{r=0}^s \mathrm{T}^r(\mathrm{Ad})$, donc est analytique. Pour $a \in \mathbf{L}(G)$ et $x_1, x_2, \ldots, x_s$ dans $\mathbf{L}(G)$, on a
$$
(\mathbf{L}(\pi)a)(x_1 x_2 \ldots x_s) = \sum_{i=1}^s x_1 \ldots (\mathbf{L}(\mathrm{Ad})a . x_i) \ldots x_s \quad \text{(prop. 41)}
$$
$$
= \sum_{i=1}^s x_1 \ldots ([a, x_i]) \ldots x_s \quad \text{(prop. 44)}
$$
$$
= (\mathrm{ad}_{U_s(G)} a)(x_1 x_2 \ldots x_s).
$$

#### Proposition 46 {#lie-iii-s3-prop-46 .statement}

Soient $h \in G,\ x \in T_h(G)$ et $a \in L(G)$. Soit $\varphi$ l’application $(g, g') \mapsto gg'g^{-1}$ de $G \times G$ dans $G$. L’image $y$ de $(a, x) \in T_e(G) \times T_h(G)$ par $T_{(e,h)}(\varphi)$ est $y = x + h((\mathrm{Ad}\ h^{-1})a - a)$.

En effet,
$$
y = (T_{(e,h)}\varphi)(a \otimes \varepsilon_h + \varepsilon_e \otimes x)
= a \top \varepsilon_h + \varepsilon_e \top x
= a * \varepsilon_h - \varepsilon_h * a + x
= h((\mathrm{Ad}\ h^{-1})a) - ha + x.
$$

#### Proposition 47 {#lie-iii-s3-prop-47 .statement}

Soient $G$ un groupe de Lie, $H$ et $E$ des sous-groupes de Lie de $G$, et supposons que $hEh^{-1} = E$ pour tout $h \in H$. Alors $\mathcal{T}^{(\infty)}(H) \cap \mathcal{T}^{(\infty)}(E) \subset \mathcal{T}^{(\infty)}(E)$. En particulier, $\mathrm{Ad}(H)(L(E)) \subset L(E)$ et $[L(H), L(E)] \subset L(E)$.

En effet, si $t \in \mathcal{T}^{(\infty)}(H)$ et $t' \in \mathcal{T}^{(\infty)}(E)$, on a $t \otimes t' \in \mathcal{T}^{(\infty)}(H \times E)$, et l’image de $H \times E$ par l’application $(g, g') \mapsto gg'g^{-1}$ est contenue dans $E$.

#### Proposition 48 {#lie-iii-s3-prop-48 .statement}

Soient $G$ un groupe de Lie, $H$ et $E$ des sous-groupes de Lie de $G$. Supposons que $G$ soit, en tant que groupe de Lie, produit semi-direct de $H$ par $E$. Soit $\rho$ la représentation linéaire $g \mapsto (\mathrm{Ad}\ g)|L(E)$ du groupe de Lie $G$ dans $L(E)$ (cf. prop. 47), et soit $\sigma$ la restriction de $\rho$ à $H$. Alors:
(i) $L(G)$ est somme directe topologique de $L(H)$ et $L(E)$;
(ii) $L(H)$ est une sous-algèbre de $L(G)$, $L(E)$ est un idéal de $L(G)$;
(iii) $L(\sigma)$ est une représentation linéaire de $L(H)$ dans l’algèbre de Lie des dérivations de $L(E)$;
(iv) $L(G)$ est le produit semi-direct de $L(H)$ par $L(E)$ défini par $L(\sigma)$ (chap. I, § 1, n° 8).

(i) est évident, (ii) résulte de la prop. 47. On a $L(\sigma) = L(\rho)|L(H)$. Or, d’après les prop. 40 (n° 11) et 44 (n° 12), $L(\rho)(t)$ est, pour tout $t \in L(G)$, la restriction de $\mathrm{ad}_{L(G)}t$ à $L(E)$. Cela prouve (iii). Compte tenu de (i) et (ii), cela prouve aussi (iv).

#### Corollaire {#lie-iii-s3-n12-cor-1 .statement}

Soit $G$ un groupe de Lie. Munissons $T_e(G)$ de son unique structure d’algèbre de Lie commutative. Soit $\tau$ la représentation adjointe de $L(G)$. Alors l’algèbre de Lie de $T(G)$ est le produit semi-direct de $L(G)$ par $T_e(G)$ défini par $\tau$. En d’autres termes, pour $x, x'$ dans $L(G)$ et $y, y'$ dans $T_e(G)$, on a
$$
[(x, y), (x', y')] = ([x, x'], [x, y'] + [y, x'])
$$
(le crochet de gauche étant calculé dans $L(T(G))$ et les crochets de droite dans $L(G)$).

Cela résulte de la prop. 48, et de la prop. 6 du § 2, n° 2.

#### Proposition 49 {#lie-iii-s3-prop-49 .statement}

Soit $A$ une algèbre associative unifière normable complète. Identifions $A$ à $L(A^*)$. Alors, si $g \in A^*$ et $y \in A$, on a $(\mathrm{Ad}\ g)y = gyg^{-1}$.

Rappelons que $\mathrm{Ad}\, g = T_1(\mathrm{Int}\, g)$. Soit $u_g$ l’application $x \mapsto gxg^{-1}$ de $A$ dans $A$. La carte identique de $A^*$ dans $A$ transforme $\mathrm{Int}\, g$ en $u_g|A^*$. L’application tangente en chaque point de $A^*$ à cette application est égale à $u_g$, d’où la proposition.

#### Corollaire {#lie-iii-s3-n12-cor-2 .statement}

*Pour tout $g \in A^*$, soit $i(g)$ l’automorphisme $y \mapsto gyg^{-1}$ de $A$, de sorte que $i$ est une représentation linéaire analytique de $A^*$ dans $A$. Pour tout $z \in \mathbf{L}(A^*) = A$, $\mathbf{L}(i)z$ est la dérivation intérieure $y \mapsto zy - yz$ de $A$.
    Cela résulte des prop. 49 et 44.

### 13. Tenseurs et formes invariantes

Soit $G$ un groupe de Lie. Considérons $G$ comme opérant sur lui-même par translations à gauche (resp. à droite). Soit $\lambda$ un foncteur vectoriel de classe $C^\omega$ pour les isomorphismes. Alors $\lambda(TG)$ est un $G$-fibré vectoriel à gauche (resp. à droite) analytique ($§ 1$, n° 8, cor. de la prop. 16). L’application $(g, u) \mapsto gu$ (resp. $ug$) de $G \times \lambda(\mathbf{L}(G))$ sur $\lambda(TG)$ est un isomorphisme $\varphi$ (resp. $\psi$) de $G$-fibrés vectoriels ($§ 1$, n° 8, cor. 2 de la prop. 17). Toute section $G$-invariante de $\lambda(TG)$ est analytique, et déterminé par sa valeur en $e$ ($§ 1$, n° 8, cor. 1 de la prop. 17). Une telle section est dite *invariante à gauche* (resp. *à droite*). Soit $\sigma$ une section invariante-à-gauche de $\lambda(TG)$; la transformée $\sigma'$ de $\sigma$ par une translation à droite $\delta(g)$ est définie par $\sigma'(\delta(g)h) = \lambda(T_h(\delta(g)))\sigma(h)$ quel que soit $h \in G$; elle est encore invariante à gauche; elle se déduit aussi de $\sigma$ par $\gamma(g) \circ \delta(g) = \mathrm{Int}(g)$, donc

$$
\sigma'(e) = \lambda(\mathrm{Ad}\, g) \cdot \sigma(e).
$$

De même, soit $\tau$ une section invariante à droite de $\lambda(TG)$; la transformée $\tau'$ de $\tau$ par une translation à gauche $\gamma(g)$ est encore invariante à droite, et l’on a

$$
\tau'(e) = \lambda(\mathrm{Ad}\, g) \cdot \tau(e).
$$

Considérons maintenant $G \times G$ comme opérant à gauche dans $G$ par $((g, g'), g'') \mapsto gg''{g'}^{-1}$. Alors $G$ est un espace homogène de Lie à gauche pour $G \times G$ ($§ 1$, n° 6, *Exemple*). Donc $\lambda(TG)$ est un $(G \times G)$-fibré vectoriel à gauche analytique. Une section de $\lambda(TG)$ est dite *biinvariante* si elle est invariante par l’action de $G \times G$ dans $\lambda(TG)$, autrement dit si elle est invariante par les translations à gauche et à droite. Soit $\lambda(\mathbf{L}(G))_0$ l’ensemble des éléments de $\lambda(\mathbf{L}(G))$ invariants par $\lambda(\mathrm{Ad}(G))$. Pour tout $u \in \lambda(\mathbf{L}(G))_0$, soit $\sigma_u$ l’application de $G$ dans $\lambda(TG)$ définie par $\sigma_u(g) = gu = ug$. Alors, $u \mapsto \sigma_u$ est une bijection de $\lambda(\mathbf{L}(G))_0$ sur l’ensemble des sections biinvariantes de $\lambda(TG)$ ($§ 1$, n° 8, cor. 1 de la prop. 17).

#### Proposition 50 {#lie-iii-s3-prop-50 .statement}

*Soit $G$ un groupe de Lie (supposé de dimension finie si $K$ est de caractéristique $> 0$). Soit $E$ l’espace vectoriel des formes multilinéaires alternées continues de degré k sur $T_e(G)$. Pour tout $u \in E$, soit $\omega^u$ la forme différentielle de degré k sur G telle que $(\omega^u)_g$ soit la forme multilinéaire sur $T_g(G)$ déduite de u par la translation $h \mapsto gh$ (resp. $h \mapsto hg$). Alors $\omega^u$ est analytique invariante à gauche (resp. à droite) sur G. L’application $u \mapsto \omega^u$ est un isomorphisme de E sur l’espace vectoriel des formes différentielles de degré k invariantes à gauche (resp. à droite) sur G.

C’est un cas particulier de ce qu’on a dit plus haut.

Soit F un espace normable complet. La prop. 50 reste valable si l’on remplace les formes différentielles sur G à valeurs dans K par les formes différentielles sur G à valeurs dans F. Pour toute application linéaire continue u de $T_e(G)$ dans F, il existe une forme différentielle $\omega^u$ de degré 1 sur G, à valeurs dans F, telle que $(\omega^u)_g = u \circ T_g(\gamma(g)^{-1})$. En particulier, prenons $F = T_e(G)$ et $u = \mathrm{Id}_{T_e(G)}$. On obtient alors la forme différentielle $\omega$ sur G telle que $\omega_g = T_g(\gamma(g^{-1}))$; cette forme différentielle est invariante à gauche et analytique; on l’appelle la forme différentielle canonique gauche de G. On a $\omega_g(t) = g^{-1}t$ pour tout $t \in T_g(G)$.

Si F est de nouveau un espace normable complet quelconque, et si $u \in \mathcal{L}(T_e(G), F)$, on a $\omega^u = u \circ \omega$. En particulier (prenant $F = K$), l’application $v \mapsto v \circ \omega$ est une bijection linéaire du dual de $T_e(G)$ sur l’espace vectoriel des formes différentielles de degré 1 à valeurs dans K invariantes à gauche sur G.

De même, la forme différentielle $\omega'$ sur G telle que $\omega'_g = T_g(\delta(g))$ s’appelle la forme différentielle canonique droite de G. On a des propriétés analogues à celles de $\omega$, qu’on laisse au lecteur le soin d’énoncer. L’application $g \mapsto g^{-1}$ de G sur G transforme $\omega$ en $\omega'$.

### 14. Formules de Maurer-Cartan

Soit X une variété de classe $C^r$, de dimension finie si K est de caractéristique > 0 et soit L une algèbre de Lie normable complète. Soit $\alpha$ une forme différentielle de degré 1 sur X à valeurs dans L, de classe $C^{r-1}$. Soit $x \in X$. L’application

$$
(u_1, u_2) \mapsto [\alpha_x(u_1), \alpha_x(u_2)]
$$

de $T_x(X) \times T_x(X)$ dans L est une forme bilinéaire alternée continue sur $T_x(X)$, à valeurs dans L. Nous la noterons $[\alpha]^2_x$, de sorte que $[\alpha]^2$ est une forme différentielle de degré 2 sur X à valeurs dans L. Identifiant un voisinage ouvert de x dans X à une partie ouverte d’un espace de Banach, on voit aussitôt que $[\alpha]^2$ est de classe $C^{r-1}$. Si $X'$ est une variété de classe $C^r$ et $f : X' \to X$ un morphisme, on a

$$
[f^*(\alpha)]^2 = f^*([\alpha]^2).
$$

Soient $\alpha, \beta$ deux formes différentielles de degré 1 sur X à valeurs dans L, de classe $C^{r-1}$. Le produit extérieur $\alpha \wedge \beta$ de $\alpha$ et $\beta$ (VAR, R, 7.8.2) est une forme différentielle de degré 2 sur X, à valeurs dans L, de classe $C^{r-1}$; on a

$$
(\alpha \wedge \beta)_x(u_1, u_2) = [\alpha_x(u_1), \beta_x(u_2)] - [\alpha_x(u_2), \beta_x(u_1)]
$$

pour $u_1, u_2$ dans $T_x(X)$. Il est immédiat que
$$
[\alpha + \beta]^2 = [\alpha]^2 + [\beta]^2 + \alpha \wedge \beta
$$
$$
\alpha \wedge \alpha = 2[\alpha]^2.
$$

#### Proposition 51 {#lie-iii-s3-prop-51 .statement}

*Soit G un groupe de Lie, de dimension finie si K est de caractéristique > 0, et soient $a_1, \ldots, a_p$ des éléments de $L(G)$, F un espace normable complet, $\alpha$ une forme différentielle de degré $p - 1$ sur G à valeurs dans F. Si $\alpha$ est invariante à gauche, on a*
$$
(d\alpha)_e(a_1, \ldots, a_p) =
\sum_{i < j} (-1)^{i+j} \alpha_e([a_i, a_j], a_1, \ldots, a_{i-1}, a_{i+1}, \ldots, a_{j-1}, a_{j+1}, \ldots, a_p).
$$
*Si $\alpha$ est invariante à droite, on a*
$$
(d\alpha)_e(a_1, \ldots, a_p) =
-\sum_{i < j} (-1)^{i+j} \alpha_e([a_i, a_j], a_1, \ldots, a_{i-1}, a_{i+1}, \ldots, a_{j-1}, a_{j+1}, \ldots, a_p).
$$

Supposons $\alpha$ invariante à gauche. D’après VAR, R, 8.5.7, on a
$$
(d\alpha)(L_{a_1}, \ldots, L_{a_p}) = \sum_i (-1)^{i-1} L_{a_i} \alpha(L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_p})
+ \sum_{i < j} (-1)^{i+j} \alpha([L_{a_i}, L_{a_j}], L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_{j-1}}, L_{a_{j+1}}, \ldots, L_{a_p}).
$$
Mais les fonctions $\alpha(L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_p})$ sur G sont invariantes à gauche, donc constantes. Donc
$$
L_{a_i} \alpha(L_{a_1}, \ldots, L_{a_{i-1}}, L_{a_{i+1}}, \ldots, L_{a_p}) = 0.
$$
Par ailleurs, $[L_{a_i}, L_{a_j}] = L_{[a_i, a_j]}$ (prop. 23), d’où la première formule de la prop. 51. La deuxième s’établit de manière analogue, en tenant compte cette fois de $[R_{a_i}, R_{a_j}] = -R_{[a_i, a_j]}$.

#### Corollaire 1 {#lie-iii-s3-prop-51-cor-1 .statement}

*Soient G un groupe de Lie, de dimension finie si K est de caractéristique > 0, $\omega$ et $\omega'$ les formes différentielles canoniques gauche et droite de G. On a*
$$
d\omega + [\omega]^2 = 0 \qquad d\omega' - [\omega']^2 = 0.
$$
D’après la prop. 51, on a
$$
(d\omega)_e(a_1, a_2) = -\omega_e([a_1, a_2]) = -[a_1, a_2] = -[\omega_e(a_1), \omega_e(a_2)]
= -[\omega]^2_e(a_1, a_2)
$$
d’où la première formule. La deuxième s’établit de manière analogue.

#### Corollaire 2 {#lie-iii-s3-prop-51-cor-2 .statement}

*Supposons G de dimension finie. Soient $(e_1, \ldots, e_n)$ une base de $L(G)$, $(e_1^*, \ldots, e_n^*)$ la base duale, $(c_{ijk})$ les constantes de structure de $L(G)$ relativement à la base* (e_1, \ldots, e_n), \omega_i (\text{resp. } \omega'_i) \text{ la forme différentielle invariante à gauche (resp. à droite) sur } G, à valeurs dans K, telle que (\omega_i)_e = e_i^* (\text{ resp. } (\omega'_i)_e = e_i^*). Alors

$$
d\omega_k + \sum_{i < j} c_{ijk} \omega_i \wedge \omega_j = 0 \quad (k = 1, 2, \ldots, n)
$$
$$
d\omega'_k - \sum_{i < j} c_{ijk} \omega'_i \wedge \omega'_j = 0 \quad (k = 1, 2, \ldots, n).
$$

En effet, si $r < s$, on a
$$
(d\omega_k)_e(e_r, e_s) = - (\omega_k)_e([e_r, e_s])
$$
$$
= - \sum_l c_{rst} (\omega_k)_e(e_l)
$$
$$
= - c_{rsk}
$$
$$
= - \sum_{i < j} c_{ijk} (\omega_i \wedge \omega_j)_e(e_r, e_s).
$$

On raisonne de même pour les $\omega'_k$.

### 15. Construction de formes différentielles invariantes

#### Lemme 2 {#lie-iii-s3-lem-2 .statement}

Soient $G$ un groupe de Lie, $U$ un voisinage ouvert symétrique de $e$ dans $G$, $E$ un espace normable complet, $\varphi : U^2 \to E$ une application analytique. Pour tout $g \in U$, soit $\omega_g$ la différentielle au point $g$ de l’application $h \mapsto \varphi(g^{-1}h)$. Alors $\omega$ est la restriction à $U$ de la forme différentielle invariante à gauche sur $G$ dont la valeur en $e$ est $d_e \varphi$.

Il est clair que $\omega_e = d_e \varphi$. Pour tout $g \in U$ et tout $t \in T_e(G)$, on a
$$
\langle \omega_g, T_e(\gamma(g))t \rangle = \langle d_g(\varphi \circ \gamma(g)^{-1}), T_e(\gamma(g))t \rangle
$$
$$
= \langle d_e \varphi \circ T_g(\gamma(g)^{-1}), T_e(\gamma(g))t \rangle = \langle d_e \varphi, t \rangle
$$
donc $\omega_g$ se déduit de $d_e \varphi$ par $T_e(\gamma(g))$.

#### Proposition 52 {#lie-iii-s3-prop-52 .statement}

Soient $n$ un entier $> 0$, $G$ un groupe de Lie de dimension $n$, $U$ un voisinage ouvert symétrique de $e$ dans $G$, $\psi : U^2 \to K^n$ une carte de $G$ telle que $\psi(e) = 0$. Si $(x_1, \ldots, x_n)$ sont les coordonnées de $x \in \psi(U)$ et $(y_1, \ldots, y_n)$ les coordonnées de $y \in \psi(U)$, notons
$$
m_1(x_1, \ldots, x_n, y_1, \ldots, y_n), \ldots, m_n(x_1, \ldots, x_n, y_1, \ldots, y_n)
$$
les coordonnées de $\psi(\psi^{-1}(x)^{-1}\psi^{-1}(y))$. Alors, si l’on pose, pour $1 \leq k \leq n$,
$$
\varpi_k(x_1, \ldots, x_n) = D_{n+1} m_k(x_1, \ldots, x_n, x_1, \ldots, x_n) dx_1 + \cdots
$$
$$
+ D_{2n} m_k(x_1, \ldots, x_n, x_1, \ldots, x_n) dx_n,
$$
les formes différentielles $\varpi_k$ sur $\psi(U)$ sont déduites par $\psi$ de formes différentielles invariantes à gauche sur $G$, et telles que $\varpi_k(0, \ldots, 0) = dx_k$.

Appliquons le lemme 2 avec $E = K$, en prenant pour $\varphi(g)$ la coordonnée d’indice $k$ de $\psi(g)$. On obtient une forme différentielle $\omega_k$; soit $\varpi_k$ sa transformée par $\psi$. La valeur de $\varpi_k$ en $(x_1, \ldots, x_n)$ est la différentielle en $(x_1, \ldots, x_n)$ de la fonction $y \mapsto m_k(x_1, \ldots, x_n, y_1, \ldots, y_n)$; cette valeur est donc fournie par la formule (32). Il suffit alors d’utiliser la conclusion du lemme 2.

#### Proposition 53 {#lie-iii-s3-prop-53 .statement}

Soient $G$ un groupe de Lie, $A$ une algèbre normable complète, $\varphi$ un morphisme de groupes de Lie de $G$ dans $A^*$. Pour tout $g \in G$, soit $\omega_g = \varphi(g)^{-1} \cdot d_g \varphi$. Alors $\omega$ est la forme différentielle invariante à gauche sur $G$ dont la valeur en $e$ est $d_e \varphi$.

En effet, appliquons le lemme 2 avec $E = A$, $U = G$. La différentielle en $g$ de l’application $h \mapsto \varphi(g^{-1}h) = \varphi(g)^{-1} \varphi(h)$ est $\varphi(g)^{-1} \cdot d_g \varphi$.

### 16. Mesure de Haar sur un groupe de Lie

Soit $G$ un groupe de Lie de dimension finie $n$. Alors $\wedge^n(T_e(G))$ est de dimension 1. Donc (n° 13) l’espace vectoriel $S$ des formes différentielles de degré $n$ invariantes à gauche sur $G$ est de dimension 1. Soit $(\omega_1, \ldots, \omega_n)$ une base de l’espace vectoriel des formes différentielles de degré 1 invariantes à gauche sur $G$; alors $\omega_1 \wedge \omega_2 \wedge \cdots \wedge \omega_n$ est une base de $S$.

#### Proposition 54 {#lie-iii-s3-prop-54 .statement}

Soient $G$ un groupe de Lie de dimension finie $n$, $\omega$ une forme différentielle de degré $n$ invariante à gauche sur $G$, et $\varphi$ un endomorphisme de $G$. On a
$$
\varphi^*(\omega) = (\det L(\varphi)) \omega.
$$
Posons $L(\varphi) = u, \omega_e = f, \varphi^*(\omega)_e = g$. Quels que soient $x_1, \ldots, x_n$ dans $L(G)$, on a
$$
g(x_1, \ldots, x_n) = f(ux_1, \ldots, ux_n) = (\det u) f(x_1, \ldots, x_n)
$$
donc $\varphi^*(\omega)_e = \det L(\varphi) \cdot \omega_e$. D’autre part, si $g \in G$, on a $\varphi \circ \gamma(g) = \gamma(\varphi(g)) \circ \varphi$, donc $\gamma(g)^* \varphi^*(\omega) = \varphi^*(\omega)$. Ainsi, $\varphi^*(\omega)$ est invariante à gauche, d’où la proposition.

#### Corollaire {#lie-iii-s3-n16-cor-1 .statement}

Pour tout $g \in G$, on a
$$
\delta(g)^* \omega = (\det \mathrm{Ad}\ g) \omega.
$$
En effet, $\delta(g)^* \omega = \delta(g)^* \gamma(g)^* \omega = (\mathrm{Int}\ g)^* \omega$, et $L(\mathrm{Int}\ g) = \mathrm{Ad}\ g$.

Soient $G$ un groupe localement compact, $\varphi$ un endomorphisme de $G$. Supposons qu’il existe des voisinages ouverts $V, V'$ de $e$ tels que $\varphi(V) = V'$ et que $\varphi|V$ soit un isomorphisme local de $G$ à $G$. Soit $\mu$ une mesure de Haar à gauche

#### Proposition 55 {#lie-iii-s3-prop-55 .statement}

*Supposons K localement compact. Soit $\mu$ une mesure de Haar sur le groupe additif de K. Soit G un groupe de Lie de dimension finie n.*

(i) *Soit $\omega$ une forme différentielle de degré n sur G, invariante à gauche et non nulle. Alors la mesure mod $(\omega)_\mu$ (VAR, R, 10.1.6) est une mesure de Haar à gauche de G. Si $K = \mathbf{R}$, et si G est muni de l’orientation définie par $\omega$, la mesure définie par $\omega$ (VAR, R, 10.4.3) est une mesure de Haar à gauche de G.*

(ii) *Soit $\varphi$ un endomorphisme étale de G. On a $\mathrm{mod} \varphi = \mathrm{mod} \det L(\varphi)$.

(i) est évident. Soient V, $V'$ des voisinages ouverts de $e$ tels que $\varphi(V) = V'$ et que $\varphi|V$ soit un isomorphisme local de G à G. On a*

$$
\varphi^{-1}(\mathrm{mod} (\omega)_\mu | V') = \mathrm{mod} (\varphi^*(\omega))_\mu | V) \quad \text{par transport de structure}
$$
$$
= \mathrm{mod}(\det L(\varphi)\omega | V)_\mu \quad \text{(prop. 54)}
$$
$$
= \mathrm{mod} \det L(\varphi) \ (\mathrm{mod} (\omega)_\mu) | V)
$$

d’où $\mathrm{mod} \varphi = \mathrm{mod} \det L(\varphi)$ par définition de $\mathrm{mod} \varphi$.

#### Corollaire {#lie-iii-s3-n16-cor-2 .statement}

*Pour tout $g \in G$, on a $\Delta_G(g) = (\mathrm{mod} \det \mathrm{Ad} \ g)^{-1}$. En particulier, pour que G soit unimodulaire, il faut et il suffit $\mathrm{mod} \det \mathrm{Ad} \ g = 1$ pour tout $g \in G$.

En effet,

$$
\Delta_G(g) = (\mathrm{mod} \mathrm{Int} \ g)^{-1} \tag{INT, VII, § 1, formule (33)}
$$
$$
= (\mathrm{mod} \det L(\mathrm{Int} \ g))^{-1} \tag{prop. 55}
$$
$$
= (\mathrm{mod} \det \mathrm{Ad} \ g)^{-1}.
$$

#### Remarque {#lie-iii-s3-n16-rem-1 .statement}

Reprenons les hypothèses et les notations de la prop. 52, et supposons K localement compact. Soit $\mu$ la mesure
$$
\mathrm{mod} \det (D_{n+i} m_k (x_1, \ldots, x_n, x_1, \ldots, x_n))_{1 \leq i, k \leq n} dx_1 \ldots dx_n
$$
sur $\psi(U)$. Alors $\psi^{-1}(\mu)$ est la restriction à U d’une mesure de Haar de G.

#### Proposition 56 {#lie-iii-s3-prop-56 .statement}

*Soient G un groupe de Lie de dimension finie n, H un sous-groupe de Lie de dimension p, X l’espace homogène de Lie G/H. On suppose que*
$$
\det \mathrm{Ad}_{L(G)} h = \det \mathrm{Ad}_{L(H)} h
$$
*pour tout $h \in H$. Alors:*

(i) *Les formes différentielles de degré n — p sur X invariantes par G sont analytiques.*

(ii) *L’espace vectoriel de ces formes est de dimension 1.*

(iii) Si $\omega$ est une telle forme non nulle, et si $K$ est localement compact, mod $(\omega)_u$ est une mesure non nulle sur $X$ invariante par $G$.

D’après le § 1, n° 8, Exemples, $\mathrm{Alt}^{n-p}(TX, K)$ est un $G$-fibré vectoriel analytique. Soit $x_0$ l’image canonique de $e$ dans $X$; son stabilisateur est $H$. La fibre de $\mathrm{Alt}^{n-p}(TX, K)$ en $x_0$ est $\wedge^{n-p} T_{x_0}(X)^*$, et $T_{x_0}(X)$ s’identifie canoniquement à $L(G)/L(H)$. Si $h \in H$, l’automorphisme $\tau_h$ de $X$ défini par $h$ se déduit par passage au quotient de l’automorphisme $g \mapsto hgh^{-1}$ de $G$. Donc l’automorphisme $T_{x_0}(\tau_h)$ se déduit par passage au quotient de $\mathrm{Ad}_{L(G)}(h)$. Comme

$$
\det \mathrm{Ad}_{L(G)} h = (\det \mathrm{Ad}_{L(H)} h) \cdot (\det T_{x_0}(\tau_h)),
$$

l’hypothèse entraîne que $\det T_{x_0}(h) = 1$. Ainsi, tout élément de $\wedge^{n-p} T_{x_0}(X)^*$ est invariant par $H$. Ceci posé, (i) et (ii) résultent du § 1, n° 8, cor. 1 de la prop. 17, et (iii) est évident.

L’existence d’une mesure positive non nulle sur $X$ invariante par $G$ résulte d’ailleurs d’INT, VII, § 2, cor. 2 du th. 3, car l’hypothèse de la prop. 56 implique $\Delta_G|H = \Delta_H$ (cor. de la prop. 55).

#### Proposition 57 {#lie-iii-s3-prop-57 .statement}

Soit $G$ un groupe de Lie de dimension finie $n$. Choisissons une base de $\wedge^n T_e(G)^*$; grâce à la trivialisation droite (resp. gauche) de $\wedge^n T(G)^*$, cela permet d’identifier ce fibré vectoriel au fibré vectoriel trivial $G \times K$, de sorte que le transposé d’un opérateur différentiel scalaire s’identifie à un opérateur différentiel scalaire.

Ceci posé, si $u \in U(G)$, le transposé de $L_u$ (resp. $R_u$) est $L_u^\vee$ (resp. $R_u$).

Nous raisonnons dans le cas où on a trivialisé $\wedge^n T(G)^*$ à l’aide d’une forme $\omega$ invariante à droite.

Supposons la proposition prouvée pour des éléments $u_1, u_2$ de $U(G)$. Alors,

$$
\begin{align*}
t(L_{u_1 * u_2}) &= t(L_{u_1} \circ L_{u_2}) & \text{(prop. 23)} \\
&= t(L_{u_2}) \circ t(L_{u_1}) & \text{(VAR, R, 14.3.3)} \\
&= L_{u_2}^\vee \circ L_{u_1}^\vee & \text{par hypothèse} \\
&= L_{u_2 * u_1}^\vee & \text{(prop. 23)} \\
&= L_{(u_1 * u_2)^\vee} & \text{(prop. 7)},
\end{align*}
$$

donc la proposition est vraie pour $u_1 * u_2$. Il suffit par conséquent de prouver la proposition quand $u \in T_e(G)$. Or, $L_u$ est défini par $G$ opérant à droite dans $G$ (n° 6), donc $\theta_{L_u} \omega = 0$ puisque $\omega$ est invariante à droite (VAR, R, 8.4.5); par suite, si $f$ est une fonction analytique dans un voisinage ouvert de $e$, à valeurs dans $K$, on a $\theta_{L_u}(f \omega) = (\theta_{L_u} f) \omega$ (VAR, R, 8.4.8). Compte tenu des identifications faites et de VAR, R, 14.4.1, le transposé de $L_u$ est $-L_u$, c’est-à-dire $L_u^\vee$.

#### Corollaire {#lie-iii-s3-n16-cor-3 .statement}

Soient $G$ un groupe de Lie réel de dimension finie, $\mu$ (resp. $\nu$) une mesure de Haar à gauche (resp. à droite) de G, k un entier $\geqslant 0$, $u \in U_k(G)$, f et g des fonctions réelles de classe $C^k$ sur G à support compact. Alors

$$
\int_G (R_u f) g \, d\mu = \int_G f(R_{u^*} g) \, d\mu
$$
$$
\int_G (L_u f) g \, dv = \int_G f(L_{u^*} g) \, dv.
$$

Cela résulte de la prop. 57, et de VAR, R, 14.3.8.

### 17. Différentielle gauche

#### Définition 8 {#lie-iii-s3-def-8 .statement}

Soient G un groupe de Lie, M une variété de classe $C^r$, f une application de classe $C^r$ de M dans G. On appelle différentielle gauche (resp. droite) de f la forme différentielle de degré 1 sur M à valeurs dans $L(G)$ qui, à tout vecteur $u \in T_m(M)$, associe l’élément $f(m)^{-1} \cdot (T_m f)(u)$ (resp. $(T_m f)(u) \cdot f(m)^{-1}$).

Dans ce chapitre, nous ne considérerons que la différentielle gauche, que nous noterons $f^{-1} \cdot df$, et laisserons au lecteur le soin de traduire les résultats pour la différentielle droite.

Si f est l’application identique de G, $f^{-1} \cdot df$ est la forme différentielle gauche canonique $\omega$ de G. Revenant au cas général de la déf. 8, on a $(f^{-1} \cdot df)_m = \omega_{f(m)} \circ T_m(f)$, donc $f^{-1} \cdot df = f^*(\omega)$. Cela entraîne que $f^{-1} \cdot df$ est de classe $C^{r-1}$.

#### Exemple 1 {#lie-iii-s3-n17-exa-1 .statement}

Si G est le groupe additif d’un espace normable complet, et si on identifie canoniquement $T_0(E)$ à E, $f^{-1} \cdot df$ est la différentielle $df$ définie en VAR, R, 8.2.2.

#### Exemple 2 {#lie-iii-s3-n17-exa-2 .statement}

Supposons que G soit le groupe multiplicatif $A^*$ associé à une algèbre normable complète A. Alors f peut être considérée comme une application de M dans A, donc la différentielle $df$ au sens de VAR, R, 8.2.2 est définie, et le produit $f^{-1} \, df$ au sens de VAR, R, 8.3.2 est défini. Il est clair que cette dernière forme est identique à la différentielle gauche de f.

#### Proposition 58 {#lie-iii-s3-prop-58 .statement}

Soient G et H deux groupes de Lie, M une variété de classe $C^r$, f une application de classe $C^r$ de M dans G, et h un morphisme de G dans H. On a

$$
(h \circ f)^{-1} \cdot d(h \circ f) = L(h) \circ (f^{-1} \cdot df) = (h^{-1} \cdot dh) \circ T(f).
$$

On a, en effet, quels que soient $x \in M$ et $u \in T_x(M)$,

$$
(h \circ f)^{-1} \cdot d(h \circ f)(u) = ((h \circ f)(x))^{-1} \cdot T(h \circ f)(u).
$$

Cette dernière expression est égale, d’une part, à

$$
T(h)(f(x)^{-1} \cdot T(f)(u)) \quad (\text{§ 2, prop. 5})
$$
$$
= T_e(h)((f^{-1} \cdot df)(u))
$$

et d’autre part à

$$
h(f(x))^{-1} T(h)(T(f)u)
= (h^{-1}.dh)(T(f)u).
$$

#### Proposition 59 {#lie-iii-s3-prop-59 .statement}

*Soient G un groupe de Lie, M une variété de classe C^r, f et g des applications de classe C^r de M dans G, et p la surjection canonique de TM sur M.*

(i) *On a*

$$(fg)^{-1}.d(fg) = (\mathrm{Ad} \circ g \circ p)^{-1} \circ (f^{-1}.df) + g^{-1}.dg.$$

(ii) *Posons h(m) = f(m)^{-1} pour tout m \in M. Alors*

$$h^{-1}.dh = -(\mathrm{Ad} \circ f \circ p) \circ (f^{-1}.df).$$

L’assertion (i) résulte du § 2, n° 2, prop. 7. L’assertion (ii) résulte de (i) en faisant $g = h$.

#### Corollaire 1 {#lie-iii-s3-prop-59-cor-1 .statement}

*Soient s \in G, et sg l’application x \mapsto sg(x) de M dans G. On a*

$$(sg)^{-1}.d(sg) = g^{-1}.dg.$$

Cela résulte de la prop. 59 (i) en prenant pour $f$ l’application constante $x \mapsto s$ de M dans G.

#### Corollaire 2 {#lie-iii-s3-prop-59-cor-2 .statement}

*Si les applications f et g de M dans G ont même différentielle gauche, l’application tangente à $fg^{-1}$ est partout nulle. Si de plus K est de caractéristique 0, alors $fg^{-1}$ est localement constante.*

On a en effet, d’après la prop. 59

$$(fg^{-1})^{-1}.d(fg^{-1}) = (\mathrm{Ad} \circ g \circ p) \circ (f^{-1}.df) - (\mathrm{Ad} \circ g \circ p) \circ (g^{-1}.dg).$$

Si $f^{-1}.df = g^{-1}.dg$, on a donc $(fg^{-1})^{-1}.d(fg^{-1}) = 0$, c’est-à-dire $T_x(fg^{-1}) = 0$ pour tout $x \in M$. Ceci prouve la première assertion. La deuxième en résulte, d’après VAR, R, 5.5.3.

#### Proposition 60 {#lie-iii-s3-prop-60 .statement}

*Soient G un groupe de Lie, de dimension finie si K est de caractéristique > 0, M une variété de classe C^r, f une application de classe C^r de M dans G, et $\alpha$ la différentielle gauche de f. On a $d\alpha + [\alpha]^2 = 0$.*

En effet, soit $\omega$ la forme différentielle gauche canonique de G. Utilisant le cor. 1 de la prop. 51, n° 14, on a

$$
d\alpha = d(f^*(\omega)) = f^*(d\omega) = f^*(-[\omega]^2)
= -[f^*(\omega)]^2 = -[\alpha]^2.
$$

### 18. Algèbre de Lie d’un groupuscule de Lie

Dans ce n°, on désigne par (G, e, θ, m) un groupuscule de Lie. Une grande partie des résultats du § sont encore valables, avec la même démonstration. Nous allons passer en revue ceux qui nous seront utiles.

18.1 Soit $\Omega$ l’ensemble de définition de $m$. Soient $(g, g') \in \Omega,\ t \in T_g^{(\infty)}(G),\ t' \in T_{g'}^{(\infty)}(G)$. Comme au n° 1, on appelle produit de convolution de $t$ et $t'$, et on note $t * t'$, l’image de $t \otimes t'$ par $m$. On pose $U(G) = T_e^{(\infty)}(G),\ U_s(G) = T_e^{(s)}(G),\ U^+(G) = T_e^{(\infty)+}(G),\ U_s^+(G) = T_e^{(s)+}(G)$. Pour $t, t'$ dans $U(G)$, $t * t'$ est défini et appartient à $U(G)$. Pour le produit de convolution, $U(G)$ est une algèbre associative, avec l’élément unité $\varepsilon_e$, filtrée par les $U_s(G)$. L’isomorphisme canonique $i_{G,e}$ de gr $U(G)$ sur $TS(T_e(G))$ est un isomorphisme d’algèbres.

18.2. Soient $G, H$ des groupuscules de Lie, $\varphi : G \to H$ un morphisme. Si $t \in U(G)$, l’image $U(\varphi)(t)$ de $t$ par $\varphi_*$ est un élément de $U(H)$, et $U(\varphi)$ est un morphisme de l’algèbre $U(G)$ dans l’algèbre $U(H)$. L’application $\theta : x \mapsto x^{-1}$ de $G$ dans $G$ définit une application $t \mapsto t^\vee$ de $U(G)$ dans $U(G)$. Pour $t, t'$ dans $U(G)$, le produit $t * t'$ calculé relativement à $G^\vee$ est égal au produit $t' * t$ calculé relativement à $G$, et $(t * t')^\vee = {t'}^\vee * t^\vee$. On a $U(\varphi)(t^\vee) = (U(\varphi)t)^\vee$. Si $G_1, \ldots, G_n$ sont des groupuscules de Lie, et $G = G_1 \times \cdots \times G_n$, l’isomorphisme canonique de $U(G_1) \otimes \cdots \otimes U(G_n)$ sur $U(G)$ est un isomorphisme d’algèbres; pour $t_1, \ldots, t_n$ dans $U(G)$, on a $(t_1 \otimes \cdots \otimes t_n)^\vee = t_1^\vee \otimes \cdots \otimes t_n^\vee$. Soient $L$ un sous-groupuscule de Lie de $G$, et $i : L \to G$ l’injection canonique. Alors $U(i)$ est un homomorphisme injectif de l’algèbre $U(H)$ dans l’algèbre $U(G)$, et $U(i)(t^\vee) = (U(i)(t))^\vee$ pour tout $t \in U(H)$. Munie du produit de convolution et du coproduit que définit la structure de variété de $G$, $U(G)$ est une bigèbre, et $U(\varphi)$ est un morphisme de bigèbres.

18.3. Soient $G$ un groupuscule de Lie, $X$ une variété de classe $C^r$, et $\psi$ un morceau de loi d’opération à gauche de classe $C^r$ de $G$ dans $X$. Soit $\Omega$ l’ensemble de définition de $\psi$. Si $t \in T_g^{(s)}(G),\ u \in T_x^{(s')}(X)$, si $(g, x) \in \Omega$ et si $s + s' \leq r$, on note $t * u$ l’image de $t \otimes u$ par $\psi_*$. Soient $t \in T_g^{(s)}(G),\ t' \in T_{g'}^{(s')}(G),\ u \in T_x^{(s'')}(X)$; si $s + s' + s'' \leq r$, et si $gg',\ (gg')x, g'x, g(g'x)$ sont définis, alors
$$
(t * t') * u = t * (t' * u).
$$
Soient $x_0 \in X$, et $\rho(x_0)$ l’application $g \mapsto gx_0$, qui est définie dans un voisinage ouvert de $e$. Si $t \in U_r(G)$, on a $\rho(x_0)_* t = t * \varepsilon_{x_0}$. Ici et dans la suite de ce n°, nous laisserons au lecteur le soin de faire les traductions pour les morceaux de lois d’opération à droite.

18.4. Conservons les notations de 18.3. Soit $t \in U_s(G)$ avec $s \leq r$. Soit $f$ une fonction de classe $C^r$ sur $X$ à valeurs dans un espace polynormé séparé. On note $t * f$ la fonction sur $X$ définie par
$$
\begin{align*}
(t * f)(x) &= \langle t, g \mapsto f(\psi(\theta(g), x)) \rangle \\
&= \langle t^\vee, f \circ \rho(x) \rangle = \langle \rho(x)_*(t^\vee), f \rangle = \langle t^\vee * \varepsilon_x, f \rangle.
\end{align*}
$$

Si $t \in U_s(G)$, $t' \in U_{s'}(G)$ et si $s + s' \leq r$, on a $\langle t', t * f \rangle = \langle t^\vee * t', f \rangle$, et $(t * t') * f = t * (t' * f)$. Soient $t \in U_s(G)$, $f$ et $f'$ des fonctions de classe $C^r$ sur $X$ à valeurs dans des espaces polynormés séparés $F$, $F'$, et $(u, u') \mapsto u . u'$ une application bilinéaire continue de $F \times F'$ dans un espace polynormé séparé; soit $\sum_{i=1}^n t_i \otimes t'_i$ l’image de $t$ par le coproduit; si $s \leq r$, on a
$$
t * (ff') = \sum_{i=1}^n (t_i * f)(t'_i * f').
$$

18.5. Conservons les notations de 18.3. Soit $t \in U_s(G)$, avec $s \leq r$. L’application $x \mapsto t * \varepsilon_x$ s’appelle le champ de distributions ponctuelles défini par $t$ et par le morceau de loi d’opération, et se note parfois $D_t^\psi$ ou $D_t$. Si $f : X \to F$ est une fonction de classe $C^r$, la fonction $t^\vee * f$ sur $X$ se note aussi $D_t f$; elle est de classe $C^{r-s}$ si $s < \infty$. Si $t \in U_s(G)$, $t' \in U_{s'}(G)$, et $s + s' \leq r$, on a $D_{t*t'} f = D_{t'}(D_t f)$. Si $G$ et $X$ sont de dimension finie, $D_t$ est un opérateur différentiel sur $X$ d’ordre $\leq s$, et de classe $C^{r-s}$ (si $s < \infty$). La fonction $D_t f$ est alors la transformée de $f$ par cet opérateur différentiel.

18.6. Soient $G$ un groupuscule de Lie, et $t \in U(G)$. On note $L_t$ le champ de distributions ponctuelles $g \mapsto \varepsilon_g * t$ sur $G$, et $R_t$ le champ de distributions ponctuelles $g \mapsto t * \varepsilon_g$ sur $G$. Si $f \in C^\omega(G, F)$, on a $L_t f \in C^\omega(G, F)$ et $R_t f \in C^\omega(G, F)$. Pour $t, t'$ dans $U(G)$, on a $L_{t*t'} = L_t \circ L_{t'}$, $R_{t*t'} = R_{t'} \circ R_t$, $L_t \circ R_{t'} = R_{t'} \circ L_t$, $\theta(L_t) = R_t^\vee$.

18.7. Comme $T_e(G)$ est l’ensemble des éléments primitifs de $U(G)$, on a $[T_e(G), T_e(G)] \subset T_e(G)$. L’espace normable $T_e(G)$, muni du crochet, est une algèbre de Lie normable, appelée algèbre de Lie normable de $G$ (ou algèbre de Lie de $G$), et notée $L(G)$. Soit $E(G)$ l’algèbre enveloppante de $L(G)$. L’injection canonique de $L(G)$ dans $U(G)$ définit un homomorphisme $\eta$ de l’algèbre $E(G)$ dans l’algèbre $U(G)$; si $K$ est de caractéristique 0, $\eta$ est un isomorphisme de bigèbres, grâce auquel on identifie $U(G)$ à $E(G)$. Reprenons les notations de 18.3. Pour tout $a \in L(G)$, soit $D_a$ le champ de distributions ponctuelles défini par $a$ sur $X$. L’application $(a, x) \mapsto D_a(x)$ est un morphisme de classe $C^{r-1}$ du fibré vectoriel trivial $L(G) \times X$ dans le fibré vectoriel $T(X)$. Soient $I$ une partie ouverte de $K$ contenant 0, et $\gamma : I \to G$ une application de classe $C^r$ telle que $\gamma(0) = e$. Soit $a = T_0(\gamma) 1 \in L(G)$. Si $f : X \to F$ est une fonction de classe $C^r$, on a
$$
(D_a f)(x) = \lim_{k \in \mathbf{K}^*, k \to 0} k^{-1}(f(\gamma(k)x) - f(x)).
$$
Si $r \geq 2$, l’application $a \mapsto D_a$ est une loi d’opération infinitésimale à gauche de classe $C^{r-1}$ de $L(G)$ dans $X$.

18.8. Soient G et H des groupuscules de Lie, $\varphi$ un morphisme de G dans H. La restriction de $U(\varphi)$ à $L(G)$, qui n’est autre que $T_e(\varphi)$, est un morphisme continu de $L(G)$ dans $L(H)$, qu’on note $L(\varphi)$. Si $\psi$ est un morphisme de H dans un groupuscule de Lie, on a $L(\psi \circ \varphi) = L(\psi) \circ L(\varphi)$. Pour que $\varphi$ soit une immersion, il faut et il suffit que $L(\varphi)$ soit un isomorphisme de $L(G)$ sur une sous-algèbre de Lie de $L(H)$ admettant un supplémentaire topologique. En particulier, si G est un sous-groupuscule de Lie de H et si $\varphi$ est l’injection canonique, on identifie $L(G)$ à une sous-algèbre de Lie de $L(H)$ grâce à $L(\varphi)$. Si $(G_i)_{i \in I}$ est une famille finie de groupuscules de Lie et G leur produit, $L(G)$ s’identifie canoniquement à $\prod_{i \in I} L(G_i)$.

18.9. Soit G un groupuscule de Lie, de dimension finie si K est de caractéristique > 0. Soit F un espace normable complet. Soit $\alpha$ une forme différentielle de degré k sur G à valeurs dans F. On dit que $\alpha$ est invariante à gauche sur G si $\alpha_g$ se déduit de $\alpha_e$ par l’application $h \mapsto gh$ d’un voisinage de e sur voisinage de g. Si $\alpha$ est invariante à gauche, $\alpha$ est analytique. L’application $\alpha \mapsto \alpha_e$ est une bijection de l’ensemble des formes différentielles de degré k sur G à valeurs dans F et invariantes à gauche sur l’ensemble des applications k-linéaires alternées continues de $T_e(G)$ dans F. Si $\alpha_e = \mathrm{Id}_{T_e(G)}$, $\alpha$ s’appelle la forme différentielle canonique gauche de G. On définit de manière analogue les formes différentielles invariantes à droite et la forme différentielle canonique droite de G. Si $\omega$ est la forme différentielle canonique gauche de G, on a $d\omega + [\omega]^2 = 0$. Soient M une variété de classe $C^r$, f une application de classe $C^r$ de M dans G. On appelle différentielle gauche de f, et on note $f^{-1}.df$, la forme différentielle de degré 1 sur M à valeurs dans $L(G)$ qui, à tout vecteur $u \in T_m(M)$, associe l’élément $f(m)^{-1}.(T_mf)(u)$. On a $f^{-1}.df = f^*(\omega)$, $d\alpha + [\alpha]^2 = 0$. Si deux applications f et g de M dans G ont même différentielle gauche, et si K est de caractéristique 0, alors $fg^{-1}$ est localement constante.

## EXERCICES {#lie-iii-s3-exercises}

See the [exercises for § 3](exercises/s3/).
