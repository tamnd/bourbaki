---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 4
section_title: Integration of positive point measures
lang: ja
source: int-i-vi
book_pages: INT V.31-INT V.38, INT V.99
pdf_pages: 0286-0293, 0354-0354
extraction: ocr
subsections:
    - "no": 1
      title: Families of point measures
      page: 31
      pdf_page: 286
    - "no": 2
      title: Upper integrals of positive functions with respect to an integral of point measures
      page: 33
      pdf_page: 288
    - "no": 3
      title: Measurability with respect to an integral of point measures
      page: 35
      pdf_page: 290
    - "no": 4
      title: Integration of functions with values in a Banach space, with respect to an integral of point measures
      page: 37
      pdf_page: 292
statements: 10
exercises: 2
content_sha256: 9d395e84ef04fb065115feeacc80352d98c8b5e93aafe6290d8069f8b105a9ab
translated_from: content/en/int/V/04_s4_integration_of_positive_point_measures.md
translation_method: google
source_content_sha256: dd55e7fee706c3d9d06f24460ca7220536b2e52fe66b64ab093af515c9c25f41
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: b7a3d164ae66093ebbb64dec26be3066745a2bdc118f8cfd911bb0eba47bdfc8
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 4。積極的な点対策の統合

### 1. 点措置の家族

X と T を、T の 2 つの局所的にコンパクトな空間、$\pi$ 写像を X に、そして $g$ を T 上で定義された有限数値写像 $\geqslant 0$ とします。これら 2 つの写像定義する写像 $t \mapsto \lambda_t = g(t)\varepsilon_{\pi(t)}$ を X の小節の空間 $\mathscr{M}(X)$ に組み込むと、$t \in T$ ごとに $\lambda_t$ が点小節のいずれかになります (Ch. III, §2, No. 4) $f$ が X で定義された数値写像 $\geqslant 0$ の場合、$\int^* f(x) d\lambda_t(x) = \int^\bullet f(x) d\lambda_t(x) = f(\pi(t))g(t)$ ($g(t) = 0$ と $f(\pi(t)) = +\infty$ のときにこの積を 0 とみなす慣例を思い出してください)。 X で定義されたすべての写像 (トポロジカル空間では値) は、すべての $t \in T$ に対して $\lambda_t$ で測定可能です。 Banach 空間 F への X のすべての写像 $f$ は、すべての $t \in T$ および $\int f(x) d\lambda_t(x) = f(\pi(t))g(t)$ に対して $\lambda_t$ 積分可能です。最後に、$f$ が X で定義された任意の数値写像である場合、$f$ が $\lambda_t$ 可積分であるためには、$f(\pi(t))g(t)$ が有限であることが必要かつ十分であり、その場合は $\int f(x) d\lambda_t(x) = f(\pi(t))g(t)$ になります。

#### 定義 1 {#int-v-s4-def-1 .statement tag=0921}

$\mu$ を T の正の尺度とします。以下の条件が満たされる場合、対 $(\pi, g)$ は $\mu$ に適応されると言われます。
1° 写像 $\pi$ と $g$ は $\mu$ で測定可能です。
2° 写像 $f \in \mathscr{K}(X)$ ごとに、写像 $t \mapsto f(\pi(t))g(t)$ は本質的に $\mu$ 積分可能です。

#### 命題 1 {#int-v-s4-prop-1 .statement tag=0922}

対 $(\pi, g)$ が $\mu$ 適応されている場合、T の $\mathscr{M}_+(X)$ への写像 $\Lambda : t \mapsto \lambda_t = g(t)\varepsilon_{\pi(t)}$ はスカラー的に本質的に $\mu$ 積分可能であり、漠然と $\mu$ 測定可能であり、$\mu$ 適切である。逆に、$\Lambda$ がスカラー的に本質的に $\mu$ 積分可能で漠然と $\mu$ 可測である場合、写像 $g$ は $\mu$ 可測であり、$\pi$ ～ 集合の制限 $g(t) \neq 0$ が $\mu$ 可測となるような $t \in T$ の $S$。

対 $(\pi, g)$ が $\mu$ 適応されていると仮定します。すべての写像 $f \in \mathscr{K}(X)$、写像 $t \mapsto \langle f, \lambda_t \rangle = f(\pi(t))g(t)$ は、本質的に $\mu$ 積分可能です。 $t \mapsto \lambda_t$ が漠然と $\mu$ で測定可能であることを示しましょう。 というのは、まず、$\pi$ と $g$ が連続である場合、写像 $t \mapsto \lambda_t$ は漠然と連続であることに注意します。 一般的な場合、$\pi$ と $g$ ～ $K$ の制約が連続するような$T$ のコンパクトなサブセット$K$ の集合は、$\mu$ 密です (Ch. IV, §5, No. 10、提案 15); $K$ がそのような集合である場合、$t \mapsto \lambda_t$ から $K$ までの制限は漠然と連続しており、よっては主張の最初の主張です。 §3, No. 1 の提案 2 は、$\Lambda$ が $\mu$ で十分であることを示しています。

逆に、$\Lambda$ はスカラー的に本質的に $\mu$ 積分可能であり、漠然と $\mu$ 可測であると仮定します。その場合、それは $\mu$ で十分です (§3, No. 1、提案 2)。 写像 1 は $X$ で下位半連続であるため、写像 $t \mapsto \lambda_t(1) = g(t)$ は $\mu$ 測定可能です (§3、定義 1)。 したがって、集合 $S$ は測定可能です (Ch. IV, §5, No. 5、提案 7)。 $g|K$ が連続し、$\Lambda|K$ が曖昧に連続するようなコンパクトな集合 $K \subset S$ の集合 $\mathfrak{K}$ は、$S$ では $\mu$ 密です (Ch. IV, §5, No. 10、提案 15); $K \in \mathfrak{K}$ の場合、写像 $t \mapsto \varepsilon_{\pi(t)} = \frac{1}{g(t)} \lambda_t$ の制限から $K$ は漠然と連続しており、これは $\pi|K$ の連続性を意味します (Ch. III, §1, No. 9、提案 13)。 $S$では$\mathfrak{K}$が$\mu$-密であるため、$\pi$から$S$の制限は$\mu$-測定可能です。

次の補題を使用します。

#### 補題 {#int-v-s4-n1-lem-1 .statement tag=0923}

*$T$と$X$を2つのトポロジー空間、$\pi$を$T$から$X$への適切な連続写像(GT、I, §10, No. 1、定義1)とする。 $g$ を、$T$ で定義された下位の半連続数値写像とします。すべての $x \in X$ について、$f(x)$ を集合 $\overline{\pi}^{-1}(x)$ における写像 $g(t)$ の下限値とします (下限値は $\overline{\pi}^{-1}(x) = \varnothing$; cf. S、III, §1, No. 9 の場合、$+\infty$ に等しい)。その後、$f$ は$X$ で半連続的に下降します。*

すべての (有限) 実数 $a$ について、$f(x) \leq a$ のような $x \in X$ の集合を $B_a$ で表し、$g(t) \leq a$ のような $t \in T$ の集合を $A_a$ で表します。すべては、$B_a$ が閉じていることを示すことに帰着します (GT、IV, §6, No. 2、提案 1)。 ここで、$A_a$ は閉じられており (同じ参照)、適切な写像 $\pi$ は閉じられています (GT、I, §10, No. 1、提案 1)。したがって、$\pi(A_a) = B_a$ から証明に減ります。 すべての $t \in T$ に対する明らかな関係 $f(\pi(t)) \leq g(t)$ は、$\pi(A_a) \subset B_a$ を意味します。 一方、$x \in B_a$; としましょう。 集合 $\overline{\pi}^{-1}(x)$ は準コンパクト (GT、I, §10, No. 2、Th. 1) および空でないであるため、次のような $t \in \overline{\pi}^{-1}(x)$ が存在します。

$$
g(t) = \inf_{u \in \pi^{-1}(x)} g(u) = f(x) \quad (\text{GT, IV, } § 6, \text{ No. 2, Th. 3}); \text{ thus } t \in A_a \text{ and } \pi(t) = x.
$$

### 2. 点メジャーの積分に対する正の写像の上積分

$(\pi, g)$ が $\mu$ で適応された対である場合、$§ 3$ の適用命題によって得られた結果を、提案 1 によって $\mu$ に適した族 $t \mapsto \lambda_t = g(t)\varepsilon_{\pi(t)},$ に鮮明化できることがわかります。

#### 定理 1 {#int-v-s4-thm-1 .statement tag=0924}

*$(\pi, g)$ *を $\mu$ に適応した対とし、* としましょう
$$
\nu = \int g(t)\varepsilon_{\pi(t)}\, d\mu(t).
$$
*すべての数値写像* $f \geq 0$ *X で定義される* (1)
$$
\int^\bullet f(x)\, d\nu(x) = \int^\bullet f(\pi(t))g(t)\, d\mu(t).
$$

A) まず、メジャー$\mu$ がコンパクトサポート K を持ち、写像 $g$ と $\pi$ の制限から K が連続していると仮定します。 $§ 3$、No. 1、$\nu^\bullet(1) = \int_K g(t)\, d\mu(t) < +\infty,$ の公式 (4) によって、公式 (1) に含まれるすべてのメジャーが制限されます。したがって、最初のメンバーでは $\int^*$ までに置き換える $\int^\bullet$ になる可能性があります。 $§ 3$、No. 2 の公式 (6) を考慮すると、すべては証明 (2) に帰着します。
$$
\int^* f(x)\, d\nu(x) \leq \int^\bullet f(\pi(t))g(t)\, d\mu(t),
$$
ここで、2 番目のメンバーの記号 $\int^\bullet$ は、$\int^*$ に置き換えることができます。上積分の定義により、不等式 (3) を検証すれば十分です。
$$
\int^* f(x)\, d\nu(x) \leq \int^* h(t)\, d\mu(t)
$$
T 上のすべての下部半連続写像 $h$、つまり $\geq$ 写像 $t \mapsto f(\pi(t))g(t)$ です。さて、$\varepsilon$ を数 $> 0$ とし、$u$ を写像 $(h + \varepsilon)/g,$ とします。これは、K の下位半連続です。 $t \in \pi^{-1}(\{x\}) \cap K,$ の場合、$u(t) \geq f(x):$ であれば、$g(t) = 0,$ であるため、$u(t) = +\infty;$ であることは明らかです。 $g(t) > 0,$ それでは
$$
u(t)g(t) = h(t) + \varepsilon \geq f(\pi(t))g(t) = f(x)g(t),
$$

よってが主張した不等式 。これらの条件の下で、すべての $x \in X$ について、$v(x)$ を $t \in \pi^{-1}(\{x\}) \cap K$ の $u(t)$ の下限とします。前述のとおり、写像 $v$ は $\geq f$ であり、$X$ では補題 ($\pi$ から $K$ の制限に適用)、およびすべての $t \in K$ に対して $v(\pi(t))g(t) \leq h(t) + \varepsilon$ が半連続的に低くなります (思い出してください)。慣例により、最初のメンバーは $g(t) = 0$ の場合、零になります)。次に、§3, No. 1の$v$公式の(4)に当てはめてみましょう。以下を取得します。

$$
\int^* f(x)\, d\nu(x) \leq \int^* v(x)\, d\nu(x)
$$
$$
= \int^* v(\pi(t))g(t)\, d\mu(t) \leq \int_K^* (h(t) + \varepsilon)\, d\mu(t)
$$
$$
= \int_K^* h(t)\, d\mu(t) + \varepsilon \mu(1).
$$

メジャー $\mu$ は有界であり、$\varepsilon$ は任意であるため、不等式 (3) が続きます。

B) 次に、一般的なケースに移りましょう。 $T$ の $X \times \mathbf{R}_+$ への写像 $t \mapsto (\pi(t), g(t))$ は $\mu$ 可測であるため (Ch. IV, §5, No. 3, Th. 1)、コンパクト部分集合の $K$ などの $T$ の集合 $\mathscr{K}$ $\pi$ と $g$ ～ $K$ の制限が連続していることは、$\mu$ 密です (Ch. IV, §5, No. 10、提案 15)。 §2, No. 3 の提案 4 によれば、$\mu$ は、$\mathscr{K}$ の元をサポートとするメジャーの加算可能な族 $(\mu_\alpha)_{\alpha \in A}$ の和です。 対 $(\pi, g)$ を $\alpha \in A$ ごとに $\mu_\alpha$ に適応させて、$\nu_\alpha$ をメジャー $\int g(t) \varepsilon_{\pi(t)}\, d\mu_\alpha(t)$ とします。次に、A) により、

$$
\int^* f(x)\, d\nu_\alpha(x) = \int^* f(\pi(t))g(t)\, d\mu_\alpha(t).
$$

しかし、$\nu_\alpha$ 形は、和が $\nu$ に等しい加算可能な族です (§3, No. 1、提案 1 の補正)。したがって、§2, No. 2の提案1により、

$$
\int^* f(x)\, d\nu(x) = \sum_{\alpha \in A} \int^* f(x)\, d\nu_\alpha(x).
$$

(5) の 2 番目の要素には類似の関係があり、したがって、(1) は $\alpha$ を合計することで (5) から得られます。

#### 系 {#int-v-s4-n2-cor-1 .statement tag=0925}

— *Xの部分集合Nが$\nu$に対して局所的に無視できるという位数において、$\pi^{-1}(N)$の共通部分と点の$t \in T$の集合が必要かつ十分であり、ここで$g(t) > 0$は局所的に無視できる$\mu$.*

#### 命題 2 {#int-v-s4-prop-2 .statement tag=0926}

— *$\pi$を、TのXへの適切な連続写像(GT、I, §10, No. 1)とし、gを、すべての$t \in T$に対して$g(t) > 0$となるようなT上の連続有限数値写像とする。 対 $(\pi, g)$ は $\mu$ に適応され、1 つが集合* の場合
$$
\nu = \int g(t) \varepsilon_{\pi(t)}\, d\mu(t),
$$

次に、$X$ で定義されたすべての数値写像 $f \geq 0$ について、

$$
\int^* f(x)\, d\nu(x) = \int^* f(\pi(t))g(t)\, d\mu(t).
$$

$\pi$ と $g$ が $\mu$ 可測であることは明らかです。さらに、$\pi$ が適切であるため、写像 $\psi \in \mathscr{K}(X)$ ごとに、$\psi \circ \pi$ はコンパクトなサポートで連続します。従って、対 $(\pi, g)$ は $\mu$ に適応されており、さらに、写像 $t \mapsto g(t)\varepsilon_{\pi(t)}$ は漠然と連続しています。

$h$ を、次のような $T$ の下位半連続写像とします。

$$
f(\pi(t))g(t) \leq h(t) \quad \text{for all } t \in T.
$$

それを示していきます

$$
\int^* f(x)\, d\nu(x) \leq \int^* h(t)\, d\mu(t).
$$

上積分の定義により、これは不等式を意味します。

$$
\int^* f(x)\, d\nu(x) \leq \int^* f(\pi(t))g(t)\, d\mu(t),
$$

これを§3, No. 2の不等式 (7)と組み合わせると、(7)が証明されます。

(8) を証明するには、次の方法で $X$ 上の定義する写像 $\overline{f}$ を計算しましょう: $\overline{f}(x)$ は集合 $\overline{\pi}^{-1}(x)$ における $h(t)/g(t)$ の下限です (下限は $+\infty$ に等しい) $\overline{\pi}^{-1}(x) = \varnothing$）。 写像 $\overline{f}$ には次の特性があります。

すべての $x \in X$ に対して $1^\circ$ $\overline{f}(x) \geq f(x)$ (すべての $t \in T$ に対して $g(t) > 0$ 以降)。

$2^\circ$ $\overline{f}(\pi(t))g(t) \leq h(t)$ $t \in T$ 全員。

$3^\circ$ 写像 $\overline{f}$ は、補題のおかげで下位半連続であり、写像 $h/g$ は $T$ の下位半連続です。

従って、§3, No. 1 の提案 2a) を考慮すると、次のようになります。

$$
\int^* f(x)\, d\nu(x) \leq \int^* \overline{f}(x)\, d\nu(x) = \int^* \overline{f}(\pi(t))g(t)\, d\mu(t) \leq \int^* h(t)\, d\mu(t),
$$

これにより (8) が成立し、証明が完了します。

### 3. 点メジャーの積分に関する可測性

#### 命題 3 {#int-v-s4-prop-3 .statement tag=0927}

— $(\pi, g)$ を $\mu$ に適応した対とします。

$$
\nu = \int g(t)\varepsilon_{\pi(t)}\, d\mu(t).
$$

$f$ を $X$ の写像としてトポロジカル空間 $G$ とし、$S$ を点 $t \in T$ の ($\mu$ 可測) 集合とします。 $g(t) > 0$。 $f$が$\nu$可測である位数において、$f \circ \pi$から$S$のうち制限が$\mu$可測であることが必要十分である。

まず、$f$ が $\nu$ 可測であると仮定します。 仮説によれば、$\pi$ から $K$ までの制限が連続であるような、$S$ のコンパクトな部分集合 $K$ の集合 $\mathscr{K}$ は、$S$ では $\mu$ 密です。 IV, §5, No. 10、提案 15)。 したがって、$f \circ \pi$ から $S$ までの制限が $\mu$ で測定可能であることを示すには、$f \circ \pi$ から $H$ までの制限が連続であるような、$K$ のコンパクトな部分集合の集合 $H$ が、すべての $K \in \mathscr{K}$ について証明するだけで十分です。 $K$の$\mu$-密集（Ch. IV, §5, No. 8、提案 13)。 しかし仮説によれば、各 $C_n$ に対する $f$ の制限が連続するように、$\nu$ 無視できる集合 $N$ とコンパクト集合のシーケンス $(C_n)$ によって形成されるコンパクト集合 $\pi(K)$ の分割が存在します。 これらの条件、$K \cap \overline{\pi}(N)$、および集合 $K \cap \overline{\pi}(C_n)$ 形分割の $K$ の下。しかし、$K \cap \overline{\pi}(N)$ はコルのおかげで $\mu$ は無視できます。 Thの。 No. 2、集合、$K \cap \overline{\pi}(C_n)$の1はコンパクトで、$f \circ \pi$の制限から後者の集合までは連続しているため、$f \circ \pi$から$S$の制限が$\mu$可測であることがわかります。

逆に、これが当てはまると仮定してください。 $f$ が $\nu$ 可測であることを示すには、$f$ から $L$ の制限が連続であるような、コンパクト部分集合 $L$ の $X$ の集合 $\mathscr{L}$ を証明すれば十分です。 $\nu$-密 (Ch. IV, §5, No. 10、提案 15)。 $N$ を $X$ の部分集合として、$N \cap L$ がすべての $L \in \mathscr{L}$ に対して $\nu$ で無視できるようにし、$N$ が局所的に $\nu$ で無視できることを示します。このためには、$\overline{\pi}(N) \cap S$ が局所的には $\mu$ で無視できることを示さなければなりません (No. 2 の Th. 1 の Cor.)。さて、$\pi$と$f \circ \pi$の制限から$H$が連続するようなコンパクト部分集合$H$の$S$の集合$\mathscr{H}$は仮定までです$S$ では $\mu$ が密集しています (Ch. IV, §5, No. 10、提案 15)。従って、$\overline{\pi}(N) \cap H$ がすべての $H \in \mathscr{H}$ に対して $\mu$ が無視できることを証明すれば十分です。さて、$\pi(H)$ はコンパクトであり、同値関係 $\pi(t) = \pi(t')$ によって $H$ の商空間と識別され、$\pi$ はこの商空間上で $H$ の標準写像と識別される可能性があります。 (GT、I, §5, No. 2、提案 3)。 $f \circ \pi$から$H$の制限は連続であるため、$f$から$\pi(H)$の制限も連続であり、他の語$\pi(H) \in \mathscr{L}$では、$N \cap \pi(H)$は$\nu$-無視できます。コルによって。 Thの。 No. 2、$\overline{\pi}(N \cap \pi(H)) \cap S$ の 1 は、局所的には $\mu$ は無視できます。従って、集合にも同じことが当てはまります

$$
H \cap \overline{\pi}(N) \subset \overline{\pi}(N \cap \pi(H)) \cap S;
$$

しかし、$H$ はコンパクトなので、$H \cap \overline{\pi}(N)$ は $\mu$ を無視でき、証明が完成します。

#### 注意 {#int-v-s4-n3-rem-1 .statement tag=0928}

$f$ が $X$ の写像をバナッハ空間 $F$ にすると、$f \circ \pi$ から $S$ の制限が$\mu$ 測定可能であると言うのも、次のように言うのも同じことになります。 写像 $(f \circ \pi)g$ ($T$ で定義) は、$g$ が $\mu$ 測定可能であり、$S$ では零ではなく、$T - S$ では零であるため、$\mu$ 測定可能です。 (第 IV, §5, No. 10、提案 15)。

### 4. 点メジャーの積分に関して、バナッハ空間における写像と値の積分

#### 定理 2 {#int-v-s4-thm-2 .statement tag=0929}

*$(\pi, g)$ *を $\mu$ に適応した対とし、* としましょう
$$
\nu = \int g(t) \varepsilon_{\pi(t)} \, d\mu(t).
$$
*$f$ *写像を * $X$ に定義し、 *バナッハ空間* $F$ * または * $\overline{\mathbf{R}}$ の値とします。 *$f$ *本質的に $\nu$ 積分可能であるためには、* $t \mapsto f(\pi(t))g(t)$ *本質的に $\mu$ 積分可能であることが必要かつ十分であり、その場合*
$$
\int f(x) \, d\nu(x) = \int f(\pi(t))g(t) \, d\mu(t).
$$
*さらに、* $\pi$ * は連続的で適切であり、* $g$ * は連続的で* $g(t) > 0$ *すべてに* $t \in T$ であると仮定します。 *そして、* $f$ * が $\nu$ 可積分であるためには、* $t \mapsto f(\pi(t))g(t)$ * $\mu$ 可積分であることが必要かつ十分です。

A) まず、メジャー $\mu$ にコンパクトサポート $K$ があり、その上に $g$ が境界付けられている場合を扱います。次に、尺度 $\mu$ と $\nu$ は制限され、「積分可能」によって置き換えるが主張で「本質的に積分可能」になります。 $f$ が $\nu$ 可積分であるとします。 写像 $f(\pi(t))g(t)$ は $\mu$ 可積分であり、関係 (9) が Th によって検証されます。 §3, No. 3 の 1 つ。逆に、$f(\pi(t))g(t)$ が $\mu$ 可積分であると仮定します。 $f$ は $\nu$ 可測です (No. 3、提案 3 および *注意*)、そして
$$
\int^\bullet |f(x)| \, d\nu(x) = \int^\bullet |f(\pi(t))|g(t) \, d\mu(t) < +\infty
$$
(No. 2、木 1);したがって、$f$ は本質的に $\nu$ 積分可能 (§1, No. 3、提案 9)、したがって $\nu$ 積分可能です。 Th. §3, No. 3 の 1 は (9) を意味します。

B) 一般的なケースに移りましょう。 $\mathscr{K}$ を、$g|K$ が連続となるような、$T$ のコンパクトなサブセット $K$ の集合とします。 $\mathscr{K}$ は、$\mu$ 密です (Ch. IV, §5, No. 10、提案 15)、したがって、措置 $\mu$ は、$\mathscr{K}$ の元を支持する措置のファミリー $(\mu_\alpha)_{\alpha \in A}$ の和です (§2, No. 3、提案 4)。 対 $(g, \pi)$ は明らかに $\alpha \in A$ ごとに $\mu_\alpha$ 適応されており、尺度 $\nu$ は尺度 $\nu_\alpha = \int \varepsilon_{\pi(t)}g(t) \, d\mu_\alpha(t)$ の族の和 (§3, No. 1、提案 1 の補正)。 A)の議論は$\mu_\alpha, \nu_\alpha$の対策に適用できるので、§2, No. 2の提案3から主張の最初の部分が導かれます。

写像 $f$ (それぞれ $t \mapsto f(\pi(t))g(t)$) が $\nu$ (それぞれ $\mu$) に対して積分可能であるためには、それが本質的に積分可能であり、

$$
\int^* |f(x)| d\nu(x) < +\infty \quad (\text{resp. } \int^* |f(\pi(t))|g(t)\,d\mu(t) < +\infty ).
$$

したがって、主張の 2 番目の部分は、最初の部分と命題 2 の後に続きます。

#### 注意 {#int-v-s4-n4-rem-1 .statement tag=092A}

— Let $(\pi, g)$ be a $\mu$-adapted pair, $\pi'$ a mapping of T into X, and $g'$ a finite numerical function $\geq 0$ defined on T, such that $\pi'$ (resp. $g'$) is equal to $\pi$ (resp. $g$) locally almost everywhere for $\mu$. 次に、対 $(\pi', g')$ は $\mu$ に適応され、$\lambda_t = g(t)\varepsilon_{\pi(t)}$ と $\lambda'_t = g'(t)\varepsilon_{\pi'(t)}$ はほぼどこでも局所的に等しく、$\int g(t)\varepsilon_{\pi(t)}\,d\mu(t) = \int g'(t)\varepsilon_{\pi'(t)}\,d\mu(t)$ です。 現在、$\pi'$ と $g'$ がほぼどこでも ($\mu$ の場合) ローカルにのみ定義されており、$\pi'$ (それぞれ $g'$) が $\pi$ (それぞれ $g$) に等しいような $\mu$ に適応した対 $(\pi, g)$ が存在するとします。地元ではほぼどこでも、対 $(\pi', g')$ は $\mu$ に適応したものであり、もう 1 つは集合であると言われています。

$$
\int g'(t)\varepsilon_{\pi'(t)}\,d\mu(t) = \int g(t)\varepsilon_{\pi(t)}\,d\mu(t)
$$

(cf. §3, No. 3、*注意*)。 主張 $\pi$ と $g$ がほぼどこでもローカルに定義されているとのみ想定されている場合、提案 1 と 2、および提案 3 は引き続き有効です。

### 練習問題 {#int-v-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
