---
book: evt
book_title: Topological Vector Spaces
chapter: II
chapter_title: CONVEX SETS AND LOCALLY CONVEX SPACES
section: 4
section_title: Locally convex spaces
lang: ja
source: evt-i-v
book_pages: TVS II.23-TVS II.36, TVS II.74-TVS II.76
pdf_pages: 0060-0073, 0111-0113
extraction: ocr
subsections:
    - "no": 1
      title: Definition of a locally convex space
      page: 23
      pdf_page: 60
    - "no": 2
      title: Examples of locally convex spaces
      page: 25
      pdf_page: 62
    - "no": 3
      title: Locally convex initial topologies
      page: 26
      pdf_page: 63
    - "no": 4
      title: Locally convex final topologies
      page: 27
      pdf_page: 64
    - "no": 5
      title: The direct topological sum of a family of locally convex spaces
      page: 29
      pdf_page: 66
    - "no": 6
      title: Inductive limits of sequences of locally convex spaces
      page: 31
      pdf_page: 68
    - "no": 7
      title: Remarks on Fréchet spaces
      page: 34
      pdf_page: 71
statements: 33
exercises: 17
content_sha256: 56e4de869510b0bc2cfd6662ac40691502c9cd2bac31f4d1f38b2fa0f8fe7366
translated_from: content/en/evt/II/04_s4_locally_convex_spaces.md
translation_method: google
source_content_sha256: 739b1018258c46c62f41370f616639ef1cdd404280e387353dc0a0e48e83ef94
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 9cd67e9f5ab4343474fd0497e97e4ecfa315378126099f216b5eb961c41d86ca
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 4。局所的に凸空間

### 1. 局所凸型の定義空間

#### 定義 1 {#evt-ii-s4-def-1 .statement tag=07E4}

— *凸集合である 0 の近傍の基本系が存在する場合、トポロジカルベクトル空間は局所的に凸 (実) です。*

このような空間は *局所的に凸な空間* と呼ばれます。その位相は *局所凸位相* と呼ばれます。

この本の残りの部分で研究する $\mathbf{R}$ 上のトポロジー ベクトル空間は、ほぼすべて局所的に凸です。

$V$ が局所凸空間 $E$ の 0 の凸近傍である場合、$V \cap (-V)$ は 0 の対称凸近傍です。 As the closure of a convex set is convex (II, p. 13, prop. 14) it follows from I, p. 7, prop. 4 that the neighbourhoods of 0 in $E$ which are *closed, symmetric and convex*, form a fundamental system of neighbourhoods invariant under homotheties of centre 0 and ratio $\neq 0$.

#### 命題 1 {#evt-ii-s4-prop-1 .statement tag=07E5}

— *$\mathfrak{S}$ を、吸収性、対称性、凸面の集合から形成されたベクトル空間 $E$ 上のフィルター 基底とします。 Then the set $\mathfrak{B}$ of transforms of the sets of $\mathfrak{S}$ by homotheties of ratio $> 0$ is a fundamental system of neighbourhoods of 0 for a locally convex topology on $E$.*

明らかに、$\mathfrak{B}$ は、I、p. 7、プロップのフィルター基底満たす (EV_I) および (EV_{II}) です。 4; $V \in \mathfrak{S}$ であれば $\frac{1}{2}V + \frac{1}{2}V = V$ であるため、(EV_{III}) も満たします。

$\mathscr{T}$ が 0 の近傍の基本系に対して $\mathfrak{B}$ を持つ E 上の局所凸位相である場合、集合 $(1/n) \ V$、ここで $n$ は整数 $> 0$ で変化し、 Vは、$\mathfrak{S}$、形、位相$\mathscr{T}$の0の近傍の基本的な系で変化します。そして、E のすべての $x \neq 0$ に対して整数 $n$ と集合 $V \in \mathfrak{S}$ が存在し、$nx \notin V$ となる場合に限り、$\mathscr{T}$ はハウスドルフです。さらに、$\mathfrak{S}$ が列挙可能である場合、位相 $\mathscr{T}$ は計量可能な局所凸位相です。逆に、$\mathscr{T}$ が測定可能な局所凸型位相である場合、$\mathscr{T}$ に対して 0 の閉じた対称凸型近傍の数え切れない基本関数系が存在することは明らかです。

#### 系 {#evt-ii-s4-n1-cor-1 .statement tag=07E6}

— トポロジカルベクトル空間 E の *位相 $\mathscr{T}$ は、半ノルム* (II、p. 3) の集合によって定義されます。*ただし、$\mathscr{T}$ が局所的に凸である場合*に限ります。

E 上のすべての半ノルムは凸写像であるため、条件が必要です。したがって、$\alpha > 0$ では、$p(x) \leq \alpha$ である $x \in E$ の集合が凸です (II、p. 17、系)。逆に、V が E の 0 の対称で閉じた凸型近傍である場合、V の *ゲージ* $p$ は、V が E 点の集合満たすの $x$ であるような E 上の準ノルムです。 $p(x) \leq 1$ (II、p. 20、提案 23)。

これはさらに、局所的に凸な位相 $\mathscr{T}$ が、$\mathscr{T}$* に対して連続する *すべての半ノルムの集合によって定義されることを示しています。さらに、$\mathscr{T}$ が測定可能である場合、それは *数えられる* 集合の半規範によって定義されます。

系からプロップまで。 1、半ノルムの集合によって定義されたトポロジーに関する § 1 のすべての結果は、実際のベクトル空間に対する局所凸トポロジーに特に当てはまります。局所凸ハウスドルフ空間 E は、局所凸である完成 $\hat{E}$ を持ちます。完全で計量可能な局所凸型空間は *Fréchet 空間* と呼ばれます。すべてのバナッハ空間はフレシェ空間です。

#### 命題 2 {#evt-ii-s4-prop-2 .statement tag=07E7}

— * f を、局所的に凸な空間 E のベクトル部分空間 M 上で定義された連続線型形式とします。その場合、E 上で定義され、f* の拡大である連続線型形式 h が存在します。

上の系とII、p. 7、corから。 2 では、すべての $y \in M$ に対して $|f(y)| \leq p(y)$ となるような連続半ノルム $p$ が E 上に存在します。ハーン・バナッハ著(II, p. 23, cor. 1) 拡大する $f$ である E 上に線型形式 $h$ が存在し、すべての $x \in E$ に対して $|h(x)| \leq p(x)$ となるので、これは $h$ が連続であることを意味します (II, p. 6、提案 5)。

#### 注意 {#evt-ii-s4-n1-rem-1 .statement tag=07E8}

— $g$ が積空間 $\mathbf{R}^I$ の M の連続線形写像である場合、$\mathbf{R}^I$ の E の連続線形写像 $h$、つまり $g$ の拡大が存在します。 $g = (g_i)$ を書く場合、$g_i$ は M で定義された連続線型形式であり、$i \in I$ ごとに $g_i$ の拡大 $h_i$ があり、$h_i$ は E で連続線型形式になります。連続線形写像 $h = (h_i)$ には必要なプロパティがあります。

F が局所凸ハウスドルフ空間であり、F の M の連続線形写像である $g$ である場合、$g$ の拡大である F の E の連続線形写像が必ずしも存在するわけではないことに注意してください (IV、p. 55、演習​​ 16、c))。ただし、M が有限次元の場合には、そのような拡大が存在します (*cf.* cor. 2、以下)。

#### 系 1 {#evt-ii-s4-prop-2-cor-1 .statement tag=07E9}

— *E を局所凸空間とします。 $x_0 \in E$ が $\{0\}$ の閉包内にない場合、$f(x_0) \neq 0$* で E 上に定義された連続線型形式 f が存在します。

プロップを適用します。 2 を、$x_0$ によって生成された 1 次元のベクトル空間 M と、M 上で定義された線型形式 $\xi x_0 \mapsto \xi$ に変換します。これは、I、p. 12 によって、prop されます。 2、連​​続です。

#### 系 2 {#evt-ii-s4-prop-2-cor-2 .statement tag=07EA}

— M を E の有限次元ベクトル部分空間、局所凸ハウスドルフ空間とします。このとき、E の閉じたベクトル部分空間 N が存在します。これは、E における M のトポロジー的補集合です。

E における M へのトポロジー的補数が存在するのは、それ自体上の M の恒等写像が M 上の E の連続線形写像に拡張でき、その場合、写像は必然的に連続射影子になります (GT, III, § 6.2, 系)。さて、M は空間 $\mathbf{R}^n$ (I, p. 13, th. 2) と同型であるため、これは上記の注意から続きます。

#### 命題 3 {#evt-ii-s4-prop-3 .statement tag=07EB}

— 局所的に凸な空間 E では、プリコンパクト集合のバランスのとれた凸エンベロープ自体がプリコンパクト集合です。

A を E のプレコンパクト集合とします。E の 0 の平衡凸近傍である V が与えられると、A が S、近傍の和集合に含まれるような有限個の点 $a_i \in A$ ($1 \leq i \leq n$) が存在します。 $a_i + V$ ($1 \leq i \leq n$)。したがって、A の平衡凸状包絡線 C は、S の平衡凸状包絡線 T に含まれます。しかし、T は B + V に含まれます。ここで、B は、点 $a_i, -a_i$ ($1 \leq i \leq n$) の有限集合の凸包絡線を示します。ここで、B はプリコンパクト (II, p. 14, cor. 2) です。したがって、近傍 $b_k + V$ の和集合に $B_k$ が含まれるような、有限個の点 $b_k \in B$ ($1 \leq k \leq m$) が存在します。するとCは近傍$b_k + 2V$の和集合に含まれ、命題が証明されます。

無限次元の局所凸ハウスドルフ空間では、コンパクト集合の凸包絡線は必ずしも閉じていないことに注意してください (II、p. 74、演習 3)。

#### 系 {#evt-ii-s4-n1-cor-2 .statement tag=07EC}

— 局所凸ハウスドルフ空間 E において、コンパクト集合 X が完全な凸集合 (E の均一な構造で完全) に含まれる場合、X の凸閉包絡線はコンパクトです。

このエンベロープは完全な空間の閉じた部分集合であるため、完全ですが、プレコンパクトでハウスドルフでもあります。

ただし、不完全な局所凸ハウスドルフ空間では、コンパクト集合の凸閉包絡線はコンパクトである必要はありません (II、p. 87、演習 2)。

### 2. 局所凸の例空間

1) 中心 0 の開いた立方体は凸であるため、空間 $\mathbf{R}^n$ は局所的に凸です (II、p. 9、提案 6)。したがって、これはすべての実位相位相ベクトル空間または有限次元にも当てはまります。実際には、上記と I, § 2.3 から次のようになります。 2 ただし、E がハウスドルフである場合。そうでない場合、E に関連付けられたハウスドルフ空間 F は有限次元であるため、局所的に凸であり、標準写像 $E \to F$ の下で F の 0 の凸近傍の逆像は凸であり、 の基本系である形 E の 0 の近傍。

2) E を $\mathbf{R}$ のベクトル空間とし、$\mathfrak{B}$ を吸収性、対称性、凸面である E のすべての部分集合の族とします。 プロップにより。 II、p. 23 の 1 から、E 上のすべての局所凸トポロジの中で最も細かい、E 上の局所凸位相 $\mathscr{T}_\omega$ の 0 の基本系近傍が $\mathfrak{B}$ であることがわかります。 This topology is Hausdorff; for let $x \neq 0$ be any point of E; there exists a basis $(i_i)_{i \in I}$ of E with an $\alpha \in I$ such that $e_\alpha = x$; the set of points $y = \sum_i y_i e_i$ such that $|y_\alpha| < 1$ is absorbent, symmetric and convex. 含む $x$ ではありません。 II、p. 24、系から、$\mathscr{T}_\omega$ も E 上の*すべて* 半ノルムの集合によって定義される位相であることがわかり、したがって、すべての半ノルムは $\mathscr{T}_\omega$ で連続です。

In particular, if $u$ is a linear mapping of E in any locally convex space F, the inverse image, under $u$, of every convex neighbourhood of 0 in F is an *absorbent* convex set in E; therefore it is a neighbourhood of 0 for $\mathscr{T}_\omega$ and thus $u$ is *continuous* for $\mathscr{T}_\omega$.

E の凸型集合 C が与えられた場合、すべての行 D 含む $a$, 共通部分 $D \cap C$ の場合、点 $a \in C$ は C の *内部点* であると言います。 含む含む $a$ の開いたセグメント。その他の語 — $a + C$ は *吸収性* です。 集合の点 $a$ E の A は、$a \in C \subset A$ と凸の集合 C が存在し、$a$ が内部の点である場合に限り、E の A の *内部 $\mathscr{T}_\omega$ です。 C。

より一般的には、V を E のアフィン線形多様体、C を V に含まれる凸型集合とします。 ベクトル部分空間 $V_0 = -a + V$、点 0 が集合の内部点である場合、点 $a \in C$ は、* V に対する C の *内部点です。 $C_0 = -a + C$。

E が有限次元の場合、位相 $\mathscr{T}_\omega$ は E 上の正規の位相 (I、p. 13、th. 2) です。これは、E の凸型集合 C のすべての内部点が、標準位相の C の内部にあることを示しています (*cf.* II, p. 74、演習 5)。

3) A を $\mathbf{R}$ 上のベクトル空間 E における対称凸集合とする。 ベクトル部分空間 A によって *生成された * F は、$-A = A$ 以降、A によって生成された凸円錐でもあります。この集合は $x \in A$ と $\lambda \in \mathbf{R}$ の $\lambda x$ の集合です。 集合 A は F および集合 $\lambda A$ に *吸収されます。ここで、$\lambda > 0$、形は、局所的に凸な位相 *on* F (A によって *定義* と言われる) の 0 の近傍の基本系、これは、A の *ゲージ* である半ノルム $p_A$ によって定義されます (II、p. 20、提案 22)。この準ノルムを F に与えることで得られる局所凸型空間を $E_A$ と書きます。 空間 $E_A$ は、$p_A$ が *ノルム* であるか、あるいは A が含む *任意の行* でない場合に限り、*ハウスドルフ* です。 B が E の 2 番目の対称凸面集合で、$A \subset B$ の場合、明らかに $E_A \subset E_B$ と $E_B$ の $E_A$ の標準単射は、A と B によってそれぞれ定義されたトポロジーに対して *連続* です。さらに、$f$ が実数ベクトル空間 $E'$ における E の線形写像であれば、$f(A)$ は $E'$ において凸対称であり、$f$ は $E_A$ *on* $E'_{f(A)}$ の *連続* 線形写像です。

最後に、E がそのベクトル空間構造と互換性のある位相 $\mathscr{T}$ を持ち、V が $\mathscr{T}$ に対して 0 の対称 *凸* 近傍である場合、V によって生成されるベクトル空間は次のようになります。 V は吸収性であり、$E_V$ の E の恒等写像は *連続* であるため、E と同一です。

### 3. 局所的に凸な初期トポロジー

#### 命題 4 {#evt-ii-s4-prop-4 .statement tag=07ED}

*E をベクトル空間とし、$(E_i)_{i \in I}$ を局所凸空間の族とする。それぞれの $i \in I$ について、$f_i$ を $E_i$ の E の線形写像とします。次に、E 上の位相* $\mathscr{T}$ は、各写像 $f_i$ を連続的にする最も粗いもので、局所的に凸の位相になります。

II、p. 24、系を使用すると、これは準ノルム (II、p. 5) によって定義されたトポロジーの対応する性質の特定のケースです。

特に、局所凸空間のすべてのベクトル部分空間、および局所凸空間のすべての積空間は局所凸です。局所凸型空間のすべての射影極限は局所凸型です。

フレシェ空間のすべての *数え切れない積* (特にバナハ空間の数え切れないすべての積) はフレシェ空間です。

すべての局所凸ハウスドルフ空間 E はバナッハ空間の積の部分空間と同型であり、E が完全であればこの部分空間は閉じます (II、p. 5、提案 3)。すべての Fréchet 空間は、Banach 空間の数えられる積の閉じた部分空間と同型です (*loc. cit.*)。

### 4. 局所的に凸の最終トポロジー

#### 命題 5 {#evt-ii-s4-prop-5 .statement tag=07EE}

*E をベクトル空間、$(F_\alpha)_{\alpha \in A}$ をトポロジカルベクトル空間の族とし、各 $\alpha \in A$ について、$g_\alpha$ を E の $F_\alpha$ の線形写像とします。*

(i) *$g_\alpha^{-1}(V)$ が $\alpha$ ごとに $F_\alpha$ で 0 の近傍となるような、E の吸収性対称凸面部分集合 V のファミリーを $\mathfrak{B}$ で示します。ファミリ $\mathfrak{B}$ は、位相 $\mathscr{T}$ の E の 0 の近傍の基本的な系であり、ベクトル空間構造と互換性があります。*

(ii) 局所凸空間における E の *線形写像 f (または E 上の半ノルム) は、すべての添字 $\alpha$、$f \circ g_\alpha$ (それぞれ $p \circ g_\alpha$) が連続である場合に限り、$\mathscr{T}$ について連続です。 $F_\alpha$.*

(iii) *位相 $\mathscr{T}$ は、$g_\alpha$ が連続している E 上の局所凸トポロジーの中で最も細かいものです。

*さらに、位相 $\mathscr{T}$ は、線形写像 (それぞれ準ノルム) の条件 (ii) を満たす E 上の唯一の局所凸位相です。

$\mathfrak{B}$ は比 > 0 の相等性の下で不変フィルタ基底であるため、主張 (i) は II、p. 23、prop から直接続きます。 1. $\mathfrak{B}$ の定義により、位相 $\mathscr{T}$ は、$g_\alpha$ を連続にする E 上の局所凸トポロジーの最も細かいものです。 よって (iii).最後に、$f$ が連続であれば、$f \circ g_\alpha$ も連続であることは明らかです。逆に、$f \circ g_\alpha$ がすべての $\alpha$ で連続している場合、G の 0 の各対称凸近傍 W に対して、集合 $g_\alpha^{-1}(f^{-1}(W))$ は、各 $\alpha$ の $F_\alpha$ の 0 の近傍になります。ここで、$f^{-1}(W)$ は吸収性、対称、凸面であるため、$f^{-1}(W)$ は $\mathscr{T}$ で 0 の近傍となり、$f$ は連続です。同様に、$p$ が E 上の準ノルムで、$p \circ g_\alpha$ がすべての $\alpha$ に対して連続であり、U が $p(x) < 1$ のように点 $x \in E$ の集合である場合、$\alpha$ ごとに集合 $g_\alpha^{-1}(U)$ は、$E_\alpha$ の 0 の凸型近傍で、対称的で吸収性があります。したがって、U は E の 0 の近傍であり、$p$ は連続です (II、p. 2、提案 1)。

最後の主張は、S、IV, § 2.5、基準 CST 18 から続きます。

$\mathscr{T}$ は、線形写像 $g_\alpha$ の族に対して、$F_\alpha$ のトポロジー族 $\mathscr{T}_\alpha$ の *局所的に凸な最終位相* であると言います。

$\mathscr{T}$ が、そのベクトル空間構造と互換性があり、$f_\alpha$ を連続にする E 上のトポロジの中で最も優れたものではない可能性があります (II、p. 75、演習 15。II、p. 75、演習 14 も参照)。

最も重要なケース $E = \sum_{\alpha \in A} g_\alpha(F_\alpha)$ では、次のように $\mathscr{T}$ に対して 0 の近傍の基本的な系が得られます。それぞれの $\alpha \in A$ について、$V_\alpha$ を、$\alpha \in A$ に対する $g_\alpha(V_\alpha)$ の 0 の対称近傍、$\mathscr{T}_\alpha$、形和集合とし、この和集合の E の凸包絡線を次のように表します。 $\Gamma((g_\alpha(V_\alpha)))$; E のすべての元は形 $\sum_{\alpha \in J} x_\alpha$ であり、J は I と $x_\alpha \in g_\alpha(F_\alpha)$ の有限部分集合であるため、$\Gamma((g_\alpha(V_\alpha)))$ が E の *吸収性* 対称凸面集合であるのは明らかです (各$V_\alpha$ は $F_\alpha$ に吸収性があります)。 $\Gamma((g_\alpha(V_\alpha)))$ 含むがすべて $g_\alpha(V_\alpha)$ である場合、$\mathscr{T}$ では 0 の近傍になります。一方、$\mathscr{T}$ の 0 のすべての対称凸型近傍 V に対して、$V \supset \Gamma((V \cap g_\alpha(F_\alpha)))$ があり、そこから主張が続くことは明らかです。

#### 系 1 {#evt-ii-s4-prop-5-cor-1 .statement tag=07EF}

*With 記法 of prop. 5、H を局所凸空間 G の E の線形写像の集合とします。E がその部分空間 $g_\alpha(F_\alpha)$ の和であると仮定します。 H は、$f$ が H で変化するすべての $\alpha$、集合 $f \circ g_\alpha$ について、$F_\alpha$ で等連続である場合にのみ、$\mathscr{T}$ で等連続です。*

I、p. 9、プロップを思い出してください。 6 議論は (ii) prop の議論と同様です。 5. W を G の 0 の対称凸近傍とします。$f \in H$ が等連続である集合 $f \circ g_\alpha$ の場合、共通部分 $\bigcap_{f \in H} g_\alpha^{-1}(f^{-1}(W))$ は $F_\alpha$ の 0 の対称凸近傍であることに注意してください。この共通部分は$g_\alpha^{-1}(\bigcap_{f \in H} f^{-1}(W))$と同じであり、集合$\bigcap_{f \in H} f^{-1}(W)$は対称で凸であるため、すべてはそれが*吸収*であることを示すことにかかっています。さて、仮定までに、すべての $x \in E$ は $z_{\alpha_i} \in F_{\alpha_i}$ として $\sum_{i=1}^n g_{\alpha_i}(z_{\alpha_i})$ として書くことができます。すべての $f \in H$ に対して $f(\lambda x) \in W$ となるような $\lambda > 0$ が存在することを示すには、$z_\alpha \in F_\alpha$ を伴う $x = g_\alpha(z_\alpha)$ の場合を考慮するだけで十分です ($W/n$ による置き換えること W による一般的な場合に進むことができるため)。しかし、この場合は、$g_\alpha^{-1}(\bigcap_{f \in H} f^{-1}(W))$ が $F_\alpha$ の 0 の近傍であるという事実から導かれます。

#### 系 2 {#evt-ii-s4-prop-5-cor-2 .statement tag=07EG}

*$(J_\lambda)_{\lambda \in L}$ を添字集合の分割とします。 A. $(G_\alpha)_{\alpha \in A}$ を局所凸空間の族、$(F_\lambda)_{\lambda \in L}$ をベクトル空間の族とします。それぞれの $\lambda \in L$ について、$h_\lambda$ をベクトル空間 E の $F_\lambda$ の線形写像とします。 $\lambda \in L$ と $\alpha \in J_\lambda$ それぞれについて、$g_{\lambda \alpha}$ を $F_\lambda$ の $G_\alpha$ の線形写像とします。 $f_\alpha = h_\lambda \circ g_{\lambda \alpha}$と書きます。それぞれの $F_\lambda$ が、$g_{\lambda \alpha}$ ($\alpha \in J_\lambda$) を連続にする、局所的に最も細かい凸面位相を持っていると仮定します。次に、$f_\alpha$ を連続にする E 上の最も細かい局所凸型位相は、$h_\lambda$ を連続させる最も細かい局所凸型位相と同一です。

これは S、IV, § 2.5 基準 CST 19 の特殊なケースであり、prop を使用して直接証明することもできます。 5.

局所凸最終トポロジーの例。

I。 商空間。

M を局所凸空間 F の部分空間とし、φ を F/M 上の F の標準写像とします。 F/M 上の商位相は局所的に凸であり、φ を連続にするすべてのトポロジー (局所的に凸であるかどうかにかかわらず) の中で最も細かいものであるため、単一の写像 φ の族からなるの局所的に凸な最後の位相でもあります。

II。局所凸型空間の帰納型極限。

A を右方向の順序付けられた集合とし、$(E_\alpha, f_{\beta\alpha})$ を集合 A に対するベクトル空間の帰納的系とします (A, II, § 6.2)。 $E = \varinjlim E_\alpha$ と $f_\alpha : E_\alpha \to E$ をそれぞれの $\alpha \in A$ の正規の線形写像とします。各 $E_\alpha$ が局所的に凸な位相 $\mathscr{T}_\alpha$ を保持すると仮定し、さらに $\alpha \leq \beta$ について、写像 $f_{\beta\alpha} : E_\alpha \to E_\beta$ が *連続* であると仮定します。次に、線形写像 $f_\alpha$ (それぞれ位相 $\mathscr{T}$ を運ぶ空間 E) に対する族 $(\mathscr{T}_\alpha)$ の局所的に凸な最終位相 $\mathscr{T}$ が族の *帰納的極限* であると言います。 $(\mathscr{T}_\alpha)$ (それぞれ、系 $(E_\alpha, f_{\beta\alpha})$ の *帰納的極限* 空間、または単に局所的に凸な空間 $E_\alpha$)。 E はベクトル部分空間 $f_\alpha(E_\alpha)$ の和集合であり、$\alpha \leq \beta$ のときは $f_\alpha(E_\alpha) \subset f_\beta(E_\beta)$ であることを思い出してください。 $f_\alpha(E_\alpha)$ に写像 $f_\alpha$ の最後の位相を与えると (これは $f_\alpha(E_\alpha)$ を商空間 $E_\alpha/f_\alpha^{-1}(0)$ と識別するのと同じです)、位相 $\mathscr{T}$ も最後のものになります標準単射と比較した、$f_\alpha(E_\alpha)$ のトポロジーのファミリーの位相 (II、上記の cor. 2)。さらに、$\alpha \leq \beta$ に対する $f_{\beta\alpha}$ の連続性は、標準単射 $j_{\beta\alpha} : f_\alpha(E_\alpha) \to f_\beta(E_\beta)$ が連続であることを意味するため、E は、単射 $j_{\beta\alpha}$ に対する先行トポロジーを運ぶ $f_\alpha(E_\alpha)$ の帰納的極限でもあります。

#### 例 {#evt-ii-s4-n4-exa-1 .statement tag=07EH}

— X を、ローカルでコンパクトな空間と、コンパクト サポートを使用して X 上で定義された有限連続実数値写像の $E = \mathscr{K}(X; \mathbf{R})$ ベクトル空間とします。 X の各コンパクト部分集合 K について、$x \notin K \Rightarrow f(x) = 0$ となる写像 $f \in E$ によって形成される E のベクトル部分空間を $E_K$ とします。 $E_K$ で誘導された $\mathscr{T}_K$ 位相と、X での *一様収束* の $\mathscr{T}_u$ 位相で表します。トポロジー $\mathscr{T}_K$ の帰納的極限 $\mathscr{T}$ は、$\mathscr{T}_u$ よりもより細かいです。 X がパラコンパクトでありコンパクトではない場合、$\mathscr{T}$ は厳密には $\mathscr{T}_u$ よりもより細かいであることがわかります (*cf.* INT, III, 2nd ed., § 1.8)。 $\mathscr{T}$ の重要性は、$\mathscr{T}$ で連続する E の線型形式が正確に X (INT, III, 2nd., § 1.3) の実際の *メジャー* であるという事実にあります。

#### 注意 {#evt-ii-s4-n4-rem-1 .statement tag=07EI}

— 最後の例では、$E_K$の$\mathscr{T}$によって引き起こされる位相は、定義までに$\mathscr{T}_K$より粗くなり、$\mathscr{T}$がより細かいであるため、$\mathscr{T}_K$と同一になります。 $E_K$に$\mathscr{T}$によって誘発される$\mathscr{T}_u$、位相は、$\mathscr{T}_u$、つまり$\mathscr{T}_K$によって誘発されるものよりより細かいです。

この推論は、E 上に局所凸型位相 $\mathscr{T}'$ があり、$\mathscr{T}_\alpha$ が $E_\alpha$ 上で誘導される位相である場合、局所凸トポロジー $(\mathscr{T}_\alpha)$ の帰納極限に直ちに一般化されます。 $\mathscr{T}'$。

より一般的には、$E_\beta \subset E_\alpha$ と $\mathscr{T}_\beta$ が $\mathscr{T}_\alpha$ によって位相誘導されたと仮定した場合、それぞれの $E_\alpha$ でどのような状況で $\mathscr{T}$ 誘導する $\mathscr{T}_\alpha$ が発生するのかを尋ねることができます。一般に、これはそうではありません (II、p. 80、演習 26)。しかし、これが実際に発生する 2 つの重要な状況については、次の番号で説明します。

### 5. 局所凸型空間の族の直接位相幾何学和

#### 定義 2 {#evt-ii-s4-def-2 .statement tag=07EJ}

*E をベクトル空間とします。これは、局所凸型空間* $(E_i)_{i \in I}$ の族の直和* (A, II, § 1.6) です。 *それぞれ* $i \in I$、*$f_i$ を *$E$ の $E_i$ の標準単射* にします。 *族のトポロジー 直和* $(E_i)$ *私たちは空間* $E$ *局所的に最も細かい凸型位相を持ち、それぞれ* $f_i$ *連続になります (この位相は、* のトポロジーの直和と呼ばれます) $E_i$）。

この番号の残りの部分では、def と同じ記法を保持します。 2 (〜でない限りその逆は明示的に述べられています)、そして私たちは同一視する、標準的には、$f_i$によって、$E$の部分空間を持つそれぞれの$E_i$です。

II、p. 28 で与えられる局所凸最終位相の一般的な近傍の記述により、ここで直和位相の $E$ の 0 の近傍の基本系を得ることができます。次の方法で; *すべての* ファミリ $(V_i)_{i \in I}$ について、$V_i$ は $E_i$ の 0 の対称凸近傍であり、$V_i$ の和集合の凸包絡線 $\Gamma((V_i))$ を考慮します。すべてのファミリー $(V_i)$ の $\Gamma((V_i))$ (または、$E_i$ の 0 の近傍の基本系にある各 $i$ の $V_i$ のみを取る) 形 0 の近傍の基本系 $E$。

#### 例 {#evt-ii-s4-n5-exa-1 .statement tag=07EK}

— $(a_i)_{i \in I}$ をベクトル空間 $E$ の基底とし、各行 $Ra_i$ の正規の位相 (I、p. 2、*例 5*) を考慮します。これらのトポロジのうち直和は、$E$ (II、p. 26) に局所的に凸の *最も細かい* 位相です。実際、$V$ が $E$ の吸収性、対称、凸面集合である場合、$V_i = V \cap Ra_i$ は $Ra_i$ および $V$ の 0 の近傍であり、明らかに含むは凸面包絡線 $\Gamma((V_i))$ です。

#### 命題 6 {#evt-ii-s4-prop-6 .statement tag=07EL}

*局所凸位相* $\mathscr{T}$ *上* $E$ * は* $E_i$ のトポロジの直和であり、*その場合に限り、次の性質が成り立ちます: 線形写像の* $E$ *局所凸空間* $G$ *(それぞれ準ノルム* $p$ *on* $E$) *すべて* $i \in I$, *写像* $g \circ f_i$ *(それぞれ $p \circ f_i$) が* $E_i$で連続である。

これはプロップの特殊なケースです。 5、II、p. 27。

Recalling the definition of the direct sum of a family of vector spaces (A, II, p. 12, prop. 6), we can say that the topology $\mathscr{T}$ is the only one for which the canonical mapping $g \mapsto (g \circ f_i)$ is a *bijection*

$$
\mathscr{L}(E; G) \to \prod_{i \in I} \mathscr{L}(E_i; G)
$$

局所的に凸の空間 $G$ ごとに。

#### 系 {#evt-ii-s4-n5-cor-1 .statement tag=07EM}

※支柱記法付き。 5、II、p. 27、* $E$ * が* $g_\alpha(F_\alpha)$ の和であると仮定します。 * $F$ * を族* $(F_\alpha)_{\alpha \in A}$ のトポロジー 直和とし、*そして * $j_\alpha : F_\alpha \to F$ * を標準単射とします。 * $g : F \to E$ *は線形写像が* $g \circ j_\alpha = g_\alpha$ *すべて* $\alpha \in A$ であると仮定します。 *もし* $N$ *が* $g$の核である場合、*標準的な全単射* $F/N \to E$ *に関連付けられています* $g$ *は* $F/N$ *on* $E$ *withのトポロジカル同型です位相* $\mathscr{T}$。

これは、II、p. 28、cor の特殊なケースです。 2 II、p. 29、*例 I* を覚えています。

#### 命題 7 {#evt-ii-s4-prop-7 .statement tag=07EN}

*標準単射* $j : E \to \prod_{i \in I} E_i$ *は* $E$ * が* $E_i$ * の直和位相を運ぶとき* および* $\prod_{i \in I} E_i$ * 積位相を運ぶとき連続です。 * $I$ * が有限のとき、この写像はトポロジー ベクトル空間の同型です。

最初の主張は、各 $\kappa \in I$ に対して標準単射 $E_\kappa \to \prod_{\iota \in I} E_\iota$ が連続しているという事実から導き出されます。 $I$ が有限である場合、$j$ は恒等写像であり、積位相 $\mathscr{T}'$ が直和位相 $\mathscr{T}$ よりもより細かいであることを示すだけで十分です。さて、$V$を$\mathscr{T}$の0の凸近傍とします。それぞれの集合 $V \cap E_\iota$ は、$E_\iota$ の 0 の凸近傍です。 $n$ が $I$ の元の数である場合、集合 $V$ 含む集合 $\frac{1}{n} \sum_n (V \cap E_\iota)$、つまり $\mathscr{T}'$ の 0 の近傍です、そして命題が証明されました。

When $I$ is infinite, if, for each finite subset $J$ of $I$, we write $E_J$ for the space $\prod_{\iota \in J} E_\iota$, with the product topology, then $E$ is the *inductive limit* of the $E_J$ (identified as subspaces of $E$).

#### 命題 8 {#evt-ii-s4-prop-8 .statement tag=07EO}

*$\iota \in I$ごとに、$N_\iota$を$E_\iota$の部分空間とします*

(i) *$E$上の直和位相$\mathscr{T}$によって$N = \sum_\iota N_\iota$に誘導された位相は、$N_\iota$のトポロジーの直和と同一です。

(ii) *The canonical mapping $h$ of the topological direct sum space of the $E_\iota / N_\iota$ on $E/N$ (A, II, § 1.6, formula (26)) is an isomorphism between topological vector spaces.*

(i) 上で紹介した記法を使用して、$x = \sum_\iota \lambda_\iota x_\iota$ 所属から $N \cap \Gamma((V_\iota))$ を考慮します ($(\lambda_\iota)$ は数 $\geqslant 0$ の族であり、そのうちの多くは $\sum_\iota \lambda_\iota = 1$ と $x_\iota \in V_\iota$ のように非ゼロです。 $\iota \in I$）。 $N_\iota$ の和は直接なので、すべての $\iota \in I$ に対して $\lambda_\iota x_\iota \in N_\iota$ が得られます。したがって、$\lambda_\iota > 0$ となるすべての $\iota$ に対して、凸包絡線 $\Gamma((N_\iota \cap V_\iota))$ に対して $x_\iota \in N_\iota \cap V_\iota$、$x$ 属するも成り立つため、(i) が証明されます。

(ii) 標準写像を次のように表します: $f_\iota : E_\iota \to E, h_\iota : E_\iota / N_\iota \to E/N, p_\iota : E_\iota \to E_\iota / N_\iota$ および $p : E \to E/N$。 $\iota \in I$、$h_\iota \circ p_\iota = p \circ f_\iota$、命題ごとに、II、p. 28、cor から続きます。 2 と p. 29 *例 I*。

#### 系 1 {#evt-ii-s4-prop-8-cor-1 .statement tag=07EP}

*$N_\iota$ が $\iota \in I$ ごとに $E_\iota$ にクローズされる場合、$N = \sum_\iota N_\iota$ は $E$ にクローズされます。*

なぜなら、標準写像 $p_\iota : E \to E_\iota$ はすべての $\iota \in I$ に対して連続 (II, § 4.5、提案 6) であるため、$p_\iota^{-1}(N_\iota)$ は $E$ で閉じられ、したがって共通部分 $N = \bigcap_{\iota \in I} p_\iota^{-1}(N_\iota)$ にも同じことが当てはまります。

#### 系 2 {#evt-ii-s4-prop-8-cor-2 .statement tag=07EQ}

*それぞれの $E_\iota$ がハウスドルフである場合、$E$ も同様であり、それぞれの $E_\iota$ は $E$ で閉じられます。*

最初の主張を証明するには、cor を適用します。 1 はすべて $\iota \in I$ に対して $N_\iota = \{0\}$ を取得します。 2 番目の場合は cor を適用します。 $\kappa \neq \iota$ごとに$N_\iota = E_\iota$と$N_\kappa = \{0\}$が1つ。

III、p. 21、cor に示します。 2 $E_\iota$ がハウスドルフで *完全* である場合、それらのトポロジー 直和 $E$ も同様です。

### 6. 帰納的極限の数列の局所凸空間

この番号では、ベクトル空間 $E$ のベクトル部分空間の *増加する数列* $(E_n)$ を考慮します。つまり、$E$ は $E_n$ の *和集合* です。それぞれの $E_n$ が局所的に凸な位相 $\mathscr{T}_n$ を保持していると仮定します。そのため、すべての $n$ について、$\mathscr{T}_{n+1}$ によって $E_n$ に誘導された位相は $\mathscr{T}_n$ より *粗く、$E$ に局所的な凸を与えます。凸型位相 $\mathscr{T}$、これは数列 $(\mathscr{T}_n)$ (II, p. 29, *例 II*) の *帰納的極限* です。これらの仮説と記法は、再表明することなく、この番号の残りの部分全体で使用されます。

それぞれの $\mathscr{T}_n$ はハウスドルフであるが、$\mathscr{T}$ はハウスドルフではないということが起こります。また、整数 $n, m$ の各対について、$n \leq m$、部分空間 $E_n$ は $E_m$ (位相 $\mathscr{T}_m$ を使用) で閉じられますが、$E_n$ は $E$ を使用して閉じられないということも起こります。 $\mathscr{T}$ (II、p. 80、演習 26)。

#### 補題 1 {#evt-ii-s4-lem-1 .statement tag=07ER}

— *$\mathfrak{F}$ を $E$ に対するコーシー フィルター ($\mathscr{T}$ の場合) とします。次に、整数 $k$ が存在し、$E$ の$0$ のすべての $N \in \mathfrak{F}$ とすべての近傍 $V$ について、部分空間 $E_k$ が $N + V$ と一致します。

逆のことを仮定すると矛盾が生じます。 $k$ ごとに、次のような $0$ と集合 $M_k \in \mathfrak{F}$ の凸型近傍 $V_k$ が存在すると仮定します。
$$
(E_k + V_k) \cap M_k = \varnothing.
$$
明らかに、すべての $k$ に対して $V_{k+1} \subset V_k$ と仮定できます。 $V$を$\bigcup_k (E_k \cap V_k)$の凸包絡線とすると、これは明らかに$\mathscr{T}$に対する$0$の近傍です。すべての $n$ に対して、$V \subset V_n + E_n$ があります。実際、すべての $x \in V$ は $\sum_i \lambda_i x_i$ と書くことができ、すべての $i$ に対して $\lambda_i \geq 0$、$\sum_i \lambda_i = 1$、$x_i \in V_i \cap E_i$ が表されます。さて、$i < n$ には $x_i \in E_n$ があるため、$\sum_{i < n} \lambda_i x_i \in E_n$ になります。そして、$i \geq n$ については、$x_i \in V_n$ があり、$V_n$ が凸であるため、$\sum_{i \geq n} \lambda_i x_i \in V_n$、含む $0$ と $\sum_{i \geq n} \lambda_i \leq 1$ です。したがって、すべての $n$ に対して $V + E_n \subset V_n + E_n$ となります。そうすると、$M \in \mathfrak{F}$を集合、つまり$V$-小さいとします。一部の整数 $m$ では、$E_m \cap M$ は空ではありません。そして私たちは結論する
$$
M \subset E_m + V \subset E_m + V_m;
$$
$\mathfrak{F}$ はフィルターであるため、集合 $M_m$ は $M$ と一致するため、$E_m + V_m$ になります。 補題を成立させる矛盾があります。

#### 命題 9 {#evt-ii-s4-prop-9 .statement tag=07ES}

*$\mathscr{T}_{n+1}$によって$E_n$に誘発された位相が、すべての整数$n$において$\mathscr{T}_n$と同一であると仮定します。それから
(i) $E_n$ の $\mathscr{T}$ によって誘発された位相は、各 $n$ の $\mathscr{T}_n$ と同一です。 $\mathscr{T}_n$ がハウスドルフであれば、$\mathscr{T}$ はハウスドルフです。
(ii) $n$ごとに、$E_n$が$E_{n+1}$でクローズされる場合（$\mathscr{T}_{n+1}$の場合）、$E_n$は$n$ごとに$E$でクローズされます（$\mathscr{T}$を使用）。
(iii) 各 $E_n$ が ($\mathscr{T}_n$ を使用して) 完了した場合、$E$ は $\mathscr{T}$ を使用して完了します。*

(i) 最初の主張を証明するには、$E_n$の$\mathscr{T}$によって引き起こされる位相$\mathscr{T}'_n$が$\mathscr{T}_n$よりもより細かいであることを証明すれば十分です。このために、$V_n$ を $E_n$ の位相 $\mathscr{T}_n$ に対する $0$ の凸近傍とします。 $\mathscr{T}_{n+p}$ に対して $E_{n+p}$ の $0$ の凸近傍の構成する増加する数列を、添字ごとに $V_{n+p} \cap E_n = V_n$ になるように、$(V_{n+p})_{p \geq 1}$ とします。 $p \geq 1$。次に、増加する数列 $(V_{n+p})$ の和集合 $V$ は、$V \cap E_k$ が $E_k$ の $0$ の近傍となるような凸型集合になります ($\mathscr{T}_k$ を使用)。 添字 $k$ごと。したがって、$V$は、$\mathscr{T}$の$E$の$0$の近傍となり、$V \cap E_n = V_n$と同様に、$\mathscr{T}'_n$が$\mathscr{T}_n$よりもより細かいであることが証明されました。

定義する $V_{n+p}$ までは、次の補題を使用して $p$ で帰納法まで進みます。

#### 補題 2 {#evt-ii-s4-lem-2 .statement tag=07ET}

*$V$ を $M$ の 0 の凸近傍 、局所凸空間 $F$ のベクトル部分空間とします。すると、$W \cap M = V$ となるような 0 の凸近傍 $W$ が $F$ に存在します。さらに、$M$が$F$で閉じられている場合、点$x_0 \in \complement M$ごとに、$F$に0の凸近傍$W_0$が存在し、$W_0 \cap M = V$と$x_0 \notin W_0$のようになります*。

実際、仮定までに、$F$ に 0 の凸近傍 $U$ が存在し、$U \cap M \subset V$ になります。明らかに、$F$ の $U \cup V$ の凸包絡線 $W$ は、$F$ の 0 の近傍です。 $W \cap M = V$ であることを示します。なぜなら、すべての点 $z \in W$ は、$x \in V, y \in U$ および $0 \leq \lambda \leq 1$ を伴う形 $\lambda x + (1-\lambda) y$ です (II、p. 9、提案 8)。 $z \in M$ と $\lambda \neq 1$ の場合、必然的に $y \in M$、したがって $y \in U \cap M \subset V$、したがって $z \in V$ になります。 $\lambda = 1$ の場合、結果は明らかに true です。 $M$ が $F$ で閉じている場合、空間 $F/M$ はハウスドルフであるため、$F$ に 0 の凸近傍 $U_0 \subset U$ が存在し、$U_0$ は $x_0 + M$ と一致しません。この場合、$U_0 \cup V$ の凸包絡線 $W_0$ は必要な条件を満たします。

定理に戻り、(i) の 2 番目の部分を証明するために、$x \in E$ の場合、一部の $n$ については $x \in E_n$ となることに注意してください。 $x \neq 0$ と $\mathscr{T}_n$ がハウスドルフである場合、$\mathscr{T}_n$ には 0 の近傍 $V_n$ が存在しますが、含む $x$ は存在しません。 $\mathscr{T}$ に対して 0 の近傍 $V$ があり、$V \cap E_n = V_n$ となるため、$x \notin V$ となり、$\mathscr{T}$ はハウスドルフであることがわかります。

(ii) $x \in E - E_n$ とします。 $x \in E_m$ となるような $m > n$ が存在するので、$E_n$ が $\mathscr{T}_m$ に対して $E_m$ で閉じられるため (仮定が $n$ ごとに $E_n$ に$\mathscr{T}_{n+1}$ 誘導する $\mathscr{T}_n$ となるため) が存在します。 位相 $\mathscr{T}_m$ $E_m$ の 0 の凸近傍 $V_m$ で、$(x + V_m) \cap E_n$ は空です。さて、(i) で、$\mathscr{T}$ に対して 0 の凸近傍 $V$ が存在し、$V \cap E_m = V_m$ となることが分かりました。したがって $(x + V) \cap E_m = x + V_m$、したがって $(x + V) \cap E_n = \varnothing$ となり、(ii) が証明されます。

(iii) 補題 1 から、$\mathfrak{F}$ が $\mathscr{T}$ (GT、II, § 3.2) の *最小* コーシー フィルターである場合、$E_k$ 上の $\mathfrak{F}$ のトレースがフィルター $\mathfrak{F}_k$ となるような $k$ が存在します。 (i) この最後のは $\mathscr{T}_k$ のコーシー フィルターであるため、$\mathfrak{F}_k$ は仮定によって $E_k$ に収束します。しかし、$\mathfrak{F}_k$によって生成された$E$のフィルターは$\mathfrak{F}$よりもより細かいであるため、$\mathfrak{F}$には$\mathscr{T}$に対してクラスター点があり、したがって$\mathscr{T}$に収束することがわかります。

$\mathscr{T}_{n+1}$によって$E_n$に誘導された$n$位相が単に$\mathscr{T}_n$であるとき、$\mathscr{T}$は数列$(\mathscr{T}_n)$の*厳密な帰納極限*であり、空間であると言います。 $E$ と位相 $\mathscr{T}$ は、局所凸空間 $E_n$ の数列の *厳密帰納法極限* です。

#### 注意 {#evt-ii-s4-n6-rem-1 .statement tag=07EU}

— 1) $E$ が増加するの和集合であり、部分空間 $(E_\alpha)_{\alpha \in I}$ の *非数えられない* 族であり、それぞれの $E_\alpha$ が局所的に凸な位相 $\mathscr{T}_\alpha$ を持ち、$E_\alpha \subset E_\beta$ について、 $\mathscr{T}_\beta$によって$E_\alpha$に誘発された位相は$\mathscr{T}_\alpha$と同一です。 位相 $\mathscr{T}$ によってそれぞれの $E_\alpha$ に誘導された位相が $\mathscr{T}_\alpha$ に等しく、$E_\alpha$ が *ハウスドルフで完全であるが、$E$ が $\mathscr{T}$* に対して完全ではない場合があるかもしれません (INT, III、第 2 版、§ 1、演習 2)。

2) Let $F$ be a locally convex space, which is the union of an increasing sequence of vector subspaces $(F_n)$, and for each index $n$, let $\mathscr{T}_n$ be the topology induced on $F_n$ by the topology $\mathscr{T}$ of $F$. 一般に、$\mathscr{T}$ は $\mathscr{T}_n$ の帰納的な極限ではないことに注意する必要があります。

3) $E$ が数列 $(E_n)$ の厳密な帰納法極限であると仮定します。 $F$ が閉じた ($\mathscr{T}$ の) $E$ ベクトル部分空間である場合、$F \cap E_n$ 上の $\mathscr{T}_n$ によって誘導されるトポロジーの厳密な帰納法極限は、*厳密により細かい* である可能性があります。 位相は $\mathscr{T}$ によって誘発されます (IV、p. 63、演習 10)。

#### 命題 10 {#evt-ii-s4-prop-10 .statement tag=07EV}

※E,Fを局所2凸空間とする。次のように仮定します:*

1) *Fréchet 空間* $(E_\alpha)$ の族が存在し、 *それぞれの $\alpha$ 線形写像* $g_\alpha : E_\alpha \to E$ に対して、 *E の位相がその族 * $(g_\alpha)$ の最後の局所凸位相となるようにします。

2) *フレシェの数列空間* $(F_n)$ *そしてそれぞれの n に対して連続線形単射* $j_n : F_n \to F$ *そのような* $F = \bigcup_n j_n(F_n)$ が存在します。

*すると、グラフが * $E \times F$ で閉じられている F 内の E の各線形写像 u は、 * 必然的に連続になります。*

$u$ が連続であることを証明するには、すべての $\alpha$、写像 $u \circ g_\alpha : E_\alpha \to F$ が連続であることを示すだけで十分です (II、p. 27、提案 5)。さて、$u \circ g_\alpha$のグラフは、連続写像$g_\alpha \times 1_F : E_\alpha \times F \to E \times F$の下で$u$のグラフの逆像であるため、仮定までに$E_\alpha \times F$で閉じられます。したがって、E 自体が *Fréchet 空間* である場合に限定できます。しかし、命題は I、p. 20、プロップの特殊なケースです。 1.

#### 系 {#evt-ii-s4-n6-cor-1 .statement tag=07EW}

*E と F については prop と同じ仮説を使用します。 10 そして E がハウスドルフであると仮定すると、E における F のすべての連続全射法写像 v は厳密な射です。*

N を $v$ の核として、$N_n = j_n^{-1}(N)$ と書きます。 写像 $j'_n : F_n / N_n \to F / N$ は、商を取って$j_n$ から推定され、単射的連続であり、また、$F_n / N_n$ はフレシェ空間 ($N_n$ が閉じているため) であり、$F / N$ は の和集合です。 $j'_n$の下の像。 仮定までに、正準因数分解 $v : F \to F / N \xrightarrow{w} E$ では、線形写像 $w$ は全単射かつ連続であり、したがって $(F / N) \times E$ のグラフは *閉じています* (GT、I, § 8.1、提案 2 の cor. 2)。冒頭では注意、プロップでは。したがって、$w$ の逆数写像 $u$ は連続であり、系が証明されます。

\* 提案 10 とその系は、E が *完全な生まれつき空間* (III, p. 12) であり、F が Fréchet 空間の数列の帰納的極限である場合に特に適用されます。 \*

### 7. フレシェの注意空間

プロップを検討していきます。 GTの2、局所凸空間の場合IX, § 3.1。

#### 命題 11 {#evt-ii-s4-prop-11 .statement tag=07EX}

*E を可測定局所凸空間とする。 E の位相は、平行移動下で不変で、開いたボールが凸になる距離によって定義できます。*

$(p_n)_{n \in \mathbf{N}}$ を、E の定義する位相である準ノルムの数列とします。 $d_n$ を、E の $x, y$ に対して $d_n(x, y) = \inf(p_n(x - y), 1/n)$ によって定義された擬似計量とします。それは翻訳下では不変です。すべての $n \geq 0$ とすべての実数 $R \geq 0$ について、$B_{n, R}$ を $d_n(x, 0) < R$ の $x \in E$ の集合とします。 $R \geq 1/n$ の場合、$B_{n, R} = E$、その他の場合、$B_{n, R}$ は $x \in E$ から$p_n(x) < R$ のように形成されます。すべての場合において、$B_{n, R}$ は凸です。

$E$ 定義する $d(x, y) = \sup_{n \in \mathbf{N}} d_n(x, y)$ の $x, y$ の場合。 $d$ は距離であり、$E$ の変換下で不変であり、$E$ の位相を定義していることがすぐにわかります。 $x_0 \in E$ と $R \geq 0$ の場合、中心 $x_0$ と半径 $R$ (距離 $d$ の場合) のオープンボールは $\bigcap_{n \in \mathbf{N}} (x_0 + B_{n, R})$ に等しいため、凸です。

#### 命題 12 {#evt-ii-s4-prop-12 .statement tag=07EY}

*$E$と$F$を2つのフレシェ空間と$u$を$F$の$E$の連続する線形写像とします。次に、必ずしも線形ではない連続けれどもの $u$ の切断が存在します。

プロップにより。 11 $E$ には、平行移動下で不変の距離 $d$ が存在し、$E$ の位相を定義し、開いたボールが凸になります。 $F$ の $y$ と $y'$ を考えると、$E$ の閉じた集合 $u^{-1}(y)$ と $u^{-1}(y')$ の距離を $\delta(y, y')$ とします。 $u$ は GT の厳密な射 (I、p. 17、th.1) 注意であるため、IX, § 3.1 は、$\delta$ が $F$ の位相を定義する $F$ 上の距離であることを示します。 We shall construct, inductively, a sequence of continuous mappings $(s_n)_{n \in \mathbf{N}}$ of $F$ in $E$ satisfying the following inequalities for all $y \in F$:

$$
\delta(y, u(s_n(y))) < 2^{-n}
$$
$$
d(s_n(y), s_{n-1}(y)) < 2^{-n+1} \quad \text{(only if } n \geq 1 \text{)}.
$$

次に、$n = 0$ または $n \geq 1$ が構築され、$s_{n-1}$ が構築されたとします。 $y_0 \in F$ にしましょう。 $u$ は全射的であり、集合 $u^{-1}(y_0)$ は空ではなく、$n \geq 1$ については、帰納法の仮定によって $d(u^{-1}(y_0), s_{n-1}(y_0)) < 2^{-n+1}$ が得られます。 Therefore there exists a point $x_0$ of $E$ such that $u(x_0) = y_0$ and for $n \geq 1$, $d(x_0, s_{n-1}(y_0)) < 2^{-n+1}$. As the mapping $s_{n-1}$ is continuous, the set of points $y$ of $F$ which satisfy the inequalities $\delta(y, y_0) < 2^{-n}$ and $d(x_0, s_{n-1}(y)) < 2^{-n+1}$ is an open neighbourhood of $y_0$. したがって、$E$ には、$F$ の開いたカバー$(V_i)_{i \in I}$ と$F$ の定数写像 $s_{n,i}$ が存在します。これは、満たす *in* $V_i$ の不等式 (2) と (3) で、1 置き換える $s_n$ は、 $s_{n,i}$。 空間 $F$ は計量可能であるため、単位元 $(f_i)_{i \in I}$ の連続分割が存在します。これは局所的に有限であり、カバー $(V_i)_{i \in I}$ (GT、IX, § 4.5、th. 4 および § 4.4、cor. 1) に従属します。 $y \in F$ごとに$s_n(y) = \sum_{i \in I} f_i(y) \cdot s_{n,i}(y)$を入れます。 $E$ の $F$ の写像 $s_n$ は連続しています。オープンボールは$E$と$F$で凸であるため、写像$s_n$はすべての$y \in F$について不等式(2)と(3)を満たします。

不等式 (3) 写像 $s_n : F \to E$ 形から、一様収束のためのコーシー 数列 。 $E$ が完了すると、数列 $(s_n)_{n \in \mathbf{N}}$ は連続的な写像 $s : F \to E$ (GT, X, § 1.6) に一様に収束します。 公式 (2) は、$u \circ s$ が $F$ の恒等写像であるため、$s$ は $u$ の連続する切断であることを示しています。

#### 系 {#evt-ii-s4-n7-cor-1 .statement tag=07EZ}

*$L$ が $F$ のコンパクト集合である場合、$E$ には $u(K) = L$ のようなコンパクト集合 $K$ が存在します。

$s$ が $u$ の連続する切断である場合、$K = s(L)$ を置くだけで十分です。

#### 注意 {#evt-ii-s4-n7-rem-1 .statement tag=07F0}

— 1) 系を支柱に置きます。 12 も th から推測できます。 I、p. 17、および小道具の 1 つ。 GTの18、IX, § 2.10。
2) 小道具記法を保管します。 12. $p$ を $E$ 上の連続半ノルムとします。

すべての $y \in F$ に対して $q(y) = \inf_{u(x)=y} p(x)$ を置き、$q$ が $F$ (II、p. 4) の連続半ノルムになるようにします。 $\phi$を、$\overline{\mathbf{R}}$の区間$]0, +\infty[$における$F$の下位半連続写像とします。私たちは、* $p \circ s < q + \phi$ となるような * 連続する切断秒が存在することを示します。

$s_0$ を $u$ の連続切断 (提案 12) および $u$ の $N$ 核とします。 $y_0 \in F$ とすると、$p(s_0(y_0) + z_0) < q(y_0) + \phi(y_0)$ となるような $z_0 \in N$ が存在します。 $F$ には、すべての $y \in W$ に対して $p(s_0(y) + z_0) < q(y) + \phi(y)$ となる、$y_0$ のオープン近傍 $W$ が存在します。 したがって、$F$ のオープンカバー $(W_i)_{i \in I}$ と、すべての $y \in W_i$ に対して $p(s_0(y) + t_i(y)) < q(y) + \phi(y)$ となる定数写像 $t_i : F \to N$ が存在します。 $F$ は計量可能であるため、カバー $(W_i)_{i \in I}$ に従属する単位元の局所有限連続分割、たとえば $(g_i)_{i \in I}$ (GT, IX, § 4.5, th. 4 および § 4.4, cor. 1) が存在します。 $s(y) = s_0(y) + \sum_{i \in I} g_i(y) \cdot t_i(y)$ によって定義される $E$ の $F$ の写像 $s$ は、指定された条件を満たします。

### 練習問題 {#evt-ii-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
