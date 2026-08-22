---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 2
section_title: Zeros of polynomials
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.14-A IV.19, A IV.87-A IV.88
pdf_pages: 0023-0028, 0096-0097
extraction: ocr
subsections:
    - "no": 1
      title: Roots of a polynomial in one indeterminate. Multiplicity
      page: 14
      pdf_page: 23
    - "no": 2
      title: Differential criterion for the multiplicity of a root
      page: 17
      pdf_page: 26
    - "no": 3
      title: Polynomial functions on an infinite integral domain
      page: 17
      pdf_page: 26
statements: 19
exercises: 5
content_sha256: 4d07e5496ffa92896b6a8af8eb86890619c755fca813fec2af0ea6af12a558a0
---

## § 2. ZEROS OF POLYNOMIALS

### 1. Roots of a polynomial in one indeterminate. Multiplicity

Let $g \in A[(X_i)_{i \in I}]$ and let $E$ be a unital associative $A$-algebra. Let $x = (x_i)_{i \in I}$, be a family of pairwise permutable elements of $E$. We shall say that $x$ is a zero of $g$ in $E^l$ if $g(x) = 0$. If $f$ is a polynomial in a single indeterminate, a zero of $f$ in $E$ is also called a root of $f$ in $E$.

#### Proposition 1 {#alg-iv-s2-prop-1 .statement}

— Let $f \in A[X]$ and $\alpha \in A$. The remainder of the division of $f$ by $X - \alpha$ is $f(\alpha)$. For $\alpha$ to be a root of $f$ it is necessary and sufficient that $X - \alpha$ should be a divisor of $f$ in $A[X]$.

For if $ u,\ v \in \mathbf{A}[X] $ are such that $ f = (X - \alpha)\ u + v,\ \deg v < 1 $, then $ v $ is a scalar and $ f(a) = (a - a)\ u(\alpha) + v = v $. This proves the first assertion and the second follows from it.

#### Proposition 2 {#alg-iv-s2-prop-2 .statement}

— *Let $ f \in \mathbf{A}[X] $, $ a \in \mathbf{A} $, and let $ h $ be an integer $ \geq 0 $. The following conditions are equivalent*:
(i) $ f $ is divisible by $ (X - \alpha)^h $ but not by $ (X - \alpha)^{h-1} $;
(ii) *there exists $ g \in \mathbf{A}[X] $ such that $ f = (X - \alpha)^h g $ and $ g(a) \neq 0 $.
(i) $ \Rightarrow $ (ii) follows at once from Prop. 1.
(ii) $ \Rightarrow $ (i) : Suppose that $ f = (X - \alpha)^h g $, where $ g $ does not admit $ a $ as a root. Then $ f $ is divisible by $ (X - \alpha)^h $; if $ g_1 \in \mathbf{A}[X] $ existed such that $ f = (X - \alpha)^{h+1} g_1 $, then since $ (X - \alpha)^n $ is not a divisor of zero in $ \mathbf{A}[X] $ (IV, p. 9, Prop. 7), we have $ g = (X - a)\ g_1 $ and so $ g(\alpha) = 0 $, which is absurd.

#### Proposition 3 {#alg-iv-s2-prop-3 .statement}

— *Let $ f $ be a non-zero element of $ \mathbf{A}[X] $ and $ a \in \mathbf{A} $. There exists just one integer $ h \geq 0 $ satisfying the conditions (i) and (ii) of Prop. 2.*
This is clear for condition (i), bearing in mind the fact that iff is divisible by $ (X - \alpha)^h $, then $ \deg f \geq h $ (IV, p. 9, Prop. 7).

#### Definition 1 {#alg-iv-s2-def-1 .statement}

— *With the above notation we say that $ a $ is of order $ h $, or multiplicity $ h $ relative to $ f $.*
If $ h > 0 $ we also say that $ a $ is a root of order $ h $ or multiplicity $ h $ off. A root of order 1 is called a simple root, a root of order 2 a double root,... A root of order $ > 1 $ is said to be multiple.

#### Remark {#alg-iv-s2-n1-rem-1 .statement}

— 1) If $ f = 0 $ we agree to say that $ a $ has order $ \geq h $ relative to $ f $, whatever $ a \in \mathbf{A} $ and the integer $ h \geq 0 $. For any $ f \in \mathbf{A}[X] $ and $ a \in \mathbf{A} $, to say that $ a $ has order $ \geq h $ relative to $ f $ means that $ (X - \alpha)^h $ divides $ f $.
2) Let $ B $ be a commutative ring containing $ \mathbf{A} $ as subring. Let $ f \in \mathbf{A}[X] $ be non-zero and $ a \in \mathbf{A} $. The order of $ a $ relative to $ f $ is the same, whether we consider $ f $ as element of $ B[X] $ or as element of $ \mathbf{A}[X] $. This is clear from condition (ii) of Prop. 2.

#### Proposition 4 {#alg-iv-s2-prop-4 .statement}

— *Let $ f $ and $ g $ be non-zero elements of $ \mathbf{A}[X] $. Let $ a \in \mathbf{A} $, and let the orders of $ a $ relative to $ f $ and $ g $ be $ p $ and $ q $ respectively.*
(i) *The order of $ a $ relative to $ f + g $ is $ \geq \inf(p, q) $. It is equal to $ \inf(p, q) $ if $ p \neq q $*.
(ii) *The order of $ a $ relative to $ fg $ is $ \geq p + q $. It is equal to $ p + q $ if $ \mathbf{A} $ is an integral domain*.

For we have $ f(X) = (X - \alpha)^p f_1(X) $, $ g(X) = (X - \alpha)^q g_1(X) $ with $ f_1(\alpha) \neq 0 $, $ g_1(a) \neq 0 $. Suppose for example that $ p \leq q $; then we have
$$
f(X) + g(X) = (X - \alpha)^p (f_1(X) + (X - \alpha)^{q-p} g_1(X)) .
$$

and if $ p < q $, $ a $ is not a root of $ f_1(X) + (X - \alpha)^{q-p} g_1(X) $; this proves (i). On the other hand, we have $ f(X)g(X) = (X - \alpha)^{p+q} f_1(X)g_1(X) $ and $ f_1(\alpha)g_1(\alpha) \neq 0 $ if $ A $ is an integral domain; this proves (ii).

#### Proposition 5 {#alg-iv-s2-prop-5 .statement}

*Suppose that $ A $ is an integral domain. Let $ f $ be a non-zero element of $ A[X] $, and $ a,, \ldots, \alpha_p $ pairwise distinct roots of $ f $ in $ A $, of orders $ k_1, \ldots, k_r $. We have*

$$
f(X) = (X - \alpha_1)^{k_1}(X - \alpha_2)^{k_2} \ldots (X - \alpha_p)^{k_p} g(X)
$$

*where $ g \in A[X] $ and $ a,, \ldots, a, $ are not roots of $ g $.*

We proceed by induction on $ p $, the proposition being evident for $ p = 1 $, by Def. 1. Suppose then that $ f(X) = g_1(X)g_2(X) $, where

$$
g_1(X) = (X - \alpha_1)^{k_1} \ldots (X - \alpha_{p-1})^{k_{p-1}}, \quad g_2(X) \in A[X].
$$

Since $ A $ is an integral domain and $ \alpha_p $ is distinct from $ a,, \ldots, \alpha_{p-1} $ it follows that $ \alpha_p $ is not a root of $ g_1(X) $, hence $ \alpha_p $ is a root of order $ k_p $ of $ g_2(X) $ (Prop. 4, (ii)). It follows that $ g_2(X) $ is divisible by $ (X - \alpha_p)^{k_p} $, and so

$$
f(X) = (X - \alpha_1)^{k_1} \ldots (X - \alpha_p)^{k_p} g(X)
$$

where $ g(X) \in A[X] $. Clearly $ a,, \ldots, \alpha_p $ are not roots of $ g $.

#### Theorem 1 {#alg-iv-s2-thm-1 .statement}

*Let $ A $ be an integral domain. Given a non-zero element $ f $ of $ A[X] $, of degree $ n $, then the sum of the orders of all the roots off in $ A $ is $ \leq n $.*

This follows immediately from Prop. 5.

#### Corollary {#alg-iv-s2-n1-cor-1 .statement}

*Assume that $ A $ is an integral domain and let $ f, g \in A[X] $, of degrees $ \leq n $. If there exist $ n + 1 $ pairwise distinct elements $ x_1, \ldots, x_{n+1} $ of $ A $ such that $ f(x_i) = g(x_i) $ for $ 1 \leq i \leq n + 1 $, then $ f = g $.*

It suffices to apply Th. 1 to $ f - g $.

#### Proposition 6 (Lagrange interpolation formula) {#alg-iv-s2-prop-6 .statement}

— *Let $ K $ be a commutative field, $ \alpha_1, \alpha_2, \ldots, a, $ distinct elements of $ K $ and $ \beta_1, \beta_2, \ldots, \beta_n $ any elements of $ K $. For $ i = 1, 2, \ldots, n $ we put*

$$
f_i(X) = \prod_{j \in U(i)} (X - \alpha_j)/(\alpha_i - \alpha_j),
$$

*where $ U(i) $ is the set of integers $ j $ such that $ j \neq i $ and $ 1 \leq j \leq n $. Then $ \beta_1 f_1 + \ldots + \beta_n f_n $ is the unique element $ f $ of $ K[X] $ such that $ \deg f < n $ and $ f(\alpha_i) = \beta_i $ for $ 1 \leq i \leq n $.*

The uniqueness off follows from the Cor. to Th. 1. Let $ f = \beta_1 f_1 + \ldots + \beta_n f_n $, then since $ f_i $ has degree $ n - 1 $, we have $ \deg f < n $. On the other hand, $ f_i(\alpha_j) = 0 $ for $ j \neq i $ and $ f_i(\alpha_i) = 1 $, hence $ f(\alpha_i) = \beta_i $ for $ 1 \leq i \leq n $.

#### Corollary {#alg-iv-s2-n1-cor-2 .statement}

— Suppose that $ \mathbf{A} $ is an integral domain. Let $ f \in \mathbf{A}[X] $, of degree $ < n $, and let $ K $ be a subring of $ \mathbf{A} $ which is a field. If there exist $ n $ distinct elements $ \alpha_1, \ldots, a_n $ of $ \mathbf{A} $ such that $ \alpha_i \in K $ and $ f(\alpha_i) \in K $ for $ i = 1, \ldots, n $, then $ f \in K[X] $.

### 2. Differential criterion for the multiplicity of a root

#### Proposition 7 {#alg-iv-s2-prop-7 .statement}

— Let $ f \in \mathbf{A}[X] $ and let $ a \in \mathbf{A} $ be a root off: For $ a $ to be a simple root off it is necessary and sufficient that $ a $ should not be a root of the derivative $ Df $ of $ f $.

By hypothesis we have $ f = (X - a)\ g $, where $ g \in \mathbf{A}[X] $. For $ a $ to be a simple root of $ f $ it is necessary and sufficient that $ g(\alpha) \neq 0 $. Now we have $ Df = g + (X - \alpha)\ Dg $, whence $ (Df)(\alpha) = g(\alpha) $.

More generally:

#### Proposition 8 {#alg-iv-s2-prop-8 .statement}

— Let $ f \in \mathbf{A}[X] $ and $ a \in \mathbf{A} $, and suppose that $ a $ has order $ k \geq 1 $ relative to $ f $: Then $ a $ has order $ \geq k - 1 $ relative to $ Df $. If $ k . 1 $ is cancellable in $ \mathbf{A} $, then $ a $ has order $ k - 1 $ relative to $ Df $.

By hypothesis there exists $ g \in \mathbf{A}[X] $ such that $ f = (X - a)^k g $ and $ g(a) \neq 0 $. Hence $ Df = k(X - \alpha)^{k-1}g + (X - \alpha)^k Dg = (X - \alpha)^{k-1}(kg + (X - \alpha)\ Dg) $, which establishes the first part of the proposition. The value of $ kg + (X - \alpha)\ Dg $ for $ X = \alpha $ is $ kg(a) $, and this is non-zero if $ k . 1 $ is cancellable in $ \mathbf{A} $; this proves the second part of the proposition.

Let $ k $ be an integer $ > 0 $ such that $ k . 1 = 0 $ in $ \mathbf{A} $. If $ f(X) = X^k $, then $ 0 $ is a root of order $ k $ of $ f $, and a root of arbitrarily high order of $ Df $.

#### Corollary {#alg-iv-s2-n2-cor-1 .statement}

— Let $ f \in \mathbf{A}[X] $, $ a \in \mathbf{A} $ and $ p $ an integer $ \geq 0 $, further, suppose that $ p! . 1 $ is cancellable in $ \mathbf{A} $. Then for $ a $ to be a root of order $ p $ of $ f $, it is necessary and sufficient that $ a $ should be a root of $ f, Df, ..., D^{p-1}f $ and not a root of $ D^pf $.

This follows from Prop. 8 by induction on $ p $.

### 3. Polynomial functions on an infinite integral domain

#### Proposition 9 {#alg-iv-s2-prop-9 .statement}

— Assume that $ A $ is an integral domain. Let $ I $ be a set, $ (\mathbf{H}_i)_{i \in I} $ a family of infinite subsets of $ \mathbf{A} $ and $ H = \prod_{i \in I} \mathbf{H}_i \subset A' $. Iff is a non-zero element of $ \mathbf{A}[(X_i)_{i \in I}] $, and $ H_f $ the set of all $ x \in H $ such that $ f(x) \neq 0 $, then $ H $ and $ H_f $ are equipotent.

a) First suppose that $ I $ is finite and put $ n = \mathrm{Card}\ I $. The proposition is clear for $ n = 0 $; we shall prove it by induction on $ n $. Choose an element $ i_0 $ of $ I $ and put $ J = I - \{i_0\} $, $ B = \mathbf{A}[(X_i)_{i \in J}] $. Since $ f \neq 0 $, we can write $ f = \sum_{k=0}^m g_k X_{i_0}^k $, where g_0, \ldots, g_m \in B \text{ and } g_m \neq 0. \text{ By the induction hypothesis the set K of all } x \in \prod_{i \in s} H_i \text{ such that } g_m(x) \neq 0 \text{ is equipotent with } \prod_{i \in J} H_i. \text{ For } x \in K \text{ the polynomial}
$$
h(X_{i_0}) = \sum_{k=0}^m g_k(x) X_{i_0}^k \in A[X_{i_0}]
$$
is non-zero. By Th. 1 (IV, p. 16) the set of $ a \in H_{i_0} $ such that $ h(\alpha) \neq 0 $ is equipotent with $ H_{i_0} $ whence
$$
\operatorname{Card} H \geq \operatorname{Card} H_f \geq (\operatorname{Card} K) \cdot (\operatorname{Card} H_{i_0}) = \operatorname{Card} H,
$$
and so $ \operatorname{Card} H = \operatorname{Card} H_f $.

b) In the general case there is a finite subset $ I' $ of I such that $ f \in A[(X_i)_{i \in I'}] $. Let $ H'_f $ be the set of all $ x \in \prod_{i \in I'} H_i $ such that $ f(x) \neq 0 $. Then
$$
H_f = H'_f \times \left( \prod_{i \in I - I'} H_i \right),
$$
and it suffices to apply the first part of the proof to $ H'_f $.

#### Corollary 1 {#alg-iv-s2-prop-9-cor-1 .statement}

— *We keep the hypothesis and notation of Prop. 9. If l is non-empty, then $ H_f $ is infinite.*

#### Corollary 2 {#alg-iv-s2-prop-9-cor-2 .statement}

— *Suppose that A is an infinite integral domain or that A is an algebra over an infinite field. For every $ f \in A[(X_i)_{i \in I}] $, let $ \tilde{f}: A^I \to A $ be the polynomial function defined by f (IV, p. 4). Then the mapping $ f \mapsto \tilde{f} $ is injective.*

When A is an infinite integral domain, the corollary follows at once from Prop. 9. Suppose that A is an algebra over an infinite field k. Let $ f = \sum_{v \in \mathbf{N}^{(I)}} \alpha_v X^v $ be a non-zero element of $ A[(X_i)_{i \in I}] $; then there exists $ v_0 \in \mathbf{N}^{(I)} $ such that $ \alpha_{v_0} \neq 0 $, and a k-linear form $ \varphi $ on A such that $ \varphi(\alpha_{v_0}) \neq 0 $. Let $ g = \sum_{v \in \mathbf{N}^{(I)}} \varphi(a_v) X^v \in k[(X_i)_{i \in I}] $; we have $ g \neq 0 $, hence there exists $ x \in k^I $ such that $ g(x) \neq 0 $. Then $ \varphi(f(x)) = g(x) \neq 0 $, and so $ f(x) \neq 0 $.

When A is an infinite integral domain or when A is an algebra over an infinite field, we shall usually identify f with $ \tilde{f} $.

Suppose that A is finite and let $ f(X) = \prod_{a \in A} (X - a) $, then $ f \neq 0 $, but $ \tilde{f} = 0 $. For other examples see IV, p. 88, exercises 7 and 8.

#### Theorem 2 (Principle of extension of algebraic identities) {#alg-iv-s2-thm-2 .statement}

— *Suppose that A is an infinite integral domain. Let $ g_1, \ldots, g_m, f $ be elements of $ A[(X_i)_{i \in I}] $ and assume the following hypotheses:*

a) $ g_1 \neq 0, \ldots, g_m \neq 0 $;
b) *for all* $ x \in \mathbf{A}^1 $ *such that* $ g_1(x) \neq 0, \ldots, g_m(x) \neq 0 $, *we have* $ f(x) = 0 $. *Then* $ f = 0 $.

For if $ f \neq 0 $, we have $ fg_1 \ldots g_m \neq 0 $ (IV, p. 9, Prop. 8), hence there exists $ x \in \mathbf{A}^1 $ such that $ f(x)g_1(x) \ldots g_m(x) \neq 0 $ (IV, p. 18, Cor. 2), which contradicts the hypothesis.

#### Scholium {#alg-iv-s2-n3-sch-1 .statement}

— Let A be an integral domain and $ f \in A[(X_i)_{i \in I}] $. Th. 2 provides a convenient means of proving that $ f = 0 $. It suffices to consider an infinite integral domain E containing A as subring; if we can show that $ f((x_i)) = 0 $ for all $ (x_i) \in E^I $ (or even for those $ (x_i) \in E^I $ at which a finite number of given non-zero polynomials do not vanish) then it follows that $ f = 0 $. If A itself is not infinite, we can for example take E to be the ring $ A[X] $ or its field of fractions.

Once we have proved the relation $ f = 0 $, we can clearly deduce that $ f((y_i)) = 0 $ for all $ (y_i) \in F^I $ where F is any unital associative and commutative A-algebra whatsoever; in particular F may be finite or non-integral.

In other words, the proof of the identity $ f((x_i)) = 0 $ when the $ x_i $ run over an infinite integral domain containing A as subring (with the possible restriction that $ g_k((x_i)) \neq 0 $ for $ 1 \leq k \leq m $, where the $ g_k $ are non-zero polynomials) implies the same identity when the $ x_i $ run over any unital associative and commutative A-algebra.

In particular let $ f \in Z[(X_i)_{i \in I}] $. If $ f((x_i)) = 0 $ when the $ x_i $ run over $ \mathbf{Z} $ (with the possible restriction that $ g_k((x_i)) \neq 0 $ for $ 1 \leq k \leq m $, where the $ g_k $ are non-zero elements of $ \mathbf{Z}[(X_i)] $), then we have the same identity when the $ x_i $ run over an arbitrary commutative ring.

### Exercises {#alg-iv-s2-exercises}

See the [exercises for § 2](exercises/s2/).
