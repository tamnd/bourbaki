---
book: ac
book_title: Commutative Algebra
chapter: IV
chapter_title: ASSOCIATED PRIME IDEALS AND PRIMARY DECOMPOSITION
section: 1
section_title: Prime ideals associated with a module
lang: zh
source: ac-i-vii
book_pages: 261-267, 286-290
pdf_pages: 0281-0287, 0306-0310
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF ASSOCIATED PRIME IDEALS
      page: 261
      pdf_page: 281
    - "no": 2
      title: LOCALIZATION OF ASSOCIATED PRIME IDEALS
      page: 263
      pdf_page: 283
    - "no": 3
      title: RELATIONS WITH THE SUPPORT
      page: 265
      pdf_page: 285
    - "no": 4
      title: THE CASE OF FINITELY GENERATED MODULES OVER A NOETHERIAN RING
      page: 265
      pdf_page: 285
statements: 24
exercises: 19
content_sha256: adc0381ee4c2fa61d22dbcdd510f5d1b490f1125b1e15b7156e0621cc631fa99
translated_from: content/en/ac/IV/01_s1_prime_ideals_associated_with_a_module.md
translation_method: google
source_content_sha256: 41bc8b6bc73ee003f10c2b0789585e99cc74ba8b5cfcd5f713cf440dd2d53406
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 77fc82be215326fff5611639833d566f6d91ee56d1bdb276fcfbbe2dd487a39f
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 1. 与模相关的素理想

### 1. 定义相关素理想

#### 定义 1 {#ac-iv-s1-def-1 .statement tag=04J7}

令 M 为模大于环 A。如果存在 x ∈ M 使得 p 等于湮没子 & x，则称素理想 p 与 M 相关。与 M 相关的素理想的集合表示为 Ass_A(M)，或简称为 Ass(M)。

\* 例。令 a 为多项式环 A = \mathbf{C}[X_1, ..., X_n], V 相应的仿射代数簇中的理想，V_1, ..., V_p 为 V 的不可约分量。如果M被取为函数的环A/a，其在V上是正则的，则与M相关的素理想集合由V_1，...，V_p的理想和一般其他素理想组成，其中每个包含V_i的理想之一。 \*

由于 0 的湮没子是 A，元素 x ∈ M，其湮没子是素理想，则必然 ≠ 0。 说一个素思想 p 与 M 相关联

(*) 本章的结果仅取决于本书I至VI和章I至III，不包括章I, § 4和章III, § 5。

amounts to saying that $M$ contains a submodule *isomorphic to* $A/p$ (namely $Ax$, for all $x \in M$ whose annihilator is $p$).

如果$A$-模块$M$是子模族$(M_i)_{i \in I}$的并，那么显然
$$
\operatorname{Ass}(M) = \bigcup_{i \in I} \operatorname{Ass}(M_i).
$$

#### 命题 1 {#ac-iv-s1-prop-1 .statement tag=04J8}

*对于环$A$的每个素理想$p$和$A/p$、$\operatorname{Ass}(M) = \{p\}$的每个子模$M \neq 0$。*

由于环$A/p$为整环，所以$A/p$的元素$\neq 0$的湮没子为$p$。

#### 命题 2 {#ac-iv-s1-prop-2 .statement tag=04J9}

*令 $M$ 为模超过环 $A$。 $A$的理想$\operatorname{Ann}(x)$的每个极大元素，集合，其中$x$贯穿元素的集合，$M$的$\neq 0$，属于到$\operatorname{Ass}(M)$。*

令$a = \operatorname{Ann}(x)$ ($x \in M, x \neq 0$) 为极大元素；只要证明 $a$ 是素数就足够了。如$x \neq 0$、$a \neq A$。令$b, c$为$A$的元素，使得$bc \in a$和$c \notin a$。然后是$cx \neq 0$、$b \in \operatorname{Ann}(cx)$和$a \subset \operatorname{Ann}(cx)$。由于$a$最大，$\operatorname{Ann}(cx) = a$，从而$b \in a$，所以$a$是质数。

#### 推论 1 {#ac-iv-s1-prop-2-cor-1 .statement tag=04JA}

*设$M$为模超过诺特环$A$。那么条件$M \neq \{0\}$相当于$\operatorname{Ass}(M) \neq \varnothing$。*

如果$M = \{0\}$，显然$\operatorname{Ass}(M)$是空的（$A$上没有任何假设）。如果形式$\operatorname{Ann}(x)$的理想$M \neq \{0\}$、集合非空且由理想$\# A$组成，其中$x \in M$和$x \neq 0$；因为$A$是诺特，所以这个集合有极大元素；那么应用命题2就足够了。

#### 推论 2 {#ac-iv-s1-prop-2-cor-2 .statement tag=04JB}

*令$A$为诺特环，$M$为$A$模，$a$元素为$A$。为了使$M$上的位似与比率$a$是单射的，$a$属于没有与$M$相关的素理想是必要且充分的。*

如果$a$属于到素理想$p \in \operatorname{Ass}(M)$，则$p = \operatorname{Ann}(x)$，其中$x \in M, x \neq 0$； 从而 $ax = 0$ 和位似与比率 $a$ 不是单射。相反，如果$ax = 0$对于某些$x \in M$使得$x \# 0$，则$Ax \# \{0\}$，从而$\operatorname{Ass}(x) \neq \varnothing$（推论1）。设 $p \in \operatorname{Ass}(Ax)$；那么显然$p \in \operatorname{Ass}(M)$和$p = \operatorname{Ann}(bx)$，其中$b \in A$； 从而$a \in p$，从$abx = 0$开始。

#### 推论 3 {#ac-iv-s1-prop-2-cor-3 .statement tag=04JC}

*诺特环$A$中零除子集合是理想的$p \in \operatorname{Ass}(A)$并。*

#### 命题 3 {#ac-iv-s1-prop-3 .statement tag=04JD}

*令$A$为环，$M$为$A$模，$N$为$N$的子模。然后*
$$
\operatorname{Ass}(N) \subset \operatorname{Ass}(M) \subset \operatorname{Ass}(N) \cup \operatorname{Ass}(M/N).
$$
*包含$\operatorname{Ass}(N) \subset \operatorname{Ass}(M)$是明显的。设$p \in \operatorname{Ass}(M)$、$E$为$M$的子模，与$A/p$和$F = E \cap N$同构的。如果$F = \{0\}$、$E$同构于$M/N$、从而$p \in \operatorname{Ass}(M/N)$的*子模。如果$F \neq \{0\}$，则$F$的每一个元素$\neq 0$的湮没子是$p$（命题1），因此$p \in \operatorname{Ass}(F) \subset \operatorname{Ass}(N)$。

#### 推论 1 {#ac-iv-s1-prop-3-cor-1 .statement tag=04JE}

*如果A-模$M$是子模家庭$(M_i)_{i \in I}$的直和，则*$\operatorname{Ass}(M) = \bigcup_{i \in I} \operatorname{Ass}(M_i)$。

它可以通过(1)简化为$I$有限的情况，然后简化为$\operatorname{Card}(I) = 2$在$\operatorname{Card}(I)$上乘以归纳的情况。然后令$I = \{i, j\}$，其中$i \neq j$；因为$M/M_i$同构于$M_j$、$\operatorname{Ass}(M) \subset \operatorname{Ass}(M_i) \cup \operatorname{Ass}(M_j)$ (命题 3)；而且，$\operatorname{Ass}(M_i)$和$\operatorname{Ass}(M_j)$包含在$\operatorname{Ass}(M)$（命题3）、从而结果中。

#### 推论 2 {#ac-iv-s1-prop-3-cor-2 .statement tag=04JF}

*令$M$为A-模，且$(Q_i)_{i \in I}$为$M$的子模的有限族。如果*$\bigcap_{i \in I} Q_i = \{0\}$，*那么*
$$
\operatorname{Ass}(M) \subset \bigcup_{i \in I} \operatorname{Ass}(M/Q_i).
$$
典范映射 $M \to \bigoplus_{i \in I} (M/Q_i)$ 是单射；那么就满足应用命题 3 及其推论 1。

#### 命题 4 {#ac-iv-s1-prop-4 .statement tag=04JG}

*令 $M$ 为 A-模，且 $\operatorname{Ass}(M)$ 为 $\Phi$ 子集。那么存在$M$的子模$N$使得*$\operatorname{Ass}(N) = \operatorname{Ass}(M) - \Phi$*和*$\operatorname{Ass}(M/N) = \Phi$。

令 $\mathscr{E}$ 为子模 $P$ $M$ 的集合，使得$\operatorname{Ass}(P) \subset \operatorname{Ass}(M) - \Phi$。 公式 (1) 表明集合 $\mathscr{E}$ 按包含排序，是*归纳*；此外，$\{0\} \in \mathscr{E}$，因此$\mathscr{E} \neq \varnothing$。设$N$为$\mathscr{E}$的极大元素。然后$\operatorname{Ass}(N) \subset \operatorname{Ass}(M) - \Phi$。我们将看到$\operatorname{Ass}(M/N) \subset \Phi$，到命题 3，将完成证明。让$p \in \operatorname{Ass}(M/N)$；那么 $M/N$ 包含子模 $F/N$ 同构于 $A/p$。 命题 1 和 3，$\operatorname{Ass}(F) \subset \operatorname{Ass}(N) \cup \{p\}$。由于$N$在$\mathscr{E}$、$F \notin \mathscr{E}$中最大，因此$p \in \Phi$最大。

### 2. 相关素数理想的本地化

#### 命题 5 {#ac-iv-s1-prop-5 .statement tag=04JH}

*令$A$为环，$S$不满足$S$和$M$的$A$素理想的$A$，$\Phi$集合的乘法子集 A-模。然后*：
(i) *映射* $p \mapsto S^{-1}p$ *是* $\operatorname{Ass}_A(M) \cap \Phi$ 的双射 *到* $\operatorname{Ass}_{S^{-1}A}(S^{-1}M)$ 的子集。
(ii) *如果* $p \in \Phi$ *是有限生成的理想且* $S^{-1}p \in \operatorname{Ass}_{S^{-1}A}(S^{-1}M)$，*则* $p \in \operatorname{Ass}_A(M)$。

回想一下（章 II, § 2, no. 5，命题 11），映射$p \mapsto S^{-1}p$是$\Phi$的双射到$S^{-1}A$素理想的集合。如果$p \in \operatorname{Ass}_A(M) \cap \Phi$，$p$是$M$的单生子模$N$的湮没子；那么$S^{-1}p$是$S^{-1}M$的单生子模$S^{-1}N$的湮没子（章II, § 2, no. 4，公式（9）），因此$S^{-1}\mathfrak{p} \in \mathrm{Ass}_{S^{-1}A}(S^{-1}M)$。相反，假设$\mathfrak{p} \in \Phi$是有限生成的，并且$S^{-1}\mathfrak{p}$与$S^{-1}M$相关联；则存在$x \in M$和$t \in S$，使得$S^{-1}\mathfrak{p}$是$x/t$的湮没子。设$(a_i)_{1 \leq i \leq n}$为$\mathfrak{p}$生成元系统；那么$(a_i/1)(x/t) = 0$，因此存在$s_i \in S$使得$s_i a_i x = 0 \ (1 \leq i \leq n)$。让我们写$s = s_1 s_2 \ldots s_n$；对于所有 $a \in \mathfrak{p}$、$s a x = 0$、从而 $p \subset \mathrm{Ann}(s x)$；另一方面，如果$b \in A$满足$b s x = 0$，则$b/1 \in S^{-1}\mathfrak{p}$乘以定义，从而$b \in \mathfrak{p}$。然后是$\mathfrak{p} = \mathrm{Ann}(s x)$和$\mathfrak{p} \in \mathrm{Ass}_A(M)$。

#### 推论{#ac-iv-s1-n2-cor-1 .statement tag=04JI}

*如果环 A 是诺特，则映射 $\mathfrak{p} \mapsto S^{-1}\mathfrak{p}$ 是$\mathrm{Ass}_A(M) \cap \Phi$ 的双射到$\mathrm{Ass}_{S^{-1}A}(S^{-1}M)$。*

如果 A 不是诺特，$\mathrm{Ass}_A(M) \cap \Phi$ 到 $\mathrm{Ass}_{S^{-1}A}(S^{-1}M)$ 的映射 $p \mapsto S^{-1}p$ 不一定是满射（习题 1）。

#### 命题 6 {#ac-iv-s1-prop-6 .statement tag=04JJ}

*设A为诺特环，M A-模，S为A的子集和$\mathrm{Ass}_A(M)$的元素的Y集合，不满足S。则典范映射的核N $M \to S^{-1}M$是M唯一的子模，满足关系*

$$
\mathrm{Ass}(N) = \mathrm{Ass}(M) - \Psi, \quad \mathrm{Ass}(M/N) = \Psi.
$$

到no. 1的命题4，M中存在满足关系$\mathrm{Ass}(N') = \mathrm{Ass}(M) - Y$和$\mathrm{Ass}(M/N') = \Psi$的子模$N'$。我们需要证明$N = N'$。考虑交换律图表

$$
\begin{array}{ccc}
M & \xrightarrow{p} & M/N' \\
|u| & & |v| \\
S^{-1}M & \xrightarrow{S^{-1}p} & S^{-1}(M/N')
\end{array}
$$

其中$p, u, v$是典范同态。我们将证明$S^{-1}p$和$v$是单射的，这将证明$u$和$p$具有相同的核，因此$N = N'$。

作为$\mathrm{Ass}(N') \cap \Psi = \varnothing$，$\mathrm{Ass}(N')$的每一个元素都满足S。然后$\mathrm{Ass}_{S^{-1}A}(S^{-1}N') = \varnothing$（推论到命题5），从而$S^{-1}N' = \{0\}$（no. 1，推论1到命题2），这证明了$S^{-1}p$是单射 (章 II, §2, no. 4, 定理 1)。另一方面，如果$x$属于到$v$的核K，则$\mathrm{Ann}(x) \cap S \neq \varnothing$(章II, §2, no. 2，命题4)；因此从 $\mathrm{Ass}(K) \subset \mathrm{Ass}(M/N') = \Psi$ 开始$\mathrm{Ass}(K) = \varnothing$；我们推断$K = \{0\}$（no. 1，推论1到命题2）和$v$是单射的。

### 3. 关系的支持

令 M 为环 A 上的模。回想一下 A 的素理想 $\mathfrak{p}$ 的集合，使得 $M, \neq 0$ 称为 M 的支持，并用 $\operatorname{Supp}(M)$ (章 II, § 4, no. 4, 定义 5) 表示。

#### 命题 7 {#ac-iv-s1-prop-7 .statement tag=04JK}

设 A 为环，M 为 A-模。

(i) 包含元素$\in \operatorname{Ass}(M)$属于到$\operatorname{Supp}(M)$的每个素理想$\mathfrak{p}$。

(ii) 相反，如果 A 是诺特，则每个理想 $\mathfrak{p} \in \operatorname{Supp}(M)$ 包含元素 $\in \operatorname{Ass}(M)$。

如果$\mathfrak{p}$包含元素$q$等于$\operatorname{Ass}(M)$，则$q \cap (A - \mathfrak{p}) = \varnothing$，因此，如果我们写$S = A - \mathfrak{p}$，$S^{-1}\mathfrak{p}$是与$S^{-1}M = M$相关的素理想，（no. 2，命题5）和*更不必说* $M, \# 0$，因此$\mathfrak{p} \in \operatorname{Supp}(M)$。相反，如果 A 是诺特，则 A 也是，（章 II, § 2, no. 4，推出 2 到命题 10）。如果$M_{\mathfrak{p}} \neq 0$，则$\operatorname{Ass}_{A_{\mathfrak{p}}}(M_{\mathfrak{p}}) \neq 0$（no. 1，推论1到命题2），因此存在$q \in \operatorname{Ass}_A(M)$使得$q \cap (A - \mathfrak{p}) = \varnothing$（no. 2，推论到命题5）。

#### 推出 1 {#ac-iv-s1-prop-7-cor-1 .statement tag=04JL}

如果 M 是模超过诺特环，则 $\operatorname{Ass}(M) \subset \operatorname{Supp}(M)$ 和这两个集合具有相同的最小值元素。

#### 推出 2 {#ac-iv-s1-prop-7-cor-2 .statement tag=04JM}

诺特环 A 的零根是理想$\mathfrak{p} \in \operatorname{Ass}(A)$ 的交。

我们知道 A 的零根是 $\operatorname{Spec}(A) = \operatorname{Supp}(A)$ 的最小值元素 (章 II, § 2, no. 6, 命题 13) 的交。

### 4.有限生成模超过诺特环的情况

#### 定理 1 {#ac-iv-s1-thm-1 .statement tag=04JN}

设 A 为诺特环，M 有限生成A-模。 M 存在合成列 $(M_i)_{0 \leq i \leq n}$，使得对于$0 \leq i \leq n - 1$，$M_i / M_{i+1}$ 同构于$A / \mathfrak{p}_i$，其中$\mathfrak{p}_i$ 是A 的素理想。

令$\mathscr{G}$为M的子模的集合，其中合成列和性质为叙述。由于$\mathscr{G}$非空（对于$\{0\}$属于到$\mathscr{G}$）并且M是诺特，$\mathscr{G}$有极大元素N。如果$M \neq N$，则$M/N \neq 0$，因此$\operatorname{Ass}(M/N) \neq \varnothing$（no. 1，推论1至命题2)； $M/N$因此包含子模$N'/N$同构于形式$A/\mathfrak{p}$的A-模，其中$\mathfrak{p}$是质数；然后乘定义$N' \in \mathscr{G}$，其中与……矛盾是N的最大特征标。那么必然是$N = M$。

#### 定理 2 {#ac-iv-s1-thm-2 .statement tag=04JO}

令 M 为诺特环 A 上的有限生成模和 M 的 $(M_i)_{0 \leq i \leq n}$ 合成列，使得对于 $0 \leq i \leq n - 1$，$M_i / M_{i+1}$ 同构于 $A / \mathfrak{p}_i$，其中 $\mathfrak{p}_i$ 是 A 的素理想。然后

(4)
$$
\operatorname{Ass}(M) \subset \{\mathfrak{p}_0, \ldots, \mathfrak{p}_{n-1}\} \subset \operatorname{Supp}(M);
$$

这三个集合的最小值元素相同，且重合与素理想包含Ann(M)的集合的最小值元素相同。

包含于 Ass(M) $\subset \{p_0, \ldots, p_{n-1}\}$ 紧随no. 1 的命题 1 和 3。对于$0 \leq i \leq n - 1$，

$$
p_i \in \operatorname{Supp}(A/p_i) = \operatorname{Supp}(M_i/M_{i+1})
$$

(章 II, § 4, no. 4, 例), 从而 $p_i \in \operatorname{Supp}(M_i) \subset \operatorname{Supp}(M)$ (章 II, § 4, no. 4, 命题 16)，显示包含

$$
\{p_0, \ldots, p_{n-1}\} \subset \operatorname{Supp}(M).
$$

推论1到no. 3的命题7表明Ass(M)和Supp(M)具有相同的最小元素，并且(4)表明这些只是$\{p_0, \ldots, p_{n-1}\}$的最小元素。然后从章 II, § 4, no. 4、命题 17 开始最后一个断言。

#### 推论{#ac-iv-s1-n4-cor-1 .statement tag=04JP}

*如果 M 是有限生成模超过诺特环 A，则 Ass(M) 是有限的。*

在定理2的条件下，集合$\{p_0, \ldots, p_{n-1}\}$不一定由M唯一确定；特别是它可能与 Ass(M) (习题 6) 不同。

#### 命题 8 {#ac-iv-s1-prop-8 .statement tag=04JQ}

*设A为诺特环，A和M有限生成A-模的理想。以下条件是等效的：*

(a) *M 存在元素 x $\# O$，使得 $ax = 0$。*
(b) *对于所有 $a \in a$，存在 M 的元素 x $\neq O$，使得 $ax = 0$；*
(c) *存在$p \in \operatorname{Ass}(M)$使得$a \subset p$。*

显然（a）意味着（b）。根据no. 1，推论2到命题2，条件(b)意味着理想a包含在与M相关的素理想的并中，因此包含在其中一个中，因为Ass(M)是有限的(章11，§ 1, no. 1， 命题2);因此(b)意味着(c)。最后，如果存在$p \in \operatorname{Ass}(M)$使得$a \subset p$，则p是M（no. 1，定义1）的元素$x \neq 0$和$ax = 0$的湮没子；因此(c)意味着(a)。

#### 命题 9 {#ac-iv-s1-prop-9 .statement tag=04JR}

*设A为诺特环，A和M有限生成A-模的理想。为了存在整数$n > 0$使得$a^n M = 0$，a包含在与M相关的素理想的交中是必要且充分的。*

这个交也是Supp(M)的最小元素（no. 3，推论1到命题7），并且说a包含在这个交中相当于说，即记号中的$V(a) \supset \operatorname{Supp}(M)$ 章II, § 4；然后从章 11、§ 4, no. 4、推论2到命题 17得出结论。

#### 定义 2 {#ac-iv-s1-def-2 .statement tag=04JS}

给定一个$A$模$M$，自同态$u$为$M$，如果对于所有$x \in M$，存在整数$n(x) > 0$使得$u^{n(x)}(x) = 0$，则称为几乎幂零。

如果 $M$ 是有限生成的，则几乎所有幂零自同态都是幂零的。

#### 推论{#ac-iv-s1-n4-cor-2 .statement tag=04JT}

设$A$为诺特环。 $M$ 一个 $A$ 模块和 $A$ 的 $a$ 元素。为了使$M$的同态$a_M : x \mapsto ax$几乎为零，$a$属于对于$\operatorname{Ass}(M)$的每个理想是充分必要的。

叙述的条件等价于说，对于所有$x \in M$，存在$n(x) > 0$使得$(Aa)^{n(x)}(Ax) = 0$；通过命题 9，这也意味着$a$属于与子模$Ax$相关的$M$的所有素理想；然后从以下事实得出推论：$\operatorname{Ass}(M)$ 是$\operatorname{Ass}(Ax)$ 的并，其中$x$ 穿过$M$（no. 1，公式 (1)）。

#### 命题 10 {#ac-iv-s1-prop-10 .statement tag=04JU}

令$A$为诺特环，$E$为有限生成的$A$模块，$F$为$A$模块。然后

$$
\operatorname{Ass}(\operatorname{Hom}_A(E, F)) = \operatorname{Ass}(F) \cap \operatorname{Supp}(E).
$$

通过假设，$E$同构于形式$A^n/R$的$A$模，因此$\operatorname{Hom}_A(E, F)$同构于$\operatorname{Hom}_A(A^n, F)$的子模，而后者又同构于$F^n$；现在，$\operatorname{Ass}(F^n) = \operatorname{Ass}(F)$（no. 1，推论 1 到命题 3）；因此$\operatorname{Ass}(\operatorname{Hom}_A(E, F)) \subset \operatorname{Ass}(F)$。另一方面，

$$
\operatorname{Supp}(\operatorname{Hom}_A(E, F)) \subset \operatorname{Supp}(E):
$$

对于$A$的每个素理想$p$，$\operatorname{Hom}_{A_p}(E_p, F_p)$同构于$(\operatorname{Hom}_A(E, F))_p$（章11，§ 2, no. 7，命题19），从而我们的断言立即；那么我们从定理 2 结论得到

$$
\operatorname{Ass}(\operatorname{Hom}_A(E, F)) \subset \operatorname{Supp}(E).
$$

相反，令$p$为$A$属于到$\operatorname{Ass}(F) \cap \operatorname{Supp}(E)$的素理想。由定义，$F$包含子模同构于$A/p$。另一方面，由于$E$是有限生成的，而$E, \neq 0$，我们知道从$E$到$A/p$存在同态$w \neq 0$（章II, § 4, no. 4，命题20）。因为从$A/p$到$F$、$j \circ w \in \operatorname{Hom}(E, F)$和$j \circ w \neq 0$存在单同态$j$。另一方面，关系$aw = 0$对于某些$a \in A$相当于$a \in p$，$A/p$的每元素$\neq 0$中的湮没子是$p$；那么当然$p \in \operatorname{Ass}(\operatorname{Hom}_A(E, F))$。

### 习题 {#ac-iv-s1-exercises}

§ 1](exercises/s1/)参见[习题。
