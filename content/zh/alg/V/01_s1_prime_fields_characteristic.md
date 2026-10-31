---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 1
section_title: Prime fields. Characteristic
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
pdf_pages: 0115-0123, 0259-0260
extraction: ocr
subsections:
    - "no": 1
      title: Prime fields
      page: 0
      pdf_page: 115
    - "no": 2
      title: Characteristic of a ring and of a field
      page: 2
      pdf_page: 116
    - "no": 3
      title: Commutative rings of characteristic p
      page: 3
      pdf_page: 117
    - "no": 4
      title: Perfect rings of characteristic p
      page: 5
      pdf_page: 119
    - "no": 5
      title: Characteristic exponent of a field. Perfect fields
      page: 7
      pdf_page: 121
    - "no": 6
      title: Characterization of polynomials with zero differential
      page: 7
      pdf_page: 121
statements: 23
exercises: 5
content_sha256: fac66829247f6ca4e892a6fbeb5b194bdd87cf6ba6dcf7830c0e818c60e53a8f
translated_from: content/en/alg/V/01_s1_prime_fields_characteristic.md
translation_method: google
source_content_sha256: 2397d756974854b3ee958d9e41606c68fd59ce8ff67222f074fcb59adc452c32
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 4570807e5b86d5a214ef7d5b41b203972e3f77ff314528345b19785240f81829
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 1。优质域。特征

### 1. 优质域

有理整数的环Z分数域称为有理数的域，记为Q(I，p. 117)。对于每个素数数 p 商环 $\mathbf{Z}/(p)$ 都是 p 元素的有限 $^1$ 域，在续集中用 $\mathbf{F}_p$ 表示。 域 Q 是无限的，因为它包含 Z，因此不与任何域 $\mathbf{F}_p$ 同构。如果 p 和 $p'$ 是不同的素数数，域 $\mathbf{F}_p$ 和 $\mathbf{F}_{p'}$ 具有不同的基数，因此不是同构的。

#### 定义 1 {#alg-v-s1-def-1 .statement tag=06G3}

如果域与 Q 或域 $\mathbf{F}_p$ 之一同构，则称其为素数。

Q 包含环 Z 的每个子域，因此 Z 的分数 Q 的域； $\mathbf{F}_p$ 中的每个子环必然等于 $\mathbf{F}_p$。因此，素数域的每个子域都必然等于它（下面Th.1的cf.Cor.2）。设 P 为素数域且 A 环；如果f和$f'$是P到A中的两个同态，那么$x \in P$的集合使得$f(x) = f'(x)$是P的子域，因此根据所说我们必须有$f = f'$。特别是，素数域中唯一的自同态是恒等映射。

$^1$ 通过滥用语言，如果其底层集合是有限的，那么环或域也是有限的。

#### 定理 1 {#alg-v-s1-thm-1 .statement tag=06G4}

— 令 $A$ 为环 ；假设存在$A$中的子域。那么$A$有唯一的子域$P$，它是素数域。此外，$P$包含在$A$的中心中以及$A$的每个子域中。

令$K$为$A$的子域，$A$的$C$中心，并放入$K' = K \cap C$；那么$K'$是$A$的子域。设$f$为$\mathbf{Z}$的唯一同态为$A$，$p$为核。 $A$中的每子环，特别是$K'$、包含于$f(\mathbf{Z})$；因此理想的$p$是素数（I，p. 116-117）。如果$p = (0)$，$\mathbf{Z}$到$K'$的同态$f$是单射；因此它从$\mathbf{Q}$的扩展（I，p. 116）到同构$\bar{f}$到$K'$的子域$P$。如果$p \neq (0)$，则严格存在正整数$p$，使得$p = (p)$（I，p. 111）；如果我们有$p = ab$、$a > 1$和$b > 1$，这将意味着$a \notin p, b \notin p$和$ab \in p$，这与$p$是素数这一事实相矛盾。因此，数 $p$ 是素数，并通过 $F_p = \mathbf{Z}/p$ 的商$f$ 定义同构到 $K'$ 的子域 $P$。在这两种情况下，$P$都是包含在$A$的中心$C$中的$A$的子域，并且它是素数域。设$L$为$A$中的子域；那么$P \cap L$是$P$的子域，并且由于$P$是素数，所以我们有$P \cap L = P$，从而$P \subset L$。如果$P'$是$A$的子域并且是素数域，那么根据前面所说的，$P \subset P'$，从而$P = P'$，因为$P'$是素数域。

#### 推论 1 {#alg-v-s1-thm-1-cor-1 .statement tag=06G5}

— 令 $K$ 为域。 $K$存在唯一的子域，它是素数域，并且这是$K$中最小的子域。

#### 推论 2 {#alg-v-s1-thm-1-cor-2 .statement tag=06G6}

— 要使域成为素数，它除了自身之外不应该有包含子域是必要且充分的。

### 2.环和域的特点

只有当$A$有子域时，我们才可以得到定义环$A$的特征。如果是这样，则令$f$为$\mathbf{Z}$到$A$的唯一环同态，并让$n$为正整数生成的的理想$\mathbf{Z}$，即$f$的核 （I，p. 111）；那么整数$n$称为$A$的特征。

令 $A$ 为环，为其定义特征；那么 $A$ 不会约化为 0。到 Th。 1 $A$存在唯一的子域$P$，它是素数域；我们将其称为$A$的素数子域。截至周四证明。 1.有以下两种可能：
a) $A$的特征为0，$P$与$Q$同构的，
b) $A$的特征是素数数$p$，$P$与$\mathbf{F}_p$同构的。

若$A$的特征为零，则$Q$到$A$存在唯一的环同态；它的像是$A$的质数子域，包含在$A$的中心中。 因此，存在唯一与环结构兼容的$A$的$Q$-代数结构。 当$A$的特征是素数数$p$时，我们在替换域$Q$乘域$\mathbf{F}_p$上有相应的属性。

#### 命题 1 {#alg-v-s1-prop-1 .statement tag=06G7}

— 令 $A$ 为环，不减至 0。
a) 为了使 $A$ 具有特征 0，对于每个整数 $n \neq$，$A$ 的映射 $x \mapsto n \cdot x$ 自身应该是双射的是必要且充分的

b) 设 $p$ 为素数数。为了使$A$具有特征$p$，$p \cdot x = 0$对于所有$x \in A$是必要且充分的。

设$f$为$\mathbf{Z}$的唯一同态入$A$；对于整数$n$和$A$中的每个$x$，我们都有$n \cdot x = f(n)x$。为了使$A$具有特征0，$f$应将$\mathbf{Q}$的扩展至同态转化为$A$，即对于每个$n \neq 0$，$f(n)$应在$A$可逆（I，p. 113）；这就证明了$a$。同样，要使$A$具有特征$p$，$f$应消灭$p\mathbf{Z}$，即$f(p) = 0$，或者对于所有$x \in A$，$p \cdot x = 0$是必要且充分的；这就证明了$b$。

让我们假设 $A$ 不一定是交换域。 $A$ 的中心是（可交换的）域；因此定义了$A$的特征和素数子域。

#### 注 1 {#alg-v-s1-n2-rem-1 .statement tag=06G8}

令$A$和$A'$为两个不减为0的环。假设定义了$A$的特征，并且$A$中有同态$u$进入$A'$。 $A$的素数子域在$u$下的像是$A'$的子域$P'$，与$P$同构的，因此也是素数。由此可见$A'$的特征被定义并且等于$A$的特征。如果$A$和$A'$的特征为0（分别为$p \neq 0$），则映射$u$是代数的同态超过$\mathbf{Q}$（分别为$\mathbf{F}_p$）。

#### 注 2 {#alg-v-s1-n2-rem-2 .statement tag=06G9}

注 1 表明，如果 $A$ 是特征 0 的环（分别为 $p \neq 0$），则任何环 $A'$ 包含 $A$ 与子环或任何 的商都成立$A$ 由双面理想$a \neq A$。特别地，如果$K$是域，$K$的每个子域和$K$的每个扩张域都具有与$K$相同的特征。

#### 注 3 {#alg-v-s1-n2-rem-3 .statement tag=06GA}

令 $A$ 为代数，而不是在域 $K$ 上减少到 0。由于$K$到$A$的映射$\lambda \mapsto \lambda \cdot 1$为环同态，注1表明$A$的特性已定义并且等于$K$的特性。

#### 注 4 {#alg-v-s1-n2-rem-4 .statement tag=06GB}

由于域$\mathbf{Q}$是无穷大，因此特征0的每个环都是无穷大；由此可见，每个有限域都具有非零特征。

#### 注 5 {#alg-v-s1-n2-rem-5 .statement tag=06GC}

设$A$为不减至0的环，其加法群为无扭$\mathbf{Z}$模，并放入$B = \mathbf{Q} \otimes_{\mathbf{Z}} A$。 $A$的映射$x \mapsto 1 \otimes x$到$B$是单射（II，p. 314），因此$A$同构于特征0的环的子环。

### 3. 特征p的交换环

在这个数和下面的数中$p$表示素数数。

#### 定理 2 {#alg-v-s1-thm-2 .statement tag=06GD}

— 令 $A$ 为特征 $p$ 的交换环。 映射$a \mapsto a^p$是环$A$的自同态，也就是说，我们有关系

(1) $$(a + b)^p = a^p + b^p$$
(2) $$(ab)^p = a^p b^p$$

对于$A$中的$a, b$。

公式 (2) 由$A$ 的交换律推出。为了证明(1)，我们使用二项式公式$(a + b)^p = a^p + b^p + \sum_{i=1}^{p-1} \binom{p}{i} \cdot a^i b^{p-i}$；由于$p \cdot x = 0$对于所有$x \in A$，只需证明以下引理：

#### 引理 1 {#alg-v-s1-lem-1 .statement tag=06GE}

设$p$是1到$p - 1$范围内的素数数和$i$整数，则二项式系数$\binom{p}{i}$是整数能被$p$整除。

我们以归纳对$i$进行争论，案例$i = 1$是直接的从公式$\binom{p}{1} = p$。假设 $2 \leq i \leq p - 1$ 和 $\binom{i}{i-1}$ 能被 $p$整除。然后整数$i \binom{p}{i} = (p - i + 1) \binom{p}{i-1}$属于到$\mathbf{Z}$的素理想$p\mathbf{Z}$；从$i \notin p\mathbf{Z}$开始，我们有$\binom{p}{i} \in p\mathbf{Z}$，然后是引理。

令$A$为特征$p$和$f$整数$\geq 0$的交换环。来自 Th。 2 我们通过$f$上的归纳推出映射$a \mapsto a^{p^f}$是环$A$的自同态。特别是我们有关系

$$
(a_1 + \cdots + a_n)^{p^f} = a_1^{p^f} + \cdots + a_n^{p^f}
$$

对于$A$中的任何$a_1, \ldots, a_n$。 映射 $a \mapsto a^p$ 是有时，称为 $A$ 的 *Frobenius 自同态*。取$A = \mathbf{F}_p$和$a_i = 1$，我们从(3)关系得到：

$$
n^{p^f} \equiv n \mod p \quad (n \in \mathbf{Z}, f \in \mathbf{N}) .
$$

For each subset $S$ of $A$ we denote by $S^{p^f}$ the set of elements of $A$ of the form $x^{p^f}$ with $x \in S$^1. 特别地，如果$K$是$A$中的子环，则集合$K^{p^f}$是$A$中的子环。 如果$K$是$A$的子环和$A$的$S$子集，我们用$K \cup S$生成的$A$的$K[S]$子环来表示；当$A$为域时，我们用$K[S]$的分数的$K(S)$域来表示，即$K \cup S$生成的$A$的子域。

#### 命题 2 {#alg-v-s1-prop-2 .statement tag=06GF}

— *令$A$为特征$p$的交换环，$A$的$K$子环，$A$的$S$子集和$f$正整数。*

a) *我们有$K[S]^{p^f} = K^{p^f}[S^{p^f}]$，如果$A$是域，则$K(S)^{p^f} = K^{p^f}(S^{p^f})$。*

b) *如果$K$-模块$K[S]$由$A$的元素的族$(a_i)_{i \in I}$生成，则$K$-模块$K[S^{p^f}]$由$(a_i^{p^f})_{i \in I'}$族生成*

由于$K[S]$是$K \cup S$生成的$A$的子环，因此环$A$的自同态$\pi : a \mapsto a^{p^f}$下的像$KISlp^f$是$A$生成的子环 $\pi$、从而 $K[S]^{p^f} = K^{p^f}[S^{p^f}]$ 下的$K \cup S$ 像 $K^{p^f} \cup S^{p^f}$。 域的情况类似处理；这证明了a）。

很明显，家族$(a_i^{p^f})_{i \in I}$生成$K^{p^f}$-模块$K[S]^{p^f}$。 $K$-模块$K[S^{p^f}]$由形式$x_1^{p^f} \cdots x_n^{p^f} = (x, \ldots x_n)^{p^f}$的乘积生成，$x_1, \ldots, x_n$在$S$中任意生成，因此也由集合$K[S]^{p^f}$生成。 断言 b) 直接由此得出。

^1 当然，集合$S^{p^f}$不应与$p^f$集合等于$S$的集合乘积混淆，也不应与$p^f$元素的乘积集合混淆属于至 $S$。

### 4. 特征p完美环

#### 定义 2 {#alg-v-s1-def-2 .statement tag=06GG}

— 特征 $p \neq 0$ 的环 $A$ 被认为是完美的，如果它是可交换的并且映射 $a \mapsto a^p$ 是双射的。

如果环$A$是特征$p$的完美，映射$a \mapsto a^{p^f}$对于每个整数$f \geq 0$是环$A$自同构； 自同构的逆数用$a \mapsto a^{1/p^f}$或$a \mapsto a^{p^{-f}}$表示，而$A$的子集$S$的像则写成自同构写为$S^{1/p^f}$或$S^{p^{-f}}$。很明显，$(a^{p^e})^{p^f} = a^{p^{e+f}}$对于所有$a \in A$和任何整数$e$和$f$（无论符号）。

令$A$为特征$p$的交换环。对于每个整数$f \geq 0$，让我们为自同态$a \mapsto a^p$的核或环$A$写出$\mathfrak{n}_f$。那么$(\mathfrak{n}_f)_{f \geq 0}$就是$A$的理想的递增序列；由于每个正整数都以$p$的幂为大，所以理想的$\mathfrak{n} = \bigcup_{f \geq 0} \mathfrak{n}_f$由$A$的所有幂零元组成。特别是，如果$A$是完美的，则$A$的每个幂零元都是零。

#### 定义 3 {#alg-v-s1-def-3 .statement tag=06GH}

— 令 $A$ 为特征 $p \neq 0$ 的交换环。通过$A$的完美闭包，我们理解对$(A, u)$，其中$A$是特征$p$的完美环，$u$是$A$的同态到$A$满足以下泛性质：

(PC) *如果 B 是特征 p 的完美环，v 是 A 到 B 的同态，则存在 A 到 B 的唯一同态 h，使得 $v = h \circ u$。*

泛性质 (PC) 立即暗示完美闭包的唯一性，在以下意义上：如果$(A, u)$和$(A', u')$是$A$的两个完美闭包，则存在$A$到$A'$的唯一同构$h$这样 $u' = h \circ u$ (cf. *E, IV*, p. 23)。我们现在将建立完美闭包的“存在”：

#### 定理 3 {#alg-v-s1-thm-3 .statement tag=06GI}

— 令 $A$ 为特征 $p \neq 0$ 的交换环。存在$A$的完美闭包$(A, u)$。此外，$u$的核是$A$的所有幂零元的集合，并且对于每个$x \in A$，存在整数$n \geq 0$使得$x^{p^n} \in u(A)$。

对于每个整数$n \geq 0$，放入$A_n = A$；当$m \geq n$我们将$A_n$的定义同态$\pi_{m,n}$通过$\pi_{m,n}(a) = a^{p^{m-n}}$转换为$A_m$时。由此我们得到环 $(A_n, \pi_{m,n})$ (I, p. 120) 的直接系统；令$A$为该系统的直极限和$A_n = A$的$u_n$典范同态代入$A$；我们还放了$u = u_0$。由 $u$ 直极限核 $\mathfrak{n}$ 构造为同态 π_{n,0} 核并：a \mapsto $A$ 的 a^{p^n} 成$A$，因此它由$A$的所有幂零元组成。 环$A$可通过V、p. 3的注 1交换特征$p$。

环 $A$ 是子环升序的序列 $(u, (A))_n$ 的并。我们有$u_n(A)^{p^n} = A$；因此，对于每个$x \in \hat{A}$，存在整数$n \geq 0$，使得$x^{p^n} \in u(A)$。我们还有$u_n(A) = u_{n+1}(A)^p$、从而$\hat{A}^p = A$。令 $x \in A$ 使得 $x^p = 0$； 选择整数$n \geq 1$和元素$a \in A$使得$x = u_n(a)$。那么我们就有$u_{n-1}(a) = u_n(a)^p = 0$；通过直极限的定义，存在整数$m$，使得$\pi_m^{1,n-1}(a) = 0$，即$a^{p^{m-n}} = 0$。因此我们有$\pi_{m,n}(a) = 0$，从而$u_n(a) = 0$，即$x = 0$。因此环$A$是$p$的完美特征。

令$v$为$A$的同态，成为特征$p$的完美环$B$。对于每个整数$n \geq 0$，映射$b \mapsto b^{p^n}$是$B$的自同构，因此存在$A, = A$的同态$v_n$到$B$，特征为$v(a) = v_n(a)^{p^n}$。然后我们有 $v_m \circ \pi_{m,n} = v_n$ 对应 $m \geq n \geq 0$；通过直极限的定义，存在$A$的同态$h$进入$B$，使得$v_n = h \circ u$，对于所有$n \geq 0$；特别是我们有$v = v_0 = h \circ u_0 = h \circ u$。最后让$h'$是$A$的同态到$B$，这样$h' \circ u = v$。设 $x \in A$；正如我们所看到的，存在整数$n \geq 0$和元素$a \in A$使得$x^{p^n} = u(a)$。然后我们有

$$
h(x)^{p^n} = h(u(a)) = v(a) = h'(u(a)) = h'(x)^{p^n},
$$

由于$B$是完美的，我们找到$h(x) = h'(x)$。因此我们有$h' = h$，这完成了证明，$(A, u)$是$A$的完美闭包。

#### 命题 3 {#alg-v-s1-prop-3 .statement tag=06GJ}

— *令$B$是特征$p$和$A$子环特征$B$的完美环。写出$\mathbf{A}^{p^{-\infty}} = \bigcup_{f \geq 0} \mathbf{A}^{p^{-f}}$并用$\mathbf{A}^{p^{-\infty}}$中$A$的$j$典范嵌入表示。那么$\mathbf{A}^{p^{-\infty}}$是$B$包含$A$的最小的完美子环，$(\mathbf{A}^{p^{-\infty}}, j)$是$A$的完美闭包。*

对于每个整数 $f \in \mathbf{Z}$ 表示为 $\pi_f$ 自同构 $b \mapsto b^{p^f}$ of $B$。 $B$（对于$f \geq 0$）的子环$\pi_{-f}(A)$的序列是升序，因此它的并$\mathbf{A}^{p^{-\infty}}$是$B$的子环。我们有$\pi_1(\mathbf{A}^{p^{-\infty}}) = \bigcup_{f \geq 0} \pi_{-(f-1)}(A) = \mathbf{A}^{p^{-m}}$，因此$\mathbf{A}^{p^{-\infty}}$是$B$的完美子环。最后让$B_0$成为$B$包含$A$的完美子环；对于每个整数$f \geq 0$，我们有$\pi_{-f}(A) \subset \pi_{-f}(B_0) = B_0$，从而$\mathbf{A}^{p^{-\infty}} \subset B_0$。

如果$v$是将$A$的同态转化为特征$p$的完美环$B'$，那么对于每个整数$f \geq 0$，我们可以将$\pi_{-f}(A)$的定义同态$h_f$转化为$B'$ 乘以 $h_f(\pi_{-f}(a)) = v(a)^{p^{-f}}$ 对于所有 $a \in A$。 我们立即看到$h_{f+1}$与$h_f$在$\pi_{-f}(A)$上一致；因此，对于所有$f \geq 0$，$\mathbf{A}^{p^{-\infty}}$存在同态$h$到$B'$，其中诱导$h_f$在$\pi_{-f}(A)$上，特别是$h$扩展$h_0 = v$。 如果在B中$h'$是$v$的另一个扩张到$A^{p^{-\infty}}$的同态，则可以如Th的证明那样成立等式$h' = h$。 3.

### 5. 域的特征指数。 完美域

设$K$为域。 By the *characteristic exponent* of $K$ we understand the integer equal to *1* if $K$ is of characteristic 0, and equal to the characteristic of $K$ when this is non-zero.

#### 命题 4 {#alg-v-s1-prop-4 .statement tag=06GK}

— *令$K$为特征指数q的域。对于每个整数 $f \geq 0$ 映射 $x \mapsto x^{q^f}$ 是 K 的同构在其子域之一上（由 $K^{q^f}$ 表示）。*
这是从 Th 得出的。当 q ≠ 1 时为 2，当 q = 1 时为平凡。
同样，对于特征指数 q 的 $A$ 是域的情况，可以使用扩展命题 2，q = *1* 的情况是微不足道的。

#### 定义 4 {#alg-v-s1-def-4 .statement tag=06GL}

— *域如果我们有 $K^q = K$，则特征指数 q 的 K 被认为是完美的。当$K^q \neq K$时，K称为不完美。*
由此，如果定义域是特征0，或者如果它是Def意义上的特征$p \neq 0$的完美环，则它是完美的。 2. 如果$K$是特征$p \neq 0$的域且$(K, u)$是$K$的完美闭包，那么根据命题3 *(V, p. 6)*，K是域，$u$是K的同构子域共 $\hat{K}$。人们经常将$K$与$\hat{K}$中$u$下的像进行识别，因此我们有$\hat{K} = K^{p^{-\infty}}$（命题**3**）。
令K为特征*0*的域；那么$K$的特征指数就是*1*。按照惯例，记号$x^{q^{-f}}$和$S^{q^{-f}}$分别表示x和S*（对于$K$的元素$x$和$K$的子集S）*。特别是我们输入$K^{q^{-\infty}} = K$，并且我们同意将$K$的完美闭包取为$K$。

#### 命题 5 {#alg-v-s1-prop-5 .statement tag=06GM}

— *如果 K 是特征 0 的域，或者是有限的，\* 或代数闭 \*，那么它是完美的。特别是每个质数域都是完美的。*
假设$K$具有特征$p \neq 0$。如果$K$是有限的，则$K$的子域$K^p$与$K$、从而$K^p = K$具有相同的基数。 \* 如果 $K$ 是代数闭的，则对于每个 $a \in K$，多项式 $X^p - a$ 在 $K$ 中具有根 $x$ *(V, p. 20, Def. 1)* 从而 $x^p = a$所以$K^p = K$。 \* 最后，素数域的特征为 *0* 或有限。
令$K_0$为特征$p \neq 0$的域，在$K_0$上的不确定$X$中为有理分式的$K = K_0(X)$域。那么$K$是*不完美的*，因为不存在$K$的元素$u(X)/v(X)$*（$K_0[X]$中的u，v多项式）*使得$(u(X)/v(X))^p = X$。把这个关系写在形式$u(X)^p = Xv(X)^p$中，比较两边的次数就可以看出。

### 6. 刻画具有零微分的多项式

#### 命题 6 {#alg-v-s1-prop-6 .statement tag=06GN}

— *令 K 为交换环，A 为 A 的元素 F 的多项式代数 $K[X_i]_{i \in I}$，且 S 集合使得 $dF = 0$。*

a) *如果 K 是特征 0 的环，则 S = K。*
b) *如果K是特征$p \neq 0$的环，则$S = K[X_i^p]_{i \in I}$；而且如果 K 是完美的，那么 $K = A^P$.*

A 的映射 $F \mapsto dF$ 转化为 A 的 K 微分的模 $\Omega_K(A)$ 是 K 线性且满足关系

$$
d(FF') = F \cdot dF' + F' \cdot dF
$$

（III，p. 569）。因此S是子代数。

当K的特征为$p \neq 0$时，放入$T = K[X_i^p]_{i \in I}$；因此，如果 K 是完美的，我们就有 $T = A^P$（$V$，p. 4，命题 2）；此外，对于所有$i \in I$，我们都有$d(X_i^p) = pX_i^{p-1} \cdot dX_i = 0$，因此包含 T 的子代数 S。如果K 的特征为0，我们放入$T = K$，仍然会发现$T \subset S$。仍有待证明 S 包含在 T 中。

对于I的每个有限子集J，令$A_J$为族$(X_j)_{j \in J}$生成的A的子代数。我们有$A_\emptyset = K$和$A = \bigcup_{J \in I} A_J$；因此，只要证明关系$S \cap A_J \subset T$就足够了，我们将在J的基数上通过归纳来完成它。因此，令J为I的有限子集，使得$S \cap A_J \subset T$，令i为$I - J$和$J' = J \cup \{ i \}$的元素。 A 的每个元素 F 都可以用一种方式写成形式

$$
F = \sum_{n=0}^\infty F_n \cdot X_i^n,
$$

对所有 $n \geq 0$ 使用 $F_n \in A_J$，然后

$$
dF = \sum_{n=0}^\infty X_i^n \cdot dF_n + \sum_{n=0}^\infty nX_i^{n-1}F_n \cdot dX_i.
$$

假设 F 属于至 S；族$(dX_r)_{r \in J}$是A-模$\Omega_K(A)$（III，p. 570）的基，$dF_n$是$j \in J$的微分$dX_j$的线性组合，因为$F_n \in A_J = K[X_j]_{j \in J}$。通过 (6)，我们对于每个整数 $n \geq 0$ 都有 $dF_n = 0$ 和 $nF_n = 0$。自$dF_n = 0$起，所有$n$的归纳假设$F_n \in T$。

a) 如果 K 的特征为 0，则根据命题 1，对于所有 $n \geq 1$、从而 $F_n = 0$，我们有 $nF_n = 0$（$V$、p. 2）；所以我们有$F = F_0$，从而$F \in T$。

b) 如果 K 具有特征 $p \neq 0$，则 A 是代数超过域 $\mathbf{F}_p$，并且关系 $nF_n = 0$ 意味着对于每个不可被 $p$ 整除的整数 $n$，有 $F_n = 0$。所以我们有$F = \sum_{m=0}^m F_{mp} X_i^{mp}$，从而$F \in T$

#### 注 {#alg-v-s1-n6-rem-1 .statement tag=06GO}

— 当 K 的加法群无扭转时，我们仍然有 $S = K$；这是从上面的证明或从V、p. 3中的注 5得出的。

#### 推论 {#alg-v-s1-n6-cor-1 .statement tag=06GP}

— 令 K 为域，F(X) 为系数为 K 的多项式，其导数 F'(X) 为零。
a) 如果 K 的特征为 0，则 F ∈ K。
b) 如果 K 的特征为 p ≠ 0，则存在多项式 G(X)，使得 F(X) = G(X^p)。
因为我们有 dF = F 。 dX = 0。

### 习题 {#alg-v-s1-exercises}

§ 1](exercises/s1/)参见[习题。
