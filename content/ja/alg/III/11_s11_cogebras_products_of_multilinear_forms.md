---
book: alg
book_title: Algebra
chapter: III
chapter_title: TENSOR ALGEBRAS, EXTERIOR ALGEBRAS, SYMMETRIC ALGEBRAS
section: 11
section_title: Cogebras, products of multilinear forms, inner products and duality
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 574-611, 647-654
pdf_pages: 0598-0635, 0671-0678
extraction: ocr
subsections:
    - "no": 1
      title: COGEBRAS
      page: 574
      pdf_page: 598
    - "no": 2
      title: COASSOCIATIVITY, COCOMMUTATIVITY, COUNIT
      page: 578
      pdf_page: 602
    - "no": 3
      title: PROPERTIES OF GRADED COGEBRAS OF TYPE N
      page: 584
      pdf_page: 608
    - "no": 4
      title: BIGEBRAS AND SKEW-BIGEBRAS
      page: 585
      pdf_page: 609
    - "no": 5
      title: THE GRADED DUALS $T(M)^{*gr}$, $S(M)^{*gr}$ AND $\bigwedge(M)^{*gr}$
      page: 587
      pdf_page: 611
    - "no": 6
      title: 'INNER PRODUCTS: CASE OF ALGEBRAS'
      page: 594
      pdf_page: 618
    - "no": 7
      title: 'INNER PRODUCTS: CASE OF COGEbras'
      page: 597
      pdf_page: 621
    - "no": 8
      title: 'INNER PRODUCTS: CASE OF BIGEBRAS'
      page: 600
      pdf_page: 624
    - "no": 9
      title: INNER PRODUCTS BETWEEN $T(M)$ AND $T(M^*)$, $S(M)$ AND $S(M^*)$, $\Lambda(M)$ AND $\Lambda(M^*)$
      page: 603
      pdf_page: 627
    - "no": 10
      title: EXPLICIT FORM OF INNER PRODUCTS IN THE CASE OF A FINITELY GENERATED FREE MODULE
      page: 605
      pdf_page: 629
    - "no": 11
      title: ISOMORPHISMS BETWEEN $\wedge^p(M)$ AND $\wedge^{n-p}(M^*)$ FOR AN $n$-DIMENSIONAL FREE MODULE M
      page: 607
      pdf_page: 631
    - "no": 12
      title: APPLICATION TO THE SUBSPACE ASSOCIATED WITH A p-VECTOR
      page: 608
      pdf_page: 632
    - "no": 13
      title: PURE $p$-VECTORS. GRASSMANNIANS
      page: 609
      pdf_page: 633
statements: 40
exercises: 25
content_sha256: 89df8adc405067d2457db96b685800645d8ee8486f9d67b30fa6b1ccd7230b44
translated_from: content/en/alg/III/11_s11_cogebras_products_of_multilinear_forms.md
translation_method: google
source_content_sha256: d9e2a61c3971782f685be044252b3450406801250b05574efb54eb00ac04501c
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 9a05d32e38471ffc790a17d23ea7fb874012db387a012ef949057aff4747fecb
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 11。多重線形形式の余代数、積、内部積および双対性

この段落では、A は些細な卒業式で可換環です。 型 N の段階的 A-加群 M の場合、M^{gr} は型 N の段階的 A-加群を表します。その次数 n の同次元は、すべての k ≠ n について M_k 上で零である A 線形形式です。

### 1. 余代数

#### 定義 1 {#alg-iii-s11-def-1 .statement tag=067H}

A 上の cogebr a (または A-cogebra、または混乱が生じない場合は単に cogebr a) は集合 E で、構造は次のように定義されます。
(1) E の A-加群構造;
(2) A-線型写像 c: E → E ⊗_A E が E の余積と呼ばれる。

#### 定義 2 {#alg-iii-s11-def-2 .statement tag=067I}

2 つの余代数 E、E' があり、その余積がそれぞれ c と c' で表される場合、E から E' への射は、次のような A-線型写像 u: E → E' になります。
(1) $(u \otimes u) \circ c = c' \circ u,$ を他の語にすると、A-線型写像の可換図式になります。

$$
\begin{array}{ccc}
E & \xrightarrow{u} & E' \\
\downarrow c & & \downarrow c' \\
E \otimes_A E & \xrightarrow{u \otimes u} & E' \otimes_A E'
\end{array}
$$

恒等写像は射であり、2 つの射のうち合成は射であり、すべての全単射語射は同型であることがすぐに検証されます。

#### 例 {#alg-iii-s11-n1-exa-1 .statement tag=067J}

(1) 標準同型 $A \to A \otimes_A A$ (II, § 3, no. 5) 定義する A 上の A-cogebra 構造。

(2) E を余代数、$c$ をその余積、$\sigma$ を A-加群 $E \otimes_A E$ の正規の自己同型として、$x \in E, y \in E$ に対して $\sigma(x \otimes y) = y \otimes x$ とする。 A-線型写像 $\sigma \circ c$ 定義する E 上の新しい余代数構造により、構造 E は、指定された余代数 E の*反対* 余代数と呼ばれます。

(3) B を A-*代数* とし、$m : B \otimes_A B \to B$ を A-線型写像とし、B (§ 1, no. 3) で乗法を定義します。 転置 $^t m$ は、A-加群 B の双対 $B^*$ の A-線型写像から、A-加群 $B \otimes_A B$ の双対 $(B \otimes_A B)^*$ になります。 B が *有限生成射影* A-加群である場合、標準写像 $\mu : B^* \otimes_A B^* \to (B \otimes_A B)^*$ は A-加群同型 (II, § 4, no. 4) です。 写像 $c = \mu^{-1} \circ ^t m$ は、A-加群 B の *デュアル* $B^*$ で *余代数* 構造を定義する余積です。

(4) X を、A (II, § 1, no. 11) と $(e_x)_{x \in X}$ の係数を使用して、X の元の正式な線形結合の集合、$A^{(X)}$ A-加群とします。 $A^{(X)}$の標準基底。 A-線型写像 $c : A^{(X)} \to A^{(X)} \otimes_A A^{(X)}$ は条件 $c(e_x) = e_x \otimes e_x$ によって定義され、正規の余代数構造が $A^{(X)}$ で得られます。

(5) M を M (§ 5, no. 1) のA-加群と $T(M)$ テンソル代数とする。 II, § 3, no. 9 により、A-加群 $T(M)$ の A-加群 $T(M) \otimes_A T(M)$ には、A-線型写像 $c$ が 1 つだけ存在し、すべての $n \geq 0$ について、

$$
c(x_1 x_2 \ldots x_n) = \sum_{0 \leq p \leq n} (x_1 x_2 \ldots x_p) \otimes (x_{p+1} \ldots x_n)
$$

すべての$x_i \in M$ ($x_1 x_2 \ldots x_n$ は代数 $T(M)$ の積を示します)。したがって、$T(M)$ には *余代数* 構造が与えられます。

(6) M をA-加群と M (§ 6, no. 1) の対称代数である$S(M)$ とします。 M の対角線写像 $\Delta : x \mapsto (x, x)$ から $M \times M$ は A-線型写像なので、対応する準同型 A-代数 $S(M)$ の $S(\Delta)$ は A-代数 $S(M \times M)$ になります。 (§ 6, no. 2、命題 3)。一方、§ 6, no. 6 では、標準的な等級付けされた代数同型 $h : S(M \times M) \to S(M) \otimes_A S(M)$ を定義しました。したがって、合成によって *A-代数* 準同型が得られます。

$$
c = h \circ S(\Delta) : S(M) \to S(M) \otimes_A S(M),
$$

したがって、$S(M)$ に *余代数* 構造を定義します。すべての $x \in M$ について、§ 6, no. 6 で与えられた $h$ の定義 $S(\Delta)(x) = (x, x)$ と定義により、次のことがわかります。

$$
h((x, x)) = x \otimes 1 + 1 \otimes x.
$$

したがって、$c$ は一意な代数準同型となり、すべての $x \in M$ について、

(4)
$$
c(x) = x \otimes 1 + 1 \otimes x.
$$

$c$ は代数準同型であるため、$M$ の $n$ 元の数列 $(x_i)_{1 \leq i \leq n}$ ごとに、

(5)
$$
c(x_1 x_2 \ldots x_n) = \prod_{i=1}^n (x_i \otimes 1 + 1 \otimes x_i)
$$
$$
= \sum (x_{i_1} \ldots x_{i_p}) \otimes (x_{j_1} \ldots x_{j_{n-p}})
$$

(5) の右側の合計は、真に増加する数列のすべての注文された対を引き継ぎます (空の場合もあります)

$$
i_1 < i_2 < \cdots < i_p, \quad j_1 < j_2 < \cdots < j_{n-p}
$$

$\{1, n\}$の元の元の集合は補完的です。 元 $c(x_1 x_2 \ldots x_n)$ は、$S(M) \otimes_A S(M)$ の *合計次数* $n$ の元であり、その 2 度 $(p, n-p)$ の成分は、

(6)
$$
\sum_{\sigma} (x_{\sigma(1)} \ldots x_{\sigma(p)}) \otimes (x_{\sigma(p+1)} \ldots x_{\sigma(n)})
$$

ここで、合計は、区間 $\{1, p\}$ と $\{p+1, n\}$ のそれぞれの *増加する* であるすべての置換 $\sigma \in S_n$ に引き継がれます。

(7) Let $M$ be an $A$-module and proceed with the exterior algebra $\Lambda(M)$ as with $S(M)$ in *Example* 6; the diagonal mapping $\Delta : M \to M \times M$ this time defines a homomorphism $\Lambda(\Delta)$ of the $A$-algebra $\Lambda(M)$ into the $A$-algebra $\Lambda(M \times M)$ (§ 7, no. 2, Proposition 2); on the other hand there is a canonical graded algebra isomorphism

$$
h : \Lambda(M \times M) \to \Lambda(M)^g \otimes_A \Lambda(M)
$$

(§ 7, no. 7、命題 10)、よって by 合成には *代数* 準同型 $c = h \circ \Lambda(\Delta) : \Lambda(M) \to \Lambda(M)^g \otimes_A \Lambda(M)$ があり、これは $A$ モジュール準同型 $\Lambda(M) \to \Lambda(M) \otimes_A \Lambda(M)$ と見なすことができ、したがって定義するになります。 $\Lambda(M)$ *余代数* 構造。 *例* 6 のように、$c$ が一意な代数準同型であることが証明でき、すべての $x \in M$ について、

(7)
$$
c(x) = x \otimes 1 + 1 \otimes x,
$$

よって、$M$の元の数列$(x_i)_{1 \leq i \leq n}$ごとに、
$$
c(x_1 \wedge x_2 \wedge \cdots \wedge x_n) = (x_1 \otimes 1 + 1 \otimes x_1) \wedge \ldots \wedge (x_n \otimes 1 + 1 \otimes x_n)
$$
ここで、右側の積は代数に取り込まれます。
$$
\bigwedge(M)^{\mathfrak{g}} \otimes_A \bigwedge(M);
$$
計算するこの積に対して、真に増加するの数列 $i_1 < i_2 < \cdots < i_p,\ j_1 < j_2 < \cdots < j_{n-p}$ の元の $[1, n]$ のうち、元の集合が補完的であるすべての注文された対について、積を考慮してください。 $y_1 y_2 \ldots y_n$、ここで、$y_{i_h} = x_{i_h} \otimes 1$ ($1 \leq h \leq p$) と $y_{j_k} = 1 \otimes x_{j_k}$ ($1 \leq k \leq n - p$) および和は、これらすべての積を引き継ぎます。等級付けされた代数 $\bigwedge(M)^{\mathfrak{g}} \otimes_A \bigwedge(M)$ は反可換であり、元 $x_i \otimes 1$ と $1 \otimes x_i$ は、§ 4, no. 6、補題 3、補題 1 により合計次数 1 となるため、
$$(8)\quad c(x_1 \wedge x_2 \wedge \cdots \wedge x_n)$$
$$
= \sum (-1)^v (x_{i_1} \wedge \cdots \wedge x_{i_p}) \otimes (x_{j_1} \wedge \cdots \wedge x_{j_{n-p}})
$$
$v$ は、注文された対 $(h, k)$ の数であるため、$j_k < i_h$ となり、その合計は (5) と同じ集合に引き継がれます。 元 $c(x_1 \wedge \cdots \wedge x_n)$ は、$\bigwedge(M)^{\mathfrak{g}} \otimes_A \bigwedge(M)$ の *合計次数* $n$ であり、二次 $(p, n - p)$ の同次の成分は次と等しいです。
$$(9)\quad \sum_{\sigma} \varepsilon_\sigma (x_{\sigma(1)} \wedge \cdots \wedge x_{\sigma(p)}) \otimes (x_{\sigma(p+1)} \wedge \cdots \wedge x_{\sigma(n)})
$$
区間* $[1, p]$ と $[p + 1, n]$ のそれぞれに *増加するである置換 $\sigma \in S_n$ の合計が引き継がれます。

将来、$A^{(x)}, T(M), S(M)$ または $\bigwedge(M)$ を *余代数* として話すときは、特に記載のない場合は 〜でない限りを意味し、余代数構造はそれぞれ *例* 4、5、6、7 で定義されます。

(8) $E, F$ を 2 つの $A$-cogebra と $c, c'$ のそれぞれの余積とします。 $\tau : (E \otimes_A E) \otimes_A (F \otimes_A F) \to (E \otimes_A F) \otimes_A (E \otimes_A F)$ が、$E$ の $x, x'$ と $F$ の $y, y'$ に対する $\tau((x \otimes x') \otimes (y \otimes y')) = (x \otimes y) \otimes (x' \otimes y')$ のような結合性同型を表すものとします。次に、合成線形写像
$$
E \otimes_A F \xrightarrow{c \otimes c'} (E \otimes_A E) \otimes_A (F \otimes_A F) \xrightarrow{\tau} (E \otimes_A F) \otimes_A (E \otimes_A F)
$$
$A$ モジュール $E \otimes_A F$ の定義する余代数構造は、余代数 $E$ および $F$ の *テンソル積* と呼ばれます。

$E$ を余代数および $\Delta$ を可換モノイドとする。 $A$ モジュール $E$ の目盛り $(E_\lambda)_{\lambda \in \Delta}$ は、$c$ が段階的次数 $O$ の段階的準同型である場合、$E$ の余積* $c$ と *互換性があると言われます。 $A$ モジュール $E$ をグレード付き $A$ モジュール (型 $\Delta$) $E \otimes_A E$ に、他の語 (II, § 11, no. 5) に追加する場合
$$(10)\quad c(E_\lambda) \subset \sum_{\mu + \nu = \lambda} E_\mu \otimes_A E_\nu.$$

以下では、ほとんどの場合、極限型 $\mathbf{N}$ が余積と互換性があることに注目します。このような目盛を持つコゲブラは、*等級付きコゲブラ*とも呼ばれます。 F が他の等級付けされたコゲブラである場合、 * 等級付けされたコゲブラ射* $\phi : E \to F$ は、 定義による等級付けされたコゲブラ射 (定義 2) であり、これはまた、等級付けされた次数* 0 の * 等級付けされた準同型です。 A-加群。

#### 例 {#alg-iii-s11-n1-exa-2 .statement tag=067K}

(9) 上記で定義された余代数 $T(M)$、$S(M)$、$\Lambda(M)$ が余代数と評価されるのは、明らかです。

### 2. 共結合性、共可換性、余単位

E をコゲブラ、$c$ その余積、N、$N'$、$N''$ 3 つの A-加群、および $m$ を $N \times N'$ から $N''$ への双線形写像とします。 $\tilde{m} : N \otimes_A N' \to N''$ を A-線型写像対応する ～ $m$ とします。 $u : E \to N$、$v : E \to N'$ が 2 つの A-線型写像である場合、A-線型写像 $u \otimes v : E \otimes_A E \to N \otimes_A N'$ と E の合成 A-線型写像を$N''$ に導き出します。

$$
m(u, v) : E \xrightarrow{c} E \otimes_A E \xrightarrow{u \otimes v} N \otimes_A N' \xrightarrow{\tilde{m}} N''.
$$

明らかに、$\mathrm{Hom}_A(E, N) \times \mathrm{Hom}_A(E, N')$ から $\mathrm{Hom}_A(E, N'')$ への A 双線形写像 $(u, v) \mapsto m(u, v)$ を定義しました。

When E is a graded cogebrà, N, $N'$, $N''$ graded A-modules of the same type and $\tilde{m}$ a graded homomorphism of degree k of $N \otimes_A N'$ into $N''$, then, if $u$ (resp. $v$) is a graded homomorphism of degree $p$ (resp. $q$), $m(u, v)$ is a graded homomorphism of degree $p + q + k$.

#### 例 {#alg-iii-s11-n2-exa-1 .statement tag=067L}

(1) E を等級付き cogebrà $T(M)$ (no. 1) とし、N、$N'$、$N''$ が自明な等級を持つと仮定します。 A graded homomorphism of degree $-p$ of $T(M)$ into N (resp. $N'$, $N''$) then corresponds to a multilinear mapping of $M^p$ into N (resp. $N'$, $N''$). 多重線形写像 $u : M^p \to N$ と多重線形写像 $v : M^q \to N'$ を考えると、上記の方法により、$u$ の *積* ($m$ に相対) と呼ばれる多重線形写像 $m(u, v) : M^{p+q} \to N''$ を推定することができます。 $v$。 式 (3) (no. 1) と (11) は、M の $x_1, \ldots, x_{p+q}$ に対して、

$$
(m(u, v))(x_1, \ldots, x_{p+q}) = m(u(x_1, \ldots, x_p), v(x_{p+1}, \ldots, x_{p+q})).
$$

(2) N、$N'$、$N''$ について同じ仮説を維持して、E を段階的 cogebrà $S(M)$ (no. 1) とします。 A graded homomorphism of degree $-p$ of $S(M)$ into N then corresponds to a *symmetric multilinear mapping* of $M^p$ into N (§ 6, no. 3). 次に、対称多重線形写像 $u : M^p \to N$ と対称多重線形写像 $v : M^q \to N'$ から対称多重線形写像 $m(u, v) : M^{p+q} \to N''$ を導出します。これは (混乱を避けるために) $u._m v$ (または $u.v$) で表され、*対称と呼ばれます。 $u$ と $v$ の積* ($m$ に対して)。 式 (6) (no. 1) と (11) は、M の $x_1, \ldots, x_{p+q}$ に対して、

$$(u \cdot_m v)(x_1, \ldots, x_{p+q}) = \sum_\sigma m(u(x_{\sigma(1)}, \ldots, x_{\sigma(p)}), v(x_{\sigma(p+1)}, \ldots, x_{\sigma(p+q)}))$$

合計は、区間 $[1, p]$ および $[p+1, p+q]$ のそれぞれで増加するである置換 $\sigma \in \mathfrak{S}_{p+q}$ に引き継がれます。

(3) E を採点済みの余代数 $\bigwedge(M)$ (no. 1) とします。次に、交代的多重線形写像 $u : M^p \to N$ と交代的多重線形写像 $v : M^q \to N'$ 交代的多重線形写像 $m(u, v) : M^{p+q} \to N''$ から同様に推論します。これも $u \wedge_m v$ または$u \wedge v$ と、$u$ と $v$ の *交代的積* ($m$ に対して) と呼ばれます。式 (9) (no. 1) および (11) は、この場合、$M$ の $x_1, \ldots, x_{p+q}$ について、

$$(u \wedge_m v)(x_1, \ldots, x_{p+q}) = \sum_\sigma \varepsilon_\sigma m(u(x_{\sigma(1)}, \ldots, x_{\sigma(p)}), v(x_{\sigma(p+1)}, \ldots, x_{\sigma(p+q)}))$$

合計は再び区間 $[1, p]$ と $[p+1, p+q]$ の増加するである置換 $\sigma \in \mathfrak{S}_{p+q}$ に引き継がれます。

E が任意の等級付けされた余代数 (型 N の) である場合に戻り、3 つの加群 N、N'、N'' がすべて、型 $\mathbf{Z}$、写像の *等級付けされた A-代数* B の基礎となる A-加群に等しいと仮定します。 $m$ は B の乗法であるため、$\tilde{m} : B \otimes_A B \to B$ は次数 0 の等級付けされた A-線型写像になります。 したがって、等級付けされた A-加群 $\mathrm{Homgr}_A(E, B) = C$ に対して *等級付けされた A-代数* 構造が得られます。

特に、$B = A$ (自明な目盛り付き) と仮定すると、$\mathrm{Homgr}_A(E, A)$ は *等級付き双対* $E^{*gr}$ となり、等級付き A-代数構造になります。

F を他の等級付け余代数 $c'$ とし、その余積と $\phi : E \to F$ を余代数射 (no. 1) と等級付けします。その後、正規のグレードは射

$$\tilde{\phi} = \mathrm{Hom}(\phi, 1_B) : \mathrm{Homgr}_A(F, B) \to \mathrm{Homgr}_A(E, B)$$

*グレードは代数準同型*です。 $\mathrm{Homgr}_A(F, B)$ と $x \in E$ の $u, v$ については、

$$(\tilde{\phi}(uv))(x) = (uv)(\phi(x)) = m((u \otimes v)(c'(\phi(x)))).$$

しかし仮定 $c'(\phi(x)) = (\phi \otimes \phi)(c(x))$ までに、したがって

$$(u \otimes v)(c'((x))) = (\tilde{\phi}(u) \otimes \tilde{\phi}(v))(c(x))$$

したがって、$\tilde{\phi}(uv) = \tilde{\phi}(u)\tilde{\phi}(v)$ は、主張を証明します。

特に、等級付けされた転置 $^t\phi : F^{*gr} \to E^{*gr}$ は等級付けされた代数準同型です。

#### 注意 {#alg-iii-s11-n2-rem-1 .statement tag=067M}

$E_p$ が有限生成された射影 $A$ 加群であると仮定します。そのため、等級付けされた $A$ 加群 $(E \otimes_A E)^{*gr}$ および $E^{*gr} \otimes_A E^{*gr}$ は正規に識別できます (II, § 4, no. 4、系 1 から命題 4)。 $A$ モジュール $A \otimes_A A$ と $A$ も正規に識別される場合 (II, § 3, no. 4)、$E^{*gr}$ の定義する乗法である線形写像 $E^{*gr} \otimes_A E^{*gr} \to E^{*gr}$ は、余積のグレード化された転置と呼ぶことができます。 $c$。

#### 命題 1 {#alg-iii-s11-prop-1 .statement tag=067N}

※$E$を$A$より余代数とします。 位数では、すべての結合$A$-代数$B$、$A$-代数$\mathrm{Hom}_A(E, B)$ が結合である場合、余積 $c : E \to E \otimes_A E$ が図式* となることが必要かつ十分です。

$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
\downarrow c & & \downarrow l_E \otimes c \\
E \otimes_A E & \xrightarrow{c \otimes l_E} & E \otimes_A E \otimes_A E
\end{array}
$$

*可換的であること*

$B$ を連想 $A$-代数、$u, v, w$ 3 つの元を $C = \mathrm{Hom}_A(E, B)$ とします。 $m_3$ が写像 $b \otimes b' \otimes b''$ から $bb'b''$ までの $A$ 線形写像 $B \otimes_A B \otimes_A B \to B$ を表すものとします。 代数 $C$ の積の定義により、$(uv)w$ は合成写像になります

$$
E \xrightarrow{c} E \otimes E \xrightarrow{c \otimes 1_E} E \otimes E \otimes E \xrightarrow{u \otimes v \otimes w} B \otimes B \otimes B \xrightarrow{m_3} B
$$

一方、$u(vw)$ は合成写像です

$$
E \xrightarrow{c} E \otimes E \xrightarrow{l_E \otimes c} E \otimes E \otimes E \xrightarrow{u \otimes v \otimes w} B \otimes B \otimes B \xrightarrow{m_3} B.
$$

図式 (12) が可換である場合、代数 $\mathrm{Hom}_A(E, B)$ はすべての結合$A$-代数 $B$ に対して結合であるということになります。 逆を確立するには、写像 $m_3 \circ (u \otimes v \otimes w)$ $E \otimes E \otimes E$ となるような結合$A$-代数 $B$ と $E$ から $B$ への 3 つの $A$ 線形写像 $u, v, w$ が存在することを示すだけで十分です。 into $B$ は単射です。 $B$ を $A$-代数 $\mathscr{T}(E)$ と $E$ の $u, v, w$ 標準写像を $\mathscr{T}(E)$ に代入します。 写像 $m_3 \circ (u \otimes v \otimes w)$ は標準写像 $E \otimes E \otimes E = \mathscr{T}^3(E) \to \mathscr{T}(E)$ となり、単射法になります。

余代数 $E$ が命題 1 の条件を満たすとき、それは共結合的であると言われます。

#### 例 {#alg-iii-s11-n2-exa-2 .statement tag=067O}

(4) 余代数 $A$ (no. 1, 例 (1)) 余代数 $A^{(X)}$ (no. 1, 例 4) および余代数 $\mathscr{T}(M)$ がすぐに検証されます。 (no. 1、例 5) は共結合です。 $B$ が有限生成射影 $A$ 加群である結合 $A$ 代数である場合、余代数 $B^*$ (no. 1, 例 3) は結合可換性の図式に対して共結合です。 (12) は、図式の転置によって続き、$B$ (§ 1, no. 3) の結合性を表します。逆に、同じ議論と、A-加群 B とその二双対数 (II, § 2, no. 7、系 4 ～ 命題 13) の標準的同定は、余代数 B* が共結合である場合、代数 B は結合であることを示しています。最後に、余代数 S(M) と $\Lambda(M)$ (no. 1、例 6 および 7) は共結合です。これは図式の可換性から続きます

$$
\begin{array}{ccc}
M & \xrightarrow{\Delta} & M \times M \\
\downarrow & & \downarrow 1_M \times \Delta \\
M \times M & \xrightarrow{\Delta \times 1_M} & M \times M \times M
\end{array}
$$

S(M) (§ 6, no. 2) と $\Lambda(M)$ (§ 7, no. 2) の関数的性質。これは対応する可換図式を与えます

$$
\left\{
\begin{array}{ccc}
S(M) & \xrightarrow{S(\Delta)} & S(M \times M) \\
\downarrow S(\Delta) & & \downarrow S(\Delta_M \times 1) \\
S(M \times M) & \xrightarrow{S(\Delta \times 1_M)} & S(M \times M \times M)
\end{array}
\right.
$$
$$
\left\{
\begin{array}{ccc}
\Lambda(M) & \xrightarrow{\Lambda(\Delta)} & \Lambda(M \times M) \\
\downarrow \Lambda(\Delta) & & \downarrow \Lambda(1_M \times \Delta) \\
\Lambda(M \times M) & \xrightarrow{\Lambda(\Delta \times 1_M)} & \Lambda(M \times M \times M)
\end{array}
\right.
$$

そして、直和 (§ 6, no. 6 と § 7, no. 7) の対称および外部代数に対する標準同型の存在と関数性。

#### 命題 2 {#alg-iii-s11-prop-2 .statement tag=067P}

*E を A 上の余代数とする。位数では、すべての可換 A-代数 B に対して、A-代数 $\mathrm{Hom}_A(E, B)$ が可換であるため、余積 $c : E \to E \otimes_A E$ が図式* となることが必要かつ十分である。

$$
\begin{array}{ccc}
E & & \\
 & \swarrow_c & \searrow_c \\
E \otimes_A E & \xrightarrow{\sigma} & E \otimes_A E
\end{array}
$$

(ここで、$\sigma$ は、$\sigma(x \otimes y) = y \otimes x$ となるような対称性準同型) は *可換*です (他の語では、余代数 E がその反対* (no. 1, 例 2) と *同一であれば十分です。

B を $C = \mathrm{Hom}_A(E, B)$ の 2 つの元と $u, v$ の可換A-代数とする。

C の積の定義により、$uv$ と $vu$ はそれぞれ合成写像と等しくなります。

$$
E \xrightarrow{c} E \otimes E \xrightarrow{u \otimes v} B \otimes B \xrightarrow{m} B
$$

そして

$$
E \xrightarrow{c} E \otimes E \xrightarrow{v \otimes u} B \otimes B \xrightarrow{m} B.
$$

図式 (15) が可換である場合、代数 $\mathrm{Hom}_A(E, B)$ は、すべての可換 A-代数 B に対して可換であることがわかります。 逆を確立するには、1 つの可換 A-代数 B と 2 つの A-線型写像が存在することを示すだけで十分です。 $m \circ (u \otimes v): E \otimes E \to B$ が単射となるように、E の $u, v$ を B に変換します。 B を、E の標準写像 $E \oplus E \to S(E \oplus E)$ の代数 $S(E \oplus E)$ と $u$ (それぞれ $v$) 合成と、E の写像 $x \mapsto (x, 0)$ (それぞれ $x \mapsto (0, x)$) を $E \oplus E$ にします。 $h: S(E) \otimes S(E) \to S(E \otimes E)$ が標準同型 (§ 6, no. 6、命題 9) で、$\lambda: E \to S(E)$ が標準写像の場合、$h^{-1} \circ m \circ (u \otimes v) = \lambda \otimes \lambda$ です。ここで、$\lambda \otimes \lambda$ は単射法です。なぜなら、$\lambda(E)$ は $S(E)$ の直因子 (II, § 3, no. 7、系 5 から命題 7) です。

余代数 E が命題 2 の条件を満たすとき、それは共可換であると言われます。

#### 例 {#alg-iii-s11-n2-exa-3 .statement tag=067Q}

(5) 余代数 A (no. 1, 例 1) と余代数 $A^{(X)}$ (II, § 11, no. 1, 例 4) が共可であるのは明らかです。 no. 1 の公式 (5) から、余代数 $S(M)$ は共可換であることがわかります。最後に、A-加群 B が射影であり、余代数 $B^*$ (no. 1, 例 3) が共可換である性質をもつように有限生成される A-代数 B の場合、B が可換であることが必要かつ十分です。 (A-加群 B とその双対 (II, § 2, no. 7) の正規同定を使用する) とすると、これは、図式 (14) の可換性が B (§ 1, no. 3) の可換性を表現した図式と転置により等価であるという事実から導かれます。

#### 命題 3 {#alg-iii-s11-prop-3 .statement tag=067R}

*E を A 上の余代数とします。位数では、すべての単位 A-代数 B に対して、A-代数 $\mathrm{Hom}_A(E, B)$ が単位であるため、可換図式をレンダリングする E 上に線型形式 $\gamma$ が存在することが必要かつ十分です*

$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
& & \downarrow \gamma \otimes 1_E \\
& & A \otimes_A E
\end{array}
$$
$h'$

$$
\begin{array}{ccc}
E & \xrightarrow{c} & E \otimes_A E \\
& & \downarrow 1_E \otimes \gamma \\
& & E \otimes_A A
\end{array}
$$
$h''$

ここで、$c: E \to E \otimes_A E$ は余積、$h'$、$h''$ 標準同型です。

(II, § 3, no. 4、命題 4)。 * Hom$_A$(E, B) の *単位元 * は、線形写像* x $\mapsto$ $\gamma(x)1$ (1 は B の単位元を表します)。

図式 (16) 可換である E レンダリングで $\gamma$ を線型形式とします。 B を A-代数 C = Hom$_A$(E, B) の単位元 1、$\eta:A \to B$ 標準写像および $v = \eta \circ \gamma$ 元をもつ単位 A-代数とする。 元 $u \in C$ ごとに、$uv$ は合成写像です

$$
\text{(17)} \quad E \xrightarrow{c} E \otimes E \xrightarrow{1_E \otimes \gamma} E \otimes A \xrightarrow{u \otimes \eta} B \otimes B \xrightarrow{m} B.
$$

次に$uv = m \circ (u \otimes \eta) \circ h'' = u$。同様に、$vu = u$、したがって$v$ は、C の単位元であることが証明されます。逆に、A-加群 A $\oplus$ E に単位代数構造が与えられ、A の $a, a'$ と E の $x, x'$ に対して $(a, x)(a', x') = (aa', ax' + a'x)$ が与えられます。B はこのように定義された A-代数を表し、C はA-代数ホム$_A$(E、B)。 C が単体であると仮定し、$e:x \mapsto (\gamma(x), \lambda(x))$ をその単位元とします (ここで、$\gamma(x) \in A$ と $\lambda(x) \in E$)。一方、$f$をCの元$x \mapsto (0, x)$とします。 明らかの計算により、$fe$ は元であることがわかります

$$
x \mapsto (0, (h'')^{-1}((1_E \otimes \gamma)(c(x))))
$$

Cの。 条件 $fe = f$ は、(16) の 2 番目の図式の可換性を暗示し、同様に、条件 $ef = f$ は、(16) の最初の図式の可換性を暗示していることがわかります。

線型形式 $\gamma$ E レンダリング図式 (16) 可換は余代数 E の *余単位* と呼ばれます。 余代数は *最大 1 つ* 余単位を認めます: なぜなら、それは単位元であるからです。 代数ホム$_A$(E、A)。 余代数と余単位は *共同* と呼ばれます。

#### 例 {#alg-iii-s11-n2-exa-4 .statement tag=067S}

(6) 恒等写像は余代数 A の余単位です。 余代数 A$^{(X)}$ (no. 1, *例 4*) 線型形式 $\gamma$ では、すべての $x \in X$ に対する $\gamma(e_x) = 1$ は余単位になります。 余代数 T(M) (それぞれ S(M)、$\Lambda(M)$) 線型形式 $\gamma$ では、$T^n(M)$ (それぞれ $S^n(M)$、$\Lambda^n(M)$) の $z$ に対して $\gamma(1) = 1$ と $\gamma(z) = 0$ $n \geq 1$は余単位です。最後に、B を A-代数とします。これは有限生成射影 A-加群であり、単位元 $e$ を持ちます。次に、余代数 B* (no. 1, *例 3*) 線型形式 $\gamma: x^* \mapsto \langle e, x^* \rangle$ は余単位です。これは、形は、A の A-線型写像 $\eta_e: \xi \mapsto \xi e$ の転置を B に転置したものにすぎません。 図式 (16) の可換性は、$e$ が B (§ 1, no. 3) の単位元であるという事実を ($\eta_e$ を使用して) 表す図式から続きます。さらに、同じ議論は、逆に、余代数 B* が余単位 $\gamma$ を認めた場合、B の $\gamma$ 定義する単位元 $e = t_\gamma(1)$ の転置が認められることを示しています。

#### 命題 4 {#alg-iii-s11-prop-4 .statement tag=067T}

*E を余単位 $\gamma$ を認める余代数とし、$\gamma(e) = 1$ となるような e 元 e が E に存在すると仮定します。この場合、E はサブ A モジュール Ae の直和と $E_{\gamma} = \mathrm{Ker}(\gamma)$ であり、*

$$
\text{(18)} \quad \begin{cases}
c(e) \equiv e \otimes e \pmod{E_{\gamma} \otimes E_{\gamma}} \\
c(x) \equiv x \otimes e + e \otimes x \pmod{E_{\gamma} \otimes E_{\gamma}} & \text{for all } x \in E_{\gamma}.
\end{cases}
$$

最初の主張は明らかで、$\gamma(x - \gamma(x)e) = 0$ と関係 $\gamma(\alpha e) = 0$ は $\alpha = 0$ を意味します。 $c(e) = \sum_i s_i \otimes t_i$ にしましょう。
$$
e = \sum_i \gamma(s_i)t_i = \sum_i \gamma(t_i)s_i
$$
(16) と $1 = \gamma(e) = \sum_i \gamma(s_i)\gamma(t_i)$ による。したがって、
$$
\sum_i (s_i - \gamma(s_i)e) \otimes (t_i - \gamma(t_i)e) = \sum_i s_i \otimes t_i - \sum_i e \otimes \gamma(s_i)t_i \\
- \sum_i \gamma(t_i)s_i \otimes e \\
+ \sum_i \gamma(s_i)e \otimes \gamma(t_i)e
$$
上記の関係により、これはちょうど $c(e) - e \otimes e$ になります。したがって、これは (18) の最初の関係を証明します。一方、$E \otimes E$の分解は直和となります
$$
A(e \otimes e) \oplus ((Ae) \otimes E_\gamma) \oplus (E_\gamma \otimes (Ae)) \oplus (E_\gamma \otimes E_\gamma)
$$
これにより、$x \in E_\gamma$、$c(x) = \lambda(e \otimes e) + (e \otimes y) + z \otimes e) + u$、$u = \sum_j v_j \otimes w_j, y, z$、$v_j$、$w_j$、属するから$E_\gamma$までを書くことができます。 余単位 $\gamma$ の定義は $x = \lambda e + y = \lambda e + z$ を与え、$\gamma(x) = 0$ として必然的に $\lambda = 0, x = y = z$、よっては (18) の 2 番目の関係になります。

#### 注意 {#alg-iii-s11-n2-rem-2 .statement tag=067U}

C を結合共結合 A-coalgebra、B を単位結合 A-代数、M 左B-加群とする。 $B \times M$ の A 双線形写像 $(b, m) \mapsto bm$ を M 定義するへの A 双線形写像
$$
\operatorname{Hom}_A(C, B) \times \operatorname{Hom}_A(C, M) \to \operatorname{Hom}_A(C, M)
$$
この番号の冒頭に記載されている一般的な手順に従ってください。この写像で定めるが $\operatorname{Hom}_A(C, M)$ 左加群構造上で環 $\operatorname{Hom}_A(C, B)$ であることがすぐに検証されます。

### 3. 型 N のグレーディング余代数の特性

#### 命題 5 {#alg-iii-s11-prop-5 .statement tag=067V}

(i) *E を余単位 $\gamma$ を認める採点余代数とする。この場合、$\gamma$ は次数 0 の同次線型形式です。*

(ii) *さらに、$E_0 = Ae$ と $\gamma(e) = 1$ のような元 $e \in E$ が存在するとします。すると、$\gamma$ の核 $E_\gamma$ は、$E_+ = \sum_{n \geq 1} E_n$、$c(e) = e \otimes e$、および * に等しくなります。
$$
c(x) \equiv x \otimes e + e \otimes x \ (\text{mod. } E_+ \otimes E_+)
$$
*全員に* $x \in E_+$。

(i) $x \in E_n$ に対して、すべての $n \geq 1$ に対して $\gamma(x) = 0$ であることを検証するだけで十分です。 $c$ は次数 0 の準同型であるため、

$$
c(x) = \sum_{0 \leq j \leq n} \left( \sum_i y_{ij} \otimes z_{i, n-j} \right)
$$

$E_j$ の $0 \leq j \leq n$、$y_{ij}$、$z_{ij}$ などのすべての $j$ について; 適用 (16) (no. 2) を取得します

$$
x = \sum_{0 \leq j \leq n} \left( \sum_i \gamma(y_{ij}) z_{i, n-j} \right) = \sum_{0 \leq j \leq n} \left( \sum_i \gamma(z_{i, n-j}) y_{ij} \right),
$$

よって、両側の次数 0 および次数 $n$ の成分に等しい

$$
x = \sum_i \gamma(y_{i0}) z_{in} = \sum_i \gamma(z_{i0}) y_{in}
$$
$$
0 = \sum_i \gamma(y_{in}) z_{i0} = \sum_i \gamma(z_{in}) y_{i0}
$$

したがって $\gamma(x) = \sum_i \gamma(y_{in}) \gamma(z_{i0}) = \gamma(0) = 0$ です。

(ii) (i) により、$\mathrm{Ker}(\gamma)$ と $E_+$ は両方とも $Ae = E_0$ と $E_+ \subset \mathrm{Ker}(\gamma)$ の補助サブモジュールであるため、$E_+ = \mathrm{Ker}(\gamma)$ (II, § 1, no. 8, 注意 1)。残りの主張は、no. 2 の命題 4 から続きます。

#### 命題 6 {#alg-iii-s11-prop-6 .statement tag=067W}

*E を A の等級付けされた余代数とします。 位数では、すべての可換 A-代数 B に対して、自明な段階を使用して、型 $\mathbf{Z} \mathrm{Homgr}_A(E, B)$ (no. 2) の等級付けされた A-代数が反可換 (§ 4, no. 9, 定義 7) であるとします。 $\sigma_g$ が A-加群 $E \otimes_A E$ の自己同型を表す場合、* は必要十分です*

$$
\sigma_g(x_p \otimes x_q) = (-1)^{pq} x_q \otimes x_p
$$

for $x_p \in E_p, x_q \in E_q$, *where p and q are arbitrary elements of $\mathbf{N}$, the diagram*

$$
\begin{array}{ccc}
E & & \\
 & \searrow^c & \swarrow^c \\
E \otimes_A E & \xrightarrow{\sigma_g} & E \otimes_A E
\end{array}
$$

*可換的であること*

証明は、no. 2 の命題 2 に類似しています。

等級付けされた余代数 E が命題 6 の条件を満たす場合、それは *反共換性 * であると言われます。

#### 例 {#alg-iii-s11-n3-exa-1 .statement tag=067X}

no. 1 の公式 (8) から、すべての A-加群 M に対して、等級付けされた余代数 $\bigwedge(M)$ は *反共可換* であることがわかります。

### 4. ビジェブラとスキュービジェブラ

#### 定義 3 {#alg-iii-s11-def-3 .statement tag=067Y}

*環 A 上の等級付き双数 (それぞれスキュー等級付き双数) は集合 E で、型 $\mathbf{N}$ の等級付き A-代数構造と、型 $\mathbf{N}$ の等級付き A 共形体構造があり、基礎となる等級は同じですA-加群構造など:*

(1) *A-代数 E は結合的かつ単体です。*

(2) *A-cogebra E は共結合的で共同結合的です。*
(3) *余積 c : E \to E \otimes_A E は、段階的代数 E の準同型から段階的代数 E \otimes_A E* (それぞれ *段階的代数 E^g \otimes_A E* (cf. § 4, no. 7)))。
(4) E の *余単位 $\gamma$ は、代数 E を代数 A に段階的に変換したもの (自明な目盛り付き) の準同型であり、e が A-代数 E の単位元を表す場合、$\gamma(e) = 1$。

E が、その卒業が *trivial* である等級付き双眼鏡である場合、E は単に *bigebra* と呼ばれます。基礎となる代数が可換である場合 (基礎となる余代数が共可換である場合)、段階的双晶は可換 (または共可) と呼ばれます。基礎となる等級代数が反可換性である場合 (それぞれ、基礎となる等級余代数が反共可換性である場合)、スキュー等級双晶は反可換性 (それぞれ反共可換性) と呼ばれます。

定義 3 と no. 2, 命題 5 から、段階的双眼鏡またはスキュー段階的双眼鏡 E の場合、次のことがわかります。

$$
c(e) = e \otimes e \\
c(x) \equiv x \otimes e + e \otimes x (\text{mod. } E_+ \otimes E_+) \quad \text{for } x \in E_+ = \bigoplus_{n \geq 1} E_n.
$$

E と F が 2 つの等級付き双晶 (それぞれ 2 つの傾斜傾斜双晶) である場合、次の場合、写像 $\phi : E \to F$ は *傾斜傾斜双晶射* (それぞれ *傾斜傾斜双晶射*) と呼ばれます: (1) $\phi$ が傾斜傾斜代数射 (したがって、E の写像単位元から F の単位元); (2) $\phi$ は、余代数射であり、$\gamma$ と $\gamma'$ がそれぞれ E と F の余単位である場合、$\gamma = \gamma' \circ \phi$ になります。

#### 例 {#alg-iii-s11-n4-exa-1 .statement tag=067Z}

(1) Let S be a monoid with identity element u, so that the algebra $E = A^{(S)}$ of the monoid S over A admits the unit element $e_u$ (§ 2, no. 6); it has been seen on the other hand that E has canonically a coassociative cocommutative A-cogebra structure with a counit $\gamma$ such that $\gamma(e_s) = 1$ for all $s \in S$ (no. 1, Example 4 and no. 2, Examples 4, 5 and 6). 公式 $c(e_s) = e_s \otimes e_s$ に余積を与えると、c が代数準同型であることがすぐにわかります。 したがって、*共可換双数* 構造が E および E 上で定義されており、この構造は A* 上のモノイド S の *大数と呼ばれます。

T が $f(u) = v$ と $f_{(A)} : A^{(S)} \to A^{(T)}$ A-代数準同型が $f$ (§ 2, no. 6) から導出されるように、単位元 v、$f : S \to T$ 準同型をもつ他のモノイドである場合、$f_{(A)}$ が *bigebra であることがすぐに検証されます。 準同型*。

(2) M をA-加群とします。等級付き A-代数 (§ 6, no. 1) と等級付き A-cogebra (no. 1, 例 6) 構造は S(M) 定義するでこの集合上で *可換共可級等数* 構造で定義されます。なぜなら、S(M) の余積は *代数* 準同型であり、余単位 $\gamma$ (no. 2, 例 6) の定義から次のことが分かるからです (no. 1, 例 6)。 $\gamma(1) = 1$ そしてその $\gamma$ は E の代数準同型を A に変換します。

(3) M をA-加群とします。 例 2 のように、等級付けされた A-代数 (§ 7, no. 1) と等級付けされた A-cogebra (no. 1, 例 7) 構造が $\bigwedge(M)$ 定義するにこの集合で *反可換反共換スキューが等級付けされたことがわかります。ビゲブラ* 構造。

#### 注意 {#alg-iii-s11-n4-rem-1 .statement tag=0680}

M が $M \otimes_A M \neq \{0\}$ のような A-加群の場合、一般に、$T(M)$ 上の等級付けされた A-代数 (§ 5, no. 1) および等級付けされた A-cogebra (no. 1、例 5) 構造 *は定義する* 構造ではありません。

$$
c(x_1 x_2 y_1 y_2) \neq c(x_1 x_2) c(y_1 y_2)
$$

M の 4 つの元 $x_1, x_2, y_1, y_2$ については、no. 1 の公式 (3) が示しています。

### 5. グレードデュアル $T(M)^{*gr}$、$S(M)^{*gr}$、$\bigwedge(M)^{*gr}$

*これ以降、代数での章の一般的な規則に戻ります。したがって、これは (〜でない限り別途言及) 結合的かつ単体であると想定されます。

Let M be an A-module; the graded A-cogebra structures defined on $T(M)$ (no. 1, Example 5), $S(M)$ (no. 1, Example 6) and $\bigwedge(M)$ (no. 1, Example 7) allow us to define canonically on the graded duals $T(M)^{*gr}$, $S(M)^{*gr}$ and $\bigwedge(M)^{*gr}$ *graded algebra* structures of type N, by virtue of no. 2, Propositions 1 and 3 and the convention made on the graduation of the graded dual of a graded module (no. 1). さらに、等級付けされた代数 $S(M)^{*gr}$ は *可換* (no. 2、命題 2 および例 5) であり、等級付けされた代数 $\bigwedge(M)^{*gr}$ は *反可換* (no. 3、命題 6 および例) です。 $\bigwedge(M)^{*gr}$ * 次数 1 のすべての元は零平方* です。このような元は M 上の線型形式 $f$ と識別され、その平方は $M^2$ 上の交代的双線形形式 $f \wedge f$ であるようになります。

$$
(f \wedge f)(x, y) = f(x) f(y) - f(y) f(x)
$$

(no. 2、例 3)。

N を M から N への他の A-加群および $u$ A-線型写像とします。$u$ 定義するが標準的に等級付けされていることがわかります代数準同型

$$
\begin{cases}
T(u): T(M) \to T(N) \\
S(u): S(M) \to S(N) \\
\bigwedge(u): \bigwedge(M) \to \bigwedge(N)
\end{cases}
$$

(§ 5, no. 2、§ 6, no. 2、§ 7, no. 2)。 no. 1 の公式 (3) で、$T(u)$ も *余代数射* であることがすぐに検証されます。一方、$\Delta_M$ (それぞれ $\Delta_N$) が対角線写像 $M \to M \times M$ (それぞれ $N \to N \times N$) を表す場合、関係 $(u \times u) \circ \Delta_M = \Delta_N \circ u$ があります。つまり$S(u \times u) \circ S(\Delta_M) = S(\Delta_N) \circ S(u)$

(それぞれ $\Lambda(u \times u) \circ \Lambda(\Delta_M) = \Lambda(\Delta_N) \circ \Lambda(u)$)。

$S(M)$ と $\Lambda(M)$ (no. 1、例 6 と 7) で余積の定義と標準同型の関数関数指標を使用する

$$
S(M \times M) \to S(M) \otimes_A S(M)
$$

と $\Lambda(M \times M) \to \Lambda(M)^{\text{g}} \otimes_A \Lambda(M)$ では、$S(u)$ と $\Lambda(u)$ も *余代数射*† (したがって、この場合は *bigebra* 射) であることがわかります。 *採点された転置* (II, § 11, no. 6) は準同型 (23) ということになります。

$$
\begin{align*}
tT(u): T(N)^{*gr} &\to T(M)^{*gr} \\
tS(u): S(N)^{*gr} &\to S(M)^{*gr} \\
t\Lambda(u): \Lambda(N)^{*gr} &\to \Lambda(M)^{*gr}
\end{align*}
$$

*採点は代数準同型*です。

ここで、$M$ の二重 $M^*$ が、$T(M)^{*gr}$ (それぞれ $S(M)^{*gr}$、$\Lambda(M)^{*gr}$) の次数 1 の元の部分加群と識別されることに注目します。したがって、テンソル代数 (§ 5, no. 1) の普遍性と対称代数 (§ 6, no. 1) の普遍性から、 *等級付けされた代数準同型は 1 つだけ存在します*

$$
\theta_T: T(M^*) \to T(M)^{*gr}
$$

*どれが拡大する標準単射* $M^* \to T(M)^{*gr}$、*そして 1 つだけが代数準同型* と評価されました

$$
\theta_S: S(M^*) \to S(M)^{*gr}
$$

*どれ拡大する標準単射* $M^* \to S(M)^{*gr}$。 一方、$\Lambda(M)^{*gr}$ の*反対* 代数の $M^*$ の標準単射は、$M^*$ のすべての元の平方が零になります。したがって (§ 7, no. 1, 命題 1) *等級付けされた代数準同型は 1 つだけ存在します*

$$
\theta_\Lambda: \Lambda(M^*) \to (\Lambda(M)^{*gr})^0
$$

*どれ拡大する標準単射* $M^* \to \Lambda(M)^{*gr}$.‡ これら準同型

† これはno. 1の式(5)、(9)からも導かれます。
‡ この単射は、計算の便宜上、準同型から $\Lambda(M)^{*gr}$ ではなく、準同型から反対多元環から $\Lambda(M)^{*gr}$ に拡張されます。

関数的です: たとえば、すべての $A$ モジュール準同型 $u : M \to N$、図式に対して

$$
\begin{array}{ccc}
T(N^*) & \xrightarrow{T(tu)} & T(M^*) \\
\theta_T \downarrow & & \theta_T \downarrow \\
T(N)^{*gr} & \xrightarrow{t_{T(n)}} & T(M)^{*gr}
\end{array}
$$

は可換であり、テンソル代数 (§ 5, no. 1) の普遍性からすぐに続きます。 $\theta_S$ と $\theta_\wedge$ に対して同様の可換図式があります。

準同型 $\theta_T, \theta_S$ と $\theta_\wedge$ を明示的に見つけます。このために、より一般的に、余積 $c$ と定義するを $n$ の帰納法で、$E$ の $n \geq 2$、線形写像 $c_n$ を求める共結合$A$-cogebra $E$ を考慮します。 $E^{\otimes n}$ by $c_2 = c$ そして
$$
c_n = (c_{n-1} \otimes 1_E) \circ c.
$$
一方、$m_n(\xi_1 \otimes \xi_2 \otimes \cdots \otimes \xi_n) = \xi_1 \xi_2 \cdots \xi_n$ のような正規の線形写像を $m_n : A^{\otimes n} \to A$ で表し、$n \geq 2$ については、
$$
m_n = m \circ (m_{n-1} \otimes 1_A)
$$
$m = m_2$を書いています。これで記法:

#### 補題 1 {#alg-iii-s11-lem-1 .statement tag=0681}

(i) *連想代数 $E^* = \mathrm{Hom}_A(E, A)$, $n$ 元 $u_1, u_2, \ldots, u_n$ 次数 1 の積は次の式で与えられます*
$$
u_1 u_2 \ldots u_n = m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ c_n.
$$
(ii) *余代数 $E$ が採点されていると仮定します。 次に、段階的結合代数 $E^{*gr} = \mathrm{Homgr}_A(E, A)$、$n$ 元 $u_1, u_2, \ldots, u_n$ 次数 1 の積は、* によって与えられます。
$$
u_1 u_2 \ldots u_n = m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ \delta_n
$$
*ここで、$\delta_n : E \to E^{\otimes n}$は、多度$(1, 1, \ldots, 1)$の$c_n(x)$のそれぞれ$x \in E$から成分の写像である線形写像です。*

公式 (26) は、$n = 2$ の $E^*$ の積の定義です。 $n$の帰納法までにそれを証明するには、次のことを観察してください。
$$
u_1 u_2 \ldots u_n
$$
$$
= m \circ ((u_1 u_2 \ldots u_{n-1}) \otimes u_n) \circ c
$$
$$
= m \circ ((m_{n-1} \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_{n-1}) \circ c_{n-1}) \otimes u_n) \circ c
$$
$$
= m \circ (m_{n-1} \otimes 1_A) \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_{n-1} \otimes u_n) \circ (c_{n-1} \otimes 1_E) \circ c
$$
$$
= m_n \circ (u_1 \otimes u_2 \otimes \cdots \otimes u_n) \circ c_n
$$
(24)、(25)、II, § 3, no. 3、公式 (5)、関係により
$$
u_n = 1_A \circ u_n \circ 1_{E^*}.
$$

E が等級付けされ、次数 1 の同種の元 $u_i \in E^{*gr}$ の場合、*同種* の定義元 $x_i \in E$、

$$
(u_1 \otimes u_2 \otimes \cdots \otimes u_n)(x_1 \otimes x_2 \otimes \cdots \otimes x_n) = 0
$$

〜でない限りすべての $x_i$ は次数 1、よって公式 (27) です。

no. 1 と公式の式 (3)、(5)、(7) (24) から、E を 3 つの等級付けされた余代数 $\mathbf{T}(M)$、$\mathbf{S}(M)$、$\mathbf{\Lambda}(M)$ の 1 つとすると、$n$ で帰納法によってそれぞれ得られます (次の事実を使用)。 余積は、M の $x_1, x_2, \ldots, x_n$ に対して、次数 0) のグレード準同型です。

$E = \mathbf{T}(M)$のとき、
$$
\delta_n(x_1 x_2 \cdots x_n) = x_1 \otimes x_2 \otimes \cdots \otimes x_n
$$

$E = \mathbf{S}(M)$のとき、
$$
\delta_n(x_1 x_2 \cdots x_n) = \sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \otimes x_{\sigma(2)} \otimes \cdots \otimes x_{\sigma(n)}
$$

$E = \mathbf{\Lambda}(M)$のとき、
$$
\delta_n(x_1 x_2 \cdots x_n) = \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma \cdot x_{\sigma(1)} \otimes x_{\sigma(2)} \otimes \cdots \otimes x_{\sigma(n)}.
$$

たとえば、$E = \mathbf{\Lambda}(M)$ の場合、式内の次のことに注意するだけで十分です。
$$
c_n(x_1 x_2 \cdots x_n) = (c_{n-1} \otimes 1_E) \left( \sum (-1)^v (x_{i_1} \ldots x_{i_p}) \otimes (x_{j_1} \ldots x_{j_{n-p}}) \right)
$$
no. 1 の公式 (8) から生じ、多次数 $(1, 1, \ldots, 1)$ の項を与えることができる唯一の項は、$n - p = 1$ であるため、
$$
\delta_n(x_1 x_2 \cdots x_n)
$$
和の多度$(1, 1, \ldots, 1)$の項です
$$
\sum_{i=1}^n (-1)^{n-i} c_{n-1}(x_1 \ldots x_{i-1} x_{i+1} \ldots x_n) \otimes x_i
$$
そして、この項は必ず次と等しくなります。
$$
\sum_{i=1}^n (-1)^{n-i} \delta_{n-1}(x_1 \ldots x_{i-1} x_{i+1} \ldots x_n) \otimes x_i,
$$
よって帰納法の仮定による結果。

$n$ の $\mathbf{T}(M)^{*gr}$ 線型形式 $M^*$ の $x_1^*, x_2^*, \ldots, x_n^*$ に補題 1、積を使用すると、次のようになります。

$$
\langle x_1^* x_2^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \prod_{i=1}^n \langle x_i^*, x_i \rangle
$$
$x_i \in M$ ($1 \leq i \leq n$) の場合。これら $n$ のうち積 $\mathbf{S}(M)^{*gr}$ の形は次のように与えられます。

$$
\langle x_1^* x_2^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \sum_{\sigma \in \mathfrak{S}_n} \left( \prod_{i=1}^n \langle x_{\sigma(i)}^*, x_i \rangle \right);
$$

最後に、$\bigwedge(M)^{*gr}$ のこれら形のうち積は次のように与えられます。
$$
\langle x_1^* x_1^* \ldots x_n^*, x_1 x_2 \ldots x_n \rangle = \det(\langle x_i^*, x_j \rangle).
$$
3 つのケースのそれぞれで、
$$
\theta_T(x_1^* \otimes x_2^* \otimes \ldots \otimes x_n^*) = x_1^* x_2^* \ldots x_n^*
$$
$$
\theta_S(x_1^* x_2^* \ldots x_n^*) = x_1^* x_2^* \ldots x_n^*
$$
$$
\theta_\Lambda(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*) = x_n^* x_{n-1}^* \ldots x_1^* = (-1)^{n(n-1)/2} x_1^* x_2^* \ldots x_n^*
$$
したがって、(28)、(29)、(30) から推論します関係
$$(28\ \mathrm{bis})\quad \langle \theta_T(x_1^* \otimes x_2^* \otimes \cdots \otimes x_n^*), x_1 \otimes x_2 \otimes \cdots \otimes x_n \rangle = \prod_{i=1}^n \langle x_i^*, x_i \rangle$$
(他の語 $\theta_T$ は $T^2(M^*)$ に制限されており、II, § 4, no. 4 の標準準同型にすぎません)
$$(29\ \mathrm{bis})\quad \langle \theta_S(x_1^* x_2^* \ldots x_n^*), x_1 x_2 \ldots x_n \rangle = \sum_{\sigma \in S_n} \left( \prod_{i=1}^n \langle x_{\sigma(i)}^*, x_i \rangle \right)$$
$$(30\ \mathrm{bis})\quad \langle \theta_\Lambda(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*), x_1 \wedge x_2 \wedge \cdots \wedge x_n \rangle$$
$$
= (-1)^{n(n-1)/2} \det(\langle x_i^*, x_j \rangle).
$$

#### 命題 7 {#alg-iii-s11-prop-7 .statement tag=0682}

*M を有限生成射影 A-加群とする。すると、標準準同型 $\theta_T : T(M^*) \to T(M)^{*gr}$ と $\theta_\Lambda : \bigwedge(M^*) \to (\bigwedge(M)^{*gr})^0$ は全単射です。また、等級付けされた双対 $\bigwedge(M)^{*gr}$ は、A-加群 $\bigwedge(M)$ の双対 $\bigwedge(M)^*$ と等しくなります。*

まず、M が *有限基底* $(e_i)_{1 \leq i \leq m}$ を持ち、$(e_i^*)_{1 \leq i \leq m}$ を $M^*$ (II, § 10, no. 4) の双対基底とします。 公式 (28 ビス) は、n の有限列 $s = (j_k)_{1 \leq k \leq n}$ 元の区間 $[1, m]$ の $\mathbf{N}$ ごとに、
$$
\theta_T(e_{j_1}^* \otimes \cdots \otimes e_{j_n}^*)
$$
は、$(T^n(M))^*$の基底の添字の元、$e_s = e_{j_1} \otimes \cdots \otimes e_{j_n}$の$T^n(M)$のからなる（§ 5, no. 5、定理1）の基底への*デュアル*です。したがって、$\theta_T$ は全単射です。

同様に、公式 (30 ビス) は、n が元の $[1, m]$ の有限部分集合 H ごとに、$(-1)^{n(n-1)/2} \theta_\Lambda(e_H^*)$ (§ 7, no. 8 の記法、定理 1) が、元であることを示します。 $(\bigwedge^n(M))^*$の基底の添字H、$\bigwedge^n(M)$の基底と$e_H$のからなるの*デュアル*。したがって、$\theta_\Lambda$ は全単射です。

ここで、M が有限に生成され、射影されるとだけ仮定します。この場合、M は有限生成された自由A-加群 L の直因子であるため、次の 2 つが存在します。

A-線型写像 $M \xrightarrow{j} L \xrightarrow{p} M$ の合成は $l_M$ です。可換性図式を導き出します

$$
\begin{array}{ccc}
T(M^*) & \xrightarrow{T(tj)} & T(L^*) \\
\theta_T \downarrow & & \theta_T \downarrow \\
T(M)^{*gr} & \xrightarrow{tT(j)} & T(L)^{*gr}
\end{array}
$$
$$
\begin{array}{ccc}
T(L^*) & \xrightarrow{T(tp)} & T(M^*) \\
\theta_T \downarrow & & \theta_T \downarrow \\
T(L)^{*gr} & \xrightarrow{tT(p)} & T(M)^{*gr}
\end{array}
$$

同様の可換図式では、$T$ が $\Lambda$ に置き換えられます。 命題は次の補題から続きます。

#### 補題 2 {#alg-iii-s11-lem-2 .statement tag=0683}

*しましょう*

$$
\begin{array}{ccccc}
X & \xrightarrow{u} & Y & \xrightarrow{v} & X \\
f \downarrow & & g \downarrow & & f \downarrow \\
X' & \xrightarrow{u'} & Y' & \xrightarrow{v'} & X'
\end{array}
$$

*$v \circ u$ と $v' \circ u'$ がそれぞれ $X$ と $X'$ の恒等写像となるような、集合と写像の可換図式であること。次に、$g$ が単射語 (それぞれ全単射、それぞれ全単射) であれば、$f$ も同様です。*

$v \circ u$ が単射であるため、$u$ は単射です。したがって、$g$ が単射である場合、$u' \circ f = g \circ u$ は単射であり、したがって $f$ は単射です。同様に、$v' \circ u'$ は全射であるため、$v'$ は全射です。したがって、$g$ が全射である場合、$f \circ v = v' \circ g$ は全射であり、したがって $f$ は全射です。

命題 7 の最後の主張は、$\Lambda(M)$ が有限生成A-加群 (§ 7, no. 3、命題 6 および II, § 11, no. 6、注意) であるという事実から導き出されます。

ここで、$M$ が *射影的かつ有限生成* である場合、 準同型 $\theta_S$ に関して何が言えるかを検討します。まず、$M$ が有限の基底 $(e_i)_{1 \leq i \leq m}$ を許容すると仮定します。 記法では、章A-加群$S^n(M)$は、$|\alpha| = n$のような元$e^\alpha$の家族を基底として認めています。 $u_\alpha$ ($|\alpha| = n$ の場合) は、$(S^n(M))^*$ から $(e^\alpha)$ への *双対* の基底における添字の $\alpha$ の元を表すものとします。 元 $u_\alpha$ は、$\alpha \in \mathbf{N}^m$ に対して、代数 $S(M)^{*gr}$ の形基底となり、この基底の乗法表が明示的に得られます。私たちは書きます

$$
u_\alpha u_\beta = \sum_{\gamma \in \mathbf{N}^m} a_{\alpha \beta \gamma} u_\gamma \quad \text{with } a_{\alpha \beta \gamma} \in A.
$$

その後、定義までに

$$
a_{\alpha \beta \gamma} = \langle u_\alpha u_\beta, e^\gamma \rangle = m((u_\alpha \otimes u_\beta)(c(e^\gamma))),
$$

ここで、$A$ と $c$ の $m : A \otimes A \to A$ 定義する乗法は、$S(M)$ の余積です。他の語では、$e^\xi \otimes e^\eta$のからなるの$S(M) \otimes S(M)$の基底の項に$c(e^\gamma)$が書かれているとき、$a_{\alpha \beta \gamma}$は$e^\alpha \otimes e^\beta$の係数であり、$\xi$と$\eta$は$\mathbf{N}^m$まで走ります。しかし、$c$は代数準同型なので、

$$
c(e^\gamma) = \prod_{i=1}^m (c(e_i))^{r_i} = \prod_{i=1}^m (e_i \otimes 1 + 1 \otimes e_i)^{r_i}
$$

公式 (4) 作 no. 1;これは与えます

(31)
$$
c(e^\gamma) = \sum_{\xi + \eta = \gamma} (\xi, \eta) e^\xi \otimes e^\eta
$$
私たちが書く場所

(32)
$$
((\xi, \eta)) = \prod_{i=1}^n \frac{(\xi_i + \eta_i)!}{\xi_i! \eta_i!} \quad \text{(cf. § 10, no. 4, formula (18))}.
$$
したがって、乗法表が得られます。

(33)
$$
u_\alpha u_\beta = ((\alpha, \beta)) u_{\alpha + \beta}.
$$
一方、$(e_i^*)_{1 \leq i \leq m}$ が $M^*$ の基底で、$(e_i)$ と双対である場合、公式 (29 ビス) から、すべての $\alpha \in \mathbf{N}^m$ について、

(34)
$$
\theta_S(e^{*\alpha}) = \alpha! u_\alpha
$$
§ 6, no. 6の記法に。したがって、準同型 $\theta_S$ は、$\alpha! u_\alpha$ 形が $S(M)^{*gr}$ の *基底* である場合、または元 $\alpha! 1$ が *可逆* である場合に限り、全単射となります。

#### 命題 8 {#alg-iii-s11-prop-8 .statement tag=0684}

*環 $A$ が有理数数の体 $\mathbf{Q}$ を超える代数であるとします。次に、有限に生成された射影 $A$ モジュールごとに $M$、準同型*

$$
\theta_S : S(M^*) \to S(M)^{*gr}
$$
*は全単射です*

$M$ が有限に生成され、自由である場合、これは証明になります。ここから、命題 7 の証明のように補題 2 を使用する一般的なケースに移ります。

#### 注意 {#alg-iii-s11-n5-rem-1 .statement tag=0685}

Let $M$ be an $A$-module and $\rho : A \to B$ a commutative ring homomorphism. 次に、次数付き $B$-代数準同型性の可換図式が存在します。

$$
\begin{array}{ccc}
T((M^*)_{(B)}) & \longrightarrow & (T(M)^{*gr})_{(B)} \\
\downarrow_{T(u_M)} & & \downarrow^{u_{T(M)}} \\
T((M_{(B)})^*) & \xrightarrow{\theta_T} & T(M_{(B)})^{*gr}
\end{array}
$$

ここで、最初の行は準同型で、準同型 $\theta_T \otimes 1_B : T(M^*) \otimes_A B \to T(M)^{*gr}$ と標準同型で構成されます。

$$
T((M^*)_{(B)}) \to T(M^*) \otimes_A B
$$

§ 5, no. 3、命題 5)。 準同型 $v_E$ (II, § 5, no. 4) の公式 (28) と定義を使用すると、この図式が *可換*であることがすぐに検証されます。 M が *有限生成射影* A-加群であるとき、 $M_{(B)}$ は有限生成射影 B-加群 (II, § 5, no. 1、系 ～ 命題 4) であり、上記図式のすべての準同型は *全単射 * (命題) です。 7とII, § 5, no. 4、命題8）。 T を S または $\Lambda$ に置き換えた同様の可換図式があります。 M が射影で有限生成される場合 (命題 7)、$\Lambda$ の図式も全単射準同型で構成されます。さらに A が $\mathbf{Q}$ よりも代数である場合、S の図式も全単射準同型 (命題 8) で構成されます。

### 6. 内部積: 代数の場合

$E = \bigoplus_{p \geq 0} E_p$ を型 $\mathbf{N}$ の *グレード A-代数* とし、P を型 $\mathbf{Z}$ の A-加群とグレードします。すべての*同次* 元 $x \in E_p$ に対して、x による *左* 乗法は、それ自体に E の A-線型写像 $e(x)$ が含まれ、*グレードは次数 p* になります。すべての元 $u \in \mathrm{Homgr}_A(E, P)$ について、$u \perp x$ で示される x* による u の *右内部積は、$\mathrm{Homgr}_A(E, P)$ の元 $u \circ e(x)$ です。また、$(i(x))(u) = u \perp x$ と書くと、$i(x)$ は、等級付けされた A-加群 $\mathrm{Homgr}_A(E, P)$ の次数 p の等級付けされた自己準同型であることがわかります。ここで、$x = \sum_{p \geq 0} x_p$ が E の任意の元である場合 ($p$ の値の有限の数を除き、すべての $p \geq 0$、$x_p = 0$ に対して $x_p \in E_p$ が付きます)、$i(x) = \sum_{p=0}^\infty i(x_p)$ と書きます。 A-加群 $\mathrm{Homgr}_A(E, P)$の自己準同型。

式 $u \perp x$ のどちらの元が他方に「作用」するかを思い出すには、u に「作用」する元 x が $\perp$ の水平線の自由端に配置されていることを観察します。

代数 E の *結合性* は、$x, y$ が均一であれば関係 $e(xy) = e(x) \circ e(y)$ に移ります。 よって、$i(x)$の定義によって、

$$
i(xy) = i(y) \circ i(x)
$$

最初は同次の $x, y$ に対して、次に線形性により E の *任意* $x, y$ に対して。これも書かれるかもしれない

$$
(u \perp x) \perp y = u \perp (xy)
$$

for $x, y$ in E and $u \in \mathrm{Homgr}_A(E, P)$; as on the other hand clearly $i(1)$ is the identity mapping (since this follows from $e(1) = 1_E$) and $x \mapsto i(x)$ is *A-linear*, it is seen that the external law of composition $(x, u) \mapsto u \perp x$ ($x \in E, u \in \mathrm{Homgr}_A(E, P)$) defines, with addition, a *right E-module* structure on $\mathrm{Homgr}_A(E, P)$.

特に、$P = A$、$\mathrm{Homgr}_A(E, P)$ が、この場合、$E$ の *段階的双対* $E^{*gr}$ であると考えます。 $i(x)$ は、$E$、$u \in E^{*gr}$ のすべての $x, y$ に対して、$A$ 線形写像 $e(x)$ (II, § 11, no. 6)、他の語の *等級付けされた転置* になります。

$$
\langle u \sqcup x, y \rangle = \langle u, xy \rangle.
$$

段落の冒頭の規則に従って、$x \in E_p$ の場合、$i(x)$ は $E^{*gr}$ *of 次数* $-p$ の自己準同型であることに注意してください。

すべての同次元 $x \in E_p$ について、$x$ による *右* 乗法は、$\mathrm{Homgr}_A(E, P)$ の $e'(x)$ と元 $u \circ e'(x)$ によって同様に表され、u の *左内部積と呼ばれますx* による、$x \sqcup u$ による。 $i'(x) = x \sqcup u$ と書くと、$i'(x)$ は、次数 $p$ の $\mathrm{Homgr}_A(E, P)$ の自己準同型となります。上記のように、この定義は、$x$ が $E$ の任意の元である場合に拡張できます。この $e'(xy) = e'(y)e'(x)$ の場合のように、

$$
i'(xy) = i'(x) \circ i'(y)
$$

これも書かれているかもしれません

$$
x \sqcup (y \sqcup u) = (xy) \sqcup u
$$

そして、合成 $(x, u) \mapsto x \sqcup u$ 定義するの外部法則が、加法、$\mathrm{Homgr}_A(E, P)$ 上の *左 E モジュール* 構造であることを示しています。一方、$E$ の結合性は、$E$、よって関係において$x, y$ に対する$e(x) \circ e'(y) = e'(y) \circ e(x)$ が同次であることを意味します。

$$
(y \sqcup u) \sqcup x = y \sqcup (u \sqcup x)
$$

つまり、$\mathrm{Homgr}_A(E, P)$ 定義するの合成の 2 つの外部法則と、この集合は *(E, E)*-*両側加群* 構造 (II, § 1, no. 14) になります。

$P = A$ を取ると、$i'(x)$ は $e'(x)$ の転置となります。その他の語、すべての $x, y$ の $E$、$u \in E^{*gr}$、

$$
\langle y, x \sqcup u \rangle = \langle yx, u \rangle.
$$

等級付けされた代数 $E$ が *可換* である場合、明らかに $u \sqcup x = x \sqcup u$ です。 $E$ が *反可換* で、$P = A$ の場合、$x \in E_p$、$y \in E_r$、$u \in E_q^*$、$yx = (-1)^{pr} xy$、よってについては、(37) と (41) により、$\langle u \sqcup x, y \rangle = (-1)^{pr} \langle y, x \sqcup u \rangle$ となります。しかし、この関係の両辺は$r = q - p$を除いて零なので、

$$
x \sqcup u = (-1)^{p(q-p)} u \sqcup x.
$$

$F$ を他の等級付けされた $A$-代数、および $\phi : E \to F$ を等級付けされた代数の $A$-準同型写像とします。この場合、$\tilde{\phi} = \mathrm{Hom}(\phi, 1_P) : \mathrm{Homgr}_A(F, P) \to \mathrm{Homgr}_A(E, P)$ は次数 0 の段階的$A$-準同型写像です。 定義により、$E$ と $u \in \mathrm{Homgr}_A(F, P)$ の $x, y$ に

$$
\begin{align*}
(\tilde{\phi}(u \sqcup \phi(x)))(y) &= (u \sqcup \phi(x))(\phi(y)) \\
&= u(\phi(x)\phi(y)) = u(\phi(xy)) = (\tilde{\phi}(u))(xy) = (\tilde{\phi}(u) \sqcup x)(y)
\end{align*}
$$

またはまた

$$
\tilde{\phi}(u \sqcup \phi(x)) = \tilde{\phi}(u) \sqcup x
$$

そして同様に

$$
\tilde{\phi}(\phi(x) \sqcup u) = x \sqcup \tilde{\phi}(u).
$$

他の語では、Homgr_A(F, P) が環準同型 $\phi : E \to F$ によって (E, E) 双加群とみなされると、$\tilde{\phi}$ は (E, E) 双加群準同型 (または (F, の E 準同型) であることがわかります。 F)-双モジュール Homgr_A(F, P) を (E, E)-双モジュール Homgr_A(E, P)) に変換します。

#### 例 {#alg-iii-s11-n6-exa-1 .statement tag=0686}

特に、上記は、E が A-加群 M および P A-加群 (自明な目盛り付き) の等級付けされた代数 T(M)、S(M) または $\bigwedge(M)$ のいずれかである場合に適用できます。このようにして得られた両側加群構造を明示的に見つけるには、Homgr_A(T(M), P) (それぞれ Homgr_A(S(M), P)、それぞれ Homgr_A($\bigwedge(M)$, P)) の次数 $-n$ の元が *n 線形写像* (それぞれ *対称) で識別されることに注意してください。 $M^n$ の n 線形写像*、それぞれ *交代的 n 線形写像*) を P に変換します。 積を表すだけで十分です。

$$
f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p)
$$

(それぞれ $f \sqcup (x_1 x_2 \ldots x_p)$)、それぞれ$f \sqcup (x_1 \wedge x_2 \wedge \cdots \wedge x_p)$) M の元の各有限列 $(x_i)_{1 \leq i \leq p}$ と、左の内部積の類似物。 定義からすぐに次のことが続きます。

$$
f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = (x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f = 0
$$

*もし* $p > n$ の場合、$p \leq n$、$f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p)$ (それぞれ

$$
(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f)
$$

は、次のように定義される *(n - p)* 線形マッピングです。

$$
\begin{cases}
(f \sqcup (x_1 \otimes x_2 \otimes \cdots \otimes x_p))(y_1, \ldots, y_{n-p}) \\
\hspace{10cm} = f(x_1, \ldots, x_p, y_1, \ldots, y_{n-p}) \\
((x_1 \otimes x_2 \otimes \cdots \otimes x_p) \sqcup f)(y_1, \ldots, y_{n-p}) \\
\hspace{10cm} = f(y_1, \ldots, y_{n-p}, x_1, \ldots, x_p).
\end{cases}
$$

$p > n$ については、Homgr_A(S(M), P) (それぞれ Homgr_A($\bigwedge(M)$, P)) の式 (44) にもあり、$x_1 \otimes x_2 \otimes \cdots \otimes x_p$ は $x_1 x_2 \ldots x_p$ (それぞれ $x_1 \wedge x_2 \wedge \cdots \wedge x_p$) に置き換えられます。 $p \leq n$ の場合、(45) 定義する *対称* *(n - p)*-線形写像 $f \sqcup (x_1 x_2 \ldots x_p)$ および $(x_1 x_2 \ldots x_p) \sqcup f$ (それぞれ *交代的* *(n - p)*-線形写像

$$
f \sqcup (x_1 \wedge x_2 \wedge \cdots \wedge x_p) \quad \text{and} \quad (x_1 \wedge x_2 \wedge \cdots \wedge x_p) \sqcup f).
$$

$n = p$ のとき、上記の積は、$M$ が $f(x_1, \ldots, x_p)$ に等しい定数写像に等しくなります。

$u : M \to N$ が $A$ 加群準同型であり、$T(u) : T(M) \to T(N)$ が段階的 $A$ 代数準同型写像である場合、上で見たことから、$(T(u))^\sim$ は $(T(N), T(N))$ 双加群の $T(M)$ 準同型写像であるということになります。 $\mathrm{Homgr}_A(T(N), P)$ を、環準同型 $T(u)$ を基準にして、$(T(M), T(M))$-bimodule $\mathrm{Homgr}_A(T(M), P)$ に変換します。 $(S(u))^\sim$ と $(\wedge(u))^\sim$ にも同様の結果があります。

### 7. 内部積: 余代数のケース

$E = \bigoplus_{p \geq 0} E_p$ を余代数に等級付けされた共結合共同体とします。次に、等級付き双対 $E^{*\mathrm{gr}}$ が (段落の冒頭で作成された等級に関する規則に従って) 2 のうち $A$、積よりも型 $\mathbf{N}$ のうち等級付けされた代数構造があることがわかります (no. 2、命題 1 および 3)。この代数の元 $u, v$ は $uv = m \circ (u \otimes v) \circ c$ によって定義されます。ここで、$c : E \to E \otimes_A E$ は余積と $m : A \otimes_A A \to A$ 定義する乗法です。他の語では、$x \in E$、$c(x) = \sum_i y_i \otimes z_i$ について、次のように書くことができます ($A \otimes_A E$ と $E$ を正規に識別します)。

$$
\langle x, uv \rangle = (uv)(x) = \sum_i u(y_i)v(z_i) = v\left( \sum_i u(y_i)z_i \right)
= v(((u \otimes 1_E) \circ c)(x)) = \langle ((u \otimes 1_E) \circ c)(x), v \rangle.
$$

これは、$E^{*\mathrm{gr}}$ の次数 $p$ の同種のすべての $u$ について、$E^{*\mathrm{gr}}$ の左側の乗法 $e(u) : v \mapsto uv$ が、等級付けされた自己準同型の等級付けされた転置であると、というによって解釈できます。 次数 $-p$

$$(46)$$
$$
i(u) = (u \otimes 1_E) \circ c
$$
$E$の;したがって、上記の記法では、

$$
(i(u))(x) = \sum_i u(y_i)z_i.
$$

公式 (46) も元 $u \in E^{*\mathrm{gr}}$ ごとに定義する元 $i(u) \in \mathrm{Endgr}_A(E)$ になります。すべての $x \in E$ とすべての $u \in E^{*\mathrm{gr}}$ について、私たちは書きます

$$(47)$$
$$
x \perp u = (i(u))(x)
$$
したがって、$E^{*\mathrm{gr}}$ の $u$ と $v$ については、

$$
\langle x, uv \rangle = \langle x \perp u, v \rangle.
$$

$E$の元$x \perp u$は、$u$によって$x$の右内部積と呼ばれます。

ここでも、$x$ で「動作」する元 $u$ が、$\underline{\phantom{x}}$ の水平線の自由端に配置されます。

$E^{*\mathrm{gr}}$ のいずれか 2 つの元 $u, v$ について、

$$
x \underline{\phantom{(uv)}} = (x \underline{\phantom{u}}) \underline{\phantom{v}},
$$

その他語

$$
i(uv) = i(v) \circ i(u).
$$

上記のように $c(x) = \sum_i y_i \otimes z_i$ とすると、 $x \underline{\phantom{(uv)}} = \sum_i (uv)(y_i)z_i$ になります。もし

$$
c(y_i) = \sum_j y_{ij}' \otimes y_{ij}'',
$$

それから

$$
x \underline{\phantom{(uv)}} = \sum_{i,j} u(y_{ij}')v(y_{ij}'')z_i.
$$

一方、$c(z_i) = \sum_k z_{ik}' \otimes z_{ik}''$ の場合、

$$
(x \underline{\phantom{u}}) \underline{\phantom{v}} = \sum_{i,k} u(y_i)v(z_{ik}')z_{ik}''.
$$

ここで、$E$ の共結合性は、(no. 2, 命題 1) を示します。

$$
\sum_{i,j} y_{ij}' \otimes y_{ij}'' \otimes z_i = \sum_{i,k} y_i \otimes z_{ik}' \otimes z_{ik}''
$$

式 (49) と (50) の等式は、それぞれ、線形写像 $f$ の下で、$E \otimes E \otimes E$ から $E$ の下で、$f(x \otimes y \otimes z) = u(x)v(y)z$ となる (51) の左辺と右辺の像であるという事実から導き出されます。

一方 (no. 2, 命題 3) 代数 $E^{*\mathrm{gr}}$ の単位元は線型形式 $e : x \mapsto \gamma(x).1$ であることを思い出します。したがって

$$
x \underline{\phantom{e}} = \sum_i \gamma(y_i)z_i = x
$$

余単位の定義のおかげで。 写像 $u \mapsto i(u)$ は線形であるため、合成 $(u, x) \mapsto x \underline{\phantom{u}}$ 定義するの外部法則は、$E$ 上の *正しい* $E^{*\mathrm{gr}}$ 加群構造であることがわかります。

同様に、$E$ のすべての $u \in E^{*\mathrm{gr}}$、自己準同型に対して、定義する

$$
i'(u) = (1_E \otimes u) \circ c
$$

そして、すべての$x \in E$のために、私たちは書きます

$$
(i'(u))(x) = u \underline{\phantom{x}}
$$

そして、この $E$ の元は、u* による x の *左内部積と呼ばれます。上のように、外部法則 $(u, v) \mapsto u \sqcup x$ 定義するが $E$ 上の *左 $E^{*\mathrm{gr}}$ モジュール構造* であることがわかります。さらに、これら 2 つの構造は *互換性* があり、他の語では、

$$(54)$$
$$(u \sqcup x) \sqcap v = u \sqcup (x \sqcap v)$$

$E^{*\mathrm{gr}}$ (II, § 1, no. 14) の $u, v$ について。上と同じ記法の場合、(54)の左辺は$\sum_{i,j} u(z_i)v(y_{ij}')y_{ij}''$、右辺は$\sum_{i,k} v(y_i)u(z_{ik}'')z_{ik}'$になります。それらの等式は、$E \otimes E \otimes E$ の線形写像 $g$ を $E$ に置き換えた (51) の左辺と右辺のそれぞれ像であるという事実から、$g(x \otimes y \otimes z) = v(x)u(z)y$ になります。

It is therefore seen that the two external laws of composition on $E$ defines on this set an $(E^{*\mathrm{gr}}, E^{*\mathrm{gr}})$*-bimodule* structure.

余代数 $E$ が *共可換* の場合、すべての $x \in E$ と $u \in E^{*\mathrm{gr}}$ に対して $u \sqcup x = x \sqcap u$ になります。 *反共換* (§ 4, no. 9) と $u \in E_p^*$ と $x \in E_q$ の場合、すべての $j$ に対して $E_j$ で $y_{ij}$ と $z_{ij}$ を含む $c(x) = \sum_{0 \leq j \leq q} \left( \sum_i y_{ij} \otimes z_{i, q-j} \right)$ を書くことができ、その後仮定までに

$$\sum_i z_{ij} \otimes y_{i, q-j} = (-1)^{j(q-j)} \sum_i y_{ij} \otimes z_{i, q-j}.$$

定義、$x \sqcap u = \sum_{0 \leq j \leq q} \left( \sum_i u(y_{ij})z_{i, q-j} \right)$、および

$$u \sqcup x = \sum_{0 \leq j \leq q} \left( \sum_i u(z_{i, q-j})y_{ij} \right).$$

$u(y_{ij}) = 0$ (それぞれ $u(z_{i, q-j}) = 0$ 〜でない限り $j = p$ (それぞれ $q - j = p$) として、上記から $u \sqcup x = (-1)^{p(q-p)} x \sqcap u$ であることがわかります。

最後に、$\phi : E \to F$ を *等級付けされた余代数射* とします。次に、等級付けされた転置 $t\phi : F^{*\mathrm{gr}} \to E^{*\mathrm{gr}}$ が *等級付けされた代数準同型* であることがわかりました (no. 2)。したがって、$F^{*\mathrm{gr}}$ の $x \in E$、$u, v$ については、

$$
\langle \phi(x \sqcap t\phi(u)), v \rangle = \langle x \sqcap t\phi(u), t\phi(v) \rangle = \langle x, t\phi(u)t\phi(v) \rangle = \langle x, t\phi(uv) \rangle
$$
$$
= \langle \phi(x), uv \rangle = \langle \phi(x) \sqcap u, v \rangle
$$

よって

$$(55)$$
$$\phi(x) \sqcap u = \phi(x \sqcap t\phi(u));$$

そして同様に

$$(56)$$
$$u \sqcup \phi(x) = \phi(t\phi(u) \sqcup x).$$

他の語では、$\phi$ は、環準同型に対する $(E^{*\mathrm{gr}}, E^{*\mathrm{gr}})$*-bimodule* $E$ の $(F^{*\mathrm{gr}}, F^{*\mathrm{gr}})$*-bimodule* $F$ への $F^{*\mathrm{gr}}$*-準同型写像* です。

$$
t\phi : F^{*\mathrm{gr}} \to E^{*\mathrm{gr}}.
$$

#### 例 {#alg-iii-s11-n7-exa-1 .statement tag=0687}

特に、上記は、E が余代数 T(M)、S(M)、または A-加群 M (no. 1、例 5、6、7) の $\Lambda(M)$ のいずれかである場合に適用できます。 このようにして得られた両側加群構造を明示的に求めるために、$T(M)^{*gr}$ (それぞれ $S(M)^{*gr}$、それぞれ $\Lambda(M)^{*gr}$) の次数 n の同次元 f を *n 線形形式* (それぞれ *対称 n 線形形式*、それぞれ *交代的) で再度同一視する求めます。 n-linear form*、*n-form* とも呼ばれます) $M^n$。 積と表現すれば十分です

$$
(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \triangleleft f \text{ (resp. } (x_1 x_2 \ldots x_p) \triangleleft f,
$$

それぞれM の元のすべての有限列 $(x_i)_{1 \leq i \leq p}$ と、左側の内部積の類似物に$(x_1 \wedge x_2 \wedge \cdots \wedge x_p) \triangleleft f$。ここで、定義 (46) と (52) と、no. 1 の式 (3)、(6)、(9) はそれぞれ次のようになります。

$$
\begin{cases}
(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \triangleleft f = f \triangleright (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = 0 \\
(x_1 x_2 \ldots x_p) \triangleleft f = f \triangleright (x_1 x_2 \ldots x_p) = 0 \quad \text{for } p < n. \\
(x_1 \wedge x_2 \wedge \cdots \wedge x_p) \triangleleft f = f \triangleright (x_1 \wedge x_2 \wedge \cdots \wedge x_p) = 0
\end{cases}
$$

$p \geq n$ については、それぞれ

(58) $(x_1 \otimes x_2 \otimes \cdots \otimes x_p) \triangleleft f = f(x_1, \ldots, x_n)x_{n+1} \otimes \cdots \otimes x_p$

(59) $(x_1 x_2 \ldots x_p) \triangleleft f = \sum_{\sigma} f(x_{\sigma(1)}, \ldots, x_{\sigma(n)})x_{\sigma(n+1)} \cdots x_{\sigma(p)}$

(60) $(x_1 \wedge x_2 \wedge \cdots \wedge x_p) \triangleleft f = \sum_{\sigma} \varepsilon_{\sigma} f(x_{\sigma(1)}, \ldots, x_{\sigma(n)})x_{\sigma(n+1)} \wedge \cdots \wedge x_{\sigma(p)}$

(ここで、(59) と (60) では、合計は $\mathbf{N}$ の区間* $[1, n]$ と $[n+1, p]$ の *増加するである置換 $\sigma \in \mathfrak{S}_p$ を引き継ぎます。そして同様に

(61) $f \triangleright (x_1 \otimes x_2 \otimes \cdots \otimes x_p) = f(x_{p-n+1}, \ldots, x_p)x_1 \otimes x_2 \otimes \cdots \otimes x_{p-n}$

(62) $f \triangleright (x_1 x_2 \ldots x_p) = \sum_{\sigma} f(x_{\sigma(p-n+1)}, \ldots, x_{\sigma(p)})x_{\sigma(1)} \cdots x_{\sigma(p-n)}$

(63) $f \triangleright (x_1 \wedge x_2 \wedge \cdots \wedge x_p) = \sum_{\sigma} \varepsilon_{\sigma} f(x_{\sigma(p-n+1)}, \ldots, x_{\sigma(p)})x_{\sigma(1)} \wedge \cdots \wedge x_{\sigma(p-n)}$

(ここで、(62) と (63) では、合計は $\mathbf{N}$ の区間* $[1, p-n]$ と $[p-n+1, p]$ の *増加するである置換 $\sigma \in \mathfrak{S}_p$ を引き継ぎます。)

### 8. 内部積: ビゲブラの場合

E を段階的双眼鏡 (それぞれスキュー段階的双眼鏡) (no. 4, 定義 3) とします。次に、nosの結果。 6 と 7 は、すべての $x \in E$ とすべての $u \in E^{*\mathrm{gr}}$ に対して、右 (それぞれ左) 定義する内部積 $x \triangleleft u \in E$ と $u \triangleleft x \in E^{*gr}$ (それぞれ $u \triangleright x \in E$ と $x \triangleright u \in E^{*gr}$) に適用できます。したがって、$E$ では、$(E, E)$-bimodule 構造と $(E^{*\mathrm{gr}}, E^{*\mathrm{gr}})$-bimodule 構造が得られます。さらに遠く：

#### 命題 9 {#alg-iii-s11-prop-9 .statement tag=0688}

*$E$ を段階的双眼鏡 (それぞれスキュー段階双眼鏡) とします。 $E$ の次数 1 の元 $x$ ごとに、$x$ による左右の内部積は、代数の導分 (反導出) ($§ 10$、no. 2) になります。 $E^{*\mathrm{gr}}$.*

no. 6 の記法では、勾配双晶 (または斜勾配双晶) $E$ の *次数* 1 の同次元 $x$ ごとに、
$$
c(x) = x \otimes 1 + 1 \otimes x,
$$
no. 3 の命題 5 と、$c$ が次数 0 の準同型であるという事実によって計算されます。まず、$E$ が等級付き双眼鏡であると仮定します。 $y \in E$ 全員のために、定義により
$$
\langle (uv) \mathbin{\&} x, y \rangle = \langle uv, xy \rangle = m((u \otimes v)(c(xy)))
$$
$c$ は *代数* 準同型なので、$c(xy) = c(x)c(y)$。 $c(y) = \sum_i s_i \otimes t_i$ を $s_i$ と $t_i$ で$E$ にします。したがって
$$
c(xy) = \sum_i (xs_i) \otimes t_i + \sum_i s_i \otimes (xt_i).
$$
したがって$\langle (uv) \mathbin{\&} x, y \rangle = \sum_i u(xs_i)v(t_i) + \sum_i u(s_i)v(xt_i)$です。しかし、私たちは書くかもしれません
$$
\sum_i u(xs_i)v(t_i) = m(((u \mathbin{\&} x) \otimes v)(c(y))) = \langle (u \mathbin{\&} x)v, y \rangle
$$
そして同様に
$$
\sum_i u(s_i)v(xt_i) = m((u \otimes (v \mathbin{\&} x))(c(y))) = \langle u(v \mathbin{\&} x), y \rangle,
$$
よって、記法 $i(x)$ に戻り、内部積。
$$(64)$$
$$(i(x))(uv) = ((i(x))(u))v + u((i(x))(v))$$
これは、$i(x)$ が $E^{*\mathrm{gr}}$ の *導分* であることを証明します。

ここで、$E$ が *skew* 等級付けされた双眼鏡、つまり $u \in E_p^*$、$v \in E_q^*$、および $y \in E_r$ であると仮定します。そうすれば書けます
$$
c(y) = \sum_{0 \leq j \leq r} \left( \sum_i s_{ij} \otimes t_{i,r-j} \right)
$$
ここで、$s_{ij}$ と $t_{ij}$ 属するから $E_j$ です。 $E^g \otimes_A E$ の積の定義までに、その後
$$
c(xy) = c(x)c(y) = \sum_{0 \leq j \leq r} \left( \sum_i (xs_{ij}) \otimes t_{i,r-j} + (-1)^j \sum_i s_{ij} \otimes (xt_{i,r-j}) \right)
$$
今回はよって
$$
\langle (uv) \mathbin{\&} x, y \rangle = \sum_{0 \leq j \leq r} \left( \sum_i u(xs_{ij})v(t_{i,r-j}) + (-1)^j \sum_i u(s_{ij})v(xt_{i,r-j}) \right).
$$

それから$\sum_{0 \leq j \leq r} \left( \sum_i u(x s_{ij}) v(t_{i,r-j}) \right) = \langle (u \sqcup x)v, y \rangle$も。一方、$u(s_{ij}) = 0$ 〜でない限り $j = -p$ したがって、次のように書くこともできます。
$$
\sum_{0 \leq j \leq r} (-1)^j \left( \sum_i u(s_{ij}) v(x t_{i,r-j}) \right) = (-1)^p \langle u(v \sqcup x), y \rangle.
$$
したがって、私たちは結論する
$$
(i(x))(uv) = ((i(x))(u))v + (-1)^p u((i(x))(v)),
$$
他の語 $i(x)$ は $E^{*gr}$ の *反微分* です。 $E$ の次数 1 の元 $x$ による左内部積に関する主張も同様に証明されます。

#### 注意 {#alg-iii-s11-n8-rem-1 .statement tag=0689}

(1) $E$ を 3 つの等級付けされた $A$ 加群 $A$ および $N, N', N''$ 上の等級付き双数とします。 $m$ を $N \times N'$ から $N''$ への $A$ 双線形写像とします。 $u \in \mathrm{Homgr}_A(E, N)$ と $v \in \mathrm{Homgr}_A(E, N')$ について、$u.v$ は、$E$ から $N''$ に等級付けされた準同型 $m \circ (u \otimes v) \circ c$ を表します。一方、$i(x)$ は、$A$ モジュール $\mathrm{Homgr}_A(E, N)$、$\mathrm{Homgr}_A(E, N')$、$\mathrm{Homgr}_A(E, N'')$ の $x \in E$ による (右または左) 内部積を表すものとします。次に、$x$ が *of 次数* 1 である場合、
$$
(i(x))(u.v) = ((i(x))(u)).v + u.((i(x))(v))
$$
$u \in \mathrm{Homgr}_A(E, N)$ と $v \in \mathrm{Homgr}_A(E, N')$ 全員に。

同じ条件の下で、$E$ が傾斜勾配双晶であり、$u$ が次数 $p$ と同次である場合、
$$
(i(x))(u.v) = ((i(x))(u)).v + (-1)^p u.((i(x))(v)).
$$
証明は命題9と同じです。

(2) 上記の証明と同じ議論は、より一般的に、すべての $x \in E$ について、$c(x) = \sum_j x'_j \otimes x''_j$ であれば、$E^{*gr}$ のすべての $u, v$ について、「ライプニッツ公式」であることを証明します。
$$
(i(x))(uv) = \sum_j (i(x'_j))(u).(i(x''_j))(v)
$$
が成立する。特に、等級付き双眼鏡 $E$ のすべての *プリミティブ* 元について、つまり $c(x) = x \otimes 1 + 1 \otimes x$、$i(x)$ は $E^{*gr}$ の *導分* になります。

#### 命題 10 {#alg-iii-s11-prop-10 .statement tag=068A}

*$E$ を段階的双眼鏡 (またはスキュー段階双眼鏡) とします。 $E^{*gr}$ の次数 1 の元 $f$ ごとに、左右の内部積は代数 $E$ の導分 (反導出) です。*

$x \in E_p, y \in E_q$ ($p \geq 1, q \geq 1$) にしましょう。 no. 3 の命題 5 までに、次のように書くことができます
$$
c(x) = x \otimes 1 + \sum_{1 \leq j \leq p-1} \left( \sum_i x'_{ij} \otimes x''_{ij,p-j} \right) + 1 \otimes x
$$
$$
c(y) = y \otimes 1 + \sum_{1 \leq k \leq q-1} \left( \sum_i y'_{i,k} \otimes y''_{i,q-k} \right) + 1 \otimes y
$$

ここで、$x'_{ij}$ と $x''_{ij}$ 属するから $E_j$、 $y'_{ik}$ および $y''_{ik}$ から $E_k$ です。 $E$ が等級付き双眼鏡の場合、$c(xy) = c(x)c(y)$ 所属 ～ $E_1 \otimes E$ の成分は次と等しくなります。
$$
\sum_i x'_{i,1} \otimes x''_{i,p-1}y + \sum_i y'_{i,1} \otimes xy''_{i,q-1}
$$
したがって定義までに
$$
(xy) \leftarrow f = \sum_i f(x'_{i,1})x''_{i,p-1}y + \sum_i f(y'_{i,1})xy''_{i,q-1}
$$
$$
= (x \leftarrow f)y + x(y \leftarrow f)
$$
そして、$f$ による右側の内部積は *導分* です。一方、$E$ が傾斜勾配双眼鏡である場合、$c(xy)$ 所属から $E_1 \otimes E$ の成分は次と等しくなります。
$$
\sum_i x'_{i,1} \otimes x''_{i,p-1}y + (-1)^p \sum_i y'_{i,1} \otimes xy''_{i,q-1}
$$
そして今回は取得します
$$
(xy) \leftarrow f = (x \leftarrow f)y + (-1)^p x(y \leftarrow f)
$$
これは、$i(f)$ が *反派生* であることを示しています。議論は左の内部積 by $f$ についても同様です。

#### 例 {#alg-iii-s11-n8-exa-1 .statement tag=068B}

命題 9 と 10 は、特に段階的双眼鏡 $S(M)$ とスキュー段階的双眼鏡 $\Lambda(M)$ に適用されます。 $S(M)$ (それぞれ $S(M)^{*gr}$) の次数 1 の元による内部積は *導分* です。これは、$S(M)$ (それぞれ $S(M)^{*gr}$) が可換であるため、1 つの他の* と * 交換します。

Similarly, the inner products by elements of degree 1 in $\Lambda(M)$ (resp. $\Lambda(M)^{*gr}$) are *antiderivations*, which are of *zero square*, for the square of an element of degree 1 in the algebra $\Lambda(M)$ (resp. $\Lambda(M)^{*gr}$) is zero.

### 9. 内部積 $T(M)$ と $T(M^*)$、 $S(M)$ と $S(M^*)$、 $\Lambda(M)$ と $\Lambda(M^*)$ の間

$T(M)$ (それぞれ $S(M)$、それぞれ $\Lambda(M)$) 上の右内部積定義する代数 $T(M)^{*gr}$ (それぞれ $S(M)^{*gr}$、それぞれ $\Lambda(M)^{*gr}$) 上の右加群構造 (no. 7、*例*)。 no. 5 の標準準同型 $\theta_T$ (それぞれ $\theta_S$、それぞれ $\theta_\Lambda$) を使用して、次を導き出します。
$T(M)$ の右側の $T(M^*)$ モジュール構造
$S(M)$ の右側の $S(M^*)$ モジュール構造
$\Lambda(M)$ の左側の $\Lambda(M^*)$ モジュール構造。

これら構造のいずれかの外部法則は、次のようにも表されます。
$$
(z^*, t) \mapsto i(z^*) \cdot t
$$

（言葉の乱用による） $T(M)$ または $S(M)$ の場合も、$i(z^*) . t$ の代わりに $t \prec z^*$ と書きます。一方、$\Lambda(M)$の場合は$z^* \prec t$と書き、これは$z^*$による$t$の*左* 内部積であると言います。それ以降、*左* $\Lambda(M^*)$モジュール法則ができます。 $z^*$ の同次の次数 $n$ および $t$ の同次の次数の場合 $p$、$p < n$ の場合は $i(z^*) . t = 0$、そして $x_i \in M$ ($1 \leq i \leq p$) の場合、$x_j^* \in M^*$ ($1 \leq j \leq n$) および $p \geq n$、no. 7 の式 (58)、(59)、および (60) により、

$$
(66)\quad i(x_1^* \otimes x_2^* \otimes \cdots \otimes x_n^*) . (x_1 \otimes x_2 \otimes \cdots \otimes x_p)
$$
$$
= \left( \prod_{j=1}^n \langle x_j^*, x_j \rangle \right) x_{n+1} \otimes \cdots \otimes x_p
$$

$$
(67)\quad i(x_1^* x_2^* \ldots x_n^*) . (x_1 x_2 \ldots x_p) = \sum_\sigma \left( \prod_{j=1}^n \langle x_j^*, x_{\sigma(j)} \rangle \right) x_{\sigma(n+1)} \cdots x_{\sigma(p)}
$$

$$
(68)\quad i(x_1^* \wedge x_2^* \wedge \cdots \wedge x_n^*) . (x_1 \wedge x_2 \wedge \cdots \wedge x_p)
$$
$$
= (-1)^{n(n-1)/2} \sum_\sigma \varepsilon_\sigma \left( \prod_{j=1}^n \langle x_j^*, x_{\sigma(j)} \rangle \right) x_{\sigma(n+1)} \wedge \cdots \wedge x_{\sigma(p)}
$$

ここで、式 (67) と (68) である $\sigma$ は、区間 $\{1, n\}$ と $\{n + 1, p\}$ 上の *増加する* である置換 $\sigma \in \mathfrak{S}_p$ の集合を通過します。

内部積記法で次のように書くこともできます。

$$
\langle t \prec u^*, v^* \rangle = \langle t, \theta_T(u^* v^*) \rangle \quad \text{for } t \in T(M), u^*, v^* \text{ in } T(M^*)
$$
$$
\langle t \prec u^*, v^* \rangle = \langle t, \theta_S(u^* v^*) \rangle \quad \text{for } t \in S(M), u^*, v^* \text{ in } S(M^*)
$$
$$
\langle v^*, u^* \prec t \rangle = \langle \theta_\Lambda(u^* \wedge v^*), t \rangle \text{ for } t \in \Lambda(M), u^*, v^* \text{ in } \Lambda(M^*).
$$

左内部積の類似の式を明示的に見つける作業は読者に任せます。今回は式 (61)、(62)、および (63) を使用します。

上記は、$M$ をその二重の $M^*$ に置き換えて適用できます。たとえば、$M^*$ は、双対の $M^{**}$ と $T(M^*)$ で置き換える必要があり、したがって、代数 $T(M^{**})$ に対して加群構造の権利があります。しかし、標準写像 $c_M : M \to M^{**}$ 定義する代数準同型 $T(c_M) : T(M) \to T(M^{**})$ により、$T(M^*)$ は *権利* $T(M)$-*加群* 構造を持ちます。同様に、$S(M^*)$ (それぞれ $\Lambda(M^*)$) には *右* $S(M)$-*加群* (それぞれ *左* $\Lambda(M)$-*加群*) 構造があります。これら加群の外部法則を与える明示的な公式は、$M$ と $M^*$ の役割を交換することによって上記から直接導出されます。すべての $x \in M$ について、$i(x)$ は常に、等級付けされた代数 $S(M^*)$ (それぞれ $\Lambda(M^*)$) の *導分* (それぞれ *零平方* の逆微分) であることに注意してください。

#### 命題 11 {#alg-iii-s11-prop-11 .statement tag=068C}

*標準準同型* $\theta_T : T(M^*) \to T(M)^{*gr}$ (それぞれ $\theta_S : S(M) \to S(M)^{*gr}$、それぞれ $\theta_\Lambda : \Lambda(M^*) \to \Lambda(M)^{*gr}$) *は右です* $T(M)$-*加群* (それぞれ *右* $S(M)$-*加群*、それぞれ *左* $\Lambda(M)$-*加群*) *準同型.*

まず、$z^* \in T(M^*)$ と $t \in T(M)$ について、

$$
\theta_T(z^* \wedge t) = \theta_T(z^*) \wedge t.
$$

$M$ は代数 $T(M)$ の生成する系であるため、$t = x \in M$ のとき (69) を証明するだけで済みます。さらに、$x_j^* \in M^*$ が$z^* = x_1^* \otimes x_2^* \otimes \cdots \otimes x_p^*$ になり、その後、(66) によって$M$ と$M^*$ の役割が入れ替わって$z^* \wedge x = \langle x, x_1^* \rangle x_2^* \otimes \cdots \otimes x_p^*$ になる場合に注意を限定することができます。したがって、$M$ のすべての $y_2, \ldots, y_p$ について、

$$
\begin{align*}
\langle \theta_T(z^* \wedge x), y_2 \otimes y_3 \otimes \cdots \otimes y_p \rangle &= \langle x, x_1^* \rangle \prod_{j=2}^p \langle y_j, x_j^* \rangle \\
&= \langle \theta_T(z^*), x \otimes y_2 \otimes \cdots \otimes y_p \rangle \\
&= \langle \theta_T(z^*) \wedge x, y_2 \otimes \cdots \otimes y_p \rangle
\end{align*}
$$

よって (69)。

次に、$z^* \in S(M^*)$ と $t \in S(M)$ について、

$$
\theta_S(z^* \wedge t) = \theta_S(z^*) \wedge t.
$$

上記のように、$t = x \in M$ のケースに極限対応できます。しかしさらに、ここでの$i(x)$は$S(M^*)$の導分と$S(M)^{*gr}$の導分です。したがって (§ 10, no. 7、系から命題 9) $M^*$ は $S(M^*)$ の生成する系であるため、$z^* = x^* \in M^*$ について (70) を検証するだけで十分です。しかし、これは自明のことであり、その場合、両辺は $\langle x^*, x \rangle$ に等しくなります。同様の議論により、関係が証明されます。

$$
\theta_\wedge(t \wedge z^*) = t \wedge \theta_\wedge(z^*)
$$

$z^* \in \Lambda(M^*)$ と $t \in \Lambda(M)$ の場合: $x \in M$ の場合、$i(x)$ は $\Lambda(M^*)$ および $\Lambda(M)^{*gr}$ の逆導出であることを観察し、§ 10, no. 7、系から命題を使用します。 9. 左の内部についても同様の結果があります。 積。

### 10. 有限生成された自由加群の場合の、内部積の明示的な形

$M$ を有限生成された自由な $A$ モジュール、$M$ の $(e_i)_{1 \leq i \leq n}$ 基底と $M^*$ の $(e_i^*)_{1 \leq i \leq n}$ 双対基底とします。 $\{1, n\}$ の元のすべての有限列 $s = (i_1, \ldots, i_p)$ について、$e_s = e_{i_1} \otimes e_{i_2} \otimes \cdots \otimes e_{i_p}$ (それぞれ $e_s^* = e_{i_1}^* \otimes \cdots \otimes e_{i_p}^*$) とします。 (§ 5, no. 5、定理 1) は、$A$ モジュール $T(M)$ の $e_s$ 形基底と $A$ モジュールの $e_s^*$ 基底であることがわかっています。 $T(M^*)$。 $s, t$ が $\{1, n\}$ の元の 2 つの有限列である場合、$s.t$ は次のように得られる数列を表します。$s = (i_1, \ldots, i_p)$ と $t = (j_1, \ldots, j_q)$ の場合、$s.t$ は数列 $(i_1, \ldots, i_p, j_1, \ldots, j_q)$ になります。 $p + q$ 項。それから$e_{s.t} = e_s \otimes e_t$。次に、(66) から次のようになります。

$$
\begin{cases}
e_s \wedge e_t^* = 0 & \text{if } s \text{ is not of the form } t.u \\
e_{t.u} \wedge e_t^* = e_u.
\end{cases}
$$

同様に、対称代数 $S(M)$ は、単項式 $e^\alpha$ の基底集合と、単項式 $e^{*\alpha}$ の $\alpha \in \mathbf{N}^n$ (§ 6, no. 6, 定理 1) および $S(M^*)$ 集合を持ちます。 $\alpha \in \mathbf{N}^n$付き。 recall (no. 5) that $u_\alpha$, for $|\alpha| = k$, denotes 元 of 基底 of $(S^k(M))^*$, dual to 基底 $(e^\alpha)_{|\alpha|=k}$ of $S^k(M)$; the $u_\alpha$, for $\alpha \in \mathbf{N}^n$, therefore 形基底 of $S(M)^{*gr}$. 定義 of right 内部積 by $e^\beta$ in $S(M)^{*gr}$ as 転置 of 乗法 by $e^\beta$ in $S(M)$ then shows that

$$
\begin{cases}
u_\alpha \perp e^\beta = 0 & \text{if } \alpha \not\geq \beta \\
u_\alpha \perp e^\beta = u_{\alpha-\beta} & \text{if } \alpha \geq \beta.
\end{cases}
$$

(73)

同様に、ここでは $S(M)$ が $S(M)^{*gr}$ の等級双対で正規に識別されているため、$i(u_\beta)$ は $S(M)^{*gr}$ の $u^\beta$ によって乗法の等級付けされた転置であり、したがって乗法表 (33) (no. 5) から基底 $(u_\alpha)$ 私たちは次のように推測します

$$
\begin{cases}
e^\alpha \perp u_\beta = 0 & \text{if } \alpha \not\geq \beta \\
e^\alpha \perp u_\beta = (\beta, \alpha - \beta)e^{\alpha-\beta} & \text{if } \alpha \geq \beta.
\end{cases}
$$

(74)

$S(M^*)$の元による$S(M)$の元の右側内部積と、この積(no. 9)の定義とno. 5の公式(34)から、次のように推測できます。 (74) 数式

$$
\begin{cases}
e^\alpha \perp e^{*\beta} = 0 & \text{if } \alpha \not\geq \beta \\
e^\alpha \perp e^{*\beta} = \frac{\alpha!}{(\alpha-\beta)!} e^{\alpha-\beta} & \text{if } \alpha \geq \beta.
\end{cases}
$$

(75)

There are analogous formulae for the inner product of an element of $S(M^*)$ by an element of $S(M)$ interchanging the roles of $M$ and $M^*$ (since $M^{**}$ is here identified with $M$).

#### 注意 {#alg-iii-s11-n10-rem-1 .statement tag=068D}

基底 $(e_i)_{1 \leq i \leq n}$ が与えられると、多項式代数 $A[X_1, \ldots, X_n]$ (§ 6, no. 6) で同一視する代数 $S(M)$ が可能になります。 公式 (75) は、$e^{*\alpha}$ による内部積が、$1 \leq i \leq n$ (§ 10, no. 11, 例) の $D_i = \partial/\partial X_i$ である微分演算子 $D^\alpha = D_1^{\alpha_1}D_2^{\alpha_2}\ldots D_n^{\alpha_n}$ であることを示しています。

最後に、外部代数 $\Lambda(M)$ を考えてみましょう。これは、元 $e_J$ の基底集合を持ち、$J$ は、区間の部分集合の集合 $\mathbf{N}$ の $\{1, n\}$ を通過します。 (§ 7, no. 8, 定理 1);同様に、$\Lambda(M^*)$ は基底元 $e_J^*$ となります。 no. 9 の公式 (68) から次のようになります。

$$
\begin{cases}
e_K^* \wedge e_J = 0 & \text{if } K \notin J \\
e_K^* \wedge e_J = (-1)^{p(p-1)/2} \rho_{K, J-K} e_{J-K} & \text{if } K \subset J \text{ and } p = \operatorname{Card}(K),
\end{cases}
$$

(76)

ここで、$\rho_{K, J-K}$ は、§ 7, no. 8 の公式 (19) によって定義される数です。 $M$ と $M^*$ の役割を入れ替えた類似の式があります。

### 11. $\wedge^p(M)$ と $\wedge^{n-p}(M^*)$ の間の同型 $n$ 寸法自由加群 M

#### 命題 12 {#alg-iii-s11-prop-12 .statement tag=068E}

*M を次元 n の自由A-加群とします。 $e \in \wedge^n(M)$ を $\wedge^n(M)$ の基底を形成する元とし、$e^*$ を $\wedge^n(M^*)$ の元とし、$(\wedge^n(M))^*$ で $\{(-1)^{n(n-1)/2} \theta_{\wedge}(e^*)\}$ が $\{e\}$ の双対基底となるようにします。 $\phi : \wedge(M^*) \to \wedge(M)$ を写像 $z \mapsto z \wedge e^*$ および $\phi' : \wedge(M^*) \to \wedge(M)$ 写像 $z^* \mapsto z^* \wedge e$ とします。 $\phi_p$ (それぞれ $\phi'_p$) を、$\phi$ (それぞれ $\phi'$) から $\wedge^p(M)$ (それぞれ $\wedge^p(M^*)$) の制限とします。それから：

(i) *The mapping $\phi$ is a left $\wedge(M)$-module isomorphism and the mapping $\phi'$ is a left $\wedge(M^*)$-module isomorphism; moreover the mappings $\phi$ and $\phi'$ are inverses of one another.*

(ii) *写像 $\phi_p$ は A-加群 $\wedge^{n-p}(M^*)$ 上の A-加群 $\wedge^p(M)$ の同型であり、写像 $\phi'_p$ は A-加群 $\wedge^p(M^*)$ の同型ですA-加群 $\wedge^{n-p}(M)$。

(iii) *$u \in \wedge(M)$と$v^* \in \wedge(M^*)$を$B(u, v^*) = \langle u, \theta_{\wedge}(v^*) \rangle$と書くと、$u^* \in \wedge^p(M^*)$と$v^* \in \wedge^{n-p}(M^*)$は、

$$
B(\phi'_p(u^*), v^*) = (-1)^{p(n-p)} B(u^*, \phi'_{n-p}(v^*)).
$$

The fact that $\phi$ is $\wedge(M)$-linear and $\phi'$ is $\wedge(M^*)$-linear follows from the formulae $(u \wedge v) \wedge e^* = u \wedge (v \wedge e^*)$ and $(u^* \wedge v^*) \wedge e = u^* \wedge (v^* \wedge e)$ (no. 6, formula (37)), using the fact that $\theta_{\wedge}$ is an isomorphism of $\wedge(M^*)$ onto the opposite algebra to $\wedge(M)^*$. 一方、次のような M の基底 $(e_i)_{1 \leq i \leq n}$ が存在します。

$$
e = e_1 \wedge e_2 \wedge \cdots \wedge e_n \quad \text{and} \quad e^* = (-1)^{n(n-1)/2} e_1^* \wedge e_2^* \wedge \cdots \wedge e_n^*,
$$

ここで、$(e_i^*)$ は $(e_i)$ の双対である基底です。 $I = \{1, n\}$と書きます。 (76) から、p 元を持つ I の部分集合 J ごとに、

$$
\begin{cases}
\phi(e_J) = (-1)^{n(n-1)/2 + p(p-1)/2} \rho_{J, I-J} e_I^* J \\
\phi'(e_J^*) = (-1)^{p(p-1)/2} \rho_{J, I-J} e_{I-J}.
\end{cases}
$$

これは、$\phi$ と $\phi'$ が全単射であることを証明します。さらに$\rho_{J, I-J} \rho_{I-J, J} = (-1)^{p(n-p)}$ (§ 7, no. 8, 公式 (21)); 数として

$$
\frac{n(n-1)}{2} + \frac{p(p-1)}{2} + \frac{(n-p)(n-p-1)}{2} + p(n-p) = n(n-1)
$$

が偶数である場合、$\phi$ と $\phi'$ は 1 つの他のの逆数になります。最後に、(77) を証明するには、$u^* = e_J^*$ と $v^* = e_{I-J}^*$ を取るだけで十分です。この検証は、$\theta_{\wedge}$ の定義、式 (78) および関係 $\rho_{J, I-J} \rho_{I-J, J} = (-1)^{p(n-p)}$ (§ 7, no. 8、公式 (21)) からも行われます。 $u^* \in \wedge^p(M^*)$ と $v^* \in \wedge^{n-p}(M^*)$ については、

B(\phi_p'(u^*), v^*) は、符号内では、$\Lambda^n(M^*)$ の基底 $\{e^*\}$ に対して、$u^* \wedge v^*$ の係数です。

#### 命題 13 {#alg-iii-s11-prop-13 .statement tag=068F}

*仮説と命題 11 の記法を使用すると、A-加群 M の自己準同型 g ごとに。*

$$(79)$$
$$(\det g)\phi = \Lambda^{(tg)} \circ \phi \circ \Lambda(g).$$

明らかに$\Lambda^{(tg)} = \theta_{\Lambda}^{-1} \circ (t\Lambda(g)) \circ \theta_{\Lambda}$; $\Lambda(g)$ は代数 $\Lambda(M)$ の自己準同型なので、定義までには、すべての
$$z \in \Lambda(M), \quad \theta_{\Lambda}(\Lambda(g)(z) \perp e^*) = \theta_{\Lambda}(e^*) \perp \theta_{\Lambda}(\Lambda(g)(z)),$$
no. 6 の公式 (42) から次のように推測します。
$$
((\theta_{\Lambda}^{-1} \circ (t\Lambda(g)) \circ \theta_{\Lambda}) \circ \phi \circ \Lambda(g))(z) = \theta_{\Lambda}^{-1}(t\Lambda(g)(\theta_{\Lambda}(e^*)) \perp z)
= z \perp (\Lambda^{(tg)}(e^*)) = (\det g)(z \perp e^*) = (\det g)\phi(z)
$$
§ 8, no. 4、命題を考慮すると 8.

#### 系 {#alg-iii-s11-n11-cor-1 .statement tag=068G}

*E 自己同型 g ごとに、*
$$(80)$$
$$\Lambda^{(tg^{-1})} = (\det g)^{-1}\phi \circ (\Lambda(g)) \circ \phi^{-1}.$$

### 12. p-Vector に関連する部分空間への適用

K を K 上の体および E ベクトル空間とします。すべての $p$ ベクトル $z \in \Lambda^p(E)$ には、E の有限次元部分空間 $M_z$、つまり E の最小のベクトル部分空間 M が関連付けられていることを思い出してください。 $z \in \Lambda^p(M)$ (§ 7, no. 2、系 ～ 命題 4)。

#### 命題 14 {#alg-iii-s11-prop-14 .statement tag=068H}

(i) *$E^*$ の $M_z$ の直交は、$x^* \perp z = 0$ となるように、$x^* \in E^*$ の集合です。

(ii) z に関連付けられている *部分空間 $M_z$ は、E の $\Lambda^{p-1}(E^*)$ の写像 $\lambda_z : u^* \mapsto u^* \perp z$ の下で $\Lambda^{p-1}(E^*)$ の像です。

N を $\lambda_z$ の像とします。 $x^* \in E^*$と$u^* \in \Lambda^{p-1}(E^*)$の場合、
$$
\langle \theta_{\Lambda}(x^*), u^* \perp z \rangle = \langle \theta_{\Lambda}(u^* \wedge x^*), z \rangle = (-1)^{p-1} \langle \theta_{\Lambda}(x^* \wedge u^*), z \rangle \\
= (-1)^{p-1} \langle \theta_{\Lambda}(u^*), x^* \perp z \rangle.
$$
したがって、$x^*$ が N に直交するには、$x^* \perp z$ が $\theta_{\Lambda}(\Lambda(E^*))$ に直交することが必要十分です。さて、後者の条件は$x^* \perp z = 0$のというと同等です。 $(e_{\lambda})_{\lambda \in L}$ を E の基底とします。 L に合計順序を与えると、J の $e_J$ が集合の有限部分集合の $\mathscr{F}(L)$ 、L、形を通過することがわかります (§ 7, no. 8、定理 1)。 $\Lambda(E)$中基底;次に、no. 5 の公式 (30) から、元 $\theta_{\wedge}(e_J^*)$ は、符号内で、基底 $(e_J)$ に対する$\wedge(E)$ 上の座標形であることがわかります。 よって私たちの主張。

したがって、N の直交は $x^* \perp z = 0$ となるような $x^* \in E^*$ で構成され、(i) の結論は (ii) から得られます。

まず、$N \subset M_z$ を示します。 M を E のベクトル部分空間とし、$z \in \wedge(M)$ とし、$j : M \to E$ を標準単射とします。 $\mu_z$ は、$\wedge^{p-1}(M^*)$ の写像 $v^* \mapsto v^* \perp z$ を M に表します。 no. 7 の公式 (60) から正規因数分解が存在することがわかります

$$
\lambda_z : \wedge^{p-1}(E^*) \xrightarrow{\wedge^{p-1}(t_j)} \wedge^{p-1}(M^*) \xrightarrow{\mu_z} M \xrightarrow{j} E
$$

これは、$M_z$の定義によって$N \subset M$、したがって$N \subset M_z$であることを証明します。 $N = M_z$ を検証する必要があります。 逆を仮定します。$M_z$ と元 $x^* \in E^*$ の基底 $(e_i)_{1 \leq i \leq n}$ が存在し、$2 \leq j \leq n$ に対して $\langle x^*, e_1 \rangle = 1, \langle x^*, e_j \rangle = 0$ が存在し、$x^*$ が N に直交するため、$x^* \perp z = 0$ になります。 $z = \sum_H a_H e_H$と書きます。ここで、和は、$\{1, n\}$の部分集合を$p$元で引き継ぎます。 (68) (no. 9) までに、

$$
x^* \perp e_H = 0 \quad \text{if } 1 \notin H \\
x^* \perp e_{\{1\} \cup H} = e_H \quad \text{if } H \subset \{2, n\}
$$

これは、関係 $x^* \perp z = 0$ が $1 \in H$ に対して $a_H = 0$ を意味することを示しています。しかし、これは不可能です。なぜなら、$z$ は属するから $\wedge^p(M')$ になるからです。ここで、$M'$ は $e_2, \ldots, e_n$ によって生成された M の部分空間です。

### 13. 純粋な$p$-ベクトル。グラスマニアン

K を体とし、K に対する E をベクトル空間とします。 $p$-ベクトル $z \in \wedge^p(E)$ は、それが非ゼロであり、$z = x_1 \wedge x_2 \wedge \cdots \wedge x_p$ となるような E 内にベクトル $x_1, \ldots, x_p$ が存在する場合、*純粋* (またはときどき *分解可能*) と呼ばれます。 このためには、$z$ に関連付けられた部分空間 $M_z$ ($z \neq 0$ の場合は常に次元 $\geq p$ である) が次元 $p$ の*正確に* であることが必要かつ十分です ($\wedge^p(M_z)$ は次元 1 であるため)。 特に、E が次元 $n$ の場合、すべての *非ゼロ* スカラー、$E = \wedge^1(E)$ のすべての非ゼロ元、$\wedge^n(E)$ のすべての非ゼロ元は *純粋* です。

#### 命題 15 {#alg-iii-s11-prop-15 .statement tag=068I}

*E を次元 n のベクトル空間とし、e を $\wedge^n(E)$ の元 $\neq 0$ とします (したがって、このベクトル空間の基底を形成します)。 $\phi : \wedge(E) \to \wedge(E^*)$ を e (no. 11、命題 12) に関連付けられたベクトル空間同型とします。 z が $\wedge^p(E)$ の純粋な元である場合、$\phi(z)$ は $\wedge^{n-p}(E^*)$ の純粋な元であり、z に関連付けられた部分空間と $\phi(z)$ は直交します。*

$p = 0$ と $p = n$ のケースは自明です。したがって、$1 \leq p \leq n - 1$ と仮定し、$z = x_1 \wedge \cdots \wedge x_p \neq 0$ とします。すると、$1 \leq i \leq p$と$e = e_1 \wedge e_2 \wedge \cdots \wedge e_n$に対して$e_i = x_i$となるようなEの基底$(e_i)_{1 \leq i \leq n}$が存在します。次に、no. 11の公式 (78) から、$\phi(z) = \pm e_{p+1}^* \wedge \cdots \wedge e_n^*$、よって命題が続きます。

#### 系 {#alg-iii-s11-n13-cor-1 .statement tag=068J}

*E が次元 n の場合、ゼロ以外のすべての $(n-1)$ ベクトル E は純粋です。*

#### 命題 16 {#alg-iii-s11-prop-16 .statement tag=068K}

*$\bigwedge^p(E)$の元$z \neq 0$が純粋であるためには、すべての$u^* \in \bigwedge^{p-1}(E^*)$について、

$$
(u^* \perp z) \wedge z = 0.
$$

$p = 0$ の場合は自明であり、$p \geq 1$ と仮定します。 $z = x_1 \wedge \cdots \wedge x_p$、公式 (68) (no. 9) と$n = p - 1$ は、$u^* \perp z$ が $x_i$ ($1 \leq i \leq p$)、よって (81) の線形結合であることを示します。 一方、$z$ に関連付けられた部分空間 $M_z$ が次元 $> p$ である場合、この部分空間の基底 $(e_j)_{1 \leq j \leq n}$ を $n > p$ と考慮します。 no. 11、命題 13 から、それぞれの $e_j$ は一部の $u^* \in \bigwedge^{p-1}(E^*)$ については形 $u^* \perp z$ であり、関係 (81) は$1 \leq j \leq n$ については $e_j \wedge z = 0$ を意味します。 したがって、式 $z = \sum_H a_H e_H$ (H は $p$ 元を使用して $\{1, n\}$ の部分集合の集合を通過) では、すべての係数 $a_H$ は、反対に、零、よって $z = 0$ であることがわかります。 仮定。

命題 16 の基準は、$u^*$ が $\bigwedge^{p-1}(E^*)$ の *基底* を通過するときに条件 (81) を記述するのと同等です。特に、E が有限次元 $n$ であり、$(e_i)_{1 \leq i \leq n}$ が E の基底であるとします。 条件 (81) は条件と等価です。

$$(82-(J, H))$$
$$
\langle e_J^*, (e_H^* \perp e_I) \wedge z \rangle = 0
$$
$\mathrm{Card}(J) = p + 1$ と $\mathrm{Card}(H) = p - 1$ など、$\{1, n\}$ のすべての部分集合 J、H に対して。さて、IとI'が$\{1, n\}$の2つの部分集合と$p$元の場合、no. 10の式(76)と乗法表の§ 7, no. 8の式(20)は以下を示します。

$$
\langle e_J^*, \langle e_H^* \perp e_I \rangle \wedge e_{I'} \rangle = 0
$$
*〜でない限り* $I - H = \{i\}$ と $J - I' = \{i\}$ のような $i \in \{1, n\}$ が存在します。この場合、

$$(83)$$
$$
\langle e_J^*, (e_H^* \perp e_I) \wedge e_{I'} \rangle = (-1)^{(p-1)(p-2)/2} \varepsilon_{i, J, H}
$$
where $\varepsilon_{i, J, H} = \rho_{\{i\}, H} \rho_{\{i\}, I'}$; it can then be said that for $i \in J \cap C H$, $\varepsilon_{i, J, H}$ is equal to $+1$ if the number of element of J which are $< i$ and the number of elements of H which are $< i$ have the *same parity*, and $-1$ otherwise.

It follows immediately that if we write $z = \sum_I a_I e_I$, where I runs through the set of subsets of $\{1, n\}$ with $p$ elements, relation (82–(J, H)) is equivalent to the relation

$$
\sum_{i \in J \cup C_H} \varepsilon_{i, J, H} a_{J-\{i\}} a_{H \cup \{i\}} = 0.
$$

Relations (84) are called *Grassman’s relations*; these are therefore necessary and sufficient conditions (when J describes the set of subsets with $p + 1$ elements and H the set of subsets with $p - 1$ elements of $\{1, n\}$) for an element $z \neq 0$ of $\bigwedge^p(E)$ to be *pure*.

関係 (84) は独立していないことに注意してください。たとえば、$n = 4$ と $p = 2$ の場合、グラスマンの関係簡約するが単一の関係に変換されます。

$$
a_{12} a_{34} - a_{13} a_{24} + a_{14} a_{23} = 0.
$$

$D_p(E)$ を *純粋な * $p$ ベクトルの $\bigwedge^p(E)$ からなるの部分集合とします。明らかに、$D_p(E)$ は、$u$ と $v$ の間の同値関係に関して飽和しています。「$v = \lambda u$ となるような $\lambda \in K^*$ が存在します」と、$D_p(E)$ の 2 つの元 $u, v$ は、この関係の下で等価です。これらに関連付けられている E の部分空間 $M_u$ と $M_v$ は同じです。 したがって、$\bigwedge^p(E)$ に関連付けられた射影空間* $\mathbf{P}(\bigwedge^p(E))$ の $D_p(E)$ の *像* $G_p(E)$ 上で、E の p 次元ベクトル部分空間* の *集合の *正準全単射* を取得します。 $\mathbf{P}(\bigwedge^p(E))$ の部分集合 $G_p(E)$ は、ベクトル空間 E の添字 $p$ の *グラスマニアン* と呼ばれます。 E が有限次元で、$(e_i)_{1 \leq i \leq n}$ が E の基底であるとき、添字 $p$ のグラスマンニアンは $\mathbf{P}(\bigwedge^p(E))$ の点の集合であり、同次座標 $(a_I)$ の系 ( 基底 $(e_I)$ of $\bigwedge^p(E)$) はグラスマンの関係 (84) を満たします。

When $E = K^n$, we sometimes write $G_{n,p}(K)$ instead of $G_p(K^n)$, so that $G_{n,1}(K) = P_{n-1}(K)$. 写像 $M \mapsto M^0$、$K^n$ のすべての $p$ 次元部分空間と、$E^*$ の *直交* 部分空間 (基底の選択の下で $K^n$ と識別される) $K^n$の標準基底) したがって、定義するは$G_{n,p}(K)$の$G_{n,n-p}(K)$に対する正規の*全単射*です。 命題 15 は、この全単射が射影空間 $\mathbf{P}(\bigwedge^{n-p}(K^n))$ に対する射影空間 $\mathbf{P}(\bigwedge^p(K^n))$ の正準 *同型* の *制限* から $G_{n,p}(K)$ であることを示しています。

### 練習問題 {#alg-iii-s11-exercises}

[§ 11 に対して練習問題](exercises/s11/)を参照してください。
