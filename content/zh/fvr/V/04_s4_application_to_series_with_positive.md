---
book: fvr
book_title: Functions of a Real Variable
chapter: V
chapter_title: LOCAL STUDY OF FUNCTIONS
section: 4
section_title: APPLICATION TO SERIES WITH POSITIVE TERMS
lang: zh
source: fvr-i-vii
book_pages: 236-246, 261-263
pdf_pages: 0251-0261, 0276-0278
extraction: ocr
subsections:
    - "no": 1
      title: CONVERGENCE CRITERIA FOR SERIES WITH POSITIVE TERMS
      page: 236
      pdf_page: 251
    - "no": 2
      title: ASYMPTOTIC EXPANSION OF THE PARTIAL SUMS OF A SERIES
      page: 238
      pdf_page: 253
    - "no": 3
      title: ASYMPTOTIC EXPANSION OF THE PARTIAL PRODUCTS OF AN INFINITE PRODUCT
      page: 243
      pdf_page: 258
    - "no": 4
      title: 'APPLICATION: CONVERGENCE CRITERIA OF THE SECOND KIND FOR SERIES WITH POSITIVE TERMS'
      page: 244
      pdf_page: 259
statements: 13
exercises: 11
content_sha256: b8f7197749bb4cd174ea6411f1d1f6d92a2b915d06679decd134b6434420b362
translated_from: content/en/fvr/V/04_s4_application_to_series_with_positive.md
translation_method: google
source_content_sha256: c18bf105a0a19fb75952b1cd2547b25be59f3bbcc6840083c077e38c89496107
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: ba4566d95c9d223ced903e0da8e7e0b259603c80d517beb8e7124fe560b661bc
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 4。适用于级数并具有正值项

### 1. 判据级数与正项收敛

在这个截面通过*级数和积极的项*我们将理解（通过滥用语言）真正的项的级数$(u_n)$，使得$u_n \geq 0$*从n的某个特定*值开始。 Everything we shall say about such series will extend immediately by a change of sign to series all of whose terms are $\leq 0$ starting from some particular value of n. 我们已经看到（II，p. 64，例 3），对于规范化的空间 E 中点的每一个序列$(\mathbf{u}_n)_{n \geq 1}$，我们可以将$[1, +\infty[$上定义的步骤函数$\mathbf{u}$关联起来： 条件$\mathbf{u}(x) = \mathbf{u}_n$对于$n \leq x < n+1$：则级数$(\mathbf{u}_n)$收敛当且仅当积分$\int_1^{+\infty} \mathbf{u}(t)\,dt$收敛。

令$(u_n)$和$(v_n)$为两个级数且项为正数，并且$u$和$v$关联的步骤函数：关系$u_n \leq v_n$对于$n \geq n_0$相当于$u(x) \leq v(x)$对于$x \geq n_0$。因此，关系 $u_n \preccurlyeq v_n, u_n \ll v_n, u_n \sim v_n$分别相当于$u(x) \preccurlyeq v(x), u(x) \ll v(x)$和$u(x) \sim v(x)$；这个注允许我们翻译命题1（V，p. 228）和6（V，p. 230）如下：

#### 命题 1 {#fvr-v-s4-prop-1 .statement tag=08FZ}

*令*$(u_n)$*和*$(v_n)$*为两个级数且项为正。如果* $u_n \preccurlyeq v_n$ *且如果级数* $(v_n)$ *收敛，则* $(u_n)$ *收敛；如果* $u_n \succ v_n$ *并且如果* $\sum_{n=1}^{\infty} v_n = +\infty$，*则* $\sum_{n=1}^{\infty} u_n = +\infty$。

#### 命题 2 {#fvr-v-s4-prop-2 .statement tag=08G0}

*令* $(u_n)$ *和* $(v_n)$ *为两个级数且项*为正数：
1. *如果级数* $(v_n)$ *收敛，则关系* $u_n \ll v_n$ *（分别* $u_n \sim v_n$）*意味着* $\sum_{p=n}^{\infty} u_p \ll \sum_{p=n}^{\infty} v_p$ *（分别* $\sum_{p=n}^{\infty} u_p \sim \sum_{p=n}^{\infty} v_p$）。
2. *如果* $\sum_{n=1}^{\infty} v_n = +\infty$ *则关系* $u_n \ll v_n$ *（分别* $u_n \sim v_n$）*意味着* $\sum_{p=1}^{n} u_p \ll \sum_{p=1}^{n} v_p$ *（分别* $\sum_{p=1}^{n} u_p \sim \sum_{p=1}^{n} v_p$）。

通过在prop中进行比较级数$(v_n)$，可以方便地收敛判据。 1 级数，其项为形式$v_n = f(n)$，其中$f$为函数$\geq 0$，为区间$[x_0, +\infty[$上的每个实数$x > x_0$和递减定义；的确：

#### 命题 3（柯西-麦克劳林准则）{#fvr-v-s4-prop-3 .statement tag=08G1}

*如果* $f$ *是函数* $\geq 0$ *且递减在* $[x_0, +\infty[$上，*则级数与一般项* $v_n = f(n)$ *收敛当且仅当积分* $\int_{x_0}^{+\infty} f(t)\,dt$ *收敛*。

为了证明这一点，注是足够的，如果$v$是与级数$(v_n)$相关的步骤函数，那么对于每个$x \geq x_0$，$v(x+1) \leq f(x) \leq v(x)$是足够的，因为$f$是递减；因此，命题是比较原理的推论（II，p. 66，道具 3）。

由于函数具有积分（V、p. 229、属性 2、3 和 4）的对数收敛性判据的特征，因此在区间 $[x_0, +\infty[$、应用属性上为递减。 V、p. 237的1和3给出以下判据：

#### 命题 4（“阶 0 的对数准则”）{#fvr-v-s4-prop-4 .statement tag=08G2}

设$(u_n)$为级数，且项为正；如果$u_n \preccurlyeq n^\mu$对于某些$\mu < -1$则级数$(u_n)$收敛；如果$u_n \succcurlyeq n^\mu$对于某些$\mu \geq -1$，则级数$(u_n)$有一个无限的和。

#### 命题 5（“阶 $p$ 的对数标准”）{#fvr-v-s4-prop-5 .statement tag=08G3}

令 $(u_n)$ 为级数，项为正值。如果$u_n \preccurlyeq \frac{1}{nl_1(n)l_2(n)\ldots l_{p-1}(n)(l_p(n))^\mu}$对于某些$\mu > 1$则级数$(u_n)$收敛；如果 $u_n \succcurlyeq \frac{1}{nl_1(n)l_2(n)\ldots l_{p-1}(n)(l_p(n))^\mu}$ 对于某些 $\mu \leq 1$ 那么级数 $(u_n)$ 有一个无限的和。

如果 $0 \leq q < 1$ 对于任何 $\mu > 0$ 都有 $q^n \preccurlyeq n^{-\mu}$； 应用阶 0 的对数准则再次证明了级数$\sum_{n=0}^\infty q^n$对于$|q| < 1$的收敛性（Gen. Top.、IV、p. 364）。如果有人应用道具。 1 与 $v_n = q^n$ 得到一个准则，该准则可放入以下形式（“柯西准则”）中： *令 $(u_n)$ 为级数，项为正；如果$\limsup_{n \to \infty}(u_n)^{1/n} < 1$则级数$(u_n)$收敛；如果 $\limsup_{n \to \infty}(u_n)^{1/n} > 1$ 则级数 $(u_n)$ 有无限和。* 事实上，如果 $\limsup_{n \to \infty}(u_n)^{1/n} = a < 1$ 那么 $u_n \preccurlyeq q^n$ 对于每个 $q$ 使得 $a < q < 1$。另一方面，如果$\limsup_{n \to \infty}(u_n)^{1/n} = a > 1$则$u_n \succcurlyeq q^n > 1$对于$n$的无限多个值，对于任何$q$使得$1 < q < a$；因为 $u_n$ 不趋于 0，所以有 $\sum_{n=1}^\infty u_n = +\infty$。

这个准则在*整个级数*理论中非常有用，我们稍后会研究；但即便如此，它也不允许人们决定级数$(1/n^\alpha)$的收敛性，在其他字中，它的域的应用比对数判据的限制要大得多。

### 2. 级数部分和的渐近展开

对于趋于 $+\infty$ 的 $x$ 实数，令 $\mathscr{E}$ 为由函数形成的比较量表，其中每个量表均在*整个区间* $[x_0, +\infty[$（取决于函数）上定义，并且在此区间上为 $\geq 0$。令 $(\mathbf{u}_n)$ 为级数，其项属于为完全范数空间 $\mathbf{E}$，使得 $\mathbf{u}_n$ 相对于规模 $\mathscr{E}'$ 承认渐近展开至精度 $g_\alpha$ $\mathscr{E}$中函数的限制到$\mathbf{N}$：

$$
\mathbf{u}_n = \sum_{\lambda \leq \alpha} \mathbf{a}_\lambda g_\lambda(n) + \mathbf{r}_\alpha(n).
$$

假设每个部分和$\sum_{m=1}^n g(m)$，其中$g \in \mathscr{E}$，都承认相对于$\mathscr{E}'$渐近展开。然后可以获得 $s_n = \sum_{m=1}^n \mathbf{u}_m$ 相对于 $\mathscr{E}'$ 的渐近展开；我们再次区分两种情况：

1°$\sum_{n=1}^{\infty} g_{\alpha}(n) = +\infty$。那么 (V, p. 237, 命题 2) 有 $\sum_{m=1}^{n} r_{\alpha}(m) \ll \sum_{m=1}^{n} g_{\alpha}(m)$：
通过假设可以得到渐近展开
$$
\sum_{\lambda \leq \alpha} a_{\lambda} \left( \sum_{m=1}^{n} g(m) \right)
$$
(V, p. 222) 达到一定精度$g_{\sigma}$；如果$c g_{\sigma}(n)$是$\sum_{m=1}^{n} g_{\alpha}(m)$的主部分，则$s_{n}$的渐近展开精确到$g_{\min(\rho,\sigma)}$。

2°$\sum_{n=1}^{\infty} g_{\alpha}(n)$收敛；然后令$\beta$为指标$\lambda \leq \alpha$的最小的，使得$a_{\lambda} \neq 0$且$\sum_{n=1}^{\infty} g_{\lambda}(n)$收敛； 级数
$$
C = \sum_{n=1}^{\infty} \left( u_{n} - \sum_{\lambda < \beta} a_{\lambda} g_{\lambda}(n) \right)
$$
然后绝对收敛，可以写
$$
s_{n} = \sum_{\lambda < \beta} a_{\lambda} \left( \sum_{m=1}^{n} g_{\lambda}(m) \right) + C - \sum_{\beta \leq \lambda \leq \alpha} a_{\lambda} \left( \sum_{m=n+1}^{\infty} g_{\lambda}(m) \right) - \sum_{m=n+1}^{\infty} r_{\alpha}(m).
$$
此外，$\sum_{m=n+1}^{\infty} r_{\alpha}(m) \ll \sum_{m=n+1}^{\infty} g_{\alpha}(m)$；如果$c g_{\sigma}(n)$是$\sum_{m=n+1}^{\infty} g_{\alpha}(m)$的本金部分，
如果渐近展开为
$$
\sum_{\lambda < \beta} a_{\lambda} \left( \sum_{m=1}^{n} g_{\lambda}(m) \right) + C - \sum_{\beta \leq \lambda \leq \alpha} a_{\lambda} \left( \sum_{m=n+1}^{\infty} g_{\lambda}(m) \right)
$$
因而，对于精度$g_{\rho}$，我们可以得到$s_{n}$到精度$g_{\min(\rho,\sigma)}$的渐近展开。

因而，我们得出了级数 $(g(n))$ 其中 $g \in \mathscr{E}$ 的特殊情况。我们将看到，在满足一定的条件的条件下，如何立即获得$s_{n} = \sum_{m=1}^{n} g(m)$（当$\sum_{n=1}^{\infty} g(n) = +\infty$时）或$r_{n} = \sum_{m=n+1}^{\infty} g(m)$（当$\sum_{n=1}^{n} g(n) < +\infty$时）的本金部分。

#### 命题 6 {#fvr-v-s4-prop-6 .statement tag=08G4}

*设 g 为实数函数，> 0 并且单调，定义在区间 [x_0, +\infty[ （其中 x_0 \leq 1 ）上，并且 log g 和 x 与阶 1 相当。*

1° *如果 g 相对于 e* 无限阶，则有

$$
s_n = \sum_{m=1}^n g(m) \sim g(n) \qquad \text{if} \quad \sum_{n=1}^\infty g(n) = +\infty; \tag{1}
$$

$$
r_n = \sum_{m=n+1}^\infty g(m) \sim g(n+1) \qquad \text{if} \quad \sum_{n=1}^\infty g(n) < +\infty. \tag{2}
$$

2° *如果 g 相对于 $e^x$ 是有限的阶 $\mu$，则有*

$$
s_n = \sum_{m=1}^n g(m) \sim \frac{\mu}{1 - e^{-\mu}} \int_{\lambda_0}^n g(t) \, dt \qquad \text{if} \quad \sum_{n=1}^\infty g(n) = +\infty; \tag{3}
$$

$$
r_n = \sum_{m=n+1}^\infty g(m) \sim \frac{\mu}{1 - e^{-\mu}} \int_n^\infty g(t) \, dt \qquad \text{if} \quad \sum_{n=1}^\infty g(n) < +\infty \tag{4}
$$

（当$\mu = 0$时，（3）和（4）中数$\frac{\mu}{1 - e^{-\mu}}$替换为1）。

1° 如果 g 相对于 $e^x$ 为阶 $+\infty$，则有 $\log g \gg x$ 从而 $g'/g \gg 1$，或 $g' \gg g$，除以假设；因而，g 为递增，并且趋向于 $+\infty$，其中 $x$、从而 $\sum_{n=1}^\infty g(n) = +\infty$。如果$u$是与级数$(g(n))$（V，p. 237）相关联的步骤函数，则从$x$的某个值开始有$u(x) \leq g(x)$，因而$u \ll g$，因而

$$
s_{n-1} = \int_1^n u(t) \, dt \ll \int_1^n g(t) \, dt \ll \int_1^n g'(t) \, dt \sim g(n);
$$

因为$s_n = s_{n-1} + g(n)$一个人有$s_n \sim g(n)$。当g相对于$e^x$为阶$-\infty$时，证明类似；由此我们得到公式 (2)。

2° 如果 g 相对于 $e^x$ 是有限的阶 $\mu$，则可以写成 $g(x) = e^{\mu x} h(x)$，其中 h 相对于 $e^x$ 是阶 0；此外，通过假设，$\log g \sim \mu x$代表$\mu \neq 0$（$\log g \ll x$代表$\mu = 0$）意味着$h' \ll h$。首先假设$\sum_{n=1}^\infty g(n) = +\infty$（这意味着如果$\mu > 0$，$\mu \geq 0$；逆命题总是成立，从那时起$g(x)$趋向于$+\infty$和$x$）；让我们评估 $\int_{n-1}^n g(t) \, dt$ 的本金部分。一个人可以写

$$
\int_{n-1}^n g(t) \, dt = \int_{n-1}^n e^{\mu t} h(t) \, dt
$$
$$
= h(n) \int_{n-1}^n e^{\mu t} \, dt + \int_{n-1}^n e^{\mu t} (h(t) - h(n)) \, dt
$$
$$
= \frac{1 - e^{-\mu}}{\mu} g(n) + \int_{n-1}^n e^{\mu t} (h(t) - h(n)) \, dt.
$$

现在，关系$h' \ll h$意味着对于每个$\varepsilon > 0$都有一个$n_0$，这样关系$x \geq n_0$意味着$|h'(x)/h(x)| \leq \varepsilon$；从值定理的平均值推断出 $-\varepsilon \leq \log |h(t)/h(n)| \leq \varepsilon$，对于 $n-1 \leq t \leq n$，如果 $n \geq n_0$，从而

$$
|h(t) - h(n)| \leq (e^\varepsilon - 1)h(n)
$$

因而

$$
\left| \int_{n-1}^n e^{\mu t} (h(t) - h(n)) \, dt \right| \leq (e^\varepsilon - 1)e^{\mu n}h(n) = (e^\varepsilon - 1)g(n)
$$

因为$e^{\mu t}$是递增。由于$e^\varepsilon - 1$随着$\varepsilon$变得任意小，我们可以看到可以写

$$
\int_{n-1}^n g(t) \, dt = \frac{1 - e^{-\mu}}{\mu} g(n) + o(g(n))
$$

$\left( \frac{1 - e^{-\mu}}{\mu} \text{ being replaced by } 1 \text{ when } \mu = 0 \right)$。 命题就是 prop 的推论。 2 个V、p. 237。当 $\sum_{n=1}^\infty g(n)$ 有限时，人们也会提出类似的观点。

通过应用道具。 V、p. 239中的6个，重复有时就可以得到$s_n = \sum_{m=1}^n g(m)$的*渐近展开*。首先假设$g$相对于$e^\lambda$有阶$+\infty$；对于 $p$ 的每个*固定* 值，可以通过 prop 来写。 6、

$$
s_n = g(n) + g(n-1) + \cdots + g(n-p) + o(g(n-p))
$$

并且只需扩展（相对于$\mathscr{E}'$）函数和$g(n-k)$（$0 \leq k \leq p$）中的每一个，将展开的精度限制为$g(n-p)$的主部分，即可获得$s_n$的展开。

#### 例 {#fvr-v-s4-n2-exa-1 .statement tag=08G5}

让$g(x) = x^\lambda = \exp(\lambda \log x)$，阶$+\infty$相对于$e^\lambda$。拿 $p = 2$ 一个有

$$
(n-1)\log(n-1) = (n-1)\log n - 1 + \frac{1}{2n} + o\left( \frac{1}{n} \right)
$$

从而（V、p. 225）

$$
(n-1)^{n-1} = \frac{1}{e} n^{n-1} + \frac{1}{2e} n^{n-2} + o_1\left( n^{n-2} \right)
$$

和类似地

$$
(n-2)^{n-2} = \frac{1}{e^2} n^{n-2} + o_2\left( n^{n-2} \right);
$$

因而

$$
s_n = n^n + \frac{1}{e} n^{n-1} + \left( \frac{1}{2e} + \frac{1}{e^2} \right) n^{n-2} + o_3\left( n^{n-2} \right).
$$

当 $g$ 相对于 $e^\lambda$ 为阶 $-\infty$ 时，可进行类似的处理（对于 $r_n$）。

现在，如果$g$相对于$e^x$是有限的阶$\mu$，并且如果对于例，$\sum_{n=1}^\infty g(n) = +\infty$，可以写
$$
s_n = \frac{\mu}{1 - e^{-\mu}} \int_1^n g(t)\, dt + \sum_{m=1}^n f_1(m)
$$
其中 $f_1(n) = g(n) - \frac{\mu}{1 - e^{-\mu}} \int_1^n g(t)\, dt \ll g(n)$ 由道具决定。 6 个V、p. 239。如果一个人的本金部分$c g_1(n)$相对于$f_1(n)$相对于$\mathscr{E}'$，并且如果一个人可以再次应用道具。 6 到函数 $g_1$ 如果$\sum_{n=1}^\infty g_1(n) = +\infty$，则将获得相当于$\sum_{m=1}^n f_1(m)$的原语，在相反情况下相当于$\sum_{m=n+1}^\infty f_1(m)$（在后一种情况下，我们写为$\sum_{m=1}^n f_1(m) = C - \sum_{m=n+1}^\infty f_1(m)$，带有$C = \sum_{n=1}^\infty f_1(n)$）。

因此，一步一步地，我们最终可以得到$s_n$的表达式，即某个数基元的和，每个基元相对于前一个基元都可以忽略不计，项相对于最后写入的基元仍然可以忽略不计，最后是一个常数（余数项趋于0的情况）。然后剩下的就是扩展关于$\mathscr{E}'$（cf.V，p. 235）获得的每个基元。

#### 例 {#fvr-v-s4-n2-exa-2 .statement tag=08G6}

设 $g(n) = \frac{1}{n}$；然后
$$
s_n = \sum_{m=1}^n \frac{1}{m} \sim \int_1^n \frac{dt}{t} = \log n
$$
然后
$$
\frac{1}{n} - (\log n - \log(n-1)) \sim -\frac{1}{2n^2}
$$
从而
$$
s_n = \log n + \gamma + \frac{1}{2n} + o\left(\frac{1}{n}\right).
$$
公式中出现的常数$\gamma$在数学分析（cf.章节VI和VII）中起着重要作用；它被称为*欧拉常数*；一个有
$$
\gamma = 0.577\,215\,664\ldots
$$
到$1/10^9$以内。

我们将在VI、p. 288中看到，在最重要的情况下，*欧拉-麦克劳林求和公式*如何针对$s_n$（或$r_n$）给出*任意*阶的渐近展开。

### 3.无穷乘积的部分积的渐近展开

人们知道（Gen. Top.，V。p. 22和23），对于无限乘积与一般因子$1 + u_n$（$u_n > -1$）收敛（或可交换收敛），级数与一般级数是必要且充分的项 $\log(1 + u_n)$ 应该收敛（或交换收敛），那么就有关系

$$
\log \prod_{n=1}^{\infty} (1 + u_n) = \sum_{n=1}^{\infty} \log(1 + u_n).
$$

当无穷大乘积收敛时，我们知道$u_n$趋于0；因此$\log(1 + u_n) \sim u_n$；现在我们知道，要使实数的级数交换收敛，它绝对收敛是必要且充分的（Gen. Top., IV, p. 372, 命题 5）；通过道具。 1 因此恢复了这样一个事实：乘积与一般因子$1 + u_n$是可交换收敛的当且仅当级数与一般项$u_n$绝对收敛（Gen.Top.，IV，p. 368，th.1）。 4）。

类似的论证适用于无限乘积，其一般因子为复数 $1 + u_n$ ($u_n \neq -1$)。事实上，对于这样的乘积是可交换收敛的，它是必要且充分的（Gen. Top.，VIII，p. 115，道具 2），具有一般因子 $|1 + u_n|$ 的无限乘积应该如此，并且进一步，如果 $\theta_n$ 是$1 + u_n$（在$-\pi$和$+\pi$之间取），$\theta_n$的级数应该是可交换收敛的。由于$u_n$趋于0，$\log(1 + u_n)$是从$n$（III，p. 100）的某个特定值开始定义的，并且有

$$
\log(1 + u_n) = \log |1 + u_n| + i \theta_n;
$$

因此，要使乘积与广义因子 $1 + u_n$ 交换收敛，级数与广义项 $|\log(1 + u_n)|$ 绝对收敛是必要且充分的（Gen Top., VII, p. 84, th. 1）；现在$\log(1 + u_n) \sim u_n$（I，p. 18，道具5），因此再次获得条件，级数与一般项$u_n$应该绝对收敛（Gen.Top.，VIII，p. 116，th.） 1）。

实数有时的无限乘积和级数之间的关系允许获得部分乘积$p_n = \prod_{k=1}^{n} (1 + u_k)$的渐近展开；对于部分和 $s_n = \sum_{k=1}^{n} \log(1 + u_k)$ 有一个渐近展开就足够了，然后展开 $p_n = \exp(s_n)$；因此，一个被带回到之前检查的两个问题（V，p. 238和p. 226）。

#### 例 {#fvr-v-s4-n3-exa-1 .statement tag=08G7}

*斯特林的公式。*让我们寻找$n!$的渐近展开；这导致我们扩展$s_n = \sum_{p=1}^{n} \log p$，然后扩展$\exp(s_n)$。 n 2 的方法依次给出

$$
s_n = \sum_{p=1}^{n} \log p \sim \int_{1}^{n} \log t \, dt = n \log n - n + 1
$$

然后
$$
\log n - \int_{n-1}^{n} \log t \, dt = \log n - (n \log n - (n-1) \log(n-1) - 1) \sim \frac{1}{2n}
$$
从而
$$
s_n = n \log n - n + \frac{1}{2} \log n + o(\log n).
$$
然后
$$
\log n - \int_{n-1}^{n} \log t \, dt - \frac{1}{2} (\log n - \log(n-1)) \sim -\frac{1}{12n^2}
$$
从而
$$
s_n = n \log n - n + \frac{1}{2} \log n + k + \frac{1}{12n} + o_1 \left( \frac{1}{n} \right) \quad (k \text{ constant})
$$
最终推导出 (V, p. 226)
$$
n! = e^k \, n^{n+1/2} \, e^{-n} \left( 1 + \frac{1}{12n} + o_2 \left( \frac{1}{n} \right) \right). \tag{5}
$$
我们将在VII、p. 322、$e^k = \sqrt{2\pi}$中展示。 公式 (5)（与$k$的值）称为*斯特林的公式*。同样地，对于每一个实数 $a$ 而不是整数 $> 0$，都表明
$$
(a+1)(a+2)\ldots(a+n) \sim K(a) \, n^{n+a+\frac{1}{2}} \, e^{-n}. \tag{6}
$$
我们也将确定函数$K(a)$（VII，p. 18）。从公式 (5) 和 (6) 特别可以得出：
$$
\binom{a}{n} \sim (-1)^n \varphi(a) \, n^{-a-1} \tag{7}
$$
对于每个实数$a$而不是整数$> 0$，其中$\varphi(a)$是$a$的函数，这将在VII，p. 322中指定。

### 4. 应用：级数与正项的第二类收敛判据

人们经常遇到级数$(u_n)$，其中$u_n > 0$从某个点开始，并且$u_{n+1}/u_n$有一个渐近展开，很容易得到确定。对于这样的级数，有判据（称为第二类*判据*）是很方便的，允许人们知道确定级数是否单独从$u_{n+1}/u_n$的形式收敛。以下是这样一个标准：

#### 命题 7（“拉贝测试”）{#fvr-v-s4-prop-7 .statement tag=08G8}

*令$(u_n)$为级数，从点开始为项$> 0$。如果从某个阶段开始，$u_{n+1}/u_n \leqslant 1 - \frac{\alpha}{n}$对于某些$\alpha > 1$，则级数$(u_n)$收敛；如果从某个点开始，$u_{n+1}/u_n \geqslant 1 - \frac{1}{n}$，那么级数$(u_n)$有无限和。*

事实上，如果$u_{n+1}/u_n \leqslant 1 - \frac{\alpha}{n}$和$\alpha > 1$，对于所有$n \geqslant n_0$，那么就有$u_n \preccurlyeq p_n = \prod_{k=n_0}^{n} \left( 1 - \frac{\alpha}{k} \right)$。现在，$\log \left( 1 - \frac{\alpha}{n} \right) = -\frac{\alpha}{n} - \frac{\alpha^2}{2n^2} + o \left( \frac{1}{n^2} \right)$、从而 $\log p_n =$ $-\alpha \log n + k + o(1/n)$（$k$常数）和$p_n \sim e^k \frac{1}{n^\alpha}$；因为 $\alpha > 1$ 阶 0 的对数标准允许 1 完成。

另一方面，如果$u_{n+1}/u_n \geq 1 - \frac{1}{n}$来自某个点，则相同的计算证明$u_n \geq \frac{1}{n}$，从而命题。

以同样的方式求一个可以证明，使用阶$> 0$的对数判据，第二类判据如下：

#### 命题 8 {#fvr-v-s4-prop-8 .statement tag=08G9}

*令$(u_n)$为级数，从某个点开始，项$> 0$。如果从某个点开始，有*

$$
\frac{u_{n+1}}{u_n} \leq 1 - \frac{1}{n} - \frac{1}{nl_1(n)} - \ldots - \frac{1}{nl_1(n)l_2(n)\ldots l_{p-1}(n)} - \frac{\alpha}{nl_1(n)l_2(n)\ldots l_p(n)}
$$

*对于某些$\alpha > 1$，则级数$(u_n)$收敛；如果，从某个点开始，一个人有*

$$
\frac{u_{n+1}}{u_n} \geq 1 - \frac{1}{n} - \frac{1}{nl_1(n)} - \ldots - \frac{1}{nl_1(n)l_2(n)\ldots l_p(n)}
$$

*那么级数$(u_n)$有一个无限的和。*

#### 例 {#fvr-v-s4-n4-exa-1 .statement tag=08GA}

考虑*超几何级数*，以及一般的项

$$
u_n = \frac{\alpha(\alpha+1)\ldots(\alpha+n-1)\,\beta(\beta+1)\ldots(\beta+n-1)}{1.2\ldots n.\gamma(\gamma+1)\ldots(\gamma+n-1)}
$$

其中$\alpha, \beta, \gamma$是任意的实数，而不是整数$\leq 0$：很明显，$u_n$从某个阶段开始是$> 0$，或者从某个阶段开始是$< 0$。一个有

$$
\begin{align*}
\frac{u_{n+1}}{u_n} &= \frac{(\alpha+n)(\beta+n)}{(n+1)(\gamma+n)} \\
&= \left(1 + \frac{\alpha+\beta}{n} + \frac{\alpha\beta}{n^2}\right) \left(1 + \frac{\gamma+1}{n} + \frac{\gamma}{n^2}\right)^{-1} \\
&= 1 + \frac{\alpha+\beta-\gamma-1}{n} \\
&\quad + \frac{\alpha\beta-(\alpha+\beta)(\gamma+1)+\gamma^2+\gamma+1}{n^2} + o\left(\frac{1}{n^2}\right).
\end{align*}
$$

拉贝检验表明，对于$\alpha + \beta < \gamma$，级数收敛，对于$\alpha + \beta > \gamma$，和无穷大；当$\alpha + \beta = \gamma$级数也有一个无限的和时，如prop所示。 8.

#### 注 1 {#fvr-v-s4-n4-rem-1 .statement tag=08GB}

作为拉贝测试的一个特定实例，我们可以看到，如果 $\limsup_{n \to \infty} u_{n+1}/u_n < 1$ 级数 $(u_n)$ 收敛；另一方面，如果 $\liminf_{n \to \infty} u_{n+1}/u_n > 1$、级数 $(u_n)$ 具有无限的和（*达朗贝尔测试*）。

#### 注 2 {#fvr-v-s4-n4-rem-2 .statement tag=08GC}

第二类判据只能应用于级数，其一般项表现得非常有规律，因为$n$趋向于$+\infty$；在其他字中，它们的范围比对数判据的范围受到更多限制，并且尝试在它们特别适合的特殊情况之外使用它们将是一个错误。对于例，对于由$u_{2m} = 2^{-m}$、$u_{2m+1} = 3^{-m}$定义的级数、$(u_n)$，有$u_{2m+1}/u_{2m} = \left(\frac{2}{3}\right)^m$、$u_{2m+2}/u_{2m+1} = \frac{1}{2} \left(\frac{3}{2}\right)^m$；随着 $m$ 无限增加，第一个比率趋向于 0，第二个比率趋向于 $+\infty$，因此第二类标准不适用；然而，从$u_n \preccurlyeq 2^{-n/2}$开始，级数收敛于直接的。

即使$u_{n+1}/u_n$有一个简单的表达式，右$u_n$的主体部分直接求值通常会像第二种判据一样快速地得出结果。对于例，对于超几何级数，斯特林的公式立即显示$u_n \sim a n^{\alpha + \beta - \gamma - 1}$，其中$a$是常数$\neq 0$，然后适用阶0的对数准则。

### 习题 {#fvr-v-s4-exercises}

§ 4](exercises/s4/)参见[习题。
