---
book: int
book_title: Integration
chapter: I
chapter_title: INEQUALITIES OF CONVEXITY
section: 0
section_title: INEQUALITIES OF CONVEXITY
kind: front
lang: zh
source: int-i-vi
pdf_pages: 0016-0022
extraction: ocr
subsections:
    - "no": 1
      title: The fundamental inequality of convexity
      page: 0
      pdf_page: 16
    - "no": 3
      title: The semi-norms $N_p$
      page: 4
      pdf_page: 19
statements: 0
exercises: 0
content_sha256: 8e30353d8f396e9b0cde8ea49c650506585c76d878f18875d1b078b39b85e51a
translated_from: content/en/int/I/00_frontmatter.md
translation_method: google
source_content_sha256: f9fb1f9ad9415bc967e08205858a5af5eecf03e7f2b0b9123eb6a2caf75a5af8
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: ac3540840cc1cb0421105095ec958e436783d536bf45fec779d6716c610d3236
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 章 I

# 凸性不等式

### 1. 凸性的基本不等式

设X为集合；在X上定义的所有有限数值函数$^1$的向量空间$\mathbf{R}^X$中，令P为X上所有正实值函数的集合。另一方面，令 $M$ 为数值函数，$^2$ 是否有限，且值 $\geqslant 0$，定义在 P 上，使得：

$1^\circ$ $M(0) = 0$，且 $M$ 是正齐次的，即，对于每个实数 $\lambda > 0$.$^3$，$M(\lambda f) = \lambda M(f)$

$2^\circ$$M$在P中是递增，在其他字关系$f \leqslant g$意味着$M(f) \leqslant M(g)$。

$3^\circ$$M$在P中是凸的，在其他字（TVS，II, §2, No. 8）满足关系$M(f + g) \leqslant M(f) + M(g)$。

*例.* — 假设X是有限的集合，对于例，$[1, n]$为$\mathbf{N}$；用 $x_i$ ($1 \leqslant i \leqslant n$) 表示向量 $\mathbf{x} \in \mathbf{R}^n$、函数的坐标
$$
M_1(\mathbf{x}) = \sum_{i=1}^n x_i \quad \text{and} \quad M_\infty(\mathbf{x}) = \sup_{1 \leqslant i \leqslant n} x_i
$$
满足向量 $\mathbf{x}$ 的集合 P 中的前一个条件，坐标为 $\geqslant 0$。

*注.* — 令 S 为 P 中包含的尖凸圆锥体（即，集合，使得 $S + S \subset S$ 和 $\lambda S \subset S$ 对于 $\lambda \geqslant 0$；cf. TVS，II, §2, No. 4）；令 $M$ 为数值函数（有限或非有限），其中值 $\geqslant 0$，在 S 上定义，并在 S 中定义满足，即上述条件 $1^\circ, 2^\circ$ 和 $3^\circ$。然后$M$可以扩展到整个集合P，这样扩展的函数（我们再次用$M$表示）满足相同的条件：对于每个函数$f \in P$，到集合就足够了如果不存在满足$f \leqslant g$的函数$g \in S$，则为$M(f) = +\infty$，反之则为$M(f) = \inf_{g \in S, f \leqslant g} M(g)$。该程序将应用于第 1 章。 IV, §1 到定义正函数的*上积分*。

(1) 数字函数 — $\mathbf{R}$ 中的函数和值 — 也可翻译为“实值函数”（cf. GT、IV, §5, No. 1）。

(2) 数字函数——“数字函数”——表示函数和$\overline{\mathbf{R}}$中的值（TG，IV, §5, No. 1）。 有时添加短语“是否有限”，以提醒函数可能会呈现无限值。

(3) 回想一下，在$\overline{\mathbf{R}}$、乘积例如$0 \cdot (+\infty)$中没有定义（GT、IV, §4, No. 3）。

命题 1. — 令 $\varphi(t_1, t_2, \ldots, t_n)$ 为有限数值函数，对于 $t_i \geq 0$ ($1 \leq i \leq n$) 定义且连续，使得：
$1^\circ$ 关系 $t_i > 0$ ($1 \leq i \leq n$) 意味着$\varphi(t_1, t_2, \ldots, t_n) > 0$；
$2^\circ$ 函数 $\varphi$ 是正齐次的；
$3^\circ$ 集合 $K \subset \mathbf{R}^n$ 由关系 $t_i \geq 0$ ($1 \leq i \leq n$) 定义，$\varphi(t_1, t_2, \ldots, t_n) \geq 1$ 是凸的。
在这些条件下，如果$f_1, f_2, \ldots, f_n$是$n$有限的函数$\geq 0$定义在$X$上，使得$M(f_i) < +\infty$对于$1 \leq i \leq n$，那么

$$
M(\varphi(f_1, f_2, \ldots, f_n)) \leq \varphi(M(f_1), M(f_2), \ldots, M(f_n)).
$$

人们知道，根据 Hahn-Banach 定理（TVS，II, §5），$K$ 是 $n$ 半空间 $t_i \geq 0$ ($1 \leq i \leq n$) 和一系列闭半空间 $(U_\iota)_{\iota \in I}$、$U_\iota$ 的交由关系或形式定义

$$
\alpha_{\iota 1} t_1 + \alpha_{\iota 2} t_2 + \cdots + \alpha_{\iota n} t_n - \beta_\iota \geq 0,
$$

其中$\alpha_{\iota k}$并不都是零。根据假设，如果$t = (t_i)$对于$1 \leq i \leq n$来说是$t_i > 0$，则$\varphi(t_1, \ldots, t_n) > 0$，因此存在$\lambda_0 > 0$使得关系$\lambda \geq \lambda_0$蕴含$\lambda t \in K$；这表明，对于每个$\iota \in I$，关系$t_i \geq 0$（$1 \leq i \leq n$）意味着$\alpha_{\iota 1} t_1 + \cdots + \alpha_{\iota n} t_n \geq 0$，因此$\alpha_{\iota k} \geq 0$意味着$1 \leq k \leq n$；那么很明显，$K$也是半空间$t_i \geq 0$（$1 \leq i \leq n$）和$U_\iota$的交，使得$\beta_\iota \geq 0$；此外，由于原点不是属于到$K$，因此至少存在一个指标$\iota$使得$\beta_\iota > 0$。

现在令 $C$ 为关系 $t_i \geq 0$ ($1 \leq i \leq n+1$)、$t_{n+1} \leq \varphi(t_1, t_2, \ldots, t_n)$ 定义的$\mathbf{R}^{n+1}$ 中的凸锥（由凸集合 $K \times \{1\}$ 在$\mathbf{R}^{n+1}$ 中生成的凸锥的闭合）； 直接的 $C$ 也由关系 $t_i \geq 0$ ($1 \leq i \leq n+1$) 定义，并且

$$
\beta_\iota t_{n+1} \leq \alpha_{\iota 1} t_1 + \cdots + \alpha_{\iota n} t_n \quad (\iota \in I, \ \beta_\iota \geq 0).
$$

因此，对于每个 $x \in X$，我们有

$$
\beta_\iota \varphi(f_1(x), \ldots, f_n(x)) \leq \alpha_{\iota 1} f_1(x) + \cdots + \alpha_{\iota n} f_n(x)
$$

对于所有$\iota \in I$。对于每个指标$\iota$使得$\beta_\iota > 0$，从(4)和$M$的假设可以得出$M(\varphi(f_1, f_2, \ldots, f_n))$是有限的并且

$$
\beta_\iota M(\varphi(f_1, f_2, \ldots, f_n)) \leq \alpha_{\iota 1} M(f_1) + \alpha_{\iota 2} M(f_2) + \cdots + \alpha_{\iota n} M(f_n),
$$

而这个关系也以明显的方式验证了如果$\beta_\iota = 0$。因此我们看到点的坐标

$$
M(f_1), M(f_2), \ldots, M(f_n), \quad M(\varphi(f_1, f_2, \ldots, f_n))
$$

属于到$C$，从而证明命题。

2. 霍尔德和闵可夫斯基的不等式

本号及下号中，$X$、$P$与No. 1含义相同，$M$表示在$P$上定义的函数满足No. 1中列出的条件。

命题 2. — *令$\alpha$和$\beta$为两个数，使得$0 < \alpha < 1$、$0 < \beta < 1$、$\alpha + \beta = 1$。如果$f$和$g$是定义在$X$上的两个有限函数$\geq 0$，并且如果$M(f)$和$M(g)$是有限的，那么*

$$
M(f^\alpha g^\beta) \leq (M(f))^\alpha (M(g))^\beta
$$

（*霍尔德的不等式*）。

By Prop. 1, it all comes down to proving that, in $\mathbf{R}^2$, the set defined by the relations $t_1 \geq 0$, $t_2 \geq 0$, $t_1^\alpha t_2^\beta \geq 1$ is convex, or again (FRV, I, §4, No. 1, Def. 1) that the function $u(t) = t^{-\alpha/\beta}$ is convex for $0 < t < +\infty$. 现在，设定$r = \alpha/\beta$，我们有$D^2 u(t) = r(r+1)t^{-r-2}$，并且从$r > 0$开始，$]0, +\infty[$上有$D^2 u(t) > 0$，这证明了命题（FRV，I, §4, No. 4，Prop.8的Cor.）。

推论。 — *令 $\alpha_i$ ($1 \leq i \leq n$) 为 $n$ 数 $\geq 0$ 这样*
$$
\sum_{i=1}^n \alpha_i = 1,
$$
*并令$f_i$ ($1 \leq i \leq n$) 为定义在$X$上的$n$ 函数 $\geq 0$，使得$M(f_i)$ 对于$1 \leq i \leq n$ 是有限的。在这些条件下，*

$$
M(f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}) \leq (M(f_1))^{\alpha_1} (M(f_2))^{\alpha_2} \cdots (M(f_n))^{\alpha_n}.
$$

我们可以将注意力限制在每个$i$都有$\alpha_i > 0$的情况。通过归纳对$n$，通过应用不等式(5)到数$\alpha = \alpha_1$和$\beta = \sum_{i=2}^n \alpha_i$，以及到函数$f = f_1$，$g = (f_2^{\alpha_2} f_3^{\alpha_3} \cdots f_n^{\alpha_n})^{1/\beta}$就足够了。

命题 3. — *令$p$为实数$\geq 1$。如果 $f$ 和 $g$ 是在 $X$ 上定义的两个有限函数 $\geq 0$，则*

$$
\left( M((f+g)^p) \right)^{1/p} \leq \left( M(f^p) \right)^{1/p} + \left( M(g^p) \right)^{1/p}
$$

（*闵可夫斯基的不等式*）。

我们可以将注意力限制在$M(f^p)$和$M(g^p)$有限的情况。根据命题1，我们被简化为证明，由关系$t_1 \geq 0,\ t_2 \geq 0,\ t_1^{1/p} + t_2^{1/p} \geq 1$定义的$\mathbf{R}^2$中的集合是凸的，或者函数$u(t) = (1 - t^{1/p})^p$对于$0 \leq t \leq 1$来说是凸的。现在，

$$
D^2 u(t) = \left(1 - \frac{1}{p}\right)t^{1/p-2}(1-t^{1/p})^{p-2} \geq 0
$$

$0 < t \leq 1$、从而命题。

### 3. 半范数$N_p$

令 $p$ 为实数 $\geq 1$，并令 $\mathscr{F}^p(X, M)$ 为集合，在 $X$ 上定义有限数值函数 $f$，使得 $M(|f|^p)$ 是*有限*。显然，如果$g$是函数，属于到$\mathscr{F}^p(X, M)$，并且如果$|f| \leq |g|$，那么$f$也是属于到$\mathscr{F}^p(X, M)$；这个注和Minkowski的不等式表明$\mathscr{F}^p(X, M)$中的两个函数中的和也属于到这个集合；考虑到$M$是正齐次的，因此我们看到$\mathscr{F}^p(X, M)$是$X$上定义的所有有限数值函数的空间$\mathbf{R}^X$的*线性子空间*。

对于每个数 $p > 0$ 以及在 $X$、集合上定义的每个有限数值函数 $f$

$$
N_p(f) = \left(M(|f|^p)\right)^{1/p};
$$

然后对于每个标量 $\lambda$ $N_p(\lambda f) = |\lambda| N_p(f)$；此外，如果 $p \geq 1$ 那么，根据 (7)，

$$
N_p(f+g) \leq N_p(f) + N_p(g),
$$

这证明 $N_p$ 是向量空间 $\mathscr{F}^p(X, M)$（TVS，II, §1）上的*半范数*。

**命题 4.** — *令$p$和$q$为两个实数$> 0$和集合$1/r = 1/p + 1/q$。对于 $X$ 上定义的任何有限数值函数 $f, g$，*

$$
N_r(fg) \leq N_p(f) N_q(g)
$$

*假设$N_p(f)$和$N_q(g)$是有限的。*

对于， 关系 (9) 可以写成

$$
M(|f|^r |g|^r) \leq (M(|f|^p))^{r/p} (M(|g|^q))^{r/q},
$$

这正是 Hölder 的不等式 (5) 应用于数 $\alpha = r/p$ 和 $\beta = r/q$ 以及函数 $|f|^p$ 和 $|g|^q$。

推论。 — *假设* $M(1) = 1$； *然后，对于每个有限数值函数* $f$ *定义在* $X$，*映射* $p \mapsto N_p(f)$ *是递增在* $]0, +\infty[$。

应用不等式 (9) 对于$g = 1$的情况，我们看到对于所有$q > 0$都有$N_r(f) \leq N_p(f)$；由于由$1/r = 1/p + 1/q$定义的数$r$会越过数的集合，因此当$q$会越过数$> 0$的集合时，$0 < r < p$，推论得证。

命题 5. — *对于每个有限数值函数* $f$ *定义在* $X$、*集合* $I$ *的值的* $1/p$ ($p > 0$) *这样* $N_p(f)$ *是有限要么是空要么是一个区间；如果* $I$ *不减少到点，则映射* $\alpha \mapsto \log N_{1/\alpha}(f)$ *要么在* $I$ *上凸，要么等于* $-\infty$ *在* $I$的内部。

令$r$和$s$是两个不同的数$> 0$，使得$1/r$和$1/s$属于到$I$；这一切都归结为证明如果

$$
\frac{1}{p} = \frac{t}{r} + \frac{1-t}{s},
$$

与$0 < t < 1$，则

$$
\log N_p(f) \leq t \cdot \log N_r(f) + (1-t) \log N_s(f),
$$

或者，结果是一样的，

$$
N_p(f) \leq (N_r(f))^t (N_s(f))^{1-t},
$$

关系可以由 $N_p$ 的定义写成

$$
M(|f|^p) \leq (M(|f|^r))^{tp/r} (M(|f|^s))^{(1-t)p/s}.
$$

设定$\alpha = tp/r$，我们有$1-\alpha = (1-t)p/s$乘以关系即定义$p$作为$t, r, s$的函数； 从而$p = \alpha r + (1-\alpha)s$。 Hölder 的不等式现在收益率

$$
M(|f|^{r\alpha}|f|^{s(1-\alpha)}) \leq (M(|f|^r))^{\alpha} (M(|f|^s))^{1-\alpha},
$$

这正是不等式 (12)。

习题

1) 根据No. 1的假设，证明X上有界函数的集合使得$M(|f|)$是有限的，是$\mathbf{R}^X$的子代数A，并且在函数上有界函数的集合 X使得$M(|f|) = 0$是A中的理想。此外，如果$M(1)$是有限的，则证明当A在X中配备一致收敛的拓扑时，映射$f \mapsto M(f)$是连续的。

2) 令X为$\mathbf{R}$的区间$[0, +\infty[$，S由在X上定义的函数形成的凸锥体，使得$0 \leq f(x) \leq kx$在X上（对于有限的数$k > 0$，取决于$f$）。 集合$M(f) = 0$对于$f \in S$，以及$M(f) = +\infty$对于每个正函数$f$定义在X而不是属于到S。证明$M$满足条件 No. 1，以及$M(x) = 0$和$M(x^r) = +\infty$，对于每个数$r > 0$不等于1。

3）给出例，其中X是集合，有两个元素，$N_p(\mathbf{x})$对于每个$p > 0$和每个$\mathbf{x} \in \mathbf{R}^2$都是有限的，但是如果存在$p$的值使得映射$p \mapsto N_p(\mathbf{x})$在这些点处不可微分。

4) 从几何平均值不等式推导出不等式 (6)

$$
z_1^{\alpha_1} z_2^{\alpha_2} \cdots z_n^{\alpha_n} \leq \alpha_1 z_1 + \cdots + \alpha_n z_n \quad \text{(where } \sum_{i=1}^n \alpha_i = 1 \text{)}
$$

（FRV，III, §1, No. 1，提案 2）。 （约化对于$M(f_i) = 1$代表$1 \leq i \leq n$的情况。）

5) 令$\alpha$为实数$> 1$并令$\beta = 1 - \alpha < 0$。令 $g$ 为有限函数，在 X 上定义，使得 $g(x) > 0$ 对于所有 $x \in X$ 且$M(g) > 0$；证明对于在 X 上定义的每个有限函数 $f \geq 0$ 使得 $M(f)$ 是有限的，

$$
M(f^\alpha g^\beta) \geq (M(f))^\alpha (M(g))^\beta
$$

（适当应用 Hölder 的不等式）。

6) 从 Hölder 的不等式推导出 Minkowski 的不等式（在 Hölder 的不等式的帮助下找到 $M((f+g)^{p-1})$ 的上界）。如果假设定义了函数 $f, g$ 中的每一个对 $M(f+g) = M(f) + M(g)$ 以及$X$ 上的 $\geq 0$，则可以从 Exer 中进行类似的推导。 5 不等式

$$
(M((f+g)^p))^{1/p} \geq (M(f^p))^{1/p} + (M(g^p))^{1/p}
$$

在以下情况下：

a) $0 < p < 1$、$f$和$g$有限函数$\geq 0$定义在$X$上，使得$f(x) + g(x) > 0$对于所有$x \in X$并且使得$M(f^p)$和$M(g^p)$是有限的；

b) $p < 0$、$f$和$g$有限函数定义在$X$上，使得$f(x) > 0$和$g(x) > 0$对于所有$x \in X$、$M(f^p)$和$M(g^p)$都是有限的，并且$M((f+g)^p) > 0$。
