---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 3
section_title: The Hahn-Banach Theorem (analytic form)
lang: zh
source: evt-i-v
book_pages: TVS II.21-TVS II.23, TVS II.72-TVS II.74
pdf_pages: 0058-0060, 0109-0111
extraction: ocr
subsections:
    - "no": 1
      title: Extension of positive linear forms
      page: 21
      pdf_page: 58
    - "no": 2
      title: The Hahn-Banach theorem (analytic form)
      page: 22
      pdf_page: 59
statements: 6
exercises: 8
content_sha256: 74c83b37e8464ab2930eb5b903399b296eb6e232a19632be352917cfe2a3419d
translated_from: content/en/evt/II/03_s3_the_hahn_banach_theorem_analytic_form.md
translation_method: google
source_content_sha256: 62f888c305293cb384c8f41fb0d8824e2a25c39637bd4054f2e1ce6efe281846
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 802d2c7a703a227799429b1beb3cea8c443271353f103f115cde4793e639faa1
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 3。哈恩-巴纳赫定理（分析形式）

### 1. 扩张正线性形式

#### 命题 1 {#evt-ii-s3-prop-1 .statement tag=07DQ}

— 令 E 为预定的向量空间，V 为 E 的向量子空间，使得 E 的每个元素都以 V 的元素为界。给定 V 上的线性形式 f 对于 V 的预序向量空间结构为正（由 E 引起），则存在 E 上正线性形式的非空集合 $S_f$，每个集合都是 f 的扩张。如果 $h \in S_f$ 则 $a \in E$ 的值 $h(a)$ 位于区间 $[\alpha', \alpha'']$ 内，其中

$$
\alpha' = \sup_{z \in V, z \leq a} f(z), \quad \alpha'' = \inf_{y \in V, y \geq a} f(y).
$$

I。特例。

首先假设$E = V + \mathbf{R}a$。由于如果 $a \in V$ 则命题是微不足道的，因此我们将自己限制在$a \notin V$ 的情况。 V上的条件意味着$y \in V$的集合$A''$使得$a \leq y$不为空；类似地，$z \in V$的集合$A'$使得$-z \geq -a$（\emph{即}$z \leq a$）不为空。对于$y \in A''$和$z \in A'$，我们有$z \leq a \leq y$，因此有假设$f(z) \leq f(y)$。因此$\alpha', \alpha''$是有限的并且$\alpha' \leq \alpha''$。 E 上的任何线性形式 $f_1$ 扩展 $f$ 完全由 $f_1(a)$ 决定，并且对于所有 $\lambda \in \mathbf{R}$ 和所有 $x \in V$，我们有

$$
f_1(x + \lambda a) = f(x) + \lambda f_1(a).
$$

因此 $f_1$ 为正当且仅当关系

$$
x \in V, \quad \lambda \in \mathbf{R}, \quad x + \lambda a \geq 0
$$

暗示

$$
f(x) + \lambda f_1(a) \geq 0.
$$

由于$f(\mu x) = \mu f(x)$和关系、$x \geq 0$和$\mu x \geq 0$对于$\mu > 0$是等价的，因此在特定情况下$\lambda = 0, \lambda = 1$和$\lambda = -1$足以证明(2)蕴涵(3)。对于 $\lambda = 0$，(2) 暗示 (3) 的事实是从假设得出 $f$ 是正数。对于$\lambda = 1$，说(2)意味着(3)意味着对于$-x \in A'$，我们有$f_1(a) \geq f(-x)$，\emph{即}$f_1(a) \geq \alpha'$；对于$\lambda = -1$，(2)意味着(3)，意味着对于$x \in A''$，我们有$f(x) \geq f_1(a)$，\emph{即}$f_1(a) \leq \alpha''$。因此在这种情况下命题得证。

II。一般情况。

令 $\mathfrak{F}$ 为对 $(W, g)$ 的集合，其中 $W$ 为 $E$ 包含 $V$ 的向量子空间，$g$ 为线性形式的正值$W$ 是 $f$ 的扩张。如果$W \subset W'$并且如果$g'$是$g$的扩张，我们将阶$\mathfrak{F}$放入$(W, g) \leq (W', g')$。显然 $\mathfrak{F}$ 是归纳性的并且由 th 组成。 S的2个，III, § 2.4，有极大元素$(W_0, g_0)$。假设$W_0 \neq E$。那么存在向量$b \notin W_0$，并且，如果$W_1 = W_0 + \mathbf{R}b$，上面的特殊情况表明$W_1$上存在正线性形式，即$g_0$的扩张；这个与……矛盾假设 $(W_0, g_0)$ 是最大的。这样$W_0 = E$，命题的第一个部分就被证明了。当$a \in V$时，第二个断言显然与$\alpha' = \alpha'' = f(a)$成立；相反，如果 $a \notin V$ 并且有人放入 $V_1 = V + \mathbf{R}a$，则第二个断言由证明的特殊情况 I 得出。

#### 推论{#evt-ii-s3-n1-cor-1 .statement tag=07DR}

在具有兼容的预序结构的拓扑向量空间$E$中，令$P$为$E$中元素$\geq 0$的集合。设$V$为$E$包含的向量子空间，$P$的至少一个内部点$x_0$。那么$V$上的每个正线性形式都可以扩展到$E$上的正线性形式。

通过道具。 1 足以证明对于每个$x \in E$，都存在$x' \in V$使得$x' - x \in P$。 现在让$U$是$E$中$0$的邻域，使得$x_0 + U \subset P$。 Then $x + x_0 + U \subset x + P$, and, hence there exists $\varepsilon$ such that $0 < \varepsilon < 1$ and the point $y = x_0 + (1 - \varepsilon)x$ belongs to $x + P$; then every point of the form $x + \lambda(y - x)$ belongs to $x + P$ for $\lambda > 0$. 如果我们取$\lambda = 1/\varepsilon$，则$x + \lambda(y - x) = \lambda x_0 \in V$，由此得出结论。

The conclusion of the corollary is not necessarily valid if one does not assume that $V$ 包含 an interior 点 of $P$, even if $E$ is of 有限维 and if $P \cap V$ 包含点 interior in $V$ （II，p. 91，练习 25，b））。

### 2. Hahn-Banach 定理（解析形式）

#### 定理 1（哈恩-巴纳赫）{#evt-ii-s3-thm-1 .statement tag=07DS}

设$p$是向量空间$E$上的次线性函数。令$V$为$E$和$f$线性形式在$V$上的向量子空间，这样，对于所有$y \in V$，我们有$f(y) \leq p(y)$。那么$E$上存在线性形式$h$，即$f$的扩张，并且$h(x) \leq p(x)$对应$x \in E$。

对 $(x, a)$的集合，使得$p(x) \leq a$是向量空间$E_1 = E \times \mathbf{R}$的凸子集$P$（II，p. 17，道具19），并且它显然是一个尖锥体。对于每个点$(y, a) \in V_1$，令$V_1$为$E_1$和$g(y, a) = -f(y) + a$的子空间$V \times \mathbf{R}$。那么$g$是由$P \cap V_1$定义的$V_1$上预序结构的正线性形式；因为如果$(y, a) \in P \cap V_1$，则$a \geq p(y) \geq f(y)$，因此$g(y, a) \geq 0$。接下来让$(x, a) \in E_1$；我们证明对于由$P$定义的预序，$(x, a)$小于$V_1$的点。如果$(x', a') \in V_1$则$(x, a) \leq (x', a')$当且仅当$p(x' - x) \leq a' - a$，取$a' \geq p(-x) + a$，我们看到$V_1$的$(0, a')$满足要求。因此我们可以应用 prop. II、p. 21中的I；在$E_1$上有线性形式$u$延伸$g$，并且预序由$P$定义为正。因此，$u(0, 1) = g(0, 1) = 1$和$u$是形式$u(x, a) = -h(x) + a$，其中$h$是$E$上的线性形式，即扩展$f$；此外，对于所有$x \in E$和所有$a \geq p(x)$，我们有$h(x) \leq a$，因此$h(x) \leq p(x)$。 Q.E.D.

#### 推论 1 {#evt-ii-s3-thm-1-cor-1 .statement tag=07DT}

— 设 $p$ 为向量空间 $E$ 的半范数。令$V$为$E$和$f$线性形式在$V$上的向量子空间，使得$|f(y)| \leq p(y)$对于所有$y \in V$。那么在$E$上存在定义的线性形式$h$，它是$f$的扩张，并且$|h(x)| \leq p(x)$对于$x \in E$。

对于$E$上的半范数$q$和线性形式$g$，关系$g \leq q$与$|g| \leq q$相同。推论如下。 1.

#### 推论 2 {#evt-ii-s3-thm-1-cor-2 .statement tag=07DU}

— 设$p$为向量空间$E$的半范数。给定点$x_0 \in E$，存在在$E$上定义的线性形式$f$，使得$f(x_0) = p(x_0)$和$|f(x)| \leq p(x)$适用于所有$x \in E$。

应用cor。 1 到向量子空间、$V$，由 $x_0$ 生成，并到线性形式 $\xi x_0 \mapsto \xi p(x_0)$ 在 $V$ 上定义。

#### 推论 3 {#evt-ii-s3-thm-1-cor-3 .statement tag=07DV}

— 令$V$为范数空间$E$的向量子空间，并令$f$为$V$上的连续线性形式；则存在在 $E$ 上定义的连续线性形式 $h$，其中扩展 $f$ 且具有相同的范数 (GT, X, § 3.2)。

应用cor。 1、取$p(x) = \|f\| \cdot \|x\|$，得到$\|h\| \leq \|f\|$；但显然 $\|h\| \geq \|f\|$，推论如下。

Cor的结论。 3 不一定适用于将范数空间连续线性映射转化为任意范数空间（IV，p. 55，exerc.16，c）和V，p. 65，exerc。 22）。

### 习题 {#evt-ii-s3-exercises}

参见[习题为 § 3](exercises/s3/)。
