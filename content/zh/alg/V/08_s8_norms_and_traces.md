---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 8
section_title: Norms and traces
lang: zh
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.47-A V.51, A V.153
pdf_pages: 0161-0165, 0267-0267
extraction: ocr
subsections:
    - "no": 1
      title: Recall
      page: 47
      pdf_page: 161
    - "no": 2
      title: Norms and traces in etale algebras
      page: 47
      pdf_page: 161
    - "no": 3
      title: Norms and traces in extensions of finite degree
      page: 50
      pdf_page: 164
statements: 9
exercises: 2
content_sha256: e986f7e60fe2a604b4e3072d5f40307c7b81ec0c757fc522f19819dcc35ab5de
translated_from: content/en/alg/V/08_s8_norms_and_traces.md
translation_method: google
source_content_sha256: c2e7557b98c678b7ab7b76840a046be64717fd2ef2e68d0dbcc702987b154e2d
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 644f9c9f22fd0d68700b44659b1aee1b1857cc22e0996dea53f7d6fbd6348cd0
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 8。 范数和痕迹

在本段中，K 表示域。

### 1.回忆

令 A 为 K 上的有限次数 $n$ 的代数。对于每个 $x \in A$，我们用 A 的 $L_x$ 线性映射 $a \mapsto xa$ 表示其自身。我们回想一下（III，p. 543），$L_x$的迹称为x相对于A的迹，记为$\mathrm{Tr}_{A/K}(x)$；同样，$L_x$的行列式称为x相对于A的范数，并用$N_{A/K}(x)$表示。 A 的 n 元素的序列 $(x_1, ..., x_n)$ 的判别式是由定义矩阵 $(\mathrm{Tr}_{A/K}(x_i x_j))_{1 \leq i,j \leq n}$ 的行列式$D_{A/K}(x_1, ..., x_n)$ (III，p. 549)。

令 K' 为 K 的扩张，并令 $A' = A_{(K')}$ 为通过标量的扩张从 A 导出的 K' 代数。我们有公式

(1) $$
\mathrm{Tr}_{A'/K'}(1 \otimes x) = \mathrm{Tr}_{A/K}(x) . 1 , \quad N_{A'/K'}(1 \otimes x) = N_{A/K}(x) . 1
$$
对于所有$x \in A$（III，p. 544）。对于 A 的每个序列 $(x_1, ..., x_n)$ 元素我们有

(2) $$
D_{A'/K'}(1 \otimes x_1, ..., 1 \otimes x_n) = D_{A/K}(x_1, ..., x_n) . 1 ,
$$
从第一个公式(1)开始如下。

### 2. 范数和 etale 代数中的痕迹

设 A 是 K 上（有限）次数 $n$ 的 etale 代数。到定义时，存在 K 的扩张 L 以及 A 的不同同态 $u_1, ..., u_n$ 到 L 中，具有以下属性。

a) $A$到$L$的每个同态等于$u_i$之一（V，p. 29，Cor.）；
b) 存在 $L$-代数同构 $u : A_{(L)} \to L^n$ 使得

$$
u(1 \otimes x) = (u_1(x), \ldots, u_n(x)) \quad \text{for all } x \in A .
$$

此外，$K$的每个代数闭扩张$L$都具有上述性质（V，p. 30，命题2）。

我们在下面修复$L, u_1, \ldots, u_n$。设 $x \in A$；我们将证明公式

$$
\text{Tr}_{A/K}(x) \cdot 1 = \sum_{i=1}^n u_i(x) , \quad \text{N}_{A/K}(x) \cdot 1 = \prod_{i=1}^n u_i(x) .
$$

Let $v$ be multiplication by $l \otimes x$ in $A_{(L)}$; with respect to the basis of $A_{(L)}$ which is the image under $u^{-1}$ of the canonical basis of $L^n$, the matrix of the linear mapping $v$ is diagonal, with diagonal elements $u_1(x), \ldots, u_n(x)$. 我们结论那个

$$
Tr_{A_{(L)}/L}(1 \circ x) \cdot 1 = \sum_{r=1}^n u_i(x) , \quad \text{whence} \quad \text{Tr}_{A/K}(x) \cdot 1 = \sum_{i=1}^n u_i(x) \text{ by (1)} ;
$$

范数的情况也类似处理。

进一步令$(x_1, \ldots, x_n)$为$A$元素序列，令U为矩阵

$$
(u_i(x_j))_{1 \leq i,j \leq n}
$$

令$(t_{ij}) = 'U . U$。通过第一个公式 (3) 我们有

$$
\text{Tr}_{A/K}(x_i x_j) \cdot 1 = \sum_{k=1}^n u_k(x_i x_j) = \sum_{k=1}^n u_k(x_i) u_k(x_j) = t_{ij} ;
$$

经过到行列式，我们得到

$$
D_{A/K}(x_1, \ldots, x_r) \cdot 1 = [\det u_i(x_j)]^2 .
$$

#### 命题 1 {#alg-v-s8-prop-1 .statement tag=06L9}

— *令 $A$ 为有限次数中的交换代数除以 $K$。那么下面的条件是等价的*：
a) *代数 $A$ 是 etale。*
b) *$A$存在判别式非零的基。*
c) *对于$A$中的每个$x \neq 0$，$A$中都存在$y$，使得$\text{Tr}_{A/K}(xy) \neq 0$。*
*此外，当满足这些条件时，$A$的任何基的判别式都是非零的。*

我们将证明当$A$假设为etale时，$A$相对于$A$的任何基$(x_1, \ldots, x_n)$在$K$上的判别式不为零；这将特别建立蕴涵$a) \Rightarrow b)$。由(4)式，结合上述记号，足以证明矩阵 U是可逆的，或者等价地，线性方程组的系统

$$
\sum_{i=1}^n \lambda_i u_i(x_j) = 0 \quad (\text{for } 1 \leq j \leq n)
$$

L 中只有解 $\lambda_1 = \cdots = A, = 0$。现在，关系 (5) 意味着$\sum_{i=1}^n \lambda_i u_i(x) = 0$对于所有$x \in A$，从而$\lambda_i = 0$对于$1 \leq i \leq n$，通过定理关于同态（V，p. 27，Th.1）的线性独立性。

b)和c)的等价是以下一般引理的推论：

#### 引理 1 {#alg-v-s8-lem-1 .statement tag=06LA}

令 V 为 K 和 B 上有限维的向量空间，在 * V x V 上为双线性 *形式。设$(v_1, \ldots, v_n)$*是*V*的基*超过*K*和*$\Delta = \det B(v_i, v_j)$。那么$A \neq 0$当且仅*如果*，对于V中的每个$x \neq 0$，V中存在y使得$B(x, y) \neq 0$。

我们有 $A \neq 0$ 当且仅当系统线性方程

$$
\sum_{i=1}^n \lambda_i B(v_i, v_j) = 0 \quad (1 \leq j \leq n)
$$

K 中只有解 $A, = \cdots = A, = 0$。如果我们放入 $x = \sum_{i=1}^n \lambda_i v_i$，则上面的系统等价于 $1 \leq j \leq n$ 的 $B(x, v_j) = 0$，或者，由于 $(v_1, \ldots, v_n)$ 是 V 的基在 K 上，对于所有的$B(x, y) = 0$ $y \in V$、从而引理。

让我们证明条件 c) 意味着 A 被约简。设 x 为 A 的幂零元 ：对于任何 $y \in A$ 元素 xy 都是幂零的，因此向量空间 A 的自同态 $L_{xy}$ 也是幂零的。现在下面的引理意味着$\mathrm{Tr}(xy) = 0$对于所有$y \in A$，从而$x = 0$在假设c)下。

#### 引理 2 {#alg-v-s8-lem-2 .statement tag=06LB}

令V为K上有限维的向量空间和V的$u$幂零自同态，则为$\mathrm{Tr}(u) = 0$。

对于每个整数 $n \geq 0$，令 $V_n$ 为 $u^n$ 的像。由于$u$是幂零的，因此存在整数$r \geq 0$使得$V_0 = V, V_r = 0$和$V_i \neq V_{i+1}$对于$0 \leq i < r - 1$。令 $d_i$ 为 $V_{i-1}$ 的维数（对于 $1 \leq i \leq r$）。存在V的基$(x_1, \ldots, x_d)$使得向量$x_j$与$d - d_i < j \leq d$形式基$V_{i-1}$（对于$1 \leq i \leq r$）。我们有$u(V_{i-1}) \subset V_i$，因此基$(x_1, \ldots, x_d)$的矩阵和$u$的对角线元素是零。因此我们有 $\mathrm{Tr}(u) = 0$ 和引理。

最后让我们证明 b) 蕴涵 a)。令$(x_1, \ldots, x_n)$为A除以K的基，使得$D_{A/K}(x_1, \ldots, x_n) \neq 0$。令 K' 为 K 的扩张，A' 为由 A 的标量扩张和 $1 \leq i \leq n$ 的 $x'_i = 1 \otimes x_i$ 导出的 K' 代数。到公式 (2) (V, p. 47) 我们有$D_{A'/K'}(x'_1, \ldots, x'_n) \neq 0$。 应用 A' 的前面结果我们看到 A' 被约简，因此代数 A 是 etale (V, p. 34, Th. 4)。

#### 推论{#alg-v-s8-n2-cor-1 .statement tag=06LC}

— 令 E 为 K 的扩张 *有限* 次数。为了使 E 可分离，E 中存在 a 使得 $\mathrm{Tr}_{E/K}(a) \neq 0$ 是必要且充分的。

根据命题1，条件是必要的。相反，假设存在$a \in E$使得$\mathrm{Tr}_{E/K}(a) \neq 0$。给定E中的$x \neq 0$，如果我们放入$y = a x'$，则$\mathrm{Tr}_{E/K}(xy) \neq 0$。现在，命题 1 表明 E 是 K 上的 etale 代数，因此是 K 的可分扩张。

### 3. 范数以及扩张有限次数中的痕迹

代数（III，p. 548）中的传递性公式在扩张或有限次数的情况下意味着以下命题。

#### 命题 2 {#alg-v-s8-prop-2 .statement tag=06LD}

— 令 F 为 K 的有限次数的扩张，E 为 F 的子扩展。那么对于每个 $x \in F$，我们有
$$
\text{Tr}_{F/K}(x) = \text{Tr}_{E/K}(\text{Tr}_{F/E}(x)) \\
\text{N}_{F/K}(x) = \text{N}_{E/K}(\text{N}_{F/E}(x)) .
$$

#### 推论{#alg-v-s8-n3-cor-1 .statement tag=06LE}

— 将$m = [F : E]$；那么对于每个 $x \in E$ 我们有
$$
\text{Tr}_{F/K}(x) = m \cdot \text{Tr}_{E/K}(x) \\
\text{N}_{F/K}(x) = \text{N}_{E/K}(x)^m .
$$

#### 命题 3 {#alg-v-s8-prop-3 .statement tag=06LF}

— 令 E 为 K 的有限次数 n 的扩张，以及 E 的 x 元素，K 上的次数 d。将 $f(X) = X^d + \sum_{i=1}^d a_i X^{d-i}$ 写为 K 上的 X 的最小多项式。然后我们有
$$
\text{Tr}_{E/K}(x) = - \frac{n}{d} a_1 \\
\text{N}_{E/K}(x) = (((-1)^d a_d)^{n/d} = (-1)^n a_d^{n/d} .
$$

提案 3 直接源自 Cor。提案 2 和引理：

#### 引理 3 {#alg-v-s8-lem-3 .statement tag=06LG}

设 R 为交换环、$f(X) = X^d + \sum_{i=1}^d a_i X^{d-i}$ $\mathbf{R}[X]$、A R-代数 $\mathbf{R}[X]/(f)$ 和 A 中 X 的 x 剩余类类。然后是 $\text{Tr}_{A/R}(x) = -a_1$ 和 $\text{N}_{A/R}(x) = (-1)^d a_d$。

由科。 (IV, p. 11) 序列 $(1, x, ..., x^{d-1})$ 是 A 的基 ；进一步我们有
$$
x \cdot 1 = x , \quad x \cdot x = x^2 , \ldots , x \cdot x^{d-2} = x^{d-1} ,
$$
$$
x \cdot x^{d-1} = -a_d \cdot 1 - a_{d-1} \cdot x - \ldots - a_1 \cdot x^{d-1}
$$

矩阵用x相对于$A$的基$(1, x, ..., x^{d-1})$表达乘法，因此是以下形式（我们采用$d = 5$来修正想法）：

$$
\begin{pmatrix}
0 & 0 & 0 & 0 & -a \\
1 & 0 & 0 & 0 & -a \\
0 & 1 & 0 & 0 & -a_3 \\
0 & 0 & 1 & 0 & -a_2 \\
0 & 0 & 0 & 1 & -a_1
\end{pmatrix}
$$

这个矩阵的痕迹明显是$-a$；行列式可以通过第一行展开来计算，然后我们发现

$$
(-1)^{d-1} (-a_d) = (-1)^d a_d .
$$

对于这个编号的其余部分，我们用 K 的有限次数的 E 扩张和 E 的 $x$ 元素表示。我们将指出在各种情况下如何计算范数和$x$ 的踪迹。

a) *可分扩张*的情况：假设E在K上与次数$n$可分，用K的$\Omega$代数闭包和$\sigma_1, \ldots, \sigma_n$表示E与R的$n$不同的$K$同态。 公式 (3) ($V$, p. 48) 我们在 R 中有

$$
\text{Tr}_{E/K}(x) = \sum_{i=1}^n \sigma_i(x) , \quad N_{E/K}(x) = \prod_{i=1}^n \sigma_i(x) .
$$

b) *p 根式扩展的情况*：假设 K 具有特征 $p > 0$ 并且扩张 E 是 p 根式；存在整数$e \geq 0$使得$[E:K] = p^e$（$V$，p. 26，命题4）。如果$f$是$x$在K上的高度，则$x$在K上的最小多项式是$X^{p^f} - x^{p^f}$（$V$，p. 24，命题1）。根据第 3 条命题，我们有 $N_{E/K}(x) = (x^{p^f})^{p^e/p^f}$，从而

$$
N_{E/K}(x) = x^{p^e} = x^{[E:K]}
$$

对于迹，我们找到$\text{Tr}_{E/K}(x) = -p^{e-f} a$，其中$a$是多项式$X^{p^f} - x^{p^f}$中$X^{p^f-1}$的系数；在其他字中，我们有

$$
\text{Tr}_{E/K}(x) = p^e \cdot x = [E:K] x = \begin{cases} x & \text{if } [E:K] = 1 \\ 0 & \text{if } [E:K] > 1 . \end{cases}
$$

c) *一般情况*：我们可以总结范数的计算和跟踪如下命题：

#### 命题 4 {#alg-v-s8-prop-4 .statement tag=06LH}

*令 p 为 K 的有限次数的 K 和 E 扩张的特征指数。令 $\sigma_1, \ldots, \sigma_n$ 为 E 与 K 的代数闭包 $\Omega$ 的不同 K 同态，并令 $p^e = [E:K]_i$。对于每个 $x \in E$，我们都有 $\Omega$*

$$
\text{Tr}_{E/K}(x) = p^e \cdot \sum_{i=1}^n \sigma_i(x) , \quad N_{E/K}(x) = \left( \prod_{i=1}^n \sigma_i(x) \right)^{p^e} .
$$

令E为E中K的相对可分闭包；则$E_s$是K的次数$n$的可分扩张和E的$\sigma_1, \ldots, \sigma_n$诱导不同的K同态，转化为R；此外，E 是 E 的近似根式扩展，p$^e$ 度（$V$、p. 44、第 13 条命题和p. 46）。因此，第 4 条命题由公式 (6)、(7)、(13)、(14) 和 (12) 得出。

### 习题{#alg-v-s8-exercises}

§ 8](exercises/s8/)参见[习题。
