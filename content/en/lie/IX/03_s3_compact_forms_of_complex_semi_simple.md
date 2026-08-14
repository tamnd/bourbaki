---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 3
section_title: Compact forms of complex semi-simple Lie algebras
lang: en
source: lie-vii-ix
book_pages: A IX.296-A IX.303, A IX.394-A IX.396
pdf_pages: 0303-0310, 0401-0403
extraction: native+ocr
subsections:
    - "no": 1
      title: REAL FORMS
      page: 296
      pdf_page: 303
    - "no": 2
      title: REAL FORMS ASSOCIATED TO A CHEVALLEY SYSTEM
      page: 297
      pdf_page: 304
    - "no": 3
      title: CONJUGACY OF COMPACT FORMS
      page: 299
      pdf_page: 306
    - "no": 4
      title: 'EXAMPLE I: COMPACT ALGEBRAS OF TYPE A$_{\boldsymbol{n}}$'
      page: 300
      pdf_page: 307
    - "no": 5
      title: 'EXAMPLE II: COMPACT ALGEBRAS OF TYPE B$_{\boldsymbol{n}}\mathbf{A}\mathbf{N}\mathbf{D}$ $\mathbf{D}_{\boldsymbol{n}}$'
      page: 301
      pdf_page: 308
    - "no": 6
      title: COMPACT GROUPS OF RANK 1
      page: 302
      pdf_page: 309
statements: 17
exercises: 9
content_sha256: 8c6af33be7bfa914d08767f309c3b61ce8fde4ef372cc0c42b8a92c3363d045f
---

## § 3. COMPACT FORMS OF COMPLEX SEMI- SIMPLE LIE ALGEBRAS

### 1. REAL FORMS

If $\mathfrak{a}$ is a complex Lie algebra, we denote by $\mathfrak{a}_{[\mathbf{R}]}$ (or sometimes by $\mathfrak{a})$ the real Lie algebra obtained by restriction of scalars. If $\mathfrak{g}$ is a real Lie algebra, we denote by $\mathfrak{g}_{(\mathbf{C})}$ (or sometimes by $\mathfrak{g}_{\mathbf{C}})$ the complex Lie algebra $\mathbf{C}\otimes_{\mathbf{R}}\mathfrak{g}$ obtained by extension of scalars. The homomorphisms of real Lie algebras $\mathfrak{g}\rightarrow \mathfrak{a}_{[\mathbf{R}]}$ correspond bijectively to the homomorphisms of complex Lie algebras $\mathfrak{g}_{(\mathbf{C})}\rightarrow \mathfrak{a}:$ if $f:\mathfrak{g}\rightarrow \mathfrak{a}_{[\mathbf{R}]}$ and $g:\mathfrak{g}_{(\mathbf{C})}\rightarrow \mathfrak{a}$ correspond, we have $f(x) =g(1\otimes x)$ and $g(\lambda \otimes x) =\lambda f(x)$ for $x\in \mathfrak{g}, \lambda \in \mathbf{C}$.

#### Definition 1 {#lie-ix-s3-def-1 .statement tag=01B1}

Let $\mathfrak{a}$ be a complex Lie algebra. A real form of $\mathfrak{a}$ is a real subalgebra $\mathfrak{g}$ of $\mathfrak{a}$ that is an $\mathbf{R}$-structure on the $\mathbf{C}$-vector space $\mathfrak{a}($Algebra, Chap. II, §8, no. 1, Def. 1).

This means that the homomorphism of complex Lie algebras $\mathfrak{g}_{(\mathbf{C})}\rightarrow \mathfrak{a}$ associated to the canonical injection $\mathfrak{g}\rightarrow \mathfrak{a}_{[\mathbf{R}]}$ is bijective. Thus, a real subalgebra $\mathfrak{g}$ of $\mathfrak{a}$ is a real form of $\mathfrak{a}$ if and only if the subspaces $\mathfrak{g}$ and $i\mathfrak{g}$ of the real vector space $\mathfrak{a}$ are complementary. The conjugation of $\mathfrak{a}$ relative to the real form $\mathfrak{g}$ is the map $\sigma :\mathfrak{a}\rightarrow \mathfrak{a}$ such that

$$
\sigma (x+iy) =x-iy,x, y\in \mathfrak{g} \tag{1}
$$

#### Proposition 1 {#lie-ix-s3-prop-1 .statement tag=01JF}

$a)$ Let $\mathfrak{g}$ be a real form of $\mathfrak{a}$ and $\sigma$ the conjugation of $\mathfrak{a}$ relative to $\mathfrak{g}$. Then:

$\sigma^2=$ Id$_{\mathfrak{a}}, \sigma (\lambda x+\mu y) = \overline{\lambda \sigma}(x) + \overline{\mu\sigma}(y),[\sigma (x), \sigma (y)] =\sigma [x, y]$ (2)

for $\lambda , \mu\in \mathbf{C},x, y\in \mathfrak{a}$. An element $x$ of $\mathfrak{a}$ belongs to $\mathfrak{g}$ if and only if $\sigma (x) =x$.

$b)$ Let $\sigma :\mathfrak{a}\rightarrow \mathfrak{a}$ be a map satisfying (2). Then the set $\mathfrak{g}$ of fixed points of $\sigma$ is a real form of $\mathfrak{a}$, and $\sigma$ is the conjugation of $\mathfrak{a}$ relative to $\mathfrak{g}$.

The proof is immediate.

Note that if B denotes the Killing form of $\mathfrak{a}$, and if $\mathfrak{g}$ is a real form of $\mathfrak{a}$, the restriction of B to $\mathfrak{g}$ is the Killing form of $\mathfrak{g}$; in particular, B is real-valued on $\mathfrak{g}\times \mathfrak{g}$. Assume that $\mathfrak{a}$ is reductive; then the real Lie algebra $\mathfrak{g}$ is compact if and only if the restriction of B to $\mathfrak{g}$ is negative (§1, no. 3). In that case we say that $\mathfrak{g}$ is a compact real form of $\mathfrak{a}$.

### 2. REAL FORMS ASSOCIATED TO A CHEVALLEY SYSTEM

In this number, we consider a split semi-simple Lie algebra $(\mathfrak{a},\mathfrak{h})$ over the field $\mathbf{C}$ (Chap. VIII, §2, no. 1), with root system $R(\mathfrak{a},\mathfrak{h}) = R$, and a Chevalley system $(X_{\alpha})_{\alpha\in R}$ of $(\mathfrak{a},\mathfrak{h})$ (Chap. VIII, §2, no. 4, Def. 3).

Recall (loc. cit.) that the linear map $\theta :\mathfrak{a}\rightarrow \mathfrak{a}$ that coincides with $-$Id$_{\mathfrak{h}}$ on $\mathfrak{h}$ and maps $X_{\alpha}$ to $X_{-\alpha}$ for all $\alpha \in R$ is an automorphism of $\mathfrak{a}$. Moreover (loc. cit., Prop. 7), if $\alpha , \beta , \alpha +\beta$ are roots, then

$$
[X_{\alpha}, X_{\beta}] = N_{\alpha ,\beta}X_{\alpha+\beta} \tag{3}
$$

with $N_{\alpha ,\beta}\in \mathbf{R}^*$ and

$$
N_{-\alpha ,-\beta}= N_{\alpha ,\beta} \tag{4}
$$

Denote by $\mathfrak{h}_0$ the real vector subspace of $\mathfrak{h}$ consisting of the $H\in \mathfrak{h}$ such that $\alpha (H)\in \mathbf{R}$ for all $\alpha \in R$. Then $\mathfrak{h}_0$ is an $\mathbf{R}$-structure on the complex vector space $\mathfrak{h}$, we have $[X_{\alpha}, X_{-\alpha}]\in \mathfrak{h}_0$ for all $\alpha \in R$, and the restriction of the Killing form B of $\mathfrak{a}$ to $\mathfrak{h}_0$ is separating positive (Chap. VIII, §2, no. 2, Remark 2). Moreover,

$B(H, X_{\alpha}) = 0,B(X_{\alpha}, X_{\beta}) = 0$ if $\alpha +\beta \not= 0,B(X_{\alpha}, X_{-\alpha})<0$ (5)

(Chap. VIII, §2, no. 2, Prop. 1 and no. 4, Lemma 3).

#### Proposition 2 {#lie-ix-s3-prop-2 .statement tag=01JG}

$a)$ The real vector subspace $\mathfrak{a}_0=\mathfrak{h}_0+\sum_{\alpha\in R}\mathbf{R}X_{\alpha}$ of $\mathfrak{a}$ is a

real form of $\mathfrak{a}$, of which $\mathfrak{h}_0$ is a Cartan subalgebra. The pair $(\mathfrak{a}_0,\mathfrak{h}_0)$ is a split semi-simple real Lie algebra, of which $(X_{\alpha})$ is a Chevalley system.

$b)$ Let $\sigma$ be the conjugation of $\mathfrak{a}$ relative to $\mathfrak{a}_0$. Then $\sigma \circ \theta =\theta \circ \sigma$. The set of fixed points of $\sigma \circ \theta$ is a compact real form $\mathfrak{a}_u$ of $\mathfrak{a}$, of which $i\mathfrak{h}_0$ is a Cartan subalgebra.

Part $a)$ follows immediately from the preceding. We prove $b)$. Since $\sigma \circ \theta$ and $\theta \circ \sigma$ are two semi-linear maps from $\mathfrak{a}$ to $\mathfrak{a}$ that coincide on $\mathfrak{a}_0$, they coincide. Now $\sigma \circ \theta$ satisfies conditions (2) of no. 1, hence is the conjugation of $\mathfrak{a}$ relative to the real form $\mathfrak{a}_u$ consisting of the $x\in \mathfrak{a}$ such that $\sigma \circ \theta (x) =x$ (Prop. 1). For all $\alpha \in R$ put

$$
u_{\alpha}=X_{\alpha}+X_{-\alpha},v_{\alpha}=i(X_{\alpha}-X_{-\alpha}) \tag{6}
$$

Then the $\mathbf{R}$-vector space $\mathfrak{a}_u$ is generated by $i\mathfrak{h}_0$, the $u_{\alpha}$ and the $v_{\alpha}$. More precisely, if we choose a chamber C of R, then

$$
\mathfrak{a}_u=i\mathfrak{h}_0\oplus \bigoplus_{\alpha\in R_+(C)}(\mathbf{R}u_{\alpha}+\mathbf{R}v_{\alpha}) \tag{7}
$$

It is clear that $i\mathfrak{h}_0$ is a Cartan subalgebra of $\mathfrak{a}_u$, and it remains to prove that the restriction of B to $\mathfrak{a}_u$ is negative. Now $i\mathfrak{h}_0$ and the different subspaces of the form $\mathbf{R}u_{\alpha}\oplus \mathbf{R}v_{\alpha}$ are orthogonal with respect to B, by (5); the restriction of B to $i\mathfrak{h}_0$ is negative and

$$
B(u_{\alpha}, u_{\alpha}) = B(v_{\alpha}, v_{\alpha}) = 2B(X_{\alpha}, X_{-\alpha})<0,B(u_{\alpha}, v_{\alpha}) = 0 \tag{8}
$$

hence the conclusion.

#### Remark {#lie-ix-s3-n2-rem-1 .statement tag=01B2}

With the preceding notations, we have the following formulas:

$$
[h, u_{\alpha}] =-i\alpha (h)v_{\alpha},[h, v_{\alpha}] =i\alpha (h)u_{\alpha},[u_{\alpha}, v_{\alpha}] = 2iH_{\alpha},(h\in \mathfrak{h}) \tag{9}
$$

$$
[u_{\alpha}, u_{\beta}] = N_{\alpha ,\beta}u_{\alpha+\beta}+ N_{\alpha ,-\beta}u_{\alpha-\beta},\alpha \not=\pm \beta \tag{10}
$$

$$
[v_{\alpha}, v_{\beta}] =-N_{\alpha ,\beta}u_{\alpha+\beta}+ N_{\alpha ,-\beta}u_{\alpha-\beta},\alpha \not=\pm \beta \tag{11}
$$

$$
[u_{\alpha}, v_{\beta}] = N_{\alpha ,\beta}v_{\alpha+\beta}-N_{\alpha ,-\beta}v_{\alpha-\beta},\alpha \not=\pm \beta \tag{12}
$$

(in the last three formulas, it is understood, as usual, that $N_{\gamma ,\delta}= 0$ if $\gamma +\delta$ is not a root).

Note that $\sum\mathbf{R}u_{\alpha}$ is a real subalgebra of $\mathfrak{a}$, namely $\mathfrak{a}_0\cap \mathfrak{a}_u$.

Let Q(R) be the group of radical weights of R (Chap. VI, §1, no. 9). Recall that to any homomorphism $\gamma : Q(R)\rightarrow \mathbf{C}^*$ is associated an elementary automorphism $f(\gamma )$ of $\mathfrak{a}$ such that $f(\gamma )(h) =h$ for all $h\in \mathfrak{h}$ and $f(\gamma )X_{\alpha}=$ $\gamma (\alpha )X_{\alpha}$ (Chap. VIII, §5, no. 2).

#### Proposition 3 {#lie-ix-s3-prop-3 .statement tag=01B3}

Let $\mathfrak{g}$ be a compact real form of $\mathfrak{a}$ such that $\mathfrak{g}\cap \mathfrak{h}=i\mathfrak{h}_0$. There exists a homomorphism $\gamma : Q(R)\rightarrow \mathbf{R}^*_+$ such that $\mathfrak{g}=f(\gamma )(\mathfrak{a}_u)$.

Let $\tau$ be the conjugation of $\mathfrak{a}$ relative to $\mathfrak{g}$. By hypothesis $\tau (x) =x$ for $x\in i\mathfrak{h}_0$, so $\tau (x) =-x$ for $x\in \mathfrak{h}_0$. Thus, for all $\alpha \in R$ and all $h\in \mathfrak{h}_0$,

$$
[h, \tau (X_{\alpha})] = [-\tau (h), \tau (X_{\alpha})] =-\tau ([h, X_{\alpha}]) =-\tau (\alpha (h)X_{\alpha})
$$

it follows that $[h, \tau (X_{\alpha})] =-\alpha (h)\tau (X_{\alpha})$ for all $h\in \mathfrak{h}_0$, hence also for all $h\in \mathfrak{h}$. Hence there exists $c_{\alpha}\in \mathbf{C}^*$ such that $\tau (X_{\alpha}) =c_{\alpha}X_{-\alpha}$. Since $[X_{\alpha}, X_{-\alpha}]\in \mathfrak{h}_0$, we have $[\tau (X_{\alpha}), \tau (X_{-\alpha})] =-[X_{\alpha}, X_{-\alpha}]$, so $c_{\alpha}c_{-\alpha}$ = 1; similarly, formulas (3) and (4) give $c_{\alpha+\beta}=c_{\alpha}c_{\beta}$ if $\alpha , \beta , \alpha +\beta$ are roots. By Chap. VI, §1, no. 6, Cor. 2 of Prop. 19, there exists a homomorphism $\delta : Q(R)\rightarrow \mathbf{C}^*$ such that $\delta (\alpha ) =c_{\alpha}$ for all $\alpha \in R$.

We now show that each $c_{\alpha}$ is strictly positive. Indeed, $c_{\alpha}B(X_{\alpha}, X_{-\alpha}) =$ $B(X_{\alpha}, \tau (X_{\alpha}))$, and since $B(X_{\alpha}, X_{-\alpha})$ is negative, it suffices to show that $B(z, \tau (z))<0$ for every non-zero element $z$ of $\mathfrak{a}$; but every element of $\mathfrak{a}$ can be written as $x+iy$, with $x$ and $y$ in $\mathfrak{g}$, and

$$
B(x+iy, \tau (x+iy)) = B(x+iy, x-iy) = B(x, x) + B(y, y)
$$

hence the stated assertion, the restriction of B to $\mathfrak{g}$ being negative and separating by hypothesis.

It follows that the homomorphism $\delta$ takes values in $\mathbf{R}^*_+$; hence there exists a homomorphism $\gamma : Q(R)\rightarrow \mathbf{R}^*_+$ such that $\delta =\gamma^{-2}$. Then $f(\gamma )^{-1}(\mathfrak{g})$ is a real form of $\mathfrak{a}$; the corresponding conjugation is $\tau '=f(\gamma )^{-1}\circ \tau \circ f(\gamma )$. For all $\alpha \in R$, we have

$$
\tau '(X_{\alpha}) =f(\gamma )^{-1}(\tau (c^{-1/2}_{\alpha}X_{\alpha})) =f(\gamma )^{-1}(c^{1/2}_{\alpha}X_{-\alpha}) =X_{-\alpha}
$$

and $\tau '(h) =\tau (h) =h$ for $h\in i\mathfrak{h}_0$; it follows that $\tau '$ is the conjugation with respect to $\mathfrak{a}_u$, and hence that $f(\gamma )^{-1}(\mathfrak{g}) =\mathfrak{a}_u$.

### 3. CONJUGACY OF COMPACT FORMS

#### Theorem 1 {#lie-ix-s3-thm-1 .statement tag=01B4}

Let $\mathfrak{a}$ be a complex semi-simple Lie algebra.

a$)\mathfrak{a}$ has compact (resp. splittable) real forms.

b) The group Int($\mathfrak{a}$) operates transitively on the set of compact (resp. splittable) real forms of $\mathfrak{a}$.

Let $\mathfrak{h}$ be a Cartan subalgebra of $\mathfrak{a}$. Then $(\mathfrak{a},\mathfrak{h})$ is split (Chap. VIII, §2, no. 1, Remark 2), and has a Chevalley system $(X_{\alpha})$ (Chap. VIII, §4, no. 4, Cor. of Prop. 5). Part $a)$ now follows from Prop. 2. Let $\mathfrak{g}$ be a compact real form of $\mathfrak{a}$; we show that there exists $v\in$ Int($\mathfrak{a}$) such that $v(\mathfrak{a}_u) =\mathfrak{g}$. Let $\mathfrak{t}$ be a Cartan subalgebra of $\mathfrak{g}$; then $\mathfrak{t}_{(\mathbf{C})}$ is a Cartan subalgebra of $\mathfrak{a}$; since Int($\mathfrak{a}$) operates transitively on the set of Cartan subalgebras of $\mathfrak{a}$ (Chap. VII, §3, no. 2, Th. 1), we are reduced to the case in which $\mathfrak{t}_{(\mathbf{C})}=\mathfrak{h}$. Since $\mathfrak{g}$ is a compact form, the eigenvalues of the endomorphisms ad $h$, for $h\in \mathfrak{t}$, are purely imaginary (§1, no. 3, Prop. 1), so the roots $\alpha \in R$ map $\mathfrak{t}$ to $i\mathbf{R}$; this implies that $\mathfrak{t}=i\mathfrak{h}_0$. Then, by Prop. 3 (no. 2), there exists $v\in$ Int($\mathfrak{a}$) such that $v(\mathfrak{a}_u) =\mathfrak{g}$, hence $b)$ in the case of compact forms. Finally, let $\mathfrak{m}_1$ and $\mathfrak{m}_2$ be two splittable real forms of $\mathfrak{a}$. There exist framings $(\mathfrak{m}_1,\mathfrak{h}_1,B_1,(X_{\alpha}^1))$ and $(\mathfrak{m}_2,\mathfrak{h}_2,B_2,(X_{\alpha}^2))$ (Chap. VIII, §4, no. 1). These extend in an obvious way to bases $e_1$ and $e_2$ of $\mathfrak{a}$. An automorphism of $\mathfrak{a}$ that maps $e_1$ to $e_2$ maps $\mathfrak{m}_1$ to $\mathfrak{m}_2$; thus, it suffices to apply Prop. 5 of Chap. VIII, §5, no. 3, to obtain the existence of an element $u$ of Aut$_0(\mathfrak{a}) =$ Int($\mathfrak{a}$) such that $u(\mathfrak{m}_1) =\mathfrak{m}_2$.

#### Remark {#lie-ix-s3-n3-rem-1 .statement tag=01B5}

We shall see much later a general classification of real forms of a complex semi-simple Lie algebra.

#### Corollary 1 {#lie-ix-s3-thm-1-cor-1 .statement tag=01B6}

Let $\mathfrak{g}$ and $\mathfrak{g}'$ be two compact real Lie algebras. Then $\mathfrak{g}$ and $\mathfrak{g}'$ are isomorphic if and only if the complex Lie algebras $\mathfrak{g}_{(\mathbf{C})}$ and $\mathfrak{g}'_{(\mathbf{C})}$ are isomorphic.

The condition is clearly necessary. Conversely, assume that $\mathfrak{g}_{(\mathbf{C})}$ and $\mathfrak{g}'_{(\mathbf{C})}$ are isomorphic. Let $\mathfrak{c}$ (resp. $\mathfrak{c}')$ be the centre of $\mathfrak{g}$ (resp. $\mathfrak{g}')$ and $\mathfrak{s}$ (resp. $\mathfrak{s}')$ the derived algebra of $\mathfrak{g}$ (resp. $\mathfrak{g}')$. Then $\mathfrak{c}_{(\mathbf{C})}$ and $\mathfrak{c}'_{(\mathbf{C})}$ are the centres of $\mathfrak{g}_{(\mathbf{C})}$ and $\mathfrak{g}'_{(\mathbf{C})}$, respectively, and hence are isomorphic; it follows that the commutative algebras $\mathfrak{c}$ and $\mathfrak{c}'$ are isomorphic. Similarly, $\mathfrak{s}_{(\mathbf{C})}$ and $\mathfrak{s}'_{(\mathbf{C})}$ are isomorphic, hence $\mathfrak{s}$ and $\mathfrak{s}'$, which are compact real forms of two isomorphic complex semi-simple Lie algebras, are isomorphic by Th. $1b)$.

#### Corollary 2 {#lie-ix-s3-thm-1-cor-2 .statement tag=01B7}

Let $\mathfrak{a}$ be a complex Lie algebra. The following conditions are equivalent:

(i) $\mathfrak{a}$ is reductive.

(ii) There exists a compact real Lie algebra $\mathfrak{g}$ such that $\mathfrak{a}$ is isomorphic to $\mathfrak{g}_{(\mathbf{C})}$.

(iii) There exists a compact Lie group G such that $\mathfrak{a}$ is isomorphic to $L(G)_{(\mathbf{C})}$.

By Def. 1 of §1, no. 3, conditions (ii) and (iii) are equivalent and imply (i). If $\mathfrak{a}$ is reductive, it is the direct product of a commutative algebra, which clearly has a compact real form, and a semi-simple algebra which has one by Th. $1a)$, hence (i) implies (ii).

#### Corollary 3 {#lie-ix-s3-thm-1-cor-3 .statement tag=01B8}

Let $\mathfrak{a}_1$ and $\mathfrak{a}_2$ be two complex semi-simple Lie algebras. The compact real forms of $\mathfrak{a}_1\times \mathfrak{a}_2$ are the products $\mathfrak{g}_1\times \mathfrak{g}_2$, where, for $i= 1,2,\mathfrak{g}_i$ is a compact real form of $\mathfrak{a}_i$.

Indeed, there exists a compact real form $\mathfrak{g}_1$ (resp. $\mathfrak{g}_2)$ of $\mathfrak{a}_1$ (resp. $\mathfrak{a}_2)$; then $\mathfrak{g}_1\times \mathfrak{g}_2$ is a compact real form of $\mathfrak{a}_1\times \mathfrak{a}_2$. The corollary now follows from Th. $1b)$, applied to $\mathfrak{a}_1,\mathfrak{a}_2$ and $\mathfrak{a}_1\times \mathfrak{a}_2$.

Note that it follows from Cor. 3 above that a compact real Lie algebra $\mathfrak{g}$ is simple if and only if the complex Lie algebra $\mathfrak{g}_{(\mathbf{C})}$ is simple. We say that $\mathfrak{g}$ is of type $A_n$, or $B_n,. .$., if $\mathfrak{g}_{(\mathbf{C})}$ is of type $A_n$, or $B_n,. .$. (Chap. VIII, §2, no. 2). By Cor. 1 above, two compact simple real Lie algebras are isomorphic if and only if they are of the same type.

Let G be an almost simple connected compact Lie group (Chap. III, §9, no. 8, Def. 3). We say that G is of type $A_n$, or $B_n,. .$., if its Lie algebra is of type $A_n$, or $B_n,. .$.. Two simply-connected almost simple compact Lie groups are isomorphic if and only if they are of the same type.

### 4. EXAMPLE I: COMPACT ALGEBRAS OF TYPE A$_{\boldsymbol{n}}$

Let V be a finite dimensional complex vector space and $\Phi$ a separating positive hermitian form on V. The unitary group associated to $\Phi$ (cf. Algebra, Chap. IX) is the subgroup $\mathbf{U}(\Phi )$ of $\mathbf{G}\mathbf{L}(V)$ consisting of the automorphisms of the complex Hilbert space $(V, \Phi )$; this is a (real) Lie subgroup of the group $\mathbf{G}\mathbf{L}$(V), whose Lie algebra is the subalgebra $\mathfrak{u}(\Phi )$ of the real Lie algebra $\mathfrak{g}\mathfrak{l}(V)$ consisting of the endomorphisms $x$ of V such that $x^*=-x$ (Chap. III, §3, no. 10, Cor. 2 of Prop. 37), where $x^*$ denotes the adjoint of $x$ relative to $\Phi$. Since the group $\mathbf{U}(\Phi )$ is compact (§1, no. $1),\mathfrak{u}(\Phi )$ is a compact real Lie algebra. Similarly, the special unitary group $\mathbf{S}\mathbf{U}(\Phi ) =\mathbf{U}(\Phi )\cap \mathbf{S}\mathbf{L}(V)$ is a compact Lie subgroup of $\mathbf{S}\mathbf{L}$(V), whose Lie algebra is $\mathfrak{s}\mathfrak{u}(\Phi ) =\mathfrak{u}(\Phi )\cap \mathfrak{s}\mathfrak{l}(V)$.

When $V =\mathbf{C}^n$ and $\Phi$ is the usual hermitian form (for which the canonical basis of $\mathbf{C}^n$ is orthonormal), we write $\mathbf{U}(n,\mathbf{C}),\mathbf{S}\mathbf{U}(n,\mathbf{C}),\mathfrak{u}(n,\mathbf{C}),\mathfrak{s}\mathfrak{u}(n,\mathbf{C})$ instead of $\mathbf{U}(\Phi ),\mathbf{S}\mathbf{U}(\Phi ),\mathfrak{u}(\Phi ),\mathfrak{s}\mathfrak{u}(\Phi )$. The elements of $\mathbf{U}(n,\mathbf{C})$ (resp. $\mathfrak{u}(n,\mathbf{C}))$ are the matrices $A\in M_n(\mathbf{C})$ such that $A.^t\overline{A}=I_n$ (resp. $A=-^t\overline{A})$, which are said to be unitary (resp. anti-hermitian).

#### Proposition 4 {#lie-ix-s3-prop-4 .statement tag=01B9}

a) The compact real forms of the complex Lie algebra $\mathfrak{s}\mathfrak{l}(V)$ are the algebras $\mathfrak{s}\mathfrak{u}(\Phi )$, where $\Phi$ belongs to the set of separating positive hermitian forms on the complex vector space V.

b) The algebras $\mathfrak{u}(\Phi )$ are the compact real forms of $\mathfrak{g}\mathfrak{l}(V)$.

Let $\Phi$ be a separating positive hermitian form on V. For all $x\in \mathfrak{g}\mathfrak{l}$(V), put $\sigma (x) =-x^*$ (where $x^*$ is the adjoint of $x$ relative to $\Phi )$. Then $\sigma$ satisfies conditions (2) of Prop. 1 of no. 1, so the set $\mathfrak{u}(\Phi )$ (resp. $\mathfrak{s}\mathfrak{u}(\Phi ))$ of fixed points of $\sigma$ on $\mathfrak{g}\mathfrak{l}(V)$ (resp. $\mathfrak{s}\mathfrak{l}(V))$ is a compact real form of $\mathfrak{g}\mathfrak{l}(V)$ (resp. $\mathfrak{s}\mathfrak{l}(V))$. Since $\mathbf{G}\mathbf{L}(V)$ operates transitively on the set of separating positive hermitian forms on V (Algebra, Chap. IX) and on the set of compact real forms of $\mathfrak{s}\mathfrak{l}(V)$ (no. 3, Th. 1 and Chap. VIII, §13, no. 1 (VII)), Prop. 4 is proved.

#### Corollary {#lie-ix-s3-n4-cor-1 .statement tag=01BA}

Every compact simple real Lie algebra of type $A_n(n\geq 1)$ is isomorphic to $\mathfrak{s}\mathfrak{u}(n+ 1,\mathbf{C})$.

Indeed, every complex Lie algebra of type $A_n$ is isomorphic to $\mathfrak{s}\mathfrak{l}(n+ 1,\mathbf{C})$ (Chap. VIII, §13, no. 1).

#### Remark 1 {#lie-ix-s3-n4-rem-1 .statement tag=01BB}

We have $\mathfrak{g}\mathfrak{l}(V) =\mathfrak{s}\mathfrak{l}(V)\times \mathbf{C}.1_V,\mathfrak{u}(\Phi ) =\mathfrak{s}\mathfrak{u}(\Phi )\times \mathbf{R}.i1_V$; the compact real forms of $\mathfrak{g}\mathfrak{l}(V)$ are the $\mathfrak{s}\mathfrak{u}(\Phi )\times \mathbf{R}.\alpha 1_V,\alpha \in \mathbf{C}^*$.

#### Remark 2 {#lie-ix-s3-n4-rem-2 .statement tag=01BC}

If the complex Lie algebra $\mathfrak{a}=\mathfrak{s}\mathfrak{l}(n,\mathbf{C})$ is equipped with the splitting and Chevalley system introduced in Chap. VIII, §13, no. 1 (IX), then, with the notations in no. 2,

$$
\mathfrak{a}_u=\mathfrak{s}\mathfrak{u}(n,\mathbf{C}),\mathfrak{a}_0=\mathfrak{s}\mathfrak{l}(n,\mathbf{R}),\mathfrak{a}_u\cap \mathfrak{a}_0=\mathfrak{o}(n,\mathbf{R})
$$

### 5. EXAMPLE II: COMPACT ALGEBRAS OF TYPE B$_{\boldsymbol{n}}\mathbf{A}\mathbf{N}\mathbf{D}$ $\mathbf{D}_{\boldsymbol{n}}$

Let V be a finite dimensional real vector space and Q a separating positive quadratic form on V. The orthogonal group associated to Q (Algebra, Chap. IX) is the subgroup $\mathbf{O}(Q)$ of $\mathbf{G}\mathbf{L}(V)$ consisting of the automorphisms of the real Hilbert space $(V,Q)$; this is a Lie subgroup of $\mathbf{G}\mathbf{L}$(V), whose Lie algebra is the subalgebra $\mathfrak{o}(Q)$ of $\mathfrak{g}\mathfrak{l}(V)$ consisting of the endomorphisms $x$ of V such that $x^*=-x$ (Chap. III, §3, no. 10, Cor. 2 of Prop. $37),x^*$ denoting the adjoint of $x$ relative to Q. Since the group $\mathbf{O}(Q)$ is compact, $\mathfrak{o}(Q)$ is thus a compact real Lie algebra. Put $\mathbf{S}\mathbf{O}(Q) =\mathbf{O}(Q)\cap \mathbf{S}\mathbf{L}(V)$; this is a closed subgroup of finite index of $\mathbf{O}(Q)$ (of index 2 if dim $V\not= 0)$, hence also with Lie algebra $\mathfrak{o}(Q)$.

When $V =\mathbf{R}^n$ and Q is the usual quadratic form (for which the canonical basis of $\mathbf{R}^n$ is orthonormal), we write $\mathbf{O}(n,\mathbf{R}),\mathbf{S}\mathbf{O}(n,\mathbf{R}),\mathfrak{o}(n,\mathbf{R})$ instead of $\mathbf{O}(Q),\mathbf{S}\mathbf{O}(Q),\mathfrak{o}(Q)$. The elements of $\mathbf{O}(n,\mathbf{R})$ (resp. $\mathfrak{o}(n,\mathbf{R}))$ are the matrices $A\in M_n(\mathbf{R})$ such that $A.^tA=I_n$ (resp. $A=-^tA)$, which are said to be orthogonal (resp. anti-symmetric).

Let $V_{(\mathbf{C})}$ be the complex vector space associated to V and let $Q_{(\mathbf{C})}$ be the quadratic form on $V_{(\mathbf{C})}$ associated to Q. Identify $\mathfrak{g}\mathfrak{l}(V)_{(\mathbf{C})}$ with $\mathfrak{g}\mathfrak{l}(V_{(\mathbf{C})})$; then $\mathfrak{o}(Q)_{(\mathbf{C})}$ is identified with $\mathfrak{o}(Q_{(\mathbf{C})}):$ this is clear since the map $x \rightarrow x^*+x$ from $\mathfrak{g}\mathfrak{l}(V_{(\mathbf{C})})$ to itself is $\mathbf{C}$-linear. Since $\mathfrak{o}(Q_{(\mathbf{C})})$ is of type $B_n$ if dim $V = 2n+ 1$, $n\geq 1$, and of type $D_n$ if dim $V = 2n,n\geq 3$ (Chap. VIII, §13, nos. 2 and 4), we deduce:

#### Proposition 5 {#lie-ix-s3-prop-5 .statement tag=01BD}

Every compact simple real Lie algebra of type $B_n,n\geq 1$ (resp. of type $D_n,n\geq 3)$ is isomorphic to $\mathfrak{o}(2n+ 1,\mathbf{R})$ (resp. $\mathfrak{o}(2n,\mathbf{R}))$.

### 6. COMPACT GROUPS OF RANK 1

By General Topology, Chap. VIII, §1, no. 4, Prop. 3, Prop. 4 and Remark 4, the topological group $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ is isomorphic to the topological group $\mathbf{S}_3$ of quaternions of norm 1, and the quotient of $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ by the subgroup Z consisting of the matrices $I_2$ and $-I_2$ is isomorphic to the topological group $\mathbf{S}\mathbf{O}(3,\mathbf{R})$. Note that Z is the centre of $\mathbf{S}\mathbf{U}(2,\mathbf{C}):$ indeed, since $\mathbf{H}=\mathbf{R}.\mathbf{S}_3$, every element of the centre of the group $\mathbf{S}_3$ is in the centre $\mathbf{R}$ of the algebra $\mathbf{H}$ and hence belongs to the group with two elements $\mathbf{S}_3\cap \mathbf{R}=\{-1,1\}$.

#### Proposition 6 {#lie-ix-s3-prop-6 .statement tag=01BE}

Every compact semi-simple real Lie algebra of rank 1 is isomorphic to $\mathfrak{s}\mathfrak{u}(2,\mathbf{C})$ and to $\mathfrak{o}(3,\mathbf{R})$. Every connected semi-simple compact Lie group of rank 1 is isomorphic to $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ if it is simply-connected, and to $\mathbf{S}\mathbf{O}(3,\mathbf{R})$ if not.

The first assertion follows from the Cor. of Prop. 4 and Prop. 5. Since $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ is homeomorphic to $\mathbf{S}_3($General Topology, Chap. VIII, §1, no. 4, Remark 4), hence is simply-connected (General Topology, Chap. XI, in preparation), every simply-connected compact semi-simple Lie group of rank 1 is isomorphic to $\mathbf{S}\mathbf{U}(2,\mathbf{C})$; every connected compact semi-simple Lie group of rank 1 that is not simply-connected is isomorphic to a quotient of $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ by a subgroup of Z that does not reduce to the identity element, hence to $\mathbf{S}\mathbf{O}(3,\mathbf{R})$.

#### Remark {#lie-ix-s3-n6-rem-1 .statement tag=01BF}

We have seen above that $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ is simply-connected and that $\pi_1(\mathbf{S}\mathbf{O}(3,\mathbf{R}))$ is of order 2. We shall see much later that these results generalize to $\mathbf{S}\mathbf{U}(n,\mathbf{C}) (n\geq 1)$ and $\mathbf{S}\mathbf{O}(n,\mathbf{R}) (n\geq 3)$, respectively (cf. also §3, Exerc. 4 and 5).

Recall (Chap. VIII, §1, no. 1) that the canonical basis of $\mathfrak{s}\mathfrak{l}(2,\mathbf{C})$ is the basis $(X_+, X_-, H)$, where

$(01)(00)(1$ 0 $)$

$X^+=$ 0 0 $, X^-=-1$ 0 $, H=$ 0 $-1$.

We thus obtain a basis $(U,V,iH)$ of $\mathfrak{su}(2,\mathbf C)$, also called canonical, by putting
$$
U=X_++X_-=
\begin{pmatrix}
0&1\\
-1&0
\end{pmatrix},
\qquad
V=i(X_+-X_-)=
\begin{pmatrix}
0&i\\
i&0
\end{pmatrix},
$$
$$
iH=
\begin{pmatrix}
i&0\\
0&-i
\end{pmatrix}.
$$

We have
$$
[iH,U]=2V,\qquad [iH,V]=-2U,\qquad [U,V]=2iH.
\tag{13}
$$

If B denotes the Killing form of $\mathfrak{su}(2,\mathbf C)$ an immediate calculation gives
$$
\mathrm{B}(aU+bV+ciH,a'U+b'V+c'iH)=-8(aa'+bb'+cc'),
\tag{14}
$$
so that, if we identify $\mathfrak{su}(2,\mathbf C)$ with $\mathbf R^3$ by means of the canonical basis, the adjoint representation of $\mathbf{SU}(2,\mathbf C)$ defines a homomorphism $\mathbf{SU}(2,\mathbf C)\to\mathbf{SO}(3,\mathbf R)$ (cf. above).

Further, note that $\mathbf RiH$ is a Cartan subalgebra of $\mathfrak{su}(2,\mathbf C)$, that the maximal torus T of $\mathbf{SU}(2,\mathbf C)$ that corresponds to it consists of the diagonal matrices
$$
\begin{pmatrix}
a&0\\
0&\bar a
\end{pmatrix},
$$
where $a\bar a=1$, and that the exponential map
$$
\exp:\mathbf RiH\longrightarrow T
$$
maps $xH$, for $x\in\mathbf Ri$, to the matrix
$$
\begin{pmatrix}
\exp(x)&0\\
0&\exp(-x)
\end{pmatrix},
$$
and thus has kernel $\mathbf Z.K$, where K is the element of $\mathfrak{su}(2,\mathbf C)$ defined by
$$
K=2\pi iH=
\begin{pmatrix}
2\pi i&0\\
0&-2\pi i
\end{pmatrix}.
\tag{15}
$$

Further, the centre of $\mathbf{SU}(2,\mathbf C)$ consists of the identity and $\exp(K/2)$.

Put
$$
\theta=
\begin{pmatrix}
0&-1\\
1&0
\end{pmatrix}
\in\mathbf{SU}(2,\mathbf C).
\tag{16}
$$

By Chap. VIII, §1, no. 5,
$$
\theta^2=
\begin{pmatrix}
-1&0\\
0&-1
\end{pmatrix},
\qquad
(\mathrm{Int}\,\theta)t=t^{-1},\quad t\in T,
\tag{17}
$$
$$
(\mathrm{Ad}\,\theta)X_+=X_-,
\qquad
(\mathrm{Ad}\,\theta)X_-=X_+,
\qquad
(\mathrm{Ad}\,\theta)U=U,
\qquad
(\mathrm{Ad}\,\theta)V=-V.
\tag{18}
$$

Finally, for $t=
\begin{pmatrix}
a&0\\
0&\bar a
\end{pmatrix}
\in T$, we have
$$
(\mathrm{Ad}\,t)X_+=a^2X_+,
\qquad
(\mathrm{Ad}\,t)X_-=a^{-2}X_-,
\qquad
(\mathrm{Ad}\,t)H=H,
\tag{19}
$$
$$
(\mathrm{Ad}\,t)U=\mathscr{R}(a^2)U+\mathscr{I}(a^2)V,
\qquad
(\mathrm{Ad}\,t)V=-\mathscr{I}(a^2)U+\mathscr{R}(a^2)V.
\tag{20}
$$

### Exercises {#lie-ix-s3-exercises}

See the [exercises for § 3](exercises/s3/).
