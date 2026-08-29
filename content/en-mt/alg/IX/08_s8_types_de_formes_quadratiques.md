---
book: alg
book_title: Algebra
chapter: IX
chapter_title: Formes sesquilinéaires et formes quadratiques
section: 8
section_title: Types de formes quadratiques
lang: en
source: alg-ix-fr
pdf_pages: 0130-0137
extraction: ocr
subsections:
    - "no": 1
      title: Types de formes quadratiques.
      page: 0
      pdf_page: 130
    - "no": 2
      title: Groupe des types de formes quadratiques.
      page: 0
      pdf_page: 132
    - "no": 3
      title: Anneau des types de formes quadratiques.
      page: 0
      pdf_page: 135
statements: 10
exercises: 0
content_sha256: 9597d70ccc4f2287399276b7482c92a23e2147cbca1b5400cff671a619b25517
translated_from: content/fr/alg/IX/08_s8_types_de_formes_quadratiques.md
source_lang: fr
translation_method: machine
source_content_sha256: 41114d3659ba1c03e45fbacc1d14e1405e0ae472fba157d2ff91fc89f7b4d7b1
translation_model: gpt-5-6-mini
translation_run: translate-en-mt-6f5b41cf
glossary_version: 34
glossary_terms_sha256: 03b8507ed3e75d118bbe9c5e958ab554bec1b6917ce8df8771557c923ea28315
prompt_sha256: 5b9b7144015934413fe8e16b5155e2bc50bed2041525e1b1db7c19a297193094
---

## § 8. Types of quadratic forms

In this paragraph we suppose that A is a commutative field.

### 1. Types of quadratic forms.

Given a quadratic form Q ($§ 3, n° 4$) on a vector space E over A, we shall say that E is the space of defini-

(*) These results (unpublished) were communicated to us by I. Kaplansky.

tion of Q and that dim(E) is the dimension of Q. Given two quadratic forms Q, Q' on vector spaces E, E' over A, we shall denote by Q ⊕ Q' their direct sum (§ 3, no 4). Recall that the direct sum of two neutral forms is neutral (§ 4, no 2).

Let us introduce the following relation:

« Q and Q' are non-degenerate quadratic forms of finite dimensions over A, and there exist neutral quadratic forms N, N' such that Q ⊕ N is equivalent to Q' ⊕ N' ».

This relation, which we shall denote by Q ~ Q', is manifestly reflexive and symmetric. It is also transitive: indeed, if Q, Q', Q'' are quadratic forms such that Q ~ Q' and Q' ~ Q'', there exist neutral quadratic forms M, M', N, N' such that Q ⊕ M is equivalent to Q' ⊕ M' and Q' ⊕ N to Q'' ⊕ N' ; then Q ⊕ (M ⊕ N) is equivalent to (Q ⊕ M) ⊕ N, hence to (Q' ⊕ M') ⊕ N, and also to (Q' ⊕ N) ⊕ M', hence again to (Q'' ⊕ N') ⊕ M' and to Q'' ⊕ (N' ⊕ M') ; since M ⊕ N and N' ⊕ M' are neutral, we indeed have Q ~ Q''. The relation Q ~ Q' is therefore an equivalence relation between Q and Q'. It is clear that, if Q and Q' are two non-degenerate quadratic forms of finite dimensions and equivalent, we have Q ~ Q'.

For every quadratic form Q over A, non-degenerate and of finite dimension, we shall put

(1)
$$
\theta(Q) = \tau_x(X \sim Q),
$$
and we shall say that $\theta(Q)$ is the type of Q. If Q and Q' are two quadratic forms over A, non-degenerate and of finite dimensions, the relations Q ~ Q' and $\theta(Q) = \theta(Q')$ are equivalent.

#### Proposition 1 {#alg-ix-s8-prop-1 .statement}

Let Q and Q' be two quadratic forms over A, non-degenerate and of finite dimensions. In order that Q and Q' be equivalent, it is necessary and sufficient that they have the same dimension and the same type.

The condition is obviously necessary. Suppose that it is satisfied. There then exist neutral forms N, N' such that Q ⊕ N and Q' ⊕ N' are equivalent. Since these two forms have the same dimension, the same is true of N and N', which are consequently equivalent (§ 4, no 2, cor. 2 of prop. 2). Hence Q and Q' are equivalent by virtue of Witt's theorem (§ 4, no 3, cor. 1 of th. 1).

#### Proposition 2 {#alg-ix-s8-prop-2 .statement}

The relation « there exists a quadratic form Q over A, non-degenerate and of finite dimension, such that X = θ(Q) » is collectivizing in X (Ens., chap. II, § 1, n° 4).

Indeed, let V be an infinite-dimensional vector space over A, $\mathfrak{S}$ the set of non-degenerate quadratic forms defined on the finite-dimensional subspaces of V, and $\mathfrak{W}$ the set of the $\theta(Q)$ for $Q \in \mathfrak{S}$. It is clear that every non-degenerate quadratic form $Q'$ of finite dimension over A is equivalent to at least one element of $\mathfrak{S}$; whence $\theta(Q') \in \mathfrak{W}$, which proves our assertion.

### 2. Group of types of quadratic forms.

We shall endow the set $\mathfrak{W}$ of the types of non-degenerate quadratic forms of finite dimensions over A with a commutative group structure. We shall define an addition in $\mathfrak{W}$ by the formula

$$
T + T' = \theta(T \tau T') \tag{2}
$$

This addition is commutative since $T' \tau T$ is equivalent to $T \tau T'$. It is associative because, if $T, T'$ and $T''$ are elements of $\mathfrak{W}$, we have

$$
(T + T') + T'' \sim (T + T') \tau T'' \sim (T \tau T') \tau T''
$$
$$
\sim T \tau (T' \tau T'') \sim T \tau (T' + T'') \sim T + (T' + T''),
$$
whence $(T + T') + T'' = T + (T' + T'')$ since two elements of $\mathfrak{W}$ which have the same type are equal. Moreover the addition which we have just defined possesses an identity element: it is clear indeed that all neutral forms have the same type $T_0$, namely that of the zero form of zero dimension; we see at once that $T_0$ is the identity element sought. Finally the existence, for every $T \in \mathfrak{W}$, of an element opposite to T follows at once from the following proposition:

#### Proposition 3 {#alg-ix-s8-prop-3 .statement}

Let Q be a non-degenerate quadratic form of finite dimension on a vector space V over A. Let – Q denote the quadratic form on V defined by $(-Q)(x) = -Q(x)$ ($x \in V$). Then the form $Q \tau (-Q)$ is neutral.

Indeed the restriction of $Q \tau (-Q)$ to the diagonal D of $V \times V$ is zero. The index of this form is therefore $\geqslant \frac{1}{2} \dim (V \times V)$ (§ 4, no 2, déf. 2), and consequently is equal to $\frac{1}{2} \dim (V \times V)$ (*ibid.*, formula (4)). It follows that $Q \tau (-Q)$ is neutral (*ibid.*).

This permits us to give the following definition:

#### Definition 1 {#alg-ix-s8-def-1 .statement}

*The set of types of non-degenerate quadratic forms of finite dimensions over $A$, endowed with the addition defined by (2), is called the group of types of quadratic forms, or Witt group, of $A$.*

*Remarks. —* 1) Every non-degenerate quadratic form $Q$ of finite dimension whose type is zero (i.e. such that $\theta(Q) = T_0$ with the above notation) is a neutral form. There indeed exist neutral forms $N, N'$ such that $Q \tau N$ is equivalent to $N'$. This shows that $Q$ is of even dimension, and hence that there exists a neutral form $N_1$ having the same dimension as $Q$. Since $Q$ and $N_1$ have the same type, it follows from prop. 1 that they are equivalent, and hence that $Q$ is neutral.

2) For every finite-dimensional quadratic form $Q$ over $A$, let $\delta(Q)$ denote the class modulo 2 of the dimension of $Q$. We have
$$
\delta(Q \tau Q') = \delta(Q) + \delta(Q').
$$
Since every neutral form $N$ is of even dimension, we have $\delta(N) = 0$; the relation $Q \sim Q'$ therefore entails $\delta(Q) = \delta(Q')$. Thus the restriction of $\delta$ to the group $\mathfrak{W}$ of types of quadratic forms over $A$ is a homomorphism of $\mathfrak{W}$ into the group $\mathbf{Z}/(2)$. This homomorphism is surjective when $A$ is of characteristic $\neq 2$, but is not so if $A$ is of characteristic 2, since a quadratic form of odd dimension is then degenerate, its associated bilinear form being alternating (cf. § 5).

3) Let $a$ be an element $\neq 0$ of $A$. If $N$ is a neutral form, then so is $aN$. It follows that the relation $Q \sim Q'$ entails $aQ \sim aQ'$. For every element $T$ of the group $\mathfrak{W}$, we shall put
$$
a.T = \theta(aT).
$$
We thus obtain an external composition law between the group $A^*$ of the non-zero elements of $A$ and the group $\mathfrak{W}$. The following formulas result immediately from the definition:
$$
a.(T + T') = a.T + a.T', \quad ab.T = a.(b.T)
$$
$
(a, b \text{ in } A^*, \quad T, T' \text{ in } \mathfrak{W}).
$

On the other hand, if $a, b$ and $a + b$ are in $A^*$, one does not in general have $(a + b).T = a.T + b.T$ ($T \in \mathfrak{W}$).

#### Proposition 4 {#alg-ix-s8-prop-4 .statement}

*Let Q be a non-degenerate quadratic form on a finite-dimensional vector space E over A. Suppose that A is of characteristic $\neq 2$, and let $(x_1, \ldots, x_n)$ be an orthogonal basis of V. Let $T_1$ be the type of the quadratic form $Q_1$ defined on the vector space A and such that $Q_1(1) = 1$. The type of Q is then $\sum_{i=1}^n Q(x_i) \cdot T_1$.

Indeed the form Q is equivalent to
$$(Q(x_1)Q_1) \tau \ldots \tau (Q(x_n)Q_1)$$

#### Corollary {#alg-ix-s8-n2-cor-1 .statement}

*The hypotheses and notation being those of prop. 3, the elements $a.T_1$ ($a \in A^*$) form a set of generators of the group of types of quadratic forms over A.*

To seek the structure of the group of types of quadratic forms over A is therefore to seek the $\mathbf{Z}$-linear relations which exist between the elements of the form $a.T_1$. If $b \in A^*$, the form $Q_1$ defined in prop. 4 is manifestly equivalent to $b^2Q_1$; hence $a.T_1 = ab^2.T_1$, which shows that $a.T_1$ depends only on the class of $a$ modulo the subgroup $(A^*)^2$ of squares of elements of $A^*$. Moreover, it follows from prop. 3 that we have $(-a).T_1 = -a.T_1$. However, in general there are other $\mathbf{Z}$-linear relations between the $a.T_1$ than those which follow from the relations we have just indicated.

#### Proposition 5 {#alg-ix-s8-prop-5 .statement}

*We suppose that A is a maximal ordered field. Let Q be a non-degenerate quadratic form of finite dimension over A, and $(s, t)$ its signature ($§ 7$, no 2, def. 2). Then the type of Q is $(s - t).T_1$, and the group $\mathfrak{W}$ of types of quadratic forms over A is an infinite monogenic group generated by $T_1$.

Indeed, since $A^*/(A^*)^2$ is of order 2 and $(-1).T_1 = -T_1$, $\mathfrak{W}$ is generated by $T_1$ and is therefore monogenic. For every $n > 0$, $n.T_1$ is the type of the positive non-degenerate quadratic forms of dimension $n$; since these forms are not neutral, we have $n.T_1 \neq 0$, which shows that $\mathfrak{W}$ is infinite. Finally, a form of signature $(s, t)$ is isomorphic, with the notation of prop. 4, to the direct sum of $s$ forms $Q_1$ and of $t$ forms $- Q_1$ (§ 7, n° 2, th. 1); it follows that its type is $(s - t). T_1$.

### 3. Ring of types of quadratic forms.

We shall suppose, in this no., that $A$ is a field of characteristic $\neq 2$.

Given two quadratic forms $Q, Q'$ on vector spaces $V, V'$ over $A$, we shall call tensor product of $Q$ and $Q'$, and denote by $Q \otimes Q'$ the quadratic form on $V \otimes V'$ whose associated bilinear form is the tensor product (§ 1, n° 9, def. 11) of the bilinear forms associated with $Q$ and $Q'$. It is readily seen that $Q \otimes Q'$ satisfies the relation

$$(5)$$
$$(Q \otimes Q')(x \otimes x') = Q(x)Q'(x') \quad (x \in V, x' \in V').$$

If $Q$ and $Q'$ are non-degenerate and of finite dimensions, the same is true of $Q \otimes Q'$ (§ 1, n° 9, prop. 9).

Let $Q, Q', Q''$ be quadratic forms on the vector spaces $V, V', V''$. Using the canonical isomorphism of $V \otimes V'$ onto $V' \otimes V$ (resp. of $(V \otimes V') \otimes V''$ onto $V \otimes (V' \otimes V'')$), of $(V \times V') \otimes V''$ onto $(V \otimes V'') \times (V' \otimes V'')$), one sees at once that $Q \otimes Q'$ is equivalent to $Q' \otimes Q$ (resp. $(Q \otimes Q') \otimes Q''$ to $Q \otimes (Q' \otimes Q'')$, $(Q \tau Q') \otimes Q''$ to $(Q \otimes Q'') \tau (Q' \otimes Q'')$).

Let $Q$ and $Q'$ be two non-degenerate quadratic forms of finite dimensions. If $Q$ is neutral, then so is $Q \otimes Q'$. Indeed, let $V, V'$ be the spaces on which $Q, Q'$ are defined, $2n$ and $n'$ their dimensions, and let $W$ be a totally singular subspace of dimension $n$ of $V$ (§ 4, No. 2); then, $W \otimes V'$ is a totally singular subspace, and its dimension is half that of $V \otimes V'$; it follows, as in prop. 3, that $Q \otimes Q'$ is neutral. Analogously $Q \otimes Q'$ is neutral whenever $Q'$ is neutral.

It follows from this that, if $Q, Q', Q_1, Q'_1$ are non-degenerate quadratic forms of finite dimensions over $A$, and if one assumes that $\theta(Q_1) = \theta(Q)$ and $\theta(Q'_1) = \theta(Q')$, then $\theta(Q_1 \otimes Q'_1) = \theta(Q \otimes Q')$. It is enough in fact to verify this in the case where $Q_1 = Q \tau N$ and $Q'_1 = Q' \tau N'$, $N$ and $N'$ being neutral forms; in this case $Q_1 \otimes Q'_1$ is equivalent to

$$
(Q \otimes Q') \tau (Q \otimes N' \tau Q' \otimes N \tau N \otimes N')
$$

and the second parenthesis denotes a neutral form; this proves our assertion.

Let now $\mathfrak{B}$ be the group of types of quadratic forms over $A$. Define, on the set $\mathfrak{B}$, a second law of composition, denoted multiplicatively, by the formula

(6)
$$
TT' = \theta(T \otimes T') \qquad (T, T' \text{ dans } \mathfrak{B}).
$$

It follows at once from what we have just seen that this law of composition is commutative, associative and distributive with respect to addition. It has a unit element, namely the type $T_1$ of the quadratic form $Q_1$ defined on the vector space $A$ and such that $Q_1(1) = 1$: indeed, according to (5), $Q_1 \otimes Q = Q$ for every quadratic form $Q$. The additive group $\mathfrak{B}$, endowed with the multiplication which we have just defined, is therefore a commutative ring with unit element; it is called the *ring of types of quadratic forms* of $A$ (or the *Witt ring* of $A$, when there is no danger of confusion).

#### Remark 1 {#alg-ix-s8-n3-rem-1 .statement}

It is clear that, if $a$ is an element of $A^*$, one has

(7)
$$
a . (TT') = (a . T)T' = T(a . T')
$$

whatever the elements $T, T'$ of $\mathfrak{B}$ may be. It will moreover be observed that one has $a . T = T_a T$, denoting by $T_a$ the type of the quadratic form $aQ_1$ over $A$.

#### Remark 2 {#alg-ix-s8-n3-rem-2 .statement}

Since $A$ is of characteristic $\neq 2$, every element $T$ of $\mathfrak{B}$ can be written in the form $\sum_{i=1}^n a_i . T_1$ where $a_i \in A^*$ (No. 2, prop. 4). One has

(8)
$$
(\sum_{i=1}^n a_i . T_1)(\sum_{j=1}^q b_j . T_1) = \sum_{i,j} a_i b_j . T_1 \qquad (a_i, b_j \text{ dans } A^*).
$$

#### Remark 3 {#alg-ix-s8-n3-rem-3 .statement}

Suppose that $A$ is a *maximal ordered field*. Then the ring $\mathfrak{B}$ is isomorphic to $\mathbf{Z}$ (prop. 5), the integer corresponding to the type of a form of signature $(s,\ t)$ being $s - t$ (*ibid.*). Since the tensor product of two forms $Q$, $Q'$ of signatures $(s,\ t)$, $(s',\ t')$ is a form of dimension $(s + t)\,(s' + t')$, it follows, by means of an elementary calculus, that the signature of $Q \otimes Q'$ is $(ss' + tt',\ st' + ts')$.
