---
book: alg
book_title: Algebra
chapter: IV
chapter_title: Polynômes et fractions rationnelles
section: 5
section_title: TENSEURS SYMÉTRIQUES ET APPLICATIONS POLYNOMIALES
lang: fr
source: alg-iv-vii-fr
book_pages: A IV.39-A IV.57, A IV.87-A IV.92
pdf_pages: 0046-0064, 0094-0099
extraction: ocr
subsections:
    - "no": 1
      title: Traces relatives
      page: 39
      pdf_page: 46
    - "no": 2
      title: Définition des tenseurs symétriques
      page: 40
      pdf_page: 47
    - "no": 3
      title: Produit dans les tenseurs symétriques
      page: 41
      pdf_page: 48
    - "no": 4
      title: Puissances divisées
      page: 42
      pdf_page: 49
    - "no": 5
      title: Tenseurs symétriques sur un module libre
      page: 44
      pdf_page: 51
    - "no": 6
      title: Le foncteur $TS$
      page: 45
      pdf_page: 52
    - "no": 7
      title: Coproduit dans les tenseurs symétriques
      page: 47
      pdf_page: 54
    - "no": 8
      title: Relations entre $TS(M)$ et $S(M)$
      page: 49
      pdf_page: 56
    - "no": 9
      title: Applications polynomiales homogènes
      page: 51
      pdf_page: 58
    - "no": 10
      title: Applications polynomiales
      page: 54
      pdf_page: 61
    - "no": 11
      title: Relations entre $S(M^*)$, $TS(M)^{*gr}$ et $Pol(M, A)$
      page: 56
      pdf_page: 63
statements: 37
exercises: 16
content_sha256: 436be7555b6615cd1e246da18dd676adabf926d4b4c53dec6a5b23c4c066abd8
---

## § 5. TENSEURS SYMÉTRIQUES ET APPLICATIONS POLYNOMIALES

### 1. Traces relatives

Soient H un groupe, M un $A[H]$-module à gauche $^1$. Nous noterons $M^H$ l’ensemble des $m \in M$ tels que $hm = m$ pour tout $h \in H$ $^2$; c’est un sous-A-module de M.
Soit G un sous-groupe de H. Alors $M^G$ est un sous-A-module de M contenant $M^H$.
Soient $m \in M^G$, $h \in H$, et $x = hG$ la classe à gauche de $h$ suivant G. On a $xm = hGm = \{hm\}$. Par abus de notation, l’élément $hm$ de M sera noté $xm$. Si $h' \in H$, on a

$$(1)$$
$$h'(xm) = (h'x)m.$$

Supposons désormais que G soit d’indice fini dans H. Alors

$$(2)$$
$$\sum_{x \in H/G} xm \in M^H.$$

En effet, pour tout $h' \in H$, on a, compte tenu de (1),

$$
h'\left( \sum_{x \in H/G} xm \right) = \sum_{x \in H/G} (h'x)m = \sum_{y \in H/G} ym.
$$

$^1$ On a noté $A[H]$ l’algèbre du groupe H (III, p. 19).
$^2$ On prendra garde de ne pas confondre cette notation avec celle qu’on a introduite dans l’étude des produits d’ensembles (E, II, p. 31).

#### Définition 1 {#alg-iv-s5-def-1 .statement}

Si G est d’indice fini dans H, on note Tr_{H/G} l’application de M^G dans M^H définie par :

(3) $$ \operatorname{Tr}_{H/G} m = \sum_{x \in H/G} x m . $$

Cette application est un homomorphisme du A-module M^G dans le A-module M^H.

#### Proposition 1 {#alg-iv-s5-prop-1 .statement}

(i) Soient m \in M^G et h \in H. Alors hm \in M^{hGh^{-1}} et

$$ \operatorname{Tr}_{H/hGh^{-1}}(hm) = \operatorname{Tr}_{H/G} m . $$

(ii) Soit F un sous-groupe de G d’indice fini dans G. Soit m \in M^F. Alors

$$ \operatorname{Tr}_{H/G}(\operatorname{Tr}_{G/F} m) = \operatorname{Tr}_{H/F} m . $$

(iii) Si m \in M^H, on a \operatorname{Tr}_{H/G} m = (H : G) m.

(i) Soit h \in H. Pour h' \in H et m \in M, posons \varphi(h') = hh'h^{-1} et \psi(m) = hm. On a \varphi(h') \psi(m) = \psi(h'm). Par transport de structure, on en déduit que, si m \in M^G, on a hm \in M^{hGh^{-1}} et

$$ \operatorname{Tr}_{H/hGh^{-1}}(hm) = \psi(\operatorname{Tr}_{H/G}(m)) . $$

Comme \operatorname{Tr}_{H/G}(m) \in M^H, cela prouve (i).

(ii) Soit m \in M^F. Soit (g_\alpha)_{\alpha \in A} un système de représentants des classes à gauche de G suivant F. Soit (h_\beta)_{\beta \in B} un système de représentants des classes à gauche de H suivant G. Alors (h_\beta g_\alpha)_{(\beta, \alpha) \in B \times A} est un système de représentants des classes à gauche de H suivant F, donc

$$ \operatorname{Tr}_{H/G}(\operatorname{Tr}_{G/F} m) = \sum_{\beta \in B} h_\beta (\sum_{\alpha \in A} g_\alpha m ) $$
$$ = \sum_{(\beta, \alpha) \in B \times A} (h_\beta g_\alpha) m = \operatorname{Tr}_{H/F} m . $$

(iii) L’assertion est évidente.

### 2. Définition des tenseurs symétriques

Soit M un A-module. Rappelons (III, p. 71) que \mathfrak{S}_n opère à gauche dans le A-module T^n(M), de telle sorte que

$$ \sigma(x_1 \otimes x_2 \otimes \ldots \otimes x_n) = x_{\sigma^{-1}(1)} \otimes x_{\sigma^{-1}(2)} \otimes \ldots \otimes x_{\sigma^{-1}(n)} $$

quels que soient x_1, ..., x_n \in M et \sigma \in \mathfrak{S}_n. Les éléments z de T^n(M) tels que \sigma.z = z pour tout \sigma \in \mathfrak{S}_n sont appelés tenseurs symétriques d’ordre n ; ils forment un sous-A-module de T^n(M) noté TS^n(M) ; on a TS^0(M) = A, TS^1(M) = M. On pose TS(M) = \bigoplus_{n=0}^\infty TS^n(M) ; c’est un sous-A-module gradué de T(M). Pour tout z \in T^nM, l’élément $\sum_{\sigma \in S_n} \sigma . z$ appartient à $TS^n(M)$; on le note $s.z$, et on dit que $s.z$ est le symétrisé de $z$. L’application $s : z \mapsto s.z$ est un homomorphisme du A-module $T^n(M)$ dans le A-module $TS^n(M)$. Si $z \in TS^n(M)$, on a $s.z = n!z$.

### 3. Produit dans les tenseurs symétriques

Soient $p, q \in \mathbf{N}$. Soit $S_{p|q}$ le sous-groupe de $S_{p+q}$ formé des permutations $\sigma \in S_{p+q}$ qui laissent stables les intervalles $(1, p)$ et $(p+1, p+q)$ de $\mathbf{N}$. Si $\sigma \in S_p$ et $\sigma' \in S_q$, on définit un élément $\sigma''$ de $S_{p|q}$ en posant $\sigma''(n) = \sigma(n)$ pour $1 \leq n \leq p$ et $\sigma''(p+n) = p + \sigma'(n)$ pour $1 \leq n \leq q$; l’application $(\sigma, \sigma') \mapsto \sigma''$ est un isomorphisme de $S_p \times S_q$ sur $S_{p|q}$.

Soient $z \in TS^p(M)$, $z' \in TS^q(M)$. Alors l’élément $z \otimes z'$ de $T^{p+q}(M)$ est invariant par $S_{p|q}$. On peut donc définir l’élément $\mathrm{Tr}_{S_{p+q}/S_{p|q}}(z \otimes z')$ de $TS^{p+q}(M)$. Nous munirons $TS(M)$ de la multiplication A-bilinéaire $(y, y') \mapsto yy'$ telle que, pour $p, q \in \mathbf{N}$, $z \in TS^p(M)$, $z' \in TS^q(M)$, on ait

$$
zz' = \mathrm{Tr}_{S_{p+q}/S_{p|q}}(z \otimes z')
$$

Si $y \in TS(M)$ et $y' \in TS(M)$, on dit que $yy'$ est le produit symétrique de $y$ et $y'$. La famille $(TS^p(M))_{p \in \mathbf{N}}$ est une graduation de type $\mathbf{N}$ de l’algèbre $TS(M)$. L’élément unité de $T(M)$ est un élément unité de $TS(M)$.

Soit $S_{p,q}$ l’ensemble des $\sigma \in S_{p+q}$ tels que

$$
\begin{align*}
&\sigma(1) < \sigma(2) < ... < \sigma(p) \\
&\sigma(p+1) < \sigma(p+2) < ... < \sigma(p+q)
\end{align*}
$$

L’application $(\sigma, \tau) \mapsto \sigma \tau$ de $S_{p,q} \times S_{p|q}$ dans $S_{p+q}$ est bijective (I, p. 57, Example 2); donc, si $z \in TS^p(M)$ et $z' \in TS^q(M)$, on a

$$
zz' = \sum_{\sigma \in S_{p,q}} \sigma(z \otimes z')
$$

#### Proposition 2 {#alg-iv-s5-prop-2 .statement}

(i) *La A-algèbre $TS(M)$ est associative, commutative et unifère.*

(ii) *Soient $p_1, ..., p_n$ des entiers $> 0$. Soit $S_{p_1|...|p_n}$ l’ensemble des $\sigma \in S_{p_1+\cdots+p_n}$ qui laissent stables les intervalles :

$$
(1, p_1), (p_1+1, p_1+p_2), ..., (p_1+\cdots+p_{n-1}+1, p_1+\cdots+p_n)
$$

de $\mathbf{N}$. *Soient $z_1 \in TS^{p_1}(M), ..., z_n \in TS^{p_n}(M)$. Alors*

$$
z_1 z_2 ... z_n = \mathrm{Tr}_{S_{p_1+\cdots+p_n}/S_{p_1|...|p_n}}(z_1 \otimes z_2 \otimes ... \otimes z_n)
$$

*En particulier, si $x_1, ..., x_n \in M$, on a $x_1 ... x_n = s(x_1 \otimes ... \otimes x_n)$.*

L’assertion (ii) est évidente pour $n = 1$. Supposons démontrée la relation

$$
z_2 ... z_n = \mathrm{Tr}_{S_{p_2+\cdots+p_n}/S_{p_2|...|p_n}}(z_2 \otimes ... \otimes z_n)
$$

Identifions $\mathfrak{S}_{p_2 + \cdots + p_n}$ au sous-groupe de $\mathfrak{S}_{p_1 + \cdots + p_n}$ formé des permutations dont la restriction à $\{1, p_1\}$ est l’identité. Alors

$$
\operatorname{Tr}_{\mathfrak{S}_{p_1|p_2+\cdots+p_n}/\mathfrak{S}_{p_1|p_2|\ldots|p_n}}(z_1 \otimes z_2 \otimes \ldots \otimes z_n) =
$$
$$
= z_1 \otimes \operatorname{Tr}_{\mathfrak{S}_{p_2+\cdots+p_n}/\mathfrak{S}_{p_2|\ldots|p_n}}(z_2 \otimes \ldots \otimes z_n) = z_1 \otimes (z_2 \ldots z_n) .
$$

On a donc

$$
z_1 z_2 \ldots z_n = z_1(z_2 \ldots z_n) =
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2+\cdots+p_n}/\mathfrak{S}_{p_1|p_2+\cdots+p_n}}(z_1 \otimes (z_2 \ldots z_n))
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+\cdots+p_n}/\mathfrak{S}_{p_1|p_2+\cdots+p_n}}(\operatorname{Tr}_{\mathfrak{S}_{p_1|p_2+\cdots+p_n}/\mathfrak{S}_{p_1|p_2|\ldots|p_n}}(z_1 \otimes z_2 \otimes \ldots \otimes z_n))
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+\cdots+p_n}/\mathfrak{S}_{p_1|\ldots|p_n}}(z_1 \otimes z_2 \otimes \ldots \otimes z_n)
$$

d’après la prop. 1, (ii) de IV, p. 40. Ainsi, (ii) est démontré.
En particulier,

$$
z_1(z_2 z_3) = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2+p_3}/\mathfrak{S}_{p_1|p_2|p_3}}(z_1 \otimes z_2 \otimes z_3),
$$

et l’on établit de même que

$$
(z_1 z_2) z_3 = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2+p_3}/\mathfrak{S}_{p_1|p_2|p_3}}(z_1 \otimes z_2 \otimes z_3).
$$

Donc l’algèbre $\mathbf{TS}(M)$ est associative.
Soit $\sigma$ l’élément de $\mathfrak{S}_{p_1+p_2}$ tel que

$$
\sigma(1) = p_2 + 1, \sigma(2) = p_2 + 2, \ldots, \sigma(p_1) = p_2 + p_1,
$$
$$
\sigma(p_1 + 1) = 1, \sigma(p_1 + 2) = 2, \ldots, \sigma(p_1 + p_2) = p_2.
$$

Alors

$$
z_2 z_1 = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\mathfrak{S}_{p_2|p_1}}(z_2 \otimes z_1)
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\sigma \mathfrak{S}_{p_1|p_2} \sigma^{-1}} \sigma(z_1 \otimes z_2)
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\mathfrak{S}_{p_1|p_2}}(z_1 \otimes z_2) \quad \text{d’après la prop. 1, (i)}
$$
$$
= z_1 z_2 .
$$

Donc l’algèbre $\mathbf{TS}(M)$ est commutative.

On prendra garde que l’injection canonique de $\mathbf{TS}(M)$ dans $\mathbf{T}(M)$ n’est pas en général un homomorphisme d’algèbres. Pis encore, $\mathbf{TS}(M)$ n’est pas en général stable par la multiplication de $\mathbf{T}(M)$.

### 4. Puissances divisées

Soient $x \in M$ et $k \in \mathbf{N}$. Il est clair que $x_1 \otimes x_2 \otimes \ldots \otimes x_k$, où
$$
x_1 = x_2 = \cdots = x_k = x,
$$
est un élément de $\mathbf{TS}^k(M)$.

#### Définition 2 {#alg-iv-s5-def-2 .statement}

Si $x \in \mathbf{M}$, l’élément $x \otimes x \otimes \ldots \otimes x$ de $\mathbf{TS}^k(\mathbf{M})$ se note $\gamma_k(x)$.

#### Proposition 3 {#alg-iv-s5-prop-3 .statement}

(i) Si $x \in \mathbf{M}$, la puissance $p$-ième de $x$ calculée dans $\mathbf{TS}(\mathbf{M})$ est égale à $p! \; \gamma_p(x)$.
(ii) Soient $x_1, \ldots, x_n \in \mathbf{M}$. On a
$$
\gamma_p(x_1 + x_2 + \cdots + x_n) = \sum_{p_1 + p_2 + \cdots + p_n = p} \gamma_{p_1}(x_1) \gamma_{p_2}(x_2) \ldots \gamma_{p_n}(x_n) .
$$
(iii) Soient $x_1, \ldots, x_n \in \mathbf{M}$, $p_1, \ldots, p_n$ des entiers $\geqslant 0$, et $p = p_1 + \cdots + p_n$. Soit $E$ l’ensemble des applications $\varphi$ de $\{1, \ldots, p\}$ dans $\{1, \ldots, n\}$ telles que
$$
\operatorname{Card} \varphi^{-1}(1) = p_1, \ldots, \operatorname{Card} \varphi^{-1}(n) = p_n .
$$
On a
$$
\gamma_{p_1}(x_1) \gamma_{p_2}(x_2) \ldots \gamma_{p_n}(x_n) = \sum_{\varphi \in E} x_{\varphi(1)} \otimes x_{\varphi(2)} \otimes \ldots \otimes x_{\varphi(p)} .
$$
(iv) Soient $x \in \mathbf{M}$, et $q, r$ des entiers $\geqslant 0$. On a
$$
\gamma_q(x) \gamma_r(x) = \frac{(q + r)!}{q! \; r!} \gamma_{q+r}(x) .
$$
(v) Soient $x_1, \ldots, x_n \in \mathbf{M}$. Pour $H \subset \{1, \ldots, n\}$, posons $x_H = \sum_{i \in H} x_i$. Alors
$$
(-1)^n x_1 x_2 \ldots x_n = \sum_{H \subset \{1, \ldots, n\}} (-1)^{\operatorname{Card} H} \gamma_n(x_H) .
$$

L’assertion (i) résulte aussitôt de la prop. 2, (ii).
Prouvons (ii). Par récurrence sur $n$, on voit qu’il suffit d’envisager le cas où $n = 2$.
Alors on a
$$
\gamma_p(x_1 + x_2) = (x_1 + x_2) \otimes (x_1 + x_2) \otimes \ldots \otimes (x_1 + x_2) \quad (p \text{ facteurs})
$$
$$
= \sum_{p_1 + p_2 = p} \sum_{\sigma \in S_{p_1, p_2}} \sigma(x_1 \otimes x_1 \otimes \ldots \otimes x_1 \otimes x_2 \otimes x_2 \otimes \ldots \otimes x_2)
$$
$$
\quad (p_1 \text{ facteurs } x_1, \; p_2 \text{ facteurs } x_2)
$$
$$
= \sum_{p_1 + p_2 = p} \sum_{\sigma \in S_{p_1, p_2}} \sigma(\gamma_{p_1}(x_1) \otimes \gamma_{p_2}(x_2))
$$
$$
= \sum_{p_1 + p_2 = p} \gamma_{p_1}(x_1) \gamma_{p_2}(x_2) .
$$

Prouvons (iii). Soit $S_{p_1, \ldots, p_n}$ l’ensemble des permutations de $\{1, p_1 + \cdots + p_n\}$ dont les restrictions aux intervalles
$$
\{1, p_1\}, \{p_1 + 1, p_1 + p_2\}, \ldots, \{p_1 + \cdots + p_{n-1} + 1, p_1 + \cdots + p_n\}
$$
sont croissantes. D’après I, p. 57, exemple 2, et la prop. 2, (ii), on a
$$
\gamma_{p_1}(x_1) \gamma_{p_2}(x_2) \ldots \gamma_{p_n}(x_n) =
$$
$$
= \sum_{\rho \in S_{p_1, p_2, \ldots, p_n}} \rho(x_1 \otimes x_1 \otimes \ldots \otimes x_1 \otimes x_2 \otimes x_2 \otimes \ldots \otimes x_2 \otimes \ldots \otimes x_n \otimes x_n \otimes \ldots \otimes x_n)
$$

(avec $p_i$ facteurs $x_i$) et cette somme est égale à

$$
\sum_{\varphi \in E} x_{\varphi(1)} \otimes x_{\varphi(2)} \otimes \ldots \otimes x_{\varphi(p)} .
$$

Dans (iii), faisons $n = 2,\ x_1 = x_2 = x,\ p_1 = q$ et $p_2 = r$. On obtient (iv) (I, loc. cit.).

Enfin, (v) résulte de la prop. 2, (ii), et de la prop. 2 de I, p. 95, appliquée aux éléments $x_i$ de l’anneau $\mathbf{T}(M)$.

#### Remarque 1 {#alg-iv-s5-n4-rem-1 .statement}

Soit $(x_i)_{i \in I}$ une famille d’éléments de M. Pour tout $v \in \mathbf{N}^{(l)}$, posons

$$
x_v = \prod_{i \in I} \gamma_{v_i}(x_i) .
$$

Si $(\lambda_i) \in \mathbf{A}^{(l)}$ et si $p \in \mathbf{N}$, on a, d’après la prop. 3, (ii),

$$
\gamma_p \left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{v \in \mathbf{N}^{(l)}, |v| = p} \lambda^v x_v .
$$

#### Remarque 2 {#alg-iv-s5-n4-rem-2 .statement}

Soit $\mathcal{M}$ l’ensemble des applications de $[1, p]$ dans I. On définit une application $\rho \mapsto \rho^*$ de $\mathcal{M}$ dans $\mathbf{N}^{(l)}$ en posant

$$
\rho^*(i) = \operatorname{Card} \rho^{-1}(i) .
$$

Pour que deux éléments $\rho_1, \rho_2$ de $\mathcal{M}$ vérifient $\rho_1^* = \rho_2^*$, il faut et il suffit qu’il existe $\sigma \in \mathfrak{S}_p$ tel que $\rho_2 = \rho_1 \circ \sigma$ (I, p. 90). D’après la prop. 3, (iii), on a, si $|v| = p$,

$$
x_v = \sum_{\rho \in \mathcal{M}, \rho^* = v} x_{\rho(1)} \otimes x_{\rho(2)} \otimes \ldots \otimes x_{\rho(p)} .
$$

### 5. Tenseurs symétriques sur un module libre

#### Proposition 4 {#alg-iv-s5-prop-4 .statement}

Supposons $M$ libre, et soit $(e_i)_{i \in I}$ une base de $M$.
(i) Pour $v \in \mathbf{N}^{(l)}$, soit $e_v = \prod_{i \in I} \gamma_{v_i}(e_i)$. Alors $(e_v)_{v \in \mathbf{N}^{(l)}}$ est une base du $\mathbf{A}$-module $\mathbf{TS}(M)$. En particulier, l’algèbre $\mathbf{TS}(M)$ est engendrée par la famille des éléments $\gamma_k(x)$ pour $k \in \mathbf{N}$ et $x \in M$.
(ii) Pour tout $p \in \mathbf{N}$, $\mathbf{TS}^p(M)$ est facteur direct dans le $\mathbf{A}$-module $\mathbf{T}^p(M)$.
Utilisons les notations de la remarque 2 ci-dessus. La famille $(e_{\rho(1)} \otimes \ldots \otimes e_{\rho(p)})_{\rho \in \mathcal{M}}$ est une base de $\mathbf{T}^p(M)$. Alors la prop. 4 résulte de la formule (7) et du lemme suivant, appliqué avec $H = \mathfrak{S}_p$ et $U = \mathbf{T}^p(M)$ :

#### Lemme 1 {#alg-iv-s5-lem-1 .statement}

Soient $H$ un groupe fini, $U$ un $\mathbf{A}[H]$-module à gauche. On suppose que le $\mathbf{A}$-module $U$ possède une base $B$ stable pour les opérations de $H$ dans $U$. Soit $\Omega = B/H$.
Pour tout $\omega \in \Omega$, soit $u_\omega = \sum_{b \in \omega} b$. Alors
(i) $(u_\omega)_{\omega \in \Omega}$ est une base du $\mathbf{A}$-module $U^H$.

(ii) Pour tout $\omega \in \Omega$, soit $v_\omega$ un point de $\omega$; posons $\omega' = \omega - \{ v_\omega \}$ et $B' = \bigcup_{\omega \in \Omega} \omega'$. Alors $B'$ est une base d’un supplémentaire de $U^H$ dans $U$.

La réunion de l’ensemble des $u_\omega$ (pour $\omega \in \Omega$) et de $B'$ est une base de $U$. Si $U' = \sum_{\omega \in \Omega} Au_\omega$ et $U'' = \sum_{b \in B'} Ab$, on a donc $U = U' \oplus U''$. D’autre part, on a $u_\omega \in U^H$ pour tout $\omega \in \Omega$, donc $U' \subset U^H$. Enfin, soit $(\alpha_b)_{b \in B}$ une famille d’éléments de $A$ à support fini et soit $x = \sum_{b \in B} \alpha_b b$. Si $x \in U^H$, on a $\alpha_{hb} = \alpha_b$ pour tout $b \in B$ et tout $h \in H$, donc $x \in U'$. Par suite, $U' = U^H$.

#### Proposition 5 {#alg-iv-s5-prop-5 .statement}

Soient $M$ un $A$-module libre, $k$ un entier $\geqslant 0$, $P$ le sous-$A$-module de $TS^k(M)$ engendré par $\gamma_k(M)$. On suppose $A$ intègre et infini. Pour tout $z \in TS^k(M)$, il existe $\alpha \in A - \{0\}$ tel que $\alpha z \in P$.

Soit $K$ le corps des fractions de $A$. Identifions $TS^k(M)$ à un sous-$A$-module du $K$-espace vectoriel $V = TS^k(M) \otimes_A K$ (prop. 4, et II, p. 116). Il s’agit de montrer que $\gamma_k(M)$ engendre ce $K$-espace vectoriel, c’est-à-dire que toute forme $K$-linéaire $f$ sur $V$ satisfaisant à $f(\gamma_k(M)) = 0$ est nulle. Soit $(e_i)_{i \in I}$ une base de $M$, et définissons les $e_v$ comme dans la prop. 4. Quel que soit $(\alpha_i) \in A^{(l)}$, on a, compte tenu de (6),

$$
0 = f(\gamma_k(\sum_{i \in I} \alpha_i e_i)) = \sum_{v \in N^{(l)}, |v| = k} \alpha^v f(e_v).
$$

D’après le cor. 2 de IV, p. 17, on en déduit que $f(e_v) = 0$ pour tout $v \in N^{(l)}$, d’où $f = 0$.

### 6. Le foncteur $TS$

Soient $M, N$ des $A$-modules, $u$ un homomorphisme de $M$ dans $N$. Il est immédiat que $T(u) (TS(M)) \subset TS(N)$. L’application de $TS(M)$ dans $TS(N)$ déduite de $T(u)$ se note $TS(u)$. On vérifie aussitôt que c’est un homomorphisme unifère d’algèbres graduées, et que l’on a $TS(u) (\gamma_p(x)) = \gamma_p(u(x))$ pour tout $x \in M$ et tout entier $p \geqslant 0$. Si $v : N \to P$ est un homomorphisme de $A$-modules, on a

$$
TS(v \circ u) = TS(v) \circ TS(u).
$$

Par définition de $TS(u)$, le diagramme

$$
\begin{array}{ccc}
M & \longrightarrow & TS(M) \longrightarrow T(M) \\
u \downarrow & & \downarrow TS(u) \\
N & \longrightarrow & TS(N) \longrightarrow T(N)
\end{array}
$$

où les flèches horizontales désignent les injections canoniques, est commutatif.

Si M est un facteur direct de N et si $i : M \to N$ est l’injection canonique, $TS(i)$ est un homomorphisme injectif de $TS(M)$ sur un facteur direct R de $TS(N)$, par lequel on identifie d’ordinaire $TS(M)$ et R. Cela se démontre comme pour l’algèbre tensorielle (III, p. 58).

Supposons que M soit somme directe d’une famille $(M_\lambda)_{\lambda \in L}$ de sous-modules. Les injections canoniques $TS(M_\lambda) \to TS(M)$ définissent un homomorphisme unifère h d’algèbres graduées, dit canonique :

$$
\bigotimes_{\lambda \in L} TS(M_\lambda) \to TS(M)
$$

Soient $\lambda_1, \lambda_2, \ldots, \lambda_n$ des éléments de L deux à deux distincts, et soient $x_1 \in M_{\lambda_1}, \ldots, x_n \in M_{\lambda_n}$. D’après la prop. 3, (ii) de IV, p. 43, on a

(8)
$$
h\left( \sum_{p_1 + \ldots + p_n = p} \gamma_{p_1}(x_1) \otimes \ldots \otimes \gamma_{p_n}(x_n) \right) = \gamma_p(x_1 + \cdots + x_n)
$$

Soit N un A-module somme directe d’une famille $(N_\lambda)_{\lambda \in L}$ de sous-modules. Pour tout $\lambda \in L$, soit $u_\lambda$ un homomorphisme de $M_\lambda$ dans $N_\lambda$. Soit $u$ l’homomorphisme de M dans N défini par les $u_\lambda$. Alors le diagramme

$$
\begin{array}{ccc}
\bigotimes_{\lambda \in L} TS(M_\lambda) & \xrightarrow{h} & TS(M) \\
\downarrow & & \downarrow TS(u) \\
\bigotimes_{\lambda \in L} TS(u_\lambda) & & \\
\downarrow & & \downarrow \\
\bigotimes_{\lambda \in L} TS(N_\lambda) & \xrightarrow{h'} & TS(N)
\end{array}
$$

où h et $h'$ sont les homomorphismes canoniques, est commutatif. En effet, si $z \in TS(M_\lambda)$, et si $i_\lambda$ (resp. $j_\lambda$) désigne l’injection canonique de $M_\lambda$ dans M (resp. $N_\lambda$ dans N), on a

$$
TS(u)\ (h(z)) = TS(u) \circ TS(i_\lambda)\ (z) = TS(u \circ i_\lambda)\ (z) = TS(j_\lambda \circ u_\lambda)\ (z) =
= TS(j_\lambda) \circ TS(u_\lambda)\ (z) = h'(TS(u_\lambda)\ (z))
$$

#### Proposition 6 {#alg-iv-s5-prop-6 .statement}

*Soit M un A-module somme directe d’une famille $(M_\lambda)_{\lambda \in L}$ de sous-modules. Si chaque $M_\lambda$ est un module libre, l’homomorphisme canonique de $\bigotimes_{\lambda \in L} TS(M_\lambda)$ dans $TS(M)$ est un isomorphisme.*

Soit $(e_{i,\lambda})_{i \in I_\lambda}$ une base de $M_\lambda$. Pour $v \in \mathbf{N}^{(I_\lambda)}$, posons $e_{v,\lambda} = \prod_{i \in I_\lambda} \gamma_{v(i)}(e_{i,\lambda})$. Les $e_{v,\lambda}$, pour $v \in \mathbf{N}^{(I_\lambda)}$, forment une base de $TS(M_\lambda)$ (IV, p. 44, prop. 4, (i)) et $e_{0,\lambda}$ est élément unité de $TS(M_\lambda)$. Donc les éléments

(9)
$$
\bigotimes_{\lambda \in L} e_{v_\lambda,\lambda}
$$

où $v_\lambda \in \mathbf{N}^{(I_\lambda)}$, et où $v_\lambda = 0$ sauf pour un nombre fini d’indices, forment une base de $\bigotimes_{\lambda} \mathbf{TS}(M_{\lambda})$. L’image de l’élément (9) par l’homomorphisme canonique de la proposition est $\prod_{\lambda \in L} e_{v_{\lambda}, \lambda}$. Si l’on désigne par $(e_i)_{i \in I}$ la réunion disjointe des familles $(e_{i, \lambda})_{i \in I_{\lambda}}$ les éléments ci-dessus ne sont autres que les $\prod_{i \in I} \gamma_{v(i)}(e_i)$ où $v \in \mathbf{N}^{(I)}$, et constituent donc une base de $\mathbf{TS}(M)$. Cela prouve la proposition.

Dans les conditions de la prop. 6, l’isomorphisme réciproque $\mathbf{TS}(M) \to \bigotimes_{\lambda} \mathbf{TS}(M_{\lambda})$ est encore dit *canonique*. On identifie souvent $\mathbf{TS}(M)$ à $\bigotimes_{\lambda} \mathbf{TS}(M_{\lambda})$ grâce à cet isomorphisme. On prendra garde que, si $z \in \mathbf{TS}(M_{\lambda})$ et $z' \in \mathbf{TS}(M_{\mu})$ avec $\lambda \neq \mu$, l’élément de $\mathbf{TS}(M)$ qu’on est alors amené à noter $z \otimes z'$ n’est pas le produit tensoriel de $z$ et $z'$ dans $\mathbf{T}(M)$ mais le produit symétrique de $z$ et $z'$.

#### Proposition 7 {#alg-iv-s5-prop-7 .statement}

*Soient M un A-module, u l’application* $(x, y) \mapsto x + y$ *de* $M \oplus M$ *dans* $M$, *et f l’application composée*

$$
\mathbf{TS}(M) \otimes \mathbf{TS}(M) \xrightarrow{h} \mathbf{TS}(M \oplus M) \xrightarrow{\mathbf{TS}(u)} \mathbf{TS}(M)
$$

*où h est l’homomorphisme canonique.* *Si* $z, z' \in \mathbf{TS}(M)$, *on a* $f(z \otimes z') = zz'$.

En effet, soit i l’application $x \mapsto (x, 0)$ de $M$ dans $M \oplus M$. On a $u \circ i = \mathrm{Id}_M$, donc $\mathbf{TS}(u) \circ \mathbf{TS}(i) = \mathrm{Id}_{\mathbf{TS}(M)}$. Par suite

$$
f(z \otimes 1) = \mathbf{TS}(u)(h(z \otimes 1)) = \mathbf{TS}(u)(\mathbf{TS}(i)(z)) = z .
$$

De même, $f(1 \otimes z') = z'$, d’où $f(z \otimes z') = f(z \otimes 1) f(1 \otimes z') = zz'$.

### 7. Coproduit dans les tenseurs symétriques

Soit M un A-module *libre*. Soit $\Delta_M = \Delta$ l’homomorphisme diagonal $x \mapsto (x, x)$ de M dans $M \oplus M$. Soit $c_M = c$ l’homomorphisme unifère de A-algèbres graduées composé des homomorphismes :

$$
\mathbf{TS}(M) \xrightarrow{\mathbf{TS}(\Delta)} \mathbf{TS}(M \oplus M) \xrightarrow{\sigma} \mathbf{TS}(M) \otimes \mathbf{TS}(M)
$$

où $\sigma$ est l’isomorphisme canonique. Muni de $c$, $\mathbf{TS}(M)$ est une A-cogèbre graduée.

Pour tout $x \in M$ et tout entier $p \geqslant 0$, on a $\mathbf{TS}(\Delta)(\gamma_p(x)) = \gamma_p((x, x))$, donc d’après (8),

$$
c(\gamma_p(x)) = \sum_{r+s=p} \gamma_r(x) \otimes \gamma_s(x) .
$$

En particulier,

$$
c(x) = x \otimes 1 + 1 \otimes x .
$$

Soit $(x_i)_{i \in I}$ une famille d’éléments de $M$. Pour $v \in \mathbf{N}^{(I)}$, posons $x_v = \prod_{i \in I} \gamma_{v_i}(x_i)$.

Alors

$$
c(x_v) = \sum_{\rho + \sigma = v} x_\rho \otimes x_\sigma .
$$

Cela résulte de (10) puisque $c$ est un homomorphisme d’algèbres.

#### Proposition 8 {#alg-iv-s5-prop-8 .statement}

*Soit M un A-module libre. Pour ses structures d’algèbre et de cogèbre, TS(M) est une bigèbre graduée commutative et cocommutative. La coïunité est l’application A-linéaire $\varepsilon : TS(M) \to TS^0(M) = A$ nulle sur $TS^p(M)$ pour $p > 0$, et telle que $\varepsilon(1) = 1$.

On sait que la A-algèbre $TS(M)$ est associative, commutative et unifère. D’autre part, le coproduit est par construction un homomorphisme d’algèbres graduées. Le fait que la cogèbre $TS(M)$ est coassociative et cocommutative résulte par un calcul facile de la formule (10). L’application $\varepsilon$ de $TS(M)$ dans $A$ est un homomorphisme d’algèbres graduées tel que $\varepsilon(1) = 1$. Enfin, pour tout $x \in M$, on a $\varepsilon(\gamma_p(x)) = 0$ si $p > 0$, $\varepsilon(\gamma_0(x)) = 1$; cela montre, compte tenu de (10), que l’on a $(\varepsilon \otimes 1) \circ c = (1 \otimes \varepsilon) \circ c = \mathrm{Id}_{TS(M)}$; ainsi, $\varepsilon$ est la coïunité de $TS(M)$.

#### Proposition 9 {#alg-iv-s5-prop-9 .statement}

*Soient M et N des A-modules libres, u un A-homomorphisme de M dans N. Alors TS(u) est un homomorphisme de bigèbres.

En effet, on a $\Delta_N \circ u = (u, u) \circ \Delta_M$, donc le diagramme

$$
\begin{array}{ccccc}
TS(M) & \xrightarrow{TS(\Delta_M)} & TS(M \oplus M) & \xrightarrow{\sigma} & TS(M) \otimes TS(M) \\
| & & | & & | \\
TS(N) & \xrightarrow{TS(\Delta_N)} & TS(N \oplus N) & \xrightarrow{\tau} & TS(N) \otimes TS(N),
\end{array}
$$

où $\sigma$ et $\tau$ sont les isomorphismes canoniques, est commutatif (IV, p. 46). Donc $c_N \circ TS(u) = (TS(u) \otimes TS(u)) \circ c_M$.

#### Proposition 10 {#alg-iv-s5-prop-10 .statement}

*Soit M un A-module libre. Les éléments primitifs (III, p. 164) de la bigèbre TS(M) sont les éléments de M.

Soit $(e_i)_{i \in I}$ une base de M. Pour $v \in \mathbf{N}^{(I)}$, posons $e_v = \prod_{i \in I} \gamma_{v_i}(e_i)$. Soit $z = \sum_{v \in \mathbf{N}^{(I)}} \lambda_v e_v$ un élément de $TS(M)$. On a d’après (12)

$$
c(z) = \sum_v \lambda_v \sum_{\rho, \sigma \in \mathbf{N}^{(I)}, \rho + \sigma = v} e_\rho \otimes e_\sigma = \sum_{\rho, \sigma} \lambda_{\rho + \sigma} e_\rho \otimes e_\sigma
$$

donc

$$
c(z) - 1 \otimes z - z \otimes 1 = \sum_{\rho \neq 0, \sigma \neq 0} \lambda_{\rho + \sigma} e_\rho \otimes e_\sigma - \lambda_0 e_0 \otimes e_0 .
$$

Alors

$$
z \text{ primitif} \Leftrightarrow \lambda_{\rho+\sigma} = 0 \quad \text{lorsque} \quad \rho \neq 0 \quad \text{et} \quad \sigma \neq 0 \quad \text{et} \quad \lambda_0 = 0 \\
\Leftrightarrow \lambda_v = 0 \quad \text{lorsque} \quad |v| \neq 1 \\
\Leftrightarrow z \in M .
$$

### 8. Relations entre $TS(M)$ et $S(M)$

L’injection canonique de $M$ dans $TS(M)$ se prolonge de manière unique en un homomorphisme d’algèbres de $T(M)$ dans $TS(M)$ (III, p. 56, prop. 1). D’après la prop. 2, (ii), de IV, p. 41, cet homomorphisme est l’opérateur s de symétrisation. Comme l’algèbre $TS(M)$ est commutative, il existe (III, p. 67) un *homomorphisme d’algèbres* $\varphi_M$ et un seul, dit *canonique*, de l’algèbre $S(M)$ dans l’algèbre $TS(M)$ tel que le diagramme

$$
\begin{array}{ccc}
T(M) & & \\
\downarrow \rho & & \searrow s \\
S(M) & \xrightarrow{\varphi_M} & TS(M),
\end{array}
$$

ou $\rho$ désigne l’homomorphisme canonique de $T(M)$ sur $S(M)$, soit commutatif. On a $\varphi_M(S^p(M)) \subset TS^p(M)$ pour tout $p \in \mathbf{N}$.

D’autre part, en composant l’injection canonique $i$ de $TS(M)$ dans $T(M)$ et l’homomorphisme canonique $\rho$ de $T(M)$ sur $S(M)$, on obtient un *homomorphisme* $\psi_M$ de *A-modules gradués*, dit *canonique*. Le diagramme

$$
\begin{array}{ccc}
& & T(M) \\
& \nearrow i & \\
TS(M) & \xrightarrow{\psi_M} & S(M)
\end{array}
$$

est commutatif.

Si $u : M \to N$ est un homomorphisme de A-modules, le diagramme

$$
\begin{array}{ccccccccc}
S(M) & \xrightarrow{\varphi_M} & TS(M) & \xrightarrow{\psi_M} & S(M) \\
| & & | & & | \\
S(u) & & TS(u) & & S(u) \\
| & & | & & | \\
S(N) & \xrightarrow{\varphi_N} & TS(N) & \xrightarrow{\psi_N} & S(N)
\end{array}
$$

est commutatif, comme on le vérifie aisément.

Si M est somme directe de modules $M_\lambda$, le diagramme

$$
\begin{array}{ccc}
\otimes S(M_\lambda) & \xrightarrow{\otimes \varphi_{M_\lambda}} & \otimes TS(M_\lambda) \\
\downarrow f & & \downarrow g \\
S(M) & \xrightarrow{\varphi_M} & TS(M),
\end{array}
$$

où $f$ et $g$ sont les homomorphismes canoniques, est commutatif. En effet, $g \circ \otimes \varphi_{M_\lambda}$ et $\varphi_M \circ f$ sont des homomorphismes d’algèbres qui, pour tout $\lambda$, coïncident sur $M_\lambda$.

#### Proposition 11 {#alg-iv-s5-prop-11 .statement}

*Si M est libre, $\varphi_M$ est un morphisme de bigèbres graduées.*
En utilisant la commutativité des diagrammes (13) et (14), on obtient le diagramme commutatif

$$
\begin{array}{cccccc}
S(M) & \xrightarrow{S(\Delta)} & S(M \oplus M) & \xrightarrow{h} & S(M) \otimes S(M) \\
\downarrow \varphi_M & & \downarrow \varphi_{M \oplus M} & & \downarrow \varphi_M \otimes \varphi_M \\
TS(M) & \xrightarrow{TS(\Delta)} & TS(M \oplus M) & \xrightarrow{k} & TS(M) \otimes TS(M),
\end{array}
$$

où $\Delta$ est l’homomorphisme diagonal, et où $h, k$ sont les isomorphismes canoniques. La proposition résulte de là.

#### Proposition 12 {#alg-iv-s5-prop-12 .statement}

(i) *Si $u \in S^n(M)$, on a $\psi_M(\varphi_M(u)) = n!u$.*
(ii) *Si $v \in TS^n(M)$, on a $\varphi_M(\psi_M(v)) = n!v$.*
Soient $x_1, ..., x_n \in M$, et $u$ le produit $x_1 ... x_n$ calculé dans $S(M)$. Alors $\varphi_M(u)$ est le produit $x_1 ... x_n$ calculé dans $TS(M)$, c’est-à-dire
$$
\sum_{\sigma \in S_n} x_{\sigma(1)} \otimes ... \otimes x_{\sigma(n)}.
$$
Donc $\psi_M(\varphi_M(u))$ est égal à $\sum_{\sigma \in S_n} x_{\sigma(1)} ... x_{\sigma(n)}$ calculé dans $S(M)$, c’est-à-dire à
$$
n! x_1 ... x_n = n!u.
$$
Soit $v = \sum_{i=1}^p x_1^i \otimes x_2^i \otimes ... \otimes x_n^i$ un élément de $TS^n(M)$, où les $x_j^i$ appartiennent à $M$. Alors $\psi_M(v)$ est égal à $\sum_{i=1}^p x_1^i x_2^i ... x_n^i$ calculé dans $S(M)$, d’où
$$
\varphi_M(\psi_M(v)) = \sum_{i=1}^p s(x_1^i \otimes x_2^i \otimes ... \otimes x_n^i) = s(v) = n!v.
$$

#### Corollaire 1 {#alg-iv-s5-prop-12-cor-1 .statement}

*Si A est une Q-algèbre, l’homomorphisme canonique de $S(M)$* dans $\mathbf{TS}(M)$ est un isomorphisme d’algèbres. Si de plus $M$ est libre, c’est un isomorphisme de bigèbres graduées.

#### Corollaire 2 {#alg-iv-s5-prop-12-cor-2 .statement}

Si $A$ est une $\mathbf{Q}$-algèbre, le module $\mathbf{TS}^n(M)$ est engendré par les puissances $n$-ièmes des éléments de $M$ dans $\mathbf{TS}(M)$.
Cela résulte du cor. 1 et de la propriété analogue de $\mathbf{S}(M)$ (III, p. 68).

### 9. Applications polynomiales homogènes

#### Proposition 13 {#alg-iv-s5-prop-13 .statement}

Soient $M$ et $N$ des $A$-modules, $q$ un entier $\geqslant 0$, $f$ une application de $M$ dans $N$. On suppose $M$ libre. Les conditions suivantes sont équivalentes :
(i) Il existe une application $q$-linéaire $g$ de $M^q$ dans $N$ telle que $f(x) = g(x, x, ..., x)$ pour tout $x \in M$.
(ii) Il existe une application linéaire $h$ de $\mathbf{TS}^q(M)$ dans $N$ telle que $f(x) = h(\gamma_q(x))$ pour tout $x \in M$.
(iii) Il existe une base $(e_i)_{i \in I}$ de $M$ et une famille $(u_\nu)_{\nu \in \mathbf{N}^{(I)}, |\nu| = q}$ d’éléments de $N$ tels que
$$
f\left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{\nu \in \mathbf{N}^{(I)}, |\nu| = q} \lambda^\nu u_\nu
$$
pour tout $(\lambda_i) \in A^{(I)}$.
(iv) Pour toute base $(e_i)_{i \in I}$ de $M$, il existe une famille $(u_\nu)_{\nu \in \mathbf{N}^{(I)}, |\nu| = q}$ d’éléments de $N$ tels que
$$
f\left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{\nu \in \mathbf{N}^{(I)}, |\nu| = q} \lambda^\nu u_\nu
$$
pour tout $(\lambda_i) \in A^{(I)}$.

(i) $\Rightarrow$ (ii) : soit $g$ satisfaisant aux conditions de (i). Il existe une application linéaire $g'$ de $T^q(M)$ dans $N$ telle que $g(x_1, x_2, ..., x_q) = g'(x_1 \otimes x_2 \otimes ... \otimes x_q)$ quels que soient $x_1, ..., x_q \in M$. Alors
$$
f(x) = g(x, x, ..., x) = g'(x \otimes x \otimes ... \otimes x) = g'(\gamma_q(x)) ;
$$
en posant $h = g'|_{\mathbf{TS}^q(M)}$, on voit que la condition (ii) est vérifiée.
(ii) $\Rightarrow$ (i) et (iv) : soit $h$ satisfaisant aux conditions de (ii). D’après la proposition 4, (ii) (IV, p. 44), il existe une application linéaire $g'$ de $T^q(M)$ dans $N$ telle que $h = g'|_{\mathbf{TS}^q(M)}$. Soit $g$ l’application $q$-linéaire de $M$ dans $N$ associée à $g'$. Alors, pour tout $x \in M$, on a
$$
f(x) = h(\gamma_q(x)) = g'(x \otimes x \otimes ... \otimes x) = g(x, x, ..., x) ,
$$
d’où (i). D’autre part, si $(e_i)_{i \in I}$ est une base de $M$, on a, d’après la formule (6) (IV, p. 44)
$$
f\left( \sum_i \lambda_i e_i \right) = h(\gamma_q(\sum_i \lambda_i e_i)) = h\left( \sum_{|\nu| = q} \lambda^\nu e_\nu \right)
$$

en posant $e_v = \prod_{i \in I} \gamma_{v_i}(e_i)$; on a donc
$$
f(\sum_i \lambda_i e_i) = \sum_{|v|=q} \lambda^v h(e_v) .
$$
(iv) $\Rightarrow$ (iii) : c’est évident.
(iii) $\Rightarrow$ (ii) : soient $(e_i), (u_v)$ vérifiant les conditions de (iii). Posons $e_v = \prod_{i \in I} \gamma_{v_i}(e_i)$; rappelons que $(e_v)_{|v|=q}$ est une base de $\mathbf{TS}^q(M)$. Soit $h$ l’homomorphisme de $\mathbf{TS}^q(M)$ dans $N$ défini par $h(e_v) = u_v$. Alors pour tout $x = \sum_i \lambda_i e_i$ dans $M$, on a
$$
f(x) = f(\sum_i \lambda_i e_i) = \sum_{|v|=q} \lambda^v u_v = h(\sum_{|v|=q} \lambda^v e_v) = h(\gamma_q(x)) .
$$

#### Définition 3 {#alg-iv-s5-def-3 .statement}

Soient $M$ et $N$ des $A$-modules, $q$ un entier $\geqslant 0$. On suppose $M$ libre. On note $\mathrm{Pol}_A^q(M, N)$ ou simplement $\mathrm{Pol}^q(M, N)$ l’ensemble des applications de $M$ dans $N$ vérifiant les conditions de la prop. 13. Les éléments de $\mathrm{Pol}^q(M, N)$ s’appellent les applications polynomiales homogènes de degré $q$ de $M$ dans $N$.

La prop. 13, (i), définit un homomorphisme de $A$-modules :
$$
\mathcal{L}_q^*(M, ..., M; N) \to \mathrm{Pol}^q(M, N) .
$$
La prop. 13, (ii), définit un homomorphisme de $A$-modules :
$$
\mathrm{Hom}_A(\mathbf{TS}^q(M), N) \to \mathrm{Pol}^q(M, N) .
$$
Ces homomorphismes sont dits canoniques. Ils sont surjectifs.

#### Exemple 1 {#alg-iv-s5-n9-exa-1 .statement}

Les applications polynomiales homogènes de degré 1 de $M$ dans $N$ sont les applications $A$-linéaires de $M$ dans $N$.
2) Soient $(N_i)_{i \in I}$ une famille de $A$-modules, $f_i$ une application de $M$ dans $N_i$, $i \in I$, et $f : M \to \prod_{i \in I} N_i$ l’application de composantes $f_i$. Pour que $f$ soit polynomiale homogène de degré $q$, il faut et il suffit que chaque $f_i$ soit polynomiale homogène de degré $q$.
3) Soient $(M_j)_{j \in J}$ une famille finie de $A$-modules libres et $u : \prod_{j \in J} M_j \to N$ une application multilinéaire. Alors $u$ est polynomiale de degré $\mathrm{Card}(J)$.
4) Soient $(X_i)_{i \in I}$ une famille d’indéterminées, $N$ un $A$-module, et $u \in N[(X_i)_{i \in I}]$ un polynôme homogène de degré $q$. L’application $(x_i)_{i \in I} \mapsto u((x_i)_{i \in I})$ de $A^{(I)}$ dans $N$ est une application polynomiale homogène de degré $q$ : cela se voit aussitôt sur la condition (iii) de la prop. 13. Si $I$ est fini, toute application polynomiale homogène de degré $q$ de $A^{(I)} = A^I$ dans $N$ est de cette forme.
5) L’application $(x_i)_{i \in \mathbf{N}} \mapsto x_0^2 + x_1^2 + \cdots + x_n^2 + \cdots$ de $A^{(\mathbf{N})}$ dans $A$ est une application polynomiale homogène de degré 2. Si $A = \mathbf{Z}/2\mathbf{Z}$, elle coïncide avec la forme linéaire $(x_i)_{i \in \mathbf{N}} \mapsto x_1 + x_2 + \cdots + x_n + \cdots$.
6) Soit $f \in \mathrm{Pol}_A^q(M, N)$. Soient $B$ un anneau commutatif, $\rho$ un homomorphisme de B dans A, M' et N' les B-modules déduits de M et N grâce à ρ. Supposons M' libre. Alors f ∈ Pol_B^q(M', N') : cela se voit aussitôt sur la condition (i) de la prop. 13.

#### Proposition 14 {#alg-iv-s5-prop-14 .statement}

Soient M, N, P des A-modules, q et r des entiers ≥ 0. On suppose M et N libres. Soient f ∈ Pol^q(M, N), f' ∈ Pol^r(N, P). Alors f' ∘ f ∈ Pol^{qr}(M, P).

Il existe une application q-linéaire g de M^q dans N, et une application r-linéaire g' de N' dans P telles que

$$
f(x) = g(x, x, ..., x) \quad \text{pour tout } x \in M,
$$
$$
f'(y) = g'(y, y, ..., y) \quad \text{pour tout } y \in N.
$$

Alors, pour tout x ∈ M, on a

$$
f'(f(x)) = g'(f(x), f(x), ..., f(x)) = g'(g(x, x, ..., x), ..., g(x, x, ..., x))
$$

et l’application (x_1, ..., x_{qr}) ↦ g'(g(x_1, ..., x_q), ..., g(x_{q(r-1)+1}, ..., x_{qr})) de M^{qr} dans P est qr-linéaire.

#### Proposition 15 {#alg-iv-s5-prop-15 .statement}

Soient M un A-module libre, N un A-module, q un entier ≥ 0. On suppose que l’application y ↦ q !y est un automorphisme de N. Soit f ∈ Pol^q(M, N). Il existe une application q-linéaire symétrique h et une seule de M^q dans N telle que f(x) = h(x, x, ..., x) pour tout x ∈ M. Quels que soient x_1, ..., x_q ∈ M, on a

$$
h(x_1, x_2, ..., x_q) = \frac{(-1)^q}{q!} \sum_{H \subset \{1, 2, ..., q\}} (-1)^{\mathrm{Card}\, H} f(\sum_{i \in H} x_i).
$$

a) Il existe une application q-linéaire g de M^q dans N telle que f(x) = g(x, x, ..., x) pour tout x ∈ M. Définissons l’application q-linéaire h de M dans N par

$$
h(x_1, x_2, ..., x_q) = \frac{1}{q!} \sum_{\sigma \in S_q} g(x_{\sigma(1)}, x_{\sigma(2)}, ..., x_{\sigma(q)}).
$$

Alors h est symétrique et f(x) = h(x, x, ..., x) pour tout x ∈ M.

b) Soit h une application q-linéaire symétrique de M^q dans N telle que f(x) = h(x, x, ..., x). Soit l l’application linéaire de T^q(M) dans N telle que h(x_1, ..., x_q) = l(x_1 ⊗ ... ⊗ x_q) quels que soient x_1, ..., x_q ∈ M. On a

$$
(-1)^q q ! h(x_1, ..., x_q) = (-1)^q \sum_{\sigma \in S_q} h(x_{\sigma(1)}, ..., x_{\sigma(q)}) = (-1)^q l(s(x_1 ⊗ ... ⊗ x_q)) =
= \sum_{H \subset \{1, ..., q\}} (-1)^{\mathrm{Card}\, H} l(\gamma_q(\sum_{i \in H} x_i))
$$

d’après la prop. 3, (v) (IV, p. 43). Or on a

$$
l(\gamma_q(\sum_{i \in H} x_i)) = h(\sum_{i \in H} x_i, ..., \sum_{i \in H} x_i) = f(\sum_{i \in H} x_i).
$$

Cela prouve la formule (16) et l’unicité de h.

#### Proposition 16 {#alg-iv-s5-prop-16 .statement}

Soient M un A-module libre, N un A-module, q un entier positif, u l’homomorphisme canonique de Hom(TS^q(M), N) dans Pol^q(M, N).

(i) Si A est intègre et infini et N sans torsion, u est un isomorphisme.

(ii) Si l’application y ↦ q!y dans N est injective, u est un isomorphisme.

Dans les deux cas de la proposition, il s’agit de prouver que u est injectif, c’est-à-dire que toute application linéaire f de TS^q(M) dans N, nulle sur γ_q(M), est nulle.

Supposons A intègre et infini et N sans torsion. Pour tout z ∈ TS^q(M), il existe α ∈ A − {0} tel que αz soit combinaison A-linéaire d’éléments de γ_q(M) (IV, p. 45, prop. 5). Alors αf(z) = f(αz) = 0, donc f(z) = 0.

Supposons que l’application y ↦ q!y dans N soit injective. D’après IV, p. 43, prop. 3, (v), f est nulle sur s.T^q(M). Donc, si z ∈ TS^q(M), on a q!f(z) = f(sz) = 0 et par suite f(z) = 0.

#### Corollaire {#alg-iv-s5-n9-cor-1 .statement}

Soient M un A-module libre, N un A-module, q un entier positif, h ∈ Pol^q(M, N), (e_i)_{i∈I} une base de M. Dans les deux cas de la prop. 16, il existe une unique famille (u_v)_{v∈\mathbf{N}^{(I)},|v|=q} d’éléments de N tels que h(\sum_{i∈I} λ_i e_i) = \sum_{|v|=q} λ^v u_v pour tout (λ_i) ∈ A^{(I)}.

### 10. Applications polynomiales

#### Définition 4 {#alg-iv-s5-def-4 .statement}

Soient M et N deux A-modules. On suppose que M est libre. Soit Ap(M, N) le A-module des applications de M dans N. Le sous-module $\sum_{q≥0} \mathrm{Pol}_A^q(M, N)$ de Ap(M, N) se note Pol_A(M, N), ou simplement Pol(M, N); ses éléments s’appellent les applications polynomiales de M dans N.

Soit (e_i)_{i∈I} une base de M, et supposons I fini; d’après la prop. 13 (IV, p. 51), une application f de M dans N est polynomiale si et seulement s’il existe un polynôme F à coefficients dans N en les indéterminées X_i tel que l’on ait

$$ f(\sum_{i∈I} x_i e_i) = F(x) $$

pour toute famille x = (x_i)_{i∈I} dans A^{(I)}. Cette propriété est indépendante de la base choisie de M et justifie la terminologie « application polynomiale ».

#### Proposition 17 {#alg-iv-s5-prop-17 .statement}

Soient M un A-module libre et B une A-algèbre associative, commutative et unifière. Alors Pol_A(M, B) est une sous-B-algèbre de l’algèbre Ap(M, B).

Cela résulte de la déf. 4 et de la prop. 13, (iv) (IV, p. 51).

#### Proposition 18 {#alg-iv-s5-prop-18 .statement}

Soient M, N, P des A-modules. On suppose M et N libres. Soient f ∈ Pol(M, N), g ∈ Pol(N, P). Alors g ∘ f ∈ Pol(M, P).

On se ramène aussitôt au cas où il existe un entier q tel que g ∈ Pol^q(N, P). Il existe alors une application q-linéaire h de N^q dans P telle que g(y) = h(y, y, ..., y) pour tout y ∈ N. Écrivant f comme somme d’applications polynomiales homogènes, on est ramené à prouver que l’application

$$
x \mapsto h(f_1(x), f_2(x), \ldots, f_q(x))
$$

de M dans P, où $f_i \in \mathrm{Pol}^{q_i}(M, N)$, est polynomiale. Il existe, pour $i = 1, \ldots, q$, une application $q_i$-linéaire $l_i$ de $M^{q_i}$ dans $N$ telle que $f_i(x) = l_i(x, x, \ldots, x)$ pour tout $x \in M$. Alors

$$
h(f_1(x), f_2(x), \ldots, f_q(x)) = h(l_1(x, \ldots, x), \ldots, l_q(x, \ldots, x)) ,
$$

d’où notre assertion.

#### Lemme 2 {#alg-iv-s5-lem-2 .statement}

*Soient N un A-module, n un entier $\geqslant 0$, et*

$$
f = m_0 + m_1 X + \cdots + m_n X^n \in N[X].
$$

*On suppose qu’il existe $\alpha_0, \alpha_1, \ldots, \alpha_n \in A$ tels que $f(\alpha_0) = \cdots = f(\alpha_n) = 0$, et tels que, pour $i \neq j$, l’homothétie de rapport $\alpha_i - \alpha_j$ dans N soit injective. Alors $f = 0$.*

(Ce lemme généralise le cor. de IV, p. 15).
Le lemme est évident pour $n = 0$. Démontrons-le par récurrence sur $n$. On a

$$
f(X) = f(X) - f(\alpha_0) = \sum_{i=1}^n m_i (X^i - \alpha_0^i) = (X - \alpha_0) g(X)
$$

où $g$ est un élément de $N[X]$ de la forme $m'_0 + m'_1 X + \cdots + m'_{n-1} X^{n-1}$. Les hypothèses du lemme entraînent que $g(\alpha_1) = \cdots = g(\alpha_n) = 0$, donc $g = 0$ d’après l’hypothèse de récurrence, d’où $f = 0$.

#### Proposition 19 {#alg-iv-s5-prop-19 .statement}

*Soient M un A-module libre, N un A-module, G un sous-groupe additif infini de A. On suppose que les homothéties de N définies par les éléments non nuls de G sont injectives. Alors $\mathrm{Pol}(M, N)$ est somme directe des $\mathrm{Pol}^q(M, N)$.*

Soient $f_0, f_1, \ldots, f_n$ tels que $f_i \in \mathrm{Pol}^i(M, N)$. Supposons qu’on ait la relation $f_0 + \cdots + f_n = 0$. Soit $x \in M$. Pour tout $\lambda \in G$, on a

$$
0 = \sum_{i=0}^n f_i(\lambda x)^i = \sum_{i=0}^n \lambda^i f_i(x) .
$$

D’après le lemme 2, appliqué au polynôme $\sum_{i=0}^n f_i(x) X^i$, on a

$$
f_0(x) = \cdots = f_n(x) = 0.
$$

#### Corollaire {#alg-iv-s5-n10-cor-1 .statement}

*On suppose A intègre infini. Soient M un A-module libre, N un A-module sans torsion.*
(i) *On a $\mathrm{Pol}(M, N) = \bigoplus_{q \geqslant 0} \mathrm{Pol}^q(M, N)$, et chaque $\mathrm{Pol}^q(M, N)$ s’identifie canoniquement à $\mathrm{Hom}(\mathbf{T S}^q(M), N)$.*
(ii) *Soient $f \in \mathrm{Pol}(M, N)$, et $(e_i)_{i \in I}$ une base de M. Il existe une famille et une seule $(u_v)_{v \in N^{(I)}}$ d’éléments de N tels que $f(\sum_{i \in I} \lambda_i e_i) = \sum_{v \in N^{(I)}} \lambda^v u_v$ pour tout $(\lambda_i) \in A^{(I)}$.*

L’assertion (i) résulte des prop. 16 et 19. L’assertion (ii) résulte de (i) et du cor. de la prop. 16.

### 11. Relations entre $S(M^*)$, $TS(M)^{*gr}$ et $Pol(M, A)$

Soit M un A-module libre. On munit le dual gradué $TS(M)^{*gr}$ de la structure d’algèbre graduée $^1$, commutative, associative et unifière, déduite de la structure de cogèbre graduée de $TS(M)$ (III, p. 143). D’après III, p. 67, il existe un unique homomorphisme de A-algèbres graduées

$$
\theta : S(M^*) \to TS(M)^{*gr}
$$

induisant en degré 1 l’application identique de $M^*$.

#### Proposition 20 {#alg-iv-s5-prop-20 .statement}

Si le A-module M est libre de type fini, $\theta$ est un isomorphisme d’algèbres graduées.

Soient $(e_i)_{i \in I}$ une base de M, $(e_i^*)_{i \in I}$ la base duale de $M^*$. Pour $v \in \mathbf{N}^I$, posons

$$
e_v = \prod_{i \in I} \gamma_{v_i}(e_i) \in TS(M)
$$

D’après la prop. 4 (IV, p. 44), la famille $(e_v)_{v \in \mathbf{N}^I}$ est une base de $TS(M)$; soit $(e_v^*)$ la base de $TS(M)^{*gr}$ duale de $(e_v)$. Vu III, p. 75, th. 1, il suffit de prouver qu’on a, pour tout $v \in \mathbf{N}^I$

$$
e_v^* = \prod_{i \in I} (e_i^*)^{v_i},
$$

ou encore que, pour $\rho, \sigma \in \mathbf{N}^I$, on a $e_\rho^*.e_\sigma^* = e_{\rho+\sigma}^*$; mais cette dernière assertion résulte de IV, p. 48, formule (12).

#### Remarque 1 {#alg-iv-s5-n11-rem-1 .statement}

On voit de même que, si M est un A-module libre de type fini, l’algèbre graduée $S(M)^{*gr}$ introduite en III, p. 150, s’identifie à $TS(M^*)$.

#### Proposition 21 {#alg-iv-s5-prop-21 .statement}

L’homomorphisme canonique de A-modules (IV, p. 52)

$$
u : TS(M)^{*gr} \to Pol_A(M, A)
$$

est un homomorphisme d’algèbres.

Soient $a \in TS^q(M)^*$, $b \in TS^r(M)^*$, $x \in M$; on a

$$
u(ab)(x) = \langle ab, \gamma_{q+r}(x) \rangle = \langle a \otimes b, c(\gamma_{q+r}(x)) \rangle = \langle a \otimes b, \gamma_q(x) \otimes \gamma_r(x) \rangle =
$$
$$
= \langle a, \gamma_q(x) \rangle \langle b, \gamma_r(x) \rangle = u(a)(x).u(b)(x),
$$

d’où la proposition.

$^1$ On considère ici qu’un homomorphisme gradué de degré – k de $TS(M)$ dans A est un élément de degré k de $TS(M)^{*gr}$ (II, p. 176).

#### Remarque 2 {#alg-iv-s5-n11-rem-2 .statement}

L’homomorphisme composé $\lambda_M = u \circ \theta : S(M^*) \to \mathrm{Pol}_A(M, A)$ est l’unique homomorphisme unifère d’algèbres induisant l’inclusion de
$$
M^* = \mathrm{Pol}^1(M, A)
$$
dans $\mathrm{Pol}(M, A)$. Si $M$ est libre de type fini et $A$ intègre infini, alors $\lambda_M$ est bijectif (prop. 20 et cor. de la prop. 19). En particulier, si $A$ est intègre infini, l’homomorphisme canonique $f \mapsto \tilde{f}$ de $A[X_1, ..., X_n]$ dans $\mathrm{Pol}(A^n, A)$ (IV, p. 4) est un isomorphisme.

#### Remarque 3 {#alg-iv-s5-n11-rem-3 .statement}

Considérons le coproduit $c_S : S(M^*) \to S(M^* \times M^*)$ (III, p. 139, Exemple 6). Quels que soient $v \in S(M^*)$, $x, y \in M$, l’application polynomiale $\lambda_{M \times M}(c_S(v)) : M \times M \to A$ applique $(x, y)$ sur $\lambda_M(v)(x + y)$. En effet, les deux homomorphismes d’algèbres de $S(M^*)$ dans $\mathrm{Ap}(M \times M, A)$ ainsi définis coïncident sur $M^*$, en vertu de la relation
$$
(v \otimes 1 + 1 \otimes v)(x, y) = v(x + y) \quad (v \in M^*) .
$$

## EXERCICES {#alg-iv-s5-exercises}

See the [exercises for § 5](exercises/s5/).
