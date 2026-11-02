---
book: ens
book_title: Theory of Sets
chapter: II
chapter_title: THEORY OF SETS
section: 6
section_title: Equivalence relations
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 112-122, 127-129
pdf_pages: 0119-0129, 0134-0136
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF AN EQUIVALENCE RELATION
      page: 113
      pdf_page: 120
    - "no": 2
      title: EQUIVALENCE CLASSES ; QUOTIENT SET
      page: 114
      pdf_page: 121
    - "no": 3
      title: RELATIONS COMPATIBLE WITH AN EQUIVALENCE RELATION
      page: 116
      pdf_page: 123
    - "no": 4
      title: SATURATED SUBSETS
      page: 117
      pdf_page: 124
    - "no": 5
      title: MAPPINGS COMPATIBLE WITH EQUIVALENCE RELATIONS
      page: 118
      pdf_page: 125
    - "no": 6
      title: INVERSE IMAGE OF AN EQUIVALENCE RELATION; INDUCED EQUIVALENCE RELATION
      page: 119
      pdf_page: 126
    - "no": 7
      title: QUOTIENTS OF EQUIVALENCE RELATIONS
      page: 119
      pdf_page: 126
    - "no": 8
      title: PRODUCT OF TWO EQUIVALENCE RELATIONS
      page: 120
      pdf_page: 127
    - "no": 9
      title: CLASSES OF EQUIVALENT OBJECTS
      page: 121
      pdf_page: 128
statements: 13
exercises: 11
content_sha256: 2b6ea6666d436905689ad28e378a200b193ec61af05d25092f5d58193970d34f
translated_from: content/en/ens/II/06_s6_equivalence_relations.md
translation_method: google
source_content_sha256: f7ce72a4dfc4c2df0edb07393e9d9b7234a3b676d35f6cff417c9f89092d2c5a
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 178454ebf40e5fd4b0f776d42f079fed3ae0524548dfcc2b11282793f09be770
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 6. 同値関係

原則として、今後は未決定のアセンブリを示すために太字の斜体文字を使用するのをやめます。読者は、未確定の文字または関係に適用される文脈主張から簡単に識別できます。

### 1. 定義/同値関係

$R\{x, y\}$ を関係、$x$ と $y$ を別個の文字とする。 関係 $R$ は、次の場合に (文字 $x$ と $y$ に関して) *対称* であると言われます。

$$R\{x, y\} \Rightarrow R\{y, x\}.$$

その場合、$x$ と $y$ を、互いに区別され、$R$ に含まれるすべての文字とは異なる 2 つの文字 $x'$ と $y'$ に置き換え、次に、$x'$ と $y'$ をそれぞれ$y$ と $x$ に置き換えることで、次のようになります。それを見てください

$$R\{y, x\} \Rightarrow R\{x, y\}.$$

したがって、$R\{x, y\}$ と $R\{y, x\}$ は同等です。

¶ $z$を$R$に現れない文字とする。 関係 $R$ は、次の場合、(文字 $x, y$ に関して) *他動* であると言われます。

$$(R\{x, y\} \text{ and } R\{y, z\}) \Rightarrow R\{x, z\}.$$

#### 例 {#ens-ii-s6-n1-exa-7 .statement tag=077S}

関係 $x = y$ は対称かつ推移的です。 関係 $X \subset Y$ は推移的ですが対称ではありません。 関係 $X \cap Y = \emptyset$ は対称ですが推移的ではありません。

$R\{x, y\}$ が対称かつ推移的である場合、それは *同値関係* (文字 $x$ と $y$ に関して) であると言われます。この場合、記法 $x \equiv y \pmod{R}$ は、ときどきが $R\{x, y\}$ の同義語として使用されます。 「*x は y のモジュロ* $R$ と同等です」と読み取られます。 $R$ が同値関係の場合、$R\{x, y\}$ は $R\{y, x\}$ を暗示し、$(R\{x, y\}$ と $R\{y, x\})$ は、次の理由により $(R\{x, x\}$ と $R\{y, y\})$ を暗示するため、$R\{x, y\} \Rightarrow (R\{x, x\}$ と $R\{y, y\})$ になります。 定義。

¶ $R\{x, y\}$ を関係とします。 関係 $R\{x, x\}$ が $x \in E$ と等しい場合、それは (文字 $x, y$ に関して) $E$ に *再帰的* であると言われます。 $E$ について曖昧さの可能性がない場合、言葉の乱用によって、$R$ は再帰的であると単純に言えます。

¶ * $E$ 上の *同値関係は、$E$ で再帰的である同値関係として定義されます。 $R\{x, y\}$ が $E$ で同値関係である場合、$R\{x, y\} \Rightarrow ((x, y) \in E \times E)$ があり、従って $R$ にはグラフが表示されます (文字 $x, y$ に関して)。逆に、同値関係 $R\{x, y\}$ にグラフ $G$ があるとします。 関係 $R\{x, x\}$ は関係 $(\exists y)R\{x, y\}$ と同等であることに注意してください。前者は後者を暗示します (章 I, § 4, no. 2、スキーム S5)。逆に、$R\{x, y\}$ は $R\{x, x\}$ を暗示するため、$(\exists y) R\{x, y\}$ は $(\exists y) R\{x, x\}$、従って $R\{x, x\}$ も暗示します。従って、$R\{x, x\}$ は $x \in \mathrm{pr}_1 G$ と同等であるため、$R$ は $\mathrm{pr}_1 G$ の同値関係になります。

¶ 集合 E 上の *同値* は対応で、そのソースとターゲットは両方とも E に等しく、そのグラフ F は、関係 $(x, y) \in F$ が E 上の同値関係となるようなものです。

*例*

#### 例 1 {#ens-ii-s6-n1-exa-1 .statement tag=03IX}

関係 $x = y$ はグラフのない同値関係です。グラフがある場合、このグラフの最初の射影はすべてのオブジェクトの集合になるからです。

#### 例 2 {#ens-ii-s6-n1-exa-2 .statement tag=03SC}

関係「$x = y$と$x \in E$」は、グラフが$E \times E$の対角となるE上の同値関係です。

#### 例 3 {#ens-ii-s6-n1-exa-3 .statement tag=03TQ}

関係「Y上にXの全単射が存在する」はグラフのない同値関係です(cf.章III, § 3)。

#### 例 4 {#ens-ii-s6-n1-exa-4 .statement tag=03TR}

関係「$x \in E$と$y \in E$」はEの同値関係で、そのグラフは$E \times E$です。

#### 例 5 {#ens-ii-s6-n1-exa-5 .statement tag=03TS}

$A \subset E$ と仮定します。それから関係

$$(x \in E - A \text{ and } y = x) \text{ or } (x \in A \text{ and } y \in A)$$

Eの同値関係です。

#### 例 6 {#ens-ii-s6-n1-exa-6 .statement tag=03TP}

\* 関係 「$x \in \mathbf{Z}$ と $y \in \mathbf{Z}$ と $x - y$ は 4 で割り切れます」は、$\mathbf{Z}$ では同値関係です。\*

#### 命題 1 {#ens-ii-s6-prop-1 .statement tag=03QH}

*対応* $\Gamma$ *間* X *と* X *同値がオン* X *次の条件を満たす場合に限り、* (a) X *は*のドメインです$\Gamma$; (b) $\Gamma = \overset{-1}{\Gamma}$; (c) $\Gamma \circ \Gamma = \Gamma$。
$\Gamma$ を X と X の間の対応とし、そのグラフを G とします。 $\Gamma$ が X の同値である場合、すべての $x \in X$ に対して $(x, x) \in G$ になります。従って、X は $\Gamma$ のドメインです。 関係 $(x, y) \in G$ は $(y, x) \in G$ と同等なので、$(x, y) \in \overset{-1}{G}$、つまり $G = \overset{-1}{G}$、従って $\Gamma = \overset{-1}{\Gamma}$ と同等です。 関係 $(x, y) \in G$ と $(y, z) \in G$ は $(x, z) \in G$ を意味するため、$G \circ G \subset G$ になります。逆に、$(x, y) \in G$ は $(x, x) \in G$ を意味するため、$(x, y) \in G \circ G$ となり、$G \subset G \circ G$ となります。従って $G = G \circ G$、その結果 $\Gamma = \Gamma \circ \Gamma$ となります。
¶ 逆に、条件 (a)、(b)、(c) が満たされるとします。 関係 $(x, y) \in G$ は対称 ((b) による) かつ推移的 ((c) による) です。従って、それは同値関係であり、(a) により、X では同値関係になります。

### 2. 同値類 ; 商集合

$f$ を写像とし、E をそのドメイン、F をグラフとします。 関係「$x \in E$と$y \in E$と$f(x) = f(y)$」はE上の同値関係で、同値関係*f*に関連付けられています。 関係 $(\exists z)((x, z) \in F$ と $(y, z) \in F)$、つまり $(\exists z)((x, z) \in F$ と $(z, y) \in \overset{-1}{F})$ に相当するため、そのグラフは $\overset{-1}{F} \circ F$ になります。

¶ これから、集合 $\mathrm{E}$ 上のすべての同値関係 $\mathrm{R}$ がこの型のものであることを示します。 $\mathrm{G}$を$\mathrm{R}$のグラフとします。それぞれの $x \in \mathrm{E}$ について、(空ではない) 集合 $\mathrm{G}(x) \subset \mathrm{E}$ は、* $\mathrm{R}$ に関して $x$ の *同値類と呼ばれます。したがって、すべての $y \in \mathrm{E}$ の集合は、$\mathrm{R}\{x, y\}$ になります。一部の $x \in \mathrm{E}$ に対して $\mathrm{G}(x)$ と表記できるすべての集合は、($\mathrm{R}$ に関して) 同値類と呼ばれます。 同値類の元は、この類の*代表*と呼ばれます。 $\mathrm{R}$ に対する同値類の集合 (つまり、形 $\mathrm{G}(x)$ の一部の $x \in \mathrm{E}$ のすべてのオブジェクトの集合) は、$\mathrm{E}$ の *商集合* と呼ばれます。 $\mathrm{R}$ は $\mathrm{E}/\mathrm{R}$ で示されます。ドメインが $\mathrm{E}$ でターゲットが $\mathrm{E}/\mathrm{R}$ である写像 $x \to \mathrm{G}(x)$ $(x \in \mathrm{E})$ は、$\mathrm{E}/\mathrm{R}$ に対する $\mathrm{E}$ の *標準写像* と呼ばれます。

C55。 *$\mathrm{R}$ *を集合* $\mathrm{E}$ の同値関係とし、 *そして $p$ を * $\mathrm{E}$ * $\mathrm{E}/\mathrm{R}$ の標準写像とします。 *それでは*

$$\mathrm{R}\{x, y\} \Leftrightarrow (p(x) = p(y)).$$

上記の記法で、$x$ と $y$ を $\mathrm{E}$ の元とします。

$$(x, y) \in \mathrm{G}.$$

次に$x \in \mathrm{E}$と$y \in \mathrm{E}$。 $\mathrm{G}(x) = \mathrm{G}(y)$ を示してみましょう。 $y \in \mathrm{G}(x)$ から、(命題 1) $\mathrm{G}(y) \subset (\mathrm{G} \circ \mathrm{G})(x) = \mathrm{G}(x)$ になります。一方、$(y, x) \in \mathrm{G}$、よって $\mathrm{G}(x) \subset \mathrm{G}(y)$ もあるため、

$$\mathrm{G}(x) = \mathrm{G}(y),$$

つまり、$p(x) = p(y)$。逆に、$\mathrm{G}(x) = \mathrm{G}(y)$の場合、$y \in \mathrm{G}(y) = \mathrm{G}(x)$があるので、$(x, y) \in \mathrm{G}$となります。これで証明は完了です。

¶ 標準写像の切断 $\mathrm{E}$ の $\mathrm{E}/\mathrm{R}$ (§ 3, no. 8、定義 11) への$p$ は、より簡単には $\mathrm{E}$ の *切断* (関係 $\mathrm{R}$ に関して) と呼ばれます。

*例*

#### 例 1 {#ens-ii-s6-n2-exa-1 .statement tag=03SD}

$\mathrm{R}$ を集合 $\mathrm{E}$ の同値関係 「$x \in \mathrm{E}$ と $y \in \mathrm{E}$ と $x = y$」 とします。 The equivalence class of $x \in \mathrm{E}$ is then the set $\{x\}$, and the canonical mapping $x \to \{x\}$ of $\mathrm{E}$ onto $\mathrm{E}/\mathrm{R}$ is bijective.

#### 例 2 {#ens-ii-s6-n2-exa-2 .statement tag=03SE}

Let $\mathrm{E}$, $\mathrm{F}$ be two sets and let $\mathrm{R}$ be the equivalence relation on $\mathrm{E} \times \mathrm{F}$ associated with the mapping $\mathrm{pr}_1$ of $\mathrm{E} \times \mathrm{F}$ onto $\mathrm{E}$. $\mathrm{R}$ に対する同値類は、形 $\{x\} \times \mathrm{F}$ の集合であり、$x \in \mathrm{E}$ です。 写像 $x \to \{x\} \times \mathrm{F}$ は、$\mathrm{E}$ の $(\mathrm{E} \times \mathrm{F})/\mathrm{R}$ 上の全単射です。

$\mathrm{R}$ を集合 $\mathrm{E}$ の同値関係とします。 商集合 $\mathrm{E}/\mathrm{R}$ は $\mathfrak{P}(\mathrm{E})$ の部分集合であり、$\mathrm{E}/\mathrm{R}$ の恒等写像は $\mathrm{E}$ (§ 4, no. 7) の *分割* です。なぜなら、$\mathrm{G}$ が $\mathrm{R}$ のグラフである場合、すべての $x \in \mathrm{E}$ に対して $x \in \mathrm{G}(x)$ があり、2 つの同値類 $\mathrm{G}(x)$ と $\mathrm{G}(y)$ に共通の元 $z$ がある場合、$\mathrm{R}\{x,\ z\}$ となります。 $\mathrm{R}\{y,\ z\}$、つまり$\mathrm{G}(x) = \mathrm{G}(y)$。さらに、関係

$$(\exists \mathrm{X})(\mathrm{X} \in \mathrm{E}/\mathrm{R} \text{ and } x \in \mathrm{X} \text{ and } y \in \mathrm{X})$$

は$\mathrm{R}\{x,\ y\}$と同等です。

¶ 逆に、$(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ を集合 E の分割とします。関係 $(\exists \iota)(\iota \in \mathrm{I}$ と $x \in \mathrm{X}_\iota$ および $y \in \mathrm{Y}_\iota)$ が E 上の同値関係 R であることがすぐに検証されます。 R に関する同値類は、分割の集合 $\mathrm{X}_\iota$ であり、写像 $\iota \to \mathrm{X}_\iota$ は E/R 上では I の全単射です。各 $\iota \in \mathrm{I}$、集合 $\mathrm{S} \cap \mathrm{X}_\iota$ が単一の元で構成されるような E のすべての部分集合 S は、R に関する同値類の代表* (または *横断*) の *系と呼ばれます。この名前は、任意の単射を表すのにも使用されます。 集合 K を E に変換し、この単射の下にある K の像が、R に関する同値類の代表の系となるようにします。たとえば、R に関する E の任意の *切断*。

### 3. 関係は同値関係と互換性があります

$\mathrm{R}\{x,\ x'\}$ を同値関係 、$\mathrm{P}\{x\}$ を関係とします。 関係 $\mathrm{P}\{x\}$ は、同値関係* $\mathrm{R}\{x,\ x'\}$ ($x$ に関して) と *互換性があると言われます。

$$(\mathrm{P}\{x\} \text{ and } \mathrm{R}\{x,\ y\}) \Rightarrow \mathrm{P}\{y\},$$

ここで、$y$ は P にも R にも現れない文字を表します。

たとえば、C43 (章 I, §5)、no. 1) から、すべての関係 $\mathrm{P}\{x\}$ は同値関係 $x = x'$ と互換性があることがわかります。

C56。 *$\mathrm{R}\{x,\ x'\}$ *を集合* E の同値関係とし、 *そして * $\mathrm{P}\{x\}$ * 関係とします。これは含むの文字* $x'$ ではなく、 (* $x$* に関して) 同値関係* と互換性があります* $\mathrm{R}\{x,\ x'\}$。 *その後、* $t$ * が * $\mathrm{P}\{x\}$ に現れない場合、*関係 "*$t \in \mathrm{E}/\mathrm{R}$ *and* $(\exists x)(x \in t$ *and* $\mathrm{P}\{x\})$*" は関係 "*$t \in \mathrm{E}/\mathrm{R}$ *and* $(\forall x)((x \in t) \Rightarrow \mathrm{P}\{x\})$*" と同等です。*

$t \in \mathrm{E}/\mathrm{R}$ にしましょう。 $\mathrm{P}\{a\}$ のような $a \in t$ が存在する場合、各 $x \in t$ には $\mathrm{R}\{a,\ x\}$ があり、したがって $\mathrm{P}\{x\}$ になります。したがって、$(\exists x)(x \in t$ と $\mathrm{P}\{x\})$ は $(\forall x)((x \in t) \Rightarrow \mathrm{P}\{x\})$ を意味します。 $t \in \mathrm{E}/\mathrm{R}$ は $t \neq \emptyset$ を意味するため、逆は明らかです。

¶ 関係

$$t \in \mathrm{E}/\mathrm{R} \text{ and } (\exists x)(x \in t \text{ and } \mathrm{P}\{x\})$$

は、R に関して、移行から商* に ($x$ に関して) $P\{x\}$ * によって *誘導されると言われています。この関係が $P'\{t\}$ で示され、$f$ が E/R 上の E の標準写像である場合、 関係

$$y \in E \text{ and } P'\{f(y)\}$$

($y$ が $P\{x\}$ に現れない) は、すぐに検証されるように、( $y \in E$ および $P\{y\}$) と *同等* です。

### 4. 飽和部分集合

$R\{x, y\}$ を集合 E 上の同値関係とし、A を E の部分集合とします。 関係 $x \in A$ が ($x$ に関して) $R\{x, y\}$ と互換性がある場合、A は R に関して *飽和していると言われます。または、同様に、*各 $x$ の $x \in A$ 同値類が * A に含まれている場合、他の語では、* R に関して同値類の *集合の *和集合である場合に限り、集合は R に関して飽和します。

¶ $f$ を E/R 上の E の標準写像とします。 A が R に関して飽和している場合、各 $x \in A$ の同値類 ($\overset{-1}{f}\langle\{f(x)\}\rangle$ に等しい) が A に含まれているため、$\overset{-1}{f}\langle f\langle A\rangle\rangle \subset A$ になります。いずれにせよ、$A \subset \overset{-1}{f}\langle f\langle A\rangle\rangle$があるので、$\overset{-1}{f}\langle f\langle A\rangle\rangle = A$ということになります。逆に、$A = \overset{-1}{f}\langle f\langle A\rangle\rangle$ の場合、R に関する$x$ のすべての $x \in A$ 同値類 $K = f(x)$ は、$f\langle A\rangle$ の元になります。 $K = \overset{-1}{f}\langle\{K\}\rangle$ から、$K \subset \overset{-1}{f}\langle f\langle A\rangle\rangle = A$ になります。したがって、R に関して飽和している E の部分集合は、正確に $A = \overset{-1}{f}\langle f\langle A\rangle\rangle$ となる E の部分集合 A です。同等に、それらは形 $\overset{-1}{f}\langle B\rangle$ の E の部分集合です。ここで、$B \subset E/R$; 関係 $A = \overset{-1}{f}\langle B\rangle$ は $B = f\langle A\rangle$ を意味するため、$A = \overset{-1}{f}\langle f\langle A\rangle\rangle$ になります。

¶ $(X_\iota)_{\iota \in I}$ が E の飽和部分集合の族である場合、集合 $\bigcup_{\iota \in I} X_\iota$ と $\bigcap_{\iota \in I} X_\iota$ は飽和します (§4、命題 3 と 4)。 A が E の飽和部分集合である場合、$\complement_E A$ (§4, 命題 6) も同様です。

¶ ここで、A を E の任意の部分集合とします。すると、集合 $\overset{-1}{f}\langle f\langle A\rangle\rangle$ 含む A となり、飽和します。逆に、A' が含む A である E の飽和部分集合である場合、$f\langle A'\rangle \supset f\langle A\rangle$ が得られます。

$$A' = \overset{-1}{f}\langle f\langle A'\rangle\rangle \supset \overset{-1}{f}\langle f\langle A\rangle\rangle.$$

したがって、$\overset{-1}{f}\langle f\langle A\rangle\rangle$ は、含む A (cf. 章 III) である E の「最小の」が飽和した部分集合であると言えます。この集合は、関係 R に対する A の *彩度* と呼ばれます。 A の彩度は、A の元の同値類の和集合であることがすぐにわかります。 $(\mathrm{X}_\iota)_{\iota \in \mathrm{I}}$ が E の部分集合のファミリーであり、$\mathrm{A}_\iota$ がR に対する $\mathrm{X}_\iota$ の彩度の場合、$\bigcup_{\iota \in \mathrm{I}} \mathrm{X}_\iota$ の彩度は $\bigcup_{\iota \in \mathrm{I}} \mathrm{A}_\iota$ (§4, 命題 3) になります。

### 5. 写像は同値関係と互換性があります

R を集合 E 上の同値関係とし、$f$ をドメイン E の写像とします。そのとき、関係 $y = f(x)$ が ($x$ に関して) と互換性がある場合、$f$ は関係* R と *互換性があると言われます。 関係 $\mathrm{R}\{x,\ x'\}$。

¶ 各同値類に対する $f$ の制限が定数写像であると言うのも同じことになります。この場合、* $f$ は * R に関して各同値類で定数であると言います。 $g$ が E/R 上の E の標準写像である場合、 主張は、関係 $g(x) = g(x')$ は $f(x) = f(x')$ を意味します。したがって (§3, 命題 9) 次の基準があります。

C57。 *R *を集合* E 上の同値関係とし、 *g を * E *上* E/R の標準写像とする。 *その後、写像 f of* E *into* F *は、f を形 h $\circ$ g に入れることができる場合に限り、* R と互換性があります。ここで、h は写像 of* E/R *into* F です。 *写像 h は f によって一意に決定されます。 s が g のいずれかの切断である場合、h $= f \circ s$ が得られます。*

写像 $h$ は、R に関して、移行から商* の f によって*誘導されると言われています。

¶ $f$ を集合 E の写像を集合 F に変換し、$\mathrm{A} = f\langle \mathrm{E}\rangle \subset \mathrm{F}$ とします。 R を同値関係と $f$ (no. 2) に関連付けるとします。 $f$ が R と互換性があることは明らかです。 さらに、移行から商に $f$ によって誘導される写像 $h$ は、F への E/R の *単射* です。つまり、$t$, $t'$ が R に関して同値類で、$h(t) = h(t')$ となる場合、次のようになります。すべての $x \in t$ と $x' \in t'$ に対して $f(x) = f(x')$ は、R の定義によって $t = t'$ を意味します。 $k$ を、$h$ と同じグラフを持つ A への E/R の写像とします。その場合、$k$ は *全単射* です。 $j$ が A の F の標準単射であり、$g$ が E/R の E の標準写像である場合、次のように書くことができます。

$$f = j \circ k \circ g.$$

この関係は f* の *標準分解と呼ばれます。

¶ $f$ を集合 E の写像を集合 F に、R を E の同値関係とし、S を F の同値関係とします。 $u$ を E/R 上の E の標準写像とし、$v$ を $F/S$ 上の $F$ の標準写像とします。 $v\mathbin{\circ}f$ が $R$ と互換性がある場合、写像 $f$ は、同値関係* $R$ および $S$ と *互換性があると言われます。これは、関係 $x\equiv x'$ (mod $R$) *暗黙* $f(x)\equiv f(x')$ (mod $S$) を意味します。 $R$ に関して移行から商に $v\mathbin{\circ}f$ によって引き起こされる $E/R$ の $F/S$ への写像 $h$ は、移行に $f$ によって引き起こされる *写像と呼ばれます$R$と$S$*に関しては商。 関係 $v\mathbin{\circ}f=h\mathbin{\circ}u$ が特徴です。

### 6. 同値関係中逆像;誘発同値関係

$\varphi$ を集合 $E$ の写像を集合 $F$ に、$S$ を $F$ の同値関係とします。 If $u$ is the canonical mapping of $F$ onto $F/S$, the equivalence relation associated with the mapping $u\mathbin{\circ}\varphi$ of $E$ into $F/S$ is called the *inverse image* of $S$ under $\varphi$; if $R$ is this relation, $R\{x,y\}$ is equivalent to $S\{\varphi(x),\varphi(y)\}$, and the equivalence classes with respect to $R$ are the inverse images under $\varphi$ of the equivalence classes with respect to $S$ which meet $\varphi\langle E\rangle$.

¶ In particular, consider an equivalence relation $R$ on a set $E$, and let $A$ be a subset of $E$; then the inverse image of $R$ under the injection $j$ of $A$ into $E$ is called the equivalence relation *induced* by $R$ on $A$, and is denoted by $R_A$.

¶ $R_A$ に関する同値類は、$A$ を満たす $R$ に関する同値類の $A$ 上の *トレース* です。 単射 $j$ は明らかに関係 $R_A$ および $R$ と互換性があります。 写像 $A/R_A$ の $h$ から $E/R$ への $R_A$ に対する移行から商への $j$ によって誘発され、$R$ は $A/R_A$ の *単射語* 写像です$E/R$: $f$ (または $g$) が $E$ から $E/R$ への標準写像 (または $A$ から $A/R_A$) である場合、関係 $h(g(x))=h(g(x'))$、ここで$x\in A$ と $x'\in A$ は、$f(x)=f(x')$ に相当し、したがって $g(x)=g(x')$ に相当します。 像 $h\langle A/R_A\rangle$ は $f\langle A\rangle$ に等しい。 $k$ が $h$ と同じグラフを持つ $f\langle A\rangle$ に対する $A/R_A$ の全単射写像である場合、$k$ とその逆関数は *正準 * であると言われます。

### 7. 同値関係中商

$x$、$y$ の 2 つの文字に対して、$R$、$S$ を 2 つの同値関係とします。 関係 $S\Rightarrow R$ が真の場合、$S$ は $R$ より *より細かい* (または $R$ は $S$ より *⟦粗い*) と言えます。 If $R$ and $S$ are equivalence relations on the same set $E$, the statement that $S$ is finer than $R$ means that the graph of $S$ is contained in that of $R$, or again that every equivalence class with respect to $S$ is contained in an equivalence class with respect to $R$; or, equivalently, that every equivalence class with respect to $R$ is saturated with respect to $S$.

*例*

#### 例 1 {#ens-ii-s6-n7-exa-1 .statement tag=03SF}

関係「$x \in E$と$y \in E$と$x = y$」は、Eのすべての同値関係よりもより細かいです。 関係「$x \in E$と$y \in E$」は、Eのすべての同値関係よりも粗いです。

#### 例 2 {#ens-ii-s6-n7-exa-2 .statement tag=03SG}

\* 同値関係 「$x \in \mathbf{Z}$ と $y \in \mathbf{Z}$ と $x - y$ は 4 で割り切れます」は、同値関係 「$x \in \mathbf{Z}$ と $y \in \mathbf{Z}$ と $x - y$ は 2 で割り切れます」よりもより細かいです。 \*

R と S を、同じ集合 E 上の 2 つの同値関係とし、S が R よりより細かいであるようにします。 $f$ と $g$ を、それぞれ E/R 上の E と E/S 上の E の標準写像とします。その場合、写像 $f$ は S と互換性があります。$h$ を、S に関して移行から商に$f$ によって誘導される写像とします。そうすると、$h$ は E/S の E/R への写像になります。 E/S 上の $h$ に関連付けられた同値関係は、R *S による *商と呼ばれ、R/S で表されます。 関係 $x \equiv y \pmod{R}$ は $g(x) \equiv g(y) \pmod{R/S}$ と等しく、R/S に関する同値類は、R に関する同値類の $g$ の下にある像です。 $h = j \circ h_2 \circ h_1$ を正規の分解 (no. 5) とします。 写像 $h$。次に、$h_1$ は (E/S)/(R/S) への E/S の標準写像であり、$j$ は E/R の恒等写像であり、$h_2$ は E/R への (E/S)/(R/S) の 1 対 1 の写像です。 写像 $h_2$ とその逆は *標準* と言われます。

¶ 逆に、集合 E/S 上の任意の同値関係 T を考え、R を関係 T (no. 6) の $g$ 下の逆像である E 上の同値関係とします。 関係 $x \equiv y \pmod{R}$ は $g(x) \equiv g(y) \pmod{T}$ と同等であるため、T は R/S と同等ということになります。

### 8. 積/2 同値関係

$R\{x, y\}$ と $R'\{x', y'\}$ を 2 つの同値関係とします。 $S\{u, v\}$ を関係とします

$$(\exists x)(\exists y)(\exists x')(\exists y')(u = (x, x') \text{ and } v = (y, y') \text{ and } R\{x, y\} \text{ and } R'\{x', y'\});$$

$S\{u, v\}$ が同値関係であることがすぐに検証され、R と R' の *積* と呼ばれ、$R \times R'$ で示されます。 R が集合 E 上の同値関係で、R' が集合 E' 上の同値関係であるとします。したがって、関係 $S\{u, u\}$ は次と同等です。

$$(\exists x)(\exists x')(u = (x, x') \text{ and } R\{x, x\} \text{ and } R'\{x', x'\})$$

つまり、$(\exists x)(\exists x')(u = (x, x')$、$x \in E$、$x' \in E')$、したがって $u \in E \times E'$ になります。したがって、$R \times R'$ は $E \times E'$ の同値関係になります。もし

$$u = (x, x')$$

$E \times E'$ の元は、関係 $S\{u, v\}$ と同等です

$$(\exists y)(\exists y')(v = (y, y') \text{ and } R\{x, y\} \text{ and } R'\{x', y'\});$$

$G$ と $G'$ がそれぞれ $R$ と $R'$ のグラフである場合、この関係は$v \in G(x) \times G(x')$ と等価になります。したがって、* $R \times R'$ に関して *すべての同値類は、* $R$ に関しては同値類の積であり、* $R'$ に関しては同値類であり、*その逆も同様です。

¶ $f$ と $f'$ を、それぞれ $E/R$ に対する $E$ と $E'/R'$ に対する $E'$ の標準写像とし、$f \times f'$ を $f$ と $f'$ の正規の拡大とします。 積集合 (§ 3, no. 9)。次に、すべての $(x, x') \in E \times E'$ に対して $(f \times f')(x, x') = (f(x), f'(x'))$ です。 元の $f \times f'$ $(E/R) \times (E'/R')$ の $(u, u')$ の下の逆像は、$R$ と同値類に関しては、同値類 $u$ の積 $u \times u'$ です。 $R'$に関しては$u'$。したがって、$f \times f'$ に関連付けられた同値関係は $R \times R'$ と同等になります。したがって、写像 $f \times f'$ は、$h \circ g$ と書くことができます。ここで、$g$ は、$E \times E'$ の標準写像です。

$$(E \times E')/(R \times R')$$

$h$ は $(E \times E')/(R \times R')$ の 1 対 1 の写像です

$$(E/R) \times (E'/R');$$

この写像 $h$ とその逆は *正規* と言われます。

#### 注意 {#ens-ii-s6-n8-rem-1 .statement tag=03IY}

$P\{x, x'\}$ を $y$、$y'$ の文字が出現しない関係とします。 関係 $(P\{x, x'\}$ と $R\{x, y\}$ および $R'\{x', y'\})$ が $P\{y, y'\}$ を暗示する場合、P は同値関係 $R\{x, y\}$ および $R'\{x', y'\}$ ($x$ および $x'$ に関して) と *互換性がある* と言われます。 $Q\{u\}$ を関係 $(\exists x)(\exists x')(u = (x, x')$ および $P\{x, x'\})$ とします。その場合、$Q\{u\}$ は ($u$ に関して) $R$ および $R'$ の同値関係 $S\{u, v\}$、積と互換性があると言うのと同じことになります。

### 9. 同等のオブジェクトの類

$R\{x, y\}$ を同値関係とします。グラフを持つ必要はありません。 $x$、$x'$、$y$ が 3 つの異なる文字である場合、関係 $R\{x, x'\}$ は「$R\{x, y\} \Longleftrightarrow R\{x', y\}$」を意味し、したがって関係 $(\forall y)(R\{x, y\} \Longleftrightarrow R\{x', y\})$ も意味することは明らかです。スキーム S7 (章 I, § 5, no. 1) により、$\theta\{x\} = \tau_y(R\{x, y\})$ とすると、関係 $R\{x, x'\}$ が意味します

$$\theta\{x\} = \theta\{x'\}.$$

一方、注意は、定義 $R\{x, \theta\{x\}\}$ により関係 $(\exists y)(R\{x, y\})$ となるため、(no. 1) は $R\{x, x\}$ と同等になります。 S6 (章 I, §5, no. 1), 関係により、関係 $(R\{x, x\}$ と $R\{x', x'\}$ と $\theta\{x\} = \theta\{x'\})$ は$R\{x, x'\}$ と *同等* であることがわかります。

$$(R\{x, x\} \text{ and } R\{x', x'\} \text{ and } (R\{x', \theta\{x\}\} \Leftrightarrow R\{x', \theta\{x'\}\})),$$

従って、$(R\{x, \theta\{x\}\}$ と $R\{x', \theta\{x\}\})$ もあり、最後に推移性と対称性によって $R\{x, x'\}$ になります。逆に、$R\{x, x'\}$ は $R\{x, x\}$ と $R\{x', x'\}$ を意味するので、主張が証明されます。 項 $\theta\{x\}$ は、x* に相当するオブジェクトの *類 (関係 R に関して) と呼ばれます。

¶ 今、T が項で、関係であると仮定します。

(1) $$(\forall y)(R\{y, y\} \Rightarrow (\exists x)(x \in T \text{ and } R\{x, y\}))$$

それは本当です。次に、関係 $(\exists x)(R\{x, x\}$ と $z = \theta\{x\})$ は *z で集合化しています*。なぜなら、$x \in T$ は $R\{x, x\}$ を暗示していると考えられるからです。 $R\{x, x\}$ ($R\{x, y\}$ は $R\{x, x\}$ を意味する観察すると) となるように、すべての $x \in T$ の集合で置き換える T を実行するだけで十分です。 $x \in T$ (§1, no. 6) に対する形 $\theta\{x\}$ のすべてのオブジェクトの $\Theta$ を集合とします。 $R\{y, y\}$ が true であると仮定します。その場合、$R\{x, y\}$ となるような $x \in T$ が存在し、従って $\theta\{y\} = \theta\{x\} \in \Theta$ になります。 集合 $\Theta$ は、R に関して等価なオブジェクト* の類の * 集合と呼ばれます。そして、$R\{x, x\}$ のような各 $x$ に対して、$\theta\{x\}$ は、$R\{x, z\}$ のような *一意の* 元 $z \in \Theta$ です。

同じ仮定の下で、$R\{x, y\}$ が $A\{x\} = A\{y\}$ を意味するように、$A\{x\}$ を項とします。次に、関係 $(\exists x)(R\{x, x\}$ と $z = \{x\})$ は $z$ で集団化されます。$R\{x, x\}$ は $R\{x, \theta\{x\}\}$ と同等であるため、$A\{x\} = A\{\theta\{x\}\}$ を意味し、その結果、E が形のオブジェクトの集合である場合、 $A\{t\}$ が $t \in \Theta$ の場合、$R\{x, x\}$ は $A\{x\} \in E$ を意味します。 $f$ が写像 $t \to A\{t\}$ $(t \in \Theta, A\{t\} \in E)$ である場合、関係 $R\{x, x\}$ は $A\{x\} = f(\theta\{x\})$ を意味します。

特に、R が集合* F 上の同値関係である場合、$A\{x\}$ を * R (no. 2) に関する x の *同値類とみなし、写像 $f$ は$\Theta$ の *全単射* となります。 商集合 F/R;これにより、導入された用語が正当化されます。

\* *例*。 $R\{x, y\}$ を同値関係とします。「$x$ と $y$ は、$\mathbf{C}$ 上の同じ有限次元の 2 つのベクトル空間です」。この関係にはグラフがありません。 T がすべてのベクトル部分空間の $\mathbf{C}^{(\mathbf{N})}$ の集合であるとき、または T の部分集合 T' が空間 $\mathbf{C}^n$ $(n \in \mathbf{N})$ で構成されているとき、$\mathbf{C}^0$ が以下から構成される規則に従って、条件 (1) を満たします。 $\mathbf{C}^{(\mathbf{N})}$ の点 0、そしてその $\mathbf{C}^n$ $(n > 0)$ は、直和 $\mathbf{C}^{(\mathbf{N})}$ の最初の $n$ 成分の和です。この 2 番目の選択では、$\Theta = T'$ になります。\*

### 練習問題 {#ens-ii-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
