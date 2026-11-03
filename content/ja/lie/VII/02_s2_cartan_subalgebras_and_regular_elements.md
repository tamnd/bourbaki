---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 2
section_title: Cartan subalgebras and regular elements of a Lie algebra
lang: ja
source: lie-vii-ix
book_pages: 12-20, 55-57
pdf_pages: 0022-0030, 0064-0066
extraction: native
subsections:
    - "no": 1
      title: CARTAN SUBALGEBRAS
      page: 13
      pdf_page: 23
    - "no": 2
      title: REGULAR ELEMENTS OF A LIE ALGEBRA
      page: 16
      pdf_page: 26
    - "no": 3
      title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
      page: 18
      pdf_page: 28
    - "no": 4
      title: CARTAN SUBALGEBRAS OF SEMI-SIMPLE LIE ALGEBRAS
      page: 19
      pdf_page: 29
statements: 40
exercises: 16
content_sha256: edc96079cfb99f1d237592a767de9a32bf6e227ae7866219b21881ab6a147f8f
translated_from: content/en/lie/VII/02_s2_cartan_subalgebras_and_regular_elements.md
translation_method: google
source_content_sha256: 05b31ef931fa1971af6f075dc663eed9dae014f8584d9c3690519a9cceb1ce2d
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 2f96fde0b7151c839ca85f99f051b2ba8e41cceb08d56f594886273568dde234
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。 リー代数のカルタン部分代数と正則元

no. 2 以降、体 $k$ は無限であるとみなされます。

### 1. カルタン部分代数

#### 定義 1 {#lie-vii-s2-def-1 .statement tag=00TJ}

$\mathfrak{g}$をリー代数とします。 $\mathfrak{g}$ のカルタン部分代数は、それ自体のノーマライザーと等しい $\mathfrak{g}$ の nilpotent 部分代数です。

後で次の結果が得られます。

1) $k$ が無限である場合、$\mathfrak{g}$ はカルタン部分代数 (no. 3、Th. 1 のコリント 1) になります。

2) $k$ が標数0 の場合、$\mathfrak{g}$ のすべてのカルタン部分代数は同じ次元を持ちます (§3, no. 3、Th. 2)。

3) $k$ が代数的に閉で標数 0 の場合、$\mathfrak{g}$ のすべてのカルタン部分代数は、$\mathfrak{g}($§3, no. 2 の初等自己同型の群の下で共役になります。 1)。

#### 例 1 {#lie-vii-s2-n1-exa-1 .statement tag=00TK}

$\mathfrak{g}$ が無能である場合、$\mathfrak{g}$ の唯一のカルタン部分代数は $\mathfrak{g}$ 自体です (章 I, §4, no. 1、提案 3)。

#### 例 2 {#lie-vii-s2-n1-exa-2 .statement tag=00TL}

$\mathfrak{g}=\mathfrak{g}\mathfrak{l}(n, k)$ を、$\mathfrak{h}$ を行列所属から $\mathfrak{g}$ までの対角線の集合とします。 $\mathfrak{h}$ は $\mathfrak{g}$ のカルタン部分代数であることがわかります。まず、$\mathfrak{h}$ は可換であるため、零能です。 $(E_{ij})$ を $\mathfrak{g}\mathfrak{l}(n, k)$ の標準基底とし、$x=\sum\mu_{ij}E_{ij}$ を $\mathfrak{g}$ の $\mathfrak{h}$ の正規化器の元とします。 $i\not=j$ の場合、公式章の (5) I, §1, no. 2は、$[E_{ii}, x]$の$E_{ij}$の係数が$\mu_{ij}$であることを示します。 $E_{ii}\in \mathfrak{h}$、$[E_{ii}, x]\in \mathfrak{h}$、そして問題の係数は零となります。したがって、$i\not=j$ に対して $\mu_{ij}= 0$ なので、$x\in \mathfrak{h}$ となり、$\mathfrak{h}$ は確かに $\mathfrak{g}$ のカルタン部分代数であることがわかります。

#### 例 3 {#lie-vii-s2-n1-exa-3 .statement tag=00TM}

$\mathfrak{h}$ を $\mathfrak{g}$ のカルタン部分代数とし、$\mathfrak{g}_1$ を $\mathfrak{g}$ 含む $\mathfrak{h}$ の部分代数とします。すると、$\mathfrak{h}$ は $\mathfrak{g}_1$ のカルタン部分代数になります。これはDefからすぐに続きます。 1.

#### 命題 1 {#lie-vii-s2-prop-1 .statement tag=00TN}

$\mathfrak{g}$ をリー代数とし、$\mathfrak{h}$ を $\mathfrak{g}$ のカルタン部分代数とします。この場合、$\mathfrak{h}$ は $\mathfrak{g}$ の最大ゼロポテント部分代数です。

$\mathfrak{h}'$ を $\mathfrak{g}$ 含む $\mathfrak{h}$ のゼロポテント部分代数とします。すると、$\mathfrak{h}$ は $\mathfrak{h}'$ (例 3) のカルタン部分代数なので、$\mathfrak{h}=\mathfrak{h}'$ (例 1) となります。

カルタン部分代数ではない最大零能部分代数が存在します (例題 2)。

#### 命題 2 {#lie-vii-s2-prop-2 .statement tag=00TO}

$(\mathfrak{g}_i)_{i\in I}$ をリー代数と $\mathfrak{g}=\prod_{i\in I}\mathfrak{g}_i$ の有限族とする。

$\mathfrak{g}$ のカルタン部分代数は、形 $\prod_{i\in I}\mathfrak{h}_i$ の部分代数であり、$\mathfrak{h}_i$

$\mathfrak{g}_i$のカルタン部分代数です。

$\mathfrak{h}_i$ がノーマライザー $\mathfrak{n}_i$ を使用した $\mathfrak{g}_i$ の部分代数である場合、$\prod\mathfrak{h}_i$ はノーマライザー $\prod\mathfrak{n}_i$ を使用した $\mathfrak{g}$ の部分代数です。 $\mathfrak{h}_i$ が無能である場合、$\prod\mathfrak{h}_i$ は無能です。したがって、$\mathfrak{h}_i$ が $\mathfrak{g}_i$ のカルタン部分代数である場合、すべての $i,\prod\mathfrak{h}_i$ は $\mathfrak{g}$ のカルタン部分代数になります。 逆に、$\mathfrak{h}$ を $\mathfrak{g}$ のカルタン部分代数とする。 the projection $\mathfrak{h}_i$ of $\mathfrak{h}$ onto $\mathfrak{g}_i$ is a nilpotent subalgebra of $\mathfrak{g}_i$, and $\prod\mathfrak{h}_i$ is a nilpotent subalgebra of $\mathfrak{g}$ containing $\mathfrak{h}$;したがって、$\mathfrak{h}=\prod\mathfrak{h}_i$ (提案 1)。したがって、すべての $i,\mathfrak{h}_i$ は $\mathfrak{g}_i$ における独自の正規化子であり、$\mathfrak{g}_i$ のカルタン部分代数も同様です。

#### 例 4 {#lie-vii-s2-n1-exa-4 .statement tag=00TP}

$k$ が特性である場合、$0,\mathfrak{g}\mathfrak{l}(n, k)$ は理想 $\mathfrak{s}\mathfrak{l}(n, k)$ と $k.1$ の積です。 例 2 と提案 2 から、$\mathfrak{s}\mathfrak{l}(n, k)$ のトレース 0 の対角線行列の集合は $\mathfrak{s}\mathfrak{l}(n, k)$ のカルタン部分代数であることがわかります。

#### 命題 3 {#lie-vii-s2-prop-3 .statement tag=00TQ}

$\mathfrak{g}$ をリー代数、$\mathfrak{h}$ 部分代数の $\mathfrak{g}$、$k'$ 拡大の $k$ とします。このとき、$\mathfrak{h}\otimes_kk'$ が $\mathfrak{g}\otimes_kk'$ のカルタン部分代数である場合に限り、$\mathfrak{h}$ は $\mathfrak{g}$ のカルタン部分代数になります。

Indeed, $\mathfrak{h}$ is nilpotent if and only if $\mathfrak{h}\otimes_kk'$ is (Chap. I, §4, no. 5). 一方、$\mathfrak{n}$が$\mathfrak{g}$の$\mathfrak{h}$の正規化器である場合、$\mathfrak{g}\otimes_kk'$の$\mathfrak{h}\otimes_kk'$の正規化器は$\mathfrak{n}\otimes_kk'$になります（I, §3, no. 8章）。

#### 命題 4 {#lie-vii-s2-prop-4 .statement tag=00TR}

$\mathfrak{g}$ をリー代数、$\mathfrak{h}$ を $\mathfrak{g}$ の nilpotent 部分代数とします。すると、$\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h}$の場合に限り、$\mathfrak{h}$は$\mathfrak{g}$のカルタン部分代数になります。

$\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h},\mathfrak{h}$ がそれ自体のノーマライザー (§1、提案 10 (i)) である場合、$\mathfrak{h}$ は $\mathfrak{g}$ のカルタン部分代数です。 $\mathfrak{g}^0(\mathfrak{h})\not=\mathfrak{h}$ と仮定します。 随伴物表現から商への通過によって得られた$\mathfrak{g}^0(\mathfrak{h})/\mathfrak{h}$上の$\mathfrak{h}$の表現を考えてみましょう。 By applying Engel’s theorem (Chap. I, §4, no. 2, Th. 1), we see that there exists $x\in \mathfrak{g}^0(\mathfrak{h})$ such that $x \notin \mathfrak{h}$ and $[\mathfrak{h}, x]\subset \mathfrak{h}$; then $x$ belongs to the normalizer of $\mathfrak{h}$ in $\mathfrak{g}$, so $\mathfrak{h}$ is not a Cartan subalgebra of $\mathfrak{g}$.

#### 系 1 {#lie-vii-s2-prop-4-cor-1 .statement tag=00TS}

$\mathfrak{g}$ を $\mathfrak{g}$ のリー代数、$\mathfrak{h}$ カルタン部分代数とします。 $k$ が無限である場合、$\mathfrak{h}=\mathfrak{g}^0(x)$ となるような $x\in \mathfrak{h}$ が存在します。

確かに、$\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$ であり、§1 の提案 9 (ii) を適用できます。

#### 系 2 {#lie-vii-s2-prop-4-cor-2 .statement tag=00TT}

$f:\mathfrak{g}\rightarrow \mathfrak{g}'$ をリー代数の全射準同型とします。 $\mathfrak{h}$ が $\mathfrak{g},f(\mathfrak{h})$ のカルタン部分代数である場合、$\mathfrak{g}'$ のカルタン部分代数です。

確かに、$f(\mathfrak{h})$ は $\mathfrak{g}'$ の無能な部分代数です。一方、$\mathfrak{g}'$の$\mathfrak{h}$の表現$x \rightarrow$の広告$f(x)$を考えてみましょう。 §1, no. 3、$f(\mathfrak{g}^0(\mathfrak{h})) ={\mathfrak{g}'}^0(\mathfrak{h})$ の提案 9 (iv) による。今は$\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h}$ですが、一方で${\mathfrak{g}'}^0(\mathfrak{h}) ={\mathfrak{g}'}^0(f(\mathfrak{h}))$であることは明らかです。したがって、$f(\mathfrak{h}) ={\mathfrak{g}'}^0(f(\mathfrak{h}))$ となり、提案 4 を適用すれば十分です。

#### 系 3 {#lie-vii-s2-prop-4-cor-3 .statement tag=00TU}

$\mathfrak{h}$ をリー代数 $\mathfrak{g}$ のカルタン部分代数とし、$\mathscr{C}^n\mathfrak{g}(n\geq 1)$ を $\mathfrak{g}$ の下降中心系列の項とします（第 I, §1, no. 5 章）。次に$\mathfrak{g}=\mathfrak{h}+\mathscr{C}^n\mathfrak{g}$。

実際、系 2 は、$\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$ の $\mathfrak{h}$ の像が $\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$ のカルタン部分代数であることを示しており、したがって、$\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$ はゼロポテント (例 1) であるため、$\mathfrak{g}/\mathscr{C}^n\mathfrak{g}$ に等しいことがわかります。

#### 系 4 {#lie-vii-s2-prop-4-cor-4 .statement tag=00TV}

$\mathfrak{g}$ を $\mathfrak{g}$ のリー代数、$\mathfrak{h}$ カルタン部分代数、および $\mathfrak{g}$ 含む $\mathfrak{h}$ の $\mathfrak{a}$ 部分代数とします。

(i) $\mathfrak{a}$ は、$\mathfrak{g}$ の独自のノーマライザーと等しい。

(ii) $k=\mathbf{R}$ または $\mathbf{C}$ と仮定します。 G をリー代数 $\mathfrak{g}$ を伴うリー群とし、A をリー代数 $\mathfrak{a}$ を伴う G の積分部分群とします。このとき、A は G の嘘部分群であり、G における A の正規化器の正体成分です。

$\mathfrak{n}$ を $\mathfrak{g}$ の $\mathfrak{a}$ のノーマライザーとします。 $\mathfrak{h}$ は $\mathfrak{n}$ (例 $3$) のカルタン部分代数であるため、$,\{0\}$ は $\mathfrak{n}/\mathfrak{a}$ (Cor. 2) のカルタン部分代数であるため、$\mathfrak{n}/\mathfrak{a}$ の正規化子と等しくなります。他には語、$\mathfrak{n}=\mathfrak{a}$。 主張 (ii) は (i) と第 2 章の続きです。 III, §9, no. 4、コル。提案11の。

#### 系 5 {#lie-vii-s2-prop-4-cor-5 .statement tag=00TW}

$\mathfrak{g}$ をリー代数、$\mathfrak{g}$ の E 部分集合とします。 E を随伴表現によって $\mathfrak{g}$ 上で演算するとします。すると、$E =\mathfrak{g}^0(E)$の場合に限り、Eは$\mathfrak{g}$のカルタン部分代数になります。

条件が必要です (提案 4)。ここで$E =\mathfrak{g}^0(E)$と仮定します。 §1, no. 1 の提案 2 (ii) により、E は $\mathfrak{g}$ の部分代数になります。 $x\in E$ の場合、ad$_Ex$ は $E\subset \mathfrak{g}^0(E)$ 以降無能です。したがって、代数 E は零能です。しかし、提案 4 により E はカルタン部分代数になります。

#### 系 6 {#lie-vii-s2-prop-4-cor-6 .statement tag=00TX}

$\mathfrak{g}$ をリー代数とし、$k_0$ を $[k:k_0]<+\infty$ となる $k$ の部分体とし、$\mathfrak{g}_0$ をスカラーの体を次のように制限することで $\mathfrak{g}$ から得られるリー代数とします。 $k_0$。 $\mathfrak{h}$を$\mathfrak{g}$の部分集合とします。そして、$\mathfrak{h}$が$\mathfrak{g}_0$のカルタン部分代数である場合に限り、$\mathfrak{h}$は$\mathfrak{g}$のカルタン部分代数になります。

これはコルからの続きです。 5、なぜなら、条件 $\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$ には基礎体が含まれないからです。

#### 命題 5 {#lie-vii-s2-prop-5 .statement tag=00TY}

$\mathfrak{g}$をリー代数、$\mathfrak{c}$をその中心、$\mathfrak{h}$をベクトル部分空間、$\mathfrak{g}$とします。この場合、$\mathfrak{h}$ 含む $\mathfrak{c}$ であり、$\mathfrak{h}/\mathfrak{c}$ が $\mathfrak{g}/\mathfrak{c}$ のカルタン部分代数である場合に限り、$\mathfrak{h}$ は $\mathfrak{g}$ のカルタン部分代数になります。

$\mathfrak{h}$が$\mathfrak{g}$のカルタン部分代数であると仮定します。 $[\mathfrak{c},\mathfrak{g}]\subset \mathfrak{h}$ なので、$\mathfrak{c}\subset \mathfrak{h}$ になります。一方、$\mathfrak{h}/\mathfrak{c}$はCorによる$\mathfrak{g}/\mathfrak{c}$のカルタン部分代数です。提案 4 の 2。

$\mathfrak{h}\supset \mathfrak{c}$ と $\mathfrak{h}/\mathfrak{c}$ が $\mathfrak{g}/\mathfrak{c}$ のカルタン部分代数であると仮定します。 $f$ を、$\mathfrak{g}$ から $\mathfrak{g}/\mathfrak{c}$ までの正規の射とします。 $\mathfrak{h}/\mathfrak{c}$ の中央の拡大である代数 $\mathfrak{h}$ は無能です。 $\mathfrak{n}$ を $\mathfrak{g}$ の $\mathfrak{h}$ のノーマライザーとします。 $x\in \mathfrak{n}$、$[f(x),\mathfrak{h}/\mathfrak{c}]\subset \mathfrak{h}/\mathfrak{c}$ の場合、$f(x)\in \mathfrak{h}/\mathfrak{c}$、したがって $x\in \mathfrak{h}$ となります。これは、$\mathfrak{h}$が$\mathfrak{g}$のカルタン部分代数であることを証明します。

#### 系 {#lie-vii-s2-n1-cor-1 .statement tag=00TZ}

$\mathscr{C}_{\infty}\mathfrak{g}$ を、リー代数 $\mathfrak{g}$ の上昇中心系列の和集合とします（I, §1, no. 6 章）。 $\mathfrak{g}$のカルタン部分代数は、$\mathfrak{g}/\mathscr{C}_{\infty}\mathfrak{g}$のカルタン部分代数の逆像です。

確かに、$\mathfrak{g}/\mathscr{C}_i\mathfrak{g}$ の中心は $\mathscr{C}_{i+1}\mathfrak{g}/\mathscr{C}_i\mathfrak{g}$ であり、系は提案 5 の直後に帰納法によって続きます。

#### 注意 {#lie-vii-s2-n1-rem-1 .statement tag=00U0}

$\mathscr{C}_{\infty}\mathfrak{g}$ は、$\mathfrak{g}/\mathfrak{n}$ の中心が零となるような、$\mathfrak{g}$ の最小のの理想的な$\mathfrak{n}$ です。それは$\mathfrak{g}$の特徴的で無能な理想です。

### 2. リー代数中正則元

[これ以降、$k$ は無限大であると仮定することを思い出してください。]

$\mathfrak{g}$ を次元 $n$ のリー代数とします。 $x\in \mathfrak{g}$の場合、広告$x$の特性多項式を形に書きます

det(T $-$ ad $x$) $=\sum_{i=0}^na_i(x)T^i$、$a_i(x)\in k$ 付き。

$a_i(x) = (-1)^{n-i}$Tr $(\bigwedge^{n-i}$ ad x)、cf. 代数、Chap があります。 III, §8, no. 11。これは、$x \rightarrow a_i(x)$ が $\mathfrak{g}$ から $k($代数までの次数 $n-i$ の同次多項式写像であることを示しています。 IV, §5, no. 9）。

#### 注意 1 {#lie-vii-s2-n2-rem-1 .statement tag=00U1}

(ad $x$)$(x) = 0$ 以降、すべての $x\in \mathfrak{g}$ に対して $\mathfrak{g}\not=\{0\},a_0= 0$ の場合。

#### 注意 2 {#lie-vii-s2-n2-rem-2 .statement tag=00U2}

$k'$を$k$の拡大とします。 $x'\in \mathfrak{g}\otimes_kk'$ には det(T $-$ ad $x'$) $=\sum_{i=0}^na'_i(x')T^i$ と書きます。次に、すべての $i$ に対して $a'_i|\mathfrak{g}=a_i$ です。

#### 定義 2 {#lie-vii-s2-def-2 .statement tag=00U3}

rk($\mathfrak{g}$) で示される $\mathfrak{g}$ の階数は、最小の整数 $l$ であり、$a_l\not= 0$ となります。 元 $\mathfrak{g}$ の $x$ が $a_l(x)\not= 0$ の場合はレギュラーと呼ばれます。

すべての $x\in \mathfrak{g}$、rk($\mathfrak{g}$)$\leq$ dim$\mathfrak{g}^0(x)$、および等式は、$x$ が正規である場合にのみ成立します。

正則元の集合は密集しており、$\mathfrak{g}$ではザリスキー位相（App.I）のために開いています。

#### 例 1 {#lie-vii-s2-n2-exa-1 .statement tag=00U4}

$\mathfrak{g}$ が nilpotent の場合、rk($\mathfrak{g}$) $=$ dim$\mathfrak{g}$ と $\mathfrak{g}$ のすべての元は正規です。

#### 例 2 {#lie-vii-s2-n2-exa-2 .statement tag=00U5}

$\mathfrak{g}=\mathfrak{s}\mathfrak{l}(2, k)$ にしましょう。 $x=(\gamma -\alpha )\in \mathfrak{g}$ の場合、簡単に計算すると次のようになります。

$$
\beta \gamma
$$

det(T $-$ ad $x$) $= T^3-4(\alpha \beta +\gamma^2)T$。

$k$ の特性が $\not= 2$ である場合、rk($\mathfrak{g}$) $= 1$ と正則元は、$\alpha \beta +\gamma^2\not= 0$ となるような $x$ です。

#### 例 3 {#lie-vii-s2-n2-exa-3 .statement tag=00U6}

V を有限次元 $n$ と $\mathfrak{g}=\mathfrak{g}\mathfrak{l}(V)$ のベクトル空間とします。 $\overline{k}$ を $k$ の代数閉包とします。 $x\in \mathfrak{g}$ を、$\lambda_1, . . . , \lambda_n$ を $x$ の特性多項式の $\overline{k}$ の根とします (各根は、その重複度に等しい数回書かれます)。 The canonical isomorphism from $V^*\otimes V$ to $\mathfrak{g}$ is compatible with the $\mathfrak{g}$-module structures of these two spaces, in other words it takes $1\otimes x-^tx\otimes 1$ to ad $x$ (Chap. I, §3, no. 3, Prop. 4). §1、提案 4 (i) を考慮すると、ad $x$ の特性多項式の根は、$1\leq i\leq n,1\leq j\leq n$ の $\lambda_i-\lambda_j$ であることがわかります (各根は、その重複度に等しい数回書かれます)。 したがって、$\mathfrak{g}$ の階数は $n$ であり、各 $\lambda_i$ が $x$ の特性多項式の単純な根である場合に限り、$x$ は正規です。

#### 命題 6 {#lie-vii-s2-prop-6 .statement tag=00U7}

$\mathfrak{g}$ を $k$ のリー代数、$k'$ 拡大、および $\mathfrak{g}'=$ $\mathfrak{g}\otimes_kk'$ とします。

(i) $\mathfrak{g}$ の元 $x$ は、$x\otimes 1$ が $\mathfrak{g}'$ で正規である場合にのみ、$\mathfrak{g}$ で正規です。

(ii) rk($\mathfrak{g}$) $=$ rk($\mathfrak{g}'$)。

これは注意 2 から続きます。

#### 命題 7 {#lie-vii-s2-prop-7 .statement tag=01IY}

$(\mathfrak{g}_i)_{i\in I}$ をリー代数の有限族とし、$\mathfrak{g}=$ $\prod_{i\in I}\mathfrak{g}_i$ とします。

(i) $\mathfrak{g}$ の元 $(x_i)_{i\in I}$ は、$\mathfrak{g}$ で正規であり、すべての $i\in I,x_i$ が $\mathfrak{g}_i$ で正規である場合に限ります。

(ii) rk($\mathfrak{g}$) $=\sum_{i\in I}$ rk($\mathfrak{g}_i$)。

実際、任意の $x= (x_i)_{i\in I}\in \mathfrak{g}$ について、ad$_{\mathfrak{g}}x$ の特性多項式は、ad$_{\mathfrak{g}_i}x_i$ の特性多項式の積です。

#### 命題 8 {#lie-vii-s2-prop-8 .statement tag=00U8}

$f:\mathfrak{g}\rightarrow \mathfrak{g}'$ をリー代数の全射準同型とします。

(i) $x$ が $\mathfrak{g}'$ の$\mathfrak{g},f(x)$ の正則元である場合。 $\mathfrak{g}$ の中心に Ker $f$ が含まれている場合、逆は true です。

(ii) rk($\mathfrak{g}$)$\geq$ rk($\mathfrak{g}'$)。

rk($\mathfrak{g}$) $=r$、rk($\mathfrak{g}'$) $=r'$ と入れます。 $x\in \mathfrak{g}$ にしましょう。 ad $x$、ad $f(x)$、ad $x|$Ker $f$ の固有多項式は形です。

$$
P(T) = T^n+a_{n-1}(x)T^{n-1}+\cdots +a_r(x)T^r
$$

$$
Q(T) = T^{n'}+b_{n'-1}(x)T^{n'-1}+\cdots +b_{r'}(x)T^{r'}
$$

$$
R(T) = T^{n''}+c_{n''-1}(x)T^{n''-1}+\cdots +c_{r''}(x)T^{r''}
$$

ここで、$a_i, b_i, c_i$ は $\mathfrak{g}$ の多項式関数であり、$a_r\not= 0, b_{r'}\not= 0, c_{r''}\not= 0$ です。 P = QR なので、$r=r'+r''$ と $a_r(x) =b_{r'}(x)c_{r''}(x)$ が得られ、(ii) と (i) の最初の主張が証明されます。 Ker $f$ が $\mathfrak{g}$、$R(T) = T^{n''}$ の中心に含まれている場合、$a_r(x) =b_{r'}(x)$ となるため、(i) の 2 番目の主張になります。

#### 系 {#lie-vii-s2-n2-cor-1 .statement tag=00U9}

$\mathscr{C}_n\mathfrak{g}(n\geq 0)$を$\mathfrak{g}$の上昇中心系列の項とします（I, §1, no. 6章）。 $\mathfrak{g}$の正則元は、$\mathfrak{g}/\mathscr{C}_n\mathfrak{g}$の像が正規のものです。

#### 命題 9 {#lie-vii-s2-prop-9 .statement tag=00UA}

$\mathfrak{g}$ を $\mathfrak{g}$ のリー代数、$\mathfrak{g}'$ 部分代数とします。 $\mathfrak{g}$ の$\mathfrak{g}'$ のすべての元は、$\mathfrak{g}'$ の正規です。

$x\in \mathfrak{g}'$ の場合、広告$_{\mathfrak{g}}x$ から $\mathfrak{g}'$ の制限は広告$_{\mathfrak{g}'}x$ であるため、商への通過により、ベクトル空間 $\mathfrak{g}/\mathfrak{g}'$ の定義する自己準同型 $u(x)$ になります。 $d_0(x)$ (それぞれ $d_1(x)$) を広告$_{\mathfrak{g}'}(x)$ (それぞれ $u(x)$) のゼロスペースの次元とし、$c_0$ (それぞれ $c_1$) を $d_0(x)$ (それぞれ $d_1(x)$) の最小値とします。 $x$ 属するから $\mathfrak{g}'$ まで。 次のような $\mathfrak{g}'$ から $k$ までの非ゼロ多項式写像 $p_0, p_1$ が存在します。

$$
d_0(x) =c_0\Leftarrow \Rightarrow p_0(x)\not= 0,d_1(x) =c_1\Leftarrow \Rightarrow p_1(x)\not= 0
$$

$k$ は無限であるため、$d_0(x) =c_0$ と $d_1(x) =c_1$ が空でないように、$x\in \mathfrak{g}'$ の集合 S は空ではありません。 $\mathfrak{g}'$ では S のすべての元が定期的に発生します。一方、S は $\mathfrak{g}'$ の元のうち集合であり、ad$_{\mathfrak{g}}x$ の nilspace は最小値次元を持つため、$\mathfrak{g}$ では $\mathfrak{g}'$ の元ごとに含むになります。

#### 注意 3 {#lie-vii-s2-n2-rem-3 .statement tag=00UB}

$\mathfrak{g}$ の$\mathfrak{g}'$ の元は必ずしも存在するとは限りません。少なくとも 1 つが存在する場合、これら元のうち集合は、正確に上記証明の S で示される集合になります。

### 3. カルタン部分代数と正則元

#### 定理 1 {#lie-vii-s2-thm-1 .statement tag=00UC}

$\mathfrak{g}$をリー代数とします。

(i) $x$ が $\mathfrak{g},\mathfrak{g}^0(x)$ の正則元である場合、$\mathfrak{g}$ のカルタン部分代数です。

(ii) $\mathfrak{h}$ が $\mathfrak{g}$ の最大零能部分代数であり、$x\in \mathfrak{h}$ が $\mathfrak{g}$ で正規である場合、$\mathfrak{h}=\mathfrak{g}^0(x)$ です。

(iii) $\mathfrak{h}$ が $\mathfrak{g}$ のカルタン部分代数である場合、dim($\mathfrak{h}$)$\geq$ rk($\mathfrak{g}$)。

(iv) 次元 rk($\mathfrak{g}$) の $\mathfrak{g}$ のカルタン部分代数は $\mathfrak{g}^0(x)$ で、$x$ は正則元です。

$x$ を $\mathfrak{g}$ の正則元とし、$\mathfrak{h}=\mathfrak{g}^0(x)$ とします。明らかに$\mathfrak{h}^0(x) =\mathfrak{h}$。 $x$ は $\mathfrak{h}$ で正則なので (提案 9)、rk($\mathfrak{h}$) $=$ dim($\mathfrak{h}$) であるため、$\mathfrak{h}$ は零能です。一方、$\mathfrak{h}=\mathfrak{g}^0(x)\supset \mathfrak{g}^0(\mathfrak{h})\supset \mathfrak{h}$なので、$\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h})$は$\mathfrak{g}$のカルタン部分代数になります（提案4）。これは(i)を証明します。

$\mathfrak{h}$ が $\mathfrak{g}$ の最大の零能部分代数であり、$x\in \mathfrak{h}$ が $\mathfrak{g}$ で正規である場合、$\mathfrak{h}\subset \mathfrak{g}^0(x)$ と $\mathfrak{g}^0(x)$ は (i) により零能であるため、$\mathfrak{h}=\mathfrak{g}^0(x)$ となり、(ii) が証明されます。

$\mathfrak{h}$ が $\mathfrak{g}$ のカルタン部分代数である場合、$\mathfrak{h}=\mathfrak{g}^0(x)$ (提案 4 の Cor. 1) となるような $x\in \mathfrak{h}$ が存在するため、dim($\mathfrak{h}$)$\geq$ rk($\mathfrak{g}$) となり、(iii) が証明されます。 加法 dim($\mathfrak{h}$) $=$ rk($\mathfrak{g}$)$,x$ の場合は通常です。最後に、$x'$ が $\mathfrak{g},\mathfrak{g}^0(x')$ で正規である場合、(i) によりカルタン部分代数となり、明らかに次元 rk($\mathfrak{g}$) になります。これは(iv)を証明する。

§3、Th でわかります。 2、$k$ が標数0 の場合、$\mathfrak{g}$ のすべてのカルタン部分代数は次元 rk($\mathfrak{g}$) を持ちます。

#### 系 1 {#lie-vii-s2-thm-1-cor-1 .statement tag=00UD}

すべてのリー代数 $\mathfrak{g}$ にはカルタン部分代数があり、$\mathfrak{g}$ の階数はカルタン部分代数の最小の次元です。

#### 系 2 {#lie-vii-s2-thm-1-cor-2 .statement tag=00UE}

$f:\mathfrak{g}\rightarrow \mathfrak{g}'$をリー代数の全射準同型とします。 $\mathfrak{h}'$が$\mathfrak{g}'$のカルタン部分代数である場合、$\mathfrak{h}'=f(\mathfrak{h})$となる$\mathfrak{g}$のカルタン部分代数$\mathfrak{h}$が存在します。

$\mathfrak{a}=f^{-1}(\mathfrak{h}')$ にしましょう。コル著$1,\mathfrak{a}$ にはカルタン部分代数 $\mathfrak{h}$ があります。コル著提案$4,f(\mathfrak{h}) =\mathfrak{h}'$の2。 $\mathfrak{h}$ は $\mathfrak{g}$ のカルタン部分代数であることがわかります。 $\mathfrak{n}$ を $\mathfrak{g}$ の $\mathfrak{h}$ のノーマライザーとします。 $\mathfrak{h}=\mathfrak{n}$ を証明できれば十分です。 $x\in \mathfrak{n},f(x)$ 属するを $\mathfrak{g}'$ の $\mathfrak{h}'$ のノーマライザーにすると、$f(x)\in \mathfrak{h}'$ と $x\in \mathfrak{a}$ になります。ただし、$\mathfrak{h}$ は $\mathfrak{a}$ の独自のノーマライザーであるため、$x\in \mathfrak{h}$ になります。

#### 系 3 {#lie-vii-s2-thm-1-cor-3 .statement tag=00UF}

すべてのリー代数 $\mathfrak{g}$ は、そのカルタン部分代数の和です。

和 $\mathfrak{s}$ のカルタン部分代数の $\mathfrak{g}$ 含む集合の正則元の $\mathfrak{g}$ (Th. 1 (i))。この集合はザリスキー位相の$\mathfrak{g}$に密なので、$\mathfrak{s}=\mathfrak{g}$。

#### 命題 10 {#lie-vii-s2-prop-10 .statement tag=00UG}

$\mathfrak{g}$を$\mathfrak{g}$のリー代数、$\mathfrak{a}$可換部分代数、$\mathfrak{g}$の$\mathfrak{a}$の$\mathfrak{c}$交換子環とします。 ad$_{\mathfrak{g}}x$ がすべての $x\in \mathfrak{a}$ に対して半単純であると仮定します。すると、$\mathfrak{c}$のカルタン部分代数は、$\mathfrak{g}$含む$\mathfrak{a}$のカルタン部分代数になります。

$\mathfrak{h}$を$\mathfrak{c}$のカルタン部分代数とします。 $\mathfrak{a}$は$\mathfrak{c},\mathfrak{a}\subset \mathfrak{z}\subset \mathfrak{h}$の中心$\mathfrak{z}$に含まれるので（案5）。 $\mathfrak{n}$ を $\mathfrak{g}$ の $\mathfrak{h}$ のノーマライザーとします。それから

$$
[\mathfrak{a},\mathfrak{n}]\subset [\mathfrak{h},\mathfrak{n}]\subset \mathfrak{h}
$$

広告$_{\mathfrak{g}}x,x\in \mathfrak{a}$ は半単純で相互に通勤しているので、代数章の続きになります。 VIII, §5, no. 1、ad$_{\mathfrak{g}}\mathfrak{a}$ の下で安定した $\mathfrak{n}$ のベクトル部分空間 $\mathfrak{d}$ が存在し、そのような $\mathfrak{n}=\mathfrak{h}\oplus \mathfrak{d}$ が存在します。そうすると、$[\mathfrak{a},\mathfrak{d}]\subset \mathfrak{h}\cap \mathfrak{d}= 0$なので、$\mathfrak{d}\subset \mathfrak{c}$になります。したがって、$\mathfrak{n}$ は $\mathfrak{c}$ の $\mathfrak{h}$ のノーマライザーであり、したがって $\mathfrak{n}=\mathfrak{h}$ となるため、$\mathfrak{h}$ は $\mathfrak{g}$ 含む $\mathfrak{a}$ のカルタン部分代数になります。

逆に、$\mathfrak{h}$ を $\mathfrak{g}$ 含む $\mathfrak{a}$ のカルタン部分代数とします。それから$\mathfrak{h}=$ $\mathfrak{g}^0(\mathfrak{h})\subset \mathfrak{g}^0(\mathfrak{a})$、そして仮定 $\mathfrak{g}_0(\mathfrak{a}) =\mathfrak{g}^0(\mathfrak{a}) =\mathfrak{c}$までに。したがって、$\mathfrak{a}\subset \mathfrak{h}\subset \mathfrak{c}$ と $\mathfrak{h}$ は $\mathfrak{c}$ のカルタン部分代数です ($\mathfrak{g}$ では独自のノーマライザーと等しいため、$\mathfrak{c}$ ではなおさらとなります)。

#### 命題 11 {#lie-vii-s2-prop-11 .statement tag=00UH}

$\mathfrak{n}$ をリー代数 $\mathfrak{g}$ の nilpotent 部分代数とします。 $\mathfrak{g}^0(\mathfrak{n})$に含まれる$\mathfrak{g}$のカルタン部分代数が存在します。

$\mathfrak{a}=\mathfrak{g}^0(\mathfrak{n})$を入れてください。 次に、$\mathfrak{n}$ はゼロであるため、$\mathfrak{n}\subset \mathfrak{a}$ になります。 $x\in \mathfrak{a}$ の場合、$P(x)$ を広告 $x$ で定義された $\mathfrak{g}/\mathfrak{a}$ の行列式の自己準同型とします。 $\mathfrak{a}'$ は、$P(x)\not= 0$ となるような $x\in \mathfrak{a}$ の集合を表します。これは、ザリスキートポロジーにおける $\mathfrak{a}$ の開いた部分集合です。関係 $x\in \mathfrak{a}'$ と $\mathfrak{g}^0(x)\subset \mathfrak{a}$ は同等です。 §1, no. 2 の提案 7 (ii) により、$\mathfrak{g}^0(y) =\mathfrak{a}$ および $y\in \mathfrak{a}'$ となるような $y\in \mathfrak{n}$ が存在するため、$\mathfrak{a}'$ は空ではありません。 $\mathfrak{a}'$ が開いているため、$\mathfrak{a}$ の正則元の集合を含むその共通部分は空ではありません。 $x$をこの共通部分の元とします。 この場合、$\mathfrak{g}^0(x)\subset \mathfrak{a}$ と $\mathfrak{g}^0(x)$ は $\mathfrak{a}$ のカルタン部分代数であるため、零能です。 一方、§1, no. 3 の提案 10 (i) は、$\mathfrak{g}^0(x)$ が $\mathfrak{g}$ における独自のノーマライザーであることを示しています。したがって、$\mathfrak{g}$ のカルタン部分代数となり、証明が完成します。

### 4. 半単純リー代数中カルタン部分代数

#### 定理 2 {#lie-vii-s2-thm-2 .statement tag=00UI}

$k$ が特性 0 であると仮定します。 $\mathfrak{g}$ を $\mathfrak{g}$ の半単純リー代数、$\mathfrak{h}$ カルタン部分代数とします。 この場合、$\mathfrak{h}$ は可換であり、その元はすべて $\mathfrak{g}$ の半単純になります (I, §6, no. 3 章、定義 3)。

$\mathfrak{h}=\mathfrak{g}^0(\mathfrak{h}),\mathfrak{h}$ は還元的であるため (§1、提案 11)、それは零能であるため可換です。一方、$\mathfrak{g}$から$\mathfrak{h}$の随伴表現の制限は半単純（前掲）なので、$\mathfrak{h}$の元は$\mathfrak{g}$では半単純になります（代数、第2章、第1章）。 VIII, §5, no. 1）。

#### 系 1 {#lie-vii-s2-thm-2-cor-1 .statement tag=00UJ}

$x\in \mathfrak{h}$ と $y\in \mathfrak{g}^{\lambda}(\mathfrak{h})$ の場合、$[x, y] =\lambda (x)y$ になります。

確かに、広告 $x$ は半単純なので、$\mathfrak{g}^{\lambda(x)}(x) =\mathfrak{g}_{\lambda(x)}(x)$ です。

#### 系 2 {#lie-vii-s2-thm-2-cor-2 .statement tag=00UK}

$\mathfrak{g}$ のすべての正則元は半単純です。

確かに、そのような元属するからカルタン部分代数 (no. 3、Th. 1 (i))。

#### 系 3 {#lie-vii-s2-thm-2-cor-3 .statement tag=00UL}

$\mathfrak{h}$ を還元的リー代数 $\mathfrak{g}$ のカルタン部分代数とします。

a$)\mathfrak{h}$ は可換です。

b) $\rho$ が有限次元 $\mathfrak{g}$ の半単純表現である場合、$\rho (\mathfrak{h})$ の元は半単純です。

$\mathfrak{c}$ を $\mathfrak{g}$ の中心とし、その派生代数を $\mathfrak{s}$ とします。すると、$\mathfrak{g}=\mathfrak{c}\times \mathfrak{s}$、つまり$\mathfrak{h}=\mathfrak{c}\times \mathfrak{h}'$となり、$\mathfrak{h}'$は$\mathfrak{s}$のカルタン部分代数になります（提案2）。 Thの観点から、 $2,\mathfrak{h}'$ は可換であるため、$\mathfrak{h}$ も可換です。さらに、$\rho (\mathfrak{h}')$ は半単純元で構成され、$\rho (\mathfrak{c})$ も同様です (第 4 章、I, §6, no. 5)。 主張 b) が続きます。

### 練習問題 {#lie-vii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
