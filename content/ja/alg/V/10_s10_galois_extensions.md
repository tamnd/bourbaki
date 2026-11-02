---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 10
section_title: Galois extensions
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.56-A V.76, A V.154-A V.160
pdf_pages: 0170-0190, 0268-0274
extraction: ocr
subsections:
    - "no": 1
      title: Definition of Galois extensions
      page: 56
      pdf_page: 170
    - "no": 2
      title: The Galois group
      page: 58
      pdf_page: 172
    - "no": 3
      title: Topology of the Galois group
      page: 60
      pdf_page: 174
    - "no": 4
      title: Galois descent
      page: 62
      pdf_page: 176
    - "no": 5
      title: '*Galois cohomology*'
      page: 64
      pdf_page: 178
    - "no": 6
      title: Artin’s theorem
      page: 65
      pdf_page: 179
    - "no": 7
      title: The fundamental theorem of Galois theory
      page: 67
      pdf_page: 181
    - "no": 8
      title: Change of base field
      page: 69
      pdf_page: 183
    - "no": 9
      title: The normal basis theorem
      page: 72
      pdf_page: 186
    - "no": 10
      title: Finite $\Gamma$-sets and etale algebras
      page: 75
      pdf_page: 189
    - "no": 11
      title: The structure of quasi-Galois extensions
      page: 76
      pdf_page: 190
statements: 49
exercises: 23
content_sha256: 1faf856a7d9fed59e23319c65eb6ed3d6c77e0179c1d0c1e634665106bd80d0f
translated_from: content/en/alg/V/10_s10_galois_extensions.md
translation_method: google
source_content_sha256: ed1a3cc64fa97276bda6bff686f4a827b57d0250dbe6c9cb5ce9dddcfe06ceb5
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 5df048becd460ac08b9199de8a89e7ceb91b1081d5819c7a51bc7a958a804c8b
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 10。 ガロア拡大

この段落全体を通じて、K は体を表します。

### 1. ガロア拡大中定義

#### 定理 1 {#alg-v-s10-thm-1 .statement tag=06MB}

— N を K の代数拡大および N の K 自己同型の $\Gamma$ 群とします。すると、次の主張は等価です。
a) N の K の $\Gamma$ 属するから像の下で N の各元が不変です。
b) N は、K の分離可能な準ガロア拡張です。
c) 各 $x \in N$ について、$N[X]$ の K 分裂上の x の最小多項式を、次数 1 の別個の多項式の積に変換します。
b) および c) の同値は、Cor.提案 6 (V、p. 40) および準ガロア拡張の定義 (V、p. 53、定義 2)。 同一視する K とその標準像を N にしましょう。
$a) \Rightarrow c)$: K が $\Gamma$ の不変量の体であると仮定します。 K 上の最小多項式 $f$ をもつ $x \in N$ とし、A を N の f のすべての根の集合とします。
$$
g(X) = \prod_{y \in A} (X - y).
$$
A の自己同型 $a \in \Gamma$ 誘導する置換ごとに、多項式 $g \in N[X]$ の係数が不変のままになります。したがって、$g \in K[X]$ があり、$g(x) = 0$ 以降、多項式 g は、$K[X]$ (V, p. 16, Th. 1) の $f$ の倍数になります。さらに、$f$ と g はモニックであり、g 割る $f$ (IV, p. 16、提案 5)。したがって、$f = g$ が得られます。これは、$K$ 上の$x$ の最小多項式$f$ は、次数 1 の別個の多項式の$N[X]$ の積であることを意味します。

c) ⇒ a): x を K に対する所属ではなく、N の元とする。 K 含む N の Ω 代数閉包をサブエクステンション (V、p. 23、Th. 2) として表します。 Let f be the minimal polynomial of x over K, which is of degree ≥ 2 by hypothesis and let A be the set of roots of $f(X)$ in N. 条件 c) が成り立つ場合、$f(X) = \prod_{y \in A} (X - y)$ があり、したがって (V, p. 53, Cor. 1) A は Ω で表した x の共役の集合です。 f は次数 ≥ 2 であるため、A には元 $y \neq x$ が存在し、したがって $u(x) = y$ となる Ω の K 自己同型 u が存在します。 現在、仮定 c) では、K の拡大 N は準ガロアであるため、$u(N) = N$ (V, p. 54, Cor. 1);したがって、u 誘導するは $\sigma(x) = y \neq x$ となる N の K 自己同型 a であるため、K は Γ の不変量の体になります。

#### 定義 1 {#alg-v-s10-def-1 .statement tag=06MC}

— 拡大 K の N が代数的であり、Th の等価な条件 a)、b)、c) を満たす場合、ガロアであると言われます。 1.

N を体、N の自己同型の Γ 群、および Γ の不変量の $N_0$ 体とします。 N が $N_0$ 上で代数的である場合、それは $N_0$ のガロア拡大です。これは必ずしもそうである必要はありません。たとえば、K が無限で、N が有理分数 K(X) の体であるとします。それぞれの $a \in K$ について、$\sigma_a$ を K(X) の自己同型とし、写像 $f(X)$ から $f(X + a)$ とします。すべての $a$ の集合は、K(X) の自己同型の群であり、その不変式の体は K であることが容易にわかります。ただし、K(X) は K に対して代数的ではありません。

Ω を K の代数閉包とし、A を K 上で分離可能な Ω の元の集合と、B を A の元の K 上で分離可能な共役の集合とします。 この場合、B は代数的で K に関して分離可能な元で構成されます。 したがって、(V、p. 39、提案 6 および p. 56、提案 5) 体 K(B) は、K の分離可能な準ガロア拡張です。他の語では、A (V, p. 55) によって生成された準ガロア拡張は K のガロア拡大です。また、それは O の部分集合 A によって生成された K のガロア拡大であるとも言えます。

特に、K 上の可分多項式族の Ω の分解体、K の分離閉包は、K のガロア拡大です。

#### 命題 1 {#alg-v-s10-prop-1 .statement tag=06MD}

— N を K の拡大と N の部分拡張の空ではない族である $(N_i)_{i \in I}$ とします。$E = \cap_{i \in I} N_i$ と $F = K \left( \bigcup_{i \in I} N_i \right)$ を置きます。すべての拡大 N が K 上のガロアである場合、E と F にも同じことが当てはまります。

そもそも E は代数的であり、K (V, p. 36, 命題 1) に関して可分であり、F (V, p. 41, 命題 8) についても同じことが当てはまります。さらに、E と F は、提案 4 (V, p. 55) により K 上の準ガロアです。

#### 命題 2 {#alg-v-s10-prop-2 .statement tag=06ME}

— N を K のガロア拡大とし、E を K 上の有限次数の N の部分拡張とします。N 含む E、ガロアおよび K 上の有限次数の部分拡張 F が存在します。

N は K 上の準ガロアであるため、Cor。 V, p. 56 の 1 は、N 含む E と K 上の有限次数の準ガロア部分拡張 F の存在を証明します。N は K 上で分離可能であるため、F (V, p. 36、提案 1) にも同じことが当てはまります。したがって、F は K 上のガロアです。

提案 2 は次の結果を暗示しています: R を K および E₁, ..., Eₙ の代数閉包として、R に含まれる K 上の有限次数の可分代数拡大とする。すると、R に含まれる K の有限次数のガロア拡大 N と含む E₁, ..., Eₙ が存在します。

### 2. ガロア群

#### 定義 2 {#alg-v-s10-def-2 .statement tag=06MF}

N を体 K のガロア拡大とします。N のすべての K 自己同型の群は、K 上の N のガロア群と呼ばれ、Gal(N/K) で表されます。

N を K の有限ガロア拡大とします。このとき、N は K の有限可分かつ擬似ガロア拡張です。 したがって (V、p. 32、提案 4 および V、p. 54、提案 3)、Gal(N/K) の位数は [N : K] に等しくなります。 Gal(N/K) が有限となるように N が K のガロア拡大である場合、N は K に対して有限次数であることを後で証明します (V, p. 66, Th. 3)。

可分多項式 f ∈ K[X] の Ω において、Ω を K の代数閉拡大とし、A を根の集合とします。そのとき、体 N = K(A) は K のガロア拡大です。N のすべての K 自己同型が A を安定にすることは明らかであり、K 上の生成する N であるため、写像 a ↦ σ|A は対称群の部分群 Γ 上の Gal(N/K) の同型です。 集合 A の S_A。多項式 f のガロア群と呼ばれます。 注意 3 (V, p. 55) から、x と y 属するが A である場合、次のプロパティは同等であることがわかります。

a) x と y は K を超えて共役、
b) x と y 属するは Γ の下で同じ軌道、
c) x と y は f の同じ既約因子の根です。

特に、A が空でなく、Γ が A に対して推移的に作用する場合に限り、 f は既約です。

#### 例 1 {#alg-v-s10-n2-exa-1 .statement tag=06MG}

K の特性が 2 とは異なると仮定し、N を K の 2 次式拡大とします。 x ∈ N − K の場合、N = K(x) となり、K 上の x の最小多項式は形 f(X) = X² − aX + b となります。ただし、a、b ∈ K となります。 f(X) = (X − x)(X − y) ここで、y = a − x であるため、y は x に対して共役です。 f(X) は分離可能であるため、拡大 N はガロアです。 群 Gal(N/K) には 2 つの元があり、これは集合 {x, y} の 2 つの置換である誘導するです。

#### 例 2 {#alg-v-s10-n2-exa-2 .statement tag=06MH}

\* f = X³ + X² − 2X − 1 ∈ Q[X] とします。多項式 f は既約です。そうでない場合は、根 x ∈ Q になります。 a、b ∈ Z、a と b が互いに素である x = a/b を書くと、a(a² + ab − 2b²) = b³ および a³ = b(b² + 2ab − a²) が見つかるはずです。しかし、これは割る b および b 割る a であることを意味するため、x = ±1 となり、これは不可能です。 ξ = e^{2\pi i / 7} ∈ C; と置きます。この場合、多項式 f は根 α = ξ + ξ⁻¹、β = ξ² + ξ⁻²、γ = ξ³ + ξ⁻³ となります。 β = a² − 2 および γ = a³ − 3α であるため、拡大 Q(α) は Q 上のガロアです。Q 上の Q(α) のガロア群は位数 3 の巡回であり、σ(α) = β、σ(β) = γ、σ(γ) となるように元 σ によって生成されます。 =α。 \*

#### 例 3 {#alg-v-s10-n2-exa-3 .statement tag=06MI}

$K = \mathbf{Q}$ として $f = X^3 - 2$ を取るとします。 整数の分解を素数因子 (I, p. 51) の積に代入すると、2 が $\mathbf{Q}$ の元の 3 乗ではないことが簡単にわかります。したがって、多項式 $f$ は既約です。そうでない場合、$\mathbf{Q}$ は根になるからです。 $A = \{ x_1, x_2, x_3 \}$を、$\Omega$の$f$の根の集合と、$f$の$\Gamma$ガロア群とします。 $A$ に推移的に作用します。したがって、位数は 3 で割り切れます。一方、商 $j = \frac{x_2}{x_1}$ は 1 とは異なり、$j^3 = 1$ があります。したがって、$j$ は関係 $j^2 + j + 1 = 0$ を満たします。現在、多項式 $T^2 + T + 1 = \left( T + \frac{1}{2} \right)^2 + \frac{3}{4}$ には $\mathbf{Q}$ に根が含まれておらず、(例 1) は $[\mathbf{Q}(j) : \mathbf{Q}] = 2$ であることがわかります。したがって、$[\mathbf{N} : \mathbf{Q}]$ は 2 で割り切れ、$\Gamma$ の位数は 6 で割り切れます。$\Gamma$ は位数 6 の群 $\mathfrak{S}_A$ に含まれるため、$\Gamma = \mathfrak{S}_A$ が得られます。

#### 例 4 {#alg-v-s10-n2-exa-4 .statement tag=06MJ}

$K$ が特性 $p \neq 0$ であると仮定し、$K(T)$ を有理分数と $U = T^p - T$ の体とします。 $E = K[U]$ と $F = K[T]$ を置くと、$E[X]$ の多項式 $f(X) = X^p - X - U$ は、$F$ で根 $T, T+1, ..., T+p-1$ になります。 $\sigma$ を、$\sigma(T) = T+1$ となるような $F$ の $K$ 自己同型とする。 $\sigma^i(T) = T+i$と$\sigma(U) = U$がございます。 群 $G = \{ 1, \sigma, ..., \sigma^{p-1} \}$ は、位数 $p$ とその不変量含む $E$ の体の巡回です。 $[F : E] \leq p$ 以来、デデキントの定理 (V、p. 27、Cor. 2) は、$E$ が $G$ と $[F : E] = p$ の不変量の体であることを意味します。したがって、多項式 $f$ は $E[X]$ で既約です。 $E$ の拡大 $F$ はガロアであり、そのガロア群 $G$ は位数 $p$ の巡回であり、群 $\Gamma$ は巡回の群です$T, T+1, ..., T+p-1$の置換。

この例の一般化については、V、p. 93、例 2を参照してください。

#### 例 5 {#alg-v-s10-n2-exa-5 .statement tag=06MK}

$F = K(X_1, ..., X_n)$ を $n$ の有理分数の体とすると、$K$ の係数で $X_1, ..., X_n$ が不定になります。置く
$$
s_k = \sum_{1 \leq i_1 < ... < i_k \leq n} X_{i_1} ... X_{i_k}
$$
$1 \leq k \leq n$ と $E = K(s_1, ..., s_n)$ の場合。多項式を $f(T)$ で表します
$$
T^n - s_1 T^{n-1} + \cdots + (-1)^n s_n .
$$
$f(T) = \prod_{i=1}^n (T - X_i)$ があるため、$F$ は可分多項式 $f(T) \in E[T]$ の分解体になります。さらに、$1 \leq i \leq n$ に対して $h_a(X_i) = X_{a(i)}$ となるような、$F$ の$K$ 自己同型$h_a$ が置換 $a \in \mathfrak{S}_n$ ごとに存在します。 $1 \leq k \leq n$ に対して $h_a(s_k) = s_k$ があるため、$h_a$ は $F$ の $E$ 自己同型です。他の語では、$F$は$E$のガロア拡大と、根の$\{ X_1, ..., X_n \}$、$f(T)$の定義する、同型の制限から集合です。 $\mathrm{Gal}(F/E)$ から群 $\mathfrak{S}_n$ へ。特に、$E$ は、次のような有理分数 $f$ で構成されます。
$$
f(X_{\sigma(1)}, ..., X_{\sigma(n)}) = f(X_1, ..., X_n)
$$
$\sigma \in \mathfrak{S}_n$ (cf. IV、p. 67、Cor.) ごとに。

#### 例 6 {#alg-v-s10-n2-exa-6 .statement tag=06ML}

f が次数 > 0 のモニックであり、K が標数 ≠ 2 であるとします。 定義する A について、≤ で示される全順序付けを行い、δ(f) = $\prod_{\alpha < \beta} (\beta - a)$、$(\alpha, \beta) \in A \times A$ を置き、それぞれの $\sigma \in \mathfrak{S}_A$ に対して $\delta_\sigma(f) = \prod_{\alpha < \beta} (\sigma(\beta) - \sigma(\alpha))$ を置きます。 $\delta_\sigma(f) = \varepsilon(u) \delta(f)$ があり、$\varepsilon(u)$ は $\sigma$ (I、p. 64) と $\delta(f) \neq 0$ の署名です。 $\tau \in \mathrm{Gal}(N/K)$ ごとに $\tau(\delta(f)) = \delta_{\tau|_A}(f)$ があります。したがって、$\Gamma$ は、$\delta(f) \in K$ の場合に限り、交代的群 $\mathfrak{A}_A$ に含まれます。また、$\delta(f)^2 = \prod_{\alpha < \beta} (\beta - a)' = d(f)$ は多項式 f (IV, p. 81) の判別式です。したがって、$d(f)$ が K の元の平方である場合に限り、$\Gamma \subset \mathfrak{A}_A$ になります。 したがって、例 2 では $d(f) = 49 = 7^2$ が得られ、例 3 では $d(f) = -108$ (IV, p. 85) になります。

N を K のガロア拡大とし、L を K 上のガロアである N の部分拡張とします。N 誘導するのすべての K 自己同型 $\sigma$ は、L (V、p. 55、注意) の K 自己同型 $\sigma_L$ となります。 1)。したがって、写像 $\sigma \mapsto \sigma_L$ は、$\mathrm{Gal}(N/K)$ の準同型が $\mathrm{Gal}(L/K)$ になり、制限準同型と呼ばれます。

#### 命題 3 {#alg-v-s10-prop-3 .statement tag=06MM}

— *制限準同型* の $\mathrm{Gal}(N/K)$ を $\mathrm{Gal}(L/K)$ に *全射*です。

より一般的には、N の 2 つの部分拡張 L および L' と、L' への L の K-同型写像 $u$ を考えてみましょう。サブ内線としての K 含む N の選ぶ代数閉包 $\Omega$ (V、p. 23、Th. 2)。 L 上で $u$ をもつ一致するである $\Omega$ の K 自己同型 $v$ が存在し (V, p. 52, 提案 1)、N は K の準ガロア拡張であるため、$v$ 誘導する a N の K 自己同型 $\sigma$ (V, p. 55, 注意 1)。他の語、元 $\sigma$の$\mathrm{Gal}(N/K)$ 一致するには、Lに$u$が付きます。

### 3. ガロア群中位相

N を K のガロア拡大と K 上の N の $\Gamma$ ガロア群とします。N のすべての写像の離散位相集合 $N^N$ と、N の離散位相の積位相を N に装備します。 因子 (「N の単純収束の位相」) と $N^N$ から誘導された位相を伴う群 $\Gamma$。

A を K 上の有限次数の N のすべての部分拡張の集合とします。 $\sigma \in \Gamma$ と $E \in A$ については、元の $\tau$ と同じ制限を持つ $\Gamma$ の集合に対して $U_E(\sigma)$ を書きます。 $\sigma$ から E。$E = K(x_1, ..., x_n)$ の場合、集合 $U_E(\sigma)$ は $\tau(x_i) = \sigma(x_i), ..., \tau(x_n) = \sigma(x_n)$ となるように元 $\tau \in \Gamma$ で構成されます。したがって、ファミリー $(U_F(\sigma))_{F \in \mathscr{F}}$ は、$\Gamma$ の $\sigma$ の近傍のフィルターの基底になります。

N が K に対して有限次数であるとき、$N \in A$ と $U_N(\sigma) = \{\sigma\}$ があり、したがって $\mathrm{Gal}(N/K)$ の位相は離散的です。 (V, p. 58)、この場合、群 $\mathrm{Gal}(N/K)$ は有限であることを思い出してください。

この $\mathrm{Gal}(N/K)$ の位相の記述は、$\mathrm{Gal}(N/K)$ *onto* $\mathrm{Gal}(L/K)$ の *制限準同型* が、N 上のガロアである N のすべての部分拡張 L に対して連続していることを示しています。

$A$ を $\Gamma$ の部分集合とします。 $A$ が開いているということは、$\sigma \in A$ ごとに $A$ に $E$ が存在し、集合 $U_E(\sigma)$ が $A$ に含まれることを意味します。 $A$ の閉包 $\overline{A}$ はすべての $\sigma \in \Gamma$ で構成されており、どの $E \in A$ についても $\sigma$ と同じ制限から $E$ を持つ $\tau \in A$ が存在します。 $\overline{A}$ の不変量の体は、$A$ の不変量と同じです。

$\varepsilon$ を $\Gamma$ の中立値元とし、$A'$ を $N$ の部分拡張 (ガロア) と $K$ 上の有限次数の部分拡張の集合とします。提案 2 (V, p. 57) により、集合 $A'$ は $A$ で cofinal となり、ファミリー $(U_E(\varepsilon))_{E \in A'}$ は、$\Gamma$ の $\varepsilon$ の近傍のフィルターの基底になります。さらに、$E \in A'$の集合$U_E(E)$は、$\mathrm{Gal}(N/K) = \Gamma$の制限準同型の核が$\mathrm{Gal}(E/K)$になります。 $\mathrm{Gal}(E/K)$ は有限であるため、$U_{\Gamma}(\varepsilon)$ は、$\Gamma$ における通常の開いた閉じた部分群であり、有限の添字であることがわかります。

明らかに、$\sigma \in \Gamma$ と $E \in A'$ に対して $U_{\Gamma}(\sigma) = \sigma U_{\Gamma}(\varepsilon) = U_{\Gamma}(\varepsilon) \sigma$ があります。 $U_{\Gamma}(\varepsilon)$ はすべての $E \in A'$ の $\Gamma$ の通常の部分群であり、家族 $(U_E(\varepsilon))_{E \in A'}$ は $\varepsilon$ での近傍の基底であるため、$\Gamma$ の位相は群構造と互換性があります。 (将軍トップ、III、p. 223)。その他語、写像$(\sigma, \tau) \mapsto \sigma \tau^{-1}$、$\Gamma \times \Gamma$から$\Gamma$までが連続します。

#### 命題 4 {#alg-v-s10-prop-4 .statement tag=06MN}

— $N$ を $K$ のガロア拡大とします。次に、ガロア群 $\Gamma = \mathrm{Gal}(N/K)$ はコンパクトで完全に切り離されています。

$\Gamma$ のすべての元 $\sigma$ には、近傍からなるの基底があり、集合 $U_E(\sigma)$ が開いているため、$\Gamma$ は完全に切断されています (Gen. トップ。、I、p. 111）。 $\{\sigma\} = \bigcap_{E \in \Lambda} U_E(\sigma)$ があるため、$\Gamma$ は分離されます。 $x$ の共役 $\sigma(x)$ のそれぞれの $x \in N$ 集合について、$\sigma$ が $\Gamma$ にわたる範囲であるとき、$x$ は$K$ で代数的であるため、*有限* です (V、p. Cor. 1)。したがって、$N^N$の因子空間上の$\Gamma$のすべての射影は有限集合であり、これは$N^N$では$\Gamma$が比較的コンパクトであることを示しています。 トップ。、I、p. 88）。 $\Gamma$ が $N^N$ で閉じられていることを示すことが残っています。 ここで、$u$ が $N^N$ の $\Gamma$ の閉包にある場合、点 $(x, y)$ の $N$ の各対に対して、$u(x) = \sigma(x), \ u(y) = \sigma(y), \ u(x+y) = \sigma(x+y), \ u(xy) = \sigma(xy)$、よって $u(x+y) = u(x) + u(y)$ を含む $a \in \Gamma$ が存在します。 $u(xy) = u(x)u(y)$。 同じ推論により、すべての $x \in K$ に対して $u(x) = x$ が得られるため、$u$ は $N$ から $N$ への $K$ 準同型写像になります。 $N$ は $K$ に対する代数であるため、$u$ は $N$ (V, p. 52、提案 1) の $K$ 自己同型であるため、$u \in T$ です。

$N$ を $K$ のガロア拡大と $(N_i)_{i \in I}$ 増加するのサブエクステンションの$N$ の有向ファミリーとします。 $N_i$ がすべての $i \in I$ と $N = \bigcup_{i \in I} N_i$ について $K$ に対するガロアであるとします。 For each $i \in I$ denote by $\Gamma_i$ the Galois group of $N_i$ over $K$; for $i \leq j$ in $I$ we have $N_i \subset N_j$ and the restriction homomorphism $\varphi_{ij}$ of $\Gamma_j$ into $\Gamma_i$ is defined. それは連続であるため、族 $(\Gamma_i, \varphi_{ij})$ はトポロジー 群の逆系です。 さらに、各 $i \in I$ を $\mathrm{Gal}(N/K)$ の $\lambda_i$ 制限準同型を $\mathrm{Gal}(N_i/K) = \Gamma_i$ に表します。これは連続であり、$i \leq j$ には $\lambda_i = \varphi_{ij} \circ \lambda_j$ があるため、家族 $(\lambda_i)_{i \in I}$ 定義するは、$\mathrm{Gal}(N/K)$ の準同型 $\Lambda$ が $\varprojlim \Gamma_i$ に連続します。

#### 命題 5 {#alg-v-s10-prop-5 .statement tag=06MO}

— *準同型* $\lambda$ *of* $\mathrm{Gal}(N/K)$ *into* $\varprojlim \mathrm{Gal}(N_i/K)$ *はトポロジカル群* の同型です。

$\mathrm{Gal}(N/K)$ はコンパクトで、$\lambda$ は連続で、群 $\varprojlim \mathrm{Gal}(N_i/K)$ は分離しているため、$h$ が全単射であることを示すだけで十分です (*Gen. Top.*, *I*, p. 87, Cor. 2)。 $u = (u_i)_{i \in I}$ を $\varprojlim \mathrm{Gal}(N_i/K)$ の元とします。それぞれの $i \in I$、$u_i$ は $N_i$ の K 自己同型であり、$u_i$ は $i \leq j$ の $u_j$ から $N_i$ の制限です。 $N = \bigcup_{i \in I} N_i$以降、すべての$i \in I$に対して、$N_i$に$u_i$が付く一致するが存在する$\mathrm{Gal}(N/K)$の一意元$\sigma$が存在します。したがって、$\sigma$ は $\lambda(u) = u$ となるように $\mathrm{Gal}(N/K)$ の一意元であるため、$\lambda$ は全単射です。

これは特に、$N$ のすべての有限ガロア部分拡張の族 $(N_i)$ をとったときに当てはまります。その場合、それぞれの群 $\mathrm{Gal}(N_i/K)$ は離散的で有限です。したがって、トポロジカル群 $\mathrm{Gal}(N/K)$ は、離散位相を備えた有限群の有向逆反転極限と同型です。これは *profinite* トポロジカル群と呼ばれるときどきです。

### 4. ガロア降下法

*この番号*では、$N$ *体*、$\Gamma$ *群の自己同型の*、$N$、$e$ *中立元の* $\Gamma$ *および* $K$ *体の* $\Gamma$ の不変式。

$V$を$N$以上のベクトル空間とします。 $V$ 上の *K 構造* は $V$ のベクトルサブ K 空間 $V_0$ であり、 写像 $h \otimes x$ から $\lambda x$ である K-線型写像 $\varphi : N \otimes_K V_0 \to V$ であることを思い出します (II、p. 317)。全単射。 $V_0$ をそのような K 構造とします。それぞれの $\sigma \in \Gamma$ に $u_\sigma = \varphi \circ (\sigma \otimes \mathrm{Id}_{V_0}) \circ \varphi^{-1}$ を入れます。次に、元 $\lambda_i$ の $N$ と $e_i$ の $V_0$ よってのすべての家族に対して $u_\sigma \left( \sum_{i \in I} \lambda_i e_i \right) = \sum_{i \in I} \sigma(\lambda_i) e_i$ が得られ、関係が得られます。
$$
\begin{align*}
u_\sigma(x + y) &= u_\sigma(x) + u_\sigma(y) \\
u_\sigma(\lambda x) &= \sigma(\lambda) u_\sigma(x) \\
u_\sigma \circ u_\tau &= u_{\sigma \tau} \\
u_e &= \mathrm{Id}_V
\end{align*}
$$
$\Gamma$の$\sigma, \tau$、$V$の$x, y$、$N$の$\lambda$。

#### 命題 6 {#alg-v-s10-prop-6 .statement tag=06MP}

— *a)* *$V$ *ベクトル空間を過ぎてください* $N$ *a* $K$-*構造* にしてください。 *ベクトル* $x \in V$ *以上に合理的であるために* $K$ *それは必要かつ十分です* $u_\sigma(x) = x$ *すべて* $\sigma \in \Gamma$。 *ベクトルサブ N 空間* $W$ *の* $V$ * $K$ * に対して有理であること* $u_\sigma(W) \subset W$ *すべて* $\sigma \in \Gamma$ であることが必要かつ十分です。

*b)* *$V_1$ *と* $V_2$ *2つのベクトル空間を* $N$とし、*それぞれに* $K$-*構造*を付けます。 *線形写像* $f$ *の* $V_1$ *に* $V_2$ *以上に合理的であるために* $K$ *それは必要かつ十分* $f(u_\sigma(x)) = u_\sigma(f(x))$ *すべて* $\sigma \in \Gamma$ *そしてすべて* $x \in V_1$。

*明らかに* $K$ *は $x \in N$ の集合 * であること* $\sigma(xy) = x \sigma(y)$ *すべて* $\sigma \in \Gamma$ *そしてすべて* $y \in N$ です。 *命題したがって、Th から続きます。 1* (II、p. 324)。

#### 系 {#alg-v-s10-n4-cor-1 .statement tag=06MQ}

— $V_0$ を $K$ 上のベクトル空間とし、$W$ を $N \otimes_K V_0$ のサブ N 空間ベクトルとします。 $W$ がすべての $\sigma \in \Gamma$ に対して写像 $\sigma \otimes \mathrm{Id}_{V_0}$ で安定しているとします。 $W_0$ を $x \in V_0$ の集合とし、$1 \otimes x \in W$ とします。この場合、$W_0$ は、$W = N \otimes_K W_0$ となる、$V_0$ の一意のベクトルサブ K 空間です。

It suffices to remark that the set of elements of the form $1 \otimes x \ (x \in V_0)$ is a K-structure on $N \otimes_K V_0$ for which we have $u_\sigma = \sigma \otimes \mathrm{Id}_{V_0}$ for $\sigma \in \Gamma$.

#### 命題 7 {#alg-v-s10-prop-7 .statement tag=06MR}

— $V$ を $N$、$(u_\sigma)_\sigma$ 上でベクトル空間とし、$V$ の写像をそれ自体満たす (1) から (4) および $x \in V$ の $V_0$ 集合として、すべてが $u_\sigma(x) = x$ になるようにします。 $\sigma \in \Gamma$。

a) $V_0$ は、$V$ のベクトルサブ K 空間と $N \otimes_K V_0$ の K-線型写像 $\varphi$ を $V$ に変換したもので、写像 $\lambda \otimes x$ ～ $\lambda x$ は単射です。

b) $\Gamma$ が有限である場合、$\varphi$ は全単射であり、$V_0$ は $V$ 上の K 構造です。

$V_0$ が $V$ のベクトルサブ K 空間であることは明らかです。

公式 $u_\sigma \circ \varphi = \varphi \circ (\sigma \otimes \mathrm{Id}_{V_0})$ は、$\varphi$ の核 $W$ が写像 $\sigma \otimes \mathrm{Id}_{V_0}$ で安定していることを示します。コルによって。提案 6 に対して、したがって、$W = N \otimes_K W_0$ となるような $V_0$ の部分空間 $W_0$ が存在します。 $x$ 属するから $W_0$ の場合、$x = \varphi(1 \otimes x) = 0$、したがって $W_0 = 0$、したがって $W = 0$ になります。これは a) を証明します。

ここで、$\Gamma$ が有限であると仮定します。 $\varphi$ が全射であるか、同等に $V_0$ 生成するベクトル N 空間 $V$ であることを示さなければなりません。したがって、$f$ を $V$ 上の N 線形形式とし、その制限から $V_0$ が零であるとします。 $x \in V$ にしましょう。 $V$ の $\lambda \in N$ 元 $y_\lambda = \sum_{\sigma \in \Gamma} u_\sigma(\lambda x)$ ごとに、明らかに属するから $V_0$、よって $f(y_\lambda) = 0$、つまり、
$$
\sum_{\sigma \in \Gamma} f(u_\sigma(x)) \sigma(A) = 0.
$$
デデキントの定理 (V、p. 27、コリント 2) によれば、それぞれの $\sigma \in \Gamma$ に対して $f(u_\sigma(x)) = 0$ が得られます。特に、$\sigma = \varepsilon$ を取ると $f(x) = 0$ が見つかり、これは $f = 0$ を意味します。これは b) を証明します。

$M$ を $N$ よりもベクトル空間とします。それぞれの $\sigma \in \Gamma$ について、$M^\sigma$ を $N$ 上のベクトル空間とし、$M$ と同じ加法群を外部法則 $(A, x) \mapsto \sigma(\lambda) x$ とします。 $V = \prod_{\sigma \in \Gamma} M^\sigma$と書きます。 $V$ の基礎となる加法群は、$\Gamma$ のすべての写像を $M$ に変換したもので、外部法則は次のように定義されます。
$$
(\lambda . h)(\sigma) = \sigma(\lambda) h(\sigma) \quad (\lambda \in N, h \in V, \sigma \in \Gamma).
$$
(積 $\sigma(\lambda) h(\sigma)$ はベクトル空間 $M$ で計算されます。) さらに、$N \otimes_K M$ ベクトル空間構造を $N$ 公式で定義するとします。
$$
\lambda \left( \sum_i \mu_i \otimes x_i \right) = \sum_i \lambda \mu_i \otimes x_i
$$
最後に、$N \otimes_K M$ の $\psi$ K-線型写像を、関係によって特徴付けられる $V$ に表します。
$$
\psi(\lambda \otimes x)(\sigma) = \sigma(\lambda) . x
$$
$A \in N, x \in M$と$\sigma \in \Gamma$の場合。 $\psi$ が N 線形であることは明らかです

#### 命題 8 {#alg-v-s10-prop-8 .statement tag=06MS}

— *N 線形写像* $\psi$ *of* $N \otimes_K M$ *into* $V = \prod_{\sigma \in \Gamma} M^\sigma$ *は単射であり、* $\Gamma$ *が有限である場合は全単射です*。

$a \in \Gamma$ごとに、$V$の定義する写像$u_\sigma$を$V$にします。

$$
(u_\sigma h)(\tau) = h(\tau \sigma)
$$

$h \in V$ と $\tau \in \Gamma$ の場合。 *(1)～(4)*の検証は明らかです。すべての $\sigma \in \Gamma$ に対して $u_\sigma(h) = h$ となるように、$h \in V$ の $V$、集合で表します。それぞれの $x \in M$ について、$\theta(x)$ を $\Gamma$ の定数写像として、値 $x$ を使用して $M$ に変換します。この場合、$\theta$ は $V$ に対する $M$ の K-同型写像です。上記のように定義する準同型 $\varphi : N \otimes_K V, \to V$ とすると、$\psi = \varphi \circ (\mathrm{Id}_N \otimes \theta)$ が得られ、提案 8 は提案 7 の後に続きます。

#### 系 {#alg-v-s10-n4-cor-2 .statement tag=06MT}

— *$\psi$ *を* $N \otimes_K N$のK-線型写像 *を積ベクトル空間* $N^\Gamma$ *として* $\psi(x \otimes y)\,(a) = \sigma(x)\,y$ *for* $x,\,y$ *in* $N$ *and* $\sigma \in \Gamma$。 *そのとき* $\psi$ *は単射であり、* $\Gamma$ *が有限であるとき*は全単射です。

これは、提案 8 の特定のケース $M = N$ です。

#### 注意 1 {#alg-v-s10-n4-rem-1 .statement tag=06MU}

FをKの拡大とFの部分拡張である$N$とし、$\Gamma$を$N$の自己同型の*有限*群とし、そのうちKは不変量の体とします。提案 8 は、$x \in N,\,y \in F$ と $\sigma \in \Gamma$ に対して $\theta(x \otimes y)\,(a) = \sigma(x)\,y$ によって特徴付けられる K-代数 $0 : N \otimes_F F \to F^\Gamma$ の同型の存在を意味します。

#### 注意 2 {#alg-v-s10-n4-rem-2 .statement tag=06MV}

記法 K、N、$\Gamma$ は前にと同じ意味です。それぞれの整数 $n \geqslant 1$ について、$A_n$ を $N$ と同一の n K-代数のテンソル積とします。 $B_n$ を $\Gamma^{n-1}$ の写像の集合を $N$ にします。 $n$の帰納法までに、コルから推測できます。提案 8 の同型 $\varphi_n : A_n \to B_n$、写像 $x_1 \otimes \ldots \otimes x_n$ ～ 写像 $(\sigma_1, \ldots, a, ) \quad \sigma_1(x_1) \cdot \sigma_n(x_{n-1})\,x_n$ の存在。

### 5. *ガロアコホモロジー*

Let $N$ be a field, $\Gamma$ a *finite* group of automorphisms of $N$ and K the field of invariants of $\Gamma$. すべての整数 $n \geqslant 1$ を、$N$ の係数とゼロ以外の行列式 (II; p. 349) を使用して、位数 $n$ の正方行列の $\mathbf{GL}(n, N)$ 群で表します。 $A = (a_{ij})$ に対するルール $\sigma(A) = (\sigma(a_{ij}))$ に従って、群 $\Gamma$ を群 $\mathbf{GL}(n, N)$ に作用させます。

#### 命題 9 {#alg-v-s10-prop-9 .statement tag=06MW}

— *$(U_\sigma)_{\sigma \in \Gamma}$ *$\mathbf{GL}(n, N)$ の元の家族としましょう。 *のために* $A$ *存在する* $GL(n, N)$ *そのように* $U_\sigma = A^{-1}\,a(A)$ *すべてのために* $\sigma \in \Gamma$ *それは必要十分* $U_{\sigma \tau} = U_\sigma \cdot \sigma(U_\tau)$ *のために* $\sigma,\,\tau$ *に* $\Gamma$。

条件は *必須*: $U_\sigma = A^{-1}\,a(A)$ の場合、

$$
U_\sigma \cdot \sigma(U_\tau) = A^{-1}\,\sigma(A)\,\sigma(A^{-1}\,\tau(A)) = A^{-1}\sigma\tau(A) = U_{\sigma \tau}.
$$

条件は *十分* です。: $n$ 行の行列を持つ $N^n$ の同一視する元と、$N$ の係数を持つ 1 つの列です。 群 $\Gamma$ を $N^n$ に作用させます。
$$
\sigma(x) = (\sigma(x_i))_{1 \leq i \leq n} \quad \text{for} \quad x = (x_i)_{1 \leq i \leq n}.
$$
それぞれの $a \in \Gamma$ を、$N^n$ の $u_\sigma$ 写像 $x \mapsto U_\sigma \cdot \sigma(x)$ で表します。 V、p. 62の式(1)～(3)の検証は明らかです。さらに、$u_\varepsilon \circ u_\varepsilon = u_\varepsilon$ があり、$u_\varepsilon$ は全単射なので、$u_\varepsilon = \mathrm{Id}_{N^n}$ があります。 $V_0$ を $\sigma \in \Gamma$ すべてに対して $u_\sigma(x) = x$ となるように、ベクトル $x \in N^n$ の集合とします。提案 7 (V、p. 63) により、$V_0$ は $N^n$ 上の K 構造です。特に、$V_0$ ベクトル $b_1, \ldots, b_n$ には、$N$ を超えて $N^n$ の基底が形成されます。したがって、行列 $B$ と列 $b_1, \ldots, b_n$ は反転可能であり、$1 \leq i \leq n$ の関係 $u_\sigma(b_i) = b_i$ は $U_\sigma \cdot \sigma(B) = B$ と同等です。 $A = B^{-1}$と書くと、すべての$a \in \Gamma$に対して$U_\sigma = A^{-1} \sigma(A)$が得られます。

#### 系 1 {#alg-v-s10-prop-9-cor-1 .statement tag=06MX}

*$(c_\sigma)_{\sigma \in \Gamma}$ を $N$ の非ゼロ元の族とする。 $a \neq 0$ がすべての $\sigma \in \Gamma$ に対して $c_\sigma = \sigma(a) \cdot a^{-1}$ となるように $N$ に存在するには、$\Gamma$ の $\sigma, \tau$ に対して $c_{\sigma \tau} = c_\sigma \cdot \sigma(c_\tau)$ が存在することが必要かつ十分です。

#### 系 2 {#alg-v-s10-prop-9-cor-2 .statement tag=06MY}

※$(a_\sigma)_{\sigma \in \Gamma}$を$N$の元の家族とします。 $b$ がすべての $\sigma \in \Gamma$ に対して $a_\sigma = \sigma(b) - b$ となるように $N$ に存在するには、$\Gamma$ の $\sigma, \tau$ に対して $a_{\sigma \tau} = a_\sigma + \sigma(a_\tau)$ が存在することが必要かつ十分です。

$N$ のすべての $b$ と $\Gamma$、よっての $\sigma, \tau$ に対して $\sigma \tau(b) - b = [\sigma(b) - b] + \sigma[\tau(b) - b]$ があります。

逆に、$\Gamma$ の$\sigma$ と $\tau$ が$a_{\sigma \tau} = a_\sigma + \sigma(a_\tau)$ であるとします。 $\sigma \in \Gamma$ に $U_\sigma = \begin{pmatrix} 1 & a_\sigma \\ 0 & 1 \end{pmatrix}$ を入れます。次に、$\Gamma$ の $\sigma, \tau$ に対して $U_{\sigma \tau} = U_\sigma \cdot \sigma(U_\tau)$ が得られます。提案 9 により、すべての $a \in \Gamma$ に対して $\sigma(A) = A U_\sigma$ となるような非ゼロ行列式を持つ行列 $A = \begin{pmatrix} x & y \\ z & t \end{pmatrix}$ が存在します。 関係 $\sigma(A) = A U_\sigma$ を書き留めます
$$
\begin{pmatrix} \sigma(x) & \sigma(y) \\ \sigma(z) & \sigma(t) \end{pmatrix} = \begin{pmatrix} x & x a_\sigma + y \\ z & z a_\sigma + t \end{pmatrix} \quad (\sigma \in \Gamma).
$$
特に、$x$ と $z$ 属するから $K$ まで、
$$
\sigma(y) = x a_\sigma + y, \quad \sigma(t) = z a_\sigma + t \quad (\sigma \in \Gamma).
$$
$x \neq 0$ の場合、$b = x^{-1} y$ を含む $a, = \sigma(b) - b$ が得られます。 $z \neq 0$ の場合、$b = z^{-1} t$ と同じ関係になります。これで、$x$ と $z$ できないは両方とも零になります。
$$
xt - yz = \det A \neq 0.
$$

### 6. アーティンの定理

#### 定理 2 (アーティン) {#alg-v-s10-thm-2 .statement tag=06MZ}

— *$N$ を、$N$ の自己同型の体、$\Gamma$ 群、および $\Gamma$ の不変式の $K$ 体とします。 $V$ を、K 上の有限次元* の $N$ のベクトルサブ K 空間とします。すると、N に入る V のすべての K-線型写像 u は、線形結合となり、制限 ～ V の N には係数が入ります。 $\Gamma$中元。

u を V の K-線型写像を N にし、$V_{(N)} = N \otimes_K V$ を V からスカラーの拡大で導出されたベクトル N 空間とします。 $x \in N$ と $y \in V$ に対して $\tilde{u}(x \otimes y) = x \cdot u(y)$ となるような、$V_{(N)}$ 上の N 線形形式を $\tilde{u}$ で示します。 それぞれの $a \in \Gamma$ に対して、$x \in N$ と $y \in V$ に対して $h_\sigma(x \otimes y) = x \sigma(y)$ となるような、$V_{(N)}$ 上の N 線形形式 h が存在します。 $V_{(N)} = N \otimes_K V$ の $N \otimes_K N$ への標準写像は単射です。 さて、コル。提案 8 の (V, p. 64) は、$V_{(N)}$ で線型形式 h の核の共通部分が 0 に減少することを示します。 したがって (II、p. 302、コリント 1) $\Gamma$ には $a_1, \ldots, \sigma_n$、$N$ には $a_1, \ldots, a_n$ が存在し、すべての $x \in V$ に対して $\tilde{u} = \sum_{i=1}^n a_i h_{\sigma_i}$ よって $u(x) = \sum_{i=1}^n a_i \sigma_i(x)$ が存在します。

N のすべての写像の集合 $N^N$ に、因子の離散トポロジーの積位相を N に装備しましょう。 Th. 2は、$\Gamma$の元のNに係数を含む線形結合の集合が、NのK-線型写像の集合でそれ自体に密集していることを意味します。

#### 定理 3 {#alg-v-s10-thm-3 .statement tag=06N0}

— N を、N の自己同型の体、$\Gamma$ 有限群、および $\Gamma$ の不変量の K 体とします。 n を $\Gamma$ の基数とします。
a) $[N : K] = n$ があり、N はガロア群 $\Gamma$ を持つ K のガロア拡大です。
b) $\sigma_1, \ldots, \sigma_n$ を $\Gamma$ の元と K 上の N の $(x_1, \ldots, x_n)$ 基底とし、$\det (\sigma_i(x_j)) \neq 0$ とします。
c) u を N の K-線型写像を N にするとします。すべての $x \in N$ に対して $u(x) = \sum_{\sigma \in \Gamma} a_\sigma \sigma(x)$ となるような、N の元の一意の族 $(a_\sigma)_\sigma$ が存在します。

環 $N \otimes_K N$ に N 代数構造を装備します。その外部法則は N の $\lambda, x, y$ に対して $\lambda(x \otimes y) = x \otimes \lambda y$ によって与えられます。そのとき、ベクトル N 空間 $NO, N$ の次元は $[N : K]$ です。 積ベクトルの次元 N スペース $N^\Gamma$ は n に等しい。 写像 $\psi$ は Cor.提案 8 の (V, p. 64) は、$N^\Gamma$, よって $[N : K] = n$ に対する $NO, N$ の N-同型写像です。 A を N の K 自己同型の群とします。$\Gamma \subset A$ があるため、K は A の不変量の体であり、N は K のガロア拡大です。さらに、A の位数は、デデキントの定理により、最大でも $[N : K]$ に等しくなります。 (V、p. 27、コリント 2) そして、$\Gamma$ の位数は $[N : K]$ に等しいので、$\Gamma = A$ になります。したがって、$\Gamma$ は K 上の N のガロア群であり、これは a) を証明します。

b)の記法に$f_i = \psi(x_i \otimes 1)$を入れます。 $1 \leq i \leq n$ と $\sigma \in \Gamma$ には $f_i(\sigma) = \sigma(x_i)$ があります。 $\psi$ はベクトル N 空間の同型であるため、数列 $(f_1, \ldots, f_n)$ は N 上の N の基底、よって $\det (f_j(\sigma_i)) \neq 0$、つまり、

$$
\det (\sigma_i(x_j)) \neq 0
$$

これは b) を証明します。

Finally, c) follows from Th. 2 (V, p. 65) which proves the existence of a family $(a_\sigma)_{\sigma \in \Gamma}$ such that $u(x) = \sum_{\sigma \in \Gamma} a_\sigma \sigma(x)$ (for all $x \in N$) and from Dedekind's theorem (V, p. 27, Cor. 2) which proves the uniqueness of $(a_\sigma)_{\sigma \in \Gamma}$.

### 7. ガロア理論の基本定理

#### 定理 4 {#alg-v-s10-thm-4 .statement tag=06N1}

— N を K のガロア拡大とし、$\Gamma$ をそのガロア群とします。 $\mathscr{K}$ を N の部分拡張の集合と、$\Gamma$ の閉じた部分群の $\mathscr{G}$ 集合とします。 すべての部分群 $A \in \mathscr{G}$ を A の不変量の $k(\Delta)$ 体で表し、すべての *部分体* $E \in \mathscr{K}$ を N の E-*自己同型* の $g(E)$ 群で表します。 *すると* $A \mapsto k(\Delta)$ は $\mathscr{G}$ の $\mathscr{K}$ 上の全単射であり、 $E \mapsto g(E)$ は逆全単射です。

A) 関係 $E = k(g(E))$ ($E \in \mathscr{K}$ の場合) は、以下のより正確な補題の帰結です。

#### 補題 1 {#alg-v-s10-lem-1 .statement tag=06N2}

E を N の部分拡張とします。その場合、N は E のガロア拡大であり、$\mathrm{Gal}(N/E)$ は誘導位相を伴う $\mathrm{Gal}(N/K)$ の閉じた部分群です。

$x \in N$ にしましょう。 $E[X]$ における E 割る上の x の最小多項式 f K 上の x の最小多項式 $g$ (V, p. 17, Cor. 2)。 N は K 上のガロアであるため、多項式 g は次数 1 の別個の因子の $N[X]$ で積です。したがって、同じことが f にも当てはまり、N は E 上のガロアになります。

$\Gamma$ を K 上の N のガロア群とし、A を E 上の N のガロア群とします。 定義により、A はすべての $x \in E$ に対して $\sigma(x) = x$ となるように、すべての $\sigma$ のうち $\Gamma$ からなるの部分群になります。 ここで、$\Gamma$ の各 $x \in E$ 写像 $\sigma \mapsto \sigma(x)$ を離散空間に変換すると、N は連続であるため、D は $\Gamma$ で閉じられます。 $\sigma \in \Gamma$ にしましょう。 N の $x_1, \ldots, x_n$ について、$U(x_1, \ldots, x_n)$ をすべての $\tau \in \Gamma$ の集合とし、$1 \leq i \leq n$ については $\tau(x_i) = \sigma(x_i)$ とします。置く

$$
V(x_1, \ldots, x_n) = U(x_1, \ldots, x_n) \cap \Delta.
$$

すると、集合 $U(x_1, \ldots, x_n)$ (それぞれ $V(x_1, \ldots, x_n)$) の族は、$\Gamma$ (それぞれ A) の $\sigma$ の近傍の基底になります。したがって、A 上の位相は、$\Gamma$ によって誘発されたものです。

B) 関係 $A = g(k(\Delta))$ ($A \in g$ の場合) は、以下のより正確な補題の帰結です。

#### 補題 2 {#alg-v-s10-lem-2 .statement tag=06N3}

A を $\Gamma$ の部分群とします。 E を A の不変量の体とします。すると、E 上の N のガロア群は、$\Gamma$ の A の閉包になります。

The Galois group of N over E is closed in $\Gamma$ (Lemma 1) and contains A, hence it contains the closure $\bar{\Delta}$ of A. $\sigma$ を N の E 自己同型とし、$x_1, \ldots, x_n$ を N に置きます。 Since N is Galois over E (Lemma 1) there exist (V, p. 57, Prop. 2) a subextension $N_0$ of N, Galois of finite degree over E and containing $x_1, \ldots, x_n$. $A_0$ を $\mathrm{Gal}(N/E)$ の制限準同型から $\mathrm{Gal}(N_0/E)$ の $\mathrm{Gal}(N/E)$ の部分群 A の像とします。 $[N_0 : E]$ は有限であるため、デデキントの定理 (V、p. 27、コリント 2) は、$\mathrm{Gal}(N_0/E)$ が有限であることを示しています。 したがって、$A_0$ は有限であり、E は $A_0$ の不変量の体であるため、$\Delta_0 =$ が得られます。

ガル(N_0/E) (V, p. 66, 木 3)。特に$\sigma$から$N_0$の$\Delta_0$含む制限です。したがって、$\sigma$と$\tau$が同じ制限から$N_0$、よって$\sigma(x_1) = \tau(x_1), \ldots, \sigma(x_n) = \tau(x_n)$を持つような$\tau \in A$が存在します。したがって、$\sigma$ は $\Gamma$ の $A$ の極限点であるため、$\mathrm{Gal}(N/E) \subset \overline{\Delta}$ となります。

#### 系 1 {#alg-v-s10-lem-2-cor-1 .statement tag=06N4}

*E と E' を N 含む K の 2 部分体とします。 g(E) $\supset$ g(E') の場合に限り、E $\subset$ E' になります。 A と A' が 2 つの閉じた $\Gamma$ 部分群である場合、k($\Delta$) $\supset$ k($\Delta'$) の場合に限り、A $\subset$ A' になります。*

2 つの逆全単射 $E \rightleftharpoons g(E)$ と $A \rightleftharpoons k(\Delta)$ は包含反転です。

#### 系 2 {#alg-v-s10-lem-2-cor-2 .statement tag=06N5}

*$(E_i)_{i \in I}$ を N 含む K の部分体の家族とします。 $L = \bigcap_{i \in I} E_i$と$M = K\left( \bigcup_{i \in I} E_i \right)$を入れます。 Then g(L) is the smallest closed subgroup of containing $U_{i \in I} g(E_i)$ and we have $g(M) = \bigcap_{i \in I} g(E_i)$.*

最初の主張は Cor から続きます。 1、2 番目は明らかです。

#### 系 3 {#alg-v-s10-lem-2-cor-3 .statement tag=06N6}

*i = 1, 2 の場合、$E_i$ を N 含む K の部分体とし、$\Delta_i = g(E_i)$ とします。任意の $\sigma \in \Gamma$ 関係 $\sigma(E_1) = E_2$ と $\sigma \Delta_1 \sigma^{-1} = \Delta_2$ は同等です。*

なぜなら、$\tau \sigma(x) = \sigma(x)$、つまり$\sigma^{-1} \tau \sigma(x) = x$、すべての$x \in E_1$の場合に限り、$\tau \in g(\sigma(E_1))$があるからです。これは、$\sigma^{-1} \tau \sigma \in \Delta_1$、よって $g(\sigma(E_1)) = \sigma \Delta_1 \sigma^{-1}$ のというに相当します。

#### 系 4 {#alg-v-s10-lem-2-cor-4 .statement tag=06N7}

*E を N 含む K の部分体とし、$A = g(E)$ とします。 E が K 上のガロアであるためには、A が $\Gamma$ の正規の部分群であることが必要かつ十分です。そうなると、$\Gamma$の制限準同型は$\mathrm{Gal}(E/K)$定義するに、商への通過によって、$\Gamma / \Delta$のトポロジカル群同型は$\mathrm{Gal}(E/K)$へ*となります。

N は K 上で分離可能であるため、同じことが E にも当てはまります (V, p. 36、提案 1)。したがって、E は K 上の準ガロアである場合に限り、K 上のガロアです。これは、N のすべての K 自己同型 $\sigma$ に対して $\sigma(E) = E$ であることも意味します (V、p. 52、提案 1 および p. 54、提案 3)。コル著3 これは、すべての $\sigma \in \Gamma$ の $\sigma \Delta \sigma^{-1} = A$ に相当します。

制限準同型 $\varphi : \mathrm{Gal}(N/K) \to \mathrm{Gal}(E/K)$ は連続かつ全射的であり (V、p. 60、提案 3)、その核は明らかに $A = \mathrm{Gal}(N/E)$ に等しい。 $\Gamma$ はコンパクトなので、$\varphi$ から商への通過によって導出される $\mathrm{Gal}(E/K)$ への $\Gamma / \Delta$ の準同型は、トポロジカル群の同型になります (Gen. Top., I, p. 87, Cor. 2)。

#### 系 5 {#alg-v-s10-lem-2-cor-5 .statement tag=06N8}

*E を N 含む K の部分体とする。E が K に対して有限次数を持つためには、g(E) が $\Gamma$ で開いていなければならないことが必要かつ十分である。この場合、添字 $(\Gamma : g(E))$ は有限であり、[E : K] に等しくなります。*

$g(E)$ がオープンであるためには、V、p. 60 の記法のように、K 上の有限次数の N の部分拡張子 F が存在することが必要かつ十分です。

g(E) 含む $U_F(\mathrm{Id}_N) = g(F)$。 関係 $g(E) \supset g(F)$ は Cor による $E \subset F$ と同等です。 1 (V、p. 68)、よってコルの最初の主張 5.

$[E : K]$ が有限であると仮定します。 $\Omega$ を部分拡張 (V、p. 23、Th. 2) として $K$ 含む $N$ の代数閉包とし、$\mathscr{H}$ を $E$ の $K$ 準同型射の集合とします。 $\Omega$に。 $\mathscr{H}$ のすべての元は、$\Omega$ の $K$ 自己同型 (V、p. 52、提案 1) によって誘導され、$N$ は $K$ 上の準ガロアであるため、写像 $\sigma \mapsto \sigma|_E$ $\Gamma$ から $\mathscr{H}$ は全射です。 $\Gamma$の$\sigma$と$\sigma'$が同じ制限から$E$を持つためには、$\sigma^{-1}\sigma' \in g(E)$、よってのカード$A? = (\Gamma : g(E))$が必要十分です。 最後に、$E$ は $K$ に対するエタール代数であるため、カード $\mathscr{H} = [E : K]$ (V、p. 32、提案 4) があり、結論としては $(\Gamma : g(E)) = [E : K]$ になります。

#### 系 6 {#alg-v-s10-lem-2-cor-6 .statement tag=06N9}

— $i = 1, 2$ の場合、$E_i$ を $E_i$ に対する $N$ と $\Gamma_i$ ガロア群の $N$ の部分拡張とします。次の条件は同等です。
a) 群 $\Gamma$ は、部分群 $\Gamma_1$ と $\Gamma_2$ の直接の積です。
b) 拡大 $E_1$ と $E_2$ は $K$ に対するガロアであり、$E_1 \cap E_2 = K$ があり、
$$
K(E_1 \cup E_2) = N .
$$

$\Gamma$ が部分群 $\Gamma_1$ と $\Gamma_2$ の直接の積であるためには、次の条件が成立することが必要かつ十分です (I、p. 48、提案 15)。
(i) 部分群 $\Gamma_1$ と $\Gamma_2$ は $\Gamma$ では正常です。
(ii) $\Gamma_1 \cap \Gamma_2 = \{ \varepsilon \}$、$\varepsilon$ は$\Gamma$ の中立元です。
(iii) $\Gamma = \Gamma_1 . \Gamma_2$。

ここで (i) は、$E_1$ と $E_2$ が $K$ 上のガロアであることを意味します (Cor. 4)。コル著2、条件 (ii) は $N = K(E_1 \cup E_2)$ と同等であり、最後に (i) と (ii) が成立する場合、$\Gamma_1 \Gamma_2$ は $\Gamma$ 含む $\Gamma_1 \cup \Gamma_2$ の最小の部分群です。 $\Gamma_1$と$\Gamma_2$がコンパクトで、$\Gamma_1 \times \Gamma_2$の$\Gamma$への写像$(a, \tau) \mapsto \sigma \tau$が連続しているため閉じられます（Gen.Top.、I、p. 63、Cor.1）。コル。 2 は (iii) が $E_1 \cap E_2 = K$ に相当することを示しており、これは a) と b) の同値を証明します。

#### 注意 {#alg-v-s10-n7-rem-1 .statement tag=06NA}

コルの記法と6 条件 a) と b) が成り立つと仮定します。 $i = 1, 2$ 誘導するトポロジカル群同型の制限準同型 $\varphi_i : \Gamma \to \mathrm{Gal}(E_i/K)$
$$
\Psi_1 : \Gamma_2 \to \mathrm{Gal}(E_1/K) , \quad \Psi_2 : \Gamma_1 \to \mathrm{Gal}(E_2/K)
$$
a) によって、写像 $\sigma \mapsto (\varphi_1(\sigma), \varphi_2(\sigma))$ が $\mathrm{Gal}(E_1/K) \times \mathrm{Gal}(E_2/K)$ 上での $\mathrm{Gal}(N/K)$ のトポロジカル群同型であることがわかります。

### 8. 基礎体中変更

Let $N$ be a Galois extension of $K$ and $\Gamma$ the Galois group of $N$ over $K$; further let $N'$ be a Galois extension of $K'$ with Galois group $\Gamma'$. 同一視する $K$ (それぞれ $K'$) を $N$ (それぞれ $N'$) の像とします。 $u$を$K$の準同型を$K'$に、$v$を$N$の準同型を$N'$にするとします。その制限から$K$は$u$（cf.）に等しくなります。

図1）。 $\sigma \in \Gamma'$ にしましょう。 $u(K) \subset K'$ なので、$a$ は $N'$ の $u(K)$ 自己同型です。さらに、$v(N)$ は $u(K)$ のガロア拡大であるため、$a$ 誘導するは $v(N)$ (V, p. 55, 注意 1) の $u(K)$ 自己同型です。他の語では、$\sigma \in \Gamma'$ ごとに $\Gamma$ の一意元 $v^*(\sigma)$ が存在します。

(8)

$$
v \circ v^*(\sigma) = \sigma \circ v .
$$

![N、N'、K、K' の間の写像 v と u を示す図式](図 1)

写像 $v^*$ は、$\mathrm{Gal}(N'/K')$ の準同型を $\mathrm{Gal}(N/K)$ に変換したものです。 $\Gamma'$ のすべての $x \in N$、写像 $a \mapsto v^*(o)(x) = v^{-1}(\sigma(v(x)))$ を離散空間 $N$ は連続であるため、$v^*$ は連続です。

3 つの特定のケースが重要です。

a) $F$ が $K$ のガロア拡大であり、$E$ が $F$ の部分拡張である場合、$F$ が $E$ のガロア拡大であることがわかります (V、p. 67、補題 1)。これまで述べたことを、$N = F$、$K' = E$、$N' = F$、$v = \mathrm{Id}_F$ の場合に当てはめてみましょう。その場合、$v^*$ は単に標準単射になります

$$
j : \mathrm{Gal}(F/E) \to \mathrm{Gal}(F/K) .
$$

これはインフレーション準同型と呼ばれるときどきです。

b) 加法 $E$ が $K$ 上のガロアであると仮定します。 $N = E$、$K' = K$、$N' = F$、$v$が$E$の標準単射である場合を$F$に当てはめてみましょう。すると、$v^*$はちょうど制限準同型になります

$$
\pi : \mathrm{Gal}(F/K) \to \mathrm{Gal}(E/K)
$$

V、p. 60、提案 3) $\pi$ は核 $\mathrm{Gal}(F/E)$ で全射的であり、商を定義するとすることで $\mathrm{Gal}(F/K)/\mathrm{Gal}(F/E)$ の位相幾何学的群同型を $\mathrm{Gal}(E/K)$ に当てはめることができます。 (V、p. 68、コリント 4)。

c) $v^{-1}(K') = K$ と $N' = K'(v(N))$ を仮定します。 準同型を見せてみましょう

$$
v^* : \mathrm{Gal}(N'/K') \to \mathrm{Gal}(N/K) ,
$$

は、翻訳と呼ばれる位相的な群同型, ときどきです。 群 $\mathrm{Gal}(N'/K')$ はコンパクト、群 $\mathrm{Gal}(N/K)$ は分離、$v^*$ は連続です。それで十分です（Gen. トップ、I、p. 87、Cor. 2) $v^*$ が全単射であることを証明する。 Now every element $\sigma$ of the kernel of $v^*$ is an automorphism of $N'$ which induces the identity on $K'$ and on $v(N)$, hence $a = \epsilon$ because $N' = K'(v(N))$; it follows that $v^*$ is injective. さらに、$v^*$ の像は、$\mathrm{Gal}(N/K)$ のクローズド部分群 $A$ です。

(Gen. Top., I, p. 81, *ibid.*) および $A$ の不変式の体は $v^{-1}(K') = K$ に等しい。したがって、$A = \mathrm{Gal}(N/K)$ (V, p. 67, Th. 4) があり、$v^*$ は全射です。

一般的なケースは、合成までに前述のケースに帰着する可能性があります。まず、$K'(v(N))$ は、核の $N'$ $v^*$ の $A$ における不変式の体であることに注意します。 $A$ は $\mathrm{Gal}(N'/K')$ の正規の部分群であるため、$K'$ の拡大 $K'(v(N))$ はガロア (V、p. 68、Cor. 4) です。したがって、$v^*$ は準同型で構成されます

$$
\mathrm{Gal}(N'/K') \to \mathrm{Gal}(K'(u(N))/K') \xrightarrow{\psi} \mathrm{Gal}(N/v^{-1}(K')) \xrightarrow{j} \mathrm{Gal}(N/K);
$$

この数列 $\pi$ はトリプル $K' \subset K'(u(N)) \subset N'$ に関連付けられた制限準同型であり、$\psi$ は図式の中央の平方に関連付けられた翻訳同型 (図 2)、および $j$ はトリプルに関連付けられたインフレーション準同型です$K \subset v^{-1}(K') \subset N$。

次の定理では、翻訳同型の構造についてさらに詳しく説明します。

![図式は拡大とその翻訳を表示しています](fig2.png)

図2

#### 定理 5 {#alg-v-s10-thm-5 .statement tag=06NB}

*$N'$ を 2 つのサブ拡張子 $K'$ と $N$ によって生成された $K$ の拡大とします。 $N$ が $K$ 上のガロアで、ガロア群 $\Gamma$ と $K' \cap N = K$ があるとします。 この場合、$K'$ の拡大 $N'$ はガロアであり、$K' \otimes_K N$ の $N'$ への標準準同型 $\varphi$ は同型です。 $\sigma \in \mathrm{Gal}(N/K)$ と $\sigma'$ を $\mathrm{Gal}(N'/K')$ の元とし、翻訳同型の下ではそれに対応するを加えます。そうすると $\sigma' \circ \varphi = \varphi \circ (\mathrm{Id}_{K'} \otimes u)$ になります。*

$N' = K'(N)$ があり、$N$ は代数的であり、$K$ に関して分離可能です。したがって (V, p. 42, 提案 10)、$K'$ の拡大 $N'$ は代数的で分離可能です。コル著V の 4、p. 54 拡大 $K'$ の $N'$ は準ガロアです。したがって、$K'$ の拡大 $N'$ はガロアです。 c) 上記の写像 $\sigma \mapsto \sigma|_N$ は、$\mathrm{Gal}(N/K)$ 上の $\mathrm{Gal}(N'/K')$ の準同型 $\lambda$ です。

$N = K'[N]$ があるのは、$N$ が $K$ (V, p. 18, Cor. 1) に対して代数的であるため、$\varphi$ が全射であるからです。 $a$ 属するから $\mathrm{Gal}(N/K)$ の場合、

$$
\lambda^{-1}(\sigma) \circ \varphi = \varphi \circ (\mathrm{Id}_{K'} \otimes \sigma).
$$

したがって、$\varphi$ の核は写像 $\mathrm{Id}_{K'} \otimes \sigma$ で安定し、したがって形 $K' \otimes_K N_0$ と $N_0 \subset N$ (V、p. 63、Cor.) が安定します。 $N_0$ の $x$ には $x = \varphi(1 \otimes x) = 0$ があるため、$N_0 = 0$ となり、$\varphi$ は単射法になります。

#### 系 1 {#alg-v-s10-thm-5-cor-1 .statement tag=06NC}

*$E'$を$N'$含む$K'$の部分体とします。 $N$ 含む $K$ や $E' = K'(E)$ などの固有の部分体 $E$ が存在します。 $E = E' \cap N$ があります。*

$E = E' \cap N$を入れてから、$E' \supset K'(E)$を入れます。次に、$\Gamma = \mathrm{Gal}(N/K)$ と $A = \mathrm{Gal}(N/E)$ 、定義する $\Gamma'$ と $A'$ を同様に置きます。 写像 $A : a \mapsto a|_N$ は、$\Gamma$ に対する $\Gamma'$ の同型であり、また $A$ に対する $A'$ の同型です。他の語、$A'$は$\sigma \in \Gamma'$のうち$\lambda(\sigma)$属するから$A$で構成されます。 $\sigma \in \Gamma'$ が $K'(E)$ の元を固定した場合、$\lambda(\sigma) \in A$、よって $a \in A'$、そして $a$ が $E'$ の元を固定します。コル著V、p. 68 の 1 なので、$K'(E) \supset E'$ になります。

等式 $E' = K'(E)$、よって $\varphi^{-1}(E') = K' \otimes_K E$ を証明しました。 $F$ が $N$ 含む $K$ の部分体で、$E' = K'(F)$ である場合、同様に $\varphi^{-1}(E') = K' \otimes_K F$、よって $F = E$ になります。

#### 系 2 {#alg-v-s10-thm-5-cor-2 .statement tag=06ND}

*$N$を$K$のガロア拡大とします。 Suppose that the Galois group $\Gamma$ of $N$ over $K$ is the direct product of two closed subgroups $\Gamma_1$ and $\Gamma_2$ and denote by $E_i$ the field of invariants of $\Gamma_i$ for $i = 1, 2$. すると、$E_1 \otimes_K E_2$ の $N$ への標準準同型は同型になります。*

Cor の $E_1 \cap E_2 = K$ と $N = K(E_1 \cup E_2)$ があります。 6 (V、p. 69) なので、定理を適用する 5 で十分です。

#### 注意 {#alg-v-s10-n8-rem-1 .statement tag=06NE}

$K$と$K'$を、$K$の2つの体と$u$準同型を$K'$にします。 $K_s$ (それぞれ $K'_s$) を $K$ (それぞれ $K'$) および $\Pi$ (それぞれ $\Pi'$) ガロア群の分離閉包 (V、p. 45、提案 14) とします。 $K_s$ が $K$ を超えます (それぞれ $K'_s$ が $K'$ を超えます)。 Since $K_s$ is a separable algebraic extension of $K$ and the extension $(K'_s, u)$ of $K$ is separably closed, there exists (V, p. 45, Cor.) a homomorphism $v$ of $K_s$ into $K'_s$ extending $u$. $v$ から $\Pi'$ から $\Pi$ までの連続した準同型 $v^*$ が得られます。 $v_1$ を $u$ の他の拡大とします。 $K_s$ は $K$ の準ガロア拡張であるため、$v_1 = v \circ a_s$ となるような $\Pi$ の元 $a_s$ が存在します。 私たちは結論する、すべての$\tau \in \Pi$に対して$v_1^*(\tau) = \sigma_0^{-1} v^*(\tau) \sigma_0$です。

### 9. 通常の基底定理

$N$ を $K$ のガロア拡大とし、ガロア群 $\Gamma$ とします。私たちは同一視する $\Gamma$ と群代数 $K^{(\Gamma)}$ (III、p. 446) の標準基底です。その場合、$N$ は左の $K^{(\Gamma)}$ モジュール (III、p. 447、例) と見なされます。

$$
u \cdot x = \sum_{\sigma \in \Gamma} a_\sigma \sigma(x) \quad \text{for} \quad x \in N \quad \text{and} \quad u = \sum_{\sigma \in \Gamma} a_\sigma \sigma \quad \text{in} \quad K^{(\Gamma)}.
$$

$N$ が $K$ 上の有限次数である場合、群 $\Gamma$ はデデキントの定理 (V, p. 27, Cor. 2) によって有限であり、次のように定義する元 $t = \sum_{\sigma \in \Gamma} a$ ができます。 $K^{(\Gamma)}$;それなら私たちは持っています

$$
\mathrm{Tr}_{N/K}(x) = \sum_{\sigma \in \Gamma} \sigma(x),
$$

つまり、すべての $x \in N$ に対して $\mathrm{Tr}_{N/K}(x) = t \cdot x$ です。

$N$ by $x^\sigma = \sigma^{-1}(x)$ に、$\Gamma$ によって右側の定義する作用を入力しましょう。同様に、乗法群 $N^*$ を右側の $Z^{(\Gamma)}$ モジュールとして考えることができ、外部法則は $(x, u) \mapsto x^u$ と書かれています。たとえば、記法 $x^{2a + 3r + \pi}$ ($a, r, \pi$ は $\Gamma$ の元 ) は、積 $(x^a)^2 \cdot (x^r)^3 \cdot x^\pi$ を示します。上記のように、$N$ が $K$ と $t = \sum_{\sigma \in \Gamma} a$ を超える有限次数である場合、$N_{N/K}(x) = \prod_{\sigma \in \Gamma} x^\sigma$、つまりすべての $x \in N^*$ に対して $N_{N/K}(x) = x'$ が得られます。

今後、$N$ が $K$ に対して有限次数であると仮定します。 $x \in N$ が与えられた場合、$\{x\}$ が $\mathbf{K}^{(\Gamma)}$ モジュール $N$ の基底であるためには、ファミリー $(\sigma(x))_{\sigma \in \Gamma}$ が $K$ 上の $N$ の基底であることが必要かつ十分です。このような基底は、$K$* を超える $N$ の *通常の基底と呼ばれます。

#### 定理 6 {#alg-v-s10-thm-6 .statement tag=06NF}

*$N$ を $K$ の有限次数のガロア拡大とし、$\Gamma$ を $K$ の $N$ のガロア群とします。そして、$K$を超える$N$の通常の基底が存在します。他の語では、$\mathbf{K}^{(\Gamma)}$ モジュール $N$ には階数 1 が含まれていません。*

この主張のうち、証明を2つあげます。最初は次の補題を使用します。これは章 VIII (§ 2, No. 5) で証明されます。

\* Lemma 3. — Let $A$ be a $K$-algebra, $M_1$ and $M_2$ two $A$-modules of finite rank over $K$ and suppose that there exists an extension $L$ of $K$ such that the modules $L \otimes_K M_1$ and $L \otimes_K M_2$ over the ring $L \otimes_K A$ are isomorphic. この場合、$A$ モジュール $M_1$ と $M_2$ は同型です。

$A = \mathbf{K}^{(\Gamma)}$、$M_1 = N$、$M_2 = A$、$L = N$の場合には補題 3を適用します。コルによって。 V、p. 64 の写像 $x \otimes y$ から $\sum x u^1(y) \otimes \sigma$ への $N \otimes_K N$ の $\varphi$ の $N \otimes_K \mathbf{K}^{(\Gamma)}$ への $K$ 同型写像が存在します。 $\varphi$ は $N \otimes_K \mathbf{K}^{(\Gamma)}$ モジュールの同型であるため、定理は補題 3 から続きます。

2 番目の証明には、次の命題を使用します。

#### 命題 10 {#alg-v-s10-prop-10 .statement tag=06NG}

*$x \in N$ とすると、$\mathbf{K}^{(\Gamma)}$ モジュール $N$ の $\{x\}$ から形基底については、$\det(\sigma \tau(x))_{\sigma, \tau \in \Gamma} \neq 0$ であることが必要十分です。

$\mathbf{K}^{(\Gamma)}$と$N$は$K$に対して同じ次元を持っているため、$\{x\}$が$\mathbf{K}^{(\Gamma)}$に対して$N$の基底であるということは、$\mathbf{K}^{(\Gamma)}$の$a \mapsto ax$が$N$に写像であることを意味します。単射的な。 これは、$N \otimes_K \mathbf{K}^{(\Gamma)}$ の $N \otimes_K N$ への写像 $b \mapsto b(1 \otimes x)$ が単射であることを意味します (II, p. 306、提案 14)。 これで、$N \otimes_K N$ の $N \otimes_K \mathbf{K}^{(\Gamma)}$ に写像 $1 \otimes x$ から $\sum \sigma^{-1}(x) \otimes \sigma$ までの $N \otimes_K \mathbf{K}^{(\Gamma)}$ モジュール同型ができました。 したがって、元 $(n_\tau)$ のすべての非ゼロ族について、$N$ の $\left( \sum n_\tau \otimes \tau \right) \left( \sum \sigma^{-1}(x) \otimes \sigma \right) \neq 0$ がある場合に限り、$\{x\}$ は $N$ の $\mathbf{K}^{(\Gamma)}$ の基底になります。 しかし、この最後の関係は、$\sum n_\tau \sigma^{-1}(x) \neq 0$、よって、命題のような$\sigma \in \Gamma$が存在することを意味します。

\* A) $K$ が無限であると仮定します。 $N$ の $N$ への写像 $x \mapsto \det(\sigma \tau(x))$ は、$K$ (IV, p. 54) にわたる多項式写像です。 $K$ から $N$ までのスカラーの拡大により、ベクトル $N$-空間 $N \otimes_K N$ に対して対応する写像が得られ、後者が同じ零ではないことがわかりました（$N \otimes_K N$ は自由であるため） 階数 1 オーバー $N \otimes_K \mathbf{K}^{(\Gamma)}$)。したがって、$\det(\sigma \tau(x)) \neq 0$ (IV, p. 18, Th. 2) となるような $x \in N$ が存在します。より一般的には、同じ参考文献から次のようになります。

#### 命題 11 {#alg-v-s10-prop-11 .statement tag=06NH}

— K が無限大で、P : N → K を K 上で非ゼロの多項式写像とします。 P(x) ≠ 0 であり、{x} が $\mathbf{K}^{(\Gamma)}$ にわたる N の基底であるような x ∈ N が存在します。

B) K が有限であると仮定します。提案 4 (V, p. 95)$^1$ により、K 上の有限次数のすべての拡大には循環ガロア群が存在します。したがって、群 $\Gamma$ が位数 n の循環である場合をより一般的に考えます。 $\Gamma$ の $\gamma$ 生成元で表します。

次の補題は、章 VII で証明されたより一般的な結果の特定のケースです。 環 $A$ は、有理数整数の環 $\mathbf{Z}$ または体 $K$ の多項式の環 $K[X]$ のいずれかです。

#### 補題 4 {#alg-v-s10-lem-4 .statement tag=06NI}

M を元の有限数 $x_1, ..., x_h$ によって生成される捩れ A-加群とします。その場合、消滅子 (II, p. 219) が M の消滅子に等しい M の元 x が存在します。

どちらの場合も、$A$ は整域であり、$A$ のすべての理想が主です。 $A = \mathbf{Z}$ (それぞれ $A = K[X]$) のとき、素数数 (それぞれ $K[X]$ の既約モニック多項式の集合) の $\mathscr{P}$ 集合で表します。 $A$ の元 $a \neq 0$ ごとに、$A$ の可逆元 $u$ と、$a = u \prod_{p \in \mathscr{P}} p^{v_p(a)}$ と $u$ のような有限台、正の整数を含む家族 $(v_p(a))_{p \in \mathscr{P}}$ が存在します。 整数 $v_p(a)$ は一意に決定されます (I、p. 51 および IV、p. 13、提案 13)。

Let $a_i$ be the annihilator of $x_i$, (for $1 \leq i \leq h$) and $a$ the annihilator of M; let $a_1, ..., a_h, a$ be non-zero elements of $A$ such that $a_i = Aa_i$, and $a = Aa$; since $a = a_1 \cap ... \cap a_h$, it follows from what has been said that

$$
v_p(a) = \sup_{1 \leq i \leq h} v_p(a_i) \quad \text{for all } p \in \mathscr{P}.
$$

形 $up_1^{n(1)} ... p_r^{n(r)}$ に $a$ を書き、$A$ の $\mathscr{P}$、$n(1) > 0, ..., n(r) > 0$、$u$ 可逆元で$p_1, ..., p_r$ を区別します。 Let $j = 1, ..., r$; by (10) there exists an integer $c(j)$ such that $1 \leq c(j) \leq h$ and $v_{p_j}(a_{c(j)}) = n(j)$; there exists $b_j$ in $A$ with $a_{c(j)} = p_j^{n(j)} b_j$ and the element $y_j = b_j x_{c(j)}$ has as annihilator the ideal $Ap_j^{n(j)}$.

$y = y_1 + ... + y_r$ の消滅子 b が M の消滅子 a に等しいことを示しましょう。いずれにしても、$a \subset b$ があるので、b は形 $Ap_1^{m(1)} ... p_r^{m(r)}$ で、$1 \leq j \leq r$ に対して $0 \leq m(j) \leq n(j)$ が付きます。もし$a \neq b$があれば、$1 \leq j \leq r$と$m(j) < n(j)$が存在する整数が存在するため、$d_j = a/p_j$は$y$を全滅させます。 $k \neq j$ に対して $d_j y_k = 0$ があり、よっては $d_j y_j = 0$ になります。しかし、$y_j$の消滅子は$Ap_j^{m(j)}$であり、$d_j$は$p_j^{m(j)}$の倍数ではありません。したがって、仮定 $a \neq b$ は不合理です。

$^1$ 読者は、通常の基底定理が命題の前に証明のどこにも使用されていないことを簡単に納得できます。

$A$ が多項式環 $K[X]$ および $M$ アーベル群 $N$ の場合に補題 4 を適用します。$K[X]$ の $a = \sum_{k=0}^\infty c_k X^k$ に対して $a \cdot x = \sum_{k=0}^m c_k \gamma^k(x)$ で定義された外部法則です。そして$x \in N$。 $a$ を $M$ の消滅子とすると、$\gamma^n = 1$ となり、多項式 $X^n - 1$ は $a$ になります。 $F \in a$ にしましょう。 *IV*、p. 11、Cor 著。次のような $K$ と $G \in K[X]$ のうち元 $c_0, c_1, \ldots, c_{n-1}$ が存在します。

$$
F(X) = c_0 + c_1 X + \cdots + c_{n-1} X^{n-1} + (X^n - 1) G(X).
$$

したがって、$\operatorname{Hom}_K(N, N)$ には $c_0 + c_1 \gamma + \ldots + c_{n-1} \gamma^{n-1} = 0$ があり、$N$ の自己同型 $1, \gamma, \gamma^2, \ldots, \gamma^{n-1}$ は別個であるため、デデキントの定理 (*V*, p. 27, Cor. 2) は $c_0 = c_1 = \ldots = c_{n-1} = 0$ を意味します。最後に、

$$
F(X) = (X^n - 1) G(X), \quad \text{that is, } a = (X^n - 1) K[X].
$$

補題 4 までに、$N$ の元 $x$ が存在し、$K[X]$ の消滅子は $(X^n - 1) K[X]$ に等しくなります。 $(X^n - 1) K[X]$ (*IV*, p. 11, Cor.) を補足する単項式 $1, X, \ldots, X^{n-1}$ 形基底のベクトル部分空間 $K[X]$ は、元 $x, \gamma(x), \ldots, \gamma^{n-1}(x)$ $N$ は $K$ に対して線形独立です。 $[N : K] = n$ (*V*, p. 66, Th. 3) なので、数列 $(x, \gamma(x), \ldots, \gamma^{n-1}(x))$ は、$K$ に対する $N$ の (通常の) 基底です。

### 10. 有限$\Gamma$集合とエタール代数

Let $K_s$ be a separable closure of $K$ (*V*, p. 45, Prop. 14) and $\Gamma$ the Galois group of $K$, over $K$. $\Gamma$-*集合* により、$X$ のそれぞれの点の固定群が *open* 部分群であるように、群 $\Gamma$ の作用 $(\sigma, x) \mapsto \sigma x$ を持つ集合 $X$ がわかります。 $\Gamma$の。 $X$ に個別の位相が装備されている場合、$\Gamma \times X$ の $X$ への写像 $(\sigma, x) \mapsto \sigma x$ が *連続* であると言うのと同じになります。

$X$ を *有限* $\Gamma$ 集合とします。 $K$-代数上の$\Gamma$の定義する作用を、公式によって写像の$X$の$K_s^X$を$K_s$にします

$$
u_\sigma f(x) = \sigma(f(\sigma^{-1}x))
$$

$\pi \in \Gamma, f \in K_s^X$ と $x \in X$ の場合。 $\Theta(X)$ を $K_s^X$ の $\Gamma$ の不変量の集合とします。これは、$\sigma \in \Gamma$ と $x \in X$ に対して $f(\sigma x) = \sigma(f(x))$ となる、写像 $f : X \to K_s$ の$K_s^X$ からなるの部分 K 代数です。

#### 補題 5 {#alg-v-s10-lem-5 .statement tag=06NJ}

*$X$を有限の$\Gamma$集合とし、$x_1, \ldots, x_n$を$X$の点とし、$X$の軌道$\Gamma x_1, \ldots, \Gamma x_n$形分割とします。 $1 \leq i \leq n$ について、$\Delta_i$ を $\Gamma$ の $x_i$ の固定群とし、$L_i$ を $A_i$ の不変式の体とします。次に、$L_1, \ldots, L_n$ は $K$ の有限次数の分離拡大であり、写像 $f \mapsto (f(x_1), \ldots, f(x_n))$ は $L_1 \times \ldots \times L_n$ の $\Theta(X)$ の K-代数同型です。

仮定部分群 $A_i, \ldots, A_n$ までに $\Gamma$ がオープンし、Cor. V、p. 68 の 5 は、$K$ のサブ拡張$L_1, \ldots, L_n$ が $K$ 上の有限次数であることを示しています。明らかにそれらは分離可能です。現在、補題 5 の最後の主張は明らかです。

補題 5 と Th から。 4 (*V*, p. 34f.) すぐに次の結果が得られます。

#### 命題 12 {#alg-v-s10-prop-12 .statement tag=06NK}

— すべての有限 $\Gamma$ 集合 $X$ 代数 $\Theta(X)$ は、次数の $X$ の基数に等しい、$K$ 上のエタールです。さらに、$K$ 上のすべてのエターレ代数は、形 $\Theta(X)$ の代数と同型です。

#### 注意 {#alg-v-s10-n10-rem-1 .statement tag=06NL}

a) $\Theta(X)$ から $K$ へのすべての $K$-代数準同型性 $\varphi$ に対して、すべての $f \in \Theta(X)$ に対して $\varphi(f) = f(x)$ となるような $X$ の一意元 $x$ が存在することを示すのは簡単です。

2) $X$ と $Y$ を 2 つの有限$\Gamma$ 集合とします。 $\mathfrak{T}_\Gamma(X, Y)$ を写像の集合 $X$ の $u$ を $Y$ にすると、すべての $\sigma \in \Gamma$ とすべての $x \in X$ が $u(\sigma x) = \sigma u(x)$ になります。 $u \in \mathfrak{T}_\Gamma(X, Y)$ については、$u^*(f) = f \circ u$ による $K$-代数準同型性 $u^*: \Theta(Y) \to \Theta(X)$ を定義するとします。 For every homomorphism $\Psi$ of $\Theta(Y)$ into $\Theta(X)$ there exists a unique element $u$ of $\mathfrak{T}_\Gamma(X, Y)$ such that $\Psi = u^*$.

### 11. 準ガロア拡張の構造

#### 命題 13 {#alg-v-s10-prop-13 .statement tag=06NM}

— $N$ を $K$ の準ガロア拡張とします。 We denote by $N_r$, the field of invariants of the group of all $K$-automorphisms of $N$ and by $N_s$, the relative separable algebraic closure of $K$ in $N$ ($V$, p. 44). それから：

a) $N_r$ は、$N$ ($V$、p. 25) における$K$ の相対的な$p$-ラジカル閉包です。

b) $N$ は、$K$ のガロア拡大と、$N_s$ 拡大するのすべての $K$ 自己同型が、$N$ の $N_r$ 自己同型に固有の形式で表されます。

c) 体 $N_r$ と $N$ は、$K$ 上で直線的に互いに素となり、$N = K[N, \cup N_s]$ になります。 $N_r \otimes_K N$の他の語、標準準同型、$N$には同型です。

$\Omega$ をサブ内線 ($V$、p. 23、Th. 2) として $K$ 含む $N$ の代数閉包とします。 $N$ は準ガロアであるため、$N$ の $\Omega$ 誘導する自己同型のすべての $K$ 自己同型。したがって、$N_r$ のすべての元は、$\Omega$ の$K$ 自己同型の群の下で不変であり、したがって、$K$ 上で $p$-基数になります ($V$, p. 53, Cor. 3)。逆に、$K$ に対する $p$ 基数である $N$ のすべての元は、$N$ のすべての $K$ 自己同型のもとで明らかに不変であり、したがって属するから $N_r$ までです。これは a) を証明します。

$\Omega$ 写像 $N$ のすべての $K$ 自己同型は $N$ に変換され、したがって $N_r$ は $N_r$ に変換されます。したがって、$N_r$ は $K$ ($V$, p. 54、提案 3)。したがって、$N_s$ は $K$ のガロア拡大になります。 $N_r \cap N$ のすべての元は可分代数的であり、$K$ 上の $p$ 根号であるため、属するから $K$ ($V$、p. Cor. 3)。したがって、$K_r \cap K_s = K$ となります。さて、$N$ は、$N_r$ ($V$, p. 44, Prop. 13) 上では $p$-根数であり、$N_r$ ($V$, p. 56, Th. 1) 上では可分代数であるため、両方$p$-部首で、$K(N_r \cup N_s)$ を超えると分離可能。したがって、Th から続く $N = K(N_r \cup N_s)$ ($V$, p. 39, Cor. 3) と主張 b), c) が得られます。 5 ($V$、p. 71)。

#### 系 {#alg-v-s10-n11-cor-1 .statement tag=06NN}

— Let $p$ the characteristic exponent of $K$, $\overline{K}$ an algebraic closure of $K$, $K_s$, the relative separable closure of $K$ in $\overline{K}$ and $K^{p^{-\infty}}$ the perfect closure of $K$. すると、$K^{p^\infty} \otimes K_s$の$\overline{K}$への標準準同型は同型になります。

#### 注意 {#alg-v-s10-n11-rem-1 .statement tag=06NO}

$R$ (それぞれ $S$) を $K$ の $p$ 基 (それぞれ可分代数) 拡大とします。次に、代数 $R \otimes_K S$ は体です。 : $R$ (それぞれ $S$) は $K^{p^\infty}$ (それぞれ $K_s$) の部分拡張と同型であり、上記の Cor を適用するだけで十分です。 $V$、p. 17の提案1。

### 練習問題 {#alg-v-s10-exercises}

[§ 10 に対して練習問題](exercises/s10/)を参照してください。
