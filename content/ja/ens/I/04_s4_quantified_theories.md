---
book: ens
book_title: Theory of Sets
chapter: I
chapter_title: DESCRIPTION OF FORMAL MATHEMATICS
section: 4
section_title: Quantified theories
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 36-44, 58-59
pdf_pages: 0043-0051, 0065-0066
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF QUANTIFIERS
      page: 36
      pdf_page: 43
    - "no": 2
      title: AXIOMS OF QUANTIFIED THEORIES
      page: 37
      pdf_page: 44
    - "no": 3
      title: PROPERTIES OF QUANTIFIERS
      page: 38
      pdf_page: 45
    - "no": 4
      title: TYPICAL QUANTIFIERS
      page: 41
      pdf_page: 48
statements: 0
exercises: 8
content_sha256: 48055b4ef408d7477da04f7030487cee7806e5f05b40b6ffd093d15fd6ae4d85
translated_from: content/en/ens/I/04_s4_quantified_theories.md
translation_method: google
source_content_sha256: 07568a80b2b793e5dd22b88d7dc9caf03ded631f676da9f844c975c64e8b5a2c
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 21ea32afb2560eb023357b363125e3602618d02909f94498a2797c5c1fbab3ca
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 4. 定量化された理論

### 1. 数量詞の定義

§ 3 で役割を果たした唯一の論理記号は、$\neg$ と $\vee$ です。これから説明するルールは、基本的に論理記号 $\tau$ と $\square$ の使用に関するものです。

¶ $R$ がアセンブリ、$x$ が文字の場合、アセンブリ $(\tau_x(R)|x)R$ は、「$R$ となるような $x$ が存在する」、または $(\exists x)R$ で表されます。集会

$$\text{"not } ((\exists x) \text{ not } R)\text{"}$$

は、「すべての $x$、$R$」、または「任意の $x$、$R$」、または $(\forall x)R$ で表されます。省略記号 $\exists$ と $\forall$ は、それぞれ *存在量指定子* と *普遍量指定子* と呼ばれます。文字 $x$ は、$\tau_x(R)$ で示されるアセンブリには表示されず、*したがって、$(\exists x)R$ および $(\forall x)R$ で示されるアセンブリにも表示されません*。

CS8。 ※$R$をアセンブリ、$x$と$x'$を文字とします。 $x'$ が $R$ に現れない場合、$(\exists x)R$ と $(\forall x)R$ はそれぞれ $(\exists x')R'$ と $(\forall x')R'$ と同一になります。ここで、$R'$ は $(x'|x)R$ です*。

$(\tau_x(R)|x)R$ は CS1 (§ 1, no. 2) によって$(\tau_x(R)|x')R'$ と同一であり、$\tau_x(R)$ は CS3 (§ 1, no. 2) によって$\tau_{x}'(R')$ と同一です。したがって、$(\exists x)R$ は $(\exists x')R'$ と同一です。したがって、$(\forall x)R$ は $(\forall x')R'$ と同一になります。

CS9。 *$R$ と $U$ をアセンブリとし、$x$ と $y$ を個別の文字とします。 $X$ が $U$ に現れない場合、$(U|y)(\exists x)R$ と $(U|y)(\forall x)R$ はそれぞれ $(\exists x)R'$ と $(\forall x)R'$ と同一になります。ここで、$R'$ は $(U|y)R$ です*。

というのは、CS2 (§ 1, no. 2) によれば、$(U|y)(\tau x(R)|x)R$ は以下と同一であるからです。

$$(T|x)(U|y)R,$$

ここで、CS4 (§ 1, no. 2) によると、$T$ は $(U|y)\tau_x(R)$、つまり $\tau_x(R')$ です。従って、$(U|y)(\exists x)R$ は $(\exists x)R'$ と同一であり、その結果、$(U|Y)(\forall x)R$ は$(\forall x)R'$ と同一です。

CF11。 *$R$ が理論 $\mathscr{T}$ の関係で、$x$ が文字の場合、$(\exists x)R$ と $(\forall x)R$ は $\mathscr{T}$ の関係です。

これは、CF3、CF8、CF2 (§ 1, no. 4) の直後に続きます。

直感的に、$R$ は、$x$ で示されるオブジェクトの性質を表現していると考えてみましょう。 項 $\tau_x(R)$ の直感的な意味から、主張 $(\exists x)R$ は、性質 $R$ を持つオブジェクトがあることを意味します。 主張「$(\exists x)$ではない($R$ではない)」は、性質「$R$ではない」を持つオブジェクトはなく、したがってすべてのオブジェクトは性質$R$を持つことを意味します。

論理理論 $\mathscr{T}$ では、形 $(\exists x)R$ の定理があり、文字 $x$ が $\mathscr{T}$ の定数ではない場合、この定理は、次の正当性の定理として機能します。補助定数 (§ 3, no. 3) の方法は、$(\tau_x(R)|x)R$ と同一であるためです。 $\mathscr{T}'$ を $R$ を $\mathscr{T}$ の公理に隣接させて得られる理論とします。 理論 $\mathscr{T}'$ で $x$ が現れない証明できる関係 $S$ とすると、$\mathscr{T}$ では $S$ が定理になります。

C26. *$\mathscr{T}$ を論理的な理論とし、$R$ を $\mathscr{T}$ の関係とし、$x$ を文字とします。 関係 $(\forall x)R$ と $(\tau_x(\text{not } R)|x)R$ は、$\mathscr{T}$ では等価になります。*

$(\forall X)R$ は「$(\tau_x(\text{not } R)|x)(\text{not } R)$ ではない」と同じであり、従って「$(\tau_x(\text{not } R)|x)R$ ではない」と同じです。

C27. *文字 $x$ が定数ではない論理理論 $\mathscr{T}$ で $R$ が定理である場合、$(\forall x)R$ は $\mathscr{T}$ の定理になります。

$(\tau_x(\text{not } R)|X)R$ は、C3 (§ 2, no. 3) による $\mathscr{T}$ の定理です。

一方、$x$ が $\mathscr{T}$ の定数である場合、$R$ の真実は $(\forall x)R$ の真実を意味しません。直観的には、$R$ が $\mathscr{T}$ の明確なオブジェクトである $x$ の真の性質であるという事実は、明らかに、$R$ がすべてのオブジェクトの真の性質であることを意味しません。

C28. *$\mathscr{T}$ を論理理論とし、$R$ を $\mathscr{T}$ の関係とし、$x$ を文字とします。次に、関係* 「$(\forall x)R$ ではない」 * と $(\exists x)(\text{not } R)$ は $\mathscr{T}$ では同等です。*

「$(\forall x)R$ではない」は「$(\exists x)(\text{not } R)$ではない」と同じです。

### 2. 定量化された理論の公理

*定量化された理論* は、スキーム S1 から S4 (§ 3, no. 1) と以下のスキーム S5 が暗黙の公理を提供する任意の理論 $\mathscr{T}$ です。

S5. *$R$ が $\mathscr{T}$ の関係である場合、$T$ が $\mathscr{T}$ の項である場合、および $x$ が文字の場合、関係 $(T|x)R \Rightarrow (\exists x)R$ は公理です。

このルールはまさに計画です。 $A$ を適用 S5 によって得られた $\mathscr{T}$ の公理とする。次に、$\mathscr{T}$には関係$R$、$\mathscr{T}$には項$T$、そして$A$が$(T|x)R \Rightarrow (\exists x)R$となる文字$x$があります。 $U$ を $\mathscr{T}$ の項とし、$y$ を文字とします。 $(U|y)A$ は適用 S5 によっても取得できることを示します。 CS1 (§1, no. 2) と CS8 (no. 1) を使用すると、$x$ が $y$ とは異なり、$U$ には現れない場合に限定できます。 $R'$ を関係 $(U|y)R$ および $T'$ 項 $(U|y)T$ とします。基準 CS2 (§1, no. 2) および CS9 (no. 1) は、$(U|y)A$ が $(T'|x)R' \Rightarrow (\exists x)R'$ と同一であることを示しています。

スキーム S5 は、$x$ の性質を表すと考えられる関係 $R$ が真であるオブジェクト $T$ がある場合、オブジェクト $\tau_x(R)$ については $R$ が真であると述べています。これは、$\tau_x(R)$ (§1, no. 3、注意) に帰する直感的な意味と一致します。

### 3. 数量指定子のプロパティ

これからは定量化された理論のみを考慮する必要があります。この切断の残りについては、$\mathscr{T}$ はそのような理論を表し、$\mathscr{T}_0$ は$\mathscr{T}$ と同じ符号を持ち、唯一のスキームが S1 から S5 である明示的な公理なしで理論を表します。 $\mathscr{T}$は$\mathscr{T}_0$よりも強いです。

C29. ※$R$を$\mathscr{T}$の関係とし、$x$を文字とします。その場合、関係「$(\exists x)R$ではない」と$(\forall x)(\text{not } R)$は、$\mathscr{T}$では同等です。*

$x$ が定数ではない理論 $\mathscr{T}_0$ の基準を証明できれば十分です。 定理 $R \Leftrightarrow (\text{not not } R)$ は、C3 (§2, no. 3) により、定理を与えます。
$$(\exists x)R \Rightarrow (\tau_x(R)|x)(\text{not not } R)$$
そして
$$(\exists x)(\text{not not } R) \Rightarrow (\tau_x(\text{not not } R)|X)R.$$

適用 S5、$\mathscr{T}_0$ で定理を推測します
$$(\exists x)R \Rightarrow (\exists x)(\text{not not } R), \quad (\exists x)(\text{not not } R) \Rightarrow (\exists x)R,$$
よって定理 $(\exists x)R \Leftrightarrow (\exists x)(\text{not not } R)$。今
$$(\exists x)(\text{not not } R)$$
$\mathscr{T}_0$ では、「$(\exists x)(\text{not not } R)$ ではない」、つまり「$(\forall x)(\text{not } R)$ ではない」と同等です。従って、結果は次のとおりです。

基準 C28 および C29 により、一方の量指定子のプロパティを他方の量指定子のプロパティから推定することができます。

C30。 *$R$を$\mathscr{T}$の関係、$T$を$\mathscr{T}$の項、$x$を文字とします。すると、関係 $(\forall x)R\Longrightarrow(T|x)R$ は $\mathscr{T}$ の定理になります。*

S5 までに、$(T|x)(\text{not }R)\Longrightarrow(\tau_x(\text{not }R)|x)(\text{not }R)$ は公理です。この関係は以下と同一です

$$
(\text{not }(T|x)R)\Longrightarrow\text{not}(\tau_x(\text{not }R)|x)R.
$$

従って、$(\tau_x(\text{not }R)|x)R\Longrightarrow(T|x)R$は$\mathscr{T}$の定理になります。ここでは C26 (no. 1) を使用します。

$R$を$\mathscr{T}$の関係とします。 C26、C27、および C30 では、$\mathscr{T}$ または定理 $(\forall x)R$ で定理 $R$ を述べても、あるいはメタ数学的規則を述べても、同じです (文字 $x$ が $\mathscr{T}$ の定数ではないという条件)。 $T$ が $\mathscr{T}$ の任意の項である場合、$(T|x)R$ は $\mathscr{T}$ の定理になります。

C31. ※$R$と$S$は$\mathscr{T}$の関係、$x$は$\mathscr{T}$の定数ではない文字とします。 $R\Longrightarrow S$ (それぞれ $R\Longleftrightarrow S$) が $\mathscr{T}$ の定理である場合、*

$$
(\forall x)R\Longrightarrow(\forall x)S,\qquad(\exists x)R\Longrightarrow(\exists x)S
$$

$$
[\text{resp. }(\forall x)R\Longleftrightarrow(\forall x)S,\qquad(\exists x)R\Longleftrightarrow(\exists x)S]
$$

*は定理は $\mathscr{T}$ です。*

$R\Longrightarrow S$が$\mathscr{T}$の定理だとします。 仮定 $(\forall x)R$ ($x$ は現れません) を隣接させましょう。その場合、$R$、従って $S$、従って $(\forall x)S$ も真になります。従って、$(\forall x)R\Longrightarrow(\forall x)S$ は $\mathscr{T}$ の定理になります。従って、$R\Longleftrightarrow S$ が $\mathscr{T}$ の定理である場合、同様になります。

$$
(\forall x)R\Longleftrightarrow(\forall x)S.
$$

$\exists$ に関連するルールは、C29 を使用して推定できるようになりました。

C32. ※$R$と$S$を$\mathscr{T}$の関係、$x$を文字とします。それでは関係*

$$
(\forall x)(R\text{ and }S)\Longleftrightarrow((\forall x)R\text{ and }(\forall x)S),
$$

$$
(\exists x)(R\text{ or }S)\Longleftrightarrow((\exists x)R\text{ or }(\exists x)S)
$$

*は $\mathscr{T}$ の定理です。*

これらの基準は、$x$ が定数ではない $\mathscr{T}_0$ で証明できれば十分です。 $(\forall x)(R\text{ and }S)$ が true の場合、「$R$ と $S$」も true となり、関係 $R$、$S$ もそれぞれ true になります。従って、関係 $(\forall x)R$、$(\forall x)S$ はそれぞれ true となり、従って「$(\forall x)R$ および $(\forall x)S$」も true になります。同様に、「$(\forall x)R$ と $(\forall x)S$」が真であれば、$(\forall x)(R\text{ and }S)$ も真であることがわかります。従って、最初の定理です。 2 番目は適用 C29 に続きます。

It should be noted that if $(\forall x) (R$ or S) is a theorem in $\mathscr{T}$, we may not conclude that $((\forall x)R$ or $(\forall x)S)$ is a theorem in $\mathscr{T}$. 直観的には、関係 $(\forall x) (R$ または S) が true であるということは、各オブジェクト $x$ について、関係 $R$、$S$ の少なくとも 1 つが true であることを意味します。しかし、一般的には 2 つのうち 1 つだけが真となり、それが $R$ か $S$ かは $x$ の選択によって決まります。 Likewise, if $((\forall x)R$ and $(\exists x)S)$ is a theorem in $\mathscr{T}$, we may not conclude that $(\exists x)(R$ and S) is a theorem in $\mathscr{T}$. ただし、次の基準があります。

C33. ※$R$と$S$は$\mathscr{T}$の関係、$x$は$R$に出てこない文字とします。それから関係*

$$(\forall x)(R \text{ or } S) \iff (R \text{ or } (\forall x)S),$$
$$(\exists x)(R \text{ and } S) \iff (R \text{ and } (\exists x)S)$$

*は $\mathscr{T}$ の定理です。*

$x$ が定数ではない$\mathscr{T}_0$ で基準を確立するだけで十分です。 $\mathscr{T}'$ を $\mathscr{T}_0$ の公理に $(\forall x)(R$ または S) を隣接させて得られる理論とします。 $\mathscr{T}'$ では、「$R$ または $S$」、従って ($R$ ではなく) $\Rightarrow S$ は定理です。 「$R$ではない」が真（$x$が登場しない仮定）の場合、$S$、従って$(\forall x)S$も真になります。その結果

$$(\text{not } R) \Rightarrow (\forall x)S$$

は $\mathscr{T}'$ の定理であるため、$(\forall x)(R$ または $S) \Rightarrow (R$ または $(\forall x)S)$ は $\mathscr{T}_0$ の定理になります。同様に、「$R$ または $(\forall x)S$」が true の場合、「$R$ または $S$」、つまり $(\forall x)(R$ または S) が true になります。その結果

$$(R \text{ or } (\forall x)S) \Rightarrow (\forall x)(R \text{ or } S)$$

は $\mathscr{T}_0$ の定理です。 $\exists$ に関連するルールは、適用 C29 に続きます。

C34. ※$R$を関係、$x$と$y$を文字とします。それから関係*

$$(\forall x)(\forall y)R \iff (\forall y)(\forall x)R,$$
$$(\exists x)(\exists y)R \iff (\exists y)(\exists x)R,$$
$$(\exists x)(\forall y)R \implies (\forall y)(\exists x)R$$

*は $\mathscr{T}$ の定理です。*

これらの定理を $\mathscr{T}_0$ で証明すれば十分です。ただし、$x$ と $y$ は定数ではありません。 $(\forall x)(\forall y)R$ が真の場合、$(\forall y)R$、従って $R$、従って $(\forall x)R$、従って $(\forall y)(\forall x)R$ も真になります。同様に、$(\forall y)(\forall x)R$ が true の場合、$(\forall x)(\forall y)R$ も true になります。最初の定理が続きます。 2 番目は C29 を使用して続きます。最後に、$(\forall y)R \Rightarrow R$ は $\mathscr{T}_0$ の定理であるため、C31 による $(\exists x)(\forall y)R \Rightarrow (\exists x)R$ も同様です。 $(\exists x)(\forall y)R$ が真の場合、$(\exists x)R$ も真となり、従って $(\forall y)(\exists x)R$ も真になります。従って、3 番目の定理です。

一方、$(\forall y)(\exists x)R$ が $\mathscr{T}$ の定理である場合、$(\exists x)(\forall y)R$ が $\mathscr{T}$ の定理であることは結論するではない可能性があります。 直観的には、関係 $(\forall y)(\exists x)R$ が真であるということは、任意のオブジェクト $y$ が与えられた場合、オブジェクト $x$ と $y$ の間に $R$ が真関係となるようなオブジェクト $x$ が存在することを意味します。 しかし、一般に、オブジェクト $x$ はオブジェクト $y$ の選択に依存しますが、$(\exists x)(\forall y)R$ が true であるということは、このオブジェクトと *任意の* オブジェクト $y$ の間に $R$ が真関係となるような *固定* オブジェクト $x$ が存在することを意味します。

### 4. 典型的な量指定子

$A$ と $R$ をアセンブリ、$x$ を文字とします。アセンブリ $(\exists x)(A$ と R) を $(\exists_A x)R$ で表し、アセンブリ

$$\text{“not } (\exists_A x) \text{ (not } R)\text{”}$$

$(\forall_A x)R$ によって。省略記号 $\exists_A$ と $\forall_A$ は *典型的な数量詞* と呼ばれます。 $(\exists_A x)R$、$(\forall_A x)R$ で示されるアセンブリには文字 $x$ が表示されないことに注意してください。

CS10。 *$A$と$R$をアセンブリ、$x$と$x'$を文字とします。 $x$ が $R$ にも $A$ にも現れない場合、$(\exists_A x)R$ と $(\forall_A x)R$ はそれぞれ$(\exists_{A'} x')R'$ と $(\forall_{A'} x')R'$ と同一になります。ここで、$R'$ は $(x'|x)R$ で、$A'$ は$(x'|x)A$.*

CS11。 *$A$、$R$、$U$ をアセンブリとし、$x$、$y$ を個別の文字とします。 $x$ が $U$ に現れない場合、アセンブリ $(U|y)(\exists_A x)R$ と $(U|y)(\forall_A x)R$ はそれぞれ $(\exists_{A'} x')R'$ と $(\forall_{A'} x')R'$ と同一になります。ここで、$R'$ は $(U|y)R$ で、$A'$ は $(U|y)A$ です*。

これらのルールは、基準 CS8、CS9 (no. 1)、CS5 (§ 1, no. 2)、および CS6 (§ 3, no. 4) の明らか帰結です。

CF12。 ※$A$と$R$を$\mathscr{T}$の関係とし、$x$を文字とします。それから*

$$(\exists_A x)R \quad \text{and} \quad (\forall_A x)R$$

*は $\mathscr{T}$ の関係です。*

これは、CF11 (no. 1)、CF9 (§ 3, no. 4)、CF2 (§ 1, no. 4) から直接続きます。

直感的には、$A$ と $R$ が $x$ のプロパティを表現していると考えてください。 証明の系列では、満たす $A$ のオブジェクトのみに関心があることが起こります。 $R$ のようなオブジェクト満たす $A$ が存在すると言うことは、「$A$ と $R$」のようなオブジェクトが存在することを意味します。 よって定義/$\exists_A$。 満たす $A$ が性質 $R$ を持つすべてのオブジェクトは、「$R$ ではない」オブジェクト満たす $A$ が存在しないことを意味します。 よって定義/$\forall_A$。実際には、これらの記号は、関係 $A$ の性質に応じて、さまざまなフレーズに置き換えられます。 \* 例: "すべての整数 $x$, $R$"; 「$R$となるような集合Eの元$x$が存在します。」;等々。 \*

C35。 ※$A$と$R$を$\mathscr{T}$の関係、$x$を文字とします。その場合、関係 $(\forall_A x)R$ と $(\forall x)(A \Rightarrow R)$ は $\mathscr{T}$ で等価です。*

関係の場合、$(\forall_A x)R$ は以下と同じです

$$\text{"not}(\exists x)(A \text{ and } (\text{not } R))\text{"}.$$

ここで、「$A$ と ($R$ ではない)」は、$\mathscr{T}_0$ では「$(A \Rightarrow R)$ ではない」と同等です。従って、「$(\exists x)(A$ ではなく、($R$ ではない))」は、$\mathscr{T}_0$ では次と同等です。

$$\text{"not } (\exists x)(\text{not } (A \Rightarrow R))\text{"},$$

C31 (no. 3) で、後者の関係は$(\forall x)(A \Rightarrow R)$ と同一です。従って、基準は $\mathscr{T}_0$ で確立され、その結果、 $\mathscr{T}$ で確立されます。

私たちはしばしば、形 $(\forall_A x)R$ の関係を証明しなければなりません。一般に、次の 2 つの基準のいずれかを使用します。

C36. ※$A$と$R$を$\mathscr{T}$の関係、$x$を文字とします。 $\mathscr{T}'$ を $\mathscr{T}$ の公理に $A$ を隣接させて得られる理論とします。 $x$ が $\mathscr{T}$ の定数ではなく、$R$ が $\mathscr{T}'$ の定理である場合、$(\forall_A x)R$ は $\mathscr{T}$ の定理になります。*

$A \Rightarrow R$ は、減算基準により、$\mathscr{T}$ の定理であるため、C27 (no. 1) と C35 により、$(\forall_A x)R$ は、$\mathscr{T}$ の定理となります。

実際には、「$x$ を $A$ のような任意の元にしましょう」のようなフレーズによってこのルールを使用することを示します。このように定義された理論 $\mathscr{T}'$ において、$R$ を証明しようとします。もちろん、できないは、$R$自体が$\mathscr{T}$の定理であると主張します。

C37. ※$A$と$R$を$\mathscr{T}$の関係とし、$x$を文字とします。 $\mathscr{T}'$ を関係 $A$ に隣接させて得られる理論とし、$\mathscr{T}$ の公理に「$R$ ではない」とします。 $x$ が $\mathscr{T}$ の定数ではなく、$\mathscr{T}'$ が矛盾する場合、$(\forall_A x)R$ は $\mathscr{T}$ の定理になります。

理論の場合、$\mathscr{T}'$ は、$\mathscr{T}$ の公理に「$(A \Rightarrow R)$ ではない」を隣接させることで得られる理論と等価です。 *reductio ad absurdum* の方法により、$A \Rightarrow R$ は $\mathscr{T}$ の定理となり、したがって C27 (no. 1) と C35 により $(\forall_A x)R$ も同様になります。

実際には、「$R$ が偽であるオブジェクト $x$ 満たす $A$ が存在すると仮定します」と言い、矛盾を確立しようとします。

一般的な量指定子のプロパティは、量指定子の特性と類似しています。

C38。 ※$A$と$R$を$\mathscr{T}$の関係とし、$x$を文字とします。それでは関係*

$$\text{not } (\forall_A x)R \Leftrightarrow (\exists_A x)(\text{not } R),$$
$$\text{not } (\exists_A x)R \Leftrightarrow (\forall_A x)(\text{not } R)$$

*は定理は $\mathscr{T}$ です。*

C39. ※$A$、$R$、$S$は$\mathscr{T}$の関係、$x$は$\mathscr{T}$の定数ではない文字とします。 関係 $A \Rightarrow (R \Rightarrow S)$ [それぞれ$A \Rightarrow (R \Leftrightarrow S)$] は $\mathscr{T}$ の定理、その後関係*

$$(\exists_A x)R \Rightarrow (\exists_A x)S, \qquad (\forall_A x)R \Rightarrow (\forall_A x)S$$
$$[\text{resp. } (\exists_A x)R \Leftrightarrow (\exists_A x)S, \qquad (\forall_A x)R \Leftrightarrow (\forall_A x)S]$$

*は定理は $\mathscr{T}$ です。*

C40。 ※$\mathscr{T}$の$A$、$R$、$S$を関係、$x$を文字とします。それでは関係*

$$(\forall_A x)(R \text{ and } S) \Leftrightarrow ((\forall_A x)R \text{ and } (\forall_A x)S),$$
$$(\exists_A x)(R \text{ or } S) \Leftrightarrow ((\exists_A x)R \text{ or } (\exists_A x)S)$$

*は $\mathscr{T}$ の定理です。*

C41. ※$A$、$R$、$S$は$\mathscr{T}$の関係、$x$は$R$に出てこない文字とします。それでは関係*

$$(\forall_A x)(R \text{ or } S) \Leftrightarrow (R \text{ or } (\forall_A x)S),$$
$$(\exists_A x)(R \text{ and } S) \Leftrightarrow (R \text{ and } (\exists_A x)S)$$

*は $\mathscr{T}$ の定理です。*

C42。 ※$\mathscr{T}$の$A$、$B$、$R$を関係とし、$x$と$y$を文字とします。 $B$に$x$が現れず、$A$に$y$が現れない場合、関係*

$$(\forall_A x)(\forall_B y)R \Leftrightarrow (\forall_B y)(\forall_A x)R,$$
$$(\exists_A)x(\exists_B y)R \Leftrightarrow (\exists_B y)(\exists_A x)R,$$
$$(\exists_A x)(\forall_B y)R \Rightarrow (\forall_B y)(\exists_A x)R$$

*は $\mathscr{T}$ の定理です。*

例を使って、C42の部分を証明しましょう。 関係

$$(\exists_A x)(\exists_B y) R$$

は $(\exists x)(A$、$(\exists y)(B$、$R))$ と同一であるため、($y$ は $A$ には現れないため) $\mathscr{T}_0$ では以下と同等です。

$$(\exists x)(\exists y)(A \text{ and } (B \text{ and } R))$$

C33とC31による。同様に、$(\exists_B x)(\exists_A y)R$ は次と同等です。

$$(\exists y)(\exists x)(B \text{ and } (A \text{ and } R)).$$

次に、C31 と C34 (no. 3) を適用します。

\* これらの基準の適用の例として、次の関係を考慮してください。「実数値写像 $(f_n)$ の数列は、$[0, 1]$ で一様に 0 に収束します」。これは、「各 $\varepsilon > 0$ に対して整数 $n$ が存在し、各 $x \in [0, 1]$ と各整数 $m \geqslant n$ に対して $|f_m(x)| \leqslant \varepsilon$ が存在する」ことを意味します。この関係の否定を取りたいとします (たとえば、矛盾によって証明を取得するため)。基準 C38 は、この否定が次の関係と同等であることを示しています。「それぞれの整数 $n$ に対して $x \in [0, 1]$ と $m \geqslant n$ が存在するような $\varepsilon > 0$ が存在し、それに対して $|f_m(x)| > \varepsilon$ が存在する」。

### 練習問題 {#ens-i-s4-exercises}

*合計練習問題 for* § 4、$\mathscr{T}$ *は定量化された理論を表します。

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
