---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 4
section_title: Natural integers. Finite sets
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 166-171, 230-234
pdf_pages: 0172-0177, 0236-0240
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF INTEGERS
      page: 166
      pdf_page: 172
    - "no": 2
      title: INEQUALITIES BETWEEN INTEGERS
      page: 166
      pdf_page: 172
    - "no": 3
      title: THE PRINCIPLE OF INDUCTION
      page: 168
      pdf_page: 174
    - "no": 4
      title: FINITE SUBSETS OF ORDERED SETS
      page: 170
      pdf_page: 176
    - "no": 5
      title: PROPERTIES OF FINITE CHARACTER
      page: 170
      pdf_page: 176
statements: 15
exercises: 11
content_sha256: a2c276dacfe451c5c560dd852746deed76d85c8ddacedf24738ae4f1faf2ea51
translated_from: content/en/ens/III/04_s4_natural_integers_finite_sets.md
translation_method: google
source_content_sha256: b07b7ce28c5ec4cebf51e51a369145ff5f0d99cab971bd69c71b3b417b968e57
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: c319adf515ed73f19f166854c990cd51861b4bed8a34bdc96d8be0613fa23691
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 4. ナチュラル整数。有限集合

### 1. 定義/整数

#### 定義 1 {#ens-iii-s4-def-1 .statement tag=03R9}

*基数 $\alpha$ は、$\alpha \ne \alpha + 1$ であれば有限であると言われます。有限基数は、自然整数 (または、混乱の危険がない場合 [^1] であれば、単に整数) とも呼ばれます。 $\operatorname{Card}(E)$ が有限基数である場合、集合 $E$ は有限であると言われます。そして、$\operatorname{Card}(E)$ は、$E$ の元の数と呼ばれます。

家族 (章 II, § 3, no. 4) は、添字集合が有限であれば *有限* であると言われます。

*ある型の対象の数が整数$m$であると言うとき、これらの対象は元の数が$m$である有限集合の元であることを意味します。 元の数が $m$ である集合は、$m$ 元の集合とも呼ばれます。

#### 命題 1 {#ens-iii-s4-prop-1 .statement tag=03RA}

*基数 $\alpha$ は、$\alpha + 1$ が有限である場合にのみ有限です。*

関係 $\alpha = \mathfrak{b}$ と $\alpha + 1 = \mathfrak{b} + 1$ の場合、基数 $\alpha$ と $\mathfrak{b}$ の間は等価です (§ 3, no. 4、命題 8)。したがって、関係 $\alpha \ne \alpha + 1$ と $\alpha + 1 \ne (\alpha + 1) + 1$ は同等です。

¶ $0 \ne 1$ であることは明らかです。したがって、$0$ は整数です。したがって、$1$ と $2$ は整数となります。 基数 $2 + 1$ と $(2 + 1) + 1$ は整数で、それぞれ $3$ と $4$ で表されます。

### 2. 整数間の不平等

#### 命題 2 {#ens-iii-s4-prop-2 .statement tag=03RB}

※$n$を整数とします。次に、$\alpha \le n$ が整数となるように、すべての基数 $\alpha$ を計算します。 $n \ne 0$ の場合、$n = m + 1$ のような一意の整数 $m$ が存在し、関係 $\alpha < n$ は $\alpha \le m$ と同等です。*

$\alpha \le n$ の場合、$n = \alpha + \mathfrak{b}$ (§ 3, no. 6, 命題 13) となる基数 $\mathfrak{b}$ が存在します。次に、$(\alpha + 1) + \mathfrak{b} = (\alpha + \mathfrak{b}) + 1 = n + 1$ (§ 3, no. 3、命題 5、系);そして$n \ne n + 1$以来、私たちは

$$
(\alpha + 1) + \mathfrak{b} \ne \alpha + \mathfrak{b}.
$$

したがって、$\alpha + 1 \ne \alpha$、つまり $\alpha$ は整数になります。 $n \ne 0$ の場合、$n \ge 1$ (§ 3, no. 2) があるため、$n = m + 1$ (§ 3, no. 6、命題 13 および no. 4、命題 8) のような一意の基数 $m$ が存在します。 $m \leqslant n$ なので、すでに証明されていることから、$m$ は整数です。最後に、整数 $a$ が $a < n$ である場合、$b \neq 0$ (§ 3, no. 6, 命題 13) を含む $n = a + b$ が得られます。 $b$ は整数なので、$b = c + 1$ と $n = m + 1 = (a + c) + 1$ になります。したがって、$m = a + c$ (§ 3, no. 4, 命題 8) となり、$a \leqslant m$ となります。逆に、$a \leqslant m$ の場合、

$$a \leqslant m + 1 = n;$$

そして、$a = n = m + 1$ の場合、仮定とは反対に、$a > m$ になります。

#### 系 1 {#ens-iii-s4-prop-2-cor-1 .statement tag=03RC}

*有限な集合のすべての部分集合は有限です。*

#### 系 2 {#ens-iii-s4-prop-2-cor-2 .statement tag=03RD}

*もし* X *が有限集合* E の部分集合である *そして* X $\neq$ E、*その後*

$$\mathrm{Card}\ (\mathrm{X})\ <\ \mathrm{Card}\ (\mathrm{E}).$$

なぜなら、X は、単一の元の E からなるの部分集合の補数 X$'$ に含まれているからです。 $\mathrm{Card}\,(\mathrm{X}) \leqslant \mathrm{Card}\,(\mathrm{X}')$ と $\mathrm{Card}\,(\mathrm{E}) = \mathrm{Card}\,(\mathrm{X}') + 1$ があるため、(命題 2) $\mathrm{Card}\,(\mathrm{X}') < \mathrm{Card}\,(\mathrm{E})$ と *なおさら* $\mathrm{Card}\,(\mathrm{X}) < \mathrm{Card}\,(\mathrm{E})$ です。

定義 1 は、逆に、E が集合である場合、次のことを示します。

$$\mathrm{Card}\ (\mathrm{X}) < \mathrm{Card}\ (\mathrm{E})$$

X $\neq$ E となるような E のすべての部分集合 X について、E は有限です。

#### 系 3 {#ens-iii-s4-prop-2-cor-3 .statement tag=03RE}

*もし* $f$ *が有限集合* E の写像である * を集合* F にすると、*その後* $f(\mathrm{E})$ * は* F の有限部分集合になります。

$\mathrm{Card}\ (f(\mathrm{E})) \leqslant \mathrm{Card}\ (\mathrm{E})$ (§ 3, no. 2、命題 3) の場合。

#### 系 4 {#ens-iii-s4-prop-2-cor-4 .statement tag=03RF}

*E *と* F *を、同じ元の数を持つ2つの有限集合とし、* $f$を* E *into* Fの写像とする。 *すると、次の主張は等価である:*

(a) $f$ *は単射* です。
(b) $f$ *は射影です*。
(c) $f$ *は全単射です*。

(a) と (b) が同等であることを証明できれば十分です。 $f$ が単射であれば、$\mathrm{Card}(f(\mathrm{E})) = \mathrm{Card}\,(\mathrm{E}) = \mathrm{Card}\,(\mathrm{F})$、よって $f(\mathrm{E}) = \mathrm{F}$ (系 2)。 $f$ が単射でない場合、$x$ と $x'$ は、$x \neq x'$ と $f(x) = f(x')$ のように E の 2 つの元とします。次に、$\mathrm{E}' = \mathrm{E} - \{x\}$ を置くと、系 2 により、$f(\mathrm{E}') = f(\mathrm{E})$、よって $\mathrm{Card}(f(\mathrm{E})) \leqslant \mathrm{Card}\,(\mathrm{E}') < \mathrm{Card}\,(\mathrm{E})$ が得られます。しかし、$\mathrm{Card}\,(\mathrm{F}) = \mathrm{Card}\,(\mathrm{E})$ なので、$f(\mathrm{E}) \neq \mathrm{F}$ になります。

### 3. 帰納法の原理

C61 (帰納法の原理)。 *$R\{n\}$ *を理論* $\mathscr{T}$ の関係とします *(n は * $\mathscr{T}$* の定数ではありません)。* *関係* と仮定します

$$R\{0\} \quad \text{and} \quad (\forall n)((n \text{ is an integer and } R\{n\}) \Rightarrow R\{n+1\})$$

*は定理で * $\mathscr{T}$ です。 *この下条件関係*

$$(\forall n)((n \text{ is an integer}) \Rightarrow R\{n\})$$

*は定理で * $\mathscr{T}$ です。

私たちは矛盾によって議論しよう。 Suppose that 関係

$$(\exists n)(n \text{ is an integer and } (\text{not } R\{n\}))$$

それは本当です。 $q$ を「$R\{q\}$」（補助定数の方法、cf. 章 I, § 3, no. 3 および § 4, no. 1）ではない整数とします。 整数 $n$、「$n \leqslant q$ と ($R\{n\}$ ではない)」 形は整然とした空ではない集合 (§ 3, no. 2、注意) であるため、最小の元が得られます。 $s$。 $s = 0$の場合、仮定とは逆に、「$R\{0\}$ではない」。 $s > 0$ の場合、$s = s' + 1$、ここで、$s'$ は整数となり、$s' < s$ (no. 2, 命題 2) となります。 $s$ の定義までに $R\{s'\}$ が得られますが、その後仮定は、$s$ の定義とは反対に、$R\{s\}$ が真であることを意味します。

順序で帰納法の原則を適用するには、特に関係を証明する必要があります。

$$(n \text{ is an integer and } R\{n\}) \Rightarrow R\{n+1\}.$$

この目的のために、補助記号仮定 (章 I, § 3, no. 3) の方法が一般的に使用され、関係 「$n$ は整数と $R\{n\}$」 (または $R\{n\}$) と呼ばれるのはこのためです。 *inductive 仮定*.

#### 注意 {#ens-iii-s4-n3-rem-1 .statement tag=077T}

「帰納法の原則」の名の下に頻繁に使用されるさまざまな基準があります。それらはすべて C61 から簡単に推測できますが、ここではそのうちの最も重要なものを示します。

(1) $S\{n\}$ を関係とする

$$(\forall p)((n \text{ is an integer and } p \text{ is an integer and } p < n) \Rightarrow R\{p\})$$

そして、$S\{n\}$ が $R\{n\}$ を *暗示している* と仮定します。それでは関係

$$(\forall n)((n \text{ is an integer}) \Rightarrow R\{n\})$$

それは本当です。 関係 $S\{0\}$ は true であり、仮定までに $S\{n\}$ は $R\{n\}$ を意味します。 関係 $m < n + 1$ は $m \leqslant n$ (no. 2、命題 2) に相当し、関係 $S\{n + 1\}$ は "$S\{n\}$ および $R\{n\}$" に相当するため、$S\{n\}$ は $S\{n + 1\}$ を意味します。従って、基準 C61 は、関係を証明します。

$$(\forall n)\ ((n \text{ is an integer}) \Rightarrow S\{n\})$$

は true であり、$S\{n\}$ は $R\{n\}$、関係を意味するため、

$$(\forall n)\ ((n \text{ is an integer}) \Rightarrow R\{n\})$$

それは本当です。

(2) $k$ を整数とし、$R\{n\}$ を関係とし、関係

$$R\{k\} \text{ and } (\forall n)\ ((n \text{ is an integer} \geqslant k \text{ and } R\{n\}) \Rightarrow R\{n + 1\})$$

それは本当です。それでは関係

$$(\forall n)\ ((n \text{ is an integer} \geqslant k) \Rightarrow R\{n\})$$

は true (「*帰納法 k* から始まる」)。 $S\{n\}$ を関係とします

$$(n \geqslant k) \Rightarrow R\{n\}.$$

次に、場合の論理和の方法によって、 $S\{0\}$ が真であることがわかります。一方、関係は簡単に検証できます。

$$(n \text{ is an integer and } S\{n\}) \Rightarrow S\{n + 1\}$$

それは本当です。 C61 から、関係となります。

$$(n \text{ is an integer}) \Rightarrow S\{n\}$$

は真実であり、これは私たちの主張を証明します。

(3) $a$ と $b$ を 2 整数とし、$a \leqslant b$ とし、$R\{n\}$ を関係とします。

$$R\{a\} \text{ and } (\forall n)((n \text{ is an integer and } a \leqslant n < b \text{ and } R\{n\}) \Rightarrow R\{n + 1\}).$$

それでは関係

$$(\forall n)((n \text{ is an integer and } a \leqslant n \leqslant b) \Rightarrow R\{n\})$$

それは本当です。 証明は前のケースと同様です。 $S\{n\}$ は関係 "$(a \leqslant n < b) \Rightarrow R\{n\}$" ("*帰納法は区間* に制限される") であるとみなします。

(4) $a$、$b$ を 2 整数とし、$a \leqslant b$ とし、$\mathrm{R}\{n\}$ を関係とします。

$\mathrm{R}\{b\}$ と $(\forall n)((n$ は整数と $a \leqslant n < b$ と $\mathrm{R}\{n+1\}) \Rightarrow \mathrm{R}\{n\})$ です。

それでは関係

$$(\forall n)((n \text{ is an integer and } a \leqslant n \leqslant b) \Rightarrow \mathrm{R}\{n\})$$

それは本当です。私たちには関係があるからです

$(n$ は整数と $a \leqslant n < b$ そして ($\mathrm{R}\{n\}$ ではない)) $\mathrm{R}\{n+1\}$ ではなく $\Rightarrow$ です。

$a \leqslant n \leqslant b$ のようないくつかの $n$ について ($\mathrm{R}\{n\}$ ではない)、(3) から仮説に反して ($\mathrm{R}\{b\}$ ではない) という結果が得られます (*「下降帰納法」*)。

### 4. 順序集合中有限部分集合

#### 命題 3 {#ens-iii-s4-prop-3 .statement tag=03L9}

*E *を右方向の事前順序付け集合* (それぞれ *格子*、それぞれ *完全に順序付けされた集合*) とします。 *その場合、* E の空でないすべての有限部分集合は * 上に制限されます (それぞれ * には少なくとも上界と最大の下界* があり、それぞれには * には最大の元と少なくとも元* があります)。

証明は部分集合の元の数$n$の帰納法までに検討中です。 $n = 1$ の結果は些細なものです。 X を E の $n + 1$ 元 ($n \geqslant 1$ を含む) の部分集合とし、$\mathrm{X} = \mathrm{Y} \cup \{x\}$ を置きます。ここで、Y は $n$ 元を持ち、したがって空ではありません。帰納的仮定は、Y の上界 (それぞれ最小上界、それぞれ最大の元) $y$ の存在を意味します。 E は右向き (それぞれ格子、それぞれ完全に順序付けられている) であるため、$\{x, y\}$ は上界を持ちます。 (それぞれ最小上界、それぞれ最大の元)、これは明らかに X の上界 (それぞれ最小上界、それぞれ最大の元) です。

#### 系 1 {#ens-iii-s4-prop-3-cor-1 .statement tag=03LA}

*完全に順序付けされた有限有限集合はすべて整順序であり、最大の元を持ちます。*

#### 系 2 {#ens-iii-s4-prop-3-cor-2 .statement tag=03LB}

*すべての有限順序集合には極大元があります。*

このような集合は、系 1 (cf. § 2, no. 4, 定理 2) によって帰納的です。

### 5. 有限指標の性質

#### 定義 2 {#ens-iii-s4-def-2 .statement tag=03LC}

*E *を集合とします。 集合* $\mathfrak{S}$ *of 部分集合 of* E * は、関係* $\mathrm{X} \in \mathfrak{S}$ * が関係に等しい場合、* X *属するから * までの有限部分集合ごとに、指標が有限であると言われます$\mathfrak{S}$」。

$P\{X\}$ が true である$E$ の部分集合 $X$ が有限文字である場合、集合 $E$ の部分集合 $X$ の特性 $P\{X\}$ は *有限文字* であると言われます。

*例*

#### 例 1 {#ens-iii-s4-n5-exa-1 .statement tag=03T9}

完全に順序付けられた集合部分集合順序付けられた集合 $E$ は有限指標です。 実際、$E$ の部分集合 $X$ は、2 つの元のうち $X$ からなるのすべての部分集合が完全に順序付けされている場合に限り、完全に順序付けされています。

#### 例 2 {#ens-iii-s4-n5-exa-2 .statement tag=03TA}

\* すべての自由な部分集合の加群の集合は有限の指標です。同じことが、代数的に自由なすべての集合、部分集合、拡大、体にも当てはまります。

#### 例 3 {#ens-iii-s4-n5-exa-3 .statement tag=03TB}

$E$ の部分加群の有限部分集合は必ずしも $E$ の部分加群ではないため、加群 $E$ の部分加群の集合は有限指標ではありません。 \*

#### 定理 1 {#ens-iii-s4-thm-1 .statement tag=03LD}

*有限指標である集合 $E$ の部分集合のすべての集合 $\mathfrak{S}$ には極大元があります (包含によって順序付けされた場合)。

§ 2, no. 4 の定理 2 までに、$\mathfrak{S}$ が帰納的であることを示すのに十分です。これを行うには、$\mathfrak{G}$ が包含によって完全に順序付けされた $\mathfrak{S}$ のいずれかの部分集合である場合、$\mathfrak{G}$ 属するから $\mathfrak{S}$ までの集合の和集合 $X$ (§ 2, no. 4, 定理) であることを示します。 2、系 2）。 $\mathfrak{S}$ は有限指標であるため、$X$ 属するから $\mathfrak{S}$ までのすべての有限部分集合 $Y$ が示されれば十分です。さて、各 $y \in Y$ には、$y \in Z_y$ となる集合 $Z_y \in \mathfrak{G}$ が存在します。 集合 $Z_y$ $(y \in Y)$ の集合は有限であり、包含によって完全に順序付けされているため、 最大の元 $S$ (no. 4、系 1 ～ 命題 3) になります。他の語には、$Y \subset S$のような集合$S \in \mathfrak{G}$が存在します。しかし、$S \in \mathfrak{S}$ と $Y$ は $S$ の有限部分集合であるため、$\mathfrak{S}$ は有限指標であるため、$Y \in \mathfrak{S}$ になります。これで証明は完了です。

### 練習問題 {#ens-iii-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。

[^1]: The notion of “integer” will be generalized later, in Algebra, where we shall define the *rational integers* and the *algebraic integers*.
