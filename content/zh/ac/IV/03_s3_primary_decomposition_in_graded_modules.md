---
book: ac
book_title: Commutative Algebra
chapter: IV
chapter_title: ASSOCIATED PRIME IDEALS AND PRIMARY DECOMPOSITION
section: 3
section_title: Primary decomposition in graded modules
lang: zh
source: ac-i-vii
book_pages: 283-285, 301
pdf_pages: 0303-0305, 0321-0321
extraction: ocr
subsections:
    - "no": 1
      title: PRIME IDEALS ASSOCIATED WITH A GRADED MODULE
      page: 283
      pdf_page: 303
    - "no": 2
      title: PRIMARY SUBMODULES CORRESPONDING TO GRADED PRIME IDEALS
      page: 284
      pdf_page: 304
    - "no": 3
      title: PRIMARY DECOMPOSITION IN GRADED MODULES
      page: 285
      pdf_page: 305
statements: 6
exercises: 3
content_sha256: 4208a1793b87ce20b72a72a146894673c4d86d82c10dc53b21826ce886348391
translated_from: content/en/ac/IV/03_s3_primary_decomposition_in_graded_modules.md
translation_method: google
source_content_sha256: 44d441232ef2de6c8b1ed43a9b9091b103360b9960ee00be0b5d251f8b5a5aff
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: a51b3b1ec321966e09bc4e0b2a2970ea002071bcb3b96954e04e2b5cad0f5622
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 3. 初等分解已评分模

### 1. 与分级模相关的素理想

#### 命题 1 {#ac-iv-s3-prop-1 .statement tag=04MJ}

令$A$为无扭交换律群，$A$为型$A$的分级环，$M$为型$A$的分级$A$模。每个与$M$相关的素理想都是分级的，并且是$M$的齐次元素的湮没子。

我们知道$A$可以给出与其群结构兼容的总共阶结构（代数，章II, § 11, no. 4，引理2）。令$p$为与$M$、湮没子相关的元素$x \in M$的素理想，令$(x_i)_{i \in \Delta}$为$x$的齐次分量族；令$i(1) < i(2) < \cdots < i(r)$为$i$的值，其中$x_i \neq 0$。考虑元素 $a \in p$ 并令 $(a_i)_{i \in \Delta}$ 为其同构成分族；我们将证明$a, \in p$对于所有$i \in A$，这将表明$p$是一个分级理想。

我们通过归纳对指标$i$的数进行论证，使得$a, \neq 0$。如果这个数是0，我们的断言是显而易见的；如果不是，则令$m$为指标$i$中的最大的，其中$a, \neq 0$；如果我们证明$a, \in p$，将归纳假设应用到$a - a,$就会得出结论。现在，$ax = 0$；对于所有$j \in A$，利用$ax$的次数$m + j$的齐次分量为0，我们得到
$$
\sum_{i \in \Delta} a_{m-i} x_{j+i} = 0;
$$
我们结论认为$a_m x_j$是指标$i > j$的$x_i$中的线性组合。特别是因此$a_m x_{i(r)} = 0$、从而，通过在$n < r$、$a_m^{r-n+1} x_{i(n)} = 0$上下降归纳。然后 $a_m^r x = 0$、从而 $a_m^r \in p$，并且由于 $p$ 是质数，$a, \in p$。

现在我们证明$p$是$M$的齐次元素的湮没子。让我们把$1 \leq n \leq r$写成$b_n = \operatorname{Ann}(x_{i(n)})$。对于$p$的每个齐次元素$b$和所有$n$，次数$i(n) + \deg(b)$的$bx$的齐次分量是$bx_{i(n)}$，因此$bx_{i(n)} = 0$和$b \in 6$；因为$p$是由其同构元素、$p \subset 6$生成的。另一方面，显然$\bigcap_{n=1}^r 6_n \subset \operatorname{Ann}(x) = p$；由于$p$是质数，因此存在$n$使得$b_n \subset p$（章11，§ 1, no. 1，命题1），从而$b_n = P = \operatorname{Ann}(x_{i(n)})$，完成证明。

#### 推论{#ac-iv-s3-n1-cor-1 .statement tag=04MK}

对于与分级$A$-模块$M$相关的每个（必然分级的）素理想$p$，存在指标$k \in A$，使得从分级$A$-模块$A/p$获得分级$A$-模块$(A/p)(k)$： 次数减 $k$ (代数, 章 II, § 11, no. 2) 与 $M$ 的分级子模同构。

当命题 1 的证明记号时，考虑从$A$ 的同态 $a \mapsto ax_{i(n)}$ 到$M$ 取商获得同态；后者是次数 $i(n)$ 的分级同态，因此它在取商时将次数的分级双射同态 $A/p$ 的分级双射$i(n)$ 转换为 $M$ 的分级子模。

#### 命题 2 {#ac-iv-s3-prop-2 .statement tag=04ML}

*令$A$为无扭交换群，$A$为型$A$的分级诺特环，以及$M$为$A$的分级有限生成模型$A$。存在$M$的分级子模的合成列$(\mathbf{M}_i)_{0 \leq i \leq n}$由……组成，使得对于$0 \leq i \leq n - 1$，分级模$\mathbf{M}_i / \mathbf{M}_{i+1}$同构于移位分级模$(A/p_i)(k_i)$，其中$p_i$ 是 $A$ 和 $k_i \in A$ 的分级素理想。*

回溯§ 1, no. 4、定理 1 的论证就足够了，此时$\mathscr{G}$是$M$的分级子模的集合，而合成列具有叙述的性质；我们利用得出命题 1 的推论。

### 2. 初级子模相应的至分级素理想

#### 命题 3 {#ac-iv-s3-prop-3 .statement tag=04MM}

*令$A$为无扭交换律群，$A$为型$A$的分级诺特环，$p$为$A$和$M$的分级理想$A$-型$A$的模没有减少到$0$。假设对于 $M$ 上比率 $a$ 的 $p$ 位似的每个齐次元素 $a$ 几乎是幂零的，并且对于比率 $A - p$ 位似的每个齐次元素 $b$ $M$ 上的$b$ 是单射的。那么$p$是primary，$M$的子模$\{0\}$是$p$-primary。*

只要证明 $\operatorname{Ass}(M) = \{p\}$ (§ 2, no. 1, 命题 1) 就足够了。设$q$为与$M$相关的素理想；它是一个分级理想，它是湮没子的齐次元素 $x \neq 0$ 的 $M$（no. 1，命题 1）。对于$q$、$ax = 0$的每个齐次元素$a$，因此$M$上比率$a$的位似不是单射的，从而$a \in p$。相反，令 $b$ 为 $p$ 的齐次元素；存在整数$n > 0$使得$b^n x = 0$，从而$b^n \in \operatorname{Ann}(x) = q$，并且由于$q$是质数，因此$b \in q$。由于$p$和$q$是由它们各自的齐次元素、$p = q$生成的，这就证明了$\operatorname{Ass}(M) \subset \{p\}$。如$M \neq \{0\}, \operatorname{Ass}(M) \# \varnothing$（§ 1, no. 1，推论1至命题2），从而$\operatorname{Ass}(M) = \{p\}$。

#### 命题 4 {#ac-iv-s3-prop-4 .statement tag=04MN}

*令$A$为无扭交换律群，$A$为型$A$的分级诺特环，以及$M$为型的分级$A$模$A$。令$p$为$A$和$N$的素理想，$M$的子模相对于$M$是$p$主理想。

(i) $p$ (代数, 章 11, § 11, no. 3) 中包含的$A$的最大的分级理想$p'$是素数。

(ii) $N$ 的最大的分级子模 $N'$ 相对于$M$ 是$p'$-主要。*

我们知道（*loc.cit.*）$p'$（或$N'$）的齐次元素只是$p$（或$N$）的齐次元素。令 $a$ 为 $p$ 的齐次元素；如果$x$是$M$的齐次元素，则存在整数$n > 0$使得$a^n x \in N$；由于 $a^n x$ 是齐次的，$a^n x \in N'$；因为每个$y \in M$都是齐次元素的有限数的直和，我们结论存在整数$q > 0$使得$a^q y \in N'$，因此位似与比率$a$ $M/N'$ 几乎是幂零的。

现在考虑 $A - p'$ 的齐次元素 $b$；那么 $b \notin p$ 因为 $b$ 是齐次的。令$x$ 为$M$ 的元素，使得$bx \in N'$ 且令$(x_i)_{i \in \Delta}$ 为$x$ 的齐次分量族。由于 $N'$ 已分级，因此 $i$ 为 $bx_i \in N'$，因此为 $bx_i \in N$，并且，作为 $b \notin p$，我们对 $x_i \in N$ 进行结论；由于 $x_i$ 是齐次的，$x_i \in N'$、从而 $x \in N'$ 和位似以及 $M/N'$ 上的比率 $b$ 是单射的。 命题 4 然后将命题 3 应用于$p'$ 和$M/N'$。

### 3. 初等分解已评分模

#### 命题 5 {#ac-iv-s3-prop-5 .statement tag=04MO}

令$A$为无扭交换律群，$A$为型$A$的分级诺特环，$M$为型的分级$A$模$M$、$N$ $M$ 中的子模以及$M$ 中$N$ 的$N = \bigcap_{i \in I} Q_i$ 初等分解。

(i) 令$Q'_i$为最大的，对$Q_i$中包含的$M$进行分级子模。那么$Q'_i$是主要的，$N = \bigcap_{i \in I} Q'_i$。

(ii) 如果初等分解$N = \bigcap_{i \in I} Q_i$减少，初等分解$N = \bigcap_{i \in I} Q'_i$也减少，并且对于所有$i \in I$，素理想相应的到$Q_i$和$Q'_i$相等。

(iii) 如果$Q_i$对应到素理想$p_i$，即$\operatorname{Ass}(M/N)$的最小元素，则$Q_i$是$M$的分级子模。

我们已经看到(no. 2, 命题 4)，$Q'_i$相对于$M$和$N \subset Q'' \subset Q_i$是主要的，这证明了(i)。 no. 2的命题 4还表明，素理想$p'_i$相应的至$Q'_i$是素理想$p_i$相应的至$Q_i$中包含的最大的分级理想。如果减少分解$N = \bigcap_{i \in I} Q_i$，$p_i \in \operatorname{Ass}(M/N)$对于所有$i$（§ 2, no. 3，命题4），因此$p_i$是分级理想（no. 1，命题1），因此$p'_i = p_i$；然后$\operatorname{Ass}(M/N) = \bigcup_{i \in I} \{p'_i\}$(§ 2, no. 3,命题4)，证明分解$N = \bigcap_{i \in I} Q'_i$减少了(§ 2, no. 3,命题4)。最后，如果$p_i$是$\operatorname{Ass}(M/N)$的最小元素，则$p'_i = p_i$自$p_i$起被评分（no. 1，命题1），从而$Q'_i = Q_i$凭借§ 2, no. 3， 命题5.

### 习题 {#ac-iv-s3-exercises}

§ 3](exercises/s3/)参见[习题。
