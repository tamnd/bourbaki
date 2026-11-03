---
book: evt
book_title: Topological Vector Spaces
chapter: III
chapter_title: SPACES OF CONTINUOUS LINEAR MAPPINGS
section: 5
section_title: Hypocontinuous bilinear mappings
lang: ja
source: evt-i-v
book_pages: TVS III.28-TVS III.33, TVS III.46-TVS III.49
pdf_pages: 0160-0165, 0178-0181
extraction: ocr
subsections:
    - "no": 1
      title: Separately continuous bilinear mappings
      page: 28
      pdf_page: 160
    - "no": 2
      title: Separately continuous bilinear mappings on a product of Fréchet spaces
      page: 29
      pdf_page: 161
    - "no": 3
      title: Hypocontinuous bilinear mappings
      page: 30
      pdf_page: 162
    - "no": 4
      title: Extension of a hypocontinuous bilinear mapping
      page: 32
      pdf_page: 164
    - "no": 5
      title: Hypocontinuity of the mapping $(u, v) \mapsto v \circ u$
      page: 32
      pdf_page: 164
statements: 16
exercises: 15
content_sha256: 2c0e5bad1b808bba5559192c8325100aa94d49e298e180a8009fd912366e0fef
translated_from: content/en/evt/III/05_s5_hypocontinuous_bilinear_mappings.md
translation_method: google
source_content_sha256: eefe4b53c6330aa7a5e81cb0b9c60f3b12b31b2df9f7ff14d5388452b92097de
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 67532201240910ebbb0fa3f035209fd3764ecbb811a79e291e3c64f66a236907
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 5。非連続双線形マッピング

### 1. 個別に連続する双線形マッピング

$E, F, G$を局所的に3凸空間とする。 For every bilinear mapping $u$ from $E \times F$ into $G$, and for every $x \in E$ (resp. $y \in F$), we denote by $u(x, .)$ (resp. $u(., y)$) the mapping $y \mapsto u(x, y)$ (resp. $x \mapsto u(x, y)$) from $F$ into $G$ (resp. from $E$ into $G$).

#### 定義 1 {#evt-iii-s5-def-1 .statement tag=07P9}

*$E \times F$ から $G$ への双線形写像 $u$ は、$F$ から $G$ までのすべての $x \in E$、線形写像 $u(x, .)$ が連続であり、すべての $y \in F$、線形写像 $u(., y)$ が連続であると言われます。 $E$ から $G$ までは連続です。*

定義の直後に次の命題が続きます。

#### 命題 1 {#evt-iii-s5-prop-1 .statement tag=07PA}

*$E \times F$ から $G$ への双線形写像 $u$ が個別に連続であるためには、$E$ から $G$ までのすべての $y \in F$、線形写像 $u(., y)$ が連続であり、線形写像 $y \mapsto u(., y)$ が連続であることが必要かつ十分です。 $F$ から $\mathscr{L}_s(E; G)$ は連続です。*

また、すべての線形写像 $v \in \mathscr{L}(F; \mathscr{L}_s(E; G))$ には双線形写像 $(x, y) \mapsto v(y)(x)$ が関連付けられており、その後 $E \times F$ から $G$ まで個別に連続する双線形写像の $\mathscr{L}(F; \mathscr{L}_s(E; G))$ からベクトル空間への線形 *全単射* が定義する行われるとも言えます。

$E \times F$ から $G$ への個別に連続する双線形マッピングは、必ずしも $E \times F$ で連続である必要はありません (III、p. 47、演習 2、cf. ただし、III、p. 30、および IV、p. 26、演習 2)。

2 つの局所凸空間の積 $E_1 \times E_2$ 上の別々に連続する双線形 *形式* の概念は、$E_1$ と $E_2$ に *弱い* トポロジー (II、p. 42) が割り当てられている場合、連続線形写像の概念に直接関係します。 $(E_1, F_1)$ と $(E_2, F_2)$ が 2 つの実数ペアであると仮定します。分離双対性における (それぞれ複素数) ベクトル空間 (*loc. cit.*)。 $i = 1, 2$ の弱いトポロジー $\sigma(E_i, F_i)$ (それぞれ $\sigma(F_i, E_i)$) を $E_i$ (それぞれ $F_i$) に割り当て、$E_1 \times E_2$ 上の別々の *連続* 双線形形式のベクトル空間を $B(E_1, E_2)$ で表します。 適用小道具。 1 を $G = K$ の場合に当てはめると、すべての双線形形式 $\Phi \in B(E_1, E_2)$ とすべての $x_2 \in E_2$ について、写像 $x_1 \mapsto \Phi(x_1, x_2)$ は $E_1$ 上で連続する線型形式であることがわかります。したがって、(II, p. 43, prop. 3) 元と $^d\Phi(x_2) \in F_1$ は 1 つだけ

$$
\Phi(x_1, x_2) = \langle x_1, ^d\Phi(x_2) \rangle
$$

$x_1 \in E_1$ と $x_2 \in E_2$ ごとに;さらに、写像 $^d\Phi : E_2 \to F_1$ は、$E_2$ と $F_1$ の (弱い) トポロジに対して線形で *連続* です。

逆に、連続するすべての線形写像 $u : E_2 \to F_1$ 写像 $(x_1, x_2) \mapsto \Phi(x_1, x_2) = \langle x_1, u(x_2) \rangle$ は、$E_1 \times E_2$ 上で個別に連続する双線形形式となり、$u = {}^d \Phi$ が得られます。したがって、私たちは $B(E_1, E_2)$ から $\mathscr{L}(E_2; F_1)$ までの同型 $d : \Phi \mapsto {}^d \Phi$ を *標準* であると定義しました。同様に公式

$$
\Phi(x_1, x_2) = \langle {}^s \Phi(x_1), x_2 \rangle
$$

定義する $B(E_1, E_2)$ から $\mathscr{L}(E_1, F_2)$ への *正規* 同型 $s : \Phi \to {}^s \Phi$。明らかに可換性図式があります

$$
\begin{array}{ccc}
& B(E_1, E_2) & \\
s & / & d \\
\downarrow & & \downarrow \\
\mathscr{L}(E_1; F_2) & \leftrightarrow & \mathscr{L}(E_2; F_1)
\end{array}
$$

ここで、$t$ は転置の同型 (II、p. 46、提案 5 および系) です。 $F_1$と$F_2$の弱いトポロジの定義を考慮すると、$B(E_1, E_2)$、$\mathscr{L}(E_1; E_2)$、$\mathscr{L}(E_2; F_1)$に単純収束*の*位相、図式(3)の*同型が割り当てられるのは明らかです。トポロジカルベクトル空間同型*。

### 2. Fréchet 空間の積上の個別に連続する双線形マッピング

#### 命題 2 {#evt-iii-s5-prop-2 .statement tag=07PB}

※E、F、Gを局所的に3凸空間とする。 E と F が計量可能であり、E がバレル化されていると仮定します。 H を E × F から G への個別連続双線形写像の集合とします。すべての $x \in E$ について、F から G までの写像 $u(x, .)$ の集合 (u は H を通過します) が等連続であるとします。この場合、H は等連続です。*

$U_n$ (それぞれ $V_n$) を E (それぞれ F) の 0 の近傍の基本音数列とします。 H が等連続でない場合、G に 0 の閉じた凸型の平衡型近傍 W が存在し、すべての $n$、$H(U_n \times V_n)$ が W に含まれないことになります。その場合、対 $(x_n, y_n) \in U_n \times V_n$ の数列、および数列 $(u_n)$ が存在します。 H の元は、$u_n(x_n, y_n) \notin W$ になります。 $p$ を W のゲージとします。すべての $y \in F$ とすべての $u \in H$ について、E から G までの写像 $u(., y)$ は連続です。したがって、$p \circ u(., y)$ は E 上の連続半ノルムです。一方、すべての $x \in E$、集合については、 $u \in H$ の写像 $u(x, .)$ は等連続です。 数列 $(y_n)$ は 0 になる傾向があるため、有界であり、$n \geq 0$ と $u \in H$ のすべての $u(x, y_n)$ のうち集合は有界です (III、p. 22、提案 9)。このことから、写像 $p'(x) = \sup_{\substack{u \in H \\ n \geq 0}} p(u(x, y_n))$ は E の上の下位半連続半ノルム (有限) であることがわかります。E はバレル化されているため、$p'$ は連続です (III, p. 24, 系)。 E では $(x_n)$ は 0 になる傾向があり、$p'(x_n)$ も 0 になる傾向があるため、$n$ が十分に大きい場合は $p'(x_n) \leq 1$ になります。しかし、その後 $p(u_n(x_n, y_n)) \leq p'(x_n) \leq 1$ となり、したがって $u_n(x_n, y_n) \in W$ となり、$u_n, x_n, y_n$ では矛盾する仮定となります。

#### 系 1 {#evt-iii-s5-prop-2-cor-1 .statement tag=07PC}

— E と F を 2 つのフレシェ空間とし、G を局所的に凸な空間とします。 $E \times F$ から G までの個別に連続する双線形写像は連続です。

実際、すべてのフレシェ空間は樽詰めされています (III、p. 25、系)。

E と F を 2 つの局所凸空間とします。 $\mathscr{B}(E, F)$ を使用して、形 $A \times B$ の集合で一様収束の位相を使用して、$E \times F$ での連続双線形形式の空間を表します。ここで、A (それぞれ B) は E (それぞれ F) で制限されています。 公式
$$
u(x, y) = \langle y, \phi(u)(x) \rangle
$$
($x \in E, y \in F$ と $u \in \mathscr{B}(E, F)$ の場合) 定義する写像 $\phi$ $\mathscr{B}(E, F)$ から $\mathscr{L}_b(E; F'_b)$ への連続線形注入。

#### 系 2 {#evt-iii-s5-prop-2-cor-2 .statement tag=07PD}

— E と F が計量可能であり、E がバレル化されていると仮定します。この場合、$\phi$ は、$\mathscr{B}(E, F)$ から $\mathscr{L}_b(E; F'_b)$ へのトポロジカルベクトル空間同型です。

$f \in \mathscr{L}_b(E; F'_b)$ にしましょう。 $x \in E$と$y \in F$に$u(x, y) = \langle y, f(x) \rangle$を入れます。 $E \times F$ の双線形形式 $u$ は個別に連続しています。プロップによって。 2、それは属するから$\mathscr{B}(E, F)$で、$f = \phi(u)$があります。したがって、$\phi$ は、$\mathscr{B}(E, F)$ から $\mathscr{L}_b(E; F'_b)$ までの直線である全単射です。 $\phi$ が共連続であるのは明らかであるため、cor になります。 2が続きます。

### 3. 非連続双線形写像

以下では、連続双線形写像と個別連続双線形写像の中間である定義する概念とします。

#### 命題 3 {#evt-iii-s5-prop-3 .statement tag=07PE}

— E、F、G を 3 つの局所凸空間、E の有界部分集合の族である $\mathfrak{S}$ とします。 u を $E \times F$ から G まで個別に連続する双線形写像とします。以下のプロパティは同等です。

a) G の 0 のすべての近傍 W とすべての集合 $M \in \mathfrak{S}$ に対して、$u(M \times V) \subset W$ となる F の 0 の近傍 V が存在します。

b) 写像 $x \mapsto u(x, .)$ の下の M のすべての集合 $M \in \mathfrak{S}$、像は、$\mathscr{L}(F; G)$ の等連続部分集合です。

c) F から $\mathscr{L}_{\mathfrak{S}}(E; G)$ までの写像 $y \mapsto u(., y)$ は連続です。

a) $\mathscr{L}_{\mathfrak{S}}(E; G)$ (III, p. 13) の 0 の近傍の定義により、$y \mapsto u(., y)$ が点 0 で連続であることを表します。同様に a) は、写像 $x \mapsto u(x, .)$ の下の M の像が点 0 (III, p. 16) で等連続であることを表します。

#### 定義 2 {#evt-iii-s5-def-2 .statement tag=07PF}

— u を $E \times F$ から G への双線形写像とします。u が個別に連続であり、prop の同等の条件 a)、b)、c) の 1 つが検証される場合、u は $\mathfrak{S}$-次連続であると言います。 3.

条件 c) プロップ。図 3 は、$\mathfrak{S}$ 非連続双線形写像の概念が、$\mathscr{L}(E, G)$ 上の $\mathfrak{S}$ トポロジを通じてのみ $\mathfrak{S}$ に依存していることを示しています。

F の有界部分集合のすべての集合 $\mathfrak{T}$ に対して、同様に $\mathfrak{T}$ 次次連続写像の定義する概念を、prop における E と F の役割交換することによって行います。 3. 個別に連続する双線形写像 u は、$\mathfrak{S}$-hypocontinuous と $\mathfrak{T}$-hypocontinuous の両方である場合、$(\mathfrak{S}, \mathfrak{T})$-hypocontinuous であると言われます。

$E \times F$ から $G$ へのすべての *連続* 双線形写像は、有界部分集合の集合の対 $(\mathscr{S}, \mathscr{T})$ ごとに $(\mathscr{S}, \mathscr{T})$ 準連続です: 0 の近傍 $W$ ごとに$G$、$E$ には 0 の近傍 $U$ が存在し、$F$ には 0 の近傍 $V$ が存在し、$u(U \times V) \subset W$ になります。すべての集合 $M \in \mathscr{S}$ は有界であるため、$\lambda M \subset V$ となるような $\lambda > 0$ が存在します。

$$
u(M \times \lambda V) = u(\lambda M \times V) \subset u(U \times V) \subset W .
$$

逆は一般に偽です (III、p. 47、演習 3)。

#### 命題 4 {#evt-iii-s5-prop-4 .statement tag=07PG}

*$u$ を $E \times F$ から $G$ までの $\mathscr{S}$ 準連続双線形写像とします。 集合 $M \in \mathscr{S}$ ごとに、$u$ から $M \times F$ の制限は連続しており、$u(M \times Q)$ は、$F$ の境界のある部分集合 $Q$ ごとに $G$ で境界づけられます。

最初の主張は cor から続きます。 GTの3、X, § 2, No. 1。 $W$ を $G$ の 0 の近傍とします。 $F$ には、仮定, 近傍 $V$ が存在し、$u(M \times V) \subset W$ になります。 $\lambda Q \subset V$のような$\lambda \neq 0$が存在するので、$\lambda u(M \times Q) = u(M \times \lambda Q) \subset W$があり、これは命題の2番目の部分を証明します。

#### 命題 5 {#evt-iii-s5-prop-5 .statement tag=07PH}

*$u$ を $E \times F$ から $G$ までの $(\mathscr{S}, \mathscr{T})$ 準連続双線形写像とします。 集合のすべての対 $M \in \mathscr{S}$、$N \in \mathscr{T}$、$u$ は$M \times N$ で均一に連続します。*

命題はプロップの直後に続きます。 GT、X, § 2, No. 1、プロップの2台。 GTの5、X, § 2, No. 2。

#### 命題 6 {#evt-iii-s5-prop-6 .statement tag=07PI}

*$F$ がバレル化された空間の場合、$E \times F$ から局所的に凸な空間 $G$ への個別に連続する双線形マッピング $u$ は、有界部分集合のすべての集合 $\mathscr{S}$ に対して $\mathscr{S}$ 亜連続になります。 $E$.*

他の語では、$F$ から $\mathscr{L}_b(E; G)$ までの *線形写像* $y \mapsto u(., y)$ は *連続* です。

$x \mapsto u(x, .)$ の下の $E$ のすべての有界部分集合 $M$ の像が $\mathscr{L}(F; G)$ で等連続であることを証明するには (III, p. 30, 提案 3) で十分です。しかし、プロップのおかげで。 1 (III, p. 28) この像は $\mathscr{L}(F; G)$ の単純有界部分集合であり、$F$ はバレル化されているため、$\mathscr{L}(F; G)$ のすべての単純有界部分集合は等連続です (III, p. 25, 1)。

#### 注意 {#evt-iii-s5-n3-rem-1 .statement tag=07PJ}

— $F$ の位相が $F$ 上の最も細かい局所凸位相であり、線形写像 $h_\alpha : F_\alpha \to F$ が連続しているとします (II、p. 27)。次に、プロップの条件 *c)*。 3 (III、p. 30) は、$E$ と $G$ が局所的に凸である場合、双線形写像 $u : E \times F \to G$ は、各双線形写像が次の場合に限り、$\mathscr{S}$ 準連続であることを示しています。

$$
(x, y_\alpha) \mapsto u(x, h_\alpha(y_\alpha))
$$

$E \times F_\alpha$ から $G$ へは $\mathscr{S}$ - 非連続です。

ここで、$E$ が局所凸空間であり、$E$ (II, p. 33) の閉ベクトル部分空間の増加シーケンス $(E_n)$ の *厳密な* 帰納限界であると仮定します。その場合、すべての集合 $M \in \mathscr{S}$ は $E_n$ の 1 つに含まれ、この部分空間内で境界付けされます (III、p. 5、提案 6)。 $E_n$ に含まれるすべての部分集合所属から $\mathscr{S}$ のファミリーを $\mathscr{S}_n$ で表します。

条件 a) プロップ。 3 (III、p. 30) は、双線形写像 $u : E \times F \to G$ が $\mathfrak{S}$ 次次連続であるためには、 $u$ の制限 $u_n : E_n \times F \to G$ がそれぞれ $\mathfrak{S}_n$ 次次連続であることが必要かつ十分であることを示しています。

### 4. 非連続双線形マッピングの拡大

#### 命題 7 {#evt-iii-s5-prop-7 .statement tag=07PK}

*$E, F, G$ *を 3 つの局所凸空間*、$G$ *ハウスドルフと仮定* します。 *$E_0$ *(それぞれ $F_0$) を * $E$ *(それぞれ $F$) の密なベクトル部分空間とします。 * $u$ *を* $E \times F$ *から* $G$への個別に連続する双線形写像とする。

1) *$u(E_0 \times F_0) = \{0\}$ の場合、*その後* $u = 0$。

2) *$\mathfrak{S}_0$ *$E_0$ の有界な部分集合の族とする。 *制限の* $u$ *から* $E_0 \times F_0$ *が* $\mathfrak{S}_0$*-非連続である場合、* $u$も同様です。

1) 仮定までに、すべての $x \in E_0$ について、連続線形写像 $u(x, .)$ は $F_0$ で null であるため、$F$ では null です。したがって、すべての $y \in F$ について、連続線形写像 $u(., y)$ は $E_0$ で null であるため、 $E$。これは$u = 0$であることを証明します。

2) $G$ の 0 の閉じた近傍 $W$ とすべての集合 $M \in \mathfrak{S}_0$ について、仮定までに $F_0$ の 0 の近傍 $V$ が存在し、$u(M \times V) \subset W$ になります。しかし、$\overline{V}$ は $F$ の 0 の近傍です。すべての $x \in M$、関係 $u(\{x\} \times V) \subset W$ は、$u(x, .)$ が連続で、$W$ が閉じているため、$u(\{x\} \times \overline{V}) \subset W$ を意味します。したがって、$u(M \times \overline{V}) \subset W$ は、$u$ が $\mathfrak{S}_0$* 準連続であることを証明します。

#### 命題 8 {#evt-iii-s5-prop-8 .statement tag=07PL}

*$E, F, G$ *局所的に 3 凸空間* とします。 *$G$ *はハウスドルフで準完全*であると仮定します。 *$E_0$ *(それぞれ $F_0$) を、* $E$ *(それぞれ $F$)、$\mathfrak{S}_0$ *(それぞれ $\mathfrak{T}_0$) の密集ベクトル部分空間とします* $E_0$ の境界のある部分集合 *(それぞれ $F_0$) * $E$ *(それぞれ $F$) のすべての点が * $\mathfrak{S}_0$ *(それぞれ $\mathfrak{T}_0$) の元のクロージャー内にあるようにします。次に、すべて* $(\mathfrak{S}_0, \mathfrak{T}_0)$*-非連続双線形マッピング* $u$ *from* $E_0 \times F_0$ *into* $G$ *拡大する個別連続双線形マッピング* $\overline{u}$ *from* $E \times F$ *into* $G$ *and* $\overline{u}$ *は* $(\mathfrak{S}_0, \mathfrak{T}_0)$*-低連続*です。

一意性と $\overline{u}$ の低連続性がプロップから続きます。 7; $\overline{u}$ の存在を証明することはまだ残っています。 $y' \in F_0$ ごとに、$E_0$ から $G$ 拡大するまでの連続線形写像 $x' \mapsto u(x', y')$ は、$E$ から $G$ までの連続線形写像 $x \mapsto u_1(x, y')$ (III、p. 8、小道具10）。すべての $x \in E$ について、$F_0$ から $G$ までの写像 $y' \mapsto u_1(x, y')$ は線形であることがすぐにわかります。そしてそれが連続的であることを示しましょう。 仮定までに$M \in \mathfrak{S}_0$が存在し、$x \in \overline{M}$になります。 $G$ の 0 の閉じた近傍 $W$ ごとに、仮定までに、$F_0$ の 0 の近傍 $V$ が存在し、そのような $u(M \times V) \subset W$; $x \mapsto u_1(x, y')$ は連続であるため、すべての $y' \in V$ に対して $u_1(\overline{M} \times V) \subset W$、特に $u_1(x, y') \in W$ が推定されます。これにより、主張が確立されます。プロップのおかげで。図 7 では、$E \times F_0$ から $G$ までの双線形写像 $u_1$ は $(\mathfrak{S}_0, \mathfrak{T}_0)$* 準連続です。 証明の最初の部分で$u_1$ に適用された$E$ と $F$ の役割は、交換することまでに証明を終了します。

### 5. 写像 $(u, v) \mapsto v \circ u$ の低連続性

#### 命題 9 {#evt-iii-s5-prop-9 .statement tag=07PM}

*$R, S, T$ *を局所的に 3 凸のハウスドルフ空間* とします。 *空間* $\mathscr{L}(R; S), \mathscr{L}(S; T), \mathscr{L}(R; T)$ * にそれぞれ単純* (それぞれ *コンパクト*、*有界*) 収束の位相が割り当てられているとします。 *その後、双線形写像* $(u, v) \mapsto v \circ u$ *from* $\mathscr{L}(R; S) \times \mathscr{L}(S; T)$ *into* $\mathscr{L}(R; T)$ *is* $(\mathfrak{S}, \mathfrak{T})$-*hypocontinuous*, *where* $\mathfrak{T}$ *は等連続の族部分集合 of* $\mathscr{L}(S; T)$, *and* $\mathfrak{S}$ *の族有限* (それぞれ *コンパクト、有界*) *部分集合/* $\mathscr{L}(R; S)$。

まず、$(u, v) \mapsto v \circ u$ が $\mathfrak{T}$ 非連続であることを証明します。 H を $\mathscr{L}(S; T)$ の等連続集合とし、W を T の 0 の近傍とし、M を R の有限 (それぞれコンパクト、有界) 部分集合とします。 S に 0 の近傍 V が存在し、$u(M) \subset V$ と $v \in H$ であれば $v(u(M)) \subset W$ となることを示さなければなりません。 しかし、このためには、すべての $v \in H$ に対して $v(V) \subset W$ があれば十分であり、そのような近傍の存在は H の等連続性から導き出されます。

$(u, v) \mapsto v \circ u$ が $\mathfrak{S}$ 非連続であることを確認するには、T の 0 のすべての近傍 W、R のすべての有限 (それぞれコンパクト、有界) 部分集合 M、および $\mathscr{L}(R; S)$ のすべての有限 (それぞれコンパクト、有界) 部分集合 L に対して、有限 (それぞれコンパクト、有界) 関係 $v(N) \subset W$ および $u \in L$ は $v(u(M)) \subset W$ を意味するような S の部分集合 N。 明らかに、L と M が存在するときはいつでも、$N = \bigcup_{u \in L} u(M)$、*つまり* 集合 N が有限 (それぞれコンパクト、有界) であることを示すだけで十分です。 L と M が有限である場合、または M が R で有界であり、L が $\mathscr{L}(R; S)$ で有界である場合、これは明らかになります (有界収束の位相の場合、*cf.* III、p. 22)。 最後に、コンパクト収束の位相に対して、MがRでコンパクトで、Lが$\mathscr{L}(R; S)$でコンパクトである場合、NはSでコンパクトであることを示します。 しかし、$u_M$ が $u \in L$ の M までの制限である場合、L から空間 $\mathscr{C}(M; S)$ までの写像 $u \mapsto u_M$ は、M から S までのすべての連続写像で一様収束の位相で連続です。したがって、この写像の下にあるLの像はコンパクトであり、次に主張は、$\mathscr{C}(M; S) \times M$からSへの写像$(w, x) \mapsto w(x)$の連続性から続きます（GT、X, § 1, No. 6、提案9）。

以下の 2 つの帰結では、prop のように仮定します。 9 では、空間 $\mathscr{L}(R; S)$、$\mathscr{L}(S; T)$、$\mathscr{L}(R; T)$ は、*3 つすべて* に単純収束の位相、またはコンパクト収束の 3 つすべて位相、または有界収束の 3 つすべてが割り当てられています。

#### 系 1 {#evt-iii-s5-prop-9-cor-1 .statement tag=07PN}

** $\mathscr{L}(S; T)$ *写像* $(u, v) \mapsto v \circ u$ *from* $\mathscr{L}(R; S) \times H$ *into* $\mathscr{L}(R; T)$ *の等連続部分集合 H は *連続*です。

これは prop の直後に続きます。 9 (III、p. 32) と 4 (III、p. 31)。

#### 系 2 {#evt-iii-s5-prop-9-cor-2 .statement tag=07PO}

※Sがバレルだと仮定します。 数列* $(u_n)$ *$\mathscr{L}(R; S)$ *および数列* $(v_n)$ *$\mathscr{L}(S, T)$ *に入る傾向がある場合、*その場合、数列* $(v_n \circ u_n)$ *$v \circ u$ *$\mathscr{L}(R; T)$ *になる傾向があります。

実際、数列 $(v_n)$ は、S がバレル化されているため (III, p. 25, th. 1)、$\mathscr{L}(S; T)$ で単純に境界付けられているため等連続です。 系は cor の帰結になります。 1.

### 練習問題 {#evt-iii-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
