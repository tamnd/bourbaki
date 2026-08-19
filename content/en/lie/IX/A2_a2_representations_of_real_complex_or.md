---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 2
section_title: Representations of real, complex or quaternionic type
appendix: true
lang: en
source: lie-vii-ix
book_pages: 385-388
pdf_pages: 0392-0395
extraction: native
subsections:
    - "no": 1
      title: REPRESENTATIONS OF REAL ALGEBRAS
      page: 385
      pdf_page: 392
    - "no": 2
      title: REPRESENTATIONS OF COMPACT GROUPS
      page: 387
      pdf_page: 394
statements: 6
exercises: 0
content_sha256: b1abe927440628b085d7a372f483b3d90c467463452fcb1aefa24f60c64818f0
---

## APPENDIX II

# REPRESENTATIONS OF REAL, COMPLEX OR QUATERNIONIC TYPE

### 1. REPRESENTATIONS OF REAL ALGEBRAS

Denote by $\sigma$ the automorphism $\alpha  \rightarrow \overline{\alpha}$ of $\mathbf{C}$; if W is a complex vector space, denote by W the $\mathbf{C}$-vector space $\sigma_*(W)$ (that is, the group W with the law of operation $(\alpha , w) \rightarrow \overline{\alpha w}$ for $\alpha \in \mathbf{C}, w\in W$).

#### Proposition 1 {#lie-ix-a2-prop-1 .statement tag=01IS}

Let A be an $\mathbf{R}$-algebra (associative and unital) and V a finite dimensional simple A-module over $\mathbf{R}$. Then, we must be in one of the following three situations:

$\alpha )$ The commutant of V (Algebra, Chap. VIII, § 5, no. 1) is isomorphic to $\mathbf{R}$, and the $A_{(\mathbf{C})}$-module $V_{(\mathbf{C})}$ is simple;

$\beta )$ the commutant of V is isomorphic to $\mathbf{C}$; the $A_{(\mathbf{C})}$-module $V_{(\mathbf{C})}$ is the direct sum of two non-isomorphic simple $A_{(\mathbf{C})}$-submodules which are interchanged by $\sigma \otimes 1_V$;

$\gamma )$ the commutant of V is isomorphic to $\mathbf{H}$; the $A_{(\mathbf{C})}$-module $V_{(\mathbf{C})}$ is the direct sum of two isomorphic simple $A_{(\mathbf{C})}$-submodules that are interchanged by $\sigma \otimes 1_V$.

The commutant E of V is a field, a finite extension of $\mathbf{R}($Algebra, Chap. VIII, §3, no. 2, Prop. 2), hence isomorphic to $\mathbf{R},\mathbf{C}$ or $\mathbf{H}($Algebra, Chap. VIII, §15). The $A_{(\mathbf{C})}$-module $V_{(\mathbf{C})}$ is semi-simple (Algebra, Chap. VIII, §11, no. 4), and its commutant can be identified with $\mathbf{C}\otimes_{\mathbf{R}}E ($Algebra, Chap. VIII, §11, no. 2, Lemma 1).

If E is isomorphic to $\mathbf{R}$, the commutant of $V_{(\mathbf{C})}$ is isomorphic to $\mathbf{C}$, and $V_{(\mathbf{C})}$ is a simple $A_{(\mathbf{C})}$-module (Algebra, Chap. VIII, §11, no. 4).

If E is not isomorphic to $\mathbf{R}$, it contains a field isomorphic to $\mathbf{C}$; it follows that V has an $A_{(\mathbf{C})}$-module structure, denoted by $V^c$. Then $V^c$ is a simple $A_{(\mathbf{C})}$-module, and the $\mathbf{C}$-linear map $\psi : V_{(\mathbf{C})}\rightarrow V^c\oplus \overline{V}^c$ such that $\psi (\alpha \otimes v) =$ $(\alpha v,\overline{\alpha v})$ for $\alpha \in \mathbf{C},v\in V$, is an isomorphism (Algebra, Chap. V, §10, no. 4, Prop. 8). Moreover, $\sigma \otimes 1_V$ corresponds under this isomorphism to the $\mathbf{R}$-automorphism $(v, v') \rightarrow (v', v)$ of $V^c\oplus \overline{V}^c$, and hence interchanges the two $A_{(\mathbf{C})}$-submodules $\psi^{-1}(V^c)$ and $\psi^{-1}(V^c)$.

The commutant $E_{(\mathbf{C})}$ of $V_{(\mathbf{C})}$ thus contains $\mathbf{C}\times \mathbf{C}$, operating by homotheties on $V^c\oplus \overline{V}^c$. There is no isomorphism of $A_{(\mathbf{C})}$-modules from $V^c$ to $\overline{V}^c$ if and only if $E_{(\mathbf{C})}$ reduces to $\mathbf{C}\times \mathbf{C}$, that is, if E is isomorphic to $\mathbf{C}$. This completes the proof.

#### Proposition 2 {#lie-ix-a2-prop-2 .statement tag=01IT}

Let A be an $\mathbf{R}$-algebra (associative and unital), and W a finite dimensional simple $A_{(\mathbf{C})}$-module over $\mathbf{C}$. Then, we must be in one of the following three situations:

a) There exists an $A_{(\mathbf{C})}$-isomorphism $\theta$ from W to $\overline{W}$ with $\theta \circ \theta = 1_W$. Then the set V of fixed points of $\theta$ is an $\mathbf{R}$-structure on W, and a simple A-module with commutant $\mathbf{R}.1_V$. Moreover, $W_{[\mathbf{R}]}$ is the direct sum of two isomorphic simple A-modules.

b) The $A_{(\mathbf{C})}$-modules W and $\overline{W}$ are not isomorphic; then $W_{[\mathbf{R}]}$ is a simple A-module with commutant $\mathbf{C}.1_W$.

c) There exists an $A_{(\mathbf{C})}$-isomorphism $\theta$ from W to $\overline{W}$ with $\theta \circ \theta =-1_W$. Then the A-module $W_{[\mathbf{R}]}$ is simple, and its commutant is the field $\mathbf{C}.1_W\oplus \mathbf{C}.\theta$, which is isomorphic to $\mathbf{H}$.

The complex vector space Hom$_{A_{(\mathbf{C})}}(W,W)$ is of dimension $\leq 1 ($Algebra, Chap. VIII, §3, no. 2); if $\theta \in$ Hom$_{A_{(\mathbf{C})}}(W,W)$, the endomorphism $\theta \circ \theta$ of W is a homothety, with ratio $\alpha \in \mathbf{C}$. For all $w\in W$, we have $\alpha \theta (w) =\theta \circ \theta \circ \theta (w) =$ $\theta (\alpha w) = \overline{\alpha \theta}(w)$, so $\alpha$ is real. If $\theta '=\lambda \theta$, with $\lambda \in \mathbf{C}$, then $\theta '\circ \theta '=|\lambda |^2\theta \circ \theta$; thus, exactly one of the following three possibilities is realised:

$a)$ There exists $\theta \in$ Hom$_{A_{(\mathbf{C})}}(W,W)$ with $\theta \circ \theta = 1_W$;

$b)$ Hom$_{A_{(\mathbf{C})}}(W,W) =\{0\}$;

$c)$ There exists $\theta \in$ Hom$_{A_{(\mathbf{C})}}(W,W)$ with $\theta \circ \theta =-1_W$.

In case $a)$, the set V of fixed points of $\theta$ is an $\mathbf{R}$-structure on W (Algebra, Chap. V, p. 61, Prop. 7); since $V_{(\mathbf{C})}$ is isomorphic to W, the A-module V is simple with commutant $\mathbf{R}.1_V$ (Prop. 1), and $W_{[\mathbf{R}]}$ is not simple.

Conversely, if $W_{[\mathbf{R}]}$ is not simple, let V be a simple A-submodule of $W_{[\mathbf{R}]}$; since the $A_{(\mathbf{C})}$-module W is simple, $V +iV = W$ and $V\cap iV =\{0\}$, that is, $W = V\oplus iV$. Thus, V is an $\mathbf{R}$-structure on W, and the isomorphism $\theta$ from W to $\overline{W}$ such that $\theta (v+iv') =v-iv'$ for $v$ and $v'$ in V satisfies $\theta \circ \theta = 1_W$.

Consequently, in cases $b)$ and $c)$, the A-module $W_{[\mathbf{R}]}$ is simple; by Prop. 1, its commutant E is isomorphic to $\mathbf{C}$ in case $b)$, and to $\mathbf{H}$ in case $c)$. Moreover, it is clear that E contains $\mathbf{C}.1_W$, and $\mathbf{C}.\theta$ in case $c)$, hence the proposition.

With the assumptions in the proposition, the $A_{(\mathbf{C})}$-module W is said to be of real, complex or quaternionic type (relative to A) in case $a),b)$ or $c)$, respectively.

For $K =\mathbf{R}$ or $\mathbf{C}$, denote by $\mathfrak{S}_K(A)$ the set of classes of finite dimensional simple $A_{(K)}$-modules over K. The group $\Gamma =$ Gal($\mathbf{C}/\mathbf{R}$) operates on $\mathfrak{S}_{\mathbf{C}}(A)$; the two preceding propositions establish a bijective correspondence between $\mathfrak{S}_{\mathbf{R}}(A)$ and the quotient set $\mathfrak{S}_{\mathbf{C}}(A)/\Gamma$.

### 2. REPRESENTATIONS OF COMPACT GROUPS

Let G be a compact topological group, and let $\rho : G\rightarrow \mathbf{G}\mathbf{L}(W)$ be a continuous representation of G on a finite dimensional complex vector space. We shall say that $\rho$ is irreducible of real, complex or quaternionic type if this is the case for the $\mathbf{C}^{(G)}$-module W (relative to the algebra $A =\mathbf{R}^{(G)}$). Let H be a separating positive hermitian form on W, invariant under G.

#### Proposition 3 {#lie-ix-a2-prop-3 .statement tag=01IU}

Assume that $\rho$ is irreducible.

a) The representation $\rho$ is of real type if and only if there exists a non-zero symmetric bilinear form B on W, invariant under G. In this case the form B is separating; the set V of $w\in W$ such that $H(w, x) = B(w, x)$ for all $x\in W$ is an $\mathbf{R}$-structure on W invariant under G.

b) The representation $\rho$ is of complex type if and only if there exists no non-zero bilinear form on W invariant under G.

c) The representation $\rho$ is of quaternionic type if and only if there exists a non-zero alternating bilinear form on W, invariant under G; such a form is necessarily separating.

For $\theta \in$ Hom$_{\mathbf{C}^{(G)}}(W,W)$ and $x, y\in W$, put $B_{\theta}(x, y) = H(\theta x, y)$. Then $B_{\theta}$ is a bilinear form on W, invariant under G, and separating if $\theta$ is non-zero. Denote by $\mathscr{B}(W)^G$ the space of bilinear forms on W invariant under G; the map $\theta  \rightarrow B_{\theta}$ from Hom$_{\mathbf{C}^{(G)}}(W,W)$ to $\mathscr{B}(W)^G$ is an isomorphism of $\mathbf{C}$-vector spaces. This implies, in particular, assertion $b)$.

Let $\theta$ be a $\mathbf{C}^{(G)}$-isomorphism from W to $\overline{W}$ such that $\theta \circ \theta =\alpha_W$, with $\alpha \in  \{-1,+1\}$ (Prop. 2); since $\mathscr{B}(W)^G$ is of dimension 1, there exists $\varepsilon \in \mathbf{C}$ such that

$B_{\theta}(y, x) =\varepsilon B_{\theta}(x, y)$ for all $x, y$ in $W$.

Iterating, we obtain $B_{\theta}(y, x) =\varepsilon B_{\theta}(x, y) =\varepsilon^2B_{\theta}(y, x)$, so $\varepsilon^2$ = 1 and $\varepsilon \in  \{-1,+1\}$. Moreover, for $x$ in W,

$$
H(\theta x, \theta x) = B_{\theta}(x, \theta x) =\varepsilon B_{\theta}(\theta x, x) =\varepsilon H(\theta \circ \theta (x), x) =\varepsilon \alpha H(x, x)
$$

so $\varepsilon \alpha  >0$ since H is positive, that is, $\varepsilon =\alpha$. Assertions $a)$ and $c)$ now follow from Prop. 2.

Denote by $dg$ the Haar measure of total mass 1 on G.

#### Lemma 1 {#lie-ix-a2-lem-1 .statement tag=01IV}

Let $W^G$ be the subspace of W consisting of the elements invariant under G. The endomorphism $\int_G\rho (g)dg$ of W is a projection with image $W^G$, compatible with the operations of G. In particular, dim $W^G=\int_G$ Tr $\rho (g)dg$.

Put $p=\int_G\rho (g)dg$; for $h\in G$,

$$
\rho (h)\circ p=\int_G\rho (hg)dg=\int_G\rho (g)dg=p
$$

and similarly $p\circ \rho (h) =p$. Thus, $p$ is compatible with the operations of G, and its image is contained in $W^G$. If $w\in W^G$, we have $p(w) =\int_G\rho (g)w dg=w$, hence the lemma.

#### Lemma 2 {#lie-ix-a2-lem-2 .statement tag=01IW}

Let $u$ be an endomorphism of a finite dimensional vector space E over a field K. Then

Tr $u^2=$ Tr $\mathbf{S}^2(u)-$ Tr $\wedge \wedge^2(u)$.

Let $\chi_u(X) =\prod_{i=1}^n(X-\alpha_i)$ be a decomposition of the characteristic polynomial of $u$ into linear factors in a suitable extension of K. We have Tr $u^2=\sum_i\alpha^2_i$, Tr $\wedge \wedge^2(u) =\sum_{i<j}\alpha_i\alpha_j$, Tr $\mathbf{S}^2(u) =\sum_{i\leq j}\alpha_i\alpha_j$ (cf. Algebra, Chap. VII, §5, no. 5, Cor. 3), hence the result.

#### Proposition 4 {#lie-ix-a2-prop-4 .statement tag=01IX}

Assume that $\rho$ is irreducible. Then, $\rho$ is of real (resp. complex, resp. quaternionic) type if and only if the integral $\int_G$ Tr$\rho (g^2)dg$ is equal to 1 (resp. 0, resp. $-1$).

Denote by $\check{\rho}$ the contragredient representation of $\rho$ on $W^*$ (defined by $\check{\rho}(g) =^t\rho (g^{-1})$). Applying Lemma 2 to $\check{\rho}(g)$ and integrating over G gives

$\int_G$ Tr$\rho (g^2)dg=\int_G$ Tr $^t\rho (g^{-2})dg=\int_G$ Tr $\mathbf{S}^2( \check{\rho}(g))dg-\int_G$ Tr $\wedge \wedge^2( \check{\rho}(g))dg$

hence, by Lemma 1,

$\int_G$ Tr $\rho (g^2)dg=$ dim($\mathbf{S}^2W^*$)$^G-$ dim($\wedge \wedge^2W^*$)$^G$.

But $\mathbf{S}^2W^*$ (resp. $\wedge \wedge^2W^*$) can be identified with the space of symmetric (resp. alternating) bilinear forms on W. Thus, the proposition follows immediately from Prop. 3.
