---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 2
section_title: Enveloping algebra of a Lie algebra
lang: ja
source: lie-i-iii
book_pages: 12-25, 83-85
pdf_pages: 0030-0043, 0101-0103
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF THE ENVELOPING ALGEBRA
      page: 12
      pdf_page: 30
    - "no": 2
      title: ENVELOPING ALGEBRA OF A PRODUCT OF LIE ALGEBRAS
      page: 13
      pdf_page: 31
    - "no": 3
      title: ENVELOPING ALGEBRA OF A LIE SUBALGEBRA
      page: 14
      pdf_page: 32
    - "no": 4
      title: ENVELOPING ALGEBRA OF THE OPPOSITE LIE ALGEBRA
      page: 15
      pdf_page: 33
    - "no": 5
      title: SYMMETRIC ALGEBRA OF A MODULE
      page: 16
      pdf_page: 34
    - "no": 6
      title: FILTRATION OF THE ENVELOPING ALGEBRA
      page: 17
      pdf_page: 35
    - "no": 7
      title: THE POINCARÉ–BIRKHOFF–WITT THEOREM
      page: 18
      pdf_page: 36
    - "no": 8
      title: EXTENSION OF DERIVATIONS
      page: 23
      pdf_page: 41
    - "no": 9
      title: EXTENSION OF THE BASE RING
      page: 25
      pdf_page: 43
statements: 22
exercises: 10
content_sha256: 6d51791e08cabf9171d5490d3e34f8847b83e7dc2be6cb6883dcf0c9372aa5d2
translated_from: content/en/lie/I/02_s2_enveloping_algebra_of_a_lie_algebra.md
translation_method: google
source_content_sha256: 0efee89afffa5507d5ac319dd9602df1317a1ebd3ab29f31c8942d8c7c2a2199
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 0a5518f604f46e1d40c61bdaf18822391943bfbbc020c54b6d6508cb906cc807
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。 代数/リー代数を包む

### 1. 定義の包み代数

$g$ を $K$ よりもリー代数とします。 For any associative algebra with unit element $L$ over $K$, an $\alpha$-mapping of $g$ into $L$ is a $K$-linear mapping $\sigma$ of $g$ into $L$ such that
$$
\sigma([x, y]) = \sigma(x)\sigma(y) - \sigma(y)\sigma(x) \quad (x, y \text{ in } g)
$$
(in other words a homomorphism of $g$ into the Lie algebra associated with $L$).

$L'$ が、$K$ と $\tau$ 上の単位要素を持つ別の結合代数であり、$L$ から 1 対 1 への写像である $L'$ への準同型写像である場合、$\tau \circ \sigma$ は $g$ から $L'$ への $\alpha$ 写像です。 単位元との結合代数と、普遍的な (集合理論、章 IV, § 3, no. 1) のこの代数への $g$ の $\alpha$ マッピングを探します。

#### 定義 1 {#lie-i-s2-def-1 .statement tag=09UW}

*$g$を$K$、$T$、テンソル、代数の$K$モジュール$g$と$J$、テンソルによって生成された$T$の両側理想をリー代数とします。 $x \otimes y - y \otimes x - [x, y]$ どこで $x \in g, y \in g$。連想代数 $U = T/J$ は、$g$ を包む代数と呼ばれます。 制限から$T$の標準写像の$U$への$g$は、$g$の標準写像から$U$と呼ばれます*。

$T_+$ を、位数 0 の成分が零であるテンソルの $T$ からなるの両側イデアルとします。 $T_0 = K.1$ を元の $T$ の位数の集合とします。 $U_+$ と $U_0$ を $U$ の $T_+$ と $T_0$ の標準像とします。 $J \subset T_+$ のように、分解から直和 $T = T_0 + T_+$ は、分解から直和 $U = U_0 + U_+$ を意味します。したがって、代数 $U$ は、0 および $U_0 = K.1$ とは異なる単位元を持ちます。すべての $x \in U$、$U_0$ の $x$ の成分は、$x$ の *定数項* と呼ばれます。 元と定数項零形は、$U$ の両側イデアル、つまり、$U$ の $g$ の標準像によって生成される両側イデアル $U^+$ です。

連想代数 $U$ は、$U$ の $g$ の 1 と標準像によって生成されます。

$x \in g$ と $y \in g$ の場合、$x \otimes y - y \otimes x$ と $[x, y]$ は $J$ を法とする $T$ で合同です。したがって、$\sigma_0$ が $g$ の標準写像を $U$ に表す場合、

$$
\sigma_0(x)\sigma_0(y) - \sigma_0(y)\sigma_0(x) = \sigma_0([x, y])
$$

$U$で。他の語では、$\sigma_0$ は $g$ から $U$ への $\alpha$ マッピングです。

#### 命題 1 {#lie-i-s2-prop-1 .statement tag=09UX}

*$\sigma$ を、単位元との結合代数 $L$ への $g$ の $\alpha$ マッピングとします。 $U$ から $L$ への 1 対 1 のマッピング、$\sigma = \tau \circ \sigma_0$ のような準同型性 $\tau$ が 1 つだけ存在します。ここで、$\sigma_0$ は $g$ から $U$ への正規マッピングを示します。

$\tau'$ を $T$ の一意な準同型を $L$ にすると、拡大する $\sigma$ と写像が 1 対 1 になります。次に、$g$ の $x, y$ については、

$$
\tau'(x \otimes y - y \otimes x - [x, y]) = \sigma(x)\sigma(y) - \sigma(y)\sigma(x) - \sigma([x, x]) = 0;
$$

したがって、$\tau'$は$J$ではゼロであり、$U$の準同型性$\tau$を$L$に渡すことを定義し、$\sigma = \tau \circ \sigma_0$のように1対1にマッピングします。 $\tau$ の一意性は、$\sigma_0(g)$ と 1 生成する代数 $U$ なので、明らかです。

$g'$ を、$K$ 上の別のリー代数、$U'$ を包囲する代数、および $g'$ から $U'$ への正準写像を $\sigma'_0$ とします。 $\phi$を$g$の準同型を$g'$にします。 次に、$\sigma'_0 \circ \phi$ は、$g$ から $U'$ への $\alpha$ マッピングです。したがって、$U$ の準同型 $\tilde{\phi}$ が $U'$ 写像 1 対 1 になり、図式が 1 つだけ存在します。

$$
\begin{array}{ccc}
g & \xrightarrow{\phi} & g' \\
\downarrow \sigma_0 & & \downarrow \sigma'_0 \\
U & \xleftarrow{\tilde{\phi}} & U'
\end{array}
$$

可換です。 この $U$ の準同型写像元は、定数項が $U'$ の零から元で、定数項が零です。 $g''$ が $K$ の他のリー代数で、$\phi'$ が $g'$ の $g''$ の準同型である場合、$(\phi' \circ \phi)^{\sim} = \tilde{\phi}' \circ \tilde{\phi}$ です。

### 2. 代数/積/リー代数を包み込む

$g_1, g_2$ を、$K$、$U_i$ の 2 つのリー代数を、$g_i$ の代数と $g_i$ の $\sigma_i$ 標準写像を$U_i$ ($i = 1, 2$) に包むものとします。 $g$の代数と$\sigma$標準写像を$U$に包むものを$g = g_1 \times g_2, U$とします。 $g_1$の標準単射と$g_2$は$g$に定義する $U_1$の標準準同型と$U_2$は$U$に、その像は通勤なので準同型代数 $U_1 \otimes_K U_2$ の $\phi$ を代数 $U$、写像 1 対 1 にします。

#### 命題 2 {#lie-i-s2-prop-2 .statement tag=09UY}

*準同型 $\phi$ は代数同型*

写像 $\sigma': (x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)$ ($x_1 \in g_1, x_2 \in g_2$) は、$g$ の $U_1 \otimes_K U_2$ への $\alpha$ マッピングであるため、$U$ の $U_1 \otimes_K U_2$ への (no. 1, 命題 1) 一意な準同型 $\tau$ が存在します。 写像 1 対 1、次のようになります。

$$(1)$$
$$
\sigma' = \tau \circ \sigma.
$$

ここで、$\phi \circ \tau \circ \sigma = \phi \circ \sigma' = \sigma$ と $\tau \circ \phi \circ \sigma' = \tau \circ \sigma = \sigma'$ なので、$\phi \circ \tau$ と $\tau \circ \phi$ は、それぞれ $U$ と $U_1 \otimes_K U_2$ の恒等写像になります。したがって命題です。

$U_1 \otimes_K U_2$ は、同型 $\phi$ の下で $U$ と識別されます。次に、$g$ から $U$ への標準写像は、(1) と写像によって識別されます。
$$
(x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2).
$$

同様に、$g_1, \ldots, g_n$ が包絡代数 $U_1, \ldots, U_n$ をもつ $K$ 上のリー代数である場合、$g_1 \times \cdots \times g_n$ の包絡代数 $U$ は $U_1 \otimes_K \cdots \otimes_K U_n$ と正準的に識別され、$g_1 \times \cdots \times g_n$ から $U$ への正準写像が識別されます。マッピングを使用すると:
$$
(x_1, \ldots, x_n) \mapsto \sigma_1(x_1) \otimes 1 \otimes \cdots \otimes 1 + \cdots + 1 \otimes \cdots \otimes 1 \otimes \sigma_n(x_n)
$$
($\sigma_i$は、$g_i$から$U_i$への正規マッピングを示します)。

### 3. 代数の嘘部分代数を包み込む

$g$ を $K$、$h$ 部分代数の $g$、および $\sigma, \sigma'$ 標準写像の $g, h$ をそれらを囲む代数 $U, V$ にリー代数とします。次に、$h$ の標準単射 $i$ を $g$ 定義する準同型 $\tilde{i}$ (*正規* と呼ばれます)、$V$ を $U$ にすると、$\sigma \circ i = \tilde{i} \circ \sigma'$ になります。 代数 $\tilde{i}(V)$ は 1 と $\sigma(h)$ によって生成されます。 (no. 7, 系から定理 5) は、重要な場合には $\tilde{i}$ が単射であることを見てみましょう。

$h$が$g$の理想であるとすると、$\sigma(h)$一致するによって生成された$U$の左の理想と、$\sigma(h)$によって生成された右の理想、他の語では、両側の理想$R$になります。 $x \in h$ と $x' \in g$ については、次のようになります。
$$
\sigma(x)\sigma(x') = \sigma(x')\sigma(x) + \sigma([x, x'])
$$
そして$[x, x'] \in h$。

#### 命題 3 {#lie-i-s2-prop-3 .statement tag=09UZ}

*$h$を、$g$の$g$、$p$、標準準同型を$g/h$、$W$に加え、それを囲む$g/h$の代数とします。 準同型:*
$$
\tilde{p}: U \to W
$$
*正準的に定義された$p$は全射的であり、その核は$\sigma(h)$によって生成された$U$の理想的な$R$です。

$\sigma''$ を $g/\mathfrak{h}$ の標準写像を W に変換します。可換図式:

$$
\begin{array}{ccc}
\mathfrak{h} & \xrightarrow{i} & g \\
\downarrow \sigma' & & \downarrow \sigma \\
V & \xrightarrow{\iota} & U
\end{array}
$$
$$
\begin{array}{ccc}
g & \xrightarrow{p} & g/\mathfrak{h} \\
\downarrow \sigma & & \downarrow \sigma'' \\
U & \xrightarrow{\tilde{p}} & W
\end{array}
$$

$\tilde{p}$ は $\sigma(\mathfrak{h})$ 上、つまり R 上では零であることを証明します。 $\psi$ を U/R 上の U の標準準同型とします。 U/R の準同型 $\phi$ が存在します

$$
\begin{array}{ccc}
g & \xrightarrow{p} & g/\mathfrak{h} \\
\downarrow \sigma & & \downarrow \sigma'' \\
U & \xrightarrow{\psi} & U/R
\end{array}
$$
$$
\begin{array}{ccc}
U/R & \xleftarrow{\phi'} & W \\
& \uparrow \theta & \\
& \uparrow \phi & \\
U/R & \xrightarrow{\phi} & W
\end{array}
$$

$\tilde{p} = \phi \circ \psi$ となる W に変換します。 g の U/R への写像 $\psi \circ \sigma$ は $\alpha$ マッピングであり、$\mathfrak{h}$ 上の零であるため、定義するは $\theta \circ p = \psi \circ \sigma$ となるような U/R への $g/\mathfrak{h}$ の $\theta$ $\alpha$ マッピングになります。次に$\phi \circ \theta \circ p = \phi \circ \psi \circ \sigma = \sigma'' \circ p$。したがって$\phi \circ \theta = \sigma''$です。 U/R 写像 1 対 1 に W の準同型 $\phi'$ が 1 つだけ (no. 1, 命題 1) 存在し、そのような $\theta = \phi' \circ \sigma''$ が存在します。すると$\phi' \circ \phi \circ \theta = \phi' \circ \sigma'' = \theta$と$\phi \circ \phi' \circ \sigma'' = \phi \circ \theta = \sigma''$、したがって$\phi' \circ \phi$と$\phi \circ \phi'$はそれぞれU/RとWの恒等写像になります。これで証明は完了です。

U/R は、同型 $\phi$ の下で W と識別されます。 次に、$g/\mathfrak{h}$ の W への正規写像 $\sigma''$ は $\theta$ で識別されます。つまり、商を取ることによって $\sigma$ から導出される U/R への $g/\mathfrak{h}$ の写像と識別されます。

### 4. 反対側のリー代数を代数を包み込む

$g$をKの上のリー代数、$g^0$の反対のリー代数と$\sigma$、$g$と$g^0$の$\sigma_0$標準写像を、それらを囲む代数UとVにするとします。 次に、$\sigma$ は、代数 U の反対の結合代数 $U^0$ への $g^0$ の $\alpha$ マッピングです。 したがって、$U^0$ 写像 1 対 1 に V の準同型 $\phi$ が 1 つだけ存在し、そのような $\sigma = \phi \circ \sigma_0$ が存在します。

#### 命題 4 {#lie-i-s2-prop-4 .statement tag=09V0}

*準同型 $\phi$ は、$U^0$ 上の V の同型です。

U の準同型 $\phi'$ が $V^0$ 写像 1 対 1 になり、$\sigma_0 = \phi' \circ \sigma$ が存在します。 $\phi'$は$U^0$の準同型をVにすると考えられます。すると、$\sigma_0 = \phi' \circ \phi \circ \sigma_0$と$\sigma = \phi \circ \phi' \circ \sigma$、したがって$\phi' \circ \phi$と$\phi \circ \phi'$は、VとUの恒等写像になります。したがって、命題となります。

V は、同型 $\phi$ の下で $U^0$ と識別されます。次に、$\sigma_0$ は $\sigma$ と同一視されます。

この識別では、$g$ の同型 $\theta : x \mapsto -x$ が $g^0$ 定義する同型 $\tilde{\theta}$ から $V = U^0$ に移動します。 この同型は U の反自己同型であると考えることができます。 これは U の主要な反自己同型と呼ばれます。 $x_1, \ldots, x_n$ が $g$ にある場合、次のようになります。

$$
(2) \quad \tilde{\theta}(\sigma(x_1) \ldots \sigma(x_n)) = \tilde{\theta}(\sigma(x_n)) \ldots \tilde{\theta}(\sigma(x_1)) = (-\sigma(x_n)) \ldots (-\sigma(x_1))
$$
$$
= (-1)^n \sigma(x_n) \ldots \sigma(x_1).
$$

### 5. 対称代数/加群

VをK-加群とします。 V は、可換なリー代数として独特の方法で考えることができます。 V の包絡線代数は次のように取得できます。 T を V のテンソル代数とします。 I を、テンソル $x \otimes y - y \otimes x$ ($x \in V, y \in V$) によって生成される T の両側イデアルとします。次に、形代数 $S = T/I$。

S が V の対称代数と呼ばれていること (*代数*、章 III, § 6) を思い出して、この章、証明のうち明らかに必要なプロパティを簡単にまとめます。 $T^n$ を、T の位数 n の同次テンソルの集合とします。すると、$I = (I \cap T^2) + (I \cap T^3) + \cdots$ となり、S は、$T^n$ の標準像 $S^n$ の直和となります。 $S^n$ の元は、次数 n の同次と呼ばれます。 $S^0 = K.1, S^1$ は V および $S^n S^p \subset S^{n+p}$ と識別されます。 代数 S は 1 と $S^1 = V$ によって生成されます。明らかに、$S^1$ の任意の 2 つの元は置換可能であり、したがって S は可換です。 V が基底 $(x_\lambda)_{\lambda \in \Lambda}$ の自由K-加群である場合、多項式代数 $K[X_\lambda]_{\lambda \in \Lambda}$ の標準準同型 f を S にすると、写像 1 対 1 および$X_\lambda$ から $x_\lambda$ になります。 $\lambda \in \Lambda$ は同型: S の普遍性 (no. 1, 命題 1) により、$K[X_\lambda]_{\lambda \in \Lambda}$ に S の準同型 g が存在し、すべて写像 1 対 1 および $x_\lambda$ から $X_\lambda$ になります。 $\lambda \in \Lambda$ と f と g は 1 つの他のの逆数準同型です。

${S'}^n \subset T^n$ を位数 n (*代数*, 章 III, § 5, no. 1, 定義 2) の同次対称テンソルの集合とします。 Kが特性0の体の場合、$T^n$では${S'}^n$と$I \cap T^n$が補足されます。 $(x_\lambda)_{\lambda \in \Lambda}$ を V の基底とします。 $\Lambda$ に合計順序 (*集合理論*、章 III, § 2, no. 3、定理 1) を与えます。 $\Lambda_n$ を増加するの集合数列の n 元の $\Lambda$ とします。 $M = (\lambda_1, \ldots, \lambda_n) \in \Lambda_n$ については、

$$
y_M = \frac{1}{n!} \sum_{\sigma \in S_n} x_{\lambda_{\sigma(n)}} \otimes \cdots \otimes x_{\lambda_{\sigma(n)}}.
$$

ベクトル K-space ${S'}^n$ の $M \in \Lambda_n$ 形系の生成元の $y_M$。さて、$S^n$ の標準像は、上記の段落により、$S^n$ の基底を構成します。したがって、$(y_M)_{M \in \Lambda_n}$ は、$T^n$ の $I \cap T^n$ の補足部分空間の基底 (*代数*、章 II, § 1, no. 6、命題 4) であり、主張が確立されます。

したがって、K が特性 0 の体であるとき、標準写像 $T^n \to S^n$ の制限から ${S'}^n$ は、空間 ${S'}^n$ の同型であり、空間 $S^n$ となるので、 逆同型。このようにして、空間 S の各 n 定義する標準同型に対して空間上に得られる逆同型

$$
S' = \sum_{n \geq 0} {S'}^n \text{ of symmetric tensors}.
$$

### 6. エンベロープの濾過代数

$K$ モジュール $g$ の $K$ および $T$ テンソル代数を $g$ リー代数とします。 $T^n$ を、位数 $n$ と $T_n = \sum_{i \leq n} T^i$ の同次テンソルの $T$ からなるの部分加群とします。次に、$T_n \subset T_{n+1}$、$T_0 = K.1$、$T_{-1} = \{0\}$、$T_n T_p \subset T_{n+p}$となります。

$U_n$ を、$g$ の代数 $U$ を囲む$T_n$ の標準像とします。次に、$U_n \subset U_{n+1}$、$U_0 = K.1$、$U_{-1} = \{0\}$、$U_n U_p \subset U_{n+p}$。したがって、$U$ は、*$U_n$ (*可換代数*, 章 III, § 2, no. 1) によって *フィルターされた代数として記述できます。 $U_n$の元は*濾過*の$\leq n$と言われます。

$G^n$ を $K$ モジュール $U_n / U_{n-1}$ とし、$G$ を $G^n$ の $K$ モジュール直和とします。 $U$ 定義する上の乗法、商を取ると、$G^n \times G^m$ から $G^{n+m}$ への双線形マッピング、したがって $G \times G$ から $G$ への双線形マッピング、これは結合的です。したがって、$G$ には結合的な $K$-代数構造が与えられます。それから$G^n G^m \subset G^{n+m}$。 $G^n$ の元は *次数* $n$ であると言われています。このようにして得られた等級付けされた代数は、フィルター処理された代数 $U$ (*可換代数*、章 III, § 2, no. 3) に関連付けられた等級付けされた代数です。

$\phi_n$ を正規の $K$ 線形マッピングの合成とします

$$
T^n \to U_n \to G^n.
$$

$T^n$は$T_n$の$T_{n-1}$を補足するので、$\phi_n$は全射です。 $\phi_n$ 定義するは、$\sum_n T^n = T$ の $\sum_n G^n = G$ への $K$ 線形マッピング $\phi$ です。

#### 命題 5 {#lie-i-s2-prop-5 .statement tag=09V1}

* $T$ の $G$ 上の写像 $\phi$ は、代数準同型写像 1 対 1 であり、テンソル $x \otimes y - y \otimes x$ ($x \in g, y \in g$) によって生成される両側イデアルでは零です。

$t \in T^n$ と $t' \in T^p$ の場合、$G$ の乗法の定義により $\phi(t)\phi(t') = \phi(tt')$ になります。したがって、$\phi$ は代数準同型であり、明らかに $\phi(1) = 1$ です。 $g$に$x, y$がある場合、$U_2$のこの元の$x \otimes y - y \otimes x \in T^2$と標準像は$[x, y]$の属するから$U_1$となります。したがって、$\phi(x \otimes y - y \otimes x) = 0$ となり、命題が証明されます。

$S$ を、$K$ モジュール $g$ と $T$ の $S$ 上での$\tau$ 標準準同型の対称代数とします。 命題 5 は、代数 $G$、写像上に 1 対 1 で $\phi = \omega \circ \tau$ となる、*標準* と呼ばれる代数 $S$ の一意な準同型 $\omega$ が存在することを証明します。 $\omega(S^n) = \phi(T^n) = G^n$ あります。 $\tau_n$を$\tau$から$T^n$の制限、$\omega$から$S^n$の$\omega_n$制限、$T^n$の$\psi_n$標準写像とします。 $U_n$ の $U_n$ と $\theta_n$ 標準写像が $G^n$ に。 $\omega_n$ の定義は、次の図式が可換であることを証明します。

$$
\begin{array}{ccccc}
T^n & \xrightarrow{\psi_n} & U_n & \xrightarrow{\theta_n} & G^n \\
& \searrow & & \swarrow & \\
& & S^n & \xrightarrow{\omega_n} &
\end{array}
$$

#### 命題 6 {#lie-i-s2-prop-6 .statement tag=09V2}

*K がネーター で、g が有限生成加群の場合、環 U は正しく、左ネーター です。*

S は K 上で有限生成された代数であるため、ネーター 環 (*可換代数*, 章 III, § 2, no. 10, 系 3 ～ 定理 2)。したがって、S の商環と同型の G はネーター です。したがって、U は正しく、左ネーター (*可換代数*, 章 III, § 2, no. 10, *注意 2*) です。

#### 系 {#lie-i-s2-n6-cor-1 .statement tag=09V3}

*K が体で、g が K 上の有限次元であると仮定します。I₁, ..., Iₘ を U の有限余次元の右 (それぞれ左) イデアルとします。すると、積イデアルになります。 I₁I₂...Iₘ は有限余次元のものです。*

帰納法までに、たとえば 2 つの正しい理想の場合を考えるだけで十分です。右側の U モジュール I₁ は、元 u₁, ..., uₚ (命題 6) の有限数によって生成されます。 v₁, ..., vₐ を、I₂ 生成するベクトル空間 U/I₂ を法とする類 U の元とします。次に、uᵢvⱼ 生成するベクトル空間 I₁/I₁I₂ の I₁/I₁I₂ の標準像です。有限次元。したがって、dim_K(U/I₁I₂) = dim_K(U/I₁) + dim_K(I₁/I₁I₂) < +∞。

#### 注意 {#lie-i-s2-n6-rem-1 .statement tag=09V4}

g' を環 K 上の他のリー代数とし、U' を包む代数、濾過 $\leq n$ の U' の元の U'_n 集合と U^n (それぞれ U'^n) とします。 位数 n の同次対称テンソルの g (それぞれ g') の U (それぞれ U') における標準像の集合。 $\eta$ を g から g' への準同型とし、$\tilde{\eta}$ を U から U' への対応する準同型とします。それから

$$
\tilde{\eta}(U_n) \subset U'_n, \quad \tilde{\eta}(U^n) \subset {U'}^n.
$$

特に、U の主要な反自己同型性により、U_n と U^n は安定したままになります。 K-線型写像の T^n がそれ自体に写像

$$
x_1 \otimes x_2 \otimes \cdots \otimes x_n \quad \text{to} \quad x_n \otimes x_{n-1} \otimes \cdots \otimes x_1
$$

g のすべての $x_1, ..., x_n$ は対称演算子であるため、位数 n の同次対称テンソルは固定されたままになります。したがって、比 $(-1)^n$ の各 U^n ホモテティー に対する U 誘導するの主反自己同型性が成り立ちます。

### 7. ポアンカレ – ビルコフ – ウィット定理

#### 定理 1 {#lie-i-s2-thm-1 .statement tag=09V5}

*g を嘘 K-代数、U を包み込む代数、G をフィルタリングされた代数 U に関連付けられた段階的な代数、S を K-加群の対称代数とする。 g が自由K-加群の場合、標準準同型 $\omega : S \to G$ は同型となります。*

$(x_\lambda)_{\lambda \in \Lambda}$ を K-加群 g の基底とします。 $\Lambda$ に合計順序 (*集合理論*, 章 III, § 2, no. 3, 定理 1) を与えます。 P を、$x_\lambda$ と 1 対 1 対応の不定変数 $z_\lambda$ における多項式代数 $K[z_\lambda]_{\lambda \in \Lambda}$ とします。 $\Lambda$ の元のすべての数列 $M = (\lambda_1, \lambda_2, ..., \lambda_n)$ について、$z_M$ が単項式 $z_{\lambda_1}z_{\lambda_2}...z_{\lambda_n}$ と $x_M$ テンソル $x_{\lambda_1} \otimes x_{\lambda_2} \otimes \cdots \otimes x_{\lambda_n}$ を表すものとします。

K-加群 P の M 増加する、形基底の $z_M$ ($\varnothing$ は増加する数列であり、$z_\varnothing = 1$ であるという慣例を作ります)。 $P_p$ を次数 $\leq p$ の多項式の部分加群とします。まずいくつかの補題を証明します。 (省略すると、数列 M の添字 $\mu$ ごとに $\lambda \leq \mu$ なら $\lambda \leq M$ と書きます。)

#### 補題 1 {#lie-i-s2-lem-1 .statement tag=09V6}

*すべての整数 $p \geq 0$ に対して、K-加群 P 満たすには、次の条件に K-加群 $g \otimes_K P_p$ の一意な準同型 $f_p$ が存在します。
$$
\begin{align*}
(A_p) \quad & f_p(x_\lambda \otimes z_M) = z_\lambda z_M \quad \text{for } \lambda \leq M, z_M \in P_p; \\
(B_p) \quad & f_p(x_\lambda \otimes z_M) - z_\lambda z_M \in P_q \quad \text{for } z_M \in P_q, q \leq p; \\
(C_p) \quad & f_p(x_\lambda \otimes f_p(x_\mu \otimes z_N)) = f_p(x_\mu \otimes f_p(x_\lambda \otimes z_N)) + f_p([x_\lambda, x_\mu] \otimes z_N)
\end{align*}
$$
*$z_N \in P_{p-1}$用。 ((C_p)に出現する項は(B_p)によって意味を持ちます。)*

さらに$f_p$の制限が$f_{p-1}$で$g \otimes P_{p-1}$一致するに。

$f_p$ から $g \otimes_K P_{p-1}$ までの制限は条件 (A_{p-1})、(B_{p-1})、(C_{p-1}) を満たすため、最後の主張は他の結果から続きます。 $p$の帰納法までに$f_p$の存在と一意性を証明します。 $p = 0$ の場合、条件 (A_0) は $f_0(x_\lambda \otimes 1) = z_\lambda$ を与え、条件 (B_0) と (C_0) は明らかに満たされます。今、$f_{p-1}$の存在と一意性が証明されたとします。 $f_{p-1}$ は一意の拡大 $f_p$ から $g \otimes_K P_p$ 満たす条件 (A_p)、(B_p)、および (C_p) を許容することを示します。

$p$ 元の増加する数列 M に対して定義する $f_p(x_\lambda \otimes z_M)$ を必要とします。

$\lambda \leq M$の場合、値は条件で与えられます(A_p)。それ以外の場合、M は $\mu < \lambda, \mu \leq N$ である形 ($\mu, N$) に一意に書くことができます。それから
$$
z_M = z_\mu z_N = f_{p-1}(x_\mu \otimes z_N)
$$
(A_{p-1}) によって、(C_p) の左辺は $f_p(x_\lambda \otimes z_M)$ になります。これで、(C_p) の右側はすでに定義されています。(B_{p-1}) では次のように書くことができます。
$$
f_p(x_\lambda \otimes z_N) = f_{p-1}(x_\lambda \otimes z_N) = z_\lambda z_N + w
$$
ここで$w \in P_{p-1}$;したがって、(C_p) の右辺は次のようになります。
$$
z_\lambda z_\mu z_N + f_{p-1}(x_\mu \otimes w) + f_{p-1}([x_\lambda, x_\mu] \otimes z_N).
$$

したがって、$f_p$ は一意に定義され、明らかに条件 (A_p) と (B_p) を満たします。 $\mu < \lambda, \mu \leq N$ であれば、条件 (C_p) が満たされます。 $[x_\mu, x_\lambda] = -[x_\lambda, x_\mu]$と同様に、$\lambda < \mu, \lambda \leq N$に対して条件(C_p)も満たされます。 (C_p) は $\lambda = \mu$ について自明に満たされるため、(C_p) は $\lambda \leq N$ または $\mu \leq N$ の場合に満たされます。これらの不等式がいずれも当てはまらない場合、$N = (\nu, Q)$、ここで $\nu \leq Q, \nu < \lambda, \nu < \mu$ となります。今後、$f_p(x \otimes z) = xz$ を $x \in g$ および $z \in P_p$ と略記すると、帰納法の仮定までに次のようになります。
$$
x_\mu z_N = x_\mu(x_\nu z_Q) = x_\nu(x_\mu z_Q) + [x_\mu, x_\nu]z_Q.
$$

ここで、$z_\mu z_Q$ は形 $z_\mu z_Q + w$ であり、$w \in P_{p-2}$ です。 (C_p) は、$\nu \leq Q$ と $\nu < \mu$ から $x_\lambda(x_\nu(z_\mu z_Q))$ に適用でき、帰納法の仮定までに $x_\lambda(x_\nu w)$ に適用できるため、$x_\lambda(x_\nu(x_\mu z_Q))$ にも適用できます。したがって、次のようになります。
$$
x_\lambda(x_\mu z_N) = x_\nu(x_\lambda(x_\mu z_Q)) + [x_\lambda, x_\nu](x_\mu z_Q) + [x_\mu, x_\nu](x_\lambda z_Q)
+ [x_\lambda, [x_\mu, x_\nu]]z_Q.
$$

$\lambda$ と $\mu$ を交換して減算すると、次のようになります。

$$
x_{\lambda}(x_{\mu}z_{N}) - x_{\mu}(x_{\lambda}z_{N}) = x_{v}(x_{\lambda}(x_{\mu}z_{Q}) - x_{\mu}(x_{\lambda}z_{Q}))
+ [x_{\lambda}, [x_{\mu}, x_{v}]]z_{Q} - [x_{\mu}, [x_{\lambda}, x_{v}]]z_{Q}
= x_{v}([x_{\lambda}, x_{\mu}]z_{Q}) + [x_{\lambda}, [x_{\mu}, x_{v}]]z_{Q} + [x_{\mu}, [x_{v}, x_{\lambda}]]z_{Q}
= [x_{\lambda}, x_{\mu}](x_{v}z_{Q}) + ([x_{v}, [x_{\lambda}, x_{\mu}]]
+ [x_{\lambda}, [x_{\mu}, x_{v}]] + [x_{\mu}, [x_{v}, x_{\lambda}]])z_{Q}
$$

したがって、ヤコビのアイデンティティによって

$$
x_{\lambda}(x_{\mu}z_{N}) - x_{\mu}(x_{\lambda}z_{N}) = [x_{\lambda}, x_{\mu}]z_{N}
$$

これで補題 1 の証明が完成します。

#### 補題 2 {#lie-i-s2-lem-2 .statement tag=09V7}

*次のような $g$ から $\mathscr{L}_{K}(P)$ への $\alpha$ マッピング $\sigma$ が存在します。

(1) $\lambda \leq M$ の場合は $\sigma(x_{\lambda})z_{M} = z_{\lambda}z_{M}$;
(2) $M$ に $p$ 元がある場合、$\sigma(x_{\lambda})z_{M} \equiv z_{\lambda}z_{M}$ (修正 $P_{p}$)。

補題 1 までに、$p$、条件 (A$_{p}$)、(B$_{p}$) に対して、K-加群 $g \otimes_{K} P_{p}$ の $P$ 満たすに準同型 $f$ が存在します。 (C$_{p}$) ($f_{p}$ は $f$ に置き換えられます)。この準同型定義する準同型 $\sigma$ の K-加群 $g$ から K-加群 $\mathscr{L}_{K}(P)$ および $\sigma$ は、条件のため、$\alpha$ マッピングになります。 (C$_{p}$)。最後に、$\sigma$ は、条件 (A$_{p}$) と (B$_{p}$) により、補題の特性 (1) と (2) を満たします。

#### 補題 3 {#lie-i-s2-lem-3 .statement tag=09V8}

※$t$を$T_{n} \cap J$のテンソルとします。 位数 $n$ の $t$ の同次成分 $t_{n}$ は、標準準同型 $T \to S$ の核 $I$ にあります。

形 $\sum_{i=1}^{r} x_{M_{i}}$ に $t_{n}$ と書きます。ここで、$M_{i}$ は $n$ の数列 $\Lambda$ の元です。 写像 $\sigma$ 拡大するから準同型の代数 $T$ を代数 $\mathscr{L}_{K}(P)$ ($\sigma$ とも表記します)、つまり $J$ の零です。 補題 2 により、$\sigma(t) . 1$ は、最高次数の項が $\sum_{i=1}^{r} z_{M_{i}}$ となる多項式になります。 $t \in J$、$\sigma(t) = 0$、したがって $P$ では $\sum_{i=1}^{r} z_{M_{i}} = 0$ となります。 $g$ には基底 $(x_{\lambda})$ があるため、$P$ は正規的に $S$ と識別されます。したがって、$S$の$t_{n}$の標準像は零、つまり$t_{n} \in I$です。

これで、定理 1 を証明できます。$G$ に対する $S$ の標準準同型が単射であることを証明する必要があります。他の語において、$t \in T^{n}$と$\psi$が$U$に対する$T$の標準準同型を表す場合、条件$\psi(t) \in U_{n-1}$が$t \in I$を暗示していることを示す必要があります。ここで、$\psi(t) \in U_{n-1}$ は、$t - t' \in J$ となるテンソル $t' \in T_{n-1}$ が存在することを意味します。 テンソル $t - t'$ は、$t$ を位数 $n$ の同次成分として認め、したがって補題により $t \in I$ を認めます。

#### 系 1 {#lie-i-s2-lem-3-cor-1 .statement tag=09V9}

*$g$ が無料の $K$ モジュールであると仮定します。 $W$ を $T^{n}$ のサブ K モジュールとします。*

*もし、図式* (3) の記法で、* $\tau_n$ *to* $W$ の *制限 * が * $W$ * に * $S^n$ の同型である場合、 *そして * の制限 $\psi_n$ *to* $W$ *は $W$ の同型 * $U_{n-1}$ * $U_n$ の補充です。

$\omega_n \circ \tau_n$の$W$への制限は、$W$の$G^n$への全単射です。 制限 $\theta_n \circ \psi_n$ から $W$ も同様です。したがって系です。

#### 系 2 {#lie-i-s2-lem-3-cor-2 .statement tag=09VA}

*$g$ が自由K-加群の場合、$g$ を囲む代数への標準写像は単射です。*

これは、系 1 が $W = T^1$ を取ることから続きます。

$g$が自由K-加群の場合（特にKが体の場合）、$g$は$g$の標準写像の下で$U$の部分加群と同一視され、$U$になります。この規約は、次の系以降から採用されます。

#### 系 3 {#lie-i-s2-lem-3-cor-3 .statement tag=09VB}

*$g$ が、エンベロープ代数 $U$ の完全に順序付けられた基底 $(x_\lambda)_{\lambda \in \Lambda}$、元 $x_{\lambda_1} x_{\lambda_2} \ldots x_{\lambda_n}$ を認める場合、$(\lambda_1, \ldots, \lambda_n)$ は、任意の増加する有限列です。 元/$\Lambda$、形基底/K-加群 $U$。*

$\Lambda_n$ を増加するの集合 $n$ の数列 $\Lambda$ の元とします。 $M = (\lambda_1, \ldots, \lambda_n) \in \Lambda_n$ の場合は、$y_M = x_{\lambda_1} \otimes x_{\lambda_2} \otimes \cdots \otimes x_{\lambda_n}$ にします。 $W$ を $T^n$ の部分加群と基底 $(y_M)_{M \in \Lambda_n}$ とします。 系 1 は、$\psi_n$ から $W$ の制限が $U_n$ の $U_{n-1}$ の補充に$W$ の同型であることを示します。しかし

$$
\psi_n(y_M) = x_{\lambda_1} x_{\lambda_2} \ldots x_{\lambda_n},
$$

よって系。

#### 系 4 {#lie-i-s2-lem-3-cor-4 .statement tag=09VC}

*${S'}^n \subset T^n$を位数nの同次対称テンソルの集合とします。 K が特性 0 の体であるとします。その場合、標準写像* の合成写像

$$
S^n \to {S'}^n \to U_n
$$

*は $U_n$ の $U_{n-1}$ の補充にベクトル空間 $S^n$ の同型が入ります。*

これは、系 1 が $W = {S'}^n$ を取ることから続きます。

今後、K が特性 0 の体であると仮定します。$\eta_n$ を、先ほど定義した $U_n$ の $S^n$ の写像とします。 $U^n = \eta_n(S^n)$ にしましょう。 ベクトル空間 $U$ は、$U^n$ の直和です。 ベクトル空間 $S = \sum_n S^n$ のベクトル空間 $U = \sum_n U^n$ への $\eta_n$ 定義する同型 $\eta$ は、S の U* への *標準同型と呼ばれます。これは*ではありません* 代数同型。可換図式があります:

$$
\begin{array}{ccccc}
& & U^n & & \\
& \nearrow \psi_n & \uparrow \eta_n & \searrow \theta_n & \\
{S'}^n & & & & G^n \\
& \searrow \tau_n & & \nearrow \omega_n & \\
& & S^n & &
\end{array}
$$

ここで、各矢印はベクトル空間同型を表します。 $g$、$\eta_n$、写像、積、$x_1 x_2 \ldots x_n$に$x_1, x_2, \ldots, x_n$が入っている場合、$S$で計算して元まで

$$
\frac{1}{n!} \sum_{\sigma \in S_n} x_{\sigma(1)} x_{\sigma(2)} \cdots x_{\sigma(n)}
$$

$U$ で計算されます。

#### 系 5 {#lie-i-s2-lem-3-cor-5 .statement tag=09VD}

*$h$をリー代数$g$の部分代数と、それを囲む代数を$U'$とします。 $K$ モジュール $h$ と $g/h$ が空いていると仮定します (たとえば、$K$ が体の場合)。 $(x_\alpha)_{\alpha \in L}$ を $h$ の基底とし、$(y_\beta)_{\beta \in M}$ を $g$ の元の家族、その標準像が $g/h$ 形 $g/h$ の基底であるとします。

(a) *$U'$の$U$への標準準同型は単射です*。

(b) *$M$ が完全に順序付けされている場合、元 $y_{\beta_1} \ldots y_{\beta_q}$、ここで、$U$ の $\beta_1 \leq \cdots \leq \beta_q$、形基底は、$U'$ の左または右加群とみなされます。

$L$ のすべての元が $M$ のすべての元よりも小さくなるように、$L \cup M$ に合計順序を与えます。 元 $x_{\alpha_1} x_{\alpha_2} \ldots x_{\alpha_p}$ は、$U'$ (系 3) の $U'$ ($\alpha_1 \leq \cdots \leq \alpha_p$) 形基底で計算されます。 元

$$
x_{\alpha_1} \ldots x_{\alpha_p} y_{\beta_1} \ldots y_{\beta_q}
$$

$U$ の形基底も同様に $U$ ($\alpha_1 \leq \cdots \leq \alpha_p \leq \beta_1 \leq \cdots \leq \beta_q$ のところ) で計算されます。 したがって、$U'$ の $U$ への正準準同型性は、$U'$ の基底の要素を $U$ の線形独立要素にマッピングするため、単射的です。 さらに、$U$ の$y_{\beta_1} \ldots y_{\beta_q}$ ($\beta_1 \leq \cdots \leq \beta_q$) 形基底が左$U'$ モジュールと見なされていることがわかります。 $M$ のすべての元が $L$ のすべての元よりも小さくなるように $L \cup M$ を順序付けると、同様に、$U$ の $y_{\beta_1} \ldots y_{\beta_q}$ ($\beta_1 \leq \cdots \leq \beta_q$) 形基底が権利とみなされます。 $U'$-モジュール。

系 5 の条件では、$U'$ は、$h$ によって $U'$ の標準準同型によって $U$ に生成された $U$ の部分代数と識別されます。

#### 系 6 {#lie-i-s2-lem-3-cor-6 .statement tag=09VE}

*$K$ モジュール $g$ が部分代数 $g_1, g_2, \ldots, g_n$ の直和であり、各 $g_i$ が空き $K$ モジュールであると仮定します。 $U_i$ を $g_i$ ($1 \leq i \leq n$) を囲む代数とします。 $\phi$ を、$U_1 \times \cdots \times U_n$ から $U$ への多重線形写像 $(u_1, \ldots, u_n) \mapsto u_1 \ldots u_n$ によって定義された $K$ モジュール $U_1 \otimes_K \cdots \otimes_K U_n$ から $U$ への $K$ 線形写像とします。この場合、$\phi$ は $K$ モジュール同型です。*

$(x^i_{\lambda})_{\lambda \in L_i}$ を $g_i$ の基底とします。合計位数 $L_1 \cup \cdots \cup L_n$ なので、$L_i$ のすべての元が $i \geq j$ の $L_j$ のすべての元を超えます。次に元:

$$
(x^1_{\lambda_1} x^1_{\lambda_2} \ldots x^1_{\lambda_p}) \otimes \cdots \otimes (x^n_{v_1} x^n_{v_2} \ldots x^n_{v_q}),
$$

ここで、$\lambda_1 \leq \lambda_2 \leq \cdots \leq \lambda_p \leq \cdots \leq v_1 \leq v_2 \leq \cdots \leq v_q$ は、$U_1 \otimes_K \cdots \otimes_K U_n$ の基底を構成します。それらは $\phi$ から元によってマッピングされます。

$$
x^1_{\lambda_1} x^1_{\lambda_2} \ldots x^1_{\lambda_p} \ldots x^n_{v_1} x^n_{v_2} \ldots x^n_{v_q}
$$

$U$ の基底を構成します。したがって系です。

#### 系 7 {#lie-i-s2-lem-3-cor-7 .statement tag=09VF}

*K が整域で、g が自由K-加群の場合、代数 U には零の因子がありません。*

G は K (定理 1) 上の多項式代数と同型であるため、整域 (*代数*, 章 IV, § 1, no. 4, 定理 1) です。したがって、系 (*可換代数*、章 III, § 2, no. 3、命題 1) となります。

### 8. 導分中拡大

#### 補題 4 {#lie-i-s2-lem-4 .statement tag=09VG}

*VをK-加群、TをVのテンソル代数とします。あなたをVの自己準同型にしましょう。 拡大する u である T の導分は 1 つだけ存在します。この導分は T 上の対称演算子と可換です。*

F = V × V × ... × V (n 因子) とします。 写像
$$
(x_1, \ldots, x_n) \mapsto ux_1 \otimes x_2 \otimes \cdots \otimes x_n \\
+ x_1 \otimes ux_2 \otimes \cdots \otimes x_n + \cdots + x_1 \otimes x_2 \otimes \cdots \otimes ux_n
$$
F の $\bigotimes^n V$ への変換は多重線形です。したがって、次のような $\bigotimes^n V$ の自己準同型 $u_n$ が存在します。
$$
u_n(x_1 \otimes \cdots \otimes x_n) = ux_1 \otimes \cdots \otimes x_n + \cdots + x_1 \otimes \cdots \otimes ux_n
$$
V のすべての $x_1, \ldots, x_n$ に対して。次に$u_1 = u$。 v を K-加群 T の自己準同型とし、各 $T^n = \bigotimes^n V$ には $u_n$ が付き一致するで、$T^0 = K.1$ には零です。 v が T の導分であることを示します。 $x_1, \ldots, x_n, y_1, \ldots, y_p$ が V の元である場合、
$$
v((x_1 \otimes \cdots \otimes x_n) \otimes (y_1 \otimes \cdots \otimes y_p)) \\
= \sum_{i=1}^n x_1 \otimes \cdots \otimes x_{i-1} \otimes ux_i \otimes x_{i+1} \otimes \cdots \otimes x_n \otimes y_1 \otimes \cdots \otimes y_p \\
+ \sum_{j=1}^p x_1 \otimes \cdots \otimes x_n \otimes y_1 \otimes \cdots \otimes y_{j-1} \otimes uy_j \otimes y_{j+1} \otimes \cdots \otimes y_p \\
= v(x_1 \otimes \cdots \otimes x_n) \otimes (y_1 \otimes \cdots \otimes y_p) + (x_1 \otimes \cdots \otimes x_n) \otimes v(y_1 \otimes \cdots \otimes y_p).
$$
線形性により、v は導分であることがわかります。 v の一意性は明らかです。最後に、明らかに $u_n$ は、$\bigotimes^n V$、よって最後の主張のすべての対称演算子と交換します。

#### 命題 7 {#lie-i-s2-prop-7 .statement tag=09VH}

* g をリー代数とし、U を包む代数、g の σ 標準写像を U に、D 導分を g とします。*
(a) *$\sigma \circ D = D_U \circ \sigma$ となる U の導分 $D_U$ は 1 つだけ存在します (つまり、g が σ の下で U の部分加群と同一視できる場合、$D_U$ 拡大する D になります)。
(b) $D_U$ は、g 上の位数 n の同次対称テンソルの U で、像の$U_n$ と集合 $U^n$ を安定に残します。

(c) $D_U$ は、$U$ の主反自己同型と可換です。

(d) *$D$ が $g$ の元 $x$ によって定義される $g$ の内部導分である場合、$D_U$ は $\sigma(x)$ によって定義される $U$ の内部導分です。

$D_T$ を、$D$ を拡張する $g$ のテンソル代数 $T$ の導出とします (補題 4)。 によって生成される$T$の両面の理想$J$

$$
x \otimes y - y \otimes x - [x, y]
$$

$g$ の $(x, y$) は $D_T$ で安定しています。のために：

$$
D_T(x \otimes y - y \otimes x - [x, y]) = Dx \otimes y - y \otimes Dx - [Dx, y]
$$
$$
+ x \otimes Dy - Dy \otimes x - [x, Dy].
$$

移行から商では、$D_T$ 定義する導分 $U$ の $D_U$ は $\sigma \circ D = D_U \circ \sigma$ になります。 $D_U$の一意性は、1から明らか、$\sigma(g)$生成する代数$U$です。 主張 (b) は明らかです。 $A$ を $U$ の主反自己同型とする。ここで (c) を証明します。 $x_1, \ldots, x_n$ が $g$ にある場合、

$$
D_U A(\sigma(x_1) \ldots \sigma(x_n)) = D_U((-1)^n \sigma(x_n) \ldots \sigma(x_1))
$$
$$
= (-1)^n \sum_{i=1}^n \sigma(x_n) \ldots D_U(\sigma(x_i)) \ldots \sigma(x_1)
$$
$$
= (-1)^n \sum_{i=1}^n \sigma(x_n) \ldots \sigma(Dx_i) \ldots \sigma(x_1)
$$
$$
= A \left( \sum_{i=1}^n \sigma(x_1) \ldots \sigma(Dx_i) \ldots \sigma(x_n) \right)
$$
$$
= AD_U(\sigma(x_1) \ldots \sigma(x_n)).
$$

最後に$x \in g$とします。 $\Delta$ を $U$ の内部導分 $y \mapsto \sigma(x)y - y\sigma(x)$ とします (*代数*, 章 IV, § 4, no. 3, *例 2*)。次に、$x' \in g$については、

$$
(\Delta \circ \sigma)(x') = \sigma(x)\sigma(x') - \sigma(x')\sigma(x) = \sigma([x, x']) = (\sigma \circ \mathrm{ad}\, x)(x'),
$$

よって $\Delta \circ \sigma = \sigma \circ \mathrm{ad}\, x$。これで証明は完了です。

適用命題 7 を可換リー代数の場合に当てはめると、$K$ モジュールのすべての自己準同型 $u$ は、この加群の対称代数の導分に一意に拡張できることがわかります。この導分はテンソル代数の導分から移行から商に拡大する$u$が導出されます。

再び $K$ にリー代数 $g$ を加え、$D$ を $g$ の導分とします。 以前の記法 $T, S, U, G$ を使用します。 $D_T, D_S$ を拡大する $D$ である $T, S$ の導分とし、$D_U$ を $\sigma \circ D = D_U \circ \sigma$ となる$U$ の一意の導分とします。 $D_U$ は $U_n$ 安定を離れるので、$G$ の商導分 $D_G$ を取って $D_U$ 定義するになります。 移行から商のとき、$D_T$ から $D_U$ と $D_S$ が導出されることから、可換図式 (3) は、no. 6 で定義された準同型 $\omega$ によって $D_S$ から $D_G$ も導出できることを証明します。 さらに$K$が特性0の体であれば、図式の同型 (4) 写像が$D_T, D_S, D_U, D_G$～${S'}^n, S^n, U^n, G^n$の他の制限に1となります。 したがって、$S$ の標準同型は $U$ 写像 $D_S$ から $D_U$ になります。

### 9. 拡大/基底環

$g$を$K$のリー代数、$T$をそのテンソル代数、$J$を$x \otimes y - y \otimes x - [x, y]$（$g$の$x, y$）と$U = T/J$によって生成された$T$の両面理想とします。 $K_1$を単位元と$K$の$\sigma$準同型を$K_1$写像1対1で可換環とします。 次に、$g_{(K_1)}$ のテンソル代数は正規的に $T_{(K_1)}$ と識別されます。 Let $J'$ be the two-sided ideal of $T_{(K_1)}$ generated by the

$$
x' \otimes y' - y' \otimes x' - [x', y']
$$

($g_{(K_1)}$の$x', y'$)。 $T_{(K_1)}$の$J_{(K_1)}$の標準像が$J'$に含まれていることは明らかです。それが$J'$と等しいことを確認するには、$x'$と$y'$が$g_{(K_1)}$、$x' \otimes y' - y' \otimes x' - [x', y']$属するからこの像の2つの元を表すことを示せば十分です。今

$$
x' = \sum_i x_i \otimes \lambda_i, y' = \sum_j y_j \otimes \mu_j \quad (x_i, y_j \text{ in } g, \lambda_i, \mu_j \text{ in } K_1);
$$

よって

$$
x' \otimes y' - y' \otimes x' - [x', y'] = \sum_{i,j} (x_i \otimes y_j - y_j \otimes x_i - [x_i, y_j]) \otimes \lambda_i \mu_j
$$

それは私たちの主張を証明します。次に、$U_{(K_1)} = (T/J)_{(K_1)}$ は $T_{(K_1)}/J'$ と正規的に識別されることがわかります。 * $g_{(K_1)}$ の代数を包含するものは $U_{(K_1)}$* と正規的に識別され、$g_{(K_1)}$ の標準写像をその包含代数に包含するものは、 で識別されます。 $\sigma \otimes 1$ ($\sigma$ は、$g$ の $U$ への標準写像を表します)。

### 練習問題 {#lie-i-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
