---
book: ac
book_title: Commutative Algebra
chapter: II
chapter_title: LOCALIZATION
section: 2
section_title: Rings and modules of fractions
lang: ja
source: ac-i-vii
book_pages: 55-79, 123-136
pdf_pages: 0075-0099, 0143-0156
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF RINGS OF FRACTIONS
      page: 55
      pdf_page: 75
    - "no": 2
      title: MODULES OF FRACTIONS
      page: 60
      pdf_page: 80
    - "no": 3
      title: CHANGE OF MULTIPLICATIVE SUBSET
      page: 64
      pdf_page: 84
    - "no": 4
      title: PROPERTIES OF MODULES OF FRACTIONS
      page: 67
      pdf_page: 87
    - "no": 5
      title: IDEALS IN A RING OF FRACTIONS
      page: 70
      pdf_page: 90
    - "no": 6
      title: NILRADICAL AND MINIMAL PRIME IDEALS
      page: 73
      pdf_page: 93
    - "no": 7
      title: FRACTIONS OF TENSOR PRODUCTS AND HOMOMORPHISM MODULES
      page: 75
      pdf_page: 95
    - "no": 8
      title: APPLICATION TO ALGEBRAS
      page: 77
      pdf_page: 97
    - "no": 9
      title: MODULES OF FRACTIONS OF GRADED MODULES
      page: 78
      pdf_page: 98
statements: 52
exercises: 27
content_sha256: 62715b41a4772b0ab59a8ef97b2c6de10ac8550bcb68242c8279b24c3c7db1dd
translated_from: content/en/ac/II/02_s2_rings_and_modules_of_fractions.md
translation_method: google
source_content_sha256: 463e49262f632d4a137e725a82bdc25960c4aa1e43d83744037d89388a37100c
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: eabc5fe6cb510874272b6f89099e83d717bb8940ac2315d526a7c01df356936e
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 2. 分数の環と加群

### 1. 定義/環/分数

#### 定義 1 {#ac-ii-s2-def-1 .statement tag=045K}

※$A$を環とします。 部分集合 $S$ の $A$ は、$S$ 属するから $S$ までのすべての有限の積 、 元の場合、乗法と呼ばれます。

これは、$S$ 属するから $S$ の 2 つの元の $1 \in S$ のというとその積と同じです。

*例*
(1) $a^n$ のすべての $a \in A$、集合について、$n \in \mathbf{N}$ は$A$ の乗算部分集合です。
(2) $p$を$A$の理想とする。 $A - p$ が $A$ の乗法部分集合になるためには、$p$ が素数であることが必要かつ十分です。
(3) 零の因子ではない、$A$の元の集合は、$A$の乗算部分集合です。

(4) S と T が A の乗法部分集合である場合、積 st の集合 ST (s ∈ S および t ∈ T) は乗法部分集合です。

(5) G を A の乗法部分集合の (関係 ⊂ に関して) 有向集合とします。そのとき、T = ⋃_{S ∈ G} S は、T 属するの任意の 2 つの元をいくつかの部分集合 S ∈ にすると、A の乗法部分集合になります。 G、したがって、彼らの積属するは T になります。

(6) A の乗算部分集合のすべての共通部分は乗算部分集合です。

環 A のすべての部分集合 S に対して、含む S の乗法部分集合が存在します (たとえば A 自体)。これらすべての部分集合のうちの共通部分は、含むSの最小の乗法部分集合です。それは S によって生成されると言われています。直ちに、それが S の元の有限のすべての積の集合からなるであることがわかります。

#### 命題 1 {#ac-ii-s2-prop-1 .statement tag=045L}

A を A の環および S 部分集合とします。以下のプロパティを持つ A から A' の環 A' および準同型 h が存在します。
(1) h(S) の元は A において可逆です。
(2) u(S) の元が B で可逆であるような A から環 B までのすべての準同型 u に対して、u = u' ∘ h となるような A から B までの一意な準同型 u' が存在します。

他の語では、(A', h) は普遍写像問題 (集合理論, 章 IV, § 3, no. 1) の解であり、次の条件: 考慮される構造 Σ の種は、 環、射は環準同型であり、a マッピングは A の準同型から環であり、そのような準同型の下にある S の像は可逆元で構成されます。 (A', h) と (A'_1, h_1) が両方ともこの問題の解である場合、h_1 = j ∘ h となるような一意の同型 j : A' → A'_1 が存在することを思い出してください (上記参照)。

$\overline{S}$ を S によって生成された A の乗算部分集合とします。明らかに、上記の普遍写像問題のすべての解は、置き換えること S によって $\overline{S}$ によって得られる普遍写像問題の解でもあり、その逆も同様です。

集合 A × S において、 元 (a, s), (a', s') の間にある次の関係を考えてみましょう。

(1) 「t (sa' − s'a​​) = 0 となる t ∈ $\overline{S}$ が存在する」。

この関係は同値関係です。これは明らかに再帰的で対称的です。これは推移的です。t (sa' − s'a​​) = 0 および t'(s'a'' − s''a') = 0 の場合、tt's'(sa' − s'a​​) = 0 および tt's' ∈ $\overline{S}$ です。この同値関係の下で、A'をA×$\overline{S}$の商集合とします。順序付けされたすべての対 (a, s) ∈ A × $\overline{S}$ について、A の (a, s) の a/s 標準像で表し、すべての a ∈ A に対して集合 h(a) = a/1 となります。順序付けられた対が成り立つように A' が環構造与えられることがわかります。 (A', h) は問題を解きます。

x = a/s および y = b/t を A' の 2 元とします。 元 (ta + sb)/st と $ab/st$ は $x$ と $y$ にのみ依存します。なぜなら、$x = a'/s'$ の場合、仮定 $r \in \overline{S}$ までに $r(s'a - sa') = 0$、よってが存在します。

$$
r(s't(ta + sb) - st(ta' + s'b)) = 0
$$

そして$r(s'tab - sta'b) = 0$。 It is easily verified that the laws of composition $(x, y) \mapsto x + y = (ta + sb)/st$ and $(x, y) \mapsto xy = ab/st$ define a commutative ring structure on $\mathbf{A}'$, under which $0/1$ is the identity element under addition and $1/1$ is the unit element. さらに、$h$ が環準同型であり、すべての $s \in S$ に対して、$s/1$ が $\mathbf{A}'$ で可逆であり、その逆が $1/s$ であることは、明らかです。 最後に、$B$ を環および $u : \mathbf{A} \to B$ 準同型として、元 $u(S)$ が $B$ で反転可能であるようにします。そのような一意な写像 $u' : \mathbf{A}' \to B$ が存在します

(2)
$$
u'(a/s) = u(a)(u(s))^{-1} \quad (a \in \mathbf{A}, s \in \overline{S}).
$$

$a/s = a'/s'$ の場合、$t(sa' - s'a) = 0$、よって $u(t)(u(s)u(a') - u(s')u(a)) = 0$、そして$u(t)$、$u(s)$、$u(s')$ が反転可能な$u(a)(u(s))^{-1} = u(a')(u(s'))^{-1}$ となるような $t \in \overline{S}$ が存在します。 $u'$ が加法と乗法に関して準同型であることは簡単に検証されます。最後に、明らかに $u' \circ h = u$ と $u'$ は、この関係の準同型満たすだけです。

$$
u'(a/s) = u'((a/1)(1/s)) = u'(1/s)u'(a/1) = u'(1/s)u(a)
$$

と $1 = u'(1/1) = u'(s/1)u'(1/s) = u(s)u'(1/s)$、よって公式 (2)。

#### 定義 2 {#ac-ii-s2-def-2 .statement tag=045M}

$\mathbf{A}$ を $\mathbf{A}$ の環、$S$ 部分集合、および $S$ によって生成された乗算部分集合を$\overline{S}$ とします。 The ring of fractions of $\mathbf{A}$ defined by $S$ and denoted by $\mathbf{A}[S^{-1}]$ is the quotient set of $\mathbf{A} \times \overline{S}$ under the equivalence relation (1) with the ring structure defined by

$$
(a/s) + (b/t) = (ta + sb)/st, \qquad (a/s)(b/t) = (ab)/(st)
$$

$\mathbf{A}$の$a, b$、$\overline{S}$の$s, t$。 $\mathbf{A}$ から $\mathbf{A}[S^{-1}]$ の標準写像は準同型 $a \mapsto a/1$ で、$\mathbf{A}[S^{-1}]$ は $A$ 代数になります。

この章では、通常、この標準写像を $i_A^S$ で表します。 命題 1 の証明は、注文された対 $(\mathbf{A}[S^{-1}], i_A^S)$ がこの命題の主張の条件を満たすことを示します。

**注意**

(1) 明らかに$\mathbf{A}[\overline{S}^{-1}] = \mathbf{A}[S^{-1}]$。

(2) Two elements of $\mathbf{A}[S^{-1}]$ can always be written in the form $a/s$ and $a'/s$ ($a, a'$ in $\mathbf{A}$, $s \in \overline{S}$) with the *same* "denominator" $s$, for if $b/t$ and $b'/t'$ are two elements of $\mathbf{A}[S^{-1}]$, then $b/t = bt'/tt'$ and $b'/t' = b't/tt'$.

(3) The kernel of $i_A^S$ is the set of $a \in A$ such that there exists $s \in \overline{S}$ satisfying $sa = 0$; for $i_A^S$ to be injective, it is necessary and sufficient that $S$ contain no divisor of zero in $A$.

(4) $S$ 含む冪零元の場合、$0 \in \overline{S}$ と環 $A[S^{-1}]$ は 0 に減らされます。これは定義 2 から簡単にわかります。

(5) $i_A^S$ が全単射であるためには、すべての元 $s \in S$ が $A$ で可逆であることが必要かつ十分です。 $s/1$ は $A[S^{-1}]$ で可逆であるため、条件は明らかに必要です。すべての $t \in \overline{S}$ について、$t$ は $A$ で、$a/t = at^{-1}/1$ は $A[S^{-1}]$ で反転可能であるため、これで十分です。したがって、$i_A^S$ は全射法であり、それが単射法であることは注意 3 ですでに見られました。次に、$A$ と $A[S^{-1}]$ が $i_A^S$ によって識別されます。

例 (7)。 $R$ が 0 の因子ではない、$A$ の元の集合である場合、環 $A[R^{-1}]$ は、まさに $A$ の分数の環 (代数, 章 I, §9, no. 4);混乱を避けるために、私たちはこれを、$A$の分数の合計環と呼ぶことにします。特に、$A$ が整域である場合、$A[R^{-1}]$ は $A$ の分数の体です (上記参照)。

#### 命題 2 {#ac-ii-s2-prop-2 .statement tag=045N}

$A, B$ を 2 つの環、$A$ の $S$ 部分集合、$B$ の $T$ 部分集合、$A$ から $B$ までの $f$ 準同型とします。それは$f(S) \subset T$です。 $A[S^{-1}]$ から $B[T^{-1}]$ までの一意な準同型 $f'$ が存在し、すべての $a \in A$ に対して $f'(a/1) = f(a)/1$ になります。

さらに、$f(S)$ によって生成された $B$ の乗法部分集合に $T$ が含まれているとします。すると、iff は全射法 (単射法) なので、$f'$ も同様です。

最初の主張は、一意な準同型 $f': A[S^{-1}] \to B[T^{-1}]$ が存在するというとなり、可換図式が得られます。

$$
\begin{array}{ccc}
A & \xrightarrow{f} & B \\
i_A^S \downarrow & & \downarrow i_B^T \\
A[S^{-1}] & \xrightarrow{f'} & B[T^{-1}]
\end{array}
$$

ここで、関係 $f(S) \subset T$ は、すべての $s \in S$ に対して $i_B^T(f(s))$ が $B[T^{-1}]$ で反転可能であり、命題を適用する 1 から $i_B^T \circ f$ までで十分であることを意味します。 (2) から簡単に次のことがわかります。すべての $a \in A$ と $s \in \overline{S}$ ($S$ によって生成される $A$ の乗算部分集合) について、

$$
f'(a/s) = f(a)/f(s).
$$

$T$ が $f(S)$ によって生成された乗法部分集合に含まれているとします。これは正確には $f(\overline{S})$ です。次に、(3) から、 iff が全射法であれば、 $f'$ も全射法であることがわかります。

ここで、$f$ が単射法であると仮定します。 $a/s$ を核の元にします。 $T$ によって生成される乗法部分集合は $f(\overline{S})$ であるため、$f(s_1)f(a) = 0$、よって $f(s_1a) = 0$ となる元 $s_1 \in \overline{S}$ があり、$f$ は単射なので結果として $s_1a = 0$ になります。次に $a/s = 0$ ですが、これは $f'$ が単射であることを証明します。

注意 (6)。 $T$の元が$B$で可逆である場合、$B[T^{-1}]$は同型$i_B^T$および$f'$によって$B$と同一視され、$A[S^{-1}]$の一意な準同型$u'$と同一になります。 $B$ は $u' \circ i_A^S = f$ になります。

#### 系 1 {#ac-ii-s2-prop-2-cor-1 .statement tag=045O}

*$A$ を $A$ の環、$S$ 部分集合、および $A$ から環 $B$ の $u$ 単射準同型とし、$u(S)$ の元が反転可能であるようにします。 $B$。 $A[S^{-1}]$ から $B$ までの一意な準同型 $u'$ は、$u' \circ i_A^S = u$ が単射法になります。*

これは、命題 2 と注意 6 の明らか帰結です。

#### 系 2 {#ac-ii-s2-prop-2-cor-2 .statement tag=045P}

*$A$を環、$S$、$T$に$A$の2つの部分集合を加えて$S \subset T$とします。 $A[S^{-1}]$ から $A[T^{-1}]$ までは $i_A^T = i_A^{T,S} \circ i_A^S$ となる一意な準同型 $i_A^{T,S}$ が存在します。*

すべての $a \in A$、$i_A^{T,S}$、次に $A[S^{-1}]$ の写像元 $a/s$ から $A[T^{-1}]$ の元 $a/s$ です。

注意 (7)。 $i_A^T$ が単射であれば、$i_A^{T,S}$ (系 1) も単射であることに注意してください。 This is what happens if $T$ is the set $R$ of elements of $A$ which are not divisors of 0; then it is possible to identify $A[S^{-1}]$ with the subring of the total ring of fractions $A[R^{-1}]$ generated by $A$ and the inverses in $A[R^{-1}]$ of the elements of $S$.

#### 系 3 {#ac-ii-s2-prop-2-cor-3 .statement tag=045Q}

*$A, B, C$ を 3 つの環、$S$ (それぞれ $T, U$)、$A$ (それぞれ $B, C$)、$f : A \to B$、$g : B \to C$ 2 つの準同型と $h : A \to C$ の乗算部分集合とします。 準同型 $g \circ f$; $f(S) \subset T$、$g(T) \subset U$ だとします。 $f' : A[S^{-1}] \to B[T^{-1}]$、$g' : B[T^{-1}] \to C[U^{-1}]$、$h' : A[S^{-1}] \to C[U^{-1}]$ 準同型対応するから $f, g, h$ とします。その後、$h' = g' \circ f'$.*

これは定義から簡単に続きます。

特に、$S, T, U$ が $S \subset T \subset U$ となるような $A$ の 3 つの乗算部分集合である場合、$i_A^{U,S} = i_A^{U,T} \circ i_A^{T,S}$ になります。

#### 系 4 {#ac-ii-s2-prop-2-cor-4 .statement tag=045R}

*$S$ を環 $A$ の部分集合、$A[S^{-1}]$ 含む $i_A^S(A)$ および $S'$ 集合 $i_A^S(A)$ の $B$ 部分環とします。 $j$ を $B$ の標準単射から $A[S^{-1}]$ にします。 一意な準同型 $g$ $B[{S'}^{-1}]$ から $A[S^{-1}]$ まで、$g \circ i_A^S = j$ は同型となります。*

写像 $g$ は系 1 による単射です。 環 $g(B[{S'}^{-1}])$ 含む $i_A^S(A)$ および $S'$ の元の逆数。したがって、それは $A[S^{-1}]$ に等しくなります。

If $A$ is an integral domain and $0 \notin S$, the notation $A[S^{-1}]$ agrees with that of Algebra, Chapter IV, § 2, no. 1; also, if $S$ is multiplicative, $A[S^{-1}]$ coincides in this case with the set denoted by $S^{-1}A$ in Algebra, Chapter I, § 1, no. 1.

As an extension of notation, for any multiplicative subset $S$ of a ring $A$, we henceforth denote by $S^{-1}A$ the ring of fractions $A[S^{-1}]$. $S$ が $A$ の素イデアル $p$ の補数である場合、$S^{-1}A$ の代わりに $A$ と書きます。

$A$ が整域および $0 \notin S$ の場合、$S^{-1}A$ は常に $A$ の分数、含む $A$ (注意 7) の体の部分環と識別されます。

### 2. 分数中加群

no. 1 で定義された標準準同型 $i_A^S : A \to A[S^{-1}]$ により、すべての $A[S^{-1}]$ モジュールを $A$ モジュールとみなすことができます。

#### 命題 3 {#ac-ii-s2-prop-3 .statement tag=045S}

$A$ を $A$ の環、$S$ 部分集合、$M$ を $A$ モジュール、$M'$ を $A$ モジュール $M \otimes_A A[S^{-1}]$ および $f$ を標準とします。 $M$ から $M'$ の $A$-準同型性 $x \mapsto x \otimes 1$。次に:
(1) $s \in S$、$M'$ のホモテティー $z \mapsto sz$ はすべて全単射です。
(2) すべての $s \in S$、$N$ のホモテティー $y \mapsto sy$ が全単射であり、$M$ から $N$ のすべての準同型 $u$ が存在するような、すべての $A$ 加群 $N$ について、 $M'$ から $N$ までの一意な準同型 $u'$ は、$u = u' \circ f$ になります。

他の語では、$(M', f)$ は普遍的な写像問題 (集合理論、章 IV, § 3, no. 1) の解で、次の条件: 構造の種です。 $\Sigma$ は、$S$ の元によって引き起こされる相似性が全単射である $A$ 加群のものであり、射は $A$ 加群準同型であり、$a$ マッピングも$A$-モジュール準同型。

すべての $A$ モジュール $N$ とすべての $a \in A$ について、$N$ の $h_a$ ホモテティー $y \mapsto ay$ で表します。 $a \mapsto h_a$ は、$A$ から $\operatorname{End}_A(N)$ までの環準同型になります。 $h_a$ が全単射であるということは、$h_a$ が $\operatorname{End}_A(N)$ の可逆元であることを意味します。すべての $s \in S$ に対して、$h_s$ は $\operatorname{End}_A(N)$ で反転可能であると仮定します。 元 $h_a$、$a \in A$、および元 $h_s$ の逆$s \in S$、次に $\operatorname{End}_A(N)$ の生成する 、可換部分環 $B$ および$A$ から $B$ までの準同型 $a \mapsto h_a$ は、$S$ の元のうち像が反転可能です。次に、(no. 1, 命題 1) として、$A[S^{-1}]$ から $B$ までの一意な準同型 $h'$ が存在することがわかります。

$$
h'(a/s) = h_a(h_s)^{-1};
$$

私たちは (代数, 章 II, , no. 14) 、N 上の準同型定義するが $(a/s).y = h_s^{-1}(a.y)$ のような $A[S^{-1}]$ モジュール構造であることを知っています。 A-加群構造は、準同型 $i_A^S$ によってこの $A[S^{-1}]$ モジュール構造から導出され、最初に与えられた構造と正確に一致します。

逆に、N が $A[S^{-1}]$ 加群で、$i_A^S$ によって A-加群とみなされる場合、$s \in S$ の相似関係 $y \mapsto sy$ は全単射であり、$y \mapsto (1/s)y$ は $y \mapsto sy$ の逆写像であるためです。そして、上記のプロセスによってその A-加群構造から導出された N 上の $A[S^{-1}]$ モジュール構造は、最初に与えられた $A[S^{-1}]$ モジュール構造です。したがって、$A[S^{-1}]$加群とA-加群の間には標準的な1対1対応があり、Sの元によって引き起こされる相同性は全単射です。さらに、N、N' が 2 つの A-加群で、この性質すべての A-加群準同型 $u : N \to N'$ も、N と N' の $A[S^{-1}]$ 加群構造の準同型である場合、味方 $\in N$ とすべての $s \in S$ については、 $u(y) = u(s.((1/s)y)) = s.u((1/s)y)$、よって $u((1/s)y) = (1/s)u(y)$と書くことができます。 逆は明らかです。

したがって、命題 3 の主張は、上記の解釈 (代数, 章 II, § 5, no. 1, 注意) を考慮して、スカラーを $A[S^{-1}]$ に拡張することによって M から得られた加群の特徴付けにすぎません。 1)。

#### 定義 3 {#ac-ii-s2-def-3 .statement tag=045T}

Aを環、AのS部分集合、SとM A-加群によって生成されたAの乗算部分集合を$\overline{S}$とします。このとき、S によって定義され、$M[S^{-1}]$ または $\overline{S}^{-1}M$ で示される M の分数の加群は、$A[S^{-1}]$ モジュール $M \otimes_A A[S^{-1}]$ です。

この章では、通常、M の $i_M^S$ 標準写像 $m \mapsto m \otimes 1$ で表します。

**注意**
(1) 明らかに$M[\overline{S}^{-1}] = M[S^{-1}]$。
(2) $m \in M$ と $s \in \overline{S}$ については、 $M[S^{-1}]$ の元 $m \otimes (1/s)$ についても $m/s$ と書きます。 $M[S^{-1}]$ のすべての元は形であり、そのような元は形 $\sum_i m_i \otimes (a_i/s)$ であり、$m_i \in M, a_i \in A, s \in S$ (no. 1, 注意 2)、および

$$
m_i \in 3 (a_i/s) = (a_i m_i) \in 3 (1/s),
$$

従って、$\sum_i m_i \otimes (a_i/s) = m \otimes (1/s)$、ここで$m = \sum_i a_i m_i$です。それから

(4)
$$
(m/s) + (m'/s') = (s'm + sm')/ss'
$$
(5)
$$
(a/s)(m/s') = (am)/(ss')
$$

ここで、$m, m' \in M, a \in A$と$s, s' \in S$です。

(3) S が A の素イデアル p の補数である場合、S^{-1}M の代わりに M_p と書きます。

(4) M を A[S^{-1}] モジュールとする。 M が正準的に A-加群とみなされる場合、M と恒等写像 1 の順序付けられた対からなるに対して、i_M^S は全単射となり、M[S^{-1}] によって解かれた普遍的な写像問題の自明な解でもあり、 i_M^S.この場合、M は M[S^{-1}] で識別されます。

#### 命題 4 {#ac-ii-s2-prop-4 .statement tag=045U}

*S を A と M A-加群の乗算部分集合とします。 m|s = 0 (m \in M, s \in S) の場合、s'm = 0 となる s' \in S が存在することが必要かつ十分です。*

S の s' \in が s'm = 0 である場合、明らかに m|s = (s'm)/(ss') = 0 です。逆に、m|s = 0 であると仮定します。S^{-1}A では 1/s は可逆であるため、m/1 = 0。S^{-1}A 含む 1 のすべてのサブ A 加群 P について、\beta(P, m) で表します。 M \times P から M \otimes_A P の標準写像の下の (m, 1) の像; \beta(S^{-1}A, m) = 0. S^{-1}A 含む 1 の *有限生成* 部分加群 P が存在すること (代数, 章 II, § 6, no. 3, 系 4 ～ 命題 7) が存在することがわかっています。 \beta(P, m) = 0. すべての t \in S について、a/t の A_t 集合で表します。ここで、a \in A; P は有限に生成されるため、P \部分集合 A_t (no. 1, 注意 2), よって \beta(A_t, m) = 0 となるような t \in S が存在します。 写像 A から A_t への \mapsto a/t は全射的です。 Bをその核とします。それは定義する全射法写像 h : M \otimes_A A \to M \otimes_A A_t であり、その核は BM (M は M \otimes A と同一視される) です。 \beta(A_t, m) = h(tm) となり、その結果、tm は形 $\sum_{i=1}^r b_i m_i$ で表すことができます。ここで、b_i \in B、m_i \in M (1 \leq i \leq r) となります。 b_i/t = 0 for 1 \leq i \leq r であるため、 t' b_i = 0 for 1 \leq i \leq r、よって t'tm = 0 となるような t' \in S が存在し、命題 4 が証明されます。

#### 系 1 {#ac-ii-s2-prop-4-cor-1 .statement tag=045V}

* S^{-1}M の m|s = m'|s' の場合、 t(s'm - sm') = 0 となるような t \ が S に存在することが必要かつ十分です。*

$$(m|s) - (m'|s') = (s'm - sm')/ss'.$$

#### 系 2 {#ac-ii-s2-prop-4-cor-2 .statement tag=045W}

※Mを有限生成A-加群とします。 S^{-1}M = 0 の場合、sM = 0 となる s \in S が存在することが必要かつ十分です。*

M に条件がなければ、S の一部の s \in について明らかに関係 sM = 0 は S^{-1}M = 0 を意味します。逆に、S^{-1}M = 0 と仮定し、(m_i)_{1 \leq i \leq n} を M の生成元の系とします。 m_i/1 生成する S^{-1}A-加群 S^{-1}M、従って S^{-1}M = 0 はというに相当し、1 \leq i \leq n に対して m_i/1 = 0 になります。 命題 4 により、$s_i m_i = 0$ となる $s_i \in S$ が存在し、$s = s_1 s_2 \cdots s_n$ を取ると、すべての $i$ に対して $s m_i = 0$ となり、従って $sM = 0$ となります。

#### 系 3 {#ac-ii-s2-prop-4-cor-3 .statement tag=045X}

※Mを有限生成A-加群とします。理想的な $a \& A$ が $aM = M$ となるためには、$(1 + a)M = 0$ となるような $a \in a$ が存在することが必要かつ十分です。

明らかに、関係 $(1 + a)M = 0$ は $M = aM$ を暗示します。 逆を証明するには、次の補題を使用します。

#### 補題 1 {#ac-ii-s2-lem-1 .statement tag=045Y}

*A の各イデアル a について、元 $1 + a$ の集合 S は、$a \in a$ は A の部分集合と、元の $S^{-1}A$ の集合 $a'$ です。 形 $a/s$、$a \in a$ と $s \in S$ は、$S^{-1}A$ のヤコブソン根基に含まれる理想です。

最初の主張は明らかであり、$a'$ が $S^{-1}A$ の理想であるという事実も同様です。一方、S の定義によるすべての $s \in S$ と $a \in a$ に対して $(1/1) + (a/s) = (s + a)/s$ と $s + a \in S$従って、$(1/1) + (a/s)$ はすべての $a/s \in a'$ に対して $S^{-1}A$ で反転可能であり、補題の証明が完成します (*代数*, 章 VIII, § 6, no. 3, 定理 1)。

従って、集合 $N = S^{-1}M$ とすると、明らかに N は有限生成された $S^{-1}A$ 加群です。 $aM = M$なら$a'N = N$、そして中山の補題により$N = 0$になります（*代数*、章VIII, § 6, no. 3、系から命題6）。 系は系 2 から続きます。

#### 命題 5 {#ac-ii-s2-prop-5 .statement tag=045Z}

*A、Bを2つの環、SをAの乗算部分集合、TをBの乗算部分集合、そして$f(S) \subset T$となるようなAからBへのf準同型とする。 M を M から N までの A-加群、N B-加群、u A-線型写像とします。すると、すべての $m \in M$ に対して $u'(m/1) = u(m)/1$ となるような、$S^{-1}M$ から $T^{-1}N$ までの一意の $S^{-1}A$ 線形マッピング $u'$ が存在します。

M から $T^{-1}N$ までの写像 $i_N^T \circ u$ は A-linear です。さらに、$s \in S$ の場合、$f(s) \in T$、したがって、$T^{-1}N$ 上の s によって引き起こされるホモテティー は全単射です。 命題 3 から$u'$ の存在と一意性が続きます。そして、$m \in M$ と $s \in S$ については、

$$
u'(m/s) = u(m)/f(s).
$$

同じ記法で、Cを3番目の環とし、UはCの乗法部分集合、gはBからCまでの準同型で、$g(T) \subset U$、PはCモジュール、vはNからPまでのB-線型写像とします。および $v'$ v に関連付けられた B から $U^{-1}P$ への $T^{-1}B$ 線形マッピング。

$$
(v \circ u)' = v' \circ u'
$$

ここで、左側は A-線型写像 $S^{-1}M \to U^{-1}P$ と $v \circ u$ に関連付けられています。同様に、$u_1$ が M から N への 2 番目の A-線型写像である場合、

$$
(u + u_1)' = u' + u_;
$$

左側は A-線型写像 $S^{-1}M \to T^{-1}N$ が $u + u_1$ に関連付けられています。

注意 (5)。 命題 5 で $B = A, T = S$ と $f = 1_A$ を取ると、$u'$ がちょうど写像 $u \otimes 1 : M \otimes S^{-1}A \to N \otimes S^{-1}A$ であることが簡単にわかります。今後、それを $S^{-1}u$ で表すことにします。 S が A の素イデアル $p$ の補数である場合、$S^{-1}u$ の代わりに $u_p$ と書きます。

#### 命題 6 {#ac-ii-s2-prop-6 .statement tag=0460}

$f$ を環 A から環 B までの準同型とし、S を A の乗算部分集合とします。 $(f(S))^{-1}B$ から $S^{-1}B$ までの一意な写像 j が存在します (ここで、B は $f$ によって A-加群と見なされます)。そのため、すべての $b \in B, s \in S$ に対して $j(b|f(s)) = b|s$ になります。 $f' : S^{-1}A \to (f(S))^{-1}B$ が $f$ (no. 1、命題 2) に関連付けられた環準同型の場合、$j \circ f' = S^{-1}f$ です。 写像 j は、$(f(S))^{-1}B$ の $S^{-1}A$ モジュール構造の同型で、$f'$ によって定義され、$S^{-1}B$ の構造に定義され、また、$(f(S))^{-1}B$ の B-加群構造が$S^{-1}B$ の構造に定義されます (結果として得られるから) 定義 $S^{-1}B = (S^{-1}A) \otimes_A B$）。

$b, b'$ が B にあり、$s, s'$ が S にある場合、系 1 から命題 4 までのように、条件 $b|s = b'|s'$ と $b|f(s) = b'|f(s')$ は同等であり、これは j の存在を確立し、j が全単射であることを示します。 jの一意性は明らかです。明らかに j は加法群同型です。 $a \in A, b \in B, s \in S, t \in S$ の場合、

$$
(a|s).(b|f(t)) = f'(a|s)(b|f(t)) = f(a)|f(s)(b|f(t)) = (f(a)b)|f(st),
$$

ここから、 j は $(S^{-1}A)$ 線形であることがわかります。明らかに$j \circ f^1 = S^{-1}f$。最後に、$b \in B, b' \in B, s \in S$ の場合、$j(b.(b'|f(s))) = j(bb'|f(s)) = bb'|s = b.(b'|s)$ となり、最後の主張が証明されます。

命題 6 の写像 j は、$S^{-1}B$ 上で $(fS)^{-1}B$ の標準同型と呼ばれます。これら 2 つの集合は、一般に $f'$ によって識別されます。次に$f' = S^{-1}f, i_B^S = i_B^{f(S)}$。

### 3. 乗法部分集合の変更

A を環、S を A と M A-加群の乗算部分集合とします。 T が含む S の乗算部分集合である場合、no. 2 の命題 5 から、 i_M^T = i_M^{T,S} \circ i_M^S のような固有の $S^{-1}A$ 線形写像 $i_M^{T,S} : S^{-1}M \to T^{-1}M$ が存在することがわかります。 写像 i_M^{T,S} 写像元 m/s の S^{-1}M から元 m/s の T^{-1}M。 i_M^{T,S} = i_A^{T,S} \otimes 1_M であることは簡単に検証できます。 U が T \部分集合 U となる A の 3 番目の乗法部分集合である場合、 i_M^{U,S} = i_M^{U,T} \circ i_M^{T,S};さらに、u: M \to N が A-加群準同型, 図式の場合

$$
\begin{array}{ccc}
S^{-1}M & \xrightarrow{s^{-1}u} & S^{-1}N \\
i_M^{T,S} \downarrow & & \downarrow i_N^{T,S} \\
T^{-1}M & \xrightarrow{T^{-1}u} & T^{-1}N
\end{array}
$$

可換です。

#### 命題 7 {#ac-ii-s2-prop-7 .statement tag=0461}

A を環とし、S、T を A の 2 つの乗算部分集合とします。集合 T' = i(T_A^S)。

(i) 図式となるような、環 (ST)^{-1}A から環 T'^{-1}(S^{-1}A) までの一意の同型 j が存在します。

$$
\begin{array}{ccc}
A & \xrightarrow{i_A^S} & S^{-1}A \\
i_M^{ST} \downarrow & & \downarrow i_{S^{-1}A}^{T'-1A} \\
(ST)^{-1}A & \xrightarrow{j} & {T'}^{-1}(S^{-1}A)
\end{array}
$$

可換です。

(ii) M をA-加群とします。 There exists an (ST)^{-1}A-isomorphism k from the (ST)^{-1}A-module (ST)^{-1}M onto the T'^{-1}(S^{-1}A)-module T'^{-1}(S^{-1}M) such that the diagram

$$
\begin{array}{ccc}
M & \xrightarrow{i_M^S} & S^{-1}M \\
i_A^{ST} \downarrow & & \downarrow i_{S^{-1}M}^{T'-1M} \\
(ST)^{-1}M & \xrightarrow{k} & {T'}^{-1}(S^{-1}M)
\end{array}
$$

可換です。

(i) (ST)^{-1}A の定義を汎用写像問題の解として使用します。 f(ST) が可逆元で構成されるように、A から B まで B を環 、f 準同型とします。 f(S) は結果的に可逆元から構成されるので、 f = f' \circ i_A^S (no. 1, 命題 1) となる一意な準同型 f': S^{-1}A \to B が存在します。 T のすべての t \について、f'(i_A^S(t)) = f(t) は、B において、hypo-\&\& によって可逆です。従って、f'(T') は可逆元で構成されます。すると、no. 1, 命題 1, 一意な準同型 f'' によって、f'' = f'' \circ i_{S^{-1}A}^{T'} となるような T'^{-1}(S^{-1}A) から B までの f'' が存在します。 よって f = f'' \circ u, 設定 u = i_{S^{-1}A}^{T'} \circ i_S^A。

さらに、$f''_1 : {T'}^{-1}(S^{-1}A) \to B$ が 2 番目の準同型である場合、$f''_1 \circ u = f$、次に $(f''_1 \circ i^{T'}_{S^{-1}A}) \circ i^S_A = (f'' \circ i^{T'}_{S^{-1}A}) \circ i^S_A$、よって $f''_1 \circ i^{T'}_{S^{-1}A} = f'' \circ i^{T'}_{S^{-1}A}$、そしてその結果 $f''_1 = f''$ になります。

${T'}^{-1}(S^{-1}A)$のSTの元の$u$の下の像は可逆であるため、順序付けられた対$({T'}^{-1}(S^{-1}A), u)$は、no. 1で考慮された普遍的な写像問題の解になります。これは$j$の存在と一意性を示しています。

(ii) 証明は (i) と完全に類似しており、この場合は no. 2、命題 3 を使用しており、読者に委ねられています。

#### 命題 8 {#ac-ii-s2-prop-8 .statement tag=0462}

Let A be a ring and S, T two multiplicative subsets of A such that $S \subset T$. 次のプロパティは同等です。

(a) *準同型* $i^{T,S}_A : S^{-1}A \to T^{-1}A$ *は全単射*です。
(b) *すべての A-加群 M に対して、準同型* $i^{T,S}_A : S^{-1}M \to T^{-1}M$ *は全単射*です。
(c) *すべて* $t \in T$ に対して、*$a \in A$ *そのような* $at \in S$ (他の語では、T *割る* 元のすべての元)。
(d) *T を満たすすべての素イデアルは S* を満たす。

$i^{T,S}_A = 1_M \otimes i^{T,S}_A$ は上で見られましたが、これは (a) と (b) の同値を直ちに証明します。 集合 $T' = i^S_A(T)$;すると (命題 7) $T^{-1}A$ は ${T'}^{-1}(S^{-1}A)$ と同一視され、(a) は $T'$ の元が $S^{-1}A$ (no. 1, *注意 5*) で *可逆* であるというというと等価です。 さて、$(t/1)(a/s) = 1/1$($t \in T$,$a \in A, s \in S$)ということは、(a)と(c)の同値を示す$tas' = ss'$となるような$s' \in S$が存在することを意味します。 (d) が (c) を意味することを示します。 $t$ を T の元とし、$t/1$ が $S^{-1}A$ で反転できないと仮定します。その場合、$S^{-1}A$ 含む $t/1$ (*代数*、章 I, § 8, no. 7、定理 2) の最大理想 $m'$ が存在し、$p = (i^S_A)^{-1}(m')$ は含む $t$ の主要理想であり、そうではありません。 S との出会い (S の元の $i^S_A$ の下の像は反転可能であるため)。 Conversely, if there exists a prime ideal $p$ which meets T without meeting S, then no element of $p \cap T$ can divide an element of S; this proves that (c) implies (d) and completes the proof.

It follows from Proposition 8 that, amongst the multiplicative subsets T of A containing S and satisfying the equivalent conditions of Proposition 8, there exists a *greatest*, consisting of *all* the elements of A which divide an element of S (cf. Exercise 1).

#### 命題 9 {#ac-ii-s2-prop-9 .statement tag=0463}

I を、環 A と $S = \bigcup_{\alpha \in I} S_\alpha$ の乗法部分集合の右方向事前順序付け集合、$(S_\alpha)_{\alpha \in I}$ 増加する族とします。 $\alpha \leq \beta$、$\rho_\alpha = i^{S_\alpha, S_\alpha}$ を $\rho_{\beta \alpha} = i^{S_\beta, S_\alpha}_{A^{S_\beta, S_\alpha}}$ と書きます。この場合、$(S_\alpha^{-1}A, \rho_{\beta \alpha})$ は Zings の直接系であり、すべての $\alpha \in I$、$\rho'_\alpha$ が $S_\alpha^{-1}A$ から $\lim \rightarrow S_\alpha^{-1}A$ の標準写像である場合、$\lim \rightarrow S_\alpha^{-1}A$ から $S^{-1}A$ までの一意の同型 $j$ が存在します。すべての $\alpha \in I$ に対して $j \circ \rho'_\alpha = \rho_\alpha$ となるようにします。

$\alpha \leq \beta \leq \gamma$、$\rho_{\gamma \alpha} = \rho_{\gamma \beta} \circ \rho_{\beta \alpha}$ (no. 1、系 3 ～ 命題 2) の場合、$(S_\alpha^{-1}A, \rho_{\beta \alpha})$ は直接系になります。 $A' = \lim \rightarrow S_\alpha^{-1}A$と書きます。 $\alpha \leq \beta$ の $\rho_\alpha = \rho_\beta \circ \rho_{\beta \alpha}$ (no. 1、系 3 ～ 命題 2)、$(\rho_\alpha)$ は準同型の直接系、$j = \lim \rightarrow \rho_\alpha$ は $A'$ から一意な準同型です$S^{-1}A$ は、すべての $a \in I$ に対して $j \circ \rho'_\alpha = \rho_\alpha$ になります。 準同型 $\rho'_\alpha \circ i^{S}_{A^\alpha} : A \to A'$ は、$\rho_{\beta \alpha} \circ i^{S}_{A^\alpha} = i^{S}_{A^\beta}$ と $a \leq \beta$ はすべて等しいです。 $u$ を彼らの共通の値とします。明らかに、$u(S)$ の元は $A'$ で反転可能です。これは、$h \circ i^{S}_{A} = u$ (no. 1, 命題 1) のような準同型 $h : S^{-1}A \to A'$ が存在することを示しています。それから

$$
j \circ h \circ i^{A}_{S} = j \circ u = j \circ \rho'_\alpha \circ i^{A^\alpha}_{S^\alpha} = \rho_\alpha \circ i^{S}_{A^\alpha} = i^{S}_{A}
$$

すべての $\alpha \in I$ にとって、その結果、$j \circ h$ は $S^{-1}A$ のアイデンティティ自己同型となります。一方、$\alpha \in I$の皆さんにとっては、

$$
h \circ j \circ \rho'_\alpha \circ i^{S}_{A^\alpha} = h \circ \rho_\alpha \circ i^{S}_{A^\alpha} = h \circ i^{S}_{A} = u = \rho'_\alpha \circ i^{S}_{A^\alpha},
$$

よって $h \circ j \circ \rho'_\alpha = \rho'_\alpha$ $\alpha \in I$ 全員。従って、$h \circ j$ は $A'$ の同一性自己同型であり、その結果、$j$ は同型になります。

#### 系 {#ac-ii-s2-n3-cor-1 .statement tag=0464}

※命題9の仮説のもと、MをA-加群とします。すべての $\alpha \in I$ に対して $\alpha \leq \beta, f_\alpha = i^{S, S_\alpha}_{M}$ を $f_{\beta \alpha} = i^{S_\beta, S_\alpha}_{M}$ と書き、$f'_\alpha$ を $S_\alpha^{-1}M$ から $\lim \rightarrow S_\alpha^{-1}M$ までの標準写像とします。その場合、すべての $a \in I$ に対して $g \circ f_\alpha = f'_\alpha$ となるような $S^{-1}M$ の $\lim \rightarrow S_\alpha^{-1}M$ への $S^{-1}A$ 同型写像 $g$ が存在します。

系は定義 $S_\alpha^{-1}M = M \otimes_A S_\alpha^{-1}A$ と $S^{-1}M = M \otimes_A S^{-1}A$ の直後であり、極限を直接取るとテンソル積 (*代数*, 章 11, § 6, no. 3, 命題 7) と互換性があるという事実。

### 4. 分数の加群の特性

*この番号全体で、A は環を表し、S は A の乗算部分集合を表します。*

$(M_\alpha, \phi_{\beta \alpha})$ を A-加群の直接系とします。この場合、$(S^{-1}M_\alpha, S^{-1}\phi_{\beta \alpha})$ は $S^{-1}A$ モジュールの直接系であり、直接極限をテンソル積 (*代数*, 章 II, § 6, no. 3, 命題 7) と交換できるという事実により、次のことが可能になります。 定義する標準同型

$$
\lim \rightarrow (S^{-1}M_\alpha) \to S^{-1} \lim \rightarrow M_\alpha.
$$

同様に、直和がテンソル積 (代数, 章 II, , no. 7, 命題 7) と通勤するという事実により、すべての家族 $(M_i)_{i \in I}$ に対して定義するが可能になります。 $A$ モジュール標準同型

$$
\bigoplus_{i \in I} S^{-1} M_i \to S^{-1} \bigoplus_{i \in I} M_i.
$$

最後に、$A$ モジュール $M$ が部分加群のファミリー $(N_i)_{i \in I}$ の和である場合、$S^{-1}M$ は $i_M^S(N_i)$ によって生成されたサブ$S^{-1}A$ モジュールのファミリーの和であることに注意します。 Then it follows that, if $M$ is a finitely generated $A$-module (resp. finitely presented $A$-module), $S^{-1}M = S^{-1}A \otimes_A M$ is a finitely generated $S^{-1}A$-module (resp. finitely presented $S^{-1}A$-module).

#### 定理 1 {#ac-ii-s2-thm-1 .statement tag=0465}

*環 $S^{-1}A$ はフラット $A$ モジュール* (章 I, § 2, no. 1、定義 2) です。

$u : M' \to M$ が $A$ モジュールの単射準同型である場合、$S^{-1}u : S^{-1}M' \to S^{-1}M$ が単射であることを確立する必要があります。さて、$m'/s$ ($m' \in M'$, $s \in S$) が $u(m')/s = 0$ である場合、これは $s'u(m') = 0$ (no. 2, 命題 4) または $u(s'm') = 0$ のような $s' \in S$ の存在を意味します。 $u$ は単射なので、$s'm' = 0$、よって $m'/s = 0$ になります。

$S^{-1}A$ がフラットな $A$ モジュールであるという事実により、章 I, § 2 の結果をそれに適用することができます。 In particular:
(1) If $M$ is an $A$-module and $N$ a submodule of $M$, $S^{-1}N$ is canonically identified with a *submodule* of $S^{-1}M$ generated by $i_M^S(N)$ (Chapter I. § 2, no. 3, *Remark 2*); with this identification, $S^{-1}(M/N)$ is identified with $(S^{-1}M)/(S^{-1}N)$ and, if $P$ is a second submodule of $M$, then

$$
S^{-1}(N + P) = S^{-1}N + S^{-1}P, \quad S^{-1}(N \cap P) = S^{-1}N \cap S^{-1}P
$$

(章 I, § 2, no. 6、命題 2)。
(2) $M$ が *有限生成* $A$ モジュールである場合、

$$
S^{-1} \operatorname{Ann}(M) = \operatorname{Ann}(S^{-1}M)
$$

(章 I, § 2, no. 10、系 2 ～ 命題 12)。

#### 命題 10 {#ac-ii-s2-prop-10 .statement tag=0466}

*$M$を$A$モジュールとします。 $S^{-1}A$ モジュール $S^{-1}M$ のすべての部分加群 $N'$ について、$\phi(N')$ を $i_M^S$ の下の $N'$ の逆像とします。次に:*
(i) $S\phi(N') = N'$。

(ii) $M$ のすべての部分加群 $N$ に対して、$M$ の部分加群 $\phi(S^{-1}N)$ は、$sm \in N$ となるような$s \in S$ が存在する$m \in M$ で構成されます。

(iii) $\phi$ is an isomorphism (for the orderings defined by inclusion) of the set of sub- $S^{-1}A$-modules of $S^{-1}M$ onto the set of submodules $Q$ of $M$ which satisfy the following condition:

(MS) $sm \in Q$、$s \in S$、$m \in M$ の場合、$m \in Q$。

明らかに $S^{-1}\phi(N') \subset N'$;逆に、$n' = m/s \in N'$ の場合、$m/1 \in N'$、従って $m \in \phi(N')$、従って $n' \in S^{-1}(\phi(N'))$ になります。 よって (i)。 元 $m \in M$ が $m \in \phi(S^{-1}N)$ となるためには、$m/1 \in S^{-1}N$ が必要かつ十分です。つまり、$m/1 = n/s$ となるような $s \in S$ と $n \in N$ が存在する必要があります。これは、$s'sm = sn \in N$、よってとなるような$s' \in S$ が存在することを意味します (ii)。最後に、関係 $sm \in \phi(N')$ は定義によって $sm/1 \in N'$ と等価であり、$s/1$ は $S^{-1}A$ で可逆であるため、これは $m/1 \in N'$ または $m \in \phi(N')$ を意味し、従って $\phi(N')$ は条件を満たします。 (MS);一方、(ii) から、$N$ が (MS) を満たす場合は、$\phi(S^{-1}N) = N$ となり、(iii) の証明が完了します。

部分加群 $\phi(S^{-1}N)$ は、$S$ に対する $M$ の $N$ の飽和と呼ばれ、部分加群満たす条件 (MS) (したがってそれらの彩度に等しい) は、$S$ に関して飽和していると言われます。 部分加群 $\phi(S^{-1}N)$ は合成準同型の核です

$$
M \xrightarrow{h} M/N \xrightarrow{i_{M/N}^{S}} S^{-1}M/S^{-1}N
$$

ここで、$h$ は図式の可換性から次のように標準準同型です

$$
\begin{array}{ccc}
M & \xrightarrow{h} & M/N \\
i_M^S \downarrow & & i_{M/N}^S \downarrow \\
S^{-1}M & \xrightarrow{s^{-1}h} & S^{-1}M/S^{-1}N
\end{array}
$$

$S$ が素イデアル $p$ の $A$ の補数である場合、$\phi(S^{-1}N)$ は $p$ に対する $M$ の $N$ の飽和とも呼ばれます。

#### 系 1 {#ac-ii-s2-prop-10-cor-1 .statement tag=0467}

$N_1, N_2$ を $A$ モジュール $M$ の 2 つの部分加群とします。 $S^{-1}N_1 \subset S^{-1}N_2$については、$S$に対する$N_1$の彩度が$N_2$の彩度の中に含まれていれば必要十分です。

#### 系 2 {#ac-ii-s2-prop-10-cor-2 .statement tag=0468}

*M がネーター* (それぞれアルティン) *A* モジュールの場合、*S^{-1}M* はネーター (それぞれアルティン) *S^{-1}A* モジュールです。 *特に、環 A がネーター* (それぞれアルティン) の場合、*同様に環 S^{-1}A* になります。

### 5. 分数中環の理想

#### 命題 11 {#ac-ii-s2-prop-11 .statement tag=0469}

*A を環とし、S を A の乗算部分集合とします。S^{-1}A の理想 b' ごとに、b = (i_A^S)^{-1}(b') を b' = S^{-1}b とする。*

(i) *f を標準準同型 A \to A/b とします。 The homomorphism from S^{-1}A to (f(S))^{-1}(A/b) canonically associated with f (no. 1, Proposition 2) is surjective and its kernel is b', which defines, by taking quotients, a canonical isomorphism of (S^{-1}A)/b' onto (f(S))^{-1}(A/b). さらに、A/b から (f(S))^{-1}(A/b) への標準準同型は単射です。*

(ii) *写像 b' \mapsto b = (i_M^S)^{-1}(b') は、S^{-1}A の最大 (それぞれ素数) イデアルの集合に制限されており、この集合を、そうでないものの中で最大である A のイデアルの集合に (包含に関して) 同型となります。 S を満たす (S を満たさない A の主な理想の集合)*

(iii) *q' が S^{-1}A の素イデアルで、q = (i_A^S)^{-1}(q') の場合、分数 A の環の同型が環 (S^{-1}A)_{q'} 上に存在し、これは写像 a/b (a/1)/(b/1)、ここで、a \in A、b \in A - q.*

(i) *(f(S))^{-1}(A/b) は、これら 2 つの加群 (no. 2, 命題 6) の間の標準同型によって S^{-1}(A/b) と同定できます。 完全系列 0 \to b \to A \to A/b \to 0 そして誘導する完全系列*

$$
0 \to S^{-1}b \to S^{-1}A \to S^{-1}(A/b) \to 0
$$

(no. 4, 定理 1) その存在は、b' = S^{-1}b であるという事実を考慮すると、(i) の最初の主張を証明します。 b は S に関して飽和しているため、 条件 a \in A、s \in S、\in b は a \in b を意味します。 A/b の比 s のホモテティー は単射となり、(i) の 2 番目の主張が証明されます。

(ii) まず、関係 b' = S^{-1}A は関係 b \cap S \neq \varnothing と同等であり、後者は S^{-1}A の b' 含む可逆元であるという事実を表していることに注意します。 It follows from no. 4, Proposition 10 (iii) that b' \mapsto b = (i_A^S)^{-1}(b') is an isomorphism (with respect to inclusion) of the set of ideals of S^{-1}A distinct from S^{-1}A onto the set \mathscr{F} of ideals of A not meeting S and satisfying condition (MS) of Proposition 10. b' が最大 (それぞれ素数) の場合、明らかに b' は \mathscr{F} (それぞれ素数) で最大であり、その逆も ((i) によって) なります。 On the other hand, if r is an ideal of A disjoint from S, its saturation r_1 with respect to S is an ideal of A containing t and disjoint from S : for no element $a \in S$ can satisfy $sa \in t$ for some $s \in S$, since it would follow that $sa \in t \cap S$. 私たちは結論する、$A$と$S$の理想のうち$r$が最大であるなら、それは$\mathscr{F}$で最大であると考えています。 同様に、$r$ が$S$ を満たさない素イデアルである場合、no. 4、命題 10 定義の条件 (MS) を満たし、したがって属するから $\mathscr{F}$ を満たします。 これで(ii)の証明は完了です。

(iii) $q'$ が素数であり、$q$ も素数であると仮定します。 集合 $T = A - q$ は、含む $S$、よって $ST = T$ の $A$ の乗算部分集合です。 $T' = i_A^S(T)$と書きます。 no. 3, 命題 7 (i) から、$T^{-1}A = A$ の固有の同型 $j$ が ${T'}^{-1}(S^{-1}A)$ に存在することがわかります。

$$
j(a/b) = (a/1)/(b/1),
$$

ここで、$a \in A$ と $b \in T$ です。一方、$T'$ は明らかに $q'$ を満たしていません。逆に、$a/s \in S^{-1}A$ とします。 $1/s$ は $S^{-1}A$ で可逆であるため、条件 $a/s \notin q'$ は $i_A^S(a) = a/1 \notin q'$、したがって $a \notin q$ と同等です。したがって、$S^{-1}A - q' = S^{-1}T'$ となり、no. 3、${T'}^{-1}(S^{-1}A) = (S^{-1}A)_{q'}$ の 8 が命題となります。

(iii) で定義される同型をカノニカルと呼びます。 If $A$ is an integral domain, the canonical isomorphisms of $A$, and $(S^{-1}A)_{q'}$ onto subrings of the field of fractions $K$ of $A$ have the same image.

#### 注意 {#ac-ii-s2-n5-rem-1 .statement tag=046A}

$A$ から満たす $S^{-1}a = S^{-1}A$ までの理想的な $a$ (または、no. 4、定理 I、$S^{-1}(A/a) = 0$ によって同じことに相当するもの) の場合、定義からすぐに続くように、$a \cap S \neq \varnothing$ であることが必要かつ十分です。

#### 系 1 {#ac-ii-s2-prop-11-cor-1 .statement tag=046B}

$A$ を環とし、$S$ を $A$ の乗算部分集合とします。 $S$ を満たさないものの中で最大となる $A$ のすべての理想 $p$ は素数です。

命題 11 により、$p$ の仮定は $p = (i_A^S)^{-1}(m')$ を意味します。ここで、$m'$ は $S^{-1}A$ の最大理想です。 $m'$ は素数であるため、$p$ も素数です。

#### 系 2 {#ac-ii-s2-prop-11-cor-2 .statement tag=046C}

Let $A$ be a ring and $S$ a multiplicative subset of $A$. $A$ のすべての理想 $a$ が $S$ を満たさない場合、主要な理想含む $a$ が存在し、$S$ を満たさないものとなります。

$S^{-1}a \neq S^{-1}A$ (注意) であるため、$S^{-1}A$ 含む $S^{-1}a$ (代数、章 I, § 8, no. 7、定理 2) の最大理想が存在し、命題 11 (ii) から系が続きます。

#### 系 3 {#ac-ii-s2-prop-11-cor-3 .statement tag=046D}

$A, B$ を 2 つの環、$\rho$ 準同型 $A$ から $B$ 、$p$ を $A$ の主要な理想とします。 $\overline{\rho}^{-1}(p') = p$ となるような$B$ の主要な理想 $p'$ が存在するには、$\overline{\rho}^{-1}(B\rho(p)) = p$ が必要かつ十分です。

$\bar{\rho}^{-1}(p') = p$、$\rho(p) \subset p'$、よって、$B_{\rho}(p) \subset p'$、$\bar{\rho}^{-1}(B_{\rho}(p)) \subset \bar{\rho}^{-1}(p') \subset p$ のような $B$ の理想 $p'$ が存在する場合、 逆が含まれていることは明らかなので、$\bar{\sigma}^{-1}(B_{\rho}(p)) = p$。逆に、$\bar{\rho}^{-1}(B_{\rho}(p)) = p$ と仮定し、$B$ の乗算部分集合 $S = \rho(A - p)$ を考えてみましょう。 仮定はそれを示しています
$$
S \cap B_{\rho}(p) = \varnothing;
$$
系 2 までに、$B$ 含む $B_{\rho}(p)$ の主要な理想 $p'$ が存在しますが、$S$ には至りません。次に、$\bar{\rho}^{-1}(p')$ 含む $p$ とできない含む $A - p$ のいずれかの元なので、$p$ と等しくなります。

#### 系 4 {#ac-ii-s2-prop-11-cor-4 .statement tag=046E}

※$A, B$を$A$から$B$までの2つの環と$\rho$準同型とします。
(i) $\rho_*(E)$ が忠実に平坦な $A$ モジュールとなる $B$ モジュール $E$ が存在すると仮定します。そして、$A$の各素イデアル$p$に対して、$\bar{\rho}^{-1}(p') = p$となるような$B$の素イデアル$p'$が存在します。
(ii) 逆に、$B$ がフラットな $A$ モジュールであると仮定します。次に、$A$ のすべての素イデアル $p$ に対して、$\bar{\rho}^{-1}(p') = p$、$B$ が忠実に平坦な $A$ 加群となるような $B$ のイデアル $p'$ が存在するとします。

(i) 仮定は、$A$、$\bar{\rho}^{-1}(B_{\rho}(a)) = a$ (章 I, § 3, no. 5、命題 8 (ii)) のすべての理想 $a$ に対して、系を適用する 3 で十分であることを意味します。
(ii) $A$ のすべての最大理想 $m$ に対して、$\bar{\rho}^{-1}(m') = m$ (章 I, § 2, no. 5, 命題 9 (e)) のような $B$ の最大理想 $m'$ が存在することを示すだけで十分です。今、仮定までに$B$の理想的な$q$が存在し、$\bar{\rho}^{-1}(q) = m$になります。 $q \neq B$ として、$B$ 含む $q$ の最大理想 $m'$ が存在し、その結果、$\bar{\rho}^{-1}(m') \supseteq m$ になります。ただし、$\bar{\rho}^{-1}(m')$ できない含む 1、$\bar{\rho}^{-1}(m') = m$ となります。

#### 系 5 {#ac-ii-s2-prop-11-cor-5 .statement tag=046F}

*$A$を環、$S$を$A$と$B$環の乗算部分集合として、$i_A^S(A) \subset B \subset S^{-1}A$とします。 $q$ を $A$ の素イデアル $p = (i_A^S)^{-1}(q)$ が $S$ を満たさないように、$B$ の素イデアルとし、$p'$ を $S^{-1}A$ の素イデアル $S^{-1}p$ とします。次に、$p' \cap B = q$.*

$S' = i_A^S(S)$ にしましょう。 標準同型は、${S'}^{-1}B$ から $S^{-1}A$ (no. 1、系 4 から命題 2) まで定義されています。私たちは同一視するこの環をこの同型によって実現しました。 $q \cap S' = \varnothing$ として、$q' = {S'}^{-1}q$ は $q' \cap B = (i_A^S)^{-1}(q') = q$ (命題 11 (ii))、よって $(i_A^S)^{-1}(q') = p$ となるような $S^{-1}A = {S'}^{-1}B$ の一意の素イデアルです。従って、$q' = p'$ (命題 11 (ii))。

系 5 の記法には、$A$ の標準同型があり、$(S^{-1}A)_q$ には $B_q$ があります。 (命題 11 (iii)) 従って、*標準同型* $A, \to B_q$ となります。

### 6. ニラディカルでミニマルなプライムの理想

(可換) では、冪零元の環 $A$ 集合は *理想* です。なぜなら、$x, y$ が $x^m = y^n = 0$ となるような $A$ の元である場合、二項定理により $(x + y)^{m+n} = 0$ になります。

#### 定義 4 {#ac-ii-s2-def-4 .statement tag=046G}

*a (可換) 環 $A$ の冪零元のイデアルは、$A$ のニルラジカルと呼ばれます。 $a$ が $A$ の理想である場合、標準写像 $A \to A/a$ の下で、$A/a$ のニルラジカルの逆像は、$a$ の根基と呼ばれます。

$A$ の理想 $a$ を $r(a)$ 根基で表すことがよくあります。

従って、$a$の元$x \in A$属するから根基ということは、$x^n \in a$となる整数$n > 0$が存在することを意味します。 準同型が$A$から環$B$で、$b$が$B$の理想である場合、$^{-1} (b)$を外した根基は$b$の根基を下回る*逆像*です。 $x^n \in f^{-1} (b)$は$(f(x))^n \in b$を意味します。

環 $A$ のニラディカルは、ヤコブソン根基 (*代数*、章 VIII, § 6, no. 3、系 3 ～ 定理 1) に含まれていますが、それとは異なる場合があります。 $A$ が *アルティン* (*代数*, 章 VIII, § 6, no. 4, 定理 3) の場合、常にそれに等しくなります。

環 $A$ の素イデアル $p$ が、包含順に並べられた $A$ の素イデアルの集合で最小である場合、それは *最小素イデアル* であると言います。

#### 命題 12 {#ac-ii-s2-prop-12 .statement tag=046H}

*$p$ を環 $A$ の最小素イデアルとします。すべての $x \in p$ に対して、$sx^k = 0$ となる $s \in A - p$ と整数 $k > 0$ が存在します。*

形 $sx^k$ の元の集合 $S$ ($k$ 整数 $> 0$、$s \in A - p$) は、$A$ の乗算部分集合です。 $0 \notin S$ の場合、$S$ (no. 5、系 2 ～ 命題 11) を満たさない主要な理想 $p'$ が存在します。 次に、仮定とは反対に、$p$ が最小であるため、$x \notin p'$ から $p' = p$ と $p' \# p$ になります。

#### 命題 13 {#ac-ii-s2-prop-13 .statement tag=046I}

*環 $A$ の nilradical は、$A$ のすべての素イデアルの共通部分であり、$A$ の最小素イデアルの共通部分でもあります。

明らかに、$x \in A$ がゼロポテントである場合、それは $A$ (§ 1, no. 1、定義 1) のすべての素イデアルに含まれます。逆に、$x$ を $A$ の非零能要素とします。 $x^k$ の集合 $S$ ($k$ 整数 $\geqslant 0$) は、含む 0 ではなく $A$ の乗法部分集合であるため、$A$ を満たさない主理想$p$ が存在します。 $S$ (no. 5、系 2 ～ 命題 11) および *なおさら* $x \notin p$;これにより最初の主張が確立されます。 2 番目を証明するには、次のことを証明すれば十分です。

#### 補題 2 {#ac-ii-s2-lem-2 .statement tag=046J}

*環 $A$ 含むのすべての素イデアル、$A$ の最小素イデアル。*

Zorn の補題によって、関係 $\supseteq$ で順序付けされた素イデアルの集合 P が *帰納的*であることを示すだけで十分です。 Now, if $G$ is a non-empty totally ordered subset of P, the intersection $p_0$ of the ideals $p \in G$ is also a prime ideal: for if $x \notin p_0$ and $y \notin p_0$, there exists an ideal $p \in G$ such that $x \notin p$ and $y \notin p$, whence $xy \notin p$ and *a fortiori* $xy \notin p_0$.

#### 注意 {#ac-ii-s2-n6-rem-1 .statement tag=046K}

§ 4, no. 3、系 3 から命題 14 では、最小素数イデアルの *ネーター* 環集合が *有限* であることを示します。さらに、ネーター 環の素イデアルのすべての減少列が *定常* であることが後でわかります。

#### 系 1 {#ac-ii-s2-lem-2-cor-1 .statement tag=046L}

*理想の根基* $a$ *環* $A$ *は、主要な理想の共通部分含む* $a$ *そして、この主要な理想の集合の最小の元の共通部分でもあります。

#### 系 2 {#ac-ii-s2-lem-2-cor-2 .statement tag=046M}

*For an ideal* $a$ *of a ring* $A$ *we denote by* $r(a)$ *the radical of* $a$. *次に、2 つの理想* $a, b$ *of* $A$ について、
$$
r(a \cap b) = r(ab) = r(a) \cap r(b);
$$
*特に、* $a \subset b$ の場合、* $r(a) \subset r(b)$ です。

主要な理想を含む $a \cap b$ (または $ab$) にするには、それが含む理想 $a, b$ (§ 1, no. 1、命題 1) の 1 つであることが必要かつ十分です。

#### 命題 14 {#ac-ii-s2-prop-14 .statement tag=046N}

*2 つの理想* 環の $a, b$ * が相対的に素であるためには、それらの根基* $r(a)$ * と* $r(b)$ * が互いに素であることが必要かつ十分です。

$a \subset r(a)$ と $b \subset r(b)$ があるため、条件の必要性は明らかです。 条件は§ 1, no. 2、命題3で十分です。

#### 命題 15 {#ac-ii-s2-prop-15 .statement tag=046O}

*環* $A$ *$a$ *理想とし、* $b$ *$a$ の根基に含まれる *有限生成された理想とする*。 *その後、整数* $k > 0$ *そのような* $b^k \subset a$ が存在します。

$(b_i)_{1 \leq i \leq n}$ を $b$ の生成元の系とします。 仮定までに整数 $h$ が存在し、$1 \leq i \leq n$ に対して $b_i^h \in a$ が存在します。 $A$の係数と$b_i$の線形結合である$nh$元の積を展開すると、それぞれの項は$nh$の積の倍数になります因子、それぞれは $b_i$ に等しい。これらの因子のうち、少なくとも$h$は一部の$i$と同じ添字$i$を持っているため、積属するから$a$となり、$nh$が必須の整数となります。 $k$。

#### 系 {#ac-ii-s2-n6-cor-1 .statement tag=046P}

*ネーター 環では、ニルラジカルは無能の理想です*。

#### 命題 16 {#ac-ii-s2-prop-16 .statement tag=046Q}

*$B$ *を環とし、* $A$ *部分環を * $B$ とします。 *すべての最小素数イデアル* $p$ *of* $A$ *最小素数イデアル* $q$ *of* $B$ *そのような* $q \cap A = p$ が存在します。

$S = A - p$と書きます。その場合、環 $A_+ = S^{-1}A$ は $S^{-1}B$ (no. 1, 命題 2) の部分環と同一視され、一方、$A_+$ は $p$ が最小であるため (no. 5, 命題) 、素数イデアル $p'$ を 1 つだけ持ちます。 11)。 $S^{-1}B$ は 0 に減らないので (含む $A_+$ なので)、少なくとも 1 つの素イデアル $r'$ を持ち、したがって $r' \cap A_+ = p'$ になります。 $j = i_B^S$ で $r = j'(t')$ と書くと、
$$
i_A^S(r \cap A) \subset r' \cap A_+ = p'
$$
したがって、$r \cap A \subset p$、そして$p$ が最小であるため、$t \cap A = p$ となります。さらに、$r$ は $B$ の素数です。 $q$ が $r$ (補題 1) に含まれる $B$ の最小素イデアルである場合、$p$ が最小であるため、なおさら $q \cap A = p$ になります。

#### 定義 5 {#ac-ii-s2-def-5 .statement tag=046R}

環 $A$ は、その nilradical が 0 に還元される場合、還元されたと呼ばれます。他の語では、$A$ の元 $\neq 0$ が nilpotent でない場合、還元と呼ばれます。

If $\mathfrak{N}$ is the nilradical of a ring $A$, $A/\mathfrak{N}$ is reduced, for if the class mod. $\mathfrak{N}$ of an element $x \in A$ is nilpotent in $A/\mathfrak{N}$, this means that $x^h \in \mathfrak{N}$ for some integer $h$, hence $x^{hk} = 0$ for some integer $k$ and $x \in \mathfrak{N}$.

#### 命題 17 {#ac-ii-s2-prop-17 .statement tag=046S}

$A$ を環 、$\mathfrak{N}$ をニルラジカルとします。 $A$ のすべての乗法部分集合 $S$ について、$S^{-1}\mathfrak{N}$ は $S^{-1}A$ のニルラジカルです。 特に、$A$ が減少すると、$S^{-1}A$ が減少します。

$x \in A$、$s \in S$ 満たす $(x/s)^n = x^n/s^n = 0$ の場合、$s'x^n = 0$ (no. 1、注意 3) およびなおさら $(s'x)^n = 0$ のような $s' \in S$ が存在するため、$s'x \in \mathfrak{N}$ と $x/s = s'x/s's \in S^{-1}\mathfrak{N}$ が存在します。 逆は明らかです。

### 7. テンソル積と準同型加群の分数

#### 命題 18 {#ac-ii-s2-prop-18 .statement tag=046T}

Let $A$ be a ring and $S$ a multiplicative subset of $A$.

(i) $M$ と $N$ が 2 つの $A$ モジュールである場合、$S^{-1}A$ モジュール $(S^{-1}M) \otimes_A N, M \otimes_A (S^{-1}N)$、$(S^{-1}M) \otimes_{S^{-1}A} (S^{-1}N)$ および $S^{-1}(M \otimes_A N)$ は正準的に同型です。

(ii) $M$ と $N'$ が 2 つの $S^{-1}A$ モジュールの場合、標準準同型
$$
M' \otimes_A N' \to M' \otimes_{S^{-1}A} N'
$$
$M' \times N'$ から $M' \otimes_{S^{-1}A} N'$ までの $A$-双線形写像 $(x', y') \mapsto x' \otimes y'$ から導出
単射的です
主張 (i) は定義 $S^{-1}M =$ の明らか帰結です

M \otimes_A S^{-1}A と標準同型内に与えるテンソル積の結合性

$$
(S^{-1}M \otimes_{S^{-1}A} (S^{-1}N)) = (S^{-1}M) \otimes_{S^{-1}A} (S^{-1}A \otimes N) = (S^{-1}M) \otimes_A N \\
= (S^{-1}A) \otimes_A M \otimes_A N = S^{-1}(M \otimes_A N).
$$

(ii) を証明するために、まず、$A$ 加群と考えられる $M'$ と $N'$ では、元 $s \in S$ によって引き起こされる相同性は全単射であるため、$M' = S^{-1}M'$ と $N' = S^{-1}N'$ (no. 2, 注意 4) および同様に$S^{-1}(M' \otimes_A N') = M' \otimes_A N'$; (ii) は (i) の特殊なケースです。

#### 系 {#ac-ii-s2-n7-cor-1 .statement tag=046U}

Let $M$ be an $A$-module and $a$ an ideal of $A$. サブ$S^{-1}A$ モジュール $(S^{-1}a)(S^{-1}M)$、$a(S^{-1}M)$、$(S^{-1}a)j(M)$ ($j : M \to S^{-1}M$ は標準写像) と $S^{-1}M$ の $S^{-1}(aM)$ は同一です。 特に、$a$ と $b$ が $A$ の 2 つの理想である場合、

$$
(S^{-1}a)(S^{-1}b) = a(S^{-1}b) = (S^{-1}a)b = S^{-1}(ab).
$$

#### 注意 {#ac-ii-s2-n7-rem-1 .statement tag=046V}

$M, N, P$ を 3 つの $A$ モジュール、$f : M \times N \to P$ を $A$ 双線形写像、$S^{-1}f : (S^{-1}M) \times (S^{-1}N) \to (S^{-1}P)$ を $f$ からスカラー 環を拡張して得られた $S^{-1}A$ 双線形写像とします。 $S^{-1}A$ (代数、章 IX, § 1, no. 4、命題 1)。 $i : M \to S^{-1}M, j : N \to S^{-1}N$ を標準準同型とします。 $Q$ が $f(M \times N)$ によって生成された $P$ のサブ $A$ モジュールである場合、$S^{-1}Q$ は $(S^{-1}f)(i(M) \times j(N))$ によって生成された $S^{-1}P$ のサブ $S^{-1}A$ モジュールであることがすぐにわかります。

#### 命題 19 {#ac-ii-s2-prop-19 .statement tag=046W}

Let $A$ be a ring and $S$ a multiplicative subset of $A$.
(i) If $M$ and $N$ are two $A$-modules and $M$ is finitely generated (resp. finitely presented), the canonical homomorphism (Chapter I, §2, no. 10, formula (10))

$$
S^{-1}\operatorname{Hom}_A(M, N) \to \operatorname{Hom}_{S^{-1}A}(S^{-1}M, S^{-1}N)
$$

は単射（それぞれ全単射）です。
(ii) $M', N'$ が 2 つの $S^{-1}A$ モジュールである場合、正規の全単射

$$
\operatorname{Hom}_{S^{-1}A}(M', N') \to \operatorname{Hom}_A(M', N')
$$

全客観的です。

$S^{-1}A$ はフラットな $A$ 加群であるため、(i) は章 I, §2, no. 10、命題 11 の特殊なケースです。 一方、$S^{-1}A$ 加群のすべての $A$ 準同型写像は必ず $S^{-1}A$ 準同型写像であることをすでに述べました。 証明命題 no. 2の3のコース。 よって (ii)。

#### 命題 20 {#ac-ii-s2-prop-20 .statement tag=046X}

$A, A'$ を 2 つの環、$p : A \to A'$ 準同型、$S$ $A$、$S' = \rho(S)$、$\rho' : S^{-1}A \to {S'}^{-1}A'$ 準同型対応するから $p$ の乗算部分集合とします。 (no. 1、命題 2)。

(i) *すべての* $A'$-モジュール $M'$ に対して、固有の $S^{-1}A$-同型性が存在します。
$$
j : S^{-1}\rho_*(M') \to \rho'_*({S'}^{-1}M')
$$
*そのような* $j(m'/s) = m'/\rho(s)$ *すべてに* $m' \in M', s \in S$。

(ii) *すべての* $A$ モジュール $M$ には、一意の同型が存在します。
$$
j' : (S^{-1}M) \otimes_{S^{-1}A} ({S'}^{-1}A') \to {S'}^{-1}(M \otimes_A A')
$$
*の* ${S'}^{-1}A'$*-モジュール* *そのような* $j'((m/s) \otimes (a'/s')) = (m \otimes a')/(\rho(s)s')$。

(i) ${S'}^{-1}M'$ を合成準同型 $i^{S'}_{M'} \circ p$ によって $A$ 加群として考えると、$S$ の元によって引き起こされる相似性は全単射であるため、記述された性質と一意な準同型 $j$ が存在します。 (no. 2、命題 3)。 $\rho(S) = S'$、$j$ は全射です。さらに、$m' \in M'$、$s \in S$、$m'/\rho(s) = 0$ の場合、$t'm' = 0$ となるような $t' \in S'$ が存在します。 $\rho_*(M')$ に $\rho(t) = t', t'.m' = 0$ があるような $t \in S$ が存在するため、$S^{-1}\rho_*(M')$ には $m'/s = 0$ が存在します。

(ii) $(S^{-1}M) \otimes_{S^{-1}A} ({S'}^{-1}A') = (M \otimes_A S^{-1}A) \otimes_{S^{-1}A} ({S'}^{-1}A')$ として、および
$$
{S'}^{-1}(M \otimes_A A') = (M \otimes_A A') \otimes_{A'} ({S'}^{-1}A'),
$$
$j'$ の存在は、テンソル積の結合性から生じます。

### 8. 代数へのお申込み

Let $A$ be a ring, $B$ an $A$-algebra (not necessarily associative or commutative and not necessarily possessing a unit element) and $S$ a multiplicative subset of $A$. We know that it is possible to define on the $S^{-1}A$-module $S^{-1}B = B \otimes_A S^{-1}A$ a canonical $S^{-1}A$-*algebra* structure, said to be obtained by extension of the ring of scalars to $S^{-1}A$ (Algebra, Chapter III, § 3) and under which the product $(x/s)(y/t)$ is equal to $(xy)/(st)$. $e$ が $B$ の単位元である場合、$e/1$ は $S^{-1}B$ の単位元であり、$B$ が結合 (可換) である場合、*so* は $S^{-1}B$ です。

$A$ を環 、$M$ を $A$ モジュールとします。 $M$ (代数、章 111) の *テンソル* 代数 (それぞれ外側代数、対称代数) を $T(M)$ (それぞれ $\Lambda(M)$、$S(M)$) で表します。すべての可換 $A$-代数 $C$ に対して、$T(M \otimes_A C)$ への $T(M) \otimes_A C$ の固有の同型 $j$ (それぞれ $\Lambda(M) \oplus_A C$ の $\Lambda(M \otimes_A C)$ 、$S(M) \otimes_A C$ の $S(M \otimes_A C)$ ) が存在することが知られています。そのような
$$
i(x \otimes 1) = x \otimes 1
$$
すべての $x \in M$、$M$ は、標準的に $T(M)$ の部分加群 (それぞれ $\Lambda(M), S(M)$) と識別されます (*loc. cit.*)。次に、特に、$A$ のすべての乗法部分集合 $R$ に対して *標準同型* があることがわかります。
$$
R^{-1}T(M) \to T(R^{-1}M), \qquad R^{-1}\Lambda(M) \to \Lambda(R^{-1}M), \qquad R^{-1}S(M) \to S(R^{-1}M)
$$
簡約するは $R^{-1}M$ の ID になります。

### 9. 加群 / 分数 / 採点済み加群

$A$ を段階的環、$M$ を段階的 $A$ モジュール、$A$ 次数モノイドとする。この番号を仮定します。 $A$ は *群* です。 (*代数*、章 II, § 11) $A$ と $M$ はそれぞれ加法群の直和であることを思い出してください。
$$
A = \bigoplus_{i \in \Delta} A_i, \qquad M = \bigoplus_{i \in \Delta} M_i
$$
$i, j \in A$すべてに$A_i A_j \subset A_{i+j}$と$A_i M_j \subset M_{i+j}$が付きます。 $S$ を $A$ の乗算部分集合とします *その元はすべて同次です*。すべての $i \in A$ について、$S_i = S \cap A_i$ と書き、$A$、元の元 $j, k$ が存在する、元の $m'$ $S^{-1}M$ の $(S^{-1}M)_i$ 集合で表します。 $m \in M_j$ と元 $s \in S_k$ は、$j - k = i$ と $m' = m/s$ のようになります。 $(m'_q)_{1 \leq q \leq r}$ が $S^{-1}M$ の元の有限族である場合、次のようになります。
$$
m'_q \in (S^{-1}M)_{j(q)},
$$
元 $j(q) \in A$ と $k \in A$、元 $m_q \in M_{j(q)}$ ($1 \leq q \leq r$) と $s \in S_k$ が存在し、$1 \leq q \leq r$ (no. 1, *注意 2*) に対して $m'_q = m_q/s$ が成り立ちます。

#### 命題 21 {#ac-ii-s2-prop-21 .statement tag=046Y}

*家族との環 $S^{-1}A$ $((S^{-1}A)_i)$ はグレード環で、家族との $S^{-1}M$ $((S^{-1}M)_i)$ はグレード環 $S^{-1}A$ を超えるグレード加群です。 標準写像 $i^S_A$ と $i^S_M$ は次数 0 と同次です。*

$m \in M$、$s \in S_k$、$m' \in M_{j'}$、$s' \in S_{k'}$ として、$j - k = j' - k' = i$ と仮定します。次に、$(m/s) - (m'/s') = (s'm - sm')/ss'$、$s'm - sm' \in M_{j'+k'} = M_{j'+k'}$、$ss' \in S_{k+k'}$、したがって、$(m/s) - (m'/s') \in (S^{-1}M)_i$ by 定義。これは、$(S^{-1}M)_i$ が $S^{-1}M$ の加法的な部分群であることを示しています。これらの群のうち和は $S^{-1}M$ の全体です。すべての $x \in S^{-1}M$ は $m/s$ と書くことができます。ここで、$m \in M, s \in S; s$ は仮定によって同種であり、$m$ は同種元の和です。 $m_j$;したがって、$x$ は $m_j/s$ の和であり、それぞれ属するから部分群 $(S^{-1}M)_i$ です。最後に、$(S^{-1}M)_i$ の和が直接です。というのは、$x_q \in (S^{-1}M)_{i(q)}$ のような元 $x_q$ ($1 \leq q \leq n$) の有限族を考えてみましょう。ここで、添字 $i(q)$ は別個であり、$\sum_{q=1}^n x_q = 0$ と仮定します。それぞれの $x_q$ は、$s \in S_k$ と $m_q \in M_{i(q)+k}$ の場合、$x_q = m_q/s$ と書くことができます。 仮定は、$s'\left( \sum_{q=1}^n m_q \right) = 0$ となるような $s' \in S$ が存在することを意味します。 $s'm_q$ がすべて零ではない場合、$s' \in S_d$ であれば、$s'm, \in M_{i(q)+d}$ と $i(q) + d$ はすべて別個であるため、矛盾が生じます。したがって、添字 $q$ ごとに $x_q = 0$ となります。

$a \in (S^{-1}A)_i$ と $x \in (S^{-1}M)_j$ の場合、$ax \in (S^{-1}M)_{i+j}$ であることがすぐに検証されます。 適用この結果をケース $M = A$ に当てはめると、まず $S^{-1}A$ が $(S^{-1}A)_i$ によって等級付けされた環であることがわかります。次に、$S^{-1}M$ が $S^{-1}A$ よりも加群に評価されていることがわかります。最後に、$1 \in A_0$、$i_A^S$、$i_M^S$ は次数 0 と同次です。

#### 命題 22 {#ac-ii-s2-prop-22 .statement tag=046Z}

A (それぞれ B) を型 A の等級環とし、M (それぞれ N) を等級環 A (それぞれ B)、S (それぞれ T) の等級加群とする A (それぞれ B) の乗算部分集合のすべての元は同次、$f : A \to B$ $f(S) \subset T$ と $u : M \to N$ A-線型写像が次数 k と同次であるような、次数 0 の同次準同型。次に、 f (no. 1, 命題 2) から導出された準同型 $f' : S^{-1}A \to T^{-1}B$ は、次数 0 と $(S^{-1}A)$ 線形写像と同次です。

$$
u' : S^{-1}M \to T^{-1}N
$$

f と $u$ (no. 2, 命題 5) は次数 k と同次です。

これは、方程式$f'(a/s) = f(a)/f(s)$ と$u'(m/s) = u(m)/f(s)$ からすぐに得られます。

最後に、E が段階的 A-代数であり、S が同次元のからなるの乗法部分集合である場合、$S^{-1}E$ とその $(S^{-1}A)$-代数構造 (no. 8) および目盛り $(S^{-1}E)_i$ は、 定義からすぐに続くように、$S^{-1}A$-代数を等級付けしました。

### 練習問題 {#ac-ii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
