---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 18
section_title: Simple Algebras over a Finite Field
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.355-A VIII.360
pdf_pages: 0372-0377
extraction: native+ocr
subsections:
    - "no": 1
      title: Polynomials over a Finite Field
      page: 355
      pdf_page: 372
    - "no": 2
      title: Simple Algebras over Finite Fields
      page: 357
      pdf_page: 374
statements: 10
exercises: 7
content_sha256: 826a4e73672f145834533d0e0c34524a80c7bb14ac4cd9f74bbd6fb0a211d0c8
translated_from: content/en/alg/VIII/18_s18_simple_algebras_over_a_finite_field.md
translation_method: google
source_content_sha256: 54d2a6b31a60bad387aff00416b44414a3612b96aff88b09c11c2b91d78d43d8
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 1780e1a3efb1f4f37efb56b7a8e6aa172f42fc0df9671c159b91b5367219257e
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 18。 单代数超过有限域

### 1. 有限域以上的多项式

#### 定理 1（Chevalley-警告）{#alg-viii-s18-thm-1 .statement tag=00SA}

令 K 为特征 $p$ 的有限交换域。令$n$为整数$\geqslant 1$，且$(f_i)_{i\in I}$为$K[X_1, . . . ,X_n]$的非零元素的有限族。用元素 $\mathbf{x}$ 的 Z 集合 $K^n$ 表示，这样我们就有 $i\in I$ 的$f_i(\mathbf{x}) = 0$。如果我们有$n >\sum_{i\in I}$ deg($f_i$)，那么Z的基数可以被$p$整除。

#### 引理 1 {#alg-viii-s18-lem-1 .statement tag=00LB}

令L为域，G为有限群，且$\chi$为从G到乘法群$L^*$的非平凡同态。我们有$\sum_{x\in G}\chi (x) = 0$。

到假设，G 存在元素 $a$，使得$\chi (a)\not= 1$；因为乘法除以$a$是G的置换，我们有

$$
\sum_{x\in G}\chi (x) =\sum_{x\in G}\chi (ax) =\chi (a)\sum_{x\in G}\chi (x)
$$

这给出了引理 1。

#### 引理 2 {#alg-viii-s18-lem-2 .statement tag=00LC}

令 $q$ 为 K 的基数。对于任意整数 $m\geqslant 0$，集合 $S_m=$ $\sum_{x\in K}x^m$。如果$m$是$q-1$的非零的倍数，我们有$S_m=-1$，在所有其他情况下$S_m= 0$。

回想一下 $0^0= 1$ (I, §2, No. 1, p. 14)。假设$m$是$q-1$的倍数。由于阿贝尔的群 $K^*$ 具有阶 $q-1$，因此对于每个 $x\in K^*$ 和 $S_m= 0^m+ (q-1)\cdot 1$，我们都有 $x^m= 1$，在本例中给出断言。

假设$m$不是$q-1$的倍数。 集合 $\chi (x) =x^m$ $x\in K^*$。由于乘法群$K^*$是阶$q-1$的循环（V, §12, No. 1，p. 93，命题1），因此存在$K^*$的元素$a$使得$\chi(a) \neq 1$。将引理 1 应用于$G = K^*$，我们有
$$
S_m = 0^m + \sum_{x \in K^*} \chi(x) = 0;
$$
这给出了引理 2。

现在让我们证明定理 1。令$\mathbf{x} = (x_1, \ldots, x_n)$为$K^n$的元素。如果$f_i(\mathbf{x}) \neq 0$，我们有$1 - f_i(\mathbf{x})^{q-1} = 0$；如果$f_i(\mathbf{x}) = 0$，我们有$1 - f_i(\mathbf{x})^{q-1} = 1$。 集合$P = \prod_{i=1}^r (1 - f_i^{q-1})$。我们有
$$
P(\mathbf{x}) = \begin{cases}
1 & \text{if } \mathbf{x} \in \mathbf{Z}, \\
0 & \text{if } \mathbf{x} \notin \mathbf{Z}.
\end{cases}
$$
让我们将多项式$P$展开为$\sum_{\alpha \in \mathbf{N}^n} c_\alpha X^\alpha$；到假设，它有次数$< (q-1)n$。令$\alpha$为$\mathbf{N}^n$的元素，使得$c_\alpha$为非零的。由于我们有$\alpha_1 + \cdots + \alpha_n < (q-1)n$，因此存在整数$\ell$，使得$1 \leq \ell \leq n$和$0 \leq \alpha_\ell < q-1$。到引理 2，我们就有 $\sum_{x \in K} x^{\alpha_\ell} = 0$，因而
$$
\sum_{\mathbf{x} \in K^n} \mathbf{x}^\alpha = \prod_{j=1}^n \left( \sum_{x \in K} x^{\alpha_j} \right) = 0.
$$
因此我们有
$$
\sum_{\mathbf{x} \in K^n} P(\mathbf{x}) = \sum_{\alpha \in \mathbf{N}^n} c_\alpha \left( \sum_{\mathbf{x} \in K^n} \mathbf{x}^\alpha \right) = 0.
$$
现在，通过公式 (1)，我们有 $\sum_{\mathbf{x} \in K^n} P(\mathbf{x}) = \operatorname{Card}(\mathbf{Z}) \cdot 1$，因此有 $\operatorname{Card}(\mathbf{Z}) \cdot 1 = 0$，这意味着 $\operatorname{Card}(\mathbf{Z})$ 可以被 $p$整除。

#### 推论{#alg-viii-s18-n1-cor-1 .statement tag=00LD}

*令$V$为有限维$n$的向量空间超过$K$，并且$I$是有限的集合，并且对于每个$i \in I$，令$F_i : V \to K$为齐次多项式映射或次数 $d_i > 0$。如果我们有 $\sum_{i \in I} d_i < n$，则存在非零元素 $x$ 或 $V$，使得每个 $i \in I$ 都有 $F_i(x) = 0$。*

令$(e_1, \ldots, e_n)$为$V$除$K$的基。通过齐次多项式映射的定义 (IV, §5, No. 9, p. 55, 定义 3)，对于每一个 $i \in I$，在次数 $d_i$ 的 $K[X_1, \ldots, X_n]$ 中存在一个齐次多项式 $f_i$，使得我们有$F_i(\xi_1 e_1, \ldots, \xi_n e_n) = f_i(\xi_1, \ldots, \xi_n)$。令$Z$为集合/元素$x$/$V$，使得每个$i \in I$都有$F_i(x) = 0$。通过定理 1，$Z$的基数可以被$p$整除，并且从$0$属于到$S$，我们有$\operatorname{Card}(Z) \geq p > 1$。

### 2. 单代数超过有限域

#### 定理 2（韦德伯恩）{#alg-viii-s18-thm-2 .statement tag=00SB}

每个有限域都是可交换的。

令 D 为有限域，令 K 为其中心。 K-代数 D 是次数 $m^2$ 的中心简单，其中$m$ 是严格的正整数。 约化范数是次数 $m$ (VIII, p. 345, 命题 6) 的齐次多项式映射 Nrd$: D\rightarrow K$，并且对于 D 中的每个$a\not= 0$，我们有 Nrd($a$)$\not= 0$ （VIII、p. 340、命题 3）。上面的推论意味着$m\geqslant m^2$，因而$m= 1$。所以我们有 D = K。

#### 推论 1 {#alg-viii-s18-thm-2-cor-1 .statement tag=00LE}

每个有限简单环都同构于矩阵环 $\mathbf{M}_n(L)$，其中 $n$ 是严格的正整数，L 是有限的交换域。

这是从定理 2 和结构定理得出简单的环（VIII、p. 120、定理 1）。

#### 推论 2 {#alg-viii-s18-thm-2-cor-2 .statement tag=00LF}

令 K 为有限交换域。 K 上的每个中心单代数都同构于矩阵代数 $\mathbf{M}_n(K)$，其中$n$ 是严格的正整数。

这是从定理 2 和结构定理到中央单代数（VIII、p. 252、定理 1）。

#### 注 1 {#alg-viii-s18-n2-rem-1 .statement tag=00LG}

这里是定理的另一个证明 2. 令 D 为有限域，令 K 为其中心，令 L 为 D 的极大交换子域。令 $x$ 为 的元素 $D^*$。 D 的属于到极大交换子域 $L_1$。我们有等式

$$
[D : K] = [L : K]^2= [L_1: K]^2
$$

由VIII、p. 265的推论2，因而$[L : K] = [L_1: K]$。由K的V, §12, No. 2、p. 94、扩张、L和$L_1$的命题3同构。由VIII，p. 263，推论，$D^*$存在元素$a$使得$aLa^{-1}= L_1$，所以$a^{-1}xa$属于到L。那么对于每个$y\in L^*$我们就有$(ay)^{-1}x(ay) =a^{-1}xa$。因而，如果 S 是 $D^*$ 模 $L^*$ 的左陪集代表的集合，则 $D^*-\{1\}$ 的每个元素都可以用 $s\in S$ 和 $x\in L^*-\{1\}$ 写成 $sxs^{-1}$。我们用$d$表示$D^*$的阶，用$\ell$表示$L^*$。由于 S 的基数等于 $d/\ell$，因此我们有 $d-1\leqslant (d/\ell )(\ell -1) =d-d/\ell$。由此可知$\ell =d$，故L = D，证明域 D 是可交换的。

#### 注 2 {#alg-viii-s18-n2-rem-2 .statement tag=00LH}

令L为交换域，性质：$(C_1)$令V为有限维$n$中的向量空间超过域L，并令$d$使得$0< d < n$。对于次数$d$的每个齐次多项式映射$F : V\rightarrow L$，存在V的非零元素$x$使得$F(x) = 0$。

定理 2 的证明表明有限次数的每个域超过L 且中心 L 等于L。

根据VIII、p. 356的推论，每个有限域都有性质$(C_1)$。我们可以证明（VIII，p. 360，习题7）以下域有性质$(C_1):$

– 有限域的每个代数扩张

– 有理分式中的每一个域在一个变量中，系数为代数闭域（Tsen 的定理）。

– $*$每个域被赋予完整的离散估值

其剩余类域是代数闭 (VIII, p. 332, 习题 17)$.*$

#### 注 3 {#alg-viii-s18-n2-rem-3 .statement tag=00LI}

假设域 K 满足以下条件：

– 如果L是有限次数的K的扩张，则它是循环的并且范数映射$N : L^*\rightarrow K^*$是满射的。

特别是当域 K 是有限的（V, §12, No. 2、p. 95、命题 4）时，条件得到满足。然后我们可以证明 K 上的每个域 of 有限次数与中心 K 都等于 K（习题 10 of VIII, p. 329）。

### 习题{#alg-viii-s18-exercises}

参见[习题为 § 18](exercises/s18/)。
