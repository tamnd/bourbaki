---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 2
section_title: Cartan subalgebras and regular elements of a Lie algebra
lang: en
source: lie-vii-ix
book_pages: 12-20, 55-57
pdf_pages: 0022-0030, 0064-0066
extraction: native
subsections:
    - "no": 1
      title: CARTAN SUBALGEBRAS
      page: 13
      pdf_page: 23
    - "no": 2
      title: REGULAR ELEMENTS OF A LIE ALGEBRA
      page: 16
      pdf_page: 26
    - "no": 3
      title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
      page: 18
      pdf_page: 28
    - "no": 4
      title: CARTAN SUBALGEBRAS OF SEMI-SIMPLE LIE ALGEBRAS
      page: 19
      pdf_page: 29
statements: 40
exercises: 16
content_sha256: 05b31ef931fa1971af6f075dc663eed9dae014f8584d9c3690519a9cceb1ce2d
---

## § 2. CARTAN SUBALGEBRAS AND REGULAR ELEMENTS OF A LIE ALGEBRA

From no. 2 onwards, the field $k$ is assumed to be infinite.

### 1. CARTAN SUBALGEBRAS

#### Definition 1 {#lie-vii-s2-def-1 .statement tag=00TJ}

Let $\mathfrak{g}$ be a Lie algebra. A Cartan subalgebra of $\mathfrak{g}$ is a nilpotent subalgebra of $\mathfrak{g}$ equal to its own normalizer.

Later we shall obtain the following results:

1) if $k$ is infinite, $\mathfrak{g}$ has Cartan subalgebras (no. 3, Cor. 1 of Th. 1);

2) if $k$ is of characteristic zero, all Cartan subalgebras of $\mathfrak{g}$ have the same dimension (§3, no. 3, Th. 2);

3) if $k$ is algebraically closed and of characteristic 0, all Cartan subalgebras of $\mathfrak{g}$ are conjugate under the group of elementary automorphisms of $\mathfrak{g}($§3, no. 2, Th. 1).

#### Example 1 {#lie-vii-s2-n1-exa-1 .statement tag=00TK}

If $\mathfrak{g}$ is nilpotent, the only Cartan subalgebra of $\mathfrak{g}$ is $\mathfrak{g}$ itself (Chap. I, §4, no. 1, Prop. 3).

#### Example 2 {#lie-vii-s2-n1-exa-2 .statement tag=00TL}

Let $\mathfrak{g}=\mathfrak{g}\mathfrak{l}(n, k)$, and let $\mathfrak{h}$ be the set of diagonal matrices belonging to $\mathfrak{g}$. We show that $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$. First, $\mathfrak{h}$ is commutative, hence nilpotent. Let $(E_{ij})$ be the canonical basis of $\mathfrak{g}\mathfrak{l}(n, k)$, and let $x=\sum\mu_{ij}E_{ij}$ be an element of the normalizer of $\mathfrak{h}$ in $\mathfrak{g}$. If $i\not=j$, formulas (5) of Chap. I, §1, no. 2 show that the coefficient of $E_{ij}$ in $[E_{ii}, x]$ is $\mu_{ij}$. Since $E_{ii}\in \mathfrak{h}$, $[E_{ii}, x]\in \mathfrak{h}$, and the coefficient in question is zero. Thus $\mu_{ij}= 0$ for $i\not=j$, so $x\in \mathfrak{h}$, which shows that $\mathfrak{h}$ is indeed a Cartan subalgebra of $\mathfrak{g}$.

#### Example 3 {#lie-vii-s2-n1-exa-3 .statement tag=00TM}

Let $\mathfrak{h}$ be a Cartan subalgebra of $\mathfrak{g}$ and let $\mathfrak{g}_1$ be a subalgebra of $\mathfrak{g}$ containing $\mathfrak{h}$. Then $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}_1$; this follows immediately from Def. 1.

#### Proposition 1 {#lie-vii-s2-prop-1 .statement tag=00TN}

Let $\mathfrak{g}$ be a Lie algebra and let $\mathfrak{h}$ be a Cartan subalgebra of $\mathfrak{g}$. Then $\mathfrak{h}$ is a maximal nilpotent subalgebra of $\mathfrak{g}$.

Let $\mathfrak{h}'$ be a nilpotent subalgebra of $\mathfrak{g}$ containing $\mathfrak{h}$. Then $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{h}'$ (Example 3), so $\mathfrak{h}=\mathfrak{h}'$ (Example 1).

There exist maximal nilpotent subalgebras that are not Cartan subalgebras (Exerc. 2).

#### Proposition 2 {#lie-vii-s2-prop-2 .statement tag=00TO}

Let $(\mathfrak{g}_i)_{i\in I}$ be a finite family of Lie algebras and $\mathfrak{g}=\prod_{i\in I}\mathfrak{g}_i$.

The Cartan subalgebras of $\mathfrak{g}$ are the subalgebras of the form $\prod_{i\in I}\mathfrak{h}_i$, where $\mathfrak{h}_i$

is a Cartan subalgebra of $\mathfrak{g}_i$.

If $\mathfrak{h}_i$ is a subalgebra of $\mathfrak{g}_i$ with normalizer $\mathfrak{n}_i$, then $\prod\mathfrak{h}_i$ is a subalgebra of $\mathfrak{g}$ with normalizer $\prod\mathfrak{n}_i$; if the $\mathfrak{h}_i$ are nilpotent, $\prod\mathfrak{h}_i$ is nilpotent; thus, if $\mathfrak{h}_i$ is a Cartan subalgebra of $\mathfrak{g}_i$ for all $i,\prod\mathfrak{h}_i$ is a Cartan subalgebra of $\mathfrak{g}$. Conversely, let $\mathfrak{h}$ be a Cartan subalgebra of $\mathfrak{g}$; the projection $\mathfrak{h}_i$ of $\mathfrak{h}$ onto $\mathfrak{g}_i$ is a nilpotent subalgebra of $\mathfrak{g}_i$, and $\prod\mathfrak{h}_i$ is a nilpotent subalgebra of $\mathfrak{g}$ containing $\mathfrak{h}$; hence $\mathfrak{h}=\prod\mathfrak{h}_i$ (Prop. 1); thus, for all $i,\mathfrak{h}_i$ is its own normalizer in $\mathfrak{g}_i$, and so is a Cartan subalgebra of $\mathfrak{g}_i$.

#### Example 4 {#lie-vii-s2-n1-exa-4 .statement tag=00TP}

If $k$ is of characteristic $0,\mathfrak{g}\mathfrak{l}(n, k)$ is the product of the ideals $\mathfrak{s}\mathfrak{l}(n, k)$ and $k.1$. It follows from Example 2 and Prop. 2 that the set of diagonal matrices of trace 0 in $\mathfrak{s}\mathfrak{l}(n, k)$ is a Cartan subalgebra of $\mathfrak{s}\mathfrak{l}(n, k)$.

#### Proposition 3 {#lie-vii-s2-prop-3 .statement tag=00TQ}

Let $\mathfrak{g}$ be a Lie algebra, $\mathfrak{h}$ a subalgebra of $\mathfrak{g}$, and $k'$ an extension of $k$. Then $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$ if and only if $\mathfrak{h}\otimes_kk'$ is a Cartan subalgebra of $\mathfrak{g}\otimes_kk'$.

Indeed, $\mathfrak{h}$ is nilpotent if and only if $\mathfrak{h}\otimes_kk'$ is (Chap. I, §4, no. 5). On the other hand, if $\mathfrak{n}$ is the normalizer of $\mathfrak{h}$ in $\mathfrak{g}$, the normalizer of $\mathfrak{h}\otimes_kk'$ in $\mathfrak{g}\otimes_kk'$ is $\mathfrak{n}\otimes_kk'$ (Chap. I, §3, no. 8).

#### Proposition 4 {#lie-vii-s2-prop-4 .statement tag=00TR}

Let $\mathfrak{g}$ be a Lie algebra, $\mathfrak{h}$ a nilpotent subalgebra of $\mathfrak{g}$. Then $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$ if and only if $\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h}$.

If $\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h},\mathfrak{h}$ is its own normalizer (§1, Prop. 10 (i)), so $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$. Assume that $\mathfrak{g}^0(\mathfrak{h})\not=\mathfrak{h}$. Consider the representation of $\mathfrak{h}$ on $\mathfrak{g}^0(\mathfrak{h})/\mathfrak{h}$ obtained from the adjoint representation by passage to the quotient. By applying Engel’s theorem (Chap. I, §4, no. 2, Th. 1), we see that there exists $x\in \mathfrak{g}^0(\mathfrak{h})$ such that $x \notin \mathfrak{h}$ and $[\mathfrak{h}, x]\subset \mathfrak{h}$; then $x$ belongs to the normalizer of $\mathfrak{h}$ in $\mathfrak{g}$, so $\mathfrak{h}$ is not a Cartan subalgebra of $\mathfrak{g}$.

#### Corollary 1 {#lie-vii-s2-prop-4-cor-1 .statement tag=00TS}

Let $\mathfrak{g}$ be a Lie algebra, $\mathfrak{h}$ a Cartan subalgebra of $\mathfrak{g}$. If $k$ is infinite, there exists $x\in \mathfrak{h}$ such that $\mathfrak{h}=\mathfrak{g}^0(x)$.

Indeed, $\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$ and we can apply Prop. 9 (ii) of §1.

#### Corollary 2 {#lie-vii-s2-prop-4-cor-2 .statement tag=00TT}

Let $f:\mathfrak{g}\rightarrow \mathfrak{g}'$ be a surjective homomorphism of Lie algebras. If $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g},f(\mathfrak{h})$ is a Cartan subalgebra of $\mathfrak{g}'$.

Indeed, $f(\mathfrak{h})$ is a nilpotent subalgebra of $\mathfrak{g}'$. On the other hand, consider the representation $x \rightarrow$ ad $f(x)$ of $\mathfrak{h}$ on $\mathfrak{g}'$. By Prop. 9 (iv) of §1, no. 3, $f(\mathfrak{g}^0(\mathfrak{h})) ={\mathfrak{g}'}^0(\mathfrak{h})$. Now $\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h}$, and on the other hand it is clear that ${\mathfrak{g}'}^0(\mathfrak{h}) ={\mathfrak{g}'}^0(f(\mathfrak{h}))$. Hence, $f(\mathfrak{h}) ={\mathfrak{g}'}^0(f(\mathfrak{h}))$ and it suffices to apply Prop. 4.

#### Corollary 3 {#lie-vii-s2-prop-4-cor-3 .statement tag=00TU}

Let $\mathfrak{h}$ be a Cartan subalgebra of a Lie algebra $\mathfrak{g}$, and let $\mathscr{C}^n\mathfrak{g}(n\geq 1)$ be a term of the descending central series of $\mathfrak{g}$ (Chap. I, §1, no. 5). Then $\mathfrak{g}=\mathfrak{h}+\mathscr{C}^n\mathfrak{g}$.

Indeed, Corollary 2 shows that the image of $\mathfrak{h}$ in $\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$ is a Cartan subalgebra of $\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$, hence is equal to $\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$ since $\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$ is nilpotent (Example 1).

#### Corollary 4 {#lie-vii-s2-prop-4-cor-4 .statement tag=00TV}

Let $\mathfrak{g}$ be a Lie algebra, $\mathfrak{h}$ a Cartan subalgebra of $\mathfrak{g}$, and $\mathfrak{a}$ a subalgebra of $\mathfrak{g}$ containing $\mathfrak{h}$.

(i) $\mathfrak{a}$ is equal to its own normalizer in $\mathfrak{g}$.

(ii) Assume that $k=\mathbf{R}$ or $\mathbf{C}$; let G be a Lie group with Lie algebra $\mathfrak{g}$, A the integral subgroup of G with Lie algebra $\mathfrak{a}$. Then A is a Lie subgroup of G, and it is the identity component of the normalizer of A in G.

Let $\mathfrak{n}$ be the normalizer of $\mathfrak{a}$ in $\mathfrak{g}$. Since $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{n}$ (Example $3$)$,\{0\}$ is a Cartan subalgebra of $\mathfrak{n}/\mathfrak{a}$ (Cor. 2), hence is equal to its normalizer in $\mathfrak{n}/\mathfrak{a}$; in other words, $\mathfrak{n}=\mathfrak{a}$. Assertion (ii) follows from (i) and Chap. III, §9, no. 4, Cor. of Prop. 11.

#### Corollary 5 {#lie-vii-s2-prop-4-cor-5 .statement tag=00TW}

Let $\mathfrak{g}$ be a Lie algebra, E a subset of $\mathfrak{g}$. Let E operate on $\mathfrak{g}$ by the adjoint representation. Then E is a Cartan subalgebra of $\mathfrak{g}$ if and only if $E =\mathfrak{g}^0(E)$.

The condition is necessary (Prop. 4). Assume now that $E =\mathfrak{g}^0(E)$. By Prop. 2 (ii) of §1, no. 1, E is then a subalgebra of $\mathfrak{g}$. If $x\in E$, ad$_Ex$ is nilpotent since $E\subset \mathfrak{g}^0(E)$; hence the algebra E is nilpotent. But then E is a Cartan subalgebra by Prop. 4.

#### Corollary 6 {#lie-vii-s2-prop-4-cor-6 .statement tag=00TX}

Let $\mathfrak{g}$ be a Lie algebra, let $k_0$ be a subfield of $k$ such that $[k:k_0]<+\infty$, and let $\mathfrak{g}_0$ be the Lie algebra obtained from $\mathfrak{g}$ by restricting the field of scalars to $k_0$. Let $\mathfrak{h}$ be a subset of $\mathfrak{g}$. Then $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$ if and only if $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}_0$.

This follows from Cor. 5, since the condition $\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$ does not involve the base field.

#### Proposition 5 {#lie-vii-s2-prop-5 .statement tag=00TY}

Let $\mathfrak{g}$ be a Lie algebra, $\mathfrak{c}$ its centre, $\mathfrak{h}$ a vector subspace of $\mathfrak{g}$. Then $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$ if and only if $\mathfrak{h}$ contains $\mathfrak{c}$ and $\mathfrak{h}/\mathfrak{c}$ is a Cartan subalgebra of $\mathfrak{g}/\mathfrak{c}$.

Assume that $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$. Since $[\mathfrak{c},\mathfrak{g}]\subset \mathfrak{h}$, we have $\mathfrak{c}\subset \mathfrak{h}$. On the other hand, $\mathfrak{h}/\mathfrak{c}$ is a Cartan subalgebra of $\mathfrak{g}/\mathfrak{c}$ by Cor. 2 of Prop. 4.

Assume that $\mathfrak{h}\supset \mathfrak{c}$ and that $\mathfrak{h}/\mathfrak{c}$ is a Cartan subalgebra of $\mathfrak{g}/\mathfrak{c}$. Let $f$ be the canonical morphism from $\mathfrak{g}$ to $\mathfrak{g}/\mathfrak{c}$. The algebra $\mathfrak{h}$, which is a central extension of $\mathfrak{h}/\mathfrak{c}$, is nilpotent. Let $\mathfrak{n}$ be the normalizer of $\mathfrak{h}$ in $\mathfrak{g}$. If $x\in \mathfrak{n}$, $[f(x),\mathfrak{h}/\mathfrak{c}]\subset \mathfrak{h}/\mathfrak{c}$, hence $f(x)\in \mathfrak{h}/\mathfrak{c}$, and so $x\in \mathfrak{h}$. This proves that $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$.

#### Corollary {#lie-vii-s2-n1-cor-1 .statement tag=00TZ}

Let $\mathscr{C}_{\infty}\mathfrak{g}$ be the union of the ascending central series of the Lie algebra $\mathfrak{g}$ (Chap. I, §1, no. 6). The Cartan subalgebras of $\mathfrak{g}$ are the inverse images of the Cartan subalgebras of $\mathfrak{g}/\mathscr{C}_{\infty}\mathfrak{g}$.

Indeed, the centre of $\mathfrak{g}/\mathscr{C}_i\mathfrak{g}$ is $\mathscr{C}_{i+1}\mathfrak{g}/\mathscr{C}_i\mathfrak{g}$, and the corollary follows immediately from Prop. 5 by induction.

#### Remark {#lie-vii-s2-n1-rem-1 .statement tag=00U0}

$\mathscr{C}_{\infty}\mathfrak{g}$ is the smallest ideal $\mathfrak{n}$ of $\mathfrak{g}$ such that the centre of $\mathfrak{g}/\mathfrak{n}$ is zero; it is a characteristic and nilpotent ideal of $\mathfrak{g}$.

### 2. REGULAR ELEMENTS OF A LIE ALGEBRA

[Recall that $k$ is assumed to be infinite from now on.]

Let $\mathfrak{g}$ be a Lie algebra of dimension $n$. If $x\in \mathfrak{g}$, write the characteristic polynomial of ad $x$ in the form

det(T $-$ ad $x$) $=\sum_{i=0}^na_i(x)T^i$, with $a_i(x)\in k$.

We have $a_i(x) = (-1)^{n-i}$Tr $(\bigwedge^{n-i}$ ad x), cf. Algebra, Chap. III, §8, no. 11. This shows that $x \rightarrow a_i(x)$ is a homogeneous polynomial map of degree $n-i$ from $\mathfrak{g}$ to $k($Algebra, Chap. IV, §5, no. 9).

#### Remark 1 {#lie-vii-s2-n2-rem-1 .statement tag=00U1}

If $\mathfrak{g}\not=\{0\},a_0= 0$ since (ad $x$)$(x) = 0$ for all $x\in \mathfrak{g}$.

#### Remark 2 {#lie-vii-s2-n2-rem-2 .statement tag=00U2}

Let $k'$ be an extension of $k$. Write det(T $-$ ad $x'$) $=\sum_{i=0}^na'_i(x')T^i$ for $x'\in \mathfrak{g}\otimes_kk'$. Then $a'_i|\mathfrak{g}=a_i$ for all $i$.

#### Definition 2 {#lie-vii-s2-def-2 .statement tag=00U3}

The rank of $\mathfrak{g}$, denoted by rk($\mathfrak{g}$), is the smallest integer $l$ such that $a_l\not= 0$. An element $x$ of $\mathfrak{g}$ is called regular if $a_l(x)\not= 0$.

For all $x\in \mathfrak{g}$, rk($\mathfrak{g}$)$\leq$ dim$\mathfrak{g}^0(x)$, and equality holds if and only if $x$ is regular.

The set of regular elements is dense and open in $\mathfrak{g}$ for the Zariski topology (App. I).

#### Example 1 {#lie-vii-s2-n2-exa-1 .statement tag=00U4}

If $\mathfrak{g}$ is nilpotent, rk($\mathfrak{g}$) $=$ dim$\mathfrak{g}$ and all elements of $\mathfrak{g}$ are regular.

#### Example 2 {#lie-vii-s2-n2-exa-2 .statement tag=00U5}

Let $\mathfrak{g}=\mathfrak{s}\mathfrak{l}(2, k)$. If $x=(\gamma -\alpha )\in \mathfrak{g}$, an easy calculation gives

$$
\beta \gamma
$$

det(T $-$ ad $x$) $= T^3-4(\alpha \beta +\gamma^2)T$.

If the characteristic of $k$ is $\not= 2$, then rk($\mathfrak{g}$) $= 1$ and the regular elements are those $x$ such that $\alpha \beta +\gamma^2\not= 0$.

#### Example 3 {#lie-vii-s2-n2-exa-3 .statement tag=00U6}

Let V be a vector space of finite dimension $n$, and $\mathfrak{g}=\mathfrak{g}\mathfrak{l}(V)$. Let $\overline{k}$ be an algebraic closure of $k$. Let $x\in \mathfrak{g}$, and let $\lambda_1, . . . , \lambda_n$ be the roots in $\overline{k}$ of the characteristic polynomial of $x$ (each root being written a number of times equal to its multiplicity). The canonical isomorphism from $V^*\otimes V$ to $\mathfrak{g}$ is compatible with the $\mathfrak{g}$-module structures of these two spaces, in other words it takes $1\otimes x-^tx\otimes 1$ to ad $x$ (Chap. I, §3, no. 3, Prop. 4). In view of §1, Prop. 4 (i), it follows that the roots of the characteristic polynomial of ad $x$ are the $\lambda_i-\lambda_j$ for $1\leq i\leq n,1\leq j\leq n$ (each root being written a number of times equal to its multiplicity). Thus, the rank of $\mathfrak{g}$ is $n$, and $x$ is regular if and only if each $\lambda_i$ is a simple root of the characteristic polynomial of $x$.

#### Proposition 6 {#lie-vii-s2-prop-6 .statement tag=00U7}

Let $\mathfrak{g}$ be a Lie algebra, $k'$ an extension of $k$, and $\mathfrak{g}'=$ $\mathfrak{g}\otimes_kk'$.

(i) An element $x$ of $\mathfrak{g}$ is regular in $\mathfrak{g}$ if and only if $x\otimes 1$ is regular in $\mathfrak{g}'$.

(ii) rk($\mathfrak{g}$) $=$ rk($\mathfrak{g}'$).

This follows from Remark 2.

#### Proposition 7 {#lie-vii-s2-prop-7 .statement tag=01IY}

Let $(\mathfrak{g}_i)_{i\in I}$ be a finite family of Lie algebras, and let $\mathfrak{g}=$ $\prod_{i\in I}\mathfrak{g}_i$.

(i) An element $(x_i)_{i\in I}$ of $\mathfrak{g}$ is regular in $\mathfrak{g}$ if and only if, for all $i\in I,x_i$ is regular in $\mathfrak{g}_i$.

(ii) rk($\mathfrak{g}$) $=\sum_{i\in I}$ rk($\mathfrak{g}_i$).

Indeed, for any $x= (x_i)_{i\in I}\in \mathfrak{g}$, the characteristic polynomial of ad$_{\mathfrak{g}}x$ is the product of the characteristic polynomials of the ad$_{\mathfrak{g}_i}x_i$.

#### Proposition 8 {#lie-vii-s2-prop-8 .statement tag=00U8}

Let $f:\mathfrak{g}\rightarrow \mathfrak{g}'$ be a surjective homomorphism of Lie algebras.

(i) If $x$ is a regular element of $\mathfrak{g},f(x)$ is regular in $\mathfrak{g}'$. The converse is true if Ker $f$ is contained in the centre of $\mathfrak{g}$.

(ii) rk($\mathfrak{g}$)$\geq$ rk($\mathfrak{g}'$).

Put rk($\mathfrak{g}$) $=r$, rk($\mathfrak{g}'$) $=r'$. Let $x\in \mathfrak{g}$. The characteristic polynomials of ad $x$, ad $f(x)$ and ad $x|$Ker $f$ are of the form

$$
P(T) = T^n+a_{n-1}(x)T^{n-1}+\cdots +a_r(x)T^r
$$

$$
Q(T) = T^{n'}+b_{n'-1}(x)T^{n'-1}+\cdots +b_{r'}(x)T^{r'}
$$

$$
R(T) = T^{n''}+c_{n''-1}(x)T^{n''-1}+\cdots +c_{r''}(x)T^{r''}
$$

where the $a_i, b_i, c_i$ are polynomial functions on $\mathfrak{g}$, with $a_r\not= 0, b_{r'}\not= 0, c_{r''}\not= 0$. We have P = QR, so $r=r'+r''$ and $a_r(x) =b_{r'}(x)c_{r''}(x)$, which proves (ii) and the first assertion of (i). If Ker $f$ is contained in the centre of $\mathfrak{g}$, $R(T) = T^{n''}$ and so $a_r(x) =b_{r'}(x)$, hence the second assertion of (i).

#### Corollary {#lie-vii-s2-n2-cor-1 .statement tag=00U9}

Let $\mathscr{C}_n\mathfrak{g}(n\geq 0)$ be a term of the ascending central series of $\mathfrak{g}$ (Chap. I, §1, no. 6). The regular elements of $\mathfrak{g}$ are those whose image in $\mathfrak{g}/\mathscr{C}_n\mathfrak{g}$ is regular.

#### Proposition 9 {#lie-vii-s2-prop-9 .statement tag=00UA}

Let $\mathfrak{g}$ be a Lie algebra, $\mathfrak{g}'$ a subalgebra of $\mathfrak{g}$. Every element of $\mathfrak{g}'$ regular in $\mathfrak{g}$ is regular in $\mathfrak{g}'$.

For $x\in \mathfrak{g}'$, the restriction of ad$_{\mathfrak{g}}x$ to $\mathfrak{g}'$ is ad$_{\mathfrak{g}'}x$, and so defines an endomorphism $u(x)$ of the vector space $\mathfrak{g}/\mathfrak{g}'$ by passage to the quotient. Let $d_0(x)$ (resp. $d_1(x)$) be the dimension of the nilspace of ad$_{\mathfrak{g}'}(x)$ (resp. of $u(x)$), and let $c_0$ (resp. $c_1$) be the minimum of $d_0(x)$ (resp. $d_1(x)$) when $x$ belongs to $\mathfrak{g}'$. There exist non-zero polynomial maps $p_0, p_1$ from $\mathfrak{g}'$ to $k$ such that

$$
d_0(x) =c_0\Leftarrow \Rightarrow p_0(x)\not= 0,d_1(x) =c_1\Leftarrow \Rightarrow p_1(x)\not= 0
$$

Since $k$ is infinite, the set S of $x\in \mathfrak{g}'$ such that $d_0(x) =c_0$ and $d_1(x) =c_1$ is non-empty. Every element of S is regular in $\mathfrak{g}'$. On the other hand, S is the set of elements of $\mathfrak{g}'$ such that the nilspace of ad$_{\mathfrak{g}}x$ has minimum dimension, and thus contains every element of $\mathfrak{g}'$ regular in $\mathfrak{g}$.

#### Remark 3 {#lie-vii-s2-n2-rem-3 .statement tag=00UB}

Elements of $\mathfrak{g}'$ regular in $\mathfrak{g}$ do not necessarily exist. If at least one does exist, the set of these elements is precisely the set denoted by S in the above proof.

### 3. CARTAN SUBALGEBRAS AND REGULAR ELEMENTS

#### Theorem 1 {#lie-vii-s2-thm-1 .statement tag=00UC}

Let $\mathfrak{g}$ be a Lie algebra.

(i) If $x$ is a regular element of $\mathfrak{g},\mathfrak{g}^0(x)$ is a Cartan subalgebra of $\mathfrak{g}$.

(ii) If $\mathfrak{h}$ is a maximal nilpotent subalgebra of $\mathfrak{g}$, and if $x\in \mathfrak{h}$ is regular in $\mathfrak{g}$, then $\mathfrak{h}=\mathfrak{g}^0(x)$.

(iii) If $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$, then dim($\mathfrak{h}$)$\geq$ rk($\mathfrak{g}$).

(iv) The Cartan subalgebras of $\mathfrak{g}$ of dimension rk($\mathfrak{g}$) are the $\mathfrak{g}^0(x)$ where $x$ is a regular element.

Let $x$ be a regular element of $\mathfrak{g}$ and let $\mathfrak{h}=\mathfrak{g}^0(x)$. Clearly $\mathfrak{h}^0(x) =\mathfrak{h}$. Since $x$ is regular in $\mathfrak{h}$ (Prop. 9), rk($\mathfrak{h}$) $=$ dim($\mathfrak{h}$), so $\mathfrak{h}$ is nilpotent. On the other hand, $\mathfrak{h}=\mathfrak{g}^0(x)\supset \mathfrak{g}^0(\mathfrak{h})\supset \mathfrak{h}$, so $\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$ is a Cartan subalgebra of $\mathfrak{g}$ (Prop. 4). This proves (i).

If $\mathfrak{h}$ is a maximal nilpotent subalgebra of $\mathfrak{g}$, and if $x\in \mathfrak{h}$ is regular in $\mathfrak{g}$, then $\mathfrak{h}\subset \mathfrak{g}^0(x)$ and $\mathfrak{g}^0(x)$ is nilpotent by (i), so $\mathfrak{h}=\mathfrak{g}^0(x)$, which proves (ii).

If $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$, there exists $x\in \mathfrak{h}$ such that $\mathfrak{h}=\mathfrak{g}^0(x)$ (Cor. 1 of Prop. 4), so dim($\mathfrak{h}$)$\geq$ rk($\mathfrak{g}$), which proves (iii). If in addition dim($\mathfrak{h}$) $=$ rk($\mathfrak{g}$)$,x$ is regular. Finally, if $x'$ is regular in $\mathfrak{g},\mathfrak{g}^0(x')$ is a Cartan subalgebra by (i), and is obviously of dimension rk($\mathfrak{g}$). This proves (iv).

We shall see in §3, Th. 2 that, when $k$ is of characteristic zero, all the Cartan subalgebras of $\mathfrak{g}$ have dimension rk($\mathfrak{g}$).

#### Corollary 1 {#lie-vii-s2-thm-1-cor-1 .statement tag=00UD}

Every Lie algebra $\mathfrak{g}$ has Cartan subalgebras, and the rank of $\mathfrak{g}$ is the minimum dimension of a Cartan subalgebra.

#### Corollary 2 {#lie-vii-s2-thm-1-cor-2 .statement tag=00UE}

Let $f:\mathfrak{g}\rightarrow \mathfrak{g}'$ be a surjective homomorphism of Lie algebras. If $\mathfrak{h}'$ is a Cartan subalgebra of $\mathfrak{g}'$, there exists a Cartan subalgebra $\mathfrak{h}$ of $\mathfrak{g}$ such that $\mathfrak{h}'=f(\mathfrak{h})$.

Let $\mathfrak{a}=f^{-1}(\mathfrak{h}')$. By Cor. $1,\mathfrak{a}$ has a Cartan subalgebra $\mathfrak{h}$. By Cor. 2 of Prop. $4,f(\mathfrak{h}) =\mathfrak{h}'$. We show that $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$. Let $\mathfrak{n}$ be the normalizer of $\mathfrak{h}$ in $\mathfrak{g}$. It is enough to prove that $\mathfrak{h}=\mathfrak{n}$. If $x\in \mathfrak{n},f(x)$ belongs to the normalizer of $\mathfrak{h}'$ in $\mathfrak{g}'$, so $f(x)\in \mathfrak{h}'$ and $x\in \mathfrak{a}$; but $\mathfrak{h}$ is its own normalizer in $\mathfrak{a}$, so $x\in \mathfrak{h}$.

#### Corollary 3 {#lie-vii-s2-thm-1-cor-3 .statement tag=00UF}

Every Lie algebra $\mathfrak{g}$ is the sum of its Cartan subalgebras.

The sum $\mathfrak{s}$ of the Cartan subalgebras of $\mathfrak{g}$ contains the set of regular elements of $\mathfrak{g}$ (Th. 1 (i)). Since this set is dense in $\mathfrak{g}$ for the Zariski topology, $\mathfrak{s}=\mathfrak{g}$.

#### Proposition 10 {#lie-vii-s2-prop-10 .statement tag=00UG}

Let $\mathfrak{g}$ be a Lie algebra, $\mathfrak{a}$ a commutative subalgebra of $\mathfrak{g}$ and $\mathfrak{c}$ the commutant of $\mathfrak{a}$ in $\mathfrak{g}$. Assume that ad$_{\mathfrak{g}}x$ is semi-simple for all $x\in \mathfrak{a}$. Then the Cartan subalgebras of $\mathfrak{c}$ are the Cartan subalgebras of $\mathfrak{g}$ containing $\mathfrak{a}$.

Let $\mathfrak{h}$ be a Cartan subalgebra of $\mathfrak{c}$. Since $\mathfrak{a}$ is contained in the centre $\mathfrak{z}$ of $\mathfrak{c},\mathfrak{a}\subset \mathfrak{z}\subset \mathfrak{h}$ (Prop. 5). Let $\mathfrak{n}$ be the normalizer of $\mathfrak{h}$ in $\mathfrak{g}$. Then

$$
[\mathfrak{a},\mathfrak{n}]\subset [\mathfrak{h},\mathfrak{n}]\subset \mathfrak{h}
$$

Since the ad$_{\mathfrak{g}}x,x\in \mathfrak{a}$, are semi-simple and commute with each other, it follows from Algebra, Chap. VIII, §5, no. 1, that there exists a vector subspace $\mathfrak{d}$ of $\mathfrak{n}$ stable under ad$_{\mathfrak{g}}\mathfrak{a}$ and such that $\mathfrak{n}=\mathfrak{h}\oplus \mathfrak{d}$. Then $[\mathfrak{a},\mathfrak{d}]\subset \mathfrak{h}\cap \mathfrak{d}= 0$, so $\mathfrak{d}\subset \mathfrak{c}$. Thus, $\mathfrak{n}$ is the normalizer of $\mathfrak{h}$ in $\mathfrak{c}$, and hence $\mathfrak{n}=\mathfrak{h}$, so $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$ containing $\mathfrak{a}$.

Conversely, let $\mathfrak{h}$ be a Cartan subalgebra of $\mathfrak{g}$ containing $\mathfrak{a}$. Then $\mathfrak{h}=$ $\mathfrak{g}^0(\mathfrak{h})\subset \mathfrak{g}^0(\mathfrak{a})$, and by hypothesis $\mathfrak{g}_0(\mathfrak{a}) =\mathfrak{g}^0(\mathfrak{a}) =\mathfrak{c}$. Hence $\mathfrak{a}\subset \mathfrak{h}\subset \mathfrak{c}$ and $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{c}$ (for it is equal to its own normalizer in $\mathfrak{g}$, and so a fortiori in $\mathfrak{c}$).

#### Proposition 11 {#lie-vii-s2-prop-11 .statement tag=00UH}

Let $\mathfrak{n}$ be a nilpotent subalgebra of a Lie algebra $\mathfrak{g}$. There exists a Cartan subalgebra of $\mathfrak{g}$ contained in $\mathfrak{g}^0(\mathfrak{n})$.

Put $\mathfrak{a}=\mathfrak{g}^0(\mathfrak{n})$. Then $\mathfrak{n}\subset \mathfrak{a}$ since $\mathfrak{n}$ is nilpotent. If $x\in \mathfrak{a}$, let $P(x)$ be the determinant of the endomorphism of $\mathfrak{g}/\mathfrak{a}$ defined by ad $x$. Denote by $\mathfrak{a}'$ the set of $x\in \mathfrak{a}$ such that $P(x)\not= 0$, which is an open subset of $\mathfrak{a}$ in the Zariski topology; the relations $x\in \mathfrak{a}'$ and $\mathfrak{g}^0(x)\subset \mathfrak{a}$ are equivalent. By Prop. 7 (ii) of §1, no. 2, there exists $y\in \mathfrak{n}$ such that $\mathfrak{g}^0(y) =\mathfrak{a}$, and $y\in \mathfrak{a}'$ so $\mathfrak{a}'$ is non-empty. Since $\mathfrak{a}'$ is open, its intersection with the set of regular elements of $\mathfrak{a}$ is non-empty. Let $x$ be an element of this intersection. Then $\mathfrak{g}^0(x)\subset \mathfrak{a}$ and $\mathfrak{g}^0(x)$ is a Cartan subalgebra of $\mathfrak{a}$, hence is nilpotent. On the other hand, Prop. 10 (i) of §1, no. 3, shows that $\mathfrak{g}^0(x)$ is its own normalizer in $\mathfrak{g}$; it is therefore a Cartan subalgebra of $\mathfrak{g}$, which completes the proof.

### 4. CARTAN SUBALGEBRAS OF SEMI-SIMPLE LIE ALGEBRAS

#### Theorem 2 {#lie-vii-s2-thm-2 .statement tag=00UI}

Assume that $k$ is of characteristic 0. Let $\mathfrak{g}$ be a semi-simple Lie algebra, $\mathfrak{h}$ a Cartan subalgebra of $\mathfrak{g}$. Then $\mathfrak{h}$ is commutative, and all of its elements are semi-simple in $\mathfrak{g}$ (Chap. I, §6, no. 3, Def. 3).

Since $\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h}),\mathfrak{h}$ is reductive (§1, Prop. 11), hence commutative since it is nilpotent. On the other hand, the restriction of the adjoint representation of $\mathfrak{g}$ to $\mathfrak{h}$ is semi-simple (loc. cit.), so the elements of $\mathfrak{h}$ are semi-simple in $\mathfrak{g}$ (Algebra, Chap. VIII, §5, no. 1).

#### Corollary 1 {#lie-vii-s2-thm-2-cor-1 .statement tag=00UJ}

If $x\in \mathfrak{h}$ and $y\in \mathfrak{g}^{\lambda}(\mathfrak{h})$, we have $[x, y] =\lambda (x)y$.

Indeed, $\mathfrak{g}^{\lambda(x)}(x) =\mathfrak{g}_{\lambda(x)}(x)$ since ad $x$ is semi-simple.

#### Corollary 2 {#lie-vii-s2-thm-2-cor-2 .statement tag=00UK}

Every regular element of $\mathfrak{g}$ is semi-simple.

Indeed, such an element belongs to a Cartan subalgebra (no. 3, Th. 1 (i)).

#### Corollary 3 {#lie-vii-s2-thm-2-cor-3 .statement tag=00UL}

Let $\mathfrak{h}$ be a Cartan subalgebra of a reductive Lie algebra $\mathfrak{g}$.

a$)\mathfrak{h}$ is commutative.

b) If $\rho$ is a finite dimensional semi-simple representation of $\mathfrak{g}$, the elements of $\rho (\mathfrak{h})$ are semi-simple.

Let $\mathfrak{c}$ be the centre of $\mathfrak{g}$, and $\mathfrak{s}$ its derived algebra. Then $\mathfrak{g}=\mathfrak{c}\times \mathfrak{s}$, so $\mathfrak{h}=\mathfrak{c}\times \mathfrak{h}'$, where $\mathfrak{h}'$ is a Cartan subalgebra of $\mathfrak{s}$ (Prop. 2). In view of Th. $2,\mathfrak{h}'$ is commutative, hence so is $\mathfrak{h}$. Moreover, $\rho (\mathfrak{h}')$ consists of semi-simple elements and so does $\rho (\mathfrak{c})$ (Chap. I, §6, no. 5, Th. 4); assertion b) follows.

### Exercises {#lie-vii-s2-exercises}

See the [exercises for § 2](exercises/s2/).
