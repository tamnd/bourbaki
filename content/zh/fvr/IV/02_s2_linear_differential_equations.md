---
book: fvr
book_title: Functions of a Real Variable
chapter: IV
chapter_title: DIFFERENTIAL EQUATIONS
section: 2
section_title: LINEAR DIFFERENTIAL EQUATIONS
lang: zh
source: fvr-i-vii
book_pages: 177-198, 204-206
pdf_pages: 0192-0213, 0219-0221
extraction: ocr
subsections:
    - "no": 1
      title: EXISTENCE OF INTEGRALS OF A LINEAR DIFFERENTIAL EQUATION
      page: 177
      pdf_page: 192
    - "no": 2
      title: LINEARITY OF THE INTEGRALS OF A LINEAR DIFFERENTIAL EQUATION
      page: 179
      pdf_page: 194
    - "no": 3
      title: INTEGRATING THE INHOMOGENEOUS LINEAR EQUATION
      page: 182
      pdf_page: 197
    - "no": 4
      title: FUNDAMENTAL SYSTEMS OF INTEGRALS OF A LINEAR SYSTEM OF SCALAR DIFFERENTIAL EQUATIONS
      page: 183
      pdf_page: 198
    - "no": 5
      title: ADJOINT EQUATION
      page: 186
      pdf_page: 201
    - "no": 6
      title: LINEAR DIFFERENTIAL EQUATIONS WITH CONSTANT COEFFICIENTS
      page: 188
      pdf_page: 203
    - "no": 7
      title: LINEAR EQUATIONS OF ORDER $n$
      page: 192
      pdf_page: 207
    - "no": 8
      title: LINEAR EQUATIONS OF ORDER $n$ WITH CONSTANT COEFFICIENTS
      page: 194
      pdf_page: 209
    - "no": 9
      title: SYSTEMS OF LINEAR EQUATIONS WITH CONSTANT COEFFICIENTS
      page: 196
      pdf_page: 211
statements: 25
exercises: 10
content_sha256: f9a3c5fb8657ed7274648841febd41875d7f0403818bb15517d8c547590d1a66
translated_from: content/en/fvr/IV/02_s2_linear_differential_equations.md
translation_method: google
source_content_sha256: bb9011131c235f557b70d1568fb503a2bded76eb3a6bc7fabc1b5db368218573
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 77ad2efa31902a22dc01e377338aa2c32aab22eee7b7da545dfa71d8f91e2371
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 2。线性微分方程

### 1. 线性微分方程积分的存在性

令 E 为域 $\mathbf{R}$ 上的完全范数空间，J 为 $\mathbf{R}$ 中的区间，不减少至点。有人说微分方程

$$
\frac{d\mathbf{x}}{dt} = \mathbf{f}(t, \mathbf{x})
$$

(1) 其中 $f$ 在 $J \times E$ 上定义，是一个*线性*方程，如果对于每个 $t \in J$，映射 $x \mapsto f(t, x)$ 是一个从 $E$ 到自身的*连续仿射线性映射* [^1]；如果将 $b(t) = f(t, 0)$ 映射 $x \mapsto f(t, x) - f(t, 0) = f(t, x) - b(t)$ 则为从 $E$ 到自身的连续线性映射；从现在开始，我们将用$A(t)$来表示这个映射，并在点$x \in E$处将其值写为$A(t).x$（或简称为$A(t)x$）；因此线性微分方程（1）可以写成

$$
\frac{dx}{dt} = A(t).x + b(t)
$$

(2)

其中$b$是从$J$到$E$的映射；当$b = 0$时，我们说线性微分方程（2）是*齐次*的。

#### 例 1 {#fvr-iv-s2-n1-exa-1 .statement tag=08CO}

当$E$是有限维$n$超过$\mathbf{R}$一个可以确定自同态$A(t)$及其*矩阵*$\left(a_{ij}(t)\right)$*相对于*$E$的任何基时（*代数*，II，p. 343）；当相对于 $E$ 的基识别向量 $x \in E$ 及其组件的列矩阵 $(x_j)$ 时，表达式 $A(t).x$ 符合代数 (*Alg.*, II，p. 343，道具 2)。在这种情况下，方程（2）相当于标量微分方程的系统

$$
\frac{dx_i}{dt} = \sum_{j=1}^n a_{ij}(t)x_j + b_i(t) \qquad (1 \leq i \leq n).
$$

(3)

#### 例 2 {#fvr-iv-s2-n1-exa-2 .statement tag=08CP}

令$G$是$\mathbf{R}$上的*完全归一化的代数*，并且$a(t)$、$b(t)$和$c(t)$是从$J$到$G$的三个映射；等式

$$
\frac{dx}{dt} = a(t)x + x b(t) + c(t)
$$

是一个线性微分方程；这里$A(t)$是$G$自身的线性映射$x \mapsto a(t)x + x b(t)$。

对于每个$t \in J$，$A(t)$是从$E$到自身的连续线性映射的集合$\mathscr{L}(E)$的元素（$E$的连续自同态）；人们知道（*Gen.Top.*，X，p. 298）$\mathscr{L}(E)$，赋予了*范数*$\|U\| = \sup_{\|x\| \leq 1} \|Ux\|$，是一个*完全规范的代数*超过域$\mathbf{R}$，以及$\|UV\| \leq \|U\|\ \|V\|$。

*在整个截面中，我们假设满足以下条件：*

a) *映射* $t \mapsto A(t)$ *的* $J$ *进入* $\mathscr{L}(E)$ *受到监管*。

b) *映射* $t \mapsto b(t)$ *的* $J$ *进入* $E$ *受到管制*。

当$E$有维数$n$时，$\mathscr{L}(E)$与$\mathbf{R}^{n^2}$同构的（作为拓扑向量空间）和条件*a*）意味着矩阵的每个元素$a_{ij}(t)$ $A(t)$ 是$J$ 上的*受监管* 函数。

从$\|A(t')\mathbf{x} - A(t)\mathbf{x}\| \leq \|A(t') - A(t)\|\|\mathbf{x}\|$开始，映射
$$
t \mapsto A(t).\mathbf{x} + \mathbf{b}(t)
$$
每$\mathbf{x} \in E$受监管；进一步，
$$
\|A(t)\mathbf{x}_1 - A(t)\mathbf{x}_2\| = \|A(t)(\mathbf{x}_1 - \mathbf{x}_2)\| \leq \|A(t)\|\|\mathbf{x}_1 - \mathbf{x}_2\|
$$
对于$E$中的任何$t \in J$和$\mathbf{x}_1, \mathbf{x}_2$；在其他字中，(2)的右边满足IV、p. 165中的引理1的条件，并且相对于$J \times E$上规定的函数$\|A(t)\|$是Lipschitz。在推论（IV，p. 173，cor.2）：

#### 定理 1 {#fvr-iv-s2-thm-1 .statement tag=08CQ}

*设*$t \mapsto A(t)$*是*$J$*到*$\mathscr{L}(E)$的调节映射，*和*$t \mapsto \mathbf{b}(t)$*是*$J$*到*$E$的调节映射。 *对于* $J \times E$ *线性方程*的每一个点* $(t_0, \mathbf{x}_0)$ * (2) *承认在所有* $J$ *上定义了一个且唯一的一个解，并且等于* $\mathbf{x}_0$ *在点* $t_0$。

### 2. 线性微分方程积分的线性度

求解线性微分方程(2)是线性问题(*Alg.*,II,p. 240)；齐次线性方程
$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x}
$$
据说与非齐次方程 (2) *相关联；并且知道 (*Alg.*, II, p. 241, 命题 14)，如果 $\mathbf{u}_1$ 是非齐次方程 (2) 的积分，则该方程的每个积分都是形式 $\mathbf{u} + \mathbf{u}_1$，其中 $\mathbf{u}_1$ 是相关齐次方程 (4) 的解，并且反之。我们首先要研究这个小节*齐次*方程（4）的积分。

#### 命题 1 {#fvr-iv-s2-prop-1 .statement tag=08CR}

*集合* $\mathscr{I}$ *齐次线性方程的积分* (4)，*定义于* $J$，*是空间* $C(J; E)$ 的向量子空间 *连续映射从* $J$ *到* $E$。

证明是直接的。

#### 定理 2 {#fvr-iv-s2-thm-2 .statement tag=08CS}

*对于* $J \times E$ *的每个点* $(t_0, \mathbf{x}_0)$ *让* $\mathbf{u}(t, t_0, \mathbf{x}_0)$ *成为齐次方程的积分* (4) *定义于* $J$ *并等于* $\mathbf{x}_0$ *在* $t_0$。
1. *对于每个点* $t \in J$ *映射* $\mathbf{x}_0 \mapsto \mathbf{u}(t, t_0, \mathbf{x}_0)$ *是一个双射双连续线性映射* $C(t, t_0)$ *of* $E$ *自身*。
2. *映射* $t \mapsto C(t, t_0)$ *of* $J$ *化为* $\mathscr{L}(E)$ *与齐次线性微分方程的积分相同*
$$
\frac{dU}{dt} = A(t)\ U
$$
*需要值* $I$ **（* $E$ *自身的身份映射）* *在点* $t_0$。
3. *对于任何点* $s, t, u$ ** $J$
$$
C(s, u) = C(s, t)C(t, u), \qquad C(s, t) = (C(t, s))^{-1}.
$$

通过道具。 1, $\mathbf{u}(t, t_0, \mathbf{x}_1) + \mathbf{u}(t, t_0, \mathbf{x}_2)$（或$\lambda \mathbf{u}(t, t_0, \mathbf{x}_0)$）是（4）的积分，并且在$t_0$处取值$\mathbf{x}_1 + \mathbf{x}_2$（或$\lambda \mathbf{x}_0$），因此，通过th。 IV、p. 179 中的 1 个与 $\mathbf{u}(t, t_0, \mathbf{x}_1 + \mathbf{x}_2)$（分别为 $\mathbf{u}(t, t_0, \lambda \mathbf{x}_0)$）相同；因此，映射$\mathbf{x}_0 \mapsto \mathbf{u}(t, t_0, \mathbf{x}_0)$是E自身的线性映射$C(t, t_0)$，并且可以写成$\mathbf{u}(t, t_0, \mathbf{x}_0) = C(t, t_0). \mathbf{x}_0$。

由于 $\mathscr{L}(E) \times \mathscr{L}(E)$ 到 $\mathscr{L}(E)$ 的映射 $(X, Y) \mapsto XY$ 是连续的（*Gen. Top.*, X, p. 298，第 8 条），因此 J 到 $\mathscr{L}(E)$ 的映射 $t \mapsto A(t)U$ 受到所有监管$U \in \mathscr{L}(E)$；进一步（*Gen.Top.*，X，p. 296）

$$
\| A(t)X - A(t)Y \| = \| A(t)(X - Y) \| \leq \| A(t) \| \| X - Y \|,
$$

所以人们可以应用th。将IV、p. 179的I代入齐次线性方程(5)；令 $V(t)$ 为在 J 上定义的该方程的积分，并等于 $t_0$ 处的$I$。其中一个有 (I, p. 6, 道具 3)

$$
\frac{d}{dt} (V(t)\mathbf{x}_0) = \frac{dV(t)}{dt} \mathbf{x}_0 = A(t)(V(t)\mathbf{x}_0)
$$

对于$t = t_0$，我们有$V(t)\mathbf{x}_0 = I\mathbf{x}_0 = \mathbf{x}_0$；到了。 IV、p. 179 中的 1 个对于所有 $\mathbf{x}_0 \in E$ 必须有 $V(t).\mathbf{x}_0 = C(t, t_0)\mathbf{x}_0$，即 $V(t) = C(t, t_0)$；这就证明了$C(t, t_0)$属于到$\mathscr{L}(E)$，在其他字中，$\mathbf{x}_0 \mapsto C(t, t_0).\mathbf{x}_0$在E上连续，并且映射$t \mapsto C(t, t_0)$是(5)的积分，在$t_0$处等于$I$。

最后，(4) 的积分$s \mapsto C(s, u).\mathbf{x}_0$在点$t$处等于$C(t, u).\mathbf{x}_0$，因此，通过定义，

$$
C(s, u).\mathbf{x}_0 = C(s, t)(C(t, u).\mathbf{x}_0) = (C(s, t)C(t, u)).\mathbf{x}_0
$$

对于任意 $\mathbf{x}_0 \in E$，从而第一个关系 (6)；因为$C(s, s) = I$有$C(s, t)C(t, s) = I$，对于J中的任何$s$和$t$；这证明了（*集合理论*，II，p. 86，推论）$C(t, t_0)$是E到自身的双射映射，具有逆映射$C(t_0, t)$。这样就完成了定理的证明。

有人说$C(t, t_0)$是IV、p. 178的方程(2)的*解*。

#### 推论 1 {#fvr-iv-s2-thm-2-cor-1 .statement tag=08CT}

*映射，对于每个点 $\mathbf{x}_0 \in E$，将 J 上定义的连续函数 $t \mapsto C(t, t_0).\mathbf{x}_0$ 关联起来，是范数空间 E 的同构到 (4) 积分的向量空间 $\mathscr{I}$，赋予拓扑紧凑收敛。*

它肯定是E到$\mathscr{I}$的双射线性映射：现在$C(t, t_0)$有界于紧集$K \subset J$，因此$\| C(t, t_0).\mathbf{x}_0 \| \leq M \| \mathbf{x}_0 \|$对于任何$t \in K$和$\mathbf{x}_0 \in E$，这表明这个映射是连续的；自从

$$
C(t_0, t_0).\mathbf{x}_0 = \mathbf{x}_0,
$$

显然，逆矩阵映射也是连续的。

#### 推论 2 {#fvr-iv-s2-thm-2-cor-2 .statement tag=08CU}

*$J \times J$到$\mathscr{L}(E)$的映射$(s, t) \mapsto C(s, t)$是连续的。*

由(6)我们有$C(s, t) = C(s, t_0) \left( C(t, t_0) \right)^{-1}$；现在，$\mathscr{L}(E) \times \mathscr{L}(E)$的映射$(X, Y) \mapsto XY$到$\mathscr{L}(E)$是连续的，$\mathscr{L}(E)$的可逆元的（开放）群到其自身上的映射$X \mapsto X^{-1}$也是连续的（TG，IX，p. 40，道具 14）。

一个可能注那个映射
$$
t \mapsto C(t_0, t) = (C(t, t_0))^{-1}
$$
承认导数等于$-(C(t, t_0))^{-1} (dC(t, t_0)/dt)(C(t, t_0))^{-1}$（在可数集合的补集上）（I，p. 8，命题4），也就是说（由IV，p. 179，公式（5））等于$-C(t_0, t) A(t)$。

#### 推论 3 {#fvr-iv-s2-thm-2-cor-3 .statement tag=08CV}

*设K为J中包含的紧区间，并设$k = \sup_{t \in K} \|A(t)\|$。对于 K* 中的所有 t 和 $t_0$
$$
\|C(t, t_0) - I\| \leq e^{k|t-t_0|} - 1 .
$$ (7)

事实上，$\|A(t)x_0\| \leq k \|x_0\|$对于所有$t \in K$；在 K 上，常数函数等于 $x_0$，因此是通过等式（4）右 IV、p. 18 在 $k \|x_0\|$ 内的近似积分；通过 IV、p. 170 的公式 (15)，因此有
$$
\|C(t, t_0)x_0 - x_0\| \leq \|x_0\| (e^{k|t-t_0|} - 1)
$$
对于 K 中的任意 $t$ 和 $t_0$，以及 E 中的 $x_0$，等价于 $\mathscr{L}(E)$ 上范数的定义不等式 (7)。

#### 命题 2 {#fvr-iv-s2-prop-2 .statement tag=08CW}

*设B是E的连续自同态，独立于t，并且对于所有$t \in J$与A(t)可交换；那么 B 对于所有 t 都使用 $C(t, t_0)$ 进行通勤，而 J 中则使用 $t_0$。*

确实，由 (5)
$$
\frac{d}{dt}(BC) = BAC = ABC \quad \text{and} \quad \frac{d}{dt}(CB) = ACB ,
$$
所以$\frac{d}{dt}(BC - CB) = A(BC - CB)$；但是$BC(t_0, t_0) - C(t_0, t_0)B = 0$，所以（IV，p. 179，第1）$BC(t, t_0) - C(t, t_0)B = 0$对于所有$t \in J$。

道具的一个重要例子。 2 是，其中 E 被赋予相对于复数* $\mathbf{C}$ 的 *域的范数向量空间的结构，并且对于每个 $t \in J$，$A(t)$ 是 E 的自同态对于这个向量空间结构；这意味着 $A(t)$ 与 E 的连续自同态 $x \mapsto tx$ 通勤（对于向量空间结构 *超过* $\mathbf{R}$）；那么$C(t, t_0)$与这个自同态交换，这意味着对于J中的任何$t$和$t_0$，映射$C(t, t_0)$是E上范数向量空间结构的连续自同态 $\mathbf{C}$。

### 3. 对非齐次线性方程积分

对非齐次线性方程积分

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x} + \mathbf{b}(t)
$$

约化对关联的齐次方程进行积分

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x}
$$

并评估一个原语。与第记号。 IV、p. 179中的2个，让我们从IV、p. 179、$\mathbf{z} = C(t_0, t).\mathbf{x}$的第二个公式开始放入$\mathbf{x} = C(t, t_0).\mathbf{z}$、从而；如果 $\mathbf{x}$ 是 (2) 的积分，则 $\mathbf{z}$ 是方程 $\frac{d}{dt}\left(C(t, t_0).\mathbf{z}\right) = A(t)C(t, t_0).\mathbf{z} + \mathbf{b}(t)$ 的积分；由于双线性映射

$$
(U, y) \mapsto U.y
$$

$\mathscr{L}(\mathbf{E}) \times \mathbf{E}$ 到 $\mathbf{E}$ 是连续的（\emph{Gen. Top.}，X，p. 297，道具 6），$\mathbf{z}$ 承认导数（除了 J 的可数子集），并且可以通过公式来微分双线性函数（I，p. 6，道具 3）

$$
\frac{d}{dt}\left(C(t, t_0).\mathbf{z}\right) = \frac{dC(t, t_0)}{dt}.\mathbf{z} + C(t, t_0).\frac{d\mathbf{z}}{dt} = A(t)C(t, t_0).\mathbf{z} + C(t, t_0).\frac{d\mathbf{z}}{dt}
$$

（根据（5）（IV，p. 179），替换$dC(t, t_0)/dt$乘$A(t)C(t, t_0)$）。 $\mathbf{z}$ 然后约化到 $C(t, t_0).d\mathbf{z}/dt = \mathbf{b}(t)$ 的方程，或者再次到

$$
\frac{d\mathbf{z}}{dt} = C(t_0, t).\mathbf{b}(t)
$$

由IV的第二个公式(6)，p. 179。现在等式(8)的右边是J上的调节函数，通过将调节的函数$U$和$y$代入连续双线性函数$U.y$(\emph{cf.}II， p. 55，2)；因此，方程 (8) 在 $t_0$ 处有一个且仅有一个积分值 $\mathbf{x}_0$，由公式给出

$$
\mathbf{z}(t) = \mathbf{x}_0 + \int_{t_0}^t C(t_0, s).\mathbf{b}(s)\,ds.
$$

由于有 $C(t, t_0).\int_{t_0}^t C(t_0, s).\mathbf{b}(s)\,ds = \int_{t_0}^t C(t, t_0)C(t_0, s).\mathbf{b}(s)\,ds$ (II, p. 59, 公式 (9))，因此可以得到以下结果（考虑到 IV, p. 179 的第一个公式 (6)）：

#### 命题 3 {#fvr-iv-s2-prop-3 .statement tag=08CX}

*第记号。 2* (IV, p. 179), *对于每个点* $(t_0, \mathbf{x}_0)$ *的* $J \times \mathbf{E}$ *线性方程的积分* (2) *定义于* $J$ *并等于* $\mathbf{x}_0$ *在* $t_0$ *由下式给出公式*

$$
\mathbf{u}(t) = C(t, t_0).\mathbf{x}_0 + \int_{t_0}^t C(t, s).\mathbf{b}(s)\,ds.
$$

方法导致公式(10)，其中将函数$\mathbf{z}$作为新的未知数函数，通常被称为“参数变化的方法”。

### 4. 标量微分方程线性系统积分的基本系统

在这个小节和接下来的我们将考虑这样的情况，其中E是有限维n的向量空间超过域$\mathbf{C}$的复数（因此维数2n超过$\mathbf{R}$），并且对于每个$t \in J$， $A(t)$ 是 E 的自同态相对于向量空间结构的$\mathbf{C}$。然后，可以将认同$A(t)$及其矩阵$(a_{ij}(t))$相对于E的基（超过域$\mathbf{C}$）进行定义，$a_{ij}$这次是$n^2$复数函数，并且对 J 进行监管；令 $x_j$ ($1 \leq j \leq n$) 表示向量 $x \in E$ 相对于所选基的（复）分量，线性方程

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x} + \mathbf{b}(t)
$$

再次等于系统

$$
\frac{dx_i}{dt} = \sum_{j=1}^n a_{ij}(t)x_j + b_i(t) \qquad (1 \leq i \leq n).
$$

定理 1 (IV, p. 179) 和 2 (IV, p. 179) 和道具。 2 (IV, p. 181) 那么证明对于 E 中的每个 $\mathbf{x}_0 = (x_{k0})_{1 \leq k \leq n}$，存在且仅有一个方程的积分 $\mathbf{u} = (u_k)_{1 \leq k \leq n}$

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x}
$$

定义在 E 上且等于点 $t_0$ 处的 $\mathbf{x}_0$；这个积分可以写成

$$
\mathbf{u}(t, t_0, \mathbf{x}_0) = C(t, t_0).\mathbf{x}_0,
$$

$C(t, t_0)$是阶$n$的可逆平方矩阵$(c_{ij}(t, t_0))$，其条目是$J \times J$上的连续复数函数，因此$t \mapsto c_{ij}(t, t_0)$是受监管函数的原语在 J 上。

在特殊情况下 $n = 1$ 系统 (3) 约化为单个标量方程

$$
\frac{dx}{dt} = a(t)x + b(t)
$$

$a(t)$ 和 $b(t)$ 在 J) 上受到复杂调节函数；立即验证（一个元素）矩阵$C(t, t_0)$等于$\exp \left( \int_{t_0}^t a(s)\, ds \right)$； (11) 在点 $t_0$ 处等于 $x_0$ 的积分因此由公式明确给出

$$
u(t) = x_0 \exp \left( \int_{t_0}^t a(s)\, ds \right) + \int_{t_0}^t b(s) \exp \left( \int_{t_0}^\tau a(\tau)\, d\tau \right) ds.
$$

从J到E的连续映射的空间$\mathscr{C}(J; E)$中，由于拓扑的紧收敛性，式(4)积分的集合$\mathscr{I}$为向量子空间(超过$\mathbf{C}$)与 E 同构的，因此与 $\mathbf{C}^n$（IV、p. 180，对应 1，以及 IV、p. 181，道具 2）。

这个空间（超过域$\mathbf{C}$）的基$(\mathbf{u}_j)_{1 \leq j \leq n}$被称为（4）积分的*基本系统*。

#### 命题 4 {#fvr-iv-s2-prop-4 .statement tag=08CY}

*对于方程（4）的$n$整的$\mathbf{u}_j$（$1 \leq j \leq n$）到形式基本系统，它们在点$t_0 \in J$处的值$\mathbf{u}_j(t_0)$是线性独立的向量是必要且充分的$E$.*

事实上，与每个$\mathbf{x}_0 \in E$关联积分$t \mapsto C(t, t_0).\mathbf{x}_0$的映射是$E$到$\mathscr{I}$的同构（IV，p. 180，相关1和IV，p. 181，道具2）。

如果$(\mathbf{e}_j)_{1 \leq j \leq n}$是$E$超过$\mathbf{C}$的任何基，则$n$整的
$$
\mathbf{u}_j(t) = C(t, t_0).\mathbf{e}_j \qquad (1 \leq j \leq n)
$$
因此形式是一个基本的系统；如果将$C(t, t_0)$与矩阵相对于基$(\mathbf{e}_j)$进行识别，则$\mathbf{u}_j$的积分恰好是矩阵$C(t, t_0)$的*列*。 (4) 在点 $t_0$ 取值 $\mathbf{x}_0 = \sum_{j=1}^n \lambda_j \mathbf{e}_j$ 的积分则为 $C(t, t_0).\mathbf{x}_0 = \sum_{k=1}^n \lambda_k \mathbf{u}_k(t)$。

给定（4）一个项的*任何*$n$整的$\mathbf{u}_j$（$1 \leq j \leq n$），这些$n$积分在点$t \in J$相对于$E$的基$(\mathbf{e}_j)_{1 \leq j \leq n}$的*行列式*，行列式
$$
\Delta(t) = (\mathbf{u}_1(t), \ \mathbf{u}_2(t), \ \ldots, \ \mathbf{u}_n(t))
$$
$n$ 向量 $\mathbf{u}_j(t)$ 相对于基 $(\mathbf{e}_j)$ (*Alg.*, III, p. 522)。其中一个有 (*Alg.*, III, p. 523, 道具 2)
$$
\Delta(t) = \Delta(t_0) \det \left( C(t, t_0) \right).
$$

通过道具。 IV、p. 184 的 4，对于$(\mathbf{u}_j)_{1 \leq j \leq n}$ 作为 (4) 积分的基本系统，$\mathbf{u}_j$ 的行列式 $\Delta(t)$ 在某个点 $t_0$ 处为 $\neq 0$ 是必要且充分的$J$； 公式 (14) 然后表明$\Delta(t) \neq 0$在$J$的每点处，在其他字中，向量$\mathbf{u}_j(t)$($1 \leq j \leq n$)始终是线性独立的。

#### 命题 5 {#fvr-iv-s2-prop-5 .statement tag=08CZ}

*矩阵 $C(t, t_0)$ 的行列式由公式给出*
$$
\det \left( C(t, t_0) \right) = \exp \left( \int_{t_0}^t \operatorname{Tr}(A(s)) \, ds \right).
$$
(15)

事实上，如果有人将 $\delta(t) = \det \left( C(t, t_0) \right)$ 放入公式中，则可以得到行列式的导数 (I, p. 8, 公式 (3))
$$
\frac{d \delta}{dt} = \operatorname{Tr} \left( \frac{dC(t, t_0)}{dt} (C(t, t_0))^{-1} \right) \delta(t)
$$

即由IV、p. 179满足$C(t, t_0)$的微分方程(5)，

$$
\frac{d \delta}{dt} = \operatorname{Tr}(A(t)) \delta(t).
$$

由于 $\delta(t_0) = 1$ 公式 (15) 由标量线性方程积分的表达式 (12) (IV, p. 183) 得出。

指定 (4) 确定该方程的所有积分的 $n$ 线性独立积分，正如我们刚才所看到的。现在我们将证明，对于$1 \leq p \leq n$，方程（4）约化的$p$线性独立积分$\mathbf{u}_j$（$1 \leq j \leq p$）的知识，将该方程与$n - p$标量方程的齐次线性系统积分。假设在区间 $K \subset J$ 上有 $n - p$ 映射

$$
\mathbf{u}_{p+k} \quad (1 \leq k \leq n - p)
$$

$K$ 到 $E$，它们是 $K$ 上受监管的函数的原语，因此，对于每个 $t \in K$，$n$ 向量 $\mathbf{u}_j(t)$ ($1 \leq j \leq n$) 形式基 $E$。

For every point $t_1 \in J$ there always exists an interval $K$, a neighbourhood of $t_1$ in $J$, on which there are defined $n - p$ functions $\mathbf{u}_{p+k}$ ($1 \leq k \leq n - p$) having the preceding properties. For, let $(\mathbf{e}_i)_{1 \leq i \leq n}$ be a basis of $E$; there exist $n - p$ vectors of this basis which form with the $\mathbf{u}_j(t_1)$ ($1 \leq j \leq p$) a basis of $E$ (Alg., II, p. 292, th. 2); suppose for example that they are $\mathbf{e}_{p+1}, \ldots, \mathbf{e}_n$; since the determinant $\det(\mathbf{u}_1(t), \ldots, \mathbf{u}_p(t), \mathbf{e}_{p+1}, \ldots, \mathbf{e}_n)$ (with respect to the basis $(\mathbf{e}_i)$) is a continuous function of $t$ and does not vanish for $t = t_1$ there exists a neighbourhood $K$ of $t_1$ on which it does not vanish; one can then take $\mathbf{u}_{p+k}(t) = \mathbf{e}_{p+k}$ ($1 \leq k \leq n - p$) for $t \in K$.

存在阶$n$的可逆矩阵$B(t)$，其元素是$K$上受管制函数的原语，使得$B(t).\mathbf{e}_j = \mathbf{u}_j(t)$对应于$1 \leq j \leq n$。让我们把$x = B(t).y$；那么$y$满足方程$\frac{dB}{dt}.y + B(t).\frac{dy}{dt} = A(t)B(t).y$，也可以写成

$$
\frac{dy}{dt} = (B(t))^{-1} \left( A(t)B(t) - \frac{dB}{dt} \right) .y = H(t).y
$$

其中 $H(t) = (h_{jk}(t))$ 是矩阵，并且 $K$ 上有受监管的条目。通过 $B(t)$ 的定义，该线性方程允许 $p$ 常数向量 $\mathbf{e}_j$ ($1 \leq j \leq p$) 作为积分；立即一个结论必然 $h_{jk}(t) = 0$ 对应 $1 \leq k \leq p$；因此，$y$的分量$y_k$（相对于基$(\mathbf{e}_i)$）以及指标$k \geq p + 1$满足是$n - p$方程的齐次线性系统；一旦确定了这个系统的解，指标$j \leq p$的$dy_j/dt$与$y_k$的函数与$k \geq p + 1$是线性的，所以是已知的，并且这些函数的原语将给出$y_j$ 指标$j \leq p$。

特别是，当知道IV、p. 183的方程（4）的$n - 1$线性无关积分时，将该方程约化积分到单个齐次标量方程，然后对$n$基元求值。

#### 注 1 {#fvr-iv-s2-n4-rem-1 .statement tag=08D0}

上述所有内容也适用于 E 为维数 $n$ 超过域 $\mathbf{R}$ 且$A(t)$ 为每个 $t \in J$ 的 E 的自同态的情况：整个过程中只需替换 $\mathbf{C}$ $\mathbf{R}$。

#### 注 2 {#fvr-iv-s2-n4-rem-2 .statement tag=08D1}

令 $A(t) = (a_{ij}(t))$ 为阶 $n$ 的平方矩阵，其条目是 $J$ 上 $t$ 的实数（或复数）调节的函数，并令 $C(t, t_0) = (c_{ij}(t, t_0))$ 为矩阵的解析相应的线性系统 (3) (IV, p. 22)。令 F 为 $\mathbf{R}$（或$\mathbf{C}$）上的任意完全赋范空间，并考虑线性微分方程的系统

$$
\frac{dy_i}{dt} = \sum_{j=1}^n a_{ij}(t) y_j
$$

其中未知的函数$y_j$，取F中的值。系统的解$(\mathbf{u}_j)_{1 \leq j \leq n}$是直接的，使得$1 \leq j \leq n$的$\mathbf{u}_j(t_0) = \mathbf{d}_j$（$\mathbf{d}_j$在F中是任意的）由公式给出

$$
\mathbf{u}_i(t) = \sum_{j=1}^n c_{ij}(t, t_0) \mathbf{d}_j \qquad (1 \leq i \leq n).
$$

我们特别考虑$A(t)$是有限维$n$的向量空间E的自同态超过$\mathbf{C}$的情况，使得存在E的基相对于$A(t)$的矩阵对于每个都有实数元素 $t \in J$。 那么上面显示（通过IV，p. 179的第1个），关于相同基的解析矩阵$C(t, t_0)$也有实数元素：只需考虑向量空间$E_0$超过$\mathbf{R}$生成考虑E的基，对于注，$A(t)$到$E_0$的限制是这个向量空间的自同态。

### 5. 伴随方程

假设空间 E 始终为有限维 $n$ 超过 $\mathbf{C}$，令 $E^*$ 为其对偶 (A, II, p. 40)，即空间为维数 $n$ 超过 $\mathbf{C}$ （阿尔格.，II，p. 299，第 4）；在$E \times E^*$（代数，II，p. 234）上定义的规范双线性形式$\langle \mathbf{x}, \mathbf{x}^* \rangle$在这个乘积上是连续的（是$\mathbf{x} \in E$和$\mathbf{x}^* \in E^*$分量中的多项式）。

给定齐次线性方程 (4) (IV, p. 183)，其中 $t \mapsto A(t)$ 是 J 到 $\mathscr{L}(E)$ 的调节映射，让我们看看是否存在 J 到 $E^*$ 的映射 $t \mapsto \mathbf{v}(t)$，即 J 上调节函数的原语，并且使得当 $\mathbf{u}$ 是 (4) 的任意解时，标量函数 $t \mapsto \langle \mathbf{u}(t), \mathbf{v}(t) \rangle$ 在 J 上是常数；同样的，写出这个函数的导数在每个点处应该是零，其中$\mathbf{u}$和$\mathbf{v}$是可微的，也就是说，必须有

$$
\left\langle \frac{d\mathbf{u}}{dt}, \mathbf{v}(t) \right\rangle + \left\langle \mathbf{u}(t), \frac{d\mathbf{v}}{dt} \right\rangle = 0
$$

在这样的点。

现在，根据 (4)，$\left\langle \frac{d\mathbf{u}}{dt}, \mathbf{v}(t) \right\rangle = \langle A(t).\mathbf{u}(t), \mathbf{v}(t) \rangle = -\langle \mathbf{u}(t), B(t).\mathbf{v}(t) \rangle$，其中 $-B(t)$ 是 $A(t)$ 的转置（代数，II，p. 234）。 关系 $\mathbf{v}$ 必须满足因此可以写成

$$
\left\langle \mathbf{u}(t), \frac{d\mathbf{v}}{dt} - B(t).\mathbf{v}(t) \right\rangle = 0
$$

总共点，其中$A(t)$是连续的，$\mathbf{v}(t)$是可微的。现在对于这样的点 $t$ 和*任意* 点 $\mathbf{x}_0 \in \mathrm{E}$ 来说，存在。 (4)的IV、p. 179、解$\mathbf{u}$中的1使得$\mathbf{u}(t) = \mathbf{x}_0$；因而，对于*所有* $\mathbf{x}_0 \in \mathrm{E}$，必须有$\left\langle \mathbf{x}_0, \frac{d\mathbf{v}}{dt} - B(t).\mathbf{v}(t) \right\rangle = 0$，这需要$\frac{d\mathbf{v}}{dt} - B(t).\mathbf{v}(t) = 0$。因而：

#### 命题 6 {#fvr-iv-s2-prop-6 .statement tag=08D2}

*将 J 的映射 $t \mapsto \mathbf{v}(t)$ 转换为 $\mathrm{E}^*$（J 上受调节的函数的原语），对于方程* (4) 的每个解 $\mathbf{u}$，$\langle \mathbf{u}(t), \mathbf{v}(t) \rangle$ 在 J 上是常数* (4) * of IV, p. 183 当且仅当$\mathbf{v}$ 是齐次线性方程的解*

$$
\frac{d\mathbf{x}}{dt} = B(t).\mathbf{x} \tag{16}
$$

*其中 $-B(t)$ 是 $A(t)$ 的转置。*

方程（16）称为（4）的*伴随*；显然 (4) 是 (16) 的伴随。将矩阵$B(t)$的元素调节到J上的函数或$t$，上面在线性方程组上得到的结果适用于(16)。特别是，(16) 在点 $t_0$ 取值 $\mathbf{x}_0^*$ 的积分可写为 $H(t, t_0).\mathbf{x}_0^*$，其中 $H(t, t_0)$ 是 $\mathrm{E}^*$ 自身的双射线性映射，与方程的积分相同

$$
\frac{dV}{dt} = B(t)V \tag{17}
$$

需要值 $I$ 点 $t_0$。结果有（IV、p. 179的记号）

$$
\left\langle C(t, t_0).\mathbf{x}_0, H(t, t_0).\mathbf{x}_0^* \right\rangle = \left\langle \mathbf{x}_0, \mathbf{x}_0^* \right\rangle
$$

对于任意 $\mathbf{x}_0 \in \mathrm{E}$ 和 $\mathbf{x}_0^* \in \mathrm{E}^*$，这表明

$$
H(t, t_0) = \check{C}(t, t_0) \tag{18}
$$

（$C(t, t_0)$的*对梯度*）。特别是，如果知道伴随方程 (16) 的积分的基本系统矩阵 $H(t, t_0)$ 确定的，则 $C(t, t_0)$ 也已确定，因而，方程 (4) 的*所有*积分也已确定。

#### 注 {#fvr-iv-s2-n5-rem-1 .statement tag=08D3}

令 E 和 F 是 $\mathbf{R}$（或$\mathbf{C}$）上的两个完整范数空间，以及 $(\mathbf{x}, \mathbf{y}) \mapsto \langle \mathbf{x}, \mathbf{y} \rangle$ $\mathrm{E} \times \mathrm{F}$ 上的*连续* 双线性形式，使得关系 “$\langle \mathbf{x}, \mathbf{y} \rangle = 0$ 对于所有 $\mathbf{y} \in \mathrm{F}$”（分别为关系）。 $\langle \mathbf{x}, \mathbf{y} \rangle = 0$ 对于所有 $\mathbf{x} \in \mathrm{E}$”）意味着 $\mathbf{x} = 0$（或$\mathbf{y} = 0$）。进一步假设对于每个 $t \in \mathrm{J}$，F 都有一个连续的线性映射 $B(t)$ 到其自身，这样 $\langle A(t).\mathbf{x}, \mathbf{y} \rangle + \langle \mathbf{x}, B(t).\mathbf{y} \rangle = 0$ 对于每个 $(\mathbf{x}, \mathbf{y}) \in \mathrm{E} \times \mathrm{F}$。在这些情况下， 之前认为，对于 J 的映射 $t \mapsto \mathbf{v}(t)$ 到 F（受规管函数的原语），使得 $\langle \mathbf{u}(t), \mathbf{v}(t) \rangle$ 对于 (4) 的*每个*整的 $\mathbf{u}$ 是*常数*，$\mathbf{v}$ 应该是以下的积分是充分必要的： （16），我们再次将其称为（4）的*伴随*。

### 6. 常系数线性微分方程

再次假设 E 是 $\mathbf{R}$ 上的任意完全范数空间；设 A 为 A 的连续自同态，与 t 无关，并考虑齐次线性方程

$$
\frac{d\mathbf{x}}{dt} = A.\mathbf{x}.
$$

当E为有限维时，方程(19)等价于标量微分方程的齐次系统(3)(IV，p. 183)，其中系数$a_{ij}$是常数。

到了。 1 (IV,p. 179)，(19)的每个积分都定义在所有$\mathbf{R}$上；到了。 2 (IV, p. 179) (19) 在点 $t_0 \in \mathbf{R}$ 取值 $\mathbf{x}_0$ 的积分可写为 $C(t, t_0)\mathbf{x}_0$，其中 $C(t, t_0)$ 是 E 自身的双射双连续线性映射，满足方程

$$
\frac{dU}{dt} = AU
$$

并且是$C(t_0, t_0) = I$。而且，我们还有身份

$$
C(t + \tau, t_0 + \tau) = C(t, t_0)
$$

对于任何 $\tau \in \mathbf{R}$：事实上，通过 (20) 有 $dC(s, t_0 + \tau)/ds = AC(s, t_0 + \tau)$，并且由于 A 是常数，因此也有

$$
\frac{dC(t + \tau, t_0 + \tau)}{dt} = AC(t + \tau, t_0 + \tau);
$$

而且

$$
C(t_0 + \tau, t_0 + \tau) = I = C(t_0, t_0).
$$

从而我们有恒等式 (21)，因为 (20) 在点 $t_0$ 处等于 I 的积分是唯一的。

如果有人放入$C_0(t) = C(t, 0)$，则$C(t, t_0) = C_0(t - t_0)$；此外，对于每个 $\lambda \in \mathbf{R}$，$C_0(\lambda t)$ 与方程的积分相同

$$
\frac{dU}{dt} = \lambda AU
$$

值 I 点 0。我们制作以下定义：

#### 定义 1 {#fvr-iv-s2-def-1 .statement tag=08D4}

*给定 E 的连续自同态 A，我们用 E 的 $e^A$ 或 $\exp A$ 自同构表示等于值在点 $t = 1$ 的方程 (20) 整的，其中值 I 在点$t = 0$.*

有了这个记号注前面的 def。 1 表明

$$
C(t, t_0) = \exp \left( A(t - t_0) \right).
$$

刚刚引入的指数记号由以下属性证明，这些属性与函数 exp z 的属性完全相似，对于 z 实数或复数（cf. III、p. 98 和 106）：

#### 命题 7 {#fvr-iv-s2-prop-7 .statement tag=08D5}

1' *映射* $X \mapsto e^X$ *是* $\mathscr{L}(E)$ *的连续映射 *进入* E * 的自同构群（*可逆元 of* $\mathscr{L}(E)$）。

2 *映射* $t \mapsto e^{Xt}$ *的* $\mathbf{R}$ *到* $\mathscr{L}(E)$ *可微，并且*

$$
\frac{d}{dt} (e^{Xt}) = X e^{Xt} = e^{Xt} X.
$$ (24)

3 *对于任何* $X \in \mathscr{L}(E)$ *一个有*

$$
e^X = \sum_{n=0}^{\infty} \frac{X^n}{n!}
$$ (25)

*右侧绝对一致地收敛于* $\mathscr{L}(E)$的每个有界子集； *特别是，*$e^{It} = e^t I$*对于*$t \in \mathbf{R}$。

4) *如果* X *和* Y *通勤，那么* Y *和* $e^Y$ *通勤与* $e^X$，*和*

$$
e^{X+Y} = e^X e^Y.
$$ (26)

关系 (24) 由 $C(t, 0)$ 的表达式 (23) 得出，并且根据这个函数是 (20) 的积分这一事实；通过对 n 进行递归，从 (24) 推出 $t \mapsto e^{Xt}$ 在 $\mathbf{R}$ 上无限可微，并且

$$
D^n (e^{Xt}) = X^n e^{Xt}.
$$

根据泰勒的公式，我们可以写出

$$
e^X = I + \frac{X}{1!} + \frac{X^2}{2!} + \cdots + \frac{X^n}{n!} + X^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{Xt} \, dt.
$$ (27)

另一方面，科。 IV、p. 181中的3个表示$\| e^{Xt} \| \leq \exp (\| X \| |t| )$。因此公式(27)中的余数$r_n(X) = X^{n+1} \int_0^1 \frac{(1-t)^n}{n!} e^{Xt} \, dt$满足不等式

$$
\| r_n(X) \| \leq \frac{\| X \|^{n+1}}{(n+1)!} e^{\| X \| }
$$

从而推论出公式 (25)，右侧的级数绝对一致地收敛于$\mathscr{L}(E)$的每个有界子集。对于元素 $X,\ T$ $\mathscr{L}(E)$ 中的每一个对，因此有

$$
e^{X+T} - e^X = \sum_{n=1}^{\infty} \frac{1}{n!} ((X+T)^n - X^n ).
$$

现在，可以写 $(X + T)^n - X^n = \sum_{(V_i)} V_1 V_2 \ldots V_n$，其中和取代 $\mathscr{L}(E)$ 的元素的 $2^n - 1$ 序列 $(V_i)$，使得 $V_i = X$ 或 $V_i = T$ 代表 $1 \leq i \leq n$，并且至少其中之一$V_i$等于$T$； 不等式
$$
\|(X + T)^n - X^n\| \leq (\|X\| + \|T\|)^n - \|X\|^n
$$
立即跟进，从而
$$
\|\exp(X + T) - \exp X\| \leq \exp \left( \|X\| + \|T\| \right) - \exp \|X\|
$$
这就建立了映射 $X \mapsto \exp X$ 的连续性。

Finally, if $X$ and $Y$ commute, then $Y$ commutes with $e^{Xt}$ (IV, p. 181, prop. 2), so
$$
\frac{d}{dt} (e^{Xt} e^{Yt}) = X e^{Xt} e^{Yt} + e^{Xt} (Y e^{Yt}) = (X + Y) e^{Xt} e^{Yt}.
$$
Since, on the other hand, $e^{Xt} e^{Yt}$ is equal to $I$ for $t = 0$, one has $e^{Xt} e^{Yt} = e^{(X+Y)t}$, whence formula (26). 从后者，我们特别推断出对于任意实数$s$和$t$，有
$$
e^{X(s+t)} = e^{Xs} e^{Xt}
$$
还有那个
$$
e^{-X} = (e^X)^{-1}.
$$

相反，如果$X$和$Y$不再被假设为通勤，则（26）中的注不需要保持有效：实际上，这意味着$\exp X$和$\exp Y$总是通勤，但事实并非如此，如简单的例（IV，p. 204，exerc）所示。 3）。

现在让我们假设 $E$ 是有限维的向量空间 * 超过域* $\mathbf{C}$，并且 $A$ 自同态是 $E$（对于其向量空间结构超过 $\mathbf{C}$）哪一个可以确定及其矩阵相对于$E$的基；那么，对于所有$t \in \mathbf{R}$，对于相同的结构，$e^{At}$是$E$的自同构（IV，p. 181，道具2）。令 $r_k$ ($1 \leq k \leq q$) 为自同态 $A$ 的*特征多项式* $\varphi(r) = \det(A - rI)$ 的不同根（$\mathbf{C}$中）（$A$的“特征根”）；如果 $n_k$ 是$r_k$ 重数阶，则$\sum_{k=1}^q n_k = n$。我们知道 (Alg., VII, 31, n° 3) 对于每个根 $r_k$，$E$、维数 $n_k$ 都有对应子空间 $E_k$，这样 $E_k$在$A$下*稳定*，并且$E$是$E_k$的*直和*：$E_k$可以定义为向量$\mathbf{x}$的子空间，这样
$$
(A - r_k I)^{n_k} . \mathbf{x} = 0.
$$
令$\mathbf{a}$为$E$中的任意向量；可以写 $\mathbf{a} = \sum_{k=1}^q \mathbf{a}_k$，其中 $\mathbf{a}_k \in E_k$； IV、p. 188的方程 (19) 的积分，在点 $t = 0$ 取值 $\mathbf{a}$ 则由下式给出
$$
\mathbf{u}(t) = e^{At} . \mathbf{a} = \sum_{k=1}^q e^{At} . \mathbf{a}_k = \sum_{k=1}^q e^{r_k t} e^{(A - r_k I)t} . \mathbf{a}_k.
$$

但自从 $\mathbf{a}_k \in E_k$ 以来，

$$
e^{(A - r_k I)t} \cdot \mathbf{a}_k = \mathbf{a}_k + \frac{t}{1!}(A - r_k I) \cdot \mathbf{a}_k + \frac{t^2}{2!}(A - r_k I)^2 \cdot \mathbf{a}_k + \cdots
$$
$$
+ \frac{t^{n_k - 1}}{(n_k - 1)!}(A - r_k I)^{n_k - 1} \cdot \mathbf{a}_k .
$$

因此，IV、p. 188的方程（19）的每个积分都可以写为

$$
\mathbf{u}(t) = \sum_{k=1}^q e^{r_k t} \mathbf{p}_k(t)
$$

其中 $\mathbf{p}_k(t)$ 是 $t$ 中的多项式，系数为向量空间 $E_k$ 和次数 $\leq n_k - 1$。特别地，如果$A$的特征方程的所有根都是*简单*，空间$E_k$($1 \leq k \leq n$)在域$\mathbf{C}$上都是维数1，所以存在$n$向量 $c_k$使得$n$函数$e^{r_k t} c_k$($1 \leq k \leq n$)形式是IV、p. 188的方程(19)积分的基本系统。

自同态$A$的特征根也称为IV、p. 188的*线性方程*(19)的特征根。人们可以观察到，通过写出函数$c e^{r t}$是向量$c \neq 0$的(19)整的，就可以得到$A$的特征方程。

当明确确定根$r_k$($1 \leq k \leq q$)，从而确定重数$n_k$或$r_k$的阶时，实际上可以通过写出该方程满足IV的表达式(32)来获得(19)的积分， p. 191，其中$\mathbf{p}_k$是次数$\leq n_k - 1$的任意多项式，系数*in*$E$；在确定如此获得的方程两侧的$e^{r_k t}$（对于$1 \leq k \leq q$）的系数时，我们可以得到多项式$\mathbf{p}_k$的系数的线性方程：我们很容易建立这些方程次数的确定项$\mathbf{p}_k$的$> 0$为常数项的函数，后者是方程$(A - r_k I)^{n_k} \cdot \mathbf{x} = 0$的解，其中定义子空间$E_k$（“未定系数”的方法）。

#### 注 {#fvr-iv-s2-n6-rem-1 .statement tag=08D6}

当存在$E$的基使得$A$的矩阵相对于此基有*实数*元素(*cf.*IV,p. 186,*注*2)时，特征方程为$A$ 有实数系数。对于$E$的每个$\mathbf{x} = (\xi_k)_{1 \leq k \leq n}$，在考虑中以基表示，令$\overline{\mathbf{x}} = (\overline{\xi}_k)_{1 \leq k \leq n}$； 映射 $\mathbf{x} \mapsto \overline{\mathbf{x}}$ 是 $E$ 的反线性对合。知道(*Alg.*, VII)，如果$r_k$是特征方程的非实根，且$E_k$是相应的稳定子空间，则$\overline{r}_k$是具有相同重数的特征根 $n_k$为$r_k$，映射$\mathbf{x} \mapsto \overline{\mathbf{x}}$下$E_k$的像$E'_k$是稳定的子空间相应的至$\overline{r}_k$。由此推断，如果$\mathbf{u}_j$ ($1 \leq j \leq n_k$) 是$n_k$ 与值在$E_k$ 中线性无关的积分，则$2n_k$ 整的$\mathbf{u}_j + \overline{\mathbf{u}}_j,\ i(\mathbf{u}_j - \overline{\mathbf{u}}_j)$ 是线性独立的，并且相对于所选的基有$E$，是$E$*真实*函数的分量。如果$r_k$是实数特征根 *注* 2 of IV、p. 186，则表明（与记号相同）存在$n_k$线性无关积分$\mathbf{v}_j$（$1 \leq j \leq n_k$）与值在 $E_k$ 中，其成分是真实的。这样就可以得到 (19) 积分的基本系统，其分量都是*实数*。

### 7. 阶 $n$ 的线性方程

我们将 *阶* $n$ 的线性微分方程称为形式的方程

$$
D^n x - a_1(t) D^{n-1} x - \ldots - a_{n-1}(t) D x - a_n(t) x = b(t)
$$

其中 $a_k$ ($1 \leq k \leq n$) 和 $b$ 是实数变量 $t$ 的实数（复数）函数，定义在 $\mathbf{R}$ 的区间 $J$ 上。 IV、p. 164的一般过程表明该方程等价于$n$第一个阶方程的线性系统

$$
\left\{
\begin{aligned}
\frac{dx_k}{dt} &= x_{k+1} & (1 \leq k \leq n-1) \\
\frac{dx_n}{dt} &= a_1(t)x_n + a_2(t)x_{n-1} + \cdots + a_n(t)x_1 + b(t)
\end{aligned}
\right.
$$

也就是说，对于线性方程

$$
\frac{d\mathbf{x}}{dt} = A(t).\mathbf{x} + \mathbf{b}(t)
$$

我们放置 $\mathbf{x} = (x_1, x_2, \ldots, x_n) \in \mathbf{C}^n$、$\mathbf{b}(t) = (0, 0, \ldots, 0, b(t))$ 的位置，以及矩阵 $A(t)$ 的定义为

$$
A(t) = \begin{pmatrix}
0 & 1 & 0 & \ldots & 0 \\
0 & 0 & 1 & \ldots & 0 \\
\vdots & \vdots & \vdots & \ddots & \vdots \\
0 & 0 & 0 & \ldots & 1 \\
a_n(t) & a_{n-1}(t) & a_{n-2}(t) & \ldots & a_1(t)
\end{pmatrix}.
$$

因此，阶$n$线性方程的研究由应用上述特定线性方程（35）的一般结果组成。对于每个间隔 $J$，其中函数 $a_j$ ($1 \leq j \leq n$) 和 $b$ 受到*调节*，存在且仅有一个函数 $u$，在 $J$ 上定义，具有阶的连续导数$n-1$，以及阶$n$在此区间上的受管制导数（可数集合的点除外），满足(33)关于$J$的可数子集的补集，并且使得

$$
u(t_0) = x_0, \qquad Du(t_0) = x_0', \ldots, \quad D^{n-1}u(t_0) = x_0^{(n-1)}
$$

其中$t_0$是$J$的任意点，$x_0, x_0', \ldots, x_0^{(n-1)}$是$n$任意复数。

对于齐次方程的 $p$ 整的 $u_j$ ($1 \leq j \leq p$)

$$
D^n x - a_1(t) D^{n-1} x - \ldots - a_{n-1}(t) D x - a_n(t) x = 0
$$

与 (33) 线性无关（在从$J$到$\mathbf{C}$连续映射的空间$C(J; \mathbf{C})$中，视为向量空间超过$\mathbf{C}$），相应的$p$积分是充分必要的齐次方程$d\mathbf{x}/dt = A(t).\mathbf{x}$的$\mathbf{u}_j = (u_j, Du_j, \ldots, D^{n-1}u_j)$应该是线性独立的（在连续映射从$J$到$\mathbf{C}^n$的空间$C(J; \mathbf{C}^n)$中）。显然这个条件是必要的。

相反，如果存在 $n$ 复数常量 $\lambda_j$，而不是全部零，使得 $\sum_{j=1}^n \lambda_j u_j(t) = 0$ 在 $J$ 上相同，则可以推断对于每个整数 $k$，$\sum_{j=1}^n \lambda_j D^k u_j(t) = 0$ 在 $J$ 上，这样$1 \leq k \leq n - 1$，这意味着$\sum_{j=1}^n \lambda_j \mathbf{u}_j(t) = 0$在$J$上。

因而（IV，p. 180，cor.1）

#### 命题 8 {#fvr-iv-s2-prop-8 .statement tag=08D7}

*在 $J$ 上定义的齐次线性方程 (37) 的积分集合是维数 $n$ 在域 $\mathbf{C}$ 上的向量空间。*

给定方程（37）的任何$n$整的$u_j$（$1 \leq j \leq n$），我们将这个系统积分的*Wronskian*称为相应的$n$积分的行列式（相对于$\mathbf{C}^n$的典范基）方程$d\mathbf{x}/dt = A(t).\mathbf{x}$的$\mathbf{u}_j$，即函数

$$
W(t) = \begin{vmatrix}
u_1(t) & u_2(t) & \ldots & u_n(t) \\
Du_1(t) & Du_2(t) & \ldots & Du_n(t) \\
\vdots & \vdots & \ddots & \vdots \\
D^{n-1}u_1(t) & D^{n-1}u_2(t) & \ldots & D^{n-1}u_n(t)
\end{vmatrix}.
$$

对于$n$整的$u_j$线性无关，$W(t) \neq 0$在$J$上是必要且充分的；此外，$W(t_0) \neq 0$在$J$*仅一个*$t_0$就足够了（IV，p. 184，道具4）；此外，还有 (IV, p. 184, 命题 5)

$$
W(t) = W(t_0) \exp \left( \int_{t_0}^t a_1(s)\, ds \right).
$$ (38)

我们认同方程（35）的解$C(t, t_0)$及其矩阵相对于$\mathbf{C}^n$的典范基； 矩阵的列 $\mathbf{v}_j(t, t_0)$ ($1 \leq j \leq n$) 则为 $n$ 线性独立积分

$$
\mathbf{v}_j(t, t_0) = (v_j(t, t_0), Dv_j(t, t_0), \ldots, D^{n-1}v_j(t, t_0))
$$

齐次方程 $d\mathbf{x}/dt = A(t).\mathbf{x}$ 的对应到 $n$ 方程 (37) 的线性独立积分 $v_j(t, t_0)$ 使得

$$
D^{k-1}v_j(t_0, t_0) = \delta_{jk}
$$

（克罗内克三角洲）$1 \leq j \leq n, 1 \leq k \leq n$（同意放置$D^0 v_j = v_j$）。特别是，应用于方程（35）的参数变化（IV，p. 182）的方法给出了（33）的特定积分，等于0及其在点$t_0$，函数处的第一个$n-1$导数

$$
w(t) = \int_{t_0}^t v_n(t, s)b(s)\, ds.
$$ (39)

在方程 $D^n x = b(t)$ 公式 (39) 的特殊情况下，再次给出公式 ，表示调节的函数 $b(t)$ 的$n^{th}$原语，其在点 $t_0$处的第一个$n - 1$导数消失，即
$$
w(t) = \int_{t_0}^t b(s) \frac{(t-s)^{n-1}}{(n-1)!} \, ds
$$
(II, p. 62, 公式 (19))：$D^n x = 0$的积分，在点 $t_0$处与它的第一个$n - 2$导数一起消失，并且其$n - 1$在那里的导数等于1，实际上是多项式$(t-t_0)^{n-1}/(n-1)!$。

### 8. 具有常数系数的阶 $n$ 线性方程

若式(33)中的系数$a_j$为常数，则相应的矩阵$A$为常数；特征方程可写为 $e^{rt}$ 为解，即
$$
r^n - a_1 r^{n-1} - \ldots - a_{n-1} r - a_n = 0.
$$
令 $r_j$ ($1 \leq j \leq q$) 为该方程的不同根，并且 $n_j$ ($1 \leq j \leq q$) 重数为根 $r_j \left( \sum_{j=1}^q n_j = n \right)$。由IV、p. 188到194的结果，对于每个根$r_j$都有对应，对于齐次方程
$$
D^n x - a_1 D^{n-1} x - \cdots - a_{n-1} D x - a_n x = 0
$$
$n_j$ 线性无关积分的系统
$$
u_{jk}(t) = e^{r_j t} p_{jk}(t),
$$
其中 $p_{jk}$ 是次数 $\leq n_j - 1$ ($1 \leq k \leq n_j$) 的多项式（具有复系数）；此外，如此获得的$n$整的$u_{jk}$（$1 \leq j \leq q,\ 1 \leq k \leq n_j$）是线性无关的。由此可见，$n_j$ 多项式 $p_{jk}$ ($1 \leq k \leq n_j$) 在空间中与次数 $\leq n_j - 1$ $t$ 中的多项式线性无关，因此形式基（超过 $\mathbf{C}$）这个空间，因为后者是维数$n_j$。其他字：

#### 命题 9 {#fvr-iv-s2-prop-9 .statement tag=08D8}

*令$r_j$ ($1 \leq j \leq q$) 为特征方程(40) 的不同根，令$n_j$ 为根 $r_j$ ($1 \leq j \leq q$) 的重数。那么 $n$ 函数 $t^k e^{r_j t}$ ($1 \leq k \leq n_j,\ 1 \leq j \leq q$) 是齐次方程 (41) 的线性独立积分。*

1 可以证明这个结果直接通过以下方式得到。从方程（41）得出，该方程的每个积分的$n^{th}$导数在$\mathbf{R}$上可微，由此可以立即通过归纳在整数$m > n$上推导出，（41）的每个积分都承认阶$m$的导数，即，在 $\mathbf{R}$ 上*可微分*。令 $\mathscr{D}$ 为$\mathbf{R}$ 上的不定可微复值函数在$\mathbf{C}$ 上的（非拓扑）向量空间； 映射$x \mapsto Dx$是这个空间的自同态，方程（41）可以写成

$$
f(D)x = 0 \tag{42}
$$

其中$f(D) = D^n - a_1 D^{n-1} - \ldots - a_{n-1} D - a_n$（代数，IV，p. 4）。

#### 命题 10 {#fvr-iv-s2-prop-10 .statement tag=08D9}

*设g和h是两个互素多项式，使得$f = gh$。 (42) 的解子空间是两个方程的解的子空间直和*

$$
g(D)x = 0, \qquad h(D)x = 0.
$$

现在，根据 Bezout 恒等式 (Alg., VII.2, th.1)，存在两个多项式 $p(D)$ 和 $q(D)$，使得 $p(D)g(D) + q(D)h(D) = 1$.对于（42）中的每一个解$x$，都可以写出$x = y + z$，其中$y = p(D)g(D)x$和$z = q(D)h(D)x$；然后是$h(D)y = p(D)(f(D)x) = 0$和$g(D)z = q(D)(f(D)x) = 0$。另一方面，如果 $g(D)x = 0$ 和 $h(D)x = 0$ 都存在，则可以推断

$$
x = p(D)(g(D)x) + q(D)(h(D)x) = 0,
$$

完成证明。

有了前面的记号就可以写

$$
f(D) = \prod_{j=1}^q (D - r_j)^{n_j}
$$

和道具。 10、由$q$上的归纳可知，(42)的解子空间是$q$方程的解子空间直和

$$
(D - r_j)^{n_j} x = 0 \qquad (1 \leq j \leq q). \tag{43}
$$

现在，每复数 $r$ 就有一个

$$
D(e^{rt} x) = e^{rt}(D + r)x \tag{44}
$$

所以 (43) 等价于

$$
D^{n_j}(e^{-r_j t} x) = 0
$$

因此有解函数$e^{r_j t} p_j(t)$，其中$p_j$穿过次数$\leq n_j - 1$多项式的集合；这样就恢复了支撑。 9 个IV、p. 194。

假设齐次方程（41）已解（即假设已找到特征根），则知道参数变化的方法可以求出非齐次方程的解

$$
D^n x - a_1 D^{n-1} x - \ldots - a_{n-1} Dx - a_n x = b(t) \tag{45}
$$

其中$b(t)$是*任意*调节的函数（IV，p. 182）；我们注，如果$b(t)$在区间J上*不定可微*，那么(45)的所有积分在J上都是不定可微的。在特殊情况$b(t) = e^{\alpha t} p(t)$，其中$p$是多项式（具有复系数），$\alpha$是任意复数，一通过以下方法更简单地获得(45)的积分。把$x = e^{\alpha t} y$；等式

$$
f(D)x = e^{\alpha t} p(t)
$$

由(44)可以写成

$$
f(\alpha + D)y = p(t)
$$

或者，将泰勒公式应用于多项式 $f(D)$，

$$
\frac{f^{(n)}(\alpha)}{n!} D^n y + \frac{f^{(n-1)}(\alpha)}{(n-1)!} D^{n-1} y + \cdots + \frac{f'(\alpha)}{1!} Dy + f(\alpha) y = p(t). \tag{46}
$$

令$m$为多项式$p(t) = \sum_{k=0}^m \lambda_k t^{m-k}$的次数；如果$f(\alpha) \neq 0$（即，如果$\alpha$不是特征根），则存在且仅有一个次数* $m$的多项式$u(t) = \sum_{k=0}^m c_k t^{m-k}$*，即(46)的解，因为系数$c_k$由下式确定线性方程组系统

$$
f(\alpha)c_k + \binom{m-k+1}{1} f'(\alpha)c_{k-1} + \binom{m-k+2}{2} f''(\alpha)c_{k-2} + \cdots
+ \binom{m}{k} f^{(k)}(\alpha)c_0 = \lambda_k \qquad (0 \leq k \leq m)
$$

显然承认只有一个解。另一方面，如果$\alpha$是根的特征，$h$是其重数，则前面的计算表明次数$m$存在且仅有一个多项式，使得$D^h y = v(t)$的每个解都是积分；在其他字中，(46) 的每个多项式解都是次数 $m + h$（“共振”）。

### 9. 常数系数线性方程的系统

当记号为n° 8时，让我们更一般地考虑$m$的系统微分方程形式

$$
\sum_{k=1}^n p_{jk}(D) x_k = b_j(t) \qquad (1 \leq j \leq m) \tag{47}
$$

其中未知数 $x_k$ ($1 \leq k \leq n$) 和右侧 $b_j$ ($1 \leq j \leq m$) 是实数变量 $t$ 的复数函数，并且其中 $p_{jk}(D)$ 是具有*常数*（复数）系数的多项式（任何次数）在微分运算符 $D$ ($1 \leq j \leq m,\ 1 \leq k \leq n$) 中。

这样的系统与IV，p. 1164（公式（5））中考虑的型不同，如下例所示：

$$
\begin{cases}
D x_1 = a(t) \\
D^2 x_1 + D x_2 + x_2 = b(t).
\end{cases}
$$

我们将把自己限制在函数 $b_j(t)$ 在区间 J 上“无限可微”的情况，并且我们只寻找在 J 上无限可微的解 $(x_k)_{1 \leq k \leq n}$。 将$\mathbf{b}(t) = (b_1(t), \ldots, b_m(t))$、（从J中的映射放入$\mathbf{C}^m$）和$\mathbf{x} = (x_1, x_2, \ldots, x_n)$、系统（47）可以写成

$$
P(D) \mathbf{x} = \mathbf{b}(t)
$$

其中$P(D)$是矩阵$(p_{jk}(D))$，有m行和n个列，其系数为D中多项式的属于到环$\mathbf{C}[D]$，系数为$\mathbf{C}$。令 $f_j(D)$ ($1 \leq j \leq r \leq \operatorname{Min}(m, n)$) 为非零的 *矩阵 $P(D)$ 的相似不变量*；人们知道 (*Alg.*, VII, p. 32) 这些是明确确定的一元多项式，例如 $f_j$ 除 $f_{j+1}$ 对于 $1 \leq j \leq r - 1$（$r$ 是 $P(D)$ 的 *秩*）；此外，还有两个分别为阶 m 和 n 的方阵 $U(D)$ 和 $V(D)$，*可逆*（分别为阶 m 和 n 的方阵环，*系数为多项式的环 $\mathbf{C}[D]$）在具有复系数的 D 中*)，并且除了 $1 \leq j \leq r$ 的对角线项 $q_{jj}(D) = f_j(D)$ 之外，矩阵 $Q(D) = (q_{jk}(D)) = U(D) P(D) V(D)$ 的所有条目均为零。现在我们输入$\mathbf{y} = V^{-1}(D) \mathbf{x}$；方程(49)等价于方程

$$
U(D) (P(D)(V(D) \mathbf{y})) = U(D) \mathbf{b}
$$

也就是说，到

$$
Q(D) \mathbf{y} = U(D) \mathbf{b}
$$

因为 $U(D)$ 是可逆的。现在，如果 $\mathbf{y} = (y_1, y_2, \ldots, y_n)$，并且如果

$$
U(D) \mathbf{b}(t) = (c_1(t), \ldots, c_m(t)),
$$

则方程(50)可写成

$$
f_j(D) y_j = c_j(t) \quad \text{for } 1 \leq j \leq r \tag{51}
$$
$$
0 = c_j(t) \quad \text{for } r + 1 \leq j \leq m. \tag{52}
$$

系统因此不承认任何无限可微解除非条件 (52) 得到满足；确定指标$j \leq r$的$y_j$，然​​后确定约化，以将r个线性微分方程与常系数积分（51）； 指标 $> r$ 的 $y_j$ 是任意无限可微的函数。一旦确定了(50)的解$\mathbf{y}$，就可以从公式$\mathbf{x} = V(D) \mathbf{y}$推出(47)的解。

#### 注 1 {#fvr-iv-s2-n9-rem-1 .statement tag=08DA}

一些多项式$f_j(D)$可能是约化到非零的常数； 相应的 $y_j$ 就完全确定了。

#### 注 2 {#fvr-iv-s2-n9-rem-2 .statement tag=08DB}

当$b_j$都是零时，即如果系统(47)是*齐次的*，则条件(52)总是满足；进一步，如果$r = n$，可以看到(47)的解的集合比维数的$\mathbf{C}$是向量空间，等于$f_j(D)$的次数*的*和，即*次数* 共 $\det(P(D))$。

#### 注 3 {#fvr-iv-s2-n9-rem-3 .statement tag=08DC}

给定多项式 $p_{jk}(D)$，系统 (47) 当右侧无限可微（或某个阶可微）时承认解，当右侧任意调节函数时可能不承认它们：这由例 (48) 表示，它没有当 $a(t)$ 不是原语时，解。我们在此不承诺寻求当右侧任意调节函数时进入的补充可能性条件。

### 习题{#fvr-iv-s2-exercises}

参见[习题为 § 2](exercises/s2/)。

[^1]: 回想一下，如果 $E$ 为有限维，则从 $E$ 到自身的每个仿射线性映射都是连续的（*Gen. 顶部。*、VI、p. 33 和 37)。
