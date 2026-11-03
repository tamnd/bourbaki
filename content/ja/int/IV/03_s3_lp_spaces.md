---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 3
section_title: LP spaces
lang: ja
source: int-i-vi
book_pages: INT IV.18-INT IV.32, INT IV.120
pdf_pages: 0125-0139, 0227-0227
extraction: ocr
subsections:
    - "no": 1
      title: Minkowski’s inequality
      page: 18
      pdf_page: 125
    - "no": 2
      title: The semi-norms $N_p$
      page: 19
      pdf_page: 126
    - "no": 3
      title: The spaces $\mathscr{F}_F^p$
      page: 20
      pdf_page: 127
    - "no": 4
      title: $p$-th power integrable functions
      page: 23
      pdf_page: 130
    - "no": 5
      title: Properties of $p$-th power integrable functions
      page: 25
      pdf_page: 132
    - "no": 6
      title: Directed sets in $L^p$ and increasing sequences in $\mathscr{L}^p$
      page: 27
      pdf_page: 134
    - "no": 7
      title: Lebesgue’s theorem
      page: 30
      pdf_page: 137
    - "no": 8
      title: Relations between the spaces $\mathscr{L}_F^p$ ($1 \leq p < +\infty$)
      page: 31
      pdf_page: 138
statements: 44
exercises: 3
content_sha256: 571e05820e1eff3d2b10e4586ca1c9e388bda31865127bd10681ea7e38e48ae2
translated_from: content/en/int/IV/03_s3_lp_spaces.md
translation_method: google
source_content_sha256: 7e23198285dc5cb4353370685c3d59fc0442a1a826f792dd80d1ab78eaae10e8
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: a4ba25890a3eef3e40dcf5424628feb30b2d5025272515cc5b0dd108f0295d72
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。 L$^p$ 空間

### 1. ミンコフスキーの不等式

X を局所的にコンパクトな空間、$\mu$ を X のメジャーとします。 X で定義された正の数値写像 (有限であるかどうか) の集合では、写像 $|\mu|^*(f)$ は正で、正に均質で、増加するは凸です ($§ 1$、No. 3、提案 10、11、および 12)。

#### 命題 1 {#int-iv-s3-prop-1 .statement tag=08QN}

— X で定義された正の写像 $f, g$ (有限であるかどうか) のすべての実数 $p \geqslant 1$ およびすべての対について、

$$
(|\mu|^*((f + g)^p))^{1/p} \leqslant (|\mu|^*(f^p))^{1/p} + (|\mu|^*(g^p))^{1/p}
$$

(ミンコフスキーの不等式)。

不等式 (1) は、2 番目のメンバーの項の 1 つが $+\infty$ に等しい場合に明らかです。逆の場合、$f$ と $g$ はほぼどこでも有限です ($§ 2$、No. 3、提案 7)。 $f_1$ と $g_1$ がそれぞれ $f$ と $g$ に相当する有限の正の写像である場合、$f_1^p, g_1^p$ と $(f_1 + g_1)^p$ はそれぞれ $f^p, g^p$ と $(f + g)^p$ に相当し、等価の正の写像は同じ上積分を持つため、 ($§ 2$, No. 3, 提案 6)、$f$ と $g$ がどこでも有限である場合、証明不等式 (1) に還元されます。しかし、この場合不等式は、第 2 章で証明された一般的なミンコフスキー 不等式の特殊なケースです。 I、No. 2、提案 3。

また、次の基本的な不等式を使用する機会もあります。 $p \geqslant 1$ の場合、任意の数 $a \geqslant 0,\ b \geqslant 0$ に対して、

$$
a^p + b^p \leqslant (a + b)^p .
$$

$a = b = 0$ または数 $a, b$ の 1 つが $+\infty$ の場合、不等式は明らかです。 $a, b$ が有限で $a + b > 0$ の場合、次のように書くことができます。

$$
\left( \frac{a}{a + b} \right)^p + \left( \frac{b}{a + b} \right)^p \leqslant 1 ,
$$

それは次の事実から導かれます

$$
\left( \frac{a}{a + b} \right)^p \leqslant \frac{a}{a + b} , \quad \left( \frac{b}{a + b} \right)^p \leqslant \frac{b}{a + b} \quad \text{and} \quad \frac{a}{a + b} + \frac{b}{a + b} = 1 .
$$

### 2. 準規範 $N_p$

以下のすべてにおいて、$F$ は、体 $\mathbf{R}$ または体 $\mathbf{C}$ に対する *完全なノルム* ベクトル空間 (つまり、バナッハ空間) を表します。 元 $z \in F$ の *ノルム* は $|z|$ と表記されます。 Given a mapping $f$ of a set $A$ into $F$, we write $|f|$ for the mapping $x \mapsto |f(x)|$ of $A$ into $\mathbf{R}_+$ (one must take care to note that $|f|$ is a *numerical function*, and not a *number*).

#### 定義 1 {#int-iv-s3-def-1 .statement tag=08QO}

*$X$ を局所的にコンパクトな空間、$\mu$ を $X$ 上のメジャーとします。 $X$ のすべての写像 $f$ を Banach 空間 $F$ に変換し、$1 \leq p < +\infty$ となるすべての数 $p$ を、$N_p(f, \mu)$ または単に $N_p(f)$ で、正の数* で表します。 $(\int^* |f|^p d|\mu|)^{1/p}$。

数 $N_p(f)$ は $+\infty$ に等しい可能性があることに注意してください。

#### 命題 2 {#int-iv-s3-prop-2 .statement tag=08QP}

*$f$ と $g$ が $X$ の 2 つの写像を $F$ に変換したもので、$\alpha$ が任意のスカラー $\neq 0$ である場合、$1 \leq p < +\infty$ については、

(3) $$
N_p(\alpha f) = |\alpha| N_p(f)
$$
(4) $$
N_p(f + g) \leq N_p(f) + N_p(g).
$$

なぜなら、関係 (3) は Def からすぐに続きます。 1 そして、$|\mu|^*$ が確実に均一であるという事実。一方、$|f + g| \leq |f| + |g|$ なので、ミンコフスキーの不等式 (1) と $|\mu|^*$ が増加するであるという事実から、不等式 (4) が得られます。

私たちは拡大する Def. 1 から数値写像の場合、*有限であるかどうか*、$X$ で定義され、再度設定によって定義されます。

$$
N_p(f) = \left( \int^* |f|^p d|\mu| \right)^{1/p}
$$

写像 $f$ などの場合。 $f + g$ が $X$ と $\alpha \neq 0$ で定義されている場合、関係 (3) と (4) がこれらの写像にも成り立つことがすぐにわかります。さらに：

#### 定理 1 (可算凸数定理) {#int-iv-s3-thm-1 .statement tag=08QQ}

— *$(f_n)$ を、$X$ で定義された写像 $\geq 0$ (有限であるかどうか) の数列とします。 $1 \leq p < +\infty$の場合、

(5) $$
N_p \left( \sum_{n=1}^\infty f_n \right) \leq \sum_{n=1}^\infty N_p(f_n).
$$

集合 $f = \sum_{n=1}^\infty f_n$; $f$ は、写像 $g_n = \sum_{k=1}^n f_k$ の増加する数列の上部エンベロープです。 $N_p(f)$の定義、およびTh。 §1, No. 3 の 3 は、$N_p(f) = \sup_n N_p(g_n)$ であることを示します。しかし、提案 1 により $N_p(g_n) \leq \sum_{k=1}^n N_p(f_k)$、よって不等式 (5)。

#### 命題 3 {#int-iv-s3-prop-3 .statement tag=08QR}

*f と g が、バナッハ空間 F に X の 2 つ等しい写像である場合、$1 \leq p < +\infty$ は $N_p(f - g) = 0$ になります。逆に、$p \geq 1$ の値に対して $N_p(f - g) = 0$ の場合、f と g は同等です。*

Thから命題が一気に続きます。 §2, No. 3 の 1。

f と g が F に等しい 2 つの X 写像である場合、すべての $p \geq 1$ に対して $N_p(f) = N_p(g)$ (§ 2, No. 3、提案 6)。したがって、$N_p(f)$ は f の類 $\tilde{f}$ と、定義、$N_p(\tilde{f}) = N_p(f)$ による 1 つの集合にのみ依存します。 Xの写像の類をF形ベクトル空間（§ 2, No. 4）にすると、関係（3）と（4）も書くことができます

$$
(6) \quad N_p(\alpha \tilde{f}) = |\alpha| N_p(\tilde{f})
$$
$$
(7) \quad N_p(\tilde{f} + \tilde{g}) \leq N_p(\tilde{f}) + N_p(\tilde{g}).
$$

同等の数値写像 (有限であるかどうか) の類ごとに、同様に 1 つの定義する $N_p(\tilde{f})$。

One can then define $N_p(f)$ for a function with values in F (resp. in $\overline{\mathbf{R}}$) defined almost everywhere in X, by setting $N_p(f) = N_p(\tilde{f})$; it is then clear that the relations (3) and (4) again hold (assuming $\alpha \neq 0$ and $f + g$ defined almost everywhere, in the case of numerical functions, finite or not).

$0 < p < 1$ の場合、再び集合 $N_p(f) = (\int^* |f|^p d|\mu|)^{1/p}$ になりますが、不等式 (4) と (5) はもはや有効ではありません (cf. 第 3 章)。 I、エクサー。 6およびCh. IV, §6、エクサー。 13)。

### 3. 空間 $\mathscr{F}_F^p$

F を、X のすべての写像のバナッハ空間、$\mathscr{F}(X; F)$ (または単に $\mathscr{F}_F$) ベクトル空間を F にするとします。 $1 \leq p < +\infty$ については、$\mathscr{F}^p(X, \mu; F)$ または $\mathscr{F}_F^p(X, \mu)$、または単純に $\mathscr{F}_F^p(\mu)$ または $\mathscr{F}_F^p$ (混乱が生じない場合)、X の写像 f の集合を F に入れて、$N_p(f) < +\infty$ (代わりに $\mathscr{F}^p$ と書きます) で表します。 $\mathscr{F}_R^p$）。 $\mathscr{F}_F^p(|\mu|) = \mathscr{F}_F^p(\mu)$であることは明らかです。 No. 2の提案2から、$\mathscr{F}_F^p$は$\mathscr{F}_F$の*線形部分空間*であり、$N_p(f)$はこの空間の*準ノルム*であることがすぐにわかります。 私たちは常に (反対の明示的な言及がない限り) $\mathscr{F}_F^p$ にはこの準規範によって定義される位相が装備されていると仮定します。この位相は位数 p* の平均収束の *位相であると言います ($p = 1$ については、単に平均収束の *位相* と呼びます。$p = 2$ については、«二次平均の収束の位相» とも言います)。 We shall say that a filter $\mathscr{G}$ on $\mathscr{F}_F^p$ (resp. a sequence $(f_n)$ of elements of $\mathscr{F}_\mathbf{F}^p$) that converges to $f$ for this topology *converges in mean of order* $p$ to $f$; this means, therefore, that $N_p(g - f)$ tends to 0 with respect to $\mathscr{G}$ (resp. that $N_p(f_n - f)$ tends to 0 as $n$ tends to infinity).

この用語拡大するは、写像 $f_n$ と写像 $f$ がほぼどこでも定義されている (または $\overline{\mathbf{R}}$ に値があり、ほぼどこでも定義され有限である) 場合に一度に適用されます。

局所的に凸な空間 $\mathscr{F}_\mathbf{F}^p$ は一般に *ハウスドルフではない*ことに注意してください。この空間の 0 の閉包は、F への X の *無視できる* 写像の線形部分空間 $\mathscr{N}_\mathbf{F}$ です (No. 2、提案 3)。

#### 注意 {#int-iv-s3-n3-rem-1 .statement tag=08QS}

— F をバナッハ空間 * 体* $\mathbf{C}$ の複素数とする。次に、写像 $f \in \mathscr{F}_\mathbf{F}^p$ ごと、および複素数 $\alpha$ ごとに、$\alpha f$ 属するから $\mathscr{F}_\mathbf{F}^p$ および $N_p(\alpha f) = |\alpha| N_p(f)$ まで。他の語では、$\mathscr{F}_\mathbf{F}^p$も$\mathbf{C}$よりもベクトル空間であり、この複合体ベクトル空間（TVS、II, §1）では$N_p(f)$が準標準です。

#### 命題 4 {#int-iv-s3-prop-4 .statement tag=08QT}

*$\mathscr{B}$を$\mathscr{F}_\mathbf{F}^p$のフィルター基底とします。すべての集合 $M \in \mathscr{B}$ に対して、すべての写像 $f \in M$ のサポートが K に含まれるようなコンパクト集合 $K \subset X$ が存在すると仮定します。これらの条件の下で、$\mathscr{B}$ が X に一様に収束すると、 $f_0$、次に $f_0$ 属する ～ $\mathscr{F}_\mathbf{F}^p$ および $\mathscr{B}$ は、位数 $p$ ～ $f_0$ の平均で収束します。*

同じことになります。サポートが固定コンパクト集合に含まれている写像 $f \in \mathscr{F}_\mathbf{F}^p$ の集合では、位数 $p$ を平均すると、一様収束の位相は収束の位相よりも *より細かい* です。

なぜなら、$h$ は、K の 1 に等しい、コンパクトなサポートを備えた X から $[0,1]$ への連続した写像であるとします (Ch. III, §1, No. 2、補題 1)。 $\varepsilon > 0$ ごとに $M \in \mathscr{B}$ が存在し、写像ごとに $f \in M$、すべての $x \in X$ に対して $|f(x) - f_0(x)| \leq \varepsilon h(x)$ が存在します。これから、$N_p(f - f_0) \leq \varepsilon N_p(h)$、よって命題となります。

#### 命題 5 {#int-iv-s3-prop-5 .statement tag=08QU}

*局所凸空間$\mathscr{F}_\mathbf{F}^p$が完成しました*

$\mathscr{F}_\mathbf{F}^p$ に関連付けられたハウスドルフ空間はノルム空間であるため、$\mathscr{F}_\mathbf{F}^p$ のすべての *Cauchy 数列* $(f_n)$ が位数の平均で位相に対して収束する極限を有することを証明すれば十分です。 $p$ (GT、IX, §2, No. 6、提案 9)。 仮定までに、$\varepsilon > 0$ ごとに整数 $m_0$ が存在し、関係 $m \geq m_0,\ n \geq m_0$ は $N_p(f_n - f_m) \leq \varepsilon$ を暗示します。 One may therefore define, by induction on $k$, a strictly increasing sequence $(n_k)$ of integers $\geq 0$ such that $N_p(f_{n_{k+1}} - f_{n_k}) \leq 2^{-k}$. If we show that the series with general term $g_k = f_{n_{k+1}} - f_{n_k}$ ($k \geq 1$) is *convergent in mean of order* $p$, then it will have a sum $g \in \mathscr{F}_\mathbf{F}^p$, and $f = g + f_{n_1}$ will be the limit of the sequence $(f_{n_k})$ in $\mathscr{F}_\mathbf{F}^p$; $f$ will then be a cluster point of the sequence $(f_n)$; since this sequence is a Cauchy sequence, it will have $f$ as limit, and Prop. 5 will have been proved (GT, II, §3, No. 2, Cor. 2 of Prop. 5).

したがって、提案 5 は、次の命題の帰結です。

#### 命題 6 {#int-iv-s3-prop-6 .statement tag=08QV}

*$(f_n)$ を $\mathscr{F}_\mathbf{F}^p$ の写像の数列として、$\sum_{n=1}^\infty N_p(f_n) < +\infty$ とします。これらの条件、系列と一般的な項 $f_n(x) \in \mathbf{F}$ は、$X$ のほぼどこでも絶対に収束します。 系列が収束する点では設定$f(x) = \sum_{n=1}^\infty f_n(x)$、その他の場所では$f(x) = 0$、写像$f$属するから$\mathscr{F}_\mathbf{F}^p$で、一般的な系列の和です項 $f_n$ (位数 $p$ の平均収束の位相について)。より正確には、$n \geqslant 0$ごとに、

$$
N_p \left( f - \sum_{k=1}^n f_k \right) \leqslant \sum_{k=n+1}^\infty N_p(f_k).
$$

正の写像 (有限であるかどうか) $g(x) = \sum_{n=1}^\infty |f_n(x)|$ を考えてみましょう。可算凸面定理 (No. 2, Th. 1) により、

$$
N_p(g) \leqslant \sum_{n=1}^\infty N_p(f_n) < +\infty;
$$

したがって、$g$ はほぼどこでも有限です (§ 2, No. 3、提案 7)。これは、系列と一般的な項 $f_n(x)$ がほぼどこでも絶対収束することを意味します。 $\mathbf{F}$ が完了しているため、この系列はほぼどこでも収束し、すべての $x \in X$、$|f(x)| \leqslant \sum_{n=1}^\infty |f_n(x)| = g(x)$、よってについても収束します。

$$
N_p(f) \leqslant N_p(g) \leqslant \sum_{n=1}^\infty N_p(f_n) < +\infty,
$$

これは、$f$ 属するから $\mathscr{F}_\mathbf{F}^p$ であることを証明します。一方、整数 $n$ ごとに、

$$
|f(x) - \sum_{k=1}^n f_k(x)| \leqslant \sum_{k=n+1}^\infty |f_k(x)|
$$

ほとんどどこでも、よって $N_p \left( f - \sum_{k=1}^n f_k \right) \leqslant \sum_{k=n+1}^\infty N_p(f_k)$。 仮定までに、系列と一般的な項 $N_p(f_n)$ は収束します。したがって、すべての $\varepsilon > 0$ に対して、$\sum_{k=n+1}^{\infty} N_p(f_k) \leq \varepsilon$ となる整数 $n$ が存在し、不等式 (8) は、位相に対して一般的な項 $f_n$ と$f$ が系列の和であることを証明します。 位数 $p$ の平均での収束。

命題したがって、5 と 6 は完全に証明されます。

### 4. $p$ 冪可積分関数

ベクトル空間 $\mathscr{H}(X; F)$ (混乱を恐れない場合は、単に $\mathscr{H}_F$ と表記します)、$X$ から $F$ への連続写像のからなるは、明らかに、それぞれのベクトル空間の部分空間です。 $\mathscr{F}_F^p$。

#### 定義 2 {#int-iv-s3-def-2 .statement tag=08QW}

*局所的にコンパクトな空間* $X$、*測定* $\mu$ *on* $X$、*およびバナッハ空間* $F$、*表す* $\mathscr{L}_F^p(X, \mu)$ *(または単に* $\mathscr{L}_F^p(\mu)$、*または* $\mathscr{L}_F^p$) *閉鎖、局所凸型空間* $\mathscr{F}_F^p(X, \mu)$、*のベクトル空間* $\mathscr{H}(X; F)$ *連続写像の* $X$ *へ* $F$ *コンパクトサポート付き* *で表します* $L_F^p(X, \mu)$ *(または* $L_F^p(\mu)$、*または* $L_F^p$) *(標準)* ハウスドルフ *空間は* $\mathscr{L}_F^p(X, \mu)$ に関連付けられています。 *写像所属から* $\mathscr{L}_F^p$ * は、* $p$* 番目の冪可積分関数* (*) と呼ばれます。

明らかに$\mathscr{L}_F^p(X, |\mu|) = \mathscr{L}_F^p(X, \mu)$と$L_F^p(X, |\mu|) = L_F^p(X, \mu)$です。

$\mathscr{L}_R^p$ と $L_R^p$ (混乱が生じない場合は $\mathscr{L}_C^p$ と $L_C^p$) の代わりに、$\mathscr{L}^p$ と $L^p$ と書きます。 $F$ が*複素* Banach 空間である場合、$\mathscr{L}_F^p$ と $L_F^p$ は、体 $\mathbf{C}$ (No. 3, *注意*) 上のトポロジカルベクトル空間の構造を備えています。

$\mathscr{F}_F^p$ のすべての写像が、$\mathscr{L}_F^p$、属するから $\mathscr{L}_F^p$ の写像に相当することは明らかです。 写像と $F$ の値および $X$ の *ほぼどこでも定義* は、$\mathscr{L}_F^p$ の写像と同等であれば、*$p$*-*番目の冪可積分*であると言われます。同様に、$\overline{\mathbf{R}}$ の値を持つ写像は、$X$ のほぼどこでも定義され有限ですが、$\mathscr{L}^p$ の写像と等しい場合、*$p$*-*番目の冪可積分*であると言われます。

したがって、$\mathscr{L}_F^p$ (それぞれ$\mathscr{L}^p$) の写像は、*$p$*-* 番目の冪可積分関数* であり、*$X$ のすべてで定義されています (それぞれ、$X$ のすべてで定義され有限です)。この切断と次のものでは、$\mathscr{L}_F^p$ (それぞれ $\mathscr{L}^p$) で写像に対して証明された命題のほとんどは、どこでも定義されていない (それぞれ、どこでも定義されておらず有限である) *$p$*-*番目の冪可積分関数* にすぐに拡張できます。通常、これらの結果を定式化する作業と証明は読者に任せます。

(*) この用語の根拠については、§4, No. 2 で説明します。

#### 注意 1 {#int-iv-s3-n4-rem-1 .statement tag=08QX}

すでに通知されているように (§2, No. 5)、$\mathbf{F}$ の値を含む $p$ 番目の冪可積分関数は一般に形ベクトル空間になりません。

#### 注意 2 {#int-iv-s3-n4-rem-2 .statement tag=08QY}

一般に、空間 $\mathscr{F}_\mathbf{F}^p$ は、その部分空間 $\mathscr{L}_\mathbf{F}^p$ (§4、Exer. 8) とは異なります。

デフ。 2 により、次の基準がすぐに得られます。

#### 命題 7 {#int-iv-s3-prop-7 .statement tag=08QZ}

写像 $\mathbf{f}$ から属する 、そして $\mathscr{L}_\mathbf{F}^p$ については、$\varepsilon > 0$ ごとに、$N_p(\mathbf{f} - g) \leq \varepsilon$ のようなコンパクトなサポートを備えた連続した写像 $g$ が存在することが必要かつ十分です。

他の語、$\mathscr{L}_\mathbf{F}^p$の写像は、位数$p$の平均で収束の位相のため、コンパクトなサポートを備えた連続写像の数列の極限です。

#### 命題 8 {#int-iv-s3-prop-8 .statement tag=08R0}

$f$ を、ほぼどこでも定義されている数値写像 (有限かどうか) とします。すべての $\varepsilon > 0$ に対して、2 つの $p$ 番目冪可積分関数 $g, h$ が存在し、ほぼどこでも $g \leq f \leq h$ と $N_p(h - g) \leq \varepsilon$ が存在する場合、$f$ は $p$ 番目冪可積分です。

なぜなら、$f$ はほぼどこでも有限であり、$N_p(f - g) \leq N_p(h - g) \leq \varepsilon$ は有限だからです。したがって、提案 7 は、$f$ が $p$ 番目の冪で可積分であることを示しています。

定義により、$\mathscr{L}_\mathbf{F}^p$ は $\mathscr{F}_\mathbf{F}^p$ の閉じた部分空間であり、後者の空間が完了しているため (No. 3、提案 5)、次の結果が得られます (GT、II, §3, No. 4、提案 8)。

#### 定理 2 {#int-iv-s3-thm-2 .statement tag=08R1}

空間 $\mathscr{L}_\mathbf{F}^p$ が完了しました。 空間 $L_\mathbf{F}^p$ はバナハ空間です。

空間 $L_\mathbf{F}^p$ では、類のノルム $N_p(\tilde{\mathbf{f}})$ が再び $\| \tilde{\mathbf{f}} \|_p$ と表されます。

Th. 2 は次のようにシャープ化できます。

#### 定理 3 {#int-iv-s3-thm-3 .statement tag=08R2}

$(\mathbf{f}_n)$ を空間 $\mathscr{L}_\mathbf{F}^p$ の Cauchy 数列とします。次のプロパティを持つ $(\mathbf{f}_n)$ のサブシーケンス $(\mathbf{f}_{n_k})$ が存在します。
1° 系列と一般的な項 $N_p(\mathbf{f}_{n_{k+1}} - \mathbf{f}_{n_k})$ は収束します。
2° 系列と一般的な項 $\mathbf{f}_{n_{k+1}}(x) - \mathbf{f}_{n_k}(x)$ はほぼどこでも絶対に収束します。
3° $\mathbf{f}$ が $X$ で定義された写像で、ほぼどこでも数列 $(\mathbf{f}_{n_k}(x))$ の極限に等しい場合、$\mathbf{f}$ 属するから $\mathscr{L}_\mathbf{F}^p$ および数列 $(\mathbf{f}_n)$ は次のように収束します。 位数 $p$ ～ $\mathbf{f}$ の平均。
4°には、$N_p(g) < +\infty$ となるような下位の半連続写像 $g \geq 0$ が存在し、すべての $k$ に対して、すべての $x \in X$ に対して $|\mathbf{f}_{n_k}(x)| \leq g(x)$ が存在します。

No. 3 の提案 5 の証明のように、$N_p(\mathbf{f}_{n_{k+1}} - \mathbf{f}_{n_k}) \leq 2^{-k}$ が成り立つように、定義する数列 $(n_k)$ を帰納法で満たせば十分です。 部分 2° と 3° は、No. 3 の提案 6 と、$\mathscr{L}_\mathbf{F}^p$ が $\mathscr{F}_\mathbf{F}^p$ で閉じられるという事実から続きます。一方、$h(x)$ が一般項 $|\mathbf{f}_{n_{k+1}}(x) - \mathbf{f}_{n_k}(x)|$ で系列の和である場合、Th. No. 2 の 1 は $N_p(h) < +\infty$ を示します。したがって、$|\mu|^*$の定義までに、$N_p(g) < +\infty$のような下位の半連続写像$g \geq h + |\mathbf{f}_{n_1}|$が存在し、証明が完成します。

#### 系 1 {#int-iv-s3-thm-3-cor-1 .statement tag=08R3}

— *コーシー 数列* $(f_n)$ *in 空間* $\mathscr{L}_F^p$ *が数列* $(f_n(x))$ *ほぼどこでも* $f(x)$* に収束するような場合、* $f$ * は p 番目冪積分可能であり、 数列* $(f_n)$ *は位数* $p$ *から* $f$ の平均で収束します。

なぜなら、$(f_{n_k}(x))$ がほぼどこでも $g(x)$ に収束するような $(f_n)$ の部分列 $(f_{n_k})$ が存在し、$g$ は $\mathscr{L}_F^p$ の写像であり、$(f_n)$ は位数の平均で収束するからです。 $p$から$g$まで。したがって、仮説は、ほぼどこでも $f(x) = g(x)$、よって系を意味します。

#### 系 2 {#int-iv-s3-thm-3-cor-2 .statement tag=08R4}

— *$\mathscr{E}$ *$\mathscr{L}_F^p$ の密な部分集合とします。 *すべての写像* $f \in \mathscr{L}_F^p$ に対して、*写像の数列* $(g_n)$ が * $\mathscr{E}$ に存在し、 *次のプロパティを持ちます*:

1° *数列* $(g_n)$ *位数* $p$ *から* $f$ の平均で収束します。
2° *ほぼすべて* $x \in X$、*数列* $(g_n(x))$ *$f(x)$ に収束します。

なぜなら、空間 $\mathscr{L}_F^p$ は計化可能であるため、$\mathscr{E}$ の写像のからなるに $\mathscr{L}_F^p$ のコーシー 数列 $(f_n)$ が存在し、位数の平均で収束するからです。 $p$ ～ $f$ (GT、IX, §2, No. 6、提案 8)。 Thを適用するだけで十分です。 3からこれ数列まで。

コル。 2 は、特に、$\mathscr{E}$ が *コンパクト サポート* の連続写像の空間 $\mathscr{K}_F$ とみなされる場合に適用されます。

#### 注意 3 {#int-iv-s3-n4-rem-3 .statement tag=08R5}

$\mathscr{L}_F^p$ のコーシー 数列 $(f_n)$ は、数列 $(f_n(x))$ が $X$ の * 点において収束しないようなものになる可能性があります (例 1)。

#### 注意 4 {#int-iv-s3-n4-rem-4 .statement tag=08R6}

$f$ 属するから $\mathscr{L}_F^p$ の場合、数列 $(f_n(x))$ が $X$ の *どこでも* 収束するようなコンパクトなサポートを使用して連続写像の数列 $(f_n)$ を見つけることが常に可能であるとは限りません。 写像はほぼどこでも $f(x)$ に等しい (§4、Exer. 4 c))。

### 5. $p$番目冪可積分関数の物件

#### 定理 4 {#int-iv-s3-thm-4 .statement tag=08R7}

— *$F$ *と* $G$ *2 つのバナッハ空間、* $u$ *$F$ の *連続線形写像を *$G$ にします。 *各写像* $f \in \mathscr{L}_F^p$、*複合写像* $u \circ f$ *属するから* $\mathscr{L}_G^p$。

$f \in \mathscr{L}_F^p$ にしましょう。すべての $\varepsilon > 0$ に対して、$N_p(f - g) \leq \varepsilon$ となる写像 $g \in \mathscr{K}_F$ が存在します。 $|u \circ f - u \circ g| \leq \|u\| \cdot |f - g|$ 以来、

$$
N_p(u \circ f - u \circ g) \leq \|u\| \cdot N_p(f - g) \leq \varepsilon \|u\|,
$$

$u \circ g$ はコンパクトサポートで連続なので、定理が証明されます。

#### 系 1 {#int-iv-s3-thm-4-cor-1 .statement tag=08R8}

— *$a'$ *$F$ で連続する線型形式とします。 *if* $f \in \mathscr{L}_F^p$、*数値写像* $x \mapsto \langle f(x), a' \rangle$ **($\langle f, a' \rangle$ で示されます)* 属するから* $\mathscr{L}^p$。

#### 系 2 {#int-iv-s3-thm-4-cor-2 .statement tag=08R9}

— F ($1 \leq k \leq n$) の n 点 $a_k$ と、n 個の数値写像 $f_k$ ($1 \leq k \leq n$) 所属から $\mathscr{L}^p$、写像 $f = \sum_{k=1}^n a_k f_k$ 属するから $\mathscr{L}_F^p$ が与えられたとします。

これは、F への $\mathbf{R}$ の写像 $t \mapsto a t$ が連続であるという事実からわかります。

#### 命題 9 {#int-iv-s3-prop-9 .statement tag=08RA}

— F を $\mathbf{R}$ 上の n 次元ベクトル空間とし、$(e_k)_{1 \leq k \leq n}$ を F の基底とします。 写像 $f = \sum_{k=1}^n e_k f_k$ から属する $\mathscr{L}_F^p$ については、それぞれの数値写像 $f_k$ が必要かつ十分です属するから$\mathscr{L}^p$まで。

これはコルスからすぐに続きます。 Thの1と2。 4.

#### 命題 10 {#int-iv-s3-prop-10 .statement tag=08RB}

— 空間 $\mathscr{L}_F^p$ では、(有限) 線形結合 $\sum_k a_k f_k$ によって形成される線形部分空間は、$a_k \in F$ と $f_k$ がコンパクトなサポートを持つ連続数値写像であり、密です (位数を平均して収束する位相の場合) $p$）。

コンパクトなサポートを備えた F への連続 X の写像の集合 $\mathscr{K}_F$ は、$\mathscr{L}_F^p$ での定義による密集です。一方、すべての写像 $g \in \mathscr{K}_F$ は、形 $\sum_k a_k f_k$ の写像によって一様に近似できます。ここで、$f_k$ は、$g$ のサポートの固定されたコンパクトな近傍に含まれるサポートを持つ連続写像です (Ch. III, §1, No. 2、 補題 2);したがって、(No. 3、提案 4) $g$ は、$\sum_k a_k f_k$、よって命題の集合の $\mathscr{L}_F^p$ の閉包内にあります。

#### 命題 11 {#int-iv-s3-prop-11 .statement tag=08RC}

— 写像 $f$ 属するから $\mathscr{L}_F^p$ までの場合、 写像 $|f|$ 属するから $\mathscr{L}^p$ 、および $\mathscr{L}_F^p$ から $\mathscr{L}^p$ への写像 $f \mapsto |f|$ は一様連続です ( 位数 $p$ の平均における収束の位相)。

$\varepsilon > 0$ ごとに、$N_p(f - g) \leq \varepsilon$ のようなコンパクトなサポートを備えた連続的な写像 $g$ が存在します。 $||f| - |g|| \leq |f - g|$ から、$N_p(|f| - |g|) \leq \varepsilon$ があり、これは $|f| \in \mathscr{L}^p$ であることを証明します。一方、$\mathscr{L}_F^p$の$f_1, f_2$が2つの写像であれば$N_p(|f_1| - |f_2|) \leq N_p(f_1 - f_2)$となり、$f \mapsto |f|$が一様連続の写像であることがわかります。

#### 命題 12 {#int-iv-s3-prop-12 .statement tag=08RD}

— 写像 $f$ ～ 属する ～ $\mathscr{L}^p$ の場合、写像 $f^+$ と $f^-$ 属する ～ $\mathscr{L}^p$ がそれぞれ必要十分です。

$f = f^+ - f^-$ であるため、条件で十分です。 $f \in \mathscr{L}^p$ なら $|f| \in \mathscr{L}^p$ となるため、これは必要です (提案 11)。

#### 系 {#int-iv-s3-n5-cor-1 .statement tag=08RE}

— $\mathscr{L}^p$ 属するから $\mathscr{L}^p$ の写像の有限族の上部 (それぞれ下部) エンベロープ。

### 6. $L^p$ では有向集合 、$\mathscr{L}^p$ では増加する数列

同値類の集合 $\widetilde{\mathscr{F}}$ で (§ 2, No. 6) 位数関係 $\tilde{f} \leq \tilde{g}$ を定義し、$X$ のほぼすべての場所で数値写像を定義し有限にしました。この位数関係とそのベクトル空間構造を装備した $\widetilde{\mathscr{F}}$ は *Riesz 空間* です。 No. 5 の提案 12 の系は、$\tilde{f}$ と $\tilde{g}$ が 2 つの元部分空間 $L^p$ $\widetilde{\mathscr{F}}$ である場合、$\tilde{f}$ の最高$\sup(\tilde{f}, \tilde{g})$ と$\widetilde{\mathscr{F}}$の$\tilde{g}$（写像$\sup(f, g)$のそれぞれ類、$f \in \tilde{f}$と$g \in \tilde{g}$）属するから$L^p$。これは特に、$\widetilde{\mathscr{F}}$ によって誘発された位数関係を備えた$L^p$ が *Riesz 空間* であることを証明します。

#### 命題 13 {#int-iv-s3-prop-13 .statement tag=08RF}

*リース空間 $L^p$ では、ノルム $\| \tilde{f} \|_p$ によって定義される位相が装備されており、写像 $\tilde{f} \mapsto | \tilde{f} |$ は一様連続で、元 $\tilde{f} \geq 0$ の集合は閉じています。

命題の最初の部分は、No. 5 の提案 11 からすぐに続きます。 $\tilde{f} \geq 0$の集合は$\tilde{f}$の集合でもあり、$| \tilde{f} | = f$となるため、$\tilde{f} \mapsto | \tilde{f} |$は連続写像であり、$L^p$はハウスドルフであるため、閉じられます。

したがって、ノルム $\| \tilde{f} \|_p$ によって定義された $L^p$ の位相は、$L^p$ (TVS、II, § 2, No. 7) の順序付けられたベクトル空間構造と *互換性* があることがわかります。

#### 命題 14 {#int-iv-s3-prop-14 .statement tag=08RG}

*$H$をリース空間$L^p$の部分集合、類$\geq 0$のからなるとし、関係$\leq$に向けます。 $H$ が $L^p$ で最高値を持つためには、次のことが必要かつ十分です*

$$
\sup_{\tilde{f} \in H} \| \tilde{f} \|_p < +\infty.
$$

*$L^p$ の $H$ の最高値は、極限* (Banach 空間 $L^p$ では) *$H$* の切断フィルターです。

The condition is clearly necessary, since $\tilde{f} \mapsto \| \tilde{f} \|_p$ is an increasing function on the set of elements $\geq 0$ of $L^p$. To see that it is sufficient, we first observe that it implies that the image of $H$ under the mapping $\tilde{f} \mapsto \| \tilde{f} \|_p$ has a limit in $\mathbf{R}$, by the monotone limit theorem; the image of the section filter $\mathfrak{F}$ of $H$ under this mapping is therefore a base of a Cauchy filter on $\mathbf{R}$. $\mathfrak{F}$ 自体が $L^p$ 上のコーシーフィルター* の *基底であることを示せば、証明は完了します。なぜなら、$L^p$ が完了しているため (No. 4、Th. 2)、$\mathfrak{F}$ は $L^p$ で収束し、TVS、II, § 2, No. 7、提案 18 から命題が続きます。

$\mathfrak{F}$ が Cauchy フィルターの基底であることを確認するには、次の補題を使用します。

#### 補題 {#int-iv-s3-n6-lem-1 .statement tag=08RH}

$f$ と $g$ が $\mathscr{L}^p$ の 2 つ写像で、$0 \leq f \leq g$ となる場合、

$$
(N_p(g - f))^p \leq (N_p(g))^p - (N_p(f))^p .
$$

$f$ と $g$ がコンパクトサポートで連続している場合、関係 (9) と書くことができます

$$
\int (g - f)^p d|\mu| \leq \int g^p d|\mu| - \int f^p d|\mu|
$$

そして、初級の不等式 $(g - f)^p \leq g^p - f^p$ (No. 1, 公式 (2)) の帰結です。ここから一般的な場合に移るには、(9) の 2 つの要素が $\mathscr{L}^p \times \mathscr{L}^p$ で連続写像であり、$\mathscr{L}^p$ のすべての写像 $f \geq 0$ が (位数 $p$ の平均で収束するため) 極限であることを観察すれば十分です。 $\mathscr{L}^p$ の写像 $g \mapsto |g|$ の連続性により、コンパクトなサポートを備えた連続写像 $\geq 0$ の数列 (提案 11)。

補題が確立されると、$\varepsilon > 0$ ごとに仮定までに $\tilde{f} \in \mathrm{H}$ が存在し、$\tilde{g} \geq \tilde{f}$ 所属から $\mathrm{H}$ ごとに$(\|\tilde{g}\|_p)^p - (\|\tilde{f}\|_p)^p \leq \varepsilon$ が存在します。このことから、$(\|\tilde{g} - \tilde{f}\|_p)^p \leq \varepsilon$ ということがわかります。したがって、$\tilde{g}_1$と$\tilde{g}_2$が$\geq \tilde{f}$である$\mathrm{H}$の2つの元であれば、$\|\tilde{g}_1 - \tilde{g}_2\|_p \leq 2\varepsilon^{1/p}$となり、$\mathfrak{F}$が$L^p$に対するコーシーフィルター基底であることが証明され、Prop.の証明が完成します。 14.

#### 系 1 {#int-iv-s3-prop-14-cor-1 .statement tag=08RI}

$\tilde{g}$ が $L^p$ の $\mathrm{H}$ の上限である場合、

$$
\|\tilde{g}\|_p = \lim_{\tilde{f} \in \mathrm{H}} \|\tilde{f}\|_p = \sup_{\tilde{f} \in \mathrm{H}} \|\tilde{f}\|_p .
$$

これは、$L^p$ のノルム $\|\tilde{f}\|_p$ の連続性と、単調な極限定理から生じます。

#### 系 2 {#int-iv-s3-prop-14-cor-2 .statement tag=08RJ}

Riesz 空間 $L^p$ は完全に格子順序付けされています。

Every directed set $\mathrm{H}$ in $L^p$ (for the relation $\leq$), consisting of classes $\geq 0$ and bounded above in $L^p$, has a supremum: for, if $\tilde{h}$ is an upper bound for $\mathrm{H}$ in $L^p$, then $\|\tilde{f}\|_p \leq \|\tilde{h}\|_p$ for all $\tilde{f} \in \mathrm{H}$, and Prop. 14 is applicable. これは系を証明します (Ch. II, §1, No. 3、提案 1)。

提案 14 の結論は、$\mathscr{L}^p$ の類ではなく写像について定式化されると、もはや成立しません。正確に言うと、$M$ が $\mathscr{L}^p$ の部分集合、写像 $\geq 0$ のからなるで、関係 $\leq$ に向けられている場合、$\sup_{f \in M} N_p(f) < +\infty$、上部エンベロープの *類* $g$ $M$ *は必ずしも * の最高値と同一ではありません* $L^p$ *of 類 of 写像* f \in M ;特に、g は必ずしも p 番目の冪が可積分であるとは限らず、たとえ $g \in \mathscr{L}^p$ であっても $N_p(g)$ は $\sup_{f \in M} N_p(f)$ とは区別できます (Th. 3 に続く cf. §1, No. 3、注意 1)。

それにもかかわらず、次の定理があります。

#### 定理 5 {#int-iv-s3-thm-5 .statement tag=08RK}

※$(f_n)$を$\mathscr{L}^p$の写像$\geqslant 0$の増加する数列とします。この数列の上包絡線$f$ が p 番目の冪が可積分であるためには、$\sup_n N_p(f_n) < +\infty$ であることが必要十分です。 数列 $(f_n)$ は、位数 $p$ から $f$ の平均で収束し、*

$$
N_p(f) = \sup_n N_p(f_n) = \lim_{n \to \infty} N_p(f_n).
$$

条件は明らかに必要なので、それが十分であることを証明するだけで十分です。さて、条件が満たされる場合、提案 14 は、数列 $(\tilde{f}_n)$ が $L^p$ のコーシー 数列であるため、数列 $(f_n)$ は $\mathscr{L}^p$ のコーシー 数列であることを示します。 $f_n(x)$ はすべての $x \in X$ に対して $f(x)$ になる傾向があるため、$f$ は p 番目の冪で可積分であり、位数の平均で収束する位相に対して数列 $(f_n)$ の極限になります。 $p$ (No. 4、Th. 3 のコリント 1)。したがって、$N_p$は$\mathscr{L}^p$に連続した写像であるため、$N_p(f_n)$は$N_p(f)$になる傾向があります。

#### 系 1 {#int-iv-s3-thm-5-cor-1 .statement tag=08RL}

*$(f_n)$ を $\mathscr{L}^p$ の写像 $\geqslant 0$ の減少列とします。次に、数列属する ～ $\mathscr{L}^p$、数列 $(f_n)$ の下側エンベロープ $f$ は、位数 $p$ ～ $f$ の平均で収束し、*

$$
N_p(f) = \lim_{n \to \infty} N_p(f_n) = \inf_n N_p(f_n).
$$

最初の 2 つの主張は Th から続きます。 5 は数列 $g_n = f_1 - f_n$ に適用され、これは増加するであり、その上に制限されています。残りは明らかです。

#### 系 2 {#int-iv-s3-thm-5-cor-2 .statement tag=08RM}

※$(f_n)$を$\mathscr{L}^p$の写像の数列とします。 数列 $(f_n)$ の上包絡線 $f$ が p 番目冪で可積分であるためには、すべての $n$ に対して $\int^* g^p d|\mu| < +\infty$ と $f_n \leqslant g$ となるような写像 $g \geqslant 0$ が存在することが必要かつ十分です。

$g = f^+$を取る場合、条件は明らかに必要です。逆に、検証されたとすると、集合 $g_n = \sup_{k \leqslant n} f_k$; 数列 $(g_n)$ は増加するで、p 番目の冪可積分関数で構成されます (No. 5、提案 12 の修正)。正の写像 $h_n = g_n + g_1^-$ の増加する数列は Th の条件を満たします。 5、$N_p(h_n) \leqslant N_p(g + g_1^-) < +\infty$ 以降。したがって、その上部包絡線 $\sup_n h_n$ は p 番目冪が可積分であり、同じことが $f = \sup_n h_n - g_1^-$ にも当てはまります。

#### 系 3 {#int-iv-s3-thm-5-cor-3 .statement tag=08RN}

— $A$ を可算集合、$\mathfrak{F}$ を可算基底を持つ $A$ のフィルター、$(f_\alpha)_{\alpha \in A}$ を $\mathscr{L}^p$ の写像 $\geq 0$ の族とする。すべての $\alpha \in A$ に対して $N_p(g) < +\infty$ と $f_\alpha \leq g$ となる写像 $g \geq 0$ が存在すると仮定します。この場合、写像 $\limsup_{\mathfrak{F}} f_\alpha$ は $p$ 番目の冪が可積分であり、

$$
\limsup_{\mathfrak{F}} N_p(f_\alpha) \leq N_p(\limsup_{\mathfrak{F}} f_\alpha).
$$

Let $(A_n)$ be a decreasing base of $\mathfrak{F}$ and set $g_n = \sup_{\alpha \in A_n} f_\alpha$; since $A_n$ is a countable set, it follows from Cor. 2 that $g_n$ is $p$-th power integrable; on the other hand, $N_p(g_n) \geq \sup_{\alpha \in A_n} N_p(f_\alpha)$. したがって、$\limsup_{\mathfrak{F}} f_\alpha$ は減少列 $(g_n)$ の下側の包絡線です。したがって、$\limsup_{\mathfrak{F}} f_\alpha$ は、$p$ 番目の冪が Cor によって積分可能です。 1、そして

$$
N_p(\limsup_{\mathfrak{F}} f_\alpha) = N_p \left( \inf_n g_n \right) = \lim_{n \to \infty} N_p(g_n)
$$
$$
\geq \lim_{n \to \infty} \left( \sup_{\alpha \in A_n} N_p(f_\alpha) \right) = \limsup_{\mathfrak{F}} N_p(f_\alpha).
$$

### 7. ルベーグ定理

#### 定理 6 (ルベーグ) {#int-iv-s3-thm-6 .statement tag=08RO}

— $F$ を、$\mathscr{L}_F^p$ の写像のバナッハ空間、$(f_n)$ 数列とします。 $1^\circ$ 数列 $(f_n(x))$ は、ほぼどこでも極限 $f(x) \in F$ に収束します。 $2^\circ$ 整数 $n$ ごとに、$X$ のほぼどこにでも $\int^* g^p d|\mu| < +\infty$ と $|f_n(x)| \leq g(x)$ という数値写像 $g \geq 0$ が存在します。すると、写像 $f$ (ほぼどこでも定義されている) は、$p$ 番目の冪が可積分であり、数列 $(f_n)$ は、位数 $p$ から $f$ の平均で収束します。

数値写像 $g_{mn} = |f_m - f_n|$ の「倍」 数列、つまり属するから $\mathscr{L}^p$ を考えてみましょう (No. 5、提案 11)。 仮定、$\lim_{m \to \infty, n \to \infty} g_{mn}(x) = 0$ はほぼどこでも、その一方で $|g_{mn}(x)| \leq 2g(x)$ はほぼどこでも。 適用コル。 Thの3。 No. 6 の 5 をこのダブル数列に、

$$
\limsup_{m \to \infty, n \to \infty} N_p(f_m - f_n) \leq N_p(0) = 0,
$$

そして $N_p(f_m - f_n) \geq 0$ 以降、これは $\lim_{m \to \infty, n \to \infty} N_p(f_m - f_n) = 0$ を意味します。他の語, 数列 $(f_n)$ は、$\mathscr{L}_F^p$ のコーシー数列です。したがって、定理はコルから続きます。 Thの1 No. 4の3。

#### 系 {#int-iv-s3-n7-cor-1 .statement tag=08RP}

— $A$ を、可算基底を持つフィルタ $\mathfrak{F}$ でフィルタリングした、添字の集合とします。 $(f_\alpha)_{\alpha \in A}$ が $\mathscr{L}_F^p$ の写像の族で、フィルター $\mathfrak{F}$ に関して、ほぼどこでも点ごとに写像 $f$ に収束し、さらに、$\int^* g^p d|\mu| < +\infty$ となるような数値写像 $g \geq 0$ が存在するとします。 $|f_\alpha(x)| \leq g(x)$ は $\alpha \in A$ ごとに $X$ のほぼどこでも、その場合、写像 $f$ は $p$ 番目の冪可積分であり、$f_\alpha$ は位数 $p$ の平均となる傾向があります。フィルター$\mathfrak{F}$に関しては$f$。

というのは、$(A_n)$ を $\mathfrak{F}$ の可算基底である減少するとし、$\alpha_n$ を $A_n$ の任意の元とするからです。 数列 $(f_{\alpha_n})$ は、$X$ のほぼすべての場所で点的に $f$ に収束します。 6は、$f$が$p$番目の冪可積分であり、$\lim_{n \to \infty} N_p(f - f_{\alpha_n}) = 0$が可分であることを示しています。 $\mathfrak{F}$ は、そのようなすべての数列 $(\alpha_n)$ (GT、I, §6, No. 8、提案 11) に関連付けられた基本フィルターの共通部分フィルターであるため、$\lim_{\mathfrak{F}} N_p(f - f_\alpha)$ が存在し、すべての数列の共通の極限 0 に等しくなります。 $(N_p(f - f_{\alpha_n}))$。

#### 注意 1 {#int-iv-s3-n7-rem-1 .statement tag=08RQ}

Th. 仮定 $|f_n| \leq g$ ($N_p(g) < +\infty$) がより弱い仮定 $\sup_n N_p(f_n) < +\infty$ に置き換えられた場合、6 は成り立ちません。たとえば、$\mu$ が $\mathbf{R}$ のルベーグ測度であるとします。 定義するは次のように連続写像 $f_n$: $x \leq 0$ に対して $f_n(x) = 0$、$x \geq \frac{2}{n}$、$f_n(\frac{1}{n}) = n$、$f_n$ は区間 $[0, \frac{1}{n}]$ 上で直線的であり、 $[\frac{1}{n}, \frac{2}{n}]$。次に、すべての $x \in \mathbf{R}$ に対しては $\lim_{n \to \infty} f_n(x) = 0$ ですが、すべての $n$ に対しては $N_1(f_n) = 1$ になります (cf. §5、Exer. 12)。

#### 注意 2 {#int-iv-s3-n7-rem-2 .statement tag=08RR}

コル。 Thの。フィルター $\mathfrak{F}$ が可算数基底 (Th. 3 の Cor. に続く cf. §1, No. 3、注意 1) を持っていると仮定しない場合、6 はもはや成り立ちません。

### 8. 関係空間 $\mathscr{L}_F^p$ ($1 \leq p < +\infty$)

実数 $\alpha > 0$ ごとに、写像 $z \mapsto |z|^{\alpha-1} \cdot z$ が定義され、$F$ の 0 の補数で連続します。さらに、$||z|^{\alpha-1} \cdot z| = |z|^{\alpha}$ 以降、この写像は $z$ で 0 になる傾向があるため、$\alpha < 1$ であっても、この点で値 0 を与えることで、連続性によって点 0 まで拡張される可能性があります。

#### 定理 7 {#int-iv-s3-thm-7 .statement tag=08RS}

— $p$ と $q$ を 2 つの実数とし、$1 \leq p < +\infty$、$1 \leq q < +\infty$ とします。 写像 $f$ 属する ～ $\mathscr{L}_F^p$ の場合、写像 $|f|^{(p/q)-1} \cdot f$ 属する ～ $\mathscr{L}_F^q$、およびその逆。

仮定までに、ほぼどこにでも $\sum_{n=1}^\infty N_p(f_n) < +\infty$ と $f(x) = \sum_{n=1}^\infty f_n(x)$ のようなコンパクトなサポートを備えた連続写像の数列 $(f_n)$ が存在します (No. 4、Th. 3)。 集合

$$
g_n = |f_1 + f_2 + \cdots + f_n|^{(p/q)-1} \cdot (f_1 + f_2 + \cdots + f_n);
$$

写像 $g_n$ はコンパクトなサポートで継続的です。一方で、

$$
|g_n|^q = |f_1 + f_2 + \cdots + f_n|^p \leq \left( \sum_{n=1}^\infty |f_n| \right)^p = h^q,
$$

ここで、数値写像 $h \geqslant 0$ (有限であるかどうか) は不等式を満たします。

$$
(N_q(h))^q = \left( N_p \left( \sum_{n=1}^{\infty} |f_n| \right) \right)^p \leqslant \left( \sum_{n=1}^{\infty} N_p(f_n) \right)^p < +\infty
$$

可算凸部定理によって。さらに、$g_n(x)$ はほぼどこでも $g(x) = |f(x)|^{(p/q)-1} \cdot f(x)$ になる傾向があるため、ルベーグの定理は $g \in \mathscr{L}_F^q$ であることを示しています。 $f = |g|^{(q/p)-1} \cdot g$ なので、逆は明らかです。

写像 $f \mapsto |f|^{\frac{p}{q}-1} \cdot f$ は $\mathscr{L}_F^p$ の $\mathscr{L}_F^q$ への同写写像であることが示されます (§ 6、Exer. 10)。

#### 系 1 {#int-iv-s3-thm-7-cor-1 .statement tag=08RT}

— *写像 $f$ ～ 属する ～ $\mathscr{L}_F^p$ については、 写像 $|f|^{p-1} \cdot f$ 属する ～ $\mathscr{L}_F^1$ が必要十分です。*

#### 系 2 {#int-iv-s3-thm-7-cor-2 .statement tag=08RU}

— *正の数値写像 $f$ ～ 属する ～ $\mathscr{L}^p$ の場合、 $f^p$ 属する ～ $\mathscr{L}^1$ であることが必要十分です。*

$f$ が、$|f|^p$ 属するから $\mathscr{L}^1$ のような任意の符号の数値写像である場合、$f$ は必ずしも属するから $\mathscr{L}^p$ になるわけではないことに注意してください (cf. § 4、Exer. 8)。

### 練習問題 {#int-iv-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
