---
book: ac
book_title: Commutative Algebra
chapter: V
chapter_title: INTEGERS
section: 2
section_title: The lift of prime ideals
lang: ja
source: ac-i-vii
book_pages: 325-344, 362-369
pdf_pages: 0344-0363, 0381-0388
extraction: ocr
subsections:
    - "no": 1
      title: THE FIRST EXISTENCE THEOREM
      page: 325
      pdf_page: 344
    - "no": 2
      title: DECOMPOSITION GROUP AND INERTIA GROUP
      page: 330
      pdf_page: 349
    - "no": 3
      title: DECOMPOSITION AND INERTIA FOR INTEGRALLY CLOSED DOMAINS
      page: 337
      pdf_page: 356
    - "no": 4
      title: THE SECOND EXISTENCE THEOREM
      page: 343
      pdf_page: 362
statements: 36
exercises: 22
content_sha256: fb7437053723a32200b40fe36b94a9a025e1e187b841d74608d8659bf640a685
translated_from: content/en/ac/V/02_s2_the_lift_of_prime_ideals.md
translation_method: google
source_content_sha256: 89a50149d078678d4ea98a688a9a6bd071b42b62e0d62c0a7d340a9d004553ca
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: e2a6ed373afbf85f43cab20e44e55eb2426a34722ee620eebc379e31551d2b80
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 2. 挙上の主要な理想

### 1. 最初の存在定理

#### 定義 1 {#ac-v-s2-def-1 .statement tag=04PJ}

$\mathbf{A}, \mathbf{A}'$ を 2 つの環と $h : \mathbf{A} \to \mathbf{A}'$ 環準同型とします。理想$a' \in A'$は、$a = \overline{h}^1(a')$であれば$\mathbf{A}$の理想$a$の上にあると言われます。

したがって、$A'$ の素理想 $p'$ が $\mathbf{A}$ の理想 $p$ の上にあるということは、$h$ に関連付けられた連続写像 「$h : \mathrm{Spec}(A') \to \mathrm{Spec}(A)$」の下で、$p$ が $p'$ の像であることを意味します。 (章 11、§ 4, no. 3)。

$\mathbf{A}$ の理想 $(0)$ の上に$A'$ の理想が存在するには、$h : \mathbf{A} \to \mathbf{A}'$ が単射であることが必要かつ十分であることに注意してください。

$a$ を $\mathbf{A}$ の理想とします。 商準同型 $h$ を取ると、準同型 $h_1 : \mathbf{A}/a \to \mathbf{A}'/a'$ が得られます。 $a'$ は $a$ の上にある $A'$ の理想であると言うのは、$aA' \subset a'$ であるというと同等であり、$a'/aA'$ は $(0)$ の上にある $\mathbf{A}'/aA'$ の理想であると言えます。

#### 補題 1 {#ac-v-s2-lem-1 .statement tag=04PK}

$h : \mathbf{A} \to \mathbf{A}'$ を環準同型, $S$ を $\mathbf{A}$, $i = i_A^S : \mathbf{A} \to S^{-1}\mathbf{A}$, $i' = i_{A'}^{h(S)} : \mathbf{A}' \to S^{-1}\mathbf{A}' = (h(S))^{-1}\mathbf{A}'$ 標準準同型および $h_1 = S^{-1}h : S^{-1}\mathbf{A} \to S^{-1}\mathbf{A}'$ の乗算部分集合とすると、可換式が成立します。 図式

$$
\begin{array}{ccc}
\mathbf{A} & \xrightarrow{h} & \mathbf{A}' \\
i \downarrow & & i' \downarrow \\
S^{-1}\mathbf{A} & \xrightarrow{h_1} & S^{-1}\mathbf{A}'
\end{array}
$$

$p$ を $p \cap S = \varnothing$ となるような $\mathbf{A}$ の主要な理想とする。すると、$a' \mapsto S^{-1}a'$ は、$p$ の上にある$\mathbf{A}'$ の理想の集合 $\mathscr{F}$ を、$S^{-1}p$ の上にある$S^{-1}\mathbf{A}'$ の理想の集合 $\mathscr{F}_1$ への全射写像です。 写像 $a'_1 \mapsto i'(a'_1)$ は、所属から $\mathscr{F}$ までの理想の集合上に $\mathscr{F}_1$ の全単射が重なり、$h(S)$ に関して飽和しています。特に、$p' \mapsto S^{-1}p'$ は、$p$ の上にある$\mathbf{A}'$ の主理想の集合の全単射と、$S^{-1}p$ の上にある$S^{-1}\mathbf{A}'$ の主理想の集合です。

$S^{-1}p$ は $S^{-1}\mathbf{A}$ の主な理想であり、$i_1(S^{-1}p) = p$ (章 11、§ 2, no. 5、命題 11) であることがわかっています。 $S^{-1}p$ の上に$S^{-1}\mathbf{A}'$ の理想的な$b'$ が存在する場合、$h(i_1(b')) = i(h_1(b')) = p$ になります。 $S^{-1}i'(b') = b'$ (上記参照) のように、これはすでに写像 $a' \mapsto S^{-1}a'$ 含む $\mathscr{F}_1$ の下に $\mathscr{F}$ の像があることを示しています。一方、$a' \in \mathscr{F}$、$a \in A$、$s \in S$の場合、以下の同値が存在します。

$$
h_1(a/s) \in S^{-1}a' \iff h(a)/h(s) \in S^{-1}a'
$$
$\iff$ $h(t)h(a) \in a'$ となるような $t \in S$ が存在します
$\iff$ $ta \in \mathfrak{p}$ となるような $t \in S$ が存在します
$\iff a/z \in S^{-1}\mathfrak{p}$。

したがって、$h_1^{-1}(S^{-1}a') = S^{-1}\mathfrak{p}$ は、写像 $a' \mapsto S^{-1}a'$ の下で $\mathscr{F}$ の像が $\mathscr{F}_1$ に等しいという証明を完成させます。もう 1 つの主張は、章 11、§ 2, no. 5、命題 11 から続きます。

#### 命題 1 {#ac-v-s2-prop-1 .statement tag=04PL}

*$h : A \to A'$ を環準同型とし、$A'$ が $A$、$\mathfrak{p}'$ 、$A'$ および $\mathfrak{p} = h^{-1}(\mathfrak{p}')$ の主イデアルに対して積分となるようにします。 $\mathfrak{p}$ が最大であるためには、$\mathfrak{p}'$ が最大であることが必要かつ十分です。*

$B = A/\mathfrak{p}$, $B' = A'/\mathfrak{p}'$ と書き、$h_1 : B \to B'$ を商を取って $h$ から導出された準同型とします。 $B$ と $B'$ は整域で、$B'$ は $B$ の積分です ($§ 1$、no. 1、命題 2)。 $\mathfrak{p}$ (それぞれ $\mathfrak{p}'$) が最大であるということは、$B$ (それぞれ $B'$) が体であることを意味します。 命題は次の補題から続きます。

#### 補題 2 {#ac-v-s2-lem-2 .statement tag=04PM}

*$B$ を $B$ の整域と $A$ 部分環とし、$B$ が $A$ で整数となるようにします。 $B$ が体であるためには、$A$ が体であることが必要かつ十分です。*

$A$ が体の場合、$B$ の同盟国 $\neq 0$ にとって、$A[y]$ は仮定 ($§ 1$, 定理 1) によって有限生成された $A$ モジュールになります。 $A[y]$ は整域なので、それは体 (*代数*, 章 V, § 2, no. 1, 命題 1) であり、*なおさら* $y$ は $B$ で反転可能であるため、$B$ 体です。逆に、$B$ が体で、$z \neq 0$ を $A$ とします。 $z^{-1} \in B$、$z^{-1}$ は $A$ に対して積分であるため、他の語には積分依存関係の方程式が存在します。

$$
z^{-n} + a_1 z^{-(n-1)} + \ldots + a_n = 0
$$

どこに$a_i \in A$;さて、これ関係はそれを示しています

$$
-z^{-1} = a_1 + a_2 z + \ldots + a_n z^{n-1} \in A,
$$

したがって、$A$ は確かに体です。

#### 系 1 {#ac-v-s2-lem-2-cor-1 .statement tag=04PN}

*$h : A \to A'$ 環準同型を、$A'$ が $A$、$\mathfrak{p}$ の主要な理想である $A$ と $\mathfrak{p}'$ および $a'$ の上にある $A'$ の 2 つの理想を積分するようにします。 $\mathfrak{p}$ は $\mathfrak{p}' \subset a'$ となります。 $\mathfrak{p}'$ が素数の場合、$a' = \mathfrak{p}'$。*

$S = A - \mathfrak{p}$ と書きましょう。この場合、$S^{-1}A'$ は $S^{-1}A$ の積分になります ($§ 1$、no. 5、命題)

16)、$S^{-1}p$ は $S^{-1}A$ (章 11、§ 2, no. 5、命題 11) の最大の理想であり、$S^{-1}a'$ と $S^{-1}p'$ は $S^{-1}p$ の上にある $S^{-1}A'$ の理想です(補題 1) と $S^{-1}a' \supseteq S^{-1}p'$。 $S^{-1}p'$ は素数なので、命題 1 によって最大となり、したがって $S^{-1}p' = S^{-1}a'$ になります。したがって、$a'$ は、$h(S)$ に対する$p'$ の彩度に含まれており、$p'$ (章 II, § 2, no. 5, 命題 11) に等しくなります。

#### 系 2 {#ac-v-s2-lem-2-cor-2 .statement tag=04PO}

$A'$ を $A'$ の整域、$A$ 部分環とし、$A'$ が$A$ と$f$ 準同型で$A'$ から環までの積分となるようにします。 $B$。 制限から $A$ までが単射である場合、$f$ は単射です。

$a'$ が核オフの場合、仮定は $a' \cap A = (0)$ を意味します。 $A'$ が整域であるため、$p$ と $p'$ をそれぞれ$A$ の理想 (0) と$A'$ の理想 (0) としてよって $a' = (0)$ として、系 1 を適用できます。

#### 系 3 {#ac-v-s2-lem-2-cor-3 .statement tag=04PP}

$h : A \to A'$ を環準同型とし、$A'$ が $A$ と $m$ の最大理想$A$ について積分し、$A'$ には有限の数の個別の最大理想$m'_j$ のみが存在すると仮定します。 ($1 \leq j \leq n$) $m$ の上に横たわっています。 $m'_j$ (章 II, § 2, no. 4) に対する $mA'$ の彩度を $q'_j$ とします。次に:
(i) 環 $A'/q'_j$ では、零の因子は $m'_j/q'_j$ の元であり、それらは零能 ($1 \leq j \leq n$) です。
(ii) $mA' = \bigcap_j q'_j = \prod_j q'_j$。
(iii) 標準準同型 $A'/mA' \to \prod_j (A'/q'_j)$ は全単射です。

$A'$ から含む $mA'$ までの主要な理想の場合、$m$ は $A$ で最大であるため、その逆像が $h$ 含む $m$ の下にあり、したがって$m$ より上にあることが必要かつ十分です。したがって、$m'_j$ は $A'$ 含む $mA'$ (命題 1) の唯一の素イデアルであり、したがって $c' = \bigcap_j m'_j$ は $mA'$ の根基 (章 II, § 2, no. 6, 系 1 ～ 命題 13）。 $q'_j$の定義までに、類mod。 $A' - m'_j$の元の$q'_j$は、$A'/q'_j$の0の因子ではありません。一方、$m'_j$ は別個の最大理想であるため、添字 $j$ ごとに元 $a'_j$ 所属から $\bigcap_j m'_j$ までが存在し、$m'_j$ (章 II, § 1, no. 1, 命題 4): したがって、すべての $x \notin m'_j, a'_j x \in r'$ に対して、類 mod. $a'_j x$の$q'_j$はゼロであり、$a'_j$は0の因子ではないので、$x$の類はゼロであると結論する考えます。他の語 $m'_j$ は$q'_j$ の根基であり、(i) を証明します。したがって、$q'_j$ は対 (章 II, § 1, no. 1, 命題 3) において互いに素であることがわかります。したがって、(iii) は、章 II, § 1, no. 2、命題を考慮すると、(ii) の帰結になります。 5. (ii) を確立するには、環 $A'/mA'$ では、$m'_j/mA'$ が唯一の最大理想であり、$q'_j/mA'$ が飽和であることに注意してください。 $m'_j/mA'$ (章 11, § 2, no. 4) に関して (0) のうち、したがって、私たちはケース $mA' = (0)$ に注意を限定するかもしれません。 (ii) の主張は、章 II, § 3, no. 3、系 2 から定理 1 に続きます。

#### 注意 (1) {#ac-v-s2-n1-rem-1 .statement tag=04PQ}

$A'$ がネーター の場合、(i) と (ii) から、$(q'_j)_{1 \leq j \leq n}$ は $mA'$ (章 IV, § 2, no. 3) の一意の主分解であることがわかります。

#### 定理 1 {#ac-v-s2-thm-1 .statement tag=04PR}

$h : A \to A'$ を単射詞環準同型とし、$A$ が $A$ と $p$ が $A$ の素イデアルに対して積分となるようにします。 $p$の上には、$A'$の主要な理想$p'$が存在します。

まず、$A$ が局所環であり、$p$ が $A$ の最大理想であると仮定します。すると、$A'$ のすべての最大イデアル $m'$ に対して、$h^{-1}(m')$ は $A$ (命題 1) の最大イデアルなので、$p$ に等しくなります。この場合、定理であることが証明されます ($A'$ 含むなので) $A$ 仮定なので 0 には減りません)。 一般的なケースでは、$S = A - p$ と書きましょう。その場合、$S^{-1}A$ は局所環で、その最大理想値は $S^{-1}p$ (章 11、§ 2, no. 5、命題 11)、$S^{-1}h : S^{-1}A \to S^{-1}A$ は単射法 (章 II, § 2, no. 4、定理 1) であり、 $S^{-1}A'$ は $S^{-1}A$ に対して整数です ($§ 1$、no. 5、命題 16)。その場合、$S^{-1}p$の上にある$S^{-1}A'$の主イデアル$q'$が存在し、$q' = S^{-1}p'$がわかります。ここで、$p'$は、$p$(補題1)の上にある$A'$の主イデアルです。

$h : A \to A'$ が単射でない場合、準同型 $Z \to \mathbf{Z}/n\mathbf{Z} \ (n > 1)$ の例が示すように、定理 1 は必ずしも真ではなくなります。ただし、定理 1 は標準単射 $h(A) \to A'$ に適用できます。他の語、主張の定理 1 は、素イデアル $p$ 含む $\mathrm{Ker}(h)$ に当てはまります。

#### 系 1 {#ac-v-s2-thm-1-cor-1 .statement tag=04PS}

仮説と定理 1、$\bar{h}^{-1}(pA') = p$ の記法を使用します。

$pA' \subset p'$ と $\bar{h}(p') = p$。

#### 系 2 {#ac-v-s2-thm-1-cor-2 .statement tag=04PT}

$h : A \to A'$ を環準同型とし、$A'$ が $A$、$a$、$p$ の 2 つの理想$A$ に対して積分となり、$a \subset p$ と $a'$ が$A'$ の理想を上に置くようにします。 $a$。 $p$ が素数だとします。そして、$p$と含む$a'$の上に、$A'$の主要な理想$p'$が存在します。

$h_1 : A/a \to A'/a'$ が $h$ から商を取って導出された準同型である場合、$h_1$ は仮定により単射であり、$A'/a'$ は $A/a$ の積分です ($§ 1$, no. 1, 命題 2)。その場合、$p/a$ (定理 1) の上に$A'/a'$ ($A$ の p' 素数) の素イデアル $p'/a'$ が存在し、$p'$ が必要なイデアルです。

#### 系 3 {#ac-v-s2-thm-1-cor-3 .statement tag=04PU}

$A$ を環および $A'$ 環含む $A$ とし、$A$ について積分します。 $\mathscr{R}'$ が $A'$ のジェイコブソン根基である場合、$\mathscr{R}' \cap A$ は $A$ のジェイコブソン根基です。

$32$ を $A$ のジェイコブソン根基とします。 $A'$ の各最大イデアル $m'$ に対して、$m' \cap A$ は $A$ (命題 1) の最大イデアルなので、$\mathscr{R} \subset m' \cap A$、したがって $\mathscr{R} \subset \mathscr{R}' \cap A$ (代数, 章 VIII, § 5, no. 3, 定義 3）。逆に、$x \in 32' \cap A$; とします。 $A$ の最大理想 $m$ ごとに、$m$ (定理 1) の上にある主理想 $A'$ が存在し、この理想 $m'$ は必然的に最大 (命題 1) となるため、$x \in m' \cap A = m$ となり、したがって$x \in 32$。

#### 系 4 {#ac-v-s2-thm-1-cor-4 .statement tag=04PV}

$A$ を環、$A'$ 環含む $A$ とし、$A$ と $f$ 準同型を $A$ から代数閉体まで積分します。 $L$。すると、$f$ は、$A'$ から $L$ まで、準同型まで拡張できます。

$\mathfrak{p}$ を $f$ の核とします。これは、$f(A) \subset L$ が整域であるため、最も理想的です。 $\mathfrak{p}'$ を、$\mathfrak{p}$ (定理 1) の上にある $A'$ の主要な理想とします。 次に、$A/\mathfrak{p}$ は$A'/\mathfrak{p}'$ の部分環と正準的に識別され、$A'/\mathfrak{p}'$ は$A/\mathfrak{p}$ ($§ 1$、no. 1、命題 2) に対して積分されます。 準同型 $f$ 定義する、$A/\mathfrak{p}$ の商、同型を $L$ の部分環 $f(A)$ にすると、体の同型 $g$ に拡張できます。 分数 $A/\mathfrak{p}$ の $K$ を $L$ の部分体に。 As the field of fractions $K'$ of $A'/\mathfrak{p}'$ is algebraic over $K$, $g$ can be extended to an isomorphism $g'$ of $K'$ onto a subfield of $L$ (Algebra, Chapter V, $§ 4$, no. 2, Corollary to Theorem 1); if $\pi': A' \to A'/\mathfrak{p}'$ is the canonical homomorphism, $g' \circ \pi'$ is a homomorphism from $A'$ to $L$ extending $f$.

#### 注意 (2) {#ac-v-s2-n1-rem-2 .statement tag=04PW}

$h : A \to A'$ を環準同型とし、$A'$ が $A$ で整数となるようにします。その後、関連する連続写像 $^a h : \mathrm{Spec}(A') \to \mathrm{Spec}(A)$ が閉じられます。 $A'$ のすべての理想 $a'$ について、$A'/a'$ は $A'$ に対して積分であるため、$A$ ($§ 1$、no. 1、命題 6) に対しても整数であり、$\mathrm{Spec}(A'/a')$ は閉じた部分空間 $V(a')$ と同一視されます。 $\mathrm{Spec}(A')$の; $^a h$ が閉じていることを示すには、($A'/a'$ による置き換えること $A'$)、$^a h$ の下の $\mathrm{Spec}(A)'$ の像が $\mathrm{Spec}(A)$ の閉じた部分集合であることを証明すれば十分であることがわかります。さて、定理 1 から、この像は、$A$ 含むの理想 $\mathrm{Ker}(h)$ の主な理想の集合であり、この集合は $\mathrm{Spec}(A)$ の位相の定義によって閉じられます。

#### 命題 2 {#ac-v-s2-prop-2 .statement tag=04PX}

$h : A \to A'$ を環準同型とし、$A'$ が $A$、$\mathfrak{p}$ の主理想 $A$、$S = A - \mathfrak{p}$、$(p'_i)_{i \in I}$ の上にある$A'$ のすべての主理想 $\mathfrak{p}$ の族に対して積分となるようにします。 $\mathfrak{p}$ と $S' = \bigcap_{i \in I} (A' - p_i)$;それから$S^{-1}A' = {S'}^{-1}A'$。

実際、定義 $h(S) \subset S'$ までに、そして、

$$
h(S)^{-1}A' = S^{-1}A',
$$

章 II, $§ 2$, no. 3, 命題 8 によって、$A'$ の素イデアル $q'$ が $h(S)$ を満たさない場合、$S'$ も満たさないことを証明するだけで十分です。ここで、$q' \cap h(S) = \varnothing$ を仮定し、$q = h^{-1}(q')$ とします。次に$q \cap S = \varnothing$、もう一方は語 $q \subset \mathfrak{p}$です。 $q'$ は定義だけ$q$ の上にあるので、系 2 から命題 1 まで、添字 $c$ があり、$q' \subset p'_c$ となり、$q' \cap S' = \varnothing$ となり、証明が完成します。

#### 命題 3 {#ac-v-s2-prop-3 .statement tag=04PY}

$A'$ が有限生成された $A$ 加群となるように、$h : A \to A'$ を環準同型とします。その場合、$A$ のすべての素イデアル $\mathfrak{p}$ に対して、$\mathfrak{p}$ の上にある $A'$ の素イデアルの集合は有限です。

$S = A - p$ にしましょう。 補題 1 により、$S^{-1}A$ により置き換える $A$、$S^{-1}A'$ (有限生成された $S^{-1}A$ モジュール) により $A'$、そして $S^{-1}p$ により $p$ を生成できます。他の語では、$A$が局所環で、$p$がその最大の理想であると仮定できます。次に、(この番号の最初に作成された注意によって) $A'/pA' = (A/p) \otimes_A A'$ は有限生成された $(A/p)$ モジュールであるため、$A$ は $A/p$ に、$A'$ は $A'/pA'$ に、$p$ は $(0)$ に置き換えることができます。したがって、$A$ が体と $p = (0)$ である場合、最終的に問題を証明命題に減らすことができます。 $A'$ は有限階数の $A$-代数であり、したがってアルティンであり、そのような代数には有限の素イデアル (章 IV, § 2, no. 5, 命題 9) だけが有限の数しか存在しないことがわかります。

### 2. 分解群と慣性群

#### 定義 2 {#ac-v-s2-def-2 .statement tag=04PZ}

$A'$ を環および $G$ 群を $A'$ ($§ 1$、no. 9) で演算するとします。 元 $\sigma \in G$ の主イデアル $p' \subset A'$ 部分群が与えられると、$\sigma.p' = p'$ は ($G$ に関して) $p'$ の分解群と呼ばれ、$G^z(p')$ で示されます。 $G^z(p')$ の下で不変である $A'$ の元の環は、($G$ に関して) $p'$ の分解環と呼ばれ、$A^z(p')$ (*) で表されます。

曖昧さがない場合は、$G^z(p')$ と $A^z(p')$ の代わりに、それぞれ $G^z$ と $A^z$ と書くことがよくあります。

すべての $\sigma \in G^z(p')$ について、商を取り、$A'$ の自己準同型 $x \mapsto \sigma.x$ から派生した環 $A'/p'$ の $z \mapsto \sigma.z$ 自己準同型によっても表します。明らかに群 $G^z(p')$ は環 $A'/p'$ にこのように動作します。

#### 定義 3 {#ac-v-s2-def-3 .statement tag=04Q0}

With the notation of Definition 2, the subgroup of $G^z(p')$ consisting of those $\sigma$ such that the endomorphism $z \mapsto \sigma.z$ of $A'/p'$ is the identity is called the inertia group of $p'$ (with respect to $G$) and denoted by $G^T(p')$ (or $G^T$). $G^T(p')$ の下での不変量 $A'$ の元の環は、$p'$ ($G$ に関して) の慣性環と呼ばれ、$A^T(p')$ (または $A^T$) (†) で表されます。

$A$ が $G$ の不変式の $A'$ からなるの部分環である場合、明らかに

$$
A \subset A^z(p') \subset A^T(p') \subset A'.
$$

定義 2 と 3 から、すべての $p \in G$ について、

$$
G^z(\rho.p') = \rho G^z(p') \rho^{-1}, \quad G^T(\rho.p') = \rho G^T(p') \rho^{-1}.
$$

すべての $\sigma \in G^z(p')$ について、$\bar{\sigma}$ が $A'/p'$ の自己同型 $z \mapsto \sigma.z$ である場合、$\sigma \mapsto \bar{\sigma}$ は、$G^z$ から群自己同型の $\Gamma_0$ の準同型 (正規と呼ばれます) です。

(*) 文字$Z$はドイツ語の語「Zerlegung」の頭文字で、「分解」を意味します。
(†) T という文字は、「慣性」を意味するドイツ語の語「Tragheit」の頭文字です。

A'/p' は不変のまま $A^{\mathbf{Z}}/(p' \cap A^{\mathbf{Z}})$ の元 (標準的には $A'/p'$ の部分環と識別される) であり、定義 $\mathscr{G}^{\Gamma}(p')$ により、この標準準同型の核になります。したがって、$\mathscr{G}^{\Gamma}$ は、$\mathscr{G}^{\mathbf{Z}}$ の通常の部分群です。 $k'$ が $A'/p'$ の分数の体である場合、$A'/p'$ のすべての自己同型は$k'$ の自己同型に一意に拡張できるため、$\sigma \mapsto \bar{\sigma}$ は $\mathscr{G}^{\mathbf{Z}}(p')$ から準同型と見なすことができます。 $k'$の自己同型の群。 注意最後に、$\mathscr{G}^{\mathbf{Z}}$では$\mathscr{G}^{\Gamma}$が正常であるため、$A^{\Gamma}$は$\mathscr{G}^{\mathbf{Z}}$以下で安定します。

#### 補題 3 {#ac-v-s2-lem-3 .statement tag=04Q1}

*$A'$ を $A'$ と $S$ の主要な理想である $\mathscr{G}$、$p'$ の不変式の $A'$、$A$ 環で演算する環、$\mathscr{G}$ 群とします。 $A$ の乗法部分集合が $p'$ を満たしていません。次に、$\mathscr{G}^{\mathbf{Z}}(S^{-1}p') = \mathscr{G}^{\mathbf{Z}}(p')$、$\mathscr{G}^{\Gamma}(S^{-1}p') = \mathscr{G}^{\Gamma}(p')$、そして$\mathscr{G}$ が局所的に有限である場合、$S^{-1}A^{\mathbf{Z}}(p') = A^{\mathbf{Z}}(S^{-1}p')$ と $S^{-1}A^{\Gamma}(p') = A^{\Gamma}(S^{-1}p')$ です。*

$S$ の元は $\mathscr{G}$ の下で不変であるため、$\sigma.p' = p'$ の場合は明らかに $\sigma.(S^{-1}p') = S^{-1}p'$ も不変です。逆に、$\sigma \in \mathscr{G}$ が $\sigma.(S^{-1}p') = S^{-1}p'$ となると仮定します。次に、$x \in p'$、$(\sigma.x)/1 \in S^{-1}p'$ の場合、$p'$ は素数であり、$s \notin p'$ であるため、$s(\sigma.x) \in p'$、よって $\sigma.x \in p'$ となる $s \in S$ が存在します。これは $\sigma.p' \subset p'$ であることを証明し、同様に $\sigma^{-1}.p' \subset p'$ であることが証明できるため、$\sigma.p' = p'$ と $\sigma \in \mathscr{G}^{\mathbf{Z}}(p')$ が決まります。 $\sigma \in \mathscr{G}^{\Gamma}(p')$ の場合、すべての $x \in A'$ に対して $\sigma.x - x \in p'$、したがってすべての $s \in S$ に対しても、

$$
\sigma.(x/s) - (x/s) = (O.x - x)/s \in S^{-1}p'
$$

したがって $\sigma \in \mathscr{G}^{\Gamma}(S^{-1}p')$ です。逆に、$\sigma \in \mathscr{G}^{\Gamma}(S^{-1}p')$; と仮定します。すると、すべての $x \in A'$、$\sigma.(x/1) - (x/1) \in S^{-1}p'$ に対して、上記 $\sigma.x - x \in p'$ と同様に $s(\sigma.x - x) \in p'$、よってとなる $s \in S$ が存在し、$\sigma \in \mathscr{G}^{\Gamma}(p')$ が証明されます。最後の 2 つの主張は、§ 1, no. 9、命題 23 に続きます。

#### 定理 2 {#ac-v-s2-thm-2 .statement tag=04Q2}

*$A'$ を環、$\mathscr{G}$ 有限群とし、$\mathscr{G}$ の不変量の $A'$ および $A$ 環で演算すると、$A'$ は $A$ (§ 1, no. 9、命題) について整数になります。 22).*

(i) *$A$ の同じ素イデアル $p$ の上にある 2 つの素イデアル $A'$ $p', q'$ が与えられると、$q' = \sigma.p'$ となるような $\sigma \in \mathscr{G}$ が存在します。他の語では、$\mathscr{G}$ は、$p$ の上にある $A'$ の素イデアルの集合で推移的に動作します。

(ii) *$p'$ を、$A'$、$p = p' \cap A$、$k$ (それぞれ $k'$) 体の分数または $A/p$ (それぞれ $A'/p'$) の主理想とする。 次に、$k'$ は、$k'$ 定義するの $k$ 自己同型の $\mathscr{G}^{\mathbf{Z}}(p')$ から群 $\Gamma$ までの $k$ と標準準同型 $\sigma \mapsto \bar{\sigma}$ の準ガロア拡張 (*) です。 $\mathscr{G}^{\mathbf{Z}}(p')/\mathscr{G}^{\Gamma}(p')$ の商、同型を $\Gamma$ に*。

(*) 位数では、語 「正規」の他の意味との混同を避けるため、今後、代数、章 V, § 6, no. 2、定義 2 で定義される項 「正規拡大」と同義として、項 「準ガロア拡張」を使用します。

(i) $x \in \mathfrak{q}$ の場合は $\prod_{\sigma \in \mathscr{G}} \sigma.x \in q' \cap A = p \subset p'$;その場合、$\sigma.x \in p'$、つまり $x \in \sigma^{-1}.q'$ となるような $\sigma \in \mathscr{G}$ が存在します。 結論するは $q' \subset \bigcup_{\sigma \in \mathscr{G}} \mathfrak{s}.\mathfrak{p}'$ であり、したがって ($\mathscr{G}$ は有限であり、$\mathfrak{s}.\mathfrak{p}'$ 素数であるため) $\mathfrak{q}' \subset \mathfrak{s}.\mathfrak{p}'$ (章 II, § 1, no. 1, 命題 2) となる $\sigma \in \mathscr{G}$ が存在します。 $q'$ と $\sigma.\mathfrak{p}'$ は両方とも $p$、$q' = \sigma.\mathfrak{p}'$ (no. 1、系 1 ～ 命題 1) の上にあります。

(ii) $k'$ が $k$ の準ガロア拡張であることを確認するには、すべての元 $\bar{x} \in A'/p'$ が、$k[X]$ の多項式 $P$ の根であり、そのすべての根が $A'/p'$ に含まれることを証明するだけで十分です。 (代数、章、V, § 6, no. 3、系 3 ～ 命題 9)。さて、$x \in A'$ を類 $\bar{x}$ の代表とします。多項式 $Q(X) = \prod_{\sigma \in \mathscr{G}} (X - \sigma.x)$ の係数はすべて $A$ にあります。 $P(X)$ を $(A/p)[X]$ の多項式とし、その係数は標準準同型 $\pi : A \to A/p$ の下で $Q$ の像となります。 $\pi$ は標準準同型 $\pi' : A' \to A'/p'$ の制限から $A$ と考えることができるので、$P$ は線形因子 $X - \pi'(\sigma.x)$ の $(A'/p')[X]$ の積であることがわかり、次のようになります。 $\bar{x} = \pi'(x)$から問題。

明らかに、すべての $\sigma \in \mathscr{G}^z$ に対して、$\hat{\sigma}$ は $k'$ の $k$ 自己同型です。 $k'$ のすべての $k$ 自己同型の群上で $\sigma \mapsto \hat{\sigma}$ 写像 $\mathscr{G}^z$ が成り立つことを検証する必要があります。 $S = A - p$ と書きましょう。 $k$ と $k'$ は、§ 1, no. 9、命題 23、関係 $S^{-1}p' \cap S^{-1}A = S^{-1}(A \cap p') = S^{-1}p$ により、置き換えること $A'$ と$p'$ はそれぞれ$S^{-1}A'$ と$S^{-1}p'$ によって変更されません。 (章 11、§ 2, no. 4); 補題 3 から、$k'$ の $\mathscr{G}^z$ もその演算も変更されていないことがわかります。したがって、$p$ が最大である場合に注意を限定することができます。この場合、$p'$ (no. 1、命題 1) も同様であることがわかり、したがって、$k'$ のすべての元は、一部の $x \in A'$ では形 $\pi'(x)$ になります。このような元は、次数 $\leq \mathrm{Card}(\mathscr{G})$ の $k[X]$ における多項式の根であることが上でわかりました。 $k$ のすべての有限分離拡大は原始元 (代数、章 V, § 7, no. 7、命題 12 および § 11, no. 4、命題 4) を受け入れるので、すべての有限が$k'$ に含まれる $k$ の分離拡大は次数 $\leq \mathrm{Card}(\mathscr{G})$, よってであるため、$k'$ に含まれる $k$ の最大の分離拡大 $k'_s$ (代数, 章 V, § 7, no. 6、命題 11) は、次数 $\leq \mathrm{Card}(\mathscr{G})$ (代数、章 V, § 3, no. 2、注意 2) です。 $y \in A'$ を元とし、$\pi'(y)$ が $k'_s$ のプリミティブ元であるようにします。 $\sigma \in \mathscr{G} - \mathscr{G}^z$ の理想 $\sigma.p'$ は最大であり、$p'$ から定義まで異なります。したがって、$\sigma \in \mathscr{G} - \mathscr{G}^z$ (章 11、§ 1, no. 2、命題 5) に対して $x \equiv y \pmod{p'}$ と $x \in \sigma^{-1}p'$ となるような $x \in A'$ が存在します。 したがって、$u$ を $k'$ の $k$ 自己同型とし、$P(X) = \prod_{\sigma \in \mathscr{G}} (X - \pi'(\sigma.x))$ とします。 $\pi'(x)$ は $P$ と $P \in k[X]$ の根であるため、$u(\pi'(x))$ は $k'$ の $P$ の根であるため、次のような $\tau \in \mathscr{G}$ が存在します。

$$
u(\pi'(x)) = \pi'(\tau.x);
$$

しかし、$u(\pi'(x)) \neq 0$、そして$\sigma \in \mathscr{G} - \mathscr{G}^z$の場合、$\sigma.x \in p'$、したがって$\pi'(\sigma.x) = 0$です。私たちは結論する、必然的に$\tau \in \mathscr{G}^z$になります。しかし、$u$ と $\tilde{\tau}$ は、$k'_s$ の原始元 $\pi'(y) = \pi'(x)$ に対して同じ値を持っているため、$k'_s$ では一致するとなり、$k'$ は基数拡大であるため、 $k'_s$、彼らは$k'$に一致するです。

#### 系 {#ac-v-s2-n2-cor-1 .statement tag=04Q3}

*仮説と定理 2 のうち記法を使って、$f_1, f_2$ を $A$ ～ 体 $L$ の 2 つの準同型とし、同じ制限 ～ $A$ とします。すると、次のような $\sigma \in \mathscr{G}$ が存在します*

$$
f_2(x) = f_1(\sigma.x)
$$

*すべての方へ* $x \in A'$。

$p'_i$ を $f_i$ ($i = 1, 2$) の核とします。これは、$A'$ の主要な理想です。 仮定 $p'_1 \cap A = p'_2 \cap A$ によって、この共通部分は $A$ の主要な理想 $p$ です。したがって、$\tau.p'_2 = p'_1$ (定理 2 (i)) となるような $\tau \in \mathscr{G}$ が存在します。 置き換えること $f_1$ 準同型 $x \mapsto f_1(\tau.x)$ により、$p'_2 = p'_1$ (理想を $p'$ で表す) と仮定できます。 商を取ることで、$f_1$ と $f_2$ から $A'/p'$ から $L$ までの 2 つの単射準同型 $f'_1, f'_2$ を導き出し、したがって拡大するは体から 2 つの単射準同型 $f''_1, f''_2$ になります。 分数 $A'/p'$ から $L$ の $k'$。 $k'$ は $k$ の準ガロア拡張であるため、$k''_1 = f''_1(k')$ と $k''_2 = f''_2(k')$ (k は $L$ の部分体で識別される) と、$k''_2, k''_1 = k''_2$ への $k''_1$ の k-同型写像があるため、 (*代数*、章 V, § 6、命題 6)。したがって、$f''_1 \circ {f''_2}^{-1}$ は $k'$ の k 自己同型です。 定理 2 (ii) より、それは形 6 であり、ここで $\sigma \in \mathscr{G}^z(p')$ です。特に、すべての $x \in A'$ 元 $f_2(x)$ と $f_1(\sigma.x)$ は等しいです。

**注意**

(1) 定理 2 の仮説の下では、$k'$ が $k$ (練習問題 9) 上で分離できない場合、$k'$ は $k$ 上で *無限* になる可能性があることに注意してください。

(2) 体 $k$ が *完全* であれば、明らかに $k$ は $k$ の *ガロア* 拡大です。その後、$k$ にわたって有限になります。

#### 命題 4 {#ac-v-s2-prop-4 .statement tag=04Q4}

*$A'$ を $\mathscr{G}$ の不変式の $\mathscr{G}$、$A$、$B$ 環の$A'$、$\mathscr{H}$ 部分群で演算する環、$\mathscr{G}$ 有限群とします。それぞれ$\mathscr{H}$と$p'$は$A$の主要な理想です。 $p = A \cap p'$と$p(B) = B \cap p'$と書きましょう。

(i) $\mathscr{H}$ が分解群 $\mathscr{G}^z(p')$ に含まれるためには、$p'$ が$p(B)$ の上にある$A$ の唯一の主要イデアルであることが必要かつ十分です。

(ii) *$\mathscr{H}$ 含む $\mathscr{G}^z(p')$ の場合、次の条件が満たされます*:
(a) *環 $A/p$ と $B/p(B)$ は、分数* の同じ体を持ちます。
(b) *局所環 $B_{p(B)}$ の最大理想は $pB_{p(B)}$* に等しい。

(iii) *さらに、$A'$ が整域であり、$\bigcap_{n \geq 0} p^nA'_p = 0$ であると仮定します。この場合、条件 (a) および (b) & (ii) は、$\mathscr{G}^z(p')$ が $B$* の元を不変のままにすることを意味します。

(i) 定理 2 (i) から、$p(B)$ の上にある$A$ の主要な理想は、$\sigma \in \mathscr{H}$ である形 $\sigma.p'$ の理想であることがわかります。 よってすぐに (i)。

(ii) $S = A - p$ と書きます。 $S^{-1}A'$ における $\mathscr{G}$ と $\mathscr{H}$ の不変量の環は、それぞれ $S^{-1}A$ と $S^{-1}B$ (§ 1, no. 9, 命題 23) と $\mathscr{G}^{\mathbf{Z}}(S^{-1}p) = \mathscr{G}^{\mathbf{Z}}(p')$ (補題 3) であることがわかります。最後に $S^{-1}p(B) = S^{-1}p' \cap S^{-1}B$ (章 II, § 2, no. 4)、素イデアルの局所環環の $S^{-1}p(B)$ $S^{-1}B$ は正準的に $B_{p(B)}$ と同型であり、その剰余体は の体と同型である$B/p(B)$ の分数 (章 II, § 2, no. 5、命題 11)。したがって、(ii) $p$ が最大である場合に注意を限定することを示すことができます。 (a) を確立するには、次のことを証明すれば十分です。

$$
B = A + p(B)
$$

これにより、体 $A/p$ と $B/p(B)$ が *正準的に同型* であることがわかります。 定理 2 までに、$p$ の上にある$A'$ の有限の素イデアル数だけが存在し、no. 1 の定理 1 までに、$B$ のすべての素イデアルの上に $A'$ の少なくとも 1 つの素イデアルが存在します。これは、$p$ の上にある $B$ の素理想の *有限の* 数だけが存在することを意味します。 $n_j$ ($1 \leq j \leq r$) は、これらの理想のうち $\neq p(B)$ であるものを示します。 $x$ を $B$ の元とします。理想 $p(B)$ と $n_j$ が最大 (no. 1, 命題 1) であるため、$1 \leq j \leq r$ (章) に対して $y \equiv x$ (修正 $p(B)$) と $y \in n_j$ となる $y \in B$ が存在します。 11、§ 1, no. 2、命題 5）。 $y_1 = y, y_2, \ldots, y_q$ を $\mathscr{G}$ の下の $y$ の軌道の元と区別します。明らかに

$$
z = y_1 + y_2 + \cdots + y_q \in A,
$$

そして、(3) を確立するには、$i \geq 2$ に対して $y_i \in p'$ を示すだけで十分です。その場合、$x \equiv y$ (修正 $p(B)$) から、$z - y \in p' \cap B = p(B)$、よって $x \in A + p(B)$ が推定されるからです。次に、$i \geq 2$ と $\sigma \in \mathscr{G}$ を $\sigma.y = y_i$ となるようにします。 $\sigma^{-1}.p'$ が $p(B)$ の上にないことがわかります。そうでなければ、$\sigma^{-1}.p' = \tau.p'$ (定理 2 (i))、よって $(\tau^{-1}\sigma^{-1}).p' = p'$ のような$\tau \in \mathscr{H}$ が存在し、仮定、よって $\sigma \in \mathscr{H}$ による他の語 $\tau^{-1}\sigma^{-1} \in \mathscr{G}^{\mathbf{Z}} \subset \mathscr{H}$ が存在することになるからです。しかし、$y \in B$ と $\sigma.y \neq y$ としては、これは不合理です。私たち結論するは、$\sigma^{-1}.p'$が理想$n_j$の一つの上にあり、構成による$y \in n_j$のように、確かに$y \in \sigma^{-1}.p'$か$y_i = \sigma.y \in p'$です。

(b) を証明するには、$p(B)$ が、$p(B)$ (章 II, § 2, no. 4, 命題 10) に関して理想$pB$ の*飽和* $q$ に含まれていることを確立すれば十分です。 $p(B)$ は $n_j$ ($1 \leq j \leq r$) のいずれにも含まれていないため、次のことを証明するだけで十分です。

$$
p(B) \subset q \cup n_1 \cup \cdots \cup n_r
$$

by 章 II, § 1, no. 1, 命題 2. このため、元 $u \in p(B)$ 所属を $n_j$ ($1 \leq j \leq r$) (章 11, § 1, no. 1, 命題) に含めないことを考慮します。 2); $u_1 = u, u_2, \ldots, u_m$ を、$\mathscr{G}$ の下の $u$ の軌道の別個の元とします。 $w = u_1u_2 \ldots u_m, v = u_2 \ldots u_m$と書きます。明らかに$w \in A$;一方、$\tau \in \mathscr{H}$ の場合、$\tau.u = u$ となり、$i \geq 2$ の場合は必然的に $\tau.u_i \neq u$ となり、$\tau.v = v$ となり、$v \in B$ となることがわかります。 (a) の証明のように、$\sigma \in \mathscr{G}$ が $\sigma.u = u_i$ である場合、$i \geq 2$、$\sigma^{-1}.p'$ は $n_j$ の 1 つの上にあり、$u \notin n_j$ と同様に $u \notin \sigma^{-1}.p'$、他の語にもあることがわかります。 $u_i \notin p'$。私たちは$v \notin p'$を結論する、したがって$v \notin p(B)$となります。一方、$w \in p' \cap A = p$ と関係 $w = uv$ は、$u$ が $p(B)$ に関して$pB$ の飽和状態にあることを示しており、したがって (4) が成立します。

(iii) Suppose that $A'$ is an integral domain, that $\bigcap_{n \geq 0} p^n A'_p = 0$ and that conditions (a) and (b) of (ii) hold. (ii) と同じ記法では、明らかに $S^{-1}A'$ は整域と $S^{-1}A'_p = A'_p$ です。したがって、$S^{-1}A'$ と $S^{-1}p'$ によって置き換える $A'$ と $p'$ が可能であり、他の語では、イデアル $p$ が最大であると仮定します。 仮説 (a) と (b) は次のことを意味します。

$$
\mathbf{B}_{p(B)} = A + p \mathbf{B}_{p(B)}
$$

$n$ の帰納法までに、すべての $n > 0$ について $\mathbf{B}_{p(B)} = A + p^n \mathbf{B}_{p(B)}$ であると推定します。次に、$\sigma$ を $\mathscr{G}^\mathbf{Z}$ の元とし、$x$ を $B$ の元とします。すべての $n > 0$ に対して、$x - a_n \in p^n \mathbf{B}_{p(B)} \subset p^n A'_p$ となる $a_n \in A$ が存在します。 $\sigma.a_n = a$ と $\sigma.p' = p'$ から、$\sigma.x - x \in p^n A'_p$ と推測します。この関係はすべての$n$に当てはまりますので、仮定から$\sigma.x = x$を結論するとします。

ハークス

(3) $A'$ が整域とネーター の場合、条件 $\bigcap_{n \geq 1} p^n A'_p = 0$ が常に成り立ちます (章 III, § 3, no. 2、系 ～ 命題 5)。 $A'$を整域、$A$をネーターとすれば、この条件も満たされることが示されます。

(4) $p$ が $A$ 関係の最大イデアルではない場合、(3) は (ii) の仮説のもとでは必ずしも成り立ちません。したがって、$\mathscr{H} = \mathscr{G}^\mathbf{Z}$, よって $B = A''$ (練習問題 10) をとったとしても、$A/p$ と $B/p(B)$ は必ずしも同型ではありません。

#### 系 1 {#ac-v-s2-prop-4-cor-1 .statement tag=04Q5}

定理 2 環 $A/p$ と $A^\mathbf{Z}/(p' \cap A^\mathbf{Z})$ は同じ体分数を持ち、局所環 $(A^\mathbf{Z})'_{p' \cap A^\mathbf{Z}}$ の最大理想は $p$ によって生成されます。

#### 系 2 {#ac-v-s2-prop-4-cor-2 .statement tag=04Q6}

$A'$ を $A'$ の主イデアルである $\mathscr{G}$ および $p'$ の不変式の $A'$ 、 $A'$ 環で動作する整域、$\mathscr{G}$ 有限群とします。 $K, K^\mathbf{Z}$ と $K$ をそれぞれ $A, A^\mathbf{Z}$ と $A'$ の分数の体とします。すると、$K'$ は $K$ と部分体 $L$ の $K$ 含む $K$ のガロア拡大となり、$p'$ が$A'$ の理想を上回る唯一の主要理想となります。 $A' \cap L$ の $p' \cap L$ は、含む $K^\mathbf{Z}$ となるものにすぎません。

$\mathscr{G}$ は $K'$ で動作し、$K$ は $K'$ の $\mathscr{G}$ の不変式の体 (§ 1, no. 9、命題 23 が $S = A - \{0\}$ に適用される) であり、同様に $K^\mathbf{Z}$ は不変式の体です$\mathscr{G}^\mathbf{Z}$の;したがって、定義 $K'$ は、$K$ のガロア拡大になります。 $\mathscr{G}$の部分群 $\sigma \in \mathscr{G}$のからなるがLの元を不変のままにすると、L 含む $K^{\mathbf{Z}}$は$\mathscr{H}$が$\mathscr{G}^{\mathbf{Z}}$に含まれることを意味します(代数, 章 V, § 10, no. 5, 定理 3) そして、L は $K'$ の $\mathscr{H}$ の不変量の体であるため、$A' \cap L$ は$\mathscr{H}$ の不変量の環です。 $A'$; 2 番目の主張は命題 4 (i) から続きます。

#### 定義 4 {#ac-v-s2-def-4 .statement tag=04Q7}

*仮説と系 2から命題 4の記法により、$A$の素イデアル$\mathfrak{p}$は、$\mathfrak{p}$の上にある$A'$の素イデアルの数が以下に等しい場合、$K'$で完全に分解するといわれています。 $[K':K]$.*

$\mathfrak{p}$ の上に横たわる $A'$ の素理想 $\mathfrak{p}'$ について、$A'$ のすべての元または $A^{\mathbf{Z}}(\mathfrak{p}') = A'$ を不変のままにして、部分群 $\mathscr{G}^{\mathbf{Z}}(\mathfrak{p}')$ が部分群 $\mathscr{M}$ に等しいと言うのと同じことになります。 $\mathscr{G}/\mathscr{M}$ は、$\mathfrak{p}$ の上にある$A'$ の主要な理想の集合に忠実に動作します。

#### 系 3 {#ac-v-s2-def-4-cor-3 .statement tag=04Q8}

*$A'$を整域、$\mathscr{G}$を$\mathscr{G}$の不変量の$A'$、$A$環、$A$の主イデアルである$\mathfrak{p}$で演算する有限可換群とする。それぞれ$A$と$A'$の$K$と$K'$分数の体。すると、$\mathfrak{p}$の上にある$A'$の主要な理想はすべて同じ分解環$A^{\mathbf{Z}}$を持ち、分数$K^{\mathbf{Z}}$の$A^{\mathbf{Z}}$の体は最大の中間の体になります。 $K$ と $K'$ の間で、$\mathfrak{p}$ は完全に分解します。*

If $\mathfrak{p}'$ is a prime ideal of $A'$ lying above $\mathfrak{p}$, then $\mathscr{G}^{\mathbf{Z}}(\sigma.\mathfrak{p}') = \mathscr{G}^{\mathbf{Z}}(\mathfrak{p}')$ since $\mathscr{G}$ is commutative (formula (2)), hence (Theorem 2 (i)) all the prime ideals of $A'$ lying above $\mathfrak{p}$ have the same decomposition group $\mathscr{G}^{\mathbf{Z}}$ and therefore the same decomposition ring $A^{\mathbf{Z}}$; their number is $(\mathscr{G}:\mathscr{G}^{\mathbf{Z}})$. L を K と $K'$ の中間値体とし、$\mathscr{H}$ を $\mathscr{G}$ の部分群とし、L の元を不​​変のままにします。 $\mathscr{H}$ に対する $\mathfrak{p}'$ の分解群は $\mathscr{G}^{\mathbf{Z}} \cap \mathscr{H}$ です。 $A' \cap L$ は $A'$ における $\mathscr{H}$ の不変量の環であるため、$\mathfrak{p}' \cap L$ の上にある $A'$ の素イデアルの数は $(\mathscr{H}:(\mathscr{G}^{\mathbf{Z}} \cap \mathscr{H})) = (\mathscr{H}\mathscr{G}^{\mathbf{Z}}:\mathscr{G}^{\mathbf{Z}})$ です ($\mathscr{G}$ は可換であるため)。 したがって、$\mathfrak{p}$ の上にある$A' \cap L$ の主要な理想の数は、$(\mathscr{G}:\mathscr{H}\mathscr{G}^{\mathbf{Z}})$ になります。 $\mathfrak{p}$ が完全にL に分解するには、$(\mathscr{G}:\mathscr{H}\mathscr{G}^{\mathbf{Z}}) = [L:K] = (\mathscr{G}:\mathscr{H})$、そして$\mathscr{H} \subset \mathscr{H}\mathscr{G}^{\mathbf{Z}}$ として、これが $\mathscr{H}\mathscr{G}^{\mathbf{Z}} = \mathscr{H}$ または$\mathscr{G}^{\mathbf{Z}} \subset \mathscr{H}$、そして最終的に$L \subset K^{\mathbf{Z}}$ と同等であることが必要かつ十分です。

#### 命題 5 {#ac-v-s2-prop-5 .statement tag=04Q9}

*With the hypotheses and notation of Theorem 2, the field of fractions $k^T$ of $A^T/(\mathfrak{p}' \cap A^T)$ is equal to the greatest separable extension $k'_s$ of $k$ contained in $k'$.*

As in Proposition 4 this may be reduced to the case where $\mathfrak{p}$ is a maximal ideal of $A$, which implies that $\mathfrak{p}'$, $\mathfrak{p}' \cap A^{\mathbf{Z}}$ and $\mathfrak{p}' \cap A^T$ are maximal in $A'$, $A^{\mathbf{Z}}$ and $A^T$ respectively (no. 1, Proposition 1).

すべての $x \in A'$ について、多項式 $P(X) = \prod_{\sigma \in \mathscr{G}^T} (X - \sigma.x)$ の慣性環 $A^T$ には係数があり、$\mathscr{G}^T$ の定義により、$A'$ のすべての根は合同 mod になります。 $\mathfrak{p}'$; $A^T/(\mathfrak{p}' \cap A^T)$ 上の多項式 $\pi'(P)$ の係数は、準同型 $\pi':A' \to A'/\mathfrak{p}'$ の下の P の標準像であるため、$A'/\mathfrak{p}'$ のすべての根は $x$ の像に等しく、次のことがわかります。 $k'$ は $k^T$ の部首拡大です。 よって $k'_s \subset k^T$、$k'_s$ のすべての元は k 上で分離可能であり、なおさらは $k^T$ 上で分離可能です。

$k'_s$ は k (代数, 章 V, § 10, no. 9, 命題 14) のガロア拡大であることがわかっており、定理 2 からそのガロア群は $\mathscr{G}' = \mathscr{G}^z / \mathscr{G}^T$ と同型であることがわかります。 $k^T$ は $k'_s$ の基数拡大であるため、$k^T$ は k の準ガロア拡張であり、k 上の $k^T$ の次数の分離可能な因子は $q = (\mathscr{G}^z : \mathscr{G}^T )$ です。 $k^T$ が k の分離拡大であることがわかります。上で、$\mathscr{G}'$ が $A^T$ の自己同型群と同一視され、$A^z$ が $\mathscr{G}'$ の不変式の環であることを見てきました。したがって、$x \in A^T$ の場合、多項式 $Q(X) = \prod_{\sigma' \in \mathscr{G}'} (X - \sigma'(x))$ の係数は $A^z$ になります。 $\pi'$ における Q の多項式の係数が像である $A^z / (p' \cap A^z)$ 上の多項式は、次数 $q$ であり、根 $\pi'(x) \in A^T / (p' \cap A^T )$ を持ちます。 命題 4 (ii) による $A^z / (p' \cap A^z) = k$ のように、$k^T$ のすべての元は k を超える次数 $\leq q$ であることがわかります。

従って、k を、$k$ の準ガロア拡張 $k^T$ の k 自己同型の群の不変量の体とします。次に、$[k^T : k_1] = q$ (代数、章 V, § 10, no. 9、命題 14)。 $u$ を $k_1$ 上の $k^T$ のプリミティブ元とします。 k 上の次数 $q$ と k 上の次数 $\leq q$ であるため、k 上の次数 $q$ であり、k 上の最小多項式は $k$ で係数になります。これは、$u$ が k 上で分離可能であることを示しています。一方、すべての $v \in k_1$ に対して、$v^{p'} \in k$ となるような特性指数 p の冪 $p'$ が存在します。私たちは結論する、それは$k(u - v)$、どれは含むです
$$
(u - v)^{p'} = u^{p'} - v^{p'},
$$
含む $u^{p'}$、従って $k(u^{p'})$ です。しかし、$u$ は$k$、$k(u) = k(u^{p'})$ (代数、章 V, § 8, no. 3、命題 4)、よって $k(u) \subset k(u - v)$ で分離可能です。 $u$ は k 上の次数 $q$ であり、$u - v$ は次数 $\leq q$ であるため、$k(u) = k(u - v)$、よって $v \in k(u)$ になります。これは、$v$ が k 上で分離可能であるため、$k_1 = k$ と $k^T$ が $k$ 上で分離可能であることを示しています。

#### 系 {#ac-v-s2-n2-cor-2 .statement tag=04QA}

*慣性群$\mathscr{G}^T(p')$の位数がkの特性指数pと相対的に素である場合、体$k'$はkのガロア拡大です。*

命題 5 の証明の記法では、多項式 $\pi'(P)$ の $k^T = k'_s$ には係数が含まれ、その根はすべて $\pi'(x)$ に等しくなります。 $\pi'(P)$ は $k'_s$ 上の $\pi'(x)$ の最小多項式の冪であるとすぐに推測します。しかし、後者は、p の冪に等しい次数を持ち、従って、$\pi'(P)$ の次数は $\mathscr{G}^T$ の位数に等しいので、仮定は $\pi'(x) \in k'_s$ を、他の語 $k'_s = k'$ を意味します。

### 3. 分解と一体的に閉じられた領域の慣性

#### 補題 4 {#ac-v-s2-lem-4 .statement tag=04QB}

*A を積分閉領域、K を分数の体、p を K の特性指数、K' を K の基数拡大、A' を K' 含む A の部分環とし、A 上の積分とする。 A のすべての素イデアル p に対して、固有の主イデアル * p' が存在します。 $p$ と $p'$ の上にある $A'$ は $x \in A'$ の集合であるため、$x^{p^m} \in p$ に対して整数 $m \geq 0$ が存在します。

$p'$ の存在は、no. 1、定理 1 から続きます。$x \in p'$ の場合、$A$ が積分的に閉じているため、$x^{p^m} \in p' \cap A = p$ であるため、$x^{p^m} \in K$、よって $x^{p^m} \in A$ となる$m \geq 0$ が存在します。逆に、$x \in A'$ が $x^{p^m} \in p \subset p'$ となる場合、$p'$ は素数であるため、$x \in p$ になります。

#### 注意 (1) {#ac-v-s2-n3-rem-1 .statement tag=04QC}

§ 1, no. 3, 系から命題 11 から、$K'$ の $A$ の積分閉包は $x \in K'$ の集合となり、$x^{p^m} \in A$ (代数, 章) に対して $m \geq 0$ が存在します。 V, § 8, no. 1、命題 1)。

#### 命題 6 {#ac-v-s2-prop-6 .statement tag=04QD}

Let $A$ be an integrally closed domain, $K$ its field of fractions, $K'$ a quasi-Galois extension of $K$ and $A'$ the integral closure of $A$ in $K'$. それから：

(i) $A$ のすべての素イデアル $p$ 、$K$ の群 $\mathscr{G}$ について、$K'$ の自己同型は、$p$ の上にある$A'$ の素イデアルの集合上で推移的に作用します。

(ii) For every prime ideal $p'$ of $A'$, the field of fractions $k'$ of $A'/p'$ is a quasi-Galois extension of the field of fractions $k$ of $A/(A \cap p')$ and the canonical homomorphism $\sigma \mapsto \tilde{\sigma}$ from $\mathscr{G}^Z(p')$ to the group $\Gamma$ of $k$-automorphisms of $k'$ defines, by taking the quotient, a bijection of $\mathscr{G}^Z(p')/\mathscr{G}^T(p')$ onto $\Gamma$.

(A) まず、$K'$ が $K$ のアジナイトガロア拡大であるとします。次に、$A$ は積分的に閉じており、$A$ は$A'$ における $\mathscr{G}$ の不変量の環であるため、$A = A \cap K$ となります。 $\mathscr{G}$ は有限であるため、この場合、no. 2、定理 2 から命題が続きます。

(B) 次に、$K'$ が $K$ のいずれかのガロア拡大であると仮定します。すると、$K'$は$K$の有限ガロア拡大の右指向家族$(K_\alpha)_{\alpha \in I}$の和集合です。 (i) を示すために、$p$ の上にある 2 つの主要な理想 $A'$ $p', q'$ を考えてみましょう。すべての$\alpha \in I$、$p' \cap K_\alpha$、$q' \cap K_\alpha$ は、$p$ の上にある $A \cap K_\alpha$ の 2 つの主要な理想です。 $A' \cap K_\alpha$ は $K_\alpha$ の $A$ の積分閉包なので、 $\mathscr{G}$ の形群の $K$ の自己同型の元の $K_\alpha$ への制限です。 $K$ の場合、(A) から、$(\sigma.(p' \cap K_\alpha)) = q' \cap K_\alpha$ となるような $\sigma \in \mathscr{G}$ が存在することがわかります。 $\mathscr{E}_\alpha$を上記性質をもつ$\sigma \in \mathscr{G}$の集合とします。 $\sigma \in \mathscr{G} - 8$ にしましょう。次に、すべての $\tau \in \mathscr{G}$ について、$K_\alpha$ の不変条件元を残して、(QT) $(\sigma.(p' \cap K_\alpha)) = \varrho.(p' \cap K_\alpha) \neq q' \cap K_\alpha$、したがって $\sigma \tau \in \mathscr{G} - b$ になります。その結果、$\mathscr{E}_\alpha$ はトポロジカルガロア群 $\mathscr{G}$ (代数, 章 V, 付録 11, no. 1) で閉じられており、明らかに家族 $(\mathscr{E}_\alpha)_{\alpha \in I}$ は方向付けされたままになっています。 $\mathscr{G}$ はコンパクト (前述、no. 2、命題 3) であり、$\mathscr{E}_\alpha$ は空ではないため、ファミリー $(8,)$ の共通部分 $\mathscr{E}$ は空ではなく、すべての $\sigma \in \mathscr{E}$ に対して $\sigma.p' = q'$、 よって (i)。

(ii) を示すには、$k'$ が右有向族 $(k_\alpha)_{\alpha \in I}$ の和集合であり、$k_\alpha$ が $(A' \cap K_\alpha)/(p' \cap K_\alpha)$ の分数の体であることに注意してください。各 $k_\alpha$ は (A) による $k$ の準ガロア拡張であるため、$k'$ (代数, 章 V, § 6, no. 3, 命題 8) も同様です。一方、$u$ を $k'$ の $k$ 自己同型とし、$\pi': A' \to A'/p'$ を標準準同型とします。 no. 2、定理 2 が $A' \cap K_\alpha$ に適用されるため、すべての $\alpha$ に対して $\sigma.(p' \cap K_\alpha) = p' \cap K_\alpha$ と $u(\pi'(x)) = \pi'(\sigma.x)$ となるような、元 $\sigma \in \mathscr{G}$ の空ではない集合 $F_\alpha$ が存在します。 $x \in A' \cap K_\alpha$。上記のように、$\mathscr{F}_\alpha$ は $\mathscr{G}$ で閉じられており、$(\mathscr{F}_\alpha)$ は左の有向集合であるため、その共通部分 $\mathscr{F}$ は空ではないことがわかります。 $\alpha \in \mathscr{F}$、$\alpha \in \mathscr{G}^\mathbf{Z}(p')$、$\tilde{\sigma} = u$ については明らかに、これで (ii) の証明が完了します。

(C) *一般的なケア*。 $\mathscr{G}$ の不変式 $K_1$ の体は、$K$ の基数拡大 (*代数*, 章 V, § 10, no. 9, 命題 14)。したがって、$p$ (補題 4) の上に、$A_1 = A' \cap K_1$ の単一の素数イデアル $p_1$ が存在します。 $p'$ と $q'$ が $p$ の上にある $A'$ の 2 つの主要な理想である場合、それらは $p_1$ の上にあります。 $K'$ は $K$ のガロア拡大であり、$A' \cap K$ は一体的に閉じているため (§ 1, no. 2、命題 7 および系から命題 8)、(B) から次のような $\sigma \in \mathscr{G}$ が存在することがわかります。 $(1.p' = q'$; よって (i)。一方、明らかに、分数 $k$、$A_1/p_1$ の体は、$k$ の基数拡大 (A は積分で閉じている) です。 (B) より、$k'$ は $k$ の準ガロア拡張であるため、$k'$ は $k$ の準ガロア拡張であり、$k'$ の $k'$ から代数閉拡大までのすべての $k$ 同型写像は、 $k_1$-同型。この最後の注意は、(B) を考慮して、$k'$ のすべての $k$ 自己同型は形 $\tilde{\sigma}$ であり、$\alpha \in \mathscr{G}^\mathbf{Z}(p')$ で (ii) の証明が完成することも示しています。

*注意*

(2) $K$ が $K$ の *ガロア* 拡大であると仮定し、命題 6 の証明の記法を維持しましょう。すべての $a$ について、$\mathscr{G}_a^\mathbf{Z}$ (それぞれ $\mathscr{G}_a^\mathbf{T}$) を $\mathscr{G}$ のからなる 、$\sigma$ の制限から $A' \cap K$、属するから $\mathscr{G}^\mathbf{Z}(p' \cap K_\alpha)$ の部分群とします。 $\mathscr{G}^\mathbf{T}(p' \cap K_\alpha)$）。 The proof of Proposition 6 shows that these subgroups are *closed* in $\mathscr{G}$ and that
$$
\mathscr{G}^\mathbf{Z}(p') = \bigcap_a \mathscr{G}_a^\mathbf{Z} \quad \text{and} \quad \mathscr{G}^\mathbf{T}(p') = \bigcap_a \mathscr{G}_a^\mathbf{T}.
$$
Moreover, the set of restrictions to $A' \cap K$, of the elements of $\mathscr{G}$ (resp. $\mathscr{G}_a^\mathbf{T}$) is the whole of the group $\mathscr{G}^\mathbf{Z}(p' \cap K_\alpha)$ (resp. $\mathscr{G}^\mathbf{T}(p' \cap K_\alpha)$), every $K$-automorphism of $K$, extending to an element of $\mathscr{G}$.

同じ仮説により、環 $A^\mathbf{Z}(p')$ (それぞれ $A^\mathbf{T}(p')$) は、$A^\mathbf{Z}(p' \cap K_\alpha)$ (それぞれ $A^\mathbf{T}(p' \cap K_\alpha)$) の有向族の *和集合* です。実際、$x \in A^\mathbf{Z}(p')$ごと (それぞれ$x \in A^\mathbf{T}(p')$ごと) 属するから$K$の1つまでであり、上記により、$\mathscr{G}^\mathbf{Z}(p')$の元のうち$K_\alpha \subset K_\beta$と制限から$A' \cap K$のような$\beta$が存在します。 $\mathscr{G}^\mathbf{T}(p')$) は、$\mathscr{G}^\mathbf{Z}(p' \cap K_\beta)$ の元 (それぞれ $\mathscr{G}^\mathbf{T}(p' \cap K_\beta)$) の制限から $A' \cap K$ と同じで、群 $\mathscr{G}^\mathbf{Z}(p' \cap K_\alpha)$ と $\mathscr{G}^\mathbf{T}(p' \cap K_\beta)$ は有限です。したがって、$x$ 属するから $A^\mathbf{Z}(p' \cap K_\beta)$ (それぞれ $A^\mathbf{T}(p' \cap K_\beta)$) となります。

#### 系 1 {#ac-v-s2-prop-6-cor-1 .statement tag=04QE}

*命題 6 の仮説の下で、f を A から体 L までの準同型とし、g_1、g_2 は A' から L までの 2 つの準同型から拡大する f とします。この場合、$g_1 = g_2 \circ \sigma$* となるような K 自己同型 $\sigma \in K'$ が存在します。

命題6から始まる証明は、後者から始まる系から定理2までと同じです。

#### 系 2 {#ac-v-s2-prop-6-cor-2 .statement tag=04QF}

*A を積分閉領域、K を分数の体、K' を K の有限代数拡大、A' を K' 含む A の有限代数部分環とし、A 上の積分とする。

(i) $\mathfrak{p}$ の上にある$A'$ の素イデアルの$A$ 集合のすべての素イデアル $\mathfrak{p}$ は有限です。
(ii) $\mathfrak{p}'$ が $\mathfrak{p}$ の上にある $A'$ の主要な理想である場合、$A'/\mathfrak{p}'$ のすべての元は、$A/\mathfrak{p}$ の分数の体を超える次数 $\leq [\mathbf{K}':\mathbf{K}]$ になります。

(i) $K''$ を、$K'$ の代数閉包の $K'$ と $K''$ の $A$ の積分閉包$A''$ によって生成される $K$ の準ガロア拡張とします。 体 $K''$ は、$K$ (代数、章 V, § 6, no. 3、系 1 ～ 命題 9) の有限拡大であるため、$K$ 自己同型の群は次のようになります。有限;したがって、$\mathfrak{p}$ の上にある$A''$ の素イデアルのうち集合は有限であることがわかります (命題 6 (i))。 On the other hand, as $A''$ is integral over $A$, the mapping $\mathfrak{p}'' \mapsto \mathfrak{p}'' \cap A'$ of the set of prime ideals of $A''$ lying above $\mathfrak{p}$ to the set of prime ideals of $A'$ lying above $x$ is surjective (no. 1, Theorem 1).

(ii) 元 $x' \in A'$ 属する ～ $A$ ($§ 1$、no. 3、系 ～ 命題 10) の最小多項式 ($K$ 以上) の係数。この多項式の適用標準準同型 $\pi': A' \to A'/\mathfrak{p}'$ ～ 係数に対して、$A/\mathfrak{p}$ の係数と次数 $\leq [\mathbf{K}':\mathbf{K}]$ の積分依存関係式が類 mod に対して得られます。 $x$中$\mathfrak{p}'$; よって結論。

#### 系 3 {#ac-v-s2-prop-6-cor-3 .statement tag=04QG}

仮説と系 2 の記法により、$A$ が準局所的であれば、$A'$ も準局所的です。

$A'$ の各最大理想 $m'$ に対して、$m' \cap A$ は $A$ (no. 1, 命題 1) の最大理想です。 仮定集合までに $A$ の最大理想が有限であるため、系 2 から系が続きます。

#### 系 4 {#ac-v-s2-prop-6-cor-4 .statement tag=04QH}

Let $A$ be an integrally closed domain, $K$ its field of fractions, $K$ a Galois extension of $K$, $A'$ the integral closure of $A$ in $K'$, $\mathfrak{p}'$ a prime ideal of $A$, $\mathfrak{p} = A \cap \mathfrak{p}'$ and $k$ and $k'$ the fields of fractions of $A/\mathfrak{p}$ and $A'/\mathfrak{p}'$ respectively. それから：

(i) $A^{\mathbf{Z}}/(\mathfrak{p}' \cap A^{\mathbf{Z}})$の分数の体は$k$に等しく、$\mathfrak{p}' \cap A^{\mathbf{Z}}$に対する$A^{\mathbf{Z}}$の局所環の最大理想は$\mathfrak{p}$によって生成されます。

(ii) $A^T/(\mathfrak{p}' \cap A^T)$の分数$k^T$の体は、$k'$に含まれる$k$の最大の分離拡大です。

環 $A$ は、$K$ に対する $K'$ のガロア群の $A'$ における不変式の環です。 $K'$ が $K$ 上の有限次数である場合、系は命題から no. 2 の 4 と 5 になります。 Consider now the general case, $K'$ therefore being the union of a right directed set $(K_i)$ of finite Galois extensions of $K$. それから：

(i) If $x, y$ are two elements of $A^{\mathbf{Z}}$, where $y \notin \mathfrak{p}'$, there is an index $\alpha$ such that $x$ and $y$ belong to $A^{\mathbf{Z}}(\mathfrak{p}' \cap K_{\alpha})$ (Remark 2); by Proposition 4 of no. 2, there are $x_0, y_0$ in $A$ with $y_0 \notin \mathfrak{p}'$ such that $xy_0 - x_0y \in \mathfrak{p}'$, which proves the first assertion of (i); if further $x \in \mathfrak{p}'$, we may assume that $y_0$ satisfies
$$
xy_0 \in \mathfrak{p}A^{\mathbf{Z}}(\mathfrak{p}' \cap K_{\alpha}) \subset \mathfrak{p}A^{\mathbf{Z}}(\mathfrak{p}'),
$$
which proves the second assertion of (i).

(ii) 今、$x \in A^T$ だと仮定します。 $x \in A^T(p' \cap K_\alpha)$ (注意 2) および no. 2 の命題 5 が存在する $\alpha$ は、$x \mod.(p' \cap K_\alpha \cap A^T)$ の類 $\bar{x}$ が代数的であり、$k$ 上で分離可能であることを示しています。 *なおさら* 類 $x$ の $\mod.(p' \cap A^T)$ は $k$ で分離可能です。 系の証明を完成するには、$k'$ が $k^T$ の *根長* 拡大であることを示すだけで十分です。さて、$k'$ は、分数の体環 $(A' \cap K_\alpha)/(p' \cap K_\alpha)$ の$k_\alpha$ の右指向家族の和集合です。したがって、命題 5 から、$k'$ 属するから $k$ の元が、分数の体より根長であることがわかります。

$$
A^T(p' \cap K_\alpha)/(p' \cap A^T(p' \cap K_\alpha))
$$

そして *なおさら* が $k^T$ を超えます (注意 2 により)。

#### 定義 5 {#ac-v-s2-def-5 .statement tag=04QI}

*With the hypotheses and notation of Proposition 6, the field of invariants $K^Z(p')$ (resp. $K^T(p')$) of the group $G^Z(p')$ (resp. $G^T(p')$) in the field $K'$ is called the decomposition field* (resp. *inertia field*) *of $p'$ with respect to $K$*.

また、$K^Z(p')$ (それぞれ $K^T(p')$) の代わりに $K^Z$ (それぞれ $K^T$) と書きます。 § 1, no. 9、命題 23 から、$K^Z$ (それぞれ $K^T$) は、環 $A^Z$ (それぞれ $A^T$) の分数* の体であることがわかります。 $A^Z$ (それぞれ $A^T$) は、$K^Z$ (それぞれ $K^T$) の $A$ の積分閉包です。

*注意*

(3) 命題 6 の系 4 の条件の下で、$[K':K]$ が *有限* であると仮定すると、$p$ の上にある個別の素イデアルの数は $[K^Z:K]$ であり、この次数は添字に等しい('3:*G*Z*) by ガロア理論;さらに、ガロア理論から次のようになります。

$$(6)$$
$$
[K^T:K^Z] = (G^Z:G^T) = [k^T:k].
$$

(4) Let $A$ be an integrally closed domain, $K$ its field of fractions, $K'$ a *finite* algebraic extension of $K$ and $A'$ the integral closure of $A$ in $K'$. 次に、$A$ のすべての素イデアル $p$ について、 *数* $\&$ *素イデアル* $\&$ *の* $A'$ *上にある* $p$ *最大でも* $[K':K]_s$ (可分な因子の次数 ) $K$ over $K$). We may first restrict our attention to the case where $K$ is a separable extension of $K$, for in general $K$ is a radicial extension of the greatest separable extension $K_0$ of $K$ contained in $K'$, $[K':K]_s = [K_0:K]$ by definition and, if $A$, is the integral closure of $A$ in $K_0$, the prime ideals of $A$, and $A'$ are in one-to-one correspondence (Lemma 4). Suppose therefore that $K$ is separable over $K$ and let $N$ be the Galois extension of $K$ generated by $K$ in an algebraic closure of $K$, $G$ its Galois group, $B$ the integral closure of $A$ in $N$ and $\mathfrak{P}$ a prime ideal of $B$ lying above $p$. Let $\mathscr{H}$ be the Galois group of $N$ over $K$ and $G^Z$ the decomposition group of $\mathfrak{P}$; the prime ideals of $B$ lying above $p$ are the $s.\mathfrak{P}$ where $s \in G$ (no. 2, Theorem 2) and the relation $s.\mathfrak{P} = s'.\mathfrak{P}$ means that $s' = sg$ where $g \in G^Z$. 一方、$s.\mathfrak{P} \cap K' = s'.\mathfrak{P} \cap K'$の位数では、$t \in \mathscr{H}$(no. 2、定理2)、よって、最後に$s' = tsg$、$t \in \mathscr{H}$と$g \in G^Z$が$s'.\mathfrak{P} = ts.\mathfrak{P}$であることが必要十分です。 したがって、$p$の上にある$A'$の素イデアルの数は、同値関係*の下にある$G$の類の*数に等しい。「$s$の間に$s' = tsg$となるような$t \in \mathscr{H}$と$g \in G^{\mathbf{Z}}$が存在する」そして$s'$;明らかに、この数は、$G$ の $\mathscr{H}$ の右剰余類の添字 $(G : \mathscr{H})$、数、およびガロア理論による $(G : \mathscr{H}) = [K' : K]$ に等しくなります。

#### 命題 7 {#ac-v-s2-prop-7 .statement tag=04QJ}

*$A$ を積分閉領域、$K$ を分数の体、$K'$ ガロア拡大を $K$、$\mathscr{G}$ をガロア群、$A'$ を $A$ の積分閉包とします。 $K'$、$p'$ は $A'$ と $p = A \cap p'$ の主要な理想です。 最後に、$L$ を $K'$ 含む $K$ の部分体とし、$p(L) = p' \cap L$ とします。

(i) *分解体* (*慣性体*) *$L$ に対する $p'$ は $L(K^{\mathbf{Z}})$ (それぞれ $L(K^T)$); ※さらに$L$が$K$のガロア拡大であれば、$K$に対して$p(L)$の分解体は$L \cap K^{\mathbf{Z}}$となります。

(ii) *$L$ が$K^{\mathbf{Z}}$、$A/p$、$(A' \cap L)/p(L)$ が分数の体と局所環 $A' \cap L$ 対応するに素理想$p(L)$ が含まれている場合、最大理想は次のように生成されます。 $p$。逆に、この2つの条件が成り立ち、さらに$\bigcap_{n > 0} p^n A'_p = 0$が成立すれば、$K^{\mathbf{Z}}$の中に$L$が含まれます。

(i) If $\mathscr{H}$ is the subgroup of $\mathscr{G}$ leaving invariant the elements of $L$, clearly the decomposition group (resp. inertia group) of $p'$ with respect to $L$ is $G^{\mathbf{Z}} \cap \mathscr{H}$ (resp. $G^T \cap \mathscr{H}$) and the first assertion follows from Galois theory if $K'$ is a *finite* Galois extension of $K$ (*Algebra*, Chapter V, § 10, no. 6, Corollary 1 to Theorem 3); in the general case it follows from the fact that $A^{\mathbf{Z}}$ (resp. $A^T$) is the union of the $A^{\mathbf{Z}}(p' \cap K_\alpha)$ (resp. $A^T(p' \cap K_\beta)$) in the notation of *Remark 2*: every element $x \in K'$ belongs to some $K$, and if it is invariant under $G^{\mathbf{Z}}(p') \cap \mathscr{H}$ (resp. $G^T(p') \cap \mathscr{H}$) it is also invariant under $G^{\mathbf{Z}}(p' \cap K_{\beta'}) \cap \mathscr{H}$ (resp. $G^T(p' \cap K_{\beta'}) \cap \mathscr{H}$) for some suitable $\beta'$; hence it belongs by the beginning of the argument to

$$
L(K^{\mathbf{Z}}(p' \cap K_{\alpha})) \subset L(K^{\mathbf{Z}}) \quad (\text{resp. } L(K^T(p' \cap K_{\beta})) \subset L(K^T)).
$$

ここで、$L$ が $K$ のガロア拡大であると仮定します。すべての $\sigma \in G^{\mathbf{Z}}$ の $L$ から制限は、$p(L) = p' \cap L$ を不変のままにし、したがって $K$ に関して $p(L)$ の属するから分解群は変わりません。逆に、$\tau$ をこの群に対する $L$ 所属の自己同型とし、$\sigma$ を $K'$ の $K$ 自己同型に対する $\tau$ の拡大とする。 $q' = \sigma.p'$と書きます。 $p'$ と $q'$ は両方とも $p(L)$ の上にあるため、$q' = \rho.p'$、よって $\rho^{-1}\sigma \in G^{\mathbf{Z}}$、$\tau$ が$\rho^{-1}\sigma$ の制限となるような自己同型 $\rho \in \mathscr{H}$ が存在します。 $L$;その他、$K$ に対する $p(L)$ の語分解群は、自己同型 $\sigma \in G^{\mathbf{Z}}$ の制限から $L$ の群と同一であることが証明されます。 主張。

(ii) $L \subset K^{\mathbf{Z}}$ は、$[K':K]$ が有限である場合、(ii) の $\mathscr{H} \supset G^{\mathbf{Z}}$ と主張は、no. 2、命題 4 (ii) および (iii) の特殊な場合であることを意味します。一般的なケースでは、議論は命題 6 の証明のようになります。

### 4. 第二の存在定理

#### 定理 3 {#ac-v-s2-thm-3 .statement tag=04QK}

$A$ を積分閉領域とし、$A'$ 環含む $A$ を積分し、$A$ について積分します。 $0$ が $A$ の唯一の元であり、これは $A'$ の $0$ の因子であるとします。 $p, q$ を、$q \supset p$ と $q'$ が $q$ の上にある $A$ の主イデアルとなるような、$A$ の 2 つの主イデアルであるとします。そして、$p$の上に$A$の主要な理想$p'$が存在し、そのような$q' \supset p'$が存在します。

まず、$A'$ が整域であると仮定します。 $K, K'$ をそれぞれ $A$ と $A'$ の分数の体とします。 $K''$ を $K$ の代数閉包と $K''$ の $A$ の積分閉包$A$ とします。次に$A \subset A' \subset A''$。 $p''$ を $p$ (no. 1, 定理 1) の上にある $A''$ の主理想とし、$q''$ を $q$ の上にある $A''$ の主理想とし、$p'' \subset q''$ (no. 1, 系 2 から定理 1)、そして最後に $q_1''$ は $q'$ (no. 1、定理 1) の上にある $A''$ という主要な理想です。 no. 3, 命題 6 (i) により、$Q.q'' = q_1''$ となるような $K''$ の $K$ 自己同型 $\sigma$ が存在します。その場合、$Q.p''$ は $p$ の上にある $A''$ の主イデアルであり、$Q.p'' = q_1''$ となるため、$p' = A' \cap \sigma.p''$ は$p$ の上にあり、$A' \cap q_1'' = q'$ に含まれる$A'$ の主イデアルになります。

一般的なケースに移ります。 $A$ は整域で、$q'$ は素数であるため、部分集合 $A - \{0\}$ と $A'$ の $A' - q'$ は乗法です。 then their 積 $S = (A - \{0\})(A' - q')$ is a multiplicative 部分集合 of $A'$ which does not 含む 0 since the non-zero 元 of $A$ are not 因子 of 0 in $A'$. Then there exists (章 II, §2, no. 5, 系 2 to 命題 11) a prime ideal $m'$ of $A'$ 互いに素 from $S$, in other 語 such that $m' \subset q'$ and $m' \cap A = 0$。 $h$ を標準準同型 $A' \to A'/m'$ とします。 $h$ から $A$ の制限は単射なので、$h(A)$ は積分で閉じています。 $m' \subset q'$ のように、$h(q')$ は $h(q)$ の上にある $A'/m'$ の主要な理想です。 since $A'/m'$ is 整域, the first 部分 of 証明 proves that there exists a prime ideal $n'$ of $A'/m'$ such that $n' \cap h(A) = h(p)$ and $h(q') \supset n'$.理想 $p' = h^{-1}(n')$ は、$h$ の $q'$ 含む核以来、$A'$ と $q' \supset p'$ の主要な理想です。 $n' \supset h(p)$、$p' \supset p$として。最後に、$x \in p' \cap A$、$h(x) \in n' \cap h(A) = h(p)$、したがって$x \in p$については、$h$から$A$の制限が単射法であるためです。したがって$p' \cap A = p$。

#### 系 {#ac-v-s2-n4-cor-1 .statement tag=04QL}

定理 3 の $A$ と $A'$ に関する仮説の下で、$p$ を $A$ の主な理想とする。 $p$ の上にある $A'$ の主理想は、$A'$ 含む $pA'$ の主理想の最小の集合 $\mathscr{E}$ の元です。

$p$ の上にある $A'$ の主要な理想は、no. 1、系 1 ～ 命題 1 によって、$\mathscr{E}$ で最小になります。逆に、$q'$ を $\mathscr{E}$ の最小元とします。 $q' \cap A \supset p$、定理 3 は、$p$ の上に$q' \supset p'$ となるような$A'$ の主要な理想$p'$ が存在することを示しています。 $p'$ 含む $pA'$ のように、$q'$ に作成された仮定は、$q' = p'$、したがって $q'$ が $p$ の上にあることを意味します。

\* $V, V'$ を 2 つのアフィン代数多様体とし、$f(V')$ が $V$ 内で密になるように、$V'$ から $V$ までの $f$ 射とします。 $A$ (それぞれ $A'$) を、$V$ (それぞれ $V'$) の写像の環とします。 $f$ が与えられたので、私たちは同一視できる $A$ にサブリング $A'$ を付けました。 $A'$ が $A$ に対して整数であると仮定します。 no. 1の定理 1は、Vの既約部分変種Wごとに、f(W')がWの稠密な部分集合であるようなV'の既約部分変種W'が存在することを示しています。特に、V のすべての点は、V' の既約部分変種の像であり、これは f が全射であることを示しています。同様に、f の制限を V' 写像 W' の各既約部分変種 W' に V の既約部分変種に代入します。 系 2 から定理 1 までの no. 1 は、W と X が W ⊃ X となる V の 2 つの既約部分変種であり、W' が次のような V' の既約部分変種である場合を示します。 f(W') = W の場合、W' に含まれる V' の既約部分変種 X' が存在し、f(X') = X となります。

A が積分的に閉じている場合、V は正常と呼ばれます。 定理 3 は、V が正規である場合、W と X が W ⊃ X のように V の既約部分変種である場合、および X' が次のような V' の既約部分変種である場合を示します。 f(X') = Xの場合、V' 含む X' の部分変種 W' が存在し、f(W') = W となります。 最後に、系から定理 3 は、V が正常で W がV の既約部分変種、f(W') = W となるような V' の既約部分変種 W' は、まさに $\overline{f}(W)$ の既約成分です。

### 練習問題 {#ac-v-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
