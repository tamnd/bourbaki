---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 5
section_title: Extension of the ring of scalars
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 277-284, 398-399
pdf_pages: 0301-0308, 0422-0423
extraction: ocr
subsections:
    - "no": 1
      title: EXTENSION OF THE RING OF SCALARS OF A MODULE
      page: 277
      pdf_page: 301
    - "no": 2
      title: RELATIONS BETWEEN RESTRICTION AND EXTENSION OF THE RING OF SCALARS
      page: 280
      pdf_page: 304
    - "no": 3
      title: EXTENSION OF THE RING OF OPERATORS OF A HOMOMORPHISM MODULE
      page: 282
      pdf_page: 306
    - "no": 4
      title: DUAL OF A MODULE OBTAINED BY EXTENSION OF SCALARS
      page: 283
      pdf_page: 307
    - "no": 5
      title: A CRITERION FOR FINITENESS
      page: 284
      pdf_page: 308
statements: 13
exercises: 7
content_sha256: 2b42ea7e981d8095bf633ce93277c7c4f6ced3100fe52c3f3b12a14112de2e42
translated_from: content/en/alg/II/05_s5_extension_of_the_ring_of_scalars.md
translation_method: google
source_content_sha256: 77418857e92cac7b8d57a775fbe6a401b2e7ca09da87ea0dd014ebf83b887e38
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 8e359a14d4c3007c9b024a912dbdde1e15a6a7a691cdf7b6447bc1bfefebac2b
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 5。スカラーの環の拡大

### 1. 加群のスカラーの環の拡大

$A, B$ を 2 つの環と $\rho : A \to B$ 環準同型とします。この準同型 ($§ 1$, no. 13) によって定義される正しい $A$ モジュール $\rho^*(B_d)$ を検討します。この$A$モジュールには左の$B$モジュール構造、つまり$B_s$の構造もあり、$B$の$a \in A, b, b'$に対する$b'(b\rho(a)) = (b'b)\rho(a)$と同様に、$B$のこれら2つの加群構造は互換性があります($§ 1$、no. 14)。これにより、左の$A$モジュール$E$ごとに、$B$と$x \in E$の$\beta, \beta'$に対して$\beta'(\beta \otimes x) = (\beta'\beta) \otimes x$となるように、テンソル積$\rho_*(B_d) \otimes_A E$の左$B$モジュール構造を定義するにすることができます。 ($§ 3$、no. 3)。この左の$B$加群は、スカラーの環を$\rho$*によって$B$に拡張することによって$E$から導出されたものであると言われており、混乱が生じない限り、$\rho^*(E)$または$E_{(B)}$で表されます。

#### 命題 1 {#alg-ii-s5-prop-1 .statement tag=05QD}

* $A$ モジュール $\rho_*(\rho^*(E))$ への左の $A$ モジュール $E$、写像 $\phi : x \mapsto 1 \otimes x$ $E$ は $A$-線形、集合 $\phi(E)$ 生成する $B$-モジュール$\rho^*(E)$。 さらに、左のすべての $B$ モジュール $F$ と $A$ モジュール $\rho_*(F)$ への $E$ のすべての $A$ 線形写像 $f$ に対して、$\rho^*(E)$ の $B$ 線形写像 $\bar{f}$ が 1 つだけ存在します。 $F$ は、すべての $x \in E$ に対して $\bar{f}(1 \otimes x) = f(x)$ となります。*

$B$ は、$\rho$ によって $(B, A)$-bimodule とみなすことができます。次に、標準的 $\mathbf{Z}$ モジュール同型があります。

(1)
$$
\operatorname{Hom}_B(B \otimes_A E, F) \to \operatorname{Hom}_A(E, \operatorname{Hom}_B(B_s, F))
$$
$§ 4$、no. 1、命題 1 で見られるように。 しかし、左の $A$ 加群 $\operatorname{Hom}_B(B_s, F)$ は標準的に $\rho^*(F)$ と識別されます。定義により ($§ 1$, no. 14)、要素 $y \in F$ の準同型性 $\theta(y) : B_s \to F$ があり、$(\theta(y))(1) = y$;したがって、すべての $\lambda \in A$ について、$B_s$ の $F$ への準同型性 $\mu \mapsto \mu \rho(\lambda)y$ が $\rho(\lambda)y \in F$ に対応します。これは、$\operatorname{Hom}_B(B_s, F)$ ($§ 1$、no. 14) の左側の $A$ 加群構造のちょうど $\lambda \theta(y)$ です。 したがって、この識別を使用すると、(1) の逆である *標準* $\mathbf{Z}$-モジュール *同型* が得られます。

(2)
$$
\delta : \operatorname{Hom}_A(E, \rho_*(F)) \to \operatorname{Hom}_B(\rho^*(E), F)
$$
そして、定義からすぐに、$\delta(f) = \bar{f}$ であれば、すべての $x \in E$ に対して $\bar{f}(1 \otimes x) = f(x)$ が続きます。特に、写像 $\phi_E : x \mapsto 1 \otimes x$ は
(3)
$$
\phi_E = \delta^{-1}(1_{\rho^*(E)}).
$$

したがって、命題 1 が証明されます。 写像 $\phi_E : E \to \rho_*(\rho^*(E))$ は *正規* と呼ばれます。

#### 注意 {#alg-ii-s5-n1-rem-1 .statement tag=05QE}

(1) 命題 1 は、$E_{(B)}$ と $\phi_E$ の順序付けられた対からなるがユニバーサル写像問題 (集合理論, IV, § 3, no. 1) の解であることを示します。 $\Sigma$ は左B-加群構造 (射は B-線型写像) の種であり、$\alpha$ マッピングは E の A-線型写像から B-加群です。

(2) E が $(A, (C'_i); (D'_j))$ マルチモジュール、F が $(B, (C''_h); (D''_k))$ マルチモジュールの場合、同型 (2) は両側の $((D'_j, (C''_h); (C'_i), (D''_k))$ マルチモジュール構造 ($§ 1$、no. 14 および $§ 3$、no. 4) に関して線形です。

(3) E を A と $\rho : A \to A/a$ 標準準同型の両側イデアルである左A-加群、$a$ とします。 $§ 3$、no. 6、系 2 から命題 6 の記法では、A-加群 $E/aE$ は $a$ によって消滅されるため、標準的には左の $(A/a)$ モジュール構造 ($§ 1$、 no. 12); $§ 3$、no. 6、系 2 から命題 6 で定義された標準写像 $\pi : \rho^*(E) \to E/aE$ が、$(A/a)$ モジュール構造では同型であるのは明らかです。

#### 系 {#alg-ii-s5-n1-cor-1 .statement tag=05QF}

*E、E' を 2 左A-加群とします。すべての A-線型写像 $u : E \to E'$ に対して、$v = l_B \otimes u$ は可換な図式* をレンダリングする一意の B-線型写像です。

$$
\begin{array}{ccc}
E & \xrightarrow{\phi_E} & E_{(B)} \\
| & & | \\
u \downarrow & & v \downarrow \\
E' & \xrightarrow{\phi_{E'}} & E'_{(B)}
\end{array}
$$

*ここで、$\phi_E$ と $\phi_{E'}$ は標準写像です。*

A 準同型性 $\phi_{E'} \circ u : E \to E'_{(B)}$ に対して命題を適用する 1 を加えれば十分です。

上記系で定義した写像$v$を$\rho^*(u)$または$u_{(B)}$で表します。

$E''$ が 3 番目の左A-加群と $v : E' \to E''$ A-線型写像である場合、それは明らか

$$
(v \circ u)_{(B)} = v_{(B)} \circ u_{(B)}.
$$

加群の演算子の環を拡張すると *推移的* 演算になります。正確に言うと:

#### 命題 2 {#alg-ii-s5-prop-2 .statement tag=05QG}

*$\rho : A \to B,\ \sigma : B \to C$を環準同型とします。すべての左A-加群 E に対して、唯一の C-準同型写像* が存在します。

$$(4)$$
$$
\sigma^*(\rho^*(E)) \to (\sigma \circ \rho)^*(E)
$$
*写像 $1 \otimes (1 \otimes x)$ から $1 \otimes x$ はすべての $x \in E$ とこの準同型は全単射です。*

$\sigma^*(\rho^*(E))$ と $(\sigma \circ \rho)^*(E)$ の基礎となる $\mathbf{Z}$ モジュールは、それぞれ $C \otimes_B (B \otimes_A E)$ と $C \otimes_A E$ です。標準的 $\mathbf{Z}$-同型 $C \otimes_B (B \otimes_A E) \to (C \otimes_B B) \otimes_A E$ ($§ 3$、no. 8、命題 8) が存在します。これは、両側の左 C 加群構造の C- 同型でもあります。さらに、

C-モジュール $C \otimes_B B$ は、同型の写像 $\gamma \otimes \beta$ から $\gamma \sigma(\beta)$ (§ 3, no. 4、命題 4) である C モジュール $C_s$ と正規的に識別され、この同型も同様です$\rho$ で定義された $C \otimes_B B$ の右A-加群構造と、$\sigma \circ \rho$ で定義された C の右A-加群構造は同型です。したがって標準同型

$$
(C \otimes_B B) \otimes_A E \to C \otimes_A E
$$

を取得し、同型で合成します

$$
C \otimes_B (B \otimes_A E) \to (C \otimes_B B) \otimes_A E
$$

前に定義したように、目的の標準同型が得られます。

$\phi, \phi'$ と $\phi''$ が標準写像 $E \to \rho^*(E), \rho^*(E \to) \sigma^*(\rho^*(E))$ と $E \to (\sigma \circ \rho)^*(E)$ を表す場合、$\phi' \circ \phi$ は命題 2 の標準同型の下の $\phi''$ と識別されます。

#### 命題 3 {#alg-ii-s5-prop-3 .statement tag=05QH}

*A、B を 2 つの可換環、$\rho : A \to B$ 環準同型、E、E' を 2 つの A-加群とします。 B 準同型写像は 1 つだけ存在します*

$$
E_{(B)} \otimes_B E'_{(B)} \to (E \otimes_A E')_{(B)}
$$

*写像* $(1 \otimes x) \otimes (1 \otimes x')$ *to* $1 \otimes (x \otimes x')$ *for* $x \in E, x' \in E'$、*そしてこの準同型は全単射*です。

(5) の左側は $(B \otimes_A E) \otimes_B (B \otimes_A E')$ と書くことができ、A と B は可換であるため、$(E \otimes_A B) \otimes_B (B \otimes_A E')$ と識別されます。後者の積は、テンソル積 (§ 3, no. 8、命題 8)、命題 4、§ 3, no. 4、および A と B の可換性の結合性を使用して、順に $E \otimes_A (B \otimes_B B) \otimes_A E'$、$E \otimes_A (B \otimes_A E')$、$E \otimes_A (E' \otimes_A B)$、そして最後に $(E \otimes_A E') \otimes_A B$ と識別されます。 希望の同型は、連続する標準同型の合成です。

明らかに、S が E の生成する系である場合、標準写像 $E \to E_{(B)}$ の下の S の像は $E_{(B)}$ の生成する系です。特に、E が有限生成A-加群の場合、$E_{(B)}$ は有限生成された B-加群です。

#### 命題 4 {#alg-ii-s5-prop-4 .statement tag=05QI}

*E を A-加群が基底* $(a_\lambda)_{\lambda \in L}$ を認めたとします。 *if* $\phi : x \mapsto 1 \otimes x$ *E の標準写像が * $\rho^*(E)$ になると、*その後* $(\phi(a_\lambda))_{\lambda \in L}$ *は * $\rho^*(E)$ の基底になります。 *もし* $\rho$ *が単射であれば* $\phi$も同様です。

最初の主張は、§ 3, no. 7、系 1 から命題 7 に続きます。また、すべての家族について、有限台の A の元の $(\xi_\lambda)_{\lambda \in L}$、

$$
\phi \left( \sum_{\lambda \in L} \xi_\lambda a_\lambda \right) = \sum_{\lambda \in L} \rho(\xi_\lambda) \phi(a_\lambda)
$$

したがって、関係 $\phi \left( \sum_{\lambda \in L} \xi_\lambda a_\lambda \right) = 0$ は、すべての $\lambda \in L$、よってと 2 番目の主張に対する $\rho(\xi_\lambda) = 0$ と同等です。

#### 系 {#alg-ii-s5-n1-cor-2 .statement tag=05QJ}

*すべての射影 A-加群 E、B-加群* $\rho^*(E)$ * は射影です。さらに* $\rho$ *が単射であれば、Eの標準写像は* $\rho^*(E)$ *は単射です*。

仮定までに自由A-加群 M 含む E が存在し、その中で E は補充 F を認めます。 § 3, no. 7, 命題 7 から、$M_{(B)}$ が $E_{(B)}$ と $F_{(B)}$ の直和と同一視されることがすぐに続きます。 $\phi$と$\psi$は標準写像$E \to E_{(B)}$と$F \to F_{(B)}$、標準写像$M \to M_{(B)}$はちょうど$x + y \mapsto \phi(x) + \psi(y)$です。 系は、命題 4 を A-加群 M に適用した直後に続きます。

E が右A-加群のとき、同様に $\rho^*(E) = E \otimes_A \rho_*(B_s)$ と書きます。今回は B を (A, B)-bimodule として考慮し、$\rho^*(E)$ 上の右B-加群構造は、$\beta \in B' \ \beta' \in B$ と $x \in E$ に対して $(x \otimes \beta)\beta' = x \otimes (\beta\beta')$ となるようにします。この番号の結果対応するを正しく加群述べる作業は読者に委ねます。そして以下。

注意 (4)。 $\rho$ によって定義された左A-加群 $\rho_*(B_s)$ を検討し、すべての左A-加群 E について、$\mathbf{Z}$ モジュールを検討します
$$
\tilde{\rho}(E) = \operatorname{Hom}_A(\rho_*(B_s), E).
$$
$\rho_*(B_s)$ には右B-加群構造があるため、左B-加群構造は $\tilde{\rho}(E)$ (§ 1, no. 14) から導出され、$u \in \tilde{\rho}(E)$ と $b' \in B$ の場合、$b'u$ は準同型になります。 $\rho_*(B_s)$ の $b \mapsto u(bb')$ を E に変換します。さらに定義する A-線型写像を標準と呼びます
$$
\eta : \rho_*(\tilde{\rho}(E)) \to E
$$
E のすべての準同型 $u \in \tilde{\rho}(E)$ 元 $u(1)$ と関連付けられます。B は $\rho$ によって (A, B) バイモジュールと見なされるため、すべての左B-加群 F に対して、標準的 $\mathbf{Z}$ モジュール同型が存在します。
$$
\operatorname{Hom}_A(\rho_*(B_s) \otimes_B F, E) \to \operatorname{Hom}_B(F, \operatorname{Hom}_A(\rho_*(B_s), E))
$$
(§ 1, no. 1、命題1)。 左A-加群 $\rho^*(B_s) \otimes_B F$ は、§ 3, no. 4、命題 4 によって正規的に $\rho_*(F)$ と識別されるため、上記の逆である正規の $\mathbf{Z}$ モジュール同型が得られます。
$$
\operatorname{Hom}_B(F, \tilde{\rho}(E)) \to \operatorname{Hom}_A(\rho_*(F), E)
$$
これは、F のすべての B-線型写像 g を $\tilde{\rho}(E)$ に関連付け、合成写像 $\eta \circ g$ を E への $\rho_*(F)$ の A-線型写像とみなします。特に、命題 2 の仮説の下で、F を $\sigma_*(C_s)$ に置き換えると、正準が得られます。 C-同型性
$$
\tilde{\sigma}(\tilde{\rho}(E)) \to (\sigma \circ \rho)^*(E).
$$

### 2. スカラーの環の制限と拡大の間の関係

$\rho : A \to B$ を環準同型とします。 左A-加群 E ごとに、標準的 A-線型写像
$$
\phi_E : E \to \rho_*(\rho^*(E))
$$
は no. 1 で $\phi_E(x) = 1 \otimes x$ のように定義されました。ここで、左B-加群 F と命題を適用する 1 (no. 1) から準同型 $l_{\rho_*(F)} : \rho_*(F) \to \rho_*(F)$ を検討すると、B-線型写像が得られます。

$$
\psi_F : \rho^*(\rho_*(F)) \to F
$$

$\delta(l_{\rho_*(F)})$ などに等しいため、すべての $y \in F$ とすべての $\beta \in B$ について、
$\psi_F(\beta \otimes y) = \beta y$。

#### 命題 5 {#alg-ii-s5-prop-5 .statement tag=05QK}

*E を左A-加群、F を左B-加群とします。合成写像*

$$
\rho^*(E) \xrightarrow{\rho^*(\phi_E)} \rho^*(\rho_*(\rho^*(E))) \xrightarrow{\psi_{\rho^*(E)}} \rho^*(E)
$$
$$
\rho_*(E) \xrightarrow{\phi_{\rho_*(F)}} \rho_*(\rho^*(\rho_*(F))) \xrightarrow{\rho_*(\psi_F)} \rho_*(F)
$$

*はそれぞれ、$\rho^*(E)$と$\rho_*(F)$の恒等写像に等しい。*

たとえば、(12) の場合は証明となります。すべての $x \in E$、写像 $\rho^*(\phi_E)$ 写像 $1 \otimes x$ ～ 元 $1 \otimes (1 \otimes x)$ および写像 $\psi_{\rho^*(E)}$ 写像 $1 \otimes (1 \otimes x)$ ～ 元 $1 \otimes x$;結論は、形 $1 \otimes x$ 生成する B-加群 $\rho^*(E)$ の元という事実から得られます。 (13) の場合、証明はさらに簡単です。

#### 系 {#alg-ii-s5-n2-cor-1 .statement tag=05QL}

*写像 $\rho^*(\phi_E)$ と $\phi_{\rho_*(F)}^*$ は単射であり、それぞれ同一視する $\rho^*(E)$ は $\rho^*(\rho_*(\rho^*(E)))$ の直因子と$\rho_*(F)$ は $\rho_*(\rho^*(\rho_*(F)))$ の直因子となります。

これは、命題 5 と § 1, no. 9、系 2 ～ 命題 15 の帰結です。

#### 命題 6 {#alg-ii-s5-prop-6 .statement tag=05QM}

※Eを左A-加群、Fを右B-加群とします。 $\mathbf{Z}$-準同型性* は 1 つだけ存在します。

$$
\rho_*(F) \otimes_A E \to F \otimes_B \rho^*(E)
$$

*写像 $y \otimes x$ から $y \otimes (1 \otimes x)$ はすべての $x \in E$ とすべての $y \in F$ であり、この準同型は全単射です。*

定義により、(14) の右辺は $F \otimes_B (B \otimes_A E)$ となり、B は (B, A) 双加群とみなされ、§ 3, no. 8, 命題 8 で定義される標準的な $\mathbf{Z}$-同型写像 $(F \otimes_B B) \otimes_A E \to F \otimes_B (B \otimes_A E)$ が存在します。一方、§ 3, no. 4の標準同型 $F \to F \otimes_B B$、命題 4は、$\rho$で定義される両側の右A-加群構造の同型です。 よって希望の同型。

A と B が *可換* の場合、同型 (14) は *A-加群* 同型

$$
\rho_*(F) \otimes_A E \to \rho_*(F \otimes_B \rho^*(E)).
$$

### 3. 準同型加群の演算子の環の拡大

$A$ を *可換* 環、$B$ 環、$\rho : A \to B$ 環準同型および $E, F$ 2 つの $A$ モジュールとしましょう。 $B$ は ($\rho$ による) $(A, A)$ バイモジュールであり、$F$ は $(A, A)$ バイモジュールと見なすことができるため、$\mathbf{Z}$ モジュール上には $B \otimes_A F$ *2 つの* $A$ モジュール構造があり、その下にそれぞれ$a \in A,\ b \in B,\ y \in F$の場合は$a(b \otimes y) = (\rho(a)b) \otimes y$と$a(b \otimes y) = b \otimes (ay)$。このように定義された 2 つの $A$ モジュールを $G'$ と $G''$ で表すことにします。さらに、$G'$ は単なる $A$ モジュール $\rho_*(\rho^*(F))$ です。

したがって、§ 4, no. 2の標準準同型の定義、公式 (7)では、$A$によって置き換える $B$、環$B$によって$B$-モジュール$F$が、 $\rho$ による $A$ モジュールと $F$ による $G$ モジュールは、$(A, A)$ バイモジュールと見なされます。 $A$ は可換なので、次のように得られる *正準* $\mathbf{Z}$*-準同型写像* を書くことができます。

$$
(15) \quad B \otimes_A \operatorname{Hom}_A(E, F) \to \operatorname{Hom}_A(E, G'').
$$

一方 (no. 1, 公式 (2)) には、*正準* $\mathbf{Z}$*-同型* があります。

$$
(16) \quad \operatorname{Hom}_A(E, G') = \operatorname{Hom}_A(E, \rho_*(\rho^*(F))) \to \operatorname{Hom}_B(\rho^*(E), \rho^*(F)).
$$

今、$\rho(A)$ が $B$ の *中心* に含まれていると仮定します。この場合、$\rho$ は *中心* 準同型 *(または $\rho$ は定義する上の $A$*-代数* 構造とも呼ばれます) $B$、cf. III, § 1, no. 3)*。次に、$G'$ と $G''$ の $A$ 加群構造は *同一* であり、 準同型 (16) と (15) を構成すると、標準的な $\mathbf{Z}$*-準同型性* が得られます。

$$
(17) \quad \omega : B \otimes_A \operatorname{Hom}_A(E, F) \to \operatorname{Hom}_B(E_{(B)}, F_{(B)})
$$

これは、すべての $u \in \operatorname{Hom}_A(E, F)$ とすべての $b \in B$ について、

$$
(18) \quad \omega(b \otimes u) = r_b \otimes u,
$$

ここで、$r_b$ は、$B$ の $b$ による右乗法を表します。

さらに、$\omega$ が *中心* 準同型であるという仮説は、$B$ と $a \in A$ の $b,\ b'$ が $(bb')\rho(a) = b\rho(a))b'$ であることを意味します。言い換えれば、$B_d$ の *正しい* $B$ モジュール構造は、その $A$ モジュール構造と * 互換性があります。したがって、$B \otimes_A \operatorname{Hom}_A(E, F)$ で *right* $B$*-module* 構造 (§ 3, no. 4) と $F_{(B)} = B \otimes_A F$ で定義され、最後に、$F_{(B)}$ の左右の $B$-module 構造が *互換性* であるため、*right* $B$*-module* 構造も取得されます。 $\operatorname{Hom}_B(E_{(B)}, F_{(B)})$ (§ 1, no. 14)。 次に、(17) がこれらの構造に対して *正しい* $B$*-モジュール* 準同型* であることがすぐに検証されます。

#### 命題 7 {#alg-ii-s5-prop-7 .statement tag=05QN}

*$A$ を可換環、$B$ 環、$\rho : A \to B$ を中央の準同型、$E, F$ 2 つの $A$ モジュールとします。*

(i) *B が射影* (または *有限生成射影*) *A* モジュールの場合、準同型 (17) は単射* (または *全単射*) です。

(ii) *E が有限生成射影 A* 加群である場合、準同型* (17) *全単射* です。

(16) は全単射なので、§ 4, no. 2 から命題が続きます。 命題 2、標準準同型 (15) に適用されます。

### 4. 拡大のスカラーによって得られる加群の双対

A、B を 2 つの環、$\rho : A \to B$ 環準同型、E 左A-加群、E* を双対とします。 定義する正規 B-*線型* 写像とします

$$
v_E : (E^*)_{(B)} \to (E_{(B)})^*.
$$

(19) の左辺は、$\mathrm{Hom}_A(E, A) \otimes_A \rho_* (B_s)$ と書くことができます。ここで、$\mathrm{Hom}_A(E, A)$ では、A は (A, A)-bimodule と見なされます。次に、標準的な $\mathbf{Z}$ 準同型写像 ($§ 4$、no. 2、公式 (7)) が存在します。

$$
v : \mathrm{Hom}_A(E, A) \otimes_A \rho_* (B_s) \to \mathrm{Hom}_A(E, A \otimes_A \rho_* (B_s)) = \mathrm{Hom}_A(E, \rho_* (B_s))
$$

$§ 3$、no. 4、命題 4 の標準同型によって与えられる ID を使用します。一方、(19) の右辺は $\mathrm{Hom}_B(\rho_* (B_d) \otimes_A E, B_s)$ と書くことができます。 B は (B, A) 双加群であるため、正準 $\mathbf{Z}$ 同型性 ($§ 4$, no. 1, 命題 1) が存在します。

$$
\beta : \mathrm{Hom}_B(\rho_* (B_d) \otimes_A E, B_s) \to \mathrm{Hom}_A(E, \mathrm{Hom}_B(B_s, B_s))
$$

そして、$\mathrm{Hom}_B(B_s, B_s)$ は、$\rho_* (B_s)$ で A-加群として正規に識別されます (no. 1 の証明、命題 1 を参照)。これらの識別を考慮すると、準同型 $v_E$ が得られます。この準同型が次の方程式によって特徴付けられることは簡単に検証できます。

$$
\langle \xi \otimes x, v_E(x^* \otimes \eta) \rangle = \xi_p (\langle x, x^* \rangle) \eta,
$$

B の $x \in E, x^* \in E^*, \xi, \eta$ について、$v_E$ が B-*線形* であることがすぐにわかります。さらに、A-線型写像 $u : E \to F$ 図式ごとに

$$
\begin{array}{ccc}
(F^*)_{(B)} & \xrightarrow{v_F} & (F_{(B)})^* \\
(tu)_{(B)} \downarrow & & \downarrow t(u_{(B)}) \\
(E^*)_{(B)} & \xrightarrow{v_E} & (E_{(B)})^*
\end{array}
$$

可換です。

#### 命題 8 {#alg-ii-s5-prop-8 .statement tag=05QO}

*A-加群* E、$\rho_* (B_s)$ * が射影的で有限生成される場合、準同型* $v_E$ * は全単射* です。

これは上記と§ 4, no. 2、命題 2 から続きます。

特に、E が有限生成された自由A-加群であり、$(e_i)_{1 \leq i \leq n}$ が E の基底と $(e_i^*)$ 双対基底であるとします。次に、標準同型 (19) 写像基底 $(E^*)_{(B)}$ の $(e_i^* \otimes 1)$ から基底の双対基底 $E_{(B)}$ の $(1 \otimes e_i)$ となります。

### 5. 有限性の基準

#### 命題 9 {#alg-ii-s5-prop-9 .statement tag=05QP}

B を環、B の A 部分環、P を射影左A-加群とします。次に、$P_{(B)}$ が有限生成された B-加群である場合、P はそれ自体有限生成A-加群になります。

私たちは (§ 2, no. 6, 命題 12)、P の元の家族 $(a_\lambda)_{\lambda \in L}$ と双対 P* の元の家族 $(a_\lambda^*)_{\lambda \in L}$ が存在し、すべての $x \in P$ について、家族 $\langle x, a_\lambda^* \rangle$ は有限台であることを知っています。 $x = \sum_\lambda \langle x, a_\lambda^* \rangle a_\lambda$。 $P_{(B)}$ は有限生成されるため、元 $1 \otimes y_i$ によって $P_{(B)}$ が生成されるような P の元の有限族 $(y_i)_{i \in I}$ が存在します。それぞれの添字私に対して、家族 $\langle y_i, a_\lambda^* \rangle$ は有限台を持っています。したがって、$i \in I$ と $\lambda \notin H$ に対して $\langle y_i, a_\lambda^* \rangle = 0$ となるような L の有限部分集合 H が存在します。以来
$$
\langle 1 \otimes y_i, 1 d_B \otimes a_\lambda^* \rangle = \langle y_i, a_\lambda^* \rangle,
$$
したがって、$1 d_B \otimes a_\lambda^* = 0$ は $\lambda \notin H$ になります。したがって、$x \in P$ 全員にとって、
$$
\langle x, a_\lambda^* \rangle = \langle 1 \otimes x, 1_B \otimes a_\lambda^* \rangle = 0
$$
$\lambda \notin H$用。これは、A-加群 P が $a_\lambda$ によって$\lambda \in H$ のように生成されることを示しています。

### 練習問題 {#alg-ii-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
