---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 4
section_title: Lifting in complete rings
lang: zh
source: ac-i-vii
book_pages: 209-226, 255-258
pdf_pages: 0229-0246, 0275-0278
extraction: ocr
subsections:
    - "no": 1
      title: STRONGLY RELATIVELY PRIME POLYNOMIALS
      page: 209
      pdf_page: 229
    - "no": 2
      title: RESTRICTED FORMAL POWER SERIES
      page: 212
      pdf_page: 232
    - "no": 3
      title: HENSEL'S LEMMA
      page: 215
      pdf_page: 235
    - "no": 4
      title: COMPOSITION OF SYSTEMS OF FORMAL POWER SERIES
      page: 218
      pdf_page: 238
    - "no": 5
      title: SYSTEMS OF EQUATIONS IN COMPLETE RINGS
      page: 220
      pdf_page: 240
    - "no": 6
      title: APPLICATION TO DECOMPOSITIONS OF RINGS
      page: 225
      pdf_page: 245
statements: 23
exercises: 8
content_sha256: f6aac2b6db7e526e665db0802f133afff49c34441a0691a0ef4182f989c19b6e
translated_from: content/en/ac/III/04_s4_lifting_in_complete_rings.md
translation_method: google
source_content_sha256: e207aa232d5bd052ada28a852533dc7566c32021e210764a8b52a3fbf49d5170
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 19412e545b046dd1099c0c367d1a8e0a0d32097abd53ad1a6670080a9f32c86a
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 4. 完整提升环

### 1. 强相对素多项式

设$R$为交换环。如果主理想$Rx$和$Ry$互质，则$R$的两个元素$x, y$被称为*强互质*，在其他字（章II, § 1, no. 2）如果$R x + R y = R$；相当于说，$R$中存在两个元素$a, b$，使得$ax + by = 1$。

#### 引理 1（“欧几里得的引理”）{#ac-iii-s4-lem-1 .statement tag=04HS}

*设$x, y$是$R$的两个强互质元素；如果 $z \in R$ 满足 $x$ 除 $yz$，则 $x$ 除 $z$。*

如果$1 = ax + by$，则$z = x(az) + (yz)b$。

如果 $x$ 和 $y$ 在 $R$ 中强互质，则
$$
R_{xy} = (Rx) \cap (Ry)
$$
（章II, § 1, no. 2，命题5）；如果$R$是整环，两个强互质元素则有一个*lcm*等于它们的乘积（*代数*，章VI, § 1, no. 8），因此在*代数*，章的意义上是*相对质数* VI, § 1, no. 12。相反，如果 $R$ 是主理想整环，则两个互质元素也强互质，如下从 Bezout 恒等式 (*代数*, 章 VII, § 1, no. 2, 定理 1)。

对于多项式环，有以下结果：

#### 命题 1 {#ac-iii-s4-prop-1 .statement tag=04HT}

*设$\mathbf{A}$为交换环，并且$P$和$P'$是$\mathbf{A}[X]$中的两个强互素多项式。假设 $P$ 是单数且为次数 $s$。那么 $\mathbf{A}[X]$ 中的每个多项式 $T$ 都可以唯一地写成形式*
$$
T = PQ + P'Q'
$$
*其中 $Q \in \mathbf{A}[X]$、$Q' \in \mathbf{A}[X]$ 和 $\deg(Q') < s$。
如果进一步$\deg(T) \leq t$和$\deg(P') \leq t - s$，则$\deg(Q) \leq t - s$。*

由于$P$是单调的，$PR \neq 0$对于$\mathbf{A}[X]$的每个多项式$R \neq 0$，在本例中为$\deg(PR) = s + \deg(R)$。

令$T$为$\mathbf{A}[X]$中的任意多项式。由于$P$和$P'$生成的理想是$\mathbf{A}[X]$的整体，因此存在多项式$Q_1$和$Q'$使得
$$
T = PQ_1 + P'_1Q'_1;
$$
由于 $P$ 是次数 $s$ 的 monic，欧几里得除法 (*代数*, 章 IV, § 1, no. 5) 表明存在两个多项式 $Q', Q''$，使得 $Q'_1 = PQ'' + Q'$ 其中 $\deg(Q') < s$；然后我们推断
$$
T = PQ_1 + P'(PQ'' + Q') = PQ + P'Q'
$$
其中$Q = Q_1 + P'Q''$。要显示公式 (1) 的唯一性，只需证明关系
$$
0 = PQ + P'Q', \quad \deg(Q') < s
$$
暗示$Q = Q' = 0$。现在，如果 (2) 成立，则 $P$ 除 $-PQ = P'Q'$ 并且，如 $P$ 和

P' 强互质，P 除 Q' by 引理 1；如果 Q' ≠ 0，则存在多项式 S ≠ 0，使得 Q' = PS, 从而

$$
\deg(Q') = s + \deg(S) \geq s,
$$

这是一个矛盾。我们在开始时结论 Q' = 0，从而 PQ = 0，最后通过注 Q = 0。

最后，假设$\deg(T) \leq t$和$\deg(P') \leq t - s$；与形式 (1) 中的多项式 T，

$$
\deg(P'Q') \leq \deg(P') + \deg(Q') < s + \deg(P') \leq t
$$

因此

$$
s + \deg(Q) = \deg(PQ) = \deg(T - P'Q') \leq t
$$

从而$\deg(Q) \leq t - s$。

#### 例 {#ac-iii-s4-n1-exa-1 .statement tag=04HU}

对于与 $X - a$（其中 $a \in \mathbf{A}$）强互质的多项式 $P \in \mathbf{A}[X]$，$P(a)$ 在 $\mathbf{A}$ 中“可逆”是充分必要的。因为如果 P 和 $X - a$ 强互质，则从命题 1 可知存在 $c \in \mathbf{A}$ 和多项式 $Q \in \mathbf{A}[X]$，使得 $cP + (X - a)Q = 1$、从而 $cP(a) = 1$ 和 $P(a)$ 可逆。相反，欧几里得除法

$$
P = (X - a)R + P(a)
$$

并且，如果$P(a) = b^{-1}$，其中$b \in \mathbf{A}$，我们推论出$1 = bP - b(X - a)R$，这表明P和$X - a$是强互质的。

令$\mathbf{A}$和$\mathbf{B}$是两个交换环和$f : \mathbf{A} \to \mathbf{B}$环同态。如果$P = \sum_{i \geq 0} a_i X^i$是$\mathbf{A}[[X]]$中的形式幂级数，则令$\bar{f}(P)$表示$\mathbf{B}[[X]]$中的形式幂级数$\sum_{i \geq 0} f(a_i) X^i$。如果 P 是多项式，则 $\bar{f}(P)$ 也是，如果进一步 P 是多项式，则 $\bar{f}(P)$ 是与 P 相同的次数的多项式。最后，$P \mapsto \bar{f}(P)$ 显然是 $\mathbf{A}[[X]]$ 到 $\mathbf{B}[[X]]$ 的同态，其中扩展 $f$以及映射 X 至 X。 *记号将在本段的其余部分中不断地使用这种意义。*

#### 命题 2 {#ac-iii-s4-prop-2 .statement tag=04HV}

*令$\mathbf{A}$和$\mathbf{B}$为从$\mathbf{A}$到$\mathbf{B}$的两个交换环、$f$同态以及$P, P'$$\mathbf{A}[X]$中的两个多项式。如果$P$和$P'$在$\mathbf{A}[X]$中强互质，则$\bar{f}(P)$和$\bar{f}(P')$在$\mathbf{B}[X]$中强互质。 逆命题为真，当且仅当是满射，如果它的核包含在 $\mathbf{A}$ 的 Jacobson 根式中并且 $P$ 是单调的。*

假设 P 和 P' 强互质；则$\mathbf{A}[X]$中存在多项式Q、Q'使得$PQ + P'Q' = 1$；我们推断

$$
\bar{f}(P)\bar{f}(Q) + \bar{f}(P')\bar{f}(Q') = 1,
$$

从而第一个断言。为了显示第二个，让 a 表示核或 $f$；

令$E = A[X]$和$F$为由$P$和$P'$生成的$E$的理想；由于 $f$ 是满射且 $\bar{f}(P)$ 单调，命题 1 表明对于每个多项式 $T \in A[X]$，$A[X]$ 中存在两个多项式 $Q, Q'$，使得
$$
\bar{f}(T) = \bar{f}(P) \bar{f}(Q) + \bar{f}(P') \bar{f}(Q'),
$$
从而关系$E = F + aE$。现在，$E/F$是一个有限生成的$A$模，因为每个多项式都是同余模。 $P$ 到次数 $< \deg(P)$ 的多项式，$P$ 是单调的。由于$E/F = a(E/F)$和$a$包含在$A$的雅各布森根中，中山的引理表明$E/F = 0$（代数，章VIII, § 6, no. 3，推论2到命题6），这意味着$P$ 和 $P'$ 强互质。

### 2. 限制正式幂级数

#### 定义 1 {#ac-iii-s4-def-1 .statement tag=04HW}

如果存在理想 $\mathfrak{o} \subset A$ 的邻域 $\mathfrak{o}$ 由……组成的基本系统 $\mathscr{B}$，则可交换拓扑环 $A$ 被称为线性拓扑（并且其拓扑被称为线性）。

注在这样的环中，理想$3 \in \mathscr{B}$是开放和封闭的（一般拓扑，章111，§ 2, no. 1，命题4的推论）。对于所有 $3 \in \mathscr{B}$，商拓扑环 $A/\mathfrak{J}$ 是离散的；对于$8 \in \mathscr{B}$，$8' \in \mathscr{B}$，$\mathfrak{J}' \subset 8$，令
$$
h_{\mathfrak{J}\mathfrak{J}'} : A/\mathfrak{J}' \to A/\mathfrak{J}
$$
为典范映射。我们知道（一般拓扑，章III, § 7, no. 3）$(A/\mathfrak{J}, h_{\mathfrak{J}\mathfrak{J}'})$是离散环的逆系（相对于按$\supset$排序并有向的索引集合$\mathscr{B}$），其逆极限是一个完整的逆极限 Hausdorff 线性拓扑环 $\tilde{A}$；进一步（loc. cit.，命题 2），定义了严格的态射$i : A \to \tilde{A}$，其核是$A$中$\{0\}$的闭包，并且其像在$\tilde{A}$中处处稠密，因此$\tilde{A}$是规范地认定为 $A$ 的 Hausdorff 完备的。

#### 定义 2 {#ac-iii-s4-def-2 .statement tag=04HX}

Given a commutative topological ring $A$, a formal power series
$$
T = \sum_{(n_i)} c_{n_1 n_2 \ldots n_p} X_1^{n_1} X_2^{n_2} \ldots X_p^{n_p}
$$
in the ring $A[[X_1, \ldots, X_p]]$ is called restricted if, for every neighbourhood $V$ of 0 in $A$, there is only a finite number of coefficients $c_{n_1 n_2 \ldots n_p}$ not belonging to $V$ (in other words, the family $(c_{n_1 n_2 \ldots n_p})$ tends to 0 in $A$ with respect to the filter of complements of finite subsets of $\mathbf{N}^p$).

If $A$ is linearly topologized, the restricted formal power series in $A[[X_1, \ldots, X_p]]$ form a subring of $A[[X_1, \ldots, X_p]]$, denoted by $A\{X_1, \ldots, X_p\}$: for if
$$
T = \sum_{(n_i)} c_{n_1 \ldots n_p} X_1^{n_1} \ldots X_p^{n_p}, \quad T' = \sum_{(n_i)} c'_{n_1 \ldots n_p} X_1^{n_1} \ldots X_p^{n_p}
$$
are two restricted formal power series and $\mathfrak{J}$ a neighbourhood of 0 in $A$ which is an ideal of $A$, there exists an integer $m$ such that $c_{n_1 \ldots n_p} \in \mathfrak{z}$ and $c'_{n_1 \ldots n_p} \in \mathfrak{g}$ for every system $(n_1, \ldots, n_p)$ such that $n_k \geq m$ for at least one index $k$; now, if

$$
T'' = TT' = \sum_{(n_i)} c''_{n_1 \ldots n_p} X_1^{n_1} \ldots X_p^{n_p},
$$

那么$c''_{n_1 \ldots n_p} = \sum c_{r_1 \ldots r_p} c'_{s_1 \ldots s_p}$对于所有系统$(r_k), (s_k)$使得$r_k + s_k = n_k$对于$1 \leq k \leq p$；我们结论，如果$n_k \geq 2m$，则$r_k \geq m$或$s_k \geq m$，因此，由于$\mathfrak{z}$是一个理想，$c''_{n_1 \ldots n_p} \in \mathfrak{g}$只要$n_k \geq 2m$至少有一个$k$，这就建立了我们的断言。此外，受限制形式幂级数的每个导数$\partial T / \partial X_i$（$1 \leq i \leq p$）都是受限制的，紧随定义以及邻域$\mathfrak{z} \in \mathscr{B}$是$\mathbf{A}$的加性子群这一事实。

如果$\mathbf{A}$是离散的，则受限形式幂级数的环就是多项式环$\mathbf{A}[X_1, \ldots, X_n]$。

让我们始终假设$\mathbf{A}$是线性拓扑的，并让$\mathscr{B}$是$\mathbf{A}$理想的$\mathbf{A}$由……组成中0的邻域的基本系统；对于所有$\mathfrak{g} \in \mathscr{B}$，令$p_\mathfrak{g}: \mathbf{A} \to \mathbf{A}/\mathfrak{g}$为典范同态。到定义，对于每个受限正式幂级数$T \in \mathbf{A}\{X_1, \ldots, X_n\}$，

$$
\bar{p}_\mathfrak{g}(T) \in (\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_p].
$$

显然

$$
((\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_p], \bar{h}_{\mathfrak{g}\mathfrak{g}'})
$$

是环的逆系（相对于有向索引集合$\mathscr{B}$），$(\bar{p}_\mathfrak{g})$是同态$\mathbf{A}\{X_1, \ldots, X_n\} \to (\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_p]$的逆系；由于每个多项式都是受限形式幂级数，因此 $\bar{p}_\mathfrak{g}$ 是满射；它的核$N_\mathfrak{g}$是限制形式幂级数的$\mathbf{A}\{X_1, \ldots, X_n\}$由……组成的理想，其所有系数都为属于到$\mathfrak{g}$；我们将给$\mathbf{A}\{X_1, \ldots, X_n\}$（线性）拓扑，其中$N_\mathfrak{g}$（对于$\mathfrak{g} \in \mathscr{B}$）形式，邻域的基本系统为0（拓扑显然仅取决于$\mathbf{A}$）。然后由一般拓扑、章III, § 7, no. 3、命题2得出

$$
\pi = \lim_{\leftarrow} \bar{p}_\mathfrak{g}: \mathbf{A}\{X_1, \ldots, X_n\} \to \lim_{\rightarrow} (\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_p]
$$

是一个严格的态射，其核是$\mathbf{A}\{X_1, \ldots, X_n\}$中$\{0\}$的闭包，并且其像密集于

$$
\mathbf{A}' = \lim_{\rightarrow} (\mathbf{A}/\mathfrak{g})[X_1, \ldots, X_n].
$$

#### 命题 3 {#ac-iii-s4-prop-3 .statement tag=04HY}

*如果线性拓扑交换环$\mathbf{A}$是Hausdorff且完备，则典范同态$\pi$是拓扑环同构。*

对于所有$(n_1, \ldots, n) \in \mathbf{N}^p$和所有$3 \in \mathscr{B}$，令$\phi_{n_1 \ldots n_p}^3$为映射$(A/\mathfrak{J})[X_1, \ldots, X_p] \to A/\mathfrak{J}$，其中映射每个多项式除以该多项式中$X_1^{n_1} \ldots X_p^{n_p}$的系数；显然，$(A/\mathfrak{J})$-模块同态的$\phi_{n_1 \ldots n_p}^3$形式逆系（相对于有序集合$\mathscr{B}$），并且，由于$A$通过假设与$\lim_{\leftarrow} (A/\mathfrak{J})$规范地标识， $\phi_{n_1 \ldots n_p} = \lim_{\leftarrow} \phi_{n_1 \ldots n_p}^3$是从$A'$到$A$的连续$A$同态。对于$A'$的每一个元素$S = (S_\mathfrak{J})_{\mathfrak{J} \in \mathscr{B}}$，我们将看到形式的幂级数$T = \sum_{(n_i)} \phi_{n_1 \ldots n_p}(S) X_1^{n_1} \ldots X_p^{n_p}$受到限制并满足$\pi(T) = S$。对于所有$3 \in \mathscr{B}$和所有$\mathfrak{J}' \in \mathscr{B}$，使得$\mathfrak{J}' \subset \mathfrak{J}$，关系$\phi_{n_1 \ldots n_p}^{\mathfrak{J}'}(S_{\mathfrak{J}'}) = 0$意味着
$$
\phi_{n_1 \ldots n_p}^{\mathfrak{J}'}(S_{\mathfrak{J}'}) \in \mathfrak{J}/\mathfrak{J}'
$$
由于$S_{\mathfrak{J}}$是一个多项式，我们看到$\phi_{n_1 \ldots n_p}(S) \in \mathfrak{J}$除了那些$(n_1, \ldots, n_p)$之外，在数中有限，这样$\phi_{n_1 \ldots n_p}^{\mathfrak{J}}(S_{\mathfrak{J}}) \neq 0$，这证明了我们的第一个断言；第二个来自定义。由于$A$是Hausdorff，$\mathbf{N}_\mathfrak{J}$约化的交为0，因此$\pi$是*双射的*，它完成证明，因为$\pi$是严格的态射。

#### 命题 4 {#ac-iii-s4-prop-4 .statement tag=04HZ}

*令$A, B$为两个线性拓扑交换环，$B$为Hausdorff且完备，$u : A \to B$为连续的同态。对于$B$的元素的每个家庭$b = (b_i)_{1 \leq i \leq p}$，都存在唯一的连续同态*
$$
\tilde{u} : A\{X_1, \ldots, X_p\} \to B
$$
*使得$\tilde{u}(a) = u(a)$代表所有$a \in A$，$\tilde{u}(X_i) = b_i$代表$1 \leq i \leq p$。*

存在唯一同态$v : A[X_1, \ldots, X_p] \to B$，使得$v(a) = u(a)$对应$a \in A$，$v(X_i) = b_i$对应$1 \leq i \leq p$。此外，如果$\mathfrak{J}$是理想的$B$中0的邻域，则$\overline{u}^{-1}(\mathfrak{J}) = 3$是$A$的理想，即邻域为0，并且对于每个多项式$P \in \mathbf{N}_\mathfrak{J}$，显然$v(P) \in \mathfrak{J}$，因此$v$是连续的。由于$A[X_1, \ldots, X_p]$在$A\{X_1, \ldots, X_p\}$中稠密，$\tilde{u}$的存在和唯一性遵循扩张的*一般拓扑*、章111、§ 3, no. 3、命题5和原理身份。

在$A = B$和$u$为恒等映射的特殊情况下，对于每个受限形式幂级数$f \in A\{X_1, \ldots, X_p\}$，我们将为$\tilde{u}(f)$的值写为$f(b_1, \ldots, b_p)$或$f(b)$。

*注*

#### 注 1 {#ac-iii-s4-n2-rem-1 .statement tag=04I0}

命题 4 证明，对于环 $A$ 中的每个“封闭”理想 $a$（假定为 Hausdorff 且完备），$1 \leq i \leq p$ 的关系 $b_i \in a$ 意味着$f(b_1, \ldots, b_p) \in a$ 对于每个受限形式幂级数 $f \in A\{X_1, \ldots, X_p\}$。

#### 注 2 {#ac-iii-s4-n2-rem-2 .statement tag=04I1}

假设$A$是线性拓扑的；令 $r$ 为整数，使得 1 $\leq r \leq p$ 且令环 $A\{X_1, \ldots, X_r\}$ 为上面定义的拓扑。然后拓扑环 $A\{X_1, \ldots, X_r\}$ 与受限形式幂级数的环等价

$$
(A\{X_1, \ldots, X_r\})\{X_{r+1}, \ldots, X_p\}
$$

从定义开始如下。

#### 注 3 {#ac-iii-s4-n2-rem-3 .statement tag=04I2}

有了*注 2*的记号，进一步假设$A$是Hausdorff且完备，让我们在形式中写出每个受限形式幂级数$f \in A\{X_1, \ldots, X_r\}$

$$
f = \sum_{(n_i)} c_{n_{r+1} \ldots n_p}(X_1, \ldots, X_r) X_{r+1}^{n_{r+1}} \ldots X_p^{n_p}
$$

其中 $c_{n_{r+1} \ldots n_p}$ 是受限形式幂级数。对于$A$的元素的每个系统$x = (x_1, \ldots, x_r)$，让

$$
b_{n_{r+1} \ldots n_p} = c_{n_{r+1} \ldots n_p}(x_1, \ldots, x_p).
$$

紧接着*注 1*，$\sum_{(n_i)} b_{n_{r+1} \ldots n_p} X_{r+1}^{n_{r+1}} \ldots X_p^{n_p}$ 是一个*受限*正式的幂级数，用$f(x_1, \ldots, x_r, X_{r+1}, \ldots, X_p)$ 表示；据说它是通过在$f$中*替换*$x_i$为$X_i$为$1 \leq i \leq r$而获得的。

### 3.亨塞尔引理

在拓扑环 $A$ 中，如果 $O$ 是序列 $(x^n)_{n \geq 0}$ 的极限，则元素 $x$ 被称为“拓扑幂零”。 If $A$ is a *linearly topologized* commutative ring, to say that $x$ is topologically nilpotent means that for every open ideal $\mathfrak{J}$ of $A$ the canonical image of $x$ in $A/\mathfrak{J}$ is a *nilpotent* element of that ring. 如果$\mathfrak{r}_g$是$A/\mathfrak{J}$的零根，则显然$(\mathfrak{r}_g)$是子集的逆系并且$A$的拓扑幂零元的集合$t$是$\mathfrak{r} = \lim \mathfrak{r}_g$的逆像典范同态$A \to \lim A/\mathfrak{J}$；因此它是$A$的“封闭理想”。 如果 $A$ 也是 *Hausdorff* 和 *完全*，则该理想包含在 $A$ 的 Jacobson 根式中，并且，对于元素 $x \in A$ 可逆，其类 mod 是充分必要的。 $t$ 在 $A/t$ (§ 2, no. 13, 引理 3) 中可逆。

注，如果$A$是环且$m$是$A$的双面理想，$m$的元素相对于*m-adic*拓扑在拓扑上是幂零的。

**定理 1（亨塞尔）**。令 $A$ 为完全豪斯多夫线性拓扑交换环。令$m$为$A$的封闭理想，其元素拓扑幂零。令$B = A/m$为拓扑环与$\varphi : A \to B$典范映射的商。令$R$为$A\{X\}$中的限制形式幂级数，$\overline{P}$为$B[X]$中的一元多项式，$\overline{Q}$为$B\{X\}$中的限制形式幂级数。假设$\overline{\varphi}(R) = \overline{P} \cdot \overline{Q}$、$\overline{P}$和$\overline{Q}$在$B\{X\}$中强互质。那么存在一个单调多项式 $P \in A[X]$ 的唯一有序对 $(P, Q)$ 由……组成和一个受限形式幂级数 $Q \in A\{X\}$ 使得
(4)
$$
R = P.Q, \quad \bar{\varphi}(P) = P, \quad \bar{\varphi}(Q) = \overline{Q}.
$$
此外，$P$和$Q$在$A\{X\}$中是强互质的，并且如果$R$是多项式，$Q$也是多项式。

证明分为四步。在前三个中，我们假设 $A$ 是离散的，在这种情况下 $R$ 和 $\overline{Q}$ 是多项式。

(I)$m^2 = 0$
令 $S, T$ 为 $A[X]$ 的两个多项式，使得 $S$ 为单调且$\bar{\varphi}(S) = \overline{P}$、$\bar{\varphi}(T) = \overline{Q}$； no. 1的命题2表明$S$和$T$强互质；因此 (no. 1, 命题 1) 存在$A[X]$多项式$(S', T')$的唯一有序对，使得
(5)
$$
R - ST = ST' + TS' \quad \text{and} \quad \deg(S') < \deg(S) = \deg(\overline{P}).
$$
多项式$P = S + TS'$、$Q = T + T'$则为解至问题；那么事实上
(6)
$$
\overline{P} \cdot \bar{\varphi}(T') + \overline{Q} \cdot \bar{\varphi}(S') = \bar{\varphi}(ST' + TS') = \bar{\varphi}(R - ST) = 0.
$$
由于 $\overline{P}$ 是单调的，$\overline{P}$ 和 $\overline{Q}$ 强互质且
$$
\deg(\bar{\varphi}(S')) < \deg(\overline{P}),
$$
no. 1的命题 1表明$\bar{\varphi}(S') = \bar{\varphi}(T') = 0$，在其他字中，$S'$和$T'$属于到$m$和关系$m^2 = 0$的系数给出
$$
PQ = ST + ST' + TS' = R,
$$
满足关系 (4)。由于$\bar{\varphi}(P) = \overline{P}$和$\bar{\varphi}(Q) = \overline{Q}$，$P$和$Q$强互质（no. 1，命题2）；最后，如果 $P_1$ 和 $Q_1$ 是 $A[X]$ 满足 (4) 中的另外两个多项式，并且 $P_1$ 是单调的，那么必然有设定 $S'_1 = P_1 - S, \ T'_1 = Q_1 - T, \ \deg(S'_1) < \deg(S)$ 和 $R - ST = ST'_1 + TS'_1$，因为 $S'_1$ 和$T'_1$ 的系数在 $m$ 中；但命题 1 然后证明$S' = S'_1$ 和$T' = T'_1$，从而证明有序对 $(P, Q)$ 的唯一性。

(2) $m$ 幂零的
令$n$为最小的整数，使得$m^n = 0$，让我们通过归纳对$n > 2$进行论证，定理已被证明为$n = 2$。设$A = A/m^{n-1}$，$m' = m/m^{n-1}$；如${m'}^{n-1} = 0$，$A'[X]$中存在唯一的多项式有序对$(P', Q')$，使得$P'$是单调的，$R' = P'Q'$、$\psi(P') = \overline{P}$和$\psi(Q') = \overline{Q}$，其中$\psi$表示典范同态 $A' \to A'/m' = B$、$\theta$、典范同态、$A \to A'$ 和 $R' = \tilde{\theta}(R)$。另一方面，如$(m^{n-1})^2 = 0$，$A[X]$中存在唯一的多项式有序对$(P, Q)$，使得$P$是单次的且$R = PQ$、$\bar{\theta}(P) = \overline{P}$、$\bar{\theta}(Q) = \overline{Q}$；作为$\phi = \psi \circ \theta$，这表明$P$和$Q$满足的存在和唯一性 (4)；此外，$P'$和$Q'$与归纳假设强互质，因此$P$和$Q$也是如此。

(3) **是离散的**

注在这种情况下$m$不再一定是幂零的，但它始终是假设的*nilideal*。 令$P_0$、$Q_0$为$A[X]$的两个多项式，使得$\bar{\varphi}(P_0) = \overline{P}$、$\bar{\varphi}(Q_0) = \overline{Q}$和$P_0$是单调的。 让我们考虑由$R - P_0 Q_0$的系数生成的$A$的理想$n$；它是有限生成的并包含在$m$中，因此它是*幂零*（章11，§ 2, no. 6，命题15）和定义，如果$\psi : A \to A/n$是典范映射，那么$\bar{\psi}(R) = \bar{\psi}(P_0) \bar{\psi}(Q_0)$。 此外，$\bar{\psi}(P_0)$和$\bar{\psi}(Q_0)$是强互质，如下从$\overline{P}$上的假设和$\overline{Q}$以及no. 1的命题2应用于典范同态$A/n \to A/m$。 根据情况(2)，$A[X]$中存在有序对$(P, Q)$多项式，使得$P$是单调的并且关系(4)成立。 $\overline{P}$ 和 $\overline{Q}$ 强互质的事实也意味着，$P$ 和 $Q$ 在 $A[X]$ 中凭借 no. 1、命题 2 强互质，因为 $m$ 包含在 $A$ 的雅各布森根式中。 最后假设$P_1$、$Q_1$是$A[X]$满足(4)中的两个多项式，且$P_1$是单调的，令$n_1$是由$P - P_1$的系数和$Q - Q_1$的系数生成的$A$的有限生成理想；由于$n_1$包含在$m$中，因此它是幂零的，并且如果$\psi_1 : A \to A/n_1$是典范映射，则$\bar{\psi}_1(P) = \bar{\psi}_1(P_1)$和
$$
\bar{\psi}_1(Q) = \bar{\psi}_1(Q_1);
$$
因此，对于情况 (2)，唯一性性质意味着$P = P_1,\ Q = Q_1$。

(4) **一般情况**

设$\mathscr{B}$为$A$理想的$A$由……组成中0的邻域的基本系统。对于所有$\mathfrak{s} \in \mathscr{B}$，令$f_{\mathfrak{s}}$为典范映射$A \to A/\mathfrak{s}$，$\phi_{\mathfrak{s}}$典范映射
$$
A/\mathfrak{s} \mapsto (A/\mathfrak{s})/((m + \mathfrak{s})/\mathfrak{s}) = A/(m + \mathfrak{s}),
$$
$g_{\mathfrak{s}}$典范映射$B = A/m \to A(m + \mathfrak{s})$并写$R_{\mathfrak{s}} = f_{\mathfrak{s}}(R)$、$P_{\mathfrak{s}} = g_{\mathfrak{s}}(\overline{P})$、$\overline{Q}_{\mathfrak{s}} = g_{\mathfrak{s}}(\overline{Q})$。由于每个环$A/\mathfrak{s}$都是离散的，因此可以将情况（3）应用于它，我们看到$(A/\mathfrak{s})[X]$中存在唯一的多项式有序对$(P_{\mathfrak{s}}, Q_{\mathfrak{s}})$，使得$P_{\mathfrak{s}}$是单调的并且$R_{\mathfrak{s}} = P_{\mathfrak{s}} Q_{\mathfrak{s}}$，$\bar{\varphi}_{\mathfrak{s}}(P_{\mathfrak{s}}) = \overline{P}_{\mathfrak{s}}$， $\bar{\varphi}_{\mathfrak{s}}(Q_{\mathfrak{s}}) = \overline{Q}_{\mathfrak{s}}$。这个有序对的唯一性意味着，如果$\mathfrak{s}' \subset \mathfrak{s}$，$\mathfrak{s}' \in \mathscr{B}$和$f_{\mathfrak{s}'\mathfrak{s}} : A/\mathfrak{s}' \to A/\mathfrak{s}$是典范映射，那么$P_{\mathfrak{s}} = f_{\mathfrak{s}'\mathfrak{s}}(P_{\mathfrak{s}'})$，$Q_{\mathfrak{s}} = f_{\mathfrak{s}'\mathfrak{s}}(Q_{\mathfrak{s}'})$。然后根据$A[X]$与$\lim(A/\mathfrak{s})[X]$（no. 2，命题3）的规范标识，存在$P \in A\{X\}$和$Q \in A\{X\}$，使得对于所有$s \in \mathscr{B}$都存在$R = PQ$和$\bar{f}_s(P) = P_s, \bar{f}_s(Q) = Q_s$。而且，
$$
\bar{g}_s(\overline{P} - \overline{\varphi}(P)) = 0, \quad \bar{g}_s(\overline{Q} - \overline{\varphi}(Q)) = 0
$$
对于所有$s \in \mathscr{B}$，这意味着对于所有$\mathfrak{J} \in \mathscr{B}$，$\overline{P} - \overline{\varphi}(P)$和$\overline{Q} - \overline{\varphi}(Q)$的系数都是属于到$(m + \mathfrak{J})/m$。但是，由于$m$在$A$、$\bigcap_s (m + s) = m$、从而、$\overline{P} = \overline{\varphi}(P), \overline{Q} = \overline{\varphi}(Q)$、$P$和$Q$关闭，那么当然满足 (4)；此外，由于 $P_s$ 是单调多项式且具有相同的次数，因此受限形式幂级数 $P$ 是单调多项式。如果 $(P', Q')$ 是另一个有序对满足 (4) 并且 $P'$ 是一个单调多项式，我们将推导出 $R_s = \bar{f}_s(P') \bar{f}_s(Q'), \bar{\varphi}_s(\bar{f}_s(P')) = \overline{P}_s$ 和 $\bar{\varphi}_s(\bar{f}_s(Q')) = \overline{Q}_s$ 以及在情况 (3) $\bar{f}_s(P') = P_s, \bar{f}_s(Q') = Q_s$ 中的唯一性对于所有$s \in \mathscr{B}$，这意味着$P = P'$和$Q = Q'$。最后让我们证明$P$和$Q$是强互质的；根据情况 (3) 和 no. 1 的命题 1，对于所有 $s \in \mathscr{B}$，$(A/\mathfrak{J})[X]$ 中存在唯一的多项式有序对 $(S_s, T_s)$，使得
$$
1 = P_s S_s + Q_s T_s \quad \text{and} \quad \deg(T_s) < \deg(P_s) = \deg(\overline{P}).
$$
这个有序对的唯一性立即表明，对于$3' \in \mathscr{B}$，$\mathfrak{J}' \subset \mathfrak{J}, S_{3'} = \bar{f}_{33'}(S_{3}), T_{3'} = \bar{f}_{33'}(T_{3});$考虑到no. 2，命题3，我们结论存在两个受限形式幂级数$S, T$ $A\{X\}$使得$S_s = \bar{f}_s(S), T_s = \bar{f}_s(T)$和$1 = PS + QT$。

仍有待验证的是，如果 $R$ 是多项式，$Q$ 也是多项式。现在，$Q_s$是构造的多项式，并且由于$P_s$是单调的，关系$R_s = P_s Q_s$意味着
$$
\deg(Q_s) \leq \deg(R_s) \leq \deg(R)
$$
对于所有$s \in \mathscr{B}$； 从而立即通过$Q$的定义得到所需的结果。

### 4. 合成系统正式幂级数

设$A$为交换环；我们会说系统
$$
\mathbf{f} = (f_1, \ldots, f_p) \in (A[[X_1, \ldots, X_q]])^p
$$
$X_j$ ($1 \leq j \leq q$) 中的形式幂级数，其系数在 $A$ 中，*没有常数项*，如果对于所有 $f_j$ 都是如此。对于正式幂级数的每系统 (8) 和每系统
$$
\mathbf{g} = (g_1, \ldots, g_q) \in (A[[X_1, \ldots, X_r]])^q
$$
$q$正式幂级数没有常数项，我们将用$\mathbf{f} \circ \mathbf{g}$（或$\mathbf{f}(\mathbf{g})$）系统表示正式幂级数$f_j(g_1, \ldots, g_q)$（$1 \leq j \leq p$）
$$
(A[[X_1, \ldots, X_r]])^p
$$

（代数、章IV, § 5, no. 5）。如果
$$
\mathbf{h} = (h_1, \ldots, h_r) \in (\mathbf{A}[[X_1, \ldots, X_s]])^r
$$
是没有常数项的第三个系统，那么
$$(10)$$
$$(f \circ g) \circ h = f \circ (g \circ h).$$

对于每个整数 $m$，
$$(f^{(m)} \circ g^{(m)}) \circ h^{(m)} = f^{(m)} \circ (g^{(m)} \circ h^{(m)})$$
其中$f^{(m)}, g^{(m)}, h^{(m)}$表示形式幂级数$f, g, h$的系统中总次数$\leq m$的项多项式由……组成的系统。 但显然，$(f \circ g) \circ h$（或$f \circ (g \circ h)$）的级数中的总次数$\leq m$中的项与$(f^{(m)} \circ g^{(m)}) \circ h^{(m)}$（或$f^{(m)} \circ (g^{(m)} \circ h^{(m)})$）、从而和断言中的相同。

对于每个系统（8），我们将用$M_f$或$M_f(\mathbf{X})$表示雅可比行列式矩阵$(\partial f_i / \partial X_j)$（$1 \leq i \leq p, 1 \leq j \leq q$），其中$i$是指标的行，$j$是列的行；对于两个系统 (8) 和 (9)，其中 $g$ 没有常数项，
$$(11)$$
$$M_{f \circ g} = (M_f(g)). M_g$$
其中$M_f(g)$是矩阵，其中元素是通过将$M_f$的每个级数、元素中的$g$替换$\mathbf{X}$、($1 \leq j \leq q$)得到；这个公式只是代数、章IV, § 5, no. 8的公式(9)的重新表述。我们用$M_f$的元素的常数项的$M_f(0)$矩阵来表示；然后我们从 (11) 推出
$$(12)$$
$$M_{f \circ g}(0) = M_f(0). M_g(0).$$

给定整数 $n > 0$，我们将写
$$(13)$$
$$\mathbf{1}_n = \mathbf{X} = (X_1, \ldots, X_n) \in (\mathbf{A}[[X_1, \ldots, X_n]])^n,$$
这将被视为带有单个列的矩阵。

对于每个系统$\mathbf{f} = (f_1, \ldots, f_n) \in (\mathbf{A}[[X_1, \ldots, X_n]])^n$，$M_f$是阶$n$的平方矩阵；我们用$J_f$或$J_f(\mathbf{X})$表示它的行列式，用$J_f(0)$表示$J_f$的常数项，等于$\det(M_f(0))$；如果$\mathbf{g} = (g_1, \ldots, g_n)$是系统，而$(\mathbf{A}[[X_1, \ldots, X_n]])^n$中没有常数项，那么，由（11）和（12），
$$(14)$$
$$J_{f \circ g} = J_f(g) \cdot J_g$$
$$(15)$$
$$J_{f \circ g}(0) = J_f(g) J_g(0).$$

#### 命题 5 {#ac-iii-s4-prop-5 .statement tag=04I3}

*设$\mathbf{A}$为交换环且$\mathbf{f} = (f_1, \ldots, f_n)$系统，$\mathbf{A}[[X_1, \ldots, X_n]]$中没有$n$级数的常数项。假设$J_f(0)$在$\mathbf{A}$中可逆。那么$\mathbf{A}[[X_1, \ldots, X_n]]$中存在系统，没有$n$级数的常数项$\mathbf{g} = (g_1, \ldots, g_n)$，使得*
$$(16)$$
$$f \circ g = \mathbf{1}_n.$$

这个系统是独一无二的

(17)$g \circ f = 1_1$。

$g$的存在性和唯一性源自代数、章IV, § 5, no. 9、命题10，应用于$n$形式幂级数

$$
f_i(Y_1, \ldots, Y_n) - X_i \quad (1 \leq i \leq n).
$$

从 (15) 和 (16) 可知 $J_f(0)J_g(0) = 1$ 以及$J_g(0)$ 也是可逆的。我们结论存在$n$级数的系统$h = (h_1, \ldots, h_n)$，而$A[[X_1, \ldots, X_n]]$中没有常数项，使得$g \circ h = 1_1$；由此关系和 (16) 可以得出结论，借助 (10)，

$$
h = 1_n \circ h = (f \circ g) \circ h = f \circ (g \circ h) = f \circ 1_n = f.
$$

命题 5 和公式 (10) 和 (15) 表明，在合成 $(f, g) \mapsto f \circ g$ 集合系统 $f = (f_1, \ldots, f_n)$ $n$ 级数的律下，没有常数项时$A[[X_1, \ldots, X_n]]$，其中$J_f(0)$在$A$中可逆，是群。

### 5.完整方程的系统环

简而言之，如果环是可交换的、线性拓扑的、豪斯多夫且完备的，那么环满足*Hensel的条件*；给定这样的环中的理想$m$，$m$（或有序对$(A, m)$）将被称为满足*Hensel的条件*，如果$m$在$A$中封闭并且其元素在拓扑上是封闭的幂零。所有拓扑幂零元的$A$由……组成的理想$t$满足Hensel的条件（no. 3）。

特别是，如果$A$是交换环并且$m$$A$和$A$的理想是Hausdorff并且关于*m-adic*拓扑完整，有序对$(A, m)$满足Hensel的条件。

#### 命题 6 {#ac-iii-s4-prop-6 .statement tag=04I4}

*令$A$为交换环，$B$环满足亨塞尔的条件和$u : A \to B$同态。对于$B$的拓扑幂零元的每个族$x = (x_1, \ldots, x_n)$，存在从$A[[X_1, \ldots, X_n]]$到$B$的唯一同态$\tilde{u}$，使得$\tilde{u}(a) = u(a)$对于所有$a \in A$和$\tilde{u}(X_i) = x_i$对于$1 \leq i \leq n$。此外，如果 $m$ 表示级数的理想，而 $A[[X_1, \ldots, X_n]]$ 中没有常数项，则 $\tilde{u}$ 对于 m 进数拓扑是连续的。*

令 $a$ 为$x_i$ ($1 \leq i \leq n$) 在$B$ 中生成的有限生成理想；对于$B$的每个开放理想$\mathfrak{H}$，$B/\mathfrak{H}$中$x_i$的像都是幂零的，因此理想$(a + \mathfrak{H})/\mathfrak{H}$在$B/\mathfrak{H}$中是幂零的，并且存在整数$k$，使得对于$\sum_{i=1}^n p_i \geq k$， $x_1^{p_1} \cdots x_n^{p_n} \in \mathfrak{H}$。由于$m^k$的每个元素都是形式$X_1^{p_1} \cdots X_n^{p_n} g(X_1, \ldots, X_n)$的形式幂级数的有限和，其中$\sum_{i=1}^n p_i \geq k$，可以看出，如果$\tilde{u}$解问题，则$\tilde{u}(m^k) \subset \mathfrak{H}$，证明了$\tilde{u}$的连续性。显然存在唯一同态

$$
\nu : A[X_1, \ldots, X_n] \to B
$$

这样对于$a \in A$有$\nu(a) = u(a)$，对于$1 \leq i \leq n$有$\nu(X_i) = x_i$，上述论证表明$\nu$相对于由m进数拓扑在$A[X_1, \ldots, X_n]$上诱导的拓扑是连续的。由于 $A[X_1, \ldots, X_r]$ 在 $A[[X_1, \ldots, X_r]]$ 中与 m 进数拓扑是稠密的，并且 B 是 Hausdorff 且完备，因此完成了存在性的证明和 $\tilde{u}$ 的唯一性。

注，这个命题再次给我们作为§ 2, no. 9的命题 11的特例（i）。

如果$A$本身是线性拓扑的，$\tilde{u}$的限制到$A\{X_1, \ldots, X_r\}$重合，其中同态源自no. 2的命题4中的$u$。 这直接源于以下事实：如果给定环拓扑，且邻域的基数系统为 0，则理想$m^k \cap N_3$（在 no. 2 的记号中，该拓扑是最小的，则$A[X_1, \ldots, X_r]$ 在 $A\{X_1, \ldots, X_r\}$ 中是稠密的） $A\{X_1, \ldots, X_r\}$ 上的上界或拓扑由$A[[X_1, \ldots, X_n]]$ 和拓扑上定义的 m 进数拓扑在no. 2 中定义）。

如果$B = A$和$u$是恒等映射，则对于每个正式的幂级数$f \in A[[X_1, \ldots, X_r]]$，我们将元素$\tilde{u}(f)$写为$f(x_1, \ldots, x_r)$或$f(x)$；对于$A[[X_1, \ldots, X_r]]$的形式幂级数的每一个系统$\mathbf{f} = (f_1, \ldots, f_r)$，令$\mathbf{f}(x)$表示$A^r$的元素$(f_1(x), \ldots, f_r(x))$，则据说是通过用$x_i$代替来获得$X_i$在$\mathbf{f}$。如果$n \leq m$且F是$A[[X_1, \ldots, X_m]]$的形式幂级数，则可以将F视为$X_{n+1}, \ldots, X_m$中的形式幂级数，系数在$A[[X_1, \ldots, X_n]]$中；让

$$
F(x_1, \ldots, x_n, X_{n+1}, \ldots, X_m)
$$

表示将F系数中的$x_i$替换为$X_i$而得到的$A[[X_{n+1}, \ldots, X_m]]$中的形式幂级数，替代$1 \leq i \leq n$。

让我们取$B$为形式幂级数$A[[X_1, \ldots, X_r]]$的环，并让$n$为$B$中级数的理想，没有常数项，因此$(B, n)$满足Hensel 的条件（$§ 2$，no. 6，命题 6 的推论）。 命题 6 可以通过将$x_i \in B$取为级数而无需常数项来应用；那么，对于每个级数$\mathbf{f} \in A[[X_1, \ldots, X_r]]$，$\tilde{u}(f)$只是在代数，章IV，$§ 5$，no. 5中定义的正式幂级数$f(x_1, \ldots, x_n)$。如果 $f$ 是多项式，并且在一般情况下从命题得出，通过指出 $f \mapsto f(x_1, \ldots, x_n)$ 相对于 m 进数拓扑在 $A[[X_1, \ldots, X_n]]$ 上连续，这是显而易见的。

#### 推论{#ac-iii-s4-n5-cor-1 .statement tag=04I5}

令$A$为环满足亨塞尔的条件和$x = (x_1, \ldots, x_n)$$A$的拓扑幂零元族。设$g = (g_1, \ldots, g_q)$为系统，没有$A[[X_1, \ldots, X_s]]$中级数的常数项和$A[[X_1, \ldots, X_q]]$中形式幂级数的$f = (f_1, \ldots, f_p)$系统。那么 $g(x) = (g_1(x), \ldots, g_q(x))$ 是 $A$ 的拓扑幂零元族，并且

$$
(f \circ g)(x) = f(g(x)).
$$

$g_i(x)$ 拓扑幂零的事实直接从命题 6 得出，并且在 $A$ 中拓扑幂零元的理想是封闭的。当$f_j$是多项式时，关系(18)是明显的；另一方面，如果 $m$ 和 $m'$ 是级数的理想值，且不存在常数项

$$
A[[X_1, \ldots, X_q]] \quad \text{and} \quad A[[X_1, \ldots, X_n]]
$$

分别，显然关系$f \in {m'}^k$意味着$f(g_1, \ldots, g_q) \in {m'}^k$。因此，如果根据上述注和命题 6 给 $A[[X_1, \ldots, X_q]]$ $m$-adic 拓扑，则 (18) 的两侧是 $f$ 到 $(A[[X_1, \ldots, X_q]])^p$ 的连续函数； 从而关系 (18)。

接下来，对于环$A$和$A$的理想$m$，我们将在$A^n$中用$m^{x^n}$乘积集合$\prod_{i=1}^n m$表示，其中$m_i = m$代表$1 \leq i \leq n$，以避免歧义。

#### 命题 7 {#ac-iii-s4-prop-7 .statement tag=04I6}

*Let $A$ be 环 and $m$ an ideal of $A$ such that 有序对 $(A, m)$ satisfies Hensel's 条件. Let $f = (f_1, \ldots, f_n)$ be 系统 without constant 项 of 级数 in $A[[X_1, \ldots, X_n]]$ such that $J_f(0)$ is invertible in $A$.那么，对于所有 $x \in m^{x^n}$、$f(x) \in m^{x^n}$ 和 $x \mapsto f(x)$，$m^{x^n}$ 的双射到其自身，逆双射为$x \mapsto g(x)$，其中 $g$ 由 no. 4 中的关系 (16) 给出。*

当盗窃是多项式时，$f(x) \in m^{x^n}$ 是显而易见的，并且在一般情况下从命题 6 开始，并且$m$ 在 $A$ 中闭合。 The other 断言 of 命题 are then 直接的推论 of (16), (17) and (18).

#### 推论 {#ac-iii-s4-n5-cor-2 .statement tag=04I7}

*Let $q$ be a closed ideal of $A$ contained in $m$. Then 关系 $x \equiv x' \pmod{q^{x^n}}$ is equivalent to $f(x) \equiv f(x') \pmod{q^{x^n}}$.*

对于每一个正式的幂级数$f \in A[[X_1, \ldots, X_n]]$，

$$
f(X_1, \ldots, X_n) - f(Y_1, \ldots, Y_n) = \sum_{i=1}^n (X_i - Y_i) h_i(X_1, \ldots, X_n, Y_1, \ldots, Y_n)
$$

where the $h_i$ 属于 to $A[[X_1, \ldots, X_n, Y_1, \ldots, Y_n]]$ (代数, 章 IV, § 5, no. 8, 命题 9); it follows immediately that 关系 $x \equiv x' \pmod{q^{x^n}}$ implies $f(x) \equiv f(x') \pmod{q^{x^n}}$. 逆命题 is obtained by 替换 $f$ by its "inverse" $g$.

#### 定理 2 {#ac-iii-s4-thm-2 .statement tag=04I8}

*Let $A$ be 环 and $m$ an ideal of $A$ such that 有序对 $(A, m)$ satisfies Hensel's 条件.令 $f = (f_1, \ldots, f_n)$ 为 $n$ 元素的系统

A\{X_1, \ldots, X_n\} 并设 $a \in A^n$；让我们写$J_t(a) = e$。 $A\{X_1, \ldots, X_n\}$ 中存在系统 $g = (g_1, \ldots, g_n)$ 限制形式幂级数且没有常数项，使得
（一）$M_g(0) = I$，（单位矩阵）。
(ii) 对于所有$x \in A^n$，
$$(19)$$
$$f(a + ex) = f(a) + M_t(a) \cdot eg(x).$$
(iii) 设$h = (h_1, \ldots, h_n)$为形式幂级数的系统，没有常数项（不一定受限制），使得$g \circ h = 1_n$（命题5）。对于所有$y \in m^{n \times n}$，
$$(20)$$
$$f(a + eh(y)) = f(a) + M_t(a) \cdot ey.$$
对于每一个正式的幂级数$f \in A[[X_1, \ldots, X_n]]$，
$$(21)$$
$$f(X + Y) = f(X) + M_f(X) \cdot Y + \sum_{1 \leq i < j \leq n} G_{ij}(X, Y)Y_i Y_j,$$
其中 $G_{ij}$ 是明确确定的正式幂级数
$$A[[X_1, \ldots, X_n, Y_1, \ldots, Y_n]].$$
Iff 是受限制的，$M_f$ 的元素和 $G_{ij}$ 也是受限制的，因为这些形式的幂级数是多项式 iff 是多项式，并且从它们的唯一性可以得出，对于 $A$ 的每个开理想 $\mathfrak{J}$，表示为$p_\mathfrak{J}: A \to A/\mathfrak{J}$典范映射、$p_\mathfrak{J}$下$G_{ij}$的像是$p_\mathfrak{J}(F)$中$Y_i Y_j$的系数，其中$F$是幂级数$f(X + Y)$的形式$A[[X_1, \ldots, X_n, Y_1, \ldots, Y_n]]$； 从而我们的断言。

既然这样，对每个系列$(1 \leq i \leq n)$写出公式(21)，我们就得到所有$x \in A^n$(no. 2，命题4)，
$$(22)$$
$$f(a + ex) = f(a) + M_t(a) \cdot ex + e^2 r(x)$$
其中$r = (r_1, \ldots, r_r)$是受限形式幂级数的系统，每个阶$\geq 2$的总和。由代数、章III, § 6, no. 5的公式(18)得出，存在平方矩阵$M' \in \mathbf{M}_n(A)$使得
$$(23)$$
$$M_t(a) \cdot M' = eI_n,$$
从而在 (22) 中使用这个
$$(24)$$
$$f(a + ex) = f(a) + M_t(a) \cdot ex + M_t(a) M' \cdot er(x).$$

写出$g = 1, + M' \cdot r$，我们看到$g$满足条件(i)和(ii)；那么替换$x$乘以$h(y)$就足以获得(iii)。

#### 推论 1 {#ac-iii-s4-thm-2-cor-1 .statement tag=04I9}

令$A$为环且$m$为$A$的理想，使得有序对$(A, m)$满足Hensel的条件。设$f \in A\{X\}$、$a \in A$并写出$e = f'(a)$。如果 $f(a) \equiv 0$ (mod. $e^2 m$)，则存在 $b \in A$ 使得 $f(b) = 0$ 和 $b \equiv a$ (mod. $em$)。如果 b' 是 $\mathbf{A}$ 的另一个元素，使得 $f(b') = 0$ 和 $b' \equiv a \pmod{\mathfrak{m}}$，则$e(b - b') = 0$。特别是，如果$e$不是$\mathbf{A}$中零的除子，则$b$是唯一的。

设$f(a) = e^2 c$，其中$c \in \mathfrak{m}$； 公式 (20) 对于 $n = 1$ 给出
$$
f(a + eh(y)) = e^2(c + y)
$$
因此取$y = -c$、$b = a + eh(-c)$就足够了。此外，如果$b = a + ex, b' = a + ex', x \in \mathfrak{m}, x' \in m, f(b) = f(b') = 0$，我们从（19）推导出$e^2(g(x) - g(x')) = 0$。作为$g(\mathbf{X}) - g(\mathbf{Y}) = (\mathbf{X} - \mathbf{Y})u(\mathbf{X}, \mathbf{Y})$，其中$u$受限制，以及$u(0, 0) = 1$、$g(x) - g(x') = (x - x')v$，其中$v \in \mathbf{A}$可逆，因为，由于$m$是封闭的，$v - 1 = u(x, x') - 1 \in \mathfrak{m}$和$m$包含在$\mathbf{A}$的雅各布森根中； 从而关系$e(b - b') = 0$。

#### 注 {#ac-iii-s4-n5-rem-1 .statement tag=04IA}

当 $e$ 在 $\mathbf{A}$ 中可逆时，该推论尤其适用；然后我们还可以从 Hensel 的定理推导出 $b$ 的存在性，因为 $(\mathbf{A}/\mathfrak{m})\{\mathbf{X}\}$ 中 $f(\mathbf{X})$ 的典范像是形式 $(\mathbf{X} - a)f_1(\mathbf{X}), \mathbf{X} - a$ 和 $f_1(\mathbf{X})$ 强互质，因为 $f_1(\alpha) = f'(\alpha)$ 是像共 $e$（no. 1、例）。

例
(1) 设$p$为素数数$\neq 2$和$n$整数，其类模。 $p$ 是平方 $\neq 0$ 位于素数域 $\mathbf{F}_p$ 中。如果$\mathbf{Z}_p$是$p$-adic整数（§ 2, no. 12，例3）的环，则将推论1应用到多项式$\mathbf{X}^2 - n$可知$n$在$\mathbf{Z}_p$中是平方；对于例 7 来说，$\mathbf{Z}_3$ 中的平方。
(2) 设$\mathbf{A} = \mathbf{K}[[\mathbf{Y}]]$为形式幂级数的环，其系数为交换域$\mathbf{K}$；与 $(\mathbf{Y})$-adic 拓扑、环 $\mathbf{A}$ 是 Hausdorff 且完整（§ 2, no. 6，命题 6 的推论）和映射 $f(\mathbf{Y}) \mapsto f(0)$ 定义由经过到将$\mathbf{A}/(\mathbf{Y})$的商环同构转移到域$\mathbf{K}$。由推论1，如果$F(\mathbf{Y}, \mathbf{X})$是$\mathbf{X}$中的多项式，系数在$\mathbf{A}$中，并且$a$是$\mathbf{K}$中$F(0, \mathbf{X})$的简单根，则存在唯一形式幂级数 $f(\mathbf{Y})$使得$f(0) = a$和$F(\mathbf{Y}, f(\mathbf{Y})) = 0$。

#### 推论 2 {#ac-iii-s4-thm-2-cor-2 .statement tag=04IB}

令$\mathbf{A}$为环且$\mathfrak{m}$为$\mathbf{A}$的理想，使得有序对$(\mathbf{A}, m)$满足Hensel的条件。令$r, n$为整数，使得$0 \leq r < n$和$\mathbf{f} = (f_{r+1}, \ldots, f_n)$为$n - r$的系统，$\mathbf{A}\{\mathbf{X}_1, \ldots, \mathbf{X}_n\}$的元素；让$J^{(n-r)}_{\mathbf{f}}(\mathbf{X})$表示指标$j$的$M_{\mathbf{f}}(\mathbf{X})$由……组成或列的小数，使得$r + 1 \leq j \leq n$。令$a \in \mathbf{A}^n$使得$J^{(n-r)}_{\mathbf{f}}(a)$在$\mathbf{A}$和$\mathbf{f}(a) \equiv 0 \pmod{\mathfrak{m}^{(n-r)}}$中可逆。那么存在唯一的$\mathbf{x} = (x_1, \ldots, x_n) \in \mathbf{A}^n$，使得$x_k = a_k$对应于$1 \leq k \leq r$、$\mathbf{x} \equiv a \pmod{\mathfrak{m}^n}$和$\mathbf{f}(\mathbf{x}) = 0$。

将$f_i$（no. 2，注 3）中的$a$、$X_k$替换为$1 \leq k \leq r$，我们立即发现我们可以将注意力限制在$r = 0$证明推论的情况。 定理 1 和命题 7 表明$a + \mathfrak{m}^n$ 的$\mathbf{f}$ 定义双射到$\mathbf{f}(a) + \mathfrak{m}^n = \mathfrak{m}^n$；推论源自$0 \in \mathfrak{m}^n$。

#### 推论 3 {#ac-iii-s4-thm-2-cor-3 .statement tag=04IC}

*有了记号和推论2，令$a \in \mathbf{A}^n$；让我们写 $e = J_r^{(n-r)}(\mathbf{a})$ （不一定在 $\mathbf{A}$ 中可逆）并假设 $f(\mathbf{a}) \equiv 0$ (mod. $e^{2m^{\times(n-r)}}$)。那么在 $\mathbf{A}[[X_1, \ldots, X_r]]$ 中存在没有常数项 $\phi_i$ ($r + 1 \leq i \leq n$) 的 $n - r$ 形式幂级数，这样，对于所有 $t = (t_1, \ldots, t_r) \in m^{\times r}$，

$$
f_i(a_1 + e^2 t_1, \ldots, a_r + e^2 t_r, a_{r+1} + e \phi_{r+1}(t), \ldots, a_n + e \phi_n(t)) = 0
$$

$r + 1 \leq i \leq n$。

*对于$1 \leq i \leq r$，设$f_i(X) = X_i - a$，并设$u = (f_1, \ldots, f_n)$；那么$J_u(a) = e$和定理2可以应用于系统$u$。对于定理 2 的记号，从上面的定义得出$g_i(X) = X$，对于$1 \leq i \leq r$，从而$h_i(X) = X_i$对于$1 \leq i \leq r$；此外，如果$M' \in \mathbf{M}_n(\mathbf{A})$使得$M_u(a) . M' = e I_n$，则$M'$等于形式

$$
\begin{pmatrix}
e I_r & 0 \\
* & *
\end{pmatrix}.
$$

替换$y$乘以$M'.z$（其中$z = (z_1, \ldots, z_n) \in m^{\times n}$）在公式（20）中，我们得到

$$
f_i(a_1 + e^2 z_1, \ldots, a_r + e^2 z_r, a_{r+1} + e h_{r+1}(M'.z), \ldots, a_n + e h_n(M'.z))
= \& (a) + e^2 z_i \quad \text{for } 1 \leq i \leq n.
$$

假设、$f_j(a) = e^2 b_j$，其中 $b_j \in m$ $r + 1 \leq j \leq n$。让我们写 $\psi_j(X_1, \ldots, X_r) = h_j(M'.X)$ 和

$$
\phi_j(X_1, \ldots, X_r) = \psi_j(X_1, \ldots, X_r, -b_{r+1}, \ldots, -b_n)
$$

$r + 1 \leq j \leq n$。对于$r + 1 \leq i \leq n$，在(26)中用$t_j$代替$z_j$代替$1 \leq j \leq r$，用$b_j$代替$z_j$代替$r + 1 \leq j \leq n$，我们得到所有$t \in m^{\times r}$的关系(25)。

### 6. 分解环的申请

#### 引理 2 {#ac-iii-s4-lem-2 .statement tag=04ID}

*令$\mathbf{A}$为环且$m$为$\mathbf{A}$的理想，使得有序对$(\mathbf{A}, m)$满足Hensel的条件。令$\mathbf{B}$为商环$\mathbf{A}/m$，$\pi : \mathbf{A} \to \mathbf{B}$为典范同态。对于$\mathbf{B}$的每个幂等$c$，都存在一个唯一的$\mathbf{A}$幂等$e$，使得$\pi(e) = c$。*

设$a$使得$\pi(a) = c$； no. 5的推论1到定理2可以应用于$\mathbf{A}[X]$和元素$a \in \mathbf{A}$中的多项式$f(X) = X^2 - X$。那么 $f'(a) = 2a - 1$ 并且，正如$\mathbf{B}$中的$\pi(2a - 1) = 2c - 1$和$(2c - 1)^2 = 1$一样，$2c - 1$在$\mathbf{B}$中可逆，因此$2a - 1$在$\mathbf{A}$中可逆（§ 2, no. 13，引理3）。作为$f(a) \in m$，no. 5的推论1至定理2立即给出$e$的存在性和唯一性。

#### 命题 8 {#ac-iii-s4-prop-8 .statement tag=04IE}

*令$\mathbf{A}$为环且$m$为$\mathbf{A}$的理想，使得有序对$(\mathbf{A}, m)$满足Hensel的条件。令$\mathbf{B}$为商环$\mathbf{A}/m$和$\pi : \mathbf{A} \to \mathbf{B}$典范同态。 *如果 B 是有限族* $(\mathfrak{b}_i)_{i \in I}$ *理想的直接合成，则存在 A 的唯一理想族* $(\mathfrak{a}_i)_{i \in I}$ *，使得* $\pi(\mathfrak{a}_i) = \mathfrak{b}_i$ *对于所有* $i \in I$ *并且 A 是该族* $(\mathfrak{a}_i)$ 的直接合成。

让 $I = \sum_i c_i$ 其中 $c_i \in \mathfrak{b}_i$ 代表所有 $i$； $c_i$ 是 $B$ 的幂等，因此 $c_i c_j = 0$ 对于 $i \neq j$。因此，到引理 2 时，存在 $A$ ($i \in I$) 的幂等$e_i$，使得 $\pi(e_i) = c_i$ 对于所有 $i$；因为 $e_i e_j$ 是幂等的
$$
\pi(e_i e_j) = c_i c_j = 0
$$
$i \neq j$，$e_i e_j = 0$ $i \neq j$ (引理 2)；因为 $1 - \sum_i e_i$ 是幂等的
$$
\pi\left(1 - \sum_i e_i\right) = 1 - \sum_i c_i = 0,
$$
同样$1 = \sum_i e_i$。由此可见，$A$是理想$\mathfrak{a}_i = e_i A$的直接合成，而$\pi(\mathfrak{a}_i) = \pi(e_i) B = \mathfrak{b}_i$。

剩下的就是显示这样的分解中的唯一性。现在，假设$A$是理想另一个族$(\mathfrak{a}'_i)_{i \in I}$的直接合成，使得$\pi(\mathfrak{a}'_i) = \mathfrak{b}_i$对于所有$i$；那么$1 = \sum_i e'_i$，其中$e'_i \in \mathfrak{a}'_i$，从而，在$B$，$1 = \sum_i \pi(e'_i)$，其中$\pi(e'_i) \in \mathfrak{b}_i$，这意味着$\pi(e'_i) = c_i$；因为$e'_i$和$e_i$是幂等的，必然是$e'_i = e_i$（引理2），从而完成证明。

#### 注 {#ac-iii-s4-n6-rem-1 .statement tag=04IF}

命题 8 再次给出 $A$ 上半局部环的结构，它是 Hausdorff，并与 $c$-adic 拓扑完成（c $A$ 的 Jacobson 根），它已经作为 § 2, no. 13 的推论获得，推论命题19。

### 习题 {#ac-iii-s4-exercises}

§ 4](exercises/s4/)参见[习题。
