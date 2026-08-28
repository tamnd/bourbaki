---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: V
chapter_title: Groupes engendrés par des réflexions
section: 4
section_title: Représentation géométrique d’un groupe de Coxeter
lang: fr
source: lie-iv-vi-fr
pdf_pages: 0088-0101, 0129-0134
extraction: ocr
subsections:
    - "no": 1
      title: Forme associée à une matrice de Coxeter
      page: 0
      pdf_page: 88
    - "no": 2
      title: Le plan $E_{s, s'}$ et le groupe engendré par $\sigma_s$ et $\sigma_{s'}$
      page: 0
      pdf_page: 89
    - "no": 3
      title: Groupe et représentation associés à une matrice de Coxeter
      page: 0
      pdf_page: 90
    - "no": 4
      title: La représentation contragrédiente
      page: 0
      pdf_page: 91
    - "no": 5
      title: Démonstration du lemme 1
      page: 0
      pdf_page: 93
    - "no": 6
      title: Domaine fondamental de W dans la réunion des chambres
      page: 0
      pdf_page: 95
    - "no": 7
      title: Irréductibilité de la représentation géométrique d’un groupe de Coxeter
      page: 0
      pdf_page: 96
    - "no": 8
      title: Critère de finitude
      page: 0
      pdf_page: 97
    - "no": 9
      title: Cas où $B_M$ est positive et dégénérée
      page: 0
      pdf_page: 99
statements: 23
exercises: 20
content_sha256: d174f4a0062639a75e80d935a7ed7b8739343b89dd6a774962b297cb0c0e8426
---

## § 4. Représentation géométrique d’un groupe de Coxeter

Dans ce paragraphe, tous les espaces vectoriels considérés sont des espaces vectoriels réels.

### 1. Forme associée à une matrice de Coxeter

Soit S un ensemble, et soit $M = (m(s, s')_{s,s' \in S})$ une matrice de Coxeter (chap. IV, § 1, n° 9) de type S. Rappelons ce que cela signifie:
(1) Les éléments de $M$ sont des entiers ou $+\infty$.
(2) $M$ est symétrique.
(3) On a $m(s, s) = 1$ pour tout $s$.
(4) On a $m(s, s') \geqslant 2$ pour $s \neq s'$.

Soit $E = \mathbf{R}^{(s)}$, soit $(e_s)_{s \in S}$ la base canonique de $E$, et soit $B_M$ la forme bilinéaire sur $E$ telle que

$$
B_M(e_s, e_{s'}) = -\cos \frac{\pi}{m(s, s')}.
$$

La forme $B_M$ est symétrique. On dit que c’est la *forme associée* à la matrice $M$. On a

$$
B_M(e_s, e_s) = 1 \quad \text{et} \quad B_M(e_s, e_{s'}) \leq 0 \quad \text{si} \quad s \neq s'.
$$

Soit $s \in S$, et soit $f_s$ la forme linéaire $x \mapsto 2B_M(e_s, x)$. Nous noterons $\sigma_s$ la *pseudo-réflexion* définie par le couple $(e_s, f_s)$ (cf. § 2, no 1); du fait que $\langle e_s, f_s \rangle = 2$, c’est une *réflexion* (§ 2, no 2). On a

$$
\sigma_s(x) = x - 2B_M(e_s, x) \cdot e_s
$$

et en particulier

$$
\sigma_s(e_{s'}) = e_{s'} + 2 \cos \frac{\pi}{m(s, s')} \cdot e_s.
$$

Puisque $e_s$ n’est pas isotrope pour $B_M$, l’espace $E$ est somme directe de la droite $\mathbf{R} e_s$ et de l’hyperplan $H_s$ orthogonal à $e_s$. Comme $\sigma_s$ est égal à $-1$ sur $\mathbf{R} e_s$ et à $1$ sur $H_s$, il s’ensuit que $\sigma_s$ *conserve* la forme $B_M$. Lorsque $S$ est fini et $B_M$ non dégénérée (cas sur lequel on reviendra au no 8), on voit donc que $\sigma_s$ est une *réflexion orthogonale* (§ 2, no 3).

### 2. Le plan $E_{s, s'}$ et le groupe engendré par $\sigma_s$ et $\sigma_{s'}$

Dans ce numéro, on désigne par $s$ et $s'$ deux éléments de $S$, avec $s \neq s'$. On pose $m = m(s, s')$, et l’on note $E_{s, s'}$ le plan $\mathbf{R} e_s \oplus \mathbf{R} e_{s'}$.

#### Proposition 1 {#lie-v-s4-prop-1 .statement}

*La restriction de $B_M$ à $E_{s, s'}$ est positive. Elle est non dégénérée si et seulement si $m$ est fini.*

Soit $z = x e_s + y e_{s'}$, avec $x, y \in \mathbf{R}$, un élément de $E_{s, s'}$. On a

$$
B_M(z, z) = x^2 - 2xy \cos \frac{\pi}{m} + y^2
$$
$$
= (x - y \cdot \cos \frac{\pi}{m})^2 + y^2 \sin^2 \frac{\pi}{m},
$$

ce qui montre que $B_M$ est positive sur $E_{s, s'}$, et qu’elle y est non dégénérée si et seulement si $\sin \frac{\pi}{m} \neq 0$. D’où la proposition.

Les réflexions $\sigma_s$ et $\sigma_{s'}$ laissent stable $E_{s,s'}$. Nous allons déterminer l’ordre de la restriction de $\sigma_s \sigma_{s'}$ à $E_{s,s'}$. Distinguons deux cas :

a) $m = + \infty$.

Soit $u = e_s + e_{s'}$. On a $B_M(u, e_s) = B_M(u, e_{s'}) = 0$, donc $u$ est invariant par $\sigma_s$ et $\sigma_{s'}$. De plus :

$$
\sigma_s(\sigma_{s'}(e_s)) = \sigma_s(e_s + 2e_{s'}) = 3e_s + 2e_{s'} = 2u + e_s,
$$
d’où
$$
(\sigma_s \sigma_{s'})^n(e_s) = 2nu + e_s \quad \text{pour tout } n \in \mathbf{Z}.
$$

Il en résulte que la restriction de $\sigma_s \sigma_{s'}$ à $E_{s,s'}$ est d’ordre infini.

b) $m$ est fini.

La forme $B_M$ munit $E_{s,s'}$ d’une structure de plan euclidien. Puisque le produit scalaire de $e_s$ et $e_{s'}$ est égal à $- \cos \frac{\pi}{m} = \cos (\pi - \frac{\pi}{m})$, on peut orienter $E_{s,s'}$ de telle sorte que l’angle des demi-droites $R_{+e_s}$ et $R_{+e_{s'}}$ soit égal à $\pi - \frac{\pi}{m}$. Si $D$ et $D'$ désignent les droites orthogonales à $e_s$ et $e_{s'}$, on a

$$
(\overline{D'}, \overline{D}) = \pi - (\overline{D}, \overline{D'}) = \frac{\pi}{m}.
$$

Or, les restrictions $\overline{\sigma}_s$ et $\overline{\sigma}_{s'}$ de $\sigma_s$ et $\sigma_{s'}$ à $E_{s,s'}$ sont les symétries orthogonales par rapport à $D$ et $D'$. D’après le cor. de la prop. 6 du § 2, n° 5, il s’ensuit que $\overline{\sigma}_s \overline{\sigma}_{s'}$ est la rotation d’angle $\frac{2\pi}{m}$. En particulier, son ordre est $m$.

Revenons maintenant à $E$ :

#### Proposition 2 {#lie-v-s4-prop-2 .statement}

Le sous-groupe de $\mathbf{GL}(E)$ engendré par $\sigma_s$ et $\sigma_{s'}$ est un groupe diédral d’ordre $2m(s, s')$.

Comme $\sigma_s$ et $\sigma_{s'}$ sont d’ordre 2, et sont distincts, il suffit de voir que leur produit $\sigma_s \sigma_{s'}$ est d’ordre $m(s, s')$. Lorsque $m(s, s')$ est infini, cela résulte de a) ci-dessus. Lorsque $m(s, s')$ est fini, il résulte de la prop. 1 que $E$ est somme directe de $E_{s,s'}$ et de son orthogonal $V_{s,s'}$; comme $\sigma_s$ et $\sigma_{s'}$ sont l’identité dans $V_{s,s'}$, et que la restriction de $\sigma_s \sigma_{s'}$ à $E_{s,s'}$ est d’ordre $m(s, s')$ d’après b), l’ordre de $\sigma_s \sigma_{s'}$ est bien égal à $m(s, s')$.

### 3. Groupe et représentation associés à une matrice de Coxeter

Conservons les notations des numéros précédents. Soit $W = W(M)$ le groupe défini par la famille génératrice $(g_s)_{s \in S}$ et par les relations (*)

$$
(g_s g_{s'})^{m(s, s')} = 1, \quad \text{pour } s, s' \in S, \ m(s, s') \neq + \infty.
$$

#### Proposition 3 {#lie-v-s4-prop-3 .statement}

Il existe un homomorphisme et un seul

$$
\sigma : W \to \mathbf{GL}(E)
$$

(*) Cela signifie que, si $L_S$ désigne le groupe libre sur $S$, $W$ est le quotient de $L_S$ par le plus petit sous-groupe distingué de $L_S$ contenant les éléments $(ss')^{m(s, s')}$, pour $m(s, s') \neq + \infty$.

tel que $\sigma(g_s) = \sigma_s$ pour tout $s \in S$. Les éléments de $\sigma(W)$ conservent la forme bilinéaire $B_M$.

Pour prouver l’existence et l’unicité de $\sigma$, il suffit de voir que l’on a $(\sigma_s \sigma_{s'})^{m(s,s')} = 1$ si $m(s,s') \neq +\infty$. Or, si $s = s'$, cela résulte de ce que $\sigma_s$ est d’ordre 2 ; si $s \neq s'$, cela résulte de ce qui a été démontré au n° 2. Enfin, comme les réflexions $\sigma_s$ conservent $B_M$, il en est de même des éléments de $\sigma(W)$.

Remarque 1). — Nous verrons au n° 4 que $\sigma$ est injective ; le groupe W pourra donc être identifié au sous-groupe de $\mathbf{GL}(E)$ engendré par les $\sigma_s$.

#### Proposition 4 {#lie-v-s4-prop-4 .statement}

a) L’application $s \mapsto g_s$ de S dans W est injective.

b) Chacun des $g_s$ est d’ordre 2.

c) Si $s, s' \in S$, $g_sg_{s'}$ est d’ordre $m(s, s')$.

L’assertion a) résulte de ce que l’application composée

$$
s \mapsto g_s \mapsto \sigma_s
$$

de S dans $\mathbf{GL}(E)$ est injective.

Pour b) (resp. c)), on remarque que l’ordre de $g_s$ (resp. l’ordre de $g_sg_{s'}$) est au plus 2 (resp. au plus $m(s, s')$). Comme on a vu au n° 2 que l’ordre de $\sigma_s$ (resp. de $\sigma_s \sigma_{s'}$) est 2 (resp. $m(s, s')$), il y a nécessairement égalité.

Vu a), on peut identifier S à une partie de W, au moyen de l’application $s \mapsto g_s$.

#### Corollaire {#lie-v-s4-n3-cor-1 .statement}

Le couple $(W, S)$ est un système de Coxeter, de matrice M.

Cela ne fait que traduire les propriétés b) et c), ainsi que la définition de W.

Remarque 2). — Nous avons ainsi démontré que toute matrice de Coxeter correspond à un groupe de Coxeter.

### 4. La représentation contragrédiente

Soit E* le dual de E. Comme W opère sur E au moyen de $\sigma$, il opère aussi, par transport de structure, sur E*. La représentation correspondante

$$
\sigma^*: W \to \mathbf{GL}(E^*)
$$

s’appelle la représentation contragrédiente de $\sigma$. On a

$$
\sigma^*(w) = {}^t \sigma(w^{-1}) \quad \text{pour tout } w \in W.
$$

Si $x^* \in E^*$ et $w \in W$, nous noterons également $w(x^*)$ le transformé de $x^*$ par $\sigma^*(w)$.

Si $s \in S$, notons $A_s$ l’ensemble des $x^* \in E^*$ tels que $x^*(e_s) > 0$. Soit C l’intersection des $A_s$, $s \in S$. Lorsque S est fini, C est un cône simplicial ouvert de $E^*$ (§ 1, n° 6).

#### Théorème 1 (Tits) {#lie-v-s4-thm-1 .statement}

Si $w \in W$ et si $C \cap w(C) \neq \emptyset$, on a $w = 1$.
Indiquons tout de suite quelques conséquences de ce théorème:

#### Corollaire 1 {#lie-v-s4-thm-1-cor-1 .statement}

Le groupe $W$ opère de façon simplement transitive sur l’ensemble des $w(C)$ pour $w \in W$.
C’est clair.

#### Corollaire 2 {#lie-v-s4-thm-1-cor-2 .statement}

Les représentations $\sigma$ et $\sigma^*$ sont injectives.
En effet, si $\sigma^*(w) = 1$, on a $w(C) = C$, d’où $w = 1$ d’après le théorème. L’injectivité de $\sigma$ résulte de celle de $\sigma^*$.

#### Corollaire 3 {#lie-v-s4-thm-1-cor-3 .statement}

Si $S$ est fini, $\sigma(W)$ est un sous-groupe discret de $\mathbf{GL}(E)$ (muni de sa structure canonique de groupe de Lie); de même, $\sigma^*(W)$ est un sous-groupe discret de $\mathbf{GL}(E^*)$.
Soit $x^* \in C$. L’ensemble $U$ des $g \in \mathbf{GL}(E^*)$ tels que $g(x^*) \in C$ est un voisinage de l’élément neutre dans $\mathbf{GL}(E^*)$; d’après le théorème, on a
$$
\sigma^*(W) \cap U = \{1\};
$$
donc $\sigma^*(W)$ est un sous-groupe discret de $\mathbf{GL}(E^*)$. Par transport de structure, on en déduit que $\sigma(W)$ est discret dans $\mathbf{GL}(E)$.

Démonstration du théorème 1.
Si $w \in W$, notons $l(w)$ la longueur de $w$ par rapport à $S$ (chap. IV, § 1, n° 1).
Nous allons démontrer les assertions suivantes, où $n$ désigne un entier $\geqslant 0$:

(P_n) Soient $w \in W$, avec $l(w) = n$, et $s \in S$. On a alors:
ou bien $w(C) \subset A_s$;
ou bien $w(C) \subset s(A_s)$ et $l(sw) = l(w) - 1$.

(Q_n) Soient $w \in W$, avec $l(w) = n$, et $s, s' \in S, s \neq s'$. Soit $W_{s, s'}$ le sous-groupe de $W$ engendré par $s$ et $s'$. Il existe $u \in W_{s, s'}$ tel que
$$
w(C) \subset u(A_s \cap A_{s'}) \quad \text{et} \quad l(w) = l(u) + l(u^{-1}w).
$$
Ces assertions sont triviales pour $n = 0$. Nous les démontrerons par récurrence sur $n$, suivant le schéma
$$
((P_n) \text{ et } (Q_n)) \Longrightarrow (P_{n+1}) \quad \text{et} \quad ((P_{n+1}) \text{ et } (Q_n)) \Longrightarrow (Q_{n+1}).
$$

Démonstration de ((P_n) et (Q_n)) \Longrightarrow (P_{n+1}).
Soient $w \in W$, avec $l(w) = n + 1$, et $s \in S$. On peut écrire $w$ sous la forme $w = s'w'$ avec $s' \in S$ et $l(w') = n$. Si $s' = s$, (P_n) appliqué à $w'$ montre que $w'(C) \subset A_s$, d’où $w(C) \subset s(A_s)$ et l’on a bien $l(sw) = l(w') = l(w) - 1$. Si $s' \neq s$, (Q_n) appliqué à $w'$ montre qu’il existe $u \in W_{s, s'}$ tel que
$$
w'(C) \subset u(A_s \cap A_{s'}) \quad \text{et} \quad l(w') = l(u) + l(u^{-1}w').
$$
On a $w(C) = s'w'(C) \subset s'u(A_s \cap A_{s'})$.

#### Lemme 1 {#lie-v-s4-lem-1 .statement}

Soient s, s' ∈ S, avec s ≠ s' et soit v ∈ W_{s,s'}. Alors v(A_s ∩ A_{s'}) est contenu, soit dans A_s, soit dans s(A_s), et dans le second cas, on a l(sv) = l(v) — 1.

La démonstration sera donnée au n° 5.

Appliquons ce lemme à l’élément v = s’u. On a alors deux possibilités :
ou bien
$$
s'u(A_s ∩ A_{s'}) ⊂ A_s \quad \text{et} \quad \text{a fortiori} \quad w(\mathbf{C}) ⊂ A_s,
$$
ou bien
$$
s'u(A_s ∩ A_{s'}) ⊂ s(A_s) \quad \text{et} \quad \text{a fortiori} \quad w(\mathbf{C}) ⊂ s(A_s).
$$

De plus, dans le second cas, on a l(ss'u) = l(s’u) — 1. D’où :
$$
\begin{align*}
l(sw) &= l(ss'w') = l(ss'u.u^{-1}w') \leq l(ss'u) + l(u^{-1}w') \\
&= l(s'u) + l(u^{-1}w') — 1 = l(w) — 1,
\end{align*}
$$
et l’on sait que cela entraîne bien l(sw) = l(w) — 1.

*Démonstration de ((P_{n+1}) et (Q_n)) ⇒ (Q_{n+1}).*

Soient w ∈ W, avec l(w) = n + 1, et s, s' ∈ S, s ≠ s'. Si w(C) est contenu dans A_s ∩ A_{s'}, la condition (Q_{n+1}) est vérifiée en prenant u = 1. Sinon, supposons par exemple que w(C) ne soit pas contenu dans A_s. D’après (P_{n+1}), on a w(C) ⊂ s(A_s) et l(sw) = n. D’après (Q_n), appliqué à sw, il existe v ∈ W_{s,s'} tel que
$$
sw(C) ⊂ v(A_s ∩ A_{s'})
$$
et
$$
l(sw) = l(v) + l(v^{-1}sw).
$$
On a alors
$$
w(C) ⊂ sv(A_s ∩ A_{s'})
$$
et
$$
\begin{align*}
l(w) &= 1 + l(sw) = 1 + l(v) + l(v^{-1}sw) \\
&\geq l(sv) + l((sv)^{-1}w) \geq l(w),
\end{align*}
$$
et les inégalités ci-dessus sont des égalités. On en conclut que (Q_{n+1}) est vérifiée en prenant u = sv.

*Démonstration du théorème.*

Soit w ∈ W, avec w ≠ 1. On peut écrire w sous la forme sw', avec s ∈ S, et l(w') = l(w) — 1. D’après (P_n), appliqué à w' et à n = l(w'), on a w'(C) ⊂ A_s, puisque le cas w'(C) ⊂ s(A_s) est exclu du fait que l(sw') = l(w) = l(w') + 1. D’où w(C) = sw'(C) ⊂ s(A_s), et comme A_s et s(A_s) sont disjoints, on a C ∩ w(C) = ∅. C.Q.F.D.

### 5. Démonstration du lemme 1

Soit E_{s,s'}^* le dual du plan E_{s,s'} = \mathbf{R}e_s ⊕ \mathbf{R}e_{s'} (n° 2). La transposée de l’injection E_{s,s'} → E est une surjection
$$
p : E^* → E_{s,s'}^*
$$
qui commute à l’action du groupe W_{s,s'}. Il est clair que A_s, A_{s'}, et A_s ∩ A_{s'}, sont les images réciproques par $p$ des sous-ensembles correspondants de $E_{s,s'}^*$ (considéré comme espace de la représentation contragrédiente du groupe de Coxeter $W_{s,s'}$). Comme en outre la longueur d’un élément de $W_{s,s'}$ est la même par rapport à $\{s, s'\}$ et par rapport à S (chap. IV, § 1, n° 8), on voit que l’on est finalement ramené au cas où $S = \{s, s'\}$; si $m = m(s, s')$, le groupe W est alors un groupe diédral d’ordre $2m$.

Distinguons maintenant deux cas :

a) $m = + \infty$.
Soit $(\varepsilon, \varepsilon')$ la base duale de $(\ell_s, \ell_{s'})$. On a
$$
s.\varepsilon = -\varepsilon + 2\varepsilon', \quad s'.\varepsilon = \varepsilon \\
s.\varepsilon' = \varepsilon', \quad s'.\varepsilon' = 2\varepsilon - \varepsilon'.
$$

Soit D la droite affine de $E^*$ contenant $\varepsilon$ et $\varepsilon'$; les formules ci-dessus montrent que D est stable par s et $s'$ et que la restriction de s (resp. de $s'$) à D est la réflexion par rapport au point $\varepsilon'$ (resp. $\varepsilon$). Soit
$$
\theta : \mathbf{R} \to D
$$
la bijection affine $t \mapsto \theta(t) = t\varepsilon + (1-t)\varepsilon'$. Soit $I_n$ l’image par $\theta$ de l’intervalle ouvert $]n, n+1[$, et soit $C_n$ la réunion des $\lambda I_n$, pour $\lambda > 0$. On a $C_0 = C$; de plus, d’après la Remarque du § 2, n° 4, appliquée à l’espace affine D, les $I_n$ sont permutés de façon simplement transitive par W; il en est donc de même des $C_n$. Si $v \in W$, $v(C)$ est égal à l’un des $C_n$, donc est contenu dans $A_s$ si $n \geq 0$ et dans $s(A_s)$ si $n < 0$. Dans le second cas, $I_0$ et $I_n$ sont de part et d’autre du point $\varepsilon'$; d’où $l(sv) = l(v) - 1$ (loc. cit.).

b) $m$ est fini.
La forme $B_M$ est alors non dégénérée (n° 2) ce qui permet d’identifier $E^*$ à E. On a vu que l’on peut orienter E de telle sorte que les demi-droites $\mathbf{R}_{+\ell_s}$ et $\mathbf{R}_{+\ell_{s'}}$ fassent un angle égal à $\pi - \frac{\pi}{m}$.

Soit D (resp. D’) la demi-droite déduite de $\mathbf{R}_{+\ell_s}$ (resp. de $\mathbf{R}_{+\ell_{s'}}$) par une rotation de $\pi/2$ (resp. de $-\pi/2$), cf. figure 2. La chambre C est l’ensemble des $x \in E$ dont le produit scalaire avec $e_s$ et $e_{s'} > 0$; c’est le secteur angulaire ouvert d’origine D’ et d’extrémité D. D’après la Remarque du § 2, n° 5, tout élément $v$ de W transforme C en un secteur angulaire qui est, soit situé du même côté que C de D (i.e. est contenu dans $A_s$), soit situé de l’autre côté (i.e. contenu dans $s(A_s)$) et dans ce dernier cas, on a
$$
l(sv) = l(v) - 1,
$$
ce qui achève de démontrer le lemme.

![Figure 2](https://example.com/figure2.png)

FIGURE 2

### 6. Domaine fondamental de W dans la réunion des chambres

On conserve les notations du n° 4. Pour s ∈ S, on désigne par H_s l’hyperplan de E* orthogonal à e_s, par $\overline{A}_s$ l’ensemble des x* ∈ E* tels que $\langle x*, e_s \rangle \geq 0$ et par $\overline{C}$ l’intersection des $\overline{A}_s$ pour s ∈ S. Pour la topologie faible σ(E*, E) définie par la dualité entre E* et E ($Esp.\ vect.\ top.$, chap. II, 2e éd., § 6, n° 2), les $\overline{A}_s$ sont des demi-espaces fermés et $\overline{C}$ est un cône convexe fermé. De plus, $\overline{C}$ est l’adhérence de C : en effet, si x* ∈ $\overline{C}$ et y* ∈ C, on a $x* + ty* \in C$ pour tout nombre réel t > 0 et $x* = \lim_{t \to 0} (x* + ty*)$.

Pour X ⊂ S, on pose :

$$
C_X = \left( \bigcap_{s \in X} H_s \right) \cap \left( \bigcap_{s \in S - X} A_s \right).
$$

On a $C_X \subset \overline{C}$, $C_\emptyset = C$ et $C_S = \{0\}$. Les ensembles $C_X$, pour $X \in \mathfrak{P}(S)$, forment une partition de $\overline{C}$.

Rappelons d’autre part (chap. IV, § 1, n° 8) que l’on désigne par $W_X$ le sous-groupe de W engendré par X. On a évidemment $w(x*) = x*$ pour $w \in W_X$ et $x* \in C_X$.

#### Proposition 5 {#lie-v-s4-prop-5 .statement}

Soient X, $X' \subset S$ et $w, w' \in W$. Si $w(C_X) \cap w'(C_{X'}) \neq \varnothing$, alors on a $X = X'$, $wW_X = w'W_{X'}$ et $w(C_X) = w'(C_{X'})$.

On se ramène aussitôt au cas $w' = 1$. Nous ferons alors la démonstration par récurrence sur la longueur n de w. Si $n = 0$, l’assertion est évidente. Si $l(w) > 0$, il existe un s ∈ S tel que $l(sw) = l(w) - 1$ et on a alors (cf. fin du n° 4) $w(C) \subset s(A_s)$, d’où $w(\overline{C}) \subset s(\overline{A}_s)$. Comme $\overline{C} \subset \overline{A}_s$, il en résulte que

$$
\overline{C} \cap w(\overline{C}) \subset H_s.
$$

On a donc $s(x*) = x*$ pour tout $x* \in \overline{C} \cap w(\overline{C})$ et a fortiori pour tout

$$
x* \in C_{X'} \cap w(C_X).
$$

Par suite, la relation $C_{X'} \cap w(C_X) \neq \varnothing$ entraîne d’une part $C_{X'} \cap H_s \neq \varnothing$, d’où $s \in X'$, d’autre part $C_{X'} \cap sw(C_X) \neq \varnothing$. L’hypothèse de récurrence entraîne alors que $X = X'$ et $swW_X = W_{X'} = W_X$, d’où $sw \in W_X$ et $w \in W_X$ puisque $s \in W_X$. Il en résulte que $wW_X = W_{X'}$ et que $w(C_X) = C_X = C_{X'}$.

#### Corollaire {#lie-v-s4-n6-cor-1 .statement}

Soient X une partie de S et x* un élément de C_X. Le stabilisateur de x* dans W est W_X.

Soit maintenant U la réunion des $w(\overline{C})$ pour $w \in W$, et soit $\mathfrak{F}$ l’ensemble des parties de U de la forme $w(C_X)$, avec $X \subset S$ et $w \in W$. Vu ce qui précède, $\mathfrak{F}$ est une partition de U.

#### Proposition 6 {#lie-v-s4-prop-6 .statement}

(i) Le cône U est convexe.
(ii) Tout segment fermé contenu dans U ne rencontre qu’un nombre fini d’éléments de $\mathfrak{F}$.
(iii) Le cône $\overline{C}$ est un domaine fondamental de W opérant dans U.

Pour prouver (iii), il suffit de montrer que si $x^*, y^* \in \overline{C}$ et $w \in W$ sont tels que $w(x^*) = y^*$, on a $x^* = y^*$. Or il existe deux parties X et Y de S telles que $x^* \in C_X$ et $y^* \in C_Y$; on a $w(C_X) \cap C_Y \neq \emptyset$, et la prop. 5 montre que $X = Y$ et $w \in W_X$, ce qui entraîne bien $x^* = y^*$.

Soient maintenant $x^*, y^* \in U$, et montrons que le segment fermé $[x^*y^*]$ est recouvert par un nombre fini d’éléments de $\mathfrak{F}$, ce qui établira à la fois (i) et (ii). Quitte à transformer $x^*$ et $y^*$ par un même élément de W, on peut supposer que $x^* \in \overline{C}$. Soit $w \in W$ tel que $y^* \in w(\overline{C})$. Nous allons raisonner par récurrence sur la longueur de $w$. Pour $s \in S$, la relation $w(\overline{C}) \subset \overline{A}_s$ est équivalente à $w(C) \subset A_s$ et par suite à $l(sw) < l(w)$ (cf. n° 4). La prop. 7 du n° 8 du chap. IV, § 1, entraîne donc qu’il n’existe qu’un nombre fini de $s \in S$ tels que $w(\overline{C}) \subset \overline{A}_s$. L’ensemble T des $s \in S$ tels que $\langle y^*, e_s \rangle < 0$ est donc fini. D’autre part, l’intersection $\overline{C} \cap [x^*y^*]$ est un segment fermé $[x^*z^*]$. Si $z^* = y^*$, c’est-à-dire si $y^* \in \overline{C}$, il existe des parties X et Y de S telles que $x^* \in C_X$ et $y^* \in C_Y$. Le segment ouvert $]x^*y^*[$ est alors contenu dans $C_{X \cap Y}$, d’où $[x^*y^*] \subset C_X \cup C_Y \cup C_{X \cap Y}$. Si $z^* \neq y^*$, il existe un $s \in T$ tel que $z^* \in H_s$. On a alors $w(C) \subset A_s$ et $l(sw) < l(w)$. L’hypothèse de récurrence entraîne donc que le segment $[z^*y^*] = s([z^*(sw(y^*))])$ est recouvert par un nombre fini d’éléments de $\mathfrak{F}$, donc aussi

$$
[x^*y^*] = [x^*z^*] \cup [z^*y^*]
$$

puisque $[x^*z^*] \subset \overline{C}$.

### 7. Irréductibilité de la représentation géométrique d’un groupe de Coxeter

On conserve les notations des n°s précédents, et l’on suppose que S est fini.

#### Proposition 7 {#lie-v-s4-prop-7 .statement}

Supposons que $(W, S)$ soit irréductible (chap. IV, § 1, n° 9). Soit $E^0$ le sous-espace de E orthogonal à E vis-à-vis de $B_M$. Le groupe W opère trivialement sur $E^0$, et tout sous-espace de E, distinct de E et stable par W, est contenu dans $E^0$.

Si $x \in E^0$, on a $\sigma_s(x) = x - 2B_M(e_s, x)e_s = x$ pour tout $s \in S$. Comme W est engendré par S, il en résulte bien que W opère trivialement sur $E^0$.

Soit $E'$ un sous-espace de E stable par W. Soient $s, s' \in S$ deux éléments liés dans le graphe $\Gamma$ de $(W, S)$ (chap. IV, § 1, n° 9); rappelons que cela signifie que $m(s, s') \geq 3$. Supposons que $e_s \in E'$. On a alors $\sigma_{s'}(e_s) \in E'$ et comme le coefficient de $e_{s'}$ dans $\sigma_{s'}(e_s)$ est non nul, on a $e_{s'} \in E'$. Comme $\Gamma$ est connexe, il s’ensuit que, si $E'$ contient l’un des $e_s$, il les contient tous et coïncide avec E. Ce cas étant écarté, il résulte de la prop. 3 du § 2, n° 2 que, pour tout $s \in S$, $E'$ est contenu dans l’hyperplan $H_s$ orthogonal à $e_s$. Comme l’intersection des $H_s$ est égale à $E^0$, cela démontre la proposition.

#### Corollaire {#lie-v-s4-n7-cor-1 .statement}

Supposons que $(W, S)$ soit irréductible. Alors:
a) Si $B_M$ est non dégénérée, le $W$-module $E$ est absolument simple.
b) Si $B_M$ est dégénérée, le $W$-module $E$ n’est pas semi-simple.
Dans le cas a), la prop. 7 montre que $E$ est simple, donc aussi absolument simple ($\S 2$, no 1, prop. 1).
Dans le cas b), on a $E^0 \neq 0$, $E \neq E^0$ (puisque $B_M \neq 0$), et la prop. 7 montre que $E^0$ n’admet pas de supplémentaire stable par $W$; le $W$-module $E$ n’est donc pas semi-simple.

### 8. Critère de finitude

On conserve les notations des nos précédents, et l’on suppose que $S$ est fini.

#### Théorème 2 {#lie-v-s4-thm-2 .statement}

Les propriétés suivantes sont équivalentes :
(1) $W$ est fini.
(2) La forme $B_M$ est positive non dégénérée.
(1) $\Longrightarrow$ (2). Soit $S = \bigcup_i S_i$ la décomposition de $S$ en composantes connexes (chap. IV, $\S 1$, no 9), et soit $W = \prod_i W_i$ la décomposition correspondante de $W$. L’espace $E$ s’identifie à la somme directe des espaces $E_i = \mathbf{R}^{s_i}$, et $B_M$ s’identifie à la somme directe des formes $B_{M_i}$ correspondantes. On est donc ramené au cas où $(W, S)$ est irréductible. Comme $W$ est supposé fini, $E$ est un $W$-module semi-simple (Annexe, prop. 2). D’après le cor. de la prop. 5, il s’ensuit que $E$ est absolument simple. Soit alors $B'$ une forme positive non dégénérée sur $E$, et soit $B''$ la somme de ses transformées par $W$. Puisque $B''$ est invariante par $W$, elle est proportionnelle à $B_M$ ($\S 2$, no 1, prop. 1); du fait que $B_M(e_s, e_s) = 1$ pour tout $s \in S$, le coefficient de proportionnalité est $> 0$, et, comme $B''$ est positive, il en est de même de $B_M$, ce qui démontre (2).
(2) $\Longrightarrow$ (1). Si $B_M$ est positive non dégénérée, le groupe orthogonal $O(B_M)$ est compact (Intégr., chap. VII, $\S 3$, no 1). Comme $\sigma(W)$ est un sous-groupe discret de $O(B_M^-)$ (cor. 3 du th. 1), il s’ensuit que $\sigma(W)$ est fini, donc aussi $W$.
C.Q.F.D.

Le résultat suivant a été prouvé en cours de démonstration :

#### Corollaire {#lie-v-s4-n8-cor-1 .statement}

Si $(W, S)$ est irréductible et fini, $E$ est un $W$-module absolument simple.
Le critère fourni par le th. 2 permet de classifier tous les groupes de Coxeter finis (cf. chap. VI, $\S 4$). Bornons-nous ici à un résultat préliminaire :

#### Proposition 8 {#lie-v-s4-prop-8 .statement}

Si $W$ est fini, le graphe de $(W, S)$ est une forêt (chap. IV, Annexe).
Sinon, ce graphe contiendrait un circuit $(s_1, \ldots, s_n)$, $n \geqslant 3$. Si l’on pose $m_i = m(s_i, s_{i+1})$, $1 \leqslant i < n$, et $m_n = m(s_n, s_1)$, cela signifie que l’on a $m_i \geqslant 3$ pour tout $i$. Soit
$$
x = e_{s_1} + \cdots + e_{s_n}.
$$

On a $B_M(x, x) = n + 2 \sum_{i < j} B_M(e_{s_i}, e_{s_j})$. Or
$$
B_M(e_{s_i}, e_{s_{i+1}}) = -\cos \frac{\pi}{m_i} \leq -\cos \frac{\pi}{3} \leq -\frac{1}{2} (*),
$$
et de même pour $B_M(e_{s_n}, e_{s_1})$. Comme les autres termes de la somme ci-dessus sont $\leq 0$, on obtient
$$
B_M(x, x) \leq n - n = 0.
$$
contrairement au fait que $B_M$ est positive non dégénérée.

#### Corollaire {#lie-v-s4-n8-cor-2 .statement}

Si $(W, S)$ est irréductible et fini, son graphe est un arbre.
En effet, une forêt connexe est un arbre.

Comparaison avec les résultats du § 3.
Soit tout d’abord $(W, S)$ un groupe de Coxeter fini. Notons $(x|y)$ la forme $B_M(x, y)$; d’après le th. 2, c’est un produit scalaire sur $E$. Pour tout $s \in S$, soit $H_s$ l’hyperplan associé à la réflexion orthogonale $\sigma_s$, et soit $\mathcal{H}$ la famille des hyperplans $w(H_s)$, pour $s \in S, w \in W$. Soit $C_0$ l’ensemble des $x \in E$ tels que $(x|e_s) > 0$ pour tout $s \in S$. Enfin, identifions $W$ (au moyen de $\sigma$) à un sous-groupe du groupe orthogonal $\mathbf{O}(E)$ de l’espace $E$.

#### Proposition 9 {#lie-v-s4-prop-9 .statement}

Avec les notations précédentes, $W$ est le sous-groupe de $\mathbf{O}(E)$ engendré par les réflexions par rapport aux hyperplans de $\mathcal{H}$. C’est un groupe essentiel ($\S 3, \mathrm{n}^\circ 7$) et $C_0$ est une chambre de $E$ relativement à $\mathcal{H}$.

La première assertion est triviale. D’autre part, si $x \in E$ est invariant par $W$, il est orthogonal à tous les $e_s$, donc nul; cela montre que $W$ est essentiel. Enfin, l’isomorphisme $E \to E^*$ défini par $B_M$ transforme $C_0$ en l’ensemble $C$ du $\mathrm{n}^\circ 4$; la propriété (P_n) démontrée à cet endroit prouve que, pour tout $w \in W$, et tout $s \in S$, $w(C_0)$ ne rencontre pas $H_s$. On en conclut que $C_0$ est contenu dans le complémentaire $U$ de la réunion des hyperplans de $\mathcal{H}$, et comme $C_0$ est connexe, ouvert et fermé dans $U$, c’est une chambre de $E$ relativement à $\mathcal{H}$, C.Q.F.D.

On peut donc appliquer à $W$ et $C_0$ toutes les propriétés démontrées au $\S 3$. En

(*) Les racines de l’équation $z^3 - 1 = 0$ sont 1 et $\frac{-1 \pm i \sqrt{3}}{2}$. Donc $\cos \frac{2\pi}{3} = -\frac{1}{2}$ et par suite $\cos \frac{\pi}{3} = \frac{1}{2}$. Notons à cette occasion que $\sin \frac{2\pi}{3} = \frac{\sqrt{3}}{2}$, d’où
$$
\sin \frac{\pi}{3} = \frac{\sqrt{3}}{2}, \quad \cos \frac{\pi}{6} = -\cos \frac{5\pi}{6} = \frac{\sqrt{3}}{2}, \quad \sin \frac{\pi}{6} = \sin \frac{5\pi}{6} = \frac{1}{2}.
$$
De même, les racines de l’équation $z^2 - i = 0$ sont $\pm \frac{1+i}{\sqrt{2}}$, d’où
$$
\cos \frac{\pi}{4} = \sin \frac{\pi}{4} = \frac{\sqrt{2}}{2} \quad \text{et par suite} \quad \sin \frac{3\pi}{4} = -\cos \frac{3\pi}{4} = \frac{\sqrt{2}}{2}.
$$

particulier, $\overline{C}_0$ est un *domaine fondamental* pour l’action de W sur E (en d’autres termes, le cône U défini au n° 6 est égal à E tout entier).

Inversement, soit E un espace vectoriel réel de dimension finie, muni d’un produit scalaire $(x|y)$ et soit W un groupe fini essentiel de déplacements de E laissant 0 fixe; supposons W *engendré par des réflexions*. Soit $C_0$ une chambre de E par rapport à W (cf. § 3), et soit S l’ensemble des réflexions orthogonales relativement aux murs de $C_0$. Alors (W, S) est un *système de Coxeter fini* ($\S 3, n° 2, th. 1$). De plus, si $s \in S$, notons $H_s$ le mur de $C_0$ correspondant à s, et notons $e_s$ le vecteur unitaire orthogonal à $H_s$ et situé du même côté que $C_0$ de $H_s$. Si $(m(s, s'))$ désigne la matrice de Coxeter de (W, S), les prop. 3 et 7 du § 3 montrent que

$$
(e_s|e_{s'}) = -\cos (\pi/m(s, s'))
$$

et que les $e_s$ forment une base de E. *La représentation naturelle de W dans E s’identifie donc à la représentation $\sigma$ du n° 3*.

### 9. Cas où $B_M$ est positive et dégénérée

Dans ce numéro, nous supposons que S est fini, que (W, S) est *irréductible*, et que la forme $B_M$ est *positive et dégénérée*.

#### Lemme 2 {#lie-v-s4-lem-2 .statement}

*L’orthogonal $E^0$ de E pour $B_M$ est de dimension 1 ; il est engendré par un élément $v = \sum_{s \in S} v_s e_s$, avec $v_s > 0$ pour tout s.*

Cela résulte du lemme 4 du § 3, n° 5, appliqué à la matrice des $B_M(e_s, e_{s'})$.

Soit $v = \sum_s v_s e_s$ le vecteur satisfaisant aux conditions du lemme 2, tel que $\sum_s v_s = 1$ et soit A l’hyperplan affine de $E^*$ formé des $y^* \in E^*$ tels que $\langle v, y^* \rangle = 1$. Si T désigne l’orthogonal de v dans $E^*$, A est muni de façon naturelle d’une structure d’espace affine d’espace de translations T. De plus, la forme $B_M$ définit par passage au quotient un produit scalaire non dégénéré sur $E/E^0$, donc aussi sur son dual T ; d’où une *structure euclidienne* sur l’espace affine A (*Alg.*, chap. IX, § 6, n° 6).

Soit G le sous-groupe de $\mathbf{GL}(E)$ formé des automorphismes laissant invariants v et $B_M$; si $g \in G$, le contragrédient $^tg^{-1}$ laisse stables A et T, et définit par restriction à A un *déplacement i(g)* de A (cf. § 3). Il est immédiat que l’on obtient ainsi un *isomorphisme* de G sur le groupe des déplacements de A. De plus le stabilisateur $G_a$ d’un point a de A s’identifie au groupe orthogonal de l’espace hilbertien T et est donc *compact*. Par ailleurs, G est un groupe localement compact dénombrable à l’infini et A est un espace de Baire : il s’ensuit (*Integr.*, chap. VII, Appendice, lemme 2) que l’application $\psi : g \mapsto g(a)$ définit un homéomorphisme de $G/G_a$ sur A. Donc G *opère proprement sur A* (*Top. gén.*, chap. III, 3e éd., § 4, n° 2, cor. de la prop. 5). Puisque W est un sous-groupe de G, il s’identifie à un groupe de déplacements de A. Nous allons voir que ce groupe satisfait aux hypothèses du § 3. Plus précisément :

#### Proposition 10 {#lie-v-s4-prop-10 .statement}

Le groupe W muni de la topologie discrète opère proprement sur A ; il est engendré par des réflexions orthogonales ; il est infini, irréductible et essentiel (§ 3, no 7). L’intersection C ∩ A est une chambre de A pour W. Si l’on désigne par L_s l’hyperplan de A intersection de A avec l’hyperplan de E* orthogonal à e_s, les L_s pour s ∈ S forment la famille des murs de C ∩ A. Si ε_s est le vecteur unitaire de T orthogonal à L_s situé du même côté que C ∩ A de L_s, on a $(\varepsilon_s|\varepsilon_t) = -\cos(\pi/m(s, t))$ (pour s, t ∈ S) et la matrice de Coxeter de W (§ 3, no 4) s’identifie à M.

D’après le cor. 3 du th. 1, W est discret dans GL(E), donc dans G et opère proprement dans A. Soit s ∈ S. Comme Card S ≥ 2, l’hyperplan de E* orthogonal à e_s n’est pas orthogonal à v et son intersection L_s avec A est bien un hyperplan. Le déplacement correspondant à s est donc un déplacement d’ordre 2 laissant fixes tous les points de L_s : c’est nécessairement la réflexion orthogonale associée à L_s. Il en résulte que W est bien engendré par des réflexions orthogonales. Le th. 2 montre alors que W est infini et la prop. 7 qu’il est essentiel et irréductible.

Comme C est un cône simplicial ouvert, ayant pour murs les hyperplans d’équations $\langle x^*, e_s \rangle = 0$ (pour s ∈ S), l’intersection C ∩ A est une partie convexe, donc connexe, ouverte et fermée du complémentaire de la réunion des L_s dans A. De plus C ∩ A est non vide, car si x* ∈ C, on a $\langle x^*, v \rangle = \sum_s v_s \langle x^*, e_s \rangle > 0$ et $\langle x^*, v \rangle^{-1} x^* \in C \cap A$. Il en résulte que C ∩ A est une chambre de A relativement au système des L_s. De plus, on a w(C ∩ A) ∩ L_s = ∅ pour tout w ∈ W (cf. no 4, propriété (P_n)) et il en résulte que C ∩ A est une chambre de A relativement au système formé des transformés des L_s par tous les éléments de W ; d’après le cor. du th. 1 du § 3, no 2, il en résulte que C ∩ A est une chambre de A relative à W.

Soit alors a_s^* le sommet du simplexe C ∩ A non situé dans L_s. On a

$$
\langle a_s^*, e_t \rangle = 0
$$

pour s, t ∈ S et s ≠ t, et

$$
\langle a_s^*, e_s \rangle = v_s^{-1} \langle a_s^*, v \rangle = v_s^{-1}.
$$

Soit ε_s le vecteur de T défini par les relations :

$$
(\varepsilon_s|a_s^* - a_t^*) = v_s^{-1} \quad \text{pour} \quad t \in S, t \neq s.
$$

Le vecteur ε_s est orthogonal à L_s et est situé du même côté que C ∩ A de l’hyperplan L_s. On a de plus :

$$
(\varepsilon_s|a_s^* - a_t^*) = \langle e_s, a_s^* - a_t^* \rangle \quad \text{quels que soient} \ s, t \in S
$$

ce qui montre que ε_s est l’image de la classe de e_s par l’isomorphisme de

E/E^0 sur T déduit de la forme quadratique B_M. Il en résulte que

$$(\varepsilon_s|\varepsilon_t) = B_M(e_s, e_t).$$

Par suite $\varepsilon_s$ est bien un vecteur unitaire et la dernière assertion de la prop. 10 est démontrée.

Nous dirons que l’espace affine euclidien A muni du groupe W est l’espace associé à la matrice de Coxeter M et nous le noterons $A_M$.

La proposition 10 admet une réciproque:

#### Proposition 11 {#lie-v-s4-prop-11 .statement}

*Soit W un groupe de déplacements d’un espace affine euclidien A, satisfaisant aux hypothèses du § 3. On suppose que W est infini, essentiel et irréductible. Alors la forme $B_M$ attachée à la matrice de Coxeter M de W est positive dégénérée et il existe un isomorphisme et un seul de l’espace affine $A_M$ associé à M sur A, commutant à l’action de W. Cet isomorphisme transforme le produit scalaire de $A_M$ en un multiple du produit scalaire de A.*

Soit $C_0$ une chambre de A et soit S l’ensemble des réflexions orthogonales par rapport aux murs de $C_0$. Si $\eta_s$ désigne le vecteur unitaire orthogonal à l’hyperplan $N_s$ associé à la réflexion s, situé du même côté que $C_0$ de $N_s$ ($\S$ 3, prop. 3), la forme $B_M$ est telle que $B_M(e_s, e_t) = (\eta_s|\eta_t)$ pour $s, t \in S$. Elle est donc *positive*. Comme les $\eta_s$ sont linéairement dépendants ($\S$ 3, no 9, prop. 8), elle est *dégénérée*.

On peut donc appliquer à $M$ les constructions précédentes. Avec les mêmes notations que ci-dessus, on a $(\varepsilon_s|\varepsilon_t) = (\eta_s|\eta_t)$ et il existe un isomorphisme $\varphi$ d’espaces hilbertiens et un seul de T sur l’espace des translations de A tel que $\varphi(\varepsilon_s) = \eta_s$. Soient $a$ et $b$ deux sommets distincts de $C_0$ et $s_0$ la réflexion de S telle que $a \notin N_{s_0}$. Posons $\lambda = (\eta_{s_0}|a - b)$ et soit $\psi$ la bijection affine de $A_M$ sur A définie par:

$$
\psi(a_{s_0} + x) = a + v_{s_0} \lambda \varphi(x) \quad \text{pour } x \in T.
$$

Il est alors immédiat que $\psi(L_s) = N_s$ pour tout $s \in S$ et que $\psi$ transforme le produit scalaire de $A_M$ en un multiple de celui de A. On en déduit aussitôt que $\psi$ commute à l’action de W. Enfin, l’unicité de $\psi$ est évidente, car $a_s$ par exemple est l’unique point de $A_M$ invariant par les réflexions $t \in S, \ t \neq s$.

## EXERCICES {#lie-v-s4-exercises}

Dans les exercices ci-dessous, (W, S) désigne un système de Coxeter. On suppose S fini; son cardinal est appelé le rang de (W, S). On identifie W à un sous-groupe de $\mathbf{GL}(E)$ au moyen de $\sigma$ (cf. n°s 3 et 4).

See the [exercises for § 4](exercises/s4/).
