---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 11
section_title: Graded modules and rings
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 363-377, 424-425
pdf_pages: 0387-0401, 0448-0449
extraction: ocr
subsections:
    - "no": 1
      title: GRADED COMMUTATIVE GROUPS
      page: 363
      pdf_page: 387
    - "no": 2
      title: GRADED RINGS AND MODULES
      page: 364
      pdf_page: 388
    - "no": 3
      title: GRADED SUBMODULES
      page: 367
      pdf_page: 391
    - "no": 4
      title: CASE OF AN ORDERED GROUP OF DEGREES
      page: 371
      pdf_page: 395
    - "no": 5
      title: GRADED TENSOR PRODUCT OF GRADED MODULES
      page: 374
      pdf_page: 398
    - "no": 6
      title: GRADED MODULES OF GRADED HOMOMORPHISMS
      page: 375
      pdf_page: 399
statements: 28
exercises: 1
content_sha256: 8d75023ce25bed5faa4faada06dbbbd3594ab0b5093930d3b88a43567dca06f3
translated_from: content/en/alg/II/11_s11_graded_modules_and_rings.md
translation_method: google
source_content_sha256: cee0143d544bc99c4e8496ec6bc7458982857f3f0ed4fb081e4de491d7e81dfd
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 6a21f762aef11749a5721f87afffbd839d7b7e107a2a7df0410ff999c2d8d0f2
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 11。グレード加群および環

*この段落のno. 2以降、$\Delta$は加法的に書かれた可換モノイド(I, § 2, no. 1)を表し、単位元は0で表されます。*

### 1. 段階的可換群

直和 (§ 1, no. 8) について、他の言語定義に翻訳します。

#### 定義 1 {#alg-ii-s11-def-1 .statement tag=05XX}

*加法的に書かれた可換群 $G$ と集合 $\Delta$ を考えると、$G$ 上の型 $\Delta$ の卒業は、$G$ の部分群の家族 $(G_\lambda)_{\lambda \in \Delta}$ になります。 $G$は直和です。 集合 $G$ は、群法則とその目盛によって定義される構造を、型 $\Delta$ の段階的 (可換) 群と呼ばれます。

$\Delta$は、$G$の次数*の*集合と呼ばれます。 元 $x \in G$ は、$G_\lambda$ の 1 つに対して属するの場合は *同次*、$x \in G_\lambda$ の場合は次数* $\lambda$ の *同次* と呼ばれます。したがって、元 0 はすべての次数と同次です。しかし、$x \neq 0$ が同種であれば、$G_\lambda$ のうちの 1 つだけに属するが適用されます。 添字 $\lambda$ では、$x \in G_\lambda$ は * $x$ の *次数 (または $x$ の *重み* であるときどき) と呼ばれ、ときどきは $\deg(x)$ で表されます。すべての $y \in G$ は、同種の元と $y_\lambda \in G_\lambda$ の和 $\sum_\lambda y_\lambda$ として一意に記述できます。 $y_\lambda$ は、$y$ の次数* $\lambda$ の *同次成分 (または単に次数* $\lambda$ の *成分) と呼ばれます。 「次数」の代わりに語「重み」が使用される場合、形容詞「均質」は「等圧」に置き換えられます。

#### 例 {#alg-ii-s11-n1-exa-1 .statement tag=05XY}

(1) 可換モノイド $\Delta$ (単位元 0) と可換群 $G$ が与えられた場合、$\lambda \neq 0$ に対して $G_0 = G$ と $G_\lambda = \{0\}$ を取ることにより、$G$ に目盛$(G_\lambda)_{\lambda \in \Delta}$ が定義されます。この卒業は *trivial* と呼ばれます。

(2) $\Delta, \Delta'$を$\Delta$の2つの集合と$\rho$写像を$\Delta'$とします。 $(G_\lambda)_{\lambda \in \Delta}$ を、可換群 $G$ 上の型 $\Delta$ の卒業式とします。 $\mu \in \Delta'$ の場合、$G'_\mu$ を $G_\lambda$ の和とし、$\rho(\lambda) = \mu$ とします。明らかに $(G'_\mu)_{\mu \in \Delta'}$ は $G$ の型 $\Delta'$ の卒業であり、写像 $\rho$ によって $(G_\lambda)$ から *派生* したと言われています。

$\Delta$ が加法的に書かれた可換群と、$\Delta$ の $\rho$ 写像 $\lambda \mapsto -\lambda$ であるとき、$(G'_\mu)$ は $(G_\lambda)$ の *反対の* 目盛と呼ばれます。

(3) $\Delta = \Delta_1 \times \Delta_2$ が 2 つの集合の積である場合、型 $\Delta$ の卒業は型 $\Delta_1, \Delta_2$ の *bigraduation* と呼ばれます。すべての $\lambda \in \Delta_1$ については $G'_\lambda = \bigoplus_{\mu \in \Delta_2} G_{\lambda \mu}$ とし、すべての $\mu \in \Delta_2$ については $G''_\mu = \bigoplus_{\lambda \in \Delta_1} G_{\lambda \mu}$ とします。明らかに、$(G'_\lambda)_{\lambda \in \Delta_1}$ は型 $\Delta_1$ の卒業であり、$(G''_\mu)_{\mu \in \Delta_2}$ は $G$ の型 $\Delta_2$ の卒業です。これらの卒業は、bigraduation $(G_{\lambda \mu})$ から派生した *部分卒業* と呼ばれます。 $G_{\lambda \mu} = G'_\lambda \cap G''_\mu$; に注意してください。逆に、$(G'_\lambda)_{\lambda \in \Delta_1}$ と $(G''_\mu)_{\mu \in \Delta_2}$ が $G$ の 2 つの目盛りで、$G$ が $G_{\lambda \mu} = G'_\lambda \cap G''_\mu$ の直和である場合、これらの部分群形は型 $\Delta_1, \Delta_2$ の 2 つの目盛りになります。 $G$、うち$(G'_\lambda)$と$(G''_\mu)$は部分卒業です。これを $\Delta$ が集合の有限積である場合に一般化する作業は読者に委ねます。

(4) $\Delta_0$ を加法的に書かれた可換モノイドとし、単位元を 0 で表します。 $I$ を任意の集合とし、$\Delta_0^{(I)} = \Delta$ は有限台の家族 $(\lambda_i)_{i \in I}$ の積 $\Delta_0^I$ からなるの部分モノイドを表します。 $\rho : \Delta \to \Delta_0$ を、$\rho((\lambda_i)) = \sum_{i \in I} \lambda_i$ によって定義される $\Delta_0$ への $\Delta$ の全射（余対角）準同型とします。 型 $\Delta$ の各目盛りから型 $\Delta_0$ の目盛りが $\rho$ (*例 2*) によって導出されます。それは、型 $\Delta$ の特定の「多階調」に関連付けられた *合計卒業* と呼ばれます。

このNo.の定義と例拡大するは、$G$ が群である場合にすぐに適用されます。これは *必ずしも可換であるとは限りません*。 直和のどこでも概念を「制限付き和」 (§ 1, no. 6, *注意*) で置き換えるにするだけです。この場合、$G_\lambda$ は $G$ の通常の部分群であり、$\lambda \neq \mu$ では、$G_\lambda$ のすべての元が $G_\mu$ のすべての元と置換可能であることに注意してください。

### 2. グレード環および加群

#### 定義 2 {#alg-ii-s11-def-2 .statement tag=05XZ}

*環 $A$ と、加法群 $A$ の型 $\Delta$ の目盛 $(A_\lambda)$ を考慮すると、この目盛りは、$A$ の環構造と互換性があると言われます。

$$
A_\lambda A_\mu \subset A_{\lambda + \mu} \quad \text{for all } \lambda, \mu \text{ in } \Delta.
$$

*この目盛りの環 $A$ は、型 $\Delta$ のグレード付き環と呼ばれます。

#### 命題 1 {#alg-ii-s11-prop-1 .statement tag=05Y0}

※$\Delta$の全ての元がキャンセル可能で、$(A_\lambda)$が型$\Delta$の環$A$の構造と互換性のある卒業である場合、$A_0$は部分環となります$A$ (特に $1 \in A_0$)*

$A_0 A_0 \subset A_0$ by 定義なので、$1 \in A_0$ であることを証明すれば十分です。 $1 = \sum_{\lambda \in \Delta} e_\lambda$ を 1 の分解として同次の成分にします。 $x \in A_\mu$ の場合は、$x = x . 1 = \sum_{\lambda \in \Delta} x e_\lambda$。 次数 $\mu$ の成分を比較すると、($\mu + \lambda = \mu$ は $\lambda = 0$ を意味するため) $x = x e_0$ になります。この関係は $A$ のすべての同種元に当てはまるため、すべての $x \in A$ に当てはまります。特に$1 = 1 . e_0 = e_0 \in A_0$。

#### 定義 3 {#alg-ii-s11-def-3 .statement tag=05Y1}

*$A$ を型 $\Delta$ の等級付けされた環、$(A_\lambda)$ をその卒業、$M$ を左 (それぞれ右) $A$ モジュールとします。 加法群 $M$ の型 $\lambda$ の目盛り $(M_\lambda)$ は、* の場合、$M$ の $A$ モジュール構造と互換性があります。

(2)
$$
A_\lambda M_\mu \subset M_{\lambda + \mu} \quad (\text{resp. } M_\mu A_\lambda \subset M_{\lambda + \mu})
$$
*$\Delta$のすべての$\lambda, \mu$。この目盛の加群 $M$ は、等級付けされた環 $A$ を超えて、型 $\Delta$ の左 (または右) 等級加群と呼ばれます。

$\Delta$ の元がキャンセル可能である場合、(2) と命題 1 から、$M_\lambda$ は $A_0$ モジュールであることがわかります。

明らかに、$A$ が型 $\Delta$ のグレード環である場合、左側の $A$ モジュール $A_s$ (それぞれ右側の $A$ モジュール $A_d$) は型のグレードとなります。 $\Delta$。

#### 例 {#alg-ii-s11-n2-exa-1 .statement tag=05Y2}

(1) 環 $A$ の型 $\Delta$ の自明な目盛りは、環構造と互換性があります。 $A$ が自明な目盛りによって評価される場合、$A$ モジュール $M$ 上の型 $\Delta$ の目盛り $(M_\lambda)$ が $A$ モジュール構造と互換性があるためには、$M_\lambda$ が以下であることが必要かつ十分です。 $M$の*部分加群*。

(2) $A$ を型 $\Delta$ の等級付けされた環、$M$ 型 $\Delta$ および $\Delta$ の$\rho$ 準同型の等級付けされた $A$ 加群とする。モノイド $\Delta'$ の単位元は 0 で表されます。その場合、$A$ は型 $\Delta'$ の等級付けされた環と、$M$ は型 $\Delta'$ の等級付けされた加群です。 型 $\Delta'$ は、$\rho$ と、$A$ と $M$ の型 $\Delta$ の目盛から、no. 1、*例* 1 の手順で導出されます。 1: これは、関係の直後に続きます。 $\rho(\lambda + \mu) = \rho(\lambda) + \rho(\mu)$。

特に、$\Delta = \Delta_1 \times \Delta_2$ が 2 つの可換モノイドの積である場合、射影 $\mathrm{pr}_1$ と $\mathrm{pr}_2$ は準同型であり、対応するの目盛りは、型 $\Delta$ の目盛りから導出された単なる *部分目盛り* になります。 (no. 1、*例* 3);したがって、これらの部分的な目盛りは、$A$ の環構造および $M$ の加群構造と互換性があります。

同様に、$\Delta = \Delta_0^{(r)}$ ($\Delta_0$ は 0 で示される単位元の可換モノイド) の場合、型 $\Delta_0$ の *合計目盛* (no. 1, 例 4) は型の目盛から導出されます。余対角準同型による$A$上の$\Delta$(それぞれ$M$)は、$A$上の環構造(それぞれ$M$上の加群構造)と互換性があります。

(3) Let $A$ be a graded ring of type $\Delta$, $M$ a graded $A$-module of type $\Delta$ and $\lambda_0$ an element of $\Delta$; for all $\lambda \in \Delta$, let $M'_\lambda = M_{\lambda + \lambda_0}$ and let $M'$ be the $\mathbf{Z}$-module $\bigoplus_{\lambda \in \Delta} M'_\lambda$. As $A_\lambda M'_\mu \subset M_{\lambda + \mu + \lambda_0} = M'_{\lambda + \mu}$, $M'$ is an $A$-module and the $M'_\lambda$ form on $M'$ a graduation of type $\Delta$ compatible with the $A$-module structure of $M'$; the graded $A$-module $M'$ of type $\Delta$ thus defined is said to be obtained by shifting by $\lambda_0$ the graduation of $M$ and it is denoted by $M(\lambda_0)$. $\Delta$ が群の場合、等級付けされた $A$ モジュール $M'$ の基礎となる $A$ モジュールは $M$ で識別されます。

*(4) $B$を可換環とします。 1 つの不確定要素の多項式環 $B[X]$ は、部分群 $BX^n$ ($n \geqslant 0$) (cf. III, § 2, no. 9 および IV) によって型 $\mathbf{N}$ に評価されます。

*(5) Let $B$ be a commutative ring, $E$ a $B$-module, $Q$ a quadratic form on $E$ and $C(Q)$ the Clifford algebra of $Q$ (cf. IX, § 9). $C(Q)$ のサブ$B$ モジュール $C^+(Q)$ および $C^-(Q)$ 形は、$C(Q)$ の環構造と互換性のある型 $\mathbf{Z}/2\mathbf{Z}$ の目盛りです。

#### 注意 {#alg-ii-s11-n2-rem-1 .statement tag=05Y3}

(1) 最もよく使用される目盛りは、型 $\mathbf{Z}$ または型 $\mathbf{Z}^n$ です。 型について言及せずに、等級 (それぞれ 2 等級、3 等級など) 加群および環について話す場合、型 $\mathbf{Z}$ (それぞれ $\mathbf{Z}^2, \mathbf{Z}^3$ など) の等級を意味すると理解されます。 型 $\mathbf{N}$ のグレーディング環 (それぞれ加群) は、プラスの次数を持つグレーディング環 (それぞれ加群) とも呼ばれます。

(2) 型 $\Delta$ の等級付き $\mathbf{Z}$ 加群は、$\mathbf{Z}$ が自明な階位を持つ場合、定義 1 の等級付き可換群 (次数の集合は可換モノイド) にすぎません。 (no. 1)。

#### 定義 4 {#alg-ii-s11-def-4 .statement tag=05Y4}

*$A, A'$ を、同じ型 $\Delta$ と $(A_\lambda), (A'_\lambda)$ の 2 つの等級環とします。 環準同型 $h : A \to A'$ は、すべての $\lambda \in \Delta$ に対して $h(A_\lambda) \subset A'_\lambda$ の場合、グレーディングと呼ばれます。

$M, M'$ を、型 $\Delta$ の等級付けされた環に対して、型 $\Delta$ の 2 つの等級付けされた加群とします。 Let $u : M \to M'$ be an $A$-homomorphism and $\delta$ an element of $\Delta$; $u$ is called graded of degree $\delta$ if $u(M_\lambda) \subset M_{\lambda + \delta}$ for all $\lambda \in \Delta$.

$A$ を型 $\Delta$ のグレード環、$A'$ を型 $\Delta'$ および $\rho : \Delta \to \Delta'$ 準同型のグレード環とします。 A ring homomorphism $h : A \to A'$ is called graded if $h$ is a graded homomorphism of graded rings of type $\Delta'$ when $A$ is given the graduation of type $\Delta'$ derived from its graduation of type $\Delta$ by means of $\rho$ (no. 1, Example 2); this therefore means that $h(A_\lambda) \subset A'_{\rho(\lambda)}$ for all $\lambda \in \Delta$.

$u$ が次数 $\delta$ に等級付けされるような $\delta \in \Delta$ が存在する場合、$A$-準同型性 $u : M \to M'$ は等級付きと呼ばれます。 $u \neq 0$ と $\Delta$ のすべての元がキャンセル可能である場合、$u$ の次数 $\delta$ は一意に決まります。

$h : A \to A', h' : A' \to A''$ が 2 つの等級付けされた準同型と型 $\Delta$ の等級付けされた環である場合、$h' \circ h : A \to A''$ も同様です。 写像 $h : A \to A'$ が等級付けされた環同型であるためには、$h$ が全単射であること、および $h$ とその逆写像 $h'$ が等級付けされている準同型であることが必要かつ十分です。このためには、$h$ が準同型と評価された全単射であることでも十分です。したがって、等級付けされた準同型は、型 $\Delta$ (*集合理論*、IV, § 2, no. 1) の等級付けされた環構造の種の射として解釈できることがわかります。

同様に、$u : M \to M'$ と $u' : M' \to M''$ がそれぞれ次数 $\delta$ と $\delta'$ の 2 つのグレード準同型のグレード A-加群型 $\Delta$ である場合、$u' \circ u : M \to M''$ はグレード準同型になります。 次数 $\delta + \delta'$。 $\delta$ が $\Delta$ の逆 $-\delta$ を認め、$u : M \to M'$ が次数 $\delta$ の全単射準同型である場合、その逆写像 $u' : M' \to M$ は、準同型の全単射となります。 次数 $-\delta$。上記のように、次数* 0 の * 等級付けされた準同型は、型 $\Delta$ の等級付けされた A-加群の種の射として解釈できることがわかります。しかし、$M$ と $N$ がゼロ以外で、$\Delta$ の元がキャンセル可能な場合、次数 $\neq 0$ の準同型 $u : M \to N$ と評定された全単射は、A-加群同型と評定されません。

#### 例 {#alg-ii-s11-n2-exa-2 .statement tag=05Y5}

(6) $M$ が等級付けされた A-加群で、$M(\lambda_0)$ が (no. 2, *例 3*) をシフトすることによって得られた等級付けされた A-加群である場合、$M(\lambda_0)$ を $M$ に$\mathbf{Z}$ 線形写像します。各々の $M_{\lambda + \lambda_0}$ に標準単射が付いている一致するは、次数 $\lambda_0$ のグレード準同型です ($\Delta$ が *群* の場合、これは全単射です)。

(7) $a$ が、次数 $\delta$ 所属から中心の$A$、ホモテティー $x \mapsto ax$ のいずれかの等級A-加群 $M$ の元である場合次数 $\delta$ のグレードは準同型です。

*注意* (3) *均質* 元の $M$ からなるの基底 $(m_i)_{i \in I}$ が存在する場合、等級付けされた A-加群 $M$ は *等級付けされた自由A-加群* と呼ばれます。それがそうであり、$\Delta$ が可換 *群* であると仮定します。 $\lambda_i$ を $m_i$ の次数とし、各 $i$ について、シフトされた A-加群 $A(-\lambda_i)$ (no. 2, *例 3*) を考慮します。 $e_i$ が元を表す場合、$A$ の 1 は次数* の元とみなされる $A(-\lambda_i)$ の $\lambda_i$、A-線型写像 $u : \bigoplus_{i \in I} A(-\lambda_i) \to M$ がすべて $u(e_i) = m_i$ となる$i$ は *グレード A-加群同型* です。

常に $\Delta$ が可換群であると仮定して、今度は $N$ を $N$ の *均質* 生成元の等級付けされた A-加群、$(n_i)_{i \in I}$ 系とし、$n_i$ が次数であると仮定します。 $\mu_i$。次に、A-線型写像 $v : \bigoplus_{i \in I} A(-\mu_i) \to N$ は、すべての $i$ に対する $u(e_i) = n_i$ が次数* 0 の *全射的等級付けされた A-加群準同型になります。 $N$ が *有限生成* 等級付けされた A-加群である場合、常に有限が存在します。 $N$の同次生成元の系したがって、$I$ *有限*を持つ上記の型の全射準同型が存在します。

### 3. 評価部分加群

#### 命題 2 {#alg-ii-s11-prop-2 .statement tag=05Y6}

*A を型 $\Delta$ の等級環、M を型 $\Delta$、$(M_\lambda)$ の等級 A-加群とし、N を M のサブ A モジュールとします。以下のプロパティは同等です:*

(a) $N$ * は家族の和* $(N \cap M_\lambda)_{\lambda \in \Delta}$ です。
(b) *N 属するから N* までのすべての元の同種成分。
(c) $N$ * は同種の元* によって生成されます。

N のすべての元は、$M_\lambda$ の元の和として一意に書くことができるため、(a) と (b) は同等であり、(a) は (c) を暗黙的に示すことは明らかになります。 (c) が (b) を意味することを示します。次に、$(x_i)_{i \in I}$ を N の同種生成元 $\neq 0$ の族とし、$\delta(i)$ を $x_i$ の次数とします。 N のすべての元は、$a_i \in A$ を使用して $\sum_i a_i x_i$ として書くことができます。 $a_{i,\lambda}$ が次数 $\lambda$ の $a_i$ の成分である場合、結論は関係から得られます。

$$
\sum_{i \in I} \left( \sum_{\mu \in \Delta} a_{i,\mu} x_i \right) = \sum_{\lambda \in \Delta} \left( \sum_{\mu + \delta(i) = \lambda} a_{i,\mu} x_i \right).
$$

**注意 (1)** 上記の記法では、関係 $\sum_{i \in I} a_i x_i = 0$ は、関係 $\sum_{\mu + \delta(i) = \lambda} a_{i,\mu} x_i = 0$ の系に相当します。 $\Delta$が群のとき、これらの関係は$\sum_{i \in I} a_{i,\lambda - \delta(i)} x_i = 0$と書くことができます。

M の部分加群 N が命題 2 で述べた同等の特性を持つ場合、明らかに $N \cap M_\lambda$ 形は N の A-加群構造と互換性のある目盛りであり、M 上の目盛りによって *誘導される*目盛りと呼ばれます。この等級の N は、M の *等級部分加群* と呼ばれます。

#### 系 1 {#alg-ii-s11-prop-2-cor-1 .statement tag=05Y7}

*N が M の段階的な部分加群で、$(x_i)$ が N の生成する系である場合、N の $x_i$ 形生成する系の同種成分です。

#### 系 2 {#alg-ii-s11-prop-2-cor-2 .statement tag=05Y8}

*N が M から有限に生成された部分加群である場合、N は同次元の有限生成系からなるを許容します。*

M の元には同次成分 $\neq 0$ の有限数しかないことに注意して系を適用する 1 を行うだけで十分です。

$A_s$ (それぞれ $A_d$) の等級付けされた部分加群は、等級付けされた環 A の *等級付けされた左* (それぞれ *右*) と呼ばれます。 $A(B \cap A_\lambda)(B \cap A_\mu) \subset B \cap A_{\lambda+\mu}$ の部分環 B ごとに; B が A の *段階付きサブ$\mathbf{Z}$モジュール* である場合、A の段階によって B に引き起こされる段階は、B の環構造と互換性があります。 次に、B は A の *グレード付けされた部分環* と呼ばれます。

明らかに、N (または B) が M の等級付きサブ A モジュール (または A の等級部分環) である場合、標準単射 $N \to M$ (それぞれ $B \to A$) は次数 0 の等級付けされた加群準同型 (それぞれ等級環) です。 準同型）。

N が、等級付けされた A-加群 M の等級付けされた部分加群と、M の卒業である $(M_\lambda)_{\lambda \in \Delta}$ である場合、部分加群 $(M_\lambda + N)/N$ の $M/N$ 形は、この商加群の構造と互換性のある *卒業* です。なぜなら、$N_\lambda = M_\lambda \cap N$, $(M_\lambda + N)/N$ が $M_\lambda/N_\lambda$ と同一視され、命題 2 と § 1, no. 6, 公式 (26) から、$M/N$ がそれらの直和であることがわかります。さらに、

$$
A_\lambda(M_\mu + N) \subset A_\lambda M_\mu + N \subset M_{\lambda+\mu} + N
$$
したがって、$A_\lambda((M_\mu + N)/N) \subset (M_{\lambda+\mu} + N)/N$ が主張を確立します。

ション。目盛り ((M_\lambda + N)/N)_{\lambda \in \Delta} は、N による M の目盛りの商目盛りと呼ばれ、この目盛りを持つ商加群 M/N は、段階付けされた部分加群 N による M の段階付けされた商加群と呼ばれます。 標準準同型 M \to M/N は、この卒業式では次数 0 の準同型に評価されます。

b が A の等級付き両側イデアルである場合、A/b の商目盛は A/b の環構造と互換性があります。この等級の環 A/b は、A by b の商等級付け環と呼ばれます。 標準準同型 A \to A/b は、この卒業式では環の評価のうち準同型です。

#### 命題 3 {#alg-ii-s11-prop-3 .statement tag=05Y9}

*A を型 \Delta の等級付けされた環、M、N を型 \Delta の等級付けされた 2 つの A-加群および u: M \to N を次数 \delta の等級付けされた A 準同型性とします。次に:*
(i) Im(u) は N のグレード部分加群です。
(ii) *\delta が \Delta の正則元である場合、Ker(u) は M の部分加群に評価されます。*
(iii) * \delta = 0 の場合、u に正規に関連付けられた全単射 M/Ker(u) \to Im(u) は、等級付けされた加群の同型です。*

主張 (i) は、定義および命題 2(c) の直後に続きます。 x が M の元で、u(x) = 0 かつ x = \和_\lambda である場合、x_\lambda はその分解を同次成分に変換したもの (x_\lambda は次数 \lambda のもの)、
$$
\sum_\lambda u(x_\lambda) = u(x) = 0
$$
そして u(x_\lambda) は次数 \lambda + \delta です。 \delta が正則関係 \lambda + \delta = \mu + \delta である場合、 \lambda = \mu を意味します。 したがって、u(x_\lambda) は u(x) の同次成分であり、\Delta 内のすべての \lambda \ について必然的に u(x_\lambda) = 0 となり、これは (ii) を証明します。 全単射 v: u に正規に関連付けられた M/Ker(u) \to Im(u) は、商卒業の定義から次のように、次数 \delta の準同型に等級付けされます。 よって (iii) \delta = 0 の場合。

#### 系 {#alg-ii-s11-n3-cor-1 .statement tag=05YA}

*A、B を 2 つの評価環の型 \Delta とし、u: A \to B を評価準同型の評価環とします。この場合、Im(u) は B の等級付けされた部分加群であり、Ker(u) は A の等級付けされた両側イデアルであり、 全単射 A/Ker(u) \to Im(u) は u に正規に関連付けられており、等級付けされた環の同型です。

等級付けされた \mathbf{Z} モジュールの次数 0 の準同型とみなすには、命題を適用する 3 で十分です。

#### 命題 4 {#alg-ii-s11-prop-4 .statement tag=05YB}

*A を型 \Delta の環と評価し、M を型 \Delta の A-加群と評価します。*
(i) *M の等級付けされた部分加群のすべての和とすべての共通部分は等級付けされた部分加群です。*
(ii) * x が \Delta でキャンセル可能な次数 \mu の M の同次元である場合、x の消滅子は A の段階的左イデアルです。*
(iii) * \Delta のすべての元がキャンセル可能である場合、M の段階的部分加群の消滅子は A の段階的両側イデアルです。*

$(\mathbf{N}_i)$ が $M$ の等級付けされた部分加群の族である場合、命題 2 の性質 (c) は、$\mathbf{N}_i$ の和が同次元によって生成されることを示し、命題 2 の性質 (b) が証明します。 $\bigcap_i \mathbf{N}_i$ 属するから $\bigcap_i \mathbf{N}_i$ のすべての元の同種の成分 。 よって (i)。

(ii) を証明するには、$\operatorname{Ann}(x)$ が $A$ モジュール $A_s$ の $M$ の準同型 $a \mapsto ax$ の核であり、この準同型が次数 $\mu$ のグレードであることに注意するだけで十分です。結論は命題 3(ii) から得られます。 Finally (iii) is a consequence of (i) and (ii) for the annihilator of a graded submodule $N$ of $M$ is the intersection of the annihilators of the homogeneous elements of $N$, by virtue of Proposition 2.

#### 注意 2 {#alg-ii-s11-n3-rem-2 .statement tag=05YC}

Let $M$ be a graded $A$-module and $E$ a submodule of $M$; it follows from Proposition 4(i) that there exists a *largest* graded submodule $N'$ of $M$ contained in $E$ and a *smallest* graded submodule $N''$ of $M$ containing $E$; $N'$ is the set of $x \in E$ all of whose homogeneous components belong to $E$ and $N''$ is the submodule of $M$ generated by the homogeneous components of a generating system of $E$.

#### 命題 5 {#alg-ii-s11-prop-5 .statement tag=05YD}

*$A$ を型 $\Delta$ の環とします。 $\Delta$ のすべての元がキャンセル可能である場合、同種のすべての元 $a \in A$ について、$A$ (I, § 1, no. 5) の $a$ のセントラライザーは、$A$ のグレード付けされた部分環です。

$a$ が次数 $\delta$ であると仮定します。 $b = \sum_\lambda b_\lambda$ を元とし、$a$ を置換可能とし、$b_\lambda$ をすべての $\lambda \in \Delta$ について次数 $\lambda$ の$b$ の同次成分とします。次に、仮定 $\sum_\lambda (ab_\lambda - b_\lambda a) = 0$ と $ab_\lambda - b_\lambda a$ により、次数 $\lambda + \delta$ と同次になります。 $\delta$ はキャンセル可能であるため、すべての $\lambda$ に対して $ab_\lambda = b_\lambda a$ となり、主張であることが証明されます。

#### 系 {#alg-ii-s11-n3-cor-2 .statement tag=05YE}

*$\Delta$のすべての元がキャンセル可能な場合、$A$のグレード付けされた部分環$B$(特に$A$の中心)のセントラライザーは、$A$のグレード付けされた部分環になります。

それは$B$の均質な元の集中化者の共通部分です。

注意 (3) *型 $\Delta$ の段階的環の *直接系 $(A_\alpha, \phi_{\beta\alpha})$ (それぞれ型 $\Delta$ の段階的 $A_\alpha$ モジュールの直接系 $(M_\alpha, f_{\beta\alpha})$) は環 (それぞれ $A_\alpha$ モジュール) の直接系で、それぞれの $A_\alpha$ (それぞれ $M_\alpha$) が型 $\Delta$ にグレードされ、各 $\phi_{\beta\alpha}$ (それぞれ $f_{\beta\alpha}$) が *準同型となる等級付けされた環* (それぞれ * 等級付けされた加群* の次数 0 の *$A_\alpha$* 準同型性)。 $(A^\lambda_\alpha)_{\lambda \in \Delta}$ (または $(M^\lambda_\alpha)_{\lambda \in \Delta}$) が $A_\alpha$ (または $M_\alpha$) の卒業である場合、次のように書きます。

$$
A = \lim_{\longrightarrow} A_\alpha,\quad A^\lambda = \lim_{\longrightarrow} A^\lambda_\alpha \quad (\text{resp. } M = \lim_{\longrightarrow} M_\alpha,\ M^\lambda = \lim_{\longrightarrow} M^\lambda_\alpha),
$$

§ 6, no. 2、命題 5 から、$(A^\lambda)$ (それぞれ $(M^\lambda)$) は A (それぞれ M) の目盛りであることがわかり、I, § 10 からは、番号 2 がわかります。図 3 と図 4 から、この目盛りは A の環構造 (M の A-加群構造) と互換性があることがわかります。グレード環 A (それぞれグレード A-加群 M) は、グレード環 $(A_\alpha, \phi_{\beta\alpha})$ (それぞれグレード加群 $(M_\alpha, f_{\beta\alpha})$) の直接系の直接極限と呼ばれます。 $\phi_\alpha : A_\alpha \to A$ (それぞれ $f_\alpha : M_\alpha \to M$) が標準写像の場合、$\phi_\alpha$ (それぞれ $f_\alpha$) は等級の準同型環 (それぞれ次数の準同型 0) $A_\alpha$-modules).

### 4. 次数の群を注文した場合

可換的な群 $\Delta$ 上で加法的に書かれた位数構造 ($\leq$ で示される) は、すべての $\rho \in \Delta$ について関係 $\lambda \leq \mu$ が意味する場合、群構造と *互換性がある* と言われます。 $\lambda + \rho \leq \mu + \rho$. 群 $\Delta$ とこの位数構造は *順序付き群* と呼ばれます。これら群については VI, § 1 で詳しく学習します。ここでは、そのような群関係 $\lambda > 0$ は、すべての $\mu$ に対して $\lambda + \mu > \mu$ を意味するという指摘に限定します。なぜなら、定義と関係 $\xi + \mu = \mu$ による $\lambda + \mu \geq \mu$ が意味するからです。 $\xi = 0$。

$\Delta$ を順序付き可換性群とし、A を型 $\Delta$ および $(A_\lambda)$ の等級付け環とし、関係 $A_\lambda \neq \{0\}$ が $\lambda \geq 0$ を暗黙すると仮定します。次に、定義から、上で作成した注意により、$\mathfrak{I}_0 = \sum_{\lambda > 0} A_\lambda$ は A の *段階的な両側イデアル* であることがわかります。

#### 命題 6 {#alg-ii-s11-prop-6 .statement tag=05YF}

*$\Delta$ を順序付き可換群とし、A を型 $\Delta$ の環と評価し、$(A_\lambda)$ をその卒業とし、M を型 $\Delta$ の A-加群と評価し、 $(M_\lambda)$ 卒業です。 関係 $A_\lambda \neq \{0\}$ は $\lambda \geq 0$ を暗示し、$\lambda < \lambda_0$ に対して $M_{\lambda_0} \neq \{0\}$ と $M_\lambda = \{0\}$ が存在するような $\lambda_0$ が存在するとします。次に、$\mathfrak{I}_0 = \sum_{\lambda > 0} A_\lambda$、$\mathfrak{I}_0 M \neq M$ の場合。*

$x$ を $M_{\lambda_0}$ の非ゼロ元とします。 $x \in \mathfrak{I}_0 M$ だとします。次に、$x = \sum_i a_i x_i$、ここで、$a_i$は、$\mathfrak{I}_0$の元$\neq 0$と、Mの$x_i$は、すべての$i$(no. 2)に対して$\deg(x) = \deg(a_i) + \deg(x_i)$と同種の元$\neq 0$です。しかし、$\deg(a_i) > 0$、$\lambda_0 = \deg(a_i) + \deg(x_i) > \deg(x_i)$、そして矛盾する仮定として。

#### 系 1 {#alg-ii-s11-prop-6-cor-1 .statement tag=05YG}

*$\Delta$ と命題 6 の A の仮説で、M が $\mathfrak{I}_0 M = M$ のように有限に生成された等級付けされた A-加群である場合、$M = \{0\}$ になります。*

$M \neq \{0\}$ と仮定します。 Let $\lambda_0$ be a minimal element of the set of degrees of a finite generating system of M consisting of homogeneous elements $\neq 0$; then the hypotheses of Proposition 6 would be fulfilled, which implies a contradiction.

#### 系 2 {#alg-ii-s11-prop-6-cor-2 .statement tag=05YH}

*$\Delta$ と命題 6 の A に関する仮説を使用して、M を有限* 生成された等級付けされた $\mathbf{A}$ モジュールと、$\mathbf{N}$ を $\mathbf{N} + \mathfrak{J}_0 \mathbf{M} = \mathbf{M}$ となるような $\mathbf{M}$ の等級付けされた部分加群とします。次に$\mathbf{N} = \mathbf{M}$。

$\mathbf{M}/\mathbf{N}$ は有限生成された段階的 $\mathbf{A}$ モジュールであり、仮定は $\mathfrak{J}_0 . (\mathbf{M}/\mathbf{N}) = \mathbf{M}/\mathbf{N}$ を意味します。したがって $\mathbf{M}/\mathbf{N} = 0$ です。

#### 系 3 {#alg-ii-s11-prop-6-cor-3 .statement tag=05YI}

*命題 6 の $\Delta$ と $\mathbf{A}$ の仮説を使用して、$u : \mathbf{M} \to \mathbf{N}$ を段階的右 $\mathbf{A}$ モジュールの段階的準同型とし、$\mathbf{N}$ は有限に生成されると仮定します。 準同型*の場合

$$
u \otimes 1 : \mathbf{M} \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0) \to \mathbf{N} \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0)
$$

*が全射である場合、$u$は全射です。*

$u(\mathbf{M})$ は、$\mathbf{N}$ および $(\mathbf{A}/\mathfrak{J}_0)$ モジュールのグレード付けされた部分加群です

$$
(N/u(\mathbf{M})) \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0)
$$

は $(N \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0))/\mathrm{Im}(u \otimes 1)$ (§ 3, no. 6, 命題 6) と同型です。したがって、仮定は $(N/u(\mathbf{M})) \otimes_{\mathbf{A}} (\mathbf{A}/\mathfrak{J}_0) = 0$ を意味し、したがって系 1 による $\mathbf{N} = u(\mathbf{M})$ を意味します。

#### 注意 {#alg-ii-s11-n4-rem-1 .statement tag=05YJ}

It follows from the proof of Corollary 1 that Corollaries 1 and 2 (resp. Corollary 3) are still valid when, instead of assuming that $\mathbf{M}$ (resp. $\mathbf{N}$) is finitely generated, the following hypothesis is made: there exists a subset $\Delta^+$ of $\Delta$ satisfying the following conditions:

(1) $\lambda \notin \Delta^+$、$M_\lambda = \{0\}$ (それぞれ $N_\lambda = \{0\}$) の場合。
(2) $\Delta^+$ の空でないすべての部分集合には、少なくとも元があります。

これは、$\Delta = \mathbf{Z}$ と $\mathbf{M}$ (それぞれ $\mathbf{N}$) が *ポジティブ* 次数でグレード付けされた加群である場合に当てはまります。

#### 命題 7 {#alg-ii-s11-prop-7 .statement tag=05YK}

※$\Delta = \mathbf{Z}$とします。 命題 6 の $\mathbf{A}$ と $\mathbf{M}$ の仮説を使用して、等級付けされた $\mathbf{A}_0$ モジュール $\mathbf{N} = \mathbf{M}/\mathfrak{J}_0 \mathbf{M}$ を検討し、次の条件が成立すると仮定します。
(i) $\mathbf{A}_0$ モジュールとみなされるそれぞれの $N_\lambda$ は基底 $(y_{i\lambda})_{i \in I_\lambda}$ を認めます。
(ii) 標準準同型 $\mathfrak{J}_0 \otimes_{\mathbf{A}} \mathbf{M} \to \mathbf{M}$ は単射です。

この場合、$\mathbf{M}$ は段階的自由$\mathbf{A}$ モジュール (no. 2、注意 3) であり、正確に言うと、$x_{i\lambda}$ が $M_\lambda$ の元で、$N_\lambda$ の像が $y_{i\lambda}$ である場合、そのファミリーは$(x_{i\lambda})_{(i, \lambda) \in I}$ ($I$ は $I_\lambda$ の集合和) は、$\mathbf{M}$ の基底です。*

私たちは (no. 2, *注意 3*)、すべての$p(e_{i\lambda}) = x_{i\lambda}$ となるような、段階的な無料の $\mathbf{A}$ モジュール $\mathbf{L}$ (卒業 $(L_\lambda)$) と次数 0 の全射準同型 $p : \mathbf{L} \to \mathbf{M}$ があることを知っています。 $(i, \lambda) \in I$ ($(e_{i\lambda})_{(i, \lambda) \in I}$ は同種元 $e_{i\lambda} \in L_\lambda$ の $\mathbf{L}$ からなるの基底です)。上記の *注意* から、$p$ は *全射* であることがわかります。等級付けされた $\mathbf{A}$ モジュール $\mathbf{R} = \mathrm{Ker}(p)$ を考えて、定義による $\lambda < \lambda_0$ に対する $R_\lambda = \{0\}$ に注目してください。 $\mathbf{R} = \{0\}$ を証明する必要があり、命題 6 までに $\mathfrak{J}_0 R = R$ を証明すれば十分です。可換図式 (§ 3, no. 6, 命題 5) を考えてみましょう。

$$
\begin{array}{ccccccccc}
\mathfrak{J}_0 \otimes R & \xrightarrow{1 \otimes j} & \mathfrak{J}_0 \otimes L & \xrightarrow{1 \otimes p} & \mathfrak{J}_0 \otimes M & \longrightarrow & 0 \\
\downarrow a & & \downarrow b & & \downarrow c & & \\
0 & \longrightarrow & R & \xrightarrow{f} & L & \xrightarrow{p} & M & \longrightarrow & 0
\end{array}
$$

ここで、$j$ は標準単射、$a, b, c$ は標準単射 $\mathfrak{J}_0 \to A$ (§ 3, no. 4, 命題 4) から導出されます。 $a$ が全射であることを示さなければなりません。 $L$ は自由であるため、$b$ は単射 (§ 3, no. 7、系 6 から命題 7) であり、$c$ は仮定による単射であることに注意してください。次に、$t$ を $R$ の元とし、$t$ を $R / \mathfrak{J}_0 R$ の類とします。次に、完全系列 (§ 3, no. 6、命題 5、系 2 ～ 命題 6) があります。

$$
R / \mathfrak{J}_0 R \xrightarrow{j} L / \mathfrak{J}_0 L \xrightarrow{\bar{p}} M / \mathfrak{J}_0 M \longrightarrow 0
$$

ここで、$j$ と $\bar{p}$ は、移行から商まで、$\bar{p}$ は仮定全単射までのとき、$j$ と $p$ から導出されます。次に $j(\bar{t}) = 0$、他の場合は語 $j(t) \in \mathfrak{J}_0 L$ です。次に、$j(t) = b(z)$ となる元 $z \in \mathfrak{J}_0 \otimes L$ があります。 $p(b(z)) = 0$、$c((1 \otimes p)(z)) = 0$、そして$c$は単射なので、$(1 \otimes p)(z) = 0$。他の語では、$z$ は $1 \otimes j$ の下の元 $t' \in \mathfrak{J}_0 \otimes R$ の像であり、その後 $j(a(t')) = b(z) = j(t)$ になります。 $j$ は単射なので、これは $t = a(t')$ を意味します。

この命題を非評定加群に拡張する方法については、後で (可換代数、II, § 3, no. 2、命題 5) 示します。

#### 補題 1 {#alg-ii-s11-lem-1 .statement tag=05YL}

*可換群 $\Delta$ が、 $\Delta$ の群構造と互換性のある合計順序が $\Delta$ に存在するようにするには、 $\Delta$ がねじれなしであることが必要かつ十分です。

$\Delta$ にそのような位数構造が存在し、$\lambda > 0$ であれば、すべての $\mu \geq 0$ に対して $\lambda + \mu > 0$ となり、特に整数 $n > 0$、$n.\lambda > 0$ の帰納法によって、次のことが証明されます。 $\Delta$ にはねじれがありません ($\Delta$ のすべての元 $\neq 0$ は $> 0$ または $< 0$ のいずれかであるため)。逆に、$\Delta$ にねじれがない場合、$\Delta$ はベクトル $\mathbf{Q}$ 空間 (§ 7, no. 10、系 1 ～ 命題 26) のサブ$\mathbf{Z}$ モジュールであり、形と仮定できます。 $\mathbf{Q}^{(I)}$; $I$ に適切な順序 (*集合理論*、III, § 2, no. 3、定理 1) が与えられ、$\mathbf{Q}$ に通常の順序が与えられた場合、*辞書順* の集合 $\mathbf{Q}^{(I)}$ は完全に順序付けされます (*集合) 理論*、III, § 2, no. 6);この順序が $\mathbf{Q}^{(I)}$ の加法群構造と互換性があるのは明らかです。

#### 命題 8 {#alg-ii-s11-prop-8 .statement tag=05YM}

*$\Delta$ をねじりなし可換群とし、$A$ を型 $\Delta$ の段階的環とします。 2 つの同種元 $\neq 0$ の $A$ の積が $\neq 0$ である場合、環 $A$ には 0 の因子はありません。*

$\Delta$ に、その群構造 (補題) と互換性のある合計順序が与えられるとします。

1) $x = \sum_{\lambda \in \Delta} x_\lambda, y = \sum_{\lambda \in \Delta} y_\lambda$ を、$A$ の 2 つの非ゼロ元とする ($x_\lambda$ と $y_\lambda$ は、すべての $\lambda \in \Delta$ に対して次数 $\lambda$ と同次である)。 $\alpha$ (それぞれ $\beta$) を元 $\lambda \in \Delta$ の最大のとし、$x_\lambda \neq 0$ (それぞれ $y_\lambda \neq 0$) とします。 $\lambda \neq \alpha$ または $\mu \neq \beta$ の場合は、$x_\lambda y_\mu = 0$ または $\deg(x_\lambda y_\mu) < \alpha + \beta$ のいずれかが明らかです。したがって、次数 $\alpha + \beta$ の $xy$ の同次成分は $x_\alpha y_\beta$ となり、仮定までは非ゼロになります。 よって $xy \neq 0$。

### 5. グレードテンソル積 / グレード加群

$\Delta$ を可換モノイドとし、その単位元を 0、$A$ を型 $\Delta$ の段階的環、および $M$ (それぞれ $N$) を段階的右 (それぞれ左) とします。 型 $\Delta$ の $A$ モジュール。 $(A_\lambda)$ (それぞれ $(M_\lambda), (N_\lambda)$) を $A$ (それぞれ $M, N$) の卒業とします。 $\mathbf{Z}$ モジュール $M$ と $N$ のテンソル積 $M \otimes_{\mathbf{Z}} N$ は、$M_\lambda \otimes_{\mathbf{Z}} N_\mu$ (§ 3, no. 7、命題 7) の直和であるため、後者の形は *bigradation* です。この $\mathbf{Z}$ モジュールの型 $\Delta, \Delta$。 $M \otimes_{\mathbf{Z}} N$ で、この大卒業 (no. 1、*例 4*) に関連する型 $\Delta$ の *合計卒業* を考えてみましょう。これはサブ $\mathbf{Z}$ モジュール $P_\lambda = \sum_{\mu + \nu = \lambda} (M_\mu \otimes_{\mathbf{Z}} N_\nu)$ で構成されます。 元 $(xa) \otimes y - x \otimes (ay)$ によって生成されたサブ$\mathbf{Z}$ モジュール $Q$ により、$\mathbf{Z}$ モジュール $M \otimes_A N$ は $M \otimes_{\mathbf{Z}} N$ の商であることが知られています。ここで、$x \in M, y \in N$ と $a \in A$ (§ 3, no. 1);すべての $\lambda \in \Delta$、$x_\lambda, y_\lambda, a_\lambda$ がそれぞれ次数の同種成分、$\lambda$ の $x, y, a$ である場合、明らかに $(xa) \otimes y - x \otimes (zy)$ は同種元 $(x_\lambda a_\nu) \otimes y_\mu - x_\lambda \otimes (a_\nu y_\mu)$ の和です。 語 $Q$ は、$M \otimes_{\mathbf{Z}} N$ (no. 3、命題 2) および商の *グレード付き* サブ $\mathbf{Z}$ モジュールです。

$$
M \otimes_A N = (M \otimes_{\mathbf{Z}} N)/Q
$$

したがって、正規化された $\mathbf{Z}$ モジュール構造は型 $\Delta$ (no. 3) になります。さらに (no. 3、命題 5)、$A$ の *中心* $C$ は、$A$ のグレード部分環です。 $M \otimes_A N$ で定義した目盛りは、その加群構造と、段階付けされた環* $C$ と * 互換性があります。 $M \otimes_{\mathbf{Z}} N$ には標準的に *2 つの* $C$ モジュール構造があり、それぞれ $c(x \otimes y) = (xc) \otimes y$ と $(x \otimes y)c = x \otimes (cy)$ 、$x \in M, y \in N, c \in C$ (§ 3, no. 3) です。 $x \in M_\lambda, y \in N_\mu, c \in C \cap A_v$ の場合、2 つの元 $c(x \otimes y)$ と $(x \otimes y)c$ 属するから $(M \otimes_{\mathbf{Z}} N)_{\lambda + \mu + v}$ とその差属するから $Q$ 、したがって$M \otimes_A N$ の共通の像属するから $(M \otimes_A N)_{\lambda + \mu + v}$ までで、主張が確立されます。 *グレード* $C$-*加群* として $M \otimes_A N$ について話すとき、私たちは常にこのように定義された構造を意味し、それ以外の場合は 〜でない限りを意味します。 $(M \otimes_A N)_\lambda$ は、$x_\mu \otimes y_\nu$ ($x_\mu \in M_\mu, y_\nu \in N_\nu$ と $\mu + \nu = \lambda$) によって生成された $M \otimes_A N$ の加法群として定義できることに注意してください。

$M'$ (それぞれ $N'$) を右 (それぞれ左) $A$ モジュールの他のに格付けし、それぞれ次数 $\alpha$ および $\beta$ の準同型に格付けした $u : M \to M', v : N \to N'$ とします。次に、上記の発言からすぐに、$u \otimes v$ は次数 $\alpha + \beta$ の *グレード* (C モジュール) 準同型であることがわかります。

$A$ が可換である場合、等級 ($A$ モジュール構造と互換性のある) は、等級付き $A$ モジュールの有限数のテンソル積で同様に定義されます。さらに、$(M \otimes N) \otimes P \to M \otimes (N \otimes P)$ ($§ 3$、no. 8、命題 8) などの結合性同型は、*等級* 加群の同型であるのは明らかです。

#### 注意 {#alg-ii-s11-n5-rem-1 .statement tag=05YN}

$A$ が*自明な* 目盛 (no. 1、*例* 1) を持つ場合、$(M \otimes_A N)_\lambda$ は単に $\mu + \nu = \lambda$ のような $M \otimes_A N$ のサブ$Y$ モジュール $M_\mu \otimes_A N_\nu$ の直和になります。

$M$ (それぞれ $N$) を型 $\Delta$ の段階的右 (それぞれ 左) $A$ モジュール、$P$ 型 $\Delta$ の段階的 $\mathbf{Z}$ モジュール、$f$ を$M \times N$ から $P$ 満たす条件 (1) への $§ 3$、no. 1 などの $\mathbf{Z}$ 双線形写像
$$
f(x_\lambda, y_\mu) \in P_{\lambda+\mu} \quad \text{for } x_\lambda \in M_\lambda, y_\mu \in N_\mu, \lambda, \mu \text{ in } \Delta.
$$
次に、$f(x, y) = g(x \otimes y)$、ここで、$g : M \otimes_A N \to P$ は $\mathbf{Z}$ 線形マッピング ($§ 3$、no. 1、命題 1) であり、上記の条件から、$g$ は *次数付き* $\mathbf{Z}$ モジュールであることがわかります。 準同型/次数 0。

Let $B$ be another graded ring of type $\Delta$ and $\rho : A \to B$ a homomorphism of graded rings (no. 2); then $\rho^*(B_d)$ is a graded right $A$-module of type $\Delta$. $E$ が型 $\Delta$ の段階的左 $A$ モジュールであり、$\rho^*(B_d) \otimes_A E$ に上で定義された型 $\Delta$ の段階的 $\mathbf{Z}$ モジュール構造が与えられる場合、正規の左 $B$ モジュール構造 ($§ 5$, no. 1) の卒業に対応しています。
$$
E_{(B)} = \rho^*(E) = \rho^*(B_d) \otimes_A E.
$$
このようにして得られた段階的$B$加群は、スカラーの環を$\rho$によって$B$に拡張することによって得られると言われており、次数付き$B$加群として$E_{(B)}$または$\rho^*(E)$について話すときは、常にこの構造を意味します。 〜でない限り別途記載。

### 6. グレード加群 / グレード準同型

このNo.で推測します。モノイド $\Delta$ が *群* であること。 $A$ を、型 $\Delta$ のグレード付き環と、$M, N$ 2 つのグレード付き左 (たとえば) 型 $\Delta$ の $A$ モジュールとします。 $H_\lambda$ が準同型の次数* $\lambda$ の $M$ から $N$ (no. 2) に等級付けされた加法群を表すものとします。 加法群 $\mathrm{Hom}_A(M, N)$ の *すべて* 準同型の $M$ を $N$ (*非段階的* $A$ モジュール構造を使用) $H_\lambda$ の和 ($\lambda \in \Delta$ 用) は *直接* です。 なぜなら、すべての $\lambda$ に対して $u_\lambda \in H_\lambda$ を伴う関係 $\sum_\lambda u_\lambda = 0$ がある場合、すべての $\mu$ とすべての $x_\mu \in M_\mu$ に対して $\sum_\lambda u_\lambda(x_\mu) = 0$ が求まります。 $\Delta$の元はキャンセル可能であるため、$u_\lambda(x_\mu)$は次数$\lambda + \mu$の$\sum_\lambda u_\lambda(x_\mu)$の同次成分です。したがって、注文されたすべての対 $(\mu, \lambda)$ とすべての $x_\mu \in M_\mu$ に対して $u_\lambda(x_\mu) = 0$ となり、すべての $\lambda \in \Delta$ に対して $u_\lambda = 0$ が意味されます。 (この段落では) $\mathrm{Hom}_A(M, N)$ 和の $H_\lambda$ の加法部分群を $\mathrm{Homgr}_A(M, N)$ で表し、それを *次数付き* $A$-*加群準同型* の $M$ の加法群と呼ぶことにします。 $N$。 $C$ を $A$ の中心とします。これは、等級付けされた部分環 (no. 3、系 ～ 命題 5) です。 $\mathrm{Hom}_A(M, N)$ ($§ 1$、no. 14、*注意* 1) の標準的な $C$ モジュール構造の場合、$\mathrm{Homgr}_A(M, N)$ は *部分加群* であり、目盛り $(H_\lambda)$ は $C$ モジュール構造と *互換性* があります。 $c_v \in C \cap A_v$、$x_\mu \in N_\mu$、$u_\lambda \in H_\lambda$、そして定義 $(c_vu_\lambda)(x_\mu) = c_v.u_\lambda(x_\mu) \subset N_{\lambda+\mu+v}$、したがって$c_vu_\lambda \in H_{\lambda+v}$までです。

$M'$ と $N'$ を、型 $\Delta$ と $u': M' \to M$ の 2 つの等級付けされた左 $A$ モジュール、それぞれ次数 $\alpha$ と $\beta$ の $v': N \to N'$ 等級付けされた準同型とします。 Then it is immediate that $\mathrm{Hom}(u', v'): w \mapsto v' \circ w \circ u'$ maps $\mathrm{Homgr}_A(M, N)$ into $\mathrm{Homgr}_A(M', N')$ and that its restriction to $\mathrm{Homgr}_A(M, N)$ is a *graded* homomorphism into $\mathrm{Homgr}_A(M', N')$ *of degree* $\alpha + \beta$.

特に、$\mathrm{Homgr}_A(M, M)$ は、$\mathrm{End}_A(M)$ の *グレード付けされた部分環* であり、$\mathrm{Endgr}_A(M)$ で示されます。

#### 注意 {#alg-ii-s11-n6-rem-1 .statement tag=05YO}

$M$ と $N$ が左の $A$ モジュールにグレード付けされている場合、$\mathrm{Homgr}_A(M, N)$ は一般に $\mathrm{Hom}_A(M, N)$ とは異なります。ただし、$M$ が *有限生成* $A$ モジュールである場合、これら 2 つの集合は等しくなります。 $M$ は、同次元 $x_i$ ($1 \leq i \leq n$) の有限数によって生成されます。 $d(i)$ を $x_i$ の次数とします。 $u \in \mathrm{Hom}_A(M, N)$ とすべての $\lambda \in \Delta$ について、$z_{i,\lambda}$ は次数 $\lambda + d(i)$ の $u(x_i)$ の同種の成分を表すものとします。すべての $i$ に対して $u_\lambda(x_i) = z_{i,\lambda}$ となる準同型 $u_\lambda : M \to N$ が存在することを示します。 $1 \leq i \leq n$ に対して $a_i \in A$ を含む $\sum_i a_ix_i = 0$ がある場合、すべての $\lambda \in \Delta$ ($§ 1$、no. 7、*注意*) に対して $\sum_i a_iz_{i,\lambda} = 0$ であることを証明すれば十分です。すべての $i$ (no. 3, *注意* 1) に対して $d(i) + d'(i) = \mu$ となるように、各 $a_i$ は次数 $d'(i)$ と同次であると仮定できます。それから$\sum_i a_iu(x_i) = 0$;左側の次数 $\lambda + \mu$ の同次成分を取得すると、$\sum_i a_iz_{i,\lambda} = 0$、よってが得られ、準同型 $u_\lambda$ の存在がわかります。さらに、$u_\lambda$ は明らかに次数 $\lambda$ の *グレード* です。最後に、$\lambda$の値の有限の数と、定義による$u = \sum_\lambda u_\lambda$を除いた$u_\lambda = 0$は、主張を証明します。

In particular, $\mathrm{Homgr}_A(A_s, M) = \mathrm{Hom}_A(A_s, M)$ for every graded left $A$-module $M$; moreover $\mathrm{Hom}_A(A_s, M)$ has a *graded left A-module* structure (and not just a graded $C$-module structure), and it is immediate that with this structure the canonical mapping of $M$ into $\mathrm{Hom}_A(A_s, M)$ ($§ 1$, no. 14, *Remark* 2) is a *graded A-module isomorphism*.

同様に、$\mathrm{Homgr}_A(M, A_s)$ には *段階的な右A-加群* 構造があります (段階的な $C$ モジュール構造だけではありません)。これは、次数付き$A$モジュール$M$の*段階的双対*と呼ばれ、$M^{*\mathrm{gr}}$、または混乱が生じない場合は単に$M^*$で示されます。 $u : M \to N$ が次数 $\delta$ のグレーディング準同型である場合、上記のことから、${}^t u = \mathrm{Hom}(u, 1_{A_s})$ の制限から $N^{*\mathrm{gr}}$ は、グレーディングデュアル $N^{*\mathrm{gr}}$ のグレーディングデュアル $M^{*\mathrm{gr}}$ へのグレーディング準同型であることがわかります。 次数 $\delta$、$u$ の *グレード転置* と呼ばれます。

ときどきは、$\Delta$ (no. 1, 例 2) の同型 $\lambda \mapsto -\lambda$ を使用して、上記から導き出された段階的双対 $M^{*\mathrm{gr}}$ の目盛を考慮し、次数 $\lambda$ の同次元 $M^{*\mathrm{gr}}$ は、$M$ の次数* $-\lambda$ の等級付けされた線型形式です ($A$ に些細な卒業がある場合、これらは添字 $\mu \neq \lambda$ の $M_\mu$ の零線型形式です)。 次に、$u : M \to N$ が次数 $\delta$ のグレード準同型である場合、$u'$ は次数 $-\delta$ のグレード準同型になります。

$A$ が *可換* で、型 $\Delta$ の等級付けされ、$M, N, P, Q$ が型 $\Delta$ の 4 つの *等級付けされた* $A$ モジュールであるとします。次に、*正規に等級付けされた準同型 of 次数* 0 があります。

(3) $$
\operatorname{Homgr}_A(M, \operatorname{Homgr}_A(N, P)) \to \operatorname{Homgr}_A(M \otimes_A N, P)
$$
(4) $$
\operatorname{Homgr}_A(M, N) \otimes_A P \to \operatorname{Homgr}_A(M, N \otimes_A P)
$$
(5) $$
\operatorname{Homgr}_A(M, P) \otimes_A \operatorname{Homgr}_A(N, Q) \to \operatorname{Homgr}_A(M \otimes_A N, P \otimes_A Q)
$$
(テンソル積には no. 5 で定義された目盛りが与えられます) § 4 で定義された標準準同型を制限することによって得られます。 1、2、4。なぜなら、$u : M \to \operatorname{Homgr}_A(N, P)$ が次数 $\delta$ に等級付けされている場合、すべての $x \in M_\lambda$ について、$u(x)$ は次数 $\delta + \lambda$ の準同型 $N \to P$ であるため、$y \in N_\mu$、$u(x)(y) \in P_{\delta + \lambda + \mu}$ については、 $v : M \otimes_A N \to P$ 対応するが正規的に $u$ である場合、$v$ は、(3) に関して次数 $\delta$、よっての主張のグレード付けされた準同型であることがわかります。さらに、この準同型は *全単射 * であることがわかります。議論は (4) と (5) についても同様です。

(5) で特に $P = Q = A$ の場合、次数 0 の正規 *等級付け* 準同型が存在します。

(6) $$
M^{*\mathrm{gr}} \otimes_A N^{*\mathrm{gr}} \to (M \otimes_A N)^{*\mathrm{gr}}.
$$

### 練習問題 {#alg-ii-s11-exercises}

[§ 11 に対して練習問題](exercises/s11/)を参照してください。
