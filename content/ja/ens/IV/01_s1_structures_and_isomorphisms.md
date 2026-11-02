---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 1
section_title: Structures and isomorphisms
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 259-271, 289
pdf_pages: 0264-0276, 0294-0294
extraction: ocr
subsections:
    - "no": 1
      title: ECHELONS
      page: 259
      pdf_page: 264
    - "no": 2
      title: CANONICAL EXTENSIONS OF MAPPINGS
      page: 260
      pdf_page: 265
    - "no": 3
      title: TRANSPORTABLE RELATIONS
      page: 261
      pdf_page: 266
    - "no": 4
      title: SPECIES OF STRUCTURES
      page: 262
      pdf_page: 267
    - "no": 5
      title: ISOMORPHISMS AND TRANSPORT OF STRUCTURES
      page: 264
      pdf_page: 269
    - "no": 6
      title: DEDUCTION OF STRUCTURES
      page: 266
      pdf_page: 271
    - "no": 7
      title: EQUIVALENT SPECIES OF STRUCTURES
      page: 268
      pdf_page: 273
statements: 17
exercises: 1
content_sha256: 14bb20a25df4ae974b33ef560e65d4b077e31582c9b46ea8f8c4eb48c10159f0
translated_from: content/en/ens/IV/01_s1_structures_and_isomorphisms.md
translation_method: google
source_content_sha256: 0afa8f8b2eeacc6c331a25088f06579b838538c263fddf5f044dbaa9e0fb2b95
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 57a934073072d55abbd58dee78572aeb4e5b16cbc2003f4d3e9036854e236624
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 1. 構造と同型

この章の目的は、数学で頻繁に現れる形成的な構成と証明 (cf. 章 I, § 1, no. 3 と § 2, no. 2) の特定の数をきっぱり説明することです。

### 1. エシュロン

*階層構成スキーム* は、自然整数 [^1] $c_i = (a_i,\ b_i)$、満たす、次の条件の順序付け対の数列 $c_1$、$c_2$、...、$c_m$ です。

(a) $b_i = 0$なら$1 \leqslant a_i \leqslant i - 1$。
(b) $a_i \neq 0$と$b_i \neq 0$なら、$1 \leqslant a_i \leqslant i - 1$と$1 \leqslant b_i \leqslant i - 1$。

これらの条件は、$b_1 > 0$ とともに $c_1 = (0,\ b_1)$ を意味します。 $n$ が対 $(0,\ b_i)$ に現れる整数 $b_i$ の最大のである場合、$c_1, c_2, ..., c_m$ は $n$ 項* 上の階層構成スキームであると言われます。

Given an echelon construction scheme $\mathrm{S} = (c_1,\ c_2,\ \ldots,\ c_m)$ on $n$ terms, and given $n$ terms $\mathrm{E}_1$, $\mathrm{E}_2$, ..., $\mathrm{E}_n$ in a theory $\mathscr{T}$ which is stronger than the theory of sets, an *echelon construction of scheme* $\mathrm{S}$ *on* $\mathrm{E}_1$, ..., $\mathrm{E}_n$ is defined to be a sequence $\mathrm{A}_1$, $\mathrm{A}_2$, ..., $\mathrm{A}_m$ of $m$ terms in the theory $\mathscr{T}$, defined step by step by the following conditions :

(a) $c_i = (0,\ b_i)$なら、$\mathrm{A}_i$は項$\mathrm{E}_{b_i}$となる。
(b) $c_i = (a_i,\ 0)$なら、$\mathrm{A}_i$は項$\mathfrak{P}(\mathrm{A}_{a_i})$となる。
(c) $a_i \neq 0$と$b_i \neq 0$を$c_i = (a_i,\ b_i)$とすると、$\mathrm{A}_i$は項$\mathrm{A}_{a_i} \times \mathrm{A}_{b_i}$となる。

$\mathrm{E}_1$, ..., $\mathrm{E}_n$ 上のスキーム S の階層構成の最後の項 $\mathrm{A}_m$ は、基底集合* $\mathrm{E}_1$, ..., $\mathrm{E}_n$ 上のスキーム S の *階層* と呼ばれます。以下の一般論では、記法 $\mathrm{S}(\mathrm{E}_1, \ldots, \mathrm{E}_n)$ で表されます。

#### 例 {#ens-iv-s1-n1-exa-1 .statement tag=03V4}

2 つの集合 E、F、集合 $\mathfrak{P}(\mathfrak{P}(\mathrm{E})) \times \mathfrak{P}(\mathrm{F})$ は、スキームを使用した E、F 上の階層です。

$$(0, 1), \quad (0, 2), \quad (1, 0), \quad (3, 0), \quad (2, 0), \quad (4, 5).$$

それはスキームを備えた E、F の階層でもあります

$$(0, 2), \quad (0, 1), \quad (1, 0), \quad (2, 0), \quad (4, 0), \quad (5, 3).$$

したがって、異なる計画によって、同じ項上に同じ階層が生じる可能性があります。

### 2. 正規拡大/写像

$\mathrm{S} = (c_1, c_2, \ldots, c_m)$ を $n$ 項の階層構成スキームとします。 $\mathrm{E}_1$, ..., $\mathrm{E}_n$, $\mathrm{E}'_1$, ..., $\mathrm{E}'_n$ を集合 ($\mathscr{T}$ で項) とし、$f_1$, ..., $f_n$ を $\mathscr{T}$ で項とします。 関係 「$f_i$は$\mathrm{E}_i$の写像が$\mathrm{E}'_i$になる」は$1 \leqslant i \leqslant n$の$\mathscr{T}$の定理です。 $\mathrm{A}_1$, ..., $\mathrm{A}_m$ (それぞれ $\mathrm{A}'_1$, ..., $\mathrm{A}'_m$) を、$\mathrm{E}_1$, ..., $\mathrm{E}_n$ (それぞれ $\mathrm{E}'_1$, ..., $\mathrm{E}'_n$) 上のスキーム S の階層構成とします。 We define step by step a sequence of $m$ terms $g_1$, ..., $g_m$ such that $g_i$ is a *mapping of* $\mathrm{A}_i$ *into* $\mathrm{A}'_i$ (for $1 \leqslant i \leqslant m$) by the following conditions :

(a) $c_i = (0, b_i)$ の場合、$\mathrm{A}_i = \mathrm{E}_{b_i}$ と $\mathrm{A}'_i = \mathrm{E}'_{b_i}$ であるため、$g_i$ は写像 $f_{b_i}$ になります。

(b) $c_i = (a_i, 0)$ の場合、$\mathrm{A}_i = \mathfrak{P}(\mathrm{A}_{a_i})$ と $\mathrm{A}'_i = \mathfrak{P}(\mathrm{A}'_{a_i})$ である場合、$g_i$ は、$g_{a_i}$ の $\hat{g}_{a_i}$ から部分集合の集合 (章 II, § 5, no. 1) の * 正準拡大* です。

(c) $c_i = (a_i, b_i)$ の場合、$a_i \neq 0$ と $b_i \neq 0$ は次のようになります。

$$\mathrm{A}_i = \mathrm{A}_{a_i} \times \mathrm{A}_{b_i} \qquad \text{and} \qquad \mathrm{A}'_i = \mathrm{A}'_{a_i} \times \mathrm{A}'_{b_i},$$

その場合、$g_i$ は、$g_{a_i}$ および $g_{b_i}$ から $\mathrm{A}_{a_i} \times \mathrm{A}_b$ (章 II, § 3, no. 9) の *正規の拡大* $g_{a_i} \times g_{b_i}$ です。

この数列の最後の項 $g_m$ は、*標準拡大と呼ばれ、スキーム* S、*of 写像* $f_1$、...、$f_n$ で、$\langle f_1, \ldots, f_n \rangle^{\mathrm{S}}$ で表されます。

¶ 次の基準を段階的に検証できます。

CST1。 *もし* $f_i$ *が* $\mathrm{E}_i$ *into* $\mathrm{E}'_i$の写像で、*かつ* $f'_i$ *が* $\mathrm{E}'_i$ *into* $\mathrm{E}''_i$ *(*$1 \leqslant i \leqslant n$*)の写像である場合、各階層について構成スキーム* S *on* $n$ *項私たちは*

$$\langle f'_1 \circ f_1, f'_2 \circ f_2, \ldots, f'_n \circ f_n \rangle^{\mathrm{S}} = \langle f'_1, f'_2, \ldots, f'_n \rangle^{\mathrm{S}} \circ \langle f_1, f_2, \ldots, f_n \rangle^{\mathrm{S}}.$$

CST2。 *$f_i$ が単射法* (それぞれ *全射法*) の場合、*$1 \leqslant i \leqslant n$ に対して*、*そのとき* $\langle f_1, \ldots, f_n \rangle^{\mathrm{S}}$ は *単射法* (それぞれ *全射法*) です。

この基準は、拡大 $\hat{g}$ (章 II, § 5, no. 1, 命題 1) および拡大 $g \times h$ (章 II, § 3, no. 9) の対応するプロパティに従います。

CST3。 *$f_i$ が $\mathrm{E}_i$ *上* $\mathrm{E}'_i$ の全単射である場合、 *そして $f_i^{-1}$ が逆全単射* [^2] である場合、 *そのとき* $\langle f_1, \ldots, f_n \rangle^{\mathrm{S}}$ * は全単射であり、* $\langle f_1^{-1}, \ldots, f_n^{-1} \rangle^{\mathrm{S}}$ * はその逆。その他の語*では、

$$(\langle f_1, \ldots, f_n \rangle^{\mathrm{S}})^{-1} = \langle f_1^{-1}, \ldots, f_n^{-1} \rangle^{\mathrm{S}}.$$

これは、CST1 と CST2 の直後に続きます。

### 3. 可搬性関係

$\mathscr{T}$を集合の理論より強い理論とし、$x_1, \ldots, x_n$、$s_1, \ldots, s_p$を$\mathscr{T}$の定数とは異なる別個の文字とし、$\mathrm{A}_1, \ldots, \mathrm{A}_m$を$\mathscr{T}$の項とする$x_i$ $(1 \leqslant i \leqslant n)$ と $s_j$ $(1 \leqslant j \leqslant p)$ の文字は表示されません。 $\mathrm{S}_1, \ldots, \mathrm{S}_p$ を $n + m$ 項の階層構成計画とします。次に関係 $\mathrm{T}\{x_1, \ldots, x_n, s_1, \ldots, s_p\}$ :

「$s_1 \in \mathrm{S}_1(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$と$s_2 \in \mathrm{S}_2(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$と$\ldots$と$s_p \in \mathrm{S}_p(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$」

は文字$s_1, \ldots, s_p$の*類型*と呼ばれます。

¶ $\mathrm{R}\{x_1, \ldots, x_n, s_1, \ldots, s_p\}$ を $\mathscr{T}$ の関係とし、含むの特定の文字$x_i$、$s_j$ (おそらく他の文字も同様) を表します。この場合、R は *輸送可能* (*in* $\mathscr{T}$) であると言われます *典型化* T に関して、*$x_i$ $(1 \leqslant i \leqslant n)$ は主要な基底集合と見なされ、* $\mathrm{A}_h$ $(1 \leqslant h \leqslant m)$ *補助的な基底と見なされます集合*、次の条件が満たされる場合: $y_1, \ldots, y_n, f_1, \ldots, f_n$ を、$x_i$ $(1 \leqslant i \leqslant n)$、$s_j$ $(1 \leqslant j \leqslant p)$、$\mathscr{T}$ の定数、および R または項に現れるすべての文字とは異なる別個の文字とする。 $\mathrm{A}_h$ $(1 \leqslant h \leqslant m)$ そして、$\mathrm{Id}_h$ $(1 \leqslant h \leqslant m)$ が$\mathrm{A}_h$ の恒等写像をそれ自体に表します。それから関係

(1) 「$\mathrm{T}\{x_1, \ldots, x_n, s_1, \ldots, s_p\}$ と ($f_1$ は $x_1$ の $y_1$ の全単射です) と $\ldots$ と ($f_n$ は $y_n$ の $x_n$ の全単射です)」

*暗黙的に* $\mathscr{T}$、*関係*

(2) $\mathrm{R}\{x_1, \ldots, x_n, s_1, \ldots, s_p\} \Leftrightarrow \mathrm{R}\{y_1, \ldots, y_n, s'_1, \ldots, s'_p\}$、ここで

$$(3) \qquad s'_j = \langle f_1, \ldots, f_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^s{}_j(s_j) \qquad (1 \leqslant j \leqslant p).$$

補助集合がない場合には、類似していますがより単純な定義があります。

たとえば、$n = p = 2$ で、類型 T が「$s_1 \in x_1$ および $s_2 \in x_1$」の場合、関係 $s_1 = s_2$ は可搬可能です。一方、関係 $x_1 = x_2$ は輸送できません。

### 4. 構造の種

$\mathscr{T}$を集合の理論より強い理論とします。 $\mathscr{T}$ の *構造* の種は、次のアセンブリで構成されるテキスト $\Sigma$ です。

(1) 文字 $x_1, \ldots, x_n, s$ の特定の数は、互いに区別され、$\mathscr{T}$ の定数からも区別されます。 $x_1, \ldots, x_n$ は、構造 $\Sigma$ の種の *主要な基底集合* と呼ばれます。

(2) $\mathscr{T}$ の項 $\mathrm{A}_1, \ldots, \mathrm{A}_m$ の特定の数には $x_1, \ldots, x_n, s$ の文字は現れず、$\Sigma$ の * 補助基底集合* と呼ばれます。 $\Sigma$ おそらく含む補助なし基底集合 (ただし、少なくとも 1 つのプリンシパル基底集合含むが必要です)。

(3) 類型化 $\mathrm{T}\{x_1, \ldots, x_n, s\}$ :

$$s \in \mathrm{S}(x_1, \ldots, x_n, \mathrm{A}_1, \ldots, \mathrm{A}_m),$$

ここで、S は $n + m$ 項 (no. 1) の階層構成スキームです。 $\mathrm{T}\{x_1, \ldots, x_n, s\}$ は、構造 $\Sigma$ の種の *典型的な特徴付け* と呼ばれます。

(4) 関係 $\mathrm{R}\{x_1, \ldots, x_n, s\}$ は、典型化 T に関して *移送可能* ($\mathscr{T}$)、$x_i$ が主基底集合であり、$\mathrm{A}_h$ が補助基底集合 (no. 3); R は、構造 $\Sigma$ の種の *公理* と呼ばれます。

理論 $\mathscr{T}_\Sigma$ は、$\mathscr{T}$ と同じ公理スキームを持ち、その明示的な公理が $\mathscr{T}$ の公理であり、公理 "T と R" とともに、構造* $\Sigma$ の種の *理論と呼ばれます。したがって、$\mathscr{T}_\Sigma$ の定数は、$\mathscr{T}$ の定数と、T または R に現れる文字です。

¶ $\mathscr{T}'$を$\mathscr{T}$より強い理論とし、$\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}$を$\mathscr{T}'$の項とする。 理論 $\mathscr{T}'$ では、U は *構造種* $\Sigma$ *主要な基底集合* $\mathrm{E}_1, \ldots, \mathrm{E}_n$ に * $\mathrm{A}_1, \ldots, \mathrm{A}_m$ * 補助基底が付いていると言われています。 集合*、関係の場合

$$\text{"}\mathrm{T}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}\} \text{ and } \mathrm{R}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}\}\text{"}$$

は *定理の * $\mathscr{T}'$ です。この場合、理論 $\mathscr{T}_\Sigma$ 関係 $\mathrm{B}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{U}\}$ のそれぞれの定理 $\mathrm{B}\{x_1, \ldots, x_n, s\}$ は、* $\mathscr{T}'$ (章 I, § 2, no. 3) の *定理になります。 $\mathscr{T}_\Sigma$ では、定数 $s$ は、種* $\Sigma$ の *ジェネリック構造と呼ばれます。

¶ 理論 $\mathscr{T}'$ では、プリンシパル基底集合 $\mathrm{E}_1, \ldots, \mathrm{E}_n$ には * 構造* $\mathrm{U}$ が与えられていると言われます。明らかに、$\mathrm{U}$ は集合の元です。

$$\mathrm{S}(\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{A}_1, \ldots, \mathrm{A}_m).$$

The set of elements $\mathrm{V}$ of $\mathrm{S}(\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{A}_1, \ldots, \mathrm{A}_m)$ which satisfy the relation $\mathrm{R}\{\mathrm{E}_1, \ldots, \mathrm{E}_n, \mathrm{V}\}$ is therefore the *set of structures of the species* $\Sigma$ *on* $\mathrm{E}_1, \ldots, \mathrm{E}_n$ (and it may be empty).

*例*

#### 例 1 {#ens-iv-s1-n4-exa-1 .statement tag=03V5}

$\mathscr{T}$を集合の理論とし、補助基底集合、1つの主基底集合$\mathrm{A}$、典型的な特徴付け$s \in \mathfrak{P}(\mathrm{A} \times \mathrm{A})$、および公理を持たない構造の種を考えます。

$$s \circ s = s \quad \text{and} \quad s \cap \overset{-1}{s} = \Delta_{\mathbf{A}}$$

($\Delta_{\mathbf{A}}$ は $\mathrm{A} \times \mathrm{A}$ の対角線です)、これは簡単に検証できるように、類型化 $s \in \mathfrak{P}(\mathrm{A} \times \mathrm{A})$ に関して可搬性関係です。この種の構造の理論が*順序集合* (章 III, §1, no. 3)の理論であることは明らかです。したがって、そのように定義された構造の種は、$\mathrm{A}$ の順序構造* の種とも呼ばれます。 章 III では、この種の構造が備わった集合のうち例が多く見られました。

#### 例 2 {#ens-iv-s1-n4-exa-2 .statement tag=03V6}

Take $\mathscr{T}$ to be the theory of sets, and consider the species of structures which has no auxiliary base set, one principal base set $\mathrm{A}$, the typical characterization $\mathrm{F} \in \mathfrak{P}((\mathrm{A} \times \mathrm{A}) \times \mathrm{A})$, and as axiom the transportable relation "F is a functional graph whose domain is $\mathrm{A} \times \mathrm{A}$". この種の構造は *代数構造* と呼ばれるものの特別なケースであり、そのグラフが $\mathrm{F}$ ($\mathrm{A} \times \mathrm{A}$ の写像を $\mathrm{A}$ に変換) である写像は *the* (*どこでも定義されている*) と呼ばれます。そのようなものの合成の *内部法則* 構造。

#### 例 3 {#ens-iv-s1-n4-exa-3 .statement tag=03V7}

前にとして、$\mathscr{T}$を集合の理論とし、補助基底集合、主基底集合$\mathrm{A}$、典型的な特徴付けを持たない構造の種を考えます。 $\mathrm{V} \in \mathfrak{P}(\mathfrak{P}(\mathrm{A}))$、そして公理として可搬性の関係

$$(\forall \mathrm{V}) \, ((\mathrm{V}' \subset \mathrm{V}) \Rightarrow ((\bigcup_{\mathrm{X} \in \mathrm{V}'} \mathrm{X}) \in \mathrm{V}))$$
$$\text{and} \quad (\forall \mathrm{X})(\forall \mathrm{Y})((\mathrm{X} \in \mathrm{V} \text{ and } \mathrm{Y} \in \mathrm{V}) \Rightarrow ((\mathrm{X} \cap \mathrm{Y}) \in \mathrm{V})).$$

この構造の種は、*トポロジカルな構造*の種と呼ばれます。本種の構造は*位相*とも呼ばれ、関係$\mathrm{X} \in \mathrm{V}$は$\mathrm{X}$が位相$\mathrm{V}$の*開いた集合*であることをというで表します（*一般的な位相*、章） I, § 1）。

#### 例 4 {#ens-iv-s1-n4-exa-4 .statement tag=03V8}

\* $\mathscr{T}$ を、(とりわけ) 一意 (主) として定数 K を持つ基底集合の除算種環構造の理論とします。 *左ベクトル空間* K の構造の種は、補助として K 基底集合、主基底集合 E、そして典型として特徴付け関係を持ちます。

$$V \in \mathfrak{P}((E \times E) \times E) \times \mathfrak{P}((K \times E) \times E)$$

(pr$_1$V は E の加法のグラフ、pr$_2$V はスカラー 乗法のグラフです);この種の構造の公理についてはここでは述べません。

#### 例 5 {#ens-iv-s1-n4-exa-5 .statement tag=03V9}

もう一度、$\mathscr{T}$ を集合の理論とします。この理論、体 $\mathbf{C}$ の複素数は項で、含むには文字がありません。 次元 n* の *複素解析多様体の構造の種には、補助基底集合として $\mathbf{C}$ と、1 つの主基底集合 V があります。ここでは、典型的な特徴付けやこの種の公理である構造については示さないことにします。 \*

*注意*

#### 注意 1 {#ens-iv-s1-n4-rem-1 .statement tag=03VA}

アプリケーションでは、(上記の例 4 のように) 階層 $S(E_1, \ldots, E_n, A_1, \ldots, A_m)$ が階層の積であることがよくあります。

$$S_1(E_1, \ldots, A_m) \times \cdots \times S_p(E_1, \ldots, A_m).$$

その場合、$\Sigma$ の定義の文字 $s$ は、多くの場合、「$p$-タプル」$(s_1, \ldots, s_p)$ (cf. 章 II, § 2, no. 1) に置き換えられます。

さらに、構造 $\Sigma$ の種の公理は、(上記の例 3 のように) いくつかの可搬性のある関係の結合として書かれることが最も多いです。これらの関係は、種 $\Sigma$ の *公理* と呼ばれます。

#### 注意 2 {#ens-iv-s1-n4-rem-2 .statement tag=03VB}

数学で最も頻繁に使用される構造の種と、これらの種の構造を備えた集合には名前が付けられます。したがって、*順序付けられた集合* (章 III, § 1) は集合に順序構造 (例 1) が与えられます。 \* この系列の後の本では、*群、体、トポロジカル空間、微分可能な多様体* などの定義する概念とします。これらはすべて、特定の構造を備えた集合を示します。 \*

#### 注意 3 {#ens-iv-s1-n4-rem-3 .statement tag=03VC}

言語の濫用により、集合 $\mathscr{T}$ の理論において、$n$ の異なる文字 $x_1, \ldots, x_n$ (典型的な特徴付けも公理も持たない) の付与は、構造 $\Sigma_0$ の種とみなされ、集合* の *構造と呼ばれます。 $n$ 校長基底集合 $x_1, \ldots, x_n$。

### 5. 構造の同型と輸送

$\Sigma$ を理論 $\mathscr{T}$ の構造 、主$n$ 基底集合 $x_1, \ldots, x_n$ に$m$ 補助基底集合 $A_1, \ldots, A_m$ の種とする。 S を $\Sigma$ の典型的な特徴付けに特徴がある $n + m$ 文字の階層構成スキームとし、R を $\Sigma$ の公理とします。 $\mathscr{T}$ より強い理論 $\mathscr{T}'$ では、U を集合 $E_1, \ldots, E_n$ の種 $\Sigma$ の構造とし（主基底集合として）、U$'$ を *同じ種* の構造とします。 集合 $E'_1, \ldots, E'_n$。 最後に、$f_i$ ($\mathscr{T}'$) を $\mathrm{E}'_i$ $(1 \leqslant i \leqslant n)$ に対する $E_i$ の *全単射* とします。 次に、$(f_1, \ldots, f_n)$ は、($\mathscr{T}'$ で) 構造 $\mathrm{U}'$ が付与された集合 $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$ に、構造 U が付与された集合 $\mathrm{E}_1, \ldots, \mathrm{E}_n$ の *同型* であると言われます。

(4) $$\langle f_1, \ldots, f_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{S}}(\mathrm{U}) = \mathrm{U}'$$

ここで、$\mathrm{Id}_h$ は、$\mathrm{A}_h$ の恒等写像を$(1 \leqslant h \leqslant m)$ に重ねたものを表します。

¶ $f'_i$ を全単射 $f_i$ $(1 \leqslant i \leqslant n)$ の逆数とします。 (4) と、我々が持っている基準 CST3 (no. 2) からすぐに得られます。

$$\langle f'_1, \ldots, f'_n, \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{S}}(\mathrm{U}') = \mathrm{U}$$

その結果、$(f'_1, \ldots, f'_n)$ は、$\mathrm{U}'$ を備えた $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$ の *同型* で、U を備えた $\mathrm{E}_1, \ldots, \mathrm{E}_n$ になります。 同型 $(f_1, \ldots, f_n)$ と $(f'_1, \ldots, f'_n)$ は、お互いの *逆* であると言われます。

$\mathrm{E}'_1, \ldots, \mathrm{E}'_n$上に$\mathrm{E}_1, \ldots, \mathrm{E}_n$の同型が存在する場合、$\mathrm{U}'$を備えた$\mathrm{E}'_1, \ldots, \mathrm{E}'_n$は、Uを備えた$\mathrm{E}_1, \ldots, \mathrm{E}_n$と*同型*であると言われます。この場合、構造 U と $\mathrm{U}'$ は *同型* であると言われます。

¶ 上記の定義は、CST1 とともに次の基準を意味します。

CST4。 *U、$\mathrm{U}'$、$\mathrm{U}''$ *同じ種の 3 つの構造 $\Sigma$ *主基底集合* $\mathrm{E}_1, \ldots, \mathrm{E}_n$、$\mathrm{E}'_1, \ldots, \mathrm{E}'_n$、$\mathrm{E}''_1, \ldots, \mathrm{E}''_n$、 *それぞれとする。 * $f_i$ *を* $\mathrm{E}_i$ *から* $\mathrm{E}'_i$の全単射とし、*そして* $g_i$ *を* $\mathrm{E}'_i$ *から* $\mathrm{E}''_i$ $(1 \leqslant i \leqslant n)$の全単射とします。 *$(f_1, \ldots, f_n)$ *と* $(g_1, \ldots, g_n)$ *が同型である場合、* $(g_1 \circ f_1, \ldots, g_n \circ f_n)$ も同様です。

$\mathrm{E}_1, \ldots, \mathrm{E}_n$ の $\mathrm{E}_1, \ldots, \mathrm{E}_n$ への同型 (*同じ* 構造に関して) は、$\mathrm{E}_1, \ldots, \mathrm{E}_n$ の *自己同型* と呼ばれます。 $\mathrm{E}_1, \ldots, \mathrm{E}_n$ の 2 つの自己同型の合成は自己同型であり、自己同型の逆数 \* なので、$\mathrm{E}_1, \ldots, \mathrm{E}_n$ 形の自己同型は *群* になります。 \*

#### 注意 {#ens-iv-s1-n5-rem-1 .statement tag=03VD}

言葉の乱用により、$f_i$が$\mathrm{E}_i$の$\mathrm{E}'_i$$(1 \leqslant i \leqslant n)$の全単射である場合、$(f_1, \ldots, f_n)$は、構造の種に関して、$\mathrm{E}_1, \ldots, \mathrm{E}_n$の$\mathrm{E}'_1, \ldots, \mathrm{E}'_n$の同型であると言われます。 集合 (no. 4、注意 3)。

CST5。 *$\mathscr{T}$ よりも強い理論* $\mathscr{T}'$ では、*U を *種* 構造 $\Sigma$ *に* $\mathrm{E}_1, \ldots, \mathrm{E}_n$、*そして* $f_i$ *$\mathrm{E}_i$ の全単射に *させてください集合* $\mathrm{E}'_i$ $(1 \leqslant i \leqslant n)$。 *その後、固有の種* 構造が存在します* $\Sigma$ *上* $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$ *そのような* $(f_1, \ldots, f_n)$ *は* $\mathrm{E}_1, \ldots, \mathrm{E}_n$ *上* $\mathrm{E}'_1, \ldots, \mathrm{E}'_n$の同型です。

この構造が存在する場合、関係 (4) によって定義される項 $\mathrm{U}'$ のみです。この項が確かに種$\Sigma$の構造であること、つまり$\mathscr{T}'$において関係$\mathrm{R}\{\mathrm{E}'_1, \ldots, \mathrm{E}'_n, \mathrm{U}'\}$が真であることはまだ検証されていない。しかし、これは、$\mathrm{R}\{x_1, \ldots, x_n, s\}$ が *輸送可能* であるという事実から導かれます。

$R\{E'_1, \ldots, E'_n, U'\}$ は、$\mathscr{T}'$ から関係 $R\{E_1, \ldots, E_n, U\}$ (no. 3) に等しく、$\mathscr{T}'$ から仮定までが当てはまります。

¶ 構造 $U'$ は、構造* $U$ *を集合* $E'_1, \ldots, E'_n$ *全単射写像* $f_1, \ldots, f_n$ を使って *輸送することによって得られると言われています。したがって、同じ種の 2 つの構造は、それぞれが構造の輸送によって他方から得られる場合に限り、同型となります。

It may happen that *any* two structures of species $\Sigma$ are *necessarily isomorphic*; the species of structure $\Sigma$ is then said be *univalent*. \* This is the case for the structure of an infinite cyclic group (isomorphic to $\mathbf{Z}$), the structure of a prime field of characteristic zero (isomorphic to $\mathbf{Q}$), the structure of a complete Archimedean ordered field (isomorphic to $\mathbf{R}$), the structure of an algebraically closed, connected, locally compact topological field (isomorphic to $\mathbf{C}$), and of the structure of a non-commutative, connected, locally compact topological division ring (isomorphic to $\mathbf{H}$, the division ring of quaternions). これらの構造の種の一部、たとえば、標数0 の素数体や完全なアルキメデスの順序体の種では、恒等写像以外には自己同型すら存在しません。しかし、上記の他の例に対してそのような自己同型は存在します (たとえば、$\mathbf{Z}$ の対称性 $x \rightarrow -x$)。 \*

上記の構造の種は、本質的に古典数学の基底であることが観察されます。一方、 \* 群構造の種、順序付けられた集合の構造の種、およびトポロジー 構造の種は一価ではありません。 \*

### 6. 構造の控除

$\Sigma$ を理論 $\mathscr{T}$ の構造 、主$n$ 基底集合 $x_1, \ldots, x_n$ に$m$ 補助基底集合 $A_1, \ldots, A_m$ の種とする。 $s$ を $\Sigma$ の汎用構造とし、$T$ を $n + m$ 項の階層構成スキームとします。 $\mathscr{T}_\Sigma$ の定数以外の文字が含むない項 $V\{x_1, \ldots, x_n, s\}$ は、次の条件を満たす場合、型 $T(x_1, \ldots, x_n, A_1, \ldots, A_m)$ の $s$ に対して *固有* であると言われます。

(1) 関係 $V\{x_1, \ldots, x_n, s\} \in T(x_1, \ldots, x_n, A_1, \ldots, A_m)$ は $\mathscr{T}_\Sigma$ の定理です。

(2) let $\mathscr{T}'_\Sigma$ be the theory obtained by adjoining to the axioms of $\mathscr{T}_\Sigma$ the axioms "$f_i$ is a bijection of $x_i$ onto $y_i$" $(1 \leqslant i \leqslant n)$ (where the letters $y_i$ and $f_i$ are distinct from each other and from the constants of $\mathscr{T}_\Sigma$, for $1 \leqslant i \leqslant n$); if $s'$ is the structure obtained by transporting $s$ by means of $(f_1, \ldots, f_n)$ (no. 5), then

$$V\{y_1, \ldots, y_n, s'\} = \langle f_1, \ldots, f_n. \mathrm{Id}_1, \ldots, \mathrm{Id}_m \rangle^{\mathrm{T}}(V\{x_1, \ldots, x_n, s\})$$

は $\mathscr{T}'_\Sigma$ の定理です。

構造の種の理論でどれが定義するにつながる項のほとんどは本質的な項です。

¶ Let $\Theta$ be another species of structures in the theory $\mathscr{T}$, on $r$ principal base sets $u_1,\ldots,u_r$, with $p$ auxiliary base sets $B_1,\ldots,B_p$, and let $t\in T(u_1,\ldots,u_r,B_1,\ldots,B_p)$ be the typical characterization of $\Theta$ (no. 4). 次に、$s$ に固有の $r+1$ 項 $P,U_1,\ldots,U_r$ の系が、理論 $\mathscr{T}_\Sigma$ において、$P$ が $U_1,\ldots,U_r$ 上の種 $\Theta$ の構造であることを演繹の手続きと呼びます。 $\Sigma$ の種構造から $\Theta$ の種構造 。 言葉の乱用により、項 $P$ だけを演繹の手順と呼ぶことがよくあります。

¶ $\mathscr{T}'$ を $\mathscr{T}$ よりも理論強くします。 $\mathscr{S}$ が $E_1,\ldots,E_n$ の種 $\Sigma$ の $\mathscr{T}'$ の構造である場合、$P\{E_1,\ldots,E_n,\mathscr{S}\}$ は $r$ 集合 $F_j=U_j\{E_1,\ldots,E_n,\mathscr{S}\}$ $(1\leq j\leq r)$ の種 $\Theta$ の構造であると言われています。 $P$ の手順によって $\mathscr{S}$ から推定されるか、$\mathscr{S}$ に従属します。 仮定項 $P,U_1,\ldots,U_r$ が $s$ に固有であることは、さらに次の基準を意味します。

**CST6.** $(g_1,\ldots,g_n)$ を、種 $\Sigma$ の構造 $\mathscr{S}$ を備えた $E_1,\ldots,E_n$ の同型とし、同じ種の構造 $\mathscr{S}'$ を備えた $E'_1,\ldots,E'_n$ とします。 $U_j$ が型 $\mathfrak{P}(T_j)$ の場合、

$$
h_j=\langle g_1,\ldots,g_n,\mathrm{Id}_1,\ldots,\mathrm{Id}_{m}\rangle^{T_j}\quad(1\leq j\leq r),
$$

そして $F'_j=U_j\{E'_1,\ldots,E'_n,\mathscr{S}'\}$ $(1\leq j\leq r)$ とします。次に、これら集合の系に、手順$P$によって$\mathscr{S}$と$\mathscr{S}'$からそれぞれ推定される種$\Theta$の構造が付与されると、$(h_1,\ldots,h_r)$は$F_1,\ldots,F_r$の同型が$F'_1,\ldots,F'_r$になります。

項 $x_1,\ldots,x_n$ が $s$ に固有であることは明らかです。多くの場合、項 $U_1,\ldots,U_r$ は$x_1,\ldots,x_n$ の文字に当てはまります。手順$P$によって$s$から推定された種$\Theta$の構造は、$s$の根底にある構造であると言われます。

*例*

#### 例 1 {#ens-iv-s1-n6-exa-1 .statement tag=03VE}

\* The species of topological group structures has a single principal base set $A$, no auxiliary base set, and the corresponding generic structure is a pair $(s_1,s_2)$ ($s_1$ being the graph of the law of composition on $A$, and $s_2$ the set of open sets in the topology of $A$; cf. General Topology, Chapter III, § 1). 項 $s_1,s_2$ のそれぞれは演繹の手順であり、トポロジカル群構造 $(s_1,s_2)$ の基礎となる群構造と位相をそれぞれ提供します。

同様に、ベクトル空間構造から、基礎となる可換式群構造を演繹することができます。 環構造から、基礎となる可換群構造と (乗法) 半群を推定できます。

IV
構造

構造。微分可能な多様体の構造から、基礎となる位相などが推定できます。

#### 例 2 {#ens-iv-s1-n6-exa-2 .statement tag=03VF}

$\mathbf{C}$ (それぞれ $\mathbf{R}$) 上のベクトル空間構造の種には、主基底集合 $E$、補助基底集合が $\mathbf{C}$ (それぞれ $\mathbf{R}$) に等しく、典型的な特徴付け

$$
s_1\in\mathfrak{P}((E\times E)\times E)\qquad\text{and}\qquad s_2\in\mathfrak{P}((\mathbf{C}\times E)\times E)
$$

(それぞれ $s_1\in\mathfrak{P}((E\times E)\times E)$ と $s_2\in\mathfrak{P}((\mathbf{R}\times E)\times E)$)。

対 $(s_1,s_2\cap((\mathbf{R}\times E)\times E))$ は、$\mathbf{C}$ に対するベクトル空間構造から $\mathbf{R}$ に対するベクトル空間構造を減算する手順です (「スカラーの体から $\mathbf{R}$ までの制限」)。 \*

#### 例 3 {#ens-iv-s1-n6-exa-3 .statement tag=03VG}

$\Theta$ が $\Sigma$ と同じ (主および補助) 基底集合と、同じ典型的な特徴付けを持っているとします。 さらに、$\Sigma$ の公理が ($\mathscr{T}$ において) $\Theta$ の公理を含意する場合、項 $s$ が種 $\Sigma$ の構造から種 $\Theta$ の構造を演繹する手順であることは明らかです。そして、$\Theta$は$\Sigma$よりも貧しく、$\Sigma$は$\Theta$よりも豊かであると言われます。 $\mathscr{T}$ よりも強い理論 $\mathscr{T}'$ の種 $\Sigma$ のすべての構造は、種 $\Theta$ の構造でもあります。 たとえば、合計順序集合の構造の種 (順序構造 (no. 4, 例 1) と関係 $s\cup s^{-1}=A\times A$ の公理の結合を公理として得られる) は、順序の種よりも豊かです。 構造。 \*可換群構造の種は、群構造の種よりも豊富です。 コンパクトなトポロジカル空間構造の種は、トポロジカル構造などの種よりも豊富です。 \*

#### 例 4 {#ens-iv-s1-n6-exa-4 .statement tag=077U}

\* $\Sigma$ と $\Theta$ がそれぞれ群構造 (それぞれ環構造) の種である場合、その上の各群構造 (それぞれ環構造) 群構造 (それぞれ環構造) に関連する演繹手順が代数で定義されます。 中心。 $\Sigma$ が体 $K$ 上のベクトル空間構造の種であるとき、および $\Theta$ が $K$ 上の代数構造の種であるとき、$K$ 上のすべてのベクトル空間に関連する演繹手順が定義されています。 テンソル代数またはその外観代数。この系列の後半で、他の多くの例に会うでしょう。 \*

#### 注意 {#ens-iv-s1-n6-rem-1 .statement tag=03VH}

$P$ が「q タプル」$(P_1,\ldots,P_q)$ であるとき、項 $P_1,\ldots,P_q$ は、種 $\Sigma$ の構造から種 $\Theta$ の構造を演繹する手順を構成するとも言われています。

### 7. 構造の同等種

$\Sigma$ と $\Theta$ を、同じ理論 $\mathscr{T}$ 内にあり、同じ主基底集合 $x_1,\ldots,x_n$ を持つ 2 つの種構造とします。それぞれ$s,t$を種$\Sigma,\Theta$の総称構造とします。次の条件が満たされるとします。

(1) We have a procedure of deduction $P\{x_1,\ldots,x_n,s\}$ of a structure of species $\Theta$ on $x_1,\ldots,x_n$ from a structure of species $\Sigma$ on $x_1,\ldots,x_n$.

(2) $x_1,\ldots,x_n$の種$\Theta$の構造から、$x_1,\ldots,x_n$の種$\Sigma$の構造の$Q\{x_1,\ldots,x_n,t\}$を差し引く手順があります。

(3) 関係 $Q\{x_1,\ldots,x_n,P\{x_1,\ldots,x_n,s\}\}=s$ は $\mathscr{T}_{\Sigma}$ の定理であり、関係 $P\{x_1,\ldots,x_n,Q\{x_1,\ldots,x_n,t\}\}=t$ は $\mathscr{T}_{\Theta}$ の定理です。

構造 $\Sigma$ と $\Theta$ の種は、演繹$P$ と $Q$ の手順によって同等であると言われます。この場合、理論 $\mathscr{T}_{\Sigma}$ の定理 $B\{x_1,\ldots,x_n,s\}$ ごとに、関係 $B\{x_1,\ldots,x_n,Q\}$ は $\mathscr{T}_{\Theta}$ の定理になります。逆に、理論 $\mathscr{T}_{\Theta}$ の定理 $C\{x_1,\ldots,x_n,t\}$ ごとに、関係 $C\{x_1,\ldots,x_n,P\}$ は $\mathscr{T}_{\Sigma}$ の定理になります。

☡

$U$が種$\Sigma$の構造である場合、$U$から$P$の手順で推定される構造は$U$と同等であると言われます。基準 CST6 は次のことを意味します。

CST7。 *主基底集合 $(E_1,\ldots,E_n),(E'_1,\ldots,E'_n)$ 上の種 $\Sigma$ の 2 つの構造を$\mathscr{S},\mathscr{S}'$ とします。 $\mathscr{S}_0,\mathscr{S}'_0$ を、それぞれ$\mathscr{S}$ と$\mathscr{S}'$ に等しい種 $\Theta$ の構造とします。 順序において、構造$\mathscr{S}_0$と$\mathscr{S}'_0$に関して$(g_1,\ldots,g_n)$が同型であることは、$(g_1,\ldots,g_n)$が構造$\mathscr{S}$に関して同型であることが必要十分であり、 $\mathscr{S}'$.*

実際には、構造の 2 つの同等の種の理論 $\mathscr{T}_{\Sigma}$ と $\mathscr{T}_{\Theta}$ を区別しません。

*例*

#### 例 1 {#ens-iv-s1-n7-exa-1 .statement tag=03VI}

\* $\Sigma$ を可換群構造の種とします。 $\Sigma$ には 1 つの (主要な) 基底集合 $A$ があり、その総称構造は 1 つの文字 $F$ で構成されます。 $\Sigma$ の典型的な特徴付けは $F\in\mathfrak{P}((A\times A)\times A)$ であり、$\Sigma$ の公理を $R\{A,F\}$ で表します。この公理は、特に、$F$ が写像 (群の「合成の法則」、cf. no. 4、例 2) のグラフであることを意味します。 理論 $\mathscr{T}_{\Sigma}$ ($\mathscr{T}$ は集合の理論を表します) では、 定義する項 $M\{A,F\}$ は、$\mathfrak{P}((\mathbf{Z}\times A)\times A)$ の関数グラフであり、次の関係を満たします。 $B\{M,A,F\}$:

$$
(\forall x)(\forall y)(\forall n)((x\in A\ \text{and}\ y\in A\ \text{and}\ n\in\mathbf{Z})
\Rightarrow (M(n,F(x,y))=F(M(n,x),M(n,y))))
$$

そして

$$
(\forall x)(\forall m)(\forall n)((x\in A\ \text{and}\ m\in\mathbf{Z}\ \text{and}\ n\in\mathbf{Z})
\Rightarrow (M(m+n,x)=F(M(m,x),M(n,x))))
$$

そして

$$
(\forall x)(\forall m)(\forall n)((x\in A\ \text{and}\ m\in\mathbf{Z}\ \text{and}\ n\in\mathbf{Z})
\Rightarrow (M(m,M(n,x))=M(mn,x)))
$$

そして

$$
(\forall x)((x\in A)\Rightarrow (M(1,x)=x)).
$$

(「$A$ の元の乗法 by 整数」)。

単一の主要な基底集合 $A$ と、補助的な集合としての $\mathbf{Z}$ を持ち、一般的な構造含む 2 つの文字 G、L が典型的な$\mathbf{Z}$ モジュール構造の種 $\Theta$ を考えてみましょう。 特徴付け

$G \in \mathfrak{P}((A \times A) \times A)$ と $L \in \mathfrak{P}((\mathbf{Z} \times A) \times A)$

そして公理

「$R \mid A, G$ と $(L$ は関数グラフです) と $B \mid L, A, G$」。

項 F, M は種 $\Sigma$ の構造から種 $\Theta$ の構造を演繹する手順を構成し、項 G は種 $\Theta$ の構造から種 $\Sigma$ の構造を演繹する手順であることがすぐに検証されます。 さらに、上記の条件 (3) は自明に満たされます。 したがって、可換群構造の種と $\mathbf{Z}$ 加群構造の種は同等であると言えます。

#### 例 2 {#ens-iv-s1-n7-exa-2 .statement tag=03VJ}

$\Sigma$ をトポロジー 構造 (no. 4, 例 3) の種とし、$A$ を (主) 基底集合とし、$V$ を $\Sigma$ の総称構造とします。 関係を検討してください

$$x \in A \text{ and } X \subset A \text{ and } (\forall U)((U \in V \text{ and } x \in U) \Rightarrow (X \cap U \neq \varnothing)).$$

この関係には、対$(X, x)$に関してグラフ$P \subset \mathfrak{P}(A) \times A$があります。 $P \mid A, V$ は、「位相 $V$ に関して $x$ が$X$ の閉包にあるように、すべての対 $(X, x)$ の集合」と呼ばれる項です。 次に、次の関係が $\mathscr{T}_{\Sigma}$ の定理であることを証明できます (cf. 一般位相、章 I, § 1)。

$$P(\varnothing)=\varnothing,$$

$$(\forall Y)((Y \subset A) \Rightarrow (\forall Y \subset P(Y))),$$

$$(\forall Y)((Y \subset A) \Rightarrow (P(P(Y))=P(Y))),$$

$$(\forall Y)(\forall Z)((Y \subset A \text{ and } Z \subset A) \Rightarrow (P(Y \cup Z)=P(Y)\cup P(Z))).$$

単一の (主) 基底集合 $A$ を持ち、その総称構造が 1 つの文字 $W$ で構成され、典型的な特徴付け $W \in \mathfrak{P}(\mathfrak{P}(A) \times A)$ と公理として持つ構造 $\Theta$ の種を考えてみましょう。

$$W(\varnothing)=\varnothing \text{ and } (\forall Y)((Y \subset A) \Rightarrow (Y \subset W(Y)))$$

そして

$$(\forall Y)((Y \subset A) \Rightarrow (W(W(Y))=W(Y)))$$

そして

$$(\forall Y)(\forall Z)((Y \subset A \text{ and } Z \subset A) \Rightarrow (W(Y \cup Z)=W(Y)\cup W(Z))).$$

関係も検討してください

$$U \subset A \text{ and } (\forall x)((x \in U) \Rightarrow x \notin W(A-U)).$$

すべての$U \in \mathfrak{P}(A)$の集合と、この関係の満たすは、$\mathfrak{P}(A)$の部分集合$Q \mid A, W$です。次に、次の関係が $\mathscr{T}_{\Theta}$ の定理であることを証明できます (一般位相、章 I, § 1、練習問題 10)。

$$A \in Q,$$

$$(\forall M)((M \subset Q) \Rightarrow ((\bigcup_{X \in M} X) \in Q)),$$

$$(\forall X)(\forall Y)((X \in Q \text{ and } Y \in Q) \Rightarrow ((X \cap Y) \in Q)).$$

したがって、上記の項 $P\{A,V\}$ と $Q\{A,W\}$ 満たす条件 (1) と (2)、そしてそれらが満たす条件 (3) であることも簡単にわかります。したがって、構造 $\Sigma$ と $\Theta$ の種は同等であり、したがって、種 $\Theta$ のすべての構造を位相、つまり、演繹$Q\{A,W\}$ の手順に基づいてそれに対応する加えられたものとみなします。 \*

### 練習問題 {#ens-iv-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。

[^1]: We use the notion of integer in the same manner as in Chapter I, that is to say, in the metamathematical sense of marks arranged in a certain order; this use has nothing to do with the mathematical theory of integers which was developed in Chapter III.
[^2]: For typographical reasons we write here $f^{-1}$ instead of $\overset{-1}{f}$.
