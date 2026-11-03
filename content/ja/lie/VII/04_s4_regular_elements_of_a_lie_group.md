---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 4
section_title: Regular elements of a Lie group
lang: ja
source: lie-vii-ix
book_pages: 27-34, 63
pdf_pages: 0037-0044, 0072-0072
extraction: native
subsections:
    - "no": 1
      title: REGULAR ELEMENTS FOR A LINEAR REPRESENTATION
      page: 27
      pdf_page: 37
    - "no": 2
      title: REGULAR ELEMENTS OF A LIE GROUP
      page: 29
      pdf_page: 39
    - "no": 3
      title: RELATIONS WITH REGULAR ELEMENTS OF THE LIE ALGEBRA
      page: 31
      pdf_page: 41
    - "no": 4
      title: APPLICATION TO ELEMENTARY AUTOMORPHISMS
      page: 34
      pdf_page: 44
statements: 18
exercises: 4
content_sha256: 57ad39bf98e090bda7916acb9fcdd6c2cc7c7101270e1f23e505657b4af6a22e
translated_from: content/en/lie/VII/04_s4_regular_elements_of_a_lie_group.md
translation_method: google
source_content_sha256: 1839a11c4384fe28967cd541901f8ab98cc088922894403c4f8106b9bf54bee7
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: b76e3423a75d79596862aec58fb42cf617e31f09932a63f4bf8c54ce676ebe77
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 4。 正則元/リー群

番号で。この段落の 1、2、3 では、$k$ が $\mathbf{R},\mathbf{C}$ または特性 0 の非離散完全超計量体であると仮定します。 $k$ 上の有限次元リー群を、$\mathfrak{g}$ でそのリー代数を、そして $e$ でそのリー群を表します単位元。 $a\in G$ の場合、Ad $(a)-1$ のゼロスペースを $\mathfrak{g}^1(a)$ で表し、その他の場合は語空間 $\mathfrak{g}^1$(Ad($a$)) (cf. §1, no. 1) となります。

### 1. 線型表現の正則元

#### 補題 1 {#lie-vii-s4-lem-1 .statement tag=00VU}

M を、M 上の分析写像の $k$ および $a= (a_0, . . . , a_{n-1}, a_n= 1)$ 数列に対する分析多様体とします。すべての $x\in M$ について、$r_a(x)$ を、$a_j(x) = 0$ が成り立つような $i\in 0, n$ の上界とします。 $j < i$ そして、$r_a^0(x)$ をそれら $i\in 0, n$ の上界とし、$a_j$ は $j < i$ の $x$ の近傍上の零とします。

(i) 写像 $r_a$ は上半連続です。

(ii) すべての $x\in M,r_a^0(x) =$ lim inf$_{y\rightarrow x}r_a(y)$ に対して。

(iii) 写像 $r_a^0$ は局所的に一定です。

(iv) $r^0_a(x) =r_a(x)$ が近傍上の M の点の集合であり、その $r_a$ が定数であるような、点 $x\in M$ の集合。これは M の密な開いた部分集合です。$k=\mathbf{C}$ と M が有限次元で接続されている場合、それは開いていて接続されています。

(i) $r_a(x) =i$ の場合、$a_i(x)\not= 0$、そして $x$ の近傍のすべての $y$ に対して、$a_i(y)\not= 0$ があるため、$r_a(y)\leq i$ になります。

(ii) $r^0_a(x) =i$、写像 $a_0, . . . , a_{i-1}$ が $x$ の近傍で零であり、この近傍の$y$ については、$r_a(y)\geq i$ である場合。従って、lim inf$_{y\rightarrow x}r_a(y)\geq i$ となります。 $x$ 含む点 $y$ のすべての近傍は、$a_i(y)\not= 0$ となり、従って $r_a(y)\leq i$ となります。従って、lim inf$_{y\rightarrow x}r_a(y) =i$ となります。

(iii) $i=r_a^0(x)$ と V を $x$ の近傍とし、すべての $y\in V$ とすべての $j < i$ に対して $a_j(y) = 0$ となるようにします。次に $x\in M$**--** Z です。ここで、Z は近傍の M の点の集合を表し、そのうち写像 $a_i$ は零です。 Z は M で閉じているため (微分可能および解析的多様体、結果$, 5.3.5$)$, V\cap (M$ **--** Z) は $x$ の近傍です。この近傍、$r_a^0(y) =i$ のすべての点 $y$ に対して。

(iv) 写像 $r_a-r_a^0$ は上部半連続であり、任意の点におけるその値は $\geq 0$ です。 $r_a(x) =r^0_a(x),r_a-r^0_a$ が $x$ の近傍で零である場合、(iii) により $r_a$ が $x$ の近傍で定数であることがわかります。逆に、$x$の近傍で$r_a$が一定であれば、(ii)により$r_a^0(x) =r_a(x)$になります。 点 $x\in M$ の集合は、$r_a^0(x) =r_a(x)$ が M のオープン部分集合 $\Omega$ になります。 $x\in M$ と $r^0_a(x)< r_a(x)$ の場合、$x$ 含むのすべての近傍点 $y$ は $r_a(y)< r_a(x)$ と $r^0_a(y) =r_a^0(x)$ になります。 $x$ の近傍ごとに、含む点 $y$ のようになります

$$
r_a(y)-r^0_a(y)< r_a(x)-r^0_a(x)
$$

したがって、$\Omega$ は M で密であることがわかります。

M が接続されており、$p$ が M 上の $r_a^0$ の値である場合、$\Omega$ の点は $a_p(x)\not= 0$ のように点 $x\in M$ になります。 $k=\mathbf{C}$ の場合、これは、$\Omega$ が付録 II の補題 3 によって接続されていることを意味します。

$\rho$ を、$k$ に対する有限次元 $n$ のベクトル空間 V に対する G の解析線型表現とします。置く

デット(T $-\rho (g) + 1$) $=a_0(g) +a_1(g)T +\cdots +a_{n-1}(g)T^{n-1}+ T^n$。

数列 $(a_0, a_1, . . . , a_{n-1},1)$ に関連付けられた写像 $r_a$ と $r_a^0$ は、それぞれ $r_{\rho}$ と $r^0_{\rho}$ で表されます。それでは、$g\in G$ 全員に対して、

$r_{\rho}(g) =$ 薄暗い $V^1(\rho (g))$

$r_{\rho}^0(g) =$ 薄暗い$_{g'\rightarrow g}$ 薄暗い$V^1(\rho (g'))$。

#### 補題 2 {#lie-vii-s4-lem-2 .statement tag=00VV}

$0\rightarrow V'\rightarrow V\rightarrow V''\rightarrow 0$ を、それぞれ G の解析線型表現 $\rho ', \rho , \rho ''$ によって定義される G モジュールの完全系列とします。次に:

$r_{\rho}=r_{\rho'}+r_{\rho''}$、および$r^0_{\rho}=r^0_{\rho'}+r^0_{\rho''}$。

実際、すべての $g\in G$ について、 (§1, no. 1、Th.1 の Cor. 3 ) 完全系列が存在します。

$$
0\rightarrow (V')^1(\rho '(g))\rightarrow V^1(\rho (g))\rightarrow (V'')^1(\rho ''(g))\rightarrow 0
$$

これは最初の主張を証明します。 2 番目は、G の密なオープン部分集合で補題 1 (iv)、$r^0_{\rho}=r_{\rho}, r^0_{\rho'}=r_{\rho'}$、および $r_{\rho''}^0=r_{\rho''}$ によって続きます。

#### 定義 1 {#lie-vii-s4-def-1 .statement tag=00VW}

元 $g\in G$ は、線型表現 $\rho$ の場合、$r_{\rho}(g) =r^0_{\rho}(g)$ の場合はレギュラーと呼ばれます。

#### 命題 1 {#lie-vii-s4-prop-1 .statement tag=00VX}

G の分析線型表現 $\rho$ に対する通常の点は、近傍の G の点であり、そのうち $r_{\rho}$ は定数です。それらは G の密なオープン部分集合を構成します。 $k=\mathbf{C}$ と G が接続されている場合、$\rho$ の通常の点の集合が接続されます。

これは補題 1 (iv) から続きます。

#### 注意 {#lie-vii-s4-n1-rem-1 .statement tag=00VY}

$G^*$ を G のオープン部分群とします。 元 $a\in G^*$ は、線型表現 $\rho |G^*$ に対して $G^*$ の正則元である場合に限り、G の線型表現 $\rho$ に対して G の正則元です。

### 2. リー群中正則元

#### 定義 2 {#lie-vii-s4-def-2 .statement tag=00VZ}

G の元が、G の随伴表現に対して正則であれば、正則であると言われます。

他の語 (提案 1) では、G の $g$ の近傍のすべての元 $g'$ について、Ad($g'$)$-1$ の nilspace の次元が以下に等しい場合、元 $g\in G$ は正規です。 Ad($g$)$-1$のゼロスペースの次元。

#### 命題 2 {#lie-vii-s4-prop-2 .statement tag=00W0}

$G'$ を $k$ 上の有限次元リー群とし、$f$ を G から $G'$ までの開いた射とします。 Gの正則元の$f$の下の像は、$G'$の正則元です。 $f$の核がGの中心に含まれる場合、元$g\in G$は$f(g)$が正則である場合に限り正則です。

確かに、$\mathfrak{g}'$ を $G'$ のリー代数とし、$Tf|\mathfrak{g}$ の核によって与えられる $\mathfrak{g}$ の理想を $\mathfrak{h}$ とします。 $\rho$ を、すべての $g\in G$ について $\rho (g) =$ Ad $g|\mathfrak{h}$ によって定義される $\mathfrak{h}$ 上の G の線型表現とし、Ad $\circ f$ を、$f$ と随伴項の合成によって与えられる $\mathfrak{g}'$ の G の線型表現とする$G'$の表現。これらの線型表現定義する完全系列の G モジュール:

$$
0\rightarrow \mathfrak{h}\rightarrow \mathfrak{g}\rightarrow \mathfrak{g}'\rightarrow 0
$$

補題 $2,r_{Ad}=r_{\rho}+r_{Ad\circ f}$までに。 $r_{Ad\circ f}=r_{Ad}\circ f$ と $f$ はオープン写像、$r_{Ad\circ f}^0=r_{Ad}^0\circ f$ であるため。その結果：

$$
r_{Ad}-r^0_{Ad}=r_{\rho}-r_{\rho}^0+ (r_{Ad}-r_{Ad}^0)\circ f
$$

従って、$g$ が正規である場合、$(r_{Ad}-r^0_{Ad})(f(g)) = 0$、つまり $f(g)$ が正規であることを意味します。 $f$の核がGの中心に含まれる場合、

$r_{\rho}(g) =r_{\rho}^0(g) =$ 薄暗い$\mathfrak{h}$ はすべて $g\in G$ です。従って、$f(g)$が正規であれば$r_{Ad}(g) =r_{Ad}^0(g)$、その他の語であれば$g$が正規となります。

#### 命題 3 {#lie-vii-s4-prop-3 .statement tag=00W1}

$G_1$ と $G_2$ を $k$ 上の 2 つの有限次元リー群とします。 $g_1$ と $g_2$ がそれぞれ $G_1$ と $G_2$ の正則元である場合に限り、$G_1\times G_2$ の元 $(g_1, g_2)$ は正規です。

条件は提案 2 により必要ですが、それで十分であることを示します。すべての$g= (g_1, g_2)\in G_1\times G_2,r_{Ad}(g) =r_{Ad}(g_1) +r_{Ad}(g_2)$に。 補題 1 (ii) を考慮すると、$r^0_{Ad}(g) =r^0_{Ad}(g_1) +r_{Ad}^0(g_2)$ となる。 $g_1$ と $g_2$ が正規である場合、$r^0_{Ad}(g_1) =$ $r_{Ad}(g_1)$ と $r^0_{Ad}(g_2) =r_{Ad}(g_2)$ は、$r^0_{Ad}(g) =r_{Ad}(g)$、つまり $g$ が正規であることを意味します。

#### 補題 3 {#lie-vii-s4-lem-3 .statement tag=00W2}

$a\in G$ と $\mathfrak{m}$ を $\mathfrak{g}$ の $\mathfrak{g}^1(a)$ の補数とします。 U を $\mathfrak{g}$ の 0 の近傍とし、U から G まで指数関数写像を計算します。 写像

$f: (x, y) \rightarrow$ (経験値 $y$)$a$(経験値 $x$)(経験値 $y$)$^{-1}$

$(\mathfrak{g}^1(a)\times \mathfrak{m})\cap U$からGは$(0,0)$のエターレです。

写像 $x \rightarrow a$(exp $x$) と $y \rightarrow$ (exp $y$)$a$(exp $y$)$^{-1}$ の 0 における接線線形写像は写像 $x \rightarrow ax$ であり、 $y \rightarrow ya-ay=a(a^{-1}ya-y)$から$\mathfrak{g}$から$T_aG =a\mathfrak{g}$まで（III, §3, no. 12章、提案46）。従って、$(0,0)$における$f$の接線写像は、$\mathfrak{g}^1(a)\times \mathfrak{m}$から$a\mathfrak{g}$まで写像$(x, y) \rightarrow ax+a(a^{-1}ya-y) =a(x+a^{-1}ya-y)$となります。この写像は単射です。確かに、$x\in \mathfrak{g}^1(a), y\in \mathfrak{m}$ かつ $x+a^{-1}ya-y$ = 0 の場合、Ad($a$)$\mathfrak{g}^1(a)\subset \mathfrak{g}^1(a)$ なので、(Ad($a$)$-1$)$y$ = Ad($a$)$x\in \mathfrak{g}^1(a)$ となります。これは、$y\in \mathfrak{g}^1(a)$、従って $y$ = 0 であることを意味します。 Ad($a$) は $\mathfrak{g}^1(a)$ で単射であるため、$x$ = 0 になります。 dim $\mathfrak{g}=$ dim$\mathfrak{g}^1(a) +$ dim $\mathfrak{m}$ であるため、これは次のことを示します。 $f$は$(0,0)$のエターレです。

#### 命題 4 {#lie-vii-s4-prop-4 .statement tag=00W3}

$a\in G$ と H を、リー代数 $\mathfrak{g}^1(a)$ を伴う G の嘘部分群胚芽とする。 $H\times G$からGまでの写像$(b, c) \rightarrow cabc^{-1}$は$(e, e)$で水没です。

実際、$\mathfrak{m}$ を $\mathfrak{g}$ の $\mathfrak{g}^1(a)$ の補数とし、$\mathfrak{g}$ の 0 の開いた近傍 U 上で定義された G の指数写像をexp します。 選ぶ U なので、exp(U $\cap \mathfrak{g}^1(a)$)$\subset H$ となります。 写像 $f: (x, y) \rightarrow$ (exp $x$, exp $y$) は、$\mathfrak{g}^1(a)\times \mathfrak{m}$ の $(0,0)$ の近傍と $H\times G$ の値に対する分析写像です。 補題 3 までに、$f$ と写像 $\varphi : (b, c) \rightarrow cabc^{-1}$ の合成は $(0,0)$ でエタールになります。したがって、$\varphi$は$f(0,0) = (e, e)$で水没となります。

#### 命題 5 {#lie-vii-s4-prop-5 .statement tag=00W4}

$a\in G$ を、G の $e$ の近傍とします。以下の性質を伴う $a$ の近傍 V が存在します。すべての $a'\in V$ に対して、次のような元 $g\in W$ が存在します。 $\mathfrak{g}^1(a')\subset$ 広告($g$)$\mathfrak{g}^1(a)$。

$\mathfrak{g}^1=\mathfrak{g}^1(a)$を入れて、$\mathfrak{g}=\mathfrak{g}^1+\mathfrak{g}^+$を広告($a$)$-1 ($§1, no. 1)のフィッティング分解とします。 H をリー代数 $\mathfrak{g}^1$ を持つ G の嘘部分群胚芽とする。すべての$h\in H$、広告($h$)$\mathfrak{g}^1\subset \mathfrak{g}^1$。 $[\mathfrak{g}^1,\mathfrak{g}^+]\subset \mathfrak{g}^+$ 以降、H には $e$ の近傍 U が存在し、すべての $h\in H$ に対して Ad($h$)$\mathfrak{g}^+\subset \mathfrak{g}^+$ となります。 Ad($a$)$-1$から$\mathfrak{g}^+$の制限は全単射なので、Ad($ah$)$-1$から$\mathfrak{g}^+$の制限がすべての$h\in U$に対して全単射となるようにUを選ぶことができます。次に、すべての $h\in U$ に対して $\mathfrak{g}^1(ah)\subset \mathfrak{g}^1(a) =\mathfrak{g}^1$ です。 命題 4 により、Int(W)($aU$) は G の $a$ の近傍になります。 $a'\in$ Int(W)($aU$) の場合、$g\in W$ と $h\in U$ を伴う $a'=g(ah)g^{-1}$ になります。したがって、$\mathfrak{g}^1(a') =$ Ad($g$)$\mathfrak{g}^1(ah)\subset$ Ad($g$)$\mathfrak{g}^1(a)$ となります。

#### 系 {#lie-vii-s4-n2-cor-1 .statement tag=00W5}

$G^*$ を G のオープン部分群とします。 $a\in G$ が正則の場合、Ad($G^*$) の下ですべての $a'\in V,\mathfrak{g}^1(a')$ が共役から $\mathfrak{g}^1(a)$ になるように、$a$ の近傍 V が存在します。

### 3. 関係と正則元のリー代数

#### 命題 6 {#lie-vii-s4-prop-6 .statement tag=00W6}

V を $\mathfrak{g}$ の開始値部分群とし、exp$: V\rightarrow G$ を V で定義された指数写像とします。

(i) V には 0 の近傍 W が存在し、すべての $x\in W$ に対して $\mathfrak{g}^1$(exp $x$) $=\mathfrak{g}^0(x)$ となります。

(ii) すべての $x\in \mathfrak{g}$ に対して $k=\mathbf{R}$ または $\mathbf{C},\mathfrak{g}^1$(exp $x$)$\supset \mathfrak{g}^0(x)$ の場合。

コル著第 8 章の提案 8 の 3 III, §4, no. 4、V には 0 の近傍 $V'$ が存在し、すべての $x\in V'$ に対して、exp(ad($x$)) $=\sum_{n=0}^{\infty}\frac{1}{n!}$ ad($x$)$^n$ が定義され、Ad(exp $x$) $=$ exp(ad($x$))。 $P\in k[X]$と$\alpha \in$が終了($\mathfrak{g}$)であれば、すべての$\lambda \in k$について$\mathfrak{g}^{\lambda}(\alpha )\subset \mathfrak{g}^{P(\lambda)}(P(\alpha ))$であることを確認するのは簡単です。従って、

$\mathfrak{g}^0$(広告($x$))$\subset \mathfrak{g}^1$(経験値(広告($x$))) $=\mathfrak{g}^1$(広告(経験値$x$)) $=\mathfrak{g}^1$(経験値$x$)

$x\in V'$の皆さんへ。 $k=\mathbf{R}$ または $\mathbf{C}, V =\mathfrak{g}$ の場合、$V'$ = V が取れ、これは (ii) を証明します。 (i) を証明します。 U を End($\mathfrak{g}$) の 0 の近傍とし、Log(1 $+\alpha$ ) $=\sum_{n>0}(-1)^{n+1 1}_{\overline{n}}\alpha^n$ がすべての $\alpha \in U$ に対して定義されるようにします。次に、0 の近傍で $\circ$ exp = 1 をログし、すべての $\alpha \in U$ について $\mathfrak{g}^1(1 +\alpha )\subset \mathfrak{g}^0$(Log(1 $+\alpha$ )) を計算します。 W を $x\in V'$ のうち $\mathfrak{g}$ からなるの 0 の近傍とし、exp ad $x\in 1 + U$ とします。

Log(exp(ad($x$))) $=$ ad($x$)。

それでは、$x\in W$ 全員に対して、

$\mathfrak{g}^1$(exp $x$) $=\mathfrak{g}^1$(広告(exp $x$)) $=\mathfrak{g}^1$(exp(ad($x$)))

$\subset \mathfrak{g}^0$(Log(exp(ad($x$)))) $=\mathfrak{g}^0$(ad($x$)) $=\mathfrak{g}^0(x)$。

これは、すべての $x\in W$ に対して $\mathfrak{g}^1$(exp $x$) $=\mathfrak{g}^0(x)$ であることを示しています。

#### 補題 4 {#lie-vii-s4-lem-4 .statement tag=00W7}

U を $\mathfrak{g}$ の 0 の近傍とし、U から G まで指数関数写像を計算し、U の点ごとにエタールを計算し、すべての $x\in U$ について $\mathfrak{g}^1$(exp $x$) $=\mathfrak{g}^0(x)$ とします。

(i) 写像 $r^0_{Ad}$ は定数で、exp(U) の $\mathfrak{g}$ の階数に等しい。

(ii) $x\in U$ の場合、exp $x$ は、$x$ が $\mathfrak{g}$ の正則元である場合に限り、正規になります。

(iii) 元 $a\in$ exp(U) は、$\mathfrak{g}^1(a)$ が $\mathfrak{g}$ のカルタン部分代数である場合に限り正規です。

$l=$ rk($\mathfrak{g}$) にしましょう。 $x\in U$ が $\mathfrak{g}$ の正則元である場合、

$r_{Ad}$(経験値$x$)$=$薄暗い$\mathfrak{g}^1$(経験値$x$)$=$薄暗い$\mathfrak{g}^0(x) =l$。

Uに対する$\mathfrak{g}$所属の正則元は$x$の近傍を構成し、expは$x$でエタールであるため、これはexp$x$が正規であり、$r^0_{Ad}$(exp$x$)であることを示しています。 $=l$。 $\mathfrak{g}$ 所属の正則元から U が密であるため、すべての $a\in$ exp(U) に対して $r^0_{Ad}(a) =$ $l$ が得られます。 $a\in$ exp(U) を G の正則元とし、$x\in U$ を $a=$ exp $x$ となるようにします。 $\mathfrak{g}^0(x) =\mathfrak{g}^1(a)$から、薄暗い$\mathfrak{g}^0(x) =r^0_{Ad}(a) =l$。従って、$x$ は $\mathfrak{g}$ の正則元であり、$\mathfrak{g}^1(a)$ は $\mathfrak{g}$ のカルタン部分代数です。最後に、$a\in$ exp(U) と $\mathfrak{g}^1(a)$ が $\mathfrak{g}$ のカルタン部分代数である場合、

$r_{Ad}(a) =$ 薄暗い$\mathfrak{g}^1(a) =l=r_{Ad}^0(a)$,

なので$a$はレギュラーです。

#### 命題 7 {#lie-vii-s4-prop-7 .statement tag=00W8}

V を G の $e$ の近傍とします。 $\mathfrak{g}$ のすべてのカルタン部分代数は形 $\mathfrak{g}^1(a)$ で、$a$ は G 所属 ～ V の正則元です。

提案 6 により、$\mathfrak{g}$ に 0 の開近傍 U と、補題 4 の指数関数写像 exp$: U\rightarrow G$ 満たす条件が存在します。 $\mathfrak{h}$ が $\mathfrak{g}$ のカルタン部分代数である場合、 $\mathfrak{h}=\mathfrak{g}^0(x) ($§3 となる正則元 $x\in \mathfrak{h}$ が存在します。 2)。 一方、$tx\in U$ と exp($tx$)$\in V$ となる元 $t\in k^*$ が存在します。 次に、$\mathfrak{h}=\mathfrak{g}^0(x) =\mathfrak{g}^0(tx) =\mathfrak{g}^1$(exp($tx$))、補題 4 (ii)により、exp($tx$)はGの正則元になります。

#### 命題 8 {#lie-vii-s4-prop-8 .statement tag=00W9}

$l$ を $\mathfrak{g}$ の階数とします。次のような G の開いた部分群 $G^*$ が存在します。

(i) 写像 $r^0_{Ad}$ は $G^*$ で定数であり、その値は $l$ です。

(ii) 元 $a\in G^*$ は、$\mathfrak{g}^1(a)$ が $\mathfrak{g}$ のカルタン部分代数である場合にのみ正規です。

(iii) $a\in G^*$ の場合、$\mathfrak{g}^1(a)$ のすべてのカルタン部分代数は $\mathfrak{g}$ のカルタン部分代数になります。

(i) 提案 6 により、$\mathfrak{g}$ の 0 の開近傍 U と、U から G 満たす条件の補題 4 への指数関数写像 exp が存在します。 以下では、$k=\mathbf{R}$ または $\mathbf{C}$ の場合、$G^*$ は G の恒等性成分を表し、$k$ がウルトラメトリックである場合、exp(U) に含まれる G のオープン部分群を表します。 $r_{Ad}^0$ は局所的に定数であり、exp(U) の任意の点におけるその値は $l$ (補題 4 (i)) であるため、$r_{Ad}^0$ は定数であり、$G^*$ 上の $l$ に等しいということになります。

(ii) $R^*$ (それぞれ $S^*$) を $G^*$ の正則元の集合とする (それぞれ元 $a\in G^*$ の集合で、$\mathfrak{g}^1(a)$ は $\mathfrak{g}$ のカルタン部分代数となる)。 次に$S^*\subset R^*$。 確かに、$a\in S^*$ の場合は、$r_{Ad}(a) =l=r^0_{Ad}(a)$ になります。 $R^*\subset S^*$ であることを示します。 $k$ がウルトラメトリックである場合、これは、$G^*\subset$ exp(U) および補題 4 (iii) を包含することから導き出されます。 $k=\mathbf{C}$ と仮定します。 コルによって。提案 5 の、$a\in R^*$ の場合、$a,\mathfrak{g}^1(a')$ の近傍に属するすべての $a'$ は、$\mathfrak{g}$ の自己同型により $\mathfrak{g}^1(a)$ に共役になります。 これは、$S^*$ と $R^*$ **--** $S^*$ が $G^*$ の部分集合を開いていることを証明します。 $e$ の近傍で $S^*$ 含むがすべて正則元 (補題 4 (iii)) であることがわかりました。従って、$S^*$ は空ではありません。 $G^*$ が接続されているため、$R^*$ (提案 1) も接続され、その結果、$S^*= R^*$ も接続されます。

$k=\mathbf{R}$ のケースを研究することは残っています。まず、$G^*$ が $\mathbf{G}\mathbf{L}(E)$ の積分部分群であると仮定します。ここで、E は有限次元の実数ベクトル空間を表します。 $G^*_c$ を $\mathbf{G}\mathbf{L}(E\otimes_{\mathbf{R}}\mathbf{C})$ とリー代数 $\mathfrak{g}_c=\mathfrak{g}\otimes \mathbf{C}$ の積分部分群とします。 $G^*_c$ には解析的写像が存在します。その零の集合は、$G^*_c$ の正則元のオープン集合の補数です。 Differentiable and Analytic 多様体、結果、3.2.5 により、この写像できないは $G^*$ の点ごとに消えます。その結果、$G^*_c$ の $G^*$ 含む正則元となります。 Ad$_c$ を $G^*_c$ の随伴物表現とします。 $a\in G^*,\mathfrak{g}^1_c(a) =\mathfrak{g}^1(a)\otimes \mathbf{C}$ の場合は、$r_{Ad_c}(a) =r_{Ad}(a)$ になります。 $a\in G^*$が$G^*_c$の正則元である場合、これは$G^*$と$r_{Ad}^0(a) =r_{Ad}^0(a)$の正則元です。 写像 $r^0_{Ad}$ と $r_{Ad}^0$ は、それぞれ $G^*_c$ と $G^{^c*}$ で定数であるため、$G^*$ の正則元$^{^c}$ は、$G^*_c$ 所属の正則元であることがわかります。 $G^*$。上記より、$a$が$G^*,\mathfrak{g}^1_c(a) =\mathfrak{g}^1(a)\otimes \mathbf{C}$の正則元であれば、$\mathfrak{g}_c$のカルタン部分代数になります。これは、$\mathfrak{g}^1(a)$ が $\mathfrak{g}($§2 のカルタン部分代数であることを意味します、提案 3)。

ここで、G が単純に接続されていると仮定します。有限次元実数ベクトル空間 E と、G から $\mathbf{G}\mathbf{L}(E)$ の積分部分群 $G'$ までのエタール射 $f$ が存在します (Chap. III, §6, no. 1、Cor. of Th. 1)。提案 2 より、$a\in G$ が正規であれば、$f(a)$ も正規です。上記により、${\mathfrak{g}'}^1(f(a))$ はリー代数のカルタン部分代数 $G'$ の $\mathfrak{g}'$ です。 ${\mathfrak{g}'}^1(f(a)) = (Tf)\mathfrak{g}^1(a)$と$Tf$は$\mathfrak{g}$から$\mathfrak{g}'$までの同型なので、$\mathfrak{g}^1(a)$は$\mathfrak{g}$のカルタン部分代数であることが証明されます。

最後に一般的なケース$(k=\mathbf{R})$に移ります。 $\widetilde{G}$ を $G^*, \widetilde{\mathfrak{g}}= L( \widetilde{G})$ の普遍的なカバーとし、$q$ を $\widetilde{G}$ から $G^*$ までの正規の写像とします。 $q$の核は$\widetilde{G}$の中心に含まれるので、$a\in G^*$が正則で、$a'\in q^{-1}(a)$であれば、$a'$が正則となります(提案2)。上記により、$\widetilde{\mathfrak{g}}^1(a')$は$\widetilde{\mathfrak{g}}$のカルタン部分代数になります。 $\mathfrak{g}^1(a) = (Tq)\widetilde{\mathfrak{g}}^1(a')$ と $Tq$ は $\widetilde{\mathfrak{g}}$ から $\mathfrak{g}$ までの同型であるため、$\mathfrak{g}^1(a)$ は $\mathfrak{g}$ のカルタン部分代数であることが証明されます。

(iii) 提案 5 により、$a$ の近傍 V が存在し、すべての $a'\in V,\mathfrak{g}^1(a')$ は、$\mathfrak{g}$ の自己同型により、$\mathfrak{g}^1(a)$ の共役 ～ 部分代数となる。 $a$ 含む正則元の $G^*$ の各近傍なので、(ii) から $\mathfrak{g}$ の $\mathfrak{g}^1(a)$ 含むカルタン部分代数が求まります。したがって、§3 の提案 3 により、$\mathfrak{g}^1(a)$ のすべてのカルタン部分代数は $\mathfrak{g}$ のカルタン部分代数になります。

#### 注意 {#lie-vii-s4-n3-rem-1 .statement tag=00WA}

$k=\mathbf{C}$、部分代数 $\mathfrak{g}^1(a)$、通常の $a$ および接続された G の成分 M に対する所属は、Int($\mathfrak{g}$) の下で共役になります。確かに、R を G の正則元の集合とします。すべての $a\in R\cap M$ について、$M_a$ をそれらの $b\in R\cap M$ の集合とし、$\mathfrak{g}^1(a)$ は Int($\mathfrak{g}$) で共役から $\mathfrak{g}^1(a)$ になります。 Int($\mathfrak{g}$) $=$ Ad(G$^0$) があり、$G^0$ は G の単位成分です。系によって Prop. $5, M_a$ は R で開いています。したがって、$M_a$ は R で開いていて閉じています。 $k=\mathbf{C}, R\cap M$ は接続されています (補題 1)、したがって $M_a= R\cap M$ です。

### 4. 小学校への応用自己同型

#### 命題 9 {#lie-vii-s4-prop-9 .statement tag=00WB}

$k$ を特性 0 の体とし、$k$ に対する $\mathfrak{g}$ リー代数とします。 $a\in$ Aut$_e(\mathfrak{g})$ の場合、$a-1$ の nilspace の次元は $\mathfrak{g}$ の階数以上です。

By the “Lefschetz principle” (Algebra, Chap. V, §14, no. 6, Cor. 2 of Th. $5$)$,k$ is an ascending directed union of subfields $(k_i)_{i\in I}$ which admit $\mathbf{C}$ as extension field. $(e_{\alpha})$ を $k$ 上の $\mathfrak{g}$ の基底と $\mathfrak{g}$ の $x_1, . . . , x_m$ 元とし、ad($x_1$)$, . . .$、ad($x_m$) がゼロポテント、$a=e^{ad(x_1)}. . . e^{ad(x_m)}$ であるようにします。 $c^{\gamma}_{\alpha \beta}$ を、基底 $(e_{\alpha})$ に対する $\mathfrak{g}$ の定数構造と、この基底 $(1\leq r\leq m)$ に対する $x_r$ の $(x^{\alpha}_r)$ 成分とします。 $c^{\gamma}_{\alpha \beta}$ と $x^{\alpha}_r$ がすべて属するから $k_j$ になるような添字 $j\in I$ が存在します。 $\mathfrak{g}_j=\sum_{\alpha}k_je_{\alpha}$ にしましょう。

これは $k_j$ 含む $x_1, . . . , x_m$ を超えるリー代数であり、$a$ から $\mathfrak{g}_j$ の制限 $a_j$ は $\mathfrak{g}_j$ の基本自己同型です。 $a_j$ から $\mathfrak{g}_j\otimes_{k_j}\mathbf{C}$ の拡大は、$\mathfrak{g}_j\otimes \mathbf{C}$ の初等自己同型 $a_j\otimes 1$ です。したがって、$G_j$ を、Ad($s$) $=a_j\otimes 1$ となるように、$G_j$ のリー代数 $\mathfrak{g}_j\otimes \mathbf{C}$ および $s$ 元と接続された複合体リー群とします。 対 $(G_j, s)$ に適用される提案 8 は、$a_j\otimes 1-1$ のゼロスペースが次元 $n$ であることを示しています。

$n\geq$ rk($\mathfrak{g}_j\otimes \mathbf{C}$) $=$ rk($\mathfrak{g}_j$) $=$ rk($\mathfrak{g}$)。

しかし、この無空間は、$a_j-1$ や $a-1$ と同じ次元を持ちます。したがって命題です。

### 練習問題 {#lie-vii-s4-exercises}

記法と仮定は No. のものです。 §4の1、2、3。

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
