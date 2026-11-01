---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 3
section_title: Hilbert’s Nullstellensatz
appendix: true
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.461-A VIII.462
pdf_pages: 0478-0479
extraction: native
statements: 3
exercises: 0
content_sha256: e3f95f598d11da6eddc2e3b3b20177c8a95df2a10cab2c66c68b60f599b7c462
translated_from: content/en/alg/VIII/A3_a3_hilbert_s_nullstellensatz.md
translation_method: google
source_content_sha256: 07f9a0ede5f4c5e394c02864754c6d680dbb4f9d6eb5a745c7ccb3b3fef1f87d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 45a15ae0c761f62a81e5a1f6f34488164bb06fdfb8c7e6e6ba6aa5f93ff94d2c
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 附录 3 希尔伯特零点定理

#### 定理 1 {#alg-viii-a3-thm-1 .statement tag=00QM}

设A为整环，K为分数的域，L为交换K-代数。假设A-代数L是由有限多个元素生成的，并且L是域。

a) K 上的 L 的次数是有限的。

b) A 存在非零元素 $a$，使得 K 等于 $A[a^{-1}]$。

令 S 为生成子集 / A-代数 L。我们使用归纳法在S枢机主教上。

首先，假设 S 的元素都是 K 上的代数。那么 K 上的 L 的次数是有限的（V, §3, No. 2、p. 18、定理 2）。令$(e_i)_{i\in I}$为K上L的基。存在A的非零元素$a$，使得S的元素、元素1和元素$e_ie_j$相对于该基的坐标为$i,j$在I属于到$A[a^{-1}]$。 线性组合 $\sum_{i\in I}a_ie_i$ 的集合加上每个 $i$ 的 $a_i\in A[a^{-1}]$ 则为 L 的子环。 包含 A 和 S 乘以构造，因此等于 L。特别是包含$Ke_1$，所以K等于$A[a^{-1}]$。

现在假设S的元素$s$超越K。用环$A[s]$的分数的E域来表示。 $A[s$]-代数L由S$-\{s\}$生成。到归纳假设，存在非零的多项式$P\in A[X]$，使得E等于$A[s][P(s)^{-1}]$。令 $\overline{K}$ 为 K (V, §4, No. 3, p. 23, 定理 2) 的代数闭包。由于域$\overline{K}$是无限的（V, §4, No. 1，p. 20，命题3），因此$\overline{K}$存在元素$x$使得$P(x)\not= 0$。令$\varphi : E\rightarrow K$为唯一同态，从K-代数$E = A[s][P(s)^{-1}]$到K-代数$\overline{K}$，将$s$发送到$x$。这是荒谬的，因为 E 是 K 的超越扩张，而 $\overline{K}$ 是 K 的代数扩张。这完成了定理的证明。

#### 推论 1 {#alg-viii-a3-thm-1-cor-1 .statement tag=00RV}

设K为交换域，A为由有限多个元素生成的交换K-代数，$\mathfrak{m}$为A的最大理想。

a) K 上的 $A/\mathfrak{m}$ 的次数是有限的。

b) 令Ω为K的代数闭扩张。从A到Ω存在K-代数同态，且核$\mathfrak{m}$。

K-代数$A/\mathfrak{m}$由有限多个元素生成，$A/\mathfrak{m}$是域。通过定理 1，$A/\mathfrak{m}$的次数是有限的； 断言a)如下。 有限次数的 K 的每个扩张同构于 Ω 的子扩张 (V, §4, No. 1, p. 20, 定理 1);这给出了b)。

#### 推论 2 {#alg-viii-a3-thm-1-cor-2 .statement tag=00QN}

令K为交换域，$n$为自然数，$(P_i)_{i\in I}$为$K[X_1, . . . ,X_n]$的元素族，Ω为K的代数闭扩张。以下条件是等价的：

(i) 多项式 $P_i$ 在 $\Omega^n$ 中没有公共零点。

(ii) 存在一个族$(Q_i)_{i\in I}$，其中有限支撑，元素，$K[X_1, . . . ,X_n]$，使得$\sum_{i\in I}P_iQ_i= 1$。

用 A 环 $K[X_1, . . . ,X_n]$ 和 $\mathfrak{a}$ 表示由多项式 $P_i$ 生成的理想值。 条件(i)表示从$A/\mathfrak{a}$到Ω不存在K-代数同态。如果满足，则根据推论1，环$A/\mathfrak{a}$没有极大理想，因此为零，并且1属于到$\mathfrak{a}$。这证明(i)蕴含(ii)。 (ii) $\Rightarrow$ (i) 的含义是明确的。
