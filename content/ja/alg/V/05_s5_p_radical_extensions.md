---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 5
section_title: p-radical extensions
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.24-A V.26, A V.150-A V.151
pdf_pages: 0138-0140, 0264-0265
extraction: ocr
subsections:
    - "no": 1
      title: p-radical elements
      page: 24
      pdf_page: 138
    - "no": 2
      title: pradical extensions
      page: 25
      pdf_page: 139
statements: 8
exercises: 3
content_sha256: 15956f989000205ad2735d77e14f0bebe149c44e412bce5c01c8185bdb342a0b
translated_from: content/en/alg/V/05_s5_p_radical_extensions.md
translation_method: google
source_content_sha256: 3693c7ad10eed43de9af13fff4d3447ffd7fc25ca8cc3c3bf9505041a61ff985
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 8794bd7a1b6395b32413bf6c773db39f1d114f90a8d8a2f28a754734df9a8fcc
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 5。 *p*-ラジカル拡張機能

*この段落全体を通じて、文字 p は 1 または素数数のいずれかである整数を表します。考慮されたすべての体は、特徴的な指数 p.この段落に記載されているすべての結果は、$p = 1$ の場合は自明です。*

### 1. p-ラジカル元

#### 定義 1 {#alg-v-s5-def-1 .statement tag=06IZ}

*K を K の体および E 拡大とします。$x^{p^m} \in K$ となるような整数 $m \geq 0$ が存在する場合、E の n 元 x は K に対して p ラジカルであると言われます。これら整数のうち最小のものは、x の高さ (K 以上) と呼ばれます。*

#### 命題 1 {#alg-v-s5-prop-1 .statement tag=06J0}

*E を体 K の拡大とし、x を K 上の高さ e の p ラジカル元とします。 $a = x^{p^e}$を入れます。次に、$a \in K$ となり、K 上の x の最小多項式は $X^{p^e} - a$ になります。さらに、$[K(x):K] = p^e$ が得られます。*

多項式 $X^{p^e} - a$ が $K[X]$ で既約であることを証明すれば十分です。 x の高さ定義により、$a \notin K^p$ が得られ、補題から命題が続きます。

#### 補題 1 {#alg-v-s5-lem-1 .statement tag=06J1}

*K を体とし、$a \notin K^p$ となるような K の元とします。次に、すべての整数 $e \geq 0$ について、多項式 $f(X) = X^{p^e} - a$ は $K[X]$ で既約です。*

$\Omega$ を $K$ の代数閉包とし、b を $\Omega$ の元 $a^{p^{-e}}$ とします。 $K$ 上の b の最小多項式を g で表します。 $f(X) = (X - b)^{p^e}$ があるため、$K[X]$ の既約多項式はすべて、割る $f$ は b を根として認め、したがって g に等しくなります。したがって、 (*IV*, p. 13, 提案 13) 整数 $q \geq 1$ が存在し、そのような $f = g^q$; q 割る次数 $p^e$ of $f$ から、$0 \leq e' \leq e$ と $q = p^{e'}$ となる整数 $e'$ が存在します。 c が g の定数項である場合、$-a = c^q$ になります。 a は $K^p$ にないと仮定したので、$q = 1$、つまり $f = g$ がなければならないので、補題が続きます。

### 2. 根本的な拡張

#### 定義 2 {#alg-v-s5-def-2 .statement tag=06J2}

E を体 K の拡大とします。E のすべての元が K 上で p 基である場合、E は p 基 $^1$ (K 上) であると言えます。この場合、E の元の高さのうち集合が上で制限されているとき、E は有限の高さであると言われますそして E の高さをその元の高さの最大値と呼びます。

完全体 (特に標数 0 の体) のすべての p ラジカル拡張は自明であることに注意してください。

K を体とします。K の高さ 0 の p ラジカル拡張は自明な拡大です。 K のすべての p ラジカル拡張は代数的です。 E が K の p ラジカル拡張であり、F が E の p ラジカル拡張である場合、F は K の p ラジカル拡張です。つまり、任意の $x \in F$ が与えられた場合、$x^{p^m} \in E$ および整数 $n \geq 0$ が $(x^{p^m})^{p^n} \in K$ となるような整数 $m \geq 0$ が存在します。 $x^{p^m + n} \in K$。

#### 命題 2 {#alg-v-s5-prop-2 .statement tag=06J3}

E を体 K の拡大とします。すべての整数 $n \geq 0$ について、$E_n$ を E の元の集合とし、K よりも高さ $\leq n$ $p\text{-radical}$ を$E_r$ とします。 K 上で p ラジカルである E のすべての元の集合になります。その場合、$(E_n)_{n \geq 0}$ は、和集合が $E_\infty$ である E の部分拡張の昇順数列であり、$E_r$ は、K に含まれる K の p ラジカル拡張である最大のです。 E.

それぞれの整数 $n \geq 0$ 集合 $E_n$ は、$x^{p^n} \in K$ となるような E のすべての元 $x$ で構成されます。 写像 $x \mapsto x^{p^n}$ は体 E の自己準同型であるため、$E_n$ は E の部分拡張であると推定されます。 数列 $(E_n)_{n \geq 0}$ は昇順であり、和集合 $E_r$ であるため、 $E_r$ は E の部分拡張です (V、p. 11、提案 3)。 $E_r$ が K の p ラジカル拡張であり、$E_r$ 含むが K に対して p ラジカルである E のすべての部分拡張であることは明らかです。

#### 系 {#alg-v-s5-n2-cor-1 .statement tag=06J4}

体 K の拡大 E が K 上で $p\text{-radical}$ 元の集合によって生成される場合、それは K 上で p-ラジカルです。

$E_r$ は E の部分拡張であり、仮定 $E = K(E_\infty)$ よって $E = E_r$ によるものです。したがって、E は K の p ラジカル拡張です。

命題 2 の条件では、$E_r$ は E における K の相対的な $p\text{-radical}$ 閉包であると言われます。

提案 2 を特に E が K の代数閉拡大である場合に適用します。この場合、E は完全で、すべての $n \geq 0$ に対して $E_n = K^{p^{-n}}$ が得られます。 この場合、K 上の p-ラジカルである E の元の $K^{p^{-\infty}}$ 集合によって表されます。それは E の部分体で、E の部分体の昇順数列 $(K^{p^{-n}})_{n > 0}$ の和集合です。 提案 2 により、$K^{p^{-\infty}}$ は K 上の p-ラジカルである E の最大の部分拡張です。 V, p. 6, $K^{p^{-\infty}}$ の提案 3 は K の完全閉包であり、E 含む K の最小の完全部分体でもあります。 K が完全な場合、すべての n に対して明らかに $K = K^{p^{-n}} = K^{p^{-\infty}}$ が得られます。 K が不完全であれば、$K \neq K^P$、よってになります。

$^1$ p ラジカル拡張は、純粋に分離不可能な拡大または根基拡大とも呼ばれます。

$$
K^{p^{-n}} \neq (K^p)^{p^{-n}} = K^{p^{-(n-1)}}
$$
$n \geq 1$の場合。 E の部分体 $K^{p^{-n}}$ はペアごとに区別され、$K^{p^{-\infty}}$ は K の無限次数の代数拡大になります。

#### 命題 3 {#alg-v-s5-prop-3 .statement tag=06J5}

— K を体、K の p 基である E 拡大体、および K の完全体 F への K の $u$ 準同型とする。すると、$u$ に広がる F への E の一意な準同型 $v$ が存在する。

$E_n$ を、K 上の高さ $\leq n$ の p 根である E の元の集合とします。 提案 2 により、体 E は、部分体の昇順数列 $(E_n)_{n \geq 0}$ の和集合です。 $v$ を、$u$ を拡張した E から F への準同型射とします。任意の $x \in E_n$ に対して $x^{p^n} \in K$ があり、そこから $v(x)^{p^n} = v(x^{p^n}) = u(x^{p^n})$ が得られます。したがって、すべての $n \geq 0$ とすべての $x \in E_n$ に対して $v(x) = u(x^{p^n})^{p^{-n}}$ があり、そこから $u$ の E への拡張の一意性が得られます。

$n$ を正の整数とします。任意の $x \in E_n$ に対して $x^{p^n} \in K$ があり、F が完全なので、F の定義する元 $v_n(x)$ を $v_n(x) = u(x^{p^n})^{p^{-n}}$ で求めることができます。 $v_n$ は F の $E_n$ の準同型であり、$v_0 = u$ であり、$E_n$ の $v_{n+1}$ 誘導する $v_n$ であることは明らかです。したがって、すべての $n \geq 0$ に対して $E_n$ に $v_n$ を誘導する F への E の準同型 $v$ が存在し、特に $E_0 = K$ の $v_0 = u$ と一致します。

#### 系 {#alg-v-s5-n2-cor-2 .statement tag=06J6}

— 体 K の拡大 E が K の完全閉包であるためには、それが K の p ラジカル拡張であること、および体 E が完全であることが必要かつ十分です。

$p = 1$ の場合、系は自明です。次に、$p \neq 1$ と仮定します。記載されている条件は、V、p. 5、Thまでに必要です。 3 ;これらは提案 3 によって十分です。

#### 命題 4 {#alg-v-s5-prop-4 .statement tag=06J7}

— E を、体 K の *有限* 次数の p 根拡張とします。その場合、$[E : K]$ は、K の標数指数 p の冪です。

E は K の有限次数の p ラジカル拡張であるため、$E = K(a_1, \ldots, a_m)$ のように、K 上の p ラジカルである E の元 $a_1, \ldots, a_m$ が存在します。 i を 1 から m の範囲内とする。 $a_i$ は $K(a_1, \ldots, a_{i-1})$ 上のなおさら p-ラジカルであるため、次数
$$
n_i = [K(a_1, \ldots, a_i) : K(a_1, \ldots, a_{i-1})]
$$
は p の冪 (V、p. 24、提案 1)。 V、p. 18、Thまでに$[E : K] = n_1 \ldots n_m$がございます。 2、よって結果。

### 練習問題 {#alg-v-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
