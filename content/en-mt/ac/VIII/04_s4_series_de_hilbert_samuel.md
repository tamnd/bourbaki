---
book: ac
book_title: Commutative Algebra
chapter: VIII
chapter_title: DIMENSION
section: 4
section_title: Séries de Hilbert-Samuel
lang: en
source: ac-viii-ix-fr
book_pages: AC VIII.87-AC VIII.94
pdf_pages: 0041-0055, 0091-0098
extraction: ocr
subsections:
    - "no": 1
      title: L’anneau $\mathbf{Z}((T))$
      page: 0
      pdf_page: 41
    - "no": 2
      title: Série de Poincaré d’un module gradué sur un anneau de polynômes
      page: 39
      pdf_page: 43
    - "no": 3
      title: Série de Hilbert-Samuel d’un module bien filtré
      page: 43
      pdf_page: 47
    - "no": 4
      title: Degré de la fonction de Hilbert-Samuel
      page: 47
      pdf_page: 51
    - "no": 5
      title: Série de Hilbert-Samuel d’un module quotient
      page: 48
      pdf_page: 52
statements: 34
exercises: 12
content_sha256: 8518b17dacc0f03ac30617ca34c9f6bdc5c164f581fb18cb0106084a763f0d6c
translated_from: content/fr/ac/VIII/04_s4_series_de_hilbert_samuel.md
source_lang: fr
translation_method: machine
source_content_sha256: f91639f7d7cb284f8e82df2e8c5a6d8828ff744149f2b0de169070ff32670b04
translation_model: gpt-5.4
translation_run: translate-en-mt-99f56812
glossary_version: 34
glossary_terms_sha256: bc7f6c9627da133b68a795d28b78cb95d605ecafa5adb064f52bc16d2e3f0a94
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 4. HILBERT-SAMUEL SERIES

### 1. The ring $\mathbf{Z}((T))$

Let A be a ring. Endow the A-module $A^\mathbf{Z}$ with the product topology of the discrete topologies. The elements $(a_n) \in A^\mathbf{Z}$ such that there exists $n_0 \in \mathbf{Z}$ with $a_n = 0$ for $n < n_0$ form a submodule B of $A^\mathbf{Z}$. If for $a = (a_n) \in B, b \in (b_n) \in B$, one sets $ab = c$, with $c_n = \sum_{i+j=n} a_i b_j$, one defines on B a structure of A-algebra. Let T be the element $(\theta_n)$ of B such that $\theta_n = 0$ for $n \neq 1$ and $\theta_1 = 1$. Then T is invertible in B; for every element $a = (a_n)$ of B, the family $(a_n T^n)_{n \in \mathbf{Z}}$ is summable in $A^\mathbf{Z}$ and one has

$$
a = \sum_{n \in \mathbf{Z}} a_n T^n .
$$

In the sequel of this chapter, the A-algebra $B$ will be denoted by $A((T))$; it contains as subalgebras the algebra $A[[T]]$ of formal series and the algebra $A[T, T^{-1}]$; their intersection is the algebra $A[T]$ of polynomials.

#### Remark {#ac-viii-s4-n1-rem-1 .statement}

The ring $A((T))$ is naturally identified with the ring of fractions $A[[T]]_T$ of the ring $A[[T]]$ defined by the multiplicative subset formed by the powers of $T$.

For $n, p$ in $\mathbf{Z}$, the natural number $\left[ \begin{array}{c} n \\ p \end{array} \right]$ is defined by

$$
\left( \begin{array}{ll}
\left[ \begin{array}{c} n \\ p \end{array} \right] = 0 & \text{if } p < 0 \text{ or } p > n, \\
\left[ \begin{array}{c} n \\ p \end{array} \right] = \binom{n}{p} = \frac{n(n-1)...(n-p+1)}{p!} & \text{if } 0 \leq p \leq n .
\end{array} \right.
$$

One has $\left[ \begin{array}{c} n \\ p \end{array} \right] = \left[ \begin{array}{c} n \\ n-p \end{array} \right]$ for $n, p \in \mathbf{Z}$.

#### Lemma 1 {#ac-viii-s4-lem-1 .statement}

*The element $1 - T$ of $\mathbf{Z}((T))$ is invertible. For every integer $r > 0$ one has*

$$
(1 - T)^{-r} = \sum_{n \in \mathbf{Z}} \left[ \begin{array}{c} n + r - 1 \\ r - 1 \end{array} \right] T^n = \sum_{n \in \mathbf{N}} \binom{n + r - 1}{r - 1} T^n .
$$

In fact, $1 - T$ is invertible in the ring $\mathbf{Z}[[T]]$, with inverse $\sum_{m \geq 0} T^m$; one therefore has

$$
(1 - T)^{-r} = (\sum_{m \geq 0} T^m)^r = \sum_{m_1, ..., m_r \geq 0} T^{m_1 + m_2 + ... + m_r},
$$

and the announced formula follows from E, III, p. 44, prop. 15.

Let $Q(T) \in \mathbf{Z}[T, T^{-1}]$, let $r$ be an integer $> 0$, and let $F = (1 - T)^{-r} Q \in \mathbf{Z}((T))$. Put

$$
Q(T) = \sum_{i \in \mathbf{Z}} a_i T^i , \quad F = \sum_{n \in \mathbf{Z}} \alpha_n T^n .
$$

Then, by lemma 1, one has

$$
\alpha_n = \sum_{i \in \mathbf{Z}} a_i \left[ \begin{array}{c} n - i + r - 1 \\ r - 1 \end{array} \right] = \sum_{i \leq n} a_i \binom{n - i + r - 1}{r - 1}.
$$

Let $n_1$ be the least upper bound in $\overline{\mathbf{R}}$ of the set of integers $i \in \mathbf{Z}$ such that $a_i \neq 0$. For every integer $n \geq n_1$, one has $\alpha_n = \tilde{\alpha}(n)$, where $\tilde{\alpha}$ is the polynomial of $\mathbf{Q}[X]$ defined by

$$
\tilde{\alpha}(X) = \frac{1}{(r-1)!} \sum_{i \in \mathbf{Z}} a_i \prod_{j=1}^{r-1} (X - i + j) .
$$

If one sets $c = Q(1) = \sum_{i \in \mathbf{Z}} a_i$, one has $\tilde{\alpha}(X) = c X^{r-1}/(r-1)! + \theta(X)$, where $\theta$ is a polynomial of degree $\leq r-2$. Consequently, one has

$$
\alpha_n = c \frac{n^{r-1}}{(r-1)!} + \rho_n n^{r-2},
$$

where the rational number $\rho_n$ tends to a limit as $n$ increases indefinitely. Hence one deduces the relation

$$
Q(1) = (r-1)! \lim_{n \to \infty} n^{1-r} \alpha_n.
$$

If $F = \sum_{n \in \mathbf{Z}} a_n T^n$ and $G = \sum_{n \in \mathbf{Z}} b_n T^n$ are two elements of $\mathbf{Z}((T))$, one denotes by “ $F \leq G$ ” the relation “ $a_n \leq b_n$ for all $n \in \mathbf{Z}$ ”. This is an order relation compatible with the ring structure of $\mathbf{Z}((T))$ (A, VI, p. 18, Def. 1). One has $(1-T)^{-1} \geq 1$. If $Q \in \mathbf{Z}[T, T^{-1}]$ is $\geq 0$, then the integer $Q(1)$ is positive.

**Lemma 2. — a)** Let $F$ be a nonzero element of $\mathbf{Z}((T))$ such that there exists $r \in \mathbf{Z}$, with $(1-T)^r F \in \mathbf{Z}[T, T^{-1}]$; then $F$ can be written uniquely in the form $F = (1-T)^{-d}.Q$, where $Q \in \mathbf{Z}[T, T^{-1}]$, $Q(1) \neq 0$ and $d \in \mathbf{Z}$. If $F \geq 0$, then one has $Q(1) > 0$ and $d \geq 0$.

b) Let $Q, R$ be in $\mathbf{Z}[T, T^{-1}]$, $d, d'$ in $\mathbf{Z}$ with $Q(1) > 0$. If

$$
(1-T)^{-d}.Q \leq (1-T)^{-d'}.R,
$$

then either $d < d'$, or else $d = d'$ and $Q(1) \leq R(1)$.

a) We may write $F = (1-T)^{-r} T^n P(T)$ with $r, n \in \mathbf{Z}$ and $P(T) \in \mathbf{Z}[T]$. By euclidean division, we may write $P(T) = (1-T)^p R(T)$ with $R(T) \in \mathbf{Z}[T]$ and $R(1) \neq 0$. Hence $F = (1-T)^{-(r-p)} Q(T)$, where $Q(T) = T^n R(T) \in \mathbf{Z}[T, T^{-1}]$ and $Q(1) \neq 0$. This proves the existence of $d$ and $Q$. Moreover, if $(1-T)^r Q(T) = (1-T)^s R(T)$ with $r > s$ and $Q, R$ in $\mathbf{Z}[T, T^{-1}]$, we have $R(T) = (1-T)^{r-s} Q(T)$, hence $R(1) = 0$; this proves the uniqueness. Suppose that $F$ is $\geq 0$; if we had $d < 0$, then we should have $F(1) = 0$, which is impossible since $F$ is nonzero and all its coefficients are positive; thus we have $d \geq 0$. If $d = 0$, then $Q = F \geq 0$, hence $Q(1)$ is positive. If $d \geq 1$, then $Q(1)$ is positive by formula (3). This proves a).

b) Suppose $d \geq d'$. Then $(1-T)^{-d} ((1-T)^{d-d'} R - Q) \geq 0$; since $S(T) = (1-T)^{d-d'} R - Q$ belong to $\mathbf{Z}[T, T^{-1}]$, this implies $S(1) \geq 0$ by what precedes. If $d > d'$, we have $S(1) = -Q(1) < 0$, whence a contradiction; if $d = d'$, we have $S(1) = R(1) - Q(1)$, whence $Q(1) \leq R(1)$.

### 2. Poincaré series of a graded module over a polynomial ring

Let $H_0$ be a ring, $I$ a finite set and $H$ the polynomial ring $H_0[(X_i)_{i \in I}]$. For each $i \in I$, let $d_i$ be an integer $> 0$. Endow $H$ with the structure of a graded ring of type $\mathbf{Z}$ such that the elements of $H_0$ are homogeneous of degree 0 and each $X_i$ homogeneous of degree $d_i$. When $d_i = 1$ for all $i$, we recover the usual grading of polynomial rings.

Let $M$ be a graded $H$-module of *finitely generated* type whose homogeneous components are all $H_0$-modules of finite length; the *Poincaré series* of $M$ is by definition the element $P_M$ of $\mathbf{Z}((T))$ such that $P_M = \sum_{n \in \mathbf{Z}} \operatorname{long}_{H_0}(M_n) \cdot T^n$, and one puts $Q_M = P_M \cdot \prod_{i \in I} (1 - T^{d_i})$.

#### Theorem 1 {#ac-viii-s4-thm-1 .statement}

*The element $Q_M$ of $\mathbf{Z}((T))$ belongs to $\mathbf{Z}[T, T^{-1}]$*.

Dividing $H_0$ by the annihilator of the $H_0$-module $M$, one is reduced to the case where $M$ is a faithful $H_0$-module. If $a, b \in \mathbf{Z}$ are such that $M$ is generated as an $H$-module by $M' = \sum_{a \leq i \leq b} M_i$, then $M'$ is a faithful $H_0$-module of finite length; hence the ring $H_0$ is artinian (A, VIII, § 1, No. 3), therefore noetherian (*loc. cit.*, § 9, No. 1). The polynomial ring $H$ is therefore noetherian (*loc. cit.*, § 1, No. 4). If $I$ is empty, then $H = H_0$, and the family of integers $(\operatorname{long}_{H_0}(M_n))_{n \in \mathbf{Z}}$ has finite support, since $M$ is a finitely generated $H_0$-module; whence the theorem in this case. Let us then argue by induction on the cardinal of the set $I$, assumed nonempty; let $j \in I$ and $J = I - \{j\}$. Let $H'$ denote the graded subring of $H$ generated by $H_0$ and the $X_i$ for $i$ in $J$; consider the homothety $(X_j)_M$ of ratio $X_j$ in $M$, its kernel $R$, and its cokernel $S$. For each $n \in \mathbf{Z}$ there is an exact sequence of $H_0$-modules

$$
0 \to R_{n-d_j} \to M_{n-d_j} \to M_n \to S_n \to 0 ,
$$

therefore $R_{n-d_j}$ and $S_n$ are of finite length, and one has

$$
\operatorname{long}_{H_0}(M_n) - \operatorname{long}_{H_0}(M_{n-d_j}) = \operatorname{long}_{H_0}(S_n) - \operatorname{long}_{H_0}(R_{n-d_j}) .
$$

Since $M$ is a finitely generated module over the noetherian ring $H$, the $H$-modules $R$ and $S$ are finitely generated; since they are annihilated by $X_j$, they are finitely generated $H'$-modules. By the induction hypothesis, the elements $P_R \cdot \prod_{i \in J} (1 - T^{d_i})$ and $P_S \cdot \prod_{i \in J} (1 - T^{d_i})$ of $\mathbf{Z}((T))$ therefore belong to $\mathbf{Z}[T, T^{-1}]$; from (4), one derives

$$
P_M - T^{d_j} \cdot P_M = P_S - T^{d_j} \cdot P_R ,
$$

that is, $(1 - T^{d_j}) \cdot P_M = P_S - T^{d_j} \cdot P_R$; hence

$$
P_M \cdot \prod_{i \in I} (1 - T^{d_i}) = P_S \cdot \prod_{i \in J} (1 - T^{d_i}) - T^{d_j} \cdot P_R \cdot \prod_{i \in J} (1 - T^{d_i}) ,
$$

whence the conclusion.

#### Example 1 {#ac-viii-s4-n2-exa-1 .statement}

Suppose $H_0$ artinian and take $M = H$. Then, with the preceding notations, we have $R = 0$ and $S = H'$, hence by (5), $Q_H = Q_{H'}$; since we have $Q_{H_0} = \operatorname{long}(H_0)$, we infer by induction that $Q_H = \operatorname{long}(H_0)$, that is,

$$
P_H = \operatorname{long}(H_0) \cdot \prod_{i \in I} (1 - T^{d_i})^{-1} .
$$

Now suppose H endowed with the usual grading, for which $d_i = 1$ for all $i \in I$, and put $r = \mathrm{Card}(I)$; we have $P_M = Q_M(T).(1 - T)^{-r}$. Put $c_M = Q_M(1)$. Then, by formula (2) of No. 1, we have:

#### Corollary {#ac-viii-s4-n2-cor-1 .statement}

a) If $r = 0$, then we have $\mathrm{long}_{H_0}(M) = c_M$.

b) If $r = 1$, then we have $\mathrm{long}_{H_0}(M_n) = c_M$ for $n$ sufficiently large.

c) If $r > 1$, then we have $\mathrm{long}_{H_0}(M_n) = c_M \frac{n^{r-1}}{(r-1)!} + \rho_n n^{r-2}$, where $\rho_n$ tends to a limit in $\mathbf{R}$ when $n$ increases indefinitely.

#### Remark 1 {#ac-viii-s4-n2-rem-1 .statement}

The integer $c_M$ is positive by lemma 2. One may have $M \neq 0$ and $c_M = 0$ (cf. prop. 2).

#### Remark 2 {#ac-viii-s4-n2-rem-2 .statement}

Let $0 \to M' \to M \to M'' \to 0$ be an exact sequence of graded H-modules and homomorphisms of degree 0 such that M is of finite type over H and $M_n$ of finite length over $H_0$ for each $n$. Then, for each $n \in \mathbf{Z}$, we have
$$
\mathrm{long}_{H_0}(M_n) = \mathrm{long}_{H_0}(M'_n) + \mathrm{long}_{H_0}(M''_n),
$$
hence $P_M = P_{M'} + P_{M''}$, $Q_M = Q_{M'} + Q_{M''}$ and $c_M = c_{M'} + c_{M''}$.

#### Remark 3 {#ac-viii-s4-n2-rem-3 .statement}

Let $M(p)$ be the module deduced from M by shifting the grading by $p$ (A, II, p. 165, example 3). Since we have $M(p)_n = M_{p+n}$, we have $P_{M(p)} = T^{-p}P_M$, $Q_{M(p)} = T^{-p}Q_M$ and $c_{M(p)} = c_M$.

#### Example 2 {#ac-viii-s4-n2-exa-2 .statement}

Suppose $H_0$ artinian, and let M be a free graded H-module generated by s homogeneous, linearly independent elements, of respective degrees $\delta_1, ..., \delta_s$. Then M is isomorphic to $H(-\delta_1) \oplus \cdots \oplus H(-\delta_s)$. By remarks 2 and 3 and example 1, we therefore have
$$
P_M = \mathrm{long}(H_0)\left( \sum_{i=1}^s T^{\delta_i} \right)(1 - T)^{-r},
$$
$$
Q_M = \mathrm{long}(H_0)\left( \sum_{i=1}^s T^{\delta_i} \right),
$$
$$
c_M = s.\mathrm{long}(H_0).
$$

#### Example 3 {#ac-viii-s4-n2-exa-3 .statement}

Suppose again $H_0$ artinian; let M be a graded H-module, and suppose that there exists an exact sequence of graded H-modules and homomorphisms of degree 0
$$
0 \to L_n \to L_{n-1} \to \cdots \to L_0 \to M \to 0,
$$
where, for $k = 0, 1, ..., n$, $L_k$ is a free graded H-module generated by linearly independent homogeneous elements, of respective degrees $\delta_{k,1}, ..., \delta_{k,m(k)}$. Then, by remark 2 and example 2, we have
$$
Q_M = \mathrm{long}(H_0).\sum_{0 \leq k \leq n} \sum_{1 \leq j \leq m(k)} (-1)^k T^{\delta_{k,j}},
$$
$$
c_M = \mathrm{long}(H_0).\sum_{0 \leq k \leq n} (-1)^k m(k).
$$

#### Remark 4 {#ac-viii-s4-n2-rem-4 .statement}

One can prove (p. 88, exerc. 4) that under the hypotheses of th. 1, the $H_0$-modules $\mathrm{Tor}_j^H(H_0, M)$ are of finite length, are zero for $j > r$, and that one has
$$
c_M = \sum_{j=0}^r (-1)^j \mathrm{long}_{H_0}(\mathrm{Tor}_j^H(H_0, M)).
$$
More precisely, the $H$-modules $T_j = \mathrm{Tor}_j^H(H_0, M)$ are naturally endowed with gradings and one has
$$
Q_M = \sum_{j=0}^r (-1)^j P_{T_j}.
$$

#### Proposition 1 {#ac-viii-s4-prop-1 .statement}

Let $M$ be a graded $H$-module. Suppose that $M$ is generated by $M_0$ and that $M_0$ is an $H_0$-module of finite length. Then one has
$$
P_M \leq (1 - T)^{-r} \mathrm{long}_{H_0}(M_0), \quad c_M \leq \mathrm{long}_{H_0}(M_0).
$$
Moreover, the following conditions are equivalent:
(i) $c_M = \mathrm{long}_{H_0}(M_0)$;
(ii) $P_M = \mathrm{long}_{H_0}(M_0) \cdot (1 - T)^{-r}$, that is to say $M = M_0$ if $r = 0$ and
$$
\mathrm{long}_{H_0}(M_n) = \mathrm{long}_{H_0}(M_0) \binom{n + r - 1}{r - 1}
$$
for $n \in \mathbf{N}$ if $r > 0$;
(iii) the canonical homomorphism of $H$-modules
$$
\varphi : H \otimes_{H_0} M_0 \to M
$$
is bijective.

Let $R$ denote the kernel of $\varphi$. Since $\varphi$ is surjective, one has
$$
P_M = P_{H \otimes M_0} - P_R = \mathrm{long}_{H_0}(M_0) (1 - T)^{-r} - P_R \quad \text{and} \quad c_M = \mathrm{long}_{H_0}(M_0) - c_R.
$$
The conditions (i), (ii) and (iii) are respectively equivalent to $c_R = 0$, $P_R = 0$ and $R = 0$.
Hence one has (iii) $\Rightarrow$ (ii) $\Rightarrow$ (i), and it is enough to prove that $c_R = 0$ implies $R = 0$. Suppose $R \neq 0$ and let $0 = N^h \subset N^{h-1} \subset ... \subset N^0 = M_0$ be a Jordan-Hölder sequence of the $H_0$-module $M_0$. Let $R^m$ be the intersection of $R$ and of the image of $H \otimes_{H_0} N^m$ in $H \otimes_{H_0} M_0$; there exists an integer $m$ between 1 and $h$ such that $R^m \neq R^{m-1}$. Put $L = R^{m-1}/R^m$; one has $0 \leq c_L \leq c_R$ and it is enough to prove that $c_L \neq 0$. Now, if $k$ is the quotient field of $H_0$ by the maximal annihilator ideal of $N^{m-1}/N^m$, $L$ is identified with a nonzero graded submodule of $k[(X_i)_{i \in I}]$. Hence $L$ contains a submodule isomorphic to a shifted module of $k[(X_i)_{i \in I}]$; since $c_{k[(X_i)_{i \in I}]} = 1$, one therefore has $c_L \geq 1$ (Remarks 2 and 3), which was to be proved.

#### Remark 5 {#ac-viii-s4-n2-rem-5 .statement}

According to A, X, p. 160, th. 1, condition (iii) means that $(X_1, ..., X_r)$ is a completely secant sequence for the $H$-module $M$.

#### Proposition 2 {#ac-viii-s4-prop-2 .statement}

Suppose that $H_0$ is a field, and let $M$ be a finitely generated graded $H$-module. Let $K$ be the field of fractions of $H$. Then $c_M$ is equal to the rank of the $H$-module $M$, that is to say to the dimension of the vector space $M \otimes_H K$ over $K$.

This is clear if $M = H$, since $c_H = 1$. On the other hand, let $x \in H$ be homogeneous of degree $d$, and nonzero; one has $(H/xH) \otimes_H K = 0$; from the exact sequence
$$
0 \to H(-d) \to H \to H/xH \to 0,
$$
and remarks 2 and 3, one deduces that $c_{H/xH} = 0$. The proposition is therefore verified when $M$ is generated by a homogeneous element. The general case follows from this, since every finitely generated graded $H$-module has a composition series whose quotients are of the preceding form.

#### Remark 6 {#ac-viii-s4-n2-rem-6 .statement}

Under the hypotheses of Prop. 2, one therefore has $c_M = 0$ if and only if $M$ is a torsion $H$-module, or again if and only if $\dim_H(M) < r$ (\$ 1, No. 5, example 4).

### 3. Hilbert-Samuel Series of a Well-Filtered Module

In the sequel to this paragraph, we shall use the following notation: if $G \in \mathbf{Z}((T))$ and if $r \in \mathbf{N}$, we set $G^{(r)} = (1 - T)^{-r}G$; in particular, if $G = \sum_{n \in \mathbf{Z}} a_n T^n$, then
$$
G^{(1)} = \sum_{n \in \mathbf{Z}} \left( \sum_{i \leq n} a_i \right) T^n.
$$
If $G \geq 0$, one has $G^{(r)} \geq 0$ for every $r \in \mathbf{N}$.

Let $A$ be a noetherian ring, $q$ an ideal of $A$ and $M$ a finitely generated $A$-module. Recall (III, § 3, No. 1, Def. 1) that a $q$-good filtration on $M$ is a mapping $F : n \mapsto F_n$ of $\mathbf{Z}$ into the set of submodules of $M$ satisfying the following three conditions:
a) one has $qF_n \subset F_{n+1} \subset F_n$ for every $n \in \mathbf{Z}$,
b) there exists $n_0 \in \mathbf{Z}$ such that $qF_n = F_{n+1}$ for $n \geq n_0$,
c) there exists $n_1 \in \mathbf{Z}$ such that $F_{n_1} = M$.
If $n_0$ and $n_1$ satisfy the preceding conditions, one has, for every $n \in \mathbf{Z}$,
$$
q^{n-n_1}M \subset F_n \subset q^{n-n_0}M
$$
(recall that we have set $q^r = A$ for $r \leq 0$, by convention).

#### Lemma 3 {#ac-viii-s4-lem-3 .statement}

If $F$ and $F'$ are two $q$-good filtrations on $M$, there exists an integer $m$ such that $F'_n \subset F_{n-m}$ for every $n \in \mathbf{Z}$.
In fact, there exists $n_2$ such that $F'_n \subset q^{n-n_2}M$ for every $n$, hence $F'_n \subset F_{n-(n_2-n_1)}$ for every $n$.

#### Lemma 4 {#ac-viii-s4-lem-4 .statement}

Let $F$ be a $q$-good filtration on $M$. If $M/qM$ is of finite length, $M/F_{n+1}$ and $F_n/F_{n+1}$ are of finite length for every $n \in \mathbf{Z}$.
With the notation of (7), we have $\operatorname{long}(M/F_{n+1}) \leq \operatorname{long}(M/q^{n-n_1+1}M)$ and it is enough to prove that $q^nM/q^{n+1}M$ is of finite length for every $n$. We are thus reduced to the case of the $q$-adic filtration. Let $(x_1, ..., x_r)$ be a finite generating system of the $A$-module $q$, and let $I$ be the finite set of monomials of total degree $n$ in $r$ variables

X_1, ..., X_r. The homomorphism from (M/qM)^l into q^nM/q^{n+1}M which maps the family (u_m)_{m\in I} to the element $\sum m(x_1, ..., x_r)\ u_m$ is surjective. Since M/qM is of finite length, q^nM/q^{n+1}M is so also.

Henceforth suppose M/qM of finite length. Let F be a q-good filtration on M. There exists $n_1 \in \mathbf{Z}$ such that $F_{n_1} = M$, hence $F_n = M$ for $n \leq n_1$; we therefore define an element $H_{M,F}$ of $\mathbf{Z}((T))$ by putting

(8)
$$
H_{M,F} = \sum_{n \in \mathbf{Z}} \operatorname{long}_{A/q}(F_n/F_{n+1}). T^n \in \mathbf{Z}((T)).
$$

#### Definition 1 {#ac-viii-s4-def-1 .statement}

The series $H_{M,F}$ is called the Hilbert-Samuel series of the A-module M (relative to the q-good filtration F).

The mapping $n \mapsto \operatorname{long}_A(F_n/F_{n+1})$ is often called the Hilbert-Samuel function of M (relative to F).

This applies in particular to the case of the q-adic filtration ($F_n = q^nM$); we then put $H_{M,F} = H_{M,q}$. We therefore have

(9)
$$
H_{M,q} = \sum_{n \in \mathbf{Z}} \operatorname{long}_{A/q}(q^nM/q^{n+1}M). T^n .
$$

#### Proposition 3 {#ac-viii-s4-prop-3 .statement}

a) If F is a q-good filtration on M, we have

(10)
$$
H_{M,F}^{(1)} = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(M/F_{n+1}). T^n .
$$

b) If F and F’ are two q-good filtrations on M, there exists an integer m such that $H_{M,F'}^{(1)} \geq T^m H_{M,F}^{(1)}$.

Part a) results immediately from the definition of $H_{M,F}^{(1)}$; part b) results from a) and Lemma 3.

#### Theorem 2 {#ac-viii-s4-thm-2 .statement}

Let A be a noetherian ring, q an ideal of A, M a finitely generated A-module such that M/qM is nonzero and of finite length, and F a q-good filtration on M.

a) There exist an integer d $\geq 0$, and an element R of $\mathbf{Z}[T, T^{-1}]$, uniquely determined, such that $R(1) > 0$ and $H_{M,F} = (1 - T)^{-d}R$.

b) The integers d and R(1) are independent of the q-good filtration F chosen.

a) Let us consider the graded ring gr(A) such that $\operatorname{gr}_n(A) = q^n/q^{n+1}$ and the graded gr(A)-module gr(M) such that $\operatorname{gr}_n(M) = F_n/F_{n+1}$. Since one has $F_{n_1} = M$ and $qF_n = F_{n+1}$ for $n \geq n_0$, gr(M) is generated by $\bigoplus_{n_1 \leq n \leq n_0} \operatorname{gr}_n(M)$, hence is finitely generated. Moreover, if $(x_1, ..., x_r)$ is a finite system of generators of the A-module q, gr(A) is generated by $\operatorname{gr}_0(A)$ and the classes of the $x_i$ modulo $q^2$, hence is isomorphic to a quotient graded ring of $H = (A/q)[X_1, ..., X_r]$. By Theorem 1 of No. 2, one has
$$
(1 - T)^r H_{M,F} \in \mathbf{Z}[T, T^{-1}] .
$$
One has $H_{M,F} \neq 0$ and there therefore exist $d \in \mathbf{N}$ and $R \in \mathbf{Z}[T, T^{-1}]$, uniquely determined, such that $R(1) > 0$ and $H_{M,F} = (1 - T)^{-d}.R$ (Lemma 2 of No. 1).

b) Let $F'$ be another q-good filtration and let us write analogously
$$
H_{M,F'} = (1 - T)^{-d'} R'.
$$
By Proposition 3, b), there exists an integer $m$ such that $(1 - T)^{-d' - 1} R' \geq T^m (1 - T)^{-d - 1} R$.
By Lemma 2, b) of No. 1, this implies $d' \geq d$ and, if $d' = d$, $R'(1) \geq R(1)$.
Exchanging the roles of $F$ and $F'$, one obtains $d = d'$ and $R(1) = R'(1)$.

#### Remark 1 {#ac-viii-s4-n3-rem-1 .statement}

With the notation of a), let us write $R = \sum_{i \in \mathbf{Z}} a_i T^i$, and suppose $d > 0$.
By No. 1, the relation $H_{M,F} = (1 - T)^{-d} R$ may also be written
$$
\text{(11)} \quad \operatorname{long}_A(F_n/F_{n+1}) = \sum_{i \in \mathbf{Z}} a_i \binom{n - i + d - 1}{d - 1} = \sum_{i \leq n} a_i \binom{n - i + d - 1}{d - 1}.
$$
Analogously, since $H^{(1)}_{M,F} = (1 - T)^{-d - 1} R$, one has
$$
\text{(12)} \quad \operatorname{long}_A(M/F_{n+1}) = \sum_{i \in \mathbf{Z}} a_i \binom{n - i + d}{d} = \sum_{i \leq n} a_i \binom{n - i + d}{d}.
$$

Let $A$ be a noetherian ring, $q$ an ideal of $A$, $M$ a finitely generated $A$-module such that $M/qM$ is of finite length. If $M \neq qM$, there exist by Theorem 2, b) integers $d_q(M) \geq 0$ and $e_q(M) > 0$ such that, for every q-good filtration $F$ on $M$, there exists $R \in \mathbf{Z}[T, T^{-1}]$ with
$$
H_{M,F} = (1 - T)^{-d_q(M)} R , \quad R(1) = e_q(M) .
$$
If $M = qM$, one puts by convention $d_q(M) = -\infty$, $e_q(M) = 0$.

#### Remark 2 {#ac-viii-s4-n3-rem-2 .statement}

To say that $M/qM$ is of finite length means that
$$
\operatorname{Supp}(M/qM) = \operatorname{Supp}(M) \cap V(q)
$$
consists of maximal ideals (IV, § 2, No. 5, Proposition 7). We shall see below (No. 4, corollary to Theorem 3) that $d_q(M)$ is the least upper bound of the numbers $\dim_{A_m}(M_m)$, where $m$ runs through the set $\operatorname{Supp}(M) \cap V(q)$.

#### Corollary {#ac-viii-s4-n3-cor-1 .statement}

*Let $A$ be a noetherian ring, $q$ an ideal of $A$, $M$ a finitely generated $A$-module such that $M/qM$ is of finite length, and $F$ a q-good filtration on $M$.
a) In order that one have $d_q(M) \leq 0$, it is necessary and sufficient that the sequence $(q^n M)$ be stationary, or again that the sequence $(F_n)$ be stationary. One then has, for every sufficiently large $n$,
$$
\operatorname{long}(M/F_{n+1}) = \operatorname{long}(M/q^{n+1}M) = e_q(M) .
$$
b) Suppose that one has $d_q(M) > 0$. One then has
$$
\text{(13)} \quad \operatorname{long}_A(F_n/F_{n+1}) = e_q(M) n^{d_q(M) - 1}/(d_q(M) - 1)! + \rho_n n^{d_q(M) - 2},
$$
$$
\text{(14)} \quad \operatorname{long}_A(M/F_{n+1}) = e_q(M) n^{d_q(M)}/d_q(M)! + \sigma_n n^{d_q(M) - 1},
$$
where $\rho_n$ and $\sigma_n$ tend to a limit as $n$ increases indefinitely.
This results at once from Theorem 2 and formula (2) of No. 1.*

#### Remark 3 {#ac-viii-s4-n3-rem-3 .statement}

Suppose q is contained in the radical of A. Then, by Nakayama's lemma, the sequence (q^nM) is stationary if and only if one has q^nM = 0 for n sufficiently large. It then follows from part a) of the corollary that one has d_q(M) \leq 0 if and only if M is of finite length, and that one then has e_q(M) = \operatorname{long}_A(M).

#### Proposition 4 {#ac-viii-s4-prop-4 .statement}

Let A be a noetherian ring, x_1, ..., x_r elements of A, x the ideal which they generate, and M a finitely generated A-module such that M/xM is nonzero and of finite length.
a) One has d_x(M) \leq r.
b) If d_x(M) = r, then e_x(M) \leq \operatorname{long}_A(M/xM).
c) If the sequence (x_1, ..., x_r) is completely secant for M (A, X, p. 157), then d_x(M) = r and e_x(M) = \operatorname{long}_A(M/xM). The converse is true if the x_i belong to the radical of A.

Let H be the polynomial ring (A/x)[X_1, ..., X_r]. Let us endow G = \bigoplus_n x^nM/x^{n+1}M with the structure of a graded H-module for which (X_i)_G is multiplication by the class of x_i modulo x^2. With the notation P_G, Q_G, c_G of No. 2, one has H_{M,x} = P_G, hence (1 - T)^{-d_x(M)}R = (1 - T)^{-r}Q_G, where R(1) = e_x(M) > 0 and Q_G(1) = c_G.

One therefore has either d_x(M) < r and c_G = 0, or d_x(M) = r and c_G = e_x(M). Moreover, by Prop. 1 of No. 2, one has c_G \leq \operatorname{long}(M/xM), and there is equality if and only if the canonical homomorphism A/x[X_1, ..., X_r] \otimes_{A/x} M/xM \to \bigoplus_n x^nM/x^{n+1}M is bijective. This entails the proposition, in view of A, X, p. 160, th. 1.

#### Proposition 5 {#ac-viii-s4-prop-5 .statement}

Let 0 \to M' \to M \to M'' \to 0 be an exact sequence of finitely generated modules over a noetherian ring A, and q an ideal of A.
a) In order that M/qM be of finite length, it is necessary and sufficient that the same be true of M'/qM' and M''/qM''.
b) Suppose M/qM of finite length. Then one is in one of the following three cases:
1) d_q(M) = d_q(M') > d_q(M'') \text{ and } e_q(M) = e_q(M'),
2) d_q(M) = d_q(M'') > d_q(M') \text{ and } e_q(M) = e_q(M''),
3) d_q(M) = d_q(M') = d_q(M'') \text{ and } e_q(M) = e_q(M') + e_q(M'').
a) One has Supp(M) = Supp(M') \cup Supp(M'') and the assertion results from Remark 2.
b) Let us endow M with a q-good filtration F (for example the q-adic filtration), M'' with the quotient filtration F'', and M' with the induced filtration F'. The filtrations F' and F'' are q-good (III, § 3, No. 1, Prop. 1). Then for each n one has an exact sequence of A-modules
$$
0 \to F'_n/F'_{n+1} \to F_n/F_{n+1} \to F''_n/F''_{n+1} \to 0
$$
(III, § 2, No. 4, Prop. 2), so that one has H_{M,F} = H_{M',F'} + H_{M'',F''}, or again
$$
(1 - T)^{-d_q(M)}R = (1 - T)^{-d_q(M')}R' + (1 - T)^{-d_q(M'')}R''
$$
with R, R', R'' \in \mathbf{Z}[T, T^{-1}], R(1) = e_q(M), R'(1) = e_q(M'), R''(1) = e_q(M''). Assertion b) results from this at once.

### 4. Degree of the Hilbert-Samuel function

#### Theorem 3 {#ac-viii-s4-thm-3 .statement}

Let $A$ be a noetherian local ring, $q$ an ideal of $A$ distinct from $A$, and $M$ a finitely generated $A$-module such that $M/qM$ is of finite length. Then the integer $d_q(M)$ is the dimension of the $A$-module $M$ ($\S 1$, No. 4, Def. 8).

One may suppose $M \neq 0$. Let us prove the inequality $d_q(M) \leq \dim_A(M)$. By Cor. 2 to Prop. 9 of $\S 3$, No. 5, there exist $x_1, ..., x_r \in q$, with $r = \dim_A(M)$ and $\operatorname{long}(M / \sum_{i=1}^r x_i M) < +\infty$; let us put $x = \sum_{i=1}^r x_i A$. By Prop. 4 of No. 3, one has $d_x(M) \leq r$; one has $x \subset q$, whence $H^{(1)}_{M,q} \leq H^{(1)}_{M,x}$ and therefore (Lemma 2 of No. 1)

$$
d_q(M) \leq d_x(M) \leq r = \dim_A(M).
$$

Let us now prove, by induction on $\dim_A(M)$, the inequality $\dim_A(M) \leq d_q(M)$, which is obvious when $\dim_A(M) = 0$.

Suppose that $\dim_A(M) > 0$, and that $\dim_A(N) \leq d_q(N)$ for every finitely generated $A$-module $N$ such that $\dim_A(N) < \dim_A(M)$. If $0 = M_0 \subset M_1 \subset ... \subset M_n = M$ is a composition series of $M$, one has $\dim_A(M) = \sup(\dim_A(M_i/M_{i-1}))$ ($\S 1$, No. 4, prop. 9) and $d_q(M) = \sup(d_q(M_i/M_{i-1}))$ (No. 3, prop. 5). By IV, $\S 1$, No. 4, th. 1, one may therefore suppose that $M$ is of the form $A/p$, where $p$ is a prime ideal of $A$, and one has $p \neq m_A$ since $\dim_A(M) > 0$. Let $x \in m_A - p$; the homothety $x_M$ of $M = A/p$ is injective, and one has the exact sequence

$$
0 \longrightarrow M \xrightarrow{x_M} M \longrightarrow M/xM \longrightarrow 0.
$$

By $\S 3$, No. 2, prop. 3, one has $\dim_A(M/xM) = \dim_A(M) - 1$; by prop. 5 of No. 3, and the preceding exact sequence, one has $d_q(M/xM) \leq d_q(M) - 1$. By the induction hypothesis, one therefore has

$$
\dim_A(M) = \dim_A(M/xM) + 1 \leq d_q(M/xM) + 1 \leq d_q(M),
$$

which completes the proof.

#### Corollary {#ac-viii-s4-n4-cor-1 .statement}

Let $A$ be a noetherian ring, $M$ a finitely generated $A$-module and $q$ an ideal of $A$ such that $M/qM$ is of finite length. Then $d_q(M)$ is the least upper bound of the dimensions $\dim_{A_m}(M_m)$, where $m$ ranges over the finite set $S = \operatorname{Supp}(M) \cap V(q)$, and $e_q(M)$ is the sum of the $e_{q_m}(M_m)$ extended to those elements $m$ of $S$ for which one has $\dim_{A_m}(M_m) = d_q(M)$.

For each integer $n$, the length of $M/q^nM$ is the sum of the $\operatorname{long}_{A_m}(M_m/q^n_m M_m)$ (IV, $\S 2$, No. 5, cor. 1 to prop. 7 and corollary to prop. 8). Consequently, one has $H_{M,q} = \sum_{m \in S} H_{M_m,q_m}$, whence the corollary.

#### Remark 1 {#ac-viii-s4-n4-rem-1 .statement}

One also has $d_q(M) = \sup_{m \in V(q)} \dim(M_m)$, that is, $d_q(M) = \dim(\hat{M})$, where $\hat{M}$ is the completion of $M$ for the q-adic topology ($\S 3$, No. 4, prop. 8).

#### Remark 2 {#ac-viii-s4-n4-rem-2 .statement}

Suppose q contained in the radical of A; then $\dim(\hat{M}) = \dim(M)$ (*loc. cit.*, cor. 1), hence $d(M) = \dim(M)$.

### 5. Hilbert-Samuel series of a quotient module

#### Lemma 5 {#ac-viii-s4-lem-5 .statement}

Let A be a ring, M an A-module and $(P_n), (Q_n)$ two decreasing filtrations on M consisting of submodules. Suppose that one has $P_n \supset Q_n$ and $\operatorname{long}_A(P_n/Q_n) < +\infty$ for every $n \in \mathbf{Z}$ and that there exists an integer $n_1$ such that $Q_{n_1} = M$. In $\mathbf{Z}((T))$, one has the inequalities

$$
\sum_{n \in \mathbf{Z}} \operatorname{long}_A((P_{n+1} \cap Q_n)/Q_{n+1}).T^n \leq \sum_{n \in \mathbf{Z}} \operatorname{long}_A(P_{n+1}/Q_{n+1}).T^n \leq
$$
$$
\leq (1-T)^{-1} \sum_{n \in \mathbf{Z}} \operatorname{long}_A((P_{n+1} \cap Q_n)/Q_{n+1}).T^n .
$$

It is a matter of proving that one has the inequalities

(15) $\operatorname{long}((P_{n+1} \cap Q_n)/Q_{n+1}) \leq \operatorname{long}(P_{n+1}/Q_{n+1})$,
(16) $\operatorname{long}(P_{n+1}/Q_{n+1}) \leq \sum_{i \leq n} \operatorname{long}((P_{i+1} \cap Q_i)/Q_{i+1})$.

The first is obvious. On the other hand, one has $P_{n+1} \cap Q_i = P_{n+1}$ for $i \leq n_1$ and $P_{n+1} \cap Q_{n+1} = Q_{n+1}$; whence one deduces the inequality
$$
\operatorname{long}(P_{n+1}/Q_{n+1}) \leq \sum_{i \leq n} \operatorname{long}((P_{n+1} \cap Q_i)/(P_{n+1} \cap Q_{i+1})) .
$$

But the A-module $(P_{n+1} \cap Q_i)/(P_{n+1} \cap Q_{i+1})$ is isomorphic to a submodule of $(P_{i+1} \cap Q_i)/Q_{i+1}$, and inequality (16) follows.

#### Lemma 6 {#ac-viii-s4-lem-6 .statement}

Let A be a ring, M an A-module and $(F_n)$ a decreasing filtration on M consisting of submodules; suppose that there exists an integer $n_1$ such that $F_{n_1} = M$. Let f be an endomorphism of M, $M'$ its kernel and $M''$ its cokernel. We equip $M'$ with the filtration $(F'_n)$ induced by $(F_n)$ and $M''$ with the quotient filtration $(F''_n)$ of $(F_n)$. Suppose that $F_n/F_{n+1}$ is of finite length for every $n \in \mathbf{Z}$ and that there exists an integer $\delta$ such that $f(F_n) \subset F_{n+\delta}$. Let $\varphi$ be the graded endomorphism of degree $\delta$ of the graded module $\mathrm{gr}(M) = \bigoplus_{n \in \mathbf{Z}} F_n/F_{n+1}$ deduced from f. Between the following elements of $\mathbf{Z}((T))$

$$
H_M = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(F_n/F_{n+1}).T^n
$$
$$
H_{M'} = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(F'_n/F'_{n+1}).T^n
$$
$$
H_{M''} = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(F''_n/F''_{n+1}).T^n
$$
$$
P_{\mathrm{Ker}(\varphi)} = \sum_{n \in \mathbf{Z}} \operatorname{long}_A(\mathrm{Ker}(\varphi_n)).T^n ,
$$

one has the inequalities

(17) $H_{M'} \leq P_{\mathrm{Ker}(\varphi)}$

(18) $(1 - T^\delta).H_M^{(1)} + T^\delta.P_{\mathrm{Ker}(\varphi)} \leq H_{M''}^{(1)} \leq (1 - T^\delta).H_M^{(1)} + T^\delta.P_{\mathrm{Ker}(\varphi)}^{(1)}$.

The sequence of submodules $G_n = f^{-1}(F_{n+\delta})$ of $M$ is a decreasing filtration, and one has $F_n \subset G_n$ for every integer $n$.
By definition, one has $\mathrm{Ker}(\varphi_n) = (G_{n+1} \cap F_n)/F_{n+1}$, whence

(19) $P_{\mathrm{Ker}(\varphi)} = \sum_{n \in \mathbf{Z}} \mathrm{long}_A((G_{n+1} \cap F_n)/F_{n+1}).T^n$.

For every $n$, the A-module $(M' \cap F_n)/(M' \cap F_{n+1})$ identifies with a submodule of $(G_{n+1} \cap F_n)/F_{n+1}$, and inequality (17) follows at once from (19). By lemma 5, one has moreover

(20) $P_{\mathrm{Ker}(\varphi)} \leq \sum_{n \in \mathbf{Z}} \mathrm{long}_A(G_{n+1}/F_{n+1}).T^n \leq P_{\mathrm{Ker}(\varphi)}^{(1)}$.

For every $n \in \mathbf{Z}$, one has an exact sequence of A-modules

$$ 0 \longrightarrow G_{n+1}/F_{n+1} \longrightarrow M/F_{n+1} \xrightarrow{f_n} M/F_{n+\delta+1} \longrightarrow M''/F''_{n+\delta+1} \longrightarrow 0, $$

where $f_n$ is deduced from $f$ by passing to quotients. Consequently one has

$\mathrm{long}_A(M''/F''_{n+\delta+1}) = \mathrm{long}_A(M/F_{n+\delta+1}) - \mathrm{long}_A(M/F_{n+1}) + \mathrm{long}_A(G_{n+1}/F_{n+1})$.

Multiplying by $T^{n+\delta}$ and summing over $n$, one obtains

(21) $H_{M''}^{(1)} = (1 - T^\delta)H_M^{(1)} + T^\delta.\sum_{n \in \mathbf{Z}} \mathrm{long}_A(G_{n+1}/F_{n+1}).T^n,$

and inequality (18) follows at once from (20) and (21).

#### Lemma 7 {#ac-viii-s4-lem-7 .statement}

Retain the notation of lemma 6.

a) One has the inequality $H_{M''}^{(1)} \geq \frac{1 - T^\delta}{1 - T} H_M$.

b) In order that one have equality, it is necessary and sufficient that $\varphi$ be injective.

c) If this is so, one has $M' \subset \bigcap_n F_n$, and the exact sequence of A-modules

$$ 0 \longrightarrow \mathrm{gr}(M) \xrightarrow{\varphi} \mathrm{gr}(M) \xrightarrow{v} \mathrm{gr}(M'') \longrightarrow 0, $$

where $v$ is the canonical mapping, is exact.

Assertions a) and b) follow from formula (18) of lemma 6, and from the definition $H_M^{(1)} = (1 - T)^{-1}.H_M$.

Suppose that $\varphi$ is injective. By III, § 2, no 8, th. 1, (i), one has

$$ \mathrm{Ker}(f) \subset f^{-1}(F_{n+\delta}) = F_n $$

for all $n$, whence the first assertion of c). Moreover there is an exact sequence

$$
0 \longrightarrow M/M' \xrightarrow{f'} M \longrightarrow M/f(M) \longrightarrow 0,
$$

where $f'$ is deduced from $f$ by passing to the quotient. If $\varphi$ is injective, one has as above $f'^{-1}(F_n) = F_{n-\delta}/M'$. It follows that the filtration on $M/M'$ deduced as inverse image by $f'$ of the filtration $F$ on $M$ is the filtration $n \mapsto F_{n-\delta}/M'$; the associated graded is $\mathrm{gr}(M)(-\delta)$ and there is an exact sequence of graded modules (III, § 2, no. 4, prop. 2)

$$
0 \longrightarrow \mathrm{gr}(M)(-\delta) \xrightarrow{\varphi'} \mathrm{gr}(M) \longrightarrow \mathrm{gr}(M'') \longrightarrow 0,
$$

where $\varphi'_n = \varphi_{n-\delta}$ for all $n$. This completes the proof of c).

#### Proposition 6 {#ac-viii-s4-prop-6 .statement}

*Let A be a noetherian ring, M a finitely generated A-module and q an ideal of A such that M/qM is of finite length. Let F be a q-good filtration of M, and let $\mathrm{gr}(A) = \bigoplus_{n \geq 0} (q^n/q^{n+1})$ be the graded ring associated with A for the q-adic filtration.*

*Let $(x_1, ..., x_s)$ be a sequence of elements of A, $(\delta_1, ..., \delta_s)$ a sequence of strictly positive integers such that $x_i \in q^{\delta_i}$ for $1 \leq i \leq s$, and let $\xi_i$ be the class of $x_i$ in $\mathrm{gr}_{\delta_i}(A) = q^{\delta_i}/q^{\delta_i+1}$.*

a) Endow the A-module $\overline{M} = M/(x_1M + \cdots + x_sM)$ with the q-good filtration $\overline{F}$ quotient of F. Then one has in $\mathbf{Z}((T))$ the inequality

$$
H_{\overline{M}, \overline{F}}^{(s)} \geq \left( \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T} \right) \cdot H_{M, F}.
$$

b) *For there to be equality in (22), it is necessary and sufficient that the sequence $(\xi_1, ..., \xi_s)$ of elements of the ring $\mathrm{gr}(A)$ be completely secant for the module $\mathrm{gr}(M) = \bigoplus_{n} (F_n/F_{n+1})$.*

*In that case, the canonical homomorphism of $\mathrm{gr}(M)/\sum_{i=1}^s \xi_i \cdot \mathrm{gr}(M)$ into $\mathrm{gr}(\overline{M}) = \bigoplus (\overline{F}_n/\overline{F}_{n+1})$ is an isomorphism.*

c) *Assume the conditions of b) satisfied, and that each of the A-modules $M_i = M/(x_1M + \cdots + x_iM)$ ($0 \leq i < s$) is separated for the q-adic topology¹. Then the sequence $(x_1, ..., x_s)$ is completely secant for the A-module M.*

When $s = 1$, one has $\bigcap_n F_n = \bigcap_n q^nM$ and the sequence $\{ \xi_1 \}$ is completely secant for $\mathrm{gr}(M)$ if and only if the homothety of ratio $\xi_1$ in $\mathrm{gr}(M)$ is injective. Prop. 6 then follows at once from lemma 7 applied to the homothety $f = (x_1)_M$ in M.

Assume that one has $s \geq 2$ and argue by induction on s. The induction hypothesis applied to the A-module $M_1 = M/x_1M$ endowed with the filtration G quotient of F, and to the sequence $(x_2, ..., x_s)$ yields the inequality

$$
H_{M_1, G}^{(s-1)} \geq \left( \prod_{i=2}^s \frac{1 - T^{\delta_i}}{1 - T} \right) \cdot H_{M_1, G};
$$

¹ This occurs in particular if q is contained in the radical of A (III, § 3, no. 3, prop. 6).

there is equality if and only if the sequence $(\xi_2, ..., \xi_s)$ is completely secant for the gr(A)-module $gr(M_1) = \bigoplus_n G_n/G_{n+1}$. Since the elements $\frac{1 - T^{\delta_i}}{1 - T}$ of $\mathbf{Z}((T))$ are positive, the case $s = 1$ already treated and formula (23) yield the inequalities

$$
H^{(s)}_{M,F} \geq \left( \prod_{i=2}^s \frac{1 - T^{\delta_i}}{1 - T} \right) \cdot H^{(1)}_{M_1,G} \geq \left( \prod_{i=1}^s \frac{1 - T^{\delta_i}}{1 - T} \right) \cdot H_{M,F}.
$$

This proves *a*).

There can be equality in (22) only if one has simultaneously equality in (23) and the equality

$$
H^{(1)}_{M_1,G} = \left( \frac{1 - T^{\delta_1}}{1 - T} \right) \cdot H_{M,F}.
$$

This last relation signifies that $\{\xi_1\}$ is completely secant for gr(M) and implies that the canonical homomorphism of gr(M)/$\xi_1\cdot$gr(M) into gr(M_1) is an isomorphism. In other words, one has equality in (22) if and only if $\{\xi_1\}$ is completely secant for gr(M) and $\{\xi_2, ..., \xi_s\}$ completely secant for gr(M)/$\xi_1\cdot$gr(M). This signifies that $\{\xi_1, ..., \xi_s\}$ is completely secant for gr(M) (A, X, p. 160, Corollary 2). Thus the equivalence of the two conditions of *b*) has been proved. Suppose them satisfied; then, by the induction hypothesis, gr(M) is identified with $gr(M_1)/\sum_{i=2}^s \xi_i \cdot gr(M_1)$; since moreover gr(M_1) is identified with gr(M)/$\xi_1\cdot$gr(M), the last assertion of *b*) is therefore satisfied.

Now suppose that $\{\xi_1, ..., \xi_s\}$ is completely secant for gr(M) and M_i separated for the q-adic topology (for $0 \leq i < s$). From the preceding and the induction hypothesis, the sequence $(x_2, ..., x_s)$ is completely secant for M_1; since one has $M_1 = M/x_1M$ and $\{x_1\}$ is completely secant for M, the sequence $(x_1, x_2, ..., x_s)$ is completely secant for M (A, X, p. 160, Theorem 1).

## EXERCISES {#ac-viii-s4-exercises}

See the [exercises for § 4](exercises/s4/).
