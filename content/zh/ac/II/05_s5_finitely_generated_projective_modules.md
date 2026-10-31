---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 5
section_title: Finitely generated projective modules. Invertible fractional ideals
lang: zh
source: ac-i-vii
book_pages: 108-120, 146-153
pdf_pages: 0128-0140, 0166-0173
extraction: ocr
subsections:
    - "no": 1
      title: LOCALIZATION WITH RESPECT TO AN ELEMENT
      page: 108
      pdf_page: 128
    - "no": 2
      title: LOCAL CHARACTERIZATION OF FINITELY GENERATED PROJECTIVE MODULES
      page: 109
      pdf_page: 129
    - "no": 3
      title: RANKS OF PROJECTIVE MODULES
      page: 111
      pdf_page: 131
    - "no": 4
      title: PROJECTIVE MODULES OF RANK 1
      page: 114
      pdf_page: 134
    - "no": 5
      title: NON-DEGENERATE SUBMODULES
      page: 116
      pdf_page: 136
    - "no": 6
      title: INVERTIBLE SUBMODULES
      page: 117
      pdf_page: 137
    - "no": 7
      title: THE GROUP OF CLASSES OF INVERTIBLE MODULES
      page: 119
      pdf_page: 139
statements: 34
exercises: 25
content_sha256: d1b56bcdd5f4871b3b6407c9ceb665683c26505758927b8a5107de91c50e6d8b
translated_from: content/en/ac/II/05_s5_finitely_generated_projective_modules.md
translation_method: google
source_content_sha256: 39903d36e71fd82b177991bd175a5a56543cc66eaadad8c82a42b81dab501389
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 8f3d55d61f7870ec5c3bd4b14a7cb65116cfdb7450e44c677c758fa0efe491e6
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 5.有限生成射影模。可逆分数理想

### 1. 元素的本地化

令 $A$ 为环，且 $M$ 为 $A$ 模块。 对于每个元素 $f \in A$，我们应该写 $A_f = A[f^{-1}], M_f = M[f^{-1}] = M \otimes_A A[f^{-1}]$（§ 2，第 1 和第 2）；如果 $n \geq 0$ 的 $S_f$ 为集合关闭”，则 $A_{S_f} = S_f^{-1}A, M_{S_f} = S_f^{-1}M$。 Iff 在 $A$ 中可逆，$A_f$（分别为 $M_f$）被规范地识别为 $A$（分别为 $M$）； iff 是幂零的，则 $A_f = 0$ 和 $M_f = 0$。 对于每个$A$-模块同态$u : M \to N$，我们写$u_f = u \otimes 1 : M_f \to N_f$。

设$g$为$A$的另一个元素； $A_g$（分别$M_g$）与$(A_f)_{g/1}$（分别$(M_f)_{g/1}$）规范地标识，其中$g/1$是$A_g$中$g$的像，$u_{f,g}$与$(u_f)_{g/1}$（§ 2, no. 3， 命题7)。

#### 命题 1 {#ac-ii-s5-prop-1 .statement tag=04BE}

*令$f$为环$A$和$\phi : A \to A_f$、典范映射中的元素。 映射 $^a\phi : \operatorname{Spec}(A_f) \to \operatorname{Spec}(A)$ 是 $\operatorname{Spec}(A_f)$ 到 $X = \operatorname{Spec}(A)$ (§ 4, no. 3) 的开子空间 $X_f$ 的同胚。*

这是 § 4, no. 3 的特殊情况，命题 13 的推论。

#### 命题 2 {#ac-ii-s5-prop-2 .statement tag=04BF}

*设$A$为环，$u : M \to N$为$A$模同态，$p$为$A$的素理想。

(i) 假设 $u_p : M_p \to N_p$ 是满射且 $N$ 是有限生成的。那么存在 $f \in A - p$ 使得 $u_f : M \to N$ 是满射的。

(ii) 假设 $u_p$ 是双射，$M$ 是有限生成的，$N$ 是有限呈现的。那么存在 $f \in A - p$ 使得 $u_f$ 是双射的。*

设$R$和$Q$为$u$的核和余核；如果$u_g$（或$u_p$）的$g \in A$、核和余核分别为$R_g$和$Q_g$（分别为$R_p$和$Q_p$）（§ 2, no. 4、定理 1）。然后$Q_p = 0$；由于$N$是有限生成的，所以$Q$也是有限生成的，并且存在$g' \in A - p$使得$g'Q = 0$（§ 2, no. 2，推论2到命题4），从而$Q_{g'} = 0$。在(ii)的假设下，序列$0 \to R_{g'} \to M \to N \to 0$是精确的，因此$R_{g'}$是有限生成的（章I, § 2, no. 8，引理9）。现在，

$$
(R_{g'})_{pR_{g'}} = R_p = 0;
$$

因此存在$g_1 \in A, - pA_{g'}$使得$g_1 R_{g'} = 0$（§ 2, no. 2，推论2到命题4）。然后$g_1 = g''/{g'}^h$，其中$g'' \in A - p$；因为 $g'/1$ 在 $R_{g'}$、$(g''/1)R_{g'} = 0$、从而 $R_{g'g''} = (R_{g'})_{g''/1} = 0$ 中是可逆的。如果$f = g'g''$、$f \in A - p$、$Q_f = 0$和$R_f = 0$，则$u_f$是双射的。

#### 推论 {#ac-ii-s5-n1-cor-1 .statement tag=04BG}

*如果$N$是有限存在的并且$N_p$是秩$p$的自由$A_p$模块，则存在$f \in A - p$使得$N$是秩$p$的自由$A_f$模块。*

存在假设 $p$ 元素 $x_i \in \mathbf{N}$ ($1 \leq i \leq p$)，使得自由 $A_,-$ 模块 $N_p$ 的 $x_i/1$ 形式基。考虑同态$u : A^p \to \mathbf{N}$，使得$u(e_i) = x_i$对应于$1 \leq i \leq p$，$(e_i)_{1 \leq i \leq p}$是典范基等于$A^p$。由于 $u_p$ 与假设是双射的，因此存在 $f \in A - p$ 使得 $u_f$ 是双射的，因为命题 2。

#### 命题 3 {#ac-ii-s5-prop-3 .statement tag=04BH}

*让*$(f_i)_{i \in I}$*成为环*$A$的元素的有限族，*生成的是*$A$*的理想*$A$。 *环* $B = \prod_{i \in I} A_i$，*是一个忠实的平坦*$A$*-模块*。

到§ 2，没有。 **4**，定理 1，每个$A_i$都是一个扁平的$A$模块，因此$B$也是（章I, § 2, no. 3，命题2）。另一方面，如果$p$是$A$的素理想，则存在指标$i$，因此$f_i \notin p$和$p_{f_i} = pA_{f_i}$是$A_{f_i}$的素理想。然后从 $pA_{f_i} \neq A_{f_i}$ 开始$pB \subset pA_{f_i} \times \prod_{j \neq i} A_j \neq B$；这足以暗示$B$是一个忠实的扁平$A$模块（章I, § 3, no. 1，命题1）。

#### 推论{#ac-ii-s5-n1-cor-2 .statement tag=04BI}

*在命题 3 的假设下，对于一个* $A$*-模* $M$ *的有限生成（或有限呈现），对于每个指标* $i$，*该* $A_{f_i}$*-模* $M_{f_i}$ *是有限生成（或有限呈现）*。

条件显然是必要的（§ 2，第**4**）。相反，如果所有 $M_{f_i}$ 都是有限生成（或有限呈现）的，则 $M' = \prod_{i \in I} M_{f_i}$ 是有限生成（或有限呈现）$B$ 模块，因为我们显然可以假设对于每个 $i$ 都有正合序列 $AT_i \to A^n_{f_i} \to M_{f_i} \to 0$，其中 $m$ 和$n$ *独立于* $i$。现在，$M' = M \otimes_A B$。然后从命题 3 和章 I, § 3 得出推论，没有。 **6**，命题11。

注 $f_i$ 上的条件意味着开集合 $X_{f_i}$ 形式 $\mathrm{Spec}(A)$ 的*覆盖*（§ 4, no. 3，推论 3 到命题 11）。

### 2.本地刻画有限生成射影模

#### 定理 1 {#ac-ii-s5-thm-1 .statement tag=04BJ}

*设*$A$*为环和*$P$*一个*$A$*-模块*。 *以下属性是等效的*：

(a) $P$ *为有限生成射影模*。
(b) $P$ *是有限呈现的模，并且对于每个最大理想* $m$ *的* $A$，$P_m$ *是一个自由* $A_m$*-模块*。
(c) $P$ * 是有限生成模，对于所有 * $p \in \mathrm{Spec}(A)$，* $A_p$*-模块* $P_p$ * 是免费的，并且，如果我们用* $r_p$ 表示它的秩，则 *函数* $p \mapsto r_p$ * 是局部常数拓扑空间* $\mathrm{Spec}(A)$ *（即，* $\mathrm{Spec}(A)$ 的每个点 *承认邻域，其中函数是常数）*。

(d) 存在$A$的元素的有限族$(f_i)_{i \in I}$，生成的理想的$A$，这样，对于所有$i \in I$，$A,$-模块$P_{f_i}$对于有限秩是自由的。

(e) 对于$A$的每个最大理想$m$，都存在$f \in A - m$，使得$P_f$是有限秩的自由$A,$模。

我们通过证明展示定理以下概形的含义

(一)⇔(四)

(b) ⇌ (e)

(三)

(a) ⇒ (b)：我们知道有限生成射影模是有限呈现的 (章 I, § 2, no. 8, 引理 8 (iii))；如果$P$是射影$A$模，$P_m = P \otimes_A A_m$是射影$A_m$模（\emph{代数}，章II, § 5, no. 1，命题4的推论）；最后，由于 $A_m$ 是局部环，因此每个有限呈现的射影 $A_m$ 模都是自由的（§ 3, no. 2，命题 5 的推论）。

(b) ⇒ (e)：这是从 no. 1 的命题 2 的推论得出的。

(c) ⇒ (e): 令$m$为$A$的极大理想；写出$r_m = n$，并令$(x_i)_{1 \leq i \leq n}$为$P$的基。我们可以假设$x_i$是元素$p_i \in P$$(1 \leq i \leq n)$的典范像到乘法乘可逆元的$A,$之内。令$(e_i)_{1 \leq i \leq n}$为$A^n$和$u : A^n \to P$同态的典范基，使得$u(e_i) = p_i$为$1 \leq i \leq n$。由于 $P$ 是有限生成的，因此从 no. 1 的命题 2 可以得出，存在 $f \in A - m$ 使得 $u_f$ 是满射的。我们结论认为$u_{f,g}$对于所有$g \in A - m$也是满射，并且到假设存在$g \in A - m$使得$r_p = n$对于$p \in X,$。然后，替换$f$乘以$f g$，我们可以假设$r_p = n$对于所有$p \in X,$。那么$u_p : A_p^n \to P_p$就是满同态，而$P_p$和$A_p$都是相同秩的免费$A,$模块；因而（§ 3, no. 2，命题 6 的推论）$u_p$ 对于所有 $p \in X_f$ 都是双射的。令$p'$为$A,$的素理想，令$p$为典范映射下$A$中的逆像；如果$(A_f^{n})_{p'}$和$(P_f)_{p'}$在典范同构下与$A_p^n$和$P_p$等同，则$(u_f)_{p'}$与$u_p$等同，因此是双射的。我们结论 $u_f$ 是双射 (§ 3, no. 3, 定理 1)，从而成立 (e)。

(e) ⇒ (d)：令 $E$ 为 $\in A$ 的集合，使得 $P_f$ 是有限生成的自由 $A_f$ 模块。 假设意味着$E$不包含在$A,$的最大理想中，因此$E$生成是理想$A$，因此存在$E$和$a_i \in A$$(1 \leq i \leq n)$的元素的有限族$(f_i)_{1 \leq i \leq n}$，这样那个$1 = \sum_{i=1}^n a_i f_i$； 从而 (d)。

(d) ⇒ (c): 从no. 1推论到命题 3，$P$是有限生成的。另一方面，对于$A$的每个素理想$p$，都存在指标$i$使得$p \in X_{f_i}$；如果$p' = p_{f_i}$，则$P_p = (P_{f_i})_{p'}$（§ 2, no. 5，命题

10) 因此到假设 $P_p$ 是自由的并且与 $P_{f_i}$ 具有相同的秩，这证明了 (c)。

(d) ⇒ (a): 考虑环 $B = \prod_{i \in I} A_i$ 和 B-模
$$
M = \prod_{i \in I} P_i = P \otimes_A B.
$$
对于每个指标$i$，都存在一个空闲的$A_i$模块$L$，使得$P_i$是$L$的直因子，并且可以假设所有$L$具有相同的秩；则$L = \prod_{i \in I} L_i$是一个自由的B-模，其中M是直因子，在其他字中，M是有限生成的射影B-模。由于 B 是忠实平坦的 A-模 (no. 1, 命题 3)，我们结论 P 是有限生成的射影 A-模 (章 I, §3, no. 6, 命题 12)。

#### 推论 1 {#ac-ii-s5-thm-1-cor-1 .statement tag=04BK}

假设叙述与定理 1 的等价性质成立。令 m 为整数 > 0，这样，对于 P 的元素的每个族 $(x_i)_{1 \leq i \leq m}$，都存在 A 的元素的族 $(a_i)_{1 \leq i \leq m}$，该族不全是零的除子并且为 $\sum_{i=1}^m a_i x_i = 0$。然后，对于所有 $p \in \operatorname{Spec}(A)$，$r_p \leq m$。

设p是A的素理想； 集合 $r = r_p$ 并令 $(y_j)_{1 \leq j \leq r}$ 为免费 $A_p$ 模块 $P_p$ 的基。 P 和 $s \in A - p$ 存在元素 $x_j$ ($1 \leq j \leq r$)，使得$y_j = x_j / s$ 对于所有 $j$。然后对于A的元素的每个家庭$(a_j)_{1 \leq j \leq r}$，使得$\sum_{j=1}^r a_j x_j = 0$，$\sum_{j=1}^r (a_j/1) y_j = 0$在$P_p$，从而$a_j/1 = 0$对于$1 \leq j \leq r$。由于$A - p$不为包含0，这表明$a_j$都是A中零的除子（§ 2, no. 1，注3），因此必然有$r \leq m$。

#### 推论 2 {#ac-ii-s5-thm-1-cor-2 .statement tag=04BL}

每个有限呈现的平面模都是投影的。

如果 P 是有限呈现的平坦 A-模并且 m 是 A 的最大理想，则 $A_m$ 模 P 是平坦的（§ 3, no. 4，命题 13）并且是有限呈现的（§ 2, no. 4），因此是自由的（§ 3, no. 2，推论 2 到命题 5），因此，定理 1 的条件 (b) 成立。

注
(1) 存在有限生成平面模，它不是射影的(习题7)。
(2) 非交换环上的推论 2 到定理 1 扩展到模 (章 I, §2, 习题 15)。

### 3.秩投射模

#### 定义 1 {#ac-ii-s5-def-1 .statement tag=04BM}

令 P 为有限生成的射影 A-模。对于A的每个素理想$p$，自由$A_p$模$P_p$的秩称为P在$p$处的秩，并用$\operatorname{rg}_p(P)$表示。

到定理 1 时，整数值函数 $p \mapsto \mathrm{rg}_p(P)$ 在 $X = \mathrm{Spec}(A)$ 上是*局部常数*；因此，如果 $X$ *连接*，特别是如果环 $A$ 是 *整环*（§ 4, no. 3，推论 2 到命题 15）。

#### 定义 2 {#ac-ii-s5-def-2 .statement tag=04BN}

*令$n$为整数$\geqslant 0$。射影$A$模$P$如果是有限生成的，则被称为*秩* $n$，并且对于$A$的每个素理想$p$来说，$\mathrm{rg}_p(P) = n$。*

显然，每个有限生成的*自由* $A$-模块$L$在定义2、$n$等于$L$的*维数*（或*秩*）的意义上具有秩$n$，其中定义*代数*，章II, § 7, no. 2。

秩 0 的投射模是零（§ 3, no. 3，推论 2 到定理 1）。如果$A$不减为0，且射影$A$模$P$为秩$n$，则唯一确定整数$n$；然后用$\mathrm{rg}(P)$表示。

#### 定理 2 {#ac-ii-s5-thm-2 .statement tag=04BO}

*令$P$为$A$模块，且$n$整数$\geqslant 0$。以下属性是等效的：*

(a) *$P$ 是秩* $n$ 的投影。

(b) *$P$是有限生成的，并且对于每个最大理想*$m$*的*$A$，**$A$-*模*$P$，*不包含秩*$n$。

(c) *$P$ 是有限生成的，并且对于每个素理想* $p$ *的* $A$，*该* $A$-*模* $P_p$ *不包含秩* $n$。

(d) *对于* $A$的每个最大理想* $m$ *，*存在* $f \in A - m$ *使得* $A$-*模* $P_f$ *不包含秩* $n$。

由定义2和定理1，(a)和(c)是等价的； (b) 意味着 (c)，因为对于 $A$ 的每个素理想 $p$，都存在一个极大理想 $m$ 包含 $p$，并且写作 $p' = p_m$，$P_p$ 同构于 $(P_m)_{p'}$ (§ 2, no. 5，命题) 11）；如果$P_m$不含秩$n$，那么$P_{p'}$也是。 性质 (c) 凭借定理 1 隐含 (d)，且当且仅当 $\in A - m$ 和 $m' = m_f$，$P_m$ 与 $(P_f)_{m'}$ 同构的，因此 $P_f$ 和 $P$ 的秩相等。最后，最后一个参数和定理 1 表明 (d) 蕴涵 (b)。

#### 注 {#ac-ii-s5-n3-rem-1 .statement tag=04BP}

*如果* $A$ *是整环，射影* $A$-*模承认明确定义的秩*（在定义 2 的意义上），*如上面所观察到的；此外，这个秩重合与代数、章II, § 7, no. 2中定义的秩； 应用定理 2 (c) 和* $p = (0)$ 就足够了。

令 $E$ 和 $F$ 为两个有限生成的射影 $A$ 模。我们知道（*代数*、章II, §§ 2和3）$E \times F$、$E \otimes_A F$、$\mathrm{Hom}_A(E, F)$和$E$的对偶$E^*$是射影且有限生成的；每个整数$k > 0$的外部幂$\bigwedge^k E$也是如此（*代数*，章111）。此外，从定义 1 和 § 2, no. 7、命题 18 和 19 以及 no. 8 可以立即得出，对于 $A$ 的每个素理想 $p$：

(1)
$$
\mathrm{rg}_p(E \times F) = \mathrm{rg}_p(E) + \mathrm{rg}_p(F)
$$

(2) $\mathrm{rg}_p(E \otimes_A F) = \mathrm{rg}_p(E) \cdot \mathrm{rg}_p(F)$

(3) $\mathrm{rg}_p(\mathrm{Hom}_A(E, F)) = \mathrm{rg}_p(E) \cdot \mathrm{rg}_p(F)$

(4) $\mathrm{rg}_p(E^*) = \mathrm{rg}_p(E)$

（5）$\mathrm{rg}_p(\wedge^k E) = \binom{\mathrm{rg}_p(E)}{k}$。

如果定义了E和F的秩，则定义了$E \times F, E \otimes_A F,$、$\mathrm{Hom}_A(E, F), E^*$和$\wedge^k E$，省略指标$p$，上式也成立。此外：

#### 推论 {#ac-ii-s5-n3-cor-1 .statement tag=04BQ}

*对于有限生成的射影 A-模 P 为秩 n，$\mathbf{A}^n P$ 为秩 1 是充分必要的。*

#### 命题 4 {#ac-ii-s5-prop-4 .statement tag=04BR}

*设 B 为交换律 A-代数，P 为秩 n 的射影 A-模。 B-模 $P_{(B)} = B \otimes_A P$ 是秩 n 的投影。*

我们知道 $P_{(B)}$ 是射影且有限生成的（*代数*、章 II, § 5, no. 1，命题 4 的推论）。如果 q 是 B 的素理想，p 是 A 中的逆像，则

$$
(P_{(B)})_q = (P \otimes_A B) \otimes_B B_q = P @_A B_q = (P \otimes_A A_i) \otimes_A B_q
$$

并且，根据假设，$P \otimes_A A_i$是秩$n$的自由A，模块，$(P_{(B)})_q$是秩$n$的自由$B_q$模块。

#### 命题 5 {#ac-ii-s5-prop-5 .statement tag=04BS}

*设 A 为半局部环，P 为有限生成射影 A-模。如果定义 P 的秩，则 P 为自由A-模。*

首先假设 A 同构于域 $K_i$ ($1 \leq i \leq n$) 的乘积。然后用 A 的最小理想 (*代数*, 章 VIII, § 3, no. 1) 来确定 $K_i$，并且对于 K 的所有 $i$、和 $p_i$，指标 $j \neq i$ 是 A 的最大理想， $p_i$ ($1 \leq i \leq n$) 是 A 的唯一素理想。因此，每个有限生成A-模 P 都是其同典型分量 $P_i$ ($1 \leq i \leq n$) 的直和，$P_i$ 同构于有限数 $r_i$ 的直和 A-模同构于 K，(*代数*、章 VIII, § 5, no. 1、命题 1 和 no. 3、命题 11)； 环$A_{r_i}$等同于K，并湮灭指标$j \neq i$的$P_j$，因此$r_i = \mathrm{rg}_{p_i}(P)$；如果所有$r_i$都等于相同的数$r$，则在这种情况下P与$A^r$、从而命题同构。一般情况下，令$\mathfrak{R}$为A和$B = A / \mathfrak{R}$的雅各布森根式；因为 B 是域的乘积，所以射影 B-模 $P_{(B)}$ 在命题 4 之前的注是自由的。 *此外，P 是平 A-模和命题，然后从 § 3, no. 2、命题得出5.*

### 4.投射模共秩1

#### 定理 3 {#ac-ii-s5-thm-3 .statement tag=04BT}

令 $A$ 为环且 $M$ ajnitely 生成 $A$ 模块。

(i) *如果存在一个$A$模$N$使得$M \otimes_A N$同构于$A$，模$M$是秩1的投影。*

(ii) *相反，如果 $M$ 是秩 1 的投影且 $M^*$ 是 $M$ 的对偶，则典范同态 $u : M \otimes_A M^* \to A$ 相应的到规范双线性形式 $(x, x^*) \to \langle x, x^* \rangle$ $M \times M^*$ (代数, 章 II, § 2, no. 3) 是双射。*

(i) 需要证明，对于$A$的每个最大理想$m$，$A_m$模$M$不包含秩 1 (定理 2 (b))；我们可以通过 $A_m$ 自由地替换 $A$，因此可以假设 $A$ 是*本地* 环（$§ 2$，no. 7，命题 18）。让$k = A/m$。 同构的$v : M \otimes_A N \to A$定义同构

$$
v \otimes 1_k : (M/mM) \otimes_k (N/mN) \to k
$$

由于$(M/mM) \otimes_k (N/mN)$超过$k$的秩是$M/mM$和$N/mN$秩乘积，后者必然等于1，另外字$M/mM$是单生的。由此可见$M$是单生的（$§ 3$，no. 2，推论2至命题4）；另一方面，$M$的湮没子也湮灭了$M \otimes_A N$，因此是零，这证明$M$与$A$同构的。

(ii) 足以证明，对于$A$的每个最大理想$m$，$u_m$是同构（$§ 3$，no. 3，定理1）。由于 $M$ 是有限呈现的 (章 I, $§ 2$, no. 8, 引理 8)，$(M^*)_m$ 被规范地识别为对偶 $(M_m)^*$ ($§ 2$, no. 7, 命题) 19) 并且，由于 $M_m$ 与它的对偶 $(M_m)^*$ 一样没有秩 1，因此显然典范同态 $u_m : (M_m) \otimes_{A_m} (M_m)^* \to A_m$ 是双射，从而完成证明。

*注* (1)。如果 $M$ 是秩 1 的射影且 $N$ 使得 $M \otimes_A N$ 同构于 $A$，则 $N$ 同构于 $M^*$：有同构

$$
N \to N \otimes A \to N \otimes M \otimes M^* + A \otimes M^* \to M^*.
$$

#### 命题 6 {#ac-ii-s5-prop-6 .statement tag=04BU}

*设$M$和$N$是秩1的射影$A$模。那么$M \otimes_A N$、$\operatorname{Hom}_A(M, N)$和$M$的对偶$M^*$是秩1的射影。*

这紧接着公式 (2)、(3) 和 (4)。

Let us now note that every finitely generated $A$-module is isomorphic to a quotient module of $L = \mathbf{A}^{(\mathbf{N})}$; we may therefore speak of the *set $F(A)$ of classes of finitely generated $A$-modules* with respect to isomorphism (*Set Theory*, Chapter I, §6, no. 9); we denote by $P(A)$ the subset of $F(A)$ consisting of the classes of projective $A$-modules of rank 1 and by $\operatorname{cl}(M)$ the image in $P(A)$ of a projective $A$-module $M$ of rank 1. 对于两个射影$A$模$M$，直接的，

N of 秩 1, cl(M \otimes_A N) 仅取决于 cl(M) 和 cl(N)；作为定义我们集合

(6) $$ \mathrm{cl}(M) + \mathrm{cl}(N) = \mathrm{cl}(M \otimes AN) $$

因此，在 $P(A)$ 上定义了合成的内部律。

#### 命题 7 {#ac-ii-s5-prop-7 .statement tag=04BV}

* 秩 1 的射影 A-模类集合 $P(A)$，与合成 (6) 的律，是交换律群。如果 M 是秩 1 的射影 A-模并且 $M^*$ 是它的对偶，那么*

(7) $$ \mathrm{cl}(M^*) = -\mathrm{cl}(M) \quad \text{and} \quad \mathrm{cl}(A) = 0. $$

张量积的结合性和交换律表明合成(6)的律是结合律和交换律； $A \otimes_A M$和M之间的同构证明在这个律下$\mathrm{cl}(A)$是单位元素，并且凭借定理3，$\mathrm{cl}(M) + \mathrm{cl}(M^*) = \mathrm{cl}(A)$，从而命题。

设 B 为交换律 A-代数，M 为秩 1 的射影 A-模；那么 $M_{(B)} = B \otimes_A M$ 是秩 1 (no. 3, 命题 4) 的投影 B-模。那么存在称为规范 $\phi : P(A) \to P(B)$ 的映射使得

(8) $$ \phi(\mathrm{cl}(M)) = \mathrm{cl}(M_{(B)}). $$

两个 A-模 M, N 的方程 $M_{(B)} \otimes_B N_{(B)} = (M \otimes_A N)_{(B)}$ 证明映射 $\phi$ 是可交换的群 *同态*。

*注 (2).* 定理 1 的条件 (e)（相当于 P 是射影且有限生成的事实）也可以用说表示，模* $\tilde{P}$ 在$X = \mathrm{Spec}(A)$ *与 P 相关联(*) 上的*束是局部自由且有限的型*，因此可以解释为向量丛的截面束超过 X。相反，超过X的每个向量丛都来自有限生成射影模，它被确定在唯一的同构内； 秩 $n$的投射模，因此对应到向量丛，所有纤维都具有维数$n$。特别是，秩 1 对应的向量丛到秩 1的投射模。如果我们用$\mathscr{O}_X$结构捆$\tilde{A}$和$\mathscr{O}_X^*$表示单位*的*捆$\mathscr{O}_X$（其X开路集合U上的截面是U上$\mathscr{O}_X$截面环可逆元），因此群$P(A)$与第一个同构上同调群$H^1(X, \mathscr{O}_X^*)$.*

(*参见 A. Grothendieck, Éléments de géométrie algébrique, I (§ 1) (Publ. Math. I.H.E.S., no. 4, 1960)。

### 5.非简并子模

在这个没有。以及以下两个，$A$表示环，$S$是$A$由……组成与元素的乘法子集，它们不是$A$中零的除子，和 $B$ 环 $S^{-1}A$； $A$ 与子环或 $B$ ($§ 2$、no. 1、注 3) 被规范地标识。因此，$S$的元素在$B$中是可逆的。

对于应用来说，最重要的特殊情况之一是，其中$A$是整环，而$S$是元素中的集合，$\neq 0$中$A$；那么$B$就是$A$的分数中的域。

#### 定义 3 {#ac-ii-s5-def-3 .statement tag=04BW}

令$M$为$B$的子A模块。如果$B.M = B$，$M$ 称为非简并。

如果$B$是域，这个条件仅仅意味着$M$没有减少到0。

#### 命题 8 {#ac-ii-s5-prop-8 .statement tag=04BX}

令$M$为$B$的子A模块。以下条件是等效的：
(a) $M$ 是非简并的。
(b) $M$ 满足 $S$。
(c) 如果 $j : M \to B$ 是典范嵌入，则同态 $u = S^{-1}j : S^{-1}M \to B$ 是双射的。

(a) 意味着 (b)，因为如果 $B.M = B$，则存在 $a \in A, s \in S$ 和 $x \in M$，使得 $(a/s)x = 1$，因此 $ax = s$ 属于到 $S \cap M$。看出 (b) 暗示 (c)，注 $u$ 已经是单射的 ($§ 2$, no. 4, 定理 1)；此外，如果$B$中$x/x \in S^{-1}M$的$u$下的$x \in M \cap S$、像等于1，因此$u$是满射。最后，(c) 清楚地暗示了(a)。

#### 推论{#ac-ii-s5-n5-cor-1 .statement tag=04BY}

如果$M$和$N$是$B$的两个非简并子A-模块，则A-模、$M + N, M.N$和$M \cap N$是非简并的。

断言对于 $M + N$ 来说是微不足道的；另一方面，如果$s \in S \cap M$和$t \in S \cap N$，则$st \in S \cap (M.N)$和$st \in S \cap (M \cap N)$。

给定$B$的两个子A模块$M$和$N$，让我们用$N : M$表示那些$b \in B$的$B$由……组成的子A模块，使得$bM \subset N$（章I， $§ 2$、no. 10、注）。如果将$M$到$N$的每个$b \in N : M$映射到同态$h_b : x \mapsto bx$，则从$N : M$到$\operatorname{Hom}_A(M, N)$得到典范同态$b \mapsto h_b$。

#### 命题 9 {#ac-ii-s5-prop-9 .statement tag=04BZ}

令$M, N$为$B$的两个子A模块。如果 $M$ 是非简并的，则从 $N : M$ 到 $\operatorname{Hom}_A(M, N)$ 的典范同态是双射的。

让$s \in S \cap M$。如果对于所有 $x \in M$，$b \in N : M$ 使得 $bx = 0$，则 $bs = 0$、从而 $b = 0$，因为 $s$ 不是 $B$ 中 0 的除子。另一方面，令 $f \in \mathrm{Hom}_A(M, N)$ 和集合 $b = f(s)/s$；对于所有$x \in M$，存在$t \in S$使得$tx \in A$。然后
$$
f(x) = s^{-1}t^{-1}f(stx) = s^{-1}t^{-1}txf(s) = bx,
$$
从而$b \in N : M$和$f = h_b$，证明命题。

#### 注 {#ac-ii-s5-n5-rem-1 .statement tag=04C0}

特别是，$A : M$ 被规范地标识为$M$ 的对偶$M^*$，$M \times M^*$ 上的规范双线性形式被规范地标识为乘法 $B \times B \to B$ 的限制到$M \times (A : M)$。

### 6.不可逆子模

（我们保留记号和no. 5。）

#### 定义 4 {#ac-ii-s5-def-4 .statement tag=04C1}

如果存在$B$的*子*-A-模块$N$使得$M.N = A$，则$B$的*子*-A-模块$M$称为可逆的。

#### 例 {#ac-ii-s5-n6-exa-1 .statement tag=04C2}

如果$b$是$B$的可逆元，则$A$模$Ab$是可逆的，如取$N = Ab^{-1}$所示。

#### 命题 10 {#ac-ii-s5-prop-10 .statement tag=04C3}

*令 $M$ 为可逆子*-A*-模 & $B$。然后：
(i) 存在$s \in S$使得$As \subset M \subset As^{-1}$（特别是$M$是非简并的）。
(ii) $A : M$ 是 $B$ 中唯一满足 $M.N = A$ 的*子*-A*-模块* $N$。

如果$M.N = A$，则$B.M = B.(B.M) \supset B.(M.N) = B.A = B$，因此$M$是非简并的。类似地，$N$是非简并的。如果$t \in S \cap M$和$u \in S \cap N$（no. 5，命题8），元素$s = tu$属于到$S \cap M \cap N$，从而$Ms \subset M.N = A$，因此$As \subset M \subset As^{-1}$。
另一方面，显然$N \subset A : M$，从而
$$
A = M.N \subset M.(A : M) \subset A
$$
和$M.(A : M) = A$；将两边乘以 $N$，得出 $A : M = N$，即完成证明。

#### 定理 4 {#ac-ii-s5-thm-4 .statement tag=04C4}

*令$M$为$B$的非简并子*-A*-模块*。 *以下属性是等效的*：
(a) $M$ 是可逆的。
(b) $M$ 是投影。
(c) $M$ 是秩 1 的投影。
(d) $M$ 是有限生成的 $A$ 模，并且对于 $A$ 的每个最大理想 $m$，$A_m$ 模 $M_m$ 是单生的。

让我们首先展示属性 (a)、(b) 和 (c) 的等价。如果 (a) 成立并且 N 是 B 的子 A 模块，使得 M 。 N = A，则有关系

$$
\sum_{i=1}^{p} m_i n_i = 1 \quad (m_i \in M, n_i \in N \text{ for all } i).
$$

对于所有 $x \in M$、集合 $v_i(x) = n_i x$； M 上的 $v_i$ 为线性形式，并且对于所有 $x \in M$，通过 (9) $x = \sum_{i=1}^{n} m_i v_i(x)$；这证明了 (代数, 章 11, §2, no. 6, 命题 12) M 是射影的并且由 $m_i$ 生成；因此M是有限生成射影模。

设m为A的最大理想；我们证明整数$r = \mathrm{rg}_m(M)$等于1。令S'为$\mathbf{A}_{m'}$中S的像；因为 S 的元素不是 A 中 0 的除子，所以 S' 的 $\mathbf{A}_{m'}$ 不是 0 的除子，因为 $\mathbf{A}_{m'}$ 是平的 A-模（§ 2, no. 4、定理 1 和章） I, §2, no. 4、命题 3)；那么 ${S'}^{-1}A_m \neq 0$ 并且，由于 $M_m$ 是秩 $r$ 的免费 $A_m$ 模块，${S'}^{-1}M_m$ 是秩 $r$ 的免费 ${S'}^{-1}A_m$ 模块。但是，如果 T' 是 $S^{-1}A$ 中 A $-m$ 的像，则${S'}^{-1}A$（分别为 ${S'}^{-1}M_m$）被规范地标识为 ${T'}^{-1}(S^{-1}A)$（分别为 ${T'}^{-1}(S^{-1}M)$）（§ 2, no. 3、命题 7）。现在$S^{-1}M = B$ (命题 8 (c))，因此${T'}^{-1}(S^{-1}M)$是秩 1除以${T'}^{-1}(S^{-1}A)$的自由A-模，这证明了$r = 1$并显示了蕴涵(a)$\Rightarrow$(c)。

蕴涵 (c) $\Rightarrow$ (b) 是微不足道的。让我们证明 (b) $\Rightarrow$ (a)。 M 上存在假设线性形式的族（不一定有限）$(f_\lambda)_{\lambda \in L}$ 和 M 的元素族$(m_\lambda)_{\lambda \in L}$，使得对于所有$x \in M$，族$(f_\lambda(x))$ 具有有限支撑和$x = \sum_{\lambda \in L} m_\lambda f_\lambda(x)$ （代数，章II, §2, no. 6，命题12）。由于 M 是非简并的，$f_\lambda(x) = n_\lambda x$ 对于某些 $n_\lambda \in A$：M 凭借 no. 5 的命题 9。取x为M$\cap S$（no. 5，命题8）的元素，可以看出，除了指标和$\sum_{\lambda \in L} m_\lambda n_\lambda = 1$的有限数之外，必然为$n_\lambda = 0$。这显然暗示了 M 。 （A：M）= A，从而（a）。

根据no. 3的定义2，(c)蕴含(d)。让我们展示逆命题。由于M是非简并的，所以它的湮没子是零（命题8（b）），那么$M_m$的湮没子也是（§ 2, no. 4，公式（9））。由于 M, 被假定为单生 & 模，因此它不包含秩 1，然后从 no. 3、定理 2 得出 M 是秩 1 的投影。

#### 推论{#ac-ii-s5-n6-cor-1 .statement tag=04C5}

B 的每个可逆子 A 模块都是平坦且有限呈现的。
这是从定理 4 (c) 得出的。

#### 命题 11 {#ac-ii-s5-prop-11 .statement tag=04C6}

设M、N为B的两个子A模。假设M是可逆的。然后：
(i) 典范同态 $M \otimes_A N \to M . N$ 是双射的。
(ii)$N : M = N . (A : M)$和$N = (N : M) . M$。

设$j$为典范嵌入$N \to B$。由于 $M$ 是平面 $A$ 模（定理 4 的推论），$1 \otimes j : M \otimes_A N \to M \otimes_A B$ 是单射的。但是，作为$B = S^{-1}A$，$B$-模块$M \otimes_A B$等于$S^{-1}M$，因此被识别为$B$，因为$M$是非简并的（no. 5，命题8）。如果进行该识别，则$1 \otimes j$中的像为$M . N$、从而(i)。

让我们集合$M' = A : M$。那么显然是$M'.N \subset N : M$和$M.(N : M) \subset N$。另一方面，从 $M.M' = A$ (命题 10) 开始，

$$
N : M = M'.M.(N : M) \subset M'.N
$$

和 $N = M.M'.N \subset M.(N : M)$、从而 (ii)。

#### 注 {#ac-ii-s5-n6-rem-1 .statement tag=04C7}

命题 11 中 (i) 的证明仅使用$M$ 是平坦且非退化的事实。

### 7. 可逆模的类的群

（我们保留第5和第6号的记号。）

在乘法下，B形式的子A模是可交换幺半群$\mathfrak{m}$，其中A为单位元素。那么可逆的模是$\mathfrak{m}$的可逆元，因此形式是可交换的群$\mathfrak{z}$。我们已经看到 (no. 6, 命题 10) $M \in \mathfrak{z}$ 的逆是 $A : M$。

令$A^*$（或$B^*$）为A（或B）的可逆元的乘法群，并令$u$表示典范嵌入$A + B$。对于所有 $b \in B^*$，$\theta(b) = bA$ 是可逆子 A 模。 映射$\theta : B^* \to \mathfrak{g}$是同态，其核是$u(A^*)$；它的余核将由$\mathfrak{c}$或$\mathfrak{c}(A)$表示。 群$\mathfrak{c}$称为B的可逆子A模块的类的群。以下正合序列已构造

$$
\text{(10)} \quad (1) \longrightarrow A^* \xrightarrow{u} B^* \xrightarrow{\theta} \mathfrak{g} \xrightarrow{\rho} \mathfrak{c} \longrightarrow (1)
$$

其中（1）仅表示单位元素中的群由……组成，$\rho$是典范映射$\mathfrak{g} \to \mathfrak{c} = \mathfrak{g}/\theta(B^*)$。

由于 B 的每个可逆子 A 模 M 都是秩 1 (no. 6, 定理 4) 的投影，因此定义了元素 $cl(M) \in P(A)$ (no. 4)。

#### 命题 12 {#ac-ii-s5-prop-12 .statement tag=04C8}

*映射* $cl : \mathfrak{g} \to P(A)$ *定义，通过商，同构从* $\mathfrak{c} = \mathfrak{g}/\theta(B^*)$ *到核 of 典范同态*

$$
\phi : P(A) \to P(B)
$$

（no. 4）。

另外字，还有正合序列

$$
\text{(11)} \quad (1) \longrightarrow A^* \xrightarrow{u} B^* \xrightarrow{\theta} \mathfrak{g} \xrightarrow{cl} P(A) \xrightarrow{\phi} P(B).
$$

由$P(A)$中no. 6的命题11和加法的定义得出，$\mathbf{3}$中$M, N$的$cl(M.N) = cl(M) + cl(N)$，这表明$cl$是同态。如果$M \in \mathfrak{J}$与$A$同构的，则存在$b \in B$使得$M = Ab$，并且由于$M$是可逆的，所以存在$b' \in B$使得$b'b = 1$，在其他字$b$是可逆的$B$； 逆命题是直接的。因此，$\mathfrak{J}$中的$cl$的核是$\theta(B^*)$。

现在让我们计算$cl$的确定像。如果$M \in \mathfrak{J}$，则$M \otimes_A B = S^{-1}M = B$（no. 5，命题 8 (c)），从而$cl(M) \in \mathrm{Ker}(\phi)$。相反，令$P$为秩1的射影$A$模，使得$P_{(B)} = P \otimes_A B$与$B$同构于$B$。由于$P$是一个扁平的$A$模块，单射$u : A \to B$定义单射$u \otimes 1 : P \to P_{(B)} = B$和$P$因此被识别为$B$的子$A$模块；根据no. 5的命题 8 (c)，$P$是非简并的，并且no. 6的定理 4表明$P$是可逆的。因此，$\phi$的核等于$cl : \mathfrak{J} \to P(A)$的像。

#### 推论 1 {#ac-ii-s5-prop-12-cor-1 .statement tag=04C9}

*对于 B 的两个可逆子 A 模，在 $\mathfrak{C}$ 中具有相同的像，它们同构是充分必要的。*

#### 推论 2 {#ac-ii-s5-prop-12-cor-2 .statement tag=04CA}

*If the ring $B$ is semi-local, the group $\mathfrak{C}$ of classes of invertible sub-A-modules of B is canonically identified with the group $P(A)$ of classes of projective A-modules of rank 1.*

在这种情况下$P(B) = 0$（no. 3，命题5）。

#### 注 {#ac-ii-s5-n7-rem-1 .statement tag=04CB}

推论2的假设在以下两种情况下得到满足：

(1) $A$为整环且$S$为$A$元素$\neq 0$集合，$B$则为$A$分数域。在这种情况下，$B$的可逆子A模也称为*可逆分数理想*；那些单生自由$A$-模块$Ab$（$B$中的$b \# 0$）只是*代数*，章VI, § 1, no. 5中定义的*分数主理想*。

*(2)* 环 $A$ 是诺特，$S$ 是 $A$ 的元素的集合，它们不是 0 的除子，因此 $B$ 是分数的总和环 $A$。在这种情况下$S = A - \bigcup p_i$，其中$p_i$是$\mathrm{Ass}(A)$（章IV, § 1）的元素（数有限），因此$B$是半局部的（§ 3, no. 5，命题17）。*

### 习题{#ac-ii-s5-exercises}

§ 5](exercises/s5/)参见[习题。
