---
book: evt
book_title: Topological Vector Spaces
chapter: IV
chapter_title: DUALITY IN TOPOLOGICAL VECTOR SPACES
section: 1
section_title: Duality
lang: ja
source: evt-i-v
pdf_pages: 0183-0196, 0229-0234
extraction: ocr
subsections:
    - "no": 1
      title: Topologies compatible with a duality
      page: 0
      pdf_page: 183
    - "no": 2
      title: Mackey topology and weakened topology on a locally convex space
      page: 4
      pdf_page: 186
    - "no": 3
      title: Transpose of a continuous linear mapping
      page: 6
      pdf_page: 188
    - "no": 4
      title: Dual of a quotient space and of a subspace
      page: 8
      pdf_page: 190
    - "no": 5
      title: Dual of a direct sum and of a product
      page: 11
      pdf_page: 193
statements: 36
exercises: 25
content_sha256: a45567c3e13680f6eb2a81165f461d68aafc8989402743cdbf37e0617546a0b7
translated_from: content/en/evt/IV/01_s1_duality.md
translation_method: google
source_content_sha256: b7f26d454273886007de38188e9c263540c6eccc68705afe146cbdcbcc0c7806
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 1ca2c3aa9df03798502d45f167b063cc1774af813678b8cc2fe09431b91c3c9d
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 1。二元性

### 1. 二重性と互換性のあるトポロジ

この切断において、E と F は、双線形形式 B (II, p. 40) によって双対関係に置かれた 2 つのベクトル空間を表します。 (II、p. 41) で 2 つの線形写像を定義したことを思い出します。

$$
d_B : F \to E^*, \quad s_B : E \to F^*
$$

関係が特徴

(1)
$$
B(x, y) = \langle x, d_B(y) \rangle = \langle y, s_B(x) \rangle
$$

$x \in E, \ y \in F$の場合。

#### 定義 1 {#evt-iv-s1-def-1 .statement tag=07QI}

*E 上の局所凸位相 $\mathscr{T}$ は、位相 $\mathscr{T}$ を E に代入して得られる局所凸空間の双対上に、$d_B$ が F から全単射である場合、E と F の間の双対性と互換性があると言われます。

このような位相 $\mathscr{T}$ が存在する場合、写像 $d_B$ は単射的です。つまり、E と F の双対性は F (II, p. 41) で分離します。

#### 命題 1 {#evt-iv-s1-prop-1 .statement tag=07QJ}

(i) *E の閉じた凸部分集合は、E と F の間の双対性と互換性のある E 上のすべての局所凸トポロジーで同じです。*
(ii) E の * 有界部分集合は、E と F の間の双対性と互換性のある E 上のすべての局所凸トポロジーで同じです。*

$\mathscr{T}$ を E と F の双対性と互換性のある E 上の位相とします。従って、$\sigma(E, F)$ よりもより細かいになります。 E の凸型部分集合が $\mathscr{T}$ に対して閉じている場合、それは閉じた実数半空間 (II、p. 38、cor. 1) の共通部分であるため、$\sigma(E, F)$ に対して閉じています。これは(i)を証明します。 主張 (ii) は cor で証明されました。 III、p. 27の3つ。

$F_\sigma$ を、弱い位相 $\sigma(F, E)$ を備えたベクトル空間 F を表すとします。次に、線形写像 $s_B$ 写像 E を $F_\sigma$ のデュアル $(F_\sigma)'$ に追加します (II、p. 43、提案 3)。 $\mathfrak{S}$ を、$F_\sigma$ の有界な部分集合の族とします。言葉の乱用により、$(F_\sigma)'$上の$\mathfrak{S}$トポロジーの$s_B$の下にある逆像は$\mathfrak{S}\text{-topology on } E$と呼ばれます。それは準規範のファミリーによって定義されます

$$
p_A(x) = \sup_{y \in A} |B(x, y)|,
$$

A が $\mathfrak{S}$ を通過するところ。特に、$\mathfrak{S}$ が F の有限部分集合の族である場合、$\mathfrak{S}$-トポロジーはまさに弱い位相 $\sigma(E, F)$ になります。

#### 定義 2 {#evt-iv-s1-def-2 .statement tag=07QK}

*E と F を双対性の 2 つの空間とします。 $\tau(E, F)$ で示される E 上のマッキー 位相は、E 上の $\mathfrak{S}$ トポロジーとして定義されます。ここで、$\mathfrak{S}$ は、F のすべての部分集合のファミリーであり、$E^*$ ($d_B$ の下) の像は、$\sigma(E^*, E)$ に対して凸でバランスが取れており、コンパクトです*。

E と F の双対性が F で分離しているとき、$d_B$ は単射であり、F の位相 $\sigma(F, E)$ は $E^*$ の位相 $\sigma(E^*, E)$ の $d_B$ の下で逆像になります。この場合、$\mathfrak{S}$ は、$\sigma(F, E)$ に対して凸でバランスが取れており、コンパクトである F のすべての部分集合で構成されます。

一般に、$F_1 = d_B(F) \subset E^*$ で、正規の双線形形式 $(x, x^*) \mapsto \langle x, x^* \rangle$ から $E \times F_1$ の $(x, y_1) \mapsto B_1(x, y_1)$ 制限で表すと、E と $F_1$ は $B_1$ によって双対関係に置かれ、この双対性は $F_1$ で分離します。 定義は $B(x, y) = B_1(x, d_B(y))$ です、間違いなく。 2は$\tau(E, F) = \tau(E, F_1)$を示しています。

#### 注意 1 {#evt-iv-s1-n1-rem-1 .statement tag=07QL}

— A をハウスドルフ局所凸空間 G のコンパクト凸部分集合とし、$\tilde{A}$ を A の閉じた凸バランス包絡線とします。 体 K が $\mathbf{R}$ のとき、集合 $\tilde{A}$ は $A \cup (-A)$ の閉じた凸包絡線です。 K が $\mathbf{C}$ のとき、集合 $\tilde{A}$ は$2A \cup (-2A) \cup (2iA) \cup (-2iA)$ の閉じた凸包絡線に含まれます。その結果、(II、p. 14、提案 15)、$\tilde{A}$ はコンパクトになります。

特に、E と F の双対性が F で分離しているとき、*Mackey 位相 $\tau(E, F)$ も $\mathfrak{S}'$-トポロジーであり、$\mathfrak{S}'$ は $\sigma(F, E)$* に対してコンパクトである F のすべての凸部分集合の集合であると推論します。同様の方法で、F 上のマッキー 位相 $\tau(F, E)$ を定義するとします。

#### 定理 1 (マッキー) {#evt-iv-s1-thm-1 .statement tag=07QM}

— *E と F を双対性の 2 空間とします。双対性が F で分離していると仮定します。E 上の局所的に凸な位相 $\mathscr{T}$ が E と F の間の双対性と互換性があるという位数において、$\mathscr{T}$ が位相 $\sigma(E, F)$ よりもより細かいであり、マッキー 位相よりも粗いことが必要かつ十分です。 $\tau(E, F)$.*

$d_B$ の下の $E^*$ に像がある同一視する F。 $\mathfrak{S}_0$ は、$\sigma(F, E)$ に対して凸でバランスが取れていてコンパクトな F のすべての部分集合のうちの集合を表すものとします。 定義までに、$\tau(E, F)$ は E 上の $\mathfrak{S}_0$ トポロジになるため、$\sigma(E, F)$ よりもより細かいになります。

#### 補題 1 {#evt-iv-s1-lem-1 .statement tag=07QN}

*部分空間 F of E* は、$\tau(E, F)$ にわたって連続する E 上のすべての線型形式で構成されます。

F のすべての元は、$\sigma(E, F)$ に対して連続した写像であるため、$\tau(E, F)$ に対してもなります。

逆に、$f \in E^*$が$\tau(E, F)$に対して連続であるとします。 E には 0 の近傍 U が存在し ($\tau(E, F)$ の場合)、U では $|f| \leq 1$ になります。 $U = A^\circ$ となるような集合 $A \in \mathscr{S}_0$ が存在すると仮定できます。他の語, $f$ 属するは、$E^*$ と E の間の双極性のために A の双極$A^{\circ\circ}$ につながります。しかし、F の位相 $\sigma(F, E)$ は$\sigma(E^*, E)$ によって誘発されます。従って、A は $\sigma(E^*, E)$ に対して凸でバランスが取れておりコンパクトであり、双極性の定理 (II、p. 44、th. 1) は等式 $A = A^{\circ\circ}$ を意味します。従って、$f \in F$ があり、そこから補題が続きます。

#### 補題 2 {#evt-iv-s1-lem-2 .statement tag=07QO}

*$\mathscr{T}$ を E 上の局所凸位相とし、E 上のすべての線型形式が $\mathscr{T}$ 属するから F まで連続するようにします。 その場合、$\mathscr{T}$ は $\tau(E, F)$ よりも粗くなります。*

*$\mathscr{U}$を凸の集合、$\mathscr{T}$に対して0のバランスのとれた近傍とします。 $\mathscr{S}$を$\mathscr{U}$の元のFにある極の集合とします。コルによって。 III、p. 17 の 2 つ、$\mathscr{S} \subset \mathscr{S}_0$ があり、cor によって。プロップの1。 III、p. 19、$\mathscr{T}$ の 7 は、$\mathscr{S}'$ トポロジーと同一です。ここで、$\mathscr{S}'$ は、E の双対 $E'$ における $\mathscr{U}$ の集合の極の集合です。しかし、$E' \subset F$ は、 仮定なので、$\mathscr{S}'$ のすべての集合は $\mathscr{S}$ の集合に含まれます。そして補題が続きます。*

EとFの双対性と互換性のあるE上の$\mathscr{T}$を位相とします。すると、$\mathscr{T}$は$\tau(E, F)$より補題2だけ粗くなり、明らかに$\mathscr{T}$は$\sigma(E, F)$よりより細かいになります。逆に、F は、位相 $\tau(E, F)$ (補題 1) および位相 $\sigma(E, F)$ (II, p. 43, prop. 3) の E の双対であり、従って、$\tau(E, F)$ と $\sigma(E, F)$ の間のすべての位相についても同様です。

#### 系 {#evt-iv-s1-n1-cor-1 .statement tag=07QP}

*p を E 上の準ノルムとします。次の条件は同等です :*

(i) *p は位相 $\tau(E, F)$ まで連続です;*
(ii) *E 上のすべての線型形式 f は、$|f| \leq p$ が F の元から来ます。*

(i) $\Rightarrow$ (ii) : p が $\tau(E, F)$ に対して連続である場合、$|f| \leq p$ が $\tau(E, F)$ に対して連続であるような E 上のすべての線型形式 f は、従って、F の元から補題 1 によって得られます。

(ii) $\Rightarrow$ (i) : $\mathscr{T}$ を、半ノルム p によって定義される E 上の位相とします。 条件 (ii) が満たされる場合、E 上の線型形式は、$\mathscr{T}$ 属するから F まで連続です。 補題 2 $\mathscr{T}$ により、$\tau(E, F)$ より粗くなり、従って、p は$\tau(E, F)$ について連続になります。

#### 注意 2 {#evt-iv-s1-n1-rem-2 .statement tag=07QQ}

*K を、弱者位相 $\sigma(F, E)$ と K の正の尺度 $\mu$ にとってコンパクトな F の凸部分集合とします。*

$$
p(x) = \int_K |B(x, y)| \, d\mu(y)
$$

すべての$x \in E$に。 p が準正規であることは明らかです。さらに、すべての $x \in E$、関係 « すべての $y \in K$ について $|B(x, y)| \leq 1$ » は、$p(x) \leq \mu(K)$ を意味します。これは、E 上の準ノルム p が Mackey 位相 $\tau(E, F)$ に対して連続であることを証明します。 \*

#### 例 {#evt-iv-s1-n1-exa-1 .statement tag=07QR}

G を局所凸空間とし、G' をその双対とする。 G' では、凸コンパクト収束 (III、p. 14) の弱い位相 $\sigma(G', G)$ と位相が、G' と G の間の双対性と互換性があります。 一般に、G' に対するコンパクトな収束の強い位相と位相は、G' と G の間の双対性と互換性がありません。 Recall however that when G is Hausdorff and quasi-complete, the topology of compact convergence on G' coincides with that of convex compact convergence (III, p. 8), hence is compatible with the duality between G' and G.

#### 定義 3 {#evt-iv-s1-def-3 .statement tag=07QS}

*E と F を双対性の 2 つのベクトル空間と、$\sigma(F, E)$ に有界された F の部分集合の族 $\mathscr{T}$ とします。この場合、F 上の $\mathscr{T}$ トポロジは $\beta(E, F)$ で表されます。

同様に、F について定義する位相 $\beta(F, E)$ とします。位相 $\beta(E, F)$ が $\beta(E, F/E^\circ)$ と同一であることは簡単にわかり、E と F の双対性が F で分離している場合も簡約するできます。

*注意。 —* 3) 位相 $\sigma(E, F)$ を備えた空間 E を $E_\sigma$ とします。 $E_\sigma$ のバレル (III、p. 24) は E の部分集合で、凸型でバランスが取れており、閉じており、$\sigma(E, F)$ に対して吸収性があります。これらは他ならぬ F の部分集合の極であり、凸型でバランスが取れており、$\sigma(F, E)$ に向かって境界が定められています。従って、$E_\sigma$ のすべてのバレルのファミリーは、E の位相 $\beta(E, F)$ の 0 の近傍の基本系です。他の語では、E の半ノルムは、$\sigma(E, F)$ でより低い半連続である場合に限り、$\beta(E, F)$ で連続です。 (*cf.* III、p. 24、提案 1)。

4) E と F の間の双対性と互換性のある E 上の $\mathscr{T}$ を位相とします。 F のIV、p. 1、位相 $\beta(F, E)$ の 1、(ii) は、F が E の双対 (位相 $\mathscr{T}$ と) と同一視されるとき、F の強い位相に他なりません。

5) E の位相 $\beta(E, F)$ は $\tau(E, F)$ よりより細かいです。一般に、E と F の二重性とは互換性がありません (*cf.* ただし、§ 2)。特に、$\sigma(E, F)$ に有界である E の部分集合は、必ずしも $\beta(E, F)$ に有界であるとは限りません。

### 2. マッキー位相と局所凸空間の弱体化位相

E を局所凸空間とし、E' をその双対とする。 $E \times E'$ の標準的な双線形形式 $(x, x') \mapsto \langle x, x' \rangle$ を使って E と E' を双対性にします。この二重性は E' で分離しつつあります。 E と E' の間の二重性と互換性のある E 上の 3 つのトポロジを考慮します。

a) E に与えられた位相。混乱が生じそうな場合は常に、これを *頭文字位相* と呼びます。

b) 位相 $\sigma(E, E')$、E の *弱体化位相* と呼ばれます。

c) 位相 $\tau(E, E')$、E では *Mackey 位相* と呼ばれます。

最初の位相は、弱められた位相よりもより細かいで、マッキー位相よりも粗いです。さらに、これら 3 つのトポロジは別個のものにすることもできます (IV、p. 49、演習 8)。

By prop. 1 of IV, p. 1, these three topologies have the same closed convex sets, the same barrels, the same bounded sets and the same adapted bornologies. 特に ：

#### 命題 2 {#evt-iv-s1-prop-2 .statement tag=07QT}

*E を局所的に凸な空間とし、A を E の凸部分集合とします (たとえば、E のベクトル部分空間)。 A の終結は、最初の位相と E の弱体化された位相で同じです。*

#### 注意 1 {#evt-iv-s1-n2-rem-1 .statement tag=07QU}

E の元のファミリー $(x_i)_{i \in I}$ が最初の位相に対して完全である (それぞれ位相的に独立している) ためには、弱体化した位相についても同様であることが必要かつ十分です。これはプロップから続きます。 2. 従って、II、p. 43 の基準を適用できます。

#### 注意 2 {#evt-iv-s1-n2-rem-2 .statement tag=07QV}

$\mathscr{T}_1$ と $\mathscr{T}_2$ を E 上の 2 つのローカル凸トポロジとし、E と $E'$ の間の双対性と互換性があり、$\mathscr{T}_1$ は $\mathscr{T}_2$ よりもより細かいであるとします。次に、$\mathscr{T}_1$ の 0 のすべての近傍は、$\mathscr{T}_1$ に対して凸で閉じられていますが、prop によって $\mathscr{T}_2$ に対して閉じられます。 IV、p. 1 の 1 つ。その結果、(GT、II, § 3, No. 3、系) $\mathscr{T}_2$ に対して完了する E のすべての部分集合は、$\mathscr{T}_1$ にも当てはまります。

特に、弱体化した位相に対して完了したEのすべての部分集合は、初期の位相に対して完了し、初期の位相に対して完了したEのすべての部分集合は、マッキー位相についても同様です。 E が弱体化した位相に対して準完全である場合、E と $E'$ の二重性と互換性のあるすべての位相についても同様です。初期の位相が準完成だとしたら、マッキー位相も同様です。

#### 注意 3 {#evt-iv-s1-n2-rem-3 .statement tag=07QW}

E がハウスドルフ (頭文字位相) であるとします。 A を E の部分集合とします。これは閉じていて $\sigma(E, E')$ に対して有界なので、すべての位相についても E と $E'$ の間の双対性と互換性があります。 A は $\sigma(E, E')$ (III、p. 3、注意 5) に対して事前コンパクトであるため、A が $\sigma(E, E')$ に対して *コンパクト* であると仮定すると、A が $\sigma(E, E')$ に対して *完全* であることと同等です。

したがって、注意 2 により、次のことがわかります。

#### 命題 3 {#evt-iv-s1-prop-3 .statement tag=07QX}

*E がハウスドルフであり、$E'$ がその双対であると仮定します。 E のすべての部分集合は、初期位相では事前コンパクトであり、$\sigma(E, E')$ ではコンパクトですが、初期位相ではコンパクトです。*

#### 注意 4 {#evt-iv-s1-n2-rem-4 .statement tag=07QY}

位相 $\beta(E, E')$ (IV、p. 4、def. 3) は、マッキー 位相よりもより細かいです。 $\beta(E, E')$ が $\tau(E, E')$ と異なる場合、E と $E'$ の間の二重性と互換性がありません。 空間 E は、最初の位相が $\beta(E, E')$ (III、p. 24) に等しい場合にのみバレル化されます。

#### 命題 4 {#evt-iv-s1-prop-4 .statement tag=07QZ}

*E を局所凸空間とする。 E の Mackey 位相は、次の各ケースで最初の位相と同一です:*

a) E はバレル付きです。
b) E は骨相学的です。
c) E は計量化可能です。

まず、E 上のマッキー 位相は、$\sigma(E', E)$ に対してコンパクトである $E'$ のすべての凸部分集合が等連続である場合に限り、最初の位相と同一であることに注意します。 E がバレル (III、p. 24、系) の場合、これは確かに当てはまります。

E がボーンロジーであると仮定します。 V を凸で、位相 $\tau(E, E')$ に対して E で 0 のバランスの取れた近傍とします。 B を E の部分集合とし、最初の位相を境界とします。 B はマッキー 位相に対して有界であるため、V は B を吸収し、E はボーンロジーであるため、V は最初の位相に対して 0 の近傍です。

ケース c) の場合、空間 E はボーンロジカルです (III, p. 12、提案 2)。

### 3. 連続した線形写像の転置

この切断では、$E_1$ と $E_2$ は 2 つの局所的に凸な空間を表し、それぞれ双対 $E'_1$ と $E'_2$ を持ちます。

$u$を$E_1$から$E_2$まで線形写像とします。 $E_1$ と $E_2$ に弱体化トポロジが割り当てられているときに $u$ が連続するためには、すべての $f \in E'_2$ について $f \circ u$ 属するから $E'_1$ であることが必要かつ十分です。これは、$u$ が連続している場合に当てはまります。そして、$E'_2$から$E'_1$までの線形写像$f \mapsto f \circ u$は、$u$の転置と呼ばれ、$^t u$で表されます。

#### 命題 5 {#evt-iv-s1-prop-5 .statement tag=07R0}

*$u$を、$E_1$から$E_2$までの連続した線形写像とします。

(i) *$E_1$ と $E_2$ がハウスドルフである場合、$^t u$ の像が弱い位相 $\sigma(E'_1 : E_1)$ に対して$E'_1$ で密である場合に限り、$u$ は単射法になります。

(ii) *$^t u$が単射であるためには、$u$の像が$E_2$で密であることが必要かつ十分です。*

$E_2$ のベクトル部分空間は、弱体化した位相 (IV、p. 4、提案 2) に対して密度が高い場合に限り、最初の位相に対して密度が高くなります。提案 5 は、II、p. 47、cor から続きます。 2.

#### 命題 6 {#evt-iv-s1-prop-6 .statement tag=07R1}

*$u$ を $E_1$ から $E_2$ までの線形写像とします。これは、弱体化トポロジーで連続です。 $i = 1, 2$ について、$\mathfrak{S}_i$ を $E_i$ の有界な部分集合の族とする。 $^t u$が$(E'_2)_{\mathfrak{S}_2}$から$(E'_1)_{\mathfrak{S}_1}$まで連続する写像である位数では、集合$A \in \mathfrak{S}_1$ごとに、$\mathfrak{S}_2$と実数に集合$A_1, ..., A_n$が存在することが必要十分です。 $\lambda > 0$ は、$\lambda \cdot u(A)$ が $A_1 \cup ... \cup A_n$\footnote{他の語では、$u(\mathfrak{S}_1)$ が最小の適応ボーンロジー 含む $\mathfrak{S}_2$ (III, p. 3) に含まれるようになります。}.*

これはプロップの明らか帰結です。 III、p. 15 の 2 つ。

#### 系 {#evt-iv-s1-n3-cor-1 .statement tag=07R2}

※$u$を$E_1$から$E_2$まで連続する線形写像とします。デュアル $E'_i$ に次のトポロジが割り当てられている場合、$^t u$ は連続的です:*
a) *弱いトポロジ $\sigma(E'_i, E_i)$;*
b) *強力なトポロジー $\beta(E'_i, E_i)$;*
c) *マッキートポロジ $\tau(E'_i, E_i)$;*
d) *プレコンパクト コンバージェンスのトポロジー*
*さらに、$E_2$ がハウスドルフの場合、双対 $E'_i$ が割り当てられている場合、$^t u$ は連続です。*
e) *コンパクト収束*のトポロジー (それぞれ *コンパクト凸*)。

証明を必要とする唯一の点は c) のケースで、$E_1$ と $E_2$ のトポロジーが必ずしもハウスドルフではない場合です。 次に、線型形式 $f \in E'_1*$ ごとに、$f \circ ^t u$ は $E'_2$ で線型形式になります。従って、トポロジー $\sigma(E'_1*, E'_1)$ と $\sigma(E'_2*, E'_2)$ に対して連続する線形写像 $v : E'_1* \to E'_2*$ があり、これは $d_{B_2} \circ u = v \circ d_{B_1}$ になります。ここで、$d_{B_i}$ は $E_i$ から $E'_i*$ ($i = 1, 2$) までの標準写像です。 従って、$A$ が $E_1$ の部分集合であり、$d_{B_1}(A)$ が $\sigma(E'_1*, E'_1)$ に対して凸でバランスが取れておりコンパクトである場合、トポロジー $\sigma(E'_1*, E'_1)$ と $\sigma(E'_2*, E'_2)$ はハウスドルフであるため、$d_{B_2}(u(A)) = v(d_{B_1}(A))$ は$\sigma(E'_2*, E'_2)$ に対して凸でバランスがありコンパクトです。

#### 命題 7 {#evt-iv-s1-prop-7 .statement tag=07R3}

— $u : E_1 \to E_2$ を線形写像とします。 $E_1$ と $E_2$ の弱体化トポロジに対して $u$ が連続していると仮定します。

(i) $E_1$ と $E_2$ に Mackey トポロジが割り当てられている場合、写像 $u$ は連続です。

(ii) $E_1$ がボーンロジカルまたはバレル型である場合、$u$ は $E_1$ と $E_2$ の初期トポロジーに対して連続です。

(iii) $E_1$ と $E_2$ の初期トポロジーで $u$ が連続であるという位数では、$E_2'$ のすべての等連続部分集合の $'u$ の下の像が $E_1'$ で等連続であることが必要かつ十分です。

仮定は、弱いトポロジー $\sigma(E_2', E_2)$ および $\sigma(E_1', E_1)$ (II、p. 46、系) に対して$'u$ が連続であることを意味します。したがって、凸型でバランスのとれたコンパクトな部分集合の$'u$ の下に像が存在します。 $\sigma(E_2', E_2)$ は、$\sigma(E_1', E_1)$ に対して凸型でバランスが取れており、コンパクトです。トポロジー $\sigma(E_2', E_2)$ と $\sigma(E_1', E_1)$ はハウスドルフです。したがって、主張 (i) は GT、X, § 1, No. 4、prop から続きます。 3、b)。 主張 (ii) は (i) の帰結です。つまり、$E_1$ がボーンロジカルまたはバレルドである場合、その最初の位相はマッキー 位相であり、$E_2$ のマッキー 位相は、その最初の位相よりもより細かいです。 $E_2$。最後に、$E_i$ の最初の位相は、$E_i'$ の等連続部分集合への一様収束です (III、p. 19、提案 7 の cor. 1)。これは(iii)を証明する。

#### 系 {#evt-iv-s1-n3-cor-2 .statement tag=07R4}

— $E_1$ が標準の空間であると仮定します。 $u$ を $E_1$ から $E_2$ に線形写像とします。次のプロパティは同等です。

a) $u$ は連続的です。

b) $u$ は、弱体化されたトポロジでは連続です。

c) $u$ の下の $E_1$ にある単位元ボールの像は $E_2$ でバウンドされています。

d) $E_1$ の点のすべての数列 $(x_n)$ は、最初の位相の 0 になる傾向があり、数列 $(u(x_n))$ は、$E_2$ の弱体化された位相に限定されます。

$E_1$ はボーンロジカルであるため、a) と b) の同値は prop から続きます。 7; a)とc)のそれは明らかです。 a)とd)の同値はpropから続きます。 IV、p. 1、およびプロップの 1 つ。 III、p. 11 の 1 つ。

#### 命題 8 {#evt-iv-s1-prop-8 .statement tag=07R5}

— (i) $E$ を、双対 $E'$ を持つ正規の空間とします。 $x \in E$ ごとに、

$$
\|x\| = \sup_{x' \in E', \|x'\| \leq 1} |\langle x, x' \rangle|.
$$

(ii) $E_1$ と $E_2$ を 2 つの正規化空間と $u$ を、$E_1$ から $E_2$ まで連続する線形写像とする。我々は持っています

$$
\|u\| = \|t u\|.
$$

$x \in E$ にしましょう。 $\|x'\| \leq 1$ のようなすべての $x' \in E'$ について、

$$
|\langle x, x' \rangle| \leq \|x\| \cdot \|x'\| \leq \|x\|.
$$

Hahn-Banach 定理 (II, p. 23, cor. 2) によれば、$E'$ には $\|x'\| \leq 1$ と $\langle x, x' \rangle = \|x\|$ のように元 $x'$ が存在します。これは(i)を証明します。

では、(ii)を証明しましょう。 公式 (3) と転置の定義により、

$$
\|^{t}u\| = \sup_{\|y'\| \leq 1} \|^{t}u(y')\| = \sup_{\|y'\| \leq 1, \|x\| \leq 1} |\langle x, ^{t}u(y') \rangle|
= \sup_{\|x\| \leq 1, \|y'\| \leq 1} |\langle u(x), y' \rangle| = \sup_{\|x\| \leq 1} \|u(x)\| = \|u\|.
$$

#### 注意 1 {#evt-iv-s1-n3-rem-1 .statement tag=07R6}

公式 (3) は (4) の特殊なケースで、対応するから線形写像 $\lambda \mapsto \lambda x$ K から E までです。

#### 注意 2 {#evt-iv-s1-n3-rem-2 .statement tag=07R7}

$x \in E_1,\ y' \in E'_2$に$B(x, y') = \langle u(x), y' \rangle = \langle x, ^{t}u(y') \rangle$を入れます。上の証明は、B が $E_1 \times E'_2$ で連続する双線形形式であり、ノルム (GT, X, § 3, No. 2) が $\|u\|$ に等しいことを示しています。

#### 系 {#evt-iv-s1-n3-cor-3 .statement tag=07R8}

— *$\dot{E}$ を可算性の最初の公理であるノルム空間満たすとします。次のような可算部分集合 D の $E' - \{0\}$ が存在します*

$$
\|x\| = \sup_{\xi \in D} |\langle x, \xi \rangle| / \|\xi\|
$$

*全員に* $x \in E$。

B' を、弱い位相 $\sigma(E', E)$ が割り当てられた E の双対 $E'$ の単位元ボールとします。この場合、B' はコンパクトな metrizable 空間 (III, p. 19, cor. 2) です。したがって、B' には可算密な部分集合 D' が存在します。 $D = D' \cap (E' - \{0\})$を入れます。 $x \in E$ にしましょう。 写像 $x' \mapsto \langle x, x' \rangle$ B' から K までは連続なので、

$$
\sup_{x' \in B'} |\langle x, x' \rangle| = \sup_{\xi \in D'} |\langle x, \xi \rangle| \leq \sup_{\xi \in D} |\langle x, \xi \rangle| / \|\xi\| \leq \|x\|.
$$

公式 (3) から (5) が続きます。

### 4. 商空間と部分空間の二重

この切断を通して、Eは局所的に凸な空間、EのMベクトル部分空間、そしてEの双対$E'$におけるMの直交$M^\circ$を表します。$p$をEから$E/M$までの標準写像とします。この場合、$^{t}p$ は単射的であり、像 $M^\circ$ であるため、定義するベクトル空間同型 (トポロジカルではありません)

$$
\pi : (E/M)' \to M^\circ .
$$

同様に、$i$ を M から E への標準単射とします。すると、$^{t}i$ は全射になります (II, p. 24、提案 2)。その核は $M^\circ$ に等しいので、 ベクトル空間同型が得られます (トポロジカルではありません)

$$
i : E'/M^\circ \to M'.
$$

#### 命題 9 {#evt-iv-s1-prop-9 .statement tag=07R9}

— (i) *$(E/M)'$の部分集合Aが*等連続であるためには、*$\pi(A)$*が*$E'$の等連続部分集合であることが必要かつ十分です。

(ii) $\mathfrak{S}$ を、$E$ の有界部分集合の集合とし、$E/M$ の部分集合 $A \in \mathfrak{S}$ の像の$\mathfrak{S}_1$ 集合とします。次に、$\pi$は$(E/M)'_{\mathfrak{S}_1}$から$M^\circ$への同型で、$M^\circ$には$E'_{\mathfrak{S}}$の影響で位相が割り当てられます。

(iii) $E$ がノルム空間であると仮定します。その場合、$\pi$ は、ノルム空間 $(E/M)'$ から $E'$ のノルム部分空間 $M^\circ$ へのアイソメです。

$A$を$(E/M)'$と$B = {}^t p(A) \subset E'$の部分集合とします。置く
$$
q(\xi) = \sup_{\xi' \in A} |\langle \xi, \xi' \rangle|
$$
すべての$\xi \in E/M$に。 $A$ が等連続である位数において、$E/M$ から $\overline{\mathbf{R}}_+$ への写像 $q$ が連続半ノルムであることが必要かつ十分です。これは、$q \circ p$ が $E$ 上の連続半ノルムであることを意味します (II、p. 27、提案 5、(ii))。以来、
$$
(q \circ p)(x) = \sup_{x' \in B} |\langle x, x' \rangle|
$$
すべての $x \in E$ について、これは、$B$ が $E'$ で等連続であることを意味し、(i) が続きます。

$A \in \mathfrak{S}$ と $f$ を $E/M$ で連続する線型形式とします。すべての $\lambda \in \mathbf{R}_+$ について、$A$ に $|{}^t p(f)| \leq \lambda$ がある場合にのみ、$p(A)$ に $|f| \leq \lambda$ が存在します。したがって (ii)。

最後に(iii)を証明します。 $y'$ を $(E/M)'$ に入れます。 An element in $E/M$ has norm $< 1$ if and only if it is the image under $p$ of an element of norm $< 1$ in $E$. したがって、
$$
\begin{align*}
\|y'\| &= \sup_{y \in E/M, \|y\| < 1} |\langle y, y' \rangle| = \sup_{x \in E, \|x\| < 1} |\langle p(x), y' \rangle| \\
&= \sup_{x \in E, \|x\| < 1} |\langle x, {}^t p(y') \rangle| = \|{}^t p(y')\|,
\end{align*}
$$
${}^t p$ 誘導する $(E/M)'$ から $M^\circ$ までのアイソメトリ。

#### 命題 10 {#evt-iv-s1-prop-10 .statement tag=07RA}

— (i) For a subset $A$ of $M'$ to be equicontinuous, it is necessary and sufficient that it is the image under ${}^t i$ of an equicontinuous subset of $E'$.

(ii) $M$ が $E$ で閉じられているとします。 Let $\mathfrak{S}$ be a covering of $E$ consisting of bounded subsets and let $\mathfrak{S}_1$ be the set of subsets of $M$ of the form $M \cap A$ for $A$ in $\mathfrak{S}$. $E'_{\mathfrak{S}}/M^\circ$ から $M'_{\mathfrak{S}_1}$ への全単射線形写像 $i$ は連続です。 $\mathfrak{S}$ が関係 $\subset$ に対して有向集合であり、$\sigma(E, E')$ に対して閉じた凸と密な集合で構成される場合、それは同相同型です。

(iii) $E$ が正規化されていると仮定すると、$i$ は $E'/M^\circ$ から $M'$ までのアイソメトリです。

$E'$ の等連続部分集合の ${}^t i$ の下にある像は、$M'$ の等連続部分集合です (IV、p. 7、提案 7)。逆に、$A$を$M'$の等連続部分集合とします。 $M$の位相は、$E$の連続半ノルムの制限から$M$の集合によって定義されます。したがって、すべての $f \in A$ とすべての $x \in M$ に対して $|f(x)| \leq p(x)$ となるような、$E$ 上の連続的な半ノルム $p$ が存在します。 $B$ を、$E$ のすべての線型形式 $g$ の集合として、$|g| \leq p$ と、制限から $M$ 属するから $A$ とします。 集合 $B$ は $E'$ で等連続です。 Hahn-Banach 定理 (II, p. 23, cor. 1) より、${}^t i(B) = A$ があるため、(i) が続きます。

ここで (ii) を証明します。プロップにより。 $E'_{\mathfrak{S}}$から$M'_{\mathfrak{S}_1}$までIV、p. 6、線形写像${}^t i$の6は連続し、定義するは移行から商まで、線形写像$\iota$が連続します。 $E'_\mathscr{S}/M^\circ$から$M'_{\mathscr{S}_1}$へ。 $\mathscr{T}$を$E'_\mathscr{S}/M^\circ$を$\iota$で移した$M'$の位相とする。これは、$\mathscr{S}_1$ トポロジではなく、より細かいです。

ここで、$\mathscr{S}$ が $\subset$ に対して有向集合であり、$\sigma(E, E')$ に対して閉じた、凸型、バランスが取れたコンパクトな集合で構成されているとします。 $\iota$ が同相写像であること、つまり、$\mathscr{T}$ が $M'$ の $\mathscr{S}_1$ トポロジーよりも粗いことを示すには、$\mathscr{T}$ が $M'$ と $M$ の双対性と互換性があり、すべての等連続集合が一致することを証明するだけで十分です。 $M$ ($M$ と $\mathscr{T}$ の双対とみなされる) は、集合所属から $\mathscr{S}_1$ の相似形に含まれます。 $\mathscr{T}$は$\mathscr{S}_1$-トポロジーよりより細かいで、$\mathscr{S}_1$は$M$の覆いなので、$M'$上の線型形式$y' \mapsto \langle y, y' \rangle$は$y \in M$ごとに$\mathscr{T}$連続します。 $f$ を $M'$ で線型形式とし、これは $\mathscr{T}$ にわたって連続します。そうすると、$f \circ \iota$ は $E'_\mathscr{S}$ で連続する線型形式になります。 The $\mathscr{S}$-topology on $E'$ is coarser than the Mackey topology $\tau(E', E)$; for, the mapping $d_B : E \to {E'}^*$ is continuous for the topologies $\sigma(E, E')$ and $\sigma({E'}^*, E')$, and since the latter is Hausdorff, the image under $d_B$ of a set which is compact for $\sigma(E, E')$ is compact for $\sigma({E'}^*, E')$. IV、p. 3 の補題 1 までに、すべての $x' \in E'$ に対して $f(\iota(x')) = \langle x_0, x' \rangle$ となるような $x_0 \in E$ が存在します。 特に、すべての $x' \in M^\circ$ に対して $\langle x_0, x' \rangle = 0$ があり、$M$ が $E$ で閉じているため、$x_0 \in M$ (II、p. 45、cor. 2) が得られます。そして最後に、$y' \in M'$全員に対して$f(y') = \langle x_0, y' \rangle$です。 これは、$\mathscr{T}$ * $M$ * と* $M'$ の二重性と互換性があることを証明します。

ここで、$A$ を $M'$ の位相 $\mathscr{T}$ に対して等連続である $M$ の部分集合とします。 $\mathscr{T}$ の定義により、$\mathscr{S}$ が指示されている仮定を考慮すると、集合 $B \in \mathscr{S}$ 含む 0 が存在し、数 $|\langle y, x' \rangle|$ の上界 $\lambda$ が存在することを意味します。 $y \in A$ と $x' \in B^\circ$ は有限です (III, p. 19、提案 7)。 $B$ は $E$ で閉じているため、双極性の定理 (II、p. 44、th. 1) は、$A \subset \lambda(B \cap M)$ があることを示します。これで(ii)の証明は完了です。

これから(iii)を証明していきます。 $y' \in M'$ にしましょう。 公式を証明してみます

$$
\|y'\| = \inf_{\iota(x') = y'} \|x'\|.
$$

プロップにより。 8、IV、p. 7 の (ii)、$\|\iota\| = \|i\|$ があるため、$\|\iota\| \leq 1$、そして

$$
\|y'\| \leq \inf_{\iota(x') = y'} \|x'\|.
$$

ハーン・バナッハ定理 (II, p. 23, cor. 3) によれば、$E$ には拡大する $y'$ と同じノルムである線型形式 $x'_0$ が存在します。したがって、$\iota(x'_0) = y'$ なので、(7) の反対の不等式が得られます。

#### 注意 {#evt-iv-s1-n4-rem-1 .statement tag=07RB}

— 私たちは、$\iota$ が $E'_s/M^\circ$ から $M'_s$ へのトポロジカルベクトル空間同型 (弱い双対) であることを知っています (II、p. 48、提案 7、(ii))。コンパクトな凸収束の位相の場合は、prop。図10は、$E$がハウスドルフで$M$が$E$で閉じられたとき、$\iota$は$E'_{cc}/M^\circ$から$M'_{cc}$まで同型であることを示しています。強力なトポロジの場合、$\iota$ は $E'_b/M^\circ$ から $M'_b$ まで連続する写像です。 $E$ が Banach 空間 \* である場合、または $E$ が半再帰的で、$M$ が $E$ (IV, p. 15) * で閉じている場合、それは同型ですが、$E$ がフレシェ空間 (IV, p. 58、演習 5、*c*))。

#### 命題 11 {#evt-iv-s1-prop-11 .statement tag=07RC}

— (i) *$E/M$ で位相が弱体化* $E$ での商です。 *$M$ で *位相が弱体化* $E$ の影響で誘発されます。

(ii) *E/M のマッキー 位相は E のマッキー 商です。 M 上のマッキー 位相は、τ(E, E') によって誘導された位相よりもより細かいです。*

主張 (i) はプロップから続きます。 II、p. 48の7。

標準単射 $i : M \to E$ は、弱体化トポロジでは連続です。したがって、Mackey トポロジ $\tau(M, M')$ および $\tau(E, E')$ では連続です (IV、p. 7、提案 7)。同様に、正規の射影 $p : E \to E/M$ は Mackey トポロジでは連続です。 $\tau(E, E')$ から取得された $E/M$ の商位相は、$E/M$ と $(E/M)'$ の間の双対性と互換性があるため、Mackey の $E/M$ の Mackey 位相よりも粗いことがすぐにわかります。 定理 (IV、p. 2、th. 1)。これは(ii)を証明します。

### 5. 直和と積のデュアル

すべての $i \in I$ について、$(E_i, F_i)$ を双線形形式 $B_i$ による双対性のベクトル空間、集合の対とします。 $E = \prod_{i \in I} E_i$と$F = \bigoplus_{i \in I} F_i$を入れて、$F$の部分空間でそれぞれ$F_i$を同一視するとします。 双線形形式を使って $E$ と $F$ を双対性にします

$$
B(x, y) = \sum_{i \in I} B_i(x_i, y_i) \quad \text{for} \quad x = (x_i) \quad \text{and} \quad y = (y_i)
$$

(家族 $(B_i(x_i, y_i))_{i \in I}$ には有限台がいます)。

弱い位相 $\sigma(E, F)$ は弱いトポロジー $\sigma(E_i, F_i)$ の積であることを思い出します (II、p. 50、提案 8)。

#### 補題 3 {#evt-iv-s1-lem-3 .statement tag=07RD}

— (i) *すべての $i \in I$ について、$\mathfrak{S}_i$ を $\sigma(F_i, E_i)$ の範囲にある $F_i$ の部分集合の族とします。 $\mathfrak{S} = \bigcup_{i \in I} \mathfrak{S}_i$を入れます。この場合、$E$ の $\mathfrak{S}$ トポロジは、$E_i$ の $\mathfrak{S}_i$ トポロジの積になります。

(ii) *すべての $i \in I$ について、$\mathfrak{J}_i$ を、弱い位相 $\sigma(E_i, F_i)$ に恵まれた空間 $E_i$ に適応した生まれつき学とし、$\{ \varnothing \}$ に等しいものはありません。 $\mathfrak{J}$ を、$E = \prod_{i \in I} E_i$ の部分集合 $A$ の家族とし、すべての $i \in I$ に対して $\operatorname{pr}_i(A) \in \mathfrak{J}_i$ とします。この場合、$F$ の $\mathfrak{J}$ トポロジは、$F_i$ の $\mathfrak{J}_i$ トポロジの直和になります。

$\mathscr{T}$ を $\mathfrak{S}_i$ トポロジーの積とします。 集合/形

$$
A = \prod_{i \in J} A_i^\circ \times \prod_{i \in I - J} E_i
$$

ここで、$J \subset I$ は有限であり、すべての $i \in J$ に対して $A_i \in \mathfrak{S}_i$、形は $\mathscr{T}$ の 0 の近傍の基本的な系です。 $A = (\bigcup_{i \in J} A_i)^\circ$ があるため、$\mathscr{T}$ は $\mathfrak{S}$ トポロジと同一です。これは(i)を証明します。

$\mathfrak{J}$ トポロジを $F$ に割り当て、$\mathfrak{J}_i$ トポロジを各 $F_i$ に割り当てます。 $E$ の部分集合 $A$ ごとに $F_i \cap A^\circ = \operatorname{pr}_i(A)^\circ$ があり、したがって $F_i$ から $F$ までの単射は連続です。 $q$ を $F$ の準標準とします。 $q$ から $F_i$ の制限 $q_i$ がすべての $i \in I$ で連続していると仮定します。次に、次のような空ではない部分集合 $A_i \in \mathfrak{J}_i$ を見つけることができます。

$$
q_i(y_i) \leq \sup_{x_i \in A_i} |B_i(x_i, y_i)| \quad (y_i \in F_i) .
$$

$A = \prod_{i \in I} A_i$を入れてください。それから$A \in \mathfrak{J}$。 $F$の$y = (y_i)_{i \in I}$については、
$$
q(y) \leq \sum_{i \in I} q_i(y_i) \leq \sum_{i \in I} \sup_{x_i \in A_i} |B_i(x_i, y_i)| = \sup_{x \in A} |B(x, y)|,
$$
ここで、最後の等式は (8) から続きます。なぜなら、ファミリー $(y_i)_{i \in I}$ には有限台があり、$A_i$ は空ではなく、バランスが取れていると想定できるからです (GT、IV, § 5, No. 7、cor. 2 から prop. 12)。この不等式は、$q$ が $F$ で連続であること、したがって (ii) を証明します。

#### 命題 12 {#evt-iv-s1-prop-12 .statement tag=07RE}

*位相 $\beta(F, E)$ は、トポロジ $\beta(F_i, E_i)$ の直和です。 位相 $\beta(E, F)$ は、トポロジ $\beta(E_i, F_i)$ の積です。*

$\sigma(F_i, E_i)$ を境界とする $F_i$ のすべての部分集合のファミリーを $\mathfrak{S}_i$ に、そして $\sigma(E_i, F_i)$ を境界とする $E_i$ のすべての部分集合のファミリーを$\mathfrak{J}_i$ として、補題 3 を適用します。

コルによって。 III、p. 4、$\mathfrak{J}$ の 2 は、$\sigma(E_i, F_i)$ の積位相に限定される $E_i$ のすべての部分集合の族であり、$\sigma(E, F)$ と同一です。したがって、$\beta(F, E)$ の主張が続きます。

$F = \bigoplus_{i \in I} F_i$ に、トポロジー $\sigma(F_i, E_i)$ の直和である位相 $\mathscr{T}$ を与えます。次に、$F$ の双対は $x$ が $E$ を通る線型形式 $y \mapsto B(x, y)$ で構成されます (II、p. 30、提案 6)。プロップにより。 IV、p. 1 の 1、トポロジ $\mathscr{T}$ および $\sigma(F, E)$ は同じ境界集合を持ちます。まず、トポロジー $\sigma(F_i, E_i)$ がハウスドルフであると仮定します。プロップにより。 III、p. 5 の 5 つ、これらの集合は、形 $\sum_{i \in J} B_i$ の部分集合に含まれ、$J \subset I$ は有限で、$B_i$ はすべて$F_i$ ($\sigma(F_i, E_i)$ の場合) に制限されます。 $i \in J$。 $\sum_{i \in J} B_i$ は$n = \mathrm{Card}(J)$ の凸包絡線$\bigcup_{i \in J} nB_i$ に含まれているので、この場合$\beta(E, F)$ で主張を証明するには、補題 3 を適用できます。

一般的なケースでは、$N_i$ を $\sigma(F_i, E_i)$ の 0 のすべての近傍のうちの共通部分とし、$N = \sum_{i \in I} N_i$ とします。その場合、$F/N$ は $F_i/N_i$ のトポロジカル直和です (II、p. 31、提案 8)。このことから、$\mathscr{T}$ に制限される$F$ のすべての部分集合は、$J \subset I$ が有限で、$B_i$ がすべての $i \in J$ について$F_i$ に制限される、形 $N + \sum_{i \in J} B_i$ の集合に含まれると推測します。 (III、p. 2、*注意* 3);この$E$の集合の極点は$\sum_{i \in J} B_i$の極点と同じであるため、結果は上記のようになります。

#### 命題 13 {#evt-iv-s1-prop-13 .statement tag=07RF}

*Mackey 位相 $\tau(F, E)$ は、Mackey トポロジ $\tau(F_i, E_i)$ の直和です。 位相 $\tau(E, F)$ は、トポロジ $\tau(E_i, F_i)$ の積です。*

$\tau(F, E)$ の主張は、補題 3 (ii) と次の性質から続きます: $F^* = \prod_{i \in I} F_i^*$ の閉じた凸型でバランスの取れた部分集合が $\sigma(F^*, F)$ に対してコンパクトであるためには、各 $F_i^*$ の射影がコンパクトであることが必要かつ十分です$\sigma(F_i^*, F_i)$。

To prove the assertion on $\tau(E, F)$, assume first that the topologies $\sigma(F_i, E_i)$ are Hausdorff, it is enough (lemma 3 (i)) to prove that every subset $A$ of $F$ which is convex, balanced and compact for $\sigma(F, E)$ is contained in a set of the form $\sum_{i \in J} A_i$ where $J \subset I$ is finite and where $A_i$ is convex, balanced and compact for $\sigma(F_i, E_i)$. しかし、そのような部分集合は $\sigma(F, E)$ に限定されます。 By the proof of prop. 12, there exists a finite subset $J$ of $I$ such that $A \subset \sum_{i \in J} F_i$, and it is enough to take for $A_i$ the projection of $A$ on $F_i$.

一般的なケースでは、プロップの証明と同じ記法を使用します。図 12 では、$\tau(E_i, F_i) = \tau(E_i, F_i/N_i)$ と $\tau(E, F) = \tau(E, F/N)$ (IV、p. 2) があり、$F/N$ は $F_i/N_i$ のトポロジー 直和であるため、前のケースに帰着します。

Q.E.D.

この段落の残りの部分では、$(E_i)_{i \in I}$ が局所的に凸な空間の族であると仮定します。 $S$ が $E_i$ と $P$ のトポロジー 直和、それらの積を表すものとします。私たち定義する線形写像 $\theta : S' \to \prod_{i \in I} E_i'$ は、*正規* であると言われています。

$$
\theta(x') = (x'|E_i)_{i \in I} \quad (x' \in S')
$$

(ここで、$S'$ は $S$ の双対を表し、$E_i'$ は $E_i$ の双対を表します)。

#### 命題 14 {#evt-iv-s1-prop-14 .statement tag=07RG}

(i) *写像 $\theta$ は、$S = \bigoplus_{i \in I} E_i$ の強い (それぞれ弱い) 双対から $E_i$ の強い (それぞれ弱い) 双対の積への同型です。

(ii) *$S'$の部分集合$A$が等連続であるためには、$\theta(A)$の$E_i'$上の射影がすべての$i \in I$で等連続であることが必要かつ十分です。

(iii) *Mackey 位相 $\tau(S, S')$ は、Mackey トポロジ $\tau(E_i, E_i')$ の直和です。*

(iv) *位相 $\beta(S, S')$ は、トポロジー $\beta(E_i, E_i')$ の直和です。*

$\theta$ が全単射であることは、トポロジカル直和の定義 (II, p. 30、提案 6) の直後に続きます。 主張 (i) は prop から続きます。 IV、p. 12 の 12 個、強力なトポロジ用、およびプロップから。 II の 8、p. 50、弱いトポロジ用。同様に (iii) は prop から続きます。 13 (IV、p. 12) および (iv) プロップから。 12 (IV、p. 12)。

(ii) を証明するには、$A$ を $S'$ の部分集合とします。置く

$$
q(x) = \sup_{x' \in A} |\langle x, x' \rangle| \quad \text{for} \quad x \in S ;
$$

$q_i$ は $q$ から $E_i$、よっての制限を表します

$$
q_i(x_i) = \sup_{x_i' \in A_i} |\langle x_i, x_i' \rangle| \quad \text{for} \quad x_i \in E_i ,
$$

ここで、$A_i$ は、$E_i'$ 上の $\theta(A)$ の射影を表します。 $A$ が等連続であるためには、$q$ が有限 (つまり、各 $q_i$ が有限である) で連続であることが必要かつ十分です。位相幾何学的な直和 (II, p. 27, 提案 5) 上の連続半ノルムの特徴付けを考慮すると、これは、それぞれの $q_i$ が連続であると仮定すること、または実際に、それぞれの集合 $A_i$ が等連続であると仮定するのと同じです。

$\phi$ を *正規* と言われる線形写像とし、$\bigoplus_{i \in I} E_i'$ から公式によって定義される $P = \prod_{i \in I} E_i$ の双対 $P'$ にします。

$$
\langle x, \phi(x') \rangle = \sum_{i \in I} \langle x_i, x'_i \rangle
$$

$P$の$x = (x_i)$と$\bigoplus_{i \in I} E'_i$の$x' = (x'_i)$。

#### 命題 15 {#evt-iv-s1-prop-15 .statement tag=07RH}

— (i) *写像 $\phi$ は、$E_i$ の強い双対のトポロジカル直和から $P = \prod_{i \in I} E_i$ の強い双対への同型です。

(ii) *$P'$の部分集合$A$が等連続であるためには、それが有限和$\sum_{i \in J} \phi(A_i)$に含まれていることが必要かつ十分であり、$J \subset I$は有限であり、$A_i$はすべての$E'_i$に等連続である$i \in J$.*

(iii) *Mackey 位相 $\tau(P, P')$ は、トポロジー $\tau(E_i, E'_i)$ の積です。*

(iv) *位相 $\beta(P, P')$ は、トポロジー $\beta(E_i, E'_i)$ の積です。*

$\phi$が単射であるのは明らかです。 $P$ の 0 の近傍の基本的な系は、形 $V = \prod_{i \in J} V_i \times \prod_{i \in I - J} E_i$ の集合で構成されます。ここで、$J \subset I$ は有限で、$V_i$ は $i$ の $E_i$ の 0 の近傍です。 $J$。 $P'$の$V$の極は$\sum_{i \in J} \phi(V_i^0)$に等しい。

これは、$\phi$ と主張 (ii) の全射性を証明します。

主張 (i) と (iv) は prop から続きます。 12 (IV、p. 12) および (iii) プロップから。 13 (IV、p. 12)。

#### 系 {#evt-iv-s1-n5-cor-1 .statement tag=07RI}

— *バレル化された空間のすべての積がバレル化されます。*

局所的に凸の空間 $E$ は、最初の位相が $\beta(E, E')$ (IV、p. 4、*注意 3*) と同一である場合にのみバレルされます。したがって、propを適用するだけで十分です。 15(iv)。

### 練習問題 {#evt-iv-s1-exercises}

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
