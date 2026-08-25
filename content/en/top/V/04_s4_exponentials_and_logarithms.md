---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 4
section_title: Exponentials and logarithms
lang: en
source: top-v-x
pdf_pages: 0025-0029, 0034-0034
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF $ a^x $ AND $ \log_a x $
      page: 0
      pdf_page: 25
    - "no": 2
      title: BEHAVIOUR OF THE FUNCTIONS $ a^x $ AND $ \log_a x $
      page: 0
      pdf_page: 27
    - "no": 3
      title: MULTIPLIABLE FAMILIES OF NUMBERS $> 0$
      page: 0
      pdf_page: 28
statements: 1
exercises: 2
content_sha256: c68940cee2128331ec6615f36d357b51c3b138ed4881abd37a7be6e09b4e5422
---

## 4. EXPONENTIALS AND LOGARITHMS

### 1. DEFINITION OF $ a^x $ AND $ \log_a x $

#### Theorem 1 {#top-v-s4-thm-1 .statement}

*The multiplicative group* $ \mathbf{R}_+^* $ *of real numbers* $ > 0 $ *is a topological group isomorphic to the additive group* $ \mathbf{R} $ *of real numbers*.

For $ \mathbf{R}_+^* = ]0, +\infty[ $ is an open interval of $ \mathbf{R} $ and is therefore *homeomorphic* to $ \mathbf{R} $ (Chapter IV, § 4, no. 1, Proposition 1). By Theorem 2 of § 3, it is therefore a topological group *isomorphic* to $ \mathbf{R} $.

From the Corollary to Proposition 5 of § 1, no. 3, for every number $ a > 0 $ there is a unique continuous homomorphism $ f_a $ of $ \mathbf{R} $ into $ \mathbf{R}_+^* $ such that $ f_a(1) = a $. Hence, for all $ x \in \mathbf{R} $ and all $ y \in \mathbf{R} $ we have

$$
f_a(x + y) = f_a(x) f_a(y), \qquad f_a(-x) = \frac{1}{f_a(x)},
$$

and hence, in particular, for all $ n \in \mathbf{Z} $,

$$
f_a(n) = a^n.
$$

For this reason we denote $ f_a(x) $ by $ a^x $ for all $ x \in \mathbf{R} $; the functions $ a^x $ (for all values of $ a > 0 $) are called *exponential functions*. We have $ 1^x = 1 $ for all $ x \in \mathbf{R} $; if $ a \neq 1 $, $ x \to a^x $ is an *isomorphism* of the group $ \mathbf{R} $ onto the group $ \mathbf{R}_+^* $.

If $ a \neq 1 $, the isomorphism of $ \mathbf{R}_+^* $ onto $ \mathbf{R} $ which is the inverse of $ x \to a^x $ is called the *logarithm to base* $ a $, and its value at $ x \in \mathbf{R}_+^* $ is denoted by $ \log_a x $. Thus, with this notation, we have

(1) $$
a^{x+y} = a^x a^y \qquad (x \in \mathbf{R}, y \in \mathbf{R}, a > 0);
$$
(2) $$
a^{-x} = \frac{1}{a^x} \qquad (x \in \mathbf{R}, a > 0);
$$
(3) $$
\log_a 1 = 0, \quad \log_a a = 1 \qquad (a > 0, a \neq 1);
$$
(4) $$
\log_a (xy) = \log_a x + \log_a y \qquad (x > 0, y > 0);
$$
(5) $$
\log_a \left( \frac{1}{x} \right) = -\log_a x \qquad (x > 0);
$$
(6) $$
a^{\log_a x} = x \qquad (x > 0);
$$
(7) $$
\log_a a^x = x \qquad (x \in \mathbf{R}).
$$

By Proposition 5 of § 1, no. 3, every continuous homomorphism of $ \mathbf{R} $ into $ \mathbf{R}_+^* $ is of the form $ y \to a^{xy} $, where $ x \in \mathbf{R} $; since its value when $ y = 1 $ is $ a^x $, we have identically

(8) $$
(a^x)^y = a^{xy} \qquad (x \in \mathbf{R}, \ y \in \mathbf{R}, \ a > 0),
$$
or, changing the notation,

(9) $$
x^y = a^{y \cdot \log_a x} \qquad (x > 0, y \in \mathbf{R}, a > 0, a \neq 1).
$$

The formula (8) shows that, for every integer $ n > 0 $, we have $ (a^{1/n})^n = a $, which justifies the notation $ a^{1/n} $ introduced for the *nth root* $ \sqrt[n]{a} $, defined in Chapter IV, § 3, no. 3.

Formulas (7) and (9) show that

(10) $$
\log_a (x^y) = y \log_a x \qquad (x > 0, y \in \mathbf{R}),
$$
or, changing the notation,

(11) $$
\log_a x = \log_a b \cdot \log_b x \qquad (x > 0, a > 0, b > 0, a \neq 1, b \neq 1),
$$
which is the formula for "change of base".

Finally, let us obtain all the *continuous homomorphisms* of the topological group $ \mathbf{R}^* $ into itself; if $ g $ is such a continuous homomorphism,

$$
\log_a (g(a^x))
$$

is a continuous homomorphism of $ \mathbf{R} $ into $ \mathbf{R} $, therefore (§ 1, no. 3, Proposition 5) there exists $ \alpha \in \mathbf{R} $ such that $ \log_a (g(a^x)) = \alpha x $ for all $ x \in \mathbf{R} $; hence, by (8), $ g(x) = x^\alpha $ for all $ x > 0 $. Hence we have identically

(12) $$
(xy)^\alpha = x^\alpha y^\alpha \text{ for all } x > 0, y > 0 \text{ and } \alpha \in \mathbf{R}.
$$

By reason of formula (4), which reduces every multiplication to an addition (the only operation to which the customary system of numeration is well adapted), logarithms have long been an indispensable instrument in numerical calculations (see the Historical Note to this Chapter).

When used for this purpose, the base chosen is $ a = 10 $; and there are tables giving the values of the function $ \log_{10} x $ (to a certain approximation). In analysis, one is led to choose a different base (denoted by $ e $) which is such that $ \lim_{x \to 1, x \neq 1} \frac{\log_e x}{(x - 1)} = 1 $ (cf. Exercise 1).

### 2. BEHAVIOUR OF THE FUNCTIONS $ a^x $ AND $ \log_a x $

By Theorem 5 of Chapter IV, § 2, no. 6, if $ a \neq 1, x \to a^x $ is a strictly monotone mapping of $ \mathbf{R} $ onto the interval $ \mathbf{R}_+^* = ]0, + \infty[ $. If $ a > 1 $, we have $ a^1 = a \geq 1 = a^0 $, hence $ a^x $ is strictly increasing; moreover, since $ \mathbf{R}_+^* $ is not bounded above, $ a^x $ is not bounded above in $ \mathbf{R} $, so that

$$
\lim_{x \to +\infty} a^x = +\infty \quad (a > 1)
$$

and, by (2),

$$
\lim_{x \to -\infty} a^x = 0 \quad (a > 1).
$$

On the other hand, if $ a < 1 $, the function $ a^x $ is strictly decreasing, tends to 0 as $ x $ tends to $ +\infty $, and tends to $ +\infty $ as $ x $ tends to $ -\infty $ (Fig. 1).

![Graph showing y = a^x (a > 1) and y = a^x (a < 1)](https://i.imgur.com/1.png)

Figure 1.

![Graph showing y = log_a x (a > 1) and y = log_a x (a < 1)](https://i.imgur.com/2.png)

Figure 2.

From these properties and from (12), we deduce that if $0 < a < b$, we have $a^x < b^x$ for $x > 0$, and $a^x > b^x$ for $x < 0$; for $\left(\frac{b}{a}\right)^x > 1$ if $x > 0$, and $\left(\frac{b}{a}\right)^x < 1$ if $x < 0$.

The behaviour of $\log_a x$ in $\mathbf{R}_+^*$ is deduced from that of $a^x$ in $\mathbf{R}$; if $a > 1$, the function $\log_a x$ is strictly increasing, tends to $-\infty$ as $x$ tends to $0$, and tends to $+\infty$ as $x$ tends to $+\infty$; if $a < 1$, the function $\log_a x$ is strictly decreasing, tends to $+\infty$ as $x$ tends to $0$, and to $-\infty$ as $x$ tends to $+\infty$ (Fig. 2).

The function $a^x$ (resp. $\log_a x$), considered as defined on a subset of the extended line $\overline{\mathbf{R}}$ and taking its values in $\overline{\mathbf{R}}$, can be *extended by continuity* to $\overline{\mathbf{R}}$ (resp. to the interval $[0, +\infty]$ of $\overline{\mathbf{R}}$) by assigning to it its limiting values at the points $+\infty$ and $-\infty$ (resp. $0$ and $+\infty$).

More generally, formula (9) shows that the function $x^y$ is continuous on the subspace $\mathbf{R}_+^* \times \mathbf{R}$ of $\overline{\mathbf{R}}^2$ and tends to a limit when $(x, y)$ tends to any point $(a, b)$ of $\overline{\mathbf{R}}^2$ which lies in the closure of $\mathbf{R}_+^* \times \mathbf{R}$, with the exception of the points $(0, 0)$, $(+\infty, 0)$, $(1, +\infty)$, $(1, -\infty)$. We can therefore extend $x^y$ by continuity to those points of $\overline{\mathbf{R}}^2$ at which the limit exists; by the principle of extension of identities (Chapter I, § 8, no. 1, Proposition 2, Corollary 1), formulas (1), (4) and (8) remain valid whenever both sides have a meaning.

Note that the extension by continuity of $x^y$ does not allow us to obtain the formula $0^0 = 1$.

Note also that the definition of the exponential allows us to extend to $\mathbf{R}$ the function $n \to a^n$ defined on $\mathbf{Z}$, for all $a > 0$; but we do not obtain in this way any extension of this function when $a < 0$; a "natural" extension of this function can be defined only in terms of the theory of analytic functions.

### 3. MULTIPLIABLE FAMILIES OF NUMBERS $> 0$

The isomorphism of the topological groups $\mathbf{R}$ and $\mathbf{R}_+^*$ shows immediately that for a family $(x_i)$ of finite real numbers $> 0$ to be *multipliable* (Chapter IV, § 7, no. 4) it is necessary and sufficient that the family $(\log_a x_i)$ should be *summable* ($a$ being any number $> 0$ and $\neq 1$); and we have

$$
\prod_i x_i = a^{\sum \log_a x_i}.
$$

Likewise, an infinite product defined by a sequence $(1 + u_n)$ of finite numbers $> 0$ is *convergent* (Chapter IV, § 7, no. 6) if and only if the series whose general term is $ \log_a (1 + u_n) $ is convergent, and then we have

$$
\prod_{n=0}^{\infty} (1 + u_n) = a^{S_{n=0}^{\infty} \log_a (1 + u_n)}.
$$

The study of infinite products of real numbers $ > 0 $ is thus reduced to that of infinite series of real numbers whose terms appear in the form of logarithms; we shall see later how sums of this nature can be easily studied by means of the differential properties of the logarithm.

### Exercises {#top-v-s4-exercises}

See the [exercises for § 4](exercises/s4/).
