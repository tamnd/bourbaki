---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: I
chapter_title: Lie Algebras
section: 3
section_title: Representations
lang: ja
source: lie-i-iii
book_pages: 25-38, 85-91
pdf_pages: 0043-0056, 0103-0109
extraction: ocr
subsections:
    - "no": 1
      title: REPRESENTATIONS
      page: 25
      pdf_page: 43
    - "no": 2
      title: TENSOR PRODUCT OF REPRESENTATIONS
      page: 28
      pdf_page: 46
    - "no": 3
      title: REPRESENTATIONS ON HOMOMORPHISM MODULES
      page: 29
      pdf_page: 47
    - "no": 4
      title: EXAMPLES
      page: 31
      pdf_page: 49
    - "no": 5
      title: INVARIANT ELEMENTS
      page: 32
      pdf_page: 50
    - "no": 6
      title: INVARIANT BILINEAR FORMS
      page: 33
      pdf_page: 51
    - "no": 7
      title: CASIMIR ELEMENT
      page: 35
      pdf_page: 53
    - "no": 8
      title: EXTENSION OF THE BASE RING
      page: 36
      pdf_page: 54
statements: 24
exercises: 12
content_sha256: 649487443c3adfde51663f794fdaab106b4ee75feb98021bcbc287071cfe31cd
translated_from: content/en/lie/I/03_s3_representations.md
translation_method: google
source_content_sha256: a021ec46ba121f306f571608589128b59fe9512dee7105b93f2d9f49b1ae24bd
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 20cc1f06100c0fd42d6992c17a7bd9698bdec4a5f84588e535cfbc007c37c2ad
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。 表現

### 1. 表現

#### 定義 1 {#lie-i-s3-def-1 .statement tag=09VS}

*$g$ を $K$ 上のリー代数とし、$M$ を $K$ モジュールとします。 $g$の準同型からリー代数$gl(M)$は、加群$M$の$g$の表現と呼ばれます。単射詞表現は忠実と呼ばれます。 $K$ が体の場合、$K$ を超える $M$ の次元 (有限または無限) は、表現の次元と呼ばれます。 $K$ モジュール $g$ の $g$ の表現 $x \mapsto \operatorname{ad} x$ は、$g$ の随伴物表現と呼ばれます。*

したがって、$M$ 上の $g$ の表現は、$g$ の $\rho$ から $M$ の自己準同型加群への $K$ 線形マッピングです。

$$
\rho([x, y]) \cdot m = \rho(x) \rho(y) \cdot m - \rho(y) \rho(x) \cdot m
$$

すべての$x \in g, y \in g, m \in M$に。

#### 例 {#lie-i-s3-n1-exa-1 .statement tag=09VT}

G を実リー群、g をそのリー代数とし、θ を有限次元実数ベクトル空間 E 上の G の解析表現とします。すると、g の gl(E) への対応する準同型は、E 上の g の表現になります。

U を g を包む代数とします。 Proposition 1 of § 2, no. 1 defines a one-to-one correspondence between the set of representations of g on M and the set of representations of U on M. 一方、結合代数 U の表現と左 U モジュールの概念の間に同値があることが (代数, 章 VIII, § 13, no. 1) わかります。

#### 定義 2 {#lie-i-s3-def-2 .statement tag=09VU}

*g を K と U の上でリー代数とし、それを囲む代数とします。 U 上のユニタリ左加群は、左 g モジュール、または単に g モジュールと呼ばれます。*

M が g モジュールで x ∈ U の場合、x_M は x によって定義される M のホモテティー (cf. 代数, 章 VIII, § 1, no. 2) を表します。

U 上の単一右加群は右 g 加群と呼ばれます。このような加群は左 U^0 加群、つまり (§ 2, no. 4) は左 g^0 加群と識別されます。

φ を U の主反自己同型とする。M が右 g モジュールの場合、m ∈ M および a ∈ U に対して a.m = m.φ(a) と書くことによって、左 g モジュール構造が M 上に定義されます。

概念と加群の理論の結果は、表現の言語に翻訳できます。

(1) M と M' 上の g の 2 つの表現 ρ と ρ' は、g 加群 M と M' が同型である場合、*類似* または *同型* と呼ばれます。このためには、次のような K-加群 M の上に K-加群 M' の同型 u が存在することが必要かつ十分です。

$$
\rho'(x) = u \circ \rho(x) \circ u^{-1}
$$

すべての x ∈ g に対して。

(2) すべての i ∈ I について、ρ_i を M_i 上の g の表現とする。 M を g モジュール M_i の g モジュール直和とします。 M 上の g の対応する表現 ρ は、ρ_i の *直和* と呼ばれ、$\sum_{i \in I} \rho_i$ (または n 表現 $\rho_1, \ldots, \rho_n$ の場合は $\rho_1 + \cdots + \rho_n$) で表されます。 $m = (m_i)_{i \in I}$ が M と x ∈ g の元である場合、$\rho(x).m = (\rho_i(x).m_i)_{i \in I}$ です。

(3) M 上の g の表現 ρ は、付随した g モジュールが単純な場合、*単純* または *既約* と呼ばれます。すべての $\rho(x), x \in g$ の下で安定した M のサブ K モジュール ({0} と M 以外) が存在しないと言うのと同じことになります。単純な g モジュールの類 (代数、章 VIII, § 3, no. 2) 定義する g* の単純な表現の *類。

(4) M 上の g の表現 ρ は、付随した g 加群が半単純の場合、*半単純* または *完全に簡約可能* と呼ばれます。 ρ が単純な表現の直和に似ている、あるいは、

$\rho(x)$ ($x \in g$) で安定した M には、$\rho(x)$ ($x \in g$) (cf. *代数*、章 VIII, § 3, no. 3) で安定した補充があります。

(5) $\delta$ を、単純な $g$ モジュールの $g$ 対応するから類 C の単純な表現の類とします。一方、$\rho$ を M 上の $g$ の表現とします。 $g$ モジュール M の種 C の同型成分 $M_C$ (*代数*、章 VIII, § 3, no. 4) も、 *種の M $\delta$ の同型成分。この成分は、$\rho(x)$ で安定した M のサブ K モジュールの和であり、その上に類 $\delta$ の $\rho(x)$ 誘導する表現が含まれます。それはこれら部分加群のうちの直和です。 $M_C$ が長さ $n$ の場合、$\rho$ は *含む* $\delta$ *n 回*と言われます。別の $M_C$ の和は直接です。 $\rho$ が半単純である場合に限り、M と等しくなります。

(6) $\rho, \rho'$を$g$の2つの表現とします。 $\rho'$の加群が$\rho$の加群の部分加群（それぞれ商加群）である場合、$\rho'$は$\rho$の*部分表現*（それぞれ*商表現*）と呼ばれます。

M をK-加群とします。 零表現の $g$ on M 定義する on M $g$ モジュール構造。この構造 M は *自明* $g$ モジュールと呼ばれます。

M を $g$ 加群とする。 M のサブ$g$ モジュールの商 $g$ モジュールは、M の商加群のサブ$g$ モジュールでもあります。これらは、$U \supset U'$ となるように M の 2 つのサブ$g$ モジュール U、$U'$ を考慮し、 $g$-モジュール$U/U'$。次に、上記の型のすべての単純加群が指定された単純な $g$ 加群 N と同型である場合、M は *純粋な* $g$ 加群 *種* N と呼ばれます。 $\rho$ と $\sigma$ が $g$ の表現である場合対応する M と N に、$\rho$ は *純粋な種* $\sigma$ であるとも言います。

$M'$ を M のサブ加群 $g$ とする。M が種 N から純粋であるためには、$M'$ と $M/M'$ が種 N から純粋であることが必要かつ十分である。条件については、明らかに必要である。それが成立し、U、$U'$ を M のサブ$g$ 加群とし、$U' \subset U$ と $U/U'$ が単純になると仮定します。 $\phi$を$M/M'$に対するMの標準準同型とします。 $\phi(U) \neq \phi(U')$ の場合、$U/U'$ は同型から $\phi(U)/\phi(U')$ であるため、N と同型です。 $\phi(U) = \phi(U')$ の場合、$U \subset U' + M'$ であるため、$U/U'$ は $(U' + M')/U'$ の単純部分加群と同型であり、後者の加群自体は $M'/(U' \cap M')$ と同型です。したがって、$U/U'$ は再び N と同型であるため、M は種 N から純粋です。

今後、M を $g$ 加群とし、純粋な種 N である M のサブ $g$ 加群の集合が極大元 $M'$ を許容すると仮定します。すると、種 N から純粋な M のすべての部分加群 $M''$ が $M'$ に含まれます。なぜなら、$M''/(M' \cap M'')$ と $M'$ は種 N から純粋であるため、上記により $M' + M''$ は種 N から純粋であり、したがって $M' + M'' \subset M'$ となります。

$g$ モジュール M が Jordan-Hölder 系列 $(M_i)_{0 \leq i \leq n}$ を許容すると仮定します。 M が種 N から純粋であるためには、$M_0/M_1, M_1/M_2, \ldots, M_{n-1}/M_n$ が N と同型であることが必要かつ十分です。なぜなら、条件は明らかに必要であり、その十分性は、上で見たことから、$n$ の帰納法によってすぐに続きます。

#### 命題 1 {#lie-i-s3-prop-1 .statement tag=09VV}

*g を K よりもリー代数とし、g のイデアルを仮定します。 M を g モジュール*、$N$ を単純な $a$ モジュールとします。 $M$ を $a$ 加群として考え、純粋な種 $N$ である $M$ のサブ $a$ 加群の集合が極大元 $M'$ を認めると仮定します。次に、$M'$ は $M$ のサブ$g$ モジュールです。

$y \in g$ にしましょう。 $\phi$を$M$の標準写像を$M/M'$に、$f$を写像$m \mapsto \phi(y_M \cdot m)$を$M'$から$M/M'$にします。 $f(M') = \{0\}$ を示せば十分です。 $x \in a$ にしましょう。次に、$m \in M$ については、

$$
x_{M/M'} \cdot f(m) = \phi(x_M y_M \cdot m) = \phi(y_M x_M \cdot m) + \phi([x, y]_M \cdot m).
$$

現在 $[x, y] \in a$、よって $\phi([x, y]_M \cdot m) = 0$;一方で、

$$
\phi(y_M x_M \cdot m) = f(x_M \cdot m).
$$

したがって、$x_{M/M'} \cdot f(m) = f(x_M \cdot m)$です。したがって、$f(M')$ は $M'$ の商と同型の $M/M'$ のサブ$a$ 加群であり、したがって種 $N$ の純粋であることがわかります。したがって$f(M') = \{0\}$です。

#### 系 {#lie-i-s3-n1-cor-1 .statement tag=09VW}

*$g$を$K$と$a$の$g$を超えるリー代数とします。 $M$ を単純な $g$ モジュール、有限長を $K$ モジュールとします。 $M$ が種 $N$ の純粋な $a$ 加群であるような単純な $a$ 加群 $N$ が存在します。

$a$ モジュール $M$ は有限長であるため、$M$ のサブ $a$ モジュールの集合には最小限の元 $N$ が存在します。これは、$M$ の単純なサブ $a$ モジュールです。種$N$から純粋である$M$のサブ$a$加群最大のは、したがって$\neq \{0\}$であり、$M$(命題1)のサブ$g$加群であり、したがって$M$と同一である。

### 2. 表現中テンソル積

$g$ の表現のファミリーの no. 1 直和で定義しました。これから表現に定義するその他の演算を行います。

$g_1, g_2$ を 2 つのリー代数と $K$ および $M_i$ を $g_i$ モジュール ($i = 1, 2$) とします。 $U_i$を、$g_i$の代数と$g_i$の$\sigma_i$標準写像を$U_i$に包むものとします。この場合、$M_i$ は左 $U_i$ モジュールであるため、$M_1 \otimes_K M_2$ は標準的な左 $(U_1 \otimes_K U_2)$ モジュール構造になります。さて、$U_1 \otimes_K U_2$は$g_1 \times g_2$の代数を包むものであり、写像$(x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)$は$g_1 \times g_2$の標準写像をこの包む代数(§ 2, no. 2)に包含します。したがって、$M = M_1 \otimes_K M_2$ には次のような $(g_1 \times g_2)$ モジュール構造が存在します。

$$
\begin{align*}
(1) \quad (x_1, x_2)_M \cdot (m_1 \otimes m_2) &= (\sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)) \cdot (m_1 \otimes m_2) \\
&= ((x_1)_{M_1} \cdot m_1) \otimes m_2 + m_1 \otimes ((x_2)_{M_2} \cdot m_2).
\end{align*}
$$

これは、$M$ の $g_1 \times g_2$ の構造定義する表現です。

ここで、$g$ の $g_1 = g_2 = g$、準同型 $x \mapsto (x, x)$ を $g \times g$ にすると、上記の表現、定義する表現 $M$ の $g$ で構成され、したがって $g$ モジュール構造になります。 $M$ 次のようになります:

$$
(2) \quad x_M \cdot (m_1 \otimes m_2) = (x_{M_1} \cdot m_1) \otimes m_2 + m_1 \otimes (x_{M_2} \cdot m_2).
$$

同様の議論により、次のことがわかります。

#### 命題 2 {#lie-i-s3-prop-2 .statement tag=09VX}

$g$ を $K$ 上のリー代数とし、$M_i$ を $g$ モジュール ($1 \leq i \leq n$) とします。 テンソル積 $M_1 \otimes_K M_2 \otimes \cdots \otimes M_n$ には、次のような $g$ モジュール構造が 1 つだけ存在します。

$$
x_M \cdot (m_1 \otimes \cdots \otimes m_m) = \sum_{t=1}^n m_1 \otimes \cdots \otimes (x_{M_t} \cdot m_i) \otimes \cdots \otimes m_n
$$

すべての$x \in g, m_1 \in M_1, \ldots, m_n \in M_n$に。

対応する表現は、$M_i$ の $g$ の指定された表現の *テンソル積* と呼ばれます。

In particular, if $M$ is a $g$-module, Proposition 2 defines a $g$-module structure on each $M_p = \bigotimes^p M$ and hence on the tensor algebra $T$ of $M$.

公式 (3) は、すべての $x \in g, x_T$ が拡大する $x_M$ である代数 $T$ の一意の *導分* であることを示しています。私たちは、$M$の対称代数$S$の移行から商導分に$x_T$定義するがいることを知っています（§ 2, no. 8）。したがって、$S$ は $T$ の商 $g$ モジュールと考えることができ、$x_S$ は $S$ の導分です。

Still more particularly, consider $g$ as a $g$-module by means of the adjoint representation of $g$. $U$ を $g$ を囲む代数とします。 By Proposition 7 of § 2, $x_M$ defines on passing to the quotients a derivation of $U$ which is just the inner derivation defined by $\sigma(x)$ ($\sigma$ denoting the canonical mapping of $g$ into $U$). すると、$U$ は $T$ の商 $g$ モジュールと考えることができます。 $K$ が特性 0 の体である場合、$U$ 上の $S$ の標準同型は、$g$ モジュール同型 (§ 2, no. 8) です。

### 3. 準同型加群の表現

もう一度、$g_1$ と $g_2$ を、$K$ と $M_i$ 上の 2 つのリー代数である $g_i$ モジュール ($i = 1, 2$) とします。 $U_i$ を、$g_i$ の代数と $g_i$ の $\sigma_i$ 標準写像を $U_i$ に包むものとします。 この場合、$M_i$ は左 $U_i$ モジュールであるため、$\mathscr{L}_K(M_1, M_2)$ は標準的な左 $(U_1^0 \otimes U_2)$ モジュール構造になります。 現在、$U_1^0 \otimes_K U_2$ は、$g_1^0 \times g_2$ と写像を囲む代数です。

$$
(x_1, x_2) \mapsto \sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)
$$

$g_1^0 \times g_2$ の標準写像がこの代数に収まります。 したがって、$M = \mathscr{L}_K(M_1, M_2)$ には次のような $(g_1^0 \times g_2)$ モジュール構造が存在します。

$$
((x_1, x_2)_M \cdot u) \cdot m_1 = ((\sigma_1(x_1) \otimes 1 + 1 \otimes \sigma_2(x_2)) \cdot u) \cdot m_1 \\
= u((x_1)_{M_1} \cdot m_1) + (x_2)_{M_2} \cdot u(m_1)
$$

すべての$u \in \mathscr{L}_K(M_1, M_2), m_1 \in M_1$に。これは、$M$ の $g_1^0 \times g_2$ の構造定義する表現です。

ここで、$g$ の $g_1 = g_2 = g$、準同型 $x \mapsto (-x, x)$ を $g^0 \times g$ にすると、上記の表現、定義する表現 $M$ の $g$ で構成され、したがって $g$ モジュール構造になります。 $M$そのような

$$
(x_M \cdot u) \cdot m_1 = x_{M_2} \cdot u(m_1) - u(x_{M_1} \cdot m_1)
$$

または

$$
x_M \cdot u = x_{M_2} u - u x_{M_1}.
$$

これらの結果を命題 2 と組み合わせると、次のことがわかります。

#### 命題 3 {#lie-i-s3-prop-3 .statement tag=09VY}

*$g$ を $K$ 上のリー代数とし、$M_i$ を $g$ モジュール ($1 \leq i \leq n + 1$) とします。 $N$ を、$\prod_{i=1}^n M_i$ から $M_{n+1}$ への多重線形写像の $K$ 加群 $\mathscr{L}_K(M_1, \ldots, M_n; M_{n+1})$ とします。 $N$ には、次のような $g$ モジュール構造が 1 つだけ存在します*

$$
(x_N \cdot u)(m_1, \ldots, m_n) = - \sum_{i=1}^n u(m_1, \ldots, x_{M_i} \cdot m_i, \ldots, m_n)
$$
$$
+ x_{M_{n+1}} \cdot u(m_1, \ldots, m_n)
$$

*全員に* $x \in g, u \in N$ *そして* $m_i \in M_i$ ($1 \leq i \leq n$)。

特に、$g$ を $K$ および $M$ のリー代数を $g$ モジュールとし、$K$ を自明な $g$ モジュールと考えます。 命題 3 定義する $\mathscr{L}_K(M, K) = M^*$ の $g$ モジュール構造。 対応する表現は、表現 $x \mapsto x_M$ の *双対* 表現と呼ばれます。我々は持っています：

$$
(x_{M^*} \cdot f)(m) = -f(x_M \cdot m)
$$

すべての$x \in g, f \in M^*, m \in M$に。その他語:

$$
x_{M^*} = -{}^t x_M.
$$

$K$ が体で、$M$ が有限次元の場合、$g$ モジュール $M^*$ が単純 (それぞれ半単純) である場合に限り、$g$ モジュール $M$ は単純 (それぞれ半単純) です。

#### 命題 4 {#lie-i-s3-prop-4 .statement tag=09VZ}

*$M_1, M_2$ を 2 つの $g$ モジュールとします。標準的 $K$ 線形マッピング* (代数、章 II, § 4, no. 2、命題 2 および no. 1、命題 1):

$$
M_1^* \otimes_K M_2 \xrightarrow{\phi} \mathscr{L}_K(M_1, M_2), \quad \mathscr{L}_K(M_1, M_2^*) \xrightarrow{\psi} (M_1 \otimes_K M_2)^*
$$

*(2 番目が全単射である場合)* は $g$-モジュール準同型です。

私たちは書きます

$$
N = M_1^* \otimes M_2, \quad P = \mathscr{L}(M_1, M_2), \quad Q = \mathscr{L}(M_1, M_2^*), \quad R = (M_1 \otimes M_2)^*.
$$

次に、$x \in g, f \in M_1^*, m_1 \in M_1, m_2 \in M_2$ については、

$$
((\phi x_N)(f \otimes m_2)) \cdot m_1 = (\phi(x_{M_1^*} f \otimes m_2 + f \otimes x_{M_2} m_2)) \cdot m_1 \\
= \langle x_{M_1^*} f, m_1 \rangle m_2 + \langle f, m_1 \rangle x_{M_2} m_2
$$

$$
((x_P \phi)(f \otimes m_2)) \cdot m_1 = x_{M_2}(\phi(f \otimes m_2) \cdot m_1) - \phi(f \otimes m_2)(x_{M_1} m_1) \\
= \langle f, m_1 \rangle x_{M_2} m_2 - \langle f, x_{M_1} m_1 \rangle m_2
$$

and hence $\phi x_N = x_P \phi$.一方、$x \in g, u \in \mathscr{L}(M_1, M_2^*), m_1 \in M_1, m_2 \in M_2$ の場合:

$$
(\psi x_Q u)(m_1 \otimes m_2) = \langle (x_Q u) \cdot m_1, m_2 \rangle = \langle x_{M_2^*} u m_1 - u x_{M_1} m_1, m_2 \rangle \\
(x_R \psi u)(m_1 \otimes m_2) = -\langle \psi u, x_{M_1} m_1 \otimes m_2 + m_1 \otimes x_{M_2} m_2 \rangle \\
= -\langle u x_{M_1} m_1, m_2 \rangle - \langle u m_1, x_{M_2} m_2 \rangle
$$

したがって $\psi x_Q = x_R \psi$ となり、証明が完成します。

$g$ モジュール $\mathscr{L}(M_1, M_2^*)$ および $(M_1 \otimes M_2)^*$ は、同型 $\psi$ で識別されます。 $M_1$ と $M_2$ が有限の基底を持つ場合、$\phi$ は同型 (代数, 章 II, § 4, no. 2, 命題 2) となり、同一視するが可能になります。 $g$-モジュール $M_1^* \otimes M_2$ および $\mathscr{L}(M_1, M_2)$;その場合、したがって、$g$ モジュール $M_1^* \otimes M_2^*, \mathscr{L}(M_1, M_2^*)$ と $(M_1 \otimes M_2)^*$ を同一視するにすることができます。

### 4. 例

#### 例 1 {#lie-i-s3-n4-exa-1 .statement tag=09W0}

$g$ を $K$ 上のリー代数とし、$M$ を $g$ モジュールとします。 $M$ の $g$ モジュール構造と、$K$ 定義するの自明な $g$ モジュール構造、$M$ の双線形形式の $N = \mathscr{L}(M, M; K)$ の $K$ モジュール上の $g$ モジュール構造。 それから

$$
(x_N \cdot \beta)(m, m') = -\beta(x_M \cdot m, m') + \beta(m, x_M \cdot m')
$$

$M, \beta \in N$ のすべての $x \in g, m, m'$ に対して。 $\beta$ が $N$ の元、$x \in g$ の集合である場合、$x_N \cdot \beta = 0$ は $g$ の部分代数になります。

Let $M$ be a $K$-module and $\beta$ a bilinear form on $M$. By the above, the set of $x \in gl(M)$ such that

$$
\beta(x \cdot m, m') + \beta(m, x \cdot m') = 0
$$

すべての$m \in M$と$m' \in M$は、$gl(M)$の嘘部分代数です。 $K$ が体、$M$ が有限次元、$\beta$ が非縮退であると仮定します。次に、すべての $x \in gl(M)$ は、どこでも定義されている左随伴 $x^*$ ($\beta$ に対して) を認めます。また、問題の部分代数は、$x^* = -x$ のように、$x \in gl(M)$ の集合です。このプロセスにより、構成する 2 つの重要な例リー代数:

(a) $M = K^n$ を取得し、

$$
\beta((\xi_1, \ldots, \xi_n), (\eta_1, \ldots, \eta_n)) = \xi_1 \eta_1 + \cdots + \xi_n \eta_n.
$$

正規的には同一視する $gl(K^n)$ と $M_n(K)$ です。すると、リー代数は、斜対称行列のリー代数になります。 *($K = \mathbf{R}$のとき、この代数は直交群$O(n, \mathbf{R})$のリー代数です)。

(b) $M = K^{2m}$ を取得し、
$$
\beta((\xi_1, \ldots, \xi_{2m}), (\eta_1, \ldots, \eta_{2m})) = \xi_1 \eta_{m+1} - \eta_1 \xi_{m+1} + \cdots + \xi_m \eta_{2m} - \eta_m \xi_{2m}.
$$
$K^{2m}$の標準基底に対して$\beta$の行列は行列
$$
\begin{pmatrix}
0 & I_m \\
-I_m & 0
\end{pmatrix}.
$$
元の$K^{2m}$の標準基底、$\mathrm{gl}(M)$の$u$($\mathbf{M}_m(K)$に$A, B, C, D$が入っている)に対して$U = \begin{pmatrix} A & B \\ C & D \end{pmatrix}$を行列とします。 *代数*の公式(50)により、章IX, § 1, no. 10、$u^*$は同じ基底行列に関して
$$
\begin{pmatrix}
0 & -I_m \\
I_m & 0
\end{pmatrix}
\begin{pmatrix}
tA & tC \\
tB & tD
\end{pmatrix}
\begin{pmatrix}
0 & I_m \\
-I_m & 0
\end{pmatrix}
= \begin{pmatrix}
tD & -tB \\
-tC & tA
\end{pmatrix}.
$$
したがって、条件 $u^* = -u$ は条件と同等です
$$
D = -tA \quad B = tB \quad C = tC.
$$
*$K = \mathbf{R}$の場合、リー代数はシンプレクティック群$\mathbf{Sp}(2m, \mathbf{R})$のリー代数となります。

#### 例 2 {#lie-i-s3-n4-exa-2 .statement tag=09W1}

*例 1* の記法を保存します。

The $g$-module structure on $M$ defines on the $K$-module $P = \mathscr{L}_K(M, M)$ of endomorphisms of $M$ a $g$-module structure. (6) により、すべての $x \in g$ と $u \in P$ について:
$$(11)$$
$$
x_P \cdot u = [x_M, u] = (\mathrm{ad}\, x_M) \cdot u
$$
ここで、$\mathrm{ad}\, x_M$ は、$\mathrm{gl}(M)$ の随伴表現の下にある $x_M$ の像を表します。 その他語:
$$(12)$$
$$
x_P = \mathrm{ad}\, x_M
$$
$\mathscr{L}(\mathscr{L}(M, M)) = \mathscr{L}(\mathrm{gl}(M))$で。

### 5. 不変式元

#### 定義 3 {#lie-i-s3-def-3 .statement tag=09W2}

*$g$をリー代数、$M$を$g$モジュールとします。 元 $m \in M$ は、すべての $x \in g$ に対して $x_M \cdot m = 0$ である場合 ($M$ の $g$ モジュール構造に関して、または $g$ の対応する表現に関して) 不変と呼ばれます。*

*$G$ を接続された実リー群、$g$ をそのリー代数、$\theta$ を有限次元実数ベクトル空間 $E$ および $\rho$ 対応する上の $G$ の解析表現とします。 $E$の$g$の表現。 $m \in E$ にしましょう。 元 $m$ は、すべての $g \in G$ に対して $\theta(g) \cdot m = m$ である場合に限り、 $\rho$ に関して不変です。これにより、語「不変量」の使用が正当化されます。*

#### 例 1 {#lie-i-s3-n5-exa-1 .statement tag=09W3}

$M, N$ を 2 つの $g$ モジュールと $P = \mathscr{L}_K(M, N)$ とします。 $P$ の元 $f$ が不変であるためには、(6) により、$f$ が $g$ モジュール $M$ の $g$ モジュール $N$ の準同型であることが必要かつ十分です。特に、すべての $x \in g$ に対して $M = N$ と $x_M = x_N$ がある場合、$f$ が $x_M$ で置換可能な場合に限り、$f$ は不変です。

#### 例 2 {#lie-i-s3-n5-exa-2 .statement tag=09W4}

M を K-加群とし、有限の基底とします。 M が g 加群構造を持つ場合、$\mathscr{L}(M, M)$ と $M^* \otimes M$ は g 加群構造を持ち、$M^* \otimes M$ の $\mathscr{L}(M, M)$ への標準写像は g 加群同型 (命題 4) です。 $1 \in \mathscr{L}(M, M)$ は明らかに不変式 (cf. 例 1) であるため、$M^* \otimes M$ の対応する元 $u$ も不変式です。 $(e_i)_{1 \leq i \leq n}$ が M の基底で、$(e_i^*)_{1 \leq i \leq n}$ が双対基底である場合、$u = \sum_{i=1}^n e_i^* \otimes e_i$ が得られます。

#### 例 3 {#lie-i-s3-n5-exa-3 .statement tag=09W5}

M を g モジュールとする。 $\beta$ を M の双線形形式とし、$\mathscr{L}(M, M^*)$ の f 対応する元とします。 $\beta$ が不変であるためには、f が g モジュール準同型 (命題 4 および例 1) であることが必要かつ十分です。 K が体で、K が $\dim_K M < +\infty$ であるとします。 g モジュール M の M 定義する同型上の非縮退不変双線形形式 $\beta$ が g モジュール $M^*$ に配置され、したがって g モジュール $M \otimes M$ の同型が g モジュール $M^* \otimes M$ に配置されます。したがって、例 2 により、$\beta$ 定義するは、g モジュール $M \otimes M$ 内の正規不変量元 c を与え、次のように構築できます。 $(e_i)_{1 \leq i \leq n}$ を M の基底および M の $(e'_i)_{1 \leq i \leq n}$ 基底とします。 $\beta(e_i, e'_j) = \delta_{ij}$;それから$c = \sum_{i=1}^n e_i \otimes e'_i$。

#### 命題 5 {#lie-i-s3-prop-5 .statement tag=09W6}

*g を嘘 K-代数、h を g の理想、M 上の g の $\rho$ 表現、h に対する $\rho$ の $\rho'$ 制限とする。このとき、$\rho'$ に関して不変な M の元の集合 N は、$\rho(g)$ の下で安定です。*

$n \in N$ と $y \in g$ としましょう。 $x \in h, [x, y] \in h$ 全員にとって、そしてそれ故
$$
\rho(x)\rho(y)n = \rho([x, y])n + \rho(y)\rho(x)n = 0;
$$
したがって$\rho(y)n \in N$です。

#### 命題 6 {#lie-i-s3-prop-6 .statement tag=09W7}

*M を半単純 g モジュールとします。次に、M の不変式元の部分加群 $M_0$ は、$x_M$ の下で安定な補充を 1 つだけ許容します。つまり、$x_M.m$ ($x \in g, m \in M$) によって生成される部分加群 $M_1$ です。

$M'$ を M の部分加群とします。これは、M の $M_0$ の $x_M$ と補充の下で安定です。すべての $m \in M, m = m_0 + m'$ と $m_0 \in M_0, m' \in M'$、したがって $x_M m = x_M m' \in M'$ についてです。したがって$M_1 \subset M'$です。 $M_2$ を $x_M$ の下で安定し、$M'$ で $M_1$ を補う $M'$ の部分加群とします。 $m \in M_2$の皆様、
$$
x_M m \in M_2 \cap M_1 = \{0\}
$$
すべての $x \in g$、したがって $m \in M_0$、そして $m = 0$ です。したがって、$M_2 = \{0\}$ は、$M_1 = M'$ であることを証明します。

### 6. 不変双線形形式

g を K よりリー代数とします。 g on g の随伴表現と K 上の g の零表現定義する K-加群の g モジュール構造

$g$ の双線形形式の $N = \mathscr{L}(g, g; K)$。簡単に言うと、表現 $x \mapsto x_N$ で不変であれば、$g$ 上の双線形形式 $\beta$ は *不変量* であると言います。 公式 (10) により、これがそうなるために必要かつ十分な条件は次のとおりです。

$$
\beta([x, y], z) = \beta(x, [y, z])
$$

$g$ のすべての $x, y, z$ に対して。

ここで、$\mathfrak{d}$ を $g$ の導分のリー代数とします。 The identity representation of $\mathfrak{d}$ and the zero representation of $\mathfrak{d}$ on $K$ define a representation $D \mapsto D_N$ of $\mathfrak{d}$ on $N$. 簡単に言うと、$g$ 上の双線形形式が表現 $D \mapsto D_N$ で不変である場合、それは *完全に不変* であると言います。 完全に不変双線形形式は不変です。 $g$ 上の双線形形式 $\beta$ が完全に不変であるためには、次のことが必要かつ十分です。

$$
\beta(Dx, y) + \beta(x, Dy) = 0
$$

$g$ と $D \in \mathfrak{d}$ のすべての $x, y$ に対して。

#### 命題 7 {#lie-i-s3-prop-7 .statement tag=09W8}

*$g$をリー代数、$\beta$を$g$上の不変対称双線形形式、$a$を$g$の理想とする。*

(a) *$\beta$に関して$a$の直交$a'$は$g$のイデアルです*。
(b) *$a$ が特性であり、$\beta$ が完全に不変である場合、$a'$ は特性です。*
(c) *$\beta$ が非縮退の場合、$a \cap a'$ は可換です。*

$D$ を $g$ の導分とします。 $a$が$D$では安定しており、$g$の$x, y$に対して$\beta(Dx, y) + \beta(x, Dy) = 0$が安定しているとします。次に、$z \in a'$ は、すべての $t \in a$、$Dt \in a$、したがって $\beta(Dz, t) = -\beta(z, Dt) = 0$ について、$Dz \in a'$ を意味します。したがって、$a'$ は $D$ の下で安定します。これにより、(a) と (b) が成立します。

さて、$b$を$g$の理想とし、$\beta$～$b$の制限が零であるとします。 $b$と$z \in g$、$\beta([x, y], z) = \beta(x, [y, z]) = 0$の$x, y$、$[y, z] \in b$の場合。したがって、$[b, b]$ は $g$ に直交します。 $\beta$ が非縮退であれば、$b$ は可換です。この結果を$a \cap a'$に適用すると、(c)が証明されます。

#### 定義 4 {#lie-i-s3-def-4 .statement tag=09W9}

*Let $g$ be a Lie $K$-algebra and $M$ a $g$-module. $M$ が $K$ 加群として考えられ、有限の基底を許容すると仮定します。 $g$ モジュール $M$ (または対応する表現) に関連付けられた双線形形式は、$g$ 上の対称の双線形形式 $(x, y) \mapsto \operatorname{Tr}(x_M y_M)$ です。 問題の表現が随伴表現である場合、関連する双線形形式は $g$ の Killing 形と呼ばれます。

#### 命題 8 {#lie-i-s3-prop-8 .statement tag=09WA}

*$g$をリー代数、$M$を$g$モジュールとします。 $M$ が $K$ 加群として考慮され、有限の基底が許容されると仮定します。 $M$ に関連付けられた双線形形式は不変です。*

$g$ の $x, y, z$ については、次のようになります。

$$
\begin{align*}
\operatorname{Tr}([x, y]_M z_M) &= \operatorname{Tr}(x_M y_M z_M) - \operatorname{Tr}(y_M x_M z_M) = \operatorname{Tr}(x_M y_M z_M) - \operatorname{Tr}(x_M z_M y_M) \\
&= \operatorname{Tr}(x_M [y, z]_M).
\end{align*}
$$

#### 命題 9 {#lie-i-s3-prop-9 .statement tag=09WB}

*$K$ が体で、リー代数 $g$ が $K$ 上の有限次元* であると仮定します。 *$a$を$g$の理想とし、$\beta$を$g$の殺害形、$\beta'$を$a$の殺害形とします。すると、$\beta'$は$\beta$から$a$の制限になります。

$u$ をベクトル空間 $g$ の自己準同型とすると、$a$ は安定します。 $v$を$u$から$a$の制限と、移行から商のときの$u$から導かれるベクトル空間$g/a$の$w$自己準同型とします。 次に、$g$ の基底 $(x_1, \ldots, x_n)$ のうち、$a$ の最初の $p$ 元形基底を取得すると、$\operatorname{Tr} u = \operatorname{Tr} v + \operatorname{Tr} w$ が得られます。 次に$x \in a, y \in a$とし、上記の公式を$u = (\operatorname{ad}_g x)(\operatorname{ad}_g y)$の場合に適用します。 次に、$v = (\operatorname{ad}_a x)(\operatorname{ad}_a y)$ と $w = 0$ です。 したがって、$\beta(x, y) = \beta'(x, y)$です。

#### 命題 10 {#lie-i-s3-prop-10 .statement tag=09WC}

*$K$ が体で、リー代数 $g$ が $K$ 上で有限次元であると仮定します。 $g$ の殺害形 $\beta$ は完全に不変です。*

$D$を$g$の導分とします。コディメンション 1 の理想としてリー代数 $g'$ 含む $g$ と、すべての $x \in g$ (§ 1, no. 8, 例 1) に対して $Dx = [x_0, x]$ となるような $g'$ の元 $x_0$ が存在します。 $\beta'$を$g'$の殺害形とします。 $g$、$\beta'([x, x_0], y) = \beta'(x, [x_0, y])$の$x, y$、つまり$\beta'(Dx, y) + \beta'(x, Dy) = 0$です。これで、$\beta'$から$g$の制限は$\beta$(命題9)となります。したがって命題です。

### 7. カシミール元

#### 命題 11 {#lie-i-s3-prop-11 .statement tag=09WD}

*$g$を体$K$の上のリー代数、$U$を囲む代数、$h$を$g$上の$g$と$\beta$不変双線形形式の有限次元理想とする。 制限 ～ $h$ は非退化です。 $(e_i)_{1 \leq i \leq n}, (e'_j)_{1 \leq j \leq n}$ を $h$ の 2 つの基底として、$\beta(e_i, e'_j) = \delta_{ij}$ とします。次に、$U$ 属するの元 $c = \sum_{i=1}^n e_i e'_i$ から $U$ の中心までとなり、基底 $(e_i)$ の選択とは独立しています。

$x \in g$ の場合、$x_h$ を $\operatorname{ad}_g x$ の制限から $h$ とします。すると、$x \mapsto x_h$ はベクトル空間 $h$ 上の $g$ の表現であり、$\beta$ から $h$ の制限 $\beta'$ は、この表現の下で不変です。 no. 5、*例 3*、テンソル $\sum_{i=1}^n e_i \otimes e'_i$ は、基底 $(e_i)$ の選択から独立しており、テンソル代数の不変条件元 $h$。また、$g$ のテンソル代数 $T$ の元であり、$g$ の随伴表現から導出された表現に対して不変です。したがって、$U$の標準像、つまり$c$は、$(e_i)$の基底の選択から独立しており、no. 2の終わりに考慮される$U$上の$g$の表現にとっては不変式です。したがって、この元は $g$ のすべての元で置換可能であり、したがって $U$ の属するから中心となります。

$\beta$ が $g$ モジュール $M$ に関連付けられている双線形形式である場合、命題 11 の元 $c$ は、$M$ (または対応するに関連付けられている) *Casimir 元* と呼ばれます表現）。この元は、$\beta$～$h$の制限が非縮退であれば存在します。

#### 命題 12 {#lie-i-s3-prop-12 .statement tag=09WE}

*$g$ を体 $K$ 上のリー代数、有限次元 n の $g$ と K 上の有限次元の M a g-module の理想を $h$ とします。 c をカシミール元とします（存在します）M と h に関連付けられています。

(a) $\operatorname{Tr}(c_M) = n$。
(b) *M が単純で、n が K の標数で割り切れない場合、$c_M$ は M* の自己同型です。

命題 11の記法では、

$$
\operatorname{Tr}(c_M) = \sum_{i=1}^n \operatorname{Tr}((e_i)_M(e'_i)_M) = \sum_{i=1}^n \beta(e_i, e'_i) = n.
$$

したがって、n が K の特性で割り切れない場合、$c_M \neq 0$ となります。一方、U の c 属するから中心のように、$c_M$ はすべての $x_M, x \in g$ と置換可能です。さらに M が単純な場合、$c_M$ は $\mathscr{L}(M)$ (*代数*, 章 VIII, § 4, no. 3, 命題 2) で可逆です。

### 8. 拡大/基底環

$K_1$ を可換環とし、K の単位元と $\phi$ 準同型を $K_1$ 写像と 1 対 1 にします。 g を嘘 K-代数とし、U をそれを囲む代数とし、M を左とします。 g モジュール、つまり左側の U モジュールです。この場合、$M_{(K_1)}$ は標準的な左 $U_{(K_1)}$ モジュール構造を持ち、したがって左 $g_{(K_1)}$ モジュール構造になります。 $\rho$ と $\rho_{(K_1)}$ を g の表現とし、$g_{(K_1)}$ 対応するを M および $M_{(K_1)}$ とします: $\rho_{(K_1)}$ は、基底環* を * 拡張することで $\rho$ から導出されると言われます。 *代数*、章 VIII, § 13, no. 4 の結果を適用できます。 $x \in g$ の場合、$\rho_{(K_1)}(x)$ は $M_{(K_1)} = M \otimes_K K_1$ の自己準同型 $\rho(x) \otimes 1$ にすぎません。

K が体、$K_1$ が K の拡大、$\phi$ が K の標準単射から $K_1$ であるとします。 V と V' を M のベクトル部分空間とします。 a を $\rho(x)(V) \subset V'$ となるような $x \in g$ の g からなるのベクトル部分空間とします。 $a'$ を $g_{(K_1)}$ からなるのベクトル部分空間 、$x' \in g_{(K_1)}$ の$\rho_{(K_1)}(x')(V_{(K_1)}) \subset V'_{(K_1)}$ とする。 次に$a' = a_{(K_1)}$。 明らかに$a_{(K_1)} \subset a'$のため。 では、$x' \in a'$ にしましょう。 $x' = \sum_{i=1}^n \lambda_i x_i$ と書くことができます。ここで、$x_i$ は g にあり、$\lambda_i$ は K 上で線形独立な $K_1$ の元です。 すべての $u \in V$、$\rho(x') \cdot u \in V'_{(K_1)}$、つまり $\sum_{i=1}^n \lambda_i \rho(x_i) \cdot u \in V'_{(K_1)}$、よって $\rho(x_i) \cdot u \in V'$、したがって $x_i \in a$ と $x' \in a_{(K_1)}$ です。 これは、$a' = a_{(K_1)}$ であることを示しています。 特に、$g_{(K_1)}$ の *中心* は、K を $K_1$ まで拡張することによって g の中心から導出されます。上記を g の随伴部分表現に適用するだけで十分です。 すべての $p$ に対して $\mathscr{C}_p(g_{(K_1)}) = (\mathscr{C}_p g)_{(K_1)}$ ということになります。 同様に、h を g の部分代数とし、n を g の h の *ノーマライザー* とします。 すると、$g_{(K_1)}$ の $h_{(K_1)}$ のノーマライザーは $n_{(K_1)}$ になります。

K、$K_1$、g、$\rho$、M を最後の段落と同じとする。 b を g のベクトル部分空間および M の W ベクトル部分空間とします。 V を M のベクトル部分空間 $m \in M$ のからなるとし、$\rho(b) \cdot m \subset W$ とします。 V' を $m' \in M_{(K_1)}$ の $M_{(K_1)}$ からなるのベクトル部分空間とし、$\rho_{(K_1)}(b_{(K_1)}) \cdot m' \subset W_{(K_1)}$ とします。上のように$V' = V_{(K_1)}$であることがわかります。特に、$M_{(K_1)}$ の *不変量* のベクトル部分空間は、$K$ から $K_1$ まで基礎体を拡張することにより、$M$ の不変量のベクトル部分空間から導出されます。

$K, K_1$ と $\phi$ をこの番号の冒頭と同じようにします。 $g$ を Lie $K$-代数、$M$ および $N$ $g$-加群とする。 $M$ と $N$ が同型 $g$ 加群である場合、$M_{(K_1)}$ と $N_{(K_1)}$ は同型 $g_{(K_1)}$ 加群です。逆に:

#### 命題 13 {#lie-i-s3-prop-13 .statement tag=09WF}

*$K$ を $K$ の体、$K_1$ 拡大、$g$ を嘘$K$-代数、$M, N$ $K$ 上の有限次元の 2 つの $g$ 加群とする。 $M_{(K_1)}$ と $N_{(K_1)}$ が同型 $g_{(K_1)}$ 加群である場合、 $M$ と $N$ は同型 $g$ 加群です。*

証明は2段階です。

(1) まず、$K_1$ が *有限次数* $n$ の $K$ の拡大であるとします。 $U$ を $g$ のエンベロープ代数とすると、$g_{(K_1)}$ のエンベロープ代数は $U_{(K_1)} = U \otimes_K K_1$ (§ 2, no. 9) になります。 $M_{(K_1)}$ と $N_{(K_1)}$ は $U_{(K_1)}$ モジュールと同型であるため、*なおさら* $U$ モジュールと同型です。しかし、$U$ モジュールとしては、それぞれ $M^n$ および $N^n$ と同型です。 Now $M$ and $N$ are $U$-modules of finite length; $M$ (resp. $N$) is therefore the direct sum of a family $(P_i^{r_i})_{1 \leq i \leq p}$ (resp. $(Q_j^{s_j})_{1 \leq j \leq q}$) of submodules such that the $P_i$ (resp. $Q_j$) are indecomposable and two $P_i$ (resp. $Q_j$) of different indices are not isomorphic (*Algebra*, Chapter VIII, § 2, no. 2, Theorem 1). 次に、$M^n$ (それぞれ $N^n$) は、$P_i^{n r_i}$ (それぞれ $Q_j^{n s_j}$) の直和と同型です。 (*loc. cit.*) $p = q$ と後では、必要に応じて $Q_j$ を並べ替えると、 $n r_i = n s_i$ と $P_i$ は $1 \leq i \leq p$ に対して $Q_i$ と同型であるため、$M$ は $N$ と同型であることがわかります。

(2) *一般的なケース* $P$ を、$P$ の不変式の $g$ モジュール $\mathscr{L}_K(M, N)$ および $Q$ 部分空間とします。つまり、$g$ モジュール $M$ の準同型の集合です。 $g$-モジュール$N$。 $g_{(K_1)}$ モジュール $\mathscr{L}_{K_1}(M_{(K_1)}, N_{(K_1)}) = (\mathscr{L}_K(M, N))_{(K_1)}$ では、不変式の部分空間は $Q_{(K_1)}$ です。 $M_{(K_1)}$ と $N_{(K_1)}$ が同型であるという仮定は、$M$ と $N$ が $K$ に対して同じ次元を持ち、$Q_{(K_1)}$ 元 $g$ に存在することを意味します。 $M_{(K_1)}$の同型が$N_{(K_1)}$に。 $(f_1, \ldots, f_d)$ を、$K$ を超える $Q$ の基底と、$M$ と $K$ を超える $N$ の選ぶ基底とします。 $1 \leq k \leq d$ に対する $\lambda_k \in K_1$ の場合、これらの基底に関する $f = \sum_{k=1}^d \lambda_k f_k$ の行列は行列式となり、係数 *in* $K$ の多項式 $D(\lambda_1, \ldots, \lambda_d)$ になります。 $f = g$ のとき、この行列式は非ゼロであるため、$D$ の係数はすべて非ゼロではありません。したがって、$\Omega$ が $K$ の代数閉包である場合、($\Omega$ は無限であるため) $D(\mu_1, \ldots, \mu_d) \neq 0$ (*代数*, 章) となる元 $\mu_k \in \Omega$ $(1 \leq k \leq d)$ が存在します。 IV, § 2, no. 5、命題 8)。 $K_2$ が $\mu_k$ $(1 \leq k \leq d)$ によって生成された $K$ の代数拡大である場合、$\sum_{k=1}^d \mu_k f_k$ は $N_{(K_2)}$ 上の $M_{(K_2)}$ の同型であるということになります。しかし、$K_2$ は $K$ よりも有限次数 (*代数*, 章 V, § 3, no. 2, 命題 5) であるため、$M$ と $N$ は引数の最初の部分によって同型です。

もう一度、$K, K_1$ と $\phi$ をこの番号の始まりとします。 $\rho$ を、有限基底 $(x_1, \ldots, x_n)$ を持つ $K$ モジュール $M$ 上の $g$ の表現とします。次に、$\rho_{(K_1)}$ に関連付けられた $g_{(K_1)}$ の双線形形式は、基底環を $K_1$ に拡張することにより、$\rho$ に関連付けられた双線形形式から導出されます (つまり、$u \in \mathscr{L}_K(M)$ の場合、$u$ は同じ行列を持ちます)。 $(x_1, \ldots, x_n)$ に関しては、$(x_1 \otimes 1, \ldots, x_n \otimes 1)$ に関しては $u \otimes 1$ であるため、$u$ と $u \otimes 1$ は同じトレースになります）。特に、$K$ モジュール $g$ が有限の基底を持つ場合、$g_{(K_1)}$ の *Killing 形* は、基底環を $K_1$ に拡張することで、$g$ の *Killing 形* から導出されます。

### 練習問題 {#lie-i-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
