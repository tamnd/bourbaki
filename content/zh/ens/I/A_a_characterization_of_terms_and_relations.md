---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 0
section_title: Characterization of terms and relations
appendix: true
lang: zh
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 50-55, 60-64
pdf_pages: 0057-0062, 0067-0071
extraction: ocr
subsections:
    - "no": 1
      title: SIGNS AND WORDS
      page: 50
      pdf_page: 57
    - "no": 2
      title: SIGNIFICANT WORDS
      page: 51
      pdf_page: 58
    - "no": 3
      title: CHARACTERIZATION OF SIGNIFICANT WORDS
      page: 51
      pdf_page: 58
    - "no": 4
      title: APPLICATION TO ASSEMBLIES IN A MATHEMATICAL THEORY
      page: 53
      pdf_page: 60
statements: 7
exercises: 8
content_sha256: 4a5de8a297faa16bbcf0d48793a9c12dd96d5895f346f50158036ca004382525
translated_from: content/en/ens/I/A_a_characterization_of_terms_and_relations.md
translation_method: google
source_content_sha256: 13db39e88a8780043e156517521974c8c14af043efeaa643d5625514ba9d1ea2
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 72d1289fe6db8966f7c93b210fde7a5433ab93862a4467835dd5a3542027c893
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## 附录

# 刻画的项与关系

正如我们在引言中所说，当元数学超越了当前章的初级水平时，它会大量利用数学结果。这个附录的目的是给出这个型的推理[^1]的简单例。我们将首先建立“自由半群”数学理论属于的某些结果；然后我们将在元数学“应用”中使用这些结果来获得理论中项与关系的刻画。

### 1. 符号与字

\* 令 S 为非空集合，其元素将被称为 *signs* （这个术语适合我们心目中的元数学应用）。设$\mathrm{L}_0(\mathrm{S})$为S生成的自由半群； $\mathrm{L}_0(\mathrm{S})$的元素称为*字*，并与S的元素的有限序列$A = (s_i)_{0 \leqslant i \leqslant n}$标识。$\mathrm{L}_0(\mathrm{S})$中的合成的律将被乘法写入，因此$AB$是$A$和$B$并列得到序列。空的字$\emptyset$是$\mathrm{L}_0(\mathrm{S})$的单位元素。我们记得，字$A \in \mathrm{L}_0(\mathrm{S})$的*长度*$l(A)$是序列$A$中元素的数；因此 $l(AB) = l(A) + l(B)$ 和长度 1 的字是符号。让$\mathrm{L}(\mathrm{S})$表示$\mathrm{L}_0(\mathrm{S})$中非空字的集合。
¶ 此外，假设我们将 S 的映射 $s \rightarrow n(s)$ 放入整数 $\geqslant 0$ 的集合 $\mathbf{N}$ 中。对于 L(S) 的每个非空字 $A = (s_i)_{0 \leqslant i \leqslant k}$，我们将

$$n(A) \;=\; \sum_{i=0}^{k} \, n(s_i)$$

和$n(\emptyset) = 0$。 $n(A)$称为$A$的*权*。显然$n(AB) = n(A) + n(B)$。 ¶ 如果 $A = A'BA''$，字 $B$ 被称为 $A$ 的*段*（如果也是 $B \neq A$，则为*正确的*段）。如果$A'$（或$A''$）为空，则$B$被称为$A$的*初始*（或*最终*）段。如果 $l(A') = k$，则$B$ *从第 $(k+1)$ 位置开始*。

¶ 如果$A = BCDEF$（其中字$B$、$C$、$D$、$E$、$F$可能为空）段、$C$和$A$的$E$成为*不相交的*。

### 2. 有意义字

*重要的序列* 是 $\mathrm{L}_0(\mathrm{S})$ 的字中的任何序列 $(A_j)_{1 \leqslant j \leqslant n}$ 以及以下性质 ：对于序列的每个字 $A_i$，以下两个之一条件满意：

(1) $A_i$ 是权 0 的符号。

(2) 序列中存在$p$字$A_{i_1}$、$A_{i_2}$、…、$A_{i_p}$，且指标小于$i$，且权的符号$f$ $p$ 这样

$$A_i = f\, A_{i_1} A_{i_2} \, \ldots \, A_{i_p}.$$

出现在有意义的序列中的字称为*有意义字*。然后我们有：

#### 命题 1 {#ens-i-a0-prop-1 .statement tag=03P6}

*如果 $A_1$、$A_2$、...、$A_p$ 是 $p$ 有意义字并且$f$ 是权 $p$ 的符号，则字 $f A_1 A_2 \ldots A_p$ 有意义。*

### 3. 刻画 / 有意义字

如果字 $A \in \mathrm{L}_0(\mathrm{S})$ 具有以下两个属性，则称其为“平衡”：

(1) $l(A) = n(A) + 1$（这意味着$A$不为空）。

(2) 对于$A$、$l(B) \leqslant n(B)$的每个真初始线段$B$。

#### 命题 2 {#ens-i-a0-prop-2 .statement tag=03P7}

*字当且仅当它是平衡时才是重要的。*

令 $A$ 成为显着字属于到显着序列

$$A_1, \; A_2, \; \ldots, \; A_n.$$

我们将通过归纳对$k$证明每个$A_k$是平衡的。假设这对于 $A_j$ 和指标 $j < k$ 成立，让我们证明它对于 $A_k$ 成立。如果 $A_k$ 是权 0 的符号（这是 $k = 1$ 时的唯一可能性），$A_k$ 是平衡的，因为

$$l(A_k) = 1 \qquad \text{and} \qquad n(A_k) = 0.$$

如果 $A_k$ 不是权 0 的符号，则 $A_k = fB_1B_2 \ldots B_p$，其中 $f$ 是权 $p$ 的符号，$B_j$ 是形式 $A_{i_j}$，其中 $i_j < k$，因此通过电感假设平衡字。我们有

$$\begin{aligned} l(A_k) &= 1 + l(B_1) + l(B_2) + \cdots + l(B_p) \\ &= 1 + (n(B_1) + 1) + (n(B_2) + 1) + \cdots + (n(B_p) + 1) \\ &= 1 + p + n(B_1) + n(B_2) + \cdots + n(B_p) \\ &= 1 + n(A_k). \end{aligned}$$

令$C$为$A$的真初线段，并令$q$为整数$m < p$的最大的，使得$B_m$是$C$的线段，因此

$$C = f B_1 B_2 \ldots B_q D,$$

其中$D$是$B_{q+1}$的真初段。然后

$$\begin{aligned} l(C) &= 1 + l(B_1) + l(B_2) + \cdots + l(B_q) + l(D) \\ &\leqslant 1 + (n(B_1) + 1) + (n(B_2) + 1) + \cdots + (n(B_q) + 1) + n(D) \\ &\leqslant p + n(B_1) + \cdots + n(B_q) + n(D) = n(C). \end{aligned}$$

因此$A_k$是平衡的。

¶ 相反，为了证明每个平衡的字都是显着的，我们需要以下两个引理 ：

#### 引理 1 {#ens-i-a0-lem-1 .statement tag=03P8}

*设 A 为平衡的字。那么对于每个整数 k 使得 $0 \leqslant k < l(A)$ 恰好存在 A 的一个平衡线段 S，它从第 $(k + 1)$ 位置开始。*

$S$的唯一性是以下注的直接的推论：如果$T$是平衡的字，则到定义没有适当的$T$的初始段被平衡。让我们证明$S$的存在性。在 $l(B) = k$ 处写下 $A = BC$。对于每个$i$使得$0 \leqslant i \leqslant q = l(C)$，令$C_i$为长度$i$的$C$的初始段。由于$B$是$A$的真初段，我们有

$$l(C_q) = l(A) - l(B) \geqslant n(A) + 1 - n(B) = n(C_q) + 1.$$

另一方面，我们有$0 = l(C_0) \leqslant n(C_0) = 0$。令$i$为整数$j < q$的最大的，使得$l(C_h) \leqslant n(C_h)$对应$0 \leqslant h \leqslant j$；那么我们就有$l(C_i)\leq n(C_i)$和$l(C_{i+1})\geq n(C_{i+1})+1$。我们证明$C_{i+1}$是平衡的：与原初段有关的条件由于$i$的定义而得到满足；另一方面，我们有

$$
n(C_{i+1})+1\leq l(C_{i+1})=l(C_i)+1\leq n(C_i)+1\leq n(C_{i+1})+1,
$$

这样引理 1 的 $l(C_{i+1})=n(C_{i+1})+1$ 和证明就完整了。

#### 引理 2 {#ens-i-a0-lem-2 .statement tag=03GT}

每个平衡的字$A$都可以放入形式

$$
A=fA_1A_2\ldots A_p,
$$

其中 $A_i$ 是平衡的，$n(f)=p$ 是平衡的。

设$f$为$A$的初始符号。由引理 1，$A$ 可以写成

$$
fA_1A_2\ldots A_p,
$$

其中$A_i$是平衡的：我们只需要定义$A_i$作为$A$的平衡段，从第$k(i)$开始，其中

$$
k(i)=2+\sum_{j<i}l(A_j).
$$

此外，我们还有

$$
1+l(A_1)+\ldots+l(A_p)=l(A)=n(A)+1
$$
$$
=n(f)+n(A_1)+\ldots+n(A_p)+1
$$
$$
=n(f)+(l(A_1)-1)+\ldots+(l(A_p)-1)+1,
$$

由此得出$n(f)=p$。

¶ 现在两个引理已经被证明了，通过$A$的长度上的归纳显然，由于引理2和命题1，每个平衡的字$A$都是显着的。

#### 推论 1 {#ens-i-a0-lem-2-cor-1 .statement tag=03GU}

让 $A$ 成为重要的字。对于每个整数$k$，使得$0\leq k<l(A)$恰好有一个从第$(k+1)$位置开始的$A$的重要部分。

#### 推论 2 {#ens-i-a0-lem-2-cor-2 .statement tag=03GV}

每个重要的字都可以用一种方式写成形式$fA_1A_2\ldots A_p$，其中$A_i$是重要的，而$n(f)=p.$*

### 4. 组合在数学理论中的应用

假设集合 S 是数学理论$\mathscr{T}$ 的符号集合。我们为每个字母$x$放置$n(\square)=0$、$n(\tau)=n(\eta)=1$、$n(\vee)=2$、$n(x)=0$；

最后，对于$\mathscr{T}$的每个特定符号$s$，$n(s)$是$s$的权，当给出$\mathscr{T}$时，这是固定的。

¶ 令 $A$ 为 $\mathscr{T}$ 中的组件。我们用删除$A$中的链接获得的$A^*$字表示，如果$A^*$[在$L_0(S)$]平衡，我们可以说$A$是*平衡的*。 $A$的*段*是由替换在$A^*$的段$S$中获得的任何集合，这些链接在$A$中连接$S$中的符号的对。

**标准 1.** *如果 $\mathscr{T}$ 中的 $A$ 为项或关系，则 $A$ 平衡。*

设$A_1$、$A_2$、$\ldots$、$A_n$为$\mathscr{T}$中的构成构造，其中出现$A$。让我们通过归纳论证，并假设我们已经证明了指标$j<i$的$A_j$是平衡的；那么我们必须证明$A_i$是平衡的。 证明与命题 2 的证明的第一个部分一样，除非 $A_i$ 是形式 $\tau_x(B)$ 以及 $B=A_j$ 和 $j<i$。在这种情况下，令 $C$ 为替换 $x$ 获得的集合，无论它出现在 $B$ 中的任何位置，由 $\square$ 获得。 字 $A^*$ 与 $\tau C^*$ 相同；现在$B^*$是平衡的，因而$C^*$是平衡的（因为$n(\square)=n(x)=0$）。因而 $A_i^*$ 是平衡的。

¶ 因而，我们获得了将 $\mathscr{T}$ 中的装配所必需的条件为项或关系。但正如我们将看到的，这个条件还不够。

¶ 设 $A$ 为 $\mathscr{T}$ 的平衡装配。如果 $A$ 以字母或 $\square$ 开头，则 $A$ 必须仅由该符号组成（命题 2，推论 2）。对于所有其他情况，我们现在将定义装配或组合*先行词*到$A$。

(1) 如果$A$以$\land$、$\vee$或特定符号开头，则$A^*$可以完全以一种方式放入形式$fB_1B_2\ldots B_p$，其中$f$是权$p\geq 1$的符号，并且$B_i$是平衡的（命题2，推论 2）。 $A$ 的段 $A_1$、$A_2$、$\ldots$、$A_p$，其中对应至段 $B_1$、$B_2$、$\ldots$、$A^*$ 的$B_p$被称为组合 *先行词*到 $A$。 Moreover, we shall say that $A$ is *perfectly balanced* if $A$ is identical with

$$
fA_1A_2\ldots A_p,
$$

在其他字中，如果$A$中没有链接将$f$连接到$B_i$之一，或连接两个不同的$B_i$。

(2) 如果 $A$ 以 $\tau$ 开头，则 $A^*$ 为形式 $\tau B$，其中 $B$ 是平衡的（命题 2，推论 2）。在这种情况下，$A$的先行汇编是组合$A_1$中的任何一个，定义如下：替换$B$中的符号$\square$，它们在$A$中通过字母$x$链接到初始$\tau$，与出现在中的其他字母不同$B$和替换将$B$的两个符号连接到$A$。 （如果我们用一个也没有出现在 $B$ 中的字母 $y$ 代替 $x$，我们得到的组件就是 $(y|x)A_1$。）此外，如果 $A$ 与 $\tau_x(A_1)$ 相同，我们可以说 $A$ 是*完美平衡的*，在其他情况下，如果没有链接将初始 $\tau$ 与 $B$ 的任何符号（$\square$ 除外）连接起来，则为字。

¶ 我们现在可以陈述以下标准：

C2。 *设$A$是$\mathscr{T}$的平衡装配。*

¶ *要使$A$成为项，满足以下条件之一是必要且充分的： (1) $A$由单个字母组成； (2) $A$以$\tau$开头，是完美平衡的，它的先行词组合是关系*（通过CF8，足以验证*一个*先行词集合是关系）； *(3) $A$ 以实质符号开始，是完全平衡的，其先行词组合是项。* ¶ *对于 $A$ 为关系，满足以下条件之一是必要且充分的： (1) $A$ 以 a 开头$\vee$或$\neg$，是完美平衡的，它的先行词组合是关系； (2) $A$以关系符号开始，是完美平衡的，它的先行词组合是项。*

判据 CF1 到 CF4 (§ 1, no. 4) 表明条件就足够了。让我们证明它们是必要的。我们已经看到（§ 1, no. 3），如果$A$是关系，那么$A$以$\vee$、$\neg$或关系符号开始。 推理在这三种情况下都是相似的。如果对于例，$A$ 以 $\vee$ 开头，则 $A$ 为形式 $\vee BC$，其中 $B$ 和 $C$ 为关系，因此 $B$ 和 $C$ 为组合 $A$ 的先行词；因此 $A$ 是完美平衡的。如果$A$是项，那么有两种情况：它由单个字母组成，或者它以实数符号或$\tau$开头。对于第二种情况，我们的论证如上。如果$A$以$\tau$开头，则构成构造的定义表明$A$是形式$\tau_x(B)$，其中$B$是关系，$x$是一个字母，这样我们就可以取$B$ 作为$A$ 的先决组装，并且 $A$ 是完美平衡的。

当我们想要测试$\mathscr{T}$中给定的组合$A$（不是单个字母的由……组成）是否为关系（或项）时，我们首先验证$A$是否平衡，并且它以$\vee$，$\neg$或关系符号（或以a开头） $\tau$ 或实质符号）。然后我们形式先行集合或组合，并验证（如果适用）$A$完美平衡。完成此操作后，我们留下了与较短的组合相关的类似问题。因此，一步一步地，我们得出组合，每个组合都由一个符号组成，其中解是直接的。

#### 注 {#ens-i-a0-n4-rem-1 .statement tag=03GW}

除了在公理方面特别薄弱的某些数学理论（cf. 习题 7）之外，我们没有型的一般过程来使我们能够测试理论$\mathscr{T}$中的给定关系$R$是否是$\mathscr{T}$中的定理。

### 习题{#ens-i-a0-exercises}

参见[习题附录 0](exercises/a0/)。

[^1]: The results established in this Appendix will not be used anywhere else in this series.
