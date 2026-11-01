---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IV
chapter_title: COXETER GROUPS AND TITS SYSTEMS
section: 1
section_title: Coxeter Groups
lang: zh
source: lie-iv-vi
pdf_pages: 0014-0028, 0044-0056
extraction: ocr
subsections:
    - "no": 1
      title: LENGTH AND REDUCED DECOMPOSITIONS
      page: 0
      pdf_page: 14
    - "no": 2
      title: DIHEDRAL GROUPS
      page: 0
      pdf_page: 15
    - "no": 3
      title: FIRST PROPERTIES OF COXETER GROUPS
      page: 0
      pdf_page: 17
    - "no": 4
      title: REDUCED DECOMPOSITIONS IN A COXETER GROUP
      page: 0
      pdf_page: 18
    - "no": 5
      title: THE EXCHANGE CONDITION
      page: 0
      pdf_page: 20
    - "no": 6
      title: CHARACTERISATION OF COXETER GROUPS
      page: 0
      pdf_page: 23
    - "no": 7
      title: FAMILIES OF PARTITIONS
      page: 0
      pdf_page: 23
    - "no": 8
      title: SUBGROUPS OF COXETER GROUPS
      page: 0
      pdf_page: 25
    - "no": 9
      title: COXETER MATRICES AND COXETER GRAPHS
      page: 0
      pdf_page: 26
statements: 30
exercises: 26
content_sha256: fc72db914dd4d073ad5043cedff0d07af10defc3b65e3c191c715aba5b061ca3
translated_from: content/en/lie/IV/01_s1_coxeter_groups.md
translation_method: google
source_content_sha256: aeca25119a4e3b1300664856f323c4070b977911903d6cf99cfb24051466f433
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 1dee64191f8b99b6c77e076f6393ca885aa51a29f93be17fa377694ab5117824
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 1。考克塞特群

在这个截面中，W表示群乘法写成，单位元素1，S表示W的生成元的集合，使得S = S^{-1}和1\notin S。W的每个元素都是乘积 S 的元素的有限序列。从 no. 3 开始，我们假设 S 的每个元素都有阶 2。

### 1. 长度并减少分解

#### 定义 1 {#lie-iv-s1-def-1 .statement tag=0ALN}

设 w \in W。w 的长度（相对于 S），用 l_S(w) 或简称为 l(w) 表示，是最小的整数 q \geq 0，使得 w 是 S 的 q 元素的序列的乘积。 w 的约化分解 （相对于 S）是 S 的元素中的任意序列 s = (s_1, \ldots, s_q)，使得 w = s_1 \cdots s_q 且 q = l(w)。

因此 1 是长度 0 的唯一元素，S 由长度 1 的元素组成。

#### 命题 1 {#lie-iv-s1-prop-1 .statement tag=0ALO}

令 w 和 w' 在 W 中。我们有公式：

$$
l(ww') \leq l(w) + l(w'), \tag{1}
$$
$$
l(w^{-1}) = l(w), \tag{2}
$$
$$
|l(w) - l(w')| \leq l(w{w'}^{-1}). \tag{3}
$$

令 (s_1, \ldots, s_p) 和 (s'_1, \ldots, s'_q) 分别减少 w 和 w' 的分解。因此 l(w) = p 且 l(w') = q。由于 ww' = s_1 \ldots s_p s'_1 \ldots s'_q，我们有 l(ww') \leq p + q, 证明 (1)。由于 S = S^{-1} 且 w^{-1} = s_p^{-1} \ldots s_1^{-1}，我们有 l(w^{-1}) \leq p = l(w)。 替换 w 除以 w^{-1} 给出相反的不等式 l(w) \leq l(w^{-1}), 证明 (2)。 (1) 和 (2) 中的替换 w 除以 ww'^{-1} 得到关系

$$
l(w) - l(w') \leq l(w{w'}^{-1}), \tag{4}
$$
$$
l(w{w'}^{-1}) = l(w'w^{-1}). \tag{5}
$$

交换(4)中的$w$和$w'$，通过(5)、证明(3)得到$l(w') - l(w) \leq l(w{w'}^{-1})$。

#### 推论{#lie-iv-s1-n1-cor-1 .statement tag=0ALP}

*令$s = (s_1, \ldots, s_p)$和$s' = (s'_1, \ldots, s'_q)$为$S$的元素中的两个序列，使得$w = s_1 \ldots s_p$和$w' = s'_1 \ldots s'_q$。如果序列 $(s_1, \ldots, s_p, s'_1, \ldots, s'_q)$ 是 $ww'$ 的减少的分解，则 $s$ 是 $w$ 的减少的分解，并且 $s'$ 是 $w'$ 之一。*

假设、$l(w) \leq p$、$l(w') \leq q$ 和 $l(ww') = p + q$。根据 (1)，我们必须有 $l(w) = p$ 和 $l(w') = q$，因此得出推论。

#### 注 {#lie-iv-s1-n1-rem-1 .statement tag=0ALQ}

鉴于公式（1）和（2），公式$d(w, w') = l(w{w'}^{-1})$定义在$W$上的距离，在右平移下不变。

### 2. 二面角群

#### 定义 2 {#lie-iv-s1-def-2 .statement tag=0ALR}

*二面体群是群由阶两个不同的元素生成。*

#### 例 {#lie-iv-s1-n2-exa-1 .statement tag=0ALS}

令 $M$ 为乘法群 $\{1, -1\}$，并令 $m$ 为整数 $\geq 2$（分别为 $m = \infty$）。然后$M$通过$(-1).x = -x$作用于群$\mathbf{Z}/m\mathbf{Z}$（分别作用于$\mathbf{Z}$），并且相应的通过$\mathbf{Z}/m\mathbf{Z}$作用于$M$的半直接乘积（分别作用于$M$） $\mathbf{Z}$）用$D_m$表示。 $D_m$中的元素因此为对$(\varepsilon, x)$以及$\varepsilon = \pm 1$和$x \in \mathbf{Z}/m\mathbf{Z}$（分别为$x \in \mathbf{Z}$）； $D_m$ 上的群运算由公式给出
$$
(\varepsilon, x).(\varepsilon', x') = (\varepsilon \varepsilon', \varepsilon' x + x').
$$
我们用 1 模 $m$（分别为 $\iota = 1$）和集合表示 $\iota$ 类
$$
\rho = (-1, 0), \quad \rho' = (-1, \iota), \quad \pi = (1, \iota).
$$
然后是$\rho^2 = {\rho'}^2 = 1$和$\pi = \rho \rho'$。 公式
$$
\pi^n = (1, n\iota), \quad \rho \pi^n = (-1, n\iota)
$$
证明$D_m$是由$\{\rho, \rho'\}$生成的二面角群。

#### 命题 2 {#lie-iv-s1-prop-2 .statement tag=0ALT}

*假设$S$由两个不同的元素$s$和$s'$组成阶2。*

(i) *$p = ss'$生成$W$的子群$P$是正常的，$W$是子群$T = \{1, s\}$和$P$的半直接乘积。此外，$(W : P) = 2$.*

(ii) *令 $m$ 为 $p$ 的阶（有限或无限）。那么$m \geq 2$和$W$就是阶$2m$。从$D_m$到$W$有一个独特的同构$\varphi$，这样$\varphi(\rho) = s$和$\varphi(\rho') = s'$。*

(i) 我们有 $sps^{-1} = sss's = s's = p^{-1}$，因此
$$
sp^n s^{-1} = p^{-n}
$$

每整数$n$。由于$W$是由$\{ s, s' \}$生成的，因此是由$\{ s, p \}$生成的，所以子群$P$是正常的。由此可见，$TP$是$W$的子群，并且由于$TP$包含$s$和$s' = sp$，我们有$W = TP = P \cup sP$。因此，为了证明 (i)，只需证明 $W \neq P$ 即可。如果 $W = P$、群 $W$ 是可交换的，那么$p^2 = s^2 {s'}^2 = 1$。但$W = P$中唯一的元素将是1和$p$，与假设相矛盾，$W$包含至少有三个元素，即1、$s$和$s'$。

(ii) 从$s \neq s'$开始，我们有$p \neq 1$，所以$m \geq 2$。由于$P$是阶$m$和$(W : P) = 2$，$W$的阶是$2m$。如果$m$是有限（或无限），则存在从$\mathbf{Z}/m\mathbf{Z}$（或$\mathbf{Z}$）到$P$，从$\pi$到$p$的同构$\varphi'$。此外，从$M = \{ 1, -1 \}$到$T$，从$-1$到$s$，存在同构$\varphi''$。 群$W$是$T$和$P$的半直接乘积。鉴于公式 (9) 和 $\rho \pi^n \rho^{-1} = \pi^{-n}$、$\varphi'$ 和 $\varphi''$ 诱导同构 $\varphi$ 从 $D_m$ 到 $W$，使得 $\varphi(\rho) = s$ 和 $\varphi(\pi) = p$，因此$\varphi(\rho') = s'$。 $\varphi$的唯一性源自$D_m$是由$\{ \rho, \rho' \}$生成的事实。

#### 注 {#lie-iv-s1-n2-rem-1 .statement tag=0ALU}

考虑阶 $2m$ 的二面角群 $W$ 由两个不同的元素 $s$ 和阶 2 的 $s'$ 生成。用 $s_q$ 表示（分别为 $s'_q$） 长度 $q$ 中的序列，其奇数（或偶数）编号项等于 $s$，其偶数（或奇数）编号项等于 $s'$，并设 $w_q$（或$w'_q$）为乘积序列 $s_q$（分别为 $s'_q$）。我们有

$$
w_{2k} = (ss')^k, \quad w_{2k+1} = (ss')^k s,
$$
$$
w'_{2k} = (s's)^k = (ss')^{-k}, \quad w'_{2k+1} = (s's)^k s' = (ss')^{-k-1} s.
$$

如果$s = (s_1, \ldots, s_q)$是$W$的元素$w$的减少的分解（相对于$\{ s, s' \}$），那么显然$s_i \neq s_{i+1}$等于$1 \leq i \leq q-1$。因此，$s = s_q$或$s = s'_q$。

如果$m = \infty$、元素、$(ss')^n$和$(ss')^n s$对于$n \in \mathbf{Z}$是不同的。 因此，元素$w_q$（$q \geq 0$）和$w'_q$（$q > 0$）是不同的，如果$s$是$w_q$（或$w'_q$）的减少的分解，我们必然有$s = s_q$（或$s = s'_q$）。 由此可见，$W$的元素的约化分解的$l(w_q) = l(w'_q) = q$和*集合由$s_q$和$s'_q$*组成。 此外，$W$的每个元素都有一个独特的缩减分解。

现在假设 $m$ 是*有限*。如果$q \geq 2m$，我们有$w_q = w_{q-2m}$和$w'_q = w'_{q-2m}$；如果$m \leq q \leq 2m$，我们有$w_q = w'_{2m-q}$，$w'_q = w_{2m-q}$。因此，如果$q > m$，$s_q$和$s'_q$都不会减少分解。因此，$W$的每个$2m$元素是$1 \leq q \leq m-1$和$w_m = w'_m$的$2m$、元素、$w_0 = w'_0$、$w_q$和$w'_q$之一。因此，这些$2m$元素是不同的，并且如上所述，$q \leq m$的$l(w_q) = l(w'_q) = q$以及$W$的元素的减少分解的*集合由$s_q$和$s'_q$组成$0 \leq q \leq m$*。除$w_m$外，$W$中的每个元素都有一个唯一的缩减分解； $w_m$ 有两个。

### 3. Coxeter 的第一个特性群

回想一下，从现在开始，我们假设 S 的元素是阶 2。

#### 定义 3 {#lie-iv-s1-def-3 .statement tag=0ALV}

如果 (W, S) 满足以下条件，则称其为 Coxeter 系统：

(C) 对于 S 中的 s, s'，令 m(s, s') 为 ss' 的阶，并令 I 为对 (s, s') 的集合，使得 m(s, s') 是有限的。 生成的集合 S 和关系 (ss')^{m(s,s')} = 1，对于 I 形式群 W 的演示文稿 1 中的 (s, s')。

当 (W, S) 是 Coxeter 系统时，人们还滥用语言说 W 是 Coxeter 群。

#### 例 1 {#lie-iv-s1-n3-exa-1 .statement tag=0ALW}

令m为整数$\geq 2$或$\infty$，并令W为群，当$m = \infty$时，由生成元S = {s, s'}的集合和关系$s^2 = {s'}^2 = 1$定义，当m有限时，$s^2 = {s'}^2 = (ss')^m = 1$。另一方面考虑由 (7) 定义的 D_m 的二面角群 D_m (no. 2, 例) 和元素 $\rho$ 和 $\rho'$。由于$\rho^2 = (\rho')^2 = 1$和$(\rho\rho')^m = 1$，当m有限时，从W到D_m存在唯一同态 f，使得$f(s) = \rho$和$f(s') = \rho'$。由于 $\rho\rho'$ 的长度为阶 m，因此 ss' 本身的长度为阶 m。因此，(W, S) 是 Coxeter 系统，W 是阶 $2m$ 的二面角群，f 是同构（命题 2）。

根据结构的迁移，得出每个二面角群都是 Coxeter 群。

#### 例 2 {#lie-iv-s1-n3-exa-2 .statement tag=0ALX}

令 $\mathfrak{S}_n$ 为次数 n 的对称群，且$n \geq 2$。令 $s_i$ 为 i 和 $i+1$ 对 $1 \leq i < n$ 的转置，并令 S = {s_1, ..., s_{n-1}}。可以证明（§ 2, no.4、例和 § 1，练习 4）$(\mathfrak{S}_n, S)$ 是 Coxeter 系统。

#### 例 3 {#lie-iv-s1-n3-exa-3 .statement tag=0ALY}

对于有限 Coxeter 群、cf. 的分类4、§ 4。

#### 注 {#lie-iv-s1-n3-rem-1 .statement tag=0ALZ}

假设 (W, S) 是 Coxeter 系统。对于所有 $s \in S$，存在从 W 到群 {1, -1} 的特征为 $\varepsilon(s) = -1$ 的同态 $\varepsilon$。我们称$\varepsilon(w)$为w的签名；它等于$(-1)^{l(w)}$。 公式 $\varepsilon(ww') = \varepsilon(w)\varepsilon(w')$ 因此转换为 $l(ww') \equiv l(w) + l(w') \mod 2$。

1 这意味着 (W, S) 具有以下泛性质：给定从 S 到 G 的群 G 和映射 f，使得 $(f(s)f(s'))^{m(s,s')} = 1$ 对于 I 中的 (s, s')，存在从 W 到 G 延伸 f 的同态 g。这个同态是唯一的，因为S生成W。这个定义的等价形式如下。令$\overline{W}$为群，从$\overline{W}$到W的f同态以及从S到$\overline{W}$的h映射，使得$f(h(s)) = s$和$(h(s)h(s'))^{m(s,s')} = 1$对于S中的(s, s')并且使得h(s)(对于$s \in S$) 生成$\overline{W}$。那么 f 是单射的（因此从 $\overline{W}$ 到 W 是同构）。

#### 命题 3 {#lie-iv-s1-prop-3 .statement tag=0AM0}

假设 (W, S) 是 Coxeter 系统。那么，当且仅当满足以下条件时，S的两个元素 s和s'在W中是共轭$^2$：

(I) S 的元素存在有限序列$(s_1, \ldots, s_q)$，使得$s_1 = s, s_q = s'$和$s_j s_{j+1}$对于$1 \leq j < q$来说是有限奇数阶。

令 S 中的 s 和 s' 使得 $p = ss'$ 具有有限阶 $2n + 1$。由(9)，$sp^{-n} = p^n s$因此

$$
p^n sp^{-n} = p^n p^n s - p^{-1} s = s' ss = s',
$$

并且 $s'$ 是 s 的共轭。

对于 S 中的所有 s，令 $A_s$ 为 $s' \in S$ 满足 (I) 中的集合。根据(I)中的假设，元素$s_j$和$s_{j+1}$对于$1 \leq j < q$来说是共轭，因此$A_s$的每个元素$s'$对于s来说都是共轭。

令 $f$ 为映射，从 S 到 $M = \{1, -1\}$ 在 $A_s$ 上等于 1，在 $S - A_s$ 上等于 -1。令 S 中的 $s'$ 和 $s''$ 使得 $s's''$ 的长度为有限阶 m。如果$s'$和$s''$都在$A_s$或者都在$S - A_s$，那么$f(s') f(s'') = 1$。在另一种情况下，$f(s') f(s'') = -1$，但 m 是偶数。因此在所有情况下都是$(f(s') f(s''))^m = 1$。由于 (W, S) 是 Coxeter 系统，因此存在从 W 到 M 的同态 g，在 S 上感应出 f。令 $s'$ 为 s 的共轭。由于g的s属于到核，$s'$也是如此，因此$f(s') = g(s') = 1$，最后是$s' \in A_s$。 Q.E.D.

### 4. 在 COXETER 中减少分解群

假设 (W, S) 是 Coxeter 系统。令T为S的元素W中的共轭集合。对于S的元素任意有限序列$s = (s_1, \ldots, s_q)$，用元素的$\Phi(s)$序列$(t_1, \ldots, t_q)$表示T 的定义为

$$
t_j = (s_1 \ldots s_{j-1}) s_j (s_1 \ldots s_{j-1})^{-1} \quad \text{for } 1 \leq j \leq q.
$$

然后是$t_1 = s_1$和$s_1 \ldots s_q = t_q t_{q-1} \ldots t_1$。对于任何元素$t \in T$，用整数$j$的$n(s, t)$数表示，使得$1 \leq j \leq q$和$t_j = t$。最后，放

$$
R = \{1, -1\} \times T.
$$

#### 引理 1 {#lie-iv-s1-lem-1 .statement tag=0AM1}

(i) 设$w \in W$和$t \in T$。对于S的元素的所有序列$s = (s_1, \ldots, s_q)$，数$(-1)^{n(s, t)}$具有相同的值$\eta(w, t)$，使得$w = s_1 \ldots s_q$。

(ii) 对于 $w \in W$，令 $U_w$ 为映射，从 R 到自身定义为

$$
U_w(\varepsilon, t) = (\varepsilon \cdot \eta(w^{-1}, t), wtw^{-1}) \quad (\varepsilon = \pm 1, t \in T).
$$

从W到R的置换的群，映射$w \mapsto U_w$为同态。

(2) 回想一下，如果存在 W 的内自同构且变换彼此相交，则群 W 的两个元素（分别为两个子集）被称为共轭。

对于 $s \in S$，定义映射 $U_s$ 从 $R$ 到自身
$$
U_s(\varepsilon, t) = (\varepsilon.(-1)^{\delta_{s,t}}, st s^{-1}) \quad (\varepsilon = \pm 1, t \in T),
$$
其中 $\delta_{s,t}$ 是克罗内克符号。 $U_s^2 = \mathrm{Id}_R$是直接的，这表明$U_s$是$R$的置换。

令$s = (s_1, \ldots, s_q)$为$S$的元素中的序列。输入$w = s_q \ldots s_1$和$U_s = U_{s_q} \ldots U_{s_1}$。我们将在 $q$ 的归纳之前证明，
$$
U_s(\varepsilon, t) = (\varepsilon.(-1)^{n(s,t)}, wt w^{-1}).
$$
对于 $q = 0, 1$ 来说这是很清楚的。如果 $q > 1$，则输入 $s' = (s_1, \ldots, s_{q-1})$ 并
$$
w' = s_{q-1} \ldots s_1.
$$
使用归纳假设，我们得到
$$
\begin{align*}
U_s(\varepsilon, t) &= U_{s_q}(U_{s_q}(\varepsilon.(-1)^{n(s',t)}, w't {w'}^{-1})) \\
&= (\varepsilon.(-1)^{n(s',t)+\delta_{s_q,w't {w'}^{-1}}}, wt w^{-1}).
\end{align*}
$$
但是$\Phi(s) = (\Phi(s'), {w'}^{-1} s_q w')$和$n(s, t) = n(s', t) + \delta_{w', -1} s_q w', t$，证明公式（14）。

现在让$s, s' \in S$使得$p = ss'$有有限的阶$m$。 令$s = (s_1, \ldots, s_{2m})$为$S$的元素的序列，对于$j$奇数由$s_j = s$定义，对于$j$偶数由$s_j = s'$定义。 那么 $s_{2m} \ldots s_1 = p^{-m} = 1$ 和公式 (11) 意味着
$$
t_j = p^{j-1} s \quad \text{for } 1 \leq j \leq 2m.
$$
由于$p$是阶$m$，元素$t_1, \ldots, t_m$是不同的，$t_{j+m} = t_j$对于$1 \leq j \leq m$是不同的。 对于所有$t \in T$，整数$n(s, t)$因此等于0或2，并且（14）表明$U_s = \mathrm{Id}_R$。 其他字，$(U_s U_{s'})^m = \mathrm{Id}_R$。 Thus, by the definition of Coxeter systems, there exists a homomorphism $w \mapsto U_w$ from $W$ to the group of permutations of $R$ such that $U_s$ is given by the right-hand side of (13). 然后，对于每个序列$s = (s_1, \ldots, s_q)$，$U_w = U_s$使得$w = s_q \ldots s_1$和引理1紧随(14)而来。

#### 引理 2 {#lie-iv-s1-lem-2 .statement tag=0AM2}

*设$s = (s_1, \ldots, s_q)$、$\Phi(s) = (t_1, \ldots, t_q)$和$w = s_1 \ldots s_q$。令$T_w$为$T$的元素中的集合，使得$\eta(w, t) = -1$。那么，当且仅当 $t_i$ 不同时，$s$ 是 $w$ 的缩减分解，在这种情况下，$T_w = \{ t_1, \ldots, t_q \}$ 和 $\mathrm{Card}(T_w) = l(w)$。*

显然$T_w \subset \{ t_1, \ldots, t_q \}$。将$s$减少，可得$\mathrm{Card}(T_w) \leq l(w)$。此外，如果$t_i$不同，则根据$t$是否存在属于至$\{ t_1, \ldots, t_q \}$，$n(s, t)$等于1或0。由此得出$T_w = \{ t_1, \ldots, t_q \}$和$q = \mathrm{Card}(T_w) \leq l(w)$，这意味着$s$被减少。最后假设$t_i = t_j$和$i < j$。这给出 $s_i = us_j u^{-1}$，以及 $u = s_{i+1} \ldots s_{j-1}$，因此

$$
w = s_1 \ldots s_{i-1} s_{i+1} \ldots s_{j-1} s_{j+1} \ldots s_q.
$$

这表明$s$不是$w$的约分解。

#### 引理 3 {#lie-iv-s1-lem-3 .statement tag=0AM3}

*设$w \in W$和$s \in S$使得$l(sw) \leq l(w)$。 For any sequence $s = (s_1, \ldots, s_q)$ of elements of $S$ with $w = s_1 \ldots s_q$, there exists an integer $j$ such that $1 \leq j \leq q$ and*

$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_{j-1} s_j.
$$

设$p$为$w$和$w' = sw$的长度。由 no. 3、$l(w') \equiv l(w) + 1$ mod 的 *注* 得出。 2.假设$l(w') \leq l(w)$和关系

$$
|l(w) - l(w')| \leq l(w{w'}^{-1}) = l(s) = 1
$$

从而导致$l(w') = p - 1$。 选择减少分解

$$
(s'_1, \ldots, s'_{p-1})
$$

$w'$ 并放入 $s = (s, s'_1, \ldots, s'_{p-1})$ 和 $\Phi(s') = (t'_1, \ldots, t'_p)$。很明显，$s'$是$w$和$t'_1 = s$的减少的分解。 元素 $t'_1, \ldots, t'_p$ 与引理 2 不同，我们有 $n(s', s) = 1$。由于$w$是序列$s$的乘积，所以我们有$n(s, s) \equiv n(s', s)$模。 2乘以引理1，因而$n(s, s) \neq 0$。因而，$s$等于元素$t_j$或序列$\Phi(s)$之一，因此引理。

#### 注 {#lie-iv-s1-n4-rem-1 .statement tag=0AM4}

引理 2 中定义的集合 $T_w$ 由形式 $w''s{w''}^{-1}$ 相应的的元素到三元组$(w', w'', s) \in W \times W \times S$ 组成，使得$w = w''sw'$ 和$l(w') + l(w'') + 1 = l(w)$。

### 5. 交换条件

“交换条件”是关于$(W, S)$的以下断言：

**(E)** *令$w \in W$和$s \in S$使得$l(sw) \leq l(w)$。对于 $w$ 的任何约简分解 $(s_1, \ldots, s_q)$，存在整数 $j$，使得 $1 \leq j \leq q$ 和*

$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_{j-1} s_j.
$$

我们假设在这个数中$(W, S)$满足(E)。到引理 3 时，如果 $(W, S)$ 是 Coxeter 系统，则情况如此。因而，该数的结果适用于 Coxeter 系统。

#### 命题 4 {#lie-iv-s1-prop-4 .statement tag=0AM5}

*令 $s \in S, w \in W$ 和 $s = (s_1, \ldots, s_q)$ 为 $w$ 的约分解。那么必须满足以下条件之一：*

a) $l(sw) = l(w) + 1$ 和 $(s, s_1, \ldots, s_q)$ 是 $sw$ 的减少的分解。

b) $l(sw) = l(w) - 1$并且存在整数$j$使得$1 \leq j \leq q$、$(s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q)$是$sw$的减少的分解并且$(s, s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q)$是$w$的减少的分解。

把$w' = sw$。到no. 1的公式(3)，我们有
$$
|l(w) - l(w')| \leq l(s) = 1.
$$
我们区分两种情况：

a) $l(w') > l(w)$。然后$l(w') = q + 1$和$w' = ss_1 \ldots s_q$，所以
$$
(s, s_1, \ldots, s_q)
$$
分解减少为 $w'$。

b) $l(w') \leq l(w)$。由(E)，存在整数$j$使得$1 \leq j \leq q$和(16)被满足。然后$w = ss_1 \ldots s_{j-1} s_{j+1} \ldots s_q$，因此
$$
w' = s_1 \ldots s_{j-1} s_{j+1} \ldots s_q.
$$
从$q - 1 \leq l(w') \leq q$开始，$l(w') = q - 1$和$(s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q)$是$w'$的减少的分解。

#### 引理 4 {#lie-iv-s1-lem-4 .statement tag=0AM6}

令$w \in W$具有长度$q \geq 1$，令D为$w$减少的分解的集合，并令F为从D到集合E的映射。假设$F(s) = F(s')$如果元素 D 满足的$s = (s_1, \ldots, s_q); s' = (s'_1, \ldots, s'_q)$ 以下假设之一：

a) $s_1 = s'_1$ 或 $s_q = s'_q$。
b) S 中存在 s 和 $s'$，使得对于 $j$ 奇数和 $k$ 偶数，$s_j = s'_k = s$ 和 $s_k = s'_j = s'$。

那么F是常数。

A) 设 $s, s' \in D$ 并放入 $t = (s'_1, s_1, \ldots, s_{q-1})$。我们将证明如果$F(s) \neq F(s')$则$t \in D$和$F(t) \neq F(s)$。事实上，$w = s'_1 \ldots s'_q$因此$s'_1 w = s'_2 \ldots s'_q$是长度$< q$。根据命题 4，存在整数 $j$，使得 $1 \leq j \leq q$ 和序列 $u = (s'_1, s_1, \ldots, s_{j-1}, s_{j+1}, \ldots, s_q)$ 属于到 D。我们有 $F(u) = F(s')$ by 条件 a)；如果$j \neq q$，出于同样的原因，我们将得到$F(s) = F(u)$，因此$F(s) = F(s')$与我们的假设相反。因此$j = q$，因此$t = u \in D$和$F(t) = F(s') \neq F(s)$。

B) 让 s 和 $s'$ 属于到 D。对于 S 的 q 元素的任何整数 $j$ 以及 $0 \leq j \leq q + 1$ 定义序列 $s_j$，如下：
$$
s_0 = (s'_1, \ldots, s'_q)
$$
$$
s_1 = (s_1, \ldots, s_q)
$$
$$
s_{q+1-k} = (s_1, s'_1, \ldots, s_1, s'_1, s_1, s_2, \ldots, s_k)
$$
对于$q - k$偶数和$0 \leq k \leq q$
$$
s_{q+1-k} = (s'_1, s_1, \ldots, s_1, s'_1, s_1, s_2, \ldots, s_k)
$$
对于$q - k$奇数和$0 \leq k \leq q$。

用 (H_j) 断言 “s_j \in D, s_{j+1} \in D \text{ 和 } F(s_j) \neq F(s_{j+1})”表示。根据 A)，(H_j) \ 意味着 $0 \leq j < q$ 的 (H_{j+1})，并且条件 b) 不满足 (H_q)。因而，(H_0)不满足。由于$s_0 = s'$和$s_1 = s$，因此得出$F(s) = F(s')$。

#### 命题 5 {#lie-iv-s1-prop-5 .statement tag=0AM7}

*设 M 为幺半群（其中单位元 1）且 f 映射从 S 到 M。对于 s, s' \in S，令 m(s, s') 为 ss' 的阶并放入*

$$
a(s, s') = \begin{cases}
(f(s)f(s'))^l & \text{if } m(s, s') = 2l, l \text{ finite} \\
(f(s)f(s'))^lf(s) & \text{if } m(s, s') = 2l + 1, l \text{ finite} \\
1 & \text{if } m(s, s') = \infty.
\end{cases}
$$

*如果当$s \neq s'$在S中时$a(s, s') = a(s', s)$，则从W到M存在映射g使得*
$$
g(w) = f(s_1) \ldots f(s_q)
$$
*适用于所有 $w \in W$ 以及任意减少的分解 $(s_1, \ldots, s_q)$。*

对于任何$w \in W$，令$D_w$是w的减少的分解和$F_w$映射从$D_w$到M的集合，定义为
$$
F_w(s_1, \ldots, s_q) = f(s_1) \ldots f(s_q).
$$
我们将通过 w 的长度上的归纳证明 $F_w$ 是常数，这将建立命题 5。 $l(w) = 0, 1$ 的情况是微不足道的，我们假设 $q \geq 2$ 并且我们的断言被证明对于元素 w 和 $l(w) < q$。设 w 为长度 q 和 $s, s' \in D_w$；通过引理 4 足以证明引理的情况 a) 和 b) 中的$F_w(s) = F_w(s')$。

a) 公式
$$
F_w(s_1, \ldots, s_q) = f(s_1)F_{w''}(s_2, \ldots, s_q) = F_{w'}(s_1, \ldots, s_{q-1})f(s_q)
$$
对于$w' = s_1 \ldots s_{q-1}$、$w'' = s_2 \ldots s_q$和归纳假设，如果$s_1 = s'_1$或$s_q = s'_q$，则显示$F_w(s) = F_w(s')$。

b) 假设 S 存在两个元素和 s'，使得对于 j 奇数和 k 偶数，$s_j = s'_k = s$ 和 $s_k = s'_j = s'$。治疗这个案子就够了$s \neq s'$。 序列 s 和 s' 是由 s 和 s' 生成的二面体群中 w 的两个不同的约化分解。根据no. 2中的*注*，ss'的阶 m必然是有限的，并且在注中的记号中，$s = s_m$和$s' = s'_m$。因而，$F_w(s) = a(s, s')$和$F_w(s') = a(s', s)$，因而
$$
F_w(s) = F_w(s').
$$

### 6. 考克斯特的特征群

#### 定理 1 {#lie-iv-s1-thm-1 .statement tag=0AM8}

(W, S) 是 Coxeter 系统当且仅当它满足 no. 5 的交换条件 (E)。

no. 4 中的引理 3 表明任何 Coxeter 系统满足 (E)。

相反，假设满足(E)。令G为从S到G的群和f映射，使得每当s和$s'$属于到S和$ss'$时$(f(s)f(s'))^m = 1$是有限的阶m。根据命题 5，从 W 到 G 存在映射 g，使得
$$
g(w) = f(s_1) \ldots f(s_q)
$$
每当 $w = s_1 \ldots s_q$ 为长度 q 时。要证明 (W, S) 是 Coxeter 系统，只需证明 g 是同态，即公式的推论
$$
g(sw) = f(s)g(w) \quad \text{for } s \in S, w \in W
$$
由于 S 生成 W。根据 no. 5 的 Prop. 4，只有两种情况是可能的：

a) $l(sw) = l(w) + 1$：如果$(s_1, \ldots, s_q)$是$w$的减少的分解，则$(s, s_1, \ldots, s_q)$是$sw$的减少的分解，因而（21）。

b) $l(sw) = l(w) - 1$：放入$w' = sw$；然后是$w = sw'$和$l(sw') = l(w') + 1$。由a)，$g(w) = f(s)g(sw)$，因此从$(f(s))^2 = 1$开始$f(s)g(w) = g(sw)$。

### 7. 划分的家庭

假设 (W, S) 是 Coxeter 系统。对于任何$s \in S$，令$P_s$为W中元素$w$的集合，使得$l(sw) > l(w)$。我们有以下属性：

（一）$\bigcap_{s \in S} P_s = \{1\}$。

事实上，让$w \neq 1$在W中，并让$(s_1, \ldots, s_q)$是$w$的减少的分解。那么$q \geq 1$和$(s_2, \ldots, s_q)$是$s_2w$的减少的分解，所以$l(w) = q$和$l(s_1w) = q - 1$。因此，$w \notin P_{s_1}$。

(B) *对于 S 中的任何 s，W 的集合 $P_s$ 和 $sP_s$ 形式划分*

设$w \in W$和$s \in S$。根据no. 5的第4条命题，我们必须区分两种情况：

a) $l(sw) = l(w) + 1$：然后$w \in P_s$。
b) $l(sw) = l(w) - 1$：将$w' = sw$改为$w = sw'$；那么
$$
l(w') < l(sw')
$$
因此$w' \in P_s$，即$w \in sP_s$。

(C) *设 s、s' 在 S 中，w 在 W 中。如果 $w \in P_s$ 和 $ws' \in P_s$，则$sw = ws'$。*

设$q$为$w$中的长度。从$w \in P_s$得出$l(sw) = q + 1$；从$ws' \in P_s$得出$l(sws') = l(ws') - 1 \leq q$。从$l(sws') = l(sw) \pm 1$开始，我们终于有了$l(ws') = q + 1$和$l(sws') = q$。

令$(s_1, \ldots, s_q)$为$w$和$s_{q+1} = s'$的约分解；那么 $(s_1, \ldots, s_q, s_{q+1})$ 是分解的元素 $ws'$ 长度 $q + 1$ 的减少。通过交换条件，存在整数 $j$ 与 $1 \leq j \leq q + 1$ 使得
$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_j.
$$
(22)
如果$1 \leq j \leq q$，我们就会有$sw = s_1 \ldots s_{j-1} s_{j+1} \ldots s_q$与公式$l(sw) = q + 1$相矛盾。因此$j = q + 1$和公式(22)可以写成$sw = ws'$。

相反，我们得到以下结果：

#### 命题 6 {#lie-iv-s1-prop-6 .statement tag=0AM9}

*设* $(P_s)_{s \in S}$ *是子集的* $W$ *满足* (C) *和以下条件*的家庭：

(A') $1 \in P_s$ *对于所有人* $s \in S$。
(B') *集合* $P_s$ *和* $sP_s$ *对于所有* $s \in S$ 都是不相交的。

*那么*，$(W, S)$*是一个Coxeter系统，并且*$P_s$*由元素*$w$*组成*$W$*使得*$l(sw) > l(w)$。

令$s \in S$和$w \in W$。有两种可能：

a) $w \notin P_s$。令 $(s_1, \ldots, s_q)$ 为 $w$ 的约分解，并且
$$
w_j = s_1 \ldots s_j
$$
$1 \leq j \leq q$；还放了$w_0 = 1$。由于 $w_0 \in P_s$ 由 (A') 且由于 $w = w_q$ 不在 $P_s$ 中，因此存在整数 $j$ 与 $1 \leq j \leq q$，使得 $w_{j-1} \in P_s$ 和 $w_j = w_{j-1} s_j$ 不会属于到 $P_s$。通过（C），
$$
sw_{j-1} = w_{j-1} s_j.
$$
由此我们证明了公式
$$
ss_1 \ldots s_{j-1} = s_1 \ldots s_{j-1} s_j
$$
这意味着$sw = s_1 \ldots s_{j-1} s_{j+1} \ldots s_q$和$l(sw) < l(w)$。

b) $w \in P_s$：放入$w' = sw$，使得$w' \notin P_s$乘以(B')。通过a)，我们就有$l(sw') < l(w')$，即$l(w) < l(sw)$。

a) 和 b) 的比较证明 $P_s$ 由那些 $w \in W$ 组成，使得 $l(sw) > l(w)$。正如我们在 a) 中看到的，交换条件由此而来，因此 $(W, S)$ 是 Coxeter 系统（no. 6 的第 1 个）。

### 8. 考克塞特的子群群

在这个数中，我们假设$(W, S)$是Coxeter系统。对于$S$的任何子集$X$，我们用$X$生成的$W$的$W_X$子群表示。

#### 命题 7 {#lie-iv-s1-prop-7 .statement tag=0AMA}

*让$w$位于$W$中。存在 $S$ 的子集 $S_w$，使得 $\{s_1, \ldots, s_q\} = S_w$ 对于 $w$ 的任何减少的分解 $(s_1, \ldots, s_q)$。*

用$M$表示$S$的子集的幺半群由……组成和合成律$(A, B) \mapsto A \cup B$； $M$的单位元素是$\varnothing$。将 $f(s) = \{s\}$ 替换为 $s \in S$。我们将把no. 5的第5号提案应用到$M$和$f$。如果$m(s, s')$是有限的，那么对于$S$中的$s, s'$，我们有$a(s, s') = \{s, s'\}$，因此从$W$到$M$存在映射$g : w \mapsto S_w$，使得$g(w) = f(s_1) \cup \cdots \cup f(s_q)$，即$S_w = \{s_1, \ldots, s_q\}$对于任何$w \in W$ 以及 $w$ 的任何减少的分解 $(s_1, \ldots, s_q)$。

#### 推论 1 {#lie-iv-s1-prop-7-cor-1 .statement tag=0AMB}

*对于$S$的任何子集$X$，$W$的子群$W_X$由$W$的元素$w$组成，使得$S_w \subset X$。

若$w = s_1 \ldots s_q$且$s_1, \ldots, s_q$在$S$内，则$w^{-1} = s_q \ldots s_1$；因此

$$
S_{w^{-1}} = S_w.
$$

no. 5的第4条命题表明$S_{sw'} \subset \{s\} \cup S_{w'}$对应于$s \in S$和$w' \in W$，这意味着公式

$$
S_{ww'} \subset S_w \cup S_{w'}
$$

由 $w$ 长度归纳出发。由(23)和(24)，$w \in W$的集合$U$使得$S_w \subset X$是$W$的子群；我们有 $X \subset U \subset W_X$，因此有 $U = W_X$。

#### 推论 2 {#lie-iv-s1-prop-7-cor-2 .statement tag=0AMC}

*对于 $S$ 中的任意子集 $X$，我们有 $W_X \cap S = X$。

这是从 Cor 得出的。 1 和 $S$ 中的 $s$ 为公式 $S_s = \{s\}$。

#### 推论 3 {#lie-iv-s1-prop-7-cor-3 .statement tag=0AMD}

*集合 $S$ 是 $W$ 的最小生成的集合。

如果$X \subset S$生成$W$，则$W = W_X$，因此$X = S \cap W_X = S$。 2.*

#### 推论 4 {#lie-iv-s1-prop-7-cor-4 .statement tag=0AME}

*对于$S$中的任何子集$X$和$W_X$中的任何$w$，$w$中的长度相对于$W_X$中的生成的集合$X$等于$l_S(w)$。

令 $(s_1, \ldots, s_q)$ 为 $w$ 的减少的分解，视为 $W$ 的元素。对于 $1 \leq j \leq q$，我们有 $w = s_1 \ldots s_q$ 和 $s_j \in X$（Cor. 1）；另外，$w$不能由$q = l_S(w)$定义为$X \subset S$$q' < q$元素乘积。*

#### 定理 2 {#lie-iv-s1-thm-2 .statement tag=0AMF}

(i) *对于 $S$ 中的任何子集 $X$，对 $(W_X, X)$ 是 Coxeter 系统。*

(ii) 设 $(X_i)_{i \in I}$ 为 $S$ 的子集的家庭。如果$X = \bigcap_{i \in I} X_i$，则$W_X = \bigcap_{i \in I} W_{X_i}$。

(iii) 令$X$和$X'$为$S$中的两个子集。那么$W_X \subset W_{X'}$（或$W_X = W_{X'}$）当且仅当$X \subset X'$（或$X = X'$）。

$X$的每个元素都是阶2和$X$生成$W_X$。让$x \in X$和$w \in W_X$与$l_X(xw) \leq l_X(w) = q$。由科.提案 7 中的第 4 条，我们有
$$
l_S(xw) \leq l_S(w) = q.
$$
令$x_1, \ldots, x_q$为$X$的元素，使得$w = x_1 \ldots x_q$。由于$(W, S)$满足交换条件（no. 6的Th.1），因此存在整数$j$使得$1 \leq j \leq q$和$xx_1 \ldots x_{j-1} = x_1 \ldots x_{j-1} x_j$。因此，$(W_X, X)$满足交换条件，因此是Coxeter系统（no. 6的Th.1）。这就证明了(i)。

断言 (ii) 和 (iii) 紧随 Cor.提案 7 中的 1 条。

### 9. 考克塞特矩阵和考克塞特图

#### 定义 4 {#lie-iv-s1-def-4 .statement tag=0AMG}

令 $I$ 为集合。 型 $I$ 的 Coxeter 矩阵是一个对称的平方矩阵 $M = (m_{ij})_{i,j \in I}$，其条目为整数或 $+\infty$ 满足关系
$$
m_{ii} = 1 \quad \text{for all } i \in I; \tag{25}
$$
$$
m_{ij} \geq 2 \quad \text{for } i, j \in I \text{ with } i \neq j. \tag{26}
$$

型 $I$ 的 Coxeter 图（通过滥用语言）是图 $\Gamma^3$ 的对由……组成，其$I$ 作为其集合顶点，映射 $f$ 来自集合的边绘制到$+\infty$的集合由……组成和整数$\geq 3$的集合。 $\Gamma$ 称为 Coxeter 图 $(\Gamma, f)$ 的底层图。

Coxeter 图 $(\Gamma, f)$ 与型 $I$ 的任何 Coxeter 矩阵 $M$ 相关联，如下所示：

图$\Gamma$有集合个顶点$I$和集合个边集合对$\{i, j\}$（$I$的元素），使得$m_{ij} \geq 3$和映射 $f$关联到$M$的边$\{i, j\}$相应的元素$m_{ij}$。

显然，这在型$I$的Coxeter图矩阵的集合和型$I$的Coxeter图的集合之间产生了双射。

为了帮助读者理解我们的论点，我们经常用图表来表示型 $I$ 的 Coxeter 图，用于表示其底层图，并在每条边的旁边或上方写上 $\{i, j\}$ 数 $f(\{i, j\})$。如果这些数等于 3，我们通常会忽略它们。

3 请参阅附录了解定义以及此处使用的图的属性。

如果 (W, S) 是一个 Coxeter 系统、矩阵 $M = (m(s, s'))_{s, s' \in S}$，其中 $m(s, s')$ 是 $ss'$ 的阶，则为型 S 的 Coxeter 矩阵，称为 的 Coxeter 矩阵 （W，S）：确实，对于所有 $s \in S$，从 $s^2 = 1$ 开始，$m(s, s) = 1$；如果从 $ss' = (s's)^{-1}$ 开始 $s \neq s'$，则$m(s, s') = m(s', s) \geqslant 2$ 则为 $\neq 1$。与 M 相关的 Coxeter 图 $(\Gamma, f)$ 称为 (W, S) 的 Coxeter 图。我们注认为$\Gamma$的两个顶点$s$和$s'$是“连接”当且仅当$s$和$s'$不交换。对于例，阶 $2m$ 的二面角群的 Coxeter 矩阵为 $\begin{pmatrix} 1 & m \\ m & 1 \end{pmatrix}$，其 Coxeter 图表示为

$$
\circ \overset{m}{\text{---}} \circ
$$

当$m \geqslant 3$（或

$$
\circ \text{---} \circ
$$

如果 $m = 3$) 并且由

$$
\circ \qquad \circ
$$

当$m = 2$时。 \* 对称群 $\mathfrak{S}_n$ 的 Coxeter 图表示为

$$
\circ \text{---} \circ \text{---} \circ \cdots \circ \text{---} \circ
$$

（$n - 1$ 顶点。）\*

我们稍后（第 V, § 4 章）证明，相反，任何 Coxeter 矩阵都是 Coxeter 系统的矩阵。

如果 Coxeter 图的底层图是*连通*（附录，no. 2）且*非空*，则 Coxeter 系统 (W, S) 被称为*不可约*。等价地，S 是非空的，并且不存在 S 的划分分成 S 的两个不同的子集 S' 和 S''，使得 S' 的每个元素与 S'' 的每个元素交换。更一般地，令$(\Gamma_i)_{i \in I}$为$\Gamma$（附录，no. 2）的连通分量族，并令$S_i$为$\Gamma_i$顶点的集合。令$W_i = W_{S_i}$为由$S_i$(cf.no. 8)生成的W的子群。那么 $(W_i, S_i)$ 是不可约 Coxeter 系统 (no. 8, Th. 2) ，称为 (W, S) 的*不可约分量*。而且，群 W 是$i \in I$ 子群 $W_i$ 的*限制直接乘积*[^1]。事实上，这是从以下更一般的命题得出的：

#### 命题 8 {#lie-iv-s1-prop-8 .statement tag=0AMH}

令$(S_i)_{i \in I}$为$S$的划分，使得$S_i$的每个元素与$S_j$的每个元素交换，如果$i \neq j$。对于所有$i \in I$，令$W_i$为由$S_i$生成的子群。那么$W$就是家庭$(W_i)_{i \in I}$的限制直接乘积。

很明显，对于$j \neq i$的$W_j$的并生成的所有$i \in I$、子群、$W'_i$也是由$S'_i = \bigcup_{j \neq i} S_j$生成的。因此
$$
W_i \cap W'_i = W_\varnothing = \{1\}
$$
通过 Th。 no. 8 中的 2 个。由于$W$是由$W_i$的并生成的，这就证明了命题。

### 习题{#lie-iv-s1-exercises}

参见[习题为 § 1](exercises/s1/)。

[^1]: 群 G 是子群族$(G_i)_{i \in I}$的*受限直接乘积*，如果对于I的任何有限子集 J，由$i \in J$的$G_i$生成的G的子群$G_J$是直接$i \in J$的$G_i$的乘积，并且如果G是$G_J$的并。 等价地，对于$i \neq j$，$G_i$的每个元素与$G_j$的每个元素可交换，并且G的每个元素可以唯一地写为乘积$\prod_{i \in I} g_i$，对于除有限多个之外的所有$g_i \in G_i$和$g_i = 1$ 指标$i$。 最后一个条件相当于说，G是由$G_i$的并生成的，并且对于所有$i \in I$和I的所有有限子集J生成$G_i \cap G_J = \{1\}$，使得$i \notin J$。
