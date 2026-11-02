---
book: fvr
book_title: Functions of a Real Variable
chapter: I
chapter_title: DERIVATIVES
section: 3
section_title: DERIVATIVES OF HIGHER ORDER
lang: ja
source: fvr-i-vii
book_pages: 20-23, 39-45
pdf_pages: 0035-0038, 0054-0060
extraction: ocr
subsections:
    - "no": 1
      title: DERIVATIVES OF ORDER $n$
      page: 20
      pdf_page: 35
    - "no": 2
      title: TAYLOR'S FORMULA
      page: 21
      pdf_page: 36
statements: 8
exercises: 18
content_sha256: e929058be4b170de6ea603ed4a7b46d225259f2cbf6b1026e8e465570fe79b3a
translated_from: content/en/fvr/I/03_s3_derivatives_of_higher_order.md
translation_method: google
source_content_sha256: 699d9104f5cbf89e2acd64f1b847b3d92cb37baff716a8c7f28471e185a92054
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 8f37591d190688b21e9c01184e7d05ce18b08a1531f6d4a31d569f03d4d28cf3
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。上位位数のデリバティブ

### 1. 位数 $n$ の導関数

$f$ を、区間 $I$ で定義され、連続で微分可能な実数変数のベクトル写像とします。導関数 $f'$ が点 $x_0 \in I$ の近傍 ($I$ に関して) に存在し、 点 $x_0$ で微分可能である場合、その導関数は点 $x_0$ での $f$ の *二次導関数* と呼ばれ、は$f''(x_0)$または$D^2f(x_0)$で表されます。この二次導関数が $I$ の点ごとに存在する場合 (これは、$f'$ が存在し、$I$ で連続であることを意味します)、$x \mapsto f''(x)$ は $f''$ または $D^2f$ で示されるベクトル写像になります。 定義するも同様に、再帰的に $f$ の $n^{th}$ *導関数* (または位数* $n$ の *導関数) を$f^{(n)}$ または $D^n f$ で表します。 定義によると、点 $x_0 \in I$ での値は、点 $x_0$ での写像 $f^{(n-1)}$ の導関数です。この定義は、その導関数 $f^{(k)}$ の *すべて* が存在することを前提としています。 $I$ に対する $x_0$ の *近傍* 上の位数 $k \leq n - 1$ と、点 $x_0$ での $f^{(n-1)}$ の微分可能性。

この点 (この区間でそれぞれ) で $n^{th}$ 導関数が認められる場合、$f$ は点 $x_0$ (それぞれ区間) で *n 回微分可能*であると言えます。 整数 $n > 0$ のそれぞれについて、$I$ 上の位数 $n$ の導関数が認められる場合、$f$ は $I$ で *無限微分可能*であると言われます。

$m$ の帰納法までに、次のことがわかります。

$$
D^m(D^n f) = D^{m+n} f.
$$

より正確には、(1) の 2 つの項のうちの 1 つが定義されると、もう 1 つも定義され、それに等しくなります。

#### 命題 1 {#fvr-i-s3-prop-1 .statement tag=084Y}

*ベクトル写像の集合は区間* $I \subset \mathbf{R}$ で定義され、 *特定のトポロジベクトル空間* $E$ で値を取り、 * $n^{th}$ * の導関数* $I$ を持ち、 * はベクトル空間は* $\mathbf{R}$、*そして* $f \mapsto D^n f$ *はこの空間の線形写像が線形写像のベクトル空間に* $I$ *から* $E$になります。

公式を証明する

$$
D^n(f + g) = D^n f + D^n g \tag{2}
$$
$$
D^n(fa) = D^n f . a \tag{3}
$$

$f$ と $g$ が $I$ ($a$ は定数) に $n^{th}$ 導関数がある場合、$n$ で帰納法によって計算されます。

#### 命題 2 (「ライプニッツ公式」) {#fvr-i-s3-prop-2 .statement tag=084Z}

*$E, F, G$ *3 つのトポロジカルベクトル空間を * $\mathbf{R}$、*および* $(x, y) \mapsto [x.y]$ * $E \times F$ * $G$ の *連続双線形写像とします。 *もし* $f$ *(resp.* $g$) *が区間* $I \subset \mathbf{R}$ で定義されている場合、 *その値を* $E$ *(resp.* $F$) *そして* $n^{th}$ * $I$ の派生* があります。 *その後* $[f.g]$ *は* $n^{th}$ *派生* $I$、*公式*によって与えられます

$$
D^n[f.g] = [f^{(n)}.g] + \binom{n}{1}[f^{(n-1)}.g'] + \cdots + \binom{n}{p}[f^{(n-p)}.g^{(p)}] + \cdots + [f.g^{(n)}]. \tag{4}
$$

公式 (4) は、$n$ で帰納法によって証明されます (二項式係数に関係 $\binom{n}{p} = \binom{n-1}{p} + \binom{n-1}{p-1}$ を使用)。

同様に、次の公式を検証できます (仮説は提案 2 と同じです)。

$$
[f^{(n)} . g] + (-1)^{n-1} [f . g^{(n)}] = D([f^{(n-1)} . g] - [f^{(n-2)} . g'] + \cdots + (-1)^{n-1} [f . g^{(n-1)}]).
$$

前述の命題は、区間で $n$ 回微分可能である写像について記述されています。 点で $n$ 回微分可能である写像に対する類似の命題を定式化するのは読者に任せます。

### 2. テイラーズ公式

$f$ を区間 $I \subset \mathbf{R}$ で定義されたベクトル写像とします。値は $\mathbf{R}$ に対する *正規化* 空間 $E$ です。 $f$ が点 $a \in I$ で導関数を持つということは、次のことを意味します。

$$
\lim_{x \to a,\ x \in I,\ x \neq a} \frac{f(x) - f(a) - f'(a)(x-a)}{x-a} = 0;
$$

または、そうでない場合、$f$ は、$a$ の近傍上の *線型* 写像 $f(a) + f'(a)(x-a)$ と「ほぼ等しい」と考えられます (*cf.* 章 V、この概念は一般的な方法で展開されています)。 点 $a$ における $f$ の導関数 $n^{th}$ 位数の存在は、$f$ が $x$* の次数 $n$ の * 多項式と「ほぼ等しい」のと同じ方法を伴うことがわかります。 $E$ の係数 (*Gen. Top.*、X、p. 315)、$a$ の近傍。正確に言うと:

#### 定理 1 {#fvr-i-s3-thm-1 .statement tag=0850}

*写像 $f$ に点 $a$ で $n^{th}$ 導関数がある場合*

$$
\lim_{x \to a,\ x \in I,\ x \neq a} \frac{f(x) - f(a) - f'(a)\frac{(x-a)}{1!} - \cdots - f^{(n)}(a)\frac{(x-a)^n}{n!}}{(x-a)^n} = 0.
$$

$n$の帰納法までに進みます。 定理は $n = 1$ に当てはまります。任意の $n$ に対して、帰納法の仮定によって、それを $f$ の導関数 $f'$ に適用できます。任意の $\varepsilon > 0$ に対して、次のような $h > 0$ が存在します。

$$
g(x) = f(x) - f(a) - f'(a)\frac{(x-a)}{1!} - f''(a)\frac{(x-a)^2}{2!} - \cdots - f^{(n)}(a)\frac{(x-a)^n}{n!}
$$

$|y-a| \leq h$ と $y \in I$ については、

$$
\|g'(y)\| = \left\| f'(y) - f'(a) - f''(a)\frac{(y-a)}{1!} - \cdots - f^{(n)}(a)\frac{(y-a)^{n-1}}{(n-1)!} \right\|
$$
$$
\leq \varepsilon\ |y-a|^{n-1}.
$$

平均値定理 (I, p. 15, th. 2) を区間にエンドポイント $a,\ x$ ($|x-a| \leq h$) からベクトル写像 $g$ に適用し、実数に適用します。 増加する写像は、$x > a$ の場合は $\varepsilon |y - a|^n / n$ に、$x < a$ の場合は $-\varepsilon |y - a|^n / n$ に等しい。したがって、$\|g(x)\| \leq \varepsilon |x - a|^n / n$ となり、定理が証明されます。

したがって、次のように書くことができます
$$
f(x) = f(a) + f'(a) \frac{(x - a)}{1!} + f''(a) \frac{(x - a)^2}{2!} + \cdots \\
+ f^{(n)}(a) \frac{(x - a)^n}{n!} + u(x) \frac{(x - a)^n}{n!}
$$
ここで、I に留まりながら、$x$ が $a$ に近づくと、$u(x)$ は 0 に近づきます。この公式は、点 $a$における位数* $n$の*テイラーの公式と呼ばれ、(8)の右辺は、写像の位数* $n$の*テイラー展開と呼ばれます。 $f$ 点 $a$。最後の項 $r_n(x) = u(x)(x - a)^n / n!$ は、位数 $n$ のテイラー 公式の *剰余* と呼ばれます。

$f$ が I 上で位数* $n + 1$ の*導関数を持つ場合、この $n + 1^{th}$ 導関数の項で $\|r_n(x)\|$ を、不特定の近傍だけでなく I のすべてについて推定できます。 $a$:

#### 命題 3 {#fvr-i-s3-prop-3 .statement tag=0851}

*I が $\|f^{(n+1)}(x)\| \leq M$ の場合、*
$$
\|r_n(x)\| \leq M \frac{|x - a|^{n+1}}{(n + 1)!}
$$
*オン* I。

確かに、公式は、I、p. 15 までの $n = 0$ に当てはまります。 2. $n$ の帰納法によって証明しましょう: 帰納法の仮定を $f'$ に適用すると、
$$
\|r'_n(y)\| \leq M \frac{|y - a|^n}{n!}
$$
ここから公式 (9) の後に平均値定理 (I, p. 23, th. 2) が続きます。

#### 系 {#fvr-i-s3-n2-cor-1 .statement tag=0852}

*$f$ が有限実数写像で、位数* $n + 1$ *on* I の場合、*そして * $m \leq f^{(n+1)}(x) \leq M$ *on* I の場合、*すべて* $x \geq a$ *in* I *1つは持っています*
$$
m \frac{(x - a)^{n+1}}{(n + 1)!} \leq r_n(x) \leq M \frac{(x - a)^{n+1}}{(n + 1)!}
$$
*そして 2 番目の項できないは、最初の * と等しくなります (*3 番目*) *〜でない限り* $f^{(n+1)}$ *は定数であり、* $m$ (それぞれ $M$) *区間* $[a, x]$ と等しくなります。

証明も同様に進みますが、適用番目。 I、p. 14 の 1 つ。

#### 注意 1 {#fvr-i-s3-n2-rem-1 .statement tag=0853}

証明ですでに気づいています。 1 $f$ が I 上で位数 $n$ の導関数を持つ場合、および次の場合
$$
f(x) = a_0 + a_1(x - a) + a_2(x - a)^2 + \cdots + a_n(x - a)^n + r_n(x)
$$
は、点 $a$ での位数 $n$ のテイラー展開であり、点 $a$ での $f'$ に対する位数 $n - 1$ のテイラー展開は次のようになります。
$$
f'(x) = a_1 + 2a_2(x - a) + \cdots + na_n(x - a)^{n-1} + r'_n(x).
$$

これは、$f$ の展開 (11) から*項ごとに微分*することによって得られると言います。

#### 注意 2 {#fvr-i-s3-n2-rem-2 .statement tag=0854}

同じ仮説を使用すると、(11) の係数 $a_i$ は関係によって再帰的に決定されます。

$$
a_0 = f(a)
$$
$$
a_1 = \lim_{x \to a} \frac{f(x) - f(a)}{x - a}
$$
$$
a_2 = \lim_{x \to a} \frac{f(x) - f(a) - a_1(x - a)}{(x - a)^2}
$$
$$
\ldots
$$
$$
a_n = \lim_{x \to a} \frac{f(x) - f(a) - a_1(x - a) - \cdots - a_{n-1}(x - a)^{n-1}}{(x - a)^n}.
$$

$a = 0$ 1 つの結論するの場合、特に、$f(x^p)$ ($p$ 整数 > 0) が 0 の近傍で位数 $pn$ の導関数を持つ場合、位数のテイラー展開になります。この写像の $pn$ は単に

$$
f(x^p) = a_0 + a_1 x^p + a_2 x^{2p} + \cdots + a_n x^{np} + r_n(x^p)
$$

ここで、$r_n(x^p)$ は展開の余り (*cf.* V, p. 222) です。

#### 注意 3 {#fvr-i-s3-n2-rem-3 .statement tag=0855}

位数 $n$ の導関数の定義と前述の結果は、複素変数の写像に直ちに一般化されます。ここではこの話題をこれ以上追及しません。これについては、この系列の後の本で詳しく説明します。

### 練習問題 {#fvr-i-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
