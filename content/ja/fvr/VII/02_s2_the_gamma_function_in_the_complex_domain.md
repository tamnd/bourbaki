---
book: fvr
book_title: Functions of a Real Variable
chapter: VII
chapter_title: THE GAMMA FUNCTION
section: 2
section_title: THE GAMMA FUNCTION IN THE COMPLEX DOMAIN
lang: ja
source: fvr-i-vii
book_pages: 315-323, 327-328
pdf_pages: 0330-0338, 0342-0343
extraction: ocr
subsections:
    - "no": 1
      title: EXTENDING THE GAMMA FUNCTION TO C
      page: 315
      pdf_page: 330
    - "no": 2
      title: THE COMPLEMENTS’ RELATION AND THE LEGENDRE-GAUSS MULTIPLICATION FORMULA
      page: 316
      pdf_page: 331
    - "no": 3
      title: STIRLING'S EXPANSION
      page: 319
      pdf_page: 334
statements: 6
exercises: 6
content_sha256: 37213a1524411575a056e2ab7ea416491364fe5e6361fd326b2fdcc4509a5b91
translated_from: content/en/fvr/VII/02_s2_the_gamma_function_in_the_complex_domain.md
translation_method: google
source_content_sha256: 1c81174cbd47bb500a623e0c569e0a38286f1c72eeae4b3d0069a0e65ec296a4
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: d7f75b663719f602a3c271e59f13085eb1828803df12f92a8c86a5b6762e8c3f
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。複素領域のガンマ写像

### 1. ガンマ写像を C に拡張する

ワイエルシュトラスの公式に戻って、次の式を与えます。

$$
\frac{1}{\Gamma(x)} = x\, e^{\gamma x} \prod_{n=1}^{\infty} \left(1 + \frac{x}{n}\right) e^{-x/n}
$$

すべての実数 $x$ に対して $1/\Gamma(x)$ を、任意の複素数 $z$ に対して一般的な項 $\left(1 + \frac{z}{n}\right) e^{-z/n}$ を使用して無限積を考えます。 $e^{-z/n} = 1 - \frac{z}{n} + h(z)$、$|h(z)| \leq \frac{|z|^2}{2n^2} e^{|z/n|}$ (III、p. 106、公式 (8))、よってと書くことができます。

$$
\left(1 + \frac{z}{n}\right) e^{-z/n} = 1 + v_n(z)
$$

$|v_n(z)| \leq \frac{|z|^2}{n^2} \left(1 + \frac{e^{|z|}}{2}(1 + |z|)\right)$付き;したがって、検討中の無限積は、$\mathbf{C}$ のすべてのコンパクト部分集合に絶対的かつ一様に収束します。さらに、その値は点 $z = -n$ (\emph{Gen. Top.}、IX、p. 214、系) でのみ零になります。 VII、p. 315 の公式 (1) を考慮して、すべての複合体 $z$ に対して、

$$
\frac{1}{\Gamma(z)} = z\, e^{\gamma z} \prod_{n=1}^{\infty} \left(1 + \frac{z}{n}\right) e^{-z/n}.
$$

したがって、写像 $\Gamma(z)$ は、点 $-n$ ($n \in \mathbf{N}$) を除くすべての点 $z \in \mathbf{C}$ に対して定義されます。この集合と$-n$の近傍に$(z + n)\Gamma(z) \sim \frac{(-1)^n}{n!}$が連続しています。 公式 (2) は、マイナスの整数とは異なる $z$ ごとに $\Gamma(\overline{z}) = \overline{\Gamma(z)}$ があることを示しています。

手順を逆にすると、ガウスの公式 (VII, p. 307, 公式 (8)) からワイエルシュトラスの公式に進むことを可能にする議論は、複素数 $z$ にも当てはまり、$z \neq -n$ ($n \in \mathbf{N}$) については、

$$
\Gamma(z) = \lim_{n \to \infty} \frac{n^z n!}{z(z+1)\ldots(z+n)}
$$

$n^z = e^{z \log n}$ を入れることに同意します。以来

$$
\frac{n^{z+1} n!}{(z+1)(z+2)\ldots(z+n+1)} = z \frac{n}{n+1+z} \frac{n^z n!}{z(z+1)\ldots(z+n)}
$$

移行から極限に、再び基本関数方程式があります。

$$
\Gamma(z+1) = z\, \Gamma(z)
$$

$z \neq -n$ ($n \in \mathbf{N}$) ごとに。

$p$ を任意の整数 $> 0$、$K_p$ を開いたディスク $|z| < p$ とします。すべての $z \in K_p$ およびすべての整数 $n > p$ について、$1 + \frac{z}{n}$ は負の実数ではないため、$\log \left( 1 + \frac{z}{n} \right)$ が定義され、上記のことから、系列と一般的な項 $\log \left( 1 + \frac{z}{n} \right) - \frac{z}{n}$ ($n > p$) は *通常収束* することがわかります。 $K_p$に;一般的な項を有限の数回微分して得られる系列についても同じことが当てはまります。

$$
\left| \frac{1}{n} - \frac{1}{z+n} \right| \leq \frac{p}{n(n-p)} \quad \text{and} \quad \left| \frac{1}{(z+n)^k} \right| \leq \frac{1}{(n-p)^k} \qquad (k > 1)
$$

$z \in K_p$ と $n > p$ の場合。次に、(*cf.* II, p. 59, *注意 3*) $\Gamma(z)$ は、点 $-n$ を別にすれば、点 $z \in \mathbf{C}$ において *無限微分可能* であることがわかり、これらの点では、

$$
\frac{\Gamma'(z)}{\Gamma(z)} = -\gamma - \frac{1}{z} + \sum_{n=1}^{\infty} \left( \frac{1}{n} - \frac{1}{z+n} \right)
$$
(5)

$$
D^{k-1} \left( \frac{\Gamma'(z)}{\Gamma(z)} \right) = \sum_{n=0}^{\infty} \frac{(-1)^k (k-1)!}{(z+n)^k} \qquad \text{for} \quad k \geq 2,
$$
(6)

(5) と (6) の右辺は、含む整数 $\leq 0$ ではない、$\mathbf{C}$ のすべてのコンパクト部分集合で *通常収束* します。さらに、次のように書くこともできます

$$
\log \Gamma(z) \equiv -\gamma z - \log z + \sum_{n=1}^{\infty} \left( \frac{z}{n} - \log \left( 1 + \frac{z}{n} \right) \right) \qquad (\text{mod. } 2\pi i)
$$
(7)

この公式の対数が実負数数の場合、この点では $\log z$ のいずれか極限値 ($2\pi i$ だけ異なる) になることに同意します。 (7) の右辺の系列は、通常、整数 $\leq 0$ の含むではなく、$\mathbf{C}$ のすべてのコンパクト部分集合に収束します。

### 2. 補数の関係とルジャンドル ガウス乗法公式

VII、p. 315 の公式 (2) から、$z \in \mathbf{C}$ ごとに、

$$
\frac{1}{\Gamma(z)\Gamma(-z)} = -z^2 \prod_{n=1}^{\infty} \left( 1 - \frac{z^2}{n^2} \right).
$$

ここで、$\sin z$ (VI, p. 287, th. 2) のオイラー展開は次のことを示します。

$$
z \prod_{n=1}^{\infty} \left( 1 - \frac{z^2}{n^2} \right) = \frac{1}{\pi} \sin \pi z;
$$

VII、p. 315 の関数方程式 (4) を考慮すると、次のことがわかります。

#### 命題 1 {#fvr-vii-s2-prop-1 .statement tag=08JB}

あらゆるコンプレックス $z$ に対して、人は

$$
\frac{1}{\Gamma(z)\Gamma(1-z)} = \frac{1}{\pi} \sin \pi z
$$

(補語関係)。

#### 系 {#fvr-vii-s2-n2-cor-1 .statement tag=08JC}

実数 $t$ ごとに、

$$
|\Gamma(it)| = \sqrt{\frac{\pi}{t \sinh \pi t}} \quad (t \neq 0)
$$

$$
|\Gamma(\frac{1}{2} + it)| = \sqrt{\frac{\pi}{\cosh \pi t}}.
$$

実際、(8) から $\Gamma(it)\Gamma(-it) = \frac{i\pi}{t \sin \pi it} = \frac{\pi}{t \sinh \pi t}$ が推定され、$\Gamma(-it) = \overline{\Gamma(it)}$ になります。同様に、(8) は次のようになります。

$$
\Gamma\left(\frac{1}{2} + it\right)\Gamma\left(\frac{1}{2} - it\right) = \frac{\pi}{\sin (\frac{\pi}{2} + \pi it)} = \frac{\pi}{\cos \pi it} = \frac{\pi}{\cosh \pi t},
$$

そして一人は持っています

$$
\Gamma\left(\frac{1}{2} - it\right) = \overline{\Gamma\left(\frac{1}{2} + it\right)}.
$$

ここで、$p$ を任意の整数 $> 0$ とし、積を考えます。

$$
f(z) = \Gamma\left(\frac{z+1}{p}\right) \Gamma\left(\frac{z+2}{p}\right) \ldots \Gamma\left(\frac{z+p}{p}\right).
$$

(3) (VII、p. 315) により、$z \neq -n \ (n \in \mathbf{N})$、$f(z)$ ごとに、積の極限になります。

$$
\frac{n^{(z+1)/p} n!}{\left(\frac{z+1}{p}\right) \left(\frac{z+1}{p} + 1\right) \ldots \left(\frac{z+1}{p} + n\right)}
$$

$$
\frac{n^{(z+2)/p} n!}{\left(\frac{z+2}{p}\right) \left(\frac{z+2}{p} + 1\right) \ldots \left(\frac{z+2}{p} + n\right)} \cdots
$$

$$
\ldots \frac{n^{(z+p)/p} n!}{\left(\frac{z+p}{p}\right) \left(\frac{z+p}{p} + 1\right) \ldots \left(\frac{z+p}{p} + n\right)}
$$

$$
= \frac{n^{z+(p+1)/2} p^{(n+1)p} (n!)^p}{(z+1)(z+2) \ldots (z+(n+1)p)}
$$

特に $f(0)$ は積の極限です

$$
\frac{n^{(p+1)/2} p^{(n+1)p} (n!)^p}{((n+1)p)!}
$$

ここから、$f(z)/f(0)$ は の極限であることがわかります。
$$
\frac{n^z ((n+1)p)!}{(z+1)(z+2)\ldots(z+(n+1)p)}
= z\ p^{-z} \left( \frac{n}{n+1} \right)^z \cdot \frac{((n+1)p)^z ((n+1)p)!}{z(z+1)(z+2)\ldots(z+(n+1)p)}
$$
これは、(3) (VII, p. 315) により、次のようになります。
$$
f(z) = f(0)\ z\ p^{-z}\ \Gamma(z).
$$
しかし、人は書くことができる
$$
f(0) = \prod_{k=1}^{p-1} \Gamma \left( \frac{k}{p} \right) = \prod_{k=1}^{p-1} \Gamma \left( 1 - \frac{k}{p} \right) = \sqrt{\prod_{k=1}^{p-1} \Gamma \left( \frac{k}{p} \right) \Gamma \left( 1 - \frac{k}{p} \right)}
$$
$f(0) > 0$以来。補数の関係は次のようになります。
$$
f(0) = \sqrt{\pi^{p-1} / \prod_{k=1}^{p-1} \sin \frac{k\pi}{p}}
$$
そして、右辺の積は $p/2^{p-1}$ (VI, p. 284, cor. 1) に等しいので、最終的に次のことがわかります。

#### 命題 2 {#fvr-vii-s2-prop-2 .statement tag=08JD}

*すべての複素数* $z$ *整数* $\leqslant 0$ ではありません *そしてすべての整数* $p > 0$ *1 つは*
$$
\Gamma \left( \frac{z}{p} \right) \Gamma \left( \frac{z+1}{p} \right) \ldots \Gamma \left( \frac{z+p-1}{p} \right) = (2\pi)^{(p-1)/2}\ p^{\frac{1}{2}-z}\ \Gamma(z)
$$
*(ルジャンドル＝ガウス乗法公式)*。

#### 命題 3 {#fvr-vii-s2-prop-3 .statement tag=08JE}

*すべての実質* $x > 0$ *1 つは持っています*
$$
\int_1^{x+1} \log \Gamma(t)\ dt = x(\log x - 1) + \frac{1}{2} \log 2\pi
$$
*(ラーベの積分)*。

まず、$x = 0$ に対して公式 (13) を確立します。 $\log \Gamma(x) \sim \log \frac{1}{x}$ と $x$ は 0 に近づく傾向があるため、積分 $\int_0^1 \log \Gamma(x)\ dx$ は収束します。さらに、写像 $\log \Gamma(x)$ は、$]0, 1]$ (VII、p. 310) で減少します。 $\alpha > 0$ごとに、人はこうして
$$
\frac{1}{n} \sum_{k=1}^q \log \Gamma \left( \frac{k}{n} \right) \leqslant \int_0^\alpha \log \Gamma(x)\ dx,
$$

$q$ は最大の整数であるため、$q/n \leqslant \alpha$ になります。 $\int_0^\alpha \log \Gamma(x) dx$ は $\alpha$ で 0 になる傾向があり、$n$ が $+\infty$ になる傾向があるため、$\frac{1}{n} \sum_{k=q+1}^n \log \Gamma \left( \frac{k}{n} \right)$ も $\int_\alpha^1 \log \Gamma(x) dx$ になる傾向があるため (II、p. 57、提案 5)、次のようになります。

$$
\int_0^1 \log \Gamma(x) dx = \lim_{n \to \infty} \frac{1}{n} \sum_{k=1}^n \log \Gamma \left( \frac{k}{n} \right).
$$

しかし、(12) により、この公式の右辺は の極限になります。

$$
\frac{n-1}{2n} \log 2\pi - \frac{1}{2} \frac{\log n}{n},
$$

よって

$$
\int_0^1 \log \Gamma(x) dx = \frac{1}{2} \log 2\pi.
$$ (14)

次にアイデンティティから次のことを述べます

$$
\log \Gamma(x+1) = \log \Gamma(x) + \log x
$$

積分すると、$x > 0$ が推測されます。

$$
\int_0^x \log \Gamma(t+1) dt = \int_0^x \log \Gamma(t) dt + \int_0^x \log t dt.
$$

しかし、左辺の積分も $\int_1^{x+1} \log \Gamma(t) dt$ に等しくなります。したがって、(14) により、

$$
\int_1^{x+1} \log \Gamma(t) dt = \int_0^x \log t dt + \frac{1}{2} \log 2\pi = x (\log x - 1) + \frac{1}{2} \log 2\pi.
$$

### 3. スターリングの拡張

$x$ と $y$ を、負の実数の半軸上にない 2 つの複素数とします。 VII、p. 315 の公式 (3) により、対数に関して VII、p. 316 の規則に従って、$\log \Gamma(x) - \log \Gamma(y)$ は式の $2\pi i$ から極限を法として合同です。

$$
(x-y) \log n + \sum_{k=0}^n \left( \log(y+k) - \log(x+k) \right).
$$ (15)

$f(t) = \log(y+t) - \log(x+t)$ を入れましょう。オイラー・マクローリン和公式 (VI, p. 288) を写像 $f$ に適用します。

$$
f(0) + f(1) + \cdots + f(n) = \int_0^{n+1} f(t) dt - \frac{1}{2} (f(n+1) - f(0))
$$
$$
+ \sum_{k=1}^p \frac{b_{2k}}{(2k)!} \left( f^{(2k-1)}(n+1) - f^{(2k-1)}(0) \right) + T_p(n)
$$

と
$$
|T_p(n)| \leq \frac{4 e^{2\pi}}{(2\pi)^{2p+1}} \int_0^{n+1} |f^{(2p+1)}(u)|\ du.
$$
(16)

以来
$$
f^{(m)}(t) = (-1)^{m-1} (m-1)! \left( \frac{1}{(y+t)^m} - \frac{1}{(x+t)^m} \right),
$$
$k \geq 1$ については、$n$ が $+\infty$ になる傾向があるように、$f^{(2k-1)}(n+1)$ は 0 になる傾向があります。それは同じです
$$
f(n+1) = \log \left( 1 + \frac{y}{n+1} \right) - \log \left( 1 + \frac{x}{n+1} \right).
$$
さらに、1つは、
$$
\int_0^{n+1} \log(x+t)\ dt = (x+n+1)(\log(x+n+1)-1) - x(\log x - 1);
$$
$n$ は $+\infty$ になる傾向があるため、漸近展開します。
$$
(x+n)(\log(x+n)-1) = n \log n - n + x \log n + O \left( \frac{1}{n} \right).
$$
式 (15) に代入すると、$n$ が $+\infty$ になる傾向があるため、$T_p(n)$ は極限 $R_p(x,\ y)$ となり、次のように書けることが最終的にわかります。
$$
\log \Gamma(x) - g(x) \equiv \log \Gamma(y) - g(y) + R_p(x,\ y) \quad (\text{mod. } 2\pi i)
$$
置く上で
$$
g(x) = x \log x - x - \frac{1}{2} \log x + \sum_{k=1}^p \frac{b_{2k}}{2k(2k-1)} \frac{1}{x^{2k-1}}.
$$
(17)

ここで、$x$ と $y$ が両方とも関係 "$\mathscr{R}(z) \geq A$ または $|\mathscr{I}(z)| \geq A$" で定義される $\mathbf{C}$ の部分集合 $\mathbf{H}_A$ にあると仮定して、(16) を使用して $R_p(x,\ y)$ の境界を評価します。 $A$ は任意の数 $> 0$ です (図 2)。この目的のために、$x = s + it$ と $s > A$ の場合、$u > 0$ ごとに $|x+u| \geq A+u$ があり、その結果、
$$
\int_0^{n+1} \frac{du}{|x+u|^{2p+1}} \leq \int_0^\infty \frac{du}{(A+u)^{2p+1}} = \frac{1}{2pA^{2p}}.
$$
同様に、$|t| \geq A$ の場合、すべての実数 $u$、よってに対して $|x+u| = |s+u+it| \geq \sqrt{A^2 + (s+u)^2}$ が得られます。
$$
\int_0^{n+1} \frac{du}{|x+u|^{2p+1}} \leq \int_{-\infty}^{+\infty} \frac{du}{(A^2 + u^2)^{p+1/2}} = \frac{2}{A^{2p}} \int_0^\infty \frac{dv}{(1+v^2)^{p+1/2}}.
$$
したがって、$x$ と $y$ が $\mathbf{H}_A$ にあるとき、
$$
|R_p(x,\ y)| \leq \frac{C_p}{A^{2p}}
$$

![t、s とラベル付けされた軸と領域 H_A、A、-A、0 を示す複素平面図式](図 2)

ここで、C_p は p にのみ依存します。ここで、集合 H_A を基底とするフィルターを $\mathfrak{F}$ とします。コーシー基準は、フィルター $\mathfrak{F}$、写像 $\log \Gamma(z) - g(z)$ が有限極限 $\delta$ (モジュロ $2\pi i$) を持ち、$\omega(z) = \max(\mathscr{R}(z), |\mathscr{I}(z)|)$ を置くと、

$$
\log \Gamma(z) - g(z) - \delta \equiv O \left( \frac{1}{(\omega(z))^{2p}} \right) \quad (\text{mod. } 2\pi i).
$$

x 実数および > 0 の場合、$\Gamma(x) > 0$ があり、$g(x)$ が実数であるため、$\delta$ が実数で、1 つが実数であると仮定できます。

$$
\log \Gamma(x) = g(x) + \delta + O \left( \frac{1}{x^{2p}} \right).
$$

ここで、定数 $\delta$ の値を prop によって推定します。 VII、p. 318 のうち 2 つは $p = 2$ に申請しましたが、1 つは実際には $x$ で $+\infty$ になる傾向があります

$$
\begin{align*}
&\frac{x-1}{2} \log \frac{x}{2} - \frac{x}{2} + \frac{x}{2} \log \frac{x+1}{2} - \frac{x+1}{2} + 2\delta \\
&\qquad = x \log x - x - \frac{1}{2} \log x + (\frac{1}{2} - x) \log 2 + \frac{1}{2} \log 2\pi + \delta + o(1)
\end{align*}
$$

そこから$\delta = \frac{1}{2} \log 2\pi$ と容易に推測できます。最終的には次のような結果が得られます。

#### 命題 4 {#fvr-vii-s2-prop-4 .statement tag=08JF}

*フィルター $\mathfrak{F}$ に沿って (整数 $p \geqslant 1$ ごとに) 漸近展開*

$$
\log \Gamma(z) \equiv z \log z - z - \frac{1}{2} \log z + \frac{1}{2} \log 2\pi
+ \sum_{k=1}^{p} \frac{b_{2k}}{2k(2k-1)} \frac{1}{z^{2k-1}} + O \left( \frac{1}{(\omega(z))^{2p}} \right) \quad (\text{mod. } 2\pi i)
$$

*(スターリングの拡張)*。

#### 系 {#fvr-vii-s2-n3-cor-1 .statement tag=08JG}

*フィルター $\mathfrak{F}$ に沿って *

$$
\Gamma(z) \sim \sqrt{2\pi} \exp(z \log z - z - \frac{1}{2} \log z).
$$

特に、$x$ の実数傾向については、$+\infty$ 公式 (20) と書くことができます。

$$
\Gamma(x) \sim \sqrt{2\pi} \, x^{x-1/2} e^{-x},
$$

よって、整数 $n$ は $+\infty$ になる傾向があるため、

$$
n! \sim \sqrt{2\pi} \, n^{n+1/2} \, e^{-n}
$$

(*cf.* V、p. 244)。

これから多くの公式を導き出すことができます。たとえば、複素数 $\alpha$ と整数 $n$ ごとに、$n$ が $+\infty$ になる傾向があるため、次のようになります。

$$
\frac{\Gamma(n+\alpha)}{\Gamma(n)} \sim n^{\alpha} \quad (= e^{\alpha \log n}).
$$

同様に、整数 $\leqslant 0$ ではなく、複素数 $a$ ごとに、

$$
a(a+1)(a+2)\ldots(a+n) = \frac{\Gamma(n+a+1)}{\Gamma(a)} \sim \frac{\sqrt{2\pi}}{\Gamma(a)} \, n^{n+a+1/2} \, e^n
$$

そして、整数 $\geqslant 0$ ではなく、複素数 $a$ ごとに

$$
\binom{a}{n} = \frac{(-1)^n}{\Gamma(-a)} \frac{\Gamma(n-a)}{\Gamma(n+1)} \sim \frac{(-1)^n}{\Gamma(-a)} \, n^{-a-1}.
$$

最後に、すべての実定数 $k > 1$ について、

$$
\binom{kn}{n} = \frac{\Gamma(kn+1)}{\Gamma(n+1) \Gamma((k-1)n+1)} \sim \sqrt{\frac{k}{2\pi(k-1)n}} \left( \frac{k^k}{(k-1)^{k-1}} \right)^n.
$$

同じ議論は、次の類似の命題につながります。

#### 命題 5 {#fvr-vii-s2-prop-5 .statement tag=08JH}

フィルター $\mathfrak{F}$ に沿って (整数 $p \geqslant 1$ ごとに) 漸近展開します。

$$
\frac{\Gamma'(z)}{\Gamma(z)} = \log z - \frac{1}{2z} - \sum_{k=1}^{p} \frac{b_{2k}}{2k} \frac{1}{z^{2k}} + O \left( \frac{1}{(\omega(z))^{2p+1}} \right).
$$

プロップの代わりに。 VII、p. 318 のうち 2 つ、1 つは公式を使用します

$$
\int_{x}^{x+1} \frac{\Gamma'(t)}{\Gamma(t)} \, dt = \log \Gamma(x+1) - \log \Gamma(x) = \log x
$$

位数 ～ 決定するには定数が入ります。

### 練習問題 {#fvr-vii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
