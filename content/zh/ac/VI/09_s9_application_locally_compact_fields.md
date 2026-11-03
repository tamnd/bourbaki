---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 9
section_title: 'Application: locally compact fields'
lang: zh
source: ac-i-vii
book_pages: 431-434, 470-471
pdf_pages: 0449-0452, 0488-0489
extraction: ocr
subsections:
    - "no": 1
      title: THE MODULUS FUNCTION ON A LOCALLY COMPACT FIELD
      page: 431
      pdf_page: 449
    - "no": 2
      title: EXISTENCE OF REPRESENTATIVES
      page: 432
      pdf_page: 450
    - "no": 3
      title: STRUCTURE OF LOCALLY COMPACT FIELDS
      page: 433
      pdf_page: 451
statements: 10
exercises: 5
content_sha256: 2e86d9facabfe195ab3465fbc8ec38eae68ede4bb9be58ca8aa4210c051b269a
translated_from: content/en/ac/VI/09_s9_application_locally_compact_fields.md
translation_method: google
source_content_sha256: cbf8d7f6c26e3c562858fae29ec698adc8ce0ba172721d0d36754a85dbdf6f59
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: dc182aa02530d611ecfac8fe87d31160aa783aecd3080bff696de71e39b0fd77
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## 9. 应用：局部紧凑域

### 1. 局部紧致域上的模数函数

令 $K$ 为局部紧致域 （不一定可交换）。回想一下，函数 mod（或 mod,）已在 $K$ 上定义（积分、章 VII, § 1, no. 10、定义 6），如下所示：$\operatorname{mod}_K(0) = 0$ 和$K$ 中的$x \neq 0$，数 $\operatorname{mod}_K(x)$ 是模数自同构 $y \mapsto xy$ 加法群 $K$。

#### 命题 1 {#ac-vi-s9-prop-1 .statement tag=04XQ}

*如果 $K$ 是局部紧致域，则函数 mod, 属于到 $\mathscr{V}(K)$ (§ 6, no. 1)。此外：*
(i) *如果$s > 0$使得$(\operatorname{mod}_K)^s = g$是绝对值，则$g$定义拓扑在$K$上。*
(ii) *如果$K$不是离散且模的，是超度量绝对值，则在$K$上存在规范离散估值$v$，其环是紧致的并且其残差域是有限的$q$元素，因此$\operatorname{mod}, = q^{-v}$。 $K$ 上的拓扑由$v$ 定义。*

这是从§ 6, no. 1、命题 1、§ 5, no. 1、命题 2 以及积分、章 VII, § 1, no. 10、命题 12 和 13 得出的。

#### 命题 2 {#ac-vi-s9-prop-2 .statement tag=04XR}

*令$K, K'$是两个（不一定可交换）局部紧致域，使得$K$是$K'$的拓扑子域，并且$K$不是离散的。然后：*
(i) *$K'$ 是 $K$ 上的有限维左（右）向量空间。*
(ii) *如果$K$包含在$K'$的中心中，则对于所有$x \in K'$。*
(1)
$$
\operatorname{mod}_{K'}(x) = \operatorname{mod}_K(N_{K'/K}(x)).
$$
由于 $K$ 是一个完整的值域，它不是离散的，断言 (i) 由拓扑向量空间、章 I, § 2, no. 4、定理 3 得出； 断言 (ii) 只是积分，章 VII, § 1, no. 11，命题 17。

#### 推论 1 {#ac-vi-s9-prop-2-cor-1 .statement tag=04XS}

*每个中心不是离散的局部紧致域的有限秩超过其中心。*

局部紧致域 $K$ 的中心 $Z$ 在 $K$ 中闭合，因此局部紧致。

#### 推论 2 {#ac-vi-s9-prop-2-cor-2 .statement tag=04XT}

*令 $K'$ 为局部紧致域且 $K$ 为 $K'$ 的闭子域（不一定可交换）。如果 $K'$ 是有限维 $n$ 的左（右）向量空间超过 $K$，则*
(2)
$$
\operatorname{mod}_{K'}(x) = (\operatorname{mod}_K(x))^n \quad \text{for all } x \in K.
$$

一般来说，已知在有限维$n$的（左或右）向量空间超过$K$时，位似与比率$x \in K$的模数等于$(\mathrm{mod}_K(x))^n$；将其应用于$K'$就足够了。

### 2. 代表的存在

#### 命题 3 {#ac-vi-s9-prop-3 .statement tag=04XU}

*令 $K$ 为（不一定可交换的）局部紧致域，它不是离散的，并且其拓扑由离散估值 $v$ 定义；令$A$为环，$m$为$v$的理想，并让我们写出$\mathrm{Card}(A/m) = q = p^f$（p素数）。 那么，$A$中存在$A/m$的代表$S$的系统和$v$的均匀化器$u$，使得$O \in S$、$S^* = S \cap K^*$是$K^*$和$u^{-1} Su = S$的循环子群。 此外，$A$的每个元素都可以唯一地写成形式$\sum_{i=0}^\infty s_i u^i$，其中$s_i \in S$。*

我们将使用以下引理：

#### 引理 1 {#ac-vi-s9-lem-1 .statement tag=04XV}

*令$x, y$为$A$的两个可置换元素，使得$x - y \in m^j \ (j \geq 1)$；然后每整数 $n \geq 0$ $x^{p^n} - y^{p^n} \in m^{j+n}$。*

到$n$的归纳，$n = 1$减少为证明引理。然后

$$
x^p - y^p = (x - y)(x^{p-1} + x^{p-2}y + \ldots + y^{p-1});
$$

第二个因子是$p$项的和，与一个另一个模全等。 $m$ 并且，由于 $A/m$ 具有 $p$ 的特征，$p \cdot 1 \in m$ 在 $A$ 中，因此

$$
x^{p-1} + x^{p-2}y + \ldots + y^{p-1} \in m;
$$

从而$x^p - y^p \in m^{j+1}$。

我们知道乘法群$(A/m)^*$是一个循环群，其中$q - 1$元素（*代数*，章V, § 11, no. 1，定理1）；设$x$为该群的生成元中的$A$的代表；那么$x^q - x \in m$，从而，乘以引理 1，$x^{q^{n+1}} - x^{q^n} \in m^{1+fn}$，因为$x^q$和$x$是可置换的。这就证明$(x^{q^n})_{n \geq 0}$是$A$中的柯西序列；由于$A$是紧致的，因此是完备的，因此序列在$A$中有极限，这显然满足$s \equiv x \pmod{m}$和$s^q = s$。因为$s \neq 0$、$s^{q-1} = 1$，更准确地说，$s$是$A$中单位元*的*原始*$(q-1)$*-第根。显然$0$和幂$s^j \ (0 \leq j \leq q-2)$的集合$S$由……组成是$A$模类的代表*系统。 $m$ 并且在 $A$ 中的乘法下是*不变*。

现在让 $a$ 为 $v$ 的均匀化器，并考虑 $K$ 的内自同构 $y \mapsto a^{-1}ya$；它对自身映射$A$，对自身$m$，因此，取商，它对域$A/m$有定义自同构；已知(*代数*,章V, § 11, no. 4,命题5)这样的自同构是形式$z \mapsto z^{p^r}$，其中$0 \leq r \leq f-1$。然后$a^{-1}s^j a \equiv s^{jp^r} \pmod{m}$换$0 \leq j \leq q-2$；如$a \in m$和$s \notin m$，这意味着$s^{-j}as^{jp^r} \equiv a \pmod{m^2}$。

让我们写

$$
u = \sum_{i=0}^{q-2} s^{-1} a s^i p^r.
$$

然后从 $p . 1 \in m$ 开始$u \equiv (q - l) a \equiv -a (\text{mod. } m^2)$；我们结论认为$u$也是$v$的均匀化器；而且
(3)
$$
s^{-1} u s^{p^r} = u
$$
从而我们推断出$u^{-1} S u = S$。

最后，对于所有$x \in A$，存在唯一的序列$(s_i)$（$i \in \mathbf{N}$），使得对于所有$i$有$s_i \in S$，对于所有$n \geq 0$有$x \equiv \sum s_i u^i$（mod.$m^{n+1}$）：它是直接的除以归纳 $n$，$m^{n+1}$ 满足关系形式 $t \equiv t' u^{n+1}$（模$m^{n+2}$）的每个元素 $t$，其中 $t'$ 是唯一确定的元素 $S$。然后$x = \sum_{i=0}^{\infty} s_i u^i$和家庭$(s_i)$满足这个关系，这样所有$i$的$s_i \in S$都是唯一确定的。

### 3. 局部紧凑域的结构

域 $\mathbf{Q}$ 相对于$\mathbf{Q}$（$p$任何素数）上的非不当绝对值的补全$\mathbf{R}$和$\mathbf{Q}_p$是局部紧致的。 另一方面，对于素数$p$的每个幂$q = p^f$，有限域$F$上的形式幂级数域$\mathbf{F}_q((T))$，在§ 3, no. 4中定义估值，示例3是*局部紧凑的*：对于估值环$\mathbf{F}_q[[T]]$的最大理想，由$T$生成；我们知道这个环是完整的(T)-adic拓扑（第III, § 2, no. 6章，命题6），并且由于留数域$\mathbf{F}_q$是有限的，§ 5, no. 1的命题2证明了我们的断言。 反过来：

#### 定理 1 {#ac-vi-s9-thm-1 .statement tag=04XW}

*设 K 是一个（不一定可交换的）局部紧致域，它不是离散的。*

(i) *如果 K 具有特征 0 且 mod，不是超量绝对值值，则 K 同构于域 $\mathbf{R}, \mathbf{C}$ 或 $\mathbf{H}$ 之一。*

(ii) *如果 K 的特征为 0 且 mod，则为超量绝对值值，则 K 是 p 进数域 $\mathbf{Q}_p$ 上的代数有限秩。*

(iii) *如果 K 具有特征 $p \neq 0$，则它与域与形式幂级数 $\mathbf{F}_q((T))$ 的中心域同构（其中 $q$ 是 $p$ 的幂）且超过有限秩它中心.*

(i) 从 Ostrowski 的定理 (§ 6, no. 4, 定理 2) 可以得出，K 是一个拓扑域同构于 $\mathbf{R}, \mathbf{C}$ 或 $\mathbf{H}$ 的处处稠密子域，并且，由于 K 是完备的，它同构于 $\mathbf{R}, \mathbf{C}$ 或$\mathbf{H}$。

(ii) 设 A 为绝对值 mod 的环，m 为其最大理想值。我们知道 A/m 是有限域 (§ 5, no. 1, 命题 2)，因此由 mod 引起的绝对值，在 $\mathbf{Q}$ 上有一个有限的剩余类域，只有当它等价于 $p$-adic 绝对值 ($§ 6$, no. 3、命题 4)；因此，$K$中$\mathbf{Q}$的闭包与$\mathbf{Q}_p$同构的，并且包含在$K$的中心中，因为后者在$K$中闭包；我们利用得出命题 2 / no. 1。

(iii) 第二个断言是从第一个推论到no. 2的命题2。 为了显示第一个断言，请注意 mod，必然是超度量绝对值（$§ 6$，no. 2，命题 3 的推论）；在no. 2命题3证明的表示法中，$K$的中心$Z$由同时与$s$和$u$可交换的元素组成；但由于(3)，

$$
u^{-q} s u^q = s^{q p^r} = s,
$$

因此 $u^q \in Z$ 和结论 $Z$ 不是离散的。 由于$Z$是局部紧致的，我们可以将注意力集中在$K$是可交换的情况。 $K$中的子$\mathbf{F}_p$代数$\mathbf{F}_p[s]$则从$s^{q-1} = 1$开始是有限域，并且显然对于这个域的每个元素是$y^q = y$，因此它与$S$相同并且同构于$\mathbf{F}_q$，因为$S \subset \mathbf{F}_p[s]$有$q$元素。 由于$S$的两个元素之和在$S$中，因此将每个形式幂级数$\sum_{i=0}^\infty s_i T^i \in \mathbf{F}_q[[T]]$映射到元素$\sum_{i=0}^\infty s_i u^i$的映射是环$\mathbf{F}_q[[T]]$到环$A$的双射同态，由此立即得出结论。

#### 推论 1 {#ac-vi-s9-thm-1-cor-1 .statement tag=04XX}

*每个局部紧致域*（不是离散的*）都是有限秩*超过其中心。

#### 推论 2 {#ac-vi-s9-thm-1-cor-2 .statement tag=04XY}

每个局部*紧凑域*都连接*或*完全断开； *如果*它是连通的，它*就*同构于$\mathbf{R}, \mathbf{C}$*或*$\mathbf{H}$。

如果域 $K$ 上的拓扑由超量绝对值定义，则$K$ 与此拓扑完全断开。

#### 注 {#ac-vi-s9-n3-rem-1 .statement tag=04XZ}

设$s$为整数$> 0$； $K = \mathbf{F}_q((T))$的子域$\mathbf{F}_q((T^s)) = L$在$K$、$e(K/L) = s$、$f(K/L) = 1$关闭。因此可以看出，$K$存在封闭的子域$L$，它们不是离散的，因此$e(K/L)$（和*更不必说*次数$[K:L]$）是任意大的（与特征0的局部紧凑域的情况相反，其中每个局部紧凑这样的域$K$中的子域$L$必然是包含$\mathbf{R}$或$\mathbf{Q}_p$，因此$[K:L]$是有界的）。

### 习题{#ac-vi-s9-exercises}

22. (a) 如果域 K 存在离散估值，证明 K 的代数闭包在 K 上无限大。

(b) 令 K 为域 $K_0$ 的有限生成扩张。证明，如果 K 不是 $K_0$ 上的代数，则 K 上存在离散估值 $v$，使得 $K_0$ 上有 $v(x) = 0$。

39

参见[习题为 § 9](exercises/s9/)。
