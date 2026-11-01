---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 6
section_title: Modules over a split semi-simple Lie algebra
lang: zh
source: lie-vii-ix
book_pages: 115-123, 238
pdf_pages: 0123-0131, 0246-0246
extraction: native
subsections:
    - "no": 1
      title: WEIGHTS AND PRIMITIVE ELEMENTS
      page: 116
      pdf_page: 124
    - "no": 2
      title: SIMPLE MODULES WITH A HIGHEST WEIGHT
      page: 118
      pdf_page: 126
    - "no": 3
      title: EXISTENCE AND UNIQUENESS THEOREM
      page: 119
      pdf_page: 127
    - "no": 4
      title: COMMUTANT OF $\mathfrak{h}$ IN THE ENVELOPING ALGEBRA $\mathbf{O}\mathbf{F}\mathfrak{g}$
      page: 122
      pdf_page: 130
statements: 17
exercises: 5
content_sha256: 249ab71af024809fce768475754b280fa1bf3b6cece1fe5e9010012cfe3e52fd
translated_from: content/en/lie/VIII/06_s6_modules_over_a_split_semi_simple_lie.md
translation_method: google
source_content_sha256: 487388bd8ad7aeeaec7bc35a084734841a8e2e5b22d8bc35a3035539d1b008d8
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 503d5ef18f0eca3183df1b935c66c06297ef999b71ad5591afefe12b920cdf42
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 6。 模超过分裂的半单李代数

在本段中，$(\mathfrak{g},\mathfrak{h})$表示分裂的半单李代数，R表示根系，W表示Weyl群，R的B基，$R_+$（或$R_-$）集合表示正（或负） 根相对于 B. Put

$\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha},\mathfrak{n}_-=\sum_{\alpha\in R_-}\mathfrak{g}^{\alpha},\mathfrak{b}_+=\mathfrak{h}+\mathfrak{n}_+$和$\mathfrak{b}_-=\mathfrak{h}+\mathfrak{n}_-$。

我们有$\mathfrak{n}_+= [\mathfrak{b}_+,\mathfrak{b}_+],\mathfrak{n}_-= [\mathfrak{b}_-,\mathfrak{b}_-]$。

对于所有 $\alpha \in R$, 选择元素 $X_{\alpha}\in \mathfrak{g}^{\alpha}$ 使得

$$
[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}
$$

(§2, no. 4);下面的定义都不会依赖于这个选择。

### 1. 权和原始元素

令 V 为 $\mathfrak{g}$ 模块。对于所有$\lambda \in \mathfrak{h}^*$，用$V^{\lambda}$表示主要子空间，相对于$\lambda$，V被视为$\mathfrak{h}$模块（第VII, §1, no. 1章）。 $V^{\lambda}$的元素被称为$\mathfrak{g}$模块V的权$\lambda$的元素。 $V^{\lambda}$ 的和是直接的（第 VII, §1, no. 1 章，第 3 条命题）。对于所有 $\alpha \in \mathfrak{h}^*$ 和 $\lambda \in \mathfrak{h}^*,\mathfrak{g}^{\alpha}V^{\lambda}\subset V^{\alpha+\lambda}$（第 VII, §1, no. 3 章，提案 10 (ii)）。 $V^{\lambda}$的维数在V中称为$\lambda$的重数；如果它是$\geq 1$，即如果$V^{\lambda}\not= 0,\lambda$被称为V的权。如果 V 是有限维的，则由 $\mathfrak{h}$ 的元素定义的 V 的同位性为半单，因此 $V^{\lambda}$ 是 $x\in V$ 的集合，使得对于所有 $H\in \mathfrak{h}$ 都有 $Hx=\lambda (H)x$。

#### 引理 1 {#lie-viii-s6-lem-1 .statement tag=012M}

令V为$\mathfrak{g}$模块，$v\in V$。以下条件是等效的：

（一）$\mathfrak{b}_+v\subset kv$；

(ii)$\mathfrak{h}v\subset kv$和$\mathfrak{n}_+v= 0$；

(iii) $\mathfrak{h}v\subset kv$ 和 $\mathfrak{g}^{\alpha}v= 0$ 对于所有 $\alpha \in B$。

(i) $=\Rightarrow$ (ii)：假设$\mathfrak{b}_+v\subset kv$。存在$\lambda \in \mathfrak{h}^*$使得$v\in V^{\lambda}$。让$\alpha \in R_+$。然后$\mathfrak{g}^{\alpha}.v\subset V^{\lambda}\cap V^{\lambda+\alpha}= 0$。因此$\mathfrak{n}_+v= 0$。

(ii) $=\Rightarrow$ (iii)：这很清楚。

(iii) $=\Rightarrow$ (i)：这是根据$(X_{\alpha})_{\alpha\in B}$ 生成 $\mathfrak{n}_+($§3, no. 3，提案 9 (iii)）得出的。

#### 定义 1 {#lie-viii-s6-def-1 .statement tag=012N}

令 V 为 $\mathfrak{g}$ 模块，$v\in V$。如果 $v\not= 0$ 和 $v$ 满足引理 1 的条件，则 $v$ 被称为 V 的原语元素。

原始元素属于到 $V^{\lambda}$ 之一。对于所有$\lambda \in \mathfrak{h}^*, V_{\pi}^{\lambda}$表示$v\in V^{\lambda}$的集合，使得$\mathfrak{b}_+v\subset kv$。因此，权$\lambda$的原语元素是$V_{\pi}^{\lambda}$的非零元素。

#### 命题 1 {#lie-viii-s6-prop-1 .statement tag=012O}

令V为$\mathfrak{g}$模块，$v$为V的原语元素，以及$\omega$权为$v$。假设 V 由 $v$ 作为 $\mathfrak{g}$ 模块生成。

(i) 如果$U(\mathfrak{n}_-)$表示$\mathfrak{n}_-$的包络代数，我们有$V = U(\mathfrak{n}_-).v$。

(ii) 对于所有 $\lambda \in \mathfrak{h}^*,V^{\lambda}$ 是 $x\in V$ 的集合，使得 $Hx=\lambda (H)x$ 对于所有 $H\in \mathfrak{h}$。我们有 $V =\bigoplus_{\lambda\in\mathfrak{h}^*}V^{\lambda}$，每个 $V^{\lambda}$ 都是有限维的。 空间

$V^{\omega}$ 为维数 1，V 的每个权为形式 $\omega -\sum_{\alpha\in B}n_{\alpha}.\alpha$，其中 $n_{\alpha}$ 为整数 $\geq 0$。

(iii) V 是不可分解的 $\mathfrak{g}$ 模，其交换子约化为标量。

(iv) 设$U(\mathfrak{g})$为$\mathfrak{g}$的包络代数，以及$\mathscr{Z}$中心为$U(\mathfrak{g})$。从$\mathscr{Z}$到$k$存在唯一同态$\chi$，使得对于所有$z\in \mathscr{Z}$，$z_V$是位似，比率为$\chi (z)$。

令$U(\mathfrak{b}_+)$为$\mathfrak{b}_+$的包络代数。我们有 $U(\mathfrak{g}) = U(\mathfrak{n}_-).U(\mathfrak{b}_+)$（第 I, §2, no. 7 章，第 1 章第 6 章）。因此

$$
V = U(\mathfrak{g}).v= U(\mathfrak{n}_-).U(\mathfrak{b}_+).v= U(\mathfrak{n}_-).v
$$

用 $\alpha_1, . . . , \alpha_n$ 表示与 $R_+$ 不同的元素。然后

$$
(X_{-\alpha_1}^{p_1}X_{-\alpha_2}^{p_2}. . . X_{-\alpha_n}^{p_n})_{(p_1,...,p_n)\in\mathbf{N}^n}
$$

是基 / $U(\mathfrak{n}_-)$，所以

V = $\sum kX_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}v$。 (1)

$(p_1,...,p_n)\in \mathbf{N}^n$

对于 $\lambda \in \mathfrak{h}^*$，输入

$$
T_{\lambda}=\sum kX_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}v
$$

$(p_1,...,p_n)\in \mathbf{N}^n, \omega -p_1\alpha_1-\cdot \cdot \cdot -p_n\alpha_n=\lambda$

由章。 VII, §1, no. 1，提案 2 (ii)，如果 $h\in \mathfrak{h},h_V|T_{\lambda}$ 是位似，比率为 $\lambda (h)$。所以$T_{\lambda}\subset V^{\lambda}$。另一方面，(1) 意味着

V = $\sum T_{\lambda}$。

$\lambda \in \omega -\mathbf{N}\alpha_1-\cdot \cdot \cdot -\mathbf{N}\alpha_n$

$V^{\lambda}$ 的和是直接的（第 VII, §1, no. 1 章，第 3 条命题）。从这些观察结果可以看出，$V^{\lambda}= T_{\lambda}$，V是$V^{\lambda}$的直和，$V^{\lambda}$是$x\in V$的集合，这样对于所有$h\in \mathfrak{h}$来说$hx=\lambda (h)x$。另一方面，dim $V^{\lambda}$ 至多是$(p_1, . . . , p_n)\in \mathbf{N}^n$ 的集合的基数，使得$p_1\alpha_1+\cdots +p_n\alpha_n=\omega -\lambda$。这证明了 $V^{\lambda}= 0$ 如果 $\omega -\lambda  \notin \sum_{\alpha\in B}\mathbf{N}\alpha$，

暗淡的 $V^{\omega}= 1$ 和 $V^{\lambda}$ 都是有限维的。

令$c$为V的交换子元素。对于所有$h\in \mathfrak{h}$，

$$
hc(v) =ch(v) =\omega (h)c(v)
$$

所以$c(v)\in V^{\omega}$；因此存在$t\in k$使得$c(v) =tv$。现在，对于所有$(p_1, . . . , p_n)\in \mathbf{N}^n$，

$$
cX_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}v=X_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}cv=tX_{-\alpha_1}^{p_1}. . . X_{-\alpha_n}^{p_n}v
$$

这样$c=t.1$。因此，V 约化与标量的交换律。这意味着 (iv) 以及 V 不可分解的事实。

#### 定义 2 {#lie-viii-s6-def-2 .statement tag=012P}

提案1（iv）的同态$\chi$被称为$\mathfrak{g}$模块V的中心特征标。

#### 命题 2 {#lie-viii-s6-prop-2 .statement tag=012Q}

令V是由权$\omega$的基元元素$e$和X半单$\mathfrak{g}$生成的$\mathfrak{g}$模块。令$\Phi$为从$\mathfrak{g}$-模块V到$\mathfrak{g}$-模块X的同态的集合。那么$\varphi  \rightarrow \varphi (e)$就是从向量空间$\Phi$到向量空间$X^{\omega}_{\pi}$的同构。

很明显，$\varphi (e)\in X^{\omega}_{\pi}$ 对于所有$\varphi \in \Phi$。如果 $\varphi \in \Phi$ 和 $\varphi (e) = 0$，则 $\varphi = 0$ 自 $e$ 生成 $\mathfrak{g}$-模V。我们证明，如果$f$是$X^{\omega}_{\pi}$的非零元素，则存在$\varphi \in \Phi$使得$\varphi (e) =f$。令$X'$为由$f$生成的X的子模。根据命题，$1, X'$是不可分解的，因此很简单，因为X是半单。 元素 $(e, f)$ 在 $\mathfrak{g}$ 模块 $V\times X$ 中是原语。令 N 为 $(e, f)$ 生成的 $V\times X$ 的子模。那么$N\cap X\subset$ pr$_2(N) = X'$，所以$N\cap X = 0$或$X'$；如果$N\cap X = X', N$包含线性无关元素$(e, f)$和$(0, f)$，它们是权$\omega$的原语；这是荒谬的（命题 1），所以 $N\cap X = 0$。因此 pr$_1|N$ 是从 N 到 V 的单射映射 $h$；这个映射是满射的，因为它的像包含 $e$。因此，$\varphi =$pr$_2\circ h^{-1}$是从$\mathfrak{g}$-模块V到$\mathfrak{g}$-模块X的同态，使得$\varphi (e) =f$。

### 2. 单模与最高权

回想一下，将 B 定义序关系固定在 $\mathfrak{h}^*_{\mathbf{Q}}$ 上（第 VI, §1, no. 6 章）。 $\mathfrak{h}^*_{\mathbf{Q}}$的元素即$\geq 0$是B的元素的线性组合，有理系数$\geq 0$。

更一般地，我们将考虑以下元素 $\lambda , \mu\in \mathfrak{h}^*:$ 之间的序关系

$\lambda -\mu$ 是 B 的元素的线性组合，其有理系数$\geq 0$。

#### 引理 2 {#lie-viii-s6-lem-2 .statement tag=012R}

让V是一个简单的$\mathfrak{g}$模块，$\omega$权为V。以下条件是等效的：

(i) V 的每个权都是形式 $\omega -\mu$，其中 $\mu$ 是部首权 $\geq 0$；

(ii) $\omega$ 是 V 中的最高权；

(iii) 对于所有 $\alpha \in B,\omega +\alpha$ 不是权或 V；

(iv) 存在原语元素权 $\omega$。

(i) $=\Rightarrow$ (ii) $=\Rightarrow$ (iii)：这很清楚。

(iii)$=\Rightarrow$(iv)：假设满足条件(iii)。对于所有$h\in \mathfrak{h}$，

克尔($h_V-\omega (h)$)

非零，包含在$V^{\omega}$内，并且在$\mathfrak{h}_V$下稳定。通过$\mathfrak{h}$上的归纳，我们看到$V^{\omega}$中存在非零$v$，使得$\mathfrak{h}v\subset kv$。 条件 (iii) 意味着$\mathfrak{n}_+v= 0$，所以$v$ 是原语。

(iv) $=\Rightarrow$ (i)：令 $v$ 为权 $\omega$ 的原语元素。由于V很简单，V由$v$生成为$\mathfrak{g}$模块。 断言 (i) 现在由命题 1 得出。

Q.E.D.

因此，对于任何简单的$\mathfrak{g}$模块，原语元素的存在等价于最高权的存在，或者与最大权的存在。存在简单的$\mathfrak{s}\mathfrak{l}(2,\mathbf{C}$)-模块V，对于$\mathfrak{s}\mathfrak{l}(2,\mathbf{C}) ($§1的任何嘉当子代数$\mathfrak{h}$，Exerc没有权。 $14f))$。这些模在$\mathbf{C}($§1, no. 3上有无限的维数，Th。 1）。

#### 命题 3 {#lie-viii-s6-prop-3 .statement tag=012S}

让 V 成为一个简单的 $\mathfrak{g}$ 模块，其中包含最高权 $\omega$。

(i) V 的原语元素是$V^{\omega}$ 的非零元素。

(ii) V 是半单作为 $\mathfrak{h}$ 模块。

(iii) 我们有 $V =\bigoplus_{\lambda\in\mathfrak{h}^*}V^{\lambda}$。对于所有 $\lambda \in \mathfrak{h}^*,V^{\lambda}$ 都是有限维的。我们

有暗淡$V^{\omega}= 1$。

(iv) $\mathfrak{g}$-模块V 绝对简单。

断言 (i)、(ii) 和 (iii) 源自提案 1 和引理 2。断言 (iv) 源自提案 1 (iii) 和代数，第 1 章。 VIII, §7, no. 3。

#### 推论{#lie-viii-s6-n2-cor-1 .statement tag=012T}

如果 V 是有限维的，则典范同态 $U(\mathfrak{g})\rightarrow$ End(V) 是满射的。

这是从 (iv), cf. 代数, 第 1 章得出的。 VIII, §3, no. 3。

#### 命题 4 {#lie-viii-s6-prop-4 .statement tag=012U}

设 V 是一个简单的 $\mathfrak{g}$ 模块，其中最高权 $\omega$、X 半单 $\mathfrak{g}$ 模块，以及 $X'$ 型 V 的同型组件X。那么$X'$就是$X^{\omega}_{\pi}$生成的X的子模。它的长度等于$X^{\omega}_{\pi}$的维数。

令$X''$为$X^{\omega}_{\pi}$生成的X中的子模。显然，X同构于V的每个子模都包含在$X''$中。因此$X'\subset X''$。另一方面，令$\Phi$为从$\mathfrak{g}$-模块V到$\mathfrak{g}$-模块X的同态的集合。 $X'$的长度暗淡$_k\Phi ($代数，第1章。 VIII, §4, no. 4），即暗$_kX^{\omega}_{\pi}$（命题 2）。

### 3. 存在和唯一性定理

让$\lambda \in \mathfrak{h}^*$。自$\mathfrak{b}_+=\mathfrak{h}\oplus \mathfrak{n}_+$和$\mathfrak{n}_+= [\mathfrak{b}_+,\mathfrak{b}_+]$以来，映射$h+n \rightarrow \lambda (h)$（其中$h\in \mathfrak{h},n\in \mathfrak{n}_+$）从$\mathfrak{b}_+$到$k$是$\mathfrak{b}_+$的一维表示。用$L_{\lambda}$表示配备有由表示定义的$\mathfrak{b}_+$模块结构的$k$向量空间$k$。令$U(\mathfrak{g}), U(\mathfrak{b}_+)$为$\mathfrak{g},\mathfrak{b}_+$的包络代数，使得$U(\mathfrak{b}_+)$为$U(\mathfrak{g})$的子代数；回想一下，$U(\mathfrak{g})$是一个自由的右$U(\mathfrak{b}_+$)模块（第I, §2, no. 7章，第1章的Cor.5）。放

$$
Z(\lambda ) = U(\mathfrak{g})\otimes_{U(\mathfrak{b}_+)}L_{\lambda} \tag{2}
$$

那么$Z(\lambda )$是左$\mathfrak{g}$模。用$Z(\lambda )$的$e$元素$1\otimes 1$表示。

#### 命题 5 {#lie-viii-s6-prop-5 .statement tag=012V}

(i) $Z(\lambda )$的元素$e$是权$\lambda$和生成的$\mathfrak{g}$模$Z(\lambda )$的原语。

(ii) 设 $Z^+(\lambda ) =\sum_{\lambda\not=\mu}Z(\lambda )^\mu$。 $Z(\lambda )$ 中的每个子模与 $Z(\lambda )$ 不同

包含在$Z^+(\lambda )$中。

(iii) $Z(\lambda )$中存在与$Z(\lambda )$不同的最大的子模$F_{\lambda}$。 商模$Z(\lambda )/F_{\lambda}$很简单，有最高权$\lambda$。

很明显，$e$生成$\mathfrak{g}$-模块$Z(\lambda )$。如果$x\in \mathfrak{b}_+$，

$$
x.e= (x.1)\otimes 1 = (1.x)\otimes 1 = 1\otimes x.1 =\lambda (x)(1\otimes 1) =\lambda (x)e
$$

因此(i)。

$\mathfrak{h}$-模块$Z(\lambda )$是半单（提案1）。如果 G 是 $Z(\lambda )$ 的$\mathfrak{g}$子模，则$G =\sum_{\mu\in\mathfrak{h}^*}(G\cap Z(\lambda )^\mu)$。 假设 $G\cap Z(\lambda )^{\lambda}\not= 0$ 意味着

$G = Z(\lambda )$，因为暗淡$Z(\lambda )^{\lambda}= 1$和$e$生成$\mathfrak{g}$模块$Z(\lambda )$。如果$G\not= Z(\lambda )$，则$G =\sum_{\mu\not=\lambda}G\cap Z(\lambda )^\mu\subset Z^+(\lambda )$。

令 $F_{\lambda}$ 为 $Z(\lambda )$ 的 $\mathfrak{g}$ 子模块中与 $Z(\lambda )$ 不同的和。由(ii)，$F_{\lambda}\subset Z^+(\lambda )$。因此，$F_{\lambda}$是$Z(\lambda )$的最大的子模，与$Z(\lambda )$不同。显然，$Z(\lambda )/F_{\lambda}$是简单的，并且$Z(\lambda )/F_{\lambda}$中$e$的典范像是权$\lambda$的本原。

在这个章的剩余部分中，第5号提案的$\mathfrak{g}$模块$Z(\lambda )/F_{\lambda}$将由$E(\lambda )$表示。

#### 定理 1 {#lie-viii-s6-thm-1 .statement tag=012W}

让$\lambda \in \mathfrak{h}^*$。 $\mathfrak{g}$-模块$E(\lambda )$很简单，有最高权$\lambda$。 最高权 $\lambda$ 的每个简单$\mathfrak{g}$模都与$E(\lambda )$同构的。

第一个断言源自命题 5 (iii)。第二个来自于命题 4。

#### 命题 6 {#lie-viii-s6-prop-6 .statement tag=012X}

令V为$\mathfrak{g}$模块，$\mathfrak{h}^*$的$\lambda$元素以及$v$为权$\lambda$的V的原语元素。

(i) 存在$\mathfrak{g}$模块$\psi : Z(\lambda )\rightarrow V$中的唯一同态使得$\psi (e) =v$。

(ii) 假设$v$生成V。那么 $\psi$ 是满射。此外，$\psi$ 是双射的当且仅当，对于 $U(\mathfrak{n}_-),u_V$ 的每个非零元素 $u$ 都是单射的。

(iii) 从$U(\mathfrak{n}_-)$到$Z(\lambda )$的映射$u \rightarrow u\otimes 1$是双射的。

设K为$L_{\lambda}$上$U(\mathfrak{b}_+)$表示核；它的余维数为 1，位于 $U(\mathfrak{b}_+)$ 中。令$J = U(\mathfrak{g})K$为K生成的$U(\mathfrak{g})$的左理想；那么$L_{\lambda}$可以用$U(\mathfrak{b}_+)/K$识别为左$U(\mathfrak{b}_+$)-模块，并且$Z(\lambda )$可以用$U(\mathfrak{g})/J$识别为左$U(\mathfrak{g}$)-模块。我们有$K.v= 0$，所以$J.v= 0$，这证明了(i)。

现在假设$v$生成V。显然$\psi$是满射的。

根据Poincaré-Birkhoff-Witt 定理（第1章第I, §2, no. 7章，Cor.6），$U(\mathfrak{n}_-)$的基超过$k$也是$U(\mathfrak{g})$的基作为右$U(\mathfrak{b}_+)$模。因而，从$U(\mathfrak{n}_-)$到$U(\mathfrak{g})\otimes_{U(\mathfrak{b}_+)}L_{\lambda}$的映射$\varphi :u \rightarrow u\otimes 1$是双射的。让$u\in U(\mathfrak{n}_-)$。然后$\varphi^{-1}\circ u_{Z(\lambda)}\circ \varphi$在$U(\mathfrak{n}_-)$上被$u$留下乘法。鉴于章。 I, §2, no. 7，科。 7 Th。如果 $u\not= 0$，$1,u_{Z(\lambda)}$ 是单射的。因而，如果 $\psi$ 是双射，则 $u_V$ 对于 $U(\mathfrak{n}_-)$ 中的非零 $u$ 是单射的。

假设 $\psi$ 不是单射的。存在$u\in U(\mathfrak{n}_-)$使得$u\not= 0$和$\psi (\varphi (u)) = 0$。然后

$$
u_V.v=u_V.\psi (1\otimes 1) =\psi (u\otimes 1) =\psi (\varphi (u)) = 0
$$

#### 推论 1 {#lie-viii-s6-prop-6-cor-1 .statement tag=012Y}

令$\lambda \in \mathfrak{h}^*$和$\alpha \in B$使得$\lambda (H_{\alpha}) + 1\in \mathbf{N}$。那么$Z(-\alpha +s_{\alpha}\lambda )$同构于$Z(\lambda )$的$\mathfrak{g}$子模块。

输入$m=\lambda (H_{\alpha})$。设$x= X^{m+1}_{-\alpha}.e\in Z(\lambda )$，并令V为由$x$生成的$Z(\lambda )$的子模。然后$x\not= 0$（命题6）。另一方面，$x\in Z(\lambda )^{\lambda-(m+1)\alpha}$。对于$\beta \in B$、$\beta \not=\alpha , [\mathfrak{g}^{-\alpha},\mathfrak{g}^{\beta}] = 0$和$\mathfrak{g}^{\beta}.e= 0$，所以$\mathfrak{g}^{\beta}.x= 0$。最后，从$[X_{\alpha},X_{-\alpha}] =-H_{\alpha}$开始，我们有

$$
[X_{\alpha}, X_{-\alpha}^{m+1}] = (m+ 1)X_{-\alpha}^m(-H_{\alpha}+m)
$$

（§1, no. 1，引理 1 (ii)），所以

$$
X_{\alpha}.x=X_{\alpha}X_{-\alpha}^{m+1}.e= [X_{\alpha}, X_{-\alpha}^{m+1}].e= (m+ 1)X_{-\alpha}^m(me-\lambda (H_{\alpha})e) = 0
$$

因而，$x$是权$\lambda -(m+ 1)\alpha$的原语。根据命题6，$\mathfrak{g}$-模V与$Z(-\alpha +\lambda -m\alpha ) = Z(-\alpha +s_{\alpha}\lambda )$同构的。

#### 推论 2 {#lie-viii-s6-prop-6-cor-2 .statement tag=012Z}

设$\rho =\frac{1}{2}\sum_{\alpha\in R_+}\alpha$和$\lambda , \mu\in \mathfrak{h}^*$。假设$\lambda +\rho$是R中的主导权，并且存在$w\in W$和$\mu+\rho =w(\lambda +\rho )$。那么$Z(\mu)$同构于$Z(\lambda )$的子模。

$w= 1$ 时断言清晰。假设每当$w$为长度$< q$时成立。如果$w$是长度$q$，则存在$\alpha \in B$使得$w=s_{\alpha}w^{'-1}$和$l(w') =q-1$。我们有$w'(\alpha )\in R_+$（第VI, §1, no. 6章，第17号提案第2条），因此$w^{'-1}(\lambda +\rho )(H_{\alpha}) = (\lambda +\rho )(H_{w'\alpha})$是整数$\geq 0$。放

$$
\mu'=w^{'-1}(\lambda +\rho )-\rho
$$

到归纳假设，$Z(\mu')$同构于$Z(\lambda )$的子模。另一方面，由章。 VI, §1, no. 10，提案 29 (ii)，

$$
-\alpha +s_{\alpha}\mu'=-\alpha +s_{\alpha}w^{'-1}(\lambda +\rho )-s_{\alpha}\rho =w(\lambda +\rho )-\rho =\mu
$$

此外，$\rho (H_{\alpha}) = 1$（第VI, §1章，提案29（iii）），所以$\mu'(H_{\alpha})+1\in \mathbf{N}$。科。 1现在意味着$Z(\mu)$与$Z(\mu')$的子模同构，因此也与$Z(\lambda )$的子模同构。

### 4. 代数 $\mathbf{O}\mathbf{F}\mathfrak{g}$ 中$\mathfrak{h}$的交换

令U为$\mathfrak{g}, V\subset U$的包络代数和$\mathfrak{h}$的包络代数。 代数V可以与$\mathfrak{h}$的对称代数$\mathbf{S}(\mathfrak{h})$识别，也可以与$\mathfrak{h}^*$上的多项式函数的代数识别。用 $\alpha_1, . . . , \alpha_n$ 表示成对不同的正值根。设$(H_1, . . . , H_l)$为$\mathfrak{h}$中的基。由庞加莱-伯克霍夫-维特定理，元素

$$
u((q_i),(m_i),(p_i)) =X_{-\alpha_1}^{q_1}. . . X_{-\alpha_n}^{q_n}H_1^{m_1}. . . H_l^{m_l}X_{\alpha_1}^{p_1}. . . X_{\alpha_n}^{p_n}
$$

$(q_i, m_i, p_i$ 整数 $\geq 0)$ 形式基向量空间 U。对于所有 $h\in \mathfrak{h}$，我们有

$$
[h, u((q_i),(m_i),(p_i))] = ((p_1-q_1)\alpha_1+\cdots +(p_n-q_n)\alpha_n)(h)u((q_i),(m_i),(p_i)).(3)
$$

向量空间 U 是伴随表示下的 $\mathfrak{g}$ 模（因此也是 $\mathfrak{h}$ 模）。如果定义了$\lambda \in \mathfrak{h}^*$、子空间、$U^{\lambda}$和$U_{\lambda}$（第VII, §1, no. 3章）； 公式 (3) 表明$U^{\lambda}= U_{\lambda}$ 和$U =\bigoplus_{\lambda\in Q}U^{\lambda}$

（其中Q是R的根权的群）。特别是，在 U 中，$U^0$ 是 $\mathfrak{h}$ 或 V 的交换子。

#### 引理 3 {#lie-viii-s6-lem-3 .statement tag=0130}

把$L = (\mathfrak{n}_-U)\cap U^0$。

(i) 我们有$L = (U\mathfrak{n}_+)\cap U^0$，L是$U^0$的双面理想。

(ii) 我们有 $U^0= V\oplus L$。

很明显，$\mathfrak{n}_-U$（或$U\mathfrak{n}_+$）是元素$u((q_i),(m_i),(p_i))$的线性组合的集合，使得$\sum q_i>0$（或$\sum p_i>0$）。另一方面

$$
u((q_i),(m_i),(p_i))\in U^0\Leftarrow \Rightarrow p_1\alpha_1+\cdots +p_n\alpha_n=q_1\alpha_1+\cdots +q_n\alpha_n
$$

这意味着$(\mathfrak{n}_-U)\cap U^0= (U\mathfrak{n}_+)\cap U^0$。最后，$(\mathfrak{n}_-U)\cap U^0$（或$(U\mathfrak{n}_+)\cap U^0$）是$U^0$的右（或左）理想，因此(i)。此外，元素$u((q_i),(m_i),(p_i))$位于$U^0$属于到V（分别到L）当且仅当$p_1=\cdots =p_n=q_1=\cdots =q_n= 0$（分别$p_1+\cdots +p_n+q_1+\cdots +q_n>0$），因此(ii)。 Q.E.D.

鉴于引理 3，$U^0$的投影到V与核L是代数的同态。从 $U^0$ 到 V（相对于 B）被称为 Harish-Chandra 同态。回想一下，V可以与$\mathfrak{h}^*$上的多项式函数的代数识别。

#### 命题 7 {#lie-viii-s6-prop-7 .statement tag=0131}

设$\lambda \in \mathfrak{h}^*$，E是由权$\lambda ,\chi$的原语元素生成的$\mathfrak{g}$模块，E的中心特征标，以及$\varphi$从$U^0$到V的Harish-Chandra同态。然后，$\chi (z) = (\varphi (z))(\lambda )$对于U的中心中的所有$z$。

令$v$为权$\lambda$的E的原语元素，以及U的中心的$z$元素。存在$u_1, . . . , u_p\in U$和$n_1, . . . , n_p\in \mathfrak{n}_+$使得$z=\varphi (z) +u_1n_1+\cdots +u_pn_p$。然后

$$
\chi (z)v=zv=\varphi (z)v+u_1n_1v+\cdots +u_pn_pv=\varphi (z)v= (\varphi (z))(\lambda )v
$$

#### 推论{#lie-viii-s6-n4-cor-1 .statement tag=0132}

令$\langle  \cdot ,\cdot  \rangle$是$\mathfrak{g}$上的非简并不变对称双线性形式，C与$\langle  \cdot ,\cdot  \rangle$相关的卡西米尔元素。也用$\langle  \cdot ,\cdot  \rangle$表示$\langle  \cdot ,\cdot  \rangle$到$\mathfrak{h}($§2, no. 3的限制的$\mathfrak{h}^*$的逆形式，命题5）。然后$\chi (C) =\langle \lambda , \lambda + 2\rho \rangle$，其中$\rho =\frac{1}{2}\sum_{\alpha\in R_+}\alpha$。

我们回忆一下第 6 条命题 §2, no. 3 的记号。我们有

1 1

C = $\sum X_{\alpha}X_{-\alpha}+\sum X_{-\alpha}X_{\alpha}$

$$
_{\alpha\in R_-}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}\alpha^{\in}_{R_+}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}
$$

1 $'$

$$
+\sum[X_{\alpha}, X_{-\alpha}] +\sum H_iH
$$

$$
_{\alpha\in R_+}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}i_{\in I}^i
$$

所以

$$
\varphi (C) =\sum_{\alpha\in R_+}\frac{1}{\langle X_{\alpha}, X_{-\alpha}\rangle}[X_{\alpha}, X_{-\alpha}] +\sum_{i\in I}H_iH'_i
$$

根据第 7 号提案，

1 $'$

$$
\chi (C) =\sum\lambda ([X_{\alpha}, X_{-\alpha}]) +\sum\lambda (H_i)\lambda (H)
$$

$$
_{\alpha\in R_+}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}i_{\in I}i
$$

令 $h_{\lambda}$ 为 $\mathfrak{h}$ 的元素，使得 $\langle h_{\lambda}, h\rangle =\lambda (h)$ 对于所有 $h\in \mathfrak{h}$。根据 §2, no. 2，第 1 号提案，

$($ 1 $)\langle$ 1 $\rangle$

$\lambda [X_{\alpha}, X_{-\alpha}]$ = $h_{\lambda},[X_{\alpha}, X_{-\alpha}]=\alpha (h_{\lambda}) =\langle \lambda , \alpha \rangle$。

$$
\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}\overline{\langle X_{\alpha}, X_{-\alpha}\rangle}
$$

因此

$$
\chi (C) =((\sum_{\alpha\in R_+}\langle \lambda , \alpha \rangle )+\langle \lambda , \lambda \rangle =\langle \lambda , \lambda + 2\rho \rangle
$$

### 习题{#lie-viii-s6-exercises}

请参阅[习题为 § 6](exercises/s6/)。
