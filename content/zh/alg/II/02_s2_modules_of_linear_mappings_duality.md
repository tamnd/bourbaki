---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 2
section_title: Modules of linear mappings. Duality
lang: zh
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 227-243, 386-395
pdf_pages: 0251-0267, 0410-0419
extraction: ocr
subsections:
    - "no": 1
      title: PROPERTIES OF $\mathrm{Hom}_A(E, F)$ RELATIVE TO EXACT SEQUENCES
      page: 227
      pdf_page: 251
    - "no": 2
      title: PROJECTIVE MODULES
      page: 231
      pdf_page: 255
    - "no": 3
      title: LINEAR FORMS; DUAL OF A MODULE
      page: 232
      pdf_page: 256
    - "no": 4
      title: ORTHOGONALITY
      page: 234
      pdf_page: 258
    - "no": 5
      title: TRANSPOSE OF A LINEAR MAPPING
      page: 234
      pdf_page: 258
    - "no": 6
      title: DUAL OF A QUOTIENT MODULE. DUAL OF A DIRECT SUM. DUAL BASES
      page: 236
      pdf_page: 260
    - "no": 7
      title: BIDUAL
      page: 239
      pdf_page: 263
    - "no": 8
      title: LINEAR EQUATIONS
      page: 240
      pdf_page: 264
statements: 42
exercises: 26
content_sha256: 05ffa52ee5925c951f9d50dc433b7be8fe2efc61140b64600aa3639472a69d07
translated_from: content/en/alg/II/02_s2_modules_of_linear_mappings_duality.md
translation_method: google
source_content_sha256: b68d6b666aad78a9fe6c8ac80cb610da120336ed9a4c3178da2cb94e6cf08597
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-39653cda
glossary_version: 34
glossary_terms_sha256: 12d5a2ebfd417633baffc020d75b2bc66864efa07b13018a671891ffb4c5275a
prompt_sha256: 7fdd4e0b5e6067ff04498ebe670ef3580d6ba9506bf4d0c582d73af15fd73ef3
---

## § 2。 模线性映射。二元性

### 1. $\mathrm{Hom}_A(E, F)$ 相对于正合序列的性质

#### 定理 1 {#alg-ii-s2-thm-1 .statement tag=05MV}

*设 A 为环、E'、E、E'' 三个 A-模，u : E' \to E, v : E \to E'' 两个同态。 序列*

$$
\text{(1)} \quad E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

*准确地说，对于每个 A-模 F，序列* 是充分必要的

$$
\text{(2)} \quad 0 \longrightarrow \mathrm{Hom}(E'', F) \xrightarrow{\bar{v}} \mathrm{Hom}(E, F) \xrightarrow{\bar{u}} \mathrm{Hom}(E', F)
$$

（其中$\bar{u} = \mathrm{Hom}(u, 1_F)$，$\bar{v} = \mathrm{Hom}(v, 1_F)$）*准确*。

假设序列 (1) 是精确的。如果 $w \in \mathrm{Hom}(E'', F)$ 和 $\bar{v}(w) = w \circ v = 0$，则 $w = 0$ 因为 $v$ 是满射。因此，序列 (2) 精确为 $\mathrm{Hom}(E'', F)$。我们证明它在 $\mathrm{Hom}(E, F)$ 处是精确的。 $\bar{u} \circ \bar{v} = \mathrm{Hom}(v \circ u, 1_F)$ (§ 1, no. 2, 公式 (10)) 和 $v \circ u = 0$，因为序列 (1) 在 E 处精确。因此 $\bar{u} \circ \bar{v} = 0$，即 $\mathrm{Im}(\bar{v}) \subset \mathrm{Ker}(\bar{u})$。另一方面，如果$w \in \mathrm{Ker}(\bar{u})$，则$w \circ u = 0$，因此$\mathrm{Ker}(w) \supset \mathrm{Im}(u)$。但由于序列 (1) 在 E 处精确，$\mathrm{Im}(u) = \mathrm{Ker}(v)$ 因此为 $\mathrm{Ker}(w) \supset \mathrm{Ker}(v)$；由于 $v$ 是满射，因此从 § 1, no. 3, *注* 可以得出，存在一个 $w' \in \mathrm{Hom}(E'', F)$ 使得 w = w' \circ v = \bar{v}(w')。因此 Ker(\bar{u}) \子集 \operatorname{Im}(\bar{v}) 完成证明序列 (2) 是精确的。

相反，假设 (2) 对于每个 A-模 F 都是精确的。对于每个同态 $w : E'' \to F$，$\bar{u} \circ \bar{v} = \operatorname{Hom}(v \circ u, 1_F) = 0, w \circ v \circ u = 0$ 都是精确的。取$F = E''$和$w = 1_{E''}$，首先看到$v \circ u = 0$，因此$u(E') \subset \operatorname{Ker}(v)$。现在取$F = \operatorname{Coker}(u)$，令$\phi : E \to F = E/u(E')$为典范映射。然后$\bar{u}(\phi) = \phi \circ u = 0$乘以定义，因此存在$\psi \in \operatorname{Hom}(E'', F)$使得$\phi = \bar{v}(\psi) = \psi \circ v$；这显然隐含了$u(E') = \operatorname{Ker}(\phi) \supset \operatorname{Ker}(v)$，从而证明序列(1)在E处精确。最后，令$\theta$为$E''$的典范同态到$F = E''/v(E)$；那么$\bar{v}(\theta) = \theta \circ v = 0$，因此$\theta = 0$；因此，$F = \{0\}$和$v$是满射的。因此，序列 (1) 精确为 $E''$。

#### 推论 {#alg-ii-s2-n1-cor-1 .statement tag=05MW}

*对于A-线性映射* $u : E \to F$ *为满射*（分别为*双射的*，分别为*零*），*对于每个A-模 G，映射* $\operatorname{Hom}(u, 1_G) : \operatorname{Hom}(F, G) \to \operatorname{Hom}(E, G)$ *为单射*（分别为*双射的*，分别为*零*），这是必要且充分的*零*）。

对于$E'' = \{0\}$（分别为$E' = \{0\}$、$E'' = E$ 和$v = 1_E$）的情况，应用定理 1 就足够了。

注从正合序列开始

$$
0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

相应的序列

$$
0 \longrightarrow \operatorname{Hom}(E'', F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F) \xrightarrow{\bar{u}} \operatorname{Hom}(E', F) \longrightarrow 0
$$

*不一定是精确的*，在其他字，同态$\bar{u}$不一定是满射的。如果 $E'$ 与 E 的子模相同，这意味着 $E'$ 的线性映射到 F 不能总是扩展到 E 的线性映射到 F（习题 11 和 12）。然而：

#### 命题 1 {#alg-ii-s2-prop-1 .statement tag=05MX}

*如果正合序列 / 线性映射*

(3)
$$
0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

*分裂的*（在其他字中，如果$u(E')$是E的*直因子*）*序列*

(4)
$$
0 \longrightarrow \operatorname{Hom}(E'', F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F) \xrightarrow{\bar{u}} \operatorname{Hom}(E', F) \longrightarrow 0
$$

*准确且分裂的*。 *相反，如果对于每个 A-模 F，序列 (4) 都是精确的，序列 (3) 分裂的*。

如果正合序列 (3) 分裂的，则存在与 $u$ (§ 1, no. 9，命题 15) 相关的线性回缩$u' : E \to E'$；如果

$$
\bar{u}' = \operatorname{Hom}(u', 1_F) : \operatorname{Hom}(E', F) \to \operatorname{Hom}(E, F),
$$

$u' \circ u$ 是恒等式意味着 $\bar{u} \circ \bar{u}'$ 是恒等式 ($§ 1$, no. 2, 公式 (10))，因此第一个断言是从 $§ 1$, no. 9, 命题 15 得出的。相反，假设序列 (4) 与 $F = E'$ 完全相同。则存在元素$f \in \mathrm{Hom}(E, E')$使得$f \circ u = 1_{E'}$，由$§ 1$、no. 9、命题15得出结论。

注，命题 1 的第一个断言也可以被视为$§ 1$、no. 6的特例，推论 1 到命题 6，通过$\mathbf{Z}$线性映射将$\mathrm{Hom}(E', F) \oplus \mathrm{Hom}(E'', F)$与$\mathrm{Hom}(E' \oplus E'', F)$规范地识别$\mathrm{Hom}(p', 1_F) + \mathrm{Hom}(p'', 1_F)$，其中$p': E' \oplus E'' \to E'$和$p'': E' \oplus E'' \to E''$是规范的投影。

#### 定理 2 {#alg-ii-s2-thm-2 .statement tag=05MY}

*令$A$为环，$F', F, F''$三个$A$模块和$u: F' \to F, v: F \to F''$两个同态。 序列*

$$
0 \longrightarrow F' \xrightarrow{v} F \xrightarrow{u} F''
$$

*准确地说，对于每个$A$-模块$E$，序列是必要且充分的*

$$
0 \longrightarrow \mathrm{Hom}(E, F') \xrightarrow{\bar{u}} \mathrm{Hom}(E, F) \xrightarrow{\bar{v}} \mathrm{Hom}(E, F'')
$$

*（其中 $\bar{u} = \mathrm{Hom}(1_E, u), \bar{v} = \mathrm{Hom}(1_E, v)$）准确地说。*

假设序列 (5) 是精确的。 注首先

$$
\bar{v} \circ \bar{u} = \mathrm{Hom}(1_E, v \circ u) = 0
$$

（II、$§ 1$、no. 2、公式 (10)）自 $v \circ u = 0$ 起。因此，$\bar{u}$下的$\mathrm{Hom}(E, F')$的像包含在$\bar{v}$的核$N$中；令$f$为$\mathbf{Z}$模块$\mathrm{Hom}(E, F')$的同态进入$N$，其图等于$\bar{u}$的图；有必要证明$f$是*双射的*，因此定义映射$g: N \to \mathrm{Hom}(E, F')$使得$f \circ g$和$g \circ f$是恒等映射。为此，令$w$为$N$的元素，即线性映射$w: E \to F$使得$v \circ w = 0$。后者关系通过假设等价于$w(E) \subset \mathrm{Ker}(v) = u(F')$，因此，由于$u$是单射的，因此存在且仅有一个线性映射$w': E \to F'$，使得$w = u \circ w'$和我们取$g(w) = w'$；立即验证$g$满足所需的条件。

相反，假设序列 (6) 对于每个 $A$-模块 $E$ 都是精确的。作为$\mathrm{Hom}(1_E, v \circ u) = \bar{v} \circ \bar{u} = 0$，那么对于每个同态$w: E \to F'$，$v \circ u \circ w = 0$。取$E = F'$和$w = 1_{F'}$，首先看到$v \circ u = 0$，因此$u(F') \subset \mathrm{Ker}(v)$。现在我们取 $E = \mathrm{Ker}(v)$ 并令 $\phi: E \to F$ 为典范嵌入。那么$\bar{v}(\phi) = v \circ \phi = 0$乘以定义，因此存在$\psi \in \mathrm{Hom}(E, F')$使得$\phi = \bar{u}(\psi) = u \circ \psi$，这显然意味着$\mathrm{Ker}(v) \subset u(F')$并且在$F$处完成了(5)的精确性的证明。最后，如果$\theta$是$\mathrm{Ker}\, u$的恒等映射，则$\bar{u}(\theta) = 0$，因此$\theta = 0$和$\mathrm{Ker}\, u = \{0\}$，这证明了（5）在$F'$处的正确性。

#### 注 {#alg-ii-s2-n1-rem-1 .statement tag=05MZ}

(1) 定理 2 允许我们对于 F 的每个子模 F'，通过 Hom(E, F) 的子 $\mathbf{Z}$ 模到认同 Hom(E, F')。当进行此识别时，对于 F 的子模的每个家庭 $(M_\lambda)$

$$
\operatorname{Hom}(E, \bigcap_\lambda M_\lambda) = \bigcap_\lambda \operatorname{Hom}(E, M_\lambda)
$$

因为如果$u \in \operatorname{Hom}(E, F)$属于到每个$\operatorname{Hom}(E, M_\lambda)$，那么，对于所有$x \in E$，$u(x) \in M_\lambda$对于所有$\lambda$，因此$u$映射E到$\bigcap_\lambda M_\lambda$。

#### 推论{#alg-ii-s2-n1-cor-2 .statement tag=05N0}

*对于A-线性映射* $u : E \to F$ *是单射的，对于每个A-模 G，映射* $\operatorname{Hom}(1_G, u) : \operatorname{Hom}(G, E) \to \operatorname{Hom}(G, F)$ *是单射的*是必要且充分的。

对于$F' = \{0\}$的情况，应用定理2就足够了。

从正合序列开始

$$
0 \longrightarrow F' \xrightarrow{u} F \xrightarrow{v} F'' \longrightarrow 0
$$

相应的序列

$$
0 \longrightarrow \operatorname{Hom}(E, F') \xrightarrow{\bar{u}} \operatorname{Hom}(E, F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F'') \longrightarrow 0
$$

*不一定是精确的*，在其他字$\bar{v}$不一定是满射的。如果$F'$与$F$的子模识别，$F''$与商模$F/F'$识别，这意味着$E$的线性映射进入$F''$不一定是形式$v \circ w$，其中$w$是$E$到$F$的线性映射。然而：

#### 命题 2 {#alg-ii-s2-prop-2 .statement tag=05N1}

*如果正合序列*

(7)

$$
0 \longrightarrow F' \xrightarrow{u} F \xrightarrow{v} F'' \longrightarrow 0
$$

*分裂的*（在其他字中，如果$u(F')$是$F$的*直因子*），*序列*

(8)

$$
0 \longrightarrow \operatorname{Hom}(E, F') \xrightarrow{\bar{u}} \operatorname{Hom}(E, F) \xrightarrow{\bar{v}} \operatorname{Hom}(E, F'') \longrightarrow 0
$$

*准确且分裂的*。 *相反，如果序列* (8) *对于每个A-模 E 都是精确的，正合序列* (7) *分裂的*。

第一个断言源自以下事实：

$$
\operatorname{Hom}(E, F') \oplus \operatorname{Hom}(E, F'')
$$

通过$\mathbf{Z}$线性映射$\operatorname{Hom}(1_E, j') + \operatorname{Hom}(1_E, j''), j' : F' \to F' \oplus F''$和$j'' : F'' \to F' \oplus F''$为典范嵌入（§ 1, no. 6，推论1到命题6），被规范地识别为$\operatorname{Hom}(E, F' \oplus F'')$。相反，如果序列 (8) 对于 $E = F''$ 是精确的，则存在元素 $g \in \operatorname{Hom}(F'', F)$，使得 $v \circ g = 1_{F''}$ 且结论由 § 1, no. 9、命题 15 得出。

注 (2)。这个结果没有。对于所有带有运算符的可交换群都是有效的，无需修改。

### 2.投射模

#### 定义 1 {#alg-ii-s2-def-1 .statement tag=05N2}

A-模 P 称为射影，如果对于 A-线性映射的每个正合序列 F' → F → F''，序列

$$
\operatorname{Hom}(P, F') \to \operatorname{Hom}(P, F) \to \operatorname{Hom}(P, F'')
$$

是准确的。

#### 命题 3 {#alg-ii-s2-prop-3 .statement tag=05N3}

对于子模 (M_i) 族中的 A-模 P、直和来说，要投影，每个 M_i 都是投影的充分必要。

对于每个 A-模同态 u : E → F，

$$
\operatorname{Hom}(1_P, u) : \operatorname{Hom}(P, E) \to \operatorname{Hom}(P, F)
$$

被识别为$\prod_i \operatorname{Hom}(1_{M_i}, u)$（§ 1, no. 6，推论1到命题6）；由此得出定义 1 和§ 1, no. 5、命题 5 (ii) 的结论。

#### 推论{#alg-ii-s2-n2-cor-1 .statement tag=05N4}

每个自由A-模都是投影。

通过命题 3 就足以证明 A_s 是射影的，它紧随 § 1, no. 14 的图表 (50) 的交换律而来。

#### 命题 4 {#alg-ii-s2-prop-4 .statement tag=05N5}

令 P 为 A-模。以下属性是等效的：

(a) P 是投影。
(b) 对于 A-线性映射中的每个正合序列 0 → F' → F → F'' → 0，序列

$$
0 \to \operatorname{Hom}(P, F') \to \operatorname{Hom}(P, F) \to \operatorname{Hom}(P, F'') \to 0
$$

是准确的。

(c) 对于每个满射 A-模同态 u : E → E'' 和每个同态 f : P → E''，存在同态 g : P → E 使得 f = u ∘ g （据说 f 可以“提升”到 P 的同态到 E）。

(d) A-线性映射分裂的的每个正合序列 0 → E' → E → P → 0 （因此 P 与 E 的直因子同构）。

(e) P 同构于直因子或自由A-模。

(a) 暗示(b) 是微不足道的。要看出 (b) 蕴含 (c)，只需将 (b) 应用于正合序列 0 → E' → E → E'' → 0，其中 E' = Ker(u)，因为 (c) 表达了以下事实：

$$
\operatorname{Hom}(1_P, u) : \operatorname{Hom}(P, E) \to \operatorname{Hom}(P, E'')
$$

是主观的。为了看出(c)蕴含(d)，只需将(c)应用于满同态$v : E \to P$和同态$l_P : P \to P$即可； 同态 $g : P \to E$ 的存在使得 $l_P = v \circ g$ 意味着序列

$$
0 \longrightarrow E' \longrightarrow E \xrightarrow{v} P \longrightarrow 0
$$

分裂的（§ 1, no. 9，命题15）。对于每一个A-模 M，都存在自由A-模 L 和正合序列 $0 \to R \to L \to M \to 0$（§ 1, no. 11，命题 20），显然（d）蕴含（e）。最后，(e) 凭借命题 3 及其推论意味着 (a)。

#### 推论 1 {#alg-ii-s2-prop-4-cor-1 .statement tag=05N6}

*为了使A-模是射影且有限生成的，它是自由A-模的直因子以及有限的基是必要且充分的。*

条件显然就足够了；反之，有限生成射影模 E 同构于自由模 F 与有限基 (§ 1, no. 11) 的商，并且 E 通过命题 4 (d) 同构于 F 的直因子。

#### 推论 2 {#alg-ii-s2-prop-4-cor-2 .statement tag=05N7}

*设C为交换环，E、F为两个有限生成射影C-模；那么$\operatorname{Hom}_C(E, F)$是有限生成的射影C-模。*

可以假设有两个有限生成的空闲C-模M，N使得$M = E \oplus E', N = F \oplus F'$；从 § 1, no. 6，推论 1 到命题 6，$\operatorname{Hom}_C(M, N)$ 是有限生成且自由的，另一方面，$\operatorname{Hom}_C(M, N)$ 同构于

$$
\operatorname{Hom}_C(E, F) \oplus \operatorname{Hom}_C(E', F) \oplus \operatorname{Hom}_C(E, F') \oplus \operatorname{Hom}(E', F'),
$$

从而推论。

### 3.线性形式;双模

令 E 为 *左* A-模。由于 A 是 (A, A) 双模，$\operatorname{Hom}_A(E, A_s)$ 具有规范的*右* A-模结构 (§ 1, no. 14)。

#### 定义 2 {#alg-ii-s2-def-2 .statement tag=05N8}

*对于每个右A-模 E，右A-模 $\operatorname{Hom}_A(E, A_s)$ 被称为 E* 的对偶模（或简称为 E 的*对偶†*）*及其元素被称为 E* 上的线性形式。

如果 E 是 *右* A-模，则集合 $\operatorname{Hom}_A(E, A_d)$ 及其规范的 *左* A-模结构同样被称为 E 的 *对偶*，其元素被称为 E 上的 *线性形式*。

† 在*拓扑向量空间*，IV 中，我们将定义，对于向量空间，以及“对偶空间”的*拓扑*、概念，这将取决于此拓扑，并且与此处定义的不同。读者必须小心地小心应用到“拓扑”对偶空间本段中建立的“代数”对偶的属性。

在这个章中，$E^*$将用于表示（左或右）A-模$E$的对偶。

#### 例 {#alg-ii-s2-n3-exa-1 .statement tag=05N9}

*在向量空间（相对于域$\mathbf{R}$）连续实值函数上，$[a, b]$为$\mathbf{R}$，映射$x \mapsto \int_a^b x(t) dt$为线性形式。*

设$E$为左A-模，$E^*$为它的对偶；对于元素$x \in E, x^* \in E^*$的每个有序对，A的元素$x^*(x)$用$\langle x, x^* \rangle$表示。然后关系

$$
\begin{align*}
(9) \quad & \langle x + y, x^* \rangle = \langle x, x^* \rangle + \langle y, x^* \rangle \\
(10) \quad & \langle x, x^* + y^* \rangle = \langle x, x^* \rangle + \langle x, y^* \rangle \\
(11) \quad & \langle \alpha x, x^* \rangle = \alpha \langle x, x^* \rangle \\
(12) \quad & \langle x, x^* \alpha \rangle = \langle x, x^* \rangle \alpha
\end{align*}
$$

在$E, x^*, y^*$、$E^*$和$\alpha \in A$中保持$x, y$。 $E \times E^*$的映射$(x, x^*) \mapsto \langle x, x^* \rangle$到$A$称为$E \times E^*$上的规范双线性形式（双线性形式的概念一般会在IX, § 1中定义）。 $E$上的每个线性形式$x^*$都可以被视为规范双线性形式的部分映射$x \mapsto \langle x, x^* \rangle$相应的。

当$E$为右A-模时，元素$x \in E$处的线性形式$x^* \in E^*$的值$x^*(x)$记为$\langle x^*, x \rangle$，公式相应的则将(11)、(12)分别写为

$$
\begin{align*}
\langle x^*, x \alpha \rangle &= \langle x^*, x \rangle \alpha \\
\langle \alpha x^*, x \rangle &= \alpha \langle x^*, x \rangle.
\end{align*}
$$

当 A 是可交换的时，记号是允许的。

#### 命题 5 {#alg-ii-s2-prop-5 .statement tag=05NA}

对于每个环 A，与$A_s$上的每个$\xi \in A$线性形式$\eta \mapsto \eta \xi$相关联的映射是$A_d$的同构到$A_s$的对偶上。

这是§ 1, no. 14、注 2、相应的到$E = A_s$的典范同构$E \to \mathrm{Hom}_A(A_s, E)$的特例； § 1, no. 14的图表（50）交换律，表明我们这里有右A-模的同构。

如果通过命题 5的同构将$A_d$与$A_s$的对偶进行识别，则$A_s \times A_d$上的规范双线性形式可表示为

$$
\langle \xi, \xi^* \rangle = \xi \xi^* \quad \text{for } \xi, \xi^* \text{ in } A.
$$

类似地，$A_d$ 的对偶被规范地等同于 $A_s$，$A_d \times A_s$ 上的规范双线性形式被表达为

$$
\langle \xi^*, \xi \rangle = \xi^* \xi \quad \text{for } \xi, \xi^* \text{ in } A.
$$

### 4. 正交性

#### 定义 3 {#alg-ii-s2-def-3 .statement tag=05NB}

设 E 为 A-模，E* 为对偶；如果 ⟨x, x*⟩ = 0，则元素 x ∈ E 和元素 x* ∈ E* 称为正交。

E 的子集 M 和 E* 的子集 M' 被称为正交集合如果对于所有 x ∈ M，x* ∈ M'，x 和 x* 是正交的。 特别地，x* ε E*（分别x ε E）被称为与M（分别X）正交。 M') 如果它与 M 的每个元素正交（分别为 M'）。 如果 x* 和 y* 与 M 正交，则根据 (10) 和 (12) (no. 3)，对于所有 α ∈ A，x* + y* 和 x*α 也与 M 正交，这证明了以下定义：

#### 定义 4 {#alg-ii-s2-def-4 .statement tag=05NC}

给定 E 的子集 M（或 E* 的子集 M'），x* ∈ E* 的集合（x ∈ E 的集合）与 M（或 M'）正交，称为子模与 M（或 M'）完全正交（或简称子模）如果不会引起混淆，则与 M 正交（分别为 M'）。

通过线性形式的定义，与E正交的E*的子模减为0； E* 与 {0} 正交的子模与 E* 相同。

#### 命题 6 {#alg-ii-s2-prop-6 .statement tag=05ND}

令 M、N 为 E 的两个子集，使得 M ⊂ N；如果M'和N'分别是与M和N正交的E*的子模，则N'⊂M'。

#### 命题 7 {#alg-ii-s2-prop-7 .statement tag=05NE}

设(M_i)为E的子集族；与M_i的并正交的子模是分别与M_i正交的子模M'_i的交；这个子模也是子模正交于由M_i的并生成的E的子模。

这些结果是直接的推论或定义。

对于 E 的子模与 E* 的子集正交，有一个类似的命题（我们将留给读者说明）。

如果 M 是 E 的子模，M' 是与 M 正交的 E* 的子模，并且 E 的 M'' 子模与 M' 正交，则 M ⊂ M'' 但也可能是 M ≠ M'' (习题 9)。 注然而，如果 M'' 是 E* 中 M'' 的正交，则 M'' = M'；对于 M' ⊂ M'' 并且另一方面关系 M ⊂ M'' 意味着 M'' ⊂ M'。

### 5. 转置的线性映射

设E、F为两个左A-模；对于每个线性映射 u : E → F，映射 Hom(u, l_{A_s}) 是右A-模 F* 的线性映射到右A-模 E* (§ 1, no. 2)，称为 u 的转置。

在其他字中：

#### 定义 5 {#alg-ii-s2-def-5 .statement tag=05NF}

对于A-模 E 的每个线性映射 u 到 A-模 F，F 的对偶 F* 的线性映射 y* ↦ y* ∘ u 到 E 的对偶 E* 称为 u 的转置，并用 tu 表示。

因此转置 $^t u$ 由关系定义
(15) $$
\langle u(x), y^* \rangle = \langle x, ^t u(y^*) \rangle \quad \text{for all } x \in E \text{ and all } y^* \in F^*.
$$

定义 5 在不改变右A-模的情况下适用，然后相当于关系
$$
\langle y^*, u(x) \rangle = \langle ^t u(y^*), x \rangle \quad \text{for all } x \in E \text{ and all } y^* \in F^*.
$$

公式 § 1, no. 2 的 (9) 和 (10) 给出
(16) $$
^t(u_1 + u_2) = ^t u_1 + ^t u_2
$$
对于 $\mathrm{Hom}_A(E, F)$ 中的两个元素 $u_1, u_2$ 和
(17) $$
^t(v \circ u) = ^t u \circ ^t v
$$
对于$u \in \mathrm{Hom}_A(E, F)$和$v \in \mathrm{Hom}_A(F, G)$，G是第三个A-模；最后，显然地
(18) $$
^t 1_E = 1_{E^*}.
$$

#### 注 {#alg-ii-s2-n5-rem-1 .statement tag=05NG}

从 (17) 和 (18) 可以看出，如果 $u$ 是左（或右）可逆的，则 $^t u$ 是右（或左）可逆的。

#### 命题 8 {#alg-ii-s2-prop-8 .statement tag=05NH}

*设$u : E \to F$为A-线性映射，E的M为子模，$M'$为M在$E^*$的正交； $u(M)$ 在 $F^*$ 中的正交是逆像 $^t u^{-1}(M')$。*

这直接从 (15) 得出。

#### 推论{#alg-ii-s2-n5-cor-1 .statement tag=05NI}

*$F^*$中像$u(E)$的正交是$^t u$的核$^t u^{-1}(0)$。*

E 在 $E^*$ 中的正交为 0。

如果$u : E \to F$是同构，$^t u : F^* \to E^*$是同构，并且如果$v : F \to E$是$u$的逆同构，$^t v$是$^t u$的逆同构（公式（17）和（18））。

#### 定义 6 {#alg-ii-s2-def-6 .statement tag=05NJ}

*将 A-模 E 的同构 u 放到 A-模 F 上，u 的逆同构的转置（等于 u 的转置的逆同构）称为 u 的同余同构，并用 $\tilde{u}$ 表示。*

因此，同构$\tilde{u}$的特征为关系
(19) $$
\langle u(x), \tilde{u}(y^*) \rangle = \langle x, x^* \rangle \quad \text{for } x \in E, x^* \in E^*.
$$

如果$v : F \to G$是同构，则$v \circ u$的同余同构是$\tilde{v} \circ \tilde{u}$。

特别地，映射$u \mapsto \tilde{u}$是线性群$\mathbf{GL}(E)$到线性群$\mathbf{GL}(E^*)$的子群的*同构*。

设$\sigma : A \to B$是环$A$的*同构*到环$B$，$E$左$A$模块，$F$左$B$模块和$u : E \to F$ *半线性* 映射 (§ 1, no. 13) *相对于* $\sigma$。设$\sigma^{-1}$为$\sigma$中的逆同构；对于所有$y^* \in F^*$，$E$到$A$的映射$x \mapsto \langle u(x), y^* \rangle^{\sigma^{-1}}$是*线性形式*；如果也用${}^t u(y^*)$表示，则定义映射${}^t u : F^* \to E^*$，也称为半线性映射$u$的*转置*；因此它的特征是身份

$$
\langle u(x), y^* \rangle = \langle x, {}^t u(y^*) \rangle^\sigma
$$

$x \in E, y^* \in F^*$。立即验证${}^t u$是*半线性*映射*相对于*$\sigma^{-1}$。如果$v$表示映射$u$被视为$E$的*A线性*映射到$\sigma_*(F)$（§ 1, no. 13），我们可以写成$u = \phi \circ v$，其中$\phi$是恒等映射 $\sigma_*(F) \to F$，被视为相对于$\sigma$的半线性映射。 ${}^t u = {}^t v \circ {}^t \phi$和$({}^t \phi, \sigma^{-1})$是直接的相对于同构$\sigma^{-1}$的$F^*$到$(\sigma_*(F))^*$的二同构；这个关系允许我们立即得到扩展半线性映射的线性映射到转置的转置的属性。

### 6. 商模的双重。 直和的双重。双基

我们将应用定理 1 of no. 1 应用于 $F = A_s$ 的情况：

#### 命题 9 {#alg-ii-s2-prop-9 .statement tag=05NK}

*设*$E', E, E''$*为A-模并且*

$$
E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$

*线性映射中的正合序列。* *然后转置映射中的序列*

$$
0 \longrightarrow {E''}^* \xrightarrow{{}^t v} E^* \xrightarrow{{}^t u} {E'}^*
$$

*准确。*

#### 推论{#alg-ii-s2-n6-cor-1 .statement tag=05NL}

*设 M 为 A-模 E 和 $\phi : E \to E/M$ 典范同态中的子模。那么*${}^t \phi$*是*$E/M$*的对偶的同构到子模*$M'$*的*$E^*$*正交于*$M$。

如果$j : M \to E$是典范嵌入，则${}^t j$的核通过定义在$E^*$中与$M$正交。

此外，在推论的记号中，当经过为商时，从${}^t j$获得*内射*同态$E^*/M' \to M^*$。

#### 命题 10 {#alg-ii-s2-prop-10 .statement tag=05NM}

*让* $(E_i)_{i \in I}$ *成为A-模的一个家庭，并为所有人* $i \in I$ *让* $j_i : E_i \to E = \bigoplus_{i \in I} E_i$ *成为典范嵌入。* *然后乘积映射* $x^* \mapsto ({}^t j_i(x^*))$

*是对偶* $E^*$ *的* $E$ *的同构到乘积* $\prod_{i \in I} E_i^*$。

这是 § 1, no. 6 的特殊情况，推论 1 到命题 6，适用于 $\prod_{\lambda} F_{\lambda} = A_s$ 的情况。

如果通过典范嵌入 $j_i$，$E_i$ 被其直和 $E$ 的子模识别，如果通过乘积映射 $x^* \mapsto (tj_i(x^*))$，$E^*$ 被$\prod_{i \in I} E_i^*$ 识别，则可以可以说 $\prod_{i \in I} E_i^*$ 是 $\bigoplus_{i \in I} E_i$ 的对偶，规范的双线性形式由下式给出

$$
\langle (x_i), (x_i^*) \rangle = \sum_{i \in I} \langle x_i, x_i^* \rangle.
$$

(22)

#### 推论{#alg-ii-s2-n6-cor-2 .statement tag=05NN}

*Let M, N be two supplementary submodules in an A-module E and $p : E \to M, q : E \to N$ the corresponding projectors; then $^tp + ^tq : M^* \oplus N^* \to E^*$ is an isomorphism and $^tp$ (resp. $^tq$) is an isomorphism of $M^*$ (resp. $N^*$) onto the submodule of $E^*$ orthogonal to $N$ (resp. $M$). 此外，如果$i : M \to E$和$j : N \to E$是典范嵌入，$^tp \circ ^ti$和$^tq \circ ^tj$是投影算子$E^* \to ^tp(M^*)$，$E^*$的$E^* \to ^tq(N^*)$相应的到分解作为直和 $^tp(M^*)$ 和 $^tq(N^*)$。

$p \circ i = 1_M, \quad q \circ j = 1_N, \quad p \circ j = q \circ i = 0, \quad i \circ p + j \circ q = 1_E$、从而，通过转置（no. 5、公式 (16)、(17) 和 (18)），$^ti \circ ^tp = 1_{M^*}, \ ^tj \circ ^tq = 1_{N^*}, \ ^tj \circ ^tp = ^ti \circ ^tq = 0. \ ^tp \circ ^ti + ^tq \circ ^tj = 1_{E^*}$ 和命题由§ 1, no. 6推出，推论 2 到命题 6。

在推论的假设下，$M^*$（或$N^*$）通常与$E^*$中$N$（或$M$）的正交$^tp(M^*)$（或$^tq(N^*)$）进行识别，从而识别每个线性形式$u$ $M$（或$N$），$E$上的线性形式延伸$u$，并且零在$N$（或$M$）上。

当A-模$E$承认*基*$(e_t)_{t \in T}$时，可以看出，给出这个基定义规范地同构$u : A_s^{(T)} \to E$。凭借命题 10 和no. 3、命题 5，$A_s^{(T)}$ 的对偶被规范地标识为乘积 $A_d^T$；考虑相反的同构 $\tilde{u} : A_d^T \to E^*$。如果，对于所有$t \in T, f_t$是$A_d^T$的元素，所有投影都是零，除了指标$t$，它等于1，并且如果我们写出$e_t^* = \tilde{u}(f_t)$，元素$e_t^*$ $E^*$ 由 (19) 和 (22) 得出，其特征在于关系

$$
\langle e_t, e_{t'}^* \rangle = \begin{cases}
0 & \text{for } t' \neq t \\
1 & \text{for } t' = t.
\end{cases}
$$

(23)

对于所有 $x = \sum_{t \in T} \xi_t e_t \in E, \ e_t^*(x) = \xi_t$ 来说，这相当于说： $e_t^*$也称为指标$t$在$E$上的*坐标形式*。从(23)可知$(e_t^*)$是$E^*$中的*免费系统*。

特别是，如果$T$是*有限*，则$E^*$的$e_t^*$形式a *基*，$f_t$则形成$A_d^T$的典范基。因此：

#### 命题 11 {#alg-ii-s2-prop-11 .statement tag=05NO}

*n 元素的自由模和基的对偶是自由模和 n 元素的基。*

注自由模与无限基的对偶不一定是自由模 (VII, § 3, 习题 10)。

#### 定义 7 {#alg-ii-s2-def-7 .statement tag=05NP}

*如果 E 是自由模，且具有有限基* $(e_t)$，则由关系 (23) 定义的对偶 E* *的 *基* $(e_t^*)$ *称为对偶基 of* $(e_t)$。

关系 (23) 也可以写成形式
$$
\langle e_t, e_{t'}^* \rangle = \delta_{tt'}
$$
其中 $\delta_{tt'}$ 是 $T \times T$ 上的*克罗内克符号*。

注如果$T$是有限的并且$(e_t^*)$是$(e_t)$的对偶基，那么，对于
$$ x = \sum_{t \in T} \xi_t e_t \in E, \quad x^* = \sum_{t \in T} \xi_t^* e_t^* \in E^*, $$
$$
\langle x, x^* \rangle = \sum_{t \in T} \xi_t \xi_t^*.
$$

*右* A-模的有限基的对偶基当然也有类似的定义。

#### 推论 {#alg-ii-s2-n6-cor-3 .statement tag=05NQ}

*有限生成射影模的对数是有限生成射影模。*

有限生成的射影左A-模可以用自由A-模$A_s^n$的直因子M和有限基（no. 2，推论1到命题4）来识别。那么（命题 11 和命题 10 的推论）M* 同构于$A_d^n$ 的直因子，从而的推论。

#### 命题 12 {#alg-ii-s2-prop-12 .statement tag=05NR}

*设 E 为 E 的 A-模且* $(a_t)_{t \in T}$ *生成的系统。以下条件是等效的：*
(a) *E 是射影 A-模。*
(b) *在 E 上存在一个族* $(a_t^*)_{t \in T}$ *线性形式，使得对于所有* $x \in E$，*族* $(\langle x, a_t^* \rangle)_{t \in T}$ *有有限支撑并且*
$$
x = \sum_{t \in T} \langle x, a_t^* \rangle a_t.
$$

存在满同态$u : L \to E$，其中$L = A_s^{(T)}$，使得如果$(e_t)_{t \in T}$是L的典范基，则$u(e_t) = a_t$(§ 1, no. 11，命题17)；要使 E 射影，存在线性映射 $v : E \to L$ 使得 $u \circ v = 1_E$ (no. 2, 命题 4 和 § 1, no. 9, 命题 15) 是充分必要的。如果这样的映射存在并且我们写${}^tv(e_t^*) = a_t^*$，那么$\langle x, a_t^* \rangle = \langle x, {}^tv(e_t^*) \rangle = \langle v(x), e_t^* \rangle$，因此$(\langle x, a_t^* \rangle)$族对于所有$x \in E$有有限支撑和$x = u \left( \sum_{t \in T} \langle (x), e_t^* \rangle e_t \right) = \sum_{t \in T} \langle x, a_t^* \rangle a_t$。相反，如果满足叙述的条件(b)，则为所有$x \in E$定义和$\sum_{t \in T} \langle x, a_t^* \rangle e_t$，并且$x \to \sum_{t \in T} \langle x, a_t^* \rangle e_t$为线性映射$v : E \to L$，使得$u \circ v = 1_E$。

### 7. 双向

令 E 为左A-模。 E 的对偶 $E^*$ 的对偶 $E^{**}$ 称为 E 的双偶；也是左A-模（no. 3）。对于所有$x \in E$，从no. 3，公式（10）和（12）得出，映射$x^* \mapsto \langle x, x^* \rangle$是右A-模$E^*$上的线性形式，在双数的其他字元素中$E^{**}$，我们用$\tilde{x}$表示；此外，从 (9) 和 (11) (no. 3) 可以立即得出，E 到 $E^{**}$ 的映射 $c_E : x \mapsto \tilde{x}$ 是线性的；这个映射将被称为规范的；一般来说，它既不是单射也不是满射，即使 E 是有限生成的（cf. 习题 9(e) 和 § 7, no. 5, 定理 6）。

如果典范同态 $c_E : E \to E^{**}$ 是双射的，A-模 E 称为自反。

设 F 为第二个左A-模；对于每个线性映射 $u : E \to F$，映射 $t(tu) : E^{**} \to F^{**}$（也将由 $tu$ 表示）是线性的，并且图表

$$
\begin{array}{ccc}
E & \xrightarrow{u} & F \\
c_E \downarrow & & \downarrow c_F \\
E^{**} & \xrightarrow{tu} & F^{**}
\end{array}
$$

是可交换的，如下直接从定义和公式 (15) 给出转置或线性映射。

#### 命题 13 {#alg-ii-s2-prop-13 .statement tag=05NS}

*如果 E 为自由模*（分别为 *自由模和有限的基*），则 *典范映射* $c_E : E \to E^{**}$ *是单射*（分别为*双射*）。

令$(e_t)_{t \in T}$为E的基，并令$(e_t^*)$为相应的坐标形式的族；通过定义，如果$x \in E$使得$\tilde{x} = 0$，则$\langle x, e_t^* \rangle = 0$对于所有$t \in T$，在其他字中，$x$的所有坐标都是零，因此$x = 0$。进一步假设 T 是有限的；因为$\langle \tilde{e}_t, e_{t'}^* \rangle = \delta_{tt'}$，$(\tilde{e}_t)$是$E^{**}$中$(e_t^*)$的对偶基，并且，当E的$c_E$变换基进入$E^{**}$的基时，$c_E$是双射（§ 1, no. 11，推论 3 到命题 17）。我们还证明了：

#### 推论 1 {#alg-ii-s2-prop-13-cor-1 .statement tag=05NT}

*设 E 为自由A-模，且基有限；对于E的每个基*$(e_t)$*，$(c_E(e_t))$*是基*$(e_t^*)$*的对偶基*$E^*$*对偶*$(e_t)$。

在这种情况下，可以说 $(e_t)$ 和 $(e_t^*)$ 是一个另一个* 的两个*对偶基。

#### 推论 2 {#alg-ii-s2-prop-13-cor-2 .statement tag=05NU}

*如果 E 是自由A-模且基有限，则 E* 的每个有限基是 E 的基的对偶基。*

考虑给定基的 E** 对偶基以及规范地使用 E** 来考虑认同 E 就足够了。

#### 推论 3 {#alg-ii-s2-prop-13-cor-3 .statement tag=05NV}

*令 E、F 为两个 A-模，每个都有一个有限的基，E（分别为 F）与其双元 E**（分别为 F**）被规范地识别。然后，对于每个线性映射 u ：E → F，$t^t u = u$。*

这紧随图表 (27) 的交换律而来。

#### 推论 4 {#alg-ii-s2-prop-13-cor-4 .statement tag=05NW}

*如果 P 为投射模（或有限生成射影模）典范映射 $c_P : P \to P**$ 是单射（或双射）。*

我们将使用以下引理：

#### 引理 1 {#alg-ii-s2-lem-1 .statement tag=05NX}

*设M、N为A-模E中的两个补子模，且i：M→E，j：N→E典范嵌入。然后图表*

$$
\begin{array}{ccc}
M \oplus N & \xrightarrow{c_M \oplus c_N} & M** \oplus N** \\
i + j \downarrow & & \uparrow t_{i_1} + t_{j_1} \\
E & \xrightarrow{c_E} & E**
\end{array}
$$

(28)

*是可交换的。*

定义，$x \in M, y \in N, z^* \in E*$，

$$
\begin{align*}
\langle c_E(i(x) + j(y)), z^* \rangle &= \langle i(x) + j(y), z^* \rangle \\
&= \langle i(x), z^* \rangle + \langle j(y), z^* \rangle \\
&= \langle x, t_i(z^*) \rangle + \langle y, t_j(z^*) \rangle \\
&= \langle c_M(x), t_i(z^*) \rangle + \langle c_N(y), t_j(z^*) \rangle \\
&= \langle t_i(c_M(x)) + t_j(c_N(y)), z^* \rangle.
\end{align*}
$$

因此，如果 E 是自由模（分别是自由模和有限的基），则 $c_E$ 是单射（分别是双射）；另一方面，从 no. 6, 命题 10 可以得出，$t_i \oplus t_j$ 是双射的； 图表 (28) 的交换律意味着 $c_M \oplus c_N$ 是单射（或双射），因此 $c_M$ 和 $c_N$ 也是（§ 1, no. 6，推论 1 到命题 7），从而是推论，取no. 2、命题 4 的账户。

### 8. 线性方程

设E、F为两个A-模。每个形式$u(x) = y_0$的方程，其中$u : E \to F$是给定的线性映射，$y_0$是给定的F的元素，并且未知的$x$受到条件的影响，它在E中取其值，称为a *线性*方程； $y_0$ 称为等式的右边；如果$y_0 = 0$，则该方程称为齐次线性方程。

每个元素$x_0 \in E$使得$u(x_0) = y_0$称为线性方程$u(x) = y_0$的解。†

人们常说，宽泛地说，如果问题等价于确定线性方程的解，则它是线性的。

给定线性方程$u(x) = y_0$，方程$u(x) = 0$称为与$u(x) = y_0$相关的齐次线性方程。

#### 命题 14 {#alg-ii-s2-prop-14 .statement tag=05NY}

*如果$x_0$是线性方程$u(x) = y_0$的解，则该方程的解的集合等于元素$x_0 + z$的集合，其中$z$经过解的集合相关齐次方程 $u(x) = 0$.*

关系$u(x) = y_0$可以写成$u(x) = u(x_0)$，相当于$u(x - x_0) = 0$。

在其他字中，若方程$u(x) = y_0$至少有一个解$x_0$，则其解的集合为集合$x_0 + \overline{u}(0)$，由核$\overline{u}(0)$平移得到$u$。观察$\overline{u}(0)$，即子模，永远不会为空，因为它包含 0（称为齐次方程$u(x) = 0$的零解，或平凡的解）。

凭借命题 14，对于线性方程$u(x) = y_0$来说，要*正好有一个解*，它至少有一个解和$\overline{u}(0) = \{0\}$是必要且充分的（在其他字中，相关的齐次方程没有非零解，或者也有$u$ 是*内射*）；在这种情况下，对于*所有* $y \in F$，方程$u(x) = y$*至多*有一个解。

#### 命题 15 {#alg-ii-s2-prop-15 .statement tag=05NZ}

*令$u$为模$E$中的线性映射变成模$F$。如果方程 $u(x) = y_0$ 至少有一个解，则 $y_0$ 与 $^t u$ 的核正交。*

说$u(x) = y_0$承认解意味着$y_0 \in u(E)$和命题从no. 5推出，推论到命题8。

† 这实际上是一种语言滥用；从逻辑点来看，我们这里并不是定义字“解”，而是简单地将“$x_0$是方程$u(x) = y_0$的解”这句话等同于关系“$x_0 \in E$和$u(x_0) = y_0$”。观察在数学理论中$\mathscr{T}$，其中关系“$A$是环，$E$和$F$是$A$模，$u$是$E$的同态” $F$的$F$、$y_0$元素为定理，$\mathscr{T}$的每个*项* $T$使得关系“$T \in E$和$u(T) = y_0$”为真$\mathscr{T}$是方程$u(x) = y_0$在*集合理论*、I, § 5, no. 2意义上的*解*；这证明了上述滥用语言的行为是合理的。

观察到，当 $A$ 为域（§ 7, no. 6，命题 12）时，由命题 15 给出的解或 $u(x) = y_0$ 存在的必要条件是充分的，但*一般情况下不是*（习题 10）。

#### 注 {#alg-ii-s2-n8-rem-1 .statement tag=05O0}

(1) 令$E$为$A$模块，$(F_i)_{i \in I}$为$A$模块系列，对于所有$i \in I$，令$u_i : E \to F_i$为线性映射。每系统线性方程
$$
u_i(x) = y_i \quad (i \in I)
$$
其中给出$y_i \in F_i$，相当于*单个*线性方程$u(x) = y$，其中$u$是将$E$的映射$x \mapsto (u_i(x))$转化为$F = \prod_{i \in I} F_i$和$y = (y_i)$。如果 $y_i = 0$ 对于所有 $i \in I$，系统 (29) 被称为“齐次”。

(2) 假设$E$承认一个*基* $(a_\lambda)_{\lambda \in L}$；如果我们对所有$\lambda \in L$集合$u(a_\lambda) = b_\lambda$，则说$x = \sum_{\lambda \in L} \xi_\lambda a_\lambda$满足等式$u(x) = y_0$相当于$A$的元素的族（有限支撑）$(\xi_\lambda)_{\lambda \in L}$满足说关系
$$
\sum_{\lambda \in L} \xi_\lambda b_\lambda = y_0.
$$

相反，寻找有限支撑满足 (30) 的 $A$ 的元素族$(\xi_\lambda)_{\lambda \in L}$，相当于求解线性方程 $u(x) = y_0$，其中 $u$ 是 $E$ 到 $F$ 的唯一线性映射，使得$u(a_\lambda) = b_\lambda$ 对于所有 $\lambda \in L$（§ 1, no. 11，推论 3 至命题 17）。

(3) 当 $F = A_s$ 时，线性方程 $u(x) = y_0$ 称为*标量*，因此 $u$ 是 $E$ 上的 *线性形式*，而 $y_0$ 是一个*标量*。如果 $E$ 承认基 $(a_\lambda)_{\lambda \in L}$，则由 *注* (2) 得出，这样的方程也可以写为
$$
\sum_{\lambda \in L} \xi_\lambda \alpha_\lambda = y_0 \in A
$$
其中标量族$(\alpha_\lambda)$是任意的，并且可以理解，标量族$(\xi_\lambda)$必须具有有限支撑。一般来说，由标量线性方程组系统的*解*（在$A$中）
$$
\sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda_i} = \eta_i \quad (i \in I)
$$
其中$\alpha_{\lambda_i} \in A$和$\eta_i \in A$，被理解为*有限*支持的$A$的元素的家庭$(\xi_\lambda)_{\lambda \in L}$和满足（32）； $\alpha_{\lambda_i}$ 称为方程系统的*系数*，$\eta_i$ 称为*右侧*。这样的系统的解等价于等式$u(x) = y$，其中$y = (\eta_i)$和$u : A_s^{(L)} \to A_s^I$是线性映射
$$
(\xi_\lambda) \mapsto \left( \sum_{\lambda \in L} \xi_\lambda \alpha_{\lambda_i} \right).
$$

(4) 当需要避免混淆时，线性系统 (32) 也称为左标量线性方程*系统。 系统方程组
$$
\sum_{\lambda \in L} \alpha_{\lambda_i} \xi_\lambda = \eta_i \quad (i \in I)
$$

同样称为右标量线性方程的系统；通过将$\xi_{\lambda}, \eta_i$和$\alpha_{\lambda_i}$视为属于到逆环$A^0$到A，这样系统可以立即转换为系统（32）。

### 习题{#alg-ii-s2-exercises}

§ 2](exercises/s2/)参见[习题。
