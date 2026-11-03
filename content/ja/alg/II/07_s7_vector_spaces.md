---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 7
section_title: Vector spaces
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 292-316, 400-409
pdf_pages: 0316-0340, 0424-0433
extraction: ocr
subsections:
    - "no": 1
      title: BASES OF A VECTOR SPACE
      page: 292
      pdf_page: 316
    - "no": 2
      title: DIMENSION OF VECTOR SPACES
      page: 293
      pdf_page: 317
    - "no": 3
      title: DIMENSION AND CODIMENSION OF A SUBSPACE OF A VECTOR SPACE
      page: 295
      pdf_page: 319
    - "no": 4
      title: RANK OF A LINEAR MAPPING
      page: 298
      pdf_page: 322
    - "no": 5
      title: DUAL OF A VECTOR SPACE
      page: 299
      pdf_page: 323
    - "no": 6
      title: LINEAR EQUATIONS IN VECTOR SPACES
      page: 304
      pdf_page: 328
    - "no": 7
      title: TENSOR PRODUCTS OF VECTOR SPACES
      page: 306
      pdf_page: 330
    - "no": 8
      title: RANK OF AN ELEMENT OF A TENSOR PRODUCT
      page: 309
      pdf_page: 333
    - "no": 9
      title: EXTENSION OF SCALARS FOR A VECTOR SPACE
      page: 310
      pdf_page: 334
    - "no": 10
      title: MODULES OVER INTEGRAL DOMAINS
      page: 312
      pdf_page: 336
statements: 87
exercises: 39
content_sha256: 0171c78eebd776d53011027ccf963139b565db378e765a1ca629cb771adf8d2f
translated_from: content/en/alg/II/07_s7_vector_spaces.md
translation_method: google
source_content_sha256: 4fff0cdb1537b620d81d2d1d46ed26cb35c156c51e85408f9907b6d12e29297b
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 32936dc4a7fcc6fb8cbe716a2c55999a4320f437006133fcfe61167e8732e167
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 7。 ベクトル空間

### 1. 基底/ベクトル空間

#### 定理 1 {#alg-ii-s7-thm-1 .statement tag=05RI}

体 K を超えるすべてのベクトル空間は自由K-加群です。

すべてのベクトル空間が基底を認めることを証明しなければなりません。これは、次のより正確な定理から導き出されます。

#### 定理 2 {#alg-ii-s7-thm-2 .statement tag=05RJ}

体 K 上のベクトル空間 E の生成する系 S と、S に含まれる E の自由部分集合 L が与えられると、L ⊂ B ⊂ S となる E の基底 B が存在します。

定理 1 は、この主張から L = ∅ を計算して得られます。

定理 2 を証明するには、包含順に並べた S に含まれる E の自由部分集合の集合 Λ が、§ 1, no. 11 によって帰納的集合 (集合理論, III, § 2, no. 4) であることに注意します。自由な部分集合含む L の集合 M も同様であり、S に含まれています。Zorn の補題により、M は極大元 B を認め、B によって生成された E のベクトル部分空間が E に等しいことを証明するのに十分です。これは次のことからすぐに得られます。 B の定義と次の補題:

#### 補題 1 {#alg-ii-s7-lem-1 .statement tag=05RK}

(a_i)_{i \in I} を E の元の自由家族とします。 E の b \in が (a_i) によって生成された属するから部分空間 F にならない場合、a_i と b の E からなるの部分集合は空きます。

すべての $i \in I$ に対して $\mu \in K$ と $\lambda_i \in K$ を持つ関係 $\mu b + \sum_i \lambda_i a_i = 0$ があり、家族 $(\lambda_i)$ には有限台があったとします。 $\mu \neq 0$ の場合、$b = -\sum_i (\mu^{-1} \lambda_i) a_i$ となり、したがって仮定とは反対に $b \in F$ になります。したがって、$\mu = 0$ と関係は $\sum_i \lambda_i a_i = 0$ となり、仮定によってすべての $i \in I$ が $\lambda_i = 0$ になることを意味します。 よって補題。

#### 系 {#alg-ii-s7-n1-cor-1 .statement tag=05RL}

ベクトル空間 E の部分集合 B の場合、次のプロパティは同等です。
(a) BはEの基底です。
(b) B は E の最大の自由部分集合です。
(c) B は E の最小値生成する系です。
これは定理 2 の直後に続きます。

#### 例 {#alg-ii-s7-n1-exa-1 .statement tag=05RM}

A の環 A と部分体 K が与えられると、A は K 上の (右または左) ベクトル空間であるため、基底が認められます。特に、体 K のすべての拡大体は、K 上の左 (それぞれ右) ベクトル空間として基底を持ちます。
*したがって、実数の体 R は、有理数数の体 Q に対する (無限の) 基底をベクトル空間として認めます。このような R の基底はハーメル基底と呼ばれます。

#### 注意 {#alg-ii-s7-n1-rem-1 .statement tag=05RN}

体 $K$ を超える $(a_i)_{i \in I}$ of 元 of ベクトル空間 $E$ が *無料* であるためには、すべての $\kappa \in I$、$a_\kappa$ 属するが「無料」であることが必要かつ十分です。 添字 $i \neq \kappa$ の $a_i$ によって生成された $E$ の部分空間 。この条件は、どの加群 (§ 1, no. 11, *注意* 1) でも必要であることがわかっています。 *不条理な還元* によって直ちに議論され、$(a_i)$ の最小関連サブファミリーを考慮するとわかるように、補題 1 によって十分です。

### 2. 次元/ベクトル空間

#### 定理 3 {#alg-ii-s7-thm-3 .statement tag=05RO}

*同じベクトル空間* $E$ *体* $K$ のうちの 2 つの基底は *等価* です。

まず、$E$ が *無限* 基底 $B$ を許容する場合、§ 1, no. 12、系 2 から命題 23 まで、$E$ の 1 つおきの基底が等価であることに注意してください。 $B$。したがって、$E$ が $n$ 元の有限基底を持つ場合に注意を限定することができます。 0 に減らされない、$K$ 上のすべての *単次* ベクトル空間は、*単純な* $K$ モジュール (I, § 4, no. 4、定義 7) であることに注意してください。これは、その元 $\neq 0$ のそれぞれによって生成されるためです。 関係 $\mu a = (\mu \lambda)(\lambda^{-1}a)$ は、$\mu \in K$、$\lambda \in K$、$\lambda \neq 0$ です。したがって、$(a_i)_{1 \leq i \leq n}$ が $E$ の基底である場合、$E = \bigoplus_{i=1}^n Ka_i$ は同型まで、部分空間 $E_k = \bigoplus_{i=1}^\kappa Ka_i$ は $0 \leq k \leq n$ 形の *Jordan-Hölder 系列* になります。 $E$、$E_k/E_{k-1}$ は $Ka_k$ と同型です。この場合、ヨルダン ヘルダー 定理 (I, § 4, no. 7、定理 6) から定理 3 が続きます。

A proof can be given independent of the Jordan-Hölder Theorem, by showing by induction on $n$ that, if $E$ admits a basis of $n$ elements, every other basis $B'$ has *at most* $n$ elements. 命題は $n = 0$ にとって明らかです。 $n \geq 1$ の場合、$B'$ は空ではありません。それなら$a \in B'$にしましょう。 定理 2 (no. 1) までに、$B$ の部分集合 $C$ が存在し、$\{a\} \cup B$ は明らかに生成する系であるため、$\{a\} \cup C$ は $E$ と $a \notin C$ の基底になります。 $E$。 $B$ は $E$ の基底であるため、$C = B$ は不可能 (no. 1、系から定理 2) であるため、$C$ は最大でも $n - 1$ 元です。 $V$ を $C$ によって生成された部分空間および $B' - \{a\}$ によって生成された $V'$ 部分空間とします。 $V$ と $V'$ はどちらも $E$ の部分空間 $Ka$ を補足するものであるため、同型です (§ 1, no. 10、命題 13)。 $V$ が$n - 1$ 元までで基底を認めるように、$B' - \{a\}$ は帰納法の仮定までに最大 $n - 1$ 元を持ち、したがって $B'$ は最大 $n$ 元しかありません。

#### 定義 1 {#alg-ii-s7-def-1 .statement tag=05RP}

*ベクトル空間* の次元 $E$ *体* $K$、*で示される* $\dim_K E$ *または* $[E:K]$ (*または単に* $\dim E$) *は*の基底のいずれかの基数 $E$。 *もし* $M$ *が* $E$の部分集合、* $M$の*階数 *(over* $K$*)、* $\operatorname{rg} M$ *または* $\operatorname{rg}_K M$で示される場合、*はベクトルの次元部分空間/* $E$ *生成者* $M$。

$E$ が有限次元であると言うのは、$E$ が *有限長* と $\dim_K E = \operatorname{long}_K E$ の $K$ 加群であるというというに相当します。

#### 系 {#alg-ii-s7-n2-cor-1 .statement tag=05RQ}

*E の部分集合 M ごとに、M の階数は最大でも dim E に等しくなります。*

V が M によって生成された E のベクトル部分空間である場合、M、M 含む基底 B' の V (no. 1、定理 2) であり、B' は E のフリーの部分集合であるため、E の基底 B に含まれます。 (no. 1、定理 2);次に、カード(B') $\leq$ カード(B)、よって系。

定理 2 と 3 は、次の命題を直ちに暗示します。

#### 命題 1 {#alg-ii-s7-prop-1 .statement tag=05RR}

(i) *K 上の左ベクトル空間が有限次元 n であるためには、それが K_s^n と同型であることが必要かつ十分です。*

(ii) *2 つのベクトル空間 K_s^m と K_s^n が同型 (m と n 整数 $\geq 0$) であるためには、m = n であることが必要かつ十分です。*

(iii) *有限次元 n のベクトル空間 E では、すべての生成する系には少なくとも n 元があります。 E の生成する系と n 元は E の基底です。*

(iv) *有限次元 n のベクトル空間 E では、すべての空き部分集合には最大でも n 元が含まれます。 n 元を持つ自由な部分集合は E の基底です。*

#### 命題 2 {#alg-ii-s7-prop-2 .statement tag=05RS}

*(E_t)_{t \in I} を K 上のベクトル空間の家族とします。すると*

$$
\dim_K \left( \bigoplus_{t \in I} E_t \right) = \sum_{t \in I} \dim_K E_t.
$$

E_t が $E = \bigoplus_{t \in I} E_t$ の部分空間で正規に識別され、B_t が E_t ($t \in I$) の基底である場合、$B = \bigcup_{t \in I} B_t$ は E ($§ 1$、no. 11、命題 19) の基底です。 よって関係 (1) B_t はペアで互いに素なので。

#### 注意 {#alg-ii-s7-n2-rem-1 .statement tag=05RT}

(1) 例は、元の同じ数を持たない 2 つの有限基底を認める加群から与えられます ($§ 1$, 練習問題 16(c))。ただし:

#### 命題 3 {#alg-ii-s7-prop-3 .statement tag=05RU}

*A を環として、体 D に A の準同型 $\rho$ が存在するようにします。その場合、すべての自由A-加群 E に対して、E の任意の 2 つの基底が等価になります。*

スカラーの環を D ($§ 5$, no. 1) に拡張することで得られる D 上のベクトル空間 $\rho^*(E) = D \otimes_A E$ を考え、$\phi : x \mapsto 1 \otimes x$ を E の標準写像を $\rho^*(E)$ にします。 $(a_\lambda)$ が E の基底である場合、$(\phi(a_\lambda))$ は $\rho^*(E)$ の基底 ($§ 5$、no. 1、命題 4)。 定理 3 からは命題が続きます。

#### 系 {#alg-ii-s7-n2-cor-2 .statement tag=05RV}

*A が可換環 $\neq 0$ で E 自由A-加群の場合、E の任意の 2 つの基底は等価です。*

A には少なくとも 1 つの最大イデアル m (I, $§ 8$, no. 6, 定理 1) が存在し、A/m が体であるため、命題 3 のうち条件が満たされます。

#### 注意 {#alg-ii-s7-n2-rem-2 .statement tag=05RW}

(2) 自由A-加群 E が、E の任意の 2 つの基底が等能であるようなとき、A 上の E の任意の基底の基数は、E の *次元* または *階数* とも呼ばれ、$\dim_A E$ または で表されます。 $\dim E$。

(3) 自由な $A$ モジュールの任意の 2 つの基底が等能になるように $A$ を環とし、$K$ を $A$ の部分体として、$A$ をスカラーを制限することにより、*左ベクトル空間* が $K$ を超えます。すべての空き $A$ モジュール $E$ も同様に、$K$ 上の左ベクトル空間と考えることができ、§ 1, no. 13、命題 25 から次のようになります。

$$
\dim_K E = \dim_K E \cdot \dim_K A_s.
$$

(4) 章 VIII では、環満たすの例で、命題 3 の結論がわかりますが、仮定はわかりません。

### 3. 次元およびベクトル空間の部分空間の補次元

#### 命題 4 {#alg-ii-s7-prop-4 .statement tag=05RX}

*すべての部分空間 $F$ のベクトル空間 $E$ は $E$ の直因子であり、*

$$
\dim F + \dim(E/F) = \dim E.
$$

商ベクトル空間 $E/F$ は自由加群であるため、(§ 1, no. 11, 命題 21) $F$ は $E$ の直因子であることがわかります。 関係 (3) は、公式 (1) (no. 2) の特殊なケースになります。

#### 系 1 {#alg-ii-s7-prop-4-cor-1 .statement tag=05RY}

* $E, F, G$ がベクトル空間体 $K$ を超える場合、線形写像 $0 \to E \to F \to G \to 0$ 分裂の完全系列ごと。

これは、命題 4 (§ 1, no. 9) を他ので表現したものです。

#### 系 2 {#alg-ii-s7-prop-4-cor-2 .statement tag=05RZ}

*$(E_i)_{0 \leq i \leq n}$ を体 $K$ 上のベクトル空間の有限族とする。 線形写像* の完全系列が存在する場合

$$
0 \longrightarrow E_0 \xrightarrow{u_0} E_1 \xrightarrow{u_1} E_2 \longrightarrow \cdots \longrightarrow E_{n-1} \xrightarrow{u_{n-1}} E_n \xrightarrow{u_n} 0
$$

*関係*

$$
\sum_{2k+1 \leq n} \dim E_{2k+1} = \sum_{2k \leq n} \dim E_{2k}
$$

*成り立つ、または、すべての空間が有限次元である場合、*

$$
\sum_{i=1}^n (-i)^i \dim E_i = 0.
$$

$I_k = \operatorname{Im}\ u_k = \operatorname{Ker}\ u_{k+1}$を$0 \leq k \leq n-1$にしましょう。したがって、$I_{k+1}$ は $E_{k+1}/I_k$ と同型であり、したがって (公式 (3)) $\dim I_k + \dim I_{k+1} = \dim E_{k+1}$ は $0 \leq k \leq n-2$ に対して、さらに $\dim I_0 = \dim E_0$ と $I_{n-1} = E_n$、したがって $\dim I_{n-1} = \dim E_n$ と同型です。 置き換えること $\dim E_i$ は、(5) の両辺の $\dim I_k$ の写像として表現すると、各辺 $\sum_{k=0}^{n-1} \dim I_k$、よって系が得られます。

#### 系 3 {#alg-ii-s7-prop-4-cor-3 .statement tag=05S0}

*M と N が 2 つの部分空間のベクトル空間 E である場合、*

(7) $$
\dim(M + N) + \dim(M \cap N) = \dim M + \dim N.
$$

系を適用する 2 ～ 完全系列で十分です

$$ 0 \to M \cap N \to M \oplus N \to M + N \to 0 $$

(§ 1, no. 8, 命題 10) という事実を考慮すると、

$$
\dim(M \oplus N) = \dim M + \dim N
$$

(no. 2、命題 2)。

#### 系 4 {#alg-ii-s7-prop-4-cor-4 .statement tag=05S1}

*ベクトル空間 E の部分空間 F ごとに、$\dim F \leq \dim E$; E が有限次元の場合、関係 $\dim F = \dim E$ は $F = E$ と同等です。*

最初の主張は (3) から明らかです。さらに、$\dim E$ が有限である場合、関係 $\dim F = \dim E$ は (3) により $\dim(E/F) = 0$ を意味し、次元 0 簡約するのベクトル空間が 0 になることを意味します。

#### 系 5 {#alg-ii-s7-prop-4-cor-5 .statement tag=05S2}

*ベクトル空間 E がベクトル部分空間の家族 $(F_i)$ の和である場合、*

(8) $$
\dim E \leq \sum_i \dim F_i.
$$

*さらに $\dim E$ が有限である場合、(8) の 2 つの辺は、E が族 $(F_i)$ の直和である場合にのみ等しくなります。*

不等式 (8) は (3) と、E が $\bigoplus_i F_i$ の商 (§ 1, no. 7, 公式 (28)) と同型であるという事実から導かれます。 2 番目の主張は、§ 1, no. 10、系 5 ～ 命題 16 の特定のケースであり、(8) の両辺の等式は、添字の有限の数を除いて、$\dim F_i = 0$ を意味します。

#### 定義 2 {#alg-ii-s7-def-2 .statement tag=05S3}

*ベクトル空間 E が与えられると、$\operatorname{codim}_E F$ または単に $\operatorname{codim} F$ で示される E の部分空間 F の余次元 (E に関する) は、$E/F$ の次元 (E の F の任意の補充の次元に等しい)。

関係 (3) と書くことができます

(9) $$
\dim F + \operatorname{codim} F = \dim E.
$$

#### 命題 5 {#alg-ii-s7-prop-5 .statement tag=05S4}

*F, F' をベクトル空間 E の 2 つの部分空間とし、$F \subset F'$ とします。それから$\operatorname{codim}_E F' \leq \operatorname{codim}_E F \leq \dim E$。 $\operatorname{codim}_E F$ が有限の場合、関係 $\operatorname{codim}_E F' = \operatorname{codim}_E F$ は $F = F'$ を意味します。*

不等式 $\operatorname{codim}_E F \leq \dim E$ は (9) から明らかであり、$\dim E$ が有限である場合関係 $\operatorname{codim}_E F = \dim E$ は $\dim F = 0$、したがって $F = \{0\}$ を意味します。 命題の残りは次のようになります。
$$
\operatorname{codim}_E F' = \operatorname{codim}_{E/F'}(F'/F),
$$
$E/F'$ は正準的に $(E/F)/(F'/F)$ (I, § 4, no. 7, 定理 4) と同型であるためです。

#### 命題 6 {#alg-ii-s7-prop-6 .statement tag=05S5}

*M と N が 2 つの部分空間のベクトル空間 E である場合、*
$$
\operatorname{codim}(M + N) + \operatorname{codim}(M \cap N) = \operatorname{codim} M + \operatorname{codim} N.
$$
(10)
命題 4 から完全系列までの系を適用する 2 で十分です
$$
0 \to E/(M \cap N) \to (E/M) \oplus (E/N) \to E/(M + N) \to 0
$$
(§ 1, no. 7、命題 10)、no. 2、命題 2 を使用します。

E が有限次元の場合、(10) は (7) と (9) の帰結であることに注意してください。

#### 命題 7 {#alg-ii-s7-prop-7 .statement tag=05S6}

*$(F_i)$ がベクトル空間 E の部分空間の有限族である場合、*
$$
\operatorname{codim}\left(\bigcap_i F_i\right) \leq \sum_i \operatorname{codim} F_i.
$$
$F = \bigcap_i F_i$ の場合、$E/F$ は、$E/F_i$ (§ 1, no. 7, 公式 (27)) の直和の部分空間と同型です。

次元 1 (それぞれ次元 2) のベクトル空間 E のベクトル部分空間は、しばしば * ライン移行から 0* (それぞれ * 面移行から 0*) (または単に *ライン* (それぞれ次元 2) と呼ばれます)。 *平面*) 混乱が生じない場合 (cf. § 9, no. 3))、古典幾何学の言語から類推します。 E の部分空間は、余次元 1 の場合、*超平面移行から 0* (または単に *超平面*) と呼ばれます。 超平面は、集合 $\mathscr{S}$ の *最大* 元として定義することもできます。 E のベクトル部分空間は E とは *区別* されており、包含順に並べられています。 E 含む部分空間 H の部分空間と $E/H$ (I, § 4, no. 7、定理 4) の部分空間の間には 1 対 1 の対応があります。 E が次元 $\geq 1$ の場合、$\mathscr{S}$ は空ではなく、H が $\mathscr{S}$ で最大であると言うことは、$E/H$ 含む部分空間は $\{0\}$ と $E/H$ とは区別されることを意味します。これは、次のことを意味します。 $E/H$ はその元 $\neq 0$ のいずれかによって生成され、他の語では次元 1 になります。

有限次元 $n \geq 1$ のベクトル空間では、超平面は公式による部分空間 *of 次元* $n - 1$ です (3)。

#### 命題 8 {#alg-ii-s7-prop-8 .statement tag=05S7}

*体 K 上のベクトル空間 E では、すべてのベクトル部分空間 F は、含むである超平面の共通部分です。*

すべての $x \notin F$ に対して、超平面 H 含む F が存在し、含む x は存在しないことを示すだけで十分です。 仮定 $F \cap Kx = \{0\}$ により、したがって F と $Kx$ の和 M は直接です。 N を E の M を補足するものとします。この場合、E は $H = F + N$ と $Kx$ の直和となり、H は所望の性質により超平面となります。

#### 注意 {#alg-ii-s7-n3-rem-1 .statement tag=05S8}

ほとんどの特性はこの番号で証明されています。 ベクトル空間の部分空間は、次元 ($§ 2,$ no. 7, 注意 2) が定義されている自由加群の部分加群には当てはまりません。 *たとえば、可換環の理想は必ずしも基底を認めるわけではありません。なぜなら、特定の理想が主要ではない整域 $A$ があり (VII、$§ 1,$ no. 1)、そのような環のいずれか 2 つの元が線形依存 ($§ 1,$ no. 11, 注意 1).* 自由な $A$ モジュール $E$ の部分加群は、主理想によって示されているように、$E$ とは異なり、自由であり、$E$ と同じ次元を持つ可能性があります。 整域 $A$に;さらに、同じ例は、自由な $A$ モジュールの空き部分加群が必ずしも補充を許可するわけではないことを証明します。

### 4. 階数/線形写像

#### 定義 3 {#alg-ii-s7-def-3 .statement tag=05S9}

*$E, F$ を体 $K$ の 2 ベクトル空間とします。 $E$ から $F$ へのすべての線形写像 $u$ について、$F$ の部分空間 $u(E)$ の次元は $u$ のランクと呼ばれ、$\mathrm{rg}(u)$ で表されます。

$N = \mathrm{Ker}(u)$、$E/N$ は $u(E)$、よって関係と同型です
$$
\mathrm{rg}(u) = \mathrm{codim}_E(\mathrm{Ker}(u))
$$
したがって
$$
\mathrm{rg}(u) + \dim(\mathrm{Ker}(u)) = \dim E.
$$
また、公式により (3)
$$
\mathrm{rg}(u) + \dim(\mathrm{Coker}(u)) = \dim F.
$$

#### 命題 9 {#alg-ii-s7-prop-9 .statement tag=05SA}

*$E, F$ を体 $K$ と $u : E \to F$ 線形写像の 2 つのベクトル空間とします。*
(i) $\mathrm{rg}(u) \leq \inf(\dim E, \dim F)$。
(ii) *$E$ が有限次元であると仮定します。 位数の $\mathrm{rg}(u) = \dim E$ では、$u$ が単射であることが必要かつ十分です。*
(iii) *$F$ が有限次元であると仮定します。 位数の $\mathrm{rg}(u) = \dim F$ では、$u$ が全射であることが必要かつ十分です。*

これは、関係 (12) および (13) の直後に続きます。

#### 系 {#alg-ii-s7-n4-cor-1 .statement tag=05SB}

*$E$ を有限次元 $n$ のベクトル空間と $E$ の $u$ 自己準同型とします。次のプロパティは同等です:*
(a) $u$ は全単射です。
(b) $u$ は単射です。
(c) $u$ は全射的です。
(d) $u$ は右反転可能です。
(e) $u$ は反転可能なままです。
(f) $u$ は階数 $n$ のものです。

E が無限次元ベクトル空間の場合、全単射 (練習問題 9) ではない E の単射 (それぞれ全単射) 自己準同型が存在します。

K、K'を2つの体、$\sigma : K \to K'$K'上のKの*同型*、EベクトルK空間、E'ベクトルK'空間、および$u : K \to K'$$\sigma$(§ 1, no. 13)に対する*半線形*写像とする。 E' の部分空間 $u(E)$ の次元は、$u$ の *階数* とも呼ばれます。また、$u(E)$ のすべての基底は、$\sigma_*(u(E))$ の基底であるため、$u$ の階数は E の線形写像として $\sigma_*(E')$ に考慮されます。

### 5. ベクトル空間の二重

#### 定理 4 {#alg-ii-s7-thm-4 .statement tag=05SC}

双対* $E^*$ *ベクトル空間* E の *次元は * E の次元と少なくとも等しい。 *$E^*$ *が有限次元であるためには、* E *が有限次元であることが必要かつ十分であり、そのとき* $\dim E^* = \dim E$ です。

K が E のスカラーの体である場合、E は空間 $K_s^{(I)}$ と同型であり、したがって $E^*$ は $K_d^I$ (§ 2, no. 6, 命題 10) と同型です。 $K_s^{(I)}$ は $K_d^I$ の部分空間であるため、$\dim E = \mathrm{Card}(I) \leq \dim E^*$ (no. 3、系 4 ～ 命題 4)。さらに、I が有限であれば、$K_d^I = K_d^{(I)}$ (cf. 練習問題 3(d))。

#### 系 {#alg-ii-s7-n5-cor-1 .statement tag=05SD}

*ベクトル空間* E の場合、*関係* $E = \{0\}$ *および* $E^* = \{0\}$ *は同等*です。

#### 定理 5 {#alg-ii-s7-thm-5 .statement tag=05SE}

*ベクトル空間 (同じ体* K*) と線形写像* のうち 2 つの完全系列が与えられる
$$
\begin{align*}
0 &\to E' \to E \to E'' \to 0 \\
0 &\to F' \to F \to F'' \to 0
\end{align*}
$$
*そして 2 つのベクトル空間* G、H *over* K、*対応する数列*
$$
\begin{align*}
0 &\to \mathrm{Hom}(E'', G) \to \mathrm{Hom}(E, G) \to \mathrm{Hom}(E', G) \to 0 \\
0 &\to \mathrm{Hom}(H, F') \to \mathrm{Hom}(H, F) \to \mathrm{Hom}(H, F'') \to 0
\end{align*}
$$
* は正確であり、分裂* です。

これは、すべてのベクトル部分空間は直因子 (no. 3、命題 4) であり、§ 2, no. 1、命題 1 および 2 であるという事実からわかります。

#### 系 {#alg-ii-s7-n5-cor-2 .statement tag=05SF}

*完全系列*ごとに
$$
0 \longrightarrow E' \xrightarrow{u} E \xrightarrow{v} E'' \longrightarrow 0
$$
*同じ体* K * と線形写像数列* に対するベクトル空間
$$
0 \longrightarrow E''* \xrightarrow{t_v} E^* \xrightarrow{t_u} {E'}^* \longrightarrow 0
$$
* は正確であり、分裂* です。

特に、E 標準準同型 $E^*/M' \to M^*$ のすべてのベクトル部分空間 M について、$M'$ は M (§ 2, no. 4) に直交する $E^*$ の部分空間であり、*全単射*であることがわかります。

#### 定理 6 {#alg-ii-s7-thm-6 .statement tag=05SG}

*体 K を超えるすべてのベクトル空間 E について、標準写像 $c_E : E \to E^{**}$ (§ 2, no. 7) は単射法です。全単射であるためには、E が有限次元であることが必要かつ十分です。*

最初の主張と、E が有限次元の場合 $c_E$ は全単射であるという事実は、§ 2, no. 7、命題 14 の特殊なケースです。 E が無限次元であると仮定すると、$E = K_s^{(L)}$ と仮定できます。ここで、L は無限の集合であるため、$E^* = K_d^L$ となります。 $(e_\lambda)_{\lambda \in L}$ を E の標準基底とし、$(e_\lambda^*)_{\lambda \in L}$ を $E^*$ (§ 2, no. 6) の対応する座標形式の族とします。 $e_\lambda^*$ によって生成される $E^*$ のベクトル部分空間は、単なる直和 $F' = K_d^{(L)}$ であり、L が無限であるという仮説は、$F' \neq E^*$ を意味します。 次に、$E^*$ 含む $F'$ (no. 3、命題 8) の超平面 $H'$ が存在し、$E^*/H'$ が非ゼロであるため、その双対も非ゼロ (系 ～ 定理 4) であり、これは$E^{**}$の$H'$の直交$H''$(§ 2, no. 6、系から命題9)。 しかし、$H'' \cap c_E(E)$ は、E の $F'$ の直交行列の $c_E$ の下の像に含まれており、これは定義 0 だけです。したがって、$c_E(E) = E^{**}$は不可能です。

Eは通常、$E^{**}$の部分空間、$c_E$の像で*識別*されます。

E、F を 2 ベクトル空間体 K と $u : E \to F$ 線形写像とします。 定義する *標準同型*:

(1) *Im(u) = u(E) の双対 Im($^t u$) = $^t u(F^*)$ への*。

(2) *Ker(u) = $^{-1}u(0)$ の Coker($^t u$) = $E^*/^t u(F^*)$ への双対。*

(3) *Coker(u) = F/u(E) の双対 Ker($^t u$) = $^t u^{-1}(0)$.*

I = Im(u)、N = Ker(u)、C = Cok​​er(u) と書きます。 完全系列から

(14) $0 \to N \to E \xrightarrow{p} I \to 0,\quad 0 \to I \xrightarrow{j} F \to C \to 0$

転置 (系から定理 5) により、完全系列を導き出します。

(15)
$$
\begin{array}{ccccccccc}
0 & \to & I^* & \xrightarrow{^t p} & E^* & \to & N^* & \to & 0, \\
0 & \to & C^* & \to & F^* & \xrightarrow{^t j} & I^* & \to & 0.
\end{array}
$$

さらに、$u = j \circ p,\ ^t u = ^t p \circ ^t j$として;したがって、正確な配列 (15) は、$^t p$ が単射であり、$^t j$ 全射であるため、Ker($^t u$) に対する $C^*$、Im($^t u$) に対する $I^*$、および Coker($^t u$) に対する$N^*$ の正準同型を定義します。 正確に言うと、$y \in \mathrm{Im}(u)$、$z \in \mathrm{Ker}(u)$、$t \in \mathrm{Coker}(u)$、$y' \subset \mathrm{Im}(^t u)$、$z' \in \mathrm{Coker}(^t u)$、$t' \in \mathrm{Ker}(^t u)$ とします。 $y'$、$z'$、$t'$ がそれぞれ$\mathrm{Im}(u)$、$\mathrm{Ker}(u)$、$\mathrm{Coker}(u)$ で線型形式と正規に識別される場合、

(16) $u(x) = y$ となるすべての $x \in E$ に対して $\langle y, y' \rangle = \langle x, y' \rangle$;

(17) 類 mod を持つすべての $x^* \in E^*$ に $\langle z, z' \rangle = \langle z, x^* \rangle$。 $^t u(F)$ は $z'$ に等しい。

(18) 類 mod を持つすべての $s \in F$ に $\langle t, t' \rangle = \langle s, t' \rangle$。 $u(E)$ は $t$ に等しい。

特に次の結果から導き出されます。

#### 命題 10 {#alg-ii-s7-prop-10 .statement tag=05SH}

*E、F を同じ体 K 上の 2 つのベクトル空間と u : E \to F 線形写像とします。*

(i) *u が単射 (または全単射) であるためには、$^t u$ が全射 (または単射) であることが必要かつ十分です。*

(ii) $\operatorname{rg}(u)$ が有限の場合、$\operatorname{rg}(u) \leq \operatorname{rg}(^t u)$ と $\operatorname{rg}(u) = \operatorname{rg}(^t u)$。

2 番目の主張は上記と定理 4 の後に続きます。

#### 定理 7 {#alg-ii-s7-thm-7 .statement tag=05SI}

*E を体 K 上のベクトル空間、E の F 部分空間、および E* における F の直交 F' とします。*

(i) $\dim F' \geq \operatorname{codim}_E F;$ $\dim F'$ が有限であるためには、$\operatorname{codim}_E F$ が有限であることが必要かつ十分であり、その次に $\dim F' = \operatorname{codim}_E F$ です。

(ii) *E における F' の直交は F に等しい*。

(iii) *E* のすべての有限次元部分空間 G' は、E のいくつかの部分空間の直交であり、必然的に E および有限余次元の G' の直交に等しくなります。

(i) F' は双対 (E/F)* (§ 2, no. 6、系から命題 9) と同型であることがわかっているため、$\dim(E/F) = \operatorname{codim}_E F$ から定義まで主張は定理 4 から続きます。

(ii) $F_1$ を E における F' の直交とします。明らかに $F \subset F_1$ と $F_1$ の直交 $F'_1$ は F' (§ 2, no. 4) に等しい。したがって、$E/F \to E/F_1$ の標準的な線形写像 $(E/F_1)^* \to (E/F)^*$、転置は全単射です (§ 2, no. 6、系から命題 10)。次に、命題 10 から、標準写像 $E/F \to E/F_1$ は全単射であることがわかり、これは $F_1 = F$ を意味します。

(iii) G' を有限次元 $p$ の E* の部分空間とし、F を E におけるその直交とします。次に$\operatorname{codim}_E F \leq \dim G'$。 なぜなら、$(a_i^*)_{1 \leq i \leq p}$ が G' の基底である場合、F は E から $K_s^p$ までの線形写像 $x \mapsto (\langle x, a_i^* \rangle)$ の核であり、その階数は最大でも $p$ (no. 4, 命題 9)、よってであるからです。 (no. 4)。 次に、F' を E* における F の直交座標とします。 (i) から、$\dim F' \leq \dim G'$ となります。しかし一方で、明らかに $G' \subset F'$、よって $F' = G'$ (§ 2, no. 3、系 4 ～ 命題 4)。

#### 注意 {#alg-ii-s7-n5-rem-1 .statement tag=05SJ}

E* の無限次元部分空間 G' は必ずしも E の部分空間の直交ではなく、他の語では、F が E の G' の直交である場合、E* の F の直交 F' は G' とは異なる可能性があります (練習問題 20(b))。

† E と E* に適切なトポロジーを与え、これらのトポロジーに関して閉じた E と E* 部分空間のみを考慮することにより、E が無限次元 (cf. トポロジー ベクトル空間, II, § 6) の場合、E と E* の特性間に完全な対称性を再確立することが可能です。

#### 系 1 {#alg-ii-s7-thm-7-cor-1 .statement tag=05SK}

$(x_i^*)_{1 \leq i \leq p}$ を E の線型形式の有限列とし、F を E の部分空間からなるとします。

$$
\langle x, x_i^* \rangle = 0 \quad \text{for } 1 \leq i \leq p.
$$

この場合、$\operatorname{codim}_E F$ は $x_i^*$ の集合の階数に等しく、F の零である E のすべての線型形式は、$x_i^*$ の線形結合になります。次に、$\operatorname{codim}_E F \leq p$ と位数の $\operatorname{codim}_E F = p$ では、$x_i^*$ が線形独立であることが必要かつ十分です。

$x_i^*$ の線形結合の集合 $G'$ は $E^*$ の部分空間であり、F は E における $G'$ の直交であるため、定理 7 より $\operatorname{codim}_E F = \dim G'$ です。さらに、$\dim G' \leq p$ と関係$\dim G' = p$ は、$(x_i^*)$ が自由系であることを意味します (no. 2、命題 1)。したがって当然の結果です。

#### 系 2 {#alg-ii-s7-thm-7-cor-2 .statement tag=05SL}

(i) *$(x_i^*)_{1 \leq i \leq p}$ *を * E 上の線型形式の有限列とする。 *$(x_i^*)$ * が自由な系であるためには、*E の数列* $(x_i)_{1 \leq i \leq p}$ *が元の * $\langle x_i, x_j^* \rangle = \delta_{ij}$ が存在することが必要かつ十分である*(クロネッカー添字)*。

(ii) *$(x_i)_{1 \leq i \leq p}$ *を * E の元の有限列とします。 *$(x_i)$ *自由な系であるためには、* E 上に数列* $(x_i^*)_{1 \leq i \leq p}$ **の線型形式が存在することが必要かつ十分です* $\langle x_i, x_j^* \rangle = \delta_{ij}$。

$c_E$ (定理 6) によって$E^{**}$ の部分空間と同一視される E を考慮すると、(ii) は明らかに (i) から導かれます。 $G'$ を $x_i^*$ によって生成された $E^*$ の部分空間とし、F は E で直交します。 E/F と $G'$ はそれぞれ、互いの双対として正規に識別できます。ファミリ $(x_i^*)$ が自由な場合、E/F 基底 $(\dot{x}_i)$ には $(x_i^*)$ の双対があり、類 $\dot{x}_i$ のすべての代表系 $(x_i)$ は必要なプロパティを持ちます。逆に、$\langle x_i, x_j^* \rangle = \delta_{ij}$ のような系 $(x_i)$ の存在は、K に直交する $E^*$ のすべての $i$ 部分空間について、$x_i$ 含むが添字の $x_j^*$ であることを意味します。 $j \neq i$ ですが、含む $x_i^*$ はそうではありません。したがって、系 $(x_i^*)_{1 \leq i \leq p}$ は無料です。

#### 系 3 {#alg-ii-s7-thm-7-cor-3 .statement tag=05SM}

*S を、S の写像を K* に代入した右側ベクトル K 空間* $K_d^S$ の集合と V ベクトル部分空間とします。 *位数という* $\dim V \geq p$ *(p は整数)* では、 *S と p 元* $f_i$ *V* $(1 \leq i \leq p)$ *の p 元* $s_i$ が存在することが必要かつ十分です* $f_i(s_j) = \delta_{ij}$。

空間 $K_d^S$ は、$s \in S$ と $f \in K_s^S$ の$E = K_d^{(S)}$ と $f(s) = \langle e_s, f \rangle$ の双対で標準的に識別され、$(e_s)_{s \in S}$ は E の標準基底です。系 2 は、条件で十分であることを示します。逆に、$\dim V \geq p$ とすると、次元 $p$ の部分空間 $G'$ の V が存在します。 F を E の $G'$ の直交とすれば、$\dim(E/F) = p$ となります。 no. 1, 定理 2 から、E の補充 F の $e_{s_i}$ $(1 \leq i \leq p)$ 形基底となる $p$ 元 $s_i \in S$ が存在することがわかります。 (適用定理 2 (no. 1) を E の基底の空き部分集合からなるとこの空き部分集合の生成する系和集合とE)の標準基底;次に、$f_i$ を G' デュアルの基底の元と E/F の基底 、 $e_{s_i}$ mod の類のからなるとします。 F.

#### 系 4 {#alg-ii-s7-thm-7-cor-4 .statement tag=05SN}

*E をベクトル空間とし、M、N を有限余次元の E の 2 つ部分空間とします。 M'、N' が E* における M と N の直交行列である場合、E* における M ∩ N の直交行列は M' + N' です。

M (resp. N) は E (定理 7) における M' (resp. N') の直交であるため、M ∩ N は E における M' + N' の直交であり、したがって M' + N' は E* (定理 7 (iii)) における M ∩ N の直交です。

#### 系 5 {#alg-ii-s7-thm-7-cor-5 .statement tag=05SO}

*E を有限次元 n のベクトル空間とします。 次元 p の E のすべての部分空間 F について、E* における F の直交 F' は次元 n − p になります。 次元 q の E* のすべての部分空間 G' について、E の G' の直交 G は次元 n − q であり、G' は E* の G の直交です。

定理 7 は、E の *超平面* の他の特徴付けを与えます。

#### 命題 11 {#alg-ii-s7-prop-11 .statement tag=05SP}

*ベクトル空間 E の各超平面 H に対して、H = $x_0^{*-1}(0)$ となるように E に線型形式 $x_0^*$ が存在します。このような形 $x_0^*$ を考えると、E の線型形式 $x^*$ から満たす H = $x^{*-1}(0)$ に対して、 $x^* = x_0^* \alpha$ であることが必要かつ十分であり、ここで $\alpha$ はスカラー ≠ 0 です。 Eの線型形式 $x^* \neq 0$、部分空間 $x^{*-1}(0)$はEの超平面です*。

この主張は、コディメンション 1 の E の部分空間と次元 1 の E* の部分空間に対する定理 7 を表現しているだけです。

H が超平面および $x_0^*$ 線型形式である場合、H = $x^{*-1}(0)$、関係

$$
\langle x, x_0^* \rangle = 0
$$

元 $x \in H$ を特徴付けるものを *H の方程式 * と呼びます。

より一般的には、$(x_i^*)$ が E 上の線型形式のファミリーであり、F が超平面 $x_i^{*-1}(0)$ のベクトル部分空間共通部分を表す場合、関係は「すべての $i, \langle x, x_i^* \rangle = 0$ に対して」 F の元を特徴付けます。 関係

$$
\langle x, x_i^* \rangle = 0 \quad \text{for all } i
$$

形部分空間 F. 定理 7 (ii) の *系の方程式* は、E の *すべてのベクトル部分空間が方程式系で定義できるという事実を表します。

定理 7 (i) と (ii) は、*有限*余次元 $p$ の部分空間 F が $p$ 方程式の系によって定義できることを証明します

(19)
$$
\langle x, x_i^* \rangle = 0, \quad 1 \leq i \leq p,
$$

ここで、形 $x_i^*$ は *一次独立* です。逆に、系 1 から定理 7 は、$p$ 方程式 (19) の系によって定義される部分空間 F が共次元 $\leq p$ であり、$x_i^*$ が線形独立である場合に限り、共次元 $p$ であることを示しています。 F できないが式 (19) の最大 $p - 1$ の系からなるによって定義されると言うのは同じことになります。

### 6. ベクトル空間の一次方程式

#### 命題 12 {#alg-ii-s7-prop-12 .statement tag=05SQ}

E、F を 2 ベクトル空間体 K と $u : E \to F$ 線形写像とします。一次方程式の場合

$$
u(x) = y_0
$$

少なくとも 1 つの解 $x \in E$ を持つには、$y_0$ が転置写像 ${}^t u$ の核に直交することが必要かつ十分です。

$F^*$ の $u(E)$ の直交は ${}^t u^{-1}(0)$ (§ 2, no. 5, 系から命題 8) であり、したがって F の ${}^t u^{-1}(0)$ の直交は $u(E)$ (no. 5, 定理 7 (ii)) です。

スカラー線形方程式の系に対するより便利な基準を取得します。

$$
\langle x, x_i^* \rangle = \eta_i \quad (i \in I)
$$

ここで、未知の $x$ は体 K 上のベクトル空間 E の値をとり、$x_i^*$ は E の線型形式であり、K の右辺 $\eta_i$ 元です。

E の基底 $(a_\lambda)_{\lambda \in L}$ を考慮すると、系 (21) は方程式の系と等価です

$$
\sum_{\lambda \in L} \xi_\lambda \langle a_\lambda, x_i^* \rangle = \eta_i \quad (i \in I)
$$

(22) の $x = \sum_{\lambda \in L} \xi_\lambda a_\lambda$、解は、有限台の K の元の $(\xi_\lambda)$ である必要があります。

#### 定義 4 {#alg-ii-s7-def-4 .statement tag=05SR}

家族$(x_i^*)$によって生成された$E^*$の部分空間の次元は、系の階数と呼ばれます(21)。

#### 命題 13 {#alg-ii-s7-prop-13 .statement tag=05SS}

系 (21) が有限階数 r であるためには、E の線形写像 $u : x \mapsto (\langle x, x_i^* \rangle)$ が $K_s^I$ に階数 r であることが必要かつ十分です。

F' が $x_i^*$ によって生成された $E^*$ の部分空間である場合、u の核は E の F' の直交 F です。 F' が次元 r の場合、F は共次元 r であり、逆に (no. 5, 定理 7) および $\mathrm{rg}(u) = \mathrm{codim}_E F$ (no. 4, 公式 (11)) です。

#### 定理 8 {#alg-ii-s7-thm-8 .statement tag=05ST}

させて

$$
\langle x, x_i^* \rangle = \eta_i \quad (i \in I)
$$

ベクトル空間 E 対体 K 上のスカラー線形方程式の系になります。 この系が少なくとも 1 つの解を持つためには、$\sum_i x_i^* \rho_i = 0,\ \sum_i \eta_i \rho_i = 0.$ となるような有限台のスカラーのすべての族 $(\rho_i)$ について必要です。 * 系 (21) の階数が有限である場合、この条件でも十分です。

条件は明らかに必要です。それは、$F'$が家族$(x_i^*)$によって生成された$E^*$の部分空間である場合、すべての$i \in I$に対して$f(x_i^*) = \eta_i$となるような線形写像$f : F' \to K_d$が存在する、ということです。 $F'$ が有限次元 $r$ の場合、$F'$ は共次元 $r$ (no. 5, 定理 7) の $E$ の部分空間 $F$ の直交であり、 $F'$ は、$E/F$ (§ 2, no. 6、系 ～ 命題 9) の二重と識別されます。したがって、$f$ は、双対$(E/F)**$ の元です。 $E/F$ は有限次元であるため、すべての $x^* \in F'$ (no. 5, 定理 6) に対して $f(x^*) = \langle y, x^* \rangle$ となるような元 $y \in E/F$ が 1 つだけ存在します。 (21) の解は、$E/F$ の標準像が $y$ となる $x \in E$ です。

#### 注意 {#alg-ii-s7-n6-rem-1 .statement tag=05SU}

系 (21) の階数が *無限* の場合、 定理 8 の条件はもはや十分ではありません。たとえば、$x_i^*$ が空間 $E = K_s^{(I)}$ 上の * 座標形* であり、$I$ は無限 (§ 2, no. 6) であると仮定します。 $x_i^*$ は線形独立であるため、定理 8 の条件はすべての家族 $(\eta_i)$ に当てはまりますが、家族 $(\eta_i)$ が有限台を持つ場合、系 (21) は解しか持ちません。

系 (21) は、方程式の *有限の数のみ* を持ち、その階数が方程式 (no. 2, 命題 1) の数に *最大でも等しい*場合、系 (21) は常に有限階数です。同様に、$E$ が有限次元 $n$ である場合 (*有限の数 n 個の未知数* しか存在しない場合の系 (22) 対応するの場合)、その双対 $E^*$ は次元 $n$ であり、したがって系 (21) の階数は、最大でも $n$ (no. 3、系 4 ～ 命題 4) に等しくなります。このことから、次のように推測できます。

#### 系 1 {#alg-ii-s7-thm-8-cor-1 .statement tag=05SV}

*ベクトル空間におけるスカラー線形方程式系は、左側が線形独立形式である有限数の方程式で構成され、常に解を許容します。*

#### 系 2 {#alg-ii-s7-thm-8-cor-2 .statement tag=05SW}

*体 $K$ に係数を含む n 個の未知数の方程式の同次線形系 (22) が自明ではない解からなるまたは $K$ の元を認めるには、その階数 < n であることが必要かつ十分です。*

方程式の数が有限で < n の場合、これは常に当てはまります。

#### 系 3 {#alg-ii-s7-thm-8-cor-3 .statement tag=05SX}

*n 個の未知数における n 方程式の係数と右辺体 $K$、からなるをもつ線形系 (22) の場合、$K$ の元の解からなるが 1 つだけ存在するためには、関連する一次式が必要かつ十分です。 系には自明でない解* がありません (または、これと同じこと、この系の左側が *線形独立である形*)。

### 7. ベクトル空間中テンソル積

無料または射影加群に関連する §§ 3、4、および 5 の結果は、特にベクトル空間に適用され、次の特性が得られます。

#### 命題 14 {#alg-ii-s7-prop-14 .statement tag=05SY}

*与えられた完全系列*

(23)
$$
0 \to E' \to E \to E'' \to 0
$$
*体 K 上の右ベクトル空間、K 上の線形写像および左ベクトル空間 F、$\mathbf{Z}$ の線形マッピングの対応する数列*
$$
0 \to E' \otimes_K F \to E \otimes_K F \to E'' \otimes_K F \to 0
$$
* は正確であり、分裂* です。

数列 (23) 分裂のように、これは § 3, no. 7、系 5 ～ 命題 7 および § 3, no. 6、命題 5 の特殊なケースです。

命題 14 のため、$E'$ が $E$、$j : E' \to E$ 標準単射のベクトル部分空間である場合、$E' \otimes_K F$ は通常、$E \otimes_K F$ の *サブ$\mathbf{Z}$* モジュールで *識別*されます。 単射 $j \otimes 1_F$。この規約により、次のようになります。

#### 系 {#alg-ii-s7-n7-cor-1 .statement tag=05SZ}

*K を体、K 上の E 右ベクトル空間、K 上の F 左ベクトル空間、E のベクトル部分空間の族 $(M_\alpha)_{\alpha \in A}$、F のベクトル部分空間の族 $(N_\beta)_{\beta \in B}$ とします。
$$
\left( \bigcap_{\alpha \in A} M_\alpha \right) \otimes_K \left( \bigcap_{\beta \in B} N_\beta \right) = \bigcap_{(\alpha, \beta) \in A \times B} (M_\alpha \otimes_K N_\beta).
$$

特定のケースを証明するには明らかに十分です
$$
\left( \bigcap_{\alpha \in A} M_\alpha \right) \otimes_K F = \bigcap_{\alpha \in A} (M_\alpha \otimes_K F).
$$

明らかに、(25) の左辺は右辺に含まれています。 逆を証明するには、F の基底 $(f_\lambda)_{\lambda \in L}$ を考慮します。その後、$E \otimes_K F$ のすべての元は形 $\sum_{\lambda \in L} x_\lambda \otimes f_\lambda$ で一意に表現できます。ここで、$x_\lambda \in E$ (§ 3, no. 7, 系 1 ～ 命題 7); $E'$ が E のベクトル部分空間である場合、関係 $\sum_{\lambda \in L} x_\lambda \otimes f_\lambda \in E' \otimes_K F$ は、すべての $\lambda \in L$ に対して命題 14 により $x_\lambda \in E'$ と等価です。したがって、$M_\alpha \otimes_K F$ のそれぞれに対して $\sum_{\lambda \in L} x_\lambda \otimes f_\lambda$ 属するということは、すべての $\lambda \in L$ とすべての $\alpha \in A$、$x_\lambda \in M_\alpha$ について、つまりすべての $\lambda \in L$ について $x_\lambda \in \bigcap_{\alpha \in A} M_\alpha$ を意味し、(25) の右辺が左辺に含まれることが証明されます。

#### 命題 15 {#alg-ii-s7-prop-15 .statement tag=05T0}

*$(E_\lambda)_{\lambda \in L}$ が体 K を超える右ベクトル空間の家族であり、$(F_\mu)_{\mu \in M}$ が K を超える左ベクトル空間の家族である場合、標準写像*
$$
\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_K \left( \prod_{\mu \in M} F_\mu \right) \to \prod_{(\lambda, \mu) \in L \times M} (E_\lambda \otimes_K F_\mu)
$$
*(§ 3, no. 7, 公式 (22)) は単射法です。*

$F = \prod_{\mu \in M} F_\mu$と書きます。 写像 (26) は標準写像の合成です
$$
\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_K F \to \prod_{\lambda \in L} (E_\lambda \otimes_K F)
$$
そして
$$
\prod_{\lambda \in L} (E_\lambda \otimes_K F) \to \prod_{\lambda \in L} \left( \prod_{\mu \in M} (E_\lambda \otimes_K F_\mu) \right);
$$
$F$ と $E_\lambda$ は $K$ を超えるベクトル空間であるため、この簡約するから § 3, no. 7、系 3 から命題 7 となります。

命題 15 のうち条件が満たされると、テンソル積
$$
\left( \prod_{\lambda \in L} E_\lambda \right) \otimes_K \left( \prod_{\mu \in M} F_\mu \right)
$$
多くの場合、その標準像で特定されます。
$$
\prod_{\lambda, \mu} (E_\lambda \otimes_K F_\mu).
$$
この規約により、次のようになります。

#### 系 {#alg-ii-s7-n7-cor-2 .statement tag=05T1}

*$F$を$K$より左ベクトル空間とします。すべての集合 $X$、左ベクトル空間 $K_d^X \otimes_K F$ は、空間 $F^X$ の部分空間、$X$ のすべての写像の $F$、からなると識別されます。 写像 $u$ では、$u(X)$ は $F$ の有限階数になります。*

$(f_\lambda)$ が $F$ の基底である場合、$K_d^X \otimes_K F$ の元 $\sum_{\lambda \in L} v_\lambda \otimes f_\lambda$ は、(26) で写像 $x \mapsto \sum_\lambda v_\lambda(x) f_\lambda$ と識別されます。 $L$の添字$\lambda$所属から有限部分集合$H$を除く$v_\lambda = 0$として、上記写像の下の$X$の像は、有限次元の部分空間に含まれます。 $F$は添字 $\lambda \in H$の$f_\lambda$によって生成されます。逆に、$u(X)$ が $F$ の有限次元部分空間 $G$ に含まれるように、$u : X \to F$ を写像とし、$(b_i)_{1 \leq i \leq n}$ を $G$ の基底とします。すべての $x \in X$ について、$u(x) = \sum_{i=1}^n v_i(x) b_i$ と書くことができます。ここで、$v_i(x)$ は、$K$ の元でよく決まります。したがって、$n$ 写像 $v_i : X \to K$ が定義され、明らかに $u$ は元 $\sum_{i=1}^n v_i \otimes b_i$ と識別されます。

同様に、$K$ および集合 $Y$ 上の右ベクトル空間 $E$ について、$E \otimes_K K_s^Y$ は、空間 $E^Y$ の部分空間、写像 $v : Y \to E$ のからなると識別されます。 $v(Y)$は有限階数のものです。 より具体的には、すべてのフィールド $K$ について、$K_d^X \otimes_K K_s^Y$ は、$X \times Y$ から $K$ へのマッピングの空間 $K^{X \times Y}$ の部分空間で識別されます ($K$ は $(K, K)$ バイモジュールと見なされます)。要素 $\sum_i u_i \otimes v_i$ ($u_i$ は $X$ から $K$ へのマッピング、$v_i$ は $Y$ から $K$ へのマッピング) は、$X \times Y$ から $K$ へのマッピング $(x, y) \mapsto \sum_i u_i(x) v_i(y)$ と識別されます。

#### 命題 16 {#alg-ii-s7-prop-16 .statement tag=05T2}

(i) *K, L を 2 つの体、K 上の E 左ベクトル空間、L 上の F 左ベクトル空間、および G を (K, L) 双モジュールとする。次に、正準 $\mathbf{Z}$-準同型*

$$
\nu : \operatorname{Hom}_K(E, G) \otimes_L F \to \operatorname{Hom}_K(E, G \otimes_L F)
$$

(§ 4, no. 2, 公式 (7)) *は単射です。 ベクトル空間 E、F のいずれかが有限次元* の場合、それは全単射です。

(ii) *$E_1, E_2, F_1, F_2$ を 4 ベクトル空間可換体 K とします。次に、正準 K 準同型*

$$
\lambda : \operatorname{Hom}(E_1, F_1) \otimes \operatorname{Hom}(E_2, F_2) \to \operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2)
$$

(§ 4, no. 4, 公式 (21)) *は単射です。順序付けられた対 $(E_1, E_2), (E_1, F_1), (E_2, F_2)$ の 1 つが有限次元空間* で構成されている場合、それは全単射です。

主張 (i) は、§ 4, no. 2、命題 2 の特定のケースです。同様に、(ii) の 2 番目の主張は、§ 4, no. 4、命題 4 の特定のケースです。最後に、準同型 (28) が常に単射であることを確認するには、$\operatorname{Hom}(E_i, F_i)$ が次であることを観察します。 ベクトル部分空間の $F_i^{E_i}$ ($i = 1, 2$) とそれ

$$
\operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2)
$$

正規的には、空間 $(F_1 \otimes F_2)^{E_1 \times E_2}$ (II, § 3, no. 1, 命題 1) のベクトル部分空間と識別されます。これらの識別が行われ、(28) の左側が $F_1^{E_1} \otimes F_2^{E_2}$ (命題 14) の部分空間と識別されると、標準写像 (28) は制限となり、この標準写像 (26) の部分空間となり、次のことがわかります (命題 15)。後者は単射です。

#### 系 1 {#alg-ii-s7-prop-16-cor-1 .statement tag=05T3}

*E と F を 2 ベクトル空間体 K とします。 標準写像*

$$
E^* \otimes_K F \to \operatorname{Hom}_K(E, F)
$$

(§ 4, no. 2, 公式 (11)) *は単射です。 E または F が有限次元* の場合、それは全単射になります。

これは命題 16 (i) の特殊なケースです。

#### 系 2 {#alg-ii-s7-prop-16-cor-2 .statement tag=05T4}

*E を右ベクトル空間とし、F 左ベクトル空間を同じ体 K とします。 標準写像*

$$
E \otimes_K F \to \operatorname{Hom}_K(E^*, F)
$$

(§ 4, no. 2, 公式 (15)) *は単射です。 E が有限次元* の場合、それは全単射になります。

これは、§ 4, no. 2、注意 2 の特殊なケースです。

#### 注意 {#alg-ii-s7-n7-rem-1 .statement tag=05T5}

(1) K を *可換* 体、E、F を K 上の 2 つのベクトル空間、(a_\lambda) を E の基底、(b_\mu) を F の基底とします。その場合、 (a_\lambda \otimes b_\mu) はベクトル K 空間 E \otimes_K F (II, § 3, no. 7、命題 2 の系 2) の基底であるため、
$$
\dim_K(E \otimes_K F) = \dim_K E \cdot \dim_K F.
$$
(2) K を *可換* 体とし、K 上の 4 つのベクトル空間 E_1、E_2、F_1、F_2、および u:E_1 \to F_1、v:E_2 \to F_2 の 2 つの線形マッピングを考えます。それから
$$
\operatorname{rg}(u \otimes v) = \operatorname{rg}(u) \cdot \operatorname{rg}(v).
$$
$(u \otimes v)(E_1 \otimes E_2)$ が $F_1 \otimes F_2$ の $u(E_1) \otimes v(E_2)$ の正準イメージであることはすぐにわかり、したがって (命題 14) は $u(E_1) \otimes v(E_2)$ と同型です。結論は (30) から得られます。
(3) *備考* 1 と同じ仮説の下で、
$$
\dim_K(\operatorname{Hom}_K(E, F)) \geq \dim_K E \cdot \dim_K F.
$$
E が $K^{(I)}$ と同型である場合、$\operatorname{Hom}(E, F)$ は $(\operatorname{Hom}(K, F))^I$ (§ 1, no. 6、命題 6 の系 1) と同型であり、したがって $F^I$ (§ 1, no. 14) と同型です。 $F^{(I)}$ は $F^I$ と $\dim(F^{(I)}) = \operatorname{Card}(I) \cdot \dim F = \dim E \cdot \dim F$ の部分空間 (no. 2、命題 2) であるため、不等式 (32) は no. 3、系 4 から命題 4 に続きます。 同じ議論は、$\dim E$ が *有限* である場合 (32) の 2 つの辺が等しいことを示しています (cf. § 10、番号 3 と 4)。

### 8. 階数/元/テンソル積

同じフィールド K 上の右ベクトル空間を E、左ベクトル空間を F とします。すべての要素 $u \in E \otimes_K F$ には、(29) 準同型性 $u_1 \in \operatorname{Hom}_K(E^*, F)$ の下で正準的に対応します。 $u = \sum_i x_i \otimes y_i$ と $x_i \in E, y_i \in F$ の場合、要素 $u_1$ は線形マッピングです
$$
x^* \mapsto \sum_i \langle x^*, x_i \rangle y_i.
$$
一方、$E \otimes_K F$ は正準的に $F \otimes_{K^0} E$ と同一視されます。ここで、E は反対のフィールド $K^0$ 上の左ベクトル空間、F は右ベクトル空間と見なされます。したがって、次によって与えられる $u$ 準同型性 $u_2 \in \operatorname{Hom}_K(F^*, E)$ に正準的に対応します。
$$
y^* \mapsto \sum_i x_i \langle y_i, y^* \rangle;
$$
$u_1$ (それぞれ $u_2$) は、$E^*$ から $F^{**}$ (それぞれ $F^*$ から $E^{**}$) へのマッピングと見なされ、$u_2$ (それぞれ $u_1$) の *転置* にすぎません。 したがって、$u_1$ と $u_2$ の *階数* は、同じ *有限* 数 $r$、共通の次元の部分空間 $u_1(E^*)$ の F および $u_2(F^*)$ は、それぞれ正規化されています。もう一方の双対 (no. 5) と同型。 $r$ ($\operatorname{rg}(u)$と表記) は $E \otimes_K F$ の元 $u$ の *階数* であり、$u_1(E^*)$ と $u_2(F^*)$ は (それぞれ F と E の) 部分空間で $u$ に *関連付けられている* とします。

#### 命題 17 {#alg-ii-s7-prop-17 .statement tag=05T6}

あなたを $E \otimes_K F$ と $M \subset E$ と $N \subset F$ の元とし、それに関連付けられた部分空間とします。 $u$ のすべての式 $u = \sum_{i=1}^s x_i \otimes y_i$ について、$1 \leq i \leq s$ の $x_i \in E$ と $y_i \in F$ では、部分空間 $M$ (それぞれ $N$) は、によって生成された $E$ (それぞれ $F$) の部分空間に含まれます。 $x_i$ (それぞれ $y_i$)。さらに、次のプロパティは同等です。

(a) 整数 $s$ は、$u$ の階数に等しい。
(b) 家族$(x_i)_{1 \leq i \leq s}$は$M$の基底です。
(c) 家族$(y_i)_{1 \leq i \leq s}$は$N$の基底です。
(d) 家族 $(x_i)_{1 \leq i \leq s}$ と $(y_i)_{1 \leq i \leq s}$ は両方とも無料です。

(33) (または (34)) により、$N = u_1(E^*)$ (それぞれ $M = u_2(F^*)$) のそれぞれの元は、$y_i$ (それぞれ $x_i$) の線形結合になります。 よって最初の主張。 $s = r$ の場合、次元 $\leq \dim M$ (それぞれ $\leq \dim N$) と含む $M$ (それぞれ $N$) を使用して $x_i$ (それぞれ $y_i$) によって生成された部分空間がそれと同一である場合、したがって、(a) は (b) と (c) および *なおさら* (d) を意味します。逆に、条件 (b) と (c) はそれぞれ、$\mathrm{rg}(u)$ の定義によって (a) を意味します。最後に (d) が成り立つ場合、$\langle x_i, x_j^* \rangle = \delta_{ij}$ (no. 5, 系 1 ～ 定理 7) のような $E^*$ の元の族 $(x_i^*)_{1 \leq i \leq s}$ が存在するため、(33) から $(y_i)$ は の基底であることがわかります。 $N$、これで証明が完了します。

#### 系 1 {#alg-ii-s7-prop-17-cor-1 .statement tag=05T7}

u の *階数は最小の整数であるため、式* $u = \sum_{i=1}^s x_i \otimes y_i$、*どこに* $x_i \in E$ *および* $y_i \in F$ *for* $1 \leq i \leq s$ が存在します。

これは、命題 17 と no. 2、命題 1 の直後に続きます。

#### 系 2 {#alg-ii-s7-prop-17-cor-2 .statement tag=05T8}

*K を K 上の可換体、E、F 2 つのベクトル空間と、K の可換拡大体である L とします。 u を * $E \otimes_K F$ の元とし、*M と N に関連する部分空間と u' とします。 * $(E \otimes_K F)_{(L)}$ * の u の標準像 (標準的には * $E_{(L)} \otimes_L F_{(L)}$、*cf. § 5, no. 1、命題 3 と識別されます)。その場合、u' に関連付けられた * $\mathrm{rg}(u') = \mathrm{rg}(u)$ * および部分空間は、正規的に * $M_{(L)}$ * および* $N_{(L)}$ と識別されます。

$u = \sum_{i=1}^r x_i \otimes y_i$ で、ファミリー $(x_i)$ と $(y_i)$ が無料の場合、$u' = \sum_{i=1}^r (1 \otimes x_i) \otimes (1 \otimes y_i)$ とファミリー $(1 \otimes x_i)$ と $(1 \otimes y_i)$ は、それぞれ $E_{(L)}$ と $F_{(L)}$ で無料になります (§ 5, no. 1、命題 4)。

### 9. ベクトル空間のスカラーの拡大

(I, § 9, no. 1, 定理 2) を思い出してください。 体 K の準同型をゼロ以外の環 A に変換することは、必ず *単射* です。

#### 命題 18 {#alg-ii-s7-prop-18 .statement tag=05T9}

$\varphi$ を体 $K$ の準同型を環 $A$ とします。 ベクトルの $K$ スペースおよび $K$ 線形マッピングのすべての完全系列について

$$
E' \xrightarrow{u} E \xrightarrow{v} E''
$$

数列

$$
E'_{(A)} \xrightarrow{u_{(A)}} E_{(A)} \xrightarrow{v_{(A)}} E''_{(A)}
$$

正確です。

これは、§ 1, no. 4、注意 4 を考慮した、no. 7、命題 14 の特殊なケースです。

#### 系 {#alg-ii-s7-n9-cor-1 .statement tag=05TA}

$K$ 線形マッピング $f : E' \to E$、$\operatorname{Im}(f_{(A)}) = (\operatorname{Im}(f))_{(A)}$、$\operatorname{Ker}(f_{(A)}) = (\operatorname{Ker}(f))_{(A)}$、$\operatorname{Coker}(f_{(A)}) = (\operatorname{Coker}(f))_{(A)}$ ごとに、標準同型以内に。

#### 命題 19 {#alg-ii-s7-prop-19 .statement tag=05TB}

$\varphi$ を体 $K$ の単射準同型から環 $A$ とします。 $K$ を超えるすべての左ベクトル空間 $E$ について、標準写像 $\phi : E \to \varphi^*(E) = A \otimes_K E$ は単射法です。さらに、$E$ のすべてのベクトル部分空間 $E'$ について、$\varphi^*(E') = A \otimes_K E'$ は$A \otimes_K E$ の直因子サブモジュール$A$ で正規に識別され、この識別により、

$$
(A \otimes_K E') \cap \phi(E) = \phi(E').
$$

最初の主張は、§ 5, no. 1、命題 4 の特殊なケースです。 2 番目は、no. 7、命題 14 の特殊なケースです。最後に、(35) を示すには、添字 $\lambda_0$ (no. 1, 定理) に対して $a_{\lambda_0} = 1$ となるように $A$ (右側の $K$ モジュールとみなされる) 基底 $(a_\lambda)_{\lambda \in L}$ を取り込むだけで十分です。 2); $A \otimes_K E$の元は、$x_\lambda \in E$で$\sum \lambda a_\lambda \otimes x_\lambda$と一意に書くことができ、そのような元～属する～$A \otimes_K E'$については、すべての$\lambda$が$x_\lambda \in E'$であれば必要十分です。一方、$\phi(E)$の元は、$\lambda \neq \lambda_0$に対して$x_\lambda = 0$となるものです。 元 $\sum \lambda a_\lambda \otimes x_\lambda$ から属する 〜 $(A \otimes_K E') \cap \phi(E)$ に対して、$\lambda \neq \lambda_0$ と $x_{\lambda_0} \in E'$ に対して $x_\lambda = 0$、よってという結論が必要十分です。

#### 系 {#alg-ii-s7-n9-cor-2 .statement tag=05TC}

$\varphi$ を体 $K$ の単射準同型を環 $A$ とします。 $K$ 線形写像 $f : E \to F$ (ここで、$E$ と $F$ は $K$ 上の 2 つのベクトル空間である) が単射的 (それぞれ全射、零) であるためには、$f_{(A)} : E_{(A)} \to F_{(A)}$ が単射的 (それぞれ零) であることが必要かつ十分です。全射、零）。

これは、命題 19 と系から命題 18 の直後に続きます。

#### 命題 20 {#alg-ii-s7-prop-20 .statement tag=05TD}

$\rho$を体$K$の準同型を環$A$とします。 $K$ を超えるすべての左ベクトル空間 $E$ に対して、正規の右 $A$ モジュール準同型

$$
v : (E^*)_{(A)} \to (E_{(A)})^*
$$

(§ 5, no. 4) は単射です。 $E$ が有限次元の場合、それは全単射です。

2 番目の主張は、§ 5, no. 4、命題 8 から続きます。最初のものを証明するために、$(E^*)_{(A)}$ のすべての元が $\sum_i x_i^* \otimes \alpha_i$ として記述されることに注意してください。ここで、$\alpha_i \in A$ と $(x_i^*)_{1 \leq i \leq n}$ は $E^*$ の自由ファミリーです。 $(E_{(A)})^*$ 線型形式 $y^*$ には対応するがあり、すべての $x \in E$ に対して $y^*(1 \otimes x) = \sum_i \rho(\langle x, x_i^* \rangle) \alpha_i$ になります。しかし、$E$ には、$\langle x_i, x_j^* \rangle = \delta_{ij}$ (no. 5、系 2 ～ 定理 7)、よって $y^*(1 \otimes x_i) = \alpha_i$ のような族 $(x_i)_{1 \leq i \leq n}$ が存在します。したがって、関係 $y^* = 0$ は、すべての $i$ に対して $\alpha_i = 0$ を意味し、これは私たちの主張を証明します。

#### 命題 21 {#alg-ii-s7-prop-21 .statement tag=05TE}

$K$ を $K$ の体と $L$ 拡大体とします。

(i) $K$ を超えるベクトル空間 $E$ ごとに、$\dim_L(E_{(L)}) = \dim_K E$。

(ii) すべての $K$ 線形マッピング $u : E \to F$ について、$E$ と $F$ は $K$、$\operatorname{rg}(u_{(L)}) = \operatorname{rg}(u)$ 上のベクトル空間です。

$(e_i)_{i \in I}$ が $K$ を超えた $E$ の基底である場合、$(1 \otimes e_i)_{i \in I}$ は $L$ を超えた $E_{(L)}$ の基底 (§ 5, no. 1、命題 4)、よっては最初の主張; 2 番目は最初の結果に続き、$u_{(L)}(E_{(L)})$ が系から命題 18 によって正規的に $(u(E))_{(L)}$ と同一視されるという事実です。

#### 命題 22 {#alg-ii-s7-prop-22 .statement tag=05TF}

$K$を可換体、$\rho : K \to A$を単射中心準同型、$E, F$を$K$の上に2つのベクトル空間とします。それから標準準同型

$$
\omega : A \otimes_K \operatorname{Hom}(E, F) \to \operatorname{Hom}_A(E_{(A)}, F_{(A)})
$$

(§ 5, no. 3, 公式 (17)) は単射です。 $A$ または $E$ が $K$ よりも有限次元ベクトル空間である場合、それは全単射です。

これは、§ 5, no. 3、命題 7 の特別なケースです。

### 10. 加群整域を超える

#### 命題 23 {#alg-ii-s7-prop-23 .statement tag=05TG}

加群 $E$ が整域 $A$ を超えると、非フリー 元の集合 $T$ は $E$ の部分加群になります。

$x$ と $y$ が自由でない場合、$A$ には $\alpha x = 0$ と $\beta y = 0$ のように 2 つの非ゼロ元 $\alpha, \beta$ が存在します。 次に、$A$ は整数領域であるため $\alpha \beta \neq 0$ 、$A$ は可換であるため、$A$ のすべての $\lambda$ と $\mu$ に対して $\alpha \beta (\lambda x + \mu y) = 0$ となり、したがって $\lambda x + \lambda y$ は自由ではありません。

#### 注意 {#alg-ii-s7-n10-rem-1 .statement tag=05TH}

$E$ を任意の可換環 $A$ よりも加群とします。 $x$ が $E$ の非自由な元である場合、部分加群 $Ax$ のすべての元は非自由です。一方、0 の $A$ 含む因子の場合、自由ではない 2 つの和と $E$ の元は自由になる可能性があります。たとえば、$\mathbf{Z}/6\mathbf{Z}$ がそれ自体に対して加群とみなされる場合、3 と 4 は自由ではありませんが、$3 + 4 = 1$ は自由です。

命題 23 は次の定義につながります。

#### 定義 5 {#alg-ii-s7-def-5 .statement tag=05TI}

*整域 $A$ の加群 $E$ では、$E$ の捩れ部分加群は、自由ではない元* (*捩れとも呼ばれます) の $E$ からなるの部分加群です。 $E$の元*）。

$E$ がその捩れ部分加群と等しいとき (つまり、$E$ のすべての元が $A$ の元 $\neq 0$ によって消滅するとき) $E$ は *捩れ加群* と呼ばれます。 $E$ の捩れ部分加群が 0 に減らされると (つまり、$E$ のゼロ以外のすべての元が *フリー*)、$E$ は (言葉の乱用により) *ねじれのないモジュール* と呼ばれます。

自由な $A$ モジュールのすべての部分加群 (特にすべての *射影* $A$ モジュール) にはねじれがありません。 $\mathbf{Z}$ モジュール $\mathbf{Q}$ にはねじれがありません。

#### 命題 24 {#alg-ii-s7-prop-24 .statement tag=05TJ}

※$A$を整域とします。すべての $A$ モジュール $E$ について、$T(E)$ が $E$ の捩れ部分加群を表すものとします。 $f : E \to E'$ を $A$ 線形マッピング、$E$ と $E'$ を $A$ モジュールとします。*

(i) $f(T(E)) \subset T(E')$。
(ii) *$f$が単射の場合、$f(T(E)) = T(E') \cap f(E)$.*
(iii) *$f$が全射で、$\operatorname{Ker}(f) \subset T(E)$の場合、$f(T(E)) = T(E')$。*

主張 (i) と (ii) は明らかです。一方、$f$が全射で$x' \in T(E')$の場合、$x' = f(x)$、ここで$x \in E$、そして仮定までに、$f(\alpha x) = \alpha x' = 0$となるような$A$に$\alpha \neq 0$が存在します。 よって $\alpha x \in \operatorname{Ker}(f)$ そして仮定までに $A$ には $\beta(\alpha x) = 0$ となる $\beta \neq 0$ が存在します。 $\beta \alpha \neq 0$、$x \in T(E)$ のように。

#### 系 1 {#alg-ii-s7-prop-24-cor-1 .statement tag=05TK}

*すべての $A$ モジュール $E$、$E/T(E)$ にはねじれがありません。*

$f : E \to E'$ が $A$ 線形写像である場合、$f_T$ は $f$ から $T(E)$ の制限と同じグラフで写像 $T(E) \to T(E')$ を表すものとします。これで記法:

#### 系 2 {#alg-ii-s7-prop-24-cor-2 .statement tag=05TL}

*$A$ モジュールおよび $A$ 線形マッピングのすべての完全系列について*

$$
0 \longrightarrow E' \xrightarrow{f} E \xrightarrow{g} E''
$$

*数列*

$$
0 \longrightarrow T(E') \xrightarrow{f_T} T(E) \xrightarrow{g_T} T(E'')
$$

*正確です*。

$$
\operatorname{Ker}(g_T) = \operatorname{Ker}(g) \cap T(E) = f(E') \cap T(E) = f(T(E')) = \operatorname{Im}(f_T).
$$

#### 命題 25 {#alg-ii-s7-prop-25 .statement tag=05TM}

*$A$ を整域とし、$(E_i)$ を $A$ モジュールのファミリーとします。それから*

$$
T\left( \bigoplus_i E_i \right) = \bigoplus_i T(E_i).
$$

$(x_i)$ を $\bigoplus_i E_i$ の元として、すべての $i$ に対して $x_i \in T(E_i)$ となるようにします。その場合、それぞれの $x_i$ は $A$ の元 $\alpha_i \neq 0$ によって消滅し、$x_i = 0$ のときは $\alpha_i = 1$ であると想定できます。ファミリ $(x_i)$ には有限台、元 $A$ の $\alpha = \prod_i \alpha_i$ が定義され、$\neq 0$ となります。それは明らかに $\bigoplus_i x_i$ を消滅させ、したがって $\bigoplus_i T(E_i) \subset T\left(\bigoplus_i E_i\right)$ を消滅させます。 逆は明らかです。

$E$ と $F$ が 2 つの $A$ モジュールである場合、明らかに $T(E) \otimes_A F$ と $E \otimes_A T(F)$ の $T(E \otimes_A F)$ 含む標準像。しかし、例は、$T(E \otimes_A F) \neq 0$ (練習問題 31) のような *ねじれのない* $A$ モジュール $E, F$ で与えられます。

捩れ加群の *無限* 積は、必ずしも捩れ加群ではないことに注意してください。たとえば、$\mathbf{Z}$ モジュール $\prod_{n=1}^\infty (\mathbf{Z}/p^n\mathbf{Z})$ ($p$ 整数 > 1) では、座標がすべて 1 である元は自由です。

#### 命題 26 {#alg-ii-s7-prop-26 .statement tag=05TN}

*$A$ を整域、$K$ を分数の体、$E$ を $A$ モジュール、$E_{(K)} = K \otimes_A E$ ベクトル空間を演算子の環を拡張して得られた $K$ に置き換えます。 $\phi$ は、$E$ から $E_{(K)}$ への正規 $A$ 線形写像 $x \mapsto 1 \otimes x$ を表します。

(i) *$E_{(K)}$の各元は、$\lambda \in A, \lambda \neq 0$と$x \in E$の形$\lambda^{-1} \phi(x)$になります。*
(ii) *$\phi$の核は、$E$の捩れ部分加群$T(E)$です。*

(i) $E_{(K)}$ のすべての元は、$\xi_i \in K$ と $x_i \in E$ を伴う $z = \sum_{i=1}^n \xi_i \phi(x_i)$ の形です。すべての $i$ に対して、$\alpha_i \neq 0$ と $\alpha_i \xi_i \in A$ のような $\alpha_i \in A$ が存在します。 $\alpha = \prod_{i=1}^n \alpha_i$ の場合、$E_{(K)}$ のすべての $i$、よってに対して、$\alpha \neq 0$ と $\alpha \xi_i = \beta_i \in A$、

$$
z = \alpha^{-1}(\alpha z) = \alpha^{-1} \sum_{i=1}^n \beta_i \phi(x_i) = \alpha^{-1} \phi\left( \sum_{i=1}^n \beta_i x_i \right)
$$

$\phi$ は $A$ 線形であるため。

(ii) $E$ で $x \neq 0$ が空いていない場合、$A$ には $\alpha \neq 0$ が存在し、$E_{(K)}$ には $\alpha x = 0$、よって $\alpha \phi(x) = \phi(\alpha x) = 0$ が存在し、これは$\phi(x) = 0$ を意味します。 逆に、一部の $x \in E$ について、$E_{(K)}$ の $1 \otimes x = 0$ があったとします。 $x$ は $E$ の捩れ元であることがわかります。 $K$ の *単一* サブ$A$ モジュールの集合 $\mathfrak{M}$ を考慮します。これは、包含の関係の下にある権利有向集合であり、$K$ の任意の 2 つの元 $\alpha, \beta$ は $\alpha = \zeta^{-1} \xi, \beta = \zeta^{-1} \eta$ と書くことができ、$\xi, \eta, \zeta$ 属するから $A$ と $\zeta \neq 0$ であるため、$A.\alpha \subset A.\zeta^{-1}$ となります。 $A.\beta \subset A.\zeta^{-1}$。 さらに、$K$ は加群 $M \in \mathfrak{M}$ の和集合であるため、加群 $M \in \mathfrak{M}$ および標準単射 (§ 6, no. 2、*注意*) によって定義される直接系の *直接の極限* と考えることができます。 したがって、$E_{(K)}$ の標準同型、$E_{(K)} = \lim \rightarrow (M \otimes_A E)$ (§ 6, no. 3、命題 7) および関係 $1 \otimes x = 0$ 内には、

テンソル積 M ⊗_A E (集合理論, III, § 7, no. 5, 補題 1) において l ∈ M および l ⊗ x = 0 となるような M ∈ $\mathscr{P}$。さらに (置き換えることが K の単次部分加群 M' ⊃ M によって M である必要がある場合)、M = A.γ^{-1}、ここで γ ∈ A および γ ≠ 0 であると仮定できます。 ここで、写像 ξ ↦ γξ は A-加群 A 上の M の同型です。一方、標準同型 A ⊗_A E → E (§ 3, no. 4, 命題 4) 写像 ξ ⊗ x から E の元 ξx。したがって、E の写像テンソル積 ξ ⊗ x から元 (γξ)x となる同型 M ⊗_A E → E が存在します。したがって、M ⊗_A E の仮定 l ⊗ x = 0 は、γx = 0 を意味します。

#### 注意 {#alg-ii-s7-n10-rem-2 .statement tag=05TO}

α^{-1}φ(x)、β^{-1}φ(y) を E_{(K)} の 2 つの元とし、α ∈ A、β ∈ A、x ∈ E、y ∈ E、αβ ≠ 0 とします。 位数では、α^{-1}φ(x) = β^{-1}φ(y) の場合、βx − αy が E の捩れ元であることが必要かつ十分です。この関係は βφ(x) = αφ(y) と等価であり、φ(βx − αy) = 0 と書くこともできます。

#### 系 1 {#alg-ii-s7-prop-26-cor-1 .statement tag=05TP}

*E がねじりのない A 加群の場合、標準写像* φ : E → E_{(K)} *単射法*です。

K 上の E からベクトル空間 F へのすべての A-線型写像に対して、$f = \vec{f} \circ \phi$ となるような K-線型写像 $\vec{f} : E_{(K)} \to F$ が 1 つだけ存在することを思い出してください (§ 5, no. 1)。 $\vec{f}$ は $f$ に *関連付けられている* と言えます。

#### 系 2 {#alg-ii-s7-prop-26-cor-2 .statement tag=05TQ}

*f を E の A-線型写像から K 上のベクトル空間 F とします。 Ker(f) ⊂ T(E) の場合、 K-線型写像* $\vec{f}$ *f に関連付けられたものは単射*です。

カー($\vec{f}$)の元を形$\lambda^{-1}\phi(x)$に書きます。$\lambda \in A, \lambda \neq 0, x \in E$; 関係 $\vec{f}(\lambda^{-1}\phi(x)) = 0$ は F の $\lambda^{-1}\vec{f}(\phi(x)) = 0$ に相当し、したがって $f(x) = \vec{f}(\phi(x)) = 0$ に相当します。 仮定ということは、$x \in T(E)$ を意味し、したがって $\phi(x) = 0$ となり、系が証明されます。

#### 系 3 {#alg-ii-s7-prop-26-cor-3 .statement tag=05TR}

*E を A-加群とし、E の g A-線型写像を K 上のベクトル空間 F に変換し、g(E) 生成する F および Ker(g) ⊂ T(E) とします。すると、K-線型写像* $\bar{g}$ *g に関連付けられたものは、* E_{(K)} *上の F* の同型になります。

$\bar{g}$ は系 2 と仮定により単射的であり、$g(E)$ 生成する F は $\bar{g}$ が全射であることを意味します。

すべての A-加群 E について、ベクトル空間 E_{(K)} は E に *関連付けられている*と言われます。E のすべての部分集合 S について、K 上の S の *階数* (または言葉の乱用により、S の *階数*) は、S の標準像 $\phi(S)$ の階数です。 E_{(K)}、$\phi(S)$ によって生成された E_{(K)} のベクトル部分空間の K 上の他の語 (no. 2, 定義 1) 次元。

E が *ねじれのない* A-加群である場合、通常は E_{(K)} の標準像 $\phi(E)$ と識別されます。この規則では、E 含むのすべての生成する系は E_{(K)} (no. 1, 定理 2) の *基底* になります。特に：

#### 系 4 {#alg-ii-s7-prop-26-cor-4 .statement tag=05TS}

*すべての有限生成A-加群は有限階数* です。

この系の逆は必ずしも真ではないことに注意してください。たとえば、$\mathbf{Q}$ は階数 1 の $\mathbf{Z}$ モジュールですが、$\mathbf{Z}$ にわたって有限には生成されません。

(§ 5, no. 1)、すべての線形写像 $f : E \to E'$ ($E$ と $E'$ は $A$ モジュール) について、$f_{(K)}$ は $K$ 線形マッピング $1_K \otimes f : E_{(K)} \to E'_{(K)}$ を示します。

#### 命題 27 {#alg-ii-s7-prop-27 .statement tag=05TT}

*完全系列*ごとに

$$
E' \xrightarrow{f} E \xrightarrow{g} E''
$$

*$A$ 線形マッピングのうち対応する数列 $K$ 線形マッピング*

$$
E'_{(K)} \xrightarrow{f_{(K)}} E_{(K)} \xrightarrow{g_{(K)}} E''_{(K)}
$$

*正確です。*

$g_{(K)}(\lambda^{-1} \otimes x) = 0$ と $\lambda \in A, \lambda \neq 0, x \in E$ を仮定します。これは $E''_{(K)}$ の $\lambda^{-1} \otimes g(x) = 0$ に相当するため、

$$
1 \otimes g(x) = \lambda(\lambda^{-1} \otimes g(x)) = 0;
$$

命題 26 までに、$A$ には $\alpha \neq 0$ が存在し、$E''$ には $\alpha g(x) = 0$、あるいは$g(\alpha x) = 0$ が存在します。したがって、仮定までに、$\alpha x = f(x')$ となる $x' \in E'$ が存在し、したがって $\lambda^{-1} \otimes x = f_{(K)}(\alpha^{-1}\lambda^{-1} \otimes x')$ となり、命題が証明されます。

#### 系 1 {#alg-ii-s7-prop-27-cor-1 .statement tag=05TU}

*$E'$ が $E$ の部分加群である場合、$E'_{(K)}$ は正規的に $E_{(K)}$ のベクトル部分空間と、$(E/E')_{(K)}$ は $E_{(K)}/E'_{(K)}$ と識別されます。

命題を適用する 27 ～ 完全系列で十分です

$$
0 \to E' \to E \to E/E' \to 0.
$$

#### 系 2 {#alg-ii-s7-prop-27-cor-2 .statement tag=05TV}

*すべての $A$ 線形マッピング $f : E \to F$、$\operatorname{Ker}(f_{(K)}) = (\operatorname{Ker}(f))_{(K)}$、$\operatorname{Im}(f_{(K)}) = (\operatorname{Im}(f))_{(K)}$、$\operatorname{Coker}(f_{(K)}) = (\operatorname{Coker}(f))_{(K)}$ が標準同型内に収まります。特に、$f_{(K)}$ が単射法 (全射法、零) であるためには、$\operatorname{Ker}(f) \subset T(E)$ ($\operatorname{Coker}(f)$ が捩れ加群、それぞれ $\operatorname{Im}(f) \subset T(F)$) であることが必要かつ十分です。*

これは、系 1 と命題 26 から続きます。

#### 系 3 {#alg-ii-s7-prop-27-cor-3 .statement tag=05TW}

*$E$を$A$モジュール、$(x_\lambda)_{\lambda \in L}$を$E$の元のファミリーとします。 $(x_\lambda)$ が自由な家族であるためには、ベクトル $K$ 空間 $E_{(K)}$ で家族 $(1 \otimes x_\lambda)$ が自由であることが必要かつ十分です。*

ファミリ $(x_\lambda)$ 定義するは、すべての $\lambda \in L$ に対して $f(e_\lambda) = x_\lambda$ ($(e_\lambda)$ は $A^{(L)}$ の標準基底である) となるような $A$ 線形マッピング $f : A^{(L)} \to E$ で、$(x_\lambda)$ が自由であると言うのは、次のことを意味します。 $f$は単射です。 系を適用する 2 から $f$、観察するとまで$A^{(L)}$ にねじれがないこと (命題 25) だけで十分です。

### 練習問題 {#alg-ii-s7-exercises}

[§ 7 に対して練習問題](exercises/s7/)を参照してください。
