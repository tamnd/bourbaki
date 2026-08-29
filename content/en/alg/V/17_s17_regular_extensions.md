---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 17
section_title: Regular extensions
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.180-A V.181
pdf_pages: 0251-0259, 0294-0295
extraction: ocr
subsections:
    - "no": 1
      title: Complements on the relative separable algebraic closure
      page: 137
      pdf_page: 251
    - "no": 2
      title: The tensor product of extensions
      page: 139
      pdf_page: 253
    - "no": 3
      title: Regular algebras
      page: 140
      pdf_page: 254
    - "no": 4
      title: Regular extensions
      page: 141
      pdf_page: 255
    - "no": 5
      title: Characterization of regular extensions
      page: 142
      pdf_page: 256
    - "no": 6
      title: Application to composite extensions
      page: 143
      pdf_page: 257
statements: 20
exercises: 5
content_sha256: 0970c4aa41158ef33231d08b21a0ce6a9b85ee1660b0f424d771a6b9760e1253
---

## § 17. REGULAR EXTENSIONS

### 1. Complements on the relative separable algebraic closure

#### Theorem 1 (Zariski) {#alg-v-s17-thm-1 .statement}

— *Let K be a field, L an extension of K, $K_1$ the relative separable algebraic closure of K in L (V, p. 44), $K_2$ the relative algebraic closure of K in L (V, p. 19) and $(X_i)_{i \in I}$ a family of indeterminates. Then $K_1(X_i)_{i \in I}$ is the relative separable algebraic closure of $K(X_i)_{i \in I}$ in $L(X_i)_{i \in I}$, and $K_2(X_i)_{i \in I}$ is the relative algebraic closure of $K(X_i)_{i \in I}$ in $L(X_i)_{i \in I}$.

A) Suppose that E is a field and F an extension field of E and that every element of F which is separable algebraic over E belongs to E. Let $u$ be an element of $F(X)$ which is separable algebraic over $E(X)$; we shall show that $u$ belongs to $E(X)$. There exist in $F(X)$ two relatively prime polynomials P and Q such that $u = P/Q$ and we may take Q to be monic. Let S be the *finite* subset of F consisting of the coefficients of P and Q, $F_0 = E(S)$ and let A be an E-derivation of $F_0$ into $F_0$. Let $D$ be the derivation of $F_0(X)$ into itself which agrees with $A$ on $F_0$ and maps $X$ to $0$ (V, p. 128, Prop. 3).

Since $u \in F_0(X)$ is separable algebraic over $E(X)$ and $D$ is zero on $E(X)$, we have $D(u) = 0$ (V, p.129, Prop. 4), whence $D(P) . Q = P . D(Q)$. Since $P$ and $Q$ are relatively prime, we conclude that $Q$ divides $D(Q)$ (IV, p. 13, Cor. 4). Now $Q$ may be written in the form
$$
Q(X) = X^n + a_1 X^{n-1} + \ldots + a_{n-1} X + a_n
$$
with $a,, \ldots, a,$ in $F_0$; since $D(x) = 0$, we thus have
$$
D(Q) = \Delta(a_1) X^{n-1} + \cdots + \Delta(a_{n-1}) X + \Delta(a_n)
$$
whence $\deg D(Q) < \deg Q$. Since $Q$ divides $D(Q)$, this is possible only if $D(Q) = 0$. But then $D(P) = 0$ because $D(P) . Q = P . D(Q)$. Now (1) and a similar formula for $P$ show that $A$ annihilates the set $S$ of coefficients of $P$ and $Q$, whence $A = 0$, because $F_0 = E(S)$. By V, p. 135, Cor. 2, the finitely generated extension $F_0$ of $E$ is thus separable algebraic; by the hypotheses on $E$ and $F$ we have $F_0 = E$, so finally $u \in E(X)$.

B) Suppose now that $E$ is relatively algebraically closed in the extension field $F$ and denote by $p$ the characteristic exponent of $E$. Let $u$ be an element of $F(X)$ which is algebraic over $E(X)$. There exists an integer $f \geq 0$ such that $v = u^{p^f}$ is separable algebraic over $E(X)$ (V, p. 44, Prop. 13). By A) we thus have $v \in E(X)$. There exists a unique representation of $u$ in the form $P/Q$ with relatively prime polynomials $P$ and $Q$ in $F[X]$ and $Q$ monic; we have a similar decomposition $v = P_1/Q_1$ with $P_1$ and $Q_1$ relatively prime in $E[X]$ and $Q_1$ monic. It follows that $P_1/Q_1 = P^{p^f}/Q^{p^f}$; the polynomials $P^{p^f}$ and $Q^{p^f}$ are relatively prime in $F[X]$ (IV, p. 13, Cor. 6), like $P_1$ and $Q_1$, and $Q^{p^f}$ is monic. It follows that $P^{p^f} = P_1 \in E[X]$ and $Q^{p^f} = Q_1 \in E[X]$. Therefore the coefficients of $P$ and $Q$ are $p$-radical over $E$, and hence belong to $E$ because $E$ is relatively algebraically closed in $F$. We thus have $P \in E[X]$, $Q \in E[X]$ and finally $u \in E(X)$. This proves $E(X)$ to be relatively algebraically closed in $F(X)$.

C) We use the notation of Theorem 1. Since $K_1$ is a separable algebraic extension of $K$, the extension $K_1(X_i)_{i \in I}$ of $K(X_i)_{i \in I}$, is algebraic and separable (V, p. 39, Prop. 6). Moreover, every element of $L$ which is algebraic and separable over $K$, belongs to $K$, (V, p. 44, Prop. 13, a)). Let $J$ be a finite subset of $I$; by an immediate induction on the cardinal of $J$ we deduce from A) that every element of $L(X_i)_{i \in I}$, which is algebraic and separable over $K(X_i)_{i \in I}$, belongs to $K_1(X_i)_{i \in J}$. Finally let $u$ be an element of $L(X_i)_{i \in I}$, algebraic and separable over $K(X_i)_{i \in I}$; there exists a finite subset $J$ of $I$ such that $u$ belongs to $L(X_i)_{i \in I}$ and is algebraic and separable over $K(X_i)_{i \in J}$; by what has been said, $u$ belongs to $K_1(X_i)_{i \in J}$, and a fortiori to $K_1(X_i)_{i \in I}$.

We have thus deduced from A) that $K_1(X_i)_{i \in I}$ is the relative separable closure of $K(X_i)_{i \in I}$ in $L(X_i)_{i \in I}$; in the same way it follows from B) that $K_2(X_i)_{i \in I}$ is the relative algebraic closure of $K(X_i)_{i \in I}$ in $L(X_i)_{i \in I}$.

### 2. The tensor product of extensions

#### Proposition 1 {#alg-v-s17-prop-1 .statement}

— Let $\Omega$ be an extension of a field $K$ and let $L, M$ be two subextensions of $\Omega$ which are algebraically disjoint over $K$. Suppose that the relative separable algebraic closure of $K$ in $L$ is equal to $K$^1. Let $\varphi$ be the $K$-algebra homomorphism of $L \otimes_K M$ into $\Omega$ mapping $x \otimes y$ to $xy$ for $x \in L, y \in M$, and let $p$ be the kernel of $\varphi$. Then $p$ is the set of nilpotent elements of $L \otimes_K M$ and this is the smallest prime ideal of $L \otimes_K M$.

On replacing $\Omega$ by an algebraic closure if necessary, we may suppose $\Omega$ algebraically closed. Let $B$ be a transcendence basis of $M$ over $K$, $N$ the relative algebraic closure of $K(B)$ in $\Omega$ and $N_r$ (resp. $N_s$) the set of elements of $N$ which are separable (resp. p-radical) over $K(B)$. We remark that $M$ is algebraic over $K(B)$, so that $N$ is the relative algebraic closure of $M$ in $\Omega$.

$$
\begin{array}{ccccccccc}
L & \longrightarrow & L(B) & \longrightarrow & L(B \cup N_s) \\
\uparrow & & \uparrow & & \uparrow \\
K & \longrightarrow & K(B) & \longrightarrow & N_s \\
& & \downarrow & & \downarrow \\
& & M & \longrightarrow & N \\
\uparrow & & \downarrow & & \downarrow \\
N_r & \longrightarrow & N & \longrightarrow & \Omega
\end{array}
$$

Fig. 1.

Let us define the following chain of homomorphisms:

$$
L \otimes_K M \xrightarrow{\alpha} L \otimes_K N \xrightarrow{\beta} (L \otimes_K K(B)) \otimes_{K(B)} N \xrightarrow{\gamma} L(B) \otimes_{K(B)} N
$$
$$
\rightarrow L(B) \otimes_{K(B)} N_s \otimes_{K(B)} N_r \xrightarrow{\varepsilon} L(B \cup N_s) \otimes_{K(B)} N_r \xrightarrow{\zeta} \Omega .
$$

We have $\alpha = \mathrm{Id}_L \otimes u$ where $u$ is the canonical injection of $M$ into $N$, hence $\alpha$ is injective. The mapping $\beta$ is the isomorphism of commutative groups which maps $x \otimes y$ to $(x \otimes 1) \otimes y$ (II, p. 278, Prop. 2) for $x \in L$ and $y \in N$. We have $\gamma = v \otimes \mathrm{Id}_N$, where $v$ is the $K$-algebra homomorphism of $L \otimes_K K(B)$ into $L(B)$ which maps $x \otimes y$ to $xy$, for $x \in L$ and $y \in K(B)$; since $L$ and $M$ are algebraically disjoint over $K$, Prop. 14 (V, p. 114) shows that $L$ and $K(B)$ are linearly disjoint over $K$, in other words, $v$ is injective, hence $y$ is injective. Since $N$ is a quasi-Galois extension of $K(B)$, there exists (V, p. 76, Prop. 13) a $K(B)$-algebra isomorphism $w$ of $N_s \otimes_{K(B)} N_r$ onto $N$ mapping $x \otimes y$ to

1 This hypothesis is sometimes expressed by saying that $L$ is a primary extension of $K$.

xy for $x \in \mathbf{N}$, and $y \in \mathbf{N}_r$; we denote by 6 the *isomorphism* $\mathrm{Id}_{L(B)} \otimes w \ ^1$. By Th. 1 (V, p. 137) and the hypothesis on the extension L of K, every element of $L(B)$ which is algebraic and separable over $K(B)$ belongs to $K(B)$; in particular, we have $L(B) \cap N_s = K(B)$. Since $N_r$ is a Galois extension of $K(B)$, Th. 5 (V, p. 71) shows that there exists a $K(B)$-algebra isomorphism $w'$ of $L(B) \otimes_{K(B)} N_s$ onto $L(B U N_r)$ mapping $x \otimes y$ to $xy$ for $x \in L(B)$ and $y \in N_r$; we denote by $\varepsilon$ the *isomorphism* $w' \otimes \mathrm{Id}_{N_r}$. Finally, $\zeta$ is the K-algebra homomorphism mapping $x \otimes y$ to $xy$ for $x \in L(B U N_r)$ and $y \in N_r$.

What has been said shows that $\eta = \varepsilon \delta \gamma \beta \alpha$ is an injective K-algebra homomorphism of $L \otimes_K M$ into $L(B U N_r) \otimes_{K(B), N_r}$. Further, every element of M is of the form $\sum_{i=1}^n a_i b_i$ with $a_i \in \mathbf{N}$, and $b_i \in \mathbf{N}_r$ for $1 \leq i \leq n$; hence we obtain $\varphi = \zeta \eta$.

The kernel $p$ of $\varphi$ is a prime ideal of $L \otimes_K M$, hence every nilpotent element of $L \otimes_K M$ belongs to $p$, by Prop. 2 (V, p. 118). Conversely let $a$ be an element of $p$; put $\eta(a) = \sum_{r=1}^s b_i \otimes c_i$ with $b_i \in L(B U N_r)$ and $c_i \in N_r$ for $1 \leq i \leq s$. Since $N_r$ is a p-radical extension of $K(B)$, there exists an integer $f \geq 0$ such that $c_i^{p^f}$ belongs to $K(B)$ for $1 \leq i \leq s$ (where $p$ is the characteristic exponent of K). But we have

$$
\eta(a^{p^f}) = \sum_{i=1}^s b_i^{p^f} \otimes c_i^{p^f} = \left( \sum_{i=1}^s b_i^{p^f} c_i^{p^f} \right) \otimes 1 - \zeta \eta(a)^{p^f} \otimes 1 = 0
$$

and since $\eta$ is injective we finally have $a^{p^f} = 0$. We have thus shown $p$ to be the set of all nilpotent elements of $L \otimes_K M$. Now every prime ideal of $L \otimes_K M$ contains $p$ by Prop. 2 (V, p. 118).

#### Corollary {#alg-v-s17-n2-cor-1 .statement}

*Let L and M be two extensions of a field K. Suppose that the relative separable algebraic closure of K in L is equal to K. Then the set p of nilpotent elements of $L \otimes_K M$ is a prime ideal. If moreover L or M is separable over K, then $L \otimes_K M$ is an integral domain.*

We may assume that L and M are algebraically disjoint subextensions of an extension $\Omega$ of K (V, p. 116, Th. 5); then p is a prime ideal by Prop. 1 (V, p. 139). If moreover L or M is separable over K, then $L \otimes_K M$ is a reduced ring by the definition of separable extension (V, p. 119, Def. 1); so $p = 0$ and $L \otimes_K M$ is an integral domain because p was prime.

### 3. Regular algebras

#### Definition 1 {#alg-v-s17-def-1 .statement}

*Let K be a field. An algebra A over K is said to be regular if $L \otimes_K A$ is an integral domain for every extension L of K.*

A regular algebra is in particular an integral domain, hence commutative.

#### Proposition 2 {#alg-v-s17-prop-2 .statement}

— Let $A$ and $B$ be two algebras over a field $K$. If $A$ is an integral domain and $B$ is regular then $A \otimes_K B$ is an integral domain.

Let $L$ be the field of fractions of $A$. Since $B$ is a regular $K$-algebra, $L \otimes_K B$ is an integral domain, hence so is $A \otimes_K B$, since it is isomorphic to a subring of $L \otimes_K B$.

#### Proposition 3 {#alg-v-s17-prop-3 .statement}

— Let $K$ be a field.
a) Every subalgebra of a regular $K$-algebra is itself regular.
b) The tensor product of two regular $K$-algebras is again regular.
c) Let $A$ be a $K$-algebra and $K'$ an extension of $K$. For $A$ to be regular it is necessary and sufficient that the $K'$-algebra $A_{(K')}$ derived from $A$ by extension of scalars should be regular.

The proof of a) (resp. c)) is identical to that of part a) (resp. d)) of Prop. 3, V, p. 119, after replacing everywhere « reduced ring » by « integral domain » and « separable algebra » by « regular algebra ». Let us prove b).

Let $A$ and $B$ be two regular $K$-algebras. Let $L$ be an extension of $K$. Since $A$ is regular, the ring $L \otimes_K A$ is an integral domain. By Prop. 2, the ring $(L \otimes_K A) \otimes_K B$ is an integral domain, because $B$ is regular. Finally, the ring $L \otimes_K (A \otimes_K B)$ is isomorphic to $(L \otimes_K A) \otimes_K B$, and hence is an integral domain. This shows $A \otimes_K B$ to be a regular $K$-algebra.

### 4. Regular extensions

#### Definition 2 {#alg-v-s17-def-2 .statement}

— An extension of a field $K$ is said to be regular if it is regular as $K$-algebra.

#### Proposition 4 {#alg-v-s17-prop-4 .statement}

— Let $A$ be an algebra over field $K$ which is an integral domain, and $E$ its field of fractions. Let $L$ be an extension of $K$; if the ring $L \otimes_K A$ is an integral domain the same is true of $L \otimes_K E$.

If $L \otimes_K A$ is an integral domain, it may be embedded in its field of fractions $F$. Write $u(x) = x \otimes 1$ for $x \in L$ and denote by $v$ the $K$-homomorphism of $E$ into $F$ which extends the injective homomorphism $y \mapsto 1 \otimes y$ of $A$ into $F$. By Prop. 6 (V, p. 14) the subfields $u(L)$ and $v(E)$ of $F$ are linearly disjoint over $K$; therefore the homomorphism $u * v$ of $L \otimes_K E$ into $F$ (V, p. 12) is injective. This shows $L \otimes_K E$ to be an integral domain.

#### Corollary {#alg-v-s17-n4-cor-1 .statement}

— For $A$ to be a regular $K$-algebra it is necessary and sufficient that its field of fractions should be a regular extension of $K$.

The condition is necessary by Prop. 4 and sufficient by Prop. 3, a).

#### Proposition 5 {#alg-v-s17-prop-5 .statement}

— Every pure extension of a field $K$ is regular.

By the preceding corollary it is enough to prove that every polynomial algebra $A = K[X_i]_i$, is a regular $K$-algebra. Let $L$ be an extension of $K$; the ring $L \otimes_K A$ is isomorphic to $L[X_i]_{i \in I}$ (III, p. 449, Remark 2), and hence an integral domain (IV, p. 9, Prop. 8).

#### Proposition 6 {#alg-v-s17-prop-6 .statement}

— Let L be an extension of a field K. If L is regular, then every subextension of L is regular. Conversely, if every finitely generated subextension of L is regular, then L is regular.

The first assertion follows from Prop. 3, a).

Let M be an extension of K and let $\mathcal{U}$ be the set of all finitely generated subextensions of L. For each E $\in \mathcal{U}$, the ring $M \otimes_K E$ may be identified with a subring of $M \otimes_K L$ and we thus have an increasing directed family of subrings of $M \otimes_K L$ whose union is $M \otimes_K L$. Now the second assertion follows immediately.

#### Proposition 7 {#alg-v-s17-prop-7 .statement}

— Let L be an extension of a field K and M an L-algebra (for example, an extension of L). If L is regular over K and M is a regular L-algebra, then M is regular as K-algebra.

Let E be an extension of K; since L is regular over K, $E \otimes_K L$ is an integral domain. By Prop. 2 (V, p. 141) the ring $(E \otimes_K L) \otimes_L M$ is thus an integral domain and the same is true of the ring $E \otimes_K M$ isomorphic to it (II. p. 278, Prop. 2). Hence the result.

#### Proposition 8 {#alg-v-s17-prop-8 .statement}

— Let L and M be two extensions of a field K.

a) If M is regular over K, then the field of fractions of the integral domain $L \otimes_K M$ is a regular extension of L.

b) If L and M are regular extensions of K, the same is true of the field of fractions of $L \otimes_K M$.

Assertion a) follows from Prop. 3, c) (V, p. 141) and the Cor. of V, p. 141; Assertion b) follows from Prop. 3, b) (V, p. 141) and the Cor. of V, p. 141.

### 5. Characterization of regular extensions

#### Proposition 9 {#alg-v-s17-prop-9 .statement}

— Let K be a field, $\overline{K}$ an algebraic closure of K and L an extension of K. Then the following conditions are equivalent:

a) L is separable over K and K is relatively algebraically closed in L.

b) L is a regular extension of K.

c) The ring $\overline{K} \otimes_K L$ is an integral domain.

d) Let $\overline{L}$ be an algebraic closure of L. Then L is linearly disjoint over K from the relative algebraic closure of K in $\overline{L}$.

Moreover, when these conditions hold, then $\overline{K} \otimes_K L$ is a field.

a) $\Rightarrow$ b): Let M be an extension of K. Under the hypotheses of a), the ring $M \otimes_K L$ is an integral domain, by V, p. 140, Cor.

b) $\Rightarrow$ c): This follows from Def. 2.

c) $\Rightarrow$ d): With the notation of d) we can identify $\overline{K}$ with the relative algebraic closure of K in $\overline{L}$ (V, p. 22, Ex. 2). Suppose that the ring $A = \overline{K} \otimes_K L$ is an integral domain. Let E be a subextension of K of finite degree over K; the subring

E $\otimes_K$ L of A is an integral domain and hence is an algebra of finite degree over L; by the Cor. of V, p. 10 it is a field. Since $\bar{K}$ is the union the increasing directed set of extensions E of the above type, A is a field (V, p. 11, Prop. 3). The canonical homomorphism of A into $\bar{L}$ mapping $x \otimes y$ to $xy$ (for $x \in \bar{K}$ and $y \in L$) is therefore injective, so L and $\bar{K}$ are linearly disjoint over K.

$d) \Rightarrow a)$: Under the hypotheses of d) we have $L \cap \bar{K} = K$, so K is relatively algebraically closed in L; further if p is the characteristic exponent of K, the field $L$ is linearly disjoint from $K^{p^{-\infty}}$ over $K$, hence L is separable over K (V, p. 123, Cor. 1).

#### Corollary 1 {#alg-v-s17-prop-9-cor-1 .statement}

— Let A be an algebra over a field K. For A to be a regular K-algebra it is necessary and sufficient for the ring $\bar{K} \otimes_K A$ to be an integral domain.

The stated condition is clearly necessary. Conversely, assume that $\bar{K} \otimes_K A$ is an integral domain and denote by E the field of fractions of A. By Prop. 4 (V, p. 141) the ring $\bar{K} \otimes_K E$ is an integral domain, hence E is a regular extension of K, by Prop. 9; by V, p. 141, Cor., we conclude that A is regular as K-algebra.

#### Corollary 2 {#alg-v-s17-prop-9-cor-2 .statement}

— Let K be an algebraically closed field. Every K-algebra which is an integral domain is a regular K-algebra. In particular, every extension of K is regular.

This follows from Cor. 1.

#### Corollary 3 {#alg-v-s17-prop-9-cor-3 .statement}

— Let K be an algebraically closed field. If A and B are two K-algebras which are integral domains, then the same is true of $A \otimes_K B$.

By Cor. 2, A and B are regular K-algebras, and it suffices to apply Prop. 2 (V, p. 141).

### 6. Application to composite extensions

#### Proposition 10 {#alg-v-s17-prop-10 .statement}

— Let L and M be two extensions of a field K and $(E, u, v)$ a composite extension of L and M (V, p. 12). Suppose that the ring $L \otimes_K M$ is an integral domain and that the subextensions $u(L)$ and $v(M)$ of E are algebraically disjoint over K. Then $u(L)$ and $v(M)$ are linearly disjoint over K.

Put $w = u * v$ (V, p. 12), denote by F the field of fractions of the integral domain $L \otimes_K M$ and identify L (resp. M) with a subfield of F by means of the mapping $x \mapsto x \otimes 1$ (resp. $y \mapsto 1 \otimes y$); then the restriction of w to L (resp. M) is u (resp. v). Let B be a transcendence basis of M over K (V, p. 109, Th. 1).

By hypothesis $u(L)$ and $v(M)$ are algebraically disjoint over K; therefore (V, p. 114, Prop. 14), $u(L)$ and $v(K(B))$ are linearly disjoint over K. Thus there exists a K-homomorphism $u': L(B) \to E$ which agrees with u on L and with v ou K(B). By construction L and M are linearly disjoint over K in F; by Prop. 8 (V, p. 15) the subfields $L(B)$ and $M$ of F are linearly disjoint over $K(B)$. It follows that there exists a K-homomorphism $w' : M[L(B)] \to E$ which agrees with $u'$ on $L(B)$ and with $v$ on $M$. But the field $F$ is generated by $M \cup L(B)$ and $M$ is algebraic over $K(B)$; we thus have $M[L(B)] = F$ (V, p. 18, Cor. 2). Hence we conclude that $w'$ is a K-isomorphism of $F$ onto $E$ whose restriction to $L$ (resp. $M$) is $u$ (resp. $v$). This shows $u(L)$ and $v(M)$ to be linearly disjoint over $K$.

#### Corollary 1 {#alg-v-s17-prop-10-cor-1 .statement}

*Let $\Omega$ be an extension of a field $K$ and $L$ a subextension of $\Omega$ which is regular over $K$. Every subextension $M$ of $\Omega$ which is algebraically disjoint from $L$ over $K$ is linearly disjoint.*

The ring $L \otimes_K M$ is an integral domain by definition of regular extension and it suffices now to apply Prop. 10.

#### Corollary 2 {#alg-v-s17-prop-10-cor-2 .statement}

*Let $\Omega$ be an extension of a field $K$ and $L, M$ two subextensions of $\Omega$. Suppose that $L$ is separable over $K$ and that the relative separable closure of $K$ in $M$ is equal to $K$. If $L$ and $M$ are algebraically disjoint over $K$, then they are linearly disjoint over $K$.*

By Prop. 10 it is enough to remark that the ring $L \otimes_K M$ is an integral domain (V, p. 140, Cor.).

Exercises

### Exercises {#alg-v-s17-exercises}

See the [exercises for § 17](exercises/s17/).
