---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 1
section_title: GENERALIZED TAYLOR EXPANSIONS
lang: zh
source: fvr-i-vii
book_pages: 269-283, 291-292
pdf_pages: 0284-0298, 0306-0307
extraction: ocr
subsections:
    - "no": 1
      title: COMPOSITION OPERATORS ON AN ALGEBRA OF POLYNOMIALS
      page: 269
      pdf_page: 284
    - "no": 2
      title: APPELL POLYNOMIALS ATTACHED TO A COMPOSITION OPERATOR
      page: 272
      pdf_page: 287
    - "no": 3
      title: GENERATING SERIES FOR THE APPELL POLYNOMIALS
      page: 274
      pdf_page: 289
    - "no": 4
      title: BERNOULLI POLYNOMIALS
      page: 275
      pdf_page: 290
    - "no": 5
      title: COMPOSITION OPERATORS ON FUNCTIONS OF A REAL VARIABLE
      page: 277
      pdf_page: 292
    - "no": 6
      title: INDICATRIX OF A COMPOSITION OPERATOR
      page: 278
      pdf_page: 293
    - "no": 7
      title: THE EULER-MACLAURIN SUMMATION FORMULA
      page: 282
      pdf_page: 297
statements: 21
exercises: 3
content_sha256: 22c860fd503cfbbb3fea49a0491d1db1d4f288ac83b4d84e97b95bc3376e48b8
translated_from: content/en/fvr/VI/01_s1_generalized_taylor_expansions.md
translation_method: google
source_content_sha256: 7b62ad591ac33887b2cec9de99a553da0d73b1a05da4f701901b379dc016e8a0
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-50f48bb3
glossary_version: 34
glossary_terms_sha256: 00ff201d7c0e826897d147f22207c94c8c4121685cdde7b9e2eabcde2877f8b2
prompt_sha256: 77d1eb2d7fcbd90aea4f1a996022f1b3908ace921dc0bfaa5df62ffc2d1f67a6
---

## § 1。广义泰勒展开

### 1. 多项式代数的合成运算符

设 K 为特征 0 的交换域，K 上的一个不定多项式的 K[X] 代数（代数，IV.1）；在整个截面中，通过K[X]上的运算符，我们意味着向量空间K[X]（在K上）的线性映射U自身；因为对于这个空间，单项式 $X^n \ (n \geqslant 0)$ 形式基，U 由多项式 $U(X^n)$ 确定；具体来说，如果 $f(X) = \sum_{k=0}^\infty \lambda_k X^k$ 与 $\lambda_k \in K$，则
$$
U(f) = \sum_{k=0}^\infty \lambda_k U(X^k).
$$
如果G在K上是交换代数，且单位元素，则G模G[X]是通过将向量空间K[X]的标量K的域扩展到G得到的； K[X] 扩展上的每个算子 U 以独特的方式与 G 模 G[X] 自身的线性映射相关，我们再次用 U 表示（Alg., II, p. 278）；对于每个元素 $g(X) = \sum_{k=0}^\infty \gamma_k X^k$，加上 $\gamma_k \in G$，就有 $U(g) = \sum_{k=0}^\infty \gamma_k U(X^k)$。

特别考虑 G = K[Y] 的情况；那么 G[X] 是 K 上两个不定式多项式的环 K[X,Y]；为了避免混淆，我们用 $U_X$ 表示 U 到 G[X] 的扩张。对于任何多项式 $g(X, Y) = \sum_{k=0}^\infty \gamma_k(Y) X^k$ 其中 $\gamma_k(Y) \in K[Y]$ 因此有 $U_X(g) = \sum_{k=0}^\infty \gamma_k(Y) U(X^k)$。由于 $U_X$ 是线性的，所以如果写出 $g(X, Y) = \sum_{h=0}^\infty \beta_h(X) Y^h$，那么也有 $U_X(g) = \sum_{h=0}^\infty U(\beta_h) Y^h$。

在K[X]的典范同构到K[Y]上，将Y与X运算符U变换关联到K[Y]上的运算符，我们将其表示为$U_Y$，以避免混淆，因此$U_Y(f(Y))$是Y在替换X获得的多项式多项式$U(f(X)) = U_X(f(X))$。这个运算符 $U_Y$ 又可以扩展到 K[X,Y] 上的运算符（再次用 $U_Y$ 表示）： if $g(X, Y) = \sum_{h=0}^\infty \beta_h(X) Y^h$ then
$$
U_Y(g(X, Y)) = \sum_{h=0}^\infty \beta_h(X) U_Y(Y^h).
$$

作为这些扩张中的例，我们引用K[X]上的推导运算符D（算法，IV.6），它给出了K[X,Y]上的部分推导运算符D_X和D_Y。

对于任何多项式 $f \in K[X]$，我们用 $T_Y(f)$ 表示 K[X,Y] 中的多项式 $f(X + Y)$； 映射 $T_Y$ 是从 K[X] 到 K[X,Y] 的 K 线性映射，称为平移算子。

#### 定义 1 {#fvr-vi-s1-def-1 .statement tag=08HO}

*有人说K[X]上的算子U是合成算子，如果它与平移算子可交换，即如果$U_X T_Y = T_Y U$。*

在其他字中，如果$f$是K[X]中的任意多项式，并且如果$g = U(f)$，则必须有$g(X + Y) = U_X(f(X + Y))$。

从定义可以立即得出，对于每个多项式$f(X) \in K[X]$，在上面的记号中，

$$
U_X(f(X + Y)) = U_Y(f(X + Y)).
$$

(1)

#### 例 1 {#fvr-vi-s1-n1-exa-1 .statement tag=08HP}

对于每个$\lambda \in K$，与每个多项式$f(X)$关联多项式$f(X + \lambda)$的运算符是合成运算符。

#### 例 2 {#fvr-vi-s1-n1-exa-2 .statement tag=08HQ}

K[X] 上的推导 D 是合成运算符（*cf.* 命题 1）。

#### 注 {#fvr-vi-s1-n1-rem-1 .statement tag=08HR}

由于 K 是无限域，所以 K[X] 上的算子 U 是合成算子当且仅当对于每个多项式 $f \in K[X]$ 和每个元素 $\alpha \in K$ 都有一个，将 $g = U(f)$ 放入 $g(X + \alpha) = U(f(X + \alpha))$。 （阿尔格.，IV.16，更正）。

显然，合成算子中的每一个线性组合，其系数为K，都是合成算子；对于两个合成运算符中的合成也是如此。其它字、合成算子向量空间K[X]自同态代数形式子代数$\Gamma$。

#### 命题 1 {#fvr-vi-s1-prop-1 .statement tag=08HS}

*对于 K[X] 上的算子 U 成为合成算子，它与 K[X] 上的推导 D 交换是必要且充分的。*

事实上，泰勒公式表明，对于每个多项式$f \in K[X]$，有一个

$$
U_X(f(X + Y)) = U_X \left( \sum_{k=0}^{\infty} \frac{1}{k!} Y^k D^k f(X) \right) = \sum_{k=0}^{\infty} \frac{1}{k!} Y^k U(D^k f(X));
$$

如果有人放 $g = U(f)$ 那么有人有

$$
g(X + Y) = \sum_{k=0}^{\infty} \frac{1}{k!} Y^k D^k g(X) = \sum_{k=0}^{\infty} \frac{1}{k!} Y^k D^k (U(f(X)));
$$

为了使 U 成为合成运算符，对于每个整数 $k \geq 1$，尤其是 $UD = DU$，必须有 $UD^k = D^k U$。相反，如果关系成立，则意味着对于每个整数$k \geq 1$，归纳在$k$上有$UD^k = D^k U$；泰勒公式则表明$g(X + Y) = U_X(f(X + Y))$。

对于每个多项式 $f \in K[X, Y]$，我们用 $U_0(f)$ 项 *独立于* X 表示多项式 $U_X(f)$；特别是，如果$f \in K[X]$，$U_0(f)$是$U(f)$中的*常数项*，而$U_0$是$K[X]$上的*线性形式*。对于每个多项式 $f \in K[X]$ 让 $g = U(f)$；按定义。 1 个VI、p. 270

$$
g(X + Y) = U_X(f(X + Y)) = U_X \left( \sum_{k=0}^{\infty} \frac{1}{k!} X^k D^k f(Y) \right) = \sum_{k=0}^{\infty} \frac{1}{k!} U(X^k) D^k f(Y)
$$

如果在这个公式中，1个替换X除以0，则得到1

$$
g(Y) = \sum_{k=0}^{\infty} \frac{1}{k!} U_0(X^k) D^k f(Y).
$$

由此可见

$$
U(f(X)) = \sum_{k=0}^{\infty} \frac{1}{k!} \mu_k D^k f(X) \tag{2}
$$

其中 $\mu_k$ *是多项式* $U(X^k)$ 中的常数项。

这个公式完全显示了$\mu_k$确定合成运算符$U$；相反，如果 $(\mu_n)$ 是 K 的元素的*任意* 序列，则公式 (2) 定义是一个与 D 明显可交换的运算符 $U$，所以 (VI, p. 270, 命题 1) 是合成运算符。从现在开始我们在形式中写(2)

$$
U = \sum_{k=0}^{\infty} \frac{1}{k!} \mu_k D^k. \tag{3}
$$

这个公式可以用拓扑语言解释如下：如果考虑$K[X]$上的离散拓扑，以及$K[X]$的自同态的代数$\mathrm{End}(K[X])$上*简单*收敛的拓扑（*Gen.Top.*， X, p. 277), 级数与一般项 $\frac{1}{k!} \mu_k D^k$ 可交换收敛于$\mathrm{End}(K[X])$，并有和 $U$ (*Gen. Top.*, III, p. 269)。

公式 (3) 表明，对于 K (*Alg.*, IV.41) 上的一个不确定中的每个*形式级数* $u(S) = \sum_{k=0}^{\infty} \alpha_k S^k$，我们可以关联合成运算符$U = \sum_{k=0}^{\infty} \alpha_k D^k$，将来我们将用$u(D)$表示。这个注可以通过以下方式澄清：

#### 定理 1 {#fvr-vi-s1-thm-1 .statement tag=08HT}

*映射与每个正式的级数* $u(S) = \sum_{k=0}^{\infty} \alpha_k S^k$ *在一个不确定的过* K *关联合成运算符* $u(D) = \sum_{k=0}^{\infty} \alpha_k D^k$ *在* $K[X]$ *是代数* $K[[S]]$ *正式的同构级数到代数* $\Gamma$ *合成操作员。*

人们立即验证这个映射是同态。仍有待观察它是单射的，在其他字中，关系$\sum_{k=0}^{\infty} \alpha_k D^k = 0$意味着对于每个$k$都有$\alpha_k = 0$；现在$h! \alpha_h$就是应用$\sum_{k=0}^{\infty} \alpha_k D^k$到$X^h$、从而定理得到的多项式中的常数项。

#### 推论{#fvr-vi-s1-n1-cor-1 .statement tag=08HU}

*$K[X]$中合成运算符的代数$\Gamma$是可交换的。*

#### 例 {#fvr-vi-s1-n1-exa-3 .statement tag=08HV}

如果$U$是与每个多项式$f(X)$关联$f(X + \lambda)$（其中$\lambda \in K$）的运算符，则有$U_0(X^k) = \lambda^k$，因此$U = \sum_{k=0}^{\infty} \frac{1}{k!} (\lambda D)^k$。与$e^{\lambda}$（III，p. 105）的级数展开类比，我们将环中的正式级数$\sum_{n=0}^{\infty} \frac{1}{n!} S^n$写为$e^S$或$\exp(S)$ $K[[S]]$；所以可以写$U = e^{\lambda D}$。 替换域$K$乘以有理分式$K(Y)$的域，在这个论证中我们可以看到类似的，*翻译运算符*$T_Y$可以写成$e^{YD}$。

此外，在形式级数的环$K[[S, T]]$中，超过$K$的两个不定式中有一个

$$
(\exp S)(\exp T) = \sum_{p,q} \frac{S^p}{p!} \frac{T^q}{q!}
$$
$$
= \sum_{n=0}^{\infty} \frac{1}{n!} \left( \binom{n}{0} S^n + \binom{n}{1} S^{n-1} T + \cdots + \binom{n}{n} T^n \right)
$$
$$
= \exp(S + T)
$$

特别是
$$
(\exp S)(\exp(-S)) = 1
$$
这证明了我们引入的记号是正确的。

#### 学院{#fvr-vi-s1-n1-sch-1 .statement tag=08HW}

The isomorphism of the algebra $K[[S]]$ of formal series and the algebra $\Gamma$ of composition operators on $K[X]$ sometimes allows one to prove propositions on formal series most simply, by proving them for the corresponding composition operators (*cf.* VI, p. 274, prop. 6).

### 2. 附加到合成运算符的上诉多项式

给定合成运算符$U = \sum_{k=0}^{\infty} \alpha_k D^k \neq 0$，令$p$是整数$k$中最小的一个，使得$\alpha_k \neq 0$；我们可以说$p$是运算符$U$的*阶*。

#### 命题 2 {#fvr-vi-s1-prop-2 .statement tag=08HX}

阶 0 的每个合成运算符在 $\mathbf{K}[X]$ 上的合成运算符的代数 $\Gamma$ 中都是可逆的。

事实上，一个形式化的级数$\sum_{k=0}^{\infty} \alpha_k S^k$使得$\alpha_0 \neq 0$在环$\mathbf{K}[[S]]$中可逆（代数，IV.41）； 命题因此由 th 推出。 VI、p. 271 中的 1 个。

#### 命题 3 {#fvr-vi-s1-prop-3 .statement tag=08HY}

设$U$为阶$p$的合成运算符；然后 $U(f) = 0$ 对于次数 $< p$ 的每个多项式 $f$；对于次数$n \geq p$的每个多项式$f \neq 0$，$U(f)$是次数$n - p$的多项式$\neq 0$。

This is an immediate consequence of formula (2) of VI, p. 271 and of the definition of the order of $U$.

显然，阶 $p$ 的每个运算符 $U$ 都可以用唯一的方式写为 $U = D^p V = V D^p$，其中 $V$ 是阶 0 的运算符（因此可逆）。

#### 定义 2 {#fvr-vi-s1-def-2 .statement tag=08HZ}

设$U = D^p V$为$\mathbf{K}[X]$上阶$p$的合成算子。多项式 $u_n(X) = V^{-1}(X^n)$ 称为附加到算子 $U$ 的指标 $n$ 的阿佩尔多项式。

如果$V^{-1} = \sum_{k=0}^{\infty} \frac{1}{k!} \beta_k D^k$（与$\beta_0 \neq 0$）因此有
$$
u_n(X) = \sum_{k=0}^{n} \binom{n}{k} \beta_k X^{n-k}.
$$
(6)

验证 $u_n$ 是次数 $n$ 的多项式（命题 3）；进一步
$$
u_n(0) = \beta_n.
$$

#### 命题 4 {#fvr-vi-s1-prop-4 .statement tag=08I0}

Appell 多项式附加到 $U$ 满足关系
$$
\frac{d u_n}{d X} = n \, u_{n-1}
$$
(7)
$$
u_n(X + Y) = \sum_{k=0}^{n} \binom{n}{k} u_{n-k}(X) Y^k
$$
(8)
$$
U(u_n(X)) = \frac{n!}{(n-p)!} X^{n-p}.
$$
(9)

这些公式实际上分别相当于以下关系（考虑到定义2）：

$$
DV^{-1} = V^{-1}D \tag{10}
$$
$$
(\exp(YD_X))V_X^{-1} = V_X^{-1}\exp(YD_X) \tag{11}
$$
$$
UV^{-1} = D^p. \tag{12}
$$

#### 命题 5 {#fvr-vi-s1-prop-5 .statement tag=08I1}

*对于每个多项式$f \in K[X]$和阶$p$的每个合成运算符都有*

$$
f^{(p)}(X + Y) = \sum_{k=0}^{\infty} \frac{1}{k!} U \left( f^{(k)}(X) \right) u_k(Y) \tag{13}
$$
*（广义泰勒展开）*。

事实上，如果一个人放入 $U = D^p V = V D^p$ ，则有 (VI, p. 270, 公式 (1))

$$
V_X^{-1}(f(X + Y)) = V_Y^{-1}(f(X + Y)) = \sum_{k=0}^{\infty} \frac{1}{k!} f^{(k)}(X) u_k(Y) \tag{14}
$$
泰勒公式并通过定义。 VI、p. 273 中的 2 个；只需将运算符$U$应用于公式(14)的第一个和最后一个项即可获得(13)。

### 3. 生成的级数对于上诉多项式

令 E 为不定 S 中*形式级数* 的环，系数为多项式 $K[X]$ 的环 (*Alg.*, IV.41)；在正式级数$g(X, S) = \sum_{n=0}^{\infty} \alpha_n(X) S^n$的其他字、环中，其中$\alpha_n$属于至$K[X]$。对于$K[X]$上的每个运算符$U$，我们通过将$U_X(g(X, S)) = \sum_{n=0}^{\infty} U(\alpha_n) S^n$放入E的定义映射$U_X$自身。显然，E 是 S 中形式级数环 $K[[S]]$ 的模，系数为$K$；通过$K[X]$上$U$的线性，我们可以立即验证对于每个元素$\theta \in K[[S]]$和每个$g \in E$都有$U_X(\theta g) = \theta U_X(g)$；在其他字中，$U_X$是模E自身的线性映射。

#### 命题 6 {#fvr-vi-s1-prop-6 .statement tag=08I2}

*令$U = D^p V = u(D)$为$K[X]$上阶$p$的合成运算符，$u(S)$为$K[[S]]$中阶$p$的正式幂级数。然后*

$$
U_X \left( \exp(XS) \right) = u(S) \exp(XS) \tag{15}
$$
$$
\frac{S^p}{u(S)} \exp(XS) = \sum_{n=0}^{\infty} \frac{1}{n!} u_n(X) S^n \tag{16}
$$
*n 是附加到 U* 的指标 n 的阿佩尔多项式。

由学校到th。 1 (VI, p. 271)，建立 (15) 足以表明对于每个多项式 $f(Y) \in K[Y]$ 有一个

$$
U_X \left( \exp(XD_Y)(f(Y)) \right) = u(D_Y)(\exp(XD_Y)(f(Y))).
$$

现在(17)中的第一个项是$U_X(f(X + Y))$，并且由于$U = u(D)$，(17)中的第二个项是$U_Y(f(X + Y))$，所以恒等式(17)约化到(1)(VI，p. 270)。

现在只需将（15）应用于合成运算符$V^{-1} = D^p / u(D)$即可获得（16），因为到定义，我们已经

$$
V^{-1}(\exp(XS)) = \sum_{n=0}^{\infty} \frac{1}{n!} u_n(X) S^n.
$$

注 (16) 也可以通过将形式级数 $S^p / u(S)$ 与 $\exp(XS)$ 相乘，并考虑 (6) 来获得。

有人说，形式级数 (16) 是附加到 $U$ 的阿佩尔多项式的生成的级数。

### 4. 伯努利多项式

考虑合成运算符 $U$ 定义为

$$
U(f(X)) = f(X + 1) - f(X);
$$

可以写 $U = e^D - 1$ (VI, p. 270, 例 1);这是阶 1 的运算符，如果有人放入 $U = DV$，则有 $V^{-1} = \frac{D}{e^D - 1}$。 次数 $n$ 相应的对算子$U$的阿佩尔多项式称为次数 $n$的伯努利多项式，记为$B_n(X)$；如果一个人放 $b_n = B_n(0)$ 一个人放公式

$$
B_n(X) = \sum_{k=0}^{n} \binom{n}{k} b_{n-k} X^k
$$
(18)

$$
\frac{S \, e^{XS}}{e^S - 1} = \sum_{n=0}^{\infty} \frac{1}{n!} B_n(X) S^n
$$
(19)

特别是

$$
\frac{S}{e^S - 1} = \sum_{n=0}^{\infty} \frac{1}{n!} b_n S^n
$$
(20)

VI、p. 273的公式 (7) 和 (9)，对于伯努利多项式，给出关系

$$
\frac{dB_n}{dX} = n B_{n-1}(X)
$$
(21)

$$
B_n(X + 1) - B_n(X) = n X^{n-1}.
$$
(22)

特别是，对于$n > 1$有$B_n(1) - B_n(0) = 0$，考虑到(18)，给出归纳关系

$$
\sum_{m=0}^{n-1} \binom{n}{m} b_m = 0 \quad \text{(for } n > 1)
$$

这使得人们能够一步一步地从计算到 $b_n$。这些数显然是*有理的*；因为一个人可以写

$$
\frac{S}{e^S - 1} = -\frac{S}{2} + \frac{S}{2} \frac{e^S + 1}{e^S - 1}
$$

自 (VI, p. 272, 公式 (5))

$$
\frac{e^{-S} + 1}{e^{-S} - 1} = -\frac{e^S + 1}{e^S - 1}
$$

我们可以看到，在 $\frac{S}{2} \frac{e^S + 1}{e^S - 1}$ 的形式级数中，*奇数* 次数的所有项都有系数零；所以有人有

$$
b_0 = 1, \qquad b_1 = -\frac{1}{2}, \qquad b_{2n-1} = 0 \quad \text{for } n > 1.
$$

有理数数 $b_{2n}$ ($n \geq 1$) 称为 *伯努利数*；我们将看到 (VI, p. 288) $b_{2n}$ 有$(-1)^{n-1}$ 的符号。对于 $n$ 的第一个值，公式 (23) 给出，

$$
\begin{align*}
b_2 &= \frac{1}{6}, & b_4 &= -\frac{1}{30}, & b_6 &= \frac{1}{42}, & b_8 &= -\frac{1}{30}, \\
b_{10} &= \frac{5}{66}, & b_{12} &= -\frac{691}{2730}, & b_{14} &= \frac{7}{6}, \\
b_{16} &= -\frac{3617}{510}, & b_{18} &= \frac{43867}{798}, & b_{20} &= -\frac{174611}{330}, & b_{22} &= \frac{854513}{138}, \\
b_{24} &= -\frac{236364091}{2730}, & b_{26} &= \frac{8553103}{6}, & b_{28} &= -\frac{23749461029}{870}.
\end{align*}
$$

注分子 691、3617、43867 是素数；其他的质因数分解是

$$
\begin{align*}
174611 &= 283 \times 617 \\
854513 &= 11 \times 131 \times 593 \\
236364091 &= 103 \times 2294797 \\
8553103 &= 13 \times 657931 \\
23749461029 &= 7 \times 9349 \times 362903.
\end{align*}
$$

由此我们推导出第一个伯努利多项式的表达式

$$
\begin{align*}
B_0(X) &= 1, & B_1(X) &= X - \frac{1}{2}, & B_2(X) &= X^2 - X + \frac{1}{6}, \\
B_3(X) &= X^3 - \frac{3}{2}X^2 + \frac{1}{2}X, & B_4(X) &= X^4 - 2X^3 + X^2 - \frac{1}{30}.
\end{align*}
$$

### 5. 实变量函数的合成运算符

令I为$\mathbf{R}$包含区间$\mathbf{R}_+ = [0, +\infty[$中的一个区间；令 E 为向量空间超过域 $\mathbf{C}$，由具有复数值的实数变量函数组成，在 I 上定义。我们假设对于每个$a \geqslant 0$和每个函数$f \in E$函数$x \mapsto f(x + a)$属于到E；此外，我们假设*具有复系数*的多项式*和*指数*$e^{\lambda x}$的E包含限制到I，其中$\lambda$是任意*复数*数。 E 的任何线性映射 $U$ 到所有映射的空间从 I 到域 $\mathbf{C}$ 的复数将被称为 E 上的*运算符*；如果$f \in E$和$g = U(f)$使用记号会很方便

$$
g(x) = U_{\xi}^{\xi}(f(\xi))
$$

其中 $\xi$ 是右侧项 (*cf.* II, p. 58) 函数符号中的*虚拟*变量。对于每个$a \geqslant 0$，将函数$f \in E$关联到限制到函数$x \mapsto f(x + a)$的I的运算符被a*称为*平移运算符。

#### 定义 3 {#fvr-vi-s1-def-3 .statement tag=08I3}

*有人说，E 上的运算符 U 是合成运算符，如果对于每个$a \geqslant 0$，它可以通过 a* 与平移运算符进行置换。

上面介绍的记号中，这个定义就成为恒等式

$$
U_{x+a}^{\xi}(f(\xi)) = U_x^{\xi}(f(\xi + a))
$$

在 $x$ 和 $a$ ($x \in I, a \geqslant 0$)。可以交换该恒等式中$x$和$a$的角色，如果$x \geqslant 0$，则放入$a = 0$；由此获得 $x \geqslant 0$

$$
U_x^{\xi}(f(\xi)) = U_0^{\xi}(f(\xi + x))
$$

其中$U_0$是E上的*线性形式*，它与每个函数$f \in E$关联$g = U(f)$的值$g(0)$。

如果$f$是多项式，则有$f(\xi + x) = \sum_{k=0}^{\infty} \frac{1}{k!} f^{(k)}(\xi) x^k$，公式(26)表明$U(f)$也是多项式；限制为$x$多项式的集合，系数为$\mathbf{C}$，（集合其中一个可以确定与代数$\mathbf{C}[X]$），运算符$U$则为def意义上的合成运算符。 VI、p. 270中的I以及前面截面的所有结果都可以应用于它。

我们再次为附加到运算符 $U$ 的 Appell 多项式写为 $u_n$。对于多项式 (VI, p. 274, 公式 (13)) 的广义泰勒展开，有对应，对于更一般的函数，结果如下：

#### 定理 2 {#fvr-vi-s1-thm-2 .statement tag=08I4}

*设 f 为函数，承认 I 上的连续 $(n + 1)^{th}$ 导数，以及属于及其所有对 $1 \leq m \leq n$ 的导数 $f^{(m)}$，到 E。如果 U 是阶 $p \leq n$ 在 E 上的合成运算符有，对于 $x \geq 0$ 和 $h \geq 0$*

$$
f^{(p)}(x + h) = \sum_{m=0}^{n} \frac{1}{m!} u_m(x) U_h^\xi \left( f^{(m)}(\xi) \right) + R_n(x, h)
$$
(27)

与
$$
R_n(x, h) = -U_h^\xi \left( \int_0^{\xi - x - h} \frac{1}{n!} u_n(x + \eta) f^{(n+1)}(\xi - \eta) d\eta \right)
$$
(28)
*（广义泰勒展开）*。

考虑为所有 $\xi \in I$ 定义的积分 $\int_0^{\xi - x - h} \frac{1}{n!} u_n(x + \eta) f^{(n+1)}(\xi - \eta) d\eta$，
并通过阶$n + 1$的部分向公式申请积分（II，p. 59，公式（11））；考虑到关系
$$
u_n^{(k)} = n(n-1)\ldots(n-k+1)u_{n-k}
$$
由 (7) (VI, p. 273) 递归推导，可得
$$
\int_0^{\xi - x - h} \frac{1}{n!} u_n(x + \eta) f^{(n+1)}(\xi - \eta) d\eta
$$
$$
= \sum_{m=0}^{n} \frac{1}{m!} u_m(x) f^{(m)}(\xi) - \sum_{m=0}^{n} \frac{1}{m!} u_m(\xi - h) f^{(m)}(x + h).
$$
(29)

我们将运算符$U$应用于(29)的两侧，视为$\xi$的函数，然后取函数的值，这样得到变量$\xi$的值$h$；注意到，通过公式 (26) (VI, p. 277) 和 (9) (VI, p. 272)，有
$$
U_h^\xi (u_m(\xi - h)) = U_0^\xi (u_m(\xi)) = \begin{cases} 0 & \text{for } m \neq p \\ p! & \text{for } m = p \end{cases}
$$
最终得到(27)。

### 6. 合成运算符的指标

与 n° 5 中的假设相同，将 (VI, p. 277) 的公式 (26) 应用于函数 $e^{\lambda x}$，给出
$$
U_\lambda^\xi (e^{\lambda \xi}) = U_0^\xi (e^{\lambda x} e^{\lambda \xi}) = e^{\lambda x} U_0^\xi (e^{\lambda \xi}) = u(\lambda) e^{\lambda x}
$$
(30)
放置 $u(\lambda) = U_0^\xi (e^{\lambda \xi})$ 时。有人说，在$\mathbf{C}$上定义的函数$u(\lambda)$，与复数值一起，是合成运算符$U$的*指示矩阵*。 注如果多项式中$U$到环$\mathbf{C}[X]$的限制等于级数
$$
D^p \sum_{n=0}^{\infty} \alpha_n D^n
$$
（VI，p. 271，第 1）（我们在 VI，p. 271 中表示为 $u(D)$），*复数项* 的级数与一般项 $\alpha_n \lambda^{n+p}$ *不一定收敛* $\lambda \neq 0$，即使它收敛于$\lambda$的某些值，和*也不一定等于U*的指示线*$u(\lambda)$*（VI，p. 291，练习2）。我们可以说，合成运算符$U$是*正则*，如果$\mathbf{C}$中存在0的邻域，使得级数与一般项$\alpha_n \lambda^{n+p}$*绝对收敛*并且具有和*等于指标矩阵* $u(\lambda)$关于这个邻域$^1$。让我们将VI、p. 278的公式(27)应用到函数$e^{\lambda x}$，得到$h = 0$；因为 $D^m(e^{\lambda x}) = \lambda^m e^{\lambda x}$ 一个人有 $U_0^\xi \left( D^m(e^{\lambda x}) \right) = \lambda^m u(\lambda)$；那么对于每个复数$\lambda$使得$u(\lambda) \neq 0$

$$
\frac{\lambda^p e^{\lambda x}}{u(\lambda)} = \sum_{m=0}^n u_m(x) \frac{\lambda^m}{m!} - \frac{\lambda^{n+1}}{u(\lambda)} U_0^\xi \left( \int_0^{\xi-x} \frac{1}{n!} u_n(x+\eta) e^{\lambda(\xi-\eta)} d\eta \right)
$$

特别是对于 $x = 0$

$$
\frac{\lambda^p}{u(\lambda)} = \sum_{m=0}^n \beta_m \frac{\lambda^m}{m!} - \frac{\lambda^{n+1}}{u(\lambda)} U_0^\xi \left( \int_0^{\xi} \frac{1}{n!} u_n(\eta) e^{\lambda(\xi-\eta)} d\eta \right)
$$

与$\beta_m = u_m(0)$。

如果$U$是*正则*算子，对于所有$\lambda \in \mathbf{C}$，使得整个级数、$u(\lambda) = \sum_{n=0}^\infty \alpha_n \lambda^{n+p}$和$\sum_{n=0}^\infty \beta_n \frac{\lambda^n}{n!}$绝对收敛$^2$，则从两个绝对收敛级数的乘积的公式(16)和公式得出（*Gen.Top.*，VIII，p. 115，道具 1）

$$
\frac{\lambda^p}{u(\lambda)} = \sum_{n=0}^\infty \beta_n \frac{\lambda^n}{n!}.
$$

类似地，由于$e^{\lambda x}$的泰勒展开对于每个$\lambda \in \mathbf{C}$和每个$x \in \mathbf{C}$（III，p. 106）绝对收敛，因此也有（公式（6）（VI，p. 273）和（16）（VI， p. 274))，对于所有值以及所有 $x \in \mathbf{C}$

$$
\frac{\lambda^n e^{\lambda x}}{u(\lambda)} = \sum_{n=0}^\infty u_n(x) \frac{\lambda^n}{n!}.
$$

#### 注 {#fvr-vi-s1-n6-rem-1 .statement tag=08I5}

通过在整个级数上使用以下引理，可以将公式（33）（或（34））用于计算和$\beta_n$（或$u_n(x)$）：

（1）稍后我们要研究级数，它的通项是形式$c_n z^n$（$c_n \in \mathbf{C}, z \in \mathbf{C}$），称之为*整个级数*；特别是，我们将看到，当级数对于$z = z_0$绝对收敛时，它对于$|z| \leq |z_0|$“通常收敛”。
(2) 由整体级数理论可知，当其中一个级数绝对收敛于0的邻域$V$时，另一个也绝对收敛于0的邻域$W \subset V$。

艾玛。 **如果两个完整的级数** $\sum_{n=0}^{\infty} c_n \lambda^n,\ \sum_{n=0}^{\infty} d_n \lambda^n$ **对于所有** $\lambda$ **在** $0$的邻域中绝对收敛，**并且如果** $\sum_{n=0}^{\infty} c_n \lambda^n = \sum_{n=0}^{\infty} d_n \lambda^n$ **对于这些** $\lambda$的值，**则** $c_n = d_n$ **对于所有整数** $n \geqslant 0$。

如果通过任何过程，可以找到在$0$的邻域上收敛到$\lambda^p / u(\lambda)$的整个级数，那么这个级数的系数必然等于$\beta_n / n!$。我们将在下面的例中应用这个程序。

#### 例 1 {#fvr-vi-s1-n6-exa-1 .statement tag=08I6}

如果$U$是恒等式映射，则有$u(\lambda) = 1$并且运算符$U$显然是单数；因为VI、p. 278的$u_n(x) = x^n$公式(27)可以写成，把$\xi = \xi - \eta$

$$
f(x + h) = \sum_{n=0}^{\infty} \frac{1}{m!} f^{(m)}(h) x^m + \int_h^{x+h} f^{(n+1)}(t) \frac{(x + h - t)^n}{n!} dt
$$

也就是说，它约化到泰勒公式（II，p. 62）。

#### 例 2 {#fvr-vi-s1-n6-exa-2 .statement tag=08I7}

让我们采用 $U$ 合成运算符，对于 $\mathbf{R}_+$ 上定义的每个函数 $f$，关联函数 $x \mapsto f(x + 1) - f(x)$；然后

$$
U_{\lambda}^{\xi} (f(\xi)) = f(x + 1) - f(x);
$$

我们已经看到（VI，p. 275）$U$到$\mathbf{C}[X]$的限制等于$e^D - 1$。另一方面，由于 $u(\lambda) = e^{\lambda} - 1$，运算符 $U$ 是*常规*；我们将看到（VI，p. 288）如何通过将$\frac{\lambda}{e^{\lambda} - 1}$的展开计算为收敛整体级数来计算确定伯努利数$b_n$。在VI、p. 278的应用公式(27)上到函数$f$的*原语*，承认$\mathbf{R}_+$上的连续$n^{th}$导数，我们得到

$$
f(x + h) = \int_h^{h+1} f(t) dt
$$
$$
+ \sum_{m=1}^n \frac{1}{m!} B_m(x) \left( f^{(m-1)}(h+1) - f^{(m-1)}(h) \right) + R_n(x, h)
$$

与

这个引理是一般结果的特例，我们稍后会证明；这是证明。如果整个级数$\sum_{n=0}^{\infty} c_n \lambda^n$对于$\lambda = \lambda_0$绝对收敛，那么对于每个整数$k \geqslant 0$级数$\sum_{n=0}^{\infty} c_{n+k} \lambda^n$通常对于$|\lambda| \leqslant |\lambda_0|$收敛，因此在此盘上连续（*Gen.Top.*，X， p. 283); $0$ 邻域上的结论 $\sum_{n=k+1}^{\infty} c_n \lambda^n = o(\lambda^k)$。然后从函数的渐近展开在$\lambda^n$的项中的系数唯一性得出引理（V，p. 223）。

$$
R_n(x, h) = - \int_0^{1-x} \frac{B_n(x + \eta)}{n!} f^{(n)}(h + 1 - \eta) d\eta \\
+ \int_0^{-x} \frac{B_n(x + \eta)}{n!} f^{(n)}(h - \eta) d\eta.
$$

(36)

#### 例 3 {#fvr-vi-s1-n6-exa-3 .statement tag=08I8}

令 E 为函数 $f$ 的向量空间，在 $\mathbf{R}$ 上定义且连续，并且使得积分 $\int_{-\infty}^{+\infty} f(x + \xi) e^{-\xi^2/2} d\xi$ 对于所有 $x \geq 0$ 收敛。运算符 U 定义为

$$
U_\lambda^\xi \left( f(\xi) \right) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} f(x + \xi) d\xi
$$

然后定义在 E 上并且显然是合成运算符。 空间 E 包含所有指数$e^{\lambda x}$（$\lambda$任意复数），并且有一个

$$
u(\lambda) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-(\xi^2/2) + \lambda \xi} d\xi \\
= \frac{1}{\sqrt{2\pi}} e^{\lambda^2/2} \int_{-\infty}^{+\infty} e^{-(\xi - \lambda)^2/2} d\xi = e^{\lambda^2/2}
$$

（cf.III、p. 120、练习 24 和 VII、p. 313、公式 (22)）。一个有$n! \alpha_n = U_0^\xi (\xi^n) = \frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} \xi^n d\xi$。对于每一个整数 $n$ 都可以写

$$
\sum_{k=0}^n \int_{-\infty}^{+\infty} \frac{|\lambda \xi|^k}{k!} e^{-\xi^2/2} d\xi \leq 2 \int_0^{+\infty} e^{-(\xi^2/2) + |\lambda| \xi} d\xi.
$$

因而，级数$\sum_{n=0}^{\infty} e^{-\xi^2/2} \frac{(\lambda \xi)^n}{n!}$可以在$\mathbf{R}$上逐项积分（II，p. 72，cor.1），这证明级数$\sum_{n=0}^{\infty} \alpha_n \lambda^n$对于每个$\lambda \in \mathbf{C}$绝对收敛，并且和等于$u(\lambda) = e^{\lambda^2/2} = \sum_{n=0}^{\infty} \frac{\lambda^{2n}}{2^n n!}$；因此运算符 $U$ 是正则运算符。上面提到的应用引理表明，每$n \geq 0$就有$\alpha_{2n} = 1/2^n n!,\ \alpha_{2n+1} = 0$；因而，运算符 $U$ 的值是阶 0。

$$
\frac{1}{u(\lambda)} = e^{-\lambda^2/2} = \sum_{n=0}^{\infty} \frac{(-1)^n \lambda^{2n}}{2^n n!},
$$

级数对于每个$\lambda \in \mathbf{C}$绝对收敛； 另一个应用引理可知$\beta_{2n} = \frac{(-1)^n (2n)!}{2^n n!},\ \beta_{2n+1} = 0$；进一步，级数$\sum_{n=0}^{\infty} \frac{\lambda^n}{n!} u_n(x)$对于每个$\lambda \in \mathbf{C}$和每个$x \in \mathbf{R}$绝对收敛，并且有

$$
\sum_{n=0}^{\infty} \frac{\lambda^n}{n!} u_n(x) = \exp \left( -\frac{\lambda^2}{2} + \lambda x \right) = \exp \left( \frac{x^2}{2} \right) \exp \left( -\frac{1}{2} (\lambda - x)^2 \right).
$$

在应用上，泰勒公式到函数$\exp(-x^2/2)$，然​​后可以得到多项式$u_n(x)$的以下表达式：

$$
u_n(x) = (-1)^n e^{\lambda^2/2} \frac{d^n}{dx^n} (e^{-x^2/2}).
$$

该多项式称为次数 $n$ 的*埃尔米特多项式*，通常用 $\mathrm{H}_n(x)$ 表示。 VI、p. 273的公式(7)、(8)、(9)，这里给出

$$
\frac{d \mathrm{H}_n}{dx} = n \mathrm{H}_{n-1}(x)
$$

$$
\mathrm{H}_n(x+y) = \sum_{k=0}^n \binom{n}{k} \mathrm{H}_{n-k}(x) y^k
$$

$$
\frac{1}{\sqrt{2\pi}} \int_{-\infty}^{+\infty} e^{-\xi^2/2} \mathrm{H}_n(x+\xi) d\xi = x^n
$$

并且VI、p. 278的公式 (27) 变为，对于$h = 0$

$$
\sqrt{2\pi} f(x) = \sum_{m=0}^n \left( \int_{-\infty}^{+\infty} e^{\xi^2/2} f^{(m)}(\xi) d\xi \right) \frac{\mathrm{H}_m(x)}{m!}
$$
$$
- \int_{-\infty}^{+\infty} d\xi \int_0^\xi \frac{\mathrm{H}_n(x+\eta)}{n!} e^{-(\xi+\eta)^2/2} f^{(n+1)}(x+\xi-\eta) d\eta.
$$

### 7. 欧拉-麦克劳林求和公式

在VI、p. 280的公式(35)中，让我们将替换$x$乘以0，将$h$乘以$x$；因为 $\mathrm{B}_m(0) = b_m$ 是从 VI、p. 276 的关系 (24) 得出的，对于每个整数 $p > 0$ 可以写

$$
f(x) = \int_x^{x+1} f(t) dt - \frac{1}{2} (f(x+1) - f(x))
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} \left( f^{(2k-1)}(x+1) - f^{(2k-1)}(x) \right) + R_p(x)
$$
与
$$
R_p(x) = - \frac{1}{(2p+1)!} \int_0^1 \mathrm{B}_{2p+1}(t) f^{(2p+1)}(x+1-t) dt.
$$
在这个公式让我们依次通过替换$x$乘以$x+1, x+2, \ldots, x+n$，并将得到的公式一一组合起来；我们得到

$$
\begin{cases}
f(x) + f(x+1) + \cdots + f(x+n) \\
= \int_x^{x+n+1} f(t) dt - \frac{1}{2} (f(x+n+1) - f(x)) \\
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} \left( f^{(2k-1)}(x+n+1) - f^{(2k-1)}(x) \right) + T_p(x, n)
\end{cases}
$$
与
$$
T_p(x, n) = - \frac{1}{(2p+1)!} \int_0^1 \mathrm{B}_{2p+1}(t) \left( \sum_{k=0}^n f^{(2p+1)}(x+k+1-t) \right) dt.
$$

这个公式中的余数$T_p(x, n)$可以用以下方式重写：用$\overline{B}_{2p+1}(t)$表示周期为1的*周期*函数，它等于间隔$[0, 1[$上的$B_{2p+1}(t)$。然后

$$
\int_0^1 B_{2p+1}(t) f^{(2p+1)}(x + k + 1 - t) \, dt = \int_k^{k+1} \overline{B}_{2p+1}(1 - s) f^{(2p+1)}(x + s) \, ds
$$

因而

$$
T_p(x, n) = - \frac{1}{(2p+1)!} \int_0^{n+1} \overline{B}_{2p+1}(1 - s) f^{(2p+1)}(x + s) ds.
$$ (41)

公式 (39) 称为*欧拉-麦克劳林求和公式*；它适用于每个复数函数，对于每个$x \geq x_0$，在区间$[x_0, +\infty[$上都有连续的$(2p + 1)^{th}$导数。我们将看到（VI，p. 288）如何估计这个公式中的*余数*$T_p(x, n)$。

### 习题{#fvr-vi-s1-exercises}

参见[习题为 § 1](exercises/s1/)。
