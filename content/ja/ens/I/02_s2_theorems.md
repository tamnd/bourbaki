---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 2
section_title: Theorems
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 24-28, 56-57
pdf_pages: 0031-0035, 0063-0064
extraction: ocr
subsections:
    - "no": 1
      title: AXIOMS
      page: 24
      pdf_page: 31
    - "no": 2
      title: PROOFS
      page: 25
      pdf_page: 32
    - "no": 3
      title: SUBSTITUTIONS IN A THEORY
      page: 26
      pdf_page: 33
    - "no": 4
      title: COMPARISON OF THEORIES
      page: 26
      pdf_page: 33
statements: 1
exercises: 1
content_sha256: 005de5eb7c8ad5c95b72d6e46f925edca319c2c1665014a89554d2910c4c60fa
translated_from: content/en/ens/I/02_s2_theorems.md
translation_method: google
source_content_sha256: c8b7ac12f220f9f720128bb004ee9ac705cf905ac08dfbc648d08a0ff3975ca7
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 917414cf4a9b6a832dde389f4c5d276b4eea150e7198fb47dcc63c9ba0b11e67
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 2. 定理

※今後、$A$が関係の場合、$\neg A$ではなくnot($A$)と表記させていただきます。 $A$と$B$が関係の場合、$\vee AB$の代わりに「($A$)または($B$)」、$\Rightarrow AB$の代わりに($A$)$\Rightarrow$($B$)と書きます。 ときどき括弧は省略します。いずれの場合も、読者は問題なく検討中のアセンブリを決定するできるでしょう。*

### 1. 公理

理論 $\mathscr{T}$ の特定の記号決定する項と関係はすでに見ました。 構成する $\mathscr{T}$ までは、次のように進みます。

(1) まず、$\mathscr{T}$ の関係のうちの特定の数を書き留めます。これらは、$\mathscr{T}$ の *明示的な公理* と呼ばれます。明示的な公理に現れる文字は、$\mathscr{T}$ の *定数* と呼ばれます。

(2) $\mathscr{T}$ の *スキーム* と呼ばれる 1 つ以上のルール [^1] を定めます。これは次の特性を持たなければなりません: (a) このようなルール $\mathscr{R}$ の適用により、$\mathscr{T}$ に関係が提供されます。 (b) $T$ が $\mathscr{T}$ の項で、$x$ が文字の場合、$R$ が適用スキーム $\mathscr{R}$ によって構築された $\mathscr{T}$ の関係である場合、関係 $(T|x)R$は適用 $\mathscr{R}$でも構築できます。

私たちが想定するすべてのケースにおいて、これら条件の検証は常に簡単です。

適用によって構築されたすべての関係の $\mathscr{T}$ のスキームは、$\mathscr{T}$ の *暗黙の公理* と呼ばれます。

直観的には、公理は自明の主張か、あるいはそこから帰結を導き出したい仮説のいずれかを表します。定数は、明示的な公理によって表現されるプロパティが真であると想定される、明確に定義されたオブジェクトを表します。一方、文字 $x$ が定数でない場合、それは完全に不定のオブジェクトを表します。オブジェクト $x$ の性質が​​公理によって真であると仮定される場合、この公理は必然的に暗黙的であるため、オブジェクト $T$ に対して性質は真のままになります。

### 2. 証明

理論 $\mathscr{T}$ の *説明文* は次のとおりです。

(1) $\mathscr{T}$ の関係と項の補助形声構成。

(2) $\mathscr{T}$ の *証明、つまり $\mathscr{T}$ の関係の数列が補助形声構成に現れ、数列のすべての関係 $\mathbf{R}$ に対して、次の少なくとも 1 つが成立します。 条件は満足しています :

(a$_1$) $\mathbf{R}$ は $\mathscr{T}$ の明示的な公理です。

(a$_2$) $\mathbf{R}$ は、補助形成形構成に現れる項または関係に$\mathscr{T}$ のスキームを適用した結果です。

(b) 数列には、$\mathbf{R}$ の前に 2 つの関係 $\mathbf{S}$、$\mathbf{T}$ があり、$\mathbf{T}$ は$\mathbf{S} \Rightarrow \mathbf{R}$ になります。

¶ $\mathscr{T}$ の *定理* は、* $\mathscr{T}$ の証明に現れる関係です。

したがって、この概念は本質的に、それが記述されている時点での検討中の理論の状態に依存します。 理論 $\mathscr{T}$ の関係は、$\mathscr{T}$ の証明に挿入することに成功すると、$\mathscr{T}$ の定理になります。 $\mathscr{T}$の関係が「$\mathscr{T}$の定理ではない」というできないは、理論$\mathscr{T}$の発達段階に関係なく意味を持ちます。

$\mathscr{T}$ の定理は、「*true* 関係 in $\mathscr{T}$」 (または「命題」、「補題」、「系」など) とも呼ばれます。 $\mathbf{R}$ を $\mathscr{T}$ の関係とし、$\mathbf{x}$ を文字、$\mathscr{T}$ を $\mathbf{T}$ 項とします。 $(\mathbf{T}|\mathbf{x})\mathbf{R}$ が $\mathscr{T}$ の定理である場合、$\mathbf{R}$ を考慮すると、$\mathbf{T}$ は $\mathscr{T}$ の *満たす関係* $\mathbf{R}$ (または * $\mathbf{R}$ の *解である) と言われます。 $\mathbf{x}$の関係として。

¶ 関係は、$\mathscr{T}$ でその否定が定理である場合、$\mathscr{T}$ では *偽* であると言われます。 $\mathscr{T}$ で真でもあり偽でもある関係を書いた場合、理論 $\mathscr{T}$ は *矛盾* であると言われます。

ここでも、理論の特定の開発状態に依存する概念を扱っています。読者は、関係 $\mathbf{R}$ が $\mathscr{T}$ で偽であることを証明すると、それによって $\mathscr{T}$ の $\mathbf{R}$ が「真ではない」ことが確立されると信じることからなる混乱 (語 「偽」の直感的な意味によって残念なことに示唆されている) に注意する必要があります (厳密に言えば、この表現には意味がありません)上で述べたように、*数学*における正確な意味)。

¶ 以下では、*演繹的基準*と呼ばれるメタ数学的基準を与え、証明を短縮できるようにします。これらの基準は、C の後に数が続く文字で示されます。

C1 (*三段論法*)。 ※$\mathbf{A}$と$\mathbf{B}$を理論$\mathscr{T}$の関係とします。 $\mathbf{A}$ と $\mathbf{A} \Rightarrow \mathbf{B}$ が $\mathscr{T}$ の定理である場合、$\mathbf{B}$ は $\mathscr{T}$ の定理です。*

$A$ が出現する $\mathscr{T}$ の $R_1$, $R_2$, ..., $R_n$ を証明とし、$S_1$, $S_2$, ..., $S_p$ を証明とする$A \Rightarrow B$が登場する$\mathscr{T}$。明らかに、$R_1$、$R_2$、...、$R_n$、$S_1$、$S_2$、...、$S_p$ は、$A$ と $A \Rightarrow B$ の両方が出現する $\mathscr{T}$ の証明です。したがって、

$$R_1, \; R_2, \; \ldots, \; R_n, \; S_1, \; S_2, \; \ldots, \; S_p, \; B$$

は $\mathscr{T}$ の証明であるため、$B$ は $\mathscr{T}$ の定理になります。

### 3. 理論の選手交代

$\mathscr{T}$ を理論、$A_1$、$A_2$、...、$A_n$ をその明示的な公理、$x$ を文字、$\mathscr{T}$ の $T$ 項とします。 $(T|x)\mathscr{T}$ を理論とし、その符号とスキームは $\mathscr{T}$ のものと同じであり、その明示的な公理は $(T|x)A_1$、$(T|x)A_2$、...、$(T|x)A_n$ です。

C2. ※$A$を理論$\mathscr{T}$の定理、$T$を$\mathscr{T}$の項、$x$を文字とします。すると、$(T|x)A$ は理論 $(T|x)\mathscr{T}$ の定理になります。*

$A$が出現する$\mathscr{T}$の$R_1$、$R_2$、...、$R_n$を証明とします。 CF8 (§ 1, no. 4) の理由により、$\mathscr{T}$ の関係の数列である数列 $(T|x)R_1$、$(T|x)R_2$、...、$(T|x)R_n$ を考えてみましょう。この数列が理論 $(T|x)\mathscr{T}$ の証明であることを示します。これにより基準が確立されます。 $R_k$ が $\mathscr{T}$ の暗黙の公理である場合、$(T|x)R_k$ は再び $\mathscr{T}$ (no. 1) の暗黙の公理、つまり $(T/x)\mathscr{T}$ の暗黙の公理です。 $R_k$ が $\mathscr{T}$ の明示的な公理である場合、$(T|x)R_k$ は $(T|x)\mathscr{T}$ の明示的な公理です。最後に、$R_k$ の前に関係 $R_i$ および $R_j$ があり、$R_j$ が $R_i \Rightarrow R_k$ である場合、$(T|x)R_k$ の前には $(T|x)R_i$ および $(T|x)R_j$ があり、後者は $(T|x)R_i \Rightarrow (T|x)R_k$ と同一です。 (基準 CS5)。

C3. *$A$を理論$\mathscr{T}$の定理、$T$を$\mathscr{T}$の項、$x$を$\mathscr{T}$の定数ではない文字とする。すると、$(T|x)A$ は $\mathscr{T}$ の定理になります。*

$x$ は $\mathscr{T}$ の明示的な公理に含まれていないため、これは C2 の直後に続きます。より具体的には、$\mathscr{T}$ 含むに明示的な公理がない場合、または明示的な公理含むに文字がない場合、基準 C3 は文字 $x$ に制限なしで適用されます。

### 4. 理論の比較

理論 $\mathscr{T}'$ は、$\mathscr{T}$ のすべての符号が $\mathscr{T}'$ の符号であり、$\mathscr{T}$ のすべての明示的な公理が $\mathscr{T}'$ の定理であり、$\mathscr{T}$ のスキームである場合、理論 $\mathscr{T}$ より *強い* と言われます。は$\mathscr{T}'$のスキームです。

C4. *理論 $\mathscr{T}'$ が理論 $\mathscr{T}$ より強い場合、$\mathscr{T}$ のすべての定理は $\mathscr{T}'$ の定理になります。

$R_1$, $R_2$, ..., $R_n$ を $\mathscr{T}$ の証明とします。それぞれの $R_i$ が $\mathscr{T}'$ では定理であることを段階的に示していきます。これが $R_k$ より前の関係に当てはまると仮定します。 $R_k$が$\mathscr{T}$の公理であれば、仮定により$\mathscr{T}'$の定理になります。 $R_k$ の前に関係 $R_i$ と $R_i \Rightarrow R_k$ がある場合、$R_i$ と $R_i \Rightarrow R_k$ は $\mathscr{T}'$ の定理であることがすでにわかっているため、$R_k$ は定理になります。 C1のおかげで$\mathscr{T}'$。したがって、どの場合でも、$R_k$ は $\mathscr{T}'$ の定理となり、証明が完了します。

2 つの理論 $\mathscr{T}$ と $\mathscr{T}'$ がそれぞれ他方より強い場合、$\mathscr{T}$ と $\mathscr{T}'$ は *同等* であると言われます。すると、$\mathscr{T}$ のすべての定理は $\mathscr{T}'$ の定理となり、その逆も同様です。

C5. *$\mathscr{T}$ を理論、$A_1$、$A_2$、...、$A_n$ をその明示的な公理、$a_1$、$a_2$、...、$a_h$ をその定数、$T_1$ とします。 $T_2$、...、$T_h$ は $\mathscr{T}$ で項になります。次のように仮定します*

$$(T_1|a_1) \, (T_2|a_2) \, \ldots \, (T_h|a_h)A_i \qquad (\text{for} \quad i = 1, 2, \ldots, n)$$

* は理論 $\mathscr{T}'$ の定理であり、$\mathscr{T}$ の符号は $\mathscr{T}'$ の符号であり、$\mathscr{T}$ のスキームは $\mathscr{T}'$ のスキームであること。次に、$A$ が $\mathscr{T}$ の定理である場合、*

$$(T_1|a_1) \, \ldots \, (T_h|a_h)A$$

*は $\mathscr{T}'$ の定理です。*

$\mathscr{T}'$ は理論 $(T_1|a_1) \ldots (T_n|a_n) \mathscr{T}$ よりも強いため、C2 と C4 を適用できます。

この手順を使用して、$\mathscr{T}$の定理から$\mathscr{T}'$の定理を演繹すると、*$\mathscr{T}$の結果$\mathscr{T}'$では適用であると言えます*。直観的には、$\mathscr{T}$ の公理は $a_1, a_2, ..., a_h$ の性質を表し、$A$ はこれらの公理の帰結である性質を表します。 $\mathscr{T}'$ のオブジェクト $T_1, T_2, ..., T_h$ が $\mathscr{T}$ の公理で表される性質を持っている場合、それらは性質 $A$ も持ちます。

\*たとえば、群 $\mathscr{T}$ の理論では、明示的な公理含むの 2 つの定数 G と $\mu$ (合成の群と法則) です。 集合 $\mathscr{T}'$ の理論では、 定義する 2 つの項 : 実数の実直線と加法です。 $\mathscr{T}$ の明示的な公理で、これらの項を G と $\mu$ にそれぞれ代入すると、$\mathscr{T}'$ で定理が得られます。また、$\mathscr{T}$と$\mathscr{T}'$のスキームと符号は同じです。したがって、「群理論の結果を実数の加法群に適用する」ことができます。 集合の理論で群理論の*モデル*を構築したと言います。 (群の理論は集合の理論より強いため、集合の理論の結果を群の理論に適用することもできます。)\*

#### 注意 {#ens-i-s2-n4-rem-1 .statement tag=03G7}

C5 の仮説の下では、理論 $\mathscr{T}$ が矛盾していることが判明した場合、同じことが $\mathscr{T}'$ にも当てはまります。たとえば、$A$ と「$A$ ではない」が $\mathscr{T}$ の定理である場合、$(T_1|a_1) \ldots (T_h|a_h)A$ と $\mathrm{not}(T_1|a_1) \ldots (T_h|a_h)A$ は $\mathscr{T}'$ の定理です。 \* たとえば、群の理論が矛盾している場合、集合の理論も矛盾します。 \*

### 練習問題 {#ens-i-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。

[^1]: For the sake of brevity, these rules are expressed by using the symbols mentioned in § 1, no. 1 (and especially bold-faced italic letters); but it would be easy to avoid the use of these symbols completely in the formulation of the rules (see § 3, no. 1, note (*) on p. 28).
