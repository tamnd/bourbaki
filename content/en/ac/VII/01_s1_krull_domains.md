---
book: ac
book_title: Commutative Algebra
chapter: VII
chapter_title: DIVISORS
section: 1
section_title: Krull domains
lang: en
source: ac-i-vii
book_pages: 475-493, 545-555
pdf_pages: 0493-0511, 0563-0573
extraction: ocr
subsections:
    - "no": 1
      title: DMSORIAL IDEALS OF AN INTEGRAL DOMAIN
      page: 475
      pdf_page: 493
    - "no": 2
      title: THE MONOID STRUCTURE ON D(A)
      page: 478
      pdf_page: 496
    - "no": 3
      title: KRULL DOMAINS
      page: 480
      pdf_page: 498
    - "no": 4
      title: ESSENTIAL VALUATIONS OF A KRULL DOMAIN
      page: 482
      pdf_page: 500
    - "no": 5
      title: APPROXIMATION FOR ESSENTIAL VALUATIONS
      page: 484
      pdf_page: 502
    - "no": 6
      title: PRIME IDEALS OF HEIGHT 1 IN A KRULL DOMAIN
      page: 485
      pdf_page: 503
    - "no": 7
      title: 'APPLICATION: NEW CHARACTERIZATIONS OF DISCRETE VALUATION RINGS'
      page: 487
      pdf_page: 505
    - "no": 8
      title: THE INTEGRAL CLOSURE OF A KRULL DOMAIN IN A FINITE EXTENSION OF ITS FIELD OF FRACTIONS
      page: 487
      pdf_page: 505
    - "no": 9
      title: POLYNOMIAL RINGS OVER A KRULL DOMAIN
      page: 488
      pdf_page: 506
    - "no": 10
      title: DIVISOR CLASSES IN KRULL DOMAINS
      page: 489
      pdf_page: 507
statements: 41
exercises: 32
content_sha256: 9bef6d28f362c12836cf4563473a98aa78f886c75e3bc526c03329214a3be918
---

## 1. KRULL DOMAINS

### 1. DMSORIAL IDEALS OF AN INTEGRAL DOMAIN

#### Definition 1 {#ac-vii-s1-def-1 .statement}

Let $A$ be an integral domain and $K$ its field of fractions. Every sub-A-module $a$ of $K$ such that there exists an element $d \neq 0$ in $A$ for which $da \subset A$ is called a fractional ideal $\mathfrak{d}$ of $A$ (or of $K$, by an abuse of language).

Every finitely generated sub-A-module $a$ of $K$ is a fractional ideal: for if $(a_i)_{1 \leq i \leq n}$ is a system of generators of $a$, we may write $a_i = b_i/d_i$, where $b_i \in A$, $d_i \in A$ and $d, \neq 0$; if $d = d_1 \ldots d_n$, clearly $da \subset A$. In particular the monogenous sub-A-modules of $K$ are fractional ideals (recall that they have been called fractional principal ideals in Algebra, Chapter VI, § 1, no. 5). If $A$ is Noetherian, every fractional ideal is afinitely generated A-module. Every sub-A-module of a fractional ideal of $A$ is a fractional ideal. Every ideal of $A$ is a fractional ideal; to avoid confusion, these will also be called the integral ideals of $A$.

We denote by $I(A)$ the set of non-zero fractional ideals of $A$. Given two elements $a, b$ of $I(A)$, we shall write $a \prec b$ (or $b \succ a$) for the relation "every fractional principal ideal containing $a$ also contains $b$"; clearly this relation is a preordering on $I(A)$. Let $R$ denote the associated equivalence relation "$a \prec b$ and $b \prec a$" (Set Theory, Chapter III, § 1, no. 2) and $D(A)$ the quotient set $I(A)/R$; we shall say that the elements of $D(A)$ are the divisors of $A$ and, for every fractional ideal $a \in I(A)$, we shall denote by $\operatorname{div} a$ (or $\operatorname{div}, a$) the canonical image of $a$ in $D(A)$ and we shall say that $\operatorname{div} a$ is the divisor $\mathfrak{d}$ of $a$; if $a = Ax$ is a fractional principal ideal, we write div(x) instead of div(Ax) and div(x) is called the divisor of x; the elements of D(A) of the form div(x) are called principal divisors. By taking the quotient, the preordering $\prec$ on I(A) defines on D(A) an ordering which we shall denote by $\leqslant$.

For all $a \in I(A)$ there exists by hypothesis some $d \neq 0$ in A such that $a \subset Ad - 1$; the intersection $\tilde{a}$ of the fractional principal ideals containing a is therefore an element of I(A). Clearly the relation $a \prec b$ is equivalent to the relation $\tilde{a} \supset 6$; the relation $a \supset b$ therefore implies $a \prec b$. For two elements $a, b$ of I(A) to be equivalent modulo R, it is necessary and sufficient that $\tilde{a} = 6$.

#### Definition 2 {#ac-vii-s1-def-2 .statement}

*Every element a of I(A) such that $a = \tilde{a}$ is called a divisorial fractional ideal of A.*

In other words a divisorial ideal is just a non-zero intersection of a non-empty family of fractional principal ideals. Every non-zero intersection of divisorial ideals is a divisorial ideal. If a is divisorial, so is ax for all $x \in K^*$, the mapping $b \mapsto bx$ being a bijection of the set of fractional principal ideals onto itself, For all $a \in I(A)$, 6 is the least divisorial ideal containing a and is equivalent to a modulo R. Moreover, if $b$ is a divisorial ideal equivalent to a modulo R, then $\tilde{a} = 6 = b$. Hence 5 is the unique divisorial ideal $b$ such that div $a =$ div $b$ (in other words, the restriction of the mapping $a \mapsto$ div $a$ to the set of divisorial ideals is injective).

Let a and b be two fractional ideals of K. Recall (Chapter I, § 2, no. 10) that $b : a$ denotes the set of $x \in K$ such that $xa \subset b$; this is obviously an A-module; if $b \in I(A)$ and $a \in I(A)$, then $b : a \in I(A)$; for if $d$ is a non-zero element of A such that $db \subset A$ and $da \subset A$ and $a$ is a non-zero element of $A \cap a$, then $da(b : a) \subset A$; on the other hand, if $b \neq 0$ belongs to $b$, then $bda \subset b$, hence $bd \in b : a$ and $b : a \neq 0$.

The definition of $b : a$ can also be written:

$$
(1) \quad b : a = \bigcap_{x \in a, x \neq 0} b x^{-1}.
$$

#### Proposition 1 {#ac-vii-s1-prop-1 .statement}

(a) *If b is a divisorial ideal and $a \in I(A)$, $b : a$ is divisorial.*

(b) *Let a, b be in I(A). In order that div $a =$ div $b$, it is necessary and sufficient that $A : a = A : b$.*

(c) *For all $a \in I(A)$, $6 = A : (A : a)$.*

Assertion (a) follows immediately from equation (1) since, if $b$ is divisorial, so is $b x^{-1}$ for all $x \neq 0$.

To show (b), let $P(a)$ denote the set of fractional principal ideals containing a; the relation $Ax \in P(a)$ is equivalent to $x^{-1} a \subset A$ and hence to $x^{-1} \in A : a$. As the relation div $a =$ div $b$ is by definition equivalent to $P(a) = P(b)$, it is also equivalent to $A : a = A : b$.

Finally, as $a(A : a) \subset A, a \subset A : (A : a)$. Replacing $a$ by $A : a$ in this formula, it is seen that $A : a \subset A : (A : (A : a))$; on the other hand, the relation $a \subset A : (A : a)$ implies
$$
A : a \supset A : (A : (A : a)).
$$
Therefore $A : a = A : (A : (A : a))$ and it follows from (b) that $\operatorname{div} a = \operatorname{div}(A : (A : a))$
As $A : (A : a)$ is divisorial by (a), certainly $6 = A : (A : a)$, which proves (c).

#### Remark {#ac-vii-s1-n1-rem-1 .statement}

In the course of the above proof it has been proved that $A : a = A : (A : (A : a))$ for every ideal $a \in I(A)$, which is a special case of *Set Theory*, Chapter 111, § 1, no. 5, Proposition 2.

#### Proposition 2 {#ac-vii-s1-prop-2 .statement}

(i) *In $D(A)$ every non-empty set bounded above admits a least upper bound. More precisely, if $(a_i)$ is a non-empty family of elements of $I(A)$ which is bounded above, then*
$$
\sup(\operatorname{div} a_i) = \operatorname{div}\left( \bigcap_i 5_i \right).
$$
(ii) *In $D(A)$ every non-empty set bounded below admits a greatest lower bound. More precisely, if $(a_i)$ is a non-empty family of elements of $I(A)$ which is bounded below, then*
$$
\inf(\operatorname{div} a_i) = \operatorname{div}\left( \sum_i a_i \right).
$$
(iii) *The set $D(A)$ is a lattice.*

Let $(a_i)$ be a non-empty family of elements of $I(A)$ which is bounded above. To say that a divisorial ideal $b$ bounds this family above amounts to saying that it is contained in all the $a_i$, that is that $b$ is contained in $\bigcap_i 6_i$. Hence $\bigcap_i a_i \neq (0)$ and $\bigcap_i 6_i$, is therefore a divisorial ideal, which shows (i).

Now let $(6_i)$ be a non-empty family of elements of $I(A)$ which is bounded below. To say that a divisorial ideal $b$ bounds this family below means that it contains all the $a_i$, that is (since $b$ is divisorial) that it contains all the $a_i$, or also that $b \supset \sum_i a_i$. This proves (ii).

Finally, to prove (iii) it is sufficient by (i) and (ii) to prove that, if $a, b$ are in $I(A)$, the set $\{a, b\}$ is bounded both above and below in $I(A)$; now it is bounded above by $a \cap b$ (which is distinct from $(0)$). It is bounded below by $a + b$, for $a + b \in I(A)$: if $d$ and $d'$ are non-zero elements of $A$ such that $da \subset A$ and $d'b \subset A$, then $dd'(a + b) \subset A$.

#### Corollary {#ac-vii-s1-n1-cor-1 .statement}

*If $x, y$ and $x + y$ are in $K^*$, then $\operatorname{div}(x + y) \geq \inf(\operatorname{div}(x), \operatorname{div}(y))$.*

$A(x + y) \subset Ax + Ay$ and hence $\operatorname{div}(x + y) \geq \operatorname{div}(Ax + Ay)$.

### 2. THE MONOID STRUCTURE ON D(A)

#### Proposition 3 {#ac-vii-s1-prop-3 .statement}

Let $a, a', b, b'$ be elements of $I(A)$. The relations $a > a'$ and $b > b'$ imply $ab > a'b'$.

We may restrict our attention to the case where $b = b'$. Then let $Ax$ be a fractional principal ideal containing $a'b$; for every non-zero element $y$ of $b$, $Ax \supset a'y$ and hence $Axy^{-1} \supset a'$, whence $Axy^{-1} \supset a$ and $Ax \supset ay$. Varying $y$, it is seen that $Ax \supset ab$, whence $ab > a'b$.

It follows from Proposition 3 that multiplication on $I(A)$ defines, by passing to the quotient, a law of composition on $D(A)$ which is obviously associative and commutative. It is written additively so that we may write:

$$
\text{div}(ab) = \text{div } a + \text{div } b,
$$

for $a, b$ in $I(A)$. Clearly $\text{div}(1)$ is an identity element for this addition; this element is denoted by 0. Proposition 3 proves further that the order structure on $D(A)$ is *compatible* with this addition (*Algebra*, Chapter VI, § 1, no. 1) and, more precisely (no. 1, Proposition 2 (ii)):

$$
\inf(\text{div } a + \text{div } b, \text{div } a + \text{div } c) = \inf(\text{div}(ab), \text{div}(ac)) = \text{div}(ab + ac)
= \text{div}(a(b + c)) = \text{div} a + \text{div}(b + c) = \text{div} a + \inf(\text{div } b, \text{div } c).
$$

For a fractional ideal $a \neq 0$ to be such that $\text{div } a \geq 0$ in $D(A)$, it is necessary and sufficient that $a \subset A$ (in other words, that $a$ be an *integral* ideal of $A$).

For two elements $x, y$ of $K^*$, the relation $\text{div}(x) = \text{div}(y)$ is equivalent to $Ax = Ay$; the set of principal divisors of $A$ with the order relation and the monoid law induced by that on $D(A)$ is an *ordered group* canonically isomorphic to the multiplicative group of fractional principal ideals ordered by the opposite order relation to inclusion (*Algebra*, Chapter VI, § 1, no. 5). The relation $S$ between two elements $P, Q$ of $D(A)$:

"there exists $x \in K^*$ such that $P = Q + \text{div}(x)$"

is therefore an equivalence relation since the relation $P = Q + \text{div}(x)$ is equivalent to $Q = P + \text{div}(x^{-1})$; if $P$ and $Q$ are congruent modulo $S$, they are called *equivalent divisors* of $A$. Clearly moreover the relation $S$ is compatible with the law of the monoid $D(A)$ and the latter therefore defines, by taking quotients, a monoid structure on $D(A)/S$; this monoid is called the *divisor class monoid of A*.

#### Proposition 4 {#ac-vii-s1-prop-4 .statement}

Let $a, b$ be two divisorial fractional ideals of $A$. The following properties are equivalent:
(a) $\text{div } a$ and $\text{div } b$ are equivalent divisors;
(b) there exists $x \in K^*$ such that $b = xa$.

If $\operatorname{div} b = \operatorname{div} a + \operatorname{div}(x)$ for some $x \in K^*$, then $\operatorname{div} b = \operatorname{div}(xa)$ and, as $b$ and $xa$ are divisorial, $b = xa$, which proves the proposition.

Let $a$ be an invertible fractional ideal (Chapter II, § 5, no. 6); then $a = A : (A : a)$ (*loc. cit.*, Proposition 10) and hence $a$ is *divisorial* (no. 1, Proposition 1). The group $J(A)$ of invertible fractional ideals is therefore identified with a subgroup of the monoid $D(A)$ and the canonical image of $J(A)$ in $D(A)/S$ with the group of classes of *projective* $A$-modules of *rank* 1 (Chapter II, § 5, no. 7, Corollary 2 to Proposition 12 and *Remark* 1).

#### Theorem 1 {#ac-vii-s1-thm-1 .statement}

*Let $A$ be an integral domain. For the monoid $D(A)$ of divisors of $A$ to be a group, it is necessary and sufficient that $A$ be completely integrally closed.*

Suppose that $D(A)$ is a group. Let $x \in K$; suppose that $A[x]$ is contained in a finitely generated sub-$A$-module of $K$. Then we have seen (no. 1) that $a = A[x]$ is an element of $I(A)$. Then $xa \subset a$ and hence $\operatorname{div}(x) + \operatorname{div} a \geq \operatorname{div} a$. Since $D(A)$ is an ordered group, we conclude that $\operatorname{div}(x) \geq 0$, whence $x \in A$. Thus $A$ is completely integrally closed (Chapter V, § 1, no. **4**, Definition 5).

Conversely, suppose that $A$ is completely integrally closed. Let $a$ be a divisorial ideal. We shall show that $\operatorname{div} a + \operatorname{div}(A : a) = 0$, which will prove that $D(A)$ is a group. As $a(A : a) \subset A$, it suffices (no. 1) to verify that every fractional principal ideal $Ax^{-1}$ which contains $a(A : a)$ also contains $A$. Now, for $y \in K^*$, the relation $Ay \supset a$ implies $y^{-1} \in A : a$, whence $y^{-1}a \subset a(A : a) \subset Ax^{-1}$ and hence $xa \subset Ay$. As $a$ is divisorial, we deduce that $xa \subset a$, whence $x^n a \subset a$ for all $n \in \mathbf{N}$. There exist elements $x_0, x_1$ of $K^*$ such that $Ax_0 \subset a \subset Ax_1$; therefore $x^n x_0 \in Ax_1$, whence $x^n \in Ax_1 x_0^{-1}$. As $A$ is completely integrally closed, $x \in A$, that is $Ax^{-1} \supset A$, which completes the proof.

Note that, if $A$ is completely integrally closed (and even Noetherian), a divisorial ideal of $A$ is not necessarily invertible, in other words, in general $J(A) \neq D(A)$ (Exercise 2 and § 3, no. 2, Proposition 1).

#### Corollary {#ac-vii-s1-n2-cor-1 .statement}

*Let $A$ be a completely integrally closed domain and $a$ a divisorial fractional ideal of $A$. Then, for every fractional ideal $b \neq 0$ of $A$, $\operatorname{div}(a : b) = \operatorname{div} a - \operatorname{div} b$*

By virtue of formula (1) of no. 1:

$$
\operatorname{div}(a : b) = \operatorname{div}\left( \bigcap_{y \in b, y \neq 0} y^{-1}a \right) = \sup_{y \in b, y \neq 0} \operatorname{div}(y^{-1}a)
$$

taking account of Proposition 2 and the fact that the fractional ideals $y^{-1}a$ are divisorial. But since $D(A)$ is an ordered group (*Algebra*, Chapter VI, § 1, no. 8):

$$
\sup_{y \in b, y \neq 0} \operatorname{div}(y^{-1}a) = \sup_{y \in b, y \neq 0} (\operatorname{div} a - \operatorname{div}(y)) \\
= \operatorname{div} a - \inf_{y \in b, y \neq 0} \operatorname{div}(y) = \operatorname{div} a - \operatorname{div} b.
$$

### 3. KRULL DOMAINS

#### Definition 3 {#ac-vii-s1-def-3 .statement}

A n integral domain $A$ is called a Krull domain if there exists a family $(v_i)_{i \in I}$ of valuations on the field of fractions $K$ of $A$ with the following properties:
(AK,) the valuations $v_i$ are discrete;
(AK,,) the intersection of the rings & the $v_i$ is $A$;
(AK,,,) for all $x \in K^*$, the set of indices $t \in I$ such that $v_t(x) \neq 0$ is finite.

It obviously suffices to verify condition (AK$_{III}$) for the elements $x$ of $A - (0)$.

Examples
(1) Every discrete valuation ring is a Krull domain.
(2) More generally, every principal ideal domain $A$ is a Krull domain. For let $(p_i)_{i \in I}$ be a representative system of extremal elements of $A$ and let $v_i$ be the valuation on the field of fractions of $A$ defined by $p_i$ (Chapter VI, § 3, no. 3, Example 4). It is immediately seen that the family $(v_i)_{i \in I}$ satisfies properties (AK$_I$), (AK$_II$) and (AK$_{III}$).
(3) Let $F$ be a field and $(R_i)_{1 \leq i \leq n}$ a finite family of subrings of $F$ which are Krull domains. Then their intersection $S = \bigcap_{j=1}^n R_j$, is a Krull domain. For $1 \leq j \leq n$ let $(v_{j,t})_{t \in I_j}$ be a family of valuations on the field of fractions of $R_j$, satisfying (AK$_I$), (AK$_{II}$), (AK$_{III}$) (where $A$ is replaced by $R_j$). Let $w_{j,t}$ denote the restriction of $v_{j,t}$ to the field of fractionsof $S$. Then the family $(v_{j,t})_{1 \leq j \leq n, t \in I_j}$ obviously satisfies (AK$_{II}$) (where $A$ is replaced by $S$) and also (AK$_{III}$) since the set of indices$j$ is finite. The valuations $w_{j,t}$ are either discrete or improper. By retaining only those which are discrete, a family is obtained which obviously satisfies (AK$_I$), (AK$_{II}$) and (AK$_{,,}$) (where $A$ is replaced by $S$). Hence $S$ is certainly a Krull domain.
(4) In particular, if $A$ is a Krull domain and $K'$ a subfield of the field of fractions $K$ of $A$, $K' \cap A$ is a Krull domain.

#### Theorem 2 {#ac-vii-s1-thm-2 .statement}

Let $A$ be an integral domain. For $A$ to be a Krull domain, it is necessary and sufficient that the twofollowing conditions be satisfied:
(a) $A$ is completely integrally closed;
(b) every non-empty family of divisorial integral ideals of $A$ admits a maximal element (with respect to the relation $\subset$).
Moreover, if $P(A)$ is the set of extremal elements of $D(A)$, $P(A)$ is then a basis of the $\mathbf{Z}$-module $D(A)$ and the positive elements of $D(A)$ are the linear combinations of the elements of $P(A)$ with coefficients $\geq 0$.

Let $A$ be a Krull domain. It is completely integrally closed (Chapter VI, § 4, no. 5, Corollary to Proposition 9). Let $(v_i)_{i \in I}$ be a family of valuations on the field of fractions $K$ of $A$ satisfying (AK$_I$), (AK$_{II}$) and (AK$_{III}$). The $v_i$ may be assumed to be normed (Chapter VI, § 3, no. 6, Definition 3). For all $a \in I(A)$, we shall write:

$$
v_t(a) = \sup_{a \subset Ax} (v_t(x));
$$

then $v_t(a) \in \mathbf{Z}$, for, if $a$ is a non-zero element of $a$, the relation $Ax \supset Aa$ implies that $v_t(x) \leq v_t(a)$ (by (AK$_{III}$)), which shows that the family of $v_t(x)$ ($a \subset Ax$) is bounded above. We establish the following properties:

(1) *Let $a$ be a divisorial fractional ideal; in order that $y \in a$, it is necessary and sufficient that $v_t(y) \geq v_t(a)$ for all $t \in I$.*

As $a$ is divisorial, the relation $y \in a$ is equivalent to the relation "“$a \subset Ax$ implies $y \in Ax$”. Now, by (AK,,), the relation $y \in Ax$ is equivalent to “$v_t(y) \geq v_t(x)$ for all $t \in I$”. Whence (1).

(2) *Let $a$ and $b$ be two divisorial fractional ideals of $A$; in order that $a \subset b$, it is necessary and sufficient that $v_t(a) \geq v_t(b)$ for all $t \in I$.*

This follows immediately from property (1).

(3) *If $x \in K^*$, then $v_t(Ax) = v_t(x)$.*

If $Ay \supset Ax$, then $v_t(y) \leq v_t(x)$ by (AK,,) and the minimum value of $v_t(y)$ is taken at $y = x$.

(4) *For all $a \in I(A)$, the indices $t \in I$ such that $v_t(a) \neq 0$ are finite in number.*

There exist $x, y$ in $K^*$ such that $Ax \subset a \subset Ay$. By properties (2) and (3), $v_t(x) \geq v_t(a) \geq v_t(y)$ for all $t \in I$. It then sufficesto apply (AK$_{III}$).

We have therefore shown the following lemma:

#### Lemma 1 {#ac-vii-s1-lem-1 .statement}

*If $A$ is a Krull domain and $(v_t)_t$, is a family of normed valuations on $K$ satisfying (AK, ), (AK,,) and (AK$_{III}$), the mapping $a \mapsto (v_t(a))_{t \in I}$ is a decreasing injective mapping of the set of divisorial integer ideals of $A$ (ordered by $\subset$) to the set of positive elements & the ordered group the direct sum $\mathbf{Z}^{(I)}$.*

This being so, every non-empty set of positive elements of $\mathbf{Z}^{(I)}$ has a minimal element (*Algebra*, Chapter VI, § 1, no. 13, Theorem 2). Hence $A$ certainly satisfies property (b) of the statement.

Conversely, let $A$ be an integral domain satisfying properties (a) and (b) of the statement. Since $A$ is completely integrally closed, $D(A)$ is an ordered group (no. 2, Theorem 1). This group is a lattice (no. 1, Proposition 2). By condition (b) of the statement, every non-empty family of positive elements of $D(A)$ has a minimal element. Let $P(A)$ be the set of extremal elements of $D(A)$. Then (*Algebra*, Chapter VI, § 1, no. 13, Theorem 2) $P(A)$ is a basis of the $\mathbf{Z}$-module $D(A)$ and the positive elements of $D(A)$ are the linear combinations with positive integer coefficients of the elements of $P(A)$.

Thus, for $x \in K^*$, rational integers $v_P(x)$ are defined (for $P \in P(A)$) by writing:

$$
\text{div}(x) = \sum_{P \in P(A)} v_P(x) \cdot P.
$$

We also write $v_P(0) = +\infty$.

From the relations

$$
\text{div}(xy) = \text{div}(x) + \text{div}(y)
$$

and

$$
\text{div}(x + y) \geq \inf(\text{div}(x), \text{div}(y)),
$$

for $x, y$ and $x + y$ in $K^*$, we deduce that the $v_P$ are *discrete valuations* on $K$. In order that $x \in A$, it is necessary and sufficient that $\text{div}(x) \geq 0$, that is that $v_P(x) \geq 0$ for all $P \in P(A)$. Thus the $v_P$ satisfy conditions (AK$_1$) and (AK$_{11}$) and obviously also (AK$_{III}$).

#### Corollary {#ac-vii-s1-n3-cor-1 .statement}

*For a Noetherian ring to be a Krull domain, it is necessary and sufficient that it be an integrally closed domain.*

An integrally closed Noetherian domain is completely integrally closed (Chapter V, § 1, no. 4).

There are non-Noetherian Krull domains, for example the polynomial ring $K[X_n]_{n \in \mathbf{N}}$ over a field $K$ in an infinity of indeterminates (cf. Exercise 8).

### 4. ESSENTIAL VALUATIONS OF A KRULL DOMAIN

Let $A$ be a Krull domain and $K$ its field of fractions. The valuations defined by formula (4) of no. 3 (for $x \in K^*$) are called the *essential valuations* of $K$ (*or* $A$).

We have remarked in the course of the proof of Theorem 2 that the valuations $v_P$ satisfy properties (AK$_1$), (AK$_2$) and (AK$_{III}$) of Definition 3. Moreover, these discrete valuations $v_P$ are *normed*: for every extremal divisor $P \in P(A)$, $P < 2P$ and hence, if $a$ and $b$ are the divisorial ideals corresponding to $P$ and $2P$, then $a \supseteq b$ and $a \neq b$; for $x \in a - b$, $\text{div}(x) \geq P$ and $\text{div}(x) \not\geq 2P$, whence $v_P(x) = 1$, which proves our assertion.

#### Proposition 5 {#ac-vii-s1-prop-5 .statement}

*Let $A$ be a Krull domain, $K$ its field of fractions and $(v_P)_{P \in P(A)}$ the family of its essential valuations. Let $(n_P)_{P \in P(A)}$ be a family of rational integers which are zero except for a finite number of indices. Then the set of $x \in K$ such that $v_P(x) \geq n_P$ for all $P \in P(A)$ is the divisorial ideal $a$ of $A$ such that $\text{div } a = \sum_{P \in P(A)} n_P \cdot P$.*

Let $x \in K^*$. In order that $x \in a$, it is necessary and sufficient that $Ax \subset a$, hence that $\text{div}(x) \geq \text{div } a$ and hence, by (4), that $v_P(x) \geq n_P$ for all $P \in P(A)$.

#### Proposition 6 {#ac-vii-s1-prop-6 .statement}

Let $A$ be a Krull domain, $K$ its field of fractions, $(v_t)_{t \in I}$ a family of valuations on $K$ with the properties of Definition 3 and $A$, the ring of $v_t$. Let $S$ be a multiplicative subset of $A$ not containing $0$ and $J$ the set of indices $t \in I$ such that $v_t$ is zero on $S$. Then $S^{-1}A = \bigcap_{t \in J} A_t$; in particular $S^{-1}A$ is a Krull domain.

We write $B = \bigcap_{t \in J} A_t$. Then $S^{-1} \subset B$ and $A \subset B$ and hence $S^{-1}A \subset B$. Conversely, let $x \in B$. Let $J'$ denote the finite set of indices $t$ such that $v_t(x) < 0$. If $t \in J'$, then $x \notin A_t$, hence $t \notin J$ and hence there exists $s_t \in S$ such that $v_t(s_t) > 0$. Let $n(t)$ be an integer $> 0$ such that $v_t(s_t^{n(t)}x) \geq 0$; we write $s = \prod_{t \in J'} s_t^{n(t)}$. Then $v_t(sx) \geq 0$ for all $t \in I$ and hence $sx \in A$ and $x \in S^{-1}A$. Thus $B = S^{-1}A$.

#### Corollary 1 {#ac-vii-s1-prop-6-cor-1 .statement}

Let $P$ be an extremal divisor of $A$ and $p$ the corresponding divisorial ideal. Then $p$ is prime, the ring of $v_P$ is $A$, and the residue field of $v_P$ is identified with the field of fractions of $A/p$.

Let $S = A - p$. By Proposition 5, $v_P$ is zero on $S$ and $> 0$ on $p$. Hence $p$ is the intersection of $A$ and the ideal of $v_P$ and is therefore prime. On the other hand, for every extremal divisor $Q \neq P$, $Q \not\subset P$ and hence the divisorial ideal $q$ corresponding to $Q$ is not contained in $p$; thus $q \cap S \neq \varnothing$ and hence, by Proposition 5, $v_Q$ is not zero on $S$. This being so, the corollary follows from Proposition 6 and Chapter II, § 3, no. 1, Proposition 3.

#### Corollary 2 {#ac-vii-s1-prop-6-cor-2 .statement}

Let $A$ be a Krull domain, $K$ its field of fractions and $(v_t)_{t \in I}$ a family of valuations with the properties of Definition 3. Then every essential valuation of $A$ is equivalent to one of the $v_t$.

Let $P$ be an extremal divisor of $A$ and $p$ the corresponding divisorial ideal. By Corollary 1, Proposition 5, Lemma 1 and assertion (1) in the proof of Theorem 2, no. 3, there exists $t \in I$ such that the ring $A_t$ of $v_t$ contains the ring $A$, of $v_P$. As $v_t$ and $v_P$ are of height 1, they are therefore equivalent (Chapter VI, § 4, no. 5, Proposition 6).

#### Proposition 7 {#ac-vii-s1-prop-7 .statement}

Let $A$ be a Krull domain, $(v_P)_{P \in P(A)}$ the family of its essential valuations and $a \in I(A)$. Then the coefficient of $P$ in $\operatorname{div} a$ is $\inf_{y \in a} (v_P(y))$. If $p$ is the divisorial prime ideal corresponding to the extremal divisor $P$, then $aA_p = \tilde{a}A_p$.

As $a = \sum_{y \in a} Ax$, Proposition 2 (b) (no. 1) shows that $\operatorname{div}(a) = \inf_{x \in a} (\operatorname{div}(Ax))$, whence our first assertion. The second follows immediately, since $\operatorname{div} \tilde{a} = \operatorname{div} a$ and $A_p$ is the ring of the discrete valuation $v_P$.

#### Proposition 8 {#ac-vii-s1-prop-8 .statement}

Let $A$ be an integrally closed Noetherian domain.
(a) Let $P$ be an extremal divisor of $A$ and $p$ the corresponding divisorial prime ideal;

for $n \in \mathbf{N}$, let $p^{(n)} = p^n A_p \cap A$; then $p^{(n)}$ is the set of $x \in A$ such that $v_p(x) \geq n$ and is a $p$-primary ideal.

(b) Let $a$ be a divisorial integral ideal, $n_1 P_1 + \ldots + n_r P_r$ the divisor of $a$ (the $P_i$ being distinct extremal divisors) and $p_i$ the divisorial prime ideal corresponding to $P_i$. Then $a = \bigcap_{i=1}^r p_i^{(n_i)}$ is the unique reduced primary decomposition of $a$ and the $p_i$ are not immersed.

By Corollary 1 to Proposition 6, the relation $x \in p^n A_p = (pA_p)^n$ is equivalent to $v_p(x) \geq n$; on the other hand, as $A$, is a discrete valuation ring, $(pA_p)^n$ is $(pA_p)$-primary (Chapter IV, § 2, no. 1, Example 4) and hence $p^{(n)}$ is $p$-primary (Chapter IV, § 2, no. 1, Proposition 3); this shows (a). Proposition 5 certainly shows that $a = \bigcap_{i=1}^r p_i^{(n_i)}$. As $p_i \not\subset p_j$ for $i \neq j$ this primary decomposition is reduced: For if $p_i^{(n_i)} \supset \bigcap_{j \neq i} p_j^{(n_j)} \supset \prod_{j \neq i} p_j^{(n_j)}$, $p_{ji}$ would contain one of the $p_j$ for $j \neq i$ (Chapter II, § 1, no. 1, Proposition 1). The uniqueness follows from Chapter IV, § 2, no. 3, Proposition 5.

### 5. APPROXIMATION FOR ESSENTIAL VALUATIONS

As the essential valuations of a Krull domain are discrete and normed, no two of them are equivalent and hence they are independent (Chapter VI, § 7, no. 2). Corollary 2 to the approximation theorem (loc. cit., Theorem 1) may therefore be applied to them: given some $n_i \in \mathbf{Z}$ and some essential valuations $v_i$ finite in number and distinct, there exists $x \in K$ such that $v_i(x) = n_i$ for all $i$. But here there is a more precise result:

#### Proposition 9 {#ac-vii-s1-prop-9 .statement}

Let $v_1, \ldots, v_r$ be distinct essential valuations of a Krull domain $A$ and $n_1, \ldots, n_r$ rational integers. There exists an element $x$ of the field of fractions $K$ of $A$ such $v_i(x) = n_i$ for $1 \leq i \leq r$ and $v(x) \geq 0$ for every essential valuation $v$ of $A$ distinct from $v_1, \ldots, v_r$.

Let $p_1, \ldots, p_r$ be the divisorial ideals of $A$ corresponding to the valuations $v_1, \ldots, v_r$. There exists $y \in K$ such that $v_i(y) = n_i$ for $1 \leq i \leq r$ (Chapter VI, § 7, no. 2, Corollary 1 to Theorem 1). The essential valuations $w_1, \ldots, w_s$ of $A$ distinct from the $v_i$ for which the integer $w_j(y) = -m_j$ is $< 0$ are finite in number; let $q_1, \ldots, q_s$ be the corresponding ideals. There exists no inclusion relation between $p_1, \ldots, p_r, q_1, \ldots, q_s$ since these ideals correspond to extremal divisors and these ideals are prime (Corollary 1 to Proposition 6). Hence the integral ideal $a = q_1^{m_1} \ldots q_s^{m_s}$ is contained in none of the $p_i$ (Chapter 11, § 1, no. 1, Proposition 1) and is therefore not contained in their union (loc. cit., Proposition 2). Therefore there exists $z \in a$ such that $z \notin p_i$ for $1 \leq i \leq r$; then $v_1(z) = \cdots = v_r(z) = 0$ and $w_j(z) \geq m_j$ for $1 \leq j \leq s$; hence the element $x = yz$ solves the problem.

#### Corollary 1 {#ac-vii-s1-prop-9-cor-1 .statement}

Let $\mathbf{A}$ be a Krull domain, $\mathbf{K}$ its field of fractions and $\mathbf{a}, \mathbf{b}$ and $c$ three divisorial fractional ideals of $\mathbf{A}$ such that $\mathbf{a} \subset \mathbf{b}$. There exists $x \in \mathbf{K}$ such that $\mathbf{a} = \mathbf{b} \cap x\mathbf{c}$.

Let $(v_t)_{t \in I}$ be the family of essential valuations of $\mathbf{A}$ and let $(m,)$ (resp. $(n_t), (p_t)$) be the family of rational integers (zero except for a finite number of indices) such that $\mathbf{a}$ (resp. $\mathbf{b}, c$) is the set of $x \in \mathbf{K}$ for which $v(x_t) \geq m$, (resp. $n_t, p_t$) for all $t \in I$ (Proposition 5, no. 4). The set $\mathbf{J}$ of $t \in I$ such that $m_t > n_t$ is finite. As $p_t = m_t = 0$ except for a finite number of indices, Proposition 9 shows that there exists $x \in \mathbf{K}^*$ such that $v_t(x^{-1}) + m_t = p_t$ for $t \in \mathbf{J}$ and
$$
v_t(x^{-1}) + m_t \geq p_t
$$
for $t \in I - \mathbf{J}$. Then, for all $t \in I$, $m_t = \sup(n_t, v_t(x) + p_t)$. Whence $\mathbf{a} = \mathbf{b} \cap x\mathbf{c}$.

#### Corollary 2 {#ac-vii-s1-prop-9-cor-2 .statement}

Let $\mathbf{A}$ be a Krull domain. For a fractional ideal $\mathbf{a}$ of $\mathbf{A}$ to be divisorial, it is necessary and sufficient that it be the intersection of two fractional principal ideals.

The sufficiency is obvious (no. 1, Definition 2). The necessity follows from Corollary 1: take $b$ and $c$ to be principal and such that $b \supseteq a$.

### 6. PRIME IDEALS OF HEIGHT 1 IN A KRULL DOMAIN

#### Definition 4 {#ac-vii-s1-def-4 .statement}

Let $\mathbf{A}$ be an integral domain. A prime ideal $\mathfrak{p}$ of $\mathbf{A}$ is said to be of height 1 if it is minimal among the non-zero prime ideals of $\mathbf{A}$.

We shall also say that the ideal $(0)$ is of height 0; a prime ideal of height $\leq 1$ is therefore by definition equal to $(0)$ or of height 1.

We shall define below, in a general way, the height of a prime ideal.

#### Theorem 3 {#ac-vii-s1-thm-3 .statement}

Let $\mathbf{A}$ be a Krull domain and $\mathfrak{p}$ an integral ideal of $\mathbf{A}$. For $\mathfrak{p}$ to be the divisorial ideal corresponding to an extremal divisor, it is necessary and sufficient that $\mathfrak{p}$ be a prime ideal of height 1.

If $\mathfrak{p}$ is the divisorial ideal corresponding to an extremal divisor, we know (no. 4, Corollary 1 to Proposition 6) that $\mathfrak{p}$ is prime and that $\mathbf{A}_\mathfrak{p}$ is a discrete valuation ring; as $\mathbf{A}_\mathfrak{p}$ has no prime ideals other than $(0)$ and $\mathfrak{p}\mathbf{A}_\mathfrak{p}$, $(0)$ and $\mathfrak{p}$ are the only prime ideals of $\mathbf{A}$ contained in $\mathfrak{p}$ (Chapter II, § 3, no. 1, Proposition 3); hence $\mathfrak{p}$ is of height 1. Conversely, we shall show first that every prime ideal $\mathfrak{p} \neq (0)$ of $\mathbf{A}$ contains a divisorial prime ideal $\mathfrak{q}$ corresponding to an extremal divisor: for, as $\mathbf{A}_\mathfrak{p} \neq K$, $\mathbf{A}_\mathfrak{p}$ is the intersection of a non-empty family $(\mathbf{A}_t)$ of essential valuation rings (no. 4, Proposition 6); each $\mathbf{A}_t$ is of the form $\mathbf{A}_{\mathfrak{q}_t}$ (no. 4, Corollary 1 to Proposition 6) and from $\mathbf{A}_\mathfrak{p} \subset \mathbf{A}_{\mathfrak{q}_t}$ we deduce that $\mathfrak{q}_t \subset \mathfrak{p}$. Thus, if $\mathfrak{p}$ is of height 1, then $\mathfrak{p} = \mathfrak{q}$, which shows that $\mathfrak{p}$ is the divisorial ideal corresponding to an extremal divisor.

#### Corollary 1 {#ac-vii-s1-thm-3-cor-1 .statement}

In a Krull domain every non-zero prime ideal m contains a prime ideal of height 1. If m is not of height 1, then div m = 0 and A : m = A.

The first assertion has already been seen in the course of the proof of Theorem 3. If m is not of height 1 and p is a prime ideal of height 1 contained in m, then p ⊂ m̃ and p ≠ m̃; as div p is extremal, necessarily div m = div m̃ = 0; hence div(A : m) = 0 and, as A : m is divisorial (no. 1, Proposition 1), A : m = A.

#### Corollary 2 {#ac-vii-s1-thm-3-cor-2 .statement}

Let A be a Krull domain, K its field of fractions, v a valuation on K which is positive on A and p the set of x ∈ A such that v(x) > 0. If the prime ideal p is of height 1, v is equivalent to an essential valuation of A.

Let B be the ring of v and m its ideal. Then m ∩ A = p and hence A, ⊂ B. Now A,, is a discrete valuation ring (Theorem 3 and Corollary 1 to Proposition 6). As p ≠ (0), B ≠ K and hence B = A, (Chapter VI, § 4, no. 5, Proposition 6).

#### Theorem 4 {#ac-vii-s1-thm-4 .statement}

Let A be an integral domain and M the set of its prime ideals of height 1. For A to be a Krull domain, it is necessary and sufficient that the following Properties are satisfied:
(i) For all p ∈ M, A, is a discrete valuation ring.
(ii) A is the intersection of the A_p for p ∈ M.
(iii) For all x ≠ 0 in A, there exists only a finite number of ideals p ∈ M such that x ∈ p.
Moreover, the valuations corresponding to the A_p for p ∈ M are the essential valuations of A.

The conditions are trivially sufficient. Their necessity follows immediately from Theorem 3 of no. 4, Corollary I to Proposition 6 and the fact that the essential valuations of A satisfy the conditions of Definition 3 of no. 3.

#### Proposition 10 {#ac-vii-s1-prop-10 .statement}

Let A be an integrallyclosed Noetherian domain and a an integral ideal of A. The following conditions are equivalent:
(a) a is divisorial;
(b) the prime ideals associated with A/a are of height 1.

Recall that, if a = $\bigcap^n q_i$ is a reduced primary decomposition of a and p_i denotes the prime ideal corresponding to q_i, the prime ideals associated with A/a are just the p_i (Chapter IV, § 2, no. 3, Proposition 4). The fact that (a) implies (b) then follows from Proposition 8 of no. 4. Conversely, if, in the above notation, the p_i are of height 1, A_{p_i} is a discrete valuation ring (Theorem 4); now, q_i = q_i A_{p_i} ∩ A (Chapter IV, § 2, no. 1, Proposition 3); denoting by v_i the essential valuation corresponding to p_i, there therefore exists an integer n_i such that q_i is the set of x ∈ A such that v_i(x) ≥ n_i; this shows that the q_i are divisorial (no. 4, Proposition 5), hence also is a.

### 7. APPLICATION: NEW CHARACTERIZATIONS OF DISCRETE VALUATION RINGS

#### Proposition 11 {#ac-vii-s1-prop-11 .statement}

Let $\mathbf{A}$ be a local Krull domain (in particular an integrally closed local Noetherian domain) and $m$ its maximal ideal. The following conditions are equivalent:
(a) $\mathbf{A}$ is discrete valuation ring;
(b) $m$ is invertible;
(c) $\mathbf{A}:m \neq \mathbf{A}$;
(d) $m$ is divisorial;
(e) $m$ is the only non-zero prime ideal of $\mathbf{A}$.

As every non-zero ideal of a discrete valuation ring is principal (Chapter VI, § 3, no. 6, Proposition 9), it is invertible and hence (a) implies (b). If $m$ is invertible, its inverse is $\mathbf{A}:m$ (Chapter II, § 5, no. 6, Proposition 10) and hence $\mathbf{A}:m \neq \mathbf{A}$; hence (b) implies (c). If $\mathbf{A}:m \neq \mathbf{A}$, then $\mathbf{A}:(\mathbf{A}:m) \neq \mathbf{A}$; now $m \subset \mathbf{A}:(\mathbf{A}:m)$; hence $m = \mathbf{A}:(\mathbf{A}:m)$ since $m$ is maximal, so that $m$ is divisorial (no. 1, Proposition 1 (c)); thus (c) implies (d). The fact that (d) implies (e) follows from Theorem 3 of no. 6, Finally, if $m$ is the only non-zero prime ideal of $\mathbf{A}$, it is of height 1 and hence $\mathbf{A}_m$ is a discrete valuation ring (no. 6, Theorem 4); as $\mathbf{A}$ is local, $\mathbf{A}_m = \mathbf{A}$, which shows that (e) implies (a).

### 8. THE INTEGRAL CLOSURE OF A KRULL DOMAIN IN A FINITE EXTENSION OF ITS FIELD OF FRACTIONS

#### Proposition 12 {#ac-vii-s1-prop-12 .statement}

Let $\mathbf{A}$ be a Krull domain, $K$ its field of fractions, $K'$ a finite extension of $K$ and $\mathbf{A}'$ the integral closure of $\mathbf{A}$ in $K'$. Then $\mathbf{A}'$ is a Krull domain. The essential valuations of $\mathbf{A}'$ are the normed discrete valuations on $K'$ which are equivalent to the extensions of the essential valuations of $\mathbf{A}$.

Let $(v_i)_{i \in I}$ be the family of extensions to $K'$ of the essential valuations of $\mathbf{A}$. Since the degree $n = [K':K]$ is finite, the $v_i$ are discrete valuations on $K'$ (Chapter VI, § 8, no. 1, Corollary 3 to Proposition 1). Let $B_i$ be the ring of $v_i$; then $\mathbf{A}' \subset \bigcap_{L \in I} B_i$ (Chapter VI, § 1, no. 3, Theorem 3). Conversely, every element $x$ of $\bigcap_{i \in I} B_i$ is integral over each of the essential valuation rings of $\mathbf{A}$ (Chapter VI, § 1, no. 3, Corollary 3 to Theorem 3); hence the coefficients of the minimal polynomial of $x$ over $K$ belong to $\mathbf{A}$ (Chapter V, § 1, no. 3, Corollary to Proposition 11), so that $x \in \mathbf{A}'$; thus $\mathbf{A}' = \bigcap_{i \in I} B_i$. Now let $x$ be a non-zero element of $\mathbf{A}'$; it satisfies an equation of the form $x^s + a_{s-1}x^{s-1} + \ldots + a_0 = 0$

where $a_i \in \mathbf{A}$ and $a_s \neq 0$; if $v_i(x) > 0$, then $v_i(a_0) > 0$; now the essential valuations $v$ of $\mathbf{A}$ such that $v(a_0) > 0$ are finite in number and the valuations on $K'$ extending a given valuation on $K$ are also finite in number (Chapter VI, § 8, no. 3, Theorem 1); hence $v_i(x) = 0$ except for a finite number of indices $i \in I$. Thus it has been proved that $\mathbf{A}'$ is a Krull domain (no. 3, Definition 3).

It remains to show that the $v_i$ are equivalent to essential valuations of $A'$ (no. 4, Corollary 2 to Proposition 6), that is (no. 6, Corollary 2 to Theorem 3) that the prime ideal $p_i$, consisting of the $x \in A'$ such that $v_i(x) > 0$, is of height 1. If this were not so, there would exist a prime ideal $q$ of $A'$ such that $(0) \subset q \subset p_i$ distinct from $(0)$ and $p_i$; then $(0) \subset q \cap A \subset p_i \cap A$ and $q \cap A$ would be distinct from $(0)$ and $p_i \cap A$ (Chapter V, §2, no. 1, Corollary 1 to Proposition 1); the prime ideal $p_i \cap A$ would therefore not be of height 1, which contradicts the fact that it corresponds to an essential valuation of $A$.

#### Corollary {#ac-vii-s1-n8-cor-1 .statement}

*Let $p$ (resp. $p'$) be a prime ideal of $A$ (resp. $A'$) of height 1 and $v$ (resp. $u'$) the essential valuation of $A$ (resp. $A'$) corresponding to it. For $p'$ to lie above $p$, it is necessary and sufficient that the restriction of $v'$ to $K$ be equivalent to $v$.*

The valuation $v'$ is equivalent to the extension of an essential valuation $w$ of $A$ (Proposition 12). Let $q = p' \cap A$, which is a prime ideal of $A$ of height 1. For the restriction of $v'$ to $K$ to be equivalent to $v$, it is necessary and sufficient that $w = v$ and hence that $q = p$.

### 9. POLYNOMIAL RINGS OVER A KRULL DOMAIN

#### Proposition 13 {#ac-vii-s1-prop-13 .statement}

*Let $A$ be a Krull domain and $X_1, X_n, \ldots, X_n$ indeterminates. The ring $A[X_1, \ldots, X_n]$ is a Krull domain.*

Arguing by induction on $n$, it is sufficient to show that, if $X$ is an indeterminate, $A[X]$ is a Krull domain. Let $K$ be the field of fractions of $A$. The field of fractions of $A[X]$ is $K(X)$. Let $I$ be the set of monic polynomials in $K[X]$ which are irreducible over $K$; for all $f \in I$, let $v_f$ be the valuation on $K(X)$ defined by $f$ (Chapter VI, §3, no. 3, Example 4). On the other hand, for every essential valuation $w$ of $A$, let $w$ be the extension of $w$ to $K(X)$ defined by

$$
\bar{w}\left( \sum_j a_j X^j \right) = \inf_j (w(a_j))
$$

for $\sum_j a_j X^j \in K[X]$ (Chapter VI, §10, no. 1, Lemma 1). Clearly the $u$, and the $\bar{w}$ are discrete and normed and, for all $u \in K[X]$, $v_f(u) = 0$ (resp. $\bar{w}(u) = 0$) except for a finite number of valuations $v_f$ (resp. $\bar{w}$).

To show the proposition, it therefore suffices to show that $A[X]$ is the intersection of the rings of the valuations $v_f$ and $\bar{w}$. Now the intersection of the rings of the valuations $v_f$ is $K[X]$. On the other hand, for $\sum_j a_j X^j \in K[X]$, the relation $\bar{w}\left( \sum_j a_j X^j \right) \geq 0$ is equivalent to " $w(a_j) \geq 0$ for all $j$"; hence the relation " $\bar{w}\left( \sum_j a_j X^j \right) \geq 0$ for every valuation $\bar{w}'$" is equivalent to " $w(a_j) \geq 0$ for all $j$ and every essential valuation $w$ of $A$." This proves our assertion.

#### Remark {#ac-vii-s1-n9-rem-1 .statement}

The valuations $v_f$ and $\bar{w}$ introduced in the proof of Proposition 13 are the essential valuations of $A[X]$. It will be sufficient for us to show that, if $V$ is the set of valuations $v_f$ ($f$ irreducible) and $\bar{w}$ (w essential), then, for all $v' \in V$, there exists an element $g \in K(X)$ which is not in $A[X]$ and such that $v''(g) \geq 0$ for all the valuations $v'' \in V$ distinct from $v'$; this will prove that $V - \{v'\}$ does not satisfy (AK$_{II}$) and the conclusion will follow therefore from no. 4, Corollary 2 to Proposition 6. Suppose first that $v'$ is of the form $\bar{w}$: then we may take $g$ to be an element $b \in K$ such that $w(b) < 0, w'(b) \geq 0$ for the essential valuations $w'$ of $A$ distinct from $w$, for then $v_f(b) = 0$ for every irreducible monic polynomial $f$ in $K[X]$; the existence of an element $b$ satisfying the above conditions follows from no. 5, Proposition 9. Suppose secondly that $v'$ is of the form $v_f$ for an irreducible monic polynomial $f \in K[X]$ of degree $m$; then we may take $g = a/f$ where $a \in A$. For $v_h(g) \geq 0$ for every irreducible monic polynomial $h \neq f$ in $K[X]$; it remains to choose $a \in A$ such that, for every essential valuation $w$ of $A$, $w(a)$ is at least equal to the greatest lower bound of the elements $w(c_i)$, where the $c_i$ are the coefficients of $f$ ($1 \leq i \leq m$); now the existence of such an $a \in A$ follows from (AK$_{III}$) and no. 5, Proposition 9.

We may also say (no. 6, Theorem 4) that the prime ideals of $A[X]$ of height 1 are:
(1) the prime ideals of the form $pA[X]$, where $p$ is a prime ideal of $A$ of height 1;
(2) the prime ideals of the form $m \cap A[X]$, where $m$ is a (necessarily principal) prime ideal of $K[X]$.

The latter are characterized by the fact that their intersection with $A$ is reduced to 0.

### 10. DIVISOR CLASSES IN KRULL DOMAINS

Let $A$ be a Krull domain. Recall that the group $D(A)$ of divisors of $A$ is the free commutative group generated by the set $P(A)$ of its extremal elements (no. 3, Theorem 2) and that $P(A)$ is identified with the set of prime ideals of $A$ of height 1 (no. 6); for $p \in P(A)$ we shall denote by $v_p$ the normed essential valuation corresponding to $p$ (no. 4); recall that the ring of $v_p$ is $A_p$ (no. 4, Corollary 1 to Proposition 6). We shall denote by $F(A)$ the subgroup of $D(A)$ consisting of the principal divisors and by $C(A) = D(A)/F(A)$ the divisor class group of $A$ (no. 2).

#### Proposition 14 {#ac-vii-s1-prop-14 .statement}

Let $A$ be a Krull domain and $B$ a Krull domain containing $A$. Suppose that the following condition holds:

(PDE) For every prime ideal $\mathfrak{P}$ of $B$ of height 1, the prime ideal $\mathfrak{P} \cap A$ is zero or of height 1.

For $p \in P(A)$ the $\mathfrak{P} \in P(B)$ such that $\mathfrak{P} \cap A = p$ are finite in number; we write

$$
i(p) = \sum_{\mathfrak{P} \in P(B), \mathfrak{P} \cap A = p} e(\mathfrak{P}/p)\mathfrak{P},
$$

where $e(\mathfrak{P}/\mathfrak{p})$ denotes the *ramification* index of $v_{\mathfrak{p}}$ over $v_{\mathfrak{p}}$ (Chapter VI, § 8, no. 1). *Then i defines, by* linearity, an increasing *homomorphism* $i$ of $D(A)$ to $D(B)$, which enjoys the following properties:

(a) *for every non-zero element x of the field of fractions of A*,

$$
i(\operatorname{div}_A(x)) = \operatorname{div}_B(x);
$$

(b) *for all D, D' in D(A)*,

$$
i(\sup(D, D')) = \sup(i(D), i(D'));
$$

Let $\mathfrak{p} \in P(A)$; consider a non-zero element $a$ of $\mathfrak{p}$; the $\mathfrak{P} \in P(B)$ which contain $a$ are finite in number (no. 6, Theorem 4); *a fortiori* the $\mathfrak{P} \in P(B)$ such that $\mathfrak{P} \cap A = \mathfrak{p}$ are finite in number.

We now show (a). By additivity, it may be assumed that $x \in A^* = A - \{0\}$.

By definition, $\operatorname{div}_B(x) = \sum_{\mathfrak{P} \in P(B)} v_{\mathfrak{p}}(x) \cdot \mathfrak{P}$. For all $\mathfrak{P} \in P(B)$ such that $v_{\mathfrak{p}}(x) > 0$, $\mathfrak{P} \cap A$ is non-zero (for $x \in \mathfrak{P}$) and is therefore of height 1 by (PDE); setting $\mathfrak{p} = \mathfrak{P} \cap A$, by definition of the ramification index, $v_{\mathfrak{p}}(x) = e(\mathfrak{P}/\mathfrak{p}) v_{\mathfrak{p}}(x)$ (since $v_{\mathfrak{p}}$ and $v_{\mathfrak{P}}$ are normed). As $\operatorname{div}_A(x) = \sum_{\mathfrak{p} \in P(A)} v_{\mathfrak{p}}(x) \cdot \mathfrak{p}$, and $i(q) = 0$ for all $q \in P(A)$ which is not of the form $\mathfrak{Q} \cap A$ where $\mathfrak{Q} \in P(B)$, we deduce (a).

To prove (b) we write

$$
D = \sum_{\mathfrak{p} \in P(A)} n(\mathfrak{p}) \cdot \mathfrak{p} \quad \text{and} \quad D' = \sum_{\mathfrak{p} \in P(A)} n'(\mathfrak{p}) \cdot \mathfrak{p};
$$

the coefficient of $\mathfrak{p}$ in $\sup(D, D')$ is $\sup(n(\mathfrak{p}), n'(\mathfrak{p}))$. Let $\mathfrak{P}$ be an element of $P(B)$. If $\mathfrak{P} \cap A = (0)$, the coefficients of $\mathfrak{P}$ in $i(D)$ and $i(D')$ and hence also in $\sup(i(D), i(D'))$ are zero; therefore the coefficient of $\mathfrak{P}$ in $i(\sup(D, D'))$ is zero. If $\mathfrak{P} \cap A \neq (0)$, it is a prime ideal $\mathfrak{p}$ of height 1 (by (PDE)); writing $e = e(\mathfrak{P}/\mathfrak{p})$, the coefficients of $\mathfrak{P}$ in $i(D)$, $i(D')$ and $i(\sup(D, D'))$ are respectively $en(\mathfrak{p}), en'(\mathfrak{p})$ and $e \cdot \sup(n(\mathfrak{p}), n'(\mathfrak{p}))$; that of $\sup(i(D), i(D'))$ is

$$
\sup(e \cdot n(\mathfrak{p}), e \cdot n'(\mathfrak{p})) = e \cdot \sup(n(\mathfrak{p}), n'(\mathfrak{p})).
$$

This proves (b).

Under the hypotheses of Proposition 14, it follows from (a) that i defines, by taking quotients, a homomorphism $\bar{i}$, called canonical, of $C(A)$ to $C(B)$, which we shall also sometimes write as $i$, by an abuse of notation.

The condition (PDE) is fulfilled in the two following cases:

(1) B is integral over A; in this case, *for the prime* ideal $\mathfrak{P}$ of B to be *of height* 1, *it is necessary and sufficient that* $\mathfrak{p} = \mathfrak{P} \cap A$ be of height 1. For (0) is the only prime ideal of B lying above the ideal (0) of A (Chapter V, § 2, no. 1, Corollary I to Proposition 1); if $\mathfrak{P}$ is of height 1, then $\mathfrak{p} \neq 0$; if $\mathfrak{p}$ were not of height 1, there would exist a prime ideal $\mathfrak{p}'$ of A distinct from (0) and $\mathfrak{p}$ and such that 0 ⊂ p' ⊂ p; but then, as B is an integral domain and A is an integrally closed domain, there would be a prime ideal $\mathfrak{p}'$ of B such that $\mathfrak{p}' \cap A = p'$ and $\mathfrak{p}' \subset \mathfrak{p}$ (Chapter V, § 2, no. 4, Theorem 3), contrary to the hypothesis. Conversely, if p is of height 1, there can exist no prime ideal $\mathfrak{p}'$ of B distinct from 0 and $\mathfrak{p}$ and such that $0 \subset \mathfrak{p}' \subset \mathfrak{p}$, otherwise $0 \subset \mathfrak{p}' \cap A \subset p$ and $\mathfrak{p}' \cap A$ would be distinct from 0 and p by virtue of Chapter V, § 2, no. 1, Corollary 1 to Proposition 1.

(2) B is aflat A-module. More precisely:

#### Proposition 15 {#ac-vii-s1-prop-15 .statement}

Let A and B be Krull domains such that B contains A and is aflat A-module. Then:
(a) condition (PDE) of Proposition 14 is fulfilled;
(b) for every divisorial ideal $a \in A$, Ba is the divisorial ideal of B which corresponds to the divisor $i(\operatorname{div}_A(a))$.

To show (a), suppose that there exists a prime ideal $\mathfrak{p}$ of B of height 1 such that $\mathfrak{p} \cap A$ is neither 0 nor of height 1. Take an element $x \neq 0$ in $\mathfrak{p} \cap A$. The ideals $p_i$ of A of height 1 which contain x are finite in number and none contains $\mathfrak{p} \cap A$; there therefore exists an element y of $\mathfrak{p} \cap A$ such that $y \notin p_i$ for all $i$ (Chapter II, § 2, no. 1, Proposition 2). Thus $\operatorname{div}_A(x)$ and $\operatorname{div}_A(y)$ are relatively prime elements of the ordered group P(A), so that $\sup(\operatorname{div}_A(x), \operatorname{div}_A(y)) = \operatorname{div}_A(x) + \operatorname{div}_A(y) = \operatorname{div}_A(xy)$; as the ideals $Ax \cap Ay$ and $Axy$ are divisorial, we deduce that $Ax \cap Ay = Axy$. Since B is a flat A-module, $Bx \cap By = Bxy$ (Chapter I, § 2, no. 6, Proposition 6). This implies that $\sup(v_{\mathfrak{p}}(x), v_{\mathfrak{p}}(y)) = v_{\mathfrak{p}}(xy) = v_{\mathfrak{p}}(x) + v_{\mathfrak{p}}(y)$, which contradicts the inequalities $v_{\mathfrak{p}}(x) > 0, v_{\mathfrak{p}}(y) > 0$ (which hold since x and y are in $\mathfrak{p}$). Thus (a) has been proved by reductio ad absurdum.

We now show (b). If $a$ is a divisorial ideal of A, it is the intersection of two fractional principal ideals (no. 5, Corollary 2 to Proposition 9), say

$$
a = d^{-1}(Aa \cap Ab)
$$

where $a, b,$ dare in $A^*$; as B is flat over A, $Ba = d^{-1}(Ba \cap Bb)$ (Chapter I, § 2, no. 6, Proposition 6), which shows that Ba is divisorial. This shows also that $\operatorname{div}_B(Ba) = \sup(\operatorname{div}_B(a), \operatorname{div}_B(b)) - \operatorname{div}_B(d)$; using Proposition 14 (a) and (b), it is seen that

$$
\begin{align*}
\operatorname{div}_B(Ba) &= \sup(i(\operatorname{div}_A(a)), i(\operatorname{div}_A(b))) - i(\operatorname{div}_A(d)) \\
&= i(\sup(\operatorname{div}_A(a), \operatorname{div}_A(b))) - i(\operatorname{div}_A(d)) \\
&= i(\operatorname{div}_A(Aa \cap Ab)) - i(\operatorname{div}_A(d)) \\
&= i(\operatorname{div}_A(d^{-1}(Aa \cap Ab))) = i(\operatorname{div}_A(a)).
\end{align*}
$$

#### Corollary {#ac-vii-s1-n10-cor-1 .statement}

Let A be a local Krull domain and B a discrete valuation ring such that B dominates A and is aflat A-module. Then A is a field or a discrete valuation ring.

Let $\mathfrak{m}$ be the maximal ideal of B. By (PDE), $\mathfrak{m} \cap A$ is zero or of height 1. As it is, by hypothesis the maximal ideal of A, our assertion follows from Proposition 11 of no. 7.

#### Remark {#ac-vii-s1-n10-rem-1 .statement}

In the former of the two above cases, the mapping $i : D(A) \to D(B)$ is injective: as the elements of $P(B)$ form a basis of $D(B)$ and two distinct ideals of $P(A)$ cannot be the traces on A of the same ideal of $P(B)$, it amounts to verifying that $i(p) \neq 0$ for all $p \in P(A)$; now, this follows from Chapter V, § 2, no. 1, Theorem 1. It is similarly seen that, if B is a faithfully flat A-module, $i$ is injective (Chapter II, § 2, no. 5, Corollary 4 to Proposition 11).

In what follows, we propose to study the canonical homomorphism $\tilde{i}$ from $C(A)$ to $C(B)$ for certain ordered pairs of Krull domains A, B.

#### Proposition 16 {#ac-vii-s1-prop-16 .statement}

Let A be a Zariski ring such that its completion $\hat{A}$ is a Krull domain. Then A is a Krull domain and the canonical homomorphism $\tilde{i}$ from $C(A)$ to $C(\hat{A})$ (which is defined since A is a flat A-module; cf. Chapter III, § 3, no. 4, Theorem 3) is injective.

As A is an integral domain and $A \subset \hat{A}$, A is an integral domain. Let L be the field of fractions of $\hat{A}$ and K $\subset$ L that of A. As $A = \hat{A} \cap K$ (Chapter III, § 3, no. 5, Corollary 4 to Proposition 9), A is a Krull domain (no. 3, Example 4). The fact that $\tilde{i} : C(A) \to C(\hat{A})$ is injective follows from Proposition 15 (b) and the fact that, if $b \hat{A}$ is principal, b is principal (Chapter III, § 3, no. 5, Corollary 3 to Proposition 9).

Now let A be a Krull domain and S a multiplicative subset of A not containing 0. The group $D(A)$ (resp. $D(S^{-1}A)$) is the free commutative group with basis the set of $\operatorname{div}(p)$ (resp. $\operatorname{div}(S^{-1}p)$), where p runs through the set of prime ideals of A of height 1 (resp. the set of prime ideals of A of height 1 such that $p \cap S = \varnothing$) (no. 4, Proposition 6) and, if $p \cap S = \varnothing$, then $i(\operatorname{div}(p)) = \operatorname{div}(S^{-1}p)$. Thus $D(S^{-1}A)$ is identified with the directfactor of $D(A)$ generated by the elements $\operatorname{div}(p)$ such that $p \cap S = \varnothing$ and admits as complement the free commutative subgroup of $D(A)$ with basis the set of $\operatorname{div}(p)$ such that $p \cap S \neq \varnothing$; we shall denote this complement by G. As $i : D(A) \to D(S^{-1}A)$ is surjective, so is $i : C(A) \to C(S^{-1}A)$; and:

$$
G/(G \cap F(A)) = (G + F(A))/F(A) = \operatorname{Ker}(\tilde{i});
$$

for if an element of $D(S^{-1}A)$ is equal to $\operatorname{div}_{S^{-1}A}(x/s)$, where $x \in A$ and $s \in S$, it is the image under $i$ of the principal divisor $\operatorname{div}_A(x)$ (Proposition 14).

Suppose now that S is generated by a family of elements $(p_i)_{i \in I}$ of A such that the principal ideals $Ap_i$ are all prime. Then, if $p$ is a prime ideal of A of height 1 such that $p \cap S \neq \varnothing$, $p$ contains a product of powers of the $p_i$, and therefore one of the $p_i$, say $p_\alpha$; as $Ap_\alpha$ is non-zero and prime and $p$ is of height 1, it follows that $p = Ap_\alpha$. In the above notation, therefore $G \subset F(A)$ and (5) shows that the kernel of $\bar{i}$ is zero. We have therefore shown the following result:

#### Proposition 17 {#ac-vii-s1-prop-17 .statement}

*Let $A$ be a Krull domain and $S$ a multiplicative subset of $A$ not containing $0$. Then the canonical homomorphism $\bar{i}$ from $C(A)$ to $C(S^{-1}A)$ is surjective. If further $S$ is generated by a family of elements $p_i$ such that the principal ideals $Ap_i$ are all prime, then $\bar{i}$ is bijective.*

As a second application of formula (5), consider the following situation: let $R$ be a Krull domain; take $A$ to be the polynomial ring $A = R[X]$ (no. 9, Proposition 13) and $S$ to be the set $R - (0)$ of non-zero constant polynomials of $A$. The prime ideals $p$ of $A$ of height 1 such that $p \cap S \neq \varnothing$ are those of the form $p_0A$, where $p_0$ is a prime ideal of $R$ of height 1 (no. 9, *Remark*). Hence, in the notation introduced above, $G$ is identified with $D(R)$ by identifying $\mathrm{div}_A(p_0A)$ with $\mathrm{div}_R(p_0)$. On the other hand $G \cap F(A)$ is identified with $F(R)$: for if an ideal $a$, of $R$ generates a principal ideal $a_0A = f(X)A$ in $A = R[X]$, then $f(0) \in a_0A$ since $a_0A$ is a graded ideal of the ring $A$ (graded by the usual degree of polynomials) and hence $f(0) \in a$; further, for $a \in a_0A$, $a = f(X)g(X)$ where $g(X) \in R$, whence, comparing terms of degree 0, $a = f(0)g(0)$; it follows that $a$ is the principal ideal of $R$ generated by $f(0)$. Finally, denoting by $K$ the field of fractions of $R$, $S^{-1}A$ is identified with the polynomials ring $K[X]$, which is a principal ideal domain; hence $C(S^{-1}A) = (0)$. Thus, by (5), $C(A) = \mathrm{Ker}(\bar{i})$ is identified with $C(R)$ and we have proved the following result:

#### Proposition 18 {#ac-vii-s1-prop-18 .statement}

*Let $R$ be a Krull domain and $A$ the polynomial ring $R[X]$. The canonical homomorphism of $C(R)$ to $C(R[X])$ is bijective.*

### Exercises {#ac-vii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
