---
book: top
book_title: General Topology
chapter: II
chapter_title: Uniform Structures
section: 2
section_title: Uniformly continuous functions
lang: ja
source: top-i-iv
book_pages: 174-181, 207-208
pdf_pages: 0180-0187, 0213-0214
extraction: ocr
subsections:
    - "no": 1
      title: UNIFORMLY CONTINUOUS FUNCTIONS
      page: 174
      pdf_page: 180
    - "no": 2
      title: COMPARISON OF UNIFORMITIES
      page: 175
      pdf_page: 181
    - "no": 3
      title: INITIAL UNIFORMITIES
      page: 176
      pdf_page: 182
    - "no": 4
      title: INVERSE IMAGE OF A UNIFORMITY; UNIFORM SUBSPACES
      page: 177
      pdf_page: 183
    - "no": 5
      title: LEAST UPPER BOUND OF A SET OF UNIFORMITIES
      page: 178
      pdf_page: 184
    - "no": 6
      title: PRODUCT OF UNIFORM SPACES
      page: 179
      pdf_page: 185
    - "no": 7
      title: INVERSE LIMITS OF UNIFORM SPACES
      page: 180
      pdf_page: 186
statements: 27
exercises: 6
content_sha256: f53748724fd17811f99bd98df55decda178a53c83c37cf9182801c145c6af1d6
translated_from: content/en/top/II/02_s2_uniformly_continuous_functions.md
translation_method: google
source_content_sha256: 92b674d0f20d1a67ab0b8298e6f5a7fe7434487139d32666270aa426c8d22f2f
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 74613d910c0c3d532d958c286ffc100aaeb56c36276bf940e67d1432dd784fd8
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 2. 一様連続写像

### 1. 一様連続写像

#### 定義 1 {#top-ii-s2-def-1 .statement tag=0BDH}

*写像 $f$ を制服空間 $X$ から制服空間 $X'$ に変えることは、$X'$ の各取り巻き $V'$ に対して、次のような $X$ の取り巻き $V$ が存在する場合、一様連続であると言われます。 関係 $(x, y) \in V$ は $(f(x), f(y)) \in V'$ を意味します。*

より表現力豊かな項では、$x$ と $y$ が十分に近いときに、$f(x)$ と $f(y)$ が好きなだけ互いに近い場合、$f$ は一様連続であると言えます。

$g = f \times f$ とすると、定義 1 は、*$V'$ が $X'$ の側近であるとき、$\overline{g^{-1}}(V')$ は $X$ の側近であることを意味します*。

#### 例 1 {#top-ii-s2-n1-exa-1 .statement tag=0BDI}

制服空間の恒等写像はそれ自体が一様に連続しています。

#### 例 2 {#top-ii-s2-n1-exa-2 .statement tag=0BDJ}

一様空間から一様空間への定数写像は一様連続です。

#### 例 3 {#top-ii-s2-n1-exa-3 .statement tag=0BDK}

離散均一空間から均一空間へのすべての写像は均一に連続です。

#### 命題 1 {#top-ii-s2-prop-1 .statement tag=0BDL}

一様に連続するすべての写像は連続です。

定義の明らか帰結です。

一方、一様空間 X から一様空間 X' への連続写像は、例 $x \to x^3$ で示されるように \*、それ自体に対する $\mathbf{R}$ の同型写像であるため、一様連続である必要はありません。添加剤の均一性に関して均一に連続しています。 \* (§ 4, no. 1、定理 2 を参照)

#### 命題 2 {#top-ii-s2-prop-2 .statement tag=0BDM}

(a) $f : X \to X'$ と $g : X' \to X''$ が 2 つの一様連続写像である場合、$g \circ f : X \to X''$ は一様連続です。

(b) ユニフォーム空間 X のユニフォーム空間 X の全単射 $f$ は、$f$ と $f$ の逆数が一様連続である場合に限り、同型になります。

これは、積写像 $f \times f$ の項の定義 1 の解釈からすぐに続きます。

### 2. 均一性の比較

no. 1 の命題 2 は、一様連続写像 (集合理論, 章 IV, § 2, no. 1) を一様構造の射としてとることができることを示しています。私たちは将来常に射がそのように選ばれたと仮定することになります。一般的な定義 (集合理論, 章 IV, § 2, no. 2) に従って、これにより、特定の集合における均一性の定義する位数関係が可能になります。 集合 X:

#### 定義 2 {#top-ii-s2-def-2 .statement tag=0BDN}

$\mathfrak{U}_1$ と $\mathfrak{U}_2$ が同じ集合 X 上の 2 つの均一構造である場合、$\mathfrak{U}_1$ は $\mathfrak{U}_2$ よりもより細かい (そして $\mathfrak{U}_2$ は $\mathfrak{U}_1$ よりも粗い) と言われます。 $X_i$ 集合 X を均一構造 $\mathfrak{U}_i$ ($i = 1,2$) で表すと、恒等写像 $X_1 \to X_2$ は一様連続です。

$\mathfrak{U}_1$ が $\mathfrak{U}_2$ よりもより細かいであり、$\mathfrak{U}_2$ とは異なる場合、$\mathfrak{U}_1$ は厳密に $\mathfrak{U}_2$ よりもより細かいであると言います (そして、$\mathfrak{U}_2$ は厳密には $\mathfrak{U}_1$ よりも粗いです)。

2 つの均一性は、一方が他方よりより細かいであれば同等であると言われます。

#### 例 {#top-ii-s2-n2-exa-1 .statement tag=0BDO}

集合 X の均一性の順序付けられた集合では、個別の均一性が最も細かく、取り巻きの集合が単一の元 $X \times X$ で構成される均一性が最も粗いです。

次の命題は、 定義の明らか帰結 、 no. 1 の 1 です:

#### 命題 3 {#top-ii-s2-prop-3 .statement tag=0BDP}

$\mathfrak{U}_1$ と $\mathfrak{U}_2$ が集合 X 上の 2 つの一様性である場合、$\mathfrak{U}_2$ のすべての側近が $\mathfrak{U}_1$ の側近である場合に限り、$\mathfrak{U}_1$ は $\mathfrak{U}_2$ よりもより細かいになります。

#### 系 {#top-ii-s2-n2-cor-1 .statement tag=0BDQ}

$\mathfrak{U}_1$ と $\mathfrak{U}_2$ を集合 X 上の 2 つの一様性とし、$\mathfrak{U}_1$ が $\mathfrak{U}_2$ よりもより細かいであると仮定します。この場合、$\mathfrak{U}_1$ によって誘発された位相は、$\mathfrak{U}_2$ によって誘発された位相よりもより細かいになります。

これは、近傍 (章 I, , no. 2, 命題 3) の項でのトポロジの比較の直後に続きます。

#### 注意 1 {#top-ii-s2-n2-rem-1 .statement tag=0BDR}

均一性 $\mathfrak{U}_1$ が均一性 $\mathfrak{U}_2$ よりも厳密にはより細かいであるにもかかわらず、誘導された 2 つのトポロジーが同一であることが起こります。次の例はこれを示しています。

$X$ を空ではない集合とします。 $X$ の各有限分割 $\varpi = (A_i)_{1 \leq i \leq n}$ について、$V_{\overline{\varpi}}$ を次のように表します。
$$
\bigcup_i A_i \times A_i.
$$
集合 $V_{\overline{\varpi}}$ 次に形 $X$ で統一性のある取り巻きの基本系 $\mathfrak{U}$。 なぜなら、$\varpi$ が$X$ の有限分割である場合、$\Delta \subset V_{\overline{\varpi}}$ と $V_{\overline{\varpi}} \circ V_{\overline{\varpi}} = \overline{V_{\overline{\varpi}}} = V_{\overline{\varpi}}$ (§ 1, no. 1, 例 2) が存在します。そして、$\varpi' = (B_j)$ と $\varpi'' = (C_k)$ が $X$ の 2 つの有限分割である場合、集合 $B_j \cap C_k$ は空ではなく、形は有限分割 $\varpi$ の $X$ であり、次のようになります。 $V_{\overline{\varpi}} \subset V_{\overline{\varpi'}} \cap V_{\overline{\varpi''}}$。 $\mathfrak{U}$ は、$X$ 上の有限分割の一様性と呼ばれます。 $x \in X$ 集合 $\{x\}$ と $C\{x\}$ 形はそれぞれ $X$ の有限分割であるため、$\mathfrak{U}$ によって誘導される位相は離散的な位相です。 それにもかかわらず、$X$ が無限大である場合、$\mathfrak{U}$ が厳密には離散均一性よりも粗いことは明らかです。

#### 注意 2 {#top-ii-s2-n2-rem-2 .statement tag=0BDS}

$f : X \to X'$ が均一連続写像である場合、$X$ の均一性をより細かいの均一性で、$X'$ の均一性をより粗い均一性 (no. 1、命題 2) で置き換えるすれば、$f$ は均一連続のままです。他の語、より細かいでは、$X$の均一性が高く、$X'$の均一性が粗いほど、写像の$X$から$X'$までが均一に連続しています。

### 3. 初期均一性

#### 命題 4 {#top-ii-s2-prop-4 .statement tag=0BDT}

$X$ を集合とし、$(Y_i)_{i \in I}$ を均一のファミリー 空間とし、それぞれの $i \in I$ について、$f_i$ を $X$ の写像から$Y_i$ にします。 それぞれの $i \in I$ について、$g_i$ が $f_i \times f_i$ を表すものとします。 $\mathfrak{S}$ を形の $X \times X$ $\overline{g_i}(V_i)$ の部分集合の集合とします。ここで、$i \in I$ と $V_i$ は $Y_i$ の取り巻きであり、$\mathfrak{B}$ をすべての有限数の集合とします共通部分

$$
\text{(1)} \quad U(V_{i_1}, \ldots, V_{i_n}) = \overline{g_{i_1}}(V_{i_1}) \cap \cdots \cap \overline{g_{i_n}}(V_{i_n})
$$

$\mathfrak{S}$の集合。この場合、$\mathfrak{B}$ は、$X$ の均一性 $\mathfrak{U}$ の取り巻きの基本系であり、これは家族 $(f_i)$ (集合理論, 章) に関する$X$ の初期均一構造です。 IV, § 2, no. 3)、特に $\mathfrak{U}$ は $X$ 上で最も粗い均一性であり、すべての写像 $f_i$ は均一に連続しています。しかしそうでない場合、$h$ を制服空間 $Z$ の写像から $X$ にします。この場合、$h$ は、写像 $f_i \circ h$ のそれぞれが一様連続である場合に限り、一様連続になります ($X$ に一様性 $\mathfrak{U}$ が付与されている場合)。

$\mathfrak{B}$ が公理 $(B_1)$ および $(U'_1)$ を満たすことがすぐにわかります。 $W_i = \overline{g}_i^{-1}(V_i)$ の場合、$\overline{W}_i = \overline{g}_i^{-1}(\overline{V}_i)$ と $\dot{W}_i = \dot{g}_i^{-1}(\dot{V}_i)$。したがって、$\mathfrak{B}$ は公理 $(U'_{II})$ と $(U'_{III})$ も満たし、したがって、$X$ 上の均一性$\mathfrak{U}$ の取り巻きの基本系です。さらに、$\mathfrak{U}$ の定義と定義 1 および no. 1 から、$f_i$ が各添字 $i \in I$ に対して一様連続であることがすぐに続きます。したがって、(no. 1, 命題 2) $h$ がそうであれば、$f_i \circ h$ は各 $i \in I$ に対して一様連続です。逆に、$f_i \circ h$ が各 $i \in I$ に対して一様連続であると仮定し、集合 $U(V_{i_1}, \ldots, V_{i_n})$ を考えます。 仮定により、$1 \leq k \leq n$ のような各 $k$ に対して、関係 $(z, z') \in W_k$ が $[f_{i_k}(h(z)), f_{i_k}(h(z'))] \in V_k$ を暗示するように、$Z$ の側近$W_k$ が存在します。もし
$$
W = \bigcap_k W_k,
$$
これらの $n$ 関係は、$z$ と $z'$ が $W$ に近いときに同時に満たされ、その結果、$(h(z), h(z')) \in U(V_{i_1}, \ldots, V_{i_n})$ が得られ、証明が完了します。

#### 系 {#top-ii-s2-n3-cor-1 .statement tag=0BDU}

*$f_i$が一様に連続している最も粗い均一性$\mathfrak{U}$によって引き起こされる$X$の位相は、$f_i$が連続している最も粗い位相でもあります。

これは、後者の位相 (章 I, § 2, no. 3、命題 4) の点の定義の近傍の明らか帰結です。

初期値構造 (*集合理論*、章 IV, § 2, no. 3、基準 CST 10) の一般特性は、特に次の *推移性* 性質を意味します。

#### 命題 5 {#top-ii-s2-prop-5 .statement tag=0BDV}

*$X$を集合、$(Z_i)_{i \in I}$を均一空間のファミリー、$(J_\lambda)_{\lambda \in L}$を$I$の分割、$(Y_\lambda)_{\lambda \in L}$を$L$でインデックス付けされた集合のファミリーとします。それぞれの $\lambda \in L$ について、$h_\lambda$ を $X$ の写像から $Y_\lambda$ にします。それぞれの$\lambda \in L$とそれぞれの$i \in J_\lambda$について、$g_{i\lambda}$を$Y_\lambda$の写像を$Z_i$にします。そして$f_i = g_{i\lambda} \circ h_\lambda$にしましょう。それぞれの $Y_\lambda$ に、写像 $g_{i\lambda}$ ($i \in J_\lambda$) が均一に連続する最も粗い均一構造を持たせます。このとき、$f_i$が一様に連続している$X$上の最も粗い均一構造は、$h_\lambda$が一様に連続している$X$上の最も粗い均一構造と同じです。

### 4. 逆像均一性。制服部分空間

$X$を集合、$Y$を空間、$f$写像を$X$から$Y$とします。 $f$が一様連続である$X$上の最も粗い均一性$\mathfrak{U}$は、$Y$の一様構造の$f$の下にある*逆像*と呼ばれます。 no. 3の命題4と、共通部分の逆像を与える公式から、$Y$形の側近の$g = f \times f$の下で、$\mathfrak{U}$の側近の基本系が逆像になるということになります。 $\mathfrak{U}$ によって誘発される位相は、$Y$ (no. 3、系から命題 4) の位相の $f$ の下にある *逆像* です。

#### 注意 {#top-ii-s2-n4-rem-1 .statement tag=0BDW}

$f : X \to Y$ が全射であれば、$Y$ の取り巻きは $X$ の取り巻きの $g$ の下にある直像になります。

均一空間 $X$ から均一空間 $X'$ への写像 $f$ は、$X'$ の均一性の $f$ の逆画像が $X$ の均一性よりも粗い場合に限り、均一に連続します。

$A$を制服空間$X$の部分集合とします。 $X$ の均一性によって $A$ に引き起こされる均一性は、標準単射 $A \to X$ の下での後者の逆像です。 no. 3 の命題 4 により、これは次の定義と同等になります。

#### 定義 3 {#top-ii-s2-def-3 .statement tag=0BDX}

$A$を制服空間$X$の部分集合とします。取り巻きの集合が$X$の取り巻きの集合の$A \times A$の痕跡である$A$の均一性を、$X$の均一性によって$A$に誘発される均一性と呼びます。

$A$ に誘発された均一性によって誘発された位相は、$X$ の位相によって $A$ に誘発された位相と同じです。 集合 $A$ は、$X$ の均一性と位相を合わせて、$X$ の均一性部分空間と呼ばれます。

$A$ が均一空間 $X$ の部分集合で、$f : X \to X'$ が均一連続写像である場合、制限 $f|A$ は $A$ の均一連続写像になります。 $X'$。 $A' \subset X'$ が $f(X) \subset A'$ である場合、$X$ の写像は$X'$ の部分空間 $A'$ に変換され、$f$ と同じグラフを持ち、再び一様連続になります (no. 3、命題) 4)。

$B \subset A \subset X$ の場合、$X$ のユニフォーム部分空間 $B$ は、$X$ のユニフォーム部分空間 $A$ (誘導ユニフォームの推移性) のユニフォーム部分空間 $B$ と同一です。 構造; no. 3、命題 5)。

#### 命題 6 {#top-ii-s2-prop-6 .statement tag=0BDY}

$A$ をユニフォーム空間 $X$ の密集部分集合とします。次に、制服部分空間 $A$ 形の側近の$X \times X$ で、$X$ の側近の基本的な系が閉じられます。

$A \times A$ は、$X \times X$ (章 I, § 4, no. 3、命題 7) に密集しています。 $V$ を $A$ の開かれた取り巻きとします。それは$A \times A$の共通部分で、$X$のオープンな取り巻き$U$がいます。 $U \subset \overline{V}$ (章 I, § 1, no. 6、命題 5) があり、この関係と $\overline{V} \subset \overline{U}$ は、命題 2 の § 1, no. 2、系 2 を考慮して、命題を確立します。

### 5. 集合中最小の上界の均一性

集合 $X$ の均一性の各ファミリー $(\mathfrak{U}_i)_{i \in I}$ は、$X$ のすべての均一性の順序集合のうち、少なくとも上界 $\mathfrak{U}$ を持っています。 no. 3 を命題を適用する 4 にするだけで済み、$Y_i$ は集合 $X$ となり、$\mathfrak{U}_i$ が統一され、$f_i$ は恒等写像 $X \to Y_i$ となります。 $\mathfrak{U}$ によって誘発される位相は、$\mathfrak{U}_i$ によって誘発されるトポロジの最小の上界です。

no. 3 の命題 4 からも、$X$ が空ではなく、$\mathfrak{U}_i$ が $\mathfrak{U}_i$ の側近のフィルターである場合、$\mathfrak{U}$ の側近のフィルターは、$\mathfrak{U}_i$ (章) のフィルターの最小の上界であることがわかります。 I, § 6, no. 2）。

#### 例 {#top-ii-s2-n5-exa-1 .statement tag=0BDZ}

$\varpi$ が空ではない集合 $X$ の有限分割 $(A_i)_{1 \leq i \leq n}$ である場合、集合 $V_\varpi = \bigcup_i (A_i \times A_i)$ はそれ自体で $X$ 上の均一性 $\mathfrak{U}_\varpi$ の側近の基本系を構成します。 (§ 1, no. 1、例 2); $X$ (no. 2, 注意 1) 上の有限分割の均一性は、$\mathfrak{U}_\varpi$ の最小の均一性上界になります。

#### 注意 {#top-ii-s2-n5-rem-1 .statement tag=0BE0}

$X$ の均一性のファミリー $(\mathfrak{U}_i)$ は、$X$ のすべての均一性の順序付けられた集合の最大の下界も持ちます。つまり、$X$ のすべての均一性の集合のうち最小の上界があり、これはそれぞれの均一性よりも粗いです。 $\mathfrak{U}_i$ ($X$ のすべての均一性のうち集合には最小の元があるため、そのような均一性が存在します)。しかし、($X$ が空ではないと仮定すると) この均一性の側近のフィルターは、必ずしも $\mathfrak{U}_i$ の側近のフィルターの共通部分ではありません。これは、この後者のフィルターには満たす公理 $(U_{III})$ (練習問題 4) が必要ないからです。

### 6. 積の制服空間

#### 定義 4 {#top-ii-s2-def-4 .statement tag=0BE1}

*$(X_i)_{i \in I}$ * が制服空間のファミリーである場合、このファミリーの積制服空間は積集合*
$$
X = \prod_{i \in I} X_i
$$
*射影* $pr_i : X \to X_i$ の最も粗い均一性が与えられています。
*一様連続です。この均一性は * $X_i$ の均一性の積と呼ばれ、* 空間* $X_i$ * の均一性は * $X$ の因子と呼ばれます。

$X$ 上の積の均一性によって引き起こされる位相は、$X_i$ (no. 3、系 ～ 命題 4) のトポロジーの積と同じです。

#### 命題 7 {#top-ii-s2-prop-7 .statement tag=0BE2}

*$f = (f_i)$ *写像を制服空間* $Y$ * から積制服空間* $X = \prod_{i \in I} X_i$ にします。 *そうすると* $f$ *それぞれ* $f_i$ *一様連続*である場合に限り、*一様連続になります。

$f_i = pr_i \circ f$ 以降、これは no. 3 の命題 4 の特殊なケースです。

#### 系 {#top-ii-s2-n6-cor-1 .statement tag=0BE3}

*$(X_i)_{i \in I}, (Y_i)_{i \in I}$ * を、同じ集合* $I$ によってインデックス付けされた均一空間の 2 つのファミリーとします。 *それぞれ* $i \in I$、*$f_i$ *写像の* $X_i$ *を* $Y_i$にします。 *それぞれ* $f_i$ *が一様連続である場合、積写像*も同様です
$$
f : (x_i) \to (f_i(x_i)).
$$
*逆に、* $X_i$ *が空でなく、* $f$ *が一様連続である場合、それぞれ* $f_i$ *は一様連続です。*

f は $x \to (f_i(\mathrm{pr}_i x))$ と書くことができ、したがって系の最初の部分は命題 7 から続きます。 2 番目の部分は、$\prod_{i \in I} X_i$ の点 $a = (a_i)$ を考慮し、「$a$ (それぞれ $a_\kappa$) で連続」というフレーズを「一様連続」に置き換えて、命題 1 の系 1 のI、 、no. 1 章の議論を繰り返すことによって証明されます。

初期均一性 (no. 3、命題 5) の一般基準推移性は、トポロジカル空間 (章 I, § 4, no. 1) の積と同様に、均一空間の積が結合的であり、以下が真であることを示します。

#### 命題 8 {#top-ii-s2-prop-8 .statement tag=0BE4}

*$X$を集合、$(Y_i)_{i \in I}$を制服空間の家族とし、それぞれの$i \in I$について、$f_i$を$X$の写像を$Y_i$にします。 $f$ を $X$ の写像 $x \to (f_i(x))$ から $Y = \prod_{i \in I} Y_i$ とし、$U$ を $f_i$ が一様に連続する$X$ 上の最も粗い均一性とします。次に、$U$ は、$Y$ での積均一性によって$f(X)$ で誘発された均一性の $f$ の下で逆像になります。

#### 系 {#top-ii-s2-n6-cor-2 .statement tag=0BE5}

※各$i \in I$について、$A_i$を$Y_i$の部分空間とします。この場合、$\prod_{i \in I} Y_i$の積の均一性によって$A = \prod_{i \in I} A_i$に生じる均一性は、部分空間$A_i$の均一性の積と同じになります。

加法では、$X_1, X_2$ が 2 つの均一空間で、$a_1$ が $X_1$ のいずれかの点である場合、写像 $x_2 \to (a_1, x_2)$ は部分空間 $\{a_1\} \times X_2$ 上の$X_2$ の同型であることがすぐにわかります。 $X_1 \times X_2$の;したがって:

#### 命題 9 {#top-ii-s2-prop-9 .statement tag=0BE6}

*$f$ を、積均一空間 $X_1 \times X_2$ から均一空間 $Y$ への一様連続マッピングとする。その後、すべての部分マッピング*

$$
x_2 \to f(x_1, x_2)
$$

*$X_2$ から $Y$ は一様連続です。*

他の語では、2 つの引数の一様連続写像は、それぞれについて個別に一様連続です。

\* 章 I, § 4, no. 2、注意 2 で与えられた \* 例は、この命題の逆が false であることを示します。 \*

### 7. ユニフォーム空間の逆極限

$I$ を部分順序付け集合とし、部分順序付けが $\alpha \leq \beta$ と書かれているものとします。それぞれの $\alpha \in I$ について、$X_\alpha$ を均一の空間とし、添字 $\alpha, \beta$ のそれぞれの対について、$\alpha \leq \beta$ を$f_{\alpha \beta}$ を$X_\beta$ の写像から$X_\alpha$ にします。

We shall say that $(X_\alpha, f_{\alpha\beta})$ is an inverse system of uniform spaces if (i) $(X_\alpha, f_{\alpha\beta})$ is an inverse system of sets (cf. Chapter I, Appendix, no. 1) and (ii) whenever $\alpha \leq \beta$, $f_{\alpha\beta}$ is uniformly continuous. $X = \varprojlim X_\alpha$ では、標準写像 $f_\alpha : X \to X_\alpha$ が一様に連続している最も粗い均一性は、$X_\alpha$ の均一性の逆数極限 ($f_{\alpha\beta}$ に関して) と呼ばれ、この最も粗い均一性を備えた集合 $X$ は逆数と呼ばれます。 空間 $(X_\alpha, f_{\alpha\beta})$ の逆系の極限。 章 I, , no. 4 (命題 9 を除く) で確立されたトポロジカル空間の逆極限のすべての性質は、「一様連続」によって置き換える "位相" と "一様連続" によって "連続写像" が成り立つ場合、引き続き有効です。 写像」。 加法に

#### 命題 10 {#top-ii-s2-prop-10 .statement tag=0BE7}

$I$ を有向集合とし、$(X_\alpha, f_{\alpha\beta})$ を$I$ でインデックス付けされた均一空間の逆数系とし、$J$ を $I$ の共終値部分集合とします。 それぞれの $\alpha \in I$ について、$f_\alpha$ を $X = \varprojlim X_\alpha$ の標準写像から $X_\alpha$ にし、$g_\alpha$ を $f_\alpha \times f_\alpha$ とします。 次に、集合 $\overline{g}_\alpha^{-1}(V_\alpha)$ の家族は、$\alpha$ が $J$ を通過し、各 $\alpha \in J$、$V_\alpha$ が$X_\alpha$ の側近の基本系を通過し、$X$ の側近の基本系になります。

証明は読者に任せます。これは、章 I, § 4, no. 4 の命題 9 の証明をそのまま適応させたものです。

最後に、$X_\alpha$ の均一性の逆極限によって引き起こされる $X = \varprojlim X_\alpha$ 上の位相は、$X_\alpha$ のトポロジーの逆極限です。

### 練習問題 {#top-ii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
