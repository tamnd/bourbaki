---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 1
section_title: Polynomial maps and Zariski topology
appendix: true
lang: ja
source: lie-vii-ix
book_pages: 45-47, 66
pdf_pages: 0055-0057, 0075-0075
extraction: native
subsections:
    - "no": 1
      title: ZARISKI TOPOLOGY
      page: 45
      pdf_page: 55
    - "no": 2
      title: DOMINANT POLYNOMIAL MAPS
      page: 46
      pdf_page: 56
statements: 7
exercises: 4
content_sha256: 8a36241e4a96d5a994f20a2be08aa3fece04c79cbecb6da2b271c331edf269ee
translated_from: content/en/lie/VII/A1_a1_polynomial_maps_and_zariski_topology.md
translation_method: google
source_content_sha256: 35b05a39838f20b88ddf3fc98b3fdd147867c98e1efaf99bb5c98caf247537a5
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 65b22ed31b29d693927b66e489f1e2b78d43499c0179da475f2fb3e33ce32492
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 付録 I 多項式写像とザリスキー 位相

この付録では、$k$は無限大であると仮定します。

### 1. ザリスキー 位相

V を有限次元ベクトル空間とします。 $k($代数の値を、V の多項式関数の $A_V$ 代数で表します。 IV, §5, no. 10、デフォルト。 4)。 これはグレード代数です。 次数 1 の成分は、V の双対 $V^*$ と $V^*$ の単射を、対称代数 $\mathbf{S}(V^*)$ から $A_V$ 拡大するから同型に変換します。 $A_V($代数、章。 IV, §5, no. 11、注意 2)。

$(e_1, . . . , e_n)$ が V の基底で、不定の $(X_1, . . . ,X_n)$ 数列である場合、$k[X_1, . . . ,X_n]$ から $A_V$ までの写像は、$k[X_1, . . . ,X_n]$ から写像のいずれかの元 $f$ をとります。

$$
\sum_{i=1}^n\lambda_ie_i \rightarrow f(\lambda_1, . . . , \lambda_n)
$$

は、代数の同型です (代数、第 IV, §5, no. 10 章、提案 19 の修正)。

#### 命題 1 {#lie-vii-a1-prop-1 .statement tag=00XC}

H を $A_V$ から $k$ までの代数準同型の集合とします。任意の $x\in V$ について、$h_x$ を $A_V$ から $k$ までの準同型 $f \rightarrow f(x)$ とします。すると、写像$x \rightarrow h_x$はVからHまで全単射になります。

確かに、$H'$ を $k[X_1, . . . ,X_n]$ から $k$ までの代数準同型の集合とします。 写像 $\chi  \rightarrow (\chi (X_1), . . . , \chi (X_n))$ は明らかに $H'$ から $k^n$ までの全単射です。

#### 系 {#lie-vii-a1-n1-cor-1 .statement tag=00XD}

任意の $x\in V$ に対して、$\mathfrak{m}_x=$ Ker($h_x$) とします。すると、写像 $x \rightarrow \mathfrak{m}_x$ は、$A_V$ の理想$\mathfrak{m}$ のV から集合までの全単射となり、$A_V/\mathfrak{m}=k$ になります。

すべての $i\in I$ に対して $x\in F\Leftarrow \Rightarrow x\in V$ と $f_i(x) = 0$ となるような $A_V$ の元のファミリー $(f_i)_{i\in I}$ が存在する場合、V の部分集合 F は閉じていると言われます。

$\emptyset$ と V が閉じていること、および閉じている集合のいずれかの共通部分が閉じていることは明らかです。 F が $f_i$ の消滅によって定義され、$F'$ が $f'_j$ の消滅によって定義される場合、$F\cup F'$ は $f_if'_j$ の消滅によって定義されるため、閉じられます。 したがって、V には位相が存在し、この位相の閉じた集合は、上記の意味でまさに閉じた集合になります。 この位相は、Vのザリスキー位相と呼ばれます。 任意の $f\in A_V$ については、$x\in V$ の $V_f$ 集合によって $f(x)\not= 0$ のように表されます。これはVのオープン部分集合です。 ザリスキー位相の$V_f$形基底は明らかです。 ($k$ がトポロジカル体である場合、V の標準位相はザリスキー 位相よりもより細かいです。)

コルの写像 $x \rightarrow \mathfrak{m}_x$提案 1 の V から $A_V($可換代数の素スペクトル Spec(A$_V$) までの写像 $\varepsilon$ と考えることができます。 II, §4, no. 3、デフォルト。 4)。スペック(A$_V$)の位相の$\varepsilon$でザリスキー位相が逆像であるのは明らかです。

#### 命題 2 {#lie-vii-a1-prop-2 .statement tag=00XE}

ザリスキー位相を装備したベクトル空間Vは、還元不可能なネーター空間です。特に、V の空ではないオープン部分集合はすべて密集しています。

$A_V$ はネーター なので、Spec(A$_V$) はネーター (可換代数、II, §4, no. 3、提案 11 の Cor. 7)、ネーター 空間のすべての部分空間はネーター です。 (上記引用、no. 2、提案 8)。コルの記法と。提案1の$\mathfrak{m}_x$の共通部分は$\{0\}$、$\{0\}$は$A_V$の主要な理想です。したがって、V は既約です (上記引用、no. 3、提案 14)。

### 2. 支配多項式写像

$V,W$ を有限次元ベクトル空間とします。 $f$ を、V から W までの多項式写像とします (代数、章 IV, §5, no. 10、定義 4)。 $\psi \in A_W,\psi \circ f\in A_V$ の場合 (上記引用、提案 17)。 写像 $\psi  \rightarrow \psi \circ f$ は、$A_W$ から $A_V$ までの準同型で、$f$ に関連付けられていると言われています。その核は写像 $\psi \in A_W$ で構成されており、$f(V)$ に消滅します (したがって、ザリスキー 位相の $f(V)$ の終了にも伴います)。

#### 定義 1 {#lie-vii-a1-def-1 .statement tag=00XF}

$f$ に関連付けられた $A_W$ から $A_V$ までの準同型が単射である場合、多項式写像 $f: V\rightarrow W$ が優勢であると言われます。

上記を考慮すると、$f(V)$ がザリスキー位相の W に密集している場合にのみ、$f$ が優勢になります。

#### 命題 3 {#lie-vii-a1-prop-3 .statement tag=00XG}

$k$ が代数的に閉じていると仮定します。 $f: V\rightarrow W$ を優多項式写像とします。 像任意の密なオープンの $f$ の下部分集合の V 含む密なオープン部分集合 W.

$A_V,f(V_{\varphi})$ 含むのゼロ以外のすべての元 $\varphi$ に対して、$A_V$ の部分代数を伴う W の密なオープン部分集合同一視する $A_W$ を証明するだけで十分です。 準同型は $f$ に関連付けられています。 $A_W$ の非ゼロの元 $\psi$ が存在し、$\psi$ 拡大するから準同型 $v: A_V\rightarrow k$ が消滅しないすべての準同型 $w: A_W\rightarrow k$ が存在します。 $\varphi ($可換代数、章。 V, §3, no. 1、コル。 Thの3。 1)。さて、そのような$w$ (それぞれ$v$) は、$W_{\psi}$ (それぞれ$V_{\varphi}$) の元と識別でき、$v$ 拡大する $w$ は $f(v) =w$ を意味すると言えます。したがって、$W_{\psi}\subset f(V_{\varphi})$。 Q.E.D.

$f: V\rightarrow W$ を多項式写像および $x_0\in V$ とします。 写像 $h \rightarrow f(x_0+h)$ V から W は多項式です。これを同次多項式写像の有限和に分解します。

$$
f(x_0+h) =f(x_0) + D_1(h) + D_2(h) +\cdots
$$

ここで、$D_i: V\rightarrow W$ は次数 $i($代数と同次です。 IV, §5, no. 10、提案 19)。直線写像 $D_1$ は、$x_0$ における $f$ の接線直線写像と呼ばれます。それを$Df(x_0)$で表します。

#### 命題 4 {#lie-vii-a1-prop-4 .statement tag=00XH}

$f: V\rightarrow W$ を多項式写像とします。 $(Df)(x_0)$が全射となるような$x_0\in V$が存在すると仮定します。そうすると$f$が優勢です。

適用 V の翻訳と W の翻訳は、$x_0= 0$ と $f(x_0) = 0$ であると想定できます。 $f$ の分解は同種元の和として書くことができます

$f=f_1+f_2+\cdots$ 度 $f_i=i$、

そして線形写像 $f_1$ は仮定により全射です。 $f$ が優勢ではないと仮定します。次に、$\psi \circ f= 0$ のような $A_W$ の非ゼロ元 $\psi$ が存在します。 $\psi =\psi_m+\psi_{m+1}+\cdots$ を $\psi$ の分解として、$\psi_i=i$ と $\psi_m\not= 0$ 度で同次の元にします。それから

$$
0 =\psi \circ f=\psi_m\circ f+\psi_{m+1}\circ f+\cdots
$$

$$
=\psi_m\circ f_1+\rho
$$

ここで、$\rho$ は次数 $> m$ の同次多項式写像の和です。 $\psi_m\circ f_1= 0$ ということになります。 $f_1$は全射なので、$\psi_m= 0$は矛盾です。

#### 系 {#lie-vii-a1-n2-cor-1 .statement tag=00XI}

$k$ が代数的に閉じており、$f$ が提案 4 の仮定を満たす場合、任意の密なオープン V の部分集合含む W の密なオープン部分集合の $f$ の下で像が満たされます。

これは Props からの続きです。 3と4。

### 練習問題 {#lie-vii-a1-exercises}

$k$ 上の有限次元ベクトル空間を V で表します。

[練習問題付録 1](exercises/a1/)を参照してください。
