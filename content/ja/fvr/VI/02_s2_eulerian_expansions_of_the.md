---
book: fvr
book_title: Functions of a Real Variable
chapter: VI
chapter_title: GENERALIZED TAYLOR EXPANSIONS EULER-MACLAURIN SUMMATION FORMULA
section: 2
section_title: EULERIAN EXPANSIONS OF THE TRIGONOMETRIC FUNCTIONS AND BERNOULLI NUMBERS
lang: ja
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
content_sha256: f9493e4f2e4a880c12ae5bb508754cf0123b0d818038c71a7d77244f999e0e6b
translated_from: content/en/fvr/VI/02_s2_eulerian_expansions_of_the.md
translation_method: google
source_content_sha256: 3c79b30ff58a4995c02b9783d2b22927cb3d4728ceeaf6e2ab3524761187a1a8
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 883b09bd19f03c2f4d85ff99f11b50aa04d305c9819716c16a7ed9aba2d9a24f
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。三角関数写像とベルヌーイ数のオイラー展開

### 1. $\cot z$ のオイラー展開

VI、p. 275、数 $b_n / n!$ の公式 (20) により、$S/(e^S - 1)$ を *正式* 系列として拡張すると、係数になります。この切断で、写像 $z/(e^z - 1)$ が、$\mathbf{C}$ の 0 の近傍上の絶対収束全体系列の和に等しいことを示します。 VI、p. 280の補題から、この系列の係数は数$b_n / n!$となり、そこからベルヌーイ数$b_n$の推定値を導き出します。

まず最初に注意するのは、

$$
\frac{z}{e^z - 1} = - \frac{z}{2} + \frac{z}{2} \frac{e^z + 1}{e^z - 1} = - \frac{z}{2} + \frac{iz}{2} \cot \frac{iz}{2}.
$$ (1)

$\cot z$ の以下の系列拡張を取得します。これは、$\pi$ の整数倍数ではなく、すべての $z$ に有効です。

#### 命題 1 {#fvr-vi-s2-prop-1 .statement tag=08IC}

*すべての複素数* $z$ *およびすべての整数* $n$ *1 つは*

$$
\sin nz = 2^{n-1} \sin z \sin \left(z + \frac{\pi}{n}\right) \sin \left(z + \frac{2\pi}{n}\right) \ldots \sin \left(z + \frac{(n-1)\pi}{n}\right).
$$ (2)

確かに、次のように書くことができます

$$
\sin nz = \frac{e^{niz} - e^{-niz}}{2i} = \frac{e^{-niz}(e^{2niz} - 1)}{2i}
= \frac{e^{-niz}(e^{2iz} - 1)(e^{2iz} - e^{-2i\pi/n}) \ldots (e^{2iz} - e^{-2(n-1)i\pi/n})}{2i}
= A \sin z \sin \left( z + \frac{\pi}{n} \right) \sin \left( z + \frac{2\pi}{n} \right) \ldots \sin \left( z + \frac{(n-1)\pi}{n} \right)
$$

どこで
$$
A = (2i)^{n-1} e^{-\frac{i\pi}{n}(1+2+\ldots+(n-1))} = (2i)^{n-1} e^{-i(n-1)\frac{\pi}{2}} = 2^{n-1}.
$$

#### 系 1 {#fvr-vi-s2-prop-1-cor-1 .statement tag=08ID}

*誰もが持っていない整数ごとに*
$$
\sin \frac{\pi}{n} \sin \frac{2\pi}{n} \ldots \sin \frac{(n-1)\pi}{n} = \frac{n}{2^{n-1}}.
$$
(3)

(2)の両辺を$\sin z$で割るし、$z$が0になる傾向を持たせれば十分です。

#### 系 2 {#fvr-vi-s2-prop-1-cor-2 .statement tag=08IE}

*すべての奇数整数 $n = 2m + 1$ と、$nz$ が $\pi$ の整数倍数ではないようなすべての複素数 $z$ について、*
$$
\cot nz = (-1)^m \cot z \cot \left( z + \frac{\pi}{n} \right) \ldots \cot \left( z + \frac{(n-1)\pi}{n} \right).
$$
(4)

確かに、(2) の $z + \frac{\pi}{2}$ により、$\sin n \left( z + \frac{\pi}{2} \right) = \sin \left( nz + \frac{\pi}{2} + m\pi \right) = (-1)^m \cos nz$、よって、置き換えること $z$、

$$
\cos nz = (-1)^m 2^{n-1} \cos z \cos \left( z + \frac{\pi}{n} \right) \ldots \cos \left( z + \frac{(n-1)\pi}{n} \right)
$$
(5)

式 (2) と (5) は、$\sin nz \neq 0$ の場合の項ごとの除算で (4) を与えます。

以下のすべてにおいて、$n = 2m + 1$ は奇数の整数であると常に仮定します。 公式 (4) とも書くことができます

$$
\cot nz = (-1)^m \prod_{k=-m}^{m} \cot \left( z - \frac{k\pi}{n} \right).
$$

または、ある人は

$$
\cot \left( z - \frac{k\pi}{n} \right) = \frac{1 + \tan z \tan \frac{k\pi}{n}}{\tan z - \tan \frac{k\pi}{n}}
$$

Tan z 有限の場合。したがって、cot $nz$ は $u = \tan z$ の有理数写像であり、その分子は次数 $n - 1$ であり、分母は次数 $n$ であり、$n$ は単純な根 $\tan k\pi / n$ です。これを単純な分数に分解すると、次のようになります。

$$
\cot nz = \sum_{k=-m}^{m} \frac{A_k}{u - \tan \frac{k\pi}{n}}
$$

どこ

$$
A_k = \lim_{z \to k\pi/n} \cot nz \left( \tan z - \tan \frac{k\pi}{n} \right) = \lim_{z \to k\pi/n} \frac{\cos nz}{\sin nz} \frac{\sin \left( z - \frac{k\pi}{n} \right)}{\cos z \cos \frac{k\pi}{n}}
$$
$$
= \lim_{h \to 0} \frac{\cos nh}{\cos \frac{k\pi}{n} \cos \left( h + \frac{k\pi}{n} \right)} \frac{\sin h}{\sin nh} = \frac{1}{n \cos^2 \frac{k\pi}{n}}
$$

したがって、$k = 0$ に対応する (6) の項を分離し、$k$ の反対の値に対応する項を結合し、$z$ を $z/n$ に置き換えると、

$$
\cot z = \frac{1}{n \tan \frac{z}{n}} + \sum_{k=1}^{m} \frac{2n \tan \frac{z}{n}}{\cos^2 \frac{k\pi}{n} \left( n \tan \frac{z}{n} \right)^2 - \left( n \sin \frac{k\pi}{n} \right)^2}
$$

$\pi/2$ の整数倍数ではなく、すべての複素数 $z$ に対して有効です。これを公式を形で書くことができます

$$
\cot z = \frac{1}{n \tan \frac{z}{n}} + \sum_{k=1}^{\infty} v_k(n, z)
$$

$v_k(n, z) = 0$ は $k > m$ で、

$$
v_k(n, z) = \frac{2n \tan \frac{z}{n}}{\cos^2 \frac{k\pi}{n} \left( n \tan \frac{z}{n} \right)^2 - \left( n \sin \frac{k\pi}{n} \right)^2}
$$

$1 \leq k \leq m$の場合。 $\mathbf{C}$ のコンパクトな部分集合 K に含まれるすべての $z$ について、$\pi$ の整数倍数含むではなく、すべての十分大きいの奇数 $n$、系列と一般項が含まれることがわかります。 $v_k(n, z)$ は通常は収束します。確かに、$n$ は $+\infty$ になる傾向があり、$\tan \frac{z}{n}$ は K 上で一様に $\frac{z}{n}$ になる傾向があるため、十分大きい $m$ およびすべての $z \in K$ に対して $\left| n \tan \frac{z}{n} \right| \leq M$ となるような数 $M > 0$ が存在します。一方、$0 \leq x \leq \pi/2$ の場合、1 つは $\sin x / x \geq 1 - \frac{x^2}{6} \geq \frac{1}{2}$ を持ち、$1 \leq k \leq m$ の場合、1 つは $n \sin \frac{k\pi}{n} \geq k\pi/2$ を持ちます。従って、$m$が十分大きいのとき、$k\pi /2 > M$となる整数$k$ごとに$|v_k(n, z)| \leq \frac{8M}{k^2 \pi^2 - 4M^2}$があり、主張が証明されます。 $k$ 奇数の場合、$n$ が $+\infty$ になる傾向があるのと同様に、$v_k(n, z)$ は (K 上で一律に) $\frac{2z}{z^2 - k^2 \pi^2}$ になる傾向があります。その結果：

#### 定理 1 {#fvr-vi-s2-thm-1 .statement tag=08IF}

*$\pi$ の整数倍数ではない、すべての複素数 $z$ について、*

$$
\cot z = \frac{1}{z} + \sum_{n=1}^{\infty} \frac{2z}{z^2 - n^2 \pi^2}
$$

*(右側の系列は、通常、$\pi$ の含む整数倍数 ($\cot z$ のオイラー展開) ではなく、すべてのコンパクト部分集合 $K \subset \mathbf{C}$ に収束します。)*

### 2. $\sin z$ のオイラー展開

すべての *奇数* 整数 $n = 2m + 1$ と複素数 $z$ 公式 (2) の VI、p. 283 について、次のように書くことができます。

$$
\sin nz = (-1)^m 2^{n-1} \prod_{k=-m}^{m} \sin \left( z - \frac{k\pi}{n} \right)
$$
$$
= (-1)^m 2^{n-1} \sin z \prod_{k=1}^{m} \sin \left( z - \frac{k\pi}{n} \right) \sin \left( z + \frac{k\pi}{n} \right).
$$

さて、1 つは $\sin \left( z - \frac{k\pi}{n} \right) \sin \left( z + \frac{k\pi}{n} \right) = \sin^2 z - \sin^2 \frac{k\pi}{n}$ を持ち、(3) (VI, 284)、$\prod_{k=1}^{m} \sin^2 \frac{k\pi}{n} = \frac{n}{2^{n-1}}$、よってで、置き換えること $z$ は $z/n$ によって、

$$
\sin z = n \sin \frac{z}{n} \prod_{k=1}^{m} \left( 1 - \frac{\sin^2 \frac{z}{n}}{\sin^2 \frac{k\pi}{n}} \right).
$$

この公式を$\sin z = n \sin \frac{z}{n} \prod_{k=1}^{m} (1 - w_k(n, z))$、$k > m$の場合は$w_k(n, z) = 0$、$1 \leq k \leq m$の場合は$w_k(n, z) = \frac{\sin^2 \frac{z}{n}}{\sin^2 \frac{k\pi}{n}}$と書くことができます。 $\mathbf{C}$ のコンパクト部分集合 $K$ に含まれるすべての $z$ と、奇数の $n$ について、系列と一般的な項 $w_k(n, z)$ は *通常収束* であることがわかります。確かに、$n$ は $+\infty$ になる傾向があり、$n \sin \frac{z}{n}$ は$K$ に一様に $z$ になる傾向があるため、整数 $n$ ごとに $\left| n \sin \frac{z}{n} \right| \leq M$ となるような数 $M > 0$ が存在します。 $z \in K$。さらに、私たちは 19 年の証明に見ました。 VI、p. 286 の 1、つまり $1 \leq k \leq m$ には $n \sin \frac{k \pi}{n} \geq \frac{k \pi}{2}$ があります。したがって、$k \pi / 2 \geq M$ となるすべての整数 $k$ には $|w_k(n, z)| \leq 4M^2 / k^2 \pi^2$ があり、これは私たちの主張を証明します。すべての固定 $k$ について、$w_k(n, z)$ は (K 上で一様に) $z^2 / k^2 \pi^2$ になる傾向があり、$n$ は $+\infty$ になる傾向があるため、次のことがわかります。

#### 定理 2 {#fvr-vi-s2-thm-2 .statement tag=08IG}

複素数 $z$ ごとに、人は

$$
\sin z = z \prod_{n=1}^{\infty} \left( 1 - \frac{z^2}{n^2 \pi^2} \right)
$$

右側の無限積は、$\mathbf{C}$ のすべてのコンパクト部分集合 ($\sin z$ のオイラー展開) に絶対的かつ一様に収束します。

### 3. ベルヌーイへの応用数

定理 VI の 1、p. 286 は、$0 \leq x < \pi$ について、系列と一般的な項を示します。

$$
\frac{2x}{n^2 \pi^2 - x^2} \geq 0
$$

収束します。一方、複素数 $z$ ごとに、$|z| < \pi$ のように次のように書くことができます。

$$
\frac{2z}{n^2 \pi^2 - z^2} = \frac{2z}{n^2 \pi^2} \sum_{k=0}^{\infty} \frac{z^{2k}}{n^{2k} \pi^{2k}}
$$

右側の系列は完全に収束しています。これから、「ダブル」系列が推論されます。

$$
\sum_{n=1}^{\infty} \sum_{k=1}^{\infty} \frac{-2z^{2k-1}}{n^{2k} \pi^{2k}}
$$

開いた円盤 $|z| < \pi$ では絶対に収束し、通常はこの円盤に含まれるすべてのコンパクト集合で収束し、和 $\cot z - \frac{1}{z}$ を持ちます。確かに、$|z| \leq a < \pi$ については、(11) の一般項の絶対値は最大でも $2a^{2k-1} / n^{2k} \pi^{2k}$ に等しく、項 $2a^{2k-1} / n^{2k} \pi^{2k}$ の有限数の和は有限数より小さいです。 $\sum_{n=1}^{\infty} \frac{2a}{n^2 \pi^2 - a^2}$;最初に $k$ を合計し、次に $n$ を合計すると、系列 (11) の和が $\sum_{n=1}^{\infty} \frac{2z}{z^2 - n^2 \pi^2}$ に等しいことがわかり、主張が証明されます。

ここで、和系列 (11) が最初に $n$ を超え、次に $k$ を超えると、($|z| < \pi$ の) 同一性が得られます。

$$
\cot z - \frac{1}{z} = -2 \sum_{k=1}^{\infty} \frac{S_{2k}}{\pi^{2k}} z^{2k-1}
$$

$S_k = \sum_{n=1}^{\infty} \frac{1}{n^k}$ を置いたところ。 (1) (VI, p. 283) により、$|z| < 2\pi$ よってについて、公式が得られます。

$$
b_{2n} = (-1)^{n-1} (2n)! \frac{2 S_{2n}}{(2\pi)^{2n}} \quad \text{for } n \geq 1,
$$

公式は、特に数 $S_{2n}/\pi^{2n}$ が *有理* であることを示しています。明らかに $S_{k+1} \leq S_k$ なので、整数 $k \geq 2$ ごとに、$S_k \leq S_2 = \pi^2/6 \leq 2$ になります。 (14) から、ベルヌーイ数に対する次の不等式が導出されます。

$$
\frac{2 (2n)!}{(2\pi)^{2n}} \leq |b_{2n}| \leq 4 \frac{(2n)!}{(2\pi)^{2n}} \quad \text{for } n \geq 1.
$$

これらの不等式からベルヌーイ多項式の推定値を導き出すことができます。

$$
B_n(x) = \sum_{k=0}^n \binom{n}{k} b_k x^{n-k}; \text{ in particular, for } 0 \leq x \leq 1 \text{ one has}
$$

$$
|B_n(x)| \leq 4 \sum_{k=0}^n \binom{n}{k} \frac{k!}{(2\pi)^k} = 4 \frac{n!}{(2\pi)^n} \sum_{k=0}^n \frac{(2\pi)^k}{k!} \leq 4 e^{2\pi} \frac{n!}{(2\pi)^n}.
$$

### 練習問題 {#fvr-vi-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
