---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 3
section_title: Algebraic extensions
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.15-A V.19, A V.147-A V.150
pdf_pages: 0129-0133, 0261-0264
extraction: ocr
subsections:
    - "no": 1
      title: Algebraic elements of an algebra
      page: 15
      pdf_page: 129
    - "no": 2
      title: Algebraic extensions
      page: 17
      pdf_page: 131
    - "no": 3
      title: Transitivity of algebraic extensions. Fields that are relatively algebraically closed in an extension field
      page: 19
      pdf_page: 133
statements: 18
exercises: 13
content_sha256: 90645c601efd436e2cab914d1b5c36ea11bd4da2556c72bf23d27b5e9e8ee7c9
translated_from: content/en/alg/V/03_s3_algebraic_extensions.md
translation_method: google
source_content_sha256: c809206feded65830ffb1a1abf8e7582212bebf99082b59eeb85c7c315e737bc
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: a57980bdb0b113a09dd83c7fc8cf933c46f93e337da0dd9dd7ea53ecec49991c
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 3。代数扩张

### 1. 代数的代数元素

令 A 为域 K 上的代数以及 A 的 x 元素。可能有两种情况：

a) 单项式族$(x^n)_{n \in \mathbf{N}}$在$K$之上是自由的。那么我们说$x$超越$K$。 $x$生成的$A$的子代数$K[x]$上存在多项式代数$K[X]$的同构，而后者在$K$上具有无限次数。

b) 存在整数$n \geq 1$使得单项式$1,\ x,\ \ldots,\ x^{n-1},\ x^n$线性相关；同样，在 $K[X]$ 中存在一个多项式 $f \neq 0$，使得 $f(x) = 0$。那么我们说$x$是$K$的代数。上面的性质中最小的整数$n \geq 1$满足称为$x$超过$K$的次数。如果$K$上$x$的次数是$n$，则单项式$1,\ x,\ \ldots,\ x^{n-1}$在$K$上线性无关，并且存在$K$的元素$a_0,\ a_1,\ \ldots,\ a_{n-1}$，使得
$$
x^n = a_0 + a_1 x + \cdots + a_{n-1} x^{n-1}
$$
首一多项式$f(X) = X^n - \sum_{k=0}^{n-1} a_k X^k$是次数$n$在$K[X]$中的唯一一元多项式，使得$f(x) = 0$；它被称为$x$超过$K$的最小多项式。

#### 定理 1 {#alg-v-s3-thm-1 .statement tag=06HI}

— Let $A$ be an algebra over a field $K$, $x$ an element of $A$ algebraic over $K$, $n$ the degree and $f$ the minimal polynomial of $x$ over $K$.

a) 对于多项式 $g \in K[X]$ 到满足 $g(x) = 0$，$g$ 应该是 $f$ 的倍数是充分必要的。

b) 映射 $g \mapsto g(x)$ 定义通过将代数 $K[X]/(f)$ 的商同构代入代数 $K[x]$，以及元素 $1,\ x,\ \ldots,\ x^{n-1}$ 形式 $K[x]$ 中的基超过$K$。特别是$[K[x]:K] = n$。

c) 假设$A$为整环。那么$K[x]$是域，$f$是$K[X]$中唯一的一元不可约多项式，使得$f(x) = 0$。

d) 为了使$x$在$A$中可逆，$f(0) \neq 0$是充分必要的；那么我们就有$x^{-1} \in K[x]$。

存在唯一代数同态$\varphi : K[X] \to A$使得$\varphi(X) = x$；对于每个$P \in K[X]$，我们都有$\varphi(P) = P(x)$，并且$\varphi$的像等于$K[x]$。设$a$为$\varphi$的核：通过构造，$x$在$K$属于到$a$的最小多项式$f$，它是次数的最小多项式$a$。因此（$IV$，p. 11，命题11）我们有$a = (f)$，从而$a$。 断言 $b$) 立即从 a) 和 Cor 得出。 $IV$、p. 11第 10 号提案。

假设$A$是整环。 代数 $K[x]$ 那么整环和有限次数超过$K$，因此它是域（$V$，p. 10，Cor.）。因此，$K[x]$的理想$(f)$是最大的，这意味着$f$在$K[X]$（$IV$，p. 13）中不可约。最后，令$g$为$K[X]$中的一调不可约多项式，使得$g(x) = 0$；由$a$）它是$f$的倍数，因此$g = f$，这证明了$c$）。

仍有待证明$d$）。存在次数$n-1$的多项式$g \in K[X]$和$K$的元素$a$，使得$f(X) = Xg(X) + a$、从而$f(0) = a$。如果$a = 0$，我们有$xg(x) = f(x) = 0$和$g(x) \neq 0$，那么$x$在$A$中不可逆。另一方面，如果$a \neq 0$，则我们有$x \cdot [-a^{-1}g(x)] = 1$，因此$x$在$A$和$x^{-1} = -a^{-1}g(x)$中可逆。

#### 推论 1 {#alg-v-s3-thm-1-cor-1 .statement tag=06HJ}

— 令 $A$ 为代数超过域 $K$。为了使$A$的元素$x$成为$K$的代数，$x$生成的$A$的子代数$K[x]$应该是有限次数超过$K$。特别是，如果$A$是有限次数超过$K$，则$A$的每个元素都是超过$K$的代数。

#### 推论 2 {#alg-v-s3-thm-1-cor-2 .statement tag=06HK}

— 设$E$为$K$的扩张，$E$上的$A$代数以及$K$上的$A$代数$x$元素。 Then $x$ is algebraic over $E$, the minimal polynomial of $x$ over $E$ divides the minimal polynomial of $x$ over $K$ and the degree of $x$ over $E$ is at most equal to the degree of $x$ over $K$.

For let $f$ be the minimal polynomial of $x$ over $K$;我们有$f(x) = 0$和$f \in E[X]$，因此$x$是$E$的代数，$f$是$x$在$E$上的最小多项式的倍数（Th.1，*a*）。

#### 注 {#alg-v-s3-n1-rem-1 .statement tag=06HL}

Let $E$ be an extension of a field $K$ and $x$ an element of $E$ which is root of a monic irreducible polynomial $f \in K[X]$. Th。 1, *c*) 然后表明 $f$ 是 $x$ 在 $K$ 上的最小多项式。

#### 例 1 {#alg-v-s3-n1-exa-1 .statement tag=06HM}

在复数$\mathbf{C}$的域中，数$i$是次数2在素数域$\mathbf{Q}$上的代数；如果$f(X) = X^2 + 1$，则$f(i) = 0$，$x^2 + 1 \neq 0$ 对于所有$x \in \mathbf{Q}$，因此$i \notin \mathbf{Q}$。 域 $\mathbf{Q}(i)$ 因此是扩张 / 次数 2 / $\mathbf{Q}$；它由所有数$a + bi$组成，其中$a, b$是有理数。同样，$i$是次数2对实数的域$\mathbf{R}$的代数，$\mathbf{C}$是$\mathbf{R}$的次数2的扩张。 \*

#### 例 2 {#alg-v-s3-n1-exa-2 .statement tag=06HN}

设$K$为域且$F$域$K(X)$有理数函数在$K$上的一个不定数。设$E$为$F$的子域$K(X^3)$；我们有$F = E(X)$，$X$是$E$的代数，因为它是环$E[Y]$的多项式$Y^3 - X^3$的根；这个多项式在 $E[Y]$ 中是不可约的，因为在相反的情况下，它将至少有第一个次数中的一个因子，然后将存在 $K[X]$ 的两个非零多项式 $u(X)$、$v(X)$，使得 $(u(X^3))^3 = X^3(v(X^3))^3$ 是荒谬的，因为如果$m$和$n$是$u$和$v$的次数，这意味着$9m = 9n + 3$或$3m = 3n + 1$。因此，域$F$是次数3除以$E$，并且$F$的每个元素都可以用一种方式写为线性组合$f(X^3) + Xg(X^3) + X^2 h(X^3)$，其中$f, g, h$是有理分式的三个$K(X)$。

#### 例 3 {#alg-v-s3-n1-exa-3 .statement tag=06HO}

\* 在实数的域$\mathbf{R}$中，可以证明$^1$数$\pi$超越素数域$\mathbf{Q}$。 \*

### 2.代数扩张

#### 定义 1 {#alg-v-s3-def-1 .statement tag=06HP}

— 如果 $E$ 的每个元素都是超过 $K$ 的代数，则域 $K$ 的扩张 $E$ 被称为代数（超过 $K$）。 $K$的扩张$E$不是代数的，称为超越（超过$K$）。

#### 命题 1 {#alg-v-s3-prop-1 .statement tag=06HQ}

— 为了使 $K$ 的扩张 $E$ 成为代数，$E$ 的每个子 K 代数 $A$ 应为域是充分必要的。

$^1$ 参见。 例 D. Hilbert，Gesammelte Abhandlungen，卷。 1、p. 1（柏林（施普林格），1932 年）。

条件是必要的：如果 $E$ 是 $K$ 的代数，且 $x \neq 0$ 是 $E$ 的子 K 代数 $A$ 的元素，则 $x^{-1} \in K[x] \subset A$ 乘以 $V$、p. 16、Th。 1、d)。因此$A$是域。

条件就足够了：如果满足并且$x$在$E$中是元素$\neq 0$，则环$K[x]$是域，因此$x^{-1} \in K[x]$；在其他字中，存在多项式$g \in K[X]$，使得$x^{-1} = g(x)$，或者还有$xg(x) - 1 = 0$；这表明$x$是$K$的代数，因此$E$是$K$的代数扩张。

#### 命题 2 {#alg-v-s3-prop-2 .statement tag=06HR}

— *如果 K 的扩张 E 为有限次数 n，则它是代数且次数超过 E 除 n 的每个元素的 K。*

因为，给定 $x \in E$，$[K(x):K]$ 是有限的，除 n ($V$，p. 10，Cor.1)，因此 $x$ 是 $K$ ($V$，p. 17，Cor.1) 的代数。

*对于有限域 (V, p. 24, 注 4) 的例代数闭包，存在无限次代数扩张。*

#### 定理 2 {#alg-v-s3-thm-2 .statement tag=06HS}

— *令 E 为 K 的有限生成的扩张，由元素 $a_1, ..., a_m$ 生成，它们是 K 上的代数；则 E 是 K 的有限次数扩张。如果 $a_i$ 次数超过 $K(a_1, a_2, ..., a_{i-1})$ 是 $n_i$（对于 $1 \leq i \leq m$），则 E 的次数超过 K 是 $n_1 n_2 ... n_m$ 和元素 E 比 K 的$a_1^{v_1} a_2^{v_2} ... a_m^{v_m}$ ($0 \leq v_i \leq n_i - 1$) 形式基。*

$K(a_1, a_2, ..., a_i)$ 超过$K(a_1, a_2, ..., a_{i-1})$ 的元素 $a_i^{v_i}$ ($0 \leq v_i \leq n_i - 1$) 形式基截至 Th。 1、b) $V$、p. 16；因此，定理紧随$m$上的归纳，来自II、p. 222的第25号提案。

#### 推论 1 {#alg-v-s3-thm-2-cor-1 .statement tag=06HT}

— *设 E 为 K 的扩张和 A 子集的 E 由……组成的元素，它们是 K 上的代数。然后 $K(A)$ 是 K 上的代数，我们有 $K[A] = K(A)$。*

对于每个$x \in K(A)$属于到域$K(F)$，其中F是$A$的有限子集（$V$，p. 11，Cor.）；现在$K(F)$是$K$的代数并且等于$K[F]$的Th。 2，因此$x$是$K$和$K(A) = K[A]$的代数。

#### 推论 2 {#alg-v-s3-thm-2-cor-2 .statement tag=06HU}

— *令L为L的K和E、F子扩展的扩张。如果 F 是 K 上的代数，则 $E \cup F$ 生成的 L 的子环 $K[E, F]$ 是域，与 $E(F)$ 一致并且是 E 上的代数。*

对于$F$的每个元素，在$K$上是代数，在$E$上也是代数（$V$，p. 17，Cor.2），因此$E(F)$是$E$的代数扩张，我们有$E(F) = E[F]$，作者：Cor。 1.

#### 注 1 {#alg-v-s3-n2-rem-1 .statement tag=06HV}

与Th的记号。 2、 $E = K[a_1, a_2, ..., a_n]$ 因此 $E$ 同构于商 $K[X_1, X_2, ..., X_m]/\mathfrak{a}$；由于$E$是域，$a$是$K[X_1, ..., X_m]$的极大理想。

#### 注 2 {#alg-v-s3-n2-rem-2 .statement tag=06HW}

令 $E$ 为 $K$ 的无限次代数扩张。由 Th. 2 存在序列 $(a_i)$，其中元素 $E$ 使得$a_i \notin K(a_1, a_2, ..., a_{i-1})$； Th。图2进一步表明，$K(a_1, a_2, ..., a_n)$超过$K$的次数取任意大的值。在其他字中，如果E是K的代数扩张，使得有限次数的E的子外延F在K上的次数[F : K]有界，则E是K的有限次数的扩张。

### 3. 代数扩张的传递性。 域在扩张域中相对代数封闭

#### 命题 3 {#alg-v-s3-prop-3 .statement tag=06HX}

— 令 E 和 F 为域 K 的两个扩张域，使得 K ⊂ E ⊂ F。对于 F 在 K 上的代数，E 在 K 上的代数和 F 在 E 上的代数是充分必要的。

条件是必要的，由V，p. 17，Cor。 2. 让我们证明它是充分的。令x为F的任意元素；它是 E 上的代数；设 g ∈ E[X] 为 E 上的最小多项式。如果 A 是 g 系数的（有限）集合，则 g ∈ K(A)[X]，因此 x 是 K(A) 上的代数，并且 K(A U {x}) = K(A)(x) 是 K(A) 上的有限次数。现在 A ⊂ E 和 E 是 K 上的代数，因此 K(A) 是 K 上的有限次数，乘以 Th。 2. 因此 (V, p. 10, Th.1), K(A U {x}) 在 K 上为有限次数，这表明 x 在 K 上是代数 (V, p. 18，命题 2)。

#### 定义 2 {#alg-v-s3-def-2 .statement tag=06HY}

— 域 E 的子域 K 被认为在 E 中是相对代数封闭的，如果 E 的每个元素是 K 上的代数，属于到 K。

同样的道理，K 是 E 中包含的 K 的唯一代数扩张。每个域 K 本身都是相对代数封闭的。在§ 4中，我们将研究域，它们在每个扩张域中是相对代数封闭的。

#### 命题 4 {#alg-v-s3-prop-4 .statement tag=06HZ}

— 令 E 为扩张 / 域 K； E 的元素的集合 L，是 K 上的代数形式 E 的子扩展，在 E 中相对代数封闭。

对于域 K(L) 是 K (Th. 2 的 Cor. 1) 的代数，因此 K(L) ⊂ L；由此可知 K(L) = L 并且 L 为域。另一方面，如果 x ∈ E 是 L 上的代数，那么它在 K 上也是如此（命题 3），因此属于到 L。

E 的所有元素在 K 上代数的 K 由……组成的扩张 L 称为 K 在 E 中的相对代数闭包；它是E中包含的K的最大的代数扩张。

### 习题 {#alg-v-s3-exercises}

§ 3](exercises/s3/)参见[习题。
