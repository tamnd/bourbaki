---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 3
section_title: Faithfully flat modules
lang: ja
source: ac-i-vii
book_pages: 27-36, 49-50
pdf_pages: 0047-0056, 0069-0070
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF FAITHFULLY FLAT MODULES
      page: 27
      pdf_page: 47
    - "no": 2
      title: TENSOR PRODUCTS OF FAITHFULLY FLAT MODULES
      page: 30
      pdf_page: 50
    - "no": 3
      title: CHANGE OF RING
      page: 31
      pdf_page: 51
    - "no": 4
      title: RESTRICTION OF SCALARS
      page: 31
      pdf_page: 51
    - "no": 5
      title: FAITHFULLY FLAT RINGS
      page: 32
      pdf_page: 52
    - "no": 6
      title: FAITHFULLY FLAT RINGS AND FINITENESS CONDITIONS
      page: 34
      pdf_page: 54
    - "no": 7
      title: LINEAR EQUATIONS OVER A FAITHFULLY FLAT RING
      page: 35
      pdf_page: 55
statements: 18
exercises: 10
content_sha256: e94a082222dd3b912f0a9e6ff2113c407a56510b69d55b84865c613791745df3
translated_from: content/en/ac/I/03_s3_faithfully_flat_modules.md
translation_method: google
source_content_sha256: 0a1be9878f698d84733905bb7d0c759aa5a8adfb87dd8b4532795f408851fd36
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: ee54cccfff5d23a3f1c6fc738335c528b2ddffe565ae3cbcee820242d33e4fff
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 3. 忠実にフラット加群

### 1. 定義忠実にフラット加群

#### 命題 1 {#ac-i-s3-prop-1 .statement tag=0444}

$E$ を右側の $A$ モジュールとします。次の 4 つのプロパティは同等です。

(a) 左側の $A$ モジュールの数列 $N' \xrightarrow{v} N \xrightarrow{w} N''$ については、正確には、 数列であることが必要かつ十分です。
$$
E \otimes_A N' \xrightarrow{1 \otimes v} E \otimes_A N \xrightarrow{1 \otimes w} E \otimes_A N''
$$
正確に言ってください。

(b) $E$ はフラットで、左のすべての $A$-モジュール $N$ に対して、関係 $E \otimes_A N = 0$ は $N = 0$ を意味します。

(c) $E$ はフラットで、左側の $A$ モジュールの準同型 $v : N' \to N$ ごとに、関係 $1_E \otimes v = 0$ は $v = 0$ を意味します。

(d) $E$ は平坦で、左の最大理想値ごとに $A$、$E \neq Em$ の $m$ です。

記述を簡素化するために、左の $A$ モジュール $Q$ ごとに集合 $T(Q) = E \otimes_A Q$ を、左 $A$ モジュールのすべての準同型 $v$ に $T(v) = 1_E \otimes v$ を入力します。

(a)、(b)、(c) の同値をまず証明します。

(a) が (b) を意味することを証明します。 (a) が成り立つ場合、明らかに $E$ はフラット (§ 2, no. 3、命題 1) です。一方、$N$ を $T(N) = 0$ のような左 $A$ 加群とし、数列 $0 \to N \to 0$ を考慮します。 仮定 $T(N) = 0$ は、数列 $0 \to T(N) \to 0$ が正確であることを意味します。 (a) 数列 $0 \to N \to 0$ は正確です、よって $N = 0$。

(b) が (c) を意味することを示します。 (b) が成立し、$u : N' \to N$ を準同型とし、$I$ を像とします。 $T(v)$ の像は $T(I)$ (§ 2, no. 3、注意 2) と同一視されるため、仮定 $T(v) = 0$ は $T(I) = 0$ を暗示し、よって (b) により $I = 0$ が、その結果 $v = 0$ になります。

(c) が (a) を意味することを示します。次に、(c) が成り立つとして、数列を考えます。
$$
N' \xrightarrow{v} N \xrightarrow{w} N''
$$
左側の $A$ モジュールの準同型と対応する数列
$$
T(N') \xrightarrow{T(v)} T(N) \xrightarrow{T(w)} T(N'').
$$

数列 (1) が正確であれば、$E$ はフラット (§ 2, no. 3, 命題 1) であるため、(2) も正確です。逆に、(2) が正確であれば、最初に $T(w \circ v) = T(w) \circ T(v) = 0$ があり、したがって仮定によって $w \circ v = 0$ が得られます。 集合 $I = v(N')$ と $K = \overline{w}(0)$;上記により$I$は$K$に含まれます。 完全系列を検討してください
$$
0 \to I \xrightarrow{i} K \xrightarrow{p} K/I \to 0
$$
$i$ と $p$ は標準写像です。 $E$はフラットなので、数列
$$
0 \to T(I) \xrightarrow{T(i)} T(K) \xrightarrow{T(p)} T(K/I) \to 0
$$
他の語では、$T(I)$ (それぞれ $T(K)$) は $T(v)$ の像 (それぞれ核) と同一視されるため、$T(K/I)$ は仮定によって 0 である $T(K)/T(I)$ と同型です。 $T(w)$) (§ 2, no. 3、注意 2)。しかし、関係 $T(p) = 0$ は仮定によって $p = 0$ を意味するため、$K = I$ となり、数列 (1) が正確であることが証明されます。

最後に(b)と(d)の同値を示します。 (b) が成立する場合、

$$
E/E_m = E \otimes_A (A_s/m) \neq 0
$$

$A_s/m \neq 0$以来。 よって (d)。逆に、(d) が成り立つと仮定します。 $A$ のすべての左イデアル $a \neq A$ は、最大左イデアル $m$ (*代数*, 章 I, §8, no. 7, 定理 2) に含まれており、その場合、仮定 $E \neq Em$ は $E \neq Ea$ を暗示します。 語、$E \otimes_A (A_s/a) \neq 0$。つまり、すべての *単一* 左 $A$-モジュール $N \neq 0$、$T(N) \neq 0$ に対して。ここで、$N$ が左の $A$-モジュール \#0 である場合、それは含むは単一の部分加群 $N' \neq 0$ です。 $E$ はフラットなので、$T(N')$ は $T(N)$ の部分群と識別されます。 $T(N') \neq 0$ を見たので、$T(N) \neq 0$ になります。

#### 定義 1 {#ac-i-s3-def-1 .statement tag=0445}

*右 $A$-モジュール* $E$ *命題 1 の 4 つの同等の条件を満たす場合、忠実にフラットと呼ばれます。*

忠実にフラットな左 $A$ モジュールも同様に定義されます。明らかに、左側の $A$ モジュール $E$ が忠実に平坦であるためには、右側の $A^0$ モジュールとみなされる $E$ が忠実に平坦であることが必要かつ十分です。

#### 注意 {#ac-i-s3-n1-rem-1 .statement tag=0446}

$E$ が忠実にフラットな $A$ モジュールである場合、$E$ は *忠実* $A$ モジュールです。つまり、元 $a \in A$ がすべての $x \in E$、ホモテティー に対して $xa = 0$ である場合、 $A$ の $h : b \mapsto ba$ は $1, \otimes h = 0$ になります。 命題 1 の性質 (c) によるよって $h = 0$、つまり、$A$ には単位元があるため、$a = 0$ になります。

*例*
(1) フラット加群と忠実にフラット加群の直和は、命題 1 と § 2, no. 3、命題 2 の性質 (d) のおかげで、忠実にフラット加群になります。
(2) *$A$* は、命題 1 および § 2, no. 4、*例* 1 の基準 (d) により忠実にフラットであるため、(1) から、すべての自由加群 *0 に減らされない* は忠実にフラットであることがわかります。一方、自由加群の非ゼロ直因子（他の語、非ゼロ射影加群）も存在します。これらは忠実ではありますが、忠実にフラットではありません（練習問題 2）。
(3) $A$ を *主イデアル整域* とします。 $A$ モジュール $E$ が忠実に平坦であるためには、$A$ のすべての既約元 (*代数*、章 VII, § 1, no. 3) $p$ について *ねじれがない* および $E \neq Ep$ であることが必要かつ十分です。これは、§ 2, no. 4、命題 3 および命題 1 の基準 (d) からすぐに続きます。
(4) 例 (3) は、$\mathbf{Z}$ モジュール $\mathbf{Q}$ がフラットで忠実な加群ですが、*忠実にフラットではない* ことを示しています。

#### 命題 2 {#ac-i-s3-prop-2 .statement tag=0447}

*$E$ を忠実に平坦な右 $A$ モジュール、$u : N' \to N$ を左 $A$ モジュール準同型とします。 $u$ が単射（それぞれ全単射、全単射）であるためには、$1_E \otimes u : E \otimes_A N' \to E \otimes_A N$ がそうであることが必要かつ十分です。*

これは、命題 1 の基準 (a) の明らか帰結です。

#### 命題 3 {#ac-i-s3-prop-3 .statement tag=0448}

$0 \to E' \to E \to E'' \to +0$ を右側の $A$ モジュールの完全系列とします。 $E'$ と $E''$ がフラットで、そのうちの 1 つが忠実にフラットであると仮定します。すると$E$は忠実にフラットになります。

$E$ がフラット ($§ 2$、no. 5、命題 5) であることはすでにわかっています。 $E$ が命題 1 の性質 (b) を持っていることを確認します。$N$ を左の $A$ 加群としましょう。 $E''$は平坦なので完全系列もございます

$$
0 \to E' \otimes_A N \to E \otimes_A N \to E'' \otimes_A N \to 0
$$

($§ 2$、no. 5、命題 4)。 $E \otimes_A N = 0$ の場合、$E' \otimes_A N$ と $E'' \otimes_A N$ は零になります。 加群 $E'$、$E''$ の 1 つが忠実にフラットであるため、これは $N = 0$ を意味します。

### 2. 忠実にフラットな加群のテンソル積

#### 命題 4 {#ac-i-s3-prop-4 .statement tag=0449}

$R, S$ を 2 つの環、$E$ を右 $R$ モジュール、$F$ を $(R, S)$ バイモジュールとします。 $E$ が忠実にフラットであると仮定します。次に、$F$ がフラットな (つまり忠実にフラットな) $S$ モジュールであるためには、$E \otimes_R F$ がそうであることが必要かつ十分です。

(1) $F$ がフラットの場合、$E \otimes_R F$ はフラットになります ($§ 2$、no. 7、命題 8)。

(2) $E \otimes_R F$ が平坦であると仮定し、$\nu : N' \to N$ を単射左 $S$ 加群準同型とします。 準同型

$$
l_E \otimes l_F \otimes \nu : E \otimes_R F \otimes_S N' \to E \otimes_R F \otimes_S N
$$

この場合、 は単射法になります ($§ 2$, no. 3, 命題 1)。 no. 1 の命題 2 から、$l_F \otimes \nu : F \otimes_S N' \to F \otimes_S N$ は単射であることがわかります。この場合、$F$ はフラットな $S$ モジュール ($§ 2$、no. 3、命題 1) です。

(3) $F$ が忠実に平坦であると仮定し、$N$ を $E \otimes_R F \otimes_S N = 0$ のような左 $S$ 加群とする。 $E$ は忠実にフラットであるため、$F$ が忠実にフラットであるため、これは $F \otimes_S N = 0$、よって $N = 0$ を意味します。これは、$E \otimes_R F$ が忠実にフラットであることを証明しています。

(4) $E \otimes_R F$ が忠実に平坦であると仮定し、$N$ を $F \otimes_S N = 0$ のような左 $S$ 加群とする。次に、$E \otimes_R F \otimes_S N = 0$、よって $N = 0$ は、$F$ が忠実にフラットであることを示しています。

#### 系 {#ac-i-s3-n2-cor-1 .statement tag=044A}

$C$ を 2 つの忠実にフラットな $C$ モジュールである可換環と $E$ および $F$ とします。次に、$C$ モジュール $E \otimes_C F$ は忠実にフラットになります。

$R = S = C$で命題を適用する 4。

### 3. 変更/環

#### 命題 5 {#ac-i-s3-prop-5 .statement tag=044B}

$\rho$ を環 $A$ から環 $B$ までの準同型とします。 $E$ が忠実にフラットな右 $A$ モジュールである場合、右 $B$ モジュール $\rho^*(E) = E_{(B)} = E \otimes_A B$ は忠実にフラットです。

命題を適用する 4 の no. 2 と $R = A, S = F = B$ は、$B$ モジュール $B_d$ が忠実にフラットであることに注目します。

#### 系 {#ac-i-s3-n3-cor-1 .statement tag=044C}

*$E$ が忠実に平坦な右 $A$ モジュールであり、$a$ が $A$ の両側理想である場合、右 $(A/a)$ モジュール $E/Ea$ は忠実に平坦です。

命題を適用する 5 で、$B = A/a, \rho$ は標準準同型です。

#### 命題 6 {#ac-i-s3-prop-6 .statement tag=044D}

$A$を$A$から$B$の$A$と$\rho : a \mapsto a . 1$標準準同型を可換環、$B$代数とします。 $B$ が忠実にフラットな $A$ モジュールであると仮定します。次に、$A$ モジュール $E$ が平坦 (それぞれ忠実に平坦) であるためには、右側の $B$ モジュール $E_{(B)} = E \otimes_A B$ が平坦 (それぞれ忠実に平坦) であることが必要かつ十分です。

(1) $E$ がフラット (または忠実にフラット) の場合、$E_{(B)}$ は § 2, no. 7、系 2 ～ 命題 8 (それぞれ命題 5) だけフラット (または忠実にフラット) になります。

(2) $E_{(B)}$ が平坦であると仮定し、$\nu : N' \to N$ を単射加群 $A$ 加群準同型とします。 § 2, no. 7、系 3 により、$A$ 加群 $E \otimes_A B$ はフラットであるため、準同型 $1, \otimes 1_B \otimes \nu : E \otimes_A B \otimes_A N' \to E \otimes_A B \otimes_A N$ は単射的です。 $B$ 一致するの左右の $A$ モジュール構造として、この準同型は次のように識別されます。

$$
1_E \otimes \nu \otimes 1_B : E \otimes_A N' \otimes_A B \to E \otimes_A N \otimes_A B.
$$

$B$ は忠実に平坦な $A$ 加群であるため、$1_E \otimes \nu : E \otimes_A N' \to E \otimes_A N$ は単射 (no. 1、命題 2) であることがわかり、$E$ が平坦であることがわかります。

(3) 最後に、$E_{(B)}$ が忠実に平坦であると仮定します。 まず$E$は(2)でフラットになります。 また、$N$ を $E \otimes_A N = 0$ のような $A$ モジュールとする。 次に、$B$ 一致する、$E \otimes_A B \otimes_A N = 0$ の左右の $A$ モジュール構造から、$E \otimes_A N \otimes_A B = 0$、よってとなり、$(E \otimes_A B) \otimes_B (B \otimes_A N) = 0$ と書くこともできます。 $E_{(B)}$ は忠実にフラットな $B$ モジュールであるため、これは、$B$ が忠実にフラットな $A$ モジュール (no. 1、命題) であるため、$B \otimes_A N = 0$ (no. 1、命題 1)、よって $N = 0$ を意味します。 1)。

### 4. スカラーの制限

#### 命題 7 {#ac-i-s3-prop-7 .statement tag=044E}

※$A$～$B$の環と$\rho$準同型を$A, B$とします。 $E$ を忠実に平坦な右$B$ モジュールとします。 $\rho^*(E)$ がフラット (または忠実にフラット) 右 $A$ モジュールであるためには、$B$ がフラット (または忠実にフラット) 右 $A$ モジュールであることが必要かつ十分です。*

適用命題 no. 2 の 4 で、$R, S, E, F$ の代わりに $B, A, E, B$ がそれぞれ含まれており、$B$ の右側の $A$ モジュール構造が $\rho$ によって定義されていることがわかります。

$E \otimes_B B = \rho^*(E)$ がフラット (または忠実にフラット) A-加群である場合に限り、B はフラット (または忠実にフラット) A-加群です。

注意
(1) 命題 7 は、B が忠実にフラット A-加群であるためには、忠実にフラット A-加群でもある 1 つの忠実にフラット B-加群が存在するだけで十分であることを示しています。
(2) A、B、C を 3 つ環とし、$\rho : A \to B, \sigma : B \to C$ を 2 つ環準同型とします。 命題 7 は、C が忠実にフラット B-加群で、B が忠実にフラット A-加群である場合、C は忠実にフラット A-加群であることを示しています。 C が忠実なフラット B-加群と忠実なフラット A-加群である場合、B は忠実なフラット A-加群です (アイデアを修正するために、加群を正しい加群として扱います)。一方、B と C は、C が忠実にフラット B-加群 (練習問題 7) でなくても、忠実にフラット A-加群になる可能性があります。

### 5. 忠実にフラット環

#### 命題 8 {#ac-i-s3-prop-8 .statement tag=044F}

A、B を A から B までの 2 つの環と $\rho$ 準同型とします。$\rho_*(E)$ が忠実に平坦な A-加群となるような右B-加群 E が存在するとします。次に:
(i) すべての左A-加群 F に対して、標準準同型 $j : F \to F_{(B)} = B \otimes_A F$ (すべての $x \in F$ に対して $j(x) = 1 \otimes x$ となるように) は単射的です。
(ii) A の左イデアル a ごとに、$\overline{\rho}^{-1}(Ba) = a$。
(iii) 準同型 $\rho$ は単射です。
(iv) A のすべての最大左イデアル m に対して、$\overline{\rho}^{-1}(n) = m$ のような B の最大左イデアル n が存在します。

(i) を証明します。私たちは (代数、章 11、§ 5, no. 2、系 ～ 命題 5)、すべての右B-加群 M に対して、$i(y) = y \otimes 1$ によって定義される正準 A 準同型性 $i : M \to \rho_*(M) \otimes_A B = \rho^*(\rho_*(M))$ が単射であり、A-加群 $i(M)$ が$\rho_*(M) \otimes_A B$の直因子。したがって、左A-加群 F ごとに、

$$
i \otimes 1_F : \rho_*(M) \otimes_A F \to \rho_*(M) \otimes_A B \otimes_A F
$$

は単射法です (§ 2, no. 1, 補題 2)。 $M = E$ を取ると、($i \otimes 1_F = 1_M \otimes j$ 以来) $j$ は単射法 (no. 1, 命題 2) であることがわかります。

主張 (ii) は、(i) から $F = A_s/a$ を取り、(iii) は (ii) から $a = \{0\}$ を取り、続きます。

最後に、m が A の最大左イデアルである場合、(ii) により $\overline{\rho}^{-1}(Bm) = m$ となり、結果として $Bm \# B$ となります。このとき、B 含む Bm (代数, 章 I, § 8, no. 7, 定理 2) の最大左イデアル n が存在します。次に$m \subset \overline{\rho}^{-1}(n)$、$\rho(1) \notin n$、$1 \notin \overline{\rho}^{-1}(n)$となります。結果として$\overline{\rho}^{-1}(n) = m$。

$A$ と $B$ 満たす条件の命題 8 の場合、$A$ は通常、$\rho$ によって $B$ の部分環と識別されます。

#### 系 {#ac-i-s3-n5-cor-1 .statement tag=044G}

命題 8 の仮説の下では、$B$ が左ネーター (それぞれアルティン) である場合、$A$ も同様です。

(a) が$A$ の左イデアルの非定常増加 (または減少) シーケンスである場合、$B$ のイデアルのシーケンス $(\mathrm{Ba}_n)$ は仮説に反して、$\rho^{-1}(\mathrm{Ba}_n) = a_n$ 以降非定常で増加 (それぞれ減少) しています。

*注意 (1)。 $A$ と $B$ が可換である場合、章 II, § 2, no. 5、系 4 から命題 11 で、命題 8 の仮定は、すべての素イデアルについて $p$ を意味することがわかります。 $A$、$\rho^{-1}(q) = p$ となるような$B$ の主理想$q$ が存在します ($A$ が $B$ の部分環と同一視される場合の $p = A \cap q$)*。

命題 8 の重要な応用は、$B$ 自体が忠実にフラットな $A$ モジュールである場合です。ただし、この場合、次のより正確な命題が得られます。

#### 命題 9 {#ac-i-s3-prop-9 .statement tag=044H}

$A, B$を$A$から$B$の2つの環と$\rho$準同型とします。次の 5 つのプロパティは同等です。
(a) 右側の$A$-モジュール$B$ は忠実に平坦です。
(b) 準同型 $\rho$ は単射であり、右側の $A$ 加群 $B/\rho(A)$ はフラットです。
(c) 右側の $A$ モジュール $B$ はフラットで、左側の $A$ モジュール $F$ ごとに、$F$ ～ $B @ * F$ の標準準同型 $x \mapsto 1 @ x$ は単射です。
(d) 右側の$A$モジュール$B$は平坦で、左側の$A$、$\rho^{-1}(\mathrm{Ba}) = a$の各理想$a$に対して。
(e) 右$A$加群$B$は平坦であり、$A$の最大左イデアル$m$ごとに、$\rho^{-1}(n) = m$となるような$B$の最大左イデアル$n$が存在します。

命題 8 により、(a) はそれぞれのプロパティ (c)、(d)、(e) を意味します。一方、(e) が成り立つ場合、$A$ のすべての最大左理想値 $m$ に対して $Bm \# B$ ($Bm \subset n$ となるような $B$ の最大左理想値 $n$ が存在するため)、$B$ は次のとおり忠実に平坦な $A$ 加群になります。基準 (d) 命題 1 of no. 1;したがって、(e) は (a) を意味します。

これから、(c) $\Rightarrow$ (d) $\Rightarrow$ (b) $\Rightarrow$ (a) を証明して、証明を完成させます。そもそも、(c) の$F = A_s/a$ を取ることで、(c) は (d) を暗示します。 (d) が成り立つ場合、$a = \{0\}$ を取ると、$\rho$ が単射法であることがわかります。 (d) および § 2, no. 6、系から命題 7 は、$B/\rho(A)$ が平坦な右 $A$ モジュールであることを意味します。つまり、(d) は (b) を意味します。最後に、(b) が成立する場合、no. 1 の 3 つである命題が完全系列に適用されます。

$$
0 \longrightarrow A_a \xrightarrow{\rho} B \longrightarrow B/\rho(A) \longrightarrow 0
$$

$A_a$ が忠実にフラットであるため、$B$ が忠実にフラットな右 $A$ モジュールであることを示しています。

*注意 (2)。 $A$ と $B$ が可換である場合、章 II, § 2 no. 5、系 4 から命題 11 で、命題 9 の条件が以下と同等であることがわかります。

(f) B *はフラット A-加群であり、すべての素イデアル* $\mathfrak{p}$ *of* $A$ に対して、*イデアル* $q$ *of* $B$ *そのような* $\bar{\rho}^{-1}(q) = \mathfrak{p}$ が存在します。

命題 9 の条件では、$\mathfrak{p}$ を使用して $B$ の *部分環* を使用して同一視する $A$ とします。 関係 $\bar{\rho}^{-1}(Ba) = a$ は $A \cap Ba = a$ となります。一方、$F$ が左の $A$ モジュールである場合、$F$ は標準写像 $x \mapsto 1 @ x$ の下の $B \otimes_A F$ にあるその像と識別されます。 $X$ が $F$ の加法部分群である場合、$X$ によって生成された $B \otimes_A F$ の左サブ B モジュールを $BX$ で表します。この記法により、次のようになります。

#### 命題 10 {#ac-i-s3-prop-10 .statement tag=044I}

*$B$ *を環とし、* $A$ *部分環を* $B$ *として* $B$ *は忠実に平らな右* $A$-*加群とします。 * $F$ *左* $A$-*加群、$F', F''$ * $F$ の *2 つの部分加群とします。 *その後:*
(i) *標準写像* $B \otimes_A F' \to B \otimes_A F$ *は $B \otimes_A F'$ の同型です* $BF'$ です。
(ii) $F \cap BF' = F'$。
(iii) $B(F' + F'') = BF' + BF''$。
(iv) $B(F' \cap F'') = BF' \cap BF''$。

$B$ は平らな右 $A$ モジュールであるため、標準写像
$$
B \otimes_A F' \to B \otimes_A F
$$
は単射です。行われた識別を考慮すると、その像は $BF'$ となり、(i) が証明されます。 主張 (ii) は、§ 2, no. 6、命題 7 から$E = B$、$E' = A$ を適用し、式 $A \otimes_A F = F$ および $A \otimes_A F' = F'$ を使用して計算されます。 主張 (iii) は自明であり、(iv) は § 2, no. 6、命題 6 から続きます。

### 6. 忠実にフラット環と有限性条件

#### 命題 11 {#ac-i-s3-prop-11 .statement tag=044J}

*$B$ *を環とし、* $B$ の* $A$ *部分環を * $B$ * 忠実に平坦な右* $A$-*加群とする。左* $A$-*加群* $F$ *が確実に生成される(それぞれ有限に提示される)には、* $B$-*加群* $B \otimes_A F$ *が有限に生成される(それぞれ有限に提示される)ことが必要かつ十分です。*

(1) $B$ に仮定がなければ、明らかに、$F$ が有限生成された左 $A$ 加群である場合、$B \otimes_A F$ は有限生成された左 $B$ 加群です。逆に、$B \otimes_A F$ が有限生成された $B$ モジュールである場合、形 $1 \otimes x_i$ と $x_i \in F$ の有限数の元によって生成されます。 $M$ が $x_i$ と $j$ 標準単射 $M \to F$ によって生成される $F$ のサブモジュールである場合、$1, \otimes j : B \otimes_A M \to B \otimes_A F$ は全射準同型であるため、$j$ は全射 (no. 1, 命題 2)、これは、$F$ が有限に生成されることを証明します。

(2) *もし* $F$ *有限の表現を認める* $B \otimes_A F$ *B (§ 2, no. 8) に仮定* がなければ* となります。 $B \otimes_A F$ が有限表現を認める場合、F も有限表現であることを証明する必要があります。(1) から、F が有限生成されることはすでにわかっています。従って、全射準同型 $u : L \to F$ が存在します。ここで、L は有限生成された自由A-加群です。 R を u の核とすると、$B \otimes_A R$ は全射準同型 $l_B \otimes u : B \otimes_A L \to B \otimes_A F$ (§ 2, no. 3, *注意 2*) の核と識別されます。 $B \otimes_A F$ は仮定による有限の提示を認めるので、結論する (§ 2, no. 8, 補題 9) は $B \otimes_A R$ が有限に生成されることになります。次に、(1) から R は有限生成A-加群であることがわかり、その結果 F は有限表現を認めます。

#### 命題 12 {#ac-i-s3-prop-12 .statement tag=044K}

*B を環とし、A を B の中心の可換部分環とし、B を忠実に平坦な A-加群とします。 A-加群 F が射影で有限生成されるためには、$B \otimes_A F$ が有限生成射影左B-加群であることが必要かつ十分です。*

条件は、A または B に仮定がなくても明らかに必要です (*代数*、章 II, § 5, no. 1、系から命題 4)。私たちはそれで十分であることを証明します。 有限生成射影加群が有限表現 (§ 2, no. 8、補題 8) を認める場合、仮定は、F が命題 11 によって有限表現を認めることを意味します。従って、A-加群 M ごとに、標準同型が存在します。

$$
\omega : B \otimes_A \operatorname{Hom}_A(F, M) \to \operatorname{Hom}_B(B \otimes_A F, B \otimes_A M)
$$

(§ 2, no. 10、命題 11)。次に、$v : M \to M''$ を*全射法* A-加群準同型とし、可換論である図式を考えます。

$$
\begin{array}{ccc}
B \otimes_A \operatorname{Hom}_A(F, M) & \xrightarrow{\omega} & \operatorname{Hom}_B(B \otimes_A F, B \otimes_A M) \\
1_B \otimes \operatorname{Hom}(1_F, v) \downarrow & & \downarrow \operatorname{Hom}(1_B \otimes F, 1_B \otimes v) \\
B \otimes_A \operatorname{Hom}_A(F, M'') & \xrightarrow{\omega} & \operatorname{Hom}_B(B \otimes_A F, B \otimes_A M'')
\end{array}
$$

$1_B \otimes v$ は全射であり、$B \otimes_A F$ は射影であると想定されているため、$\operatorname{Hom}(1_{B \otimes F}, 1_B \otimes v)$ は *全射* (*代数*、章 II, § 2, no. 2、命題 4)、従って $1_B \otimes \operatorname{Hom}(1_F, v)$ となります。しかし、B は忠実に平坦な A-加群であるため、$\operatorname{Hom}(1_F, v)$ はそれ自体全射法 (no. 1, 命題 2) であるため、F は射影法 A-加群 (*代数*, 章 II, § 2, no. 2, 命題 4) です。

### 7. 忠実に平坦な環上の線形方程式

B を B の環および A 部分環とします。次の条件を満たす場合、順序付けされた対 (A, B) は *線形拡大性質* を持つと言えます。

(E) 線形方程式の各解 $(y_k)_{1 \leq k \leq n}$、からなる、元、$B$、系

$$
\sum_{k=1}^n y_k c_{ki} = d_i \quad (1 \leq i \leq m)
$$

係数 $c_{ki}$ と右辺 $d_i$ 属するから $A$ は形です

$$
y_k = x_k + \sum_{j=1}^p b_j z_{jk} \quad (1 \leq k \leq n)
$$

ここで、$(x_k)$ は $A$ の要素からなる (3) の解であり、$b_j$ は $B$ に属し、それぞれの $(z_{jk})_{1 \leq k \leq n}$ は、$A$ の要素からなる (3) に関連付けられた等次線形システムの解です。

#### 命題 13 {#ac-i-s3-prop-13 .statement tag=044L}

$A$ を環 $B$ の部分環とします。順序付けされた対 $(A, B)$ から満たすの線形拡大性質では、$B$ が忠実に平坦な $A$ モジュールであることが必要かつ十分です。

条件で * 十分 * です。なぜなら、$B$ は平坦な$A$ 加群であるため、(3) に関連付けられた*均質* 線形系の$B$ にある元を持つすべての解は、解の $B$ にある係数を持つ線形結合です。 からなる/元/$A$ (§ 2, no. 11、系 2、命題 13 まで)。 問題から簡約するから証明とすると、$B$ の元を伴う (3) の解の存在は、$A$ の元を伴う *1 つの* 解の存在を意味します。今、私たちが集合だったら

$$
c_k = (c_{ki})_{1 \leq i \leq m} \in A_s^m, \qquad d = (d_i) \in A_s^m,
$$

系 (3) は方程式 $\sum_{k=1}^n y_k \otimes c_k = 1 \otimes \mathrm{din}\, B \otimes_A A_s^m = B_s^m$ と等価です。

In other words, if $M$ is the sub-$A$-module of $A_s^m$ generated by the $c_k$ $(1 \leq k \leq n)$, the existence of the solution $(y_k)$ of (3) is equivalent (with the identifications made in no. 5) to the relation $d \in BM \cap A_s^m$; but as $BM \cap A_s^m = M$ (no. 5, Proposition 10, (ii)), it implies $d \in M$, that is, the existence of a solution $(x_k)$ of system (3) with elements in $A$.

条件は*必須*です。 $(A, B)$ が線形拡大性質を満たすと仮定します。 $B$ は平らな右 $A$ モジュール (§ 2, no. 11、系 2 ～ 命題 13) であることはすでにわかっています。 $A$、$Ba \cap A = a$ のすべての左イデアル $a$ について、$B$ が忠実に平坦な右 $A$ 加群 (no. 5、命題 9、(d)) であることを示します。さて、$x \in Ba \cap A$ としましょう。 $\sum_i y_i a_i = x$ となるような仮定 $y_i \in B$ と $a_i \in a$ が存在します。 性質 (E) を係数と$A$ の右辺でこの一次方程式に適用すると、$x = \sum_i x_i a_i$ となるような $x_i \in A$ が存在することがわかり、したがって $x \in a$ になります。

### 練習問題 {#ac-i-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
