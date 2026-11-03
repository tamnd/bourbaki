---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 4
section_title: Relations between tensor products and homomorphism modules
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 267-276, 396-398
pdf_pages: 0291-0300, 0420-0422
extraction: ocr
subsections:
    - "no": 1
      title: THE ISOMORPHISMS $\operatorname{Hom}_B(E \otimes_A F, G) \to \operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G))$ AND $\operatorname{Hom}_c(E \otimes_A F, G) \to \operatorname{Hom}_A(E, \operatorname{Hom}_c(F, G))$
      page: 267
      pdf_page: 291
    - "no": 2
      title: THE HOMOMORPHISM** $E^* \otimes_A F \to \mathrm{Hom}_A(E, F)$
      page: 268
      pdf_page: 292
    - "no": 3
      title: TRACE OF AN ENDOMORPHISM
      page: 273
      pdf_page: 297
    - "no": 4
      title: THE HOMOMORPHISM $\operatorname{Hom}_c(E_1, F_1) \otimes_c \operatorname{Hom}_c(E_2, F_2) \to \operatorname{Hom}_c(E_1 \otimes_c E_2, F_1 \otimes_c F_2)$
      page: 274
      pdf_page: 298
statements: 15
exercises: 9
content_sha256: a4f5c39d284bbf35182ea7d4d6791af4a0ce4499d2c50db82c36ffe872cd748f
translated_from: content/en/alg/II/04_s4_relations_between_tensor_products_and.md
translation_method: google
source_content_sha256: 426a0db21fa5ed22b6760dc79332adbd1c61d03bf2c3a4f077a67b035b99eabb
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 678c6a0fc2d8519c37e78a8670dedf4bf57f1fed5a678f5836e57ee77b55fc12
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 4。 関係テンソル積と準同型加群の間

### 1. 同型 $\operatorname{Hom}_B(E \otimes_A F, G) \to \operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G))$ と $\operatorname{Hom}_c(E \otimes_A F, G) \to \operatorname{Hom}_A(E, \operatorname{Hom}_c(F, G))$

E を右A-加群、F 左A-加群、G を $\mathbf{Z}$ モジュール、H を写像 $f : E \times F \to G$ の $\mathbf{Z}$ モジュール、つまり $\mathbf{Z}$ 双線形および満たすとします。

(1)
$$
f(x \lambda, y) = f(x, \lambda y) \quad \text{for } x \in E, y \in F, \lambda \in A.
$$

正規の $\mathbf{Z}$ モジュール準同型が存在することが確認されています (§ 3, no. 1、命題 1)。

(2)
$$
H \to \operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, G).
$$

一方、左A-加群構造は $\operatorname{Hom}_{\mathbf{Z}}(E, G)$ に、右A-加群構造は $\operatorname{Hom}_{\mathbf{Z}}(F, G)$ (§ 3, no. 3) に定義されています。したがって、$\mathbf{Z}$ モジュール $\operatorname{Hom}_A(E, \operatorname{Hom}_{\mathbf{Z}}(F, G))$ と $\operatorname{Hom}_A(F, \operatorname{Hom}_{\mathbf{Z}}(E, G))$ を考慮することができます。 G への $E \times F$ の写像 $f$ は、E の集合への写像と F への写像の $G^F$ (*集合理論*, II, § 5, no. 2) と標準的に識別されます。後者の写像属するから $\operatorname{Hom}_A(E, \operatorname{Hom}_{\mathbf{Z}}(F, G))$ までを表現することで、$f$ が二重加法であり、条件 (1) であるという事実が正確に得られます。 よって標準同型があります

(3)
$$
H \to \operatorname{Hom}_A(E, \operatorname{Hom}_{\mathbf{Z}}(F, G))
$$
同様に標準同型が定義されています

(4)
$$
H \to \operatorname{Hom}_A(F, \operatorname{Hom}_{\mathbf{Z}}(E, G)).
$$

ここで、E と G にも左 (それぞれ右) B-加群構造があり、E の A-加群と B-加群構造が互換性があるとします。次に、$E \otimes_A F$ は正規的に左 (それぞれ右) B-加群構造 (§ 3, no. 4) を持ち、一方、$\operatorname{Hom}_B(E, G)$ は正規的に左A-加群構造 (§ 1, no. 14) を持ちます。したがって、それぞれ $\operatorname{Hom}_{\mathbf{Z}}(E \otimes_A F, G)$ と $\operatorname{Hom}_A(F, \operatorname{Hom}_{\mathbf{Z}}(E, G))$ の部分加群 (§ 2, no. 1、定理 2) である $\mathbf{Z}$ モジュール $\operatorname{Hom}_B(E \otimes_A F, G)$ と $\operatorname{Hom}_A(F, \operatorname{Hom}_B(E, G))$ を考慮することができます。 条件写像 $f \in H$ が、$\operatorname{Hom}_B(E \otimes_A F, G)$ の元と $\operatorname{Hom}_A(E, \operatorname{Hom}_B(F, G))$ の元で、同型 (2) と (4) の下で像が持つものを調べます。 2 つのケースのそれぞれで、*同じ* 条件が見つかります。

$$
f(\beta x, y) = \beta f(x, y)
$$
(それぞれ $f(x \beta, y) = f(x, y) \beta$)

$x \in E, y \in F, \beta \in B$の場合。

同様に、F と G が左 (それぞれ右) C モジュールであり、F の A-加群および C モジュール構造に互換性があると仮定します。そして、写像 $f \in H$ が、それぞれ$\mathrm{Hom}_C(E \otimes_A F, G)$ または $\mathrm{Hom}_A(E, \mathrm{Hom}_C(F, G))$ の (2) または (3) 元の下で像となるためには、満たす同じ条件であることが必要十分であり、

$$
f(x, \gamma y) = \gamma f(x, y)
$$
(それぞれ $f(x, y \gamma) = f(x, y) \gamma$)

$x \in E, y \in F, \gamma \in C$の場合。

したがって、次の結果が得られました (上記の記法で)。

#### 命題 1 {#alg-ii-s4-prop-1 .statement tag=05PP}

(a) *E を (B, A) バイモジュール、F 左A-加群および G 左B-加群とします。すべての写像 $g \in \mathrm{Hom}_B(E \otimes_A F, G)$ について、$g'$ を F の写像として、$x \in E, y \in F$ の $(g'(y))(x) = g(x \otimes y)$ によって定義される $\mathrm{Hom}_B(E, G)$ とします。 写像 $g \mapsto g'$ は同型*

(5)
$$
\beta : \mathrm{Hom}_B(E \otimes_A F, G) \to \mathrm{Hom}_A(F, \mathrm{Hom}_B(E, G)).
$$

(b) *E を右A-加群、F を (A, C) 双モジュール、G を右 C モジュールとする。すべての写像 $h \in \mathrm{Hom}_C(E \otimes_A F, G)$ について、$h'$ を E の写像とし、$x \in E, y \in F$ の $(h'(x))(y) = h(x \otimes y)$ によって定義される $\mathrm{Hom}_C(F, G)$ にします。 写像 $h \mapsto h'$ は同型*

(6)
$$
\gamma : \mathrm{Hom}_C(E \otimes_A F, G) \to \mathrm{Hom}_A(E, \mathrm{Hom}_C(F, G)).
$$

特に、B と C は、環 A の中心の部分環 $\Gamma$ であると考えることができます。次に、すべての $\Gamma$-モジュール G に対して、3 つの $\Gamma$-モジュール

$$
\mathrm{Hom}_\Gamma(E \otimes_A F, G), \quad \mathrm{Hom}_A(E, \mathrm{Hom}_\Gamma(F, G)), \quad \mathrm{Hom}_A(F, \mathrm{Hom}_\Gamma(E, G))
$$

は、$\Gamma$-*双線形* 写像の $E \times F$ の $\Gamma$ 加群と正準的に同型で、満たす (1) となる G です。より具体的には:

#### 系 {#alg-ii-s4-n1-cor-1 .statement tag=05PQ}

*C が可換環で、E、F、G の 3 つの C モジュールの場合、C モジュール*
$$
\mathrm{Hom}_C(E \otimes_C F, G), \qquad \mathrm{Hom}_C(E, \mathrm{Hom}_C(F, G)),
$$
$$
\mathrm{Hom}_C(F, \mathrm{Hom}_C(E, G)), \qquad \mathscr{L}_2(E, F; G)
$$
*正規同型です。*

### 2. 準同型** $E^* \otimes_A F \to \mathrm{Hom}_A(E, F)$

A、B を 2 つの環、E 左A-加群、F 左B-加群、G を (A, B)-*両側加群* とします。 $\mathbf{Z}$ モジュール $\mathrm{Hom}_A(E, G)$ は、標準的に、$\beta \in B$、$u \in \mathrm{Hom}_A(E, G)$、$x \in E$ に対して $(u\beta)(x) = u(x)\beta$ となる *正しい* B-*加群* 構造 (§ 1, no. 14) を持ちます。一方、$G \otimes_B F$ には標準的に *左A-加群* 構造 (§ 3, no. 4) があります。 定義する *標準的な $\mathbf{Z}$-準同型*

$$
\nu : \mathrm{Hom}_A(E, G) \otimes_B F \to \mathrm{Hom}_A(E, G \otimes_B F).
$$

この目的のために、すべての $y \in F$ とすべての $u \in \mathrm{Hom}_A(E, G)$ について、$E$ の写像 $\nu'(u, y) : x \mapsto u(x) \otimes y$ を $G \otimes_B F$ に適用することを検討します。 $\nu'(u, y)$ は $A$ 線形であり、$\nu'$ は $\mathrm{Hom}_A(E, G) \times F$ から $\mathrm{Hom}_A(E, G \otimes_B F)$ への $\mathbf{Z}$ 双線形写像であることがすぐに検証されます。さらに、$(u(x)\beta) \otimes y = u(x) \otimes (\beta y)$ については、$\beta \in B$、$\nu'(u\beta, y)$、$\nu'(u, \beta y)$ はすべて等しいです。 $\nu(u \otimes y)$ が $A$ 線形写像 $x \mapsto u(x) \otimes y$ となるような、望ましい準同型 $\nu$ の存在を結論する (§ 3, no. 1, 命題 1) とします。

$E$ が $(A, (C'_i); (D'_j))$ マルチモジュール、$F$ が $(B, (C''_h); (D''_k))$ マルチモジュール、$G$ が $(A, (C'''_1); B, (D'''_m))$ マルチモジュールである場合、写像 (7) が $((D'_j), (C''_h), (C'''_1); (C'_i), (D''_k), (D'''_m))$ マルチモジュール準同型であることがすぐに検証されます。

#### 命題 2 {#alg-ii-s4-prop-2 .statement tag=05PR}

(i) *$F$ が射影* (それぞれ *有限生成射影*) の場合、 *B-加群、標準準同型 (7) は単射* (それぞれ *全単射*) です。

(ii) *$E$ が有限生成射影 $A$ 加群である場合、標準準同型 (7) は全単射 * です。

(i) $E$ と $G$ を修正し、左の *すべての* $B$-モジュール $F$ について、次のように書きます。

$$
T(F) = \mathrm{Hom}_A(E, G) \otimes_B F, \quad T'(F) = \mathrm{Hom}_A(E, G \otimes_B F);
$$

左のすべての $B$ モジュール準同型 $u : F \to F'$ に対して、 $T(u) = 1 \otimes u$ (ここでの 1 は $\mathrm{Hom}_A(E, G)$ の恒等写像を示します)、

$$
T'(u) = \mathrm{Hom}(1_E, 1_G \otimes u);
$$

一方、$\nu$ の代わりに $\nu_F$ と書きます。次に、次の補題があります。

#### 補題 1 {#alg-ii-s4-lem-1 .statement tag=05PS}

*準同型 $u : F \to F'$、図式*ごとに

$$
\begin{array}{ccc}
T(F) & \xrightarrow{\nu_F} & T'(F) \\
\downarrow T(u) & & \downarrow T'(u) \\
T(F') & \xrightarrow{\nu_{F'}} & T'(F')
\end{array}
$$

は*可換*です。

検証は明らかです。

#### 補題 2 {#alg-ii-s4-lem-2 .statement tag=05PT}

$M, N$ を $F$ と $i : M \to F, j : N \to F$ 標準単射の 2 つの補部分加群とします。 図式

$$
\begin{array}{ccc}
T(M) \oplus T(N) & \xrightarrow{\nu_M \oplus \nu_N} & T'(M) \oplus T'(N) \\
\downarrow T(i) + T(j) & & \downarrow T'(i) + T'(j) \\
T(F) & \xrightarrow{\nu_F} & T'(F)
\end{array}
$$

は可換であり、垂直矢印は全単射です。

可換性は補題 1 から続き、もう 1 つの主張は § 1, no. 6、系 2 から命題 6、および § 3, no. 7、命題 7 から続きます。

#### 補題 3 {#alg-ii-s4-lem-3 .statement tag=05PU}

補題 2 の仮説の下では、$\nu_F$ が単射的 (それぞれ全射的) であるためには、$\nu_M$ と $\nu_N$ がそうであることが必要かつ十分です。

これは、補題 2 と § 1, no. 6、系 1 から命題 6 と続きます。

次に、補題 3 は、§ 2, no. 2、命題 4 とともに、$F$ が自由加群である場合を考慮すれば十分であることを示しています。ただし、$(b_\mu)$ が $F$ の基底である場合、$\mathrm{Hom}_A(E, G) \otimes_B F$ のすべての元は$\sum_\mu u_\mu \otimes b_\mu$ として一意に記述できます。ここで、$u_\mu \in \mathrm{Hom}_A(E, G)$ (§ 3, no. 7、系 1 ～ 命題 7)。 $\nu$ の下にあるこの元の像は、$A$ 線形マッピング $x \mapsto \sum_\mu u_\mu(x) \otimes b_\mu$ です。 できないは、すべての $x \in E$ 〜でない限り $u_\mu(x) = 0$ は、すべての $x \in E$ とすべての $\mu$ で零になります。これは、すべての $\mu$ で$u_\mu = 0$ であるというと同等です。したがって、$\nu$ は単射法です。 $F$ が有限の基底, 補題 3 を認めるとき ($F$ の基底における元の数上の帰納法によって) $\nu$ が全射であることを証明するには、次で十分です。 $F = B_s$ のときにそうしてください。しかし、この場合、(7) の 2 つの辺は $\mathrm{Hom}_A(E, G)$ (§ 3, no. 4, 命題 4) で標準的に識別され、$\nu$ が同一性になります。

(ii) $E$ が射影的で有限生成されるときの命題を示すために、今回は $F$ と $G$ を固定し、左すべての $A$ モジュール $E$ について、

$$
T(E) = \mathrm{Hom}_A(E, G) \otimes_B F, \qquad T'(E) = \mathrm{Hom}_A(E, G \otimes_B F)
$$

そして、左の $A$ モジュール準同型 $v : E \to E'$ ごとに、

$$
T(v) = \mathrm{Hom}(v, 1_G) \otimes 1_F, \qquad T'(v) = \mathrm{Hom}(v, 1_G \otimes 1_F);
$$

一方、$\nu$ の代わりに $\nu_E$ と書きます。次に、2 つの補題があります。

#### 補題 4 {#alg-ii-s4-lem-4 .statement tag=05PV}

準同型 $v : E \to E'$、図式ごとに

$$
\begin{array}{ccc}
T(E') & \xrightarrow{\nu_{E'}} & T'(E') \\
\downarrow T(v) & & \downarrow T'(v) \\
T(E) & \xrightarrow{\nu_E} & T'(E)
\end{array}
$$

可換です。

#### 補題 5 {#alg-ii-s4-lem-5 .statement tag=05PW}

$M$ と $N$ を、正規の射影の $E$ と $p : E \to M, q : E \to N$ の 2 つの補部分加群とします。 図式

$$
\begin{array}{ccc}
T(M) \oplus T(N) & \xrightarrow{\nu_M \oplus \nu_N} & T'(M) \oplus T'(N) \\
\downarrow T(p) + T(q) & & \downarrow T'(p) + T'(q) \\
T(E) & \xrightarrow{\nu_E} & T'(E)
\end{array}
$$

は可換であり、垂直矢印は全単射です。

§ 1, no. 6、系 2 ～ 命題 6、§ 2, no. 1、命題 1 と § 3, no. 7、命題 7 を考慮して、補題 1 と 2 であることが証明されます。

証明の残りは (i) と同様に処理され、$E = A_s$ の場合に還元されます。 (7) の両側は $G \otimes_B F$ で標準的に識別され、$\nu$ が同一性になります。

特に、$B = A$ と $G$ 、$(A, A)$ バイモジュール ${}_sA_d$ ($§ 3$、no. 4) を取り上げると、右側の $A$ モジュール $\mathrm{Hom}_A(E, {}_sA_d)$ は、$E$ と $({}_sA_d) \otimes_A F$ のデュアル $E^*$ になります。正規的には $F$ ($§ 3$、no. 4、命題 4) と識別されます。 準同型 (7) は正規の $\mathbf{Z}$ 準同型写像になります

$$(11)$$
$$
\theta : E^* \otimes_A F \to \mathrm{Hom}_A(E, F)
$$
そして$\theta(x^* \otimes y)$は$E$の$F$の線形写像です
$$
x \mapsto \langle x, x^* \rangle y.
$$

注意 (1)。 $§ 2$、no. 6、命題 12 で与えられる *射影* $A$ 加群の特徴付けは、次のように表すこともできます。左の $A$ 加群 $E$ が射影であるためには、 標準準同型が必要かつ十分です。
$$
\theta_E : E^* \otimes_A E \to \mathrm{Hom}_A(E, E) = \mathrm{End}_A(E)
$$
$\theta_E$ の $1_E$ 属するから像になるようにします。

#### 系 {#alg-ii-s4-n2-cor-1 .statement tag=05PX}

(i) *$F$ が射影* (または *有限生成射影*) の場合 *加群、標準準同型* (11) *は単射* (または *全単射*)。
(ii) *$E$ が有限生成射影加群のとき、標準準同型* (11) *全単射*です。

$E$ と $F$ が両方とも有限に生成される場合でも、例 $A = \mathbf{Z}, E = F = \mathbf{Z}/2\mathbf{Z}$ が示すように、$\theta$ は必ずしも全射的ではありません。 (11) の右辺はゼロではありませんが、$E^* = 0$ です。一方、$E$ が *free* である場合、例は与えられますが、(11) は単射的でも全射的でもありません (練習問題 3(b))。

E が有限の基底 $(e_i)$ を認めるとき、$\theta$ の逆同型 $\theta^{-1}$ は次のように明示的に求めることができます。 $(e_i^*)$ を $(e_i)$ (§ 2, no. 6) の双対基底とします。すべての $u \in \mathrm{Hom}(E, F)$ とすべての $x = \sum_i \xi_i e_i$ と $\xi_i \in A$、

$$
u(x) = \sum_i \xi_i u(e_i) = \sum_i \langle x, e_i^* \rangle u(e_i)
$$

したがって、$u = \sum_i \theta(e_i^* \otimes u(e_i))$、他の場合は語

$$
\theta^{-1}(u) = \sum_i e_i^* \otimes u(e_i).
$$

特に、さらに $F = E$ の場合、恒等写像 $1_E$ の $\theta_E^{-1}$ の下にある像は元 $\sum_i e_i^* \otimes e_i$ であることがわかり、したがって、これは E で考慮される基底 $(e_i)$ から *独立しています。

一方、注意一方、E が有限生成射影加群のとき、$\mathrm{End}_A(E)$ 上の *環* 構造は、$\theta_E^{-1}$ によって$E^* \otimes_A E$ に輸送できます。 E の $x, y$、$E^*$ の $x^*, y^*$、環 $\mathrm{End}_A(E)$ について、

$$
\theta_E(x^* \otimes x) \circ \theta_E(y^* \otimes y) = \theta_E((y^* \langle y, x^* \rangle) \otimes x).
$$

*注意* (2)。 E を *right* A-加群とします。 置き換えること E は (11) の $E^*$ により、正準 $\mathbf{Z}$ 準同型写像が得られます。

$$
E^{**} \otimes_A F \to \mathrm{Hom}_A(E^*, F).
$$

一方、正準 A 準同型 $c_E : E \to E^{**}$、よってには $\mathbf{Z}$ 準同型 $c_E \otimes 1_F : E \otimes_A F \to E^{**} \otimes_A F$ があります。後者を準同型 (14) で合成すると、標準的 $\mathbf{Z}$ 準同型写像が得られます。

$$
\theta' : E \otimes_A F \to \mathrm{Hom}_A(E^*, F)
$$

$\theta'(x \otimes y)$ は線形写像となる

$$
x^* \mapsto \langle x, x^* \rangle y.
$$

E * と * F が *射影 * 加群である場合、 写像 (15) は *単射 * です。 $c_E$ は単射的 (§ 2, no. 7、系 4 ～ 命題 13) であり、F が射影であるため、$\mathbf{Z}$ 準同型射影 $c_E \otimes 1_F : E \otimes_A F \to E^{**} \otimes_A F$ も単射的です (§ 3, no. 7、系 6 ～ 命題 7)。最後に、命題 2) 準同型 (14) が単射法であり、よって結論であることがわかりました。

E が *射影* かつ *有限生成* である場合、 写像 (15) は *全単射 * です。なぜなら、それを構成する 2 つの写像が全単射になるからです (上記の § 2, no. 7、系 4 から命題 13 および命題 2)。

### 3. 自己準同型の痕跡

$C$ を *可換* な環 、$E$ を $C$ モジュールとします。 $E^* \times E$ の $C$ への写像 $(x^*, x) \mapsto \langle x, x^* \rangle$ は、すべての $\gamma \in C$、$\langle \gamma x, x^* \rangle = \gamma \langle x, x^* \rangle$、$\langle x, x^* \gamma \rangle = \langle x, x^* \rangle \gamma$ について、$C$*-双線形* になります。正準 $C$*-linear* 写像を導出します

$$
\tau : E^* \otimes_C E \to C
$$

$\tau(x^* \otimes x) = \langle x, x^* \rangle$ (§ 3, no. 5) のようになります。ここで、$E$ が *有限生成された射影* $C$ モジュールであると仮定します。 no. 2 の標準同型 (11) は $C$* モジュール* 同型であるため、構造を *正規の線型形式* $\mathrm{Tr} = \tau \circ \theta_E^{-1}$ を $C$ モジュールに移送することで定義するを得ることができます。 $\mathrm{End}_C(E)$。すべての $u \in \mathrm{End}_C(E)$ について、スカラー $\mathrm{Tr}(u)$ は自己準同型 $u$ の *トレース* と呼ばれます。すべての $u \in \mathrm{End}_C(E)$ は (一般に無限の方法で) 形 $x \mapsto \sum_i \langle x, x_i^* \rangle y_i$ で書くことができます。ここで、$x_i^* \in E^*$ と $y_i \in E_i$ は、no. 2、系から命題 2 によって決まります。それから

$$
\mathrm{Tr}(u) = \sum_i \langle y_i, x_i^* \rangle \quad \text{(cf. § 10, no. 11).}
$$

定義までに、

$$
\mathrm{Tr}(u + v) = \mathrm{Tr}(u) + \mathrm{Tr}(v)
$$
$$
\mathrm{Tr}(\gamma u) = \gamma \mathrm{Tr}(u)
$$

$\mathrm{End}_C(E)$ と $\gamma \in C$ の $u, v$ について。さらに：

#### 命題 3 {#alg-ii-s4-prop-3 .statement tag=05PY}

*$C$ を可換環、$E, F$ 2 つの有限生成射影 $C$*モジュール*、および $u : E \to F$ と $v : F \to E$ 2 つの線形写像とします。それから*

$$
\mathrm{Tr}(v \circ u) = \mathrm{Tr}(u \circ v).
$$

の 2 つの写像 $(u, v) \mapsto \mathrm{Tr}(u \circ v), (u, v) \mapsto \mathrm{Tr}(v \circ u)$

$$
\mathrm{Hom}_C(E, F) \times \mathrm{Hom}_C(F, E)
$$

$C$ は $C$*-双線形* になります。したがって、$u$ が形 $x \mapsto \langle x, a^* \rangle b$ および $v$ の形 $y \mapsto \langle y, b^* \rangle a$ である場合、$a \in E, a^* \in E^*, b \in F, b^* \in F^*$ を使用して (20) を検証するだけで十分です。しかし、$v \circ u$ は写像 $x \mapsto \langle x, a^* \rangle \langle b, b^* \rangle a$ と $u \circ v$ 写像 $y \mapsto \langle y, b^* \rangle \langle a, a^* \rangle b$ になります。 公式 (17) は、(20) の両辺の値が​​ $\langle a, a^* \rangle \langle b, b^* \rangle$ に等しいことを示します。

#### 系 {#alg-ii-s4-n3-cor-1 .statement tag=05PZ}

*$u_1, \ldots, u_p$ が $E$ の自己準同型である場合、*

$$
\mathrm{Tr}(u_1 \circ u_2 \circ \cdots \circ u_p) = \mathrm{Tr}(u_i \circ u_{i+1} \circ \cdots \circ u_p \circ u_1 \circ \cdots \circ u_{i-1})
$$

*for* $1 \leq i \leq p$ (「循環置換の下でのトレースの不変性」)。

(20)を積に当てはめれば十分です

$$(u_1 \circ u_2 \circ \cdots \circ u_{i-1}) \circ (u_i \circ u_{i+1} \circ \cdots \circ u_p).$$

一方で、次のことは必ずしも真実ではないことに注意してください。

$$\operatorname{Tr}(u \circ v \circ w) = \operatorname{Tr}(u \circ w \circ v)$$

E の 3 つの自己準同型 $u, v, w$ について。

### 4. 準同型 $\operatorname{Hom}_c(E_1, F_1) \otimes_c \operatorname{Hom}_c(E_2, F_2) \to \operatorname{Hom}_c(E_1 \otimes_c E_2, F_1 \otimes_c F_2)$

C を *可換* の環と $E_1, E_2, F_1, F_2$ の 4 つの C モジュールとしましょう。 § 3, no. 5, 公式 (13) では、標準的 C モジュール準同型を定義しました

(21) $\lambda : \operatorname{Hom}(E_1, F_1) \otimes \operatorname{Hom}(E_2, F_2) \to \operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2)$。

#### 命題 4 {#alg-ii-s4-prop-4 .statement tag=05Q0}

*順序付けられた対* $(E_1, E_2), (E_1, F_1), (E_2, F_2)$ * が有限生成された射影 C 加群で構成される場合、 標準準同型* (21) * は全単射です。*

順序付けられた対 $(E_1, F_1)$ および $(E_1, E_2)$ に対して証明を実行するだけで十分であることは明らかです。

まず、注文された対 $(E_1, F_1)$ の場合を考えます。 $E_2, F_1, F_2$ を修正し、*すべての* C-モジュール $T(E) = \operatorname{Hom}(E, F_1) \otimes_c \operatorname{Hom}(E_2, F_2)$ および $T'(E) = \operatorname{Hom}(E \otimes E_2, F_1 \otimes F_2)$ と、すべての C-準同型性 $v : E \to E'$ について、

$$T(v) = \operatorname{Hom}(v, 1_{F_1}) \otimes 1_{\operatorname{Hom}(E_2, F_2)}$$

そして

$$T'(v) = \operatorname{Hom}(v \otimes 1_{E_2}, 1_{F_1 \otimes F_2}).$$

次に、*補題 4 と 5* (no. 2) (*ここで v* は $\lambda$ に置き換えられます) *有効*であり、完全に類似した方法によって証明されます。

次に、$E_2$ と $F_2$ を修正し、今度はすべての C モジュール F に対して、

$$T(F) = \operatorname{Hom}(C, F) \otimes_c \operatorname{Hom}(E_2, F_2)$$ と $T'(F) = \operatorname{Hom}(C \otimes E_2, F \otimes F_2)$、そしてすべての C 準同型性 $u : F \to F'$ に対して、

$$T(u) = \operatorname{Hom}(1_C, u) \otimes 1_{\operatorname{Hom}(E_2, F_2)}$$

そして

$$T'(u) = \operatorname{Hom}(1_C \otimes 1_{E_2}, u \otimes 1_{F_2}).$$

今度は、*補題 1 および 2* (no. 2) (*ここで、$\lambda$ は常に置き換える v*) が *有効であることがすぐに検証されます*。

そこで、$E_1 = C$と$F_1$が射影的かつ有限生成される場合、まず命題を示します。 no. 2 (補題 1 と 2 に基づく) の引数は、上記の注意、簡約すると合わせて、$F_1 = C$ の場合、証明命題になります。次に、$\operatorname{Hom}(E_1, F_1), E_1 \otimes E_2$ と $F_1 \otimes F_2$ はそれぞれ C、$E_2$、$F_2$ と識別されます (§ 3, no. 4、命題 4)。 (21) の両側

準同型 $\operatorname{Hom}_c(E_1, F_1) \otimes_c \operatorname{Hom}(E_2, F_2)$

次に、$\operatorname{Hom}(E_2, F_2)$ と後での両方で正規に識別され、$\lambda$ がアイデンティティになることが検証されます。

ここで、$F_1$ は射影的であり、有限に生成されると仮定します。 no. 2 の引数 (今回は補題 4 と 5 に依存) $E_1$ に対する簡約する証明 、$E_1 = C$ の場合、つまり最初に扱われるケースに対する有限生成射影加群です。

注文された対 $(E_1, E_2)$ についても手順は同様で、今回は適用補題 4 と 5 を 2 回実行します。詳細は読者にお任せします。

$E_1 = C^{(I)}$、$E_2 = C^{(J)}$ がフリー (有限生成かどうかに関係なく) の場合、$\operatorname{Hom}(E_1, F_1) = F_1^I$、$\operatorname{Hom}(E_2, F_2 = F_2^J$、および
$$
\operatorname{Hom}(E_1 \otimes E_2, F_1 \otimes F_2) = (F_1 \otimes F_2)^{I \times J}
$$
標準同型以内で、(21) は、§ 3, no. 7 の標準準同型 (22) の特殊なケースと同一になります。

$E_2 = C$, 標準準同型 (21) が与えられるとき、後では $\operatorname{Hom}(E_2, F_2)$ を $F_2$ で、$E_1 \otimes E_2$ を $E_1$, 標準準同型と識別します。
$$
\operatorname{Hom}(E, F) \otimes G \to \operatorname{Hom}(E, F \otimes G)
$$
任意の 3 つの $C$ モジュール $E, F, G$ の場合、これは $A = B = C$ の no. 2 の準同型 (7) にすぎません。

可換環の場合、$F = C$ 標準準同型 (22) が再び (11) (no. 2) を与えることに注意してください。

今、$F_1 = F_2 = C$; と仮定します。 $F_1 \otimes F_2$ は $C$ と同一視されるため、今回は標準準同型になります
$$
\mu : E^* \otimes F^* \to (E \otimes F)^*
$$
2 つの $C$ モジュール $E, F$ の場合。 $x^* \in E^*, y^* \in F^*$、標準準同型 (23) の下の $x^* \otimes y^*$ の像は、$E \otimes F$ では線型形式 $u$ となり、次のようになります。
$$
u(x \otimes y) = \langle x, x^* \rangle \langle y, y^* \rangle.
$$
さらに、$E_1, E_2, F_1, F_2$ が 4 つの $C$ モジュール、$f : E_1 \to E_2, g : F_1 \to F_2$ 2 つの線形写像である場合、(24) からすぐに次の結果が得られます図式
$$
\begin{array}{ccc}
E_2^* \otimes F_2^* & \xrightarrow{\mu} & (E_2 \otimes F_2)^* \\
t_f \otimes t_g \downarrow & & \downarrow t_{(f \otimes g)} \\
E_1^* \otimes F_1^* & \xrightarrow{\mu} & (E_1 \otimes F_1)^*
\end{array}
$$
は*可換*です。

#### 系 1 {#alg-ii-s4-prop-4-cor-1 .statement tag=05Q1}

*加群 E、F のいずれかが射影で有限生成される場合、標準準同型 (23) は全単射です。*

#### 系 2 {#alg-ii-s4-prop-4-cor-2 .statement tag=05Q2}

*E₁、E₂ を 2 つの有限生成射影 C 加群、E₁ の u₁ 自己準同型と E₂ の u₂ 自己準同型とします。それから*

$$
\text{Tr}(u_1 \otimes u_2) = \text{Tr}(u_1)\text{Tr}(u_2).
$$

線形性により、u₁ が形 $x_1 \mapsto \langle x_1, x_1^* \rangle y_1$ で u₂ が形 $x_2 \mapsto \langle x_2, x_2^* \rangle y_2$ である場合を考慮するだけで十分です。そうすると、$u_1 \otimes u_2$ の下の $x_1 \otimes x_2$ の像は定義になります

$$
\langle x_1, x_1^* \rangle \langle x_2, x_2^* \rangle (y_1 \otimes y_2) = \langle x_1 \otimes x_2, x_1^* \otimes x_2^* \rangle (y_1 \otimes y_2)
$$

$x_1^* \otimes x_2^*$ は、$(E_1 \otimes E_2)^*$ の元と$\mu$ で正規に識別されます。 $\langle y_1 \otimes y_2, x_1^* \otimes x_2^* \rangle = \langle y_1, x_1^* \rangle \langle y_2, x_2^* \rangle$ として、この場合は (17) から公式 (26) が続きます。

#### 注意 {#alg-ii-s4-n4-rem-1 .statement tag=05Q3}

E、F、G がいずれかの 3 つの C モジュールである場合、すぐに図式であることが検証されます。

$$
\begin{array}{ccc}
E^* \otimes F^* \otimes G^* & \xrightarrow{\mu \otimes 1} & (E \otimes F)^* \otimes G^* \\
1 \otimes \mu \downarrow & & \downarrow \mu \\
E^* \otimes (F \otimes G)^* & \xrightarrow{\mu} & (E \otimes F \otimes G)^*
\end{array}
$$

は、公式 (24) により *可換* です。

また、C モジュール E、F に仮定がなければ、正規の *同型* が存在することにも注意してください。

(28) $$(E \otimes F)^* \to \text{Hom}(E, F^*)$$
(29) $$(E \otimes F)^* \to \text{Hom}(F, E^*)$$

これは、G = C、A = B = C の no. 1 の同型 (6) と (5) です。

したがって、E × F の *双線形形式*、E から F* への *準同型、および F から E* への *準同型の間で標準的な 1 対 1 対応が定義されています。u (v) が E から F* への準同型 (または F から E*) である場合、対応する双線形形式は次によって与えられます

$$(x, y) \mapsto \langle y, u(x) \rangle \quad (\text{resp. } (x, y) \mapsto \langle x, v(y) \rangle).$$

### 練習問題 {#alg-ii-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
