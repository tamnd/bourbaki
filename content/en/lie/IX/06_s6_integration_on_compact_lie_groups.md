---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 6
section_title: Integration on compact Lie groups
lang: en
source: lie-vii-ix
book_pages: A IX.333-A IX.346, A IX.409-A IX.414
pdf_pages: 0340-0353, 0416-0421
extraction: native
subsections:
    - "no": 1
      title: PRODUCT OF ALTERNATING MULTILINEAR FORMS
      page: 333
      pdf_page: 340
    - "no": 2
      title: INTEGRATION FORMULA OF H. WEYL
      page: 334
      pdf_page: 341
    - "no": 3
      title: INTEGRATION ON LIE ALGEBRAS
      page: 339
      pdf_page: 346
    - "no": 4
      title: INTEGRATION OF SECTIONS OF A VECTOR BUNDLE
      page: 341
      pdf_page: 348
    - "no": 5
      title: INVARIANT DIFFERENTIAL FORMS
      page: 344
      pdf_page: 351
statements: 25
exercises: 13
content_sha256: b4f0de44d1619bc350bca1bb7ad3da1fea92b250a1806c808dd52f47490eb8f2
---

## § 6. INTEGRATION ON COMPACT LIE GROUPS

We retain the notations of §4; put $w(G) =$ Card(W$_G(T))$. Denote by $dg$ (resp. $dt)$ the Haar measure on G (resp. T) with total mass 1, and by $n$ (resp. $r)$ the dimension of G (resp. T).

### 1. PRODUCT OF ALTERNATING MULTILINEAR FORMS

Let A be a commutative ring and M an A-module. For each integer $r\geq 0$, denote by Alt$^r(M)$ the A-module of alternating $r$-linear forms on M; it can be identified with the dual of the A-module $\wedge \wedge^r(M) ($Algebra, Chap. III, §7, no. 4, Prop. 7). Let $u\in$ Alt$^s(M)$ and $v\in$ Alt$^r(M)$; recall (Algebra, Chap. III, §11, no. 2, Example 3) that the alternating product of $u$ and $v$ is the element $u\wedge v\in$ Alt$^{s+r}(M)$ defined by

$$
(u\wedge v)(x_1, . . . , x_{s+r}) =\sum_{\sigma\in\mathfrak{S}_{s,r}}\varepsilon_{\sigma}u(x_{\sigma(1)}, . . . , x_{\sigma(s)})v(x_{\sigma(s+1)}, . . . , x_{\sigma(s+r)})
$$

where $\mathfrak{S}_{s,r}$ is the subset of the symmetric group $\mathfrak{S}_{s+r}$ consisting of the permutations whose restrictions to $1, s$ and $s+ 1, s+r$ are increasing.

Now let

0 $\longrightarrow M'\longrightarrow^i$ M $\longrightarrow^pM''\longrightarrow$ 0

be an exact sequence of free A-modules, of ranks $r, r+s$ and $s$, respectively.

#### Lemma 1 {#lie-ix-s6-lem-1 .statement tag=01EX}

There exists an A-bilinear map from Alt$^s(M'')\times$ Alt$^r(M')$ to Alt$^{s+r}(M)$, denoted by $(u, v) \rightarrow u\cap v$, and characterized by either of the following two properties:

a) Denote by $u_1\in$ Alt$^s(M)$ the form $(x_1, . . . , x_s) \rightarrow u(p(x_1), . . . , p(x_s))$, and let $v_1\in$ Alt$^r(M)$ be a form such that $v_1(i(x'_1), . . . , i(x'_r)) =v(x'_1, . . . , x'_r)$ for $x'_1, . . . , x'_r$ in $M'$; then $u\cap v=u_1\wedge v_1$.

b) For all $x_1, . . . , x_s$ in M and $x'_1, . . . , x'_r$ in $M'$,

$$
(u\cap v)(x_1, . . . , x_s, i(x'_1), . . . , i(x'_r)) =u(p(x_1), . . . , p(x_s))v(x'_1, . . . , x'_r) \tag{1}
$$

The map $\varphi :$ Alt$^s(M'')\otimes_A$Alt$^r(M')\rightarrow$ Alt$^{s+r}(M)$ such that $\varphi (u\otimes v) =u\cap v$ is an isomorphism of free A-modules of rank one.

The existence of a form $v_1$ satisfying condition $a)$ follows from the fact that $\wedge \wedge^r(i)$ induces an isomorphism from $\wedge \wedge^r(M')$ to a direct factor submodule of $\wedge \wedge^r(M) ($Algebra, Chap. III, §7, no. 2). Let $v_1$ be such a form; put $u\cap v=u_1\wedge v_1$. Formula (1) is then satisfied, since if we put $i(x'_k) =x_{s+k}$ for $1\leq k\leq r$, the only element $\sigma$ of $\mathfrak{S}_{s,r}$ such that $p(x_{\sigma(i)})\not= 0$ for $1\leq i\leq s$ is the identity permutation. On the other hand, formula (1) determines $u\cap v$ uniquely: indeed, let $(e'_1, . . . , e'_r)$ be a basis of $M', (f_1'', . . . , f_s'')$ a basis of $M''$, and $f_1, . . . , f_s$ elements of M such that $p(f_i) =f_i''$ for $1\leq i\leq s$. Then $(f_1, . . . , f_s, i(e'_1), . . . , i(e'_r))$ is a basis of M (Algebra, Chap. II, §1, no. 11, Prop. 21), and formula (1) can be written

$$
(u\cap v)(f_1, . . . , f_s, i(e'_1), . . . , i(e'_r)) =u(f_1'', . . . , f_s'')v(e'_1, . . . , e'_r) \tag{2}
$$

but an element of Alt$^{s+r}(M)$ is determined by its value on a basis.

It follows from the preceding that each of the conditions $a)$ and $b)$ determines the product $u\cap v$ uniquely; it is clear that this product is bilinear. Finally, the last assertion of the lemma follows from formula (2).

### 2. INTEGRATION FORMULA OF H. WEYL

Let $e$ be the identity element of G and $\overline{e}$ its class in $G/T$. Identify the tangent space of G at $e$ with $\mathfrak{g}$, the tangent space of T at $e$ with $\mathfrak{t}$ and the tangent space of $G/T$ at $\overline{e}$ with $\mathfrak{g}/\mathfrak{t}$. Denote by $(u, v) \rightarrow u\cap v$ the $\mathbf{R}$-bilinear map

Alt$^{n-r}(\mathfrak{g}/\mathfrak{t})\times$ Alt$^r(\mathfrak{t})\rightarrow$ Alt$^n(\mathfrak{g})$

defined in number 1.

Recall (Chap. III, §3, no. 13, Prop. 50) that the map $\omega  \rightarrow \omega (e)$ is an isomorphism from the vector space of left-invariant differential forms of degree $n$ (resp. $r)$ on G (resp. T) to the space Alt$^n(\mathfrak{g})$ (resp. Alt$^r(\mathfrak{t}))$. Further, observe that, since every connected compact subgroup of $\mathbf{R}^*$ reduces to the identity element, det Ad $g= 1$ for all $g\in G$, so that the left-invariant differential forms of degree $n$ on G are also right-invariant and invariant under inner automorphisms (Chap. III, §3, no. 16, Cor. of Prop. 54): we shall speak simply of G-invariant differential forms from now on.

Similarly, it follows from Chap. III, §3, no. 16, Prop. 56 and the preceding that the map $\omega  \rightarrow \omega (\overline{e})$ is an isomorphism from the space of G-invariant differential forms of degree $n-r$ on $G/T$ to the space Alt$^{n-r}(\mathfrak{g}/\mathfrak{t})$.

If $\omega_{G/T}$ is a G-invariant differential form of degree $n-r$ on $G/T$, and $\omega_T$ an invariant differential form of degree $r$ on T, denote by $\omega_{G/T}\cap \omega_T$ the unique invariant differential form of degree $n$ on G such that

$$
(\omega_{G/T}\cap \omega_T)(e) =\omega_{G/T}(\overline{e})\cap \omega_T(e)
$$

Recall finally that $f: (G/T)\times T\rightarrow G$ denotes the morphism of manifolds induced by the map $(g, t) \rightarrow gtg^{-1}$ from $G\times T$ to G by passage to the quotient (§5, no. 4). If $\alpha$ and $\beta$ are differential forms on $G/T$ and T, respectively, denote simply by $\alpha \wedge \beta$ the form pr$^*_1\alpha \wedge$ pr$^*_2\beta$ on $(G/T)\times T$.

For $t\in T$, denote by Ad$_{\mathfrak{g}/\mathfrak{t}}(t)$ the endomorphism of $\mathfrak{g}/\mathfrak{t}$ induced by Ad $t$ by passage to the quotient. Put

$\delta_G(t) =$ det(Ad$_{\mathfrak{g}/\mathfrak{t}}(t)-1) =\prod_{\alpha\in R(G,T)}(t^{\alpha}-1)$. (3)

Let $x\in \mathfrak{t}$ and $\alpha \in R(G,T)$; denote by $\widehat{\alpha}$ the element $(2\pi i)^{-1}\delta (\alpha )$ of $\mathfrak{t}^*$, so that

((exp $x)^{\alpha}-$ 1)((exp $x)^{-\alpha}-1) = (e^{2\pi i\widehat{\alpha}(x)}-1)(e^{-2\pi i\widehat{\alpha}(x)}-1) = 4$ sin$^2\pi \widehat{\alpha}(x)$.

If $R_+(G,T)$ denotes the set of positive roots of $R(G,T)$ relative to a basis B, we have

$\delta_G$(exp $x) =\prod_{\alpha\in R_+(G,T)}4$ sin$^2\pi \widehat{\alpha}(x)$,

so, in particular, $\delta_G(t)>0$ for all $t\in T_r$. We remark also that $\delta_G(t) =\delta_G(t^{-1})$ for $t\in T$.

#### Proposition 1 {#lie-ix-s6-prop-1 .statement tag=01EY}

Let $\omega_G, \omega_{G/T}$ and $\omega_T$ be invariant differential forms on $G,G/T$ and T, respectively, of respective degrees $n, n-r$ and $r$. If $\omega_G=$ $\omega_{G/T}\cap \omega_T$, then

$$
f^*(\omega_G) =\omega_{G/T}\wedge \delta_G\omega_T
$$

Clearly we can assume that $\omega_{G/T}$ and $\omega_T$ are non-zero; then the differential form $(u, t) \rightarrow \omega_{G/T}(u)\wedge \omega_T(t)$ on $(G/T)\times T$ is of degree $n$ and everywhere non-zero; hence there exists a numerical function $\delta$ on $(G/T)\times T$ such that

$$
f^*(\omega_G)(u, t) =\delta (u, t)\omega_{G/T}(u)\wedge \omega_T(t)
$$

Observe now that, for $h\in G,u\in G/T,t\in$ T, we have $f(h.u, t) =$ (Int $h)f(u, t)$; since $\omega_G$ is invariant under inner automorphisms, it follows immediately that $\delta (h.u, t) =\delta (u, t)$, so $\delta (u, t) =\delta (\overline{e}, t)$.

Denote by $p:\mathfrak{g}\rightarrow \mathfrak{g}/\mathfrak{t}$ the quotient map and by $\varphi :\mathfrak{g}/\mathfrak{t}\rightarrow \mathfrak{g}$ the map defined by

$\varphi (p(X)) =$ (Ad $t^{-1})X-X$ for $X\in \mathfrak{g}$; recall (§5, no. 4, Lemma 4) that the tangent map

$$
T_{(e,t)}(f) : T_e(G/T)\times T_t(T)\rightarrow T_t(G)
$$

takes $(z, tH)$ to $t(\varphi (z) +H)$ for $z\in \mathfrak{g}/\mathfrak{t}, H\in \mathfrak{t}$.

Let $z_1, . . . , z_{n-r}$ be elements of $\mathfrak{g}/\mathfrak{t},H_1, . . . , H_r$ elements of $\mathfrak{t}$. Then

$$
f^*\omega_G(\overline{e}, t)(z_1, . . . , z_{n-r}, tH_1, . . . , tH_r)
$$

$=\omega_G(t)(t\varphi (z_1), . . . , t\varphi (z_{n-r}), tH_1, . . . , tH_r)$ by the calculation of $T_{(\overline{e},t)}(f)$

$=\omega_G(e)(\varphi (z_1), . . . , \varphi (z_{n-r}), H_1, . . . , H_r)$ since $\omega_G$ is invariant

$=\omega_{G/T}(\overline{e})(p\varphi (z_1), . . . , p\varphi (z_{n-r})).\omega_T(e)(H_1, . . . , H_r)$ (no$.1$, Lemma 1)

= det($p\varphi$ )$\omega_{G/T}(\overline{e})(z_1, . . . , z_{n-r}).\omega_T(e)(H_1, . . . , H_r)$

$$
=\delta_G(t)\omega_{G/T}(\overline{e})(z_1, . . . , z_{n-r}).\omega_T(t)(tH_1, . . . , tH_r)
$$

since $\omega_T$ is invariant

$$
=\delta_G(t)(\omega_{G/T}\wedge \omega_T)(\overline{e}, t)(z_1, . . . , z_{n-r}, tH_1, . . . , tH_r)
$$

so $f^*\omega_G(\overline{e}, t) =\delta_G(t)(\omega_{G/T}\wedge \omega_T)(\overline{e}, t)$; thus, $\delta (\overline{e}, t) =\delta_G(t)$, hence the proposition.

Give the manifolds $G,T$ and $G/T$ the orientations defined by the forms $\omega_G, \omega_T$ and $\omega_{G/T}$, respectively. These forms define invariant measures on $G,T$ and $G/T$ (Chap. III, §3, no. 16, Props. 55 and 56), also denoted by $\omega_G, \omega_T$ and $\omega_{G/T}$.

#### Lemma 2 {#lie-ix-s6-lem-2 .statement tag=01EZ}

If $\omega_G=\omega_{G/T}\cap \omega_T$, then

$$
\int_G\omega_G=\int_{G/T}\omega_{G/T}.\int_T\omega_T
$$

Denote by $\pi$ the canonical morphism from G to $G/T$. Let $g\in G$, and let $t_1, . . . , t_{n-r}$ be elements of $T_{\pi(g)}(G/T)$. Identify the fibre $\pi^{-1}(\pi (g)) =gT$ with T by the translation $\gamma (g)$. The relation $\omega_G=\omega_{G/T}\cap \omega_T$ now implies the equality (Differentiable and Analytic Manifolds, Results, 11.4.5):

$$
\omega_G(t_1, . . . , t_{n-r}) = (\omega_{G/T}(t_1, . . . , t_{n-r}))\omega_T
$$

Thus $\int_{\pi}\omega_G=(\int_T\omega_T)\omega_{G/T}($Differentiable and Analytic Manifolds, Results, 11.4.6), and

$$
\int_G\omega_G=\int_{G/}\int_{T\pi}\omega_G=\int_T\omega_T.\int_{G/T}\omega_{G/T}
$$

(Differentiable and Analytic Manifolds, Results, 11.4.8).

#### Lemma 3 {#lie-ix-s6-lem-3 .statement tag=01F0}

The inverse image on $(G/T)\times T_r$ of the measure $dg$ on $G_r$ under the local homeomorphism $f_r($Integration, Chap. V, §6, no. 6) is the measure $\mu\otimes \delta_Gdt$, where $\mu$ is the unique G-invariant measure on $G/T$ of total mass 1.

Choose an invariant differential form $\omega_T$ (resp. $\omega_{G/T})$ on T (resp. $G/T)$ of maximal degree, such that the measure defined by $\omega_T$ (resp. $\omega_{G/T})$ is equal to $dt$ (resp. $\mu)$. Put $\omega_G=\omega_{G/T}\cap \omega_T$. Lemma 2 implies that the measure defined by $\omega_G$ is equal to $dg$. Let U be an open subset of $(G/T)\times T_r$ such that $f_r$ induces an isomorphism from U to an open subset V of $G_r$. Let $\varphi$ be a continuous function with compact support in V; denote also by $\varphi$ the extension of $\varphi$ to $G_r$ which vanishes outside V. We have

$$
\int_V\varphi  dg=\int_V\varphi  \omega_G=\int_U(\varphi \circ f_r)f_r^*(\omega_G)
$$

$=\int_U(\varphi \circ f_r)\omega_{G/T}\wedge \delta_G\omega_T$ (Prop$.1)$

$$
=\int_U(\varphi \circ f_r)d\mu.\delta_Gdt
$$

hence the lemma.

#### Theorem 1 (H. Weyl) {#lie-ix-s6-thm-1 .statement tag=01F1}

The measure $dg$ on G is the image under the map $(g, t) \rightarrow gtg^{-1}$ from $G\times T$ to G of the measure $dg\otimes_{w(G)}^1\delta_Gdt$, where

$\delta_G(t) =$ det(Ad$_{\mathfrak{g}/\mathfrak{t}}(t)-1) =\prod_{\alpha\in R(G,T)}(t^{\alpha}-1)$.

Equivalently (Integration, Chap. V, §6, no. 3, Prop. $4),dg$ is the image under the map $f: (G/T)\times T\rightarrow G$ of the measure $\mu\otimes_{w(G)}^1\delta_Gdt$.

We prove the last assertion. It follows from §5, no. 1 and Differentiable and Analytic Manifolds, Results$, 10.1.3c)$ that G**--** $G_r$ is negligible in G and T **--** $T_r$ is negligible in T. Further, the map $f_r$ makes $(G/T)\times T_r$ a principal covering of $G_r$, with group W (§5, no. 4, Prop. $4b))$. The theorem now follows from Lemma 3 and Integration, Chap. V, §6, no. 6, Prop. 11.

#### Corollary 1 {#lie-ix-s6-thm-1-cor-1 .statement tag=01F2}

(i) Let $\varphi$ be an integrable function on G with values in a Banach space or in $\mathbf{R}$. For almost all $t\in T$, the function $g \rightarrow \varphi (gtg^{-1})$ on G is integrable for $dg$. The function $t \rightarrow \delta_G(t)\int_G\varphi (gtg^{-1})dg$ is integrable on T, and we have

$\int$ 1 $\int(\int_{-1})$

$$
\varphi (g)dg=\varphi (gtg)dg\delta_G(t)dt \tag{4}
$$

$$
_Gw(G)_{TG}
$$

(“Hermann Weyl’s integration formula”).

(ii) Let $\varphi$ be a positive measurable function on G. For almost all $t\in T$, the function $g \rightarrow \varphi (gtg^{-1})$ on G is measurable. The function $t \rightarrow \int_G^*\varphi (gtg^{-1})dg$ on T is measurable, and we have

$\int*$ 1 $\int*(\int*-1)$

$$
\varphi (g)dg=\varphi (gtg)dg\delta_G(t)dt \tag{5}
$$

$$
_Gw(G)_{TG}
$$

Since the map $f$ is induced by passage to the quotient from the map $(g, t) \rightarrow gtg^{-1}$ from $G\times T\rightarrow G$, it suffices to apply Integration, Chap. V, §5, 6, 8 and Integration, Chap. VII, §2.

#### Corollary 2 {#lie-ix-s6-thm-1-cor-2 .statement tag=01F3}

Let $\varphi$ be a central function on G (that is, such that $\varphi (gh) =$ $\varphi (hg)$ for all $g$ and $h$ in G) with values in a Banach space or in $\mathbf{R}$.

a$)\varphi$ is measurable if and only if its restriction to T is measurable.

b$)\varphi$ is integrable if and only if the function $(\varphi |T)\delta_G$ is integrable on T, and in that case we have

$\int$ 1 $\int$

$$
\varphi (g)dg=\varphi (t)\delta_G(t)dt \tag{6}
$$

$$
_Gw(G)_T
$$

Denote by $p: G/T\times T\rightarrow T$ the second projection. We have $\varphi \circ f$ = $(\varphi |T)\circ p$; further, the image under $p$ of the measure $\mu\otimes_{w(G)}^1\delta_Gdt$ is $_{w(G)}^1\delta_Gdt$. The corollary now follows from Th. 1 above and Th. 1 of Integration, Chap. V, §6, no. 2, applied to the two proper maps $f$ and $p$.

#### Corollary 3 {#lie-ix-s6-thm-1-cor-3 .statement tag=01F4}

Let H be a connected closed subgroup of G containing T, $\mathfrak{h}$ its Lie algebra, and $dh$ the Haar measure on H of total mass 1. Let $\varphi$ be an integrable central function on G, with values in a Banach space or in $\mathbf{R}$. Then the function $h \rightarrow \varphi (h$)det(Ad$_{\mathfrak{g}/\mathfrak{h}}(h)-1)$ is integrable and central on H and we have

$$
\int w(H)\int
$$

$\varphi (g)dg=\varphi (h$)det(Ad$_{\mathfrak{g}/\mathfrak{h}}(h)-1)dh$. (7)

$$
_Gw(G)_H
$$

Indeed, the function $h \rightarrow \varphi (h$)det(Ad$_{\mathfrak{g}/\mathfrak{h}}(h)-1)$ is a central function on H whose restriction to T is the function $t \rightarrow \varphi (t)\delta_G(t)\delta_H(t)^{-1}$. Thus, the corollary follows from Cor. 2 applied to G and to H.

#### Remark 1 {#lie-ix-s6-n2-rem-1 .statement tag=01F5}

If we take $\varphi = 1$ in Cor. 3, we obtain

$\int_H$ det(Ad$_{\mathfrak{g}/\mathfrak{h}}(h)-1)dh=w(G)/w(H)$ (8)

and in particular

$$
\int_T\delta_G(t)dt=w(G) \tag{9}
$$

#### Remark 2 {#lie-ix-s6-n2-rem-2 .statement tag=01F6}

Let $\nu$ be the measure on the quotient $T/W$ defined by

$\int$ 1 $\int$

$$
\psi (\tau )d\nu (\tau ) =\psi (\pi (t))\delta_G(t)dt
$$

$$
_{T/W}w(G)_T
$$

where $\pi$ denotes the canonical projection of T onto $T/W$. Cor. 2 means that the homeomorphism $T/W\rightarrow G/$Int(G) (§2, no. 5, Cor. 1 of Prop. 5) transports the measure $\nu$ to the image of the measure $dg$ under the canonical projection $G\rightarrow G/$Int(G).

#### Remark 3 {#lie-ix-s6-n2-rem-3 .statement tag=01F7}

Assume that G is simply-connected. Let A be an alcove of $\mathfrak{t}$, and $dx$ the Haar measure on $\mathfrak{t}$ such that $\int_Adx= 1$. Then the measure $\nu$ can also be obtained by transporting the measure $_{w(G)}^1\prod_{\alpha\in R_+(G,T)}4$ sin$^2\pi \widehat{\alpha}(x)dx$ on A by

the homeomorphism $A\rightarrow T/W ($§5, no. 2, Cor. 1 of Prop. 2).

#### Example {#lie-ix-s6-n2-exa-1 .statement tag=01F8}

Take G to be the group $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ and T to be the subgroup of diagonal matrices (§3, no. 6); identify $\mathfrak{t}$ with $\mathbf{R}$ by the choice of basis $\{iH\}$ of $\mathfrak{t}($loc. cit.). Put $A = 0, \pi$; this is an alcove of $\mathfrak{t}$. The interval $A = 0, \pi$ can be identified with the space of conjugacy classes of G, the element $\theta$ of

$(e^{i\theta}$ 0 $)$

A corresponding to the conjugacy class of $-_{i\theta}$ . Let $d\theta$ be Lebesgue

0 $e$

measure on $0, \pi$; it follows from the preceding that the image on A of the Haar measure on G is the measure $^2_{\pi}$ sin$^2\theta  d\theta$.

### 3. INTEGRATION ON LIE ALGEBRAS

#### Proposition 2 {#lie-ix-s6-prop-2 .statement tag=01F9}

Let H be a (real) Lie group of dimension $m,\mathfrak{h}$ its Lie algebra. Let $\omega_H$ be a right-invariant differential form of degree $m$ on H, and let $\omega_{\mathfrak{h}}$ be the translation-invariant differential form on $\mathfrak{h}$, of degree $m$, that coincides with $\omega_H(e)$ at the origin. We have

(exp$_H)^*\omega_H=\lambda_{\mathfrak{h}}\omega_{\mathfrak{h}}$ (10)

where $\lambda_{\mathfrak{h}}$ is the Ad(H)-invariant function on $\mathfrak{h}$ such that

1 $p$

$\lambda_{\mathfrak{h}}(x) =$ det $\sum$ (ad $x)$ for $x\in \mathfrak{h}$.

$(p+$ 1)!

$p\geq 0$

Let $x, x_1, . . . , x_m$ be elements of $\mathfrak{h}$. We have

(exp$^*\omega_H)_x(x_1, . . . , x_m) = (\omega_H$(exp $x))(T_x$(exp)($x_1$)$, . . . ,T_x$(exp)($x_m$)). Denote by $(x) :\mathfrak{h}\rightarrow \mathfrak{h}$ the right differential of the exponential at $x$ (Chap. III, §3, no. 17, Def. 8); by definition,

$T_x$(exp)($y$).(exp $x)^{-1}=(x).y$ for all $y\in \mathfrak{h}$.

The form $\omega_H$ being right invariant, we obtain

$(\omega_H$(exp $x))(T_x$(exp)($x_1$)$, . . . ,T_x$(exp)($x_m$))

$=\omega_H(e)((x).x_1, . . . , (x).x_m) =$ (det $(x))\omega_{\mathfrak{h}}(x_1, . . . , x_m)$;

thus, exp$^*\omega_H=\lambda_{\mathfrak{h}}\omega_{\mathfrak{h}}$, with $\lambda_{\mathfrak{h}}(x) =$ det $(x) =$ det$^{exp ad}_{adx}^{x-1}$ (Chap. III, §6, no. 4, Prop. 12).

Let $h\in H$; since Ad $h$ is an automorphism of $\mathfrak{h}$, we have

ad ((Ad $h)(x)) =$ Ad $h\circ$ Ad$x\circ$ (Ad $h)^{-1}$,

so $\lambda_{\mathfrak{h}}$((Ad $h)(x)) =\lambda_{\mathfrak{h}}(x)$. Thus, the function $\lambda_{\mathfrak{h}}$ is invariant under Ad(H); this completes the proof of the proposition.

#### Remark {#lie-ix-s6-n3-rem-1 .statement tag=01FA}

Consider the function $\lambda_{\mathfrak{g}}$ associated to a compact Lie group G; in view of §2, no. 1, Th. 1, to calculate $\lambda_{\mathfrak{g}}$ it suffices to know its values on $\mathfrak{t}$. But, for $x\in \mathfrak{t}$, the endomorphism ad $x$ of $\mathfrak{g}$ is semi-simple, and has eigenvalues 0 (with multiplicity $r)$ and, for all $\alpha \in R(G,T),\delta (\alpha )(x)$ (with multiplicity 1). It follows immediately that

$$
\prod e^{\delta(\alpha)(x)}-1\delta_{\mathfrak{g}}(x)
$$

$\lambda_{\mathfrak{g}}(x) =$ = (11)

$$
\delta (\alpha )(x)\pi_{\mathfrak{g}}(x)
$$

$\alpha \in R(G,T)$

with $\delta_{\mathfrak{g}}(x) =\delta_G$(exp $x)$ and $\pi_{\mathfrak{g}}(x) =\prod_{\alpha\in R(G,T)}\delta (\alpha )(x) =$ det ad$_{\mathfrak{g}/\mathfrak{t}}(x)$.

Let $\omega_{G/T}$ be an invariant differential form of degree $n-r$ on $G/T$ and $\omega_{\mathfrak{t}}$ a translation-invariant differential form of degree $r$ on $\mathfrak{t}$. With the notation of no. 1, denote by $\omega_{G/T}\cap \omega_{\mathfrak{t}}$ the unique translation-invariant differential form $\omega_{\mathfrak{g}}$ of degree $n$ on $\mathfrak{g}$ such that $\omega_{\mathfrak{g}}(0) =\omega_{G/T}(\overline{e})\cap \omega_{\mathfrak{t}}(0)$.

Finally, denote by $\psi : (G/T)\times \mathfrak{t}\rightarrow \mathfrak{g}$ the morphism of manifolds induced by the map $(g, x) \rightarrow$ (Ad $g)(x)$ from $G\times \mathfrak{t}$ to $\mathfrak{g}$ by passage to the quotient.

#### Proposition 3 {#lie-ix-s6-prop-3 .statement tag=01FB}

Let $\omega_{\mathfrak{g}},\omega_{\mathfrak{t}},\omega_{G/T}$ be invariant differential forms on $\mathfrak{g},\mathfrak{t}$, $G/T$, respectively, of respective degrees $n, r, n-r$. If $\omega_{\mathfrak{g}}=\omega_{G/T}\cap \omega_{\mathfrak{t}}$, we have

$$
\psi^*\omega_{\mathfrak{g}}=\omega_{G/T}\wedge \pi_{\mathfrak{g}}\omega_{\mathfrak{t}}
$$

where $\pi_{\mathfrak{g}}$ is the function on $\mathfrak{t}$ defined by $\pi_{\mathfrak{g}}(x) =\prod_{\alpha\in R(G,T)}\delta (\alpha )(x)$.

Denote by $\omega_G$ (resp. $\omega_T)$ the invariant differential form of maximum degree on G (resp. T) that coincides with $\omega_{\mathfrak{g}}$ (resp. $\omega_{\mathfrak{t}})$ at the origin. Consider the commutative diagram

$$
(G/T)\times \mathfrak{t}\longrightarrow^{\psi}\mathfrak{g}
$$

$)$(Id,exp$_T))$exp$_G$.

$(G/T)\times T\longrightarrow^f$ G

In view of Prop. 1 of no. 2 and the relation exp$^*_T\omega_T=\omega_{\mathfrak{t}}$, we deduce the equality

$\psi^*$exp$^*_G\omega_G=\omega_{G/T}\wedge \delta_{\mathfrak{g}}\omega_{\mathfrak{t}}$.

By Prop. $2,\psi^*$exp$^*_G\omega_G= (\psi^*\lambda_{\mathfrak{g}})\psi^*\omega_{\mathfrak{g}}$. Since the function $\lambda_{\mathfrak{g}}$ is invariant under Ad(G), we have

$(\psi^*\lambda_{\mathfrak{g}})(\overline{g}, x) =\lambda_{\mathfrak{g}}(x) =\delta^{\mathfrak{g}}(x)$ for $\overline{g}\in G/T, x\in \mathfrak{t}$.

$$
\pi_{\mathfrak{g}}(x)
$$

It follows that the forms $\psi^*\omega_G(\overline{g}, x)$ and $\omega_{G/T}(\overline{g})\wedge \pi_{\mathfrak{g}}(x)\omega_{\mathfrak{t}}(x)$ coincide where $\delta_{\mathfrak{g}}(x)$ is non-zero, that is on the dense open subset $(G/T)\times \mathfrak{t}_r$; thus, they are equal, hence the proposition.

Choose invariant differential forms $\omega_G$ on G and $\omega_T$ on T, of maximum degree, such that $|\omega_G|=dg$ and $|\omega_T|=dt$; denote by $\omega_{\mathfrak{g}}$ (resp. $\omega_{\mathfrak{t}})$ the translation-invariant differential form on $\mathfrak{g}$ (resp. $\mathfrak{t})$ that coincides with $\omega_G(e)$ (resp. $\omega_T(e))$ at the origin, and $dz$ (resp. $dx)$ the Haar measure $|\omega_{\mathfrak{g}}|$ (resp. $|\omega_{\mathfrak{t}}|)$. Reasoning as in no. 2, mutatis mutandis, gives the following proposition:

#### Proposition 4 {#lie-ix-s6-prop-4 .statement tag=01FC}

The measure $dz$ on $\mathfrak{g}$ is the image under the proper map $(g, x) \rightarrow$ (Ad $g)(x)$ from $G\times \mathfrak{t}$ to $\mathfrak{g}$ of the measure $dg\otimes_{w(G)}^1\pi_{\mathfrak{g}}dx$.

We leave to the reader the statement and proof of the analogues of Cor. 1 to 3 and Remarks 1 to 3 of no. 2. For example, let $\varphi$ be an integrable function on $\mathfrak{g}$ (with values in a Banach space or $\mathbf{R})$; then

$\int$ 1 $\int(\int)$

$\varphi (z)dz=\varphi$((Ad $g)x)dg\pi_{\mathfrak{g}}(x)dx$, (12)

$$
_{\mathfrak{g}}w(G)_{\mathfrak{t}G}
$$

and, in particular, if $\varphi$ is invariant under Ad(G),

$\int$ 1 $\int$

$$
\varphi (z)dz=\varphi (x)\pi_{\mathfrak{g}}(x)dx \tag{13}
$$

$$
_{\mathfrak{g}}w(G)_{\mathfrak{t}}
$$

### 4. INTEGRATION OF SECTIONS OF A VECTOR BUNDLE

In this number and the next, we denote by X a real manifold of class $C^r$ $(1\leq r\leq  \infty )$, locally of finite dimension.

Let Y be a manifold of class $C^r$. If $r <\infty$, consider the map $f \rightarrow$ $j^r(f)$ from $\mathscr{C}^r(X; Y)$ to $\mathscr{C}(X; J^r(X,Y)) ($Differentiable and Analytic Manifolds, Results, 12.3.7). The inverse image under this map of the topology of compact convergence on $\mathscr{C}(X; J^r(X,Y))$ is called the topology of compact $C^r$-convergence on $\mathscr{C}^r(X; Y)$; it is the upper bound of the topologies of uniform $C^r$-convergence on K (Differentiable and Analytic Manifolds, Results, 12.3.10), where K runs through the set of compact subsets of X.

When $r$ = $\infty$, we call the topology of compact $C^{\infty}$-convergence on $\mathscr{C}^{\infty}(X; Y)$ the upper bound of the topologies of compact $C^k$-convergence, in other words the coarsest topology for which the canonical injections $\mathscr{C}^{\infty}(X; Y)\rightarrow \mathscr{C}^k(X; Y)$ are continuous for $0\leq k <\infty$.

Let E be a real vector bundle with base X, of class $C^r$, and let $\mathscr{S}^r(X; E)$ be the vector space of sections of E of class $C^r$. In this number we give $\mathscr{S}^r(X; E)$ the topology induced by the topology of compact $C^r$-convergence on $\mathscr{C}^r(X; E)$, also called the topology of compact $C^r$-convergence; it makes $\mathscr{S}^r(X; E)$ into a complete separated locally convex topological vector space (cf. Differentiable and Analytic Manifolds, Results, 15.3.1 and Spectral Theories, in preparation).

Now let H be a Lie group, $m: H\times X\rightarrow X$ a law of left operation of class $C^r$; put $hx=m(h, x)$ for $h\in H, x\in X$. Let E be a vector H-bundle with base X, of class $C^r$ (Chap. III, §1, no. 8, Def. 4). For $s\in \mathscr{S}^r(X; E)$ and $h\in H$, denote by $^hs$ the section $x \rightarrow h.s(h^{-1}x)$ of E; the map $(h, s) \rightarrow^hs$ is a law of operation of H on the space $\mathscr{S}^r(X; E)$.

#### Lemma 4 {#lie-ix-s6-lem-4 .statement tag=01FD}

The law of operation $H\times \mathscr{S}^r(X; E)\rightarrow \mathscr{S}^r(X; E)$ is continuous.

In view of the definition of the topology of $\mathscr{S}^r(X; E)$ and General Topology, Chap. X, §3, no. 4, Th. 3, it suffices to prove that for any integers $k\leq r$, the map $f: H\times X\times \mathscr{S}^k(X; E)\rightarrow J^k(X; E)$ such that $f(h, x, s) =j_x^k(^hs)$ is continuous. For $h\in H$, denote by $\tau_h$ (resp. $\theta_h)$ the automorphism $x \rightarrow hx$ of X (resp. of E). Define maps

$$
f_1:H\times X\rightarrow J^k(X,X)
$$

$$
f_2:H\times E\rightarrow J^k(E,E)
$$

$$
g:H\times X\times \mathscr{S}^k(X; E)\rightarrow J^k(X,E)
$$

by $f_1(h, x) =j^k_x(\tau_h), f_2(h, v) =j_v^k(\theta_h), g(h, x, s) =j_{hx}^k(s)$. We have

$$
f(h, x, s) =f_2(h, s(h^{-1}x))\circ g(h^{-1}, x, s)\circ f_1(h^{-1}, x)
$$

and consequently it suffices, by Differentiable and Analytic Manifolds, Results, 12.3.6, to prove that $f_1, f_2$ and $g$ are continuous.

Now $g$ is the composite map

$$
H\times X\times \mathscr{S}^k(X; E)-------\longrightarrow^{(m,Id)}X\times \mathscr{S}^k(X; E)
$$

$$
-------\longrightarrow^{(Id,j^k)}X\times \mathscr{C}(X; J^k(X,E))\longrightarrow^{\varepsilon}J^k(X,E)
$$

with $\varepsilon (x, u) =u(x)$; the map $\varepsilon$ being continuous (General Topology, Chap. X, §3, no. 4, Cor. 1 of Th. $3),g$ is continuous.

Let $(h_0, x_0)\in H\times X$; we shall prove that $f_1$ is continuous at $(h_0, x_0)$. There exist charts $(U, \psi ,F)$ and $(V, \chi ,F')$ of X and an open subset $\Omega$ of H such that $x_0\in U, h_0\in \Omega$ and $m(\Omega \times U)\subset V$. By using the expression for $J^k(X,X)$ in these charts, we are reduced to proving, for $1\leq l\leq k$, the continuity at $(h_0, x_0)$ of the map $(h, x) \rightarrow \Delta^l_x(\tau_h)$ from $\Omega \times U$ to $P_l(F; F')$, with $\Delta^l_x(\tau_h)(v) =$ $_{l!}^1D^l\tau_h(x).v$ for $v\in F ($Differentiable and Analytic Manifolds, Results, 12.2). But $D^l\tau_h(x)$ is simply the $l$th partial derivative of $m(h, x)$ with respect to $x$, which is continuous by hypothesis; consequently, $f_1$ is continuous. The proof that $f_2$ is continuous is similar, hence the lemma.

#### Proposition 5 {#lie-ix-s6-prop-5 .statement tag=01FE}

Assume that the group H is compact and denote by $dh$ the Haar measure on H of total mass 1. Let $s$ be a section of E of class $C^r$. Denote by $s$ the vector integral $\int_H^hs dh$. Then $s$ is a section of E of class $C^r$, invariant under H; for $x\in X$, we have $s(x) =\int_Hhs(h^{-1}x)dh\in E_x$. The endomorphism $s \rightarrow s$ of $\mathscr{S}^r(X; E)$ is a projection onto the subspace of H-invariant sections.

Consider the map $h \rightarrow^hs$ from H to $\mathscr{S}^r(X; E)$; it is continuous by Lemma 4. Since the space $\mathscr{S}^r(X; E)$ is separated and complete, the integral $s$ = $\int_H^hs dh$ belongs to $\mathscr{S}^r(X; E) ($Integration, Chap. III, §3, no. 3, Cor. 2). The linear map $s \rightarrow s(x)$ from $\mathscr{S}^r(X; E)$ to $E_x$ being continuous, we have $s(x) =$ $\int_H^hs(x)dh$ for all $x\in X$. It is clear that $s$ is invariant under H; if $s$ is an H-invariant section, we have $s=s$, hence the last assertion.

#### Corollary 1 {#lie-ix-s6-prop-5-cor-1 .statement tag=01FF}

Let F be a Banach space, $\rho : H\rightarrow \mathbf{G}\mathbf{L}(F)$ an analytic linear representation, $f\in \mathscr{C}^r(X; F)$. For $x\in X$, put

$$
f(x) =\int_H\rho (h).f(h^{-1}x)dh
$$

Then $f$ is a morphism of class $C^r$ from X to F, compatible with the operations of H; for $x\in X$, we have (with $\tau_h$ denoting the automorphism $x \rightarrow hx$ of X)

$$
d_xf=\int_H(\rho (h)\circ d_{h^{-1}x}f\circ T_x(\tau_{h^{-1}}))dh\in \mathscr{L}(T_x(X); F) \tag{14}
$$

The first assertion follows from the proposition applied to the bundle $X\times$ F, equipped with the law of operation $(h; (x, f)) \rightarrow (hx, \rho (h).f)$. The second follows from Integration, Chap. III, §3, no. 2, Prop. 2, by applying to the vector integral $f$ the homomorphism $d_x:\mathscr{C}^r(X; F)\rightarrow \mathscr{L}(T_x(X); F)$ which is continuous by the definition of the topology of compact $C^r$-convergence.

#### Corollary 2 {#lie-ix-s6-prop-5-cor-2 .statement tag=01FG}

Let F be a Banach space, $f\in \mathscr{C}^r(X; F)$; put

$$
f(x) =\int_Hf(hx)dh
$$

for $x\in X$. The function $f$ is of class $C^r$, and $f(hx) =f(x)$ for $x\in X$, $h\in H$.

#### Corollary 3 {#lie-ix-s6-prop-5-cor-3 .statement tag=01FH}

Let F be a Banach space, $p$ an integer $\geq 0,^k\Omega^p(X; F)$ the space of differential forms of degree $p$ on X, with values in F, and of class $C^k(2\leq k+ 1\leq r)$. For $\omega \in^k\Omega^p(X; F)$, put $\omega =\int_H\tau_h^*\omega  dh$. Then the map $\omega  \rightarrow \omega$ is a projection on $^k\Omega^p(X; F)$ whose image is the subspace of H-invariant forms. We have $d(\omega ) = (d\omega )$ for all $\omega \in^k\Omega^p(X; F)$.

The first assertion follows from the proposition applied to the vector H-bundle Alt$^p(T(X); F)$ (Chap. III, §1, no. 8, Examples). To prove the second assertion, it suffices, in view of Integration, Chap. III, §3, no. 2, Prop. 2, to prove that the map $d:^k\Omega^p(X; F)\rightarrow^{k-1}\Omega^{p+1}(X; F)$ is continuous when the first (resp. second) space is given the topology of compact $C^k$-convergence (resp. $C^{k-1}$-convergence). But this follows immediately from the definition of these topologies by means of semi-norms (Spectral Theories, in preparation) and the fact that $d$ is a differential operator of order $\leq 1 ($Differentiable and Analytic Manifolds, Results, 14.4.2).

### 5. INVARIANT DIFFERENTIAL FORMS

Let X be a locally finite dimensional real manifold of class $C^{\infty}$, and let $(g, x) \rightarrow gx$ be a law of left operation of class $C^{\infty}$ of a connected compact Lie group G on X. For $g\in G$, denote by $\tau_g$ the automorphism $x \rightarrow gx$ of X. Denote by $\Omega (X)$ the algebra of real differential forms of class $C^{\infty}$ on X (Differentiable and Analytic Manifolds, Results, 8.3.1).

For any element $\xi$ of $\mathfrak{g}$, denote by $D_{\xi}$ the corresponding vector field on X (Chap. III, §3, no. 5) and by $\theta (\xi ), i(\xi )$ the corresponding operators on $\Omega$(X), so that we have the formulas (Differentiable and Analytic Manifolds, Results, 8.4.5 and 8.4.7)

$$
\theta (\xi )\omega =d(i(\xi )\omega ) +i(\xi )d\omega \tag{15}
$$

$$
d_**
$$

$$
(\tau_{expt\xi}\omega ) =\tau_{expt\xi}(\theta (\xi )\omega ) \tag{16}
$$

$$
dt
$$

A differential form $\omega \in \Omega (X)$ is invariant if $\tau_g^*\omega =\omega$ for all $g\in G$; by formula (16), this is equivalent to $\theta (\xi )\omega = 0$ for all $\xi \in \mathfrak{g}$. Denote by $\Omega (X)^G$ the space of invariant differential forms on X; if $\omega \in \Omega (X)^G$, we have $d\omega \in \Omega (X)^G$, so $\Omega (X)^G$ is a subcomplex of the complex $(\Omega (X), d)$.

#### Theorem 2 {#lie-ix-s6-thm-2 .statement tag=01FI}

The canonical injection $\iota :\Omega (X)^G\rightarrow \Omega (X)$ is a homotopism of complexes (Algèbre, Chap. X, p. 33, déf. 5); the map $\omega  \rightarrow \omega =\int_G\tau_g^*\omega  dg$ is a homotopism, inverse to it up to homotopy. In particular, the map $H(\iota ) : H(\Omega (X)^G)\rightarrow H(\Omega (X))$ is bijective.

By Cor. 3 of no. 4, the map $\omega  \rightarrow \omega$ is a morphism of complexes from $\Omega (X)$ to $\Omega (X)^G$ that induces the identity on the subcomplex $\Omega (X)^G$; thus, to prove the theorem it suffices to construct a homomorphism $s:\Omega (X)\rightarrow \Omega$(X), graded of degree $-1$, such that

$\omega -\omega = (d\circ s+s\circ d)(\omega )$ for all $\omega \in \Omega (X)$. (17)

By Lemma 1 of Integration, Chapter IX, §2, no. 4 and Remark 1 of §2, no. 2, there exists a positive measure $d\xi$ on $\mathfrak{g}$ of compact support whose image under the exponential map is equal to $dg$. For $\omega \in \Omega$(X), put

$$
s(\omega ) =\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*(i(\xi )\omega ).d\xi \}dt
$$

we have to show that formula (17) is satisfied. As in the proof of Cor. 1 (no. 4), we verify the formula

$$
ds(\omega ) =\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*d(i(\xi )\omega ).d\xi \}dt
$$

We now deduce from formulas (15) and (16) the equalities

$$
ds(\omega ) +s(d\omega ) =\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*(d(i(\xi )\omega ) +i(\xi )d\omega ).d\xi \}dt
$$

$$
=\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*(\theta (\xi )\omega ).d\xi \}dt
$$

$$
\int\{\int^1d_*\}
$$

= $(\tau_{expt\xi}\omega )dtd\xi$

$$
_{\mathfrak{g}0}dt
$$

$$
=\int_{\mathfrak{g}}(\tau_{exp\xi}^*\omega -\omega )d\xi
$$

$$
=\omega -\omega
$$

hence Th. 2.

We apply the theorem in the case X = G, for the action of G by left translations. Recall (Chap. III, §3, no. 13, Prop. 50) that associating to a differential form on G its value at the identity element gives an isomorphism from $\Omega (G)^G$ to the graded algebra Alt($\mathfrak{g}$) of alternating multilinear forms on $\mathfrak{g}$. Identify $\Omega (G)^G$ with Alt($\mathfrak{g}$) by means of this isomorphism. The operator $d$ is then given by the formula (Chap. III, §3, no. 14, Prop. 51)

$$
d\omega (a_1, . . . , a_{p+1})
$$

$$
=\sum_{i<j}(-1)^{i+j}\omega ([a_i, a_j], a_1, . . . , a_{i-1}, a_{i+1}, . . . , a_{j-1}, a_{j+1}, . . . , a_{p+1})
$$

for $\omega$ in Alt$^p(\mathfrak{g})$ and $a_1, . . . , a_{p+1}$ in $\mathfrak{g}$.

For $\xi \in \mathfrak{g}$, let $L_{\xi}$ be the corresponding left-invariant vector field (defined by means of the action of G on itself by right translations, cf. Chap. III, §3, no. 6). The operators $\theta (L_{\xi}), i(L_{\xi})$ commute with the action of G on $\Omega (G)$ defined by left translation, and hence induce operators $\theta (\xi ), i(\xi )$ on $\Omega (G)^G$; with the preceding identifications, these are expressed by the formulas (Differentiable and Analytic Manifolds, Results, 8.3.2 and 8.4.2)

$$
(\theta (\xi )\omega )(a_1, . . . , a_p) =-\sum_i\omega (a_1, . . . , a_{i-1},[\xi , a_i], a_{i+1}, . . . , a_p)
$$

$$
(i(\xi )\omega )(a_1, . . . , a_{p-1}) =\omega (\xi , a_1, . . . , a_{p-1})
$$

for $\omega$ in Alt$^p(\mathfrak{g})$ and $a_1, . . . , a_p$ in $\mathfrak{g}$.

The subcomplex $^G\Omega (G)^G$ of biinvariant forms (Chap. III, §3, no. 13) can be identified with the subcomplex Alt($\mathfrak{g}$)$^G$ of alternating multilinear forms on $\mathfrak{g}$ invariant under the adjoint representation (that is, such that $\theta (\xi )\omega = 0$ for all $\xi \in \mathfrak{g})$. Thus, we have a commutative diagram of complexes

$$
^G\Omega (G)^G\longrightarrow \Omega (G)^G\longrightarrow \Omega (G)
$$

$$
)) \tag{18}
$$

Alt($\mathfrak{g}$)$^G\longrightarrow$ Alt($\mathfrak{g}$)

where the horizontal arrows are the canonical injections, and the vertical arrows are the isomorphisms induced by the map $\omega  \rightarrow \omega (e)$.

#### Corollary 1 {#lie-ix-s6-thm-2-cor-1 .statement tag=01FJ}

a) In the diagram (18), all the morphisms are homotopisms.

b) Let $\omega \in$ Alt($\mathfrak{g}$). Then $\omega$ belongs to Alt($\mathfrak{g}$)$^G$ if and only if $d\omega = 0$ and $d(i(\xi )\omega ) = 0$ for all $\xi \in \mathfrak{g}$. The differential of the complex Alt($\mathfrak{g}$)$^G$ is zero.

c) The graded vector space $H(\Omega (G))$ is isomorphic to Alt($\mathfrak{g}$)$^G$.

The theorem, applied to the action of G on G by left translations (resp. to the action $((g, h);x) \rightarrow gxh^{-1}$ of $G\times G$ on G) implies that the canonical injection $\Omega (G)^G\rightarrow \Omega (G)$ (resp. $^G\Omega (G)^G\rightarrow \Omega (G))$ is a homotopism; in view of Algèbre, Chap. X, p. 34, Cor., assertion $a)$ follows.

We prove $b)$. By Prop. 51 of Chap. III, §3, no. 14, we have $d\alpha =-d\alpha$, that is $d\alpha = 0$, for every differential form $\alpha$ on G that is left and right invariant. Thus, if $\omega \in$ Alt($\mathfrak{g}$)$^G$, then $d\omega = 0$, and consequently $d(i(\xi )\omega ) =$ $\theta (\xi )\omega -i(\xi )d\omega = 0$. Conversely, if $d\omega = 0$ and $d(i(\xi )d\omega ) = 0$, then $\theta (\xi )\omega = 0$.

Assertion $c)$ follows from $a)$ and $b)$.

#### Remark {#lie-ix-s6-n5-rem-1 .statement tag=01FK}

Consider the subcomplexes $Z(\Omega (G))$ and $B(\Omega (G))$ of $\Omega (G) ($Algèbre, Chap. X, p. 25). It follows from the formula giving the differential of the product of two forms (Differentiable and Analytic Manifolds, Results, 8.3.5) that $Z(\Omega (G))$ is a subalgebra of $\Omega (G)$ and that $B(\Omega (G))$ is an ideal of $Z(\Omega (G))$; consequently, the exterior product induces a graded algebra structure on $H(\Omega (G))$. The preceding now gives an isomorphism of graded algebras $H(\Omega (G))\rightarrow$ Alt($\mathfrak{g}$)$^G$.

Let H be a closed subgroup of G; we apply Th. 2 to $X = G/H$. By Chap. III, §1, no. 8, Cor. 1 of Prop. 17, the G-invariant differential forms on $G/H$ can be identified with the H-invariant elements of Alt(T$_e(G/H))$, that is with the elements of Alt($\mathfrak{g}$) that are H-invariant and annihilated by the operators $i(\xi )$ for all $\xi \in L(H)$. Consequently:

#### Corollary 2 {#lie-ix-s6-thm-2-cor-2 .statement tag=01FL}

Let H be a closed subgroup of G.

a) The canonical injection $\Omega (G/H)^G\rightarrow \Omega (G/H)$ is a homotopism.

b) The complex $\Omega (G/H)^G$ can be identified with the subcomplex of Alt($\mathfrak{g}$) consisting of the elements $\omega$ of Alt($\mathfrak{g}$) that are invariant under the adjoint representation of H and are such that $i(\xi )\omega = 0$ for all $\xi \in L(H)$. If, in addition, H is connected, this subcomplex consists of the $\omega \in$ Alt($\mathfrak{g}$) such that $\theta (\xi )\omega = 0$ and $i(\xi )\omega = 0$ for all $\xi \in L(H)$.

### Exercises {#lie-ix-s6-exercises}

See the [exercises for § 6](exercises/s6/).
