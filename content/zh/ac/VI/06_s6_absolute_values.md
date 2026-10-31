---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 6
section_title: Absolute values
lang: zh
source: ac-i-vii
book_pages: 403-411, 459-460
pdf_pages: 0421-0429, 0477-0478
extraction: ocr
subsections:
    - "no": 1
      title: PRELIMINARIES ON ABSOLUTE VALUES
      page: 403
      pdf_page: 421
    - "no": 2
      title: ULTRAMETRIC ABSOLUTE VALUES
      page: 405
      pdf_page: 423
    - "no": 3
      title: ABSOLUTE VALUES ON Q
      page: 406
      pdf_page: 424
    - "no": 4
      title: STRUCTURE OF FIELDS WITH A NON-ULTRAMETRIC ABSOLUTE VALUE
      page: 407
      pdf_page: 425
statements: 11
exercises: 2
content_sha256: 0066925781f94a7c07e38a7646b21e2dde8722f7869ea12273c53a3ee35684b9
translated_from: content/en/ac/VI/06_s6_absolute_values.md
translation_method: google
source_content_sha256: faa08a74b0921e5d2151aaa0990ac2856ad0a10c13dc6c2fca2752cb6b3771af
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 934cddf20bd4feaa591eccccb7c1d23ff83c2f3017f7c02182ff346669e5245e
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 6.绝对值

### 1.绝对值值的初步介绍

设$K$为域（可交换或不可交换）。回想一下（一般拓扑、章 IX, § 3, no. 2、定义 2），$K$ 上的绝对值是从 $K$ 到 $\mathbf{R}_+$ 满足的任何映射 $f$ 以下公理：

(VA,)关系$f(x) = 0$相当于$x = 0$。
(VAII) $f(xy) = f(x)f(y)$ 适用于 $K$ 中的所有 $x, y$。
(VAIll) $f(x + y) \leq f(x) + f(y)$ 对于 $K$ 中的所有 $x, y$。

从 (VA,) 和 (VAII) 可以得出 $f(1) = 1, f(-1) = 1$ 和
$$
f(x^{-1}) = \frac{1}{f(x)}
$$
$x \neq 0$。

对于从$K$到$\mathbf{R}$的映射$f$和实数$A > 0$，令$(\mathrm{U}_A)$表示关系
$$
f(x + y) \leq A \cdot \sup(f(x), f(y)) \quad \text{for all } x, y \text{ in } K.
$$

我们用映射$f$的$\mathscr{V}(K)$集合表示，从$K$到$\mathbf{R}_+$满足（VAI）和（VAII），并且存在$A > 0$（取决于$f$），使得$(\mathrm{U}_A)$成立。

注当且仅当$\in \mathscr{V}(K)$，然后，将$x = 1, y = 0$放入$(\mathrm{U}_A)$，
$$
1 = f(1) \leq A \cdot \sup(f(1), f(0)) = A.
$$

#### 命题 1 {#ac-vi-s6-prop-1 .statement tag=04VA}

对于从$K$到$\mathbf{R}$、满足(VA,)和(VAII)到属于到$\mathscr{V}(K)$的映射$f$，$f(1 + x)$以$x \in K$的集合为界是充分必要的这样$f(x) \leq 1$。

如果$f$满足$(\mathbf{U}_A)$，则$f(1 + x) \leq A$如果$f(x) \leq 1$。相反，假设 $f(x + 1) \leq A$ 对于 $x \in K$ 使得 $f(x) \leq 1$ （这意味着 $A \geq f(1) = 1$）；那么，如果$x = 0$或$y = 0$，满足条件$(\mathbf{U}_A)$；另一方面，如果$x \neq 0$和$y \neq 0$，我们可以假设例为$f(y) \leq f(x)$，因此，通过$(\mathbf{VA}_s)$，$f(yx^{-1}) \leq 1$，因此$f(1 + yx^{-1}) \leq A$，根据$(\mathbf{VA}_{II})$，$f(x + y)f(x)^{-1} \leq A$给出； 从而

$$
f(x + y) \leq Af(x) \leq A \sup(f(x), f(y)).
$$

如果$f$是$K$上的绝对值，则从$(\mathbf{VA}_{III})$开始，$f(n.1) \leq n$乘归纳在整数$n > 0$上；反之：

#### 命题 2 {#ac-vi-s6-prop-2 .statement tag=04VB}

*设$f$为$K$至$\mathbf{R}_+$属于至$\mathscr{V}(K)$中的映射；如果存在$C > 0$，使得$f(n.1) \leq C$对于每个整数$n > 0$，$f$是$K$上的绝对值。*

到$r > 0$的归纳，我们从$(\mathbf{U}_A)$关系推出

$$(1)$$
$$
f(x_1 + x_2 + \cdots + x_{2^r}) \leq A^r \sup_{1 \leq i \leq 2^r} f(x_i)
$$

对于每个家庭$(x_i)$$2^r$元素$K$。我们集合$n = 2^r - 1$；对于所有 $x \in K$，我们从 (1) 推出

$$
(f(1 + x))^n = f((1 + x)^n) = f\left( \sum_{i=0}^n \binom{n}{i} x^i \right) \leq A^r \sup \left( f\left( \binom{n}{i} \right) (f(x))^i \right)
$$
$$
\leq CA^r \sum_{i=0}^n \binom{n}{i} (f(x))^i = CA^r (1 + f(x))^n
$$

$f\left( \binom{n}{i} \right) \leq C \binom{n}{i}$；因此
$$
f(1 + x) \leq C^{1/n} A^{r/n} (1 + f(x)).
$$

让$r$趋于$+\infty$，对于所有$x \in K$，我们得到$f(1 + x) \leq 1 + f(x)$； 应用这个不等式，用$x$替换为$xy^{-1}$（其中$y \neq 0$）并考虑$(\mathbf{VA}_{II})$，我们得到关系$(\mathbf{VA}_{III})$，这证明了命题。

#### 推论 1 {#ac-vi-s6-prop-2-cor-1 .statement tag=04VC}

*要使映射$f$从$K$到$\mathbf{R}_+$成为绝对的值，满足条件$(\mathbf{VA}_I)$、$(\mathbf{VA}_{II})$和$(\mathbf{U}_2)$是充分必要的。

这是必要的，因为$(\mathbf{VA}_{II})$意味着
$$
f(x + y) \leq f(x) + f(y) \leq 2 \sup(f(x), f(y)).
$$

反之，假设$f$满足$(\mathbf{VA}_I)$、$(\mathbf{VA}_s)$和$(\mathbf{U}_2)$；对于每个整数$n > 0$，让$r$是至少整数使得$2^r \geq n$；如果将(1)中的$A$替换为2，指标$i \leq n$的$x_i$替换为1，指标$i > n$的$x_i$替换为0，我们得到
$$
f(n.1) \leq 2^r < 2n;
$$
那么命题 2 可以与$C = 2$一起应用，因此$f$是绝对的值。

#### 推论 2 {#ac-vi-s6-prop-2-cor-2 .statement tag=04VD}

对于$K$到$\mathbf{R}_+$到属于到$\mathscr{V}(K)$的映射$f$来说，它是形式$g^t$是充分必要的，其中$t > 0$和$g$是值的绝对值 $K$。

说$f$满足$(\mathbf{U}_A)$相当于说$f^s$满足$(\mathbf{U}_{A^s})$；由于存在$s > 0$使得$A^s \leq 2$，推论1表明对于$s$这样的值，$f^s$是绝对的值。

### 2. 绝对超距值

$K$ 到 $\mathbf{R}_+$ 的映射 $f$ 称为超量绝对值，如果它满足条件 $(\mathrm{VA}_I)$、$(\mathrm{VA}_{II})$ 和 $(\mathrm{U},)$（这显然意味着 $f$ 是绝对值） 值）。

#### 命题 3 {#ac-vi-s6-prop-3 .statement tag=04VE}

令$f$为$K$到$\mathbf{R}_+$中的映射。以下属性是等效的：
(a) $f$ 是超量绝对值值。
(b) $K$ 存在估价$v$，$\mathbf{R}$ 中有值，实数 $a$，使得$0 < a < 1$ 和$f = a''$。
(c) 每整数 $n > 0$ $f$ 属于至 $\mathscr{V}(K)$ 和 $f(n.1) \leq 1$。
(d) 对于所有 $s > 0$，$f^s$ 是绝对的值。

对于每个实数 $c$，使得 $0 < c < 1$、映射 $t \mapsto c^t$ 是有序群 $\mathbf{R}_+^*$ 上有序群 $\mathbf{R}$ 的同构（与通常的顺序相反）；这显示了 (a) 和 (b) 的等价。显然（a）意味着（c）； (c) 意味着 (d)，因为我们从 (c) 推断出
$$
(f(n.1))^s \leq 1 \leq n
$$
对于no. 1中的每个整数$n > 0$和命题2，表明$f''$是绝对的值。最后 (d) 意味着 (a)：对于 iff” 是绝对值，它满足 $(\mathbf{U}_2)$，因此 $f$ 对于所有 $s > 0$ 满足 $(\mathbf{U}_{2^{1/s}})$，因此也满足 $(\mathbf{U}_1)$，让 $s$ 趋于 $+\infty$。

#### 推出{#ac-vi-s6-n2-cor-1 .statement tag=04VF}

如果$K$是特征$p > 0$的（不一定可交换的）域，则$\mathscr{V}(K)$上的每个函数都是超度量绝对值。

每个非零元素 $z = n.1$ ($n$ 整数 $> 0$) 属于到 $K$ 的素数子域 $\mathbf{F}_p$，因此满足关系 $z^{p-1} = 1$，这意味着$f(z) = 1$，我们可以应用命题 3 (c)。

给定实数 $c$ 使得 $0 < c < 1$, 公式
$$
f(x) = c^{v(x)}, \quad v(x) = \log, f(x)
$$
因此，在 $K$ 上的超测量绝对值和$K$ 与实际值的估值之间建立一对一的对应。不正确的估值对应到不正确的绝对值（一般拓扑、章IX, § 3, no. 2）。令$v_1, v_2$为$K$的两个估值，真实值和$f_1, f_2$相应的绝对值；为了使$v_1$和$v_2$等价，$f_1$和$f_2$是等价的：$v_1$和$v_2$相当于说，关系$v_1(x) \geq 0$和$v_2(x) \geq 0$是等价的，或者关系$f_1(x) \leq 1$和$f_2(x) \leq 1$是等价的；因此，满足*常规拓扑*、章 IX, § 3, no. 2 中的应用命题 5 即可。此外（*loc.cit.*）为了使$f_1$和$f_2$在K上定义的拓扑相同，$f_1$和$f_2$等效是充分必要的。

### 3. Q 上绝对值

#### 命题 4 {#ac-vi-s6-prop-4 .statement tag=04VG}

*设$f$为$\mathbf{Q}$至$\mathbf{R}_+$属于至$\mathscr{V}(\mathbf{Q})$中的映射。然后：*

(i) *$f$ 是 $\mathbf{Q}$ 上的不正确绝对值值。*

(ii) *或者存在实数$a$和素数数$p$使得$0 < a < 1$和$f = a^{v_p}$，其中$v_p$是$p$-adic估值。*

(iii) *或者存在 $s > 0$ 使得 $f(x) = |x|^s$ 对于所有 $x \in \mathbf{Q}$。*

*在(iii)中，$f$是$\mathbf{Q}$上的绝对值，$0 < s \leq 1$是充分必要的。*

首先假设每整数 $n > 0$ 都有 $f(n) \leq 1$。到 no. 2 的命题 3 时，存在实数 $b$ 以及$\mathbf{Q}$ 的估值$v$，使得$0 < b < 1$ 和$f = b^v$。现在，我们知道（§ 3, no. 4，*例 4*）$\mathbf{Q}$上唯一的估值是（最多等价）不正确的估值和$p$-adic估值$v_p$；因此，我们有情况 (i) 或情况 (ii)。

假设从现在开始存在整数$h > 0$使得$f(h) > 1$；由no. 1，推论2到命题2，存在数$\rho > 0$，使得$f^\rho$是绝对的值；让我们写

$$
g(x) = \rho \log(f(x))/\log|x|
$$

对于每个有理数数 $x \neq 0$。设$a, b$为两个整数$\geq 2$；对于每个整数$n \geq 2$，让$q(n)$表示$n \log a/\log b$的积分部分，在其他字中，至少整数$m$使得$a^n < b^{m+1}$；因此，$a^n$到基$b$的展开是

$$
a^n = c_0 + c_1 b + \ldots + c_{q(n)} b^{q(n)}
$$

其中 $0 \leq c_i < b$ 代表 $0 \leq i \leq q(n)$。由于 $f^\rho$ 是绝对值，$f^\rho(c_i) \leq c_i \leq b$，因此我们从 (2) 推出

$$
(f(a))^{n\rho} = (f(a^n))^\rho \leq b(1 + (f(b))^\rho + \ldots + (f(b))^{q(n)\rho})
$$
$$
\leq b(q(n) + 1)(\sup(1, (f(b))^\rho))^{q(n)}.
$$

对不等式两边取对数除以$n \log a$，得到

$$
g(a) \leq \frac{\log b}{n \log a} + \frac{\log(q(n) + 1)}{q(n)} \cdot \frac{q(n)}{n \log a} + \frac{\sup(0, \rho \log f(b))}{\log a} \cdot \frac{q(n)}{n}.
$$

注现在随着$n$趋向于$+\infty$，$q(n)/n$趋向于$\log a/\log b$；因此 $q(n)$ 趋于 $+\infty$ 并且

$$
\log(q(n) + 1)/q(n)
$$

趋于 0（实数变量的函数，章III, § 2, no. 1）。将极限代入(3)，我们得到

(4) $$
g(a) \leq \frac{\sup(0, \rho \log f(b))}{\log b} = \sup(0, g(b)).
$$

但是$f(h) > 1$、从而$g(h) > 0$；如果在(4)中将$a$替换为$h$，我们得到$\sup(0, g(b)) > 0$，因此

$$
\sup(0, g(b)) = g(b).
$$

然后，对于任何至少等于 2 的整数 $a, b$，$g(a) \leq g(b)$ 以及$g(a) = g(b)$，交换$a$ 和 $b$ 的角色。在其他字中，存在一个常数$\lambda$，使得每个整数$a \geq 2$都有$g(a) = A$；如果我们写 $s = \lambda / \rho$，那么每个整数 $a \geq 2$ 就是$f(a) = |a|^s$。作为$f(xy) = f(x)f(y)$和$f(-x) = f(x)$，$f(x) = |x|^s$适用于所有$x \in Q$。最后，如果$0 < s \leq 1$，我们知道$x \mapsto |x|^s$是绝对的值（一般拓扑、章IX, § 3, no. 2）；反之，如果$s$使得$x \mapsto |x|^s$是$Q$上的绝对值，则$(1 + 1)^s \leq 1^s + 1^s$，即$2^s \leq 2$、从而$s \leq 1$。

### 4. 结构 OF 域与非超距绝对值值

#### 定理 1（盖尔范德-马祖尔）{#ac-vi-s6-thm-1 .statement tag=04VH}

令 $K$ 为代数超过域 $\mathbf{R}$，并具有以下两个性质：
(1) $K$ 是（不一定可交换）域。
(2) $K$ 范数 $x \mapsto \|x\|$ 与$K$ 上的代数结构兼容（通用拓扑、章 IX, § 3, no. 7、定义 9）。
那么代数$K$同构于代数$\mathbf{R}, \mathbf{C}$或$\mathbf{H}$之一。

回想一下（前述），对于$K$中的所有$x, y$，可以总是假设$\|xy\| \leq \|x\| \cdot \|y\|$。我们将给出由范数定义的$K$拓扑（与代数结构兼容）。

(A) 第一种情况：$K$是可交换的并且存在$j \in K$使得$j^2 = -1$

那么域$\mathbf{C}$的同构$\sigma$存在于$K$的子域上，使得$\mathbf{R}$中的$\xi, \eta$有$\sigma(\xi + i\eta) = \xi . 1 + \eta . j$。我们将通过反证法证明$K = \sigma(\mathbf{C})$。假设存在$x \in K - \sigma(\mathbf{C})$；因此，对于所有 $z \in \mathbf{C}, x - \sigma(z)$ 在 $K$ 中都是可逆的；让我们写$F(z) = (x - \sigma(z))^{-1}$；因为 $\sigma$ 是连续的，并且逆矩阵在 $K$ 上是连续的（一般拓扑、章 IX, § 3, no. 7、命题 13 应用于 $K$ 的补全代数），$F$ 是连续的映射 $\mathbf{C}$ 至 $K$。而且，我们可以写$z \neq 0$

$$
F(z) = (\sigma(z))^{-1}(x(\sigma(z))^{-1} - 1)^{-1}.
$$

但是，随着$z$在$\mathbf{C}$中趋于无穷大，$(\sigma(z))^{-1} = \sigma(z^{-1})$趋于0，可以看出$F(z)$趋于0；在其他字中，$z \mapsto \|F(z)\|$是$\mathbf{C}$上的连续实值函数、$\geq 0$，在点无穷大处趋于0，因此可以将其视为通过邻接获得的紧凑空间$\tilde{C}$上的连续函数到无穷远$C$点。因此，$C$上$\| F \|$的最小上界$a$是有限的，并且复数$z$的$> 0$和集合$P$，使得$\| F(z) \| = a$是封闭且非空的（*一般拓扑*、章 IV, § 6, no. 1、定理 1)。

令 $z \in P$；让我们写出$y = x - \sigma(z)$，并让$t$为复数$\neq 0$，这样$\| \sigma(t) \| < \alpha^{-1}$，从而$\| \sigma(t) \cdot y^{-1} \| < 1$除以$a$的定义。因此，$(\sigma(t) y^{-1})^n$的序列和$n(\sigma(t) y^{-1})^n$在$K$中趋于0，就像$n$趋于$+\infty$一样，$R$中范数的相应的序列也是如此。另一方面注对于每个多项式 $H(T) = \prod_{k=1}^p (T - \sigma(c_k))$，其中 $c_k$ 不同复数，在有理数函数的域 $K(T)$ 中

$$
\frac{H'(T)}{H(T)} = \sum_{k=1}^p \frac{1}{T - \sigma(c_k)}
$$

我们将这个公式应用于多项式

$$
H(T) = T^n - (\sigma(t))^n = \prod_{k=0}^{n-1} (T - \sigma(\omega_n^k t)),
$$

其中 $\omega_n = \exp(2\pi i / n)$，并替换为 $T$ 元素 $y \in K$，这与所有 $\sigma(\omega_n^k t)$ 不同。由此可见（在交换域$K$）

$$
\frac{ny^{n-1}}{y^n - (\sigma(t))^n} = \frac{1}{y - \sigma(t)} + \sum_{k=1}^{n-1} \frac{1}{y - \sigma(\omega_n^k t)}.
$$

考虑$F$和$y$的定义，我们得到

$$
\begin{align}
F(z + t) + \sum_{k=1}^{n-1} F(z + \omega_n^k t) - nF(z) \\
= \frac{ny^{n-1}}{y^n - (\sigma(t))^n} - \frac{n}{y} = \frac{1}{y} \cdot \frac{n(\sigma(t) y^{-1})^n}{1 - (\sigma(t) y^{-1})^n}.
\end{align}
$$

但凭借上述$t$和注的选择，(7)中的最后一个表达式趋于0，因为$n$趋于$+\infty$；因此

$$
\| F(z + t) \| = \lim_{n \to +\infty} \| nF(z) - \sum_{k=1}^{n-1} F(z + \omega_n^k t) \|.
$$

现在，$\| F(z) \| = \alpha$和$\| F(z + \omega_n^k t) \| \leq \alpha$由定义共$\alpha$、从而

$$
\| nF(z) - \sum_{k=1}^{n-1} F(z + \omega_n^k t) \| \geq n \| F(z) \| - \sum_{k=1}^{n-1} \| F(z + \omega_n^k t) \| \geq n \alpha - (n-1)\alpha = \alpha.
$$

因而，根据 (8)，令 n 趋于 $+\infty$，$\|F(z + t)\| \geq a$，并趋于定义 $a$，这意味着
$$
\|F(z + t)\| = \alpha,
$$
其他字$z + t \in P$。这证明集合$P$在$\mathbf{C}$中*开*；由于它也是闭且非空的且$\mathbf{C}$是连通的，因而$P = \mathbf{C}$和$\|F\|$在$\mathbf{C}$上恒定；因为这个函数在无穷远的点趋向于0，$\|F(z)\| = 0$在$\mathbf{C}$尤其是$\|F(0)\| = \|x^{-1}\| = 0$趋向于0，这是荒谬的。

(B) *第二种情况； K 是可交换的并且* $-1$ *不是 K* 的元素平方
令L为与$T^2 + 1$的K 根 j 邻接而得到的交换域； L 是向量空间超过 K，承认 $(1, j)$ 为基，L 显然是代数超过 $\mathbf{R}$。 显然，函数$x + yj \to \|x\| + \|y\|$在L上与范数兼容，与结构兼容，就像向量空间在$\mathbf{R}$上兼容；另一方面，对于L中的$z = x + yj, z' = x' + y'j$，
$$
\begin{align*}
\|zz'\| &= \|xx' - yy'\| + \|xy' + x'y\| \\
&\leq \|x\|.\|x'\| + \|y\|.\|y'\| + \|x\|.\|y'\| + \|x'\|.\|y\| \\
&= (\|x\| + \|y\|)(\|x'\| + \|y'\|) = \|z\|.\|z'\|.
\end{align*}
$$
由此定义的范数因此与L上的R-代数结构兼容。 通过情况 (A) L 与 $\mathbf{C}$ 同构于 R-代数；现在$\mathbf{C}$与$\mathbf{C}$不同的唯一子R代数是$\mathbf{R}$，因此K与$\mathbf{R}$同构的。

(C) *第三种情况：K 不可交换*
设 Z 为 K 的中心，并且 K 的 x 元素不在 Z 中； K 的子域 $Z(x)$ 是可交换的，K 上的范数与$Z(x)$ 上的R-代数结构兼容；由于凭借(A)和(B)，$Z \neq Z(x)$和Z以及$Z(x)$与$\mathbf{R}$或$\mathbf{C}$同构于R-代数，因此Z必然与$\mathbf{R}$和$Z(x)$与$\mathbf{C}$同构的。因而，对于所有$x \in K, Z(x)$，秩$\leq 2$在Z上。现在我们有以下引理：

#### 引理 1 {#ac-vi-s6-lem-1 .statement tag=04VI}

*令 D 为域和中心 L，使得对于所有 $x \in D, L(x)$ 是次数 $\leq m$ L 的扩张。那么 D 的秩超过 L 就是 $\leq m^2$。*

我们显然可以将注意力限制在$D \neq L$的情况。则 D 中存在次数 $> 1$ L 的有限*可分离*代数交换扩张 E (*代数*, 章 VIII, § 10, no. 3, 引理 1)；作为$E = L(x)$对于E中的一些合适的x（*代数*，章V, § 7, no. 7，命题12和章VII, § 5, no. 7），通过假设$[E : L] \leq m$。假设可分扩张 E 的取值使得 $[E : L]$ 是有限且尽可能大的，并考虑 D 中 E 的 *集中器* $E' \supset E$，即中心 E 的域，使得
$$
[D : E'] = [E : L] \leq m
$$

（代数，章VIII, § 10, no. 2，定理2）。若 E $\#$ E'，$\mathbf{E}'$ 中存在次数 $> 1$ $\mathbf{E}$ 的有限可分代数扩张 F (代数, 章 VIII, § 10, no. 3, 引理 1)；因而，F 将是次数 $> [\mathrm{E}: \mathrm{L}]$ 的 L (代数、章 V, § 7, no. 4、命题 7) 的有限可分代数扩张，与 E 的定义相反；因而$\mathbf{E}' = \mathbf{E}$，从而$[\mathrm{D}: \mathrm{L}] = [\mathrm{D}: \mathrm{E}][\mathrm{E}: \mathrm{L}] \leq m^2$。

将应用这个引理与$m = 2$对应到K，可以看出K是有限秩的R的非交换扩张域，因此同构于四元数$\mathbf{H}$的域（代数，章） VIII, § 11, no. 2、定理2)。

注 (1) 我们将在章中给出范数代数的 Gelfand-Mazur 定理的较短证明，它对于 R 上的每个 Hausdorff 局部凸拓扑代数 K 有效，并且其原理如下：它被减少（如情况 (B)）和(C))对于K是交换代数大于$\mathbf{C}$的情况；如果$x \in \mathbf{K} - \mathbf{C}.1$，我们考虑如上$\mathbf{C}$到K的映射$z \mapsto (x - z.1)^{-1}$，它在$\mathbf{C}$上连续且可微。对于局部凸空间 K 的对偶 $\mathbf{K}'$ 的每个元素 $x'$，$z \mapsto \langle (x - z.1)^{-1}, x' \rangle$ 是 $\mathbf{C}$ 上的有界积分函数，因此由刘维尔定理和我们结论恒定，如部分 (A) 定理 1 的证明，这对于所有$z \in \mathbf{C}$和所有$x' \in \mathbf{K}'$必然意味着$\langle (x - z.1)^{-1}, x' \rangle = 0$； Hahn-Banach 定理表明这个结论是荒谬的，因为$(x - z.1)^{-1} \neq 0$。 注定理 1 的证明部分 (A) 中的论证仅在外观上与上述不同，因为该论证只是用于证明解析函数的最大原理的特例，即对根的求和单位元和经过到极限相当于计算沿中心0的圆的积分$\int_{\gamma} \frac{\mathbf{F}(z + t)}{t} dt$，并且由于函数F的特殊形式，这里避免使用柯西公式。

#### 定理 2（奥斯特洛夫斯基）{#ac-vi-s6-thm-2 .statement tag=04VJ}

设 K 为 a（不一定可交换）域和 f 元素 $\mathscr{V}(K)$，它不是超度量绝对值。那么存在唯一的 K 的实数 $s > 0$ 和同构 j 到域 $\mathbf{R}, \mathbf{C}$ 或 $\mathbf{H}$ 之一的处处稠密子域，使得$f(x) = |j(x)|^s$ 对于所有$x \in K$ (*)。要使 f 成为 K 上的绝对值，$s \leq 1$ 是充分必要的。

根据 no. 2，推论命题 3，K 的特征为 0，因此代数大于 $\mathbf{Q}$；对于所有$x \in \mathbf{Q}$，我们写为$h(x) = f(x.1)$；显然$h \in \mathscr{V}(\mathbf{Q})$，因此可以应用no. 3中的命题 4；这个命题的叙述的情况 (i) 和 (ii) 都不成立，因为这意味着对于每个整数 $n > 0$ 都有 $f(n.1) \leq 1$，并且 f 将是超度量绝对值

(*) 在 $\mathbf{H}$ 上我们写 $|z|^2 = z.\bar{z} = \bar{z}.z$，$\bar{z}$ 是 $z$ 的共轭四元数。

no. 2, 命题 3. 则存在实数 s > 0，对于所有 x ∈ Q，h(x) = |x|^s，即 f(x.1) = |x|^s；我们写 g = f^{1/s}。那么对于每个整数 n，g ∈ V(K) 且 g(n.1) = n；因此，no. 1的命题2表明g是K上的绝对值。

对于 x ∈ Q 且 y ∈ K，g(xy) = |x|g(y)，因此 g 在 K 上是范数，与其 Q 代数结构兼容（在 Q 上通常是绝对值）。因此，K 的完成 K 是 Q = R 上的范数代数（一般拓扑、章 IX, § 3, no. 7）；令 ĝ 为 K 上的范数，即 g 的连续扩张。由于g是K上的绝对值，K是域，ĝ是K上的绝对值（一般拓扑，章IX, § 3, no. 3，命题6）。到定理 1 时，存在 K̂ R-代数同构到域 R、C 或 H 之一，并且 g'(x) = |j(x)|因此是 K̂ 上的绝对值；因为 K̂ 在 R 和 g' 上是有限维的，并且 ĝ 重合在子域 R 上。 K̂ 中的 1，g' = ĝ 由以下引理得到：

#### 引理 2 {#ac-vi-s6-lem-2 .statement tag=04VK}

设L为L的a（不一定可交换）域和K子域，使得L是K上的ajinite维左向量空间。设g为L上的绝对值，f其限制到K。如果K是完整的并且不离散对于 f，L 对于 g 是完备的；如果进一步 g' 在 L 上是另一个绝对值，并且对 K 具有相同的限制，则 g' = g。

由于g定义的拓扑是Hausdorff并且与L上的左向量K空间结构兼容，因此第一个断言来自拓扑向量空间，章I, § 2, no. 3，定理2。此外，L上的拓扑定义g 和 g' 是相同的（loc. cit.）；因此存在实数 s > 0 使得 g' = g^s （一般拓扑、章 IX, § 3, no. 2、命题 5）。令 x 为 K 的元素，使得 f(x) ≠ 1；方程 g'(x) = g(x) 证明 s = 1。

返回定理 2 的证明，可以看出，如果j 表示f 到K 的限制，则j 是K 的同构到R、C 或H 的处处稠密子域，且g(x) = |j(x)|对于 x ∈ K，从而 f(x) = |j(x)|^s。

最后注，iff是K上的绝对值，h是Q上的绝对值，且s ≤ 1 by no. 3，命题 4；反之，如果 s ≤ 1，则 f = g^s 是 K 上的绝对值，因为 g 是 (一般拓扑, 章 IX, § 3, no. 2)；这就证明了最后一个断言或叙述。

Remarks

(2) 如果 K 是域并且 R 上的范数代数，范数不一定是 K 上的绝对值；对于例, Ψ + iη → | Ψ| + |η| C 上的范数与其 R-代数结构兼容。

(3) 对于定理 1 的情况(C)的证明，不使用代数、章 VIII的一般结果，参见习题 2。

### 习题{#ac-vi-s6-exercises}

§ 6](exercises/s6/)参见[习题。
