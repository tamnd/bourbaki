---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 7
section_title: Integration with respect to an induced measure
lang: ja
source: int-i-vi
book_pages: INT V.74-INT V.78, INT V.112-INT V.114
pdf_pages: 0329-0333, 0367-0369
extraction: ocr
subsections:
    - "no": 1
      title: Integration with respect to an induced measure
      page: 74
      pdf_page: 329
    - "no": 2
      title: Properties of induced measures
      page: 77
      pdf_page: 332
statements: 20
exercises: 11
content_sha256: 99f1e6e8f427e2009f61df912a1d3184c5f6d1a8050f11240238734452d99035
translated_from: content/en/int/V/07_s7_integration_with_respect_to_an_induced.md
translation_method: google
source_content_sha256: 0f5f27152d636e2b4a3f4de2fe99a74694ba33c12058af8b625950449ac3a190
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 1492b9edb95c8dcbda2dc9685d90604a83f6274ccf6a77b07b0a7ff84065b68a
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 7。誘導措置に関する統合

### 1. 誘導措置に関する統合

$X$ を $T$ の局所圧縮部分空間とし、$\mu$ を $T$ のポジティブ測度、$\mu_X$ を $\mu$ によって $X$ に誘導された測度とする (Ch. IV, §5, No. 7)。 $t \in T$ ごとに、$X$ に対して * $\lambda_t$ を定義するメジャーにします。$t \in X$ の場合は $\lambda_t = \varepsilon_t$、$t \in \mathbf{C}X$ の場合は $\lambda_t = 0$ です。 $X$ で定義されたすべての有限数値写像 $g$ に対して、$t \in X$ の場合は $\int g(x) d\lambda_t(x) = g(t)$、$t \in \mathbf{C}X$ の場合は $\int g(x) d\lambda_t(x) = 0$ になります。 $g$ が $\mathscr{K}(X)$ の写像である場合、したがって、$\mu_X$ の定義までに、

$$
\mu_X(g) = \int \langle g, \lambda_t \rangle d\mu(t) .
$$

これは、次のように書くことができることを意味します

$$
\mu_X = \int \lambda_t d\mu(t)
$$

(§3, No. 1)。

ここで、T の定義する写像 $\pi$ を、設定 $\pi(t) = t$ で $t \in X$、$\pi(t) = t_0$ を $t \in \mathbf{C}X$ として、$t_0$ を任意の点として、X にします。 X; $t \in T$ごとに$\lambda_t = \varphi_X(t)\varepsilon_{\pi(t)}$と書くことができます。 写像 $\pi$ は、制限から X および $\mathbf{C}X$ であるため、$\mu$ 可測です (Ch. IV, §5, No. 10、提案 16)。 対 $(\pi, \varphi_X)$ が $\mu$ に適応されたもの (§4, No. 1) であることがすぐにわかります。したがって、次のような結果が得られます。

#### 命題 1 {#int-v-s7-prop-1 .statement tag=0963}

— *すべての数値写像* $g \geqslant 0$ *上に定義* X、

$$
\int^\bullet g\,d\mu_X = \int_X g\,d\mu
$$

(cf. §5, No. 3、*例*、記法 $\int_X^\bullet$ の場合)。

前述の注意と (2) を考慮すると、Th から関係 (3) が得られます。 §4 の 1。

#### 系 1 {#int-v-s7-prop-1-cor-1 .statement tag=0964}

— *X、$\mu_X^\bullet(B) = \mu^\bullet(B)$ の * 部分集合* B *ごとに; *B が *局所的* $\mu_X$*-無視できるものであるためには、* B が *局所的* $\mu$*-無視できるものであることが必要かつ十分です。

#### 系 2 {#int-v-s7-prop-1-cor-2 .statement tag=0965}

— *M を * T の部分集合とします。 *もし * $\mu$ *が M に集中している場合、*そのとき* $\mu_X$ *は $M \cap X$ に集中しています。

#### 系 3 {#int-v-s7-prop-1-cor-3 .statement tag=0966}

— *尺度* $\mu_X$ *が零になるためには、* X *局所的* $\mu$ *無視できる* ことが必要かつ十分です。

#### 注意 {#int-v-s7-n1-rem-1 .statement tag=0967}

— S が $\mu$ のサポートである場合、$S \cap X$ (これは X で閉じられます) 含むは Cor による $\mu_X$ のサポートです。 2 ですが、それとは異なる場合があります。たとえば、$\mu$ が拡散測度であり、X が部分空間から点に削減される場合、誘導測度 $\mu_X$ は零であるため、そのサポートは空です。ただし、注意、XがTでオープンであれば、$\mu_X$のサポートは$S \cap X$に等しい。

#### 命題 2 {#int-v-s7-prop-2 .statement tag=0968}

— *g *の* X *を位相空間に* $\mu_X$*-測定可能にする写像*のためには、* g *が* $\mu$* で* X *(§5, No. 3, *例*)*で*測定可能であることが必要かつ十分である。

これは、§4 の提案 3 から導かれます。

#### 系 {#int-v-s7-n1-cor-1 .statement tag=0969}

— *部分集合* B *of* X *が $\mu_X$*-測定可能であるためには、* B *が* $\mu$*-測定可能*であることが必要かつ十分である。

#### 定理 1 {#int-v-s7-thm-1 .statement tag=096A}

— *g を * X に * 写像を定義し、* $\overline{\mathbf{R}}$ * または Banach 空間に値を * 定義させます。 * g が *本質的に* $\mu_X$* 積分可能であるためには、 $g$ が $X$ (§ 5, No. 3, 例) で本質的に $\mu$ 積分可能であることが必要* で十分です。その場合、

$$
\int g \, d\mu_X = \int_X g \, d\mu.
$$

これはThから続きます。 § 4の2。

#### 系 1 {#int-v-s7-thm-1-cor-1 .statement tag=096B}

*X の部分集合 B が本質的に $\mu_X$ 積分可能であるためには、それが本質的に $\mu$ 積分可能であることが必要かつ十分であり、その場合は $\mu_X(B) = \mu(B)$ です。

#### 系 2 {#int-v-s7-thm-1-cor-2 .statement tag=096C}

*g を T 上で定義され、局所的に $\mu$ 可積分可能な複素数写像とする。 g の制限 $g_X$ から X はローカルで $\mu_X$ 積分可能であり、*

$$
(g \cdot \mu)_X = g_X \cdot \mu_X.
$$

これは Th からすぐに続きます。 1、写像 $fg_X$ ($f \in \mathscr{K}(X; \mathbf{C})$) およびX に複合測定によって引き起こされた測定の定義に適用されます (Ch. IV, § 5, No. 7)。

#### 系 3 {#int-v-s7-thm-1-cor-3 .statement tag=096D}

*$\theta$ を T の複素測度とする。それから*

$$
|\theta|_X = |\theta_X|.
$$

集合 $|\theta| = \mu$ を適用し、Cor. 2 $g$ を絶対値値 1 の複素数写像として、$\theta = g \cdot \mu$ となる (§ 5, No. 5、Th. 2 の Cor. 3)。それから$\theta_X = g_X \cdot \mu_X$;しかし、$g_X$ は絶対値値 1 の写像であり、公式 (6) は § 5, No. 2 の提案 2 から導き出されます。

#### 注意 {#int-v-s7-n1-rem-2 .statement tag=096E}

— a) コル。 3 は、他の方法 (Ch. IV, § 5, No. 7、補題 3) によってすでに証明されています。
    b) コルのおかげで。 3、提案 1、提案 2、定理 1 の系 1、2、3 とその系 1、2、拡大するを一度に複雑な尺度に適用します。

#### スコリウム {#int-v-s7-n1-sch-1 .statement tag=096F}

— バナッハ空間 $F$ または $\overline{\mathbf{R}}$ の値を使用して $X$ (それぞれ $T$) に定義されたすべての写像 $f$ (それぞれ $g$) について、次のように表します。 $\zeta(f)$ (それぞれ $\rho(g)$) 拡大は、$f$ から $T$ の 0 (それぞれ $g$ から $X$ の制限) です。続いて$\zeta(\rho(g)) = \varphi_X \cdot g$、$\rho(\zeta(f)) = f$。 $T$ の$\varphi_X \cdot \mu$ の小節を $\mu'$ で表します。 $p \in [1, +\infty]$ ごとに、小道具。 1 と 2 は、$\zeta$ 写像 $\mathscr{L}_F^p(X, \mu_X)$ が $\mathscr{L}_F^p(T, \mu')$ に変換され、$\rho$ 写像 $\mathscr{L}_F^p(T, \mu')$ が $\mathscr{L}_F^p(X, \mu_X)$ に変換され、どちらの場合もノルムが保存され、次の場合の積分も保存されることを意味します。 $p = 1$ (木 1); 移行を関連するハウスドルフ空間にすると、互いに逆数の 2 つの同型が得られます。同様に、$\zeta$ と $\rho$ を正の数値写像に適用すると、本質的な上積分は保存されます (提案 1)。したがって、$X$の*同一視する* 写像とTの写像、つまりX−Tの零に同意すると、誘導措置に関する措置$\mu'$、問題の措置$\mu_X$が削減されます。 §5 で扱われる、密度によって定義される尺度については、問題まで。この種の推論は、Cor によると、複雑な対策にも適用できます。 Thの3。 1.

### 2. 誘導措置の性質

#### 命題 3 {#int-v-s7-prop-3 .statement tag=096G}

— X を T の局所的にコンパクトな部分空間とし、$\lambda$ を X の複素測度であるとします。次のプロパティは同等です。
a) 標準単射 $i : X \to T$ は $\lambda$ が適切です。
b) T のすべてのコンパクト部分集合 K について、$K \cap X$ は本質的に $\lambda$ 積分可能です。
c) すべての点 $t \in T$ は、$V \cap X$ が本質的に $\lambda$ 可積分であるような近傍 V を認めます。
d) T には $\theta_X = \lambda$ となるような尺度 $\theta$ が存在します。
これらの同等の条件が満たされる場合、d) のように記法を使用すると、次のようになります。

$$
(i(\lambda))_X = \lambda \quad \text{and} \quad i(\lambda) = i(\theta_X) = \varphi_X \cdot \theta .
$$

単射 $i$ は連続であるため、特性 a)、b)、および c) の同値は、§6 の提案 1 から得られ、それに続く注釈は、積極的な尺度 $|\lambda|$ に適用されます。 T 上の$\theta$ の測定によって $\lambda$ が X に誘導される場合、$|\lambda| = |\theta|_X$ (公式 (6))、その結果、T のすべての圧縮部分集合 K に対して $|\lambda|(K \cap X) = |\theta|(K \cap X) \leq |\theta|(K) < +\infty$ (提案 1) となり、d) は b) を意味します。 a) が満たされると仮定して、$(i(\lambda))_X = \lambda$ を示してください。これは d) を意味します。 g を $\mathscr{H}(X; \mathbf{C})$ の元とします。 $g'$ 拡大を g から T までの 0 で表し、誘導測度の定義で表し、次に §6, No. 4 の提案 7 で表します。

$$
\int g \, d(i(\lambda))_X = \int g' \, d(i(\lambda)) = \int (g' \circ i) \, d\lambda = \int g \, d\lambda .
$$

これで、4 つのプロパティのうち同値のうち証明が完了しました。 $\lambda = \theta_X$ と $g \in \mathscr{H}(T; \mathbf{C})$ の場合、

$$
\int g \, d(i(\theta_X)) = \int (g \circ i) \, d(\theta_X) = \int g \varphi_X \, d\theta ,
$$

なぜなら、$g \varphi_X$はTに対する$g \circ i$の0により拡大になるからです。これは(7)の2番目の公式を証明します。

#### 系 1 {#int-v-s7-prop-3-cor-1 .statement tag=096H}

— X が閉じている場合、X 上のすべての複雑なメジャー $\lambda$ は T 上のメジャーによって誘導されます。

なぜなら、K が T のコンパクト集合である場合、K ∩ X はコンパクトであるため、λ 積分可能です。

#### 系 2 {#int-v-s7-prop-3-cor-2 .statement tag=096I}

— θ を T 上の複素測度、π を T の θ 固有の写像を局所的にコンパクトな空間 Y に変換し、π_X をその制限から X とする。この場合、π_X は θ_X 固有であり、π_X(θ_X) = π(φ_X · θ) となります。

π_X = π ∘ i の場合、i は標準単射 X → T です。従って、θ が正の場合、系は、提案 3 と像尺度の推移性から推定できます (§6, No. 3、提案 4)。非正の複素測度の場合には、線形性が続きます。

#### 命題 4 {#int-v-s7-prop-4 .statement tag=096J}

— X と Y を、Y ⊂ X となるような T の 2 つの局所的にコンパクトな部分空間とする。 θ が T 上の複素測度である場合、Y 上の θ_X によって誘導される測度 (θ_X)_Y は θ_Y ('推移性の誘導測度') に等しくなります。

g が $\mathscr{H}(Y; \mathbf{C})$ の元である場合、g の 0 による T への拡大は、g の 0 による拡大を X まで拡張することによって得られるか、または再び Scholium の識別子 $\varphi_Y · \theta = \varphi_Y(\varphi_X · \theta)$ を利用して得られることを観察するだけで十分です。 (§5, No. 4、提案 8)。

#### 命題 5 {#int-v-s7-prop-5 .statement tag=096K}

— $(\lambda_\alpha)_{\alpha \in A}$ を T 上の正の測度の有向族増加するとし、最高値 λ を認め、X を T の局所コンパクト部分空間とする。誘導測度の族 $\lambda_\alpha|X$ は、$\mathscr{M}(X)$ で上に制限され、

$$
\sup_{\alpha \in A} (\lambda_\alpha|X) = \lambda|X.
$$

Scholium での識別を考慮すると、この命題は、§5, No. 4 の提案 5 の特殊なケースです。

#### 系 {#int-v-s7-n2-cor-1 .statement tag=096L}

— $(\mu_i)_{i \in I}$ を、和 μ を持つ、T 上の正の測度の合計可能な族とします。誘導測定値ファミリー $\mu_i|X$ は合計可能であり、

$$
\sum_{i \in I} (\mu_i|X) = \mu|X.
$$

#### 命題 6 {#int-v-s7-prop-6 .statement tag=096M}

— $\Lambda : t \mapsto \lambda_t$ を $\mathscr{M}_+(X)$ への T の μ 適切な写像とする。ここで、X は無限で可算な局所コンパクト空間であり、Y を X の局所コンパクト部分空間とする。 集合 $\int \lambda_t d\mu(t) = \nu$。 T の写像 $t \mapsto \lambda_t|Y$ から $\mathscr{M}_+(Y)$ はμ-適切であり、

$$
\int (\lambda_t|Y) d\mu(t) = \nu|Y.
$$

スコリウムでの識別を考慮すると、この命題は§5, No. 4の提案7の特殊なケースです。

### 練習問題 {#int-v-s7-exercises}

[§ 7 に対して練習問題](exercises/s7/)を参照してください。
