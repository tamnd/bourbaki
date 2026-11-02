---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 5
section_title: Product of a family of sets
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 101-112, 127
pdf_pages: 0108-0119, 0134-0134
extraction: ocr
subsections:
    - "no": 1
      title: THE AXIOM OF THE SET OF SUBSETS
      page: 101
      pdf_page: 108
    - "no": 2
      title: SET OF MAPPINGS OF ONE SET INTO ANOTHER
      page: 102
      pdf_page: 109
    - "no": 3
      title: DEFINITIONS OF THE PRODUCT OF A FAMILY OF SETS
      page: 103
      pdf_page: 110
    - "no": 4
      title: PARTIAL PRODUCTS
      page: 105
      pdf_page: 112
    - "no": 5
      title: ASSOCIATIVITY OF PRODUCTS OF SETS
      page: 106
      pdf_page: 113
    - "no": 6
      title: DISTRIBUTIVITY FORMULAE
      page: 107
      pdf_page: 114
    - "no": 7
      title: EXTENSION OF MAPPINGS TO PRODUCTS
      page: 111
      pdf_page: 118
statements: 24
exercises: 3
errata:
    - says: Proposition 1, Corollary 5
      read: Proposition 6, Corollary 1
      why: Section 5 prints five corollaries in no. 4 and all five stand under Proposition 6, which is on page 105 and is the auxiliary the no. announces with "it is enough to prove the following proposition". Proposition 1 has no corollary at all, so there is no Corollary 5 of it. The sentence citing this, on page 106, needs the projection of a product onto a factor to be surjective, and that is Corollary 1 of Proposition 6, whose proof reads "Apply Proposition 5 to the subset J = {alpha} of I".
    - says: Proposition 5, Corollary 2
      read: Proposition 6, Corollary 2
      why: The volume hangs these five corollaries on Proposition 5 four times over and on Proposition 6 once, and the page prints them under Proposition 6. The fact wanted in both sentences here, on pages 108 and 109, is that a product is empty exactly when one of its factors is, which is Corollary 2. Proposition 5 is the statement about a partial product that the proof of Corollary 1 applies, and it carries no corollary of its own.
    - says: Corollary 2 to Proposition 5
      read: Corollary 2 to Proposition 6
      why: The same reference as the two above, written the other way round on page 109, and wrong the same way.
content_sha256: 2abc6fba69258404fbfc49fec4a6d731aa4c741d33ffc11e88ce92e93949ad2c
translated_from: content/en/ens/II/05_s5_product_of_a_family_of_sets.md
translation_method: google
source_content_sha256: 0301ddc64f4634b2f737e77987e840c82975f71ef423fb30f170e6510997d48c
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 250a8d4114255479915dcb6c7e258a8825839d877a0ae454b0abe5e874dc004f
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 5. 集合人の家族の積

### 1. 部分集合の集合の公理

A4. $(\forall \mathrm{X}) \ \mathrm{Coll}_{\mathrm{Y}}(\mathrm{Y} \subset \mathrm{X}).$

この公理は、すべての集合 X に対して集合が存在し、その元はすべて X の部分集合、つまり集合 $\mathscr{E}_{\mathrm{Y}}(\mathrm{Y} \subset \mathrm{X})$ (§1, no. 4) であることを意味します。この集合は$\mathfrak{P}(\mathrm{X})$で示され、*Xの*部分集合の*集合と呼ばれます。明らかに、$\mathrm{X} \subset \mathrm{X}'$ であれば、$\mathfrak{P}(\mathrm{X}) \subset \mathfrak{P}(\mathrm{X}')$ があります。

¶ A、B を 2 つの集合とし、A と B の間の $\Gamma$ を対応とします。 *写像* $\mathrm{X} \to \Gamma \langle \mathrm{X} \rangle$ $(\mathrm{X} \subset \mathfrak{P}(\mathrm{A}), \ \Gamma \langle \mathrm{X} \rangle \in \mathfrak{P}(\mathrm{B}))$ を *標準拡大* (または単に *拡大*) と呼びます* $\Gamma$ * 部分集合* の集合は $\hat{\Gamma}$ で示されます。 $\mathfrak{P}(\mathrm{A})$の$\mathfrak{P}(\mathrm{B})$の写像です。 Bと集合Cの間の$\Gamma'$が対応である場合、公式$(\Gamma' \circ \Gamma) \langle \mathrm{X} \rangle = \Gamma' \langle \Gamma \langle \mathrm{X} \rangle \rangle$は、$\Gamma' \circ \Gamma$の拡大から部分集合の集合が写像であることを示します。 $\hat{\Gamma}' \circ \hat{\Gamma}$。

#### 命題 1 {#ens-ii-s5-prop-1 .statement tag=03IJ}

(1) *もし* $f$ * が集合* E * 集合* F への全射である場合、 *標準拡大* $\hat{f}$ *of* $f$ *は $\mathfrak{P}(\mathrm{E})$ * へ* $\mathfrak{P}(\mathrm{F})$ の全射である。

(2) *もし* $f$ *が単射 of* E *into* F、*標準拡大* $\hat{f}$ *of* $f$ *は単射 of* $\mathfrak{P}(\mathrm{E})$ *into* $\mathfrak{P}(\mathrm{F})$。

(1) $s$ が $f$ の切断である場合、$f \circ s$ は F の恒等写像であるため、$\hat{f} \circ \hat{s}$ は $\mathfrak{P}(\mathrm{F})$ の恒等写像です。したがって、$\hat{f}$ は全射法であり、$\hat{s}$ は $\hat{f}$ (§3, no. 8) の切断です。

(2) $E = \varnothing$ であれば、$\mathfrak{P}(E) = \{\varnothing\}$ なので、命題は明らかです。 $E \ne \varnothing$ で、$r$ が $f$ の撤回である場合、$r \circ f$ は $E$ の恒等写像であるため、$\hat{r} \circ \hat{f}$ は $\mathfrak{P}(E)$ の恒等写像になります。したがって、$\hat{f}$ は単射法であり、$\hat{r}$ は $\hat{f}$ (§3, no. 8) の撤回です。

### 2. 1 つの集合を他のに写像の集合

$E$、$F$を集合とします。 $E$の写像を$F$に入れるグラフは、$E \times F$の部分集合です。 $E$の写像を$F$にグラフ化した性質を持つ$\mathfrak{P}(E \times F)$の元の集合は、$\mathfrak{P}(E \times F)$の部分集合であり、$F^E$で表されます。 The set of triples $f = (G, E, F)$, where $G \in F^E$, is therefore the set of mappings of $E$ into $F$; it is denoted by $\mathfrak{F}(E, F)$. 明らかに、$G \mapsto (G, E, F)$ は $\mathfrak{F}(E, F)$ 上の $F^E$ の全単射 (正規の全単射と呼ばれます) です。 この全単射の存在により、集合 $F^E$ に関連するすべての命題を $\mathfrak{F}(E, F)$ に関連するものに即座に変換でき、またその逆も可能です。

¶ $E$、$E'$、$F$、$F'$ を集合とします。 $u$ を $E'$ の写像から $E$ に、$v$ を $F$ の写像から $F'$ にします。すると、写像 $f \mapsto v \circ f \circ u$ は、$\mathfrak{F}(E, F)$ の写像が $\mathfrak{F}(E', F')$ になります。

#### 命題 2 {#ens-ii-s5-prop-2 .statement tag=03Q5}

(1) *If $u$ is a surjection of $E'$ onto $E$ and $v$ an injection of $F$ into $F'$, then the mapping $f \mapsto v \circ f \circ u$ is injective.*

(2) *$u$ が $E'$ の $E$ への単射であり、$v$ が $F'$ への $F$ の全射である場合、写像 $f \mapsto v \circ f \circ u$ は全射です。

集合 $E$、$E'$、$F$、$F'$ はすべて空ではないと仮定します。そうでない場合、命題は自明に検証されます。

(1) $s$ を $u$ の切断とし、$r$ を $v$ (§3、定義 11) の撤回とします。次に $r \circ (v \circ f \circ u) \circ s = I_F \circ f \circ I_E = f$ なので、

$$
f \mapsto v \circ f \circ u
$$

は単射です。

(2) $r'$を$u$の撤回とし、$s'$を$v$の切断とする。すべての写像 $f' : E' \to F'$ に対して $v \circ (s' \circ f' \circ r') \circ u = f'$ があり、写像 $f \mapsto v \circ f \circ u$ が全射であることを示しています。

#### 系 {#ens-ii-s5-n2-cor-1 .statement tag=03Q6}

*$u$ が $E$ に対する $E'$ の全単射であり、$v$ が $F'$ に対する $F$ の全単射である場合、$f \mapsto v \circ f \circ u$ は全単射です。

$A$、$B$、$C$を3つの集合とし、$f$を$B \times C$の写像を$A$とします。 すべての $y \in C$ について、$f(\mathord{\cdot}, y)$ を $B$ の部分写像 $x \mapsto f(x,y)$ を $A$ (§ 3, no. 9) に変換します。 写像 $y \mapsto f(\mathord{\cdot}, y)$ は、$C$ の写像が $\mathfrak{F}(B, A)$ になります。 逆に、$C$ の $\mathfrak{F}(B, A)$ へのすべての写像 $g$ に対して、A への $\mathrm{B} \times \mathrm{C}$ の一意な写像 $f$ が存在し、それぞれの $y \in \mathrm{C}$ に対して $g(y) = f(\bullet, y)$、つまり写像 $(x, y) \to (g(y))(x)$ が存在します。 したがって、次のようになります。

#### 命題 3 {#ens-ii-s5-prop-3 .statement tag=03Q7}

** $\mathrm{B} \times \mathrm{C}$ *into* A のすべての写像 $f$ を * C *into* $\mathfrak{F}(\mathrm{B}, \mathrm{A})$ の $\tilde{f}$ 写像 $y \to f(\bullet, y)$ で表す場合、*その後写像 $f \to \tilde{f}$ は次のようになります全単射* (*標準全単射* と呼ばれます) *の* $\mathfrak{F}(\mathrm{B} \times \mathrm{C}, \mathrm{A})$ *上に* $\mathfrak{F}(\mathrm{C}, \mathfrak{F}(\mathrm{B}, \mathrm{A}))$。

同様に、$\mathfrak{F}(\mathrm{B} \times \mathrm{C}, \mathrm{A})$ の *標準的な全単射* を $\mathfrak{F}(\mathrm{B}, \mathfrak{F}(\mathrm{C}, \mathrm{A}))$ に定義する変換します。 写像と関数グラフの間の 1 対 1 の対応により、これらの全単射は、$\mathrm{A}^{\mathrm{B} \times \mathrm{C}}$ の *正準全単射* を $(\mathrm{A}^{\mathrm{B}})^{\mathrm{C}}$ (それぞれ $(\mathrm{A}^{\mathrm{C}})^{\mathrm{B}}$) に生じさせます。

### 3. 集合人家族の積のうち定義

$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ を集合の族とし、F を $\iota \in \mathrm{I}$ ごとに $\mathrm{F}(\iota) \in \mathrm{X}_\iota$ となるようなドメイン I を持つ関数グラフとする。 次に、各 $\iota \in \mathrm{I}$ に対して $\mathrm{F}(\iota) \in \mathrm{A} = \bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ があり、したがって F は $\mathfrak{P}(\mathrm{I} \times \mathrm{A})$ の元になります。 上記の性質を持つ関数グラフは、$\mathfrak{P}(\mathrm{I} \times \mathrm{A})$の形部分集合になります。

#### 定義 1 {#ens-ii-s5-def-1 .statement tag=03Q8}

※$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$を集合の家族とします。関数グラフの集合 F *ドメイン* I *そのような* $\mathrm{F}(\iota) \in \mathrm{X}_\iota$ *それぞれ* $\iota \in \mathrm{I}$ *は、集合 $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ の族の積と呼ばれ、* $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ で表されます。 *それぞれ* $\iota \in \mathrm{I}$、$\mathrm{X}_\iota$ *は積* $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ の添字 $\iota$ の因子と呼ばれます。 *写像* $\mathrm{F} \to \mathrm{F}(\iota)$ $\left( \mathrm{F} \in \prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota,\ \mathrm{F}(\iota) \in \mathrm{X}_\iota \right)$ *添字 $\iota$ の座標写像* (または *射影*) と呼ばれ、* $\mathrm{pr}_\iota$ で表されます。

$\mathrm{F}(\iota)$ is called the *coordinate of index* $\iota$ (or *projection of index* $\iota$) of F; the image $\mathrm{pr}_\iota\langle \mathrm{A} \rangle$ of a subset A of $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ under the coordinate function of index $\iota$ is called the *projection of index* $\iota$ of A. $\mathrm{A} \subset \prod_{\iota \in \mathrm{I}} \mathrm{pr}_\iota \langle \mathrm{A} \rangle$ であることは簡単に確認できます。

$\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ (§3, no. 6) の元を表すには、記法 $(x_\iota)_{\iota \in \mathrm{I}}$ をよく使用します。

$\mathrm{I} = \emptyset$ の場合、集合 $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ には元が 1 つだけあります。つまり、空の集合 (§3, no. 4、例 1) です。

¶ 積 $\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ のすべての因子 $\mathrm{X}_\iota$ が同じ集合 E に等しい場合、$\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota = \mathrm{E}^{\mathrm{I}}$ が得られます。これは定義の直後に続きます。

¶ $(X_\iota)_{\iota \in I}$ が集合の任意の族であり、E が次のような集合である場合

$$\bigcup_{\iota \in I} X_\iota \subset E,$$

次に、定義 1 は $\prod_{\iota \in I} X_\iota \subset E^I$ を示します。したがって、$\prod_{\iota \in I} X_\iota$とIの写像の集合の間には1対1の対応が存在します（つまり、$\mathfrak{F}(I, E)$の部分集合）。

¶ $I = \{\alpha\}$ が 1 つの元の集合からなるである場合、次のようになります。

$$\prod_{\iota \in I} X_\iota = X_\alpha^{\{\alpha\}};$$

写像 $F \to F(\alpha)$ は、$\prod_{\iota \in \{\alpha\}} X_\iota$ の $X_\alpha$ 上の全単射 (*正規* と呼ばれます) になります。

¶ A、B を集合とし、$\alpha$、$\beta$ を別個のオブジェクトとします (2 つの別個のオブジェクト、たとえば $\emptyset$ と $\{\emptyset\}$ が存在します)。グラフ $\{(\alpha, A), (\beta, B)\}$ を考えてみましょう。これは明らかに機能しており、まさに $X_\alpha = A$ や $X_\beta = B$ などのファミリー $(X_\iota)_{\iota \in \{\alpha, \beta\}}$ です。それぞれの対 $(x, y) \in A \times B$ について、$f_{x,y}$ を関数グラフ $\{(\alpha, x), (\beta, y)\}$ とします。 写像 $(x, y) \to f_{x,y}$ が $A \times B$ から $\prod_{\iota \in \{\alpha, \beta\}} X_\iota$ への全単射写像であることは明らかです。この全単射の逆数は$g \to (g(\alpha), g(\beta))$です。これら 2 つの全単射は *正規* と呼ばれます。以下では、この 1 対 1 対応を使用して、集合の族の積の特性から 2 つの集合の積の特性を推定します。

¶ $(X_\iota)_{\iota \in I}$ を、それぞれが 1 つの元、たとえば $X_\iota = \{a_\iota\}$ で構成される集合のファミリーとします。その場合、積 $\prod_{\iota \in I} X_\iota$ は、シングル元 $(a_\iota)_{\iota \in I}$ の集合からなるになります。

¶ Eを集合とします。 I の *定数* 写像 $\iota \to x$ を E 形部分集合 $\Delta$ の積 $E^I$ に変換するグラフは、*対角* と呼ばれます。 $\bar{x}$ が写像 $\iota \to x$ ($x \in E$) のグラフを表す場合、写像 $x \to \bar{x}$ は、$\Delta$ 上の E の全単射であり、*対角線写像* と呼ばれます。

#### 命題 4 {#ens-ii-s5-prop-4 .statement tag=03IK}

*$(X_\iota)_{\iota \in I}$ * を集合の家族とし、あなたを集合* K * の全単射として、添字集合* I とします。 *もし* U *がuのグラフであれば、 写像* $F \to F \circ U$ *of* $\prod_{\iota \in I} X_\iota$ *into* $\prod_{x \in K} X_{u(x)}$ *は全単射*です。

させて

$$A = \bigcup_{\iota \in I} X_\iota = \bigcup_{x \in K} X_{u(x)}$$

(§4、命題1)。 写像 $F\to F\circ U$ ($F\in A^I$) は、$A^I$ の全単射を $A^K$ (命題 2) に加えたものです。 条件「$\iota\in I$、$F(\iota)\in X_\iota$ ごと」が「$x\in K$、$(F\circ U)(x)\in X_{u(x)}$ ごと」と同等であることは明らかであり、結果は次のとおりです。

### 4. 部分的積

$(X_\iota)_{\iota\in I}$ を集合の家族とし、$J$ を $I$ の部分集合とします。 積 $\displaystyle\prod_{\iota\in J}X_\iota$ は、$\displaystyle\prod_{\iota\in I}X_\iota$ の *部分積* と呼ばれます。 $f$ が写像で、グラフ $F$ が $\displaystyle\prod_{\iota\in I}X_\iota$ のメンバーである場合、$F\circ\Delta_J$ ($\Delta_J$ は $J\times J$ の対角) は、$f$ から $J$ の *制限* のグラフです。明らかに$F\circ\Delta_J\in\displaystyle\prod_{\iota\in J}X_\iota$; $\displaystyle\prod_{\iota\in I}X_\iota$ の $\displaystyle\prod_{\iota\in J}X_\iota$ への写像 $F\to F\circ\Delta_J$ は、添字* $J$ の *射影と呼ばれ、$\operatorname{pr}_J$ で表されます。

#### 命題 5 {#ens-ii-s5-prop-5 .statement tag=03Q9}

*$(X_\iota)_{\iota\in I}$を集合の家族とし、$J$を$I$の部分集合とします。それぞれの $\iota\in I$ に $X_\iota\ne\varnothing$ がある場合、射影 $\operatorname{pr}_J$ は $\displaystyle\prod_{\iota\in I}X_\iota$ の写像から $\displaystyle\prod_{\iota\in J}X_\iota$ になります。*

上記で作成した注意を考慮すると、次の命題を証明するだけで十分です。

#### 命題 6 {#ens-ii-s5-prop-6 .statement tag=03QA}

*$(X_\iota)_{\iota\in I}$ を、すべての $\iota\in I$ に対して $X_\iota\ne\varnothing$ となるような集合の家族とします。 If $g$ is a mapping of $J\subset I$ into $A=\displaystyle\bigcup_{\iota\in I}X_\iota$, such that $g(\iota)\in X_\iota$ for all $\iota\in J$, then there exists an extension $f$ of $g$ to $I$ such that $f(\iota)\in X_\iota$ for all $\iota\in I$.*

それぞれの $\iota\in I-J$ について、$T_\iota$ は項 $\tau_\iota(y\in X_\iota)$ を表します。 仮定までに$X_\iota\ne\varnothing$なので、すべての$\iota\in I-J$ (章 I, §4, no. 1) に対して$T_\iota\in X_\iota$ になります。 $G$ が $g$ のグラフである場合、グラフ $G\cup\left(\displaystyle\bigcup_{\iota\in I-J}\{(\iota,T_\iota)\}\right)$ は、すぐに検証できるように、必要な特性を備えた写像のグラフです。

#### 系 1 {#ens-ii-s5-prop-6-cor-1 .statement tag=03QB}

*$(X_\iota)_{\iota\in I}$ を、$\iota\in I$ ごとに $X_\iota\ne\varnothing$ が存在するように、集合の家族とします。次に、各 $\alpha\in I$ 射影 $\operatorname{pr}_\alpha$ は、$\displaystyle\prod_{\iota\in I}X_\iota$ の写像が $X_\alpha$ になります。*

命題を適用する 5 から $I$ の部分集合 $J=\{\alpha\}$ に、$\operatorname{pr}_\alpha$ が $X_\alpha^{\{\alpha\}}$ の標準写像の合成から $X_\alpha$ と写像 $\operatorname{pr}_{\{\alpha\}}$ であることに注意してください。

#### 系 2 {#ens-ii-s5-prop-6-cor-2 .statement tag=03QC}

※$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$を集合の家族とします。次に、$\mathrm{X}_\iota = \emptyset$ となるような $\iota \in \mathrm{I}$ が存在する場合に限り、$\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota = \emptyset$ となります。*

それぞれの $\iota \in \mathrm{I}$ に $\mathrm{X}_\iota \neq \emptyset$ がある場合、系 1 から $\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota \neq \emptyset$ が得られます。逆に、$\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota \neq \emptyset$ の場合、関係 $\mathrm{pr}_\alpha\Big(\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota\Big) \subset \mathrm{X}_\alpha$ は、$\alpha \in \mathrm{I}$ ごとに $\mathrm{X}_\alpha \neq \emptyset$ を示します。

したがって、空ではない集合の族 $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ がある場合、すべての $\iota \in \mathrm{I}$ に対して $f(\iota) \in \mathrm{X}_\iota$ となるように、ドメイン I を持つ (補助定数として) 写像 $f$ を導入できます。実際には、「各 $\mathrm{X}_\iota$ に元 $x_\iota$ を取る」と言います。したがって、直感的に、私たちはそれぞれの集合 $\mathrm{X}_\iota$ で元 $x_\iota$ を「選択」しました。論理記号 $\tau$ とその使用を管理する基準の導入により、この演算を合法化するための「選択の公理」を定式化する必要がなくなりました (cf. 結果の要約、§4, no. 10)。

#### 系 3 {#ens-ii-s5-prop-6-cor-3 .statement tag=03QD}

*$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ と $(\mathrm{Y}_\iota)_{\iota \in \mathrm{I}}$ を、同じ添字集合 I を持つ 2 つの集合ファミリーとします。 $\iota \in \mathrm{I}$ ごとに $\mathrm{X}_\iota \subset \mathrm{Y}_\iota$ の場合、*

$$\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota \subset \prod_{\iota \in \mathrm{I}} \mathrm{Y}_\iota.$$

*逆に、$\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota \subset \prod\limits_{\iota \in \mathrm{I}} \mathrm{Y}_\iota$ の場合、および $\iota \in \mathrm{I}$ ごとに $\mathrm{X}_\iota \neq \emptyset$ の場合、$\iota \in \mathrm{I}$ ごとに $\mathrm{X}_\iota \subset \mathrm{Y}_\iota$ になります。

最初の主張は明白で、2 番目は命題 1、系 5 から続きます。なぜなら、各 $\alpha \in \mathrm{I}$ について、

$$\mathrm{X}_\alpha = \mathrm{pr}_\alpha\Big(\prod_{\iota \in \mathrm{I}} \mathrm{X}_\iota\Big) \subset \mathrm{pr}_\alpha\Big(\prod_{\iota \in \mathrm{I}} \mathrm{Y}_\iota\Big) = \mathrm{Y}_\alpha.$$

### 5. 集合の積の結合性

#### 命題 7 {#ens-ii-s5-prop-7 .statement tag=03IN}

*$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ を、添字集合 I が空の集合ではない集合の家族とする。 $(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$をIの分割とします。それでは写像*

$$f \to (\mathrm{pr}_{\mathrm{J}_\lambda} f)_{\lambda \in \mathrm{L}}$$

*$\prod\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ の積集合 $\prod\limits_{\lambda \in \mathrm{L}} \Big(\prod\limits_{\iota \in \mathrm{J}_\lambda} \mathrm{X}_\iota\Big)$ は全単射です (集合の積の「結合性」)。

From the interpretation of $\mathrm{pr}_{\mathrm{J}_\lambda} f$ as the graph of the restriction of the function whose graph is $f$ (no. 4), it follows that the statement that the mapping $f \to (\mathrm{pr}_{\mathrm{J}_\lambda} f)_{\lambda \in \mathrm{L}}$ is bijective means that, for each family $(v_\lambda)_{\lambda \in \mathrm{L}}$, where $v_\lambda$ is a mapping of $\mathrm{J}_\lambda$ into $\bigcup\limits_{\iota \in \mathrm{I}} \mathrm{X}_\iota$, there exists a unique mapping $u$ of I into $\bigcup_{\iota \in I} X_\iota$ such that $v_\lambda$ is the restriction of $u$ to $J_\lambda$ for each $\lambda \in L$. But this is a consequence of the hypothesis that $(J_\lambda)_{\lambda \in L}$ is a partition of I (§4, Proposition 8).

¶ 命題 7 で定義された全単射とその逆全単射は *正規* と言われます。

*注意*

#### 注意 1 {#ens-ii-s5-n5-rem-1 .statement tag=03SA}

$\alpha$、$\beta$ を 2 つの異なるオブジェクトとし、$(J_\lambda)_{\lambda \in \{\alpha, \beta\}}$ を I の分割を 2 つの集合 $J_\alpha$、$J_\beta$ にします。 したがって、$\prod_{\lambda \in \{\alpha, \beta\}} \left( \prod_{\iota \in J_\lambda} X_\iota \right)$の標準写像の合成を$\left( \prod_{\iota \in J_\alpha} X_\iota \right) \times \left( \prod_{\iota \in J_\beta} X_\iota \right)$に形成し、$\prod_{\iota \in I} X_\iota$の標準写像を$\left( \prod_{\iota \in J_\alpha} X_\iota \right) \times \left( \prod_{\iota \in J_\beta} X_\iota \right)$に形成することで、積$\prod_{\iota \in I} X_\iota$の1対1の写像（再び*標準*と呼ばれます）を取得します。 $\prod_{\lambda \in \{\alpha, \beta\}} \left( \prod_{\iota \in J_\lambda} X_\iota \right)$。 $X_\iota$ が各 $\iota \in J_\beta$ に対する *単一の元* の集合からなるである場合、$\mathrm{pr}_{J_\alpha}$ は $\prod_{\iota \in I} X_\iota$ から $\prod_{\iota \in J_\alpha} X_\iota$ への全単射写像です。

#### 注意 2 {#ens-ii-s5-n5-rem-2 .statement tag=03SB}

$\alpha$、$\beta$、$\gamma$ を 3 つのオブジェクトとし、そのうちの 2 つが等しいものはないとします (そのようなオブジェクトが 3 つ存在します。たとえば、$\emptyset$、$\{\emptyset\}$、$\{\{\emptyset\}\}$)、A、B、C を集合とします。関数グラフ $\{(\alpha, A), (\beta, B), (\gamma, C)\}$、つまり $X_\alpha = A$、$X_\beta = B$、$X_\gamma = C$ のような集合 $(X_\iota)_{\iota \in \{\alpha, \beta, \gamma\}}$ の族を考えてみましょう。 2 つの集合 $\{\alpha, \beta\}$ と $\{\gamma\}$ によって形成された $\{\alpha, \beta, \gamma\}$ の分割には、積に$\prod_{\iota \in \{\alpha, \beta, \gamma\}} X_\iota$ の正規の全単射が対応する存在します。

$$\left( \prod_{\iota \in \{\alpha, \beta\}} X_\iota \right) \times X_\gamma^{\{\gamma\}},$$

従って、$\prod_{\iota \in \{\alpha, \beta, \gamma\}} X_\iota$ の $A \times B \times C$ (§ 2, no. 2) への全単射 (再度 *canonical* と呼ばれます) は、変換それぞれ $f \in \prod_{\iota \in \{\alpha, \beta, \gamma\}} X_\iota$ から $A \times B \times C$ の元 $(f(\alpha), f(\beta), f(\gamma))$ にグラフ化されます。従って、命題 4 までに、6 つの集合 $A \times B \times C$、$B \times C \times A$、$C \times A \times B$、$B \times A \times C$、$A \times C \times B$、$C \times B \times A$ のうちの任意の 2 つを 1 対 1 の対応に入れることができます。

### 6. 分配率の公式

#### 命題 8 {#ens-ii-s5-prop-8 .statement tag=03IO}

*$((X_{\lambda,\iota})_{\iota \in J_\lambda})_{\lambda \in L}$ * 集合の家族の家族 (添字集合* L* と) としましょう。 * $L \neq \emptyset$ *と* $J_\lambda \neq \emptyset$ *それぞれ* $\lambda \in L$ だとします。 *しましょう*

$$I = \prod_{\lambda \in L} J_\lambda \neq \emptyset.$$

*それでは*

$$\bigcup_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right) = \bigcap_{f \in I} \left( \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)} \right),$$
$$\bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right) = \bigcup_{f \in I} \left( \bigcap_{\lambda \in L} X_{\lambda, f(\lambda)} \right)$$

(共通部分に対する和集合の「分配性」、および和集合に対する共通部分の「分配性」)。

$x$ を $\bigcup_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right)$ の元とし、$f$ を I のいずれかの元とします。 $x \in \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota}$ となるような添字 $\lambda$ が存在します。従って、$x \in X_{\lambda, f(\lambda)}$、従って

$$x \in \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)}.$$

これは各 $f \in I$ に当てはまるので、次のようになります。

$$x \in \bigcap_{f \in I} \left( \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)} \right).$$

逆に、$x$ を属するから集合にならないオブジェクトとする

$$\bigcup_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota} \right).$$

次に、各 $\lambda \in L$ には $x \notin \bigcap_{\iota \in J_\lambda} X_{\lambda, \iota}$ があり、これは、添字 $\iota \in J_\lambda$ の集合 $J'_\lambda$ が、各 $\lambda \in L$ に対して $x \notin X_{\lambda, \iota}$ が空にならないことを意味します。 命題 5、系 2 までに、ドメイン L を持つ関数グラフ $f$ が存在し、各 $\lambda \in L$ に対して $f(\lambda) \in J'_\lambda$ が得られます。従って、それぞれの $\lambda \in L$ に対して $f \in I$ と $x \notin X_{\lambda, f(\lambda)}$ が計算されます。従って

$$x \notin \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)}$$

従って

$$x \notin \bigcap_{f \in I} \left( \bigcup_{\lambda \in L} X_{\lambda, f(\lambda)} \right).$$

これで最初の公式の証明が完了しました。 2 番目の公式には、家族 $((\complement_A X_{\lambda, \iota})_{\iota \in J_\lambda})_{\lambda \in L}$ の最初の適用が続きます。ここで、A は和集合 $\bigcap_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_\lambda \right)$ を表します。

#### 系 {#ens-ii-s5-n6-cor-1 .statement tag=03IP}

*$(X_\iota)_{\iota \in I}$ * と* $(Y_\varkappa)_{\varkappa \in K}$ * を、空ではない添字集合* I を含む集合の 2 つの族とする、K. *次に*

$$\left( \bigcap_{\iota \in I} X_\iota \right) \cup \left( \bigcap_{\varkappa \in K} Y_\varkappa \right) = \bigcap_{(\iota,\, \varkappa) \in I \times K} (X_\iota \cup Y_\varkappa),$$
$$\left( \bigcup_{\iota \in I} X_\iota \right) \cap \left( \bigcup_{\varkappa \in K} Y_\varkappa \right) = \bigcup_{(\iota,\, \varkappa) \in I \times K} (X_\iota \cap Y_\varkappa).$$

$\alpha$、$\beta$ を 2 つの異なるオブジェクトとします。 命題 8 ($L = \{\alpha,\ \beta\}$、$J_\alpha = I$、$J_\beta = K$) の公式を $((Z_{\lambda,\, \mu})_{\mu \in J_\lambda})_{\lambda \in L}$ ファミリーに適用します。ここで、すべての $\iota \in I$ には $Z_{\alpha,\, \iota} = X_\iota$ が、各 $\varkappa \in K$ には $Z_{\beta,\, \varkappa} = Y_\varkappa$ が適用されます。 $\coprod_{\lambda \in L} J_\lambda$ の正規全単射が $I \times K$ (no. 3) に存在することにより、そして § 4 の命題 1 により、記載された式が得られます。

#### 命題 9 {#ens-ii-s5-prop-9 .statement tag=03IQ}

*$((X_{\lambda,\, \iota})_{\iota \in J_\lambda})_{\lambda \in L}$ * を (添字集合* L と) * 集合人の家族にしましょう。しましょう* $I = \prod_{\lambda \in L} J_\lambda$。 *それから*

$$\prod_{\lambda \in L} \left( \bigcup_{\iota \in J_\lambda} X_{\lambda,\, \iota} \right) = \bigcup_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right)$$

*そして (もし* $L \neq \emptyset$ *そして* $J_\lambda \neq \emptyset$ *それぞれ* $\lambda \in L$)

$$\prod_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda,\, \iota} \right) = \bigcap_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right)$$

(和集合以上、共通部分以上の積の「分配性」)。
最初の公式は、$L = \emptyset$ の場合、または一部の $\lambda \in L$ について $J_\lambda = \emptyset$ の場合、自明に true になります。そうでない場合は、$g$ を $\prod_{\lambda \in L} \left( \bigcap_{\iota \in J_\lambda} X_{\lambda,\, \iota} \right)$ の元とします。それぞれの $\lambda \in L$ には、$g(\lambda) \in X_{\lambda,\, \iota}$ となる添字 $\iota \in J_\lambda$ が存在します。他の語、集合 $H_\lambda$、添字 $\iota \in J_\lambda$ では、$g(\lambda) \in X_{\lambda,\, \iota}$ は空ではありません。従って、系 2 から命題 5 までには、次のようなドメイン L を持つ関数グラフ $f$ が存在します。

$$f(\lambda) \in H_\lambda$$

それぞれ $\lambda \in L$、つまり $g(\lambda) \in X_{\lambda,\, f(\lambda)}$ です。従って、$g \in \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)}$ があり、その結果、$g \in \bigcup_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right)$ になります。逆に、もし

$$g \in \bigcup_{f \in I} \left( \prod_{\lambda \in L} X_{\lambda,\, f(\lambda)} \right),$$

関数グラフ $f \in I$ があり、すべての $\lambda \in L$ について次のようになります。

$$g(\lambda) \in X_{\lambda,\, f(\lambda)}$$

そして、*なおさら*、$g(\lambda) \in \bigcup_{\iota \in J_\lambda} X_{\lambda, \iota}$。これで最初の公式の証明が完了します。 2 番目の公式の証明は類似していますが、より単純なので、読者に任せます。

#### 系 1 {#ens-ii-s5-prop-9-cor-1 .statement tag=03QE}

*$L \neq \emptyset$ *および* $J_\lambda \neq \emptyset$ *それぞれ* $\lambda \in L$ であるとします。 *各インデックス* $\lambda \in L$ *家族* $(X_{\lambda, \iota})_{\iota \in J_\lambda}$ *が* $X_\lambda = \bigcup_{\iota \in J_\lambda} X_{\lambda, \iota}$の分割である場合、*家族* $\left( \prod_{\lambda \in L} X_{\lambda, f(\lambda)} \right)_{f \in I}$ *は* $\prod_{\lambda \in L} X_\lambda$の分割です。

もし私たちが集合

$$\mathrm{P}_f = \prod_{\lambda \in L} X_{\lambda, f(\lambda)},$$

その場合、命題 9 の最初の公式により、すべての $f \in I$ について $\mathrm{P}_f \neq \emptyset$ が示され、$f$ と $g$ が I の元である場合は常に $\mathrm{P}_f \cap \mathrm{P}_g = \emptyset$ であることが示されれば十分です。最初の点は、命題 5、系 2 から続きます。2 番目については、$f \neq g$ の場合、次のような $\lambda \in L$ が存在します。

$$f(\lambda) \neq g(\lambda)$$

したがって、仮定、$X_{\lambda, f(\lambda)} \cap X_{\lambda, g(\lambda)} = \emptyset$ のおかげで。したがって、所属から $\mathrm{P}_f \cap \mathrm{P}_g$ までのグラフは存在しません。というのは、G がそのようなグラフであれば、$\mathrm{G}(\lambda) \in X_{\lambda, f(\lambda)} \cap X_{\lambda, g(\lambda)} = \emptyset$ が得られることになるが、これは不合理だからである。

#### 系 2 {#ens-ii-s5-prop-9-cor-2 .statement tag=03QF}

*$(X_\iota)_{\iota \in I}$ *と* $(Y_\varkappa)_{\varkappa \in K}$ *を集合の 2 つの家族としましょう。それから*

$$\left( \bigcup_{\iota \in I} X_\iota \right) \times \left( \bigcup_{\varkappa \in K} Y_\varkappa \right) = \bigcup_{(\iota, \varkappa) \in I \times K} (X_\iota \times Y_\varkappa)$$

*そして、* I *および* K *が空でない場合*

$$\left( \bigcap_{\iota \in I} X_\iota \right) \times \left( \bigcap_{\varkappa \in K} Y_\varkappa \right) = \bigcap_{(\iota, \varkappa) \in I \times K} (X_\iota \times Y_\varkappa).$$

証明は、系から命題 8 の証明のパターンに従います。

#### 命題 10 {#ens-ii-s5-prop-10 .statement tag=03QG}

*$(X_{\iota, \varkappa})_{(\iota, \varkappa) \in I \times K}$ *を集合の家族とし、その添字集合が 2 人のうちの積集合* I *と* K であるとします。 *もし* $K \neq \emptyset$ であれば、 *私たちは*

$$\bigcap_{\varkappa \in K} \left( \prod_{\iota \in I} X_{\iota, \varkappa} \right) = \prod_{\iota \in I} \left( \bigcap_{K \in \varkappa} X_{\iota, \varkappa} \right).$$

証明する等式の両辺は関数グラフです。 $\varkappa \in K$、$f \in \prod_{\iota \in I} X_{\iota, \varkappa}$ ごとに、グラフ $f$ 属するが左側に表示される場合に限ります。つまり、すべての $(\iota, \varkappa) \in I \times K$ に対して $f(\iota) \in X_{\iota, \varkappa}$ である場合に限ります。右辺の $f$ から属するについては、$\iota \in I$ ごとに $f(\iota) \in \bigcap_{\varkappa \in K} X_{\iota, \varkappa}$、つまり対 $(\iota, \varkappa) \in I \times K$ ごとに $f(\iota) \in X_{\iota, \varkappa}$ が必要かつ十分です。これで証明は完了です。

#### 系 {#ens-ii-s5-n6-cor-2 .statement tag=03IR}

*$(X_\iota)_{\iota \in I}$ * と* $(Y_\iota)_{\iota \in I}$ * を、同じ添字集合* $I \neq \emptyset$ を持つ 2 つの集合ファミリーとします。 *それから*

$$\Big(\prod_{\iota \in I} X_\iota\Big) \cap \Big(\prod_{\iota \in I} Y_\iota\Big) = \prod_{\iota \in I} (X_\iota \cap Y_\iota),$$
$$\Big(\bigcap_{\iota \in I} X_\iota\Big) \times \Big(\bigcap_{\iota \in I} Y_\iota\Big) = \bigcap_{\iota \in I} (X_\iota \times Y_\iota).$$

命題を適用する 10 は、K (それぞれ I) が 2 つの異なる元の集合からなるである場合に適用されます。

### 7. 写像から積の拡大

#### 定義 2 {#ens-ii-s5-def-2 .statement tag=03IS}

*$(X_\iota)_{\iota \in I}$、$(Y_\iota)_{\iota \in I}$ *を 2 つの集合の族とし、* $(g_\iota)_{\iota \in I}$ *同じ添字集合* I を *写像の族とする* $g_\iota$ *は写像* $X_\iota$ *に* $Y_\iota$ *それぞれ* $\iota \in I$。 *それぞれ* $f \in \prod_{\iota \in I} X_\iota$ * $u_f$ * を写像* $\iota = g_\iota(f(\iota))$ $(\iota \in I)$ のグラフにし、* $\prod_{\iota \in I} Y_\iota$ の元です。 *写像* $f \to u_f$ *の* $\prod_{\iota \in I} X_\iota$ *から* $\prod_{\iota \in I} Y_\iota$ *は、写像* $(g_\iota)_{\iota \in I}$の家族の積への標準拡大* (または単に*拡大*) と呼ばれます。 *写像* $(g_\iota)_{\iota \in I}$ の家族のときどきは積とも呼ばれます。

添字記法を使用すると、ファミリー $(g_\iota)_{\iota \in I}$ の積は写像 $(x_\iota)_{\iota \in I} \to (g_\iota(x_\iota))_{\iota \in I}$ になります。それは $(g_\iota)_{\iota \in I}$ で示されるときどきです。

$I = \{\alpha, \beta\}$ の場合、$\alpha$ と $\beta$ は別個であり、写像 $(g_\iota)_{\iota \in I}$ のファミリーの拡大から積は単なる $\psi \circ (g_\alpha \times g_\beta) \circ \varphi$ であり、$\varphi$ は$\prod_{\iota \in I} X_\iota$ の標準写像を表します。 $Y_\alpha \times Y_\beta$ の $X_\alpha \times X_\beta$ (no. 3) と $\psi$ 標準写像が $\prod_{\iota \in I} Y_\iota$ に。

#### 命題 11 {#ens-ii-s5-prop-11 .statement tag=03IT}

*$(X_\iota)_{\iota \in I}$、$(Y_\iota)_{\iota \in I}$、$(Z_\iota)_{\iota \in I}$ *を集合の 3 つの族とし、* $(g_\iota)_{\iota \in I}$、$(g'_\iota)_{\iota \in I}$ * 写像の 2 つの族とし、すべて同じ添字集合を持ち、* $g_\iota$ * は次のようになります。 写像 * $X_\iota$ *into* $Y_\iota$ *and* $g'_\iota$ *写像 of* $Y_\iota$ *into* $Z_\iota$、*それぞれ* $\iota \in I$。 *$g$ *と* $g'$ *家族の拡大* $(g_\iota)_{\iota \in I}$ *そして* $(g'_\iota)_{\iota \in I}$ *から積とします。すると、家族* $(g'_\iota \circ g_\iota)_{\iota \in I}$ の拡大 *から積は、* $g' \circ g$ に等しくなります。

これは定義 2 の直後に続きます。

#### 系 {#ens-ii-s5-n7-cor-1 .statement tag=03IU}

$(X_i)_{i\in I}$、$(Y_i)_{i\in I}$ を 2 つの集合の家族とし、$(g_i)_{i\in I}$ を写像の家族とします。 If $g_i$ is an injection (resp. surjection) of $X_i$ into $Y_i$, for each $i\in I$, then the extension $g$ of $(g_i)_{i\in I}$ to products is an injection (resp. surjection) of $\displaystyle\prod_{i\in I}X_i$ into $\displaystyle\prod_{i\in I}Y_i$.

(1) それぞれの $i\in I$ に対して $X_i\ne\varnothing$ を仮定します。それ以外の場合、結果は些細なものになります。 $g_i$ がそれぞれの $i\in I$ に対して単射であると仮定し、$r_i$ を $g_i$ (§ 3, no. 8、定義 11) の撤回とすることで、$r_i\circ g_i$ は $X_i$ の恒等写像となります。 $r$を家族$(r_i)_{i\in I}$の拡大から積とします。 $r\circ g$ は恒等写像 $I_{X_i}$ の族の拡大から積であるため、$r\circ g$ は $\displaystyle\prod_{i\in I}X_i$ の恒等写像であるため、$g$ は単射法 (§ 3, 命題 8）。

(2) $g_i$ が各 $i\in I$ の $Y_i$ への $X_i$ の射影であると仮定し、$s_i$ を $g_i$ (§ 3, no. 8, 定義 11) の切断とすると、$g_i\circ s_i$ は次のようになります。 $Y_i$中恒等写像。 $s$ が $(s_i)_{i\in I}$ ファミリーの拡大から積である場合、$g\circ s$ は恒等写像 $I_{Y_i}$ ファミリーの拡大から積であり、したがって $\displaystyle\prod_{i\in I}Y_i$ の恒等写像になります。したがって、$g$ は全射法 (§ 3, 命題 8) です。

$(X_i)_{i\in I}$ を集合の家族とし、$E$ を集合とします。 $E$ の写像 $f$ を $\displaystyle\prod_{i\in I}X_i$ にすると、$\operatorname{pr}_i\circ f$ は $E$ の写像から $X_i$ になります。 $\bar f$ がこの写像族の拡大から積であり、$d$ が $E$ の$E^I$ への対角写像である場合、$f=\bar f\circ d$ は明らかになります。 Conversely, let $(f_i)_{i\in I}$ be a family of functions such that $f_i$ is a mapping of $E$ into $X_i$ for each $i\in I$, and let $\bar f$ be the extension to products of this family; then we have $\operatorname{pr}_i\circ(\bar f\circ d)=f_i$ for each $i\in I$. 言葉の乱用により、写像 $\bar f\circ d$ は $(f_i)_{i\in I}$ とも表記されます。 このようにして、集合 $\displaystyle\prod_{i\in I}X_i^E$ の定義するを 1 対 1 で写像から集合 $\displaystyle\left(\prod_{i\in I}X_i\right)^E$ に変換します。この写像とその逆は正規であると言われています。

### 練習問題 {#ens-ii-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
