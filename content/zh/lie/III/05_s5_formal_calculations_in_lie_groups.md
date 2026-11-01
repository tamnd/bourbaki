---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: III
chapter_title: LIE GROUPS
section: 5
section_title: Formal calculations in Lie groups
lang: zh
source: lie-i-iii
book_pages: 297-304, 382-383
pdf_pages: 0315-0322, 0400-0401
extraction: ocr
subsections:
    - "no": 1
      title: THE COEFFICIENTS $c_{\alpha \beta \gamma}$
      page: 297
      pdf_page: 315
    - "no": 2
      title: BRACKET IN THE LIE ALGEBRA
      page: 298
      pdf_page: 316
    - "no": 3
      title: POWERS
      page: 300
      pdf_page: 318
    - "no": 4
      title: EXPONENTIAL
      page: 303
      pdf_page: 321
statements: 5
exercises: 2
content_sha256: 08fddbafdeefea2595d9cfcf83597eb6173b6f6d0f9d6a34dbe5d311d495659f
translated_from: content/en/lie/III/05_s5_formal_calculations_in_lie_groups.md
translation_method: google
source_content_sha256: 11ac709b8f3f88dc9c56e0725f4895fcc0f9592e0b472ff993cd89dad5d027d2
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: bca7a58df55159514e347fe8bc29d8d7197a137543606bc4664334a604d88f1d
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 5。 李群中的正式计算

令 $f, g$ 为两个形式的幂级数，且 $K$ 中的系数处于相同的不定式中，令 $f_i$（分别为 $g_i$）为次数 $i$ 的 $f$（分别为 $g$）的齐次分量。我们将写
$$
f \equiv g \mod \deg p
$$
如果 $f_i = g_i$ 为 $i < p$。

在本§中，G表示有限维$n$的李群胚芽； 基域 $K$ 假定为特征零。我们通过图表一劳永逸地认同，G中$e$的开邻域和$K^n$中0的开邻域U，因此$e$被识别为0。对于U中的$x, y$和$n \in \mathbf{Z}$，$x.y$表示G 中$x$和$y$的乘积和$x^{[m]}$$x$的第m个幂（当它们被定义时）。 $x \in U$的坐标用$x_1, x_2, \ldots, x_n$表示。

### 1. 系数 $c_{\alpha \beta \gamma}$

令$\Omega$为$(x, y) \in U \times U$的集合，使得$x.y$被定义且属于为U。则$\Omega$在$U \times U$中开，且$\Omega$的映射$(x, y) \mapsto x.y$在U中是解析的。因此，$z = x.y$的坐标$z_1, \ldots, z_n$承认展开作为关于$x_1, \ldots, x_n, y_1, \ldots, y_n$的幂原点的积分级数。因此，存在定义明确的常数 $c_{\alpha_1, \ldots, \alpha_n, \beta_1, \ldots, \beta_n, \gamma_1, \ldots, \gamma_n} \in K$，使得
$$
z_1^{\gamma_1} \cdots z_n^{\gamma_n} = \sum_{\alpha_1, \ldots, \beta_n \in \mathbf{N}} c_{\alpha_1, \ldots, \alpha_n, \beta_1, \ldots, \beta_n, \gamma_1, \ldots, \gamma_n} x_1^{\alpha_1} \cdots x_n^{\alpha_n} y_1^{\beta_1} \cdots y_n^{\beta_n}
$$
对于$\mathbf{N}$中的$\gamma_1, \ldots, \gamma_n$。采用可微分和解析流形，R的约定，我们将更简单地写出这些公式：
$$
(x.y)^{\gamma} = \sum_{\alpha, \beta \in \mathbf{N}^n} c_{\alpha, \beta, \gamma} x^{\alpha} y^{\beta} \quad (\gamma \in \mathbf{N}^n).
$$
从$x.0 = 0.x = x$到$x \in U$，
$$
c_{\alpha, 0, \gamma} = c_{0, \alpha, \gamma} = \delta_{\alpha \gamma}
$$
其中 $\delta_{\alpha \gamma}$ 是克罗内克指标。特别是，今后将 $k = 1, \ldots, n$ 写为 $k$ 而不是 $\varepsilon_k$，
$$
(x.y)_k = x_k + y_k + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c_{\alpha, \beta, k} x^{\alpha} y^{\beta}.
$$
写$c_{\alpha \beta} = (c_{\alpha \beta 1}, c_{\alpha \beta 2}, \ldots, c_{\alpha \beta n}) \in K^n$，则得出
$$
x.y = x + y + \sum_{|\alpha| \geq 1, |\beta| \geq 1} c_{\alpha \beta} x^{\alpha} y^{\beta}.
$$

在(5)的右侧，我们考虑次数2的齐次分量：

$$
B(x, y) = \sum_{i,j=1}^n c_{ij} x_i y_j
$$

因此$(x, y) \mapsto B(x, y)$是$K^n \times K^n$到$K^n$的双线性映射。然后

(6)
$$
x.y \equiv x + y + B(x, y) \mod \deg 3.
$$

公式 (4) 另一方面意味着

(7)
$$
c_{\alpha, \beta, \gamma} = 0 \quad \text{if } |\alpha| + |\beta| < |\gamma|
$$

and that the terms of total degree $|\gamma|$ in the expansion of $z^\gamma$ are also those of $(x_1 + y_1)^{\gamma_1}(x_2 + y_2)^{\gamma_2} \ldots (x_n + y_n)^{\gamma_n} = \sum_{\alpha + \beta = \gamma} ((\alpha, \beta)) x^\alpha y^\beta$ (cf. *Differentiable and Analytic Manifolds*, R, Notation and conventions). 因此：

(8)
$$
c_{\alpha, \beta, \gamma} = 0 \quad \text{if } |\alpha| + |\beta| = |\gamma| \quad \text{but } \alpha + \beta \neq \gamma
$$
(9)
$$
c_{\alpha, \beta, \alpha + \beta} = ((\alpha, \beta)).
$$

乘积的结合性意味着关系
$$
\sum_{\xi} c_{\alpha \xi n} x^\alpha \left( \sum_{\beta, \gamma} c_{\beta \gamma \xi} y^\beta z^\gamma \right) = \sum_{\xi, \gamma} c_{\xi \gamma n} \left( \sum_{\alpha, \beta} c_{\alpha \beta \xi} x^\alpha y^\beta \right) z^\gamma
$$
对于所有$x, y, z$足够接近0，从而

(10)
$$
\sum_{\xi} c_{\alpha \xi n} c_{\beta \gamma \xi} = \sum_{\xi} c_{\xi \gamma n} c_{\alpha \beta \xi} \quad (\alpha, \beta, \gamma, \eta \text{ in } \mathbf{N}^n).
$$

群胚芽G承认交换开子群胚芽当且仅当$c_{\alpha \beta \gamma} = c_{\beta \alpha \gamma}$对于$\mathbf{N}^n$中的所有$\alpha, \beta, \gamma$。

### 2. 李代数中的支架

对于$\alpha \in \mathbf{N}^n$，令$e_\alpha$为原点处的点分布$\frac{1}{\alpha!} \frac{\partial^\alpha}{\partial x^\alpha}$。特别是，
$$
e_k = e_{e_k} = \frac{\partial}{\partial x_k}.
$$
向量空间$U(G)$的$e_\alpha$形式基。如果 $f$ 是 G 中 0 的开邻域上的解析函数，并且 $f(x) = \sum \lambda_\alpha x^\alpha$ 是它的展开作为关于原点的积分级数，则
$$
\langle e_\alpha, f \rangle = \lambda_\alpha.
$$
特别是，
$$
\langle e_\alpha, x^\gamma \rangle = \delta_{\alpha \gamma}.
$$

因此
$$
\langle e_\alpha * e_\beta, x^\gamma \rangle = \langle e_\alpha \otimes e_\beta, (x.y)^\gamma \rangle \\
= \langle e_\alpha \otimes e_\beta, \sum_{\alpha', \beta'} c_{\alpha'\beta'\gamma} x^{\alpha'} y^{\beta'} \rangle \\
= \sum_{\alpha', \beta'} c_{\alpha'\beta'\gamma} \langle e_\alpha, x^{\alpha'} \rangle \langle e_\beta, y^{\beta'} \rangle = c_{\alpha\beta\gamma}
$$
因此
$$
e_\alpha * e_\beta = \sum_\gamma c_{\alpha\beta\gamma} e_\gamma.
$$
（公式 (10) 然后在 $U(G)$ 上表达结合性。）
特别是，因为$L(G)$在支架下是稳定的。
$$
[e_i, e_j] = \sum_k (c_{ijk} - c_{jik}) e_k.
$$
因此，$L(G)$相对于基$(e_1, \ldots, e_n)$的结构常数为$c_{ijk} - c_{jik}$。在其他字中，将$L(G)$与$K^n$规范地识别，我们得到：
$$
[x, y] = B(x, y) - B(y, x).
$$

#### 命题 1 {#lie-iii-s5-prop-1 .statement tag=0AE1}

（一）$$ x^{[-1]} \equiv -x + B(x, x) \mod \deg 3 $$
（二）$$ x.y.x^{[-1]} \equiv y + [x, y] \mod \deg 3 $$
（三）$$ y^{[-1]}.x.y \equiv x + [x, y] \mod \deg 3 $$
（四）$$ x^{[-1]}.y^{[-1]}.x.y \equiv [x, y] \mod \deg 3 $$
（五）$$ x.y.x^{[-1]}.y^{[-1]} \equiv [x, y] \mod \deg 3. $$
（在（i）中，$x^{[-1]}$当然代表函数$x \mapsto x^{[-1]}$的展开作为关于原点的级数积分；其他公式可以类似地解释。）
令 $g_1$ 和 $g_2$ 为次数 1 和 2 的 $x^{[-1]}$ 的齐次分量。那么
$$
0 = x.x^{[-1]} \\
\equiv x + g_1(x) + B(x, g_1(x)) \mod \deg 2 \quad \text{(by (6))} \\
\equiv x + g_1(x) \mod \deg 2
$$
因此$g_1(x) = -x$。然后
$$
0 = x.x^{[-1]} \\
\equiv x + (-x + g_2(x)) + B(x, -x + g_2(x)) \mod \deg 3 \\
\equiv g_2(x) - B(x, x) \mod \deg 3
$$

因此$g_2(x) = B(x, x)$。这就证明了(i)。然后，使用 (i)，
$$
x.y.x^{[-1]} \equiv (x + y + B(x, y)).(-x + B(x, x)) \quad \text{mod deg 3}
$$
$$
\equiv x + y + B(x, y) + (-x + B(x, x)) + B(x + y, -x) \quad \text{mod deg 3}
$$
$$
\equiv y + B(x, y) - B(y, x) \quad \text{mod deg 3}
$$
$$
\equiv y + [x, y] \quad \text{mod deg 3 (by (13))}
$$
从而（二）。 (iii) 的证明是类似的。结合 (i) 和 (iii)，我们得到
$$
x^{[-1]},y^{[-1]}.x.y \equiv (-x + B(x, x)).(x + [x, y]) \quad \text{mod deg 3}
$$
$$
\equiv -x + B(x, x) + x + [x, y] + B(-x, x) \quad \text{mod deg 3}
$$
$$
\equiv [x, y] \quad \text{mod deg 3}
$$
从而（四）。 (v)的证明是类似的。

### 3. 幂

考虑 G 的 j 点：
$$
x(1) = (x(1)_1, x(1)_2, \ldots, x(1)_n)
$$
$$
x(2) = (x(2)_1, x(2)_2, \ldots, x(2)_n)
$$
$$
\ldots \ldots \ldots \ldots \ldots \ldots \ldots
$$
$$
x(j) = (x(j)_1, x(j)_2, \ldots, x(j)_n).
$$
映射 $(x(1), x(2), \ldots, x(j)) \mapsto x(1).x(2)\ldots x(j)$ 承认展开作为关于原点的级数积分：

$$
x(1).x(2)\ldots x(j) = \sum_{\alpha(1), \alpha(2), \ldots, \alpha(j) \in \mathbf{N}^n} a_{\alpha(1), \ldots, \alpha(j)} x(1)^{\alpha(1)} \ldots x(j)^{\alpha(j)}
$$

其中$a_{\alpha(1), \ldots, \alpha(j)}$是$\mathbf{K}^n$的元素。我们写，对于 $j = 0, 1, 2, \ldots$，

$$
\psi_j(x) = \sum_{\alpha(1) \neq 0, \ldots, \alpha(j) \neq 0} a_{\alpha(1), \ldots, \alpha(j)} x^{\alpha(1) + \ldots + \alpha(j)}
$$

其中右侧是变量 $x \in \mathbf{K}^n$ 的收敛积分级数。这个级数是通过抑制（14）项（其中变量$x(1), \ldots, x(j)$之一未显式出现）然后写入$x(1) = x(2) = \cdots = x(j) = x$而获得的。

如果 $t \in \mathbf{K}$，G 的所有第 t 个幂映射都具有相同的展开作为关于原点的积分级数，因为它们中的任何两个重合在 0 的邻域上。我们将这个展开表示为积分级数 $x^{[t]}$。

#### 命题 2 {#lie-iii-s5-prop-2 .statement tag=0AE2}

（一）$\psi_j \equiv 0 \mod \deg j$。
(ii) *如果$t \in \mathbf{K}$，则*
$$
x^{[t]} = \sum_{i=1}^8 \binom{t}{i} \psi_i(x)
$$
*由于 (i)，右侧的正式幂级数才有意义。*

（我们写

$$
\binom{t}{i} = \frac{t(t-1)\ldots(t-i+1)}{i!}
$$

对于所有$t \in \mathbf{K}$。）

断言 (i) 从$\psi_j$的定义是明显的。

我们证明 (ii) $t$ 整数 $\geq 0$。由(14)，

$$
x^{[t]} = \sum_{\alpha(1), \ldots, \alpha(t) \in \mathbf{N}^n} a_{\alpha(1), \ldots, \alpha(t)} x^{\alpha(1) + \ldots + \alpha(t)}.
$$

对于$\alpha = (\alpha(1), \ldots, \alpha(t)) \in (\mathbf{N}^n)^t$，令$\sigma(\alpha)$表示$j \in \{1, 2, \ldots, t\}$的集合，使得$\alpha(j) \neq 0$。如果，在和 (17) 中，我们群一起项，其中 $\sigma(\alpha)$ 是相同的，那么

$$
x^{[t]} = \sum_{\sigma \subset \{1, t\}} h_{t, \sigma}(x)
$$

哪里

$$
h_{t, \sigma}(x) = \sum_{\sigma(\alpha) = \sigma} a_{\alpha(1), \ldots, \alpha(t)} x^{\alpha(1) + \ldots + \alpha(t)}.
$$

让 $\sigma = \{j_1, j_2, \ldots, j_q\}$ 与 $j_1 < j_2 < \ldots < j_q$。在(14)中（其中$j$被$t$代替），我们用0代替$x(k)$代替$k \notin \sigma$；因为 0 是 $G$ 的单位元素，所以我们得到 $x(j_1) \cdot x(j_2) \ldots x(j_q)$ 的展开作为关于原点的级数积分：

$$
x(j_1) \cdot x(j_2) \ldots x(j_q) = \sum_{\sigma(\alpha) \subset \sigma} a_{\alpha(1), \ldots, \alpha(t)} x(j_1)^{\alpha(j_1)} x(j_2)^{\alpha(j_2)} \ldots x(j_q)^{\alpha(j_q)}
$$

因此，通过 $\psi_q$ 的定义：

$$
\psi_q(x) = \sum_{\sigma(\alpha) = \sigma} a_{\alpha(1), \ldots, \alpha(t)} x^{\alpha(j_1) + \ldots + \alpha(j_q)}.
$$

由(19)和(20)，我们看到$h_{t, \sigma}(x) = \psi_{\mathrm{card}\,\sigma}(x)$。那么(18) 意味着

$$
x^{[t]} = \sum_{i=0}^t \binom{t}{i} \psi_i(x) = \sum_{i=0}^\infty \binom{t}{i} \psi_i(x).
$$

然后我们为所有$t \in \mathbf{K}$写出$x^{[t]'} = \sum_{i=0}^\infty \binom{t}{i} \psi_i(x)$。在积分级数$x^{[t]}$和$x^{[t]'}$中，每个系数是$t$的多项式函数。这对于$x^{[t]'}$来说是显而易见的。就$x^{[t]}$而言，只要证明对于所有$u \in \mathrm{U}(G)$，$u$在$x \mapsto x^{[t]}$下的像就是$t$的多项式函数。现在，对于$u \in \mathrm{U}^m(G)$，这个像是$t^m u$（§ 4, no. 3，命题7（iv））。

由于$x^{[t]} = x^{[t]'}$对应于$t$整数$\geq 0$，因此$x^{[t]} = x^{[t]'}$对应于所有$t \in \mathbf{K}$。

#### 注 {#lie-iii-s5-n3-rem-1 .statement tag=0AE3}

(1) 我们将 t 整数 $\geqslant 0$ 写为命题 2 的条件 (ii)：

$$
\begin{align*}
0 &= \psi_0(x) \\
x &= \psi_0(x) + \psi_1(x) \\
x^{[2]} &= \psi_0(x) + 2\psi_1(x) + \psi_2(x) \\
&\ldots \ldots \ldots \ldots \ldots \ldots \ldots
\end{align*}
$$

这些公式足够确定 $\psi_i$。

(2) 我们看到$\psi_0(x) = 0, \psi_1(x) = x, \psi_2(x) = x^{[2]} - 2x$，

$$
x^{[-1]} = \sum_{i=1}^\infty (-1)^i \psi_i(x).
$$

(3) 上述$\psi_2$和公式的表达式 (6) 证明

$$
\psi_2(x) \equiv \mathrm{B}(x, x) \mod \deg 3.
$$
使用命题 2，(i) 和 (ii)，我们看到

$$
x^{[t]} \equiv tx + \binom{t}{2} \mathrm{B}(x, x) \mod \deg 3.
$$

(4) 令$\psi_{p,m}(x)$和$h_{t,m}(x)$表示次数m的$\psi_p(x)$和$x^{[t]}$的齐次分量。然后$\psi_{p,m} = 0$换$m < p$。另一方面，命题 2 (ii) 给出

$$
h_{t,m}(x) = \sum_{p \leq m} \frac{t(t-1)\ldots(t-p+1)}{p!} \psi_{p,m}(x)
$$
那就是

$$
h_{t,m}(x) = \sum_{1 \leq r \leq m} t^r \phi_{r,m}(x)
$$
其中$\phi_{r,m}$是齐次多项式映射，次数米，$\mathbf{K}^n$到$\mathbf{K}^n$。特别地，通过(23)，

$$
\phi_{1,m}(x) = \sum_{p \leq m} \frac{(-1)^{p-1}}{p} \psi_{p,m}(x)
$$
$$
\phi_{m,m}(x) = \frac{1}{m!} \psi_{m,m}(x).
$$

(5) If $\mathbf{K}$ is of characteristic $> 0$, the results of nos. 1 and 2 remain true, provided $e_\alpha$, in no. 2, is defined by $\langle e_\alpha, \sum_\beta \lambda_\beta x^\beta \rangle = \lambda_\alpha$. 在no. 3中，如果$\psi_j$如上定义，则论证再次证明$x^{[t]} = \sum_{i=1}^\infty \binom{t}{i} \psi_i(x)$ if $t \in \mathbf{N}$。

### 4. 指数

令 $E(x)$ 为 $G$ 的指数映射作为关于 0 的积分级数的展开。 令 $L(x)$ 为 $G$ 的单射指数映射的倒数映射作为关于 0 的积分级数的展开。 由于 0 处与任意指数映射的切线映射是 $L(G)$、$E(x) \equiv x \mod \deg 2$ 和 $L(x) \equiv x \mod \deg 2$ 的恒等式。 由于$x$的$E(L(x)) = L(E(x))$足够接近0，因此正式的幂级数$E$和$L$使得$E(L(X)) = L(E(X)) = X$。 类似的论证表明
$$
E(tX) = (E(X))^{[t]}, \quad L(X^{[t]}) = tL(X)
$$
对于$t \in K$。

#### 命题 3 {#lie-iii-s5-prop-3 .statement tag=0AE4}

(27)
$$
L = \sum_{p=1}^{\infty} \frac{(-1)^{p-1}}{p} \psi_p
$$
(28)
$$
E = \sum_{p=1}^{\infty} \frac{1}{p!} \psi_{p,p}
$$
（回想一下，$\psi_{p,p}$是次数$p$的$\psi_p$的齐次分量。）

或者，通过 (24)，
$$
E(tx) = (E(x))^{[t]}
$$

两侧分别为$t$和$x$正式幂级数。将第一个次数的项等同于$t$，我们得到
$$
x = \sum_{m \geq 0} \phi_{1,m}(E(x)).
$$
现在，当可能时，形式幂级数系统的反转只能以一种方式实现（代数、章 IV, § 6，命题 8 的推论）。然后
$$
L(x) = \sum_{m \geq 0} \phi_{1,m}(x) \quad \text{by (29)}
$$
$$
= \sum_{p,m} \frac{(-1)^p}{p} \psi_{p,m}(x) \quad \text{by (25)}
$$
$$
= \sum_p \frac{(-1)^p}{p} \psi_p(x),
$$
从而（一）。同样，对于$t \neq 0$，
$$
L(tx) = tL((tx)^{[t^{-1}]})
$$
$$
= tL\left( \sum_{m \geq 0} \sum_{1 \leq r \leq m} t^{m-r} \phi_{r,m}(x) \right) \quad \text{by (24)}.
$$

将 t 中第一个次数的项等式，我们得到

$$
x = L \left( \sum_{m \geq 0} \phi_{m,m}(x) \right)
$$

whence

$$
E(x) = \sum_{m \geq 0} \phi_{m,m}(x)
$$
$$
= \sum_{m \geq 0} \frac{1}{m!} \psi_{m,m}(x) \quad \text{by (26).}
$$

#### 命题 4 {#lie-iii-s5-prop-4 .statement tag=0AE5}

*对于 G 的图表曾经是规范的，$\psi_j = 0$ 对于 $j \geq 2$ 是充分必要的。*

命题 3 就足够了。假设图表是规范的，并且 $\psi_i = 0$ 适合 $2 \leq i < n$。然后$nx = x^{[n]} = \sum_{i=0}^n \binom{n}{i} \psi_i(x) = nx + \psi_n(x)$，从而$\psi_n = 0$。因此，$j$ 上的归纳为$j \geq 2$ $\psi_j = 0$。

### 习题 {#lie-iii-s5-exercises}

参见[习题为 § 5](exercises/s5/)。
