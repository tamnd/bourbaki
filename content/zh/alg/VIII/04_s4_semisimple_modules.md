---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 4
section_title: Semisimple Modules
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.55-A VIII.75
pdf_pages: 0072-0092
extraction: native
subsections:
    - "no": 1
      title: Semisimple Modules
      page: 55
      pdf_page: 72
    - "no": 2
      title: The homomorphism $\bigoplus_i$ Hom$_A(M,N_i)\longrightarrow$ Hom$_A(M,\bigoplus_iN_i)$
      page: 57
      pdf_page: 74
    - "no": 3
      title: Some Operations on Modules
      page: 58
      pdf_page: 75
    - "no": 4
      title: Isotypical Modules
      page: 61
      pdf_page: 78
    - "no": 5
      title: Description of an Isotypical Module
      page: 62
      pdf_page: 79
    - "no": 6
      title: Isotypical Components of a Module
      page: 65
      pdf_page: 82
    - "no": 7
      title: Description of a Semisimple Module
      page: 69
      pdf_page: 86
    - "no": 8
      title: Multiplicities and Lengths in Semisimple Modules
      page: 71
      pdf_page: 88
statements: 43
exercises: 8
content_sha256: d7d0d03aaa6f51ad932f3b7e88e925f00dbe3bd9601105d100b426cb0b9fdbf8
translated_from: content/en/alg/VIII/04_s4_semisimple_modules.md
translation_method: google
source_content_sha256: 9d4584b8ed5e9b2ea8bfc7a3b377164098496c5ee0e2c21f520fa31ff9205f9d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: a193c00d4b6b528ed5d0df3a5833765d01c41c51bb4952ede75f78abfbb2c0c6
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 4。 半单模

### 1. 半单模

#### 定义 1 {#alg-viii-s4-def-1 .statement tag=0040}

如果模是单模.[^1]家族的直和，则称为半单。

如果一个多模块是一系列简单多模块的直和（cf. I, §4, No. 4、p. 37、定义 7），则该多模块被称为半单。

A-模 M 是半单当且仅当当将其视为模超过其同位$A_M$ 的环时，它是半单。

#### 例 1 {#alg-viii-s4-n1-exa-1 .statement tag=0041}

模减为0，单模为半单模。

#### 例 2 {#alg-viii-s4-n1-exa-2 .statement tag=0042}

如果 A 是域，则每个 A-模都是半单 by 定理 1 of II, §7, No. 1、p. 292。这表明，一般来说，半单模可以通过多种方式分解为直和或简单子模（但请参见VIII、p. 68的推论2）。

#### 例 3 {#alg-viii-s4-n1-exa-3 .statement tag=0043}

设A为主理想整环，设P为A的不可约元的代表由……组成(VII, §1, No. 3，p. 3)的系统。设 M 为 A-模，并且对于每个 $\pi \in P$，令 $M(\pi )$ 为 $x\in M$ 的集合，使得 $\pi x= 0$。由VII, §2, No. 2、p. 9、A-模 M 为半单当且仅当它是子模 $M(\pi )$ 的和；那么就是这些子模中的直和。这个例将在（VIII，p. 65）进一步推广。

令$A_1$和$A_2$为代数超过交换环K。在III, §4, No. 3、p. 466中，我们引入了左双模的概念超过代数$A_1$和$A_2$，并证明了概念相当于左模超过环$A_1\otimes_KA_2$。如果 M 是一个简单的（分别是半单，有限生成的）双模，如果它是一个简单的（分别是半单，有限生成的）模超过环 $A_1\otimes_KA_2$。

#### 定理 1 {#alg-viii-s4-thm-1 .statement tag=0044}

设M为模，即简单子模的$(S_i)_{i\in I}$族的（不一定是直接的）和，并令N为M的子模。存在I的子集J，使得M是N的由……组成族的直和并且模 $S_j$ $j$ 穿过 J。

令$\mathscr{S}$为I的子集$I'$的集合，使得模N的族由……组成的和和$I'$中的$i$的$S_i$是直接的。 集合 $\mathscr{S}$ 是有限的特征标： I 属于到 $\mathscr{S}$ 的子集 J 当且仅当对于 J 的每个有限子集都成立。因而，集合 $\mathscr{S}$ 有极大元素J（集合理论、III, §4, No. 5、p. 171）。 集合$N'= N +\sum_{j\in J}S_j$。令$i$在I - J中。由于J在$\mathscr{S}$中最大，集合$J\cup  \{i\}$不会属于到$\mathscr{S}$，因而$S_i\cap N'\not= 0$。由于$S_i$是单模，所以我们有$S_i\cap N'= S_i$。因而，每 $i\in I$ 就有 $S_i\subset N'$，从而 $N'= M$。这样就完成了证明。

#### 推论 1 {#alg-viii-s4-thm-1-cor-1 .statement tag=0045}

单模的家庭中，和的每个模都是半单。

对于 N = 0 的情况，应用定理 1 就足够了。

#### 推论 2 {#alg-viii-s4-thm-1-cor-2 .statement tag=0046}

模 M 是半单当且仅当 M 的每个子模都是直因子。

定理 1 需要条件。

相反，假设 M 的每个子模都承认补充。令$M'$为M中简单子模的和，并令$M''$为M中$M'$的补充。假设我们有$M'\not= M$，因此有$M''\not= 0$。令N为$M''$的非零的单生子模。由VIII的命题 3，p. 49，存在N的极大子模 P。设Q是M中P的子模补集。则$N\cap Q$是N的子模，N中P的补集，因此与$N/P$同构的（II, §1, No. 9、p. 210、命题13）。因而，$N\cap Q$是$M''$的简单子模，与$M'$的定义相反。

因而，我们有 $M'= M$，并且模 M 是半单 × 推论 1。

#### 推论 3 {#alg-viii-s4-thm-1-cor-3 .statement tag=0047}

设M为M的半单模和N子模。模N和$M/N$为半单。更准确地说，如果 M 是单模的族$(S_i)_{i\in I}$的直和，则存在I的子集 J，使得$M/N$与$\bigoplus_{j\in J}S_j$同构的，N与$\bigoplus_{i\in I-J}S_i$同构的。

选择 J 如定理 1。 模 $N'=\bigoplus_{j\in J}S_j$ 是 M 中 N 的补充；因此它与 $M/N$ 同构的。此外，M的子模N和$\bigoplus_{i\in I-J}S_i$都是$N'$的补充，因此与$M/N'$同构的。

#### 推论 4 {#alg-viii-s4-thm-1-cor-4 .statement tag=0048}

设M为半单模。那么 M 是简单的当且仅当 M 的自同态环 E 是域。

如果M是简单的，则E是域乘VIII的命题2的推论，p. 47。

如果 E 是域，则模 M 不可分解 (VIII, p. 31, 命题 4, a))。而且因为是半单，所以很简单。

#### 注 {#alg-viii-s4-n1-rem-1 .statement tag=0049}

令 K 为代数闭交换域且 A K-代数。设 M 为半单A-模，即有限维向量空间超过域 K。则 M 是简单的，当且仅当 A-模 M 的每个自同态都是形式 $x\mapsto \alpha x$，其中 $\alpha$ 在 K 中：这对于 VIII 的定理 1 来说是必要的， p. 47，以上推论 4 就足够了。

### 2. 同态$\bigoplus_i$坎$_A(M,N_i)\longrightarrow$坎$_A(M,\bigoplus_iN_i)$

设A为环，M为A-模，$(N_i)_{i\in I}$为A-模的族。与 $\bigoplus_i$ Hom$_A(M,N_i)$ 的任意元素 $(u_i)$，我们将 Hom$_A(M,\bigoplus_iN_i)$ 的元素 $m\mapsto (u_i(m))$ 关联起来。我们因此定义典范同态

$\varphi :\bigoplus_i$坎$_A(M,N_i)\longrightarrow$坎$_A(M,\bigoplus_iN_i)$。

显然$\varphi$是单射的。设 $u$ 为 Hom$_A(M,\bigoplus_iN_i)$ 的元素。那么 $u$ 属于到 $\varphi$ 的像当且仅当集合指标 $i$ 使得 pr$_i\circ u\not= 0$ 是有限的。当模 M 有限生成时，条件会自动满足。

因而，如果模 M 是有限生成的，则同态 $\varphi$ 是双射的。

### 3. 模的若干运算

令 A 和 B 为环，并令 P 为$(A$, B)-双模 (II, §1, No. 14, p. 225)。我们将定义分两个程序，一个从左B-模到左A-模，另一个从左A-模到左B-模。

3.1. 运算$\mathscr{T}$。 — 令 V 为左B-模。用 $\mathscr{T}(V)$ 表示左A-模 $P\otimes_BV$ (II, §3, No. 4, p. 247)。 $\mathscr{T}(V)$ 上的作用的律由公式给出

$$
a(p\otimes v) = (ap)\otimes v \tag{1}
$$

对于 $a\in A,p\in P$ 和 $v\in V$。

设$V'$为左B-模。对于从V到$V'$的每个B-线性映射$g$，从$\mathscr{T}(V)$到$\mathscr{T}(V')$的映射$1_P\otimes g$是A线性的；我们用$\mathscr{T}(g)$表示。从Hom$_B(V,V')$到Hom$_A(\mathscr{T}(V),\mathscr{T}(V'))$的映射$g\mapsto \mathscr{T}(g)$是$\mathbf{Z}$线性的，我们有

$$
\mathscr{T}(1_V) = 1_{\mathscr{T}(V)},\mathscr{T}(g'\circ g) =\mathscr{T}(g')\circ \mathscr{T}(g) \tag{2}
$$

如果$V, V', V''$是左B-模并且$g: V\rightarrow V',g': V'\rightarrow V''$是B-线性映射。由于张量积与直和通勤，如果V是子模$(V_i)_{i\in I}$家庭的直和，那么我们可以确定A-模$\mathscr{T}(V)$与$\bigoplus_i\mathscr{T}(V_i)$。

3.2. 运算$\mathscr{H}$。 — 令 M 为左A-模。用 $\mathscr{H}(M)$ 表示左B-模 Hom$_A(P,M)$ (II, §1, No. 14, p. 225)。 $\mathscr{H}(M)$ 上的作用的律由公式给出

$$
(bf)(p) =f(pb) \tag{3}
$$

$b\in B,f\in$Hom$_A(P,M)$和$p\in P$。

设$M'$为左A-模。对于从 M 到 $M'$ 的每个 A-线性映射 $g$，从 $\mathscr{H}(M)$ 到 $\mathscr{H}(M')$ 的映射 Hom$_A(1_P, g)$ 是 B 线性的；我们用$\mathscr{H}(g)$表示。从Hom$_A(M,M')$到Hom$_B(\mathscr{H}(M),\mathscr{H}(M'))$的映射$g\mapsto \mathscr{H}(g)$是$\mathbf{Z}$线性的，我们有

$$
\mathscr{H}(1_M) = 1_{\mathscr{H}(M)},\mathscr{H}(g'\circ g) =\mathscr{H}(g')\circ \mathscr{H}(g) \tag{4}
$$

如果$M, M', M''$是左A-模并且$g: M\rightarrow M',g': M'\rightarrow M''$是A-线性映射。此外，假设 P 为有限生成A-模；如果M是子模$(M_i)_i$的家庭的直和，那么我们可以确定$\mathscr{H}(M)$与$\bigoplus_i\mathscr{H}(M_i)$乘以VIII，p. 57。 3.3. 关系 $\mathscr{T}$ 和 $\mathscr{H}$ 之间。 — 通过 II, §4, No. 1、p. 268 中的命题 1，对于每左A-模 M 和每左B-模 V，存在唯一群同构

(5)$\gamma :$坎$_A(\mathscr{T}(V),M)\longrightarrow$坎$_B(V,\mathscr{H}(M))$

其特点是关系

$$
(\gamma (h)(v))(p) =h(p\otimes v) \tag{6}
$$

$h\in$ Hom$_A(\mathscr{T}(V),M),v\in V$和$p\in P$。 同构$\gamma$称为伴随同构。

令 M 为左A-模。 A-模$\mathscr{T}(\mathscr{H}(M))$就是A-模$P\otimes_B$Hom$_A(P,M)$。由上面的应用到B-模$\mathscr{H}$（M），我们看到映射

$\alpha_M=\gamma^{-1}$(身份证$_{\mathscr{H}(M)}$) $:\mathscr{T}(\mathscr{H}(M))\longrightarrow M$

是唯一映射满足

$$
\alpha_M(p\otimes f) =f(p) \tag{7}
$$

$p\in P$ 和 $f\in$ Hom$_A(P,M)$。我们说$\alpha_M$是从$\mathscr{T}(\mathscr{H}(M))$到M的规范A-线性映射。对于每个A-线性映射$g: M\rightarrow M'$，我们有一个可交换的图表

$\mathscr{T}(\mathscr{H}(M))^{\alpha_M}$ // 中号

(I)$\mathscr{T}_{(\mathscr{H}(g))}g$

$\mathscr{T}(\mathscr{H}(M'))^{\alpha_{M'}}$ // $M'$。

反之

$\gamma^{-1}:$ 坎$_B(V,\mathscr{H}(M))\longrightarrow$ 坎$_A(\mathscr{T}(V),M)$

伴随同构重合与映射 $h\mapsto \alpha_M\circ \mathscr{T}(h)$。事实上，根据 (6) 和 (7)，我们有关系

$$
\gamma^{-1}(h)(p\otimes v) = (h(v))(p) =\alpha_M(p\otimes h(v)) =\alpha_M\circ \mathscr{T}(h)(p\otimes v)
$$

适用于所有 $h\in$ Hom$_B(V,\mathscr{H}$ (M))、$v\in V$ 和 $p\in P$。

设V为B-模。 B-模$\mathscr{H}(\mathscr{T}(V))$就是B-模Hom$_A(P,P\otimes_BV)$。通过应用(5)到A-模$\mathscr{T}$(V)，我们看到B-线性映射$\beta_V=\gamma$(Id$_{\mathscr{T}(V)}$)从V到$\mathscr{H}(\mathscr{T}(V))$的特征为关系

$$
\beta_V(v)(p) =p\otimes v \tag{8}
$$

对于 $p\in P$ 和 $v\in V$。我们将$\beta_V$称为从V到$\mathscr{H}(\mathscr{T}(V))$的规范B-线性映射。对于每个 B-模 $V'$ 和每个 B-线性映射 $g: V\rightarrow V'$，我们有一个可交换的图表

V $^{\beta_V}$ /$/\mathscr{H}(\mathscr{T}(V))$

(II)$g\mathscr{H}_{\mathscr{T}}$

($(g)$)

${V'}^{\beta_{V'}}$/$/\mathscr{H}(\mathscr{T}(V'))$。

请注意，伴随态射 (5) 重合与映射将 $u$ 发送到 $\mathscr{H}(u)\circ \beta_V$。事实上，从关系 (6) 和 (8)，我们推导出等式

$$
(\gamma (u)(v))(p) =u(p\otimes v) =u\circ (\beta_V(v))(p)
$$

对于所有 $u\in$ Hom$_A(\mathscr{T}(V),M),v\in V$ 和 $p\in P$。

#### 注 1 {#alg-viii-s4-n3-rem-1 .statement tag=004A}

设V和$V'$为B-模。 伴随同构

$\gamma :$ 坎$_A(\mathscr{T}(V),\mathscr{T}(V'))\longrightarrow$ 坎$_B(V,\mathscr{H}(\mathscr{T}(V')))$

对于每个 $f\in$ Hom$_B(V,V')$ 满足关系 $\gamma (\mathscr{T}(f)) =\beta_{V'}\circ f$ 因为

$$
(\gamma (\mathscr{T}(f))(v))(p) =\mathscr{T}(f)(p\otimes v) =p\otimes f(v) = (\beta_{V'}\circ f)(v)(p)
$$

令M和$M'$为A-模； 伴随同构的倒数

$\gamma^{-1}:$ 坎$_B(\mathscr{H}(M),\mathscr{H}(M'))\longrightarrow$ 坎$_A(\mathscr{T}(\mathscr{H}(M)),M')$

对于每个 $u\in$ Hom$_B(M,M')$ 满足关系 $\gamma^{-1}(\mathscr{H}(u)) =u\circ \alpha_M$。事实上，我们有关系

$$
\gamma^{-1}(\mathscr{H}(u))(p\otimes v) = (\mathscr{H}(u)(v))(p) =u(v(p)) =u\circ \alpha_M(p\otimes v)
$$

适用于所有 $u\in$ Hom$_B(M,M'),v\in \mathscr{H}$ (M) 和 $p\in P$。

#### 注 2 {#alg-viii-s4-n3-rem-2 .statement tag=004B}

令 M 为左A-模。 B-线性映射

$\beta_{\mathscr{H}(M)}:\mathscr{H}(M)\rightarrow \mathscr{H}(\mathscr{T}(\mathscr{H}(M)))$ 和 $\mathscr{H}(\alpha_M) :\mathscr{H}(\mathscr{T}(\mathscr{H}(M)))\rightarrow \mathscr{H}(M)$ 满足关系 $\mathscr{H}(\alpha_M)\circ \beta_{\mathscr{H}(M)}= 1_{\mathscr{H}(M)}$。一般来说，它们不是双射的。

设V为左B-模。 A-线性映射

$\mathscr{T}(\beta_V) :\mathscr{T}(V)\rightarrow \mathscr{T}(\mathscr{H}(\mathscr{T}(V)))$ 和 $\alpha_{\mathscr{T}(V)}:\mathscr{T}(\mathscr{H}(\mathscr{T}(V)))\rightarrow \mathscr{T}(V)$ 满足关系 $\alpha_{\mathscr{T}(V)}\circ \mathscr{T}(\beta_V) = 1_{\mathscr{T}(V)}$。一般来说，它们不是双射的。

#### 注 3 {#alg-viii-s4-n3-rem-3 .statement tag=004C}

假设 P 有限生成为 A-模。令 M 为 A-模家庭$(M_i)_{i\in I}$ 的直和。 A-模 $\mathscr{T}(\mathscr{H}(M))$ 和 $\bigoplus_i\mathscr{T}(\mathscr{H}(M_i))$ 是规范同构的。当我们认同它们时，$\alpha_M$被识别为$\bigoplus_i\alpha_{M_i}$。同样，令V为B-模的家庭$(V_j)_{j\in J}$的直和。 B-模 $\mathscr{H}(\mathscr{T}(V))$ 与$\bigoplus_j\mathscr{H}(\mathscr{T}(V_j))$ 标识，线性映射 $\beta_V$ 与$\bigoplus_j\beta_{V_j}$ 标识。

### 4. 同型模

设 A 为环，S 为简单的左A-模。设D为S的自同态环的逆环；是域。 S 具有 A 和 D 的作用，是$(A$，D)-双模。

#### 命题 1 {#alg-viii-s4-prop-1 .statement tag=004D}

令 M 为 A-模。以下属性是等效的：

(i) 存在集合I使得M与$S^{(I)}$同构。

(ii) 模 M 是子模族中的直和，与 S 同构。

(iii) 模 M 是子模族中的和，与 S 同构。

(iv) 在域 D 上存在左向量空间 V，使得A-模 M 与$S\otimes_DV$ 同构。

(i) 和 (ii) 的等价是直接的，(ii) 和 (iii) 的定理 1 of VIII, p. 56，应用于 N = 0 的情况。D 上的每个左向量空间同构于 的向量空间形式 $D_s^{(I)}$，其中 I 为集合（II, §7, No. 1、p. 292、定理 1）。由于张量积与直和交换，(i) 等价于 (iv)。

#### 定义 2 {#alg-viii-s4-def-2 .statement tag=004E}

如果A-模 M 具有与命题 1 等价的性质，则A-模 M 是型 S 的同型。如果存在单A-模 T，使得 M 是型 T 的同型，则模 M 称为同型。

每个同型模就是半单。

#### 命题 2 {#alg-viii-s4-prop-2 .statement tag=004F}

如果模是型S的同型子模和，那么它是型S的同型。型S的同型模的子模和商模是同型的型 S。

第一个断言来自定义，第二个推论 3 of VIII、p. 56。

#### 注 {#alg-viii-s4-n4-rem-1 .statement tag=004G}

型 S 的每个非零的同型模都有商模和子模同构于 S；因而，如果M和$M'$是型S的非零的同型A-模，则群Hom$_A(M,M')$不会减少到0。

#### 命题 3 {#alg-viii-s4-prop-3 .statement tag=004H}

a) 令 M 为型 S 的同型A-模。 A-线性映射 $\alpha_M: S\otimes_D$Hom$_A(S,M)\rightarrow M$ 特征在于 $\alpha_M(s\otimes f) =f(s)$ (VIII, p. 59) 是双射的。

b) 令V为左向量空间超过域D。由$\beta_V(v)(s) =s\otimes v$(VIII,p. 59)定义的D线性映射$\beta_V: V\rightarrow$Hom$_A(S,S\otimes_DV)$是双射的。

用 $\mathscr{H}(M)$ 表示左侧 D-向量空间 Hom$_A(S,M)$。 A-模 M 与假设、直和属于子模家​​族，与 S 同构的。 A-模 S 是单源的；为了证明映射 $\alpha_M$ 是双射的，因此只需考虑 M = S (VIII, p. 60, 注 3) 的情况。现在，$\mathscr{H}(S)$ 就是 D-向量空间 $D_s$，$\alpha_S$ 就是由 $\iota (s\otimes d) =sd$ 定义的同构 $\iota : S\otimes_DD_s\rightarrow S$。

同样，为了证明b)，只需考虑$V = D_s$的情况。由于映射 $\alpha_S$ 是双射，映射 $\beta_{D_s}=\beta_{\mathscr{H}(S)}$ 也是双射 (VIII, p. 60, 注 2)。

### 5. 等型模的描述

与前面的小节一样，A表示环，S表示简单的左A-模，D表示域End$_A(S)^o$。我们将 S 视为 $(A$,D)-双模。

#### 定义 3 {#alg-viii-s4-def-3 .statement tag=004I}

令 M 为型 S 的同型A-模。M 相对于 S 的描述为对 $(V, \alpha )$，其中 V 为域 D 上的左向量空间，$\alpha : S\otimes_DV\rightarrow M$ 为同构 A-模。

型 S 的每个同型A-模 M 都有规范描述：它是对 (Hom$_A(S,M), \alpha_M$)，其中 $\alpha_M: S\otimes_D$ Hom$_A(S,M)\rightarrow M$ 是 A-模的同构，特征为 $\alpha_M(s\otimes f) =f(s)$ （VIII、p. 62、命题 3、a））。

#### 定理 2 {#alg-viii-s4-thm-2 .statement tag=004J}

设 M 为型 S 的同型A-模和 M 的 $(V, \alpha )$ 描述。用 $\mathscr{D}_D(V)$ 集合（按包含排序）表示 V 的 D 线性子空间，用 $\mathscr{D}_A(M)$ 表示M 的 A-子模。对于每个 $W\in$ $\mathscr{D}_D(V)$、认同 A-模 $S\otimes_DW$ 及其典范像在 $S\otimes_DV$。

a) 映射 $W\mapsto \alpha (S\otimes_DW)$ 是从 $\mathscr{D}_D(V)$ 到 $\mathscr{D}_A(M)$ 的有序集中的同构。

b) 逆同构将M的子模N发送到元素$v$的V由……组成的线性子空间，使得对于每个$s\in S$，$\alpha (s\otimes v)$属于到N。

对于$W\in \mathscr{D}_D$（V），集合$\varphi (W) =\alpha (S\otimes_DW)$。对于$N\in \mathscr{D}_A$(M)，用元素$v\in V$中的$\psi (N)$集合表示，使得每个$s\in S$都有$\alpha (s\otimes v)\in N$。这个定义两个映射$\varphi :\mathscr{D}_D(V)\rightarrow \mathscr{D}_A(M)$和$\psi :\mathscr{D}_A(M)\rightarrow \mathscr{D}_D(V)$。他们显然是递增。

令N为M的子模。它是型S的同型（VIII，p. 61，命题2）。 集合$W =\psi (N)$。到命题 3，VIII、p. 62、A-线性映射 $h: S\rightarrow M$ 的 b) 就只是映射 $s\mapsto \alpha (s\otimes v)$，其中 $v$ 穿过 V。 N 中包含像的为映射 $s\mapsto \alpha (s\otimes w)$，其中 $w$ 穿过 W；它们的像生成N，因为N是型S的同型。因此我们有$\alpha (S\otimes_DW) = N$，即$\varphi (\psi (N)) = N$。这证明$\varphi \circ \psi$在$\mathscr{D}_A(M)$上是恒等映射。特别是，$\varphi$是满射，$\psi$是单射。

要完成证明，只需证明映射$\varphi$是单射的。设 W 和 $W'$ 是 V 的线性子空间，使得 $\varphi (W) =\varphi (W')$。当被视为$S\otimes_DV$的线性子空间时，向量空间$S\otimes_DW$和$S\otimes_DW'$重合。 选择非零的线性形式$f$在D-向量空间S上，并令$g: S\otimes_DV\rightarrow V$为由$g(s\otimes v) =f(s)v$定义的群同态。我们有 $W =g(S\otimes_DW) =g(S\otimes_DW') = W'$，所以 $\varphi$ 是单射的。

#### 注 1 {#alg-viii-s4-n5-rem-1 .statement tag=004K}

设 M 为型 S 的同型A-模和 M 的 $(V, \alpha )$ 描述。则 M 具有有限长度当且仅当 V 是有限维时，在这种情况下，我们有关系

长$_A(M) =$暗$_D(V)$。

#### 推论 1 {#alg-viii-s4-thm-2-cor-1 .statement tag=004L}

令 M 为型 S 的同型A-模。对于 M 的每个 A-子模 N，认同 Hom$_A(S,N)$ 与映射的 Hom$_A(S,M)$ 由……组成的线性子空间以及像包含在 N 中。

a) 映射 $N\mapsto$ 坎$_A(S,N)$ 是有序集中的同构，从$\mathscr{D}_A(M)$ 到$\mathscr{D}_D$（坎$_A(S,M)$）。

b) 逆双射将Hom$_A(S,M)$的线性子空间W发送到M的子模$\sum_{h\in W}h(S)$。

当我们将 $(V, \alpha )$ 视为 M 的规范描述时，这是定理 2 的重新表述。

#### 推论 2 {#alg-viii-s4-thm-2-cor-2 .statement tag=004M}

设V为D上的左向量空间，以及V的自同态为$\mathscr{F}$集合。 $S\otimes_DV$的A-子模在所有自同态$1_S\otimes u$下是稳定的，其中$u$穿过$\mathscr{F}$，当且仅当它是形式$S\otimes_DW$，其中W是子空间的线性V在所有自同态属于到$\mathscr{F}$下都是稳定的。

事实上，到定理 2，$S\otimes_DV$ 的每个 A-子模 N 都等于 $S\otimes_DW$，其中 W 是元素 $v$ V 由……组成的线性子空间，使得 $s\otimes v$每 $s\in S$ 属于到 N。

#### 定理 3 {#alg-viii-s4-thm-3 .statement tag=004N}

令M和$M'$为型S的同型A-模。令$(V, \alpha )$和$(V', \alpha ')$分别为M和$M'$的描述。对于任何 D 线性映射 $f: V\rightarrow V'$，用 $\widetilde{f}: M\rightarrow M'$ 表示唯一的 A-线性映射，它使以下图表通勤：

$S\otimes_DV^{\alpha}$ // 中号

$$
1_{_S\otimes f}\widetilde{f} \tag{9}
$$

$S\otimes_D{V'}^{\alpha'}$ // $M'$。

从霍姆$_D(V,V')$到霍姆$_A(M,M')$的映射$f\mapsto \widetilde{f}$需要群同构。

足以证明从Hom$_D(V,V')$到Hom$_A(S\otimes_DV,S\otimes_DV')$的$\mathbf{Z}$线性映射$u\mapsto 1_S\otimes u$是双射的。在No.3的记号应用于$(A$，D)-双模S，这个对应表明映射

$\mathscr{T}:$坎$_D(V,V')\longrightarrow$坎$_A(\mathscr{T}(V),\mathscr{T}(V'))$

是双射的。但是通过VIII、p. 60的注 1，由于伴随同构(VIII，p. 59)是双射的，这个对应表示将$u$发送到$\beta_{V'}\circ u$的映射是双射，源自 D-线性映射 $\beta_{V'}$ 是双射 (VIII, p. 62, 命题 3, b))。

我们保留定理 3 中的记号。令$M''$ 为型 S 中的同型A-模，并令$(V'', \alpha '')$ 为$M''$ 中的描述。对于每个 $f\in$ Hom$_D(V,V')$ 和每个 $g\in$ Hom$_D(V',V'')$，我们有 $g]\circ f=\widetilde{g}\circ \widetilde{f}$。特别地，对于$M = M'$、$V = V'$和$\alpha =\alpha '$，从End$_D(V)$到End$_A(M)$的映射$f\mapsto \widetilde{f}$是环同构。

#### 注 2 {#alg-viii-s4-n5-rem-2 .statement tag=004O}

设M为型S的同型A-模，并令$(V, \alpha )$为M的描述。设B为环End$_A(M)^o$的子环。 环同构从End$_D(V)^o$到End$_A(M)^o$赋予V与$(D$，B)-双模的结构，使得$\alpha$是$(A$，B)-双模的同构。从$(D$的集合，B）V的子双模，到$(A$的集合，B）存在同构，M的VIII，p. 62，定理 2和 VIII、p. 63、推论 2)。

#### 推论 {#alg-viii-s4-n5-cor-1 .statement tag=004P}

令M和$M'$为型S的同型A-模。映射$u\mapsto$Hom(1$_S, u$)从Hom$_A(M,M')$到Hom$_D$(Hom$_A(S,M)$,Hom$_A(S,M')$)为群同构。当M等于$M'$时，从End$_A(M)$到End$_D$(Hom$_A(S,M)$)是环同构。

由于VIII、p. 59的图表(I)交换律，这个推论是从定理3而来，应用于M的规范描述和$M'$。

### 6. 模的同型分量

#### 定义 4 {#alg-viii-s4-def-4 .statement tag=004Q}

设 A 为环，M A-模，S 单A-模。 M 的型 S 的同型分量，记为$M_S$，是M 的子模的和与S 同构的。

很明显，$M_S$是M的最大的子模，是型S的同型。因为$M_S$的每个子模都是型S的同型（VIII，p. 61， 命题 2)，对于 M 中的每子模 N，我们有 $N_S= M_S\cap N$。

如果$S'$与S单A-模同构，那么我们显然有$M_S=$$M_{S'}$，因此$M_S$仅取决于S的类（VIII，p. 51）。

令 M 为 A-模。 M 存在最大的半单子模，称为M 的底层；它是 M 的简单子模的和，也是 M 的同型分量的和。特别是，M 是半单当且仅当它等于其底层时。

#### 命题 4 {#alg-viii-s4-prop-4 .statement tag=004R}

设 A 为环。用$\mathscr{S}$表示单A-模的类的集合。令 M 为半单A-模。

a) 模 M 是其同型分量家族$(M_{\lambda})_{\lambda\in\mathscr{S}}$ 的直和。

b) 假设 M 是简单子模家庭$(N_i)_{i\in I}$ 的直和。对于每个$\lambda \in \mathscr{S}$，令$I(\lambda )$为指标$i\in I$的集合，使得$N_i$为类$\lambda$。我们有$M_{\lambda}=\bigoplus_{i\in I(\lambda)}N_i$。

c) 如果 M 是有限生成的，则 $\lambda \in \mathscr{S}$ 的集合使得 $M_{\lambda}\not= 0$ 是有限的。

d) 对于 M 的每子模 N 和每 $\lambda \in \mathscr{S}$，我们有 $N_{\lambda}= N\cap M_{\lambda}$ 和 $(M/N)_{\lambda}= (M_{\lambda}+ N)/N$。

由于M是半单，所以它是家庭$(M_{\lambda})_{\lambda\in\mathscr{S}}$的和；让我们证明这个和是直接的。让$\lambda \in \mathscr{S}$。用$M'_{\lambda}$表示家庭$(M_\mu)_{\mu\in\mathscr{S}-\{\lambda\}}$的和。 模 $M'_{\lambda}$ 是单模系列中的直和，与 $\lambda$ 不同构（VIII、p. 56、定理 1）。通过VIII、p. 56、$M'_{\lambda}$ 定理 1 中的推论 3 不包含类 $\lambda$ 中的任何简单子模。因此我们有 $M_{\lambda}\cap M'_{\lambda}= 0$。因此断言a)得证。到构造，我们有$M_{\lambda}\supset \bigoplus_{i\in I(\lambda)}N_i$，所以断言 b) 由II, §1, No. 8、p. 208 的注 1 得出。

断言 c) 由a) 和II, §1, No. 12、p. 221 的命题 23 得出。

令 N 为 M 的子模和 $\lambda \in \mathscr{S}$。 N的型$\lambda$的同型分量$N_{\lambda}$包含在$M_{\lambda}$和$M_{\lambda}\cap N\subset N_{\lambda}$中。因而，交$N\cap M_{\lambda}$是型$\lambda$的N的同型分量。

对于每个 $\lambda \in \mathscr{S}$，模 $M_{\lambda}+N/N$ 与 $M_{\lambda}/(M_{\lambda}\cap N)$ 同构的。因而，它是型 $\lambda$ 的同型并包含在 $(M/N)_{\lambda}$ 中。然后从 a) 和 II, §1, No. 8、p. 208、注 1 得出最后一个断言。

#### 推论 {#alg-viii-s4-n6-cor-1 .statement tag=004S}

令A为环和单A-模的类中的$\mathscr{S}$集合。设M为M的半单A-模和N子模。那么我们有$N =\bigoplus_{\lambda\in\mathscr{S}}N\cap M_{\lambda}$和$M/N =\bigoplus_{\lambda\in\mathscr{S}}(M_{\lambda}+ N)/N$。

由于 N 和 $M/N$ 是半单（VIII、p. 56、推论 3），推论由命题 4 得出，d)。

半单A-模 M 的支持度是单A-模的类 $\lambda$ 的集合，使得型 $\lambda$ 的M 的同型分量是非零的。有限生成的半单A-模的支持是有限的。

#### 命题 5 {#alg-viii-s4-prop-5 .statement tag=004T}

设A为环，且令$\mathscr{S}$为单A-模的类的集合。设 M 和 N 为 A-模。

a) 设$f: M\rightarrow N$为同态。对于从$M_{\lambda}$到$N_{\lambda}$的每个$\lambda \in \mathscr{S},f$诱导同态$f_{\lambda}$；如果 M 是半单和 $f$ 满射，则同态 $f_{\lambda}$ 都是满射。

b) 假设 M 为半单。从 Hom$_A(M,N)$ 到 $\prod_{\lambda\in\mathscr{S}}$ Hom$_A(M_{\lambda},N_{\lambda})$ 为映射 $f\mapsto (f_{\lambda})_{\lambda\in\mathscr{S}}$ 群同构。当M等于N时，从End$_A(M)$到$\prod_{\lambda\in\mathscr{S}}$End$_A(M_{\lambda})$，映射为环同构。

对于每个$\lambda \in \mathscr{S}$，N的子模$f(M_{\lambda})$同构于型$\lambda$同型模商；因而，它是型$\lambda$的同型，因此包含在$N_{\lambda}$中。

假设 M 是半单和 $f$ 满射。然后$f$诱导同构从$M/$Ker($f$)到N，发送$(M_{\lambda}$+Ker($f$))$/$Ker($f$)到$f(M_{\lambda})$。到VIII、p. 65的命题 4，我们有$N_{\lambda}=f(M_{\lambda})$，这就完成了a)的证明。

b)中考虑的映射显然是群同态，当M等于N时，它是环同态。令$(f_{\lambda})_{\lambda\in\mathscr{S}}$为$\prod_{\lambda\in\mathscr{S}}$Hom(M$_{\lambda},N_{\lambda}$)的元素。 b)中映射下的逆像中的唯一元素是同态$f: M\rightarrow N$，定义为

$$
f((\sum_{\lambda\in\mathscr{S}}x_{\lambda})=\sum_{\lambda\in\mathscr{S}}f_{\lambda}(x_{\lambda})
$$

对于每个$(x_{\lambda})_{\lambda\in\mathscr{S}}\in \bigoplus_{\lambda}M_{\lambda}$。

#### 注 {#alg-viii-s4-n6-rem-1 .statement tag=004U}

设 A 和 B 为环。设 M 为 $(A$, B)-双模。从命题 5 可以得出，A-模 M 的同型分量是 M 的子双模。特别是当 M 是A-模并且 B 是 End$_A(M)$ 的逆环时，这一点尤其成立。

#### 例 {#alg-viii-s4-n6-exa-1 .statement tag=004V}

让我们考虑环 A 是可交换的情况。 将最大理想 $\mathfrak{m}$ 发送到 cl(A$/\mathfrak{m}$) 的映射是从 A 的最大理想集合到简单 A 模块类 (VIII, p. 51) 的类集合 $\mathscr{S}$ 的双射。 逆双射将$\lambda$发送至其湮没子$\mathfrak{m}_{\lambda}$。

设M为A-模。对于每个$\lambda \in \mathscr{S}$，M的型$\lambda$的同型分量$M_{\lambda}$由元素被$\mathfrak{m}_{\lambda}$湮灭组成，我们可以将$M_{\lambda}$视为向量空间超过域 $A/\mathfrak{m}_{\lambda}$。如果M是半单，N是另一个A-模，那么我们可以从命题5推导出群同构从Hom$_A(M,N)$到$\prod_{\lambda\in\mathscr{S}}$Hom$_{A/\mathfrak{m}_{\lambda}}(M_{\lambda},N_{\lambda})$。

#### 推出 1 {#alg-viii-s4-prop-5-cor-1 .statement tag=004W}

设 M 为 M 的半单A-模且 N 子模。以下属性是等效的：

(i) M 中 N 存在唯一的子模补集。

(ii) 我们有Hom$_A(M/N,N) = 0$。

(iii) 存在$\mathscr{S}$的子集Λ使得$N =\bigoplus_{\lambda\in\Lambda}M_{\lambda}$。

选择子模 $N'$ 对 M 中的 N 进行补充（VIII、p. 56、推出 2）。如果我们用$N'\times N$来认同 M，那么M对N的补充子模就是A-线性映射从$N'$到N的图。由于$N'$与$M/N$同构的，我们就证明了性质(i)和(ii)的等价。由命题 5，b)，群 Hom$_A(N',N)$ 同构于群 $\prod_{\lambda\in\mathscr{S}}$ Hom$_A(N'_{\lambda},N_{\lambda})$。当且仅当对于每个$\lambda \in \mathscr{S}$，我们有$N_{\lambda}= 0$或$N'_{\lambda}= 0$（VIII，p. 61，注），即$N_{\lambda}= 0$或$N_{\lambda}= M_{\lambda}$，它才是零。这证明了性质 (ii) 和 (iii) 的等价。

#### 推出 2 {#alg-viii-s4-prop-5-cor-2 .statement tag=00R0}

设M为A-模。下面两个条件是等价的：

(i) M 的每个子模都承认唯一的补子模。

(ii) 模 M 是简单、成对非同构模族$(S_i)_{i\in I}$ 的直和。

假设M满足这些条件。然后，对于 M 的每个子模 N，都存在一个唯一的 I 子集 J，这样我们就有 $N =\bigoplus_{j\in J}S_j$，并且 M 的每个简单子模都等于 $S_i$ 之一。

条件(i)和(ii)都意味着M是半单。

假设满足条件(i)。让$\lambda \in \mathscr{S}$。通过推论 1中的(i)和(iii)的等价，$M_{\lambda}$的每个子模等于零或等于$M_{\lambda}$。因而，$M_{\lambda}$是零或简单，并且（ii）根据M是$(M_{\lambda})_{\lambda\in\mathscr{S}}$族的直和这一事实得出。

相反，如果满足条件 (ii)，则$M_{\lambda}$ 是零或对于每个 $\lambda \in \mathscr{S}$ 都是简单的。如果 N 是 M 的子模，则对于每个 $\lambda \in \mathscr{S}$，$N\cap M_{\lambda}$ 等于 0 或 $M_{\lambda}$。由于我们有 $N =\bigoplus_{\lambda\in\mathscr{S}}(N\cap M_{\lambda})$ (VIII, p. 66, 推出)，子模 N 的性质 (iii) 为推论 1，因此在 M 中承认唯一的补子模。这证明 (ii) 蕴涵 (i)，以及最后一个断言推论。

设 M 为 A-模，S 单A-模。用 D 表示域 End$_A(S)$ 的逆环，并将 S 视为$(A$，D)-双模。那么Hom$_A(S,M)$是D上的左向量空间，Hom$_A(M,S)$是D上的右向量空间。左D-向量空间Hom$_A(S,M)$的对偶是D上的右向量空间（II, §2, No. 3，p. 232，定义2）。对于每个$u\in$Hom$_A(M,S)$，从Hom$_A(S,M)$到Hom$_A(S,S) = D$的映射$h(u) :v\mapsto u\circ v$是线性形式在左边D-向量空间Hom$_A(S,M)$。

#### 命题 6 {#alg-viii-s4-prop-6 .statement tag=004X}

保留上面的记号，并假设A-模 M 为半单。从右D-向量空间Hom$_A(M,S)$到左D-向量空间Hom$_A(S,M)$的对偶映射$u\mapsto h(u)$是D-线性和双射的。

让$u\in$Hom$_A(M,S),v\in$Hom$_A(S,M)$和$d\in D$。我们有

$$
h(ud)(v) =h(d\circ u)(v) =d\circ u\circ v=d\circ (h(u)(v)) =h(u)(v)d
$$

这证明映射$h$是D-线性的。它只是由 $u\mapsto$ Hom(1$_S, u$) 从 Hom$_A(M,S)$ 到 Hom$_D$(Hom$_A(S,M)$, Hom$_A(S,S)$) 给出的映射。为了证明它是双射的，由命题 5, b) of VIII，p. 66，只需处理M与型 S同型的情况即可；然后我们可以应用VIII、p. 65中的推论。

### 7. 半单模的描述

对于这个截面的剩余部分，A是环，$\mathscr{S}$是单A-模的类中的集合。对于每个 $\lambda \in \mathscr{S}$，我们选择单模 $S_{\lambda}$ 或类 $\lambda$（例如， $S_{\lambda}=\lambda$ ）；我们用$D_{\lambda}$表示$S_{\lambda}$的自同态的域的逆环。我们将$S_{\lambda}$视为$(A,D_{\lambda}$)-双模。

令 M 为 A-模。对于每 $\lambda \in \mathscr{S}$，Hom$_A(S_{\lambda},M)$ 是左向量空间超过域 $D_{\lambda}$。由VIII、p. 59、II, §1, No. 6、p. 202、命题 6，存在一个唯一的A-线性映射，称为规范，

$\alpha_M:\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}$坎$_A(S_{\lambda},M))\rightarrow M$

满足关系

$$
\alpha_M(s\otimes f) =f(s) \tag{10}
$$

$\lambda \in \mathscr{S},s\in S_{\lambda}$、$f\in$ Hom$_A(S_{\lambda},M)$。如果我们赋予 $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M))$ 和 M 自然的结构 End$_A$(M)-模，那么映射 $\alpha_M$ 是 End$_A$(M)-线性。

#### 命题 7 {#alg-viii-s4-prop-7 .statement tag=004Y}

设 M 为 A-模。 典范映射 $\alpha_M$ 是单射的。对于每个$\lambda \in \mathscr{S}$，$S_{\lambda}\otimes_{D_{\lambda}}$Hom$_A(S_{\lambda},M)$的$\alpha_M$下的像是型$\lambda$的M的同型分量。 $\alpha_M$的像是M的底层。A-模M是半单当且仅当映射$\alpha_M$是双射。

让$\lambda \in \mathscr{S}$。用 $M_{\lambda}$ 表示型 $\lambda$ 的同型分量。从$S_{\lambda}$到M的每个A-线性映射在$M_{\lambda}$中取其值（VIII，p. 66，命题5）。因而，通过命题 3，a) 的 VIII、p. 62、映射 $\alpha_M$ 诱导双射从 $S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M)$ 到 $M_{\lambda}$。 命题遵循，因为M的底层是$(M_{\lambda})_{\lambda\in\mathscr{S}}$族的直和，并且模M是半单当且仅当它等于它的底层。

#### 定义 5 {#alg-viii-s4-def-5 .statement tag=004Z}

令 M 为半单A-模。 M 的描述（相对于家庭$(S_{\lambda})_{\lambda\in\mathscr{S}}$）为对$((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$，其中$V_{\lambda}$为左向量空间超过域$D_{\lambda}$，对于每个$\lambda \in \mathscr{S}$和$\alpha :\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda})\rightarrow M$为同构 A-模。

到命题 7，每个半单A-模 M 都有规范描述：它是对 ((Hom$_A(S_{\lambda},M)$)$_{\lambda\in\mathscr{S}}, \alpha_M$)，其中$\alpha_M$ 是由公式 (10) 定义的A-线性映射。

#### 命题 8 {#alg-viii-s4-prop-8 .statement tag=0050}

设 M 为 M 的半单A-模和 $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$ 描述。

a) 对于从A-模$S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$到型$\lambda$的M的同型分量的每个$\lambda \in \mathscr{S}$，映射$\alpha$诱导同构。

b) 对于每个$\lambda \in \mathscr{S}$，由$\beta_{\lambda}(v)(s) =\alpha (s\otimes v)$定义的映射$\beta_{\lambda}: V_{\lambda}\rightarrow$Hom$_A(S_{\lambda},M)$是$D_{\lambda}$-线性和双射的。

c) 设N为M的子模。存在一个唯一族$(W_{\lambda})_{\lambda\in\mathscr{S}}$，具有以下属性：$W_{\lambda}$对于每个$\lambda \in \mathscr{S}$是$V_{\lambda}$的$D_{\lambda}$线性子空间，并且N是模的$\alpha$下的像 $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}W_{\lambda})$ 与模 $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda})$ 中的典范像进行识别。对于每个$\lambda \in \mathscr{S},W_{\lambda}$是元素$v\in V_{\lambda}$的集合，使得对于每个$s\in S_{\lambda}$，$\alpha (s\otimes v)$属于到N。

对于每个 $\lambda \in \mathscr{S}$，A-模 $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ 是型 $\lambda$ 的同型。 断言 a) 然后根据$\alpha$ 是同构并且 M 是 $(M_{\lambda})_{\lambda\in\mathscr{S}}$ 族的直和 (VIII, p. 65, 命题 4, a)) 得出结论。

让$\lambda \in \mathscr{S}$。将$\alpha$到$S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$的限制用$\alpha_{\lambda}: S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}\rightarrow$ M表示。将No. 3的记号应用于$(A,D_{\lambda}$)-双模$S_{\lambda}$，我们有

$$
\beta_{\lambda}=\gamma (\alpha_{\lambda}) =\mathscr{H}(\alpha_{\lambda})\circ \beta_{V_{\lambda}}
$$

其中最后一个等式源自 VIII、p. 60。因而，$\beta_{\lambda}$是$D_{\lambda}$线性同态$\mathscr{H}(\alpha_{\lambda})$和$\beta_{V_{\lambda}}$的合成。 断言 b) 然后从VIII、p. 62 的命题 3、b) 得出。

令 N 为 M 的子模。我们有 $N =\bigoplus_{\lambda\in\mathscr{S}}(N\cap M_{\lambda})$ (VIII, p. 66, 推论)，因而 c) 可从 VIII、p. 62 的定理 2 得出。

#### 推论 {#alg-viii-s4-n7-cor-1 .statement tag=0051}

令 M 为半单A-模。对于M的每个子模N和$\mathscr{S}$的每个元素$\lambda$，认同Hom$_A(S_{\lambda},N)$以及映射的Hom$_A(S_{\lambda},M)$由……组成的$D_{\lambda}$线性子空间 N 中包含像。

a) 映射 $N\mapsto$ (Hom$_A(S_{\lambda},N)$)$_{\lambda\in\mathscr{S}}$ 是双射，从 M 的 A-子模的集合到$(W_{\lambda})_{\lambda\in\mathscr{S}}$ 家庭的集合，这样对于每个 $\lambda \in \mathscr{S}$，$W_{\lambda}$ 是Hom$_A(S_{\lambda},M)$的$D_{\lambda}$-线性子空间。

b) 逆双射将家人$(W_{\lambda})_{\lambda\in\mathscr{S}}$发送给M的A-子模$\sum_{\lambda\in\mathscr{S}}\sum_{w\in W_{\lambda}}w(S_{\lambda})$。

这是命题 8 的重新表述，c) 应用于 M 的规范描述。

#### 命题 9 {#alg-viii-s4-prop-9 .statement tag=0052}

设M和$M'$为半单A-模，并分别考虑M和$M'$的描述、$((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$和$((V'_{\lambda})_{\lambda\in\mathscr{S}}, \alpha ')$。对于 $\prod_{\lambda\in\mathscr{S}}$ Hom$_{D_{\lambda}}(V_{\lambda},V_{\lambda}')$ 的每个家庭 $\boldsymbol{f}= (f_{\lambda})_{\lambda\in\mathscr{S}}$，都存在一个唯一的 A-线性映射 $\varphi (\boldsymbol{f})\in$ Hom$_A(M,M')$，以下图表通勤：

$\bigoplus(S_{\lambda}\otimes_DV_{\lambda})^{\alpha}$ // 中号

$$
\lambda \in \mathscr{S}\lambda
$$

$$
\bigoplus(1_S\otimes f_{\lambda})
$$

$$
_{\lambda}\varphi (\boldsymbol{f})
$$

$\lambda \in \mathscr{S}$

$\bigoplus(S_{\lambda}\otimes_DV'_{\lambda})^{\alpha'}$ // $M'$。

$\lambda \in \mathscr{S}\lambda$

映射 $\varphi :\prod_{\lambda\in\mathscr{S}}$ Hom$_{D_{\lambda}}(V_{\lambda},V'_{\lambda})\rightarrow$ Hom$_A(M,M')$这样定义就是群同构。当我们对每个$\lambda \in \mathscr{S}$和$\alpha =\alpha '$有$M = M',V_{\lambda}= V'_{\lambda}$时，从$\prod_{\lambda\in\mathscr{S}}$End$_{D_{\lambda}}(V_{\lambda})$到End$_A(M)$，映射$\varphi$是环同构。

鉴于命题 8, a)中给出的M的同型分量和$M'$的描述，这是从VIII、p. 64和命题 5, b)的定理 3得出的，VIII， p. 66。

#### 推论 {#alg-viii-s4-n7-cor-2 .statement tag=0053}

设 M 为半单A-模和 $M'$ A-模。 映射 $u\mapsto$ (霍姆(1$_{S_{\lambda}}, u$))$_{\lambda\in\mathscr{S}}$ 从 霍姆$_A(M,M')$ 至

$\prod_{\lambda\in\mathscr{S}}$ 坎$_{D_{\lambda}}$(坎$_A(S_{\lambda},M)$, 坎$_A(S_{\lambda},M')$)

是群同构。当$M'$等于M时，从环End$_A(M)$到环$\prod_{\lambda\in\mathscr{S}}$End$_{D_{\lambda}}$(Hom$_A(S_{\lambda},M)$)为同构。

这是将命题 9 应用于M 的规范描述和$M'$ 的底层的重新表述。

### 8. 半单模中的重数和长度

#### 命题 10 {#alg-viii-s4-prop-10 .statement tag=0054}

设 M 为半单A-模。令$(M_i)_{i\in I}$为简单子模与直和M的族。以下性质是等价的：

(i) M 有有限长度。

(ii) M 为阿廷的。

(iii) M 为诺特。

(iv) M 是有限生成的。

(v) I 是有限的。

如果 M 具有这些属性，则 M 的长度等于 I 的基数。

如果集合 I 是有限的，则 M 具有属性 (i)、(ii)、(iii) 和 (iv)。假设集合 I 是无限的。 VIII、p. 2、模中的例 2，M 既不是阿廷的，也不是诺特；因为有限长度的每个模都是阿廷的和诺特（VIII，p. 2，命题1），所以M也没有有限长度。最后，M 属于到和的每个元素是子模$M_i$的有限数，因此M不是有限生成的。这证明了属性 (i) 到 (v) 的等价。如果这些成立，那么我们有 long(M) $=\sum_{i\in I}$ long(M$_i$) $=$ Card(I) (II, §1, No. 10, p. 213, 推论 5)。

#### 命题 11 {#alg-viii-s4-prop-11 .statement tag=0055}

设M为半单A-模，即简单子模的家庭$(M_i)_{i\in I}$的直和。对于每个$\lambda \in \mathscr{S}$，我们用指标$i\in I$的$I(\lambda )$集合表示，这样$M_i$就是类$\lambda$。 $I(\lambda )$的基数等于左$D_{\lambda}$向量空间Hom$_A(S_{\lambda},M)$的维数。

型 $\lambda$ 的 A 的同型分量与 $S_{\lambda}^{(I(\lambda))}$ 同构的 (VIII, p. 65, 命题 4, b))。 $D_{\lambda}$-向量空间 Hom$_A(S_{\lambda},M)$ 可以与 Hom$_A(S_{\lambda},M_{\lambda})$ 等价，因此与 $D_{\lambda}^{(I(\lambda))}$ (No. 2) 同构的。这就证明了命题。

每个单模都是原初的（VIII，p. 45），所以每个半单模都是半原初的。令M为半单A-模，并令$\lambda \in \mathscr{S}$。 M 中$\lambda$ 的重数是VIII、p. 34 中定义的M 中$\lambda$ 的原始重数 $[M :\lambda ]$。 命题 11 翻译为等式

（11）$[M :\lambda ] =$昏暗$_{D_{\lambda}}$（坎$_A(S_{\lambda},M)$）。

更一般地，如果$((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$是M的描述，则$[M :\lambda ]$等于dim$_{D_{\lambda}}(V_{\lambda})$。到 VIII、p. 68 的命题 6，我们还有

(12) $[M :\lambda ] =$ 昏暗$_{D_{\lambda}}$(坎$_A(M,S_{\lambda})$)

当重数$[M :\lambda ]$有限时。 半单A-模 M 和 $M'$ 同构当且仅当我们对于每个 $\lambda \in \mathscr{S}$ 都有 $[M :\lambda ] = [M':\lambda ]$。

设M为半单A-模。存在基数$\mathbf{I}$，其性质：对于M的每个分解$M =\bigoplus_{i\in I}M_i$到单模的直和，I的基数等于$\mathbf{I}$（VIII， p. 34、推论 2)。这个基数称为半单A-模M的长度，用long$_A(M)$或long(M)表示。当M有有限长度时，这个定义与II, §1, No. 10、p. 212兼容命题10。

单A-模是长度 1 中的半单A-模，我们有公式

(13) 长$_A(\bigoplus_{j\in J}M_j)=\sum_{j\in J}$ 长$_A(M_j)$

对于每个家庭$(M_j)_{j\in J}$ 半单A-模。到命题 11 时，我们已经

（14）长$_A(M) =\sum_{\lambda\in\mathscr{S}}$暗$_{D_{\lambda}}$坎$_A(S_{\lambda},M)$。

通过应用这个公式到$M_{\lambda}$，对于每个$\lambda \in \mathscr{S}$，我们获得$[M :\lambda ] =$长$_A(M_{\lambda})$。

当A为域时，单A-模为维数1中的向量空间；那么每个 A-模就是半单 (II, §7, No. 1, p. 292, 定理 1)，并且它的长度只是它的维数作为 A (II, §7, No. 2, p. 293) 上的向量空间 。

### 习题{#alg-viii-s4-exercises}

参见[习题为 § 4](exercises/s4/)。

[^1]: By Corollary 2 of VIII, p. 56, this definition coincides with that given in VII, §2, No. 2, p. 9
