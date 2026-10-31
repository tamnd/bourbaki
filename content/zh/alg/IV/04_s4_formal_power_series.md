---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 4
section_title: Formal power series
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.24-A IV.41, A IV.90-A IV.91
pdf_pages: 0033-0050, 0099-0100
extraction: ocr
subsections:
    - "no": 1
      title: Definition of formal power series. Order
      page: 24
      pdf_page: 33
    - "no": 2
      title: Topology on the set of formal power series. Summable families
      page: 25
      pdf_page: 34
    - "no": 3
      title: Substitutions
      page: 28
      pdf_page: 37
    - "no": 4
      title: Invertible formal power series
      page: 30
      pdf_page: 39
    - "no": 5
      title: Taylor's formula for formal power series
      page: 31
      pdf_page: 40
    - "no": 6
      title: Derivations in the algebra of formal power series
      page: 32
      pdf_page: 41
    - "no": 7
      title: The solution of equations in a formal power series ring
      page: 35
      pdf_page: 44
    - "no": 8
      title: Formal power series over an integral domain
      page: 38
      pdf_page: 47
    - "no": 9
      title: The field of fractions of the ring of formal power series in one indeterminate over a field
      page: 38
      pdf_page: 47
    - "no": 10
      title: Exponential and logarithm
      page: 39
      pdf_page: 48
statements: 23
exercises: 8
errata:
    - says: imply $w(v_\nu) \geq |\nu| + 1$
      read: imply $\omega(v_\nu) \geq |\nu| + 1$
      why: The order function of a formal power series is omega throughout this no., and the same sentence sets it round once and roman once — "the relations omega(g_i) >= 2 imply w(v_nu) >= |nu| + 1" on page 44. The French of 2007 (A IV.30) sets omega in both places. The reading is faithful to the page; it is the page that changes letter in the middle of a line.
    - says: we have $w(u) \geq w(u) + 1$, which is impossible if $u \neq 0$ because $w(u)$ would then be a positive integer
      read: we have $\omega(u) \geq \omega(u) + 1$, which is impossible if $u \neq 0$ because $\omega(u)$ would then be a positive integer
      why: Same object, same page, three more times in roman. The argument is about the order of u, which the no. defines as omega and which formula (23) is stated with.
    - says: We thus have $w(v - T(u)) \geq n + 1$
      read: We thus have $\omega(v - T(u)) \geq n + 1$
      why: Page 45 sets "We thus have w(v - T(u)) >= n + 1" on one line and "we thus have omega(v - T(u)) >= n" on the next, of the same quantity in the same induction. One of the two is a slip and it is the roman one, because the definition and the French both read omega.
    - says: then $w(u^{-1}) = -w(u)$. \* In other words (Comm. Alg., VI, § 3, No. 6, p. 392, Def. 3), w is a normalized discrete valuation
      read: then $\omega(u^{-1}) = -\omega(u)$. \* In other words (Comm. Alg., VI, § 3, No. 6, p. 392, Def. 3), $\omega$ is a normalized discrete valuation
      why: Page 48 runs the roman w twice in the displayed relation and once in the sentence naming the valuation, then sets "omega(u) >= n" round two lines below for the same function. The valuation of K((X)) is omega, as the French of 2007 (A IV.36) has it.
content_sha256: 8eec39e85b4d661461ed7763b99eb4281f618938b8d8cceda0bb99ecf40f17c2
translated_from: content/en/alg/IV/04_s4_formal_power_series.md
translation_method: google
source_content_sha256: ecc1c2d36748dfed392a2d0bff5cf730d1aaf97675f112d959e7b8c05ce7ab7f
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 4b4385afc018bc4f44354a6c39f1b0411789045b274f5440bdefe60e163a14e2
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。正式幂级数

### 1. 正式幂级数的定义。 阶

设I为集合。我们回想一下（III、p. 454 和 456），A 上幺半群 $N^{(I)}$ 的总代数被称为形式幂级数的 *代数相对于不定数* $X_i \ (i \in I)$（或在不定数 $X_i$） *系数在* A中。用$A[[X_i]]_{i \in I}$或$A[[((X_i)_{i \in I}]]$或$A[[X]]$表示，其中用X家族$(X_i)_{i \in I}$表示：在本段中我们将主要使用记号$A[[I]]$。 有时在I的元素i的$A[[I]]$中用$X_i$以外的符号来指定典范像比较方便，对于例$Y_i, Z_i, T_i, \ldots$；本例中使用的约定类似于多项式的约定 (IV, p. 1)。 代数$A[[I]]$则由$A[[Y_i]]_{i \in I}$或$A[[Y]]$等指定。

当I是p 元素的有限集合时，我们也说$A[[I]]$是p不定式中形式幂级数的代数。对于固定 p，这些代数都是同构的。 1, 2, ... 不确定中的正式幂级数的代数也将由未指定的指标的 $A[[X]]$, $A[[U, V]]$, ..., 集合 I 表示。

正式的幂级数 u 通常写作 $u = \sum_{\nu \in N^{(I)}} a_\nu X^\nu$ (cf. IV, p. 1)。

$\alpha_\nu$是$u$的*系数*；它们可能有无限多个$\neq 0$。 $a_\nu X^\nu$称为$u$的*项*；要使 u 成为多项式，$u$ 应仅具有项 $\neq 0$ 的有限数是必要且充分的。 项 $a_\nu X^\nu$ 使得 |ν| = p 称为总计次数 p 中的项。形式上的幂级数$u_p = \sum_{|\nu|=p} \alpha_\nu X^\nu$称为u的次数*p的*齐次分量（当I有限时它是一个多项式）； $u_0$ 与 A 的元素相同，也称为 u 的*常数项*。如果 $u = u_p$，我们说 u 是次数 p 的齐次。如果$u, v \in \mathbf{A}[[\mathrm{I}]]$和$w = uv$，我们有

(1)
$$
w_p = \sum_{q+r=p} u_q v_r
$$
对于每个整数 $p \geq 0$。

我们记得（III，p. 456），正式的幂级数$u \neq 0$的*阶*$\omega(u)$是使得$u_p \neq 0$最小的整数p。 We shall agree to adjoin to Z an element written $\infty$ and extend the order relation and addition from Z to $Z \cup \{\infty\}$ by the conventions
$$
n < \infty,\quad \infty + \infty = \infty,\quad \infty + n = n + \infty = \infty
$$
for every $n \in Z$; we also put $\omega(0) = \infty$. 根据这些约定，我们有关系
$$
\begin{align*}
\omega(u+v) &\geq \inf(\omega(u), \omega(v)), \\
\omega(u+v) &= \inf(\omega(u), \omega(v)) \text{ if } \omega(u) \neq \omega(v), \\
\omega(uv) &\geq \omega(u) + \omega(v),
\end{align*}
$$
对于 $\mathbf{A}[[\mathrm{I}]]$ 中的任何正式幂级数 $u$ 和 $v$。

我们记得（III，p. 457），对于I的任何子集J，我们将认同$\mathbf{A}[[\mathrm{I}]]$与$\mathbf{A}[[\mathrm{I}-J]] [[\mathrm{J}]]$，这允许我们对正式的幂进行定义阶$\omega_J(u)$ 级数相对于$X_j$（$j \in J$），$u$相对于$X_j$（$j \in J$）的齐次分量等。

设$\varphi$为A的同态到环B。我们通过让每个正式的幂级数$u = \sum \alpha_\nu X^\nu$将$\mathbf{A}[[\mathrm{I}]]$的扩展$\varphi$到同态$\overline{\varphi}$到$B[[\mathrm{I}]]$ 对应到正式幂级数 $\sum \varphi(\alpha_\nu) X^\nu$；我们说后者是通过 *应用* $\varphi$ *到形式幂级数* u 的系数获得的。我们将有时写为$^\varphi u$代表$\overline{\varphi}(u)$。

特别是，如果 A 是 B 的子环且 A 的 $\varphi$ 典范嵌入进入 B，则 $\mathbf{A}[[\mathrm{I}]]$ 的同态 $\overline{\varphi}$ 进入 $B[[\mathrm{I}]]$ 是单射的；我们通常将认同$\mathbf{A}[[\mathrm{I}]]$与子环或$B[[\mathrm{I}]]$乘以$\overline{\varphi}$。

### 2. 正式幂级数的集合上的拓扑。可求和族

定义$\mathbf{A}[[\mathrm{I}]]$无非是乘积集合$\mathbf{A}^{N^{(I)}}$。除非明确指出相反，我们将为 A 配备离散的拓扑和 $\mathbf{A}[[\mathrm{I}]]$ 配备乘积拓扑（Gen. Top. I，p. 31 f.），我们将其称为规范的拓扑。配备加法和离散的拓扑，$A$是一个分离且完整的拓扑群；因此加法$A[[I]]$是一个分离且完整的拓扑群（Gen.Top.，III，p. 238和242以及Gen.Top.，II，p. 187）。此外，多项式的代数$A[(X_i)_{i \in I}]$在$A[[I]]$（Gen.Top.，III p. 238，Prop，25）中是稠密的，因此我们可以将$A[[I]]$视为$A[(X_i)_{i \in I}]$的完成。

对于每个$\beta \in \mathbf{N}^{(I)}$，令$S_\beta$为多索引$\nu$的集合，使得$\nu \leq \beta$，并令$a_\beta$为正式幂级数$u = \sum \alpha_\nu X^\nu$的集合，使得$a_\nu = 0$ 换$\nu \in S_\beta$。显然，$S_\beta$是$\mathbf{N}^{(I)}$的有限子集，$\mathbf{N}^{(I)}$的每个有限子集都包含在形式$S_\beta$的集合中。由此可见，族$(a_\beta)_{\beta \in \mathbf{N}^{(I)}}$是$A[[I]]$中0的邻域的基本系统。 集合 $a_\beta$ 是 $A[[I]]$ 中的理想，因此 (Gen. Top., III, p. 275) $A[[I]]$ 是拓扑环。

#### 引理 1 {#alg-iv-s4-lem-1 .statement tag=06BY}

令$L$为无限集合，$(u_\lambda)_{\lambda \in L}$为$A[[I]]$的元素的族，并将$u_\lambda = \sum \alpha_{\lambda,\nu} X^\nu$代为$\lambda \in L$。那么下面的条件是等价的：
(i) 族 $(u_\lambda)_{\lambda \in L}$ 可在 $A[[I]]$ 中求和（Gen. Top., III, p. 262）。
(ii) 我们有$\lim u_\lambda = 0$，通过有限子集的补集*过滤*$L$。
(iii) 对于每个$\nu \in \mathbf{N}^{(I)}$，我们都有$\alpha_{\lambda,\nu} = 0$，除了指标$\lambda \in L$的*有限*数。

当这些条件成立时，级数$u = \sum_{\lambda \in L} u_\lambda$等于$\sum \alpha_\nu X^\nu$，每个$\nu \in \mathbf{N}^{(I)}$都有$a_\nu = \sum_{\lambda \in L} \alpha_{\lambda,\nu}$。

(i) 和 (ii) 的等价由 Cor 得出。 Gen. Top. 2，III，p. 263。
(ii) 和 (iii) 的等价由乘积空间中极限的性质得出（Gen. Top., I, p. 55, Cor. 1）。
最后一个断言源自 Gen. Top. 的第 4 条命题，III，p. 266。

让我们给出一些例个可求和族。
a) 令$u \in A[[I]]$和$a_\nu$为$X^\nu$在$u$中的系数。然后，族 $(\alpha_\nu X^\nu)_{\nu \in \mathbf{N}^{(I)}}$ 可以与和 $u$ 相加（这证明了写作 $u = \sum \alpha_\nu X^\nu$ 的合理性）。

b) 设 $u \in A[[I]]$；对于每个整数$p \geq 0$，令$u_p$为$u$的次数$p$的齐次分量。那么家庭$(u_p)_{p \geq 0}$是可求和的，我们有$u = \sum_{p \geq 0} u_p$。

c) 令$(u_\lambda)_{\lambda \in L}$为$A[[I]]$的元素族，并假设对于$\lambda \in L$的每个整数$n \geq 0$集合，使得$\omega(u_\lambda) < n$是有限的。那么家庭$(u_\lambda)_{\lambda \in L}$是可求和的。

#### 注 {#alg-iv-s4-n2-rem-1 .statement tag=06BZ}

— 假设 $I$ 是*有限*。对于每个整数$n \geq 0$，令$b_n$为正式幂级数$u \in A[[I]]$的集合，使得$\omega(u) \geq n$。 序列$(b_n)_{n \geq 0}$是$\mathbf{A}[[\mathbf{I}]]$中0的邻域的基本系统。因此，当且仅当对于$\mathbf{A} \in L$的每个$n \in \mathbf{N}$集合使得$\omega(u_\lambda) < n$是有限的时，$\mathbf{A}[[\mathbf{I}]]$（$\lambda \in L$）的元素$u_\lambda$族是可求和的。

#### 命题 1 {#alg-iv-s4-prop-1 .statement tag=06C0}

*设*$(u_\lambda)_{\lambda \in L}$*和*$(v_\mu)_{\mu \in M}$*是*$\mathbf{A}[[\mathbf{I}]]$的元素的两个可求和族。 *然后家庭* $(u_\lambda v_\mu)_{(\lambda, \mu) \in L \times M}$ *是可求和的，我们有*

$$
\sum_{(\lambda, \mu) \in L \times M} u_\lambda v_\mu = \left( \sum_{\lambda \in L} u_\lambda \right) \left( \sum_{\mu \in M} v_\mu \right)
$$

令$(\alpha_{\lambda, \nu})_{\nu \in \mathbf{N}^{(I)}}$（或$(\beta_{\mu, \nu})_{\nu \in \mathbf{N}^{(I)}}$）为$u_\lambda$（或$v_\nu$）的系数族。对于每个$\nu \in \mathbf{N}^{(I)}$，仅存在对$(\nu_1, \nu_2) \in \mathbf{N}^{(I)} \times \mathbf{N}^{(I)}$的有限数，使得$\nu_1 + \nu_2 = \nu$，因此仅存在对$(\lambda, \mu) \in L \times M$的有限数，使得$u_\lambda v_\mu$中的$X^\nu$的系数为$\neq 0$。因此家庭$(u_\lambda v_\mu)_{(\lambda, \mu) \in L \times \mathscr{J}}$是可求和的。现在公式 (2) 是从和的结合性衍生出来的（Gen. Top.、III、p. 265、公式 (2)）。

在 $\mathbf{A}[[\mathbf{I}]]$ 乘积中是结合律和交换律合成律。因此，我们可以谈论$\mathbf{A}[[\mathbf{I}]]$的元素的*可乘族*和可乘族的*乘积*（Gen.Top.，III，p. 262，注3）。

#### 命题 2 {#alg-iv-s4-prop-2 .statement tag=06C1}

*设*$(u_\lambda)_\lambda$*是*$\mathbf{A}[[\mathbf{I}]]$的元素的可和族。
(i) *家庭* $(1 + u_\lambda)_\lambda$ *可乘*。
(ii) *设*$\mathfrak{T}$*为*$L$的所有有限子集中的集合。 *对于任何* $M \in \mathscr{S}$ *放置* $u_M = \prod_{\lambda \in M} u_\lambda$。 *然后家庭* $(u_M)_{M \in \mathfrak{T}}$ *可求和，我们有*

$$
\sum_{M \in \mathfrak{T}} u_M = \prod_{\lambda \in L} (1 + u_\lambda).
$$

让我们定义理想$\mathfrak{a}_\beta$如本号开头，并让$\beta \in \mathbf{N}^{(I)}$。存在 $L$ 的有限子集 $L_0$，使得 $u_\lambda \in \mathfrak{a}_\beta$ 对应于 $\lambda \notin L_0$。那么对于每个 $M \in \mathscr{S}$ 这样 $M \not\subset L_0$ 我们就有 $u_M \in \mathfrak{a}_\beta$。由此可见，族 $(u_M)_{M \in \mathfrak{T}}$ 是可求和的。另一方面，对于 $L$ 中的任意有限子集 $M_0$，我们有

$$
\sum_{M \subset M_0} u_M = \prod_{\lambda \in M_0} (1 + u_\lambda).
$$

沿着过滤后的有序集合$\mathfrak{T}$，左边有极限$\sum_{M \in \mathfrak{T}} u_M$。因此右边有极限$\sum_{M \in \mathfrak{T}} u_M$，同时证明了(i)和(ii)。

#### 命题 3 {#alg-iv-s4-prop-3 .statement tag=06C2}

*让*$u = \sum a_\nu X^\nu \in \mathbf{A}[[\mathbf{I}]]$*和*$m$*整数*$> 0$。 *对于每个* $n \in \mathbf{N}$ *让* $(\alpha_{\nu, n})_{\nu \in \mathbf{N}^{(I)}}$ *成为* $u^n$的系数族。 *如果*$\alpha_0^m = 0$，*则*$\alpha_{\nu, n} = 0$*对于*$n \geq |\nu| + m$。

设$\nu \in \mathbf{N}^{(I)}$和$n \in \mathbf{N}$。我们有

$$
\alpha_{\nu,n} = \sum_{\nu(1) + \cdots + \nu(n) = \nu} \alpha_{\nu(1)} \cdots \alpha_{\nu(n)} .
$$

如果$n \geq |\nu| + m$和$\nu(1) + \cdots + \nu(n) = v$，我们有$|\nu(1)| + \cdots + |\nu(n)| \leq n - m$。因此，我们有$v(r) = 0$和$\alpha_{v(r)} = a_r$，对于$r$至少有$m$不同的值；由此得出结果$\alpha_{\nu(1)} \cdots \alpha_{\nu(n)} = 0$、从而。

#### 推论{#alg-iv-s4-n2-cor-1 .statement tag=06C3}

— 设 $u \in A[[I]]$；那么对于 $\lim_{n \to \infty} u^n = 0$ 来说，$u$ 的常数项是幂零的，这是充分必要的。

令$a_0$为$u$的常数项。 $u^n$的常数项是$\alpha_0^n$，因此规定的条件是必要的；根据命题 3 就足够了。

### 3.代换

设 $E$ 为 $A$ 代数。 $E$上的拓扑被认为是线性的，如果它在平移下不变并且存在$E$理想的0由……组成的邻域的基本系统（Gen.Top.，III，p. 223）。 $E$上的拓扑则与其$A$代数结构兼容（当$A$携带离散拓扑时）。具有线性拓扑的 $A$ 代数称为线性拓扑 $A$ 代数。

#### 命题 4 {#alg-iv-s4-prop-4 .statement tag=06C4}

— 令 $I$ 为集合，并且 $E$ 是一个结合的、可交换的、单位的、线性拓扑分离的完全 $A$ 代数。

(i) 设$\varphi$为$A[[I]]$到$E$和$x_i = \varphi(X_i)$的连续同态。然后：
(a) 对于所有 $i \in I$，$x_i^n$ 趋于 0，因为 $n$ 趋于 $+ \infty$；
(b) 如果 $I$ 无穷大，则$x_i$ 沿着有限子集的补集过滤器$I$ 趋于 0。

(ii) 设$x = (x_i)_i$、$_I$为(i)的$E$满足a)和b)的元素族。那么在 $A[[I]]$ 到 $E$ 中存在一个且唯一的一个单位连续同态 $\varphi$，使得对于所有 $i \in I$ 都有 $\varphi(X_i) = x_i$。

对于所有$i \in I$，$A[[I]]$中的$X_i^n$明显趋于0，因为$n$趋于$+ \infty$；另一方面，当$I$无穷大时，$X_i$沿着有限子集的补集过滤器$I$趋于0。这就证明了(i)。

设$(x_i)_{i \in I}$为(i)的$E$满足条件a)和b)的元素族，设$\psi$为$A[(X_i)_{i \in I}]$的同态$u \mapsto u((x_i)_{i \in I})$入$E$，并令$V$是$E$的0的邻域，这是$E$的理想。 b) 存在$I$的有限子集$J$，使得$x_i \in V$对于所有$i \in I - J$。接下来存在 a) 整数 $n \geq 0$，使得 $x_i^n \in V$ 对于所有 $i \in J$。令$\beta$为$\mathbf{N}^{(I)}$的元素，使得$\beta_i = n - 1$代表$i \in J$，$\beta_i = 0$代表$i \in I - J$。如果我们在No. 2开始时定义是$A[[I]]$的理想$a_\beta$（IV，p. 26），那么

$$
u \in A[(X_i)_{i \in I}] \cap a_\beta \Rightarrow \psi(u) \in V
$$

这表明，如果我们为$A[(X_i)_{i \in I}]$配备由$A[[I]]$诱导的拓扑，则$\psi$是连续的。由于$E$是分离且完整的，$\psi$扩展将$A[[I]]$的连续单位同态$\varphi$转化为$E$。我们为所有 $i \in I$ 提供了 $\varphi(X_i) = \psi(X_i) = x_i$。最后让$\varphi'$是$A[[I]]$到$E$的连续单位同态，使得$\varphi'(X_i) = x_i$。对于所有$u \in A[(X_i)_{i \in I}]$，我们都有$\varphi'(u) = \varphi(u)$，因此$\varphi' = \varphi$，因为$A[(X_i)_{i \in I}]$在$A[[I]]$中是稠密的。

让我们保留之前的记号。如果$u \in A[[I]]$，$u$的像由$\varphi$表示为$u(x)$或$u((x_i)_{i \in I})$（或者如果$I = (1, 2, ..., n)$也为$u(x_1, ..., x_n)$），并且称为由代换获得的$E$的元素 $u$中的$X_i$使用$x_i$，或者$u$中的值用于$X_i$中的值$x_i$，或者$X_i = x_i$中的$u$中的值。特别是我们有$u = u((X_i)_{i \in I})$。

令 $E'$ 为结合交换且酉线性拓扑的分离完备$A$-代数。令$\lambda$为$E$到$E'$的连续单位同态，$(x_i)_{i \in I}$为$E$满足条件a）和b）的元素族，第4条（IV）， p. 28）。家庭$(\lambda(x_i))_{i \in I}$同样满足条件a)和b)。对于每 $u \in A[[I]]$ 我们有

$$
\lambda(u((x_i)_{i \in I})) = u((\lambda(x_i))_{i \in I}),
$$

对于映射$u \mapsto A(u((x_i)_{i \in I}))$来说，是$A[[I]]$到$E'$的连续单位同态，对于所有$i \in I$，变换$X_i$到$\lambda(x_i)$。

如果$J$和$K$是两个集合，我们用所有族$(g_j)_{j \in J}$满足的$A_{J, K}$集合表示以下条件：
(i) 对于所有$j \in J$，$g_j$是$A[[K]]$的元素，其常数项是幂零的；
(ii) 如果 $J$ 是无限的，$g_j$ 沿着有限子集的补集过滤器$J$ 趋于 0。

我们注，如果$J$是有限的，则在$A[[K]]$属于到$A_{J, K}$中，形式幂级数$(g_j)_{j \in J}$的每个族都没有常数项。

让$(g_j)_{j \in J}$在$A_{J, K}$中。由科。根据第 3 号提案（IV、p. 28），我们对所有 $j \in J$ 都有 $\lim_{n \to \infty} g_j^n = 0$。让$f \in A[[J]]$；我们可以用$g_j$代替$f$中的变量指标$j$，得到形式化的幂级数$f((g_j)_{j \in J})$属于到$A[[K]]$。此外，映射$f \mapsto f((g_j)_{j \in J})$是$A$-代数$A[[J]]$到$A[[K]]$的连续同态。

特别是如果$J = (1, ..., p)$和$f \in A[[X_1, ..., X_p]]$，我们可以用正式的幂级数$g_j \in A[[K]]$代替每个$X_j$，而无需常数项；这个代换的结果写成$f(g_1, ..., g_p)$。

设$x = (x_k)_{k \in K}$是第4条命题（IV，p. 28）的$E$满足条件a）和b）的元素族。我们应用(3)，将$A[[K]]$中的$A$同态$u \mapsto u(x)$化为$E$；我们得到

$$
f((g_j)_{j \in J})(x) = f((g_j(x))_{j \in J}).
$$

设$f = (f_i)_{i \in I} \in (A[[J]])^I$和$g = (g_j)_{j \in J} \in A_{J, K}$。我们用$f(g)$或$f \circ g$元素$(f_i((g_j),_{\epsilon_J}))_{i \in I}$或$(A[[K]])^I$来表示。如果$f \in A_{I, J}$，我们有$f \circ g \in A_{,,K}$，因为$A[[I]]$到$A[[K]]$的映射$f \mapsto f((g_j)_{i, J})$是连续的。

让$f \in (A[[J]])^I$，$g \in A_{J, K}$，$h \in A_{K, L}$。然后 $g \circ h \in A_{J, L}$ 并根据 (4)，我们有
$$
(f \circ g) \circ h = f \circ (g \circ h).
$$

### 4.可逆正式幂级数

#### 命题 5 {#alg-iv-s4-prop-5 .statement tag=06C5}

— *在形式幂级数的环 $A[[T]]$ 中，在一个不定式中，多项式 $1 - T$ 是可逆的，我们有* $(1 - T)^{-1} = \sum_{n=0}^m T^n$。

对于
$$
(1 - T) \left( \sum_{n=0}^\infty T^n \right) = \sum_{n=0}^\infty T^n - \sum_{n=0}^\infty T^{n+1} = 1.
$$

#### 命题 6 {#alg-iv-s4-prop-6 .statement tag=06C6}

— *令$u \in A[[I]]$；那么要使$u$在$A[[T]]$中可逆，其常数项在$A$中可逆是必要且充分的。*

假设存在$v \in A[[I]]$使得$uv = 1$。设$a, \beta$为$u$和$v$的常数项，则$\alpha \beta = 1$，所以$a$可逆。

相反，假设$u$的常数项$a$是可逆的。那么存在正式的幂级数$t \in A[[I]]$使得$u = \alpha (1 - t)$和$\omega(t) > 0$。现在有环同态 $\varphi : A[[T]] \to A[[I]]$使得$\varphi(T) = t$，并且$1 - T$在$A[[T]]$中是可逆的（命题5）；因而 $1 - t$ 在 $A[[I]]$ 中是可逆的，因而 $u$ 也是如此。

#### 注 {#alg-iv-s4-n4-rem-1 .statement tag=06C7}

— 令 $A$ 为所有形式幂级数的集合，其中常数项 1。根据第 6 条命题，$M$ 是乘法下的交换律群；因而，$A[[I]]$的乘法群是$M$的直接乘积和$A$的乘法群。我们将为$A$配备从$A[[I]]$衍生的拓扑。对于IV中的每个$\beta \in \mathbf{N}^{(I)}$，p. 26定义了$A[[I]]$的理想$a_\beta$；那么$1 + a_\beta$是$M$的子群，并且族$(1 + a_{\beta'})$是$M$中1的邻域的基本系统。由于$M$中的乘法是连续的，我们看到$A$是拓扑群（Gen.Top.，III，p. 223）；在其他字中，*映射*$f \mapsto f^{-1}$*在*$M$中连续。

设$K$为交换域，以及由有理分式构成的有理分式$K((X_i)_{i \in I})$的域和$\mathscr{O}$子环，其中$K^1$的元素0可置换。如果$f \in \mathscr{O}$，我们有$f = \frac{u}{v}$，其中$u$和$v$是多项式，使得$v$的常数项是$\neq 0$，因此$v$在$K[[I]]$中是可逆的。我们可以立刻验证$K[[I]]$的元素$uv^{-1}$只依赖于$f$；我们说形式幂级数 $uv^{-1}$ 是有理分数* $\frac{u}{v}$ 起源处的 *展开。 映射 $f \mapsto uv^{-1}$ 是 $\mathscr{O}$ 中的单同态变成 $K[[I]]$；我们经常将认同$\mathscr{O}$及其像置于映射之下。

### 5. Taylor 的公式正式幂级数

令$X = (X_i)_{i \in I}$和$Y = (Y_i)_{i \in I}$是相对于相同指标集合I的两个不定族。我们用$X + Y$表示$A[[X, Y]]$中正式幂级数的家族$(X_i + Y_i)_{i \in I}$。显然，我们可以在正式的幂级数$u \in A[[X]]$中用$X_i + Y_i$代替$X_i$，结果写作$u(X + Y)$。对于每个$\nu \in \mathbf{N}^{(I)}$，我们用$\Delta^\nu u$表示形式上幂、级数、$u(X + Y)$中$Y^\nu$的系数，被视为属于到$A[[X]][[Y]]$（III、p. 456）。在其他字中，我们有

$$
u(X + Y) = \sum_\nu \Delta^\nu u(X) \cdot Y^\nu \quad (u \in A[[X]]) .
$$

将 $(0, X)$ 替换为 $(X, Y)$ 我们得到

$$
u(X) = \sum_\nu \Delta^\nu u(0) \cdot X^\nu ;
$$

在其他字中，$\Delta^\nu u$的常数项是$u$中$X^\nu$的系数。由于 $A[[X]]$ 的映射 $u \mapsto u(X + Y)$ 到 $A[[X, Y]]$ 是连续的，因此 $A[[X]]$ 的映射 $u \mapsto \Delta^\nu u$ 到其自身也是连续的。

与多项式 (IV, p. 7) 的情况一样，我们可以证明公式

$$
\Delta^\sigma(uv) = \sum_{v+\rho=\sigma} \Delta^\nu(u) \Delta^\rho(v) ,
$$
$$
\Delta^\rho \Delta^\sigma u = \frac{(\rho + \sigma)!}{\rho! \; \sigma!} \Delta^{\rho + \sigma} u .
$$

二项式公式 (I, p. 99, Cor. 2) 对于$\Delta^\nu u$，当 $u = \sum_\lambda \alpha_\lambda X^\lambda$ 时，给出以下值

$$
\Delta^\nu u = \sum_\lambda \alpha_{\lambda + \nu} \frac{(\lambda + \nu)!}{\lambda! \; \nu!} X^\lambda .
$$

特别考虑$\nu = \epsilon_i$的情况，即$\nu_i = 1, \nu_j = 0$对应$j \neq i$。我们将放入$D_i u = \Delta^{\epsilon_i} u$；换句话说，$D_i u$是$Y_i$在$u(X + Y)$中的系数。根据 (10) 我们有

$$
D_i u = \sum_\lambda (\lambda_i + 1) \alpha_{\lambda + \epsilon_i} X^\lambda ;
$$

特别是对于 $j \neq i$，我们有 $D_i(X_i) = 1$ 和 $D_i(X_j) = 0$。 公式(8)表明$D_i$是$A[[X]]$的推导，并且从(9)我们推导出关系

$$
D^\nu u = \nu! \; \Delta^\nu u
$$

就像多项式 (IV, p. 8) 的情况一样（我们将$D^\nu = \prod_{i \in I} D_i^{\nu_i}$代替$\nu = (\nu_i)_{i \in I}$，放在$\mathbf{N}^{(I)}$中）。当 A 是 Q 代数时，公式 (6)、(7) 和 (12) 隐含 « Taylor 公式 »：

$$
u(\mathbf{X} + \mathbf{Y}) = \sum \frac{1}{\nu!} D^\nu u(\mathbf{X}) \cdot \mathbf{Y}^\nu,
$$
$$
u(\mathbf{X}) = \sum \frac{1}{\nu!} D^\nu u(0) \cdot \mathbf{X}^\nu.
$$

#### 注 {#alg-iv-s4-n5-rem-1 .statement tag=0DHH}

*1) 我们常说$D_i u$是*u对X*的偏导数，；我们还使用记号$D_{x_i} u, \frac{\partial u}{\partial x_i}$和$u'_{x_i}$。对于单个不定X，唯一的偏导数$Du$（也写作$\frac{du}{dX}$或$u'$）称为$u$的*导数*。

2) 公式(9)表明A-模$A[[X]]$的自同态$A^p$通勤痛苦。因此自同态$D_i$同样成立。

3) 如果$u \in A[(X_i)_{i \in I}]$是多项式，IV、p. 6和7重合定义的多项式$A^p u$和$D_i u$与形式幂级数用相同的符号表示。

### 6.正式幂级数代数中的推导

令 I 为集合，E 为结合律、交换律、酉线性拓扑、分离且完备的 A-代数，$x = (x_i)_{i \in I}$ 是命题 4 (IV) 的 E 满足条件 a) 和 b) 的元素族。 p. 28）。令$\varphi$为$A[[I]]$到E的连续同态$u \mapsto u(x)$；它为E配备了$A[[I]]$模块结构。通过 III、p. 552，$A[[I]]$ 到 $A[[I]]$ 模 E 的 A 推导 D 为 A-线性映射 $D : A[[I]] \to E$ 满足关系
$$
D(uv) = u(x) \cdot D(v) + D(u) \cdot v(x)
$$
$A[[I]]$ 中的 $u, v$。

#### 命题 7 {#alg-iv-s4-prop-7 .statement tag=06C8}

— 令$(y_i)_{i \in I}$为E的元素族。当I无穷大时，*我们*假设$y_i$沿着I的有限子集的补集过滤器趋于0。那么存在$A[[I]]$到$A[[I]]$*-模* E 的唯一连续A-导数D，使得$D(X_i) = y_i$对于所有$i \in I$。我们有
$$
D(u) = \sum_{i \in I} (D_i u)(x) \cdot y_i \quad (u \in A[[I]]) .
$$

由于 0 在 E 中承认理想的邻域由……组成的基本系统，因此对于所有 $u \in A[[I]]$，族 $((D_i u)(x) \cdot y_i)_{i \in I}$ 在 E 中是可求和的（Gen. Top.、III、p. 263、Cor. 2）。 公式 (16) 因此定义 A-线性映射 $D : A[[I]] \to E$。我们让读者验证 D 是连续的推导。

令 $D_1$ 为 $A[[I]]$ 到 E 的连续 A 导数，使得 $D_1(X_i) = y_i$ 对于所有 $i \in I$。连续推导$D - D_1$的核是$\mathbf{A}[[\mathbf{I}]]$包含1和不定$X_i$的闭子代数B。由于多项式代数 $\mathbf{A}[(X_i)_{i \in I}]$ 在 $\mathbf{A}[[\mathbf{I}]]$ 中是稠密的，因此我们有 $B = \mathbf{A}[[\mathbf{I}]]$ 以及 $D_1 = D$。

#### 推出 1 {#alg-iv-s4-prop-7-cor-1 .statement tag=06C9}

— *令 A 为 A-代数 E 的连续推导。对于每个形式幂级数 $u \in \mathbf{A}[[\mathbf{I}]]$，族 $((D_iu)(x) \cdot \Delta x_i)_{i \in I}$ 是可求和的，我们有*

$$
\Delta(u(x)) = \sum_{i \in I} (D_iu)(x) \cdot \Delta x_i .
$$

这是从命题 7 得出的，因为映射 $u \mapsto \Delta(u(x))$ 是 $\mathbf{A}[[\mathbf{I}]]$ 的连续推导进入$\mathbf{A}[[\mathbf{I}]]$-模块 E。

#### 推论 2 {#alg-iv-s4-prop-7-cor-2 .statement tag=06CA}

— *推导 $D_i$ 是 A-代数 $\mathbf{A}[[\mathbf{I}]]$ 的唯一连续推导，使得*

$$
D_i(X_i) = 1 , \quad D_i(X_j) = 0 \quad \text{for} \quad j \neq i .
$$

这是从 Cor 得出的。 1.

#### 推论 3 {#alg-iv-s4-prop-7-cor-3 .statement tag=06CB}

— *令 $f \in \mathbf{A}[[X_1, ..., X_s]]$ 和 $g_i \in \mathbf{A}[[Y_1, ..., Y_q]]$ 为 $1 \leq i \leq p$。假设对于$1 \leq i \leq p$，$g_i$的常数项是零，并放入$h = f(g_1, ..., g_p)$。那么对于 $1 \leq j \leq q$ 我们有*

$$
\frac{\partial h}{\partial Y_j} = \sum_{i=1}^p D_i f(g_1, ..., g_p) \cdot \frac{\partial g_i}{\partial Y_j} .
$$

这是 Cor 的特殊情况 $E = \mathbf{A}[[Y_1, ..., Y_s]]$、$x_i = q_i$ 和 $A = \partial / \partial Y_j$。 1.

#### 命题 8 {#alg-iv-s4-prop-8 .statement tag=06CC}

— *令 $X = (X_i)_i$ 为不定式的有限族。
(i) 正式幂级数 $\mathbf{A}[[X]]$ 的环中的每个推导都是连续的。
(ii) 以独特的方式将多项式环$\mathbf{A}[X]$的推导转换为正式幂级数$\mathbf{A}[[X]]$扩展的环到环$\mathbf{A}[[X]]$的推导。
(iii) $(D_i)_{i \in I}$族是$\mathbf{A}[[X]]$自身的A-导数的$\mathbf{A}[[X]]$模的基。
令$b_n$为阶$\geq n$的所有形式幂级数中的集合。显然，$b_n$是环$\mathbf{A}[[X]]$中的理想，由次数$n$的单项式生成。因此 $b_n$ 由 $n$ 形式幂级数的乘积的有限和组成，没有常数项；如果 $D$ 是 $\mathbf{A}[[X]]$ 的推导，我们有*

$$
D(f_1 \cdots f_n) = \sum_{i=1}^n f_1 \cdots f_{i-1} D(f_i) f_{i+1} \cdots f_n ,
$$

从而立即得出 $Db_n \subset b_{n-1}$ 对应 $n \geq 1$。由于序列 $(b_n)_{n \geq 0}$ 是 $\mathbf{A}[[X]]$ (IV, p. 26 注) 中 0 的邻域的基本系统，因此 D 是连续的，并且 (i) 被证明。

令 $A$ 为 $A[X]$ 的推导到$A[[X]]$。论证为之前，我们可以证明对于次数$n \geq 1$的每个齐次多项式$h$，$A(h)$属于到$b, -_1$。现在令 $u \in A[[X]]$ 和 $u_n$ 为 $u$ 的次数 $n$ 的齐次分量。由于 $A(u_n) \in b, -_1$ 对于 $n \geq 1$，族 $(A(u)), \ldots$ 可以在 $A[[X]]$ 中求和，我们可以将 $A[[X]]$ 的定义推导 $D$ 化为自身

$$
D(u) = \sum_{n \geq 0} \Delta(u_n)
$$

我们有$D(b_n) \subset b_{n-1}$，因此$D$是$A[[X]]$的加法群的连续自同态。 $A[[X]] \times A[[X]]$到$A[[X]]$的映射$\Phi : (u, v) \mapsto D(uv) - uD(v) - D(u)v$是连续的，零在$A[X] \times A[X]$上。由于$A[X]$在$A[[X]]$中是稠密的，所以我们有$\Phi = 0$；在其他字中，$D$是$A[[X]]$的推导自身，延伸$A$。

最后，$A[X]$在$A[[X]]$中是稠密的，并且$A[[X]]$的每个推导都由(i)连续；因此，存在唯一的扩张 $A$ 到推导 $A[[X]]$。这就证明了(ii)。

仍有待证明(iii)。 公式 (18) (IV, p. 33) 表明族 $(D_i)_{i \in I}$ 与 $A[[X]]$ 线性无关，而公式 (16) (IV, p. 32)，应用于案例 $E = A[[X]]$，表明每个$A$-导数是$D_i$的线性组合，系数为$A[[X]]$。

#### 命题 9 {#alg-iv-s4-prop-9 .statement tag=06CD}

— 令$(u_\lambda)_{\lambda \in L}$为$A[[I]]$的元素的*可求和*族，没有常数项，并且$D$为$A$代数$A[[I]]$的连续推导。如果 $f = \prod_{\lambda \in L} (1 + u_\lambda)$ (IV, p. 27, 命题 2)，那么族 $(Du_\lambda/(1 + u_\lambda))_{\lambda \in L}$ 是可求和的，我们有

$$
D(f)/f = \sum_{\lambda \in L} D(u_\lambda)/(1 + u_\lambda) .
$$

如果$g$和$h$是$A[[I]]$中的两个可逆元，那么

$$
D(gh) = h \cdot Dg + g \cdot Dh
$$

从而除以$gh$，

$$
D(gh)/gh = D(g)/g + D(h)/h .
$$

对于$L$中的每个有限子集$M$，放入$f_M = \prod_{\lambda \in M} (1 + u_\lambda)$。从 (21) 中，我们通过卡片 $M$ 关系上的归纳进行推导

$$
D(f_M)/f_M = \sum_{\lambda \in M} D(u_\lambda)/(1 + u_\lambda)
$$

当 L 有限时，这证明了命题 9。现在假设L是无限的，并为L的有限子集的过滤有序集合写入$\mathfrak{F}$。我们有 $\lim_{\mathfrak{F}} f_M = f$，因此 (*IV*, p. 30 注)

$$
D(f)/f = \lim_{\mathfrak{F}} D(f_M)/f_M .
$$

现在，第 9 号提案接着是 (22) 中的极限。

### 7. 形式幂级数环中的解方程

#### 引理 2 {#alg-iv-s4-lem-2 .statement tag=06CE}

*让*$(g_i)_i$*成为阶*$\geq 2$*中的元素家庭*$\mathbf{A}[[\mathbf{I}]]$。 *当*$\mathbf{I}$*无限时，假设*$g_i$*沿着*$\mathbf{I}$的有限子集的补集过滤器趋于0。 *拓扑* A*-代数* $\mathbf{A}[[\mathbf{I}]]$ *存在一个且仅有一个自同构* T *使得* $T(X_i) = X_i + g_i$ *对于所有* $i \in \mathbf{I}$。 *此外，

(23)
$$
\omega(T(u) - u) \geq \omega(u) + 1
$$
*每个*$u \in \mathbf{A}[[\mathbf{I}]]$。

级数$f_i = X_i + g_i$没有常数项，当$\mathbf{I}$无穷大时，$f_i$沿着$\mathbf{I}$的有限子集的补集过滤器趋于0。因此（IV，p. 28，命题4），A-代数$\mathbf{A}[[\mathbf{I}]]$恰好存在一个连续的自同态T，使得$T(X_i) = f_i$对于所有$i \in \mathbf{I}$。对于每个$\nu \in \mathbf{N}'$，我们放入

$$
v_\nu = T(X^\nu) - X^\nu = \prod_{i \in \mathbf{I}} (X_i + g_i)^{\nu(i)} - \prod_{i \in \mathbf{I}} X_i^{\nu(i)} ;
$$

关系$\omega(g_i) \geq 2$暗示$w(v_\nu) \geq |\nu| + 1$，关系(23)立即由此而来。

让我们证明 $T$ 是*内射*。给定$u \in \mathbf{A}[[\mathbf{I}]]$使得$T(u) = 0$，通过(23)我们有$w(u) \geq w(u) + 1$，如果$u \neq 0$这是不可能的，因为$w(u)$将是正整数。

对于$\mathbf{A}[[\mathbf{I}]]$中的每个形式级数$v$，我们用$H_n(v)$表示其次数$n$的齐次成分。让我们用递归方程将连续的映射$S, : \mathbf{A}[[\mathbf{I}]] \to \mathbf{A}[[\mathbf{I}]]$代入$S_0(v) = H_0(v)$和定义

(24)
$$
S_n(v) = H_n \left( v - T \left( \sum_{k=0}^{n-1} S_k(v) \right) \right) \quad \text{for} \quad n \geq 1
$$

把$S(v) = \sum_{n \geq 0} S_n(v)$；如果$\nu \in \mathbf{N}^{(\mathbf{I})}$和$n = |\nu|$，则$S(v)$中$X^\nu$的系数$S^\nu(v)$等于$S,(\nu)$中$X^\nu$的系数；由于$S,$是连续的映射，所以映射$S^\nu : \mathbf{A}[[\mathbf{I}]] \to \mathbf{A}$是连续的。因此，通过$\mathbf{A}[[\mathbf{I}]] = \mathbf{A}^{\mathbf{N}^{(\mathbf{I})}}$上的乘积拓扑的定义，映射$S : \mathbf{A}[[\mathbf{I}]] \to \mathbf{A}[[\mathbf{I}]]$是连续的。

我们将为所有$v \in \mathbf{A}[[\mathbf{I}]]$证明关系$T(S(v)) = v$，这将完成引理的证明。设 $v \in \mathbf{A}[[\mathbf{I}]]$、$u_n = S_n(v)$ 和 $u = S(v)$。令 $n$ 为正整数，使得

(25)$_n$
$$
\omega(v - T(u)) \geq n .
$$

我们有$w(u - (u_0 + \ldots + u_{n-1})) \geq n$，从而

$$
\omega(T(u) - T(u_0 + \ldots + u_{n-1}) - u_n) \geq n + 1
$$

由（23）。现在递归方程（24）表明

$$
u_n = H_n(v - T(u_0 + \cdots + u_{n-1}))
$$

由(26) 可知，形式幂级数 $v - T(u)$ 和$v - T(u_0 + \ldots + u_{n-1}) - u_n$ 具有相同的齐次分量次数 $n$，且该分量为零，由(27) 得到。因此我们有$w(v - T(u)) \geq n + 1$，即$(25)_n$意味着$(25)_{n+1}$。由于$(25)_0$显然成立，因此对于每个整数$n \geq 0$、从而$v = T(u) = T(S(v))$，我们都有$\omega(v - T(u)) \geq n$，这有待证明。

对于本号的其余部分，对于任何集合$I$，我们将用$(f_i)_{i \in I}$满足家庭的$A\{I\}$集合表示以下条件：
(i) 对于每个 $i \in I$，$f_i$ 是 $A[[I]]$ 的元素，没有常数项；
(ii) 如果 $I$ 是无限的，$f_i$ 沿着 $I$ 的有限子集的补集过滤器趋于 0。

集合 $A\{I\}$ 是合成律 $(f, g) \mapsto f \circ g$ 的幺半群，$\{X_i\}_{i \in I}$ 为单位元。 $A\{I\}$ 的可逆元的集合因此是群。

另一方面，令$E$为$A$-代数$A[[I]]$的所有连续单位自同态的幺半群，留下所有形式幂级数的理想，而没有常数项不变量。如果$f \in A\{I\}$和$g \in A[[I]]$，则定义了元素$g(f)$。对于固定的$f$，$A[[I]]$的映射$g \mapsto g(f)$自身就是$E$的元素$W_f$。如果 $f_1, f_2 \in A\{I\}$ 和 $g \in A[[I]]$，我们有公式 (5) (IV, p. 30)

$$
W_{f_1 \circ f_2}(g) = g(f_1 \circ f_2) = g(f_1) \circ f_2 = W_{f_2}(W_{f_1}(g))
$$

因此，$f \mapsto W_f$是与$A\{I\}$相反的幺半群的同态进入$E$。根据命题 4 (IV, p. 28)，这个同态是双射的。

令 $f = (f_i)_{i \in I} \in A\{I\}$ 和 $\sum_{j \in I} \alpha_{ij} X_j$ 为$f_i$ 次数 1 的齐次分量。对于$I$中的任何固定$j$，我们有$\alpha_{ij} = 0$，除了后缀$i$的有限数，通过上面的假设（ii）。如果$(\lambda_i) \in A^{(I)}$，我们就有$\left( \sum_{j \in I} \alpha_{ij} \lambda_j \right) \in A^{(I)}$。

我们用$T_f$表示$A$线性映射$^1$

$$
(\lambda_i) \mapsto \left( \sum_{j \in I} \alpha_{ij} \lambda_j \right)
$$

$A^{(I)}$ 变为 $A^{(I)}$。如果$g \in A\{I\}$，很容易验证

$$
T_{f \circ g} = T_f \circ T_g .
$$

$^1$ 有时 $T_f$ 称为线性映射与 $f$ 相切。

#### 命题 10 {#alg-iv-s4-prop-10 .statement tag=06CF}

— 令 $f \in A\{I\}$；那么下面的条件是等价的：
(i) 对于律 $\circ$，$f$ 在 $A\{I\}$ 中是可逆的；
(ii) $T_f$ 在环 $\mathrm{End}(A^{(I)})$ 中可逆。

蕴涵 (i) $\Rightarrow$ (ii) 是 (28) 中的直接的。现在假设 $T_f$ 在 $\mathrm{End}(A^{(I)})$ 中是可逆的。存在$g = (g_i)_i \in A\{I\}$，使得每个$g_i$是次数$l$的齐次，并且$T_g \circ T_f$是$A^{(I)}$的恒等映射。写$h = g \circ f$；则(28)可知$T_h$是$A^{(I)}$的恒等映射，相当于断言$\omega(h_i - X_i) \geq 2$。因此，通过 IV 的引理 2，p. 35 $h$ 在 $A\{I\}$ 中是可逆的。显然，$g$ 在 $A\{I\}$ 中可逆，因此 $f$ 在 $A\{I\}$ 中可逆。

#### 推论{#alg-iv-s4-n7-cor-1 .statement tag=06CG}

— 设 $f_i(Y_1, Y_2, \ldots, Y_q, X_1, X_2, \ldots, X_p)$ ($1 \leq i \leq q$) 为 $q$ 正式幂级数，$A[[Y_1, \ldots, Y_q, X_1, \ldots, X_p]]$ 中没有常数项。如果形式幂级数 $D = \det \left( \frac{\partial f_i}{\partial Y_j} \right)$ 的常数项在 $A$ 中可逆，则 $q$ 形式幂级数 $u_1(X_1, \ldots, X_p), \ldots, u_q(X_1, \ldots, X_p)$ 中恰好存在一个系统，使得
$$
f_i(u_1, \ldots, u_q, X_1, \ldots, X_p) = 0 \quad (1 \leq i \leq q).
$$
将$f_{q+1} = X_1, \ldots, f_{q+p} = X_p$，$f = (f_1, \ldots, f_{p+q})$，则$\det T_f$等于$D$的常数项，因此在$A$中可逆；因此 $T_f$ 是可逆的。根据命题 10，存在形式幂级数，没有常数项
$$
g_1, \ldots, g_{q+p} \in A[[Y_1, \ldots, Y_q, X_1, \ldots, X_p]]
$$
这样在写作时
$$
g = (g_1, \ldots, g_{p+q}), \quad 1_{p+q} = (Y_1, \ldots, Y_q, X_1, \ldots, X_p)
$$
我们有$f \circ g = g \circ f = 1_{p+q}$。 关系 $f \circ g = 1_{p+q}$，特别是给出
$$
g_{q+1} = X_1, \ldots, g_{q+p} = X_p.
$$
因此
$$
f_i(g_1, \ldots, g_q, X_1, \ldots, X_p) = Y_i \quad (1 \leq i \leq q).
$$
现在放
$$
u_i(X_1, \ldots, X_p) = g_i(0, \ldots, 0, X_1, \ldots, X_p) \quad (1 \leq i \leq q);
$$
将 (30) 中的每个 $Y_i$ 替换为 0，我们得到所需的关系 (29)。

相反，假设环 $A[[X_1, \ldots, X_p]]$ 满足关系 (29) 中的形式幂级数 $u_1, \ldots, u_q$。 关系 $g \circ f = 1_{p+q}$ 意味着
$$
g_i(f_1, \ldots, f_q, X_1, \ldots, X_p) = Y_i \quad (1 \leq i \leq q);
$$
将(32)中的$u_i$代入$Y_i$代入$1 \leq i \leq q$，得(31)，系统(29)的解从而唯一性。

### 8.正式幂级数超过整环

#### 命题 11 {#alg-iv-s4-prop-11 .statement tag=06CH}

— 假设 $A$ 是整环。

(i) *环* $A[[I]]$ *又是整环*。

(ii) *如果* $u, v$ *非零元素 of* $A[[I]]$，*则* $\omega(uv) = \omega(u) + \omega(v)$。

对于每个$J \subset I$，令$\varphi_J$为$A[[I]]$的同态代入$A[[J]]$，通过将$A[[I]]$的每个元素代入，当$i \in J$时将$X_i$代入$X_i$，当$X_i$时代入0 $i \in I - J$。令$u, v$为$A[[I]]$、$p = \omega(u)$、$q = \omega(v)$的非零元素；存在 $I$ 的有限子集 $J$ 使得

$$
\varphi_J(u) \neq 0,\ \varphi_J(v) \neq 0,\ \omega(\varphi_J(u)) = p,\ \omega(\varphi_J(v)) = q.
$$

令 a（分别 b）为 $\varphi_J(u)$（分别 $\varphi_J(v)$）的次数 $p$（分别 $q$）的齐次分量。由于 $J$ 是有限的，因此 a 和 b 是多项式。我们有$a \neq 0, b \neq 0$，因此有$ab \neq 0$（IV，p. 9，提案 8）。因此 $\varphi_J(u)\ \varphi_J(v)$ 是非零，阶 $p + q$。由此可见 $uv \neq 0$ 和 $\omega(uv) \leq p + q$；但显然$\omega(uv) \geq p - q$。

### 9. The field of fractions of the ring of formal power series in one indeterminate over a field

如果K是交换域，我们用整环$K[[X]]$分数的$K((X))$域来表示。

#### 命题 12 {#alg-iv-s4-prop-12 .statement tag=06CI}

— *每个非零元素* $u$ *of* $K((X))$ *可以以独特的方式写为* $u = X^k v$，*其中* $k \in \mathbf{Z}$ *和* $v$ *是正式的幂级数 in* $X$ *of 阶* 0。

设$u = w/t$，其中$w, t$是$K[[X]]$的非零元素。我们有$w = X^r w_1, t = X^s t_1$，其中$r, s \in \mathbf{N}$和$w_1, t_1$是阶0的形式幂级数，因此在$K[[X]]$中可逆（IV，p. 30，命题6）。那么$u = X^{r-s} w_1 t_1^{-1}$和$w_1 t_1^{-1}$是阶0的正式幂级数。

让我们证明唯一性。假设$u = X^{k_1} v_1 = X^{k_2} v_2$，其中$k_1, k_2 \in \mathbf{Z}$和$v_1, v_2$是阶0的形式幂级数。由于$X^{k_1 - k_2} = v_2 v_1^{-1}$是阶0的形式幂级数，我们有$k_1 = k_2$ 从而$v_1 = v_2$，这就证明了唯一性断言。

我们可以说，$K((X))$的元素是$X$中的*广义形式幂级数*，系数在$K$中，或者在不会产生混淆的情况下简单地形式化幂级数（然后称为$K[[X]]$的元素） *正式幂级数带正指数*)；如果第12条命题中定义的$u \neq 0$、整数$k$也称为$u$的*阶*，写成$\omega(u)$，即使它是$< 0$；我们还放了$\omega(0) = \infty$。可以立刻验证

$$
\begin{align*}
\omega(u + v) &\geq \inf(\omega(u), \omega(v)) \\
\omega(u + v) &= \inf(\omega(u), \omega(v)) \quad \text{if}\ \ \omega(u) \neq \omega(v) \\
\omega(uv) &= \omega(u) + \omega(v)
\end{align*}
$$

仍然适用于广义形式幂级数。特别是，如果$u \neq 0$，则$w(u^{-1}) = -w(u)$。 \* 在其他字（Comm. Alg.、VI, § 3, No. 6、p. 392、Def. 3）中，w 是域 $K((X))$ 的标准化离散估值。 \*

对于每个整数$n \in \mathbf{Z}$，令$p_n$为所有$u \in K((X))$中的集合，使得$\omega(u) \geq n$。则(p.)，，，是加法群$K((X))$子群递减序列，和交0；因此，$K((X))$上存在拓扑，在翻译下不变，其中$(p_n)_{n \in \mathbf{Z}}$是0的邻域的基本系统（Gen.Top.，III，p. 223）。我们可以很容易地验证$K((X))$是一个拓扑域（Gen.Top.，III，p. 281），并且$K[[X]]$是$K((X))$的开闭子空间。

令$(\alpha_n)_{n \in \mathbf{Z}}$是$K$的元素族，并假设存在整数N，使得$a_n = 0$对于所有$n < N$。然后家庭的 $(\alpha_n X^n)_{n \in \mathbf{Z}}$ 可在 $K((X))$ 中求和（Gen. Top., III, p. 263, Cor.）；放入$u = \sum_{n \in \mathbf{Z}} \alpha_n X^n$，则$u = 0$当且仅当$a_n = 0$对于所有$n$；否则，$u$的阶是最小的整数 k，使得$\alpha_k \neq 0$。最后，$K((X))$的每个元素都可以以独特的方式写成形式$\sum_{n \in \mathbf{Z}} \alpha_n X^n$，其中序列$(\alpha_n)$对于所有足够大n满足$\alpha_{-n} = 0$。

由于环$K[X]$是$K[[X]]$的子环，每个有理分式$u/v \in K(X)$（u，v是X中的多项式）可以用（广义）形式幂级数$uv^{-1}$来识别$K((X))$，我们在原点将其称为展开；因此，域$K(X)$被识别为$K((X))$的子域。

### 10.指数和对数

通过指数幂级数，我们可以理解$Q[[X]]$的元素$\sum_{n \geq 0} \frac{X^n}{n!}$；它将由 exp X 或 $e^X$ 表示。

#### 命题 13 {#alg-iv-s4-prop-13 .statement tag=06CJ}

— 在$Q[[X, Y]]$，我们有$e^{X+Y} = e^X e^Y$。

对于二项式公式给出

$$
\frac{(X+Y)^n}{n!} = \sum_{i+j=n} \frac{X^i}{i!} \frac{Y^j}{j!}
$$

因此

$$
e^X e^Y = \left( \sum_{i \geq 0} \frac{X^i}{i!} \right) \left( \sum_{j \geq 0} \frac{Y^j}{j!} \right) = \sum_{i,j \geq 0} \frac{X^i}{i!} \frac{Y^j}{j!} = \sum_{n \geq 0} \sum_{i+j=n} \frac{X^i}{i!} \frac{Y^j}{j!}
$$
$$
= \sum_{n \geq 0} \frac{(X+Y)^n}{n!} = e^{X+Y}.
$$

我们将$Q[[X]]$中的定义两个元素$e(X)$、I(X)

$$
e(X) = e^X - 1 = \sum_{n \geq 1} \frac{X^n}{n!}
$$

(34)
$$
l(X) = \sum_{n \geq 1} (-1)^{n-1} \frac{X^n}{n}.
$$

我们有
(35)
$$
e(X+Y) = e(X) + e(Y) + e(X)e(Y)
$$
(36)
$$
D(e^X) = D(e(X)) = e^X
$$
(37)
$$
D(l(X)) = \sum_{n \geq 0} (-X)^n = (1+X)^{-1}.
$$

#### 命题 14 {#alg-iv-s4-prop-14 .statement tag=06CK}

— 我们有 $l(e(X)) = e(l(X)) = X$。

级数 l 和 e 没有常数项，并且它们的次数 1 的项等于 X。根据IV、p. 37的第10条命题，足以证明公式$l(e(X)) = X$。由公式 (36) 和 (37) 以及 Cor。 IV、p. 33 中的 3 个我们有

$$
D(l(e(X))) = (1 + e(X))^{-1} D(e(X)) = (e^X)^{-1} e^X = 1
$$

从而$I(e(X)) = X$。

令 K 为 Q 代数，则 K[[I]] 的元素在没有常数项形式的情况下是加法下的可交换群 $\mathscr{E}$。 K[[I]] 的元素，其中常数项 1 形式是乘法 (IV, p. 30) 下的可交换群 $\mathbf{A}$。对于每个$f \in \mathscr{E}$，我们可以得到$\mathscr{E}$的定义、元素、$e \circ f$和$I \circ f$，并且根据上面的第14条命题，映射、$f \mapsto l \circ f$和$f \mapsto e \circ f$是置换的互逆$\mathscr{E}$；显然它们是连续的。从$\exp X = e(X) + 1$开始，我们看到指数映射$f \mapsto \exp f = e \circ f + 1$是$\mathscr{E}$到$\mathscr{M}$的连续双射。根据IV、p. 29和第13号提案的公式(4)，我们有$\exp(f+g) = (\exp f)(\exp g)$对应$f, g \in \mathscr{E}$。因此，拓扑群$\mathscr{E}$到拓扑群$\mathbf{A}$的指数是同构。

$\mathscr{M}$乘以$\mathscr{E}$的逆同构称为对数，写为$g \mapsto \log g$。因此，我们在 $\mathscr{M}$ 中得到 $g$ 的 $\log g = l(g-1)$，特别是，

(38)
$$
\log(1+X) = l(X).
$$

由于 $\mathscr{M}$ 右 $\mathscr{E}$ 的对数为同态，因此公式 $(1+X)(1+Y) = 1 + (X+Y+XY)$ 意味着

(39)
$$
l(X) + l(Y) = l(X+Y+XY).
$$

令 $(u_\lambda)_{\lambda \in L}$ 为 $\mathscr{B}$ 的元素的可和族，则族 $(\exp u_{\lambda})_{\lambda \in L}$ 是可乘的，我们有

(40)
$$
\exp \left( \sum_{\lambda \in L} u_{\lambda} \right) = \prod_{\lambda \in L} \exp u_{\lambda}.
$$

类似地，如果 $(f_\lambda)_{\lambda \in L}$ 是 A 的元素的可乘族，则族 $(\log f_\lambda)_{\lambda \in L}$ 是可求和的，我们有

(41)
$$
\log \left( \prod_{\lambda \in L} f_\lambda \right) = \sum_{\lambda \in L} \log f_\lambda .
$$

令$g \in A$，并令D为$K[[I]]$的连续推导。我们有 $\log g = l(g - 1)$，因此 Cor. IV、p. 33 中的 3 个和 (37) 我们有

(42)
$$
D \log g = D(g)/g .
$$

表达式$D(g)/g$称为g（相对于D）的对数导数。

### 习题{#alg-iv-s4-exercises}

§ 4](exercises/s4/)参见[习题。
