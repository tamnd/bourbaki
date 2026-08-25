---
book: fvr
book_title: Functions of a Real Variable
chapter: III
chapter_title: ELEMENTARY FUNCTIONS
section: 1
section_title: DERIVATIVES OF THE EXPONENTIAL AND CIRCULAR FUNCTIONS
lang: en
source: fvr-i-vii
pdf_pages: 0106-0119, 0130-0140
extraction: ocr
subsections:
    - "no": 1
      title: DERIVATIVES OF THE EXPONENTIAL FUNCTIONS; THE NUMBER $ e $
      page: 0
      pdf_page: 106
    - "no": 2
      title: DERIVATIVE OF $ \log_a x $
      page: 0
      pdf_page: 108
    - "no": 3
      title: DERIVATIVES OF THE CIRCULAR FUNCTIONS; THE NUMBER $ \pi $
      page: 0
      pdf_page: 109
    - "no": 4
      title: INVERSE CIRCULAR FUNCTIONS
      page: 0
      pdf_page: 110
    - "no": 5
      title: THE COMPLEX EXPONENTIAL
      page: 0
      pdf_page: 112
    - "no": 6
      title: PROPERTIES OF THE FUNCTION $ e^z $
      page: 0
      pdf_page: 113
    - "no": 7
      title: THE COMPLEX LOGARITHM
      page: 0
      pdf_page: 115
    - "no": 8
      title: PRIMITIVES OF RATIONAL FUNCTIONS
      page: 0
      pdf_page: 116
    - "no": 9
      title: COMPLEX CIRCULAR FUNCTIONS; HYPERBOLIC FUNCTIONS
      page: 0
      pdf_page: 117
statements: 9
exercises: 39
content_sha256: f6d280b87294e7ccbf5da008fbb8c99fc9b148507e42e21b94db3deb3fbc13f4
---

## § 1. DERIVATIVES OF THE EXPONENTIAL AND CIRCULAR FUNCTIONS

### 1. DERIVATIVES OF THE EXPONENTIAL FUNCTIONS; THE NUMBER $ e $

We know that every continuous homomorphism of the additive group $ \mathbf{R} $ into the multiplicative group $ \mathbf{R}^* $ of real numbers $ \neq 0 $ is a function of the form $ x \mapsto a^x $ (called an exponential function) where $ a $ is a number $ > 0 $ (TG, V, p.11); it is an isomorphism of $ \mathbf{R} $ onto the multiplicative group $ \mathbf{R}_+^* $ of numbers $ > 0 $ if $ a \neq 1 $, and the inverse isomorphism from $ \mathbf{R}_+^* $ onto $ \mathbf{R} $ is denoted by $ \log_a x $ and is called the logarithm to the base $ a $.

We shall see that the function $ f(x) = a^x $ has, for every $ x \in \mathbf{R} $, a derivative of the form $ c.a^x $ (where clearly $ c = f'(0) $). This results from the following general theorem:

#### Theorem 1 {#fvr-iii-s1-thm-1 .statement}

*Let E be a complete normed algebra over the field $ \mathbf{R} $, with a unit element $ \mathbf{e} $, and let $ \mathbf{f} $ be a continuous group homomorphism of the additive group $ \mathbf{R} $ into the multiplicative group G of invertible elements of E. Then the map $ \mathbf{f} $ is differentiable at every $ x \in \mathbf{R} $, and*

$$
\mathbf{f}'(x) = \mathbf{f}(x)\mathbf{f}'(0).
$$

First we note that, E being a complete algebra, G is open in E (*Gen. Top.*, IX, p. 179, prop. 14). Consider the function $ g(x) = \int_0^a \mathbf{f}(x + t)\,dt $, where $ a > 0 $ is a number which we shall choose later; since $ \mathbf{f}(x + t) = \mathbf{f}(x)\mathbf{f}(t) $ by hypothesis, we have $ g(x) = \int_0^a \mathbf{f}(x)\mathbf{f}(t)\,dt = \mathbf{f}(x) \int_0^a \mathbf{f}(t)\,dt $ (I, p. 6, prop. 3). Let $ \alpha > 0 $ be such that the ball $ \|x - \mathbf{e}\| \leq \alpha $ is contained in G; since $ \mathbf{f}(0) = \mathbf{e} $ and $ \mathbf{f} $ is continuous by hypothesis, one can assume that $ a $ is small enough so that $ \|\mathbf{f}(t) - \mathbf{e}\| \leq \alpha $ on $[0, a]$; consequently (II, p. 61, formula (16)) one has

$$
\left\| \frac{1}{a} \int_0^a \mathbf{f}(t)\,dt - \mathbf{e} \right\| \leq \alpha,
$$

and $ \frac{1}{a} \int_0^a f(t) \, dt $ belongs to G; in other words, is invertible; so too is $ b = \int_0^a f(t) \, dt $ and one can write $ f(x) = g(x)b^{-1} $; it is therefore enough to show that g is differentiable; now, by the change of variable $ x + t = u $ we have $ g(x) = \int_x^{x+a} f(u) \, du $; since f is continuous, g is differentiable for all $ x \in \mathbf{R} $ (II, p. 56, prop. 3), and

$$
g'(x) = f(x+a) - f(x) = f(x)(f(a) - e).
$$

Hence $ f'(x) = g'(x)b^{-1} = f(x)c $, where $ c = (f(a) - e)b^{-1} $, and clearly $ f'(0) = c $.

Conversely, one can show, either directly (III, p. 115, exerc. 1), or by means of the theory of linear differential equations (IV, p. 188), that every differentiable map f of $ \mathbf{R} $ into a complete normed algebra E, such that $ f'(x) = f(x)c $ and $ f(0) = e $, is a homomorphism of the additive group $ \mathbf{R} $ into the multiplicative group G.

#### Proposition 1 {#fvr-iii-s1-prop-1 .statement}

*For every number $ a > 0 $ and $ \neq 1 $ the exponential function $ a^\lambda $ admits at every point $ x \in \mathbf{R} $ a derivative equal to $ (\log_e a)a^\lambda $ where e is a number $ > 1 $ (independent of $ a $).*

Applying th. 1 to the case where E is the field $ \mathbf{R} $ itself now shows that $ a^\lambda $ has a derivative equal to $ \varphi(a).a^\lambda $ at every point, where $ \varphi(a) $ is a real number $ \neq 0 $ depending only on $ a $. Let $ b $ be a second number $ > 0 $ and $ \neq 1 $; the function $ b^\lambda $ has a derivative equal to $ \varphi(b).b^\lambda $ from the above; on the other hand, we have $ b^\lambda = a^\lambda \log_a b $ so (I, p. 9, prop. 5) the derivative of $ b^\lambda $ is equal to $ \log_a b.\varphi(a)b^\lambda $; on comparing these two expressions we obtain

$$
\varphi(b) = \varphi(a).\log_a b.
$$ (2)

One deduces that there is one unique number $ b $ such that $ \varphi(b) = 1 $; by (2) this relation is equivalent to $ b = a^{1/\varphi(a)} $. It is conventional to denote the real number so obtained by e; from (2) one has $ \varphi(a) = \log_e a $, which completes the proof of prop. 1.

One often writes $ \exp x $ instead of $ e^x $.

The definition of the number e shows that

$$
D(e^\lambda) = e^\lambda
$$ (3)

which proves that $ e^\lambda $ is strictly increasing, hence that $ e > 1 $.

In §2 (III, p. 105) we shall see how to calculate arbitrarily close approximations to e.

#### Definition 1 {#fvr-iii-s1-def-1 .statement}

*Logarithms to the base e are called Naperian logarithms (or natural logarithms).*

We usually omit the base in the notation for the Naperian logarithm. Unless it is stated to the contrary, the notation $ \log x $ ($ x > 0 $) will denote the *Naperian logarithm* of $ x $. With this notation, prop. 1 can be written as the identity

$$
D(a^\lambda) = (\log a)a^\lambda
$$ (4)

valid for any $ a > 0 $ ($ \log a = 0 $ when $ a = 1 $).

This relation shows that $ a^x $ has derivatives of *every order*, and that
$$
D^n(a^x) = (\log a)^n a^x.
$$
(5)

In particular, for $ a > 0 $ and $ \neq 1 $ one has $ D^2(a^x) > 0 $ for all $ x \in \mathbf{R} $, and hence $ a^x $ is *strictly convex* on $ \mathbf{R} $ (I, p. 31, corollary). From this one deduces the following proposition:

#### Proposition 2 ("geometric mean inequality") {#fvr-iii-s1-prop-2 .statement}

*For any numbers* $ z_i > 0 $ ($ 1 \leq i \leq n $) *and numbers* $ p_i > 0 $ *such that* $ \sum_{i=1}^n p_i = 1 $, *one has*
$$
z_1^{p_1} z_2^{p_2} \cdots z_n^{p_n} \leq p_1 z_1 + p_2 z_2 + \cdots + p_n z_n.
$$
(6)
*Moreover, the two sides of (6) are equal only if the* $ z_i $ *are equal.*

Let us put $ z_i = e^{x_i} $; then the inequality (6) can be written
$$
\exp(p_1 x_1 + p_2 x_2 + \cdots + p_n x_n) \leq p_1 e^{x_1} + p_2 e^{x_2} + \cdots + p_n e^{x_n}.
$$
(7)
The proposition thus follows from prop. 1 of I, p. 26 applied to the function $ e^x $, which is strictly convex on $ \mathbf{R} $.

One says that the left- (resp. right-) hand side of (6) is the *weighted geometric mean* (resp. *weighted arithmetic mean*) of the $ n $ numbers $ z_i $ relative to the *weights* $ p_i $ ($ 1 \leq i \leq n $). If $ p_i = 1/n $ for $ 1 \leq i \leq n $, one calls the corresponding arithmetic and geometric means the *ordinary* arithmetic and geometric means of the $ z_i $. Then the inequality (6) can be written
$$
(z_1 z_2 \cdots z_n)^{1/n} \leq \frac{1}{n}(z_1 + z_2 + \cdots + z_n).
$$
(8)

### 2. DERIVATIVE OF $ \log_a x $

Since $ a^x $ is strictly monotone on $ \mathbf{R} $ for $ a \neq 1 $, applying the rule for differentiating inverse functions (I, p. 17, prop. 6) gives, for all $ x > 0 $
$$
D(\log_a x) = \frac{1}{x \log a}
$$
(9)
and in particular
$$
D(\log x) = \frac{1}{x}.
$$
(10)

If $ u $ is a real function admitting a derivative at the point $ x_0 $ and such that $ u(x_0) > 0 $, then the function $ \log u $ admits a derivative equal to $ u'(x_0)/u(x_0) $ at the point $ x_0 $. In particular, we have $ D(\log |x|) = 1/|x| = 1/x $ if $ x > 0 $, and
$$
D(\log |x|) = -\frac{1}{|x|} = \frac{1}{x}
$$
if $ x < 0 $; in other words, $ D(\log |x|) = 1/x $ for any $ x \neq 0 $. One concludes that if, on an interval $ I $, the real function $ u $ is not zero and admits a finite derivative, then $ \log |u(x)| $ admits a derivative equal to $ u'/u $ on $ I $; this derivative is called the *logarithmic derivative* of $ u $. It is clear that the logarithmic derivative of $ |u|^{\alpha} $ is $ \alpha u'/u $, and that the logarithmic derivative of a product is equal to the sum of the logarithmic derivatives of the factors; these rules often provide the fastest way to calculate the derivative of a function. They give again, in particular, the formula
$$
D(x^{\alpha}) = \alpha x^{\alpha-1} \qquad (\alpha \text{ an arbitrary real number, } x > 0)
$$
which has already been shown by another method (II, p. 69).

#### Example {#fvr-iii-s1-n2-exa-1 .statement}

If $ u $ is a function $ \neq 0 $ on an interval $ I $, and $ v $ is any real function, then $ \log(|u|^v) = v \cdot \log |u| $, so if $ u $ and $ v $ are differentiable
$$
\frac{1}{|u|^v} D(|u|^v) = v' \log |u| + v \frac{u'}{u}.
$$

### 3. DERIVATIVES OF THE CIRCULAR FUNCTIONS; THE NUMBER $ \pi $

We have defined, in General Topology (*Gen. Top.*, VIII, p. 106), the continuous homomorphism $ x \mapsto \mathbf{e}(x) $ of the additive group $ \mathbf{R} $ onto the multiplicative group $ \mathbf{U} $ of complex numbers of absolute value 1; this is a periodic function with principal period 1, and $ \mathbf{e}\left(\frac{1}{4}\right) = i $. One knows (*loc. cit.*) that every continuous homomorphism of $ \mathbf{R} $ onto $ \mathbf{U} $ is of the form $ x \mapsto \mathbf{e}(x/a) $, and one puts $ \cos_a x = \mathcal{R}(\mathbf{e}(x/a)), \sin_a x = \mathcal{I}(\mathbf{e}(x/a)) $ (*trigonometric functions*, or *circular functions*, to base $ a $); these last functions are continuous maps from $ \mathbf{R} $ into $ [-1, +1] $ having principal period $ a $. We have $ \sin_a(x + a/4) = \cos_a x, \quad \cos_a(x + a/4) = -\sin_a x $, and the function $ \sin_a x $ is increasing on the interval $ [-a/4, a/4] $.

#### Proposition 3 {#fvr-iii-s1-prop-3 .statement}

*The function* $ \mathbf{e}(x) $ *has a derivative equal to* $ 2\pi i \mathbf{e}(x) $ *at every point of* $ \mathbf{R} $, *where* $ \pi $ *is a constant* $ > 0 $.

Now, th. 1 of III, p. 51, applied to the case where E is the field $ \mathbf{C} $ of complex numbers, yields the relation $ \mathbf{e}'(x) = \mathbf{e}'(0) \mathbf{e}(x) $; moreover, since $ \mathbf{e}(x) $ has constant euclidean norm, $ \mathbf{e}'(x) $ is orthogonal to $ \mathbf{e}(x) $ (I, p. 7, *Example 3*); one thus has $ \mathbf{e}'(0) = \alpha i $, with $ \alpha $ real. Since $ \sin_1 x $ is increasing on $ [-\frac{1}{4}, \frac{1}{4}] $ its derivative for $ x = 0 $ is $ \geqslant 0 $, so $ \alpha \geqslant 0 $, and since $ e(x) $ is not constant, $ \alpha > 0 $; it is conventional to denote the number $ \alpha $ so obtained by $ 2\pi $.

In §2 (III, p. 23) we shall show how one can calculate arbitrarily close approximations to the number $ \pi $.

We thus have the formula

$$
D \left( e \left( \frac{x}{a} \right) \right) = \frac{2\pi i}{a} e \left( \frac{x}{a} \right).
$$

One sees that this formula simplifies when $ a = 2\pi $; this is why one uses the circular functions relative to base $ 2\pi $ exclusively in Analysis; we agree to omit the base in the notation for these functions; unless mentioned expressly to the contrary, the notations $ \cos x $, $ \sin x $ and $ \tan x $ denote $ \cos_{2\pi} x $, $ \sin_{2\pi} x $ and $ \tan_{2\pi} x $ respectively.

With these conventions, and $ a = 2\pi $, formula (12) can be written

$$
D(\cos x + i \sin x) = \cos \left( x + \frac{\pi}{2} \right) + i \sin \left( x + \frac{\pi}{2} \right),
$$

which is equivalent to

$$
D(\cos x) = -\sin x, \qquad D(\sin x) = \cos x,
$$

from which one deduces

$$
D(\tan x) = 1 + \tan^2 x = \frac{1}{\cos^2 x}.
$$

Besides the three circular functions $ \cos x $, $ \sin x $ and $ \tan x $ one also uses, in numerical work, the three auxiliary functions: cotangent, secant and cosecant, defined by the formulae

$$
\cot x = \frac{1}{\tan x}, \qquad \sec x = \frac{1}{\cos x}, \qquad \operatorname{cosec} x = \frac{1}{\sin x}.
$$

Recall (Gen. Top., VIII, p. 109) that the angle corresponding to the base $ 2\pi $ is called the radian.

### 4. INVERSE CIRCULAR FUNCTIONS

The restriction of the function $ \sin x $ to the interval $ [-\pi/2, +\pi/2] $ is strictly increasing; one denotes its inverse by $ \operatorname{Arc}\sin x $, which is thus a strictly increasing continuous map of the interval $ [-1, +1] $ onto $ [-\pi/2, +\pi/2] $ (fig. 6). The formula for differentiating inverse functions (I, p. 9, prop. 6) gives the derivative of this function

$$
D(\operatorname{Arc}\sin x) = \frac{1}{\cos(\operatorname{Arc}\sin x)}.
$$

Since $ -\pi/2 \leq \operatorname{Arc}\sin x \leq \pi/2 $ we have $ \cos(\operatorname{Arc}\sin x) \geq 0 $, and since

$$
\sin(\operatorname{Arc}\sin x) = x,
$$
we have $ \cos(\operatorname{Arc}\sin x) = \sqrt{1 - x^2} $, from which
$$
\mathrm{D}(\operatorname{Arc}\sin x) = \frac{1}{\sqrt{1 - x^2}}.
$$
Likewise the restriction of $ \cos x $ to the interval $[0, \pi]$ is strictly decreasing; one denotes its inverse function by $ \operatorname{Arc}\cos x $, and this a strictly decreasing map of $[-1, +1]$ onto $[0, \pi]$ (fig. 6). Moreover

![Graph showing y = Arc cos x and y = Arc sin x](https://i.imgur.com/3Q5z5QG.png)

Fig. 6

$$
\sin \left( \frac{\pi}{2} - \operatorname{Arc}\cos x \right) = \cos(\operatorname{Arc}\cos x) = x
$$
and since $-\pi/2 \leq \pi/2 - \operatorname{Arc}\cos x \leq \pi/2$, we have
$$
\operatorname{Arc}\cos x = \frac{\pi}{2} - \operatorname{Arc}\sin x
$$
from which in particular it follows that
$$
\mathrm{D}(\operatorname{Arc}\cos x) = -\frac{1}{\sqrt{1 - x^2}}.
$$

Finally, the restriction of tan x to the interval ]−π/2, +π/2[ is strictly increasing; one denotes its inverse by Arc tan x, and this is a strictly increasing map from \mathbf{R} onto ]−π/2, +π/2[ (fig. 7); we have

$$
\lim_{x \to -\infty} \operatorname{Arc tan} x = -\frac{\pi}{2}, \quad \lim_{x \to +\infty} \operatorname{Arc tan} x = \frac{\pi}{2},
$$

and, by applying the formula for differentiating inverse functions and formula (15) of III, p. 95, we have

$$
\mathrm{D}\left( \operatorname{Arc tan} x \right) = \frac{1}{1 + x^2}.
$$

![Graph showing y = Arc tan x](https://i.imgur.com/3Q5z5QG.png)

Fig. 7

### 5. THE COMPLEX EXPONENTIAL

We have determined (Gen. Top., VIII, p. 106) all the continuous homomorphisms of the (additive) topological group \mathbf{C} of complex numbers onto the (multiplicative) topological group \mathbf{C}^* of complex numbers ≠ 0; these are the maps

$$
x + i y \mapsto e^{\alpha x + \beta y} \mathbf{e}(\gamma x + \delta y)
$$

where $ \alpha, \beta, \gamma, \delta $ are four real numbers subject to the single condition $ \alpha \delta - \beta \gamma \neq 0 $. We now propose to determine which of these homomorphisms $ z \mapsto f(z) $ are *differentiable* on \mathbf{C}. First we remark that it is enough for $ f $ to be differentiable at the point $ z = 0 $; indeed, for every point $ z \in \mathbf{C} $ one has

$$
\frac{f(z + h) - f(z)}{h} = f(z) \frac{f(h) - 1}{h}
$$

if $ f'(0) $ exists, then so does $ f'(z) $, and $ f'(z) = a f(z) $, with $ a = f'(0) $. On the other hand, if $ g $ is a second differentiable homomorphism, such that $ g'(z) = b g(z) $, then $ g(a z / b) = f(z) $, for one notes immediately that the quotient $ g(a z / b) / f(z) $ has an everywhere zero derivative and is equal to 1 for $ z = 0 $; all the differentiable homomorphisms are thus of the form $ z \mapsto f(\lambda z) $, where $ f $ is one of them (assuming they exist) and $ \lambda $ is any (complex) constant.

This being so, if $ f $ is differentiable at the point $ z = 0 $ then each of the maps $ x \mapsto f(x),\ y \mapsto f(iy) $ of $ \mathbf{R} $ into $ \mathbf{C} $ is necessarily differentiable at the point $ 0 $, the first having derivative $ f'(0) $, the second $ if'(0) $. Now the derivatives of the maps $ x \mapsto e^{\alpha x} \mathbf{e}(\gamma x),\ y \mapsto e^{\beta y} \mathbf{e}(\delta y) $ at the point $ 0 $ are respectively equal to $ \alpha + 2\pi i \gamma $ and $ \beta + 2\pi i \delta $, from which $ \beta = -2\pi \gamma $ and $ \alpha = 2\pi \delta $; these conditions are, in particular, satisfied by the homomorphism $ x + iy \mapsto e^z \mathbf{e}(y/2\pi) $, which we shall denote provisionally by $ f_0 $. We shall now show that $ f_0 $ is actually differentiable at the point $ z = 0 $.

It is clear that $ x \mapsto f_0(x) $ and $ y \mapsto f_0(iy) $ have derivatives of every order; in particular, Taylor's formula of order 1 applied to these functions shows that for every $ \varepsilon > 0 $ there is an $ r > 0 $ such that, if one puts

$$
f_0(x) = 1 + x + \varphi(x)x,\qquad f_0(iy) = 1 + iy + \psi(y)y,
$$

then the conditions $ |x| \leq r,\ |y| \leq r $ imply that $ |\varphi(x)| \leq \varepsilon $ and $ |\psi(y)| \leq \varepsilon $; this being so, we have $ f_0(x + iy) = f_0(x)f_0(iy) = 1 + (x + iy) + \theta(x,\ y) $ with

$$
\theta(x,\ y) = (i + \varphi(x)\psi(y))xy + (1 + x)y\psi(y) + (1 + iy)x\varphi(x);
$$

for $ |z| \leq r $ we have $ |x| \leq r $ and $ |y| \leq r $, whence

$$
|\theta(x,\ y)| \leq (1 + \varepsilon^2)|z|^2 + 2\varepsilon|z|(1 + |z|)
$$

which proves that the quotient $ \frac{f_0(z) - 1 - z}{z} $ tends to 0 with $ z $, that is to say, the function $ f_0 $ admits a derivative equal to 1 at the point $ z = 0 $. The above thus proves that, for all $ z \in \mathbf{C} $,

$$
D(f_0(z)) = f_0(z).
$$

This property establishes the connection between $ f_0 $ and the function $ e^z $, which is moreover the restriction of $ f_0 $ to the real axis; for this reason we make the following definition:

**Definition 2** *The homomorphism* $ x + iy \mapsto e^z \mathbf{e}(y/2\pi) $ *of* $ \mathbf{C} $ *onto* $ \mathbf{C}^* $ *is called the complex exponential; its value at an arbitrary complex number* $ z $ *is denoted by* $ e^z $ *or* $ \exp z $.

### 6. PROPERTIES OF THE FUNCTION $ e^z $

The fact that $ z \mapsto e^z $ is a homomorphism of $ \mathbf{C} $ onto $ \mathbf{C}^* $ may be expressed by the identities

$$
e^{z+z'} = e^z e^{z'},\qquad e^0 = 1.\qquad e^{-z} = 1/e^z.
$$

By definition, one has, for every $ z = x + iy $,

$$
e^{x+iy} = e^x (\cos y + i \sin y)
$$

and since $ e^{\lambda} > 0 $ one sees that $ e^z $ has *absolute value* $ e^{\lambda} $ and *amplitude* $ y $ (modulo $ 2\pi $).

In particular, def. 2 (III, p. 98) gives
$$
\mathbf{e}(x) = e^{2\pi i x}
$$
which permits us to write the formulae defining $ \cos x $ and $ \sin x $ in the form
$$
\cos x = \frac{1}{2} (e^{i x} + e^{-i x}), \qquad \sin x = \frac{1}{2i} (e^{i x} - e^{-i x})
$$
*(Euler’s formulae)*.

Since $ 2\pi $ is the principal period of $ \mathbf{e}(y/2\pi) $, $ 2\pi i $ is the *principal period* of $ e^z $; in other words, the group of periods of $ e^z $ is the set of numbers $ 2n\pi i $, where $ n $ runs through $ \mathbf{Z} $.

Finally, formula (21) of III, p. 98 can be written
$$
\mathrm{D}(e^z) = e^z
$$
whence, for every complex number $ a $
$$
\mathrm{D}(e^{a z}) = a\, e^{a z}.
$$

#### Remark {#fvr-iii-s1-n6-rem-1 .statement}

If, in formula (27), one restricts the function $ e^{a z} $ ($ a $ complex) to the real axis, one again obtains, for $ x $ real,
$$
\mathrm{D}(e^{a x}) = a\, e^{a x}.
$$
This formula allows us to calculate a primitive for each of the functions $ e^{\alpha x} \cos \beta x $, $ e^{\alpha x} \sin \beta x $ ($ \alpha $ and $ \beta $ real); indeed we have $ e^{(\alpha + i \beta)x} = e^{\alpha x} \cos \beta x + i e^{\alpha x} \sin \beta x $, so, by (28)
$$
\mathrm{D}\left( \mathcal{R}\left( \frac{1}{\alpha + i \beta}\, e^{(\alpha + i \beta)x} \right) \right) = e^{\alpha x} \cos \beta x
$$
$$
\mathrm{D}\left( \mathcal{I}\left( \frac{1}{\alpha + i \beta}\, e^{(\alpha + i \beta)x} \right) \right) = e^{\alpha x} \sin \beta x.
$$
In the same way one reduces the evaluation of a primitive of $ x^n e^{\alpha x} \cos \beta x $, or of $ x^n e^{\alpha x} \sin \beta x $ (*n* *an integer* $ > 0 $) to that of a primitive of $ x^n e^{(\alpha + i \beta)x} $; now, the formula for integration by parts of order $ n + 1 $ (II, p. 60, formula (11)) shows that a primitive of this last function is
$$
e^{(\alpha + i \beta)x} \left[ \frac{x^n}{\alpha + i \beta} - \frac{n x^{n-1}}{(\alpha + i \beta)^2} + \frac{n(n-1)x^{n-2}}{(\alpha + i \beta)^3} + \cdots + (-1)^n \frac{n!}{(\alpha + i \beta)^{n+1}} \right].
$$
By Euler’s formulae one can on the other hand express every positive integral power of $ \cos x $ or of $ \sin x $ as a linear combination of exponentials $ e^{ip x} $ ($ p $ a positive or negative integer). By formula (28) one can thus express a primitive of a function of the form $ x^n e^{\alpha x} (\cos \beta x)' (\sin \gamma x)^s $ as a linear combination of functions of the form $ x^p e^{\alpha x} \cos \lambda x $ and $ x^p e^{\alpha x} \sin \mu x $ and ($ n, p, r, s $ integers, $ \alpha, \beta, \gamma, \lambda, \mu $ real).

#### Example {#fvr-iii-s1-n6-exa-1 .statement}

One has

$$
\sin^{2n} x = \frac{(-1)^n}{2^{2n}} \left( e^{i x} - e^{-i x} \right)^{2n} = \frac{(-1)^n}{2^{2n}} \left( e^{2n i x} - \binom{2n}{1} e^{(2n-2)i x} + \cdots + e^{-2n i x} \right)
$$

whence

$$
\int_0^1 \sin^{2n} t \, dt = \frac{(-1)^n}{2^{2n}} \left( \frac{1}{n} \sin 2n x - \binom{2n}{1} \frac{1}{n-1} \sin(2n-2)x + \cdots \right.
$$
$$
\left. + (-1)^{n-1} \binom{2n}{n-1} \sin 2x + (-1)^n \binom{2n}{n} x \right)
$$

and in particular

$$
\int_0^{\pi/2} \sin^{2n} t \, dt = \binom{2n}{n} \frac{1}{2^{2n}} \frac{\pi}{2} = \frac{1.3.5 \ldots (2n-1)}{2.4.6 \ldots 2n} \frac{\pi}{2}.
$$ (29)

### 7. THE COMPLEX LOGARITHM

Let B be the "strip" formed by the points $ z = x + i y $ such that $ -\pi \leq y < \pi $; the function $ e^z $ takes each of its values once and only once on B; in other words, $ z \mapsto e^z $ is a bijective continuous map of B onto $ \mathbf{C}^* $; the image under this map of the (half-open) segment $ x = x_0,\ -\pi \leq y < \pi $ is the circle $ |z| = e^{x_0} $; the image of the line $ y = y_0 $ is the (open) half-line defined by $ \mathrm{Am}(z) = y_0 $ (mod. $ 2\pi $). The image under $ z \mapsto e^z $ of the interior $ \dot{B} $ of B, that is, of the set of $ z \in \mathbf{C} $ such that $ |\mathcal{I}(z)| < \pi $, is the complement F of the (closed) negative real half-axis in $ \mathbf{C} $; if one agrees to denote by $ \mathrm{Am}(z) $ the measure of the amplitude of $ z $ which belongs to $ [-\pi, \pi[ $, then the set F can be defined by the relations $ -\pi < \mathrm{Am}(z) < \pi $. Since $ z \mapsto e^z $ is a strict homomorphism of $ \mathbf{C} $ onto $ \mathbf{C}^* $ the image under this map of any open subset of B (so of $ \mathbf{C} $) is an open set in $ \mathbf{C}^* $ (so in F); in other words, the restriction of $ z \mapsto e^z $ to B is a homeomorphism of $ \dot{B} $ onto F. We denote by $ z \mapsto \log z $ the homeomorphism of F onto B which is the inverse of the latter; for a complex number $ z \in F $, $ \log z $ is called the principal value of the logarithm of $ z $. If $ z = x + i y $ and $ \log z = u + i v $ then $ x + i y = e^{u+i v} $, whence $ e^u = |z| $, and since $ -\pi < v < \pi $, we have $ v = \mathrm{Am}(z) $. Moreover, we have $ \tan(v + \pi/2) = -x/y $ if $ y \neq 0 $; thus we can write

$$
\begin{cases}
u = \log |z| = \frac{1}{2} \log(x^2 + y^2) \\
v = \frac{\pi}{2} - \mathrm{Arc}\tan \frac{x}{y} & \text{if } y > 0 \\
v = 0 & \text{if } y = 0 \\
v = -\frac{\pi}{2} - \mathrm{Arc}\tan \frac{x}{y} & \text{if } y < 0.
\end{cases}
$$ (30)

It is clear that $ \log z $ is the extension to F of the function $ \log x $ defined on the positive open real half-axis $ \mathbf{R}_+^* $. If $ z,\ z' $ are two points of F such that $ zz' $ is not real negative, we have $ \log(zz') = \log z + \log z' + 2\varepsilon \pi i $, where $ \varepsilon = +1,\ -1 $ or 0 depending on the values of $ \mathrm{Am}(z) $ and $ \mathrm{Am}(z') $.

We note that at the points of the negative real half-axis the function $ \log z $ has no limit; to be precise, if $ x $ tends to $ x_0 < 0 $ and if $ y $ tends to 0 remaining > 0 (resp. < 0), then $ \log z $ tends to $ \log |x_0| + \pi i $ (resp. $ \log |x_0| - \pi i $); when $ z $ tends to 0, $ |\log z| $ increases indefinitely.

We shall see later how the theory of analytic functions allows us to extend the function $ \log z $, and to define the complex logarithm in full generality.

Since $ \log z $ is the inverse homeomorphism of $ e^z $, the formula for differentiating inverse functions (I, p. 9, prop. 6) shows that $ \log z $ is differentiable at every point $ z \in \mathbf{F} $, and that
$$
\mathrm{D}(\log z) = \frac{1}{e^{\log z}} = \frac{1}{z}
$$
a formula which generalizes formula (10) of III, p. 93.

### 8. PRIMITIVES OF RATIONAL FUNCTIONS

Formula (31) allows us to evaluate the primitive of an arbitrary rational function $ r(x) $ of a real variable $ x $, with real or complex coefficients. We know (A.VII.7) that such a function can be written (in unique manner) as a finite sum of terms, which are:

$ a) $ either of the form $ ax^p $ ($ p $ an integer $ \geqslant 0 $, $ a $ a complex number);
$ b) $ or of the form $ a/(x-b)^m $ ($ m $ an integer $ \geqslant 0 $, $ a $ and $ b $ complex numbers).

Now it is easy to obtain a primitive of each of these terms:
$ a) $ a primitive of $ ax^p $ is $ a \frac{x^{p+1}}{p+1} $;
$ b) $ if $ m > 1 $ a primitive of $ a/(x-b)^m $ is $ \frac{a}{(1-m)(x-b)^{m-1}} $;
$ c) $ finally, from formulae (10) (III, p. 93) and (31) (III, p. 101), a primitive of $ \frac{a}{x-b} $ is $ a \log |x-b| $ if $ b $ is real, $ a \log(x-b) $ if $ b $ is complex. In the last case, if $ b = p + iq $, one has furthermore (III, p. 100, formulae (30))
$$
\log(x-b) = \log \sqrt{(x-p)^2 + q^2} + i \operatorname{Arc tan} \frac{x-p}{q} \pm i \frac{\pi}{2}.
$$

We postpone the examination of more practical methods for explicitly determining a primitive of a rational function given explicitly to the part of this work dedicated to Numerical Calculus.

One can reduce to the evaluation of a primitive of a rational function:

1° the evaluation of a primitive of a function of the form $ r(e^{a x}) $, where $ r $ is a rational function and $ a $ a real number; indeed by the change of variable $ u = e^{a x} $ one reduces to finding a primitive for $ r(u)/u $;

2° the evaluation of a primitive of a function of the form $ f(\sin a x, \cos a x) $, where $ f $ is a rational function of two variables and $ a $ is a real number; the change of variables $ u = \tan(a x/2) $ reduces this to finding a primitive for

$$
\frac{2}{1 + u^2} \int \left( \frac{2u}{1 + u^2}, \frac{1 - u^2}{1 + u^2} \right).
$$

### 9. COMPLEX CIRCULAR FUNCTIONS; HYPERBOLIC FUNCTIONS

Euler’s formulae (25) (III, p. 99) and the definition of $ e^z $ for every complex $ z $ allow us to extend to $ \mathbf{C} $ the functions $ \cos x $ and $ \sin x $ defined on $ \mathbf{R} $, by putting, for all $ z \in \mathbf{C} $

$$
\cos z = \frac{1}{2} (e^{i z} + e^{-i z}), \qquad \sin z = \frac{1}{2i} (e^{i z} - e^{-i z})
$$
(cf. III, p. 119, exerc. 19).

These functions are periodic with principal period $ 2 \pi $; that is, one has $ \cos(z + \pi/2) = -\sin z, \sin(z + \pi/2) = \cos z $; one may also verify the identities

$$
\cos^2 z + \sin^2 z = 1 \\
\cos(z + z') = \cos z \cos z' - \sin z \sin z' \\
\sin(z + z') = \sin z \cos z' + \cos z \sin z'.
$$

More generally, every algebraic identity between circular functions for real variables remains true when one gives these variables arbitrary complex values (III, p. 119, exerc. 18).

One puts $ \tan z = \sin z / \cos z $ if $ z \neq (2k + 1)\pi/2 $ and $ \cot z = \cos z / \sin z $ if $ z \neq k \pi $; these are periodic functions with principal period $ \pi $.

Formula (27) (III, p. 99) shows that $ \cos z $ and $ \sin z $ are differentiable on $ \mathbf{C} $, and that

$$
\mathrm{D}(\cos z) = -\sin z, \qquad \mathrm{D}(\sin z) = \cos z.
$$

For $ z = i x $ ($ x $ real), the formulae (32) give

$$
\cos i x = \frac{1}{2} (e^i + e^{-i}), \qquad \sin i x = \frac{i}{2} (e^i - e^{-i}).
$$

It is convenient to have a specific notation for the real functions thus introduced; we put

$$
\begin{cases}
\cosh x = \frac{1}{2} (e^x + e^{-x}) & \text{(hyperbolic cosine of } x \text{)} \\
\sinh x = \frac{1}{2} (e^x - e^{-x}) & \text{(hyperbolic sine of } x \text{)} \\
\tanh x = \frac{\sinh x}{\cosh x} = \frac{e^x - e^{-x}}{e^x + e^{-x}} & \text{(hyperbolic tangent of } x \text{)}
\end{cases}
$$

One thus has, for every real $ x $

$$
\cos i x = \cosh x, \quad \sin i x = i \sinh x.
$$

From every identity between circular functions in a certain number of complex numbers $ z_k $ ($ 1 \leq k \leq n $) one can deduce an identity for the hyperbolic functions, by replacing $ z_k $ by $ i x_k $ ($ x_k $ real, $ 1 \leq k \leq n $) and using the formulae (34); for instance one has

$$
\cosh^2 x - \sinh^2 x = 1
$$
$$
\cosh(x + x') = \cosh x \cosh x' + \sinh x \sinh x'
$$
$$
\sinh(x + x') = \sinh x \cosh x' - \cosh x \sinh x'.
$$

The hyperbolic functions allow us to express the real and imaginary parts of $ \cos z $ and $ \sin z $ for $ z = x + i y $, since

$$
\cos(x + i y) = \cos x \cos i y - \sin x \sin i y = \cos x \cosh y - i \sin x \sinh y
$$
$$
\sin(x + i y) = \sin x \cos i y + \cos x \sin i y = \sin x \cosh y + i \cos x \sinh y.
$$

Finally, one has

$$
D(\cosh x) = \sinh x, \quad D(\sinh x) = \cosh x, \quad D(\tanh x) = 1 - \tanh^2 x = \frac{1}{\cosh^2 x}.
$$

Since $ \cosh x > 0 $ for all $ x $ one deduces that $ \sinh x $ is strictly increasing on $ \mathbf{R} $; since $ \sinh 0 = 0 $, it follows that $ \sinh x $ has the same sign as $ x $. In consequence $ \cosh x $ is strictly decreasing for $ x \leq 0 $, strictly increasing for $ x \geq 0 $, finally, $ \tanh x $ is strictly increasing on $ \mathbf{R} $. Moreover

$$
\lim_{x \to -\infty} \sinh x = -\infty, \qquad \lim_{x \to +\infty} \sinh x = +\infty
$$
$$
\lim_{x \to -\infty} \cosh x = \lim_{x \to +\infty} \cosh x = +\infty
$$
$$
\lim_{x \to -\infty} \tanh x = -1, \qquad \lim_{x \to +\infty} \tanh x = +1 \qquad \text{(fig. 8 and 9)}.
$$

Sometimes we write $ \operatorname{Arg} \sinh x $ for the inverse function of $ \sinh x $, which is a strictly increasing map from $ \mathbf{R} $ onto $ \mathbf{R} $: this function can also be expressed in terms of the logarithm, since from the relation $ x = \sinh y = \frac{1}{2}(e^y - e^{-y}) $ we deduce that $ e^{2y} - 2x e^y - 1 = 0 $, and since $ e^y > 0 $, we have $ e^y = x + \sqrt{x^2 + 1} $, that is to say

$$
\operatorname{Arg} \sinh x = \log \left( x + \sqrt{x^2 + 1} \right).
$$

Similarly, we denote by $ \operatorname{Arg} \cosh x $ the inverse of the restriction of $ \cosh x $ to $ [0, +\infty[ $; this map is strictly increasing from $ ]1, +\infty[ $ onto $ ]0, +\infty[ $; one shows as above that

$$
\operatorname{Arg} \cosh x = \log \left( x + \sqrt{x^2 - 1} \right).
$$

Finally, we denote by Arg tanh $ x $ the inverse function of tanh $ x $, which is a strictly increasing map from ]$ -1, +1 $ [ onto $ \mathbf{R} $; one has, moreover,

$$
\operatorname{Arg} \tanh x = \frac{1}{2} \log \frac{1 + x}{1 - x}.
$$

#### Remark {#fvr-iii-s1-n9-rem-1 .statement}

For complex $ z $ one sometimes writes

$$
\cosh z = \frac{1}{2} (e^z + e^{-z}) = \cos iz \\
\sinh z = \frac{1}{2} (e^z - e^{-z}) = -i \sin iz.
$$

These functions thus extend to $ \mathbf{C} $ the hyperbolic functions defined on $ \mathbf{R} $.

### Exercises {#fvr-iii-s1-exercises}

See the [exercises for § 1](exercises/s1/).
