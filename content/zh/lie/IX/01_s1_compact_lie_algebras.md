---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 1
section_title: Compact Lie algebras
lang: zh
source: lie-vii-ix
book_pages: 281-287, 389-391
pdf_pages: 0288-0294, 0396-0398
extraction: native
subsections:
    - "no": 1
      title: INVARIANT HERMITIAN FORMS
      page: 281
      pdf_page: 288
    - "no": 2
      title: CONNECTED COMMUTATIVE REAL LIE GROUPS
      page: 282
      pdf_page: 289
    - "no": 3
      title: COMPACT LIE ALGEBRAS
      page: 283
      pdf_page: 290
    - "no": 4
      title: GROUPS WHOSE LIE ALGEBRA IS COMPACT
      page: 284
      pdf_page: 291
statements: 13
exercises: 9
content_sha256: 4515e3418a6639e1b3fed6ddfe52289ccab2b88c252159d4921afedb1e75e88f
translated_from: content/en/lie/IX/01_s1_compact_lie_algebras.md
translation_method: google
source_content_sha256: 71ef208b41db85bf8bc8c5557777019fadb960c88536da1750a4c9288864f27c
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 3007f022ce0e552f6e1f90f23cfacdb7dd6cbbb00b03663c053cde1d49d166ea
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 1。 紧李代数

### 1. 不变厄米形式

在这个数中，字母$k$表示域$\mathbf{R}$或$\mathbf{C}$。令V为有限维$k$向量空间，$\Phi$在V上分离$^2$正厄米特形式，G群，$\mathfrak{g}$一个$\mathbf{R}$-李代数，$\rho : G\rightarrow \mathbf{G}\mathbf{L}(V)$ 群同态, $\varphi :\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(V)$ 同态 of $\mathbf{R}$-李代数。

a) 形式 $\Phi$ 在 G（或 $\mathfrak{g}$）下是不变的，当且仅当 $\rho (g)$ 对于所有 $g\in G$ 相对于 $\Phi$ 是酉的（或$\varphi (x)$ 是反厄米特$^3$） $\Phi$ 对于所有$x\in \mathfrak{g}$）。事实上，用$a^*$表示V的自同态$a$相对于$\Phi$的伴随；对于$\mathfrak{g},u$中的$G,x$中的$g$和V中的$v$，我们有

$$
\Phi (\rho (g)u, \rho (g)v) =\Phi (\rho (g)^*\rho (g)u, v)
$$

$$
\Phi (\varphi (x)u, v) +\Phi (u, \varphi (x)v) =\Phi ((\varphi (x) +\varphi (x)^*).u, v)
$$

$^1$ 在整个章中，参考了代数，第 1 章。 VIII，已到新版

（准备中）

$^2$ 回想一下（代数，第 IX 章，准备中）厄米特形式 H on V 说过

分离（或非简并）如果，对于 V 的每个非零元素 $u$，有

存在$v\in V$使得$H(u, v)\not= 0$。

$^3$ 元素 $a\in$ End(V) 相对于 $\Phi$ 被认为是反厄米特式，如果

$a$相对于$\Phi$的伴随$a^*$等于$-a$。当$k=\mathbf{C}$（或$k=\mathbf{R}$）时

也意味着V（或$\mathbf{C}\otimes_{\mathbf{R}}V$）的自同态$ia$是厄米特。因此，对于V中的所有$u, v$，$\Phi (\rho (g)u, \rho (g)v) =\Phi (u, v)$当且仅当$\rho (g)^*\rho (g) =$ Id$_V$；类似地，$\Phi (\varphi (x)u, v) +\Phi (u, \varphi (x)v) = 0$对于V中的所有$u, v$当且仅当$\varphi (x) +\varphi (x)^*= 0$，因此规定断言。

b) 如果形式 $\Phi$ 在 G 下不变（分别为 $\mathfrak{g}$），则 V 的稳定子空间的正交补是稳定的；特别是，表示$\rho$（分别$\varphi$）则为半单（cf.代数，第IX章）；此外，对于V的所有$g\in G$（或$x\in \mathfrak{g}$），自同态$\rho (g)$（或$\varphi (x)$）则为半单，其中特征值为绝对值值1（或纯虚数） 特征值);事实上$\rho (g)$是酉的（分别是$i\varphi (x)$是厄米特，cf.代数，第IX）。

c) 假设$k=\mathbf{R}$。如果 G 是李群的连通李群、$\rho$ 态射、G 的$\mathfrak{g}$ 李代数以及由 $\rho$ 引发的$\varphi$ 同态，则 $\Phi$ 在 G 下不变并且仅当它在 $\mathfrak{g}$ 下保持不变时（第 III, §6, no. 5 章，Cor. 3）。

d) 当且仅当 $\mathbf{G}\mathbf{L}(V)$ 的子群 $\rho (G)$ 相对紧时，在 G 下的 V 不变量上存在分离正厄米特形式（积分，第 VII, §3, no. 1 命题 1）。

### 2. 已连接交换实李群

令 G 为连通交换律（实数）李群。指数映射

经验$_G: L(G)\rightarrow G$

是李群的态射，与离散核的满射（第 III, §6, no. 4 章，命题 11），因此L(G) 是 G 的连通覆盖。

a) 以下条件是等价的：G是单连通的，exp$_G$是同构，G与$\mathbf{R}^n(n=$dim G同构。在这种情况下，通过同构 exp$_G$ 将 L(G) 的向量空间结构传输到 G，得到 G 上的向量空间结构，这是唯一与 G 的拓扑群结构兼容的。 李群称为向量（谎言）群； 除非否则，它们总是被赋予上面定义的$\mathbf{R}$向量空间结构。

b) 用exp$_G$的$\Gamma (G)$核表示。作者：将军拓扑，第 1 章VII, §1, no. 1，周四。 1, 群 G 是紧致的当且仅当 $\Gamma (G)$ 是 L(G) 中的格子，在其他字（前述）中，如果自由 $\mathbf{Z}$ 模 $\Gamma (G)$ 的秩等于 G 的维数。相反，如果L是有限维$\mathbf{R}$向量空间且$\Gamma$是L中的格，则商拓扑群$L/\Gamma$是紧连通交换李群。

紧连通交换李群称为实环面，或（在这个章）环面。

c) 一般情况下，令E为$\Gamma$(G)生成的L(G)的向量子空间，并令V为子空间的补集。则 G 是其 Lie 子群 exp(E) 和 exp(V) 的直乘积；第一个是环面，第二个是向量。最后，G 的每个紧凑子群都包含在 exp(E) 中（因为它的投影到 exp(V) 必然减少到单位元素）；因此，子群 exp(E) 是 G 的唯一最大紧致子群。

对于例，取$G = C^*$； 认同 L(G) 和 $\mathbf{C}$，使得 G 的指数映射为 $x \rightarrow e^x$。然后 $\Gamma (G) = 2\pi i\mathbf{Z},E =i\mathbf{R}$，所以 exp(E) $=\mathbf{U}$；如果我们取 $V =\mathbf{R}$，则 exp(V) $=\mathbf{R}^*_+$，我们恢复在一般拓扑，第 1 章中构造的同构 $\mathbf{C}^*\rightarrow \mathbf{U}\times \mathbf{R}^*_+$。 VIII, §1, no. 3，提案 1。

d) 注最后，exp$_G: L(G)\rightarrow G$ 是 G 的全覆盖，因此 $\Gamma (G)$ 可以自然地等同于 G 的基本群。

### 3. 紧李代数

#### 命题 1 {#lie-ix-s1-prop-1 .statement tag=019D}

令 $\mathfrak{g}$ 为（实数）李代数。以下条件是等效的：

(i) $\mathfrak{g}$ 同构于紧李群的李代数。

(ii) 群 Int($\mathfrak{g}$)（第 III, §6, no. 2，定义 2）是紧凑的。

(iii) $\mathfrak{g}$ 有不变双线性形式（第I, §3, no. 6），它是对称的、正的且分离的。

(iv) $\mathfrak{g}$ 是还原性的（第 I, §6, no. 4 章，定义 4）；对于所有 $x\in \mathfrak{g}$、自同态和 $x$ 都是半单，而特征值纯粹是虚构的。

(v) $\mathfrak{g}$ 是还原性的，其 Killing 形式 B 是负值。

(i) $=\Rightarrow$ (ii)：如果 $\mathfrak{g}$ 是紧李群 G 的李代数，群 Int($\mathfrak{g}$) 是分离的并且同构于紧致群 $G_0$ 的商（第 1 章） III, §6, no. 4，Cor.4)，因此是紧凑的。

(ii) $=\Rightarrow$ (iii): 如果群 Int($\mathfrak{g}$) 是紧的，$\mathfrak{g}$ 上存在对称双线性形式，它在 Int($\mathfrak{g}$) (no. 1) 下是正的、分离且不变的，因此在伴随下也是不变的表示共 $\mathfrak{g}$。

(iii) $=\Rightarrow$ (iv)：如果满足(iii)，$\mathfrak{g}$的伴随表示是半单 (no. 1)，因而$\mathfrak{g}$是可还原的；此外，自同态和$x$，对于$x\in \mathfrak{g}$，具有指定的属性（no. 1）。

(iv) $=\Rightarrow$ (v)：对于所有 $x\in \mathfrak{g}, B(x, x) =$ Tr((ad $x$)$^2$)；因而，$B(x, x)$是广告$x$的平方或特征值的和，因此如果这些纯粹是虚构的，则为负数。

(v) $=\Rightarrow$ (i)：假设 $\mathfrak{g}$ 是还原性的，因此交换子代数 $\mathfrak{c}$ 和半单子代数 $\mathfrak{s}$ 的乘积（第 I, §6, no. 4 章，第 5 条）。 $\mathfrak{s}$的杀戮形式是形式B到$\mathfrak{s}$的限制，因此是负数并且如果B是负数则分离。 $\mathbf{G}\mathbf{L}(\mathfrak{s})$ 的子群 Int($\mathfrak{s}$) 是封闭的（它是 Aut($\mathfrak{s}$) 的恒等分量，第 III, §10, no. 2，Cor. 2），并且使分离正形式 $-B$ 不变；因而，它是紧致的，并且$\mathfrak{s}$同构于紧李群Int($\mathfrak{s}$)的李代数。此外，由于$\mathfrak{c}$是可交换的，它与环面T的李代数同构。因而，$\mathfrak{g}$与紧李群Int($\mathfrak{s}$)$\times T$的李代数同构。

#### 定义 1 {#lie-ix-s1-def-1 .statement tag=019E}

紧李代数$^4$是李代数，其具有命题1的性质(i)至(v)。

因而，紧李代数是交换代数的乘积以及紧凑的半单代数。在其他字中，李代数是紧的当且仅当它是约简的并且它的派生李代数是紧的。

紧李群的李代数是紧的。

#### 命题 2 {#lie-ix-s1-prop-2 .statement tag=019F}

a) 李代数的有限数的乘积是紧李代数当且仅当每个因子都是紧的。

b) 紧李代数的子代数是紧的。

c) 令$\mathfrak{h}$为紧李代数$\mathfrak{g}$的理想。那么代数 $\mathfrak{g}/\mathfrak{h}$ 是紧致的，扩张 $\mathfrak{h}\rightarrow \mathfrak{g}\rightarrow \mathfrak{g}/\mathfrak{h}$ 是平凡的。

断言 a) 和 b) 由命题 1 的刻画 (iii) 得出。部分 c) 由 a) 得出，并且事实上，在还原的李代数中，每个理想都是直因子（第 I, §6, no. 4 章，命题 5 的修正）。

#### 命题 3 {#lie-ix-s1-prop-3 .statement tag=019G}

令 G 为李群，其中连通分量的群是有限的。以下条件是等价的：

(i) 李代数 L(G) 是紧的。

(ii) 群 Ad(G) 是紧凑的。

(iii) 在 G 的伴随表示下，L(G) 不变量存在分离正对称双线性形式。

\*(iv) G 在左右平移下具有黎曼度量不变量。\​​

(i) $=\Rightarrow$ (ii)：如果 L(G) 是紧的，则群 Ad(G$_0$) $=$ Int(L(G)) 是紧的；由于 Ad(G) 中的指标是有限的，因此后者群也是紧凑的。

(ii) $=\Rightarrow$ (iii)：这是从no. 1得出的。

(iii) $=\Rightarrow$ (i)：由于 Int(L(G)) $\subset$ Ad(G)，这由命题 1 的刻画 (iii) 得出。

\*(iii) $\Leftarrow \Rightarrow$ (iv)：这来自第 1 章。 III, §3, no. 13.\*

### 4. 群李代数是紧凑的

#### 定理 1 {#lie-ix-s1-thm-1 .statement tag=019H}

(H. Weyl) 设 G 是一个连通的李群，其李代数是紧致的半单。那么 G 是紧致的，并且它的中心是有限的。

由于G是半单，所以它的中心D是离散的。此外，商群$G/D$同构于Ad(G)（第III, §6, no. 4章，Cor.4），因此是紧凑的（命题3）。最后，群$G/D$等于它的导出群（第III, §9, no. 2章，第4号提案的Cor.）。 定理现在来自集成，第 1 章。 VII, §3, no. 2，提案 5。

#### 命题 4 {#lie-ix-s1-prop-4 .statement tag=019I}

令 G 为连通的李群，其李代数是紧致的。存在环面 T，一个单连通紧半单李

$^4$ 注实拓扑向量空间不能是紧拓扑空间

除非减少到 0。 群 S、向量群 V 以及具有有限核的满射态射 $f: V\times T\times S\rightarrow G$。如果 G 是紧致的，群 V 会减少到单位元素。

令C（分别为S）为单连通李群，其李代数同构于L(G)的中心（分别为派生的代数）。那么 C 是向量群，S 是一个紧凑的群，具有有限的中心（Th.1），G 可以通过离散的子群 D 与 $C\times S$ 的商来识别，这是中心的（积分，第 VII, §3, no. 2 章， 引理4)。由于 D 的投影的像在 S 上是中心的，因此是有限的，$D\cap C$ 在 D 中是有限的指标。设 $C'$ 是由 $D\cap C$ 生成的 C 的向量子空间，而 V 是补数子空间。那么群$T = C'/(D\cap C)$就是环面，G同构于乘积群$V\times T\times S$除以有限群的商。

如果 G 是紧致的，那么 $V\times T\times S ($General 拓扑也是紧致的，第 1 章。 III, §4, no. 1，科。命题 2 的 2），因而 V 也是如此，这意味着 $V =\{e\}$。

#### 推论 1 {#lie-ix-s1-prop-4-cor-1 .statement tag=019J}

令 G 为连通的紧李群。那么$C(G)_0$就是环面，D(G)是一个连通紧致半单李群，而态射$(x, y) \rightarrow xy$从$C(G)_0\times D(G)$到G是一个有限覆盖。

根据命题4中的记号，我们有G的$V =\{e\}$和子群、$f(T)$和$f(S)$是紧的，因此是封闭的。因此只要证明$f(T) =$$C(G)_0,f(S) = D(G)$就足够了。现在，$L(G) = L(f(T))\times L(f(S))$；由于 S 是半单并且 T 是可交换的，这意味着 $L(f(T)) =\mathscr{C}(L(G)) = L(C(G)_0)$（第 III, §9, no. 3 章，第 8 条命题）和 $L(f(S)) =\mathscr{D}L(G) = L(D(G))$（第 III, §9, no. 2 章，第 4 条命题的修正），因此称为断言。

#### 推论 2 {#lie-ix-s1-prop-4-cor-2 .statement tag=019K}

中心和连通紧凑半单李群的基本群是有限的。其通用覆盖物结构紧凑。

有了第4号提案中的记号，群V和T减少到单位元素；因此S是G的全覆盖，G的基本群同构于Ker$f$，因此是有限的。 G 的中心 D 是离散的，因为 G 是半单，所以 D 是有限的。

#### 推论 3 {#lie-ix-s1-prop-4-cor-3 .statement tag=019L}

连接的紧李群 G 的基本群是有限型的 $\mathbf{Z}$ 模，秩等于 C(G) 的维数。

事实上，Cor 中的记号。 1，$C(G)_0$的基数群与$\mathbf{Z}^n$同构的，$n=$暗淡$C(G)_0$，并且D(G)的基数群是有限的（Cor.2）。

#### 推论 4 {#lie-ix-s1-prop-4-cor-4 .statement tag=019M}

令 G 为连通的紧李群。以下条件是等效的：

(i) G 为半单；

(ii) C(G) 是有限的；

(i) $\pi_1(G)$ 是有限的。

如果 G 是单连通的，则为半单。

这是从 Cor 得出的。 1 至 3。

#### 推论 5 {#lie-ix-s1-prop-4-cor-5 .statement tag=019N}

令 G 为连通的紧李群。那么 Int(G) 就是李群 Aut(G) 的恒等分量（第 III, §10, no. 2 章）。

设 $f\in$ Aut(G)$_0$。然后$C(G)_0$的$f$诱导自同构$f_1$和D(G)的自同构$f_2$，我们有$f_1\in$自动（C（G）$_0$）$_0, f_2\in$自动（D（G））$_0$。由于 Aut(C(G)$_0$) 是离散的（一般拓扑，第VII, §2, no. 4，第 5 章），我们有 $f_1=$ Id；因为 D(G) 是半单，由第 1 章给出。 III, §10, no. 2，科。 2 Th。 1 存在 D(G) 的元素 $g$，使得对于所有 $x\in$ D(G) 都有 $f_2(x) =gxg^{-1}$。对于所有 $x\in C(G)_0$，我们有 $gxg^{-1}=x$ = $f_1(x)$；从 $G = C(G)_0.D(G)$ 开始，$gxg^{-1}=f(x)$ 对于所有 $x\in G$，因此 $f=$ Int $g$。

#### 命题 5 {#lie-ix-s1-prop-5 .statement tag=019O}

令 G 为李群，其李代数是紧致的。

a) 假设G已连通。那么G有最大的紧子群K；它已连接。 G 存在一个闭中心向量子群 (no. 2) N，使得 G 是直乘积 $N\times K$。

b) 假设 G 的连通分量群是有限的。然后：

(i) G 的每个紧凑子群都包含在最大紧凑子群中。

(ii) 如果$K_1$和$K_2$是G的两个最大紧致子群，则存在$g\in G$使得$K_2=gK_1g^{-1}$。

(iii) 令K为G的最大紧致子群，则$K\cap G_0$等于$K_0$；它是最大的紧凑子群$G_0$。

(iv) 存在$G_0$的闭中心向量子群N，在G中正常，因此，对于G的任何最大紧致子群K，$G_0$是N对$K_0$的直乘积，G是半直K 乘 N 的乘积。

a) 我们保留第 4 条的记号。Ker $f$ 到V 的投影是向量群 V 的有限子群，因此减少到单位元素。由此可知 Ker $f$ 包含在 $T\times S$ 中，因此 G 是向量群 $N =f(V)$ 的直接乘积和紧致群 $K =f(T\times S)$。 G 的每个紧致子群都有投影到 N 上，N 被约简为单位元素，因此包含在 K 中。这证明了 a)。

b) 现在假设 $G/G_0$ 是有限的。由$a), G_0$是其最大的紧致子群M和向量子群P的直接乘积； G 的子群 M 显然是正常的。令$\mathfrak{n}$为L(G)中L(M)的向量子空间补，在G的伴随表示下稳定（no. 1和no. 3，命题3）；这是L(G) 的理想，我们有$L(G) = L(M)\times \mathfrak{n}$。令 N 为 G 与李代数 $\mathfrak{n}$ 的积分子群；由章。 III, §6, no. 6，第 14 条命题，在 G 中是正常的。L(G) 的投影到 L(P)，其中核 L(M) 诱导同构从 $\mathfrak{n}$ 到L(P);由此可见，$G_0$的投影到P诱导，一个从N到P的étale态射；由于 P 是单连通的，因此为同构，N 为向量群。从$M\times N$到$G_0$的态射$(x, y) \rightarrow xy$是一个单射étale态射（因为$M\cap N$减少到单位元素），因此同构。由此可见，N 是 G 的闭子群，并且商 $G/N$ 是紧致的，因为 $G_0/N$ 是紧致的，而 $G/G_0$ 是有限的（一般拓扑，第 III, §4, no. 1，第 2 条命题的 Cor.2）。

通过整合，第 1 章。 VII, §3, no. 2，命题 3，G 的每个紧致子群都包含在最大紧致子群中，即共轭，并且对于 G 的任何最大紧致子群 K，G 是 K 与 N 的半直接乘积。因为 $G_0$ 包含于 N，是N乘$G_0\cap K$的半直接乘积；由此可见，$G_0\cap K$是连通的，因此等于$K_0$，因为$K/(G_0\cap K)$与$G/G_0$同构的，因此是有限的；最后，$K_0$ 显然是 $G_0$ 的最大的紧致子群 by a)。

#### 推论{#lie-ix-s1-n4-cor-1 .statement tag=019P}

如果 N 满足 b) (iv) 的条件，且$K_1$ 和 $K_2$ 是 G 的两个最大紧致子群，则存在$n\in$ N 使得 $nK_1n^{-1}= K_2$。

事实上，通过 (ii) 存在元素$g\in G$使得$gK_1g^{-1}= K_2$；由(iv)，存在$n\in N$和$k\in K_1$使得$g=nk$。 元素 $n$ 则具有所需的属性。

### 习题{#lie-ix-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
