---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 2
section_title: Well-ordered sets
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 148-157, 221-229
pdf_pages: 0154-0163, 0227-0235
extraction: ocr
subsections:
    - "no": 1
      title: SEGMENTS OF A WELL-ORDERED SET
      page: 148
      pdf_page: 154
    - "no": 2
      title: THE PRINCIPLE OF TRANSFINITE INDUCTION
      page: 151
      pdf_page: 157
    - "no": 3
      title: ZERMELO'S THEOREM
      page: 152
      pdf_page: 158
    - "no": 4
      title: INDUCTIVE SETS
      page: 154
      pdf_page: 160
    - "no": 5
      title: ISOMORPHISMS OF WELL-ORDERED SETS
      page: 155
      pdf_page: 161
    - "no": 6
      title: LEXICOGRAPHIC PRODUCTS
      page: 157
      pdf_page: 163
statements: 28
exercises: 20
content_sha256: 0b143ad61403a3bbbaad7a44e46bb876167510a10976f9451703771922e12ae3
translated_from: content/en/ens/III/02_s2_well_ordered_sets.md
translation_method: google
source_content_sha256: 529e0877ab160d3b3e3d67615a04958e997ebf0f3443b7d1ff61efd5c0edeeb3
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 76992b75e45281be1d907716a89d8be504743f71c4e7d3b8fff1f40e9d0c1d5d
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 2. 整然としたセット

### 1. 整然とした集合のセグメント

関係 $\mathrm{R}\{x, y\}$ は、R が $x$ と $y$ の間の順序関係であり、各非空集合 E に対して $\mathrm{R}\{x, y\}$ が順序関係を誘導する場合 (すなわち、$x \in \mathrm{E}$ が意味するような順序関係) である場合、$x$ と $y$* の間の *整順序関係であると言われます。 $\mathrm{R}\{x, x\}$; cf. § 1, no. 1), E, ordered by this relation, has a *least element*.

¶ 関係 $y \in \Gamma\langle x\rangle$ が $x$ と $y$ の間で整列関係である場合、整列 $\Gamma$ によって整列された集合 E は *整列* であると言われます。 $\Gamma$ は E の *整序* であると言われます。次の定義はこれと同等です。

#### 定義 1 {#ens-iii-s2-def-1 .statement tag=03JY}

*集合* E * が順序付けられており、* E * の空でないそれぞれの部分集合に少なくとも元がある場合、 * は整列していると言われます。

整然とした集合 E は、E のすべての部分集合 $\{x, y\}$ に少なくとも元があるため、完全に整列しています。 E で上に境界付けされている E のすべての部分集合 A は、E に少なくとも上界を持ちます。

*例*

#### 例 1 {#ens-iii-s2-n1-exa-1 .statement tag=03SX}

$\mathrm{E} = \{\alpha, \beta\}$ を元が異なる集合とします。 $\mathrm{E} \times \mathrm{E}$ の部分集合 $\{(\alpha, \alpha), (\beta, \beta), (\alpha, \beta)\}$ が E 上で整列したグラフであることは簡単に検証できます。

#### 例 2 {#ens-iii-s2-n1-exa-2 .statement tag=03SY}

適切に順序付けされた集合のすべての部分集合 (特に空の部分集合) は、誘導された順序付けによって適切に順序付けされます。

#### 例 3 {#ens-iii-s2-n1-exa-3 .statement tag=03SZ}

\* 順序が整っていない完全な順序集合の存在は、無限の公理 (§ 4, no. 4、系 1 から命題 3、および練習問題 3) と等価です。

#### 例 4 {#ens-iii-s2-n1-exa-4 .statement tag=03T0}

$\Gamma$ が E 上で適切な順序付けである場合、E が有限 (§ 4、練習問題 3) である場合に限り、$\Gamma$ の反対の順序は E 上で適切な順序付けになります。 \*

#### 例 5 {#ens-iii-s2-n1-exa-5 .statement tag=03T1}

E を整然とした集合とします。 E 最大の元 $b$ (§ 1, no. 7) に隣接することで得られる集合 $\mathrm{E}_1$ は、H が $\{b\}$ 以外の $\mathrm{E}_1$ の空でない部分集合、最も小さい元である場合、整列しています。 $\mathrm{H} \cap \mathrm{E}$ は H の最小の元でもあります。

#### 注意 {#ens-iii-s2-n1-rem-1 .statement tag=03JZ}

\* 無限公理 (§ 6, no. 1) の帰結のように、最大の元を含まない整然とした集合が存在します。たとえば、自然な整数の集合 $\mathbf{N}$ です。 \*

#### 定義 2 {#ens-iii-s2-def-2 .statement tag=03QN}

*順序付けられた集合* E、* E の *部分集合では、関係* $x \in \mathrm{S}$、$y \in \mathrm{E}$、*および* $y \leqslant x$ *暗黙* $y \in \mathrm{S}$ *E のセグメントと呼ばれます。

明らかに、E のセグメントのすべての共通部分と和集合は E のセグメントです。S が E のセグメントである場合、S のすべてのセグメントも E のセグメントです。集合 E 自体と空の集合は E のセグメントです。

#### 命題 1 {#ens-iii-s2-prop-1 .statement tag=03QO}

*整然とした集合* E では、*E 以外の* E の *すべてのセグメントは *E *自体が区間* $]\leftarrow, a[$、*どこに* $a \in \mathrm{E}$ です。

S を $\mathrm{S} \neq \mathrm{E}$ となるような E のセグメントとする。 $\mathrm{E} - \mathrm{S}$ は空ではないので、少なくとも元 $a$ があります。 定義 2 により、関係 $x \geqslant a$ は $x \notin \mathrm{S}$ を意味します。そうでなければ、$a \in \mathrm{S}$ になりますが、これは不合理です。従って、$\mathrm{E} - \mathrm{S}$ は区間 $[a, \rightarrow[$ であり、S は区間 $]\leftarrow, a[$ です。

¶ 全順序付けられた集合 E 内のすべての元 $x$ について、セグメント $]\leftarrow, x[$ は、エンドポイント x* を持つ *セグメントと呼ばれ、$\mathrm{S}_x$ で表されます。

E が整列していて空でない場合、$\mathrm{S}_x$ には少なくとも元 $\alpha$ があり、その結果、区間 $[\alpha, x[$ にもなることに注意してください。

E を完全に順序付けられた集合とします。 $\mathrm{S}_x$ の和集合 A は、$x$ が E を通過するので、E に最大の元がない場合は E です。 E が最大の元 $b$ であれば、$\mathrm{A} = \mathrm{E} - \{b\}$ があります。

#### 命題 2 {#ens-iii-s2-prop-2 .statement tag=03QP}

*集合* E\* *整然とした集合* E * のセグメントは、包含によって整然としています。 写像* $x \rightarrow \mathrm{S}_x$ *は、整然とした集合* E *の同型を * E * 以外* E * 自体* のセグメントの集合に重ねたものです。

$x \in \mathrm{E}$ と $y \in \mathrm{E}$ の場合、関係 $x \leqslant y$ は $\mathrm{S}_x \subset \mathrm{S}_y$ を意味し、$x < y$ は $\mathrm{S}_x \neq \mathrm{S}_y$ を意味することは明らかです。従って、写像 $x \rightarrow \mathrm{S}_x$ は、E 自体 (§ 1, no. 12、命題 11) とは異なる E のセグメントの集合 S(E) 上の E の同型であり、その結果、S(E) は整然としています。さらに、E\* は、最大の元を隣接することによって S(E) から得られる整列集合と同型です。

#### 命題 3 {#ens-iii-s2-prop-3 .statement tag=03QQ}

*$(\mathrm{X}_\iota)_{\iota \in \mathbf{I}}$ * を、添字* $(\iota, \varkappa)$ の各対について、集合* $\mathrm{X}_\iota$、$\mathrm{X}_\varkappa$ * の 1 つがもう一方のセグメントであるような、整然とした集合の族とします。次に、集合* $\mathrm{E} = \bigcup_{\iota \in \mathbf{I}} \mathrm{X}_\iota$ * 誘導するの各* $\mathrm{X}_\iota$ に固有の順序が存在します。 *この順序に恵まれた* E *は、整った集合です。 * $\mathrm{X}_\iota$ のすべての * *セグメントは * E のセグメントです。 *それぞれ* $x \in \mathrm{X}_\iota$、*エンドポイントを持つセグメント* $x$ *in* $\mathrm{X}_\iota$ *エンドポイントを持つセグメント* $x$ *in* E; *そして* E の各セグメントは * E *自体、または * $\mathrm{X}_\iota$ の 1 つのセグメントのいずれかです。

最初の主張は、次の一般的な補題の帰結です。

#### 補題 1 {#ens-iii-s2-lem-1 .statement tag=03QR}

*$(\mathrm{X}_\alpha)_{\alpha \in \mathrm{A}}$ * を関係* $\subset$ を基準とした順序集合の家族とする (他の語では、添字 $\alpha$、$\beta$ の各対に対して添字が存在するように) $\gamma$ は $\mathrm{X}_\alpha \subset \mathrm{X}_\gamma$ と $\mathrm{X}_\beta \subset \mathrm{X}_\gamma$ のようになります）。 *添字* $(\alpha, \beta)$ の各対について、 *$\mathrm{X}_\alpha \subset \mathrm{X}_\beta$ のように * $\mathrm{X}_\alpha$ で * $\mathrm{X}_\beta$ の順序によって * 誘発された順序付けは、 * $\mathrm{X}_\alpha$ での指定された順序付けと同じであるとします。 *これらの条件の下には、 集合* $\mathrm{E} = \bigcup_{\alpha \in \mathrm{A}} \mathrm{X}_\alpha$ に固有の順序が存在し、 * 誘導するそれぞれに指定された順序* $\mathrm{X}_\alpha$ が存在します。

$\mathrm{G}_\alpha$ を $\mathrm{X}_\alpha$ での指定された順序のグラフとします。 G が、グラフが $\mathrm{G}_\alpha$ である順序付けの各 $\mathrm{X}_\alpha$ 上で誘導するである E 上の順序付けのグラフである場合、各 $\alpha \in \mathrm{A}$ に対して $\mathrm{G}_\alpha \subset \mathrm{G}$ が必要です。したがって G 含む $\bigcup_{\alpha \in \mathrm{A}} \mathrm{G}_\alpha$ です。一方、E の元の各対 $(x, y)$ には、仮定添字 $\alpha \in \mathrm{A}$ が存在し、$x \in \mathrm{X}_\alpha$ と $y \in \mathrm{X}_\alpha$ が成り立ちます。 $(x, y) \in \mathrm{G}$ の場合、$(x, y) \in \mathrm{G}_\alpha$ があるため、$\mathrm{G} \subset \bigcup_{\alpha \in \mathrm{A}} \mathrm{G}_\alpha$ になります。したがって、E に必要な順序付けが存在する場合、そのグラフは必然的に $\mathrm{G} = \bigcup_{\alpha \in \mathrm{A}} \mathrm{G}_\alpha$ になります。この集合が補題の条件を満たすかどうかは、まだ示されていません。 $\mathrm{G}_\beta \cap (\mathrm{X}_\alpha \times \mathrm{X}_\alpha) = \mathrm{G}_\alpha$ が $\mathrm{X}_\alpha \subset \mathrm{X}_\beta$ であれば、すべての $\alpha \in \mathrm{A}$ に対して $\mathrm{G} \cap (\mathrm{X}_\alpha \times \mathrm{X}_\alpha) = \mathrm{G}_\alpha$ が得られます。一方、仮定からは、E 属するの任意の 3 つの元 $x$、$y$、$z$ は同じ $\mathrm{X}_\alpha$ になります。したがって、$(x, y) \in \mathrm{G}$ は E では順序関係であり、補題が証明されます。

¶ 命題 3 の証明を取り上げます。 まず、それぞれの $\mathrm{X}_\iota$ が E のセグメントであることを示しましょう。 実際、$x \in \mathrm{X}_\iota$、$y \in \mathrm{E}$、$y \leqslant x$ の場合、$\mathrm{X}_\iota \subset \mathrm{X}_\varkappa$ と $y \in \mathrm{X}_\varkappa$ のような添字 $\varkappa$ が存在します。 仮定までに $\mathrm{X}_\iota$ は $\mathrm{X}_\varkappa$ のセグメントであるため、$y \in \mathrm{X}_\iota$ が得られ、主張が証明されます。 同じ推論は、各 $x \in \mathrm{X}_\iota$ について、$\mathrm{X}_\iota$ の端点 $x$ を持つセグメントが E の区間 $]\leftarrow, x[$ と同一であることを証明します。 次に、E が適切に順序付けされていることを示します。 H が E の空ではない部分集合である場合、$\mathrm{H} \cap \mathrm{X}_\iota \neq \emptyset$ となる添字 $\iota \in \mathrm{I}$ が存在します。 $a$ が $\mathrm{X}_\iota$ の $\mathrm{H} \cap \mathrm{X}_\iota$ の最小元である場合、$a$ は E の H の最小元でもあります。 つまり、$x \in \mathrm{H}$ の場合、$\mathrm{X}_\iota \subset \mathrm{X}_\varkappa$ と $x \in \mathrm{X}_\varkappa$ のような添字 $\varkappa \in \mathrm{I}$ が存在します。 できないは $x < a$ です。区間 $]\leftarrow, a[$ は $\mathrm{X}_\iota$ に含まれており、$\mathrm{X}_\varkappa$ は完全に順序付けされているため、$x \geqslant a$ になります。

¶ 最後に、E 自体以外の E のセグメントが、$\mathrm{X}_\iota$ のいずれかのセグメントであることを示さなければなりません。このようなセグメントは形 $]\leftarrow, x[$ (命題 1) であり、$x$ 属するからいくつかの $\mathrm{X}_\iota$ までであるため、これは前の引数の明らか帰結です。

### 2. 超有限の原理帰納法

#### 補題 2 {#ens-iii-s2-lem-2 .statement tag=03K0}

$E$ を整然とした集合とし、$\mathfrak{S}$ を以下のプロパティを持つ $E$ のセグメントの集合とします: (1) セグメント所属から $\mathfrak{S}$ 属するから $\mathfrak{S}$ の各和集合; (2) $S_x\in\mathfrak{S}$ の場合は、$S_x\cup\{x\}\in\mathfrak{S}$。次に、$E$ 属するから $\mathfrak{S}$ までの各セグメント。

属する ～ $\mathfrak{S}$ に該当しない$E$ のセグメントがあるとします。$S$ をそのうちの最小のとします (no. 1, 命題 2)。 $S$ に最大の元がない場合、$S$ は $S$ 自体とは異なる $S$ のセグメントの和集合であり、これらのセグメントは $S$ の定義により属するから $\mathfrak{S}$ になります。したがって $S\in\mathfrak{S}$ ですが、これは不合理です。 一方、$S$ に最大の元 $a$ がある場合、$S=S_a\cup\{a\}$ となり、$S_a$ は $S$ とは異なる $S$ のセグメントであるため、$S_a\in\mathfrak{S}$ になります。しかし、$S\in\mathfrak{S}$もあり、これもまた不条理です。

¶ 便宜上、$E$ が $x\leq y$ によって書かれた関係によって *整然とした* 集合である理論 $\mathscr{T}$ に置くことにします。従って、次の基準があります。

C59。 (超有限の原理帰納法)。 *$R\{x\}$ を $\mathscr{T}$ ($x$ は $\mathscr{T}$ の定数ではない) で関係となるように関係とします。

$$
(x\in E\text{ and }(\forall y)((y\in E\text{ and }y<x)\Rightarrow R\{y\}))\Rightarrow R\{x\}
$$

$\mathscr{T}$の定理です。これらの条件関係 $(x\in E)\Rightarrow R\{x\}$ は、$\mathscr{T}$ の定理です。*

$\mathfrak{S}$ を $(y\in S)\Rightarrow R\{y\}$ となるような $E$ のセグメント $S$ の集合とします。セグメント所属から $\mathfrak{S}$ の各和集合も属するから $\mathfrak{S}$ であることは明らかです。一方、$S_x\in\mathfrak{S}$ の場合、仮定までに $R\{x\}$ になります。従って、場合の分離の方法によって $(y\in S_x\cup\{y\})\Rightarrow R\{y\}$ になります。従って (補題 2) $E\in\mathfrak{S}$ となり、基準が証明されます。

¶ C59の応用では、関係

$$
x\in E\text{ and }(\forall y)((y\in E\text{ and }y<x)\Rightarrow R\{y\})
$$

は通常「帰納的仮定」と呼ばれます。

¶ 以下では、$E$ のセグメント $S$ の各写像 $g$ を集合 $F$ に変換し、各 $x\in S$ をセグメント $S_x=]\leftarrow,x[$ の $g^{(x)}$ 写像で表すものとします。 $E$ から $g(S_x)$ へ、一致すると $S_x$ の $g$ です。これで記法は

C60。 (transfinite 帰納法による写像の定義 。) *$u$ を文字、理論 $\mathscr{T}$ の $\mathrm{T}\{u\}$ 項とします。 $U$ 上には $E$ の集合 $U$ と写像 $f$ が存在し、すべての $x\in E$ に対して $f(x)=\mathrm{T}\{f^{(x)}\}$ が存在します。さらに、集合 $U$ と写像 $f$ は、これらの条件* によって一意に決まります。

まずは一意性を証明しましょう。 $f'$ と $\mathrm{U}'$ が基準の満たす条件であると仮定します。 $\mathfrak{S}$ を E のセグメント S の集合とし、S 上の $f$ と $f'$ 一致するとします。セグメント所属 ～ $\mathfrak{S}$ のすべての和集合も属する ～ $\mathfrak{S}$ であることは明らかです。一方、$\mathrm{S}_x \in \mathfrak{S}$ の場合、$f$ と $f'$ は $\mathrm{S}_x$ に一致するため、$f^{(x)} = {f'}^{(x)}$ になります。従って

$$f(x) = \mathrm{T}\{f^{(x)}\} = \mathrm{T}\{{f'}^{(x)}\} = f'(x),$$

これは $\mathrm{S}_x \cup \{x\} \in \mathfrak{S}$ を示しています。したがって、$\mathrm{E} \in \mathfrak{S}$ (補題 2)、したがって $f' = f$ と $\mathrm{U}' = f'(\mathrm{E}) = f(\mathrm{E}) = \mathrm{U}$ になります。

¶ ここで、$\mathfrak{S}_1$ は、すべての $x \in \mathrm{S}$ に対して $f_\mathrm{S}(x) = \mathrm{T}\{f^{(x)}\}$ が得られるように、S *onto* $\mathrm{U_S}$ の集合 $\mathrm{U_S}$ と写像 $f_\mathrm{S}$ が存在する E のセグメント S の集合を表します。それぞれの $\mathrm{S} \in \mathrm{S}_1$、$f_\mathrm{S}$、$\mathrm{U_S}$ は、証明の最初の部分によって一意に決定されます。特に、$\mathrm{S}'$ と $\mathrm{S}''$ が $\mathrm{S}' \subset \mathrm{S}''$ となる 2 つのセグメント所属から $\mathfrak{S}_1$ である場合、$f_{\mathrm{S}'}$ は $\mathrm{S}'$ の $f_{\mathrm{S}''}(\mathrm{S}')$ 上の写像であり、上の $f_{\mathrm{S}''}$ と一致します。 $\mathrm{S}'$。この注意から、セグメント所属から $\mathfrak{S}_1$ のすべての和集合も、属するから $\mathfrak{S}_1$ (章 II, § 4, no. 6、命題 7) となることがわかります。一方、$\mathrm{S}_x \in \mathfrak{S}_1$ の場合、$\mathrm{S} = \mathrm{S}_x \cup \{x\}$ 写像 $f_\mathrm{S}$ に$f_{\mathrm{S}_x}$ を拡張して定義するとなります。

$$f_\mathrm{S}(x) = \mathrm{T}\{f_{\mathrm{S}_x}\}$$

(章 II, § 4, no. 7、命題 8); $f_\mathrm{S}^{(x)} = f_{\mathrm{S}_x}$ なので、$\mathrm{S}_x \cup \{x\} \in \mathfrak{S}_1$ であることは明らかです。したがって、(補題 2) $\mathrm{E} \in \mathfrak{S}_1$、そして証明が完成します。

¶ 通常、この基準は、* E のセグメントの *すべての写像 h に対して * F の部分集合に * $\mathrm{T}\{h\} \in \mathrm{F}$ があるような集合 F が存在する状況に適用されます。この場合、適用 C60 によって得られる集合 U は、* F の *部分集合です。つまり、上で使用した記法を使用して、$\mathfrak{S}_2$ を、$\mathrm{U_S} \subset \mathrm{F}$ となるような E のセグメント S の $\mathfrak{S}_1$ からなるの部分集合とします。セグメント所属から $\mathfrak{S}_2$ のすべての和集合も属するから $\mathfrak{S}_2$ であることは明らかです。一方、F の仮定は、$\mathrm{S}_x \in \mathfrak{S}_2$ の場合、$\mathrm{S}_x \cup \{x\} \in \mathfrak{S}_2$ があることを意味します。 補題 2 から主張が続きます。

### 3. ゼルメロズ定理

#### 補題 3 {#ens-iii-s2-lem-3 .statement tag=03K1}

*E *を集合に、* $\mathfrak{S}$ * を * $\mathfrak{P}(\mathrm{E})$ の部分集合に、*そして * $p$ * 写像を * $\mathfrak{S}$ *に E *そのように* $p(\mathrm{X}) \notin \mathrm{X}$ *すべて* $\mathrm{X} \in \mathfrak{S}$。 *その後、*E *の部分集合* M と、M * 上に整列* $\Gamma$ * が存在し、次のような* $x \leqslant y$ * 関係* $y \in \Gamma\langle x \rangle$ * そして* $\mathrm{S}_x$ * セグメント* $]\leftarrow, x]$ を示す、

(1) *全員に* $x \in \mathrm{M}$ *私たちには* $\mathrm{S}_x \in \mathfrak{S}$ *と* $p(\mathrm{S}_x) = x$;

(2) $\mathrm{M} \notin \mathfrak{S}$。

$\mathfrak{M}$ を、次の条件の $\mathrm{E} \times \mathrm{E}$ 満たすの部分集合 G の集合とします。

(a) G は $\mathrm{pr}_1 \mathrm{G} = \mathrm{U}$ の整った順序のグラフです。

(b) $x \leqslant y$ が U 上の関係 $(x, y) \in \mathrm{G}$ を示す場合、各 $x \in \mathrm{U}$ について、セグメント $\mathrm{S}_x$ は $\mathrm{S}_x \in \mathfrak{S}$ と $p(\mathrm{S}_x) = x$ になります。

¶ G と G' が M の 2 つの元で、U, U' が最初の射影を表す場合、2 つの集合 U, U' のうちの 1 つがもう一方に含まれ、たとえば $\mathrm{U} \subset \mathrm{U}'$ の場合は $\mathrm{G} = \mathrm{G}' \cap (\mathrm{U} \times \mathrm{U})$ (他の語では順序) であることを示します。 U の関係は U' の順序関係によって誘発され、U は U' の *セグメント* です。

¶ エンドポイント $x$ を持つセグメントが U と U' で同じであり、U と U' の順序によってこのセグメントに誘発される順序が同一であるように、元 $x \in \mathrm{U} \cap \mathrm{U}'$ の集合 V を考えます。 V が U と U' の両方の * セグメント* であり、V で誘発される順序が同じであることは明らかです。従って、$\mathrm{V} = \mathrm{U}$ または $\mathrm{V} = \mathrm{U}'$ のいずれかを示せば、私たちの主張が証明されます。矛盾によって議論し、$\mathrm{V} \neq \mathrm{U}$ と $\mathrm{V} \neq \mathrm{U}'$ を仮定してみましょう。 $x$ を U の $\mathrm{U} - \mathrm{V}$ の最小の元とし、$x'$ を U' の $\mathrm{U}' - \mathrm{V}$ の最小の元とします。 Uには$\mathrm{V} = \mathrm{S}_x$、U'には$\mathrm{V} = \mathrm{S}_{x'}$があります。しかし、仮定、$\mathrm{V} \in \mathfrak{S}$までに、

$$x = p(\mathrm{S}_x), \qquad x' = p(\mathrm{S}_{x'}),$$

つまり$x = x'$です。従って、定義 $x \in \mathrm{V}$ になりますが、これは不合理です。

¶ 従って、no. 1 の命題を適用する 3 を最初の射影 $\mathrm{U} = \mathrm{pr}_1 \mathrm{G}$ ($\mathrm{G} \in \mathfrak{M}$) の集合にすると、整然とした集合が得られます。

$$\mathrm{M} = \bigcup_{\mathrm{G} \in \mathfrak{M}} \mathrm{pr}_1 \mathrm{G}.$$

M 属するから $\mathfrak{M}$ の順序のグラフであることが簡単にわかります。 $\mathrm{M} \in \mathrm{S}$ があった場合、$a = p(\mathrm{M})$ を置くと、$a \notin \mathrm{M}$ になるはずです。従って、M 元 $a$ に最大の元として隣接することができ、集合 $\mathrm{M}' = \mathrm{M} \cup \{a\}$ は適切な順序になります。 M' では $\mathrm{M} = \mathrm{S}_a$ なので、$\mathrm{S}_a \in \mathfrak{S}$ と $p(\mathrm{S}_a) = a$ が必要です。従って、M' の順序のグラフは属するから $\mathfrak{M}$ になりますが、これは不合理です。

$\emptyset \notin \mathfrak{S}$ (特に $\mathfrak{S}$ が空の場合) の場合、補題 3 によって存在が主張される集合 M は空の集合であることに注意してください。これは補題 3 の条件 1 から続きます。

#### 定理 1 (ゼルメロ) {#ens-iii-s2-thm-1 .statement tag=03QS}

*集合* E ごとに *適切に注文できます*。

$\mathfrak{S} = \mathfrak{P}(\mathrm{E}) - \{\mathrm{E}\}$ を E 自体以外の E のすべての部分集合の集合とします。それぞれの $\mathrm{X} \in \mathfrak{S}$ について $p(\mathrm{X}) = \tau_x \ (x \in \mathrm{E} - \mathrm{X})$ とします。 関係 $\mathrm{X} \in \mathfrak{S}$ は $(\exists x)(x \in \mathrm{E} - \mathrm{X})$ を意味するので、$p(\mathrm{X}) \in \mathrm{E} - \mathrm{X}$ (章 I, § 4, no. 1) となり、$p(\mathrm{X}) \notin \mathrm{X}$ となります。従って、補題 3 を適用すると、その結果、$\mathrm{M} \notin \mathfrak{S}$ となるような E の部分集合 M に適切な順序が存在します。しかし、E のうち属するから $\mathfrak{S}$ を満たさない唯一の部分集合は E そのものであり、定理が証明されます。

### 4. 誘導集合

#### 定義 3 {#ens-iii-s2-def-3 .statement tag=03K2}

*順序付けられた集合* E * E のすべての完全に順序付けられた部分集合が * E に上界を含む場合、 * は帰納的であると言われます。

*例*

#### 例 1 {#ens-iii-s2-n4-exa-1 .statement tag=03T2}

$\mathfrak{F}$ を、包含順に並べた集合 A の部分集合の集合とし、完全に順序付けされたすべての部分集合 $\mathfrak{F}$ の $\mathfrak{G}$ $\mathfrak{G}$ の集合の和集合とします。 属するから$\mathfrak{F}$まで。この場合、$\mathfrak{G}$ の集合の和集合は、$\mathfrak{P}(\mathrm{A})$ における $\mathfrak{G}$ の最小の上界であるため、$\mathfrak{F}$ は関係 $\subset$ に関して帰納的です。

#### 例 2 {#ens-iii-s2-n4-exa-2 .statement tag=03T3}

関係 $\subset$ に関して帰納的である重要な部分集合の集合の例は、集合 A の部分集合の写像を集合 B に変換するグラフの集合 $\mathfrak{F}$ です。 なぜなら、$\mathfrak{F}$ は $\mathfrak{P}(\mathrm{A} \times \mathrm{B})$ の部分集合であり、$\mathfrak{F}$ の部分集合 $\mathfrak{G}$ が包含によって完全に順序付けされていると言うのは、$\mathfrak{G}$ の元が写像のグラフであり、これら写像のいずれか 2 つが与えられると、1 つは次のようになります。もう一方の拡大。 $\mathfrak{G}$ の集合の和集合は $\mathfrak{F}$ の元 (章 II, § 4, no. 6, 命題 7) となります。 したがって、A の部分集合の B への写像の集合 $\Phi(\mathrm{A}, \mathrm{B})$ は、$u$ と $v$ の間の順序関係「$v$ が $u$ に拡張される」に関して帰納的です。

#### 例 3 {#ens-iii-s2-n4-exa-3 .statement tag=03T4}

\* 無限公理 (§ 6, no. 1) から、自然整数の整然とした集合は関係 $\leqslant$ に関して帰納的ではないことがわかります。 \*

#### 定理 2 (「ゾーンの補題」) {#ens-iii-s2-thm-2 .statement tag=03QT}

— *すべての帰納的順序集合には極大元があります。*

この定理は、次の結果の特殊なケースです。

#### 命題 4 {#ens-iii-s2-prop-4 .statement tag=03K3}

*E * を順序付けられた集合とし、すべての整然とした部分集合が上に制限されるようにします。すると* E *は極大元になります。*

$v$ が X と $v \notin \mathrm{X}$ の上界である場合、元 $v \in \mathrm{E}$ は E の部分集合 X の *厳密な上界* であると言えます。 $\mathfrak{S}$ を、E に厳密な上界を持つ E の部分集合の集合とし、各 $\mathrm{S} \in \mathfrak{S}$ に対して $p(\mathrm{S}) = \tau_v(v$ を S$)$ の厳密な上界とします。 $p(\mathrm{S})$ は S の厳密な上界です。 適用補題 no. 3 から $\mathfrak{S}$ と $p$ の 3 から、E の部分集合 M と、次を満たす M 上の整列$\Gamma$ が存在することがわかります。 条件/補題 3;特に、M には E に厳密な上界がありません。さらに、順序付け $\Gamma$ は、E の順序付けによって M に引き起こされるものと同じです。なぜなら、M 関係では、「$y\in\Gamma\langle x\rangle$ および $x\ne y$」は $x\in S_y$ と同等です。そして、$p(S_y)=y$ は (E の順序に関して) $S_y$ の上界であるため、E の $x<y$ を意味します。しかし、これは、M から E への単射が真に増加する写像 (M には順序 $\Gamma$ が付与されている) であることを意味します。そして M は完全に順序付けされているため、関係 $y\in\Gamma\langle x\rangle$ と $x\leq y$ は M (§ 1, no. 12, 命題 11) において同等であるということになります。そうなると、E には M の仮定上界 $m$ が存在します。しかし、M には厳密な上界がないため、$m$ は E の極大元であるということになります。

#### 系 1 {#ens-iii-s2-prop-4-cor-1 .statement tag=03K4}

*E を帰納的順序付け集合とし、a を E の元とします。すると、$m\geq a$ となる E の極大元 m が存在します。*

なぜなら、定義 3 から、E の元 $x\geq a$ の集合 F は帰納的であり、F の極大元も E で最大であることがわかります。

#### 系 2 {#ens-iii-s2-prop-4-cor-2 .statement tag=03K5}

*$\mathfrak{F}$ を集合 E の部分集合の集合とし、完全に包含によって順序付けされた $\mathfrak{F}$ のすべての部分集合 $\mathfrak{G}$ について、$\mathfrak{G}$ の集合の和集合 (それぞれ交差) が $\mathfrak{F}$ に属するようにします。この場合、$\mathfrak{F}$ には最大 (または最小) 要素があります。*

### 5. 同型整然としたセット

#### 定理 3 {#ens-iii-s2-thm-3 .statement tag=03K6}

*E と F を 2 つの整った順序のセットとする。その場合、次の 2 つの主張のうち少なくとも 1 つが true になります:*

(1) *F のセグメント上に E の一意の同型が存在します。*

(2) *E のセグメント上に F の一意の同型が存在します。*

$\mathfrak{F}$ を E の部分集合の写像の集合として、各写像が E のセグメント上で定義され、このセグメントの F のセグメント上の同型となるようにします。 次に、$u$ と $v$ の間の関係 「$v$ 拡大する $u$」によって順序付けられた集合 $\mathfrak{F}$ は帰納的です。 なぜなら、$\mathfrak{G}$ が $\mathfrak{F}$ の完全に順序付けられた部分集合である場合、写像 $u\in\mathfrak{G}$ の領域の和集合 S は E のセグメントの和集合であり、したがってそれ自体 E のセグメントです。 $v$ が $\Phi(E,F)$ (no. 4、例 2) の $\mathfrak{G}$ の最小上界である場合、$v(S)$ は写像 $u\in\mathfrak{G}$ の範囲の和集合であるため、F のセグメントになります。 最後に、$x<y$ となる S の要素 $x$、$y$ に対して、ドメインに $x$ と $y$ の両方が含まれる $u\in\mathfrak{G}$ が存在します ($\mathfrak{G}$ は完全に順序付けされているため)。そして、$v(x)=u(x)<u(y)=v(y)$ より、$v$ は S の $v(S)$ への同型写像であり、私たちの主張は証明されます。

¶ さて、$u_0$ を $\mathfrak{F}$ (no. 4, 定理 2) の極大元とし、$S_0$ を $u_0$ の領域である E のセグメントとします。 $S_0=E$か$u_0(S_0)=F$のどちらかを示せば、定理が証明されます。矛盾によって議論し、$S_0\ne E$ と $u_0(S_0)\ne F$ を仮定してみましょう。次に、元 $a\in E$ と元 $b\in F$ があり、$S_0=]-\leftarrow,a[$ と $u_0(S_0)]=]-\leftarrow,b[$ (no. 1, 命題 1) になります。 $u_1(a)=b$ を入れて、セグメント $]-\leftarrow,a]$ の拡大する $u_0$ から写像 $u_1$ を F に入力します。 $u_1$ はセグメント $]-\leftarrow,b]$ 上の $]-\leftarrow,a]$ の同型であるため、この矛盾するは $\mathfrak{F}$ における $u_0$ の最大値となります。

¶ 定理 3 でアサートされた一意性は、次の補題の帰結です。

#### 補題 4 {#ens-iii-s2-lem-4 .statement tag=03K7}

*E、F を 2 つの整然とした集合とし、f、g を E から F への 2 つの増加する写像とし、$f(E)$ が F のセグメントであり、g が真に増加するであるとします。次に、すべての $x\in E$ に対して $f(x)\leq g(x)$ です。*

逆に、$f(y)>g(y)$ が空ではない、元 $y\in E$ の集合があると仮定します。その場合、この集合には少なくとも元 $a$ が含まれます。 $x<a$ の場合、$g$ は真に増加するであるため、$f(x)\leq g(x)<g(a)<f(a)$ になります。 $f(E)$ は F の線分であるため、$g(a)=f(z)$ となるような $z\in E$ が存在します。 $f$ は増加するなので、$f(z)<f(a)$ は $z<a$ を意味します。したがって、

$$f(z)\leq g(z)<g(a)=f(z),$$

それは不合理です。

#### 系 1 {#ens-iii-s2-lem-4-cor-1 .statement tag=03K8}

*E のセグメント上の整然とした集合 E の同型のみが、それ自体上の E の恒等写像です。*

定理 3に$F=E$を入れます。

#### 系 2 {#ens-iii-s2-lem-4-cor-2 .statement tag=03K9}

*E、F を 2 つの整った順序のセットとする。 F の線分 T 上に E の同型 $f$ が存在し、E の線分 S 上に F の同型 $g$ が存在する場合、$S=E$、$T=F$、および $g,f$ は互いに逆数でなければなりません*。

$g\circ f$ は、E のセグメント $g(T)\subset S$ 上の E の同型です。 系 1 により $g(T)=S=E$ が得られ、$g\circ f$ は E の恒等写像です。同様に、$f\circ g$ は F の恒等写像、結果よってです。

#### 系 3 {#ens-iii-s2-lem-4-cor-3 .statement tag=03KA}

*整然とした集合 E のすべての部分集合 A は E のセグメントと同型です。*

定理 3 により、形 $S_a$ の A のセグメント上に E の同型 $g$ が存在しないことを証明するのに十分です。存在する場合、$g$ は、E の真に増加する写像を E に変換すると $g(a)\in S_a$ になり、他の語は $g(a)<a$ になります。しかし、これは不等式矛盾する補題 4 ($f$ は恒等写像として) です。

### 6. 辞書編集積

$(E_\iota)_{\iota\in I}$ を、*整然とした* 集合 I によってインデックス付けされた順序集合のファミリーとします。 積集合 $E=\displaystyle\prod_{\iota\in I}E_\iota$ および関係を検討してください

$$
\text{``}x\in E\text{ and }y\in E,\text{ and for the least index }\iota\in I\text{ such that }\operatorname{pr}_{\iota}x\ne\operatorname{pr}_{\iota}y,\text{ we have }\operatorname{pr}_{\iota}x<\operatorname{pr}_{\iota}y\text{''},
$$

これを$R\{x,y\}$で表すことにします。 $R\{x,x\}$ は $x\in E$ と等価であり、$R\{x,y\}$ は $R\{x,x\}$ と $R\{y,y\}$ を暗示し、$(R\{x,y\}\text{ and }R\{y,x\})$ は $x=y$ を暗示していることは明らかです。また、$(R\{x,y\}\text{ and }R\{y,z\})$ が $R\{x,z\}$ を意味することも簡単に検証できます (元 $\operatorname{pr}_{\iota}x$、$\operatorname{pr}_{\iota}y$、$\operatorname{pr}_{\iota}z$ の 3 つのうち少なくとも 2 つが等しくない、最小の添字 $\iota\in I$ を考えてください)。したがって、$R\{x,y\}$ は、積集合 E* の *順序関係です。この関係とその順序定義するは *辞書編集順序関係* と $E$ の *辞書編集 * と呼ばれます ($I$ と $E_\iota$ での指定された順序によって引き起こされます)。この順序の集合 E は、順序集合 $(E_\iota)_{\iota\in I}$ の族の *辞書編集積* と呼ばれます。それぞれの $E_\iota$ が *完全に順序付けされている*場合、辞書編集上の積も *完全に順序付けられています*。

### 練習問題 {#ens-iii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
