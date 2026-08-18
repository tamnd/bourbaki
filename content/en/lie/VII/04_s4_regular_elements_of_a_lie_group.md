---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 4
section_title: Regular elements of a Lie group
lang: en
source: lie-vii-ix
book_pages: 27-34, 63
pdf_pages: 0037-0044, 0072-0072
extraction: native
subsections:
    - "no": 1
      title: REGULAR ELEMENTS FOR A LINEAR REPRESENTATION
      page: 27
      pdf_page: 37
    - "no": 2
      title: REGULAR ELEMENTS OF A LIE GROUP
      page: 29
      pdf_page: 39
    - "no": 3
      title: RELATIONS WITH REGULAR ELEMENTS OF THE LIE ALGEBRA
      page: 31
      pdf_page: 41
    - "no": 4
      title: APPLICATION TO ELEMENTARY AUTOMORPHISMS
      page: 34
      pdf_page: 44
statements: 18
exercises: 4
content_sha256: 9d1010f2a4312da7eb256b0b49777e2e7c13fd2cda13efe8e747d4ded4fee400
---

## § 4. REGULAR ELEMENTS OF A LIE GROUP

In nos. 1, 2 and 3 of this paragraph, we assume that $k$ is $\mathbf{R},\mathbf{C}$ or a non-discrete complete ultrametric field of characteristic 0. We denote by G a finite dimensional Lie group over $k$, by $\mathfrak{g}$ its Lie algebra, and by $e$ its identity element. If $a\in G$, we denote by $\mathfrak{g}^1(a)$ the nilspace of Ad $(a)-1$, in other words the space $\mathfrak{g}^1$(Ad($a$)) (cf. §1, no. 1).

### 1. REGULAR ELEMENTS FOR A LINEAR REPRESENTATION

#### Lemma 1 {#lie-vii-s4-lem-1 .statement tag=00VU}

Let M be an analytic manifold over $k$ and $a= (a_0, . . . , a_{n-1}, a_n= 1)$ a sequence of analytic functions on M. For all $x\in M$, let $r_a(x)$ be the upper bound of those $i\in 0, n$ such that $a_j(x) = 0$ for $j < i$ and let $r_a^0(x)$ be the upper bound of those $i\in 0, n$ such that $a_j$ is zero on a neighbourhood of $x$ for $j < i$.

(i) The function $r_a$ is upper semi-continuous.

(ii) For all $x\in M,r_a^0(x) =$ lim inf$_{y\rightarrow x}r_a(y)$.

(iii) The function $r_a^0$ is locally constant.

(iv) The set of points $x\in M$ such that $r^0_a(x) =r_a(x)$ is the set of points of M on a neighbourhood of which $r_a$ is constant. This is a dense open subset of M. If $k=\mathbf{C}$ and M is finite dimensional and connected, it is open and connected.

(i) If $r_a(x) =i$, then $a_i(x)\not= 0$ and, for all $y$ in a neighbourhood of $x$, we have $a_i(y)\not= 0$, so $r_a(y)\leq i$.

(ii) If $r^0_a(x) =i$, the functions $a_0, . . . , a_{i-1}$ are zero on a neighbourhood of $x$ and, for any $y$ in this neighbourhood, $r_a(y)\geq i$. Consequently, lim inf$_{y\rightarrow x}r_a(y)\geq i$. Every neighbourhood of $x$ contains a point $y$ such that $a_i(y)\not= 0$ and hence $r_a(y)\leq i$. Thus lim inf$_{y\rightarrow x}r_a(y) =i$.

(iii) Let $i=r_a^0(x)$ and let V be a neighbourhood of $x$ such that $a_j(y) = 0$ for all $y\in V$ and all $j < i$. Then $x\in M$**--** Z, where Z denotes the set of points of M in a neighbourhood of which the function $a_i$ is zero. Since Z is closed in M (Differentiable and Analytic Manifolds, Results$, 5.3.5), V\cap (M$ **--** Z) is a neighbourhood of $x$. For every point $y$ in this neighbourhood, $r_a^0(y) =i$.

(iv) The function $r_a-r_a^0$ is upper semi-continuous and its value at any point is $\geq 0$. If $r_a(x) =r^0_a(x),r_a-r^0_a$ is zero on a neighbourhood of $x$, which shows that $r_a$ is constant on a neighbourhood of $x$ by (iii). Conversely, if $r_a$ is constant on a neighbourhood of $x$, then $r_a^0(x) =r_a(x)$ by (ii). The set of points $x\in M$ such that $r_a^0(x) =r_a(x)$ is thus an open subset $\Omega$ of M. If $x\in M$ and if $r^0_a(x)< r_a(x)$, every neighbourhood of $x$ contains a point $y$ such that $r_a(y)< r_a(x)$ and $r^0_a(y) =r_a^0(x)$. Every neighbourhood of $x$ thus contains a point $y$ such that

$$
r_a(y)-r^0_a(y)< r_a(x)-r^0_a(x)
$$

It follows that $\Omega$ is dense in M.

If M is connected and if $p$ is the value of $r_a^0$ on M, the points of $\Omega$ are the points $x\in M$ such that $a_p(x)\not= 0$. If $k=\mathbf{C}$, this implies that $\Omega$ is connected by Lemma 3 of Appendix II.

Let $\rho$ be an analytic linear representation of G on a vector space V of finite dimension $n$ over $k$. Put

det(T $-\rho (g) + 1) =a_0(g) +a_1(g)T +\cdots +a_{n-1}(g)T^{n-1}+ T^n$.

The functions $r_a$ and $r_a^0$ associated to the sequence $(a_0, a_1, . . . , a_{n-1},1)$ will be denoted by $r_{\rho}$ and $r^0_{\rho}$, respectively. Then, for all $g\in G$,

$r_{\rho}(g) =$ dim $V^1(\rho (g))$

$r_{\rho}^0(g) =$ lim inf$_{g'\rightarrow g}$ dim $V^1(\rho (g'))$.

#### Lemma 2 {#lie-vii-s4-lem-2 .statement tag=00VV}

Let $0\rightarrow V'\rightarrow V\rightarrow V''\rightarrow 0$ be an exact sequence of G-modules defined by analytic linear representations $\rho ', \rho , \rho ''$ of G, respectively. Then:

$r_{\rho}=r_{\rho'}+r_{\rho''}$, and $r^0_{\rho}=r^0_{\rho'}+r^0_{\rho''}$.

Indeed, for all $g\in G$, there is (§1, no. 1, Cor. 3 of Th.1 ) an exact sequence

$$
0\rightarrow (V')^1(\rho '(g))\rightarrow V^1(\rho (g))\rightarrow (V'')^1(\rho ''(g))\rightarrow 0
$$

which proves the first assertion. The second follows from it since, by Lemma 1 (iv), $r^0_{\rho}=r_{\rho}, r^0_{\rho'}=r_{\rho'}$ and $r_{\rho''}^0=r_{\rho''}$ on a dense open subset of G.

#### Definition 1 {#lie-vii-s4-def-1 .statement tag=00VW}

An element $g\in G$ is called regular for the linear representation $\rho$ if $r_{\rho}(g) =r^0_{\rho}(g)$.

#### Proposition 1 {#lie-vii-s4-prop-1 .statement tag=00VX}

The regular points for an analytic linear representation $\rho$ of G are the points of G in a neighbourhood of which $r_{\rho}$ is constant. They constitute a dense open subset of G. If $k=\mathbf{C}$ and G is connected, the set of regular points for $\rho$ is connected.

This follows from Lemma 1 (iv).

#### Remark {#lie-vii-s4-n1-rem-1 .statement tag=00VY}

Let $G^*$ be an open subgroup of G. An element $a\in G^*$ is a regular element of G for the linear representation $\rho$ of G if and only if it is a regular element of $G^*$ for the linear representation $\rho |G^*$.

### 2. REGULAR ELEMENTS OF A LIE GROUP

#### Definition 2 {#lie-vii-s4-def-2 .statement tag=00VZ}

An element of G is said to be regular if it is regular for the adjoint representation of G.

In other words (Prop. 1), an element $g\in G$ is regular if, for all elements $g'$ in a neighbourhood of $g$ in G, the dimension of the nilspace of Ad($g'$)$-1$ is equal to the dimension of the nilspace of Ad($g$)$-1$.

#### Proposition 2 {#lie-vii-s4-prop-2 .statement tag=00W0}

Let $G'$ be a finite dimensional Lie group over $k$ and $f$ an open morphism from G to $G'$. The image under $f$ of a regular element of G is a regular element of $G'$. If the kernel of $f$ is contained in the centre of G, an element $g\in G$ is regular if and only if $f(g)$ is regular.

Indeed, let $\mathfrak{g}'$ be the Lie algebra of $G'$ and $\mathfrak{h}$ the ideal in $\mathfrak{g}$ given by the kernel of $Tf|\mathfrak{g}$. Let $\rho$ be the linear representation of G on $\mathfrak{h}$ defined by $\rho (g) =$ Ad $g|\mathfrak{h}$ for all $g\in G$, and let Ad $\circ f$ be the linear representation of G on $\mathfrak{g}'$ given by the composite of $f$ with the adjoint representation of $G'$. These linear representations define an exact sequence of G-modules:

$$
0\rightarrow \mathfrak{h}\rightarrow \mathfrak{g}\rightarrow \mathfrak{g}'\rightarrow 0
$$

By Lemma $2,r_{Ad}=r_{\rho}+r_{Ad\circ f}$. Since $r_{Ad\circ f}=r_{Ad}\circ f$ and since $f$ is an open map, $r_{Ad\circ f}^0=r_{Ad}^0\circ f$. Consequently:

$$
r_{Ad}-r^0_{Ad}=r_{\rho}-r_{\rho}^0+ (r_{Ad}-r_{Ad}^0)\circ f
$$

Thus, if $g$ is regular, $(r_{Ad}-r^0_{Ad})(f(g)) = 0$, which means that $f(g)$ is regular. If the kernel of $f$ is contained in the centre of G,

$r_{\rho}(g) =r_{\rho}^0(g) =$ dim$\mathfrak{h}$ for all $g\in G$. Consequently, if $f(g)$ is regular, $r_{Ad}(g) =r_{Ad}^0(g)$, in other words, $g$ is regular.

#### Proposition 3 {#lie-vii-s4-prop-3 .statement tag=00W1}

Let $G_1$ and $G_2$ be two finite dimensional Lie groups over $k$. An element $(g_1, g_2)$ of $G_1\times G_2$ is regular if and only if $g_1$ and $g_2$ are regular elements of $G_1$ and $G_2$, respectively.

The condition is necessary by Prop. 2. We show that it is sufficient. For all $g= (g_1, g_2)\in G_1\times G_2,r_{Ad}(g) =r_{Ad}(g_1) +r_{Ad}(g_2)$. In view of Lemma 1 (ii), it follows that $r^0_{Ad}(g) =r^0_{Ad}(g_1) +r_{Ad}^0(g_2)$. If $g_1$ and $g_2$ are regular, $r^0_{Ad}(g_1) =$ $r_{Ad}(g_1)$ and $r^0_{Ad}(g_2) =r_{Ad}(g_2)$, so $r^0_{Ad}(g) =r_{Ad}(g)$, which means that $g$ is regular.

#### Lemma 3 {#lie-vii-s4-lem-3 .statement tag=00W2}

Let $a\in G$ and let $\mathfrak{m}$ be a complement of $\mathfrak{g}^1(a)$ in $\mathfrak{g}$. Let U be a neighbourhood of 0 in $\mathfrak{g}$ and exp an exponential map from U to G. The map

$f: (x, y) \rightarrow$ (exp $y)a$(exp $x$)(exp $y)^{-1}$

from $(\mathfrak{g}^1(a)\times \mathfrak{m})\cap U$ to G is étale at $(0,0)$.

The tangent linear maps at 0 of the maps $x \rightarrow a$(exp $x)$ and $y \rightarrow$ (exp $y)a$(exp $y)^{-1}$ are the maps $x \rightarrow ax$ and $y \rightarrow ya-ay=a(a^{-1}ya-y)$ from $\mathfrak{g}$ to $T_aG =a\mathfrak{g}$ (Chap. III, §3, no. 12, Prop. 46). Consequently, the tangent map of $f$ at $(0,0)$ is the map $(x, y) \rightarrow ax+a(a^{-1}ya-y) =a(x+a^{-1}ya-y)$ from $\mathfrak{g}^1(a)\times \mathfrak{m}$ to $a\mathfrak{g}$. This map is injective. Indeed, if $x\in \mathfrak{g}^1(a), y\in \mathfrak{m}$ and if $x+a^{-1}ya-y$ = 0, then (Ad($a$)$-1)y$ = Ad($a$)$x\in \mathfrak{g}^1(a)$ since Ad($a$)$\mathfrak{g}^1(a)\subset \mathfrak{g}^1(a)$. This implies that $y\in \mathfrak{g}^1(a)$ and consequently that $y$ = 0. Since Ad($a$) is injective on $\mathfrak{g}^1(a)$, it follows that $x$ = 0. Since dim $\mathfrak{g}=$ dim$\mathfrak{g}^1(a) +$ dim $\mathfrak{m}$, this shows that $f$ is étale at $(0,0)$.

#### Proposition 4 {#lie-vii-s4-prop-4 .statement tag=00W3}

Let $a\in G$ and H be a Lie subgroup germ of G with Lie algebra $\mathfrak{g}^1(a)$. The map $(b, c) \rightarrow cabc^{-1}$ from $H\times G$ to G is a submersion at $(e, e)$.

Indeed, let $\mathfrak{m}$ be a complement of $\mathfrak{g}^1(a)$ in $\mathfrak{g}$ and exp an exponential map of G defined on an open neighbourhood U of 0 in $\mathfrak{g}$. We can choose U so that exp(U $\cap \mathfrak{g}^1(a))\subset H$. The map $f: (x, y) \rightarrow$ (exp $x$, exp $y)$ is an analytic map on a neighbourhood of $(0,0)$ in $\mathfrak{g}^1(a)\times \mathfrak{m}$ with values in $H\times G$. By Lemma 3, the composite of $f$ with the map $\varphi : (b, c) \rightarrow cabc^{-1}$ is étale at $(0,0)$. It follows that $\varphi$ is a submersion at $f(0,0) = (e, e)$.

#### Proposition 5 {#lie-vii-s4-prop-5 .statement tag=00W4}

Let $a\in G$ and let W be a neighbourhood of $e$ in G. There exists a neighbourhood V of $a$ with the following property: for all $a'\in V$, there exists an element $g\in W$ such that $\mathfrak{g}^1(a')\subset$ Ad($g$)$\mathfrak{g}^1(a)$.

Put $\mathfrak{g}^1=\mathfrak{g}^1(a)$ and let $\mathfrak{g}=\mathfrak{g}^1+\mathfrak{g}^+$ be the Fitting decomposition of Ad($a$)$-1 ($§1, no. 1). Let H be a Lie subgroup germ of G with Lie algebra $\mathfrak{g}^1$. For all $h\in H$, Ad($h$)$\mathfrak{g}^1\subset \mathfrak{g}^1$. Since $[\mathfrak{g}^1,\mathfrak{g}^+]\subset \mathfrak{g}^+$, there exists a neighbourhood U of $e$ in H such that Ad($h$)$\mathfrak{g}^+\subset \mathfrak{g}^+$ for all $h\in H$. Since the restriction of Ad($a$)$-1$ to $\mathfrak{g}^+$ is bijective, U can be chosen so that the restriction of Ad($ah$)$-1$ to $\mathfrak{g}^+$ is bijective for all $h\in U$. Then $\mathfrak{g}^1(ah)\subset \mathfrak{g}^1(a) =\mathfrak{g}^1$ for all $h\in U$. By Proposition 4, Int(W)($aU$) is a neighbourhood of $a$ in G. If $a'\in$ Int(W)($aU$), then $a'=g(ah)g^{-1}$ with $g\in W$ and $h\in U$; it follows that $\mathfrak{g}^1(a') =$ Ad($g$)$\mathfrak{g}^1(ah)\subset$ Ad($g$)$\mathfrak{g}^1(a)$.

#### Corollary {#lie-vii-s4-n2-cor-1 .statement tag=00W5}

Let $G^*$ be an open subgroup of G. If $a\in G$ is regular, there exists a neighbourhood V of $a$ such that, for all $a'\in V,\mathfrak{g}^1(a')$ is conjugate to $\mathfrak{g}^1(a)$ under Ad(G$^*)$.

### 3. RELATIONS WITH REGULAR ELEMENTS OF THE LIE ALGEBRA

#### Proposition 6 {#lie-vii-s4-prop-6 .statement tag=00W6}

Let V be an open subgroup of $\mathfrak{g}$ and let exp$: V\rightarrow G$ be an exponential map defined on V.

(i) There exists a neighbourhood W of 0 in V such that $\mathfrak{g}^1$(exp $x) =\mathfrak{g}^0(x)$ for all $x\in W$.

(ii) If $k=\mathbf{R}$ or $\mathbf{C},\mathfrak{g}^1$(exp $x)\supset \mathfrak{g}^0(x)$ for all $x\in \mathfrak{g}$.

By Cor. 3 of Prop. 8 of Chap. III, §4, no. 4, there exists a neighbourhood $V'$ of 0 in V such that, for all $x\in V'$, exp(ad($x$)) $=\sum_{n=0}^{\infty}\frac{1}{n!}$ ad($x$)$^n$ is defined and Ad(exp $x) =$ exp(ad($x$)). If $P\in k[X]$ and $\alpha \in$ End($\mathfrak{g}$), it is easy to check that $\mathfrak{g}^{\lambda}(\alpha )\subset \mathfrak{g}^{P(\lambda)}(P(\alpha ))$ for all $\lambda \in k$. Consequently,

$\mathfrak{g}^0$(ad($x$))$\subset \mathfrak{g}^1$(exp(ad($x$))) $=\mathfrak{g}^1$(Ad(exp $x)) =\mathfrak{g}^1$(exp $x)$

for all $x\in V'$. If $k=\mathbf{R}$ or $\mathbf{C}, V =\mathfrak{g}$ and we can take $V'$ = V, which proves (ii). We prove (i). Let U be a neighbourhood of 0 in End($\mathfrak{g}$) such that Log(1 $+\alpha ) =\sum_{n>0}(-1)^{n+1 1}_{\overline{n}}\alpha^n$ is defined for all $\alpha \in U$. Then Log $\circ$ exp = 1 on a neighbourhood of 0 and $\mathfrak{g}^1(1 +\alpha )\subset \mathfrak{g}^0$(Log(1 $+\alpha ))$ for all $\alpha \in U$. Let W be the neighbourhood of 0 in $\mathfrak{g}$ consisting of those $x\in V'$ such that exp ad $x\in 1 + U$ and

Log(exp(ad($x$))) $=$ ad($x$).

Then, for all $x\in W$,

$\mathfrak{g}^1$(exp $x) =\mathfrak{g}^1$(Ad(exp $x)) =\mathfrak{g}^1$(exp(ad($x$)))

$\subset \mathfrak{g}^0$(Log(exp(ad($x$)))) $=\mathfrak{g}^0$(ad($x$)) $=\mathfrak{g}^0(x)$.

This shows that $\mathfrak{g}^1$(exp $x) =\mathfrak{g}^0(x)$ for all $x\in W$.

#### Lemma 4 {#lie-vii-s4-lem-4 .statement tag=00W7}

Let U be a neighbourhood of 0 in $\mathfrak{g}$ and exp an exponential map from U to G, étale at every point of U and such that $\mathfrak{g}^1$(exp $x) =\mathfrak{g}^0(x)$ for all $x\in U$.

(i) The function $r^0_{Ad}$ is constant and equal to the rank of $\mathfrak{g}$ on exp(U).

(ii) If $x\in U$, exp $x$ is regular if and only if $x$ is a regular element of $\mathfrak{g}$.

(iii) An element $a\in$ exp(U) is regular if and only if $\mathfrak{g}^1(a)$ is a Cartan subalgebra of $\mathfrak{g}$.

Let $l=$ rk($\mathfrak{g}$). If $x\in U$ is a regular element of $\mathfrak{g}$,

$r_{Ad}$(exp $x) =$ dim$\mathfrak{g}^1$(exp $x) =$ dim$\mathfrak{g}^0(x) =l$.

Since the regular elements of $\mathfrak{g}$ belonging to U constitute a neighbourhood of $x$ and exp is étale at $x$, this shows that exp $x$ is regular and that $r^0_{Ad}$(exp $x) =l$. The regular elements of $\mathfrak{g}$ belonging to U being dense in U, we have $r^0_{Ad}(a) =$ $l$ for all $a\in$ exp(U). Let $a\in$ exp(U) be a regular element of G and let $x\in U$ be such that $a=$ exp $x$. Since $\mathfrak{g}^0(x) =\mathfrak{g}^1(a)$, dim $\mathfrak{g}^0(x) =r^0_{Ad}(a) =l$. Consequently, $x$ is a regular element of $\mathfrak{g}$ and $\mathfrak{g}^1(a)$ is a Cartan subalgebra of $\mathfrak{g}$. Finally, if $a\in$ exp(U) and $\mathfrak{g}^1(a)$ is a Cartan subalgebra of $\mathfrak{g}$,

$r_{Ad}(a) =$ dim$\mathfrak{g}^1(a) =l=r_{Ad}^0(a)$,

so $a$ is regular.

#### Proposition 7 {#lie-vii-s4-prop-7 .statement tag=00W8}

Let V be a neighbourhood of $e$ in G. Every Cartan subalgebra of $\mathfrak{g}$ is of the form $\mathfrak{g}^1(a)$ where $a$ is a regular element of G belonging to V.

By Prop. 6, there exists an open neighbourhood U of 0 in $\mathfrak{g}$ and an exponential map exp$: U\rightarrow G$ satisfying the conditions of Lemma 4. If $\mathfrak{h}$ is a Cartan subalgebra of $\mathfrak{g}$, there exists a regular element $x\in \mathfrak{h}$ such that $\mathfrak{h}=\mathfrak{g}^0(x) ($§3, Th. 2). On the other hand, there exists an element $t\in k^*$ such that $tx\in U$ and exp($tx$)$\in V$. Then $\mathfrak{h}=\mathfrak{g}^0(x) =\mathfrak{g}^0(tx) =\mathfrak{g}^1$(exp($tx$)), and by Lemma 4 (ii), exp($tx$) is a regular element of G.

#### Proposition 8 {#lie-vii-s4-prop-8 .statement tag=00W9}

Let $l$ be the rank of $\mathfrak{g}$. There exists an open subgroup $G^*$ of G such that:

(i) the function $r^0_{Ad}$ is constant on $G^*$ and its value is $l$;

(ii) an element $a\in G^*$ is regular if and only if $\mathfrak{g}^1(a)$ is a Cartan subalgebra of $\mathfrak{g}$;

(iii) if $a\in G^*$, every Cartan subalgebra of $\mathfrak{g}^1(a)$ is a Cartan subalgebra of $\mathfrak{g}$.

(i) By Prop. 6, there exists an open neighbourhood U of 0 in $\mathfrak{g}$ and an exponential map exp from U to G satisfying the conditions of Lemma 4. In what follows, $G^*$ will denote the identity component of G if $k=\mathbf{R}$ or $\mathbf{C}$ and an open subgroup of G contained in exp(U) if $k$ is ultrametric. Since $r_{Ad}^0$ is locally constant and its value at any point of exp(U) is $l$ (Lemma 4 (i)), it follows that $r_{Ad}^0$ is constant and equal to $l$ on $G^*$.

(ii) Let $R^*$ (resp. $S^*)$ be the set of regular elements of $G^*$ (resp. the set of elements $a\in G^*$ such that $\mathfrak{g}^1(a)$ is a Cartan subalgebra of $\mathfrak{g})$. Then $S^*\subset R^*$. Indeed, if $a\in S^*$, then $r_{Ad}(a) =l=r^0_{Ad}(a)$. We show that $R^*\subset S^*$. If $k$ is ultrametric, this follows from the inclusion $G^*\subset$ exp(U) and Lemma 4 (iii). Assume that $k=\mathbf{C}$. By the Cor. of Prop. 5, if $a\in R^*$, then for every $a'$ belonging to a neighbourhood of $a,\mathfrak{g}^1(a')$ is conjugate to $\mathfrak{g}^1(a)$ by an automorphism of $\mathfrak{g}$. This proves that $S^*$ and $R^*$ **--** $S^*$ are open subsets of $G^*$. We have seen that $S^*$ contains all the regular elements in a neighbourhood of $e$ (Lemma 4 (iii)); consequently, $S^*$ is non-empty. Since $G^*$ is connected, so is $R^*$ (Prop. 1) and consequently $S^*= R^*$.

It remains to study the case $k=\mathbf{R}$. Assume first of all that $G^*$ is an integral subgroup of $\mathbf{G}\mathbf{L}(E)$ where E denotes a finite dimensional real vector space. Let $G^*_c$ be the integral subgroup of $\mathbf{G}\mathbf{L}(E\otimes_{\mathbf{R}}\mathbf{C})$ with Lie algebra $\mathfrak{g}_c=\mathfrak{g}\otimes \mathbf{C}$. There exists an analytic function on $G^*_c$ whose set of zeros is the complement of the open set of regular elements of $G^*_c$. By Differentiable and Analytic Manifolds, Results, 3.2.5, this function cannot vanish at every point of $G^*$. Consequently, $G^*$ contains a regular element of $G^*_c$. Let Ad$_c$ be the adjoint representation of $G^*_c$. For any $a\in G^*,\mathfrak{g}^1_c(a) =\mathfrak{g}^1(a)\otimes \mathbf{C}$, so $r_{Ad_c}(a) =r_{Ad}(a)$. If $a\in G^*$ is a regular element of $G^*_c$, this is a regular element of $G^*$ and $r_{Ad}^0(a) =r_{Ad}^0(a)$. The functions $r^0_{Ad}$ and $r_{Ad}^0$ being constant on $G^*_c$ and on $G^{^c*}$, respectively, it follows that the regular elements$^{^c}$ of $G^*$ are the regular elements of $G^*_c$ belonging to $G^*$. From the above, if $a$ is a regular element of $G^*,\mathfrak{g}^1_c(a) =\mathfrak{g}^1(a)\otimes \mathbf{C}$ is a Cartan subalgebra of $\mathfrak{g}_c$; this implies that $\mathfrak{g}^1(a)$ is a Cartan subalgebra of $\mathfrak{g}($§2, Prop. 3).

Assume now that G is simply connected. There exists a finite dimensional real vector space E and an étale morphism $f$ from G to an integral subgroup $G'$ of $\mathbf{G}\mathbf{L}(E)$ (Chap. III, §6, no. 1, Cor. of Th. 1). By Prop. 2, if $a\in G$ is regular, $f(a)$ is regular. By the preceding, ${\mathfrak{g}'}^1(f(a))$ is a Cartan subalgebra of the Lie algebra $\mathfrak{g}'$ of $G'$. Since ${\mathfrak{g}'}^1(f(a)) = (Tf)\mathfrak{g}^1(a)$ and $Tf$ is an isomorphism from $\mathfrak{g}$ to $\mathfrak{g}'$, this proves that $\mathfrak{g}^1(a)$ is a Cartan subalgebra of $\mathfrak{g}$.

We turn finally to the general case $(k=\mathbf{R})$. Let $\widetilde{G}$ be a universal covering of $G^*, \widetilde{\mathfrak{g}}= L( \widetilde{G})$, and $q$ the canonical map from $\widetilde{G}$ to $G^*$. Since the kernel of $q$ is contained in the centre of $\widetilde{G}$, if $a\in G^*$ is regular and if $a'\in q^{-1}(a)$, then $a'$ is regular (Prop. 2). By the preceding, $\widetilde{\mathfrak{g}}^1(a')$ is a Cartan subalgebra of $\widetilde{\mathfrak{g}}$. Since $\mathfrak{g}^1(a) = (Tq)\widetilde{\mathfrak{g}}^1(a')$ and since $Tq$ is an isomorphism from $\widetilde{\mathfrak{g}}$ to $\mathfrak{g}$, this proves that $\mathfrak{g}^1(a)$ is a Cartan subalgebra of $\mathfrak{g}$.

(iii) By Prop. 5, there exists a neighbourhood V of $a$ such that, for all $a'\in V,\mathfrak{g}^1(a')$ is conjugate to a subalgebra of $\mathfrak{g}^1(a)$ by an automorphism of $\mathfrak{g}$. Since every neighbourhood of $a$ contains a regular element of $G^*$, it follows from (ii) that $\mathfrak{g}^1(a)$ contains a Cartan subalgebra of $\mathfrak{g}$. Thus, by Prop. 3 of §3, every Cartan subalgebra of $\mathfrak{g}^1(a)$ is a Cartan subalgebra of $\mathfrak{g}$.

#### Remark {#lie-vii-s4-n3-rem-1 .statement tag=00WA}

If $k=\mathbf{C}$, the subalgebras $\mathfrak{g}^1(a)$, for $a$ regular and belonging to a connected component M of G, are conjugate under Int($\mathfrak{g}$). Indeed, let R be the set of regular elements of G. For all $a\in R\cap M$, let $M_a$ be the set of those $b\in R\cap M$ such that $\mathfrak{g}^1(a)$ is conjugate to $\mathfrak{g}^1(a)$ under Int($\mathfrak{g}$). We have Int($\mathfrak{g}$) $=$ Ad(G$^0)$, where $G^0$ is the identity component of G. By the Corollary to Prop. $5, M_a$ is open in R. It follows that $M_a$ is open and closed in R. Since $k=\mathbf{C}, R\cap M$ is connected (Lemma 1), hence $M_a= R\cap M$.

### 4. APPLICATION TO ELEMENTARY AUTOMORPHISMS

#### Proposition 9 {#lie-vii-s4-prop-9 .statement tag=00WB}

Let $k$ be a field of characteristic 0 and $\mathfrak{g}$ a Lie algebra over $k$. If $a\in$ Aut$_e(\mathfrak{g})$, the dimension of the nilspace of $a-1$ is greater than or equal to the rank of $\mathfrak{g}$.

By the “Lefschetz principle” (Algebra, Chap. V, §14, no. 6, Cor. 2 of Th. $5),k$ is an ascending directed union of subfields $(k_i)_{i\in I}$ which admit $\mathbf{C}$ as extension field. Let $(e_{\alpha})$ be a basis of $\mathfrak{g}$ over $k$ and $x_1, . . . , x_m$ elements of $\mathfrak{g}$ such that ad($x_1$)$, . . .$, ad($x_m$) are nilpotent and $a=e^{ad(x_1)}. . . e^{ad(x_m)}$. Let $c^{\gamma}_{\alpha \beta}$ be the structure constants of $\mathfrak{g}$ with respect to the basis $(e_{\alpha})$ and $(x^{\alpha}_r)$ the components of $x_r$ with respect to this basis $(1\leq r\leq m)$. There exists an index $j\in I$ such that the $c^{\gamma}_{\alpha \beta}$ and the $x^{\alpha}_r$ all belong to $k_j$. Let $\mathfrak{g}_j=\sum_{\alpha}k_je_{\alpha}$;

this is a Lie algebra over $k_j$ containing $x_1, . . . , x_m$, and the restriction $a_j$ of $a$ to $\mathfrak{g}_j$ is an elementary automorphism of $\mathfrak{g}_j$. The extension of $a_j$ to $\mathfrak{g}_j\otimes_{k_j}\mathbf{C}$ is an elementary automorphism $a_j\otimes 1$ of $\mathfrak{g}_j\otimes \mathbf{C}$. So let $G_j$ be a connected complex Lie group with Lie algebra $\mathfrak{g}_j\otimes \mathbf{C}$, and $s$ an element of $G_j$ such that Ad($s$) $=a_j\otimes 1$. Prop. 8, applied to the pair $(G_j, s)$, shows that the nilspace of $a_j\otimes 1-1$ is of dimension $n$, so

$n\geq$ rk($\mathfrak{g}_j\otimes \mathbf{C}$) $=$ rk($\mathfrak{g}_j$) $=$ rk($\mathfrak{g}$).

But this nilspace has the same dimension as that of $a_j-1$ and that of $a-1$. Hence the proposition.

### Exercises {#lie-vii-s4-exercises}

The notations and assumptions are those of nos. 1, 2, 3 of §4.

See the [exercises for § 4](exercises/s4/).
