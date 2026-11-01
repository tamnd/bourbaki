---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VI
chapter_title: ROOT SYSTEMS
section: 1
section_title: Root systems
lang: zh
source: lie-iv-vi
pdf_pages: 0168-0198, 0248-0253
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A ROOT SYSTEM
      page: 0
      pdf_page: 168
    - "no": 2
      title: DIRECT SUM OF ROOT SYSTEMS
      page: 0
      pdf_page: 172
    - "no": 3
      title: RELATION BETWEEN TWO ROOTS
      page: 0
      pdf_page: 173
    - "no": 4
      title: REDUCED ROOT SYSTEMS
      page: 0
      pdf_page: 177
    - "no": 5
      title: CHAMBERS AND BASES OF ROOT SYSTEMS
      page: 0
      pdf_page: 178
    - "no": 6
      title: POSITIVE ROOTS
      page: 0
      pdf_page: 181
    - "no": 7
      title: CLOSED SETS OF ROOTS
      page: 0
      pdf_page: 186
    - "no": 8
      title: HIGHEST ROOT
      page: 0
      pdf_page: 191
    - "no": 9
      title: WEIGHTS, RADICAL WEIGHTS
      page: 0
      pdf_page: 192
    - "no": 10
      title: FUNDAMENTAL WEIGHTS, DOMINANT WEIGHTS
      page: 0
      pdf_page: 193
    - "no": 11
      title: COXETER TRANSFORMATION
      page: 0
      pdf_page: 195
    - "no": 12
      title: CANONICAL BILINEAR FORM
      page: 0
      pdf_page: 197
statements: 79
exercises: 24
content_sha256: 61570f26e83b41416af2e83c7f3695da35915181634184381487da79fe535ddf
translated_from: content/en/lie/VI/01_s1_root_systems.md
translation_method: google
source_content_sha256: e928a5393f8d44d4601610a514808a5db0798a4a4348f1d6a9e230dc8b3576c6
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 5bfdd4500e6d64db80b5c32d4f734cdedc9517c00875670fa6880fa5d8a98dd4
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 1。 根系

在本段中，$k$表示特征零中的域。从no. 3开始，我们假设$k = \mathbf{R}$。

### 1. 定义根系

#### 引理 1 {#lie-vi-s1-lem-1 .statement tag=0AU4}

令 $V$ 为向量空间超过 $k$，$R$ 有限子集 $V$ 生成的 $V$。对于任何$\alpha \in R$使得$\alpha \neq 0$，最多存在一个$V$的反射$s$使得$s(\alpha) = -\alpha$和$s(R) = R$。

令$G$为$V$的自同构中的群，使$R$保持稳定。由于$R$生成$V$，$G$同构于$R$的对称群的子群，因此是有限的。令 $s, s'$ 为 $V$ 的反射，使得 $s(\alpha) = s'(\alpha) = -\alpha$、$s(R) = R$、$s'(R) = R$。然后$t = ss'$属于到$G$，因此是有限的阶$m$。另一方面，

$$
t(\alpha) = \alpha \quad \text{and} \quad t(x) \equiv x \mod. k\alpha \quad \text{for all } x \in V.
$$

因此，在$V$上存在线性形式$f$使得

$$
t(x) = x + f(x)\alpha \quad \text{for all } x \in V
$$

和$f(\alpha) = 0$。到 $n$ 归纳时，得出如下结论：

$$
t^n(x) = x + nf(x)\alpha \text{ for all } x \in V.
$$

令$n$等于$m$，我们发现$mf(x) = 0$适用于所有$x \in V$，因此$f = 0$、$t = 1$和$s = s'$。

#### 定义 1 {#lie-vi-s1-def-1 .statement tag=0AU5}

令 $V$ 为向量空间大于 $k$，且 $R$ 子集为 $V$。那么，如果满足以下条件，则称$R$为$V$中的根系：

(RS_I) $R$ 是有限的，包含不为 0，且生成 $V$。
(RS_{II}) 对于所有$\alpha \in R$，存在$V$的对偶$V^*$的元素$\alpha^\vee$，使得$\langle \alpha, \alpha^\vee \rangle = 2$和反射$s_{\alpha, \alpha^\vee}$（cf.章节V, § 2）离开$R$稳定。

(RS_{\text{III}}) 对于所有$\alpha \in \mathbf{R}$，$\alpha^{\sim}(R) \subseteq \mathbf{Z}$。

通过引理 1，反射$s_{\alpha,\alpha^{\sim}}$（因此也线性形式$\alpha^{\sim}$）由$\alpha$唯一确定，因此(RS_{\text{III}})是有意义的。我们放$s_{\alpha,\alpha^{\sim}} = s_{\alpha}$。然后对所有 $x \in V$ 进行 $s_{\alpha}(x) = x - \langle \alpha^{\sim}, x \rangle \alpha$。

R 的元素称为根（考虑到系统）。 V的维数称为系统的秩。

使 R 保持稳定的 V 的自同构称为 R 的自同构。它们形式有限群用 A(R) 表示。由$s_{\alpha}$生成的A(R)的子群称为R的Weyl群，记为W(R)，或简称为W。

#### 注 1 {#lie-vi-s1-n1-rem-1 .statement tag=0AU6}

令 $k'$ 为 $k$ 的扩张。 认同 V 与$V \otimes k'$ 的子集和$V^*$ 与子集 $V^* \otimes k' = (V \otimes k')^*$ 规范化。那么，$V \otimes k'$中的R为根系，$\alpha^{\sim}$与之前相同。

#### 引理 2 {#lie-vi-s1-lem-2 .statement tag=0AU7}

令 R 为 V 中的根系。令$(x|y)$是V上的对称双线性形式，在W(R)下非简并且不变。 认同V和$V^*$通过这个形式。如果 $\alpha \in R$，则 $\alpha$ 是非各向同性的，并且

$$
\alpha^{\sim} = \frac{2\alpha}{(\alpha|\alpha)}.
$$

这是从第 7 章公式 (4) 得出的。 V, § 2, no. 3。

#### 命题 1 {#lie-vi-s1-prop-1 .statement tag=0AU8}

令$V_Q$（或$V_Q^*$）为由$\alpha$（或$\alpha^{\sim}$）生成的V（或$V^*$）的Q向量子空间。那么$V_Q$（分别$V_Q^*$）是V（分别$V^*$）上的Q结构（代数，第II, § 8, no. 1章）。 $V \times V^*$上的规范双线性形式的限制到$V_Q \times V_Q^*$给出了空间$V_Q, V_Q^*$中的每一个与另一个的对偶的标识。 集合 R 是 $V_Q$ 中的根系。

如果 $k = \mathbf{R}$，则在 W(R) 下的 V 不变量上存在标量乘积（积分，VII, § 3, no. 1，命题 1）； 引理 2 现在显示$\alpha^{\sim}$ 生成 $V^*$。到注 1 时，$\alpha^{\sim}$ 再次生成 $V^*$（如果$k = \mathbf{Q}$）。我们现在讨论一般情况。让 E = $V_Q$。通过 (RS_{\text{III}})，每个 $\alpha^{\sim}$ 映射 E 到 $\mathbf{Q}$，等等定义元素 $\tilde{\alpha}$ $E^*$。 E中R为根系为直接的，$E^*$中元素相应的至$\alpha$为$\tilde{\alpha}$。按照我们上面所说的，$\tilde{\alpha}$生成向量空间$E^*$。考虑典范同态$i : E \otimes_Q k \to V$，以及它的转置$^t i : V^* \to E^* \otimes_Q k$。由于 R 生成 V，$^t i$ 是单射的；但是 $^t i$ 包含的像是 $\tilde{\alpha}$，所以 $^t i$ 是满射。由此我们结论最终i和$^t i$是同构。因此，我们可以将认同V与$E \otimes k$，$V^*$与$E^* \otimes k$，$\alpha^{\sim}$与$\tilde{\alpha}$，以及$V_Q^*$与$E^*$。因此，$V_Q$（分别$V_Q^*$）是V（分别$V^*$）上的Q结构。 $V \times V^*$上的规范双线性形式的限制到$V_Q \times V_Q^*$可以与$E \times E^*$上的规范双线性形式识别，因此是命题。

#### 注 2 {#lie-vi-s1-n1-rem-2 .statement tag=0AU9}

命题 1 约化根系对案例$k = \mathbf{Q}$的研究。 注 1 约化进一步研究真实向量空间 $V_{\mathbf{R}} = V_{\mathbf{Q}} \otimes_{\mathbf{Q}} \mathbf{R}$中的根系。与这些不同的系统相关的 Weyl 群已被规范地识别。

#### 注 3 {#lie-vi-s1-n1-rem-3 .statement tag=0AUA}

由于$\alpha \tilde{}$生成$V^*$，群$W(R)$（被视为$\mathbf{GL}(V_{\mathbf{R}})$的子群）是必不可少的（第V, § 3, no. 7章）。此外，科。的 Th。第 1 章V, § 3, no. 2 显示属于到$W(R)$ 的唯一反射是$s_{\alpha}$。

#### 命题 2 {#lie-vi-s1-prop-2 .statement tag=0AUB}

*$V^*$中的$\alpha \tilde{}$形式根系，以及所有$\alpha \in R$中的$\alpha \tilde{} = \alpha$。*

提案 1 的 $\alpha \tilde{}$ 满足 (RS_I)。由于 $s_{\alpha, \alpha \tilde{}}$ 是向量空间 $V$ 的自同构，配备子集 $R$，${}^t(s_{\alpha, \alpha \tilde{}})^{-1}$ 离开集合 $R \tilde{}$ $\alpha \tilde{}$稳定；但是${}^t(s_{\alpha, \alpha \tilde{}})^{-1} = s_{\alpha \tilde{}, \alpha}$，证明$R \tilde{}$满足(RS_{II})和$\alpha \tilde{} = \alpha$。最后，$\langle \alpha \tilde{}, \beta \rangle \in \mathbf{Z}$对于所有$\alpha \tilde{} \in R \tilde{}$和$\beta \in R$，因此$R \tilde{}$满足(RS_{III})。

集合 $R \tilde{}$ 被称为*$R$的*逆根系。 映射 $\alpha \mapsto \alpha \tilde{}$ 是从 $R$ 到 $R \tilde{}$ 的双射，称为*规范双射从* $R$ *到* $R \tilde{}$。 注，如果$\alpha, \beta$是$R$的元素使得$\alpha + \beta \in R$，那么一般来说$(\alpha + \beta) \tilde{} \neq \alpha \tilde{} + \beta \tilde{}$。

由于$s_{\alpha}(\alpha) = -\alpha$，公理(RS_{II})表明$-R = R$。显然是$(-\alpha) \tilde{} = -\alpha \tilde{}$和$-1 \in A(R)$（但$-1 \in W(R)$并不总是正确）。

等式 ${}^t(s_{\alpha, \alpha \tilde{}})^{-1} = s_{\alpha \tilde{}, \alpha}$ 显示从群 $W(R)$ 到群 $W(R \tilde{})$，映射 $u \mapsto {}^t u^{-1}$ 为同构。我们通过这个同构来认同这两个群；在其他字中，我们认为$W(R)$同时在$V$和$V^*$中起作用。对于 $A(R)$ 也是如此。

#### 命题 3 {#lie-vi-s1-prop-3 .statement tag=0AUC}

*对于$x, y \in V$，输入*
$$
(x|y) = \sum_{\alpha \in R} \langle \alpha \tilde{}, x \rangle \langle \alpha \tilde{}, y \rangle.
$$
*那么*$(x|y)$*是*$V$上的非简并对称双线性形式，*在*$A(R)$下不变。 *对于* $x, y \in V_{\mathbf{Q}}$ *我们有* $(x|y) \in \mathbf{Q}$。 *规范扩张* $(x|y)$ *至*
$$
V_{\mathbf{R}} = V_{\mathbf{Q}} \otimes_{\mathbf{Q}} \mathbf{R}
$$
*是非简并且积极的*。

显然$(x|y)$是$V$上的对称双线性形式。如果$g \in A(R)$，
$$
(g(x)|g(y)) = \sum_{\alpha \in R} \langle {}^t g(\alpha \tilde{}), x \rangle \langle {}^t g(\alpha \tilde{}), y \rangle = (x|y)
$$
从${}^t g)(R \tilde{}) = R \tilde{}$开始。如果$x, y \in V_{\mathbf{Q}}$，则$(x|y) \in \mathbf{Q}$乘以(RS_{III})。根据命题 1，如果$z \in V_{\mathbf{R}}$，则$(z|z) = \sum_{\alpha \in R} \langle \alpha \tilde{}, z \rangle^2 \geq 0$，如果$z \neq 0$则$(z|z) > 0$，因此$(x|y)$到$V_{\mathbf{R}}$的规范扩张是正的且非简并的。因此，$(x|y)$到$V_{\mathbf{Q}}$的限制是非简并的，因此$V$上的形式$(x|y)$是非简并的。

#### 命题 4 {#lie-vi-s1-prop-4 .statement tag=0AUD}

(i) *令$X$为$\mathbf{R}$中的子集，令$V_X$为由$X$生成的$V$中的向量子空间，并令$V'_X$为向量子空间 $V^*$由$\alpha^-$生成，其中$\alpha \in X$。那么$V$就是$V_X$的直和和$V'_X$的正交补集； $V^*$是$V'_X$的直和和$V_X$的正交补集，$V'_X$与$V_X$的对偶一致。

(ii) $R \cap V_X$是$V_X$中的根系，并且从$R \cap V_X$到其逆根系的规范双射被识别为映射$\alpha \mapsto \alpha^-$到$R \cap V_X$的限制。

通过*注2*，我们可以假设$k = \mathbf{R}$。 认同 $V$ 和 $V^*$ 通过命题 3 的对称双线性形式得到。对于所有 $\alpha \in R$ (引理 2)，我们有 $\alpha^- = \frac{2\alpha}{(\alpha|\alpha)}$。 $V$ 的每个向量子空间都是非各向同性的，命题现在是清晰的。

#### 推论{#lie-vi-s1-n1-cor-1 .statement tag=0AUE}

*设$V_1$为$V$的向量子空间，并令$V_2$为由$R \cap V_1$生成的向量子空间。那么$R \cap V_1$就是$V_2$中的根系。

这是从适用于 $X = R \cap V_1$ 的 (ii) 得出的。

对于$\alpha, \beta \in R$，输入
$$
\langle \alpha, \beta^- \rangle = n(\alpha, \beta).
$$
(1)

然后
$$
n(\alpha, \alpha) = 2
$$
(2)
$$
n(-\alpha, \beta) = n(\alpha, -\beta) = -n(\alpha, \beta).
$$
(3)

通过（RSIII），
$$
n(\alpha, \beta) \in \mathbf{Z}.
$$
(4)

截至 $n(\alpha, \beta)$ 的定义，
$$
s_\beta(\alpha) = \alpha - n(\alpha, \beta)\beta.
$$
(5)

公式 (1) 和命题 2 意味着
$$
n(\alpha, \beta) = n(\beta^-, \alpha^-).
$$
(6)

令$(x|y)$是$V$上的对称双线性形式，在$W(R)$（命题3）下非简并且不变。 引理2 时，
$$
n(\alpha, \beta) = \frac{2(\alpha|\beta)}{(\beta|\beta)}.
$$
(7)

由此可见
$$
n(\alpha, \beta) = 0 \iff n(\beta, \alpha) = 0 \iff (\alpha|\beta) = 0 \iff s_\alpha \text{ and } s_\beta \text{ commute.}
$$
(8)

如果$(\alpha|\beta) \neq 0$，那么
$$
\frac{n(\beta, \alpha)}{n(\alpha, \beta)} = \frac{(\beta|\beta)}{(\alpha|\alpha)}.
$$
(9)

### 2. 直和根系

令V比$k$除向量空间，即向量空间的家庭$(V_i)_{1 \leq i \leq r}$的直和。 认同 $V^*$ 与 $V_i^*$ 的直和。对于所有$i$，令$V_i$中的$R_i$为根系。那么$R = \bigcup_i R_i$是V中的根系，其中逆系是$R^- = \bigcup_i R_i^-$；规范的双射从R到$R^-$扩展，对于所有$i$，规范的双射从$R_i$到$R_i^-$。 集合 R 称为根系* $R_i$ 的 *直和。让$\alpha \in R_i$。若$j \neq i$、$\alpha^-$包含$V_j$核，那么$s_\alpha$诱导$V_j$上的恒等式；另一方面，$k\alpha \subseteq V_i$，所以$s_\alpha$使得$V_i$保持稳定。这些注表明$W(R)$*可以与*$\prod_{i=1}^r W(R_i)$识别。

如果 $R \neq \varnothing$ 并且 R 不是两个非空根系的直和，则根系 R 被称为“不可约”。

#### 命题 5 {#lie-vi-s1-prop-5 .statement tag=0AUF}

*设 V 为向量空间超过 k，即向量空间* $V_1, \ldots, V_r$ 的直和。 *令 R 为 V 中的根系。把*$R_i = R \cap V_i$。 *以下三个条件是等效的*：

(i) **$V_i$ *在*$W(R)$下稳定；
(ii) $R \subseteq V_1 \cup V_2 \cup \cdots \cup V_r$；
(iii) *对于所有* $i$、$R_i$ *是* $V_i$ 中的根系，*且 R 是* $R_i$ 中的直和。
(iii) $\Longrightarrow$ (i)：这源自我们在数开头所说的内容。

(i) $\Longrightarrow$ (ii)：假设 $V_i$ 在 $W(R)$ 下稳定。设 $\alpha \in R$ 且 H 为 $\alpha^-$ 的核。根据第 3 章的提案。 V, § 2, no. 2，每个$V_i$是H的子空间的和和$k\alpha$的子空间。因此，$V_i$包含$k\alpha$之一，所以$\alpha \in V_1 \cup V_2 \cup \cdots \cup V_r$。

(ii) $\Longrightarrow$ (iii)：如果满足条件 (ii)，则对于所有$i$，$R_i$ 生成 $V_i$，因此$R_i$在$V_i$中是根系（命题4）。显然，R 是$R_i$ 中的直和。

#### 推论{#lie-vi-s1-n2-cor-1 .statement tag=0AUG}

*令 R 为 V 中的根系。以下条件是等效的*：
(i) *R 是不可约的*；
(ii) ** $W(R)$*-模块* V *很简单*；
(iii) **$W(R)$*-模块*V*绝对简单*。
(ii) $\Longleftrightarrow$ (i)：这源自第 5 条提案和 Maschke 的定理（第 V、附录、第 2 条提案）。
(iii) $\Longleftrightarrow$ (ii)：这源自第 1 章的提案 1。 V, § 2, no. 1。

#### 命题 6 {#lie-vi-s1-prop-6 .statement tag=0AUH}

*每个根系* R *in* V *是一个家族的直和* $(R_i)_{i \in I}$ *不可约的根系，在指标集合* 的双射范围内是唯一的。

$R_i$的存在性由卡R上的归纳证明：如果R非空且不可约，则R是两个根系$R', R''$的直和，使得卡$R' <$卡$R$，卡$R'' <$卡$R$，并且归纳假设适用于$R'$ 和$R''$。为了证明唯一性，只要证明：如果$R$是$R'$和$R''$的直和，则每个$R_i$必然包含在$R'$或$R''$中。令$V', V'', V'_i, V''_i$为$R', R'', R' \cap R_i, R'' \cap R_i$生成的$V$的向量子空间。由于和 $V' + V''$ 是直接的，因此和 $V'_i + V''_i$ 是直接的。由于$R_i \subseteq R' \cup R''$，$R_i$是根系$R' \cap R_i$和$R'' \cap R_i$中的直和；因此$R' \cap R_i = \varnothing$或$R'' \cap R_i = \varnothing$，这证明了断言。

$R_i$ 被称为 $R$ 的*不可约分量*。对于任何非零标量$\lambda_i$，$\lambda_i R_i$的并是$V$中的根系，其逆系是$\lambda_i^{-1} R_i$的并，其Weyl群是$W(R)$。

#### 命题 7 {#lie-vi-s1-prop-7 .statement tag=0AUI}

*令$R$为$V$、$(R_i)$不可约成分族中的根系，由$R_i$、$B$不变对称生成$V$的$V_i$向量子空间双线性形式在命题3中定义的$V$上，而$B'$是$V$上的对称双线性形式在$W(R)$下不变。那么$V_i$相对于$B'$两两正交，并且对于所有$i$，$B$的限制和$B'$到$V_i$成比例。*

如果$v_i \in V_i, v_j \in V_j, i \neq j$，并且如果$w \in W(R_j)$，那么
$$
B'(v_i, w(v_j)) = B'(v_i, v_j),
$$
这表明$w(v_j) - v_j$关于$B'$与$v_i$正交。由于$V_j$对于$W(R_j)$是不可约的，它是由$w(v_j) - v_j$生成的，因此它与$V_i$正交。

The fact that the restrictions of $B$ and $B'$ to each of the $V_i$ are proportional follows from Prop. 1 of Chap. V, § 2, no. 1。

#### 注 {#lie-vi-s1-n2-rem-1 .statement tag=0AUJ}

选择标量乘积在$V_R$ $W(R)$ 下不变量。然后就可以谈论根的*长度*和两个根之间的*角度*。命题 7 表明，这个角度与标量乘积的选择无关，就像两个根的长度之比一样，前提是它们属于与 $R$ 的*相同*不可约分量。

### 3. 关系两个根之间

回想一下，*我们从现在开始假设*$k = \mathbf{R}$。 （我们将通过使用 no. 1 的 *注 2* 中指示的方法，将定义和结果扩展到一般情况的任务留给读者。）

*以下，$R$表示向量空间$V$中的根系；并且 $V$ 在 $W(R)$、cf. 命题 3 下配备了标量乘积 $(x, y) \mapsto (x|y)$ 不变量。*

让$\alpha, \beta \in R$。由no. 1的公式(7)，
$$
n(\alpha, \beta)n(\beta, \alpha) = 4 \cos^2 (\widehat{\alpha, \beta}) \leq 4.
$$

因此，整数$n(\alpha, \beta)n(\beta, \alpha)$必须取值0、1、2、3、4之一。 V, § 2, no. 5，科。第 6 号提案以及第 1 章页脚注。 V, § 4, no. 8，我们看到唯一的可能性如下，直到交换$\alpha$和$\beta$：

1) $n(\alpha, \beta) = n(\beta, \alpha) = 0;$
   $$
   (\overline{\alpha, \beta}) = \frac{\pi}{2}; \quad s_{\alpha}s_{\beta} \text{ of order } 2;
   $$
2) $n(\alpha, \beta) = n(\beta, \alpha) = 1;$
   $$
   (\overline{\alpha, \beta}) = \frac{\pi}{3}; \quad s_{\alpha}s_{\beta} \text{ of order } 3;
   $$
   $$
   \| \alpha \| = \| \beta \|;
   $$
3）$n(\alpha, \beta) = n(\beta, \alpha) = -1;$
   $$
   (\overline{\alpha, \beta}) = \frac{2\pi}{3}; \quad s_{\alpha}s_{\beta} \text{ of order } 3;
   $$
   $$
   \| \alpha \| = \| \beta \|;
   $$
4) $n(\alpha, \beta) = 1,\ n(\beta, \alpha) = 2;$
   $$
   (\overline{\alpha, \beta}) = \frac{\pi}{4}; \quad s_{\alpha}s_{\beta} \text{ of order } 4;
   $$
   $$
   \| \beta \| = \sqrt{2}\ \| \alpha \|;
   $$
5) $n(\alpha, \beta) = -1,\ n(\beta, \alpha) = -2;$
   $$
   (\overline{\alpha, \beta}) = \frac{3\pi}{4}; \quad s_{\alpha}s_{\beta} \text{ of order } 4;
   $$
   $$
   \| \beta \| = \sqrt{2}\ \| \alpha \|;
   $$
6) $n(\alpha, \beta) = 1,\ n(\beta, \alpha) = 3;$
   $$
   (\overline{\alpha, \beta}) = \frac{\pi}{6}; \quad s_{\alpha}s_{\beta} \text{ of order } 6;
   $$
   $$
   \| \beta \| = \sqrt{3}\ \| \alpha \|;
   $$
7) $n(\alpha, \beta) = -1,\ n(\beta, \alpha) = -3;$
   $$
   (\overline{\alpha, \beta}) = \frac{5\pi}{6}; \quad s_{\alpha}s_{\beta} \text{ of order } 6;
   $$
   $$
   \| \beta \| = \sqrt{3}\ \| \alpha \|;
   $$
8) $n(\alpha, \beta) = n(\beta, \alpha) = 2;$
   $$
   \alpha = \beta;
   $$
9) $n(\alpha, \beta) = n(\beta, \alpha) = -2;$
   $$
   \alpha = -\beta;
   $$
10) $n(\alpha, \beta) = 1,\ n(\beta, \alpha) = 4;$
    $$
    \beta = 2\alpha;
    $$
11) $n(\alpha, \beta) = -1,\ n(\beta, \alpha) = -4;$
    $$
    \beta = -2\alpha.
    $$

尤其：

#### 命题 8 {#lie-vi-s1-prop-8 .statement tag=0AUK}

(i) *如果两个根成比例，则比例的因子只能是$\pm 1, \pm \frac{1}{2}, \pm 2$。*

(ii) *如果$\alpha$和$\beta$是两个不成比例的根，并且如果$\| \alpha \| \leq \| \beta \|$，则$n(\alpha, \beta)$取值 0, 1, -1之一。*

如果根 $\alpha \in \mathbf{R}$ 满足 $\frac{1}{2}\alpha \notin \mathbf{R}$，则 $\alpha$ 称为*不可整除* 根。

#### 定理 1 {#lie-vi-s1-thm-1 .statement tag=0AUL}

*令$\alpha, \beta$等于两个根。*

(i) *如果 $n(\alpha, \beta) > 0$，$\alpha - \beta$ 为根除非 $\alpha = \beta$。*
(ii) *如果 $n(\alpha, \beta) < 0$，$\alpha + \beta$ 为根除非 $\alpha = -\beta$。*

如果$n(\alpha, \beta) > 0$，根据上面的列表，可能性如下：

1）$n(\alpha, \beta) = 1$；然后$\alpha - \beta - s_{\beta}(\alpha) \in \mathbf{R}$；
2）$n(\beta, \alpha) = 1$；那么$\beta - \alpha = s_{\alpha}(\beta) \in \mathbf{R}$，所以$\alpha - \beta \in \mathbf{R}$；
3）$\beta = \alpha$。

通过将 $\beta$ 更改为 $-\beta$，可以证明 (i) 和 (ii)。

#### 推论{#lie-vi-s1-n3-cor-1 .statement tag=0AUM}

令$\alpha$和$\beta$为两个根。

(i) *如果* $(\alpha|\beta) > 0$，$\alpha - \beta$ 为根除非 $\alpha = \beta$。
(ii) *如果* $(\alpha|\beta) < 0$，$\alpha + \beta$ 为根除非 $\alpha = -\beta$。
(iii) *如果* $\alpha - \beta \notin \mathbf{R} \cup \{0\}$ 和 $\alpha + \beta \notin \mathbf{R} \cup \{0\}$，*则* $(\alpha|\beta) = 0$。

断言 (i) 和 (ii) 从 Th 开始。 1 和 no. 1 的公式 (7)。 断言 (iii) 由 (i) 和 (ii) 得出。

有可能是$\alpha + \beta \in \mathbf{R}$、$(\alpha|\beta) = 0$（cf.板X、系统B_2）。当 $\alpha - \beta \notin \mathbf{R} \cup \{0\}$ 和 $\alpha + \beta \notin \mathbf{R} \cup \{0\}$ 时，$\alpha$ 和 $\beta$ 被称为“强正交”。

#### 命题 9 {#lie-vi-s1-prop-9 .statement tag=0AUN}

令$\alpha$和$\beta$为两个不成比例的根。

(i) *集合* I *of 整数* j *使得* $\beta + j\alpha$ *是根是一个区间* $[ -q, p ]$ *in* $\mathbf{Z}$ *包含* 0。
(ii) *令* S *为* $\beta + j\alpha$ *的集合 *对于* $j \in \mathrm{I}$。 *然后*,
$$
s_{\alpha}(S) = S \quad \text{and} \quad s_{\alpha}(\beta + p\alpha) = \beta - q\alpha.
$$
（三）$p - q = -n(\beta, \alpha)$。

显然，$0 \in \mathrm{I}$。令$p$（或$-q$）为最大的（或最小的）元素 / I。如果 $[ -q, p ]$ 属于到 I 中不存在所有整数，则$[ -q, p ]$ 中存在两个整数 $r, s$，其属性如下：$s > r + 1, s \in \mathrm{I}, r \in \mathrm{I}, r + k \notin \mathrm{I}$ 对应$1 \leq k \leq s - r - 1$。与Cor的记号。的 Th。 1、$(\alpha|\beta + s\alpha) \leq 0, (\alpha|\beta + r\alpha) \geq 0$，这是荒谬的，因为
$$
(\alpha|\beta + s\alpha) \leq 0 > (\alpha|\beta + r\alpha).
$$
这就证明了(i)。

我们有 $s_{\alpha}(\beta + j\alpha) = \beta - n(\beta, \alpha)\alpha - j\alpha = \beta + j'\alpha$ 和 $j' = -j - n(\beta, \alpha)$。因而$s_{\alpha}(S) \subseteq S$，进而$s_{\alpha}(S) = S$。现在$j \mapsto -j - n(\beta, \alpha)$从I变为递减双射到I。由此可见，当$j = p$时$j' = -q$，从而$-q = -p - n(\beta, \alpha)$。这就证明了(ii)和(iii)。

集合 S 被称为$\beta$定义的根的$\alpha$链，$\beta - q\alpha$是它的起点，$\beta + p\alpha$是它的终点，$p + q$是它的长度。

#### 推论{#lie-vi-s1-n3-cor-2 .statement tag=0AUO}

设S是根的$\alpha$链，$\gamma$是S的原点。S的长度是$-n(\gamma, \alpha)$；它等于 0、1、2 或 3。

第一个断言源自第9条第(iii)条，应用于$\beta = \gamma$，并使用$q = 0$这一事实。

另一方面，由于$\gamma$与$\alpha$不成比例，因此在本号开头给出的列表。表明 $|n(\gamma, \alpha)| \leq 3$，因此得出推论。

#### 注 {#lie-vi-s1-n3-rem-1 .statement tag=0AUP}

我们保留上面的记号。然后：

1) 如果S的长度为0，则$(\alpha|\gamma) = 0$。

2）如果S的长度为1，则$n(\gamma, \alpha) = -1$，分三种情况：

$$
n(\alpha, \gamma) = -1, \quad (\alpha|\alpha) = (\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{1}{2}(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{2\pi}{3}
$$
$$
n(\alpha, \gamma) = -2, \quad (\alpha|\alpha) = 2(\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{1}{2}(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{3\pi}{4}
$$
$$
n(\alpha, \gamma) = -3, \quad (\alpha|\alpha) = 3(\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{1}{2}(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{5\pi}{6}
$$

![三个图表显示根系，角度标记为 π/3、π/4、2π/3 和向量 γ + α、γ、γ + 2α](../images/root_systems_1.png)

3）如果S的长度是2，那么$n(\gamma, \alpha) = -2$，所以

$$
n(\alpha, \gamma) = -1, \quad (\alpha|\alpha) = \frac{1}{2}(\gamma|\gamma), \quad (\alpha|\gamma) = -(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{3\pi}{4}.
$$

![图表显示根系，角度为 π/4、π/4 和向量 γ、γ + α、γ + 2α](../images/root_systems_2.png)

4）如果S的长度是3，那么$n(\gamma, \alpha) = -3$，所以

$$
n(\alpha, \gamma) = -1, \quad (\alpha|\alpha) = \frac{1}{3}(\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{3}{2}(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{5\pi}{6}.
$$

![图表显示根系，角度为 π/6、π/3、π/6 和向量 γ、γ + α、γ + 2α、γ + 3α](../images/root_systems_3.png)

我们将会看到（图板X、系统A2、B2、G2）所有这些情况都实际实现了。

#### 命题 10 {#lie-vi-s1-prop-10 .statement tag=0AUQ}

*令$\alpha, \beta$为两个不成比例的根，使得$\beta + \alpha$为根。令第 9 条命题中的 $p, q$ 为整数。那么*

$$
\frac{(\beta + \alpha|\beta + \alpha)}{(\beta|\beta)} = \frac{q + 1}{p}.
$$

令 S 为由 $\beta, \gamma$ 其原点定义的 $\alpha$ 链；它的长度$l$是$\geq 1$，因为$\beta + \alpha$是根。可能有以下情况：

1）$l = 1$；然后$\beta = \gamma, q = 0, p = 1, (\beta + \alpha|\beta + \alpha) = (\beta|\beta)$。
2）$l = 2, \beta = \gamma$；然后$q = 0, p = 2, (\beta + \alpha|\beta + \alpha) = \frac{1}{2}(\beta|\beta)$。
3）$l = 2, \beta = \gamma + \alpha$；然后$q = 1, p = 1, (\beta + \alpha|\beta + \alpha) = 2(\beta|\beta)$。

4）$l = 3, \beta = \gamma$；然后$q = 0, p = 3, (\beta + \alpha|\beta + \alpha) = \frac{1}{3}(\beta|\beta)$。
5）$l = 3, \beta = \gamma + \alpha$；然后$q = 1, p = 2, (\beta + \alpha|\beta + \alpha) = (\beta|\beta)$。
6）$l = 3, \beta = \gamma + 2\alpha$；然后$q = 2, p = 1, (\beta + \alpha|\beta + \alpha) = 3(\beta|\beta)$。

在每种情况下，都满足要证明的公式。

#### 命题 11 {#lie-vi-s1-prop-11 .statement tag=0AUR}

*假设 R 是不可约的。令$\alpha$和$\beta$为两个根，使得$\| \alpha \| = \| \beta \|$。存在 $g \in W(R)$ 使得 $g(\alpha) = \beta$.*

$\alpha$的变换由$W(R)$生成V（no. 2，第5号提案的Cor.）。因此存在$g \in W(R)$使得$(g(\alpha)|\beta) \neq 0$。从现在开始我们假设$(\alpha|\beta) \neq 0$。由no. 1、$n(\alpha, \beta) = n(\beta, \alpha)$的公式(9)。 替换 $\beta$ 如果需要$s_\beta(\beta) = -\beta$，我们可以假设$n(\alpha, \beta) > 0$。然后，根据no. 3开头的列表，要么是$\alpha = \beta$（在这种情况下命题是明确的），要么是$n(\alpha, \beta) = n(\beta, \alpha) = 1$；在那种情况下

$$
s_\alpha s_\beta s_\alpha(\beta) = s_\alpha s_\beta(\beta - \alpha) = s_\alpha(-\beta - \alpha + \beta) = \alpha.
$$

### 4.约化根系

如果系统中的每个根都不可整除（no. 3），则称根系是“约简”的。

#### 命题 12 {#lie-vi-s1-prop-12 .statement tag=0AUS}

*假设 R 是不可约且可约化的。*

(i) *$\alpha \in R, \beta \in R$的比率$\frac{(\beta|\beta)}{(\alpha|\alpha)}$必须取值 1, 2, $\frac{1}{2}$, 3, $\frac{1}{3}$之一。*

(ii) *$\alpha \in R$的$(\alpha|\alpha)$中的集合至多有两个元素。*

由于 R 是不可约的，根的变换乘以 $W(R)$ 生成 V（no. 2，Prop. 5 的 Cor.）。因此，对于任何根$\alpha, \beta$，都存在根$\beta'$，使得$(\alpha|\beta') \neq 0$和$(\beta'|\beta') = (\beta|\beta)$。通过no. 1的公式(9)和no. 3的列表，$\frac{(\beta'|\beta')}{(\alpha|\alpha)}$取值1、2、$\frac{1}{2}$、3、$\frac{1}{3}$之一（回想一下，假设系统被约简）。通过将$(x|y)$乘以合适的标量，我们可以假设$(\alpha|\alpha) = 1$对于某些根，并且$(\beta|\beta)$对于$\beta \in R$的其他可能的值是2和3。值2和3不能都可以得到，因为在这种情况下有将存在$\beta \in R, \gamma \in R$使得$\frac{(\gamma|\gamma)}{(\beta|\beta)} = \frac{3}{2}$，与我们上面看到的相反。

#### 命题 13 {#lie-vi-s1-prop-13 .statement tag=0AUT}

*假设 R 是不可约的、不可约的且为秩 $\geq 2$。*

(i) *不可分割的根中的集合$R_0$是V中的根系；这个系统是不可约的，也是可约的；和 $W(R_0) = W(R)$.*

(ii) *令 A 为根 $\alpha$ 中的集合，其中 $(\alpha|\alpha)$ 取最小的值 $\lambda$。那么 A 的任意两个不成比例的元素都是正交的。*

(iii) *令 B 为 $\beta \in R$ 的集合，使得 $(\beta|\beta) = 2\lambda$。然后$B \neq \varnothing$、$R_0 = A \cup B$、$R = A \cup B \cup 2A$。*

如果$\alpha \in R - R_0$，那么$\frac{1}{2} \alpha \in R$，但是$\frac{1}{2} (\frac{1}{2} \alpha) \notin R$（命题8），所以$\frac{1}{2} \alpha \in R_0$。这证明$R_0$满足(RS$_1$)。显然，对于所有$\alpha \in R$，$s_{\alpha, \alpha^-}(R_0) = R_0$，所以$R_0$满足(RS$_{II}$)和(RS$_{III}$)。由于$\alpha \in R - R_0$意味着$\frac{1}{2} \alpha \in R_0$，并且由于$s_\alpha = s_{\alpha/2}$，我们有$W(R) = W(R_0)$。因此$R_0$是不可约的（Prop.5的Cor.），并且它显然是约简的。

由于$R$没有被约简，所以存在$\alpha \in R_0$使得$2\alpha \in R$。由于 $R_0$ 不可约且 $\dim V \geq 2$、$\alpha$ 不能与每个根成比例或正交。令$\beta \in R_0$使得$n(\beta, \alpha) \neq 0$和$\beta$不与$\alpha$成比例。如有必要，将$\beta$更改为$-\beta$，我们可以假设$n(\beta, \alpha) > 0$。现在$\frac{1}{2} n(\beta, \alpha) = n(\beta, 2\alpha) \in \mathbf{Z}$，所以$n(\beta, \alpha) \in 2\mathbf{Z}$。来自no. 3、$n(\beta, \alpha) = 2$、$(\beta|\beta) = 2(\alpha|\alpha)$的列表。由于 $R_0$ 被约化，第 12 条命题表明，对于所有 $\gamma \in R_0$，要么是 $(\gamma|\gamma) = (\alpha|\alpha)$，要么是 $(\gamma|\gamma) = 2(\alpha|\alpha)$。另外，上式还表明，对于所有 $\gamma \in R - R_0$，向量 $\frac{1}{2} \gamma$ 是 $R_0$ 的元素，从而 $(\frac{1}{2} \gamma|\frac{1}{2} \gamma) = (\alpha|\alpha)$。因此，$\lambda = (\alpha|\alpha)$、$B \neq \varnothing$、$R_0 = A \cup B$和$R \subseteq A \cup B \cup 2A$；另一方面，如果$\gamma \in A$，则存在$g \in W(R)$使得$\gamma = g(\alpha)$（命题11），所以$2\gamma = g(2\alpha) \in R$；因此$2A \subseteq R$和$R = A \cup B \cup 2A$。最后，令$\gamma, \gamma'$为$A$的两个不成比例的元素。然后

$$
n(2\gamma, \gamma') = 2n(\gamma, \gamma') = 4n(\gamma, 2\gamma') \in 4\mathbf{Z}, \quad \text{and} \quad |n(\gamma, \gamma')| \leq 1
$$

由于$\gamma$和$\gamma'$具有相同的长度，因此$n(\gamma, \gamma') = 0$和$(\gamma|\gamma') = 0$。

#### 命题 14 {#lie-vi-s1-prop-14 .statement tag=0AUU}

*假设$R$是不可约且可约的，并且$(\alpha|\alpha)$需要值$\lambda$和$2\lambda$来换取$\alpha \in R$。令$A$为根$\alpha$的集合，使得$(\alpha|\alpha) = \lambda$。假设 $A$ 中任意两个不成比例的元素是正交的。那么$R_1 = R \cup 2A$是不可约非约约根系，$R$是$R_1$不可分的根的集合。*

显然$R_1$满足(RS$_1$)和(RS$_{III}$)。我们证明，如果$\alpha, \beta \in R_1$，则$\langle \alpha^-, \beta \rangle \in \mathbf{Z}$。如果$\alpha \in R$，这很清楚。由于$\alpha \in A$是$(2\alpha)^- = \frac{1}{2} \alpha^-$，所以如果$\alpha, \beta \in 2A$也是直接的。最后，假设 $\beta \in R$ 和 $\alpha = 2\gamma$ 以及 $\gamma \in A$。

1) 如果$\gamma = \pm \beta$，则$\langle \alpha^-, \beta \rangle = \pm \frac{1}{2} \langle \gamma^-, \gamma \rangle = \pm 1$。
2) 如果$\gamma$ 与$\beta$ 不成比例，且$\beta \in A$、假设在$A$ 上意味着$\langle \gamma^-, \beta \rangle = 0$，因此$\langle \alpha^-, \beta \rangle = 0$。
3) 如果$\beta \in R - A$，则$(\beta|\beta) = 2\lambda = 2(\gamma|\gamma)$，因此根据no. 3中的列表，$\langle \beta, \gamma^- \rangle$等于0、2或-2。因此$\langle \beta, \alpha^- \rangle = \frac{1}{2} \langle \beta, \gamma^- \rangle \in \mathbf{Z}$。

这样$R_1$就是$V$中的根系，其他断言就清楚了。

### 5. 房间和根系的基

对于所有$\alpha \in R$，令$L_\alpha$为点的$V$由……组成的超平面在$s_\alpha$下不变。 $V$中由$L_\alpha$（第V, § 1, no. 3章）的集合确定的房间称为$R$的*房间*。由标量乘积$(x|y)$定义的双射$V \to V^*$对于$\alpha \in R$来说需要$\alpha$到$\frac{2\alpha^-}{(\alpha^-|\alpha^-)}$，因此$L_\alpha$到$L_{\alpha^-}$，因此$R$的室到$R^-$。如果$C$是$R$的腔室，则$R^-$的相应的腔室由$C^-$表示。根据no. 2的第7条，$C^-$仅依赖于$C$，而不依赖于$(x|y)$的选择。

#### 定理 2 {#lie-vi-s1-thm-2 .statement tag=0AUV}

(i) *群* $W(R)$ *简单传递作用于室的集合*。

(ii) *设* $C$ *为一个房间。那么*$\overline{C}$*是*$W(R)$的基本域。

(iii) $C$ *是一个开单纯锥体*（第 V, § 1, no. 6 章）。

(iv) *设* $L_1, L_2, \ldots, L_l$ *为* $C$ 的墙。 *对于所有* $i$，*存在唯一不可分割的根* $\alpha_i$ *使得* $L_i = L_{\alpha_i}$ *并且使得* $\alpha_i$ *与* $L_i$ *与* $C$ 在同一侧。

(v) *集合* $B(C) = \{ \alpha_1, \ldots, \alpha_l \}$ *是* $V$ 的基。

(vi) $C$ *是* $x \in V$ *的集合，使得* $\langle \alpha_i, x \rangle > 0$ *对于所有* $i$ *（或者，等效地，集合属于* $x \in V$ *使得* $(x|\alpha_i) > 0$ *对于所有* $i$）。

(vii) *设*$S$*为*$s_{\alpha_i}$的集合。 *对* $(W(R), S)$ *是 Coxeter 系统*（第 IV, § 1, no. 3 章）。

断言 (i) 和 (vii) 源自第 1 章。 V, § 3, no. 2，周四。 1. 断言 (ii) 源自第 1 章。 V, § 3, no. 3，周四。 2. 断言 (iv) 清楚。 根$\alpha_i$与$L_i$正交，$\alpha_i^-$与$2\alpha_i / (\alpha_i|\alpha_i)$一致。由于$W(R)$是必不可少的（no. 1，*注3*），断言（iii），（v）和（vi）来自第1章。 V, § 3, no. 9，提案 7。

#### 注 1 {#lie-vi-s1-n5-rem-1 .statement tag=0AUW}

断言 (vii) 特别表明$W(R)$ 是由反射$s_{\alpha_i}$“生成”的。

#### 注 2 {#lie-vi-s1-n5-rem-2 .statement tag=0AUX}

如果$x, y \in C$，则$(x|y) > 0$（第V, § 3, no. 5，引理 6），在其他字中，$(x, y)$是*锐角*。

#### 注 3 {#lie-vi-s1-n5-rem-3 .statement tag=0AUY}

设$m(\alpha, \beta)$为$s_{\alpha} s_{\beta}$($\alpha, \beta \in B(C)$)中的阶。 矩阵 $(m(\alpha, \beta))$ 与 $(W, S)$ 的 *Coxeter 矩阵*（第 IV, § 1, no. 9 章）进行标识。如果 $\alpha \neq \beta$，第 3 章的命题 3 V, § 3, no. 4表明角度$(\alpha, \beta)$等于$\pi - \frac{\pi}{m(\alpha, \beta)}$；特别地，这个角或者是钝角或者等于$\pi$和$(\alpha|\beta) \leq 0$。通过使用no. 3中的列表，$m(\alpha, \beta)$ *等于* 2, 3, 4 *或* 6。

#### 定义 2 {#lie-vi-s1-def-2 .statement tag=0AUZ}

*子集* $B$ *of* $R$ *被称为基 of* $R$ *如果存在一个房间* $C$ *of* $R$ *这样* $B = B(C)$。 *如果*$C$*是一个房间*，$B(C)$*被称为*$R$*定义的基*由*$C$定义。

#### 注 4 {#lie-vi-s1-n5-rem-4 .statement tag=0AV0}

断言 (vi) 的 Th。图2示出了映射$C \mapsto B(C)$是从集合室到基的集合的*双射*。因而，$W(R)$ *简单传递*作用于基的集合。

#### 注 5 {#lie-vi-s1-n5-rem-5 .statement tag=0AV1}

令$C$为$R$的腔室，并令$B$为相应的基。如果$\alpha \in B$，如果$2\alpha \notin R$则放入$\varphi(\alpha) = \alpha^-$，如果$2\alpha \in R$则放入$\varphi(\alpha) = \frac{1}{2}\alpha^-$。那么$\varphi(B)$ *是* $R^-$ *的基 *由* $C^-$定义；这是因为$C^-$的墙是$L_{\alpha^-}$，对于$\alpha \in B$。

#### 定义 3 {#lie-vi-s1-def-3 .statement tag=0AV2}

设B为R的基。R（相对于B）的嘉当矩阵为矩阵$(n(\alpha, \beta))_{\alpha, \beta \in B}$。

对于所有 $\alpha \in B$、$n(\alpha, \alpha) = 2$。对于$\alpha, \beta \in B$，

$$
n(\alpha, \beta) = 2 \frac{(\alpha|\beta)}{(\beta|\beta)} = -2 \frac{\|\alpha\|}{\|\beta\|} \cos \frac{\pi}{m(\alpha, \beta)},
$$

其中$m(\alpha, \beta)$表示如上阶 of $s_\alpha s_\beta$。如果$\alpha \neq \beta$、$n(\alpha, \beta) = 0, -1, -2$或$-3$（cf.no. 3）。

#### 注 6 {#lie-vi-s1-n5-rem-6 .statement tag=0AV3}

Cartan 矩阵 $(n(\alpha, \beta))$ 不应与 Coxeter 矩阵 $(m(\alpha, \beta))$ 混淆。 注特别是嘉当矩阵不一定是对称的。

#### 注 7 {#lie-vi-s1-n5-rem-7 .statement tag=0AV4}

规范索引。如果B和$B'$是R的两个基，则存在唯一元素$w \in W$使得$w(B) = B'$。我们有

$$
n(w(\alpha), w(\beta)) = n(\alpha, \beta) \quad \text{and} \quad m(w(\alpha), w(\beta)) = m(\alpha, \beta)
$$

$\alpha, \beta \in B$。因而，与 B 相关的嘉当和考克塞特矩阵可以通过合成和双射从与 $B'$ 相关的那些中获得

$$
\alpha \mapsto w(\alpha)
$$

从B到$B'$。

Cartan 和 Coxeter 矩阵实际上可以通过以下方式进行规范定义。令X为对$(B, \alpha)$的集合，其中B为R的基和$\alpha \in B$。 群 W 以明显的方式作用于 X，并且 W 在 X 上的每个轨道恰好在一个点中满足集合 $\{B\} \times B$ 中的每一个。如果I是这些轨道中的集合，则每个基B承认规范索引$(\alpha_i)_{i \in I}$。此外，存在唯一的矩阵$N = (n_{ij})$（分别为$M = (m_{ij})$），型$I \times I$，使得对于任何基B，与B相关的嘉当（分别为Coxeter）矩阵可以通过以下方式从N（分别为M）获得具有 B 的规范索引；它被称为 R 的规范 Cartan 矩阵（分别为 Coxeter 矩阵）。

#### 命题 15 {#lie-vi-s1-prop-15 .statement tag=0AV5}

令 B 为 R 的基，且 $\alpha$ 是不可分割的根。存在$\beta \in B$和$w \in W(R)$使得$\alpha = w(\beta)$。

让 C 成为$B = B(C)$ 的腔室。 超平面$L_\alpha$是R的室$C'$的壁，存在变换$C'$至C的$W(R)$的元素。因而，我们被简化为$L_\alpha$是C的墙。那么$\alpha$与R的元素$\beta$成正比。由于$\alpha$和$\beta$不可整除，所以$\alpha = \pm \beta$。如果$\alpha = -\beta$，则$\alpha = s_\beta(\beta)$，因此命题。

#### 推论{#lie-vi-s1-n5-cor-1 .statement tag=0AV6}

令$R_1$和$R_2$为向量空间、$V_1$和$V_2$中的两个约化根系，并令$B_1$和$B_2$为$R_1$和$R_2$中的基。设$f : B_1 \to B_2$为双射，即变换$R_1$的嘉当矩阵与$R_2$的嘉当矩阵。那么对于所有$\alpha \in B_1$，存在同构$F : V_1 \to V_2$、变换、$R_1$到$R_2$和$\alpha$到$f(\alpha)$。

令$F$为从$V_1$到$V_2$的同构，对于所有$\alpha \in B_1$需要$\alpha$到$f(\alpha)$。然后$F$变换$s_\alpha$到$s_{f(\alpha)}$，因此$W(R_1)$到$W(R_2)$（Th.2），因此$R_1$到$R_2$（提案15）。

#### 命题 16 {#lie-vi-s1-prop-16 .statement tag=0AV7}

令$B$为$R$的基，并且$G$子群为元素的$A(R)$由……组成，使$B$保持稳定。那么$W(R)$是$A(R)$的正常子群，$A(R)$是$G$和$W(R)$的半直接乘积。

若$\alpha \in R$且$t \in A(R)$，则$ts_\alpha t^{-1} = s_{t(\alpha)}$；由于$W(R)$是由$s_\alpha$生成的，我们看到$W(R)$是$A(R)$的正常子群。由结构迁移、$R$$A(R)$变换基至$R$基。由于$W(R)$对基的集合作用简单传递，$A(R)$的每个元素都可以唯一地写成形式$g_1 g_2$，其中$g_1 \in W(R)$和$g_2 \in G$。

#### 注 8 {#lie-vi-s1-n5-rem-8 .statement tag=0AV8}

令$R_1, \ldots, R_p$为向量空间$V_1, \ldots, V_p$中的根系，$V = \prod_i V_i$中的$R_i$的$R$直和，$C_i$为$R_i$和$B_i = B(C_i)$的腔室。 $C = \prod_i C_i$是$R$的一个房间，直接的是$B(C) = \bigcup_i B_i$。这是从 Th 得出的。 2 如此得到所有的室和$R$的基。

### 6. 积极根

令$C$为$R$的腔室，并令$B(C) = \{ \alpha_1, \ldots, \alpha_l \}$为$R$的相应的基。 The order relation on $V$ (resp. $V^*$) defined by $C$ is the order relation compatible with the vector space structure of $V$ (resp. $V^*$) for which the elements $\geq 0$ are the linear combinations of the $\alpha_i$ (resp. the $\alpha_i^*$) with coefficients $\geq 0$. 对于这些关系之一为正值的元素被认为对于 $C$ 为正值，或者对于基 $B(C)$ 为正值。 这些序关系也由$C^*$定义，正如通过使用$W(R)$下的标量乘积不变量将$V$与$V^*$识别一样。 鉴于 Th. 2、$V^*$的no. 5、元素为$\geq 0$当且仅当其$C$上的值为$\geq 0$。 当且仅当$C^*$上的值是$\geq 0$时，$V$的元素$x$是$\geq 0$，或者等效地，如果对于所有$y \in C$来说$(x|y) \geq 0$。

The elements of $\overline{C}$ are $\geq 0$ for $C$ by Lemma 6 of Chap. V, § 3, no. 5。 但是 $C$ 的元素 $\geq 0$ 的集合一般不同于 $\overline{C}$ (cf. 板X、系统$A_2, B_2, G_2$）。

#### 定理 3 {#lie-vi-s1-thm-3 .statement tag=0AV9}

每个根都是线性组合，其中整数系数与元素或$B(C)$的符号相同。特别是，每个根对于 $C$ 要么是正数，要么是负数。

如果$\alpha$的$\alpha \in R$、核$L_\alpha$不满足$C^*$，那么$\alpha$要么是整个$C^*$的$> 0$，要么是整个$C^*$的$< 0$，因此是第二个断言。还需要证明$\alpha$包含在$B(C)$生成的$V$的子群$P$中；我们可以假设 $\alpha$ 是不可分的。现在群 $P$ 显然稳定在 $s_{\gamma}$ 之下，对于 $\gamma \in B(C)$，因此 Th 也低于 $W(R)$。 2. 由于$\alpha$是形式$w(\beta)$，加上$w \in W(R)$和$\beta \in B(C)$（cf.命题15），我们有$\alpha \in P$。 Q.E.D.

用根的 $R_+(C)$ 集合表示，对于 $C$ 为正。因此，
$$
R = R_+(C) \cup (-R_+(C))
$$
是划分 / $R$。

#### 推论{#lie-vi-s1-n6-cor-1 .statement tag=0AVA}

*令$\gamma$为根的线性组合，系数为整数，且$\alpha$不可分割的根。如果 $\gamma$ 与 $\alpha$ 成比例，则 $\gamma \in \mathbf{Z}\alpha$。*

根据no. 5的第15条命题，可以选择$C$，从而得到$\alpha \in B(C)$。由 Th. 3、
$$
\gamma = \sum_{\beta \in B(C)} n_{\beta} \beta \quad \text{with} \quad n_{\beta} \in \mathbf{Z}.
$$
因此，如果$\gamma$与$\alpha$成正比，则$\gamma = n_{\alpha} \alpha$，这就证明了推论。

现在令$S$为$\alpha \in B(C)$的反射$s_{\alpha}$的集合，并令$T$为$W$下$S$的共轭的并。对于$\alpha \in B(C)$和$w \in W$，$T$的元素$t = ws_{\alpha}w^{-1}$是与根$\beta = w(\alpha)$相关的正交反射$s_{\beta}$；相反，对于任何不可分割的根$\beta$，存在元素$w \in W$，使得$\alpha = w^{-1}(\beta) \in B(C)$（第15条命题）和$s_{\beta} = ws_{\alpha}w^{-1} \in T$。因此，从不可分割的根到 $\{\pm 1\} \times T$ 的集合的 *双射* $\psi$ 是通过关联到不可分割的根 $\beta$ 对 $(\varepsilon, s_{\beta})$ 获得的，其中 $\varepsilon = +1$如果 $\beta$ 为正，则 $\varepsilon = -1$ 如果 $\beta$ 为负。

另一方面，$(W, S)$ 是 Coxeter 系统（Th.2），并且是第 2 章的结果。 IV, § 1, no. 4可以申请。我们已经看到，如果$w$是长度（相对于$S$）$W$元素等于$q$，则存在$T$的子集$T_w$，和$q$ 元素，这样，如果 $w = s_1 \ldots s_q$ 与 $s_i \in S$ 并且如果
$$
t_i = s_1 \ldots s_{i-1} s_i s_{i-1} \ldots s_1
$$
（$1 \leq i \leq q$），然后$T_w = \{t_1, \ldots, t_q\}$。回想一下，我们还在 § 1 数 $\eta(w, t)$（对于$w \in W$和$t \in T$）中定义了no. 4，如果$t \notin T_w$则等于$+1$，如果$t \in T_w$则等于$-1$。最后，回想一下，如果我们通过公式从集合 $\{\pm 1\} \times T$ 定义映射 $U_w$ 到自身
$$
U_w(\varepsilon, t) = (\varepsilon \eta(w^{-1}, t), wt w^{-1}),
$$
映射$w \mapsto U_w$是集合$\{\pm 1\} \times T$的置换从$W$到群的*同态*（第IV, § 1, no. 4、引理1）。

#### 命题 17 {#lie-vi-s1-prop-17 .statement tag=0AVB}

*假设减少$R$，令$w \in W$和$\alpha \in R$。*

(i) *我们有$\psi(w(\alpha)) = U_w(\psi(\alpha))$。*
(ii) *假设 $\alpha$ 为正。 根 $w(\alpha)$ 为负当且仅当*
$$
\eta(w^{-1}, s_{\alpha}) = -1,
$$
*在其他字如果*$s_{\alpha} \in T_{w^{-1}}$。

(iii) 当且仅当室 C 和 $w(C)$ 位于超平面 $L_\alpha$ 的相对两侧时，我们才有 $\eta(w, s_\alpha) = -1$。在其他字中，集合 $T_w$ 由相对于分隔 C 和 $w(C)$ 的墙壁的反射组成。

设$\beta \in B(C)$并放入$s = s_\beta$。显然 $T_s = \{ s \}$ 因而

$$
U_s(\varepsilon, t) = \begin{cases}
(\varepsilon, st s^{-1}) & \text{if } t \neq s \\
(-\varepsilon, s) & \text{if } t = s.
\end{cases}
$$

另一方面，令 $\rho = \sum_{\gamma \in B(C)} n_\gamma(\rho) \gamma$ 为正根。放

$$
s(\rho) = \sum_{\gamma \in B(C)} n_\gamma(s(\rho)) \gamma.
$$

如果$\rho \neq \beta$，则存在元素$\gamma \in B(C)$和$\gamma \neq \beta$，从而$n_\gamma(\rho) > 0$，并且我们有$n_\gamma(s(\rho)) = n_\gamma(\rho) > 0$（no. 1，公式（5））。因而$s(\rho)$为正。我们立即推断出

$$
\psi(s(\varepsilon, \rho)) = \begin{cases}
(\varepsilon, ss_\rho s^{-1}) & \text{if } \rho \neq \beta \\
(-\varepsilon, s) & \text{if } \rho = \beta.
\end{cases}
$$

(12) 和 (13) 的比较现在表明，对于所有根 $\gamma$ 和所有$s \in S$，$U_s(\psi(\gamma)) = \psi(s(\gamma))$。由于 S 生成 W，因而 (i) 如下。

另一方面，$w(\alpha)$为负数的说等价于说

$$
\psi(w(\alpha)) = (-1, ws_\alpha w^{-1}),
$$

或者，通过 (i)，$U_w(\psi(\alpha)) = (-1, ws_\alpha w^{-1})$。如果加法$\alpha$为正，则$\psi(\alpha) = (+1, s_\alpha)$和$U_w(\psi(\alpha)) = (\eta(w^{-1}, s_\alpha), ws_\alpha w^{-1})$，因而(ii)。

最后，根据(ii)，$\eta(w, s_\alpha) = -1$当且仅当根、$\alpha$和$w^{-1}(\alpha)$之一为正，另一个为负。这相当于所有$x \in C$的说和$(\alpha|x).(w^{-1}(\alpha)|x) = (\alpha|x).(w|x) < 0$，因此是(iii)中的第一个断言。 (iii) 中的第二个断言紧随其后。

#### 推出 1 {#lie-vi-s1-prop-17-cor-1 .statement tag=0AVC}

让$\beta \in B(C)$。反射$s_\beta$排列正值根，与$\beta$不成比例。

我们约化立即转向R减少的情况。在这种情况下，我们的断言由 (ii) 和 $T_{s_\beta} = s_\beta$ 得出。

#### 推出 2 {#lie-vi-s1-prop-17-cor-2 .statement tag=0AVD}

假设 R 减小。令$w \in W$，令q为$w$相对于S的长度（第IV, § 1, no. 1章），并令$w = s_1 \ldots s_q$为$w$的约化分解。令$\alpha_1, \ldots, \alpha_q$为$B(C)$相应的到$s_1, \ldots, s_q$中的元素。放

$$
\theta_i = s_q s_{q-1} \ldots s_{i+1}(\alpha_i), \quad i = 1, \ldots, q.
$$

根$\theta_i$是$> 0$，成对不同，$w(\theta_i) < 0$，并且每个根$\alpha > 0$使得$w(\alpha) < 0$等于$\theta_i$之一。

令X为$\alpha > 0$的集合，使得$w(\alpha) < 0$。通过（二），

$$
\operatorname{Card}(X) = \operatorname{Card}(T_{w^{-1}}) = l(w^{-1}) = l(w) = q.
$$

另一方面，如果 $\alpha \in X$ 显然存在 $i \in \{1, q\}$ 使得

$$
s_{i+1} \ldots s_q(\alpha) > 0 \quad \text{and} \quad s_i s_{i+1} \ldots s_q(\alpha) < 0.
$$

由科. 1，这意味着$s_{i+1} \ldots s_q(\alpha) = \alpha_i$，因此也意味着$\alpha = \theta_i$。因此，集合X包含在$\theta_i$的集合中。由于$\operatorname{Card}(X) = q$，只有当X等于$\theta_i$的集合并且它们是成对不同的时，这才是可能的。由此得出推论。

#### 推论 3 {#lie-vi-s1-prop-17-cor-3 .statement tag=0AVE}

*假设R减小。 W中存在唯一的最长元素$w_0$，其长度等于正根和$w_0$变换室C至$-C$的数。我们为所有 $w \in W$ 提供了 $w_0^2 = 1$ 和 $l(ww_0) = l(w_0) - l(w)$。*

显然$-C$是一个房间。因此W存在元素$w_0$即变换C到$-C$。然后$w_0(\alpha) < 0$对于所有正根$\alpha$和Cor的前两个断言。 3 是 Cor 的直接的推论。 2. 我们有$w_0^2(C) = C$，所以$w_0^2 = 1$。最后，如果 $w \in W$、长度 $l(w)$（或 $l(ww_0)$）根据第 17 (iii) 条等于分隔 C 和 $w(C)$（或 $ww_0(C) = -w(C)$）的墙壁的数。由于$w(C)$和$-w(C)$位于每面墙的相对两侧，和$l(w) + l(w_0)$等于墙的总数，即$l(w_0)$。

#### 命题 18 {#lie-vi-s1-prop-18 .statement tag=0AVF}

*让$x \in V$。以下三个属性是等效的：

(i) $x \in \overline{C}$；
(ii) $x \geq s_\alpha(x)$ 对于所有$\alpha \in B(C)$（相对于C 定义的序关系）；
(iii) $x \geq w(x)$ 对于所有 $w \in W$。

由于$s_\alpha(x) = x - \langle x, \alpha^\vee \rangle \alpha$和$\overline{C}$是元素$x \in V$的集合，使得$\langle x, \alpha^\vee \rangle \geq 0$对于所有$\alpha \in B(C)$，(i)和(ii)的等价是明显的。另一方面，显然 (iii) $\Longrightarrow$ (ii)。我们证明 (i) $\Longrightarrow$ (iii)。设$x \in \overline{C}$，并设$w \in W$。我们以$w$的长度$l(w)$为归纳争论。案例$l(w) = 0$很简单。如果$l(w) \geq 1$，$w$可以写成形式$w = w' s_\alpha$，还有$\alpha \in B(C)$和$l(w') = l(w) - 1$。然后

$$
x - w(x) = x - w'(x) + w'(x - s_\alpha(x)).
$$

归纳假设表明$x - w'(x)$为正。另一方面，

$$
w'(x - s_\alpha(x)) = w(s_\alpha(x) - x) = -\langle x, \alpha^\vee \rangle w(\alpha).
$$

现在$s_\alpha \in T_{w^{-1}}$，而第 17 号提案 (ii) 表明$w(\alpha) < 0$。于是就有了这样的结果。

#### 推论{#lie-vi-s1-n6-cor-2 .statement tag=0AVG}

元素$x \in C$当且仅当$x > w(x)$对于所有$w \in W$使得$w \neq 1$。

#### 命题 19 {#lie-vi-s1-prop-19 .statement tag=0AVH}

对于室 $C$，令 $(\beta_i)_{1 \leq i \leq n}$ 为正根的序列，使得 $\beta_1 + \beta_2 + \cdots + \beta_n$ 为根。那么存在置换 $\pi \in S_n$，对于所有 $i \in \{1, 2, \ldots, n\}$，$\beta_{\pi(1)} + \beta_{\pi(2)} + \cdots + \beta_{\pi(i)}$ 是根。

我们通过归纳对$n$进行论证，命题对于$n \leq 2$来说是明确的。把$\beta = \beta_1 + \cdots + \beta_n$。那么$\sum_{i=1}^n (\beta|\beta_i) = (\beta|\beta) > 0$，所以存在指标$k$使得$(\beta|\beta_k) > 0$。如果 $\beta = \beta_k$，则从 $\beta_i > 0$ 开始，$n = 1$ 对于所有 $i$。否则$\beta - \beta_k$是根（no. 3，Th.1的Cor.）；然后将归纳假设应用于 $\beta - \beta_k = \sum_{i \neq k} \beta_i$ 即可。

#### 推论 1 {#lie-vi-s1-prop-19-cor-1 .statement tag=0AVI}

让$\alpha \in R_+(C)$。那么$\alpha \in B(C)$当且仅当$\alpha$是两个正根中的和。

如果$\alpha$是两个正根中的和，则Th。 3表明$\alpha \in B(C)$。如果$\alpha \notin B(C)$，Th。图3显示对于所有$k$和$n \geq 2$，$\alpha = \sum_{k=1}^n \beta_k$和$\beta_k \in B(C)$。

如有必要，对$\beta_k$进行排列，我们可以假设$\sum_{k=1}^{n-1}$是根（命题19），因此$\alpha$是正根$\sum_{k=1}^{n-1} \beta_k$和$\beta_n$的和。

#### 推论 2 {#lie-vi-s1-prop-19-cor-2 .statement tag=0AVJ}

设$\varphi$为映射，从$R$到阿贝尔的群$\Gamma$，具有以下性质：

1) $\varphi(-\alpha) = -\varphi(\alpha)$ 换 $\alpha \in R$；
2) 如果$\alpha \in R, \beta \in R$使得$\alpha + \beta \in R$，则$\varphi(\alpha + \beta) = \varphi(\alpha) + \varphi(\beta)$。

令$Q$为由$R$生成的$V$的子群。然后从$Q$到$\Gamma$，$\varphi$扩展到同态。

设$B$为$R$的基。令$\psi$为从$Q$到$\Gamma$的唯一同态，即重合，$\varphi$位于$B$。只要证明当$\alpha$相对于$B$是正根时，$\psi(\alpha) = \varphi(\alpha)$就足够了。我们有 $\alpha = \beta_1 + \cdots + \beta_m$ 和 $\beta_i \in B$ 代表所有 $i$，$\beta_1 + \cdots + \beta_h \in R$ 代表所有 $h$（提案 19）。我们在 $m$ 上通过归纳显示$\psi(\alpha) = \varphi(\alpha)$。如果 $m = 1$ 就很清楚了。 归纳假设给出

$$
\psi(\beta_1 + \cdots + \beta_{m-1}) = \varphi(\beta_1 + \cdots + \beta_{m-1}),
$$

我们有$\psi(\beta_m) = \varphi(\beta_m)$，因此有$\psi(\alpha) = \varphi(\alpha)$，这证明了推论。

对于$R$中的任何根$\alpha = \sum_{\beta \in B(C)} n_\beta \beta$，用$\beta \in B(C)$的$Y(\alpha)$集合表示，使得$n_\beta \neq 0$。此外，观察到$B(C)$可以与由$W(R)$和$s_{\alpha_i}$形成的Coxeter系统图的顶点集合识别（cf.第IV, § 1, no. 9章和第V, § 3, no. 2章）。

#### 推论 3 {#lie-vi-s1-prop-19-cor-3 .statement tag=0AVK}

a) 设 $\alpha \in \mathbf{R}$。那么$Y(\alpha)$是$B(C)$的连通的子集（第IV，附录）。

b) 令$Y$为$B(C)$的非空连通子集。然后$\sum_{\beta \in Y} \beta$属于到$\mathbf{R}$。

为了证明a)，我们可以假设$\alpha$是正数。我们通过归纳对$\mathrm{Card}(Y(\alpha))$进行论证，如果$\mathrm{Card}(Y(\alpha)) = 1$则断言微不足道。根据第 19 条命题，存在 $\beta \in B(C)$ 使得 $\alpha - \beta \in \mathbf{R}$。令$p$为最大的整数$\geqslant 0$，使得$\gamma = \alpha - p\beta \in \mathbf{R}$。从$\gamma - \beta \notin \mathbf{R}$和$\gamma + p\beta \in \mathbf{R}$开始，$(\gamma|\beta) \neq 0$（提案9）；因此$\beta$与$Y(\gamma)$中的至少一个元素相关联。但是$Y(\alpha) = Y(\gamma) \cup \{\beta\}$和$Y(\gamma)$是通过归纳假设连接的。因此$Y(\alpha)$是连通的，这就证明了a)。

现在令$Y$为$B(C)$的非空连通子集；我们通过$\mathrm{Card}(Y)$上的归纳证明$\sum_{\beta \in Y} \beta$是根。 $\mathrm{Card}(Y) \leqslant 1$ 是微不足道的情况。假设$\mathrm{Card}(Y) \geqslant 2$。由于 $X$ 是一片森林（第 V, § 4, no. 8 章，第 8 章），$Y$ 是一棵树，并且有一个终端顶点 $\beta$（第 IV 章，附录）。 集合$Y - \{\beta\}$相连，其中一个元素与$\beta$相连。到归纳假设、$\alpha = \sum_{\gamma \in Y - \{\beta\}} \gamma \in \mathbf{R}$，从$(\alpha|\beta) < 0$开始，得出$\alpha + \beta \in \mathbf{R}$（Th.1）。 Q.E.D.

### 7. 集合根关闭

#### 定义 4 {#lie-vi-s1-def-4 .statement tag=0AVL}

令 $P$ 为 $\mathbf{R}$ 中的子集。

(i) 如果条件 $\alpha \in P, \beta \in P, \alpha + \beta \in \mathbf{R}$ 暗示 $\alpha + \beta \in P$，则称$P$ 是封闭的。

(ii) 如果 $P$ 闭合且$P \cup (-P) = \mathbf{R}$，则$P$ 被称为抛物线。

(iii) 如果 $P = -P$，则称 $P$ 是对称的。

#### 引理 3 {#lie-vi-s1-lem-3 .statement tag=0AVM}

令$C$为$\mathbf{R}$和$P$的腔室，以及$\mathbf{R}$包含$R_+(C)$的封闭子集（在no. 6的记号中）。设$\Sigma = B(C) \cap (-P)$，并设$Q$为根集合，即$\Sigma$元素线性组合，系数为非正整数。然后，$P = R_+(C) \cup Q$。

只要证明$P \cap (-R_+(C)) = Q$就足够了。 让$-\alpha \in Q$。 那么$\alpha$就是$n$元素的$\Sigma$的和。 我们通过归纳在$n$上展示$-\alpha \in P$。 如果$n = 1$，这很清楚。 If $n > 1$, then by Prop. 19 of no. 6 we can write $\alpha = \beta + \gamma$ with $\gamma \in \Sigma$ and $\beta$ the sum of $n - 1$ elements of $\Sigma$. 归纳假设、$-\beta \in P$；由于 $-\gamma \in P$ 且由于 $P$ 已关闭，$-\alpha \in P$。 因此，$Q \subseteq P \cap (-R_+(C))$。 相反，设$-\alpha \in P \cap (-R_+(C))$。 那么$\alpha$就是$p$元素的$B(C)$的和。 我们通过归纳在$p$上展示$-\alpha \in Q$。 如果$p = 1$，这很清楚。 如果$p > 1$，那么根据命题19，我们可以用$\gamma \in B(C)$和$\beta$根来写$\alpha = \beta + \gamma$，即$p - 1$元素和$B(C)$。 由于 $-\gamma = \beta + (-\alpha)$ 和 $P$ 是闭合的，$-\gamma \in P$，因此$\gamma \in \Sigma$。 此外，由于$P$是封闭的，$-\beta = \gamma + (-\alpha)$所以$-\beta \in P$。 由归纳假设，$-\beta \in Q$，所以$-\alpha = -\beta - \gamma \in Q$。 因此，$P \cap (-R_+(C)) \subseteq Q$。

#### 命题 20 {#lie-vi-s1-prop-20 .statement tag=0AVN}

*设$P$为$R$的子集。以下条件是等效的*：

(i) $P$ *是抛物线*；
(ii) $P$ * 关闭，并且存在 $R$ 的室 $C$，使得 $P \supseteq R_+(C)$*；
(iii) *存在$R$的$C$和$B(C)$的子集$\Sigma$，使得$P$是$R_+(C)$的并和集合$Q$的根是线性组合元素 $\Sigma$ 具有非正整数系数*。

(ii) $\Longrightarrow$ (iii)：这是从引理 3 得出的。

(iii)$\Longrightarrow$(i)：我们采用(iii)的假设和记号。显然$P \cup (-P) = R$。我们证明，如果 $\alpha, \beta \in P$ 满足 $\alpha + \beta \in R$，则$\alpha + \beta \in P$。如果根 $\alpha + \beta$ 为正，这一点很明显。假设$\alpha + \beta$为负。然后是$\alpha + \beta = \sum_{\gamma \in B(C)} n_\gamma \gamma$，还有$n_\gamma \leq 0$。但$\alpha$或$\beta$中$B(C) - \Sigma$的每一个元素$\gamma$的系数为$\geq 0$；因而$n_\gamma = 0$如果$\gamma \in B(C) - \Sigma$，那么$\alpha + \beta \in Q \subseteq P$。

(i) $\Longrightarrow$ (ii)：假设$P$ 是抛物线。令 $C$ 为一个室，使得 $\mathrm{Card}(P \cap R_+(C))$ 尽可能大。设$\alpha \in B(C)$并假设$\alpha \in P$，从而得到$-\alpha \in P$。对于所有 $\beta \in P \cap R_+(C)$，$\beta$ 与 $\alpha$ 不成比例（对于假设 $\beta = 2\alpha$ 意味着 $\alpha = 2\alpha + (-\alpha) \in P$，因为 $P$ 是封闭的）。因而$s_\alpha(\beta) \in R_+(C)$（no. 6，第 17 号提案第 1 条）。如果我们放入$C' = s_\alpha(C)$，则$\beta = s_\alpha(s_\alpha(\beta)) \in s_\alpha(R_+(C)) = R_+(C)$，$-\alpha \in P \cap R_+(C')$，因而$\mathrm{Card}(P \cap R_+(C')) > \mathrm{Card}(P \cap R_+(C))$。这是荒谬的，从$\alpha \in P$开始。因而，$B(C) \subseteq P$，以及根据第 19 号命题的$R_+(C) \subseteq P$，以及$P$ 是封闭的事实。

#### 推论 1 {#lie-vi-s1-prop-20-cor-1 .statement tag=0AVO}

*令$P$为$R$中的子集。以下条件是等效的*：

(i) *存在一个室$C$使得$P = R_+(C)$*；
(ii) *$P$ 关闭且 $\{P, -P\}$ 为 $R$* 中的划分。

*腔室$C$使得$P = R_+(C)$是唯一的*。

如果$P = R_+(C)$，$C$是$x^* \in V^*$的集合，这样$\langle x^*, x \rangle > 0$对于所有$x \in P$，因此唯一性等于$C$。

#### 推论 2 {#lie-vi-s1-prop-20-cor-2 .statement tag=0AVP}

*假设$V$配备了有序向量空间的结构，使得对于这个结构，$R$的每个根不是正就是负。对于这个结构，令 $P$ 为正根的集合。那么存在一个独特的室$C$ $R$ 使得$P = R_+(C)$*。

事实上，$P$满足Cor的条件(ii)。 1.

这个推论特别适用于当考虑的阶是总计时，条件在$R$上然后自动满足。 Recall that such an order can be obtained, for example, by choosing a basis $(e_i)_{1 \leq i \leq n}$ of $V$ and taking the lexicographic order on $V$, so $x = \sum_i \xi_i e_i$ is $\geq 0$ if all the $\xi_i$ are 0, or if $\xi_i > 0$ for the smallest index $i$ such that $\xi_i \neq 0$.

#### 推论 3 {#lie-vi-s1-prop-20-cor-3 .statement tag=0AVQ}

*R 的子集 B 是 R 的基当且仅当满足以下条件：*

(i) *B 的元素线性无关；*
(ii) *R 的每个根都是 B 的元素的线性组合，其中系数要么全正，要么全负；*
(iii) *B 的每个根都是不可分的。*

我们已经知道条件是必要的（no. 5，Th.2，和no. 6，Th.3）。假设满足条件 (i), (ii), (iii)。令 P 为根的集合，即 B 的元素的线性组合，系数为 $\geq 0$。由于P满足Cor的条件(ii)。 1、存在C使得$P = R_+(C)$；设$B' = B(C)$，X和$X'$是B和$B'$生成的凸锥。然后

$$
B \subseteq P \subseteq X \quad \text{and} \quad B' \subseteq P \subseteq X',
$$

这表明X和$X'$都是由P生成的，因此重合。但是 B 的元素（或$B'$）生成的半线是X（或$X'$）的极端生成元；因为这样的半线包含只有一个不可分割的根、$B = B'$。

#### 推论 4 {#lie-vi-s1-prop-20-cor-4 .statement tag=0AVR}

*设B为R的基、B的$B'$子集、$B'$生成的V的$V'$向量子空间和$R' = R \cap V'$。那么$B'$就是根系$B'$中的基。*

这立即来自Cor。 3 和科。提案 4。

我们称$R'$根系*由$B'$*生成*。

#### 推论 5 {#lie-vi-s1-prop-20-cor-5 .statement tag=0AVS}

*设 B 为 R 的基，B 的$A_1, A_2, \ldots, A_r$ 成对正交子集，以及$A = A_1 \cup A_2 \cup \cdots \cup A_r$。那么A的每一个元素线性组合即根$\alpha$实际上是$A_i$之一的元素线性组合。特别是，如果 R 是不可约的，则 B 的划分不存在成对正交子集。*

令$E_1, \ldots, E_r, E$分别为$A_1, \ldots, A_r, A$生成的V的向量子空间。由科. 4、我们可以假设$E = V$。然后，由 Th. no. 5的2(vii)，$E_i$在$W(R)$下是稳定的，所以R是$R \cap E_i$的并（no. 2，命题5）。

#### 推论 6 {#lie-vi-s1-prop-20-cor-6 .statement tag=0AVT}

*我们采用命题20的假设和记号。令$V_1$为由$\Sigma$生成的V的向量子空间。那么 $P \cap (-P) = Q \cup (-Q) = V_1 \cap R$ 就是 $V_1$ 中的根系和基 $\Sigma$。*

我们有$P \cap (-P) = (R_+(C) \cup Q) \cap ((-R_+(C)) \cup (-Q)) = Q \cup (-Q)$。 Th。 3证明$Q \cup (-Q) = V_1 \cap R$。最后，Cor. 的$\Sigma$ 是根系 $V_1 \cap R$ 的基。 4.

#### 命题 21 {#lie-vi-s1-prop-21 .statement tag=0AVU}

*令C（分别$C'$）为R室，$\Sigma$（分别$\Sigma'$）子集为$B(C)$（分别为$B(C')$），Q（分别为$Q'$）集合为线性组合 $\Sigma$（或$\Sigma'$）的元素，具有负整数系数，以及$P = Q \cup R_+(C)$（或$P' = Q' \cup R_+(C')$）。如果存在Weyl 群将P变换为$P'$的元素，则存在Weyl 群将C变换为$C'$和$\Sigma$变换为$\Sigma'$的元素。

我们约化立即处理案件$P = P'$。令$V_1$为由$P \cap (-P)$生成的V的向量子空间。那么$\Sigma$和$\Sigma'$就是$V_1$中根系$R_1 = P \cap (-P)$的基（第20号提案第6条）。因此存在$g_1 \in W(R_1)$使得$g_1(\Sigma) = \Sigma'$。很明显，$g_1$是由$W(R)$的元素$g$引发的，即$s_\sigma$与$\sigma \in \Sigma$对称性的乘积。设$\gamma = \sum_{\beta \in B(C)} c_\beta \beta$为$P - R_1$中的元素。然后$c_\beta > 0$至少有一个$\beta \in B(C) - \Sigma$。此外，如果$\sigma \in \Sigma$，则$s_\sigma(\gamma) - \gamma \in V_1$，因此$s_\sigma(\gamma)$相对于$B(C)$至少有一个坐标$> 0$（no. 1，公式（5）），因此$s_\sigma(\gamma) \in R_+(C)$，最后$s_\sigma(\gamma) \in P - R_1$。由此可见，$P - R_1$ 在 $s_\sigma, \sigma \in \Sigma$ 下稳定，因此在 $g$ 下稳定，因此 $g(P) = P$。因此，当 $P = P'$ 和 $\Sigma = \Sigma'$ 时，我们就减少到证明命题。在这种情况下，$Q = Q'$，因此$R_+(C) = P - Q = P - Q' = R_+(C')$，因此$C = C'$（第20号提案的Cor.1）。

#### 推论{#lie-vi-s1-n7-cor-1 .statement tag=0AVV}

*令P、$P'$为R的两个抛物线子集通过Weyl群的元素相互转化。如果存在 R 的室C，使得 $R_+(C) \subseteq P$ 和 $R_+(C) \subseteq P'$，则$P = P'$。

这是从引理 3和第21条命题得出的，因为$W(R)$将C变换到C的唯一元素是1，cf.no. 5，Th。 2.

#### 命题 22 {#lie-vi-s1-prop-22 .statement tag=0AVW}

*令 P 为 R 的闭子集，使得 $P \cap (-P) = \varnothing$。那么存在 R 的室C使得$P \subseteq R_+(C)$。

1）鉴于Cor。的 Th。 1、no. 3、假设$\alpha \in P, \beta \in P, (\alpha|\beta) < 0$暗示$\alpha + \beta \in P$。

2）我们证明P的元素中没有和$\alpha_1 + \cdots + \alpha_q$（$q \geqslant 1$）是零。我们于 $q$ 沿归纳出发。 断言对于$q = 1$来说是清楚的，假设$q \geqslant 2$。如果$\alpha_1 + \cdots + \alpha_q = 0$，那么

$$
-\alpha_1 = \alpha_2 + \cdots + \alpha_q,
$$

所以$(-\alpha_1|\alpha_2 + \cdots + \alpha_q) > 0$，因此存在$j \in \{2, q\}$使得$(\alpha_1|\alpha_j) < 0$。由证明、$\alpha_1 + \alpha_j \in P$和关系$(\alpha_1 + \alpha_j) + \sum_{i \neq 1, j} \alpha_i = 0$与……矛盾归纳假设中的部分1)。

3) 我们证明$V$中存在非零元素$\gamma$，使得$(\gamma|\alpha) \geqslant 0$对于所有$\alpha \in P$。如果不是，1) 的结果将表明可以找到元素的 $P$ 的无限序列 $\alpha_1, \alpha_2, \ldots$ 使得
$$
\beta_i = \alpha_1 + \cdots + \alpha_i \in P
$$
对于所有$i$；将存在两个不同整数$i, j$使得$\beta_i = \beta_j$，这与2)的结果相矛盾。

4）为了证明命题，只要证明$V$存在基$(\alpha_k)_{1 \leq k \leq l}$就足够了（第20条的Cor.2），这样，对于由这个基定义的词典阶，$P$的每个元素是$> 0$。我们在$l = \dim V$上继续归纳，并假设命题对于所有维数$< l$成立。对于所有 $\alpha \in P$ (cf. 3))，令 $\gamma \in V$ 满足 $\gamma \neq 0$ 和 $(\gamma|\alpha) \geqslant 0$。令$L$为与$\gamma$正交的超平面，以及由$R \cap L$生成的$L$的$V'$子空间。那么$R \cap L$在$V'$中是根系，并且$P \cap L$在$R \cap L$中闭合。通过归纳假设，存在$V'$的基$(\beta_1, \ldots, \beta_{l'})$，使得$P \cap L$的元素对于由此基定义的词典阶来说是$> 0$。那么 $V$ 中的任何基 ，其前一个 $l' + 1$ 元素是 $\gamma, \beta_1, \ldots, \beta_{l'}$ ，并且其剩余的元素在 $L$ 中，则具有所需的性质 。

#### 命题 23 {#lie-vi-s1-prop-23 .statement tag=0AVX}

*令$P$为$R$的子集和由$P$生成的$V$的$V_1$（分别为$\Gamma$）向量子空间（分别为子群）。以下条件是等效的：*

(i) *P 是封闭且对称的；*
(ii) *P 是闭集，且 P 在 $V_1$ 中为根系；*
（三）$\Gamma \cap R = P$。

*假设满足这些条件。对于任何$\alpha \in P$，令$\alpha_1 \tilde{}$为$\alpha \tilde{}$到$V_1$中的限制。那么映射 $\alpha \mapsto \alpha_1 \tilde{}$ 就是从根系 $P$ 到 $P \tilde{}$ 的规范双射。*

(iii) $\Longrightarrow$ (i)：清楚。

(i) $\Longrightarrow$ (ii)：假设$P$ 是封闭且对称的。首先，$P$在$V_1$中满足(RS_I)。我们证明，如果$\alpha, \beta \in P$，则$s_\alpha(\beta) \in P$。如果 $\alpha$ 和 $\beta$ 成比例，这一点就很清楚了。否则，$s_\alpha(\beta) = \beta - n(\beta, \alpha)\alpha$ 和 $\beta - p\alpha \in R$ 对于 0 到 $n(\beta, \alpha)$ 之间的所有有理数整数 $p$（第 9 条，no. 3），所以
$$
\beta - n(\beta, \alpha)\alpha \in P
$$
因为 $P$ 是封闭且对称的。因此，$s_{\alpha, \alpha_1}(P) = P$和$P$满足(RS_{II})。显然$P$满足(RS_{III})。这样，$P$满足(ii)，同时我们也证明了命题的最后一个断言。

(ii) $\Longrightarrow$ (iii)：我们证明，如果条件 (ii) 满足，则$\Gamma \cap R = P$。显然$P \subseteq \Gamma \cap R$。让$\beta \in \Gamma \cap R$。从$\beta \in \Gamma$和$P = -P$开始，$\beta = \alpha_1 + \alpha_2 + \cdots + \alpha_k$和$\alpha_1, \ldots, \alpha_k \in P$。我们将证明$\beta \in P$。如果$k = 1$，这很清楚。我们在归纳对$k$争论。我们有

$$
0 < (\beta|\beta) = \sum_{i=1}^{k} (\beta|\alpha_i),
$$
所以$(\beta|\alpha_i) > 0$对于一些指标$i$。如果$\beta = \alpha_i$，则$\beta \in P$。否则，$\beta - \alpha_i \in R$（Th.1的Cor.，no. 3），因此$\beta - \alpha_i \in P$乘以归纳假设，因此$\beta \in P$，因为$P$是封闭的。

23号提案的条件可以用$V_1 = V$和$P \neq R$来实现。对于例，当$R$是型$G_2$中的系统和型$A_2$中的$P$系统时就是这种情况； cf. 板X。

#### 命题 24 {#lie-vi-s1-prop-24 .statement tag=0AVY}

*设$R'$为$R$的交，向量子空间为$V$，则$R'$为向量子空间$V'$中的根系，则生成（cf. Prop. 4，no. 1）。令 $B'$ 为 $R'$ 中的基。*

(i) *存在$R$包含$B'$中的基。*
(ii) *$R'$是$R$元素集合即$B'$元素线性组合。*

断言 (ii) 很清楚。我们证明（i）。令 $(\varepsilon_1, \varepsilon_2, \ldots, \varepsilon_l)$ 为 $V$ 的基，使得 $B' = (\varepsilon_{p+1}, \varepsilon_{p+2}, \ldots, \varepsilon_l)$。 $V$相应的上的字典阶到基定义$C$$R$。显然，$B'$中的每个元素在$R_+(C)$中都是最小的。因此$B' \subseteq B(C)$。

### 8.最高根

#### 命题 25 {#lie-vi-s1-prop-25 .statement tag=0AVZ}

*假设$R$是不可约的。令$C$为$R$的腔室，并令$B(C) = \{\alpha_1, \ldots, \alpha_l\}$为相应的基。*

(i) *存在根 $\tilde{\alpha} = \sum_{i=1}^{l} n_i \alpha_i$，因此对于每个根 $\sum_{i=1}^{l} p_i \alpha_i$，我们有 $n_1 \geq p_1, n_2 \geq p_2, \ldots, n_l \geq p_l$。在其他字中，$R$ 对于 $C$ 定义的排序有最大的元素。*
(ii) *我们有$\tilde{\alpha} \in \overline{C}$。*
(iii) *每根 $\alpha$ 就有 $(\tilde{\alpha}|\tilde{\alpha}) \geq (\alpha|\alpha)$。*
(iv) *对于每个与 $\tilde{\alpha}$ 不成正比的正数根 $\alpha'$，我们有 $n(\alpha', \tilde{\alpha}) = 0$ 或 $1$。*

1) 令 $\alpha = \sum_{i=1}^{l} n_i \alpha_i$、$\beta = \sum_{i=1}^{l} p_i \alpha_i$ 为$C$ 定义的排序的两个最大根。我们将证明$\alpha = \beta$，从而成立(i)。

2) 如果$(\alpha|\alpha_i) < 0$对于某些指标$i$，则可以得出$\alpha + \alpha_i \in R$或$\alpha = -\alpha_i$（Th.1的Cor.，no. 3），并且两种可能性对于$\alpha$的极大值来说都是荒谬的。因此 $(\alpha|\alpha_i) \geq 0$ 对于所有$i$。

3）如果$\alpha < 0$，那么$\alpha < -\alpha$，这是荒谬的。因此 $n_i \geq 0$ 对于所有 $i$。令$J$为$i$的集合，使得$n_i > 0$，且$J'$为$\{1, 2, \ldots, l\}$中$J$的补集。然后$J \neq \varnothing$。如果$J'$非空，则存在$i \in J$和$i' \in J'$，使得$(\alpha_i|\alpha_{i'}) < 0$（第20号提案第5条，no. 7）；那么我们就会有

$$(\alpha | \alpha_{i'}) = \sum_{i \in I} n_i (\alpha_i | \alpha_{i'}) < 0$$

因为只要 $j$ 和 $k$ 不同，$(\alpha_j | \alpha_k) \leq 0$ 就成立，这与 2) 相矛盾。因此对于所有 $i$ 都有 $J' = \varnothing$ 和 $n_i > 0$。

4) 对于所有$i$，我们有$(\beta | \alpha_i) \geq 0$乘以2)。自$\beta \neq 0$以来，我们不能为所有$i$提供了$(\beta | \alpha_i) = 0$。我们从 3) 推断出

$$(\beta | \alpha) = \sum_i n_i (\beta | \alpha_i) > 0.$$

如果$\gamma = \alpha - \beta \in \mathbf{R}$，则$\alpha > \beta$或$\beta > \alpha$（Th.3，no. 6），其中与……矛盾是$\alpha$和$\beta$的最大值。因此$\alpha = \beta$（Cor. of Th.1，no. 3）。

5) 到 2)，$\tilde{\alpha} \in \overline{C}$。我们将证明每$\alpha' \in \mathbf{R}$都有$(\alpha' | \alpha') \leq (\tilde{\alpha} | \tilde{\alpha})$。由于$\overline{C}$是$W(\mathbf{R})$的基本域，我们可以假设$\alpha' \in \overline{C}$。我们有 $\tilde{\alpha} - \alpha' \geq 0$，因此所有 $x \in \overline{C}$ 都有 $(\tilde{\alpha} - \alpha' | x) \geq 0$。特别是$(\tilde{\alpha} - \alpha' | \tilde{\alpha}) \geq 0$和$(\tilde{\alpha} - \alpha' | \alpha') \geq 0$，因此是$(\tilde{\alpha} | \tilde{\alpha}) \geq (\alpha' | \tilde{\alpha}) \geq (\alpha' | \alpha')$。因此，如果 $\alpha'$ 与 $\tilde{\alpha}$ 不成比例，$n(\alpha', \tilde{\alpha})$ 必须等于 0、1 或 -1。如果 $\alpha' \geq 0$，则 $(\tilde{\alpha} | \alpha') \geq 0$ 除以 2)，因此 $n(\alpha', \tilde{\alpha}) \geq 0$ 和 $n(\alpha', \tilde{\alpha})$ 必须为 0 或 1。

#### 注 {#lie-vi-s1-n8-rem-1 .statement tag=0AW0}

根

$$\tilde{\alpha} = \sum_i n_i \alpha_i$$

(i)中据说是$\mathbf{R}$的最高根（相对于$C$）。 注，通过 (i)，我们对所有 $i$ 都有 $n_i \geq 1$。

### 9.权，激进权

让$l = \dim V$。用$\mathbf{R}$生成的$V$的$Q(\mathbf{R})$子群表示； $Q(\mathbf{R})$的元素称为$\mathbf{R}$的部首权。由 Th. no. 6、$Q(\mathbf{R})$的3个是秩$l$的$V$的离散子群，$\mathbf{R}$的每一个基是$Q(\mathbf{R})$的基。

类似地，群$Q(\mathbf{R}^*)$是秩$l$的$V^*$的离散子群。

#### 命题 26 {#lie-vi-s1-prop-26 .statement tag=0AW1}

*$x \in V$的集合，使得对于所有$y^* \in Q(\mathbf{R}^*)$（或者等效地，对于所有$y^* \in \mathbf{R}^*$），$\langle x, y^* \rangle \in \mathbf{Z}$是$V$包含$Q(\mathbf{R})$的离散子群$G$。如果$B'$是$\mathbf{R}^*$的基，$V$的基对$B'$的对数就是$G$*的基。

让$x \in V$。以下三个属性是等效的：

(i) $\langle x, y^* \rangle \in \mathbf{Z}$ 对于所有 $y^* \in Q(\mathbf{R}^*)$；
(ii) $\langle x, y^* \rangle \in \mathbf{Z}$ 为所有 $y^* \in B'$；
(iii) $x$相对于$B'$的对偶基的坐标在$\mathbf{Z}$中。

由此我们推断，基对偶于$B'$是基除以$G$。另一方面，(RSIII)证明$\mathbf{R} \subseteq G$，因此$Q(\mathbf{R}) \subseteq G$。

26号提案的群$G$记为$P(\mathbf{R})$，其元素称为$\mathbf{R}$的权。我们还可以考虑$\mathbf{R}^*$的权中的群$P(\mathbf{R}^*)$。

$$
P(R)/Q(R), \quad P(\tilde{R})/Q(\tilde{R})
$$

有限群在 $\mathbf{Q}/\mathbf{Z}$ 上具有对偶性，因此是同构的。这两个群的公共的阶称为R（或$\tilde{R}$）的*连接指标*。

如果 R 是根系 $R_i$ 中的直和，则群 Q(R)（分别为 P(R)）可与 Q($R_i$)（分别为 P($R_i$)）中的直和规范地识别。

#### 命题 27 {#lie-vi-s1-prop-27 .statement tag=0AW2}

*令$R_1$为R的子集，由$R_1$生成的Q(R)的$Q_1$子群，以及由$s_\alpha$($\alpha \in R_1$)生成的W(R)的$W_1$子群。如果 $p \in P(R)$ 和 $w \in W_1$，则 $p - w(p) \in Q_1$。*

如果 $w = s_\alpha$ 与 $\alpha \in R_1$，则

$$
p - w(p) = \langle p, \alpha^\vee \rangle \alpha \in \mathbf{Z}\alpha \subseteq Q_1.
$$

如果$w = s_{\alpha_1} s_{\alpha_2} \ldots s_{\alpha_r}$和$\alpha_1, \ldots, \alpha_r \in R_1$，$p - w(p) \in Q_1$仍然成立，正如我们在r上通过归纳看到的那样。

群 A(R) 使 P(R) 和 Q(R) 保持不变，因此作用于商 P(R)/Q(R)。根据第 27 条命题，群 W(R) 对 P(R)/Q(R) 的作用微不足道。 经过到商，我们看到 *商群* A(R)/W(R)（cf. 命题 16，no. 5）*规范地作用于* P(R)/Q(R)。

### 10. 基本权，主导权

假设 R 被*减少*。令C为R的一个室，并令B为R的相应的基。由于R被减少，$B^\vee = \{ \alpha^\vee \}_{\alpha \in B}$为$R^\vee$的基。因此，$B^\vee$的*对偶基*$(\overline{\omega}_\alpha)_{\alpha \in B}$是权的群的基；它的元素被称为*基本权*（相对于B，或C）；如果B的元素用$(\alpha_1, \ldots, \alpha_l)$表示，则相应的基本权用$(\overline{\omega}_1, \ldots, \overline{\omega}_l)$表示。

让$x \in V$。那么，$x \in C$当且仅当$\langle x, \alpha^\vee \rangle > 0$对于所有$\alpha \in B$。由此可见，C 是系数为$\geq 0$ 的$\overline{\omega}_\alpha$ 的线性组合的集合。

对于固定的$\alpha$，嘉当矩阵的条目$n(\alpha, \beta) = \langle \alpha, \beta^\vee \rangle$是$\alpha$相对于基$(\overline{\omega}_\beta)_{\beta \in B}$的坐标：

$$
\alpha = \sum_{\beta \in B} n(\alpha, \beta) \overline{\omega}_\beta.
$$

因此嘉当矩阵是转置矩阵典范嵌入

$$
Q(R) \to P(R)
$$

关于$\mathbf{Z}$-模块Q(R)和P(R)的基B和$(\overline{\omega}_\alpha)_{\alpha \in B}$。

如果权 $\overline{\omega}$ 被认为是*主导*，如果它属于到 $\overline{C}$，在其他字，如果它相对于 $(\overline{\omega}_\alpha)_{\alpha \in B}$ 的坐标是整数 $\geq 0$，或者等效地，如果$g(\overline{\omega}) \leq \overline{\omega}$ 对于所有$g \in W(R)$（no. 6，提案 18）。由于$\overline{C}$是$W(R)$（Th.2）的基本域，因此对于任何权$\overline{\omega}$，都存在唯一的权$\overline{\omega}'$，使得$\overline{\omega}'$是$\overline{\omega}$除$W(R)$的变换。

我们有
$$
\langle \overline{\omega}_\alpha, \beta^\vee \rangle = (\overline{\omega}_\alpha | \frac{2\beta}{(\beta|\beta)}) = \delta_{\alpha\beta}
$$
对于$\alpha, \beta \in B$（$\delta_{\alpha\beta}$表示克罗内克符号），因此
$$
s_\beta(\overline{\omega}_\alpha) = \overline{\omega}_\alpha - \delta_{\alpha\beta}\beta \quad \text{and} \quad (\overline{\omega}_\alpha |\beta) = \frac{1}{2}(\beta|\beta)\delta_{\alpha\beta}.
$$
在其他字中，$\overline{\omega}_\alpha$ *与* $\beta$ *正交，对于* $\beta \neq \alpha$，*其正交投影到* $R\alpha$ *是* $\frac{1}{2}\alpha$。由于$\overline{\omega}_\alpha \in \overline{C}$，$(\overline{\omega}_\alpha |\overline{\omega}_\beta) \geqslant 0$为$\alpha, \beta \in B$，即角$(\overline{\omega}_\alpha, \overline{\omega}_\beta)$是锐角或直角。占主导地位的权是 $\overline{\omega} \in V$，因此对于所有 $\alpha \in B$，$2(\overline{\omega}|\alpha)/(|\alpha|\alpha)$ 是整数 $\geqslant 0$。

#### 命题 28 {#lie-vi-s1-prop-28 .statement tag=0AW3}

*Let* $B$ *be a basis of* $R$, $B'$ *a subset of* $B$, $V'$ *the vector subspace of* $V$ *generated by* $B'$, $R' = R \cap V'$ *(which is a root system in* $V'$*),* $R'\tilde{}$ *the inverse root system (which is identified with the canonical image of* $R'$ *in* $R'\tilde{}$), $V_1$ *the orthogonal complement of* $R'\tilde{}$ *in* $V$, *and* $p$ *the projection of* $V$ *onto* $V'$ *parallel to* $V_1$. *然后，*$Q(R') = Q(R) \cap V'$，$P(R') = p(P(R))$。 *The set of dominant weights of* $R'$ *is the image under* $p$ *of the set of dominant weights of* $R$.

事实上，$Q(R)$是$V$的子群和基$B$，$Q(R')$是$V'$的子群和基$B'$（no. 7，第20号提案的Cor.4） $Q(R') = Q(R) \cap V'$ 是直接的。如果$\overline{\omega} \in P(R)$和$\alpha \in R'$，$\langle p(\overline{\omega}), \alpha^\vee \rangle = \langle \overline{\omega}, \alpha^\vee \rangle \in \mathbf{Z}$，那么$p(\overline{\omega}) \in P(R')$，因此$p(P(R)) \subseteq P(R')$。如果$\overline{\omega}' \in P(R')$、$\overline{\omega}'$扩展到线性形式$\overline{\omega}$在$V^*$上消失在$(B - B')\tilde{}$上；我们对所有$\alpha \in B$都有$\langle \overline{\omega}, \alpha^\vee \rangle \in \mathbf{Z}$，所以$\overline{\omega} \in P(R)$和$\overline{\omega}' = p(\overline{\omega})$；因此$P(R') \subseteq p(P(R))$。这样关于显性权的$P(R') = p(P(R))$和断言也以同样的方式得到证明。

#### 命题 29 {#lie-vi-s1-prop-29 .statement tag=0AW4}

*令*$\rho$*为根*$> 0$的一半和。

(i) $\rho = \sum_{\alpha \in B} \overline{\omega}_\alpha$； *这是* $C$ 的元素。
(ii) $s_\alpha(\rho) = \rho - \alpha$ *对于所有人* $\alpha \in B$。
(iii) $(2\rho|\alpha) = (\alpha|\alpha)$ *对于所有人* $\alpha \in B$。

由于$R$被减少，$s_\alpha(R_+(C) - \{\alpha\}) = R_+(C) - \{\alpha\}$和$s_\alpha(\alpha) = -\alpha$对应于$\alpha \in B$（no. 6，第17号提案的Cor.1），所以$s_\alpha(2\rho) = 2\rho - 2\alpha$。从$s_\alpha(\rho) = \rho - \langle \rho, \alpha^\vee \rangle$开始，我们看到
$$
\langle \rho, \alpha^\vee \rangle = 1 = \langle \sum_{\beta \in B} \overline{\omega}_\beta, \alpha^\vee \rangle.
$$
因而，$\rho = \sum_{\beta} \overline{\omega}_\beta$，进而$\rho \in C$。最后，(iii) 相当于$\langle \rho, \alpha^\vee \rangle = 1$。

#### 推论{#lie-vi-s1-n10-cor-1 .statement tag=0AW5}

令 $\sigma$ 为元素 $> 0$ $R^-$ 的一半和（对于$B^-$）。对于所有$\alpha \in V$，$\alpha$相对于基$B$的坐标和是$\langle \alpha, \sigma \rangle$。如果$\alpha \in R$，这个和就等于$\frac{1}{2} \sum_{\beta \in R_+ (\mathbf{C})} n(\alpha, \beta)$。

交换 $R$ 和 $R^-$ 的角色，对于所有 $\alpha \in B$，我们都有 $\langle \alpha, \sigma \rangle = 1$，因此得出推论。

### 11.考克斯特转变

令$C$为$R$的腔室，令$\{ \alpha_1, \ldots, \alpha_l \}$为$R$的相应的基，并令$c = s_{\alpha_1} \cdots s_{\alpha_l}$。 $W$的元素$c$称为$W$的*Coxeter变换*，由$C$和双射$i \mapsto \alpha_i$定义（第V, § 6, no. 1章）。它的阶$h$被称为$W$（或$R$）的*Coxeter数*。

#### 命题 30 {#lie-vi-s1-prop-30 .statement tag=0AW6}

*假设$R$是不可约的。令 $m$ 为整数，介于 1 和 $h - 1$ 之间，并与$h$素的。那么$\exp(\frac{2i\pi m}{h})$就是重数1$c$特征值。*

特别是，$m$是$W$的*指数*，cf. V, § 6, no. 2。

我们首先证明引理：

#### 引理 4 {#lie-vi-s1-lem-4 .statement tag=0AW7}

*对于所有$w \in W$，$w$的特征多项式有整数系数。*

我们知道（no. 6，Th.3）$\{ \alpha_1, \ldots, \alpha_l \}$是$R$生成的$V$的子群$Q(R)$的基。由于$w$使$Q(R)$保持稳定，因此其相对于$\{ \alpha_1, \ldots, \alpha_l \}$的矩阵有整数条目；因此它的特征多项式有整数系数。

令$P$为$c$的特征多项式。上述引理表明$P$的系数为整数。由章。 V, § 6, no. 2，科。根据第 3 条命题 2，单位元 $z = \exp(\frac{2i\pi}{h})$ 的原语第 $h$th 根是 $P$ 的简单根。因此，$z$超过$\mathbf{Q}$的每个*共轭*也是$P$的简单根。但我们知道（*代数*，第V章）单位元的原语$h$第根是共轭超过$\mathbf{Q}$。因此它们都是$P$的简单根，这证明了命题。

#### 命题 31 {#lie-vi-s1-prop-31 .statement tag=0AW8}

*假设$R$不可约且可约，令$\beta = n_1 \alpha_1 + \cdots + n_l \alpha_l$为$R$(cf.no. 8)的最高根。然后$n_1 + \cdots + n_l = h - 1$.*

令 $R_+$ 为集合相对于 $C$ 的正根。那么（no. 10，Cor. of Prop. 29）：

$$
n_1 + \cdots + n_l = \frac{1}{2} \sum_{\alpha \in R_+} n(\beta, \alpha)
$$
$$
= 1 + \frac{1}{2} \sum_{\alpha \in R_+, \alpha \neq \beta} n(\beta, \alpha) = 1 + \sum_{\alpha \in R_+, \alpha \neq \beta} \frac{(\alpha | \beta)}{(\alpha | \alpha)}
$$

根据no. 8，第 25 号提案 (iv)，对于所有 $\alpha \in R_+$ 和 $\alpha \neq \beta$，$n(\alpha, \beta) = 0$ 或 1，所以 $n(\alpha, \beta)^2 = n(\alpha, \beta)$，即 $\frac{4(\alpha | \beta)^2}{(\beta | \beta)^2} = \frac{2(\alpha | \beta)}{(\beta | \beta)}$。因此：

$$
n_1 + \cdots + n_l + 1 = 2 + 2 \sum_{\alpha \in R_+, \alpha \neq \beta} \frac{(\alpha | \beta)^2}{(\alpha | \alpha)(\beta | \beta)}
= 2 \sum_{\alpha \in R_+} \frac{(\alpha | \beta)^2}{(\alpha | \alpha)(\beta | \beta)} = (\beta | \beta)^{-1} \sum_{\alpha \in R} \left( \frac{\alpha}{\| \alpha \|} | \beta \right)^2.
$$

由章。 V, § 6, no. 2，科。的 Th。 1、

$$
\sum_{\alpha \in R} \left( \frac{\alpha}{\| \alpha \|} | \beta \right)^2 = h(\beta | \beta)
$$

所以$n_1 + \cdots + n_l + 1 = h$。

#### 命题 32 {#lie-vi-s1-prop-32 .statement tag=0AW9}

*假设 R 是不可约的，并且所有根具有相同的长度。让$\alpha \in R$。 R 的元素的数不与 $\alpha$ 正交，为 $4h - 6$。*

令$R'$为根的集合，与$\alpha$不成比例且不正交。
由章。 V, § 6, no. 2，科。的 Th。 1、

$$
(\alpha | \alpha)^2 + (\alpha | -\alpha)^2 + \sum_{\beta \in R'} (\alpha | \beta)^2 = h(\alpha | \alpha)^2,
$$

那就是

$$
\sum_{\beta \in R'} (\alpha | \beta)^2 = (h - 2)(\alpha | \alpha)^2.
$$

如果$\beta \in R'$，则按no. 3中的列表计算$(\alpha | \beta) = \pm \frac{1}{2} (\alpha | \alpha)$。因此

$$
\frac{1}{4} \operatorname{Card} R' = h - 2, \quad \operatorname{Card} R' = 4h - 8,
$$

根与$\alpha$ 不正交的数是$\operatorname{Card} R' + 2 = 4h - 6$。

#### 命题 33 {#lie-vi-s1-prop-33 .statement tag=0AWA}

*假设 R 是不可约且可约化的。放入$s_{\alpha_i} = s_i$，并令$\Gamma$为$c = s_1 \ldots s_l$生成的W的子群。*

(i) *令 $\theta_i = s_l s_{l-1} \ldots s_{i+1} (\alpha_i)$ ($i = 1, \ldots, l$)。然后，$\theta_i > 0, c(\theta_i) < 0$.*
(ii) *如果 $\alpha$ 是根 $> 0$，使得 $c(\alpha) < 0$，则 $\alpha$ 等于 $\theta_i$ 之一。*
(iii) *家族$(\theta_i)_{1 \leq i \leq l}$是Q(R)的基。*
(iv) *令$\Omega_i$为$\Gamma$下$\theta_i$的轨道。 集合$\Omega_i$是成对的不相交的，它们都是R上$\Gamma$的轨道，并且每个都有h元素。*

首先观察$(s_1, \ldots, s_l)$ 是$c$（第IV, § 1, no. 1 章）相对于$s_i$ 的集合 S 的*约化分解*。事实上，否则就会存在 S 的 $l - 1$ 元素的子集 $X = S - \{ j \}$ 使得 $c \in W_X$，这与 Cor.第 7 章提案 2 IV, § 1, no. 8。

应用科。 no. 6到$c$的第17号提案2给出了断言(i)和(ii)。

令$Q_i$为由$\alpha_j, j > i$生成的Q(R)的子群。 $Q_i$在$s_j, j > i$下稳定的是直接的，$s_j (\alpha_i) = \alpha_i$ mod。 $Q_i$ 换$j > i$。
因此：

$$
\theta_i = s_l \ldots s_{i+1} (\alpha_i) = \alpha_i \text{ mod. } Q_i.
$$

在其他字中，存在整数$c_{ij}$使得
$$
\theta_i = \alpha_i + \sum_{j > i} c_{ij} \alpha_j.
$$
部分 (iii) 紧随其后。

最后，令$\alpha$为根。 元素$\sum_{k=0}^{h-1} c^k(\alpha)$在$c$下是不变的，因此零（第V, § 6, no. 2章）。因此，$c^k(\alpha)$ 不能都具有相同的符号，并且存在$k$，使得$c^k(\alpha) > 0$ 和$c^{k+1}(\alpha) < 0$。通过(ii)，$c^k(\alpha)$是$\theta_i$之一。因此，$R$上$\Gamma$的每个轨道都是$\Omega_i$之一。 $V \otimes \mathbf{C}$扩展$(x|y)$至厄米特形式。 $R$中$\Gamma$的每个轨道最多有$h$元素，并且最多有$l$不同的轨道，由上面的注计算。现在（V, § 6, no. 2，定理2，ii）），$R$的基数等于$hl$，这立即暗示了（iv）。

### 12. 规范双线性形式

我们已经看到（no. 1，命题 3）对称的双线性形式
$$
(x, y) \mapsto B_R(x, y) = \sum_{\alpha \in R} \langle \alpha^*, x \rangle \langle \alpha^*, y \rangle
$$
$V$ 在 $A(R)$ 下是非简并且不变的。 交换 $R$ 和$R^*$ 的角色，可以得出$V^*$ 上的对称双线性形式 $(x^*, y^*) \mapsto B_{R^*}(x^*, y^*) = \sum_{\alpha \in R} \langle \alpha, x^* \rangle \langle \alpha, y^* \rangle$ 在$A(R)$ 下是非简并且不变的。

The inverse form of $B_{R^*}$ (resp. $B_R$) on $V$ (resp. $V^*$) will be called the *canonical bilinear form* on $V$ (resp. $V^*$) and denoted by $\Phi_R$ (resp. $\Phi_{R^*}$). 它在$A(R)$下是非简并且不变的。 设$\sigma$为由$B_{R^*}$定义的从$V$到$V^*$的同构。 然后，对于$x \in V$和$y \in V$：
$$
\Phi_R(x, y) = B_{R^*}(\sigma(x), \sigma(y)) = \sum_{\alpha \in R} \langle \alpha, \sigma(x) \rangle \langle \alpha, \sigma(y) \rangle.
$$
但是$\langle \alpha, \sigma(x) \rangle = B_{R^*}(\sigma(\alpha), \sigma(x)) = \Phi_R(\alpha, x)$。 因此，
$$
\Phi_R(x, y) = \sum_{\alpha \in R} \Phi_R(\alpha, x) \Phi(\alpha, y).
$$
(16)
根据no. 2的第7条命题，$\Phi_R$是$W(R)$下唯一满足恒等式（16）的非零对称双线性形式不变量。

对于 $\beta \in R$，(16) 给出
$$
\Phi_R(\beta, \beta) = \sum_{\alpha \in R} \Phi_R(\alpha, \beta)^2 = \frac{1}{4} \Phi_R(\beta, \beta)^2 \sum_{\alpha \in R} n(\alpha, \beta)^2,
$$
因此
$$
4 \Phi_R(\beta, \beta)^{-1} = \sum_{\alpha \in R} n(\alpha, \beta)^2.
$$
此外，通过 no. 1 的引理 2，对于 $x, y \in V$，我们有：

$$
B_R(x, y) = \sum_{\alpha \in R} \Phi_R \left( \frac{2\alpha}{\Phi_R(\alpha, \alpha)}, x \right) \left( \frac{2\alpha}{\Phi_R(\alpha, \alpha)}, y \right)
= 4 \sum_{\alpha \in R} \Phi_R(\alpha, x) \Phi_R(\alpha, y) \Phi_R(\alpha, \alpha)^{-2}.
$$

由此可见，如果 $R$ 是*不可约*，则存在一个常数 $\gamma(R) > 0$ 使得

$$
\sum_{\alpha \in R} \Phi_R(\alpha, x) \Phi_R(\alpha, y) \Phi_R(\alpha, \alpha)^{-2} = \gamma(R) \Phi_R(x, y).
$$ (18)

到$\gamma(R)$的定义，我们有$B_R(x, y) = 4\gamma(R) \Phi_R(x, y)$，所以

$$
\Phi_{R^{\sim}}(x^*, y^*) = (4\gamma(R))^{-1} B_{R^{\sim}}(x^*, y^*)
$$

对于$x^*, y^* \in V^*$。这就证明了$\gamma(R) = \gamma(R^{\sim})$。另一方面，对于$\beta \in R$，

$$
\Phi_{R^{\sim}}(\beta^{\sim}, \beta^{\sim}) = (4\gamma(R))^{-1} \sum_{\alpha \in R} \langle \beta^{\sim}, \alpha \rangle^2
= \gamma(R)^{-1} \sum_{\alpha \in R} \frac{\Phi_R(\alpha, \beta)^2}{\Phi_R(\beta, \beta)^2}
$$

因此，根据 (16)，

$$
\Phi_{R^{\sim}}(\beta^{\sim}, \beta^{\sim}) = \gamma(R)^{-1} \Phi_R(\beta, \beta)^{-2} \Phi_R(\beta, \beta)
$$

或者最后

$$
\Phi_R(\beta, \beta) \Phi_{R^{\sim}}(\beta^{\sim}, \beta^{\sim}) = \gamma(R)^{-1}.
$$ (19)

此外，如果$R$的所有根对于$\Phi_R$具有相同的长度$\lambda$，则（16）和（18）表明

$$
\gamma(R) = \lambda^{-4}.
$$ (20)

此外，如果 $h$ 是 $W$ 的 Coxeter 数，则 Cor.的 Th。第 1 章V, § 6, no. 2表明：

$$
h \Phi_R(x, x) = \sum_{\alpha \in R} \left( x, \frac{\alpha}{\lambda} \right)^2 \text{ for all } x \in V.
$$

与(16)比较，我们得出

$$
\lambda = h^{-1/2} \quad \text{or} \quad \gamma(R) = h^2.
$$ (21)

最后，公式(19)表明$R^{\sim}$的根对于$\Phi_{R^{\sim}}$有长度$\lambda$。

### 习题{#lie-vi-s1-exercises}

下面考虑的所有根系都是相对于真实的向量空间。我们用 $(x|y)$ 表示 Weyl 群 (cf. no. 3) 下的标量乘积不变量。

§ 1](exercises/s1/)参见[习题。
