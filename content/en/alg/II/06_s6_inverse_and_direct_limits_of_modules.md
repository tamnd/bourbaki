---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 6
section_title: Inverse and direct limits of modules
lang: en
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 284-291, 399-400
pdf_pages: 0308-0315, 0423-0424
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE LIMITS OF MODULES
      page: 284
      pdf_page: 308
    - "no": 2
      title: DIRECT LIMITS OF MODULES
      page: 286
      pdf_page: 310
    - "no": 3
      title: TENSOR PRODUCT OF DIRECT LIMITS
      page: 289
      pdf_page: 313
statements: 17
exercises: 4
content_sha256: 0071494e46f0d6a4a97c19ea9a8d779c617f3943739c71f4a78db61ff9daaa81
---

## § 6. INVERSE AND DIRECT LIMITS OF MODULES

Throughout this paragraph, I will denote a non-empty preordered set and $\alpha \leq \beta$ the preorder relation on I. Unless otherwise mentioned, the inverse and direct systems have indexing set I.

### 1. INVERSE LIMITS OF MODULES

Let $(A_\alpha, \phi_{\alpha \beta})$ be an inverse system of rings (I, § 10, no. 1), $(E_\alpha, f_{\alpha \beta})$ an inverse system of commutative groups (written additively) (I, § 10, no. 1) and suppose that each $E_\alpha$ has a left $A_\alpha$-module structure; moreover suppose that for $\alpha \leq \beta$ $(f_{\alpha \beta}, \phi_{\alpha \beta})$ is a dimorphism of $E_\beta$ into $E_\alpha$ (§ 1, no. 13), in other words that
$$
f_{\alpha \beta}(\lambda_\beta x_\beta) = \phi_{\alpha \beta}(\lambda_\beta) f_{\alpha \beta}(x_\beta),
$$
for $x_\beta \in E_\beta$, $\lambda_\beta \in A_\beta$; then it follows from I, § 10, no. 2 that $E = \lim \leftarrow E_\alpha$ has a left module structure over $A = \lim \leftarrow A_\alpha$. For all $\alpha \in I$, let $f : E \to E_\alpha$, $\phi_\alpha : A \to A_\alpha$ be the canonical mappings; then $(f_\alpha, \phi_\alpha)$ is a dimorphism of E into $E_\alpha$. We shall say that $(E_\alpha, f_{\alpha\beta})$ is an *inverse system of left $A_\alpha$-modules* and that the $A$-module $E$ is its *inverse limit*.

Let $(E'_\alpha, f'_{\alpha\beta})$ be another inverse system of left $A_\alpha$-modules and, for all $\alpha$, let $u_\alpha : E'_\alpha \to E_\alpha$ be an *$A_\alpha$-linear* mapping, these mappings forming an *inverse system*; then $u = \lim u_\alpha$ is an *$A$-linear* mapping of $\lim E'_\alpha$ into $\lim E_\alpha$.

Moreover:

#### Proposition 1 {#alg-ii-s6-prop-1 .statement}

*Let* $(E_\alpha, f_{\alpha\beta}),\ (E'_\alpha, f'_{\alpha\beta}),\ (E''_\alpha, f''_{\alpha\beta})$ *be three inverse systems of $A_\alpha$-modules and* $(u_\alpha),\ (v_\alpha)$ *two inverse systems of $A_\alpha$-linear mappings such that the sequences*

$$
0 \longrightarrow E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha
$$

*are exact for all $\alpha$.* *Then, writing* $u = \lim u_\alpha,\ v = \lim v_\alpha$, *the sequence*

$$
0 \longrightarrow \lim E'_\alpha \xrightarrow{u} \lim E_\alpha \xrightarrow{v} \lim E''_\alpha
$$

*is exact*.

*As* $u_\alpha^{-1}(0) = \{0\}$ *for all $\alpha$, it follows from Set Theory, III, § 7, no. 2, Proposition 2 that* $u^{-1}(0) = \{0\}$, *hence* $u$ *is injective; further, the* $u_\alpha(E'_\alpha)$ *form an inverse system of subsets of the* $E_\alpha$ *and thus* $u(\lim E'_\alpha) = \lim u_\alpha(E'_\alpha)$. *As* $u_\alpha(E'_\alpha) = v_\alpha^{-1}(0)$ *by hypothesis,* $v^{-1}(0) = \lim u_\alpha(E'_\alpha) = u(\lim E'_\alpha)$ (*Set Theory*, III, § 7, no. 2, Proposition 2), *which completes the proof*.

#### Remark {#alg-ii-s6-n1-rem-1 .statement}

(1) Proposition 1 and its proof are valid for arbitrary *groups*, except for change of notation.

(2) Note that if there are exact sequences

$$
0 \longrightarrow E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha \longrightarrow 0
$$

*it does not necessarily follow* that the sequence

$$
0 \longrightarrow \lim E'_\alpha \xrightarrow{u} \lim E_\alpha \xrightarrow{v} \lim E''_\alpha \longrightarrow 0
$$

*is exact; in other words, the inverse limit of an inverse system of surjective linear mappings is not necessarily surjective* (cf. Exercise 1).

Suppose now that the $A_\alpha$ are equal to the *same ring* $A$ and the $\phi_{\alpha\beta}$ to $1_A$; then for every inverse system $(E_\alpha, f_{\alpha\beta})$ of $A$-modules, $E = \lim E_\alpha$ is an $A$-module. Let $F$ be an $A$-module and, for all $\alpha$, let $u_\alpha : F \to E_\alpha$ be an $A$-linear mapping such that $(u_\alpha)$ is an inverse system of mappings; then $u = \lim u_\alpha$ is an $A$-linear mapping of $F$ into $\lim E_\alpha$. *Conversely*, for every $A$-linear mapping $v : F \to \lim E_\alpha$, the family of $v_\alpha = f_\alpha \circ v$ is an inverse system of $A$-linear mappings such that $v = \lim_{\leftarrow} v_\alpha$. We note on the other hand that for $\alpha \leq \beta$ the mapping

$$
\operatorname{Hom}(1_F, f_{\alpha \beta}) = \bar{f}_{\alpha \beta}: \operatorname{Hom}_A(F, E_\beta) \to \operatorname{Hom}_A(F, E_\alpha)
$$

is a $\mathbf{Z}$-module homomorphism such that $(\operatorname{Hom}_A(F, E_\alpha), \bar{f}_{\alpha \beta})$ is an *inverse system of $\mathbf{Z}$-modules*; as $\bar{f}_{\alpha \beta}(v_\beta) = f_{\alpha \beta} \circ v_\beta$, the above remarks can therefore be expressed as follows:

#### Proposition 2 {#alg-ii-s6-prop-2 .statement}

*For every inverse system* $(E_\alpha, f_{\alpha \beta})$ *of $A$*-modules *and every $A$*-module $F$, *the canonical mapping* $u \mapsto (f_\alpha \circ u)$ *is a $\mathbf{Z}$*-module *isomorphism*

(2)

$$
l_F: \operatorname{Hom}_A(F, \lim_{\leftarrow} E_\alpha) \to \lim_{\leftarrow} \operatorname{Hom}_A(F, E_\alpha).
$$

#### Corollary {#alg-ii-s6-n1-cor-1 .statement}

*For every $A$*-module homomorphism $v: F \to F'$, the*

$$
\bar{v}_\alpha = \operatorname{Hom}(v, 1_{E_\alpha}): \operatorname{Hom}(F', E_\alpha) \to \operatorname{Hom}(F, E_\alpha)
$$

*form an inverse system of $\mathbf{Z}$*-linear mappings *and the diagram*

(3)

$$
\begin{array}{ccc}
\operatorname{Hom}(F', \lim_{\leftarrow} E_\alpha) & \xrightarrow{l_{F'}} & \lim_{\leftarrow} \operatorname{Hom}(F', E_\alpha) \\
\downarrow \operatorname{Hom}(v, 1_E) & & \downarrow \lim_{\leftarrow} \bar{v}_\alpha \\
\operatorname{Hom}(F, \lim_{\leftarrow} E_\alpha) & \xrightarrow{l_F} & \lim_{\leftarrow} \operatorname{Hom}(F, E_\alpha)
\end{array}
$$

*is commutative*.

For all $u \in \operatorname{Hom}(F', \lim_{\leftarrow} E_\alpha)$, $l_F(u \circ v) = (f_\alpha \circ u \circ v)$ by definition and the commutativity of diagram (3) follows immediately from the definitions.

### 2. DIRECT LIMITS OF MODULES

*Henceforth I is assumed to be right directed.*

Let $(A_\alpha, \phi_{\beta \alpha})$ be a direct system of rings (I, § 10, no. 3), $(E_\alpha, f_{\beta \alpha})$ a direct system of commutative groups (written additively) (I, § 10, no. 3) and suppose that each $E_\alpha$ has a *left $A_\alpha$*-module structure; further, suppose that, for $\alpha \leq \beta$, $(f_{\beta \alpha}, \phi_{\beta \alpha})$ is a *dimorphism* of $E_\alpha$ into $E_\beta$ (§ 1, no. 13), in other words that

(4)

$$
f_{\beta \alpha}(\lambda_\alpha x_\alpha) = \phi_{\beta \alpha}(\lambda_\alpha) f_{\beta \alpha}(x_\alpha)
$$

for $x_\alpha \in E_\alpha, \lambda_\alpha \in A_\alpha$; then $E = \lim_{\longrightarrow} E_\alpha$ has a *left module* structure over $A = \lim_{\longrightarrow} A_\alpha$ (I, § 10, no. 4). For all $\alpha \in I$, let $f_\alpha: E_\alpha \to E, \phi_\alpha: A_\alpha \to A$ be the canonical mappings; then $(f_\alpha, \phi_\alpha)$ is a *dimorphism* of $E_\alpha$ into $E$. We shall say that $(E_\alpha, f_{\beta \alpha})$ is a *direct system of left $A_\alpha$*-modules and that the $A$*-module $E$ is its *direct limit*.

Let $(E'_\alpha, f'_{\beta \alpha})$ be another direct system of left $A_\alpha$*-modules and, for all $\alpha$, let $u_\alpha : E'_\alpha \to E_\alpha$ be an $A_\alpha$-linear mapping, these mappings forming a direct system; then $u = \lim \to u_\alpha$ is an $A$-linear mapping of $\lim \to E'_\alpha$ into $\lim \to E_\alpha$.

Moreover:

#### Proposition 3 {#alg-ii-s6-prop-3 .statement}

*Let* $(E_\alpha, f_{\beta \alpha}), (E'_\alpha, f'_{\beta \alpha}), (E''_\alpha, f''_{\beta \alpha})$ *be three direct systems of* $A_\alpha$*-modules and* $(u_\alpha), (v_\alpha)$ *two direct systems of* $A_\alpha$*-linear mappings such that the sequences*

$$
E'_\alpha \xrightarrow{u_\alpha} E_\alpha \xrightarrow{v_\alpha} E''_\alpha
$$

*are exact for all* $\alpha$. *Then, writing* $u = \lim \to u_\alpha, v = \lim \to v_\alpha$, *the sequence*

$$
\lim \to E'_\alpha \xrightarrow{u} \lim \to E_\alpha \xrightarrow{v} \lim \to E''_\alpha
$$

*is exact.*

$u(\lim \to E'_\alpha) = \lim \to u_\alpha(E'_\alpha)$ *and* $v^{-1}(0) = \lim \to v_\alpha^{-1}(0)$ *(Set Theory, III, § 7, no. 6, Corollary to Proposition 7).*

Loosely speaking, Proposition 3 can also be expressed by saying that *passing to the direct limit preserves exactness*.

#### Proposition 4 {#alg-ii-s6-prop-4 .statement}

*Let* $(E_\alpha, f_{\beta \alpha})$ *be a direct system of* $A_\alpha$*-modules, $E = \lim \to E_\alpha$ *its direct limit and* $\phi_\alpha : A_\alpha \to A$ *and* $f_\alpha : E_\alpha \to E$ *the canonical mappings for all* $\alpha \in I$. *If, for all* $\alpha \in I$, $S_\alpha$ *is a generating system of* $E_\alpha$, *then* $S = \bigcup_{\alpha \in I} f_\alpha(S_\alpha)$ *is a generating system of* $E$.

Every $x \in E$ *is of the form* $f_\alpha(x_\alpha)$ *for some* $\alpha \in I$ *and some* $x_\alpha \in E_\alpha$ *and by hypothesis* $x = \sum_i \lambda^{(i)}_\alpha y^{(i)}_\alpha$, *where* $\lambda^{(i)}_\alpha \in A_\alpha$ *and* $y^{(i)}_\alpha \in S_\alpha$; *writing* $\lambda^{(i)} = \phi_\alpha(\lambda^{(i)}_\alpha)$, $y^{(i)} = f_\alpha(y^{(i)}_\alpha)$, *we obtain* $x = \sum_i \lambda^{(i)} y^{(i)}$.

#### Proposition 5 {#alg-ii-s6-prop-5 .statement}

*With the hypotheses and notation of Proposition 4, suppose that for all* $\alpha \in I$, $E_\alpha$ *is the direct sum of a family* $(M^\lambda_\alpha)_{\alpha \in L}$ *of submodules (the indexing set* $L$ *being independent of* $\alpha$) *and that* $f_{\beta \alpha}(M^\lambda_\alpha) \subset M^\lambda_\alpha$ *for* $\alpha \leq \beta$ *and for all* $\lambda \in L$. *Then* $E$ *is the direct sum of the submodules* $M^\lambda = \lim \to M^\lambda_\alpha$ $(\lambda \in L)$.

It follows from Proposition 4 that $E$ is the sum of the $M^\lambda$. Let $(y^\lambda)_{\lambda \in L}$ *be a family such that* $y^\lambda \in M^\lambda$ *for all* $\lambda \in L$ *and whose support is finite and suppose that* $\sum_\lambda y^\lambda = 0$. *By virtue of Set Theory, III, § 7, no. 5, Lemma 1, there exist an* $\alpha \in I$ *and a family* $(x^\lambda_\alpha)_{\alpha \in L}$ *of finite support consisting of elements of* $E_\alpha$ *such that* $x^\lambda_\alpha \in M^\lambda_\alpha$ *and* $y^\lambda = f_\alpha(x^\lambda_\alpha)$ *for all* $\lambda \in L$. *The relation* $f_\alpha \left( \sum_{\lambda \in L} x^\lambda_\alpha \right) = 0$ *implies the existence of a* $\beta \geq \alpha$ *such that* $f_{\beta \alpha} \left( \sum_{\lambda \in L} x^\lambda_\alpha \right) = 0$ *(Set Theory, III, § 7, no. 5, Lemma 1), which may be written as $\sum_{\lambda \in L} x_\beta^\lambda = 0$, where $x_\beta^\lambda = f_{\beta \alpha}(x_\alpha^\lambda) \in M_\beta^\lambda$ by hypothesis; hence $x_\beta^\lambda = 0$ for all $\lambda \in L$ and therefore $y^\lambda = f_\beta(x_\beta^\lambda) = 0$ for all $\lambda \in L$, which proves that the sum of the $M^\lambda$ is direct.

#### Corollary {#alg-ii-s6-n2-cor-1 .statement}

*Let* $(P_\alpha)$ *be a direct system of subsets of* $E_\alpha$ *and let* $P = \lim \overrightarrow{P_\alpha}$. *If, for all* $\alpha \in I$, $P_\alpha$ *is a free subset (resp. basis) of* $E_\alpha$, *then* $P$ *is a free subset (resp. basis) of* $E$.

The second assertion follows immediately from the first and Proposition 4. It is therefore sufficient to prove that if the $P_\alpha$ are free every subset $\{ y^{(i)} \}_{1 \leq i \leq n}$ consisting of distinct elements of $P$, is free. There exists an $\alpha \in I$ and elements $x_\alpha^{(i)} \in P_\alpha$ such that $y^{(i)} = f_\alpha(x_\alpha^{(i)})$ for $1 \leq i \leq n$ (*Set Theory*, III, § 7, no. 5, Lemma 1); if $\sum_i \lambda^{(i)} y^{(i)} = 0$, it may be assumed that $\lambda^{(i)} = \phi_\alpha(\lambda_\alpha^{(i)})$ for $1 \leq i \leq n$ and hence $f_\alpha \left( \sum_i \lambda_\beta^{(i)} x_\beta^{(i)} \right) = 0$; this implies $\sum_i \lambda_\beta^{(i)} x_\beta^{(i)} = 0$ for some $\beta \geq \alpha$, where $\lambda_\beta^{(i)} = \phi_{\beta \alpha}(\lambda_\alpha^{(i)})$, $x_\beta^{(i)} = f_{\beta \alpha}(x_\alpha^{(i)})$ and the $x_\beta^{(i)}$ belong to $P_\beta$ and are distinct since $y^{(i)} = f_\beta(x_\beta^{(i)})$; then $\lambda_\beta^{(i)} = 0$ for $1 \leq i \leq n$, whence
$$
\lambda^{(i)} = \phi_\beta(\lambda_\beta^{(i)}) = 0
$$
for $1 \leq i \leq n$.

Suppose now that all the rings $A_\alpha$ are equal to the *same ring* $A$ and the $\phi_{\beta \alpha}$ to $1_A$; then, for every direct system $(E_\alpha, f_{\beta \alpha})$ of $A$-modules, $E = \lim \overrightarrow{E_\alpha}$ is an $A$-module. Let $F$ be an $A$-module and for all $\alpha$ let $u_\alpha : E_\alpha \to F$ be an $A$-linear mapping such that $(u_\alpha)$ is a direct system of mappings; then $u = \lim \overrightarrow{u_\alpha}$ is an $A$-linear mapping of $E$ into $F$. *Conversely*, for every $A$-linear mapping $v : \lim \overrightarrow{E_\alpha} \to F$, the family of $v_\alpha = v \circ f_\alpha$ is a direct system of $A$-linear mappings such that $v = \lim \overrightarrow{v_\alpha}$. On the other hand we note that for $\alpha \leq \beta$ the mapping
$$
\operatorname{Hom}(f_{\beta \alpha}, 1_F) = \bar{f}_{\alpha \beta} : \operatorname{Hom}_A(E_\beta, F) \to \operatorname{Hom}_A(E_\alpha, F)
$$
is a $\mathbf{Z}$-module homomorphism such that $(\operatorname{Hom}_A(E_\alpha, F), \bar{f}_{\alpha \beta})$ is an *inverse system of* $\mathbf{Z}$*-modules*; as $\bar{f}_{\alpha \beta}(v_\beta) = v_\beta \circ f_{\beta \alpha}$, the above remarks can be expressed as follows:

#### Proposition 6 {#alg-ii-s6-prop-6 .statement}

*For every direct system* $(E_\alpha, f_{\beta \alpha})$ *of* $A$*-modules and every* $A$*-module* $F$, *the canonical mapping* $u \mapsto (u \circ f_\alpha)$ *is a* $\mathbf{Z}$*-module isomorphism*
$$
d_F : \operatorname{Hom}_A(\lim \overrightarrow{E_\alpha}, F) \to \lim \leftarrow \operatorname{Hom}_A(E_\alpha, F).
$$

#### Corollary 1 {#alg-ii-s6-prop-6-cor-1 .statement}

*For every* $A$*-module homomorphism* $v : F \to F'$, *the*
$$
\bar{v}_\alpha = \operatorname{Hom}(1_{E_\alpha}, v) : \operatorname{Hom}(E_\alpha, F) \to \operatorname{Hom}(E_\alpha, F')
$$

form an inverse system of $\mathbf{Z}$-linear mappings and the diagram

$$
\begin{array}{ccc}
\operatorname{Hom}(\lim E_\alpha, F) & \xrightarrow{d_F} & \lim \operatorname{Hom}(E_\alpha, F) \\
\downarrow \operatorname{Hom}(1_E, v) & & \downarrow \lim \overline{v}_\alpha \\
\operatorname{Hom}(\lim E_\alpha, F') & \xrightarrow{d_{F'}} & \lim \operatorname{Hom}(E_\alpha, F')
\end{array}
$$

is commutative.

For all $u \in \operatorname{Hom}(\lim E_\alpha, F)$, $d_{F'}(v \circ u) = (v \circ u \circ f_\alpha)$ by definition and the commutativity of diagram (6) then follows immediately from the definitions.

#### Corollary 2 {#alg-ii-s6-prop-6-cor-2 .statement}

*If* $(E_\alpha, f_{\beta \alpha})$ *is a direct system of left* $A$*-modules and* $E = \lim \longrightarrow E_\alpha$, $(E_\alpha^*, t f_{\beta \alpha})$ *is an inverse system of right* $A$*-modules and* $\lim \leftarrow E_\alpha^*$ *is canonically isomorphic to* $E^*$.

#### Remark {#alg-ii-s6-n2-rem-1 .statement}

Let $E$ be an $A$*-module and* $(M_\alpha)_{\alpha \in I}$ *an increasing family of submodules of* $E$ *such that* $E$ *is the union of the* $M_\alpha$; if $j_{\beta \alpha}: M_\alpha \to M_\beta$ (for $\alpha \leq \beta$) and $j_\alpha: M_\alpha \to E$ *are the canonical injections, it is immediate that* $j = \lim \longrightarrow j_\alpha$ *is an isomorphism of* $\lim \longrightarrow M_\alpha$ *onto* $E$ *(Set Theory, III, § 7, no. 6, Remark 1)*. In particular, every $A$*-module is the direct limit of the right directed family of its *finitely generated* submodules.

### 3. TENSOR PRODUCT OF DIRECT LIMITS

Let $(A_\alpha, \rho_{\beta \alpha})$ be a direct system of rings and $(E_\alpha, f_{\beta \alpha})$ (resp. $(F_\alpha, g_{\beta \alpha})$) be a direct system of right (resp. left) $A_\alpha$*-modules. For $\alpha \leq \beta$, there is a $\mathbf{Z}$*-module homomorphism*

$$
f_{\beta \alpha} \otimes g_{\beta \alpha}: E_\alpha \otimes_{A_\alpha} F_\alpha \to (E_\beta)_{[A_\alpha]} \otimes_{A_\alpha} (F_\beta)_{[A_\alpha]}
$$

and on the other hand there is a canonical $\mathbf{Z}$*-module homomorphism*

$$
(E_\beta)_{[A_\alpha]} \otimes_{A_\alpha} (F_\beta)_{[A_\alpha]} \to E_\beta \otimes_{A_\beta} F_\beta
$$

corresponding to the ring homomorphism $\rho_{\beta \alpha}$ ($§ 3$, no. 3, Proposition 2); whence by composition we obtain a $\mathbf{Z}$*-module homomorphism*

$$
h_{\beta \alpha}: E_\alpha \otimes_{A_\alpha} F_\alpha \to E_\beta \otimes_{A_\beta} F_\beta
$$

which maps the tensor product $x_\alpha \otimes y_\alpha$ to $f_{\beta \alpha}(x_\alpha) \otimes g_{\beta \alpha}(y_\alpha)$. Clearly

$$
(E_\alpha \otimes_{A_\alpha} F_\alpha, h_{\beta \alpha})
$$

is a *direct system* of $\mathbf{Z}$*-modules. Let* $A = \lim \longrightarrow A_\alpha$, $E = \lim \longrightarrow E_\alpha$, $F = \lim \longrightarrow F_\alpha$ *and*

let $\rho_\alpha : A_\alpha \to A, f_\alpha : E_\alpha \to E, g_\alpha : F_\alpha \to F$ be the canonical mappings. As above, a $\mathbf{Z}$-linear mapping $\pi_\alpha : E_\alpha \otimes_{A_\alpha} F_\alpha \to E \otimes_A F$ is defined, which maps the tensor product $x_\alpha \otimes y_\alpha$ to $f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)$, and it is immediate that these mappings form a direct system. Thus we obtain a $\mathbf{Z}$-linear mapping
$$
\pi = \lim \pi_\alpha : \lim (E_\alpha \otimes_{A_\alpha} F_\alpha) \to E \otimes_A F.
$$

#### Proposition 7 {#alg-ii-s6-prop-7 .statement}

*The $\mathbf{Z}$-linear mapping (7) is bijective.*

We set $P = \lim (E_\alpha \otimes_{A_\alpha} F_\alpha)$ and, for all $\alpha \in I$, let $h_\alpha : E_\alpha \otimes_{A_\alpha} F_\alpha \to P$ be the canonical mapping. On the other hand, for all $\alpha \in I$, let
$$
t_\alpha : E_\alpha \times F_\alpha \to E_\alpha \otimes_{A_\alpha} F_\alpha
$$
be the canonical $\mathbf{Z}$-bilinear mapping; for $\alpha \leq \beta$,
$$
t_\beta(f_{\beta \alpha}(x_\alpha), g_{\beta \alpha}(y_\alpha)) = f_{\beta \alpha}(x_\alpha) \otimes g_{\beta \alpha}(y_\alpha) = h_{\beta \alpha}(t_\alpha(x_\alpha, y_\alpha))
$$
and hence $(t_\alpha)$ is a direct system of mappings. Canonically identifying $\lim (E_\alpha \times F_\alpha)$ with $E \times F$ (*Set Theory*, III, § 7, no. 7, Proposition 10), we derive a mapping $t = \lim t_\alpha : E \times F \to P$ such that
$$
t(f_\alpha(x_\alpha), g_\alpha(y_\alpha)) = h_\alpha(t_\alpha(x_\alpha, y_\alpha)) = h_\alpha(x_\alpha \otimes y_\alpha).
$$
Taking account of *Set Theory*, III, § 7, no. 5, Lemma 1, it is immediately seen that $t$ is $\mathbf{Z}$-bilinear; moreover, for $x \in E, y \in F, \lambda \in A$, there exists $\alpha \in I$ such that $x = f_\alpha(x_\alpha), y = g_\alpha(y_\alpha), \lambda = \rho_\alpha(\lambda_\alpha)$ with $\lambda_\alpha \in A_\alpha, x_\alpha \in E_\alpha, y_\alpha \in F_\alpha$ (*Set Theory*, III, § 3, no. 7, Lemma 1); whence
$$
t(x \lambda, y) = h_\alpha((x_\alpha \lambda_\alpha) \otimes y_\alpha) = h_\alpha(x_\alpha \otimes (\lambda_\alpha y_\alpha)) = t(x, \lambda y).
$$
Hence there exists one and only one $\mathbf{Z}$-linear mapping $\pi' : E \otimes_A F \to P$ such that $\pi'(x \otimes y) = t(x, y)$ (§ 3, no. 1, Proposition 1). Moreover, by definition
$$
\pi'(\pi(h_\alpha(x_\alpha \otimes y_\alpha))) = \pi'(f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)) = h_\alpha(x_\alpha \otimes y_\alpha)
$$
$$
\pi(\pi'(f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha))) = \pi(h_\alpha(x_\alpha \otimes y_\alpha)) = f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)
$$
and as the elements of the form $f_\alpha(x_\alpha) \otimes g_\alpha(y_\alpha)$ (resp. $h_\alpha(x_\alpha \otimes y_\alpha)$) generate the $\mathbf{Z}$-module $E \otimes_A F$ (resp. $P$), $\pi' \circ \pi$ and $\pi \circ \pi'$ are the identity mappings.

Loosely speaking, Proposition 7 may be expressed by saying that *tensor products commute with direct limits* and usually the two sides of (7) are identified by means of the isomorphism $\pi$.

#### Corollary 1 {#alg-ii-s6-prop-7-cor-1 .statement}

*Let* $(E'_\alpha, f'_{\beta \alpha})$ (resp. $(F'_\alpha, g'_{\alpha \beta})$) *be another direct system of right* (resp. *left*) *$A_\alpha$*-*modules; for all* $\alpha \in I$, *let* $u_\alpha : E_\alpha \to E'_\alpha$ (resp. $v_\alpha : F_\alpha \to F'_\alpha$) *be an* $A_\alpha$-linear mapping such that $(u_\alpha)$ (resp. $(v_\alpha)$) is a direct system. Then $(u_\alpha \oplus v_\alpha)$ is a direct system of $\mathbf{Z}$-linear mappings and the diagram

$$
\begin{array}{ccc}
\lim(E_\alpha \otimes_{A_\alpha} F_\alpha) & \longrightarrow & (\lim E_\alpha) \otimes_A (\lim F_\alpha) \\
\downarrow & & \downarrow \\
\lim(u_\alpha \otimes v_\alpha) & & (\lim u_\alpha) \otimes (\lim v_\alpha) \\
\lim(E'_\alpha \otimes_{A_\alpha} F'_\alpha) & \longrightarrow & (\lim E'_\alpha) \otimes_A (\lim F'_\alpha)
\end{array}
$$

is commutative.

The verification is immediate.

Let $(A'_\alpha, \rho'_{\beta\alpha})$ be another direct system of rings and suppose that each $E_\alpha$ is an $(A'_\alpha, A_\alpha)$-bimodule, the $f_{\beta\alpha}$ being $(A'_\alpha, A_\alpha)$-linear for $\alpha \leq \beta$. Then if we write $A' = \lim A'_\alpha$, the isomorphism (7) is *linear* with respect to the left $A'$-module structures on the two sides by virtue of Corollary 1. This can be immediately generalized to arbitrary multimodules.

In particular, if the $A_\alpha$ are *commutative*, $A = \lim A_\alpha$ is commutative and isomorphism (7) is an *A-module isomorphism*.

#### Corollary 2 {#alg-ii-s6-prop-7-cor-2 .statement}

*Let* $(E_\alpha, f_{\beta\alpha})$ *be a direct system of right* $A_\alpha$*-modules and let* $E'_\alpha = E_\alpha \otimes_{A_\alpha} A$ *be the* $A$*-module obtained by extending the ring of scalars to* $A = \lim A_\alpha$ *by means of the canonical homomorphism* $\rho_\alpha : A_\alpha \to A$. *Then* $(E'_\alpha, f_{\beta\alpha} \otimes 1_A)$ *is a direct system of right* $A$*-modules, *whose direct limit is canonically isomorphic to* $\lim E_\alpha$.

It suffices to apply Proposition 7 with $F_\alpha$ the ring $A$ considered as an $(A_\alpha, A)$-bimodule by means of $\rho_\alpha$.

#### Corollary 3 {#alg-ii-s6-prop-7-cor-3 .statement}

*Let* $A$ *be a ring,* $(E_\alpha, f_{\beta\alpha})$ *a direct system of right* $A$*-modules and* $F$ *a left* $A$*-module. *Then the* $\mathbf{Z}$*-modules* $\lim (E_\alpha \otimes_A F)$ *and* $(\lim E_\alpha) \otimes_A F$ *are canonically isomorphic*.

It suffices to take $A_\alpha = A$ and $F_\alpha = F$ for all $\alpha \in I$ in Proposition 7.

In particular, if $\rho : A \to B$ is a ring homomorphism, $\lim \rho^*(E_\alpha)$ and $\rho^*(\lim E_\alpha)$ are canonically isomorphic.

#### Corollary 4 {#alg-ii-s6-prop-7-cor-4 .statement}

*Let* $M$ *be a right* $A$*-module, $N$ *a left* $A$*-module, $(x_i)_{1 \leq i \leq n}$ *a family of elements of* $M$, $(y_i)_{1 \leq i \leq n}$ *a family of elements of* $N$, *such that* $\sum_i (x_i \otimes y_i) = 0$ *in* $M \otimes_A N$. *Then there exists a finitely generated submodule* $M_1$ *(resp. $N_1$) of* $M$ *(resp. $N$) containing the* $x_i$ *(resp. the* $y_i$) *and such that* $\sum_i (x_i \otimes y_i) = 0$ *in* $M_1 \otimes_A N_1$.

$M$ (resp. $N$) is canonically identified with the direct limit of the right directed family of its finitely generated submodules containing the $x_i$ (resp. the $y_i$) and it suffices to apply *Set Theory, III, § 7, no. 5, Lemma 1.*

### Exercises {#alg-ii-s6-exercises}

See the [exercises for § 6](exercises/s6/).
