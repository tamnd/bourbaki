---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 5
section_title: Symmetric tensors and polynomial mappings
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.41-A IV.61, A IV.91-A IV.98
pdf_pages: 0050-0070, 0100-0107
extraction: ocr
subsections:
    - "no": 1
      title: Relative traces
      page: 41
      pdf_page: 50
    - "no": 2
      title: Definition of symmetric tensors
      page: 42
      pdf_page: 51
    - "no": 3
      title: Product for symmetric tensors
      page: 43
      pdf_page: 52
    - "no": 4
      title: Divided powers
      page: 45
      pdf_page: 54
    - "no": 5
      title: Symmetric tensors over a free module
      page: 47
      pdf_page: 56
    - "no": 6
      title: The functor TS
      page: 48
      pdf_page: 57
    - "no": 7
      title: Coproduct for symmetric tensors
      page: 50
      pdf_page: 59
    - "no": 8
      title: Relations between TS(M) and S(M)
      page: 52
      pdf_page: 61
    - "no": 9
      title: Homogeneous polynomial mappings
      page: 54
      pdf_page: 63
    - "no": 10
      title: Polynomial mappings
      page: 57
      pdf_page: 66
    - "no": 11
      title: Relations between $\mathbf{S}(M^*)$, TS(M)*gr and Pol(M, A)
      page: 59
      pdf_page: 68
statements: 36
exercises: 16
content_sha256: 6da98969b53ee5df6cf503b3f80c244de4578e27ef1ee1edd5bf16c915b72321
---

## § 5. SYMMETRIC TENSORS AND POLYNOMIAL MAPPINGS

### 1. Relative traces

Let H be a group and M a left A[H]-module $^{(1)}$. We shall denote by $M^H$ the set of all $m \in M$ such that $hm = m$ for all $h \in H$ $^{(2)}$; this is a sub-A-module of M.

Let G be a subgroup of H, then $M^G$ is a sub-A-module of M containing $M^H$.

Given $m \in M^G$, $h \in H$, if $x = hG$ is the left coset of h modulo G, then we have $xm = hGm = \{hm\}$. By abuse of notation the element $hm$ of M will be written xm. If $h' \in H$, we have

(1)
$$
h'(xm) = (h'x) m .
$$

Suppose from now on that G is of finite index in H. Then

(2)
$$
\sum_{x \in H/G} xm \in M^H .
$$

For, given $h' \in H$, we have by virtue of (1),

$$
h' \left( \sum_{x \in H/G} xm \right) = \sum_{x \in H/G} (h'x) m = \sum_{y \in H/G} ym .
$$

(1) We denote by A[H] the group algebra of H (III, p. 446).
(2) Care should be taken not to confuse this notation with that introduced in the study of products of sets (*Set Theory*, II, p. 102).

#### Definition 1 {#alg-iv-s5-def-1 .statement}

— If G *is* of finite index in H, we denote by $\mathrm{Tr}_{H/G}$ the mapping of $M^G$ into $M^H$ defined by

$$
\mathrm{Tr}_{H/G} m = \sum_{x \in H/G} x m .
$$

This mapping is a homomorphism of the A-module $M^G$ into the A-module $M^H$.

#### Proposition 1 {#alg-iv-s5-prop-1 .statement}

— (i) Let $m \in M^G$ and $h \in H$. Then $hm \in M^{hGh^{-1}}$ and

$$
\mathrm{Tr}_{H/hGh^{-1}}(hm) = \mathrm{Tr}_{H/G} m .
$$

(ii) Let F be a subgroup of G of finite index in G, and let $m \in M^F$, then

$$
\mathrm{Tr}_{H/G}(\mathrm{Tr}_{G/F} m) = \mathrm{Tr}_{H/F} m
$$

(iii) *If* $m \in M^H$, then $\mathrm{Tr}_{H/G} m = (H : G) \cdot m$.

(i) Let $h \in H$. For $h' \in H$ and $m \in M$ let us put $\varphi(h') = hh'h^{-1}$ and $\psi(m) = hm$. We have $\varphi(h') \psi(m) = \psi(h'm)$; by transfer of structure we deduce that if $m \in M^G$, then $hm \in M^{hGh^{-1}}$ and

$$
\mathrm{Tr}_{H/hGh^{-1}}(hm) = \psi(\mathrm{Tr}_{H/G}(m)) .
$$

Since $\mathrm{Tr}_{H/G}(m) \in M^H$, this proves (i).

(ii) Let $m \in M^F$ and let $(g_\alpha)_\alpha \in_A$ be a system of representatives of the left cosets of G mod F, and $(h_\beta)_\beta \in_B$ a system of representatives of the left cosets of H mod G. Then $(h_\beta g_\alpha)_{(\beta,\alpha) \in B \times A}$ is a system of representatives of the left cosets of H mod F. so

$$
\begin{align*}
\mathrm{Tr}_{H/G}(\mathrm{Tr}_{G/F} m) &= \sum_{\beta \in B} h_\beta \left( \sum_{\alpha \in A} g_\alpha m \right) \\
&= \sum_{(\beta,\alpha) \in B \times A} (h_\beta g_\alpha) m = \mathrm{Tr}_{H/F} m .
\end{align*}
$$

(iii) This assertion is evident.

### 2. Definition of symmetric tensors

Let M be an A-module. We recall (III, p. 501) that $\mathfrak{S}_n$ operates on the left of the A-module $T^n(M)$, in such a way that

$$
\sigma(x_1 \otimes x_2 \otimes \ldots \otimes x_n) = x_{\sigma^{-1}(1)} \otimes x_{\sigma^{-1}(2)} \otimes \ldots \otimes x_{\sigma^{-1}(n)}
$$

for any $x_1, \ldots, x_n \in M$ and $\sigma \in \mathfrak{S}_n$. The elements $z \in T^n(M)$ such that $\sigma \cdot z = z$ for all $\sigma \in \mathfrak{S}_n$ are called symmetric tensors of order n; they form a sub-A-module of $T^n(M)$ denoted by $\mathbf{TS}^n(M)$; we have $\mathbf{TS}^0(M) = A, \mathbf{TS}^1(M) = M$. We shall put

TS(M) = $\bigoplus_{n=0}^{\infty} TS^n(M)$; this is a graded sub-A-module of $\mathbf{T}(M)$. For every $z \in T^n(M)$ the element $\sum_{\sigma \in S_n} \sigma . z$ belongs to $TS^n(M)$; we denote it by $s . z$ and call it the symmetrization of $z$. The mapping $s : z \mapsto s . z$ is a homomorphism of the A-module $T^n(M)$ into the A-module $TS^n(M)$. If $z \in TS^n(M)$, then $s . z = n! \ z$.

### 3. Product for symmetric tensors

Let $p, q \in \mathbf{N}$ and let $S_{p|q}$ be the subgroup of $S_{p+q}$ consisting of all permutations $\sigma \in S_{p-q}$ which leave the intervals $(1, p)$ and $(p+1, p+q)$ of $\mathbf{N}$ stable. If $\sigma \in S_p$ and $\sigma' \in S_q$, we can define an element $\sigma''$ of $S_{p|q}$ by putting $\sigma''(n) = \sigma(n)$ for $1 \leq n \leq p$ and $\sigma''(p+n) = p + \sigma'(n)$ for $1 \leq n \leq q$; the mapping $(\sigma, \sigma') \mapsto \sigma''$ is an isomorphism of $S_p \times S_q$ onto $S_{p|q}$.

Let $z \in TS^p(M)$, $z' \in TS^q(M)$, then the element $z \otimes z'$ of $T^{p+q}(M)$ is invariant under $S_{p|q}$; we can therefore define the element $\operatorname{Tr}_{S_{p+q}/S_{p|q}}(z \otimes z')$ of $TS^{p+q}(M)$. We shall equip $TS(M)$ with the A-bilinear multiplication $(y, y') \mapsto yy'$ such that for $p, q \in \mathbf{N}$, $z \in TS^p(M)$, $z' \in TS^q(M)$ we have

$$
zz' = \operatorname{Tr}_{S_{p+q}/S_{p|q}}(z \otimes z')
$$

If $y \in TS(M)$ and $y' \in TS(M)$, we shall call $yy'$ the symmetric product of $y$ and $y'$. The family $(TS^p(M))_p$, , is a graduation of type $\mathbf{N}$ of the algebra $TS(M)$, and the unit element of $\mathbf{T}(M)$ is a unit element of $TS(M)$.

Let $S_{p,q}$ be the set of those $\sigma \in S_{p+q}$ such that

$$
\begin{align*}
&\sigma(1) < \sigma(2) < \ldots < \sigma(p) \\
&\sigma(p+1) < \sigma(p+2) < \ldots < \sigma(p+q).
\end{align*}
$$

The mapping $(\sigma, \tau) \mapsto \sigma \tau$ of $S_{p,q} \times S_{p|q}$ into $S_{p+q}$ is bijective (I, p. 60, Example 2); hence if $z \in TS^p(M)$ and $z' \in TS^q(M)$, we have

$$
zz' = \sum_{\sigma \in S_{p,q}} \sigma(z \otimes z')
$$

#### Proposition 2 {#alg-iv-s5-prop-2 .statement}

— (i) The A-algebra $TS(M)$ is associative, commutative and unital.

(ii) Let $p_1, \ldots, p_n$ be integers $> 0$, and let $S_{p_1| \ldots |p_n}$ be the set of all $\sigma \in S_{p_1+\cdots+p_n}$ leaving the following intervals of $\mathbf{N}$ stable:

$$
(1, p_1), (p_1+1, p_1+p_2), \ldots, (p_1+\cdots+p_{n-1}+1, p_1+\cdots+p_n).
$$

Let $z_1 \in \mathbf{TS}^{p_1}(M) , \ldots , z_n \in \mathbf{TS}^{p_n}(M)$, then

$$
z_1 z_2 \ldots z_n = \operatorname{Tr}_{\mathfrak{S}_{p_1 + \cdots + p_n}/\mathfrak{S}_{p_1}| \cdots | p_n} (z_1 \otimes z_2 \otimes \ldots \otimes z_n) .
$$

In particular if $x_1, \ldots, x_r \in M$, we have $x_1 \ldots x_r = s(x_1 \otimes \ldots \otimes x_r)$.

The assertion (ii) is clear for $n = 1$. Assume that the relation

$$
z_2 \ldots z_n = \operatorname{Tr}_{\mathfrak{S}_{p_2 + \cdots + p_n}/\mathfrak{S}_{p_2}| \cdots | p_n} (z_2 \otimes \ldots \otimes z_n)
$$

has been proved, and let us identify $\mathfrak{S}_{p_2 + \cdots + p_n}$ with the subgroup of $\mathfrak{S}_{p_1 + \cdots + p_n}$ consisting of all permutations whose restriction to $(1, p_1)$ is the identity. Then

$$
\operatorname{Tr}_{\mathfrak{S}_{p_1}|p_2+\cdots+p_n/\mathfrak{S}_{p_1}|p_2| \cdots | p_n} (z_1 \otimes z_2 \otimes \ldots \otimes z_r) =
$$
$$
= z_1 \otimes \operatorname{Tr}_{\mathfrak{S}_{p_2+\cdots+p_n}/\mathfrak{S}_{p_2}| \cdots | p_n} (z_2 \otimes \ldots \otimes z_r) = z_1 \otimes (z_2 \ldots z_n) .
$$

Hence we have

$$
z_1 z_2 \ldots z_r = z_1 (z_2 \ldots z_r) =
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2+\cdots+p_n}/\mathfrak{S}_{p_1}|p_2-\cdots+p_n} (z_1 \otimes (z_2 \ldots z_n))
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+\cdots+p_n}/\mathfrak{S}_{p_1}|p_2+\cdots+p_n} (\operatorname{Tr}_{\mathfrak{S}_{p_1}|p_2+\cdots+p_n/\mathfrak{S}_{p_1}|p_2| \cdots | p_n} (z_1 \otimes z_2 \otimes \ldots \otimes z_n))
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1-\cdots+p_n}/\mathfrak{S}_{p_1}| \cdots | p_n} (z_1 \otimes z_2 \otimes \ldots \otimes z_n)
$$

by Prop. 1, (ii) of IV, p. 42. Thus (ii) is established.

In particular,

$$
z_1 (z_2 z_3) = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2+p_3}/\mathfrak{S}_{p_1}|p_2|p_3} (z_1 \otimes z_2 \otimes z_3) ,
$$

and in the same way we show that

$$
(z_1 z_2) z_3 = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2+p_3}/\mathfrak{S}_{p_1}|p_2|p_3} (z_1 \otimes z_2 \otimes z_3) .
$$

Hence the algebra $\mathbf{TS}(M)$ is associative.

Let $o$ be the element of $\mathfrak{S}_{p_1+p_2}$ such that

$$
\begin{align*}
\sigma(1) &= p_2 + 1, \; \sigma(2) = p_2 + 2, \; \ldots, \; \sigma(p_1) = p_2 + p_1 , \\
\sigma(p_1 + 1) &= 1, \; \sigma(p_1 + 2) = 2, \; \ldots, \; \sigma(p_1 + p_2) = p_2 .
\end{align*}
$$

Then

$$
z_2 z_1 = \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\mathfrak{S}_{p_2}|p_1} (z_2 \otimes z_1)
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\sigma \mathfrak{S}_{p_1}|p_2 \sigma^{-1}\sigma} (z_1 \otimes z_2)
$$
$$
= \operatorname{Tr}_{\mathfrak{S}_{p_1+p_2}/\mathfrak{S}_{p_1}|p_2} (z_1 \otimes z_2) \quad \text{by Prop 1, (i)}
$$
$$
= z_1 z_2 .
$$

Hence the algebra $\mathbf{TS}(M)$ is commutative.

It is to be noted that the canonical injection of $\mathbf{TS}(M)$ in $\mathbf{T}(M)$ is not in general an algebra homomorphism. Worse still, $\mathbf{TS}(M)$ is not in general stable under the multiplication of $\mathbf{T}(M)$.

### 4. Divided powers

Let $x \in M$ and $k \in \mathbf{N}$. It is clear that $x, \otimes x_2 \otimes \ldots \otimes x_k$, where
$$
x_1 = x_2 = \cdots = x_k = x ,
$$
is an element of $\mathbf{TS}^k(M)$.

#### Definition 2 {#alg-iv-s5-def-2 .statement}

*If* $x \in M$, *the element* $x \otimes x \otimes \ldots \otimes x$ *of* $\mathbf{TS}^k(M)$ *is denoted by* $\gamma_k(x)$.

#### Proposition 3 {#alg-iv-s5-prop-3 .statement}

(i) *If* $x \in M$, *the pth power of* $x$, *calculated in* $\mathbf{TS}(M)$, *is equal to* $p! \; \gamma_p(x)$.
(ii) *Let* $x,, \ldots, x, \in M$; *then*
$$
\gamma_p(x_1 + x_2 + \cdots + x_n) = \sum_{p_1 + p_2 + \cdots + p_n = p} \gamma_{p_1}(x_1) \; \gamma_{p_2}(x_2) \ldots \gamma_{p_n}(x_n) .
$$
(iii) *Let* $x,, \ldots, x_n \in M$, *let* $p_1, \ldots, p$, *be integers* $\geqslant 0$ *and* $p = p_1 + \ldots + p_n$. *Let* $E$ *be the set of mappings* $\varphi$ *of* $\{1, \ldots, p\}$ *into* $(1, \ldots, n)$ *such that*
$$
\operatorname{Card} \varphi^{-1}(1) = p_1, \ldots, \operatorname{Card} \varphi^{-1}(n) = p_n .
$$
*Then*
$$
\gamma_{p_1}(x_1) \; \gamma_{p_2}(x_2) \ldots \gamma_{p_n}(x_n) = \sum_{\varphi \in E} x_{\varphi(1)} \otimes x_{\varphi(2)} \otimes \ldots \otimes x_{\varphi(p)} .
$$
(iv) *Let* $x \in M$ *and let* $q, r$ *be integers* $\geqslant 0$. *Then*
$$
\gamma_q(x) \; \gamma_r(x) = \frac{(q + r)!}{q! \; r!} \; \gamma_{q + r}(x) .
$$
(v) *Let* $x_1, \ldots, x, \in M$, *and for* $H \subset (1, \ldots, n)$ *put* $x_H = \sum_{i \in H} x_i$, *then*
$$
(-1)^n x_1 x_2 \ldots x_n = \sum_{H \subset \{1, \ldots, n\}} (-1)^{\operatorname{Card} H} \gamma_n(x_H) .
$$

The assertion (i) follows at once from Prop. 2 (ii).

Let us prove (ii); by an induction on n we see that it is enough to consider the case $n = 2$. Then we have

$$
\gamma_p(x_1 + x_2) = (x_1 + x_2) \otimes (x_1 + x_2) \otimes ... \otimes (x_1 + x_2) \quad @\text{factors})
$$
$$
= \sum_{p_1 + p_2 = p} \sum_{\sigma \in S_{p_1, p_2}} \sigma(x_1 \otimes x_1 \otimes ... \otimes x_1 \otimes x_2 \otimes x_2 \otimes ... \otimes x_2)
$$
$$
= \sum_{p_1 + p_2 = p} \sum_{\sigma \in S_{p_1, p_2}} \sigma(\gamma_{p_1}(x_1) \otimes \gamma_{p_2}(x_2))
$$
$$
= \sum_{p_1 + p_2 = p} \gamma_{p_1}(x_1) \gamma_{p_2}(x_2).
$$

To prove (iii), let $S_{p_1, ..., p_n}$ be the set of permutations of $(1, p_1 + ... + p_n)$ whose restrictions to the intervals
$$(1, p_1), (p_1 + 1, p_1 + p_2), ..., (p_1 + ... + p_{n-1} + 1, p_1 + ... + p_n)$$
are increasing. By I, p. 60, example 2 and Prop. 2, (ii) we have
$$
\gamma_{p_1}(x_1) \gamma_{p_2}(x_2) ... \gamma_{p_n}(x_n) = \sum_{\rho \in S_{p_1, p_2, ..., p_n}} \rho(x_1 \otimes x_1 \otimes ... \otimes x_1 \otimes x_2 \otimes x_2 \otimes ... \otimes x_2 \otimes ... \otimes x_n \otimes x_n \otimes ... \otimes x_n)
$$
(with $p_i$ factors $x_i$) and this sum is equal to
$$
\sum_{\varphi \in E} x_{\varphi(1)} \otimes x_{\varphi(2)} \otimes ... \otimes x_{\varphi(p)}.
$$

In (iii) let us put $n = 2, x_1 = x_2 = x, p_1 = q$ and $p_2 = r$, then we obtain (iv) (I, loc. cit.).

Finally (v) follows from Prop. 2, (ii) and Prop. 2 of I, p. 100, applied to the elements $x_i$ of the ring $\mathbf{T}(M)$.

#### Remark 1 {#alg-iv-s5-n4-rem-1 .statement}

Let $(x_i)_{i \in I}$ be a family of elements of M. For each $\nu \in \mathbf{N}^{(1)}$ put
$$
x_\nu = \prod_{i \in I} \gamma_{\nu_i}(x_i).
$$
If $(\lambda_i) \in \mathbf{A}^{(1)}$ and $p \in \mathbf{N}$, then we have by Prop. 3 (ii),
$$
\gamma_p \left( \sum_{i \in I} \lambda_i x_i \right) = \sum_{\nu \in \mathbf{N}^{(1)}, |\nu| = p} \lambda^\nu x_\nu.
$$
(6)

#### Remark 2 {#alg-iv-s5-n4-rem-2 .statement}

Let $\mathcal{M}$ be the set of mappings of $(1, p)$ into I. We define a mapping $\rho \mapsto \rho^*$ of $\mathcal{M}$ into $\mathbf{N}^{(1)}$ by putting
$$
\rho^*(i) = \operatorname{Card} \rho^{-1}(i)
$$

For two elements $\rho_1, \rho_2$ of $\mathcal{M}$ to satisfy $\rho_1^* = \rho_2^*$ it is necessary and sufficient that there should exist $\sigma \in \mathfrak{S}_p$ such that $\rho_2 = \rho_1 \circ \sigma$ (I, p. 95). By Prop. 3 (iii) we have, for $|\nu| = p$,

$$
x_\nu = \sum_{\rho \in \mathcal{M}, \rho^* = \nu} x_{\rho(1)} \otimes x_{\rho(2)} \otimes \ldots \otimes x_{\rho(p)}
$$

### 5. Symmetric tensors over a free module

#### Proposition 4 {#alg-iv-s5-prop-4 .statement}

— Let $M$ be free and $(e_i)_{i \in I}$ a basis of $M$.

(i) For $\nu \in \mathbf{N}^{(I)}$ let $e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i)$. Then $(e,)_{\nu \in \mathbf{N}^{(I)}}$ is a basis of the $A$-module $TS(M)$. In particular the algebra $\mathbf{TS}(M)$ is generated by the family of elements $\gamma_k(x)$ for $k \in N$ and $x \in M$.

(ii) For each $p \in N$, $\mathbf{TS}^p(M)$ is a direct factor of the $A$-module $\mathbf{T}^p(M)$.

Let us use the notation of the Remark 2 above. The family $(e_{\rho(1)} \otimes \ldots \otimes e_{\rho(p)})_{\rho \in \mathcal{M}}$ is a basis of $\mathbf{T}^p(M)$. Hence Prop. 4 follows from formula (7) and the following lemma, applied with $H = \mathfrak{S}_p$ and $U = \mathbf{T}^p(M)$.

#### Lemma 1 {#alg-iv-s5-lem-1 .statement}

Let $H$ be a finite group and $U$ a left $A[H]$-module. Suppose that the $A$-module $U$ has a basis $B$ which is stable under the operations of $H$ in $U$, and put $\Omega = B/H$. For each $w \in \Omega$ let $u_w = \sum_{b \in w} b$; then

(i) $(u_w)_{w \in \Omega}$ is a basis of the $A$-module $U^H$.

(ii) For each $\omega \in \Omega$ let $v$, be a point of $\omega$; put $\omega' = w - \{v_\omega\}$ and $B' = \bigcup_{\omega \in \Omega} w'$, then $B'$ is a basis of a supplementary subspace for $U^H$ in $U$.

The union of the set of all $u_w$ (for $\omega \in \Omega$) and of $B'$ is a basis of $U$. If $U' = \sum_{\omega \in \Omega} Au$, and $U'' = \sum_{b \in B'} Ab$, we therefore have $U = U' \oplus U''$. On the other hand, we have $u_w \in U^H$ for all $w \in \Omega$, hence $U' \subset U^H$. Finally, let $(\alpha_b)_{b \in B}$ be a family of elements of $A$ with finite support and let $x = \sum_{b \in B} \alpha_b b$. If $x \in U^H$, then $\alpha_{hb} = \alpha_b^H$ for all $b \in B$ and all $h \in H$, hence $x \in U'$, and it follows that $U' = u^H$.

#### Proposition 5 {#alg-iv-s5-prop-5 .statement}

— Let $M$ be a free $A$-module, $k$ an integer $\geq 0$, $P$ the sub-$A$-module of $\mathbf{TS}^k(M)$ generated by $\gamma_k(M)$. Assume $A$ to be an infinite integral domain. Then for each $z \in \mathbf{TS}^k(M)$ there exists $a \in A - \{0\}$ such that $az \in P$.

Let $K$ be the field of fractions of $A$. We identify $\mathbf{TS}^k(M)$ with a sub-A-module of the vector K-space $V = \mathbf{TS}^k(M) \otimes_A K$ (Prop. 4, and II, p. 314). We have to show that this vector K-space is generated by $\gamma_k(M)$, that is, every K-linear form $f$ on V satisfying $f(\gamma_k(M)) = 0$ is zero. Let $(e_i)_{i \in I}$ be a basis of M, and define the e, as in Prop. 4. For any $(\alpha_i) \in A^{(I)}$ we have, on taking (6) into account,

$$
0 = f \left( \gamma_k \left( \sum_{i \in I} \alpha_i e_I \right) \right) = \sum_{\nu \in N^{(I)}, |\nu| = k} \alpha^\nu f(e_\nu).
$$

By Cor. 2 of IV, p. 18 it follows that $f(e_v) = 0$ for all $v \in N^{(I)}$, whence $f = 0$.

### 6. The functor TS

Let M, N be A-modules and u a homomorphism of M into N; it is clear that $T(u)(TS(M)) \subset TS(N)$. The mapping of TS(M) into TS(N) obtained from T(u) is denoted by TS(u). It is easily verified that this is a unital homomorphism of graded algebras and we have TS(u) $(\gamma_p(x)) = \gamma_p(u(x))$ for all $x \in M$ and each integer $p \geq 0$. If $v : N \to P$ is a homomorphism of A-modules, we have

$$
TS(v \circ u) = TS(v) \circ TS(u).
$$

By definition of TS(u), the diagram

$$
\begin{array}{cccc}
M & \longrightarrow & TS(M) \longrightarrow T(M) \\
u \downarrow & & \downarrow TS(u) & \downarrow T(u) \\
N & \longrightarrow & TS(N) \longrightarrow T(N)
\end{array}
$$

is commutative, where the horizontal arrows denote canonical injections.

If M is a direct factor of N and i : M \to N is the canonical injection, then TS(i) is an injective homomorphism of TS(M) onto a direct factor R of TS(N), by which we normally identify TS(M) and R. That is proved as for the tensor algebra (III, p. 487).

Suppose that M is a direct sum of a family $(M_\lambda)_{\lambda \in L}$ of submodules. The canonical injections $TS(M_\lambda) \to TS(M)$ define a unital homomorphism h of graded algebras, called canonical:

$$
\bigotimes_{\lambda \in L} TS(M_\lambda) \to TS(M)
$$

Let $\lambda_1, \lambda_2, \ldots, \lambda_n$ be pairwise distinct elements of L and let $x_1 \in M_{\lambda_1}, \ldots, x_n \in M_{\lambda_n}$. By Prop. 3, (ii) of IV, p. 45 we have

$$
h \left( \sum_{p_1 + \cdots + p_n = p} \gamma_{p_1}(x_1) \otimes \cdots \otimes \gamma_{p_n}(x_n) \right) = \gamma_p(x_1 + \cdots + x_n).
$$

Let $N$ be an $A$-module which is a direct sum of a family $(N_\lambda)_\lambda$, of submodules. For every $\lambda \in L$ let $u_\lambda$ be a homomorphism of $M_\lambda$ into $N_\lambda$. Let $u$ be the homomorphism of $M$ into $N$ defined by the $u_\lambda$. Then the diagram

$$
\begin{array}{ccc}
\otimes \mathbf{TS}(M_\lambda) & \xrightarrow{h} & \mathbf{TS}(M) \\
\downarrow & & \downarrow \mathbf{TS}(u) \\
\otimes \mathbf{TS}(u_\lambda) & & \\
\downarrow & & \\
\otimes \mathbf{TS}(N_\lambda) & \xrightarrow{h'} & \mathbf{TS}(N)
\end{array}
$$

commutes, where $h$ and $h'$ are canonical homomorphisms. For if $z \in TS(M_\lambda)$ and if $i_\lambda$ (resp. $j_\lambda$) denotes the canonical injection of $M_\lambda$ into $M$ (resp. $N$, into $N$), then we have

$$
\mathbf{TS}(u)(h(z)) = \mathbf{TS}(u) \circ \mathbf{TS}(i_\lambda)(z) = \mathbf{TS}(u \circ i_\lambda)(z) =
$$
$$
= \mathbf{TS}(j_\lambda \circ u_\lambda)(z) = \mathbf{TS}(j_\lambda) \circ \mathbf{TS}(u_\lambda)(z) = h'(\mathbf{TS}(u_\lambda)(z)) .
$$

#### Proposition 6 {#alg-iv-s5-prop-6 .statement}

— *Let $M$ be an $A$-module which is the direct sum of a family $(M_\lambda)_\lambda$, of submodules. If each $M_\lambda$ is a free module, then the canonical homomorphism of $\otimes_{\lambda \in L} \mathbf{TS}(M_\lambda)$ into $\mathbf{TS}(M)$ is an isomorphism.*

Let $(e_{i,\lambda})_{i, I_\lambda}$ be a basis of $M_\lambda$. For $\nu \in \mathbf{N}^{(I_\lambda)}$ put $e_{\nu,\lambda} = \prod_{i \in I_\lambda} \gamma_{\nu(i)}(e_{i,\lambda})$. The $e_{\nu,\lambda}$ for $\nu \in \mathbf{N}^{(I_\lambda)}$ form a basis of $TS(M_\lambda)$ (IV, p. 47, Prop. 4 (i)) and $e_{0,\lambda}$ is the unit-element of $\mathbf{TS}(M_\lambda)$. Therefore the elements

$$
\otimes_{\lambda \in L} e_{\nu_{\lambda,\lambda}}
$$

where $\nu_\lambda \in \mathbf{N}^{(I_\lambda)}$ and $\nu_\lambda = 0$ except for a finite number of indices, form a basis of $\otimes_A TS(M_\lambda)$. The image of the element (9) under the canonical homomorphism of the proposition is $\prod_{\lambda \in L} e_{\nu_{\lambda,\lambda}}$. If we denote by $(e_i)_i$, the disjoint union of the families $(e_{i,\lambda})_{i, I_\lambda}$, then the above elements are precisely $\prod_{i \in I} \gamma_{\nu(i)}(e_i)$, where $\nu \in \mathbf{N}^{(I)}$, and so they constitute a basis of $\mathbf{TS}(M)$. This proves the proposition.

Under the conditions of Prop. 6, the inverse isomorphism $\mathbf{TS}(M) \to \otimes_{\lambda} \mathbf{TS}(M_\lambda)$ is also called *canonical*. Frequently $\mathbf{TS}(M)$ is identified with $\otimes_{\lambda} TS(M_\lambda)$ by means of this isomorphism. It should be noted that if $z \in TS(M_\lambda)$ and $z' \in \mathbf{TS}(M_{\mu})$ with $\lambda \neq \mu$, then the element of $\mathbf{TS}(M)$ which we are thus led to denote by $z \otimes z'$ is not the tensor product of $z$ and $z'$ in $\mathbf{T}(M)$ but the symmetric product of $z$ and $z'$.

#### Proposition 7 {#alg-iv-s5-prop-7 .statement}

*Let $M$ be an $A$-module, $u$ the mapping $(x, y) \mapsto x + y$ of $M \oplus M$ into $M$ and $f$ the composite mapping*

$$
\mathbf{TS}(M) \otimes \mathbf{TS}(M) \xrightarrow{h} \mathbf{TS}(M \oplus M) \xrightarrow{\mathbf{TS}(u)} \mathbf{TS}(M)
$$

*where $h$ is the canonical homomorphism. If $z, z' \in \mathbf{TS}(M)$, then $f(z \otimes z') = zz'$.*

For let $i$ be the mapping $x \mapsto (x, 0)$ of $M$ into $M \oplus M$. We have $u \circ i = \mathrm{Id}_M$, hence $\mathbf{TS}(u) \circ \mathbf{TS}(i) = \mathrm{Id}_{\mathbf{TS}(M)}$; therefore

$$
f(z \otimes 1) = \mathbf{TS}(u)(h(z \otimes 1)) = \mathbf{TS}(u)(\mathbf{TS}(i)(z)) = z .
$$

Likewise $f(1 \otimes z') = z'$, whence $f(z \otimes z') = f(z \otimes 1) f(1 \otimes z') = zz'$.

### 7. Coproduct for symmetric tensors

Let $M$ be a *free* $A$-module, and $\Delta_M = A$ the diagonal homomorphism $x \mapsto (x, x)$ of $M$ into $M \oplus M$. Let $c_M = c$ be the unital homomorphism of graded $A$-algebras composed of the homomorphisms :

$$
\mathbf{TS}(M) \xrightarrow{\mathbf{TS}(\Delta)} \mathbf{TS}(M \oplus M) \xrightarrow{\sigma} \mathbf{TS}(M) \otimes \mathbf{TS}(M)
$$

where $\sigma$ is the canonical isomorphism. Equipped with $c$, $\mathbf{TS}(M)$ is a graded $A$-cogebra.

For all $x \in M$ and each integer $p \geq 0$ we have $\mathbf{TS}(A)(\gamma_p(x)) = \gamma_p((x, x))$, hence by (8),

$$
c(\gamma_p(x)) = \sum_{r+s=p} \gamma_r(x) \otimes \gamma_s(x).
$$

In particular

$$
c(x) = x \otimes 1 + 1 \otimes x .
$$

Let $(x_i)_{i \in I}$ be a family of elements of $M$, and for $\nu \in \mathbf{N}^{(I)}$ put $x_\nu = \prod_{i \in I} \gamma_{\nu_i}(x_i)$.

Then

$$
c(x_\nu) = \sum_{\rho + \sigma = \nu} x_\rho \otimes x_\sigma .
$$

This follows from *(10)* because $c$ is an algebra homomorphism.

#### Proposition 8 {#alg-iv-s5-prop-8 .statement}

— Let M be a free A-module, then with its algebra and cogebra structures, TS (M) is a graded commutative and cocommutative bigebra. The counit is the A-linear mapping $\varepsilon : TS(M) \to TS^0(M) = A$ which is zero on $TS^p(M)$ for $p > 0$ and such that $\varepsilon(1) = 1$.

We know that the A-algebra $TS(M)$ is associative, commutative and unital. On the other hand, the coproduct is by construction a homomorphism of graded algebras; now the fact that the cogebra $TS(M)$ is coassociative and cocommutative follows by an easy calculation from the Formula (10). The mapping $\varepsilon$ of $TS(M)$ into A is a homomorphism of graded algebras such that $\varepsilon(l) = l$. Finally for every $x \in M$ we have $\varepsilon(\gamma_p(x)) = 0$ if $p > 0$, $\varepsilon(\gamma_0(x)) = l$; if we bear in mind (lo), this shows that $(F \otimes 1) \circ c = (l \otimes E) \circ c = \mathrm{Id}_{TS(M)}$; thus $E$ is the counit of $TS(M)$.

#### Proposition 9 {#alg-iv-s5-prop-9 .statement}

— Let M and N be free A-modules and u an A-homomorphism of M into N ; then $\mathbf{TS}(u)$ is a bigebra homomorphism.

For we have $\Delta_N \circ u = (u,u) \circ \Delta_M$, hence the diagram

$$
\begin{array}{ccccccccc}
\mathbf{TS}(M) & \xrightarrow{\mathbf{TS}(\Delta_M)} & \mathbf{TS}(M \oplus M) & \xrightarrow{\sigma} & \mathbf{TS}(M) \otimes \mathbf{TS}(M) \\
\downarrow \mathbf{TS}(u) & & \downarrow \mathbf{TS}(u,u) & & \downarrow \mathbf{TS}(u) \otimes \mathbf{TS}(u) \\
\mathbf{TS}(N) & \xrightarrow{\mathbf{TS}(\Delta_N)} & \mathbf{TS}(N \oplus N) & \xrightarrow{\tau} & \mathbf{TS}(N) \otimes \mathbf{TS}(N),
\end{array}
$$

where $\sigma$ and $\tau$ are canonical isomorphisms, is commutative (IV, p. 49). Thus $c_N \circ \mathbf{TS}(u) = (\mathbf{TS}(u) \otimes \mathbf{TS}(u)) \circ c_M$.

#### Proposition 10 {#alg-iv-s5-prop-10 .statement}

— Let M be a free A-module, then the primitive elements (III, p. 602) of the bigebra $\mathbf{TS}(M)$ are the elements of M.

Let $(e_i)_{i \in I}$ be a basis of M, and for $v \in \mathbf{N}^{(I)}$ put $e_v = \prod_{i \in I} \gamma_{v_i}(e_i)$. Let $z = \sum_{v \in \mathbf{N}^{(I)}} \lambda_v e_v$ be an element of $\mathbf{TS}(M)$, then by (12) we have

$$
c(z) = \sum_v \lambda_v \sum_{\rho, \sigma \in \mathbf{N}^{(I)}, \rho + \sigma = v} e_\rho \otimes e_\sigma = \sum_{\rho, \sigma} \lambda_{\rho + \sigma} e_\rho \otimes e_\sigma
$$

hence

$$
c(z) - 1 \otimes z - z \otimes 1 = \sum_{\rho \neq 0, \sigma \neq 0} \lambda_{\rho + \sigma} e_\rho \otimes e_\sigma - \lambda_0 e_0 \otimes e_0
$$

and so

zprimitive $\Leftrightarrow \lambda_{\rho + \sigma} = 0$ when $\rho \neq 0$ and $\sigma \neq 0$ and $\lambda_0 = 0$
$\Leftrightarrow \lambda_v = 0$ when $|v| \neq 1$
$\Leftrightarrow z \in M$.

### 8. Relations between TS(M) and S(M)

The canonical injection of M in TS(M) extends in a unique fashion to an algebra homomorphism of T(M) into TS(M) (III, p. 485, Prop. 1). By Prop. 2, (ii) of IV, p. 43, this homomorphism is the operators of symmetrization. Since the algebra TS(M) is commutative there exists (III, p. 497) one and only one algebra homomorphism $\varphi_M$, called canonical, of the algebra S(M) into the algebra TS(M) such that the diagram

$$
\begin{array}{ccc}
T(M) & \xrightarrow{\rho} & S(M) \\
& & \searrow s \\
& & TS(M)
\end{array}
$$

where $\rho$ denotes the canonical homomorphism of T(M) onto S(M), is commutative. We have $\varphi_M(S^p(M)) \subset TS^p(M)$ for all $p \in \mathbf{N}$.

On the other hand, by composing the canonical injection i of TS(M) into T(M) with the canonical homomorphism $\rho$ of T(M) onto S(M) we obtain a homomorphism $\psi_M$ of graded A-modules, called canonical. The diagram

$$
\begin{array}{ccc}
TS(M) & \xrightarrow{\psi_M} & S(M) \\
& & \downarrow \rho \\
& & T(M)
\end{array}
$$

is commutative.

If $u : M \to N$ is a homomorphism of A-modules, then the diagram

$$
\begin{array}{ccccccccc}
S(M) & \xrightarrow{\varphi_M} & TS(M) & \xrightarrow{\psi_M} & S(M) \\
| & & | & & | \\
S(N) & \xrightarrow{\varphi_N} & TS(N) & \xrightarrow{\psi_N} & S(N)
\end{array}
$$

is commutative, as is easily verified.

If M is the direct sum of the modules $M_\lambda$, the diagram (14)

$$
\begin{array}{ccc}
\otimes S(M_\lambda) & \xrightarrow{\otimes \varphi_{M_\lambda}} & \otimes TS(M_\lambda) \\
\downarrow f & & \downarrow g \\
S(M) & \xrightarrow{\varphi_M} & TS(M),
\end{array}
$$

where $f$ and $g$ are the canonical homomorphisms, is commutative. For $g \circ \otimes \varphi_{M_\lambda}$ and $\varphi_M \circ f$ are algebra homomorphisms which coincide on $M_\lambda$ for every $\lambda$.

#### Proposition 11 {#alg-iv-s5-prop-11 .statement}

— *If $M$ is free, then $\varphi_M$ is a morphism of graded bigebras.*

Using the commutativity of the diagrams (13) and (14), we obtain the commutative diagram

$$
\begin{array}{ccccccccc}
S(M) & \xrightarrow{S(\Delta)} & S(M \oplus M) & \xrightarrow{h} & S(M) \otimes S(M) \\
\downarrow \varphi_M & & \downarrow \varphi_{M \oplus M} & & \downarrow \varphi_M \otimes \varphi_M \\
TS(M) & \xrightarrow{TS(\Delta)} & TS(M \oplus M) & \xrightarrow{k} & TS(M) \otimes TS(M),
\end{array}
$$

where $\Delta$ is the diagonal homomorphism and $h, k$ are canonical homomorphisms. The proposition follows from this.

#### Proposition 12 {#alg-iv-s5-prop-12 .statement}

— (i) *If $u \in S^n(M)$, then $\psi_M(\varphi_M(u)) = n!u$.*

(ii) *If $v \in TS^n(M)$ then $\varphi_M(\psi_M(v)) = n!v$.*

Let $x_1, \ldots, x_n \in M$ and let $u$ be the product $x_1 \ldots x_n$ calculated in $S(M)$. Then $\varphi_M(u)$ is the product $x_1 \ldots x_n$ calculated in $TS(M)$, that is

$$
\sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \otimes \ldots \otimes x_{\sigma(n)}.
$$

Hence $\psi_M(\varphi_M(u))$ equals $\sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \ldots x_{\sigma(n)}$ calculated in $S(M)$, that is

$$
n! x_1 \ldots x_n = n!u.
$$

Let $v = \sum_{i=1}^p x_1^i \otimes x_2^i \otimes \ldots \otimes x_n^i$ be an element of $TS^n(M)$, where the $x_j^i$ belong to $M$; then $\psi_M(v)$ is equal to $\sum_{i=1}^p x_1^i x_2^i \ldots x_n^i$ calculated in $S(M)$, whence

$$
\varphi_M(\psi_M(v)) = \sum_{i=1}^p s(x_1^i \otimes x_2^i \otimes \ldots \otimes x_n^i) = s(v) = n!v.
$$

#### Corollary 1 {#alg-iv-s5-prop-12-cor-1 .statement}

— *If $\mathbf{A}$ is a $\mathbf{Q}$-algebra, then the canonical homomorphism of $S(M)$ into $TS(M)$ is an algebra isomorphism. If moreover $M$ is free, then it is an isomorphism of graded bigebras.*

#### Corollary 2 {#alg-iv-s5-prop-12-cor-2 .statement}

— *If $A$ is a $\mathbf{Q}$-algebra then the module $TS^n(M)$ is generated by the n-th powers of elements of $M$ in $TS(M)$.
This follows from Cor. 1 and the corresponding property of $S(M)$* (III, p. 498).

### 9. Homogeneous polynomial mappings

#### Proposition 13 {#alg-iv-s5-prop-13 .statement}

— *Let $M$ and $N$ be $A$-modules, $q$ an integer $\geqslant 0$, and $f$ a mapping of $M$ into $N$. Suppose that $M$ is free, then the following conditions are equivalent:
(i) There exists a $q$-linear mapping $g$ of $M^q$ into $N$ such that $f(x) = g(x, x, \ldots, x)$ for all $x \in M$.
(ii) There exists a linear mapping $h$ of $TS^q(M)$ into $N$ such that $f(x) = h(\gamma_q(x))$ for all $x \in M$.
(iii) There exists a basis $(e_i)_{i \in I}$ of $M$ and a family $(u_v)_{v \in N^{(1)}, |v| = q}$ of elements of $N$ such that
$$
f\left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{v \in N^{(1)}, |v| = q} \lambda^v u_v
$$
for all $(\lambda_i) \in A^{(1)}$.
(iv) For each basis $(e_i)_{i \in I}$ of $M$ there exists a family $(u_v)_{v \in N^{(1)}, |v| = q}$ of elements of $N$ such that
$$
f\left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{v \in N^{(1)}, |v| = q} \lambda^v u_v
$$
for all $(\lambda_i) \in A^{(1)}$.
(i) $\Rightarrow$ (ii): let $g$ satisfy (i), then there exists a linear mapping $g'$ of $T^q(M)$ into $N$ such that $g(x_1, x_2, \ldots, x_q) = g'(x_1 \otimes x_2 \otimes \ldots \otimes x)$ for any $x, \ldots, x, \in M$. Then
$$
f(x) = g(x, x, \ldots, x) = g'(x \otimes x \otimes \ldots \otimes x) = g'(\gamma_q(x));
$$
and on writing $h = g'|TS^q(M)$ we see that condition (ii) holds.
(ii) $\Rightarrow$ (i) and (iv): let $h$ satisfy the conditions of (ii). By Prop. 4, (ii) (IV, p. 47) there exists a linear mapping $g'$ of $T^q(M)$ into $N$ such that $h = g'|TS^q(M)$. Let $g$ be the $q$-linear mapping of $M$ into $N$ associated with $g'$, then for any $x \in M$ we have
$$
f(x) = h(\gamma_q(x)) = g'(x \otimes x \otimes \ldots \otimes x) = g(x, x, \ldots, x),
$$

whence (i). On the other hand, if $(e_i)_{i \in I}$ is a basis of M, we have, by formula (6) (IV, p. 46)

$$
f \left( \sum_i \lambda_i e_i \right) = h \left( \gamma_q \left( \sum_i \lambda_i e_i \right) \right) = h \left( \sum_{|\nu|=q} \lambda^\nu e_\nu \right)
$$

on writing $e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i)$; we thus have

$$
f \left( \sum_i \lambda_i e_i \right) = \sum_{|\nu|=q} \lambda^\nu h(e_\nu).
$$

(iv) $\Rightarrow$ (iii) is clear.
(iii) $\Rightarrow$ (ii) : given $(e_i), (u,)$ satisfying the conditions of (iii), let us write $e_\nu = \prod_{i \in I} \gamma_{\nu_i}(e_i)$ and recall that $(e_\nu)_{|\nu|=q}$ is a basis of $\mathrm{TS}^q(M)$. Let h be the homomorphism of $\mathrm{TS}^q(M)$ into N defined by $h(e_\nu) = u_\nu$; then for each $x = \sum_i \lambda_i e_i$ in M we have

$$
f(x) = f \left( \sum_i \lambda_i e_i \right) = \sum_{|\nu|=q} \lambda^\nu u_\nu = h \left( \sum_{|\nu|=q} \lambda^\nu e_\nu \right) = h(\gamma_q(x))
$$

#### Definition 3 {#alg-iv-s5-def-3 .statement}

— Let M and N be A-modules and q an integer $\geq 0$. Suppose that M is *free*, and denote by $\mathrm{Pol}_A^q(M, N)$ or simply $\mathrm{Pol}^q(M, N)$ the set of mappings of M into N satisfying the conditions of Prop. 13. The elements of $\mathrm{Pol}^q(M, N)$ are called homogeneous polynomial mappings of degree q of M into N.

Prop. 13 (i) defines a homomorphism of A-modules :

$$
\mathcal{L}_q(M, ..., M; N) \to \mathrm{Pol}^q(M, N).
$$

Prop. 13 (ii) defines a homomorphism of A-modules

$$
\mathrm{Hom}_A(\mathbf{TS}^q(M), N) \to \mathrm{Pol}^q(M, N).
$$

These homomorphisms are called canonical. They are surjective.

#### Example 1 {#alg-iv-s5-n9-exa-1 .statement}

The homogeneous polynomial mappings of degree 1 of M into N are the A-linear mappings of M into N.
2) Let $(N_i)_{i \in I}$ be a family of A-modules, $f_i$ a mapping of M into $N_i, i \in I$, and $f : M \to \prod_{i \in I} N_i$ the mapping with components $f_i$. For f to be a homogeneous polynomial mapping of degree q it is necessary and sufficient that each $f_i$ be a homogeneous polynomial mapping of degree q.
3) Let $(M_j)_{j \in J}$ be a finite family of free A-modules and $u : \prod_{j \in J} M_j \to N$ a multilinear mapping ; then u is polynomial of degree $\mathrm{Card}(J)$.

4) Let $(X_i)_{i \in I}$ be a family of indeterminates, $N$ an $A$-module and $u \in N[(X_i)_{i \in I}]$ a homogeneous polynomial of degree $q$. The mapping $(x_i)_{i \in I} \mapsto u((x_i)_{i \in I})$ of $A^{(I)}$ into $N$ is a homogeneous polynomial mapping of degree $q$: this is seen at once by condition (iii) of Prop. 13. If $I$ is finite, every homogeneous polynomial mapping of degree $q$ of $A^{(I)} = A'$ into $N$ is of that form.

5) The mapping $(x_i)_{i \in N} \mapsto x_0^2 + x_1^2 + \ldots + x_n^2 + \ldots$ of $A^{(N)}$ into $A$ is a homogeneous polynomial mapping of degree 2. If $A = 2/22$, it coincides with the linear mapping $(x_i)_{i \in I} \mapsto x_0 + x_1 + \ldots + x_n + \ldots$

6) Let $f \in \mathrm{Pol}_A^q(M, N)$, let $B$ be a commutative ring, $\rho$ a homomorphism of $B$ into $A$ and $M'$ and $N'$ the $B$-modules derived from $M$ and $N$ by means of $\rho$. Assume that $M'$ is free; then $f \in \mathrm{Pol}_B^q(M', N')$: this follows at once from condition (i) of Prop. 13.

#### Proposition 14 {#alg-iv-s5-prop-14 .statement}

— Let $M, N, P$ be $A$-modules, $q$ and $r$ integers $\geqslant 0$, and assume that $M$ and $N$ are free. If $f \in \mathrm{Pol}^q(M, N)$, $f' \in \mathrm{Pol}^r(N, P)$, then $f' \circ f \in \mathrm{Pol}^{qr}(M, P)$.

There exists a $q$-linear mapping $g$ of $M^q$ into $N$ and an $r$-linear mapping $g'$ of $N^r$ into $P$ such that

$$
\begin{aligned}
f(x) &= g(x, x, \ldots, x) & \text{for all } x \in M, \\
f'(y) &= g'(y, y, \ldots, y) & \text{for all } y \in N.
\end{aligned}
$$

Hence for every $x \in M$ we have

$$
f'(f(x)) = g'(f(x), f(x), \ldots, f(x)) = g'(g(x, x, \ldots, x), \ldots, g(x, x, \ldots, x))
$$

and the mapping $(x_1, \ldots, x_{qr}) \mapsto g'(g(x_1, \ldots, x_q), \ldots, g(x_{q(r-1)+1}, \ldots, x_{qr}))$ of $M^{qr}$ into $P$ is $qr$-linear.

#### Proposition 15 {#alg-iv-s5-prop-15 .statement}

— Let $M$ be a free $A$-module, $N$ an $A$-module and $q$ an integer $\geqslant 0$. We suppose that the mapping $y \mapsto q!y$ is an automorphism of $N$. Let $f \in \mathrm{Pol}^q(M, N)$, then there exists one and only one symmetric $q$-linear mapping $h$ of $M^q$ into $M$ such that $f(x) = h(x, x, \ldots, x)$ for all $x \in M$. For any $x_1, \ldots, x_q \in M$ we have

$$
h(x_1, x_2, \ldots, x_q) = \frac{(-1)^q}{q!} \sum_{H \subset \{1, 2, \ldots, q\}} (-1)^{\mathrm{Card}\ H} f\left( \sum_{i \in H} x_i \right).
$$

a) There exists a $q$-linear mapping $g$ of $M^q$ into $N$ such that $f(x) = g(x, x, \ldots, x)$ for all $x \in M$. Let us define a $q$-linear mapping $h$ of $M$ into $N$ by

$$
h(x_1, x_2, \ldots, x_q) = \frac{1}{q!} \sum_{\sigma \in S_q} g(x_{\sigma(1)}, x_{\sigma(2)}, \ldots, x_{\sigma(q)}).
$$

Then $h$ is symmetric and $f(x) = h(x, x, \ldots, x)$ for all $x \in M$.

b) Let $h$ be a symmetric $q$-linear mapping of $M^q$ into $N$ such that f(x) = g(x, x, ..., x). Let l be the linear mapping of T^q(M) into N such that h(x_1, ..., x_q) = l(x_1 \otimes ... \otimes x_q) for any x_1, ..., x_q \in M. We have

$$
(-1)^q q! h(x_1, ..., x_q) = (-1)^q \sum_{\sigma \in S_q} h(x_{\sigma(1)}, ..., x_{\sigma(q)}) =
= (-1)^q l(s(x_1 \otimes ... \otimes x_q)) = \sum_{H \subset \{1, ..., q\}} (-1)^{\text{Card } H} l \left( \gamma_q \left( \sum_{i \in H} x_i \right) \right)
$$

by Prop. 3, (v) (IV, p. 45). Now

$$
l \left( \gamma_q \left( \sum_{i \in H} x_i \right) \right) = h \left( \sum_{i \in H} x_i, ..., \sum_{i \in H} x_i \right) = f \left( \sum_{i \in H} x_i \right)
$$

and this proves formula (16) and the uniqueness of h.

#### Proposition 16 {#alg-iv-s5-prop-16 .statement}

— *Let M be a free A-module, N an A-module, q a positive integer and u the canonical homomorphism of Hom ($\mathbf{TS}^q(M)$, N) into $\mathbf{Pol}^Y(M, N)$.

(i) *If A is an infinite integral domain and N is torsion-free, then u is an isomorphism.*

(ii) *If the mapping $y \mapsto q!y$ in N is injective, u is an isomorphism.*

In the two cases of the proposition we have to prove that u is injective, that is, every linear mapping f of $\mathbf{TS}^q(M)$ into N which is zero on $\gamma_q(M)$, vanishes.

Assume A to be an infinite integral domain and N torsion-free. For every $z \in \mathbf{TS}^q(M)$ there exists $a \in A - \{0\}$ such that $az$ is an A-linear combination of elements of y, (M) (*IV*, p. 47, Prop. 5). Hence $af(z) = f(az) = 0$, and so $f(z) = 0$.

Suppose next that the mapping $y \mapsto q!y$ in N is injective, then by *IV*, p. 45, Prop. 3, (v), f vanishes on s . T^q(M). Hence if $z \in \mathbf{TS}^q(M)$, we have $q!f(z) = f(sz) = 0$, and so $f(z) = 0$.

#### Corollary {#alg-iv-s5-n9-cor-1 .statement}

— *Let M be a free A-module, N an A-module, q a positive integer, $h \in \mathbf{Pol}^q(M, N)$ and $(e_i)_i$, a basis of M. In the two cases of Prop. 16 there exists a unique family $(u,$, $\mathbf{N}^{(1)}, |\cdot|$, , of elements of N such that $h \left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{|\nu| = q} \lambda^\nu u_\nu$ for all $(\lambda_i) \in \mathbf{A}^{(1)}$*

### 10. Polynomial mappings

#### Definition 4 {#alg-iv-s5-def-4 .statement}

— *Let M and N be A-modules and assume that M is free. Let Map(M, N) be the A-module of all mappings of M into N. The submodule $\sum_{q > 0} \mathbf{Pol}_A^q(M, N)$ of Map(M, N) is denoted by $\mathbf{Pol}_A(M, N)$ or simply $\mathbf{Pol}(M, N)$; its elements are called polynomial mappings of M into N.*

Let $(e_i)_{i \in I}$ be a basis of M and suppose that $l$ is finite; by Prop. 13 (IV, p. 54) a mapping $f$ of M into N is polynomial if and only if there exists a polynomial F in the indeterminates $X_i$ with coefficients in N such that

$$
f \left( \sum_{i \in I} x_i e_i \right) = F(x)
$$

for every family $x = (x_i)_{i \in I}$ in $A^{(I)}$. This property is independent of the basis chosen for M and it justifies the terminology « polynomial mapping ».

#### Proposition 17 {#alg-iv-s5-prop-17 .statement}

— *Let M be a free A-module and B an associative, commutative and unital A-algebra. Then $\mathrm{Pol}_A(M, B)$ is a sub-B-algebra of the algebra $\mathrm{Map}(M, B)$.

This follows from Def. 4 and Prop. 13, (iv) (IV, p. 54).

#### Proposition 18 {#alg-iv-s5-prop-18 .statement}

— *Let M, N, P be A-modules, and assume that M and N are free. If $f \in \mathrm{Pol}(M, N)$, $g \in \mathrm{Pol}(N, P)$, then $g \circ f \in \mathrm{Pol}(M, P)$.

We can reduce at once to the case where there exists an integer q such that $g \in \mathrm{Pol}^q(N, P)$; then there exists a q-linear mapping $h$ of $N^q$ into P such that $g(y) = h(y, y, \ldots, y)$ for all $y \in N$. Writing $f$ as a sum of homogeneous polynomial mappings we are thus reduced to proving that the mapping

$$
x \mapsto h(f_1(x), f_2(x), \ldots, f_q(x))
$$

of M into P, where $f_i \in \mathrm{Pol}^{q_i}(M, N)$, is polynomial. For $i = 1, \ldots, q$ there exists a $q_i$-linear mapping $l_i$ of $M^{q_i}$ into N such that $f_i(x) = l_i(x, x, \ldots, x)$ for all $x \in M$. Hence

$$
h(f_1(x), f_2(x), \ldots, f_q(x)) = h(l_1(x, \ldots, x), \ldots, l_q(x, \ldots, x)),
$$

from which our assertion follows.

#### Lemma 2 {#alg-iv-s5-lem-2 .statement}

— *Let N be an A-module, n an integer $\geq 0$ and*

$$
f = m_0 + m_1 X + \cdots + m_n X^n \in N[X].
$$

*Suppose that there exist $\alpha_0, \alpha_1, \ldots, \alpha_r \in A$ such that $f(\alpha_0) = \cdots = f(\alpha_r) = 0$, and such that for $i \neq j$ the homothety of ratio $\alpha_i - \alpha_j$ in N is injective, then $f = 0$.*

(This lemma generalizes the Cor. of IV, p. 16.)

The lemma clearly holds for $n = 0$; we shall prove it by induction on $n$. We have

$$
f(X) = f(X) - f(\alpha_0) = \sum_{i=1}^n m_i (X^i - \alpha_0^i) = (X - \alpha_0) g(X)
$$

where g is an element of N[X] of the form $m_0' + m_1' X + \ldots + m_{n-1}' X^{n-1}$. The hypotheses of the lemma imply that $g(a,) = \cdots = g(a,) = 0$, hence $g = 0$ by the induction hypothesis, and so $f = 0$.

#### Proposition 19 {#alg-iv-s5-prop-19 .statement}

— *Let M be a free A-module, N an A-module, G an infinite additive subgroup of A, and suppose that the homotheties of N defined by the nonzero elements of G are injective. Then Pol(M, N) is the direct sum of the Pol$^q$(M, N).*

Let $f_0, f_1, \ldots, f_n$ be such that $f_i \in \mathrm{Pol}^i(M, N)$ and suppose that we have the relation $f_0 + \ldots + f_n = 0$. Let $x \in M$, then for all $\lambda \in G$ we have
$$
0 = \sum_{i=0}^n f_i(\lambda x) = \sum_{i=0}^n \lambda^i f_i(x).
$$
By Lemma 2, applied to the polynomial $\sum_{i=0}^n f_i(x) X^i$ we have
$$
f_0(x) = \cdots = f_n(x) = 0
$$

#### Corollary {#alg-iv-s5-n10-cor-1 .statement}

— *Assume that A is an infinite integral domain; let M be a free A-module and N a torsion-free A-module.*

(i) *We have $\mathrm{Pol}(M, N) = \bigoplus_{q \geq 0} \mathrm{Pol}^q(M, N)$ and each $\mathrm{Pol}^q(M, N)$ may be identified canonically with $\mathrm{Hom}(\mathbf{T S}^q(M), N)$.*

(ii) *Let $f \in \mathrm{Pol}(M, N)$ and $(e_i)_i$, a basis of M. There exists one and only one family $(u_v)_{v \in N^{(1)}}$ of elements of N such that $f \left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{v \in N^{(1)}} \lambda^v u_v$ for all $(\lambda_i) \in A^{(1)}$.*

The assertion (i) follows from Prop. 16 and 19, and (ii) follows from (i) and the Cor. of Prop. 16.

### 11. Relations between $\mathbf{S}(M^*)$, TS(M)*gr and Pol(M, A)

Let M be a free A-module, we shall equip the graded dual TS(M)*gr with the structure of a commutative, associative and unital graded $^1$ algebra, derived from the graded cogebrad structure of TS(M) (III, p. 580). By III, p. 497 there exists a unique homomorphism of graded A-algebras
$$
\theta : \mathbf{S}(M^*) \to \mathbf{TS}(M)^{*gr}
$$
inducing in degree 1 the identity mapping of M*.

$^1$ A graded homomorphism of degree – k of TS(M) into A is here considered as an element of degree k of TS(M)*gr (II, p. 377).

#### Proposition 20 {#alg-iv-s5-prop-20 .statement}

— *If the A-module M is free and finitely generated, then $0$ is an isomorphism of graded algebras.*

Let $(e_i)_{i \in I}$ be a basis of $M$ and $(e_i^*)_{i \in I}$ the dual basis of $M^*$. For $v \in \mathbf{N}^I$ put

$$
e_v = \prod_{i \in I} \gamma_{v_i}(e_i) \in \mathbf{TS}(M)
$$

By Prop. 4 (*IV*, p. 47) the family $(e_v)_v,_{\mathbf{N}^I}$ is a basis of $TS(M)$; let $(e_v^*)$ be the basis of $\mathbf{TS}(M)^{*gr}$ dual to $(e_v)$. In the light of III, p. 505, Th. 1 it is enough to show that for any $v \in \mathbf{N}^I$ we have

$$
e_v^* = \prod_{i \in I} (e_i^*)^{v_i},
$$

or also that for $\rho, \sigma \in \mathbf{N}^I$ we have $e_\rho^* \cdot e_\sigma^* = e_{\rho + \sigma}^*$; but this last assertion follows from *IV*, p. 50, Formula (12).

#### Remark 1 {#alg-iv-s5-n11-rem-1 .statement}

— In the same way we see that if $M$ is a finitely generated free $A$-module, then the graded algebra $S(M)^{*gr}$ defined in III, p. 593, may be identified with $TS(M^*)$.

#### Proposition 21 {#alg-iv-s5-prop-21 .statement}

— *The canonical homomorphism of A-modules* (*IV*, p. 55)

$$
u : \mathbf{TS}(M)^{*gr} \to \mathrm{Pol}_A(M, A)
$$

*is an algebra homomorphism.*

Let $a \in \mathbf{TS}^q(M)^*, b \in TS^r(M)^*, x \in M$; we have

$$
u(ab)(x) = \langle ab, \gamma_{q+r}(x) \rangle = \langle a \otimes b, c(\gamma_{q+r}(x)) \rangle =
= \langle a \otimes b, \gamma_q(x) \otimes \gamma_r(x) \rangle = \langle a, \gamma_q(x) \rangle \langle b, \gamma_r(x) \rangle = u(a)(x) \cdot u(b)(x),
$$

whence the result.

#### Remark {#alg-iv-s5-n11-rem-2 .statement}

— 2) The composite homomorphism $A, = u \circ 0 : S(M^*) \to \mathrm{Pol}_A(M, A)$ is the unique unital homomorphism of algebras inducing the inclusion of

$$
M^* = \mathrm{Pol}^1(M, A)
$$

in $\mathrm{Pol}(M, A)$. If $M$ is finitely generated free and $A$ is an infinite integral domain, then $\lambda_M$ is bijective (Prop. 20 and Cor. of Prop. 19). In particular if $A$ is an infinite integral domain, then the canonical homomorphism $f \mapsto \tilde{f}$ of $A[X_1, \ldots, X_n]$ into $\mathrm{Pol}(A^n, A)$ (*IV*, p. 4) is an isomorphism.

3) Consider the coproduct $c_S : S(M^*) \to S(M^* \times M^*)$ (III, p. 575, Example 6). For any $v \in S(M^*)$, $x, y \in M$, the polynomial mapping $\lambda_{M \times M}(c_S(v)) : M \times M \to A$ maps $(x, y)$ to $A, (v)(x + y)$. For the two algebra homomorphisms of $S(M^*)$ into $\mathrm{Map}(M \times M, A)$ defined in this way agree on $M^*$, in virtue of the relation

$$
(v \otimes 1 + 1 \otimes v)(x, y) = v(x + y) \quad (v \in M^*)
$$

### Exercises {#alg-iv-s5-exercises}

See the [exercises for § 5](exercises/s5/).
