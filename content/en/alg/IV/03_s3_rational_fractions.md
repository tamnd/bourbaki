---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 3
section_title: Rational fractions
lang: en
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.19-A IV.24, A IV.89-A IV.90
pdf_pages: 0028-0033, 0098-0099
extraction: ocr
subsections:
    - "no": 1
      title: Definition of rational fractions
      page: 19
      pdf_page: 28
    - "no": 2
      title: Degrees
      page: 20
      pdf_page: 29
    - "no": 3
      title: Substitutions
      page: 21
      pdf_page: 30
    - "no": 4
      title: Differentials and derivations
      page: 23
      pdf_page: 32
statements: 6
exercises: 7
content_sha256: 1454c218e59fd22dd66a7d3b73222098aac8674c609849f8e3e5a2017a4c893e
---

## § 3. RATIONAL FRACTIONS

### 1. Definition of rational fractions

#### Definition 1 {#alg-iv-s3-def-1 .statement}

*Let K be a commutative field and I a set. The field of fractions (I, p. 116) of the integral domain $ K[(X_i)_{i \in I}] $ is denoted by $ K((X_i)_{i \in I}) $ or $ K(X_i)_{i \in I} $. Its elements are called rational fractions in the indeterminates $ X_i $ with coefficients in K.*

For $ I = \{1, 2, \ldots, n\} $ we write $ K(X_1, X_2, \ldots, X_n) $ in place of $ K((X_i)_{i \in I}) $.

Let A be an integral domain and K its field of fractions. The ring $ A[(X_i)_{i \in I}] $ may be identified with a subring of $ K[(X_i)_{i \in I}] $, hence also of $ K((X_i)_{i \in I}) $. For each $ f \in K[(X_i)_{i \in I}] $ there exists a non-zero element $ \alpha $ of A such that $ \alpha f \in A[(X_i)_{i \in I}] $. Hence every element of $ K((X_i)_{i \in I}) $ can be written as $ u/v $ where $ u, v \in A[(X_i)_{i \in I}], v \neq 0 $. Thus $ K((X_i)_{i \in I}) $ may be identified with the field of fractions of $ A[(X_i)_{i \in I}] $.

Now let K be a commutative field, I a set and J ⊂ I. Put B = K[(X_i)_{i ∈ J}], then K[(X_i)_{i ∈ I}] = B[(X_i)_{i ∈ I - J}], and by what has been said, K((X_i)_{i ∈ I}) may be identified with K'((X_i)_{i ∈ I - J}), where K' = K((X_i)_{i ∈ J}).

### 2. Degrees

Let K be a commutative field. For every element r of K((X_i)_{i ∈ I}) there exist u, v ∈ K[(X_i)_{i ∈ I}] such that v ≠ 0 and r = $ \frac{u}{v} $. The relation $ \frac{u}{v} = \frac{u_1}{v_1} $, where v ≠ 0, v_1 ≠ 0 is equivalent to uv_1 = vu_1; if r ≠ 0, we have u ≠ 0 and u_1 ≠ 0, and so deg u + deg v_1 = deg v + deg u_1 (IV, p. 9), or also deg u − deg v = deg u_1 − deg v_1. The rational integer deg u − deg v thus depends only on r; we call it the degree, or the total degree of r, and denote it by deg r. We shall agree to write deg 0 = −∞. If J ⊂ I, we can likewise define the degree with respect to the X_j of index j ∈ J. When r is a polynomial, these notions coincide with those defined in IV, p. 2.

#### Proposition 1 {#alg-iv-s3-prop-1 .statement}

— Let r, s be two rational fractions.

(i) If deg r ≠ deg s, we have

$$
r + s \neq 0 \quad \text{and} \quad \deg(r + s) = \sup(\deg r, \deg s)
$$

If deg r = deg s, we have deg(r + s) ≤ deg r.

(ii) We have deg(rs) = deg r + deg s.

We can limit ourselves to the case where r and s are non-zero.

Let us write r = $ \frac{u}{v} $, s = $ \frac{w}{z} $, where u, v, w, z are non-zero polynomials. We have rs = $ \frac{uw}{vz} $, and so

$$
\deg(rs) = \deg(uw) - \deg(vz) = \deg u - \deg v + \deg w - \deg z =
= \deg r + \deg s.
$$

On the other hand, we have r + s = $ \frac{uz + vw}{vz} $. Suppose that deg r ≠ deg s, in other words deg u + deg z ≠ deg w + deg v. Then uz + vw ≠ 0, and

$$
\begin{align*}
\deg(r + s) &= \deg(uz + vw) - \deg(vz) \\
&= \sup(\deg(uz), \deg(vw)) - \deg(vz) \\
&= \sup(\deg(uz) - \deg(vz), \deg(wv) - \deg(vz)) \\
&= \sup(\deg r, \deg s).
\end{align*}
$$

Suppose that deg r = deg s, that is deg u + deg z = deg w + deg v. If r + s ≠ 0, then we have

$$
\begin{align*}
\deg(r + s) &= \deg(uz + vw) - \deg(vz) \\
&\leq \deg(uz) - \deg(vz) = \deg r
\end{align*}
$$

\* The mapping r ↦ −deg r is thus a discrete valuation on the field K((X_i)_{i ∈ I}). \*

### 3. Substitutions

Let K be a commutative field, E a unital associative K-algebra, $ x = (x_i)_{i \in I} $ a family of pairwise permutable elements of E. Let $ B = K[(X_i)_{i \in I}] $ and $ S_x $ the set of all non-zero $ v \in B $ such that $ v(x) $ is invertible in E. Let $ u \in B,\ v \in S_x $ and $ f = \frac{u}{v} \in K((X_i)_{i \in I}) $. The element $ u(x)\ v(x)^{-1} = v(x)^{-1}u(x) $ is defined in E; moreover, if $ u_1,\ v_1 $ are two polynomials such that $ f = \frac{u_1}{v_1} $ and $ v_1 \in S_x $, then $ uv_1 = vu_1 $, hence $ u(x)v_1(x) = v(x)u_1(x) $ and so
$$
u(x)\ v(x)^{-1} = u_1(x)\ v_1(x)^{-1}.
$$

Let $ f \in K((X_i)_{i \in I}) $. If there exists *at least one couple* $(u, v)$ such that $ f = \frac{u}{v} $ and $ v \in S_x $, we shall say that x is *substitutable* in $ f $; the element $ u(x)\ v(x)^{-1} $ which only depends on $ f $ and $ x $ is then denoted by $ f(x) $ or $ f((x_i)) $ or $ f((x_i)_{i \in I}) $.

#### Proposition 2 {#alg-iv-s3-prop-2 .statement}

*Let K be a commutative field, E a unital associative K-algebra and $ x = (x_i)_{i \in I} $ a family of pairwise permutable elements of E. The set $ S_x^{-1}B $ of $ f \in K((X_i)_{i \in I}) $ such that x is substitutable in $ f $ is a K-subalgebra of $ K((X_i)_{i \in I}) $. The mapping $ f \mapsto f(x) $ is a unital homomorphism $ \varphi $ of $ S_x^{-1}B $ into E. The image $ \varphi(S_x^{-1}B) $ is the set of all $ yz^{-1} $, where y runs over the unital subalgebra $ K[x]_E $ of E generated by the family x and where z runs over the set of all invertible elements of $ K[x]_E $.

Let $ f_1 = \frac{u_1}{v_1},\ f_2 = \frac{u_2}{v_2} $ be two elements of $ K((X_i)_{i \in I}) $ such that $ v_1,\ v_2 \in S_x $. We have $ f_1 + f_2 = \frac{u_1v_2 + u_2v_1}{v_1v_2},\ f_1f_2 = \frac{u_1u_2}{v_1v_2} $ and $ v_1,\ v_2 \in S_x $. Hence $ S_x^{-1}B $ is a K-subalgebra of $ K((X_i)_{i \in I}) $. The rest of the proposition is clear.

#### Corollary {#alg-iv-s3-n3-cor-1 .statement}

*Let L be a commutative field, K a subfield of L, $ x = (x_i)_{i \in I} $ a family of elements of L, M the set consisting of the $ x_i $, U the set of all $ f \in K((X_i)_{i \in I}) $ such that x is substitutable in $ f $ and $ \varphi $ the homomorphism $ f \mapsto f(x) $ of U into L. Then $ \varphi(U) $ is the subfield of L generated by $ KUM $.*

Let L' be the subfield of L generated by $ KUM $. We have
$$
K \cup M \subset \varphi(U) \subset L'
$$
and $ \varphi(U) $ is a subring of L. Now Prop. 2 implies that $ \varphi(U) $ is a subfield of L, whence $ \varphi(U) = L' $.

Let $ f \in K((X_i)_{i \in I}) $ and let $ (g_i)_{i \in I} $ be a family of elements of $ K((Y_l)_{l \in L}) $. If (g_i) is substitutable in f, then f((g_i)) is an element of K((Y_l)_{l \in L}). In particular, (X_i)_{i \in I} is substitutable in f and f = f((X_i)_{i \in I}).

#### Proposition 3 {#alg-iv-s3-prop-3 .statement}

— Let E be an algebra over K which is associative, commutative, unital and non-zero. Let f \in K((X_i)_{i \in I}) and for each i \in I, let g_i \in K((Y_l)_{l \in L}). Given a family y = (y_l)_{l \in L} of elements of E, suppose that y is substitutable into each g_i and (g_i(y))_{i \in I} is substitutable in f. Then:
(i) (g_i)_{i \in I} is substitutable in f;
(ii) if we denote by h the element f((g_i)) of K((Y_l)_{l \in L}), then y is substitutable in h and h(y) = f((g_i(y))).

We may take I to be finite. By hypothesis, for each i \in I, g_i can be put in the form p_i/q_i where p_i, q_i \in K[(Y_l)_{l \in L}] and q_i(y) is invertible in E. Likewise f can be written as u/v, where u, v \in K[(X_i)_{i \in I}] and v((g_i(y))) is invertible. Let m = \sup(\deg u, \deg v), and let w = \prod_{i \in I} q_i \in K[(Y_l)_{l \in L}], u_1 = u((g_i)) w^m, v_1 = v((g_i)) w^m. The polynomial u is a K-linear combination of monomials \prod_{i \in I} X_i^{v_i} such that \sum_{i \in I} v_i \leq m. We have w^m \prod_{i \in I} g_i^{v_i} = w^m \left( \prod_{i \in I} p_i^{v_i} \right) \left( \prod_{i \in I} q_i^{v_i} \right)^{-1} \in K[(Y_l)_{l \in L}] by the choice of m. Hence u_1 \in K[(Y_l)_{l \in L}] and similarly v_1 \in K[(Y_l)_{l \in L}]. Moreover, v_1(y) = (w(y))^m v((g_i(y))) is invertible. Hence v_1 \neq 0, because E \neq 0, and so v((g_i)) \neq 0. The family (g_i) is thus substitutable in f. Besides we have f((g_i)) = u_1/v_1, hence y is substitutable in h = f((g_i)), and h(y) = u_1(y)/v_1(y) = u((g_i(y)))/v((g_i(y))) = f((g_i(y))).

Let K be a commutative field, E a commutative associative and unital K-algebra, and let f \in K((X_i)_{i \in I}). Let T_f be the set of all x = (x_i)_{i \in I} \in E^I which are substitutable in f. The mapping x \mapsto f(x) of T_f into E is called the rational function associated with f (and E); we sometimes denote it by \tilde{f}. If g \in K((X_i)_{i \in I}) we have T_f \cap T_g \subset T_{f+g}, T_f \cap T_g \subset T_{fg}, hence the rational function associated with f + g (resp. fg) is defined on T_f \cap T_g and has the same value on this set as \tilde{f} + \tilde{g} (resp. \tilde{f}\tilde{g}). Let T'_f be the set of x \in T_f such that f(x) is invertible; if x \in T'_f, x is substitutable in 1/f and the rational function associated with 1/f takes at x the value f(x)^{-1}.

If K is an infinite commutative field, f \in K((X_i)_{i \in I}), g \in K((X_i)_{i \in I}) and \tilde{f}, \tilde{g} are the rational functions associated with f, g (and K), and if \tilde{f}(x) = \tilde{g}(x) for all x \in T_f \cap T_g then f = g. For if f = u/v and g = u_1/v_1, where u, v, u_1, v_1 are polynomials, we have u(x)v_1(x) = u_1(x)v(x) for all x such that v(x)v_1(x) \neq 0, hence uv_1 = u_1v (IV, p. 18, Th. 2). Therefore the mapping f \mapsto \tilde{f} is injective and we shall often identify f and \tilde{f}.

\* Using the factoriality of $ K[(X_i)_{i \in I}] $ (Comm. Alg., VII, § 3, No. 2 p. 502 and Cor. of Th. 2 p. 506), one easily shows the following: for every $ f \in K((X_i)_{i \in I}) $ there exist $ u, v \in K[(X_i)_{i \in I}] $ such that:
    1) $ f = u/v $;
    2) for $ x \in K^I $ to be substitutable in $ f $ it is necessary and sufficient that $ v(x) \neq 0. $

### 4. Differentials and derivations

Let $ K $ be a commutative field. By III, p. 558, Prop. 5, every derivation $ D $ of $ K[(X_i)_{i \in I}] $ extends in a unique fashion to a derivation $ \bar{D} $ of $ K((X_i)_{i \in I}) $. If $ D, D' $ are permutable derivations of $ K[(X_i)_{i \in I}] $, then the bracket $ [D, D'] = DD' - D'D $ is zero, hence $ [\bar{D}, \bar{D}'] $ which is a derivation of $ K((X_i)_{i \in I}) $ extending $ [D, D'] $ is zero; in other words, $ D $ and $ D' $ are permutable. In particular the derivations $ D_i $ (IV, p. 6) extend to derivations of $ K((X_i)_{i \in I}) $ again denoted by $ D_i $ and which are pairwise permutable. If $ f \in K((X_i)_{i \in I}), D_i f $ is also written $ D_{x_i} f $ or $ \frac{\partial f}{\partial x_i} $ or $ f'_{x_i} $. When there is only a single indeterminate $ X $ one uses the notation $ Df, \frac{df}{dX}, f' $.

Let $ B = K[(X_i)_{i \in I}], C = K((X_i)_{i \in I}) $. By III, p. 574, Prop. 23, the canonical mapping

$$
\Omega_K(B) \otimes_B C \to \Omega_K(C)
$$

is an isomorphism of vector $ C $-spaces. Bearing in mind III, p. 570, we see that the vector $ C $-space $ \Omega_K(C) $ admits as a basis the family $ (dX_i)_{i \in I} $ of the differentials of the $ X_i $. Let $ \partial_i $ be the coordinate form of index $ i $ on $ \Omega_K(C) $ relative to that basis. Then the mapping $ u \mapsto (\partial_i, du) $ of $ C $ into itself is a derivation of $ C $ which maps $ X_i $ to 1 and $ X_j $ to 0 for $ j \neq i $, and so is equal to $ D_i $; in other words, we have

$$
du = \sum_{i \in I} (D_i u) dX_i
$$

for every $ u \in C $. If $ I $ is finite, $ (D_i)_{i \in I} $ is a basis of the vector $ C $-space of derivations of $ C $.

#### Proposition 4 {#alg-iv-s3-prop-4 .statement}

— *Let $ E $ be an associative, commutative and unital $ K $-algebra, $ x = (x_i)_{i, I} $ a family of elements of $ E $ and $ f \in K((X_i)_{i, I}) $. Suppose that $ x $ is substitutable in $ f $ and $ y = f(x) $.
(i) For every derivation $ A $ of $ K((X_i)_{i, I}) $ which maps $ K[(X_i)_{i, I}] $ into itself, $ x $ is substitutable in $ Af $.
(ii) For every derivation $ D $ of $ E $ into an $ E $-module we have

$$
Dy = \sum_{i \in I} (D_i f)(x) \cdot Dx_i .
$$

Let $ f = \frac{u}{v} $ with $ u, v \in K[(X_i)_{i \in I}] $ and $ v(x) $ invertible in E. Let A be a derivation of $ K((X_i)_{i \in I}) $ mapping $ K[(X_i)_{i \in I}] $ into itself. We have
$$
\Delta f = \frac{(\Delta u)\ v - u(\Delta v)}{v^2}
$$
and $ v^2(x) $ is invertible, hence x is substitutable in $ Af $. Secondly put $ r = u(x) $, $ s = v(x) $; we have $ y = s^{-1}r $, hence for every derivation D of E into an E-module we have
$$
\begin{align*}
Dy &= s^{-2}(s(Dr) - r(Ds)) \\
&= s^{-2}\left( s \sum_{i \in I} (D_iu)(x) \cdot Dx_i - r \sum_{i \in I} (D_iv)(x) \cdot Dx_i \right)
\end{align*}
$$
by Prop. 4 of IV, p. 6. Thus $ Dy = \sum_{i \in I} w_i \cdot Dx_i $ with
$$
w_i = v(x)^{-2}(v(x)(D_iu)(x) - u(x)(D_iv)(x)) = (D_if)(x).
$$

### Exercises {#alg-iv-s3-exercises}

See the [exercises for § 3](exercises/s3/).
