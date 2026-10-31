---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 5
section_title: Flatness properties of filtered modules
lang: zh
source: ac-i-vii
book_pages: 226-231, 259-260
pdf_pages: 0246-0251, 0279-0280
extraction: ocr
subsections:
    - "no": 1
      title: IDEALLY HAUSDORFF MODULES
      page: 226
      pdf_page: 246
    - "no": 2
      title: STATEMENT OF THE FLATNESS CRITERION
      page: 227
      pdf_page: 247
    - "no": 3
      title: PROOF OF THE FLATNESS CRITERION
      page: 228
      pdf_page: 248
    - "no": 4
      title: APPLICATIONS
      page: 230
      pdf_page: 250
statements: 11
exercises: 8
content_sha256: 2f99f1d9cd566ebb0cfbd9abc96a4aebc514544ab43656248e36f8d07f63e3ad
translated_from: content/en/ac/III/05_s5_flatness_properties_of_filtered_modules.md
translation_method: google
source_content_sha256: 40502ef62aacbf121ac1011abdbd0936abda1c04356f56a21967a20f392ffa93
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 392cc9231255dfbb3c8d2ccea0116f3c4f8a4b7624a69d6869d52f2fdf5de4b4
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 5. 过滤后的模的平整度特性

### 1. 理想的豪斯多夫模

#### 定义 1 {#ac-iii-s5-def-1 .statement tag=04IO}

*设 A 为交换环和 $\mathfrak{g}$ A 的理想。A-模 M 被称为关于 3 的理想 Hausdorff（或者如果没有歧义，则称为理想 Hausdorff），如果对于 A 的每个有限生成的理想 $\mathfrak{a}$，A-模 $\mathfrak{a} \otimes_A M$ 是具有 3-adic 的 Hausdorff 拓扑.*

将$\mathfrak{a} = A$放入定义，我们已经看到M必然是带有3进数拓扑的*Hausdorff*。

*例*

#### 例 1 {#ac-iii-s5-n1-exa-1 .statement tag=04IP}

如果 A 是诺特并且 $\mathfrak{g}$ 包含在 A 的 Jacobson 根式中（在其他字中，如果 A 是具有 3-adic 拓扑的 Zariski 环），则每个*有限生成的* A-模理想地是 Hausdorff (*§3*， no. 3、命题 6)。

#### 例 2 {#ac-iii-s5-n1-exa-2 .statement tag=04IQ}

理想 Hausdorff 模的每个直和都是理想 Hausdorff 模，凭借关系
$$
\mathfrak{g}^n \left( a \otimes_A \bigoplus_{\lambda \in L} M_\lambda \right) = \mathfrak{g}^n \bigoplus_{\lambda \in L} (a \otimes_A M_\lambda) = \bigoplus_{\lambda \in L} \mathfrak{g}^n (a \otimes_A M_\lambda).
$$

#### 例 3 {#ac-iii-s5-n1-exa-3 .statement tag=04IR}

如果 A-模 M 是平坦的，并且 Hausdorff 具有 $\mathfrak{g}$-adic 拓扑，那么它是理想的 Hausdorff，因为 $a \otimes_A M$ 则可与 M 的子模识别，并且 $a \otimes_A M$ 上的 $\mathfrak{g}$-adic 拓扑是更细拓扑由 M 上的 $\mathfrak{g}$-进数拓扑在 $a \otimes_A M$ 上诱导，即假设的豪斯多夫 (Hausdorff)。

### 2. 平坦度标准的叙述
令 A 为环，$\mathfrak{z}$ A 的双边理想，M 为左模，gr(A) 和 gr(M) 分别与环 A 和模 M 以及$\mathfrak{g}$-adic 过滤相关的分级环和分级 gr(A) 模块（§ 2, no. 3）。我们已经看到（前述）对于每个整数 $n \geq 0$ 都有一个满射 $\mathbf{Z}$-模同态
$$
\gamma_n : (\mathfrak{g}^n / \mathfrak{g}^{n+1}) \otimes_{A/\mathfrak{g}} (M / \mathfrak{g}M) \to \mathfrak{g}^n M / \mathfrak{g}^{n+1} M
$$
以及分级 gr(A) 模块的分级同态次数 0
$$
\gamma_M : \mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M) \to \mathrm{gr}(M)
$$
对于所有 $n$，其限制到 $\mathrm{gr}_n(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M)$ 是 $\gamma_n$，因此是满射的。

#### 定理 1 {#ac-iii-s5-thm-1 .statement tag=04IS}

设 A 为交换环，$\mathfrak{g}$ A 和 M A-模的理想。考虑以下属性：
(i) M 是 afat A-模。
(ii) 每 A-模 N 被 $\mathfrak{z}$ 消灭，$\mathrm{Tor}_1^A(N, M) = 0$。
(iii) $M / \mathfrak{g}M$ 是 ajlat $(A / \mathfrak{g})$ 模，典范映射 $\mathfrak{z} \otimes_A M \to \mathfrak{g}M$ 是双射（后者条件凭借关系 $\mathrm{Tor}_1^A(A, M) = 0$ 和正合序列等价于 $\mathrm{Tor}_1^A(A / \mathfrak{g}, M) = 0$）
$$
\mathrm{Tor}_1^A(A, M) \to \mathrm{Tor}_1^A(A / \mathfrak{g}, M) \to \mathfrak{z} \otimes_A M \to M ).
$$
(iv) $M / \mathfrak{g}M$ 是 ajlat $(A / \mathfrak{g})$ 模块且典范同态
$$
\gamma_M : \mathrm{gr}(A) \otimes_{\mathrm{gr}_0(A)} \mathrm{gr}_0(M) \to \mathrm{gr}(M)
$$
是双射 (性质 (GR) of § 2, no. 8)。
(v) 对于所有 $n \geq 1$，$M / \mathfrak{g}^n M$ 是一个平面 $(A / \mathfrak{g}^n)$ 模块。
然后 (i) $\Rightarrow$ (ii) $\Leftrightarrow$ (iii) $\Rightarrow$ (iv) $\Leftrightarrow$ (v)。
如果另外 $\mathfrak{g}$ 是幂零的，或者如果 A 是诺特并且 M 理想地是 Hausdorff，则性质 (i)、(ii)、(iii)、(iv) 和 (v) 是等价的。

#### 注 {#ac-iii-s5-n1-rem-1 .statement tag=04IT}

如果$A / \mathfrak{g}$是域（应用中经常发生）条件“M/$\mathfrak{g}M$是一个平面$(A / \mathfrak{g})$-模块”对于每个A-模M自动成立，这简化了属性（iii）和（iv）的叙述；此外，在这种情况下，性质 (v) 等价于说，$M / \mathfrak{g}^n M$ 是每个整数 $n \geq 1$ 的免费 $(A / \mathfrak{g}^n)$ 模块（章 11, § 3, no. 2，推论 2 为命题5)。

### 3. 平坦度标准的证明

(A) *影响* (i) $\Rightarrow$ (ii) $\Leftrightarrow$ (iii)

蕴涵 (i) $\Rightarrow$ (ii) 为直接的 (章 I, § 4)。 等价 (ii) $\Leftrightarrow$ (iii) 是章 I, § 4 的特例，命题 2 应用于 $R = A, S = A/\mathfrak{g}, F = M, E = N$，考虑到在 $N$ 上给出一个 $(A/\mathfrak{g})$ 模块结构相当于给出一个$A$-模块结构，其中$N$被3消灭。

*注* (1)。 条件 (ii) 也等价于：

(ii') $\operatorname{Tor}_1^A(N, M) = 0$ *对于每个* $A$*-模块* $N$ *被* 3的幂消灭。

显然 (ii') 意味着 (ii)。相反，如果 (ii) 成立，则特别是对于所有 $n$ $\operatorname{Tor}_1^A(\mathfrak{g}^n N / \mathfrak{g}^{n+1} N, M) = 0$； 正合序列起
$$
0 \to \mathfrak{g}^{n+1} N \to \mathfrak{g}^n N \to \mathfrak{g}^n N / \mathfrak{g}^{n+1} N \to 0
$$
我们得出正合序列
$$
\operatorname{Tor}_1^A(\mathfrak{g}^{n+1} N, M) \to \operatorname{Tor}_1^A(\mathfrak{g}^n N, M) \to \operatorname{Tor}_1^A(\mathfrak{g}^n N / \mathfrak{g}^{n+1} N, M)
$$
并且，由于存在整数$m$使得$\mathfrak{g}^m N = 0$，我们通过在$n$上降序归纳推导出所有$n \leq m$，特别是$n = 0$的$\operatorname{Tor}_1^A(\mathfrak{g}^n N, M) = 0$。

由此可见，如果 9 是 *幂幂*，(ii) 意味着 (i)，对于 (ii') 则意味着 $\operatorname{Tor}_1^A(N, M) = 0$ 对于 *每个* $A$*-模块* $N$，因此 $M$ 是平坦的 (章 I, § 4)。

(B) 让我们证明以下命题：

#### 命题 1 {#ac-iii-s5-prop-1 .statement tag=04IU}

*设*$A$*为交换环，3是*$A$*和*$M$*一个*$A$*-模*的理想。 *以下条件是等效的*：
(a) *对于所有人*$n \geq 1$，$\operatorname{Tor}_1^A(A/\mathfrak{g}^n, M) = 0$。
(b) *对于所有人* $n \geq 1$，*典范同态*
$$
\theta_n : \mathfrak{g}^n \otimes_A M \to \mathfrak{g}^n M
$$
*是双射的*。

*此外，这些条件意味着*：
(c) *典范同态* $\gamma_M : \operatorname{gr}(A) \otimes_{\operatorname{gr}_0(A)} \operatorname{gr}_r(M) \to \operatorname{gr}(M)$ *是双射*。 *相反，如果* $\mathfrak{g}$ *幂零，(c) 意味着 (a) 和 (b)*。

(a)和(b)的等价由正合序列推出
$$
0 = \operatorname{Tor}_1^A(A, M) \to \operatorname{Tor}_1^A(A/\mathfrak{g}^n, M) \to \mathfrak{g}^n \otimes_A M \to M.
$$

考虑下一步图表
$$
\begin{array}{ccccccccc}
\mathfrak{g}^{n+1} \otimes_A M & \longrightarrow & \mathfrak{g}^n \otimes_A M & \longrightarrow & (\mathfrak{g}^n / \mathfrak{g}^{n+1}) \otimes_A (M / \mathfrak{g} M) & \longrightarrow & 0 \\
\downarrow \theta_{n+1} & & \downarrow \theta_n & & \downarrow \gamma_n & & \\
0 & \longrightarrow & \mathfrak{g}^{n+1} M & \longrightarrow & \mathfrak{g}^n M & \longrightarrow & \operatorname{gr}_n(M) & \longrightarrow & 0
\end{array}
$$

其中注 $(\mathfrak{g}^n/\mathfrak{g}^{n+1}) \otimes_A (M/\mathfrak{g}M)$ 被规范地等同于 $(\mathfrak{g}^n/\mathfrak{g}^{n+1}) \otimes_{A/\mathfrak{g}} (M/\mathfrak{g}M)$。这个图表可以通过$\gamma_n$的定义交换，并且它的行是精确的。如果 (b) 成立，$0$ 和 $\theta_{n+1}$ 是双射的，因此是 $\gamma_n$ 乘以余核的定义，因此 (b) 蕴涵 (c)。相反，假设 $\mathfrak{g}$ 是幂零的，让我们证明 (c) 蕴涵 (b)；我们将通过从$n$下降归纳来论证，因为$\mathfrak{g}^n \otimes_A M = \mathfrak{g}^n M = 0$为$n$足够大。假设在图表 (1) 中，$\gamma_n$ 和 $\theta_{n+1}$ 是双射；那么$\theta_n$凭借章I, § 1, no. 4，推论1至命题2。

(C) *含义* (ii) $\Rightarrow$ (iv)

如果 (ii) 成立，则 (ii') 也成立 *注* 1； 命题 1 那么表明$\gamma_M$ 是同构。另一方面，我们已经知道 (ii) 蕴含 (iii)，因此 $M/\mathfrak{g}M$ 是一个扁平的 $(A/\mathfrak{g})$ 模块，它完成了 (ii) 蕴含 (iv) 的证明。

*注* (2)。 命题 1 表明，如果 $\mathfrak{g}$ 幂零，(iv) 蕴含 (iii)；考虑到*注* 1，我们因此在这种情况下证明了(i)、(ii)、(iii)和(iv)是等价的。

(D) *等价* (iv) $\Leftrightarrow$ (v)

对于所有 $n \geq 1$，$M/\mathfrak{g}^n M$ 具有规范的 $(A/\mathfrak{g}^n)$ 模块结构。如果通过$(\mathfrak{g}/\mathfrak{g}^n)$-adic过滤进行过滤，如果$m < n$则为$\mathrm{gr}_m(M/\mathfrak{g}^n M) = \mathrm{gr}_m(M)$，如果$m \geq n$则为$\mathrm{gr}_m(M/\mathfrak{g}^n M) = 0$，则为直接的。对于所有$k \geq 1$，设$A_k = A/\mathfrak{g}^k$，$\mathfrak{g}_k = \mathfrak{g}/\mathfrak{g}^k$，$M_k = M/\mathfrak{g}^k M$；设 (iv), (resp. $(v)_k$) 表示由 (iv) (resp. (v)) 通过替换 $A, \mathfrak{g}, M$ 通过 $A_k, \mathfrak{g}_k, M_k$ 导出的断言。由刚才可知，(iv)相当于“对于所有$k \geq 1$，$(iv)_k$”，显然(v)相当于“对于所有$k \geq 1$，$(v)_k$”。那么只要为所有$k$建立等价$(iv)_k \Leftrightarrow (v)_k$就足够了，或者还可以证明当$3$是*幂零*时(iv)$\Leftrightarrow$(v)。现在 (*注* 2) 我们已经看到，在这种情况下 (iv) 等价于 (i)。由于$M/\mathfrak{g}^n M$与$M \otimes_A (A/\mathfrak{g}^n)$同构的，(i) 蕴涵(v) (章I, § 2, no. 7，推论2至命题8)；此外，显然 (v) 意味着 (i)。因此，我们在所有情况下都显示了等价 (iv) $\Leftrightarrow$ (v)，并且在 $3$ 幂零的情况下也显示了定理的所有性质。

(E) *蕴含* (v) $\Rightarrow$ (i) *当* $A$ *为诺特且* $M$ *理想情况下 Hausdorff*

足以证明对于$A$典范映射$j : a \otimes_A M \to M$的每个理想$a$都是*内射*（章I, § 2, no. 3，命题1）。让$x \in \mathrm{Ker}\, j$；
$a \otimes_A M$ 是具有 $\mathfrak{g}$-adic 拓扑的 Hausdorff，足以验证对于每个整数 $n > 0$，$x \in \mathfrak{g}^n(a \otimes_A M)$。令$f : \mathfrak{g}^n a \to a$为典范嵌入；只要证明 $x \in \mathrm{Im}(f \otimes 1_M)$ 就足够了；因为如果$b \in \mathfrak{g}^n$，$a \in a$和$m \in M$，$f \otimes 1$下的像，$(\mathfrak{g}^n a) \otimes_A M$的元素$(ba) \otimes m$是$a \otimes_A M$的元素$(ba) \otimes m = b(a \otimes m)$，因此$\mathrm{Im}(f \otimes 1_M) \subset \mathfrak{g}^n(a \otimes_A M)$。根据克鲁尔的定理（§ 3, no. 2，定理2），存在整数$k$使得$a_j = a \cap \mathfrak{g}^k \subset \mathfrak{g}^n a$；如果$i : a_j \to a$是典范嵌入，那么就足以证明$x \in \operatorname{Im}(i \otimes 1_M)$。现在，用 $p : a \to a/a_k$ 和 $h : a/a_k \to A/\mathfrak{g}^k$ 典范映射表示，有一个可交换的图表

$$
\begin{array}{ccccccccc}
a_k \otimes_A M & \xrightarrow{i \otimes 1_M} & a \otimes_A M & \xrightarrow{p \otimes 1_M} & (a/a_k) \otimes_A M & \longrightarrow & 0 \\
& & \downarrow & & \downarrow h \otimes 1_M & & \\
& & M & \longrightarrow & (A/\mathfrak{g}^k) \otimes_A M & &
\end{array}
$$

其中第一行是准确的。只要证明 $x \in \operatorname{Ker}(p \otimes 1_M)$ 就足够了，并且，正如 $x \in \operatorname{Ker} j$ 乘以假设一样，也足以证明映射 $h \otimes 1_1$ 是单射的。现在，也可以写成（代数，章II, § 3, no. 6，推论3到命题6）

$$
h \otimes 1_{M/\mathfrak{g}^k M} : (a/a_k) \otimes_{A/\mathfrak{g}^k} (M/\mathfrak{g}^k M) \to M/\mathfrak{g}^k M
$$

并且，由于 $h$ 是单射的，并且根据 (v)，$M/\mathfrak{g}^k M$ 是平面 $(A/\mathfrak{g}^k)$ 模，因此完成证明。

### 4. 应用

#### 命题 2 {#ac-iii-s5-prop-2 .statement tag=04IV}

令$A$为交换环，$\mathfrak{g}$为$A$的理想，$B$为可交换的诺特$A$代数，使得$B$包含在$B$的雅各布森根式中。那么每个有限生成的$B$-模$M$都是关于$\mathfrak{g}$的理想Hausdorff$A$-模。

我们将更普遍地看到，对于每个有限生成的$A$-模$N$，$N \otimes_A M$是具有$3$-adic拓扑的Hausdorff。因为$N_{(B)} = N \otimes_A B$是有限生成的$B$模块，而$B$模块$N \otimes_A M$凭借张量积的结合性被规范地标识为$N_{,,} \otimes_B M$。令$\mathfrak{L}$为$B$的雅各布森根式；由于$\mathfrak{g} B$包含在$\mathfrak{L}$中，因此$N \otimes_A M$上的$\mathfrak{g}$-adic 拓扑比$N_{(B)} \otimes_B M$上的$\mathfrak{L}$-adic 拓扑更容易被识别为更细拓扑；但后者拓扑是Hausdorff，因为$N_{,,} \otimes_B M$是有限生成的$B$模（no. 1，例1），从而结论。

#### 命题 3 {#ac-iii-s5-prop-3 .statement tag=04IW}

令$A$为交换环，$B$为可交换的$A$代数，$\mathfrak{g}$为$A$的理想，$M$为$B$模。假设 $B$ 是诺特环和一个平坦的 $A$ 模，并且 $M$ 相对于 $\mathfrak{g} B$ 是理想的 Hausdorff。以下条件是等效的：
(a) $M$ 是扁平 $B$ 模块。
(b) $M$ 是扁平 $A$ 模块，$M/\mathfrak{g} M = M/(\mathfrak{g} B) M$ 是扁平 $(B/\mathfrak{g} B)$ 模块。
如果进一步典范同态 $A/\mathfrak{g} \to B/\mathfrak{g} B$ 是双射，条件 (a) 和 (b) 也等价于：
(c) $M$ 是一个扁平的 $A$ 模块。

条件 (a) 通过章 I, §2, no. 7 隐含 (b)，推论 2 和 3 到命题 8 并且$M/\mathfrak{g} M$ 同构于 $M \otimes_B (B/\mathfrak{g} B)$。假设条件 (b) 成立；为了证明$M$是一个扁平的$B$模块，我们将no. 2中的应用定理 1，其中$A$替换为$B$，$\mathfrak{g}$替换为$\mathfrak{g} B$。因此，只要证明典范映射 $f : \mathfrak{J}B \otimes_B M \to \mathfrak{J}M$ 是单射的就足够了。令$f_1$为典范映射$\mathfrak{J} \otimes_A B \to \mathfrak{J}B$，$f_2$典范同构$\mathfrak{J} \otimes_A M \to (\mathfrak{J} \otimes_A B) \otimes_B M ; f \circ (f_1 \circ 1_M) \circ f_2$为典范映射$f' : \mathfrak{J} \otimes_A M \to \mathfrak{J}M$，这很容易验证。现在$f'$是同构，因为$M$是一个平坦的$A$模块，而$f_1$是同构，因为$B$是平坦的，$A ; f$是同构。

设$p : A/\mathfrak{J} \to B/\mathfrak{J}B$为典范同态； $M/\mathfrak{J}M$上的$(A/\mathfrak{J})$模块结构通过$p$从其$(B/\mathfrak{J}B)$模块结构导出，与$M \otimes_A (A/\mathfrak{J})$上的同构。那么，如果$M$是一个扁平的$A$模块，那么$M/\mathfrak{J}M$是一个扁平的$(A/\mathfrak{J})$模块，因此如果$p$是同构，那么它也是一个扁平的$(B/\mathfrak{J}B)$模块；因此，我们在这种情况下证明了 (c) $\Rightarrow$ (b)。

#### 推论{#ac-iii-s5-n4-cor-1 .statement tag=04IX}

*令 $A$ 为可交换的诺特环，$\mathfrak{J}$ $A$、$\hat{A}$ $A$ 相对于 $\mathfrak{J}$-adic 拓扑的 Hausdorff 完成，并且$M$ 相对于 $\mathfrak{J} \hat{A}$ 的理想 Hausdorff $\hat{A}$ 模。为了使 $M$ 成为扁平 $A$ 模块，$M$ 成为扁平 $\hat{A}$ 模块是必要且充分的。*

事实上我们知道$\hat{A}$是诺特环（$§ 3$，编号**4**，命题8）和一个扁平的$A$模块（$§ 3$，编号**4**，定理3），即$\mathfrak{J} \hat{A} = \hat{\mathfrak{J}}$ ($§ 2$, no. 12, 命题 **16**) 并且典范同态 $A/\mathfrak{J} \to \hat{A}/\hat{\mathfrak{J}}$ 是双射 ($§ 2$, no. 12, 命题 15);因此可以应用命题 **3**。

#### 命题 4 {#ac-iii-s5-prop-4 .statement tag=04IY}

*设$A$和$B$是两个可交换的诺特环，$h : A \to B$环同态，$3$$A$的理想和$2$$B$的理想包含 $\mathfrak{J}B$ 并包含在 $B$ 的雅各布森根中。令$\hat{A}$为$A$相对于$3$-adic 拓扑的豪斯多夫完成，$\hat{B}$为$B$相对于$2$-adic 拓扑的豪斯多夫完成； $h$ 与这些拓扑连续，因此 $h : \hat{A} \to \hat{B}$ 使 $\mathbf{8}$ 成为 $\hat{A}$ 代数。令 $M$ 为有限生成的 $B$-模，$\hat{M}$ 为相对于 $2$-adic 拓扑的 Hausdorff 补全；以下属性是等效的：
(a) $M$ 是扁平 $A$ 模块。
(b) $\hat{M}$ 是扁平 $A$ 模块。
(c) $\hat{M}$ 是一个扁平的 $\hat{A}$ 模块。*

由于 $B$ 和 $2$-adic 拓扑是 Zariski 环，$\hat{B}$ 是一个忠实的扁平 $B$ 模块（$§ 3$、no. 5、命题 9），$M$ 是规范同构的至$M \otimes_B \hat{B}$（$§ 3$，第**4**，定理3）；立即验证该典范同构是$\hat{M}$上的$A$模块结构的同构到源自$M$上的$M \otimes_B \hat{B}$上的$A$模块结构。 应用命题 4 个章 I、$§ 3$、no. 2，其中 $R$ 替换为 $B$，$S$ 替换为 $A$，$E$ 替换为$\hat{B}$、$F$和$M$，我们看到$M$是一个扁平的$A$模，$\hat{M}$是一个扁平的$A$模是充分必要的。此外，$\hat{M}$是有限生成的$\hat{B}$模，$\mathfrak{J} \hat{B}$包含在$\mathfrak{Q} = \mathfrak{Q} \hat{B}$中，因此包含在$\hat{B}$的Jacobson根式中（$§ 3$，编号**4**，命题8）；因此 $\hat{M}$ 是关于 $\mathfrak{J} \hat{A}$ (命题 2) 的理想 Hausdorff $A$ 模。因此，根据推论，条件 (b) 和 (c) 等价于命题 3。

### 习题 {#ac-iii-s5-exercises}

§ 5](exercises/s5/)参见[习题。
