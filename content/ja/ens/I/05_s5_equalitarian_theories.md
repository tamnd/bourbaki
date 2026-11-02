---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 5
section_title: Equalitarian theories
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 44-49, 59-60
pdf_pages: 0051-0056, 0066-0067
extraction: ocr
subsections:
    - "no": 1
      title: THE AXIOMS
      page: 44
      pdf_page: 51
    - "no": 2
      title: PROPERTIES OF EQUALITY
      page: 45
      pdf_page: 52
    - "no": 3
      title: FUNCTIONAL RELATIONS
      page: 47
      pdf_page: 54
statements: 3
exercises: 7
content_sha256: bee03181ba120919dd4ae71dbeeff7ba79d676886e160e862dbab5c0fe5a324c
translated_from: content/en/ens/I/05_s5_equalitarian_theories.md
translation_method: google
source_content_sha256: 8cbe15ed2020b27b62da706075017d090591d51c972f6b3ce0f6ebf686257ba1
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: bca82c1b6e34f280da15e58afcb0ce329f4f8fd99e59db48a030e1d49e3f5b08
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 5. 平等主義理論

### 1. 公理

*平等主義理論* は理論 $\mathscr{T}$ で、重み 2 の関係記号を持ち、$=$ (「等しい」と読む) と書き、スキーム S1 から S5 (§§3 および 4) と以下のスキーム S6 および S7 が暗黙の公理を提供します。 $T$ と $U$ が $\mathscr{T}$ の項である場合、アセンブリ $= TU$ は CF4 により $\mathscr{T}$ の関係 (等式* の *関係と呼ばれます) になります。実際には、$T = U$ または $(T) = (U)$ で表されます。

S6. *$x$を文字、$T$と$U$を$\mathscr{T}$の項、$R\{x\}$を$\mathscr{T}$の関係とする。その場合、関係 $(T = U) \Rightarrow (R\{T\} \Leftrightarrow R\{U\})$ は公理です。*

S7. *$R$と$S$が$\mathscr{T}$の関係で、$x$が文字の場合、関係$((\forall x)(R \Leftrightarrow S)) \Rightarrow (\tau_x(R) = \tau_x(S))$は公理です。

ルール S6 がスキームであることを示すために、$A$ を適用 S6 によって得られる $\mathscr{T}$ の公理とします。次に、$\mathscr{T}$には関係$R$、$\mathscr{T}$には項$T$、$U$があり、文字$x$があり、$A$は$(T = U) \Rightarrow ((T|x)R \Leftrightarrow (U|x)R)$になります。 $y$ が文字で、$\mathscr{T}$ の $V$ 項の場合、適用 S6 によって関係 $(V|x)A$ が得られることを示します。 CS1 (§1, no. 2) により、$x$ は $y$ とは異なり、$V$ には現れないと仮定できます。 $T'$、$U'$、$R'$ がそれぞれアセンブリ $(V|y)T$、$(V|y)U$、$(V|y)R$ を表すものとします。 CS2 と CS5 (§1, no. 2) では、$(V|y)A$ は

$$(T' = U') \Rightarrow ((T'|x')R' \Leftrightarrow (U'|x')R')$$

そして証明が完成しました。 S7 がスキームであるという検証も同様です。

直感的には、スキーム S6 は、2 つのオブジェクトが等しい場合、それらは同じプロパティを持つことを意味します。スキーム S7 は日常の直観からはさらに遠いものです。これは、オブジェクト $x$ の 2 つのプロパティ $R$ と $S$ が等しい場合、区別されるオブジェクト $\tau_x(R)$ と $\tau_x(S)$ (そのようなオブジェクトの場合、満たす $R$ と満たす $S$ のオブジェクトからそれぞれ選択される) を意味します。存在します）は等しいです。読者は、S7 に量指定子 $\forall x$ が存在することが不可欠であることに気づくでしょう (cf. 練習問題 7)。

関係 $= TU$ の否定は、$T \neq U$ または $(T) \neq (U)$ で表されます (記号 $\neq$ は「とは異なります」と読み取られます)。

¶ S6 から次の基準を導き出します。

C43. ※$x$を文字、$T$と$U$を$\mathscr{T}$の項、$R\{x\}$を$\mathscr{T}$の関係とします。それでは関係*

$$(T = U \text{ and } R\{T\}), \qquad (T = U \text{ and } R\{U\})$$

*は同等です。*

なぜなら、仮説 $T = U$ と $R\{T\}$ が隣接する場合、S6 までに $R\{U\}$ が真となるからです。したがって、$(T = U$ と $R\{U\})$ は true です。

形 $T = U$ の関係が理論 $\mathscr{T}$ で証明されると、$T$ と $U$ は「同じ」または「同一」であると（言葉の乱用によって）よく言われます。同様に、$\mathscr{T}$で$T \neq U$が真である場合、$T$は$U$とは異なるというというの代わりに、$T$と$U$は「別個である」と言います。

### 2. 等式の性質

これからは平等主義理論だけを考えていきます。 $\mathscr{T}$ をそのような理論とし、$\mathscr{T}_0$ を理論とし、その符号は $\mathscr{T}$ の符号であり、その唯一の公理はスキーム S1 から S7 によって提供されるものです。 理論 $\mathscr{T}_0$ は $\mathscr{T}$ (§2, no. 4) より弱く、定数がありません。次の3つの定理は$\mathscr{T}_0$の定理です。

#### 定理 1 {#ens-i-s5-thm-1 .statement tag=03P3}

$x = x$。

$S$ が $\mathscr{T}_0$ の関係 $x = x$ を表すものとします。 C27 (§4, no. 1) により、$\mathscr{T}_0$ の各関係 $R$ に対して、$(\forall x)(R \Leftrightarrow R)$ は $\mathscr{T}_0$ の定理となるため、S7 により、$\tau_x(R) = \tau_x(R)$、つまり $(\tau_x(R)|x)S$ は定理となります。 $\mathscr{T}_0$に。 $R$ を「$S$ ではない」関係とし、C26 (§4, no. 1) を考慮すると、$(\forall x)S$ は $\mathscr{T}_0$ の定理であることがわかります。したがって、C30 (§4, no. 3) により、$S$ は $\mathscr{T}_0$ の定理になります。

関係 $(\forall x)(x = x)$ は $\mathscr{T}_0$ の定理でもあります。そして、$T$ が $\mathscr{T}_0$ の項である場合、$T = T$ は $\mathscr{T}_0$ (cf. §4, no. 3) の定理です。 変換後に定理を同じ方法で文字が出現しない定理またはメタ数学的基準に入力することも可能です。今後、これらの変換を明示的に実行することはありませんが、暗黙的に使用することがよくあります。

#### 定理 2 {#ens-i-s5-thm-2 .statement tag=03P4}

$(x = y) \Leftrightarrow (y = x)$。

関係 $x = y$ が true であると仮定します。 S6 により、関係

$$(x = y) \Rightarrow ((x|y)(y = x) \Leftrightarrow (y|y)(y = x)),$$

つまり

$$(x = y) \Rightarrow ((x = x) \Leftrightarrow (y = x)),$$

それは本当です。したがって、$(x = x) \Leftrightarrow (y = x)$ は true です。 定理 1 により、$y = x$ が真となり、定理が証明されます。

#### 定理 3 {#ens-i-s5-thm-3 .statement tag=03P5}

$((x = y) \text{ and } (y = z)) \Rightarrow (x = z)$。

仮説 $x = y$、$y = z$ を $\mathscr{T}_0$ の公理に隣接させてみましょう。 S6 までに関係 $(x = y) \Rightarrow ((x = z) \Leftrightarrow (y = z))$ は true です。従って、

$$(x = z) \Leftrightarrow (y = z),$$

従って、$x = z$ は true になります。

C44。 ※$x$を文字とし、$T$、$U$、$V\{x\}$を$\mathscr{T}_0$の項とします。すると、関係 $(T = U) \Rightarrow (V\{T\} = V\{U\})$ は $\mathscr{T}_0$ の定理になります。*

$y$ と $z$ を、$x$ や $T$、$U$、$V$ に現れる文字とは異なる 2 つの異なる文字としましょう。 仮定 $y = z$ に隣接します。そして、S6までに、

$$((Y|z)(V\{y\} = V\{z\})) \Leftrightarrow (V\{y\} = V\{z\}),$$

つまり、$(V\{y\} = V\{y\}) \Leftrightarrow (V\{y\} = V\{z\})$ は true です。さて、$V\{y\} = V\{y\}$ は定理 1 までに true になります。従って、$V\{y\} = V\{z\}$ は true です。

これらすべてから、$(y = z) \Rightarrow (V\{y\} = V\{z\})$ は $\mathscr{T}_0$ の定理である、つまり $A$ であることがわかります。でも$(T|y)(U|z)A$はまさに

$$(T = U) \Rightarrow (V\{T\} = V\{U\}).$$

¶ 形 $T = U$ の関係 ($T$ と $U$ が $\mathscr{T}$ の項である) は *方程式* と呼ばれます。 関係 $T = U$ の *解* ($\mathscr{T}$) は、$x$ という文字の中の方程式として考慮され、$\mathscr{T}$ では (§2, no. 2) 項 $V$ となり、$T\{V\} = U\{V\}$ は次のようになります。 $\mathscr{T}$の定理。

¶ $T$ と $U$ を $\mathscr{T}$ の 2 つの項とし、$x_1$、$x_2$、...、$x_n$ を、$T$ には現れるが、$U$ には現れない文字とします。 関係の場合

$$(\exists x_1)\ldots(\exists x_n)(T = U)$$

が $\mathscr{T}$ の定理である場合、*U は形* $T$ ($\mathscr{T}$) に入れることができると言います。 $R$ を $\mathscr{T}$ の関係とし、$y$ を文字とします。 $V$ を $R$ の解 ($\mathscr{T}$) とし、$y$ では関係とみなします。 $y$ の関係とみなされる、$R$ のすべての解 ($\mathscr{T}$ の) が形 $V$ に収まる場合、$V$ は *完全な解* (または *一般) であると言われます。 $R$ ($\mathscr{T}$) の解*)。

### 3. 機能的関係

$R$ をアセンブリ、$x$ を文字としましょう。 $y$ と $z$ を、$x$ とは異なり、$R$ には現れない別個の文字とする。 $y'$、$z'$ を同じ特性を持つ 2 つの他の文字としましょう。 CS8、CS9 (§4, no. 1)、CS2、CS5 (§1, no. 2)、および CS6 (§3, no. 4) ごとに、アセンブリ

$$(\forall y)(\forall z)(((y|x)R \text{ and } (z|x)R) \Rightarrow (y = z))$$

そして

$$(\forall y')(\forall z')(((y'|x)R \text{ and } (z'|x)R) \Rightarrow (y' = z'))$$

は同一です。 $R$ が $\mathscr{T}$ の関係である場合、このように定義されたアセンブリは $\mathscr{T}$ の関係であり、これは「$R$ となる $x$ が最大 1 つ存在する」で示されます。この関係には文字$x$が現れません。 この関係が$\mathscr{T}$の定理であるとき、$R$は$\mathscr{T}$の$X$で*単一値*であると言われます。 To prove that $R$ is single-valued in the theory $\mathscr{T}$, it is enough to prove $y = z$ in the theory obtained by adjoining to $\mathscr{T}$ the axioms $(y|x)R$ and $(z|x)R$, where $y$ and $z$ are distinct letters which are distinct from $x$ and appear neither in $R$ nor in the explicit axioms of $\mathscr{T}$.

C45。 ※$R$は$\mathscr{T}$の関係、$x$は$\mathscr{T}$の定数ではない文字とします。 $\mathscr{T}$ の $x$ で $R$ が単一値である場合、$R \Rightarrow (x = \tau_x(R))$ は $\mathscr{T}$ の定理になります。逆に、$\mathscr{T}$ の項 $T$ が、含む $x$ ではなく、$R \Rightarrow (x = T)$ が $\mathscr{T}$ の定理である場合、$R$ は、$x$ で単一値になります。 $\mathscr{T}$.*

$\mathscr{T}$ の $x$ で $R$ が単一値であると仮定し、次のことを示しましょう

$$R \Rightarrow (x = \tau_x(R))$$

$\mathscr{T}$の定理です。 仮定 $R$ と隣接します。すると、S5 までに $(\tau_x(R)|x)R$ が真になり、したがって「$R$ と $(\tau_x(R)|x)R$」が真になります。さて、$x$ では $R$ が単一値であるため、

$$(R \text{ and } (\tau_x(R)|x)R) \Rightarrow (x = \tau_x(R))$$

C30 (§4, no. 3) による $\mathscr{T}$ の定理です。したがって、$x = \tau_x(R)$ は真です。

¶ 逆に、$R \Rightarrow (x = T)$が$\mathscr{T}$の定理だったとします。 $y$、$z$ を、$x$ とは異なり、$R$ にも$\mathscr{T}$ の明示的な公理にも現れない別個の文字とする。 $x$は$\mathscr{T}$の定数ではなく、$T$には現れないので、関係

$$(y|x)R \Rightarrow (y = T), \qquad (z|x)R \Rightarrow (z = T)$$

$\mathscr{T}$の定理です。仮説$(y|x)R$と$(z|x)R$を隣接させます。この場合、$y = T$ と $z = T$ は true であるため、$y = z$ は true になります。

¶ $R$ を $\mathscr{T}$ の関係とします。 関係

$$\text{“}(\exists x)R \text{ and there exists at most one } x \text{ such that } R\text{”}$$

は、「$R$ となる $x$ が 1 つだけ存在する」で表されます。この関係が $\mathscr{T}$ の定理である場合、$R$ は理論 $\mathscr{T}$ の * $x$ の * 関数関係であると言われます。

C46。 ※$R$は$\mathscr{T}$の関係、$x$は$\mathscr{T}$の定数ではない文字とします。 $R$ が $\mathscr{T}$ の $x$ で機能する場合、$R \Leftrightarrow (x = \tau_x(R))$ は $\mathscr{T}$ の定理になります。逆に、含む $x$ に該当しない $\mathscr{T}$ の一部の項 $T$ については、*

$$R \Leftrightarrow (X = T)$$

*は $\mathscr{T}$ の定理である場合、$R$ は $\mathscr{T}$ の $x$ で機能します。*

$R$ が $\mathscr{T}$ の $x$ で機能するとします。すると、$R \Rightarrow (x = \tau_x(R))$はC45による$\mathscr{T}$の定理になります。一方、$(\exists x)R$は$T$の定理です。 S6 関係より

$$(x = \tau_x(R)) \Rightarrow (R \Leftrightarrow (\exists x)R)$$

$\mathscr{T}$の定理です。 仮定 $x = \tau_x(R)$ に隣接すると、$R$ が真になります。したがって、$(x = \tau_x(R)) \Rightarrow R$は$\mathscr{T}$では定理となります。

¶ 逆に、$R \Leftrightarrow (x = T)$ が $\mathscr{T}$ の定理である場合、C45 により、$R$ は $\mathscr{T}$ の $x$ で単一値になります。さらに、$(T|x)R \Leftrightarrow (T = T)$は$\mathscr{T}$では定理です。したがって、$(T|x)R$、したがって$(\exists x)R$は、$\mathscr{T}$では定理になります。

¶ 関係 $R$ が T の $x$ で機能する場合、$R$ は関係 $x = \tau_x(R)$ と同等となり、多くの場合、より管理しやすくなります。一般に、項 $\tau_x(R)$ を表すために省略記号 $\Sigma$ が導入されます。このようなシンボルを、$\mathscr{T}$では*機能シンボル*と呼びます。

直観的には、$\Sigma$ は、$R$ によって定義された性質を持つ固有のオブジェクトを表します。 \* たとえば、理論では、「$y$ は実数 $\geqslant 0$」は定理、関係 「$x$ は実数 $\geqslant 0$ および $y = x^2$」は $x$ で機能します。 対応する機能記号は、$\sqrt{y}$ または $y^{1/2}$ のいずれかとみなされます。 \*

C47。 ※$x$を$\mathscr{T}$の定数ではない文字とし、$R\{x\}$と$S\{x\}$を$\mathscr{T}$の2つの関係とします。 $R\{x\}$ が $\mathscr{T}$ の $x$ で機能する場合、関係 $S\{\tau_x(R)\}$ は $(\exists x)(R\{x\}$ および $S\{x\})$ と同等です。*

なぜなら、C46 と C43 から、$(R\{x\}$ と $S\{x\})$ は $(R\{x\}$ と $S\{\tau_x(R)\})$ と同等であることがわかります。 $S\{\tau_x(R)\}$ は含む $x$ ではないので、

$$(\exists x)(R\{x\} \ \text{ and } \ S\{\tau_x(R)\})$$

C33 (§ 4, no. 3) による $(S\{\tau_x(R)\}$ および $(\exists x)R)$ に相当します。そして、$R$ は $x$ で機能するため、$(\exists x)R$ が真であるという事実から結果が得られます。

### 練習問題 {#ens-i-s5-exercises}

*合計練習問題 for* § 5、$\mathscr{T}$ *は平等主義者理論を表します。

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
