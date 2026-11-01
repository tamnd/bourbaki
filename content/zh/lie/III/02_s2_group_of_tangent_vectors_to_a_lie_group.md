---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 2
section_title: Group of tangent vectors to a Lie group
lang: zh
source: lie-i-iii
book_pages: 233-238
pdf_pages: 0251-0256
extraction: ocr
subsections:
    - "no": 1
      title: TANGENT LAWS OF COMPOSITION
      page: 233
      pdf_page: 251
    - "no": 2
      title: GROUP OF TANGENT VECTORS TO A LIE GROUP
      page: 235
      pdf_page: 253
    - "no": 3
      title: CASE OF GROUP GERMS
      page: 237
      pdf_page: 255
statements: 10
exercises: 0
content_sha256: 963f4bda36ab07046752d9258f718da283697ab03423a39732073fada575a6d5
translated_from: content/en/lie/III/02_s2_group_of_tangent_vectors_to_a_lie_group.md
translation_method: google
source_content_sha256: 9312e1a966f1c5bc60ded7611d1345461f06db492fc343d729b16bcbbd46a1c0
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 2c799a8e5f86a04dd77a0386b2ce07d96bd5075e758eaece4e03ee8cbc3ec844
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 2。 群向量与李群的切线

### 1. 合成的切线律

令X和Y为类C^r中的流形。我们知道（可微分和解析流形，R，8.1.4）X\times Y是类C^r的流形，并且映射（T（pr_1），T（pr_2）），乘积映射与规范投影的切线，是 T(X \times Y) 的类 C^{r-1} 到 T(X) \times T(Y) 的同构。\footnote{对于 r = 1，这意味着(T(pr_1), T(pr_2)) 是 T(X \times Y) 的同态到 T(X) \times T(Y)。} 这个同构与向量丛结构和基空间兼容X \times Y 并允许我们认同 T(X \times Y) 和 T(X) \times T(Y)。设a ε X，b ε Y，u ε T_a(X)，v ε T_b(Y)；上述识别允许我们将 (u, v) 视为 T_{(a, b)}(X × Y) 的元素；那么

$$(u, v) = (u, 0) + (0, v)$$

(u, 0) (resp. (0, v)) 是 u (resp. v) 的像在 X (resp. Y) 的浸没 x ↦ (x, b) (resp. y ↦ (a, y)) 到 X × Y 的切线映射下。准确地说，我们将 T_a(x) 的零元素写为 0_a。

现在设X，Y，Z为类C^r的流形和X×Y到Z的类C^r的f映射。使用上述标识，映射的切线为，将 T(X) × T(Y) 的映射类 C^{r-1} 转换为 T(Z)。对于 u Î T_a(X) 且 v Î T_b(Y)，

(1)
$$T(f)(u, v) = T(f)(u, 0_b) + T(f)(0_a, v),$$
(2)
$$T(f)(0_a, 0_b) = 0_{f(a, b)}.$$

另一方面，映射 y ↦ f(a, y) 是浸没 y ↦ (a, y) 和 f 的合成；由此可见

(3) $T(f)(0, v)$ 是 v 在映射到 $y \mapsto f(a, y)$ 的切线下的像。

同样

(4) $T(f)(u, 0)$ 是 u 在映射到 $x \mapsto f(x, b)$ 的切线下的像。

如果将 X × Y 的映射 f 代入 Z 表示为 (x, y) ↦ xy，则 uv 常用于表示元素 T(f)(u, v)，因为 u ∈ T(X)，v ∈ T(Y)。

设X为类C^r流形和m：X×X→类合成X律 C^r 于X。那么T(m)就是T(X)上类C^{r-1}合成律。称为合成与 m 的切线律。 T(X)在X上的规范投影p与律m和T(m)相容的；在其他字，

(5)
$$p \circ T(m) = m \circ (p \times p).$$

由(2)可知

(6)
$$T(m)(0_x, 0_y) = 0_{m(x, y)}$$

对于 X 中的所有 x, y；其他字、T(X)的零、截面$x \mapsto 0_x$与律 m 和 T(m) 相容的。

#### 命题 1 {#lie-iii-s2-prop-1 .statement tag=0A8Y}

*设X为类C^r流形，且X上类C^r合成m律。如果 m 是结合律（或可交换的），则 T(m) 是结合律（或可交换的）。*

如果 m 是结合律，则 $m \circ (m \times \mathrm{Id}_X) = m \circ (\mathrm{Id}_X \times m)$, 从而

$$T(m) \circ (T(m) \times \mathrm{Id}_{T(X)}) = T(m) \circ (\mathrm{Id}_{T(X)} \times T(m))$$

因此 $T(m)$ 是结合律。设 $s$ 为 $X \times X$ 的映射 $(x, y) \mapsto (y, x)$ 到 $X \times X$。如果 $m$ 是可交换的，则 $m \circ s = m$ 因此

$$
T(m) \circ T(s) = T(m).
$$

但是$T(s)$是$T(X) \times T(X)$的映射$(u, v) \mapsto (v, u)$变成$T(X) \times T(X)$。因此 $T(m)$ 是可交换的。

#### 命题 2 {#lie-iii-s2-prop-2 .statement tag=0A8Z}

*令$X$为类$C^r$流形，$X$和$e$上类$C^r$合成$m$律单位元素换$m$。

(i) *向量 $0_e$ 是单位元素对应$T(m)$。
(ii) *$T_e(X)$在$T(m)$和律下稳定，合成在$T_e(X)$上由$T(m)$诱导为向量空间加法在$T_e(X)$上。
(iii) *令$U$为$X$的开子集和$U$的类$C^r$入$X$的$\alpha$映射，使得对于所有$x \in U$， $\alpha(x)$是$x$在$m$下的逆。那么，对于所有$u \in T(U)$，$T(\alpha)u$是$u$在$T(m)$下的逆。

性质 (3) 和 (4) 表明对于所有 $u \in T(X)$、从而 (i) 都有 $T(m)(0_e, u) = T(m)(u, 0_e) = u$。对于$T_e(X)$中的$u, v$，

$$
T(m)(u, v) = T(m)(u, 0_e) + T(m)(0_e, v) = u + v,
$$

从而（二）。最后关系$m(x, \alpha(x)) = m(\alpha(x), x) = e$对于所有$x \in U$意味着

$$
T(m)(u, T(\alpha)(u)) = T(m)(T(\alpha)u, u) = 0_e
$$

对于所有$u \in T(U)$，从而 (iii)。

#### 命题 3 {#lie-iii-s2-prop-3 .statement tag=0A90}

*设$X_1, X_2, \ldots, X_p, Y$为类$C^r$流形，$\{1, p\}$$i$整数，$m_i$（分别为$n$）类合成律 $C^r$ $X_i$（分别为 $Y$）和$u$ 映射类 $C^r$ $X_1 \times X_2 \times \cdots \times X_p$ 进入$Y$。如果 $u$ 相对于指标 $i$ 变量具有分配性，则 $T(u)$ 相对于指标 $i$ 变量具有分配性。

证明类似于命题 1。

### 2. 向量到李群的切线群

#### 命题 4 {#lie-iii-s2-prop-4 .statement tag=0A91}

*令$G$为李群。那么$T(G)$，合成的律与$G$的乘法相切，就是李群。 $T(G)$的单位元素是向量$0_e$。

这是从命题 1 和 2 得出的。

#### 命题 5 {#lie-iii-s2-prop-5 .statement tag=0A92}

*设$G$和$H$为$G$的李群和$f$态射到$H$。那么$T(f)$就是李群$T(G)$的态射变成李群$T(H)$。

我们知道$T(f')$是解析的。另一方面，令$m$（或$n$）表示$G$（或$H$）上的乘法。然后$f \circ m = n \circ (f \times f)$，从而

$$
T(f) \circ T(m) = T(n) \circ (T(f) \times T(f)),
$$

它表达了$T(f)$是群同态这一事实。

#### 推论{#lie-iii-s2-n2-cor-1 .statement tag=0A93}

*令$G_1, \ldots, G_n$为李群。 流形 $T(G_1 \times \cdots \times G_n)$ 到流形 $T(G_1) \times \cdots \times T(G_n)$ 的典范同构是李群同构。*

$\mathrm{pr}_i$ 是$G_1 \times \cdots \times G_n$ 的态射到$G_i$，因此$T(\mathrm{pr}_i)$ 是$T(G_1 \times \cdots \times G_n)$ 的态射到$T(G_i)$。

#### 命题 6 {#lie-iii-s2-prop-6 .statement tag=0A94}

*令$G$为李群。*
  (i) *规范投影 $p : T(G) \to G$ 为李群态射。*
  (ii) *$p$中的核为$T_e(G)$。这是$T(G)$的谎言子群。 李群结构在 $T_e(G)$ 上由 $T(G)$ 诱发，是完整范数空间 $T_e(G)$ 的李群结构。*
  (iii) *零截面 $s$ 是李群 $G$ 的同构到子群 $s(G)$ 的$T(G)$ 上（子群我们认同与$G$).*
  (iv) *李群$T(G)$是$G$乘$T_e(G)$的半直接乘积。*

断言 (i) 由 (5) 得出。考虑到命题 2 (ii)，断言 (ii) 是显而易见的。 断言 (iii) 和 (iv) 由 (6) 和 § 1、命题 8 得出。

设$u \in T(G)$和$g \in G$。通过(3)和(4)，群$T(G)$计算出的乘积$ug, gu$是$T(\delta(g^{-1}))$和$T(\gamma(g))$下$u$的像。从§ 1，推论2到命题17，$G \times T_e(G)$进入$T(G)$的映射$(g, u) \mapsto gu$是平凡的向量丛$G \times T_e(G)$与基的同构空间$G$到向量丛$T(G)$。 逆同构被称为 $T(G)$ 的*左平凡化*。通过考虑映射$(g, u) \mapsto ug$，$T(G)$的*右平凡化*也有类似的定义。

#### 命题 7 {#lie-iii-s2-prop-7 .statement tag=0A95}

*令$G$为李群、类$C^r$的$M$流形和$f$以及类$C^r$的$g$映射 $M$ 转化为 $G$，因此 $fg$ 就是类 $C^r$ 的映射 $M$ 转化为 $G$。让$m \in M, x = f(m), y = g(m), u \in T_m(M)$。然后*

$$
(T fg)u = T(f)u.y + x.T(g)u.
$$

令 $m$ 为 $G$ 的乘法。然后$fg = m \circ (f, g)$。现在

$$
T(f, g)(u) = (T(f)u, T(g)u),
$$

因此$T(fg)u = T(f)u.T(g)u$。然后应用 (1) 并将 $f$ 替换为 $m$ 即可。

#### 推论{#lie-iii-s2-n2-cor-2 .statement tag=0A96}

*设$n \in \mathbf{Z}$。 $G$ 到 $G$ 的 $e$ 到映射 $g \mapsto g^n$ 的切线映射是 $T_e(G)$ 到 $T_e(G)$ 的映射 $x \mapsto nx$。*

对于 $n \geqslant 0$，其后面是从命题 7 到 $n$ 的归纳。另一方面，$e$ 到映射 $g \mapsto g^{-1}$ 的切线映射是映射 $x \mapsto -x$ (no. 1， 命题2)。

设G为类C^r的李群、X流形和X上G的类C^r的左运算的(g,x)\mapsto gx律。 对于命题 1，我们推导出T(G)在T(X)上的类C^{r-1}的左运算的律，我们也将其表示为(u, v) \mapsto uv。 将 G（分别为 X）与 T(G) 的零截面的像（分别为 T(X)）进行识别，我们可以通过 (6) 看到 T(G) 的左运算的律在 T(X) 扩展上X 上 G 左侧运算的律。 对于所有 u \in T_g(G) 和 v \in T_x(X)，通过 (1)，

$$
uv = gv + ux.
$$

如果 g \in G 和 v \in T_x(X)，则通过 (3)，gv 是 v 在 x 到映射处的切线映射下的像将 X 映射到 X。该切线映射是 T_x(X) 到 T_{gx}(X) 的同构。尤其，

$$
g(v + v') = gv + gv', \quad g(\lambda v) = \lambda(gv) \quad \text{for } v, v' \text{ in } T_x(X), \lambda \in K.
$$

如果 x \in X 且 u \in T_g(G)，ux 是 u 在 g 处的切线映射下到映射 h \mapsto hx of G 到 X 的 (4) 像。因此

$$
(u + u')x = ux + u'x, \quad (\lambda u)x = \lambda(ux) \quad \text{for } u, u' \text{ in } T_g(G), \lambda \in K.
$$

上述可以应用于李群通过左（或右）平移对其自身进行操作的情况。 T(G) 上 T(G) 的运算的相应的律由李群 T(G) 的左（或右）平移定义。因此，公式 (7)、(8) 和 (9) 在 T(G) 中有效。

#### 命题 8 {#lie-iii-s2-prop-8 .statement tag=0A97}

Let G_1 and G_2 be Lie groups, X_1 and X_2 manifolds of class C^r and f_i a law of left operation of class C^r of G_i on X_i (i = 1, 2). 设\phi为G_1到G_2的态射，\psi为X_1到X_2的\phi同态。 那么 T(\psi) 是 T(X_1) 到 T(X_2) 的 T(\phi) 态射。

f_2 \circ (\phi \times \psi) = \psi \circ f_1, 从而

$$
T(f_2) \circ (T(\phi) \times T(\psi)) = T(\psi) \circ T(f_1).
$$

设G为类C^r的李群、X流形，以及G在X上的类C^r的左运算的(g,x)\mapsto gx律。令 I 为 K 包含 0 和 \gamma: I \ 到类 C^r 的 G 映射的开子集，使得 \gamma(0) = e。让

$$
a = T_0(\gamma)1 \in T_e(G).
$$

设 x \in X。使用 (4)，ax 是像在 0 处向量 1 到 I 的切线映射到 \lambda \mapsto \gamma(\lambda)x 的切线下。因此 *向量域* x \mapsto ax 在 X *是向量域由映射* (\lambda, x) \mapsto \gamma(\lambda)x *在可微分和解析的意义上定义流形*, R, 8.4.5。

### 3. 群细菌案例

设(G, e, θ, m)为m的李群胚芽和定义的\Omega集合。然后 T(\Omega) 被识别为 T(G) \times T(G) 的开子集，并且 T(m) 是 $T(\Omega)$ 到 $T(G)$ 的解析映射。可以如no. 2中验证$(T(G), 0_e, T(\theta), T(m))$是李群胚芽。 $G$和$T(G)$的乘积经常写成乘法。 $T(G)$到$G$的标准投影是李群细菌的态射。 $T_e(m)$到$T_e(G)$的限制是$T_e(G)$的向量空间加法。 $T(G)$的零截面是李群胚芽$G$的同构到$T(G)$的谎言子群胚芽，我们认同与$G$。如果$f$是$G$的态射变成李群胚芽$H$，$T(f): T(G) \to T(H)$就是李群胚芽的态射。

$G \times T_e(G)$的映射$\phi: (g, u) \mapsto gu$到$T(G)$是琐碎的向量丛$G \times T_e(G)$与基空间$G$到向量丛$T(G)$的同构；因为 $\phi$ 和 $\phi^{-1}$ 是解析的，并且是向量丛态射，因此只需应用 *可微分和解析流形*，R，7.2.1。 （no. 2的证明也可以改编。）同构$\phi^{-1}$称为$T(G)$的左平凡化。 映射 $(g, u) \mapsto ug$ 的逆同构称为右平凡化。

令$X$为类$C^r$的流形和$X$上$G$的类$C^r$的左运算块$\psi$律块。那么$T(\psi)$是$T(G)$的类$C^{r-1}$的左运算的律块，在$T(X)$上延伸$\psi$。如果定义了 $gx$，公式 (7)、(8) 和 (9) 仍然有效。如果$I$是$K$包含0的开子集，如果$\gamma: I \to G$是类$C^r$的映射，使得$\gamma(0) = e$并且如果$a = T_0(\gamma)1$，向量在 $X$ 上定义的域 $x \mapsto ax$ 是由映射 $(\lambda, x) \mapsto \gamma(\lambda)x$ 定义的向量域，在*可微分和解析流形* 的意义上，R，8.4.5。
