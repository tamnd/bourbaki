---
book: ac
book_title: Commutative Algebra
chapter: VI
chapter_title: VALUATIONS
section: 4
section_title: The height of a valuation
lang: ja
source: ac-i-vii
book_pages: 393-399, 449-453
pdf_pages: 0411-0417, 0467-0471
extraction: ocr
subsections:
    - "no": 1
      title: INCLUSION OF VALUATION RINGS OF THE SAME FIELD
      page: 393
      pdf_page: 411
    - "no": 2
      title: ISOLATED SUBGROUPS OF AN ORDERED GROUP
      page: 394
      pdf_page: 412
    - "no": 3
      title: COMPARISON OF VALUATIONS
      page: 395
      pdf_page: 413
    - "no": 4
      title: THE HEIGHT OF A VALUATION
      page: 396
      pdf_page: 414
    - "no": 5
      title: VALUATIONS OF HEIGHT 1
      page: 397
      pdf_page: 415
statements: 18
exercises: 11
content_sha256: 7fe7592e4c743028968051bc8af54c7ec052484c66085491200d004252263d02
translated_from: content/en/ac/VI/04_s4_the_height_of_a_valuation.md
translation_method: google
source_content_sha256: c4cced628ead73d8a7f7dea6021c8771973779a0bf6c280142bacc5c87e4b329
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 3849a21551c0598584fe1309160acc7a8a7714e1a4cf49be329e62703623b9e8
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 4. 評価の高さ

### 1. 同じ体の評価環を含める

#### 命題 1 {#ac-vi-s4-prop-1 .statement tag=04TV}

*$K$を体、$A$を$K$の評価環とします。次に:*
(a) *$A \subset B \subset K$ が $K$ の評価環となるように、環 $B$ ごと。
(b) このような環の*最大イデアル$m(B)$は$A$に含まれており、それは$A$の素イデアルである。
(c) *写像 $\mathfrak{p} \mapsto A$ は、$A$ の素イデアの集合の減少する全単射を、$A \subset B \subset K$ となる環 $B$ の集合に重ねたものです。その逆全単射は写像$B \mapsto m(B)$です。

$B$ が $A \subset B \subset K$ と $x \in K - B$ である環である場合、$x \in K - A$、よって $x^{-1} \in m(A) \subset B$ となり、$B$ が $K$ の評価環であることと $m(B) \subset m(A)$ の両方を証明します。 $m(B) = m(B) \cap A$ は $A$ の主要な理想であるため、(a) と (b) を示しました。さらに、$A_{m(B)} \subset B$;逆に、$x \in B - A$ の場合は、$x^{-1} \in A$ と $x^{-1} \notin m(B)$、したがって $x \in A_{m(B)}$ になります。したがって$A_{m(B)} = B$。最後に、$\mathfrak{p}$ を $A$ の主要な理想とします。 $B = A_{\mathfrak{p}}$と書きます。それから$m(B) \cap A = \mathfrak{p}$。 (章 II, § 2, no. 5、命題 11) および $m(B) \subset A$ (b) による。したがって、$m(B) = \mathfrak{p}$ は、写像 $\mathfrak{p} \mapsto A$、および主張の $B \mapsto m(B)$ が逆全単射であることを示します。

#### 系 {#ac-vi-s4-n1-cor-1 .statement tag=04TW}

*K 含む A の集合と部分環は完全に包含によって順序付けされます。*

$A$ の素イデアルの集合は包含によって完全に順序付けされ ($\S$ 1、no. 2、定理 1 (e))、写像 $\mathfrak{p} \mapsto A_{\mathfrak{p}}$ は包含関係を反転します。

#### 命題 2 {#ac-vi-s4-prop-2 .statement tag=04TX}

*Kを体、BをKとhの評価環、Bに関連付けられた場所とK（$\kappa(B)$に値を含む）とする。 次に、マッピング $A \mapsto h_B(A)$ は、B に含まれる K の評価環の集合 $\mathscr{A}$ の、$\kappa(B)$ の評価環の集合 $\mathscr{A}'$ への全単射を定義します。

$A \in \mathscr{A}$ の場合、$h_B(A) \in \mathscr{A}'$: $x' = h_B(x)$ ($x \in B$) が $\kappa(B) - h_B(A)$ の元である場合、$x \notin A$、したがって $x^{-1} \in A$ と $h_B(x)^{-1} \in h_B(A)$ です。一方、$A \in \mathscr{A}$、$A \supset m(B)$ (命題 1 (b))、したがって写像については、

$A \mapsto h_B(A)$ は単射です。最後に、$A' \in \mathscr{A}'$ と $A = h_B(A') \subset B$ としましょう。 証明を完了する$A \in \mathscr{A}$ を示します。 $x \in K - A$ の場合は、$x \notin B$ または $x \in B$ のいずれかです。 $x \notin B$ の場合は $x^{-1} \in m(B) \subset A$; $x \in B$ の場合、$h_B(x) \in \kappa(B)$ と $h_B(x) \notin A$、したがって $h_B(x^{-1}) \in A$ となり、$x^{-1} \in A$ が再び結論するになります。したがって$A \in \mathscr{A}$です。

#### 系 {#ac-vi-s4-n1-cor-2 .statement tag=04TY}

*A と B を K の 2 つの評価環とし、$A \subset B$ とします。 $A' = h_B(A)$ とします。これは、$\kappa(B)$ の評価環です。 $A'$ の剰余体 $\kappa(A')$ は、A の剰余体 $\kappa(A)$ と標準的に同型であり、A に関連付けられた場所 $h_A$ は、A および B に関連付けられた場所の合成 $h_{A'} \circ h_B$ です。

局所環 $A'$ は局所環 $A$ の商であるため、それらの剰余体は正準同型であり、方程式 $h_A(x) = h_{A'}(h_B(x))$ は $x \in A$ にも当てはまります。一方、$x \in B - A$ の場合、$h_B(x) \notin A'$ となり、方程式の両辺は $\infty$ に等しくなります。 $x \in K - B$の場合も同様です。

#### 注意 {#ac-vi-s4-n1-rem-1 .statement tag=04TZ}

逆に、$K'$の値を含むKの場所を$f$、$K''$の値を含む$K'$の場所を$f'$とします。すると、$f' \circ f$は、$f$の場所の環に環が含まれるKの場所です。

### 2. 注文された群から部分群が分離されました

評価の観点から点から no. 1 の状況を研究するには、以下の定義 1 と命題 3 が必要になります。

#### 定義 1 {#ac-vi-s4-def-1 .statement tag=04U0}

* 関係 $0 \leq y \leq x$ と $x \in H$ が $y \in H$ を暗示する場合、順序付けられた群 G の部分群 H は孤立していると呼ばれます。

#### 例 (1) {#ac-vi-s4-n2-exa-1 .statement tag=04U1}

$A$ と $B$ を 2 つの順序群とします。 $A \times B$ に辞書編集上の位数を与えます (つまり、「$(a, b) \leq (a', b')$」は「$(a < a') \text{ or } (a = a' \text{ and } b \leq b')$」と同等です)。 $A \times B$ の 2 番目の因子 $B$ は、すぐにわかるように、$A \times B$ の孤立した部分群です。

#### 命題 3 {#ac-vi-s4-prop-3 .statement tag=04U2}

$G$ をその正の元の順序付けられた群と $P$ 集合とします。

(a) *増加する準同型の$G$ から順序群までの核は、$G$ の孤立した部分群です。

(b) *逆に、$H$ を $G$ の部分群と $G$ の $g$ 標準準同型を$G/H$ 上に分離したものとする。 この場合、$g(P)$ は、$G/H$ で注文された群構造の正の元の集合です。 さらに、$G$ が完全に順序付けされている場合、$G/H$ も完全に順序付けされています。*

(a) $f$ を $G$ から順序付けられた群までの増加する準同型とする。 $H$ を核オフとします。 $0 \leq y \leq x$と$x \in H$の場合、$0 \leq f(y) \leq f(x) = 0$、よって、$f(y) = 0$、つまり$y \in H$です。したがって、$H$ は孤立します。

(b) $H$ を、$G$ と $g : G \to G/H$ の孤立した部分群とします。 $P' = g(P)$ にしましょう。明らかに$P' + P' \subset P'$。また

$$
P' \cap (-P') = \{0\},
$$

*if* $x$ と $y$ が $P$ の元で、$g(x) = -g(y)$ となると、$H$ が孤立しているため、$x + y \in H$、よって $x \in H$、$y \in H$ になります。したがって$g(x) = g(y) = 0$です。したがって、$P'$ は、$G/H$ に順序付けられた群構造の正の元の集合です (*代数*、章 VI, § 1, no. 3、命題 3)。最後に、$G$ が完全に順序付けされている場合、$P \cap (-P) = G$、よって $P' \cup (-P') = G/H$、したがって $G/H$ は完全に順序付けされています (*loc. cit.*)。

#### 例 (2) {#ac-vi-s4-n2-exa-2 .statement tag=04U3}

$G$ が辞書編集的な積 $A \times B$ および $H = B$ である例を再考すると、順序付けられた群 $G/H$ は正規的に $A$ と識別されます。

### 3. 評価額の比較

$K$を体、$A$を$K$の評価環とします。 $K$ 含む $A$、$U(A) \subset U(B)$ の部分環 $B$ ごとに。 次に、$\Gamma_A = K^*/U(A)$ から $\Gamma_B = K^*/U(B)$ への正準準同型性 $\lambda$ があり、そのカーネルは $U(B)/U(A)$ です。 次に、$v_A$ と $v_B$ が、$A$ と $B$ (§ 3, no. 2) によって定義される $K$ の標準評価を表すとすると、

(1)

$$
v_B = \lambda \circ v_A.
$$

$A \subset B$、$\lambda$ 写像として、$\Gamma_A$ の正の元から $\Gamma_B$ の正の元なので、増加するとなります。したがって、(命題 3) $\lambda$ の核 $H$ は、$\Gamma_A$ と $\lambda$ 因子を $\Gamma_A \to \Gamma_A/H_B \xrightarrow{\mu} \Gamma_B$ に分離した部分群であり、$\mu$ は増加する全単射です準同型したがって、完全に注文された群の *同型* になります。したがって、$\Gamma_B$ は、完全に順序付けられた群 $\Gamma_A/H_B$ 商と識別されます。

#### 命題 4 {#ac-vi-s4-prop-4 .statement tag=04U4}

*写像* $B \mapsto H_B$ *は*の集合の部分環の増加する全単射 $K$ *含む* $A$ **の孤立した部分群の集合に$\Gamma_A$。

$H$ とすると、$v_B$ は同値まで定義されるため、$B$ は一意に決まります。一方、$H$ を $\Gamma_A$ の孤立した部分群とします。 $\Gamma_A / H$ を完全に順序付けされた群 (命題 3) として考慮すると、合成写像

$$
K^* \xrightarrow{v_A} \Gamma_A \longrightarrow \Gamma_A / H
$$

は $K$ の評価額で、その環含む $A$ です。

#### 注意 {#ac-vi-s4-n3-rem-1 .statement tag=04U5}

上記の仮説の下で、$f$ が $\kappa(B)$ と $A' = f(A)$ 上で $B$ の標準準同型を表すものとします。 $\kappa(B)$ (命題 2、no. 1) の評価額環です。それから$f^{-1}(\kappa(B)^*) = U(B), f^{-1}(A') = A, f^{-1}(m(A')) = m(A)$、したがって

$$
f^{-1}(U(A')) = U(A).
$$

次に、$U(B)/U(A)$の標準同型が$\kappa(B)^*/U(A') = \Gamma_{A'}$に続きます。 完全系列

$$
0 \to U(B)/U(A) \to \Gamma_A \to \Gamma_B \to 0
$$

次に完全系列を与えます

$$
0 \to \Gamma_{A'} \to \Gamma_A \to \Gamma_B \to 0.
$$

#### 例 {#ac-vi-s4-n3-exa-1 .statement tag=04U6}

$k$ を体とします。

$$
E = k(X) \quad \text{and} \quad K = k(X, Y) = E(Y)
$$

$(X, Y$ は不定)。 $B = E[Y]_{(Y)}$ を、主イデアル整域 $E[Y]$ の極値元 $Y$ (§ 1, no. 4、命題 3) によって定義される $K$ の評価環とします。 剰余体 $\kappa(B)$ は正規的に $E[Y]/(Y) = E$ と識別されます。同様に、$A' = k[X]_{(X)}$ を、$k[X]$ の極値元 $X$ によって定義される $E = k(X)$ の評価額環とします。 $B$に関連付けられた$E$の場所を$h$で表し、$A = h_B^{-1}(A')$と書くと、$B$と$\kappa(A) = \kappa(A') = k$に含まれる$K$の評価環$A$が定義されます。正規の位置 $h$: $K \to k$ は、次のように記述できます。 $(X, Y)$ が $K$ の元である場合、最初に $Y = 0$ inf (これにより、$\tilde{E} = k(X)^*$ の元が得られます)、次に、得られた結果に $X = 0$ を入れます。 群 $\Gamma_{A'}$ と $\Gamma_B$ は、正準的に $\mathbf{Z}$ (§ 3, no. 4、例 4) と同型です。 *群 $\Gamma_A$ が辞書編集上の積 $\mathbf{Z} \times \mathbf{Z}$ と同型であり、評価 $v_A$ が で定義された評価と同等であることを示すこと (cf. § 10, no. 2, 補題 2) は難しくありません。 § 3, no. 4、例の終わり 6.*

### 4. 評価の高さ

$G$ を完全に順序付けられた群とします。 $G$ の 2 つの孤立した部分群 $H$ と $H'$ が与えられると、そのうちの 1 つが位数に含まれます。そうでなければ、所属から $H'$ ではなく、$H$ の正の元 $x$ が存在するためです。 所属ではなく、$H'$ の元 $x'$ が H に。たとえば、$x \geq x'$ とします。 H が孤立しているため、$x' \in H$ となり、これは矛盾です。

これは、すべての全順序グループ​​が評価の順序グループ​​であるという事実を考慮して、no. 3 の命題 4 およびno. 1 の命題 1 の系からも導き出されます (§ 3, no. 4、例 6)。

#### 定義 2 {#ac-vi-s4-def-2 .statement tag=04U7}

*G を完全に順序付けられた群とします。 G とは異なる G の孤立した部分群の数が有限で n に等しい場合、G の高さは n であると言われます。この数が無限である場合、G は無限の高さであると言われます。*

例
(1) 群 $G = \{0\}$ の高さは 0 です。
(2) 群 $\mathbf{Z}$ と $\mathbf{R}$ は高さ 1 です。
(3) $G$ を完全に順序付けられた群とし、$H$ を $G$ の孤立した部分群とします。 $h(H)$ と $h(G/H)$ が完全に順序付けされた群 $H$ と $G/H$ の高さを表す場合、
$$
h(G) = h(H) + h(G/H),
$$
$G$ の孤立した部分群の集合は完全に包含によって順序付けされているためです。特に、$G$ が完全に順序付けされた 2 つの群 $H$ と $H'$ の辞書編集上の積である場合、
$$
h(G) = h(H) + h(H')
$$
(cf. no. 2、例 2);したがって、辞書編集上の積 $\mathbf{Z} \times \mathbf{Z}$ は高さ 2 です。

一方、$\mathbf{R}$ (cf. § 3, no. 4、例 6 の末尾) に埋め込むことで順序付けされた $\mathbf{Z} \times \mathbf{Z}$ の高さは 1 (以下の cf. 命題 8) に等しくなります。

#### 定義 3 {#ac-vi-s4-def-3 .statement tag=04U8}

*評価額の位数群の高さを、その評価額の高さと呼びます。*

たとえば、離散評価の高さは 1 です。不適切な評価のみが高さ 0 です。 命題 1 と 4 は次のことを意味します。

#### 命題 5 {#ac-vi-s4-prop-5 .statement tag=04U9}

*評価の高さは、環におけるゼロ以外の素数イデアルの数に等しい。

### 5. 高さの評価 1

#### 命題 6 {#ac-vi-s4-prop-6 .statement tag=04UA}

※$\mathbf{K}$を$\mathbf{K}$の体と$A$部分環とします。 $A$ が体ではないとします。したがって、次の条件は同等です:*
(a) $A$ は、$\mathbf{K}$ の高さ 1 の評価の環です。
(b) $A$ は $\mathbf{K}$ の評価環であり、$(O)$ と $m(A)$ 以外に主要な理想はありません。
(c) $A$ は、$\mathbf{K}$ とは異なる $\mathbf{K}$ の部分環の中で最大です。

no. 4 の命題 5 は (a) が (b) を意味することを示し、no. 1 の命題 1 は (b) が (c) を意味することを示します。 (c) が (a) を意味することを示すことはまだ残っています。 A が K とは異なる K の部分環の中で最大であるとします。 m を A の最大理想とし、A_m (§ 1, no. 2、系 ～ 定理 2) を支配する K の評価環をV とします。 m(V) ∩ A = m および m ≠ (0) (A が体ではないため)、V ≠ K、よって V = A として、A が K に対する評価 v の環ではないことが証明されます。 そうなると、v は命題 1 (no. 1) と 5 (no. 4) により高さ 1 になります。

#### 命題 7 {#ac-vi-s4-prop-7 .statement tag=04UB}

体の評価が高さ 1 になるためには、その位数群が \mathbf{R} の非ゼロ次数部分群と同型であることが必要かつ十分です。

これは実際には次の命題から導き出されます。

#### 命題 8 {#ac-vi-s4-prop-8 .statement tag=04UC}

G を O に還元されない完全に順序付けられた群とします。次の条件は同等です。
(a) G は高さ 1 です。
(b) G のすべての x > 0 および y ≥ 0 に対して、y ≤ nx となる整数 n ≥ 0 が存在します。
(c) G は、O に還元されない順序付けられた加法群 \mathbf{R} の部分群と同型です。

x を G の正の元とし、H を y ∈ G の集合とし、整数 n ≥ 0 満たす |y| が存在するようにします。 ≤ nx。 H, が G の孤立した部分群であり、G のすべての孤立した部分群が含む x 含む H, であることは簡単に検証されます。したがって、条件 (a) は「H, = G for all x > 0」、つまり条件 (b) と同等です。

明らかに (c) は (b) を意味します。逆に、条件 (b) が成り立ち、Q が G の元 >0 の集合を表すとします。まず、Q が最小の元 x を持つと仮定します。すべての y ∈ Q について、n を y ≤ nx となる最小の整数とする。 y < nx の場合、nx − y ≥ x、n の選択とは反対に、よって y ≤ (n − 1)x も成立します。 y = nx とすると、G = \mathbf{Z}x は \mathbf{Z} ⊂ \mathbf{R} と同型であることがわかります。ここで、Q に少なくとも元があると仮定します。一般位相、章 V, § 2 の順序付き集合 P = Q ∪ (0) 命題 1 に適用します (条件 (b) は単なる「アルキメデスの公理」であるため、これは可能です)。 \mathbf{R}_+ に対する P の真に増加する写像 f が存在することがわかります。

$$
f(x + y) = f(x) + f(y)
$$

x ∈ P および y ∈ P の場合。線形性により、 f は \mathbf{R} の部分群上で G の同型まで拡張でき、これは (b) が (c) を意味することを証明します。

#### 命題 9 {#ac-vi-s4-prop-9 .statement tag=04UD}

K を体、v を K および v の A 環に対する不適切でない評価とします。A が完全に積分的に閉じられる (章 V, § 1, no. 4, 定義 5) には、v が高さ 1 であることが必要かつ十分です。

v の高さが 1 であるとします。x ∈ K を、x^n (n ≥ 0) がすべて K の有限生成されたサブ A モジュールに含まれるようにします。すべての n ≥ 0 に対して dx^n ∈ A となるような d ∈ A − {0} が存在します。そのとき、v(d) + nv(x) ≥ 0、つまり n(−v(x)) ≤ v(d) となります。すべて $n \geqslant 0$、よって $-v(x) \leqslant 0$ (命題 8 (b)) および $x \in A$。したがって、A は完全に一体的に閉じられています。

ここで、v の高さが 1 ではないとします。そのとき、すべての $n \geqslant 0$ に対して $nv(y) < v(t)$ となるような $y \in m(A)$ と $t \in A$ が存在します (命題 8 (b))。次に、$n \geqslant 0$ はすべて $ty^{-n} \in A$ ですが、$y^{-1} \notin A$ になります。したがって、A は完全に積分的に閉じられていません。

#### 系 {#ac-vi-s4-n5-cor-1 .statement tag=04UE}

*K を、K の高さ 1 の評価群である体、$(v_\alpha)_{\alpha \in I}$ と、v の環の A 共通部分とします。* このとき、A は完全に積分的に閉じた領域です。

完全に積分的に閉じた領域は、高さ 1 (練習問題 6) の評価環の共通部分とは限りません。

### 練習問題 {#ac-vi-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
