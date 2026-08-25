---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 4
section_title: Nilpotent Lie algebras
lang: en
source: lie-i-iii
pdf_pages: 0056-0060, 0109-0116
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF NILPOTENT LIE ALGEBRAS
      page: 0
      pdf_page: 56
    - "no": 2
      title: ENGEL'S THEOREM
      page: 0
      pdf_page: 57
    - "no": 3
      title: THE LARGEST NILPOTENCY IDEAL OF A REPRESENTATION
      page: 0
      pdf_page: 58
    - "no": 4
      title: THE LARGEST NILPOTENT IDEAL OF A LIE ALGEBRA
      page: 0
      pdf_page: 60
    - "no": 5
      title: EXTENSION OF THE BASE FIELD
      page: 0
      pdf_page: 60
statements: 18
exercises: 27
content_sha256: ec8fcfdc0c4ee25ad5c1b29d58376b1ebcb9cbf681ca6ed53a7f8804eb1ab7e6
---

## § 4. NILPOTENT LIE ALGEBRAS

*Recall that henceforth $K$ denotes a commutative field. In the rest of the chapter the Lie algebras are assumed to be finite-dimensional over $K$.*

### 1. DEFINITION OF NILPOTENT LIE ALGEBRAS

#### Definition 1 {#lie-i-s4-def-1 .statement}

*A Lie algebra $g$ is called nilpotent if there exists a decreasing finite sequence of ideals $(g_i)_{1 \leq i \leq p}$ of $g$ with $g_0 = g, g_p = \{0\}$, such that* $[g, g_i] \subset g_{i+1}$ *for* $0 \leq i < p$.

A commutative Lie algebra is nilpotent.

#### Proposition 1 {#lie-i-s4-prop-1 .statement}

*Let $g$ be a Lie algebra. The following conditions are equivalent:*
(a) $g$ *is nilpotent;*
(b) $\mathcal{C}^k g = \{0\}$ *for sufficiently large* $k$;
(c) $\mathcal{C}_k g = g$ *for sufficiently large* $k$;
(d) *there exists an integer* $k$ *such that* $\operatorname{ad} x_1 \circ \operatorname{ad} x_2 \circ \cdots \circ \operatorname{ad} x_k = 0$ *for all elements* $x_1, x_2, \ldots, x_k$ *in* $g$;
(e) *there exists a decreasing sequence of ideals* $(g_i)_{0 \leq i \leq n}$ *of* $g$ *with* $g_0 = g, g_n = \{0\}$, *such that* $[g, g_i] \subset g_{i+1}$ *and* $\dim g_i / g_{i+1} = 1$ *for* $0 \leq i < n$.

If $\mathcal{C}^k g = \{0\}$ (resp. $\mathcal{C}_k g = g$), clearly the sequence $\mathcal{C}^1 g, \ldots, \mathcal{C}^k g$ (resp. $\mathcal{C}_k g, \mathcal{C}_{k-1} g, \ldots, \mathcal{C}_0 g$) has the properties of Definition 1 and hence $g$ is nilpotent. Conversely, suppose that there exists a sequence $(g_i)_{0 \leq i \leq p}$ with the properties of Definition 1. It is seen by induction on $n$ that $g_i \supset \mathcal{C}^{i+1} g$ and $g_{p-i} \subset \mathcal{C}_i g$. Hence $\mathcal{C}^{p+1} g = \{0\}$ and $\mathcal{C}_p g = g$. We have thus proved that conditions (a), (b) and (c) are equivalent. On the other hand, $\mathcal{C}^1 g$ is the set of linear combinations of elements of the form

$$
[x_1, [x_2, \ldots, [x_{i-2}, [x_{i-1}, x_i]] \ldots]]
$$

where $x_1, x_2, \ldots, x_i$ run through $g$. Hence conditions (b) and (d) are equivalent. Finally, if there exists a sequence $(g_i)_{0 \leq i \leq p}$ of ideals with the properties of

Definition 1, there exists a decreasing sequence $(\mathfrak{h}_i)_{0 \leq i \leq n}$ of vector subspaces of $g$ of dimensions $n, n-1, n-2, \ldots, 0$ and a sequence of indices
$$
i_0 < i_1 < \cdots < i_p
$$
with $g_0 = \mathfrak{h}_{i_0}, g_1 = \mathfrak{h}_{i_1}, \ldots, g_p = \mathfrak{h}_{i_p}$; then as $[g, \mathfrak{h}_{i_k}] \subset \mathfrak{h}_{i_{k+1}}$ the $\mathfrak{h}_i$ are ideals and $[g, \mathfrak{h}_i] \subset \mathfrak{h}_{i+1}$ for all $i$. Hence conditions (a) and (e) are equivalent.

#### Corollary 1 {#lie-i-s4-prop-1-cor-1 .statement}

*The centre of a non-zero nilpotent Lie algebra is non-zero.*

#### Corollary 2 {#lie-i-s4-prop-1-cor-2 .statement}

*The Killing form of a nilpotent Lie algebra is zero.*
For all $x$ and $y$ in a nilpotent Lie algebra $\operatorname{ad} x \circ \operatorname{ad} y$ is nilpotent and hence of zero trace.

#### Proposition 2 {#lie-i-s4-prop-2 .statement}

*Subalgebras, quotient algebras and central extensions of a nilpotent Lie algebra are nilpotent. A finite product of nilpotent Lie algebras is a nilpotent Lie algebra.*
Let $g$ be a Lie algebra, $g'$ a subalgebra of $g$, $\mathfrak{h}$ an ideal of $g$, $\mathfrak{k} = g/\mathfrak{h}$ and $\phi$ the canonical mapping of $g$ onto $\mathfrak{k}$. If $g$ is nilpotent, then $\mathcal{C}^k g = \{0\}$ for some integer $k$, hence $\mathcal{C}^k g' \subset \mathcal{C}^k g = \{0\}$ and $\mathcal{C}^k \mathfrak{k} = \phi(\mathcal{C}^k g) = \{0\}$ and hence $g'$ and $\mathfrak{k}$ are nilpotent. If $\mathfrak{k}$ is nilpotent and $\mathfrak{h}$ is contained in the centre of $g$, then $\mathcal{C}^k \mathfrak{k} = \{0\}$ for some integer $k$, hence $\mathcal{C}^k g \subset \mathfrak{h}$ and therefore $\mathcal{C}^{k+1} g \subset [\mathfrak{h}, g] = \{0\}$, so that $g$ is nilpotent. Finally, the assertion concerning products follows for example from the assertion (a) $\Leftrightarrow$ (d) of Proposition 1.

Definition 1 and Proposition 2 show that nilpotent Lie algebras are precisely the algebras obtained from commutative Lie algebras by a sequence of central extensions.

#### Proposition 3 {#lie-i-s4-prop-3 .statement}

*Let $g$ be a nilpotent Lie algebra and $\mathfrak{h}$ a subalgebra of $g$ distinct from $g$. The normalizer of $\mathfrak{h}$ in $g$ is distinct from $\mathfrak{h}$.*
Let $k$ be the greatest integer such that $\mathcal{C}^k g + \mathfrak{h} \neq \mathfrak{h}$. Then
$$
[\mathcal{C}^k g + \mathfrak{h}, \mathfrak{h}] \subset \mathcal{C}^{k+1} g + \mathfrak{h} \subset \mathfrak{h}
$$
and hence the normalizer of $\mathfrak{h}$ in $g$ contains $\mathcal{C}^k g + \mathfrak{h}$.

### 2. ENGEL'S THEOREM

#### Lemma 1 {#lie-i-s4-lem-1 .statement}

*Let $V$ be a vector space over $\mathbf{K}$. If $x$ is a nilpotent endomorphism of $V$, the mapping $y \mapsto [x, y]$ of $\mathcal{L}(V)$ into $\mathcal{L}(V)$ is nilpotent.*
If $f$ denotes this mapping, $f^m(y)$ is a sum of terms of the form $\pm x^i y x^j$ with $i + j = m$. If $x^k = 0$, then $f^{2k-1}(y) = 0$ for all $y$.

#### Theorem 1 (Engel) {#lie-i-s4-thm-1 .statement}

*Let $V$ be a vector space over $\mathbf{K}$ and $g$ a finite-dimensional subalgebra of $\mathfrak{gl}(V)$ whose elements are nilpotent endomorphisms of $V$. If $V \neq \{0\}$, there exists $u \neq 0$ in $V$ such that $x.u = 0$ for all $x \in g$.*

The proof proceeds by induction on the dimension $n$ of $g$. The theorem is obvious if $n = 0$. Suppose that it is true for algebras of dimension $< n$.

Let $h$ be a Lie subalgebra of $g$ of dimension $m < n$. If $x \in h$, and $\mathrm{ad}_g x$ maps $h$ into itself and defines on passing to the quotient an endomorphism $\sigma(x)$ of the space $g/h$. By Lemma 1 $\mathrm{ad}_g x$ is nilpotent and hence $\sigma(x)$ is nilpotent. By the induction hypothesis there exists a non-zero element of $g/h$ which is annihilated by all the $\sigma(x),\ x \in h$. It follows that $h$ is an ideal in a certain $(m+1)$-dimensional subalgebra of $g$.

We conclude (by iteration starting with $h = \{0\}$) that $g$ has an ideal $h$ of dimension $n-1$. Let $a \in g,\ a \notin h$. We again use the induction hypothesis: the $u \in V$ such that $x.u = 0$ for all $x \in h$ form a non-zero vector subspace U of V. This subspace is stable under $a$ (\S 3, no. 5, Proposition 5). Since $a$ is a nilpotent endomorphism of V, there exists a non-zero element of U which is annihilated by $a$ and hence by every element of $g$.

#### Corollary 1 {#lie-i-s4-thm-1-cor-1 .statement}

*For a Lie algebra g to be nilpotent, it is necessary and sufficient that, for all $x \in g$, $\mathrm{ad}\ x$ be nilpotent.*

The condition is necessary (Proposition 1). Suppose that its sufficiency has been proved for Lie algebras of dimension $< n$ ($n \neq 0$). Let $g$ be an $n$-dimensional Lie algebra such that, for all $x \in g$, $\mathrm{ad}\ x$ is nilpotent. Theorem 1, applied to the set of $\mathrm{ad}\ x\ (x \in g)$, proves that the centre $c$ of $g$ is non-zero. Then $g$ is a central extension of the Lie algebra $g/c$, which is nilpotent by our induction hypothesis. The proof is completed by applying Proposition 2.

#### Corollary 2 {#lie-i-s4-thm-1-cor-2 .statement}

*Let g be a Lie algebra and h an ideal of g. Suppose that $g/h$ is nilpotent and that, for all $x \in g$, the restriction of $\mathrm{ad}\ x$ to h is nilpotent. Then g is nilpotent.*

Let $x \in g$. As $g/h$ is nilpotent, there exists an integer $k$ such that $(\mathrm{ad}\ x)^k(g) \subset h$. By hypothesis there exists an integer $k'$ such that $(\mathrm{ad}\ x)^{k'}(h) = \{0\}$. Hence $(\mathrm{ad}\ x)^{k+k'}(g) = \{0\}$. Corollary 2 is hence a consequence of Corollary 1.

#### Corollary 3 {#lie-i-s4-thm-1-cor-3 .statement}

*Let V be a vector space and g a finite-dimensional subalgebra of $\mathfrak{gl}(V)$ whose elements are nilpotent endomorphisms of V. Then g is a nilpotent Lie algebra.*

This follows immediately from Lemma 1 and Corollary 1.

#### Example {#lie-i-s4-n2-exa-1 .statement}

The algebra $\mathfrak{n}(n, K)$ (\S 1, no. 2, Example 2 (3)) is nilpotent.

### 3. THE LARGEST NILPOTENCY IDEAL OF A REPRESENTATION

#### Lemma 2 {#lie-i-s4-lem-2 .statement}

*Let g be a Lie algebra, a an ideal of g and M a simple g-module. If, for all $x \in a,\ x_M$ is nilpotent, then $x_M = 0$ for all $x \in a$.*

Let N be the subspace of M consisting of the $m \in M$ such that $x_M.m = 0$ for all $x \in a$. By Theorem 1, $N \neq \{0\}$. On the other hand, for all $y \in g$, N is stable under $y_M$ (\S 3, no. 5, Proposition 5). Hence $N = M$, which proves the lemma.

#### Lemma 3 {#lie-i-s4-lem-3 .statement}

*Let g be a Lie algebra, a an ideal of g, M a g-module of finite dimension over*

K and $(M_i)_{0 \leq i \leq n}$ a Jordan-Hölder series of the $g$-module $M$. The following conditions are equivalent:

(a) for all $x \in a$, $x_M$ is nilpotent;
(b) for all $x \in a$, $x_M$ is in the Jacobson radical of the associative algebra $A$ generated by 1 and the $y_M$ where $y \in g$;
(c) for all $x \in a$,
$$
x_M(M_0) \subset M_1, x_M(M_1) \subset M_2, \ldots, x_M(M_{n-1}) \subset M_n.
$$

If these conditions are fulfilled, $a$ is orthogonal to $g$ with respect to the bilinear form associated with the $g$-module $M$.

(b) $\Rightarrow$ (a): as $A$ is finite-dimensional over $K$, the Jacobson radical of $A$ is a nilpotent ideal (*Algebra*, Chapter VIII, § 6, no. 4, Theorem 3) and hence every element of this radical is nilpotent.

(a) $\Rightarrow$ (c): each $Q_i = M_i/M_{i+1}$ ($0 \leq i < n$) is a simple $g$-module. For all $x \in a$, the endomorphism $x_{Q_i}$ (which is derived from $x_M$ by restricting to $M_i$ and passing to the quotient) is nilpotent if condition (a) holds and hence zero by Lemma 2; in other words, $x_M(M_i) \subset M_{i+1}$.

(c) $\Rightarrow$ (b): suppose condition (c) holds; let $x \in a$ and $z \in A$. Then $z(M_i) \subset M_i$ ($0 \leq i < n$) and hence $(zx_M)^n(M) = \{0\}$; thus $Ax_M$ is a left nilideal of $A$ and hence is contained in the Jacobson radical of $A$ (*Algebra*, Chapter VIII, § 6, no. 3, Corollary 3 to Theorem 1).

Finally, suppose conditions (a), (b) and (c) hold. Let $x \in a$ and $y \in g$. We have just seen that $y_M x_M$ is nilpotent and hence $\operatorname{Tr}(y_M x_M) = 0$, which proves the last assertion of the lemma.

#### Proposition 4 {#lie-i-s4-prop-4 .statement}

Let $g$ be a Lie algebra, $M$ a $g$-module of finite dimension over $K$ and $A$ the associative algebra generated by 1 and the set of $x_M$ ($x \in g$).

(a) The ideals $a$ of $g$ such that $x_M$ is nilpotent for all $x \in a$ are all contained in one of them, $n$.

(b) The ideal $n$ is the set of $x \in g$ such that $x_M$ belongs to the Jacobson radical of $A$.

(c) Let $(M_i)_{0 \leq i \leq n}$ be a Jordan-Hölder series of the $g$-module $M$; then $n$ is also the set of $x \in g$ such that $(x)_{M_i/M_{i+1}} = 0$ for all $i$.

(d) $n$ is orthogonal to $g$ with respect to the bilinear form associated with $\varphi$.

The set of $x \in g$ such that $x_M$ belongs to the Jacobson radical of $A$ is obviously an ideal of $g$. The proposition then follows immediately from Lemma 3.

#### Definition 2 {#lie-i-s4-def-2 .statement}

The ideal $n$ of Proposition 4 is called the largest nilpotency ideal for the $g$-module $M$ or the largest nilpotency ideal of the corresponding representation.

Clearly $n$ contains the kernel of this representation. It equals it when $M$ is semi-simple (Proposition 4 (c)), but not in general. It should be noted that an element of $x$ of $g$ such that $x_M$ is nilpotent does not necessarily belong to $n$.

We also note that a particular case of Lemma 3 immediately gives the following result:

#### Proposition 5 {#lie-i-s4-prop-5 .statement}

Let $V$ be a vector space of finite dimension $n$ over $K$ and $g$ a Lie sub-algebra of $gl(V)$ whose elements are nilpotent endomorphisms of $V$. Then there exists a decreasing sequence of vector subspaces $V_0, V_1, \ldots, V_n$ of $V$, of dimensions $n, n-1, \ldots, 0$, such that $x(V_i) \subset V_{i+1}$ for all $x \in g$ and $i = 0, 1, \ldots, n-1$.

### 4. THE LARGEST NILPOTENT IDEAL OF A LIE ALGEBRA

Let $g$ be a Lie algebra and $a$ an ideal of $g$. For $a$ to be nilpotent, it is necessary and sufficient that, for all $x \in a$, $\operatorname{ad}_g x$ be nilpotent; the condition is obviously sufficient and is necessary, for, if $a$ is nilpotent and $x \in a$, $\operatorname{ad}_a x$ is nilpotent and $\operatorname{ad}_g x$ maps $g$ into $a$, hence $\operatorname{ad}_g x$ is nilpotent. Then Proposition 4 applied to the adjoint representation of $g$ gives the following result:

#### Proposition 6 {#lie-i-s4-prop-6 .statement}

Let $g$ be a Lie algebra and $E$ the associative subalgebra of $\mathcal{L}(g)$ generated by 1 and the $\operatorname{ad}_g x$ ($x \in g$). Let $R$ be the Jacobson radical of $E$.
(a) The set $n$ of $y \in g$ such that $\operatorname{ad}_g y \in R$ is the largest nilpotent ideal of $g$.
(b) It is orthogonal to $g$ under the Killing form.

It should be noted that $g/n$ can have non-zero nilpotent ideals.

### 5. EXTENSION OF THE BASE FIELD

Let $g$ be a Lie $K$-algebra, $K_1$ an extension of $K$ and $g' = g_{(K_1)}$. As $\mathcal{C}^k g' = (\mathcal{C}^k g)_{(K_1)}$, $g$ is nilpotent if and only if $g'$ is nilpotent.

Let $M$ be a $g$-module of finite dimension over $K$, $n$ the largest nilpotency, ideal for $M$ and $M' = M_{(K_1)}$. Let $(M_i)_{0 \leq i \leq n}$ be a Jordan-Hölder series of the $g$-module $M$. Then $x_M(M_i) \subset M_{i+1}$ for all $i$ and all $x \in n$, hence

$$
x'_{M'}((M_i)_{(K_1)}) \subset (M_{i+1})_{(K_1)}
$$

for all $i$ and all $x' \in n_{(K_1)}$; hence $x'_{M'}$ is nilpotent for $x' \in n_{(K_1)}$ so that $n_{(K_1)}$ is contained in the largest nilpotency ideal $n'$ for $M'$. We shall now see that, *if $K_1$ is separable over $K$, then $n' = n_{(K_1)}$*. Let $E$ be the associative $K$-algebra generated by 1 and the $x_M$ ($x \in g$), $E'$ the associative $K$-algebra generated by 1 and the $x_{M'}$ ($x' \in g'$) and $R$ and $R'$ the Jacobson radicals of $E$ and $E'$. The algebra $E'$ is canonically identified with $E_{(K_1)}$. Then $R' = R_{(K_1)}$ (*Algebra*, Chapter VIII, § 7, no. 2, Corollary 2 (c) to Proposition 3). Then let $y' \in n'$ and write

$$
y' = \sum_{i=1}^n \lambda_i y_i,
$$

where the $y_i$ are in $g$ and the $\lambda_i \in K_1$ are linearly independent over $K$. Then $y'_{M'} = \sum_{i=1}^n \lambda_i (y_i)_{M'}$ and $y'_{M'} \in R' = R_{(K_1)}$. Hence $(y_i)_M \in R$ and therefore $y_i \in n$ for all $i$. It follows that $y' \in n_{(K_1)}$, whence $n' \subset n_{(K_1)}$.

In particular, if $K_1$ is separable over $K$, the largest nilpotent ideal of $g_{(K_1)}$ is derived from that of $g$ by extending the base field from $K$ to $K_1$.

### Exercises {#lie-i-s4-exercises}

The conventions of § 4 remain valid unless otherwise mentioned.

See the [exercises for § 4](exercises/s4/).
