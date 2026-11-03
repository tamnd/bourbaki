---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 11
section_title: Grothendieck Groups
lang: zh
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.183-A VIII.210
pdf_pages: 0200-0227
extraction: native+ocr
subsections:
    - "no": 1
      title: Additive Functions of Modules
      page: 183
      pdf_page: 200
    - "no": 2
      title: The Grothendieck Group of an Additive Set of Modules
      page: 186
      pdf_page: 203
    - "no": 3
      title: Using Composition Series
      page: 189
      pdf_page: 206
    - "no": 4
      title: The Grothendieck Group R(A)
      page: 191
      pdf_page: 208
    - "no": 5
      title: Change of Rings
      page: 193
      pdf_page: 210
    - "no": 6
      title: The Grothendieck Group $R_K(A)$
      page: 194
      pdf_page: 211
    - "no": 7
      title: Multiplicative Structure on $K(\mathscr{C})$
      page: 196
      pdf_page: 213
    - "no": 8
      title: The Grothendieck Group $K_0(A)$
      page: 199
      pdf_page: 216
    - "no": 9
      title: The Grothendieck Group $K_0(A)$ of an Artinian Ring
      page: 200
      pdf_page: 217
    - "no": 10
      title: Change of Rings for $K_0(A)$
      page: 201
      pdf_page: 218
    - "no": 11
      title: Frobenius Reciprocity
      page: 202
      pdf_page: 219
    - "no": 12
      title: The Case of Simple Rings
      page: 204
      pdf_page: 221
statements: 38
exercises: 14
content_sha256: d0672bb5b2b9cf03447f1eb07269f31e298f9d7363e7a03af3c7a51f1c92beaa
translated_from: content/en/alg/VIII/11_s11_grothendieck_groups.md
translation_method: google
source_content_sha256: 36f598ab1286cc2db64313213910bc17ed366890ee67021cf75eae8ae9f62c08
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: f923e4a085e313270157cbf7d70bcd35b9e911224c251f7b78c7928185b1e776
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 11。 格罗滕迪克群

### 1. 加性函数 / 模

令A为环，令$\mathscr{C}$为A-模类集合(VIII，p. 51)；如果类属于到$\mathscr{C}$，我们说A-模是型$\mathscr{C}$。

#### 定义 1 {#alg-viii-s11-def-1 .statement tag=00CS}

我们说A-模类集合$\mathscr{C}$是相加的，如果每个零模是型$\mathscr{C}$和型$\mathscr{C}$两个模的直和是型$\mathscr{C}$。 We say that $\mathscr{C}$ is hereditary if it is additive and the submodules and quotient modules of a module of type $\mathscr{C}$ are of type $\mathscr{C}$.

#### 例 1 {#alg-viii-s11-n1-exa-1 .statement tag=00CT}

有限长度 A 模块的类集是遗传性的（II, §1, No. 10，p. 212，命题 16）。

#### 例 2 {#alg-viii-s11-n1-exa-2 .statement tag=00CU}

有限生成A-模类集合是相加的。如果环 A 是诺特，那么这个集合是遗传性的（VIII、p. 3、命题 3 和VIII、p. 7、命题 4）。

#### 例 3 {#alg-viii-s11-n1-exa-3 .statement tag=00CV}

有限生成射影A-模的类的集合是可加的，但通常不是遗传的。

#### 定义 2 {#alg-viii-s11-def-2 .statement tag=00CW}

设$\varphi$为映射，从$\mathscr{C}$到阿贝尔的群G（相加写）； 集合 $\varphi (E) =\varphi$(cl(E)) 对于型 $\mathscr{C}$ 的每 A-模 E。如果我们对每个正合序列（或每个分裂正合序列）有$\varphi (E) =\varphi (E') +\varphi (E'')$，我们说$\varphi$是模的加性函数（或模的弱可加函数）

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

模型 $\mathscr{C}$。

#### 例 4 {#alg-viii-s11-n1-exa-4 .statement tag=00CX}

设$\mathscr{C}$为有限长度A-模类集合。向其长度发送有限长度A-模类的映射$\operatorname{long}_A : \mathscr{C} \to \mathbf{Z}$是模加性函数(II, §1, No. 10、p. 213、推论3)。这个小节的结果是II, §1, No. 10、p. 212–214中建立的有限长度的模结果的推广。

在这个小节的剩余部分中，我们考虑A-模的加法集合$\mathscr{C}$以及从$\mathscr{C}$到阿贝尔的群$G$的添加剂映射$\varphi$。

令E和$E'$为型$\mathscr{C}$的模；那么$E \oplus E'$是型$\mathscr{C}$，并且存在分裂正合序列(II, §1, No. 9，p. 210)

$$
0 \longrightarrow E \longrightarrow E \oplus E' \longrightarrow E' \longrightarrow 0;
$$

由此，我们推论

(1)
$$
\varphi(E \oplus E') = \varphi(E) + \varphi(E').
$$

特别是，我们有$\varphi(0) = 0$。

#### 命题 1 {#alg-viii-s11-prop-1 .statement tag=00CY}

假设$\mathscr{C}$是遗传性的。令 E 和 F 为 A-模和 $u : E \to F$ 线性映射。
a) 如果 E 或 F 为型 $\mathscr{C}$，则 u 的像也为像。
b) 如果 E 是型 $\mathscr{C}$，那么 u 的核也是，并且我们有

(2)
$$
\varphi(E) = \varphi(\operatorname{Ker}\,u) + \varphi(\operatorname{Im}\,u).
$$

c) 如果 F 是 $\mathscr{C}$ 类型，那么 u 的 cokernel 也是这样，我们有

(3)
$$
\varphi(F) = \varphi(\operatorname{Im}\,u) + \varphi(\operatorname{Coker}\,u).
$$

命题由正合序列的存在推出

$$
0 \longrightarrow \operatorname{Ker}\,u \longrightarrow E \longrightarrow \operatorname{Im}\,u \longrightarrow 0,
$$
$$
0 \longrightarrow \operatorname{Im}\,u \longrightarrow F \longrightarrow \operatorname{Coker}\,u \longrightarrow 0.
$$

#### 推论 {#alg-viii-s11-n1-cor-1 .statement tag=00CZ}

设$(E_i)_{0 \leq i \leq n}$为型$\mathscr{C}$的模有限序列。如果存在正合序列

$$
0 \longrightarrow E_0 \xrightarrow{u_0} E_1 \xrightarrow{u_1} \cdots \xrightarrow{u_{n-1}} E_{n-1} \xrightarrow{u_n} E_n \longrightarrow 0,
$$

那么我们有

(4)
$$
\sum_{i=0}^n (-1)^i \varphi(E_i) = 0.
$$

让我们在$n$上用归纳证明推论；情况 $n= 0$ 和 $n= 1$ 是微不足道的。所以让$n\geqslant 1$，然后让

$$
0\longrightarrow E_0\longrightarrow^{u_0}E_1\longrightarrow  \cdots  \longrightarrow^{u_1}E_{n-1}\longrightarrow^{u_{n-1}}E_n\overset{u}{-}-\rightarrow^{^n}E_{n+1}\longrightarrow 0
$$

为型$\mathscr{C}$模正合序列。到命题 1 时，$u_n$ 的核 F 是型 $\mathscr{C}$ 的模，我们有

$$
\varphi (F) =\varphi (E_n)-\varphi (E_{n+1}) \tag{5}
$$

此外，我们还有正合序列

$$
0\longrightarrow E_0\longrightarrow E_1\longrightarrow E_2\longrightarrow  \cdots  \longrightarrow E_{n-1}\longrightarrow F\longrightarrow 0
$$

归纳假设给出关系

$$
\sum^{n-1}_{i=0}(-1)^i\varphi (E_i) + (-1)^n\varphi (F) = 0 \tag{6}
$$

然后我们立即从（5）和（6）推出$\sum^{n+1}_{i=0}(-1)^i\varphi (E_i) = 0$和推论。

#### 命题 2 {#alg-viii-s11-prop-2 .statement tag=00D0}

假设集合$\mathscr{C}$是遗传性的。设E为A-模，设M和N为E的子模。

a) 如果模 M 和 N 是型 $\mathscr{C}$，那么模 $M\cap N$ 和 M + N 也是，我们有

$$
\varphi (M + N) +\varphi (M\cap N) =\varphi (M) +\varphi (N)
$$

b) 如果模$E/M$和$E/N$是型$\mathscr{C}$，那么模$E/(M\cap N)$和$E/(M + N)$也是，我们有

$$
\varphi (E/(M + N)) +\varphi (E/(M\cap N)) =\varphi (E/M) +\varphi (E/N)
$$

断言 a) 和 b) 由正合序列的存在性推出

$$
0\rightarrow M\cap N\rightarrow M\oplus N\rightarrow M + N\rightarrow 0
$$

和

$$
0\rightarrow E/(M\cap N)\rightarrow (E/M)\oplus (E/N)\rightarrow E/(M + N)\rightarrow 0
$$

（II, §1, No. 7、p. 207、命题10）。

#### 命题 3 {#alg-viii-s11-prop-3 .statement tag=00D1}

假设$\mathscr{C}$是遗传性的。令 E 为型 $\mathscr{C}$ 的模和 E 的 $(E_i)_{0\leqslant i\leqslant n}$ 合成列 (I, §4, No. 7, p. 41)。对于 $1\leqslant i\leqslant n$，模 $E_{i-1}/E_i$ 是型 $\mathscr{C}$，我们有

$$
\varphi (E) =\sum_{i=1}^n\varphi (E_{i-1}/E_i)
$$

由于$\mathscr{C}$是遗传性的，模$E_0/E_1$和$E_1$是型$\mathscr{C}$，我们有$\varphi (E) =\varphi (E_0/E_1) +\varphi (E_1)$。由于序列$(E_{i+1})_{0\leqslant i\leqslant n-1}$是$E_1$中的合成列，命题3后面跟着$n$上的归纳。

### 2. 模加法集合格罗滕迪克群

设 A 为环。在这个小节中，我们考虑A-模的类的加法集合$\mathscr{C}$；我们认同$\mathscr{C}$与免费的阿贝尔的群$\mathbf{Z}^{(\mathscr{C})}$的典范基。对于任何正合序列

$$
(\mathscr{E})0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

型$\mathscr{C}$的模，我们用$\mathbf{Z}^{(\mathscr{C})}$的$r_{\mathscr{E}}$元素cl(E)$-$cl(E$'$)$-$cl(E$''$)来表示。令R为由形式$r_{\mathscr{E}}$的元素生成的$\mathbf{Z}^{(\mathscr{C})}$子群； 商群$\mathbf{Z}^{(\mathscr{C})}/R$称为$\mathscr{C}$的格罗滕迪克群，记为$K(\mathscr{C})$。对于型$\mathscr{C}$的模E，我们用$[E]_{\mathscr{C}}$表示$K(\mathscr{C})$中cl(E)的像（当$\mathscr{C}$存在歧义时，或有时[E]）。然后我们有以下泛性质。

#### 命题 4 {#alg-viii-s11-prop-4 .statement tag=00D2}

a) 映射 $E\mapsto [E]_{\mathscr{C}}$ 从 $\mathscr{C}$ 到 $K(\mathscr{C})$ 是相加的。

b) 令G为阿贝尔的群，并令$\varphi :\mathscr{C}\rightarrow G$为模的加性函数。存在唯一同态$u: K(\mathscr{C})\rightarrow G$，因此对于型$\mathscr{C}$的每个模E，我们都有$\varphi (E) =u([E]_{\mathscr{C}})$。

断言 a) 是显而易见的。让我们证明b)。存在同态 $u':\mathbf{Z}^{(\mathscr{C})}\rightarrow G$ 扩展 $\varphi$。由于$\varphi$是可加的，因此对于型$\mathscr{C}$的模的每个正合序列$(\mathscr{E})$，我们有$u'(r_{\mathscr{E}}) = 0$；因而，R包含在$u'$的核中。因而，当经过到商时，$u'$定义同态$u$从$K(\mathscr{C})$到G，很明显，对于型$\mathscr{C}$的每一个A-模，我们都有$\varphi (E) =u([E]_{\mathscr{C}})$。 群$K(\mathscr{C})$是由元素$[E]_{\mathscr{C}}$的集合生成，其中E经过$\mathscr{C}$；接下来是 $u$ 中的唯一性。

令$\mathscr{C}$和$\mathscr{D}$为加法集合或类或A-模，使得$\mathscr{C}\subset \mathscr{D}$。由于从n$\mathscr{C}$到格罗腾迪克群nK($\mathscr{D}$)的映射$E\mapsto [E]_{\mathscr{D}}$是可加的，因此存在同态$\gamma_{\mathscr{D},\mathscr{C}}: K(\mathscr{C})\rightarrow K(\mathscr{D})$，称为规范，其特征在于公式$\gamma_{\mathscr{D},\mathscr{C}}([E]_{\mathscr{C}}) = [E]_{\mathscr{D}}$对于型的每个模E $\mathscr{C}$。它并不总是单射的 (VIII, p. 210, 习题 13)。

#### 例 {#alg-viii-s11-n2-exa-1 .statement tag=00D3}

$*$ 令 A 为诺特交换环，并令 Σ 为其频谱。对于任何整数$n\geqslant 0$，用有限生成A-模的类的$\mathscr{C}^{\geqslant n}$集合表示，并支持Σ中的余维$\geqslant n$。 集合$K(n,A) =$$K(\mathscr{C}^{\geqslant n})$和$\gamma_n=\gamma_{\mathscr{C}^{\geqslant n},\mathscr{C}^{\geqslant n+1}}$。我们有序列 / 同态

$$
\gamma_n: K(n+ 1,A)\longrightarrow K(n,A)
$$

我们可以证明（AC，VIII, §1，n$^o5$，p. 13，命题 10）在$K(n,A)$，元素$[A/\mathfrak{p}]_{\mathscr{C}_n}$，其中$\mathfrak{p}$穿过高度Σ元素的集合 $\mathbf{Z}$模块的$n$、形式基是对$\gamma_n$的像的补充。更准确地说，对于型 $\mathscr{C}^{\geqslant n}$ 的每个模 E，我们有

$[E]_{\mathscr{C}^{\geqslant n}}\equiv \sum$长$_{A_{\mathfrak{p}}}(E_{\mathfrak{p}})\cdot [A/\mathfrak{p}]_{\mathscr{C}^{\geqslant n}}$（mod Im $\gamma_n$）$.*$

$\{\mathfrak{p}\in \Sigma |$ht($\mathfrak{p}$)$=n\}$

群$K(\mathscr{C})$是由形式$[E]_{\mathscr{C}}$的元素与$E\in \mathscr{C}$生成，并且我们有$[E\oplus E']_{\mathscr{C}}= [E]_{\mathscr{C}}+ [E']_{\mathscr{C}}$由关系(1)(VIII，p. 184)。因而，$K(\mathscr{C})$的每个元素都是形式$[E]_{\mathscr{C}}-[F]_{\mathscr{C}}$，其中E和F属于到$\mathscr{C}$。

如果形式$[E]_{\mathscr{C}}$对于型$\mathscr{C}$的A-模E，$K(\mathscr{C})$的元素被称为有效。 $K(\mathscr{C})$的有效元素的集合用$K(\mathscr{C})^+$表示； $K(\mathscr{C})$的子幺半群，$K(\mathscr{C})$可以与$K(\mathscr{C})^+$(I, §2, No. 4，p. 20)的差值群识别。

#### 命题 5 {#alg-viii-s11-prop-5 .statement tag=00D4}

令 E 和 F 为型 $\mathscr{C}$ 中的模。 等式 $[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$ 成立当且仅当存在型 $\mathscr{C}$ 模正合序列

$$
(\mathscr{E})0\longrightarrow L\longrightarrow P\longrightarrow M\longrightarrow 0
$$

$$
(\mathscr{F})0\longrightarrow L\longrightarrow Q\longrightarrow M\longrightarrow 0
$$

使得 $E\oplus Q$ 与 $F\oplus P$ 同构的。

指定的条件就足够了，因为它意味着关系

$$
[P]_{\mathscr{C}}= [L]_{\mathscr{C}}+[M]_{\mathscr{C}},[Q]_{\mathscr{C}}= [L]_{\mathscr{C}}+[M]_{\mathscr{C}},[E]_{\mathscr{C}}+[Q]_{\mathscr{C}}= [F]_{\mathscr{C}}+[P]_{\mathscr{C}}
$$

给出$[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$。

现在假设我们有$[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$。到群$K(\mathscr{C})$的构造，存在型$\mathscr{C}$的正合序列、模的两个有限族

$$
(\mathscr{G}_i)0\longrightarrow G'_i\longrightarrow G_i\longrightarrow G''_i\longrightarrow 0
$$

对于 $i\in I$ 和

$$
(\mathscr{H}_j)0\longrightarrow H'_j\longrightarrow H_j\longrightarrow H''_j\longrightarrow 0
$$

对于$j\in J$，这样在$\mathbf{Z}^{(\mathscr{C})}$，我们有

cl(E) $-$ cl(F) $=\sum_{j\in J}r_{\mathscr{H}_j}-\sum_{i\in I}r_{\mathscr{G}_i}$。

更明确地说，这个关系可以写成

(7) cl(E) $+\sum_{i\in I}$ cl(G$_i$) $+\sum_{j\in J}$ cl(H$'_j$) $+\sum_{j\in J}$ cl(H$''_j$)

= cl(F) $+\sum_{i\in I}$ cl(G$'_i$) $+\sum_{i\in I}$ cl(G$''_i$) $+\sum_{j\in J}$ cl(H$_j$)。

集合 $G =\bigoplus_{i\in I}G_i, G'=\bigoplus_{i\in I}G'_i$等，由经过到直和，我们得到正合序列

$(\mathscr{G})$ 0 // ${G'}^p$ // G $^q$ // $G''$ // $0$,

$(\mathscr{H})$ 0 // ${H'}^r$ // 高 $^s$ // $H''$ // 0

型$\mathscr{C}$模由……组成。

接下来，令$M_1, . . . ,M_m,N_1, . . . ,N_n$为型$\mathscr{C}$中的A-模。如果我们在群 $\mathbf{Z}^{(\mathscr{C})}$ 中有 $\sum^m_{i=1}$ cl(M$_i$) $=\sum^n_{j=1}$ cl(N$_j$)，那么我们有 $m=n$ 并且存在置换 $\sigma \in \mathfrak{S}_m$ 使得 cl(M$_i$) $=$每 $1\leqslant i\leqslant m$（I, §7, No. 9、p. 95、命题 11）有 cl(N$_{\sigma(i)}$)。因而，模$\bigoplus^m_{i=1}M_i$和$\bigoplus^n_{j=1}N_j$是同构的。特别是，从（7），我们从$E\oplus Q$到$F\oplus P$推出同构的存在性，其中有集合

$$
P = G'\oplus G''\oplus H,Q = G\oplus H'\oplus H''
$$

我们也集合

$$
L = G'\oplus H',M = G''\oplus H''
$$

模L、M、P、Q 为型$\mathscr{C}$、序列

$(\mathscr{E})$ 0 // L $^{\lambda}$ // P $^\mu$ // M // $0$,

我们定义 $\lambda$ 和 $\mu$

$$
\lambda (g', h') = (g',0, r(h')),\mu(g', g'', h) = (g'', s(h))
$$

是准确的。我们构造正合序列

$$
(\mathscr{F})0\longrightarrow L\longrightarrow Q\longrightarrow M\longrightarrow 0
$$

以同样的方式；这个结论证明。

集合 $\mathscr{C}$ 是合成 $(E,E')\mapsto$ cl(E$\oplus E'$) 的律的交换幺半群。 我们有时用 $K'(\mathscr{C})$ 表示交换幺半群 $\mathscr{C}$ (I, §2, No. 4, p. 20) 的差群，并称其为 $\mathscr{C}$ 的直和格洛腾迪克群。 对于型 $\mathscr{C}$ 的任意模 E，我们将 $K'(\mathscr{C})$ 中 cl(E) 的像表示为 $[E]'_{\mathscr{C}}$。

#### 命题 6 {#alg-viii-s11-prop-6 .statement tag=00D5}

a) 从$\mathscr{C}$到$K'(\mathscr{C})$的映射$E\mapsto [E]'_{\mathscr{C}}$是模中的弱可加函数。

b) 令G为阿贝尔的群，并令$\varphi :\mathscr{C}\rightarrow G$为模的弱可加函数。存在唯一群同态 $u: K'(\mathscr{C})\rightarrow$ G，这样对于型 $\mathscr{C}$ 的每个模 E，我们都有 $\varphi (E) =u([E]'_{\mathscr{C}})$。

c) 令 E 和 F 为型 $\mathscr{C}$ 中的模。我们有$[E]'_{\mathscr{C}}= [F]'_{\mathscr{C}}$当且仅当存在型$\mathscr{C}$的模M，使得$E\oplus M$同构于$F\oplus M$。

断言 a) 是显而易见的。 断言 b) 由 (I, §2, No. 4, p. 19, 定理 1) 得出，断言 c) 由 (I, §2, No. 4, p. 18, 命题 6) 得出。

由于从$\mathscr{C}$到$K(\mathscr{C})$的映射$E\mapsto [E]_{\mathscr{C}}$是模的弱可加函数，我们可以从中推导出同态$u: K'(\mathscr{C})\rightarrow K(\mathscr{C})$。这个同态是满射的，但并不总是同构 (VIII, p. 191, 注 2)。

令$R'$为由形式$r_{\mathscr{E}}$的元素生成的$\mathbf{Z}^{(\mathscr{C})}$的子群，其中$\mathscr{E}$为型$\mathscr{C}$的A-模的分裂正合序列，即形式 cl(E$'\oplus E''$)$-$ cl(E$'$)$-$ cl(E$''$)的元素，其中$E'$和$E''$是型的模 $\mathscr{C}$。 典范映射从$\mathscr{C}$到商群$\mathbf{Z}^{(\mathscr{C})}/R'$扩展到群同态$v: K'(\mathscr{C})\rightarrow \mathbf{Z}^{(\mathscr{C})}/R'$。这是同构。事实上，典范映射从$\mathscr{C}$到$K'(\mathscr{C})$扩展到群同态从$\mathbf{Z}^{(\mathscr{C})}$到$K'(\mathscr{C})$其核包含$R'$，因此到同态 $v':\mathbf{Z}^{(\mathscr{C})}/R'\rightarrow K'(\mathscr{C})$由经过至商；显然$v$和$v'$是逆双射。

如果形式$[E]'_{\mathscr{C}}$对于A-模E of 型$\mathscr{C}$，则$K'(\mathscr{C})$的元素被称为有效。 $K'(\mathscr{C})$的有效元素中的集合用$K'(\mathscr{C})^+$表示。

### 3. 利用合成序列

设 A 为环。令 E 为有限长度中的 A-模，S 单A-模。由与 S 同构的 E 的 Jordan-Hölder 级数的 Jordan-Hölder 定理 (I, §4, No. 7，p. 43，定理 6)，商的数不依赖于序列。我们用$\ell_S(E)$表示，并称其为E中S的重数。A-模E的支持度为单A-模S的类的集合，使得$\ell_S(E)\not= 0$。当E为半单且具有有限长度时，整数$\ell_S(E)$为型S(VIII，p. 72)的E的同型分量的长度[E:S]，并且概念的支持重合以及VIII、p. 66 中引入的支持。

#### 引理 1 {#alg-viii-s11-lem-1 .statement tag=00D6}

令 E、$E'$ 和 $E''$ 为有限长度中的 A-模，并且

0 // ${E'}^i$ // E $^p$ // $E''$ // 0

正合序列。我们有$\ell_S(E) =\ell_S(E') +\ell_S(E'')$。

令$\Sigma '$和$\Sigma ''$分别为$i(E')$和$E/i(E')$的Jordan–Hölder级数。存在 E 的 Jordan-Hölder 级数 Σ，其商的序列可以通过将 Σ 的商的序列与 $\Sigma '$ 的I, §4, No. 8，p. 44 并列得到。

#### 命题 7 {#alg-viii-s11-prop-7 .statement tag=00D7}

令$\mathscr{C}$为模的类的遗传集合，使得型$\mathscr{C}$的每个模都有有限长度。设$\mathscr{S}$为单模类属于到$\mathscr{C}$中的集合。那么$([S]_{\mathscr{C}})_{S\in\mathscr{S}}$族就是$\mathbf{Z}$模块$K(\mathscr{C})$的基，我们有

$$
[E]_{\mathscr{C}}=\sum_{S\in\mathscr{S}}\ell_S(E)[S]_{\mathscr{C}} \tag{8}
$$

对于型$\mathscr{C}$的每个模E。

公式 (8) 从应用于 E 的 Jordan–Hölder 级数的命题 3 得出。到引理 1，对于 $\mathscr{S}$ 的每个元素 S，存在从 $K(\mathscr{C})$ 到 $\mathbf{Z}$ 线性映射 $\varphi_S$ $\mathbf{Z}$使得$\varphi_S([E]_{\mathscr{C}}) =\ell_S(E)$对于型$\mathscr{C}$的每个模E。特别是，对于$\mathscr{S}$中的每个$S'\not= S$，我们都有$\varphi_S([S]_{\mathscr{C}}) = 1$和$\varphi_S([S']_{\mathscr{C}}) = 0$。由此可见，形式 $[S]_{\mathscr{C}}$（对于$S\in \mathscr{S}$）的元素与$\mathbf{Z}$线性无关；这些元素生成 $K(\mathscr{C})$ 公式 (8)。

#### 推论 {#alg-viii-s11-n3-cor-1 .statement tag=00D8}

令 E 和 F 为型 $\mathscr{C}$ 中的半单模。 模 E 同构于 F 当且仅当$K(\mathscr{C})$中有$[E]_{\mathscr{C}}= [F]_{\mathscr{C}}$。

事实上，对于 F，我们有 $[E]_{\mathscr{C}}=\sum_{S\in\mathscr{S}}\ell_S(E)[S]_{\mathscr{C}}$ 和类似的公式，并且当且仅当我们对每个$S\in \mathscr{S}$（VIII，p. 72）都有$\ell_S(E) =\ell_S(F)$时，E 与 F 同构。

#### 注 {#alg-viii-s11-n3-rem-1 .statement tag=00D9}

集合$K(\mathscr{C})^+$是$([S]_{\mathscr{C}})_{S\in\mathscr{S}}$家族生成的$K(\mathscr{C})$中的子幺半群。

### 4. 格罗滕迪克群R(A)

设A为环。 设$\mathscr{F}(A)$为有限生成A-模(VIII，p. 51)类的集合。 有限长度 A 模块的类形成 $\mathscr{F}(A)$ 的子集 $\mathscr{L}\mathscr{F}(A)$；我们已经看到 $\mathscr{L}\mathscr{F}(A)$ 是模块类的遗传集合。 我们用 R(A) 表示与 $\mathscr{L}\mathscr{F}(A)$ 相关的格罗滕迪克群，用 [E] 表示类、A-模 E、有限长度的 R(A) 中的像。

小节 3 的结果意味着：

a) 令 $\mathscr{S}(A)$ 为集合 / 类 / 单A-模。家族$([S])_{S\in\mathscr{S}(A)}$是$\mathbf{Z}$-模块R(A)的基。

b) 令 E 和 F 为有限长度的半单A-模。那么 E 和 F 是同构的当且仅当我们在 R(A) 中有 [E] = [F]。

c) 设 E 为有限长度的 A-模，$(E_i)_{0\leqslant i\leqslant n}$ E 的 Jordan–Hölder 级数。集合 $F =\bigoplus^n_{i=1}(E_{i-1}/E_i)$。那么 F 是有限长度的半单A-模，并且我们在 R(A) 中有 [E] = [F]。

d) 对于每个单A-模 S，令$\ell : R(A)\rightarrow \mathbf{Z}$ 为同态，其特征为$\ell ([S]) = 1$。然后，对于有限长度的每个A-模 E，我们有$\ell ([E]) =\sum_{S\in\mathscr{S}(A)}\ell_S(E) =$ long$_A(E)$。

如果 D 为域，则同态 $\ell : R(D)\rightarrow \mathbf{Z}$ 为同构。

#### 注 1 {#alg-viii-s11-n4-rem-1 .statement tag=00DA}

令$\mathscr{S}\mathscr{S}(A)$为类、半单A-模、有限长度的世袭集合。由 VIII、p. 190、格罗滕迪克群 $K(\mathscr{S}\mathscr{S}(A))$ 中的命题 7 组成，是一个免费的 $\mathbf{Z}$ 模块，其元素 $[S]_{\mathscr{S}\mathscr{S}(A)}$（对于 $S\in \mathscr{S}(A)$）形式基。因此，典范同态$\gamma_{\mathscr{L}\mathscr{F}(A),\mathscr{S}\mathscr{S}(A)}$（VIII，p. 186）为同构。

#### 注 2 {#alg-viii-s11-n4-rem-2 .statement tag=00DB}

对于直和 (VIII, p. 188)，令$K'(\mathscr{L}\mathscr{F}(A))$ 为$\mathscr{L}\mathscr{F}(A)$ 的格罗滕迪克群。 Krull–Remak–Schmidt 定理 (VIII, p. 37) 意味着 $K'(\mathscr{L}\mathscr{F}(A))$ 是一个自由 $\mathbf{Z}$ 模块，其中基集合为类不可分解 A-模为有限长度，而$K(\mathscr{L}\mathscr{F}(A))$承认单A-模的类中的集合为基。

#### 注 3 {#alg-viii-s11-n4-rem-3 .statement tag=00DC}

令 E 为有限长度的 A-模。根据c)，存在有限长度的半单A-模$E'$使得$[E] = [E']$，并且根据b)，这样的模被定义到同构；我们有时称其为E的半简化。

#### 命题 8 {#alg-viii-s11-prop-8 .statement tag=00DD}

令A为不是域的主理想整环，并令L为其分数的域。存在同构 $\varphi : R(A)\rightarrow L^*/A^*$ 使得我们有

$$
\varphi ([A/aA]) =aA^* \tag{9}
$$

对于 A 中的每个$a\not= 0$。

令P为A的不可约元的代表由……组成的系统(VII, §1, No. 3，p. 3)。 A 的最大理想是 $p\in P$ 的理想 $pA$；因而，每个单A-模都同构于唯一的模 $A/pA$。而且（VII, §1, No. 3，p. 4，定理2），阿贝尔的群$L^*/A^*$是免费的，并且有家人$(pA^*)_{p\in P}$为基。因而，从 R(A) 到 $L^*/A^*$，存在同构 $\varphi$，其特征在于，对于每个 $p\in P$，其特征为 $\varphi ([A/pA]) =pA^*$。

设 A 中存在 $a\not= 0$，P 存在整数 $r\geqslant 0$、元素 $p_1, . . . , p_r$，$A^*$ 存在元素 $u$，因此我们有 $a=up_1\cdots p_r$。 模 $A/aA$ 承认合成列定义为

$$
E_0= A/aA,E_i= (p_1\cdots p_iA)/aA(1\leqslant i\leqslant r)
$$

并且模$E_{i-1}/E_i= (p_1\cdots p_{i-1}A)/(p_1\cdots p_iA)$同构于$A/p_iA$。因此我们有 (VIII, p. 185, 命题 3)

$$
\varphi ([A/aA]) =\prod_{i=1}^r\varphi ([A/p_iA]) =p_1\cdots p_rA^*=aA^*
$$

#### 注 4 {#alg-viii-s11-n4-rem-4 .statement tag=00DE}

我们保留命题 8 的假设和记号。令E 为有限长度的A-模，并令$a_1A, . . . , a_nA$ 为其不变量因子（VII, §4, No. 5，p. 20）。由于 E 与 $\bigoplus_{i=1}^nA/a_iA$ 同构的，我们有

$$
\varphi ([E]) =\prod_{i=1}^n\varphi ([A/a_iA]) =a_1\cdots a_nA^* \tag{10}
$$

#### 注 5 {#alg-viii-s11-n4-rem-5 .statement tag=00SI}

设 A 是 Dedekind 环，但不是域（Comm. Alg.，VIII, §2, No. 1）。通过推理，如命题 8，我们可以证明从R(A)到群的A的分数理想存在同构$\varphi$，其特征为$\varphi ([A/\mathfrak{a}]) =\mathfrak{a}$对于每个非零的理想$\mathfrak{a}$ $A.*$

例如，在以下两种情况下将使用命题8：

a) 假设我们有 $A =\mathbf{Z}$。 有限长度的 $\mathbf{Z}$ 模就是有限的阿贝尔的群。由于 $\mathbf{Q}^*$ 是 $\mathbf{Z}^*=$ $\{1,-1\}$ 和 $\mathbf{Q}^*_+$ 的直接乘积，我们可以从命题 8 同构的 $\varphi '$ 推出，从 $R(\mathbf{Z})$ 到 $\mathbf{Q}^*_+$ 给出：

$\varphi '([G]) =$卡(G)

对于每个有限阿贝尔的群 G。

b) 假设 A 在一个变量 T 中为多项式环 K[T]，在交换域 K 中为系数。设 E 在 K 上为有限维向量空间，在 E 上为 $u$ 自同态。如VII, §5, No. 1、p. 29，表示为$E_u$ A-模以及底层加法群 E 和外法则 $(p, x)\mapsto p(u)x$。 A-模$E_u$有有限长度。相反，每个单A-模都是K上的有限维（VII, §4, No. 8，p. 25，注4）。因而，有限长度中的每个A-模都是K上的有限维，因此形式$E_u$。而且（VII, §5, No. 3，p. 32，推论 1），$E_u$的不变量因子的乘积等于$u$的特征多项式$\chi_u$。因而，命题 8 给出同构

$$
\varphi : R(K[T])\rightarrow K(T)^*/K^*
$$

其特征为 $\varphi ([E_u]) =\chi_uK^*$ (cf. 公式 (10))。

### 5. 变换 / 环

令A和B为环，并令$f: A\rightarrow B$为环同态。令$\mathscr{C}$为A-模中的加法集合，以及$\mathscr{D}$加法集合中B-模。

首先，假设对于型$\mathscr{D}$的每个B-模M，通过将标量环限制为A而获得的A-模$f_*(M)$为型$\mathscr{C}$。那么发送M到$[f_*(M)]_{\mathscr{C}}$的从$\mathscr{D}$到$K(\mathscr{C})$的映射就是模的加性函数；由此，我们推导出群同态

$$
f_*: K(\mathscr{D})\longrightarrow K(\mathscr{C})
$$

我们定义群同态$f_*: K'(\mathscr{D})\rightarrow K'(\mathscr{C})$同样。

现在我们假设对于型$\mathscr{C}$的每个A-模E，B-模$f^*(E)$通过$f$（II, §5, No. 1，p. 277）的标量扩张从E导出是型 $\mathscr{D}$。 映射从$\mathscr{C}$到$K'(\mathscr{D})$发送$\mathscr{C}$的元素E到$[f^*(E)]'_{\mathscr{D}}$是模弱可加函数；因此诱导群同态$f^*: K'(\mathscr{C})\rightarrow K'(\mathscr{D})$。

此外，假设对于每个正合序列

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

型$\mathscr{C}$A-模、型$\mathscr{D}$B-模序列

$$
0\longrightarrow B\otimes_AE'\longrightarrow B\otimes_AE\longrightarrow B\otimes_AE''\longrightarrow 0
$$

是准确的。这尤其适用于以下情况：

a) 同态 $f$ 使 B 成为射影 A-模 (II, §3, No. 6, p. 251, 命题 5 和 II, §3, No. 7, p. 257, 推论 $6$)$*$或, 更多

一般来说，平坦（X, §1，n$^o3$，p. 8，定义1）A-模$*$。

b) $*$集合 $\mathscr{C}$ 是射影类的集合，或者更一般地说，是平面 (X,

§4, n$^o5$, p. 72, 推论 2) A-模$*$。

然后将 E 发送到 $[f^*(E)]_{\mathscr{D}}$ 从 $\mathscr{C}$ 到 $K(\mathscr{D})$ 的映射是相加的。因此诱导群同态$f^*: K(\mathscr{C})\rightarrow K(\mathscr{D})$。

### 6. 格罗滕迪克群$R_K(A)$

设 K 为交换域，A K-代数。 K 上的有限维向量空间 A-模类集合是遗传的。 相应的格罗滕迪克群用$R_K(A)$表示。它是一个自由 $\mathbf{Z}$ 模块，其中基系列为 $([S])_{S\in\mathscr{S}}$，其中 $\mathscr{S}$ 是单A-模的类的集合，在 K 上是有限维的。存在同态

昏暗$: R_K(A)\longrightarrow \mathbf{Z}$

其特征在于，对于每个在 K 上有限维的 A-模 E，dim([E]) = [E : K]。当 A = K 时，它是同构。有效元素中的子幺半群用$R_K(A)^+$表示。

#### 引理 2 {#alg-viii-s11-lem-2 .statement tag=00DF}

设M和$M'$为A-模，且有限维向量空间超过K。M和$M'$的支持度(VIII，p. 190)为不相交的当且仅当存在$a\in A$使得$a_M= 0_M$且$a_{M'}= 1_{M'}$。

假设存在$a\in A$使得$a_M= 0_M$和$a_{M'}= 1_{M'}$。令 S 为单A-模。如果 cl(S) 属于到 M 的支持$\mathscr{S}_M$，则 A-模 S 同构于 M 的 Jordan–Hölder 级数的商之一，并且我们有 $a_S= 0_S$。同样，如果 cl(S) 属于到 M’ 的支持度 $\mathscr{S}_{M'}$，则我们有 $a_S= 1_S$。由此可见$\mathscr{S}_M$和$\mathscr{S}_{M'}$是不相交的。

相反，假设集合$\mathscr{S}_M$和$\mathscr{S}_{M'}$是不相交的。它们是有限的，因为 M 和 $M'$ 在 K 上是有限维的。每个单A-模 S 的类属于到 $\mathscr{S}_M\cup \mathscr{S}_{M'}$ 在 K 上是有限维的，并且更不必说在域 End$_A(S)$ 上是有限维的。通过命题 4 (VIII, p. 83) 中的推论 1，存在元素 $b\in A$，这样对于每个类的单A-模 S，我们都有 $b_S= 0_S$（或 $b_S= 1_S$） 属于至 $\mathscr{S}_M$（分别为 $\mathscr{S}_{M'}$）。令 $(M_i)_{0\leqslant i\leqslant n}$ 为 M 的 Jordan–Hölder 级数。通过上述，我们有 $bM_i\subset M_{i+1}$ 对应于 $0\leqslant i < n$，因此有 $(b^n)_M= 0_M$。同理证明自然数$m$的存在性$((1-b)^m)_{M'}= 0_{M'}$。 集合$P(X) = 1-(1-X^n)^m$和$a= P(b)$。多项式P(X)是$X^n$的倍数，所以我们有$a_M= 0_M$，而多项式$1-P(X)$是$(1-X)^m$的倍数，所以我们有$a_{M'}= 1_{M'}$。这个结论证明。

令L为K的扩张。如果M为A-模，即K上的有限维，则$M_{(L)}$是$A_{(L)}$模，即L上的有限维。此外，每正合序列

$$
0\longrightarrow M'\longrightarrow M\longrightarrow M''\longrightarrow 0
$$

A-模、序列 $A_{(L)}$ 模块

$$
0\longrightarrow M'_{(L)}\longrightarrow M_{(L)}\longrightarrow M''_{(L)}\longrightarrow 0
$$

由标量扩张推导出来是精确的（II, §7, No. 7、p. 308、命题 14）。因此，存在唯一的环同态 $u: R_K(A)\rightarrow$ $R_L(A_{(L)})$，使得对于 K (No. 5) 上的有限维的每个 A-模 M 都有 $u([M]) = [M_{(L)}]$。

#### 定理 1 {#alg-viii-s11-thm-1 .statement tag=00DG}

上面定义的同态$u: R_K(A)\rightarrow R_L(A_{(L)})$是单射的。设$\xi$为$R_K(A)$的元素。那么$\xi$有效当且仅当$u(\xi )$有效。

#### 引理 3 {#alg-viii-s11-lem-3 .statement tag=00DH}

令 S 和 T 为两个非同构单A-模，它们在 K 上是有限维的。$A_{(L)}$ 模 $S_{(L)}$ 和 $T_{(L)}$ 的支持是不相交的。

到引理 2，存在元素 $a\in A$，使得$a_S= 0$ 和$a_T= 1$。 $A_{(L)}$的元素$1\otimes a$在$S_{(L)}$上充当0，在$T_{(L)}$上充当1。到引理 2，$A_{(L)}$模块$S_{(L)}$和$T_{(L)}$的支持度为不相交的。

让我们证明定理 1。设$\mathscr{S}$是单A-模的类的集合，它们是K上的有限维。族$([S])_{S\in\mathscr{S}}$是$\mathbf{Z}$模$R_K(A)$的基。让$S\in \mathscr{S}$。 $A_{(L)}$-模块$S_{(L)}$不是零，所以它的支持不为空。令$S'$ 为该支持的元素。通过VIII、p. 190的引理 1，存在同态$f_{S'}: R_L(A_{(L)})\rightarrow \mathbf{Z}$，使得$f_{S'}([E]) =\ell_{S'}(E)$对于每个在L上有限维的$A_{(L)}$模E。我们有$f_{S'}([S_{(L)}])\not= 0$乘构造和$f([T_{(L)}]) = 0$对于每个$T\in \mathscr{S}-\{S\}$乘引理3。因此我们证明元素或$R_L(A_{(L)})$的形式$[S_{(L)}]$对于$S\in \mathscr{S}$是线性独立的$\mathbf{Z}$。由此可见同态 $u$ 是单射的。

令$S\in \mathscr{S}$，并令$S'$为$S_{(L)}$的支持度元素。对于每个$\xi \in R_K$(A)，基$([S])_{S\in\mathscr{S}}$中指标[S]的$\xi$的坐标是$f_{S'}(u(\xi ))/[S_{(L)}: S']$。由此可见，如果$u(\xi )$有效，那么$\xi$也有效。

### 7. 乘法结构于 $K(\mathscr{C})$

设 K 为交换环，A 为环 K 上的大数（III, §11, No. 4，p. 585），其中余积 $c$ 和余单位 $\gamma$。 除非另有说明，张量积超过 K。令 E 和 F 为（左）A-模。 张量积 $E\otimes F$ 具有$(A\otimes$ A)-模块结构，其特征在于公式

$$
(a\otimes b)(x\otimes y) =ax\otimes by \tag{11}
$$

对于$a, b\in A,x\in E$和$y\in F$。使用同态$c: A\rightarrow A\otimes A$，我们从这个$(A\otimes$A)-模块A-模$c_*(E\otimes F)$（II, §1, No. 13，p. 221）推导出来。更准确地说，令 $a\in A$；如果$c(a) =\sum_ia_i\otimes b_i$，那么我们有

$$
a(x\otimes y) =\sum_ia_ix\otimes b_iy \tag{12}
$$

对于 $x\in E$ 和 $y\in F$。通过滥用记号，我们也用$E\otimes F$表示所得的A-模。根据$c$的共结合性可以立即得出K-模的典范同构

$$
\varphi : (E\otimes F)\otimes G\longrightarrow E\otimes (F\otimes G)
$$

对于所有 A-模 E、F 和 G 都是 A 线性的。同样，如果大数 A 是可交换的，则从 $E\otimes F$ 到 $F\otimes E$ 的典范同构是 A 线性的。最后，令 $K_{\gamma}$ 为 A-模，基础为群 K 和外法则 $(a, x)\mapsto \gamma (a)x$。从$K\otimes E$（或$E\otimes K$）到E 的典范同构是从$K_{\gamma}\otimes E$（或$E\otimes K_{\gamma}$）到E 的A-模的同构。

#### 命题 9 {#alg-viii-s11-prop-9 .statement tag=00DI}

设 K 为交换环，A 为 K 上的大数，且有余单位 $\gamma$，以及 A-模的类的 $\mathscr{C}$ 加法集合，具有以下性质：

(i) 型 $\mathscr{C}$ 的每个 A-模都是射影 $(*$，或者更一般地，平坦$*)$ K-模。

(ii) 如果 A 模块 E 和 F 属于类型 $\mathscr{C}$，则 A 模块$E\otimes F$ 也是类型。

(iii) 上面定义的A-模$K_{\gamma}$为型$\mathscr{C}$。那么加法群$K(\mathscr{C})$上存在唯一的环结构，其乘法满足

$$
[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes F]_{\mathscr{C}}
$$

对于型 $\mathscr{C}$ 的所有 A-模 E 和 F。 $K(\mathscr{C})$的单位元是$[K_{\gamma}]_{\mathscr{C}}$。如果大数 A 是可交换的，则环 $K(\mathscr{C})$ 是可交换的。

赋予 $(E,F)\mapsto$ cl(E $\otimes F$) 给出的合成律，集合 $\mathscr{C}$ 是一个具有单位元 cl(K$_{\gamma}$) 的幺半群。因而，$\mathbf{Z}^{(\mathscr{C})}$ 典型地具有环的结构，且乘法的特征为公式

(13) cl(E) cl(F) = cl(E $\otimes F$)

和单位元 cl(K$_{\gamma}$) (III, §2, No. 6, p. 446)。

给定型 $\mathscr{C}$ 和正合序列的 A-模 F

$$
(\mathscr{E})0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

A-模型 $\mathscr{C}$, 序列

$$
(\mathscr{E}\otimes F)0\longrightarrow E'\otimes F\longrightarrow E\otimes F\longrightarrow E''\otimes F\longrightarrow 0
$$

从 $(\mathscr{E})$ 推导出来是精确的，因为 F 是投影 $(*$，或更一般地，在 K 上平坦$*)$（II, §3, No. 6、p. 251、命题 5 和II, §3, No. 7、p. 257、推论 6）。在 No. 2 的记号中，我们有

(14) $r_{\mathscr{E}\otimes F}=r_{\mathscr{E}}$ cl(F)。

由此可见，形式$r_{\mathscr{E}}$的元素生成$\mathbf{Z}^{(\mathscr{C})}$的子群R是环$\mathbf{Z}^{(\mathscr{C})}$的右理想，同样证明它是$\mathbf{Z}^{(\mathscr{C})}$的左理想。到定义时，$K(\mathscr{C})$ 为商群 $\mathbf{Z}^{(\mathscr{C})}/R$；因而，$K(\mathscr{C})$上存在唯一的环结构，对于型$\mathscr{C}$的所有A-模E和F，其乘法满足$[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes F]_{\mathscr{C}}$。它的单位元是$[K_{\gamma}]$。

当大数A可交换时，幺半群$\mathscr{C}$可交换；由此可知环 $\mathbf{Z}^{(\mathscr{C})}$ 和商环 $K(\mathscr{C})$ 是可交换的。

#### 注 {#alg-viii-s11-n7-rem-1 .statement tag=00DJ}

仅在命题 9 的假设 (i) 和 (ii) 下，直和 (VIII, p. 188) 的格罗滕迪克群 $K'(\mathscr{C})$ 具有唯一的环结构，其乘法满足$[E]'_{\mathscr{C}}[F]'_{\mathscr{C}}= [E\otimes F]'_{\mathscr{C}}$。它的单位元是$[K_{\gamma}]'_{\mathscr{C}}$。如果大数 A 是可交换的，则环 $K'(\mathscr{C})$ 是可交换的。 证明与命题 9类似，因为群$K'(\mathscr{C})$可以与$\mathbf{Z}^{(\mathscr{C})}/R'$识别，其中$R'$是由形式的元素生成的$\mathbf{Z}^{(\mathscr{C})}$的子群 cl(E$'\oplus E''$)$-$ cl(E$'$)$-$ cl(E$''$)（前述）。

在命题 9 的假设 (i)、(ii) 和(iii) 下，环 $K(\mathscr{C})$ 称为$\mathscr{C}$ 的格罗腾迪克环。特别是，当 K 为域且 $\mathscr{C}$ 为类或 A-模的集合时，这些条件得到满足，它们是 K 上的有限维。因而，我们有以下结果。

#### 推论 {#alg-viii-s11-n7-cor-1 .statement tag=00DK}

设A是余单位$\gamma$超过交换域K的大数，则加法群$R_K(A)$上存在唯一的环结构，其乘法满足

$$
[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes_KF]_{\mathscr{C}}
$$

对于所有在 K 上有限维的 A-模 E 和 F。 $R_K(A)$ 的单位元是 $[K_{\gamma}]_{\mathscr{C}}$。如果大数 A 是可交换的，则环 $R_K(A)$ 是可交换的。

#### 例 1 {#alg-viii-s11-n7-exa-1 .statement tag=00DL}

设 K 为交换域。令G为群，令K[G]为群G的代数。我们认同G及其典范像在K[G]中（III, §2, No. 6，p. 446）。

我们赋予 K[G] 一个大数的结构余积 $c$ 和余单位 $\gamma$ 给出：

$$
c(g) =g\otimes g ,\gamma (g) = 1(g\in G) \tag{15}
$$

设 E 和 F 为 K[G]-模；由公式 (12)，$E\otimes F$ 上的 K[G]-模块结构由下式给出

$$
g(x\otimes y) =gx\otimes gy(g\in G, x\in E, y\in F) \tag{16}
$$

K[G]-模$K_{\gamma}$是向量空间K，赋予G的作用，由$g\lambda =\lambda$为$g\in G$和$\lambda \in K$定义。

环$R_K(K[G])$也表示为$R_K(G)$。它是可交换的；它的乘法由$[E] [F] = [E\otimes_KF]$给出，$R_K(G)$的单位元是$[K_{\gamma}]$。

#### 例 2 {#alg-viii-s11-n7-exa-2 .statement tag=00DM}

令 $\mathfrak{g}$ 为李代数超过交换域 K，并且 $U(\mathfrak{g})$ 包络代数；我们认同$\mathfrak{g}$及其$U(\mathfrak{g}) ($谎言中的典范像、I, §2, No. 7、p. 39、推论2)。我们赋予$U(\mathfrak{g})$一个bigebra的结构，其中余积$c$和余单位$\gamma$给出：

$$
c(\xi ) =\xi \otimes 1 + 1\otimes \xi ,\gamma (\xi ) = 0 \tag{17}
$$

对于$\xi \in \mathfrak{g}($谎言，II, §1, No. 4，p. 115）。

设E和F为$U(\mathfrak{g}$)-模；由公式 (17) 可知，$E\otimes F$ 上的 $U(\mathfrak{g}$) 模块结构的特点是

$$
\xi (x\otimes y) =\xi x\otimes y+x\otimes \xi y \tag{18}
$$

对于 $\xi \in \mathfrak{g},x\in E$ 和 $y\in F$。

格洛腾迪克环$R_K(U(\mathfrak{g}))$在《谎言》、VIII,

§7, No. 6，第 17 页中也用 $\mathscr{R}(\mathfrak{g})$ 表示。 $139.*$

设 A 为交换环。我们可以将 A 视为一个与自身共交换的大数，其中余积从 A 到 $A\otimes_AA$ 的自然同构和余单位 Id$_A$ (III, §11, No. 4, p. 585)。到命题 9，我们得到以下结果。

#### 命题 10 {#alg-viii-s11-prop-10 .statement tag=00DN}

设A为交换环，设$\mathscr{C}$为A-模满足类加法集合以下三个条件：

(i) 型 $\mathscr{C}$ 中的每个 A-模都是投影 $(*$，或者更一般地说，是平坦的$*)$。

(ii) 如果E和F是型$\mathscr{C}$的A-模，那么A-模$E\otimes_AF$也是型$\mathscr{C}$。

(iii) A-模 A 为型 $\mathscr{C}$。

那么对于型$\mathscr{C}$的A-模的每个对E、F，在加法群$K(\mathscr{C})$满足$[E]_{\mathscr{C}}[F]_{\mathscr{C}}= [E\otimes_AF]_{\mathscr{C}}$上存在唯一的环结构。 $K(\mathscr{C})$中的单位元是$[A]_{\mathscr{C}}$。

### 8. 格罗滕迪克群$K_0(A)$

设 A 为环。有限生成射影A-模的类集合$\mathscr{P}(A)$是可加的；我们用$K_0(A)$表示格罗滕迪克群$K(\mathscr{P}(A))$。

对于合成 $(E,E')\mapsto$ cl(E $\oplus E'$) 的律，集合 $\mathscr{P}(A)$ 是可交换幺半群。此外，射影A-模的每正合序列

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

分裂的 (II, §2, No. 2, p. 231, 命题 4)，因而 E 与 $E'\oplus E''$ 同构。 映射$E\mapsto [E]$从$\mathscr{P}(A)$到$K_0(A)$，因此定义同构从群的幺半群$\mathscr{P}(A)$到$K_0(A)$（VIII，p. 188）的差异。

对于每个有限生成射影模 P，都存在有限生成射影模 $P'$，使得$P\oplus P'$ 是空闲的（II, §2, No. 2，p. 232，推出 1）。令 E 和 F 为有限生成射影 A-模；由I, §2, No. 4，p. 18，命题 6，当且仅当存在有限生成的自由A-模L，使得A-模$E\oplus L$和$F\oplus L$同构，我们在$K_0(A)$中有[E] = [F]。那么我们说 E 和 F 是稳定同构的；这并不一定意味着 E 和 F 是同构的（VIII、p. 207、习题 2 和 VIII、p. 210、习题 14）。

当环 A 可交换时，加法群 $K_0(A)$ 上存在交换环结构，其乘法的特征为公式 $[E]_{\mathscr{P}(A)}[F]_{\mathscr{P}(A)}= [E\otimes_AF]_{\mathscr{P}(A)}$ (VIII, p. 199, 命题 10）。

#### 注 {#alg-viii-s11-n8-rem-1 .statement tag=00DO}

设 A 为半单环。每个 A-模都是半单和射影 (VIII, p. 138, 命题 4)；因此我们有等式

$$
\mathscr{L}\mathscr{F}(A) =\mathscr{S}\mathscr{S}(A) =\mathscr{P}(A)
$$

（cf.No. 4对应于$\mathscr{L}\mathscr{F}(A)$和$\mathscr{S}\mathscr{S}(A)$中的定义）。因而，我们有 $K_0(A) = R(A)$ x 定义其中格罗滕迪克群。

#### 例 {#alg-viii-s11-n8-exa-1 .statement tag=00DP}

如果每个有限生成的射影A-模都是自由的，则从$K_0(A)$到$\mathbf{Z}$有秩定义同构。特别是当A为主理想整环（VII, §1, No. 3、p. 15、推论3）或A为局部环（VIII、p. 36、推论6）时的情况。

### 9. 格罗滕迪克群$K_0(A)$共阿廷环

设 A 为左阿廷的环。设$\mathfrak{r}$为其根基；它是A的幂幂双面理想，环$A/\mathfrak{r}$是半单（VIII，p. 173，命题1）。通过 VIII、p. 176、映射 $P\mapsto$ 的推论，cl(P$/\mathfrak{r}P$) 是从幺半群 $\mathscr{P}(A)$ 到幺半群 $\mathscr{P}(A/\mathfrak{r})$ 的同构。我们从中推导出群同构$\gamma$从$K_0(A)$到$K_0(A/\mathfrak{r})$，其特征为关系$\gamma ([P]_{\mathscr{P}(A)}) = [P/\mathfrak{r}P]_{\mathscr{P}(A/\mathfrak{r})}$，对于每个有限生成的射影A-模P。

由于环$A/\mathfrak{r}$是半单，所以上面的注意味着等式$R(A/\mathfrak{r}) = K_0(A/\mathfrak{r})$。 有限长度的模超过环$A/\mathfrak{r}$只是有限长度的半单模超过环A（VIII，p. 174，命题2）；因而，我们将可以确定$\mathscr{L}\mathscr{F}(A/\mathfrak{r})$与$\mathscr{S}\mathscr{S}(A)$以及$R(A/\mathfrak{r})$与$K(\mathscr{S}\mathscr{S}(A))$进行组合。我们用$\delta$同态$\gamma_{\mathscr{L}\mathscr{F}(A),\mathscr{S}\mathscr{S}(A)}$表示从$R(A/\mathfrak{r}) = K(\mathscr{S}\mathscr{S}(A))$到$R(A) = K(\mathscr{L}\mathscr{F}(A))$（VIII，p. 191，注1）；是同构。最后，我们有 $\mathscr{P}(A)\subset \mathscr{L}\mathscr{F}$(A)，还有集合 $\varepsilon =$ \gamma_{\mathscr{LF}(A),\mathscr{P}(A)}。我们定义了图表

$$
\begin{array}{ccc}
K_0(A) & \xrightarrow{\gamma} & K_0(A/\mathfrak{r}) = R(A/\mathfrak{r}) \\
& \searrow^{\varepsilon} & \swarrow^{\delta} \\
& & R(A).
\end{array}
$$

我们用$\mathscr{S}$表示单A-模的类的（有限）集合；对于 $\lambda \in \mathscr{S}$、选择模 $S_\lambda$ 类 $\lambda$ 以及投影覆盖$(P_\lambda, u_\lambda)$ $S_\lambda$ (VIII、p. 175、命题 4)。从 VIII、p. 176 的命题 6 可以得出，$K_0(A)$ 是一个免费的 $\mathbf{Z}$ 模块，与基系列$([P_\lambda]_{\mathscr{P}(A)})_{\lambda \in \mathscr{S}}$ 一起使用。此外，由于$S_\lambda$与$P_\lambda / \mathfrak{r} P_\lambda$（VIII，p. 176）同构，因此将$K_0(A)$的$\gamma$变换基$([P_\lambda]_{\mathscr{P}(A)})_{\lambda \in \mathscr{S}}$转化为基$([S_\lambda])_{\lambda \in \mathscr{S}}$ $R(A/\mathfrak{r})$。将$R(A/\mathfrak{r})$的同构$\delta$变换基$([S_\lambda])_{\lambda \in \mathscr{S}}$转换为$R(A)$的基$([S_\lambda])_{\lambda \in \mathscr{S}}$。

相对于$K_0(A)$的基$([P_\lambda]_{\mathscr{P}(A)})_{\lambda \in \mathscr{S}}$和$R(A)$的$([S_\lambda])_{\lambda \in \mathscr{S}}$，$A$的*嘉当矩阵*是$\mathbf{Z}$模$\varepsilon : K_0(A) \to R(A)$的同态的矩阵$(a_{\lambda \mu})$。到定义，我们已经

$$
[P_\mu] = \sum_{\lambda \in \mathscr{S}} a_{\lambda \mu} [S_\lambda] \qquad (\mu \in \mathscr{S})
$$

在群$R(A)$。 换句话说，$a_{\lambda \mu}$是A模$P_\mu$的Jordan-Hölder级数中与$S_\lambda$同构的商数。

集合$\pi = \varepsilon \circ \gamma^{-1} \circ \delta^{-1}$；它是群$R(A)$中的自同态。如果 M 是有限生成的半单A-模和 $(P, u)$ M 的射影覆盖，那么我们有 $\pi([M]) = [P]$。根据公式(19)，$\pi$的矩阵相对于$R(A)$的基$([S_\lambda])_{\lambda \in \mathscr{S}}$，简直就是$A$的嘉当矩阵。

### 10. $K_0(A)$ 的变换环

设 A 和 B 为环。设$f : A \to B$为环同态。如果 P 是有限生成的射影 A-模，则 B-模 $f^*(P) = B \otimes_A P$ 是射影且有限生成的 (II, §5, No. 2、p. 281、推论)。 映射$P \mapsto \operatorname{cl}(f^*(P))$是从幺半群$\mathscr{P}(A)$到幺半群$\mathscr{P}(B)$的同态，因此对于每个有限生成的射影A-模P，定义同态$f^* : K_0(A) \to K_0(B)$的特征在于关系$f^*([P]_{\mathscr{P}(A)}) = [f^*(P)]_{\mathscr{P}(B)}$。如果$g : B \to C$ 是第二个环同态，则从标量 (II, §5, No. 1、p. 278、命题 2) 的扩张的传递性得出同态 $(g\circ f)^*$ 和 $g^*\circ f^*$ $K_0(A)$ 到 $K_0(C)$ 相等。

假设$f$使B成为有限生成的射影左A-模。令 Q 为有限生成的射影左B-模。那么 Q 是有限生成的自由 B-模的直因子，该自由 B-模在 A 上投影且有限生成。因而，通过标量的限制从 Q 获得的 A-模 $f_*(Q)$ 是投影且有限生成的。如上所述，对于每个有限生成射影B-模 Q，我们推导出以关系 $f_*([Q]_{\mathscr{P}(B)}) = [f_*(Q)]_{\mathscr{P}(A)}$为特征的同态$f_*: K_0(B)\rightarrow K_0(A)$。如果$g: B\rightarrow C$是环同态，则C变成有限生成射影B-模，那么从$K_0(C)$到$K_0(A)$的同态$(g\circ f)_*$和$f_*\circ g_*$相等。

### 11. 弗罗贝尼乌斯互易律

设 A 为半单环。令$f$为从A到半单环B的同态。令S为单A-模和T单B-模，并令D和E分别为S和T的中心化器。根据 Schur 的引理（VIII、p. 47、推出），D 和 E 为域。令 H 为从 S 到 $f_*(T)$ 的 A 线性同态的集合。我们赋予 H 一个$(E$，D)-双模结构，其中外法则$(e, u)\mapsto e\circ u$和$(d, u)\mapsto u\circ d$代表$e\in E,u\in H$，$d\in D$。

#### 命题 11 {#alg-viii-s11-prop-11 .statement tag=00DQ}

a) 半单A-模 $f_*(T)$ 中单A-模 S 的重数 $[f_*(T) : S]$ 等于 H 的维数，视为 D 上的右向量空间。

b) 重数 $[f^*(S) : T]$ 是有限的，等于 H 的维数视为 E 上的左向量空间。

断言 a) 由VIII、p. 72 的公式 (11) 得出。

B-模 $f^*(S)$ 是半单并且是有限生成的，因此有有限长度。由 loc 的公式 (12) 完成。如上所述，我们有

（20）$[f^*(S) : T] =$昏暗$_E$坎$_B(f^*(S),T)$。

现在，在 II, §5, No. 1、p. 277–278、公式 (2) 和注 2 中，我们定义了从 Hom$_A(S, f_*(T))$ 到 Hom$_B(f^*(S),T)$ 的 E 线性双射。 断言 b) 然后从公式 (20) 得出。

#### 推出 (弗罗贝尼乌斯互易律) {#alg-viii-s11-n11-cor-1 .statement tag=00S7}

假设 A 和 B 是半单代数，它们是交换域 K 上的有限维，并且 $f$ 是 K 线性的。那么 K-向量空间 S、T、D、E 和 H 是有限维的，我们有等式

$$
[f_*(T) : S][D : K] = [f^*(S) : T][E : K] = [H : K] \tag{21}
$$

特别是，当 K 是代数闭集时，我们有 D = E = K 且

$$
[f_*(T) : S] = [f^*(S) : T] = [H : K] \tag{22}
$$

由于A-模 S 是简单的，因此它是单生的，并且 D 是 Hom$_K(S,S)$ 的线性子空间；因而，S 和 D 在 K 上是有限维的。出于类似的原因，T 和 E 在 K 上是有限维的。最后，H 是 Hom$_K(S,T)$ 的线性子空间；因此它也是有限维的。然后从命题 11 得出公式 (21)，因为 H 在 K 上的维数等于 [H : D][D : K] 和 [H : E][E : K] (II, §1, No. 13, p. 222, 命题 25)。通过 VIII 的定理 1，p. 47，如果 K 是代数封闭的，则我们有 D = E = K。 推论的第二个部分由第一个得出。

设 A 和 B 为半单代数，它们是交换域 K 上的有限维，并令 $f$ 为从 A 到 B 的 K-代数中的同态。

设$\mathscr{S}(A)$为单A-模类集合；对于每个 $\lambda \in \mathscr{S}$ (A)，令 $S_{\lambda}$ 为类 $\lambda$ 和 $D_{\lambda}$ 的居中器中的模。那么$D_{\lambda}$是K上有限次数的代数；我们用$d_{\lambda}$表示这个次数。我们对$\mathscr{S}(B)$中的$\mu$进行类似的定义$\mathscr{S}$(B)、$T_\mu$、$E_\mu$和$e_\mu$。 格罗滕迪克群 $K_0(A)$ 的家庭 $([S_{\lambda}])_{\lambda\in\mathscr{S}(A)}$ 为基，$K_0(B)$ 的 $([T_\mu])_{\mu\in\mathscr{S}(B)}$ 为基。对于这些基，令$(a_{\mu\lambda})$为$f^*: K_0(A)\rightarrow K_0(B)$的矩阵以及$f_*: K_0(B)\rightarrow K_0(A)$的$(b_{\lambda \mu})$矩阵。到定义，我们已经

$$
a_{\mu\lambda}= [f^*(S_{\lambda}) : T_\mu],b_{\lambda \mu}= [f_*(T_\mu) : S_{\lambda}] \tag{23}
$$

对于$\mathscr{S}(A)$中的$\lambda$和$\mathscr{S}(B)$中的$\mu$。我们用$h_{\lambda \mu}$表示向量空间Hom$_A(S_{\lambda}, f_*(T_\mu))$超过域K的维数。到上面推论，我们有

$$
h_{\lambda \mu}=e_\mu a_{\mu\lambda}=d_{\lambda}b_{\lambda \mu} \tag{24}
$$

当域 K 是代数闭时，我们有 $d_{\lambda}=e_\mu= 1$；因而，我们有

$$
a_{\mu\lambda}=b_{\lambda \mu}=h_{\lambda \mu} \tag{25}
$$

在其他字中，$f_*$和$f^*$的矩阵相对于给定的$K_0(A)$和$K_0(B)$的基来说是彼此的转置。

### 12. 单环的情形

令 A 和 B 为从 A 到 B 的简单环和 $f$ 同态。令 S 为单A-模且 T 单B-模。我们集合

(26)$i(f) = [f^*(S) : T] =$长$_B(f^*(S))$；

我们称$f$为基数$i(f)$指标。当A是B的子环并且$f$是A到B的典范嵌入时，我们写$i(B,A)$而不是$i(f)$，我们称其为A在B中的基数指标。我们类似地定义是$f$的高度$h(f)$：

（27）$h(f) = [f_*(T) : S] =$长$_A(f_*(T))$。

当A是B的子环并且B的$f$典范嵌入时，我们将$h(f)$写成$h(B,A)$，我们称其为A在B中的高度。

A-模 S 是单生的，因而 B-模 $f^*(S) = B\otimes_AS$ 也是单生的。由此可知 $i(f)$ 是有限的，因此它是整数。令 M 为 A-模。将其长度表示为$\mathfrak{a}$；则 M 同构于 $S^{(\mathfrak{a})}$。因而，B-模$f_*(M)$同构于$f_*(S)^{(\mathfrak{a})}$。到 $i(f)$ 的定义时，我们有

（28）长$_B(f^*(M)) =i(f)$长$_A(M)$。

$\mathbf{Z}$-模块$K_0(A)$和$K_0(B)$不含维数 1，分别具有基[S]和[T]，并且我们有

$$
f^*([S]) =i(f)[T] \tag{29}
$$

让我们特别考虑 $M = A_s$；那么 $f^*(A_s) = B\otimes_AA_s$ 与 $B_s$ 同构的 (II, §3, No. 4, p. 249)，所以

(30)$i(f) =$长(B)$/$长(A)。

根据 Wedderburn 的定理 (VIII, p. 120, 定理 1)，存在整数 $m\geqslant$ 1 和 $n\geqslant 1$ 和域 D 和 E，使得 A 与 $\mathbf{M}_m(D)$ 同构的，B 与$\mathbf{M}_n(E)$。到公式 (30) 时，我们有$i(f) =n/m$；特别是$m$除$n$。

令N为B-模；用 $\mathfrak{a}$ 表示其长度。那么N同构于$T^{(\mathfrak{a})}$，所以A-模$f_*(N)$同构于$f_*(T)^{(\mathfrak{a})}$；到定义或 $h(f)$，我们有

（31）长$_A(f_*(N)) =h(f)$长$_B(N)$。

我们已经看到（VIII，p. 124，命题 5），$f$将B变成自由A-模，并且这个模的所有基都有相同的基数，用$[B : A]_s$表示，称为（左） B 在 A 上的次数。 A-模 $f_*(B_s)$ 与 $A_s^{[B:A]_s}$ 同构的，因此有长度 $[B : A]_s$ long(A)。通过将公式 (30) 和公式 (31) 应用于特定情况$N = B_s$，我们有

$$
[B : A]_s=i(f)h(f) \tag{32}
$$

现在假设B是有限生成A-模，即$[B : A]_s$是有限的。那么 $h(f)$ 由公式 (32) 有限。我们从$K_0(B)$到$K_0(A)$定义了(VIII,p. 202)群同态$f_*$；我们有

$$
f_*([T]) =h(f)[S] \tag{33}
$$

假设 A 和 B 是交换域 K 上的有限维代数，并且 $f$ 是 K 线性的。作为之前，从A到$\mathbf{M}_m(D)$，从B到$\mathbf{M}_n(E)$，存在整数$m\geqslant 1$和$n\geqslant 1$，K-代数D和域，以及K-代数同构。 集合$d= [D : K]$和$e= [E : K]$。那么我们就有关系

$$
[A : K] =m^2d ,[B : K] =n^2e ,[B : A]_s=\frac{n^2e}{m^2d}
$$

并且，通过公式 (30) 和 (32)，关系

$$
i(f) =\frac{n}{m},h(f) =\frac{ne}{md}
$$

当域 K 是代数闭集时，我们有 $d=e= 1$，因此有 $i(f) =h(f)$ 和 $[B : A]_s=i(f)^2$。

设A、B和C为简单的环，并令$f: A\rightarrow B$和$g: B\rightarrow C$为同态。令 S 为单A-模。 C-模块$(g\circ f)^*(S)$和$g^*(f^*(S))$是同构的；因此，通过公式 (26) 和 (28)，我们有

$i(g\circ f) =$长$_C(g^*(f^*(S))) =i(g)$长$_B(f^*(S)) =i(g)i(f)$。

我们可以证明等式$h(g\circ f) =h(g)h(f)$同样。当A是B的子环并且B是C的子环时，我们对$f$和$g$取典范嵌入，这些等式给出

$$
i(C,A) =i(C,B)i(B,A),h(C,A) =h(C,B)h(B,A) \tag{34}
$$

#### 命题 12 {#alg-viii-s11-prop-12 .statement tag=00DR}

设 B 为 B 的简单环，A 为 B 的简单子环。假设 B 是有限生成的左A-模。设 M 为非零的有限生成的左B-模。 集合$A'=$结束$_A(M)$和$B'=$结束$_B(M)$。那么$B'$是$A'$的子环，环$A'$和$B'$很简单，$A'$是有限生成的左$B'$模，我们有等式

$$
i(A',B') =h(B,A),h(A',B') =i(B,A),[A': B']_s= [B : A]_s
$$

由 VIII、p. 123、环 $A'$ 的命题 4 很简单，M 是有限长度的$A'$模，我们有

长$_A(M) =$长(A$'$)，长$_{A'}(M) =$长(A)。

出于同样的原因，环$B'$很简单，我们有

长$_B(M) =$长(B$'$)，长$_{B'}(M) =$长(B)。

通过公式 (31) 和 (30)，我们有

$h(B,A) =$长$_A(M)/$长$_B(M) =$长(A$'$)$/$长(B$'$)$=i(A',B')$;

类似地可成立等式$h(A',B') =i(B,A)$。由此，我们推论

$$
[A': B']_s=i(A',B')h(A',B') =h(B,A)i(B,A) = [B : A]_s
$$

使用公式 (32)。特别是，$A'$是有限生成的左$B'$-模块。

### 习题{#alg-viii-s11-exercises}

参见[习题为 § 11](exercises/s11/)。
