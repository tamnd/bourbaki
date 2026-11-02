---
book: alg
book_title: Algebra
chapter: IV
chapter_title: POLYNOMIALS AND RATIONAL FRACTIONS
section: 4
section_title: Formal power series
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A IV.24-A IV.41, A IV.90-A IV.91
pdf_pages: 0033-0050, 0099-0100
extraction: ocr
subsections:
    - "no": 1
      title: Definition of formal power series. Order
      page: 24
      pdf_page: 33
    - "no": 2
      title: Topology on the set of formal power series. Summable families
      page: 25
      pdf_page: 34
    - "no": 3
      title: Substitutions
      page: 28
      pdf_page: 37
    - "no": 4
      title: Invertible formal power series
      page: 30
      pdf_page: 39
    - "no": 5
      title: Taylor's formula for formal power series
      page: 31
      pdf_page: 40
    - "no": 6
      title: Derivations in the algebra of formal power series
      page: 32
      pdf_page: 41
    - "no": 7
      title: The solution of equations in a formal power series ring
      page: 35
      pdf_page: 44
    - "no": 8
      title: Formal power series over an integral domain
      page: 38
      pdf_page: 47
    - "no": 9
      title: The field of fractions of the ring of formal power series in one indeterminate over a field
      page: 38
      pdf_page: 47
    - "no": 10
      title: Exponential and logarithm
      page: 39
      pdf_page: 48
statements: 23
exercises: 8
errata:
    - says: imply $w(v_\nu) \geq |\nu| + 1$
      read: imply $\omega(v_\nu) \geq |\nu| + 1$
      why: The order function of a formal power series is omega throughout this no., and the same sentence sets it round once and roman once — "the relations omega(g_i) >= 2 imply w(v_nu) >= |nu| + 1" on page 44. The French of 2007 (A IV.30) sets omega in both places. The reading is faithful to the page; it is the page that changes letter in the middle of a line.
    - says: we have $w(u) \geq w(u) + 1$, which is impossible if $u \neq 0$ because $w(u)$ would then be a positive integer
      read: we have $\omega(u) \geq \omega(u) + 1$, which is impossible if $u \neq 0$ because $\omega(u)$ would then be a positive integer
      why: Same object, same page, three more times in roman. The argument is about the order of u, which the no. defines as omega and which formula (23) is stated with.
    - says: We thus have $w(v - T(u)) \geq n + 1$
      read: We thus have $\omega(v - T(u)) \geq n + 1$
      why: Page 45 sets "We thus have w(v - T(u)) >= n + 1" on one line and "we thus have omega(v - T(u)) >= n" on the next, of the same quantity in the same induction. One of the two is a slip and it is the roman one, because the definition and the French both read omega.
    - says: then $w(u^{-1}) = -w(u)$. \* In other words (Comm. Alg., VI, § 3, No. 6, p. 392, Def. 3), w is a normalized discrete valuation
      read: then $\omega(u^{-1}) = -\omega(u)$. \* In other words (Comm. Alg., VI, § 3, No. 6, p. 392, Def. 3), $\omega$ is a normalized discrete valuation
      why: Page 48 runs the roman w twice in the displayed relation and once in the sentence naming the valuation, then sets "omega(u) >= n" round two lines below for the same function. The valuation of K((X)) is omega, as the French of 2007 (A IV.36) has it.
content_sha256: 3df403eaf998879e8b55aee95bfe3305a5a01f084c1b070fe50bebaeb8f0157a
translated_from: content/en/alg/IV/04_s4_formal_power_series.md
translation_method: google
source_content_sha256: ecc1c2d36748dfed392a2d0bff5cf730d1aaf97675f112d959e7b8c05ce7ab7f
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 6a4e982524d6f2700f45554b06871252b3b77f0bd9ae4c6749fb0ec0b0bbfa44
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 4。フォーマル冪系列

### 1. 正式な冪系列の定義。 位数

Iを集合とします。 A 上のモノイド $N^{(I)}$ の合計代数は、不定数* $X_i \ (i \in I)$ (または不定数内) に関して形式的冪系列の *代数と呼ばれることを思い出します (III、p. 454、および 456)。 $X_i$) *係数を* A. $A[[X_i]]_{i \in I}$ または $A[[((X_i)_{i \in I}]]$ または $A[[X]]$ で示され、X によって家族 $(X_i)_{i \in I}$ が示されます。この段落では主に記法 $A[[I]]$ を使用します。 ときどき Iの元の$A[[I]]$の標準像を$Y_i, Z_i, T_i, \ldots$など$X_i$以外の記号で指定すると便利です。この場合に使用される規則は、多項式 (IV、p. 1) の規則に似ています。 代数 $A[[I]]$ は、$A[[Y_i]]_{i \in I}$ または $A[[Y]]$ などによって指定されます。

I が p 元の有限集合であるとき、$A[[I]]$ は p 不定数の形式的冪系列の代数であるとも言います。 These algebras are all isomorphic, for fixed p. An algebra of formal power series in 1, 2, ... indeterminates will also be denoted by $A[[X]]$, $A[[U, V]]$, ..., the set I of indices not being specified.

正式な冪系列 u は、慣習的に $u = \sum_{\nu \in N^{(I)}} a_\nu X^\nu$ (cf. IV, p. 1) と書かれます。

$\alpha_\nu$ は $u$ の *係数* です。それらは無限に多く存在する可能性があります $\neq 0$。 $a_\nu X^\nu$ は、$u$ の *項* と呼ばれます。 u が多項式であるためには、$u$ が項 $\neq 0$ の有限数のみを持つことが必要かつ十分です。 項 $a_\nu X^\nu$ そのような |ν| = p は合計次数 p のうち項と呼ばれます。正式な冪系列 $u_p = \sum_{|\nu|=p} \alpha_\nu X^\nu$ は、u の次数* p の * 同次成分と呼ばれます (I が有限の場合は多項式です)。 $u_0$ は、u の *定数項* とも呼ばれる A の元と識別されます。 $u = u_p$ の場合、u は次数 p と同次であると言います。 $u, v \in \mathbf{A}[[\mathrm{I}]]$ と $w = uv$ の場合、

(1)
$$
w_p = \sum_{q+r=p} u_q v_r
$$
整数 $p \geq 0$ ごとに。

(III, p. 456)、正式な冪系列 $u \neq 0$ の *位数* $\omega(u)$ は、$u_p \neq 0$ となる最小の整数 p であることを思い出してください。私たちは、条約により、Z 元 $\infty$ および拡大する位数関係および加法に Z から $Z \cup \{\infty\}$ まで隣接することに同意するものとします。
$$
n < \infty,\quad \infty + \infty = \infty,\quad \infty + n = n + \infty = \infty
$$
$n \in Z$ごとに; $\omega(0) = \infty$も入れました。これらの規則により、関係となります。
$$
\begin{align*}
\omega(u+v) &\geq \inf(\omega(u), \omega(v)), \\
\omega(u+v) &= \inf(\omega(u), \omega(v)) \text{ if } \omega(u) \neq \omega(v), \\
\omega(uv) &\geq \omega(u) + \omega(v),
\end{align*}
$$
正式な冪系列 $u$ および $v$ の $\mathbf{A}[[\mathrm{I}]]$ に対応します。

III、p. 457)、I の任意の部分集合 J に対して、$\mathbf{A}[[\mathrm{I}-J]] [[\mathrm{J}]]$ を使用して同一視する $\mathbf{A}[[\mathrm{I}]]$ となり、形式的な冪の定義する位数 $\omega_J(u)$ が可能になります。 $X_j$ ($j \in J$) に対しては系列、$X_j$ ($j \in J$) に対しては $u$ の同種の成分など。

$\varphi$をAの準同型から環Bにします。それぞれの形式を冪系列$u = \sum \alpha_\nu X^\nu$にすることで、$\mathbf{A}[[\mathrm{I}]]$の拡大する$\varphi$から準同型$\overline{\varphi}$を$B[[\mathrm{I}]]$とします。 対応するから正式な冪系列 $\sum \varphi(\alpha_\nu) X^\nu$;後者は、形式的な冪系列* u の *適用* $\varphi$ *to 係数によって得られると言います。 $\overline{\varphi}(u)$ をときどき $^\varphi u$ と書きます。

特に、A が B の部分環であり、A から B への $\varphi$ 標準単射である場合、$\mathbf{A}[[\mathrm{I}]]$ の $B[[\mathrm{I}]]$ への準同型 $\overline{\varphi}$ は単射です。一般に、$\overline{\varphi}$ を使用して、$B[[\mathrm{I}]]$ の同一視する $\mathbf{A}[[\mathrm{I}]]$ を部分環とします。

### 2. 正式な冪系列の集合に位相。加算可能なファミリー

定義 $\mathbf{A}[[\mathrm{I}]]$ によって、それは積集合 $\mathbf{A}^{N^{(I)}}$ に他なりません。反対の明示的な言及を除き、A には個別の位相を、$\mathbf{A}[[\mathrm{I}]]$ には積位相 (Gen. Top. I, p. 31 f.) を装備し、これを正規の位相と呼びます。 加法と個別の位相を備えた$A$ は、分離された完全なトポロジー 群です。したがって、加法の $A[[I]]$ は、分離された完全なトポロジカル群 (Gen. Top.、III、p. 238 および 242、および Gen. Top.、II、p. 187) です。さらに、多項式の代数 $A[(X_i)_{i \in I}]$ は $A[[I]]$ (Gen. Top., III p. 238, Prop, 25) に密集しているため、$A[[I]]$ を $A[(X_i)_{i \in I}]$ の完成と考えることができます。

それぞれの $\beta \in \mathbf{N}^{(I)}$ について、$S_\beta$ を、$\nu \leq \beta$ のような複数のインデックス $\nu$ の集合とし、$a_\beta$ を、次のような正式な冪系列 $u = \sum \alpha_\nu X^\nu$ の集合とします。 $\nu \in S_\beta$の場合は$a_\nu = 0$。明らかに、$S_\beta$ は $\mathbf{N}^{(I)}$ の有限部分集合であり、$\mathbf{N}^{(I)}$ のすべての有限部分集合は形 $S_\beta$ の集合に含まれます。したがって、ファミリー $(a_\beta)_{\beta \in \mathbf{N}^{(I)}}$ は、$A[[I]]$ の 0 の近傍の基本的な系です。 集合 $a_\beta$ は $A[[I]]$ のイデアルであるため、(Gen. Top.、III、p. 275) $A[[I]]$ はトポロジカル環です。

#### 補題 1 {#alg-iv-s4-lem-1 .statement tag=06BY}

$L$ を無限の集合とし、$(u_\lambda)_{\lambda \in L}$ を $A[[I]]$ の元の族とし、$\lambda \in L$ に $u_\lambda = \sum \alpha_{\lambda,\nu} X^\nu$ を代入します。したがって、次の条件は同等です。
(i) ファミリ $(u_\lambda)_{\lambda \in L}$ は、$A[[I]]$ で合計可能です (Gen. Top.、III、p. 262)。
(ii) $L$ の有限部分集合の補数の *フィルター* に従って、$\lim u_\lambda = 0$ が得られます。
(iii) 添字 $\lambda \in L$ の *有限* 数を除いて、すべての $\nu \in \mathbf{N}^{(I)}$ に対して $\alpha_{\lambda,\nu} = 0$ があります。

これらの条件が成立すると、系列 $u = \sum_{\lambda \in L} u_\lambda$ は、$\nu \in \mathbf{N}^{(I)}$ ごとに $a_\nu = \sum_{\lambda \in L} \alpha_{\lambda,\nu}$ を含む $\sum \alpha_\nu X^\nu$ に等しくなります。

(i) と (ii) の同値は Cor. Gen.Top.の2、III、p. 263。
(ii) および (iii) の同値は、積空間 (Gen. Top.、I、p. 55、Cor. 1) の極限の特性から派生します。
最後の主張は、Gen. Top. の提案 4、III、p. 266 に続きます。

要約可能なファミリーをいくつか例挙げてみましょう。
a) $u \in A[[I]]$ とし、$a_\nu$ を $u$ の $X^\nu$ の係数とします。ファミリ $(\alpha_\nu X^\nu)_{\nu \in \mathbf{N}^{(I)}}$ は、和 $u$ で合計可能です (これにより、$u = \sum \alpha_\nu X^\nu$ と書くことが正当化されます)。

b) $u \in A[[I]]$ とします。すべての整数 $p \geq 0$ について、$u_p$ を次数 $p$ の$u$ の同次成分とします。次に、家族 $(u_p)_{p \geq 0}$ は合計可能で、$u = \sum_{p \geq 0} u_p$ になります。

c) $(u_\lambda)_{\lambda \in L}$ を $A[[I]]$ の元の族とし、$\lambda \in L$ のすべての整数 $n \geq 0$ 集合について、$\omega(u_\lambda) < n$ が有限であると仮定します。すると、家族 $(u_\lambda)_{\lambda \in L}$ は合計可能です。

#### 注意 {#alg-iv-s4-n2-rem-1 .statement tag=06BZ}

— $I$ が *有限* であると仮定します。すべての整数 $n \geq 0$ について、$b_n$ を正式な冪系列 $u \in A[[I]]$ の集合とし、$\omega(u) \geq n$ とします。 数列 $(b_n)_{n \geq 0}$ は、$\mathbf{A}[[\mathbf{I}]]$ の 0 の近傍の基本的な系です。したがって、$\mathbf{A}[[\mathbf{I}]]$ ($\lambda \in L$) の元 $u_\lambda$ の族は、$\omega(u_\lambda) < n$ が有限であるような $\mathbf{A} \in L$ のすべての $n \in \mathbf{N}$ 集合について、かつその場合に限り、合計可能です。

#### 命題 1 {#alg-iv-s4-prop-1 .statement tag=06C0}

*$(u_\lambda)_{\lambda \in L}$ *と* $(v_\mu)_{\mu \in M}$ *を* $\mathbf{A}[[\mathbf{I}]]$の元の2つの合計可能な族とします。 *その後、家族* $(u_\lambda v_\mu)_{(\lambda, \mu) \in L \times M}$ *合計可能で、次のようになります*

$$
\sum_{(\lambda, \mu) \in L \times M} u_\lambda v_\mu = \left( \sum_{\lambda \in L} u_\lambda \right) \left( \sum_{\mu \in M} v_\mu \right)
$$

$(\alpha_{\lambda, \nu})_{\nu \in \mathbf{N}^{(I)}}$ (それぞれ $(\beta_{\mu, \nu})_{\nu \in \mathbf{N}^{(I)}}$) を、$u_\lambda$ (それぞれ $v_\nu$) の係数の家族とします。それぞれの $\nu \in \mathbf{N}^{(I)}$ には、$\nu_1 + \nu_2 = \nu$ のような対 $(\nu_1, \nu_2) \in \mathbf{N}^{(I)} \times \mathbf{N}^{(I)}$ の有限の数のみが存在するため、$X^\nu$ の係数となるような対 $(\lambda, \mu) \in L \times M$ の有限の数のみが存在します。 $u_\lambda v_\mu$は$\neq 0$です。したがって、族 $(u_\lambda v_\mu)_{(\lambda, \mu) \in L \times \mathscr{J}}$ は合計可能です。ここで、公式 (2) は、和 (Gen. Top.、III、p. 265、公式 (2)) の結合性から続きます。

$\mathbf{A}[[\mathbf{I}]]$ では、積は結合的で可換な合成法則です。したがって、$\mathbf{A}[[\mathbf{I}]]$ の元の *積* の *積* について話すことができます (Gen. Top., III, p. 262, 注意 3)。

#### 命題 2 {#alg-iv-s4-prop-2 .statement tag=06C1}

*$(u_\lambda)_\lambda$ *を * $\mathbf{A}[[\mathbf{I}]]$ の元の合計可能な族とします。
(i) *家族* $(1 + u_\lambda)_\lambda$ *乗算可能です*。
(ii) *$\mathfrak{T}$ *$L$ のすべての有限部分集合のうち集合とします。 *任意の* $M \in \mathscr{S}$ *置く* $u_M = \prod_{\lambda \in M} u_\lambda$。 *その後、家族* $(u_M)_{M \in \mathfrak{T}}$ *合計可能で、次のようになります*

$$
\sum_{M \in \mathfrak{T}} u_M = \prod_{\lambda \in L} (1 + u_\lambda).
$$

この番号の冒頭のように理想を定義する $\mathfrak{a}_\beta$ とし、$\beta \in \mathbf{N}^{(I)}$ とします。 $\lambda \notin L_0$ に対して $u_\lambda \in \mathfrak{a}_\beta$ となるような $L$ の有限部分集合 $L_0$ が存在します。次に、$M \not\subset L_0$ となるすべての $M \in \mathscr{S}$ に対して、$u_M \in \mathfrak{a}_\beta$ が得られます。したがって、家族 $(u_M)_{M \in \mathfrak{T}}$ は合計可能です。一方、$L$ の任意の有限部分集合 $M_0$ については、

$$
\sum_{M \subset M_0} u_M = \prod_{\lambda \in M_0} (1 + u_\lambda).
$$

フィルタリングされた順序集合 $\mathfrak{T}$ に沿って取得すると、左側は極限 $\sum_{M \in \mathfrak{T}} u_M$ になります。したがって、右辺は極限 $\sum_{M \in \mathfrak{T}} u_M$ となり、(i) と (ii) を同時に証明します。

#### 命題 3 {#alg-iv-s4-prop-3 .statement tag=06C2}

*$u = \sum a_\nu X^\nu \in \mathbf{A}[[\mathbf{I}]]$ *そして* $m$ *整数* $> 0$ とします。 *すべて* $n \in \mathbf{N}$ * $(\alpha_{\nu, n})_{\nu \in \mathbf{N}^{(I)}}$ * $u^n$ の係数の家族にしましょう。 *$\alpha_0^m = 0$ の場合、*その後* $\alpha_{\nu, n} = 0$ *$n \geq |\nu| + m$ の場合。

$\nu \in \mathbf{N}^{(I)}$ と $n \in \mathbf{N}$ としましょう。我々は持っています

$$
\alpha_{\nu,n} = \sum_{\nu(1) + \cdots + \nu(n) = \nu} \alpha_{\nu(1)} \cdots \alpha_{\nu(n)} .
$$

$n \geq |\nu| + m$ と $\nu(1) + \cdots + \nu(n) = v$ の場合、$|\nu(1)| + \cdots + |\nu(n)| \leq n - m$ になります。したがって、$r$ の少なくとも $m$ の異なる値に対して、$v(r) = 0$ と $\alpha_{v(r)} = a_r$ が得られます。結果は $\alpha_{\nu(1)} \cdots \alpha_{\nu(n)} = 0$、よってになります。

#### 系 {#alg-iv-s4-n2-cor-1 .statement tag=06C3}

— $u \in A[[I]]$ としましょう。その場合、$\lim_{n \to \infty} u^n = 0$ が維持されるためには、$u$ の定数項がゼロであることが必要かつ十分です。

$a_0$ を $u$ の定数項とします。 $u^n$ の定数項は $\alpha_0^n$ であるため、前述の条件が必要です。提案 3 によって十分です。

### 3. 交代

$E$ を $A$-代数 とします。 $E$ 上の位相は、変換下で不変であり、$E$ の理想の 0 からなるの近傍の基本系が存在する場合、線形であると言われます (Gen. Top.、III、p. 223)。 $E$ 上の位相は、その $A$-代数構造と互換性があります ($A$ が離散位相を運ぶ場合)。線形位相を持つ$A$-代数は、線形トポロジ化された$A$-代数と呼ばれます。

#### 命題 4 {#alg-iv-s4-prop-4 .statement tag=06C4}

— $I$ を集合とし、$E$ を結合的、可換的、単位的、線形トポロジー化された分離完全な $A$-代数とする。

(i) $\varphi$ を $A[[I]]$ から $E$ と $x_i = \varphi(X_i)$ に連続する準同型とする。次に:
(a) すべての $i \in I$、$x_i^n$ は 0 になる傾向があり、$n$ は $+ \infty$ になる傾向があります。
(b) $I$ が無限大の場合、$x_i$ は $I$ の有限部分集合の補数のフィルターに沿って 0 になる傾向があります。

(ii) $x = (x_i)_i$、$_I$ を、(i) の $E$ 満たすの a) と b) の元の族とする。その場合、$A[[I]]$ から $E$ への単位連続準同型 $\varphi$ が 1 つだけ存在し、すべての $i \in I$ に対して $\varphi(X_i) = x_i$ になります。

すべての $i \in I$ について、$n$ は $+ \infty$ になる傾向があるのと同様に、$A[[I]]$ では $X_i^n$ は明らかに 0 になる傾向があります。一方、$I$ が無限である場合、$X_i$ は $I$ の有限部分集合の補数のフィルターに沿って 0 になる傾向があります。これは(i)を証明します。

$(x_i)_{i \in I}$ を、(i) の $E$ 満たす条件 a) と b) の元の家族とし、$\psi$ を $A[(X_i)_{i \in I}]$ の準同型 $u \mapsto u((x_i)_{i \in I})$ を $E$ に、$V$ を$E$の理想である$E$の0の近傍。 b) により、すべての $i \in I - J$ に対して $x_i \in V$ となる $I$ のうち有限部分集合 $J$ が存在します。次に、a) $i \in J$ に対して $x_i^n \in V$ となるような整数 $n \geq 0$ が存在します。 $\beta$ を $\mathbf{N}^{(I)}$ の元とし、$i \in J$ は $\beta_i = n - 1$、$i \in I - J$ は $\beta_i = 0$ とします。 No. 2 (IV、p. 26) の初めのように、$A[[I]]$ の理想的な $a_\beta$ を定義するとすると、

$$
u \in A[(X_i)_{i \in I}] \cap a_\beta \Rightarrow \psi(u) \in V
$$

これは、$A[[I]]$の装備によって誘発された位相を$A[(X_i)_{i \in I}]$に装備すると、$\psi$が連続することを示しています。 $E$が分離して完了しているので、$\psi$ 拡大するから$A[[I]]$の準同型 $\varphi$が$E$に連続します。 $i \in I$全員に対して$\varphi(X_i) = \psi(X_i) = x_i$がございます。最後に、$\varphi'$を$A[[I]]$の$E$への連続単位準同型とし、$\varphi'(X_i) = x_i$とします。すべての $u \in A[(X_i)_{i \in I}]$ に対して $\varphi'(u) = \varphi(u)$ があり、$A[(X_i)_{i \in I}]$ が $A[[I]]$ に密集しているため、$\varphi' = \varphi$ になります。

前回の記法はそのままにしておきます。 $u \in A[[I]]$ の場合、$u$ by $\varphi$ の像は、$u(x)$ または $u((x_i)_{i \in I})$ ($I = (1, 2, ..., n)$ の場合は $u(x_1, ..., x_n)$) で表され、$x_i$ を代入して得られる $E$ の元と呼ばれます。 $u$の$X_i$、または値の$u$の値、$X_i$の$x_i$、または$X_i = x_i$の$u$の値。特に$u = u((X_i)_{i \in I})$があります。

$E'$ を結合的可換かつ単位線形トポロジー化された分離された完全な $A$-代数とする。 $\lambda$ を $E$ から $E'$ への連続単位準同型とし、$(x_i)_{i \in I}$ を$E$ 満たす条件の元の族とする。提案 4 (IV, p. 28）。ファミリ $(\lambda(x_i))_{i \in I}$ は、同じ条件 a) および b) を満たします。 $u \in A[[I]]$ ごとに、

$$
\lambda(u((x_i)_{i \in I})) = u((\lambda(x_i))_{i \in I}),
$$

写像 $u \mapsto A(u((x_i)_{i \in I}))$ は、$A[[I]]$ から $E'$ へ、変換 $X_i$ からすべての $i \in I$ に対して $\lambda(x_i)$ への連続単位準同型です。

$J$ と $K$ が 2 つの集合である場合、すべての家族 $(g_j)_{j \in J}$ 満たすの$A_{J, K}$ 集合によって次の条件を表します。
(i) すべての $j \in J$ について、$g_j$ は $A[[K]]$ の元であり、その定数項はゼロポテントです。
(ii) $J$ が無限である場合、$g_j$ は $J$ の有限部分集合の補数のフィルターに沿って 0 になる傾向があります。

$J$ が有限である場合、$A[[K]]$ 属するから $A_{J, K}$ までの定数項を持たない形式冪系列 $(g_j)_{j \in J}$ のすべての族に注目します。

$(g_j)_{j \in J}$を$A_{J, K}$に入れます。コルによって。提案 3 (IV、p. 28) では、すべての $j \in J$ に対して $\lim_{n \to \infty} g_j^n = 0$ が得られます。 $f \in A[[J]]$ にしましょう。 $f$ の添字 $j$ の変数に $g_j$ を代入すると、正式な冪系列 $f((g_j)_{j \in J})$ 所属から $A[[K]]$ が得られます。さらに、写像 $f \mapsto f((g_j)_{j \in J})$ は、$A$-代数 $A[[J]]$ の $A[[K]]$ への連続準同型です。

特に $J = (1, ..., p)$ と $f \in A[[X_1, ..., X_p]]$ の場合、定数項を使用せずに、それぞれの $X_j$ を正式な冪系列 $g_j \in A[[K]]$ に置き換えることができます。この置換の結果は $f(g_1, ..., g_p)$ と書き込まれます。

$x = (x_k)_{k \in K}$ を、提案 4 (IV、p. 28) の $E$ 満たす条件 a) および b) の元の族とする。 (3) を適用して、$A[[K]]$ の $A$ 準同型 $u \mapsto u(x)$ を $E$ に当てはめてみましょう。私たちは得る

$$
f((g_j)_{j \in J})(x) = f((g_j(x))_{j \in J}).
$$

$f = (f_i)_{i \in I} \in (A[[J]])^I$と$g = (g_j)_{j \in J} \in A_{J, K}$としましょう。 $(A[[K]])^I$ の $f(g)$ または $f \circ g$ 元 $(f_i((g_j),_{\epsilon_J}))_{i \in I}$ で表します。 $f \in A_{I, J}$ の場合、$A[[I]]$ の $A[[K]]$ への写像 $f \mapsto f((g_j)_{i, J})$ が連続なので、$f \circ g \in A_{,,K}$ になります。

$f \in (A[[J]])^I$、$g \in A_{J, K}$、$h \in A_{K, L}$ とします。次に $g \circ h \in A_{J, L}$ そして (4) により、次のようになります。
$$
(f \circ g) \circ h = f \circ (g \circ h).
$$

### 4. インバーチブルフォーマル冪系列

#### 命題 5 {#alg-iv-s4-prop-5 .statement tag=06C5}

— *形式的な冪系列の環 $A[[T]]$ では、多項式 $1 - T$ は可逆であり、* $(1 - T)^{-1} = \sum_{n=0}^m T^n$ が得られます。

のために
$$
(1 - T) \left( \sum_{n=0}^\infty T^n \right) = \sum_{n=0}^\infty T^n - \sum_{n=0}^\infty T^{n+1} = 1.
$$

#### 命題 6 {#alg-iv-s4-prop-6 .statement tag=06C6}

— *$u \in A[[I]]$ としましょう。従って、$u$ が $A[[T]]$ で可逆であるためには、その定数項が $A$ で可逆であることが必要かつ十分です。*

$uv = 1$となるような$v \in A[[I]]$が存在するとします。 $a, \beta$ を $u$ と $v$ の定数項とすると、$\alpha \beta = 1$ となるため、$a$ は可逆です。

逆に、$u$ の定数項 $a$ が可逆であるとします。次に、$u = \alpha (1 - t)$ と $\omega(t) > 0$ のような正式な冪系列 $t \in A[[I]]$ が存在します。ここで、$\varphi(T) = t$ となるような環準同型 $\varphi : A[[T]] \to A[[I]]$ があり、$1 - T$ は $A[[T]]$ で反転可能です (提案 5)。従って、$1 - t$ は $A[[I]]$ で反転可能であり、従って $u$ も反転可能です。

#### 注意 {#alg-iv-s4-n4-rem-1 .statement tag=06C7}

— $A$ を定数項を持つすべての形式的な冪系列の集合とします。 1. 提案 6 により、$M$ は乗法の下で可換群です。従って、$A[[I]]$の乗法群は、$M$の直接の積と$A$の乗法群です。 $A[[I]]$から派生した位相を$A$に装備します。それぞれの $\beta \in \mathbf{N}^{(I)}$ について、IV、p. 26 では、$A[[I]]$ の理想的な $a_\beta$ が定義されます。この場合、$1 + a_\beta$ は $M$ の部分群であり、ファミリー $(1 + a_{\beta'})$ は $M$ の 1 の近傍の基本的な系です。 $M$ の乗法は連続であるため、$A$ はトポロジカルな群 (Gen. Top., III, p. 223) であることがわかります。他の語では、*写像* $f \mapsto f^{-1}$ *は * $M$ に連続しています。

$K$ を $K^1$ の元 0 が代入可能である有理分数からなる有理分数 $K((X_i)_{i \in I})$ の体の可換体と $\mathscr{O}$ 部分環とします。 $f \in \mathscr{O}$ の場合、$f = \frac{u}{v}$ が得られます。ここで、$u$ と $v$ は、$v$ の定数項が $\neq 0$ となる多項式であるため、$v$ は $K[[I]]$ で可逆です。 $K[[I]]$ の元 $uv^{-1}$ が $f$ にのみ依存していることをすぐに検証できます。形式的な冪系列 $uv^{-1}$ は *有理分数の原点における展開* $\frac{u}{v}$ であると言います。 写像 $f \mapsto uv^{-1}$ は、$\mathscr{O}$ の単射準同型を $K[[I]]$ に変換します。多くの場合、同一視する $\mathscr{O}$ と、この写像の下の像が続きます。

### 5. テイラーの公式はフォーマル冪系列

$X = (X_i)_{i \in I}$ と $Y = (Y_i)_{i \in I}$ を、同じ添字集合 I に対する不定数の 2 つの族とします。 $A[[X, Y]]$ の正式な冪系列の家族 $(X_i + Y_i)_{i \in I}$ を $X + Y$ で表します。形式的な冪系列 $u \in A[[X]]$ で $X_i$ を $X_i + Y_i$ に置き換えることができ、結果は $u(X + Y)$ として書き込まれることは明らかです。それぞれの $\nu \in \mathbf{N}^{(I)}$ を、正式な冪系列 $u(X + Y)$ を所属から $A[[X]][[Y]]$ (III、p. 456) とみなして、$Y^\nu$ の $\Delta^\nu u$ 係数で表します。他の語では、

$$
u(X + Y) = \sum_\nu \Delta^\nu u(X) \cdot Y^\nu \quad (u \in A[[X]]) .
$$

$(X, Y)$ を $(0, X)$ に置き換えると、次のようになります。

$$
u(X) = \sum_\nu \Delta^\nu u(0) \cdot X^\nu ;
$$

他の語では、$\Delta^\nu u$の定数項は、$u$の$X^\nu$の係数です。 Since the mapping $u \mapsto u(X + Y)$ of $A[[X]]$ into $A[[X, Y]]$ is continuous, the mappings $u \mapsto \Delta^\nu u$ of $A[[X]]$ into itself are again continuous.

多項式 (IV、p. 7) の場合と同様に、式を証明できる

$$
\Delta^\sigma(uv) = \sum_{v+\rho=\sigma} \Delta^\nu(u) \Delta^\rho(v) ,
$$
$$
\Delta^\rho \Delta^\sigma u = \frac{(\rho + \sigma)!}{\rho! \; \sigma!} \Delta^{\rho + \sigma} u .
$$

二項公式 (I, p. 99, Cor. 2) は、$u = \sum_\lambda \alpha_\lambda X^\lambda$ のとき、$\Delta^\nu u$ に対して次の値を与えます。

$$
\Delta^\nu u = \sum_\lambda \alpha_{\lambda + \nu} \frac{(\lambda + \nu)!}{\lambda! \; \nu!} X^\lambda .
$$

特に、$\nu = \epsilon_i$、つまり$j \neq i$ の$\nu_i = 1, \nu_j = 0$ の場合を考えてみましょう。 $D_i u = \Delta^{\epsilon_i} u$ を入れます。言い換えると、$D_i u$は$u(X + Y)$の$Y_i$の係数です。 (10) により、次のようになります。

$$
D_i u = \sum_\lambda (\lambda_i + 1) \alpha_{\lambda + \epsilon_i} X^\lambda ;
$$

特に、$j \neq i$ には $D_i(X_i) = 1$ と $D_i(X_j) = 0$ があります。 公式 (8) は、$D_i$ が $A[[X]]$ の導分であることを示し、(9) から関係を推定します。

$$
D^\nu u = \nu! \; \Delta^\nu u
$$

多項式 (IV、p. 8) の場合と同様です ($\mathbf{N}^{(I)}$ の $\nu = (\nu_i)_{i \in I}$ に $D^\nu = \prod_{i \in I} D_i^{\nu_i}$ を入れています)。 A が Q 代数の場合、式 (6)、(7)、(12) は « Taylor の公式» を意味します。

$$
u(\mathbf{X} + \mathbf{Y}) = \sum \frac{1}{\nu!} D^\nu u(\mathbf{X}) \cdot \mathbf{Y}^\nu,
$$
$$
u(\mathbf{X}) = \sum \frac{1}{\nu!} D^\nu u(0) \cdot \mathbf{X}^\nu.
$$

#### 注意 {#alg-iv-s4-n5-rem-1 .statement tag=0DHH}

*1) $D_i u$ は、X* に関する u の *偏導関数である、とよく言われます。 記法 $D_{x_i} u, \frac{\partial u}{\partial x_i}$ と $u'_{x_i}$ も使用します。単一の不定X に対して、一意の偏導関数 $Du$ ($\frac{du}{dX}$ または $u'$ とも書きます) は、$u$ の *導関数* と呼ばれます。

2) 公式 (9) は、A-加群 $A[[X]]$ の自己準同型 $A^p$ が通勤痛であることを示しています。したがって、自己準同型 $D_i$ も同様です。

3) $u \in A[(X_i)_{i \in I}]$ が多項式の場合、IV、p. 6、7 一致するで定義された多項式 $A^p u$ と $D_i u$ は、形式冪系列で同じ記号で表されます。

### 6. 導分の代数の正式な冪系列

I を集合とし、E は結合的、可換的で単位線形トポロジー化され、分離され完全な A-代数、そして $x = (x_i)_{i \in I}$ は E 満たす条件の元の族、提案 4 (IV, p. 28）。 $\varphi$ を E への $A[[I]]$ の連続準同型 $u \mapsto u(x)$ とします。 E に $A[[I]]$ モジュール構造を備えています。 III, p. 552 により、$A[[I]]$ モジュール E への $A[[I]]$ の A 導出 D は、A-線型写像 $D : A[[I]] \to E$ 満たす関係となります。
$$
D(uv) = u(x) \cdot D(v) + D(u) \cdot v(x)
$$
$A[[I]]$の$u, v$用。

#### 命題 7 {#alg-iv-s4-prop-7 .statement tag=06C8}

— $(y_i)_{i \in I}$ を E の元の族とします。 I が無限であるとき、*私たちは、 I の有限部分集合の補数のフィルターに沿って $y_i$ が 0 になる傾向があると仮定します。したがって、すべての $i \in I$ に対して $D(X_i) = y_i$ となる、$A[[I]]$*モジュール* E への$A[[I]]$ の一意の連続 A 導出 D が存在します。私たちは持っています
$$
D(u) = \sum_{i \in I} (D_i u)(x) \cdot y_i \quad (u \in A[[I]]) .
$$

0 は E に理想の近傍からなるの基本的な系を認めているので、家族 $((D_i u)(x) \cdot y_i)_{i \in I}$ はすべての $u \in A[[I]]$ (Gen. Top.、III、p. 263、Cor. 2) について E で要約可能です。 公式 (16) したがって、定義する A-線型写像 $D : A[[I]] \to E$。 D が連続的な導分であることを確認するのは読者に任せます。

$D_1$ を、すべての $i \in I$ に対して $D_1(X_i) = y_i$ となるように、$A[[I]]$ から E への連続 A 微分とします。連続導分 $D - D_1$ の核は、$\mathbf{A}[[\mathbf{I}]]$ 含む 1 の閉じた部分代数 B と不定$X_i$ です。多項式代数 $\mathbf{A}[(X_i)_{i \in I}]$ は $\mathbf{A}[[\mathbf{I}]]$ で密であるため、$B = \mathbf{A}[[\mathbf{I}]]$ があり、したがって $D_1 = D$ になります。

#### 系 1 {#alg-iv-s4-prop-7-cor-1 .statement tag=06C9}

— *A を A-代数 E の連続導分とする。すべての形式的な冪系列 $u \in \mathbf{A}[[\mathbf{I}]]$ について、族 $((D_iu)(x) \cdot \Delta x_i)_{i \in I}$ は合計可能であり、*

$$
\Delta(u(x)) = \sum_{i \in I} (D_iu)(x) \cdot \Delta x_i .
$$

写像 $u \mapsto \Delta(u(x))$ は $\mathbf{A}[[\mathbf{I}]]$ モジュール E への $\mathbf{A}[[\mathbf{I}]]$ の連続導分であるため、これは提案 7 から導かれます。

#### 系 2 {#alg-iv-s4-prop-7-cor-2 .statement tag=06CA}

— *導分 $D_i$ は、A-代数 $\mathbf{A}[[\mathbf{I}]]$ の一意の連続導分であり、*

$$
D_i(X_i) = 1 , \quad D_i(X_j) = 0 \quad \text{for} \quad j \neq i .
$$

これはコルからの続きです。 1.

#### 系 3 {#alg-iv-s4-prop-7-cor-3 .statement tag=06CB}

— *$f \in \mathbf{A}[[X_1, ..., X_s]]$と$g_i \in \mathbf{A}[[Y_1, ..., Y_q]]$を$1 \leq i \leq p$とします。 $1 \leq i \leq p$について、$g_i$の定数項が零であると仮定し、$h = f(g_1, ..., g_p)$を置きます。次に、$1 \leq j \leq q$ については *

$$
\frac{\partial h}{\partial Y_j} = \sum_{i=1}^p D_i f(g_1, ..., g_p) \cdot \frac{\partial g_i}{\partial Y_j} .
$$

これは、Cor の特殊なケース $E = \mathbf{A}[[Y_1, ..., Y_s]]$、$x_i = q_i$、および $A = \partial / \partial Y_j$ です。 1.

#### 命題 8 {#alg-iv-s4-prop-8 .statement tag=06CC}

— *$X = (X_i)_i$ を不定数の有限族とする。
(i) 正式な冪系列 $\mathbf{A}[[X]]$ の環のすべての導分は連続しています。
(ii) 多項式環 $\mathbf{A}[X]$ のすべての導分を、正式な冪系列 $\mathbf{A}[[X]]$ 拡大するの環を、環 $\mathbf{A}[[X]]$ の導分に固有の方法で変換します。
(iii) 族 $(D_i)_{i \in I}$ は、$\mathbf{A}[[X]]$ の A 導出の $\mathbf{A}[[X]]$ 加群の基底です。
$b_n$ を、位数 $\geq n$ のすべての正式な冪系列の集合とします。 $b_n$ が環 $\mathbf{A}[[X]]$ のイデアルであり、次数 $n$ の単項式によって生成されることは明らかです。したがって、$b_n$ は、定数項を含まない、有限和の積の $n$ 形式冪系列で構成されます。 $D$ が $\mathbf{A}[[X]]$ の導分である場合、*

$$
D(f_1 \cdots f_n) = \sum_{i=1}^n f_1 \cdots f_{i-1} D(f_i) f_{i+1} \cdots f_n ,
$$

よって $n \geq 1$ に対して $Db_n \subset b_{n-1}$ がすぐに続きます。 数列 $(b_n)_{n \geq 0}$ は $\mathbf{A}[[X]]$ (IV, p. 26 注意) の 0 の近傍の基本系であるため、D は連続であり、(i) が証明されます。

$A$を$A[X]$の導分を$A[[X]]$とします。 前にと議論すると、次数 $n \geq 1$ のすべての同次多項式 $h$ に対して、$A(h)$ 属するから $b, -_1$ であることがわかります。ここで、$u \in A[[X]]$ を、$u_n$ を、次数 $n$ の$u$ の同次成分とします。 $n \geq 1$ に対する $A(u_n) \in b, -_1$ なので、ファミリー $(A(u)), \ldots$ は $A[[X]]$ で要約可能であり、$A[[X]]$ の定義する導分 $D$ をそれ自体にまとめることができます。

$$
D(u) = \sum_{n \geq 0} \Delta(u_n)
$$

$D(b_n) \subset b_{n-1}$ があるため、$D$ は $A[[X]]$ の加法群の連続自己準同型です。 $A[[X]] \times A[[X]]$ から $A[[X]]$ への写像 $\Phi : (u, v) \mapsto D(uv) - uD(v) - D(u)v$ は連続し、$A[X] \times A[X]$ では零になります。 $A[X]$ は $A[[X]]$ に密集しているので、$\Phi = 0$ になります。他の語では、$D$ は $A[[X]]$ の導分であり、$A$ を拡張します。

最後に、$A[X]$ は $A[[X]]$ で密であり、$A[[X]]$ のすべての導分は (i) によって連続しています。したがって、$A$ の拡大から $A[[X]]$ の導分までの一意の拡大が存在します。これは(ii)を証明します。

(iii) を証明することはまだ残っています。 公式 (18) (IV, p. 33) は、族 $(D_i)_{i \in I}$ が $A[[X]]$ に対して線形独立であることを示し、公式 (16) (IV, p. 32) は、$E = A[[X]]$ のケースに適用され、すべての$A$-派生は、$A[[X]]$に係数が入った$D_i$の線形結合です。

#### 命題 9 {#alg-iv-s4-prop-9 .statement tag=06CD}

— $(u_\lambda)_{\lambda \in L}$ を定数項のない $A[[I]]$ の元の*加算可能な*族とし、$D$ を $A$-代数 $A[[I]]$ の連続導分とします。 $f = \prod_{\lambda \in L} (1 + u_\lambda)$ (IV, p. 27, 提案 2) の場合、族 $(Du_\lambda/(1 + u_\lambda))_{\lambda \in L}$ は合計可能であり、次のようになります。

$$
D(f)/f = \sum_{\lambda \in L} D(u_\lambda)/(1 + u_\lambda) .
$$

$g$ と $h$ が $A[[I]]$ の 2 つの可逆元である場合、

$$
D(gh) = h \cdot Dg + g \cdot Dh
$$

よってを $gh$ で割ると、

$$
D(gh)/gh = D(g)/g + D(h)/h .
$$

$L$ の有限部分集合 $M$ ごとに $f_M = \prod_{\lambda \in M} (1 + u_\lambda)$ を置きます。 (21) から、カード $M$ 関係の帰納法によって推論します。

$$
D(f_M)/f_M = \sum_{\lambda \in M} D(u_\lambda)/(1 + u_\lambda)
$$

これは、L が有限である場合の提案 9 を証明します。ここで、L が無限であると仮定し、L の有限部分集合のフィルタリングされた順序付き集合に対して $\mathfrak{F}$ を書き込みます。 $\lim_{\mathfrak{F}} f_M = f$ があるので (*IV*, p. 30 注意)

$$
D(f)/f = \lim_{\mathfrak{F}} D(f_M)/f_M .
$$

さて、提案 9 は (22) の極限に続きます。

### 7. 形式的な方程式の解冪系列環

#### 補題 2 {#alg-iv-s4-lem-2 .statement tag=06CE}

*$(g_i)_i$ *位数* $\geq 2$ *in* $\mathbf{A}[[\mathbf{I}]]$ の元の家族としましょう。 *$\mathbf{I}$ *が無限である場合、* $g_i$ * $\mathbf{I}$ の有限部分集合の補数のフィルターに沿って 0 になる傾向があると仮定します。 *トポロジカル* A*-代数* $\mathbf{A}[[\mathbf{I}]]$ * $T(X_i) = X_i + g_i$ *すべてに対して* $i \in \mathbf{I}$ の * 自己同型* T * が 1 つだけ存在します。 ※さらに、

(23)
$$
\omega(T(u) - u) \geq \omega(u) + 1
$$
*それぞれ* $u \in \mathbf{A}[[\mathbf{I}]]$。

系列 $f_i = X_i + g_i$ には定数項がなく、$\mathbf{I}$ が無限大の場合、$f_i$ は $\mathbf{I}$ の有限部分集合の補数のフィルターに沿って 0 になる傾向があります。したがって (IV、p. 28、提案 4) A-代数 $\mathbf{A}[[\mathbf{I}]]$ の連続する自己準同型 T が正確に 1 つ存在し、すべての $i \in \mathbf{I}$ に対して $T(X_i) = f_i$ になります。それぞれの $\nu \in \mathbf{N}'$ に、

$$
v_\nu = T(X^\nu) - X^\nu = \prod_{i \in \mathbf{I}} (X_i + g_i)^{\nu(i)} - \prod_{i \in \mathbf{I}} X_i^{\nu(i)} ;
$$

関係 $\omega(g_i) \geq 2$ は $w(v_\nu) \geq |\nu| + 1$ を暗示し、これから関係 (23) がすぐに続きます。

$T$ が *単射* であることを示しましょう。 $T(u) = 0$ のような $u \in \mathbf{A}[[\mathbf{I}]]$ が与えられると、(23) によって $w(u) \geq w(u) + 1$ が得られますが、$u \neq 0$ の場合、$w(u)$ は正の整数になるため、これは不可能です。

$\mathbf{A}[[\mathbf{I}]]$ のすべての形式的な系列 $v$ について、次数 $n$ の同次の成分を $H_n(v)$ で表します。連続式写像 $S, : \mathbf{A}[[\mathbf{I}]] \to \mathbf{A}[[\mathbf{I}]]$ を漸化式で $S_0(v) = H_0(v)$ と定義するを入れてみましょう

(24)
$$
S_n(v) = H_n \left( v - T \left( \sum_{k=0}^{n-1} S_k(v) \right) \right) \quad \text{for} \quad n \geq 1
$$

Put $S(v) = \sum_{n \geq 0} S_n(v)$; if $\nu \in \mathbf{N}^{(\mathbf{I})}$ and $n = |\nu|$, then the coefficient $S^\nu(v)$ of $X^\nu$ in $S(v)$ is equal to that of $X^\nu$ in $S,(\nu)$; since $S,$ is a continuous mapping, the mapping $S^\nu : \mathbf{A}[[\mathbf{I}]] \to \mathbf{A}$ is continuous. したがって、$\mathbf{A}[[\mathbf{I}]] = \mathbf{A}^{\mathbf{N}^{(\mathbf{I})}}$ の積位相の定義により、写像 $S : \mathbf{A}[[\mathbf{I}]] \to \mathbf{A}[[\mathbf{I}]]$ は連続です。

すべての $v \in \mathbf{A}[[\mathbf{I}]]$ について関係 $T(S(v)) = v$ を証明し、補題の証明を完成させます。 $v \in \mathbf{A}[[\mathbf{I}]]$、$u_n = S_n(v)$、$u = S(v)$ とします。 $n$ を正の整数とすると、

(25)$_n$
$$
\omega(v - T(u)) \geq n .
$$

$w(u - (u_0 + \ldots + u_{n-1})) \geq n$、よってがあります

$$
\omega(T(u) - T(u_0 + \ldots + u_{n-1}) - u_n) \geq n + 1
$$

(23)による。さて、漸化式 (24) は次のことを示しています。

$$
u_n = H_n(v - T(u_0 + \cdots + u_{n-1}))
$$

(26) により、形式的な冪系列 $v - T(u)$ と $v - T(u_0 + \ldots + u_{n-1}) - u_n$ は、次数 $n$ の同じ同次成分を持ち、この成分は、(27) により零になります。したがって、$w(v - T(u)) \geq n + 1$ が得られます。つまり、$(25)_n$ は $(25)_{n+1}$ を意味します。 $(25)_0$ が明らかに成り立つので、証明されるように、すべての整数 $n \geq 0$、よって $v = T(u) = T(S(v))$ に対して $\omega(v - T(u)) \geq n$ が得られます。

この番号の残りの部分については、任意の集合 $I$ について、家族 $(f_i)_{i \in I}$ 満たすの $A\{I\}$ 集合によって次の条件を表すものとします。
(i) 各 $i \in I$、$f_i$ は、定数項を除いた $A[[I]]$ の元です。
(ii) $I$ が無限である場合、$f_i$ は $I$ の有限部分集合の補数のフィルターに沿って 0 になる傾向があります。

集合 $A\{I\}$ は、合成法則 $(f, g) \mapsto f \circ g$ のモノイドであり、$\{X_i\}_{i \in I}$ は単位元となります。したがって、$A\{I\}$の可逆元の集合は群となります。

一方、$E$ を、定数項不変条件のないすべての形式冪系列のイデアルを残したまま、$A$-代数 $A[[I]]$ のすべての連続ユニタル自己準同型のモノイドとする。 $f \in A\{I\}$ と $g \in A[[I]]$ の場合、元 $g(f)$ が定義されます。固定$f$、$A[[I]]$の$g \mapsto g(f)$を写像、$E$の元$W_f$とします。 $f_1, f_2 \in A\{I\}$ と $g \in A[[I]]$ の場合、公式 (5) (IV, p. 30) までに

$$
W_{f_1 \circ f_2}(g) = g(f_1 \circ f_2) = g(f_1) \circ f_2 = W_{f_2}(W_{f_1}(g))
$$

したがって、$f \mapsto W_f$ は、$A\{I\}$ から $E$ への反対のモノイドの準同型です。提案 4 (IV, p. 28) により、この準同型は全単射です。

$f = (f_i)_{i \in I} \in A\{I\}$ を、$\sum_{j \in I} \alpha_{ij} X_j$ を $f_i$ の次数 1 の同次成分とします。 $I$ の固定 $j$ については、上記の仮定 (ii) による接尾辞 $i$ の有限数を除いて、$\alpha_{ij} = 0$ になります。 $(\lambda_i) \in A^{(I)}$ の場合、$\left( \sum_{j \in I} \alpha_{ij} \lambda_j \right) \in A^{(I)}$ になります。

$A$-線形マッピング $^1$ を $T_f$ で表します

$$
(\lambda_i) \mapsto \left( \sum_{j \in I} \alpha_{ij} \lambda_j \right)
$$

$A^{(I)}$ から $A^{(I)}$ に。 $g \in A\{I\}$ の場合、次のことが簡単に検証されます。

$$
T_{f \circ g} = T_f \circ T_g .
$$

$^1$ ときどき $T_f$ は、$f$ に接する線形写像と呼ばれます。

#### 命題 10 {#alg-iv-s4-prop-10 .statement tag=06CF}

— $f \in A\{I\}$ としましょう。その場合、次の条件は同等です。
(i) $f$ は法則 $\circ$ の $A\{I\}$ で反転可能です。
(ii) $T_f$ は環 $\mathrm{End}(A^{(I)})$ で反転可能です。

(i) $\Rightarrow$ (ii) の含意は (28) から明らかです。ここで、$T_f$ が $\mathrm{End}(A^{(I)})$ で反転可能であるとします。それぞれの $g_i$ が次数 $l$ と同質であり、$T_g \circ T_f$ が $A^{(I)}$ の恒等写像であるような $g = (g_i)_i \in A\{I\}$ が存在します。 $h = g \circ f$と書きます。次に (28) は、$T_h$ が $A^{(I)}$ の恒等写像であり、主張 $\omega(h_i - X_i) \geq 2$ と同等であることを示します。したがって、IV の補題 2 により、p. 35 $h$ は $A\{I\}$ で反転可能です。 $g$ は $A\{I\}$ で可逆であるため、$f$ は $A\{I\}$ で可逆であることは明らかです。

#### 系 {#alg-iv-s4-n7-cor-1 .statement tag=06CG}

— $f_i(Y_1, Y_2, \ldots, Y_q, X_1, X_2, \ldots, X_p)$ ($1 \leq i \leq q$) を、$A[[Y_1, \ldots, Y_q, X_1, \ldots, X_p]]$ の定数項を持たずに、$q$ 正式な冪系列とします。形式的冪系列 $D = \det \left( \frac{\partial f_i}{\partial Y_j} \right)$ の定数項が $A$ で可逆である場合、次のような $q$ 形式冪系列 $u_1(X_1, \ldots, X_p), \ldots, u_q(X_1, \ldots, X_p)$ の系が正確に 1 つ存在します。
$$
f_i(u_1, \ldots, u_q, X_1, \ldots, X_p) = 0 \quad (1 \leq i \leq q).
$$
$f_{q+1} = X_1, \ldots, f_{q+p} = X_p$, $f = (f_1, \ldots, f_{p+q})$ とすると、$\det T_f$ は $D$ の定数項に等しいため、$A$ で反転可能です。したがって、$T_f$ は反転可能です。提案 10 により、定数項のない形式的な冪系列が存在します。
$$
g_1, \ldots, g_{q+p} \in A[[Y_1, \ldots, Y_q, X_1, \ldots, X_p]]
$$
書くときのような
$$
g = (g_1, \ldots, g_{p+q}), \quad 1_{p+q} = (Y_1, \ldots, Y_q, X_1, \ldots, X_p)
$$
$f \circ g = g \circ f = 1_{p+q}$ があります。 関係 $f \circ g = 1_{p+q}$、特に
$$
g_{q+1} = X_1, \ldots, g_{q+p} = X_p.
$$
したがって、
$$
f_i(g_1, \ldots, g_q, X_1, \ldots, X_p) = Y_i \quad (1 \leq i \leq q).
$$
今入れてください
$$
u_i(X_1, \ldots, X_p) = g_i(0, \ldots, 0, X_1, \ldots, X_p) \quad (1 \leq i \leq q);
$$
(30) の各 $Y_i$ に 0 を代入すると、目的の関係 (29) が得られます。

逆に、環 $A[[X_1, \ldots, X_p]]$ 満たす関係 (29) の形式的冪系列 $u_1, \ldots, u_q$ を仮定します。 関係 $g \circ f = 1_{p+q}$ が意味するもの
$$
g_i(f_1, \ldots, f_q, X_1, \ldots, X_p) = Y_i \quad (1 \leq i \leq q);
$$
(32) の $1 \leq i \leq q$ の $Y_i$ を $u_i$ に置き換えると、(31)、解の系のよって一意性 (29) が得られます。

### 8. 正式冪系列整域

#### 命題 11 {#alg-iv-s4-prop-11 .statement tag=06CH}

— $A$ が整域であると仮定します。

(i) *環* $A[[I]]$ *また整域* です。

(ii) ** $u, v$ * が* $A[[I]]$ の非ゼロ元である場合、*その後* $\omega(uv) = \omega(u) + \omega(v)$。

For each $J \subset I$ let $\varphi_J$ be the homomorphism of $A[[I]]$ into $A[[J]]$ obtained by substituting in each element of $A[[I]]$, $X_i$ for $X_i$ when $i \in J$ and 0 for $X_i$ when $i \in I - J$. $u, v$ を $A[[I]]$、$p = \omega(u)$、$q = \omega(v)$ の非ゼロ元とします。次のような有限部分集合 $J$ または $I$ が存在します。

$$
\varphi_J(u) \neq 0,\ \varphi_J(v) \neq 0,\ \omega(\varphi_J(u)) = p,\ \omega(\varphi_J(v)) = q.
$$

a (それぞれ b) を次数 $p$ (それぞれ $q$) の $\varphi_J(u)$ (それぞれ $\varphi_J(v)$) の同次成分とする。 $J$ は有限なので、a と b は多項式です。 $a \neq 0, b \neq 0$ があるため、$ab \neq 0$ (IV、p. 9、提案 8)。したがって、$\varphi_J(u)\ \varphi_J(v)$ は位数 $p + q$ の非ゼロです。したがって、$uv \neq 0$ と $\omega(uv) \leq p + q$ が続きます。しかし明らかに$\omega(uv) \geq p - q$。

### 9. 体にわたって体の分数の環の正式な冪系列が不定になります

K が可換体の場合、$K((X))$ 体の分数または整域 $K[[X]]$ で表します。

#### 命題 12 {#alg-iv-s4-prop-12 .statement tag=06CI}

— *ゼロ以外のすべての元* $u$ *of* $K((X))$ *は、* $u = X^k v$ のように独自の方法で書くことができます。*ここで* $k \in \mathbf{Z}$ *and* $v$ * は、* $X$ *of 位数* の形式的な冪系列です0.

$u = w/t$ とします。ここで、$w, t$ は $K[[X]]$ の非ゼロ元です。 $w = X^r w_1, t = X^s t_1$ があります。ここで、$r, s \in \mathbf{N}$ と $w_1, t_1$ は、位数 0 の正式な冪系列であるため、$K[[X]]$ で反転可能です (IV、p. 30、提案 6)。すると、$u = X^{r-s} w_1 t_1^{-1}$ と $w_1 t_1^{-1}$ は、位数 0 の正式な冪系列になります。

一意性を証明しましょう。 $u = X^{k_1} v_1 = X^{k_2} v_2$ ここで、$k_1, k_2 \in \mathbf{Z}$ と $v_1, v_2$ は、位数 0 の形式的な冪系列であるとします。 $X^{k_1 - k_2} = v_2 v_1^{-1}$ は、位数 0 の形式的な冪系列であるため、$k_1 = k_2$ が得られます。 よって $v_1 = v_2$ そしてこれは一意性主張を証明します。

We shall say that the elements of $K((X))$ are *generalized formal power series* in $X$ with coefficients in $K$, or simply formal power series when no confusion can arise (the elements of $K[[X]]$ are then called *formal power series with positive exponents*); if $u \neq 0$, the integer $k$ defined in Prop. 12 is also called the *order* of $u$ and is written $\omega(u)$, even if it is $< 0$; we also put $\omega(0) = \infty$. すぐに確認できるのは、

$$
\begin{align*}
\omega(u + v) &\geq \inf(\omega(u), \omega(v)) \\
\omega(u + v) &= \inf(\omega(u), \omega(v)) \quad \text{if}\ \ \omega(u) \neq \omega(v) \\
\omega(uv) &= \omega(u) + \omega(v)
\end{align*}
$$

一般化された形式的な冪系列にはまだ当てはまります。特に、$u \neq 0$ の場合は、$w(u^{-1}) = -w(u)$ になります。 \* 他の語 (共同アルゴリズム、VI, § 3, No. 6、p. 392、定義 3) では、w は体 $K((X))$ の正規化された離散評価です。 \*

それぞれの整数 $n \in \mathbf{Z}$ について、$p_n$ をすべての $u \in K((X))$ の集合とし、$\omega(u) \geq n$ とします。すると (p.)、 、 は加法群 $K((X))$ の部分群のうち減少列であり、 共通部分 0 です。したがって、翻訳下で不変である $K((X))$ には位相が存在し、その $(p_n)_{n \in \mathbf{Z}}$ は 0 の近傍の基本的な系 (Gen. Top.、III、p. 223) です。 $K((X))$ がトポロジー 体 (Gen. Top.、III、p. 281) であり、$K[[X]]$ が $K((X))$ の開いたおよび閉じた部分空間であることを簡単に検証できます。

$(\alpha_n)_{n \in \mathbf{Z}}$ を $K$ の元の族とし、すべての $n < N$ に対して $a_n = 0$ となるような整数 N が存在すると仮定します。すると、家族の $(\alpha_n X^n)_{n \in \mathbf{Z}}$ は $K((X))$ (Gen. Top., III, p. 263, Cor.) で要約可能です。すべての $n$ に対して $a_n = 0$ の場合に限り、$u = \sum_{n \in \mathbf{Z}} \alpha_n X^n$ を入れ、次に $u = 0$ を入れます。それ以外の場合、$u$ の位数は、$\alpha_k \neq 0$ となる最小の整数 k です。最後に、$K((X))$ のすべての元は、形 $\sum_{n \in \mathbf{Z}} \alpha_n X^n$ で独自の方法で書くことができます。ここで、数列 $(\alpha_n)$ は、すべての十分大きい n について $\alpha_{-n} = 0$ を満たします。

環 $K[X]$ は $K[[X]]$ の部分環であるため、すべての有理分数 $u/v \in K(X)$ (u、v は X の多項式) は、$K((X))$ の (一般化された) 形式的な冪系列 $uv^{-1}$ と同一視できます。原点での展開。したがって、体 $K(X)$ は $K((X))$ の部分体と同一視されます。

### 10. 指数関数と対数

指数関数冪系列によって、$Q[[X]]$ の元 $\sum_{n \geq 0} \frac{X^n}{n!}$ がわかります。それは exp X または $e^X$ で表されます。

#### 命題 13 {#alg-iv-s4-prop-13 .statement tag=06CJ}

— $Q[[X, Y]]$ には $e^{X+Y} = e^X e^Y$ があります。

二項式公式の場合、

$$
\frac{(X+Y)^n}{n!} = \sum_{i+j=n} \frac{X^i}{i!} \frac{Y^j}{j!}
$$

したがって、

$$
e^X e^Y = \left( \sum_{i \geq 0} \frac{X^i}{i!} \right) \left( \sum_{j \geq 0} \frac{Y^j}{j!} \right) = \sum_{i,j \geq 0} \frac{X^i}{i!} \frac{Y^j}{j!} = \sum_{n \geq 0} \sum_{i+j=n} \frac{X^i}{i!} \frac{Y^j}{j!}
$$
$$
= \sum_{n \geq 0} \frac{(X+Y)^n}{n!} = e^{X+Y}.
$$

$Q[[X]]$ の定義する 2 元 $e(X)$、I(X)

$$
e(X) = e^X - 1 = \sum_{n \geq 1} \frac{X^n}{n!}
$$

(34)
$$
l(X) = \sum_{n \geq 1} (-1)^{n-1} \frac{X^n}{n}.
$$

私たちは持っています
(35)
$$
e(X+Y) = e(X) + e(Y) + e(X)e(Y)
$$
(36)
$$
D(e^X) = D(e(X)) = e^X
$$
(37)
$$
D(l(X)) = \sum_{n \geq 0} (-X)^n = (1+X)^{-1}.
$$

#### 命題 14 {#alg-iv-s4-prop-14 .statement tag=06CK}

— $l(e(X)) = e(l(X)) = X$ があります。

系列 l と e には定数項がなく、次数 1 の項は X に等しい。 IV, p. 37 の提案 10 により、公式 $l(e(X)) = X$ を証明するのに十分です。式（３６）および（３７）とＣｏｒ． IV、p. 33 の 3 つがあります

$$
D(l(e(X))) = (1 + e(X))^{-1} D(e(X)) = (e^X)^{-1} e^X = 1
$$

よって $I(e(X)) = X$。

K を Q 代数とし、定数項形を持たない K[[I]] の元は、加法の下で可換群 $\mathscr{E}$ となります。定数項 1 形をもつ K[[I]] の元は、乗法 (IV, p. 30) の下の可換群 $\mathbf{A}$ です。それぞれの $f \in \mathscr{E}$ について、$\mathscr{E}$ の定義する元 $e \circ f$ と $I \circ f$ ができ、上記の提案 14 により、写像 $f \mapsto l \circ f$ と $f \mapsto e \circ f$ は相互に逆数置換になります。 $\mathscr{E}$;明らかにそれらは連続的です。 $\exp X = e(X) + 1$ 以降、指数関数写像 $f \mapsto \exp f = e \circ f + 1$ は $\mathscr{E}$ から $\mathscr{M}$ への連続全単射であることがわかります。 IV、p. 29、提案 13 の公式 (4) により、$f, g \in \mathscr{E}$ に対して $\exp(f+g) = (\exp f)(\exp g)$ が得られます。したがって、指数関数はトポロジカル群 $\mathscr{E}$ のトポロジカル群 $\mathbf{A}$ への同型です。

$\mathscr{M}$ の $\mathscr{E}$ に対する逆同型は対数と呼ばれ、$g \mapsto \log g$ と書きます。したがって、$\mathscr{M}$ の $g$ には $\log g = l(g-1)$ があり、特に、

(38)
$$
\log(1+X) = l(X).
$$

対数は $\mathscr{M}$ の $\mathscr{E}$ への準同型であるため、公式 $(1+X)(1+Y) = 1 + (X+Y+XY)$ は、

(39)
$$
l(X) + l(Y) = l(X+Y+XY).
$$

$(u_\lambda)_{\lambda \in L}$ を $\mathscr{B}$ の元の加算可能な族とすると、族 $(\exp u_{\lambda})_{\lambda \in L}$ は乗算可能であり、次のようになります。

(40)
$$
\exp \left( \sum_{\lambda \in L} u_{\lambda} \right) = \prod_{\lambda \in L} \exp u_{\lambda}.
$$

同様に、$(f_\lambda)_{\lambda \in L}$ が A の元の乗算可能な族である場合、族 $(\log f_\lambda)_{\lambda \in L}$ は合計可能であり、次のようになります。

(41)
$$
\log \left( \prod_{\lambda \in L} f_\lambda \right) = \sum_{\lambda \in L} \log f_\lambda .
$$

$g \in A$ とし、D を $K[[I]]$ の連続する導分とします。 $\log g = l(g - 1)$ があるため、Cor によって作成されます。 IV、p. 33、および (37) のうちの 3 つがあります

(42)
$$
D \log g = D(g)/g .
$$

式 $D(g)/g$ は、(D に対する) g の対数導関数と呼ばれます。

### 練習問題 {#alg-iv-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
