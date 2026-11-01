---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 8
section_title: Fourier transform
lang: zh
source: lie-vii-ix
book_pages: 359-369, 417-418
pdf_pages: 0366-0376, 0424-0425
extraction: native
subsections:
    - "no": 1
      title: FOURIER TRANSFORMS OF INTEGRABLE FUNCTIONS
      page: 360
      pdf_page: 367
    - "no": 2
      title: FOURIER TRANSFORMS OF INFINITELY-DIFFERENTIABLE FUNCTIONS
      page: 362
      pdf_page: 369
    - "no": 3
      title: FOURIER TRANSFORMS OF CENTRAL FUNCTIONS
      page: 366
      pdf_page: 373
    - "no": 4
      title: CENTRAL FUNCTIONS ON G AND FUNCTIONS ON T
      page: 368
      pdf_page: 375
statements: 9
exercises: 6
content_sha256: 7fd1acb4e65fa3356902610b13a26c74268fd9a92df1458993d67e3e0af2a998
translated_from: content/en/lie/IX/08_s8_fourier_transform.md
translation_method: google
source_content_sha256: 6e2618147afc628c71099020ffa7e02b28b7fa041ad48e0d3fc7f7f992c4cf3b
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 43a095631d30c68681c242233e10ba04864f8e17e81d986b3d15e24ef2675203
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 8。 傅里叶变换

我们保留记号和前一段的约定。

位置$^5$证明。前述，仅针对分裂的半单李代数进行了说明，

在分裂约化李代数的情况下，没有变换时有效。

### 1.傅里叶变换 / 可积函数

在这个数中，我们回顾了一些定义以及谱理论$^6$的结果。

用G的不可约表示类$\widehat{G}$集合表示（在有限维复数向量空间上）。对于所有$u\in \widehat{G}$，用$u$和$d(u)$的$Eu$空间表示其维数。在$u$下$E_u$不变量上存在分离正厄米特形式，且任意两个这样的形式成比例。用$A^*$（或$\|A\|_{\infty}$）表示End（E$_u$）的元素 A相对于这些形式之一的伴随（或范数）；对于所有$g\in G$，我们有$u(g)^*=u(g)^{-1}=u(g^{-1})$和$\|u(g)\|_{\infty}= 1$；对于所有$x\in \mathfrak{g}$，我们有$u(x)^*=-u(x) =u(-x)$。

给出 End(E$_u$) 希尔伯特空间结构，其中标量乘积为

$\langle A|B\rangle =d(u)\mathrm{Tr}(A^*B) =d(u)\mathrm{Tr}(BA^*)$, (1)

并把

$\|A\|_2=\langle A|A\rangle^{1/2}= (d(u)\mathrm{Tr}(A^*A))^{1/2}$。 (2)

我们有

$$
\surd\overline{d(u)}\|A\|_{\infty}\leq  \|A\|_2\leq d(u)\|A\|_{\infty} \tag{3}
$$

所以

$$
|\langle A|B\rangle | \leq d(u)^2\|A\|_{\infty}\|B\|_{\infty} \tag{4}
$$

对于所有 $g\in G$，我们有 $\|u(g)\|_2=d(u)$。

用$F( \widehat{G})$代数$\prod_{u\in\widehat{G}}$End(E$_u$)表示。用$L^2( \widehat{G})$表示希尔伯特空间End(E$_u$)的希尔伯特和；这是 $A= (A_u)\in F( \widehat{G})$ 的空间，使得 $\sum_u\|A_u\|^2_2<\infty$，标量为乘积

$\langle A|B\rangle =\sum_{u\in\widehat{G}}\langle A_u|B_u\rangle =\sum_{u\in\widehat{G}}d(u$)Tr(A$^*_uB_u$)。 (5)

将$L^2( \widehat{G})$上的希尔伯特范数也表示为$\| \|_2$，因此$\|A\|^2_2=\sum_{u\in\widehat{G}}\|A_u\|^2_2$代表$A\in L^2( \widehat{G})$。

如果 $f$ 是 G 上的可积复形函数，则

$u(f) =\int_Gf(g)u(g)dg\in$结束(E$_u$) (6)

对于所有$u\in \widehat{G}$。我们有$\|u(f)\|_{\infty}\leq \int_G|f(g)|dg=\|f\|_1$。 $f$的傅立叶协变换，用$\mathscr{F}(f)$表示，是$(u(f))_{u\in\widehat{G}}\in F( \widehat{G})$族。如果$f\in L^2( \widehat{G})$，

$^6$ 请参阅注 $^1$、§7、p. 66。

$$
\|f\|^2_2=\sum_{u\in\widehat{G}}\langle u(f)|u(f)\rangle =\|\overline{\mathscr{F}}(f)\|^2_2
$$

因此 $\overline{\mathscr{F}}$ 诱导是从希尔伯特空间 $L^2(G)$ 到其他字中的希尔伯特空间 $L^2( \widehat{G}):$ 的等距线性映射，对于 $f$ 和 $f'$ $L^2$(G)，我们有

$\int_G\overline{f(g)}f'(g)dg=\langle \overline{\mathscr{F}}(f)|\overline{\mathscr{F}}(f')\rangle =\sum_{u\in\widehat{G}}d(u$)Tr($u(f)^*u(f')$)。 (7)

对于$L^1$(G)中的$f$和$f'$，$f$和$f'$的卷积乘积$f*f'$定义为

$$
(f*f')(h) =\int_Gf(hg^{-1})f'(g)dg=\int_Gf(g)f'(g^{-1}h)dg
$$

（积分对于几乎所有 $h\in G$ 都有意义）。

我们有 $f*f'\in L^1(G)$，并且对于所有$u\in \widehat{G},u(f*f') =u(f)u(f')$，所以

$$
\overline{\mathscr{F}}(f*f') =\overline{\mathscr{F}}(f).\overline{\mathscr{F}}(f') \tag{8}
$$

相反，令$A = (A_u)_{u\in\widehat{G}}$为$F( \widehat{G})$的元素；对于所有 $u\in \widehat{G}$，令 $\mathscr{F}_uA$ 为 G 上的（解析）函数，定义为

$(\mathscr{F}_uA)(g) =\langle u(g)|A_u\rangle =d(u$)Tr(A$_uu(g)^{-1}$)。 (9)

如果$A\in L^2( \widehat{G})$，则家庭$(\mathscr{F}_uA)_{u\in\widehat{G}}$可在$L^2(G)$中求和； A 的傅里叶变换，记为$\mathscr{F}$(A)，是该族的和。 映射$\mathscr{F}$和$\mathscr{F}$是希尔伯特空间$L^2(G)$和$L^2( \widehat{G})$之间的逆同构。

其他字：

#### 命题 1 {#lie-ix-s8-prop-1 .statement tag=01GZ}

G 上的每个平方可积复形函数$f$在$(f_u)_{u\in\widehat{G}}$族的希尔伯特空间$L^2(G)$中都是和，其中，对于所有$h\in G$和所有$u\in \widehat{G}$，

$$
f_u(h) =\langle u(h)|u(f)\rangle
$$

$=d(u)\int_Gf(g$）Tr（$u(gh^{-1})$）$dg=d(u)\int_Gf(gh$）Tr（$u(g)$）$dg$。 (10)

对于所有$u\in \widehat{G}$选择，$E_u$的正交基$Bu$，并在该基中用$u(g)$的$(u_{ij}(g))$矩阵表示。命题 1 还意味着函数 $\surd\overline{d(u)}u_{ij}$ 的族，对于 $\widehat{G}$ 中的 $u$ 和 $B_u$ 中的 $i, j$，是空间 $L^2(G)$ 的正交基。

如果$f$在G上是可积函数，使得族$(f_u)$一致可求，则该族的和是连续的函数，其中重合几乎处处有$f$；在其他字中，如果我们假设在加法中$f$是连续的，那么对于所有$h\in G$，$f(h) =\sum_{u\in\widehat{G}}d(u)\int_Gf(gh$)Tr($u(g)$)$dg$。 (11)

相反地，让 $A\in F( \widehat{G})$；如果族 $(\mathscr{F}_uA)_{u\in\widehat{G}}$ 一致可求，则函数

$g \rightarrow \sum_{u\in\widehat{G}}(\mathscr{F}_uA)(g) =\sum_{u\in\widehat{G}}d(u$)Tr(A$_uu(g)^{-1}$)

是 G 上的连续函数，其傅立叶协变换为 A。

设$f$为G上的可积函数，并设$s\in G$。在$\gamma (s)f=\varepsilon_s*f,\delta (s)f=f*\varepsilon_{s^{-1}}$定义的G上用$\gamma (s)f$和$\delta (s)f$函数表示，即

$(\gamma (s)f)(g) =f(s^{-1}g),(\delta (s)f)(g) =f(gs)$ 为 $g\in G$，

（第III, §3, no. 4章和集成，第VII, §1, no. 1章）。我们有

$$
u(\gamma (s)f) =\int_Gf(s^{-1}g)u(g)dg=\int_Gf(g)u(sg)dg
$$

所以

$$
u(\gamma (s)f) =u(s)u(f) \tag{12}
$$

和类似地

$$
u(\delta (s^{-1})f) =u(f)u(s) \tag{13}
$$

当 G 是可交换的时，对于所有 $u\in \widehat{G}$，$\widehat{G}$ 是 G 的对偶群的基础集合（谱理论，第 II, §1，第 $1$）$,d(u) = 1$，并且我们恢复谱理论中给出的傅里叶变换的定义，第一章II。

### 2. 无穷微函数的傅里叶变换

回想一下（第 III, §3, no. 1 章，定义 2），U(G) 表示 G 上的分布的代数，其支持包含在 $\{e\}$ 中。 典范嵌入的 $\mathfrak{g}$ 到 U(G) 扩展到同构，从李代数 $\mathfrak{g}$ 的包络线代数到 U(G)（前述，no. 7，第 25 条）；从现在开始我们通过这个同构认同这两个代数。如果 $f$ 是 G 上的无限可微复数函数，并且如果 $t\in U(G)$，我们用 $L_tf$ 表示，G 上的 $R_tf$ 函数定义为

$$
L_tf(g) =\langle \varepsilon_g*t, f\rangle ,R_tf(g) =\langle t*\varepsilon_g, f\rangle
$$

（cf. 前述，no. 6）。对于所有$g\in G$，

$$
L_t\circ \gamma (g) =\gamma (g)\circ L_t,R_t\circ \delta (g) =\delta (g)\circ R_t
$$

设 $u\in \widehat{G}$；用 $u$ 的 $Eu$ 空间表示。 李群 $u: G\rightarrow \mathbf{G}\mathbf{L}(E_u)$ 的态射通过（实）李代数 $\mathfrak{g}\rightarrow$ End(E$_u$) 的微分得到同态，因此代数的同态，也用$u$ 表示，从 U(G) 到结束（E$_u$）。如果 $t\in U(G)$ 且 $f$ 是 G 上的无限可微函数，则

$$
u(L_tf) =u(f)u(t^{\vee}), u(R_tf) =u(t^{\vee})u(f) \tag{14}
$$

其中$t^{\vee}$表示U(G)主反自同构下$t$的像（第I, §2, no. 4章）；事实上，对于 $t\in \mathfrak{g}$ 验证这一点就足够了，在这种情况下，它可以与公式 (12) 和 (13) 区分开（cf. 第 III, §3, no. 7 章，第 27 条命题）。

对于所有$u\in \widehat{G}$，用$u($§7, no. 2、Th 的$\lambda (u)$ 最高权表示。 1)，所以$u \rightarrow \lambda (u)$是X(T)的主元素从$\widehat{G}$到集合$X_{++}$的双射映射。

令 $\Gamma \in U(G)$ 为 G (§7, no. 6) 的卡西米尔元素；对于所有$u\in \widehat{G}$，$E_u$的自同态$u(\Gamma )$是位似，其比率我们用$\widetilde{\Gamma}(u)$表示，所以我们有从$\widehat{G}$到$\mathbf{C}$的映射$u \rightarrow \widetilde{\Gamma}(u)$。

如果$\varphi$和$\psi$是$\widehat{G}$上的两个函数，且值为正实数，则用“$\varphi \preccurlyeq \psi$”或“$\varphi (u)\preccurlyeq \psi (u$）”表示关系“存在$M>0$使得$\varphi (u)\leq M\psi (u)$对于所有$u\in \widehat{G}$”；这是$\widehat{G}$上函数与正实数值的集合的先序关系。

#### 命题 2 {#lie-ix-s8-prop-2 .statement tag=01H0}

令 $m \rightarrow  \|m\|$ 为 $\mathbf{R}$ 向量空间 $\mathbf{R}\otimes X(T)$ 上的范数，且 $\Gamma$ G 的卡西米尔元素。令 $\varphi$ 为 $\widehat{G}$ 上的函数，且为正实数值。

a) 以下条件是等价的：

(i) 存在整数$n >0$使得$\varphi (u)\preccurlyeq (\|\lambda (u)\|+ 1)^n$（分别对于每个整数$n >0$，我们有$\varphi (u)\preccurlyeq (\|\lambda (u)\|+ 1)^{-n}$）。

(ii) 存在整数$n >0$使得$\varphi (u)\preccurlyeq ( \widetilde{\Gamma}(u) + 1)^n$（分别对于每个整数$n >0$，我们有$\varphi (u)\preccurlyeq ( \widetilde{\Gamma}(u) + 1)^{-n}$）。

b) 如果 G 为半单，条件 (i) 和 (ii) 也等价于：

(iii) 存在整数$n >0$使得$\varphi (u)\preccurlyeq d(u)^n$（分别对于每个整数$n >0$，我们有$\varphi (u)\preccurlyeq d(u)^{-n}$）。

注首先条件 (i) 显然独立于范数的选择。因此，我们可以使用由与$\Gamma ($§7, no. 6相关的二次形式$Q_{\Gamma}$定义的范数，命题4）。然后

$$
0\leq \widetilde{\Gamma}(u) =\|\lambda (u) +\rho \|^2- \|\rho \|^2
$$

所以 $\widetilde{\Gamma}(u) + 1\preccurlyeq (\|\lambda (u)\|+ 1)^2\preccurlyeq \widetilde{\Gamma}(u) + 1$，因此 a)。

进一步，如果G是半单，

$\|\lambda (u) +\rho \|\preccurlyeq d(u)\preccurlyeq \|\lambda (u) +\rho \|^N$，其中$N = 1/$2（暗淡$G-$暗淡T）

（§7, no. 5，Th.3 的 Cor.1），因此 $\|\lambda (u)\|+ 1\preccurlyeq d(u)\preccurlyeq (\|\lambda (u)\|+ 1)^N$，因此 b)。

根据命题 2，条件 (i) 独立于最大环面、腔室和范数的选择，并且条件 (ii) 独立于卡西米尔元素的选择。 函数 $\varphi$ 满足条件 (i) 和 (ii) 据说是中等递增（或快速递减）。 乘积两个适度递增函数适度递增；中等递增函数和快速递减函数的乘积是快速递减。如果 $\varphi$ 快速递减，则族 $(\varphi (u))_{u\in\widehat{G}}$ 是可求和的。

#### 例 {#lie-ix-s8-n2-exa-1 .statement tag=01H1}

函数 $u \rightarrow d(u)$ 中等递增（§7, no. 5，Th. 3 的 Cor. 1）；对于 $\mathbf{R}\otimes X(T)$ 上的任意范数 $\| \|$，函数 $u \rightarrow  \|\lambda (u)\|$ 是适度的递增。对于任何卡西米尔元素$\Gamma$，函数$u \rightarrow \widetilde{\Gamma}(u)$适度递增；更一般地说：

#### 命题 3 {#lie-ix-s8-prop-3 .statement tag=01H2}

对于所有 $t\in$ U(G)，函数 $u \rightarrow  \|u(t)\|_{\infty}$ 和 $u \rightarrow  \|u(t)\|_2$ 在 $\widehat{G}$ 上是中等的递增。

由于两个中等递增函数中的乘积是中等递增，因此当$t\in \mathfrak{g}:$在这种情况下断言从§7, no. 6和不等式中的注推出时，就足以证明这一点

$$
\|u(t)\|_2\leq d(u)\|u(t)\|_{\infty}
$$

#### 定理 1 {#lie-ix-s8-thm-1 .statement tag=01H3}

a) 令 $f$ 为 G 上的无限可微复形函数。则族 $(f_u)_{u\in\widehat{G}}$（其中 $f_u(g) =\langle u(g)|u(f)\rangle$）在 G 上一致可求，并且对于所有 $h\in G$，

$f(h) =\sum_{u\in\widehat{G}}\langle u(h)|u(f)\rangle =\sum_{u\in\widehat{G}}d(u)\int_Gf(g$）Tr（$u(gh^{-1})$）$dg$。

b) 令G上的$f$为可积函数；那么 $f$ 几乎处处都等于无限可微的函数当且仅当函数 $u \rightarrow  \|u(f)\|_{\infty}$ 在 $\widehat{G}$ 上快速递减。

令$f$为G上的无限可微函数，并令$\Gamma$为G的卡西米尔元素；通过公式 (14),

$$
\widetilde{\Gamma}(u)^nu(f) =u(f)u(\Gamma )^n=u((L_{\Gamma})^nf)
$$

对于所有$n\geq 0$，因而

$\widetilde{\Gamma}(u)^n\|u(f)\|_{\infty}\leq  \|(L_{\Gamma})^nf\|_1\leq$支持$_{g\in G}|((L_{\Gamma})^nf)(g)|$； (15)

因而，函数$u \rightarrow  \|u(f)\|_{\infty}$确实很快递减。

相反，令$A = (A_u)_{u\in\widehat{G}}$为$F( \widehat{G})$的元素，使得函数$u \rightarrow  \|A_u\|_{\infty}$迅速变为递减。把$f_u(g) =\langle u(g)|A_u\rangle$； 函数 $g \rightarrow f_u(g)$ 是解析的，因此是无限可微的。由章。 III, §3, no. 7，提案 27，

$$
(L_xf_u)(g) =\langle u(g)u(x)|A_u\rangle
$$

对于所有$x\in \mathfrak{g}$。让$t\in U(G)$；由前面的公式，

$$
(L_tf_u)(g) =\langle u(g)u(t)|A_u\rangle
$$

因而

$$
|(L_tf_u)(g)|=|\langle u(g)u(t)|A_u\rangle  \leq d(u)^2\|u(t)\|_{\infty}\|u(g)\|_{\infty}\|A_u\|_{\infty}
$$

$$
=d(u)^2\|u(t)\|_{\infty}\|A_u\|_{\infty}
$$

由于 $d(u)$ 和 $\|u(t)\|_{\infty}$ 是适度的递增（命题 3），而 $\|A_u\|_{\infty}$ 是快速的递减，函数 $u \rightarrow$ $_g|(L_tf_u)(g)|$ 是快速的递减；因而，族$(L_tf_u)_{u\in\widehat{G}}$是一致可求的。由此可见，$^7$族$(f_u)$的和是G上的无限可微的函数，其傅里叶协变换为$(A_u)$，因此定理。

用$A = (A_u)_{u\in\widehat{G}}$家庭的$L^2( \widehat{G})$由……组成的$\mathscr{S}( \widehat{G})$向量子空间表示，使得函数$u \rightarrow  \|A_u\|_{\infty}$在$\widehat{G}$上快速递减。从定理可以得出复合体向量空间 $\mathscr{C}^{\infty}(G;\mathbf{C})$ 和 $\mathscr{S}( \widehat{G})$ 之间的映射 $\mathscr{F}:f \rightarrow (u(f))_{u\in\widehat{G}}$ 和 $\mathscr{F}: A \rightarrow \sum_{u\in\widehat{G}}\langle u(g)|A_u\rangle$ 诱导逆同构。给出均匀 $C^{\infty}$ 收敛性 (§6, no. 4) 的空间 $\mathscr{C}^{\infty}(G;\mathbf{C})$ 拓扑，可以由$t\in U(G)$的半范数族$f \rightarrow$sup$_{g\in G}|L_tf(g)|$和空间$\mathscr{S}( \widehat{G})$定义拓扑由半范数$p_n: A \rightarrow$sup$_{u\in\widehat{G}}( \widetilde{\Gamma}(u) + 1)^n\|A_u\|_{\infty}$的序列定义。前面的证明的公式(15)表明$\overline{\mathscr{F}}$是连续的。设$t\in U(G)$，并令$A = (A_u)_{u\in\widehat{G}}$为$\mathscr{S}( \widehat{G})$的元素；输入$f_n(g) =\langle u(g)|A_u\rangle$。令$p$为整数，使得$\sum_{u\in\widehat{G}}\widetilde{\Gamma}(u)^{-p}= M<\infty$。根据前面的证明，存在正整数$m$，使得对于所有$g\in G$，

$$
|(L_tf_u)(g)| \leq d(u)^2\|u(t)\|_{\infty}\|A_u\|_{\infty}\leq m.(1 + \widetilde{\Gamma}(u))^m\widetilde{\Gamma}(u)^{-p}\|A_u\|_{\infty}
$$

所以$|(L_t\mathscr{F}(A))(g)| \leq mMp_m(A)$；这证明$\mathscr{F}$是连续的。因而：

#### 推论 {#lie-ix-s8-n2-cor-1 .statement tag=01H4}

映射$\overline{\mathscr{F}}:f \rightarrow (u(f))_{u\in\widehat{G}}$和$\mathscr{F}: A \rightarrow \sum_{u\in\widehat{G}}\langle u(g)|A_u\rangle$诱导逆同构位于拓扑向量空间$\mathscr{C}^{\infty}(G;\mathbf{C})$和$\mathscr{S}( \widehat{G})$之间。

$^7$ 这是根据空间 $\mathscr{C}^{\infty}(G;\mathbf{C})$ 的事实得出的，其中拓扑是均匀的

$C^{\infty}$-收敛(§6, no. 4)，完备的。

### 3. 傅里叶变换中环函数

对于所有$u\in \widehat{G}$，用$u$的$\chi_u$特征标表示；因而，

$\chi_u(g) =$ Tr($u(g)$)$,(g\in G)$。 (16) 回顾谱理论公式

$$
\chi_u*\chi_v= 0(u, v\in \widehat{G}, u\not=v) \tag{17}
$$

$$
\chi_u*\chi_u=\frac{1}{d(u)}\chi_u(u\in \widehat{G}) \tag{18}
$$

对于所有$u\in \widehat{G}$，用$\varepsilon_u$表示$E_u$的恒等式映射。回想一下(§7, no. 4)，ZL$^2(G)$表示中心函数$f$类由……组成$L^2(G)$由……组成子空间，即对于所有$f\circ$Int$s=f$ $s\in G$，或者相当于所有$s\in G$的$\gamma (s)f=\delta (s^{-1})f$。

#### 命题 4 {#lie-ix-s8-prop-4 .statement tag=01H5}

让$f\in L^2(G)$。那么$f$是中心当且仅当对于所有$u\in \widehat{G}$来说$u(f)$是位似。在那种情况下

$$
u(f) =\frac{\varepsilon_u}{d(u)}\int_Gf(g)\chi_u(g)dg \tag{19}
$$

根据命题1（no. 1），说$f$是中心意味着$u(\gamma (s)f) =$$u(\delta (s^{-1})f)$对于所有$s\in G$和所有$u\in \widehat{G}$；但对于所有$s\in G$和所有$u\in \widehat{G}$（公式（12）和（13）），这也可以写成$u(s)u(f) =u(f)u(s)$，因此是第4条命题的第一个断言（Schur的引理）。如果 $u(f)$ 是位似，则 $u(f) =\lambda_u\varepsilon_u$ 与

$\lambda_u=\frac{1}{d(u)}$Tr($u(f)$)$=\frac{1}{d(u)}\int_Gf(g$)Tr($u(g)$)$dg=\frac{1}{d(u)}\int_Gf(g)\chi_u(g)dg$。

因而，对于 $f\in$ ZL$^2(G)$ 我们有

$$
u(f) =\langle \overline{\chi}_u|f\rangle \frac{\varepsilon_u}{d(u)}\rangle \tag{20}
$$

所以

$$
\overline{\mathscr{F}}(f) =(\langle \overline{\chi}_u|f\rangle \frac{\varepsilon_u}{d(u)})_{u\in\widehat{G}} \tag{21}
$$

和

$$
\|\overline{\mathscr{F}}(f)\|^2_2=\sum||||\langle \overline{\chi}_u|f\rangle \frac{\varepsilon_u}{d(u)}||||^{22}=\sum|\langle \overline{\chi}_u|f\rangle |^2
$$

$uu$

相反，如果$\varphi$是$\widehat{G}$、元素$(\frac{\varphi(u)}{d(u)}\varepsilon_u)_{u\in\widehat{G}}$（$F( \widehat{G})$属于到$L^2( \widehat{G})$）上的平方可积复形函数，并且我们有 (公式 (9)) $(\mathscr{F}_u(\frac{\varphi(u)}{d(u)}\varepsilon_u))(g) =d(u$)Tr $(\frac{\varphi(u)}{d(u)}\varepsilon_uu(g)^{-1})=\varphi (u)\overline{\chi}_u(g)$，

所以

$$
\mathscr{F}((\frac{\varphi(u)}{d(u)}\varepsilon_u))=\sum\varphi (u)\overline{\chi}_u \tag{22}
$$

$u\in \widehat{G}$

注，特别是，对于$\widehat{G},^8$中的$u, v$，公式 (20) 和 (21) 给出

$u(\overline{\chi}_v) = 0$ 如果 $u\not=v$, (23)

$u(\overline{\chi}_u) =\frac{\varepsilon_u}{d(u)}\in$结束(E$_u$), (24)

$\overline{\mathscr{F}}(\chi_u) =\frac{\varepsilon_u}{d(u)}\in$结束(E$_u$)$\subset F( \widehat{G})$。 (25)

#### 命题 5 {#lie-ix-s8-prop-5 .statement tag=01H6}

令$f$为G上的连续中心函数。则$f$是无限可微的当且仅当函数$u \rightarrow  |\langle \chi_u|f\rangle |$在$\widehat{G}$上快速递减；在这种情况下，

$$
f(g) =\sum_{u\in\widehat{G}}\langle \chi_u|f\rangle \chi_u(g)
$$

对于所有$g\in G$。

由 Th. $1b)$, 函数 $\overline{f}$ 是无限可微的当且仅当函数 $u \rightarrow  \|u(\overline{f})\|_{\infty}$ 快速递减；但是，通过 (20)，

$$
\|u(\overline{f})\|_{\infty}=\frac{1}{d(u)}|\langle \chi_u|f\rangle |
$$

因此第一个断言，因为函数$d(u)$和$\frac{1}{d(u)}$适度递增。

假设$f$是无限可微的；通过 Th。 $1a),f(g) =\sum_{u\in\widehat{G}}f_u(g)$ 对于所有 $g\in G$，所以

$f_u(g) =\langle u(g)|u(f)\rangle =d(u$)Tr($u(g)^{-1}.u(f)$)$=d(u$)Tr$(u(g)^{-1}\langle \overline{\chi}_u|f\rangle \frac{\varepsilon_u}{d(u)})$

$=\langle \overline{\chi}_u|f\rangle$Tr($u(g)^{-1}$)$=\langle \overline{\chi}_u|f\rangle \overline{\chi}_u(g)$。

因此，$f(g) =\sum_{u\in\widehat{G}}\langle \overline{\chi}_u|f\rangle \overline{\chi}_u(g)$；但是，对于所有$u\in \widehat{G}$，$u$的同积表示$u'$满足$\overline{\chi}_u=\chi_{u'}$和映射$u \rightarrow u'$是$\widehat{G}$的置换；所以我们还有$f(g) =\sum_{u\in\widehat{G}}\langle \chi_u|f\rangle \chi_u(g)$，因此命题。

$^8$ 我们将 End(E$_u$) 嵌入到乘积 $F( \widehat{G}) =\prod_{v\in\widehat{G}}$ End(E$_v$) 中，方法是关联到任意

$A\in$结束（E$_u$）族$(A_v)_{v\in\widehat{G}}$，使得$A_u= A$和$A_v= 0$为$v\not=u$。

#### 推论{#lie-ix-s8-n3-cor-1 .statement tag=01H7}

设$f$是G上的连续中心函数。则$f$是无限可微的当且仅当$f$的限制对T是无限可微的。

确实，通过 Cor. 4 个§7, no. 4，

$\langle \chi_u|f\rangle =\int_G\overline{\lambda(u)(t)}\varphi (t)dt$，其中$\varphi (t) =\prod_{\alpha >0}(1-\alpha (t)^{-1})f(t)$。

如果 $f|T$ 是无限可微的，$\varphi$ 也是无限可微的；根据第 5 条，应用于群 T，$\widehat{T} = X(T)$ 上的函数 $\mu \rightarrow \int_T\overline{\mu(t)}\varphi (t)dt$ 则迅速递减，函数 $u \rightarrow  \langle \chi_u|f\rangle$ 也如此；因此函数 $f$ 是无限可微的（命题 5）。 逆命题很清楚。

### 4. G 区中央函数和 T 区函数

用 G 上连续复值函数的 $\mathscr{C}(G)$ 空间和无限可微函数的 $\mathscr{C}^{\infty}(G)$ 子空间表示。那么我们就有序列的内含物

$$
\Theta (G)\subset \mathscr{C}^{\infty}(G)\subset \mathscr{C}(G)\subset L^2(G)
$$

分别用$Z\Theta (G),Z\mathscr{C}^{\infty}(G),Z\mathscr{C}(G)$、ZL$^2$(G)表示，这些各个空间中的中心函数的子空间由……组成。类似地介绍空间$\Theta (T),\mathscr{C}^{\infty}(T),\mathscr{C}(T),L^2(T)$；对于此列表中的任何空间 E，用不变量（或反不变量）的 $E^W$（或 $E^{-W}$）子空间由……组成表示，元素表示 Weyl 群 W 的运算。我们有一个交换律图表

$$
Z\mathscr{C}(G)\longrightarrow^{a_c}\mathscr{C}(T)^W
$$

$$
Z\mathscr{C}^{\infty}(G)\longrightarrow^{a_{\infty}}\mathscr{C}^{\infty}(T)^W
$$

$$
Z\Theta (G)\longrightarrow^{a_{\Theta}}\Theta (T)^W
$$

其中垂直箭头代表典范嵌入，映射$a_c, a_{\infty}, a_{\Theta}$由限制映射从$\mathscr{C}(G)$诱导到$\mathscr{C}(T)$。

映射 $a_c, a_{\infty}, a_{\Theta}$ 是双射（§2, no. 5，第 5 号提案的 Cor.1，§8, no. 3，第 5 号提案的 Cor.，以及 §7, no. 3，第 2 号提案的 Cor.）。

现在假设正根属于与X(T)的半和$\rho$，并考虑映射$b$，它与T上的每个连续函数$\varphi$关联$\varphi .J(\rho )$。我们有一个可交换的图表

ZL$^2(G)--------------------\longrightarrow^uL^2(T)^{-W}$

$$
Z\mathscr{C}(G)\longrightarrow^{a_c}\mathscr{C}(T)^W\longrightarrow^{b_c}\mathscr{C}(T)^{-W}
$$

$$
Z\mathscr{C}^{\infty}(G)\longrightarrow^{a_{\infty}}\mathscr{C}^{\infty}(T)^W\longrightarrow^{b_{\infty}}\mathscr{C}^{\infty}(T)^{-W}
$$

$$
Z\Theta (G)\longrightarrow^{a_{\Theta}}\Theta (T)^W\longrightarrow^{b_{\Theta}}\Theta (T)^{-W}
$$

其中垂直箭头是规范包含物，映射 $b_c, b_{\infty}, b_{\Theta}$ 由 $b$ 引发，$u$ 扩展 $b_c\circ a_c$ 由连续性引发（§7, no. 4，Th. 2 的 Cor. 3）。 映射 $u$ 和 $b_{\Theta}$ 是双射（loc. cit.）； $b_{\infty}$ 也是如此（练习 5）；另一方面，$b_c$ 一般而言不是满射的（Exerc. 6）。

### 习题{#lie-ix-s8-exercises}

§ 8](exercises/s8/)参见[习题。
