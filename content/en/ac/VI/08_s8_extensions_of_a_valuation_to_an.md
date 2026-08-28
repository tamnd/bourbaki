---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 8
section_title: Extensions of a valuation to an algebraic extension
lang: en
source: ac-i-vii
book_pages: 416-431, 461-469
pdf_pages: 0434-0449, 0479-0487
extraction: ocr
subsections:
    - "no": 1
      title: RAMIFICATION INDEX. RESIDUE CLASS DEGREE
      page: 416
      pdf_page: 434
    - "no": 2
      title: EXTENSION OF A VALUATION AND COMPLETION
      page: 418
      pdf_page: 436
    - "no": 3
      title: THE RELATION $\sum_i e_i f_i \leq n$
      page: 420
      pdf_page: 438
    - "no": 4
      title: INITIAL RAMIFICATION INDEX
      page: 422
      pdf_page: 440
    - "no": 5
      title: THE RELATION $\sum_i e_i f_i = n$
      page: 423
      pdf_page: 441
    - "no": 6
      title: VALUATION RINGS IN AN ALGEBRAIC EXTENSION
      page: 427
      pdf_page: 445
    - "no": 7
      title: THE EXTENSION OF ABSOLUTE VALUES
      page: 428
      pdf_page: 446
statements: 36
exercises: 21
content_sha256: fc835dafb82892179666e1a17cd7ccd72ff8254f70295e13ff0a7b86f19eae27
---

## 8. EXTENSIONS OF A VALUATION TO AN ALGEBRAIC EXTENSION

### 1. RAMIFICATION INDEX. RESIDUE CLASS DEGREE

Let $\mathbf{K}$ be a field, $\mathbf{L}$ an extension of $\mathbf{K}$ and $\mathbf{A}'$ a valuation ring of $\mathbf{L}$. As has been seen in § 1, no. 4, the ring $\mathbf{A} = \mathbf{K} \cap \mathbf{A}'$ is a valuation ring of $\mathbf{K}$ and
$$
m(\mathbf{A}) = m(\mathbf{A}') \cap \mathbf{K}.
$$
If $v'$ is a valuation associated with $\mathbf{A}'$, the restriction $v$ of $v'$ to $\mathbf{K}$ is a valuation on $\mathbf{K}$ associated with $\mathbf{A}$; the order group $\Gamma_v$ of $v$ is a subgroup of the order group $\Gamma_{v'}$ of $v'$.

#### Definition 1 {#ac-vi-s8-def-1 .statement}

*The index* $[\mathfrak{p}_v : \Gamma_{v'}]$ *is called the ramification index of* $v'$ *over* $v$ *(or over* $\mathbf{K}$*) and denoted by* $e(v'/v)$ *(or* $e(A'/A)$, *or sometimes* $e(L/K)$*).

This index is a natural number or $+\infty$. If $v'_0$ is a valuation *equivalent* to $v'$, $e(v'/v)$ is also called the ramification index of $v'_0$ *over* $v$. If $e(v'/v) = 1$, $v'$ is called *unramified* over $v$.

On the other hand the residue field $\kappa(\mathbf{A})$ of $v$ is identified with a subfield of the residue field $\kappa(\mathbf{A}')$ of $v'$.

#### Definition 2 {#ac-vi-s8-def-2 .statement}

*The degree* $[\kappa(\mathbf{A}') : \kappa(\mathbf{A})]$ *is called the residue class degree of* $v'$ *over* $v$ *(or over* $\mathbf{K}$*) and denoted by* $f(v'/v)$ *(or* $f(A'/A)$, *or sometimes* $f(L/K)$*).

This degree is a natural number or $+\infty$.

#### Lemma 1 {#ac-vi-s8-lem-1 .statement}

*Let* $\mathbf{K}, \mathbf{K}', \mathbf{K}''$ *be three fields such that* $K \subset K' \subset K''$, $v''$ *a valuation on* $K''$ *and* $v$ *and* $v'$ *its restriction to* $\mathbf{K}$ *and* $\mathbf{K}'$. *Then there are the relations:*
$$(1)\quad e(v''/v) = e(v''/v') e(v'/v), \qquad f(v''/v) = f(v''/v') f(v'/v).$$

This is obvious.

#### Lemma 2 {#ac-vi-s8-lem-2 .statement}

Let $K$ be a field, $L$ a finite extension of $K$ of degree $n$, $v'$ a valuation on $L$ and $v$ its restriction to $K$. Then the inequality

$$
e(v'/v) f(v'/v) \leq n
$$

holds; in particular $e(v'/v)$ and $f(v'/v)$ are finite.

Let us take natural numbers $r$ and $s$ respectively not greater than $e(v'/v)$ and $f(v'/v)$. It suffices to show that $rs \leq n$. In view of the definition of $r$, there exist elements $x_i$ of $L$ ($1 \leq i \leq r$) such that $v'(x_i) \not\equiv v'(x_j)$ (mod. $\Gamma_v$) for $i \neq j$. In view of the definition of $s$, there exist elements $y_k$ ($1 \leq k \leq s$) of the ring $A'$ of $v'$ whose canonical images $\bar{y}_k$ in $\kappa(A')$ are linearly independent over $\kappa(A)$; obviously $v'(y_k) = 0$ for all $k$. We shall show that the $rs$ elements $x_i y_k$ are linearly independent over $K$, which will certainly establish the inequality $rs \leq n$.

Suppose then that there exists a non-trivial linear relation of the form

$$
\sum_{i,k} a_{ik} x_i y_k = 0 \quad (a_{ik} \in K).
$$

Let us choose the indices $j, m$ so that

$$
v'(a_{jm} x_j y_m) \leq v'(a_{ik} x_i y_k)
$$

for every ordered pair $(i, k)$; then $a_{jm} \neq 0$. If $i \neq j$, then $v'(a_{ik} x_i y_k) = v'(a_{jm} x_j y_m)$ is impossible for this would imply

$$
v'(x_i) - v'(x_j) = v'(a_{jm}) - v'(a_{ik}) \in \Gamma_v,
$$

contrary to the choice of the $x_i$. Multiplying (3) by $(a_{jm} x_j)^{-1}$, we obtain a relation of the form

$$
\sum_k b_k y_k + z = 0, \text{ where } b_k = \frac{a_{jk} x_j}{a_{jm} x_j} \in A', \quad z \in A'
$$

and $v'(b_k) \geq 0, v'(z) > 0$. Whence, in $\kappa(A')$, a relation of the form $\sum_k \bar{b}_k \bar{y}_k = 0$. As $b_m = 1$, this contradicts the hypothesis made on $y_k$.

#### Proposition 1 {#ac-vi-s8-prop-1 .statement}

Let $K$ be a field, $L$ an algebraic extension of $K$, $v'$ a valuation on $L$, $v$ its restriction to $K$ and $A$ and $A'$ the rings of $v$ and $v'$. Then $\Gamma_{v'}/\Gamma_v$ is a torsion group and $\kappa(A')$ is an algebraic extension of $\kappa(A)$.

Let $(L_\alpha)$ be the family of finite sub-extensions of $L$; let us write $\Gamma_\alpha = v'(L_\alpha^*)$. The group $\Gamma_{v'}$ is the union of the right directed family consisting of the $\Gamma_\alpha$; as the groups $\Gamma_\alpha/\Gamma_v$ are finite (Lemma 2), $\Gamma_{v'}/\Gamma_v$ is a torsion group. The argument is similar to prove that $\kappa(A')$ is an algebraic extension of $\kappa(A)$.

#### Corollary 1 {#ac-vi-s8-prop-1-cor-1 .statement}

*The height of $v'$ is equal to that of $v$.*

This follows from Proposition 1 and the following lemma:

#### Lemma 3 {#ac-vi-s8-lem-3 .statement}

*Let $G'$ be a totally ordered group, $G$ a subgroup of $G$ and $\mathcal{G}'$ (resp. $\mathcal{G}$) the set of isolated subgroups of $G'$ (resp. $G$). The mapping $H' \mapsto H' \cap G$ maps $\mathcal{G}'$ onto $\mathcal{G}$. This mapping is bijective if $G'/G$ is a torsion group.*

Clearly $H' \in \mathcal{G}'$ implies $H' \cap G \in \mathcal{G}$. Now let $H \in \mathcal{G}$; let $H'$ denote the set of $x' \in G'$ such that there exists $h \in H$ satisfying $-h \leq x' \leq h$; it is immediately verified that $H'$ is an isolated subgroup of $G'$; then $H' \cap G = H$ since $H$ is isolated; hence the mapping $H' \mapsto H' \cap G$ is surjective. Suppose finally that $G'/G$ is a torsion group; let $H'_1$ and $H'_2$ be two isolated subgroups of $G'$ such that $H'_1 \cap G = H'_2 \cap G$; then, for example, $H'_1 \supset H'_2$ (cf. § 4, no. 4); then $H'_1/H'_2$ is a totally ordered group and is isomorphic to a quotient group of $H'_1/(H'_1 \cap G)$ which itself is identified with a subgroup of $G'/G$; hence $H'_1/H'_2$ is a torsion group and therefore reduces to 0.

#### Corollary 2 {#ac-vi-s8-lem-3-cor-2 .statement}

*For $v'$ to be improper (resp. of height 1), it is necessary and sufficient that $v$ be improper (resp. of height 1).*

#### Corollary 3 {#ac-vi-s8-lem-3-cor-3 .statement}

*Suppose that $L$ is a finite extension of $K$. For $v'$ to be discrete, it is necessary and sufficient that $v$ be discrete.*
If $v'$ is discrete, $\Gamma_{v'}$ is isomorphic to a non-zero subgroup of $\mathbf{Z}$ (Corollary 2) and hence to $\mathbf{Z}$. Conversely, if $v$ is discrete, $\Gamma_v$ is isomorphic to $\mathbf{Z}$ and $\Gamma_{v'}/\Gamma_v$ is a finite group (Lemma 2); hence $\Gamma_{v'}$ is a finitely generated commutative group of rank 1 and torsion-free; consequently it is isomorphic to $\mathbf{Z}$.

### 2. EXTENSION OF A VALUATION AND COMPLETION

#### Definition 3 {#ac-vi-s8-def-3 .statement}

*Let $K$ be afield, $v$ a valuation on $K$ and $L$ an extension of $K$. A family $(v'_i)_{i \in I}$ of valuations on $L$ which extend $v$ and such that every valuation on $L$ extending $v$ is equivalent to a unique $v'_i$ is called a complete system of extensions of $v$ to $L$.*

#### Proposition 2 {#ac-vi-s8-prop-2 .statement}

*Let $K$ be afield, $v$ a valuation on $K$, $\hat{K}$ the completion of $K$ with respect to $v$, $\hat{v}$ the continuous extension of $v$ to $\hat{K}$ and $L$ a finite extension of $K$ of degree $n$.
(a) Let $v'$ be a valuation on $L$ extending $v$; let $\hat{L}_{v'}$ denote the completion of $L$ with respect to $v'$ and $8'$ the continuous extension of $v'$ to $\hat{L}_{v'}$; identifying $\hat{K}$ with the closure of $K$ in $\hat{L}_{v'}$,
$$
e(\hat{v}'|\hat{v}) = e(v'|v), \quad f(\hat{v}'|\hat{v}) = f(v'|v),
$$
$$
[\hat{L}_{v'} : \hat{K}] \leq n,
$$
$$
e(v'|v)f(v'|v) \preceq [\hat{L}_{v'} : \hat{K}].
$$
(b) *Every set of pairwise independent valuations on $L$ extending a non-improper valuation $v$ is finite. Let $v'_1, \ldots, v'_s$ denote pairwise independent valuations on $L$ extending* v such that every valuation on L extending v is dependent on one of the v_i'; let L_i be the field L with the topology defined by v_i' and $\hat{L}_i$ its completion; we write $n_i = [\hat{L}_i : \hat{K}]$. Then the canonical mapping

$$
\phi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

(extending by continuity the diagonal mapping $L \to \prod_{i=1}^s L_i$) is surjective, its kernel is the Jacobson radical of $\hat{K} \otimes_K L$ and

$$
\sum_{i=1}^s n_i \leq n.
$$

Let us first prove (a). Suppose that v is not improper. As v and $\hat{v}$ (resp. $v'$ and $\hat{v}'$) have the same order group and the same residue field (\S 5, no. 3, Proposition 5 (b) and (f)), (4) holds. We deduce (6) from it by means of Lemma 2. Finally the vector sub-$\hat{K}$-space of $\hat{L}_{v'}$ generated by L is closed (\S 5, no. 2, Corollary to Proposition 4) and everywhere dense and hence equal to $\hat{L}_{v'}$; this shows (5).

We now pass to (b). We may still assume that v is not improper. Let $(v_1', \ldots, v_r')$ be any finite family of pairwise independent valuations on L extending v. The image of L in $\prod_{i=1}^r L_i$, under the diagonal mapping is everywhere dense (\S 7, no. 2, Theorem 1) and $\prod_{i=1}^r L_i$ is dense in $\prod_{i=1}^r \hat{L}_i$. Hence the canonical image of $\hat{K} \otimes_K L$ in $\prod_{i=1}^r \hat{L}_i$ is everywhere dense. On the other hand this image is a vector sub-$\hat{K}$-space of $\prod_{i=1}^r \hat{L}_i$; as $\prod_{i=1}^r \hat{L}_i$ is of finite dimension over $\hat{K}$ by (5), the image of $\hat{K} \otimes_K L$ is closed (\S 5, no. 2, Corollary to Proposition 4) and hence equal to $\prod_{i=1}^r \hat{L}_i$. As the dimension of $\hat{K} \otimes_K L$ over K is n, $\sum_{i=1}^r n_i \leq n$. This shows in particular that the integer r is bounded above by n and shows the first assertion of (b).

We now take $(v_1', \ldots, v_s')$ as in the statement. The fact that

$$
\phi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

is surjective and relation (7) have already been shown. It remains to verify that the kernel n of $\phi$ is the Jacobson radical $t$ of $\hat{K} \otimes_K L$. As $\prod_{i=1}^s \hat{L}_i$ is semi-simple, $t \subset n$. On the other hand, for every maximal ideal m of $\hat{K} \otimes_K L$, the quotient field $L(m) = (\hat{K} \otimes_K L)/m$ is a composite extension of $\hat{K}$ and L over K (Algebra,

Chapter VIII, § 8, Proposition 1). There exists a valuation w on L(m) extending $\vartheta$ (§ 3, no. 3, Proposition 5); the restriction $v'$ of w to L extends $v$. As $[L(m): \hat{K}]$ is finite, $L(m)$ is complete with respect to w ($\S 5$, no. 2, Proposition 4). Now the closure of L in $L(m)$ is a field containing $\mathbf{K}$ and L and hence is equal to $L(m)$. Consequently $L(m)$ is identified with the completion $\hat{L}_{v'}$ and m is the kernel of the canonical mapping of $\hat{K} \otimes_K L$ onto $\hat{L}_{v'}$. Now, by hypothesis, there exists an index $i$ such that $v'$ and $v'_i$ are dependent; whence $L_{v'} = L_i$ ($\S 7$, no. 2, Proposition 3). Thus $n \subset m$, which proves that $n \subset r$ and completes the proof.

#### Corollary 1 {#ac-vi-s8-prop-2-cor-1 .statement}

*If K is complete with respect to v and v is not improper, two valuations on L extending v are dependent.*

This follows since $\hat{K} \otimes_K L = L$.

#### Corollary 2 {#ac-vi-s8-prop-2-cor-2 .statement}

*If $\hat{K}$ or L is separable over K, the canonical mapping*

$$
\phi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

*is an isomorphism*.

The Jacobson radical of $\hat{K} \otimes_K L$ is then zero (*Algebra*, Chapter VIII, § 7, no. 3, Theorem 1).

#### Remark {#ac-vi-s8-n2-rem-1 .statement}

Proposition 2 (b) shows that every composite extension of $\hat{K}$ and L over K (*Algebra*, Chapter VIII, § 8) is isomorphic to one of the completions $\hat{L}_i$ and that these are composite extensions no two of which are isomorphic.

### 3. THE RELATION $\sum_i e_i f_i \leq n$

Let K be a field, $v$ a valuation on K and L a finite extension of K of degree $n$. Let $(v'_1, \ldots, v'_r)$ be valuations on L extending $v$ *no two of which are equivalent; if* they are *independent* (which is always the case if $v$ is of height 1), then

$$
\sum_{i \in I} e(v'_i|v) f(v'_i|v) \leq n
$$

by Proposition 2 (formulae (6) and (7)). We shall see that this result is true in the general case. To be precise:

#### Theorem 1 {#ac-vi-s8-thm-1 .statement}

*Let K be a field, v a valuation on K and L a finite extension of K of degree n. Then:*

(a) *Every complete system $(v'_i)_{i \in I}$ of extensions of v to L is finite.*

(b) $\sum_{i \in I} e(v'_i|v) f(v'_i|v) \leq n$ and a fortiori $\operatorname{Card}(I) \leq n$

(c) *No two of the rings of the $v'_i$ are comparable with respect to inclusion.*

Since the theorem is trivial if $v$ is improper, we shall assume that $v$ is not improper. Let $(v'_1, \ldots, v'_s)$ be any finite family of valuations on L extending $v$, no

THE RELATION $\sum_i e_i f_i \leq n$

two of which are equivalent. We shall first prove that $\sum_{i=1}^s e(v'_i/v)f(v'_i/v) \leq n$. This will prove (a) and (b).

We argue by induction on s and suppose therefore that the inequality has been established for the case of 0, 1, ..., s - 1 valuations. We distinguish two cases.

(1) Suppose that there exist at least two independent valuations $v'_i$. Then there exists (\S 7, no. 2, Remark 1) a partition $[1, s] = I_1 \cup \ldots \cup I_t$ of $[1, s]$ such that:
(i) for $v'_i$ and $v'_j$ to be dependent, it is necessary and sufficient that $i$ and $j$ belong to the same $I_k$;
(ii) Card$(I_k) < s$ for all $k$.

We choose in each $I_k$ an index $i(k)$. Let $\hat{L}_{i(k)}$ denote the completion of $L$ with respect to $v'_{i(k)}$ and $n(k) = [\hat{L}_{i(k)} : \hat{K}]$. For all $i \in I_k$, $v'_i$ defines on $L$ the same topology as $v'_{i(k)}$ (\S 7, no. 2, Proposition 3) and hence may be extended to a valuation $\bar{v}'_i$ on $\hat{L}_{i(k)}$ whose restriction to $\hat{K}$ is 0. Since no two of the $v'_i$ for $i \in I$, are equivalent, the same is true of the $\bar{v}'_i$. The induction hypothesis applied to the ordered pair $(\hat{K}, \hat{L}_{i(k)})$ shows, by virtue of Proposition 2 (a), formula (4), that $\sum_{i \in I_k} e(v'_i/v)f(v'_i/v) \leq n(k)$. As $\sum_{k=1}^t n(k) \leq n$ (Proposition 2 (b), formula (7)), certainly $\sum_{i=1}^s e(v'_i/v)f(v'_i/v) \leq n$.

(2) We now pass to the case where any two of the $v'_i$ are dependent. Let $A'_i$ be the ring of $v'_i$ ($1 \leq i \leq s$); writing $A$ for the ring of $v$, $A'_i \cap K = A$ for all $i$. Let $B'$ be the subring of $L$ generated by $A'_1, \ldots, A'_s$; we write $B = B' \cap K$; then $B \supseteq A$. Then $B$ is the ring of a valuation $w$ on $K$ and $B'$ the ring of a valuation $w'$ which is not improper and extends $w$ (\S 7, no. 2, Proposition 4); the field $\kappa(B')$ is an extension of $\kappa(B)$ of degree $f(w'/w)$. Consider the canonical images $\bar{A}'_i, \bar{A}$ of $A'_i$ and $A$ in $\kappa(B')$; then $\bar{A}$ is the ring of a valuation $\bar{v}$ on $\kappa(B)$ and the $\bar{A}'_i$ are rings of valuations $\bar{v}'_i$ on $\kappa(B')$ extending $\bar{v}$. As the $A'_i$ generate $B'$, the $\bar{A}'_i$ generate $\kappa(B')$ and hence the $\bar{v}'_i$ are not all dependent (\S 7, no. 2, Proposition 4). From the first part of the proof,

$$
\sum_{i=1}^s e(\bar{v}'_i/\bar{v})f(\bar{v}'_i/\bar{v}) \leq [\kappa(B') : \kappa(B)] = f(w'/w)
$$

and hence

$$
\sum_{i=1}^s e(w'/w)e(\bar{v}'_i/\bar{v})f(\bar{v}'_i/\bar{v}) \leq e(w'/w)f(w'/w) \leq n \quad \text{(no. 1, Lemma 1).}
$$

The proof of (a) and (b) will therefore be completed if we prove that

$$
f(\bar{v}'_i/\bar{v}) = f(\bar{v}'_i/v), \quad e(w'/w)e(\bar{v}'_i/\bar{v}) = e(v'_i/v).
$$

For this, we note that $v$ and $\bar{v}$ (resp. $v'_i$ and $\bar{v}'_i$) have the same residue field (§ 4, no. 1, Corollary to Proposition 2); this proves the first equation. For the second there is, by virtue of the Remark in §4, no. 3, the following commutative diagram, where the rows are exact sequences and the vertical arrows represent canonical injections:

$$
\begin{array}{ccccccccc}
0 & \to & \Gamma_{\bar{v}} & \to & \Gamma_v & \to & \Gamma_w & \to & 0 \\
& & \downarrow & & \downarrow & & \downarrow & & \\
0 & \to & \Gamma_{\bar{v}_i'} & \to & \Gamma_{v_i'} & \to & \Gamma_{w'} & \to & 0
\end{array}
$$

We deduce that there is an exact sequence

$$
0 \to \Gamma_{\bar{v}_i'}/\Gamma_{\bar{v}} \to \Gamma_{v_i'}/\Gamma_v \to \Gamma_{w'}/\Gamma_w \to 0
$$

by Chapter I, § 1, no. 4, Proposition 2, which proves the second formula (8).

To complete the proof of Theorem 1, it remains to prove (c). If the ring of $v_i'$ contains that of $v_j'$, $\Gamma_{v_i'}$ is identified with a quotient group $\Gamma_{v_j'}/H$, $H$ being an isolated subgroup (§ 4, no. 3). As the composite canonical mapping

$$
\Gamma_v \to \Gamma_{v_j} \to \Gamma_{v_j'}/H = \Gamma_{v_i'}
$$

is injective, $H \cap \Gamma_v = \{0\}$, whence $H = \{0\}$ (Lemma 3, no. 1). Then $v_i'$ and $v_j'$ are equivalent, whence $i = j$.

#### Remark {#ac-vi-s8-n3-rem-1 .statement}

The intersection C of the rings $A_i'$ of the valuations $v_i'$ ($i \in I$) is the integral closure of $A$ in L (§ 1, no. 3, Corollary 3 to Theorem 3); it follows moreover from (c) and § 7, no. 1, Propositions 1 and 2 that C is a semi-local ring, that its maximal ideals are the intersections $m_i = C \cap m(A_i')$ and that $A_i' = C$, for all $i \in I$.

### 4. INITIAL RAMIFICATION INDEX

#### Definition 4 {#ac-vi-s8-def-4 .statement}

Let G be a totally ordered commutative group and H a subgroup of G of finite index. The number of major subsets of G consisting of strictly positive elements and containing all the elements > O of H is called the initial index of H in G and denoted by $\varepsilon(G, H)$.

This initial index is a natural number by virtue of the following proposition:

#### Proposition 3 {#ac-vi-s8-prop-3 .statement}

Under the hypotheses of Definition 4, if the set of strictly positive elements of G has no least element, then $\varepsilon(G, H) = 1$ for all H. If there exists a least element > O of G and $G'$ denotes the subgroup it generates, then

$$
\varepsilon(G, H) = (G : (G \cap H)).
$$

In the first case, let x be an element > 0 in G. The set of $y \in G$ such that $0 < y < x$ is infinite and hence there exist two elements of this set which are distinct and congruent modulo H; their difference is an element z of H such that $0 < z < x$. Hence every major subset which contains all the strictly positive elements of H contains x and hence all the elements > 0 of G.

In the second case, let $x$ be the least element >0 of G and let $n$ be the least integer >0 such that $nx \in H$. Clearly $n = (G : (G \cap H))$. On the other hand, writing $M(y)$ for the set of $z \in G$ such that $y \leq z \ (y \in G)$, it is immediately seen that the major sets of Definition 4 are just $M(x), M(2x), \ldots, M(nx)$.

#### Corollary {#ac-vi-s8-n4-cor-1 .statement}

*The initial index $\varepsilon(G, H)$ divides the index* $(G : H)$ *and is equal to it if* $G$ *is isomorphic to* $\mathbf{Z}$.

In particular, $\varepsilon(G, H) \leq (G : H)$.

#### Definition 5 {#ac-vi-s8-def-5 .statement}

*Let* $K$ *be a field, L a finite extension of* $K$, $w$ *a valuation on* $L$, $v$ *its restriction to* $K$ *and* $\Gamma_w$ *and* $\Gamma_v$ *their order groups. The initial index of* $\Gamma_v$ *in* $\Gamma_w$ *is called the initial ramification index of* $w$ *with respect to* $v$ *(or with respect to* $K$*) and denoted by* $\varepsilon(w/v)$.

From the above corollary, $\varepsilon(w/v)$ divides $e(w/v)$ with equality in the case of a discrete valuation.

#### Proposition 4 {#ac-vi-s8-prop-4 .statement}

*Under the hypotheses of Definition 5, let* $A$ *and* $m$ *(resp.* $A'$ *and* $m'$) *be the ring and ideal of the valuation* $v$ *(resp.* $w$*). *Then*

$$
[A'/mA': A/m] = \varepsilon(w/v) f(w/v).
$$

The ideals of $A'$ containing $mA'$ and distinct from $A'$ correspond to the major subsets of $\Gamma_w$ consisting of elements >0 and containing the elements >0 of $\Gamma_v$ (\S 3, no. 5, Corollary to Proposition 7). They are therefore equal in number to $\varepsilon(w/v)$ and, as they form a totally ordered set under inclusion, this number is equal to the length of the quotient ring $A'/mA'$. Now a module of length 1 over $A'$ is a 1-dimensional vector space over $A'/m'$ and hence a module of length $f(w/v)$ over $A$; hence, as $A'/mA'$ is of length $\varepsilon(w/v)$ over $A'$, it is of length $\varepsilon(w/v) f(w/v)$ over $A$, that is over $A/m$.

### 5. THE RELATION $\sum_i e_i f_i = n$

#### Proposition 5 {#ac-vi-s8-prop-5 .statement}

*Let* $K$ *be a field, v a valuation on* $K$, $A$ *its ring, m its ideal, L a finite extension of* $K$ *of degree* $n$, $B$ *the integral closure of* $A$ *in* $L$ *and* $(v'_i)_{1 \leq i \leq s}$ *a complete system of extensions of* $v$ *to* $L$. *Then*

$$
[B/mB : A/m] = \sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v).
$$

Let $A_i$ be the ring of $v'_i$; then $A_i = B_{m_i}$ where $m_i$ runs through the family of maximal ideals of $B$ (no. 3, Remark). Let $q_i$ be the saturation of $mB$ with respect to $m_i$ (Chapter II, \S 2, no. 4). By Chapter V, Corollary 3 to Proposition 1, no. 1, \S 2, the canonical homomorphism $B/mB \to \prod_{i=1}^s B/q_i$ is an isomorphism and $m_i$ is the only maximal ideal of B containing $q_i$. Hence $B/q_i$ is canonically isomorphic to $(B/q_i)_{m_i}$ (Chapter II, § 3, no. 3, Proposition 8), that is to
$$
B_{m_i}/mB_{m_i} = A_i/mA_i.
$$
Therefore there is a canonical isomorphism $B/mB \to \prod_{i=1}^s A_i/mA_i$, whence the result by virtue of Proposition 4 of no. 4.

#### Corollary {#ac-vi-s8-n5-cor-1 .statement}

*With the same hypotheses and notation,
$$
[B/mB : A/m] = \sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) \leq \sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) \leq n.
$$
We know that $\varepsilon(v'_i/v) \leq \varepsilon(v'_i/v)$ (no. 4, Corollary to Proposition 3) and $\sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) \leq n$ (no. 3, Theorem 1).

#### Theorem 2 {#ac-vi-s8-thm-2 .statement}

*With the hypotheses and notation of Proposition 5, the following conditions are equivalent :
(a) B is a finitely generated A-module;
(b) B is a free A-module;
(c) $[B/mB : A/m] = n;$
(d) $\sum_{i=1}^n \varepsilon(v'_i/v) f(v'_i/v) = n$ and $\varepsilon(v'_i/v) = \varepsilon(v'_i/v)$ for all i.

The equivalence of (a) and (b) follows from Lemma 1, § 3, no. 6. Clearly (b) implies (c) (*Algebra*, Chapter 11, § 1, no. 5, formula (19)). The equivalence of (c) and (d) follows from the Corollary to Proposition 5. It remains to show that (c) implies (b).

In general, if M is an A-module, we shall denote by V(M) the vector space $M/mM$ over $A/m$. Hypothesis (c) means that $\dim(V(B)) = n$. Let $x_1, \ldots, x_n$ be elements of B whose canonical images in V(B) form a basis of V(B) and let L $\subset B$ be the sub-A-module which they generate. As L is torsion-free and finitely generated, it is free (§ 3, no. 6, Lemma 1). We shall see that $B = L$. Let $y \in B$; we write $M = L + Ay$; this is also a free A-module. The canonical injections $L \to M \to B$ give canonical homomorphisms $V(L) \to V(M) \to V(B)$. As the ranks of L and M are $\leq n$, so are the dimensions of V(L) and V(M). Now, by hypothesis, $V(L) \to V(B)$ is surjective and $V(B)$ is n-dimensional hence $V(L)$ and $V(M)$ are n-dimensional and $V(L) \to V(M)$ is surjective. As M is finitely generated, $L \to M$ is surjective (Chapter II, § 3, no. 2, Corollary 1 to Proposition 4), whence $L = M, y \in L$ and $B = L$. Hence B is free.

*Remark (1)* If v is *discrete*, $\varepsilon(v'_i/v) = \varepsilon(v'_i/v)$ (no. 4) and condition (d) reduces to $\sum_{i=1}^s \varepsilon(v'_i/v) f(v'_i/v) = n.$

#### Corollary 1 {#ac-vi-s8-thm-2-cor-1 .statement}

*With the same hypotheses and notation, suppose further that v is discrete and L separable. Then*

$$
\sum_{i=1}^{s} e(v_i'/v) f(v_i'/v) = n.
$$

The integral closure B of A is then a free A-module of rank $n$, since A is a principal ideal domain (Chapter V, § 1, no. 6, Corollary 2 to Proposition 18).

#### Corollary 2 {#ac-vi-s8-thm-2-cor-2 .statement}

*Let K be a field, v a discrete valuation on K with respect to which K is complete and L a finite extension of K of degree n. Then v admits a unique (upto equivalence) extension $v'$ to L, the ring A' of $v'$ is a finitely generated free module over the ring A of v and $e(v'/v) f(v'/v) = n$.*

adic topology (where $m = m(A)$); the ring A is complete, for it is closed in K. We conclude that, since $A'/mA'$ is a finite-dimensional vector ($A/m$)-space (no. 4, Proposition 4), A' is a finitely generated A-module (Chapter III, § 2, no. 9, Corollary 3 to Proposition 12). It is therefore free and $e(v'/v) f(v'/v) = n$ by

$$
\phi : \hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

(no. 2, Proposition 2). *is bijective. For all $x \in L$, the characteristic polynomial $P_{C_{L/K}}(x; X)$ is equal to the product of the characteristic polynomials $P_{C_{\hat{L}_i/\bar{K}}}(x; X)$ ($1 \leq i \leq s$); in particular,

$$
\begin{cases}
\operatorname{Tr}_{L/K}(x) = \sum_{i=1}^s \operatorname{Tr}_{\hat{L}_i/\bar{K}}(x) \\
N_{L/K}(x) = \prod_{i=1}^s N_{\hat{L}_i/\bar{K}}(x) \\
v(N_{L/K}(x)) = \sum_{i=1}^s n_i v_i'(x).
\end{cases}
$$

(The last relation in (9) is meaningful, for we may obviously assume that the $v_i'$, which are of height 1 by Corollary 2 to Proposition 1 of no. 1, take, as does v, their values in a subgroup of $\mathbf{R}$.)

As no two of the $v'_i$ are equivalent and they are of height 1, they are independent and Proposition 2 of no. 2 shows therefore that $e(v'_i/v) f(v'_i/v) \leq n_i$ for all $i$ and $\sum_{i=1}^s n_i \leq n$. The first assertion therefore follows from these inequalities and the relation $\sum_{i=1}^s e(v'_i/v) f(v'_i/v) = n$. Under the isomorphism $\phi$ the endomorphism $z \mapsto z(1 \otimes x)$ of $\hat{K} \otimes_K L$ (for $x \in L$) is transformed into the endomorphism of $\prod_{i=1}^s \hat{L}_i$ leaving invariant each of the factors and reducing on each factor to multiplication by $x$ ($L$ being canonically imbedded in its completion $\hat{L}_i$); whence the assertion relating to the characteristic polynomial of $x$ and the first two formulae of (9). Finally, let E be a finite quasi-Galois extension of $\hat{K}$, containing $\hat{L}_i$; as $\hat{K}$ is complete and $\hat{\nu}$ of height 1, there exists only one valuation (upto equivalence) $w$ on E extending $\hat{\nu}$ (no. 2, Corollary 1 to Proposition 2); then, for every $\hat{K}$-automorphism $\sigma$ of E, $w(\sigma(x)) = v'_i(x)$. Therefore
$$
\vartheta(N_{\hat{L}_i/\hat{K}}(x)) = n_i v'_i(x)
$$
(Algebra, Chapter VIII, § 12, no. 2, formula (15)), which proves the formula of (9).

#### Corollary 4 {#ac-vi-s8-thm-2-cor-4 .statement}

*Under the hypotheses of Corollary 3, if L is a separable extension of K, each of the $\hat{L}_i$ is a separable extension of $\hat{K}$. If further L is a Galois extension of K with Galois group $\mathcal{G}$ and $\mathcal{G}_i$ denotes the decomposition group of the ideal of $v'_i$ in B (Chapter V, § 2, no. 2, Definition 2), then $\hat{L}_i$ is a Galois extension of $\hat{K}$ whose Galois group is isomorphic to $\mathcal{G}_i$.*

Clearly $\hat{L}_i = \hat{K}(L)$; hence, if L is separable over K, $\hat{L}_i$ is separable over $\hat{K}$ (Algebra, Chapter V, § 7, no. 6, Proposition 10). Suppose now that L is Galois. Every automorphism $\sigma \in \mathcal{G}_i$ is continuous on L with the topology defined by $v'_i$, the fact that no two of the ideals of the $v'_i$ are comparable with respect to inclusion (§ 7, no. 2, Corollary 1 to Theorem 1) necessarily implying that $v'_i = v'_i \circ \sigma$ by definition of $\mathcal{G}_i$; hence $\sigma$ may be extended by continuity to a $\hat{K}$-automorphism $\hat{\sigma}$ of $\hat{L}_i$. This proves that the number of $\hat{K}$-automorphisms off,, is at least equal to $\mathrm{Card}(\mathcal{G}_i)$. But as the valuations $v'_i$ are pairwise conjugate under $\mathcal{G}$ (Chapter V, § 2, no. 3, Proposition 6), $s = (\mathcal{G}_i)$, whence
$$
\mathrm{Card}(\mathcal{G}_i) = n/s \leq n.
$$
and on the other hand $n = sn$, by Corollary 3; this proves that $\hat{L}_i$ is a Galois extension of $\hat{K}$ and that the extensions by continuity of the automorphisms $\sigma \in \mathcal{G}_i$ are the only $\hat{K}$-automorphisms of $\hat{L}_i$.

*Remark (2)*. Part of the above results extends to the case of valuations on a *not necessarily commutative* field K (cf. § 3, no. 1). Let L be an extension field of K and let $v'$ be a valuation on L, $v$ its restriction to K and A' and A the respective rings of the valuations $v'$ and $v$; then there is defined a ramification index $e(v'/v)$ as in no. 1; on the other hand, $\kappa(A)$ is identified with a subfield of $\kappa(A')$ and the (left) residue rank of $v'$ with respect to $v$ is defined to be the number $f(v'/v)$ equal to the dimension of the left vector $\kappa(A)$-space $\kappa(A')$, if this dimension is finite, and $+\infty$ in the opposite case. Then, if L is a left vector K-space of finite dimension $n$, Lemma 2 of no. 1 and its proof go over unchanged. Moreover, if K is complete with respect to $v$, the assertions of Corollary 2 to Theorem 2 of no. 5 (other than the existence of $u'$) are also valid ($n$ denoting the dimension of L as a left vector K-space) with the following proof:

In the first place the topology defined by $v'$ on L is Hausdorff and compatible with its left vector K-space structure and hence two extensions of $v$ to L give the same topology on L ($\S 5$, no. 2, Proposition 4), which proves that these extensions are the same up to equivalence ($\S 6$, no. 2). We show next that, if $m = m(A)$, $A'/mA'$ is a left vector $(A/m)$-space of dimension $e(v'/v) f(v'/v)$. Writing $e = e(v'/v)$, we may assume that $v(K^*) = Z$ and $v'(L^*) = e^{-1}Z$; let $u'$ be an element of L such that $v'(u') = e^{-1}$ and $u$ an element of K such that $v(u) = 1$; hence $u = z{u'}^e$, where $z \in L$ is such that $v'(z) = 0$. As m is generated by $u$ (as a left or right ideal of A), $mA' = {u'}^eA' = A'{u'}^e$ and it suffices to prove that, for $0 \leq k \leq e - 1$, $A'{u'}^k/A'{u'}^{k+1}$ is a left vector $(A/m)$-space of dimension $f(v'/v)$. But $t \mapsto t{u'}^k$ is an isomorphism of the left A-module A onto the left A-module $A'{u'}^k$ mapping $A'u'$ to $A'{u'}^{k+1}$ and which therefore gives by taking quotients an $(A/m)$-isomorphism of $A'/A'u'$ onto $A'{u'}^k/A'{u'}^{k+1}$, whence our assertion by definition of $f(v'/v)$, $u'$ generating the maximal ideal of $A'$. The proof is completed as when K and L are commutative (the fact that a finitely generated torsion-free A-module is free being proved as in $\S 3$, no. 6, Lemma 1).

### 6. VALUATION RINGS IN AN ALGEBRAIC EXTENSION

#### Proposition 6 {#ac-vi-s8-prop-6 .statement}

Let K be a field, $v$ a valuation on K, A its ring, L an algebraic extension of K and $A'$ the integral closure of A in L. Let 23 be the set of valuation rings on L which extend $v$ and $\mathfrak{M}'$ the set of maximal ideals of $A'$. Then the mapping $V \mapsto m(V) \cap A'$ is a bijection of 23 onto $\mathfrak{M}'$ and $m' \mapsto A'_{m'}$ is the inverse bijection.

Every maximal ideal $m'$ of $A'$ is such that $m' \cap A$ is the maximal ideal of A (Chapter V, § 2, no. 1, Proposition 1) and $A'_{m'}$ is dominated by a valuation ring V of L (which is therefore the ring of a valuation on L extending $v$) ($\S 1$, no. 2, Corollary to Theorem 2). The field L is the union of a directed family of sub-extensions K, of L which are finite over K and it will suffice, in order to see that $V = A'_{m'}$, to prove that $V \cap K = A'_{m'} \cap K$, for all $\alpha$. Now, if we write $A'_\alpha = A' \cap K_\alpha$, $A'_\alpha$ is the integral closure of A in K, and hence is the intersection of the rings of the valuations on K, which extend $v$ and these rings $V_\alpha$ are finite in number and are the local rings $(A'_\alpha)_{i|m_\alpha}$ of $A'_\alpha$ ($1 \leq i \leq n$), where the $m'_{i\alpha}$ are the distinct maximal ideals of $A'_\alpha$ (no. 3, Remark); but $m' \cap A'_\alpha$ is one of the $m'_{i\alpha}$ and $V \cap K_\alpha$ is therefore equal to the corresponding local ring $(A'_\alpha)_{m'_{i\alpha}} \subset A'_{m'}$, which completes the proof that $V = A'_{m'}$. Conversely, if $V \in \mathfrak{V}$, then $A' \subset V$ (\$3, no. 3, Proposition 6) and, if $m' = m(V) \cap A'$, then $m' \cap A = m$, hence $m'$ is a maximal ideal of $A'$ (Chapter V, § 2, no. 1, Proposition 1) and the above argument shows that $V = A'_{m'}$.

#### Proposition 7 {#ac-vi-s8-prop-7 .statement}

*Let K be a field, L a quasi-Galois extension of K and f and $f'$ places of L with values in the same field F. Suppose that the restrictions off and $f'$ to K coincide. Then there exists a K-automorphism s of L such that $f' = f \circ s$.*

Let A be the ring of the place of K the common restriction off and $f'$. The rings off and $f'$ contain the integral closure $A'$ of A in L (\$ 1, no. 3, Corollary 3 to Theorem 3) and hence (Chapter V, § 2, no. 3, Corollary 1 to Proposition 6) there exists a K-automorphism s of L such that the restrictions off and $f \circ s$ to $A'$ are equal; if $m'$ is the common kernel of these restrictions, $m' \cap A$ is the maximal ideal of A, hence $m'$ is a maximal ideal of $A'$ and the places $f'$ and $f \circ s$ coincide on the ring $A'_{m'}$; but by Proposition 6 the only valuation ring of L dominating $A'_{m'}$ is the ring $A'_{m'}$ itself and hence the rings of the places $f'$ and $f \circ s$ are the same.

#### Corollary 1 {#ac-vi-s8-prop-7-cor-1 .statement}

*Let K be a field, v a valuation on K, L a quasi-Galois extension of K and $v'$ and $v''$ two extensions of v to L. Then there exists a K-automorphism s of L such that $v''$ is equivalent to $v' \circ s$.*

Let $f'$ and $f''$ be the places of K associated with $v'$ and $v''$; replacing them if need be by equivalent places, it may be assumed that they both take their values in the algebraic closure of the residue field of v (no. 1, Proposition 1). Then there exists a K-automorphism s of L such that $f'' = f' \circ s$ (Proposition 7); thus $v''$ is equivalent to $v' \circ s$ by virtue of the correspondence between places and valuations (\$ 3, no. 3).

#### Corollary 2 {#ac-vi-s8-prop-7-cor-2 .statement}

*Let K be a field, f a place of K (resp. v a valuation on K) and L a radicial extension of K. Then all the extensions of f (resp. v) to L are equivalent.*

L is a quasi-Galois extension and its only automorphism is the identity. Corollary 2 therefore follows from Proposition 7 (resp. Corollary 1).

#### Proposition 8 {#ac-vi-s8-prop-8 .statement}

*Let K be a field, v a valuation on K, L a finite quasi-Galois extension of K of degree n and $(v'_i)_{1 \leq i \leq g}$ a complete system of extensions of v to L. Then $e(v'_i/v)$ and $f(v'_i/v)$ have values e and $\mathfrak{f}$ independent of i. Then $ef g \leq n$. If the integral closure in L of the ring A of v is a finitely generated A-module, then $ef g = n$.*

This follows immediately from Theorems 1 (no. 3) and 2 (no. 5).

### 7. THE EXTENSION OF ABSOLUTE VALUES

#### Proposition 9 {#ac-vi-s8-prop-9 .statement}

*Let K be a field, L an algebraic extension of K and $\mathfrak{f}$ an absolute value on K. Then $\mathfrak{f}$ can be extended to an absolute value on L.*

Suppose first that there exists a valuation $v$ on $K$ with real values such that $f(x) = e^{-v(x)}$. There exists a valuation $v'$ on $L$ whose restriction to $K$ is equivalent to $v$ ($\S 3$, no. 3, Proposition 5). Then $v'$ is of height 0 or 1 (no. 1, Corollary 2 to Proposition 1) and therefore may be assumed to have real values. The restriction of the mapping $x \mapsto e^{-v'(x)}$ to $K$ is an absolute value equivalent to $f$ and hence of the form $f^s$ with $s > 0$ (*General Topology*, Chapter IX, $\S 3$, no. 2, Proposition 5). We conclude that

$$
x \mapsto e^{-v'(x)/s}
$$

is an absolute value on $L$ extending $f$.

Suppose now that $f$ is not ultrametric. Then $K$ is identified with a subfield of $\mathbf{C}$ such that $f(x) = |x|^s$ where $0 \leq s \leq 1$ ($\S 6$, no. 4, Theorem 2). As $\mathbf{C}$ is algebraically closed, $L$ is identified with a subfield of $\mathbf{C}$ and the absolute value $x \mapsto |x|^s$ extends $f$.

#### Proposition 10 {#ac-vi-s8-prop-10 .statement}

*Let $K$ be a field, $f$ an absolute value on $K$ such that $K$ is complete and not discrete with respect to $f$ and $L$ an algebraic extension of $K$. Then $f$ can be extended uniquely to an absolute value $f'$ on $L$ and, if $L$ is of finite degree $n$, then*

$$
f'(x) = (f(N_{L/K}(x)))^{1/n}
$$

*for all* $x \in L$.

The existence of $f'$ follows from Proposition 9 and its uniqueness (over every finite sub-extension of $L$ and therefore over the whole of $L$) from Lemma 2 of $\S 6$, no. 4. Let $f'$ be the unique extension off to the algebraic closure of $K$ and suppose $L$ is of finite degree $n$. We know that $N_{L/K}(x) = \prod_{i=1}^n x_i$, where each $x_i$ is a conjugate of $x$ over $K$ (*Algebra*, Chapter VIII, $\S 12$, no. 2, Proposition 4). In view of the uniqueness of $f'$, $f'(x_i) = f'(x)$ for all $i$, whence the stated formula.

#### Proposition 11 {#ac-vi-s8-prop-11 .statement}

*Let $K$ be a field, $f$ a non-ultrametric absolute value on $K$, $\hat{K}$ the completion of $K$ with respect to $f$, $\hat{f}$ the continuous extension off to $\hat{K}$ and $L$ a finite extension of $K$ of degree $n$.

(a) *Let $f'$ be an absolute value on $L$ extending $f$; let $\hat{L}_{f'}$ denote the completion of $L$ with respect to $f'$ and let $\hat{K}$ be identified with the closure of $K$ in $\hat{L}_{f'}$; then* $[\hat{L}_{f'} : K] \leq n$.

(b) *The absolute values on $L$ extending $f$ are finite in number. If they are denoted by* $f'_1, \ldots, f'_s$ *and the completion of $L$ with respect to* $f'_i$ *by* $\hat{L}_i$, *the canonical mapping*

$$
\hat{K} \otimes_K L \to \prod_{i=1}^s \hat{L}_i
$$

*is an isomorphism and*

$$
\sum_{i=1}^s [\hat{L}_i : \hat{K}] = n.
$$

(10)

The proof is the same as that for the analogous assertions in Proposition 2 (no. 2). The references

§ 7, no. 2, Theorem 1; § 5, no. 2, Corollary to Proposition 4 should be replaced by the following

§ 7, no. 3, Theorem 2; Topological Vector Spaces, Chapter I,
§ 2, no. 3, Corollary 1 to Theorem 2.

Observe that two extensions off to L which define the same topology are equal (General Topology, Chapter IX, § 3, no. 2, Proposition 5). Finally, as $f$ is not ultrametric, K is of characteristic 0 and hence the Jacobson radical of $\hat{K} \otimes_K L$ is zero.

Remarks
(1) Proposition 11 (b) shows that every composite extension of $\hat{K}$ and L over K is isomorphic to one of the completions $\hat{L}_i$ and that these are composite extensions no two of which are isomorphic.
(2) We know that the completions $\hat{K}$ and $\hat{L}_i$ are isomorphic to $\mathbf{R}$ or $\mathbf{C}$ ($\S 6$, no. 4, Theorem 2). If $\hat{K}$ is isomorphic to $\mathbf{C}$, so is $\hat{L}_i$ for all $i$ and (10) shows that the number of extensions $f_i'$ is *equal to n*. If $\hat{K}$ is isomorphic to $\mathbf{R}$ (for example if $K = \mathbf{Q}$), let $r_1$ (resp. $r_2$) denote the number of indices $i$ such that $\hat{L}_i$ is isomorphic to $\mathbf{R}$ (resp. $\mathbf{C}$); then (10) may be written:

$$
r_1 + 2r_2 = n.
$$

#### Proposition 12 {#ac-vi-s8-prop-12 .statement}

*Let K be a field, f an absolute value on K, L a quasi-Galois extension of K and $f'$ and $f''$ two extensions off to L. Then there exists a K-automorphism s of L such that $f'' = f' \circ s$.*

If $f$ is ultrametric, Corollary 1 to Proposition 7 (no. 6) shows that there exists a K-automorphism s of L such that $f''$ and $f' \circ s$ are equivalent absolute values; then there exists a real number $a > 0$ such that $f''(x) = (f'(s(x)))^a$ for all $x \in L$. If $f$ is not improper, take $x \in K^*$ such that $f(x) \neq 1$, which shows that $a = 1$. If $f$ is improper, so are $f'$ and $f''$ (Corollary 2 to Proposition 1, no. 1) and s may be taken to be the identity automorphism.

If $f$ is not ultrametric, there exist Q-isomorphisms $u', u''$ of L onto subfields of $\mathbf{C}$ and real exponents $a' > 0, a'' > 0$ such that $f'(x) = |u'(x)|^{a'}$ and

$$
f''(x) = |u''(x)|^{a''}
$$

for all $x \in L$ ($\S 6$, no. 4, Theorem 2). Taking $x = 2$, it is seen that $a' = a''$. The restrictions of $u'$ and $u''$ to K extend by continuity to isomorphisms $u_1$ and $u_2$ of $\hat{K}$ onto $\mathbf{R}$ (resp. $\mathbf{C}$). Then $u_2 \circ \bar{u}_1^{-1}$ is an automorphism of the *valued* field $\mathbf{R}$ (resp. $\mathbf{C}$) and is therefore the identity (resp. the identity or the automorphism $c : \zeta \to \bar{\zeta}$). Replacing if need be $u'$ by $c \circ u'$, it is seen that the restrictions of $u'$ and $u''$ to K may be assumed to coincide. Identifying K with a subfield of $\mathbf{C}$ by means of this common restriction, $u'$ and $u''$ are K-isomorphisms of L onto subfields of $\mathbf{C}$. As L is a quasi-Galois extension of K, there exists a K-automorphism s of L such that $u'' = u' \circ s$; since $a' = a''$, we deduce immediately that $f'' = f' \circ s$.

Remark (3). If $\hat{K}$ is isomorphic to $\mathbf{R}$, Proposition 12 shows that all the completions $\hat{L}_t$ of $L$ (in the notation of Proposition 11) are isomorphic to one another. Thus, with the notation of Remark 2 above, either $r_1 = n$ and $r_2 = 0$, or $r_1 = 0$ and $2r_2 = n$.

### Exercises {#ac-vi-s8-exercises}

See the [exercises for § 8](exercises/s8/).
