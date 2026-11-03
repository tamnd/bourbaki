---
book: ens
book_title: Theory of Sets
chapter: IV
chapter_title: STRUCTURES
section: 2
section_title: Morphisms and derived structures
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 271-283, 290-294
pdf_pages: 0276-0288, 0295-0299
extraction: ocr
subsections:
    - "no": 1
      title: MORPHISMS
      page: 271
      pdf_page: 276
    - "no": 2
      title: FINER STRUCTURES
      page: 273
      pdf_page: 278
    - "no": 3
      title: INITIAL STRUCTURES
      page: 274
      pdf_page: 279
    - "no": 4
      title: EXAMPLES OF INITIAL STRUCTURES
      page: 276
      pdf_page: 281
    - "no": 5
      title: FINAL STRUCTURES
      page: 280
      pdf_page: 285
    - "no": 6
      title: EXAMPLES OF FINAL STRUCTURES
      page: 281
      pdf_page: 286
statements: 12
exercises: 11
content_sha256: f26712f95c7c1734979509454b019ff07374108c48e4ac0a13e31ce54810d3b3
translated_from: content/en/ens/IV/02_s2_morphisms_and_derived_structures.md
translation_method: google
source_content_sha256: 5c7ff47f7a7c64e4e4d983dd7ce3ddd6c8c6e0cdf0393ed5ed3c52c0ad38c5b8
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 00a21aec8f41d42696554ac4f97f7a29c4b150ee3e57e2a060e25c966797459e
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 2. 射とその派生構造

### 1. 射

この切断と次の切断では、簡単のため、検討中の構造の種には基底集合が 1 つだけあると仮定します (したがって、これは主要な基底集合)。読者は、定義とその結果を一般的なケースに拡張することに困難はありません。

$\Sigma$ を、集合の理論よりも強い、理論 $\mathscr{T}$ の構造の種とし、$x$、$y$、$s$、$t$ を、 $\mathscr{T}$。 記法 $\mathfrak{F}(x,y)$ は、$x$ の写像の集合を $y$ (章 II, § 5, no. 2) に変換することを思い出します。次の条件を満たす $\mathscr{T}$ で項 $\sigma\{x,y,s,t\}$ が与えられたとします。

$(\mathrm{MO}_{\mathrm{I}})$ *関係 「$s$ は、$x$ の種 $\Sigma$ の構造であり、$t$ は、$y$ の種 $\Sigma$ の構造である」は、E では、関係を意味します。 $\sigma\{x,y,s,t\}\subset\mathfrak{F}(x,y)$.*

$(\mathrm{MO}_{\mathrm{II}})$ *理論 $\mathscr{T}'$ が $\mathscr{T}$ より強い場合、3 つの集合 E、E'、E'' にそれぞれ $\Sigma$ 種の構造 $\mathscr{S}$、$\mathscr{S}'$、$\mathscr{S}''$ が与えられます。 関係 $f\in\sigma\{E,E',\mathscr{S},\mathscr{S}'\}$ と $g\in\sigma\{E',E'',\mathscr{S}',\mathscr{S}''\}$ は関係* を意味します

$$
g\circ f\in\sigma\{E,E'',\mathscr{S},\mathscr{S}''\}.
$$

$(\mathrm{MO}_{\mathrm{III}})$ *理論 $\mathscr{T}'$ が $\mathscr{T}$ より強い場合、$\Sigma$ 種の構造 $\mathscr{S}$、$\mathscr{S}'$ を備えた 2 つの集合 E、E' があれば、全単射 E' 上の E の $f$ は、$f\in\sigma\{E,E',\mathscr{S},\mathscr{S}'\}$ と $f^{-1}\in\sigma\{E',E,\mathscr{S}',\mathscr{S}\}$ の場合に限り、同型です。*

$\Sigma$ と $\sigma$ が与えられた場合、関係 $f\in\sigma\{x,y,s,t\}$ はというによって表され、$f$ は $x$ の *射* (または $\sigma$-*射*) であり、 $s$ から $y$ に、$t$ が与えられます。 (理論 $\mathscr{T}'$ が $\mathscr{T}$ より強い) E と E' が、種 $\Sigma$ の構造 $\mathscr{S},\mathscr{S}'$ を備えた 2 つの集合である場合、項 $\sigma\{E,E',\mathscr{S},\mathscr{S}'\}$ は、種集合になります。 $\sigma$-E から E' への射。*

*例*

#### 例 1 {#ens-iv-s2-n1-exa-1 .statement tag=03VL}

$\Sigma$ を順序構造の種とし、$\sigma\{x,y,s,t\}$ がすべての写像の集合 $x$ の $f$ を $y$ にすると、関係 $(u,v)\in s$ が意味することになります。 $(f(u),f(v))\in t$。 章 III, § 1 の記法では、$u \leqslant v$ は $f(u) \leqslant f(v)$ を暗示します。つまり、$f$ は *増加する* であることを意味します。公理 $(\mathrm{MO_I})$、$(\mathrm{MO_{II}})$、および $(\mathrm{MO_{III}})$ の検証は明らかです。

#### 例 2 {#ens-iv-s2-n1-exa-2 .statement tag=03VM}

$\Sigma$ を、どこでも定義されている (§1, no. 4, 例 2) 合成の単一 (内部) 法則を持つ代数構造の種とします。 A、A$'$を、種$\Sigma$の構造を備えた2つの集合とし、$p$、$p'$を、これら2つの種構造のうちの合成法則とする。すべての $x \in \mathrm{A}$ とすべての $y \in \mathrm{A}$ に対して $p'(f(x), f(y)) = f(p(x,\ y))$ となるように、A の写像 $f$ を A$'$ に入れることを考えます。これら写像満たす $(\mathrm{MO_I})$、$(\mathrm{MO_{II}})$、$(\mathrm{MO_{III}})$ を A の *準同型* から A$'$ と呼びます。

#### 例 3 {#ens-iv-s2-n1-exa-3 .statement tag=03VN}

$\Sigma$ を位相構造の種とします (§1, no. 4, 例 3)。 A、A$'$を、それぞれトポロジーV、V$'$を備えた2つの集合とする。 関係 $\mathrm{X}' \in \mathrm{V}'$ が $\overset{-1}{f}(\mathrm{X}') \in \mathrm{V}$ を意味するように、A の写像 $f$ を A$'$ に変換します (他の語では、位相のすべてのオープン集合の逆像が含まれるようにします)。 V$'$ は、位相 V のオープン集合です)。これらの写像 (満たす $(\mathrm{MO_I})$、$(\mathrm{MO_{II}})$、および $(\mathrm{MO_{III}})$) は、A から A$'$ への *連続* 写像です (トポロジー V および V$'$ に関して) (cf. *一般位相*、章 I, § 2)。

#### 注意 {#ens-iv-s2-n1-rem-1 .statement tag=03VO}

構造 $\Sigma$ の特定の種については、定義するさまざまな項 $\sigma \} x,\ y,\ s,\ t \{$ 満たす条件 $(\mathrm{MO_I})$、$(\mathrm{MO_{II}})$、$(\mathrm{MO_{III}})$ を使用する機会があるかもしれません。たとえば、$\Sigma$ がトポロジカル構造の種で、上の例 3 の記法がある場合、関係 $\mathrm{X} \in \mathrm{V}$ が $f(\mathrm{X}) \in \mathrm{V}'$ を意味する場合、A の $'$ への写像 $f$ は *オープン* であると言われます。その他の語、各オープン集合の $f$ の下の像がオープン集合である場合）。種 $\Sigma$ に対して、オープン写像が満たす条件 $(\mathrm{MO_I})$、$(\mathrm{MO_{II}})$、$(\mathrm{MO_{III}})$ であることも簡単に確認できます。 \* さらに、連続する写像は必ずしも開いているわけではなく、開いている写像は必ずしも連続しているわけではないこともわかります。 \* したがって、特定の種構造は、明確に定義された射の概念を *意味しません。

☡

順序構造、代数的構造、およびトポロジー的構造が関係する場合、射は上記の例で定義されたものであり、〜でない限りその逆は明示的に述べられていることを常に理解する必要があります。

全単射 (章 II, § 3, no. 8、系から命題 8) の条件 $(\mathrm{MO_{III}})$ と特徴付けは、次の基準を意味します。

CST8。 *E、E$'$ *を 2 つの集合とし、それぞれに $\Sigma$ の種構造が与えられます。 $f$ を * E の *into* E$'$ * の $\sigma$ 射とし、$g$ を * E$'$ *into* E の $\sigma$ 射とします。 *$g \circ f$ が * E * 自体の恒等写像で、$f \circ g$ が * E$'$ * 自体の恒等写像である場合、$f$ は * E * E$'$ の同型であり、*、および $g$ は逆同型* です。

E$'$ への E の全単射は、逆全単射が必ずしも $\sigma$ 射であるとは限らず、$\sigma$ 射である可能性があることに注意してください。 \* たとえば、位相的空間 A から位相的空間 A$'$ への全単射写像は、逆全単射が連続でなくても連続になる可能性があります (*一般位相*、章 I, § 2, no. 1、注意 1)。 \*

☡

#### 注意 {#ens-iv-s2-n1-rem-2 .statement tag=03VP}

構造 $\Sigma$ の種がいくつかの主基底集合 $x_1, \ldots, x_n$ と補助基底集合 $\mathrm{A}_1, \ldots, \mathrm{A}_m$ を持つとき、$\sigma$ 射は系 $(f_1, \ldots, f_n)$ です。 $f_i$ は、$x_i$ の写像から $y_i$ $(1 \leqslant i \leqslant n)$ であり、これらの写像満たす条件の系は、$(\mathrm{MO_{II}})$ と $(\mathrm{MO_{III}})$ に類似しており、読者は簡単に自分で述べることができます。

### 2. より細かい構造

この切断の残りについては、この構造の種に対して、$\sigma$射の構造$\Sigma$と概念が与えられていると仮定します。 *導入されるすべての概念は、$\Sigma$ だけでなく、想定される $\sigma$-射の概念にも依存します。* 通常、「$\sigma$-射」の代わりに「射」と言うことにします。

¶ Eを集合とし、$\mathscr{S}_1$、$\mathscr{S}_2$をE上の種$\Sigma$の2つの構造とします。 $\mathscr{S}_1$が備わったEの恒等写像が、$\mathscr{S}_2$が備わったEが射である場合、構造$\mathscr{S}_1$は$\mathscr{S}_2$より*より細かい*（そして$\mathscr{S}_2$は$\mathscr{S}_1$より*粗い*）と言われます。

曖昧さを避ける必要がある場合は、 *検討中の $\sigma$射の概念と比較して、 $\mathscr{S}_1$ は $\mathscr{S}_2$ よりより細かいであると言うことにします。他のすべての概念も同様に、この切断で定義されます。

$\mathscr{S}_1$ が $\mathscr{S}_2$ よりもより細かいであるとします。 E$'$が種$\Sigma$の構造$\mathscr{S}'$を備えた集合で、$f$が$\mathscr{S}_2$を備えたEの射で、$\mathscr{S}'$が備えられたE$'$である場合、 $f$ は、$\mathscr{S}_1$ を備えた E の射で、$\mathscr{S}'$ を備えた E$'$ になります。これは、前の定義と $(\mathrm{MO_{II}})$ から続きます。同様に、$g$がE$'$の射で、$\mathscr{S}'$が付与され、Eに$\mathscr{S}_1$が付与されている場合、$g$はまた、E$'$の射で、$\mathscr{S}'$が付与され、Eに付与され、Eに付与されます。 $\mathscr{S}_2$と。

したがって、E には *より細かい* 構造 (種 $\Sigma$ の)、E をソースとして *より多い* 射、E をターゲットとして *より少ない* 射が存在します。

関係「$\mathscr{S}_1$は$\mathscr{S}_2$より粗い」は、E上の種$\Sigma$のすべての構造のうち集合の$\mathscr{S}_1$と$\mathscr{S}_2$の間の*順序関係*です。なぜなら、それは$(\mathrm{MO_{III}})$によって再帰的であり、$(\mathrm{MO_{II}})$によって推移的であり、種$\Sigma$の構造がより細かいかつ他のよりも粗い場合、2つの構造は$(\mathrm{MO_{III}})$によって同一であるからです。一般的な定義 (章 III, § 1, no. 14) に従って、E 上の 2 つの構造種 $\Sigma$ は、一方が他方よりもより細かいであれば *同等* であると言われます。 構造は、他より *より細かい* (つまり *粗い*) であり、それとは区別される場合、他のより *厳密により細かい* (つまり *厳密に粗い*) であると言われます。

*例*

#### 例 1 {#ens-iv-s2-n2-exa-1 .statement tag=03VQ}

集合にグラフ $s$ がある順序構造は、$s \subset s'$ の場合に限り、グラフ $s'$ がある順序構造よりもより細かいです。他の語、関係 $s$ に対する $x \leqslant y$ は、$s'$ に対する $x \leqslant y$ を意味します。これは、章 III, § 1, no. 4、例 3 で指定された定義に従っています。

#### 例 2 {#ens-iv-s2-n2-exa-2 .statement tag=03VR}

集合 A 上の同じ種 $\Sigma$ の 2 つの代数構造 F、F' を考えます。ここで、F と F' は、これら 2 つの構造の合成の (どこでも定義されている) 法則のグラフです。この場合 (no. 1、例 2) の射の定義から、$F \subset F'$ の場合に限り、F は F' よりもより細かいになります。しかし、F と F' は両方とも同じ領域 $A \times A$ を持つ関数グラフであるため、$F = F'$ が必要です。他の語では、種 $\Sigma$ の 2 つの *比較可能な* 構造は必然的に *同一* です。

#### 例 3 {#ens-iv-s2-n2-exa-3 .statement tag=03VS}

V、V' を同じ集合上の 2 つのトポロジとします。 A. V が V よりもより細かいであると言うのは、この場合 (no. 1、例 3) の射の定義により、次のことを意味します。 $V' \subset V$;他の語では、位相 V' のオープン集合である A のすべての部分集合は、位相 V のオープン集合です (したがって、より細かい位相の方がオープンになります) 集合あります）。

#### 注意 {#ens-iv-s2-n2-rem-1 .statement tag=03VT}

私たちは、同じ種 $\Sigma$ の比較可能な 2 つの構造が必然的に同一である例 (例 2) に出会ったところです。他にもそのような例 : 線形順序構造、 \* コンパクト トポロジ、フレシェ空間構造 (射は連続線形写像)、分割環の絶対値 (または評価) によって定義されるトポロジ、など \*

このような構造 $\Sigma$ の場合、*全単射* である E から E' への射 $f$ は *同型射* です。なぜなら、E上の構造$\mathscr{S}$を$f$によってE'に輸送すると、種の構造$\Sigma$が得られます。これはE'上の構造$\mathscr{S}'$よりも細かく、したがって$\mathscr{S}'$と一致します。

### 3. イニシャル構造

集合の家族 $(A_\iota)_{\iota \in I}$ が、それぞれ構造 $\mathscr{S}_\iota$ の種 $\Sigma$ に恵まれていると考えてください。 E を集合とし、それぞれの $\iota \in I$ について、$f_\iota$ を *of* E *into* $A_\iota$ 写像とします。 E 上の種 $\Sigma$ の構造 $\mathscr{S}$ は、以下の性質を持っている場合、家族* $(A_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in I}$ に関して *イニシャル構造であると言われます。

(IN) E' 上の任意の集合 E'、種 $\mathscr{S}'$ の任意の構造、および *E' *into* E の任意の写像 $g$ を考慮すると、関係

「$g$はE'の射をEに変換したものです」

関係と*同等*です

「それぞれの $\iota \in I, f_\iota \circ g$ は、E' の射を $A_\iota$ に変換します。」

CST9。 *家族に関して* E $(\mathrm{A}_\iota,\ \mathscr{S}_\iota,\ f_\iota)_{\iota \in \mathrm{I}}$ に最初の構造が存在する場合、*それは種のすべての構造の中で最も粗いものです* $\Sigma$ *E に * それぞれの写像* $f_\iota$ * は射であり、したがって一意です*。

$\mathscr{I}$ を E のイニシャル構造とし、$\mathscr{S}$ を E の種 $\Sigma$ の構造とし、それぞれの $f_\iota$ が射であるとします。 $i$ が、$\mathscr{S}$ を備えた E の恒等写像を、$\mathscr{I}$ を備えた E に変換すると、$f_\iota \circ i$ は、すべての $\iota \in \mathrm{I}$ に対して射となり、条件 (IN) は、$i$ が射であることを示します。これは、(no. 2) $\mathscr{S}$ が $\mathscr{I}$ より *より細かい* であることを意味します。一方、$g$ がそれ自体上で E の恒等写像 ($\mathscr{I}$ を付与) である場合の適用 (IN) では、($(\mathrm{MO_{III}})$ によって) それぞれの $f_\iota$ が E の射となって $\mathrm{A}_\iota$ になることがわかり、完了します。 証明。

$f_\iota$ が射である種 $\Sigma$ のすべての構造の中で最も粗い種 $\Sigma$ が E 上に存在する可能性がありますが、この構造は $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)$ に関する初期構造ではありません (練習問題 6)。

次の *推移性基準* があります。

CST10。 *E *を集合とし、* $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ *集合の族とし、それぞれ* $\iota \in \mathrm{I}$ *$\mathscr{S}_\iota$ *種の構造を * $\Sigma$ * $\mathrm{A}_\iota$ とします。 *$(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$ *を* Iの分割とし、*そして* $(\mathrm{B}_\lambda)_{\lambda \in \mathrm{L}}$を* Lによってインデックス付けされた集合のファミリーとします。 *それぞれ* $\lambda \in \mathrm{L}$ *let* $h_\lambda$ *be 写像 of* E *into* $\mathrm{B}_\lambda$、*and for each* $\lambda \in \mathrm{L}$ *そしてそれぞれ* $\iota \in \mathrm{J}_\lambda$ *let* $g_{\lambda\iota}$ *be 写像 of* $\mathrm{B}_\lambda$ *into* $\mathrm{A}_\iota$、*そして* $f_\iota = g_{\lambda\iota} \circ h_\lambda$ にしましょう。 *それぞれ* $\lambda \in \mathrm{L}$ について、 *最初の構造* $\mathscr{S}'_\lambda$ *上* $\mathrm{B}_\lambda$ *家族に関して* $(\mathrm{A}_\iota, \mathscr{S}_\iota, g_{\lambda\iota})_{\iota \in \mathrm{J}_\lambda}$ が存在すると仮定します。 *次の主張は同等です* :

(a) *家族に関して* $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$ *E 上に、イニシャル構造* $\mathscr{I}$ が存在します。

(b) *家族に関して* $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$ *E 上に、イニシャル構造* $\mathscr{I}'$ が存在します。

*さらに、これらの主張は * $\mathscr{I} = \mathscr{I}'$ を暗示します。

F に種 $\Sigma$ の構造が与えられた F を集合とし、E への F の写像を $u$ とします。 定義関係により、「$h_\lambda \circ u$ は F から $\mathrm{B}_\lambda$ への射である」が以下と同等であることに注目してください。 関係 「すべての $\iota \in \mathrm{J}_\lambda$、$g_{\lambda\iota} \circ h_\lambda \circ u = f_\iota \circ u$ は、F の $\mathrm{A}_\iota$ への射です。」 関係

(1) 「すべての $\lambda \in \mathrm{L}$、$h_\lambda \circ u$ は、F の $\mathrm{B}_\lambda$ の射です」

したがって、 は関係と同等です

(2) 「すべての$\iota \in \mathrm{I}$, $f_\iota \circ u$ は、F の $\mathrm{A}_\iota$ への射」です。

さて、$\mathscr{I}'$が$(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$家に関して最初の構造であると言うことは、関係(1)は関係「$u$は$\mathscr{I}'$を備えたFからEの射」であることを意味します。そして、家族$(A_i,\,\mathscr{S}_i,\,f_i)_{i\in I}$に関して、$\mathscr{I}$が最初の構造であると言うのは、関係(2)が関係と等価であることを意味します。「$u$は、$\Gamma$を備えたFからEの射である」。したがって、最初の構造の一意性の性質を考慮した結果です。

### 4. 構造のイニシャルの例

I。 *構造の逆像.* Iが単一の元の集合からなるであるとき、$(A,\,\mathscr{S},\,f)$に対する最初の構造は、$f$の下の*逆像と呼ばれます構造 $\mathscr{S}$* (存在する場合)。

\* 位相は、写像 $f$ の下に常に逆像を持ちます。しかし、これは順序構造や代数構造には当てはまりません。 \*

II。 *構造を誘導します。* Aを種$\Sigma$の構造$\mathscr{S}$を備えた集合とし、BをAの部分集合とし、$j$をBの標準単射をAに与えます。 構造 B (存在する場合) の $j$ の下の逆像は、B の $\mathscr{S}$ によって誘導された *構造と呼ばれます。

定義されている集合のすべての部分集合に同じ種の順序構造誘導する構造。ただし、有向集合の構造には当てはまりません。 \* 位相誘導する位相は、それが定義されている集合のすべての部分集合にありますが、コンパクトな位相は一般に誘導するコンパクトな位相にはなりません。 集合 A 上の代数構造は、一般に、任意の部分集合 B 上に同じ種の誘導する構造を形成しません。 A に与えられた構造が、どこでも定義されている合成の法則で構成されている場合、B がこれらの法則のそれぞれに関して安定している必要がありますが、この必要な条件が常に十分であるとは限りません。 \*

一般基準 CST10 は、誘発された構造に対して次の *推移性基準* を与えます。

CST11. *BをAの部分集合、CをBの部分集合、$\mathscr{S}$をA上の種$\Sigma$の構造とし、B上の同じ種の誘導する構造$\mathscr{S}'$とします。 C に種 $\Sigma$ のうち $\mathscr{S}$ 誘導する構造が C に$\Sigma$ $\mathscr{S}'$ 誘導する構造と、構造が誘発された場合に限り、 C by $\mathscr{S}$ と $\mathscr{S}'$ は同一になります。*

CST12。 *A、A' を 2 つの集合に、種 $\Sigma$ の構造 $\mathscr{S}$、$\mathscr{S}'$ を与えたものとする。 B を A の部分集合、B' を A' の部分集合とします。 B (それぞれ B') 上の種 $\Sigma$ の $\mathscr{S}$ (それぞれ $\mathscr{S}'$) 誘導する構造と仮定します。 $f$ が $f(B)\subset B'$ となるような A から A' への射である場合、B の $f$ と一致するである B への B の写像は射になります ($\mathscr{S}$ によって誘導された構造に関して) $\mathscr{S}'$).*

$j$ (それぞれ $j'$) を B (それぞれ B') の標準単射を A (それぞれ A') にするとします。 定義までに$f\circ j=j'\circ g$になります。 $f$ と $j$ は射なので、(MO$_{\mathrm{II}}$) による $f\circ j$ も同様です。しかしその後、$j'\circ g$ は射となり、写像 $g$ は最初の構造の定義により射になります。

III。 *積構造.* $(A_i)_{i\in I}$ を集合の家族とし、それぞれの集合 $A_i$ で、$\mathscr{S}_i$ を種 $\Sigma$ の構造とします。 $E=\prod_{i\in I}A_i$ を家族 $(A_i)_{i\in I}$ (章 II, § 5) の *積* とし、$\operatorname{pr}_i$ は $E$ の $A_i$ の射影を表すとします。家族 $(A_i,\mathscr{S}_i,\operatorname{pr}_i)_{i\in I}$ に関する最初の構造 (存在する場合) は、構造 $\mathscr{S}_i$ の *積* と呼ばれます。

\* 順序構造の家族は常に積構造を認めますが、合計順序構造の家族には必ずしも同じことが当てはまります。 群構造の家族は常に積構造を認めますが、分裂した家族環構造に同じことが当てはまる必要はありません。トポロジーのファミリーは常に積構造を認めますが、局所的にコンパクトな空間の構造のファミリーには必ずしも当てはまりません。この場合、族が *有限* であれば、同じ種の積構造が存在しますが、族が *無限* であれば、1 つである必要はありません (cf. *一般位相*、章 I, § 9, no. 7、提案 14)。 \*

基準 CST10 により、 積構造に対して次の *結合性基準* が生じます。

CST13。 *$(A_i)_{i\in I}$ を集合の族とし、各添字 $i\in I$ について、$\mathscr{S}_i$ を $A_i$ の種 $\Sigma$ の構造とします。 $(J_\lambda)_{\lambda\in L}$を$I$の分割とします。各部分積 $B_\lambda=\prod_{i\in J_\lambda}A_i$ で、家族 $(\mathscr{S}_i)_{i\in J_\lambda}$ が積構造 $\mathscr{S}'_\lambda$ を認めたとします。次に、家族 $(\mathscr{S}_i)_{i\in I}$ は、家族 $(\mathscr{S}'_\lambda)_{\lambda\in L}$ が積構造 $\mathscr{S}'$ と $E=\prod_{i\in I}A_i$ の標準写像を認めた場合に限り、積構造 $\mathscr{S}$ を認めます。 $\mathscr{S}$ を $F=\prod_{\lambda\in L}B_\lambda$ に重ね、$\mathscr{S}'$ (章 II, § 5, no. 5) を付与すると、同型になります。*

CST10 の他のの適用により、 積構造によって誘発される構造に関して次の基準が得られます。

CST14。 *$(A_i)_{i\in I}$を集合の族とし、それぞれの$i\in I$に対して、$\mathscr{S}_i$を$A_i$上の種$\Sigma$の構造とします。それぞれの $i\in I$ について、$B_i$ を $A_i$ の部分集合とします。 $B_i$ に各 $\mathscr{S}_i$ 誘導する構造 $\mathscr{S}'_i$ があり、積 $E=\prod_{i\in I}A_i$ にはその族の積である構造 $\mathscr{S}_0$ が存在すると仮定します。 $(\mathscr{S}_i)$。したがって、次の主張は同等です:*

(a) 集合 $B=\prod_{i\in I}B_i\subset E$ には、$\mathscr{S}_0$ によって誘発された構造 $\mathscr{S}$ が存在します。

(b) 集合 $B$ には、構造 $(\mathscr{S}'_i)$ のファミリーの積である構造 $\mathscr{S}'$ が存在します。

*さらに、これらの主張は $\mathscr{S}=\mathscr{S}'$ を暗示します。*

$j_\iota$ を $\mathrm{B}_\iota$ の $\mathrm{A}_\iota$ の標準単射とし、$j$ を B の E の標準単射とし、$p_\iota$ を $\mathrm{A}_\iota$ の E の射影とし、$p'_\iota$ を B の射影とします$\mathrm{B}_\iota$。すると、すべての $\iota \in \mathrm{I}$ に対して $p_\iota \circ j = j_\iota \circ p'_\iota$ が得られます。 CST10 により、$\mathscr{S}$ はファミリー $(\mathrm{A}_\iota, \mathscr{S}_\iota, p_\iota \circ j)_{\iota \in \mathrm{I}}$ に関する最初の構造であり、$\mathscr{S}'$ はファミリー $(\mathrm{A}_\iota, \mathscr{S}_\iota, j_\iota \circ p'_\iota)_{\iota \in \mathrm{I}}$ に関する最初の構造です。したがって、結果は次のとおりです。

¶ 逆像と積の概念は、次の基準によって関連付けられます。

CST15。 *$(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ を集合の族とし、それぞれの $\iota \in \mathrm{I}$ について、$\mathscr{S}_\iota$ を $\mathrm{A}_\iota$ の種 $\Sigma$ の構造とし、$f_\iota$ を集合 E の写像とします。 $\mathrm{A}_\iota$。 積集合 $\mathrm{A} = \prod_{\iota \in \mathrm{J}} \mathrm{A}_\iota$ に、$(\mathscr{S}_\iota)_{\iota \in \mathrm{I}}$ という家族の積構造 $\mathscr{S}$ が存在するとします。そして、構造 $\mathscr{S}$ が A に E の写像 $x \to f(x) = (f_\iota(x))$ の下に逆像があり、これら 2 つの構造が同一である場合に限り、家族 $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$ に関して最初の構造が存在します。

$f_\iota = \mathrm{pr}_\iota \circ f$ 以降、この基準は CST10 の特殊なケースです。

#### 注意 {#ens-iv-s2-n4-rem-1 .statement tag=03VU}

$(\mathscr{S}_\lambda)_{\lambda \in \mathrm{L}}$ を *同じ* 集合 A 上の種 $\Sigma$ の構造の家族とする。 $\mathrm{A}_\lambda$ は構造 $\mathscr{S}_\lambda$ を備えた A を集合と表し、$\mathrm{I}_\lambda$ は A の恒等写像を$\mathrm{A}_\lambda$ に表します。 B を積集合 $\mathrm{A}^{\mathrm{L}} = \prod_{\lambda \in \mathrm{L}} \mathrm{A}_\lambda$ とし、$\Delta$ をこの積 (章 II, § 5, no. 3) の対角とします。 $h$ を A の $\Delta$ に対する対角線写像とすると、$h(x)$ は元 $(x_\lambda)_{\lambda \in \mathrm{L}}$ となり、すべての $\lambda \in \mathrm{L}$ に対して $x_\lambda = x$ となります。ファミリ $(\mathscr{S}_\lambda)$ の B 積構造 $\mathscr{S}'$ が存在するとします。 $h$ は単射であるため、基準 CST 15 は、$\mathscr{S}'$ によって誘導された $\Delta$ に構造 $\mathscr{S}''$ が存在する場合に限り、家族 $(\mathrm{A}_\lambda, \mathscr{S}_\lambda, \mathrm{I}_\lambda)_{\lambda \in \mathrm{L}}$ に関して初期構造 $\mathscr{S}$ が存在することを示します。 $\mathscr{S}''$ は、$\mathscr{S}$ を $h$ によって $\Delta$ に転送することで得られる構造と同一になります。特に、すべての構造 $\mathscr{S}_\lambda$ が同一である場合、$h$ は、$\Delta$ に対する A (この構造を備えた) の *同型* です。

次の基準もあります。

CST16。 *$(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$、$(\mathrm{B}_\iota)_{\iota \in \mathrm{I}}$ を、同じ集合によってインデックス付けされた集合の 2 つのファミリーとします。それぞれの $\iota \in \mathrm{I}$ について、$\mathscr{S}_\iota$ を $\mathrm{A}_\iota$ の種 $\Sigma$ の構造とし、$\mathscr{S}'_\iota$ を $\mathrm{B}_\iota$ の種 $\Sigma$ の構造とします。ファミリ $(\mathscr{S}_\iota)$ (それぞれ $(\mathscr{S}'_\iota)$) の $\mathrm{A} = \prod_{\iota \in \mathrm{I}} \mathrm{A}_\iota \left( \text{resp. on } \mathrm{B} = \prod_{\iota \in \mathrm{I}} \mathrm{B}_\iota \right)$ 積構造 $\mathscr{S}$ (それぞれ $\mathscr{S}'$) が存在すると仮定します。それぞれの $\iota \in \mathrm{I}$ について、$f_\iota$ を $\mathrm{A}_\iota$ の射から $\mathrm{B}_\iota$ にします。次に、写像 $f = (f_\iota)_{\iota \in \mathrm{I}}$ は A の射を B に変換します。*

$p_\iota$ (それぞれ $q_\iota$) を、$\mathrm{A}_\iota$ に対する A の射影 (それぞれ $\mathrm{B}_\iota$ に対する B) とします。次に$q_\iota \circ f = f_\iota \circ p_\iota$です。 $f_\iota$ と $p_\iota$ は射なので (基準

CST9)、$f_i \circ p_i$ は (MO$_\Pi$) により射です。したがって、$f$ は (IN) によって射になります。

#### 注意 {#ens-iv-s2-n4-rem-2 .statement tag=03VV}

通常の構造のほとんどでは、CST16 で指定された条件で十分であるだけでなく、$f$ が射 (cf. 練習問題 7) であることが必要です。特に、これは次の状況で当てはまります (たとえば、$\Sigma$ が順序構造、\* または群構造の種、またはトポロジカル構造 * の種である場合など、cf. 練習問題 8 の場合に発生します)。

☡

¶ すべての $i\in I$ に対して $a_i\in A_i$ となるような族 $(a_i)_{i\in I}$ が存在します。また、$\lambda\ne i$ のときに $y_i=x_i$ と $y_\lambda=a_\lambda$ を $r_i(x)=(y_\lambda)$ とすると、それぞれの写像 $r_i$ はそれぞれの射になります。 $A_i$から$A$へ。というのは、$f=(f_i)$ が $A$ の射から $B$ になる場合、すべての $i\in I$ に対して $f_i=q_i\circ f\circ r_i$ を書くことができ、それを適用するのに十分です (MO$_\Pi$)。

¶ 次の条件が満たされる場合、$r_i$ は射になることに注意してください。

(a) 種$\Sigma$の構造を備えた集合$E$ごとに、定数写像$z\mapsto a_i$は、$E$の$A_i$への射です。つまり、各 $x\in I$ について、$p_x\circ r_i$ は、$x=i$ の場合は恒等写像であり、$x\ne i$ の場合は定数写像 $z\mapsto a_x$ であるため、$A_i$ から $A_x$ への射です。 積構造の定義により、$r_i$ は $A_i$ の射から $A$ になります。

¶ 例上記満たすは (a) だけでなく、次の条件も含みます。

(b) 種 $\Sigma$ の集合 $A'_i=A_i\times\prod_{x\ne i}\{a_x\}$、構造 $\mathscr{I}$ 誘導する構造ごと。

¶ $p_i$～$A'_i$の制限を$p'_i$とします。 条件 (a) と (b) の両方が満たされる場合、$p'_i$ は $A'_i$ の同型から $A_i$ になります。 $p'_i=p_i\circ j_i$ 以降、$j_i$ は $A'_i$ の標準単射を $A$ にすると、$p'_i$ は (MO$_\Pi$) により射になります。 $r_i=j_i\circ {p'_i}^{-1}$もあります。したがって、${p'_i}^{-1}$は、誘導された構造の定義によって、$A_i$の射が$A'_i$になります。

最後に、多くの場合射を特徴付ける次の基準があります。

**CST17.** — $A$ と $B$ を 2 つの集合とし、同じ種 $\Sigma$ の構造 $\mathscr{S}_A$、$\mathscr{S}_B$ を与えます。 $\mathscr{S}_A$と$\mathscr{S}_B$の$A\times B$構造$\mathscr{S}_{A\times B}$、積に存在するとします。 $f$ を $A$ の $B$ への写像とし、$F$ をそのグラフとし、$\pi$ を $A$ の $x\mapsto (x,f(x))$ から $F$ への全単射とします。そして、$f$が$A$の射から$B$になるためには、$\mathscr{S}_{A\times B}$によって誘発された種$\Sigma$の$F$構造に存在し、$F$がこれを備えていることが必要かつ十分です。 構造、$\pi$は、$A$の$F$上の同型になるはずです。

十分性を証明するには、$j$ を $F$ の $A\times B$ の標準単射とします。 $f=\operatorname{pr}_2\circ j\circ\pi$ と書くと、$f$ は 3 つの射のうち仮定合成になります。

¶ 必要性を証明するために、構造 $\mathscr{S}_{\mathbf{A}}$ を全単射 $\pi$ (§ 1, no. 5) によって F に輸送することによって得られる種 $\Sigma$ の構造を $\mathscr{S}_{\mathbf{F}}$ とします。 次に、$\mathscr{S}_{\mathbf{F}}$ が F の $\mathscr{S}_{\mathbf{A} \times \mathbf{B}}$ によって誘導されることを示さなければなりません。 まず、$j$ は F の $\mathbf{A} \times \mathbf{B}$ に対する射であることに注意してください。なぜなら、$j \circ \pi$はAの写像$x \to (x, f(x))$から$\mathbf{A} \times \mathbf{B}$になり、$f$の仮定と積構造の定義のおかげで射になります。したがって、構造 $\mathscr{S}_{\mathbf{F}}$ の定義により、$j$ は射になります。 E が種 $\Sigma$ の構造を備えた集合であり、$g$ が E の F への写像であり、$j \circ g$ が E の $\mathbf{A} \times \mathbf{B}$ への射である場合、$g$ は射であることがまだ示されていません。または、同等に、$g_1 = \overset{-1}{\pi} \circ g$ は E から A への射です。 しかし、$g_1 = \mathrm{pr}_1 \circ (j \circ g)$ 以降、これは積構造の仮定と定義に続きます。

### 5. 決勝構造

集合 $(\mathbf{A}_\iota)_{\iota \in \mathbf{I}}$ の家族が、それぞれ構造 $\mathscr{S}_\iota$ の種 $\Sigma$ に恵まれていると考えてください。 E を集合とし、各 $\iota \in \mathbf{I}$ について $g_\iota$ を写像 *of* $\mathbf{A}_\iota$ *E に *E 上の種 $\Sigma$ の構造 $\mathscr{T}$ は、家族に関して *最後の構造であると言われます* $(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)_{\iota \in \mathbf{I}}$ 次の性質がある場合:

(FI) E 上の任意の集合 E′、種 $\Sigma$ の任意の構造 $\mathscr{S}'$、および任意の写像 $f$ *of* E *into* E′、関係

$$\text{``}f \text{ is a morphism of E into E'''}$$

関係と*同等*です

$$\text{``for all } \iota \in \mathbf{I}, f \circ g_\iota \text{ is a morphism of } \mathbf{A}_\iota \text{ into E'''}.$$

CST18。 *家族に関して* E に最後の構造が存在する場合* $(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)_{\iota \in \mathbf{I}}$、*その場合、それは種* $\Sigma$ *E 上で最も優れた構造であり、*それぞれの写像* $g_\iota$ *は射であるため、一意です*。

$\mathscr{T}$ を E 上の最後の構造とし、$\mathscr{S}$ を E 上の種 $\Sigma$ の構造とし、各 $g_\iota$ は射とします。 $i$ が、$\mathscr{T}$ を備えた E の恒等写像を、$\mathscr{S}$ を備えた E 上に表す場合、$i \circ g_\iota$ は、$\iota \in \mathbf{I}$ ごとに射になります。次に、条件 (FI) は、$i$ が射であることを示します。これは、(no. 2) $\mathscr{S}$ が $\mathscr{T}$ より *粗い* ことを意味します。 適用 (FI) $f$ がそれ自体上で E の恒等写像である ($\mathscr{T}$ が付加されている) 場合に、($(\mathrm{MO_{III}})$ を使用して) それぞれの $g_\iota$ が E への $\mathbf{A}_\iota$ の射であることがわかります。これで完了です。 証明。

E 上に、$g_\iota$ が射である種 $\Sigma$ のすべての構造の中で最も微細な種 $\Sigma$ が E 上に存在する可能性がありますが、この構造は族 $(\mathbf{A}_\iota, \mathscr{S}_\iota, g_\iota)$ に関して最終的な構造ではありません (練習問題 6)。

次の *推移性基準* があります。

CST19。 *E *を集合とし、* $(\mathrm{A}_\iota)_{\iota \in \mathrm{I}}$ *集合の族とし、それぞれ* $\iota \in \mathrm{I}$ *$\mathscr{S}_\iota$ *種の構造を * $\Sigma$ * $\mathrm{A}_\iota$ とします。 *$(\mathrm{J}_\lambda)_{\lambda \in \mathrm{L}}$ *を* Iの分割とし、*そして* $(\mathrm{B}_\lambda)_{\lambda \in \mathrm{L}}$を* Lによってインデックス付けされた集合のファミリーとします。 *それぞれ* $\lambda \in \mathrm{L}$、*$h_\lambda$ *写像の* $\mathrm{B}_\lambda$ *をEにします。 *それぞれ* $\lambda \in \mathrm{L}$ *そしてそれぞれ* $\iota \in \mathrm{J}_\lambda$、*させて* $g_{\iota\lambda}$ *$\mathrm{A}_\iota$の写像を*に* $\mathrm{B}_\lambda$、*そして入れ* $f_\iota = h_\lambda \circ g_{\iota\lambda}$。 *それぞれ* $\lambda \in \mathrm{L}$ について、 *最終的な構造* $\mathscr{S}'_\lambda$ *上* $\mathrm{B}_\lambda$ *家族に関して* $(\mathrm{A}_\iota,\ \mathscr{S}_\iota,\ g_{\iota\lambda})_{\iota \in \mathrm{J}_\lambda}$ があると仮定します。 *次の主張は同等です* :

(a) *家族に関して* $(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$ *E に、最終的な構造* $\mathscr{S}$ が存在します。

(b) *E *家族に関して* $(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$ には、最終的な構造* $\mathscr{S}'$ が存在します。

*さらに、これらの主張は * $\mathscr{S} = \mathscr{S}'$ を暗示しています。

F を種 $\Sigma$ の構造に恵まれた集合とし、$u$ を F への E の写像とします。 定義により、関係 「$u \circ h_\lambda$ は F への $\mathrm{B}_\lambda$ の射である」は次と同等です。 関係

「すべての $\iota \in \mathrm{J}_\lambda$、$u \circ h_\lambda \circ g_{\iota\lambda} = u \circ f_\iota$ は、$\mathrm{A}_\iota$ の射を F に変換します。」

関係

(3) 「すべての $\lambda \in \mathrm{L}$、$u \circ h_\lambda$ は、$\mathrm{B}_\lambda$ の射を F に変換します」

したがって、 は関係と同等です

(4) 「すべての$\iota \in \mathrm{I}$、$u \circ f_i$は$\mathrm{A}_\iota$の射をFに変換します」。

$(\mathrm{B}_\lambda, \mathscr{S}'_\lambda, h_\lambda)_{\lambda \in \mathrm{L}}$ 家族に関して$\mathscr{S}'$ が最後の構造であるということは、関係 (3) が関係 「$u$ は E ($\mathscr{S}'$ を備えた) の射を F に変換したもの」であることを意味します。そして、家族$(\mathrm{A}_\iota, \mathscr{S}_\iota, f_\iota)_{\iota \in \mathrm{I}}$に関してEが最後の構造であるということは、関係(4)が関係「$u$はEの射($\mathscr{S}$を備えたもの)をFにする」ということを意味します。したがって、最終構造の一意性の性質を考慮した結果です。

### 6. 例 / 決勝構造

I。 構造の *直像。* I が 1 つの元の集合からなるであるとき、$(\mathrm{A}, \mathscr{S}, f)$ に関する最後の構造は * の $f$ の下の *直像と呼ばれます。 構造* $\mathscr{S}$ (存在する場合)。

II。 *商構造.* A を集合に種 $\Sigma$ の構造 $\mathscr{S}$ を与え、R を A の同値関係とし、$\varphi$ を商に対する A の標準写像とします。 集合 $\mathrm{E} = \mathrm{A}/\mathrm{R}$ (章 II, § 6, no. 2)。 写像 $\varphi$ の下の構造 $\mathscr{S}$ の直像は、関係 R によって構造 $\mathscr{S}$ の *商* と呼ばれます (存在する場合)。

\* 一般に、順序構造または代数構造は、任意の同値関係 (cf. 章 III, § 1, 練習問題) に関して商構造を認めません。 2)。一方、位相は任意の同値関係に関して常に商構造を認めますが、これはハウスドルフ位相には必ずしも当てはまりません。 \*

A、B をそれぞれ種 $\Sigma$ の構造 $\mathscr{S}$、$\mathscr{S}'$ を備えた 2 つの集合とし、$f$ を A から B への射とする。R を同値関係 $f(x) = f(y)$ とし、$\varphi$ をAの標準写像を$\mathrm{A}/\mathrm{R}$に、$j$を$f(\mathrm{A})$の標準単射をBにします。$\mathscr{S}$がRに関して商構造$\mathscr{S}_0$を認め、$\mathscr{S}'$とします。 $f(\mathrm{A})$の誘導する構造$\mathscr{S}'_0$。次に、*正規の分解* $f = j \circ g \circ \varphi$ の $f$ (章 II, § 6, no. 5) では、$f$ に関連付けられている $\mathrm{A}/\mathrm{R}$ の $f(\mathrm{A})$ への全単射 $g$ は、 *射* (ただし、必ずしも同型であるとは限りません) $\mathrm{A}/\mathrm{R}$ には $\mathscr{S}_0$ が、$f(\mathrm{A})$ には $\mathscr{S}'_0$ が与えられます。 $j \circ g$ は、商構造の定義によって、$\mathrm{A}/\mathrm{R}$ の射が B に変換され、したがって、$g$ は、誘導の定義によって、$\mathrm{A}/\mathrm{R}$ の $f(\mathrm{A})$ に射が変換されます。 構造。

CST20。 *A, A' *を 2 つの集合に *種* $\Sigma$ の構造* $\mathscr{S}$, $\mathscr{S}'$ を与え、 *R (*それぞれ* R') * を * A (*それぞれ* A') の同値関係とする。 *商構造* $\mathscr{S}_0$ (*resp.* $\mathscr{S}'_0$) *of* $\mathscr{S}$ *by* R (*resp.* $\mathscr{S}'$ *by* R') が存在すると仮定します。 *もし* $f$ *が射の* A *into* A' *これは同値関係* R *および* R'と互換性があり、 *そして* $g$ *が $f$ *から移行から商によって得られた写像である場合*、 $g$ *は $\mathrm{A}/\mathrm{R}$ の射を * $\mathrm{A}'/\mathrm{R}'$ に加えます。

$\varphi$ (それぞれ $\varphi'$) を、$\mathrm{A}/\mathrm{R}$ に対する A の標準写像 (それぞれ $\mathrm{A}'/\mathrm{R}'$ に対する A') とします。そうすると$g \circ \varphi = \varphi' \circ f$になります。 $\varphi'$ と $f$ は射なので、$\varphi' \circ f$ by ($\mathrm{MO_{II}}$) です。しかし、その後、$g \circ \varphi$ は射であるため、商構造の定義により、$g$ も射になります。

¶ 推移性基準 CST19 は、特に次の基準を生じさせます。

CST21。 *A を構造* $\mathscr{S}$ *種* $\Sigma$ を備えた集合とし、*R を * A 上の等価関係とし、* $\mathrm{A}/\mathrm{R}$ *商構造* $\mathscr{S}'$ *の* $\mathscr{S}$ *R が存在するようにします。 *S を、R よりも粗い* A 上の同値関係とし、*S を R で * 商した* $\mathrm{A}/\mathrm{R}$ 上の同値関係を * $\mathrm{S}/\mathrm{R}$ とします (II, § 6, no. 7章)。 *その後、* $(\mathrm{A}/\mathrm{R})/(\mathrm{S}/\mathrm{R})$ *商構造* $\mathscr{S}''$ *of* $\mathscr{S}'$ *by* $\mathrm{S}/\mathrm{R}$ ** $\mathrm{A}/\mathrm{S}$ *商構造* $\mathscr{S}_0$ *of* が存在する場合にのみ$\mathscr{S}$ *by* S、*そして標準写像 of* $\mathrm{A}/\mathrm{S}$ (*恵まれた* $\mathscr{S}_0$) *上* $(\mathrm{A}/\mathrm{R})/(\mathrm{S}/\mathrm{R})$ (*恵まれた* $\mathscr{S}''$) *は同型です*。

$\varphi$ を $A/R$ に対する A の標準写像とし、$\psi$ を $(A/R)/(S/R)$ に対する $A/R$ の標準写像とします。 CST19 により、$\mathscr{S}''$ が $(A,\mathscr{S},\psi\circ\varphi)$ に関して最後の構造である場合に限り、$\mathscr{S}''$ は $\mathscr{S}'$ の $S/R$ の商になります。この基準は、関係 $\psi(\varphi(x))=\psi(\varphi(y))$ が S と同等であるという事実から導かれます。

#### 注意 {#ens-iv-s2-n6-rem-1 .statement tag=03VW}

A を $\Sigma$ の構造 $\mathscr{S}$ に恵まれた集合とし、R による $\mathscr{S}$ の $E=A/R$ 商構造 $\mathscr{S}'$ が存在するように、A 上の R を同値関係とします。 $\varphi$をAからEへの標準写像とします。 一般に、E を A に *射* した $\varphi$ (章 II, § 3, no. 8) の *切断* $s$ は存在しません。 このような切断 $s$ が存在し、さらに $s(E)$ に $\mathscr{S}$ によって誘発される構造 $\mathscr{S}''$ が存在するとします。 次に、$j$ が A への $s(E)$ の標準単射を表し、$s=j\circ f$ であれば、全単射 $f$ は $s(E)$ への E の *同型* です。 なぜなら、$f$は誘導された構造の定義により射であり、$g=\varphi\circ j$は(MO$_{\mathrm{II}}$)によりE上に$s(E)$の射となるからです。 $g\circ f$ と $f\circ g$ はそれぞれ E の恒等写像と $s(E)$ であるため、主張は CST8 の帰結です。

### 練習問題 {#ens-iv-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
