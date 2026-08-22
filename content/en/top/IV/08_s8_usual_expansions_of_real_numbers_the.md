---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 8
section_title: Usual expansions of real numbers; the power of R
lang: en
source: top-i-iv
pdf_pages: 0379-0383, 0407-0411
extraction: ocr
subsections:
    - "no": 1
      title: APPROXIMATIONS TO A REAL NUMBER
      page: 0
      pdf_page: 379
    - "no": 2
      title: EXPANSIONS OF REAL NUMBERS RELATIVE TO A BASE SEQUENCE
      page: 0
      pdf_page: 379
    - "no": 3
      title: DEFINITION OF A REAL NUMBER BY MEANS OF ITS EXPANSION
      page: 0
      pdf_page: 380
    - "no": 4
      title: COMPARISON OF EXPANSIONS
      page: 0
      pdf_page: 382
    - "no": 5
      title: EXPANSIONS TO BASE A
      page: 0
      pdf_page: 382
    - "no": 6
      title: THE POWER OF R
      page: 0
      pdf_page: 383
statements: 2
exercises: 3
content_sha256: 914f3a44829462fc66adf76c60db064b9c5883f0d26bf2cfdd49a49ba9f8b612
---

## 8. USUAL EXPANSIONS OF REAL NUMBERS; THE POWER OF R

### 1. APPROXIMATIONS TO A REAL NUMBER

Definition 1. Given a number $ \varepsilon > 0 $, a real number $ r $ is said to be an approximation to within $ \varepsilon $ to a real number $ x $, if $ |x - r| \leq \varepsilon $; $ r $ is said to be an approximation by defect if $ r \leq x $, by excess if $ r \geq x $.

Let $ A $ be a dense subset of $ \mathbf{R} $. For each $ x \in \mathbf{R} $ and each $ \varepsilon > 0 $ there is an approximation by defect (resp. excess) to $ x $ to within $ \varepsilon $ belonging to $ A $, since the interval $ ]x - \varepsilon, x[ $ (resp. $ ]x, x + \varepsilon[ $) contains at least one point of $ A $. If we now consider a given strictly decreasing sequence $ (\varepsilon_n) $ of numbers $ > 0 $, tending to 0, and if $ r_n $ is an approximation to $ x $ to within $ \varepsilon_n $, then the sequence $ (r_n) $ has $ x $ as limit as $ n $ tends to infinity.

In the case where $ A $ is a subgroup of the additive group $ \mathbf{R} $, and we restrict the $ \varepsilon_n $ to belong to $ A $, we can define canonically for each $ x \in \mathbf{R} $ a sequence $ (r_n) $ of approximations to $ x $ by defect, belonging to $ A $.

For by Archimedes' axiom (\S 2, no. 1, Theorem 1), the set of integers $ p $ such that $ p \varepsilon_n \leq x $ has a greatest element $ p_n $; in other words, there is a unique integer $ p_n $ such that

$$
p_n \varepsilon_n \leq x < (p_n + 1) \varepsilon_n.
$$

Since $ |x - p_n \varepsilon_n| \leq \varepsilon_n $, it follows that $ p_n \varepsilon_n $ is an approximation to $ x $ to within $ \varepsilon_n $ by defect, and belongs to $ A $ by hypothesis; similarly $ (p_n + 1) \varepsilon_n $ is an approximation to $ x $ to within $ \varepsilon_n $ by excess, belonging to $ A $, and the two sequences $ (p_n \varepsilon_n) $ and $ ((p_n + 1) \varepsilon_n) $ have $ x $ as their limit.

### 2. EXPANSIONS OF REAL NUMBERS RELATIVE TO A BASE SEQUENCE

We shall limit ourselves to studying the case where $ \varepsilon_n = 1/d_n $, where $ (d_n) $ is a strictly increasing sequence of integers such that $ d_0 = 1 $ and $ d_n $ is a multiple of $ d_{n-1} $ for $ n \geq 1 $. Let $ a_n = d_n / d_{n-1} $ ($ n \geq 1 $): $ a_n $ is an integer $ > 1 $. In this case, the sequence of approximations by defect $ r_n = p_n / d_n $ is increasing, for $ p_n $ is the largest integer such that $ p_n / d_n \leq x $; but we have

$$
\frac{p_{n-1}}{d_{n-1}} = \frac{p_{n-1} a_n}{d_n} \leq x < \frac{p_{n-1} + 1}{d_{n-1}} = \frac{p_{n-1} a_n + a_n}{d_n}
$$

so that $ a_n p_{n-1} \leq p_n < a_n p_{n-1} + a_n $, and therefore $ r_{n-1} \leq r_n \leq x $. Let
$$
p_n = a_n p_{n-1} + u_n;
$$
then $ 0 \leq u_n - a_n $, which is equivalent to $ 0 \leq u_n \leq a_n - 1 $, since $ u_n $ is an integer. Hence
$$
r_n = r_{n-1} + \frac{u_n}{d_n} = p_0 + \sum_{k=1}^n \frac{u_k}{d_k},
$$
and, since $ x = \lim_{n \to \infty} r_n $,
$$
x = p_0 + \sum_{n=1}^\infty \frac{u_n}{d_n}.
$$
The series on the right-hand side of (4), whose sum is $ x $, is called the expansion of $ x $ relative to the base sequence $ (d_n) $. All the coefficients $ u_n $ are $ \geq 0 $; $ p_0 $ is, by definition, the largest integer $ p $ such that $ p \leq x $; it is called the integral part of $ x $, and is often denoted by $ [x] $.

### 3. DEFINITION OF A REAL NUMBER BY MEANS OF ITS EXPANSION

Conversely, suppose we are given an integer $ q_0 $ and a sequence $ (v_n) $ ($ n \geq 1 $) of integers such that $ 0 \leq v_n \leq a_n - 1 $; we ask whether there is a number $ x $ whose expansion (4) is such that $ p_0 = q_0 $ and $ u_n = v_n $ for all $ n $. If such a number exists it is unique, because it is equal to
$$
q_0 + \sum_{n=1}^\infty \frac{v_n}{d_n}.
$$
For each integer $ m > 0 $ we have (by the principle of comparison)
$$
\sum_{n=m+1}^\infty \frac{v_n}{d_n} \leq \sum_{n=m+1}^\infty \frac{a_n - 1}{d_n} = \sum_{n=m+1}^\infty \left( \frac{1}{d_{n-1}} - \frac{1}{d_n} \right) = \frac{1}{d_m}
$$
and the extreme left-hand and right-hand terms are equal only if $ v_n = a_n - 1 $ for each $ n > m $ (\S 7, no. 1, Theorem 2). Hence the series whose general term is $ \frac{v_n}{d_n} $ is convergent; moreover, if $ x = q_0 + \sum_{n=1}^\infty \frac{v_n}{d_n} $, we have
$$
s_m = q_0 + \sum_{n=1}^m \frac{v_n}{d_n} \leq x \leq s_m + \frac{1}{d_m}
$$
and $ x = s_m + \frac{1}{d_m} $ only if $ v_n = a_n - 1 $ for each $ n > m $. Since $ s_m $ is a fraction with denominator $ d_m $, the approximation $ r_m $ to $ x $ to within $ 1/d_m $ by defect is equal to $ s_m $ or $ s_m + \frac{1}{d_m} $; and the latter alternative can occur only if $ v_n = a_n - 1 $ for all $ n > m $. Thus:
(i) There is an *infinity* of values of $ n $ such that $ v_n < a_n - 1 $: then the series $ q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n} $ is identical with the expansion of its sum $ x $.
(ii) There is an integer $ m \geq 0 $ such that $ v_n = a_n - 1 $ whenever $ n > m $, and $ v_m < a_m - 1 $ (if $ m > 0 $); then the sum $ x $ of the series $ q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n} $ is equal to the rational number
$$
q_0 + \sum_{n=1}^{m} \frac{v_n}{d_n} + \frac{1}{d_m}
$$
which is of the form $ k/d_m $ ($ k $ an integer); the *expansion* of $ x $ is identical with the series (5), in which all the terms with indices $ > m $ are zero; such an expansion is said to be *terminating*, or to *terminate*. The series
$$
q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n} = q_0 + \sum_{n=1}^{m} \frac{v_n}{d_n} + \sum_{n=m+1}^{\infty} \frac{a_n - 1}{d_n}
$$
is called the *improper expansion* of the number $ x $.

Conversely, let $ x $ be a rational number which can be written in the form of a fraction with denominator $ d_n $ for some value of $ n $. Let $ m $ be the smallest integer such that $ x $ is of the form $ k/d_m $ ($ k $ an integer); we have $ r_n < x $ for $ n < m $, and $ r_m = x $, and therefore the expansion of $ x $ is of the form (5), and $ x $ has an improper expansion given by (6); moreover this improper expansion is *unique*.

A rational number, written in its irreducible form $ p/q $, is equal to a fraction with denominator $ d_n $ if and only if $ q $ *divides* $ d_n $ (the number $ m $ will therefore be the smallest integer $ n $ such that $ q $ divides $ d_n $). It can happen that *every rational number* has this property (for a suitably chosen $ n $) : this will be the case if and only if every integer $ > 0 $ divides some $ d_n $, e.g., if $ d_n = n! $ If the $ d_n $ have this property, then a number is rational if and only if its expansion, relative to the sequence $ (d_n) $, terminates.

To summarize: to every sequence $ s $ whose initial term $ q_0 $ is an arbitrary integer, and whose term $ v_n (n \geq 1) $ is such that $ 0 \leq v_n \leq a_n - 1 $, corresponds a real number equal to $ q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n} $; if $ I_n $ denotes the interval $[0, a_n - 1]$ of $ \mathbf{N} $, we thus define a mapping $ \varphi $ of $ X = \mathbf{Z} \times \prod_{n=1}^{\infty} I_n $ *onto* the real line $ \mathbf{R} $; moreover the equation $ \varphi(s) = x $, where $ x \in \mathbf{R} $ is given, has *one* solution if $ x $ is not a fraction with denominator $ d_n $ (for some $ n $), and *two* solutions otherwise.

### 4. COMPARISON OF EXPANSIONS

If we know the expansions of two distinct real numbers $ x $ and $ y $, we can determine whether $ x < y $ or $ x > y $.

Let $ x = p_0 + \sum_{n=1}^{\infty} u_n / d_n $, $ y = q_0 + \sum_{n=1}^{\infty} v_n / d_n $ be the expansions of $ x $ and $ y $. If $ p_0 < q_0 $ then $ x < y $, since

$$
p_0 \leq x < p_0 + 1 \leq q_0 \leq y.
$$

More generally, suppose that $ p_0 = q_0 $ and $ u_n = v_n $ for $ 1 \leq n \leq m $, but that $ u_m < v_m $; if

$$
r_n = p_0 + \sum_{k=1}^{n} u_k / d_k, \quad s_n = q_0 + \sum_{k=1}^{n} v_k / d_k,
$$

then $ r_n = s_n $ for $ n < m $, and since $ u_m + 1 \leq v_m $, $ r_m + \frac{1}{d_m} \leq s_m $; but $ r_m \leq x < r_m + \frac{1}{d_m} \leq s_m \leq y $, hence again we have $ x < y $. In other words, *the order of $ x $ and $ y $ is the same as the order of the first two distinct terms of their respective expansions*.

It follows that, if $ p_0 = q_0 $ and $ u_n = v_n $ for $ n < m $, then the first $ m $ terms of the expansion of every number $ z $ belonging to the closed interval with end-points $ x $ and $ y $ are the *same* as those of the expansions of $ x $ and $ y $.

We remark also that, in this case, we have $ |y - x| \leq \frac{1}{d_{m-1}} $. If we endow $ \mathbf{Z} $ and the intervals $ I_n $ with the *discrete* topology, it follows that the mapping $ \varphi $ defined above is *continuous* on the *product space* $ X $.

### 5. EXPANSIONS TO BASE A

The most important base sequences are those for which $ d_n = a^n $, where $ a $ is an integer $ > 1 $; $ a $ is then said to be the *base number* (or simply the *base*) of the corresponding expansions. For numerical calculations, expansions to base 10, which are called *decimal expansions*, are used; also expansions to base 2 (*dyadic* expansions) and base 3 (*triadic* expansions) are often used.

To represent the approximations by defect $ r_n $ to a number $ x \geq 0 $, in its expansion to base $ a $, the following symbolism is employed: each integer $ u $ such that $ 0 \leq u \leq a - 1 $ is denoted by a particular sign; if

$$
r_n = p_0 + \sum_{k=1}^{n} \frac{u_k}{d_k},
$$

we first write down, with the aid of these signs, the representation to base $ a $ of the integer $ p_0 = [x] \geq 0 $ (*Set Theory*, Chapter III, § 5, no. 7), then we put a point ("decimal point") and we write successively the signs representing the numbers $ u_1, u_2, \ldots, u_n $. If S is the symbol thus obtained, it is customary to write $ x = S... $, by abuse of language. It should be understood once and for all that such a relation is only an abbreviated method of indicating that the right-hand side is the approximation to $ x $ to within $ 1/a^n $ by defect.

For negative numbers the established usage is different: we write an approximation to $ x' = -x > 0 $ in the symbolism described above, and precede it by the sign “—”; it is thus an approximation to $ x $ to within $ 1/a^n $ by excess that is so denoted.

This usage has its inconveniences for numerical calculations. In the notation for negative logarithms the same symbolism is adopted as for positive numbers, by putting a bar over the integral part, to indicate that it is equal to the negative of the number written.

### 6. THE POWER OF R

We have $ \mathbf{R} = \bigcup_{n \in \mathbf{Z}} [n, n+1[ $, and all the intervals $ [n, n+1[ $ are equipotent to $ [0, 1[ $. Since $ [0, 1[ $ is an infinite set it follows that $ \mathbf{R} $ is equipotent to the interval $ [0, 1[ $. By considering the dyadic expansion of the numbers of the interval $ [0, 1[ $ we shall show that this interval is equipotent to the set S of all sequences $ (u_n) $ in which each term is equal to 0 or 1.

First, it is equipotent to the subset $ S' $ of S consisting of sequences $ (u_n) $ such that $ u_n = 0 $ for an infinity of values of $ n $. On the other hand, the complement $ S'' $ of $ S' $ in S is equipotent to the set of all improper expansions of rational numbers which are equal to a fraction with denominator $ 2^n $; these numbers form a subset of $ \mathbf{Q} $, hence the set of them is countable and therefore so is $ S'' $. Since $ S' $ is infinite, it is equipotent to S, hence the result.

Now S is equipotent to $ \mathfrak{P}(\mathbf{N}) $; for we can define a bijection of $ \mathfrak{P}(\mathbf{N}) $ onto S by mapping each subset A of $ \mathbf{N} $ to the sequence $ (u_n) $ such that $ u_n = 0 $ if $ n \in A $ and $ u_n = 1 $ if $ n \notin CA $. We have thus proved:

#### Theorem 1 (Cantor) {#top-iv-s8-thm-1 .statement}

*The set of real numbers is equipotent to the set of all subsets of a countably infinite set.*

#### Corollary {#top-iv-s8-n6-cor-1 .statement}

*The set of real numbers has a cardinal strictly greater than the cardinal of a countable set.*

A set equipotent to $ \mathbf{R} $ is said to have the power of the continuum. By Proposition 1 of § 4, no. 1, every interval which contains more than one point has the power of the continuum. Again, the complement of a countable subset of $ \mathbf{R} $ has the power of the continuum in particular, *the set of all irrational numbers has the power of the continuum*.

### Exercises {#top-iv-s8-exercises}

See the [exercises for § 8](exercises/s8/).
