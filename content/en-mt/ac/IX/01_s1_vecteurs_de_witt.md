---
book: ac
book_title: Commutative Algebra
chapter: IX
chapter_title: ANNEAUX LOCAUX NOETHÉRIENS COMPLETS
section: 1
section_title: Vecteurs de Witt
lang: en
source: ac-viii-ix-fr
book_pages: AC IX.42-AC IX.68
pdf_pages: 0113-0129, 0154-0180
extraction: ocr
subsections:
    - "no": 1
      title: Polynômes de Witt
      page: 0
      pdf_page: 113
    - "no": 2
      title: Les applications $f, v$ et $\Phi$
      page: 2
      pdf_page: 114
    - "no": 3
      title: Construction de polynômes
      page: 4
      pdf_page: 116
    - "no": 4
      title: L’anneau W(A) des vecteurs de Witt
      page: 6
      pdf_page: 118
    - "no": 5
      title: L’homomorphisme F et le décalage V
      page: 7
      pdf_page: 119
    - "no": 6
      title: Filtration et topologie de l’anneau W(A)
      page: 10
      pdf_page: 122
    - "no": 7
      title: Les anneaux $W_n(A)$ des vecteurs de Witt de longueur finie
      page: 12
      pdf_page: 124
    - "no": 8
      title: L’anneau des vecteurs de Witt à coefficients dans un anneau de caractéristique $p$
      page: 15
      pdf_page: 127
statements: 29
exercises: 58
content_sha256: 2e225aff9d336098123f6a04b553bca80ecbfede3d28c21e9ac1e09a70727f39
translated_from: content/fr/ac/IX/01_s1_vecteurs_de_witt.md
source_lang: fr
translation_method: machine
source_content_sha256: 1bf90a4c3564b98f34f18ff8237f5d8a6d0deeaca092b966e89f64752a810f7a
translation_model: gpt-5-6-mini, gpt-5-mini
translation_run: translate-en-mt-115f0bd4
glossary_version: 34
glossary_terms_sha256: 2856076244bcc45587bb8540816bd2a9d9e659a8b7f0f899c0504a2a3b0b8903
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. WITT VECTORS

Throughout this paragraph, $p$ denotes a prime number.

### 1. Witt polynomials

For every integer $n \geqslant 0$, one calls the $n$-th Witt polynomial the element $\Phi_n$ of $\mathbf{Z}[X_0, ..., X_n]$ defined by

$$
\Phi_n(X_0, ..., X_n) = \sum_{i=0}^n p^i X_i^{p^{n-i}} = X_0^{p^n} + p X_1^{p^{n-1}} + \cdots + p^n X_n .
$$

One has obviously $\Phi_0 = X_0$ and the recurrence relations

$$
\Phi_{n+1}(X_0, ..., X_{n+1}) = \Phi_n(X_0^p, ..., X_n^p) + p^{n+1} X_{n+1}
$$
$$
\Phi_{n+1}(X_0, ..., X_{n+1}) = X_0^{p^{n+1}} + p \Phi_n(X_1, ..., X_{n+1}) .
$$

When one assigns to $X_i$ the weight $p^i$, the polynomial $\Phi_n$ is isobaric of weight $p^n$ (A, IV, p. 3).

#### Proposition 1 {#ac-ix-s1-prop-1 .statement}

Let A be a filtered ring and $(\mathbf{J}_n)_{n \in \mathbf{Z}}$ its filtration. Assume that one has $\mathbf{J}_0 = \mathbf{A}$ and $p.1_A \in \mathbf{J}_1$. Let m and n be integers such that $m \geqslant 1$ and $n \geqslant 0$, and let $a_0, ..., a_n, b_0, ..., b_n$ be elements of A.

a) If one has $a_i \equiv b_i \mod \mathbf{J}_m$ for $0 \leqslant i \leqslant n$, then one has
$$
\Phi_i(a_0, ..., a_i) \equiv \Phi_i(b_0, ..., b_i) \mod \mathbf{J}_{m+i} \quad \text{for } 0 \leqslant i \leqslant n .
$$

b) Suppose that, for every integer $k \geqslant 1$, and every $x \in \mathbf{A}$, the relation $p.x \in \mathbf{J}_{k+1}$ entails $x \in \mathbf{J}_k$. If one has $\Phi_i(a_0, ..., a_i) \equiv \Phi_i(b_0, ..., b_i) \mod \mathbf{J}_{m+i}$ for $0 \leqslant i \leqslant n$, then one has $a_i \equiv b_i \mod \mathbf{J}_m$ for $0 \leqslant i \leqslant n$.

#### Lemma 1 {#ac-ix-s1-lem-1 .statement}

If x and y are two elements of A congruent modulo $\mathbf{J}_m$, one has
$$
x^{p^n} \equiv y^{p^n} \mod \mathbf{J}_{m+n} .
$$
By induction on n, one reduces to the case where $n = 1$. Let P denote the polynomial $\sum_{i=0}^{p-1} X^i Y^{p-1-i}$ of $\mathbf{Z}[X, Y]$. In view of the assumption made on x and y, one has $P(x, y) \equiv P(x, x) \equiv p.x^{p-1} \mod \mathbf{J}_m$. Now one has $\mathbf{J}_m + p.\mathbf{A} \subset \mathbf{J}_1$, whence $P(x, y) \in \mathbf{J}_1$. Finally, $x^p - y^p = (x - y) P(x, y)$ belongs to $\mathbf{J}_m \mathbf{J}_1 \subset \mathbf{J}_{m+1}$.

Let us prove a) by induction on n. The case $n = 0$ is immediate. Suppose $n \geqslant 1$. Under the hypotheses of a), one has
(4) $a_i^p \equiv b_i^p \mod \mathbf{J}_{m+1}$ for $0 \leqslant i \leqslant n-1$ according to Lemma 1 ,
(5) $\Phi_{n-1}(a_0^p, ..., a_{n-1}^p) \equiv \Phi_{n-1}(b_0^p, ..., b_{n-1}^p) \mod \mathbf{J}_{m+n}$
according to the induction hypothesis applied to the elements $a_0^p, ..., a_{n-1}^p, b_0^p, ..., b_{n-1}^p$ of A, and
(6) $\Phi_n(a_0, ..., a_n) - p^n.a_n \equiv \Phi_n(b_0, ..., b_n) - p^n.b_n \mod \mathbf{J}_{m+n}$
according to formulas (2) and (5). Since $a_n - b_n$ belongs to $\mathbf{J}_m$, the element $p^n.a_n - p^n.b_n$ belongs to $\mathbf{J}_{m+n}$ and one deduces from (6) the congruence
$$
\Phi_n(a_0, ..., a_n) \equiv \Phi_n(b_0, ..., b_n) \mod \mathbf{J}_{m+n} ,
$$
whence a).

Let us prove b) by induction on n. The case $n = 0$ is immediate. Suppose $n \geqslant 1$. Under the assumptions of b), we have $a_i \equiv b_i \mod \mathbf{J}_m$ for $0 \leqslant i \leqslant n-1$ by the induction hypothesis, and we deduce from this, as previously, the congruences (4), (5) and (6). But by assumption $\Phi_n(a_0, ..., a_n)$ and $\Phi_n(b_0, ..., b_n)$ are congruent mod. $\mathbf{J}_{m+n}$, and hence we have $p^n.(a_n - b_n) \in \mathbf{J}_{m+n}$. Since the relation $p.x \in \mathbf{J}_{k+1}$ implies $x \in \mathbf{J}_k$ for every $x \in \mathbf{A}$ and every $k \geqslant 1$, we have $a_n - b_n \in \mathbf{J}_m$, which completes the proof.

### 2. The mappings $f, v$ and $\Phi$

Let A be a ring. Endow $\mathbf{A}^\mathbf{N}$ with the product ring structure. Denote by $f_A$, or simply by $f$, the endomorphism $(a_n)_{n \in \mathbf{N}} \mapsto (a_{n+1})_{n \in \mathbf{N}}$ of $\mathbf{A}^\mathbf{N}$. Denote by $v_A$, or simply by $v$, the endomorphism of the additive group underlying $\mathbf{A}^{\mathbf{N}}$ which associates $(0, p \cdot a_0, p \cdot a_1, ...)$ with $(a_n)_{n \in \mathbf{N}}$.

For every integer $m \geqslant 0$, denote by $\Phi_m$ the mapping from $\mathbf{A}^{\mathbf{N}}$ into $\mathbf{A}$ which associates $\Phi_m(a_0, ..., a_m)$ with $a = (a_n)_{n \in \mathbf{N}}$. We denote by $\Phi_A$, or simply by $\Phi$, the mapping $a \mapsto (\Phi_n(a))_{n \in \mathbf{N}}$ from $\mathbf{A}^{\mathbf{N}}$ into itself.

#### Lemma 2 {#ac-ix-s1-lem-2 .statement}

Let $\mathbf{A}$ be a ring endowed with an endomorphism $\sigma$ satisfying $\sigma(a) \equiv a^p \mod. p \cdot \mathbf{A}$ for every $a \in \mathbf{A}$. Let $n \geqslant 1$ be an integer and let $a_0, ..., a_{n-1}$ be elements of $\mathbf{A}$. Put $u_i = \Phi_i(a_0, ..., a_i)$ for $0 \leqslant i \leqslant n - 1$. Let $u_n$ be an element of $\mathbf{A}$. The following conditions are equivalent:

a) There exists $a_n \in \mathbf{A}$ such that $u_n = \Phi_n(a_0, ..., a_n)$.

b) One has $\sigma(u_{n-1}) \equiv u_n \mod. p^n \cdot \mathbf{A}$.

For $0 \leqslant i \leqslant n - 1$, one has $\sigma(a_i) \equiv a_i^p \mod. p \cdot \mathbf{A}$. According to prop. 1 of no. 1 applied to the case where $J_k = p^k \cdot \mathbf{A}$ (for $k \in \mathbf{N}$) and where $m = 1$, one has the congruence

$$
\Phi_{n-1}(\sigma(a_0), ..., \sigma(a_{n-1})) \equiv \Phi_{n-1}(a_0^p, ..., a_{n-1}^p) \mod. p^n \cdot \mathbf{A},
$$

that is to say

$$
\sigma(u_{n-1}) \equiv \Phi_{n-1}(a_0^p, ..., a_{n-1}^p) \mod. p^n \cdot \mathbf{A}.
$$

Now, according to formula (2), the relation $u_n = \Phi_n(a_0, ..., a_n)$ is equivalent to

$$
u_n = \Phi_{n-1}(a_0^p, ..., a_{n-1}^p) + p^n \cdot a_n.
$$

The lemma follows.

#### Proposition 2 {#ac-ix-s1-prop-2 .statement}

Let $\mathbf{A}$ be a ring.

(a) If $p \cdot 1_A$ is not a divisor of 0 in $\mathbf{A}$, the mapping $\Phi_A$ is injective.

(b) If $p \cdot 1_A$ is invertible in $\mathbf{A}$, the mapping $\Phi_A$ is bijective.

(c) If $\sigma$ is an endomorphism of the ring $\mathbf{A}$, satisfying $\sigma(a) \equiv a^p \mod. p \cdot \mathbf{A}$ for every $a \in \mathbf{A}$, the image $\mathbf{A}'$ of $\Phi_A$ is a subring of $\mathbf{A}^{\mathbf{N}}$, stable under $f_A$ and $v_A$. It is the set of elements $(u_n)_{n \in \mathbf{N}}$ of $\mathbf{A}^{\mathbf{N}}$ such that $\sigma(u_n) \equiv u_{n+1} \mod. p^{n+1} \cdot \mathbf{A}$ for every $n \in \mathbf{N}$.

If $a = (a_n)_{n \in \mathbf{N}}$ and $u = (u_n)_{n \in \mathbf{N}}$ are elements of $\mathbf{A}^{\mathbf{N}}$, the relation $\Phi_A(a) = u$ is equivalent, according to formula (2), to the equalities

$$
\begin{cases}
u_0 = a_0, \\
u_n = \Phi_{n-1}(a_0^p, ..., a_{n-1}^p) + p^n \cdot a_n & \text{for all } n \geqslant 1.
\end{cases}
$$

Let $u = (u_n)_{n \in \mathbf{N}}$ be in $\mathbf{A}^{\mathbf{N}}$. When $p \cdot 1_A$ is not a divisor of 0 in $\mathbf{A}$ (resp. when $p \cdot 1_A$ is invertible in $\mathbf{A}$), there exists at most one sequence $(a_n)_{n \in \mathbf{N}}$ in $\mathbf{A}$ (resp. exactly one sequence $(a_n)_{n \in \mathbf{N}}$ in $\mathbf{A}$) satisfying the equalities (10), whence $a)$ and $b)$.

Let us prove $c)$. According to Lemma 2, the image $\mathbf{A}'$ of $\mathbf{A}^{\mathbf{N}}$ by $\Phi_A$ is the set of $u = (u_n)_{n \in \mathbf{N}}$ in $\mathbf{A}^{\mathbf{N}}$ such that $\sigma(u_n) \equiv u_{n+1} \mod. p^{n+1} \cdot \mathbf{A}$ for every $n \in \mathbf{N}$. It follows immediately that $\mathbf{A}'$ is a subring of $\mathbf{A}^{\mathbf{N}}$, stable under $f_A$ and $v_A$.

#### Remark {#ac-ix-s1-n2-rem-1 .statement}

Let $a = (a_n)_{n \in \mathbf{N}}$ and $u = (u_n)_{n \in \mathbf{N}}$ be elements of $A^\mathbf{N}$ such that $u = \Phi_A(a)$, and let $m$ be an integer $\geqslant 0$. From (10) one deduces the following assertions:

If the $u_n$, for $0 \leqslant n \leqslant m$, belong to a subring $B$ of $A$ and if, for every $x \in A$, the relation $p.x \in B$ implies $x \in B$, then the $a_n$, for $0 \leqslant n \leqslant m$, belong to $B$.

If $A$ is endowed with a graduation of type $\mathbf{N}$, if $p.1_A$ is not a divisor of 0 in $A$, if $d \in \mathbf{N}$ and if $u_n$ is homogeneous of degree $dp^n$ for $0 \leqslant n \leqslant m$, then $a_n$ is homogeneous of degree $dp^n$ for $0 \leqslant n \leqslant m$.

### 3. Construction of polynomials

Let $A$ be the ring $\mathbf{Z}[X, Y]$ of polynomials with integer coefficients in two families of indeterminates $X = (X_n)_{n \in \mathbf{N}}$ and $Y = (Y_n)_{n \in \mathbf{N}}$. Let $\theta$ be the endomorphism of $A$ defined by $\theta(X_n) = X_n^p$ and $\theta(Y_n) = Y_n^p$ for all $n \in \mathbf{N}$. Then $p$ is not a divisor of 0 in $A$ and the set of the $a$ in $A$ such that $\theta(a) \equiv a^p \mod. p.A$ is a subring of $A$ containing the $X_n$ and the $Y_n$, hence equal to $A$ itself.

By the prop. 2, $a)$ and $c)$ of no 2, there exist elements $S = (S_n)_{n \in \mathbf{N}}, P = (P_n)_{n \in \mathbf{N}}, I = (I_n)_{n \in \mathbf{N}}$ and $F = (F_n)_{n \in \mathbf{N}}$ of $A^\mathbf{N}$ characterized respectively by the equalities

$$
\left\{
\begin{array}{l}
\Phi_A(S) = \Phi_A(X) + \Phi_A(Y) \\
\Phi_A(P) = \Phi_A(X) \Phi_A(Y) \\
\Phi_A(I) = - \Phi_A(X) \\
\Phi_A(F) = f_A(\Phi_A(X))
\end{array}
\right.
$$

The elements $S_n, P_n, I_n$ and $F_n$ of $A$ are therefore characterized by the following formulas (where $n$ runs through $\mathbf{N}$):

(12) $$ \Phi_n(S_0, ..., S_n) = \Phi_n(X_0, ..., X_n) + \Phi_n(Y_0, ..., Y_n), $$
(13) $$ \Phi_n(P_0, ..., P_n) = \Phi_n(X_0, ..., X_n) \Phi_n(Y_0, ..., Y_n), $$
(14) $$ \Phi_n(I_0, ..., I_n) = - \Phi_n(X_0, ..., X_n), $$
(15) $$ \Phi_n(F_0, ..., F_n) = \Phi_{n+1}(X_0, ..., X_{n+1}). $$

Assign $X_n$ and $Y_n$ the weight $p^n$ for every $n \in \mathbf{N}$. We deduce from the remark of no 2 the following assertions:

$a)$ We have $S_n \in \mathbf{Z}[X_0, ..., X_n, Y_0, ..., Y_n]$ and $S_n$ is isobaric of weight $p^n$.
$b)$ We have $P_n \in \mathbf{Z}[X_0, ..., X_n, Y_0, ..., Y_n]$ and $P_n$ is isobaric of weight $p^n$ in each of the families $(X_0, ..., X_n)$ and $(Y_0, ..., Y_n)$.
$c)$ We have $I_n \in \mathbf{Z}[X_0, ..., X_n]$ and $I_n$ is isobaric of weight $p^n$.
$d)$ We have $F_n \in \mathbf{Z}[X_0, ..., X_{n+1}]$ and $F_n$ is isobaric of weight $p^{n+1}$.

Formula (2) makes it possible in practice to determine the polynomials $S_n, P_n, I_n$ and $F_n$ successively.

#### Example 1 {#ac-ix-s1-n3-exa-1 .statement}

We have

$$
S_0 = X_0 + Y_0
$$
$$
S_1 = X_1 + Y_1 - \sum_{i=1}^{p-1} \frac{1}{p} \binom{p}{i} X_0^i Y_0^{p-i}.
$$

Moreover, $S_n - X_n - Y_n$ belongs to the ring $\mathbf{Z}[X_0, ..., X_{n-1}, Y_0, ..., Y_{n-1}]$.

#### Example 2 {#ac-ix-s1-n3-exa-2 .statement}

We have

$$
P_0 = X_0 Y_0
$$
$$
P_1 = p X_1 Y_1 + X_0^p Y_1 + X_1 Y_0^p.
$$

#### Example 3 {#ac-ix-s1-n3-exa-3 .statement}

When $p \neq 2$, we have $I_n = - X_n$. For $p = 2$, we have

$$
I_0 = - X_0
$$
$$
I_1 = - (X_0^2 + X_1)
$$
$$
I_2 = - X_0^4 - X_0^2 X_1 - X_1^2 - X_2.
$$

#### Example 4 {#ac-ix-s1-n3-exa-4 .statement}

We have

$$
F_0 = X_0^p + p X_1
$$
$$
F_1 = X_1^p + p X_2 - \sum_{i=0}^{p-1} \binom{p}{i} p^{p-i-1} X_0^{pi} X_1^{p-i}.
$$

Since we have $\Phi_n(F_0, ..., F_n) \equiv \Phi_n(X_0^p, ..., X_n^p) \mod. p^{n+1}$. A for every $n \in \mathbf{N}$ (formulas (2) and (15)), it follows from prop. 1, b) that we have $F_n \equiv X_n^p \mod. p$. A for every $n \in \mathbf{N}$.

#### Remark {#ac-ix-s1-n3-rem-1 .statement}

Let $J$ be the set of integers $j \geq 1$. For every element $j$ of $J$, define the polynomial $\varphi_j$ of $\mathbf{Z}[(X_j)_{j \in J}]$ by the formula

$$
\varphi_j = \sum_d d X_d^{j/d},
$$

where the sum is taken over the elements of $J$ which divide $j$. For every integer $n \geq 0$, we have

$$
\varphi_{p^n} = \Phi_n(X_{p^0}, ..., X_{p^n}).
$$

For every ring $A$ and every element $m$ of $J$, we denote by $\varphi_m$ the mapping from $A^J$ into $A$ which associates to $(a_j)_{j \in J}$ $\varphi_m((a_j)_{j \in J})$; we denote by $\varphi_A$, or simply $\varphi$, the mapping from $A^J$ into itself which associates to $a = (a_j)_{j \in J}$ $(\varphi_m(a))_{m \in J}$.

Let $\mathcal{A} = \mathbf{Z}[(X_j)_{j \in J}, (Y_j)_{j \in J}]$ be the ring of polynomials with integer coefficients in the two families of indeterminates $X = (X_j)_{j \in J}$ and $Y = (Y_j)_{j \in J}$. One can show (p. 51, exerc. 34) that there exist in $\mathcal{A}$ elements

$$
s = (s_j)_{j \in J}, \quad p = (p_j)_{j \in J} \quad \text{and} \quad i = (i_j)_{j \in J},
$$

characterized by the following equalities:

$$
\varphi_{\mathcal{A}}(s) = \varphi_{\mathcal{A}}(\mathbf{X}) + \varphi_{\mathcal{A}}(\mathbf{Y})
$$
$$
\varphi_{\mathcal{A}}(p) = \varphi_{\mathcal{A}}(\mathbf{X}) \varphi_{\mathcal{A}}(\mathbf{Y})
$$
$$
\varphi_{\mathcal{A}}(i) = - \varphi_{\mathcal{A}}(\mathbf{X}) .
$$

### 4. The ring W(A) of Witt vectors

Let A be a ring. If $a = (a_n)_{n \in \mathbf{N}}$ and $b = (b_n)_{n \in \mathbf{N}}$ are elements of $A^\mathbf{N}$, we shall denote by $S_A(a, b)$ (resp. $P_A(a, b)$, resp. $I_A(a)$) or simply $S(a, b)$ (resp. $P(a, b)$, resp. $I(a)$) the sequence $(S_n(a_0, ..., a_n; b_0, ..., b_n))_{n \in \mathbf{N}}$ (resp. $(P_n(a_0, ..., a_n; b_0, ..., b_n))_{n \in \mathbf{N}}$, resp. $(I_n(a_0, ..., a_n))_{n \in \mathbf{N}}$). By substituting $a_n$ for $X_n$ and $b_n$ for $Y_n$, for every $n \in \mathbf{N}$, in formulas (12), (13) and (14), one obtains the equalities

(16)
$$
\Phi_A(S_A(a, b)) = \Phi_A(a) + \Phi_A(b)
$$
(17)
$$
\Phi_A(P_A(a, b)) = \Phi_A(a) \Phi_A(b)
$$
(18)
$$
\Phi_A(I_A(a)) = - \Phi_A(a) .
$$

We shall denote by W(A) the set $A^\mathbf{N}$ endowed with the composition laws $S_A$ and $P_A$.

Let $\rho : B \to A$ be a ring homomorphism. We shall denote by $\rho^\mathbf{N}$ or also W($\rho$) the mapping from $B^\mathbf{N}$ into $A^\mathbf{N}$ which associates to the element $b = (b_n)_{n \in \mathbf{N}}$ of $B^\mathbf{N}$ $(\rho(b_n))_{n \in \mathbf{N}}$. It follows immediately from the definitions that one has

(19)
$$
W(\rho) \circ S_B = S_A \circ (W(\rho) \times W(\rho))
$$
(20)
$$
W(\rho) \circ P_B = P_A \circ (W(\rho) \times W(\rho))
$$
(21)
$$
W(\rho) \circ I_B = I_A \circ W(\rho)
$$
(22)
$$
\rho^\mathbf{N} \circ \Phi_B = \Phi_A \circ W(\rho) .
$$

#### Lemma 3 {#ac-ix-s1-lem-3 .statement}

Let A be a ring. There exists a surjective homomorphism of rings $\rho : B \to A$, where B is a ring satisfying the following conditions: p is not a divisor of 0 in B, and there exists an endomorphism $\sigma$ of B such that $\sigma(b) \equiv b^p \mod. p.B$ for all $b \in B$.

It suffices indeed to set $B = \mathbf{Z}[(X_a)_{a \in A}]$, to take for $\sigma$ the endomorphism of B defined by $\sigma(X_a) = X_a^p$ for all $a \in A$, and for $\rho$ the homomorphism of B into A defined by $\rho(X_a) = a$ for all $a \in A$.

#### Theorem 1 {#ac-ix-s1-thm-1 .statement}

a) Let A be a (commutative) ring. Endowed with the addition $S_A$ and the multiplication $P_A$, W(A) is a (commutative) ring. The identity element for the addition is the sequence $0_A$ all of whose terms are zero; the identity element for the multiplication is the sequence $1_A$ all of whose terms are zero except the one of index 0 which is equal to $1_A$. The opposite of an element a of W(A) is $I_A(a)$.

b) Let $\rho : B \to A$ be a homomorphism of rings. Then $W(\rho) : W(B) \to W(A)$ is a homomorphism of rings.

c) Let $A$ be a ring. The mapping $\Phi_A$ is a homomorphism of rings from $W(A)$ into the product ring $A^\mathbf{N}$. In particular, for all $n \in \mathbf{N}$, the mapping $\Phi_n : a \mapsto \Phi_n(a_0, ..., a_n)$ is a homomorphism of rings from $W(A)$ into $A$.

Taking into account formulas (16), (17), (19) and (20), it suffices to prove assertion $a$.

Let $\rho : B \to A$ be a homomorphism of rings satisfying the conditions of Lemma 3. Let $B'$ be the subring of $B^\mathbf{N}$ formed by the elements $(b_n)_{n \in \mathbf{N}}$ such that $\sigma(b_n) \equiv b_{n+1} \mod. p^{n+1}$.B for all $n \in \mathbf{N}$. According to Prop. 2 of No. 2, $\Phi_B$ induces a bijection $\Phi'_B$ from $W(B)$ onto $B'$. Viewed from formulas (16) to (18) and the relations $\Phi_n(0_B) = 0$ and $\Phi_n(1_B) = 1_B$ ($n \in \mathbf{N}$), one sees by transport of structure that $W(B)$ is a ring, with identity element $0_B$ for the addition, $1_B$ for the multiplication, the opposite of $b$ being $I_B(b)$.

The mapping $W(\rho) : W(B) \to W(A)$ is surjective. According to formulas (19) and (20), the equivalence relation R on $W(B)$ associated with the mapping $W(\rho)$ is compatible with the ring structure of $W(B)$. Since $W(\rho)$ induces a bijection $\Psi$ from the quotient ring $W(B)/R$ onto $W(A)$, compatible with the laws of addition and multiplication, assertion $a$ follows from this by transport of structure.

#### Definition 1 {#ac-ix-s1-def-1 .statement}

Let $A$ be a ring. The ring $W(A)$ is called the ring of Witt vectors with coefficients in $A$.

For $a$ in $W(A)$ and $n$ in $\mathbf{N}$, the element $\Phi_n(a) = \Phi_n(a_0, ..., a_n)$ is sometimes called the ghost component of index $n$ of $a$.

#### Remark {#ac-ix-s1-n4-rem-1 .statement}

Let us take up again the notations of the remark of No. 3. Let $A$ be a ring. If $a$ and $b$ are elements of $A^J$ and $r = (r_j)_{j \in J}$ is an element of $A^J$, we denote by $r_A(a, b)$ the element $(r_j(a, b))_{j \in J}$ of $A^J$. Let us denote by $U(A)$ the set $A^J$ endowed with the composition laws $s_A$ and $p_A$. One can show (p. 52, Exercise 35) that, endowed with the addition $s_A$ and the multiplication $p_A$, $U(A)$ is a (commutative) ring; it is called the universal Witt ring of $A$. The identity element for the addition is the element of $U(A)$ all of whose components are zero; the identity element for the multiplication is the element of $U(A)$ all of whose components are zero except that of index 1 which is equal to $1_A$; the opposite of an element $a$ of $U(A)$ is $i_A(a)$. The mapping $\varphi_A$ is a ring homomorphism of $U(A)$ into the product ring $A^J$.

Let $\rho : B \to A$ be a ring homomorphism; we denote by $U(\rho)$ the mapping from $B^J$ into $A^J$ which associates with the element $(b_j)_{j \in J}$ of $B^J$ the element $(\rho(b_j))_{j \in J}$ of $A^J$. One can show (loc. cit.) that $U(\rho)$ is a ring homomorphism of $U(B)$ into $U(A)$.

### 5. The homomorphism F and the shift V

Let $A$ be a ring. In the sequel of this paragraph, we denote respectively by $+$ and $\times$ the laws of addition and multiplication in $W(A)$. We shall also write $0$ for $0_A$ and $1$ for $1_A$. We define $^1$ two mappings $F_A$ and $V_A$ (also simply denoted by $F$ and $V$) from $W(A)$ into itself by the formulas

$$
(23) \quad F_A(a) = (F_n(a_0, ..., a_{n+1}))_{n \in \mathbf{N}},
$$
$$
(24) \quad V_A(a) = (0, a_0, a_1, ...)
$$

(pour $a = (a_n)_{n \in \mathbf{N}}$ dans $W(A)$). The mapping $V_A$ is called the shift.

The formula
$$
(25) \quad \Phi_n(F_0(a), ..., F_n(a)) = \Phi_{n+1}(a_0, ..., a_{n+1}) \quad (n \in \mathbf{N})
$$
follows immediately from (15). It can also be written in the form
$$
(26) \quad \Phi_A \circ F_A = f_A \circ \Phi_A .
$$
The formula
$$
(27) \quad \Phi_A \circ V_A = v_A \circ \Phi_A
$$
follows from relation (3).

Let $\rho : B \to A$ be a homomorphism of rings. The relations
$$
(28) \quad W(\rho) \circ F_B = F_A \circ W(\rho)
$$
$$
(29) \quad W(\rho) \circ V_B = V_A \circ W(\rho)
$$
follow immediately from the definitions.

#### Proposition 3 {#ac-ix-s1-prop-3 .statement}

*Let A be a ring.*
  a) *The mapping $F_A$ is an endomorphism of the ring $W(A)$.*
  b) *The mapping $V_A$ is an endomorphism of the additive group underlying the ring $W(A)$.*
  c) *For every $a$ in $W(A)$, one has $F_A(V_A(a)) = p.a$ (sum in $W(A)$ of $p$ terms equal to $a$).*
  d) *Whatever $a$ and $b$ in $W(A)$ may be, one has*
$$
(30) \quad V_A(a \times F_A(b)) = V_A(a) \times b
$$
$$
(31) \quad V_A(a) \times V_A(b) = p.V_A(a \times b)
$$
(sum in $W(A)$ of $p$ terms equal to $V_A(a \times b)$).
  e) *Put $\mu = V_A(1) = (0, 1, 0, ...)$. For every $b$ in $W(A)$, one has*
$$
(32) \quad V_A(F_A(b)) = \mu \times b .
$$

$^1$ The letter $F$ is the initial of the name Frobenius, and the letter $V$ that of the German word *Verschiebung*.

f) For every element $a$ of $W(A)$ denote by $a^{*p}$ the product in $W(A)$ of $p$ elements equal to $a$. Then one has

$$
(33) \quad F_A(a) \equiv a^{*p} \mod. p.W(A) \quad (\text{ideal of } W(A) \text{ generated by } p.\mathbf{1}) .
$$

Let $\rho : B \to A$ be a homomorphism of rings satisfying the conditions of Lemma 3 of No. 4. Then $W(\rho) : W(B) \to W(A)$ is a surjective homomorphism of rings, and $\Phi_B : W(B) \to B^N$ is an injective homomorphism of rings. Moreover, $f_B : B^N \to B^N$ is a homomorphism of rings. According to the formulas (26) and (28), one has

$$
\Phi_B \circ F_B = f_B \circ \Phi_B, \quad W(\rho) \circ F_B = F_A \circ W(\rho),
$$

whence immediately assertion $a$. Assertion $b$ follows in an analogous manner from the formulas (27) and (29) and from the fact that $v_B$ is an endomorphism of the additive group underlying $B^N$.

Let $a$ be an element of $W(A)$, and choose an element $x$ of $W(B)$ which $W(\rho)$ maps onto $a$. Put $\xi = \Phi_B(x)$. It follows immediately from the definitions of $f_B$ and $v_B$ that one has $f_B(v_B(\xi)) = p.\xi$ (sum in $B^N$ of $p$ terms equal to $\xi$). According to formulas (26) and (27) (where A is replaced by B), the elements $F_B(V_B(x))$ and $p.x$ of $W(B)$ therefore have the same image $p.\xi$ by the injective mapping $\Phi_B$, and hence are equal. The formula $F_A(V_A(a)) = p.a$ then follows from relations (28) and (29). This proves $c$.

Reasoning in an analogous manner, we reduce the proof of formula (30) to that of the relation

$$
v_B(\xi f_B(\eta)) = v_B(\xi) \eta
$$

for $\xi, \eta$ in $B^N$. Now this results from the equalities

$$
\xi f_B(\eta) = (\xi_0 \eta_1, \xi_1 \eta_2, ...)
$$
$$
v_B(\xi) \eta = (0, p\xi_0 \eta_1, p\xi_1 \eta_2, ...)
$$

Taking into account $b$ and $c$, formula (31) results from formula (30), where $b$ is replaced by $V_A(b)$. Formula (32) is the particular case $a = 1$ of formula (30).

In an analogous manner, we reduce the proof of formula (33) to that of the relation

$$
f_B(\xi) \equiv \xi^p \mod. p.\Phi_B(B^N),
$$

where $\xi^p$ denotes the product in $B^N$ of $p$ elements equal to $\xi$. By Prop. 2, c) of No. 2, this is equivalent to the fact that for every $n \geqslant 0$, one has

$$
\sigma(\xi_{n+1} - \xi_n^p) \equiv \xi_{n+2} - \xi_{n+1}^p \mod. p^{n+2}B .
$$

Now, for every $n \geqslant 0$, one has, by loc. cit.,

$$
\sigma(\xi_n) \equiv \xi_{n+1} \mod. p^{n+1}B
$$

since $\xi = \Phi_B(x)$; one deduces from this, thanks to Lemma 1 of No. 1,

$$
\sigma(\xi_n)^p \equiv \xi_{n+1}^p \mod. p^{n+2}\mathbf{B}.
$$

This proves the desired relation.

#### Remark {#ac-ix-s1-n5-rem-1 .statement}

For the definition of mappings analogous to the mappings F and V, in the case of the universal Witt ring, see exercises 36, 37 and 38, p. 52 and following.

### 6. Filtration and topology of the ring W(A)

#### Lemma 4 {#ac-ix-s1-lem-4 .statement}

Let A be a ring and m $\geqslant 1$ an integer. One has

(34)
$$
a = (a_0, ..., a_{m-1}, 0, ...) + (\underbrace{0, ..., 0}_{m \text{ terms}}, a_m, a_{m+1}, ...)
$$
for every $a$ in W(A).

Let $\rho : B \to A$ be a ring homomorphism satisfying the conditions of Lemma 3 of No. 4. Then $W(\rho) : W(B) \to W(A)$ is a surjective homomorphism of rings, and $\Phi_B : W(B) \to B^N$ is an injective homomorphism. It is therefore enough to prove that one has

(35)
$$
\Phi_n(b) = \Phi_n(b_0, ..., b_{m-1}, 0, ...) + \Phi_n(0, ..., 0, b_m, b_{m+1}, ...)
$$
whatever $b$ in W(B) and the integers $m \geqslant 1, n \geqslant 0$ may be. Now one has

$$
\Phi_n(b_0, ..., b_{m-1}, ...) = \Phi_n(b_0, ..., b_n) \quad \text{if} \quad 0 \leqslant n < m
$$
$$
= \sum_{i=0}^{m-1} p^i \cdot b_i^{p^{n-i}} \quad \text{if} \quad m \leqslant n
$$
$$
\Phi_n(0, ..., 0, b_m, b_{m+1}, ...) = 0 \quad \text{if} \quad 0 \leqslant n < m
$$
$$
= \sum_{i=m}^n p^i \cdot b_i^{p^{n-i}} \quad \text{if} \quad m \leqslant n,
$$
whence formula (35).

Soit A a ring. For every integer $m \geqslant 0$, denote by $V_m(A)$ the set of Witt vectors $a = (a_n)_{n \in \mathbf{N}}$ such that $a_n = 0$ for $0 \leqslant n < m$. It is the image of the m-th power $V^m$ of the mapping $V_A$. The formulas

(36)
$$
V^m(a + b) = V^m(a) + V^m(b)
$$
(37)
$$
V^m(a) \times b = V^m(a \times F^m(b))
$$
result from prop. 3 of No. 5 by induction on $m$. They imply that $V_m(A)$ is an ideal of W(A).

In what follows, we shall endow $W(A)$ with the topology $\mathcal{T}$ associated with the filtration $(V_m(A))_{m \in \mathbf{Z}}$. Since $V_m(A)$ is an ideal of $W(A)$ for every $m \in \mathbf{Z}$, the topology $\mathcal{T}$ is compatible with the ring structure of $W(A)$ (TG, III, p. 49, example 3). Let $a \in W(A)$; the sets $a + V_m(A)$, where $m$ runs through $\mathbf{N}$, form a fundamental system of neighbourhoods of $a$ for $\mathcal{T}$. Now, it follows from lemma 4 that $a + V_m(A)$ consists of the Witt vectors $b$ such that $a_i = b_i$ for $0 \leq i < m$. Consequently, $\mathcal{T}$ is none other than the product topology on $A^\mathbf{N}$ of the discrete topology on each of the factors, and $W(A)$ is therefore a separated and complete topological ring (TG, II, p. 17, prop. 10 and TG, III, p. 22, prop. 4).

Let us denote by $\tau_A$ (or simply $\tau$) the mapping of $A$ into $W(A)$ which associates with an element $a$ of $A$ $(a, 0, 0, ...)$ . We have $\Phi_n(\tau(a)) = a^{p^n}$ for every $n \in \mathbf{N}$. For every ring homomorphism $\rho : B \to A$, we have $W(\rho) \circ \tau_B = \tau_A \circ \rho$.

#### Proposition 4 {#ac-ix-s1-prop-4 .statement}

*Let $a$ and $b$ be in $A$ and let $x = (x_n)_{n \in \mathbf{N}}$ be an element of $W(A)$.*

a) *We have the formulas*

$$
\tau(ab) = \tau(a) \times \tau(b)
$$
$$
\tau(a) \times x = (a^{p^n} x_n)_{n \in \mathbf{N}}.
$$

b) *The series with general term $V^n(\tau(x_n))$ is convergent in $W(A)$, with sum $x$.*
Let $n$ be a positive integer. The polynomial $P_n(X_0, ..., X_n; Y_0, ..., Y_n)$ introduced in No. 3 is isobaric of weight $p^n$ in the family $(X_0, ..., X_n)$ when $X_i$ is assigned the weight $p^i$. Hence
$$
P_n(X_0, 0, ..., 0; Y_0, ..., Y_n) = X_0^{p^n} P_n(1, 0, ..., 0; Y_0, ..., Y_n).
$$
Since $1 = (1, 0, 0, ...)$ is the unit element of the ring of Witt vectors with coefficients in $\mathbf{Z}[(X_n)_{n \in \mathbf{N}}, (Y_n)_{n \in \mathbf{N}}]$, we have
$$
P_n(1, 0, ..., 0; Y_0, ..., Y_n) = Y_n.
$$
By substituting $a$ for $X_0$ and $x_i$ for $Y_i$, we deduce from (40) and (41) the relation:
$$
P_n(a, 0, ..., 0; x_0, ..., x_n) = a^{p^n} x_n.
$$
According to the definition of the multiplication in $W(A)$, we have proved (39); formula (38) is a particular case of (39).

*Let us prove b).* By definition, $V^n(\tau(x_n))$ is the sequence all of whose components are zero, except the one with index $n$, which is equal to $x_n$. It follows from Lemma 4, by induction on $m$, that we have
$$
\sum_{n=0}^m V^n(\tau(x_n)) = (x_0, ..., x_m, 0, 0, ...)
$$

for every integer $m \geq 0$; we deduce b) by passing to the limit since the topology $\mathcal{T}$ on $W(A)$ is the product of the discrete topologies of the factors $A$.

### 7. The rings $W_n(A)$ of Witt vectors of finite length

#### Definition 2 {#ac-ix-s1-def-2 .statement}

Let $A$ be a ring and let $n \geq 1$ be an integer. We denote by $W_n(A)$ the quotient ring $W(A)/V_n(A)$.

Given elements $a_0, ..., a_{n-1}$ of $A$, we denote by $[a_0, ..., a_{n-1}]$ or $[a_i]_{0 \leq i < n}$ the class modulo $V_n(A)$ of the element $(a_0, ..., a_{n-1}, 0, 0, ...)$ of $W(A)$. According to Lemma 4 of No. 6, the mapping $(a_0, ..., a_{n-1}) \mapsto [a_0, ..., a_{n-1}]$ from $A^n$ into $W_n(A)$ is a bijection. For this reason, we say that the elements of $W_n(A)$ are the Witt vectors of length $n$; by analogy, one sometimes qualifies the elements of $W(A)$ as Witt vectors of infinite length.

We denote by $\pi_n$ the canonical homomorphism from $W(A)$ into $W_n(A)$. According to Lemma 4 of No. 6, we have
$$
\pi_n(a) = [a_0, ..., a_{n-1}]
$$
for every $a = (a_n)_{n \in \mathbf{N}}$ in $W(A)$.

According to the definition of the operations in $W(A)$, we have the following description of the operations in $W_n(A)$:
$$
[a_0, ..., a_{n-1}] + [b_0, ..., b_{n-1}] = [S_i(a_0, ..., a_i; b_0, ..., b_i)]_{0 \leq i < n}
$$
$$
[a_0, ..., a_{n-1}] \times [b_0, ..., b_{n-1}] = [P_i(a_0, ..., a_i; b_0, ..., b_i)]_{0 \leq i < n}
$$
$$
- [a_0, ..., a_{n-1}] = [I_i(a_0, ..., a_i)]_{0 \leq i < n}.
$$

Moreover, the identity element of the addition in $W_n(A)$ is $[0, ..., 0]$ and that of the multiplication is $[1, 0, ..., 0]$.

Let $i$ be an integer such that $0 \leq i \leq n$. By passing to the quotient, the homomorphism $\Phi_i$ from $W(A)$ into $A$ defines a homomorphism $\Phi_i$ from $W_n(A)$ into $A$. This associates with the Witt vector $[a_0, ..., a_{n-1}]$ the element $\Phi_i(a_0, ..., a_i)$ of $A$ (also called the ghost component of index $i$ of $[a_0, ..., a_{n-1}]$).

Let $\rho : B \to A$ be a ring homomorphism. By passing to the quotients, the homomorphism $W(\rho)$ from $W(B)$ into $W(A)$ defines a homomorphism $W_n(\rho)$ from $W_n(B)$ into $W_n(A)$. It is described by the formula
$$
W_n(\rho)[b_0, ..., b_{n-1}] = [\rho(b_0), ..., \rho(b_{n-1})]
$$
for every $[b_0, ..., b_{n-1}]$ in $W_n(B)$.

Let $m$ and $n$ be two integers such that $1 \leq n \leq m$. We have $V_n(A) \supset V_m(A)$, whence a canonical homomorphism from $W_m(A) = W(A)/V_m(A)$ onto $W_n(A) = W(A)/V_n(A)$; this homomorphism will be denoted by $\pi_{n,m}$. Explicitly, we have
$$
\pi_{n,m}[a_0, ..., a_{m-1}] = [a_0, ..., a_{n-1}]
$$

for $[a_0, ..., a_{m-1}]$ in $W_m(A)$. The family $(W_n(A), \pi_{n,m})$ is a projective system of rings and the mapping $\pi : a \mapsto (\pi_n(a))_{n \geq 1}$ is a ring homomorphism from $W(A)$ into $\lim_{\leftarrow} W_n(A)$, called canonical. Since $W(A)$ is separated and complete for the filtration $(V_n(A))_{n \in \mathbf{Z}}$ (*cf.* No. 6), the canonical homomorphism $\pi$ is an isomorphism of topological rings, when $W_n(A)$ is endowed with the discrete topology for every integer $n \geq 1$ (III, § 2, No. 6).

Henceforth, the homomorphisms $\pi_n$ and $\pi_{n,m}$ will be called *projection homomorphisms* from $W(A)$ into $W_n(A)$, and from $W_m(A)$ into $W_n(A)$ respectively.

#### Example 1 {#ac-ix-s1-n7-exa-1 .statement}

The homomorphism $\Phi_0 : W_1(A) \to A$ is an isomorphism.

#### Example 2 {#ac-ix-s1-n7-exa-2 .statement}

Let us make explicit the operations in $W_2(A)$. We have

$$
[a_0, a_1] + [b_0, b_1] = \left[ a_0 + b_0, a_1 + b_1 - \sum_{i=1}^{p-1} \frac{1}{p} \binom{p}{i} a_0^i b_0^{p-i} \right]
$$

$$
[a_0, a_1] \times [b_0, b_1] = [a_0 b_0, a_0^p b_1 + a_1 b_0^p + p \cdot a_1 b_1]
$$

for $[a_0, a_1]$ and $[b_0, b_1]$ in $W_2(A)$. The ghost components of $[a_0, a_1]$ are $a_0$ and $a_0^p + p \cdot a_1$.

#### Example 3 {#ac-ix-s1-n7-exa-3 .statement}

Let $n \geq 1$ be an integer. If $a_0, ..., a_{n-1}, b_0, ..., b_{n-1}$ are integers such that $a_i \equiv b_i \bmod p$ for $0 \leq i < n$, one has (No. 1, prop. 1)

$$
\Phi_{n-1}(a_0, ..., a_{n-1}) \equiv \Phi_{n-1}(b_0, ..., b_{n-1}) \bmod p^n.
$$

Consequently, $\Phi_{n-1}$ defines by passing to the quotients a ring homomorphism $\varphi_n : W_n(\mathbf{Z}/p\mathbf{Z}) \to \mathbf{Z}/p^n\mathbf{Z}$. The image of $\varphi_n$ is a subgroup of $\mathbf{Z}/p^n\mathbf{Z}$ containing 1, hence $\varphi_n$ is surjective. Since the finite sets $W_n(\mathbf{Z}/p\mathbf{Z})$ and $\mathbf{Z}/p^n\mathbf{Z}$ have the same cardinal $p^n$, $\varphi_n$ is an isomorphism.

Let $m$ and $n$ be integers such that $1 \leq n \leq m$. There exists a unique ring homomorphism $\alpha_{n,m} : \mathbf{Z}/p^m\mathbf{Z} \to \mathbf{Z}/p^n\mathbf{Z}$; consequently the diagram

$$
\begin{array}{ccc}
\mathbf{Z}/p^m\mathbf{Z} & \xrightarrow{\alpha_{n,m}} & \mathbf{Z}/p^n\mathbf{Z} \\
\varphi_m \uparrow & & \varphi_n \uparrow \\
W_m(\mathbf{Z}/p\mathbf{Z}) & \xrightarrow{\pi_{n,m}} & W_n(\mathbf{Z}/p\mathbf{Z})
\end{array}
$$

is commutative. It follows that $\varphi = \lim \varphi_n$ is an isomorphism of topological rings from $W(\mathbf{Z}/p\mathbf{Z}) = \lim_{\leftarrow} W_n(\mathbf{Z}/p\mathbf{Z})$ onto $\mathbf{Z}_p = \lim_{\leftarrow} \mathbf{Z}/p^n\mathbf{Z}$ (III, § 2, No. 12, example 3).

Let $m$ and $n$ be two integers $\geq 1$. By construction, one has an exact sequence of additive groups

(E)
$$
0 \longrightarrow W(A) \xrightarrow{\nu^m} W(A) \xrightarrow{\pi_m} W_m(A) \longrightarrow 0.
$$

By passing to the quotients, the endomorphism $V^n$ of the additive group of $W(A)$ defines a homomorphism $V^n_m$ of the additive group of $W_m(A)$ into that of $W_{m+n}(A)$. In other words, one has a commutative diagram

$$
\begin{array}{ccc}
W(A) & \xrightarrow{V^n} & W(A) \\
\pi_m \downarrow & & \pi_{n+m} \downarrow \\
W_m(A) & \xrightarrow{V^n_m} & W_{n+m}(A)
\end{array}
$$

By passing to the quotients, one deduces from the exact sequence (E) an exact sequence

(E') $$ 0 \longrightarrow W_m(A) \xrightarrow{V^n_m} W_{n+m}(A) \xrightarrow{\pi_{n,n+m}} W_n(A) \longrightarrow 0 . $$

One has

(45) $$ V^n_m[a_0, ..., a_{m-1}] = [\underbrace{0, ..., 0}_{n \text{ fois}}, a_0, ..., a_{m-1}], $$

for every element $[a_0, ..., a_{m-1}]$ of $W_m(A)$.

According to prop. 3, c) of No. 5, one has $FV^{m+1}(a) = p.V^m(a)$ for every $a$ in $W(A)$ and one consequently has $F(V_{m+1}(A)) \subset V_m(A)$. By induction on $n$, one deduces that $F^n$ maps $V_{n+m}(A)$ into $V_m(A)$, and hence defines, by passing to the quotients, a ring homomorphism $F^n_m : W_{n+m}(A) \to W_m(A)$. By construction, one has a commutative diagram

$$
\begin{array}{ccc}
W(A) & \xrightarrow{F^n} & W(A) \\
\pi_{n+m} \downarrow & & \pi_m \downarrow \\
W_{n+m}(A) & \xrightarrow{F^n_m} & W_m(A)
\end{array}
$$

Recall (No. 3) that the polynomial $F_i$ belongs to $\mathbf{Z}[X_0, ..., X_{i+1}]$ for every integer $i \geqslant 0$; the homomorphism $F^1_m$ from $W_{m+1}(A)$ into $W_m(A)$ is therefore made explicit as follows:

(46) $$ F^1_m[a_0, ..., a_m] = [F_i(a_0, ..., a_{i+1})]_{0 \leqslant i < m}. $$

Let $a \in W_m(A)$, $a' \in W_m(A)$ and $b \in W_{m+1}(A)$. The following formulas result by passing to the quotients from prop. 3 of No. 5:

(47) $$ F^1_m(V^1_m(a)) = p.a $$
(48) $$ V^1_m(a \times F^1_m(b)) = V^1_m(a) \times b $$
(49) $$ V^1_m(a) \times V^1_m(a') = p.V^1_m(a \times a') $$
(50) $$ V^1_m(F^1_m(b)) = \mu_{m+1} \times b $$

(avec $\mu_{m+1} = [0, 1, 0, ..., 0]$).

### 8. The ring of Witt vectors with coefficients in a ring of characteristic $p$

#### Proposition 5 {#ac-ix-s1-prop-5 .statement}

Let $A$ be a ring of characteristic $p$ (A, V, p. 2). Whatever the elements $a$ and $b$ of $W(A)$, and the positive integers $m, n$, one has, if $a = (a_n)_{n \in \mathbf{N}}$,

$$
(51) \quad F(a) = (a_n^p)_{n \in \mathbf{N}}
$$
$$
(52) \quad p.a = VF(a) = FV(a) = (0, a_0^p, a_1^p, ...)
$$
$$
(53) \quad V^m(a) \times V^n(b) = V^{m+n}(F^n(a) \times F^m(b)) .
$$

Formula (51) results from Example 4 of No. 3. One immediately deduces from this the equality

$$
VF(a) = FV(a) = (0, a_0^p, a_1^p, ...) ,
$$

and the equality $p.a = FV(a)$ has been proved (No. 5, prop. 3), whence (52).

Let us prove (53). According to formula (37) (where one substitutes $V^n(b)$ for $b$), one has

$$
(54) \quad V^m(a) \times V^n(b) = V^m(a \times F^m(V^n(b))) .
$$

From formula (37), one also deduces

$$
(55) \quad V^n(F^m(b)) \times a = V^n(F^m(b) \times F^n(a)) .
$$

Formula (53) then results from (54) and (55) and from the relation $F^m \circ V^n = V^n \circ F^m$, itself a consequence of (51).

#### Corollary {#ac-ix-s1-n8-cor-1 .statement}

If $m$ and $n$ are two positive integers, one has

$$
V_m(A) \times V_n(A) \subset V_{m+n}(A) .
$$

This results from formula (53), since $V_m(A)$ is the image of $V^m : W(A) \to W(A)$.

#### Proposition 6 {#ac-ix-s1-prop-6 .statement}

Let $A$ be a ring.

a) For every integer $k \geqslant 1$, one has $(V_1(A))^k = p^{k-1} \cdot V_1(A)$.

b) Suppose that $A$ is a ring of characteristic $p$. On the ring $W(A)$, the $V_1(A)$-adic topology and the $p$-adic topology coincide, and they are finer than the product topology $\mathcal{C}$ (cf. No. 6). The ring $W(A)$ is separated and complete for the $p$-adic topology.

Let us prove $a)$ by induction on $k$. The case $k = 1$ is evident. Suppose $k \geqslant 2$. By the induction hypothesis, one has $V_1(A)^{k-1} = p^{k-2} \cdot V_1(A)$ and consequently $V_1(A)^k = p^{k-2} \cdot (V_1(A))^2$. But it follows from prop. 3, $d)$, formula (31), of No. 5 that one has $(V_1(A))^2 = p \cdot V_1(A)$, whence $a)$.

Suppose now that $A$ is of characteristic $p$. As one has

$$
p \cdot W(A) = VF(W(A)) \subset V_1(A) \quad (\text{formula (52)}) ,
$$

one deduces from $a)$ the inclusions $p^k.W(A) \subset (V_1(A))^k \subset p^{k-1}.W(A)$, and from the corollary to prop. 5 the inclusion $(V_1(A))^k \subset V_k(A)$, for every integer $k \geqslant 1$. The first assertion of $b)$ follows.

Let $k$ be an integer $\geqslant 1$. According to formula (52), the ideal $p^k.W(A)$ of $W(A)$ is the set of elements $a = (a_n)_{n \in \mathbf{N}}$ of $W(A)$ such that one has $a_n = 0$ for $n < k$ and $a_n \in A^{p^k}$ for $n \geqslant k$. It is therefore closed for the topology $\mathcal{G}$. Since $W(A)$ is separated and complete for the topology $\mathcal{G}$ (no 6) and since the ideals $p^k.W(A)$ of $W(A)$, for $k \geqslant 1$, form a basis of neighbourhoods of $0$ in $W(A)$ for the $p$-adic topology, the ring $W(A)$ is separated and complete for the $p$-adic topology (TG, III, p. 26, cor. 1 to prop. 10).

#### Proposition 7 {#ac-ix-s1-prop-7 .statement}

*Let A be a perfect ring of characteristic p.*

$a)$ *For every element $a = (a_n)_{n \in \mathbf{N}}$ of $W(A)$, the series with general term $p^n \tau(a_n^{p^{-n}})$ is convergent in $W(A)$, with sum $a$.*

$b)$ *On $W(A)$, the $V_1(A)$-adic topology, the $p$-adic topology and the topology $\mathcal{G}$ coincide. More precisely, one has $V_n(A) = p^n.W(A) = (V_1(A))^n$ for every integer $n \geqslant 0$. In particular $\Phi_0$ defines an isomorphism of $W(A)/p.W(A)$ onto $A$.*

By definition (A, V, p. 5), the mapping $a \mapsto a^p$ is an automorphism of the ring $A$. According to prop. 5, F is therefore an automorphism of the ring $W(A)$, and one has, for every $n \in \mathbf{N}$,

$$
p^n.W(A) = V^n F^n(W(A)) = V^n(W(A)) = V_n(A).
$$

In particular, one has $(V_1(A))^n = (p.W(A))^n = p^n.W(A)$. The assertion $b)$ follows from this.

According to prop. 5, one has

$$
p^n.\tau(a_n^{p^{-n}}) = V^n F^n \tau(a_n^{p^{-n}}) = V^n \tau(a_n),
$$

and the assertion $a)$ follows from prop. 4 of no 6.

#### Proposition 8 {#ac-ix-s1-prop-8 .statement}

*Let A be a field of characteristic p. The ring $W(A)$ is a separated and complete integral local ring, with maximal ideal $V_1(A)$ and residue field isomorphic to A. If the field A is perfect, the ring $W(A)$ is a discrete valuation ring, and its maximal ideal is $p.W(A)$.*

The homomorphism $\Phi_0$ defines an isomorphism of $W(A)/V_1(A)$ onto $A$ (no 7, example 1). The ideal $V_1(A)$ of $W(A)$ is therefore maximal. Since the ring $W(A)$ is separated and complete for the $V_1(A)$-adic topology (prop. 6, $b$), it is a local ring, with maximal ideal $V_1(A)$ (III, § 2, no 13, prop. 19).

Let $a$ and $b$ be two nonzero elements of $W(A)$. There exist integers $m \geqslant 0$ and $n \geqslant 0$, and elements $a' = (a'_n)_{n \in \mathbf{N}}$ and $b' = (b'_n)_{n \in \mathbf{N}}$ of $W(A)$ such that $a = V^m(a')$, $b = V^n(b')$ and that the elements $a'_0$ and $b'_0$ of $A$ are nonzero. Then the component of index $m + n$ of $a \times b$ is equal to the component of index 0 of $F^n(a') \times F^m(b')$ (formula (53)), that is to say to ${a'_0}^{p^n} {b'_0}^{p^m}$ (formula (51) and No. 3, Example 2). Consequently $a \times b$ is nonzero and $W(A)$ is an integral domain.

If the field $A$ is perfect, the maximal ideal $V_1(A)$ of $W(A)$ is equal to $p.W(A)$ (Prop. 7, b)) and consequently W(A) is a discrete valuation ring (VI, § 3, No. 6, Prop. 9, c)).

#### Remark 1 {#ac-ix-s1-n8-rem-1 .statement}

Let A be a field of characteristic p. One can now prove that the ring W(A) is noetherian if and only if A is perfect (p. 43, Exercise 9).

#### Remark 2 {#ac-ix-s1-n8-rem-2 .statement}

Let A be a ring of characteristic p. According to Prop. 5, one has the formulas

$$
F_m^n[a_0, ..., a_{n+m-1}] = [a_0^{p^n}, ..., a_{m-1}^{p^n}]
$$
$$
p^n.[a_0, ..., a_{n+m-1}] = [\underbrace{0, ..., 0}_{n \text{ fois}}, a_0^{p^n}, ..., a_{m-1}^{p^n}]
$$

for every Witt vector $[a_0, ..., a_{n+m-1}]$ of length $n + m$.

In fact, the mapping $F : W(A) \to W(A)$ allows one, by passing to the quotients by $V_m(A)$, to define a mapping $\overline{F}_m : W_m(A) \to W_m(A)$. One has the formula

$$
\overline{F}_m[a_0, ..., a_{m-1}] = [a_0^p, ..., a_{m-1}^p].
$$

The mappings $V_m^1 \circ \overline{F}_m$ and $\overline{F}_{m+1} \circ V_m^1$ from $W_m(A)$ into $W_{m+1}(A)$ are equal and are obtained, by passing to the quotient, from multiplication by $p$ in $W_{m+1}(A)$.

## EXERCISES {#ac-ix-s1-exercises}

In Exercises 1 to 27, $p$ is a fixed prime number. If $A$ is a ring, the ring of Witt vectors $W(A)$ is the one attached to the prime number $p$.
