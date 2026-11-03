---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 5
section_title: Decomposable linear Lie algebras
lang: ja
source: lie-vii-ix
book_pages: 34-45, 63-66
pdf_pages: 0044-0055, 0072-0075
extraction: native
subsections:
    - "no": 1
      title: DECOMPOSABLE LINEAR LIE ALGEBRAS
      page: 34
      pdf_page: 44
    - "no": 2
      title: DECOMPOSABLE ENVELOPE
      page: 37
      pdf_page: 47
    - "no": 3
      title: DECOMPOSITIONS OF DECOMPOSABLE ALGEBRAS
      page: 37
      pdf_page: 47
    - "no": 4
      title: LINEAR LIE ALGEBRAS OF NILPOTENT ENDOMORPHISMS
      page: 39
      pdf_page: 49
    - "no": 5
      title: CHARACTERIZATIONS OF DECOMPOSABLE LIE ALGEBRAS
      page: 43
      pdf_page: 53
statements: 29
exercises: 11
content_sha256: 90edf9b738d1c922ea37cd08256979b897e938d1940c3f5147684533aace4fa8
translated_from: content/en/lie/VII/05_s5_decomposable_linear_lie_algebras.md
translation_method: google
source_content_sha256: 9348eb1c66b5306a2d380eb335d4afb9f19486f3e78d4da673c181842d07b2e0
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 46134e39224c3345c43271bf7c0bedc6182b45f8e3be599478b54691251871c4
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 5。分解可能なリニアリー代数

この段落では、$k$ は標数 0 であると仮定します。V によって有限次元ベクトル空間を表します。

### 1. 分解可能なリニアリー代数

#### 定義 1 {#lie-vii-s5-def-1 .statement tag=00WG}

$\mathfrak{g}$ を $\mathfrak{g}\mathfrak{l}(V)$ の嘘部分代数とします。 Then $\mathfrak{g}$ is said to be decomposable if $\mathfrak{g}$ contains the semi-simple and nilpotent components of each of its elements (Algebra, Chap. VII, §5, no. 8).

#### 例 1 {#lie-vii-s5-n1-exa-1 .statement tag=00WH}

$V'$ と $V''$ を V のベクトル部分空間とし、$V''\supset V'$ とします。 $x(V'')\subset V'$ が分解可能な嘘 $\mathfrak{g}\mathfrak{l}(V)$ の部分代数となるような $x\in \mathfrak{g}\mathfrak{l}(V)$ の集合;実際、すべての $x\in \mathfrak{g}\mathfrak{l}$(V)、半単純、および $x$ の零能成分は、形 $P(x)$ および $Q(x)$ であり、P と Q は定数項を持たない多項式です。

#### 例 2 {#lie-vii-s5-n1-exa-2 .statement tag=00WI}

V に代数構造があると仮定します。 Vの導分の集合は、$\mathfrak{g}\mathfrak{l}(V) ($§1, no. 1の分解可能な嘘部分代数、提案4(ii))。

#### 例 3 {#lie-vii-s5-n1-exa-3 .statement tag=01KQ}

より一般的には、$\mathbf{G}\mathbf{L}(V)$ の代数部分群のリー代数が分解可能であることが示されます。\*

#### 命題 1 {#lie-vii-s5-prop-1 .statement tag=00WJ}

$\mathfrak{g}$ を、$\mathfrak{g}\mathfrak{l}(V),x\in \mathfrak{g},s$ と $n$ 半単純の分解可能な嘘部分代数と、$x$ のゼロポテンシャル成分とします。

(i) ad$_{\mathfrak{g}}x$ の半単純と nilpotent 成分は、それぞれ ad$_{\mathfrak{g}}s$ と ad$_{\mathfrak{g}}n$ です。

(ii) $x$ は、$s$ が正規である場合に限り、$\mathfrak{g}$ で正規です。

(iii) $\mathfrak{g}'$ が $\mathfrak{g}\mathfrak{l}(V)$ 含む $\mathfrak{g}$ の部分代数である場合、$\mathfrak{g}$ 拡大するの各初級自己同型から $\mathfrak{g}'$ の初級自己同型まで。

$\mathfrak{a}=\mathfrak{g}\mathfrak{l}(V)$を入れてください。章著。 ad$_{\mathfrak{a}}x$のI, §5, no. 4、補題2、半単純、および無能成分はad$_{\mathfrak{a}}s$とad$_{\mathfrak{a}}n$です。 主張 (i) はこれに続きます。 ad$_{\mathfrak{g}}x$ と ad$_{\mathfrak{g}}s$ の特性多項式は同じであると推定します。したがって (ii)。 ad$_{\mathfrak{g}}x$ がゼロの場合、ad$_{\mathfrak{g}}x=$ ad$_{\mathfrak{g}}n$ なので、ad$_{\mathfrak{g}'}n$ 拡大する ad$_{\mathfrak{g}}x$、そして $n$ は $\mathfrak{g}'$ の冪零元であるため、(iii)。

$\mathfrak{g}$ を $\mathfrak{g}\mathfrak{l}(V)$ の嘘部分代数とします。 私たちは、次の条件が同等であることを知っています (Chap. I, §6, no. 5、Th. 4)。

(i) $\mathfrak{g}$ の同一性表現は半単純です。

(ii) $\mathfrak{g}$ は還元的で、$\mathfrak{g}$ の中心のすべての元は半単純自己準同型です。

これらの条件は、実際には次のものと同等です。

(iii) $\mathfrak{g}$ は、$\mathfrak{g}\mathfrak{l}(V)$ の還元的な部分代数です。

確かに、(i) $=\Rightarrow$ (iii) 第 1 章による。 I, §6, no. 5、コル。 Thの3。 4、および (iii) $=\Rightarrow$ (i) 第 4 章による。 I, §6, no. 6、コル。提案 7 の 1. $\mathfrak{g}$ がこれらの条件を満たす場合、$\mathfrak{g}$ は分解可能であることを示します。より一般的には:

#### 命題 2 {#lie-vii-s5-prop-2 .statement tag=00WK}

$\mathfrak{g}$ を $\mathfrak{g}\mathfrak{l}(V)$ における還元的な $\mathfrak{g}\mathfrak{l}(V)$ の嘘部分代数とし、E を有限次元のベクトル空間および E 上の $\mathfrak{g}$ の $\pi :\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(E)$ 半単純線型表現とします。

(i) $\mathfrak{g}$ と $\pi (\mathfrak{g})$ は分解可能です。

(ii) $\pi (\mathfrak{g})$ の半単純 (それぞれ nilpotent) 要素は、$\mathfrak{g}$ の半単純 (それぞれ nilpotent) 要素の $\pi$ の下にある画像です。

(iii) $\mathfrak{h}$ が分解可能な$\mathfrak{g},\pi (\mathfrak{h})$ に含まれる$\mathfrak{g}\mathfrak{l}(V)$ の部分代数は、$\mathfrak{g}\mathfrak{l}(E)$ の分解可能な部分代数である。

(iv) $\mathfrak{h}'$ が分解可能な場合、$\mathfrak{g}\mathfrak{l}(E),\pi^{-1}(\mathfrak{h}')$ の部分代数は $\mathfrak{g}\mathfrak{l}(V)$ の分解可能な部分代数です。

$\mathfrak{s}= [\mathfrak{g},\mathfrak{g}]$ と $\mathfrak{c}$ を $\mathfrak{g}$ の中心とします。 次に、チャプターによる$\mathfrak{g}=\mathfrak{s}\times \mathfrak{c}$、および$\pi (\mathfrak{g}) =$ $\pi (\mathfrak{s})\times \pi (\mathfrak{c})$ I, §6, no. 4、コル。提案 5 の。 $y\in \mathfrak{s}, z\in \mathfrak{c}, y_s$ と $y_n$ 半単純および $y$ の無能成分を仮定します。 Then $y_s, y_n\in \mathfrak{s}$ (Chap. I, §6, no. 3, Prop. $3$)$,y_s+z$ is semi-simple (Algebra, Chap. VII, §5, no. 7, Cor. of Prop. 16), and $y_n$ commutes with $y_s+z$. したがって、$y+z$ の半単純と無能成分は、$y_s+z$ と $y_n$ です。 したがって、$\mathfrak{g}$ は分解可能です。 $\mathfrak{g}\mathfrak{l}$(E) では $\pi (\mathfrak{g})$ が還元的であるため、同じ議論が $\pi (\mathfrak{g})$ にも当てはまり、$\pi (\mathfrak{g})$ が分解可能であることがわかります。 さらに、$\mathfrak{g}$ (それぞれ $\pi (\mathfrak{g})$) の冪零元は、$\mathfrak{s}$ (それぞれ $\pi (\mathfrak{s})$) の冪零元です。 したがって、$\pi (\mathfrak{g})$の冪零元は、$\mathfrak{g}$の冪零元の$\pi$の下にある像になります（I, §6, no. 3章、提案4）。 $\mathfrak{g}$ (それぞれ $\pi (\mathfrak{g})$) の半単純要素は、$\mathfrak{s}$ (それぞれ $\pi (\mathfrak{s})$) の半単純要素と $\mathfrak{c}$ (それぞれ $\pi (\mathfrak{c})$) の要素の合計です。 したがって、$\pi (\mathfrak{g})$ の半単純要素は、$\mathfrak{g}$ の半単純要素の$\pi$ の下にある画像です (I 章、前掲)。 したがって、(ii)。

主張 (iii) と (iv) は、(i) と (ii) の直後に続きます。

#### 注意 1 {#lie-vii-s5-n1-rem-1 .statement tag=00WL}

$\pi$ の半単純性仮定は、$\pi (x)$ がすべての $x\in \mathfrak{c}$ に対して半単純であるというと同等です。この仮定は、次の演算を連続的に適用することによって、同一性表現 $\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(V)$ から $\pi$ が得られるときに満たされることに注意してください: テンソル積、双対への移行、部分表現、商、直和へ。

#### 注意 2 {#lie-vii-s5-n1-rem-2 .statement tag=00WM}

$\mathfrak{g}\subset \mathfrak{g}\mathfrak{l}$(V)、$\mathfrak{g}'\subset \mathfrak{g}\mathfrak{l}(V')$を$\mathfrak{g}$から$\mathfrak{g}'$まで分解可能リー代数、$\varphi$同型とします。 $\varphi$ は、必ずしも $\mathfrak{g}$ の変換半単純 (それぞれ無能) 元から $\mathfrak{g}'$ の半単純 (それぞれ無能) 元になるわけではないことに注意してください (例題 2)。ただし、$\mathfrak{g}$が半単純の場合はこの限りです（I, §6, no. 3、第3章）。

#### 命題 3 {#lie-vii-s5-prop-3 .statement tag=00WN}

$\mathfrak{a}$ を $\mathfrak{g}\mathfrak{l}(V)$ の分解可能な嘘部分代数とし、$\mathfrak{b}$ と $\mathfrak{c}$ を $\mathfrak{b}\subset \mathfrak{c}$ となるような $\mathfrak{g}\mathfrak{l}(V)$ のベクトル部分空間とします。 $\mathfrak{a}'$ を $x\in \mathfrak{a}$ の集合として、$[x,\mathfrak{c}]\subset \mathfrak{b}$ とします。すると$\mathfrak{a}'$は分解可能です。

$\mathfrak{g}=\mathfrak{g}\mathfrak{l}(V)$を入れてください。 部分代数 $\mathfrak{g}\mathfrak{l}(\mathfrak{g})$ の $\mathfrak{h}'$ $z\in \mathfrak{g}\mathfrak{l}(\mathfrak{g})$ のからなるは、$z(\mathfrak{c})\subset \mathfrak{b}$ が分解可能です (例 1)。 $\pi :\mathfrak{g}\rightarrow \mathfrak{g}\mathfrak{l}(\mathfrak{g})$ を $\mathfrak{g}$ の随伴物表現とします。 $\pi$ に適用される提案 2 (iv) は、$\pi^{-1}(\mathfrak{h}')$ が分解可能であることを示しています。従って、$\mathfrak{a}'=\mathfrak{a}\cap \pi^{-1}(\mathfrak{h}')$も同様です。

#### 系 1 {#lie-vii-s5-prop-3-cor-1 .statement tag=00WO}

$\mathfrak{a}$ が $\mathfrak{g}\mathfrak{l}(V)$ の分解可能な嘘部分代数であり、$\mathfrak{n}$ が $\mathfrak{a}$ の嘘部分代数である場合、$\mathfrak{a}$ の $\mathfrak{n}$ のノーマライザー (セントラライザー) は分解可能です。

これは、$\mathfrak{c}=\mathfrak{n},\mathfrak{b}=\mathfrak{n}$ (それぞれ $\mathfrak{c}=\mathfrak{n},\mathfrak{b}=\{0\}$) を採用することで、提案 3 から導き出されます。

#### 系 2 {#lie-vii-s5-prop-3-cor-2 .statement tag=00WP}

分解可能な嘘のカルタン部分代数 $\mathfrak{g}\mathfrak{l}(V)$の部分代数は分解可能です。

これは系 1から続きます。

#### 注意 {#lie-vii-s5-n1-rem-3 .statement tag=00WQ}

後で、コルの逆 (no. 5、Th. 2) を証明します。 2.

### 2. 分解可能包絡

分解可能な嘘のファミリーの共通部分 $\mathfrak{g}\mathfrak{l}(V)$ の部分代数は明らかに分解可能です。従って、$\mathfrak{g}$が$\mathfrak{g}\mathfrak{l}$(V)の嘘部分代数である場合、$\mathfrak{g}\mathfrak{l}(V)$含む$\mathfrak{g}$の分解可能な嘘部分代数の集合は最小のを持ちます。 元、$\mathfrak{g}$の分解可能包絡と呼ばれます。この段落では、この封筒は $e(\mathfrak{g})$ で示されます。

#### 命題 4 {#lie-vii-s5-prop-4 .statement tag=00WR}

$\mathfrak{g}$を$\mathfrak{g}\mathfrak{l}(V)$の嘘部分代数、$\mathfrak{n}$を$\mathfrak{g}$の理想とする。すると$\mathfrak{n}$と$e(\mathfrak{n})$は$e(\mathfrak{g})$と$[e(\mathfrak{g}), e(\mathfrak{n})] = [\mathfrak{g},\mathfrak{n}]$の理想となります。

$\mathfrak{g}_1$ を $x\in \mathfrak{g}\mathfrak{l}(V)$ の集合とし、$[x,\mathfrak{n}]\subset [\mathfrak{g},\mathfrak{n}]$ とします。これは、$\mathfrak{g}\mathfrak{l}$(V)、含む $\mathfrak{g}$ の分解可能な嘘部分代数であるため、$e(\mathfrak{g})$、cf. no. 1、提案 3。他には語、$[e(\mathfrak{g}),\mathfrak{n}]\subset [\mathfrak{g},\mathfrak{n}]$。 $\mathfrak{n}_1$ を $y\in \mathfrak{g}\mathfrak{l}(V)$ の集合とすると、次のようになります。

$$
[e(\mathfrak{g}), y]\subset [\mathfrak{g},\mathfrak{n}]
$$

これは、前のものによる $\mathfrak{g}\mathfrak{l}(V)$ 含む $\mathfrak{n}$ の分解可能な嘘部分代数であるため、 含む $e(\mathfrak{n})$ になります。他の語 $[e(\mathfrak{g}), e(\mathfrak{n})]\subset [\mathfrak{g},\mathfrak{n}]$ では、

$$
[e(\mathfrak{g}), e(\mathfrak{n})] = [\mathfrak{g},\mathfrak{n}]
$$

従って、$[e(\mathfrak{g}),\mathfrak{n}]\subset [e(\mathfrak{g}), e(\mathfrak{n})]\subset \mathfrak{n}$ であるため、$\mathfrak{n}$ と $e(\mathfrak{n})$ は $e(\mathfrak{g})$ の理想となります。

#### 系 1 {#lie-vii-s5-prop-4-cor-1 .statement tag=00WS}

(i) $i\geq 1$ の場合は $\mathscr{D}^i\mathfrak{g}=\mathscr{D}^ie(\mathfrak{g})$、$i\geq 2$ の場合は $\mathscr{C}^i\mathfrak{g}=\mathscr{C}^ie(\mathfrak{g})$。

(ii) $\mathfrak{g}$ が可換 (それぞれ nilpotent、それぞれ可解) の場合、$e(\mathfrak{g})$ は可換 (それぞれ nilpotent、それぞれ可解) です。

主張 (i) は、$i$ の帰納法による提案 4 から得られ、(ii) は (i) から得られます。

#### 系 2 {#lie-vii-s5-prop-4-cor-2 .statement tag=00WT}

$\mathfrak{r}$ を $\mathfrak{g}$ の根基とします。 $\mathfrak{g}$ が分解可能であれば、$\mathfrak{r}$ も分解可能です。

実際、$e(\mathfrak{r})$ は、提案 4 と Cor による $\mathfrak{g}$ の解決可能な理想です。 1 なので $e(\mathfrak{r}) =\mathfrak{r}$ です。

### 3. 分解分解可能代数

$\mathfrak{g}$ が根基 $\mathfrak{r}$ を伴う $\mathfrak{g}\mathfrak{l}(V)$ の嘘部分代数である場合、$\mathfrak{r}$ の冪零元の集合は $\mathfrak{g}$ の零位理想であり、最大の同一性の零位理想です。 $\mathfrak{g}$の表現 (第1章I, §5, no. 3、コリント6)。 この段落では、この理想を $\mathfrak{n}_V(\mathfrak{g})$ で表すことにします。 It contains the nilpotent radical $[\mathfrak{g},\mathfrak{g}]\cap \mathfrak{r}$ of $\mathfrak{g}$ (Chap. I, §5, no. 3, Th. 1).

#### 命題 5 {#lie-vii-s5-prop-5 .statement tag=00WU}

$\mathfrak{g}$ を、$\mathfrak{g}\mathfrak{l}(V)$ の分解可能な nilpotent 嘘部分代数とします。 $\mathfrak{t}$ を半単純の集合 $\mathfrak{g}$ の元とします。すると、$\mathfrak{t}$は$\mathfrak{g}$の中心部分代数、$\mathfrak{g}$は$\mathfrak{t}$の積、$\mathfrak{n}_V(\mathfrak{g})$はリー代数となります。

$x\in \mathfrak{t}$ の場合、ad$_{\mathfrak{g}}x$ は半単純で零であるため、零となり、$x$ は $\mathfrak{g}$ の中心になります。従って、$\mathfrak{t}$は$\mathfrak{g}$、$\mathfrak{t}\cap \mathfrak{n}_V(\mathfrak{g}) = 0$の理想となります。 $\mathfrak{g}$ は分解可能であるため、$\mathfrak{g}=\mathfrak{t}+\mathfrak{n}_V(\mathfrak{g})$、したがって命題になります。

#### 命題 6 {#lie-vii-s5-prop-6 .statement tag=00WV}

$\mathfrak{g}$ を $\mathfrak{g}\mathfrak{l}(V)$ の分解可能な嘘部分代数とします。 $\mathscr{T}$ を、$\mathfrak{g}$ の可換部分代数の集合、半単純元のからなる、および $\mathscr{T}$ の極大元の $\mathscr{T}_1$ 集合とします。 $\mathscr{H}$ を $\mathfrak{g}$ のカルタン部分代数の集合とします。

(i) $\mathfrak{h}\in \mathscr{H}$ について、$\varphi (\mathfrak{h})$ を半単純の集合 $\mathfrak{h}$ の元とします。次に$\varphi (\mathfrak{h})\in \mathscr{T}_1$。

(ii) $\mathfrak{t}\in \mathscr{T}_1$ について、$\psi (\mathfrak{t})$ を $\mathfrak{g}$ の $\mathfrak{t}$ の交換子環とします。次に$\psi (\mathfrak{t})\in \mathscr{H}$。

(iii) 写像 $\varphi$ と $\psi$ は、$\mathscr{H}$ から $\mathscr{T}_1$ までと $\mathscr{T}_1$ から $\mathscr{H}$ までの逆全単射です。

(iv) $k$ が代数的に閉じている場合、Aut$_e(\mathfrak{g})$ は $\mathscr{T}_1$ で推移的に動作します。

$\mathfrak{h}\in \mathscr{H}$ として、$\mathfrak{t}=\varphi (\mathfrak{h})$ を置きます。 提案 5 および Cor.提案$3,\mathfrak{t}\in \mathscr{T}$および$\mathfrak{h}=\mathfrak{t}\times \mathfrak{n}_V(\mathfrak{h})$の2。 $\mathfrak{g}$ の任意の部分代数 $\mathfrak{u}$ については、$\mathfrak{g}$ の $\mathfrak{u}$ の $\psi (\mathfrak{u})$ 交換子環で表します。 次に、$\mathfrak{h}\subset \psi (\mathfrak{t})$ と $\psi (\mathfrak{t})\subset \mathfrak{g}^0(\mathfrak{h})$ は、$\mathfrak{n}_V(\mathfrak{h})$ の元が零であるため、$\mathfrak{h}=\psi (\mathfrak{t})$ になります。 $\mathfrak{t}'\in \mathscr{T}$ と $\mathfrak{t}\subset \mathfrak{t}'$ の場合、$\mathfrak{t}'\subset \psi (\mathfrak{t}) =\mathfrak{h}$ があるため、$\mathfrak{t}'=\mathfrak{t}$、したがって $\mathfrak{t}\in \mathscr{T}_1$ になります。

$\mathfrak{t}\in \mathscr{T}_1$ として、$\mathfrak{c}=\psi (\mathfrak{t})$ を置きます。 $\mathfrak{h}$を$\mathfrak{c}$のカルタン部分代数とします。 §2, no. 3、提案$10,\mathfrak{h}\in \mathscr{H}$および$\mathfrak{t}\subset \mathfrak{h}$により。 $\mathfrak{t}_1=\varphi (\mathfrak{h})\in \mathscr{T}$を入れます。次に、$\mathfrak{t}\subset \mathfrak{t}_1$ なので、$\mathfrak{t}=\mathfrak{t}_1$、そしてその前の$\mathfrak{h}=\psi (\mathfrak{t}_1) =\psi (\mathfrak{t}) =\mathfrak{c}$ になります。したがって、$\psi (\mathfrak{t})\in \mathscr{H}$、および$\varphi (\psi (\mathfrak{t})) =\mathfrak{t}$となります。

したがって、(i)、(ii)、(iii) が証明されました。 $k$ が代数的に閉じていると仮定します。 Aut$_e(\mathfrak{g})$ は $\mathscr{H}($§3, no. 2 で推移的に動作するため、Th. 1)、Aut$_e(\mathfrak{g})$は$\mathscr{T}_1$で推移的に動作します。

#### 系 1 {#lie-vii-s5-prop-6-cor-1 .statement tag=00WW}

$\mathfrak{g}$ のカルタン部分代数は、$\mathfrak{g}$ の通常の半単純元の中心人物です。

$x\in \mathfrak{g}$ が正規の場合、$\mathfrak{g}^0(x)$ は $\mathfrak{g}($§2, no. 3 のカルタン部分代数です。 1(i));さらに、$x$ が半単純の場合、$\mathfrak{g}^0(x)$ は $\mathfrak{g}$ の $x$ のセントラライザーです。逆に、$\mathfrak{h}$を$\mathfrak{g}$のカルタン部分代数とします。 $\mathfrak{h}=\psi (\mathfrak{t})$ となるような $\mathfrak{t}\in \mathscr{T}_1$ が存在します。 §1, no. 2、提案 7 により、$\mathfrak{h}=\mathfrak{g}^0(x)$ となるような $x\in \mathfrak{t}$ が存在します。 $x\in \mathfrak{t}$、$\mathfrak{g}^0(x) =\mathfrak{g}_0(x)$から。 §3, no. 3までに、Th。 2(ii)、$x$はレギュラーです。

#### 系 2 {#lie-vii-s5-prop-6-cor-2 .statement tag=00WX}

加法で $\mathfrak{g}$ が解けると仮定します。次に:

(i) Aut($\mathfrak{g}$) の部分群 $e^{adx}, x\in \mathscr{C}^{\infty}\mathfrak{g}$ (cf. §3, no. 4) のからなるは、$\mathscr{T}_1$ で推移的に動作します。

(ii) $\mathfrak{t}\in \mathscr{T}_1,\mathfrak{g}$ が $\mathfrak{t}$ と $\mathfrak{n}_V(\mathfrak{g})$ の半直接積である場合。

主張 (i) は、$e^{adx},x\in \mathscr{C}^{\infty}\mathfrak{g}$ の群が $\mathscr{H}($§3, no. 4 で推移的に動作するという事実から導き出されます。 3)。

(ii)を証明します。 $\mathfrak{t}\in \mathscr{T}_1$ を、$\mathfrak{h}=\psi (\mathfrak{t})$ を $\mathfrak{g}$ の対応するカルタン部分代数とします。提案$5,\mathfrak{h}=\mathfrak{t}+\mathfrak{n}_V(\mathfrak{h})\subset \mathfrak{t}+\mathfrak{n}_V(\mathfrak{g})$を考慮して。一方、$\mathfrak{g}=\mathfrak{h}+ [\mathfrak{g},\mathfrak{g}] ($§2, no. 1、コル。提案 4 の 3) と $[\mathfrak{g},\mathfrak{g}]\subset \mathfrak{n}_V(\mathfrak{g})$ なので、$\mathfrak{g}=\mathfrak{t}+\mathfrak{n}_V(\mathfrak{g})$。しかし、$\mathfrak{t}\cap \mathfrak{n}_V(\mathfrak{g}) =\{0\}$であることは明らかです。したがって、代数 $\mathfrak{g}$ は、$\mathfrak{t}$ の半直接的な積であり、イデアル $\mathfrak{n}_V(\mathfrak{g})$ です。

#### 命題 7 {#lie-vii-s5-prop-7 .statement tag=00WY}

$\mathfrak{g}$ を $\mathfrak{g}\mathfrak{l}(V)$ の分解可能な嘘部分代数とします。

(i) $\mathfrak{g}$ が $\mathfrak{m}$ と $\mathfrak{n}_V(\mathfrak{g})$ の半直接積となるように、$\mathfrak{g}\mathfrak{l}(V)$ に還元的な$\mathfrak{g}$ の嘘部分代数 $\mathfrak{m}$ が存在します。

(ii) (i) の性質を持つ $\mathfrak{g}$ の任意の 2 つの嘘部分代数は、Aut$_e(\mathfrak{g})$ では共役になります。

$\mathfrak{g}$ の根基 $\mathfrak{r}$ は分解可能です (no. 2、提案 4 の Cor. 2)。 コル著提案 6 の 2 では、$\mathfrak{r}$ の可換部分代数 $\mathfrak{t}$、半単純元のからなるが存在し、$\mathfrak{r}=\mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{r})$ となります。 ad$_{\mathfrak{g}}\mathfrak{t}$ は半単純な要素で構成されているため、$\mathfrak{g}$ は $[\mathfrak{t},\mathfrak{g}]$ と $\mathfrak{t}$ のセントラライザー $\mathfrak{z}$ の直接和になります (I, §3, no. 5 案 6)。 $[\mathfrak{t},\mathfrak{g}]\subset \mathfrak{r},\mathfrak{g}=\mathfrak{z}+\mathfrak{r}$から。 Consequently, if $\mathfrak{s}$ is a Levi subalgebra of $\mathfrak{z}$ (Chap. I, §6, no. $8$)$,\mathfrak{g}=\mathfrak{s}+\mathfrak{r}$, so $\mathfrak{s}$ is a Levi subalgebra of $\mathfrak{g}$. $\mathfrak{m}=\mathfrak{s}\oplus \mathfrak{t}$を入れてください。 $[\mathfrak{s},\mathfrak{t}] =\{0\},\mathfrak{m}$は$\mathfrak{g}$の嘘部分代数なので、第2章で$\mathfrak{g}\mathfrak{l}(V)$に還元されます。 I, §6, no. 5、木。 4. さらに、

$$
\mathfrak{g}=\mathfrak{s}\oplus \mathfrak{r}=\mathfrak{s}\oplus \mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{r}) =\mathfrak{s}\oplus \mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{g}) =\mathfrak{m}\oplus \mathfrak{n}_V(\mathfrak{g})
$$

$\mathfrak{n}_V(\mathfrak{g}) =\mathfrak{n}_V(\mathfrak{r})$から。従って、(i)。

さて、$\mathfrak{m}'$ を、$\mathfrak{n}_V(\mathfrak{g})$ を補う$\mathfrak{g}$ の嘘部分代数とし、$\mathfrak{g}\mathfrak{l}(V)$ で還元的とします。 Aut$_e(\mathfrak{g})$ では、$\mathfrak{m}'$ が共役から $\mathfrak{m}$ であることがわかります。 $\mathfrak{m}'=\mathfrak{s}'\oplus \mathfrak{t}'$があり、$\mathfrak{s}'= [\mathfrak{m}',\mathfrak{m}']$は半単純、$\mathfrak{m}'$の中心$\mathfrak{t}'$は半単純元で構成されます。それから$\mathfrak{r}=\mathfrak{t}\oplus \mathfrak{n}_V(\mathfrak{g}) =\mathfrak{t}'\oplus \mathfrak{n}_V(\mathfrak{g})$。コルの観点から。提案 6 の 2 では、ケース $\mathfrak{t}=\mathfrak{t}'$ に帰着します。それから$\mathfrak{s}'\subset \mathfrak{z}$; dim$\mathfrak{s}'=$ dim$\mathfrak{s}$ なので、$\mathfrak{s}'$ は $\mathfrak{z}$ の Levi 部分代数です。章著。 I, §6, no. 8、木曜日。 5、$e^{adx}(\mathfrak{s}) =\mathfrak{s}'$となるような$x\in \mathfrak{n}_V(\mathfrak{z})$が存在します。 $x$ は $\mathfrak{t}$ と通勤しているため、$e^{adx}(\mathfrak{t}) =\mathfrak{t}$ もいます。

### 4. 線形リー代数/冪零自己準同型

#### 補題 1 {#lie-vii-s5-lem-1 .statement tag=00WZ}

$\mathfrak{n}$ を、$\mathfrak{g}\mathfrak{l}(V)$ からなるの冪零自己準同型の嘘部分代数、および $\mathbf{G}\mathbf{L}(V) ($§3, no. 1、補題の N 部分群 exp$\mathfrak{n}$ とする 1)。

(i) $\rho$ を W 上の $\mathfrak{n}$ の有限次元線型表現とし、$\rho (\mathfrak{n})$ の元が零能であり、W の $W'$ ベクトル部分空間が $\rho ,\rho_1$ と $\rho_2$ の下で安定であるようにします。 $\rho , \rho_1, \rho_2($§3, no. 1 と互換性のある N の $W',\pi , \pi_1, \pi_2$ 表現によって定義される $\rho$ の部分表現および商表現)。すると、$\pi_1, \pi_2$ は、$W'$ によって定義される $\pi$ の部分表現と商表現になります。

(ii) $\rho_1, \rho_2$ を有限次元 $\mathfrak{n}$ の線型表現とし、$\rho_1(\mathfrak{n})$ と $\rho_2(\mathfrak{n})$ の元が冪能であり、N の $\pi_1, \pi_2$ 表現が $\rho_1, \rho_2$ と互換性があるとします。すると$\pi_1\otimes \pi_2$は$\rho_1\otimes \rho_2$と互換性のあるNの表現になります。

(iii) $\rho_1, \rho_2$ を、ベクトル空間 $V_1,V_2$ 上の $\mathfrak{n}$ の有限次元線型表現とし、$\rho_1(\mathfrak{n})$ と $\rho_2(\mathfrak{n})$ の元がゼロポテンツ、$\rho$ 表現がゼロであるようにします。 $\rho_1, \rho_2$によって決定されるホム(V$_1,V_2$)の$\mathfrak{n}$。 $\pi_1, \pi_2$ を $\rho_1, \rho_2$ と互換性のある N の表現とし、$\pi_1, \pi_2$ によって決定されるホム上の N (V$_1,V_2$) の $\pi$ 表現とします。すると、$\pi$は$\rho$と互換性のあるNの表現になります。

主張 (i) はクリアです。 $\rho_1, \rho_2, \pi_1, \pi_2$ を (ii) のようにします。 $x\in \mathfrak{n}$ の場合、$\rho_1(x)\otimes 1$ と $1\otimes \rho_2(x)$ は通勤しているため、

経験値($\rho_1(x)\otimes 1 + 1\otimes \rho_2(x)$) $=$ 経験値($\rho_1(x)\otimes 1$)。経験値(1 $\otimes \rho_2(x)$)

= (経験値$\rho_1(x)$)$\otimes 1.1\otimes$ (経験値$\rho_2(x)$)

= (経験値$\rho_1(x)$)$\otimes$ (経験値$\rho_2(x)$)

$=\pi_1$(経験値$x$)$\otimes \pi_2$(経験値$x$)

$= (\pi_1\otimes \pi_2$)(経験値$x$)、

従って (ii)。 $\rho_1, \rho_2, \rho , \pi_1, \pi_2, \pi ,V_1,V_2$ を (iii) のようにします。 $v_1\in$ EndV$_1$ と $v_2\in$ EndV$_2$ の場合、Hom(V$_1,V_2$) からそれ自体まで $R_{v_1}$ と $L_{v_2}$ 写像 $u \rightarrow uv_1$ と $u \rightarrow v_2u$ で表します。これら写像通勤と $\rho (x)u= (L_{\rho_2(x)}-R_{\rho_1(x)})u$ なので

経験値$\rho (x).u=$ 経験値$L_{\rho_2(x)}$。経験値 $R_{-\rho_1(x)}.u$

$$
= L_{exp\rho_2(x)}.R_{exp(-\rho_1(x))}.u
$$

$$
= L_{\pi_2(expx)}.R_{\pi_1(exp(-x))}.u
$$

$=\pi$(経験値$x$)$.u$,

従って (iii)。

#### 補題 2 {#lie-vii-s5-lem-2 .statement tag=01JS}

$^2$ (i) W を次元 $d$ の V のベクトル部分空間とし、D を$\bigwedge V$ の$\mathfrak{g}\mathfrak{l}(V)$ の正規表現の行$\bigwedge^dW\subset \bigwedge^dV,\theta$ とします（第 2 章）。 III、App.)。 $x\in \mathfrak{g}\mathfrak{l}(V)$ にしましょう。次に、$\theta (x)(D)\subset D$ の場合に限り、$x(W)\subset W$ になります。

(ii) $(e_1, . . . , e_n)$ を、$\bigwedge(k^n)$ および$x\in \mathfrak{g}\mathfrak{l}(n, k)$ における$\mathfrak{g}\mathfrak{l}(n, k)$ の標準表現である$k^n,\theta$ の標準基底とします。それでは $x\in \mathfrak{n}(n, k)$ もし、そしてその場合に限り

$$
\theta (x)(e_{n-d+1}\wedge  \cdots  \wedge e_n) = 0
$$

$1\leq d\leq n$の場合。

(i) $x(W)\subset W$ であれば、$\theta (x)D\subset D$ であることは明らかです。逆に$\theta (x)D\subset D$とします。 $u$ を D の非ゼロ元とし、$y\in W$ とします。それから$y\wedge u= 0$。 $\theta (x)$ は $\bigwedge V$ の導分であるため、これは意味します

$$
\theta (x)y\wedge u+y\wedge \theta (x)u= 0
$$

現在$\theta (x)u\in ku$なので、$y\wedge \theta (x)u= 0$、その結果、$\theta (x)y\wedge u= 0$となります。 代数著、第 1 章III, §7, no. 9、提案 13、これは $\theta (x)y\in W$、つまり $x(y)\in W$ を意味し、$x(W)\subset W$ を証明します。

(ii) (ii)に記載の条件は$x\in \mathfrak{n}(n, k)$に明らかに必要です。満たされていると仮定します。 (i)までに、$x$は出発します

$^2$ この補題において、$k$ は任意の (可換な) 体になる可能性があります。

$$
ke_{n-d+1}+\cdots +ke_n
$$

安定しており、これが$d= 1, . . . , n,x$に当てはまるため、下三角になります。置く

$$
x= (x_{ij})_{1\leq i,j\leq n}
$$

$0 =x(e_n) =x_{nn}e_n$ があるので、$x_{nn}= 0$ です。 $i < n$ として、$j > i$ に対して $x_{jj}= 0$ が証明されたと仮定します。それから

$$
0 =\theta (x)(e_i\wedge e_{i+1}\wedge  \cdots  \wedge e_n) =x_{ii}(e_i\wedge e_{i+1}\wedge  \cdots  \wedge e_n)
$$

だから$x_{ii}= 0$。したがって、$x\in \mathfrak{n}(n, k)$。

#### 命題 8 {#lie-vii-s5-prop-8 .statement tag=00X0}

$\mathfrak{n}$ を、$\mathfrak{g}\mathfrak{l}(V)$ の嘘部分代数、冪零元のからなる、$\mathfrak{g}\mathfrak{l}(V)$ の$\mathfrak{n}$ の正規化$\mathfrak{q}$ とします。 E 上の $\mathfrak{g}\mathfrak{l}(V)$ の有限次元ベクトル空間 E、表現 $\rho$、および E のベクトル部分空間 F、次の条件の満たすが存在します。

(i) V のホモテティー の $\rho$ の下の像は対角化可能です。

(ii) F は $\rho (\mathfrak{q})$ で安定です。

(iii) $\mathfrak{n}$ は、$\rho (x)(F) = 0$ となるような $x\in \mathfrak{g}\mathfrak{l}(V)$ の集合です。

$n=$をVを暗くしましょう。エンゲルの定理により、V は $\mathfrak{n}\subset \mathfrak{n}(n, k)$ という形で $k^n$ と識別できます。 P を $\mathfrak{g}\mathfrak{l}(n, k)$ の多項式関数の代数とします。 $i= 0,1, . .$. について、$P_i$ を次数 $i$ の同次 P の元の集合とします。 N = exp $\mathfrak{n}$ とします。これは、厳密に下三角群 T の部分群です。J を、N 上の零である P の元の集合とします。これは P の理想です。$N_J$ を $x\in \mathfrak{g}\mathfrak{l}(n, k)$ の集合とし、すべての $p\in J$ に対して $p(x) = 0$ とします。続いて$N\subset N_J$。逆に$x\in N_J$とします。 $\mathfrak{g}\mathfrak{l}(n, k)$ の元のエントリを与える $p_{ij}$ 多項式関数で表します。イデアル J 含む、$p_{ij}$ ($i < j$) および $p_{ii}-1$。したがって $x\in T$ です。一方、$u$が$\mathfrak{g}\mathfrak{l}(n, k)$では線型形式、$\mathfrak{n}$では零である場合、すべての$z\in T ($§3, no. 1に対して$p_u(z) =u$(log$z$)となるような$p_u\in P$が存在します。 補題 1 (i)); $p_u\in J$ があるので、$u$(log $x$) $= 0$ です。 $x$ 属するから $\mathfrak{n}$ までのログが続くため、$x\in N$、証明、そして $N = N_J$ となります。

すべての $p\in P$ と $g\in \mathbf{G}\mathbf{L}_n(k)$ について、$\lambda (g)p$ を $\mathfrak{g}\mathfrak{l}(n, k)$ の写像 $x \rightarrow p(g^{-1}x)$ とします。その場合、$\lambda (g)p\in P,\lambda (g)$ は代数 P の自己同型であり、$\lambda$ は P の $\mathbf{G}\mathbf{L}_n(k)$ の表現であり、それぞれの $P_i$ は安定します。私たちはそれを示します

$$
N =\{x\in \mathbf{G}\mathbf{L}_n(k)|\lambda (x)J = J\} \tag{1}
$$

$x\in N, p\in J, y\in N$ の場合、$x^{-1}y\in N$ から $(\lambda (x)p)(y) =p(x^{-1}y) = 0$。したがって、$\lambda (x)p\in J$、したがって、$\lambda (x)J = J$。 $x\in \mathbf{G}\mathbf{L}_n(k)$ を $\lambda (x)J = J$ となるようにします。 $p\in J$ にしましょう。次に$p(x^{-1}) = (\lambda (x)p)(e) = 0$、つまり$x^{-1}\in N_J= N$と$x\in N$です。これは(i)を証明します。

イデアル J は有限型 (可換代数、Chap. III, §2, no. 10、Th. 2 の Cor. 2) です。 したがって、$W = P_0+ P_1+\cdots + P_q$ の場合、理想として $J\cap W$ 生成する J となるような整数 $q$ が存在します。 $P_J$ (それぞれ W) によって定義された $\lambda$ の部分表現を $\lambda_j$ (それぞれ $\lambda '$) で表します。 (1)により、

$$
N =\{x\in \mathbf{G}\mathbf{L}_n(k)|\lambda '(x)(J\cap W) = J\cap W\} \tag{2}
$$

すべての $j$ について、$P_j$ には次のようなリー代数 $\mathfrak{g}\mathfrak{l}(n, k)$ の表現 $\sigma_j$ が存在することを示します。

$\sigma_j|\mathfrak{n}(n, k)$ は $\lambda_j|T$ と互換性があります (§$3$、いいえ$.1$)。 (3)

すべての$x\in k.1_n, \sigma_j(x)$ はホモテティー です。 (4)

$\lambda_j$ は $\lambda_1$ の $j$ 番目の対称冪であるため、$\sigma_1$、cf. 補題 1 の存在を証明するだけで十分です。今、$\lambda_1$ は表現の反格表現です。 $\mathfrak{g}\mathfrak{l}(n, k)$ の $\mathbf{G}\mathbf{L}_n(k)$ の $\gamma$ を提供者

$$
\gamma (x)y=xy, x\in \mathbf{G}\mathbf{L}_n(k), y\in \mathfrak{g}\mathfrak{l}(n, k)
$$

$c$ を、次の式で与えられる $\mathfrak{g}\mathfrak{l}(n, k)$ のリー代数 $\mathfrak{g}\mathfrak{l}(n, k)$ の表現とします。

$$
c(x)y=xy, x, y\in \mathfrak{g}\mathfrak{l}(n, k)
$$

$c|\mathfrak{n}(n, k)$と$\gamma |T$が互換性があるのは明らかであり、$x\in k.1_n$すべてに対して$c(x)$はホモテティーです。 Thus, it suffices to take for $\sigma_1$ the dual representation of $c$ (Chap. I, §3, no. 3).

ここで、$\sigma '$ を、$\sigma_j, 0\leq j\leq q$ の直和によって与えられる W 上の $\mathfrak{g}\mathfrak{l}(n, k)$ の表現とします。 (2)と関係を考慮して

$\lambda '$(exp($x$)) $=$ exp($\sigma '(x)$) および $\sigma '$(log($y$)) $=$ log($\lambda '(y)$)$, x\in \mathfrak{n}(n, k), y\in T$,

我々は持っています

$$
\mathfrak{n}=\{x\in \mathfrak{n}(n, k)|\sigma '(x)(J\cap W)\subset J\cap W\} \tag{5}
$$

$d=$ を暗くし(J $\cap W$)、$\tau =\bigwedge^d\sigma '$ にします。 $D =\bigwedge^d(J\cap W)$ にしましょう。 (5) と補題 2 (i) により、

$$
\mathfrak{n}=\{x\in \mathfrak{n}(n, k)|\tau (x)(D)\subset D\} \tag{6}
$$

ただし、$\tau (\mathfrak{n}(n, k))$ は冪零自己準同型で構成されているため、(6) とも書くことができます。

$$
\mathfrak{n}=\{x\in \mathfrak{n}(n, k)|\tau (x)(D) = 0\} \tag{7}
$$

さて、$E =\bigwedge^dW\oplus \bigwedge^1V\oplus \bigwedge^2V\oplus  \cdots  \oplus \bigwedge^nV$; としましょう。 $\rho$ を $\tau$ の直和とし、$\bigwedge^1V, . . . ,\bigwedge^nV$ の $\mathfrak{g}\mathfrak{l}(n, k)$ の正規の表現とします。 $E_0\subset E$ を $D =\bigwedge^d(J\cap W)$ の和と、$e_{n-j+1}\wedge  \cdots  \wedge e_n$ によって$j= 1, . . . , n$ に対して生成された行とします。 (7) と補題 2 (ii) により、

$$
\mathfrak{n}=\{x\in \mathfrak{g}\mathfrak{l}(V)|\rho (x)(E_0) = 0\} \tag{8}
$$

$x\in k.1_n,\rho (x)$ が対角化可能である場合、それは明らかです。最後に、F が $\rho (\mathfrak{n}), F$ によって消滅した E の元の集合が $\rho (\mathfrak{q})$ (第 I, §3, no. 5 、提案 5) および (8) の下で安定である場合、

$$
\mathfrak{n}=\{x\in \mathfrak{g}\mathfrak{l}(V)|\rho (x)(F) = 0\} \tag{9}
$$

### 5. 特徴付け分解可能リー代数

すべての分解可能なリー代数は、半単純またはゼロポテントである元の集合によって、ベクトル空間として (およびなおさらはリー代数として) 生成されます。逆に:

#### 定理 1 {#lie-vii-s5-thm-1 .statement tag=00X1}

$\mathfrak{g}$ を $\mathfrak{g}\mathfrak{l}(V)$ の嘘部分代数とし、X を $\mathfrak{g}$ 生成する $\mathfrak{g}$ の部分集合を $k$ 上のリー代数とします。 X のすべての元が半単純または無能である場合、$\mathfrak{g}$ は分解可能です。

a$)\mathfrak{g}$ は可換です。

$\mathfrak{g}$ の半単純 (それぞれ nilpotent) 要素は、ベクトル部分空間 $\mathfrak{g}_s$ (それぞれ $\mathfrak{g}_n$) を形成します。 仮定は $\mathfrak{g}=\mathfrak{g}_s\oplus \mathfrak{g}_n$ と同等であるため、$\mathfrak{g}$ は分解可能です。

b$)\mathfrak{g}$ は還元的です。

次に、$\mathfrak{g}=\mathfrak{g}'\times \mathfrak{c}$ と $\mathfrak{g}'$ 半単純および $\mathfrak{c}$ は可換です。提案$2,\mathfrak{g}'$により、分解可能です。 $x=a+b\in \mathfrak{g}$ を $a\in \mathfrak{g}',b\in \mathfrak{c}$ にしましょう。 $a_s, a_n, b_s, b_n$ を半単純とし、$a, b$ の無能を成分とします。 $a_s, a_n, b_s, b_n$ は相互に可換であるため、$x$ の半単純とゼロポテント成分は $a_s+b_s, a_n+b_n$ です。現在$a_s, a_n\in \mathfrak{g}'$。 $x$ が半単純の場合、$x=a_s+b_s$; $a_s\in \mathfrak{g}'$ からは $b_s\in \mathfrak{g}$ なので、$b_s$ から $b_s\in \mathfrak{c}$ は $\mathfrak{g}$ と通勤します。従って、$a=a_s$ と $b=b_s$ になります。同様に、$x$ がゼロの場合、$a=a_n$ と $b=b_n$ は無力です。従って、Xの元の$\mathfrak{c}$の射影は、半単純または無能のいずれかになります。 a) により、これは $\mathfrak{c}$ が分解可能であることを意味します。前の記法を保持しますが、$x$ に仮定がなければ、現在は $b_s, b_n\in \mathfrak{c}$ なので、$a_s+b_s, a_n+b_n\in \mathfrak{g}$ となり、この場合は定理となります。

c) 一般的なケース。

定理が次元 $<$ dim $\mathfrak{g}$ のリー代数について証明されたと仮定し、$\mathfrak{g}$ について証明します。

$\mathfrak{n}$ を、$\mathfrak{g}$ の同一性表現の無能の理想である最大のとします。 $\mathfrak{n}= 0,\mathfrak{g}$ に単射詞半単純表現がある場合、還元的です。 $\mathfrak{n}\not= 0$ と仮定します。 $\mathfrak{p}$ を $\mathfrak{g}\mathfrak{l}(V)$ の $\mathfrak{n}$ のノーマライザーとします。提案 8 の $E, \rho ,F$ 満たす条件が存在します。$\mathfrak{g}\subset \mathfrak{p},\rho (\mathfrak{g})$ は F を安定したままにするので、 $\rho_0$ を F の $\mathfrak{g}$ の表現 $u \rightarrow \rho (u)|F$ とします。 $\mathfrak{n}=$ カー$\rho_0$ がいます。すべての半単純 (それぞれ無能) 元の $\rho$ の下の像は、$\mathfrak{g}\mathfrak{l}(V)$ の半単純 (それぞれ無能) です (提案 2)。従って、代数 $\rho_0(\mathfrak{g})$ は、その半単純元とその冪零元によって生成されます。 帰納法の仮定までに、$\rho_0(\mathfrak{g})$ は分解可能になります。

$x\in \mathfrak{g}$ を、$x_s, x_n$ をその半単純と無能の成分とします。提案 2 により、$\rho (x)$ の半単純と nilpotent 成分は $\rho (x_s), \rho (x_n)$ になります。 $\rho_0(\mathfrak{g})$ は分解可能であるため、次のような $y, z\in \mathfrak{g}$ が存在します。

$$
\rho_0(y) =\rho (x_s)|F, \rho_0(z) =\rho (x_n)|F
$$

そうすると、$x_s\in y+\mathfrak{n}, x_n\in z+\mathfrak{n}$なので、$x_s, x_n\in \mathfrak{g}$になります。 Q.E.D.

#### 系 1 {#lie-vii-s5-thm-1-cor-1 .statement tag=00X2}

分解可能な部分代数によって生成される$\mathfrak{g}\mathfrak{l}(V)$のすべての部分代数は分解可能です。

これは明らかです。

#### 系 2 {#lie-vii-s5-thm-1-cor-2 .statement tag=00X3}

$\mathfrak{g}$ を $\mathfrak{g}\mathfrak{l}(V)$ の嘘部分代数とします。次に、$[\mathfrak{g},\mathfrak{g}]$ は分解可能です。

$\mathfrak{r}$を$\mathfrak{g},\mathfrak{s}$の根基、$\mathfrak{g}$のレヴィ部分代数とします（I, §6, no. 8章）。それから

$$
[\mathfrak{g},\mathfrak{g}] = [\mathfrak{s},\mathfrak{s}] + [\mathfrak{s},\mathfrak{r}] + [\mathfrak{r},\mathfrak{r}] =\mathfrak{s}+ [\mathfrak{g},\mathfrak{r}]
$$

The algebra $[\mathfrak{g},\mathfrak{r}]$ is decomposable since all of its elements are nilpotent (Chap. I, §5, no. 3). 一方、$\mathfrak{s}$ は分解可能です (提案 2)。 したがって、$[\mathfrak{g},\mathfrak{g}]$ は分解可能です (Cor. 1)。

#### 系 3 {#lie-vii-s5-thm-1-cor-3 .statement tag=00X4}

$\mathfrak{g}$ を $\mathfrak{g}\mathfrak{l}(V)$ の嘘部分代数とし、X を k 上のリー代数として $\mathfrak{g}$ 生成する $\mathfrak{g}($ の部分集合とする。

(i) $\mathfrak{g}$ の分解可能包絡 $e(\mathfrak{g})$ は、 半単純と X の元の無能成分によって生成されます。

(ii) $k'$ が $k,e(\mathfrak{g}\otimes_kk') =e(\mathfrak{g})\otimes_kk'$ の拡大である場合。そして、$\mathfrak{g}\otimes_kk'$ が分解可能な場合に限り、$\mathfrak{g}$ は分解可能です。

$\widetilde{\mathfrak{g}}$ を半単純によって生成された $\mathfrak{g}\mathfrak{l}(V)$ の部分代数と、X の元の無能成分とします。次に$\mathfrak{g}\subset \widetilde{\mathfrak{g}}\subset e(\mathfrak{g})$; Th 著$1, \widetilde{\mathfrak{g}}$ は分解可能であるため、$\widetilde{\mathfrak{g}}=e(\mathfrak{g})$ となり、(i) が証明されます。 X 生成するから $k'$-代数 $\mathfrak{g}\otimes_kk'$ なので、主張 (ii) が続きます。

#### 系 4 {#lie-vii-s5-thm-1-cor-4 .statement tag=00X5}

$\mathfrak{g}$ を $\mathfrak{g}\mathfrak{l}(V)$ の分解可能な嘘部分代数とします。 $\mathscr{T}$ を集合 of 可換部分代数 of $\mathfrak{g}$ からなる of 半単純元 (cf. 提案 6)。 $\mathscr{T}$ の極大元はすべて同じ次元を持っています。

$k'$ を $k$ と $V'= V\otimes_kk',\mathfrak{g}'=$ $\mathfrak{g}\otimes_kk'$ の代数閉拡大とします。 $\mathfrak{t}_1,\mathfrak{t}_2$ を $\mathfrak{g},\mathfrak{h}'_i=\mathfrak{h}_i\otimes_kk'$ の $\mathscr{T},\mathfrak{t}'_i=\mathfrak{t}_i\otimes_kk',\mathfrak{h}_i$ の極大元と $\mathfrak{t}_i$ の交換子環とします。すると、$\mathfrak{h}_i$ は $\mathfrak{g}$ のカルタン部分代数なので (提案 6)、$\mathfrak{h}'_i$ は $\mathfrak{g}'$ のカルタン部分代数になります。次に、$\mathfrak{h}_i=\mathfrak{t}_i\times \mathfrak{n}_V(\mathfrak{h}_i)$、したがって$\mathfrak{h}'_i=\mathfrak{t}'_i\times \mathfrak{n}_{V'}(\mathfrak{h}'_i)$、つまり、$\mathfrak{t}'_i$は、半単純の集合、$\mathfrak{h}'_i$の元になります。 $\mathfrak{g}'$ は分解可能なので (Cor. $3$)$,\mathfrak{t}'_1$ と $\mathfrak{t}'_2$ は Aut$_e(\mathfrak{g}')$ の下で共役 (提案 6)、したがって dim$\mathfrak{t}_1=$ dim$\mathfrak{t}_2$ です。

#### 定理 2 {#lie-vii-s5-thm-2 .statement tag=00X6}

$\mathfrak{g}$ を $\mathfrak{g}\mathfrak{l}(V)$ の嘘部分代数とします。次の条件は同等です。

(i) $\mathfrak{g}$ は分解可能です。

(ii) $\mathfrak{g}$ のすべてのカルタン部分代数は分解可能です。

(iii) $\mathfrak{g}$ には分解可能なカルタン部分代数があります。

(iv) $\mathfrak{g}$ の根基は分解可能です。

(i) $=\Rightarrow$ (ii): これは Cor.提案 3 の 2。

(ii) $=\Rightarrow$ (i): これは Cor. Thの1 $\mathfrak{g}$ はそのカルタン部分代数 (§2, no. 3、Th. 1 の Cor. 3) によって生成されるためです。

(ii) $=\Rightarrow$ (iii): これは明らかです。

(iii) $=\Rightarrow$ (ii): Cor 著。 Thの3。 1 では、$k$ が代数的に閉じていると仮定できます。 $\mathfrak{g}$ のカルタン部分代数は、$\mathfrak{g}($§3, no. 2 の基本自己同型の下にある共役になります。 1); §3, no. 1 の注意 1 を考慮すると、これらの 1 つが分解可能であれば、それらはすべて分解可能であるということになります。

(i) $=\Rightarrow$ (iv): これは Cor.提案 4 の 2。

(iv) $=\Rightarrow$ (i): $\mathfrak{g}$ の根基 $\mathfrak{r}$ が分解可能であると仮定します。 $\mathfrak{s}$ を $\mathfrak{g}$ の Levi 部分代数とします。それは分解可能です (提案 2)。したがって、$\mathfrak{g}=\mathfrak{s}+\mathfrak{r}$ は分解可能です (Th. 1 の Cor. 1)。

### 練習問題 {#lie-vii-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
