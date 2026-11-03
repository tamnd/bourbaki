---
book: alg
book_title: Algebra
chapter: V
chapter_title: COMMUTATIVE FIELDS
section: 16
section_title: Differential criteria of separability
lang: ja
source: alg-iv-vii
source_edition: 2003, Springer
book_pages: A V.127-A V.137, A V.177-A V.180
pdf_pages: 0241-0251, 0291-0294
extraction: ocr
subsections:
    - "no": 1
      title: 'Extension of derivations : the case of rings'
      page: 127
      pdf_page: 241
    - "no": 2
      title: 'Extension of derivations: the case of fields'
      page: 0
      pdf_page: 242
    - "no": 3
      title: Derivations in fields of characteristic zero
      page: 130
      pdf_page: 244
    - "no": 4
      title: Derivations in separable extensions
      page: 131
      pdf_page: 245
    - "no": 5
      title: The index of a linear mapping
      page: 132
      pdf_page: 246
    - "no": 6
      title: Differential properties of finitely generated extensions
      page: 133
      pdf_page: 247
    - "no": 7
      title: Separating transcendence bases
      page: 136
      pdf_page: 250
statements: 32
exercises: 9
content_sha256: 8c67cc274af94a96890c8c48c81d1f41978e4b77a6731a00e1f9ca58aaa743d6
translated_from: content/en/alg/V/16_s16_differential_criteria_of_separability.md
translation_method: google
source_content_sha256: 74e20434a4632131b94714a4b2546c552d9b686ae8250258434122a026af180b
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 5c7b68ef90bc7a5b08f2362d3b7ba243f28a659ecec623cdd1bd7e5ede65be8c
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 16。分離可能性の区別基準

### 1. 導分の拡大 : 環の場合

K を可換環、A 可換K-代数、および $x = (x_i)_{i \in I}$ とし、A の元の族とする。さらに、$A$ を K の導分から A-加群 M、他の語 (III, p. 553) a とする。 K の $c, c'$ に対する K の M 満たす関係 $\Delta(cc') = c \cdot \Delta(c') + c' \cdot \Delta(c)$ への Z 線形マッピング。各 $i \in I$ について、$D_i$ を多項式環 $K[X_i]_{i \in I}$ の $X_i$ に関する部分導分とします。これは、環をそれ自体に組み込んだ一意の導分で、K では零、$j \in I - \{i\}$ では $X_j$ であり、$X_i$ (IV, p. 6) では値 1 をとります。 $K[X_i]_{i \in I}$ のすべての多項式 $f = \sum_{a \in N^{(I)}} c_a \cdot X^\alpha$ を、M の $f^\Delta(x)$ 元 $\sum_{\alpha \in N^{(I)}} x^\alpha \cdot \Delta(c_\alpha)$ で表します。

#### 命題 1 {#alg-v-s16-prop-1 .statement tag=06UK}

— 家族 $x = (x_i)_{i \in I}$、生成する K-代数 A を仮定します。 $(m_i)_{i \in I}$ を M の元の家族とし、$(f_\lambda)_\lambda$ を多項式の家族生成するすべての多項式の理想的な $a$ とします。 $f \in K[X_i]_{i \in I}$ は $f(x) = 0$ になります。 A から M への導分 D が、すべての $c \in K$ に対して $D(c \cdot 1) = \Delta(c)$ となり、すべての $i \in I$ に対して $D(x_i) = m_i$ となるように存在するには、次のことが必要かつ十分です。

$$
f_\lambda^\Delta(x) + \sum_{i \in I} D_i f_\lambda(x) \cdot m_i = 0 \quad \text{for all} \quad \lambda \in A .
$$

そうであれば、導分 D は一意であり、次を満たします。

$$
D(f(x)) = f^\Delta(x) + \sum_{i \in I} D_i f(x) \cdot m_i \quad \text{for all} \quad f \in K[X_i]_{i \in I}
$$

$E = K[X_i]_{i \in I}$ を置き、E の K 準同型性の $\varphi$ を A に書き込むと、すべての $i \in I$ に対して写像 $X_i$ から $x_i$ になります。したがって、すべての $f \in E$ に対して $\varphi(f) = f(x)$ が得られます。 準同型 $\varphi : E \to A$ と定義する写像 $D'$ を使って M を E モジュールとみなします。E を $D'(f) = f^\Delta(x) + \sum_{i \in I} D_i f(x) \cdot m_i$ で M に変換します (ファミリー $(D_i f)_{i \in I}$ には各 $f \in E$ に対して有限台があることに注意してください)。 $D'$ は、E を M に拡張した一意の導分であり、各 $i \in I$ に対して A と写像 $X_i$ を $m_i$ に拡張したものであることは明らかです。

D を A の M への導分とし、すべての $c \in K$ に対して $D(c \cdot 1) = \Delta(c)$、すべての $i \in I$ に対して $D(x_i) = m_i$ とします。すると、$D \circ \varphi$はEの導分をMに拡張してAを拡張し、写像$X_i$をすべての$i \in I$に対して$m_i$とします。したがって、$D \circ \varphi = D'$、つまり関係 (2) が成立します。これは D の一意性を証明します。また、(1)は$f, (x) = 0$と(2)の帰結です。

逆に、(1) が成り立つと仮定します。他の語では、すべての $\lambda \in A$ に対して $D'(f_\lambda) = 0$ があります。 $f \in a$ にしましょう。 $E$ に $f = \sum_{\lambda \in \Lambda} q_\lambda \cdot f_\lambda$ となるような有限台 $(q_\lambda)_{\lambda \in \Lambda}$ を持つ家族が存在します。私たちは持っています
$$
D'(f) = \sum_{\lambda \in \Lambda} [f_\lambda(x) \cdot D'(q_\lambda) + q_\lambda(x) \cdot D'(f_\lambda)]
$$
よって $D'(f) = 0$ は、$f_\lambda(x)$ と $D'(f_\lambda)$ はすべての $\lambda \in A$ に対して零であるためです。 $D'$ は $a$ に消えるため、$D' = D \circ \varphi$ のような $A$ から $M$ への $Z$ 線形写像 $D$ が存在します。明らかに、$D$ は、$A$ から $M$ に必要な導分です。

### 2. 導分の拡大: 体の場合

$K, L$ と $M$ を体とし、$K \subset L \subset M$ とします。提案 21 (III, p. 572) により、ベクトル $M$ スペースのうち完全系列が得られます
$$
(\mathrm{E}_{K,L,M}) \quad \Omega_K(L) \otimes_L M \xrightarrow{\alpha} \Omega_K(M) \xrightarrow{\beta} \Omega_L(M) \to 0 ;
$$
$M$ 線形マッピング $\alpha$ と $\beta$ は関係によって特徴付けられます
$$
(3) \quad \alpha(d_{L/K} x \otimes 1) = d_{M/K} x \quad \text{for } x \in L \\
(4) \quad \beta(d_{M/K} y) = d_{M/L} y \quad \text{for } y \in M
$$

$V$ をベクトル $M$ 空間とし、$V$ に値を含む $M$ の $K$ 導出の $D_K(M, V)$ ベクトル空間で表し、同様に $D_K(L, V)$ と $D_L(M, V)$ を導入します。 III、p. 571、図式 (42) と III、p. 572、図式 (44) により、ベクトル空間の準同型の可換図式が得られます。
$$
\begin{array}{ccccccccc}
0 \to \mathrm{Hom}_M(\Omega_L(M), V) & \xrightarrow{\mathrm{Hom}(\beta, 1)} & \mathrm{Hom}_M(\Omega_K(M), V) & \xrightarrow{\mathrm{Hom}(\alpha, 1)} & \mathrm{Hom}_M(\Omega_K(L) \otimes_L M, V) \\
\downarrow & & \downarrow & & \downarrow \\
0 \to \mathrm{Der}_L(M, V) & \xrightarrow{i_V} & \mathrm{Der}_K(M, V) & \xrightarrow{r_V} & \mathrm{Der}_K(L, V),
\end{array}
$$
ここで、垂直矢印は同型、$i_V$ は標準単射、$r_V$ 制限写像です。

したがって、II, p. 299, Th から得られます。 5 および II、p. 301、提案 10、以下の命題:

#### 命題 2 {#alg-v-s16-prop-2 .statement tag=06UL}

— *以下の条件は同等です*:
a) *マッピング $\alpha$ は単射法です*。
b) *$L$ から $M$ へのすべての $K$ 導出は、$M$ から $M$* への $K$ 導出まで拡張されます。
c) *ベクトル $M$ 空間 $V$ への $L$ のすべての $K$-導出は、$M$ から $V$* への $K$-導出まで拡張されます。

#### 命題 3 {#alg-v-s16-prop-3 .statement tag=06UM}

— *$K$を体、$L$を$K$の純粋な拡大、$(x_i)_{i \in I}$を$L$*の純粋な基底とします（V、p. 106、定義2）。

a) $V$ を $L$ のベクトル空間 、$K$ の $A$ 導分を$V$ および$(v_i)_{i \in I}$ の$V$ の元の家族にします。 $L$ から $V$ への固有の導分 $D$ が存在し、$A$ を拡張し、すべての $i \in I$ に対して $D(x_i) = v_i$ になります。

b) $L$ の $K$-微分 のベクトル $L$ 空間 $\Omega_K(L)$ は、基底としてファミリー $(dx_i)_{i \in I}$ を持ちます。

主張 b) は IV、p. 23 および主張 a) で証明されています。

#### 系 {#alg-v-s16-n2-cor-1 .statement tag=06UN}

— $P$ を $K$ の部分体とします。 $\Omega_P(K) \otimes_K L$ の $\Omega_P(L)$ への正規写像 $\alpha$ は単射的であり、族 $(d_{L/P} x_i)_{i \in I}$ は、$\alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L)$ のイメージを補足する $\Omega_P(L)$ の部分空間の基礎 ($L$ 上) です。

提案 3、a) は、$L$ 上のベクトル空間 $V$ への $K$ のすべての $P$ 導出が、$L$ から $V$ への $P$ 導出まで拡張されることを示しています。 $\alpha$ の単射性の後に、提案 2 が続きます。 系の 2 番目の主張は、数列 $(\mathbf{E}_{P,K,L})$ と提案 3、b) の正確性から導き出されます (公式 (4) を考慮に入れて)。

#### 命題 4 {#alg-v-s16-prop-4 .statement tag=06UO}

— $K$ を体、$L$ を $K$ の分離可能な代数拡張、$V$ を $L$ 上のベクトル空間とします。

a) $L$ から $V$ へのすべての $K$ 導出は零です。

b) $A$ が $K$ の $V$ への導分である場合、$L$ の $V$ への拡大する $A$ の一意の導分 $D$ が存在します。

$D$ を $L$ から $V$ への $K$ 導関数とします。 $E$ が $K$ 上の有限次数の $L$ の部分拡張である場合、$K$-代数 $E$ はエタールであるため、$\Omega_K(E) = 0$ ($V$, p. 33, Th. 3), よって $D|_E = 0$ $\Omega_K(E)$ の普遍性による (III、p. 569)。 $L$ は、$K$ に対する有限次数の部分拡張ファミリーの和集合であるため、$D = 0$、よって a) が得られます。

$A$を$K$の導分を$V$とします。 $D'$と$D''$が$A$の2つの拡大から$L$の導分を$V$に変換したものである場合、差$D' - D''$は$L$の$K$導関数です。 $V$;したがって、a) によって零となり、したがって $D' = D''$ となります。

$A$の拡大の存在を証明することが残っています。 Zorn の補題 (E、III、p. 20) は、$L$ の部分体 $L_0$ で定義される $A$ から導分までの最大拡大 $D_0$ の存在を意味します。 含む $K$。

$x$ を $L$ と $g$ 、$L_0$ 上の $x$ の最小多項式に入れる。 $L$ は代数的であり、$K$ 上で分離可能であるため、$x$ は代数的であり、$L_0$ 上で分離可能です ($V$、p. 39、Prop. 6 および p. 39、Cor. 2)。したがって、$x$ は、$g$ ($V$、p. 39、提案 5)、よって $g'(x) \neq 0$ (IV、p. 17、提案 7) の単純な根です。 $V$、p. 127 のように定義する $g^{D_0}(x)$ とすると、$g^{D_0}(x) + g'(x) \cdot u = 0$ となる $V$ のうち元 $u$ が存在します。提案 1 (V, p. 127) により、$D_0$ を拡張する$V$ に$L_0(x)$ の導分 $D$ が存在し、$D(x) = u$ になります。 $(L_0, D_0)$ の最大値指標を考慮すると、$L_0(x) = L_0$、よって $x \in L_0$ になります。 $x$ は任意であったため、$L_0 = L$ を結論するとしました。

#### 系 1 {#alg-v-s16-prop-4-cor-1 .statement tag=06UP}

— $L$ が代数的で、$K$ 上で分離可能である場合、$\Omega_K(L) = 0$ が得られます。

系は、ベクトル $L$-空間 $\Omega_K(L)$ が標準的な $K$ 導出 $d_{L/K} : L \to \Omega_K(L)$ の像によって生成されるため、提案 4、a) から導かれます。

#### 系 2 {#alg-v-s16-prop-4-cor-2 .statement tag=06UQ}

— *L が代数で、体 K の分離拡大の場合、標準写像 $\alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L)$ は K の部分体 P ごとに同型になります。*

写像 $\alpha$ は、提案 2 (V、p. 128) および提案 4、*b*) によって単射的です。 $\Omega_K(L)$ 簡約するから 0 (Cor. 1) なので、正確さ数列 $(E_{P.K.L})$ は、$\alpha$ が全射であることを意味します。

#### 系 3 {#alg-v-s16-prop-4-cor-3 .statement tag=06UR}

— *E を体 K の拡大および E の導分を E に、写像 K を K にするとします。 L が代数的で K について分離可能な E の部分拡張である場合、$D(L) \subset L$ です。*

A を K の L への K の導分とします。これは K の D と一致します。提案 4 (V, p. 129) により、A を拡張して L の L への導分 D' が存在します。ここで、D の D' と制限 D'' を考えてみましょう。 $L$ の導分として L を E に変換します。彼らは K について同意しているので、提案 4、よってにより $D' = D''$ が得られます。

$$
D(L) = D''(L) = D'(L) \subset L .
$$

#### 注意 {#alg-v-s16-n2-rem-1 .statement tag=06US}

— 1) 後で (V, p. 131, Cor. 3 および p. 135, Cor. 2) 逆を Cor. 2 に証明することになります。提案 4 の 1。

2) 素数体のすべての代数拡大は分離可能です (V, p. 37, Cor.)。素数体のすべての導分は零であるため、素数体の代数拡大のすべての導分は零です (提案 4)。

### 3. 標数0 の体に導分

#### 定理 1 {#alg-v-s16-thm-1 .statement tag=06UT}

— *K を特性 0 の体、K の L 拡大、および L 上の V ベクトル空間とします。 AをKの導分からV、$(x_i)_{i \in I}$、Kに対するLの超越基底、およびVの元の族である$(u_i)_{i \in I}$とする。次に、A を拡張する V に L の一意の導分 D が存在し、すべての $i \in I$ に対して $D(x_i) = u_i$ になります。*

$E = K(x_i)_{i \in I}$を入れてください。提案 3 (V, p. 128) は、E の拡大するから一意の導分 $D_0$ を V に変換し、すべての $i \in I$ に対して $D_0(x_i) = u_i$ となることを示しています。 体 $L$ は E の代数拡大であり、L は標数 0 であるため、L は E 上で分離可能です (V, p. 37, Cor.)。したがって、(V, p. 129、提案 4) $D_0$ 拡大するを $L$ の一意の導分 D から V に変換します。

#### 系 1 {#alg-v-s16-thm-1-cor-1 .statement tag=06UU}

— *K の導分を V 拡大するから L の導分を V に*

#### 系 2 {#alg-v-s16-thm-1-cor-2 .statement tag=06UV}

— *E を L の部分拡張とし、U ベクトルを E の元の微分によって生成される $\Omega_K(L)$ の部分L 空間とする。元 x が E 上で代数的であるためには、$dx \in U$ であることが必要かつ十分である。

それぞれの $y \in L$ について、D(y) を $dy$ mod U の剰余類とします。すると、D は $\Omega_K(L)/U$ への L の E 微分になります。 K は標数 0 であるため、E のすべての代数拡大は分離可能です (V, p. 37, Cor.) 。 $x \in L$ が E 上の代数である場合、提案 4 (V, p. 129) により $Dx = 0$、つまり $dx \in U$ が得られます。

$x \in L$ が $E$ に対して超越的である場合、$\Delta(x) = 1$ ($V$, p. 128、提案 3) のように、$E(x)$ から $L$ への E 導出$A$ が存在します。 Th 著1、$A$ 拡大するを$L$ の E 導出 D から L に変換します。 $\varphi$ を $\Omega_K(L)$ で線型形式とし、$D = \varphi \circ d$ とします。 $y \in E$と$\varphi(x) = 1$、よって$dx \notin U$には$\varphi(dy) = 0$があります。

#### 系 3 {#alg-v-s16-thm-1-cor-3 .statement tag=06UW}

— *Lの元xがK上で代数的であるためには、$\Omega_K(L)$の$dx = 0$であることが必要かつ十分です。特に、L が K の代数的な拡大であるためには、$\Omega_K(L) = 0$ であることが必要かつ十分です。
これはコルからすぐに続きます。 $E = K$を取ると2。

#### 系 4 {#alg-v-s16-thm-1-cor-4 .statement tag=06UX}

— *K、L、M を標数 0 の体とし、$K \subset L \subset M$ となるようにします。その場合、標準写像 $a : \Omega_K(L) \otimes_L M \to \Omega_K(M)$ は単射です。
これはコルからすぐに続きます。 1 および$V$、p. 128、提案 2。

#### 定理 2 {#alg-v-s16-thm-2 .statement tag=06UY}

— *K を特性 0 の体、K の L 拡大、および L の元の族である $(x_i)_{i \in I}$ とします。
a) $(x_i)_{i \in I}$ について、K 上で代数的に自由であるためには、$\Omega_K(L)$ の微分 $dx_i$ ($i \in I$ の場合) が L 上で線形自由であることが必要かつ十分です。
b) L が $K(x_i)_{i \in I}$ 上で代数的であるためには、$i \in I$ 生成するベクトル空間 $\Omega_K(L)$ のL に対する微分 $dx_i$ が必要かつ十分です。
c) $(x_i)_{i \in I}$ が K に対する L の超越基底であるためには、族 $(dx_i)_{i \in I}$ が L に対する $\Omega_K(L)$ の基底であることが必要かつ十分です。
$i \in I$ ごとに、$E_i$ を L の部分体 $K(x_j)_{j \in I, j \neq i}$ とします。族 $(x_i)_{i \in I}$ にとって、K 上で代数的に自由であるためには、$x_i$ が各 $i \in I$ に対して $E_i$ 上で超越的であることが必要かつ十分です ($V$, p. 108、提案 5)。コル著Thの2。 1 これは、各 $i \in I$ の差分 $dx_i$ が、I の $j \neq i$ との差分 $dx_j$ の L の係数が線形結合ではないことを意味します。後者の条件は、家族 $(dx_i)_{i \in I}$ が L、よって a) を超えて自由であることを意味します。
主張 b) コルからすぐに続きます。 Thの2。 1とc)はa)とb)の帰結です。

#### 系 {#alg-v-s16-n3-cor-1 .statement tag=06UZ}

— *K が標数 0 の場合、$[\Omega_K(L) : L] = \operatorname{tr} \cdot \deg_K L$ になります。

### 4. 導分の分離拡大

($V$, p. 122, Th. 1) 標数 0 の体 $K$ のすべての拡大 $L$ が分離可能であることを見てきました。さらに、K の導分ごとに $L$ 拡大するを経てベクトル空間になり、その後 $L$ ($V$、p. 130、Cor. 1) の導分になります。より一般的には、次の主張があります。

#### 定理 3 {#alg-v-s16-thm-3 .statement tag=06V0}

— *K を K の体と L 拡大とします。 L が K 上で分離可能であるためには、ベクトル L 空間への K のすべての導分が L の拡大するから導分に収まる必要があって十分です。
K は特性 $\neq 0$ を持っていると仮定できます。 まず、L が K に関して分離可能であると仮定します。 $V$ を L のベクトル空間と K の $A$ 導分を $V$ にするとします。 マックで

レーンの基準 (V、p. 124、注意)、体 $L^p$ および $K$ は、$K^p$ に対して互いに素を直線的に上回ります。 Since $A$ is a $K^p$-linear mapping of $K$ into $V$, it extends in a unique way to an $L^p$-linear mapping $A'$ of $K[L^p] = K(L^p)$ into $V$. $A'$ は $K(L^p)$ の導分から $V$ になり、$L^p$ で消滅することは明らかです。したがって、拡大する (V、p. 103、コリント 3) から $L$ の導分が $V$ になります。

逆に、$L$ の値による $K$ のすべての導出が、$L$ から $L$ への導出まで拡張されると仮定します。 $B$ を $K$ (V, p. 99) の p 基底とし、$A$ を $()$ と $p - 1$ の間の整数で構成される有限サポートを持つファミリー $(\alpha_h)_{h \in R}$ のセットとします。 各 $b \in B$ には、$b' \in B$ (V、p. 103) ごとに $\Delta_b(b') = \delta_{bb'}$ (クロネッカー記号) によって特徴付けられる $K$ から $K$ への導分 $\Delta_b$ が存在します。 仮定までに、$L$ の各 $b \in B$ 導分 $D_b$ が$\Delta_b$ を拡張する $L$ に存在します。 $B$ の $b, b'$ に対して $D_b(b') = \delta_{bb'}$ が得られ、$\Omega_{1/p}(L)$ では微分 $db$ ($b \in B$ の場合) が $L$ にわたって線形独立していることが証明されます。 したがって (V、p 102、Th. 1)、$B$ は $L^p$ に対して p-free です。 (V、p. 98、提案 1 および p. 124、注意) より、$K$ の拡大 $L$ は分離可能です。

#### 系 {#alg-v-s16-n4-cor-1 .statement tag=06V1}

— *$L$ が $K$ の分離拡大である場合、標準写像 $\alpha_p : \Omega_p(K) \otimes_K L \to \Omega_p(L)$ は $K$ の部分体 $P$ ごとに単射になります。逆に、写像 $\alpha_p$ が単射であるような、$K$ の完全な部分体 $P$ (たとえば、$K$ の素数部分体) が存在する場合、$L$ は $K$ で分離可能です。

最初の主張は、提案 2 (V、p. 128) と Th から続きます。 3. 逆に、$P$ を $K$ の完全な部分体とします。 $P = P^p \subset K^p$ があるため、$K$ のすべての導分をベクトル $L$ 空間に入れると、$P$ の導出になります。 系の 2 番目の主張がコルから続きます。 2 (V、p. 130) と Th. 3.

### 5. 線形写像中添字

$L$ を体 $^1$ とし、$U$ と $V$ を 2 ベクトル空間 $^2$ $L$ と $f : U \to V$ 上の$L$ 線形マッピングとします。 $f$ の核 $N$ と余核 $C$ が有限次元と整数を持つ場合、$f$ は *有限の添字* を持つと言われます

$$
\chi(f) = [C : L] - [N : L]
$$

は $f$ の *添字* と呼ばれます。

#### 補題 1 {#alg-v-s16-lem-1 .statement tag=06V2}

— *$U$ と $V$ を体 $L$ 上の有限次元の 2 つのベクトル空間とします。すべての線形写像 $f : U \to V$ は、$[V : L] - [U : L]$ に等しい添字を所有します。*

$N$ を $f$ の核、$I$ 像、$C$ 余核とします。 $C = V/I$ があり、$I$ は $U/N$ と同型です。したがって、結果は $[U : L] = [N : L] + [I : L]$ と $[V : L] = [C : L] + [I : L]$、 よってになります。

$^1$ 必ずしも可換であるとは限りません。
$^2$ 左側。

#### 補題 2 {#alg-v-s16-lem-2 .statement tag=06V3}

$f : U \to V$ と $g : V \to W$ を 2 つの L 線形マッピングとします。 ff と g がそれぞれ添字を持つ場合、同じことが $g \circ f$ にも当てはまり、次のようになります。

$$
\chi(g \circ f) = \chi(f) + \chi(g).
$$

$h = g \circ f$ を置き、N、N'、N'' で核 off、g、h をそれぞれ表し、C、C'、C'' で余核を表します。 $N \subset N'' \subset U$ と $f(N'') = f(U) \cap N'$ があります。したがって、N'' 上の f と一致し、核 N と一致する線形写像 $\bar{f} : N'' \to N'$ が存在します。 V の標準写像 $\pi$ が $C = V / f(U)$ 誘導する写像 $\pi'$ から C になります核は$f(U) \cap N' = \bar{f}(N'')$です。 $C = V/f(U)$ の商 g 定義する写像 $\bar{g}$ から $C'' = W/g(f(U))$ に進み、その核は明らかに $(N' + f(U))/f(U) = \pi'(N')$ です。最後に、$C'' = W/g(f(U))$ の $C' = W/g(V)$ への標準写像 $\rho$ は核 $g(V)/g(f(U)) = \bar{g}(C)$ になります。 和まで、数列の正確性を確立しました

$$
0 \to N \xrightarrow{i} N'' \xrightarrow{\bar{f}} N' \xrightarrow{\pi'} C \xrightarrow{\bar{g}} C'' \xrightarrow{\rho} C' \to 0
$$

(i は N の N の標準単射です)。

![図式は、N、N'、N''、U、V、W、C、C'、C'' の関係を示し、写像と核を示す矢印](../images/fig_1.png)

図1

仮定 N、N'、C、C' は有限次元になります。したがって、N'' と C にも同じことが当てはまります。コル著2 (II, p. 295) 次に、

$$
[N : L] - [N'' : L] + [N' : L] - [C : L] + [C'' : L] - [C' : L] = 0
$$

よって $\chi(h) = \chi(f) + \chi(g)$。

### 6. 有限生成された拡大の微分特性

#### 定理 4 {#alg-v-s16-thm-4 .statement tag=06V4}

P を P の完全体、L 拡大、K を L の部分拡張とする。 L は K の有限生成拡大であると仮定します。すると、正規 L 線形写像 $a : \Omega_p(K) \otimes_K L \to \Omega_p(L)$ は、K に対する L の超越次数に等しい添字を持ちます。

$E$ と $F$ が $E \subset F$ のような $L$ の 2 つのサブ拡張である場合、$\Omega_p(E) \otimes_E F$ から $\Omega_p(F)$ への正規の $F$ 線形マッピングを $\alpha(F/E)$ で表し、それが定義されると、$\alpha(F/E)$ の添字が書き込まれます。 $d(F/E)$。 $E, F$ と $G$ が $E \subset F \subset G$ となるような $L$ の 3 つの部分拡張である場合、可換図式が得られます。

$$
\begin{array}{ccc}
\Omega_p(F) \otimes_F G & \xrightarrow{\alpha(G/F)} & \Omega_p(G) \\
\uparrow \alpha(F/E) \otimes_F \mathrm{Id}_G & & \uparrow \alpha(G/E) \\
(\Omega_p(E) \otimes_E F) \otimes_F G & \xrightarrow{\beta} & \Omega_p(E) \otimes_E G
\end{array}
$$

ここで、$\beta$ は、提案 2 (II、p. 278) で定義された標準同型です。 添字はスカラーにより拡大の下で明らかに不変であり、同型の添字は零であるため、補題 2 ($V$, p. 133) は、添字 $d(G/E)$ が次のように定義されることを示します。 $d(F/E)$ と $d(G/F)$ は、その後

$$
d(G/E) = d(G/F) + d(F/E).
$$

$L$ は、$K$、公式 (5) および Cor の有限生成された拡大であるため、 $V$、p. 111 は、$L = K(x)$ となるように $x$ が存在する場合を考慮すれば十分であることを示しています。さらに、$x$ が $K$ 上で代数的である場合、$L$ の標数指数の冪 $q$ が存在し、$x^q$ は $K$ ($V$, p. 44,提案 13)。したがって、以下の 3 つの特殊なケースで等式 $d(L/K) = \operatorname{tr} . \deg_K L$ を確立するだけで十分です。

a) $x$ は $K$ に対して超越的です。その場合、$a$ は単射であり、その余核は $L$ ($V$, p. 129, Cor.) に対して階数 1 です。したがって、$d(L/K) = 1$ と $\operatorname{tr} . \deg_K L = 1$ もあります。

b) $x$ は、$K$ に対して可分代数です。その場合、$a$ は全単射 ($V$、p. 130、Cor. 2)、よって $d(L/K) = 0$ です。明らかに$\operatorname{tr} . \deg_K L = 0$も。

c) *体 $L$ は特性 $p \neq 0$、$x \notin K$ および $x^p = a$ は $K$* にあります: $a$ の余核 $C$ は $\Omega_K(L)$ と同型であり、$\{ x \}$ は a であるため、 $p$ - $K$ に対する $L$ の基準、空間 $C$ は、$L$ に対する次元 1 ($V$、p. 102、Th. 1) です。 $a$ は $L$ の $p$ 番目の冪であるため、$a$ 含む部分空間 $R$ $U = \Omega_p(K) \otimes_K L$ の $d_{L/pa} = 0$ と核が生成されます。 $d_{K/pa} \otimes 1$。それぞれの $y \in K$ について、$\Delta(y)$ を $d_{K/p}y \otimes 1$ mod $R$ の剰余類とします。この場合、$A$ は、$K$ から $U/R$ への $P$ 導関数であり、$\Delta(a) = 0$ になります。提案 5 ($V$, p. 101) は、$A$ 拡大するから $L$ の $P$ 導出$D$ が $U/R$ になることを示しています。したがって、$D = \beta \circ d_{L/P}$ と $\beta \circ a$ が $U/R$ への $U$ の標準写像となるような $L$ 線形写像 $\beta : \Omega_p(L) \to U/R$ が存在します。これにより、$R$は$a$の核であることが証明されます。 $P$ は完全なので、$P(K^P) = K^p$、よって $a \notin P(K^P)$、そして最後に $d_{K/pa} \neq 0$ ($V$、p. 103、提案 6) が得られます。したがって、$a$ の核と余核は、次元 1、よって $d(L/K) = 0$ であり、$\operatorname{tr} . \deg_K L = 0$ もあります。

#### 系 1 {#alg-v-s16-thm-4-cor-1 .statement tag=06V5}

— *$L$を、超越次数$s$の体$K$の有限生成拡大とする。 ベクトル空間 $\Omega_K(L)$ は、$L$ 上で次元 $\geq s$ であり、$L$ が$K$ 上で分離可能な場合に限り、等式になります。*

P を K の素数部分体とします。N を α の核とし、正確さ数列 $(\mathbf{E}_{P,K,L})$ (V, p. 128) と Th とします。 4、$[ \Omega_K(L) : L ] = s + [N : L]$があります。 by V, p. 132, Cor., 拡大 L の K は、$N = 0$ の場合にのみ分離可能です。 系が続きます。

#### 系 2 {#alg-v-s16-thm-4-cor-2 .statement tag=06V6}

— *L を体 K の有限生成された拡大とします。 L が代数的で K 上で分離可能であるためには、 $\Omega_K(L) = 0$ であることが必要かつ十分です。* これは Cor から直接続きます。 1.

#### 系 3 {#alg-v-s16-thm-4-cor-3 .statement tag=06V7}

— *K を特性 $p \neq 0$ の体および超越次数の K の有限生成された拡大である L とします。 $[K : K^p]$ が有限である場合、同じことが $[L : L^p]$ にも当てはまり、$[L : L^p] = p^s$ が得られます。 $[K : K^p]$.* P を K の素数部分体とします。$[K : K^p]$ が有限である場合、ベクトル空間 $\Omega_P(K) = \Omega_{K^p}(K)$ は K 上の有限次元 m であり、$[K : K^p] = p^m$ (V, p. 103, Th. 2) が得られます。 ベクトル空間 $\Omega_P(K) \otimes_K L$ は、L を超える有限次元 m になります。さらに、K は $K^p$ に対して有限次数であるため、体 $K(L^p)$ は $K^p(L^p) = L^p$ に対して有限次数です。 体 L は K の有限生成された拡大であり、$K(L^p)$ に対して代数的であるため、$K(L^p)$ の有限次数の拡大 (V, p. 18, Th. 2)。したがって、L は $L^p$ よりも有限次数であるという結論する (V、p. 10、Th. 1)。すると、$\Omega_P(L)$ は L 上の有限次元のベクトル空間で、$[L : L^p] = p^n$ (V, p. 103, Th. 2) になります。 補題 1 (V, p. 132) により、L 線形写像 $\alpha : \Omega_P(K) \otimes_K L \to \Omega_P(L)$ は Th により添字 $n - m$, よって $n - m = s$ になります。 4 (V、p. 133) と $p^n = p^s \cdot p^m$。

#### 注意 1 {#alg-v-s16-n6-rem-1 .statement tag=06V8}

K を特性 $p \neq 0$ の体と K の L 拡大とします。$L = K(L^p)$ (V、p. 103、提案 6) の場合に限り、$\Omega_K(L) = 0$ が得られます。したがって、L が K 上で有限に生成される場合、それは代数であり、$L = K(L^p)$ がある場合に限り、分離拡大になります。 L が K 上で有限に生成されない場合、L が K の完全閉包である場合に示されるように、この結果は一般的には当てはまりません。

#### 注意 2 {#alg-v-s16-n6-rem-2 .statement tag=06V9}

K を、元 $x_1, \ldots, x_n$ によって生成された K の $K[X_1, \ldots, X_n]$ および L 拡大の多項式体、$F_1, \ldots, F_m$ とします。多項式 $F_1, \ldots, F_m$ 生成するが $F(x_1, \ldots, x_n) = 0$ となるようなすべての多項式 F の $K[X_1, \ldots, X_n]$ からなるの理想であると仮定します。提案 1 (V、p. 127) と微分 (III、p. 569) の加群の普遍性から、次の結果が簡単に推測できます: L に対するベクトル空間 $\Omega_K(L)$ は $dx_1, \ldots, dx_n$ によって生成されます。 関係があります

$$
\sum_{i=1}^n D_i F_j(x_1, \ldots, x_n) \cdot dx_i = 0 \quad \text{(for } 1 \leq j \leq m \text{)} ;
$$

最後に、$u_1, \ldots, u_n$ が $\sum_{i=1}^n u_i \cdot dx_i = 0$ となるような L の元である場合、$1 \leq i \leq n$ に対して $u_i = \sum_{j=1}^m D_i F_j(x_1, \ldots, x_n) \ v_j$ となるような L の元 $v_1, \ldots, v_m$ が存在します。 n 行、m 列の行列 $(D_i F_j(x_1, \ldots, x_n))$ の r 階数で表します。 $K$を超える$L$の超越次数になりましょう。次に$[ \Omega_K(L) : L ] = n - r$です。したがって、$K$ の拡大 $L$ は、$r + s = n$ (Cor. 1) の場合にのみ分離可能です。そしてそれは代数的であり、$r = n$ (Cor. 2) の場合に限り分離可能です。

### 7. 超越の分離基底

#### 定義 1 {#alg-v-s16-def-1 .statement tag=06VA}

*$L$を体$K$の拡大とします。 $K(B)$ の代数拡大 $L$ が分離可能である場合、$L$ の $K$ の超越基底 $B$ は分離していると言われます。

$K$ が標数 0 を持つ場合、標数 0 の体のすべての代数拡大が分離可能であるため、$K$ 上の $L$ のすべての超越基底は分離します ($V$, p. 37, Cor.)。 拡大が分離超越基底を認める場合、それは分離可能です ($V$、p. 121、提案 6 および p. 122、提案 9)。次の定理は、すべての *有限生成* 分離拡大が分離する超越性基底を認めることを示しています。この制限は必須です ($V$、p. 177、例 1)。

#### 定理 5 {#alg-v-s16-thm-5 .statement tag=06VB}

*$K$を体、$L$拡大の$K$、$(x_i)_{i \in I}$を、$L$の元の家族とします。 ファミリー $(x_i)_{i \in I}$ が $K$ 上の $L$ の分離超越基底である場合、ファミリー $(dx_i)_{i \in I}$ は $L$ 上のベクトル空間 $\Omega_K(L)$ の基底です。 $L$ が $K$ の有限生成された分離拡大である場合、逆が成り立ちます。

$M = K(x_i)_{i \in I}$を入れて、$\Omega_K(M) \otimes_M L$の標準写像を$\Omega_K(L)$に$\alpha$で表します。 $(x_i)_{i \in I}$ が $K$ 上の $L$ の分離超越基底である場合、族 $(d_{M/K} x_i)_{i \in I}$ は、ベクトル $M$-空間 $\Omega_K(M)$ の基底 ($V$, p. 128, Prop. 3) そして、$L$ は代数的であり、$M$ ($V$, p. 130, Cor. 2) 上で分離可能であるため、$\alpha$ はベクトル $L$ 空間の同型です。 $\alpha(d_{M/K} x_i \otimes 1) = d_{L/K} x_i$ なので、家族 $(d_{L/K} x_i)_{i \in I}$ は、$L$ を超えた $\Omega_K(L)$ の基底になります。

逆に、$L$ が $K$ の可分有限生成拡大であり、族 $(d_{L/K} x_i)_{i \in I}$ が $L$ 上のベクトル空間 $\Omega_K(L)$ の基底であるとします。 コル著$V$、p. 134の1、$K$に対する$L$の超越次数は、$L$に対する$\Omega_K(L)$の次元、したがって$I$の基数に等しい。 正確なシーケンス $(E_{K,M,L})$ ($V$, p. 128) から、$\Omega_M(L) = 0$ が得られます。 $L$ は $M$ の有限生成された拡張であるため、Cor. $V$、p. 135 の 2 は、$L$ が代数的であり、$M = K(x_i)_{i \in I}$ 上で分離可能であることを示しています。 $K$ に対する $L$ の超越度は有限であり、基数 $I$ に等しいため、族 $(x_i)_{i \in I}$ は $K$ に対する $L$ の超越基底です ($V$、p. 110、コリント 1)。

#### 系 {#alg-v-s16-n7-cor-1 .statement tag=06VC}

*$L$を$K$の分離可能な有限生成拡大とし、$S$を$L = K(S)$となるような$L$の部分集合とする。そして、$S$に含まれる$K$を超える$L$の分離超越基底$B$が存在します。

$\Omega_K(L)$は$S$の元の差分によって生成されるので、$(dx_1, \ldots, dx_s)$が$L$を超えた$\Omega_K(L)$の基底となるように、$S$の$s$元$x_1, \ldots, x_s$が存在します。ここで、Th を適用するだけで十分です。 5.

#### 注意 {#alg-v-s16-n7-rem-1 .statement tag=06VD}

— $L$ を特性 $p \neq 0$ の体 $K$ の可分有限生成拡大とします。分離していない$L$の超越基底が存在する可能性があります。 $\{X^p\}$ は $K(X)$ の超越基底ですが、$K(X)$ は $K(X^p)$ の次数 $p$ の p 根拡張であることを観察するだけで十分です。

#### 命題 5 {#alg-v-s16-prop-5 .statement tag=06VE}

— *L と M を、与えられた拡大に含まれる 2 つの体 K の 2 つの拡大とし、K 上で代数的に互いに素とする。M が K 上で分離可能である場合、L(M) は L 上で分離可能である。*

M の有限部分集合 S ごとに、$L(S)$ が L (V, p. 122、提案 8) 上で分離可能であることを示すだけで十分です。 S を M の有限部分集合とします。 体 $K(S)$ は K 上で分離可能であるため、分離超越基底 B (Th. 5 の Cor.) を持ちます。 L と M は K に対して代数的に互いに素であるため、B は L に対する $L(B)$ の超越基底 (V, p. 113、提案 12)。さらに、S のすべての元は代数的であり、$K(B)$ にわたって、したがって $L(B)$ にわたって分離可能です (V, p. 39、Cor. 2)。 $L(S) = L(B)(S)$ は代数的であり、$L(B)$ 上で分離可能であるため、$L(S)$ は L 上で分離可能であると推論します (V, p. 39、提案 6)。

#### 系 {#alg-v-s16-n7-cor-2 .statement tag=06VF}

— *L と M が分離拡大である場合、K 上で代数的に互いに素となり、体 $K(L \cup M)$ は K 上で分離可能です。*

$K(L \cup M) = L(M)$ は提案 5 によって L 上で分離可能であり (M は K 上で分離可能であるため)、L は K 上で分離可能であるため、よって系 (V、p. 122、提案 9)。

拡大 L と M が代数的に互いに素であるという仮定は、提案 5 とその系において不可欠です。なぜなら、K を標数 $p \neq 0$ の不完全体および形 $K(x, a)$ の E 拡大とし、 x が K を超越し、K を高さ 1 の p 根とする。 $L = K(x)$と$M = K(x + a)$を入れます。この場合、$x + a$ は K 上で超越的であり (そうでない場合、$x = (x + a) - a$ は K 上で代数的になります)、体 L と M は K 上で分離可能です。ただし、$K(L \cup M) = K(x, a)$ は $L = K(x)$ 上で次数 $p$ の p 根であり、分離可能ではありません。 L、K を超えない。

### 練習問題 {#alg-v-s16-exercises}

[§ 16 に対して練習問題](exercises/s16/)を参照してください。
