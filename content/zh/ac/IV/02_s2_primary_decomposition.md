---
book: ac
book_title: Commutative Algebra
chapter: IV
chapter_title: ASSOCIATED PRIME IDEALS AND PRIMARY DECOMPOSITION
section: 2
section_title: Primary decomposition
lang: zh
source: ac-i-vii
book_pages: 267-282, 290-301
pdf_pages: 0287-0302, 0310-0321
extraction: ocr
subsections:
    - "no": 1
      title: PRIMARY S BMODULES
      page: 267
      pdf_page: 287
    - "no": 2
      title: THE EXISTENCE OF A PRIMARY DECOMPOSITION
      page: 270
      pdf_page: 290
    - "no": 3
      title: UNIQUENESS PROPERTIES IN THE PRIMARY DECOMPOSITION
      page: 270
      pdf_page: 290
    - "no": 4
      title: THE LOCALIZATION OF A PRIMARY DECOMPOSITION
      page: 272
      pdf_page: 292
    - "no": 5
      title: RINGS AND MODULES OF FINITE LENGTH
      page: 274
      pdf_page: 294
    - "no": 6
      title: PRIMARY DECOMPOSITION AND EXTENSION OF SCALARS
      page: 279
      pdf_page: 299
statements: 39
exercises: 35
content_sha256: 7e5e3c2c52ef6e3812228c941e1950d77cd066b9d4280d0652243ce8833e0286
translated_from: content/en/ac/IV/02_s2_primary_decomposition.md
translation_method: google
source_content_sha256: 412a1eb43c414ef74369ccfcd275c3769490e226305405794c9a0f41eee4ebea
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 32bc3b2b0d4af384fd2da527b3b21df4a1fd2d262d7db2a4f6d6a3d0a6b105a2
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 2.初等分解

### 1. 主要 S B 模块

#### 命题 1 {#ac-iv-s2-prop-1 .statement tag=04KE}

令$A$为诺特环且$M$为$A$模块。以下条件是等效的：
(a) $\operatorname{Ass}(M)$ 减少为单个元素。

(b) $M \neq 0$ 和 $M$ 的每个位似要么是单射的，要么是几乎幂零的（$§ 1$，no. 4）。 *如果*满足这些条件并且$p$是$a \in A$的集合使得位似$a_M$几乎为零，那么$\operatorname{Ass}(M) = \{p\}$。

这紧接着从$§ 1$、no. 4，推论到命题 9 和no. 1，推论 2 到命题 2。

#### 定义 1 {#ac-iv-s2-def-1 .statement tag=04KF}

*令$A$为诺特环，$N$为$A$模，$Q$子模为$N$。 *如果*模$M = N/Q$满足命题1的条件，$Q$被称为关于*$N$的*p-primary（或*在*$N$）。

当没有歧义时，我们简单地说$Q$是“p-primary”或“primary”；显然，对于 $N$ 包含 $Q$ 中的每个子模 $N' \neq Q$，$Q$ 是 $N'$ 中的 p 主色。

定义 1 特别适用于$N = A$的情况； $N$的子模是$A$的*理想*，因此如果$\operatorname{Ass}(A/q)$有一个元素，那么$A$的理想$q$被称为*主*，或者，如果$A \neq q$和每个除子环 $A/q$ 中的零 *幂幂*。如果 $q$ 是 p 基数，则从定义 1 可以得出，$p$ 是理想 $q$ 的*根式*（章 II、$§ 2$、no. 6）。

#### 注 {#ac-iv-s2-n1-rem-1 .statement tag=04KG}

令 $q$ 为 $A$-模块 $N$ 的 p-primary 子模。如果$N/Q$是*有限生成的*，则存在整数$k > 0$，使得$p^k N \subset Q$乘以$§ 1$、no. 4、命题9。

*例*

#### 例 1 {#ac-iv-s2-n1-exa-1 .statement tag=04KH}

如果 $p$ 是 $A$ 的素理想，则 $p$ 是 p 初等（$§ 1$、no. 1、命题 1）。

#### 例 2 {#ac-iv-s2-n1-exa-2 .statement tag=04KI}

令$q$为$A$的理想，使得存在*单一*素理想$m$（必然是最大）包含$q$；那么，如果$M$是一个$A$模块，使得$qM \neq M$、$qM$相对于$M$来说是*m-primary*。对于 $\operatorname{Ass}(M/qM)$ 包含 $q$ 的每个元素，因此等于 $m$ 和 $\operatorname{Ass}(M/qM) \neq 0$（$§ 1$、no. 1，推论 1 到命题 2）。特别是$q$是$A$中的*m主*理想。

#### 例 3 {#ac-iv-s2-n1-exa-3 .statement tag=04KJ}

令 $m$ 为 $A$ 的*极大*理想； m-主理想则为 $A$ 的理想 $q$，其中存在整数 $n \geq 1$，使得 $m^n \subset q \subset m$。因为如果$m^n \subset q \subset m$，$m$是唯一的素理想包含$q$（章11，$§ 1$，no. 1，命题1的推论），结论来自*例2*；相反，如果$q$是m元，则$m$是$q$的根式，因此存在$n \geq 1$使得$m^n \subset q$（章II，$§ 2$，no. 6，命题15）。

#### 例 4 {#ac-iv-s2-n1-exa-4 .statement tag=04KK}

在*主理想整环* $A$中，主要理想是$(0)$和形式$Ap^n$的理想，其中$p$是极值元素和$n \geq 1$；这紧随 *例 3* 而来。

#### 例 5 {#ac-iv-s2-n1-exa-5 .statement tag=04KL}

任何素理想的幂不一定是初理想（习题1）。另一方面，存在不是幂素理想 (习题 1) 的初理想。

#### 命题 2 {#ac-iv-s2-prop-2 .statement tag=04KM}

设 M 是诺特环 A 上的模，p 是 A 的素理想，$(\mathscr{Q}_i)_{i \in I}$ 是 M 的子模非空有限族，它们相对于 M 是 p 初值。那么 $\bigcap_{i \in I} \mathscr{Q}_i$ 是关于 M 的 p 初值。

$M / (\bigcap_{i \in I} \mathscr{Q}_i)$同构于直和$\bigoplus_{i \in I} (M / \mathscr{Q}_i)$的子模$\neq 0$。现在

$$
\operatorname{Ass}\left( \bigoplus_{i \in I} (M / \mathscr{Q}_i) \right) = \bigcup_{i \in I} \operatorname{Ass}(M / \mathscr{Q}_i) = \{p\}
$$

（§ 1, no. 1，推论 1 至命题 3）。因此，$\operatorname{Ass}\left(M / (\bigcap_{i \in I} \mathscr{Q}_i)\right) = \{p\}$（§ 1, no. 1、命题 3 和推论 1 至命题 2）。

#### 命题 3 {#ac-iv-s2-prop-3 .statement tag=04KN}

设 A 为诺特环，S 为 A 的乘法子集，p 为 A 的素理想，M A-模，M 的 N 子模以及 M 到 $S^{-1}M$ 的 $i = i_A^S$ 典范映射。

(i) 假设$p \cap S \neq \varnothing$。如果 N 相对于 M 是 p 主的，则 $S^{-1}N = S^{-1}M$。

(ii) 假设$p \cap S = \varnothing$。 For N to be p-primary with respect to M, it is necessary and sufficient that N be of the form $i_1(N')$, where $N'$ is a sub-$S^{-1}A$-module of $S^{-1}M$ which is $(S^{-1}p)$-primary with respect to $S^{-1}M$; then $N' = S^{-1}N$.

(i) 如果 $p \cap S \neq \varnothing$ 且 N 相对于 M 是 p 主的，则

$$
\operatorname{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \varnothing
$$

（§ 1, no. 2，命题 5 的推论），因此$S^{-1}(M/N) = 0$（§ 1, no. 1，推论 1 到命题 2），从而 $S^{-1}M/S^{-1}N = 0$。

(ii) 假设$p \cap S = \varnothing$。如果 N 相对于 M 是 p-primary，则 $\operatorname{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \{S^{-1}p\}$（§ 1, no. 2，命题 5 的推论），因此 $S^{-1}M$ 的子模 $N' = S^{-1}N$ 是 $(S^{-1}p)$-primary；此外，如果$s \in S$和$m \in M$使得$sm \in N$，则$m \in N$，对于M/N中比s为单射的位似来说，从而$N = i_1(N')$（章II, § 2, no. 4，命题10）。相反，令$N'$为$S^{-1}M$的子模，它相对于$S^{-1}M$是$(S^{-1}p)$主要的；让我们写$N = i_1(N')$；然后$N' = S^{-1}N$（章II, § 2, no. 4，命题10）和$\operatorname{Ass}_{S^{-1}A}(S^{-1}(M/N)) = \operatorname{Ass}_{S^{-1}A}((S^{-1}M)/N') = \{S^{-1}p\}$。由于典范映射$M/N \to S(M/N)$是单射的，与M/N相关的A的素理想不满足S（§ 1, no. 2，命题6）；由此得出 $\operatorname{Ass}(M/N) = \{p\}$（§ 1, no. 2，命题 5 的推论），因此 N 相对于 M 是 p 主的。

### 2.初等分解的存在

#### 定义 2 {#ac-iv-s2-def-2 .statement tag=04KO}

令$A$为诺特环，$M$为$A$模，$N$子模为$M$。 $M$的子模的有限族$(\mathscr{Q}_i)_{i \in I}$对于$M$是主要的，因此$N = \bigcap_{i \in I} \mathscr{Q}_i$在$M$中被称为$N$的初等分解。

#### 例 {#ac-iv-s2-n2-exa-1 .statement tag=04KP}

让我们用 $A = \mathbf{Z}$、$M = \mathbf{Z}$、$N = n\mathbf{Z}$ 来表示一些整数 $n > 0$。如果$n = p_1^{\alpha_1} \cdots p_k^{\alpha_k}$是$n$的分解变成素数因子，
$$
n\mathbf{Z} = (p_1^{\alpha_1}\mathbf{Z}) \cap \ldots \cap (p_k^{\alpha_k}\mathbf{Z})
$$
是 $\mathbf{Z}$ 中的 $n\mathbf{Z}$ 初等分解乘以 no. 1 的例 4。

滥用语言，关系$N = \bigcap_{i \in I} \mathscr{Q}_i$在$M$中被称为$N$的初等分解。这相当于说$\{0\} = \bigcap_{i \in I} (\mathscr{Q}_i/N)$是$M/N$中$\{0\}$的初等分解。如果$(\mathscr{Q}_i)_{i \in I}$是$M$中$N$的初等分解，则从$M/N$到$\bigoplus_{i \in I} (M/\mathscr{Q}_i)$的典范映射是单射的。相反，让$N$是$M$和$f$单同态的子模，从$M/N$到有限的直和$P = \bigoplus_{i \in I} P_i$，其中每个集合$\operatorname{Ass}(P_i)$都减少为单个元素$p_i$；令$f_i$为同态$M/N \to P_i$，将合成减去投影$P \to P_i$，令$Q_i/N$为核；那么与$M$不同的$Q_i$对于$M$（no. 1，定义1）和$N = \bigcap_{i \in I} Q_i$来说是主要的。此外，$\operatorname{Ass}(M/N) \subset \bigcup_{i \in I} \{p_i\}$凭借§ 1, no. 1、命题3。

#### 定理 1 {#ac-iv-s2-thm-1 .statement tag=04KQ}

令$M$为有限生成模除以诺特环，并令$N$为子模除以$M$。存在形式 $N$ 初等分解
$$
N = \bigcap_{p \in \operatorname{Ass}(M/N)} Q(p)
$$
其中，对于所有$p \in \operatorname{Ass}(M/N)$，$Q(p)$相对于$M$来说是$p$-主要的。

我们可以通过替换$M$乘以$M/N$，因此假设$N = 0$。由 § 1, no. 4，推论定理 2，$\operatorname{Ass}(M)$ 是有限的；通过§ 1, no. 1，命题 4，对于$M$的每个$p \in \operatorname{Ass}(M)$，子模$Q(p)$，存在$\operatorname{Ass}(M/Q(p)) = \{p\}$和$\operatorname{Ass}(Q(p)) = \operatorname{Ass}(M) - \{p\}$。让我们写$P = \bigcap_{p \in \operatorname{Ass}(M)} Q(p)$；对于所有$p \in \operatorname{Ass}(M)$，$\operatorname{Ass}(P) \subset \operatorname{Ass}(Q(p))$，因此$\operatorname{Ass}(P) = \varnothing$，这意味着$P = 0$（§ 1, no. 1，推论1到命题2），因此证明定理。

### 3. 唯一性初等分解的房产

#### 定义 3 {#ac-iv-s2-def-3 .statement tag=04KR}

令$M$为模超过诺特环和$N$子模除$M$。如果满足以下条件，则$M$中的$N$的初等分解$N = \bigcap_{i \in I} Q_i$称为约简：

(a) *不存在指标* $i \in I$ *使得* $\bigcap_{j \neq i} Q_j \subset Q_i;$

(b) *如果* $\operatorname{Ass}(M/Q_i) = \{p_i\}$，*则* $p_i$ (*i* $\in I$) *不同*。

从$M$中$N$的每个初等分解$N = \bigcap_{i \in I} Q_i$可以推导出$N$中$M$的*减少*初等分解：令$J$是集合的最小元素子集 $I'$ / $I$ 使得 $N = \bigcap_{i \in I'} Q_i$。显然$(Q_i)_{i \in J}$满足条件(a)。那么对于$i \in J$，令$\Phi$为$p_i$的集合；对于所有$p \in \Phi$，令$H(p)$为$i \in J$的集合，使得$p_i = p$并令$Q(p) = \bigcap_{i \in H(p)} Q_i$；从 no. 1 的命题 2 可以得出，$Q(p)$ 相对于 $M$ 是$p$-主要的；此外，$N = \bigcap_{p \in \Phi} Q(p)$和家庭$Q((p))_{p \in \Phi}$因此是$M$中$N$的减少的初等分解。

我们将看到，在no. 2的定理 1的证明中定义的初等分解被*减少了*；这是从以下命题得出的：

#### 命题 4 {#ac-iv-s2-prop-4 .statement tag=04KS}

*设*$M$*为模超过诺特环，M的N子模，M中的N的$N = \bigcap_{i \in I} Q_i$*初等分解，并且对于所有*$i \in I$，*让*$\{p_i\} = \operatorname{Ass}(M/Q_i)$。 *为了减少这个分解，* $p_i$ *不同并且属于到* $\operatorname{Ass}(M/N)$是必要且充分的； *然后*

(2)
$$
\operatorname{Ass}(M/N) = \bigcup_{i \in I} \{p_i\}
$$

(3)
$$
\operatorname{Ass}(Q_i/N) = \bigcup_{j \neq i} \{p_j\} \quad \text{for all } i \in I.
$$

如果满足叙述的条件，则$N = \bigcap_{j \neq i} Q_j$不能成立，因为我们会推出与假设相反的$\operatorname{Ass}(M/N) \subset \bigcup_{j \neq i} \{p_j\}$（§ 1, no. 1，推论2至命题3）；那么$N$的初等分解$(Q_i)_{i \in I}$肯定会减少。反之，$\operatorname{Ass}(M/N) \subset \bigcup_{i \in I} \{p_i\}$始终成立（§ 1, no. 1，推论2至命题3）；另一方面，对于所有$i \in I$，让我们写成$P_i = \bigcap_j Q_j$；则 $P_i \cap Q_i = N$ 和 $P_i \neq N$ 如果 $(Q_i)_{i \in I}$ 约简，因此 $P_i/N$ 非零且同构于 $M/Q_i$、从而 $\{p_i\} = \operatorname{Ass}(P_i/N)$ 的子模 $(P_i + Q_i)/Q_i$ (§ 1, no. 1, 命题) 3 和推论 1 至命题 2)；为$P_i/N \subset M/N, p_i \in \operatorname{Ass}(M/N)$，它完成了叙述和公式（2）中条件的必要性证明。最后，如$N = \bigcap_{j \neq i} (Q_j \cap Q_i), \operatorname{Ass}(Q_i/N) \subset \bigcup_{j \neq i} \operatorname{Ass}(Q_i/(Q_j \cap Q_i))$（§ 1, no. 1，推论2至命题3）；但$Q_i/(Q_j \cap Q_i)$同构于$M/Q_j$的子模$(Q_i + Q_j)/Q_j$，因此$\operatorname{Ass}(Q_i/(Q_j \cap Q_i)) \subset \{p_j\}$和
$$
\operatorname{Ass}(Q_i/N) \subset \bigcup_{j \neq i} \{p_j\};
$$

#### 推论{#ac-iv-s2-n3-cor-1 .statement tag=04KT}

令$A$为诺特环，$M$为$A$模，$M$的$N$子模以及$M$中$N$的$(Q_i)_{i \in I}$初等分解。然后$\mathrm{Card}(I) \geq \mathrm{Card}(\mathrm{Ass}(M/N))$；为了使$(Q_i)_{i \in I}$减少为初等分解，$\mathrm{Card}(I) = \mathrm{Card}(\mathrm{Ass}(M/N))$是必要且充分的。

从命题 4 之前的注可知，$M$中存在$N$的减少初等分解$(R_j)_{j \in J}$，使得$\mathrm{Card}(J) \leq \mathrm{Card}(I)$；第一个断言紧接着第二个断言，后者是命题4的推论。

#### 命题 5 {#ac-iv-s2-prop-5 .statement tag=04KU}

令 $A$ 为诺特环，$M$ $A$ 模块，$M$ 的$N$ 子模，$N = \bigcap_{i \in I} Q_i$ $N$ 的缩减初等分解 $M$，对于所有$i \in I$，让$\{p_i\} = \mathrm{Ass}(M/Q_i)$。如果$p_i$是$\mathrm{Ass}(M/N)$的最小值元素，则$Q_i$等于$N$相对于$p_i$的饱和度（章11，§ 2, no. 4）（cf.习题2）。

显然，我们可以将注意力限制在$N = 0$，替换（如果需要）是$M$乘$M/N$的情况。如果$p_i$在$\mathrm{Ass}(M)$、$\mathrm{Ass}(M)$的元素、集合中最小，且不满足$A - p_i$、约化至$p_i$；然后从上面的公式（3）和典范映射$M \to M_0$的§ 1, no. 2、命题6、核得出命题，等于0相对于$p_i$的饱和度（章11， § 2, no. 4）。

#### 注{#ac-iv-s2-n3-rem-1 .statement tag=04KV}

素理想$p_i \in \mathrm{Ass}(M/N)$不是这个集合的最小元素，是有时，称为与$M/N$相关的*沉浸*素理想；如果 $M/N$ 是有限生成的，对于要浸没的 $p_0 \in \mathrm{Ass}(M/N)$，$V(p_0)$ *不是* $\mathrm{Supp}(M/N)$ 的不可约分量是充分必要的（章 II, § 4, no. 3，推论 2 到命题 14）；如果$(Q(p))_{p \in \mathrm{Ass}(M/N)}$和$(Q'(p))_{p \in \mathrm{Ass}(M/N)}$是$M$中$N$的两个约初等分解，则可能是$Q'(p_0) \neq Q(p_0)$（习题24（c））； $M$中$N$的*规范*减少初等分解可以始终通过在其中出现的主要子模上施加补充条件来定义（习题4）。

### 4. 初等分解的本地化

给定模$M$的子模$N$超过诺特环$A$，为了简化，我们将用$D_I(M/N)$表示，在这个数中，$N$的减少的初等分解的集合 $M$，其索引集合为$I$（相当于$\mathrm{Ass}(M/N)$）。

#### 命题 6 {#ac-iv-s2-prop-6 .statement tag=04KW}

令$A$为诺特环，$M$为$A$模，$N$子模为$M$和$I = \mathrm{Ass}(M/N)$。令$S$为$A$的子集和指标i的$I$由……组成与$J$子集的乘积，使得$S \cap p_i = \varnothing$。令$N'$为$N$相对于$M$中$S$的饱和度。然后：

(i) *如果* $(Q_i)_{i \in I}$ *是* $D_I(M/N)$ 的元素，*族* $(Q_i)_{i \in J}$ *是* $D_J(M/N')$ *的元素，并且家庭* $(S^{-1}Q_i)_{i \in J}$ *是* $D_J(S^{-1}M/S^{-1}N)$ 的元素。

(ii) *映射* $(Q_i)_{i \in J} \to (S^{-1}Q_i)_{i \in J}$ *是* $D_J(M/N')$ *的双射 *到* $D_J(S^{-1}M/S^{-1}N)$。

(iii) *如果* $(Q_i)_{i \in J}$ *是* $D_J(M/N')$ *的元素和* $(R_i)_{i \in I}$ *元素的* $D_I(M/N)$，*族* $(T_i)_{i \in I}$ *使得* $T_i = Q_i$ *对于* $i \in J$ *和* $T_i = R_i$ *对于* $i \in I - J$ *是* $D_I(M/N)$ 的元素。

(i) 我们知道 (no. 1, 命题 3) $i \in J, S^{-1}Q_i$ 是$S^{-1}p_i$ 的主要元素，$i \in I - J, S^{-1}Q_i = S^{-1}M$ 是主要元素；如 $S^{-1}N = \bigcap S^{-1}Q_i$ (章 II, § 2, no. 4)，那么还有 $S^{-1}N = \bigcap_{i \in J} S^{-1}Q_i$。 $i \in J$ 的 $S^{-1}p_i$ 是不同的，并且它们的集合是 $\operatorname{Ass}(S^{-1}M/S^{-1}N)$（$§ 1$、no. 2，命题 5 的推论）；那么 (命题 4) $(S^{-1}Q_i)_{i \in J}$ 是初等分解的减少$S^{-1}N$。此外，$Q_i = (i_M^S)^{-1}(S^{-1}Q_i)$ (no. 1 命题 3)，因此$N' = (i_M^S)^{-1}(S^{-1}N) = \bigcap_{i \in J} Q_i$和$(Q_i)_{i \in J}$显然是$M$中$N'$的减少的初等分解。

(ii) *当* $S^{-1}N' = S^{-1}N$，我们可以通过$N'$ 替换 $N$，即假设$J = I$。 令$(P_i)_{i \in I}$为$S^{-1}M$中$S^{-1}N$的约初等分解，并写为$Q_i = (i_M^S)^{-1}(P_i)$；从 no. 1、命题 3 可以得出，$Q_i$ 是 $p_i$ ($i \in I$) 的主要元素，而 $(Q_i)_{i \in I}$ 则是 $M$ 中 $N$ 的减少的初等分解，凭借 no. 3，推论命题 4. 最后，对于所有$i \in I$和每个子模$Q'_i$，其中$M$凭借no. 1、命题3和假设$J = I$相对于$M, Q'_i = (i_M^S)^{-1}(S^{-1}Q'_i)$是$p_i$主要的，我们看到两个定义了映射$D_I(M/N) \to D_I(S^{-1}M/S^{-1}N)$和$D_I(S^{-1}M/S^{-1}N) \to D_I(M/N)$，其中合成是$D_I(M/N)$和$D_I(S^{-1}M/S^{-1}N)$上的恒等式，证明了(ii)。

(iii) 凭借 (i)、$N' = \bigcap_{i \in J} R_i$、从而

$$
N = N' \cap \bigcap_{i \in I - J} R_i = \left( \bigcap_{i \in J} Q_i \right) \cap \left( \bigcap_{i \in I - J} R_i \right)
$$

紧随no. 3，推论到命题 4，初等分解会减少。

#### 推论{#ac-iv-s2-n4-cor-1 .statement tag=04KX}

*映射*

$$
D_I(M/N) \to D_J(M/N') \quad \text{and} \quad D_I(M/N) \to D_J(S^{-1}M/S^{-1}N)
$$

*在命题 6 (i)* 中定义* *是满射*。

命题 6 (iii) 证明映射 $D_I(M/N) \to D_J(M/N')$ 是满射，命题 6 (ii) 证明映射
$$
D_I(M/N) \to D_J(S^{-1}M/S^{-1}N)
$$
是主观的。

### 5. 环和模 OF 有限长度

如果$A$-模块$M$是有限长度，我们将用$\operatorname{long}_A(M)$或$\operatorname{long}(M)$来表示这个长度。回想一下，每个阿廷环都是诺特（代数，章VIII, § 6, no. 5，推论3到命题12），并且每个有限生成模超过阿廷环都是有限长度（*loc.cit.*，推论1到命题12）。 命题12）。此外，每个阿廷的整环都是域（代数，章VIII, § 6, no. 4，命题9）。

#### 命题 7 {#ac-iv-s2-prop-7 .statement tag=04KY}

*令 $M$ 为有限生成模超过诺特环 $A$。以下属性是等效的：*
(a) $M$ 为有限长度。
(b) *每个理想$p \in \operatorname{Ass}(M)$都是$A$的最大理想。*
(c) *每个理想$p \in \operatorname{Supp}(M)$都是$A$的最大理想。*

令$(M_i)_{0 \leq i \leq n}$为$M$的合成列，使得对于$0 \leq i \leq n - 1$，$M_i/M_{i+1}$同构于$A/p_i$，其中$p_i$是素数（$§ 1$、no. 4、定理1）。如果$M$是有限长度，那么每个$A$-模块$A/p_i$也是，这意味着每个环$A/p_i$都是阿廷的；但由于$A/p_i$是整环，因此是域，其他字$p_i$最大；我们结论 (a) 暗示 (b) ($§ 1$, no. 4, 定理 2)。 条件 (b) 通过 $§ 1$, no. 3, 命题 7 隐含 (c)。最后，如果 $\operatorname{Supp}(M)$ 的所有理想都最大，则 $p_i$ ($§ 1$, no. 4, 定理 2) 也最大，因此$A/p_i$是简单的$A$模块，$M$是有限长度，它完成了证明。

#### 推论 1 {#ac-iv-s2-prop-7-cor-1 .statement tag=04KZ}

*对于有限长度$M$中的每模超过诺特Zing$A$、$\operatorname{Ass}(M) = \operatorname{Supp}(M)$。*

$\operatorname{Supp}(M)$的每个元素在$\operatorname{Supp}(M)$中都是最小的，结论由$§ 1$、no. 3、推论1到命题7得出。

#### 推论 2 {#ac-iv-s2-prop-7-cor-2 .statement tag=04L0}

*设$M$是有限生成模超过诺特环$A$并且$p$是$A$的素理想。为了使$M_p$成为有限长度的非零$A_p$模，$p$是$\operatorname{Ass}(M)$的最小元素是必要且充分的。*

根据$§ 1$、no. 2，推论命题 5，$\operatorname{Ass}_{A_p}(M_p)$ 是理想$q_p$ 的集合，其中$q$ 贯穿$p$ 中包含的$\operatorname{Ass}(M)$ 理想的集合。另一方面，$p_p$是$A_p$的唯一极大理想；到命题 7，要使$M_p$成为有限长度的$A_p$模，$\operatorname{Ass}(M)$中没有元素严格包含在$p$中是必要且充分的。另一方面，对于$M_p \neq 0$，到定义 $p \in \operatorname{Supp}(M)$ (章 11, § 4, no. 4) 是充分必要的，即$\operatorname{Ass}(M)$ ($§ 1$，$p$ 包含元素， no. 3、命题7)。这就证明了推论。

#### 注 (1) {#ac-iv-s2-n5-rem-1 .statement tag=04L1}

设$M$为有限生成模超过诺特环$A$；令$(M_1), \ldots$为$M$的合成列，使得对于$0 \leq i \leq n - 1$，$M_i / M_{i+1}$同构于$A/p_i$，其中$p_i$是$A$的素理想（$§ 1$，no. 4，定理） 1）。如果 $p$ 是 $\operatorname{Ass}(M)$ 的最小元素，则长度 $\operatorname{long}_{A_p}(M_p)$ 等于指标* $i$ 的 *数，从而 $p_i = p$。对于$M$的$(M_i)_p$形式合成列，$(M_i)_p / (M_{i+1})_p$同构于$(A/p_i)_p$，因此如果$p_i \neq p$同构于$\{0\}$（因为$p$在集合中是最小的） $p_i$ 由 $§ 1$、no. 4、定理 2) 到 $(A/p)_p$，即域，如果 $p_i = p$。

#### 命题 8 {#ac-iv-s2-prop-8 .statement tag=04L2}

*令$M$为有限长度的模超过诺特环$A$。*

(i) *相对于由$\operatorname{Ass}(M)$索引的$M$，仅存在$\{0\}$的单个初等分解（必然减少）——令$\{0\} = \bigcap_{p \in \operatorname{Ass}(M)} Q(p)$为分解，其中$Q(p)$是相对于$M$的$p$主要。*

(ii) *存在整数$n_0$，使得对于所有$n \geq n_0$和所有$p \in \operatorname{Ass}(M)$，$Q(p) = p^n M$。*

(iii) *对于所有$p \in \operatorname{Ass}(M)$，$M$到$M_p$的典范映射是满射，其核是$Q(p)$。*

(iv) *$M$到$\bigoplus_{p \in \operatorname{Ass}(M)} (M/Q(p))$的典范嵌入是双射的。*

由于每个元素$p \in \operatorname{Ass}(M)$在$\operatorname{Ass}(M)$（命题7）中都是最小的，断言（i）从no. 3，命题5得出。由于$M$是有限生成的，因此存在$n_0$使得$p^n M \subset Q(p)$对于所有$p \in \operatorname{Ass}(M)$ 和所有 $n \geq n_0$ (no. 1, *注*);但由于$p$是最大理想，$p^n M$相对于$M$而言是$p$主要（no. 1，*例2和3*），并且，作为$\bigcap_{p \in \operatorname{Ass}(M)} p^n M = \{0\}$，它从(i)得出，对于所有$p \in \operatorname{Ass}(M)$必然有$p^n M = Q(p)$； 从而（二）。由于$p^n$对于$p \in \operatorname{Ass}(M)$来说，在对中互质（章 11, § 1, no. 2, 命题 3），典范映射 $M \to \bigoplus_{p \in \operatorname{Ass}(M)} (M/p^n M)$是满射（章 11， § 1, no. 2、命题 6)、从而 (iv)。然后$\operatorname{Ass}(Q(p)) = \operatorname{Ass}(M) - \{p\}$和$\operatorname{Ass}(M/Q(p)) = \{p\}$（no. 3，命题4）；由于$\operatorname{Ass}(M)$中的元素是极大理想，$p$是$\operatorname{Ass}(M)$中唯一不满足$A - p$的元素；因此，$Q(p)$ 是典范映射 $j : M \to M_p$ 中的核（$§ 1$、no. 2、命题 6）。如果 $M/Q(p)$ 的$s \in A - p$、位似与$s$ 的比率由于关系 $\operatorname{Ass}(M/Q(p)) = \{p\}$ (no. 1, 命题 1) 是单射的；因为$M/Q(p)$是阿廷的，所以这个位似是双射的（*代数*，章VIII, § 1, no. 2，引理3）。 典范映射$M \to M/Q(p)$则写作$f \circ j$，其中$f : M_p \to M/Q(p)$是$A$同态（章II, § 2, no. 2，命题3）；因为 $\operatorname{Ker}(j) = \operatorname{Ker}(f \circ j) = Q(p)$，$f$ 是单射；我们结论认为$j$是满射而$f$是双射。

#### 推论{#ac-iv-s2-n5-cor-1 .statement tag=04L3}

*如果M是有限长度的模超过诺特环A，那么*

$$
\operatorname{long}_A(M) = \sum_{p \in \operatorname{Ass}(M)} \operatorname{long}_{A_p}(M_p).
$$

如果我们证明的话，这将由命题 8 (iv)得出

$$
\operatorname{long}_A(M/\mathscr{Q}(p)) = \operatorname{long}_{A_p}(M_p).
$$

现在，从 no. 1 的命题 1 可以得出，对于所有 $s \in A - p$ 位似，$M/\mathscr{Q}(p)$ 上的比率 s 都是单射的； 位似 $M/\mathscr{Q}(p)$ 的每个子模 R 上的比率 s 因此是单射的，并且由于 R 是阿廷的，所以它是双射的 (*代数*, 章 VIII, § 2, no. 2, 引理 3)；我们结论 $M/\mathscr{Q}(p)$ 的子 A 模块是 M 的子 A 模块的双射 $f : M, \to M/\mathscr{Q}(p)$ 下的像，(章 11, § 2, no. 3)，从而我们的断言。

#### 命题 9 {#ac-iv-s2-prop-9 .statement tag=04L4}

*设A为诺特环。以下条件是等效的：*
(a) *为阿廷的。*
(b) *A 中的所有素理想 $\mathfrak{a}$ 都是极大理想。*
(c) *Ass(A) 的所有元素均为极大理想。*

*如果这些条件满足，A只有有限的数素理想，它们都是极大的并且与A-模A相关；此外，A 是半局部环，其雅各布森根是幂零的。*

说A是阿廷的相当于说，A是有限长度的A-模；因此(a)和(c)等价于命题7。显然(b)蕴涵(c)。最后，(a) 蕴含 (b)，因为每个阿廷的整环都是域。因此，性质 (a)、(b) 和 (c) 是等价的。

假设他们持有。由于属于到 Supp(A) 的每个素理想以及 Supp(A) 包含元素 Ass(A) 的每个元素 ($\S$ 1, no. 3, 命题 7)，从 (c) 可以得出 Ass(A) 是A 的所有素理想的集合；那么 A 只有有限的数素理想，所有素理想都是极大的并且与 A-模 A 相关。这显然意味着 A 是半局部的；最后，我们知道阿廷环的雅各布森根式是幂零的（*代数*，章VIII, § 6, no. 4，定理3）。

#### 注 (2) {#ac-iv-s2-n5-rem-2 .statement tag=04L5}

对于 *诺特* 环 A，命题 9 的条件意味着 A 的谱是*有限*且*离散*，因此 Spec(A) 的每个点都是封闭的（章 11、§ 4, no. 3，推论 6 为命题11)。相反，对于 *诺特* 环 A，说 *Spec(A) 的每个点* $\mathfrak{a}$ *都是封闭的*意味着 A 的每个素理想都是最大的 (*loc.cit.*.)，因此这个条件相当于命题 9。

#### 推论 1 {#ac-iv-s2-prop-9-cor-1 .statement tag=04L6}

*每个阿廷环 A 都同构于阿廷的局部环有限族的直接合成。*

由命题 9 和命题 8 (iii) 和 (iv) 可知，如果$(\mathfrak{m}_i)_{1 \leq i \leq n}$ 是$A$ 的极大理想族，则典范映射 $A \to \prod_i A_{\mathfrak{m}_i}$ 是双射的。

#### 注 (3) {#ac-iv-s2-n5-rem-3 .statement tag=04L7}

这个推论也可以从$\operatorname{Spec}(A)$是有限且离散的以及章11、§ 4, no. 3、命题15这一事实推出。

#### 推论 2 {#ac-iv-s2-prop-9-cor-2 .statement tag=04L8}

令$A$为诺特环，且$m$为$A$的理想值。以下条件是等效的：

(a) $A$ 是半局部环，$m$ 是$A$ 的定义理想。
(b) $A$ 是 Zariski 环，带有 $m$-adic 拓扑，$A/m$ 是阿廷的。

如果 (a) 成立，则 $A$ 是具有 $m$-adic 拓扑的 Zariski 环 (章 III, § 3, no. 3, 例 3)；此外，根据$A$的雅各布森根$r$的假设$m$包含幂，$A$的每个素理想其中包含$m$还有包含$r$ （章II, § 1, no. 1，命题1）；因此它是最大的，因为 $r$ 是最大理想的有限交 (\emph{loc. cit.})； 命题 9 那么表明$A/m$ 是阿廷的。相反，如果 (b) 成立，$A$ 包含 $A$ 的雅各布森根式的每个最大理想$p$，因此包含 $m$ (章 III, § 3, no. 3, 命题 6)；由于$A/m$是阿廷的，理想$p/m$在数（命题9）中是有限的，因此$A$只有有限的数最大理想，这意味着它是半局部的。

#### 推论 3 {#ac-iv-s2-prop-9-cor-3 .statement tag=04L9}

令$A, A'$是从$A$到$A'$的两个环和$h$同态。假设 $A$ 是半局部的，诺特并且 $A'$ 是有限生成的 $A$ 模块。那么环$A'$是半局部的，诺特；如果$m$是$A$的定义理想，则$mA'$是$A'$的定义理想。

我们知道 $A'$ 是 Zariski 环与 $mA'$-adic 拓扑 (章 III, § 3, no. 3, 命题 7)。由于$A/m$是阿廷的（推论2）并且$A'/mA'$是有限生成的$(A/m)$模块，$A'/mA'$是阿廷环，因此$A'$是半局部的，而$mA'$是$A'$的定义理想（推论2）。

#### 推论 4 {#ac-iv-s2-prop-9-cor-4 .statement tag=04LA}

令$A$为完全半局部诺特环，$m$为$A$的定义理想，$E$为有限生成的$A$模，$(F_n)$递减序列为子模 $E$使得$\bigcap_n F_n = 0$。那么，对于所有$p > 0$，存在$n > 0$使得$F_n \subset m^p E$。

由于 $A$ 是 Zariski 环，$E$ 是 Hausdorff，并且 $F_n$ 在 $m$-adic 拓扑下闭合。 另一方面，$E$是完整的（章III, § 2, no. 12，推论1到命题16）。 Finally, $E/m^p E$ is a finitely generated module over the ring $A/m^p$, which is Artinian (Corollary 2); then $E/m^p E$ is an Artinian $(A/m^p)$-module and hence an Artinian $A$-module. 然后从章 III, § 2, no. 7、命题 8 得出推论。

#### 推论 5 {#ac-iv-s2-prop-9-cor-5 .statement tag=04LB}

在完全半局部诺特环中，交为0的每个递减序列$\phi$理想都是收敛于0的过滤器基。

将推论 4 应用到 A-模 $\mathbf{A}$ 就足够了。

#### 命题 10 {#ac-iv-s2-prop-10 .statement tag=04LC}

设 $A$ 为诺特环，$p_1, \ldots, p_n$ 为与 A-模 $A$ 相关的素理想，其中 $p_i \neq p_j$ 为 $i \neq j$。

(i) 集合$S = \bigcap_{i=1}^n (A - p_i)$是元素中的集合，而不是$A$中0的除子。

(ii) 如果所有$p_i$都是$\operatorname{Ass}(A)$的最小元素，则$A$的分数$S^{-1}A$的总环为阿廷的。

(iii) 如果减少环$A$，则所有$p_i$都是$\operatorname{Ass}(A)$的最小元素（因此是$\operatorname{Spec}(A)$的最小元素），并且每个$A_{p_i}$都是域；对于每个指标 $i$，典范同态 $S^{-1}A \to A_{p_i}$（章 II, § 2, no. 1，推论 1 到命题 2）是满射，其核是 $S^{-1}p_i$；最后从$S^{-1}A$到$\prod_{i=1}^n (S^{-1}A/S^{-1}p_i)$的典范同态是双射的。

事实上，$S$是元素的集合，而不是$\mathbf{A}$中0的除子，这一事实已经被看到（§ 1, no. 1，推论3到命题2）。 $S^{-1}A$的素理想是形式$S^{-1}p$，其中$p$是$\bigcup_{i=1}^n p_i$（章11、§ 2, no. 5、命题10）中包含的$A$的素理想，$p_i$之一包含（章II, § 1, no. 1，命题2）。如果$p_i$是$\operatorname{Ass}(A)$的最小元素，那么它是$\operatorname{Spec}(A)$的最小元素（§ 1, no. 3，命题7的推论）；如果每个$p_i$都是$\operatorname{Ass}(A)$的最小元素，那么我们可以看到$S^{-1}A$的素理想是$S^{-1}p_i$，因此它们都是极大的，这证明$S^{-1}A$是阿廷的（命题9）。

最后假设环$A$减少了。然后$\bigcap_{i=1}^n p_i = \{0\}$（§ 1, no. 3，推论2到命题7）。我们推断$\{0\} = \bigcap_{i=1}^n p_i$是理想$\{0\}$的*减少*初等分解（no. 3，推论为命题4）；特别是，没有一个$p_i$可以包含和指标$j \neq i$的$p_j$，因此$p_i$都是$\operatorname{Ass}(A)$的最小元素。 环 $S^{-1}A$ 则由 (ii) 得到阿廷的。 $S^{-1}p_i$是与$S^{-1}A$模$S^{-1}A$（§ 1, no. 2，命题5的推论）和$\{0\} = S^{-1} \left( \bigcap_{i=1}^n p_i \right) = \bigcap_{i=1}^n S^{-1}p_i$（章II, § 2, no. 4）相关的素理想；由于$S^{-1}p_i$是不同的，$(S^{-1}p_i)_{1 \leq i \leq n}$是$S^{-1}A$中$\{0\}$的减少的初等分解（no. 3，推论到命题4）。 命题 8 然后表明规范同态： $S^{-1}A \to (S^{-1}A)_{p_i}$ 是满射，且核 $S^{-1}p_i$ 且典范同态 $S^{-1}A \to \prod_{i=1}^n (S^{-1}A/S^{-1}p_i)$ 是双射。我们还知道，典范同态$S^{-1}A \to A$是由g和同构$(S^{-1}A)_{S^{-1}p_i} \to A$（章II, § 2, no. 3，命题7）组成。最后，从命题 8 可以得出，$(S^{-1}A)_{S^{-1}p_i}$ 与 $S^{-1}A/S^{-1}p_i$ 同构的，因此是域，因为 $S^{-1}p_i$ 是极大理想。

### 6. 标量的初等分解和扩张

在这个数中，A和B将表示两个环，我们将考虑环同态$\rho : A \to B$，这使得$B$变成A-代数；回想一下，对于每个 B-模 F，$\rho_*(F)$ 是可交换的群 F，其中 A-模结构由 $a.y = \rho(a)y$ 对于所有 $a \in A, y \in F$ 定义。

#### 引理 1 {#ac-iv-s2-lem-1 .statement tag=04LD}

设 A 为诺特环，$p$ A、E A-模的素理想，其中 $p$ 的湮没子包含幂，并且$\operatorname{Ass}(E) = \{p\}$ 和 F B-模使得 $\rho_*(F)$ 是平面A-模。 条件$\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$则意味着$\rho^{-1}(\mathfrak{P}) = p$。

如果 n 满足 $p^nE = 0$，则$p^nB \subset \operatorname{Ann}(E \otimes_A F)$、从而 $p^nB \subset \mathfrak{P}$，这意味着$p^n \subset \rho_1(\mathfrak{P})$，因此$p \subset \rho_1(\mathfrak{P})$，因为$\rho_1(\mathfrak{P})$ 是素数。此外，如果$a \in A - p$，位似 h 与 E 上的比率 a 是单射的（$§ 1$，no. 1，推出 2 到命题 2）；由于 $h \otimes 1_F$ 是位似 $h'$，$E \otimes_A F$ 上的比率为 $\rho(a)$，并且 $\rho_*(F)$ 是平坦的，$h'$ 是单射 (章 I, § 2, no. 2, 定义 1)；这就证明了$\rho(a) \notin \mathfrak{P}$，从而$\rho^{-1}(\mathfrak{P}) = p$。

#### 定理 2 {#ac-iv-s2-thm-2 .statement tag=04LE}

令$\rho : A \to B$为环同态、E A-模和F B-模，使得$\rho_*(F)$是平坦的A-模。然后

$$
\operatorname{Ass}_B(E \otimes_A F) \supset \bigcup_{p \in \operatorname{Ass}_A(E)} \operatorname{Ass}_B(F/pF).
$$

当A为诺特时，(5)式两边相等。

设 $p \in \operatorname{Ass}_A(E)$； 定义存在正合序列

$$
0 \to A/p \to E.
$$

由于 F 是平的 A-模，我们推导出正合序列

$$
0 \to F/pF \to E \otimes_A F
$$

从而$\operatorname{Ass}_B(F/pF) \subset \operatorname{Ass}_B(E \otimes_A F)$，证明包含式(5)。

现在假设 A 是诺特，让我们证明相反的包含。

我们分阶段进行：

(i) 首先假设 E 为有限生成A-模并且 Ass_A(E) 被简化为单个元素 $p$。通过§ 1, no. 4、定理 1，存在 E 的合成列 $(E_i)_{0 \leq i \leq n}$，使得 $E_i/E_{i+1}$ 同构于 $A/p_i$，其中 $p_i$ 是 A 的素理想；此外（$§ 1$，no. 4，定理2和no. 3，命题7）所有$p_i$包含$p$。由于 F 是降调A-模，$E \otimes_A F$ 和 $(E_i \otimes_A F)/(E_{i+1} \otimes_A F)$ 的 $E_i \otimes_A F$ 形式合成列被标识为
$$
(A/p_i) \otimes_A F = F/p_i F.
$$
那么凭借$§ 1$、no. 1、命题 3
$$
\operatorname{Ass}_B(E \otimes_A F) \subset \bigcup_{i=0}^{n-1} \operatorname{Ass}_B(F/p_i F).
$$
我们知道E被$p$的幂湮灭（no. 1，注）； 引理 1 然后表明，对于所有 $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$，$\rho^{-1}(\mathfrak{P}) = p$。由于$F/p_i F$与$(A/p_i) \otimes_A F$同构的，对于所有$\mathfrak{P}' \in \operatorname{Ass}_B(F/p_i F)$，$\rho^{-1}(\mathfrak{P}') = p_i$同构于引理 1，如果$p_i \neq p$则有从而$\operatorname{Ass}_B(E \otimes_A F) \cap \operatorname{Ass}(F/p_i F) = \varnothing$，这在所考虑的情况下证明了定理。

(ii) 假设 E 是有限生成A-模。令$p_i$ ($1 \leq i \leq n$) 为$\operatorname{Ass}_A(E)$ 的元素，并令$\{0\} = \bigcap^n Q_i$ 为相应的减少初等分解 (no. 3)；那么，E 同构于 $E_i = E/Q_i$ 的直和的子模，并且，由于 F 是平坦的A-模，所以$E \otimes_A F$ 同构于 B-模 $E_i \otimes_A F$ 的直和的子模。我们推论（$§ 1$、no. 1、命题 3 和推论 1 到命题 3）
$$
\operatorname{Ass}_B(E \otimes_A F) \subset \bigcup_{i=1}^n \operatorname{Ass}_B(E_i \otimes_A F).
$$
但是 $E_i$ 是有限生成A-模，因此 $\operatorname{Ass}_A(E_i)$ 被简化为单个元素 $p_i$（no. 1，定义 1）。在本例中，通过 (i)、$\operatorname{Ass}_B(E_i \otimes_A F) = \operatorname{Ass}_B(F/p_i F)$、从而定理。

(iii) *一般情况。*B-模$E \otimes_A F$是子模$E' \otimes_A F$的并，其中$E'$贯穿A-模E的有限生成子模的集合。如果$\mathfrak{P}$ 属于到 $\operatorname{Ass}_B(E \otimes_A F)$，则存在 E 的有限生成子模 $E'$，使得 $\mathfrak{P} \in \operatorname{Ass}_B(E' \otimes_A F)$。由(ii)，存在$p \in \operatorname{Ass}_A(E')$使得$\mathfrak{P} \in \operatorname{Ass}_B(F/pF)$；作为 $\operatorname{Ass}_A(E') \subset \operatorname{Ass}_A(E)$，这完成了定理 2 中的证明。

#### 推出 1 {#ac-iv-s2-thm-2-cor-1 .statement tag=04LF}

*如果 A 是诺特和 $\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$，则 $\rho^{-1}(\mathfrak{P}) \in \operatorname{Ass}_A(E)$ 和 $\rho^{-1}(\mathfrak{P})$ 是 A 的唯一素理想$p$，使得 $\mathfrak{P} \in \operatorname{Ass}_B(F/pF)$。*

#### 推出 2 {#ac-iv-s2-thm-2-cor-2 .statement tag=04LG}

假设 $A$ 和 $B$ 是诺特，并且 $B$ 是平面 $A$ 模。设$p$为$A$的素理想，$Q \subset E$为$p$主子模，$\mathfrak{P}$为$B$的素理想。为了使$Q \otimes_A B$成为$E \otimes_A B$的$q$-初等子模，$pB$是$B$的“p-初等理想”是必要且充分的。

让我们应用定理 2 到 $A$-模块 $E/Q$ 和 $B$-模块 $B$；那么$\operatorname{Ass}_A(E/Q) = \{p\}$和$(E/Q) \otimes_A B$同构于$(E \otimes_A B)/(Q \otimes_A B)$，因此$\operatorname{Ass}_B((E \otimes_A B)/(Q \otimes_A B)) = \operatorname{Ass}_B(B/pB)$同构的。因此，说 $Q \otimes_A B$ 在 $E \otimes_A B$ 中是$\mathfrak{P}$-主要的，意味着 $\operatorname{Ass}_B(B/pB)$ 被简化为 $\mathfrak{P}$，即推论从而。

#### 注 {#ac-iv-s2-n6-rem-1 .statement tag=04LH}

假设$A$和$B$是诺特。设$\mathfrak{P}$为$B$的素理想，并设$p = \overline{\rho}^{-1}(\mathfrak{P})$；让我们写出$S = A - p$，并令$k(p) = S^{-1}(A/p)$为$A/p$的分数的域。由于$\mathfrak{P}$包含$pB$，$\mathfrak{P}/pB$是$B/pB$的素理想。如果 $\rho'$ 是复合同态 $A \xrightarrow{\rho} B \to B/pB$，我们知道 $S^{-1}(B/pB)$ 与环 $(\rho'(S))^{-1}(B/pB)$ 和 $\mathfrak{P}' = S^{-1}(\mathfrak{P}/pB)$ 等同，其理想为环 (章 II, § 2, no. 2, 命题) 6);由于$\mathfrak{P}/pB$不满足$\rho'(S)$，$\mathfrak{P}'$是$S^{-1}(B/pB)$的素理想（章11，§ 2, no. 5，命题11）；此外，$S^{-1}(B/pB)$、$S^{-1}((A/p) \otimes_A B)$、$(S^{-1}(A/p)) \otimes_A B = k(p) \otimes_A B$之间还有典范同构；类似地，$S^{-1}(F/pF)$ 被规范地标识为$k(p) \otimes_A F$。既然如此，在定理2的假设下，*在阶中*$\mathfrak{P} \in \operatorname{Ass}_B(E \otimes_A F)$，*充分必要*$p \in \operatorname{Ass}_A(E)$并且
$$
\mathfrak{P}' \in \operatorname{Ass}_{k(p) \otimes_A B}(k(p) \otimes_A F).
$$
对于定理 2 及其推论 1，相当于验证条件
$$
\text{``}\mathfrak{P} \in \operatorname{Ass}_B(F/pF)\text{''} \quad \text{and} \quad \text{``}\mathfrak{P}' \in \operatorname{Ass}_{k(p) \otimes_A B}(k(p) \otimes_A F)\text{''}
$$
是等价的；但是，由于$B$是诺特，这是从§ 1, no. 2、命题5的推论以及上述识别得出的。

#### 命题 11 {#ac-iv-s2-prop-11 .statement tag=04LI}

假设 $A$ 和 $B$ 是诺特并且 $B$ 是一个平面 $A$ 模。令$E$为$A$模，$E'$子模为$E$，这样，对于每个理想$p \in \operatorname{Ass}_A(E/E')$，$pB$是$B$或等于$B$的素理想。令$E' = \bigcap_{p \in \operatorname{Ass}(E/E')} Q(p)$是$E$中$E'$的减少初等分解，$Q(p)$是所有$p \in \operatorname{Ass}(E/E')$的$p$-主要。
(i) *如果* $p \in \operatorname{Ass}(E/E')$ *且* $pB = B$，*则* $Q(p) \otimes_A B = E \otimes_A B$。
(ii) *如果* $p \in \operatorname{Ass}(E/E')$ *且* $pB$ *是素数*，$Q(p)$ *是* $pB$*-主* *在* $E \otimes_A B$ 中。
(iii) *如果* $\Phi$ *是集合* $\mathfrak{p} \in \operatorname{Ass}(E/E')$ *使得* $pB$ *是质数*，*那么*
$$
E' \otimes_A B = \bigcap_{p \in \Phi} (Q(p) \otimes_A B)
$$
*这个关系是*$E' \otimes_A B$*在*$E \otimes_A B$中减少的初等分解。

如果 $pB = B$、定理 2 应用于 $E/\mathbf{Q}(p)$ 和 $B$ 表明
$$
\operatorname{Ass}_B((E/\mathbf{Q}(p)) \otimes_A B) = \varnothing
$$
并且，由于 $B$ 是诺特并且是一个扁平的 $A$ 模块，因此我们结论（§ 1, no. 1，推论 1 到命题 2）即 $\mathbf{Q}(p) \otimes_A B = E \otimes_A B$。 断言 (ii) 由推论 2 得出定理 2，取 $\mathfrak{P} = pB$。最后，关系$E' \otimes_A B = \bigcap_{p \in \Phi} (\mathbf{Q}(p) \otimes_A B)$源自$B$是一个扁平的$A$模（章I, § 2, no. 6，命题6）；如$p = \overline{\rho}^{-1}(pB)$代表$p \in \Phi$（引理1），$pB \neq p'B$代表集合$\Phi$的两个不同理想$p, p'$；另一方面，
$$
\operatorname{Ass}((E \otimes_A B)/(E' \otimes_A B)) = \Phi
$$
定理2；我们从no. 3，命题 4 开始结论
$$
E' \otimes_A B = \bigcap_{p \in \Phi} (\mathbf{Q}(p) \otimes_A B)
$$
是减少的初等分解。

#### 推论{#ac-iv-s2-n6-cor-1 .statement tag=04LJ}

*假设* $pB$ *对所有的素数*$p \in \operatorname{Ass}_A(E/E')$。 *那么，如果*$p_1, \ldots, p_n$*是*$\operatorname{Ass}_A(E/E')$的最小元素，*则*$p_iB$*是*元素的最小
$$
\operatorname{Ass}_A((E \otimes_A B)/(E' \otimes_A B)).
$$
从命题 11 可以得出，在这种情况下，$p_iB \neq p_jB$ 对应于 $i \# j$。

*例*
(1) 取$B = S^{-1}A$，其中$S$是$A$的乘法子集；如果$A$是诺特，则满足命题11的假设，并且我们恢复no. 4的命题6的部分。
(2) 令$A$为诺特环，$m$为$A$的理想，$B$为$A$相对于$m$进数拓扑的Hausdorff完成；那么$B$是一个扁平的$A$模，定理2可以与$F = B$一起应用；但一般来说，命题 11 的假设不满足$A$ 的素理想（章 III, § 2，习题 15 (b)）。
(3) 设$A$为诺特环，$B$为多项式代数$A[X_1, \ldots, X_n]$； $B$ 是诺特，并且是一个免费的 $A$ 模块，因此是扁平的。 另外，如果$p$是$A$的素理想，则$B/pB$同构于$(A/p)[X_1, \ldots, X_n]$，即整环，因此$pB$是素数；因此，对于每个$A$模块$E$和$E$的每个子模$E'$，命题11的假设都得到满足。
(4) 令$A$为$k$在域$k$、$K$扩张上的有限生成代数，以及通过扩张获得的$K$上的$B = A \otimes_k K$代数标量； $A$和$B$是诺特，$B$是一个免费的$A$模块，因此定理2可以应用于$F = B$。 在某些情况下（对于例，如果$k$是代数封闭的），可以证明对于$A$的每个素数理想$p$，$pB$是素数或等于$B$；我们稍后会回到这个例。

### 习题{#ac-iv-s2-exercises}

§ 2](exercises/s2/)参见[习题。
