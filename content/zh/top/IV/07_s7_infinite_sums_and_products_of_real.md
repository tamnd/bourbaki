---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 7
section_title: Infinite sums and products of real numbers
lang: zh
source: top-i-iv
book_pages: 363-372, 397-401
pdf_pages: 0369-0378, 0403-0407
extraction: ocr
subsections:
    - "no": 1
      title: FAMILIES OF POSITIVE FINITE NUMBERS SUMMABLE IN $\mathbf{R}$
      page: 364
      pdf_page: 370
    - "no": 2
      title: FAMILIES OF FINITE NUMBERS OF ARBITRARY SIGN SUMMABLE IN $\mathbf{R}$
      page: 366
      pdf_page: 372
    - "no": 3
      title: PRODUCT OF TWO INFINITE SUMS
      page: 367
      pdf_page: 373
    - "no": 4
      title: FAMILIES MULTIPLIABLE IN $\mathbf{R}^*$
      page: 367
      pdf_page: 373
    - "no": 5
      title: SUMMABLE FAMILIES AND MULTIPLIABLE FAMILIES IN $\overline{\mathbf{R}}$
      page: 369
      pdf_page: 375
    - "no": 6
      title: INFINITE SERIES AND INFINITE PRODUCTS OF REAL NUMBERS
      page: 370
      pdf_page: 376
statements: 20
exercises: 22
content_sha256: 914b6fddb31d783e4e0e15c113245391dec6cb0c420de82a4dd12a0c160fbd97
translated_from: content/en/top/IV/07_s7_infinite_sums_and_products_of_real.md
translation_method: google
source_content_sha256: 455d0ffdcd364c6ed9f0b7d02c710c2c2c96a2ff460df4ccbbd8a2f0e2e71d59
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: f5de6764c804278321e4064c2a2425ed385b6791bb65ac77bffd615a0ad25e8c
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 7. 和和乘积实数

由于$\mathbf{R}$的每个点都有邻域的*可数*基本系统（§ 1, no. 4，命题3的推论），因此，只有当*有限*实数的族$(x_t)$在$\mathbf{R}$中可求和时， 集合的指标 t，使得 $x_t \neq 0$ 是*可数*（章 III, § 5, no. 2，命题 1 的推论）。 $\mathbf{R}$中可求和族的研究因此约化本质上是对可求和*序列*的研究。然而，我们稍后必须考虑有限实数的不可数族$(x_t)$，其项是参数$t$的函数；有可能这个族对于所有 $t$ 都是可求和的，但是指标 $i$ 的（可数）集合使得 $x_i \neq 0$ 取决于 $t$。因此，下文中我们不会对指标集合中的幂强加任何假设。

### 1. 可在 $\mathbf{R}$ 中求和的正有限数族

#### 定理 1 {#top-iv-s7-thm-1 .statement tag=0BT9}

*族* $(x_i)$ *有限实数* $\geqslant 0$ *可求和于* $\mathbf{R}$ *当且仅当族的部分有限和的集合上界于* $\mathbf{R}$。 *如果是这样，这个集合中最小的上界是家庭的和*$(x_i)$。

对于指标集合 $I$ 中的每个有限子集 $H$，令 $s_H = \sum_{i \in H} x_i$；由于$x_i$是$\geqslant 0$，关系$H \subset H'$意味着$s_H \leqslant s_{H'}$。其它字、映射$H \to s_H$是$I$的有限子集有向集合$\mathfrak{F}(I)$*递增*函数；因此（§ 5, no. 2，定理 2 的推论）当且仅当它*有界*时，它才有有限的极限。

#### 注 {#top-iv-s7-n1-rem-1 .statement tag=0BTA}

令$(H_\lambda)$是$I$的有限子集的族，使得对于$I$的每个有限子集$H$，有指标$\lambda$使得$H \subset H_\lambda$；那么 $(x_i)$ 是可求和的当且仅当 $s_{H_\lambda}$ 的族在 $\mathbf{R}$ 中*上界*。特别地，令$(x_n)$为有限实数$\geqslant 0$的序列，并且对于每个整数$n$令$s_n = \sum_{p=0}^n x_p$；那么序列 $(x_n)$ 在 $\mathbf{R}$ 中可求和当且仅当，对于严格递增的整数 $(n_k)$ 的*一个序列*，部分序列 $(s_{n_k})$ 的*上界*为$\mathbf{R}$。

#### 例 {#top-iv-s7-n1-exa-4 .statement tag=0EAD}

1) 对于每个数$q$，使得$0 \leqslant q < 1$、序列$(q^n)$（“比率$q$的几何级数”）可在$\mathbf{R}$中求和，因为
$$
s_n = \frac{1 - q^{n+1}}{1 - q} \leqslant \frac{1}{1 - q}
$$
这个序列中的和是$\lim_{n \to \infty} s_n = \frac{1}{1 - q}$。

2) 设$a$和$b$是两个数，使得$0 \leqslant a < 1$和$0 \leqslant b < 1$；那么族$(a^m b^n)_{(m, n) \in \mathbf{N} \times \mathbf{N}}$可在$\mathbf{R}$中求和。对于$\mathbf{N} \times \mathbf{N}$的每个有限子集都包含在形式$[0, p] \times [0, p]$的子集中，我们有
$$
\sum_{m=0}^p \sum_{n=0}^p a^m b^n = \left( \sum_{m=0}^p a^m \right) \left( \sum_{n=0}^p b^n \right) = \frac{1 - a^{p+1}}{1 - a} \cdot \frac{1 - b^{p+1}}{1 - b} \leqslant \frac{1}{(1 - a)(1 - b)}.
$$

3) 对于每个整数 $p > 1$，序列 $(n^{-p})$ ($n > 0$) 是可求和的，因为
$$
s_{2^n + 1} - s_{2^n} = \sum_{k=1}^{2^n} (2^n + k)^{-p} < 2^n \cdot (2^n)^{-p}
$$
因此，将这些不等式加在一起，
$$
s_{2^n} < \frac{1}{1 - 2^{1-p}}.
$$

4) 序列 $(1/n)$ ($n > 0$) 不可在 $\mathbf{R}$ 中求和，因为
$$
s_{2^{n+1}} - s_{2^n} = \sum_{k=1}^{2^n} \frac{1}{2^n + k} > \frac{2^n}{2^{n+1}} = \frac{1}{2}
$$
因此，将这些不等式加在一起，
$$
s_{2^n} > n/2
$$
从而不满足定理 1 的标准。

5) 设$(I_n)$为互为不相交的非空开区间的序列，所有开区间都包含在有限长度$l$区间内。该族的有限区间数的长度和为$\leq l$($§ 1$，no. 5)，因此$I_n$的长度族可在$\mathbf{R}$中求和，其和为$\leq l$。

#### 定理 2（比较的原理）{#top-iv-s7-thm-2 .statement tag=0BTB}

*让*$(x_i)_{i \in I}$*和*$(y_i)_{i \in I}$*成为有限实数*$\geq 0$的两个族，*使得*$x_i \leq y_i$*对于所有*$i$。 *如果* $(y_i)$ *可求和于* $\mathbf{R}$ *那么也可以* $(x_i)$，*我们有* $\sum_i x_i \leq \sum_i y_i$； *如果在加法中有指标*$x$*使得*$x_x < y_x$，*那么*$\sum_i x_i < \sum_i y_i$。

假设意味着，
$$
\sum_{i \in H} x_i \leq \sum_{i \in H} y_i,
$$
for every 有限子集 $H$ of $I$ and the first 部分 of 定理 follows from this; 不等式 relating 和 follows from 原理 of 扩张 of inequalities ($§ 5$, no. 2, 定理 1).如果$x_x < y_x$，那么
$$
\sum_i x_i = x_x + \sum_{i \neq x} x_i < y_x + \sum_{i \neq x} y_i = \sum_i y_i.
$$

这个定理提供了最常用的标准来决定实数$\geq 0$的序列$(x_n)$在$\mathbf{R}$中是否可求和：我们尝试将给定的序列与一个更简单的序列$(y_n)$进行“比较”，其中我们已经知道它是否可求和。 如果存在有限的数$a > 0$，使得$x_n \leq a y_n$对于从某个点开始的所有$n$来说，并且如果$(y_n)$是可求和的，则$(x_n)$是可求和的；另一方面，如果存在有限的数$b > 0$，使得$x_n \geq b y_n$对于从某个点开始的所有$n$，并且如果$(y_n)$在$\mathbf{R}$中不可求和，则$(x_n)$在$\mathbf{R}$中不可求和。 我们将在后面的卷中看到如何在最常出现的情况下获得这种比较序列。

#### 例 1 {#top-iv-s7-n1-exa-1 .statement tag=0BTC}

令$a$为有限实数$> 0$，并考虑序列$\left( \frac{a^n}{n!} \right)$；令$n_0$为最小的整数，使得$a < n_0$。那么对于每个 $n \geq n_0$ 我们有
$$
\frac{a^n}{n!} \leq \frac{a^{n_0}}{n_0!} \cdot \left( \frac{a}{n_0} \right)^{n-n_0};
$$
因为 $q = \frac{a}{n_0} < 1$、序列 $(q^{n-n_0})$ 是可求和的，因此序列 $\left( \frac{a^n}{n!} \right)$ 也是可求和的。

#### 例 2 {#top-iv-s7-n1-exa-2 .statement tag=0BTD}

令 $(a_n)$ 为正数的可和序列。自从
$$
\lim_{n \to \infty} a_n = 0,
$$
存在整数$n_0$，只要$n \geq n_0$就有$a_n \leq 1$。因而，对于每个 $n \geq n_0$，我们有 $a_n^2 \leq a_n$，因此序列 $(a_n^2)$ 可在 $\mathbf{R}$ 中求和。每个整数 $p > 1$ 的序列 $(a_n^p)$ 也是如此。

#### 例 3 {#top-iv-s7-n1-exa-3 .statement tag=0BTE}

设$a$和$b$为两个数$< 1$；那么
$$
\frac{1}{a^m + b^n} \leq \frac{1}{2(\sqrt{a})^m (\sqrt{b})^n}
$$
因而，族 $\left( \frac{1}{a^m + b^n} \right)$ 可在 $\mathbf{R}$ 中求和。

#### 推论{#top-iv-s7-n1-cor-1 .statement tag=0BTF}

*设* $(x_i)_{i \in I}$ *为有限数* $\geq 0$ *在* $\mathbf{R}$ 中的可求和族。 *如果*$H$*是*$I$中的任何子集，*我们有*
$$
\sum_{i \in H} x_i \leq \sum_{i \in I} x_i,
$$
*并且等式仅在*$x_i = 0$*对于所有*$i \in \complement H$成立。

### 2. $\mathbf{R}$ 中可求和的任意符号的有限数族

#### 定理 3 {#top-iv-s7-thm-3 .statement tag=0BTG}

*设* $(x_i)_{i \in I}$ *为有限实数族；那么下面的叙述是等价的*：

a) *家庭* $(x_i)$ *可总结为* $\mathbf{R}$。
b) *家庭* $(|x_i|)$ *可总结为* $\mathbf{R}$。
c) 族的有限部分和的*集合*$(x_i)$*限制在*$\mathbf{R}$。

令$I_1$ *为所有* $i \in I$ *中的集合，使得* $x_i \geq 0$，*和* $I_2$ *集合中的所有* $i \in I$ *使得* $x_i < 0$。 *家庭* $(x_i)_{i \in I}$ *[分别。 $(|x_i|)_{i \in I}$] *可求和当且仅当每个族* $(x_i)_{i \in I_1}$ *和* $(x_i)_{i \in I_2}$ *[分别。 $(|x_i|)_{i \in I_1}$ 和 $(|x_i|)_{i \in I_2}$] *可求和*（章 III, § 5, no. 3、命题 2 和 3）。 *现在说* $(x_i)_{i \in I_1}$ *是可求和的，或者* $(|x_i|)_{i \in I_1}$ *是可求和的，或者*族$(x_i)_{i \in I_1}$的有限部分和的集合是有界的（no. 1，定理 1）；将$I_1$替换为$I_2$也是如此。 定理紧随其后。

定理 3 表明，有限实数族的$\mathbf{R}$中的可求和性仅取决于其绝对值族的可和性。

我们回想一下（章III, § 5, no. 5，命题6），如果$(x_i)$和$(y_i)$是有限实数的两个可求和族，那么$(x_i + y_i)$族是可求和的并且$\sum (x_i + y_i) = \sum x_i + \sum y_i$。此外，如果$(x_i)$是有限实数的可和族，并且$a$是任何有限实数，则$(ax_i)$族在$\mathbf{R}$中可求和，并且我们有$\sum ax_i = a \cdot \sum x_i$。

### 3. 两个无穷和的乘积

#### 命题 1 {#top-iv-s7-prop-1 .statement tag=0BTH}

*如果有限实数的族* $(x_\lambda)_{\lambda \in L}$ *和* $(y_\mu)_{\mu \in M}$ *可在* $\mathbf{R}$ 中求和，*那么族* $(x_\lambda y_\mu)_{(\lambda, \mu) \in L \times M}$ *也是如此，我们有*

(1)
$$
\sum_{(\lambda, \mu) \in L \times M} x_\lambda y_\mu = (\sum_{\lambda \in L} x_\lambda) (\sum_{\mu \in M} y_\mu).
$$

$L \times M$的每个有限子集都包含在形式$H \times K$的有限子集中，其中$H$是$L$的有限子集，$K$是$M$的有限子集。到假设，存在数$a > 0$，使得$L$和$M$的所有有限子集$H$和$K$分别有$\sum_{\lambda \in H} |x_\lambda| \leq a$和$\sum_{\mu \in K} |y_\mu| \leq a$；因此
$$
\sum_{(\lambda, \mu) \in H \times K} |x_\lambda y_\mu| = (\sum_{\lambda \in H} |x_\lambda|) (\sum_{\mu \in K} |y_\mu|) \leq a^2,
$$
这表明族$(x_\lambda y_\mu)$可以在$\mathbf{R}$中通过定理1和3求和。通过结合性我们可以写出[章III, § 5, no. 3,公式(2)]
$$
\sum_{(\lambda, \mu) \in L \times M} x_\lambda y_\mu = \sum_{\lambda \in L} (\sum_{\mu \in M} x_\lambda y_\mu) = \sum_{\lambda \in L} x_\lambda (\sum_{\mu \in M} y_\mu) = (\sum_{\lambda \in L} x_\lambda) (\sum_{\mu \in M} y_\mu);
$$
因此结果。

### 4. $\mathbf{R}^*$ 中的家庭可乘

在有限非零实数的乘法群$\mathbf{R}^*$中，仅当$\lim x_i = 1$相对于$I$的有限子集补集过滤器时$(x_i)_{i \in I}$才可以相乘（章III, § 5, no. 2，命题） 1）。特别是，只能存在指标$i$的*有限*数，使得$x_i < 0$。因此，我们可以自己极限只考虑$x_i$所有项严格为正的家庭；然后方便地放置$x_i = 1 + u_i$，其中$u_i$对于所有$i$服从不等式$-1 < u_i < +\infty$。由于$\mathbf{R}^*$的每个点都有邻域的可数基数系统，指标$i$的集合，使得$u_i \neq 0$是可数的，如果族$(1 + u_i)$可乘$\mathbf{R}^*$。

#### 定理 4 {#top-iv-s7-thm-4 .statement tag=0BTI}

*家庭* $(1 + u_i)$ *可乘于* $\mathbf{R}^*$ *当且仅当家庭* $(u_i)$ *可求和于* $\mathbf{R}$。
#### 引理（一）{#top-iv-s7-n4-lem-1 .statement tag=0BTJ}

*如果*$(a_i)_{1 \leq i \leq p}$*是数*$> 0$中的有限序列，*那么*
$$
\prod_{i=1}^p (1 + a_i) \geq 1 + \sum_{i=1}^p a_i.
$$
(ii) *如果也* $a_i < 1$ *对于每个* $i$，*那么*
$$
\prod_{i=1}^p (1 - a_i) \geq 1 - \sum_{i=1}^p a_i.
$$

如果$p = 1$，这些不等式是明确的，并由$p$上的归纳证明。如果
$$
\prod_{i=1}^{p-1} (1 + a_i) \geq 1 + \sum_{i=1}^{p-1} a_i,
$$
我们有
$$
\prod_{i=1}^p (1 + a_i) \geq (1 + a_p) \left( 1 + \sum_{i=1}^{p-1} a_i \right) = 1 + \sum_{i=1}^p a_i + a_p \cdot \sum_{i=1}^{p-1} a_i \geq 1 + \sum_{i=1}^p a_i.
$$
再说一次，如果
$$
\prod_{i=1}^{p-1} (1 - a_i) \geq 1 - \sum_{i=1}^{p-1} a_i,
$$
我们有
$$
\prod_{i=1}^p (1 - a_i) \geq (1 - a_p) \left( 1 - \sum_{i=1}^{p-1} a_i \right) = 1 - \sum_{i=1}^p a_i + a_p \cdot \sum_{i=1}^{p-1} a_i \geq 1 - \sum_{i=1}^p a_i.
$$

证明引理后，我们注如果族$(1 + u_i)$是可乘的，那么族$(1 + u_i^+)$和$(1 - u_i^-)$也是可乘的，因为$\mathbf{R}^*$是完整的群（章III, § 5, no. 3，命题2）；相反，如果族$(1 + u_i^+)$和$(1 - u_i^-)$是可乘的，那么$(1 + u_i)$也是可乘的（章III, § 5, no. 3，命题3）。因此，我们只需要考虑所有$u_i$都是$\geq 0$以及它们都是$\geq 0$的情况。

首先假设 $u_i \geq 0$ 对于所有$i$。如果族$(1 + u_i)$是可乘的，那么对于每个$\varepsilon > 0$，$I$中有指标集合的有限子集$J$，这样，对于$I$不相交的的每个有限子集$H$ $J$，我们有$1 \leq \prod_{i \in H} (1 + u_i) \leq 1 + \varepsilon$；由(2)得出$\sum_{i \in H} u_i \leq \varepsilon$，这表明根据柯西准则(章III, § 5, no. 2，定理1)，$(u_i)$可在$\mathbf{R}$中求和。

相反，假设 $(u_i)$ 可在 $\mathbf{R}$ 中求和。对于每个$\varepsilon$，使得$0 < \varepsilon < 1$，有$I$的有限子集$J$，这样，对于来自$J$的$I$不相交的的每个有限子集$H$，我们有$0 \leq \sum_{i \in H} u_i \leq \varepsilon$。根据(3)，我们有 $\prod_{i \in H} (1 - u_i) \geq 1 - \varepsilon$；但由于$1 + u \leq \frac{1}{1 - u}$对于每个数$u$使得$0 \leq u < 1$，因此

$$
1 \leq \prod_{i \in H} (1 + u_i) \leq \frac{1}{1 - \varepsilon},
$$

这表明 $(1 + u_i)$ 是可乘的（柯西准则）。

当所有$u_i$都是$\leq 0$时，证明类似。要证明如果 $(1 + u_i)$ 可乘，$(u_i)$ 是可求和的，请使用公式 (2) 和不等式 $1 - u \leq \frac{1}{1 + u}$ ($0 \leq u < 1$)；要证明如果 $(u_i)$ 可求和，$(1 + u_i)$ 是可乘的，请使用公式 (3)。

在章V（§ 4）中，群$\mathbf{R}^*$的拓扑研究将使我们能够借助对数函数给出$\mathbf{R}^*$中族可乘性的另一个准则；在下一卷中，我们将利用对数的微分性质，将这一标准与上述标准建立等价。

### 5. $\overline{\mathbf{R}}$ 中的可求族和可乘族

在$\overline{\mathbf{R}}$的区间$[0, + \infty]$上，加法是合成(§ 4, no. 3)的结合律和交换律律；因此，在此区间内定义了数的*可求和*族的概念（章III, § 5, no. 1，注3）。

#### 命题 2 {#top-iv-s7-prop-2 .statement tag=0BTK}

*每个家庭* $(x_i)$ *实数* $\geq 0$ *可在* $\overline{\mathbf{R}}$ 中求和。

对于有向集合$\mathfrak{F}(I)$到$\overline{\mathbf{R}}$的映射$H \to s_H$是*递增*；因此 (§ 5, no. 2, 定理 2) 有极限。

同样的推理表明实数$\leq 0$的每个族都可以在$\overline{\mathbf{R}}$中求和。

类似地，乘法是合成在 $[0, 1]$ 和 $[1, + \infty]$ $\overline{\mathbf{R}}$ 上的结合律和交换律律，因此可乘族的概念是在这些间隔中的每一个上定义的。

#### 命题 3 {#top-iv-s7-prop-3 .statement tag=0BTL}

每个家庭$(1 + u_i)$ [分别。 数 $\geq 1$（分别为$\geq 0$和$\leq 1$）的$(1 - u_i)$]可与$\overline{\mathbf{R}}$相乘。

与命题 2 相同的证明。

#### 推论{#top-iv-s7-n5-cor-1 .statement tag=0BTM}

乘积 $\prod (1 + u_i)$ [分别。 数 $\geq 1$（分别为 $> 0$ 和 $\leq 1$）的 $\prod (1 - u_i)$] 等于 $+ \infty$（分别为 0）当且仅当 $\sum u_i = + \infty$。

因为如果 $\sum u_i$ 是有限的，则 $\prod (1 + u_i)$ 和 $\prod (1 - u_i)$ 在 $\mathbf{R}^*$ 中，反之亦然（no. 4，定理 4）。

#### 注 {#top-iv-s7-n5-rem-1 .statement tag=0BTN}

当 G 被 $\overline{\mathbf{R}}$ 替换并且假设 $x_i$ 为 $\geq 0$ 时，结合性的定理（章 III, § 5, no. 3，定理 2）仍然有效。如果 $\sum_{i \in I} x_i$ 是有限的，这很清楚。相反，假设$\sum_{i \in I} x_i = + \infty$。那么对于每个有限的$a > 0$，都有I的有限子集 H，使得$\sum_{i \in H} x_i \geq a$。令 K 为 L 的有限子集，使得 $H \subset \bigcup_{\lambda \in K} I_\lambda$；那么从$s_\lambda \geq \sum_{i \in I_\lambda \cap H} x_i$开始，对于所有$\lambda \in K$，我们有
$$
\sum_{\lambda \in K} s_\lambda \geq \sum_{i \in H} x_i \geq a,
$$
这表明$\sum_{\lambda \in L} s_\lambda = + \infty$。我们留给读者的任务是在$[0, 1]$或$[1, + \infty]$中为数的可乘族制定类似的命题。

### 6. 无限级数和无限乘积 OF 实数

有限实数的级数如果在$\mathbf{R}$收敛，则简单地说是收敛的。

#### 定义 1 {#top-iv-s7-def-1 .statement tag=0BTO}

如果项的绝对值的级数收敛，则有限实数的级数被称为绝对收敛。

#### 命题 4 {#top-iv-s7-prop-4 .statement tag=0BTP}

有限实数的级数是可交换收敛的当且仅当它绝对收敛。

这是从章 III, § 5, no. 7、命题 9 和定理 3 of no. 2 得出的。

在其他字中，如果$(u_n)$是有限实数的序列，那么说级数（其一般项是$u_n$）是交换收敛的，或者说它是绝对收敛的，或者说序列是同样的事情$(u_n)$ 可在 $\mathbf{R}$ 中求和。因此，章III, § 5证明的可求和族的所有性质都适用于绝对收敛级数。特别是，如果项为 $u_n$ 的级数绝对收敛，则对于 $\mathbf{N}$ 的所有子集 $H$ 都存在和 $\sum_{n \in H} u_n$；并且，如果 $(H_p)$ 是 $\mathbf{N}$ 的划分，我们有
$$
\sum_{n=0}^{\infty} u_n = \sum_p \left( \sum_{n \in H_p} u_n \right)
$$
*（绝对收敛级数的结合性*）。

正如我们在章III, § 5中已经说过的，实数的级数可以收敛，但无需交换收敛，即不绝对收敛。

#### 例 {#top-iv-s7-n6-exa-1 .statement tag=0BTQ}

*交错的级数。* 由有限实数的序列 $(u_n)$ 定义的级数称为 *交错的* 如果 $u_n = (-1)^n v_n$，其中 $v_n \geq 0$ 对于所有 $n$。让我们证明，对于这样的级数的收敛来说，*足够* 条件是 *序列* $(v_n)$ *减少并具有* 0 *作为其极限*。对于如果 $s_n$ 表示
$$
\sum_{p=0}^{n} u_p,
$$
假设 $(v_n)$ 是递减意味着
$$
s_{2n+1} \leq s_{2n+3} \leq s_{2n+2} \leq s_{2n}
$$
对于所有$n \geq 0$。 序列 $(s_{2n})$ [分别。 $(s_{2n+1})$] 是递减且有界于下方（分别为递增且界于上方），因此具有有限的极限 $a$（分别为 $b$）和 $b \leq a$；自从
$$
a - b = \lim_{n \to \infty} (s_{2n} - s_{2n+1}) = \lim_{n \to \infty} v_{2n+1} = 0,
$$
断言得证。

如果我们取例$v_n = 1/n$，则满足上面的条件，因此级数其通项为$(-1)^n / n$（“交错的谐波级数”）是收敛的。我们在no. 1中看到，级数的通项为$1/n$（“调和级数”）是不收敛的，因此交错的调和级数不是绝对收敛的。

我们记得（章III, § 5, no. 6，命题7），如果$(u_n)$和$(v_n)$是有限实数的两个收敛的级数，那么级数$(u_n + v_n)$收敛，并且
$$
\sum_{n=0}^{\infty} (u_n + v_n) = \sum_{n=0}^{\infty} u_n + \sum_{n=0}^{\infty} v_n;
$$
另外，如果级数 $(u_n)$ 收敛，则级数 $(au_n)$ 对于所有有限实数 $a$ 和 $\sum_{n=0}^{\infty} au_n = a \cdot \sum_{n=0}^{\infty} u_n$ 是收敛的。

最后，如果级数$(u_n)$和$(v_n)$收敛，并且如果$u_n \leq v_n$对于所有$n$，我们有$\sum_{n=0}^{\infty} u_n \leq \sum_{n=0}^{\infty} v_n$乘原理的扩张不等式（§ 5, no. 2，定理） 1）。

需要注意的是，如果我们假设级数$(v_n)$收敛但不是绝对收敛，并且如果$|u_n| \leq |v_n|$对于每个$n$，我们绝不能推断级数$(u_n)$是收敛的，正如取$u_n = |v_n|$所见。

有限非零实数的无限乘积如果收敛于 $\mathbf{R}^*$，则简单地说它是收敛的；那么它的值就是一个有限的非零实数。

#### 定义 2 {#top-iv-s7-def-2 .statement tag=0BTR}

*如果一般因子为$1 + |u_n|$的乘积收敛，则称其广义因子为$1 + u_n$的无穷乘积绝对收敛。*

#### 命题 5 {#top-iv-s7-prop-5 .statement tag=0BTS}

*有限实数的无限乘积可交换收敛当且仅当它绝对收敛。*

这是从上面的章 III, § 5, no. 7、命题 9 和定理 4 得出的。

此外，当且仅当其一般因子为$1 + u_n$的乘积*绝对收敛*，当且仅当其一般项为$u_n$的级数*绝对收敛*。

非零实数的乘积可以收敛，但不可交换收敛，即不绝对收敛。

#### 例 {#top-iv-s7-n6-exa-2 .statement tag=0BTT}

如果我们对$n \geq 2$取$u_{2n-1} = -1/n$和$u_{2n} = 1/n$，则乘积$(1 + u_n)$不是绝对收敛的，因为级数$(u_n)$不是绝对收敛的；但自从

$$
\prod_{p=3}^{n} (1 + u_p) = \prod_{p=2}^{n} \left(1 - \frac{1}{p^2}\right),
$$
和
$$
\prod_{p=3}^{2n+1} (1 + u_p) = \left(1 - \frac{1}{n+1}\right) \prod_{p=2}^{n} \left(1 - \frac{1}{p^2}\right),
$$
由定理 4 可知乘积收敛，且其值为
$$
\prod_{n=2}^{\infty} \left(1 - \frac{1}{n^2}\right).
$$

此外，应该观察到，一般项为$u_n$的级数的*收敛*对于其一般因子为$1 + u_n$的乘积的*收敛*既不是必要的，也不是充分的（见习题21和22）。

### 习题{#top-iv-s7-exercises}

§ 7](exercises/s7/)参见[习题。
