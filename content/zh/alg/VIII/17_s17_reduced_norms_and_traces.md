---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 17
section_title: Reduced Norms and Traces
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.335-A VIII.353
pdf_pages: 0352-0370
extraction: native+ocr
subsections:
    - "no": 1
      title: Complements on Characteristic Polynomials
      page: 335
      pdf_page: 352
    - "no": 2
      title: Reduced Norms and Traces
      page: 339
      pdf_page: 356
    - "no": 3
      title: Properties of Reduced Norms and Traces
      page: 341
      pdf_page: 358
    - "no": 4
      title: The Reduced Norm is a Polynomial Function
      page: 344
      pdf_page: 361
    - "no": 5
      title: Transitivity of Reduced Norms and Traces
      page: 346
      pdf_page: 363
    - "no": 6
      title: Reduced Norms and Determinants
      page: 349
      pdf_page: 366
statements: 31
exercises: 7
content_sha256: af046eaf2c8018edbf2c1cfce69fee658b499c6799e6896e139880de0973e4a6
translated_from: content/en/alg/VIII/17_s17_reduced_norms_and_traces.md
translation_method: google
source_content_sha256: 08c1f7f51bd2df11d29e638f229d1b484c7cda3e1bc21277c413e8819b54daaf
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 7580aabb05df2b12e293fff457ded10a046e56b398602379dd93ef83d826fe57
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 17。 简化范数与迹

在这个截面中，K是交换域，A中心单K-代数是有限次数。我们将 A 的减少的次数表示为 $n$。

### 1. 特征多项式的补集

设L为交换环，M为有限秩$m$的自由L模。如果$u$是M的自同态且$r$自然数，那么我们用$c_r(u)$表示自由L模块$\wedge^r(M)$的自同态$\wedge^r(u)$的踪迹。特别是，我们有

(1) $c_0(u) = 1,c_1(u) =$ Tr($u$)$,c_m(u) =$ det($u$),

$c_r(u) = 0$ 代表 $r > m$。 由 III, §8, No. 4、p. 527、映射 $u\mapsto$ det($u$) 从 End(M) 到 L 的命题 7 是次数 $m$ 齐次多项式映射 (IV, §5, No. 9, p. 55）。 更一般地，对于每个整数$r$，使得从End(M)到L的$0\leqslant r\leqslant m$、映射$c_r$是次数$r$的齐次多项式映射；这是从 III, §8, No. 5、p. 529 中的命题 10 得出的。

令 $u$ 为 M 的自同态，$\overline{u}$ 自同态为 L[X]模 $M[X] = M\otimes_LL[X]$ 由$u$ 通过标量扩张推导出来 (II, §5, No. 1， p. 277）。回想一下 (III, §8, No. 11, p. 541, 定义 3 和 (50))，$u$ 的特征多项式是 M[X] 的 L[X]自同态 $X-\overline{u}$ 的行列式 $\chi_u(X)$，并且我们有关系

$$
\chi_u(X) =\sum_{r=0}^m(-1)^rc_r(u) X^{m-r} \tag{2}
$$

#### 命题 1 {#alg-viii-s17-prop-1 .statement tag=00KD}

设L为交换环，M为有限秩m$\geqslant 1$的自由L模，且M的u自同态。存在M满足关系的唯一内同态$\tilde{u}$

$$
\tilde{u}(x) \wedge w = x \wedge \wedge^{m-1}(u)(w)
$$

对于 $x \in M$ 和 $w \in \wedge^{m-1}(M)$。此外，我们还有关系

$$
u \circ \tilde{u} = \tilde{u} \circ u = \det(u)_M,
$$
$$
\det(\tilde{u}) = \det(u)^{m-1},
$$
$$
\tilde{u} = \sum_{r=0}^{m-1} (-1)^r c_{m-1-r}(u) u^r.
$$

#### 引理 1 {#alg-viii-s17-lem-1 .statement tag=00KE}

令 p 为整数，使得 $0 \leqslant p \leqslant m$。对于$\wedge^p(M)$中的任何w，令$h_p(w)$为从$\wedge^{m-p}(M)$到$\wedge^m(M)$的线性映射$w' \mapsto w \wedge w'$。 线性映射$h_p : w \mapsto h_p(w)$从$\wedge^p(M)$到$\operatorname{Hom}_L(\wedge^{m-p}(M), \wedge^m(M))$是同构。

令$(e_i)_{i \in I}$为M的基；我们赋予集合I总共阶。对于I、集合$e_J = e_{i_1} \wedge \cdots \wedge e_{i_r}$的任何子集 J，其中$(i_1, \ldots, i_r)$是递增阶中J的元素的序列。 L模$\wedge^{m-p}(M)$承认为基元素$e_S$，其中S通过I的子集的集合和$m - p$元素； $\wedge^m(M)$ $\{e_I\}$ 为基。因而，存在 $\operatorname{Hom}_L(\wedge^{m-p}(M), \wedge^m(M))$ 由……组成线性映射 $e_J^*$ 的基，其特征为公式

$$
e_J^*(e_S) = \begin{cases}
e_I & \text{if } I = J \cup S, \\
0 & \text{otherwise},
\end{cases}
$$

其中 J 穿过集合或子集或 I，其中 p 元素。从 III, §7, No. 8、p. 519 的公式 (20) 可以得出，对于 I 的每一个子集 J 以及 p 元素，我们有 $h_p(e_J) \in \{e_J^*, -e_J^*\}$；由于$\wedge^p(M)$的元素$e_J$形式基，线性映射$h_p$是双射的。

现在让我们证明命题 1。令 u 和 $\tilde{u}$ 为 M 的自同态。关系 (3) 等价于

$$
h_1 \circ \tilde{u} = \operatorname{Hom}(\wedge^{m-1}(u) \cdot 1_{\wedge^m(M)}) \circ h_1;
$$

映射$h_1$是从M到$\operatorname{Hom}_L(\wedge^{m-1}(M), \wedge^m(M))$乘引理1的同构。因而，对于M的每个自同态u，都存在M满足关系的唯一内同态$\tilde{u}$ (3)。

令$x_1, . . . , x_m$为M的元素。让我们在(3)中将替换$x$与$u(x_1)$以及$w$与$x_2\wedge  \cdots  \wedge x_m$进行计算；我们得到

$\widetilde{u}(u(x_1))\wedge x_2\wedge  \cdots  \wedge x_m=u(x_1)\wedge  \cdots  \wedge u(x_m) =$ det($u$)$x_1\wedge  \cdots  \wedge x_m$。

因而，$h_1(\widetilde{u}\circ u(x_1)) =h_1$(det($u$)$x_1$)，通过引理 1 得到关系 $\widetilde{u}\circ u=$ det($u$)$_M$。

我们用U自同态$X-\overline{u}$表示L[X]-模块M[X]（VIII，p. 335）。将上述应用于U，存在满足关系的L[X]-模块M[X]的自同态$\widetilde{U}$

$$
\widetilde{U}(x_1)\wedge x_2\wedge  \cdots  \wedge x_m=x_1\wedge (Xx_2-u(x_2))\wedge  \cdots  \wedge (Xx_m-u(x_m)) \tag{9}
$$

对于 M 中的 $x_1, . . . , x_m$ 和

(10)$\widetilde{U}\circ U =$det(X$-\overline{u}$)$_{M[X]}$。

让我们将 $\widetilde{U}$ 视为 End(M)[X] 的元素 (VIII, p. 9);通过公式 (9) 和引理 1，它有次数 $\leqslant m-1$，所以我们可以将其写为

$$
\widetilde{U} =\sum^{m-1}_{r=0}(-1)^ru_rX^{m-1-r} \tag{11}
$$

其中$u_r$是M的自同态。通过公式(2)，关系(10)给出等式

$$
(\sum^{m-1}_{r=0}(-1)^ru_rX^{m-1-r})(X-u) =\sum_{r=0}^m(-1)^rc_r(u)X^{m-r} \tag{12}
$$

在环结束(M)[X]。通过求X各边的单项式系数，我们得到关系

(13) $u_r+u_{r-1}\circ u=c_r(u)_M$ 为 $1\leqslant r\leqslant m-1$

和

$$
u_0=c_0(u)_M,u_{m-1}\circ u=c_m(u)_M \tag{14}
$$

由此，我们推论

$$
u_{m-1}=\sum^{m-1}_{r=0}(-1)^rc_{m-1-r}(u)u^r \tag{15}
$$

现在，当我们认同常数项时，等式（9）和（11）意味着$u_{m-1}=\widetilde{u}$； 公式 (6)如下。

特别是，$u$生成的End(M)的$\widetilde{u}$属于到子代数，因此与$u$交换。我们已经建立了关系 $\widetilde{u}\circ u=$ det($u$)$_M$； 公式 (4)如下。

最后，令$x_1, . . . , x_m$为M的元素。我们在公式(3)中将替换$x$与$x_1$以及$w$与$\widetilde{u}(x_2)\wedge  \cdots  \wedge \widetilde{u}(x_m)$进行组合。这给出了

$$
\widetilde{u}(x_1)\wedge \widetilde{u}(x_2)\wedge  \cdots  \wedge \widetilde{u}(x_m) =x_1\wedge u\circ (\widetilde{u}(x_2))\wedge  \cdots  \wedge u\circ (\widetilde{u}(x_m))
$$

= det($u$)$^{m-1}x_1\wedge x_2\wedge  \cdots  \wedge x_m$

因此公式 (5)。

#### 注 1 {#alg-viii-s17-n1-rem-1 .statement tag=00KF}

M 重合的自同态 $\widetilde{u}$ 与我们所说的III, §8, No. 6、p. 532 中$u$ 的共转置。

#### 注 2 {#alg-viii-s17-n1-rem-2 .statement tag=00KG}

从公式 (1)、(2)、(4) 和 (6)，我们推导出关系 $\chi_u(u) = 0$，从而推导出凯利-汉密尔顿定理 (III, §8, No. 11，p. 541) 的另一个证明。

#### 注 3 {#alg-viii-s17-n1-rem-3 .statement tag=00KH}

由于从 End(M) 到 L 的映射 $c_r$ 是 $0\leqslant r\leqslant m-1$ 的次数 $r$ 的齐次多项式映射，因此从公式 (6) 可以得出映射 $u\mapsto \widetilde{u}$ End(M) 到 End(M) 是次数 $m-1$ 中的齐次多项式映射。

设 B 为代数大于环 L；假设 B 是秩 $m\geqslant 1$ 的自由 L 模，且认同 L 以及 B 的子环 $L\cdot 1$。令 $b$ 为 B 的元素。我们将上述应用于自同态 L-模块 B 的$\gamma (b) :x\mapsto bx$。集合 $\gamma_r(b) =c_r(\gamma (b))$ 对于$0\leqslant r\leqslant m$；我们特别有 $\gamma_m(b) = N_{B/L}(b)$ (III, §9, No. 3, p. 543)。 $b$（参见上文）的特征多项式可以写为

（16）PC$_{B/L}(b; X) =\sum_{r=0}^m(-1)^r\gamma_r(b) X^{m-r}$。

由于从B到End$_L(B)$的映射$\gamma$是L线性，因此从B到L的映射$\gamma_r$是次数$r$的齐次多项式映射。特别地，从B到L的映射$b\mapsto N_{B/L}(b)$是次数$m$中的齐次多项式映射。

对于 B 的任意元素 $b$，集合

$$
\widetilde{b}=\sum^{m-1}_{r=0}(-1)^r\gamma_{m-1-r}(b)b^r \tag{17}
$$

由命题 1，从B到B的线性映射$\gamma (\widetilde{b})$是映射$\gamma (b)$的转置；由此，我们推论

$$
b\widetilde{b}=\widetilde{b}b= N_{B/L}(b) \tag{18}
$$

另外，从B到B的映射$b\mapsto \widetilde{b}$是次数$m-1$中的齐次多项式映射。

### 2. 简化范数与迹

回想一下，我们用 A 表示在交换域 K 上减少的次数 $n$ 的中心单代数。

#### 命题 2 {#alg-viii-s17-prop-2 .statement tag=00KI}

设$a$为A的元素，Pc($a; X$)为其特征多项式。 K[X] 中存在唯一的一元多项式 P，使得我们有 Pc($a; X$) $= P(X)^n$。

A) P 的唯一性由下面的引理 2 得出。

#### 引理 2 {#alg-viii-s17-lem-2 .statement tag=00KJ}

令 P 和 Q 为 K[X] 中的单调多项式，$s$ 是严格的正整数。如果 $P^s= Q^s$，那么我们有 P = Q。

令 $\mathscr{I}$ 为 K[X] 中不可约模多项式的集合。由于 P 和 Q 是单调的，因此存在 $\mathbf{N}^{(\mathscr{I})}$ 的元素 $(a_F)$ 和 $(b_F)$，因此我们有 $P =\prod_{F\in\mathscr{I}}F^{a_F}$ 和 $Q =\prod_{F\in\mathscr{I}}F^{b_F}$。从等式$P^s= Q^s$和分解的唯一性到不可约的因子，我们对每个$F\in \mathscr{I}$都有$sa_F=sb_F$。由于$s$严格为正，因此对于每个$F\in \mathscr{I}$我们都有$a_F=b_F$，因此P = Q。

B) 现在让我们证明 P 的存在性。

由VIII、p. 252的定理 1，存在有限次数的K的伽罗瓦扩张L和L代数$\theta : A_{(L)}\rightarrow \mathbf{M}_n(L)$的同构。由III, §9, No. 1、p. 542的公式(12)，多项式Pc($a; X$)也是L-代数$A_{(L)}$的元素$1\otimes a$的特征多项式，因此为元素 L代数$\mathbf{M}_n(L)$的$\theta (1\otimes a)$。

集合 P(X) = det(X$I_n-\theta (1\otimes a)$);它是 L[X] 中的一元多项式。到例 3 of III, §9, No. 3, p. 545，我们有

（19）电脑（$a; X$）$= P(X)^n$。

设G为K上的L伽罗瓦群。对于$\sigma \in G$，用环L[X]$\overline{\sigma}$自同构表示重合和L上的$\sigma$并固定X。那么 K[X] 是 L[X] 的多项式 Q 的集合，这样对于每个 $\sigma \in G$，我们都有 $\overline{\sigma}(Q) = Q$（V, §10, No. 1、p. 56、定理 1）。由于多项式 Pc($a; X$) $= P(X)^n$ 属于到 K[X]，对于每个$\sigma \in G$，我们有 $\overline{\sigma}(P)^n= P^n$。因此，到引理 2 时，每 $\sigma \in G$ 就有 $\overline{\sigma}(P) = P$，因此 P 属于到 K[X]。

#### 定义 1 {#alg-viii-s17-def-1 .statement tag=00RM}

令$a$为代数A的元素。$a$（相对于A）的约简特征多项式是K[X]中唯一的一元多项式，记为Pcrd$_{A/K}(a; X)$，满足关系

(20) Pc$_{A/K}(a; X) =$ Pcrd$_{A/K}(a; X)^n$。

设$a$为A的元素，由于A在K上有次数$n^2$，所以多项式Pc$_{A/K}(a; X)$有次数$n^2$，所以Pcrd$_{A/K}(a; X)$是次数$n$的一调多项式；让我们把它写成

（21）Pcrd$_{A/K}(a; X) = X^n+\sum^{n-1}_{r=0}(-1)^rb_r(a)X^{n-r}$。

我们集合

(22) Trd$_{A/K}(a) =b_1(a)$，Nrd$_{A/K}(a) =b_n(a)$。

#### 定义 2 {#alg-viii-s17-def-2 .statement tag=00KK}

我们称 A 的 Trd$_{A/K}(a)$ 约化迹和 Nrd$_{A/K}(a)$ 为约化范数（相对于 K-代数 A）。

当不存在混淆风险时，我们将 A 和 K 从记号中去掉，只写 Pcrd($a; X$)、Trd($a$) 和 Nrd($a$)。

以下公式由III, §9, No. 1、p. 542的公式(20)和(22)以及公式(7)和(8)得出：

（23）Tr$_{A/K}(a) =n$Trd$_{A/K}(a)$，

（24）$N_{A/K}(a) =$（Nrd$_{A/K}(a)$）$^n$。

#### 命题 3 {#alg-viii-s17-prop-3 .statement tag=00KL}

A 的元素 $a$ 可逆当且仅当其约化范数为非零的。特别是，当且仅当 A 的每个非零元素 $a$ 都有 Nrd$_{A/K}(a)\not= 0$ 时，A 才是域。

A 的元素 $a$ 可逆当且仅当其范数为非零的 (III, §9, No. 4, p. 545, 命题 3)。因此，命题 3 由公式 (24) 得出。

#### 注 {#alg-viii-s17-n2-rem-1 .statement tag=00KM}

令 L 为 X 中有理分式的域 K(X)。 A 的元素 $a$ 的约化特征多项式就是 L 代数 $A_{(L)}$ 的元素 $X\otimes 1-1\otimes a$ 的约化范数。这是从简化特征多项式的定义和公式 (III, §9, No. 3, p. 544) 得出的

（25）PC$_{A/K}(a; X) = N_{A_{(L)}/L}(X\otimes 1-1\otimes a)$。

#### 例 1 {#alg-viii-s17-n2-exa-1 .statement tag=00RN}

由VIII、p. 120的定理 1，存在整数$r\geqslant 1$和域D，使得A与$\mathbf{M}_r(D)$同构。令 $d$ 为 D 对 K 的约化次数；我们有$r=n/d$。设M为有限长度$\ell$中的A-模；我们将证明公式

(26) Pc$_{M/K}(a_M; X) =$ Pcrd$_{A/K}(a; X)^{d\ell}$

对于 A. A-模 $A_s$ 的每个元素 $a$ 有长度 $r$ (VIII, p. 121, 引理 2)。 A-模 $M^r$ 和 $A^{\ell}_s$ 具有相同的长度，所以它们是同构的，我们有

电脑$_{M/K}(a_M; X)^r=$ 电脑$_{A/K}(a; X)^{\ell}$

由 III, §9, No. 2、p. 542 的公式 (15) 得出。由于我们有 $rd=n$，公式 (26) 由公式 (20) 和引理 2 (VIII，p. 339) 得出。

#### 例 2 {#alg-viii-s17-n2-exa-2 .statement tag=00RO}

考虑当A是有限维K-向量空间V的自同态的代数End$_K(V)$时的具体情况。取M为单A-模V，可得关系

Pcrd$_{A/K}(u; X) =\chi_u(X)$,

(27) Nrd$_{A/K}(u) =$ det($u$),

Trd$_{A/K}(u) =$ Tr($u$)

每自同态 $u$ V。

### 3. 简化范数与迹的性质

#### 命题 4 {#alg-viii-s17-prop-4 .statement tag=00KN}

设L为K的扩张和中心单代数A的$a$元素。我们有关系

(28) Pcrd$_{A_{(L)}/L}(1\otimes a; X) =$ Pcrd$_{A/K}(a; X)$,

（29）Trd$_{A_{(L)}/L}(1\otimes a) =$Trd$_{A/K}(a)$，

(30) Nrd$_{A_{(L)}/L}(1\otimes a) =$ Nrd$_{A/K}(a)$

（“标量在扩张下的不变性”）。

等式(28)的两侧有相同的$n$第幂乘以定义(VIII、p. 340的公式(20))和关系

Pc$_{A_{(L)}/L}(1\otimes a; X) =$ Pc$_{A/K}(a; X)$（III, §9, No. 3，p. 544，公式（21））。因此，等式 (28) 由VIII、p. 339 中的引理 2 得出。 公式 (29) 和 (30) 由 (28)、(21) 和 (22) 得出。

#### 推论 1 {#alg-viii-s17-prop-4-cor-1 .statement tag=00KO}

令L为K的扩张。令V为从A到L和$\theta$K-代数同态的维数$n$的向量空间到结束$_L(V)$。对于 A 的每个元素 $a$，我们有

（31）Pcrd$_{A/K}(a; X) =\chi_{\theta(a)}(X)$，

（32）Trd$_{A/K}(a) =$Tr（$\theta (a)$），

（33）Nrd$_{A/K}(a) =$det（$\theta (a)$）。

令$\theta '$为从$A_{(L)}$到End$_L(V)$的L代数同态，使得$\theta '(\lambda \otimes a) =\lambda \theta (a)$对应于$\lambda \in L$和$a\in A$。 代数 $A_{(L)}$ 由VIII、p. 222的推论2简单；因此同态 $\theta '$ 是单射的。但是代数$A_{(L)}$和域L上的End$_L(V)$具有相同的次数，等于$n^2$，所以$\theta '$是同构。然后从上面的命题4和例2得出推论1。

#### 推论 2 {#alg-viii-s17-prop-4-cor-2 .statement tag=00KP}

设$a$和$a'$为A的元素和K的$\lambda$元素。我们有关系

（34）Pcrd$_{A/K}(a;a) = 0$，

（35）Pcrd$_{A/K}(\lambda a;\lambda X) =\lambda^n$ Pcrd$_{A/K}(a; X)$，

（36）Trd$_{A/K}(a+a') =$Trd$_{A/K}(a) +$Trd$_{A/K}(a')$，

Trd$_{A/K}(\lambda a) =\lambda$ Trd$_{A/K}(a)$,

(37) 特德$_{A/K}(aa') =$ 特德$_{A/K}(a'a)$,

(38) Nrd$_{A/K}(aa') =$ Nrd$_{A/K}(a)\cdot$ Nrd$_{A/K}(a')$,

Nrd$_{A/K}(\lambda a) =\lambda^n$ Nrd$_{A/K}(a)$,

（39）Trd$_{A/K}(1) =n$，Nrd$_{A/K}(1) = 1$。

由于 A 是中心简单且已在 K 上约简次数 $n$，因此存在 K 的扩张 L 和 L 上的维数 $n$ 的向量空间 V，使得 $A_{(L)}$ 为同构于代数 End$_L(V)$ (VIII, p. 252, 定理 1)。然后推论 2 由推论 1 以及自同态的迹和行列式的性质得出。特别是，公式 (34) 源自 Cayley–Hamilton 定理（III, §8, No. 11、p. 541、命题 20、cf. 以及VIII、p. 338、注 2）。

#### 推论 3 {#alg-viii-s17-prop-4-cor-3 .statement tag=00RP}

令 $A^o$ 为 A 的反代数。对于 A 中的每个 $a$，我们有

(40) Pcrd$_{A^o/K}(a; X) =$ Pcrd$_{A/K}(a; X)$,

(41) Trd$_{A^o/K}(a) =$ Trd$_{A/K}(a)$,

(42) Nrd$_{A^o/K}(a) =$ Nrd$_{A/K}(a)$。

K 的选择扩张 L，L 上的维数 $n$ 向量空间 V，以及从 A 到 End$_L(V)$ 的同态 $\theta$ (VIII， p. 252、定理 1)。令$V^*$为V的对偶向量空间。将A的元素$a$发送到$V^*$的自同态$^t\theta (a)$的映射是从$A^o$到End$_L(V^*)$的K-代数同态。推论 3 由III, §8, No. 4、p. 528 的推论 1 和推论 3 推出。

因此，无论我们将$a$视为A的元素还是$A^o$的元素，$a$的迹范数和特征多项式都是相同的。当 A 不假设为中心简单（III, §9、p. 644、习题 1）时，这个性质并不总是成立。

#### 命题 5 {#alg-viii-s17-prop-5 .statement tag=00KQ}

对于 A 中的任何 $x$，令 $t_x$ 为 A 上的线性形式 $y\mapsto$ Trd$_{A/K}(xy)$。

a) 映射 $t:x\mapsto t_x$ 是从 A 到其对偶 Hom$_K(A,K)$ 的 $(A,A)$ 双模的同构。

b) 设 A 上的 $h$ 为线性形式。以下属性是等效的：

(i) 存在 K 的元素 $\lambda$ 使得 $h(x) =\lambda$ Trd$_{A/K}(x)$

对于每个$x\in A$。

(ii) 对于 A 中的所有 $x, y$，我们都有 $h(xy) =h(yx)$。

回想一下 (II, §1, No. 14, p. 225–226)，$A^*=$ Hom$_K(A,K)$ 上的 $(A$, A) 双模结构由关系定义

$$
\langle atb, c\rangle =\langle t, bca\rangle \tag{43}
$$

对于 $a, b, c\in A$ 和 $t\in A^*$。特别是，对于 A 中的每个 $x$，我们有

$\langle at_xb, c\rangle =\langle t_x, bca\rangle =$Trd$_{A/K}(xbca)$,

$\langle t_{axb}, c\rangle =$Trd$_{A/K}(axbc)$,

并且这两个元素等于VIII、p. 342的公式(37)。因此，我们有$at_xb=t_{axb}$，这意味着$t$是$(A$的同态，A)从A到$A^*$的双模。

我们从L代数$A_{(L)}$到矩阵代数$\mathbf{M}_n(L)$（VIII，p. 252）选择扩张L和域K和同构$\theta$， 定理1)。 我们认同向量空间$(A^*)_{(L)}$与向量空间$A_{(L)}$的对偶超过域L。 通过VIII、p. 341的命题 4，根据这些约定，我们有

（44）Trd$_{A_{(L)}/L}= 1_L\otimes$Trd$_{A/K}$。

设$t_{(L)}$为从$A_{(L)}$到$A^*_{(L)}$的L线性映射，由$t$通过扩张标量推导出来；由公式 (44) 和推论 1，我们有

(45) $\langle t_{(L)}(x), y\rangle =$Trd$_{A_{(L)}/L}(xy) =$Tr($\theta (x)\theta (y)$)

对于$A_{(L)}$中的$x, y$。由II, §10, No. 11、p. 358、映射$t_{(L)}$的命题7是双射；由此可见 $t$ 是双射的。我们已经证明了a）。

设$h$在$A^*$中；由上可知，A存在元素$a$，使得$h$等于$t_a$。由a），我们有

$$
h(xy)-h(yx) =t_a(xy-yx) =t_{ax}(y)-t_{xa}(y)
$$

因而，关系“A 中$x, y$的$h(xy) =h(yx)$”相当于“每个$x\in$ A 的$t_{ax-xa}= 0$”，并且通过证明的部分 a)，这意味着 $a$ 属于到中心 K A. 鉴于公式 (36)，这证明了 b)。

#### 推论{#alg-viii-s17-n3-cor-1 .statement tag=00KR}

由形式$xy-yx$的元素生成的A的线性子空间，其中$x$和$y$贯穿A，是超平面，核或非零的线性形式 Trd$_{A/K}$。

#### 注 {#alg-viii-s17-n3-rem-1 .statement tag=00KS}

到 VIII、p. 340 的公式 (23)，我们有

Tr$_{A/K}(a) =n$ Trd$_{A/K}(a)$

每$a\in A$。如果域 K 的特征等于 0 或素数数 $p$ 而不是除 $n$，那么我们可以用命题 5 中的迹来替换约化迹。 另一方面，如果 K 的特征是素数数除 $n$，那么每个 $a\in A$ 就有 Tr$_{A/K}(a) = 0$。

### 4. 约化范数是多项式函数

#### 引理 3 {#alg-viii-s17-lem-3 .statement tag=00KT}

令L为K的扩张，并令I为集合和$\mathbf{T}= (T_i)_{i\in I}$一系列变量。我们有$K(\mathbf{T})\cap L[\mathbf{T}] = K[\mathbf{T}]$。

令 P 和 Q 为 $K[\mathbf{T}]$ 和 $Q\not= 0$ 的元素。 $L[\mathbf{T}]$ 中 P = QR 的多项式 R 的系数是系数为 K 的线性方程的系统的解。 因而，如果存在一个使得 P = QR 的多项式 $R\in L[\mathbf{T}]$，则$K[\mathbf{T}]$ 中也存在一个 (II, §8, No. 5， p. 321、命题 6)。这就证明了包含$K(\mathbf{T})\cap L[\mathbf{T}]\subset K[\mathbf{T}]$；反向包含是显而易见的。

回想一下，A 的元素 $a$ 的简化特征多项式可以写为

（46）Pcrd$_{A/K}(a; X) =\sum_{r=0}^n(-1)^rb_r(a) X^{n-r}$

我们有

$b_0(a) = 1,b_1(a) =$Trd$_{A/K}(a),b_n(a) =$Nrd$_{A/K}(a)$。

#### 命题 6 {#alg-viii-s17-prop-6 .statement tag=00KU}

对于每个整数$r$，使得从A到K的$0\leqslant r\leqslant n$，映射$b_r$是齐次多项式映射 / 次数$r$。特别地，从A到K，约化范数是次数$n$中的齐次多项式映射。

令$(e_i)_{i\in I}$为A在K上的基和$\mathbf{T}= (T_i)_{i\in I}$一系列变量。

#### 引理 4 {#alg-viii-s17-lem-4 .statement tag=00KV}

设$u$为中心简单$K(\mathbf{T})$代数$A_{(K(\mathbf{T}))}$的元素$\sum_{i\in I}T_i\otimes e_i$。令 P 为 $u$ 的简化特征多项式。然后P属于到环$K[\mathbf{T}][X]$；视为环$K[\mathbf{T},X]$的元素，它是次数$n$的齐次。

我们对 K 进行选择扩张 L 以及从 $A_{(L)}$ 到 $\mathbf{M}_n(L)$ 的 L 代数同构 $\theta$。我们用$L(\mathbf{T})$的$\overline{\theta}: A_{(L(\mathbf{T}))}\rightarrow \mathbf{M}_n(L(\mathbf{T}))$同构表示-由标量扩张从$\theta$推导出来的代数。根据VIII、p. 342的推论1，我们有

（47）$P(X) =\chi_{\overline{\theta}(u)}(X) =$ det（X$I_n-\overline{\theta}(u)$）$=$ det$(XI_n-\sum_{i\in I}T_i\theta (1\otimes e_i))$。

从矩阵$\theta (1\otimes e_i)$属于到$\mathbf{M}_n$(L)，这个公式表明P是$L[\mathbf{T},X]$中次数$n$的齐次多项式。它也有属于到$K(\mathbf{T})[X]$，并且可以写成$P(X) =\sum_{j\geqslant 0}c_jX^j$，其中每个$c_j$属于到交$K(\mathbf{T})\cap L[\mathbf{T}]$。 引理 3 个，元素 $c_j$ 属于至 $K[\mathbf{T}]$ 各；接下来是引理 4。

#### 引理 5 {#alg-viii-s17-lem-5 .statement tag=00KW}

对于 K 的每一个扩张 $K'$ 和 ${K'}^I$ 的每一个元素 $(t_i)_{i\in I}$，我们有

（48）Pcrd$_{A_{(K')}/K'}(\sum_{i\in I}t_i\otimes e_i)= P((t_i)_{i\in I},X)$。

令$\varphi : K[\mathbf{T}]\rightarrow K'$为唯一的K-代数同态，对于每个$i\in I$将$T_i$发送到$t_i$；它在$K[\mathbf{T}$]代数的$K'$结构上定义。 $K'$-代数$A_{(K[\mathbf{T}])(K')}$可以用$A_{(K')}$（标量的扩张的传递性）来识别，其中元素$1\otimes (\sum T_i\otimes e_i)$可以用$A_{(K')}$的元素$\sum t_i\otimes e_i$来识别。我们用从$\varphi$推导出来的$\overline{\varphi}: K[\mathbf{T}][X]\rightarrow K'[X]$K-代数同态来表示。通过III, §9, No. 3、p. 544的公式(21)，$\sum t_i\otimes e_i$关于$K'$-代数$A_{(K')}$的特征多项式是像乘$\overline{\varphi}$关于$\sum T_i\otimes e_i$的特征多项式$K[\mathbf{T}$]-代数$A_{(K[\mathbf{T}])}$，即$P^n$。在其他字中，我们有

（49）PC$_{A_{(K')}/K'}(\sum_{i\in I}t_i\otimes e_i; X)= P((t_i)_{i\in I},X)^n$；

然后从 VIII、p. 339 的引理 2 得出引理 5。

考虑引理 5 的具体情况 $K'= K$。我们有

（50）Pcrd$_{A/K}(\sum_{i\in I}t_ie_i; X)= P((t_i)_{i\in I},X)$

每元素 $(t_i)_{i\in I}$ 共 $K^I$。由于 $K[\mathbf{T},X]$ 中的多项式 P 是次数 $n$ 的齐次，因此它可以唯一展开为

$$
P(\mathbf{T},X) =\sum_{r=0}^n(-1)^rB_r(\mathbf{T}) X^{n-r} \tag{51}
$$

其中$B_r$是次数$r$在$K[\mathbf{T}]$中的齐次多项式。到公式 (46)、(50) 和 (51)，我们有

$$
b_r(\sum_{i\in I}t_ie_i)= B_r((t_i)_{i\in I})
$$

每元素$(t_i)_{i\in I}$共$K^I$。接下来是命题6。

#### 注 {#alg-viii-s17-n4-rem-1 .statement tag=00KX}

设$K'$为交换K-代数。 $A_{(K')}$的每个元素$t$都可以写成$\sum_{i\in I}t_i\otimes e_i$，其中$(t_i)\in {K'}^I$。由引理 5 的证明可知，特征多项式Pc$_{A_{(K')}/K'}(t; X)$等于$P((t_i),X)^n$。

### 5. 传递性 / 简化范数与迹

#### 命题 7 {#alg-viii-s17-prop-7 .statement tag=00KY}

令 L 为 A 的最大交换律半单子代数和 L 的 $a$ 元素。我们有

(52) Pcrd$_{A/K}(a; X) =$ Pc$_{L/K}(a; X)$，

（53）Trd$_{A/K}(a) =$Tr$_{L/K}(a)$，

（54）ND$_{A/K}(a) = N_{L/K}(a)$。

由VIII、p. 262中的命题 3，L模A与$L^n$同构的；因此我们有关系

电脑$_{A/K}(a; X) =$ 电脑$_{L/K}(a; X)^n$。

由于多项式 Pc$_{L/K}(a; X)$ 是单次的，因此它等于约简特征多项式 Pcrd$_{A/K}(a; X)$ (VIII, p. 339, 引理 2)；这给出公式 (52)。通过比较 (52) 两侧的 $X^{n-1}$（分别为常数项）的系数，我们得到公式 (53)（分别为 (54)）。

#### 推论{#alg-viii-s17-n5-cor-1 .statement tag=00KZ}

令 D 为 K 上有限次数的域，且具有中心 K。令 $a$ 为 K 的元素，且 D 包含 $a$ 的L 极大交换子域。我们有

Pcrd$_{D/K}(a; X) =$ Pc$_{L/K}(a; X)$,

(55) Tr$_{D/K}(a) =$ Tr$_{L/K}(a)$，

Nrd$_{D/K}(a) = N_{L/K}(a)$。

事实上，根据 VIII、p. 265 的推论 2，D 的极大交换子域 L 是 D 的最大交换律半单子代数。

#### 命题 8 {#alg-viii-s17-prop-8 .statement tag=00L0}

设B为A的单子代数。用L表示B的中心，用$B'$表示A中B的交换子。那么$B'$是域L的中心单代数；我们将次数减少了$r$。对于 B 的每个元素 $b$，我们有关系

（56）Pcrd$_{A/K}(b; X) = N_{L[X]/K[X]}$（Pcrd$_{B/L}(b; X)$）$^r$，

(57) Trd$_{A/K}(b) =r$ Tr$_{L/K}$(Trd$_{B/K}(b)$),

（58）Nrd$_{A/K}(b) = N_{L/K}$（Nrd$_{B/L}(b)$）$^r$。

#### 引理 6 {#alg-viii-s17-lem-6 .statement tag=00L1}

令 $K'$ 为 K 上的有限次数 $d$ 中的交换代数，并且

$$
P(X) = X^s+a_1X^{s-1}+\cdots +a_s
$$

系数为 $K'$ 的一元多项式。那么K[X]中的多项式Q = $N_{K'[X]/K[X]}(P)$是次数$sd$的mononic，Q(X)中$X^{sd-1}$的系数等于Tr$_{K'/K}(a_1)$，Q的常数项是$N_{K'/K}(a_s)$。

我们用$K''$表示$K'$-代数$K'[T]/(P(T))$，用$t$表示$K''$中T的规范类。 $K'$序列$(1, t, . . . , t^{s-1})$$K''$基，其中基形式乘法矩阵由$t$

$$
\tau = \begin{pmatrix}
0 & 0 & \cdots & 0 & -a_s \\
1 & 0 & \cdots & 0 & -a_{s-1} \\
0 & 1 & \cdots & 0 & -a_{s-2} \\
\vdots & \vdots & \ddots & \vdots & \vdots \\
0 & \cdots & \cdots & 1 & -a_1
\end{pmatrix}.
$$

$XI_n - \tau$ 的行列式由 $s$ 上的归纳沿第一行展开计算得出。我们得到$\det(XI_n - \tau) = P(X)$。在其他字中，我们有$P(X) = Pc_{K''/K'}(t; X)$。特别是$\operatorname{Tr}_{K''/K'}(t) = -a_1$和$N_{K''/K'}(t) = (-1)^s a_s$。通过传递性公式（III, §9, No. 4，p. 548，推论），我们有

$$
\operatorname{Tr}_{K''/K}(t) = -\operatorname{Tr}_{K'/K}(a_1), \quad N_{K''/K}(t) = (-1)^{sd} N_{K'/K}(a_s),
$$
$$
Q(X) = Pc_{K''/K}(t; X).
$$

另一方面，$[K'' : K] = [K'' : K'][K' : K] = sd$，所以$Q(X)$是次数$sd$的一元多项式。接下来是引理6。

让我们证明命题 8。由于环$B$很简单，所以它的中心$L$是域（VIII，p. 121，推论1）。由VIII、p. 259的定理 5，$A$中$B$的交换子$B'$是一个简单的环与中心$L$，我们有等式 $[A : K] = [B : K][B' : K]$。我们用$r$表示$B'$相对于$L$的减少的次数，$B$相对于$L$的减少$s$，以及$L$相对于$K$的减少次数表示为$d$。我们有

$$
[A : K] = n^2, \quad [B' : K] = r^2 d, \quad [B : K] = s^2 d,
$$

因此$n^2 = r^2 s^2 d^2$，即$n = rsd$。

令$b$为$B$的元素，并令$P(X)$为其在$L$代数$B$上的约化特征多项式；它是次数$s$的莫尼克。到引理 6，首一多项式 $Q = N_{L[X]/K[X]}(P)$ 是次数 $sd$ 的一阶。因此，首一多项式 $R = Q^r$ 是次数 $rsd = n$ 的单项式。再到引理 6，$R(X)$中$X^{n-1}$的系数等于$-r \operatorname{Tr}_{L/K}(\operatorname{Trd}_{B/L}(b))$，$R(X)$的常数项为$(N_{L/K}((-1)^s \operatorname{Nrd}_{B/L}(b)))^r = (-1)^n N_{L/K}(\operatorname{Nrd}_{B/L}(b))^r$。

从 $[A : K] = r^2 d[B : K]$ 开始，左侧 $B$ 模块 $A$ 不再包含秩 $r^2 d$（VIII、p. 124、命题 5）。因此我们有

$$
\operatorname{Pc}_{A/K}(b; X) = \operatorname{Pc}_{B/K}(b; X)^{dr^2}.
$$

由 III, §9, No. 4, p. 548 的推论，我们有

$$
\operatorname{Pc}_{B/K}(b; X) = N_{L[X]/K[X]}(\operatorname{Pc}_{B/L}(b; X)),
$$

由于 P(X) 是 $b$ 在 L-代数 B 上的约简特征多项式，我们有

(62) 电脑$_{B/L}(b; X) = P(X)^s$。

最后，通过R(X)的公式(60)—(62)和定义，我们有

(63) 电脑$_{A/K}(b; X) = N_{L[X]/K[X]}(P(X))^{dr^2s}= Q(X)^{dr^2s}= R(X)^{rsd}= R(X)^n$，

所以 R(X) 是 $b$ 在 K-代数 A 上的约化特征多项式。

我们已经证明了公式(56)。 公式 (57) 和 (58) 紧随公式 (56) 和引理 6，因为 Pcrd$_{A/K}(b; X)$ 中$X^{n-1}$ 的系数等于 $-$ Trd$_{A/K}(b)$ 并且常数项为 $(-1)^n$ Nrd$_{A/K}(b)$。

### 6. 约化范数和行列式

在这个小节中，D是有限次数的域除以中心K。我们用$D^*_{ab}$表示乘法群$D^*$与其派生（或换位子）群和$\pi$的商典范同态从$D^*$到$D^*_{ab}$。 映射Nrd$_{D/K}$诱导群同态从$D^*$到$K^*$； 核同态包含导出群 $D^*$ 因为 K 是可交换的。因而，从$D^*_{ab}$到$K^*$存在唯一同态Nrd，使得对于每个$x\in D^*$，Nrd$_{D/K}(x) =$Nrd$\circ \pi (x)$。

#### 命题 9 {#alg-viii-s17-prop-9 .statement tag=00L2}

令V为域D上的有限维右向量空间。令E为代数End$_D(V)$在域K上；它是中心简单且有限次数。对于 E 的每个可逆元 $u$，我们有

(64) Nrd$_{E/K}(u) =$ Nrd(det $u$)

（cf.VIII、p. 452、命题 2 表示$u$的行列式$u$的定义）。

我们用 $n$ 表示 D 上的 V 的维数，并使用 D 上的 V 的基表示矩阵代数 $\mathbf{M}_n(D)$ 和认同 E。 乘法群 GL$_n(D)$ 代数 E 由对角线矩阵和矩阵 $B_{ij}(\lambda )$ 生成（II, §10, No. 13，p. 362，推论 1）。因而，从下面两个具体情况可以得出命题 9。

A) 假设 $u$ 是对角矩阵 diag($a_1, . . . , a_n$)。对于每个$1\leqslant i\leqslant n$，令$L_i$为D包含$a_i$的极大交换子域；令 L 为对角线矩阵 diag($t_1, . . . , t_n$) 的 E 由……组成的子代数，$t_i\in L_i$ 为 $1\leqslant i\leqslant n$。令 $d$ 为 D 对 K 的约化次数。对于 $1\leqslant i\leqslant n$，我们有 $[L_i: K] =d$（VIII，p. 265，推论 2）。 K-代数 L 与 $L_1\times  \cdots  \times L_n$ 同构的，因此半单等于次数 $nd$；现在，我们有$[E : K] =n^2[D : K] =n^2d^2= [L : K]^2$。由此可见，L是E的最大交换律半单子代数（VIII，p. 262，命题3）。到 VIII、p. 346 的命题 7 时，我们有 Nrd$_{E/K}(u) = N_{L/K}(u)$。因而，通过III, §9, No. 3、p. 544的公式(18)，我们有

Nrd$_{E/K}(u) =\prod_{i=1}^nN_{L_i/K}(a_i) =\prod_{i=1}^n$ Nrd$_{D/K}(a_i)$

= Nrd$_{D/K}(a_1\cdots a_n) =$ Nrd($\pi (a_1\cdots a_n)$)。

此外，我们通过 VIII、p. 453 的命题 3 来确定$u=\pi (a_1\cdots a_n)$，在这种情况下给出公式 (64)。

B) 假设$u$等于$B_{ij}(\lambda )$，其中$\lambda$是D的元素，$i, j$是$[1, n]$区间内的不同整数。用 $d$ 表示 D 在 K 上的约化次数，并用 M 向量空间在 K 上通过从 D 到 K 的标量限制从 V 推导出来。那么 M 是一个简单的 E 模，我们有

(65) 电脑$_{M/K}(u; X) =$ 电脑$_{E/K}(u; X)^d$

由公式 (26) 共 VIII、p. 341。另外，M在K上是维数$nd^2$向量空间，$u-1_M$是M的幂零自同态；因此我们有

（66）PC$_{M/K}(u; X) = (X-1)^{nd^2}$。

通过比较公式 (65) 和 (66)，我们得到

（67）Pcrd$_{E/K}(u; X) = (X-1)^{nd}$

特别是 Nrd$_{E/K}(u) = 1$。我们还有VIII、p. 453中的命题 3 $u= 1$；因此，公式 (64) 在这种情况下成立。

#### 注 {#alg-viii-s17-n6-rem-1 .statement tag=00L3}

如果 E 的元素 $u$ 不可逆，我们有 Nrd$_{E/K}(u) = 0$（VIII、p. 340、命题 3）。

### 习题{#alg-viii-s17-exercises}

参见[习题为 § 17](exercises/s17/)。
