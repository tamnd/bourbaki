---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 4
section_title: Inverse limits of measures
lang: zh
source: int-vii-ix
book_pages: INT IX.49-INT IX.55, INT IX.112-INT IX.113
pdf_pages: 0231-0237, 0294-0295
extraction: ocr
subsections:
    - "no": 1
      title: Complements on compact spaces and inverse limits
      page: 50
      pdf_page: 232
    - "no": 2
      title: Inverse systems of measures
      page: 50
      pdf_page: 232
    - "no": 3
      title: The case of countable inverse systems
      page: 54
      pdf_page: 236
statements: 7
exercises: 2
content_sha256: 31bfe76b3e293069059a90307cc988212438bb0d85641f11c615e2869bd31374
translated_from: content/en/int/IX/04_s4_inverse_limits_of_measures.md
translation_method: google
source_content_sha256: 5dd841f191bacbaf28441eec0f88259078f641775a797c2d66f85a7d4bd2a6c4
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: d287909e5b5fdeacfbd67fb2fa9bdb648fec9a79e5556cd3ce0a87214a484b8a
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。 逆极限措施

*在整个截面中，I表示非空集合，配备预序关系，表示$i \leq j$，并针对此关系。 回想一下（GT，I, §4, No. 4），由I索引的拓扑空间的逆系是一个族$(T_i, p_{ij})$，其中$T_i$是拓扑空间，$p_{ij}$是$T_j$的连续映射到$T_i$代表$i \leq j$，其中$p_{ii}$是$T_i$的恒等映射，而$p_{ik} = p_{ij} \circ p_{jk}$代表$i \leq j \leq k$。 令 T 为拓扑空间和 $(p_i)_{i \in I}$ 连续映射 $p_i : T \to T_i$ 族。 The family $(p_i)_{i \in I}$ is said to be coherent if $p_i = p_{ij} \circ p_j$ for $i \leq j$, and it is said to be separating if for distinct $x, y$ in T there exists an $i \in I$ such that $p_i(x) \neq p_i(y)$. 当$T = \varprojlim T_i$和$p_i$是T的典范映射进入$T_i$时，$(p_i)_{i \in I}$族是连贯和分离的。*

(3) 在 Souslin 空间中，每个 Borel 集合都是 Souslin 集合（GT、IX, §6, No. 3、命题 11）。
(4) 更一般地，如果$f : X \to Y$是Souslin空间之间的连续双射，则$\mu \mapsto f(\mu)$是X上有界测度集合到Y上有界测度集合的双射映射（§ 2, No. 4，命题9）。

### 1. 紧凑空间和逆极限的补集

#### 命题 1 {#int-ix-s4-prop-1 .statement tag=09QM}

— 令 X 和 Y 为两个拓扑空间，f 为 Y 中 X 的连续映射。 设$(K_\alpha)_{\alpha \in A}$是X的紧子集的递减有向族，其中交 K。 然后$f(K) = \bigcap_{\alpha \in A} f(K_\alpha)$。

对于，令 y 为 $\bigcap_{\alpha \in A} f(K_\alpha)$ 的点；对于每个 $\alpha \in A$，集合 $L_\alpha = K_\alpha \cap f^{-1}(y)$ 都是紧凑的且非空。族$(L_\alpha)_{\alpha \in A}$是向下的，因此它的交L是非空。现在，$L = K \cap f^{-1}(y)$，从而$y \in f(K)$。这样我们就证明了包含$f(K) \supset \bigcap_{\alpha \in A} f(K_\alpha)$，并且逆包含是显而易见的。

#### 命题 2 {#int-ix-s4-prop-2 .statement tag=09QN}

— 给定由I索引的拓扑空间的逆系$(T_i, p_{ij})$、拓扑空间T，以及连续映射$p_i : T \to T_i$的连贯且分离的族。然后：

a) 对于 T 的每个紧凑子集 K，都有 $K = \bigcap_{i \in I} p_i^{-1}(p_i(K))$。

b) 令K和L是T的两个不相交的紧凑子集。存在一个$i \in I$使得$p_j(K)$和$p_j(L)$对于$j \geq i$来说是不相交的。

a) 令x为$\bigcap_{i \in I} p_i^{-1}(p_i(K))$的点；对于 K 中点 y 的每个 $i \in I$、集合 $K_i$，使得 $p_i(y) = p_i(x)$ 是 K 的非空闭子集。对于 $i \leq j$，我们有 $K_i \supset K_j$，并且，由于 K 是紧致的，集合因此$\bigcap_{i \in I} K_i$是非空。令y为$\bigcap_{i \in I} K_i$的点；对于所有 $i \in I$、从而 $y = x$，我们有 $y \in K$ 和 $p_i(y) = p_i(x)$；最后，$x \in K$，证明包含$K \supset \bigcap_{i \in I} p_i^{-1}(p_i(K))$；反向包含是显而易见的。

b) 对于每个$i \in I$，集合$M_i = p_i^{-1}(p_i(K)) \cap L$；这是紧凑空间 L 的闭子集，我们有 $M_i \supset M_j$ $i \leq j$，并且，通过 a)，

$$
\bigcap_{i \in I} M_i = K \cap L = \varnothing.
$$

因而，存在指标 i 使得$M_i = \varnothing$。对于$j \geq i$，我们有$p_j^{-1}(p_j(K)) \cap L = M_j \subset M_i = \varnothing$，从而$p_j(K) \cap p_j(L) = \varnothing$。

### 2. 逆系措施

#### 定义 1 {#int-ix-s4-def-1 .statement tag=09QO}

— 令 $\mathscr{T} = (T_i, p_{ij})$ 为由 I 索引的拓扑空间的逆系。 我们将$\mathscr{T}$上的测度称为$(\mu_i)_{i \in I}$的逆系（或子逆系统），其中$\mu_i$是所有$i \in I$在$T_i$上的有界测度，并且其中$\mu_i = p_{ij}(\mu_j)$（或$\mu_i \geq p_{ij}(\mu_j)$）对于$i \leq j$。

#### 命题 3 {#int-ix-s4-prop-3 .statement tag=09QP}

*给定由$I$索引的拓扑空间$\mathscr{T} = (T_i, p_{ij})$的逆系，拓扑空间$T$，连续映射$p_i : T \to T_i$（对于$i \in I$）的相干且分离的族以及子逆系统$(\mu_i)_{i \in I}$ $\mathscr{T}$ 的措施。对于 $T$、集合* 的每个紧凑型子集 K

$$
J(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K)).
$$

*那么$T$上存在一个有界测度$\pi$，并且只有一个，这样对于$T$的每个紧致子集$K$都有$\pi^\bullet(K) = J(K)$。一个人对所有 $i \in I$ 都有 $\mu_i \geq p_i(\pi)$，而 $\pi$ 是 $T$ 满足这个条件的最大的度量。*

让我们首先证明$J(K)$相对于有向预序集合$I$的截面过滤器$\mathfrak{F}$来说是$\mu_i^\bullet((p_i(K)))$的极限：为此，只需（GT，IV, §5, No. 2，Th.2）即可证明$\mu_i^\bullet(p_i(K)) \geq \mu_j^\bullet(p_j(K))$对于$i \leq j$；现在，设定$\mu_{ij}' = p_{ij}(\mu_j)$，我们有$\mu_{ij}' \leq \mu_i$和$p_j(K) \subset \overline{p_{ij}}^{-1}(p_i(K))$，从而

$$
\mu_j^\bullet(p_j(K)) \leq \mu_j^\bullet(\overline{p_{ij}}^{-1}(p_i(K))) = (\mu_{ij}')^\bullet(p_i(K)) \leq \mu_i^\bullet(p_i(K)).
$$

现在我们来研究函数$J$的性质：
1) 显然，当$K \subset L$时，$J(K) \leq J(L)$。
2) 设$K$和$L$是$T$的两个紧凑的子集。对于每个$i \in I$，我们有$p_i(K \cup L) = p_i(K) \cup p_i(L)$，从而

$$
\mu_i^\bullet(p_i(K \cup L)) \leq \mu_i^\bullet(p_i(K)) + \mu_i^\bullet(p_i(L));
$$

对于过滤器$\mathfrak{F}$，从经过到极限，我们得到$J(K \cup L) \leq J(K) + J(L)$。
3) 假设紧集$K$和$L$是不相交的。根据No. 1的命题2，存在$i \in I$使得$p_j(K) \cap p_j(L) = \varnothing$对应$j \geq i$。因此对于 $j \geq i$ 我们有

$$
\mu_j^\bullet(p_j(K \cup L)) = \mu_j^\bullet(p_j(K)) + \mu_j^\bullet(p_j(L)),
$$

相对于过滤器 $\mathfrak{F}$，从而 $J(K \cup L) = J(K) + J(L)$ 在经过到极限上。
4) 设$(K_\alpha)_{\alpha \in A}$是$T$的紧子集的递减有向族，其中交$K$。根据No. 1第1号提案，$p_i(K) = \bigcap_{\alpha \in A} p_i(K_\alpha)$，因此$\mu_i^\bullet(p_i(K)) = \inf_{\alpha \in A} \mu_i^\bullet(p_i(K_\alpha))$适用于所有$i \in I$（§ 1, No. 6，第5号提案的Cor.）。由此，可推知
$$
J(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K)) = \inf_{i \in I} \inf_{\alpha \in A} \mu_i^\bullet(p_i(K_\alpha))
= \inf_{\alpha \in A} \inf_{i \in I} \mu_i^\bullet(p_i(K_\alpha)) = \inf_{\alpha \in A} J(K_\alpha).
$$
5) 让我们选择、$i \in I$和集合$c = \mu_i^\bullet(T_i)$。那么$c$是有限的，$J(K) \leq \mu_i^\bullet(p_i(K)) \leq \mu_i^\bullet(T_i)$，因此$J(K) \leq c$对于$T$中的每个紧集$K$。

上述性质允许应用 Th。 § 3, No. 1 中的 1 个；我们结论在$T$上存在一个且仅有一个有界测度$\pi$，使得$\pi^\bullet(K) = J(K)$对于$T$的每个紧凑子集$K$。对于每个$i \in I$，让我们用$\nu_i$表示$T_i$上的度量，即$\pi$在$p_i$下的像。设$i \in I$、$A$是$T_i$的紧致子集，以及$\mathscr{L}$集合是$\overline{p_i^{-1}(A)}$的紧致子集。到 § 1, No. 2 的注 3 时，我们有 $\pi^\bullet(\overline{p_i^{-1}(A)}) = \sup_{K \in \mathscr{L}} \pi^\bullet(K)$；此外，$\nu_i^\bullet(A) = \pi^\bullet(\overline{p_i^{-1}(A)})$和$J(K) = \pi^\bullet(K)$对应$K \in \mathscr{L}$、从而$\nu_i^\bullet(A) = \sup_{K \in \mathscr{L}} J(K)$。

对于$K \in \mathscr{L}$，我们有$p_i(K) \subset A$、从而、$J(K) \leq \mu_i^\bullet(p_i(K)) \leq \mu_i^\bullet(A)$，最后是$\nu_i^\bullet(A) \leq \mu_i^\bullet(A)$。由于$A$是$T_i$中的任意紧集，因此我们结论即$\nu_i \leq \mu_i$。 命题的最后一个断言是显而易见的。

Q.E.D.

#### 定理 1（普罗霍罗夫）{#int-ix-s4-thm-1 .statement tag=09QQ}

— *让$\mathscr{T} = (T_i, p_{ij})$是拓扑空间的逆系，由$I$索引，$T$拓扑空间和$(p_i)_{i \in I}$连续映射$p_i : T \to T_i$的连贯且分离的族。最后，令 $(\mu_i)_{i \in I}$ 为 $\mathscr{T}$ 上的措施的逆系。

为了在$T$上存在有界测度$\mu$，使得$p_i(\mu) = \mu_i$对于所有$i \in I$，满足以下条件是必要且充分的：

(P) *对于每个$\varepsilon > 0$，都存在$T$的紧凑子集$K$，使得$\mu_i^\bullet(T_i - p_i(K)) \leq \varepsilon$对于所有$i \in I$。

当这种情况发生时，测度 $\mu$ 是唯一确定的并且*
$$
\mu^\bullet(K) = \inf_i \mu_i^\bullet(p_i(K))
$$
*对于$T$中的每个紧集$K$*。

我们首先证明$\mu$的唯一性。令 $\mu$ 为 $T$ 上的有界测度，使得 $p_i(\mu) = \mu_i$ 对于所有 $i \in I$。设$K$是$T$的紧子集；根据No. 1的第2号提案，集合$K$是递减的交定向家庭$(\overline{p_i^{-1}(p_i(K))})_{i \in I}$的*封闭*子集的$T$。由科。根据 § 1, No. 6 的第 5 条命题，我们有
$$
\mu^\bullet(K) = \inf_{i \in I} \mu^\bullet(\overline{p_i^{-1}(p_i(K))}) = \inf_{i \in I} \mu_i^\bullet(p_i(K)),
$$

从而建立公式 (2)。由于紧集的集合上的重合的两个度量相等（§ 1, No. 2，Prop. 2 的 Cor.），因此 $\mu$ 是唯一的。

根据命题 3，在 $T$ 上存在有界测度$\pi$，使得$\pi^\bullet(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K))$ 对于$T$ 的每个紧凑子集 $K$。根据公式 (2)，$T$ 上存在有界测度 $\mu$，因此对于所有 $i \in I$，$p_i(\mu) = \mu_i$ 等价于关系：

(P') $p_i(\pi) = \mu_i$ 对于所有 $i \in I$。

对于$i \leq j$，我们有$\mu_i = p_{ij}(\mu_j)$，从而$\mu_i^\bullet(T_i) = \mu_j^\bullet(T_j)$；由于$I$是有向的，因此存在有限的数$c \geq 0$，使得$\mu_i^\bullet(T_i) = c$对于所有$i \in I$。根据命题 3，测度 $\mu_i - p_i(\pi)$ 为正，因此当且仅当其总质量为零，即 $\mu_i(T_i) = p_i(\pi)^\bullet(T_i)$ 时，它才是零。由于 $p_i(\pi)^\bullet(T_i) = \pi^\bullet(T)$，条件 (P') 因此等价于 $\pi^\bullet(T) = c$，即 (§ 1, No. 2，注 3) 到性质：

(P'') $\sup_{K \in \mathscr{K}} \pi^\bullet(K) = c$，其中$\mathscr{K}$是$T$的紧致子集的集合。

现在，对于 $K \in \mathscr{K}$，我们有

$$
\pi^\bullet(K) = \inf_{i \in I} \mu_i^\bullet(p_i(K)) = c - \sup_{i \in I} \mu_i^\bullet(T_i - p_i(K))
$$

这个公式立即隐含了(P)和(P'')的等价。

Q.E.D.

令$(T_i, p_{ij})$为拓扑空间的逆系。 集合$T = \lim_{\leftarrow} T_i$并用$T$的$p_i$典范映射表示为$T_i$。概括 Def。第 2 章。 III, § 4, No. 5，我们可以说，$T$上的有界测度$\mu$是逆系*$(\mu_i)_{i \in I}$*测度*的*逆极限，如果$\mu_i = p_i(\mu)$对于所有$i \in I$来说。 Th。 1 提供了逆极限措施存在的标准。当空间 $T_i$ 是*紧致*，并且映射 $p_{ij}$ 满射时，$T$ 是紧致的，并且对于每个 $i \in I$ 是$p_i(T) = T_i$；因此，条件 (P) 得到满足，在这种情况下，我们恢复第 8 章的命题 8 (iv)。 III, § 4, No. 5。

#### 注 {#int-ix-s4-n2-rem-1 .statement tag=09QR}

— 设$(\mu_i)_{i \in I}$为空间$\mathscr{T} = (T_i, p_{ij})$中逆系的措施的逆系。假设给定拓扑空间$T'$和连续映射$p'_i : T' \to T_i$；假设家庭$(p'_i)_{i \in I}$是连贯的，但不一定是分离的。 *如果普罗霍罗夫的条件（P）被家庭满足*$(p'_i)_{i \in I}$，*存在一个措施*$\mu'$（*不一定唯一*）*在*$T'$*使得*$p'_i(\mu') = \mu_i$*对于所有人*$i \in I$。

对于，集合$T = \lim_{\leftarrow} T_i$和$p' = (p'_i)_{i \in I}$，并用$T$的$p_i$典范映射表示为$T_i$； Prokhorov 的条件由 $T$ 和 $p_i$ 满足，因为对于 $T'$ 的每个紧致子集 $K'$，$p_i(p'(K')) = p'_i(K')$ 和 $p'(K')$ 在 $T$ 中是紧致的。由 Th. 1，在$T$上存在有界测度$\mu$，使得$p_i(\mu) = \mu_i$对于所有$i \in I$。令$T'$中的$K'$为紧集；然后$\mu^\bullet(p'(K')) = \inf_{i \in I} \mu_i^\bullet(p'_i(K'))$，从而
$$
\mu^\bullet(T - p'(K')) = \sup_{i \in I} \mu_i^\bullet(T_i - p_i'(K')).
$$
让$\varepsilon > 0$；由于普罗霍罗夫的条件 (P) 满足$p_i'$，因此可以找到$T'$的紧凑子集$K'$，使得$\mu^\bullet(T - p'(K')) \leq \varepsilon$。然后，§2, No. 4 的第 8 条命题证明，对于所有 $i \in I$，$T'$ 上存在有界测度$\mu'$，其中$\mu = p'(\mu')$、从而 $\mu_i = p_i(\mu) = p_i(p'(\mu')) = p_i'(\mu')$。

### 3.可数逆系的情况

#### 定理 2 {#int-ix-s4-thm-2 .statement tag=09QS}

— *假设有向预序集合I有一个可数的共尾子集。令$\mathscr{T} = (T_i, p_{ij})$为拓扑空间、$T = \lim_{\leftarrow} T_i$和$T$的$p_i$典范映射到$T_i$的逆系。那么$\mathscr{T}$上的每逆系$(\mu_i)_{i \in I}$措施都承认逆极限。*

我们首先处理$I = \mathbf{N}$和集合$q_n = p_{n,n+1}$的情况。让$\varepsilon > 0$。 定义递归紧集$L_n \subset T_n$的序列如下：$L_0$是$T_0$的紧凑子集使得$\mu_0^\bullet(T_0 - L_0) \leq \varepsilon/2$，并且对于$n \geq 0$紧集$L_{n+1}$包含在$\overline{q_n^{-1}(L_n)}$ 且满足
$$
\mu_{n+1}^\bullet(\overline{q_n^{-1}(L_n)} - L_{n+1}) \leq \varepsilon/2^{n+2}.
$$
这个构造可以凭借§1, No. 2的*注3*来实现。我们有
$$
\begin{align*}
\mu_{n+1}^\bullet(T_{n+1} - L_{n+1}) &= \mu_{n+1}^\bullet(T_{n+1} - \overline{q_n^{-1}(L_n)}) + \mu_{n+1}^\bullet(\overline{q_n^{-1}(L_n)} - L_{n+1}) \\
&\leq \mu_{n+1}^\bullet(T_{n+1} - \overline{q_n^{-1}(L_n)}) + \varepsilon/2^{n+2} \\
&= \mu_n^\bullet(T_n - L_n) + \varepsilon/2^{n+2}
\end{align*}
$$
因为$\mu_n = q_n(\mu_{n+1})$；由归纳于 $p$ 推出
$$
\mu_p^\bullet(T_p - L_p) \leq \varepsilon(1 - 1/2^{p+1}) \leq \varepsilon.
$$
由于$T$是$\prod_{n \in \mathbf{N}} T_n$的闭子空间且乘积空间$\prod_{n \in \mathbf{N}} L_n$是紧的，因此$T$的子集$L = T \cap \prod_{n \in \mathbf{N}} L_n = \bigcap_{n \in \mathbf{N}} \overline{p_n^{-1}(L_n)}$是紧的。设 $n \in \mathbf{N}$；我们有 $p_n(L) = \bigcap_{m \geq n} p_{nm}(L_m)$（GT、I, §9, No. 6、第 8 条）和 $p_{nm}(L_m) \supset p_{nm'}(L_{m'})$ $m' \geq m \geq n$、从而
$$
\mu_n^\bullet(T_n - p_n(L)) = \lim_{m \to \infty} \mu_n^\bullet(T_n - p_{nm}(L_m)).
$$

但是，对于 $m \geq n$，度量 $\mu_n$ 是$p_{nm}$、从而下 $\mu_m$ 的像

$$
\mu_n^\bullet(T_n - p_{nm}(L_m)) = \mu_m^\bullet(T_m - \overline{p}_{nm}(p_{nm}(L_m))) \leq \mu_m^\bullet(T_m - L_m) \leq \varepsilon;
$$

对于$m$，经过到极限，我们得到$\mu_n^\bullet(T_n - p_n(L)) \leq \varepsilon$。在其他字中，满足普罗霍罗夫的条件（P），并且在$T$上存在有界测度$\mu$，使得$\mu_n = p_n(\mu)$对于所有$n \in \mathbf{N}$（No. 2，Th.1）。

让我们转向一般情况：存在于 $I$ 递增 cofinal 序列 $(i_n)_{n \in \mathbf{N}}$。 映射 $t \mapsto (p_{i_n}(t))_{n \in \mathbf{N}}$ 是 $T$ 到逆系 $(T_{i_n}, p_{i_n i_m})$ 的逆极限的同胚（GT，I, §4, No. 4）。因此，到证明的第一个部分，$T$上存在有界测度$\mu$，使得$\mu_{i_n} = p_{i_n}(\mu)$适用于所有$n \in \mathbf{N}$。让$i \in I$；存在 $n \in \mathbf{N}$ 与 $i \leq i_n$、从而

$$
p_i(\mu) = p_{i i_n}(p_{i_n}(\mu)) = p_{i i_n}(\mu_{i_n}) = \mu_i.
$$

Q.E.D.

定理 2 常用于以下情况：令$D$为可数集合，且$(X_t)_{t \in D}$为拓扑族空间。令 $\mathfrak{F}$ 为 $D$ 的有限子集的集合，按包含排序。对于$\mathfrak{F}$中的$J$，集合$X_J = \prod_{t \in J} X_t$，对于$J \subset J'$，让$p_{JJ'}$是$X_{J'}$到部分乘积$X_J$的规范投影。还有集合$X = \prod_{t \in D} X_t$，并用$p_J$表示$X$的规范投影到部分乘积$X_J$。很容易证明（cf. S，III, §7, No. 2，注 3）族$(p_J)_{J \in \mathfrak{F}}$定义是$X$到$\lim_{\leftarrow} X_J$的同胚。 逆系的测度是 $X_J$ 上的一系列有界测度$\mu_J$，使得 $\mu_J = p_{JJ'}(\mu_{J'})$ 对应于 $J \subset J'$。在$X$上存在且仅有一个有界测度$\mu$，使得$D$的每一个有限子集$J$都有$\mu_J = p_J(\mu)$（*柯尔莫戈洛夫的定理*）。其中一个有时表示 $\mu$ 是 $\prod_{t \in D} X_t$ 的度量，具有*边距* $\mu_J$。

特别是，假设对于每个 $t \in D$，在总质量 1 的 $X_t$ 上测量$\nu_t$。对于 $D$ 的每有限子集 $J$，集合 $\mu_J = \bigotimes_{t \in J} \nu_t$。令$J \subset J'$为$D$的两个有限子集，并令$K = J' - J$；将 $X_{J'}$ 与 $X_J \times X_K$ 等价，则有 $\mu_{J'} = \mu_J \otimes \mu_K$，并且由于 $\mu_K$ 的总质量为 1，因此 $X_J$ 上的 $\mu_J \otimes \mu_K$ 的投影等于 $\mu_J$。 $X$ 承认边际 $\mu_J$ 的措施表示为 $\bigotimes_{t \in D} \nu_t$，称为家庭*乘积* $(\nu_t)_{t \in D}$。当空间 $X_t$ 紧凑时，我们恢复 Ch 的构造。 III, §4, No. 6。

### 习题{#int-ix-s4-exercises}

§ 4](exercises/s4/)参见[习题。
