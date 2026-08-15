---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 2
section_title: Root system of a split semi-simple Lie algebra
lang: en
source: lie-vii-ix
book_pages: A VIII.77-A VIII.86, A VIII.226-A VIII.229
pdf_pages: 0085-0094, 0234-0237
extraction: native
subsections:
    - "no": 1
      title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
      page: 77
      pdf_page: 85
    - "no": 2
      title: ROOTS OF A SPLIT SEMI-SIMPLE LIE ALGEBRA
      page: 78
      pdf_page: 86
    - "no": 3
      title: INVARIANT BILINEAR FORMS
      page: 83
      pdf_page: 91
    - "no": 4
      title: THE COEFFICIENTS N$_{\boldsymbol{\alpha \beta }}$
      page: 83
      pdf_page: 91
statements: 28
exercises: 12
content_sha256: 76903e64a7bed03cf3d69b67d5aabf44c01f8897393cfc4484d11de5199bd2ab
---

## § 2. ROOT SYSTEM OF A SPLIT SEMI-SIMPLE LIE ALGEBRA

### 1. SPLIT SEMI-SIMPLE LIE ALGEBRAS

#### Definition 1 {#lie-viii-s2-def-1 .statement tag=00YK}

Let $\mathfrak{g}$ be a semi-simple Lie algebra. A Cartan subalgebra $\mathfrak{h}$ of $\mathfrak{g}$ is called splitting if, for all $x\in \mathfrak{h}$, ad$_{\mathfrak{g}}x$ is triangularizable. A semi-simple Lie algebra is called splittable if it has a splitting Cartan subalgebra. A split semi-simple Lie algebra is a pair $(\mathfrak{g},\mathfrak{h})$ where $\mathfrak{g}$ is a semi-simple Lie algebra and $\mathfrak{h}$ is a splitting Cartan subalgebra of $\mathfrak{g}$.

#### Remark 1 {#lie-viii-s2-n1-rem-1 .statement tag=00YL}

Let $\mathfrak{g}$ be a semi-simple Lie algebra, $\mathfrak{h}$ a Cartan subalgebra of $\mathfrak{g}$. For all $x\in \mathfrak{h}$, ad$_{\mathfrak{g}}x$ is semi-simple (Chap. VII, §2, no. 4, Th. 2). Thus, to say that $\mathfrak{h}$ is splitting means that ad$_{\mathfrak{g}}x$ is diagonalizable for all $x\in \mathfrak{h}$.

#### Remark 2 {#lie-viii-s2-n1-rem-2 .statement tag=00YM}

If $k$ is algebraically closed, every semi-simple Lie algebra $\mathfrak{g}$ is splittable, and every Cartan subalgebra of $\mathfrak{g}$ is splitting. When $k$ is not algebraically closed, there exist non-splittable semi-simple Lie algebras (Exerc. $2a))$; moreover, if $\mathfrak{g}$ is splittable, there may exist Cartan subalgebras of $\mathfrak{g}$ that are not splitting (Exerc. $2b))$.

#### Remark 3 {#lie-viii-s2-n1-rem-3 .statement tag=00YN}

Let $\mathfrak{g}$ be a semi-simple Lie algebra, $\mathfrak{h}$ a Cartan subalgebra of $\mathfrak{g}$, and $\rho$ a finite dimensional injective representation of $\mathfrak{g}$ such that $\rho (\mathfrak{h})$ is diagonalizable. Then ad$_{\mathfrak{g}}x$ is diagonalizable for all $x\in \mathfrak{h}$ (Chap. VII, §2, no. 1, Example 2), so $\mathfrak{h}$ is splitting.

#### Remark 4 {#lie-viii-s2-n1-rem-4 .statement tag=00YO}

We shall see (§3, no. 3, Cor. of Prop. 10) that if $\mathfrak{h},\mathfrak{h}'$ are splitting Cartan subalgebras of $\mathfrak{g}$, there exists an elementary automorphism of $\mathfrak{g}$ transforming $\mathfrak{h}$ into $\mathfrak{h}'$.

#### Remark 5 {#lie-viii-s2-n1-rem-5 .statement tag=00YP}

Let $\mathfrak{g}$ be a reductive Lie algebra. Then $\mathfrak{g}=\mathfrak{c}\times \mathfrak{s}$ where $\mathfrak{c}$ is the centre of $\mathfrak{g}$ and $\mathfrak{s}=\mathscr{D}\mathfrak{g}$ is semi-simple. The Cartan subalgebras of $\mathfrak{g}$ are the subalgebras of the form $\mathfrak{h}=\mathfrak{c}\times \mathfrak{h}'$ where $\mathfrak{h}'$ is a Cartan subalgebra of $\mathfrak{s}$ (Chap. VII, §2, no. 1, Prop. 2). Then $\mathfrak{h}$ is called splitting if $\mathfrak{h}'$ is splitting relative to $\mathfrak{s}$. This leads in an obvious way to the definition of splittable or split reductive algebras.

### 2. ROOTS OF A SPLIT SEMI-SIMPLE LIE ALGEBRA

In this number, $(\mathfrak{g},\mathfrak{h})$ denotes a split semi-simple Lie algebra.

For any $\lambda \in \mathfrak{h}^*$, denote by $\mathfrak{g}^{\lambda}(\mathfrak{h})$, or simply by $\mathfrak{g}^{\lambda}$, the primary subspace of $\mathfrak{g}$ relative to $\lambda$ (cf. Chap. VII, §1, no. 3). Recall that $\mathfrak{g}^0=\mathfrak{h}$ (Chap. VII, §2, no. 1, Prop. 4), that $\mathfrak{g}$ is the direct sum of the $\mathfrak{g}^{\lambda}$ (Chap. VII, §1, no. 3, Prop. 8 and 9), that $\mathfrak{g}^{\lambda}$ is the set of $x\in \mathfrak{g}$ such that $[h, x] =\lambda (h)x$ for all $h\in \mathfrak{h}$ (Chap. VII, §2, no. 4, Cor. 1 of Th. 2), and that the weights of $\mathfrak{h}$ on $\mathfrak{g}$ are the linear forms $\lambda$ on $\mathfrak{h}$ such that $\mathfrak{g}^{\lambda}\not= 0$ (Chap. VII, §1, no. 1).

#### Definition 2 {#lie-viii-s2-def-2 .statement tag=00YQ}

A root of $(\mathfrak{g},\mathfrak{h})$ is a non-zero weight of $\mathfrak{h}$ on $\mathfrak{g}$.

Denote by $R(\mathfrak{g},\mathfrak{h})$, or simply by R, the set of roots of $(\mathfrak{g},\mathfrak{h})$. We have

$$
\mathfrak{g}=\mathfrak{h}\oplus \bigoplus_{\alpha\in R}\mathfrak{g}^{\alpha}
$$

#### Proposition 1 {#lie-viii-s2-prop-1 .statement tag=00YR}

Let $\alpha ,\beta$ be roots of $(\mathfrak{g},\mathfrak{h})$ and let $\langle \cdot ,\cdot \rangle$ be a non-degenerate invariant symmetric bilinear form on $\mathfrak{g}($for example the Killing form of $\mathfrak{g})$.

(i) If $\alpha +\beta \not= 0,\mathfrak{g}^{\alpha}$ and $\mathfrak{g}^{\beta}$ are orthogonal. The restriction of $\langle \cdot ,\cdot \rangle$ to $\mathfrak{g}^{\alpha}\times \mathfrak{g}^{-\alpha}$ is non-degenerate. The restriction of $\langle \cdot ,\cdot \rangle$ to $\mathfrak{h}$ is non-degenerate.

(ii) Let $x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$ and $h\in \mathfrak{h}$. Then $[x, y]\in \mathfrak{h}$ and

$$
\langle h,[x, y]\rangle =\alpha (h)\langle x, y\rangle
$$

Assertion (i) is a particular case of Prop. 10 (iii) of Chap. VII, §1, no. 3. If $x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$ and $h\in \mathfrak{h}$, we have $[x, y]\in \mathfrak{g}^{\alpha-\alpha}=\mathfrak{h}$, and

$$
\langle h,[x, y]\rangle =\langle [h, x], y\rangle =\langle \alpha (h)x, y\rangle =\alpha (h)\langle x, y\rangle
$$

#### Theorem 1 {#lie-viii-s2-thm-1 .statement tag=00YS}

Let $\alpha$ be a root of $(\mathfrak{g},\mathfrak{h})$.

(i) The vector space $\mathfrak{g}^{\alpha}$ is of dimension 1.

(ii) The vector subspace $\mathfrak{h}_{\alpha}= [\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}]$ of $\mathfrak{h}$ is of dimension 1. It contains a unique element $H_{\alpha}$ such that $\alpha (H_{\alpha}) = 2$.

(iii) The vector subspace $\mathfrak{s}_{\alpha}=\mathfrak{h}_{\alpha}+\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$ is a Lie subalgebra of $\mathfrak{g}$.

(iv) If $X_{\alpha}$ is a non-zero element of $\mathfrak{g}^{\alpha}$, there exists a unique $X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ such that $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$. Let $\varphi$ be the linear map from $\mathfrak{s}\mathfrak{l}(2, k)$ to $\mathfrak{g}$ that takes $X_+$ to $X_{\alpha},X_-$ to $X_{-\alpha}$, and $H$ to $H_{\alpha}$; then $\varphi$ is an isomorphism from the Lie algebra $\mathfrak{s}\mathfrak{l}(2, k)$ to the Lie algebra $\mathfrak{s}_{\alpha}$.

$a)$ Let $h_{\alpha}$ be the unique element of $\mathfrak{h}$ such that $\alpha (h) =\langle h_{\alpha}, h\rangle$ for all $h\in \mathfrak{h}$. By Prop. $1, [x, y] =\langle x, y\rangle h_{\alpha}$ for all $x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$; on the other hand $\langle \mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}\rangle  \not= 0$. Hence $\mathfrak{h}_{\alpha}= [\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}] =kh_{\alpha}$.

$b)$ Choose $x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$ such that $\langle x, y\rangle = 1$, so $[x, y] =h_{\alpha}$. Recall that $[h_{\alpha}, x] =\alpha (h_{\alpha})x, [h_{\alpha}, y] =-\alpha (h_{\alpha})y$. If $\alpha (h_{\alpha}) = 0$, it follows that $kx+ky+kh_{\alpha}$ is a nilpotent subalgebra $\mathfrak{t}$ of $\mathfrak{g}$; since $h_{\alpha}\in [\mathfrak{t},\mathfrak{t}]$, ad$_{\mathfrak{g}}h_{\alpha}$ is nilpotent (Chap. I, §5, no. 3, Th. 1), which is absurd since ad$_{\mathfrak{g}}h_{\alpha}$ is non-zero semi-simple. So $\alpha (h_{\alpha})\not= 0$. Hence there exists a unique $H_{\alpha}\in \mathfrak{h}_{\alpha}$ such that $\alpha (H_{\alpha}) = 2$, which proves (ii).

$c)$ Choose a non-zero element $X_{\alpha}$ of $\mathfrak{g}^{\alpha}$. There exists $X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ such that $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ (since $[X_{\alpha},\mathfrak{g}^{-\alpha}] =\mathfrak{h}_{\alpha}$ by $b))$. Then

$$
[H_{\alpha}, X_{\alpha}] =\alpha (H_{\alpha})X_{\alpha}= 2X_{\alpha},[H_{\alpha}, X_{-\alpha}] =-\alpha (H_{\alpha})X_{-\alpha}=-2X_{-\alpha}
$$

$$
[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}
$$

hence $kX_{\alpha}+kX_{-\alpha}+kH_{\alpha}$ is a subalgebra of $\mathfrak{g}$ and the linear map $\varphi$ from $\mathfrak{s}\mathfrak{l}(2, k)$ to $kX_{\alpha}+kX_{-\alpha}+kH_{\alpha}$ such that $\varphi (X_+) =X_{\alpha},\varphi (X_-) =X_{-\alpha}$, $\varphi (H) =H_{\alpha}$ is an isomorphism of Lie algebras.

$d)$ Assume that dim$\mathfrak{g}^{\alpha}>1$. Let $y$ be a non-zero element of $\mathfrak{g}^{-\alpha}$. There exists a non-zero element $X_{\alpha}$ of $\mathfrak{g}_{\alpha}$ such that $\langle y, X_{\alpha}\rangle = 0$. Choose $X_{-\alpha}$ as in $c)$, and consider the representation $\rho :u \rightarrow$ ad$_{\mathfrak{g}}\varphi (u)$ from $\mathfrak{s}\mathfrak{l}(2, k)$ to $\mathfrak{g}$. We have

$$
\rho (H)y= [\varphi (H), y] = [H_{\alpha}, y] =-2y
$$

$$
\rho (X_+)y= [\varphi (X_+), y] = [X_{\alpha}, y] =\langle X_{\alpha}, y\rangle h_{\alpha}= 0
$$

Thus, $y$ is primitive for $\rho$, of weight $-2$, which contradicts Prop. 2 of §1, no. 2. This proves (i).

$e)$ Assertion (iii) is now a consequence of $c)$. On the other hand, if $X_{\alpha}$ is a non-zero element of $\mathfrak{g}^{\alpha}$, the element $X_{-\alpha}$ constructed in $c)$ is the unique element of $\mathfrak{g}^{-\alpha}$ such that $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ since dim $\mathfrak{g}^{-\alpha}= 1$. The last assertion of (iv) is a consequence of $c)$. Q.E.D.

The notations $h_{\alpha},H_{\alpha},\mathfrak{s}_{\alpha}$ will be retained in what follows. (To define $h_{\alpha}$, we take $\langle \cdot ,\cdot \rangle$ equal to the Killing form.) If $X_{\alpha}$ is a non-zero element of $\mathfrak{g}^{\alpha}$, the isomorphism $\varphi$ of Th. 1 and the representation $u \rightarrow$ ad$_{\mathfrak{g}}\varphi (u)$ of $\mathfrak{s}\mathfrak{l}(2, k)$ on $\mathfrak{g}$ will be said to be associated to $X_{\alpha}$.

#### Corollary {#lie-viii-s2-n2-cor-1 .statement tag=00YT}

Let $\Phi$ be the Killing form of $\mathfrak{g}$. For all $a, b\in \mathfrak{h}$,

$$
\Phi (a, b) =\sum_{\gamma\in R}\gamma (a)\gamma (b)
$$

Indeed, ad $a$.ad $b$ leaves each $\mathfrak{g}^{\gamma}$ stable, and its restriction to $\mathfrak{g}^{\gamma}$ is the homothety with ratio $\gamma (a)\gamma (b)$; if $\gamma \not= 0$, dim$\mathfrak{g}^{\gamma}= 1$.

#### Proposition 2 {#lie-viii-s2-prop-2 .statement tag=00YU}

Let $\alpha , \beta \in R$.

(i) $\beta (H_{\alpha})\in \mathbf{Z}$.

(ii) If $\Phi$ denotes the Killing form of $\mathfrak{g},\Phi (H_{\alpha}, H_{\beta})\in \mathbf{Z}$.

Let $X_{\alpha}$ be a non-zero element of $\mathfrak{g}^{\alpha}$, and let $\rho$ be the representation of $\mathfrak{s}\mathfrak{l}(2, k)$ on $\mathfrak{g}$ associated to $X_{\alpha}$. The eigenvalues of $\rho (H)$ are 0 and the $\beta (H_{\alpha})$ for $\beta \in R$. Hence (i) follows from §1, no. 2, Cor. of Prop. 2. Assertion (ii) follows from (i) and the Cor. of Th. 1. Q.E.D.

Let $\alpha \in R,X_{\alpha}$ a non-zero element of $\mathfrak{g}^{\alpha},X_{-\alpha}$ the element of $\mathfrak{g}^{-\alpha}$ such that $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$, and $\rho$ the representation of $\mathfrak{s}\mathfrak{l}(2, k)$ on $\mathfrak{g}$ associated to $X_{\alpha}$. Let $\pi$ be the representation of $\mathbf{S}\mathbf{L}(2, k)$ on $\mathfrak{g}$ compatible with $\rho ($§1, no. 4, Th. 2). Since ad $X_{\alpha}$ is nilpotent (Chap. VII, §1, no. 3, Prop. 10 (iv)), $\pi (e^{X_+}) =e^{adX_{\alpha}}$ is an elementary automorphism of $\mathfrak{g}$. Similarly, $\pi (e^{X_-}) =$ $e^{adX_{-\alpha}}$ is an elementary automorphism of $\mathfrak{g}$. Hence $\pi (\mathbf{S}\mathbf{L}(2, k))\subset$ Aut$_e(\mathfrak{g})$. We make use of the notation $\theta (t)$ of §1, no. 5. For $t\in k^*$, put

$$
\theta_{\alpha}(t) =\pi (\theta (t)) =e^{adtX_{\alpha}}e^{adt^{-1}X_{-\alpha}}e^{adtX_{\alpha}} \tag{1}
$$

#### Lemma 1 {#lie-viii-s2-lem-1 .statement tag=00YV}

(i) For all $h\in \mathfrak{h},\theta_{\alpha}(t).h=h-\alpha (h)H_{\alpha}$.

(ii) For all $\beta \in R,\theta_{\alpha}(t)(\mathfrak{g}^{\beta}) =\mathfrak{g}^{\beta-\beta(H_{\alpha})\alpha}$.

(iii) If $\alpha , \beta \in R,\beta -\beta (H_{\alpha})\alpha \in R$.

Let $h\in \mathfrak{h}$. If $\alpha (h) = 0, [X_{\alpha}, h] = [X_{-\alpha}, h] = 0$, so $\theta_{\alpha}(t).h=h$. On the other hand, the formulas (5) of §1, no. 5 show that $\theta_{\alpha}(t).H_{\alpha}=-H_{\alpha}$. This proves assertion (i). It follows that $\theta_{\alpha}(t)^2|\mathfrak{h}=$ Id. If $x\in \mathfrak{g}^{\beta}$ and $h\in \mathfrak{h}$,

$$
[h, \theta_{\alpha}(t)x] =\theta_{\alpha}(t).[\theta_{\alpha}(t)h, x]-\beta (\theta_{\alpha}(t)h).\theta_{\alpha}(t)x
$$

$$
= (\beta (h)-\alpha (h)\beta (H_{\alpha})).\theta_{\alpha}(t)x
$$

$$
= (\beta -\beta (H_{\alpha})\alpha )(h).\theta_{\alpha}(t)x
$$

so $\theta_{\alpha}(t)x\in \mathfrak{g}^{\beta-\beta(H_{\alpha})\alpha}$. This proves (ii). Assertion (iii) follows from (ii).

#### Theorem 2 {#lie-viii-s2-thm-2 .statement tag=00YW}

(i) The set $R = R(\mathfrak{g},\mathfrak{h})$ is a reduced root system in $\mathfrak{h}^*$.

(ii) Let $\alpha \in R$. The map $s_{\alpha ,H_{\alpha}}:\lambda  \rightarrow \lambda -\lambda (H_{\alpha})\alpha$ from $\mathfrak{h}^*$ to $\mathfrak{h}^*$ is the unique reflection $s$ of $\mathfrak{h}^*$ such that $s(\alpha ) =-\alpha$ and $s(R) = R$. For all $t\in k^*$, $s$ is the transpose of $\theta_{\alpha}(t)|\mathfrak{h}$.

First, R generates $\mathfrak{h}^*$, for if $h\in \mathfrak{h}$ is such that $\alpha (h) = 0$ for all $\alpha \in R$, then ad $h= 0$ and hence $h= 0$ since the centre of $\mathfrak{g}$ is zero. By definition, $0\in /R$. Let $\alpha \in R$. Since $\alpha (H_{\alpha}) = 2,s=s_{\alpha ,H_{\alpha}}$ is a reflection such that $s(\alpha ) =-\alpha$. Then $s(R) = R$ by Lemma 1 (iii), and $\beta (H_{\alpha})\in \mathbf{Z}$ for all $\beta \in R$ (Prop. 2 (i)). This shows that R is a root system in $\mathfrak{h}^*$. For all $h\in \mathfrak{h}$ and $\lambda \in \mathfrak{h}^*$,

$$
\langle s(\lambda ), h\rangle =\langle \lambda -\lambda (H_{\alpha})\alpha , h\rangle =\langle \lambda , h-\alpha (h)H_{\alpha}\rangle =\langle \lambda , \theta_{\alpha}(t)h\rangle
$$

so $s$ is the transpose of $\theta_{\alpha}(t)|\mathfrak{h}$. Finally, we show that the root system R is reduced. Let $\alpha \in R$ and $y\in \mathfrak{g}^{2\alpha}$. Since $3\alpha  /\in R$ (Chap. VI, §1, no. 3, Prop. $8), [X_{\alpha}, y] = 0$; on the other hand, $[X_{-\alpha}, y]\in \mathfrak{g}^{-\alpha+2\alpha}=\mathfrak{g}^{\alpha}=kX_{\alpha}$, so $[X_{\alpha},[X_{-\alpha}, y]] = 0$; thus

$$
4y= 2\alpha (H_{\alpha})y= [H_{\alpha}, y] =-[[X_{\alpha}, X_{-\alpha}], y] = 0
$$

so $y= 0$ and $\mathfrak{g}^{2\alpha}= 0$. In other words, $2\alpha$ is not a root. Q.E.D.

Identify $\mathfrak{h}$ canonically with $\mathfrak{h}^{**}$. With the notations of Chap. VI, §1, no. 1, we then have, by Th. 2 (ii),

$H_{\alpha}=\alpha^{\vee}$ for all $\alpha \in R$. (2)

The $H_{\alpha}$ thus form the root system $R^{\vee}$ in $\mathfrak{h}$ inverse to R.

We shall call $R(\mathfrak{g},\mathfrak{h})$ the root system of $(\mathfrak{g},\mathfrak{h})$. The reflections $s_{\alpha ,H_{\alpha}}$ will be denoted simply by $s_{\alpha}$. The Weyl group, group of weights, Coxeter number $. .$. of $R(\mathfrak{g},\mathfrak{h})$ are called the Weyl group, group of weights, Coxeter number $. .$. of $(\mathfrak{g},\mathfrak{h})$. As in Chap. VI, §1, no. 1, we consider the Weyl group as operating not only on $\mathfrak{h}^*$, but also on $\mathfrak{h}$ by transport of structure, so that $s_{\alpha}=\theta_{\alpha}(t)|\mathfrak{h}$. Since the $\theta_{\alpha}(t)$ are elementary automorphisms of $\mathfrak{g}$, we have:

#### Corollary {#lie-viii-s2-n2-cor-2 .statement tag=00YX}

Every element of the Weyl group of $(\mathfrak{g},\mathfrak{h})$, operating on $\mathfrak{h}$, is the restriction to $\mathfrak{h}$ of an elementary automorphism of $\mathfrak{g}$.

For a converse of this result, see §5, no. 2, Prop. 4.

#### Remark 1 {#lie-viii-s2-n2-rem-1 .statement tag=00YY}

If $\mathfrak{h}_{\mathbf{Q}}$ (resp. $\mathfrak{h}^*_{\mathbf{Q}})$ denotes the $\mathbf{Q}$-vector subspace of $\mathfrak{h}$ (resp. $\mathfrak{h}^*)$ generated by the $H_{\alpha}$ (resp. the $\alpha )$, where $\alpha \in R$, then $\mathfrak{h}$ (resp. $\mathfrak{h}^*)$ can be identified canonically with $\mathfrak{h}_{\mathbf{Q}}\otimes_{\mathbf{Q}}k$ (resp. with $\mathfrak{h}^*_{\mathbf{Q}}\otimes_{\mathbf{Q}}k)$ and $\mathfrak{h}^*_{\mathbf{Q}}$ can be identified with the dual of $\mathfrak{h}_{\mathbf{Q}}$ (Chap. VI, §1, no. 1, Prop. 1). We call $\mathfrak{h}_{\mathbf{Q}}$ and $\mathfrak{h}^*_{\mathbf{Q}}$ the canonical $\mathbf{Q}$-structures on $\mathfrak{h}$ and $\mathfrak{h}^*($Algebra, Chap. II, §8, no. 1, Def. 1). When we mention $\mathbf{Q}$-rationality for a vector subspace of $\mathfrak{h}$, for a linear form on $\mathfrak{h}$, etc., we shall mean these structures, unless we indicate otherwise. When we mention Weyl chambers, or facets, of $R(\mathfrak{g},\mathfrak{h})$, we shall work in $\mathfrak{h}_{\mathbf{Q}}\otimes_{\mathbf{Q}}\mathbf{R}$ or $\mathfrak{h}^*_{\mathbf{Q}}\otimes_{\mathbf{Q}}\mathbf{R}$, that we shall denote by $\mathfrak{h}_{\mathbf{R}}$ and $\mathfrak{h}^*_{\mathbf{R}}$.

#### Remark 2 {#lie-viii-s2-n2-rem-2 .statement tag=00YZ}

The root system $R^{\vee}$ in $\mathfrak{h}$ defines a non-degenerate symmetric bilinear form $\beta$ on $\mathfrak{h}$ (Chap. VI, §1, no. 1, Prop. 3), namely the form $(a, b) \rightarrow$ $\sum_{\alpha\in R}\langle \alpha , a\rangle \langle \alpha , b\rangle$. By the Cor. to Th. 1, this form is just the restriction of the

Killing form to $\mathfrak{h}$. The extension of $\beta |\mathfrak{h}_{\mathbf{Q}}\times \mathfrak{h}_{\mathbf{Q}}$ to $\mathfrak{h}_{\mathbf{Q}}\otimes_{\mathbf{Q}}\mathbf{R}$ is positive non-degenerate (Chap. VI, §1, no. 1, Prop. 3). On the other hand, we see that the inverse form on $\mathfrak{h}^*$ of the restriction to $\mathfrak{h}$ of the Killing form on $\mathfrak{g}$ is the canonical bilinear form $\Phi_R$ of R (Chap. VI, §1, no. 12).

Let $(\mathfrak{g}_1,\mathfrak{h}_1), (\mathfrak{g}_2,\mathfrak{h}_2)$ be split semi-simple Lie algebras, $\varphi$ an isomorphism from $\mathfrak{g}_1$ to $\mathfrak{g}_2$ such that $\varphi (\mathfrak{h}_1) =\mathfrak{h}_2$. By transport of structure, the transpose of the map $\varphi |\mathfrak{h}_1$ takes $R(\mathfrak{g}_2,\mathfrak{h}_2)$ to $R(\mathfrak{g}_1,\mathfrak{h}_1)$.

#### Proposition 3 {#lie-viii-s2-prop-3 .statement tag=00Z0}

Let $\mathfrak{g}$ be a semi-simple Lie algebra, $\mathfrak{h}_1$ and $\mathfrak{h}_2$ splitting Cartan subalgebras of $\mathfrak{g}$. There exists an isomorphism from $\mathfrak{h}^*_1$ to $\mathfrak{h}^*_2$ that takes $R(\mathfrak{g},\mathfrak{h}_1)$ to $R(\mathfrak{g},\mathfrak{h}_2)$.

(For more precise results, see §3, no. 3, Cor. of Prop. 10, and §5, no. 3, Prop. 5).

Let $k'$ be an algebraic closure of $k,\mathfrak{g}'=\mathfrak{g}\otimes_kk',\mathfrak{h}'_i=\mathfrak{h}_i\otimes_kk'$. Then $R(\mathfrak{g}',\mathfrak{h}'_i)$ is the image of $R(\mathfrak{g},\mathfrak{h}_i)$ under the map $\lambda  \rightarrow \lambda \otimes 1$ from $\mathfrak{h}^*_i$ to $\mathfrak{h}^*_i\otimes_kk'={\mathfrak{h}'_i}^*$. By Chap. VII, §3, no. 2, Th. 1, there exists an automorphism of $\mathfrak{g}'$ taking $\mathfrak{h}'_1$ to $\mathfrak{h}'_2$, hence an isomorphism $\varphi$ from ${\mathfrak{h}'_1}^*$ to ${\mathfrak{h}'_2}^*$ that takes $R(\mathfrak{g}',\mathfrak{h}'_1)$ to $R(\mathfrak{g}',\mathfrak{h}'_2)$. Then $\varphi |\mathfrak{h}^*_1$ takes $R(\mathfrak{g},\mathfrak{h}_1)$ to $R(\mathfrak{g},\mathfrak{h}_2)$, and hence $\mathfrak{h}^*_1$ to $\mathfrak{h}^*_2$. Q.E.D.

In view of Prop. 3, the root system of $(\mathfrak{g},\mathfrak{h})$ depends, up to isomorphism, only on $\mathfrak{g}$ and not on $\mathfrak{h}$. In the same way, the Weyl group, group of weights $. .$. of $(\mathfrak{g},\mathfrak{h})$ are simply called, by abuse of language, the Weyl group, group of weights $. .$. of $\mathfrak{g}$ (cf. also §5, no. 3, Remark 2). If the Dynkin graph of $\mathfrak{g}$ is of type $A_l$, or $B_l,. .$. (cf. Chap. VI, §4, no. 2, Th. 3), we say that $\mathfrak{g}$ is of type $A_l$, or $B_l,. .$..

Recall that, if $\alpha$ and $\beta$ are linearly independent roots, the set of $j\in \mathbf{Z}$ such that $\beta +j\alpha \in R$ is an interval $[-q, p]$ of $\mathbf{Z}$ containing 0, with $p-q=$ $-\langle \beta , \alpha^{\vee}\rangle =-\beta (H_{\alpha})$ (Chap. VI, §1, no. 3, Prop. 9).

#### Proposition 4 {#lie-viii-s2-prop-4 .statement tag=00Z1}

Let $\alpha$ and $\beta$ be linearly independent roots. Let $p$ (resp. $q)$ be the largest integer $j$ such that $\beta +j\alpha$ (resp. $\beta -j\alpha )$ is a root.

(i) The vector subspace $\sum_{-q\leq j\leq p}\mathfrak{g}^{\beta+j\alpha}$ of $\mathfrak{g}$ is a simple $\mathfrak{s}_{\alpha}$-module of dimension $p+q+ 1$.

(ii) If $\alpha +\beta$ is a root, then $[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}] =\mathfrak{g}^{\alpha+\beta}$.

Let $X_{\alpha}$ (resp. $x)$ be a non-zero element of $\mathfrak{g}^{\alpha}$ (resp. $\mathfrak{g}^{\beta+p\alpha})$. Then

$$
[X_{\alpha}, x]\in \mathfrak{g}^{\beta+(p+1)\alpha}= 0
$$

$$
[H_{\alpha}, x] = (\beta (H_{\alpha}) +p\alpha (H_{\alpha}))x= (-p+q+ 2p)x= (p+q)x
$$

Thus, $x$ is primitive of weight $p+q$ for the representation of $\mathfrak{s}\mathfrak{l}(2, k)$ on $\mathfrak{g}$ associated to $X_{\alpha}$; but the $\mathfrak{s}\mathfrak{l}(2, k$)-module $\sum_{-q\leq j\leq p}\mathfrak{g}^{\beta+j\alpha}$ is of dimension $p+q+ 1$; hence it is simple (§1, no. 2, Prop. 2). If $\alpha +\beta \in R$, then $p\geq 1$, so the elements of $\mathfrak{g}^{\beta}$ are not primitive, and hence $[X_{\alpha},\mathfrak{g}^{\beta}]\not= 0$. Since $[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}]\subset$ $\mathfrak{g}^{\alpha+\beta}$, we see finally that $[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}] =\mathfrak{g}^{\alpha+\beta}$.

#### Remark 3 {#lie-viii-s2-n2-rem-3 .statement tag=00Z2}

Recall that, by Chap. VI, §1, no. 3, Cor. of Prop. 9, the integer $p+q+ 1$ can only take the values $1,2,3,4$.

#### Remark 4 {#lie-viii-s2-n2-rem-4 .statement tag=00Z3}

Let $(\mathfrak{g},\mathfrak{h})$ be a split reductive Lie algebra, $\mathfrak{c}$ the centre of $\mathfrak{g},\mathfrak{g}'=\mathscr{D}\mathfrak{g}$, $\mathfrak{h}'=\mathfrak{h}\cap \mathfrak{g}'$. Then $\mathfrak{h}=\mathfrak{c}\times \mathfrak{h}'$, and we identify $\mathfrak{h}^{'*}$ with a vector subspace of $\mathfrak{h}^*$. For any $\lambda \in \mathfrak{h}^*$ such that $\lambda \not= 0$, the primary subspace $\mathfrak{g}^{\lambda}$ relative to $\lambda$ is equal to ${\mathfrak{g}'}^{\lambda|\mathfrak{h}'}$. A non-zero weight of $\mathfrak{h}$ on $\mathfrak{g}$ is called a root of $(\mathfrak{g},\mathfrak{h})$; every root vanishes on $\mathfrak{c}$. Denote by $R(\mathfrak{g},\mathfrak{h})$ the set of roots of $(\mathfrak{g},\mathfrak{h})$; it can be identified canonically with $R(\mathfrak{g}',\mathfrak{h}')$. Let $\alpha \in R(\mathfrak{g},\mathfrak{h})$. We define $h_{\alpha},H_{\alpha}$, $\mathfrak{s}_{\alpha}$, the isomorphisms $\mathfrak{s}\mathfrak{l}(2, k)\rightarrow \mathfrak{s}_{\alpha}$, and the representations of $\mathfrak{s}\mathfrak{l}(2, k)$ on $\mathfrak{g}$ associated to $\alpha$, as in the semi-simple case.

### 3. INVARIANT BILINEAR FORMS

#### Proposition 5 {#lie-viii-s2-prop-5 .statement tag=00Z4}

Let $(\mathfrak{g},\mathfrak{h})$ be a split semi-simple Lie algebra, $\Phi$ an invariant symmetric bilinear form on $\mathfrak{g}$, and W the Weyl group of $(\mathfrak{g},\mathfrak{h})$. Then the restriction $\Phi '$ of $\Phi$ to $\mathfrak{h}$ is invariant under W. Moreover, if $\Phi$ is non-degenerate, so is $\Phi '$.

Let $\alpha \in R$, let $X_{\alpha}$ be a non-zero element of $\mathfrak{g}^{\alpha},\rho$ the associated representation of $\mathfrak{s}\mathfrak{l}(2, k)$ on $\mathfrak{g}$, and $\pi$ the representation of $\mathbf{S}\mathbf{L}(2, k)$ on $\mathfrak{g}$ compatible with $\rho$. Then $\Phi$ is invariant under $\rho$, and hence under $\pi ($§1, no. 4). In particular, $\Phi '$ is invariant under $\theta_{\alpha}(t)|\mathfrak{h}$ (no. 2), and hence under W. The last assertion follows from Prop. 1 (i).

#### Proposition 6 {#lie-viii-s2-prop-6 .statement tag=00Z5}

Let $(\mathfrak{g},\mathfrak{h})$ be a split semi-simple Lie algebra, $\Phi$ a non-degenerate invariant symmetric bilinear form on $\mathfrak{g}$. For all $\alpha \in R$, let $X_{\alpha}$ be a non-zero element of $\mathfrak{g}^{\alpha}$. Let $(H_i)_{i\in I}$ be a basis of $\mathfrak{h}$, and $(H'_i)_{i\in I}$ the basis of $\mathfrak{h}$ such that $\Phi (H_i, H'_j) =\delta_{ij}$. The Casimir element associated to $\Phi$ in the enveloping algebra of $\mathfrak{g}$ (Chap. I, §3, no. 7) is then

$\sum$ 1 $\sum'$

$$
X_{\alpha}X_{-\alpha}+H_iH_i
$$

$$
\Phi (X_{\alpha}, X_{-\alpha})
$$

$\alpha \in Ri\in I$

Indeed, by Prop. $1,\Phi (H_i, X_{\alpha}) =\Phi (H'_i, X_{\alpha}) = 0$ for all $i\in I,\alpha \in R$, and $\Phi (\frac{1}{\Phi(X_{\alpha},X_{-\alpha})}X_{\alpha}, X_{-\beta})=\delta_{\alpha \beta}$ for all $\alpha , \beta \in R$.

### 4. THE COEFFICIENTS N$_{\boldsymbol{\alpha \beta }}$

In this number, we again denote by $(\mathfrak{g},\mathfrak{h})$ a split semi-simple Lie algebra.

#### Lemma 2 {#lie-viii-s2-lem-2 .statement tag=00Z6}

There exists a family $(X_{\alpha})_{\alpha\in R}$ such that, for all $\alpha \in R$,

$X_{\alpha}\in \mathfrak{g}^{\alpha}$ and $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$.

Let $R_1$ be a subset of R such that $R = R_1\cup (-R_1)$ and $R_1\cap (-R_1) =\emptyset$. For $\alpha \in R_1$, choose an arbitrary non-zero element $X_{\alpha}$ of $\mathfrak{g}^{\alpha}$. There exists a unique $X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ such that $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ (Th. 1 (iv)). Then

$$
[X_{-\alpha}, X_{\alpha}] =H_{\alpha}=-H_{-\alpha}.Q.E.D
$$

If $(X_{\alpha})_{\alpha\in R}$ is one family satisfying the conditions of Lemma 2, the most general family satisfying these conditions is $(t_{\alpha}X_{\alpha})_{\alpha\in R}$ where $t_{\alpha}\in k^*$ and $t_{\alpha}t_{-\alpha}= 1$ for all $\alpha \in R$.

In the remainder of this number, we denote by $(X_{\alpha})_{\alpha\in R}$ a family satisfying the conditions of Lemma 2. We denote by $\langle \cdot ,\cdot \rangle$ a non-degenerate invariant symmetric bilinear form on $\mathfrak{g}$.

Every $x\in \mathfrak{g}$ can be written uniquely in the form

$$
x=h+\sum_{\alpha\in R}\mu_{\alpha}X_{\alpha}(h\in \mathfrak{h}, \mu_{\alpha}\in k)
$$

The bracket of two such elements can be calculated by means of the following formulas:

$$
[h, X_{\alpha}] =\alpha (h)X_{\alpha}
$$

0 if $\alpha +\beta  /\in R\cup  \{0\}$

$[X_{\alpha}, X_{\beta}] =-H_{\alpha}$ if $\alpha +\beta = 0$

$N_{\alpha \beta}X_{\alpha+\beta}$ if $\alpha +\beta \in R$

the $N_{\alpha \beta}$ being non-zero elements of $k$.

#### Lemma 3 {#lie-viii-s2-lem-3 .statement tag=00Z7}

For all $\alpha \in R$,

$$
\langle X_{\alpha}, X_{-\alpha}\rangle =-1\langle H_{\alpha}, H_{\alpha}\rangle
$$

2

Indeed,

$$
2\langle X_{\alpha}, X_{-\alpha}\rangle =\langle \alpha (H_{\alpha})X_{\alpha}, X_{-\alpha}\rangle =\langle [H_{\alpha}, X_{\alpha}], X_{-\alpha}\rangle
$$

$$
=\langle H_{\alpha},[X_{\alpha}, X_{-\alpha}]\rangle =-\langle H_{\alpha}, H_{\alpha}\rangle
$$

#### Lemma 4 {#lie-viii-s2-lem-4 .statement tag=00Z8}

Let $\alpha , \beta \in R$ be such that $\alpha +\beta \in R$. Let $p$ (resp. $q)$ be the largest integer $j$ such that $\beta +j\alpha \in R$ (resp. $\beta -j\alpha \in R)$. Then,

$$
N_{\alpha ,\beta}N_{-\alpha ,\alpha+\beta}=-p(q+ 1) \tag{3}
$$

$$
N_{-\alpha ,\alpha+\beta}\langle H_{\beta}, H_{\beta}\rangle =-N_{-\alpha ,-\beta}\langle H_{\alpha+\beta}, H_{\alpha+\beta}\rangle \tag{4}
$$

$$
N_{\alpha ,\beta}N_{-\alpha ,-\beta}= (q+ 1)^2 \tag{5}
$$

Let $\rho$ be the representation of $\mathfrak{s}\mathfrak{l}(2, k)$ on $\mathfrak{g}$ defined by $X_{\alpha}$. The element $e=X_{\beta+p\alpha}$ is primitive of weight $p+q$ (Prop. 4 (i)). Put

$$
(-1)^nn
$$

$e_n=\rho (X_-)e$ for $n\geq 0$.

$n$!

By Prop. 1 of §1,

(ad $X_{\alpha})e_p= (q+ 1)e_{p-1}$

(ad $X_{-\alpha}$)(ad $X_{\alpha})e_p=-p(q+ 1)e_p$.

This proves (3) since $e_p$ is a non-zero element of $\mathfrak{g}^{\beta}$.

The form $\langle \cdot ,\cdot \rangle$ being invariant, we have

$$
\langle [X_{-\alpha}, X_{\alpha+\beta}], X_{-\beta}\rangle =-\langle X_{\alpha+\beta},[X_{-\alpha}, X_{-\beta}]\rangle
$$

so

$$
N_{-\alpha ,\alpha+\beta}\langle X_{\beta}, X_{-\beta}\rangle =-N_{-\alpha ,-\beta}\langle X_{\alpha+\beta}, X_{-\alpha-\beta}\rangle
$$

which, in view of Lemma 3, proves (4).

The restriction of $\langle \cdot ,\cdot \rangle$ to $\mathfrak{h}$ is non-degenerate and invariant under the Weyl group (Prop. 5). Identify $\mathfrak{h}$ and $\mathfrak{h}^*$ by means of this restriction. If $\gamma \in R,H_{\gamma}$ is identified with $2\gamma /\langle \gamma , \gamma \rangle$ (Chap. VI, §1, no. 1, Lemma 2); hence, for all $\gamma , \delta \in R$,

$$
\langle \gamma , \gamma \rangle \langle H_{\delta}, H_{\delta}\rangle
$$

$$
\overline{\langle\delta , \delta\rangle}=\overline{\langle H_{\gamma}, H_{\gamma}\rangle} \tag{6}
$$

Now, by Chap. VI, §1, no. 3, Prop. 10,

$$
\langle \alpha +\beta , \alpha +\beta \rangle q+ 1
$$

= (7)

$$
\langle \beta , \beta \rangle p
$$

so, by (3), (4), (6), (7),

$$
\langle H_{\beta}, H_{\beta}\rangle
$$

$$
N_{\alpha ,\beta}N_{-\alpha ,-\beta}=-N_{\alpha ,\beta}N_{-\alpha ,\alpha+\beta}
$$

$$
\langle H_{\alpha+\beta}, H_{\alpha+\beta}\rangle
$$

$$
q+ 1
$$

$$
=-N_{\alpha ,\beta}N_{-\alpha ,\alpha+\beta}= (q+ 1)^2
$$

$$
p
$$

#### Definition 3 {#lie-viii-s2-def-3 .statement tag=00Z9}

A Chevalley system for $(\mathfrak{g},\mathfrak{h})$ is a family $(X_{\alpha})_{\alpha\in R}$ such that

(i) $X_{\alpha}\in \mathfrak{g}^{\alpha}$ for all $\alpha \in R$;

(ii) $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ for all $\alpha \in R$;

(iii) the linear map from $\mathfrak{g}$ to $\mathfrak{g}$ which is equal to $-1$ on $\mathfrak{h}$ and which takes $X_{\alpha}$ to $X_{-\alpha}$ for all $\alpha \in R$ is an automorphism of $\mathfrak{g}$.

The extension of this definition to the case where $(\mathfrak{g},\mathfrak{h})$ is split reductive is immediate.

We shall show (§4, no. 4, Cor. of Prop. 5) that Chevalley systems for $(\mathfrak{g},\mathfrak{h})$ exist.

#### Proposition 7 {#lie-viii-s2-prop-7 .statement tag=00ZA}

Let $(X_{\alpha})_{\alpha\in R}$ be a Chevalley system for $(\mathfrak{g},\mathfrak{h})$. We retain the notation of Lemma 4. Then, $N_{-\alpha ,-\beta}= N_{\alpha ,\beta}$ and $N_{\alpha ,\beta}=\pm (q+ 1)$ for $\alpha , \beta , \alpha +\beta \in R$.

Let $\varphi$ be the automorphism of $\mathfrak{g}$ considered in Def. 3 (iii). Then

$$
N_{-\alpha ,-\beta}X_{-\alpha-\beta}= [X_{-\alpha}, X_{-\beta}] = [\varphi (X_{\alpha}), \varphi (X_{\beta})] =\varphi ([X_{\alpha}, X_{\beta}])
$$

$$
=\varphi (N_{\alpha ,\beta}X_{\alpha+\beta}) = N_{\alpha ,\beta}X_{-\alpha-\beta}
$$

so $N_{-\alpha ,-\beta}= N_{\alpha ,\beta}$. Now $N_{\alpha ,\beta}=\pm (q+ 1)$ by (5).

#### Proposition 8 {#lie-viii-s2-prop-8 .statement tag=00ZB}

Let $(X_{\alpha})_{\alpha\in R}$ be a Chevalley system for $(\mathfrak{g},\mathfrak{h})$. Let M be a $\mathbf{Z}$-submodule of $\mathfrak{h}$ containing the $H_{\alpha}$ and contained in the group of weights of $R^{\vee}$. Let $\mathfrak{g}_{\mathbf{Z}}$ be the $\mathbf{Z}$-submodule of $\mathfrak{g}$ generated by M and the $X_{\alpha}$. Then $\mathfrak{g}_{\mathbf{Z}}$ is a $\mathbf{Z}$-Lie subalgebra of $\mathfrak{g}$, and the canonical map from $\mathfrak{g}_{\mathbf{Z}}\otimes_{\mathbf{Z}}k$ to $\mathfrak{g}$ is an isomorphism.

If $\alpha , \beta \in R$ are such that $\alpha +\beta \in R$, then $N_{\alpha ,\beta}\in \mathbf{Z}$ (Prop. 7). On the other hand, if $\alpha \in R$ and $h\in M$, then $\alpha (h)\in \mathbf{Z}$ (Chap. VI, §1, no. 9). This proves that $\mathfrak{g}_{\mathbf{Z}}$ is a $\mathbf{Z}$-Lie subalgebra of $\mathfrak{g}$. On the other hand, M is a free abelian group of rank dim$\mathfrak{h}($Algebra, Chap. VII, §3, Th. 1), so $\mathfrak{g}_{\mathbf{Z}}$ is a free abelian group of rank dim$\mathfrak{g}$; this implies the last assertion.

### Exercises {#lie-viii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
