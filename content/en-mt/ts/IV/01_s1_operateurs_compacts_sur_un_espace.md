---
book: ts
book_title: Théories spectrales
chapter: IV
chapter_title: THÉORIE SPECTRALE HILBERTIENNE
section: 1
section_title: Opérateurs compacts sur un espace hilbertien
lang: en
source: ts-iii-v-fr
book_pages: TS IV.146-TS IV.179, TS IV.313-TS IV.319
pdf_pages: 0159-0192, 0326-0332
extraction: native
subsections:
    - "no": 1
      title: Endomorphismes diagonaux
      page: 146
      pdf_page: 159
    - "no": 2
      title: Diagonalisation des endomorphismes compacts
      page: 149
      pdf_page: 162
    - "no": 3
      title: Suite décroissante des valeurs propres
      page: 151
      pdf_page: 164
    - "no": 4
      title: Caractérisations variationnelles des valeurs propres
      page: 153
      pdf_page: 166
    - "no": 5
      title: Applications de la caractérisation variationnelle des valeurs propres
      page: 155
      pdf_page: 168
    - "no": 6
      title: Inégalités de Weyl
      page: 157
      pdf_page: 170
    - "no": 7
      title: Endomorphismes de trace finie
      page: 164
      pdf_page: 177
    - "no": 8
      title: Applications nucléaires
      page: 167
      pdf_page: 180
    - "no": 9
      title: Opérateurs intégraux de Hilbert–Schmidt
      page: 172
      pdf_page: 185
    - "no": 10
      title: Trace des opérateurs intégraux à noyau continu
      page: 174
      pdf_page: 187
statements: 66
exercises: 22
content_sha256: cff347a68f44a4f3da567c33474a6b11ca1254d89cd96fd15d27da328da51b68
translated_from: content/fr/ts/IV/01_s1_operateurs_compacts_sur_un_espace.md
source_lang: fr
translation_method: machine
source_content_sha256: b681dd80851bf0f5d53feeeac8bf034e244c262a89a447596400956cd41e3814
translation_model: gpt-5-6-mini, gpt-5-mini, gpt-5.4
translation_run: translate-en-mt-4edddf0b
glossary_version: 34
glossary_terms_sha256: 92b3d8a66f4c75ce894611b6780107b5939f48009e9370c550b07728dfeabe03
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 1. COMPACT OPERATORS ON A HILBERT SPACE

In this paragraph, K is a field equal to $\mathbf{R}$ or $\mathbf{C}$ and E denotes a Hilbert space over the field K.

### 1. Diagonal endomorphisms

#### Definition 1 {#ts-iv-s1-def-1 .statement tag=02W8}

Let $B = (e_i)_{i\in I}$ be an orthonormal basis of E. An endomorphism $u$ is said to be diagonal in the basis B or diagonal relative to B if there exists a family $\lambda = (\lambda_i)_{i\in I}$ of elements of K such that $u(e_i) =\lambda_ie_i$ for all $i\in I$.

Let $B = (e_i)_{i\in I}$ be an orthonormal basis of E. We denote by $\mathscr{D}_B(E)$ the set of endomorphisms of E which are diagonal relative to B. It is a closed commutative unital subalgebra of $\mathscr{L}(E)$. Let $u\in \mathscr{D}_B(E)$. The family $\lambda = (\lambda_i)_{i\in I}$ such that $u(e_i) =\lambda_ie_i$ is uniquely determined by $u$ and by the basis B, and it is said that this is the family of eigenvalues of $u$ relative to B.

Suppose that $K =\mathbf{R}$ and identify E with a subspace of $E_{(\mathbf{C})}$. Let $B = (e_i)_{i\in I}$ be an orthonormal basis of E. Denote by $B_{(\mathbf{C})}$ the orthonormal basis $(1\otimes e_i)_{i\in I}$ of $E_{(\mathbf{C})}($cf. EVT, V, p. 29, cor. 1). The mapping $u\mapsto u_{(\mathbf{C})}$ induces an injective algebra morphism from $\mathscr{D}_B(E)$ into $\mathscr{D}_{B_{(\mathbf{C})}}(E_{(\mathbf{C})})$; its image is the set of $u\in \mathscr{D}_{B_{(\mathbf{C})}}(E_{(\mathbf{C})})$ such that $u(E)\subset E$, in other words the set of $u$ diagonal in the basis $B_{(\mathbf{C})}$ whose eigenvalues are real.

For every $i\in I$, we denote by $p_i$ the orthogonal projector of E with image $Ke_i$. We have $\|p_i\|= 1$ for every $i\in I$. The endomorphism $p_i$ is diagonal in the basis B, the family of its eigenvalues is the family $(\delta_{ij})_{j\in I}$ (Kronecker symbol, cf. A, II, p. 24).

Let $B'= (f_i)_{i\in I}$ be an orthonormal basis of E and $u: E\rightarrow E$ the isometric isomorphism such that $u(f_i) =e_i$. Then $\mathscr{D}_{B'}(E) =u^{-1}\mathscr{D}_B(E)u$.

We equip I with the discrete topology and denote by $\mathscr{B}(I) =\mathscr{C}_b(I; K)$ the unital Banach algebra of bounded functions on I with values in K (example 2 of I, p. 17) ; if $K =\mathbf{C}$, it is a star algebra (example 2 of I, p. 102).

#### Lemma 1 {#ts-iv-s1-lem-1 .statement tag=02W9}

Let $u\in \mathscr{D}_B(E)$ and $\lambda = (\lambda_i)_{i\in I}$ the family of its eigenvalues. The family $\lambda$ is bounded and one has sup$_i|\lambda_i|=\|u\|$.

One has $|\lambda_i|\leqslant \|u\|$ for every $i$, whence sup$_{i\in I}|\lambda_i|\leqslant \|u\|$. Since moreover

$\|u(x)\|^2=\sum_{i\in I}|\lambda_i|^2|\langle e_i|x\rangle |^2\leqslant ($sup$_{i\in I}|\lambda_i|^2)\|x\|^2$

for every $x\in E$ (EVT, V, p. 22, prop. 5), it follows that $\|u\|=$ sup$|\lambda_i|$.

#### Proposition 1 {#ts-iv-s1-prop-1 .statement tag=02WA}

a) The mapping $\alpha$ from $\mathscr{D}_B(E)$ into $\mathscr{B}(I)$ which associates with a diagonal endomorphism $u$ the family of the eigenvalues of $u$ is an isometric isomorphism of Banach algebras over K. If $K =\mathbf{C}$, it is a morphism of involutive algebras ;

b) For every bounded family $\lambda = (\lambda_i)_{i\in I}$, the family $(\lambda_ip_i)_{i\in I}$ is summable in the space $\mathscr{L}(E)$ endowed with the topology of simple convergence, and the sum of this family is the unique mapping $u\in \mathscr{D}_B(E)$ such that $\alpha (u) =\lambda$;

c) Let $u\in \mathscr{D}_B(E)$ and let $\lambda$ be the family of its eigenvalues relative to B. The spectrum of $u$ is the closure in K of the set of values of $\lambda$;

d) If K = $\mathbf{C}$, then the continuous functional calculus mapping of $\mathscr{C}$ (Sp($u$)) into $\mathscr{L}(E)$ associates with a continuous function $f\in \mathscr{C}$ (Sp($u$)) the endomorphism $\alpha (f\circ \lambda )$ in $\mathscr{D}_B(E)$.

By Lemma 1, the family of eigenvalues of an endomorphism diagonal in B is bounded and the mapping of $\mathscr{D}_B(E)$ into $\mathscr{B}(I)$ thus defined is a continuous isometric morphism of unital Banach algebras.

Let $i\in I$. For every $j\in I$, one has $\langle u^*(e_i)|e_j\rangle =\lambda_j\langle e_i|e_j\rangle =\langle \overline{\lambda_j}e_i|e_j\rangle$. It follows that $u^*(e_i) =\overline{\lambda}_ie_i$. The adjoint of $u$ is therefore the endomorphism diagonal in the basis B whose family of eigenvalues is $(\lambda_i)_{i\in I}$. Assertion a) follows.

Let $\lambda = (\lambda_i)_{i\in I}\in \mathscr{B}(I)$. For every $x\in E$, the family $(|\langle e_i|x\rangle |^2)_{i\in I}$ is summable, with sum $\|x\|^2$ (EVT, V, p. 22, prop. 5), whence, for every finite subset J of I:

$\|\sum_{i\in J}\lambda_ip_i(x)\|^2=\sum_{i\in J}|\lambda_i|^2|\langle e_i|x\rangle |^2\leqslant ($sup$_{i\in I}|\lambda_i|^2)(\sum_{j\in J}|\langle e_i|x\rangle |^2$

$\leqslant ($sup$_{i\in I}|\lambda_i|)^2\|x\|^2$.

Consequently, the family $(\lambda_ip_i)$ is summable in $\mathscr{L}(E)$ endowed with the topology of simple convergence. Its sum $u_{\lambda}$ satisfies $u_{\lambda}(e_i) =\lambda_ie_i$; it is therefore an endomorphism diagonal in the basis B, with eigenvalues $\lambda$. Assertion b) follows.

The last assertions result from a), from Example 3 of I, p. 17 and from Example 4 of I, p. 111.

#### Remark {#ts-iv-s1-n1-rem-1 .statement tag=02WB}

The Banach algebra $\mathscr{D}_B(E)$ is a maximal commutative closed subalgebra of $\mathscr{L}(E)$. Indeed, let $u$ be an endomorphism of E which commutes with $\mathscr{D}_B(E)$. Let $i\in I$. Since the orthogonal projector $p_i$ is diagonal in the basis B, one has $p_i(u(e_i)) =u(p_i(e_i)) =u(e_i)$, which implies that $u(e_i)$ is proportional to $e_i$. Thus $u$ is diagonal in the basis B.

If E is of infinite dimension, there exist maximal commutative involutive subalgebras of $\mathscr{L}(E)$ which are not isomorphic to $\mathscr{D}_B(E)$ (exercise 5 of IV, p. 314).

#### Proposition 2 {#ts-iv-s1-prop-2 .statement tag=02WC}

Let $u\in \mathscr{D}_B(E)$ and $\lambda = (\lambda_i)_{i\in I}$ be the family of its eigenvalues.

a) The following conditions are equivalent:

(i) One has $\lambda \in \mathscr{C}_0(I; K)$;

(ii) The endomorphism $u$ is compact ;

(iii) The family $(\lambda_ip_i)_{i\in I}$ is summable in the Banach space

$\mathscr{L}(E)$. Its sum is then equal to $u$.

b) Suppose that $u$ is compact and denote by Λ the set of values of $\lambda$. The set of the $i\in I$ such that $\lambda_i\not = 0$ is countable. If E is of infinite dimension, one has Sp$_s(u) = \Lambda -\{0\}$ and Sp($u$) $= \Lambda \cup  \{0\}$. If E is of finite dimension, then Sp$_s(u) =$ Sp($u$) $= \Lambda$.

By Lemma 1, one has $\|\sum_{j\in J}\lambda_jp_j\|=$ sup$_{j\in J}|\lambda_j|$ for every finite subset J of I. It follows, by the Cauchy criterion, that the family $(\lambda_ip_i)$ is summable in $\mathscr{L}(E)$ if and only if the family $\lambda$ tends to 0 at infinity, which implies that conditions (i) and (iii) are equivalent.

Condition (iii) implies that $u$ is compact (corollary of Proposition 2 of III, p. 4). Conversely, suppose that the endomorphism $u$ is compact. Since the family B is bounded in E, its image by $u$ in E is relatively compact in E (III, p. 2), and hence precompact. Let $\varepsilon  >0$ and J be a finite subset of I such that the image of B by $u$ is contained in the union of the balls of radius $\varepsilon$ and centre $u(e_j)$ for $j\in J$. Let $i\in I$ - J. There exists $j\in J$ such that $\|u(e_i)-u(e_j)\|\leqslant \varepsilon$, hence

$$
|\lambda_i|^2\leqslant |\lambda_i|^2+|\lambda_j|^2=\|u(e_i)-u(e_j)\|^2\leqslant \varepsilon^2
$$

Consequently, one has $\lambda \in \mathscr{C}_0(I; K)$, that is, condition (i).

Finally, the spectrum of $u$ and its sensitive spectrum are calculated as functions of $\lambda$ by using prop. 1, c) and Proposition 5 of III, p. 90.

#### Remark {#ts-iv-s1-n1-rem-2 .statement tag=02WD}

When I is infinite, the condition $\lambda \in \mathscr{C}_0(I; K)$ may also be stated as follows: “the family $\lambda$ tends to 0 according to the filter of the complements of the finite subsets of I.”

### 2. Diagonalization of compact endomorphisms

#### Theorem 1 {#ts-iv-s1-thm-1 .statement tag=02WE}

Suppose $K =\mathbf{C}$. Let $u$ be a compact and normal endomorphism of E. There exists an orthonormal basis B of E such that $u$ is diagonal in the basis B.

The set Sp$_s(u)$ is countable, and it does not contain 0 if E is of infinite dimension (III, p. 90, prop. 5, b)). For every element $\lambda \in$ Sp$_s(u)$, denote by $N_{\lambda}$ the nullspace of $u-\lambda 1_E$. It is of finite dimension (loc. cit.) and, since $u$ is normal, it coincides with the eigenspace of $u$ relative to $\lambda$ (EVT, V, p. 43, cor. of prop. 8). The spaces $N_{\lambda}$ are pairwise orthogonal (I, p. 132, n$^o5$).

Let F be the subspace of E Hilbert sum of the spaces $N_{\lambda}$ for $\lambda \in$ Sp$_s(u)-\{0\}$. It is a space of countable type, stable under $u$ since each subspace $N_{\lambda}$ is stable under $u$. Since $N_{\lambda}$ is also the eigenspace of $u^*$ corresponding to $\overline{\lambda}$ (EVT, V, loc. cit.), the endomorphism $u$ induces an endomorphism $\widetilde{u}$ of $F^{\circ}$ by passing to subspaces. The endomorphism $\widetilde{u}$ is compact (Proposition 3 of III, p. 5) and normal (Lemma 4 of I, p. 135). By construction, the point spectrum of $\widetilde{u}$ is contained in $\{0\}$ (for, any eigenvector for $\widetilde{u}$ would be one for $u$, hence would belong to one of the spaces $N_{\lambda}$ if the corresponding eigenvalue were non-zero). Thus the spectral radius of $\widetilde{u}$ is zero, whence $\widetilde{u}= 0$ since $\widetilde{u}$ is normal (Corollary 1 of I, p. 108). Hence $F^{\circ}\subset$ Ker($u$).

For every $\lambda \in$ Sp$_s(u)$, let $B_{\lambda}$ be an orthonormal basis of $N_{\lambda}$ and let $(e_j)_{j\in J}$ be the family union of the $B_{\lambda}$; it is an orthonormal basis of F. Let B be the union of $(e_j)_{j\in J}$ and of an orthonormal basis of $F^{\circ}$. It is an orthonormal basis of E and $u$ is diagonal in the basis B.

#### Corollary 1 {#ts-iv-s1-thm-1-cor-1 .statement tag=02WF}

Let $u$ be a compact hermitian endomorphism of E. There exists an orthonormal basis B of E such that $u$ is diagonal in the basis B and its eigenvalues are real.

If $K =\mathbf{C}$, this follows at once from the theorem. Suppose $K =\mathbf{R}$. The space E is an $\mathbf{R}$-structure on $E_{(\mathbf{C})}($cf. A, II, p. 119). The endomorphism $u_{(\mathbf{C})}$ of $E_{(\mathbf{C})}$ is compact (Remark 4 of III, p. 2) and hermitian. Let $B = (e_j)_{j\in J}$ be an orthonormal basis of $E_{(\mathbf{C})}$ such that $u_{(\mathbf{C})}\in \mathscr{D}_B(E_{(\mathbf{C})})$ and $\lambda$ the family of eigenvalues of $u_{(\mathbf{C})}$ (Theorem 1). One has $\lambda \in \mathbf{R}^J($I, p. 106, Proposition 4) ; since the linear mapping $u_{(\mathbf{C})}$ is $\mathbf{R}$-rational, the eigenspace of $u_{(\mathbf{C})}$ corresponding to $\lambda_j$ is $\mathbf{R}$-rational for every $j\in J ($cf. A, V, p. 60, Proposition 6). Hence there exists a basis of it belonging to E, and a fortiori, there exists an orthonormal basis of it in E. The union of these bases is an orthonormal basis $B_{\mathbf{R}}$ of E such that $u\in \mathscr{D}_{B_{\mathbf{R}}}(E)$.

#### Corollary 2 {#ts-iv-s1-thm-1-cor-2 .statement tag=02WG}

Let F be a Hilbert space and let $u$ be a compact continuous linear mapping from E into F. There exists a countable set I, an orthonormal basis $(e_i)_{i\in I}$ of the initial space Ker($u$)$^{\circ}$ of $u$, an orthonormal family $(f_i)_{i\in I}$ of F and a family $(\alpha_i)_{i\in I}\in (\mathbf{R}^*_+)^I$ such that $u(e_i) =\alpha_if_i$ for all $i\in I$.

Let $v=u^*\circ u$. It is a compact endomorphism (III, p. 5, Prop. 3) and positive, hence hermitian, of E. By Corollary 1, there exists an orthonormal basis $(e_j)_{j\in J}$ of E such that $v$ is diagonal in this basis. The family $(\lambda_j)_{j\in J}$ of its eigenvalues is contained in $\mathbf{R}_+^J$. Put $\alpha_j=\surd\overline{\lambda_j}$ for all $j\in J$. Let I be the set of $j\in J$ such that $\alpha_j\not = 0$. It is a countable set since $v$ is compact. The family $(e_i)_{i\in I}$ is an orthonormal basis of the initial space of $v$, which is the initial space Ker($u$)$^{\circ}$ of $u$ (EVT, V, p. 43, Prop. 8). Put $f_i=\frac{1}{\alpha_i}u(e_i)$ for $i\in I$. Whatever $i$ and $j$ in I may be, one has

$$
\langle f_i|f_j\rangle =\frac{1}{\alpha_i\alpha_j}\langle u(e_i)|u(e_j)\rangle =\frac{1}{\alpha_i\alpha_j}\langle v(e_i)|e_j\rangle =\frac{\lambda_i}{\alpha_i\alpha_j}\langle e_i|e_j\rangle
$$

whence it follows that the family $(f_i)_{i\in I}$ is orthonormal in F. The corollary follows, since $u(e_i) =\alpha_if_i$ for all $i\in I$.

#### Definition 2 {#ts-iv-s1-def-2 .statement tag=02WH}

With the notations of the corollary, the family $(\alpha_i)_{i\in I}$ is the family of singular values of $u$, relative to the orthonormal basis $(e_i)_{i\in I}$ of the initial space of $u$.

#### Remark 1 {#ts-iv-s1-n2-rem-1 .statement tag=02WI}

This corollary generalizes Theorem 2 of EVT, V, p. 54, which corresponds to Hilbert–Schmidt mappings.

#### Remark 2 {#ts-iv-s1-n2-rem-2 .statement tag=02WJ}

With the notations of the corollary, one has the formula

$$
u(x) =\sum_{i\in I}\alpha_i\langle e_i|x\rangle f_i \tag{1}
$$

for all $x\in E$.

#### Remark 3 {#ts-iv-s1-n2-rem-3 .statement tag=02WK}

Let $u$ be a positive compact endomorphism of E. Let $B = (f_i)_{i\in I}$ be an orthonormal basis of E such that $u$ is diagonal in the basis B (Theorem 1), and let $(\lambda_i)_{i\in I}$ be the family of eigenvalues of $u$ in this basis. Let J be the set of $i\in I$ such that $\lambda_i>0$; the family $(e_i)_{i\in J}$ is an orthonormal basis of the space Ker($u$)$^{\circ}$. For all $i\in J$, put $e_i=f_i$ and $\alpha_i=\lambda_i$. It follows that $u(e_i) =\alpha_if_i:$ the family $(\alpha_i)_{i\in J}$ is the family of singular values of $u$ relative to the basis $(e_i)_{i\in J}$.

### 3. Decreasing sequence of eigenvalues

In this number, it is assumed that $K =\mathbf{C}$.

We denote by $\overline{\mathbf{N}}=\mathbf{N}\cup  \{+\infty \} \subset \overline{\mathbf{R}}$. In this number, we shall say that a vector space E is of dimension $+\infty  \in \overline{\mathbf{N}}$ if E is not of finite dimension.

Let $I_E\subset \mathbf{N}$ be the set of dimensions of the finite-dimensional subspaces F of E such that $F\not = E$. One has $I_E=\mathbf{N}$ if E is of infinite dimension, and otherwise $I_E=\{0, . . .$, dim(E) $-1\}$. We shall write $I = I_E$ when no confusion can result from this.

Let $u$ be a compact and positive (in particular hermitian) endomorphism of E. The point spectrum of $u$ is the set of values of a strictly decreasing sequence $(\nu_k)_{0\leqslant k<Card(Sp_s(u))}$ of positive real numbers (cf. prop. 5 of III, p. 90). For every integer $k$ such that $0\leqslant k <$ Card(Sp$_s(u)$), we denote by $n_k\geqslant 1$ the spectral multiplicity of $\nu_k$. Let $M\in \overline{\mathbf{N}}$ be the sum of the spectral multiplicities $n_k$; this is the dimension of the image of $u$. One has $M\leqslant$ Card(I).

For $0\leqslant n <M$, one defines $\lambda_n(u) =\nu_k$, where $k\geqslant 0$ is the unique integer such that

$$
n_0+\cdots +n_{k-1}\leqslant n < n_0+\cdots +n_k
$$

One sets $\lambda_n(u) = 0$ if $n\in I$ satisfies $n\geqslant M$. This case can arise only if $I =\mathbf{N}$ and if Sp$_s(u)$ is finite (or, what amounts to the same, if E is of infinite dimension and $u$ is of finite rank).

The sequence $(\lambda_n(u))_{n\in I}$ is decreasing; for every $\lambda \in$ Sp$_s(u)$, the number of integers $n$ such that $\lambda_n(u) =\lambda$ is equal to the spectral multiplicity of the eigenvalue $\lambda$ of $u$.

By an abuse of language, one says that $(\lambda_n(u))_{n\in J}$ is the decreasing sequence of the eigenvalues of $u$ repeated according to their multiplicities.

#### Proposition 3 {#ts-iv-s1-prop-3 .statement tag=02WL}

Let $u$ be a compact positive endomorphism of E. There exists an orthonormal family $(e_n)_{n\in I}$ in E such that, for every $x\in E$, one has

$$
u(x) =\sum_{n\in I}\lambda_n(u)\langle e_n|x\rangle e_n,\langle x|u(x)\rangle =\sum_{n\in I}\lambda_n(u)|\langle e_n|x\rangle |^2
$$

Let $B = (f_j)_{j\in J}$ be an orthonormal basis of E in which $u$ is diagonal (cor. 1 of IV, p. 150) and $(\lambda_j)_{j\in J}$ the family of eigenvalues of $u$ in the basis B. Let $J'$ be the set of $j\in J$ such that $\lambda_j$ belongs to the point spectrum of $u$.

For each $\lambda \in$ Sp$_s(u)$, there exists a bijection between the integers $n$ such that $0\leqslant n <M$ and $\lambda_n(u) =\lambda$ and the $j\in J'$ such that $\lambda_j=\lambda$, for these two sets have as cardinal the spectral multiplicity of $\lambda$. A choice of such bijections for each $\lambda$ defines a bijection $\iota$ of the set of integers such that $0\leqslant n <M$ onto the set $J'$. One defines the sequence $(e_n)_{0\leqslant n<M}$ in E by putting $e_n=f_{\iota(n)}$ for $0\leqslant n <M$. It is an orthonormal family in E.

In the case where M $<$ Card(I) $= +\infty$, the space F generated by $\{e_0, . . . , e_{M-1}\}$ is of finite dimension and its orthogonal complement $F^{\circ}$ is of infinite dimension; one chooses for $(e_n)_{n\geqslant M}$ an orthonormal family in $F^{\circ}$.

For every $x\in E$, one has

$$
u(x) =\sum_{j\in J'}\lambda_j\langle f_j|x\rangle f_j=\sum_{0\leqslant n<M}\lambda_n(u)\langle e_n|x\rangle e_n
$$

since $u(f_j) = 0$ when $j\in J$ - $J'$. If $n\in I$ satisfies $n\geqslant M$, one has $\lambda_n(u) = 0$, and one obtains the first formula of the proposition. The second results from it.

#### Proposition 4 {#ts-iv-s1-prop-4 .statement tag=02WM}

Let $u$ be a positive compact endomorphism of E. Let $f\in \mathscr{C}(\mathbf{R}_+)$ be a continuous increasing mapping such that $f(0) = 0$.

The endomorphism $f(u)$ is compact and positive and, for every $n\in I_E$, one has $\lambda_n(f(u)) =f(\lambda_n(u))$.

The endomorphism $f(u)$ is compact and positive by prop. 6, b) of III, p. 91 and prop. 15, a) of I, p. 117. The spectrum of $f(u)$ is the image under $f$ of the spectrum of $u$ (cor. 2 of I, p. 111). If $\lambda \in$ Sp$_s(f(u))$, the spectral multiplicity of $\lambda$ is the sum of the spectral multiplicities of the $\mu\in$ Sp($u$) such that $f(\mu) =\lambda$ (cor. 2 of III, p. 84). Since $f$ is increasing, the sequence $(f(\lambda_n(u)))_{n\in I_E}$ is decreasing. The assertion then results from the definition of the sequence $(\lambda_n(f(u)))_{n\in I_E}$.

### 4. Variational characterizations of eigenvalues

In this number, it is supposed that $K =\mathbf{C}$.

Let $u$ be a positive compact endomorphism of E and $(\lambda_n(u))_{n\in I_E}$ the decreasing sequence of eigenvalues of $u$. One puts $I = I_E$.

For every closed subspace F of E, one notes

$r_F(u) =$ inf $\frac{\langle x|u(x)\rangle}{2},R_F(u) =$ sup $\frac{\langle x|u(x)\rangle}{2}$,

$$
_{x\in F-\{0\}}\|x\|x_{\in F^{\circ-}\{0\}}\|x\|
$$

where the greatest lower bound (resp. the least upper bound) is taken in $[0,+\infty ]$.

For every $n\in \mathbf{N}$, let $\mathscr{F}_n$ denote the set of vector subspaces $F\subset E$ of dimension $n$. One says that a subspace $F\in \mathscr{F}_n$ is adapted to $u$ if it admits an orthonormal basis $(f_i)_{0\leqslant i\leqslant n-1}$ such that $u(f_i) =\lambda_i(u)f_i$ for $0\leqslant i\leqslant n-1$.

#### Proposition 5 {#ts-iv-s1-prop-5 .statement tag=02WN}

Let $n\in I$.

a) For every subspace $F\in \mathscr{F}_{n+1}$ adapted to $u$, one has $\lambda_n(u) =r_F(u)$;

b) For every subspace $F\in \mathscr{F}_n$ adapted to $u$, one has $\lambda_n(u) = R_F(u)$.

Let $F\in \mathscr{F}_{n+1}$ be a subspace adapted to $u$, and $(f_i)_{0\leqslant i\leqslant n}$ an orthonormal basis of F such that $u(f_i) =\lambda_i(u)f_i$ for every $i$. For every $x$ in F, one has

$$
\langle x|u(x)\rangle =\sum_{0\leqslant i\leqslant n}\lambda_i(u)|\langle f_i|x\rangle |^2\geqslant \lambda_n(u)\sum_{0\leqslant i\leqslant n}|\langle f_i|x\rangle |^2=\lambda_n(u)\|x\|^2
$$

with equality if $x=f_n$. This implies that $r_F(u) =\lambda_n(u)$, whence assertion a).

Let $F\in \mathscr{F}_n$ be a subspace adapted to $u$. The closed subspace $F^{\circ}$ is nonzero (for $n=$ dim(F) $<$ dim(E)) and stable under $u$; the endomorphism $\widetilde{u}$ of $F^{\circ}$ deduced from $u$ by passing to subspaces is compact and positive.

One has Sp($\widetilde{u}$)$\subset$ Sp($u$). Moreover, one has Sp($\widetilde{u}$)$\subset [0, \lambda_n(u)]$. In fact, it is enough to verify that $\lambda \leqslant \lambda_n(u)$ for every $\lambda \in$ Sp$_s(\widetilde{u})$. The number $\lambda$ is then an eigenvalue of $u$, hence there exists $j\in I$ such that $\lambda =\lambda_j(u)$. The eigenspace of $u$ relative to $\lambda_j(u)$ is therefore not contained in F, which implies that $\lambda_j(u)\leqslant \lambda_n(u)$.

Suppose that $\lambda_n(u)>0$. Then the eigenspace of $u$ relative to $\lambda_n(u)$ is not contained in F, and therefore $\lambda_n(u)$ belongs to the point spectrum of $\widetilde{u}$. It follows that sup(Sp($\widetilde{u}$)) $=\lambda_n(u)$. If $\lambda_n(u) = 0$, one has the same result since the spectrum of $\widetilde{u}$ is then reduced to $\{0\}$.

Moreover, by definition one has $R_F(u) = R_{\{0\}}(\widetilde{u})$, and finally $R_{\{0\}}(\widetilde{u}) =$ sup(Sp($\widetilde{u}$)) by Prop. 9 of I, p. 139, a). Assertion b) is proved.

#### Proposition 6 {#ts-iv-s1-prop-6 .statement tag=02WO}

For every $n\in I$, one has

$\lambda_n(u) =$ sup$_{F\in\mathscr{F}_{n+1}}r_F(u) =$ inf$_{F\in\mathscr{F}_n}R_F(u)$.

Let $(e_n)_{n\in I}$ be an orthonormal family having the property of Prop. 3 of IV, p. 152. For every integer such that $1\leqslant n <M + 1$, let $F_n\in \mathscr{F}_n$ be the subspace of dimension $n$ of E generated by $(e_0, . . . , e_{n-1})$; by construction, the space $F_n$ is adapted to $u$. By Prop. 5, one therefore has

$$
\lambda_n(u) =r_{F_{n+1}}(u) = R_{F_n}(u) \tag{2}
$$

Let $n\in I$. Let $F\in \mathscr{F}_{n+1}$. The restriction to F of the orthogonal projector onto $F_n$ is not injective, hence there exists $x\not = 0$ in F orthogonal to $F_n$. Since $x\in F^{\circ}_n$, one then has (Prop. 3 of IV, p. 152)

$$
\langle x|u(x)\rangle =\sum_{m\in I}\lambda_m(u)|\langle e_m|x\rangle |^2
$$

$m\geqslant n$

$$
\leqslant \lambda_n(u)\sum_{mm\geqslant\in nI}|\langle e_m|x\rangle |^2=\lambda_n(u)\|x\|^2
$$

This proves that $r_F(u)\leqslant \lambda_n(u)$, whence in particular the inequality

(3) Fsup$_{\in\mathscr{F}_{n+1}}r_F(u)\leqslant \lambda_n(u)$.

Let $F\in \mathscr{F}_n$. The restriction to $F_{n+1}$ of the orthogonal projector onto F is not injective, hence there exists a vector $x\not = 0$ in $F_{n+1}$ orthogonal to F. Since $x\in F_{n+1}$, one has (loc. cit.)

$$
\langle x|u(x)\rangle =\sum_{0\leqslant m\leqslant n}\lambda_m(u)|\langle e_m|x\rangle |^2
$$

$$
\geqslant \lambda_n(u)\sum_{0\leqslant m\leqslant n}|\langle e_m|x\rangle |^2=\lambda_n(u)\|x\|^2
$$

and therefore $R_F(u)\geqslant \lambda_n(u)$. In particular, one obtains

(4) Finf$_{\in\mathscr{F}_n}R_F(u)\geqslant \lambda_n(u)$.

In view of formulas (2), (3) and (4), the proposition is proved.

### 5. Applications of the variational characterization of eigenvalues

In this No., Hilbert spaces over $\mathbf{C}$ are considered.

#### Proposition 7 {#ts-iv-s1-prop-7 .statement tag=02WP}

Let $u$ and $v$ be positive compact endomorphisms of E.

a) One has $|\lambda_n(u)-\lambda_n(v)|\leqslant \|u-v\|$ for every $n\in I$;

b) If $u\leqslant v$, then $\lambda_n(u)\leqslant \lambda_n(v)$ for every $n\in I$.

Let $n\in I$ and let F be a vector subspace of dimension $n$ of E. For every $x\in F$, one has

$$
|\langle x|v(x)\rangle  - \langle x|u(x)\rangle |\leqslant \|u-v\| \|x\|^2
$$

hence the inequalities

$$
R_F(v)- \|u-v\|\leqslant R_F(u)\leqslant R_F(v) +\|u-v\|
$$

Assertion a) follows from this by Proposition 6 of IV, p. 154.

If $u\leqslant v$, one has $\langle x|u(x)\rangle \leqslant \langle x|v(x)\rangle$ for every $x\in E$. For every $n\in I$ and every subspace F of dimension $n$, one therefore has $R_F(u)\leqslant R_F(v)$, whence $\lambda_n(u)\leqslant \lambda_n(v) ($loc. cit.).

#### Proposition 8 {#ts-iv-s1-prop-8 .statement tag=02WQ}

Let $u$ be a positive compact endomorphism of E. Let H be a closed subspace of E and $i_H: H\rightarrow E$ the canonical injection. Denote by $u_H$ the endomorphism $i^*_Hui_H$ of H. It is compact and positive.

a) One has $I_H\subset I_E$ and $\lambda_n(u_H)\leqslant \lambda_n(u)$ for all $n\in I_H$;

b) If H is of finite codimension $k\in \mathbf{N}$ in E, then one has $I_H+k\subset I_E$ and $\lambda_{n+k}(u)\leqslant \lambda_n(u_H)$ for all $n\in I_H$.

The endomorphism $u_H$ is compact (prop. 3 of III, p. 5). It is positive since $\langle x|u_H(x)\rangle =\langle i_H(x)|u(i_H(x))\rangle \geqslant 0$ for all $x\in H$.

Let $n\in I_H\subset I_E$. Let F be a subspace of dimension $n+ 1$ of H adapted to $u_H$. One has therefore $\lambda_n(u_H) =r_F(u_H)$ (prop. 5 of IV, p. 153, a)), and since moreover $r_F(u_H) =r_F(u)\leqslant \lambda_n(u)$ (prop. 6 of IV, p. 154), one obtains assertion a).

Suppose that H is of codimension $k\in \mathbf{N}$ in E and that $n\in I_H$. Let F be a subspace of H of dimension $n$ adapted to $u_H$. Its orthogonal complement in H is equal to $H\cap F^{\circ}$, and it is the orthogonal complement in E of the subspace $F + H^{\circ}$ of dimension $n+k$. Hence $n+k\in I_E$ and (prop. 5 of IV, p. 153, b))

$\lambda_n(u_H) =$ sup $\frac{\langle x|u_H(x)\rangle}{2}= R_{F+H^{\circ}}(u)$

$$
_{x\in H\cap F^{\circ}}\|x\|
$$

$x\not =0$

whence $\lambda_n(u_H)\leqslant \lambda_{n+k}(u)$ (prop. 6 of IV, p. 154).

#### Definition 3 {#ts-iv-s1-def-3 .statement tag=02WR}

Let F be a Hilbert space and let $u$ be a compact linear mapping of E into F.

For every integer $n\in I_E$ one denotes by $\alpha_n(u) =\lambda_n(u^*\circ u)$. Let J be the set of $n\in I_E$ such that $\alpha_n(u)>0$. The family $(\alpha_n(u))_{n\in J}$ is called the sequence of singular values of $u$ repeated according to multiplicity.

One says that the sequence $(\alpha_n(u))_{n\in I_E}$ is the extended sequence of singular values of $u$.

The sequence $(\alpha_n(u))_{n\in I_E}$ is well defined since the endomorphism $u^*\circ u$ of E is compact (III, p. 5, prop. 3); it is a decreasing family of positive real numbers since $u^*\circ u$ is positive.

#### Proposition 9 {#ts-iv-s1-prop-9 .statement tag=02WS}

Let F be a Hilbert space and let $u$ be a compact linear mapping of E into F.

a) For $n\in I_E$, one has

$\alpha_n(u) =$ sup$_{F\in\mathscr{F}_{n+1}}$ inf$_{x\in F-\{0\}}\frac{\|u(x)\|}{\|x\|}=$ inf$_{F\in\mathscr{F}_n}$ sup$_{x\in F^{\circ-}\{0\}}\frac{\|u(x)\|}{\|x\|}$.

b) Let J be the set of $n\in I_E$ such that $\alpha_n(u)\not = 0$. There exist orthonormal families $(e_n)_{n\in J}$ in E and $(f_n)_{n\in J}$ in F such that for every $x\in E$, one has

$$
u(x) =\sum_{n\in J}\alpha_n(u)\langle e_n|x\rangle f_n
$$

Since $\langle x|u^*u(x)\rangle =\|u(x)\|^2$ for every $x\in E$, the definitions and prop. 6 of IV, p. 154, a), imply the equality of the first assertion.

Let $(e_n)_{n\in I_E}$ be an orthonormal family of E satisfying the conclusions of prop. 3 of IV, p. 152 applied to the positive compact endomorphism $u^*\circ u$ of E. Put $f_n=\alpha^{-1}_nu(e_n)$ for $n\in J$. By reasoning as in the proof of corollary 2 of IV, p. 150, one obtains assertion c).

#### Corollary {#ts-iv-s1-n5-cor-1 .statement tag=02WT}

Let F be a Hilbert space and $u$ a compact linear mapping of E into F. Let $w\in \mathscr{L}(E)$ and $v\in \mathscr{L}(F)$. For every $n\in I_E$, one has $\alpha_n(w\circ u\circ v)\leqslant \|v\| \|w\|\alpha_n(u)$.

This is a consequence of assertion a) of the preceding proposition.

#### Remark 1 {#ts-iv-s1-n5-rem-1 .statement tag=02WU}

Since the sequence $(\alpha_n(u))_{n\in I_E}$ is decreasing, the set J is either equal to $I_E$, or equal to a segment $\{0, . . . , m\}$ in $I_E$ where $m\in \mathbf{N}$. This latter case holds if and only if $u$ is of finite rank.

#### Remark 2 {#ts-iv-s1-n5-rem-2 .statement tag=02WV}

As $\|u(x)\|=\||u|(x)\|$ for every $x\in E ($I, p. 139, prop. 10), one has $\alpha_n(u) =\alpha_n(|u|)$ for every $n\in I_E$.

#### Remark 3 {#ts-iv-s1-n5-rem-3 .statement tag=02WW}

If $u$ is positive, then $\alpha_n(u) =\lambda_n(u)$ for every $n\in I_E$ (indeed, one then has $\alpha_n(u)^2=\lambda_n(u^*u) =\lambda_n(u^2) =\lambda_n(u)^2$ by Prop. 4 of IV, p. 153).

#### Remark 4 {#ts-iv-s1-n5-rem-4 .statement tag=02WX}

It is possible that $\alpha_n(v\circ u\circ w) = 0$ even if $\alpha_n(u)$ is nonzero; in this case, $\alpha_n(v\circ u\circ w)$ is not a singular value of $v\circ u\circ w$.

### 6. Weyl Inequalities

In this No., we consider Hilbert spaces over $K =\mathbf{C}$.

Let E be a Hilbert space. For every $n\in \mathbf{N}$, we recall that the Hilbert exterior power $\widehat{\wedge}^nE$ was defined in EVT, V, p. 34. For every Hilbert space F and for $u\in \mathscr{L}(E; F)$, the linear mapping $\widehat{\wedge}^nu\in \mathscr{L}(\widehat{\wedge}^nE;\widehat{\wedge}^nF) $ was also defined (loc. cit.). These constructions are functorial: for every Hilbert space G and for every linear mapping $v\in \mathscr{L}(F; G)$, the formula

$$
\widehat{\wedge}^nv\circ \widehat{\wedge}^nu=\widehat{\wedge}^n(v\circ u)
$$

holds (loc. cit., formula (28)).

Let H be a closed subspace of E and $i_H$ the canonical injection of H into E. For every endomorphism $u$ of E, we denote by $u_H$ the endomorphism $i^*_Hui_H$ of H.

#### Lemma 2 {#ts-iv-s1-lem-2 .statement tag=02WY}

Let $n\in \mathbf{N}$. The mapping $\widehat{\wedge}^ni_H$ is an isometric linear mapping of $\widehat{\wedge}^nH$ into $\widehat{\wedge}^nE$.

Let $(e_j)_{j\in J}$ be an orthonormal basis of H and $(e_j)_{j\in J'}$ an orthonormal basis of E, where $J\subset J'$. Let us endow $J'$ with a total ordering. The elements $e_{j_1}\wedge  \cdots  \wedge e_{j_n}$ for $j_1<\cdots < j_n$ in $J'$ (resp. in J) form an orthonormal basis of $\widehat{\wedge}^nE$ (resp. of $\widehat{\wedge}^nH$) by Prop. 5 of EVT, V, p. 34, prop. 5. The lemma follows.

In what follows, we shall identify $\widehat{\wedge}^nH$ with a closed subspace of $\widehat{\wedge}^nE$ by means of the mapping $\widehat{\wedge}^ni_H$.

#### Lemma 3 {#ts-iv-s1-lem-3 .statement tag=02WZ}

Let F be a Hilbert space and $u\in \mathscr{L}(E; F)$. Let $n\in \mathbf{N}$.

a) One has $(\widehat{\wedge}^nu)^*=\widehat{\wedge}^n(u^*)$;

b) If F = E and $u$ is hermitian (resp. positive, normal, unitary), then $\widehat{\wedge}^nu$ is hermitian (resp. positive, normal, unitary) ;

c) One has $|\widehat{\wedge}^nu|=\widehat{\wedge}^n|u|$;

d) Let H be a closed subspace of E. The restriction $(\widehat{\wedge}^nu)|\widehat{\wedge}^nH$ of $\widehat{\wedge}^nu$ to $\widehat{\wedge}^nH$ is equal to $\widehat{\wedge}^n(u|H) ($equality in $\mathscr{L}(\widehat{\wedge}^nH;\widehat{\wedge}^nF))$;

e) Suppose F = E. Let H be a closed subspace of E. One has $(\widehat{\wedge}^nu)_{\widehat{\wedge}^nH}=\widehat{\wedge}^n(u_H)$ in $\mathscr{L}(\widehat{\wedge}^nH)$.

Assertion a) results from EVT, V, p. 39, formula (13). It implies at once that $\widehat{\wedge}^nu$ is hermitian (resp. unitary) when $u$ is hermitian (resp. unitary). If $u$ is positive, then $u^{1/2}$ is hermitian, hence so is $\widehat{\wedge}^n(u^{1/2})$; the relation $\widehat{\wedge}^nu=(\widehat{\wedge}^nu^{1/2})^2$ implies that $\widehat{\wedge}^nu$ is positive (I, p. 138, prop. 8). This proves b).

The foregoing makes it possible to calculate that

$$
(\widehat{\wedge}^n|u|)^2=\widehat{\wedge}^n(|u|^2) =\widehat{\wedge}^n(u^*u)
$$

$$
=\widehat{\wedge}^nu^*\widehat{\wedge}^nu=(\widehat{\wedge}^nu)^*(\widehat{\wedge}^nu) =|\widehat{\wedge}^nu|^2
$$

Since $\widehat{\wedge}^n|u|$ is positive by b), it follows from prop. 16 of I, p. 118 that $\widehat{\wedge}^n|u|=|\widehat{\wedge}^nu|$, whence c).

Let $i_H$ be the canonical injection of H into E. The space $\widehat{\wedge}^nH$ is identified with a closed subspace of $\widehat{\wedge}^nE$ by the mapping $\widehat{\wedge}^ni_H$, whence

$$
(\widehat{\wedge}^nu)|\widehat{\wedge}^nH =\widehat{\wedge}^nu\circ \widehat{\wedge}^ni_H=\widehat{\wedge}^n(u\circ i_H) =\widehat{\wedge}^n(u|H)
$$

and

$$
(\widehat{\wedge}^nu)_{\widehat{\wedge}^nH}= (\widehat{\wedge}^ni_H)^*\circ \widehat{\wedge}^nu\circ \widehat{\wedge}^ni_H=\widehat{\wedge}^n(i^*_Hui_H) =\widehat{\wedge}^n(u_H)
$$

which proves d) and e).

Let F be a Hilbert space, and let $u\in \mathscr{L}^c(E; F)$. As in IV, p. 151, we denote by $I_E$ the set of dimensions of finite-dimensional subspaces F of E such that $F\not = E$. Recall that $(\alpha_n(u))_{n\in I_E}$ denotes the extended sequence of singular values of $u$ (def. 3 of IV, p. 156).

#### Proposition 10 {#ts-iv-s1-prop-10 .statement tag=02X0}

One has the equality

$$
\prod_{i=0}^n\alpha_i(u) =\|\wedge^{n+1}u\|
$$

for every $n\in I_E$.

Lemma 3, c) proves that $\|\widehat{\wedge}^{n+1}u\|=\|\widehat{\wedge}^{n+1}|u|\|$; moreover, since $\alpha_i(u) =\alpha_i(|u|)$ for every $i\in I_E$ (remark 5 of IV, p. 157, (2)), it is enough to prove the assertion for $|u|$. This makes it possible to suppose that F = E and that $u$ is positive.

Let then $B = (e_j)_{j\in J}$ be an orthonormal basis of E such that $u$ is diagonalizable in the basis B (theorem 1 of IV, p. 149), and let $(\lambda_j)_{j\in J}$ be the family of eigenvalues of $u$ in the basis B. Endow J with a total order, and denote by $J_n$ the set of strictly increasing families $(j_0, . . . , j_n)\in J^{n+1}$ of elements of J. The vectors

$$
e_{\iota}=e_{j_0}\wedge  \cdots  \wedge e_{j_n}
$$

for $\iota = (j_0, . . . , j_n)\in J_n$ form an orthonormal basis $B_n$ of $\widehat{\wedge}^{n+1}E$ (EVT, V, p. 34, prop. 5). For every $\iota = (j_0, . . . , j_n)\in J_n$, let

$$
\lambda_{\iota}=\prod_{j=0}^n\lambda_{i_j}
$$

Then $(\widehat{\wedge}^{n+1}u)e_{\iota}=\lambda_{\iota}e_{\iota}$, hence $\widehat{\wedge}^{n+1}u$ is diagonal in the basis $B_n$. Consequently, one has

$\|\widehat{\wedge}^{n+1}u\|=$ sup$_{\iota\in I_n}\lambda_{\iota}$

(lemma 1 of IV, p. 147), which is equal to the product $\lambda_0(u)\cdots \lambda_n(u)$ of the $n+ 1$ greatest eigenvalues of $u$. The desired formula follows, since $\lambda_i(u) =\alpha_i(u)$ for every $i\in I_E$ when $u$ is positive (remark 5 of IV, p. 157, (3)).

In particular, if $\alpha_1(u)< \alpha_0(u) =\|u\|$, one sees that the inequality $\|\widehat{\wedge}^n(u)\|\leqslant \|u\|^n$ (EVT, V, p. 34, formula (29)) is not an equality in general if $n\geqslant 2$.

#### Corollary {#ts-iv-s1-n6-cor-1 .statement tag=02X1}

Let G be a Hilbert space and $v\in \mathscr{L}^c(F; G)$. Then

$$
\prod_{i=0}^n\alpha_i(v\circ u)\leqslant \prod_{i=0}^n\alpha_i(u)\alpha_i(v)
$$

for every $n\in I_E$.

It suffices to remark that

$$
\|\widehat{\wedge}^{n+1}(vu)\|=\|\widehat{\wedge}^{n+1}v\circ \widehat{\wedge}^{n+1}u\|\leqslant \|\widehat{\wedge}^{n+1}v\| \|\widehat{\wedge}^{n+1}u\|
$$

and to apply proposition 10.

#### Lemma 4 {#ts-iv-s1-lem-4 .statement tag=02X2}

Let A be a ring. Let $n\in \mathbf{N}$ and let $(a_i)_{0\leqslant i\leqslant n}$ and $(b_i)_{0\leqslant i\leqslant n}$ be families of elements of A. For $0\leqslant j\leqslant n$, put

$$
A_j=\sum_{i=0}^ja_i
$$

Then

$$
\sum_{i=0}^na_ib_i= A_nb_n-\sum^{n-1}_{i=0}A_i(b_{i+1}-b_i)
$$

Put $A_{-1}= 0$. We have $a_i= A_i-A_{i-1}$ for $0\leqslant i\leqslant n$, hence

$$
\sum_{i=0}^na_ib_i=\sum_{i=0}^n(A_i-A_{i-1})b_i=\sum^{n-1}_{i=0}A_i(b_i-b_{i+1}) + A_nb_n
$$

as desired.

Let I be an interval of $\overline{\mathbf{R}}$ not containing $+\infty$. Recall (FVR, I, p. 38, remark) that a continuous function $f: I\rightarrow [-\infty ,+\infty [$ is said to be convex if its restriction to the interior of I is a convex function with values in $\mathbf{R}$; it then has a limit (finite or infinite) on the right at inf I. In the statements below, the product of 0 and an element of $\{-\infty ,+\infty \}$ is by convention equal to 0.

#### Lemma 5 {#ts-iv-s1-lem-5 .statement tag=02X3}

Let $I\subset \overline{\mathbf{R}}$ be an interval not containing $+\infty$, and let $f$ be an increasing convex function from I into $[-\infty ,+\infty [$.

Let $n$ be a natural number, and let

$$
a_0\geqslant a_1\geqslant \cdots \geqslant a_n,b_0\geqslant b_1\geqslant \cdots \geqslant b_n
$$

be elements of I.

Let $\varrho_0\geqslant \varrho_1\geqslant \cdots \geqslant \varrho_n$ be positive real numbers. Suppose that

$$
\sum_{i=0}^ja_i\leqslant \sum_{i=0}^jb_i \tag{5}
$$

for every integer $j$ such that $0\leqslant j\leqslant n$. Then

$$
\sum_{i=0}^n\varrho_if(a_i)\leqslant \sum_{i=0}^n\varrho_if(b_i) \tag{6}
$$

Suppose first that $a_i\in \mathring{I}$, and hence $f(a_i)\in \mathbf{R}$, for every $i$. Let $i$ be such that $0\leqslant i\leqslant n$, and let $(\alpha_i, \beta_i)$ be real numbers such that the line with equation $y=\alpha_ix+\beta_i$ is a support line of the graph of $f$ at the point $(a_i, f(a_i))$ (FVR, I, p. 37). Consequently we have $f(a_i) =\alpha_ia_i+\beta_i$ and $f(b_i)\geqslant \alpha_ib_i+\beta_i$ since the graph of $f$ lies above the support line, whence

$$
f(b_i)-f(a_i)\geqslant \alpha_i(b_i-a_i) \tag{7}
$$

Moreover, if $i < n$, we have

$$
\alpha_i\geqslant f'_g(a_i)\geqslant f'_d(a_{i+1})\geqslant \alpha_{i+1}
$$

(loc. cit. and FVR, I, p. 36, cor. 1); moreover $\alpha_i\geqslant 0$ since $f$ is increasing (FVR, I, p. 22, corollary), whence $\varrho_i\alpha_i\geqslant \varrho_{i+1}\alpha_{i+1}\geqslant 0$ for $0\leqslant i < n$.

Let $j$ be an integer such that $0\leqslant j\leqslant n$. Put

$$
A_j=\sum_{i=0}^j(b_i-a_i)
$$

so that $A_j\geqslant 0$ by hypothesis (5). Applying inequality (7) and then lemma 4, we deduce that

$$
\sum_{i=0}^n\varrho_i(f(b_i)-f(a_i))\geqslant \sum_{i=0}^n\varrho_i\alpha_i(b_i-a_i)
$$

$$
=\varrho_n\alpha_nA_n+\sum^{n-1}_{j=0}(\varrho_j\alpha_j-\varrho_{j+1}\alpha_{j+1})A_j\geqslant 0
$$

Consider the general case, and argue by induction on $n$. If one of the $a_i$ does not belong to the interior of I, we necessarily have $a_0=$ sup I or $a_n=$ inf I.

Suppose first that $a_n$ = inf I. Then we have $a_n\leqslant b_n$ and therefore $\varrho_nf(a_n)\leqslant \varrho_nf(b_n)$. The induction hypothesis, applied to the families $(a_0, . . . , a_{n-1}), (b_0, . . . , b_{n-1})$ and $(\varrho_0, . . . , \varrho_{n-1})$, implies

$$
\sum^{n-1}_{i=0}\varrho_if(a_i)\leqslant \sum^{n-1}_{i=0}\varrho_if(b_i)
$$

whence the desired inequality, by adding $\varrho_nf(a_n)$. The case where $a_0=$ sup I is treated similarly.

#### Proposition 11 (Weyl Inequalities) {#ts-iv-s1-prop-11 .statement tag=02X4}

Let G be a Hilbert space and $v\in \mathscr{L}^c(F; G)$. Let $g:\mathbf{R}_+\rightarrow [-\infty ,+\infty [$ be an increasing function such that the function $g\circ$ exp is convex. We have

$$
\sum_{i=0}^ng(\alpha_i(v\circ u))\leqslant \sum_{i=0}^ng(\alpha_i(v)\alpha_i(u))
$$

for all $n\in I_E\cap I_F$.

Put $I = [-\infty ,+\infty [$ and $f=g\circ$ exp. We may apply Lemma 5 with

$a_i=$ log($\alpha_i(v\circ u)$)$\in I,b_i=$ log($\alpha_i(v)\alpha_i(u)$)$\in I$

and $\varrho_i= 1$ for $0\leqslant i\leqslant n$, since

$\sum_{i=0}^ja_i=$ log$(\prod_{i=0}^j\alpha_i(v\circ u))\leqslant$ log$(\prod_{i=0}^j\alpha_i(v)\alpha_i(u))=\sum_{i=0}^jb_i$

for $0\leqslant j\leqslant n$ by the corollary to Prop. 10. Inequality (6) is then the desired conclusion.

#### Lemma 6 {#ts-iv-s1-lem-6 .statement tag=02X5}

Let $g$ and $h$ be convex functions defined on intervals I and J of $\mathbf{R}$, respectively. If $g$ is increasing and defined on the image of $h$, then the function $g\circ h$ is convex on J.

In fact, for $t\in [0,1]$ and $(x, y)\in J\times J$, we have

$$
g(h(tx+ (1-t)y))\leqslant g(th(x) + (1-t)h(y))
$$

$$
\leqslant tg(h(x)) + (1-t)g(h(y))
$$

#### Corollary {#ts-iv-s1-n6-cor-2 .statement tag=02X6}

Let G be a Hilbert space and $v\in \mathscr{L}^c(F; G)$. Let $n\in I_E\cap I_F$.

a) Let $r\in \mathbf{R}^*_+$. We have

$$
\sum_{i=0}^n\alpha_i(v\circ u)^r\leqslant \sum_{i=0}^n\alpha_i(v)^r\alpha_i(u)^r
$$

b) Let $p, q, r\in \mathbf{R}_+^*$ be such that $\frac{1}{p}+\frac{1}{q}=\frac{1}{r}$. Then

$$
(\sum_{i=0}^n\alpha_i(v\circ u)^r)^{1/r}\leqslant (\sum_{i=0}^n\alpha_i(v)^p)^{1/p}(\sum_{i=0}^n\alpha_i(u)^q)^{1/q}
$$

c) Suppose that F = E. For every integer $m\geqslant 2$, we have

$$
\sum_{i=0}^n\alpha_i(u^m)\leqslant (\sum_{i=0}^n\alpha_i(u)^2)^{m/2}
$$

Let $r\in \mathbf{R}^*_+$ and let $g$ be the function defined on $\mathbf{R}_+$ by $g(x) =x^r$. The function $g\circ$ exp is convex (Lemma 6), and therefore assertion a) follows from Prop. 11 applied to the function $g$.

Assertion b) follows from a) and Hölder's inequality (INT, I, Prop. 4).

Let $m\geqslant 2$ be an integer. Apply b) with $r= 1,p=q= 2$ and $v=u^{m-1}$. We find

$$
\sum_{i=0}^n\alpha_i(u^m)\leqslant (\sum_{i=0}^n\alpha_i(u^{m-1})^2)^{1/2}(\sum_{i=0}^n\alpha_i(u)^2)^{1/2}
$$

Let us prove c) by induction on $m\geqslant 2$. The preceding inequality establishes the assertion when $m= 2$. Suppose that $m\geqslant 3$ and that the assertion is valid for $m-1$; since one has

$$
\sum_{i=0}^n\alpha_i(u^{m-1})^2\leqslant (\sum_{i=0}^m\alpha_i(u^{m-1}))^2
$$

the above inequality implies

$$
\sum_{i=0}^n\alpha_i(u^m)\leqslant (\sum_{i=0}^n\alpha_i(u^{m-1}))^{1/2}(\sum_{i=0}^n\alpha_i(u)^2)^{1/2}\leqslant (\sum_{i=0}^n\alpha_i(u)^2)^{m/2}
$$

applying the induction hypothesis.

### 7. Endomorphisms of Finite Trace

Recall that a positive endomorphism $u$ of E is of finite trace if and only if there exists an orthonormal basis $(e_i)_{i\in I}$ of E such that

$$
\sum_{i\in I}\langle e_i|u(e_i)\rangle <+\infty
$$

(EVT, V, p. 48, lemma 3 and p. 49, def. 7). If $K =\mathbf{C}$, the space $\mathscr{L}_1(E)$ of endomorphisms of finite trace of E is the vector space generated by the set of positive endomorphisms of finite trace (EVT, V, p. 50, def. 8); if $K =\mathbf{R}$, the space $\mathscr{L}_1(E)$ is defined as the intersection $\mathscr{L}(E)\cap \mathscr{L}_1(E_{(\mathbf{C})})$ (EVT, V, p. 50).

If $u\in \mathscr{L}_1$(E), then the series

$$
\sum_{i\in I}\langle e_i|u(e_i)\rangle
$$

converges for every orthonormal basis $(e_i)_{i\in I}$ of E and its sum is independent of the orthonormal basis; one says that it is the trace Tr($u$) of $u$ (EVT, V, p. 50). If $K =\mathbf{R}$, one has Tr($u$) $=$ Tr($u_{(\mathbf{C})}$).

Let $u\in \mathscr{L}_1(E)$. One has $u^*\in \mathscr{L}_1(E)$ and Tr($u^*$) $=$ Tr($u$) $($loc. cit.).

#### Proposition 12 {#ts-iv-s1-prop-12 .statement tag=02X7}

Let $B = (e_i)_{i\in I}$ be an orthonormal basis of E. Let $u\in \mathscr{D}_B(E)$ and let us denote by $\lambda = (\lambda_i)_{i\in I}$ the family of its eigenvalues. The endomorphism $u$ is of finite trace if and only if the family $\lambda$ is summable in K. One then has Tr($u$) $=\sum\lambda_i$.

Replacing $u$ by $u_{(\mathbf{C})}$ if necessary, one may suppose that $K =\mathbf{C}$.

Suppose first that $u$ is of finite trace. According to EVT, V, p. 50 and p. 49, formula (25), the family $(\langle e_i|u(e_i)\rangle )_{i\in I}= (\lambda_i)_{i\in I}$ is summable.

Conversely, suppose that the family $\lambda$ is summable.

Each of the families $(\mathscr{R}(\lambda_i)^+), (\mathscr{R}(\lambda_i)^-), (\mathscr{I}(\lambda_i)^+), (\mathscr{I}(\lambda_i)^-)$ is then summable. The endomorphism $u$ is a linear combination of the elements of $\mathscr{D}_B(E)$ having these families as eigenvalues. These elements of $\mathscr{D}_B(E)$ are positive. Since, by definition, the space of endomorphisms of finite trace is generated by the positive endomorphisms of finite trace, one may therefore suppose that $\lambda_i\geqslant 0$ for every $i$. Since $\langle e_i|u(e_i)\rangle =\lambda_i$, the family $(\langle e_i|u(e_i)\rangle )_{i\in I}$ is summable, therefore $u$ is of finite trace (EVT, V, p. 48, lemma 3).

Finally, if $u$ is of finite trace, then according to EVT, V, p. 50, one has

Tr($u$) $=\sum_{i\in I}\langle e_i|u(e_i)\rangle =\sum_{i\in I}\lambda_i$.

#### Corollary 1 {#ts-iv-s1-prop-12-cor-1 .statement tag=02X8}

Let $u$ be an endomorphism of finite trace of E.

a) The endomorphism $u$ is compact;

b) Let $B = (e_i)_{i\in I}$ be an orthonormal basis of the initial space Ker($u$)$^{\circ}$ of $u$, $C = (f_i)_{i\in I}$ an orthonormal family in E, and $(\alpha_i)_{i\in I}$ a family in $(\mathbf{R}^*_+)^I$ such that $u(e_i) =\alpha_if_i$ for every $i\in I$ (cor. 2 of IV, p. 150). One has

Tr($u$) $=\sum_{i\in I}\alpha_i\langle e_i|f_i\rangle$.

To prove a), one may suppose that $K =\mathbf{C}$ (EVT, V, p. 50 and remark 4 of III, p. 2) and that $u$ is positive (EVT, V, p. 50, def. 8).

From EVT, V, p. 56, cor. 1, there exists an orthonormal basis $B = (e_i)_{i\in I}$ of E such that $u$ is diagonal in the basis B and moreover the family $\lambda$ of eigenvalues of $u$ belongs to $\mathbf{R}^I_+$ and is summable. The family $\lambda$ therefore belongs to $\mathscr{C}_0(I; K)$ (TG, III, p. 38, prop. 1), and consequently the endomorphism $u$ is compact (prop. 2 of IV, p. 148).

Let us prove b). Let $(e_i)_{i\in J}$ be an orthonormal basis of E extending the family B, so that $u(e_i) = 0$ if $i\in J$ - I. Then

Tr($u$) $=\sum_{i\in J}\langle e_i|u(e_i)\rangle =\sum_{i\in I}\langle e_i|u(e_i)\rangle =\sum_{i\in I}\alpha_i\langle e_i|f_i\rangle$.

#### Corollary 2 {#ts-iv-s1-prop-12-cor-2 .statement tag=02X9}

Let F be a Hilbert space. Let $u\in \mathscr{L}(E; F)$ be a Hilbert-Schmidt mapping. Then $u$ is a compact linear mapping.

Let $(j,|u|)$ be the polar decomposition of $u($I, p. 140, def. 4). By definition (EVT, V, p. 50, def. 9) the endomorphism $u^*u$ is of finite trace,$\surd$ hence is compact (corollary 1, a)); the same is true of $|u|=u^*u$ (prop. 6 of III, p. 91, b)) and of $u=j|u|$ (prop. 3 of III, p. 5).

#### Corollary 3 {#ts-iv-s1-prop-12-cor-3 .statement tag=02XA}

Suppose that $K =\mathbf{C}$. Let $u$ be a positive compact endomorphism of E. The endomorphism $u$ is of finite trace if and only if the decreasing family of its eigenvalues $(\lambda_n(u))_{n\in I_E}$ is summable; the trace of $u$ is then the sum of this family.

According to th. 1 of IV, p. 149, this follows from the preceding proposition and from the definition of the sequence $(\lambda_n(u))_{n\in I_E}$ (No$^o3$ of IV, p. 151), taking account of formula (28) of EVT, V, p. 49.

#### Corollary 4 {#ts-iv-s1-prop-12-cor-4 .statement tag=02XB}

Let F be a Hilbert space. Let $u\in \mathscr{L}(E; F)$ be a compact linear mapping. Let $B = (e_i)_{i\in I}$ be an orthonormal basis of the initial space Ker($u$)$^{\circ}$ of $u$, $C = (f_i)_{i\in I}$ an orthonormal family in F, and $(\alpha_i)_{i\in I}$ a family in $(\mathbf{R}^*_+)^I$ such that $u(e_i) =\alpha_if_i$ for every $i\in I$ (cor. 2 of IV, p. 150).

The endomorphism $|u|$ of E is of finite trace if and only if the family $(\alpha_i)_{i\in I}$ is summable. One then has $u\in \mathscr{L}_2(E; F)$ and

(8) Tr($|u|$) $=\sum_{i\in I}\alpha_i,\|u\|^2_2=$ Tr($u^*u$) $=\sum_{i\in I}\alpha^2_i$,

and in particular $\|u\|_2\leqslant$ Tr($|u|$).

The family of non-zero eigenvalues of $|u|$ is $(\alpha_i)_{i\in I}$, hence $|u|$ is of finite trace if and only if the family $(\alpha_i)_{i\in I}$ is summable (Prop. 12). If this is so, the family $(\alpha^2_i)$ of non-zero eigenvalues of $u^*u=|u|^2$ is summable, and formulas (8) result from loc. cit.

#### Lemma 7 {#ts-iv-s1-lem-7 .statement tag=02XC}

Let $\lambda = (\lambda_i)_{i\in I}$ be a family of complex numbers. For each $t\in \mathbf{C}^*$, let $n_t$ be the cardinal of the set of $i\in I$ such that $\lambda_i=t$. The family $(\lambda_i)_{i\in I}$ is summable if and only if $n_t$ is finite for each $t\in \mathbf{C}^*$ and the family $(n_tt)_{t\in\mathbf{C}^*}$ is summable. In this case, the sums of these two families are equal.

Suppose that the family $(\lambda_i)_{i\in I}$ is summable. For each $t\in \mathbf{C}$, let $I_t$ be the set of $i\in I$ such that $\lambda_i=t$. By TG, III, p. 39, Theorem 2, applied to the partition of I by the sets $I_t$, the set $I_t$ is finite for each $t\in \mathbf{C}^*$, and moreover the family $(n_tt)_{t\in\mathbf{C}^*}$ is summable, with sum equal to that of the family $(\lambda_i)_{i\in I}$.

Conversely, suppose that $n_t$ is finite for each $t\in \mathbf{C}^*$ and that the family $(n_tt)_{t\in\mathbf{C}^*}$ is summable. Let J be a finite subset of I and Λ the set of the $\lambda_i$ for $i\in J$. We have

$$
|\sum_{i\in J}\lambda_i|\leqslant \sum_{t\in\Lambda-\{0\}}n_t|t|\leqslant \sum_{t\in\mathbf{C}^*}n_t|t|
$$

hence the family $(\lambda_i)_{i\in I}$ is summable (TG, VII, p. 17, corollary).

#### Proposition 13 {#ts-iv-s1-prop-13 .statement tag=02XD}

Suppose that $K =\mathbf{C}$. Let $u$ be a compact normal endomorphism of E. For $t\in$ Sp$_s(u)$, let $n_t\geqslant 1$ be the spectral multiplicity of the eigenvalue $t$ of $u$. In order that $u$ be of finite trace, it is necessary and sufficient that the family $(n_tt)_{t\in Sp_s(u)}$ be summable. The trace of $u$ is then the sum of this family.

Let $B = (e_i)_{i\in I}$ be an orthonormal basis of E such that $u$ is diagonal in the basis B (Theorem 1 of IV, p. 149), and let $\lambda = (\lambda_i)_{i\in I}$ be the family of its eigenvalues. Since, for $t\in$ Sp$_s(u)$, the multiplicity $n_t$ is equal to the number of elements $i\in I$ such that $\lambda_i=t$, and since the non-zero elements of $\lambda$ belong to Sp$_s(u)$, the assertion then results from Prop. 12 and the preceding lemma.

### 8. Nuclear mappings

In this No., F denotes a Hilbert space over K. When $K =\mathbf{C}$, we recall (I, p. $139\surd$, Def. 3) that for $u\in \mathscr{L}(E; F)$, $|u|$ denotes the positive endomorphism $u^*\circ u$ of E. When $K =\mathbf{R}$, the element $|u_{(\mathbf{C})}|$ of $\mathscr{L}(E_{(\mathbf{C})})$ is of the form $v_{(\mathbf{C})}$ for a unique endomorphism $v\in \mathscr{L}$ (E), which is again denoted by $|u|($cf. I, p. 87).

We denote by $(u, v)\mapsto  \langle u|v\rangle =$ Tr($u^*v$) the scalar product in the Hilbert space $\mathscr{L}_2(E; F)$ (EVT, V, p. 53, Remarks 1 and 2).

For every $u\in \mathscr{L}(E; F)$, we put $\|u\|_1=$ Tr($|u|$) if $|u|$ is of finite trace and $\|u\|_1= +\infty$ if this is not the case. Thus $\|u\|_1\in \mathbf{R}_+\cup \{+\infty \}$. Since $\|u\|=\| |u| \|$ (Prop. 10, a) of I, p. 139) and if $v$ is positive and of finite trace, then Tr($v$)$\geqslant \|v\|$ (EVT, V, p. 49, formula (24bis) and p. 44, Prop. 9), it follows that

$$
\|u\|\leqslant \|u\|_1 \tag{9}
$$

If $\|u\|_1$ is finite, then $u$ is a Hilbert-Schmidt mapping and $\|u\|_2\leqslant \|u\|_1$ (Cor. 4 of IV, p. 165).

#### Proposition 14 {#ts-iv-s1-prop-14 .statement tag=02XE}

Let $u\in \mathscr{L}_2(E; F)$. Then

$\|u\|_1=$ sup$_{v\in\mathscr{L}_2(E;F)}|\langle v|u\rangle |$,

$\|v\|\leqslant 1$

the least upper bound being taken in $\mathbf{R}_+\cup  \{+\infty \}$.

Let $B = (e_i)_{i\in I}$ be an orthonormal basis of the initial space Ker($u$)$^{\circ}$ of $u, C = (f_i)_{i\in I}$ an orthonormal family in F and $(\alpha_i)_{i\in I}$ a family in $(\mathbf{R}^*_+)^I$ such that $u(e_i) =\alpha_if_i$ for every $i\in I$ (Cor. 2 of IV, p. 150). The family $(\alpha_i)_{i\in I}$ is square-summable since $u$ belongs to $\mathscr{L}_2(E; F)$ (Cor. 4 of IV, p. 165). Let $(e_j)_{j\in J}$ be an orthonormal basis of E extending $(e_i)_{i\in I}$.

Let L be a finite subset of I. Let $v_L$ be the continuous finite-rank linear mapping of E into F defined by

$$
v_L(x) =\sum_{i\in L}\langle e_i|x\rangle f_i
$$

for every $x$ in E. We have $\|v_L\|\leqslant 1$ and $v_L\in \mathscr{L}_2(E; F)$. Moreover, for every $j\in J$, we have $v_L(e_j) = 0$ if $j \notin L$ and $v_L(e_j) =f_j$ if $j\in L$. Thus

$|\langle v_L|u\rangle |=|$Tr($v^*_Lu$)$|=|\sum_{j\in J}\langle v_L(e_j)|u(e_j)\rangle |=\sum_{j\in L}\alpha_j$.

From loc. cit. we deduce that

(10) $\|u\|_1=$ sup$_L\sum_{j\in L}\alpha_j\leqslant$ sup$_{v\in\|\mathscr{L}v^2\|(E;F)\leqslant 1}|\langle v|u\rangle |$

in $\mathbf{R}_+\cup  \{+\infty \}$.

This implies the equality of the proposition when $\|u\|_1= +\infty$.

Suppose that $\|u\|_1$ is finite. For every $i\in I$, let $p_i$ be the linear mapping of E into F such that $p_i(e_i) =f_i$ and $p_i(x) = 0$ for every $x\in e^{\circ}_i$. For all $j$ and $k$ in I, one has

$\langle p_j|p_k\rangle =$ Tr($p^*_jp_k$) $=\sum_{i\in J}\langle p_j(e_i)|p_k(e_i)\rangle$,

which is zero unless $j=k$, in which case this quantity is $\|f_k\|^2= 1$. The family $(p_i)_{i\in I}$ is therefore orthonormal in $\mathscr{L}_2(E; F)$. Consequently, the family $(\alpha_ip_i)_{i\in I}$ is summable in $\mathscr{L}_2(E; F)$; its sum is equal to $u$ since these two continuous linear mappings coincide on the elements $e_i$ for every $i\in J$.

Let $v\in \mathscr{L}_2(E; F)$. For every $i\in I$, one has

$\langle v|p_i\rangle =$ Tr($v^*p_i$) $=\sum_{j\in J}\langle v(e_j)|p_i(e_j)\rangle =\langle v(e_i)|f_i\rangle$.

If $\|v\|\leqslant 1$, one then obtains the estimate

$$
|\langle v|u\rangle |=|\langle v|\sum_{i\in I}\alpha_ip_i\rangle |\leqslant \sum_{i\in I}\alpha_i|\langle v|p_i\rangle |
$$

$=\sum_{i\in I}\alpha_i|\langle v(e_i)|f_i\rangle |\leqslant \sum_{i\in I}\alpha_i=$ Tr($|u|$),

whence the inequality

sup$_{v\in\|\mathscr{L}v^2\|(E;F)\leqslant 1}|\langle v|u\rangle |\leqslant \|u\|_1$,

which, combined with formula (10), completes the proof of the proposition.

It follows from this proposition that the set $\mathscr{L}_1(E; F)$ of continuous linear mappings $u$ of E into F such that $\|u\|_1$ is finite is a vector subspace of $\mathscr{L}_2(E; F)$ and that the mapping $u\mapsto  \|u\|_1$ is a semi-norm on $\mathscr{L}_1(E; F)$; inequality (9) shows that it is a norm.

#### Definition 4 {#ts-iv-s1-def-4 .statement tag=02XF}

One says that the vector space $\mathscr{L}_1(E; F)$ endowed with the norm $u\mapsto  \|u\|_1$ is the space of nuclear mappings of E into F. If $u\in \mathscr{L}_1(E; F)$, one says that $u$ is nuclear.

#### Remark 1 {#ts-iv-s1-n8-rem-1 .statement tag=02XG}

Suppose that $K =\mathbf{R}$. Let $u\in \mathscr{L}(E; F)$. One has $u\in \mathscr{L}_1(E; F)$ if and only if $u_{(\mathbf{C})}\in \mathscr{L}_1(E_{(\mathbf{C})}; F_{(\mathbf{C})})$; in this case, one has $\|u\|_1=\|u_{(\mathbf{C})}\|_1$.

#### Remark 2 {#ts-iv-s1-n8-rem-2 .statement tag=02XH}

Let $u$ be a nuclear mapping of E into F. Since the mapping $u$ is of Hilbert–Schmidt type, it is compact (cor. 2 of IV, p. 165). Moreover, Proposition 14 implies that for every $v\in \mathscr{L}_2(E; F)$, one has

$$
|\langle v|u\rangle |\leqslant \|v\| \|u\|_1 \tag{11}
$$

#### Remark 3 {#ts-iv-s1-n8-rem-3 .statement tag=02XI}

Suppose that $K =\mathbf{C}$. Let $u\in \mathscr{L}_1(E; E)$ be such that $u$ is positive. The norm $\|u\|_1$ of $u$ is the sum of the sequence $(\lambda_n(u))_{n\in I_E}$ (cor. 3 of IV, p. 165).

#### Remark 4 {#ts-iv-s1-n8-rem-4 .statement tag=02XJ}

The canonical inclusion of $\mathscr{L}_1(E; F)$ in $\mathscr{L}(E; F)$ is of norm $\leqslant 1$ (inequality (9), p. 167).

#### Proposition 15 {#ts-iv-s1-prop-15 .statement tag=02XK}

Let G be a Hilbert space over K. The mapping $(u, v)\mapsto v\circ u$ of $\mathscr{L}(E; F)\times \mathscr{L}(F; G)$ into $\mathscr{L}(E; G)$ defines by passing to the subspaces a continuous bilinear mapping of norm $\leqslant 1$ of $\mathscr{L}_2(E; F)\times \mathscr{L}_2(F; G)$ into $\mathscr{L}_1(E; G)$.

Let $u\in \mathscr{L}_2(E; F)$ and $v\in \mathscr{L}_2(F; G)$. Let $w\in \mathscr{L}_2(E; G)$. We have $\langle uv|w\rangle =$ Tr($v^*u^*w$) $=\langle v|u^*w\rangle$ whence

$$
|\langle uv|w\rangle |\leqslant \|v\|_2\|u^*w\|_2\leqslant \|v\|_2\|u\|_2\|w\|
$$

by the Cauchy–Schwarz inequality and formula (37) of EVT, V, p 52. The result therefore follows from Prop. 14.

#### Lemma 8 {#ts-iv-s1-lem-8 .statement tag=02XL}

The mapping $u\mapsto u^*$ of $\mathscr{L}(E; F)$ into $\mathscr{L}(F; E)$ defines by passing to the subspaces an isometric linear mapping of $\mathscr{L}_1(E; F)$ into $\mathscr{L}_1(F; E)$.

Let $u\in \mathscr{L}_1(E; F)$. Since $u$ is a Hilbert–Schmidt mapping, the same is true of $u^*$ (EVT, V, p. 54). The mapping $v\mapsto v^*$ is a bijection of the set of $v\in \mathscr{L}_2(E; F)$ such that $\|v\|\leqslant 1$ onto the set of $w\in \mathscr{L}_2(F; E)$ such that $\|w\|\leqslant 1$; for every $v\in \mathscr{L}_2(E; F)$ with $\|v\|\leqslant 1$, one has $\langle v|u\rangle =\langle u^*|v^*\rangle$ (EVT, V, p. 54, formula (42)), whence the result by Prop. 14.

#### Proposition 16 {#ts-iv-s1-prop-16 .statement tag=02XM}

Let $E_1$ and $F_1$ be Hilbert spaces. Let $u$ be in $\mathscr{L}_1(E; F),v$ be in $\mathscr{L}(E_1; E)$ and $v_2$ be in $\mathscr{L}(F; F_1)$. Then $v_2uv_1\in \mathscr{L}_1(E_1; F_1)$ and $\|v_2uv_1\|_1\leqslant \|v_2\| \|v_1\| \|u\|_1$.

Let $w\in \mathscr{L}_2(E; F_1)$ such that $\|w\|\leqslant 1$. One has $v_2u\in \mathscr{L}_2(E; F_1)$ (EVT, V, p. 52, formula (36)). Since $v^*_2w\in \mathscr{L}_2(E; F) ($loc. cit.), it follows that

$$
|\langle w|v_2u\rangle |=|\langle v^*_2w|u\rangle |\leqslant \|v_2\| \|u\|_1
$$

(formula (11)), whence $v_2u\in \mathscr{L}_1(E; F_1)$ and $\|v_2u\|_1\leqslant \|v_2\|\|u\|_1$ (Prop. 14).

Let $v_1\in \mathscr{L}(E_1; E)$; since $uv_1= (v^*_1u^*)^*$, one has $uv_1\in \mathscr{L}_1(E_1; F)$ and $\|uv_1\|_1\leqslant \|v^*_1\| \|u^*\|_1=\|v_1\| \|u\|_1$ (Lemma 8).

The proposition follows at once from these inequalities.

#### Proposition 17 {#ts-iv-s1-prop-17 .statement tag=02XN}

The space $\mathscr{L}_1(E; E)$ coincides with the space $\mathscr{L}_1(E)$ of endomorphisms of finite trace of E, and one has $|$Tr($u$)$|\leqslant \|u\|_1$ for every endomorphism $u$ of E of finite trace.

We may suppose that $K =\mathbf{C}$. The space $\mathscr{L}_1(E; E)$ contains by definition the set of positive endomorphisms of finite trace, and therefore $\mathscr{L}_1(E)\subset \mathscr{L}_1(E; E)$ (EVT, p. 50, def. 8). Conversely, let us prove that $\mathscr{L}_1(E; E)$ is contained in $\mathscr{L}_1(E)$.

Let $u\in \mathscr{L}_1(E; E)$. We have $u^*\in \mathscr{L}_1(E; E)$ (lemma 8); it is therefore enough to prove that the Hermitian elements of $\mathscr{L}_1(E; E)$ are of finite trace (lemma 2 of I, p. 96).

Let $u$ be such an endomorphism. It is compact (remark 2, p. 169). Let B be an orthonormal basis of E such that $u$ is diagonal in the basis B (Theorem 1 of IV, p. 149), and let $\lambda$ be the family of eigenvalues of $u$ relative to B. The endomorphism $|u|$ is diagonalizable in the basis B and the family of its eigenvalues is $|\lambda |$ (prop. 1, d) of IV, p. 147). Since $|u|$ is of finite trace, the latter family is summable (prop. 12 of IV, p. 164), hence the family $\lambda$ is summable. Consequently, $u$ is of finite trace (loc. cit.), and we have $|$Tr($u$)$|\leqslant$ Tr($|u|$) $=\|u\|_1$.

Consequently, the space $\mathscr{L}_1(E)$ is a self-adjoint two-sided ideal of the star-algebra $\mathscr{L}(E)$. If E is of infinite dimension, this ideal is not closed in $\mathscr{L}(E)$.

Propositions 17 and 16 prove that the bilinear form $b$ on $\mathscr{L}_1(E; F)\times \mathscr{L}(F; E)$ with values in $\mathbf{C}$ defined by $b(u, v) =$ Tr($vu$) is a continuous bilinear form which puts the spaces $\mathscr{L}_1(E; F)$ and $\mathscr{L}(F; E)$ in duality.

#### Lemma 9 {#ts-iv-s1-lem-9 .statement tag=02XO}

Let $u\in \mathscr{L}_1(E; F)$. We have

$\|u\|_1=$ sup$_{v\in\mathscr{L}_c(F;E)}|b(u, v)|$.

$\|v\|\leqslant 1$

Since every Hilbert-Schmidt mapping is compact (cor. 2 of IV, p. 165), we have

$\|u\|_1\leqslant$ sup$_{v\in\|\mathscr{L}v\|^c(E;F)\leqslant 1}|$Tr($vu$)$|=$ sup$_{v\in\mathscr{L}\|v^c\|(F;E)\leqslant 1}|b(u, v)|$

by prop. 14.

Let $v\in \mathscr{L}^c(E; F)$ be of norm $\leqslant$ 1. Since $\mathscr{L}_2(E; F)$ is dense in $\mathscr{L}^c(E; F)$, there exists a sequence $(v_n)_{n\in\mathbf{N}}$ in $\mathscr{L}_2(E; F)$ which converges to $v$ in $\mathscr{L}(E; F)$. The sequence $(b(u, v_n))_{n\in\mathbf{N}}$ converges to $b(u, v)$; since $|b(u, v_n)|$ = $|$Tr($v_nu$)$|$ = $|\langle v_n^*|u\rangle |\leqslant \|u\|_1$ (prop. 14) for every $n\in \mathbf{N}$, it follows that $|b(u, v)|\leqslant \|u\|_1$.

Let us denote by $\theta$ the continuous linear mapping

$$
\theta :\mathscr{L}_1(E; F)\rightarrow \mathscr{L}^c(F; E)'
$$

such that $\theta (u)(v) =b(u, v)$.

#### Proposition 18 {#ts-iv-s1-prop-18 .statement tag=02XP}

The mapping $\theta$ is an isometric isomorphism.

By lemma 9, the mapping $\theta$ is isometric, and it is enough to prove that $\theta$ is surjective.

Let $\lambda \in \mathscr{L}^c(F; E)'$. Since $\|v\|\leqslant \|v\|_2$ for every $v\in \mathscr{L}_2(F; E)$ (EVT, V, p. 52, formula (33)), the restriction of $\lambda$ to the subspace $\mathscr{L}_2(F; E)$ is a continuous linear form on the Hilbert space $\mathscr{L}_2(F; E)$. There therefore exists an element $u$ of $\mathscr{L}_2(F; E)$ such that $\lambda (v) =\langle u|v\rangle$ for every $v\in \mathscr{L}_2(F; E)$ (EVT, V, p. 15, th. 3).

For every $w\in \mathscr{L}_2(E; F)$ of norm $\leqslant 1$, we have $|\langle w|u\rangle |=|\lambda (w)|\leqslant \|\lambda \|$. Consequently, $u$ is a nuclear mapping from E into F (prop. 14).

The continuous linear forms $\lambda$ and $\theta (u)$ are equal on the dense subspace $\mathscr{L}_2(F,E)$ of $\mathscr{L}^c(F; E)$. It follows that $\lambda =\theta (u)$, which concludes the proof.

#### Corollary {#ts-iv-s1-n8-cor-1 .statement tag=02XQ}

The normed space $\mathscr{L}_1(E; F)$ is a Banach space.

The assertion follows from the proposition and from EVT, III, p. 24, cor. 2 since the space $\mathscr{L}^c(F; E)$ is a normed space.

### 9. Hilbert-Schmidt Integral Operators

In this No., X and Y are locally compact topological spaces. Let $\mu$ be a positive measure on X and $\nu$ a positive measure on Y. We denote by $L^2$(X), $L^2(Y)$ and $L^2(X\times Y)$ the spaces $L^2(X, \mu), L^2(Y, \nu )$ and $L^2(X\times Y, \mu\otimes \nu )$ respectively, and analogously for $\mathscr{L}^2$(X), $\mathscr{L}^2(Y)$ and $\mathscr{L}^2(X\times Y)$.

We recall (cf. No.$^o4$ of III, p. 26) that for every $N\in \mathscr{L}^2(X\times Y)$, there exists a unique continuous linear mapping $u_N$ from $L^2(X)$ into $L^2(Y)$ such that

$$
\langle g|u_N(f)\rangle =\int_{X\times Y}g(y)N(x, y)f(x)d(\mu\otimes \nu )(x, y) \tag{12}
$$

for every $f\in L^2(X)$ and every $g\in L^2(Y)$. The mapping $u_N$ is compact (cor. 1 of III, p. 33). The mapping $N\mapsto u_N$ induces by passing to the quotients a continuous injective linear mapping from $L^2(X\times Y)$ into $\mathscr{L}(L^2(X); L^2(Y))$ (prop. 5 of III, p. 30).

We denote by $\theta$ the unique linear mapping from $\mathscr{L}^2(X)\otimes \mathscr{L}^2(Y)$ into $\mathscr{L}^2(X\times Y)$ which to every $f\in \mathscr{L}^2(X)$ and every $g\in \mathscr{L}^2(Y)$ associates the function defined by $(x, y)\mapsto f(x)g(y)$.

#### Lemma 10 {#ts-iv-s1-lem-10 .statement tag=02XR}

The mapping $\theta$ defines by passing to quotients a linear mapping $\widetilde{\theta}$ from $L^2(X)\otimes L^2(Y)$ into $L^2(X\times Y)$, and there exists a unique isometric isomorphism from $L^2(X)\widehat{\otimes}_2L^2(Y)$ onto $L^2(X\times Y)$ which coincides with this one on $L^2(X)\otimes L^2(Y)$.

The first assertion is elementary. Let us prove the second.

Let $(f_i)_{i\in I}$ and $(g_j)_{j\in J}$ be orthonormal bases of $L^2(X)$ and $L^2$(Y), respectively. The family $(f_i\otimes g_j)_{(i,j)\in I\times J}$ is an orthonormal basis of $L^2(X)\widehat{\otimes}_2L^2(Y)$ (EVT, V, p. 29, cor. 1) and the family $(\widetilde{\theta}(\overline{f}_i\otimes g_j))_{(i,j)\in I\times J}$ is orthonormal in $L^2(X\times Y)$ (INT, V, p. 95, § 8, n$^o3$, cor. 2). The mapping $\widetilde{\theta}$ therefore extends by continuity to an isometric linear mapping from $L^2(X)\widehat{\otimes}_2L^2(Y)$ into $L^2(X\times Y)$. It remains to prove that this extension is surjective.

For this, it is enough to prove that the image of $\widetilde{\theta}$ is dense in $L^2(X\times Y)$. Let N be an element of $L^2(X\times Y)$ orthogonal to the image of $\widetilde{\theta}$. For all $i\in I$ and $j\in J$, one has $\langle g_j|u_N(f_i)\rangle =\langle \widetilde{\theta}(\overline{f}_i\otimes g_j)|N\rangle = 0$ (formula (12)), whence $u_N= 0$, and therefore N = 0.

The preceding lemma establishes the assertion stated in EVT, V, p. 29, example 2.

Henceforth we shall identify $L^2(X)\widehat{\otimes}_2L^2(Y)$ and $L^2(X\times Y)$ by means of the isometric isomorphism of Lemma 10.

#### Proposition 19 {#ts-iv-s1-prop-19 .statement tag=02XS}

The mapping $N\mapsto u_N$ is an isometric isomorphism of $L^2(X\times Y)$ onto the space $\mathscr{L}_2(L^2(X); L^2(Y))$ of mappings

of Hilbert–Schmidt deThe linear mapping of L$L^2(X)_2$into$(Y)\otimes L\overset{2}{L}(Y)_2(X)$ into. $\mathscr{L}_2(L^2(X); L^2(Y))$ which associates to $g\otimes f$ the Hilbert–Schmidt mapping $h\mapsto  \langle f|h\rangle g$ extends to an isometric isomorphism $\theta_1$ of $L^2(Y)\widehat{\otimes}_2L^2(X)$ onto $\mathscr{L}_2(L^2(X); L^2(Y))$ (EVT, V, p. 52, th. 1).

Let us denote moreover by $\theta_2$ the isometric isomorphism of $L^2(X)\widehat{\otimes}_2L^2(Y)$ onto $L^2(Y)\widehat{\otimes}_2L^2(X)$ which to $f\otimes g$ associates $g\otimes \overline{f}$ for every $f\in L^2(X)$ and every $g\in L^2(Y)$.

The linear mapping $\theta_3=\theta_1\circ \theta_2$ is identified with an isometric isomorphism of $L^2(X\times Y)$ onto $\mathscr{L}_2(L^2(X); L^2(Y))$.

Let $f\in L^2(X)$ and $g\in L^2$(Y), and let N be the element of $L^2(X\times Y)$ identified with $f\otimes g$. From INT, V, p. 95, § 8, n$^o3$, cor. 2 and formula (12) one has

$$
\langle g_1|u_N(f_1)\rangle =\langle \overline{f}|f_1\rangle  \langle g_1|g\rangle
$$

for all $f_1\in L^2(X)$ and $g_1\in L^2(Y)$. The mapping $u=\theta_3(N)$ is the linear mapping $\theta_1(g\otimes f)$; it therefore satisfies $u(h) =\langle f|h\rangle g$ for all $h\in L^2(X)$. Consequently, for all $f_1\in L^2(X)$ and $g_1\in L^2$(Y), one has

$$
\langle g_1|u(h_1)\rangle =\langle \overline{f}|h_1\rangle  \langle g_1|g\rangle =\langle g_1|u_N(h_1)\rangle
$$

whence $\theta_3(N) =u_N$. Since $\theta_3$ and $N\mapsto u_N$ are continuous, it follows that $\theta_3(N) =u_N$ for all $N\in L^2(X\times Y)$, which completes the proof.

#### Corollary {#ts-iv-s1-n9-cor-1 .statement tag=02XT}

For every $N\in L^2(X\times Y)$, the linear mapping $u_N$ is a Hilbert–Schmidt mapping and one has Tr($u^*_Nu_N$) $=\|N\|^2$.

In fact, one has $\|u\|_2=\surd$Tr($u^*u$) for all $u\in \mathscr{L}_2(L^2(X); L^2(Y))$.

#### Remark {#ts-iv-s1-n9-rem-1 .statement tag=02XU}

Let $N\in L^2(X\times Y)$. By corollary 2 of IV, p. 150, there exist a countable set I, orthonormal families $(f_i)_{i\in I}$ in $L^2(X)$ and $(g_i)_{i\in I}$ in $L^2$(Y), as well as a family $(\alpha_i)_{i\in I}$ in $\mathbf{R}^*_+$, such that

$$
u_N(f) =\sum_{i\in I}\alpha_i\langle f_i|f\rangle g_i
$$

for all $f\in L^2$(X), where the series converges in $L^2(Y)$. By cor. 4 of IV, p. 165 and the above corollary, one has

$\sum_{i\in I}\alpha^2_i=$ Tr($u^*_Nu_N$) $=\|u_N\|^2_2=\int_{X\times Y}|N(x, y)|^2d(\mu\otimes \nu )(x, y)$.

Let us further set $h_{i,j}=\overline{f}_i\otimes g_j\in L^2(X\times Y)$ for all $(i, j)\in I\times I$. One then has

$$
N =\sum_{i\in I}\alpha_ih_{i,i}
$$

in $L^2(X\times Y)$.

In fact, let $(f_j)_{j\in J}$ and $(g_k)_{k\in K}$ be orthonormal bases of $L^2(X)$ and $L^2$(Y), respectively, extending the families $(f_i)_{i\in I}$ and $(g_i)_{i\in I}$. Set $h_{j,k}=\overline{f}_j\otimes g_k$ for all $(j, k)\in J\times K$. By lemma 10, the family $(h_{j,k})_{(j,k)\in J\times K}$ is an orthonormal basis of $L^2(X\times Y)$. One has $\langle h_{j,k}|N\rangle =\langle g_k|u_N(f_j)\rangle$ for all $(j, k)\in J\times K$. If $j \notin I$, this quantity is zero. If $j\in I$, it is equal to $\alpha_j\langle g_k|g_j\rangle$, hence is zero unless $k=j$, in which case $\langle h_{j,j}|N\rangle =\alpha_j$. Consequently

$$
N =\sum_{(j,k)\in J\times K}\langle h_{j,k}|N\rangle h_{j,k}=\sum_{i\in I}\alpha_ih_{i,i}
$$

### 10. Trace of integral operators with continuous kernel

In this number, the conventions of the preceding number are retained with Y = X and $\nu =\mu$. It is assumed that X is a locally compact topological space countable at infinity (TG, I, p. 68, Def. 5).

In particular, one identifies the spaces $L^2(X\times X)$ and $L^2(X)\widehat{\otimes}_2L^2(X)$ (lemma 10 of IV, p. 172). We shall denote by $\widetilde{f}$ the class in $L^2(X)$ (resp. in $L^2(X\times X)$) of a function $f\in \mathscr{L}^2(X)$ (resp. in $\mathscr{L}^2(X\times X)$).

#### Proposition 20 {#ts-iv-s1-prop-20 .statement tag=02XV}

Let $(f_n)_{n\in\mathbf{N}}$ be a sequence of measurable mappings of X into a metrisable space F. Suppose that the limit of $f_n(x)$ exists in the complement of a $\mu$-negligible subset of X. There exists a sequence $(C_m)_{m\in\mathbf{N}}$ of compact subsets of X whose union $\widetilde{X}$ satisfies $|\mu|(X-\widetilde{X}) = 0$, such that the functions $f_n$ are continuous on $C_m$ for all $n\in \mathbf{N}$ and all $m\in \mathbf{N}$, and the sequence $(f_n)_{n\in\mathbf{N}}$ converges uniformly to $f$ on $C_m$ for all $m\in \mathbf{N}$.

It follows from theorem 2 of INT, IV, p. 175, § 5, n$^o4$ and proposition 12, b) of INT, IV, p. 188, § 5, n$^o8$, that the set of compact subsets C of X such that the functions $f_n$ are continuous on C for all $n$, and that $(f_n)$ converges uniformly to $f$ on C, is $\mu$-dense in X (INT, IV, p. 189, § 5, n$^o8$, definition 6). The assertion then follows from the remark in INT, IV, p. 189, §5, n$^o8$.

Let N be a function belonging to $\mathscr{L}^2(X\times X)$ and let $u_N$ be the Hilbert-Schmidt mapping of $L^2(X)$ into $L^2(X)$ with kernel N (proposition 19 of IV, p. 173). Since the mapping $u_N$ is compact, there exist by proposition 9 of IV, p. 156 an element M of $\mathbf{N}$ and, denoting by I the set of integers $n\in \mathbf{N}$ such that $n\leqslant M$, orthonormal families $(f_i)_{i\in I}$ and $(g_i)_{i\in I}$ in $\mathscr{L}^2(X)$ and a family $(\alpha_i)_{i\in I}$ in $\mathbf{R}^*_+$ such that

$$
u_N(f) =\sum_{i\in I}\alpha_i\langle \widetilde{f}_i|f\rangle \widetilde{g}_i \tag{13}
$$

for all $f\in L^2$(X), where the series converges in $L^2(X)$.

For each $i\in I$, let $h_i\in \mathscr{L}^2(X\times X)$ denote the function defined by $h_i(x, y) =f_i(x)g_i(y)$, so that $\widetilde{h}_i$ is the class of $f_i\otimes g_i$. By remark 9 of IV, p. 173, the series with general term $\alpha_ih_i$ converges to N in $L^2(X\times X)$.

In the remainder of this number, we suppose that N is a continuous function.

#### Proposition 21 {#ts-iv-s1-prop-21 .statement tag=02XW}

Suppose that $u_N$ is of finite trace. Then there exist a set $\widetilde{X}\subset X$ whose complement X $-\widetilde{X}$ is $\mu$-negligible and a function $H\in \mathscr{L}^2(X\times X)$ satisfying the following conditions :

(i) For every $(x, y)\in \widetilde{X}\times \widetilde{X}$, the family $(\alpha_if_i(x)g_i(y))_{i\in I}$ is summable in $\mathbf{C}$ and its sum is $N(x, y)$;

(ii) For every finite subset J of I and every $(x, y)\in \widetilde{X}\times \widetilde{X}$, one has

$$
|\sum_{i\in J}\alpha_ih_i(x, y)|\leqslant H(x, y) \tag{14}
$$

(iii) The function $x\mapsto H(x, x)$ belongs to $\mathscr{L}^1(X)$.

Since $u_N$ is of finite trace, the family $(\alpha_i)$ is summable (cor. 4 of IV, p. 165). The series

$$
\sum_{i\in I}\alpha_i|f_i|^2,\sum_{i\in I}\alpha_i|g_i|^2
$$

therefore converge in $\mathscr{L}^1(X)$ and consequently $\mu$-almost everywhere (INT, IV, p. 128, § 3, n$^o3$, prop. 6). Let F and G denote, respectively, the functions defined $\mu$-almost everywhere by the sum of these series, putting $F(x) = 0$ and $G(x) = 0$ for every $x$ such that the corresponding series does not converge. Since F and G belong to $\mathscr{L}^1$(X), the function H defined by $H(x, y) =\surd F(x)G(y)$ belongs to $\mathscr{L}^2(X\times X)$ (INT, V, p. 95, § 8, n$^o3$, cor. 2).

Let us apply prop. 20 to the space X, to $F =\mathbf{C}^2$, and to the measurable mappings

$$
s_n:x\mapsto (\sum_{i\in I}\alpha_i|f_i(x)|^2,\sum_{i\in I}\alpha_i|g_i(x)|^2)
$$

$i\leqslant ni\leqslant n$

defined on X. There therefore exists a sequence $(C_m)_{m\in\mathbf{N}}$ of compact subsets of X satisfying the following conditions:

(1) the union $\widetilde{X}$ satisfies $\mu(X-\widetilde{X}) = 0$;

(2) for every $m\in \mathbf{N}$ and every $n\in \mathbf{N}$, the functions $s_n$ are continuous on $C_m$;

(3) for every $m\in \mathbf{N}$, the series $\sum\alpha_i|f_i|^2$ and $\sum\alpha_i|g_i|^2$ converge uniformly on $C_m$ to F and G, respectively;

(4) the support of the measure induced by $\mu$ on $C_m$ is equal to $C_m$ (replacing $C_m$ by the support of this measure if necessary).

Let us prove that the set $\widetilde{X}$ and the function H satisfy conditions (i), (ii), and (iii).

Let $(x, y)\in \widetilde{X}\times \widetilde{X}$. For every finite subset $J\subset I$, one has

$$
|\sum_{i\in J}\alpha_i\overline{f_i(x)}g_i(y)|\leqslant (\sum_{i\in J}\alpha_i|f_i(x)|^2)^{1/2}(\sum_{i\in J}\alpha_i|g_i(y)|^2)^{1/2} \tag{15}
$$

whence also

$$
|\sum_{i\in J}\alpha_i\overline{f_i(x)}g_i(y)|\leqslant H(x, y) \tag{16}
$$

which already establishes property (ii).

By inequality (15), the series $\sum_i\alpha_ih_i$ converges uniformly on $K_m\times K_n$ for every $(m, n)\in \mathbf{N}^2$. Let $\widetilde{N}$ be the function on $X\times X$ defined by

$$
\widetilde{N}(x, y) =\sum_{i\in I}\alpha_ih_i(x, y) =\sum_{i\in I}\alpha_i\overline{f_i(x)}g_i(y)
$$

for every $(x, y)\in \widetilde{X}\times \widetilde{X}$ and by $\widetilde{N}(x, y) = 0$ otherwise. The function $\widetilde{N}$ is measurable (INT, IV, p. 175, § 5, n$^o4$, th. 2), and it is continuous on $K_m\times K_n$ for every $(m, n)\in \mathbf{N}^2$.

From (16), we have $|\widetilde{N}(x, y)|\leqslant H(x, y)$ for all $(x, y)\in X\times X$, and in particular $\widetilde{N}$ belongs to $\mathscr{L}^2(X\times X)$ (INT, IV, p. 84, § 5, n$^o6$, th. 5).

Let us prove that $N =\widetilde{N}$ on $\widetilde{X}\times \widetilde{X}$, which will establish property (i). Let $f$ and $g$ be elements of $\mathscr{L}^2(X)$. We have

$$
\langle g|u_{\widetilde{N}}(f)\rangle =\int_{X\times X}\widetilde{N}(x, y)f(x)\overline{g(y)}d(\mu\otimes \mu)(x, y)
$$

(formula (12) of IV, p. 172). For all $(x, y)\in \widetilde{X}\times \widetilde{X}$ and every finite subset J of I, we have

$$
|\sum_{i\in J}\alpha_i\overline{f_i(x)}g_i(y)f(x)\overline{g(y)}|\leqslant |f(x)g(y)|H(x, y)
$$

by formula (16). Since the right-hand side of this inequality is integrable on $X\times X$ (INT, V, p. 95, § 8, n$^o3$, cor. 2), we may apply Lebesgue's theorem (INT, IV, p. 137, § 3, n$^o7$, th. 6) and formula (13), and deduce that

$$
\langle g|u_{\widetilde{N}}(f)\rangle =\sum_{i\in I}\alpha_i\int_{X\times X}\overline{f_i(x)}g_i(y)f(x)\overline{g(y)}d(\mu\otimes \mu)(x, y)
$$

$$
=\sum_{i\in I}\alpha_i\langle f_i|f\rangle \langle g|g_i\rangle =\langle g|u_N(f)\rangle
$$

Consequently, we obtain $u_{\widetilde{N}}=u_N$, whence $N =\widetilde{N}$ in $L^2(X\times X)$ (prop. 3 of III, p. 28, b)).

For all $(m, n)\in \mathbf{N}^2$, the functions N and $\widetilde{N}$ are continuous on $K_m\times K_n$ and therefore are equal on $K_m\times K_n$ (prop. 9 of INT, III, p. 69, § 2, n$^o2$), since the support of the measure induced by $\mu\otimes \mu$ on $K_m\times K_n$ is equal to $K_m\times K_n$. Hence N coincides with $\widetilde{N}$ on $\widetilde{X}\times \widetilde{X}$.

$$
\surd
$$

Finally, the estimate FG $\leqslant (F + G)/2$ implies that the function $x\mapsto \surd F(x)G(x) = H(x, x)$ is integrable on X, whence property (iii).

In the rest of this number, we retain the notation of the proposition.

#### Theorem 2 {#ts-iv-s1-thm-2 .statement tag=02XX}

Suppose that $u_N$ is of finite trace. Then the function $x\mapsto N(x, x)$ belongs to $\mathscr{L}^1(X)$ and we have

Tr($u_N$) $=\int_XN(x, x)d\mu(x)$.

From conditions (i) and (ii), we have $|N(x, x)|\leqslant H(x, x)$ for $x\in \widetilde{X}$, therefore the function $x\mapsto N(x, x)$ belongs to $\mathscr{L}^1(X)$ by condition (iii).

Condition (i) establishes the equality

$$
N(x, x) =\sum_{i\in I}\alpha_i\overline{f_i(x)}g_i(x)
$$

for all $x\in \widetilde{X}$. From conditions (ii) and (iii), we may apply Lebesgue's theorem (INT, IV, p. 137, § 3, n$^o7$, th. 6), from which it follows that

$$
\int_XN(x, x)d\mu(x) =\sum_{i\in I}\alpha_i\int_X\overline{f_i(x)}g_i(x)d\mu(x)
$$

$=\sum_{i\in I}\alpha_i\langle f_i|g_i\rangle =$ Tr($u_N$),

the last equality resulting from the cor. of prop. 17 of IV, p. 170.

#### Lemma 11 {#ts-iv-s1-lem-11 .statement tag=02XY}

If the endomorphism $u_N$ of $L^2(X)$ is positive, then $N(x, x)\geqslant 0$ for every $x$ in the support of $\mu$.

Since $u_N$ is positive, the families $(f_i)$ and $(g_i)$ may be chosen in such a way that $f_i=g_i$ for all $i\in I$ (remark 3 of IV, p. 151). For all $x\in \widetilde{X}$, we then have

$$
N(x, x) =\sum_{i\in I}\alpha_i|f_i(x)|^2\geqslant 0
$$

Since N is continuous, and $\mu(X-\widetilde{X}) = 0$, the function N is positive on the support of $\mu$.

#### Remark {#ts-iv-s1-n10-rem-1 .statement tag=02XZ}

The converse assertion of the lemma is not valid (exercise 14 of IV, p. 316).

#### Proposition 22 {#ts-iv-s1-prop-22 .statement tag=02Y0}

Suppose that $u_N$ is a positive endomorphism of $L^2(X)$. Then the endomorphism $u_N$ is of finite trace if and only if the function $x\mapsto N(x, x)$ is $\mu$-integrable. In that case, one has

Tr($u_N$) $=\int_XN(x, x)d\mu(x)$.

If $u_N$ is of finite trace, Theorem 2 implies that $x\mapsto N(x, x)$ is integrable on X and that its integral is the trace of $u_N$.

Conversely, suppose that the function $x\mapsto N(x, x)$ is integrable. Since $u_N$ is positive, the orthonormal families $(f_i)_{i\in I}$ and $(g_i)_{i\in I}$ can be chosen so that $f_i=g_i$ for all $i\in I$ (remark 3 of IV, p. 151). For every $x\in \widetilde{X}$, one has

$$
N(x, x) =\sum_{i\in I}\alpha_i|f_i(x)|^2
$$

whence, for every finite subset J of I, one deduces

$$
\sum_{i\in J}\alpha_i=\sum_{i\in J}\alpha_i\int_X|f_i(x)|^2d\mu(x)
$$

$$
=\int_X\sum_{i\in J}\alpha_i|f_i(x)|^2d\mu(x)\leqslant \int_XN(x, x)d\mu(x)
$$

The family $(\alpha_i)_{i\in I}$ is therefore summable, which implies that the endomorphism $u_N$ is of finite trace (prop. 12 of IV, p. 164).

#### Remark {#ts-iv-s1-n10-rem-2 .statement tag=02Y1}

Even when X is compact and N continuous, the endomorphism $u_N$ of $L^2(X)$ is not always of finite trace (cf. exercise 8 of IV, p. 314).

## EXERCISES {#ts-iv-s1-exercises}

See the [exercises for § 1](exercises/s1/).
