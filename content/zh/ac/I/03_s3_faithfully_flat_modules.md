---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 3
section_title: Faithfully flat modules
lang: zh
source: ac-i-vii
book_pages: 27-36, 49-50
pdf_pages: 0047-0056, 0069-0070
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF FAITHFULLY FLAT MODULES
      page: 27
      pdf_page: 47
    - "no": 2
      title: TENSOR PRODUCTS OF FAITHFULLY FLAT MODULES
      page: 30
      pdf_page: 50
    - "no": 3
      title: CHANGE OF RING
      page: 31
      pdf_page: 51
    - "no": 4
      title: RESTRICTION OF SCALARS
      page: 31
      pdf_page: 51
    - "no": 5
      title: FAITHFULLY FLAT RINGS
      page: 32
      pdf_page: 52
    - "no": 6
      title: FAITHFULLY FLAT RINGS AND FINITENESS CONDITIONS
      page: 34
      pdf_page: 54
    - "no": 7
      title: LINEAR EQUATIONS OVER A FAITHFULLY FLAT RING
      page: 35
      pdf_page: 55
statements: 18
exercises: 10
content_sha256: 679005083ef2694ac2fa8885f035bfc89749e49899616f58b8900a88fb88657f
translated_from: content/en/ac/I/03_s3_faithfully_flat_modules.md
translation_method: google
source_content_sha256: 0a1be9878f698d84733905bb7d0c759aa5a8adfb87dd8b4532795f408851fd36
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 1bdfd04fd3b264959263490dadc61894f935f1c4880059f7c6a614a08c8b4426
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## 3. 忠实平坦模

### 1. 定义忠实平坦模

#### 命题 1 {#ac-i-s3-prop-1 .statement tag=0444}

令$E$为右$A$模。以下四个属性是等效的：

(a) 准确地说，对于左$A$模块中的序列$N' \xrightarrow{v} N \xrightarrow{w} N''$，序列是充分必要的
$$
E \otimes_A N' \xrightarrow{1 \otimes v} E \otimes_A N \xrightarrow{1 \otimes w} E \otimes_A N''
$$
准确地说。

(b) $E$ 是平坦的，对于每个左$A$-模 $N$，关系 $E \otimes_A N = 0$ 意味着 $N = 0$。

(c) $E$ 是平坦的，对于左侧 $A$ 模块中的每个同态 $v : N' \to N$，关系 $1_E \otimes v = 0$ 意味着 $v = 0$。

(d) $E$ 是平坦的，并且对于 $A$ 的每个最大左理想 $m$，$E \neq Em$。

为了简化书写，我们对每个左$A$模块$Q$使用集合$T(Q) = E \otimes_A Q$，对左$A$模块的每个同态$v$使用$T(v) = 1_E \otimes v$。

我们证明(a)、(b)和(c)的第一个等价。

我们证明(a)蕴涵(b)。如果 (a) 成立，显然 $E$ 是平坦的（§ 2, no. 3，命题 1）。另一方面，令$N$为左$A$模，使得$T(N) = 0$并考虑序列$0 \to N \to 0$； 假设 $T(N) = 0$ 表示序列 $0 \to T(N) \to 0$ 是精确的。由 (a) 序列 $0 \to N \to 0$ 是准确的，从而 $N = 0$。

我们证明（b）蕴涵（c）。假设 (b) 成立，并令 $u : N' \to N$ 为同态，且 $I$ 为像。由于$T(v)$的像等同于$T(I)$（§ 2, no. 3，注2），假设$T(v) = 0$意味着$T(I) = 0$，因此通过(b)得到$I = 0$，进而得到$v = 0$。

我们证明（c）蕴涵（a）。假设 (c) 成立并考虑序列
$$
N' \xrightarrow{v} N \xrightarrow{w} N''
$$
左侧 $A$ 模块的同态和相应的序列
$$
T(N') \xrightarrow{T(v)} T(N) \xrightarrow{T(w)} T(N'').
$$

如果序列 (1) 是精确的，则 (2) 也是精确的，因为 $E$ 是平坦的 (§ 2, no. 3, 命题 1)。 相反，如果 (2) 是精确的，我们首先有 $T(w \circ v) = T(w) \circ T(v) = 0$，因此 $w \circ v = 0$ 假设。 集合$I = v(N')$和$K = \overline{w}(0)$；则$I$由上述包含在$K$中。 考虑正合序列
$$
0 \to I \xrightarrow{i} K \xrightarrow{p} K/I \to 0
$$
$i$ 和$p$ 为典范映射。 As $E$ is flat, the sequence
$$
0 \to T(I) \xrightarrow{T(i)} T(K) \xrightarrow{T(p)} T(K/I) \to 0
$$
is exact, in other words, $T(K/I)$ is isomorphic to $T(K)/T(I)$, which is 0 by hypothesis, since $T(I)$ (resp. $T(K)$) is identified with the image of $T(v)$ (resp. the kernel of $T(w)$) (§ 2, no. 3, Remark 2). 但关系$T(p) = 0$蕴涵$p = 0$乘以假设，因此$K = I$，这证明序列（1）是精确的。

最后我们展示（b）和（d）的等价。如果 (b) 成立，则

$$
E/E_m = E \otimes_A (A_s/m) \neq 0
$$

从 $A_s/m \neq 0$ 开始； 从而 (d)。相反，假设(d)成立； $A$的每个左理想$a \neq A$都包含在最大左理想$m$中（*代数*，章I, §8, no. 7，定理2），则假设$E \neq Em$蕴涵$E \neq Ea$，换句话说字，$E \otimes_A (A_s/a) \neq 0$。也就是说，对于每个*单生*留下的$A$-模块$N \neq 0$，$T(N) \neq 0$。如果现在$N$是任何左$A$-模块\#0，它包含是单生的子模$N' \neq 0$；由于$E$是平坦的，因此$T(N')$与$T(N)$的子群进行识别；我们刚刚看到了$T(N') \neq 0$，因此是$T(N) \neq 0$。

#### 定义 1 {#ac-i-s3-def-1 .statement tag=0445}

*右$A$-模块* $E$ *如果满足命题 1 的四个等价条件，则称为忠实平坦。*

忠实地平左$A$-模块的定义类似；显然，要使左$A$模$E$忠实平坦，$E$（被视为右$A^0$模）忠实平坦是必要且充分的。

#### 注 {#ac-i-s3-n1-rem-1 .statement tag=0446}

If $E$ is a faithfully flat $A$-module, $E$ is a *faithful* $A$-module: for, if 元素 $a \in A$ is such that $xa = 0$ for all $x \in E$, 位似 $h : b \mapsto ba$ in $A$使得$1, \otimes h = 0$； 从而$h = 0$除以命题1的性质(c)，即$a = 0$，因为$A$有单位元。

*例*
(1) 平坦模和忠实平坦模的直和凭借命题 1 和 § 2, no. 3、命题 2 的性质 (d) 是忠实平坦模。
(2) *由于 $A$*，根据命题 1 和 § 2, no. 4、*例* 1 的标准 (d) 是忠实平坦的，因此从 (1) 可以得出，每个自由模 *未减少到 0* 都是忠实平坦的。另一方面，存在自由模的非零直因子（在其他字、非零投射模），它们是忠实的，但*不*忠实地平坦（习题2）。
(3) 设$A$为*主理想整环*。对于$A$-模块$E$要完全平坦，对于$A$的每个不可约元（*代数*，章VII, § 1, no. 3）$p$来说，它是*无扭转*和$E \neq Ep$是必要且充分的；这紧随§ 2, no. 4、命题 3 和命题 1 的标准 (d)。
(4) 例 (3) 表明$\mathbf{Z}$-模$\mathbf{Q}$ 是一个平坦且忠实的模，但*不忠实平坦*。

#### 命题 2 {#ac-i-s3-prop-2 .statement tag=0447}

*令 $E$ 为忠实平坦的右 $A$ 模，而 $u : N' \to N$ 为左 $A$ 模同态。对于 $u$ 是单射的（分别是满射、双射的），$1_E \otimes u : E \otimes_A N' \to E \otimes_A N$ 是这样的充分必要。*

这是命题 1 的标准(a)的直接的推论。

#### 命题 3 {#ac-i-s3-prop-3 .statement tag=0448}

令$0 \to E' \to E \to E'' \to +0$为右$A$模块的正合序列。假设 $E'$ 和 $E''$ 是平坦的，并且其中之一是忠实平坦的。那么 $E$ 就忠实地平坦了。

我们已经知道 $E$ 是平坦的（$§ 2$、no. 5、命题 5）。我们验证 $E$ 的性质 (b) 为命题 1。令 $N$ 为左 $A$ 模。因为$E''$是平坦的，所以有正合序列

$$
0 \to E' \otimes_A N \to E \otimes_A N \to E'' \otimes_A N \to 0
$$

($§ 2$, no. 5, 命题 4).如果$E \otimes_A N = 0$，则$E' \otimes_A N$和$E'' \otimes_A N$是零；由于模 $E'$ 之一，$E''$ 是忠实平坦的，这意味着 $N = 0$。

### 2. 张量积忠实平坦模

#### 命题 4 {#ac-i-s3-prop-4 .statement tag=0449}

令$R, S$为两个环，$E$为右$R$模，$F$为$(R, S)$双模。假设 $E$ 是忠实平坦的。那么，要使 $F$ 成为平坦（或忠实平坦）$S$ 模，$E \otimes_R F$ 是必要且充分的。

(1) 如果 $F$ 是平坦的，则 $E \otimes_R F$ 是平坦的（$§ 2$、no. 7、命题 8）。

(2) 假设$E \otimes_R F$是平的，并令$\nu : N' \to N$为左单射$S$模同态。 同态

$$
l_E \otimes l_F \otimes \nu : E \otimes_R F \otimes_S N' \to E \otimes_R F \otimes_S N
$$

那么是单射 ($§ 2$, no. 3, 命题 1)。从 no. 1 的命题 2 可知 $l_F \otimes \nu : F \otimes_S N' \to F \otimes_S N$ 是单射的；那么$F$是一个扁平的$S$模（$§ 2$，no. 3，命题1）。

(3) 假设$F$忠实地平坦，并令$N$为左$S$模，使得$E \otimes_R F \otimes_S N = 0$。由于 $E$ 是忠实平坦的，这意味着 $F \otimes_S N = 0$、从而 $N = 0$ 因为 $F$ 是忠实平坦的；这证明 $E \otimes_R F$ 是忠实平坦的。

(4) 假设$E \otimes_R F$忠实地平坦，并令$N$为左$S$模，使得$F \otimes_S N = 0$。然后是 $E \otimes_R F \otimes_S N = 0$、从而 $N = 0$，这表明 $F$ 是忠实平坦的。

#### 推论{#ac-i-s3-n2-cor-1 .statement tag=044A}

令$C$为交换环，并且$E$和$F$是两个忠实平坦的$C$模块。那么$C$-模块$E \otimes_C F$就忠实地平坦了。

应用命题 4 与 $R = S = C$。

### 3.变换 / 环

#### 命题 5 {#ac-i-s3-prop-5 .statement tag=044B}

设$\rho$为同态，从环$A$到环$B$。如果 $E$ 是忠实平坦的右 $A$ 模，则右 $B$ 模 $\rho^*(E) = E_{(B)} = E \otimes_A B$ 也是忠实平坦的。

应用命题 4 of no. 2 与 $R = A, S = F = B$，注意到 $B$ 模块 $B_d$ 是忠实平坦的。

#### 推论{#ac-i-s3-n3-cor-1 .statement tag=044C}

*如果$E$是忠实平坦的右$A$模，并且如果$a$是$A$的双面理想，则右$(A/a)$模$E/Ea$是忠实平坦的。*

应用命题 5，$B = A/a, \rho$ 为典范同态。

#### 命题 6 {#ac-i-s3-prop-6 .statement tag=044D}

令$A$为交换环，$B$代数超过$A$，以及$A$到$B$的$\rho : a \mapsto a . 1$典范同态。假设 $B$ 是一个忠实的扁平 $A$ 模块。那么，为了使$A$-模$E$是平坦的（或忠实平坦），右$B$-模$E_{(B)} = E \otimes_A B$是平坦的（或忠实平坦）是必要且充分的。

(1) 如果 $E$ 平坦（或忠实平坦），则 $E_{(B)}$ 平坦（或忠实平坦）§ 2, no. 7，推论 2 至命题 8（或命题 5）。

(2) 假设$E_{(B)}$是平的，并令$\nu : N' \to N$是单射$A$-模同态。根据§ 2, no. 7，推论 3，$A$-模 $E \otimes_A B$ 是平坦的，因此同态 $1, \otimes 1_B \otimes \nu : E \otimes_A B \otimes_A N' \to E \otimes_A B \otimes_A N$ 是单射的。作为$B$重合上的左右$A$模块结构，这个同态被标识为

$$
1_E \otimes \nu \otimes 1_B : E \otimes_A N' \otimes_A B \to E \otimes_A N \otimes_A B.
$$

由于$B$是忠实平坦的$A$模，因此$1_E \otimes \nu : E \otimes_A N' \to E \otimes_A N$是单射的（no. 1，命题2），这表明$E$是平坦的。

(3) 最后假设 $E_{(B)}$ 是忠实平坦的。首先，$E$ 被 (2) 压扁。还令 $N$ 为 $A$ 模，使得 $E \otimes_A N = 0$。然后是$E \otimes_A N \otimes_A B = 0$、从而，因为$B$、重合、$E \otimes_A B \otimes_A N = 0$上的左右$A$模结构，也可以写成$(E \otimes_A B) \otimes_B (B \otimes_A N) = 0$。由于$E_{(B)}$是一个忠实平坦的$B$模块，这意味着$B \otimes_A N = 0$（no. 1，命题1），从而$N = 0$，因为$B$是一个忠实平坦的$A$模块（no. 1， 命题 1)。

### 4. 限制标量

#### 命题 7 {#ac-i-s3-prop-7 .statement tag=044E}

*令$A, B$为$A$至$B$中的两个环和$\rho$同态。令 $E$ 成为忠实的扁平右$B$模。为了使 $\rho^*(E)$ 成为平坦（或忠实平坦）右 $A$ 模，$B$ 成为平坦（或忠实平坦）右 $A$ 模是必要且充分的。*

no. 2的应用命题4个分别用$B, A, E, B$代替$R, S, E, F$，$B$上的右侧$A$模块结构由$\rho$定义，可见

B 是平坦的（或忠实平坦的）A-模当且仅当 $E \otimes_B B = \rho^*(E)$ 是平坦的（或忠实平坦的）A-模。

注
(1) 命题 7 表明，要使 B 成为忠实平坦 A-模，只要存在一个忠实平坦 B-模且它也是忠实平坦 A-模就足够了。
(2) 令A、B、C为三个环和$\rho : A \to B, \sigma : B \to C$两个环同态。 命题 7 表明，如果 C 是忠实平坦 B-模并且 B 是忠实平坦 A-模，则 C 是忠实平坦 A-模。如果 C 是忠实平坦的 B-模和忠实平坦的 A-模，则 B 是忠实平坦的 A-模（将模视为正确的模，以修正想法）。另一方面，B 和 C 可能是忠实平坦的 A-模，而 C 不是忠实平坦的 B-模 (习题 7)。

### 5. 忠实平坦环

#### 命题 8 {#ac-i-s3-prop-8 .statement tag=044F}

设A、B是从A到B的两个环和$\rho$同态。假设存在右B-模E，使得$\rho_*(E)$是忠实平坦的A-模。然后：
(i) 对于每个左A-模 F，典范同态 $j : F \to F_{(B)} = B \otimes_A F$（使得 $j(x) = 1 \otimes x$ 对于所有 $x \in F$）是单射的。
(ii) 对于 A 的每个左理想 a，$\overline{\rho}^{-1}(Ba) = a$。
(iii) 同态 $\rho$ 是单射的。
(iv) 对于 A 的每个最大左理想 m，都存在 B 的最大左理想 n，使得 $\overline{\rho}^{-1}(n) = m$。

我们证明（i）。我们知道（代数，章 11，§ 5, no. 2，命题 5 的推论），对于每个右B-模 M，由 $i(y) = y \otimes 1$ 定义的规范 A-同态 $i : M \to \rho_*(M) \otimes_A B = \rho^*(\rho_*(M))$ 是单射的，并且 A-模 $i(M)$ 是 $\rho_*(M) \otimes_A B$ 中的直因子。因此，对于每左A-模 F，

$$
i \otimes 1_F : \rho_*(M) \otimes_A F \to \rho_*(M) \otimes_A B \otimes_A F
$$

是单射 (§ 2, no. 1, 引理 2)。取$M = E$，可以得出（自$i \otimes 1_F = 1_M \otimes j$）$j$是单射的（no. 1，命题2）。

断言 (ii) 由 (i) 取 $F = A_s/a$ 得出，(iii) 由 (ii) 取 $a = \{0\}$ 得出。

最后，如果 m 是 A 的最大左理想，则$\overline{\rho}^{-1}(Bm) = m$乘以(ii)，因而$Bm \# B$。则存在 B 包含 Bm (代数, 章 I, § 8, no. 7, 定理 2) 的最大左理想 n；然后$m \subset \overline{\rho}^{-1}(n)$和$\rho(1) \notin n$，$1 \notin \overline{\rho}^{-1}(n)$。因而$\overline{\rho}^{-1}(n) = m$。

如果命题 8 中的$A$ 和$B$ 满足条件，$A$ 通常通过$\rho$ 与$B$ 中的子环进行识别。

#### 推论{#ac-i-s3-n5-cor-1 .statement tag=044G}

在命题 8 的假设下，如果$B$ 是左诺特的（或阿廷的），那么$A$ 也是。

如果 (a) 是$A$左理想的非平稳递增（或递减）序列，$B$理想的序列$(\mathrm{Ba}_n)$是非平稳的，并且递增（或递减）因为$\rho^{-1}(\mathrm{Ba}_n) = a_n$与假设相反。

*注（1）。如果$A$和$B$是可交换的，我们将在章II, § 2, no. 5推论4到命题11中看到，命题8的假设意味着对于$A$的每个素理想$p$，存在$B$的素理想$q$使得$\rho^{-1}(q) = p$（其中当$A$与$B$的子环相同时，$p = A \cap q$）。*

命题 8 的一个重要应用是当 $B$ 本身是一个忠实的扁平 $A$ 模时。但在这种情况下，我们有以下更精确的命题：

#### 命题 9 {#ac-i-s3-prop-9 .statement tag=044H}

令$A, B$为$A$至$B$中的两个环和$\rho$同态。以下五个属性是等效的：
(a) 右侧$A$-模块$B$ 是忠实平坦的。
(b) 同态 $\rho$ 是单射的，右$A$-模 $B/\rho(A)$ 是平的。
(c) 右$A$-模$B$是平坦的，并且对于每个左$A$-模$F$，$F$到$B @ * F$的典范同态$x \mapsto 1 @ x$是单射的。
(d) 右$A$模$B$是平坦的，对于$A$的每个左理想$a$，$\rho^{-1}(\mathrm{Ba}) = a$。
(e) 右$A$-模$B$是平坦的，并且对于$A$的每个最大左理想$m$，存在$B$的最大左理想$n$，使得$\rho^{-1}(n) = m$。

通过命题 8，(a) 隐含了属性 (c)、(d)、(e) 中的每一个。另一方面，如果 (e) 成立，则 $Bm \# B$ 对于 $A$ 的每个最大左理想 $m$（因为存在 $B$ 的最大左理想 $n$，使得 $Bm \subset n$），并且根据标准，$B$ 是忠实平坦的 $A$ 模(d) 命题 1 no. 1；因此(e)意味着(a)。

我们现在要证明 (c) $\Rightarrow$ (d) $\Rightarrow$ (b) $\Rightarrow$ (a)，这将完成证明。首先，(c)通过在(c)中取$F = A_s/a$来暗示(d)。如果 (d) 成立，通过取 $a = \{0\}$ 可以得出 $\rho$ 是单射的； (d) 和 § 2, no. 6，命题 7 的推论意味着 $B/\rho(A)$ 是平右 $A$ 模，即 (d) 隐含 (b)。最后，如果 (b) 成立，则 no. 1 的命题 3 应用于正合序列

$$
0 \longrightarrow A_a \xrightarrow{\rho} B \longrightarrow B/\rho(A) \longrightarrow 0
$$

表明 $B$ 是忠实平坦的右 $A$ 模，因为 $A_a$ 是忠实平坦的。

*注（2）。如果$A$和$B$是可交换的，我们将在章II, § 2 no. 5推论4到命题11中看到，命题9的条件等价于：

(f) B *是一个平坦的A-模，并且对于每个素理想*$\mathfrak{p}$*的*$A$，*都存在一个理想*$q$*的*$B$*使得*$\bar{\rho}^{-1}(q) = \mathfrak{p}$。

在命题 9 的条件下，让我们通过 $\mathfrak{p}$ 来计算认同 $A$，*子环* 为 $B$。 关系 $\bar{\rho}^{-1}(Ba) = a$ 然后读取$A \cap Ba = a$。另一方面，如果$F$是左$A$模块，$F$将被识别为典范映射$x \mapsto 1 @ x$下$B \otimes_A F$中的像；如果$X$是$F$的加法子群，那么我们用$BX$表示由$X$生成的$B \otimes_A F$的左子B-模块。有了这个记号，我们有：

#### 命题 10 {#ac-i-s3-prop-10 .statement tag=044I}

*令*$B$*成为环和*$A$*子环*$B$*这样*$B$*是一个忠实的平右*$A$-*模。令*$F$*成为*$A$-*模、$F', F''$*两个子模*$F$。 *然后：*
(i) *典范映射* $B \otimes_A F' \to B \otimes_A F$ *是* $B \otimes_A F'$ *的同构 *到* $BF'$。
(ii) $F \cap BF' = F'$。
（三）$B(F' + F'') = BF' + BF''$。
（四）$B(F' \cap F'') = BF' \cap BF''$。

由于$B$是平右$A$模，典范映射
$$
B \otimes_A F' \to B \otimes_A F
$$
是单射的；考虑到所做的识别，其像为$BF'$，这证明了(i)。 断言 (ii) 源自§ 2, no. 6、命题 7，应用的$E = B$、$E' = A$，并使用公式、$A \otimes_A F = F$ 和$A \otimes_A F' = F'$。 断言 (iii) 是微不足道的，(iv) 由§ 2, no. 6、命题 6 得出。

### 6. 忠实平坦环和有限性条件

#### 命题 11 {#ac-i-s3-prop-11 .statement tag=044J}

*设*$B$*为环且*$A$*子环为*$B$*使得*$B$*是一个忠实的平右*$A$-*模。对于左* $A$-*模* $F$ *确定生成（或有限呈现），* $B$-*模* $B \otimes_A F$ *有限生成（或有限呈现）是必要且充分的。*

(1) $B$上没有任何假设，显然，如果$F$是有限生成的左$A$模，$B \otimes_A F$是有限生成的左$B$模。相反，如果$B \otimes_A F$是有限生成的$B$模，则它是由形式$1 \otimes x_i$和$x_i \in F$的元素的有限数生成；如果$M$是$x_i$和$j$典范嵌入$M \to F$生成$F$的子A模，$1, \otimes j : B \otimes_A M \to B \otimes_A F$是满同态，因而$j$是满射（no. 1， 命题 2)，证明$F$是有限生成的。

(2) *如果* $F$ *承认有限表示，那么* $B \otimes_A F$ *在 B (§ 2, no. 8) 上没有任何假设*。仍有待证明的是，如果$B \otimes_A F$承认有限表示，F也承认有限表示。从（1）我们已经知道F是有限生成的，因此存在满同态$u : L \to F$，其中L是有限生成的自由A-模。设R为u的核，则$B \otimes_A R$可与满同态$l_B \otimes u : B \otimes_A L \to B \otimes_A F$的核识别（§ 2, no. 3，*注2*）。由于 $B \otimes_A F$ 承认假设的有限表示，我们结论 (§ 2, no. 8, 引理 9) $B \otimes_A R$ 是有限生成的；那么从 (1) 可以得出，R 是有限生成A-模，因而 F 承认有限表示。

#### 命题 12 {#ac-i-s3-prop-12 .statement tag=044K}

*设 B 为环，A 为 B 的中心的交换律子环，使得 B 是忠实平坦的 A-模。对于 A-模 F 是射影且有限生成的，$B \otimes_A F$ 是有限生成的射影左B-模是充分必要的。*

在 A 或 B 上没有任何假设时，条件显然是必要的（*代数*、章 II, § 5, no. 1，命题 4 的推论）；我们证明这是足够的。如果有限生成射影模承认有限表示（§ 2, no. 8，引理8），假设意味着F凭借命题11承认有限表示，因而，对于每个A-模M，有典范同构

$$
\omega : B \otimes_A \operatorname{Hom}_A(F, M) \to \operatorname{Hom}_B(B \otimes_A F, B \otimes_A M)
$$

（§ 2, no. 10，命题11）。然后令 $v : M \to M''$ 为*满射* A-模同态并考虑交换律图表

$$
\begin{array}{ccc}
B \otimes_A \operatorname{Hom}_A(F, M) & \xrightarrow{\omega} & \operatorname{Hom}_B(B \otimes_A F, B \otimes_A M) \\
1_B \otimes \operatorname{Hom}(1_F, v) \downarrow & & \downarrow \operatorname{Hom}(1_B \otimes F, 1_B \otimes v) \\
B \otimes_A \operatorname{Hom}_A(F, M'') & \xrightarrow{\omega} & \operatorname{Hom}_B(B \otimes_A F, B \otimes_A M'')
\end{array}
$$

由于 $1_B \otimes v$ 是满射且 $B \otimes_A F$ 假定为射影，因而 $\operatorname{Hom}(1_{B \otimes F}, 1_B \otimes v)$ 是*满射* (*代数*, 章 II, § 2, no. 2, 命题 4)，因而 $1_B \otimes \operatorname{Hom}(1_F, v)$ 也是如此。但由于 B 是忠实平坦的 A-模，$\operatorname{Hom}(1_F, v)$ 本身是满射 (no. 1, 命题 2)，因而 F 是射影 A-模 (*代数*, 章 II, § 2, no. 2, 命题 4).

### 7. 忠实平面环上的线性方程

设 B 为 B 的环，A 为 B 的子环。如果满足以下条件，我们可以说有序对 (A, B) 具有*线性扩张性质*：

(E) 线性方程组$B$、系统、元素、解、$(y_k)_{1 \leq k \leq n}$、由……组成

$$
\sum_{k=1}^n y_k c_{ki} = d_i \quad (1 \leq i \leq m)
$$

其系数$c_{ki}$和右侧$d_i$属于到$A$，为形式

$$
y_k = x_k + \sum_{j=1}^p b_j z_{jk} \quad (1 \leq k \leq n)
$$

其中$(x_k)$是$A$的元素的由……组成的解，$b_j$属于到$B$以及每个$(z_{jk})_{1 \leq k \leq n}$是齐次线性的解系统与(3)相关，$A$的元素的由……组成。

#### 命题 13 {#ac-i-s3-prop-13 .statement tag=044L}

令$A$为环$B$中的子环。对于有序对$(A, B)$到满足线性扩张性质，$B$是忠实平坦的$A$模是必要且充分的。

条件*足够*。因为，由于 $B$ 是一个平面 $A$ 模，因此与 (3) 相关的*齐次*线性系统的 $B$ 中的解和元素是线性组合，其中 $B$ 中的系数为解由……组成 / 元素 / $A$（§ 2, no. 11，推论 2，至命题 13）。 问题则约化到证明，(3)的解与$B$中的元素的存在意味着$A$中存在*一*解与元素。现在如果我们集合

$$
c_k = (c_{ki})_{1 \leq i \leq m} \in A_s^m, \qquad d = (d_i) \in A_s^m,
$$

系统 (3) 等价于方程$\sum_{k=1}^n y_k \otimes c_k = 1 \otimes \mathrm{din}\, B \otimes_A A_s^m = B_s^m$。

在其他字中，如果$M$是$c_k$$(1 \leq k \leq n)$生成的$A_s^m$的子$A$模块，则（3）中解$(y_k)$的存在性与关系等价（与no. 5中所做的标识） $d \in BM \cap A_s^m$;但作为$BM \cap A_s^m = M$ (no. 5, 命题 10, (ii))，则隐含$d \in M$，即系统(3)中存在解$(x_k)$，$A$中存在元素。

条件是*必要的*。假设$(A, B)$满足线性扩张性质；我们已经知道$B$是平右$A$模（§ 2, no. 11，推论2到命题13）；我们证明，对于$A$、$Ba \cap A = a$的每个左理想$a$，这表明$B$是一个忠实的平右$A$模（no. 5，命题 9，（d））。现在，令 $x \in Ba \cap A$；存在假设$y_i \in B$和$a_i \in a$使得$\sum_i y_i a_i = x$； 性质 (E) 应用于这个带有系数的线性方程以及$A$的右侧表明存在$x_i \in A$使得$x = \sum_i x_i a_i$，因此$x \in a$。

### 习题 {#ac-i-s3-exercises}

§ 3](exercises/s3/)参见[习题。
