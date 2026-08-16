---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 5
section_title: Decomposable linear Lie algebras
lang: en
source: lie-vii-ix
book_pages: 34-45, 63-66
pdf_pages: 0044-0055, 0072-0075
extraction: native
subsections:
    - "no": 1
      title: DECOMPOSABLE LINEAR LIE ALGEBRAS
      page: 34
      pdf_page: 44
    - "no": 2
      title: DECOMPOSABLE ENVELOPE
      page: 37
      pdf_page: 47
    - "no": 3
      title: DECOMPOSITIONS OF DECOMPOSABLE ALGEBRAS
      page: 37
      pdf_page: 47
    - "no": 4
      title: LINEAR LIE ALGEBRAS OF NILPOTENT ENDOMORPHISMS
      page: 39
      pdf_page: 49
    - "no": 5
      title: CHARACTERIZATIONS OF DECOMPOSABLE LIE ALGEBRAS
      page: 43
      pdf_page: 53
statements: 29
exercises: 11
content_sha256: 7a2b8fd2c87e6ff2d8189963f1e5dd66074d658bc49c392b226ae69eb4f3454e
---

## § 5. DECOMPOSABLE LINEAR LIE ALGEBRAS

In this paragraph, $k$ is assumed to be of characteristic 0. We denote by V a finite dimensional vector space.

### 1. DECOMPOSABLE LINEAR LIE ALGEBRAS

#### Definition 1 {#lie-vii-s5-def-1 .statement tag=00WG}

Let $\mathfrak{g}$ be a Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$. Then $\mathfrak{g}$ is said to be decomposable if $\mathfrak{g}$ contains the semi-simple and nilpotent components of each of its elements (Algebra, Chap. VII, §5, no. 8).

#### Example 1 {#lie-vii-s5-n1-exa-1 .statement tag=00WH}

Let $V'$ and $V''$ be vector subspaces of V such that $V''\supset V'$. The set of $x\in \mathfrak{g}\mathfrak{l}(V)$ such that $x(V'')\subset V'$ is a decomposable Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$; indeed, for all $x\in \mathfrak{g}\mathfrak{l}$(V), the semi-simple and nilpotent components of $x$ are of the form $P(x)$ and $Q(x)$, where P and Q are polynomials without constant term.

#### Example 2 {#lie-vii-s5-n1-exa-2 .statement tag=00WI}

Assume that V has an algebra structure. The set of derivations of V is a decomposable Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V) ($§1, no. 1, Prop. 4 (ii)).

#### Example 3 {#lie-vii-s5-n1-exa-3 .statement tag=01KQ}

More generally, it can be shown that the Lie algebra of any algebraic subgroup of $\mathbf{G}\mathbf{L}(V)$ is decomposable.$_*$

#### Proposition 1 {#lie-vii-s5-prop-1 .statement tag=00WJ}

Let $\mathfrak{g}$ be a decomposable Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V),x\in \mathfrak{g},s$ and $n$ the semi-simple and nilpotent components of $x$.

(i) The semi-simple and nilpotent components of ad$_{\mathfrak{g}}x$ are ad$_{\mathfrak{g}}s$ and ad$_{\mathfrak{g}}n$, respectively.

(ii) $x$ is regular in $\mathfrak{g}$ if and only if $s$ is.

(iii) If $\mathfrak{g}'$ is a subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ containing $\mathfrak{g}$, every elementary automorphism of $\mathfrak{g}$ extends to an elementary automorphism of $\mathfrak{g}'$.

Put $\mathfrak{a}=\mathfrak{g}\mathfrak{l}(V)$. By Chap. I, §5, no. 4, Lemma 2, the semi-simple and nilpotent components of ad$_{\mathfrak{a}}x$ are ad$_{\mathfrak{a}}s$ and ad$_{\mathfrak{a}}n$; assertion (i) follows from this. We deduce that the characteristic polynomials of ad$_{\mathfrak{g}}x$ and ad$_{\mathfrak{g}}s$ are the same; hence (ii). If ad$_{\mathfrak{g}}x$ is nilpotent, ad$_{\mathfrak{g}}x=$ ad$_{\mathfrak{g}}n$, so ad$_{\mathfrak{g}'}n$ extends ad$_{\mathfrak{g}}x$, and $n$ is a nilpotent element of $\mathfrak{g}'$, hence (iii).

Let $\mathfrak{g}$ be a Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$. We know (Chap. I, §6, no. 5, Th. 4) that the following conditions are equivalent:

(i) the identity representation of $\mathfrak{g}$ is semi-simple;

(ii) $\mathfrak{g}$ is reductive and every element of the centre of $\mathfrak{g}$ is a semi-simple endomorphism.

These conditions are actually equivalent to the following:

(iii) $\mathfrak{g}$ is a reductive subalgebra in $\mathfrak{g}\mathfrak{l}(V)$.

Indeed, (i) $=\Rightarrow$ (iii) by Chap. I, §6, no. 5, Cor. 3 of Th. 4, and (iii) $=\Rightarrow$ (i) by Chap. I, §6, no. 6, Cor. 1 of Prop. 7. We are going to show that if $\mathfrak{g}$ satisfies these conditions, $\mathfrak{g}$ is decomposable. More generally:

#### Proposition 2 {#lie-vii-s5-prop-2 .statement tag=00WK}

Let $\mathfrak{g}$ be a Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ reductive in $\mathfrak{g}\mathfrak{l}(V)$, E a finite dimensional vector space and $\pi :\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(E)$ a semi-simple linear representation of $\mathfrak{g}$ on E. Then:

(i) $\mathfrak{g}$ and $\pi (\mathfrak{g})$ are decomposable.

(ii) The semi-simple (resp. nilpotent) elements of $\pi (\mathfrak{g})$ are the images under $\pi$ of the semi-simple (resp. nilpotent) elements of $\mathfrak{g}$.

(iii) If $\mathfrak{h}$ is a decomposable subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ contained in $\mathfrak{g},\pi (\mathfrak{h})$ is a decomposable subalgebra of $\mathfrak{g}\mathfrak{l}(E)$.

(iv) If $\mathfrak{h}'$ is a decomposable subalgebra of $\mathfrak{g}\mathfrak{l}(E),\pi^{-1}(\mathfrak{h}')$ is a decomposable subalgebra of $\mathfrak{g}\mathfrak{l}(V)$.

Let $\mathfrak{s}= [\mathfrak{g},\mathfrak{g}]$ and let $\mathfrak{c}$ be the centre of $\mathfrak{g}$. Then $\mathfrak{g}=\mathfrak{s}\times \mathfrak{c}$, and $\pi (\mathfrak{g}) =$ $\pi (\mathfrak{s})\times \pi (\mathfrak{c})$ by Chap. I, §6, no. 4, Cor. of Prop. 5. Let $y\in \mathfrak{s}, z\in \mathfrak{c}, y_s$ and $y_n$ the semi-simple and nilpotent components of $y$. Then $y_s, y_n\in \mathfrak{s}$ (Chap. I, §6, no. 3, Prop. $3),y_s+z$ is semi-simple (Algebra, Chap. VII, §5, no. 7, Cor. of Prop. 16), and $y_n$ commutes with $y_s+z$. Hence, the semi-simple and nilpotent components of $y+z$ are $y_s+z$ and $y_n$. Thus, $\mathfrak{g}$ is decomposable. Since $\pi (\mathfrak{g})$ is reductive in $\mathfrak{g}\mathfrak{l}$(E), the same argument applies to $\pi (\mathfrak{g})$ and shows that $\pi (\mathfrak{g})$ is decomposable. Moreover, the nilpotent elements of $\mathfrak{g}$ (resp. $\pi (\mathfrak{g}))$ are the nilpotent elements of $\mathfrak{s}$ (resp. $\pi (\mathfrak{s}))$. Hence the nilpotent elements of $\pi (\mathfrak{g})$ are the images under $\pi$ of the nilpotent elements of $\mathfrak{g}$ (Chap. I, §6, no. 3, Prop. 4). The semi-simple elements of $\mathfrak{g}$ (resp. $\pi (\mathfrak{g}))$ are the sums of the semi-simple elements of $\mathfrak{s}$ (resp. $\pi (\mathfrak{s}))$ and the elements of $\mathfrak{c}$ (resp. $\pi (\mathfrak{c}))$. Thus the semi-simple elements of $\pi (\mathfrak{g})$ are the images under $\pi$ of the semi-simple elements of $\mathfrak{g}$ (Chap. I, loc. cit.). Hence (ii).

Assertions (iii) and (iv) follow immediately from (i) and (ii).

#### Remark 1 {#lie-vii-s5-n1-rem-1 .statement tag=00WL}

The semi-simplicity assumption on $\pi$ is equivalent to saying that $\pi (x)$ is semi-simple for all $x\in \mathfrak{c}$. Note that this assumption is satisfied when $\pi$ is obtained from the identity representation $\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(V)$ by the successive application of the following operations: tensor product, passage to the dual, to a subrepresentation, to a quotient, to a direct sum.

#### Remark 2 {#lie-vii-s5-n1-rem-2 .statement tag=00WM}

Let $\mathfrak{g}\subset \mathfrak{g}\mathfrak{l}$(V), $\mathfrak{g}'\subset \mathfrak{g}\mathfrak{l}(V')$ be decomposable Lie algebras, $\varphi$ an isomorphism from $\mathfrak{g}$ to $\mathfrak{g}'$. Note that $\varphi$ does not necessarily transform semi-simple (resp. nilpotent) elements of $\mathfrak{g}$ to semi-simple (resp. nilpotent) elements of $\mathfrak{g}'$ (Exerc. 2). However, this is the case if $\mathfrak{g}$ is semi-simple (Chap. I, §6, no. 3, Th. 3).

#### Proposition 3 {#lie-vii-s5-prop-3 .statement tag=00WN}

Let $\mathfrak{a}$ be a decomposable Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ and let $\mathfrak{b}$ and $\mathfrak{c}$ be vector subspaces of $\mathfrak{g}\mathfrak{l}(V)$ such that $\mathfrak{b}\subset \mathfrak{c}$. Let $\mathfrak{a}'$ be the set of $x\in \mathfrak{a}$ such that $[x,\mathfrak{c}]\subset \mathfrak{b}$. Then $\mathfrak{a}'$ is decomposable.

Put $\mathfrak{g}=\mathfrak{g}\mathfrak{l}(V)$; the subalgebra $\mathfrak{h}'$ of $\mathfrak{g}\mathfrak{l}(\mathfrak{g})$ consisting of the $z\in \mathfrak{g}\mathfrak{l}(\mathfrak{g})$ such that $z(\mathfrak{c})\subset \mathfrak{b}$ is decomposable (Example 1). Let $\pi :\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(\mathfrak{g})$ be the adjoint representation of $\mathfrak{g}$. Prop. 2 (iv), applied to $\pi$, shows that $\pi^{-1}(\mathfrak{h}')$ is decomposable. Hence so is $\mathfrak{a}'=\mathfrak{a}\cap \pi^{-1}(\mathfrak{h}')$.

#### Corollary 1 {#lie-vii-s5-prop-3-cor-1 .statement tag=00WO}

If $\mathfrak{a}$ is a decomposable Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$, and $\mathfrak{n}$ a Lie subalgebra of $\mathfrak{a}$, the normalizer (resp. centralizer) of $\mathfrak{n}$ in $\mathfrak{a}$ is decomposable.

This follows from Prop. 3 by taking $\mathfrak{c}=\mathfrak{n},\mathfrak{b}=\mathfrak{n}$ (resp. $\mathfrak{c}=\mathfrak{n},\mathfrak{b}=\{0\})$.

#### Corollary 2 {#lie-vii-s5-prop-3-cor-2 .statement tag=00WP}

The Cartan subalgebras of a decomposable Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ are decomposable.

This follows from Corollary 1.

#### Remark {#lie-vii-s5-n1-rem-3 .statement tag=00WQ}

We shall prove later (no. 5, Th. 2) a converse of Cor. 2.

### 2. DECOMPOSABLE ENVELOPE

The intersection of a family of decomposable Lie subalgebras of $\mathfrak{g}\mathfrak{l}(V)$ is clearly decomposable. Consequently, if $\mathfrak{g}$ is a Lie subalgebra of $\mathfrak{g}\mathfrak{l}$(V), the set of decomposable Lie subalgebras of $\mathfrak{g}\mathfrak{l}(V)$ containing $\mathfrak{g}$ has a smallest element, called the decomposable envelope of $\mathfrak{g}$; in this paragraph, this envelope will be denoted by $e(\mathfrak{g})$.

#### Proposition 4 {#lie-vii-s5-prop-4 .statement tag=00WR}

Let $\mathfrak{g}$ be a Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ and $\mathfrak{n}$ an ideal of $\mathfrak{g}$. Then $\mathfrak{n}$ and $e(\mathfrak{n})$ are ideals of $e(\mathfrak{g})$, and $[e(\mathfrak{g}), e(\mathfrak{n})] = [\mathfrak{g},\mathfrak{n}]$.

Let $\mathfrak{g}_1$ be the set of $x\in \mathfrak{g}\mathfrak{l}(V)$ such that $[x,\mathfrak{n}]\subset [\mathfrak{g},\mathfrak{n}]$. This is a decomposable Lie subalgebra of $\mathfrak{g}\mathfrak{l}$(V), containing $\mathfrak{g}$ and hence $e(\mathfrak{g})$, cf. no. 1, Prop. 3; in other words, $[e(\mathfrak{g}),\mathfrak{n}]\subset [\mathfrak{g},\mathfrak{n}]$. Let $\mathfrak{n}_1$ be the set of $y\in \mathfrak{g}\mathfrak{l}(V)$ such that

$$
[e(\mathfrak{g}), y]\subset [\mathfrak{g},\mathfrak{n}]
$$

This is a decomposable Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ containing $\mathfrak{n}$ by the preceding, and hence containing $e(\mathfrak{n})$; in other words $[e(\mathfrak{g}), e(\mathfrak{n})]\subset [\mathfrak{g},\mathfrak{n}]$, so

$$
[e(\mathfrak{g}), e(\mathfrak{n})] = [\mathfrak{g},\mathfrak{n}]
$$

It follows that $[e(\mathfrak{g}),\mathfrak{n}]\subset [e(\mathfrak{g}), e(\mathfrak{n})]\subset \mathfrak{n}$, so $\mathfrak{n}$ and $e(\mathfrak{n})$ are ideals of $e(\mathfrak{g})$.

#### Corollary 1 {#lie-vii-s5-prop-4-cor-1 .statement tag=00WS}

(i) $\mathscr{D}^i\mathfrak{g}=\mathscr{D}^ie(\mathfrak{g})$ for $i\geq 1$, and $\mathscr{C}^i\mathfrak{g}=\mathscr{C}^ie(\mathfrak{g})$ for $i\geq 2$.

(ii) If $\mathfrak{g}$ is commutative (resp. nilpotent, resp. solvable), then $e(\mathfrak{g})$ is commutative (resp. nilpotent, resp. solvable).

Assertion (i) follows from Prop. 4 by induction on $i$ and (ii) follows from (i).

#### Corollary 2 {#lie-vii-s5-prop-4-cor-2 .statement tag=00WT}

Let $\mathfrak{r}$ be the radical of $\mathfrak{g}$. If $\mathfrak{g}$ is decomposable, $\mathfrak{r}$ is decomposable.

Indeed, $e(\mathfrak{r})$ is a solvable ideal of $\mathfrak{g}$ by Prop. 4 and Cor. 1, hence $e(\mathfrak{r}) =\mathfrak{r}$.

### 3. DECOMPOSITIONS OF DECOMPOSABLE ALGEBRAS

If $\mathfrak{g}$ is a Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ with radical $\mathfrak{r}$, the set of nilpotent elements of $\mathfrak{r}$ is a nilpotent ideal of $\mathfrak{g}$, the largest nilpotency ideal of the identity representation of $\mathfrak{g}$ (Chap. I, §5, no. 3, Cor. 6 of Th. 1). In this paragraph, we shall denote this ideal by $\mathfrak{n}_V(\mathfrak{g})$. It contains the nilpotent radical $[\mathfrak{g},\mathfrak{g}]\cap \mathfrak{r}$ of $\mathfrak{g}$ (Chap. I, §5, no. 3, Th. 1).

#### Proposition 5 {#lie-vii-s5-prop-5 .statement tag=00WU}

Let $\mathfrak{g}$ be a decomposable nilpotent Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$. Let $\mathfrak{t}$ be the set of semi-simple elements of $\mathfrak{g}$. Then $\mathfrak{t}$ is a central subalgebra of $\mathfrak{g}$, and $\mathfrak{g}$ is the product of $\mathfrak{t}$ and $\mathfrak{n}_V(\mathfrak{g})$ as Lie algebras.

If $x\in \mathfrak{t}$, ad$_{\mathfrak{g}}x$ is semi-simple and nilpotent, hence zero, so that $x$ is central in $\mathfrak{g}$. Consequently, $\mathfrak{t}$ is an ideal of $\mathfrak{g}$, and $\mathfrak{t}\cap \mathfrak{n}_V(\mathfrak{g}) = 0$. Since $\mathfrak{g}$ is decomposable, $\mathfrak{g}=\mathfrak{t}+\mathfrak{n}_V(\mathfrak{g})$, hence the proposition.

#### Proposition 6 {#lie-vii-s5-prop-6 .statement tag=00WV}

Let $\mathfrak{g}$ be a decomposable Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$. Let $\mathscr{T}$ be the set of commutative subalgebras of $\mathfrak{g}$ consisting of semi-simple elements, and $\mathscr{T}_1$ the set of maximal elements of $\mathscr{T}$. Let $\mathscr{H}$ be the set of Cartan subalgebras of $\mathfrak{g}$.

(i) For $\mathfrak{h}\in \mathscr{H}$, let $\varphi (\mathfrak{h})$ be the set of semi-simple elements of $\mathfrak{h}$. Then $\varphi (\mathfrak{h})\in \mathscr{T}_1$.

(ii) For $\mathfrak{t}\in \mathscr{T}_1$, let $\psi (\mathfrak{t})$ be the commutant of $\mathfrak{t}$ in $\mathfrak{g}$. Then $\psi (\mathfrak{t})\in \mathscr{H}$.

(iii) The maps $\varphi$ and $\psi$ are inverse bijections from $\mathscr{H}$ to $\mathscr{T}_1$ and from $\mathscr{T}_1$ to $\mathscr{H}$.

(iv) If $k$ is algebraically closed, Aut$_e(\mathfrak{g})$ operates transitively on $\mathscr{T}_1$.

Let $\mathfrak{h}\in \mathscr{H}$, and put $\mathfrak{t}=\varphi (\mathfrak{h})$. By Prop. 5 and Cor. 2 of Prop. $3,\mathfrak{t}\in \mathscr{T}$ and $\mathfrak{h}=\mathfrak{t}\times \mathfrak{n}_V(\mathfrak{h})$. For any subalgebra $\mathfrak{u}$ of $\mathfrak{g}$, we denote by $\psi (\mathfrak{u})$ the commutant of $\mathfrak{u}$ in $\mathfrak{g}$. Then $\mathfrak{h}\subset \psi (\mathfrak{t})$, and $\psi (\mathfrak{t})\subset \mathfrak{g}^0(\mathfrak{h})$ since the elements of $\mathfrak{n}_V(\mathfrak{h})$ are nilpotent, so $\mathfrak{h}=\psi (\mathfrak{t})$. If $\mathfrak{t}'\in \mathscr{T}$ and $\mathfrak{t}\subset \mathfrak{t}'$, we have $\mathfrak{t}'\subset \psi (\mathfrak{t}) =\mathfrak{h}$ so $\mathfrak{t}'=\mathfrak{t}$, and hence $\mathfrak{t}\in \mathscr{T}_1$.

Let $\mathfrak{t}\in \mathscr{T}_1$, and put $\mathfrak{c}=\psi (\mathfrak{t})$. Let $\mathfrak{h}$ be a Cartan subalgebra of $\mathfrak{c}$. By §2, no. 3, Prop. $10,\mathfrak{h}\in \mathscr{H}$ and $\mathfrak{t}\subset \mathfrak{h}$. Put $\mathfrak{t}_1=\varphi (\mathfrak{h})\in \mathscr{T}$. Then $\mathfrak{t}\subset \mathfrak{t}_1$ so $\mathfrak{t}=\mathfrak{t}_1$, and $\mathfrak{h}=\psi (\mathfrak{t}_1) =\psi (\mathfrak{t}) =\mathfrak{c}$ by the preceding. Thus, $\psi (\mathfrak{t})\in \mathscr{H}$, and $\varphi (\psi (\mathfrak{t})) =\mathfrak{t}$.

We have thus proved (i), (ii) and (iii). Assume that $k$ is algebraically closed. Since Aut$_e(\mathfrak{g})$ operates transitively on $\mathscr{H}($§3, no. 2, Th. 1), Aut$_e(\mathfrak{g})$ operates transitively on $\mathscr{T}_1$.

#### Corollary 1 {#lie-vii-s5-prop-6-cor-1 .statement tag=00WW}

The Cartan subalgebras of $\mathfrak{g}$ are the centralizers of the regular semi-simple elements of $\mathfrak{g}$.

If $x\in \mathfrak{g}$ is regular, $\mathfrak{g}^0(x)$ is a Cartan subalgebra of $\mathfrak{g}($§2, no. 3, Th. 1 (i)); moreover, if $x$ is semi-simple $\mathfrak{g}^0(x)$ is the centralizer of $x$ in $\mathfrak{g}$. Conversely, let $\mathfrak{h}$ be a Cartan subalgebra of $\mathfrak{g}$. There exists $\mathfrak{t}\in \mathscr{T}_1$ such that $\mathfrak{h}=\psi (\mathfrak{t})$. By §1, no. 2, Prop. 7, there exists $x\in \mathfrak{t}$ such that $\mathfrak{h}=\mathfrak{g}^0(x)$; since $x\in \mathfrak{t}$, $\mathfrak{g}^0(x) =\mathfrak{g}_0(x)$. By §3, no. 3, Th. 2 (ii), $x$ is regular.

#### Corollary 2 {#lie-vii-s5-prop-6-cor-2 .statement tag=00WX}

Assume in addition that $\mathfrak{g}$ is solvable. Then:

(i) The subgroup of Aut($\mathfrak{g}$) consisting of the $e^{adx}, x\in \mathscr{C}^{\infty}\mathfrak{g}$ (cf. §3, no. 4), operates transitively on $\mathscr{T}_1$.

(ii) If $\mathfrak{t}\in \mathscr{T}_1,\mathfrak{g}$ is the semi-direct product of $\mathfrak{t}$ and $\mathfrak{n}_V(\mathfrak{g})$.

Assertion (i) follows from the fact that the group of the $e^{adx},x\in \mathscr{C}^{\infty}\mathfrak{g}$, operates transitively on $\mathscr{H}($§3, no. 4, Th. 3).

We prove (ii). Let $\mathfrak{t}\in \mathscr{T}_1$, and let $\mathfrak{h}=\psi (\mathfrak{t})$ be the corresponding Cartan subalgebra of $\mathfrak{g}$. In view of Prop. $5,\mathfrak{h}=\mathfrak{t}+\mathfrak{n}_V(\mathfrak{h})\subset \mathfrak{t}+\mathfrak{n}_V(\mathfrak{g})$. On the other hand, $\mathfrak{g}=\mathfrak{h}+ [\mathfrak{g},\mathfrak{g}] ($§2, no. 1, Cor. 3 of Prop. 4) and $[\mathfrak{g},\mathfrak{g}]\subset \mathfrak{n}_V(\mathfrak{g})$, so $\mathfrak{g}=\mathfrak{t}+\mathfrak{n}_V(\mathfrak{g})$. But it is clear that $\mathfrak{t}\cap \mathfrak{n}_V(\mathfrak{g}) =\{0\}$. The algebra $\mathfrak{g}$ is thus the semi-direct product of $\mathfrak{t}$ and the ideal $\mathfrak{n}_V(\mathfrak{g})$.

#### Proposition 7 {#lie-vii-s5-prop-7 .statement tag=00WY}

Let $\mathfrak{g}$ be a decomposable Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$.

(i) There exists a Lie subalgebra $\mathfrak{m}$ of $\mathfrak{g}$, reductive in $\mathfrak{g}\mathfrak{l}(V)$, such that $\mathfrak{g}$ is the semi-direct product of $\mathfrak{m}$ and $\mathfrak{n}_V(\mathfrak{g})$.

(ii) Any two Lie subalgebras of $\mathfrak{g}$ with the properties in (i) are conjugate under Aut$_e(\mathfrak{g})$.

The radical $\mathfrak{r}$ of $\mathfrak{g}$ is decomposable (no. 2, Cor. 2 of Prop. 4). By Cor. 2 of Prop. 6, there exists a commutative subalgebra $\mathfrak{t}$ of $\mathfrak{r}$, consisting of semi-simple elements, such that $\mathfrak{r}=\mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{r})$. Since ad$_{\mathfrak{g}}\mathfrak{t}$ consists of semi-simple elements, $\mathfrak{g}$ is the direct sum of $[\mathfrak{t},\mathfrak{g}]$ and the centralizer $\mathfrak{z}$ of $\mathfrak{t}$ (Chap. I, §3, no. 5, Prop. 6). Since $[\mathfrak{t},\mathfrak{g}]\subset \mathfrak{r},\mathfrak{g}=\mathfrak{z}+\mathfrak{r}$. Consequently, if $\mathfrak{s}$ is a Levi subalgebra of $\mathfrak{z}$ (Chap. I, §6, no. $8),\mathfrak{g}=\mathfrak{s}+\mathfrak{r}$, so $\mathfrak{s}$ is a Levi subalgebra of $\mathfrak{g}$. Put $\mathfrak{m}=\mathfrak{s}\oplus \mathfrak{t}$. Since $[\mathfrak{s},\mathfrak{t}] =\{0\},\mathfrak{m}$ is a Lie subalgebra of $\mathfrak{g}$, reductive in $\mathfrak{g}\mathfrak{l}(V)$ by Chap. I, §6, no. 5, Th. 4. Moreover,

$$
\mathfrak{g}=\mathfrak{s}\oplus \mathfrak{r}=\mathfrak{s}\oplus \mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{r}) =\mathfrak{s}\oplus \mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{g}) =\mathfrak{m}\oplus \mathfrak{n}_V(\mathfrak{g})
$$

since $\mathfrak{n}_V(\mathfrak{g}) =\mathfrak{n}_V(\mathfrak{r})$. Hence (i).

Now let $\mathfrak{m}'$ be a Lie subalgebra of $\mathfrak{g}$ complementary to $\mathfrak{n}_V(\mathfrak{g})$ and reductive in $\mathfrak{g}\mathfrak{l}(V)$. We show that $\mathfrak{m}'$ is conjugate to $\mathfrak{m}$ under Aut$_e(\mathfrak{g})$. We have $\mathfrak{m}'=\mathfrak{s}'\oplus \mathfrak{t}'$, where $\mathfrak{s}'= [\mathfrak{m}',\mathfrak{m}']$ is semi-simple and the centre $\mathfrak{t}'$ of $\mathfrak{m}'$ consists of semi-simple elements. Then $\mathfrak{r}=\mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{g}) =\mathfrak{t}'\oplus \mathfrak{n}_V(\mathfrak{g})$. In view of Cor. 2 of Prop. 6, we are reduced to the case $\mathfrak{t}=\mathfrak{t}'$. Then $\mathfrak{s}'\subset \mathfrak{z}$; since dim$\mathfrak{s}'=$ dim$\mathfrak{s}$, $\mathfrak{s}'$ is a Levi subalgebra of $\mathfrak{z}$. By Chap. I, §6, no. 8, Th. 5, there exists $x\in \mathfrak{n}_V(\mathfrak{z})$ such that $e^{adx}(\mathfrak{s}) =\mathfrak{s}'$; since $x$ commutes with $\mathfrak{t}$, we also have $e^{adx}(\mathfrak{t}) =\mathfrak{t}$.

### 4. LINEAR LIE ALGEBRAS OF NILPOTENT ENDOMORPHISMS

#### Lemma 1 {#lie-vii-s5-lem-1 .statement tag=00WZ}

Let $\mathfrak{n}$ be a Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ consisting of nilpotent endomorphisms, and N the subgroup exp$\mathfrak{n}$ of $\mathbf{G}\mathbf{L}(V) ($§3, no. 1, Lemma 1).

(i) Let $\rho$ be a finite dimensional linear representation of $\mathfrak{n}$ on W, such that the elements of $\rho (\mathfrak{n})$ are nilpotent, $W'$ a vector subspace of W stable under $\rho ,\rho_1$ and $\rho_2$ the subrepresentation and quotient representation of $\rho$ defined by $W',\pi , \pi_1, \pi_2$ the representations of N compatible with $\rho , \rho_1, \rho_2($§3, no. 1). Then $\pi_1, \pi_2$ are the subrepresentation and quotient representation of $\pi$ defined by $W'$.

(ii) Let $\rho_1, \rho_2$ be finite dimensional linear representations of $\mathfrak{n}$ such that the elements of $\rho_1(\mathfrak{n})$ and $\rho_2(\mathfrak{n})$ are nilpotent, and $\pi_1, \pi_2$ the representations of N compatible with $\rho_1, \rho_2$. Then $\pi_1\otimes \pi_2$ is the representation of N compatible with $\rho_1\otimes \rho_2$.

(iii) Let $\rho_1, \rho_2$ be finite dimensional linear representations of $\mathfrak{n}$ on vector spaces $V_1,V_2$, such that the elements of $\rho_1(\mathfrak{n})$ and $\rho_2(\mathfrak{n})$ are nilpotent, $\rho$ the representation of $\mathfrak{n}$ on Hom(V$_1,V_2)$ determined by $\rho_1, \rho_2$. Let $\pi_1, \pi_2$ be the representations of N compatible with $\rho_1, \rho_2$, and $\pi$ the representation of N on Hom(V$_1,V_2)$ determined by $\pi_1, \pi_2$. Then $\pi$ is the representation of N compatible with $\rho$.

Assertion (i) is clear. Let $\rho_1, \rho_2, \pi_1, \pi_2$ be as in (ii). If $x\in \mathfrak{n}$, we have, since $\rho_1(x)\otimes 1$ and $1\otimes \rho_2(x)$ commute,

exp($\rho_1(x)\otimes 1 + 1\otimes \rho_2(x)$) $=$ exp($\rho_1(x)\otimes 1$). exp(1 $\otimes \rho_2(x))$

= (exp $\rho_1(x))\otimes 1.1\otimes$ (exp$\rho_2(x))$

= (exp $\rho_1(x))\otimes$ (exp$\rho_2(x))$

$=\pi_1$(exp $x)\otimes \pi_2$(exp $x)$

$= (\pi_1\otimes \pi_2$)(exp $x)$,

hence (ii). Let $\rho_1, \rho_2, \rho , \pi_1, \pi_2, \pi ,V_1,V_2$ be as in (iii). If $v_1\in$ EndV$_1$ and $v_2\in$ EndV$_2$, denote by $R_{v_1}$ and $L_{v_2}$ the maps $u \rightarrow uv_1$ and $u \rightarrow v_2u$ from Hom(V$_1,V_2)$ to itself; these maps commute and $\rho (x)u= (L_{\rho_2(x)}-R_{\rho_1(x)})u$, so

exp$\rho (x).u=$ exp $L_{\rho_2(x)}$. exp $R_{-\rho_1(x)}.u$

$$
= L_{exp\rho_2(x)}.R_{exp(-\rho_1(x))}.u
$$

$$
= L_{\pi_2(expx)}.R_{\pi_1(exp(-x))}.u
$$

$=\pi$(exp $x).u$,

hence (iii).

#### Lemma 2 {#lie-vii-s5-lem-2 .statement tag=01JS}

$^2$ (i) Let W be a vector subspace of V of dimension $d$, D the line $\bigwedge^dW\subset \bigwedge^dV,\theta$ the canonical representation of $\mathfrak{g}\mathfrak{l}(V)$ on $\bigwedge V$ (Chap. III, App.). Let $x\in \mathfrak{g}\mathfrak{l}(V)$. Then $x(W)\subset W$ if and only if $\theta (x)(D)\subset D$.

(ii) Let $(e_1, . . . , e_n)$ be the canonical basis of $k^n,\theta$ the canonical representation of $\mathfrak{g}\mathfrak{l}(n, k)$ on $\bigwedge(k^n)$, and $x\in \mathfrak{g}\mathfrak{l}(n, k)$. Then $x\in \mathfrak{n}(n, k)$ if and only if

$$
\theta (x)(e_{n-d+1}\wedge  \cdots  \wedge e_n) = 0
$$

for $1\leq d\leq n$.

(i) If $x(W)\subset W$, it is clear that $\theta (x)D\subset D$. Conversely, assume that $\theta (x)D\subset D$. Let $u$ be a non-zero element of D and let $y\in W$. Then $y\wedge u= 0$. Since $\theta (x)$ is a derivation of $\bigwedge V$, this implies

$$
\theta (x)y\wedge u+y\wedge \theta (x)u= 0
$$

Now $\theta (x)u\in ku$, so $y\wedge \theta (x)u= 0$ and consequently $\theta (x)y\wedge u= 0$. By Algebra, Chap. III, §7, no. 9, Prop. 13, this implies that $\theta (x)y\in W$, i.e. $x(y)\in W$, which proves that $x(W)\subset W$.

(ii) The condition stated in (ii) is clearly necessary for $x\in \mathfrak{n}(n, k)$. Assume that it is satisfied. By (i), $x$ leaves

$^2$ In this lemma, $k$ can be an arbitrary (commutative) field.

$$
ke_{n-d+1}+\cdots +ke_n
$$

stable, and since this holds for $d= 1, . . . , n,x$ is lower triangular. Put

$$
x= (x_{ij})_{1\leq i,j\leq n}
$$

We have $0 =x(e_n) =x_{nn}e_n$, so $x_{nn}= 0$. Let $i < n$, and assume that we have proved that $x_{jj}= 0$ for $j > i$. Then

$$
0 =\theta (x)(e_i\wedge e_{i+1}\wedge  \cdots  \wedge e_n) =x_{ii}(e_i\wedge e_{i+1}\wedge  \cdots  \wedge e_n)
$$

so $x_{ii}= 0$. Thus, $x\in \mathfrak{n}(n, k)$.

#### Proposition 8 {#lie-vii-s5-prop-8 .statement tag=00X0}

Let $\mathfrak{n}$ be a Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ consisting of nilpotent elements, $\mathfrak{q}$ the normalizer of $\mathfrak{n}$ in $\mathfrak{g}\mathfrak{l}(V)$. There exists a finite dimensional vector space E, a representation $\rho$ of $\mathfrak{g}\mathfrak{l}(V)$ on E, and a vector subspace F of E, satisfying the following conditions:

(i) the image under $\rho$ of a homothety of V is diagonalizable;

(ii) F is stable under $\rho (\mathfrak{q})$;

(iii) $\mathfrak{n}$ is the set of $x\in \mathfrak{g}\mathfrak{l}(V)$ such that $\rho (x)(F) = 0$.

Let $n=$ dim V. By Engel’s theorem, V can be identified with $k^n$ in such a way that $\mathfrak{n}\subset \mathfrak{n}(n, k)$. Let P be the algebra of polynomial functions on $\mathfrak{g}\mathfrak{l}(n, k)$. For $i= 0,1, . .$., let $P_i$ be the set of elements of P homogeneous of degree $i$. Let N = exp $\mathfrak{n}$, which is a subgroup of the strictly lower triangular group T. Let J be the set of elements of P that are zero on N; this is an ideal in P. Let $N_J$ be the set of $x\in \mathfrak{g}\mathfrak{l}(n, k)$ such that $p(x) = 0$ for all $p\in J$. Then $N\subset N_J$. Conversely, let $x\in N_J$. Denote by $p_{ij}$ the polynomial functions giving the entries of an element of $\mathfrak{g}\mathfrak{l}(n, k)$. The ideal J contains the $p_{ij}$ (for $i < j)$ and the $p_{ii}-1$; hence $x\in T$. On the other hand, if $u$ is a linear form on $\mathfrak{g}\mathfrak{l}(n, k)$ which is zero on $\mathfrak{n}$, there exists $p_u\in P$ such that $p_u(z) =u$(log $z)$ for all $z\in T ($§3, no. 1, Lemma 1 (i)); we have $p_u\in J$, so $u$(log $x) = 0$. It follows that log $x$ belongs to $\mathfrak{n}$, so $x\in N$, proving that $N = N_J$.

For all $p\in P$ and $g\in \mathbf{G}\mathbf{L}_n(k)$, let $\lambda (g)p$ be the function $x \rightarrow p(g^{-1}x)$ on $\mathfrak{g}\mathfrak{l}(n, k)$; then $\lambda (g)p\in P,\lambda (g)$ is an automorphism of the algebra P, and $\lambda$ is a representation of $\mathbf{G}\mathbf{L}_n(k)$ on P which leaves each $P_i$ stable. We show that

$$
N =\{x\in \mathbf{G}\mathbf{L}_n(k)|\lambda (x)J = J\} \tag{1}
$$

If $x\in N, p\in J, y\in N$, then $(\lambda (x)p)(y) =p(x^{-1}y) = 0$ since $x^{-1}y\in N$; thus $\lambda (x)p\in J$, so $\lambda (x)J = J$. Let $x\in \mathbf{G}\mathbf{L}_n(k)$ be such that $\lambda (x)J = J$; let $p\in J$; then $p(x^{-1}) = (\lambda (x)p)(e) = 0$, so $x^{-1}\in N_J= N$ and $x\in N$. This proves (i).

The ideal J is of finite type (Commutative Algebra, Chap. III, §2, no. 10, Cor. 2 of Th. 2). Hence, there exists an integer $q$ such that, if $W = P_0+ P_1+\cdots + P_q$, then $J\cap W$ generates J as an ideal. Denote by $\lambda_j$ (resp. $\lambda ')$ the subrepresentation of $\lambda$ defined by $P_J$ (resp. by W). By (1),

$$
N =\{x\in \mathbf{G}\mathbf{L}_n(k)|\lambda '(x)(J\cap W) = J\cap W\} \tag{2}
$$

We show that, for all $j$, there exists a representation $\sigma_j$ of the Lie algebra $\mathfrak{g}\mathfrak{l}(n, k)$ on $P_j$ such that:

$\sigma_j|\mathfrak{n}(n, k)$ is compatible (§$3$, no$.1)$ with $\lambda_j|T$. (3)

For all $x\in k.1_n, \sigma_j(x)$ is a homothety. (4)

Since $\lambda_j$ is the $j$th symmetric power of $\lambda_1$, it suffices to prove the existence of $\sigma_1$, cf. Lemma 1. Now $\lambda_1$ is the contragredient representation of the representation $\gamma$ of $\mathbf{G}\mathbf{L}_n(k)$ on $\mathfrak{g}\mathfrak{l}(n, k)$ given by

$$
\gamma (x)y=xy, x\in \mathbf{G}\mathbf{L}_n(k), y\in \mathfrak{g}\mathfrak{l}(n, k)
$$

Let $c$ be the representation of the Lie algebra $\mathfrak{g}\mathfrak{l}(n, k)$ on $\mathfrak{g}\mathfrak{l}(n, k)$ given by

$$
c(x)y=xy, x, y\in \mathfrak{g}\mathfrak{l}(n, k)
$$

It is immediate that $c|\mathfrak{n}(n, k)$ and $\gamma |T$ are compatible, and that $c(x)$ is a homothety for all $x\in k.1_n$. Thus, it suffices to take for $\sigma_1$ the dual representation of $c$ (Chap. I, §3, no. 3).

Now let $\sigma '$ be the representation of $\mathfrak{g}\mathfrak{l}(n, k)$ on W given by the direct sum of the $\sigma_j, 0\leq j\leq q$. In view of (2) and the relations

$\lambda '$(exp($x$)) $=$ exp($\sigma '(x)$) and $\sigma '$(log($y$)) $=$ log($\lambda '(y)$)$, x\in \mathfrak{n}(n, k), y\in T$,

we have

$$
\mathfrak{n}=\{x\in \mathfrak{n}(n, k)|\sigma '(x)(J\cap W)\subset J\cap W\} \tag{5}
$$

Let $d=$ dim(J $\cap W)$, and let $\tau =\bigwedge^d\sigma '$. Let $D =\bigwedge^d(J\cap W)$. By (5) and Lemma 2 (i),

$$
\mathfrak{n}=\{x\in \mathfrak{n}(n, k)|\tau (x)(D)\subset D\} \tag{6}
$$

But $\tau (\mathfrak{n}(n, k))$ consists of nilpotent endomorphisms, so (6) can also be written

$$
\mathfrak{n}=\{x\in \mathfrak{n}(n, k)|\tau (x)(D) = 0\} \tag{7}
$$

Now let $E =\bigwedge^dW\oplus \bigwedge^1V\oplus \bigwedge^2V\oplus  \cdots  \oplus \bigwedge^nV$; let $\rho$ be the direct sum of $\tau$ and the canonical representations of $\mathfrak{g}\mathfrak{l}(n, k)$ on $\bigwedge^1V, . . . ,\bigwedge^nV$. Let $E_0\subset E$ be the sum of $D =\bigwedge^d(J\cap W)$ and the lines generated by $e_{n-j+1}\wedge  \cdots  \wedge e_n$ for $j= 1, . . . , n$. By (7) and Lemma 2 (ii),

$$
\mathfrak{n}=\{x\in \mathfrak{g}\mathfrak{l}(V)|\rho (x)(E_0) = 0\} \tag{8}
$$

It is immediate that, if $x\in k.1_n,\rho (x)$ is diagonalizable. Finally, if F is the set of elements of E annihilated by $\rho (\mathfrak{n}), F$ is stable under $\rho (\mathfrak{q})$ (Chap. I, §3, no. 5, Prop. 5), and by (8),

$$
\mathfrak{n}=\{x\in \mathfrak{g}\mathfrak{l}(V)|\rho (x)(F) = 0\} \tag{9}
$$

### 5. CHARACTERIZATIONS OF DECOMPOSABLE LIE ALGEBRAS

Every decomposable Lie algebra is generated as a vector space (and a fortiori as a Lie algebra) by the set of its elements that are either semi-simple or nilpotent. Conversely:

#### Theorem 1 {#lie-vii-s5-thm-1 .statement tag=00X1}

Let $\mathfrak{g}$ be a Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ and let X be a subset of $\mathfrak{g}$ generating $\mathfrak{g}$ as a Lie algebra over $k$. If every element of X is either semi-simple or nilpotent, $\mathfrak{g}$ is decomposable.

a$)\mathfrak{g}$ is commutative.

The semi-simple (resp. nilpotent) elements of $\mathfrak{g}$ form a vector subspace $\mathfrak{g}_s$ (resp. $\mathfrak{g}_n)$. The assumption is equivalent to $\mathfrak{g}=\mathfrak{g}_s\oplus \mathfrak{g}_n$, hence the fact that $\mathfrak{g}$ is decomposable.

b$)\mathfrak{g}$ is reductive.

Then $\mathfrak{g}=\mathfrak{g}'\times \mathfrak{c}$ with $\mathfrak{g}'$ semi-simple and $\mathfrak{c}$ commutative. By Prop. $2,\mathfrak{g}'$ is decomposable. Let $x=a+b\in \mathfrak{g}$ with $a\in \mathfrak{g}',b\in \mathfrak{c}$. Let $a_s, a_n, b_s, b_n$ be the semi-simple and nilpotent components of $a, b$. Since $a_s, a_n, b_s, b_n$ mutually commute, the semi-simple and nilpotent components of $x$ are $a_s+b_s, a_n+b_n$. Now $a_s, a_n\in \mathfrak{g}'$. If $x$ is semi-simple, $x=a_s+b_s$; since $a_s\in \mathfrak{g}'$, we have $b_s\in \mathfrak{g}$, so $b_s\in \mathfrak{c}$ since $b_s$ commutes with $\mathfrak{g}$; consequently, $a=a_s$ and $b=b_s$. Similarly, if $x$ is nilpotent, $a=a_n$ and $b=b_n$. It follows that the projections on $\mathfrak{c}$ of the elements of X are either semi-simple or nilpotent; by $a)$, this implies that $\mathfrak{c}$ is decomposable. Retaining the preceding notation, but without the assumption on $x$, we now have $b_s, b_n\in \mathfrak{c}$, so $a_s+b_s, a_n+b_n\in \mathfrak{g}$, which proves the theorem in this case.

c) General case.

We assume that the theorem is proved for Lie algebras of dimension $<$ dim $\mathfrak{g}$ and prove it for $\mathfrak{g}$.

Let $\mathfrak{n}$ be the largest ideal of nilpotency of the identity representation of $\mathfrak{g}$. If $\mathfrak{n}= 0,\mathfrak{g}$ has an injective semi-simple representation, and so is reductive. Assume that $\mathfrak{n}\not= 0$. Let $\mathfrak{p}$ be the normalizer of $\mathfrak{n}$ in $\mathfrak{g}\mathfrak{l}(V)$. There exist $E, \rho ,F$ satisfying the conditions of Prop. 8. Since $\mathfrak{g}\subset \mathfrak{p},\rho (\mathfrak{g})$ leaves F stable; let $\rho_0$ be the representation $u \rightarrow \rho (u)|F$ of $\mathfrak{g}$ on F; we have $\mathfrak{n}=$ Ker$\rho_0$. The image under $\rho$ of every semi-simple (resp. nilpotent) element of $\mathfrak{g}\mathfrak{l}(V)$ is semi-simple (resp. nilpotent) (Prop. 2). The algebra $\rho_0(\mathfrak{g})$ is thus generated by its semi-simple elements and its nilpotent elements. By the induction hypothesis, $\rho_0(\mathfrak{g})$ is decomposable.

Let $x\in \mathfrak{g}$, and let $x_s, x_n$ be its semi-simple and nilpotent components. By Prop. 2, the semi-simple and nilpotent components of $\rho (x)$ are $\rho (x_s), \rho (x_n)$. Since $\rho_0(\mathfrak{g})$ is decomposable, there exist $y, z\in \mathfrak{g}$ such that

$$
\rho_0(y) =\rho (x_s)|F, \rho_0(z) =\rho (x_n)|F
$$

Then $x_s\in y+\mathfrak{n}, x_n\in z+\mathfrak{n}$, so $x_s, x_n\in \mathfrak{g}$. Q.E.D.

#### Corollary 1 {#lie-vii-s5-thm-1-cor-1 .statement tag=00X2}

Every subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ generated by its decomposable subalgebras is decomposable.

This is clear.

#### Corollary 2 {#lie-vii-s5-thm-1-cor-2 .statement tag=00X3}

Let $\mathfrak{g}$ be a Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$. Then $[\mathfrak{g},\mathfrak{g}]$ is decomposable.

Let $\mathfrak{r}$ be the radical of $\mathfrak{g},\mathfrak{s}$ a Levi subalgebra of $\mathfrak{g}$ (Chap. I, §6, no. 8). Then

$$
[\mathfrak{g},\mathfrak{g}] = [\mathfrak{s},\mathfrak{s}] + [\mathfrak{s},\mathfrak{r}] + [\mathfrak{r},\mathfrak{r}] =\mathfrak{s}+ [\mathfrak{g},\mathfrak{r}]
$$

The algebra $[\mathfrak{g},\mathfrak{r}]$ is decomposable since all of its elements are nilpotent (Chap. I, §5, no. 3). On the other hand, $\mathfrak{s}$ is decomposable (Prop. 2). It follows that $[\mathfrak{g},\mathfrak{g}]$ is decomposable (Cor. 1).

#### Corollary 3 {#lie-vii-s5-thm-1-cor-3 .statement tag=00X4}

Let $\mathfrak{g}$ be a Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$, and let X be a subset of $\mathfrak{g}$ generating $\mathfrak{g}($as a Lie algebra over $k)$.

(i) The decomposable envelope $e(\mathfrak{g})$ of $\mathfrak{g}$ is generated by the semi-simple and nilpotent components of the elements of X.

(ii) If $k'$ is an extension of $k,e(\mathfrak{g}\otimes_kk') =e(\mathfrak{g})\otimes_kk'$; and $\mathfrak{g}$ is decomposable if and only if $\mathfrak{g}\otimes_kk'$ is decomposable.

Let $\widetilde{\mathfrak{g}}$ be the subalgebra of $\mathfrak{g}\mathfrak{l}(V)$ generated by the semi-simple and nilpotent components of the elements of X. Then $\mathfrak{g}\subset \widetilde{\mathfrak{g}}\subset e(\mathfrak{g})$; by Th. $1, \widetilde{\mathfrak{g}}$ is decomposable, so $\widetilde{\mathfrak{g}}=e(\mathfrak{g})$, which proves (i). Assertion (ii) follows, since X generates the $k'$-algebra $\mathfrak{g}\otimes_kk'$.

#### Corollary 4 {#lie-vii-s5-thm-1-cor-4 .statement tag=00X5}

Let $\mathfrak{g}$ be a decomposable Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$. Let $\mathscr{T}$ be the set of commutative subalgebras of $\mathfrak{g}$ consisting of semi-simple elements (cf. Prop. 6). The maximal elements of $\mathscr{T}$ all have the same dimension.

Let $k'$ be an algebraically closed extension of $k$ and $V'= V\otimes_kk',\mathfrak{g}'=$ $\mathfrak{g}\otimes_kk'$. Let $\mathfrak{t}_1,\mathfrak{t}_2$ be maximal elements of $\mathscr{T},\mathfrak{t}'_i=\mathfrak{t}_i\otimes_kk',\mathfrak{h}_i$ the commutant of $\mathfrak{t}_i$ in $\mathfrak{g},\mathfrak{h}'_i=\mathfrak{h}_i\otimes_kk'$. Then $\mathfrak{h}_i$ is a Cartan subalgebra of $\mathfrak{g}$ (Prop. 6) so $\mathfrak{h}'_i$ is a Cartan subalgebra of $\mathfrak{g}'$. Then $\mathfrak{h}_i=\mathfrak{t}_i\times \mathfrak{n}_V(\mathfrak{h}_i)$, hence $\mathfrak{h}'_i=\mathfrak{t}'_i\times \mathfrak{n}_{V'}(\mathfrak{h}'_i)$, so that $\mathfrak{t}'_i$ is the set of semi-simple elements of $\mathfrak{h}'_i$. Since $\mathfrak{g}'$ is decomposable (Cor. $3),\mathfrak{t}'_1$ and $\mathfrak{t}'_2$ are conjugate under Aut$_e(\mathfrak{g}')$ (Prop. 6), so dim$\mathfrak{t}_1=$ dim$\mathfrak{t}_2$.

#### Theorem 2 {#lie-vii-s5-thm-2 .statement tag=00X6}

Let $\mathfrak{g}$ be a Lie subalgebra of $\mathfrak{g}\mathfrak{l}(V)$. The following conditions are equivalent:

(i) $\mathfrak{g}$ is decomposable;

(ii) every Cartan subalgebra of $\mathfrak{g}$ is decomposable;

(iii) $\mathfrak{g}$ has a decomposable Cartan subalgebra;

(iv) the radical of $\mathfrak{g}$ is decomposable.

(i) $=\Rightarrow$ (ii): This follows from Cor. 2 of Prop. 3.

(ii) $=\Rightarrow$ (i): This follows from Cor. 1 of Th. 1, since $\mathfrak{g}$ is generated by its Cartan subalgebras (§2, no. 3, Cor. 3 of Th. 1).

(ii) $=\Rightarrow$ (iii): This is clear.

(iii) $=\Rightarrow$ (ii): By Cor. 3 of Th. 1, we can assume that $k$ is algebraically closed. The Cartan subalgebras of $\mathfrak{g}$ are then conjugate under the elementary automorphisms of $\mathfrak{g}($§3, no. 2, Th. 1); in view of Remark 1 of §3, no. 1, it follows that, if one of these is decomposable, they all are.

(i) $=\Rightarrow$ (iv): This follows from Cor. 2 of Prop. 4.

(iv) $=\Rightarrow$ (i): Assume that the radical $\mathfrak{r}$ of $\mathfrak{g}$ is decomposable. Let $\mathfrak{s}$ be a Levi subalgebra of $\mathfrak{g}$; it is decomposable (Prop. 2). Hence $\mathfrak{g}=\mathfrak{s}+\mathfrak{r}$ is decomposable (Cor. 1 of Th. 1).

### Exercises {#lie-vii-s5-exercises}

See the [exercises for § 5](exercises/s5/).
