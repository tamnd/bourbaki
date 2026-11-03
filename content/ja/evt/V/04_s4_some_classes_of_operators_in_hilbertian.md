---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: HILBERTIAN SPACES (ELEMENTARY THEORY)
section: 4
section_title: Some classes of operators in hilbertian spaces
lang: ja
source: evt-i-v
book_pages: TVS V.74-TVS V.79
pdf_pages: 0295-0318, 0332-0337
extraction: ocr
subsections:
    - "no": 1
      title: Adjoint
      page: 38
      pdf_page: 296
    - "no": 2
      title: Partially isometric linear mappings
      page: 41
      pdf_page: 299
    - "no": 3
      title: Normal endomorphisms
      page: 43
      pdf_page: 301
    - "no": 4
      title: Hermitian endomorphisms
      page: 44
      pdf_page: 302
    - "no": 5
      title: Positive endomorphisms
      page: 45
      pdf_page: 303
    - "no": 6
      title: Trace of an endomorphism
      page: 48
      pdf_page: 306
    - "no": 7
      title: Hilbert-Schmidt mappings
      page: 52
      pdf_page: 310
    - "no": 8
      title: Diagonalization of Hilbert-Schmidt mappings
      page: 55
      pdf_page: 313
    - "no": 9
      title: Trace of a quadratic form with respect to another
      page: 57
      pdf_page: 315
statements: 49
exercises: 15
content_sha256: 5201c35eba362383a445eb0b0325f77e225224707eef5095b062e853be9e526b
translated_from: content/en/evt/V/04_s4_some_classes_of_operators_in_hilbertian.md
translation_method: google
source_content_sha256: cb9870367ecf6e5e9e4940666c860653cc61494e1c8cc7bf56a66fd20a2556ef
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: f3731952df8697cc8c548fa2386c98b0aed9c30a328d3ba8dadc26299a357de4
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 4。ヒルバーシアンの演算子の一部類空間

この段落全体を通じて、$l_E$ はヒルバート空間 E の恒等写像を表します。2 つの線形写像のうち合成 $v \circ u$ は通常、$vu$ または $v.u$ で表されます。

### 1. 随伴

#### 命題 1 {#evt-v-s4-prop-1 .statement tag=080X}

— E と F を 2 ヒルベルト空間とします。 写像 $u \in \mathscr{L}(E; F)$ ごとに、次のような一意な写像 $u^* \in \mathscr{L}(F; E)$ が存在します。

$$
\langle u(x)|y \rangle_F = \langle x|u^*(y) \rangle_E
$$

すべての $x \in E$ とすべての $y \in F$ に対して。 $\mathscr{L}(E, F)$ から $\mathscr{L}(F; E)$ への写像 $u \mapsto u^*$ は、全単射、等長、半線形です (K の自己同型 $\xi \mapsto \overline{\xi}$ に関して)。

$\mathscr{S}(E, F)$ を、$E \times F$ 上のすべての連続セスキ線形形の空間とし、ノルムを付与します。

$$
\| \Phi \| = \sup_{\|x\| \leq 1, \|y\| \leq 1} |\Phi(x, y)| .
$$

私たち定義する空間 $\mathscr{S}(F, E)$ も同様です。 $\mathscr{L}(E; F)$ から $\mathscr{S}(F, E)$ までの Banach 空間同型を (V、p. 16、cor. 2) と定義しました。これは、$u \mapsto \Phi_u$ で示され、次のように特徴付けられます。

$$
\Phi_u(y, x) = \langle y|u(x) \rangle_F \quad (x \in E, \ y \in F) .
$$

同様の方法で、$\mathscr{L}(F, E)$ から $\mathscr{S}(E, F)$ に定義する同型を加えます。最後に、$\mathscr{S}(F, E)$ から $\mathscr{S}(E, F)$ まで、定義する写像 $\Phi \mapsto \Phi^*$ となります。

$$
\Phi^*(x, y) = \overline{\Phi(y, x)} \quad (x \in E, \ y \in F) .
$$

この写像は全単射、半線形、等長です。しかし、公式 (1) は $\Phi_{u^*} = (\Phi_u)^*$ と変換されるため、命題となります。

#### 定義 1 {#evt-v-s4-def-1 .statement tag=080Y}

— E と F を 2 ヒルベルト空間とします。すべての連続線形写像 $u : E \to F$ について、公式 (1) で定義される F から E までの連続線形写像は u の随伴物と呼ばれ、$u^*$ で表されます。

我々は持っています

$$
\begin{align*}
(u + v)^* &= u^* + v^* \\
(\lambda u)^* &= \overline{\lambda} u^* \\
(u^*)^* &= u \\
(1_E)^* &= 1_E \\
(wu)^* &= u^* w^* ;
\end{align*}
$$

これらすべての公式、$u$、$v$ 属するから $\mathscr{L}(E; F)$ では、$\lambda$ は K に、$w$ は $\mathscr{L}(F; G)$ で、G はヒルバーシアン空間です。 公式 (5) と (6) は、$u \mapsto u^*$ が半線形であることを意味します。 公式 (8) は明らかです。 (7) を証明するには、(1) の 2 つの要素のうち共役を取り、$\langle u^*(y)|x\rangle = \langle y|u(x)\rangle$ が得られます。これにより、$u$ が $u^*$ の随伴であることが証明されます。最後に、(9) の記法により、すべての$z \in G$ が得られます。

$$
\langle w(u(x))|z\rangle = \langle u(x)|w^*(z)\rangle = \langle x|u^*(w^*(z))\rangle ,
$$

したがって、$u^*w^*$ は $wu$ の随伴物です。

$u : E \to F$ を全単射で連続的な線形写像とします。この場合、それは共連続でもあります (I、p. 19、cor. 1)。 (8) と (9) から、$u^*$ は全単射かつ共連続であり、

(10)
$$
(u^{-1})^* = (u^*)^{-1} .
$$

#### 命題 2 {#evt-v-s4-prop-2 .statement tag=080Z}

*$u \in \mathscr{L}(E ; F)$ ごとに、*

(11)
$$
\|u^*u\| = \|uu^*\| = \|u\|^2 = \|u^*\|^2 .
$$

プロップにより。 1、$\|u^*\| = \|u\|$、したがって $\|u^*u\| \leq \|u^*\|\cdot\|u\| \leq \|u\|^2$。一方で、

$$
\|u\|^2 = \sup_{\|x\| \leq 1} \|u(x)\|^2 = \sup_{\|x\| \leq 1} \langle u(x)|u(x)\rangle = \sup_{\|x\| \leq 1} \langle x|u^*u(x)\rangle \leq \|u^*u\| ,
$$

したがって $\|u^*u\| = \|u\|^2$ です。 置き換えること $u$ を $u^*$ により、$\|uu^*\| = \|u^*\|^2$ が得られるため、$\|u\| = \|u^*\|$ 以降 (11) が続きます。

$E_1, ..., E_n$ と $F_1, ..., F_n$ をヒルベルト空間とし、1 と $n$ の間のすべての整数 $i$ について、$u_i$ を $E_i$ から $F_i$ まで連続する線形写像とします。それから

(12)
$$
(u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n)^* = u_1^* \hat{\otimes}_2 ... \hat{\otimes}_2 u_n^* .
$$

$v$ を連続線形写像 $u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n$ とします。

$$
E = E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n \quad \text{into} \quad F = F_1 \hat{\otimes}_2 ... \hat{\otimes}_2 F_n
$$

そして$w$は$F$から$E$までの連続した線形写像$u_1^* \hat{\otimes}_2 ... \hat{\otimes}_2 u_n^*$です。 $x \in E$ と $y \in F$ に対して等式 $\langle y|v(x)\rangle = \langle w(y)|x\rangle$ を証明するだけで十分です。線形性と連続性により、$x$と$y$が次の形を持つ場合を簡約するとします。

$$
x = x_1 \otimes ... \otimes x_n , \quad y = y_1 \otimes ... \otimes y_n
$$

$1 \leq i \leq n$ には $x_i \in E_i$ と $y_i \in F_i$ が付きます。 テンソル積 (V, p. 27, 公式 (6)) のスカラー 積の定義から、次のようになります。

$$
\langle y|v(x)\rangle = \prod_{i=1}^n \langle y_i|u_i(x_i)\rangle = \prod_{i=1}^n \langle u_i^*(y_i)|x_i\rangle = \langle w(y)|x\rangle .
$$

これは私たちの主張を証明します。

$E$ と $F$ を 2 つのヒルベルト空間、$u \in \mathscr{L}(E ; F)$、$n$ 正の整数とします。 公式 (12) に $u_1 = ... = u_n = u$ を入れると、$\hat{T}^n(F)$ から $\hat{T}^n(E)$ までの連続線形写像 $\hat{T}^n(u^*)$ が $\hat{T}^n(E)$ から $\hat{T}^n(F)$ までの連続線形写像 $\hat{T}^n(u)$ の随伴であるという結果が得られます。 公式

$$
\hat{S}^n(u)^* = \hat{S}^n(u^*) , \quad \hat{\Lambda}^n(u)^* = \hat{\Lambda}^n(u^*)
$$

は、$\hat{S}^n(E)$ (V、p. 30、式 (15)) および$\hat{\Lambda}^n(E)$ (V、p. 33、式 (26)) のスカラー積の定義により、式 (12) と同様に成立します。

#### 注意 1 {#evt-v-s4-n1-rem-1 .statement tag=0810}

Suppose the hilbertian 空間 E does not 簡約する to 0. We 同一視する $\mathscr{L}(K;E)$ with E by 写像 $u \mapsto u(1)$;他の語, ベクトルでは、E の x は K から E への写像 $\lambda \mapsto \lambda.x$ と同一視されます。そのとき、x の随伴物は $x^*(y) = \langle x|y \rangle$ によって与えられる写像 $x^*:E \to K$ です。 In other 語, $x \mapsto x^*$ is the canonical semi-linear mapping from E onto its dual (V, p. 15).

同様に、E の自己準同型 $\lambda.1_E$ を使用して同一視する数 $\lambda \in K$ を計算します。すると、$\lambda^*$ は正確に $\lambda$ の共役になります。

これらの識別を使用すると、定義する積 $t_1 ... t_n$ ここで、各 $t_i$ は、K の数、E のベクトル、または E' の線型形式所属、または $\mathscr{L}(E)$ の元になります。次の型のいずれかの 2 つの連続する因子 $t_i$ および $t_{i+1}$ :
• xy ここで、x、y は両方とも E にある、または両方とも E' にあります。
• $A \in \mathscr{L}(E)$、$x \in E$、$x' \in E'$ の xA または Ax'。

合成には次のルールがあります。
a) 結合性。
b) K のすべての元は、他のすべての因子と通勤します。
c) $(t_1 ... t_n)^* = t_n^* ... t_1^*$ があります。他の語では、積の随伴体は位数を逆にとった随伴体の積になります。 $t^{**} = t$も。

たとえば、x、y が E にあり、A が $\mathscr{L}(E)$ にあるとします。次に、$x^*y$ はスカラー 積 $\langle x|y \rangle$ を表し、$x^*Ay$ はスカラー 積 $\langle x|Ay \rangle$ を表します。 $(A^*x)^* = x^*A^{**} = x^*A$ もあるので、$(A^*x)^*y = x^*Ay$ と解釈できます。

$$
\langle A^*x|y \rangle = \langle x|Ay \rangle
$$

付属品の定義に準拠。 $yx^*z$ は結合性により $y(x^*z)$ として、または $y.\langle x|z \rangle$ として解釈できるため、$yx^*$ は E の自己準同型 $z \mapsto y \langle x|z \rangle$ であることがわかります。

ディラック$^1$に続き、数理物理学のほとんどの著作では、Eの元は記号$|x\rangle$で表され、E'の記号は$\langle t|$で表されます。スカラー 積は $\langle x|y \rangle = \langle x|.|y \rangle$ と書かれ、積の禁止の最初のルールでは、記号 $|$ と $|<$ の組み合わせ (たとえば、$|x\rangle|y\rangle$) が除外されます。

#### 命題 3 {#evt-v-s4-prop-3 .statement tag=0811}

— E と F を 2 ヒルベルト空間と $u \in \mathscr{L}(E;F)$ とします。次の条件は同等です。

(i) $u$ はトポロジー ベクトル空間同型であり、その逆数は $u^*$ に等しい。
(ii) $u$ は全射であり、$u^*u = 1_E$;
(iii) $u$ は単射であり、$uu^* = 1_F$;
(iv) $u$ は標準空間の同型です。
(v) $u$ はヒルバーティアン空間同型です。

条件 (1) は、$u^*u = 1_E$ と $uu^* = 1_F$ があることを意味します。したがって、(i)、(ii)、(iii) の同値は、E、II, § 3, No. 8、prop から得られます。 8. (iv) と (v) の同値 (V、p. 5) はすでに見ました。最後に、関係 $u^*u = 1_E$ は次と同等です。

$^1$ P.A.M.ディラック著、量子力学、オックスフォード大学出版局、ニューヨーク、1935年を参照。

$
\langle x|u^*u(y)\rangle = \langle x|y\rangle$、つまり、$E$ のすべての $x, y$ に対して $\langle u(x)|u(y)\rangle = \langle x|y\rangle$ となり、明らかに $u$ が単射であることを暗示しています。これは (ii) と (v) の同値を証明します。

ヒルバート空間 $E$ の自己同型は *ユニタリー演算子*、つまり演算子 $u \in \mathscr{L}(E)$ 満たす $uu^* = u^*u = 1_E$ とも呼ばれます。

#### 注意 2 {#evt-v-s4-n1-rem-2 .statement tag=0812}

— 関係 $u^*u = 1_E$ は、ヒルバーシアン空間 $E$ のすべての自己同型を特徴付けるわけではありません。たとえば、$E = \ell^2(\mathbf{N})$ と $u$ が $n \geq 1$ と $u(x)_0 = 0$ の $u(x_n) = x_{n-1}$ によって定義されるとします。すべての $x \in E$、つまり $u^*u = 1_E$ に対して $\|u(x)\| = \|x\|$ が得られますが、$u$ は全射的ではありません。

#### 注意 3 {#evt-v-s4-n1-rem-3 .statement tag=0813}

— 随伴関数 $u^*$ の定義 (1) は次のように書くこともできます。
$$
\langle y|u(x)\rangle = \langle u^*(y)|x\rangle ,
$$
または、V、p. 15 によって、
$$
\langle u(x), y^*\rangle = \langle x, (u^*(y))^*\rangle .
$$
しかし、$\langle u(x), y^*\rangle = \langle x, {}^t u(y^*)\rangle$ もあるので、転置の項で随伴項を表現できます。
$$
(u^*(y))^* = {}^t u(y^*) .
$$

### 2. 部分的に等角投影線形写像

#### 定義 2 {#evt-v-s4-def-2 .statement tag=0814}

*$E$ と $F$ を 2 つのヒルベルト空間と $u \in \mathscr{L}(E; F)$ とします。 $E$の$u$の核の直交は$u$の最初の部分空間と言われ、$F$の$u$の像の閉包は$u$の最後の部分空間と呼ばれます。 $E$ (それぞれ $F$) から $u$ の初期 (それぞれ最終) 部分空間へのオルソプロジェクターは、$u$ の初期 (それぞれ最終) オルソプロジェクターと呼ばれます。

$P$を$u$の頭文字部分空間とします。 $E$は$P$の直和と$u$の核なので、$u(P) = u(E)$になります。

#### 命題 4 {#evt-v-s4-prop-4 .statement tag=0815}

(i) *$u^*$ の最初 (それぞれ最終) 部分空間は、$u$ の最終 (それぞれ最初) 部分空間と等しい。

(ii) *$E = F$と仮定します。 $M$ を、$E$ とその直交である $M^\circ$ の閉じたベクトル部分空間とします。 関係 $u(M) \subset M$ と $u^*(M^\circ) \subset M^\circ$ は同等です。*

$Q = \overline{u(E)}$を$u$の最後の部分空間とします。 $F$ の $Q$ の直交 $Q^\circ$ は、すべての $x \in E$ に対して $\langle u(x)|y\rangle = 0$ となるように、すべてのベクトル $y$ で構成されます。これは、すべての $x \in E$ に対する $\langle x|u^*(y)\rangle = 0$、または $u^*(y) = 0$ と同等です。したがって、$Q^\circ = \mathrm{Ker}\, u^*$ があり、$Q$ は $u^*$ の最初の部分空間です。 $u$ は $u^*$ の随伴なので、$u^*$ の最後の部分空間は $u$ の最初の部分空間でもあります。これは(i)を証明します。

関係 $u(M) \subset M$ は、$u(M)$ が $M^\circ$ に直交していることを意味し、関係 $u^*(M^\circ) \subset M^\circ$ は、$u^*(M^\circ)$ が $M$ に直交していることを意味します。しかし、すべての $x \in M$ と $y \in M^\circ$ に対して $\langle u(x)|y\rangle = \langle u^*(y)|x\rangle$ があります。したがって (ii) が続きます。

私たちはその小道具に注目します。 4 は、注意 3、V、p. 41 を考慮して、転置 (II, p. 51, cor. 2) の一般的性質から推定できます。

#### 定義 3 {#evt-v-s4-def-3 .statement tag=0816}

*$E$と$F$を2つのヒルベルト空間とします。 写像 $u \in \mathscr{L}(E; F)$ は、$u$ の最初の部分空間までのすべての $x$ 所属が $\|u(x)\| = \|x\|$ である場合、部分的に等長であると言われます*。

$u \in \mathscr{L}(E; F)$ を $N$ を核とし、$I$ を像とします。 $u$ が部分的に等長であると言うのは、$u$ から推定される線形写像 $\tilde{u}: E/N \to I$ が等長である (V, p. 13) というというと同じです。次に、$F$ の部分空間 $I$ が完了したため閉じられ、$u$ の最後の部分空間になります。その結果、$u$ 誘導するは、$u$ の最初の部分空間から最後の部分空間へのヒルバーティアン空間同型になります。

#### 命題 5 {#evt-v-s4-prop-5 .statement tag=0817}

*$u \in \mathscr{L}(E; F)$、$P$を最初の部分空間、$Q$を最後の部分空間とします。 $p$ (それぞれ $q$) が、$u$ の初期 (それぞれ最終) オルソプロジェクターを表すものとします。 $u$ が部分的に等角であると仮定します。*

(i) *写像 $u^* \in \mathscr{L}(F; E)$ は部分的に等長であり、最初の部分空間 $Q$ と最後の部分空間 $P$ があります。 $u$ によって引き起こされる $P$ から $Q$ への同型は、$u^*$ によって引き起こされる $Q$ から $P$ への同型の逆になります。

(ii) *$u^*u = p$と$uu^* = q$があります。*

プロップの都合上。 4(i)、主張(i)は(ii)の帰結です。

ここで (ii) を証明します。 $u^*$の$P$ 含む像から、写像 $u^*u$ 写像 $E$ が $P$ になります。 $x \in E$ と $y \in P$ とすれば、

$$
\langle u^*u(x)|y \rangle = \langle u(x)|u(y) \rangle .
$$

$x$ 属するから $P$ の場合、$\langle u(x)|u(y) \rangle = \langle x|y \rangle$ × 定義は部分的に等角な写像です。 $u$ の $x$ 属するから核 $N$ の場合、$u(x) = 0$、従って $N$ と $P$ は直交なので、$\langle u(x)|u(y) \rangle = 0$ と $\langle x|y \rangle = 0$ になります。 $E = P \oplus N$ 以降、すべてのケースで $\langle u^*u(x) - x|y \rangle = 0$ が得られるため、$u^*u$ は、$E$ から $P$ へのオルソプロジェクター $p$ になります。上記の $uu^* = q$ には、交換すること $u$ と $u^*$ が続きます。

#### 命題 6 {#evt-v-s4-prop-6 .statement tag=0818}

*すべての $u \in \mathscr{L}(E; F)$ に対して、次の条件は同等です:*

(i) *$u$ は部分的に等角投影です ;*
(ii) *$u^*$ は部分的に等角投影です ;*
(iii) *$u^*u$ はオルソプロジェクター ;*
(iv) *$uu^*$ はオルソプロジェクター ;*
(v) *$uu^*u = u ;*$
(vi) *$u^*uu^* = u^* .*$

プロップにより。図５において、（ｉ）は（ｉｉ）と同等である。

(i) $\Rightarrow$ (v) : $u$ が部分的に等角であると仮定します。次に、$u^*u$ は prop による $u$ の初期オルソプロジェクターです。 5. したがって、$u$ の$x \in E$、$u^*u(x) - x$、属するから核ごと、つまり $uu^*u(x) = u(x)$ になります。

(v) $\Rightarrow$ (iii) : $uu^*u = u$ と仮定し、$p = u^*u$ とします。次に$p = p^*$と$p^2 = p$。 $M$ (それぞれ $N$) を $p$ の像 (それぞれ核) とします。 $x \in M$ と $y \in N$ の場合は、$\langle x|y \rangle = \langle p(x)|y \rangle = \langle x|p^*(y) \rangle = \langle x|p(y) \rangle = 0$ になります。 $M$ と $N$ は直交しているため、$p$ は $E$ から $M$ への直交射影です。

(iii) $\Rightarrow$ (i) : $p = u^*u$ が像 $M$ と核 $N$ を持つオルソプロジェクターであると仮定します。

$x \in E$ の皆様には、
$$
\|u(x)\|^2 = \langle u^*u(x)|x \rangle = \langle p(x)|x \rangle .
$$
したがって、$x \in N$ の場合は $u(x) = 0$、$x \in M$ の場合は $\|u(x)\| = \|x\|$ となり、したがって、$u$ は核 $N$ および最初の部分空間 $M$ と部分的に等長になります。

(i)、(iii)、(v) の同値を証明しました。 置き換えること $u$ を $u^*$ により、(ii)、(iv)、(vi) の同値を推定できます。これは有効であることを証明します。 6.

### 3. ノーマル自己準同型

#### 定義 4 {#evt-v-s4-def-4 .statement tag=0819}

$E$ をヒルバーティアン空間と $u \in \mathscr{L}(E)$ とします。 $u$ が随伴する $u^*$ と交換する場合、それが正常であると言います。

たとえば、ヒルバート空間 $E$ のすべての自己同型 $u$ は、$uu^* = u^*u = 1_E$ があるため正常です。

#### 命題 7 {#evt-v-s4-prop-7 .statement tag=081A}

$u \in \mathscr{L}(E)$ が正常であるためには、すべての $x \in E$ が $\|u(x)\| = \|u^*(x)\|$ であることが必要かつ十分です。

私たちは $E$ に定義するエルミート形 $\Phi$
$$
\Phi(x, y) = \langle uu^*(x)|y \rangle - \langle u^*u(x)|y \rangle .
$$
$u$が正常であるためには、$\Phi = 0$が必要十分です。分極公式 (V、p. 2) により、これはすべての $x \in E$ の $\Phi(x, x) = 0$ に相当します。 命題が続きます
$$
\Phi(x, x) = \|u^*(x)\|^2 - \|u(x)\|^2 .
$$

#### 命題 8 {#evt-v-s4-prop-8 .statement tag=081B}

$u \in \mathscr{L}(E)$ が正常であるとします。 $N$を$u$の核と、$E$における$N$の直交$M$とします。 $m$ と $n$ を 2 つの正の整数として、$m + n \geq 1$ とします。次に、$N$ は $u^m(u^*)^n$ の核であり、$M$ は $u^m(u^*)^n$ の最初と最後の部分空間です。特に、$M$ は、$u$ と $u^*$ の最初と最後の部分空間であり、$u$ と $u^*$ の下で安定しています。

提案 7 は、$u$ と $u^*$ が同じ核 $N$ を持つことを示しています。プロップにより。 4、V、p. 41、部分空間 $M$ の$E$ は、$u$ と $u^*$ では安定しています。これは、$N = M^\circ$ の場合、$M \cap N = \{0\}$、自己準同型以降であるためです。 $u$ と $u^*$ によって誘発される $M$ は単射的です。 $v = u^m(u^*)^n$ しましょう。前の引数は、$v$ から $M$ (または $N$) の制限が単射 (または null) であることを示しており、従って、$N$ は $v$ の核です。従って、$M = N^\circ$ は $v$ の最初の部分空間です。プロップにより。 4、V、p. 41の(i)、$v$の最後の部分空間は、$v^*$の最初の部分空間と等しい。しかし、$v^* = u^n(u^*)^m$ なので、$v^*$ の最初の部分空間は、上記により $M$ に等しくなります。

#### 系 {#evt-v-s4-n3-cor-1 .statement tag=081C}

$\lambda \in K$ にしましょう。次の $E$ の部分空間は等しい :
a) $\lambda$ に対する $u$ の固有値部分空間;
b) $\overline{\lambda}$ に対する $u^*$ の固有値部分空間;

c) * $\lambda$ に対する u の主な部分空間 (他の語では、LIE により、$(u - \lambda.1_E)^n(x) = 0$ となるような整数 $n \geqslant 0$ が存在する E のすべてのベクトル $x$ のVII, § 1, No. 1、集合)。
d) *$\overline{\lambda}$ に対する * $u^*$ の *主要な部分空間。

$w = u - \lambda.1_E$ が E の通常の自己準同型であることは明らかです。従って、E の自己準同型 $w, w^* = u^* - \overline{\lambda}.1_E, w^n$ と $(w^*)^n$ は、prop によって同じ核を持ちます。 8.

### 4. エルミート自己準同型

#### 定義 5 {#evt-v-s4-def-5 .statement tag=081D}

*E をヒルバーティアン空間とし、* $u \in \mathscr{L}(E)$ とします。 *$u^* = u$ の場合、あなたはエルミートであると言います。

$\mathscr{H}(E)$ は、$\mathscr{L}(E)$ のすべてのエルミート元の集合を表すものとします。これは、スカラーを制限することによって $\mathscr{L}(E)$ から推定される、$\mathbf{R}$ に対するベクトル空間 $\mathscr{L}(E)_{[\mathbf{R}]}$ のベクトル部分空間です。

それぞれの $u \in \mathscr{L}(E)$ に、$E \times E$ 上のセスキリニア形 $\Phi_u : (x, y) \mapsto \langle x|u(y)\rangle$ を (V、p. 16、cor. 2) 関連付けました。我々は持っています

$$
\Phi_{u^*}(x, y) = \overline{\Phi_u(y, x)} \quad (x, y \text{ in } E);
$$

従って、形 $\Phi_u$ がエルミートである場合に限り、$u$ はエルミートになります。 K が $\mathbf{C}$ の場合、すべての $x \in E$ (V、p. 2、*注意*) に対して $\Phi_u(x, x) = \langle x|u(x)\rangle$ が実数であると仮定するだけで十分です。

$u \in \mathscr{L}(E)$ にしましょう。 (V, p. 16, cor. 2) $u$ のノルムが公式によって計算できることを見てきました。

$$
\|u\| = \sup_{\|x\| \leqslant 1, \|y\| \leqslant 1} |\Phi_u(x, y)|.
$$

$u$ がエルミートの場合、次の結果が得られます。

#### 命題 9 {#evt-v-s4-prop-9 .statement tag=081E}

*E のすべてのエルミート自己準同型 u について、*私たちは*

$$
\|u\| = \sup_{\|x\| \leqslant 1} |\langle x|u(x)\rangle|.
$$

$\Phi = \Phi_u$ と $c = \sup_{\|x\| \leqslant 1} |\Phi(x, x)|$ を入れてから、明らかに $c \leqslant \|u\|$ とします。 $x, y$ を E に入れて、$\|x\| \leqslant 1, \|y\| \leqslant 1$ とします。それから

$$
\Phi(x + y, x + y) = \Phi(x, x) + \Phi(y, y) + 2\Re\Phi(x, y),
$$
従って
$$
4\Re\Phi(x, y) = \Phi(x + y, x + y) - \Phi(x - y, x - y);
$$
しかし、すべての $t \in E$ に対して $|\Phi(t, t)| \leqslant c\|t\|^2$ であるため、
$$
4|\Re\Phi(x, y)| \leqslant c(\|x + y\|^2 + \|x - y\|^2) = 2c(\|x\|^2 + \|y\|^2) \leqslant 4c.
$$
$a = \Phi(x, y)$ にしましょう。次のような絶対値 1 を持つ複素数 $\lambda$ が存在します。

λa = |a|。前の不等式で置き換えること y を λy にすると、$|\Phi(x, y)| \leq c$ が得られます。 (15) までに、$\|u\| \leq c$ と命題が続きます。 Q.E.D.

明らかに、すべてのエルミート自己準同型は正常です。逆に:

#### 命題 10 {#evt-v-s4-prop-10 .statement tag=081F}

— K が C であると仮定します。 $u \in \mathscr{L}(E)$ にしましょう。次に、$u = h_1 + ih_2$ のような、E のエルミート自己準同型の一意の対 $(h_1, h_2)$ が存在します。あなたが普通である位数では、$h_1$と$h_2$が通勤すれば必要十分です。

なぜなら、関係 « $u = h_1 + ih_2,\ h_1^* = h_1,\ h_2^* = h_2$ » は以下と同等です。

$$
\text{« } h_1 = \frac{1}{2}(u + u^*) \text{ and } h_2 = \frac{i}{2}(u^* - u) \text{ »}.
$$

加法には $h_1 h_2 - h_2 h_1 = \frac{i}{2}(uu^* - u^*u)$ があります。これは有効であることを証明します。 10.

#### 命題 11 {#evt-v-s4-prop-11 .statement tag=081G}

— $p \in \mathscr{L}(E)$ としましょう。 p が E から E の閉じたベクトル部分空間へのオルソプロジェクターである位数では、 $p^2 = p = p^*$ であることが必要かつ十分です。

$p^2 = p$ と仮定します。 M を p の像とし、N をその核とします。 E は M と N のトポロジー 直和です。p がオルソ投影器である位数では、M が N に直交していることが必要かつ十分です。つまり、E のすべての x、y に対して $\langle p(x)|y - p(y) \rangle = 0$ が得られます。この後者の関係は $p = p^*p$ と同等であり、$p^* = (p^*p)^* = p^*p = p$ を意味します。逆に、$p^* = p$ の場合は、$p = p^2 = p^*p$ になります。

### 5. ポジティブ自己準同型

#### 定義 6 {#evt-v-s4-def-6 .statement tag=081H}

— E をヒルバーティアン空間および $u \in \mathscr{L}(E)$ とします。 u が正であると言い、u がエルミートの場合、すべての $x \in E$ に対して $\langle x|u(x) \rangle \geq 0$ の場合、$u \geq 0$ と書きます。

K が C、関係に等しい場合

$$
\langle x|u(x) \rangle \geq 0 \quad \text{for all } x \in E
$$

これは、u がエルミート (V, p. 2, 注意) であるため、正であることを意味します。

$\mathscr{L}_+(E)$ は、$\mathscr{L}(E)$ のすべての正の元のうちの集合を表すものとします。これは、$\mathscr{L}(E)$ の基礎となる実際のベクトル空間 $\mathscr{L}(E)_{[\mathbf{R}]}$ にある、適切な尖った凸円錐です。 u が正である位数では、u に関連付けられた $E \times E$ 上のセスキ線形形 $\Phi_u$ が正のエルミートであることが必要かつ十分です。 $\mathscr{L}(E)$ の u と v を考えると、関係 $u - v \geq 0$ は $u \geq v$ または $v \leq u$ と書くこともできます。これは、$\mathscr{L}(E)_{[\mathbf{R}]}$ の位数関係で、実際のベクトル空間構造と互換性があります。

#### 命題 12 {#evt-v-s4-prop-12 .statement tag=081I}

— u を $\mathscr{L}(E)$ のエルミート (それぞれ正) 元とし、v を E からヒルバーシアン空間 F への連続線形写像とする。すると、$vuv^*$ は のエルミート (それぞれ正) 元となる。 $\mathscr{L}(F)$。

なぜなら、私たちには$(vuv^*)^* = v^{**}u^*v^* = vuv^*$があるからです。一方、$u \geq 0$ の場合、

$$
\langle y|vuv^*(y) \rangle = \langle v^*(y)|u(v^*(y)) \rangle \geq 0
$$

すべての$y \in F$、したがって$vuv^* \geq 0$。

提案 12 は、特に、$vv^*$ がすべての $v \in \mathscr{L}(E; F)$ に対して正であることを示しています。特に、オルソプロジェクター $p$ は $p = p^2 = pp^*$ を満たすため、これは肯定的です。

#### 注意 1 {#evt-v-s4-n5-rem-1 .statement tag=081J}

$\mathscr{L}(E)$ のエルミート $u$ ごとに、$m(u) = \inf_{\|x\|=1} \langle x|u(x)\rangle$、$M(u) = \sup_{\|x\|=1} \langle x|u(x)\rangle$ を入れます。 $E$ が単なる 0 ではない場合、$m(u)$ と $M(u)$ は有限です。さらに、$M(u)$ は最小の実数 $\lambda$ で、$u \leq \lambda \cdot 1_E$ と $m(u)$ 最大の実数 $\mu$ は $u \geq \mu \cdot 1_E$ になります。明らかに、$m(-u) = -M(u)$ と $M(-u) = -m(u)$ があります。それは明らかです
$$
\sup(|m(u)|, |M(u)|) = \sup_{\|x\|=1} |\langle x|u(x)\rangle|
$$
そしてプロップ。 9 (V、p. 44) は、($E \neq \{0\}$ の場合)
$$
\|u\| = \sup(|m(u)|, |M(u)|).
$$
\* $K$ が $\mathbf{C}$ である場合の、この公式の他の証明については、prop を参照してください。 TSの14、I, § 6, No. 8。 \*

#### 注意 2 {#evt-v-s4-n5-rem-2 .statement tag=081K}

$M$ と $N$ を、$E$ の 2 つの閉じたベクトル部分空間と、$E$ から $M$ (それぞれ $N$) へのオルソプロジェクター$p_M$ (それぞれ $p_N$) とします。次に、$p_M \leq p_N$ の場合に限り、$M \subset N$ になります。 $p_M^* p_M = p_M$ があるため、
$$
\|p_M(x)\|^2 = \langle p_M(x)|p_M(x)\rangle = \langle x|p_M^* p_M(x)\rangle = \langle x|p_M(x)\rangle
$$
$x \in E$の皆さんへ。したがって、関係 $p_M \leq p_N$ は、« すべての $x \in E$ に対して $\|p_M(x)\| \leq \|p_N(x)\|$ » と同等です。 $M \subset N$ の場合、$p_M = p_M p_N$ があるため、$\|p_M\| \leq 1$ から $\|p_M(x)\| \leq \|p_N(x)\|$ になります。逆に、すべての$x \in E$に対して$\|p_M(x)\| \leq \|p_N(x)\|$であれば、$p_M$の核、$p_N$の含む、核、つまり$M^\circ \supset N^\circ$は$M \subset N$を意味します。

#### 命題 13 {#evt-v-s4-prop-13 .statement tag=081L}

— *$\mathscr{H}(E)$ を、ヒルバーシアン空間 $E$ のすべての連続エルミート自己準同型の集合とします。 $\mathscr{F}$ を空ではなく、増加するに向けられ、$\mathscr{H}(E)$ の境界がある部分集合とします。*

(i) *集合 $\mathscr{F}$ には $\mathscr{H}(E)$ に上界 $u_0$ が含まれています。私たちは*を持っています
$$
\langle x|u_0(x)\rangle = \sup_{u \in \mathscr{F}} \langle x|u(x)\rangle \quad \text{for all} \quad x \in E .
$$

(ii) *$\mathscr{F}$の切断のフィルタは、単純収束性の位相を備えた空間$\mathscr{L}(E)$で$u_0$に収束します。

$\Sigma$ を $\mathscr{F}$ の切断のフィルターとします。すべての $u \in \mathscr{H}(E)$ について、$\Phi_u$ を、次のように定義される $E$ 上の連続エルミート形とします。
$$
\Phi_u(x, y) = \langle x|u(y)\rangle .
$$
しましょう
$$
\Psi_u(x) = \Phi_u(x, x)
$$
$u \in \mathscr{H}(E)$ と $x \in E$ 用。分極公式 (V, p. 2) により、次のようになります。
$$
\begin{align*}
(19) \quad 4\Phi_u(x, y) &= \Psi_u(x+y) - \Psi_u(x-y) & \text{if } K = \mathbf{R} \\
(20) \quad 4\Phi_u(x, y) &= \Psi_u(x+y) - \Psi_u(x-y) - i\Psi_u(x+iy) + i\Psi_u(x-iy) & \text{if } K = \mathbf{C} .
\end{align*}
$$

すべての $x \in E$ について、$\mathbf{R}$ への写像 $u \mapsto \Psi_u(x)$ は増加するであり、有界であるため、$\Sigma$ に関しては極限になります。前の公式、極限により
$$
\lim_{u,\Sigma} \Phi_u(x, y) = \Phi(x, y)
$$
は、元の $E$ のすべての対 $(x, y)$ に存在します。 $\Phi$ が $E$ のエルミート形であることは明らかです。 $v_1 \in \mathscr{F}$ と $v_2$ が $\mathscr{F}$ の境界である場合、エルミート形 $f_1 = \Phi - \Phi_{v_1}$ と $f_2 = \Phi_{v_2} - \Phi$ は正です。そのような実数 $M \geq 0$ が存在します
$$
f_1(x, x) + f_2(x, x) = \Phi_{v_2 - v_1}(x, x) \leq M \|x\|^2,
$$
従って
$$
f_1(x, x) \leq M \|x\|^2, \quad f_2(x, x) \leq M \|x\|^2 \quad (x \in E);
$$
従って、準規範 $x \mapsto f_i(x, x)^{1/2}$ は $E$ にも継続します。以来
$$
f_2 - f_1 = \Phi_{v_2} + \Phi_{v_1} - 2\Phi,
$$
$x \mapsto \Phi(x, x)$ は $E$ で連続する写像であることが結論するわかり、公式 (19) と (20) より、$\Phi$ は $E \times E$ で連続であることがわかります。従って、$\Phi = \Phi_{u_0}$ となるような $\mathscr{H}(E)$ の (V, p. 16, cor. 2) 元 $u_0$ が存在します。 公式 (18) は明らかに満たされているため、$u_0$ は $\mathscr{H}(E)$ の $\mathscr{F}$ の上界です。これは(i)を証明します。

構成までに
$$
\lim_{u,\Sigma} \langle x|(u_0 - u)(x)\rangle = 0 \quad \text{for all } x \in E.
$$
$v_1 \in \mathscr{F}$ にしましょう。 $u \geq v_1$ となるような $u \in \mathscr{F}$ が与えられた場合、$v = u_0 - u$ とします。コーシー・シュワルツ不等式を $E$ の正のエルミート形 $\Phi_v$ に適用すると、次のようになります。
$$
\begin{align*}
\|v(x)\|^4 &= |\Phi_v(v(x), x)|^2 \leq \Phi_v(v(x), v(x)) \cdot \Phi_v(x, x) \\
&= \langle v(x)|v^2(x)\rangle \langle x|v(x)\rangle \leq \|v\|^3 \|x\|^2 \langle x|v(x)\rangle \\
&\leq \|u_0 - v_1\|^3 \|x\|^2 \langle x|v(x)\rangle,
\end{align*}
$$
$\|v\| \leq \|u_0 - v_1\|$ から V、p. 44、プロップ。 9. 次に、(21) によって、すべての $x \in E$ に対して $\lim_{u,\Sigma} \|(u_0 - u)(x)\| = 0$ が得られます。これは主張 (ii) を証明します。

特にプロップ。 13 は、増加するの場合に適用でき、数列 $(u_n)_{n \in \mathbf{N}}$ の元の $\mathscr{H}(E)$ が制限されます。次に、次の特徴を持つ $\mathscr{H}(E)$ の元 $v$ が存在します。
$$
\langle x|v(x)\rangle = \lim_{n \to \infty} \langle x|u_n(x)\rangle = \sup_{n \in \mathbf{N}} \langle x|u_n(x)\rangle \quad (x \in E),
$$
そしてすべての $x \in E$ に対して $v(x) = \lim_{n \to \infty} u_n(x)$ があります。また、$v$は$\mathscr{H}(E)$の$u_n$の集合の上界です。

### 6. 自己準同型の痕跡

E と F を 2 ヒルベルト空間とします。 V、p. 40 の規則に従い、E の $a$ と F の $b$ を表す $ba^*$ を、E から F までの連続する線形写像 $x \mapsto b \langle a|x \rangle$ を表します。

#### 補題 1 {#evt-v-s4-lem-1 .statement tag=081M}

*ベクトル空間 $F \otimes E'$ から空間 $\mathscr{L}_f(E; F)$ までの有限階数線形写像 E から F までの連続する同型 $\theta$ が存在し、$\theta(b \otimes a^*) = ba^*$ 対 $a \in E, b \in F$ によって特徴付けられます。

A、II, § 4, No. 2 により、$F \otimes E'$ から $\mathscr{L}(E; F)$ への単射詞線形写像 $\theta$ が存在し、そのようなものは 1 つだけ存在し、$a' \in E', b \in F$ に対して変換 $b \otimes a'$ から線形写像 $x \mapsto ba'(x)$ になります。明らかに、$\theta$の$\theta(b \otimes a^*) = ba^*$と像は$\mathscr{L}_f(E; F)$に含まれています。ただし、$u \in \mathscr{L}_f(E; F)$ と $(e_1, ..., e_n)$ を F の $u$ の像の正規直交基底とする。 $1 \leq i \leq n$ に対して $f_i = u^*(e_i)$ とする。 $x \in E$ ごとに、

$$
u(x) = \sum_{i=1}^n \langle e_i|u(x) \rangle \cdot e_i = \sum_{i=1}^n \langle f_i|x \rangle \cdot e_i,
$$

したがって$u = \sum_{i=1}^n e_i f_i^* = \theta(\sum_{i=1}^n e_i \otimes f_i^*)$です。したがって、$\theta$の像は$\mathscr{L}_f(E; F)$と等しいです。

今後、$E = F$ と仮定し、集合 $\mathscr{L}_f(E) = \mathscr{L}_f(E; E)$ と仮定します。 補題 1 までに、$a \in E, a' \in E'$ に対して $\tau(\theta(a \otimes a')) = a'(a)$ となるように、$\mathscr{L}_f(E)$ には一意の線型形式 $\tau$ が存在します。他の語では、

(22)
$$
\tau(ba^*) = \langle a|b \rangle \quad \text{for } a, b \text{ in } E.
$$

E が有限次元の場合、$\mathscr{L}_f(E) = \mathscr{L}(E)$ があり、$\tau(u)$ は E (A, II, § 4, No. 3) の自己準同型 $u$ の *トレース* です。

#### 補題 2 {#evt-v-s4-lem-2 .statement tag=081N}

*$(e_i)_{i \in I}$ を E の正規直交値基底とします。すると*

$$
\tau(u) = \sum_{i \in I} \langle e_i|u(e_i) \rangle
$$

*すべて* $u \in \mathscr{L}_f(E)$。

E で $u = ba^*$ と $a, b$ の場合を考えれば十分です。

$$
\langle e_i|u(e_i) \rangle = e_i^* b \cdot a^* e_i = \overline{\langle e_i|a \rangle} \langle e_i|b \rangle
$$

そして、補題 2 は、V、p. 22 の公式 (22) と公式 (3) から続きます。

#### 補題 3 {#evt-v-s4-lem-3 .statement tag=081O}

*u を E の連続正の自己準同型、および E 上のすべての有限階数オルソプロジェクターの $\mathscr{F}$ 集合とします。すると、E のすべての正規直交基底 $(e_i)_{i \in I}$ について、($\mathbf{R}_+$ で) 等式が得られます。

$$
\sum_{i \in I} \langle e_i|u(e_i) \rangle = \sup_{p \in \mathscr{F}} \tau(pup).
$$

I の有限部分集合 J ごとに、$p_J = \sum_{i \in J} e_i e_i^*$ を入れます。これは、ベクトル $e_i$ によって生成された E からベクトル部分空間へのオルソプロジェクターです。ここで、i の範囲は J です。
$$
p_J u p_J = \sum_{i \in J, j \in J} \langle e_i | u(e_j) \rangle e_i e_j^* ,
$$
したがって $\tau(p_J u p_J) = \sum_{i \in J} \langle e_i | u(e_i) \rangle$ です。 $p_J \in \mathscr{F}$ 以来、
$$
\sum_{i \in J} \langle e_i | u(e_i) \rangle \leq \sup_{p \in \mathscr{F}} \tau(p u p) ;
$$
それで私たちは結論する
$$
\sum_{i \in I} \langle e_i | u(e_i) \rangle = \sup_J \sum_{i \in J} \langle e_i | u(e_i) \rangle \leq \sup_{p \in \mathscr{F}} \tau(p u p) .
$$

$v$ を有限階数連続かつ E の正の自己準同型とし、$p \in \mathscr{F}$ とします。までに。 V、p. 23 の 2 には、E の正規直交基底 $(f_\alpha)_{\alpha \in A}$ と A の有限部分集合 B が存在し、$(f_\alpha)_{\alpha \in B}$ は p. 像の正規直交基底になります。次に、$p = \sum_{\alpha \in B} f_\alpha f_\alpha^*$ があり、上記のように、関係 $\tau(p v p) = \sum_{\alpha \in B} \langle f_\alpha | v(f_\alpha) \rangle$ となります。 補題 2 (V, p. 48) までに $\tau(v) = \sum_{\alpha \in A} \langle f_\alpha | v(f_\alpha) \rangle$ となり、公式となります。
$$
\sum_{\alpha \in B} \langle f_\alpha | v(f_\alpha) \rangle \leq \tau(v) .
$$
適用この不等式を $v = p_J . u p_J$ で、J が I の有限部分集合である場合、次のようになります。
$$
\sum_{\alpha \in B} \langle p_J(f_\alpha) | u p_J(f_\alpha) \rangle \leq \sum_{i \in J} \langle e_i | u(e_i) \rangle .
$$
すべての $x \in E$ に対して、$p_J(x) = \sum_{i \in J} \langle e_i | x \rangle e_i$ があり、したがって、I の有限部分集合 J の順序付けられた有向集合に関しては $x = \lim_J p_J(x)$ になります。 (23) で J を超える移行から極限を得る
$$
\tau(p u p) = \sum_{\alpha \in B} \langle f_\alpha | u(f_\alpha) \rangle \leq \sum_{i \in I} \langle e_i | u(e_i) \rangle ,
$$
これで補題 3 の証明が完了します。

#### 定義 7 {#evt-v-s4-def-7 .statement tag=081P}

*u をヒルバーシアン空間 E の連続的で正の自己準同型とします。* しましょう
$$
\operatorname{Tr}(u) = \sup_{p \in \mathscr{F}} \tau(p u p)
$$
*($\overline{\mathbf{R}}_+$の上界)、ここで、$\mathscr{F}$はE上のすべての有限階数オルソプロジェクターの集合です。$\operatorname{Tr}(u)$がuの痕跡であると言います。*

$p$ を $E$ から $E$ の有限次元ベクトル部分空間への直交射影とし、 $(x_1, ..., x_m)$ を $F$ の正規直交値基底とします。 関係を設立しました
$$
\tau(pup) = \sum_{i=1}^m \langle x_i | u(x_i) \rangle.
$$
従って、定義する公式でトレースすることができます。
$$
\text{Tr}(u) = \sup_{x_1, ..., x_m} \sum_{i=1}^m \langle x_i | u(x_i) \rangle,
$$
ここで、$(x_1, ..., x_m)$ は、すべての有限正規直交関数の集合、$E$ のベクトルの数列の範囲になります。

補題 3 (V, p. 48) までに、
$$
\text{Tr}(u) = \sum_{i \in I} \langle e_i | u(e_i) \rangle
$$
$E$ のすべての正規直交基底 $(e_i)_{i \in I}$ に対して。 これから推測すると、
$$
\text{Tr}(u + v) = \text{Tr}(u) + \text{Tr}(v)
$$
$$
\text{Tr}(\lambda u) = \lambda \cdot \text{Tr}(u)
$$
$E$ のすべての連続かつ正の自己準同型 $u$ と $v$ 、およびすべての実数 $\lambda \geq 0$ について ((27) で$0.(+\infty) = 0$ を規則にします)。 $\phi$ を $E$ からヒルバート空間 $F$ への同型とします。 $\phi$ 変換 $E$ の各正規直交基底を $F$ の正規直交基底に変換するので、(25) から次のようになります。
$$
\text{Tr}(\phi u \phi^{-1}) = \text{Tr}(u).
$$

$(u_\alpha)_{\alpha \in A}$ を空ではない有向増加するであり、$E$ の連続かつ正の自己準同型の有界族とする。 $u = \sup_\alpha u_\alpha$、次にすべての $x \in E$ に対して $\langle x | u(x) \rangle = \sup_\alpha \langle x | u_\alpha(x) \rangle$ とします (V、p. 46、提案 13)。 $\text{Tr}(u) = \sup_{J \subset I} \sum_{i \in J} \langle e_i | u(e_i) \rangle$ があり、$J$ は $I$ のすべての有限部分集合に及ぶため、
$$
\text{Tr}(u) = \sup_\alpha \text{Tr}(u_\alpha) \quad \text{for} \quad u = \sup_\alpha u_\alpha.
$$

$p_F$ を、$E$ からヒルバーシアン部分空間 $F$ へのオルソプロジェクターとします。 $E$ の正規直交基底 $(e_i)_{i \in I}$ と $I$ の部分集合 $J$ が存在し、$(e_i)_{i \in J}$ は $F$ の正規直交基底になります。 $\text{Tr}(p_F up_F) = \sum_{i \in J} \langle e_i | u(e_i) \rangle$があります。この公式には 2 つの帰結があります。まず、$\text{Tr}(p_F up_F) \leq \text{Tr}(u)$ があります。次に、$u = 1_E$ を取ると、次のようになります。
$$
\text{Tr}(p_F) = \begin{cases}
\dim F & \text{if } F \text{ is finite dimensional} \\
+ \infty & \text{if not}.
\end{cases}
$$

#### 定義 8 {#evt-v-s4-def-8 .statement tag=081Q}

— E を複素ヒルベルト空間とします。有限トレースを持つ E のすべての連続した正の自己準同型によって生成される $\mathscr{L}(E)$ のベクトル部分空間に対して $\mathscr{L}^1(E)$ を書き込みます。

V、p. 50 の公式 (25) により、$\mathscr{L}^1(E)$ 上の拡大するから線型形式までのトレースは、再び Tr で示され、すべての $u$ については満たす関係 $\operatorname{Tr}(u) = \sum_{i \in I} \langle e_i | u(e_i) \rangle$ になります。 $\mathscr{L}^1(E)$ と、E の正規直交基底 $(e_i)_{i \in I}$ ごとに、$u \in \mathscr{L}^1(E)$ ごとに、$u^* \in \mathscr{L}^1(E)$ と $\operatorname{Tr}(u^*) = \overline{\operatorname{Tr}(u)}$ が得られます。 Vの公式(28)、p. 50拡大するから$u$属する〜$\mathscr{L}^1(E)$の場合。 F を E のヒルバーティアン部分空間とします。 F が有限次元である場合に限り、公式 (30)、オルソプロジェクター $p_F$ 属するから $\mathscr{L}^1(E)$ によって。 E のすべての $a$ と $b$ に対して、$4ab^* = \sum_{\varepsilon^4 = 1} \varepsilon(a + \varepsilon b)(a + \varepsilon b)^*$ があり、$cc^*$ はすべての $c \in E$ に対して有限トレースを持つ正の演算子です。従って、$u$がEの連続自己準同型である有限階数であれば、$u \in \mathscr{L}^1(E)$と$\operatorname{Tr}(u) = \tau(u)$になります。

E を実ヒルバーティアン空間とし、$E_{(c)}$ をその複素数 (V, p. 5) とします。私たちは$E_{(c)}$の部分集合と同一視するEです。次に、$\mathscr{L}(E)$ は、$E_{(c)}$ から $E_{(c)}$ までのすべての連続線形写像 $u$ のうち、$u(E) \subset E$ のように、$\mathscr{L}(E_{(c)})$ からなるの実ベクトル部分空間と識別できます。この場合、$\mathscr{L}^1(E) = \mathscr{L}(E) \cap \mathscr{L}^1(E_{(c)})$と書きます。すべての $u \in \mathscr{L}^1(E)$ について、トレース $\operatorname{Tr}(u)$ は実数であり、$\operatorname{Tr}(u^*)$ に等しくなります。 公式 (25) と (28) は再び有効で、$\mathscr{L}_f(E) \subset \mathscr{L}^1(E)$ と $\operatorname{Tr}(u) = \tau(u)$ はすべての $u \in \mathscr{L}_f(E)$ に対して有効です。最後に、E の閉じたベクトル部分空間 F は、$p_F$ 属するから $\mathscr{L}^1(E)$ の場合に限り、有限次元になります。

\* 注意 1. — 後で、核写像を Banach 空間 E から Banach 空間 F に定義する概念変換します。 $\mathscr{L}^1(E)$ が E から E までのすべての核写像で構成されている場合、E は実数または複素数のヒルバーシアン空間であることを示します。 \*

#### 命題 14 {#evt-v-s4-prop-14 .statement tag=081R}

— $E_1, ..., E_n$ をヒルバーティアン空間、$E = E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$、$u_i$ を $1 \leq i \leq n$ に対する $E_i$ の連続自己準同型とする。 $u_1, ..., u_n$ が正の場合、$u = u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n$ も正です。

$$
\operatorname{Tr}(u) = \prod_{i=1}^n \operatorname{Tr}(u_i).
$$

すべての $1 \leq i \leq n$ に対して $u_i \in \mathscr{L}^1(E_i)$ の場合、この場合も $u \in \mathscr{L}^1(E)$ と公式 (31) が有効になります。

$n$ で帰納法まで進み、すぐに簡約するのケース $n = 2$ に進みます。

$i = 1, 2$ の場合、$E_i$ の $x, y$ に対して公式 $\Phi_i(x, y) = \langle x | u_i(y) \rangle$ により、$E_i$ でセスキリニア形 $\Phi_i$ を定義する計算します。 $u_1$ と $u_2$ が正の場合、形 $\Phi_1$ と $\Phi_2$ はエルミートで正です。プロップにより。 V、p. 25 の 1 には、ベクトル空間 $E_1 \otimes E_2$ に正のエルミート形 $\Phi$ が存在します。

$$
\Phi(x_1 \otimes x_2, y_1 \otimes y_2) = \Phi_1(x_1, y_1) \cdot \Phi_2(x_2, y_2)
$$

$E_1$の$x_1, y_1$と$E_2$の$x_2, y_2$。 $z$ と $E_1 \otimes E_2$ の $t$ については、すぐに関係 $\Phi(z, t) = \langle z | u(t) \rangle$ を確認します。 $\Phi$ は正なので、$E_1 \otimes E_2$ のすべての $z$ に対して $\langle z | u(z) \rangle \geq 0$ が得られます。 $u$ は連続であり、$E_1 \otimes E_2$ はヒルバート空間 $E = E_1 \hat{\otimes}_2 E_2$ で密であるため、$u$ は E の連続で正の自己準同型であることが結論するわかります。

$(e_i)_{i \in I}$ を $E_1$ の正規直交基底とし、$(f_j)_{j \in J}$ を $E_2$ の正規直交基底とします。すると、族 $(e_i \otimes f_j)_{i \in I, j \in J}$ は $E$ の正規直交基底となり、次のようになります。

$$
\operatorname{Tr}(u) = \sum_{i \in I} \sum_{j \in J} \langle e_i \otimes f_j | u(e_i \otimes f_j) \rangle \\
= \sum_{i \in I} \sum_{j \in J} \langle e_i | u_1(e_i) \rangle \cdot \langle f_j | u_2(f_j) \rangle \\
= \operatorname{Tr}(u_1) \cdot \operatorname{Tr}(u_2) .
$$

特に、$u_1$ と $u_2$ が有限トレースで正の自己準同型である場合、$u$ も同様です。線形性により、$K = \mathbf{C}$ の場合は $u$ 属するから $\mathscr{L}^1(E)$ となり、$i = 1, 2$ の場合は $u_i$ 属するから $\mathscr{L}^1(E_i)$ になると推定されます。 公式 (31) 拡大するは線形性によりこの場合に成り立ちます。最後に、$K = \mathbf{R}$と$u_i \in \mathscr{L}^1(E_i)$簡約するをスカラーの拡大による複素数にした場合です。

#### 注意 2 {#evt-v-s4-n6-rem-2 .statement tag=081S}

— $E$ をヒルバーティアン空間とします。これは、ヒルバーティアン部分空間の族 $(E_i)_{i \in I}$ のヒルバーティアン和です。 $u$ を $\mathscr{L}(E)$ の元として、すべての $i \in I$ に対して $u(E_i) \subset E_i$ となるようにします。 $u_i$を$E_i$の$u$と一致するを合わせた$\mathscr{L}(E_i)$の元とします。次に、$u$ が正の場合は $\operatorname{Tr}(u) = \sum_{i \in I} \operatorname{Tr}(u_i)$、または $\mathscr{L}^1(E)$ に対して属する。この関係は、V の公式 (25) から続き、$E_i$ のそれぞれの正規直交基底の和集合である$E$ の正規直交基底に適用されるp. 50 です。

### 7. ヒルベルト・シュミット写像

#### 定義 9 {#evt-v-s4-def-9 .statement tag=081T}

*$E$と$F$を2つのヒルベルト空間とします。 $E$ から $F$ までの連続線形写像 $u$ は、$E$ の正の自己準同型 $u^*u$ の軌跡が有限である場合、ヒルベルト・シュミット写像と呼ばれます。 $E$ から $F$ までのすべてのヒルベルト・シュミット写像のうち集合は、$\mathscr{L}^2(E, F)$ で示されます。*

$E = F$の場合、$\mathscr{L}^2(E; E)$を$\mathscr{L}^2(E)$と書きます。

すべての $u \in \mathscr{L}(E, F)$ について、$\|u\|_2 = \operatorname{Tr}(u^*u)^{1/2}$ とすることで、$\|u\|_2$ が有限である場合に限り、$u$ 属するから $\mathscr{L}^2(E; F)$ になります。トレースの定義により、次の結果が得られます。

$$
\|u\|_2^2 = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m \|u(x_i)\|^2
$$

ここで、$(x_1, \ldots, x_m)$ は、$E$ の有限正規直交関数数列の集合にわたる範囲です。特に、公式 (32) の $m = 1$ を取ると、次のようになります。

$$
\|u\| \leq \|u\|_2 \quad (u \in \mathscr{L}(E; F)) .
$$

$(e_i)_{i \in I}$ を $E$ の正規直交基底とし、$(f_j)_{j \in J}$ を $F$ の正規直交基底とします。 V、p. 50 とパーシヴァルの関係 (V、p. 22) の公式 (25) までに、

$$
\|u\|_2^2 = \sum_{i \in I} \|u(e_i)\|^2 = \sum_{i,j} |\langle f_j | u(e_i) \rangle|^2 .
$$

$|\langle f_j|u(e_i)\rangle| = |\langle e_i|u^*(f_j)\rangle|$ なので、公式 (34) は次のことを意味します。
$$
\|u^*\|_2 = \|u\| ;
$$
したがって、ヒルベルト-シュミット写像の随伴物はヒルベルト-シュミット写像です。 $E_1, F_1$ をヒルベルト空間とし、$v : E_1 \to E, w : F \to F_1$ を連続線形写像とします。 (32) から、次のことがすぐに推測されます。
$$
\|wu\|_2 \leq \|w\|.\|u\|_2 .
$$
(35)、(36)、および関係 $uv = (v^*u^*)^*$ により、次のようになります。
$$
\|uv\|_2 \leq \|u\|_2\,\|v\| .
$$
特に、$u$ 属するから $\mathscr{L}^2(E, F)$ の場合、$wuv$ 属するから $\mathscr{L}^2(E_1, F_1)$ となります。

#### 定理 1 {#evt-v-s4-thm-1 .statement tag=081U}

*E と F を 2 ヒルベルト空間とします。*
(i) *集合 $\mathscr{L}^2(E, F)$ は $\mathscr{L}(E; F)$ のベクトル部分空間であり、$u \mapsto \|u\|_2$ はノルム* (V、p. 6) *$\mathscr{L}^2(E; F)$ のヒルバーティアンです。
(ii) *$F \otimes E'$から$\mathscr{L}_f(E; F)$までの同型$\theta$は、$\theta(y \otimes x^*) = yx^*$拡大するから同型$F \otimes_2 E'$から$\mathscr{L}^2(E; F)$までの$\hat{\theta}$を特徴とします。特に$\mathscr{L}^2(E; F)$では$\mathscr{L}_f(E; F)$が密集しています*。

$(e_i)_{i \in I}$ (それぞれ $(f_j)_{j \in J}$) を $E$ (それぞれ $F$) の正規直交基底とします。すべての $u \in \mathscr{L}(E; F)$ について、$E$ と $F$ (V、p. 22) に対して選択された正規直交値基底に関して、$\Lambda(u)$ を $u$ の行列とします。 $\|a\|_2$ がヒルバーシアン空間 $\ell^2(J \times I)$ の元 $a$ のノルムを表すものとします。 公式 (34) により、$\Lambda$ は $\mathscr{L}^2(E; F)$ から $\ell^2(J \times I)$ に写像となり、$\|\Lambda(u)\|_2 = \|u\|$ になります。 $\Lambda$ が*単射*であることは明らかです。 (i) を証明するには、$\Lambda$ が *全射* であることを証明すれば十分です。 $a = (a_{ji})$ を $\ell^2(J \times I)$ の元とします。コーシー・シュワルツ不等式著、
$$
|\sum_{j,i} \overline{\eta}_j a_{ji} \xi_i|^2 \leq \sum_{j,i} |a_{ji}|^2 \sum_{j,i} |\overline{\eta}_j \xi_i|^2 = \|a\|_2^2\,\|\xi\|^2\,\|\eta\|^2
$$
$\ell^2(I)$ の $\xi = (\xi_i)$ と $\ell^2(J)$ の $\eta = (\eta_j)$ ごとに。次に、$E$の$x = \sum_i \xi_i e_i$と$F$の$y = \sum_j \eta_j f_j$に対して$\Phi(y, x) = \sum_{j,i} \overline{\eta}_j a_{ji} \xi_i$となるように、$F \times E$には連続セスキロニア形$\Phi$が存在します。 $u \in \mathscr{L}(E; F)$ を $\Phi(y, x) = \langle y|u(x)\rangle$ (V, p. 16, cor. 2) となるようにします。得ます
$$
a_{ji} = \Phi(f_j, e_i) = \langle f_j|u(e_i)\rangle \quad \text{for} \quad i \in I, j \in J ,
$$
したがって $a = \Lambda(u)$ です。

$\Lambda$ は $\mathscr{L}^2(E; F)$ から $\ell^2(J \times I)$ へのヒルベルト空間同型写像であり、$(f_j \otimes e_i^*)$ は $F \otimes_2 E'$ の正規直交基底であるため、$F \otimes_2 E'$ から $\mathscr{L}^2(E; F)$ への同型写像 $\hat{\theta}$ が存在します。
$$
\langle f_j|\hat{\theta}(t)\,e_i\rangle = \langle f_j \otimes e_i^*|t\rangle
$$

$i \in I,\ j \in I$ と $t \in F \otimes_2 E'$ ごとに。特に、$t = y \otimes x^*$ については、
$$
\langle f_j | \hat{\theta}(y \otimes x^*) e_i \rangle = \langle f_j \otimes e_i^* | y \otimes x^* \rangle = \langle f_j | y \rangle \langle x | e_i \rangle = \langle f_j | y x^* e_i \rangle
$$
したがって$\hat{\theta}(y \otimes x^*) = y x^*$です。これは(ii)を証明します。 Q.E.D.

#### 例 1 {#evt-v-s4-n7-exa-1 .statement tag=081V}

I と J を 2 つの集合とします。上で与えられた証明により、$\ell^2(I)$から$\ell^2(J)$への写像$u$がヒルベルト・シュミット写像となる位数において、以下のような$\ell^2(J \times I)$に行列$(a_{ji})$が存在することが必要十分であり、 $\ell^2(I)$ のすべての $\xi = (\xi_i)$ に対して $u(\xi)_j = \sum_{i \in I} a_{ji} \xi_i$。

#### 例 2 {#evt-v-s4-n7-exa-2 .statement tag=081W}

\* X と Y を 2 つのハウスドルフ トポロジカル空間とし、それぞれ正の測度 $\mu$ と $\nu$ を与えます。ヒルベルト・シュミット写像が $\mathscr{L}^2(X)$ から $\mathscr{L}^2(Y)$ 対応するへ全単射的に $Y \times X$ の平方可積分関数の類になることを示すことができます。 写像 $N \in \mathscr{L}^2(Y \times X, \nu \otimes \mu)$ 対応する写像 $u_N$ の類への提供者
$$
(u_N f)(y) = \int_X N(y, x) f(x) \, d\mu(x)
$$
$\nu$-ほぼすべての$y \in Y$と$f \in \mathscr{L}^2(X, \mu)$。私たちは持っています
$$
\| u_N \|_2^2 = \int_X \int_Y |N(y, x)|^2 \, d\mu(x) \, d\nu(y) .
$$

#### 注意 1 {#evt-v-s4-n7-rem-1 .statement tag=081X}

$K = \mathbf{C}$ と仮定します。 $u$ と $v$ が $\mathscr{L}^2(E; F)$ にあるとします。 関係があります
$$
4\, u^* v = \sum_{\varepsilon^4 = 1} \overline{\varepsilon}(u + \varepsilon v)^* (u + \varepsilon v),
$$
したがって、$u^* v$ 属するから $\mathscr{L}^1(E)$ となります。ヒルバーシアン空間 $\mathscr{L}^2(E; F)$ のスカラー 積は次の式で与えられます。
$$
\langle u | v \rangle = \operatorname{Tr}(u^* v)
$$
これは、$\mathscr{L}^2(E; F)$ で公式定義するエルミート形となり、$\langle u | u \rangle = \| u \|_2^2$ になります。

$u \in \mathscr{L}^2(E; F)$ と $v \in \mathscr{L}^2(F; E)$ の場合、上記により $vu$ 属するから $\mathscr{L}^1(E)$ と $uv$ から $\mathscr{L}^1(F)$ になります。さらに、私たちは
$$
\operatorname{Tr}(uv) = \operatorname{Tr}(vu) .
$$
直線性と連続性により、$u = y_1 x_1^*$ と $v = x_2 y_2^*$ (E は $x_1, x_2$、F は $y_1, y_2$) のときにこの公式を検証するだけで十分です。しかし、$uv$ は写像 $y \mapsto y_1 \langle x_1 | x_2 \rangle \langle y_2 | y \rangle$ と $vu$ 写像 $x \mapsto x_2 \langle y_2 | y_1 \rangle \langle x_1 | x \rangle$ であり、(41) は V、p. 48 の公式 (22) から続きます。

従って、$u_1, u_2$ が $\mathscr{L}^2(E; F)$ の 2 つの元である場合、ヒルバーシアンでは空間 $\mathscr{L}^2(F; E)$ となります。
$$
\langle u_1^* | u_2^* \rangle = \operatorname{Tr}(u_1 u_2^*) = \operatorname{Tr}(u_2^* u_1) = \langle u_2 | u_1 \rangle = \overline{\langle u_1 | u_2 \rangle} ;
$$
他の語では、$u \mapsto u^*$ は、ヒルバーティアン空間 $\mathscr{L}^2(E; F)$ からヒルバーティアン空間 $\mathscr{L}^2(F; E)$ の共役 (V, p. 6) への同型です。この共役を $\mathscr{L}^2(F; E)$ (V, p. 15) の双対で同一視するとすると、$\mathscr{L}^2(E; F)$ は$\mathscr{L}^2(F; E)$ の双対と識別でき、正規の双線形形式 $(v, u) \mapsto \langle v, u \rangle$ は$(v, u) \mapsto \operatorname{Tr}(vu)$ と識別されることがわかります。

#### 注意 2 {#evt-v-s4-n7-rem-2 .statement tag=081Y}

$K = \mathbf{R}$ と仮定します。 公式 (40) と (41) が再び有効であることを検証し、$\mathscr{L}^2(E; F)$ が双線形形式 $(u, v) \mapsto \operatorname{Tr}(uv)$ によって $\mathscr{L}^2(F; E)$ の双対と識別できることを示すのは読者に任せます。

### 8. ヒルベルト・シュミットの対角化写像

#### 定理 2 {#evt-v-s4-thm-2 .statement tag=081Z}

*E と F を 2 つのヒルベルト空間とし、u を E から F へのヒルベルト・シュミット写像とする。u によって F の直交族に変換される E の正規直交基底 $(e_i)_{i \in I}$ が存在する。

B が E の (閉じた) 単位元ボールを表し、弱められた位相が割り当てられているとします。これはコンパクトな空間 (V、p. 17) です。 $x \in B$ にはすべて $Q(x) = \|u(x)\|^2$ を付けます。最後に、E 満たすのすべてのベクトル x のうちの集合を次の性質とします。

(H) *x に直交するすべての $y \in E$ に対して、E の元 $u(y)$ は $u(x)$ に直交します。*

#### 補題 4 {#evt-v-s4-lem-4 .statement tag=0820}

*写像 $Q : B \to \mathbf{R}$は連続です。*

$(f_j)_{j \in J}$ を F の正規直交値基底とします。すべての $j \in J$ に対して $\lambda_j = \|u^*(f_j)\|^2$ を代入します。 $u$ 属するから $\mathscr{L}^2(E; F)$ までは $u^* \in \mathscr{L}^2(F; E)$ なので、$\sum_j \lambda_j < +\infty$ になります。さらに、
$$
Q(x) = \|u(x)\|^2 = \sum_j |\langle u^*(f_j)|x \rangle|^2
$$
Parseval の公式 (V, p. 22) と随伴関数 (V, p. 38) の定義による。 $x \in B$、$|\langle u^*(f_j)|x \rangle|^2 \leq \lambda_j$ ごとに Cauchy-Schwarz 不等式によって作成されます。従って、公式 (43) における和の収束は B 上で一様であるため、補題 4 (GT, X, § 1, No. 6) となります。

#### 補題 5 {#evt-v-s4-lem-5 .statement tag=0821}

*$E_1$ を E のクローズドベクトル部分空間とし、$u^*u$ で安定します。 $E_1 \neq \{0\}$ の場合、$E_1 \cap P$ にはノルム 1 のベクトルが存在します。*

B は弱くコンパクトなので、B の弱く閉じた部分空間 $B \cap E_1$ も同様です。 従って、すべての $x \in B \cap E_1$ に対して $Q(x_0) \geq Q(x)$ となるように、$B \cap E_1$ には (GT, IV, § 6, No. 1, th. 1) 点 $x_0$ が存在します。 $Q(x_0) = 0$ の場合、$Q(x) = 0$ があり、すべての $x \in B \cap E_1$ に対して $u(x) = 0$ が得られます。従って、この場合、$E_1 \subset P$ と補題 5 が続きます。

ここで、$Q(x_0) > 0$、次に $x_0 \neq 0$ だとします。 ベクトル $\|x_0\|^{-1} \cdot x_0$ 属するから $B \cap E_1$ まで、
$$
Q(x_0) \geq Q(\|x_0\|^{-1} \cdot x_0) = Q(x_0)/\|x_0\|^2
$$
*つまり* $\|x_0\| = 1$。 P に対して $x_0$ 属するを証明します。 $y \in E$ を $x_0$ に直交させます。 $u(y)$ が $u(x_0)$ に直交することを証明できれば十分です。しかし、$y$ は $E_1$ のベクトルの和と $E_1$ に直交するベクトルであり、両方とも $x_0$ に直交するため ($x_0 \in E_1$ 以降)、次の 2 つのケースを考慮するだけで十分です。

a) $y$ は $E_1$ に直交します。$E_1$ は $u^*u$、$u^*u(x_0) \in E_1$ の下で安定しているため、$0 = \langle y|u^*u(x_0)\rangle = \langle u(y)|u(x_0)\rangle$ です。

b) $y$ 属する ～ $E_1$: すべての $t \in \mathbf{R}$、ベクトル $x(t) = (x_0 + ty)/\|x_0 + ty\|$ 属する ～ $B \cap E_1$。 $Q(xt) = f(t)/g(t)$ がいます
$$
f(t) = \|u(x_0)\|^2 + 2t \Re \langle u(x_0)|u(y)\rangle + t^2 \|u(y)\|^2 \\
g(t) = 1 + t^2 \|y\|^2 .
$$
$x_0$の定義を考慮すると、すべての実数$t$に対して$Q(x(0)) \geq Q(x(t))$が得られるため、$\frac{d}{dt} Q(x(t))$は$t = 0$に対して零となります。でも、$f(0) = \|u(x_0)\|^2$、$g(0) = 1$、$f'(0) = 2 \Re \langle u(x_0)|u(y)\rangle$、$g'(0) = 0$。以来
$$
\frac{d}{dt} Q(x(t)) = \frac{f'(t)\,g(t) - f(t)\,g'(t)}{g(t)^2},
$$
私たちは結論する、それは$f'(0) = 0$、つまり$\Re \langle u(x_0)|u(y)\rangle = 0$です。 $K = \mathbf{R}$、$u(x_0)$は$u(y)$と直交し、$K = \mathbf{C}$、ベクトル $iy$ 属するは$E_1$と$x_0$、したがって$\mathscr{I} \langle u(x_0)|u(y)\rangle = -\Re \langle u(x_0)|u(iy)\rangle = 0$と直交し、最後に$u(x_0)$は$u(y)$と直交します。これにより、補題 5 が証明されます。

今度はそれを証明します。 2. 適用番目。 S の 1、III, § 4, No. 5 では、V、p. 23 と同様に、$P$ に含まれる$E$ の正規直交部分集合の中で最大となる集合 $S$ が存在することがわかります。 $E_1$ を、$S$ に直交するすべてのベクトルの集合とします。 $y \in E_1$ にしましょう。 $x \in S$、ベクトル、$x$、$y$ が直交し、$S \subset P$ なので、$u(x)$ と $u(y)$ が直交であると結論するする場合、それから
$$
\langle x|u^*u(y)\rangle = \langle u(x)|u(y)\rangle = 0
$$
$u^*u(y)$は$S$と直交します。 したがって、$E_1$ は $u^*u$ の下で安定します。 $E_1 \neq \{0\}$ がある場合、$E_1 \cap P$ (補題 5) にはノルム 1 のベクトル $x$ が存在し、$S \cup \{x\}$ は $P$ に含まれる $E$ の正規直交部分集合になります。 これは、$S$ の最大値指標と矛盾します。 したがって、$E_1 = \{0\}$ と $S$ は $E$ の正規直交基底です。 Q.E.D.

#### 系 1 {#evt-v-s4-lem-5-cor-1 .statement tag=0822}

— *$v$ を、ヒルバーシアン空間 $E$ の有限トレースを持つ連続的な正の自己準同型とします。 $E$ の正規直交基底 $(e_i)_{i \in I}$ と、すべての $i \in I$ に対して $v(e_i) = \lambda_i e_i$ となるような正の実数 $(\lambda_i)_{i \in I}$ の加算可能な族が存在します。

$E$の$x, y$を$\Phi(x, y) = \langle x|v(y)\rangle$とします。 すると、$\Phi$ は $E$ に対してプラスのエルミート形になります。 (V、p. 8、必然的に) ヒルバート空間 $F$ と、$E$ の $x, y$ に対して $\Phi(x, y) = \langle u(x)|u(y)\rangle$ となるような、$E$ から $F$ への連続線形写像 $u$ が存在します。 他の語には、$v = u^*u$があります。 デフのおかげで。 9 (V、p. 52)、$u$ は、$E$ から $F$ へのヒルベルト・シュミット写像です。 までに。 2 では、ベクトル $u(e_i)$ が 2 × 2 直交となるような $E$ の正規直交基底 $(e_i)_{i \in I}$ が存在します。 $i \in I$ にしましょう。 $I$ のすべての $j \neq i$ について、
$$
\langle e_j|v(e_i)\rangle = \langle u(e_j)|u(e_i)\rangle = 0
$$

したがって、$v(e_i)$ は $e_i$ に比例し、形 $\lambda_i e_i$ になります。ここで、$\lambda_i = \langle e_i | v(e_i) \rangle$;それから

$$
\lambda_i \geqslant 0 \quad \text{and} \quad \sum_{i \in I} \lambda_i = \operatorname{Tr}(v) < + \infty .
$$

#### 系 2 {#evt-v-s4-lem-5-cor-2 .statement tag=0823}

*E をヒルバーティアン空間とします。次に、$\mathscr{L}^1(E) \subset \mathscr{L}^2(E)$.*

実数の場合簡約するをスカラーの拡大による複素数の場合に変換します。したがって、$K = \mathbf{C}$ と仮定できます。

$\mathscr{L}^2(E)$ は $\mathscr{L}(E)$ のベクトル部分空間であるため、E のすべての連続正の自己準同型 $v$ が有限トレース属するから $\mathscr{L}^2(E)$ であることを証明するだけで十分です。コルの記法付き。 1、私たちは持っています

$$
\sum_{i \in I} \| v(e_i) \|^2 = \sum_{i \in I} \lambda_i^2 \leq (\sum_i \lambda_i)^2 < + \infty .
$$

#### 系 3 {#evt-v-s4-lem-5-cor-3 .statement tag=0824}

* v を、有限トレースによるヒルバーシアン空間 E の連続正の自己準同型とします。 $v = w^2$ となり、v が w と可換となるような E の正のヒルベルト・シュミット自己準同型 w が存在します。

コルの記法付き。 1、変換ベクトル $\sum_{i \in I} \xi_i e_i$ をベクトル $\sum_i \lambda_i^{1/2} \xi_i e_i$ に加える自己準同型を考慮すれば十分です。

#### 注意 {#evt-v-s4-n8-rem-1 .statement tag=0825}

— 記法で。 2、J をすべての $i \in I$ の集合とし、$u(e_i) \neq 0$ とします。すべての $i \in J$ について、$\lambda_i = \| u(e_i) \|$ と $f_i = \lambda_i^{-1} u(e_i)$ とします。このとき、$(e_i)_{i \in J}$ (それぞれ$(f_i)_{i \in J}$) は u の初期 (それぞれ最終) 部分空間の正規直交基底であり、すべての $i \in J$ に対して $u(e_i) = \lambda_i f_i$ があり、$\sum_{i \in J} \lambda_i^2 = \| u \|_2^2$ は有限です。

### 9. 他のに対する二次方程式形のトレース

この切断では、E は実数ベクトル空間を表し、Q、H は E 上の 2 つの *正の二次方程式形* を表します。 $E \times E$ 上には 2 つの対称双線形形式 $(x, y) \mapsto \langle x | y \rangle_Q$ と $(x, y) \mapsto \langle x | y \rangle_H$ が存在します。

$$
Q(x) = \langle x | x \rangle_Q , \quad H(x) = \langle x | x \rangle_H
$$

すべての$x \in E$に。

H に関する Q の *trace を * と呼び、次のように定義される $\operatorname{Tr}(Q/H)$、実数の正の実数数を有限であるかどうかに関係なく書きます。

*a)* $H(x) = 0$と$Q(x) \neq 0$で$x \in E$が存在する場合、$\operatorname{Tr}(Q/H) = + \infty$を置きます。

*b)* それ以外の場合、$\operatorname{Tr}(Q/H)$ は、$\sum_{i=1}^m Q(x_i)$ の形式のすべての数値の集合の上限です。ここで、$(x_1, ..., x_m)$ は、$\langle x_i | x_j \rangle_H = \delta_{ij}$ (クロネッカーの記号) となるような E の要素の有限シーケンスの集合に及びます。

#### 注意 {#evt-v-s4-n9-rem-1 .statement tag=0826}

— 1) E のすべての部分空間 F について、$Q_F$ は Q から F の制限と H の $H_F$ を表します。$\operatorname{Tr}(Q_F/H_F) \leq \operatorname{Tr}(Q/H)$ と $\operatorname{Tr}(Q/H)$ はすべての数 $\operatorname{Tr}(Q_F/H_F)$ の集合の上界です。 $F$ は、$E$ のすべての有限次元ベクトル部分空間の族に及びます。

2) $E_1$ を実数ベクトル空間、$Q_1$、$H_1$ $E_1$ および$\pi : E \to E_1$ 全射線形写像上の 2 つの正の二次方程式形とします。 $Q = Q_1 \circ \pi$ と $H = H_1 \circ \pi$ の場合は、$\operatorname{Tr}(Q/H) = \operatorname{Tr}(Q_1/H_1)$ です。

#### 命題 15 {#evt-v-s4-prop-15 .statement tag=0827}

*すべての $x \in E$ に対して $H(x) = \|x\|^2$ となるような、$E$ 上に実際のヒルバーティアン空間構造が存在すると仮定します。 $\operatorname{Tr}(Q/H)$ が有限であるためには、すべての $x \in E$ に対して $Q(x) = \langle x|u(x)\rangle$ となるような、有限トレースを持つ $E$ の連続かつ正の自己準同型 $u$ が存在することが必要かつ十分です。この自己準同型 $u$ は一意であり、* を持っています

$$
\operatorname{Tr}(u) = \operatorname{Tr}(Q/H) = \sum_{i \in I} Q(e_i)
$$

*すべての正規直交値基底 $(e_i)_{i \in I}$/$E$。*

$\operatorname{Tr}(Q/H)$ が有限であると仮定します。 ノルム 1 の $x \in E$ ごとに $H(x) = 1$ があり、従って $Q(x) \leq \operatorname{Tr}(Q/H)$ になります。従って、すべての $x \in E$ に対して $Q(x) \leq \operatorname{Tr}(Q/H) \cdot \|x\|^2$、そして

$$
|\langle x|y\rangle_Q| \leq Q(x)^{1/2} Q(y)^{1/2} \leq \operatorname{Tr}(Q/H) \cdot \|x\| \cdot \|y\|
$$

コーシー・シュワルツ不等式による。従って、$E \times E$の双線形形式$(x, y) \mapsto \langle x|y\rangle_Q$は連続です。 $\langle x|y\rangle_Q = \langle x|u(y)\rangle$ となるような (V, p. 16, cor. 2) 写像 $u \in \mathscr{L}(E)$ が存在します。 $E$ の $x, y$ に対して $\langle x|y\rangle_Q = \langle y|x\rangle_Q$ があるため、$u$ はエルミートです。そして $\langle x|u(x)\rangle = Q(x) \geq 0$ であるため、$u$ は正です。

逆に、$u$ を、すべての $x \in E$ に対して $Q(x) = \langle x|u(x)\rangle$ となるように、$E$ の連続した正の自己準同型とします。それから

$$
\langle x|u(y)\rangle = \frac{1}{2}(Q(x + y) - Q(x) - Q(y)) = \langle x|y\rangle_Q,
$$

これにより、$u$ の一意性が得られます。 公式 (24') (V, p. 50) までに、

$$
\operatorname{Tr}(u) = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m \langle x_i|u(x_i)\rangle = \sup_{x_1, \ldots, x_m} \sum_{i=1}^m Q(x_i),
$$

ここで、$(x_1, \ldots, x_m)$ は、すべての有限正規直交関数の集合、$E$ の元の数列にわたる範囲です。 $\operatorname{Tr}(Q/H)$の定義により、$\operatorname{Tr}(u) = \operatorname{Tr}(Q/H)$が得られます。最後に、$E$ の各正規直交基底 $(e_i)_{i \in I}$ について、V、p. 50 の公式 (25) により $\operatorname{Tr}(u) = \sum_{i \in I} \langle e_i|u(e_i)\rangle$ が得られ、従って $\operatorname{Tr}(u) = \sum_{i \in I} Q(e_i)$ になります。

#### 注意 3 {#evt-v-s4-n9-rem-3 .statement tag=0828}

$E$ と $F$ を 2 つのヒルバーティアン空間と $v$ を、$E$ から $F$ まで必ずしも連続的ではない線形の写像とします。すべての$x \in E$を$H(x) = \|x\|^2$と$Q(x) = \|v(x)\|^2$とします。プロップから続きます。 15 $v$ は、$\operatorname{Tr}(Q/H)$ が有限である場合にのみ、$\operatorname{Tr}(Q/H) = \|v\|_2^2$ がヒルベルト・シュミット写像であることがわかります。

#### 注意 4 {#evt-v-s4-n9-rem-4 .statement tag=0829}

$E$ が有限次元であると仮定します。二次方程式形 $H$ が可逆である場合、prop. 15が該当します。 $(e_1, \ldots, e_n)$を$E$の基底とします。 $q_{ij} = \langle e_i|e_j\rangle_Q$と$h_{ij} = \langle e_i|e_j\rangle_H$を入れて、行列$q = (q_{ij})$と$h = (h_{ij})$を導入します。 $u$ を $E$ の自己準同型とし、すべての $x \in E$ に対して $Q(x) = \langle x|u(x)\rangle_H$ とします。我々は持っています

$$
\langle x|y\rangle_Q = \langle x|u(y)\rangle_H \quad (x, y \in E),
$$

したがって、E の基底 $(e_1, ..., e_n)$ に対する $u$ の行列は $h^{-1} q$ に等しい。プロップにより。 15、私たちは持っています

$$
\text{Tr}(Q/H) = \text{Tr}(h^{-1} q) = \text{Tr}(qh^{-1}) .
$$

基底 $(e_1, ..., e_n)$ が H の正規直交である場合、$h$ は位数 $n$ の単位元行列であり、次のようになります。

$$
\text{Tr}(Q/H) = \text{Tr}(q) = \sum_{i=1}^n Q(e_i) ;
$$

したがって、この場合は公式 (44) が得られます。

ここで、二次方程式形 H が可逆ではないと仮定します。 N を H の核とし、$\pi$ を E から E/N までの標準写像とします。 $H = H_1 \circ \pi$ となるような E/N 上に可逆二次方程式形 $H_1$ が存在します。 $(e_1, ..., e_n)$ を E の元の数列とし、数列 $(\pi(e_1), ..., \pi(e_m))$ が E/N の基底となり、$H_1$ の正規直交となります。 $(e_1, ..., e_n)$ を N の基底とします。すると、$(e_1, ..., e_n)$ は E の基底となり、次のようになります。

$$
H(\xi_1 e_1 + \cdots + \xi_n e_n) = \xi_1^2 + \cdots + \xi_m^2
$$

すべての実数 $\xi_1, ..., \xi_n$ に。

すべての $x \in E$、関係 $H(x) = 0$ が $Q(x) = 0$ を意味するとします。他の語では、E/N上に$Q = Q_1 \circ \pi$のような二次方程式形$Q_1$が存在すると仮定します。 注意 2 とプロップによる。 15、私たちは、

$$
\text{Tr}(Q/H) = Q(e_1) + \cdots + Q(e_m) .
$$

練習問題

### 練習問題 {#evt-v-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
