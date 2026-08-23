---
book: alg
book_title: Algebra
chapter: VI
chapter_title: ORDERED GROUPS AND FIELDS
section: 2
section_title: Ordered fields
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A VI.37-A VI.47
pdf_pages: 0330-0341, 0348-0358
extraction: ocr
subsections:
    - "no": 1
      title: Ordered rings
      page: 19
      pdf_page: 330
    - "no": 2
      title: Ordered fields
      page: 20
      pdf_page: 331
    - "no": 3
      title: Extensions of ordered fields
      page: 21
      pdf_page: 332
    - "no": 4
      title: Algebraic extensions of ordered fields
      page: 23
      pdf_page: 334
    - "no": 5
      title: Maximal ordered fields
      page: 25
      pdf_page: 336
    - "no": 6
      title: Characterisation of maximal ordered fields. Euler-Lagrange Theorem
      page: 26
      pdf_page: 337
    - "no": 7
      title: Vector spaces over an ordered field
      page: 28
      pdf_page: 339
statements: 31
exercises: 41
content_sha256: 35de4067e084a16e84edef67e2102758ffddde3b4289107c3615dde8486954b7
---

## § 2. ORDERED FIELDS

### 1. Ordered rings

#### Definition 1 {#alg-vi-s2-def-1 .statement}

— Given a commutative ring $ \mathbf{A} $, we say that an ordering on $ \mathbf{A} $ is compatible with the ring structure of $ \mathbf{A} $ if it is compatible with the additive group structure of $ \mathbf{A} $, and if it satisfies the following axiom :
(OR) The relations $ x \geqslant 0 $ and $ y \geqslant 0 $ imply $ xy \geqslant 0 $.
The ring $ \mathbf{A} $, together with such an ordering, is called an ordered ring.

#### Example {#alg-vi-s2-n1-exa-1 .statement}

— 1) The rings $ \mathbf{Q} $ and $ \mathbf{Z} $, with the usual orderings, are ordered rings.
2) A product of ordered rings, equipped with the product ordering, is an ordered ring. In particular the ring $ \mathbf{A}^E $ of mappings from a set $ E $ to an ordered ring $ \mathbf{A} $ is an ordered ring.
3) A subring of an ordered ring, with the induced ordering, is an ordered ring.

In an ordered ring, the relations $ x \geqslant y $ and $ z \geqslant 0 $ imply $ xz \geqslant yz $. Indeed these inequalities are equivalent to $ x - y \geqslant 0 $, $ z \geqslant 0 $ and $ (x - y)z \geqslant 0 $ respectively.
Analogously we can show that the relations $ x \leqslant 0 $ and $ y \geqslant 0 $ (resp. $ y \leqslant 0 $) imply $ xy \leqslant 0 $ (resp. $ xy \geqslant 0 $). These results are often invoked under the name of sign rules (two elements are said to have the same sign if they are both $ \geqslant 0 $ or both $ \leqslant 0 $). They imply that, if $ \mathbf{A} $ is a totally ordered ring, then every square is positive, and in particular that every idempotent (for example the unit element) is positive.

#### Example {#alg-vi-s2-n1-exa-2 .statement}

— There is only one totally ordered ring structure on $ \mathbf{Z} $: indeed $ 1 > 0 $, whence $ n > 0 $ for every natural number $ n \neq 0 $, by induction. In contrast there exist ordered ring structures on $ \mathbf{Z} $ which are not totally ordered (see below).

Let $ P $ be the set of positive elements of an ordered ring $ \mathbf{A} $. It is known (VI, p. 3, Prop. 3) that $ P $ determines the ordering on $ \mathbf{A} $. To say that $ \mathbf{A} $ is an ordered ring is equivalent to saying that $ P $ satisfies the following properties :

$$
\begin{align*}
(\mathrm{AP}_I) &\quad P + P \subset P \\
(\mathrm{AP}_{II}) &\quad PP \subset P \\
(\mathrm{AP}_{III}) &\quad P \cap (-P) = \{0\}
\end{align*}
$$

Indeed $ (\mathrm{AP}_I) $ and $ (\mathrm{AP}_{III}) $ state that the additive group of $ \mathbf{A} $ is an ordered group (VI, p. 3, Prop. 3), while $ (\mathrm{AP}_{,,}) $ is a translation of (OR).

Recall that the following condition is necessary and sufficient for the order relation on $ \mathbf{A} $ to be total :

$$
(\mathrm{AP}_{IV}) \quad P \cup (-P) = \mathbf{A}.
$$

#### Example {#alg-vi-s2-n1-exa-3 .statement}

— In $ \mathbf{Z} $, if we take $ P $ to be the set of positive (in the usual sense) even integers, we get a ring which is not totally ordered.

Recall also that, in a totally ordered abelian group, the relation $ n \cdot x = 0 $ (for a natural number $ n \neq 0 $) implies $ x = 0 $ (VI, p. 4); this gives us the following result.

#### Proposition 1 {#alg-vi-s2-prop-1 .statement}

— A *totally ordered ring is torsion free as a $ \mathbf{Z} $-module* (II, p. 313).

### 2. Ordered fields

#### Definition 2 {#alg-vi-s2-def-2 .statement}

— A commutative *field, equipped with a total ordering, is called an ordered field* if *its ordering and its ring structure are compatible*.

We restrict ourselves to *total* order relations on fields because the others are very « pathological » (VI, p. 38, Ex. 6).

*Examples. — 1) The field $ \mathbf{Q} $ of rational numbers is an ordered field.
2) A subfield of an ordered field, with the induced ordering, is an ordered field.
3) \* The field of real numbers is an ordered field. \*

Let $ K $ be an ordered field. For all $ x \in K $ we put

$$
\begin{align*}
\operatorname{sgn}(x) &= 1 & \text{if } x > 0, \\
\operatorname{sgn}(x) &= -1 & \text{if } x < 0, \\
\operatorname{sgn}(x) &= 0 & \text{if } x = 0.
\end{align*}
$$

Then we have $ \operatorname{sgn}(xy) = \operatorname{sgn}(x) \operatorname{sgn}(y) $; we call $ \operatorname{sgn}(x) $ the *sign* of $ x $. The map $ x \mapsto \operatorname{sgn}(x) $ from $ K^* $ to the multiplicative group $ \{-1, +1\} $ is a surjective homomorphism whose kernel, the set of strictly positive elements of $ K $, is a subgroup of $ K^* $ of index 2.

Conversely, if $ K $ is a commutative field and $ s : K^* \to \{-1, +1\} $ is a surjective homomorphism whose kernel is closed under addition, then $ s $ is the sign map for a unique ordered field structure, where the set of strictly positive elements is the kernel of $ s $.

For all $ x $ and $ y $ in $ K $ we have $ x = \operatorname{sgn}(x)|x| $ and $ |xy| = |x||y| $.

On the other hand every ordered field is of characteristic zero (Prop. 1).

#### Proposition 2 {#alg-vi-s2-prop-2 .statement}

— *Let $ A $ be a totally ordered integral domain, and let $ K $ be its field of fractions. Then there exists one and only one ordering on $ K $ which restricts to the given ordering on $ A $ and makes $ K $ an ordered field.*

Every $ x \in K $ can be expressed in the form $ x = ab^{-1} $, with $ a $ and $ b $ in $ A $ and $ b \neq 0 $. If $ x $ is positive, then $ a $ and $ b $ have the same sign, and conversely. Thus we see that, if there exists an ordering on $ K $ satisfying the prescribed conditions, then it is unique, and the set $ P $ of positive elements is identical to the set of $ ab^{-1} $, where $ a $ and $ b $ are elements of $ A $ of the same sign, and $ b \neq 0 $. It remains to show that $ P $ satisfies conditions (AP$_I$), (AP$_{II}$), (AP$_{III}$) and (AP$_{IV}$). This is obvious for (AP$_{II}$) and (AP$_{IV}$). For (AP$_I$), consider $ ab^{-1} + cd^{-1} $, where we may assume that $a$, $b$, $c$ and $d$ are positive; this sum is $(ad + bc)(bd)^{-1}$, and $ad + bc$ and $bd$ are positive.

To show $(\mathrm{AP}_{III})$, consider an identity of the form $ab^{-1} = -cd^{-1}$, so that $ad + bc = 0$. If we assume that $a$ and $b$ have the same sign and that $c$ and $d$ have the same sign, then the sign rules show that $ad$ and $bc$ have the same sign; whence $ad = bc = 0$, so $a = c = 0$; hence $P$ does indeed satisfy $(\mathrm{AP}_{III})$.

#### Example {#alg-vi-s2-n2-exa-1 .statement}

— Since $Z$ admits only one totally ordered ring structure (*VI*, p. 19, *example*), the field $\mathbf{Q}$ admits only one ordering which makes it an ordered field: this is the usual ordering.

### 3. Extensions of ordered fields

#### Definition 3 {#alg-vi-s2-def-3 .statement}

*Let $K$ be an ordered field. An ordered extension of $K$ is a pair $(E, u)$, where $E$ is an ordered field and $u$ is an increasing homomorphism from $K$ to $E$.*

Let $K$ be a field, let $E$ be an ordered field and let $u : K \to E$ be a homomorphism. The relation
$$
x \leq y \quad \text{if} \quad u(x) \leq u(y)
$$
is a total order relation on $K$ which gives it an ordered field structure, said to be *induced* by that of $E$. If $K$ and $E$ are ordered fields, then a homomorphism $u : K \to E$ is increasing if and only if the ordered field structure of $K$ is induced by that of $E$. We will usually identify $K$ with its image in $E$ under $u$.

#### Example {#alg-vi-s2-n3-exa-1 .statement}

— 1) Every ordered field $K$ is an ordered extension of $\mathbf{Q}$. Indeed $K$ is an extension of $\mathbf{Q}$, since it is of characteristic zero, and on the other hand $\mathbf{Q}$ can only be ordered in one way, as we have just seen.

2) Let $K$ be an ordered field, and let $K(X)$ be the field of rational functions in one indeterminate over $K$. Let us define an ordering on the polynomial ring $K[X]$ by taking the positive elements to be $0$ and those polynomials whose leading coefficient is positive. In this way we obtain a totally ordered ring whose ordering extends that of $K$. By applying Prop. 2 we give $K(X)$ the structure of an ordered extension of $K$. *For $K = \mathbf{R}$ it can be shown that the order relation defined on $K(X)$ in this way is that of growth near $+\infty$ (cf. *VI*, p. 24, Prop. 4).*

#### Theorem 1 {#alg-vi-s2-thm-1 .statement}

*For an extension $E$ of $K$ to admit the structure of an ordered extension of $K$, the following condition is necessary and sufficient:*
*(OE)* *The relation $p_1 x_1^2 + \ldots + p_n x_n^2 = 0$ implies*
$$
p_1 x_1 = \ldots = p_n x_n = 0
$$
*for any finite sequence $(x_i, p_i)$ of pairs of elements $x$, of $E$ and positive elements $p_i$ of $K$.*

Condition (OE) is clearly equivalent to:
(OE') *The element – 1 is not a sum of elements of the form* $ px^2 $ ($ x \in E, p \in K, p \geq 0 $).

Condition (OE) is necessary: if E is an ordered extension of K then the elements $ p_i x_i^2 $ are positive in E, so zero if their sum is zero. On the other hand $ p_i x_i^2 = 0 $ is equivalent to $ p_i x_i = 0 $.

Conversely, suppose condition (OE) is satisfied, then we will define an ordering on E by constructing a subset P of E which satisfies conditions (AP,,), (APII), (AP,,,) and (APIV), and which contains the set $ K_+ $ of positive elements of K. Such a subset P will certainly make E an ordered extension of K, for we will have $ K \cap P = K_+ $; indeed, if P were to contain an element $ -a < 0 $ of K, then a would belong to $ P \cap (-P) $, contradicting (APIII).

To define P, let us consider the set $ \mathcal{M} $ of subsets of E which satisfy (API), (AP,,) and (AP,,,), and which contain the union of $ K_+ $ and the set C of squares of elements of E. This set $ \mathcal{M} $ is nonempty, for it contains the set $ P_0 $ of elements of the form $ \sum p_i x_i^2 $ (that $ P_0 $ satisfies (AP,,,) follows immediately from (OE)).

Moreover $ \mathcal{M} $ is inductive (*Set Theory*, III, p. 154, Def. 3). Thus there exists, by Th. 2 of *Set Theory*, III, p. 154, a maximal element in $ \mathcal{M} $, which it remains for us to prove satisfies (APIV); now this follows from the following lemma:

#### Lemma {#alg-vi-s2-n3-lem-1 .statement}

— *Let* $ P \in \mathcal{M} $ *and* $ x \notin P $; *then there exists* $ P' \in \mathcal{M} $ *such that* $ P \subset P' $ *and* $ -x \in P' $.

Take $ P' = P - xP $, and check that $ P' $ has the required properties. Since $ 0 \in C \subset P $, we have $ P \subset P' $. Whence $ C \subset P' $ and $ K_+ \subset P' $. Since $ 1 \in C \subset P $ we have $ -x \in P' $. We have
$$
P' + P' = P - xP + P - xP = P + P - x(P + P) \subset P - xP = P',
$$
whence (API). We have
$$
P'P' = (P - xP)(P - xP) \subset \\
\quad \subset PP + x^2PP - x(PP + PP) \subset P + CP - xP \subset P - xP = P',
$$
whence (AP,,,) Finally, let us check (APIII): suppose given an identity of the form $ p - xq = -(r - xs) $ where $ p, q, r, s $ belong to P; we deduce from this the relation $ x(s + q) = p + r $; if $ s + q \neq 0 $ we have
$$
x = (s + q)^{-2}(s + q)(p + r) \in CPP \subset P,
$$
contrary to the hypothesis; hence $ s + q = 0 $, whence $ p + r = 0 $; since P satisfies (AP,,,) we deduce that $ s = q = r = p = 0 $, which completes the proof.

#### Corollary 1 (*« Artin-Schreier Theorem »*) {#alg-vi-s2-thm-1-cor-1 .statement}

— *A necessary and sufficient condition for there to exist an ordering on a commutative field* E *which makes it an ordered field, is that the relation* $ x_1^2 + \ldots + x_n^2 = 0 $ *imply* $ x_1 = \ldots = x_n = 0 $.

The necessity is obvious. Conversely, the stated condition implies that E is of characteristic zero, hence an extension of Q; then condition $(OE)$ is satisfied, and Th. 1 shows that there exists on E the structure of an ordered extension of Q, that is an ordered field structure.

There does *not* exist any ordered field structure on a field E in which $-1$ is a square, in particular on an algebraically closed field.

#### Corollary 2 {#alg-vi-s2-thm-1-cor-2 .statement}

*Let E be an extension of K admitting the structure of an ordered extension of K. For an element $x \in E$ to be positive under every such structure on E, it is necessary and sufficient that x be of the form $\sum_i p_i x_i^2$, where $x_i \in E$ and the $p_i$ are positive elements of K.*

The condition is obviously sufficient; it is also necessary, for (in the notation of the proof of Th. 1), if $x \notin P_0$ there exists a maximal element P of $\mathcal{M}$ such that $x \notin P$; then $-x \in P$ by the Lemma, and x is not positive under the ordering defined by P, since $x \neq 0$.

### 4. Algebraic extensions of ordered fields

Let K be an ordered field, and f a polynomial in K[X]. We will say that *f changes sign in K* if there exist two elements a and b in K such that $f(a) f(b) < 0$; then we say that *f changes sign between a and b*.

#### Proposition 3 {#alg-vi-s2-prop-3 .statement}

*Let K be an ordered field and f an irreducible polynomial over K which changes sign between a and b in K. Then the extension $E = K[X]/(f)$ of K admits the structure of an ordered extension.*

We will argue by induction on the degree n off. For $n = 1$ the proof is trivial. Suppose the result holds for degrees $\leq n - 1$, and let us prove it for degree n by contradiction; by Th. 1 we are thus assuming a relation of the form

$$
1 + \sum_i p_i f_i^2(X) \equiv 0 \pmod{f(X)}, \quad \text{where } f_i \in K[X], \quad p_i \in K \quad \text{and} \quad p_i \geq 0
$$

Without loss of generality we may suppose that the $f_i$ have degrees $\leq n - 1$ (*IV*, p. 11, Cor). Then

$$
1 + \sum_i p_i f_i^2(X) = h(X) f(X)
$$

where $h \neq 0$ has degree at most $n - 2$. Replacing X by a and b in the above inequality, we see that $h(a) f(a) > 0$ and $h(b) f(b) > 0$. Since f changes sign between a and b by hypothesis, we conclude that $h(a) h(b) < 0$. Then we have a similar inequality for one of the irreducible factors $ g(X) $ of $ h(X) $: that is $ g(a)\ g(b) < 0 $. But $ 1 + \sum_i P_i f_i^2(X) \equiv 0 \pmod{g(X)} $, which shows that the field $ K[X]/(g) $ cannot be an ordered extension of $ K $ (Th. 1), contrary to the induction hypothesis.

#### Remark {#alg-vi-s2-n4-rem-1 .statement}

— There exist irreducible polynomials $ f $ over an ordered field $ K $ which do not change sign in $ K $, but such that $ K[X]/(f) $ admits the structure of an ordered extension of $ K $ (cf. VI, p. 43, Ex. 26, c)).

In order to apply the previous proposition we will need the following result:

#### Proposition 4 {#alg-vi-s2-prop-4 .statement}

— *Let $ K $ be an ordered field and let $ f \in K[X] $. There exists an interval in $ K $, in the complement of which $ f $ takes the same sign as its highest degree term.*

We can immediately reduce ourselves to the case of a monic polynomial; then one can write $ f(x) = x^n(1 + a_1 x^{-1} + \ldots + a_n x^{-n}) $ for $ x \neq 0 $. Let

$$
M = \sup (1, |a_1| + \cdots + |a_n|).
$$

For $ |x| > M $ we have $ 1 + a_1 x^{-1} + \ldots + a_n x^{-n} > 0 $, which completes the proof of the proposition.

#### Corollary 1 {#alg-vi-s2-prop-4-cor-1 .statement}

— *Every extension of an ordered field of odd finite degree admits the structure of an ordered extension.*

Such an extension, being monogenous (V, p. 40, Th. 1), is isomorphic to $ K[X]/(f) $, where $ f $ is an irreducible polynomial of odd degree. Then it is enough to show that $ f $ changes sign in $ K $ (Prop. 3), which follows immediately from Prop. 4.

#### Corollary 2 {#alg-vi-s2-prop-4-cor-2 .statement}

— *If $ a $ is a positive element of an ordered field $ K $, then every splitting field $ E $ of the polynomial $ X^2 - a $ admits the structure of an ordered extension of $ K $.*

The result is trivial if $ a $ is a square in $ K $. Otherwise the polynomial $ f(X) = X^2 - a $ is irreducible and changes sign, since $ f(0) < 0 $ and $ f(x) $ has the same sign as $ x^2 $, so positive, for $ x $ in the complement of some interval of $ K $. We can now complete the proof by applying Prop. 3.

#### Remark {#alg-vi-s2-n4-rem-2 .statement}

— When the ordered field $ K $ contains the « square roots » of a positive element $ a $ of $ K $ (roots of the polynomial $ X^2 - a $) then the notation $ \sqrt{a} $ is generally reserved for the *positive* square root. If $ K $ does *not* contain the square roots $ b $ and $ -b $ of $ a $ in the field $ E $, then the latter can be made an ordered extension of $ K $ in *two* ways, each induced from the other *via* the $ K $-automorphism which sends $ b $ to $ -b $; the choice of one of these orderings determines $ \sqrt{a} $: it is whichever of the elements $ b $ and $ -b $ is positive.

If $ a $ and $ a' $ are two positive elements of $ K $, whose square roots are in $ K $, then $ \sqrt{aa'} = \sqrt{a} \sqrt{a'} $, which follows from the definition of $ \sqrt{a} $ and the sign rule.

### 5. Maximal ordered fields

#### Definition 4 {#alg-vi-s2-def-4 .statement}

— *An ordered field K is maximal if every ordered algebraic extension of K is trivial.*

#### Example {#alg-vi-s2-n5-exa-1 .statement}

— *We will see later (Gen. Top., VIII, p. 1) that the field R of real numbers is a maximal ordered field.*

The existence of maximal ordered fields is a consequence of the following theorem:

#### Theorem 2 {#alg-vi-s2-thm-2 .statement}

— *Every ordered field K admits an ordered algebraic extension which is a maximal ordered field.*

One can show that this ordered extension is unique up to K-isomorphism (VI, p. 40, Ex. 15).

Let $ \Omega $ be an algebraic closure of K, and let $ \mathfrak{N} $ be the set of pairs $(A, w)$, where $A$ is a sub-K-extension of $ \Omega $, and $w$ is an ordering on $A$ making $A$ an ordered extension of $K$. Order $ \mathfrak{N} $ by the relation « L is an ordered extension of M » between M and $L$. Equipped with this ordering, $ \mathfrak{N} $ is an *inductive* ordered set: indeed if $(L_i)$ is a totally ordered family of elements of $ \mathfrak{N} $, then the field $L = \bigcup L_i$, ordered by taking $L_1 = \bigcup (L_i)_1$, is an upper bound for the $L_i$. Then $ \mathfrak{N} $ has a maximal element, by *Set Theory*, III, p. 154, Th. 2, which completes the proof.

#### Proposition 5 {#alg-vi-s2-prop-5 .statement}

— *Let K be a maximal ordered field, and let f be a polynomial in K[X] which changes sign between two elements a and b of K (with $a < b$). Then f has a root x in K such that $a < x < b$.*

At least one of the irreducible factors off, say $h$, changes sign between $a$ and $b$. Then the field $K[X]/(h)$ admits the structure of an ordered extension of $K$ (VI, p. 23, Prop. 3), and $h$ has degree 1 (Def. 4). Since $h(a) h(b) < 0$, the unique root $x$ of $h$ is such that $a < x < b$, since a polynomial function of degree 1 is monotonic.

#### Proposition 6 {#alg-vi-s2-prop-6 .statement}

— *Every positive element of a maximal ordered field K has a square root in K. Every polynomial of odd degree in K[X] has at least one root in K.*

This follows immediately from Cor. 2 and 1 to Prop. 4 of VI, p. 24.

#### Corollary {#alg-vi-s2-n5-cor-1 .statement}

— *On a maximal ordered field K there exists only one ordering compatible with the field structure.*

Indeed the positive elements of K are determined by its algebraic structure: they are the squares.

### 6. Characterisation of maximal ordered fields. Euler-Lagrange Theorem

The property expressed by Prop. 6 of VI, p. 25 characterises maximal ordered fields. More precisely:

#### Theorem 3 (Euler-Lagrange) {#alg-vi-s2-thm-3 .statement}

— Let K be an ordered field. Then the following three properties are equivalent:
a) The field $ K(i) $ is algebraically closed (where i denotes a square root of -1).
b) The ordered field K is maximal.
c) Every positive element of K is a square, and every polynomial of odd degree in $ K[X] $ has a root in K.

It is clear that a) implies b): indeed K has only two algebraic extensions up to isomorphism, the field K itself and $ K(i) $, which cannot be ordered since -1 is a square.

The fact that b) implies c) is nothing other than Prop. 6 of VI, p. 25.

It remains for us to prove that c) implies a). That will follow from the next two propositions.

#### Proposition 7 {#alg-vi-s2-prop-7 .statement}

— Let K be an ordered field in which every positive element is a square. Then every element of $ K(i) $ is a square, and every polynomial of degree 2 over $ K(i) $ has a root in $ K(i) $.

Let us show first that the second assertion reduces to the first. One can put the second degree polynomial $ aX^2 + bX + c $ ($ a \neq 0 $) in the following form, often called the canonical trinomial form:

$$
a((X + (b/2a))^2 - (b^2 - 4ac)/4a^2)
$$

If d is a square root of $ (b^2 - 4ac)/4a^2 $, then $ d - (b/2a) $ is a root of the quadratic polynomial under consideration.

Now we show that every element $ a + bi $ ($ a \in K, b \in K $) is a square; we are looking for an element $ x + yi $ such that

$$
(x + yi)^2 = a + bi;
$$

this translates into $ x^2 - y^2 = a $ and $ 2xy = b $. From this we deduce that

$$
(x^2 + y^2)^2 = a^2 + b^2
$$

Let c denote the positive square root of $ a^2 + b^2 $; then $ c \geq |a|, c \geq |b| $ and $ x^2 + y^2 = c $. Whence $ x^2 = (c + a)/2 $ and $ y^2 = (c - a)/2 $. Since $ c \geq |a| $ these equations are soluble in K, and if $ x_0 $ and $ y_0 $ are two solutions then $ x_0^2 - y_0^2 = a $ and $ 2x_0y_0 = \pm b $. We obtain the desired square root by taking $ x = x_0 $ and $ y = b/2x_0 $.

#### Proposition 8 {#alg-vi-s2-prop-8 .statement}

— Let K be a commutative field (of arbitrary characteristic) and let $ K' $ be a splitting field for the polynomial $ X^2 + 1 \in K[X] $ (V, p. 21). Suppose:
a) every polynomial in $ K[X] $ of odd degree has a root in $ K' $;

b) every polynomial in $ K'[X] $ of degree 2 has a root in $ K' $.
Then $ K' $ is algebraically closed.

Note first that it is enough to prove that every non-constant polynomial in $ K[X] $ has a root in $ K' $: this is indeed clear if $ K' = K $; if $ K' \neq K $ then $[K':K] = 2$; let $ a \mapsto a $ denote the unique $ K $-automorphism of $ K' $ distinct from the identity map; if $ f \in K'[X] $ and if $ \bar{f} $ denotes the polynomial obtained by applying $ a \mapsto \bar{a} $ to the coefficients of $ f $, then $ f \bar{f} \in K[X] $; if $ a \in K' $ is a root of $ f \bar{f} $ then $ a $ is either a root of $ f $ or of $ \bar{f} $; thus either $ a $ or $ a $ is a root of $ f $.

Thus let $ f $ be a polynomial over $ K $ of degree $ 2^n p $, $ p $ odd. *We* will proceed by induction on $ n $, the property being true for $ n = 0 $ by hypothesis *a)*. Let E be an extension of $ K $ in which $ f $ splits into linear factors:

$$
f(X) = \prod_i (X - a_i)
$$

Let $ b \in K $; put $ y_{ij} = a_i + a_j + ba_i a_j \in E $ and

$$
h(X) = \prod_{i < j} (X - y_{ij}) \in E[X].
$$

The coefficients of this polynomial are symmetric functions in the $ a_i $, with coefficients in $ K $; it therefore belongs to $ K[X] $ (IV, p. 62, Th. 1); since it has degree $ 2^n p (2^n p - 1)/2 = 2^{n-1} p' $ ($ p' $ odd), it has a root $ y_{} $, in $ K' $ by inductive hypothesis. If we note that this holds for all $ b \in K $, and that $ K $ is an infinite field (indeed a finite field, which has monogenous extensions of arbitrarily large odd degree (V, p. 94, Prop. 3), cannot satisfy *a)*), then we can deduce the existence of at least one pair $(i, j)$ such that

$$
a_i + a_j + ba_i a_j \in K' \quad \text{and} \quad a_i + a_j + b'a_i a_j \in K',
$$

with $ b \neq b' $. Then $ a_i + a_j $ and $ a_i a_j $ are elements of $ K' $, hence so are $ a_i $ and $ a_j $, since they are the roots of the quadratic equation

$$
x^2 - (a_i + a_j)x + a_i a_j = 0.
$$

Q.E.D.

For a generalisation and an alternative proof of Prop. 8, based on Galois theory, see VI, p. 46, Ex. 33.

Let $ K $ be an ordered field and let $ K' = K(i) $; for every element $ z = a + bi $ of $ K' $, the norm $ z \overline{z} = a^2 + b' $ of $ z $ relative to $ K $ (III, p. 544, example 1) is a positive element of $ K $, which vanishes only for $ z = 0 $. If every positive element in $ K $ is a square (in particular if $ K $ is a maximal ordered field), then the positive square root of the norm $ z \overline{z} $ is called the absolute value of $ z $, and is written $ |z| $. Since $ |zz'|^2 = |z|^2 |z'|^2 $ we have $ |zz'| = |z| \cdot |z'| $.

Moreover, the triangle inequality

$$
|z + z'| \leq |z| + |z'|
$$

holds for every pair of elements $ z, z' $ of $ K' $. Indeed, if $ z = a + bi $ and $ z' = a' + b'i $, then this inequality is equivalent to

$$
(a + a')^2 + (b + b')^2 \leq a^2 + b^2 + a'^2 + b'^2 + 2 \sqrt{(a^2 + b^2)(a'^2 + b'^2)}
$$

and hence also to

$$
(aa' + bb')^2 \leq (a^2 + b^2)(a'^2 + b'^2)
$$

which can be written $ (ab' - ba')^2 \geq 0 $.

Th. 3 enables us to determine all the irreducible polynomials over a maximal ordered field:

#### Proposition 9 {#alg-vi-s2-prop-9 .statement}

— *If K is a maximal ordered field, then the only irreducible polynomials in K[X] are the first degree polynomials, and the second degree polynomials $ aX^2 + bX + c $ such that $ b^2 - 4ac < 0 $.*

Since $ K(i) $ is algebraically closed, every algebraic extension of K, and hence also every irreducible polynomial over K, has degree 1 or 2. To see which second degree polynomials are irreducible, it is enough to consider the canonical form $ a((X + (b/2a))^2 - (b^2 - 4ac)/4a^2) $ (cf. *VI*, p. 26, Prop. 7).

#### Remark {#alg-vi-s2-n6-rem-1 .statement}

— Translating into the canonical trinomial form yields this stronger result: a necessary and sufficient condition for the polynomial $ aX^2 + bX + c $ over a given ordered field K to have constant sign in K is that $ b^2 - 4ac < 0 $, and then the sign of the polynomial is that of $ a $.

### 7. Vector spaces over an ordered field

Let K be an ordered field, and let E be a vector space over $ K $. The relation « there exists $ \lambda > 0 $ in $ K $ such that $ y = \lambda x $ » between two elements $ x $ and $ y $ in the set $ E - \{0\} $ is an *equivalence relation*. The equivalence classes under this relation are called *open halflines with origin 0*; the union of an open half-line and $ \{0\} $ is called a *closed half-line* (or sometimes simply a *halfline*) with origin 0. Every vector $ a \neq 0 $ contained in an open (resp. closed) half-line A is called a *direction vector* of $ A $, and $ A $ is the set of vectors $ ha $ for all scalars $ A > 0 $ (resp. $ A \geq 0 $). Every line $ D $ through 0 contains exactly two open (resp. closed) half-lines with origin 0 ; if $ A $ is one of these, then $ -A $ is the other (called the *opposite* of $ A $).

Now if $ F $ is an *affine space* over $ K $, and E the space of translations of F, then any subset of F of the form $ A = a + A_0 $, where $ \Delta_0 $ is an open (resp. closed) half-line of E, is called an *open* (resp. *closed*) *half-line with origin* $ a \in F $. The half-line $ \Delta_0 $ is completely determined by $ A $ (for it is the half-line with direction vector $ b - a $, for any $ b \neq a $ in $ A $), and is called the *direction* of $ A $; a direction vector of $ A $, is also called a *direction vector* of $ A $.

Suppose now that E has *finite* dimension $ n $ over K ; then it is known (III, p. 518, Cor. 1) that the *n-th exterior power* $ \Lambda^n E $ is a vector space of dimension 1 over K, and so the union of two opposite closed half-lines of origin 0. These half-lines are called orientations of E; the space E together with a given one of these half-lines A is said to be oriented; an n-vector z is then called positive (resp. negative) under this orientation if it belongs to A (resp. to −A); it is negative (resp. positive) under the opposite orientation.

An orientation of an affine space F over K is by definition an orientation of the space of translations of F; the space F, together with such an orientation, is called an oriented affine space.

Let E be an oriented vector space over K, of dimension $ n $; an ordered basis $ (a_i)_{1 \leq i \leq n} $ of E is called positive or direct (resp. negative or inverse) if the n-vector $ a_1 a_2 \ldots a_n $ is positive (resp. negative). If $ u $ is an automorphism of the vector space E then $ (\bigwedge^n u)(z) = \det(u) \cdot z $ for all $ z \in \bigwedge^n E $, so a necessary and sufficient condition for $ \bigwedge^n u $ to leave invariant the orientation of E (or, as we also say, to preserve the orientation) is that $ \det(u) > 0 $; the automorphisms having this property are precisely the automorphisms of E as an oriented vector space; they form a normal subgroup $ \mathrm{GL}^+(E) $ of the linear group $ \mathrm{GL}(E) $, which has index 2 whenever $ E \neq 0 $.

When $ E = 0 $ then $ \mathrm{GL}(E) = \mathrm{End}(E) $ contains only the identity map 1, and by definition $ \det(1_E) = 1 $. Note that $ \bigwedge^n E = \bigwedge^0 E = K $ by definition in this case; the half-line of K formed by the positive scalars is called the canonical orientation of the zero space.

Let M and N be two complementary subspaces of dimensions p and $ n - p $ respectively in the vector space E of dimension n; if $ z' $ (resp. $ z'' $) is a nonzero vector in $ \bigwedge^p M $ (resp. $ \bigwedge^{n-p} N $), then $ z' \wedge z'' $ is a nonzero vector in $ \bigwedge^n E $. Given an orientation on M and an orientation on N, the vectors $ z' \wedge z'' $ for positive $ z' $ and $ z'' $ form an orientation of E, called the product orientation of the orientation of M by the orientation of N (which depends on the order of the factors when $ p(n-p) $ is odd). Conversely, given orientations on E and on M, there exists a unique orientation on N such that the given orientation on E is the product of the given orientation on M and this orientation on N (in that order); this orientation is said to be complementary to the orientation of M with respect to that of E. If $ N' $ is a second complementary subspace to M, the canonical projection $ N \to N' $ parallel to M takes the complementary orientation of N onto that of $ N' $. The image of the complementary orientation of N under the canonical map $ N \to E/M $ is thus independent of the choice of complement N; it is called the quotient orientation on E/M of the orientation of E by that of M.

Exercises

### Exercises {#alg-vi-s2-exercises}

All rings under consideration are assumed to be commutative unless explicitly stated otherwise.

See the [exercises for § 2](exercises/s2/).
