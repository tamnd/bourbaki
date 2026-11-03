---
book: top
book_title: General Topology
chapter: IV
chapter_title: Real Numbers
section: 8
section_title: Usual expansions of real numbers; the power of R
lang: ja
source: top-i-iv
book_pages: 373-377
pdf_pages: 0379-0383, 0407-0411
extraction: ocr
subsections:
    - "no": 1
      title: APPROXIMATIONS TO A REAL NUMBER
      page: 373
      pdf_page: 379
    - "no": 2
      title: EXPANSIONS OF REAL NUMBERS RELATIVE TO A BASE SEQUENCE
      page: 373
      pdf_page: 379
    - "no": 3
      title: DEFINITION OF A REAL NUMBER BY MEANS OF ITS EXPANSION
      page: 374
      pdf_page: 380
    - "no": 4
      title: COMPARISON OF EXPANSIONS
      page: 376
      pdf_page: 382
    - "no": 5
      title: EXPANSIONS TO BASE A
      page: 376
      pdf_page: 382
    - "no": 6
      title: THE POWER OF R
      page: 377
      pdf_page: 383
statements: 3
exercises: 17
content_sha256: f456a2433bbddcfbf397cf93d4a25f62a5d242bd3eaa273b83a4e32dac8cb760
translated_from: content/en/top/IV/08_s8_usual_expansions_of_real_numbers_the.md
translation_method: google
source_content_sha256: fc201404a7a205db6f15d21fa9d01ef19669eb40041bcaa87ccd2d1c2e452490
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 20cb334fab7635ca9826ce4216d800202975cc2206b098f0bcff15ab6e321027
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 8. 実数の通常の拡張。 Rの冪

### 1. 実数への近似

#### 定義 1 {#top-iv-s8-def-1 .statement tag=0BUG}

数 $\varepsilon > 0$ とすると、$|x - r| \leq \varepsilon$ の場合、実数 $r$ は $\varepsilon$ から実数 $x$ 以内の近似値であると言われます。 $r$ は、$r \leq x$ の場合は欠陥による近似値、$r \geq x$ の場合は過剰による近似値であると言われます。

$A$を$\mathbf{R}$の密な部分集合とします。それぞれの $x \in \mathbf{R}$ とそれぞれの $\varepsilon > 0$ について、区間 $]x - \varepsilon, x[$ (それぞれ $]x, x + \varepsilon[$) から、$\varepsilon$ 所属から $A$ までの$x$ までの欠陥 (それぞれ過剰) による近似があります。 含む $A$ のうち少なくとも 1 つの点。ここで、数 $> 0$ の特定の真に減少する数列 $(\varepsilon_n)$ が 0 に向かう傾向があると考え、$r_n$ が $\varepsilon_n$ 以内で $x$ の近似である場合、数列 $(r_n)$ は次のようになります。 $x$ は極限は $n$ として無限大になる傾向があります。

$A$ が加法群 $\mathbf{R}$ の部分群で、$\varepsilon_n$ から属する $A$ に制限する場合、$x \in \mathbf{R}$ 数列ごとに正規に定義するを設定できます。欠陥による$x$への近似の$(r_n)$、所属から$A$。

アルキメデスの公理 (§ 2, no. 1, 定理 1) によれば、整数 $p$ の集合により、$p \varepsilon_n \leq x$ は最大の元 $p_n$ となります。他の語には、次のような固有の整数 $p_n$ があります。

$$
p_n \varepsilon_n \leq x < (p_n + 1) \varepsilon_n.
$$

$|x - p_n \varepsilon_n| \leq \varepsilon_n$ なので、$p_n \varepsilon_n$ は欠陥による $x$ から $\varepsilon_n$ 以内、属するから仮定による $A$ の近似であることがわかります。同様に、$(p_n + 1) \varepsilon_n$ は、$x$ から $\varepsilon_n$ までの超過分、所属から $A$ までの近似であり、2 つの数列 $(p_n \varepsilon_n)$ と $((p_n + 1) \varepsilon_n)$ は、極限として $x$ を持ちます。

### 2. 基底数列に対する実数の拡張

$(d_n)$ が整数の真に増加する数列であり、$d_0 = 1$ と $d_n$ が $n \geq 1$ に対して $d_{n-1}$ の倍数である場合の $\varepsilon_n = 1/d_n$ の場合を極限で勉強してみます。 $a_n = d_n / d_{n-1}$ ($n \geq 1$) としましょう: $a_n$ は整数 $> 1$ です。この場合、欠陥$r_n = p_n / d_n$による近似値の数列は増加する、$p_n$は$p_n / d_n \leq x$となる最大の整数です。しかし、私たちは持っています

$$
\frac{p_{n-1}}{d_{n-1}} = \frac{p_{n-1} a_n}{d_n} \leq x < \frac{p_{n-1} + 1}{d_{n-1}} = \frac{p_{n-1} a_n + a_n}{d_n}
$$

したがって $a_n p_{n-1} \leq p_n < a_n p_{n-1} + a_n$、したがって $r_{n-1} \leq r_n \leq x$ になります。しましょう
$$
p_n = a_n p_{n-1} + u_n;
$$
次に $0 \leq u_n - a_n$ ですが、$u_n$ は整数なので、これは $0 \leq u_n \leq a_n - 1$ と同等です。したがって、
$$
r_n = r_{n-1} + \frac{u_n}{d_n} = p_0 + \sum_{k=1}^n \frac{u_k}{d_k},
$$
そして、$x = \lim_{n \to \infty} r_n$以降、
$$
x = p_0 + \sum_{n=1}^\infty \frac{u_n}{d_n}.
$$
和が$x$である(4)の右辺の系列を、基底数列$(d_n)$に対する$x$の展開といいます。 係数 $u_n$ はすべて $\geq 0$ です。 $p_0$ は、定義により、最大の整数 $p$ となり、$p \leq x$ になります。これは、$x$ の積分部分と呼ばれ、多くの場合、$[x]$ で表されます。

### 3. 拡張による実数の定義

逆に、$0 \leq v_n \leq a_n - 1$ となる整数の整数 $q_0$ と数列 $(v_n)$ ($n \geq 1$) が与えられたとします。すべての $n$ に対して $p_0 = q_0$ と $u_n = v_n$ となる展開 (4) となる数 $x$ があるかどうかを尋ねます。そのような数が存在する場合、それは次と等しいため一意です。
$$
q_0 + \sum_{n=1}^\infty \frac{v_n}{d_n}.
$$
それぞれの整数 $m > 0$ について、(比較原理により)
$$
\sum_{n=m+1}^\infty \frac{v_n}{d_n} \leq \sum_{n=m+1}^\infty \frac{a_n - 1}{d_n} = \sum_{n=m+1}^\infty \left( \frac{1}{d_{n-1}} - \frac{1}{d_n} \right) = \frac{1}{d_m}
$$
そして、左端と右端の項は、各 $n > m$ について $v_n = a_n - 1$ (§ 7, no. 1, 定理 2) の場合にのみ等しくなります。したがって、一般項が $\frac{v_n}{d_n}$ である系列は収束します。さらに、$x = q_0 + \sum_{n=1}^\infty \frac{v_n}{d_n}$ の場合、
$$
s_m = q_0 + \sum_{n=1}^m \frac{v_n}{d_n} \leq x \leq s_m + \frac{1}{d_m}
$$
$n > m$ ごとに $v_n = a_n - 1$ の場合のみ、$x = s_m + \frac{1}{d_m}$ となります。 $s_m$ は分母が $d_m$ の分数であるため、欠陥による $1/d_m$ 以内の$r_m$ から $x$ への近似は、$s_m$ または $s_m + \frac{1}{d_m}$ に等しくなります。後者の選択肢は、すべての $n > m$ に対して $v_n = a_n - 1$ の場合にのみ発生します。したがって:
(i) $v_n < a_n - 1$ のような $n$ の値の *無限* が存在します。すると、 系列 $q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n}$ は、その和 $x$ の展開と同一になります。
(ii) $n > m$ の場合は必ず $v_n = a_n - 1$ となり、($m > 0$ の場合は) $v_m < a_m - 1$ となる整数 $m \geq 0$ があります。その場合、系列 $q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n}$ の和 $x$ は有理数数に等しいです
$$
q_0 + \sum_{n=1}^{m} \frac{v_n}{d_n} + \frac{1}{d_m}
$$
これは形 $k/d_m$ ($k$ 整数) です。 $x$ の *展開* は系列 (5) と同一であり、添字 $> m$ を持つすべての項は零です。このような展開は、*終了*、または *終了* と言われます。 系列
$$
q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n} = q_0 + \sum_{n=1}^{m} \frac{v_n}{d_n} + \sum_{n=m+1}^{\infty} \frac{a_n - 1}{d_n}
$$
は、数 $x$ の *不適切な拡張* と呼ばれます。

逆に、$x$ を、$n$ の一部の値について、分母が $d_n$ の分数の形で書ける有理数数とします。 $m$ を最小の整数とし、$x$ が形 $k/d_m$ ($k$ 整数) となるようにします。 $n < m$ と $r_m = x$ には $r_n < x$ があるため、$x$ の展開は形 (5) となり、$x$ は (6) によって与えられる不適切な展開になります。さらに、この不適切な展開は *独特* です。

既約形 $p/q$ で書かれた有理数数は、$q$ *割る* $d_n$ (したがって、数 $m$ は最小のとなる) の場合に限り、分母が $d_n$ の分数と等しくなります。 整数 $n$ は $q$ 割る $d_n$ となります）。 *すべての有理数数* がこの性質 (適切に選択された $n$ の場合) になる可能性があります。これは、すべての整数 $> 0$ 割るの一部の $d_n$ の場合にのみ当てはまります。たとえば、$d_n = n!$ の場合、 $d_n$ にこの性質がある場合、数列 $(d_n)$ に対する拡張が終了する場合に限り、数は合理的です。

要約すると、最初の項 $q_0$ が任意の整数であり、項 $v_n (n \geq 1)$ が $0 \leq v_n \leq a_n - 1$ となるようなすべての数列 $s$ は、$q_0 + \sum_{n=1}^{\infty} \frac{v_n}{d_n}$ に等しい実数に対応します。 $I_n$ が $\mathbf{N}$ の間隔 $[0, a_n - 1]$ を表す場合、$X = \mathbf{Z} \times \prod_{n=1}^{\infty} I_n$ の *上* 実線 $\mathbf{R}$ へのマッピング $\varphi$ を定義します。さらに、$x \in \mathbf{R}$ が与えられている方程式 $\varphi(s) = x$ は、$x$ が分母 $d_n$ (一部の $n$) の分数でない場合は *1 つの* 解があり、それ以外の場合は *2* つの* 解があります。

### 4. 拡張の比較

2 つの異なる実数 $x$ と $y$ の展開がわかっていれば、$x < y$ であっても $x > y$ であっても決定するができます。

$x = p_0 + \sum_{n=1}^{\infty} u_n / d_n$、$y = q_0 + \sum_{n=1}^{\infty} v_n / d_n$ を $x$ と $y$ の展開とします。 $p_0 < q_0$ なら $x < y$、

$$
p_0 \leq x < p_0 + 1 \leq q_0 \leq y.
$$

より一般的には、$1 \leq n \leq m$ に対して $p_0 = q_0$ と $u_n = v_n$ が、$u_m < v_m$ であると仮定します。もし

$$
r_n = p_0 + \sum_{k=1}^{n} u_k / d_k, \quad s_n = q_0 + \sum_{k=1}^{n} v_k / d_k,
$$

次に、$n < m$ に対して $r_n = s_n$、そして $u_m + 1 \leq v_m$ から$r_m + \frac{1}{d_m} \leq s_m$;しかし $r_m \leq x < r_m + \frac{1}{d_m} \leq s_m \leq y$ なので、また $x < y$ になります。他の語、$x$ と $y$ の *位数は、それぞれの拡張* の最初の 2 つの異なる項の位数と同じです。

その結果、$n < m$ に対して $p_0 = q_0$ と $u_n = v_n$ があれば、各数 $z$ 所属を終点 $x$ と $y$ で閉じた区間に展開する最初の $m$ 項が得られます。 $x$と$y$の拡張のものと*同じ*です。

この場合、$|y - x| \leq \frac{1}{d_{m-1}}$ であることにも注意してください。 $\mathbf{Z}$ と区間 $I_n$ に *離散* 位相を与えると、上記で定義された写像 $\varphi$ は *積空間* $X$ 上で *連続* になります。

### 5. 基底 a への拡張

最も重要な基底数列は $d_n = a^n$ のもので、$a$ は整数 $> 1$ です。 $a$ は、対応する拡張の *基底数* (または単に *基底*) であると言われます。数値計算では、*10 進展開* と呼ばれる基底 10 への展開が使用されます。 基底 2 (*二項* 拡張) および基底 3 (*三項* 拡張) への拡張もよく使用されます。

欠陥による近似値 $r_n$ から数 $x \geq 0$ を基底 $a$ に拡張して表すために、次の象徴性が使用されます。各整数 $u$ は、$0 \leq u \leq a - 1$ が特定の符号で示されるようになります。もし

$$
r_n = p_0 + \sum_{k=1}^{n} \frac{u_k}{d_k},
$$

まず、これらの記号を使って、整数 $p_0 = [x] \geq 0$ (*集合理論*, 章 III, § 5, no. 7) の表現から基底 $a$ を書き留めてから、点 (「10 進数」) を入力します。 点") そして、数 $u_1, u_2, \ldots, u_n$ を表す記号を連続して書きます。このようにして得られた記号が S である場合、言葉を乱用して $x = S...$ と書くのが通例です。このような関係は、右辺が欠陥による $1/a^n$ 以内での $x$ の近似であることを示す方法の省略形にすぎないことを、きっぱりと理解する必要があります。

負の数の場合、確立された用法は異なります。上記の記号で $x' = -x > 0$ への近似値を書き、その前に記号「—」を付けます。したがって、それは、そのように示される超過分によって $x$ から $1/a^n$ 以内に近似されることになります。

この使用法には数値計算において不都合があります。負の対数の記法では、積分値部分の上にバーを置き、書かれた数の負の値と等しいことを示すために、正の数と同じ記号が採用されています。

### 6. Rの冪

$\mathbf{R} = \bigcup_{n \in \mathbf{Z}} [n, n+1[$ があり、すべての区間 $[n, n+1[$ は $[0, 1[$ と同等です。 $[0, 1[$ は無限大の集合であるため、$\mathbf{R}$ は区間 $[0, 1[$ と等価であることになります。 区間 $[0, 1[$ の数の二項展開を考慮することで、この区間がすべての数列 $(u_n)$ の集合 S と等価であり、各項が 0 または 1 に等しいことを示します。

まず、数列 $(u_n)$ の S からなるの部分集合 $S'$ は、$n$ の値の無限大に対して $u_n = 0$ と等価です。一方、S の $S'$ の補数 $S''$ は、分母 $2^n$ の分数に等しい有理数数のすべての不適切な展開の集合と等価です。これら $\mathbf{Q}$ の数形部分集合は、したがって、そのうちの集合は可算であり、したがって $S''$ も同様です。 $S'$ は無限であるため、S と等価であり、その結果が得られます。

現在、S は $\mathfrak{P}(\mathbf{N})$ と等価です。なぜなら、$\mathfrak{P}(\mathbf{N})$の定義する全単射をSに写像ずつ、$\mathbf{N}$の部分集合 Aを数列 $(u_n)$として、$n \in A$であれば$u_n = 0$が成り立つからです。 $n \notin CA$なら$u_n = 1$。したがって、次のことを証明しました。

#### 定理 1 (カントール) {#top-iv-s8-thm-1 .statement tag=0BUH}

* 実数の集合は、可算無限大集合のすべての部分集合の集合と等価です。

#### 系 {#top-iv-s8-n6-cor-1 .statement tag=0BUI}

* 実数の集合は、可算数集合の基数より厳密に大きい基数を持ちます。*

$\mathbf{R}$ と同等の集合は、連続体の冪を持つと言われています。 § 4, no. 1 の命題 1 までに、含む 1 つ以上の点が含まれるすべての区間には、連続体の冪が含まれます。繰り返しになりますが、$\mathbf{R}$ の可算部分集合の補数は、特に連続体の冪を持ち、すべての無理数数の *集合は連続体の冪を持ちます。

### 練習問題 {#top-iv-s8-exercises}

[§ 8 に対して練習問題](exercises/s8/)を参照してください。
