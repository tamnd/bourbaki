---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 12
section_title: Finite fields
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.166-A V.170
pdf_pages: 0207-0212, 0280-0284
extraction: ocr
subsections:
    - "no": 1
      title: The structure of finite fields
      page: 0
      pdf_page: 207
    - "no": 2
      title: Algebraic extensions of a finite field
      page: 94
      pdf_page: 208
    - "no": 3
      title: The Galois group of the algebraic closure of a finite field
      page: 96
      pdf_page: 210
    - "no": 4
      title: Cyclotomic polynomials over a finite field
      page: 97
      pdf_page: 211
statements: 11
exercises: 14
content_sha256: 62bbd33f3909de2279aae0a7b5d7f041c9f612631ec047e92d95a2b3460752f5
translated_from: content/en/alg/V/12_s12_finite_fields.md
translation_method: google
source_content_sha256: bd8e10c4a05eb5e291baa4ec9c998a38d9874d55fab72a3f4d3987c8ee8ea686
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: cff142a97956f41b321de8b36628fb930b81bb5be029495fceea8544cf37a03c
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 12。 有限体

### 1. 構造/有限体

#### 命題 1 {#alg-v-s12-prop-1 .statement tag=06Q8}

— K を有限体とし、q 元とします。

a) K の標数は素数数 p であり、q = p^f となる整数 f \geq 1 が存在します。

b) K の加法群は f の直和であり、位数の群

c) K の乗法群は、位数 q - 1 の環状です。

Z は無限で K は有限であるため、一意の環準同型 \varphi : Z \to K は単射的ではなく、その核は 0 に等しくない Z の素イデアルです。 したがって、K の特性は素数数であり、K は p の体 \mathbf{F}_p に対して代数です。 元 (V、p. 2)。 f を \mathbf{F}_p 上の K の次数とします。 f が無限の場合、K は \mathbf{F}_p、よって q \geq p^n 上の次元 n の各整数 n \geq 0 部分空間に対して含むになりますが、これは不合理です。したがって、f は有限です。したがって、K の加法群は (\mathbf{F}_p)^f、よって主張 a) および b) と同型です。

主張 c) の後に、補題 1 (V、p. 78) が続きます。

#### 命題 2 {#alg-v-s12-prop-2 .statement tag=06Q9}

— K を q 元の有限体とします。 体 K は、\mathbf{F}_p[X] の多項式 X^q - X の分解体であり、この多項式のすべての根の集合です。

1 この章の規則に従って、ここでは有限の可換体についてのみ考慮します。実際、章 VIII (cf. V、p. 170、練習問題 14) でわかるように、すべての有限体は可換です。

$K$ のすべての $x \neq 0$ に対して、$K^*$ は位数 $q-1$ (I, p. 52) の有限群であるため、$x^{q-1} = 1$ になります。したがって、$K$ のそれぞれの $x$ に対して $x^q = x$ となります。 $\mathbf{F}_p[X]$ の多項式 $X^q - X$ は次数 $q$ であり、$K$、よってには $q$ 根が含まれます

$$
X^q - X = \prod_{\xi \in K} (X - \xi).
$$

命題ここから一気に2つ続きます。

#### 系 {#alg-v-s12-n1-cor-1 .statement tag=06QA}

— *同じ基数の 2 つの有限体は同型です。*

$K'$ を $q$ 元の有限体とします。その特徴は、素数数 $p'$ を $q = p^f$、よって $p' = p$ で割ることです。したがって、$K'$ は、$\mathbf{F}_p[X]$ の多項式$X^q - X$ の分解体であり、したがって、$K$ と $K'$ は同型です (V, p. 22, Cor.)。

$K = \mathbf{F}_p$、公式のとき (1) 簡約する ～ 関係

$$
X^p - X \equiv \prod_{i=0}^{p-1} (X - i) \mod p \mathbf{Z}[X]
$$

多項式環 $\mathbf{Z}[X]$に。

公式 (2) と書かれることもあります

$$
X^{p-1} - 1 \equiv \prod_{i=1}^{p-1} (X - i) \mod p \mathbf{Z}[X]
$$

特に $X = 0$ については (« Wilson's 公式 ») を取得します。

$$
(p-1)! \equiv -1 \mod p
$$

### 2. 代数拡大/有限体

#### 命題 3 {#alg-v-s12-prop-3 .statement tag=06QB}

— *$K$ を、$q$ 元の有限体、$K$ の $\Omega$ 代数閉拡大、および $m$ 整数 $\geqslant 1$ とします。
a) $K$ 上の次数 $m$ である $\Omega$ の一意のサブ内線$K_m$ が存在します。
b) 体 $K_m$ には $q^m$ 元があり、自己同型 $x \mapsto x^{q^m}$ の $\Omega$ の固定点の集合です。
c) 循環群 $K_m^*$ の各生成元 $\zeta$ に対して $K_m = K(\zeta)$ があります。
$p$ を $\mathbf{F}_p$ に対する $K$ の $K$ と $f$ 次数の特徴とします。 $q^m = p^{fm}$ と写像 $x \mapsto x^{q^m}$ は、完全体 $\Omega$ の自己同型です (V、p. 7、提案 4)。 したがって、$K[X]$ の多項式 $X^{q^m} - X$ の根の集合 $K_m$ は、$\Omega$ の部分体です。 $X^{q^m} - X$ の導関数は $-1$ に等しいため、この多項式のすべての根は単純 (IV、p. 17、提案 7) であるため、$K_m$ は $q^m$ 元になります。 したがって、$[K_m : K] = m$ となります。

ここで、L を、$K$ に対する次数 $m$ の $\Omega$ の部分拡張とします。 $K$ に対するベクトル空間として、$L$ は $K^m$ と同型であり、$q^m$ 元も同様です。したがって、すべての $x \in L$ (提案 2)、よって $L \subset K_m$ に対して $x^{q^m} = x$ が得られます。 $[L : K] = [K_m : K] = m$から、ついに$L = K_m$になりました。

したがって、主張 a) と b)、および c) が自明であることを証明しました。

#### 系 {#alg-v-s12-n2-cor-1 .statement tag=06QC}

— *$K$ を $K$ の有限体と $\Omega$ 代数閉拡大とします。 $\Omega$ の $K$ の相対代数閉包 $\overline{K}$ は、() と単位元の根で構成され、$K$ の代数閉包です*。

$K$ は $K$ (V、p. 22、例 2) の代数閉包であることがわかっており、$\Omega$ 属するから $K$ の単位元のすべての根であることは明らかです。さらに、$K$ に対する次数 $m$ の $\overline{K}$ に $x \neq 0$ が与えられた場合、$K$ が $q$ 元である場合、体 $K(x)$ は $q^m$、よってになります。 $x^{q^m - 1} = 1$ なので、$x$ は $\Omega$ の単位元の根です。

$p$ を素数数とし、$\mathbf{F}_p = \mathbf{Z}/p\mathbf{Z}$ を $p$ 元の体とします。私たちは $\mathbf{F}_p$ の選ぶ代数閉包 $\Omega$ であり、その存在はシュタイニッツの定理 (V、p. 23、Th. 2) に続きます。 $f$を正の整数と$q = p^f$とします。提案 3 により、$\mathbf{F}_p$ を超える次数 $f$ である $\Omega$ の固有の部分体が存在します。 $\mathbf{F}_q(\Omega)$ または記法 $\mathbf{F}_q$ を乱用してそれを表します。これは、$\mathbf{F}_p$ の上に次数 $f$ を持つ、$\Omega$ の一意のサブエクステンションです。 It is the unique 部分体 of $\Omega$ of 基数 $q$, and every 体 of 基数 $q$ is isomorphic (not canonically) to $\mathbf{F}_q$ (Cor. of Prop. 2). $\mathbf{F}_q$ は、$x^q = x$ である $\Omega$ の $x$ と、$q'$ が $q$ の冪である場合に限り、$F, \subset \mathbf{F}_{q'}$ で構成されていることに注意してください。

#### 命題 4 {#alg-v-s12-prop-4 .statement tag=06QD}

— *$\mathbf{K}$ を $q$ 元の有限体および有限次数 $m$ の $K$ の $\mathbf{K}_m$ 拡大とします。

a) 体 $\mathbf{K}_m$ は $K$ のガロア拡大であり、そのガロア群は自己同型 $\sigma_q : x \mapsto x^q$ によって生成された位数 $m$ の循環群です。

b) $K$ に関する$x$ の各$x \in \mathbf{K}_m$ ノルムは$x^{(q^m - 1)/(q - 1)}$ に等しい。

c) $K$ のすべての元は、$\mathbf{K}_m$ の元のトレース (それぞれノルム) です。*

$\Gamma$ を、$\sigma_q$ によって生成された $\mathbf{K}_m$ の自己同型の循環群とします。 $\Gamma$ の不変量の体は、$\mathbf{K}_m$ の元 $x$ で構成され、$x^q = x$ は$K$ に等しくなります。したがって、$\mathbf{K}_m$ はガロア群 $\Gamma$ を伴う $K$ のガロア拡大であり、この後者は位数が $[K_m : K] = m$ (V, p. 66, Th. 3) に等しい。したがって、a) が続きます。

$\Gamma = \{1, \sigma_q, \sigma_q^2, \ldots, \sigma_q^{m-1}\}$ があります。したがって、$K$ に対する $\mathbf{K}_m$ の要素 $x$ のノルムは $N(x) = \prod_{i=0}^{m-1} \sigma_q^i(x) = x^{1 + q + \cdots + q^{m-1}}$ となり、$1 + q + \cdots + q^{m-1} = \frac{q^m - 1}{q - 1}$ が得られます。 これは b) を証明します。 $\xi$ を循環群 $\mathbf{K}_m^*$ の生成元とします。 ノルム $N : \mathbf{K}_m^* \to K^*$ の像は、元 $\xi = N(\xi) = \xi^{(q^m - 1)/(q - 1)}$ によって生成された $K^*$ の循環部分群です。 $\xi$ は位数 $q^m - 1$ のものであり、$\xi$ は位数 $q - 1$ のものであるため、生成する $K^*$ となります。 これは、 K のすべての非ゼロ元は、 K の非ゼロ元のノルムであることを証明します。さらに、$0 = N(0)$もあります。

最後に、$K_m$ は K の分離可能な代数拡大であるため、トレースは K (V, p. 49, Cor.) 上のベクトル空間 $K_m$ 上で非ゼロ線型形式になります。したがって、K のすべての元は、$K_m$ の元のトレースです。

### 3. ガロア群/代数閉包/有限体

$S \neq \{1\}$ を乗法で安定した整数 $\geq 1$ の集合とします。 位数関係 « m 割る n » までに完了します。 m 割る n のとき、$m\mathbf{Z} \supset n\mathbf{Z}$ があるため、環 $\mathbf{Z}/m\mathbf{Z}$ には環 $\mathbf{Z}/n\mathbf{Z}$ の標準準同型 $\pi_{m,n}$ が存在します。 S でインデックス付けされた環 $(\mathbf{Z}/m\mathbf{Z}, \pi_{m,n})$ の逆数系の逆数極限を $A(S)$ で表します。各有限集合 $\mathbf{Z}/m\mathbf{Z}$ には、位相を備えた離散位相と $A(S)$ が装備されています。 積 $\prod_{n \in S} (\mathbf{Z}/n\mathbf{Z})$ によって誘発されました。

この場合、$A(S)$ はコンパクトなトポロジー 環 (Gen. Top. I, p. 64、Prop. 8) です。 $\mathbf{Z}$ から $A(S)$ への一意の環準同型 $\varphi$ が、密な像を伴う単射であることがすぐにわかります。 *$A(S)$* の $\varphi$ の下にある像を同一視する $\mathbf{Z}$ とします。 $A(S)$ の$\mathbf{Z}$ によって誘発された位相の場合、*集合 $m\mathbf{Z}$ ($m \in S$ の場合) 0* の近傍の形基底。

$S = \mathbf{N}^*$の場合、$A(S)$は$\hat{\mathbf{Z}}$と書き込まれます。 S が素数数 $l$ の冪で構成されるとき、$A(S)$ は $\mathbf{Z}_l$ と書かれ、« I 進数整数の環 » と呼ばれます。したがって、私たちは

$$
\hat{\mathbf{Z}} = \lim_{\leftarrow m \geq 1} \mathbf{Z}/m\mathbf{Z} , \quad \mathbf{Z}_l = \lim_{\leftarrow n \geq 0} \mathbf{Z}/l^n\mathbf{Z} .
$$

S と T が $S \supset T$ のように乗法の下で安定した 2 つの整数の集合である場合、トポロジカル環の連続準同型である自然な射影 $A(S) \to A(T)$ が得られます。特に、すべての素数数 $l$ に対して、連続する準同型 $\mathbf{Z} \to \mathbf{Z}_l$ が存在します。そこから連続的な準同型が得られます。

$$
\hat{\mathbf{Z}} \to \prod_l \mathbf{Z}_l
$$

(積をすべての素数数に拡張) ;これは、I、p. 112、提案 11 の逆極限への移行から続くように、トポロジー 環* の *同型です。

K を q 元の有限体および K の K 代数閉包とします。すべての整数 $m \geq 1$ について、K 上の次数 m である K の一意の部分体を $K_m$ で表します (提案 3)。 $\overline{K} = \bigcup_{m \geq 1} K_m$ があります。さらに、完全体 $\overline{K}$ の $\sigma_q$ 自己同型 $x \mapsto x^q$ で表します。それは K の *Frobenius 自己同型* (K を基準にして) と呼ばれます。

#### 命題 5 {#alg-v-s12-prop-5 .statement tag=06QE}

— $\pi_K(1) = \sigma_q$ のような位相的群 $\pi_K : \mathbf{Z} \to \mathrm{Gal}(\bar{K}/K)$ の一意の同型が存在します。

$\Gamma$ を $\sigma_q$ によって生成された $\mathrm{Gal}(\bar{K}/K)$ の部分群とします。 整数 $m > 0$ ごとに、すべての $x \in \bar{K}$ に対して $\sigma_q^m(x) = x^{q^m}$ が得られるため、$\sigma_q^m$ の固定点の集合は $K$ に等しくなります。 $K \neq \bar{K}$ なので、$\sigma_q^m \neq 1$ になります。 したがって、1 を $\sigma_q$ にマッピングする $\mathbf{Z}$ の $\Gamma$ への同型性 $\pi_0$ が存在します。

$\Gamma$ の不変量の体は、$x^q = x$ となるような $x \in K$ で構成されているため、$K$ に等しくなります。したがって (V, p. 67, 補題 2) 群 $\Gamma$ は $\mathrm{Gal}(\bar{K}/K)$ に密です。 $K$ の有限次数の $\bar{K}$ のすべての部分拡張は体 $K_m$ の 1 つであるため、部分群 $\mathrm{Gal}(\bar{K}/K_m)$ 形は $\mathrm{Gal}(\bar{K}/K)$ の 1 の近傍の基本的な系です。 $\Gamma \cap \mathrm{Gal}(\bar{K}/K_m)$ は $\sigma_q^m$ によって生成された循環群であるため、$\pi_0(m\mathbf{Z})$ に等しいことは明らかです。

上記の注意から、$\mathbf{Z}$ 同型 $\pi_0 : \mathbf{Z} \to \Gamma$ 拡大するの位相について、トポロジカル群 $\pi_K : \mathbf{Z} \to \mathrm{Gal}(\bar{K}/K)$ の同型までを独自の方法で示します。

$m \geq 1$ を整数とします。 $K$に対する$\bar{K}$のフロベニウス自己同型が$\sigma_q^m$であることは明らかです。したがって、関係が得られます。

$$
\pi_{K_m}(a) = \pi_K(ma) \quad \text{for } a \in \mathbf{Z}.
$$

### 4. 有限体上の円分多項式

$K$ を $q$ 元の有限体、$n \geq 1$ 整数が $K$ と $R_n$ の特性 $p$ で割り切れない、レベル $n$ の円分法拡大とします。 $K$ (V、p. 81)。 $R_n$の単位元の$n$番目の根の群$\mu_n(R_n) = \mu_n$は、位数$n$の循環であり、$R_n = K(\mu_n)$が存在し、単射準同型が存在することがわかっています。

$$
\varphi_n : \mathrm{Gal}(R_n/K) \to (\mathbf{Z}/n\mathbf{Z})^*
$$

$\sigma \in \mathrm{Gal}(R_n/K)$、$\zeta \in \mu_n$、$j \in \varphi_n(\sigma)$ に対して $\sigma(\zeta) = \zeta^j$ というように。

さらに、$f$ が $K$ 上の $R_n$ の次数である場合、$K$ 上の $R_n$ のガロア群は、自己同型 $\sigma_q : x \mapsto x^q$ によって生成される、位数 $f$ の循環です。 (V、p. 95、提案 4)。すぐに次のことができます。

#### 命題 6 {#alg-v-s12-prop-6 .statement tag=06QF}

— フロベニウスの $\varphi_n$ の下の像自己同型 $\sigma_q$ は、$q \mod n$ の剰余類です。

したがって、V、p. 84 の提案 6 を考慮すると、次のようになります。

#### 系 {#alg-v-s12-n4-cor-1 .statement tag=06QG}

— $K$ 上の $R_n$ の次数は、$q^f \equiv 1 \pmod{n}$ となるような最小の整数 $f \geq 1$ です。円分多項式 $\Phi_n$ が $K$ に対して既約であるためには、$q$ $n$ を法とする剰余類によって群 $(\mathbf{Z}/n\mathbf{Z})^*$ が生成されることが必要かつ十分です。

#### 例 1 {#alg-v-s12-n4-exa-1 .statement tag=06QH}

多項式 $\Phi_3(X) = X^2 + X + 1$ は、$q \equiv 2 \pmod{3}$ の場合に限り、$F_q[X]$ で既約です。同様に、$\Phi_4(X) = X^2 + 1$ は、$q \equiv 3 \pmod{4}$ の場合に限り、$F_q[X]$ で既約であり、$\Phi_5 = X^4 + X^3 + X^2 + X + 1$ では、既約性条件は $q \equiv 2,\ 3 \pmod{5}$ となります。

#### 例 2 {#alg-v-s12-n4-exa-2 .statement tag=06QI}

$5^2 \equiv 1 \pmod{12}$ があるため、5 の剰余類 (mod 12) は生成する $(\mathbf{Z}/12\mathbf{Z})^*$ にはなりません。したがって、多項式 $\Phi_{12}(X) = X^4 - X^2 + 1$ は $F_5[X]$ で既約ではありません。実際、私たちは持っています
$$
\Phi_5(X) = (X^2 + 2X - 1)(X^2 - 2X - 1)
$$
$F_5[X]$に。

### 練習問題 {#alg-v-s12-exercises}

[§ 12 に対して練習問題](exercises/s12/)を参照してください。
