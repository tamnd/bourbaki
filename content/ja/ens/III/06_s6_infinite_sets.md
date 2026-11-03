---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 6
section_title: Infinite sets
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 183-190, 241-251
pdf_pages: 0189-0196, 0247-0257
extraction: ocr
subsections:
    - "no": 1
      title: THE SET OF NATURAL INTEGERS
      page: 183
      pdf_page: 189
    - "no": 2
      title: DEFINITION OF MAPPINGS BY INDUCTION
      page: 184
      pdf_page: 190
    - "no": 3
      title: PROPERTIES OF INFINITE CARDINALS
      page: 186
      pdf_page: 192
    - "no": 4
      title: COUNTABLE SETS
      page: 188
      pdf_page: 194
    - "no": 5
      title: STATIONARY SEQUENCES
      page: 189
      pdf_page: 195
statements: 26
exercises: 32
content_sha256: 990116c3cc5d8733424b8036f57f87119af0c201442041de31f66e362490604f
translated_from: content/en/ens/III/06_s6_infinite_sets.md
translation_method: google
source_content_sha256: 567e0c5f3b6c1ecb2bc3cd823e4e97976fc38f1c07ab89e7b0f38f5f38c28c46
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: d94c2836fa8833b96b7c70ae0ceb8bc06c0fb504a5a4fd91c585944069a25ba9
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 6. 無限集合

### 1. ナチュラルの集合整数

#### 定義 1 {#ens-iii-s6-def-1 .statement tag=03MV}

*集合は有限でない場合は無限であると言われます。*

特に基数は整数でなければ無限大です。

関係「無限の集合が存在する」ということは、関係「$x$は整数である」が *集合化* (章 II, § 1, no. 4) であることを意味します。なぜなら、$\mathfrak{a}$ が無限の基数で、$n$ が任意の整数である場合、できないは $\mathfrak{a} \leqslant n$ (§ 4, no. 2, 命題 2) になります。したがって、すべての整数 $n$ に対して $n < \mathfrak{a}$ が得られます。これは、整数 $< \mathfrak{a}$ の集合 (§ 3, no. 2、定理 1 に続く注意) 含むがすべて整数であることを示しています。逆に、関係「$x$は整数」が集団化している場合、整数の集合Eは*無限*の集合になります。それぞれの整数 $n$、区間 $[0, n]$ は、E の $n + 1$ 元の部分集合 (§ 5, no. 3、命題 5) です。したがって、カード(E)$\geqslant n + 1 > n$。しかし、カード(E) $\neq n$ が整数 $n$ ごとにあるということは、E が無限であることを意味します。

¶ 次の公理を導入します。

A5 (「無限の公理」。) *無限の集合が存在します。*

この公理が以前に紹介した公理や公理スキームから演繹できるかどうかは不明です。この問題は最終的には解決されていませんが、この公理は他の公理から独立していると推定されます。

前述の注意は次の定理を証明します。

#### 定理 1 {#ens-iii-s6-thm-1 .statement tag=03MW}

*関係「$x$は整数」は集団化しています。*

整数の $\mathbf{N}$ 集合で表します (曖昧さを避けるために必要な場合は、「自然な整数の集合」とも呼ばれます)。 $\mathbf{N}$の基数は$\aleph_0$で表されます。 $\mathbf{N}$ が順序付き集合とみなされる場合、常に § 3, no. 2 で定義された順序 (*通常* 順序と呼ばれる) が考慮され、〜でない限りその逆が明示的に述べられます。

#### 定義 2 {#ens-iii-s6-def-2 .statement tag=03MX}

*数列* (それぞれ集合* E の元の *数列) * は家族* (それぞれ * E の元の家族) *その添字集合は * $\mathbf{N}$ の部分集合です。 *数列は、その添字集合が * $\mathbf{N}$ の無限の部分集合である場合、無限であると言われます。

$\mathrm{P}\{n\}$ を関係とし、I が整数 $n$ の集合を表し、$\mathrm{P}\{n\}$ が true であるとします。 I は $\mathbf{N}$ の部分集合になります。 数列 $(x_n)_{n\in\mathrm{I}}$ は、ときどき $(x_n)_{\mathrm{P}\{n\}}$ と書き込まれ、$x_n$ は数列の *n 番目の項* と呼ばれます。 添字集合が整数 $n \geqslant k$ の集合である数列は、$(x_n)_{k \leqslant n}$ または $(x_n)_{n \geqslant k}$、あるいは $k = 0$ または $k = 1$ の場合は単に $(x_n)$ と書かれることがよくあります。 たとえば、同じ条件下で、表記 $\prod_{\mathrm{P}\{n\}} \mathrm{X}_n$ と $\prod_{n=k}^{\infty} \mathrm{X}_n$ は一連の集合 $(\mathrm{X}_n)_{n\in\mathrm{I}}$ の積を表すために使用され、和集合、積、基数和にも同様の表記があります。

数列のすべてのサブファミリーは数列であり、指定された数列の *サブシーケンス* と呼ばれます。

同じ添字集合を持つ 2 つの数列 $(x_n)_{n\in\mathrm{I}}$、$(y_n)_{n\in\mathrm{I}}$ は、添字集合の置換 $f$ が存在する場合、*それらの項の順序のみが異なると言われます* I は、すべての $n \in \mathrm{I}$ に対して $x_{f(n)} = y_n$ となるようにします。

*倍数数列* は、添字集合が積 $\mathbf{N}^p$ の部分集合 ($p$ 整数) ($p = 2$ の場合は「ダブル数列」、「トリプル」) である家族です。 $p = 3$ の場合は「数列」など)。

I を $\mathbf{N}$ と等価な集合とし、$f$ を I に対する $\mathbf{N}$ の全単射とします。 集合 I によってインデックス付けされた各ファミリー $(x_\iota)_{\iota\in\mathrm{I}}$ について、数列 $n \to x_{f(n)}$ は、$f$ によって定義される * 順序の *ファミリー* $(x_\iota)_{\iota\in\mathrm{I}}$ を整理することによって得られると言われます。 このように、$\mathbf{N}$ から I への 2 つの異なる全単射に対応するシーケンスは、項の順序が異なるだけです。 $n$ 元の集合 I によってインデックス付けされた有限ファミリの場合、次のように定義される順序にファミリを配置することで、$[1, n]$ または $[0, n-1]$ を添字集合として、同様に定義する有限列を作成できます。 区間のいずれか全単射を I に移動します。

### 2. 定義/写像 by 帰納法

集合 $\mathbf{N}$ は整然としているため、基準 C60 (§ 2, no. 2) を適用できます。これは次の形 (同じ記法) をとります。

C62。 *$u$ を文字とし、* $\mathrm{T}\{u\}$ *を項とします。次に、集合* U * と写像 $f$ of* $\mathbf{N}$ *onto* U が存在します *それぞれの整数 $n$ に対して* $f(n) = \mathrm{T}\{f^{(n)}\}$ が得られます。 *ここで、$f^{(n)}$ は * $[0, n[$ の写像を表します*onto* $f([0, n[)$ *これは $f$ on* $[0, n[$ と一致します。 *また、集合* U * と写像 $f$ は、この条件* によって一意に決まります。

これから次の基準を導き出します。

C63。 *$S\{v\}$ *と* $a$ *を 2 つの項とします。次に、集合* $V$ *と写像* $f$ *の* $\mathbf{N}$ *上に* $V$ *そのような* $f(0) = a$ *と* $f(n) = S\{f(n-1)\}$ *それぞれの整数* $n \geqslant 1$が存在します。 *また、集合* $V$ * と写像* $f$ * これらの条件により一意に決まります。

C62 [^1] から C63 を推定するには、次のようにします。

$$D(u) = \mathscr{E}_x(x \in \mathbf{N} \ \text{and} \ (\exists y)((x, y) \in \mathrm{pr}_1(\mathrm{pr}_1(u))))$$

各文字 $u$ ごとに。 $u$ が $\mathbf{N}$ の部分集合の集合の写像である場合、$D(u)$ はちょうど $u$ の領域 (章 II, § 3, no. 1) です。 $M(u)$ を $\mathbf{N}$ [^2] の $D(u)$ の最小値上界とします。 $\varphi$ を空の写像とし、$\emptyset$ をソースとターゲット、つまり (章 II, § 3、番号 1 と 4)、トリプル $(\emptyset, \emptyset, \emptyset))$ として、関係を検討します。

$$(u = \varphi \ \text{and} \ y = a) \ \text{or} \ (u \neq \varphi \ \text{and} \ y = S\{u(M(u))\})$$

これを $R\{y, u\}$ で表します。最後に、$T\{u\}$ を項 $\tau_y(R\{y, u\})$ とします。 C62を項$T\{u\}$に適用します。 $f^{(0)}$ は $\varphi$ に等しいので、$T\{f^{(0)}\} = a$ になります。したがって $f(0) = a$ です。一方、$n > 0$ の場合、$D(f^{(n)}) = [0, n-1]$ と $M(f^{(n)}) = n-1$、よって

$$T\{f^{(n)}\} = S\{f^{(n)}(n-1)\} = S\{f(n-1)\}.$$

*例*

#### 例 1 {#ens-iii-s6-n2-exa-1 .statement tag=03TC}

$a$ が集合 $E$ の元で、$S\{u\}$ が項 $g(u)$ であり、$g$ が $E$ の写像をそれ自体 [^3] にすると仮定します。次に、$n$ の帰納法によって、すべての $n \in \mathbf{N}$ に対して $f(n) \in E$ があることがすぐにわかります。従って、$f$ は、$\mathbf{N}$ の写像から $E$ となり、すべての整数 $n$ に対して $f(0) = a$ と $f(n+1) = g(f(n))$ になります。

同様に、$h$ を $E$ の $\mathbf{N} \times E$ の写像とし、$\psi$ を $\psi(n, x) = (n+1, h(n, x))$ で定義される$\mathbf{N} \times E$ の写像とします。 前述の議論により、すべての $n$ に対して $g(0) = (0, a)$ と $g(n+1) = \psi(g(n))$ となるような、$\mathbf{N}$ から $\mathbf{N} \times E$ への一意のマッピング $g = (\theta, f)$ が存在します。そこから、それぞれ $f(0) = a$ と $f(n + 1) = h(n, f(n))$ となるような、$\mathbf{N}$ から E へのマッピング $f$ の存在と一意性がわかります。整数 $n$。

#### 例 2 {#ens-iii-s6-n2-exa-2 .statement tag=03TD}

X を集合とし、E を X の写像の集合とします。 $e$ が X の恒等写像を表すものとし、$f$ を E の任意の元とする。$S\{u\}$ を項 $f \circ u$ [^4] とする。 適用 C63 によって、$f^0 = e$ と $f^{n+1} = f \circ f^n$ のように、$n \to f^n$ で示される E に $\mathbf{N}$ の一意な写像が存在することがわかります。 写像 $f^n$ は、写像 $f$ の *n 回目の反復* と呼ばれます。

#### 例 3 {#ens-iii-s6-n2-exa-3 .statement tag=03TE}

$S\{u\}$ を項 $\mathfrak{P}(u)$、$a$ を集合 E とすると、同様に、$\mathbf{N}$ の集合 V(E) には、$n \to \mathfrak{P}^n(\mathrm{E})$ で示される写像が存在することがわかります。 整数 $n$ ごとに $\mathfrak{P}^0(\mathrm{E}) = \mathrm{E}$、$\mathfrak{P}^1(\mathrm{E}) = \mathfrak{P}(\mathrm{E})$、$\mathfrak{P}^{n+1}(\mathrm{E}) = \mathfrak{P}(\mathfrak{P}^n(\mathrm{E}))$。

#### 注意 {#ens-iii-s6-n2-rem-1 .statement tag=03MY}

Eを集合、AをEの部分集合、$g$をAの写像をEに、$a$をAの元とします。$S\{u\}$を項$g(u)$とします。基準 C63 が適用され、整数 $n$ ごとに $f(0) = a$ と $f(n + 1) = g(f(n))$ が存在するように、集合 V 上に $\mathbf{N}$ の写像 $f$ が存在することが証明されます。 $\mathrm{V} \subset \mathrm{A}$; ということが起こるかもしれません。そうでない場合は、$p$ を最大の整数とし、$f([0, p]) \subset \mathrm{A}$ とします。次に$f(p + 1) = g(p) \notin \mathrm{A}$、そして$g(g(p))$は項ですが、これについては何とも言えません。したがって、この場合、$f$ は区間 $[0, p + 1]$ (「制限付き帰納法」) でのみ定義されているとみなされます。

### 3. 無限の性質基数

#### 定理 2 {#ens-iii-s6-thm-2 .statement tag=03MZ}

*無限の基数 $\mathfrak{a}$ ごとに、$\mathfrak{a}^2 = \mathfrak{a}$ があります。*

次の 2 つの補題を使用します。

#### 補題 1 {#ens-iii-s6-lem-1 .statement tag=03N0}

*すべての無限集合 E 含む集合は $\mathbf{N}$ と等価です。*

E (§ 2, no. 3, 定理 1) には整った順序の関係が存在します。これを $x \leqslant y$ で表します。 仮定は、整列した集合 E できないが $\mathbf{N}$ とは異なる $\mathbf{N}$ のセグメントと同型であることを意味します。そのようなセグメントは形 $[0, n]$ (§ 2, no. 1, 命題 1) であり、したがって有限です。したがって、$\mathbf{N}$ は E のセグメント (§ 2, no. 3, 定理 3) と同型であり、結果はよってになります。

#### 補題 2 {#ens-iii-s6-lem-2 .statement tag=03N1}

*集合 $\mathbf{N} \times \mathbf{N}$ は $\mathbf{N}$ と同等です。*

$\mathbf{N} \times \mathbf{N}$ 含む集合 $\{0\} \times \mathbf{N}$ は $\mathbf{N}$ と等価なので、$\mathrm{Card}(\mathbf{N}) \leqslant \mathrm{Card}(\mathbf{N} \times \mathbf{N})$ になります。 証明を完了するには、$\mathbf{N} \times \mathbf{N}$ の定義する単射 $f$ を $\mathbf{N}$ に加えるだけで十分です。 この目的のために、$\mathbf{N}$ から $\mathrm{I} = \{0, 1\}$ へのマッピングのセットへの $\mathbf{N}$ の注入 $\varphi$ が存在することに注意します。これは次のように取得されます: $r$ が $n > 2^r$ のような最小の整数である場合、および $\sum_{k=0}^{r-1} \varepsilon_k 2^{r-k-1}$ が $n$ の二項展開である場合(§ 5, no. 7)、$\varphi(n)$ は、$m < r$ の場合は $u_m = \varepsilon_{r-m-1}$、$m \geqslant r$ の場合は $u_m = 0$ となるように、シーケンス $(u_m)_{m \in \mathbf{N}}$ として定義されます。 § 5, no. 7 の命題 8 は、$\varphi$ が単射であることを示しています。 それぞれの対 $(n, n') \in \mathbf{N} \times \mathbf{N}$ について、次のように定義する $f(n, n')$ を計算します。 $\varphi(n) = (u_m)$ と $\varphi(n') = (v_m)$ の場合、$f(n, \; n')$ を整数 $s$ とし、$\varphi(s) = w_m$ とします。ここで、$w_{2m} = u_m$ と $w_{2m+1} = v_m$ はすべて$m \in \mathbf{N}$。 関係 $f(n, \; n') = f(n_1, \; n_1')$ が $\varphi(n) = \varphi(n_1)$ と $\varphi(n') = \varphi(n_1')$ を暗示していることは明らかです。したがって $(n, n') = (n_1, n_1')$ 、したがって $f$ は単射法です。

¶ 定理の証明になります。 2. E を $\mathrm{Card}(\mathrm{E}) = \mathfrak{a}$ となるように集合とします。 D を $\mathbf{N}$ (補題 1) と等しい E の部分集合とします。次に、$\mathrm{D} \times \mathrm{D}$ (補題 2) 上に D の全単射 $\psi_0$ が存在します。 $\mathfrak{M}$ を対 $(\mathrm{X}, \psi)$ の集合とします。ここで、X は E 含む D の部分集合で、$\psi$ は $\mathrm{X} \times \mathrm{X}$ 上の X の全単射です。 拡大する $\psi_0$。 順序集合 $\mathfrak{M}$ 関係による

$$\text{``} \mathrm{X} \subset \mathrm{X}' \text{ and } \psi' \text{ is an extension of } \psi \text{''}$$

$(\mathrm{X}, \psi)$ と $(\mathrm{X}', \psi')$ の間。すると、$\mathfrak{M}$ が *帰納的* (cf. § 2, no. 4, 例 2) であることがすぐにわかります。したがって、Zorn の補題 (§ 2, no. 4, 定理 2) により、$\mathfrak{M}$ は極大元 $(\mathrm{F}, f)$ になります。 定理を証明するには十分な $\mathrm{Card}\,(\mathrm{F}) = \mathfrak{a}$ を示します。 $\mathrm{Card}\,(\mathrm{F})$ が $\mathfrak{a}$ に等しくない場合は、$\mathrm{Card}\,(\mathrm{F}) = \mathfrak{b} < \mathfrak{a}$ とします。次に、$\mathfrak{b} = \mathfrak{b}^2$ と $\mathfrak{b}$ は無限で、$\mathfrak{b} \leqslant 2\mathfrak{b} \leqslant 3\mathfrak{b} \leqslant \mathfrak{b}^2 = \mathfrak{b}$ (§ 3, no. 6, 命題 14) です。したがって、$2\mathfrak{b} = \mathfrak{b}$ と $3\mathfrak{b} = \mathfrak{b}$ です。 仮定 $\mathfrak{b} < \mathfrak{a}$ から、$\mathrm{Card}\,(\mathrm{E} - \mathrm{F}) > \mathfrak{b}$ になります。そうでない場合は、$\mathrm{Card}\,(\mathrm{E}) \leqslant 2\mathfrak{b} = \mathfrak{b}$ になるはずで、$\mathfrak{b} < \mathrm{Card}\,(\mathrm{E})$ と仮定しました。したがって、F と等価な部分集合 $\mathrm{Y} \subset \mathrm{E} - \mathrm{F}$ が存在します。$\mathrm{Z} = \mathrm{F} \cup \mathrm{Y}$ とします。 $\mathrm{Z} \times \mathrm{Z}$ 上に Z の全単射 $g$ が存在し、拡大する $f$ が存在することを示します。我々は持っています

$$\mathrm{Z} \times \mathrm{Z} = (\mathrm{F} \times \mathrm{F}) \cup (\mathrm{F} \times \mathrm{Y}) \cup (\mathrm{Y} \times \mathrm{F}) \cup (\mathrm{Y} \times \mathrm{Y}),$$

右側の 4 つの積は相互に互いに素です。 F と Y は等価であるため、次のようになります。

$$\mathrm{Card}(\mathrm{F} \times \mathrm{Y}) = \mathrm{Card}(\mathrm{Y} \times \mathrm{F}) = \mathrm{Card}(\mathrm{Y} \times \mathrm{Y}) = \mathfrak{b}^2 = \mathfrak{b},$$

よって

$$\mathrm{Card}((\mathrm{F} \times \mathrm{Y}) \cup (\mathrm{Y} \times \mathrm{F}) \cup (\mathrm{Y} \times \mathrm{Y})) = 3\mathfrak{b} = \mathfrak{b}.$$

したがって、集合には Y の全単射 $f_1$ が存在します。

$$(\mathrm{F} \times \mathrm{Y}) \cup (\mathrm{Y} \times \mathrm{F}) \cup (\mathrm{Y} \times \mathrm{Y});$$

Z の $\times$ Z への写像 $g$ は、F の $f$ と Y の $f_1$ に等しいので、$f$ の定義とは反対に、拡大する $f$ である全単射になります。したがって、$\mathrm{Card}(\mathrm{F}) = \mathfrak{a}$、そして証明が完了します。

#### 系 1 {#ens-iii-s6-thm-2-cor-1 .statement tag=03N2}

*$\mathfrak{a}$ が無限の基数の場合、整数 $n \geqslant 1$ ごとに $\mathfrak{a}^n = \mathfrak{a}$ になります。

$n$ 帰納法までに。

#### 系 2 {#ens-iii-s6-thm-2-cor-2 .statement tag=03N3}

*非ゼロ基数の有限族 $(\mathfrak{a}_i)_{i \in \mathrm{I}}$ (そのうち最大のは無限基数 $\mathfrak{a}$) の積は、$\mathfrak{a}$ に等しい。*

$\mathfrak{b}$ は積を表し、$n$ は I の元の数とします。次に、$\mathfrak{b} \leqslant \mathfrak{a}^n = \mathfrak{a}$ (§ 3, no. 6、命題 14) です。一方、すべての $i \in \mathrm{I}$ に対して $\mathfrak{a}_i \geqslant 1$ なので、$\mathfrak{b} \geqslant \mathfrak{a}$ (§ 3, no. 6、命題 14) になります。

#### 系 3 {#ens-iii-s6-thm-2-cor-3 .statement tag=03N4}

*$\mathfrak{a}$ を無限の基数とし、$(\mathfrak{a}_\iota)_{\iota \in \mathrm{I}}$ を添字集合 I が基数 $\leqslant \mathfrak{a}$ を持つ基数 $\leqslant \mathfrak{a}$ の族とする。次に$\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota \leqslant \mathfrak{a}$;少なくとも 1 つの添字 $\iota \in \mathrm{I}$ に対して $\mathfrak{a}_\iota = \mathfrak{a}$ の場合、$\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota = \mathfrak{a}$。*

$\mathfrak{b}$ を I の基数とします。次に、$\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota \leqslant \mathfrak{a}\mathfrak{b} \leqslant \mathfrak{a}^2 = \mathfrak{a}$ (§ 3, no. 6、命題 14)、およびすべての $\varkappa \in \mathrm{I}$ に対して $\sum\limits_{\iota \in \mathrm{I}} \mathfrak{a}_\iota \geqslant \mathfrak{a}_\varkappa$ が得られます。

#### 系 4 {#ens-iii-s6-thm-2-cor-4 .statement tag=03N5}

*$\mathfrak{a}$ と $\mathfrak{b}$ が 2 つの非ゼロ基数で、そのうちの 1 つが無限である場合、$\mathfrak{a}\mathfrak{b} = \mathfrak{a} + \mathfrak{b} = \sup\,(\mathfrak{a},\,\mathfrak{b})$ になります。*

これは系 2 と系 3 から直接導き出されます。

### 4. 数えられる集合

#### 定義 3 {#ens-iii-s6-def-3 .statement tag=03N6}

*集合は、集合の部分集合、整数の$\mathbf{N}$と等しい場合、可算であると言われています。

#### 命題 1 {#ens-iii-s6-prop-1 .statement tag=03N7}

*数えられる集合のすべての部分集合は数えられます。可算数集合の有限族の積は可算です。可算数集合の数列の和集合は可算です。*

最初の主張は明らかです。他のものは、系から定理 2、no. 3 まで続きます。

¶ $\mathfrak{a}$ が無限の基数である場合、$\mathrm{Card}(\mathbf{N}) \leqslant \mathfrak{a}$ であることを証明しました (no. 3, 補題 1)。これには次の帰結があります。

#### 命題 2 {#ens-iii-s6-prop-2 .statement tag=03N8}

*すべての可算無限集合 E は $\mathbf{N}$ と等価です。*

$\mathrm{Card}(\mathrm{E}) \leqslant \mathrm{Card}(\mathbf{N})$ の場合は定義まで。 E は無限であるため、$\mathrm{Card}(\mathbf{N}) \leqslant \mathrm{Card}(\mathrm{E})$ となります。

#### 命題 3 {#ens-iii-s6-prop-3 .statement tag=03N9}

*すべての無限集合には分割* $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ *可算無限集合* $\mathrm{X}_\iota$、*添字集合* I *E と等価* があります。

$\mathrm{Card}(\mathrm{E}) = \mathrm{Card}(\mathrm{E})\ \mathrm{Card}(\mathbf{N})$ (no. 3、定理 2、系 4) の場合。

#### 命題 4 {#ens-iii-s6-prop-4 .statement tag=03NA}

*$f$ *を集合* E の写像として、 *無限の集合* F に * それぞれ* $y \in \mathrm{F}$、$\overset{-1}{f}(y)$ * が数えられるようにします。したがって、* F は * E と等価です。

E の集合 $\overset{-1}{f}(y)$ $(y \in \mathrm{F})$ 形分割の場合。したがって

$$\mathrm{Card}(\mathrm{E}) \leqslant \mathrm{Card}(\mathrm{F})\mathrm{Card}(\mathbf{N}) = \mathrm{Card}(\mathrm{F}),$$

と $\mathrm{Card}(\mathrm{F}) \leqslant \mathrm{Card}(\mathrm{E})$ by 命題 3 of § 3, no. 2。

#### 命題 5 {#ens-iii-s6-prop-5 .statement tag=03NB}

*集合* $\mathfrak{F}(\mathrm{E})$ *無限集合* の有限部分集合の E は E と * 等価です*。

それぞれの整数 $n$ について、$\mathfrak{F}_n$ は、$n$ 元を持つ E の部分集合の集合を表すものとします。それぞれの $\mathrm{X} \in \mathfrak{F}_n$ に対して、X には $[1, n]$ の全単射が存在します。したがって、$\mathfrak{F}_n$ の基数は、$[1, n]$ の写像の集合を E に変換したもの、つまり $\mathrm{Card}(\mathrm{E}^n) = \mathrm{Card}(\mathrm{E})$ (no. 3, 定理 2, 系 1) に等しくなります。したがって、

$$\mathrm{Card}(\mathfrak{F}(\mathrm{E})) = \sum_{n \in \mathbf{N}} \mathrm{Card}(\mathfrak{F}_n) \leqslant \mathrm{Card}(\mathrm{E})\mathrm{Card}(\mathbf{N}) = \mathrm{Card}(\mathrm{E}).$$

一方、$x \to \{x\}$は$\mathfrak{F}(\mathrm{E})$へのEの単射写像なので、$\mathrm{Card}(\mathrm{E}) \leqslant \mathrm{Card}(\mathfrak{F}(\mathrm{E}))$が得られます。

#### 定義 4 {#ens-iii-s6-def-4 .statement tag=03NC}

*集合は、* $\mathbf{N}$ のすべての部分集合の集合と等しい場合、連続体の冪を持つと言われます。

連続体の冪を持つ集合は可算できません(§ 3, no. 6, 定理 2)。

\* 「連続体の冪」という名前は、実数の集合が $\mathfrak{P}(\mathbf{N})$ (*一般的な位相*、章 IV, § 8) と等価であるという事実から生じています。 \* *連続体仮定* は、連続体の冪を持つすべての不可算集合含む部分集合の主張です。 *一般化された連続体仮定* は主張であり、無限の基数 $\mathfrak{a}$ ごとに、すべての基数 $> \mathfrak{a}$ は $\geqslant 2^{\mathfrak{a}}$ になります。

### 5. ステーショナリー 数列

#### 定義 5 {#ens-iii-s6-def-5 .statement tag=03ND}

*数列* $(x_n)_{n \in \mathbf{N}}$ *of 元 of 集合* E *整数* $m$ *そのような* $x_n = x_m$ *すべての整数* $n \geqslant m$ が存在する場合、E は静止していると言われます。

#### 命題 6 {#ens-iii-s6-prop-6 .statement tag=03NE}

*E *を注文された集合とします。したがって、次の主張は同等です:*

(a) *E の *空でないすべての部分集合には極大元があります。*
(b) *E *の増加する数列* $(x_n)$ *の元は静止しています*。

まず、(a) が (b) を意味することを示します。 X を数列 $(x_n)$ の元の集合とし、$x_m$ を X の極大元とします。 $n \geqslant m$ の場合、仮定 $x_n \geqslant x_m$ により、$x_m$ の最大値により $x_n = x_m$ になります。 逆に、極大元を持たないEの空ではない部分集合 Aが存在するとします。 それぞれの $x \in A$ について、$T_x$ をすべての $y \in A$ の集合とし、$y > x$ とします。 仮定までに、すべての$x \in A$に対して$T_x \neq \emptyset$。したがって、すべての $x \in A$ (章 II, § 5, no. 4, 命題 6) に対して $f(x) > x$ となる A への A の写像 $f$ が存在します。 $a \in A$ の場合、数列 $(x_n)_{n \in \mathbf{N}}$ は条件 $x_0 = a$ によって帰納的に定義され、$x_{n+1} = f(x_n)$ は明らかに増加するであり、定常ではありません。

#### 系 1 {#ens-iii-s6-prop-6-cor-1 .statement tag=03NF}

*完全に順序付けられた集合* E * が整列しているのは、* E * の元のすべての減少列が静止している場合に限ります。

なぜなら、E が整列していると言うのは、E の空でないすべての部分集合が最小の元 (§ 1, no. 10, 命題 10) を持ち、したがって主張が命題 6 から導かれるというというと同等だからです。

#### 系 2 {#ens-iii-s6-prop-6-cor-2 .statement tag=03NG}

*有限順序付けられた集合の元のすべての増加する数列は静止しています。*

すべての有限順序集合には極大元 (§ 4, no. 4、命題 3、系 2) があります。

¶ 命題 6 の同等の条件を満たす順序付けられた集合 E は、*ネーター* と言われるときどきです。

#### 命題 7 (「ネーター 帰納法の原則」) {#ens-iii-s6-prop-7 .statement tag=03RM}

— *E をネーター 集合とし、* F を * E の部分集合とします。 *次の性質 : if* $a \in E$ *が関係* $x > a$ *暗黙* $x \in F$、*then* $a \in F$。 *これら条件の下に、* F $=$ E.

実際、E $\neq$ F と仮定します。その場合、E $-$ F は極大元 $b$ になります。 定義までに、すべての $x > b$ に対して $x \in F$ が得られます。しかし、これは$b \in F$を意味しており、不合理です。

### 練習問題 {#ens-iii-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。

[^1]: It is also possible to give a direct proof of C63, analogous to the proof of C60 (§ 2, no. 2).
[^2]: The definition of the least upper bound (§ 1, nos. 7, 8, and 9) can be formulated in such a way that it has a meaning even for a set which is not bounded above (it denotes a term, in the formalized language, of the form $\tau_x(R\{x\})$, which the reader will have no difficulty in writing down).
[^3]: If $g = (G, E, E)$, the term $g(u)$ is the term denoted by $\tau_y((u, y) \in G)$.
[^4]: Here we mean the term denoted by (T, X, X), where T is the term denoted by $\mathfrak{S}_z(z$ is an ordered pair and $(\exists y)((\mathrm{pr}_1 z, y) \in \mathrm{pr}_1(\mathrm{pr}_1(u))$ and $(y, \mathrm{pr}_2 z) \in \mathrm{pr}_1(\mathrm{pr}_1(f)))$.
