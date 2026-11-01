---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 5
section_title: p-radical extensions
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.24-A V.26, A V.150-A V.151
pdf_pages: 0138-0140, 0264-0265
extraction: ocr
subsections:
    - "no": 1
      title: p-radical elements
      page: 24
      pdf_page: 138
    - "no": 2
      title: pradical extensions
      page: 25
      pdf_page: 139
statements: 8
exercises: 3
content_sha256: 08a28032ac2b32524f18ce9b4d4aea3019d47291b1d7c787c5be8956cea5d85f
translated_from: content/en/alg/V/05_s5_p_radical_extensions.md
translation_method: google
source_content_sha256: 3693c7ad10eed43de9af13fff4d3447ffd7fc25ca8cc3c3bf9505041a61ff985
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 6408515371d0171632f7e229ce3a0b0803828c4fd9dd872cd3fafd60428b5731
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 5。 *p*-激进的扩展

*在本段中，字母 p 表示整数，它是 1 或质数数。所有考虑的域都是特征指数p。当$p = 1$时，本段中所述的所有结果都是微不足道的。*

### 1. p 根式元素

#### 定义 1 {#alg-v-s5-def-1 .statement tag=06IZ}

*设 K 为 K 的域且 E 扩张。如果存在整数 $m \geq 0$ 使得 $x^{p^m} \in K$，则 E 的 n 元素 x 被称为 K 上的 p 根式；其中最小的整数称为 x 的高度（超过 K）。*

#### 命题 1 {#alg-v-s5-prop-1 .statement tag=06J0}

*设 E 为域 K 的扩张，x 为 k 上高度 e 的 p 根元素；把$a = x^{p^e}$。那么 $a \in K$ 和 x 在 K 上的最小多项式是 $X^{p^e} - a$：进一步我们有 $[K(x):K] = p^e$。*

只需证明多项式$X^{p^e} - a$在$K[X]$中不可约即可。通过 x 高度的定义，我们得到 $a \notin K^p$，因此从引理可以得出命题：

#### 引理 1 {#alg-v-s5-lem-1 .statement tag=06J1}

*设 K 为域和 K 的元素，使得 $a \notin K^p$。那么对于每个整数 $e \geq 0$，多项式 $f(X) = X^{p^e} - a$ 在 $K[X]$ 中是不可约的。*

令$\Omega$为$K$的代数闭包，并令b为$\Omega$的元素$a^{p^{-e}}$；我们用 g 表示 b 在 $K$ 上的最小多项式。我们有$f(X) = (X - b)^{p^e}$，因此$K[X]$中的每个不可约多项式，其中除$f$承认b为根，因此等于g。因此存在 (*IV*, p. 13, 命题 13) 整数 $q \geq 1$ 使得$f = g^q$；由于$f$的q除次数$p^e$，存在整数$e'$使得$0 \leq e' \leq e$和$q = p^{e'}$。如果c是g的常数项，则有$-a = c^q$；因为我们假设 a 不在 $K^p$ 内，所以我们必须有 $q = 1$，即 $f = g$，所以引理如下。

### 2. 实用扩展

#### 定义 2 {#alg-v-s5-def-2 .statement tag=06J2}

设 E 为域 K 的扩张。如果 E 的每个元素都是 K 上的 p 根，我们可以说 E 是 p 根$^1$（在 K 上）。在这种情况下，当 E 的元素高度中的集合被限制在上面并且我们认为 E 具有有限高度时，我们称 E 为有限高度。称 E 的高度为其元素高度中的最大值。

我们注完美域（特别是特征 0 的域）的每个 p 根扩展都是微不足道的。

令 K 为域.. K 的高度 0 的 p 根式扩展是平凡的扩张。 K 的每个 p 根扩展都是代数的。如果 E 是 K 的 p 根扩展，F 是 E 的 p 根扩展，则 F 是 K 的 p 根扩展：对于给定任何 $x \in F$，存在整数 $m \geq 0$ 使得 $x^{p^m} \in E$ 和整数 $n \geq 0$ 使得 $(x^{p^m})^{p^n} \in K$，即， $x^{p^m + n} \in K$。

#### 命题 2 {#alg-v-s5-prop-2 .statement tag=06J3}

令E为域K的扩张。对于每个整数$n \geq 0$，令$E_n$为E的元素的集合，即高度$\leq n$在K上的$p\text{-radical}$，并令$E_r$是 E 的所有元素中 K 上的 p 根式的集合。则 $(E_n)_{n \geq 0}$ 是 E 的子扩展的升序序列，其并是 $E_\infty$，$E_r$ 是包含于 K 中的最大的 p 根式扩展E.

对于每个整数 $n \geq 0$ 集合 $E_n$ 由 E 的所有元素 $x$ 组成，使得 $x^{p^n} \in K$；由于映射$x \mapsto x^{p^n}$是域E的自同态，我们推断$E_n$是E的子扩展。序列$(E_n)_{n \geq 0}$是升序的，并$E_r$因此$E_r$ 是 E 的子扩展（V、p. 11、命题 3）。很明显，$E_r$是K的p-根式扩展，并且$E_r$包含是E的每个子扩展，它是K上的p-根式。

#### 推出 {#alg-v-s5-n2-cor-1 .statement tag=06J4}

如果域 K 的扩张 E 由 $p\text{-radical}$ 元素的集合在 K 上生成，则它是 K 上的 p 根。

因为$E_r$是E的子扩展并且由假设$E = K(E_\infty)$从而$E = E_r$；所以 E 是 K 的 p 根式扩展。

在命题 2 的条件下，$E_r$ 被认为是 E 中 K 的相对 $p\text{-radical}$ 闭包。

我们将特别将命题 2 应用到 E 是 K 的代数闭扩张的情况；那么 E 是完美的，我们对所有 $n \geq 0$ 都有 $E_n = K^{p^{-n}}$。在这种情况下，我们用 E 的元素的 $K^{p^{-\infty}}$ 集合表示，它们是 K 上的 p 根；它是 E 的子域，它是 E 的子域升序序列 $(K^{p^{-n}})_{n > 0}$ 的并。根据命题 2，$K^{p^{-\infty}}$ 是 E 的最大的子扩展，它是 K 上的 p 根式；根据 V、p. 6、$K^{p^{-\infty}}$ 的命题 3，它是 K 的完美闭包，并且它也是 E 包含 K 的最小的完美子域。当 K 完美时，我们显然对所有 n 都有 $K = K^{p^{-n}} = K^{p^{-\infty}}$。如果 K 不完美，我们有 $K \neq K^P$，从而

$^1$ p 根式扩展也称为纯粹不可分的扩张或根式扩张。

$$
K^{p^{-n}} \neq (K^p)^{p^{-n}} = K^{p^{-(n-1)}}
$$
$n \geq 1$； E 的子域 $K^{p^{-n}}$ 两两不同，$K^{p^{-\infty}}$ 是 K 的无限次代数扩张。

#### 命题 3 {#alg-v-s5-prop-3 .statement tag=06J5}

— 设 K 为域，K 的 E 扩张域（K 为 K 上的 p 根），以及 K 的 $u$ 同态到完美域 F。则存在 E 到 F 的唯一同态 $v$ 延伸$u$。

设$E_n$为E的元素的集合，它是K上高度为$\leq n$的p根式。根据命题2，域E是子域的升序序列$(E_n)_{n \geq 0}$的并。设$v$为E到F延伸$u$的同态；对于任意 $x \in E_n$，我们有 $x^{p^n} \in K$、从而 $v(x)^{p^n} = v(x^{p^n}) = u(x^{p^n})$；因此，对于所有$n \geq 0$和所有$x \in E_n$，我们有$v(x) = u(x^{p^n})^{p^{-n}}$，$u$到E的扩张的从而唯一性。

设$n$为正整数；对于任何$x \in E_n$，我们有$x^{p^n} \in K$，并且由于F是完美的，我们可以通过$v_n(x) = u(x^{p^n})^{p^{-n}}$将F的定义元素$v_n(x)$。很明显，$v_n$ 是 $E_n$ 的同态到 F 中，$v_0 = u$ 以及 $E_n$ 上的 $v_{n+1}$ 诱导 $v_n$。因此，对于所有$n \geq 0$，存在E到F中的同态$v$归纳$v_n$在$E_n$上，特别是与$E_0 = K$上的$v_0 = u$重合。

#### 推论{#alg-v-s5-n2-cor-2 .statement tag=06J6}

— 对于域 K 的扩张 E 来说，要成为 K 的完美闭包，它必须是 K 的 p 根扩展，并且域 E 应该是完美的。

当 $p = 1$ 时，推论是微不足道的；假设$p \neq 1$。规定的条件在V、p. 5、Th之前是必要的。 3 ;根据命题 3，它们就足够了。

#### 命题 4 {#alg-v-s5-prop-4 .statement tag=06J7}

— 令 E 为域 K 的有限* 次数的 p 根扩展。则 $[E : K]$ 是 K 的特征指数 p 的幂。

由于 E 是 K 的有限次数的 p 根扩展，因此存在 E 的元素 $a_1, \ldots, a_m$，K 上的 p 根，使得 $E = K(a_1, \ldots, a_m)$。令 i 在 1 到 m 范围内；因为 $a_i$ 是更不必说 $K(a_1, \ldots, a_{i-1})$ 的 p 根式，次数
$$
n_i = [K(a_1, \ldots, a_i) : K(a_1, \ldots, a_{i-1})]
$$
是 p 的幂（V，p. 24，命题 1）。我们有$[E : K] = n_1 \ldots n_m$到V，p. 18，Th。 2、从而结果。

### 习题{#alg-v-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
