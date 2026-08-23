---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 1
section_title: COMPARISON OF FUNCTIONS ON A FILTERED SET
lang: en
source: fvr-i-vii
pdf_pages: 0226-0235, 0274-0274
extraction: ocr
subsections:
    - "no": 1
      title: 'COMPARISON RELATIONS: I. WEAK RELATIONS'
      page: 0
      pdf_page: 226
    - "no": 2
      title: 'COMPARISON RELATIONS: II. STRONG RELATIONS'
      page: 0
      pdf_page: 229
    - "no": 3
      title: CHANGE OF VARIABLE
      page: 0
      pdf_page: 232
    - "no": 4
      title: COMPARISON RELATIONS BETWEEN STRICTLY POSITIVE FUNCTIONS
      page: 0
      pdf_page: 232
    - "no": 5
      title: NOTATION
      page: 0
      pdf_page: 234
statements: 38
exercises: 3
content_sha256: 5938d169f8d414b2f0ad61872c6def1fa9381bea868d63d13fc922fc117ab92f
---

## § 1. COMPARISON OF FUNCTIONS ON A FILTERED SET

Let E be a set filtered by a filter with base $ \mathfrak{F} $ (*Gen. Top.*, I, p. 58); in this chapter we shall consider functions whose domain of definition is a subset of E belonging to the filter base $ \mathfrak{F} $ (the subset depending on the function) and which take their values either in the field of real numbers $ \mathbf{R} $, or, more generally, in a normed vector space over a valued field (*Gen. Top.*, IX, p. 170).

In applications, E will most often be a subspace of the real space $ \mathbf{R}^n $, or the extended line $ \overline{\mathbf{R}} $, and $ \mathfrak{F} $ will be the trace on E of the filter of neighbourhoods of a closure point of E, or else the filter of complements of relatively compact subsets of E ("neighbourhoods of the point at infinity").

It will not in general suffice to know that such a function tends to a given limit along $ \mathfrak{F} $ to be able to treat all the problems of "passage to the limit along $ \mathfrak{F} $" for expressions formed from this function.

For example, when the real variable x tends to $ +\infty $ the three functions $ x $, $ x^2 $ and $ \sqrt{x} $ all tend to $ +\infty $, but, of the expressions

$$
(x+1)^2 - x^2, \quad (x+1) - x, \quad \sqrt{x+1} - \sqrt{x},
$$

the first tends to $ +\infty $, the second to 1, the third to 0.

It is thus important to know not just the limit value of a function along $ \mathfrak{F} $ (when this limit exists) but also the "manner" in which the function approaches its limit; in other words, one is led to classify the set of functions which tend to the same limit.

### 1. COMPARISON RELATIONS: I. WEAK RELATIONS

In what follows we denote by V a normed vector space over a valued field K, and by $ \mathcal{H}(\mathfrak{F}, V) $ the set of functions with values in V, each of which is defined on a subset of E belonging to the filter base $ \mathfrak{F} $. The relations which we shall define between such functions have a *local* character relative to the filter with base $ \mathfrak{F} $: let us clarify what we mean by this. If f and g are two functions from $ \mathcal{H}(\mathfrak{F}, V) $, recall that the relation "there is a set $ Z \in \mathfrak{F} $ such that f and g are defined and equal on Z" is an *equivalence relation $ R_\infty $ on $ \mathcal{H}(\mathfrak{F}, V) $ (*Gen. Top.*, I, p. 66). This being so, we shall say that a relation S involving a function $ f $ of $ \mathcal{H}(\mathfrak{F}, V) $ is of *local* character (along $ \mathfrak{F} $) relative to $ f $, if it is *compatible* (in $ f $) with the equivalence relation $ R_\infty $ (*Set Theory*, II, p. 117); we know that if $ \tilde{f} $ is the *germ* of $ f $ along $ \mathfrak{F} $, the equivalence class of $ f $ modulo $ R_\infty $ (an element of the quotient set $ \mathcal{H}_\infty(\mathfrak{F}, V) = \mathcal{H}(\mathfrak{F}, V)/R_\infty $), then one can derive from S, by passage to the quotient, a relation between $ \tilde{f} $ and the other arguments of S, and that, conversely, every relation of this nature defines a relation of local character relative to $ f $.

#### Example {#fvr-v-s1-n1-exa-5 .statement}

If $ f $ and $ g $ are two functions in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $, the relation "there is an $ X \in \mathfrak{F} $ such that $ f $ and $ g $ are defined on $ X $ and $ f(t) \leq g(t) $ for every $ t \in X $" is of local character relative to $ f $ and $ g $. We denote by $ \tilde{f} \leq \tilde{g} $ the relation obtained by passing to the quotient (for $ f $ and $ g $); we remark that if $ \tilde{f} \leq \tilde{g} $ then there exist a function $ f_1 \in \tilde{f} $ and a function $ g_1 \in \tilde{g} $, defined on *all of* E, such that $ f_1(t) \leq g_1(t) $ for all $ t \in E $.

*Remarks.* 1) Let $ V_i $ ($ 1 \leq i \leq n $) be $ n $ normed vector spaces over K, and $ \varphi $ a function defined on $ V_1 \times V_2 \times \cdots \times V_n $, with values in V; by passing to the quotient along $ R_\infty $ the function $ \varphi $ defines a map from
$$
\mathcal{H}_\infty(\mathfrak{F}, V_1) \times \cdots \times \mathcal{H}_\infty(\mathfrak{F}, V_n)
$$
into $ \mathcal{H}_\infty(\mathfrak{F}, V) $, which one most often denotes by $ \varphi(\tilde{f}_1, \ldots, \tilde{f}_n) $ (*Gen. Top.*, I, p. 67). For example, taking $ \varphi $ to be the maps $ (x, y) \mapsto x + y $ and $ x \mapsto x\lambda $ ($ \lambda \in K $), one thus defines, for any two germs $ \tilde{f}, \tilde{g} $ in $ \mathcal{H}_\infty(\mathfrak{F}, V) $, the elements $ \tilde{f} + \tilde{g} $ and $ \tilde{f}\lambda $, and one verifies immediately that the rules of composition $ (\tilde{f}, \tilde{g}) \mapsto \tilde{f} + \tilde{g} $ and $ (\lambda, \tilde{f}) \mapsto \tilde{f}\lambda $ define on $ \mathcal{H}_\infty(\mathfrak{F}, V) $ a *vector space* structure over the field K; in this space $ \tilde{O} $ is the class formed by functions equal to 0 on a set in $ \mathfrak{F} $, and $ -\tilde{f} $ is the class formed by functions equal to $ -f $ on a set in $ \mathfrak{F} $. In the same way, if V is an *algebra* over K, one defines on $ \mathcal{H}_\infty(\mathfrak{F}, V) $ a second internal rule of composition $ (\tilde{f}, \tilde{g}) \mapsto \tilde{f}\tilde{g} $ by taking $ \varphi(x, y) = xy $; together with the two preceding rules this defines an *algebra* structure over K on $ \mathcal{H}_\infty(\mathfrak{F}, V) $; if V has a unit element e then $ \mathcal{H}_\infty(\mathfrak{F}, V) $ has as a unit element the class $ \tilde{e} $ formed by the functions equal to e on some set in $ \mathfrak{F} $; for $ \tilde{f} $ to be *invertible* in $ \mathcal{H}_\infty(\mathfrak{F}, V) $ it is necessary and sufficient that for some $ f \in \tilde{f} $ there exists a $ Z \in \mathfrak{F} $ such that $ f(t) $ is invertible in V for every $ t \in Z $ (in which case this condition is satisfied by every function in the class $ \tilde{f} $).

2) With the same notation, let $ \psi $ be a map of a subset of $ \prod_{i=1}^n V_i $ into V; we denote by $ \psi(f_1, f_2, \ldots, f_n) $ the function equal to $ \psi(f_1(t), f_2(t), \ldots, f_n(t)) $ at every point $ t \in E $ where the $ f_i(t) $ are defined and where the point $ (f_i(t)) $ belongs to the set where $ \psi $ is defined $ ^1 $. For example, $ f + g $ is the function equal to $ f(t) + g(t) $ at every point $ t \in E $ where $ f $ and $ g $ are both defined. Observe that the map $ (f, g) \mapsto f + g $ *is not a group law* on $ \mathcal{H}(\mathfrak{F}, V) $, since if $ f $ is not defined on all of E there is no function $ g \in \mathcal{H}(\mathfrak{F}, V) $ such that $ f + g = 0 $.

#### Definition 1 {#fvr-v-s1-def-1 .statement}

*Given two real functions* $ f, g $ *belonging to* $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $, *which are* $ \geq 0 $ *on a set in* $ \mathfrak{F} $, *we say that* $ f $ *is dominated by* $ g $, *or that* $ g $ *dominates* $ f $ *(along* $ \mathfrak{F} $*), and write* $ f \preceq g $ *or* $ g \succeq f $, *if there are a set* $ X \in \mathfrak{F} $ *and a number* $ k > 0 $ *such that* $ f(t) \leq k\ g(t) $ *for every* $ t \in X $ *(in other words, if there exists a* $ k > 0 $ *such that* $ \tilde{f} \leq k\ \tilde{g} $)

$ ^1 $ In particular, in all that follows, given a function $ f $ in $ \mathcal{H}(\mathfrak{F}, V) $ we shall denote by $ \|f\| $ the function $ t \mapsto \|f(t)\| $ which belongs to $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ and is defined on the same set as $ f $: we expressly draw attention to the fact that in this chapter $ \|f\| $ is a *function* and not a *number*.

Given two normed vector spaces $ V_1, V_2 $, and two functions $ f_1, f_2 $ belonging to $ \mathcal{H}(\mathfrak{F}, V_1) $ and $ \mathcal{H}(\mathfrak{F}, V_2) $ respectively, one says that $ f_1 $ is dominated by $ f_2 $ (along $ \mathfrak{F} $), and writes $ f_1 \preccurlyeq f_2 $ or $ f_2 \succeq f_1 $, if $ \|f_1\| \preccurlyeq \|f_2\| $.

The relation $ f_1 \preccurlyeq f_2 $ is clearly of local character in $ f_1 $ and $ f_2 $; it is thus equivalent to the relation $ \tilde{f}_1 \preccurlyeq \tilde{f}_2 $ derived by passing to the quotient. When $ f $ and $ g $ are real functions one must be careful not to confuse the relations $ \tilde{f} \preccurlyeq \tilde{g} $ and $ \tilde{f} \leq \tilde{g} $.

Note that for every scalar $ \lambda \neq 0 $ the relation $ f_1 \preccurlyeq f_2 \lambda $ is *equivalent to* $ f_1 \preccurlyeq f_2 $. If $ f_1 \preccurlyeq f_2 $ there exists a set $ X \in \mathfrak{F} $ such that $ f_1(x) = 0 $ for every point $ x \in X $ where $ f_2(x) = 0 $.

*Examples.* 1) The relation $ f \preccurlyeq 1 $ means that $ f $ is *bounded* on a set of $ \mathfrak{F} $.

2) For every function $ f $ of $ \mathcal{H}(\mathfrak{F}, V) $, and every scalar $ \lambda \neq 0 $, one has $ f \preccurlyeq f \lambda $.
3) When $ x $ tends to $ +\infty $ one has $ \sin^2 x \preccurlyeq \sin x $.
4) When $ (x, y) $ tends to $ (0, 0) $ in $ \mathbf{R}^2 $ one has
$$
xy \preccurlyeq x^2 + y^2.
$$

The following propositions are immediate consequences of def. 1:

#### Proposition 1 {#fvr-v-s1-prop-1 .statement}

*If* $ f, g, h $ *are three functions in* $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ *then the relations* $ f \preccurlyeq g $ *and* $ g \preccurlyeq h $ *imply* $ f \preccurlyeq h $.

#### Proposition 2 {#fvr-v-s1-prop-2 .statement}

*Let* $ f_1, f_2 $ *be two functions in* $ \mathcal{H}(\mathfrak{F}, V) $ *and* $ g $ *a function in* $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $. *The relations* $ f_1 \preccurlyeq g $ *and* $ f_2 \preccurlyeq g $ *imply* $ f_1 + f_2 \preccurlyeq g $.

Further:

#### Proposition 3 {#fvr-v-s1-prop-3 .statement}

*Let* $ V_1, V_2, V $ *be three normed spaces over the same valued field*, and $ (x, y) \mapsto [x.y] $ *a bilinear map from* $ V_1 \times V_2 $ *into* $ V $. *If* $ f_1 $ *and* $ f_2 $ *are functions in* $ \mathcal{H}(\mathfrak{F}, V_1) $ *and* $ \mathcal{H}(\mathfrak{F}, V_2) $ *respectively, and* $ g_1, g_2 $ *are two functions in* $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ *such that* $ f_1 \preccurlyeq g_1 $ *and* $ f_2 \preccurlyeq g_2 $ *then* $ [f_1.f_2] \preccurlyeq g_1 g_2 $.

Indeed (*Gen. Top.*, IX, p. 173, th. 1) there exists a number $ a > 0 $ such that
$$
|[f_1.f_2]| \leq a \|f_1\| \|f_2\|.
$$

#### Corollary {#fvr-v-s1-n1-cor-1 .statement}

*If* $ V $ *is a normed algebra*, *if* $ f_1, f_2 $ *are two functions in* $ \mathcal{H}(\mathfrak{F}, V) $, *and* $ g_1, g_2 $ *are two functions in* $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $, *then the relations* $ f_1 \preccurlyeq g_1, f_2 \preccurlyeq g_2 $ *imply* $ f_1 f_2 \preccurlyeq g_1 g_2 $.

The relation $ f \preccurlyeq g $ between functions in $ \mathcal{H}(\mathfrak{F}, V) $ is *transitive* by prop. 1; since it is *reflexive* the relation "*f \preccurlyeq g and g \preccurlyeq f*" is an *equivalence relation* on $ \mathcal{H}(\mathfrak{F}, V) $ (*Set Theory*, II, p. 113).

#### Definition 2 {#fvr-v-s1-def-2 .statement}

*Given two functions* $ f, g $ *of* $ \mathcal{H}(\mathfrak{F}, V) $ *we say that* $ f $ *and* $ g $ *are similar (along* $ \mathfrak{F} $), *and write* $ f \simeq g $, *if* $ f \preccurlyeq g $ *and* $ g \preccurlyeq f $.

For every scalar $ \lambda \neq 0 $ the relation $ f \simeq g $ is equivalent to $ f \simeq g \lambda $. It implies the existence of a set $ X \in \mathfrak{F} $ such that that the subset of $ X $ of points where $ f(x) = 0 $ is identical with the subset of $ X $ of points where $ g(x) = 0 $.

#### Example 1 {#fvr-v-s1-n1-exa-1 .statement}

For a real function $ f \in \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ the relation $ f \simeq 1 $ means that there are two numbers $ a > 0,\ b > 0 $ such that $ a \leq |f(x)| \leq b $ on a set in $ \mathfrak{F} $, or that the function $ \log |f| $ is bounded on a set in $ \mathfrak{F} $: one then says that $ f $ is *logarithmically bounded* on a set in $ \mathfrak{F} $.

#### Example 2 {#fvr-v-s1-n1-exa-2 .statement}

Let $ V $ be a normed space over a non-discrete valued field $ K $, and let $ f(x) = a_0 x^n + a_1 x^{n-1} + \cdots + a_n $ be a polynomial in the variable $ x \in K $, with coefficients in $ V $, such that $ a_0 \neq 0 $. For every vector $ b \neq 0 $ one has $ f(x) \simeq b x^n $ as $ |x| $ tends to $ +\infty $.

#### Example 3 {#fvr-v-s1-n1-exa-3 .statement}

We have seen that $ \sin^2 x \preccurlyeq \sin x $ as $ x $ tends to $ +\infty $, but *we do not have* $ \sin^2 x \simeq \sin x $, even though these functions vanish at the same points.

#### Example 4 {#fvr-v-s1-n1-exa-4 .statement}

One has $ x^2 + xy + y^2 \simeq x^2 + y^2 $ when $ (x,\ y) $ tends to $ (0,\ 0) $ in $ \mathbf{R}^2 $, but *not* $ xy \simeq x^2 + y^2 $.

It follows immediately from prop. 3 of V, p. 213, that if $ f_1,\ f_2,\ g_1,\ g_2 $ are functions in $ \mathcal{H}(\mathfrak{F}, K) $ ($ K $ being any valued field) the relations $ f_1 \simeq g_1 $ and $ f_2 \simeq g_2 $ imply that $ f_1 f_2 \simeq g_1 g_2 $.

We remark that in contrast the relations $ f_1 \simeq g_1 $ and $ f_2 \simeq g_2 $ *do not imply that* $ f_1 + f_2 \simeq g_1 + g_2 $, as is shown by the example $ f_1(x) = g_1(x) = x^2,\ f_2(x) = -(x^2 + x),\ g_2(x) = -(x^2 - 1) $, as the real variable $ x $ tends to $ +\infty $.

The comparison relations $ f \preccurlyeq g,\ f \simeq g $ are said to be *weak*. We say that two functions $ f,\ g $ from $ \mathcal{H}(\mathfrak{F}, V) $ are *weakly comparable* if they satisfy one (at least) of the relations $ f \preccurlyeq g,\ g \preccurlyeq f $.

#### Remark 1 {#fvr-v-s1-n1-rem-1 .statement}

Two functions in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ need not be weakly comparable, as is shown by the example of the functions 1 and $ x \sin x $ as $ x $ tends to $ +\infty $.

#### Remark 2 {#fvr-v-s1-n1-rem-2 .statement}

Denote by $ R_0 $ the relation $ f \simeq g $ on $ \mathcal{H}(\mathfrak{F}, V) $, and by $ \mathcal{H}_0(\mathfrak{F}, V) $ the quotient set $ \mathcal{H}(\mathfrak{F}, V)/R_0 $; note that the relation $ R $ *implies* $ R_0 $. Passing to the quotient the relation $ f \preccurlyeq g $ gives, by prop. 1 of V, p. 213, an *order relation* on $ \mathcal{H}_0(\mathfrak{F}, V) $ (*Set Theory*, III, p. 134); the preceding example shows that $ \mathcal{H}_0(\mathfrak{F}, V) $ *is not totally ordered* by this relation.

### 2. COMPARISON RELATIONS: II. STRONG RELATIONS

#### Definition 3 {#fvr-v-s1-def-3 .statement}

*Given two real functions* $ f,\ g $ *belonging to* $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $, *which are* $ \geq 0 $ *on a set in* $ \mathfrak{F} $, *one says that* $ f $ *is negligible relative to* $ g $, *or that* $ g $ *is preponderant over* $ f $ *(along* $ \mathfrak{F} $), *and one writes* $ f \ll g $ *or* $ g \gg f $ *if, for every* $ \varepsilon > 0 $, *there exists a set* $ X \in \mathfrak{F} $ *such that* $ f(t) \leq \varepsilon g(t) $ *for every* $ t \in X $.

*Given two normed spaces* $ V_1,\ V_2 $ *and two functions* $ f_1,\ f_2 $ *belonging to* $ \mathcal{H}(\mathfrak{F}, V_1) $ *and* $ \mathcal{H}(\mathfrak{F}, V_2) $ *respectively, one says that* $ f_1 $ *is negligible relative to* $ f_2 $ *(along* $ \mathfrak{F} $), *and one writes* $ f_1 \ll f_2 $ *or* $ f_2 \gg f_1 $, *if* $ \|f_1\| \ll \|f_2\| $.

For every scalar $ \lambda \neq 0 $ the relation $ f_1 \ll f_2 \lambda $ is *equivalent* to $ f_1 \ll f_2 $. The relation $ f_1 \ll f_2 $ implies $ f_1 \preccurlyeq f_2 $ but is not equivalent to it.

Note that the relation $ f_1 \preccurlyeq f_2 $ by no means implies the relation "f_1 \ll f_2 \text{ or } f_1 \asymp f_2 \text{": one has } \sin x \preccurlyeq 1 \text{ as } x \text{ tends to } +\infty, \text{ but neither of the relations } \sin x \ll 1 \text{ or } \sin x \asymp 1 \text{ is true.}"

*Examples.* 1) The relation $ f \ll 1 $ means that $ f $ *tends to 0 along $ \mathfrak{F} $*.

2) When $ \alpha $ and $ \beta $ are two real numbers such that $ \alpha < \beta $ one has $ x^\alpha \ll x^\beta $ as $ x $ tends to $ +\infty $. Similarly, when $ m $ and $ n $ are two rational integers such that $ m < n $ one has $ z^m \ll z^n $ as the complex number $ z $ tends to $ \infty $.

3) As $ x $ tends to $ +\infty $ one has $ x^n \ll e^x $ for every integer $ n $ (III, p. 105).

4) In $ \mathbf{R}^2 $ one has, as $ (x, y) $ tends to $ (0, 0) $,
$$
x^2 + y^2 \ll |x| + |y|.
$$

The following propositions can be deduced immediately from def. 3:

#### Proposition 4 {#fvr-v-s1-prop-4 .statement}

*If $ f, g, h $ are three functions in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ then the relations $ f \preccurlyeq g $ and $ g \ll h $ (resp. $ f \ll g $ and $ g \preccurlyeq h $) imply $ f \ll h $.*

#### Proposition 5 {#fvr-v-s1-prop-5 .statement}

*Let $ f_1, f_2 $ be two functions in $ \mathcal{H}(\mathfrak{F}, V) $ and $ g $ a function in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $. Then the relations $ f_1 \ll g $ and $ f_2 \ll g $ imply $ f_1 + f_2 \ll g $.*

Moreover, the same argument as in prop. 3 of V, p. 213 shows that:

#### Proposition 6 {#fvr-v-s1-prop-6 .statement}

*With the notation of prop. 3, the relations $ f_1 \ll g_1 $ and $ f_2 \preccurlyeq g_2 $ (resp. $ f_1 \preccurlyeq g_1 $ and $ f_2 \ll g_2 $) imply $ [f_1.f_2] \ll g_1g_2 $.*

Prop. 4 shows that the relation $ f \ll g $ between functions in $ \mathcal{H}(\mathfrak{F}, V) $ is *transitive*; but *it is not reflexive*: to be precise, the relation $ f \ll f $ implies that $ f $ *vanishes on a set in $ \mathfrak{F} $* (in other words, $ f $ is equivalent to 0 modulo $ R_\infty $); indeed, for an $ \varepsilon $ such that $ 0 < \varepsilon < 1 $ there exists an $ X \in \mathfrak{F} $ such that $ \|f(x)\| \leq \varepsilon \|f(x)\| $ for every $ x \in X $, which is possible only if $ f(x) = 0 $ for every $ x \in X $. It follows that the relation "f \ll g and g \ll f" is transitive and symmetric, but not reflexive: so it is not an equivalence relation (it implies that there is a set $ X \in \mathfrak{F} $ such that $ f(x) = g(x) = 0 $ for every $ x \in X $).

#### Proposition 7 {#fvr-v-s1-prop-7 .statement}

*If $ f $ and $ g $ are two functions in $ \mathcal{H}(\mathfrak{F}, V) $ then the relation $ f - g \ll f $ is equivalent to $ f - g \ll g $.*

Indeed, $ f - g \ll f $ implies that for every $ \varepsilon > 0 $ there exists an $ X \in \mathfrak{F} $ such that $ \|f(x) - g(x)\| \leq \varepsilon \|f(x)\| $ for every $ x \in X $. But then $ (1 - \varepsilon) \|f(x)\| \leq \|g(x)\| $, and consequently $ f \preccurlyeq g $, whence (V, p. 215, prop. 4) $ f - g \ll g $.

#### Corollary {#fvr-v-s1-n2-cor-1 .statement}

*The relation $ f - g \ll f $ is an equivalence relation on $ \mathcal{H}(\mathfrak{F}, V) $.*

Indeed, if $ f - g \ll f $ and $ g - h \ll g $ then $ f - g \ll g $, whence (V, p. 215, prop. 5) $ f - h \ll g $, and consequently, since $ g \preceq f $, we have $ f - h \ll f $, which shows that this relation is transitive; it is symmetric by prop. 7, and is clearly reflexive, whence the corollary.

#### Definition 4 {#fvr-v-s1-def-4 .statement}

*Given two functions* $ f, g $ *of* $ \mathcal{H}(\mathfrak{F}, V) $ *one says that* $ f $ *and* $ g $ *are equivalent (along* $ \mathfrak{F} $), *and writes* $ f \sim g $, *if* $ f - g \ll f $.

The relation $ f \sim g $ implies $ f \asymp g $ but is not equivalent to it.

#### Example 1 {#fvr-v-s1-n2-exa-1 .statement}

If $ a $ is a constant function, $ \neq 0 $ on $ E $, the relation $ f \sim a $ means that $ f $ *tends to* $ a $ *along* $ \mathfrak{F} $.

#### Example 2 {#fvr-v-s1-n2-exa-2 .statement}

Let $ V $ be a normed space over a non-discrete valued field $ K $, and let $ f(x) = a_0 x^n + a_1 x^{n-1} + \cdots + a_n $ be a polynomial in the variable $ x \in K $, with coefficients in $ V $, such that $ a_0 \neq 0 $. Then $ f(x) \sim a_0 x^n $ as $ |x| $ tends to $ +\infty $.

#### Example 3 {#fvr-v-s1-n2-exa-3 .statement}

When the real number $ x $ tends to $ +\infty $ one has $ \left( 1 + \frac{1}{x} \right) \sin x \sim \sin x $.

#### Example 4 {#fvr-v-s1-n2-exa-4 .statement}

As the complex variable $ z $ tends to 0 one has $ e^z - 1 \sim z $. More generally, if $ V $ is a normed space over a valued field $ K $, and $ f $ is a function defined on a neighbourhood of $ x_0 \in K $, with values in $ V $, and admitting a derivative $ f'(x_0) \neq 0 $ at the point $ x_0 $, then, as $ x $ approaches $ x_0 $, we have $ f(x) - f(x_0) \sim f'(x_0)(x - x_0) $ (I, p. 3, def. 1).

#### Example 5 {#fvr-v-s1-n2-exa-5 .statement}

As $ (x, y) $ approaches $ (0, 0) $ in $ \mathbf{R}^2 $ one has
$$
\sqrt{\sin^2 x + \sin^2 y} \sim \sqrt{x^2 + y^2}.
$$

#### Example 6 {#fvr-v-s1-n2-exa-6 .statement}

Let $ f(x, y) $ be a polynomial with real coefficients in two real variables $ x, y $, not having a constant term. If, as $ x $ approaches 0 while remaining $ > 0 $, there is a function $ \varphi(x) $, continuous on an interval $ [0, a] $, and such that $ \varphi(0) = 0 $ and $ f(x, \varphi(x)) = 0 $ for $ 0 \leq x \leq a $, one can show that there are a rational number $ r $ and a real number $ \lambda \neq 0 $ such that $ \varphi(x) \sim \lambda x^r $ (V, p. 259, exerc. 3).

#### Example 7 {#fvr-v-s1-n2-exa-7 .statement}

For every $ x > 0 $ let $ \pi(x) $ denote the number of prime numbers which are $ \leq x $; it has been proved that $ \pi(x) \sim x / \log x $ $ ^2 $ as $ x $ tends to $ +\infty $.

#### Remark {#fvr-v-s1-n2-rem-3 .statement}

Note that the relation $ f \sim g $ by no means implies that the difference $ f - g $ tends to 0 along $ \mathfrak{F} $; this difference can even be *unbounded*, as is shown by the example $ x^2 + x \sim x^2 $ as $ x $ tends to $ +\infty $.

#### Proposition 8 {#fvr-v-s1-prop-8 .statement}

*Let* $ K $ *be a valued field and* $ f_1, f_2, g_1, g_2 $ *four functions in* $ \mathcal{H}(\mathfrak{F}, K) $; *then the relations* $ f_1 \sim g_1 $ *and* $ f_2 \sim g_2 $ *imply* $ f_1 f_2 \sim g_1 g_2 $.

Indeed, we have $ f_1 f_2 - g_1 g_2 = f_1 (f_2 - g_2) + (f_1 - g_1) g_2 $; since $ f_1 \preceq g_1 $, $ f_1 - g_1 \ll g_1 $ and $ f_2 - g_2 \ll g_2 $, we have $ f_1 f_2 - g_1 g_2 \ll g_1 g_2 $ (V, p. 215, prop. 5 and 6).

In contrast, we have given an example in V, p. 214 where one has $ f_1 = g_1 $, $ f_2 \sim g_2 $ and yet the relation $ f_1 + f_2 \asymp g_1 + g_2 $ does not hold (so neither *a fortiori* does
$$
f_1 + f_2 \sim g_1 + g_2).
$$
2 See, for example, A. E. INGHAM, *The distribution of prime numbers* (Cambridge Tracts, n 30), Cambridge University Press, 1932.

The comparison relations $ f \ll g, f \sim g $ are called strong relations. Two functions $ f, g $ from $ \mathcal{H}(\mathfrak{F}, V) $ are called comparable (or strongly comparable when one wants to avoid any possible confusion) if they satisfy one of the three relations: $ f \ll g, f \gg g $, or "there exists a $ \lambda \neq 0 $ such that $ f \sim g\lambda $".

#### Remark 1 {#fvr-v-s1-n2-rem-1 .statement}

Two functions can be weakly comparable though not strongly comparable, for example the functions 1 and $ \sin x $ as $ x $ tends to $ +\infty $.

#### Remark 2 {#fvr-v-s1-n2-rem-2 .statement}

In the definitions of the comparison relations $ f_1 \preccurlyeq f_2 $ and $ f_1 \ll f_2 $ the norms on the spaces $ V_1, V_2 $ where $ f_1 $ and $ f_2 $ respectively take their values, are involved only apparently; in reality only the topologies on $ V_1 $ and $ V_2 $ are involved, for the relations $ f_1 \preccurlyeq f_2 $ and $ f_1 \ll f_2 $ are replaced by equivalent relations when one replaces the norm on $ V_1 $ or $ V_2 $ by an equivalent norm (\emph{Gen. Top.}, IX, p. 170, def. 7).

### 3. CHANGE OF VARIABLE

Let $ \varphi $ be a map from the set $ E' $ into $ E $ such that $ \varphi^{-1}(\mathfrak{F}) $ is a filter base on $ E' $. It is clear that if $ f_1, f_2 $ are functions in $ \mathcal{H}(\mathfrak{F}, V_1) $ and $ \mathcal{H}(\mathfrak{F}, V_2) $ respectively, then $ f_1 \circ \varphi, f_2 \circ \varphi $ belong to $ \mathcal{H}(\varphi^{-1}(\mathfrak{F}), V_1) $ and $ \mathcal{H}(\varphi^{-1}(\mathfrak{F}), V_2) $ respectively, and that the relation $ f_1 \preccurlyeq f_2 $ (resp. $ f_1 \ll f_2 $) is equivalent to $ f_1 \circ \varphi \preccurlyeq f_2 \circ \varphi $ (resp. $ f_1 \circ \varphi \ll f_2 \circ \varphi $).

### 4. COMPARISON RELATIONS BETWEEN STRICTLY POSITIVE FUNCTIONS

Let $ g $ be a function in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ which is strictly positive on a set in $ \mathfrak{F} $. Comparison relations featuring $ g $ can be formulated in another way: the relation $ f \preccurlyeq g $ is equivalent to saying that $ \|f\|/g $ (which is defined on a set in $ \mathfrak{F} $) is bounded on a set in $ \mathfrak{F} $; the relation $ f \ll g $ is equivalent to saying that $ \|f\|/g $ tends to 0 along $ \mathfrak{F} $. If $ f $ is a function in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ the relation $ f \asymp g $ means that $ f/g $ is logarithmically bounded on a set in $ \mathfrak{F} $, and the relation $ f \sim g $ that $ f/g $ tends to 1 along $ \mathfrak{F} $. If $ f $ is a function in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ and positive on a set in $ \mathfrak{F} $, to say that $ f $ and $ g $ are comparable implies that $ f/g $ tends to a limit (finite or equal to $ +\infty $) along $ \mathfrak{F} $.

#### Proposition 9 {#fvr-v-s1-prop-9 .statement}

Let $ f $ and $ g $ be two functions in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $, strictly positive on a set in $ \mathfrak{F} $. For $ f $ and $ g $ to be comparable it is necessary and sufficient that for every number $ t \geqslant 0 $, with at most one exception, the function $ f - tg $ has constant sign $ ^3 $ on a set in $ \mathfrak{F} $.

The condition is necessary. Indeed, if $ f \ll g $ one has $ f - tg \sim -tg $ except for $ t = 0 $, so $ f - tg $ is strictly negative on a set in $ \mathfrak{F} $, except for $ t = 0 $; if $ f \gg g $ then $ f - tg $ is strictly positive on a set in $ \mathfrak{F} $ for all $ t $; finally, if $ f \sim kg $ ($ k $ constant $ > 0 $), then $ f - t g \sim (k - t)g $ except for $ t = k $, so, except perhaps for $ t = k $, $ f - t g $ has the sign of $ k - t $ on a set in $ \mathfrak{F} $.

The condition is sufficient. Indeed, suppose that the ratio $ f/g $ has two distinct cluster points $ \alpha < \beta $ along $ \mathfrak{F} $. For *every* number $ t $ such that $ \alpha < t < \beta $ there then exist in *every* set $ X \in \mathfrak{F} $ two points $ x_1, x_2 $ such that $ f(x_1)/g(x_1) < t $ and $ f(x_2)/g(x_2) > t $; thus $ f(x) - t g(x) $ does not have constant sign on $ X $; we have arrived at a conclusion incompatible with the hypothesis. It follows that $ f/g $ can have *only one* cluster value (finite or infinite) along the filter with base $ \mathfrak{F} $, and consequently, (*Gen. Top.*, I, p. 85, corollary) has this value as its *limit* along $ \mathfrak{F} $.

#### Proposition 10 {#fvr-v-s1-prop-10 .statement}

*Let $ f $ and $ g $ be two functions in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ which are strictly positive on a set in $ \mathfrak{F} $; for every $ \alpha $ real and $ \neq 0 $ the relation $ f \asymp g $ (resp. $ f \sim g $) is equivalent to $ f^\alpha \asymp g^\alpha $ (resp. $ f^\alpha \sim g^\alpha $); if $ \alpha > 0 $ the relation $ f \preccurlyeq g $ (resp. $ f \ll g $) is equivalent to $ f^\alpha \preccurlyeq g^\alpha $ (resp. $ f^\alpha \ll g^\alpha $); if $ \alpha < 0 $ it is equivalent to $ f^\alpha \succcurlyeq g^\alpha $ (resp. $ f^\alpha \succ g^\alpha $).*

The proofs are immediate.

One notes that in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ the set $ I' $ of functions strictly positive on a set in $ \mathfrak{F} $ is such that $ \Gamma/\mathbf{R}_\infty $ is a *multiplicative group* $ \Gamma_\infty $ in $ \mathcal{H}_\infty(\mathfrak{F}, \mathbf{R}) $; $ \Gamma/\mathbf{R}_0 $ is identical to the quotient group of $ \Gamma_\infty $ by the subgroup of classes (mod. $ \mathbf{R}_\infty $) of logarithmically bounded functions in $ \Gamma $; on $ \Gamma/\mathbf{R}_0 $ the order relation deduced from the relation $ f \preccurlyeq g $ by passage to the quotient is *compatible* with the group structure of $ \Gamma/\mathbf{R}_0 $ and thus makes it an ordered group.

#### Proposition 11 {#fvr-v-s1-prop-11 .statement}

*Let $ g $ be a function in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ such that $ \lim_{\mathfrak{F}} g = +\infty $; the relation $ f \ll g $ implies $ e^f \ll e^g $; the relation $ f \sim g $ implies $ \log f \sim \log g $.*

Indeed, if $ f \ll g $ then $ f - g = g \left( \frac{f}{g} - 1 \right) $ tends to $ -\infty $ along $ \mathfrak{F} $. Similarly, if $ f \sim g $ one has $ \log f = \log g + \log \frac{f}{g} $, so $ \log f - \log g $ tends to 0, and the same for $ \frac{\log f}{\log g} - 1 = \frac{\log f - \log g}{\log g} $.

On the other hand, note that the relation $ f \sim g $ *does not imply* $ e^f \sim e^g $, nor even that $ e^f \asymp e^g $, as is shown by the example where $ f(x) = x^2, \ g(x) = x^3 + x $ as $ x $ tends to $ +\infty $; similarly, the relation $ f \ll g $ *does not imply* $ \log f \ll \log g $, as is shown by the example $ f(x) = x, \ g(x) = x^2 $ as $ x $ tends to $ +\infty $.

#### Definition 5 {#fvr-v-s1-def-5 .statement}

*Let $ g $ be a function in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $, strictly positive on a set in $ \mathfrak{F} $, and such that $ \lim_{\mathfrak{F}} g = 0 $ or $ \lim_{\mathfrak{F}} g = +\infty $. One says that a function $ f \in \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ is of order $ \rho $ (finite or infinite) relative to $ g $ if $ \lim_{\mathfrak{F}} \log(|f|)/\log g = \rho $.*

Note that if $ f $ is of order $ \rho $ relative to $ g $ then $ f $ is of order $ -\rho $ relative to $ 1/g $; one therefore need treat only the case where $ g(x) $ tends to $ +\infty $ along $ \mathfrak{F} $.

#### Proposition 12 {#fvr-v-s1-prop-12 .statement}

Let g be a function in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ such that $ \lim_{\mathfrak{F}} g = +\infty $; let f be a function in $ \mathcal{H}(\mathfrak{F}, \mathbf{R}) $.

a) For f to be of order $ +\infty $ relative to g it is necessary and sufficient that $ f \gg g^\alpha $ for every $ \alpha \geq 0 $.

b) For f to be of order $ -\infty $ relative to g it is necessary and sufficient that $ f \ll g^{-\alpha} $ for every $ \alpha > 0 $.

c) For f to be of finite order equal to $ \rho $ relative to g it is necessary and sufficient that, for every $ \varepsilon > 0 $, one has $ g^{\rho-\varepsilon} \ll f \ll g^{\rho+\varepsilon} $.

Let us prove c) for example. If the order of f relative to g is $ \rho $ then for every $ \varepsilon > 0 $ there exists a set $ M \in \mathfrak{F} $ such that, for every $ x \in M $, we have

$$
\left( \rho - \frac{\varepsilon}{2} \right) \log g(x) \leq \log |f(x)| \leq \left( \rho + \frac{\varepsilon}{2} \right) \log g(x),
$$

or $ (g(x))^{\rho - \frac{\varepsilon}{2}} \leq |f(x)| \leq (g(x))^{\rho + \frac{\varepsilon}{2}} $; since $ \lim_{\mathfrak{F}} g = +\infty $ one thus has $ g^{\rho-\varepsilon} \ll f \ll g^{\rho+\varepsilon} $ for every $ \varepsilon > 0 $; the converse is immediate. The proofs of a) and b) are similar.

Note that if f is of finite order $ \rho $ relative to g then $ fg^{-\rho} $ is of order 0 relative to g, and conversely; if $ f_1 $ (resp. $ f_2 $) is of order $ \rho_1 $ (resp. $ \rho_2 $) relative to g, and if $ \rho_1 + \rho_2 $ is defined, then $ f_1 f_2 $ is of order $ \rho_1 + \rho_2 $ relative to g.

#### Remark 1 {#fvr-v-s1-n4-rem-1 .statement}

Observe that though f may be of finite order $ \rho $ relative to g nevertheless the ratio $ f/g^\rho $ need not tend to a limit; for example, every logarithmically bounded function is of order 0 relative to g, but need not have a limit along $ \mathfrak{F} $.

#### Remark 2 {#fvr-v-s1-n4-rem-2 .statement}

A function defined on a set in $ \mathfrak{F} $ need not have a determinate order (finite or not) relative to g, for the functions having a determinate order relative to g are comparable to all the powers of g with at most one exception. Now f need not have this property, as one sees from the example $ g(x) = x,\ f(x) = 1 + x^2 \sin^2 x $ (as x tends to $ +\infty $). In this example f is comparable to $ g^\alpha $ for $ \alpha < 0 $ and $ \alpha > 2 $; if one takes $ f(x) = e^x \sin^2 x + e^{-x} \cos^2 x $ then f is not comparable to any power (positive or negative) of g.

### 5. NOTATION

Given a real function $ f \in \mathcal{H}(\mathfrak{F}, \mathbf{R}) $ it is often convenient in a formula to write $ O(f) $ for a function dominated by f, and $ o(f) $ for a negligible function relative to f. When, in a proof, there feature several functions dominated by the same function f (resp. negligible relative to f) we denote them by $ O_1(f),\ O_2(f) $, etc. (resp. $ o_1(f),\ o_2(f) $, etc.).

Many authors write $ O(f) $ (resp. $ o(f) $) indiscriminately for all functions in a proof that are dominated by f (resp. negligible relative to f), an abuse of language which may risk confusion.

With this notation we can express props. 1, 2, 3 (V, p. 213) as follows: if $ g = O_1(f) $ and $ h = O(g) $ then $ h = O_2(f) $; one can write

$$
\sum_{i=1}^{n} \lambda_i O_i(f) = O_{n+1}(f) \quad (\lambda_i \text{ scalars}) \tag{1}
$$
$$
O(f) \, O(g) = O(fg). \tag{2}
$$

Similarly, prop. 4 (V, p. 215) shows that if $ g = O_1(f) $ and $ h = o(g) $ (resp. $ g = o_1(f) $ and $ h = O(g) $) then $ h = o_2(f) $, and props. 5 and 6 (V, p. 5) can be expressed in the form
$$
\sum_{i=1}^{n} \lambda_i o_i(f) = o_{n+1}(f) \quad (\lambda_i \text{ scalars}) \tag{3}
$$
$$
o(f) \, O(g) = o(fg). \tag{4}
$$

The relation $ f \sim g $ is equivalent to $ f = g + o(g) $. The notation $ O(1) $ (resp. $ o(1) $) denotes a function bounded on a set in $ \mathfrak{F} $ (resp. a function tending to 0 along $ \mathfrak{F} $).

### Exercises {#fvr-v-s1-exercises}

See the [exercises for § 1](exercises/s1/).
