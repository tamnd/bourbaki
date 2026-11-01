---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 2
section_title: EULERIAN EXPANSIONS OF THE TRIGONOMETRIC FUNCTIONS AND BERNOULLI NUMBERS
lang: zh
source: fvr-i-vii
book_pages: 283-288, 292-296
pdf_pages: 0298-0303, 0307-0311
extraction: ocr
subsections:
    - "no": 1
      title: EULERIAN EXPANSION OF $\cot z$
      page: 283
      pdf_page: 298
    - "no": 2
      title: EULERIAN EXPANSION OF $\sin z$
      page: 286
      pdf_page: 301
    - "no": 3
      title: APPLICATION TO THE BERNOULLI NUMBERS
      page: 287
      pdf_page: 302
statements: 5
exercises: 13
content_sha256: 9f376a256b321221bb198ed6fbc7fde59d9d479fdd16478ee205992de94e1422
translated_from: content/en/fvr/VI/02_s2_eulerian_expansions_of_the.md
translation_method: google
source_content_sha256: 3c79b30ff58a4995c02b9783d2b22927cb3d4728ceeaf6e2ab3524761187a1a8
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 6d352228b92afef9095aebefffafa6eebfdede0627924f747c3e9fe4a4ffec5b
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 2。三角函数函数和伯努利数的欧拉展开

### 1. 欧拉展开 OF $\cot z$

通过VI、p. 275、数$b_n / n!$的公式(20)，是$S/(e^S - 1)$的展开中的系数作为*形式*级数；我们将在这个截面中证明，函数$z/(e^z - 1)$等于$\mathbf{C}$中0的邻域上绝对收敛的整个级数的和；从VI、p. 280的引理可以得出，这个级数的系数是数$b_n / n!$，从中我们可以推导出伯努利数$b_n$的估计。

首先我们注

$$
\frac{z}{e^z - 1} = - \frac{z}{2} + \frac{z}{2} \frac{e^z + 1}{e^z - 1} = - \frac{z}{2} + \frac{iz}{2} \cot \frac{iz}{2}.
$$ (1)

我们将获得以下$\cot z$的级数展开，对于$\pi$的每个$z$而不是整数倍数有效。

#### 命题 1 {#fvr-vi-s2-prop-1 .statement tag=08IC}

*对于每个复数* $z$ *和每个整数* $n$ *一个有*

$$
\sin nz = 2^{n-1} \sin z \sin \left(z + \frac{\pi}{n}\right) \sin \left(z + \frac{2\pi}{n}\right) \ldots \sin \left(z + \frac{(n-1)\pi}{n}\right).
$$ (2)

确实，可以写

$$
\sin nz = \frac{e^{niz} - e^{-niz}}{2i} = \frac{e^{-niz}(e^{2niz} - 1)}{2i}
= \frac{e^{-niz}(e^{2iz} - 1)(e^{2iz} - e^{-2i\pi/n}) \ldots (e^{2iz} - e^{-2(n-1)i\pi/n})}{2i}
= A \sin z \sin \left( z + \frac{\pi}{n} \right) \sin \left( z + \frac{2\pi}{n} \right) \ldots \sin \left( z + \frac{(n-1)\pi}{n} \right)
$$

哪里
$$
A = (2i)^{n-1} e^{-\frac{i\pi}{n}(1+2+\ldots+(n-1))} = (2i)^{n-1} e^{-i(n-1)\frac{\pi}{2}} = 2^{n-1}.
$$

#### 推出 1 {#fvr-vi-s2-prop-1-cor-1 .statement tag=08ID}

*每整数 n 人拥有*
$$
\sin \frac{\pi}{n} \sin \frac{2\pi}{n} \ldots \sin \frac{(n-1)\pi}{n} = \frac{n}{2^{n-1}}.
$$
(3)

只要将(2)两边的除除以$\sin z$即可，并且让$z$趋于0。

#### 推出 2 {#fvr-vi-s2-prop-1-cor-2 .statement tag=08IE}

*对于每个奇数整数 $n = 2m + 1$，以及每个复数 $z$，使得 $nz$ 不是 $\pi$ 的积分倍数，有一个*
$$
\cot nz = (-1)^m \cot z \cot \left( z + \frac{\pi}{n} \right) \ldots \cot \left( z + \frac{(n-1)\pi}{n} \right).
$$
(4)

事实上，(2) 中 $\sin n \left( z + \frac{\pi}{2} \right) = \sin \left( nz + \frac{\pi}{2} + m\pi \right) = (-1)^m \cos nz$、从而、替换 $z$ 乘以 $z + \frac{\pi}{2}$，

$$
\cos nz = (-1)^m 2^{n-1} \cos z \cos \left( z + \frac{\pi}{n} \right) \ldots \cos \left( z + \frac{(n-1)\pi}{n} \right)
$$
(5)

公式 (2) 和 (5) 当 $\sin nz \neq 0$ 时，逐项除法得到 (4)。

在接下来的所有内容中，我们将始终假设 $n = 2m + 1$ 是奇数整数； 公式 (4) 也可以写成

$$
\cot nz = (-1)^m \prod_{k=-m}^{m} \cot \left( z - \frac{k\pi}{n} \right).
$$

或者，一个人有

$$
\cot \left( z - \frac{k\pi}{n} \right) = \frac{1 + \tan z \tan \frac{k\pi}{n}}{\tan z - \tan \frac{k\pi}{n}}
$$

对于 tan z 有限；因此 cot $nz$ 是 $u = \tan z$ 中的有理数函数，其分子为次数 $n - 1$，其分母为次数 $n$，具有 $n$ 简单根 $\tan k\pi / n$；将其分解为简单的分数产量

$$
\cot nz = \sum_{k=-m}^{m} \frac{A_k}{u - \tan \frac{k\pi}{n}}
$$

哪里

$$
A_k = \lim_{z \to k\pi/n} \cot nz \left( \tan z - \tan \frac{k\pi}{n} \right) = \lim_{z \to k\pi/n} \frac{\cos nz}{\sin nz} \frac{\sin \left( z - \frac{k\pi}{n} \right)}{\cos z \cos \frac{k\pi}{n}}
$$
$$
= \lim_{h \to 0} \frac{\cos nh}{\cos \frac{k\pi}{n} \cos \left( h + \frac{k\pi}{n} \right)} \frac{\sin h}{\sin nh} = \frac{1}{n \cos^2 \frac{k\pi}{n}}
$$

从而，将 (6) 相应的中的项分离到 $k = 0$ 并将项相应的组合到 $k$ 的相反值，以及替换 $z$ $z/n$,

$$
\cot z = \frac{1}{n \tan \frac{z}{n}} + \sum_{k=1}^{m} \frac{2n \tan \frac{z}{n}}{\cos^2 \frac{k\pi}{n} \left( n \tan \frac{z}{n} \right)^2 - \left( n \sin \frac{k\pi}{n} \right)^2}
$$

对于每个复数 $z$ 有效，而不是 $\pi/2$ 的积分倍数。可以将公式写成形式

$$
\cot z = \frac{1}{n \tan \frac{z}{n}} + \sum_{k=1}^{\infty} v_k(n, z)
$$

$v_k(n, z) = 0$ 为 $k > m$ 且

$$
v_k(n, z) = \frac{2n \tan \frac{z}{n}}{\cos^2 \frac{k\pi}{n} \left( n \tan \frac{z}{n} \right)^2 - \left( n \sin \frac{k\pi}{n} \right)^2}
$$

对于$1 \leq k \leq m$。我们将看到，对于$\mathbf{C}$的紧凑子集 K中包含的每个$z$，而不是包含$\pi$的任何积分倍数，以及对于每个足够大奇数$n$，级数与一般项 $v_k(n, z)$ 通常是收敛的。事实上，由于$n$趋于$+\infty$，$\tan \frac{z}{n}$在K上一致趋于$\frac{z}{n}$，因此存在数$M > 0$，使得每个足够大$m$和每个$z \in K$都有$\left| n \tan \frac{z}{n} \right| \leq M$。另一方面，对于$0 \leq x \leq \pi/2$，有$\sin x / x \geq 1 - \frac{x^2}{6} \geq \frac{1}{2}$，因此对于$1 \leq k \leq m$，有$n \sin \frac{k\pi}{n} \geq k\pi/2$；因而，当$m$为足够大时，对于每一个整数$k$，使得$k\pi /2 > M$有一个$|v_k(n, z)| \leq \frac{8M}{k^2 \pi^2 - 4M^2}$，这证明了我们的断言。对于 $k$ 奇数，$v_k(n, z)$ 趋向于（在 K 上一致）$\frac{2z}{z^2 - k^2 \pi^2}$，因为 $n$ 趋于 $+\infty$。因而：

#### 定理 1 {#fvr-vi-s2-thm-1 .statement tag=08IF}

*对于每个复数$z$，不是$\pi$的整数倍数，有一个*

$$
\cot z = \frac{1}{z} + \sum_{n=1}^{\infty} \frac{2z}{z^2 - n^2 \pi^2}
$$

*（右侧的级数通常收敛于每个紧凑子集$K \subset \mathbf{C}$，而不是包含任何$\pi$的整数倍数（$\cot z$的欧拉展开）。）*

### 2. 欧拉展开 OF $\sin z$

对于 VI、p. 283 的每个 *奇数* 整数 $n = 2m + 1$ 和复数 $z$ 公式 (2)，可以写成

$$
\sin nz = (-1)^m 2^{n-1} \prod_{k=-m}^{m} \sin \left( z - \frac{k\pi}{n} \right)
$$
$$
= (-1)^m 2^{n-1} \sin z \prod_{k=1}^{m} \sin \left( z - \frac{k\pi}{n} \right) \sin \left( z + \frac{k\pi}{n} \right).
$$

现在，一个人有$\sin \left( z - \frac{k\pi}{n} \right) \sin \left( z + \frac{k\pi}{n} \right) = \sin^2 z - \sin^2 \frac{k\pi}{n}$，并且，通过（3）（VI，284），$\prod_{k=1}^{m} \sin^2 \frac{k\pi}{n} = \frac{n}{2^{n-1}}$，从而，在替换$z$通过$z/n$，

$$
\sin z = n \sin \frac{z}{n} \prod_{k=1}^{m} \left( 1 - \frac{\sin^2 \frac{z}{n}}{\sin^2 \frac{k\pi}{n}} \right).
$$

我们可以将这个公式写为$\sin z = n \sin \frac{z}{n} \prod_{k=1}^{m} (1 - w_k(n, z))$，如果$k > m$则写为$w_k(n, z) = 0$，对于$1 \leq k \leq m$则写为$w_k(n, z) = \frac{\sin^2 \frac{z}{n}}{\sin^2 \frac{k\pi}{n}}$。我们将看到，对于$\mathbf{C}$的紧凑子集$K$中包含的每个$z$，以及对于奇数$n$，级数与一般项$w_k(n, z)$*通常收敛*。事实上，由于$n$趋向于$+\infty$，$n \sin \frac{z}{n}$在$K$上一致趋向于$z$，因此存在数$M > 0$，使得$\left| n \sin \frac{z}{n} \right| \leq M$对于每个整数$n$和每个$z \in K$。此外，我们在证明中看到了。 VI、p. 286 中的 1 个，$1 \leq k \leq m$ 的其中一个有 $n \sin \frac{k \pi}{n} \geq \frac{k \pi}{2}$；因此，对于每个整数$k$，使得$k \pi / 2 \geq M$有$|w_k(n, z)| \leq 4M^2 / k^2 \pi^2$，这证明了我们的断言。因为，对于每个固定的 $k$，$w_k(n, z)$ 趋向于（在 K 上统一）$z^2 / k^2 \pi^2$，而 $n$ 趋向于 $+\infty$，因此可以看出：

#### 定理 2 {#fvr-vi-s2-thm-2 .statement tag=08IG}

每有复数 $z$ 就有

$$
\sin z = z \prod_{n=1}^{\infty} \left( 1 - \frac{z^2}{n^2 \pi^2} \right)
$$

右边的无穷乘积绝对一致地收敛于$\mathbf{C}$的每个紧致子集（$\sin z$的欧拉展开）。

### 3.伯努利数的应用

定理 1 of VI, p. 286，表明对于 $0 \leq x < \pi$，级数与一般项

$$
\frac{2x}{n^2 \pi^2 - x^2} \geq 0
$$

收敛。另一方面，对于每个复数$z$，可以写出$|z| < \pi$，

$$
\frac{2z}{n^2 \pi^2 - z^2} = \frac{2z}{n^2 \pi^2} \sum_{k=0}^{\infty} \frac{z^{2k}}{n^{2k} \pi^{2k}}
$$

右边的级数绝对收敛。由此我们可以推断出“双”级数

$$
\sum_{n=1}^{\infty} \sum_{k=1}^{\infty} \frac{-2z^{2k-1}}{n^{2k} \pi^{2k}}
$$

在开盘$|z| < \pi$中绝对收敛，通常收敛于该盘中包含的每个紧集，并且具有和$\cot z - \frac{1}{z}$。事实上，对于$|z| \leq a < \pi$，(11)的一般项的绝对值至多等于$2a^{2k-1} / n^{2k} \pi^{2k}$，并且项$2a^{2k-1} / n^{2k} \pi^{2k}$的任何有限数的和小于有限数 $\sum_{n=1}^{\infty} \frac{2a}{n^2 \pi^2 - a^2}$；首先对$k$求和，然后对$n$求和，可以看到级数(11)的和等于$\sum_{n=1}^{\infty} \frac{2z}{z^2 - n^2 \pi^2}$，这证明了我们的叙述。

如果现在一个和级数 (11) 首先超过 $n$ 然后超过 $k$ 一个获得恒等式（对于 $|z| < \pi$）

$$
\cot z - \frac{1}{z} = -2 \sum_{k=1}^{\infty} \frac{S_{2k}}{\pi^{2k}} z^{2k-1}
$$

我们放置$S_k = \sum_{n=1}^{\infty} \frac{1}{n^k}$的地方。通过 (1) (VI, p. 283)，对于 $|z| < 2\pi$ 从而，我们得到公式

$$
b_{2n} = (-1)^{n-1} (2n)! \frac{2 S_{2n}}{(2\pi)^{2n}} \quad \text{for } n \geq 1,
$$

公式特别表明数 $S_{2n}/\pi^{2n}$ 是*有理数*。显然 $S_{k+1} \leq S_k$ 因此，对于每个整数 $k \geq 2$，我们有 $S_k \leq S_2 = \pi^2/6 \leq 2$；从 (14) 推导出伯努利数的以下不等式

$$
\frac{2 (2n)!}{(2\pi)^{2n}} \leq |b_{2n}| \leq 4 \frac{(2n)!}{(2\pi)^{2n}} \quad \text{for } n \geq 1.
$$

从这些不等式中，我们可以推导出伯努利多项式的估计值

$$
B_n(x) = \sum_{k=0}^n \binom{n}{k} b_k x^{n-k}; \text{ in particular, for } 0 \leq x \leq 1 \text{ one has}
$$

$$
|B_n(x)| \leq 4 \sum_{k=0}^n \binom{n}{k} \frac{k!}{(2\pi)^k} = 4 \frac{n!}{(2\pi)^n} \sum_{k=0}^n \frac{(2\pi)^k}{k!} \leq 4 e^{2\pi} \frac{n!}{(2\pi)^n}.
$$

### 习题 {#fvr-vi-s2-exercises}

§ 2](exercises/s2/)参见[习题。
