---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 4
section_title: Formal power series
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.24-A IV.41, A IV.90-A IV.91
pdf_pages: 0033-0050, 0099-0100
extraction: ocr
subsections:
    - "no": 1
      title: Definition of formal power series. Order
      page: 24
      pdf_page: 33
    - "no": 2
      title: Topology on the set of formal power series. Summable families
      page: 25
      pdf_page: 34
    - "no": 3
      title: Substitutions
      page: 28
      pdf_page: 37
    - "no": 4
      title: Invertible formal power series
      page: 30
      pdf_page: 39
    - "no": 5
      title: Taylor's formula for formal power series
      page: 31
      pdf_page: 40
    - "no": 6
      title: Derivations in the algebra of formal power series
      page: 32
      pdf_page: 41
    - "no": 7
      title: The solution of equations in a formal power series ring
      page: 35
      pdf_page: 44
    - "no": 8
      title: Formal power series over an integral domain
      page: 38
      pdf_page: 47
    - "no": 9
      title: The field of fractions of the ring of formal power series in one indeterminate over a field
      page: 38
      pdf_page: 47
    - "no": 10
      title: Exponential and logarithm
      page: 39
      pdf_page: 48
statements: 23
exercises: 8
content_sha256: 81016120a022e796b4c0327b728d5c57805c5049830f949f0afbf59ce3e325ce
---

## § 4. FORMAL POWER SERIES

### 1. Definition of formal power series. Order

Let I be a set. We recall (III, p. 454 and 456) that the total algebra of the monoid $ N^{(I)} $ over A is called *the algebra of formal power series with respect to the indeterminates* $ X_i \ (i \in I) $ (or in the indeterminates $ X_i $) *with coefficients in* A. It is denoted by $ A[[X_i]]_{i \in I} $ or $ A[[((X_i)_{i \in I}]] $ or also $ A[[X]] $, ondenoting by X the family $ (X_i)_{i \in I} $: in this paragraph we shall mainly use the notation $ A[[I]] $. Sometimes it is convenient to designate the canonical image in $ A[[I]] $ of the element i of I by a symbol other than $ X_i $, for example $ Y_i, Z_i, T_i, \ldots $; the conventions used in this case are analogous to those for polynomials (IV, p. 1). The algebra $ A[[I]] $ is then designated by $ A[[Y_i]]_{i \in I} $, or $ A[[Y]] $ etc.

When I is a finite set of p elements, we also say that $ A[[I]] $ is an algebra of formal power series in p indeterminates. These algebras are all isomorphic, for fixed p. An algebra of formal power series in 1, 2, ... indeterminates will also be denoted by $ A[[X]] $, $ A[[U, V]] $, ..., the set I of indices not being specified.

A formal power series u is conventionally written $ u = \sum_{v \in N^{(I)}} a_v X^v $ (cf. IV, p. 1).

The $ \alpha_v $ are the *coefficients* of $ u $; there may be infinitely many of them $ \neq 0 $. The $ a_v X^v $ are called *terms* of $ u $; for u to be a polynomial it is necessary and sufficient that $ u $ should have only a finite number of terms $ \neq 0 $. The terms $ a_v X^v $ such that |ν| = p are called the terms of total degree p. The formal power series $ u_p = \sum_{|\nu|=p} \alpha_\nu X^\nu $ is called the *homogeneous component of degree* p of u (it is a polynomial when I is finite); $ u_0 $ is identified with an element of A called also the *constant term* of u. We say that u is homogeneous of degree p if $ u = u_p $. If $ u, v \in \mathbf{A}[[\mathrm{I}]] $ and $ w = uv $, we have

(1)
$$
w_p = \sum_{q+r=p} u_q v_r
$$
for every integer $ p \geq 0 $.

We recall (III, p. 456), that the *order* $ \omega(u) $ of a formal power series $ u \neq 0 $ is the least integer p such that $ u_p \neq 0 $. We shall agree to adjoin to Z an element written $ \infty $ and extend the order relation and addition from Z to $ Z \cup \{\infty\} $ by the conventions
$$
n < \infty,\quad \infty + \infty = \infty,\quad \infty + n = n + \infty = \infty
$$
for every $ n \in Z $; we also put $ \omega(0) = \infty $. With these conventions we have the relations
$$
\begin{align*}
\omega(u+v) &\geq \inf(\omega(u), \omega(v)), \\
\omega(u+v) &= \inf(\omega(u), \omega(v)) \text{ if } \omega(u) \neq \omega(v), \\
\omega(uv) &\geq \omega(u) + \omega(v),
\end{align*}
$$
for any formal power series $ u $ and $ v $ in $ \mathbf{A}[[\mathrm{I}]] $.

We recall (III, p. 457) that for any subset J of I we identify $ \mathbf{A}[[\mathrm{I}]] $ with $ \mathbf{A}[[\mathrm{I}-J]] [[\mathrm{J}]] $, which allows us to define the order $ \omega_J(u) $ of a formal power series with respect to the $ X_j $ ($ j \in J $), the homogeneous component of $ u $ with respect to the $ X_j $ ($ j \in J $) etc.

Let $ \varphi $ be a homomorphism of A into a ring B. We extend $ \varphi $ to a homomorphism $ \overline{\varphi} $ of $ \mathbf{A}[[\mathrm{I}]] $ into $ B[[\mathrm{I}]] $ by letting each formal power series $ u = \sum \alpha_\nu X^\nu $ correspond to the formal power series $ \sum \varphi(\alpha_\nu) X^\nu $; we say that the latter is obtained by *applying* $ \varphi $ *to the coefficients of the formal power series* u. We shall sometimes write $ ^\varphi u $ for $ \overline{\varphi}(u) $.

In particular if A is a subring of B and $ \varphi $ the canonical injection of A into B, then the homomorphism $ \overline{\varphi} $ of $ \mathbf{A}[[\mathrm{I}]] $ into $ B[[\mathrm{I}]] $ is injective; we shall in general identify $ \mathbf{A}[[\mathrm{I}]] $ with a subring of $ B[[\mathrm{I}]] $ by means of $ \overline{\varphi} $.

### 2. Topology on the set of formal power series. Summable families

By definition $ \mathbf{A}[[\mathrm{I}]] $ is nothing other than the product set $ \mathbf{A}^{N^{(I)}} $. Except for express mention to the contrary we shall equip A with the discrete topology and $ \mathbf{A}[[\mathrm{I}]] $ with the product topology (Gen. Top. I, p. 31 f.) which we shall call the canonical topology. Equipped with addition and the discrete topology, $ A $ is a separated and complete topological group; hence for addition $ A[[I]] $ is a separated and complete topological group (Gen. Top., III, p. 238 and 242 and Gen. Top., II, p. 187). Moreover the algebra $ A[(X_i)_{i \in I}] $ of polynomials is dense in $ A[[I]] $ (Gen. Top., III p. 238, Prop, 25) and we may thus consider $ A[[I]] $ as the completion of $ A[(X_i)_{i \in I}] $.

For each $ \beta \in \mathbf{N}^{(I)} $ let $ S_\beta $ be the set of multi-indices $ v $ such that $ v \leq \beta $ and let $ a_\beta $ be the set of formal power series $ u = \sum \alpha_v X^v $ such that $ a_v = 0 $ for $ v \in S_\beta $. Clearly $ S_\beta $ is a finite subset of $ \mathbf{N}^{(I)} $, and every finite subset of $ \mathbf{N}^{(I)} $ is contained in a set of the form $ S_\beta $. It follows that the family $ (a_\beta)_{\beta \in \mathbf{N}^{(I)}} $ is a fundamental system of neighbourhoods of 0 in $ A[[I]] $. The sets $ a_\beta $ are ideals in $ A[[I]] $, hence (Gen. Top., III, p. 275) $ A[[I]] $ is a topological ring.

#### Lemma 1 {#alg-iv-s4-lem-1 .statement}

— Let $ L $ be an infinite set and $ (u_\lambda)_{\lambda \in L} $ a family of elements of $ A[[I]] $, and put $ u_\lambda = \sum \alpha_{\lambda,v} X^v $ for $ \lambda \in L $. Then the following conditions are equivalent:
(i) The family $ (u_\lambda)_{\lambda \in L} $ is summable (Gen. Top., III, p. 262) in $ A[[I]] $.
(ii) We have $ \lim u_\lambda = 0 $, taken along *the filter* of complements of finite subsets of $ L $.
(iii) For every $ v \in \mathbf{N}^{(I)} $ we have $ \alpha_{\lambda,v} = 0 $ except for a *finite* number of indices $ \lambda \in L $.

When these conditions hold, the series $ u = \sum_{\lambda \in L} u_\lambda $ is equal to $ \sum \alpha_v X^v $ with $ a_v = \sum_{\lambda \in L} \alpha_{\lambda,v} $ for each $ v \in \mathbf{N}^{(I)} $.

The equivalence of (i) and (ii) follows from Cor. 2 of Gen. Top., III, p. 263.
The equivalence of (ii) and (iii) follows from the properties of limits in a product space (Gen. Top., I, p. 55, Cor. 1).
The last assertion follows from Prop. 4 of Gen. Top., III, p. 266.

Let us give some examples of summable families.
a) Let $ u \in A[[I]] $ and let $ a_v $ be the coefficient of $ X^v $ in $ u $. The family $ (\alpha_v X^v)_{v \in \mathbf{N}^{(I)}} $ is then summable, with sum $ u $ (which justifies writing $ u = \sum \alpha_v X^v $).

b) Let $ u \in A[[I]] $; for every integer $ p \geq 0 $ let $ u_p $ be the homogeneous component of degree $ p $ of $ u $. Then the family $ (u_p)_{p \geq 0} $ is summable and we have $ u = \sum_{p \geq 0} u_p $.

c) Let $ (u_\lambda)_{\lambda \in L} $ be a family of elements of $ A[[I]] $ and suppose that for every integer $ n \geq 0 $ the set of $ \lambda \in L $ such that $ \omega(u_\lambda) < n $ is finite. Then the family $ (u_\lambda)_{\lambda \in L} $ is summable.

#### Remark {#alg-iv-s4-n2-rem-1 .statement}

— Suppose that $ I $ is *finite*. For every integer $ n \geq 0 $ let $ b_n $ be the set of formal power series $ u \in A[[I]] $ such that $ \omega(u) \geq n $. The sequence $ (b_n)_{n \geq 0} $ is a fundamental system of neighbourhoods of 0 in $ \mathbf{A}[[\mathbf{I}]] $. Therefore a family of elements $ u_\lambda $ of $ \mathbf{A}[[\mathbf{I}]] $ ($ \lambda \in L $) is summable if and only if for every $ n \in \mathbf{N} $ the set of $ \mathbf{A} \in L $ such that $ \omega(u_\lambda) < n $ is finite.

#### Proposition 1 {#alg-iv-s4-prop-1 .statement}

*Let* $ (u,)_{\mu \in \mathcal{J}} $ *and* $ (v_\mu)_{\mu \in \mathcal{J}} $ *be two summable families of elements of* $ \mathbf{A}[[\mathbf{I}]] $. *Then the family* $ (u_\lambda v_\mu)_{(\lambda, \mu) \in \mathcal{J} \times M} $ *is summable and we have*

$$
\sum_{(\lambda, \mu) \in L \times M} u_\lambda v_\mu = \left( \sum_{\lambda \in L} u_\lambda \right) \left( \sum_{\mu \in M} v_\mu \right)
$$

Let $ (\alpha_{\lambda, \nu})_{\nu \in \mathbf{N}^{(1)}} $ (resp. $ (\beta_{\mu, \nu})_{\nu \in \mathbf{N}^{(1)}} $) be the family of coefficients of $ u_\lambda $ (resp. $ v_\nu $). For each $ \nu \in \mathbf{N}^{(1)} $ there exists only a finite number of pairs $ (\nu_1, \nu_2) \in \mathbf{N}^{(1)} \times \mathbf{N}^{(1)} $ such that $ \nu_1 + \nu_2 = \nu $, hence only a finite number of pairs $ (\lambda, \mu) \in L \times M $ such that the coefficient of $ X^\nu $ in $ u_\lambda v_\mu $ is $ \neq 0 $. Hence the family $ (u_\lambda v_\mu)_{(\lambda, \mu) \in L \times \mathcal{J}} $ is summable. Now the formula (2) follows from the associativity of the sum (Gen. Top., III, p. 265, formula (2)).

In $ \mathbf{A}[[\mathbf{I}]] $ the product is an associative and commutative composition law. We may therefore speak of a *multipliable family* of elements of $ \mathbf{A}[[\mathbf{I}]] $ and of the *product* of a multipliable family (Gen. Top., III, p. 262, remark 3).

#### Proposition 2 {#alg-iv-s4-prop-2 .statement}

*Let* $ (u_\lambda)_\lambda $ *be a summable family of elements of* $ \mathbf{A}[[\mathbf{I}]] $.
(i) *The family* $ (1 + u_\lambda)_\lambda $ *is multipliable*.
(ii) *Let* $ \mathfrak{T} $ *be the set of all finite subsets of* $ L $. *For any* $ M \in \mathcal{S} $ *put* $ u_M = \prod_{\lambda \in M} u_\lambda $. *Then the family* $ (u_M)_{M \in \mathfrak{T}} $ *is summable and we have*

$$
\sum_{M \in \mathfrak{T}} u_M = \prod_{\lambda \in L} (1 + u_\lambda).
$$

Let us define the ideals $ \mathfrak{a}_\beta $ as at the beginning of this No., and let $ \beta \in \mathbf{N}^{(1)} $. There exists a finite subset $ L_0 $ of $ L $ such that $ u_\lambda \in \mathfrak{a}_\beta $ for $ \lambda \notin L_0 $. Then for every $ M \in \mathcal{S} $ such that $ M \not\subset L_0 $ we have $ u_M \in \mathfrak{a}_\beta $. It follows that the family $ (u_M)_{M \in \mathfrak{T}} $ is summable. On the other hand, for any finite subset $ M_0 $ of $ L $ we have

$$
\sum_{M \subset M_0} u_M = \prod_{\lambda \in M_0} (1 + u_\lambda).
$$

Taken along the filtered ordered set $ \mathfrak{T} $, the left-hand side has as limit $ \sum_{M \in \mathfrak{T}} u_M $. Hence the right-hand side has as limit $ \sum_{M \in \mathfrak{T}} u_M $, which proves (i) and (ii) at the same time.

#### Proposition 3 {#alg-iv-s4-prop-3 .statement}

*Let* $ u = \sum a_\nu X^\nu \in \mathbf{A}[[\mathbf{I}]] $ *and* $ m $ *an integer* $ > 0 $. *For every* $ n \in \mathbf{N} $ *let* $ (\alpha_{\nu, n})_{\nu \in \mathbf{N}^{(1)}} $ *be the family of coefficients of* $ u^n $. *If* $ \alpha_0^m = 0 $, *then* $ \alpha_{\nu, n} = 0 $ *for* $ n \geq |\nu| + m $.

Let $ v \in \mathbf{N}^{(1)} $ and $ n \in \mathbf{N} $. We have

$$
\alpha_{v,n} = \sum_{v(1) + \cdots + v(n) = v} \alpha_{v(1)} \cdots \alpha_{v(n)} .
$$

If $ n \geq |v| + m $ and $ v(1) + \cdots + v(n) = v $, we have $ |v(1)| + \cdots + |v(n)| \leq n - m $. We thus have $ v(r) = 0 $ and so $ \alpha_{v(r)} = a_r $, for at least $ m $ distinct values of $ r $; it follows that $ \alpha_{v(1)} \cdots \alpha_{v(n)} = 0 $, whence the result.

#### Corollary {#alg-iv-s4-n2-cor-1 .statement}

— Let $ u \in A[[I]] $; then for $ \lim_{n \to \infty} u^n = 0 $ to hold it is necessary and sufficient that the constant term of $ u $ should be nilpotent.

Let $ a_0 $ be the constant term of $ u $. The constant term of $ u^n $ is $ \alpha_0^n $, hence the stated condition is necessary; it is sufficient by Prop. 3.

### 3. Substitutions

Let $ E $ be an $ A $-algebra. A topology on $ E $ is said to be linear if it is invariant under translation and if there exists a fundamental system of neighbourhoods of 0 consisting of ideals of $ E $ (Gen. Top., III, p. 223). The topology on $ E $ is then compatible with its $ A $-algebra structure (when $ A $ carries the discrete topology). An $ A $-algebra with a linear topology is called a linearly topologized $ A $-algebra.

#### Proposition 4 {#alg-iv-s4-prop-4 .statement}

— Let $ I $ be a set and $ E $ an associative, commutative, unital, linearly topologized separated complete $ A $-algebra.

(i) Let $ \varphi $ be a continuous homomorphism of $ A[[I]] $ into $ E $ and $ x_i = \varphi(X_i) $. Then:
(a) for all $ i \in I $, $ x_i^n $ tends to 0 as $ n $ tends to $ + \infty $;
(b) if $ I $ is infinite, $ x_i $ tends to 0 along the filter of complements of finite subsets of $ I $.

(ii) Let $ x = (x_i)_i $, $ _I $ be a family of elements of $ E $ satisfying a) and b) of (i). Then there exists one and only one unital continuous homomorphism $ \varphi $ of $ A[[I]] $ into $ E $ such that $ \varphi(X_i) = x_i $ for all $ i \in I $.

For all $ i \in I $, $ X_i^n $ clearly tends to 0 in $ A[[I]] $ as $ n $ tends to $ + \infty $; on the other hand when $ I $ is infinite, $ X_i $ tends to 0 along the filter of complements of finite subsets of $ I $. This proves (i).

Let $ (x_i)_{i \in I} $ be a family of elements of $ E $ satisfying conditions a) and b) of (i), let $ \psi $ be the homomorphism $ u \mapsto u((x_i)_{i \in I}) $ of $ A[(X_i)_{i \in I}] $ into $ E $, and let $ V $ be a neighbourhood of 0 of $ E $ which is an ideal of $ E $. By b) there exists a finite subset $ J $ of $ I $ such that $ x_i \in V $ for all $ i \in I - J $. Next there exists by a) an integer $ n \geq 0 $ such that $ x_i^n \in V $ for all $ i \in J $. Let $ \beta $ be the element of $ \mathbf{N}^{(I)} $ such that $ \beta_i = n - 1 $ for $ i \in J $ and $ \beta_i = 0 $ for $ i \in I - J $. If we define the ideal $ a_\beta $ of $ A[[I]] $ as at the beginning of No. 2 (IV, p. 26), then

$$
u \in A[(X_i)_{i \in I}] \cap a_\beta \Rightarrow \psi(u) \in V
$$

This shows that $ \psi $ is continuous if we equip $ A[(X_i)_{i \in I}] $ with the topology induced by that of $ A[[I]] $. Since $ E $ is separated and complete, $ \psi $ extends to a continuous unital homomorphism $ \varphi $ of $ A[[I]] $ into $ E $. We have $ \varphi(X_i) = \psi(X_i) = x_i $ for all $ i \in I $. Finally let $ \varphi' $ be a continuous unital homomorphism of $ A[[I]] $ into $ E $ such that $ \varphi'(X_i) = x_i $. We have $ \varphi'(u) = \varphi(u) $ for all $ u \in A[(X_i)_{i \in I}] $, hence $ \varphi' = \varphi $ because $ A[(X_i)_{i \in I}] $ is dense in $ A[[I]] $.

Let us keep the previous notation. If $ u \in A[[I]] $, the image of $ u $ by $ \varphi $ is denoted by $ u(x) $ or $ u((x_i)_{i \in I}) $ (or also $ u(x_1, ..., x_n) $ if $ I = (1, 2, ..., n) $) and is called the element of $ E $ obtained by substitution of $ x_i $ for $ X_i $ in $ u $, or the value of $ u $ for the values $ x_i $ of the $ X_i $ or also the value of $ u $ for $ X_i = x_i $. In particular we have $ u = u((X_i)_{i \in I}) $.

Let $ E' $ be an associative commutative and unital linearly topologized separated and complete $ A $-algebra. Let $ \lambda $ be a continuous unital homomorphism of $ E $ into $ E' $, and $ (x_i)_{i \in I} $ a family of elements of $ E $ satisfying conditions $ a) $ and $ b) $ of Prop. 4 (IV, p. 28). The family $ (\lambda(x_i))_{i \in I} $ satisfies the same conditions $ a) $ and $ b) $. For every $ u \in A[[I]] $ we have

$$
\lambda(u((x_i)_{i \in I})) = u((\lambda(x_i))_{i \in I}),
$$

for the mapping $ u \mapsto A(u((x_i)_{i \in I})) $ is a continuous unital homomorphism of $ A[[I]] $ into $ E' $ which transforms $ X_i $ into $ \lambda(x_i) $ for all $ i \in I $.

If $ J $ and $ K $ are two sets, we denote by $ A_{J, K} $ the set of all families $ (g_j)_{j \in J} $ satisfying the following conditions:
(i) for all $ j \in J $, $ g_j $ is an element of $ A[[K]] $ whose constant term is nilpotent;
(ii) if $ J $ is infinite, $ g_j $ tends to 0 along the filter of complements of finite subsets of $ J $.

We note that if $ J $ is finite, every family of formal power series $ (g_j)_{j \in J} $ without constant term in $ A[[K]] $ belongs to $ A_{J, K} $.

Let $ (g_j)_{j \in J} $ be in $ A_{J, K} $. By the Cor. of Prop. 3 (IV, p. 28) we have $ \lim_{n \to \infty} g_j^n = 0 $ for all $ j \in J $. Let $ f \in A[[J]] $; we can substitute $ g_j $ for the variable of index $ j $ in $ f $ and obtain a formal power series $ f((g_j)_{j \in J}) $ belonging to $ A[[K]] $. Moreover, the mapping $ f \mapsto f((g_j)_{j \in J}) $ is a continuous homomorphism of $ A $-algebras $ A[[J]] $ into $ A[[K]] $.

In particular if $ J = (1, ..., p) $ and $ f \in A[[X_1, ..., X_p]] $, we can substitute for each $ X_j $ a formal power series $ g_j \in A[[K]] $ without constant term; the result of this substitution is written $ f(g_1, ..., g_p) $.

Let $ x = (x_k)_{k \in K} $ be a family of elements of $ E $ satisfying conditions $ a) $ and $ b) $ of Prop. 4 (IV, p. 28). Let us apply (3), taking for $ A $ the homomorphism $ u \mapsto u(x) $ of $ A[[K]] $ into $ E $; we obtain

$$
f((g_j)_{j \in J})(x) = f((g_j(x))_{j \in J}).
$$

Let $ f = (f_i)_{i \in I} \in (A[[J]])^I $ and $ g = (g_j)_{j \in J} \in A_{J, K} $. We denote by $ f(g) $ or $ f \circ g $ the element $ (f_i((g_j),_{\epsilon_J}))_{i \in I} $ of $ (A[[K]])^I $. If $ f \in A_{I, J} $, we have $ f \circ g \in A_{,,K} $ because the mapping $ f \mapsto f((g_j)_{i, J}) $ of $ A[[I]] $ into $ A[[K]] $ is continuous.

Let $ f \in (A[[J]])^I $, $ g \in A_{J, K} $, $ h \in A_{K, L} $. Then $ g \circ h \in A_{J, L} $ and by (4), we have
$$
(f \circ g) \circ h = f \circ (g \circ h).
$$

### 4. Invertible formal power series

#### Proposition 5 {#alg-iv-s4-prop-5 .statement}

— *In the ring $ A[[T]] $ of formal power series in one indeterminate the polynomial $ 1 - T $ is invertible, and we have* $ (1 - T)^{-1} = \sum_{n=0}^m T^n $.

For
$$
(1 - T) \left( \sum_{n=0}^\infty T^n \right) = \sum_{n=0}^\infty T^n - \sum_{n=0}^\infty T^{n+1} = 1.
$$

#### Proposition 6 {#alg-iv-s4-prop-6 .statement}

— *Let $ u \in A[[I]] $; then for $ u $ to be invertible in $ A[[T]] $ it is necessary and sufficient that its constant term should be invertible in $ A $.*

Suppose that there exists $ v \in A[[I]] $ such that $ uv = 1 $. Let $ a, \beta $ be the constant terms of $ u $ and $ v $, then $ \alpha \beta = 1 $, so $ a $ is invertible.

Conversely, suppose that the constant term $ a $ of $ u $ is invertible. Then there exists a formal power series $ t \in A[[I]] $ such that $ u = \alpha (1 - t) $ and $ \omega(t) > 0 $. Now there is a ring homomorphism $ \varphi : A[[T]] \to A[[I]] $ such that $ \varphi(T) = t $, and $ 1 - T $ is invertible in $ A[[T]] $ (Prop. 5); consequently $ 1 - t $ is invertible in $ A[[I]] $, and hence so is $ u $.

#### Remark {#alg-iv-s4-n4-rem-1 .statement}

— Let $ A $ be the set of all formal power series with constant term 1. By Prop. 6, $ M $ is a commutative group under multiplication; the multiplicative group of $ A[[I]] $ is thus the direct product of $ M $ and the multiplicative group of $ A $. We shall equip $ A $ with the topology induced from that of $ A[[I]] $. For each $ \beta \in \mathbf{N}^{(1)} $ we have in IV, p. 26 defined the ideal $ a_\beta $ of $ A[[I]] $; then $ 1 + a_\beta $ is a subgroup of $ M $ and the family $ (1 + a_{\beta'}) $ is a fundamental system of neighbourhoods of 1 in $ M $. Since the multiplication in $ M $ is continuous, we see that $ A $ is a topological group (Gen. Top., III, p. 223); in other words, the *mapping* $ f \mapsto f^{-1} $ *is continuous in* $ M $.

Let $ K $ be a commutative field and $ \mathcal{O} $ the subring of the field of rational fractions $ K((X_i)_{i,,}) $ formed of rational fractions in which the element 0 of $ K^1 $ is substitutable. If $ f \in \mathcal{O} $, we have $ f = \frac{u}{v} $, where $ u $ and $ v $ are polynomials such that the constant term of $ v $ is $ \neq 0 $, hence $ v $ is invertible in $ K[[I]] $. We can verify at once that the element $ uv^{-1} $ of $ K[[I]] $ depends only on $ f $; we say that the formal power series $ uv^{-1} $ is the *expansion at the origin of the rational fraction* $ \frac{u}{v} $. The mapping $ f \mapsto uv^{-1} $ is an injective homomorphism of $ \mathcal{O} $ into $ K[[I]] $; we shall often identify $ \mathcal{O} $ with its image under this mapping.

### 5. Taylor's formula for formal power series

Let $ X = (X_i)_{i \in I} $ and $ Y = (Y_i)_{i \in I} $, be two families of indeterminates relative to the same index set I. We denote by $ X + Y $ the family $ (X_i + Y_i)_{i \in I} $, of formal power series in $ A[[X, Y]] $. It is clear that we can substitute $ X_i + Y_i $ for $ X_i $ in a formal power series $ u \in A[[X]] $, the result being written $ u(X + Y) $. For each $ v \in \mathbf{N}^{(I)} $ we denote by $ \Delta^v u $ the coefficient of $ Y^v $ in the formal power series $ u(X + Y) $ considered as belonging to $ A[[X]][[Y]] $ (III, p. 456). In other words, we have

$$
u(X + Y) = \sum_v \Delta^v u(X) \cdot Y^v \quad (u \in A[[X]]) .
$$

Substituting $ (0, X) $ for $ (X, Y) $ we obtain

$$
u(X) = \sum_v \Delta^v u(0) \cdot X^v ;
$$

In other words, the constant term of $ \Delta^v u $ is the coefficient of $ X^v $ in $ u $. Since the mapping $ u \mapsto u(X + Y) $ of $ A[[X]] $ into $ A[[X, Y]] $ is continuous, the mappings $ u \mapsto \Delta^v u $ of $ A[[X]] $ into itself are again continuous.

As in the case of polynomials (IV, p. 7) we can prove the formulae

$$
\Delta^\sigma(uv) = \sum_{v+\rho=\sigma} \Delta^v(u) \Delta^\rho(v) ,
$$
$$
\Delta^\rho \Delta^\sigma u = \frac{(\rho + \sigma)!}{\rho! \; \sigma!} \Delta^{\rho + \sigma} u .
$$

The binomial formula (I, p. 99, Cor. 2) gives the following value for $ \Delta^v u $ when $ u = \sum_\lambda \alpha_\lambda X^\lambda $

$$
\Delta^v u = \sum_\lambda \alpha_{\lambda + v} \frac{(\lambda + v)!}{\lambda! \; v!} X^\lambda .
$$

Consider in particular the case $ v = \epsilon_i $, that is $ v_i = 1, v_j = 0 $ for $ j \neq i $. We shall put $ D_i u = \Delta^{\epsilon_i} u $; put differently, $ D_i u $ is the coefficient of $ Y_i $ in $ u(X + Y) $. By (10) we thus have

$$
D_i u = \sum_\lambda (\lambda_i + 1) \alpha_{\lambda + \epsilon_i} X^\lambda ;
$$

in particular we have $ D_i(X_i) = 1 $ and $ D_i(X_j) = 0 $ for $ j \neq i $. The formula (8) shows that $ D_i $ is a derivation of $ A[[X]] $, and from (9) we deduce the relation

$$
D^v u = v! \; \Delta^v u
$$

as in the case of polynomials (IV, p. 8) (we have put $ D^\nu = \prod_{i \in I} D_i^{\nu_i} $ for $ \nu = (\nu_i)_{i \in I} $, in $ \mathbf{N}^{(I)} $). When A is a Q-algebra, the formulae (6), (7) and (12) imply the « Taylor formulae »:

$$
u(\mathbf{X} + \mathbf{Y}) = \sum \frac{1}{\nu!} D^\nu u(\mathbf{X}) \cdot \mathbf{Y}^\nu,
$$
$$
u(\mathbf{X}) = \sum \frac{1}{\nu!} D^\nu u(0) \cdot \mathbf{X}^\nu.
$$

*Remarks. — 1) We often say that $ D_i u $ is *the partial derivative of u with respect to X*, ; we also use the notation $ D_{x_i} u, \frac{\partial u}{\partial x_i} $ and $ u'_{x_i} $. For a single indeterminate X the unique partial derivative $ Du $ (also written $ \frac{du}{dX} $ or $ u' $) is called the *derivative* of $ u $.

2) The formula (9) shows that the endomorphisms $ A^p $ of the A-module $ A[[X]] $ commute painvise. Hence the same holds of the endomorphisms $ D_i $.

3) If $ u \in A[(X_i)_{i \in I}] $ is a polynomial, the polynomials $ A^p u $ and $ D_i u $ defined in IV, p. 6 and 7 coincide with the formal power series denoted by the same symbols.

### 6. Derivations in the algebra of formal power series

Let I be a set, E an associative, commutative and unital linearly topologized, separated and complete A-algebra, and $ x = (x_i)_{i \in I} $ a family of elements of E satisfying conditions a) and b) of Prop. 4 (IV, p. 28). Let $ \varphi $ be the continuous homomorphism $ u \mapsto u(x) $ of $ A[[I]] $ into E ; it equips E with an $ A[[I]] $-module structure. By III, p. 552, an A-derivation D of $ A[[I]] $ into the $ A[[I]] $-module E is thus an A-linear mapping $ D : A[[I]] \to E $ satisfying the relation
$$
D(uv) = u(x) \cdot D(v) + D(u) \cdot v(x)
$$
for $ u, v $ in $ A[[I]] $.

#### Proposition 7 {#alg-iv-s4-prop-7 .statement}

— Let $ (y_i)_{i \in I} $, be a family of elements of E. When I is infinite, *we* assume that $ y_i $ tends to 0 along the filter of complements of finite subsets of I. There exists then a unique continuous A-derivation D of $ A[[I]] $ into the $ A[[I]] $*-module* E such that $ D(X_i) = y_i $ for all $ i \in I $. We have
$$
D(u) = \sum_{i \in I} (D_i u)(x) \cdot y_i \quad (u \in A[[I]]) .
$$

Since 0 admits in E a fundamental system of neighbourhoods consisting of ideals, the family $ ((D_i u)(x) \cdot y_i)_{i \in I} $ is summable in E for all $ u \in A[[I]] $ (Gen. Top., III, p. 263, Cor. 2). Formula (16) thus defines an A-linear mapping $ D : A[[I]] \to E $. We leave the reader to verify that D is a continuous derivation.

Let $ D_1 $ be a continuous A-derivation of $ A[[I]] $ into E, such that $ D_1(X_i) = y_i $ for all $ i \in I $. The kernel of the continuous derivation $ D - D_1 $ is a closed subalgebra B of $ \mathbf{A}[[\mathbf{I}]] $ containing 1 and the indeterminates $ X_i $. Since the polynomial algebra $ \mathbf{A}[(X_i)_{i \in I}] $ is dense in $ \mathbf{A}[[\mathbf{I}]] $, we have $ B = \mathbf{A}[[\mathbf{I}]] $ and so $ D_1 = D $.

#### Corollary 1 {#alg-iv-s4-prop-7-cor-1 .statement}

— *Let A be a continuous derivation of the A-algebra E. For every formal power series $ u \in \mathbf{A}[[\mathbf{I}]] $ the family $ ((D_iu)(x) \cdot \Delta x_i)_{i \in I} $ is summable and we have*

$$
\Delta(u(x)) = \sum_{i \in I} (D_iu)(x) \cdot \Delta x_i .
$$

This follows from Prop. 7 because the mapping $ u \mapsto \Delta(u(x)) $ is a continuous derivation of $ \mathbf{A}[[\mathbf{I}]] $ into the $ \mathbf{A}[[\mathbf{I}]] $-module E.

#### Corollary 2 {#alg-iv-s4-prop-7-cor-2 .statement}

— *The derivation $ D_i $ is the unique continuous derivation of the A-algebra $ \mathbf{A}[[\mathbf{I}]] $ such that*

$$
D_i(X_i) = 1 , \quad D_i(X_j) = 0 \quad \text{for} \quad j \neq i .
$$

This follows from Cor. 1.

#### Corollary 3 {#alg-iv-s4-prop-7-cor-3 .statement}

— *Let $ f \in \mathbf{A}[[X_1, ..., X_s]] $ and $ g_i \in \mathbf{A}[[Y_1, ..., Y_q]] $ for $ 1 \leq i \leq p $. Suppose that for $ 1 \leq i \leq p $ the constant term of $ g_i $ is zero, and put $ h = f(g_1, ..., g_p) $. Then for $ 1 \leq j \leq q $ we have*

$$
\frac{\partial h}{\partial Y_j} = \sum_{i=1}^p D_i f(g_1, ..., g_p) \cdot \frac{\partial g_i}{\partial Y_j} .
$$

This is the special case $ E = \mathbf{A}[[Y_1, ..., Y_s]] $, $ x_i = q_i $ and $ A = \partial / \partial Y_j $ of Cor. 1.

#### Proposition 8 {#alg-iv-s4-prop-8 .statement}

— *Let $ X = (X_i)_i $, be a finite family of indeterminates.
(i) Every derivation of the ring of formal power series $ \mathbf{A}[[X]] $ is continuous.
(ii) Every derivation of the polynomial ring $ \mathbf{A}[X] $ into the ring of formal power series $ \mathbf{A}[[X]] $ extends in a unique fashion to a derivation of the ring $ \mathbf{A}[[X]] $.
(iii) The family $ (D_i)_{i \in I} $ is a basis of the $ \mathbf{A}[[X]] $-module of A-derivations of $ \mathbf{A}[[X]] $ into itself.
Let $ b_n $ be the set of all formal power series of order $ \geq n $. It is clear that $ b_n $ is an ideal in the ring $ \mathbf{A}[[X]] $, generated by the monomials of degree $ n $. Hence $ b_n $ consists of finite sums of products of $ n $ formal power series without constant terms; if $ D $ is a derivation of $ \mathbf{A}[[X]] $, we have*

$$
D(f_1 \cdots f_n) = \sum_{i=1}^n f_1 \cdots f_{i-1} D(f_i) f_{i+1} \cdots f_n ,
$$

whence it follows at once that $ Db_n \subset b_{n-1} $ for $ n \geq 1 $. Since the sequence $ (b_n)_{n \geq 0} $ is a fundamental system of neighbourhoods of 0 in $ \mathbf{A}[[X]] $ (IV, p. 26 remark), D is continuous and (i) is proved.

Let $ A $ be a derivation of $ A[X] $ into $ A[[X]] $. Arguing as before, we can show that $ A(h) $ belongs to $ b, -_1 $, for every homogeneous polynomial $ h $ of degree $ n \geq 1 $. Now let $ u \in A[[X]] $ and let $ u_n $ be the homogeneous component of degree $ n $ of $ u $. Since $ A(u_n) \in b, -_1 $ for $ n \geq 1 $, the family $ (A(u)), \ldots $, is summable in $ A[[X]] $ and we can define a derivation $ D $ of $ A[[X]] $ into itself by

$$
D(u) = \sum_{n \geq 0} \Delta(u_n)
$$

We have $ D(b,) \subset b, -_1 $, hence $ D $ is a continuous endomorphism of the additive group of $ A[[X]] $. The mapping $ \Phi : (u, v) \mapsto D(uv) - uD(v) - D(u)v $ of $ A[[X]] \times A[[X]] $ into $ A[[X]] $ is continuous and zero on $ A[X] \times A[X] $. Since $ A[X] $ is dense in $ A[[X]] $, we have $ \Phi = 0 $; in other words, $ D $ is a derivation of $ A[[X]] $ into itself, extending $ A $.

Finally, $ A[X] $ is dense in $ A[[X]] $ and every derivation of $ A[[X]] $ is continuous by (i); hence there exists a unique extension of $ A $ to a derivation of $ A[[X]] $. This proves (ii).

It remains to prove (iii). Formula (18) (IV, p. 33) shows that the family $ (D_i)_{i \in I} $ is linearly independent over $ A[[X]] $, and formula (16) (IV, p. 32), applied in the case $ E = A[[X]] $, shows that every $ A $-derivation is a linear combination of the $ D_i $ with coefficients in $ A[[X]] $.

#### Proposition 9 {#alg-iv-s4-prop-9 .statement}

— Let $ (u,) \ldots $ be a *summable* family of elements of $ A[[I]] $ without constant term and $ D $ a continuous derivation of the $ A $-algebra $ A[[I]] $. If $ f = \prod_{\lambda \in L} (1 + u_\lambda) $ (IV, p. 27, Prop. 2), then the family $ (Du_\lambda/(1 + u_\lambda))_{\lambda \in L} $ is summable and we have

$$
D(f)/f = \sum_{\lambda \in L} D(u_\lambda)/(1 + u_\lambda) .
$$

If $ g $ and $ h $ are two invertible elements of $ A[[I]] $, then

$$
D(gh) = h \cdot Dg + g \cdot Dh
$$

whence on division by $ gh $,

$$
D(gh)/gh = D(g)/g + D(h)/h .
$$

For every finite subset $ M $ of $ L $ put $ f_M = \prod_{\lambda \in M} (1 + u_\lambda) $. From (21) we deduce by induction on Card $ M $ the relation

$$
D(f_M)/f_M = \sum_{\lambda \in M} D(u_\lambda)/(1 + u_\lambda)
$$

This proves Prop. 9 when L is finite. Now suppose that L is infinite and write $ \mathfrak{F} $ for the filtered ordered set of finite subsets of L. We have $ \lim_{\mathfrak{F}} f_M = f $, and hence (*IV*, p. 30 remark)

$$
D(f)/f = \lim_{\mathfrak{F}} D(f_M)/f_M .
$$

Now Prop. 9 follows by passage to the limit in (22).

### 7. The solution of equations in a formal power series ring

#### Lemma 2 {#alg-iv-s4-lem-2 .statement}

*Let* $(g_i)_i$ *be a family of elements of order* $ \geq 2 $ *in* $ \mathbf{A}[[\mathbf{I}]] $. *When* $ \mathbf{I} $ *is infinite, assume that* $ g_i $ *tends to 0 along the filter of complements of finite subsets of* $ \mathbf{I} $. *There exists one and only one automorphism* T *of the topological* A*-algebra* $ \mathbf{A}[[\mathbf{I}]] $ *such that* $ T(X_i) = X_i + g_i $ *for all* $ i \in \mathbf{I} $. *Further,

(23)
$$
\omega(T(u) - u) \geq \omega(u) + 1
$$
*for each* $ u \in \mathbf{A}[[\mathbf{I}]] $.

The series $ f_i = X_i + g_i $ has no constant term and when $ \mathbf{I} $ is infinite, $ f_i $ tends to 0 along the filter of complements of finite subsets of $ \mathbf{I} $. Therefore (IV, p. 28, Prop. 4) there exists precisely one continuous endomorphism T of the A-algebra $ \mathbf{A}[[\mathbf{I}]] $ such that $ T(X_i) = f_i $ for all $ i \in \mathbf{I} $. For each $ \nu \in \mathbf{N}' $ we put

$$
v_\nu = T(X^\nu) - X^\nu = \prod_{i \in \mathbf{I}} (X_i + g_i)^{\nu(i)} - \prod_{i \in \mathbf{I}} X_i^{\nu(i)} ;
$$

the relations $ \omega(g_i) \geq 2 $ imply $ w(v_\nu) \geq |\nu| + 1 $, and the relation (23) follows at once from this.

Let us show that $ T $ is *injective*. Given $ u \in \mathbf{A}[[\mathbf{I}]] $ such that $ T(u) = 0 $, by (23) we have $ w(u) \geq w(u) + 1 $, which is impossible if $ u \neq 0 $ because $ w(u) $ would then be a positive integer.

For every formal series $ v $ in $ \mathbf{A}[[\mathbf{I}]] $ we denote by $ H_n(v) $ its homogeneous component of degree $ n $. Let us put $ S_0(v) = H_0(v) $ and define the continuous mappings $ S, : \mathbf{A}[[\mathbf{I}]] \to \mathbf{A}[[\mathbf{I}]] $ by the recursion equations

(24)
$$
S_n(v) = H_n \left( v - T \left( \sum_{k=0}^{n-1} S_k(v) \right) \right) \quad \text{for} \quad n \geq 1
$$

Put $ S(v) = \sum_{n \geq 0} S_n(v) $; if $ \nu \in \mathbf{N}^{(\mathbf{I})} $ and $ n = |\nu| $, then the coefficient $ S^\nu(v) $ of $ X^\nu $ in $ S(v) $ is equal to that of $ X^\nu $ in $ S,(\nu) $; since $ S, $ is a continuous mapping, the mapping $ S^\nu : \mathbf{A}[[\mathbf{I}]] \to \mathbf{A} $ is continuous. Hence, by the definition of the product topology on $ \mathbf{A}[[\mathbf{I}]] = \mathbf{A}^{\mathbf{N}^{(\mathbf{I})}} $, the mapping $ S : \mathbf{A}[[\mathbf{I}]] \to \mathbf{A}[[\mathbf{I}]] $ is continuous.

We shall prove the relation $ T(S(v)) = v $ for all $ v \in \mathbf{A}[[\mathbf{I}]] $ which will complete the proof of the lemma. Let $ v \in \mathbf{A}[[\mathbf{I}]] $, $ u_n = S_n(v) $ and $ u = S(v) $. Let $ n $ be a positive integer such that

(25)$_n$
$$
\omega(v - T(u)) \geq n .
$$

We have $ w(u - (u_0 + \ldots + u_{n-1})) \geq n $, whence

$$
\omega(T(u) - T(u_0 + \ldots + u_{n-1}) - u_n) \geq n + 1
$$

by (23). Now the recursion equation (24) shows that

$$
u_n = H_n(v - T(u_0 + \cdots + u_{n-1}))
$$

By (26) the formal power series $ v - T(u) $ and $ v - T(u_0 + \ldots + u_{n-1}) - u_n $ have the same homogeneous component of degree $ n $, and this component is zero, by (27). We thus have $ w(v - T(u)) \geq n + 1 $, that is $ (25)_n $ implies $ (25)_{n+1} $. Since $ (25)_0 $ clearly holds, we thus have $ \omega(v - T(u)) \geq n $ for every integer $ n \geq 0 $, whence $ v = T(u) = T(S(v)) $, as was to be proved.

For the rest of this No. we shall, for any set $ I $, denote by $ A\{I\} $ the set of families $ (f_i)_{i \in I} $ satisfying the following conditions:
(i) for each $ i \in I $, $ f_i $ is an element of $ A[[I]] $ without constant term;
(ii) if $ I $ is infinite, $ f_i $ tends to 0 along the filter of complements of finite subsets of $ I $.

The set $ A\{I\} $ is a monoid for the composition law $ (f, g) \mapsto f \circ g $, with $ \{X_i\}_{i \in I} $ as unit element. The set of invertible elements of $ A\{I\} $ is thus a group.

On the other hand, let $ E $ be the monoid of all continuous unital endomorphisms of the $ A $-algebra $ A[[I]] $ leaving the ideal of all formal power series without constant term invariant. If $ f \in A\{I\} $ and $ g \in A[[I]] $, then the element $ g(f) $ is defined. For fixed $ f $, the mapping $ g \mapsto g(f) $ of $ A[[I]] $ into itself is an element $ W_f $ of $ E $. If $ f_1, f_2 \in A\{I\} $ and $ g \in A[[I]] $, we have, by formula (5) (IV, p. 30)

$$
W_{f_1 \circ f_2}(g) = g(f_1 \circ f_2) = g(f_1) \circ f_2 = W_{f_2}(W_{f_1}(g))
$$

hence $ f \mapsto W_f $ is a homomorphism of the monoid opposite to $ A\{I\} $ into $ E $. By Prop. 4 (IV, p. 28) this homomorphism is bijective.

Let $ f = (f_i)_{i \in I} \in A\{I\} $ and let $ \sum_{j \in I} \alpha_{ij} X_j $ be the homogeneous component of degree 1 of $ f_i $. For any fixed $ j $ in $ I $ we have $ \alpha_{ij} = 0 $ except for a finite number of suffixes $ i $, by hypothesis (ii) above. If $ (\lambda_i) \in A^{(I)} $, we thus have $ \left( \sum_{j \in I} \alpha_{ij} \lambda_j \right) \in A^{(I)} $.

We denote by $ T_f $ the $ A $-linear mapping $ ^1 $

$$
(\lambda_i) \mapsto \left( \sum_{j \in I} \alpha_{ij} \lambda_j \right)
$$

of $ A^{(I)} $ into $ A^{(I)} $. If $ g \in A\{I\} $, it is easily verified that

$$
T_{f \circ g} = T_f \circ T_g .
$$

$ ^1 $ Sometimes $ T_f $ is called the linear mapping tangent to $ f $.

#### Proposition 10 {#alg-iv-s4-prop-10 .statement}

— Let $ f \in A\{I\} $; then the following conditions are equivalent :
(i) $ f $ is invertible in $ A\{I\} $ for the law $ \circ $;
(ii) $ T_f $ is invertible in the ring $ \mathrm{End}(A^{(I)}) $.

The implication (i) $ \Rightarrow $ (ii) is immediate from (28). Suppose now that $ T_f $ is invertible in $ \mathrm{End}(A^{(I)}) $. There exists $ g = (g_i)_i \in A\{I\} $ such that each $ g_i $ is homogeneous of degree $ l $ and $ T_g \circ T_f $ is the identity mapping of $ A^{(I)} $. Write $ h = g \circ f $; then (28) shows that $ T_h $ is the identity mapping of $ A^{(I)} $, which is equivalent to the assertion $ \omega(h_i - X_i) \geq 2 $. By Lemma 2 of IV, p. 35 $ h $ is therefore invertible in $ A\{I\} $. It is clear that $ g $ is invertible in $ A\{I\} $, hence $ f $ is invertible in $ A\{I\} $.

#### Corollary {#alg-iv-s4-n7-cor-1 .statement}

— Let $ f_i(Y_1, Y_2, \ldots, Y_q, X_1, X_2, \ldots, X_p) $ ($ 1 \leq i \leq q $) be $ q $ formal power series without constant term in $ A[[Y_1, \ldots, Y_q, X_1, \ldots, X_p]] $. If the constant term of the formal power series $ D = \det \left( \frac{\partial f_i}{\partial Y_j} \right) $ is invertible in $ A $, then there exists precisely one system of $ q $ formal power series $ u_1(X_1, \ldots, X_p), \ldots, u_q(X_1, \ldots, X_p) $ such that
$$
f_i(u_1, \ldots, u_q, X_1, \ldots, X_p) = 0 \quad (1 \leq i \leq q).
$$
Put $ f_{q+1} = X_1, \ldots, f_{q+p} = X_p $, $ f = (f_1, \ldots, f_{p+q}) $, then $ \det T_f $ is equal to the constant term of $ D $, hence invertible in $ A $; therefore $ T_f $ is invertible. By Prop. 10 there exist formal power series without constant term
$$
g_1, \ldots, g_{q+p} \in A[[Y_1, \ldots, Y_q, X_1, \ldots, X_p]]
$$
such that on writing
$$
g = (g_1, \ldots, g_{p+q}), \quad 1_{p+q} = (Y_1, \ldots, Y_q, X_1, \ldots, X_p)
$$
we have $ f \circ g = g \circ f = 1_{p+q} $. The relation $ f \circ g = 1_{p+q} $, in particular gives
$$
g_{q+1} = X_1, \ldots, g_{q+p} = X_p.
$$
Hence
$$
f_i(g_1, \ldots, g_q, X_1, \ldots, X_p) = Y_i \quad (1 \leq i \leq q).
$$
Now put
$$
u_i(X_1, \ldots, X_p) = g_i(0, \ldots, 0, X_1, \ldots, X_p) \quad (1 \leq i \leq q);
$$
substituting 0 for each $ Y_i $ in (30) we obtain the desired relation (29).

Conversely, suppose that the formal power series $ u_1, \ldots, u_q $ in the ring $ A[[X_1, \ldots, X_p]] $ satisfy the relation (29). The relation $ g \circ f = 1_{p+q} $ implies
$$
g_i(f_1, \ldots, f_q, X_1, \ldots, X_p) = Y_i \quad (1 \leq i \leq q);
$$
and substituting $ u_i $ for $ Y_i $ for $ 1 \leq i \leq q $ in (32), we obtain (31), whence the uniqueness of the solution of the system (29).

### 8. Formal power series over an integral domain

#### Proposition 11 {#alg-iv-s4-prop-11 .statement}

— Suppose that $ A $ is an integral domain.

(i) *The ring* $ A[[I]] $ *is again an integral domain*.

(ii) *If* $ u, v $ *are non-zero elements of* $ A[[I]] $, *then* $ \omega(uv) = \omega(u) + \omega(v) $.

For each $ J \subset I $ let $ \varphi_J $ be the homomorphism of $ A[[I]] $ into $ A[[J]] $ obtained by substituting in each element of $ A[[I]] $, $ X_i $ for $ X_i $ when $ i \in J $ and 0 for $ X_i $ when $ i \in I - J $. Let $ u, v $ be non-zero elements of $ A[[I]] $, $ p = \omega(u) $, $ q = \omega(v) $; there exists a finite subset $ J $ of $ I $ such that

$$
\varphi_J(u) \neq 0,\ \varphi_J(v) \neq 0,\ \omega(\varphi_J(u)) = p,\ \omega(\varphi_J(v)) = q.
$$

Let a (resp. b) be the homogeneous component of degree $ p $ (resp. $ q $) of $ \varphi_J(u) $ (resp. $ \varphi_J(v) $). Since $ J $ is finite, a and b are polynomials. We have $ a \neq 0, b \neq 0 $, hence $ ab \neq 0 $ (IV, p. 9, Prop. 8). Hence $ \varphi_J(u)\ \varphi_J(v) $ is non-zero, of order $ p + q $. It follows that $ uv \neq 0 $ and $ \omega(uv) \leq p + q $; but clearly $ \omega(uv) \geq p - q $.

### 9. The field of fractions of the ring of formal power series in one indeterminate over a field

If K is a commutative field, we shall denote by $ K((X)) $ the field of fractions of the integral domain $ K[[X]] $.

#### Proposition 12 {#alg-iv-s4-prop-12 .statement}

— *Every non-zero element* $ u $ *of* $ K((X)) $ *may be written in a unique way as* $ u = X^k v $, *where* $ k \in \mathbf{Z} $ *and* $ v $ *is a formal power series in* $ X $ *of order* 0.

Let $ u = w/t $, where $ w, t $ are non-zero elements of $ K[[X]] $. We have $ w = X^r w_1, t = X^s t_1 $, where $ r, s \in \mathbf{N} $ and $ w_1, t_1 $ are formal power series of order 0, hence invertible in $ K[[X]] $ (IV, p. 30, Prop. 6). Then $ u = X^{r-s} w_1 t_1^{-1} $ and $ w_1 t_1^{-1} $ is a formal power series of order 0.

Let us prove the uniqueness. Suppose that $ u = X^{k_1} v_1 = X^{k_2} v_2 $ where $ k_1, k_2 \in \mathbf{Z} $ and $ v_1, v_2 $ are formal power series of order 0. Since $ X^{k_1 - k_2} = v_2 v_1^{-1} $ is a formal power series of order 0, we have $ k_1 = k_2 $ whence $ v_1 = v_2 $ and this proves the uniqueness assertion.

We shall say that the elements of $ K((X)) $ are *generalized formal power series* in $ X $ with coefficients in $ K $, or simply formal power series when no confusion can arise (the elements of $ K[[X]] $ are then called *formal power series with positive exponents*); if $ u \neq 0 $, the integer $ k $ defined in Prop. 12 is also called the *order* of $ u $ and is written $ \omega(u) $, even if it is $ < 0 $; we also put $ \omega(0) = \infty $. It may be verified at once that

$$
\begin{align*}
\omega(u + v) &\geq \inf(\omega(u), \omega(v)) \\
\omega(u + v) &= \inf(\omega(u), \omega(v)) \quad \text{if}\ \ \omega(u) \neq \omega(v) \\
\omega(uv) &= \omega(u) + \omega(v)
\end{align*}
$$

still hold for generalized formal power series. In particular, if $ u \neq 0 $, then $ w(u^{-1}) = -w(u) $. \* In other words (Comm. Alg., VI, § 3, No. 6, p. 392, Def. 3), w is a normalized discrete valuation of the field $ K((X)) $. \*

For each integer $ n \in \mathbf{Z} $ let $ p_n $ be the set of all $ u \in K((X)) $ such that $ \omega(u) \geq n $. Then (p.), , , is a decreasing sequence of subgroups of the additive group $ K((X)) $, with intersection 0 ; there exists thus a topology on $ K((X)) $, invariant under translation, for which $ (p_n)_{n \in \mathbf{Z}} $ is a fundamental system of neighbourhoods of 0 (Gen. Top., III, p. 223). We can easily verify that $ K((X)) $ is a topological field (Gen. Top., III, p. 281) and that $ K[[X]] $ is an open and closed subspace of $ K((X)) $.

Let (a,, , be a family of elements of $ K $, and suppose that there exists an integer N such that $ a_n = 0 $ for all $ n < N $. Then the family' $ (\alpha_n X^n)_{n \in \mathbf{Z}} $ is summable in $ K((X)) $ (Gen. Top., III, p. 263, Cor.) ; put $ u = \sum_{n \in \mathbf{Z}} \alpha_n X^n $, then $ u = 0 $ if and only if $ a_n = 0 $ for all $ n $; otherwise the order of $ u $ is the least integer k such that $ \alpha_k \neq 0 $. Finally every element of $ K((X)) $ may be written in a unique fashion in the form $ \sum_{n \in \mathbf{Z}} \alpha_n X^n $, where the sequence (a,) satisfies $ \alpha_{-n} = 0 $ for all sufficiently large n.

Since the ring $ K[X] $ is a subring of $ K[[X]] $, every rational fraction $ u/v \in K(X) $ (u, v being polynomials in X) may be identified with the (generalized) formal power series $ uv^{-1} $ of $ K((X)) $, which we shall call its expansion at the origin ; the field $ K(X) $ is thus identified with a subfield of $ K((X)) $.

### 10. Exponential and logarithm

By the exponential power series we shall understand the element $ \sum_{n \geq 0} \frac{X^n}{n!} $ of $ Q[[X]] $; it will be denoted by exp X or $ e^X $.

#### Proposition 13 {#alg-iv-s4-prop-13 .statement}

— In $ Q[[X, Y]] $ we have $ e^{X+Y} = e^X e^Y $.

For the binomial formula gives

$$
\frac{(X+Y)^n}{n!} = \sum_{i+j=n} \frac{X^i}{i!} \frac{Y^j}{j!}
$$

Hence

$$
e^X e^Y = \left( \sum_{i \geq 0} \frac{X^i}{i!} \right) \left( \sum_{j \geq 0} \frac{Y^j}{j!} \right) = \sum_{i,j \geq 0} \frac{X^i}{i!} \frac{Y^j}{j!} = \sum_{n \geq 0} \sum_{i+j=n} \frac{X^i}{i!} \frac{Y^j}{j!}
$$
$$
= \sum_{n \geq 0} \frac{(X+Y)^n}{n!} = e^{X+Y}.
$$

We shall define two elements $ e(X) $, I(X) of $ Q[[X]] $ by

$$
e(X) = e^X - 1 = \sum_{n \geq 1} \frac{X^n}{n!}
$$

(34)
$$
l(X) = \sum_{n \geq 1} (-1)^{n-1} \frac{X^n}{n}.
$$

We have
(35)
$$
e(X+Y) = e(X) + e(Y) + e(X)e(Y)
$$
(36)
$$
D(e^X) = D(e(X)) = e^X
$$
(37)
$$
D(l(X)) = \sum_{n \geq 0} (-X)^n = (1+X)^{-1}.
$$

#### Proposition 14 {#alg-iv-s4-prop-14 .statement}

— We have $ l(e(X)) = e(l(X)) = X $.

The series l and e have no constant term and their terms of degree 1 are equal to X. By Prop. 10 of IV, p. 37 it suffices to prove the formula $ l(e(X)) = X $. By the formulae (36) and (37) and Cor. 3 of IV, p. 33 we have

$$
D(l(e(X))) = (1 + e(X))^{-1} D(e(X)) = (e^X)^{-1} e^X = 1
$$

whence $ I(e(X)) = X $.

Let K be a Q-algebra, then the elements of K[[I]] without constant term form a commutative group $ \mathcal{E} $ under addition. The elements of K[[I]] with constant term 1 form a commutative group $ \mathbf{A} $ under multiplication (IV, p. 30). For each $ f \in \mathcal{E} $, we can define the elements $ e \circ f $ and $ I \circ f $ of $ \mathcal{E} $, and by Prop. 14 above, the mappings $ f \mapsto l \circ f $ and $ f \mapsto e \circ f $ are mutually inverse permutations of $ \mathcal{E} $; clearly they are continuous. Since $ \exp X = e(X) + 1 $, we see that the exponential mapping $ f \mapsto \exp f = e \circ f + 1 $ is a continuous bijection of $ \mathcal{E} $ onto $ \mathcal{M} $. By formula (4) of IV, p. 29 and Prop. 13, we have $ \exp(f+g) = (\exp f)(\exp g) $ for $ f, g \in \mathcal{E} $. Thus the exponential is an isomorphism of the topological group $ \mathcal{E} $ onto the topological group $ \mathbf{A} $.

The inverse isomorphism of $ \mathcal{M} $ onto $ \mathcal{E} $ is called the logarithm and is written $ g \mapsto \log g $. We thus have $ \log g = l(g-1) $ for $ g $ in $ \mathcal{M} $, and in particular,

(38)
$$
\log(1+X) = l(X).
$$

Since the logarithm is a homomorphism of $ \mathcal{M} $ into $ \mathcal{E} $, the formula $ (1+X)(1+Y) = 1 + (X+Y+XY) $ implies

(39)
$$
l(X) + l(Y) = l(X+Y+XY).
$$

Let $ (u,)_{\lambda} $ be a summable family of elements of $ \mathcal{B} $, then the family $ (\exp u_{\lambda})_{\lambda \in L} $ is multipliable and we have

(40)
$$
\exp \left( \sum_{\lambda \in L} u_{\lambda} \right) = \prod_{\lambda \in L} \exp u_{\lambda}.
$$

Similarly, if $ (f_\lambda)_{\lambda \in L} $ is a multipliable family of elements of A, the family $ (\log f_\lambda)_{\lambda \in L} $ is summable and we have

(41)
$$
\log \left( \prod_{\lambda \in L} f_\lambda \right) = \sum_{\lambda \in L} \log f_\lambda .
$$

Let $ g \in A $, and let D be a continuous derivation of $ K[[I]] $. We have $ \log g = l(g - 1) $, hence by Cor. 3 of IV, p. 33 and (37) we have

(42)
$$
D \log g = D(g)/g .
$$

The expression $ D(g)/g $ is called the logarithmic derivative of g (relative to D).

### Exercises {#alg-iv-s4-exercises}

See the [exercises for § 4](exercises/s4/).
