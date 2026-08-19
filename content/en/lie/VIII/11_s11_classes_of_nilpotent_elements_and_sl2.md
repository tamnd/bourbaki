---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 11
section_title: Classes of nilpotent elements and sl2 -triplets
lang: en
source: lie-vii-ix
book_pages: 163-173, 261-266
pdf_pages: 0171-0181, 0269-0274
extraction: native+ocr
subsections:
    - "no": 1
      title: DEFINITION OF $\mathfrak{s}\mathfrak{l}_{2}$-TRIPLETS
      page: 163
      pdf_page: 171
    - "no": 2
      title: $\mathfrak{s}\mathfrak{l}_{2}$-TRIPLETS IN SEMI-SIMPLE LIE ALGEBRAS
      page: 165
      pdf_page: 173
    - "no": 3
      title: SIMPLE ELEMENTS
      page: 167
      pdf_page: 175
    - "no": 4
      title: PRINCIPAL ELEMENTS
      page: 170
      pdf_page: 178
statements: 29
exercises: 17
content_sha256: c0d8b9889a1fd801f649977579ba93f112fbe7fbc77b9893c748cf4521cf283a
---

## § 11. CLASSES OF NILPOTENT ELEMENTS AND $\mathfrak{s}\mathfrak{l}_{2}$-TRIPLETS

In this paragraph, $\mathfrak{g}$ denotes a finite dimensional Lie algebra.

### 1. DEFINITION OF $\mathfrak{s}\mathfrak{l}_{2}$-TRIPLETS

#### Definition 1 {#lie-viii-s11-def-1 .statement tag=0170}

An $\mathfrak{s}\mathfrak{l}_2$-triplet in $\mathfrak{g}$ is a sequence $(x, h, y)$ of elements of $\mathfrak{g}$, distinct from $(0,0,0)$, such that

$$
[h, x] = 2x,[h, y] =-2y,[x, y] =-h
$$

Let $(x, h, y)$ be an $\mathfrak{s}\mathfrak{l}_2$-triplet in $\mathfrak{g}$. The linear map $\tau$ from $\mathfrak{s}\mathfrak{l}(2, k)$ to $\mathfrak{g}$ such that $\tau (X_+) =x, \tau (H) =h, \tau (X_-) =y$ is a homomorphism which is non-zero and hence injective (since $\mathfrak{s}\mathfrak{l}(2, k)$ is simple), and with image $kx+kh+ky$. We thus obtain a canonical bijection from the set of $\mathfrak{s}\mathfrak{l}_2$-triplets in $\mathfrak{g}$ to the set of injective homomorphisms from $\mathfrak{s}\mathfrak{l}(2, k)$ to $\mathfrak{g}$. If $\mathfrak{g}$ is semi-simple and if $(x, h, y)$ is an $\mathfrak{s}\mathfrak{l}_2$-triplet in $\mathfrak{g}$, then $x$ and $y$ are nilpotent elements of $\mathfrak{g}$ and $h$ is a semi-simple element of $\mathfrak{g}$ (Chap. I, §6, no. 3, Prop. 4).

#### Lemma 1 {#lie-viii-s11-lem-1 .statement tag=0171}

Let $x, h, y, y'\in \mathfrak{g}$. If $(x, h, y)$ and $(x, h, y')$ are $\mathfrak{s}\mathfrak{l}_2$-triplets in $\mathfrak{g}$, then $y=y'$.

Indeed, $y-y'\in$ Ker(ad$_{\mathfrak{g}}x$) and (ad$_{\mathfrak{g}}h$)$(y-y') =-2(y-y')$. But ad$_{\mathfrak{g}}x$ is injective on Ker($p+$ ad$_{\mathfrak{g}}h$) for every integer $p >0 ($§1, no. 2, Cor. of Prop. 2).

#### Lemma 2 {#lie-viii-s11-lem-2 .statement tag=0172}

Let $\mathfrak{n}$ be a subalgebra of $\mathfrak{g}$ such that, for all $n\in \mathfrak{n}$, ad$_{\mathfrak{g}}(n)$ is nilpotent. Let $h\in \mathfrak{g}$ be such that $[h,\mathfrak{n}] =\mathfrak{n}$. Then $e^{ad_{\mathfrak{g}}\mathfrak{n}}.h=h+\mathfrak{n}$.

It is clear that $e^{ad_{\mathfrak{g}}(\mathfrak{n})}.h\subset h+\mathfrak{n}$. We shall prove that, if $v\in \mathfrak{n}$, then $h+v\in e^{ad_{\mathfrak{g}}(\mathfrak{n})}.h$. It suffices to prove that $h+v\in e^{ad_{\mathfrak{g}}(\mathfrak{n})}.h+\mathscr{C}0\mathfrak{n}$ for all $p\geq 1$ (since $\mathscr{C}^p\mathfrak{n}= 0$ for sufficiently large $p$). This is clear for $p= 1$ since $\mathscr{C}^1\mathfrak{n}=\mathfrak{n}$. Assume now that we have proved the existence of $y_p\in \mathfrak{n}$ and $z_p\in \mathscr{C}^p\mathfrak{n}$ such that $h+v=e^{ad_{\mathfrak{g}}y_p}.h+z_p$. Since (ad$_{\mathfrak{g}}h$)$(\mathfrak{n}) =\mathfrak{n}$, (ad$_{\mathfrak{g}}h$)$|\mathfrak{n}$ is a bijection from $\mathfrak{n}$ to $\mathfrak{n}$, hence its restriction to $\mathscr{C}^p\mathfrak{n}$, which leaves $\mathscr{C}^p\mathfrak{n}$ stable, is also bijective; consequently, there exists $z\in \mathscr{C}^p\mathfrak{n}$ such that $z_p= [z, h]$. Then

$$
e^{ad_{\mathfrak{g}}(y_p+z)}h-e^{ad_{\mathfrak{g}}y_p}h\in [z, h] +\mathscr{C}^{p+1}\mathfrak{n}
$$

so

$$
e^{ad_{\mathfrak{g}}(y_p+z)}h\in h+v-z_p+ [z, h] +\mathscr{C}^{p+1}\mathfrak{n}=h+v+\mathscr{C}^{p+1}\mathfrak{n}
$$

which establishes our assertion by induction on $p$.

#### Lemma 3 {#lie-viii-s11-lem-3 .statement tag=0173}

Let $x\in \mathfrak{g},\mathfrak{p}=$ Ker(ad $x$)$,\mathfrak{q}=$ Im(ad $x$). Then $[\mathfrak{p},\mathfrak{q}]\subset \mathfrak{q}$, and $\mathfrak{p}\cap \mathfrak{q}$ is a subalgebra of $\mathfrak{g}$.

If $u\in \mathfrak{p}$ and $v\in \mathfrak{q}$, there exists $w\in \mathfrak{g}$ such that $v= [x, w]$, so

$$
[u, v] = [u,[x, w]] = [x,[u, w]]-[[x, u], w] = [x,[u, w]]\in \mathfrak{q}
$$

On the other hand, $\mathfrak{p}$ is a subalgebra of $\mathfrak{g}$, so $[\mathfrak{p}\cap \mathfrak{q},\mathfrak{p}\cap \mathfrak{q}]\subset \mathfrak{p}\cap \mathfrak{q}$.

#### Lemma 4 {#lie-viii-s11-lem-4 .statement tag=0174}

Let $(x, h, y)$ and $(x, h', y')$ be $\mathfrak{s}\mathfrak{l}_2$-triplets in $\mathfrak{g}$. There exists $z\in \mathfrak{g}$ such that ad$_{\mathfrak{g}}z$ is nilpotent and such that

$$
e^{ad_{\mathfrak{g}}z}x=x,e^{ad_{\mathfrak{g}}z}h=h',e^{ad_{\mathfrak{g}}z}y=y'
$$

Let $\mathfrak{n}=$ Ker(ad $x$)$\cap$ Im(ad $x$). For all $p\in \mathbf{Z}$, let $\mathfrak{g}_p=$ Ker(ad $h-p$). By §1, no. 3 (applied to the adjoint representation of $kx+ky+kh$ on $\mathfrak{g}$), we have that $\mathfrak{n}\subset \sum_{p>0}\mathfrak{g}_p$, so ad$_{\mathfrak{g}}n$ is nilpotent for all $n\in \mathfrak{n}$, and $[h,\mathfrak{n}] =\mathfrak{n}$. We have $[x, h'-h] = 0$ and $[x, y-y'] =h'-h$, so $h'-h\in \mathfrak{n}$. By Lemmas 2 and 3, there exists $z\in \mathfrak{n}$ such that $e^{ad_{\mathfrak{g}}z}h=h'$. Since $z\in$ Ker ad$_{\mathfrak{g}}x$, we have $e^{ad_{\mathfrak{g}}z}x=x$. Lemma 1 now proves that $e^{ad_{\mathfrak{g}}z}y=y'$. Q.E.D.

Let G be a group of automorphisms of $\mathfrak{g}$. Then two $\mathfrak{s}\mathfrak{l}_2$-triplets $(x, h, y)$, $(x', h', y')$ are said to be G-conjugate if there exists $g\in G$ such that $gx=x'$, $gh=h', gy=y'$.

#### Proposition 1 {#lie-viii-s11-prop-1 .statement tag=0175}

Let G be a group of automorphisms of $\mathfrak{g}$ containing Aut$_e(\mathfrak{g})$. Let $(x, h, y)$ and $(x', h', y')$ be $\mathfrak{s}\mathfrak{l}_2$-triplets in $\mathfrak{g}$. Let

$$
\mathfrak{t}=kx+kh+ky,\mathfrak{t}'=kx'+kh'+ky'
$$

Consider the following conditions:

(i) $x$ and $x'$ are G-conjugate;

(ii) $(x, h, y)$ and $(x', h', y')$ are G-conjugate;

(iii) $\mathfrak{t}$ and $\mathfrak{t}'$ are G-conjugate.

We have (i) $\Leftarrow \Rightarrow$ (ii) $=\Rightarrow$ (iii). If $k$ is algebraically closed, the three conditions are equivalent.

(i) $\Leftarrow \Rightarrow$ (ii): This follows from Lemma 4.

(ii) $=\Rightarrow$ (iii): This is clear.

We assume that $k$ is algebraically closed and prove that (iii) $=\Rightarrow$ (i). We treat first the case in which $\mathfrak{t}=\mathfrak{t}'=\mathfrak{g}=\mathfrak{s}\mathfrak{l}(2, k)$. Since ad$_{\mathfrak{g}}x$ is nilpotent, the endomorphism $x$ of $k^2$ is nilpotent (Chap. I, §6, Th. 3), so there exists a matrix $A\in \mathbf{G}\mathbf{L}(2, k)$ such that $AxA^{-1}=X$, and consequently an automorphism $\alpha$ of $\mathfrak{s}\mathfrak{l}(2, k)$ such that $\alpha (x) =x'$; now $\alpha \in$ Aut$_e(\mathfrak{g}) ($§5, no. 3, Cor. 2 of Prop. 5). We now pass to the general case; we assume that $\mathfrak{t}$ and $\mathfrak{t}'$ are G-conjugate and prove that $x$ and $x'$ are G-conjugate. We can assume that $\mathfrak{t}=\mathfrak{t}'$. By the preceding, there exists $\beta \in$ Aut$_e(\mathfrak{t})$ such that $\beta x=x'$. Now, if $t\in \mathfrak{t}$ is such that ad$_{\mathfrak{t}}t$ is nilpotent, then ad$_{\mathfrak{g}}t$ is nilpotent; so $\beta$ extends to an element of Aut$_e(\mathfrak{g})$.

#### Remark {#lie-viii-s11-n1-rem-1 .statement tag=0176}

The three conditions of Prop. 1 are equivalent if we assume only that $k=k^2$ (cf. Exerc. 1).

### 2. $\mathfrak{s}\mathfrak{l}_{2}$-TRIPLETS IN SEMI-SIMPLE LIE ALGEBRAS

#### Lemma 5 {#lie-viii-s11-lem-5 .statement tag=0177}

Let V be a finite dimensional vector space, A and B endomorphisms of V. Assume that A is nilpotent and that $[A,[A,B]] = 0$. Then AB is nilpotent.

Put $C = [A,B]$. Since $[A,C] = 0$,

$[A$, BC$^p] = [A,B]C^p= C^{p+1}$

for every integer $p\geq 0$. Consequently, Tr(C$^p$) $= 0$ for $p\geq 1$, which proves that C is nilpotent (Algebra, Chap. VII, §3, no. 5, Cor. 4 of Prop. 13). Now let $\overline{k}$ be an algebraic closure of $k$, and let $\lambda \in \overline{k},x\in V\otimes_k\overline{k}$ be such that AB$x=\lambda x$, $x\not= 0$. The relation $[[B,A],A] = 0$ shows that $[B,A^p] =p[B,A]A^{p-1}$ for every integer $p\geq 0$. Let $r$ be the smallest integer such that $A^rx= 0$. Then

$\lambda A^{r-1}x= A^{r-1}$AB$x= A^rBx=$ BA$^rx-[B,A^r]x=-r[B,A]A^{r-1}x$.

Since $[B,A]$ is nilpotent and since $A^{r-1}x\not= 0$, this proves that $\lambda = 0$. Thus, all the eigenvalues of AB are zero, hence the lemma.

#### Lemma 6 {#lie-viii-s11-lem-6 .statement tag=0178}

Let $h, x\in \mathfrak{g}$ be such that $[h, x] = 2x$ and $h\in$ (ad $x$)$(\mathfrak{g})$. Then there exists $y\in \mathfrak{g}$ such that $(x, h, y)$ is either $(0,0,0)$ or an $\mathfrak{s}\mathfrak{l}_2$-triplet.

Let $\mathfrak{g}'$ be the solvable Lie algebra $kh+kx$. Since $x\in [\mathfrak{g}',\mathfrak{g}']$, ad$_{\mathfrak{g}}x$ is nilpotent (Chap. I, §5, no. 3, Th. 1); let $\mathfrak{n}$ be its kernel. Since [ad $h$, ad $x] =$ 2 ad $x$, we have (ad $h$)$\mathfrak{n}\subset \mathfrak{n}$. Let $z\in \mathfrak{g}$ be such that $h=-[x, z]$. For any integer $n\geq 0$, put $M_n=$ (ad $x$)$^n\mathfrak{g}$. If $n >0$, we have (§1, no. 1, Lemma 1)

[ad $z$,(ad $x$)$^n] =n$((ad $h$)$-n+$ 1)(ad $x$)$^{n-1}$

so, if $u\in M_{n-1}$,

$n$((ad $h$)$-n+ 1$)$u\in$ (ad $z$)(ad $x$)$u+ M_n$.

Since (ad $h$)$\mathfrak{n}\subset \mathfrak{n}$, it follows that

((ad $h$)$-n+ 1$)$(\mathfrak{n}\cap M_{n-1})\subset \mathfrak{n}\cap M_n$.

Since ad $x$ is nilpotent, $M_n= 0$ for sufficiently large $n$. Consequently, the eigenvalues of ad $h|\mathfrak{n}$ are integers $\geq 0$. Thus, the restriction of ad $h+ 2$ to $\mathfrak{n}$ is invertible.

Now $[h, z] + 2z\in \mathfrak{n}$ since

$$
[x,[h, z] + 2z] = [[x, h], z] + [h,[x, z]] + 2[x, z]
$$

$$
= [-2x, z] + [h,-h] + 2[x, z] = 0
$$

Hence there exists $z'\in \mathfrak{n}$ such that $[h, z'] + 2z'= [h, z] + 2z$, that is, $[h, y] =-2y$, putting $y=z-z'$. Since $[x, y] = [x, z] =-h$, this completes the proof.

#### Proposition 2 (Jacobson-Morozov) {#lie-viii-s11-prop-2 .statement tag=0179}

Assume that $\mathfrak{g}$ is semi-simple. Let $x$ be a non-zero nilpotent element of $\mathfrak{g}$. There exist $h, y\in \mathfrak{g}$ such that $(x, h, y)$ is an $\mathfrak{s}\mathfrak{l}_2$-triplet.

Let $\mathfrak{n}=$ Ker(ad $x$)$^2$. If $z\in \mathfrak{n}$, then [ad $x$,[ad $x$, ad $z]] =$ ad([$x,[x, z]]$) $= 0$. By Lemma 5, ad $x\circ$ ad $z$ is nilpotent, so Tr(ad $x\circ$ ad $z$) $= 0$. This shows that $x$ is orthogonal to $\mathfrak{n}$ with respect to the Killing form $\Phi$ of $\mathfrak{g}$. Since

$\Phi$((ad $x$)$^2y, y'$) $=\Phi (y$, (ad $x$)$^2y')$

for all $y, y'\in \mathfrak{g}$, and since $\Phi$ is non-degenerate, the orthogonal complement of $\mathfrak{n}$ is the image of (ad $x$)$^2$. Hence there exists $y'\in \mathfrak{g}$ such that $x=$ (ad $x$)$^2y'$. Put

$$
h=-2[x, y']
$$

we have $[h, x] = 2x$ and $h\in$ (ad $x$)$(\mathfrak{g})$. It now suffices to apply Lemma 6.

#### Corollary {#lie-viii-s11-n2-cor-1 .statement tag=017A}

Assume that $\mathfrak{g}$ is semi-simple. Let G be a group of automorphisms of $\mathfrak{g}$ containing Aut$_e(\mathfrak{g})$. The map which associates to any $\mathfrak{s}\mathfrak{l}_2$-triplet $(x, h, y)$ in $\mathfrak{g}$ the nilpotent element $x$ defines, by passage to the quotient, a bijection from the set of G-conjugacy classes of $\mathfrak{s}\mathfrak{l}_2$-triplets to the set of G-conjugacy classes of non-zero nilpotent elements.

This follows from Prop. 1 and 2.

#### Lemma 7 {#lie-viii-s11-lem-7 .statement tag=017B}

Let K be a commutative field with at least 4 elements. Let G be the group of matrices $(\alpha 0\alpha \beta_{-1})$ where $\alpha \in K^*,\beta \in K$. Let $G'$ be the group

of such matrices such that $\alpha = 1$. Then $G'= (G,G)$.

If $\alpha , \alpha '\in K^*$ and $\beta , \beta '\in K$,

$$
(\alpha \beta )((\alpha '\beta ')((\alpha \beta )^{-1}(\alpha '\beta ')^{-1}
$$

0 $\alpha^{-1}$ 0 $\alpha^{'-1}$ 0 $\alpha^{-1}$ 0 $\alpha^{'-1}$

$$
=(1-\alpha '\beta '-{\alpha \beta \alpha '}^2+\alpha^2\alpha '\beta '+\alpha \beta )
$$

0 1

In particular,

$(1\beta )((\alpha '$ 0 $)((1\beta )^{-1}(\alpha '$ 0 $)^{-1}=(1\beta (1-{\alpha '}^2))$.

0 1 0 $\alpha^{'-1}$ 0 1 0 $\alpha^{'-1}$ 0 1

But there exists $\alpha '_0\in K^*$ such that $\alpha '_0\not= 1$ and $\alpha '_0\not=-1$, and then $k.(1-{\alpha '_0}^2)$ $=k$, hence the lemma.

#### Proposition 3 {#lie-viii-s11-prop-3 .statement tag=017C}

Assume that $\mathfrak{g}$ is semi-simple. The group Aut$_e(\mathfrak{g})$ is equal to its derived group. If $\mathfrak{g}$ is splittable, Aut$_e(\mathfrak{g})$ is the derived group of Aut$_0(\mathfrak{g})$.

Let $x$ be a non-zero nilpotent element of $\mathfrak{g}$. Choose $h, y\in \mathfrak{g}$ be such that $(x, h, y)$ is an $\mathfrak{s}\mathfrak{l}_2$-triplet (Prop. 2). The subalgebra $\mathfrak{s}$ of $\mathfrak{g}$ generated by $(x, h, y)$ can be identified with $\mathfrak{s}\mathfrak{l}(2, k)$. Let $\rho$ be the representation $z \rightarrow$ ad$_{\mathfrak{g}}z$ of $\mathfrak{s}=\mathfrak{s}\mathfrak{l}(2, k)$ on $\mathfrak{g}$, and let $\pi$ be the representation of $\mathbf{S}\mathbf{L}(2, k)$ compatible with $\rho ($§1, no. 4). The image of $\pi$ is generated by the exp($t$ ad$_{\mathfrak{g}}x$) and the exp($t$ ad$_{\mathfrak{g}}y$) with $t\in k($Algebra, Chap. III, §8, no. 9, Prop. 17), hence is contained in Aut$_e(\mathfrak{g})$. Since $\mathbf{S}\mathbf{L}(2, k)$ is equal to its derived group (Lemma 7 and loc. cit.), exp(ad$_{\mathfrak{g}}x$) belongs to the derived group G of Aut$_e(\mathfrak{g})$. Hence Aut$_e(\mathfrak{g})$ is equal to G. Assume now that $\mathfrak{g}$ is splittable. Since Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})$ is commutative (§5, no. 3, Remark 3), the preceding proves that the derived group of Aut$_0(\mathfrak{g})$ is Aut$_e(\mathfrak{g})$.

### 3. SIMPLE ELEMENTS

#### Definition 2 {#lie-viii-s11-def-2 .statement tag=017D}

An element $h$ of $\mathfrak{g}$ is said to be simple if there exist $x, y\in \mathfrak{g}$ such that $(x, h, y)$ is an $\mathfrak{s}\mathfrak{l}_2$-triplet in $\mathfrak{g}$.

We also say that $h$ is the simple element of the $\mathfrak{s}\mathfrak{l}_2$-triplet $(x, h, y)$.

#### Proposition 4 {#lie-viii-s11-prop-4 .statement tag=017E}

Let $h$ be a non-zero element of $\mathfrak{g}$. Then $h$ is simple if and only if there exists $x\in \mathfrak{g}$ such that $[h, x] = 2x$ and $h\in$ (ad $x$)$(\mathfrak{g})$.

The condition is clearly necessary. It is sufficient by Lemma 6.

#### Proposition 5 {#lie-viii-s11-prop-5 .statement tag=017F}

Assume that $\mathfrak{g}$ is splittable semi-simple. Let $\mathfrak{h}$ be a splitting Cartan subalgebra of $\mathfrak{g}$, R the set of roots of $(\mathfrak{g},\mathfrak{h})$, and B a basis of R. Let $h$ be a simple element of $\mathfrak{g}$ belonging to $\mathfrak{h}$. Then $h$ is conjugate under Aut$_e(\mathfrak{g},\mathfrak{h})$ to an element $h'$ of $\mathfrak{h}$ such that $\alpha (h')\in  \{0,1,2\}$ for all $\alpha \in B$.

The eigenvalues of ad$_{\mathfrak{g}}h$ belong to $\mathbf{Z}($§1, no. 2, Cor. of Prop. 2). Hence $h\in \mathfrak{h}_{\mathbf{Q}}$. There exists an element $w$ of the Weyl group of $(\mathfrak{g},\mathfrak{h})$ such that $\alpha (wh)\geq 0$ for all $\alpha \in B$ (Chap. VI, §1, no. 5, Th. 2 (i)). In view of §2, no. 2, Cor. of Th. 2, we are reduced to the case in which $\alpha (h)\in \mathbf{N}$ for all $\alpha \in B$. Let $R_+$ be the set of positive roots relative to B, and $R_-=-R_+$. There exists an $\mathfrak{s}\mathfrak{l}_2$-triplet in $\mathfrak{g}$ of the form $(x, h, y)$. Let T be the set of roots $\beta$ such that $\beta (h) =-2$. Then $T\subset R_-$ and $y\in \sum_{\beta\in T}\mathfrak{g}^{\beta}$. Assume that there

exists $\alpha \in B$ such that $\alpha (h)>2$. For all $\beta \in T$, we have $(\alpha +\beta )(h)>0$, so $\alpha +\beta  /\in R_-$ and $\alpha +\beta \not= 0$; on the other hand, since $\beta \in R_-$ and $\alpha \in B$, we have $\alpha +\beta  /\in R_+$; hence $\alpha +\beta  /\in R\cup  \{0\}$, so $[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}] = 0$. Thus, $[y,\mathfrak{g}^{\alpha}] = 0$. But ad$_{\mathfrak{g}}y|\mathfrak{g}^{\alpha}$ is injective since $\alpha (h)>0 ($§1, no. 2, Cor. of Prop. 2). This contradiction proves that $\alpha (h)\leq 2$ for all $\alpha \in B$.

#### Corollary {#lie-viii-s11-n3-cor-1 .statement tag=017G}

If $k$ is algebraically closed and if $\mathfrak{g}$ is semi-simple of rank $l$, the number of conjugacy classes of simple elements of $\mathfrak{g}$, relative to Aut$_e(\mathfrak{g})$, is at most $3^l$.

Indeed, every semi-simple element of $\mathfrak{g}$ is conjugate under Aut$_e(\mathfrak{g})$ to an element of $\mathfrak{h}$.

#### Lemma 8 {#lie-viii-s11-lem-8 .statement tag=017H}

Assume that $k$ is algebraically closed and that $\mathfrak{g}$ is semi-simple. Let $h$ be a semi-simple element of $\mathfrak{g}$ such that the eigenvalues of ad $h$ are rational. Let $\mathfrak{g}^0=$ Ker(ad $h$)$,\mathfrak{g}^2=$ Ker(ad $h-2$). Let $G_h$ be the set of elementary automorphisms of $\mathfrak{g}$ leaving $h$ fixed. Let $x\in \mathfrak{g}^2$ be such that $[x,\mathfrak{g}^0] =\mathfrak{g}^2$. Then $G_hx$ contains a subset of $\mathfrak{g}^2$ that is dense and open in the Zariski topology.

Let $\mathfrak{h}$ be a Cartan subalgebra of $\mathfrak{g}^0$. This is a Cartan subalgebra of $\mathfrak{g}$ containing $h$ (Chap. VII, §2, no. 3, Prop. 10). We have $h\in \mathfrak{h}_{\mathbf{Q}}$. Let R be the root system of $(\mathfrak{g},\mathfrak{h}), Q$ the group of radical weights. There exists a basis B of R such that $\alpha (h)\geq 0$ for all $\alpha \in B$.

Let U be the set of $z\in \mathfrak{h}$ such that $\alpha (z)\not= 0$ for all $\alpha \in B$. Let $(H'_{\alpha})_{\alpha\in B}$ be the basis of $\mathfrak{h}$ dual to B. If $z\in U$, there exists a homomorphism from Q to $k^*$ that takes any $\gamma \in Q$ to $\prod_{\alpha\in B}\alpha (z)^{\gamma(H'_{\alpha})}$. By §5, Prop. 2 and 4, the

endomorphism $\varphi (z)$ of the vector space $\mathfrak{g}$ which induces on $\mathfrak{g}^{\gamma}$ the homothety with ratio $\prod_{\alpha\in B}\alpha (z)^{\gamma(H'_{\alpha})}$ is an elementary automorphism of $\mathfrak{g}$, which clearly

belongs to $G_h$.

Let $s\in \mathfrak{h}$. If $\gamma \in R$ is such that $\mathfrak{g}^{\gamma}\cap \mathfrak{g}^2\not= 0$,

$$
2 =\gamma (h) =\gamma (\sum_{\alpha\in B}\alpha (h)H'_{\alpha})=\sum_{\alpha\in B}\alpha (h)\gamma (H'_{\alpha})
$$

since $\alpha (h)\geq 0$ for all $\alpha \in B$, and since the $\gamma (H'_{\alpha})$ are integers either all $\geq 0$ or all $\leq 0$, we have $\gamma (H'_{\alpha})\in \mathbf{N}$ for all $\alpha \in B$. Thus, we can consider (for $z\in \mathfrak{h}$) the endomorphism $\psi (z)$ of the vector space $\mathfrak{g}^2$ that induces on $\mathfrak{g}^{\gamma}\cap \mathfrak{g}^2$ the homothety with ratio $\prod_{\alpha\in B}\alpha (z)^{\gamma(H'_{\alpha})}$. The map $z \rightarrow \psi (z)$ from $\mathfrak{h}$ to End($\mathfrak{g}^2$) is polynomial. For $z\in U$, we have $\psi (z) =\varphi (z)|\mathfrak{g}^2$.

Let $\gamma_1, . . . , \gamma_r$ be the distinct roots of $(\mathfrak{g},\mathfrak{h})$ vanishing on $h$. If $y_1\in \mathfrak{g}^{\gamma_1}, . . .$, $y_r\in \mathfrak{g}^{\gamma_r}$, we have $e^{ady_1}. . . e^{ady_r}\in G_h$. We can thus define a map $\rho$ from $\mathfrak{h}\times \mathfrak{g}^{\gamma_1}\times  \cdots  \times \mathfrak{g}^{\gamma_r}$ to $\mathfrak{g}^2$ by putting

$$
\rho (z, y_1, . . . , y_r) =\psi (z)e^{ady_1}. . . e^{ady_r}x
$$

for $z\in \mathfrak{h}, y_1\in \mathfrak{g}^{\gamma_1}, . . . , y_r\in \mathfrak{g}^{\gamma_r}$. This map is polynomial, and $\rho (U,\mathfrak{g}^{\gamma_1}, . . . ,\mathfrak{g}^{\gamma_r})$ $\subset G_hx$. By Chap. VII, App. I, Prop. 3 and 4, it suffices to prove that the tangent linear map of $\rho$ is surjective at some point.

Now let T be the tangent linear map of $z \rightarrow \psi (z)$ at $h_0=\sum_{\alpha\in B}H'_{\alpha}$. Then $T(z)$ is the endomorphism of $\mathfrak{g}^2$ that induces on $\mathfrak{g}^{\gamma}\cap \mathfrak{g}^2$ the homothety with ratio

$$
\sum_{\alpha\in B}\gamma (H'_{\alpha})\alpha (h_0)^{\gamma(H'_{\alpha})-1}\alpha (z)\prod_{\beta\in B,\beta\not=\alpha}\beta (h_0)^{\gamma(H'_{\alpha})}=\sum_{\alpha\in B}\gamma (H'_{\alpha})\alpha (z) =\gamma (z)
$$

Thus, the tangent linear map of $z \rightarrow \rho (z,0, . . . ,0)$ at $h_0$ is the map $z \rightarrow [z, x]$; its image is $[x,\mathfrak{h}]$. The tangent linear map at 0 of the map $y_1 \rightarrow \rho (h_0, y_1,0, . . . ,0)$ is the map $y_1 \rightarrow \psi (h_0)[y_1, x]$; this last map has image $\psi (h_0)[x,\mathfrak{g}^{\gamma_1}] = [x,\mathfrak{g}^{\gamma_1}]$. Similarly, the tangent linear map at 0 of the map $y_i \rightarrow \rho (h_0,0, . . . ,0, y_i,0, . . . ,0)$ has image $[x,\mathfrak{g}^{\gamma_i}]$. Finally, the tangent linear map of $\rho$ at $(h_0,0, . . . ,0)$ has image

$$
[x,\mathfrak{h}+\mathfrak{g}^{\gamma_1}+\cdots +\mathfrak{g}^{\gamma_r}] = [x,\mathfrak{g}^0] =\mathfrak{g}^2.Q.E.D
$$

$^*$The group $G_h$ is an algebraic group with Lie algebra ad $\mathfrak{g}^0._*$

#### Proposition 6 {#lie-viii-s11-prop-6 .statement tag=017I}

Assume that $k$ is algebraically closed and that $\mathfrak{g}$ is semi-simple. Let G be a group of automorphisms of $\mathfrak{g}$ containing Aut$_e(\mathfrak{g})$. Let $(x, h, y)$ and $(x', h', y')$ be $\mathfrak{s}\mathfrak{l}_2$-triplets in $\mathfrak{g}$. The following conditions are equivalent:

(i) $h$ and $h'$ are G-conjugate;

(ii) $(x, h, y)$ and $(x', h', y')$ are G-conjugate.

We only have to prove the implication (i) $=\Rightarrow$ (ii), and we are reduced immediately to the case in which $h=h'$. Introduce $\mathfrak{g}^2$ and $G_h$ as in Lemma 8. We have $x\in \mathfrak{g}^2$, and $[x,\mathfrak{g}^0] =\mathfrak{g}^2$ by §1, no. 2, Cor. of Prop. 2. Hence $G_hx$ contains a subset of $\mathfrak{g}^2$ that is dense and open in the Zariski topology, and so does $G_hx'$. So there exists $a\in G_h$ such that $a(x) =x'$. We have $a(h) =h$, and consequently $a(y) =y'$ (no. 1, Lemma 1).

#### Corollary 1 {#lie-viii-s11-prop-6-cor-1 .statement tag=017J}

The map which associates to any $\mathfrak{s}\mathfrak{l}_2$-triplet its simple element defines by passage to the quotients a bijection from the set of G-conjugacy classes of $\mathfrak{s}\mathfrak{l}_2$-triplets to the set of G-conjugacy classes of simple elements.

#### Corollary 2 {#lie-viii-s11-prop-6-cor-2 .statement tag=017K}

If rk($\mathfrak{g}$) $=l$, the number of conjugacy classes, relative to Aut$_e(\mathfrak{g})$, of non-zero nilpotent elements of $\mathfrak{g}$ is at most $3^l$.

This follows from Cor. 1, the Cor. of Prop. 2, and the Cor. of Prop. 5.

#### Corollary 3 {#lie-viii-s11-prop-6-cor-3 .statement tag=017L}

If rk($\mathfrak{g}$) $=l$, the number of conjugacy classes, relative to Aut$_e(\mathfrak{g})$, of subalgebras of $\mathfrak{g}$ isomorphic to $\mathfrak{s}\mathfrak{l}(2, k)$ is at most $3^l$.

This follows from Cor. 1, Prop. 1, and the Cor. of Prop. 5.

### 4. PRINCIPAL ELEMENTS

#### Definition 3 {#lie-viii-s11-def-3 .statement tag=017M}

Assume that $\mathfrak{g}$ is semi-simple.

(i) A nilpotent element $x$ of $\mathfrak{g}$ is said to be principal if the dimension of Ker ad $x$ is the rank of $\mathfrak{g}$.

(ii) A simple element $h$ of $\mathfrak{g}$ is said to be principal if $h$ is regular and the eigenvalues of ad $h$ in an algebraic closure of $k$ belong to $2\mathbf{Z}$.

(iii) An $\mathfrak{s}\mathfrak{l}_2$-triplet $(x, h, y)$ of $\mathfrak{g}$ is said to be principal if the length of $\mathfrak{g}$, considered as a module over $kx+kh+ky$, is equal to the rank of $\mathfrak{g}$.

#### Proposition 7 {#lie-viii-s11-prop-7 .statement tag=017N}

Assume that $\mathfrak{g}$ is semi-simple. Let $(x, h, y)$ be an $\mathfrak{s}\mathfrak{l}_2$-triplet in $\mathfrak{g}$. The following conditions are equivalent:

(i) $x$ is principal;

(ii) $h$ is principal;

(iii) $(x, h, y)$ is principal.

For $p\in \mathbf{Z}$, let $\mathfrak{g}^p=$ Ker(ad $h-p$). Let $\mathfrak{g}'=\sum_{p\in\mathbf{Z}}\mathfrak{g}^{2p}$. If $\mathfrak{g}$ is considered as

a module over $\mathfrak{a}=kx+kh+ky,\mathfrak{g}'$ is the sum of the simple submodules of odd dimension (§1, no. 2, Cor. of Prop. 2). Let $l$ (resp. $l'$) be the length of $\mathfrak{g}$ (resp. $\mathfrak{g}'$) considered as an $\mathfrak{a}$-module. By §1, no. 2,

dim(Ker ad $x$) $=l\geq l'=$ dim(Ker ad $h$)$\geq$ rk($\mathfrak{g}$).

The equivalence of (i) and (iii) follows immediately. On the other hand, condition (ii) means that dim(Ker ad $h$) $=$ rk($\mathfrak{g}$) and $\mathfrak{g}'=\mathfrak{g}$, in other words that

dim(Ker ad $h$) $=$ rk($\mathfrak{g}$) and $l=l'$. The equivalence of (ii) and the other conditions follows.

#### Proposition 8 {#lie-viii-s11-prop-8 .statement tag=017O}

Assume that $\mathfrak{g}$ is semi-simple $\not= 0$. Let $\mathfrak{h}$ be a splitting Cartan subalgebra of $\mathfrak{g}$, R the root system of $(\mathfrak{g},\mathfrak{h})$, B a basis of R$,h^0$ the element of $\mathfrak{h}$ such that $\alpha (h^0) = 2$ for all $\alpha \in B$.

(i) The element $h^0$ is simple and principal.

(ii) The elements $x$ of $\mathfrak{g}$ such that there exists an $\mathfrak{s}\mathfrak{l}_2$-triplet of the form $(x, h^0, y)$ are the elements of $\sum_{\alpha\in B}\mathfrak{g}^{\alpha}$ that have a non-zero component in each $\mathfrak{g}^{\alpha}$.

The element $h^0$ is that considered in §7, no. 5, Lemma 2 (cf. loc. cit., formula (1)). It follows from this lemma that $h^0$ is simple principal and that, if $x\in \sum_{\alpha\in B}\mathfrak{g}^{\alpha}$ has a non-zero component in each $\mathfrak{g}^{\alpha}$, there exists an $\mathfrak{s}\mathfrak{l}_2$-triplet of the form $(x, h^0, y)$. Conversely, let $(x, h^0, y)$ be a $\mathfrak{s}\mathfrak{l}_2$-triplet. We have $[h^0, x] = 2x$, so $x\in \sum_{\gamma\in R,\gamma(h^0)=2}\mathfrak{g}^{\gamma}=\sum_{\alpha\in B}\mathfrak{g}^{\alpha}$. Similarly, $y\in \sum_{\alpha\in B}\mathfrak{g}^{-\alpha}$. Write

$h^0=\sum_{\alpha\in B}a_{\alpha}H_{\alpha}$ where $a_{\alpha}>0$ for all $\alpha \in B$,

$x=\sum_{\alpha\in B}X_{\alpha}$ where $X_{\alpha}\in \mathfrak{g}^{\alpha}$ for all $\alpha \in B$,

$y=\sum_{\alpha\in B}X_{-\alpha}$ where $X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ for all $\alpha \in B$.

Then

$$
\sum_{\alpha\in B}a_{\alpha}H_{\alpha}=h^0= [y, x] =\sum_{\alpha ,\beta\in B}[X_{-\beta}, X_{\alpha}] =\sum_{\alpha\in B}[X_{-\alpha}, X_{\alpha}]
$$

so $[X_{-\alpha}, X_{\alpha}]\not= 0$ for all $\alpha \in B$.

#### Corollary {#lie-viii-s11-n4-cor-1 .statement tag=017P}

In a splittable semi-simple Lie algebra, there exist principal nilpotent elements.

In a non-splittable semi-simple Lie algebra, 0 may be the only nilpotent element.

#### Proposition 9 {#lie-viii-s11-prop-9 .statement tag=017Q}

Assume that $k$ is algebraically closed and that $\mathfrak{g}$ is semi-simple. All the principal simple (resp. nilpotent) elements of $\mathfrak{g}$ are conjugate under Aut$_e(\mathfrak{g})$.

We retain the notations of Prop. 8. Let $h$ be a principal simple element. It is conjugate under Aut$_e(\mathfrak{g})$ to an $h'\in \mathfrak{h}$ such that $\alpha (h')\in  \{0,1,2\}$ for all $\alpha \in B$ (no. 3, Prop. 5). Since $h'$ is principal simple, $\alpha (h')\not= 0$ and $\alpha (h')\in 2\mathbf{Z}$ for all $\alpha \in B$, so $\alpha (h') = 2$ for all $\alpha \in B$, and hence $h'=h^0$. This proves the assertion for principal simple elements.

Let $x, x'$ be principal nilpotent elements. There exist $\mathfrak{s}\mathfrak{l}_2$-triplets $(x, h, y)$, $(x', h', y')$. By Prop. $7,h$ and $h'$ are principal simple, hence conjugate under Aut$_e(\mathfrak{g})$ by the preceding. So $x$ and $x'$ are conjugate under Aut$_e(\mathfrak{g})$ (Prop. 6).

#### Lemma 9 {#lie-viii-s11-lem-9 .statement tag=017R}

With the notations of Prop. 8, put $\mathfrak{g}^p=$ Ker(ad $h^0-p$) for $p\in \mathbf{Z}$. Let $\mathfrak{g}^2_*$ be the set of elements of $\mathfrak{g}^2=\sum_{\alpha\in B}\mathfrak{g}^{\alpha}$ that have a non-zero component

in each $\mathfrak{g}^{\alpha}$. Let $R_+$ be the set of positive roots relative to B$,\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha}$, and $x\in \mathfrak{g}^2_*$. Then $e^{ad\mathfrak{n}_+}.x=x+ [\mathfrak{n}_+,\mathfrak{n}_+]$.

It is clear that $e^{ad\mathfrak{n}_+}.x\subset x+ [\mathfrak{n}_+,\mathfrak{n}_+]$. We prove that, if $v\in [\mathfrak{n}_+,\mathfrak{n}_+]$, then $x+v\in e^{ad\mathfrak{n}_+}.x$. Put $\mathfrak{n}^{(p)}=\sum_{r\geq p}\mathfrak{g}^{2r}$; it suffices to prove that

$$
x+v\in e^{ad\mathfrak{n}_+}.x+\mathfrak{n}^{(p)}
$$

for all $p\geq 2$. This is clear for $p= 2$ since $\mathfrak{n}$[^2] $= [\mathfrak{n}_+,\mathfrak{n}_+] ($§3, no. 3, Prop. 9 (iii)). Assume that we have found $z\in \mathfrak{n}_+$ such that $v+x-e^{adz}.x\in$ $\mathfrak{n}^{(p)}$. Since there exists an $\mathfrak{s}\mathfrak{l}_2$-triplet of the form $(x, h^0, y)$ (Prop. 8), §1, no. 2, Cor. of Prop. 2 proves that $[x,\mathfrak{g}^{2p-2}] =\mathfrak{g}^{2p}$; hence, there exists $z'\in \mathfrak{g}^{2p-2}\subset \mathfrak{n}_+$ such that

$$
v+x-e^{adz}.x\in [z', x] +\mathfrak{n}^{(p+1)}
$$

So $v+x\in e^{ad(z+z')}.x+\mathfrak{n}^{(p+1)}$, and our assertion is established by induction.

#### Proposition 10 {#lie-viii-s11-prop-10 .statement tag=017S}

Assume that $\mathfrak{g}$ is semi-simple. Let $\mathfrak{h}$ be a splitting Cartan subalgebra of $\mathfrak{g}$, R the root system of $(\mathfrak{g},\mathfrak{h})$, B a basis of R, $R_+$ the set of positive roots relative to B, and $\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha}$. The principal nilpotent elements belonging to $\mathfrak{n}_+$ are the elements of $\mathfrak{n}_+$ having a non-zero component in $\mathfrak{g}^{\alpha}$ for all $\alpha \in B$.

Prop. 8 and Lemma 9 prove that such elements are principal nilpotent. We prove the converse. Evidently we can assume that $\mathfrak{g}$ is simple. Let $h^0$ and $\mathfrak{g}^p$ be as in Prop. 8 and Lemma 9. Let $\omega$ be the highest root, and put $\omega (h^0) = 2q$; we have $q=h-1$, where $h$ is the Coxeter number of R, cf. Chap. VI, §1, no. 11, Prop. 31. Then $\mathfrak{g}^{2q}=\mathfrak{g}^{\omega},\mathfrak{g}^{-2q}=\mathfrak{g}^{-\omega}$, and $\mathfrak{g}^{2k}= 0$ for $|k|> q$. There exists a principal $\mathfrak{s}\mathfrak{l}_2$-triplet $(x^0, h^0, y^0)$. By §1, no. 2, Cor. of Prop. 2, (ad $x^0$)$^{2q}(\mathfrak{g}^{-\omega}) =\mathfrak{g}^{\omega}$, so (ad $x^0$)$^{2q}\not= 0$. Let $x$ be a principal nilpotent element of $\mathfrak{g}$ belonging to $\mathfrak{n}_+$. If $\overline{k}$ is an algebraic closure of $k,x\otimes 1$ and $x^0\otimes 1$ are conjugate under an automorphism of $\mathfrak{g}\otimes_k\overline{k}$ (Prop. 9), so (ad $x$)$^{2q}\not= 0$. There exists $\lambda \in R$ such that (ad $x$)$^{2q}\mathfrak{g}^{\lambda}\not= 0$. Put $x=\sum_{n\geq 1}x_n$, where $x_n\in \mathfrak{g}^{2n}$.

Then

(ad $x$)$^{2q}\mathfrak{g}^{\lambda}\subset$ (ad $x_1$)$^{2q}\mathfrak{g}^{\lambda}+\sum_{k>4q+\lambda(h^0)}\mathfrak{g}^k=$ (ad $x_1$)$^{2q}\mathfrak{g}^{\lambda}$, since $4q+\lambda (h^0)\geq 4q-2q= 2q$. Now (ad $x_1$)$^{2q}\mathfrak{g}^{\lambda}\subset \mathfrak{g}^{4q+\lambda(h^0)}$, where $\lambda =-\omega$. Thus, (ad $x_1$)$^{2q}\mathfrak{g}^{-\omega}=\mathfrak{g}^{\omega}$. We have $\omega =\sum_{\alpha\in B}n_{\alpha}\alpha$ with $n_{\alpha}>0$ for all $\alpha \in$ B (Chap. VI, §1, no. 8, Remark). If there exists $\alpha_0\in B$ such that $x_1\in$

$\sum\mathfrak{g}^{\alpha}$, the relation

$\alpha \in B,\alpha \not=\alpha_0$

$$
\omega  /\in  -\omega +\sum_{\alpha\in B,\alpha\not=\alpha_0}k\alpha
$$

implies that $\mathfrak{g}^{\omega}\subset /$ (ad $x_1$)$^p\mathfrak{g}^{-\omega}$ for all $p$; this is absurd, so the component of $x_1$ in $\mathfrak{g}^{\alpha}$ is non-zero for all $\alpha \in B$.

### Exercises {#lie-viii-s11-exercises}

See the [exercises for § 11](exercises/s11/).
