---
book: ac
book_title: Commutative Algebra
chapter: III
chapter_title: GRADUATIONS. FILTRATIONS AND TOPOLOGIES
section: 3
section_title: m-adic topologies on Noetherian rings
lang: ja
source: ac-i-vii
book_pages: 195-209, 245-255
pdf_pages: 0215-0229, 0265-0275
extraction: ocr
subsections:
    - "no": 1
      title: GOOD FILTRATIONS
      page: 195
      pdf_page: 215
    - "no": 2
      title: m-ADIC TOPOLOGIES ON NOETHERIAN RINGS
      page: 199
      pdf_page: 219
    - "no": 3
      title: ZARISKI RINGS
      page: 201
      pdf_page: 221
    - "no": 4
      title: THE HAUSDORFF COMPLETION OF A NOETHERIAN RING
      page: 202
      pdf_page: 222
    - "no": 5
      title: THE COMPLETION OF A ZARISKI RING
      page: 206
      pdf_page: 226
statements: 39
exercises: 27
content_sha256: f277eedcaabd6d7f82d68357f08742b863e36b9ccb98f25c8dce1b56e523ca87
translated_from: content/en/ac/III/03_s3_m_adic_topologies_on_noetherian_rings.md
translation_method: google
source_content_sha256: e4eba8899949967667773f570b755a00419ebfdad78b7c56f68274079332363d
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 2b6e59fb8f08faa3b0eaf0d37596421cde524d18672dee14e70695cc999e1118
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 3. ネーター 環の $\mathfrak{m}$ 進トポロジ

この段落で検討するすべてのフィルタリングは網羅的であると想定されています。

### 1. 良好な濾過

$\mathbf{A}$ をフィルターされた可換環、E をフィルターされた $\mathbf{A}$ モジュール、$(\mathbf{A}_n)$ と $(E_n)$ とします。

$A$ と $E$ のそれぞれの濾過。 $A_0 = A$ だとします。 多項式環 $A[X]$ 集合 $A' = \sum_{n \geq 0} A_n X^n$ は、型 $\mathbf{N}$* の *段階準 A 代数です。 $E \otimes_A A[X]$ の部分群 $E' = \sum_{n \geq 0} E_n \otimes_A A X^n$ は、型 $\mathbf{N}$ の *グレード付けされた $A'$ モジュール* です。
$$
A_m X^m (E_n \otimes_A A X^n) \subset (A_m E_n \otimes_A A X^n",") \subset E_{m+n} \otimes_A A X^{m+n}.
$$

#### 定義 1 {#ac-iii-s3-def-1 .statement tag=04FX}

*$A$を可換環、$m$を$A$、$E$を$A$モジュール、$(E_n)$を加法群$E$からなるのフィルタリングとします。 $E$中部分加群。ろ過 $(E_n)$ は、次の場合に m-good と呼ばれます:*
(1) $n \in \mathbf{Z}$ 全員に対して $m E_n \subset E_{n+1}$;
(2) *$n \geq n_0$に対して* $m E_n = E_{n+1}$ となるような* 整数 $n_0$ が存在します。

その後、$q$の帰納法までに$m^q E_n = E_{n+q}$で$n \geq n_0, q \geq 1$になります。 条件 (1) は、$A$ に $m$ 進濾過が与えられた場合、濾過 $(E_n)$ が $E$ の $A$ モジュール構造と互換性があることを意味することに注意してください。明らかに、すべての $A$ モジュール $E$ で、 $m$ 進フィルタリングは良好です。 $A$ モジュール $E$ の濾過が M-good の場合、$E$ のいずれかの商加群の商の濾過は M-good です。

#### 定理 1 {#ac-iii-s3-thm-1 .statement tag=04FY}

*$A$を可換環、$m$を$A$の理想、$E$を$A$モジュール、$(E_n)$を無限に生成された加法群$E$からなるの濾過とします。サブ$A$-モジュール。すべての $n$ に対して $m E_n \subset E_{n+1}$ であると仮定します。 $A'$ を $A[X]$ の評価済み部分代数 $\sum_{n \geq 0} m^n X^n$ とし、$E'$ を評価済み $A'$ モジュール $\sum_{n \geq 0} E_n \otimes_A A X^n$ とします。 条件に続く 2 つは同等です:*
(a) *濾過* $(E_n)$ *とても良いです*。
(b) *$E'$ は有限生成された $A'$ モジュールです。*

$n > n_0 \geq 0$ を $m E_{n-1} = E_n$ とします。 $i \leq n_0$ について、$(e_i)_{i \leq n_0}$ を $A$ 加群 $E_i$ の生成元の有限系とします。 $A$ モジュール $E_n \otimes_A A X^n$ は $0 \leq n \leq n_0$ に対して元 $e_{n,j} \otimes X^n$ によって生成され、次と等しくなります。
$$
m^{n-n_0} E_{n_0} \otimes_A A X^n
$$
$n > n_0$ の場合、$A'$ モジュール $E'$ は、$0 \leq n \leq n_0$ および $1 \leq j \leq r_n$ の場合、元 $e_{n,j} \otimes X^n$ によって生成されます。その場合、それは確かに有限に生成されます。

逆に、$E'$ が有限生成された $A'$ モジュールである場合、形 $e_k \otimes X^{n(k)}$ の元の有限族によって生成されます。ここで、$e_k \in E_{n(k)}$ です。 $n_0$ を整数 $n(k)$ の最大のとします。次に、$n \geq n_0$ と $f \in E_n$ については、
$$
f \otimes X^n = \sum_k t_k (e_k \otimes X^{n(k)})
$$
ここで$t_k \in A'$; 置き換えることが $t$ である必要がある場合、次数 $n - n(k)$ の同次成分により、$a_k \in m^{n-n(k)}$ である $t_k = a_k X^{n-n(k)}$ と仮定できます。

一意元 $X^n$ 形基底の A-加群 AX" のように、方程式 $f \otimes X^n = \left( \sum_k a_k e_k \right) \otimes X^n$ は $f = \sum_k a_k e_k$ を意味します。そして、$E_n \subset m^{n-n_0} E_{n_0}$; 逆の包含は明らかなので、

$$
E_n = m^{n-n_0} E_{n_0},
$$

$n > n_0$の場合はよって$E_n = m E_{n-1}$。

#### 補題 1 {#ac-iii-s3-lem-1 .statement tag=04FZ}

*A を可換ネーター 環とし、A のイデアルを仮定します。すると、$A[X]$ の部分環 $A' = \sum_{n \geq 0} m^n X^n$ はネーター になります。

$A'$ は $mX$ によって生成された A-代数です。 A がネーター、$mX$ が有限生成A-加群であるため、結論は § 2, no. 10、系 3 から定理 2 となります。

#### 命題 1 {#ac-iii-s3-prop-1 .statement tag=04G0}

*A を可換ネーター 環とし、m を A のイデアルとする。 A に m-adic フィルタリングを与えます。 E、F を 2 つのフィルタ A-加群と $j : F \to E$ 単射準同型のフィルタと互換性のあるものとします。 E が有限に生成され、その濾過が m-good である場合、F も有限に生成され、その濾過が m-good となります。*

F は E の部分加群と同型なので、A がネーター で E が有限生成されるため、F は有限生成されます。 $(E_n)$、$(F_n)$ を E と F のそれぞれのフィルタリングとし、有限に生成された部分加群から構成されます。 補題 1 の記法を維持すると、集合 $E' = \sum_{n \geq 0} E_n \otimes_A A X^n, F' = \sum F_n \otimes_A A X^n$ になります。 仮定 $F_n$ は $E_n$ の部分加群と同型であることから、F' は $E'$ の部分加群と同型であることがわかります。 定理 1 により、$E'$ は有限生成された $A'$ 加群となり、A' がネーター (補題 1) であるため、F' も同様になります。したがって、定理 1 による結論になります。

#### 系 1 (アーティン・リース補題) {#ac-iii-s3-prop-1-cor-1 .statement tag=04G1}

*A を可換ネーター 環、A のイデアル、E 有限生成A-加群および E の F 部分加群とします。E の m 進フィルタリングによって F に誘発されるフィルタリングは m-good です。*

他の語には、次のような整数 $n_0$ が存在します。

$$
m((m^n E) \cap F) = (m^{n+1} E) \cap F
$$

$n \geq n_0$の皆さんへ。

#### 系 2 {#ac-iii-s3-prop-1-cor-2 .statement tag=04G2}

*A を可換ネーター 環および A の 2 つのイデアル a, b とします。$a^h \cap b \subset ab$ となるような整数 h > 0 が存在します。*

$a^{n+1} \cap b = a(a^n \cap b) \subset ab$ by 系 1 を $E = A, F = b$ に適用するような n が存在します。

#### 系 3 {#ac-iii-s3-prop-1-cor-3 .statement tag=04G3}

*A を可換ネーター 環、A のイデアルと、$O$ の因子ではない、$A$ の x 元とします。 整数 $k > 0$ が存在し、すべての $n \geq k$ に対して、関係 $xy \in m^n$ は $y \in m^{n-k}$ を意味します。

系 1 を $E = A, F = A x$ に適用すると、すべての $n \geq k$、$m^n \cap Ax = m^{n-k}(m^k \cap Ax)$ となるような $k$ が存在することがわかります。次に、$xy \in m^n$ の場合、

$$
xy \in m^n \cap Ax \subset m^{n-k}x
$$

そして、$x$は$0$の因子ではないので、$y \in m^{n-k}$と推測します。

トランスポーター (章 I, § 2, no. 10) の記法では、系 3 の結論が読み取れます。

(2)
$$
m^n : Ax \subset m^{n-k}.
$$

#### 系 4 {#ac-iii-s3-prop-1-cor-4 .statement tag=04G4}

$A$ を可換ネーター 環、$m$ $A$、$E$ を並列生成した $A$ モジュールと 2 つのフィルタ $(E_n)$ と $(E'_n)$ の理想とします。 からなるの部分加群の$E$。 $A$ に $m$ 進濾過が与えられた場合、濾過 $(E_n)$ と $(E'_n)$ が $E$ の $A$ モジュール構造と互換性があるとします。濾過 $(E_n)$ が $m$ 良好で、すべての $n \in \mathbf{Z}$ について $E'_n \subset E_n$ の場合、濾過 $(E'_n)$ は $m$ 良好です。
これは命題 1 の特殊なケースです。

#### 補題 2 {#ac-iii-s3-lem-2 .statement tag=04G5}

$A, B$ を 2 つの可換なネーター 環、$\phi : A \to B$ 環準同型、$E$ を有限生成された $A$ 加群、$F$ を有限生成された $B$ 加群とする。この場合、$\mathrm{Hom}_A(E, \phi_*(F))$ は有限生成された $B$ モジュールです。

仮定によって全射 $A$-準同型性 $v : A^n \to E$ が存在します。したがって、$\mathrm{Hom}_A(E, \phi_*(F))$から$\mathrm{Hom}_A(A^n, \phi_*(F))$の写像$u \mapsto u \circ v$は単射的であり、$B$がネーターであるため、$\mathrm{Hom}_A(A^n, \phi_*(F))$が有限生成された$B$加群であることを証明するのに十分です。 $F^n$ と同型なので、これは明らかです。

#### 命題 2 {#ac-iii-s3-prop-2 .statement tag=04G6}

$A$ を可換ネーター 環、$m$ を 2 つの有限生成された $A$ 加群 $A$ および $E, F$ の理想とする。 $(F_n)$ が $F$ で $m$ 良好な濾過である場合、部分加群 $\mathrm{Hom}_A(E, F_n)$ 形は $A$ モジュール $\mathrm{Hom}_A(E, F)$ で $m$ 良好な濾過です。
$m^k F_n \subset F_{n+k}$ の $n \in \mathbf{Z}, k \geq 0$ と同様に、次のことも真実です。

$$
m^k \mathrm{Hom}_A(E, F_n) \subset \mathrm{Hom}_A(E, F_{n+k});
$$

ファミリ $(\mathrm{Hom}_A(E, F_n))_{n \in \mathbf{Z}}$ は、$m$ 進フィルタリングによってフィルタリングされた、環 $A$ の加群構造と互換性のある $\mathrm{Hom}_A(E, F)$ のフィルタリングになります。 $E$ は有限生成されるため、整数 $r > 0$ と全射的 $A$ 準同型 $u : A^r \to E$ が存在し、定義するは単射的 $A$ 準同型

$$
v = \mathrm{Hom}(u, 1_F) : \mathrm{Hom}_A(E, F) \to \mathrm{Hom}_A(A^r, F);
$$

明らかに、$v$ はフィルター $(\mathrm{Hom}_A(E, F_n))$ および $(\mathrm{Hom}_A(A^r, F_n))$ と互換性があります。
$\mathrm{Hom}_A(E, F)$ と $\mathrm{Hom}_A(A^r, F)$ は有限に生成されるため (補題 2)、濾過 $(\mathrm{Hom}_A(A^r, F))$ が m-good であることを示すには、命題 1 によって十分です。しかし、これは標準同型 $\mathrm{Hom}_A(A^r, F_r) \to F_n^r$ の存在と、関係 $mF_n = F_n +$ が $m(F_n^r) = (mF_n)^r = F_{n+1}^r$ (代数, 章 II, § 3, no. 7, 注意) を意味するという事実により、明らかです。

#### 命題 3 {#ac-iii-s3-prop-3 .statement tag=04G7}

*$A$ をネーター 環とし、$m$ を $A$ がハウスドルフであり、m 進数位相に関して完全であるような $A$ のイデアルとする。 $E$ をフィルタリングされた環 $A$ に対するフィルタリングされた $A$ モジュールとします。$A$ のフィルタリング $(E_n)$ は、$E_0 = E$ と $E$ が次のように定義される位相に関してハウスドルフになるようにします。 $(E_n)$。したがって、次の条件は同等です。
(a) $E$ は有限生成された $A$ 加群であり、$(E_n)$ は m-good フィルタリングです。
(b) $\mathrm{gr}(E)$ は有限生成された $\mathrm{gr}(A)$ 加群です。
(c) すべての $n \geq 0$ に対して、$\mathrm{gr}_n(E)$ は有限生成された $A$ 加群であり、$n \geq n_0$ 標準準同型に対して次のような $n_0$ が存在します。
$$
\mathrm{gr}_1(A) \otimes_A \mathrm{gr}_n(E) \to \mathrm{gr}_{n+1}(E)
$$
全射的です*

定義からすぐに、(a) は (c) を意味することがわかります。 (b) が (c) を意味するという事実は、§ 1, no. 3 の帰結、補題 1 です。逆に、(c) が成り立つ場合、明らかに $\mathrm{gr}(E)$ は、$p \leq n_0$ に対する $\mathrm{gr}_p(E)$ の和によって $\mathrm{gr}(A)$ 加群として生成され、したがって、仮定によって生成元の有限系が認められます。 (c) が (a) を意味することを証明することはまだ残っています。 $\mathrm{gr}_n(E)$ は有限に生成され、$E_n = E$ は明らかに最初に $n$ の帰納法によって、$E/E_n$ はすべての $n$ に対して有限に生成された $A$ モジュールです。したがって、$n > n_0$ の場合、$E_n$ は有限生成された $A$ 加群であり、$mE_n = E_{n+1}$ であることを証明すれば十分です。ここで、徹底的で分離された濾過 $(E_{n+k})(k \geq 1)$ を備えた $A$ モジュール $E_{n+1}$ を考えてみましょう。 $mE_n \subset E_{n+1}$; 仮定 (c) は、$\mathrm{gr}_{n+1}(E) = E_{n+1}/E_{n+2}$ の $mE_n$ の像が、グレード付けされた $\mathrm{gr}(A)$ モジュール $\mathrm{gr}(E_{n+1})$ の $\mathrm{gr}_{n+1}(E)$ および生成するに等しいことを意味します。 $\mathrm{gr}_{n+1}(E)$ は仮定によって有限生成された $A$ 加群であるため、§ 2, no. 9、命題 12 から $mE_n = E_{n+1}$ および $E_{n+1}$ は有限生成された $A$ 加群であることがわかります。

### 2. ネーター 環の m-ADIC トポロジ

#### 命題 4 {#ac-iii-s3-prop-4 .statement tag=04G8}

*$A$ を可換ネーター 環、$m$ を $A$ のイデアル、$E$ を有限生成された $A$ 加群とする。 $E$ 定義するのすべての m-good フィルターは同じ位相 (つまり、m-adic 位相)。*

$(E_n)$ を $E$ に対する M-good フィルタリングとします。このフィルタリングは網羅的であるため、$E$ 属するのすべての元から $E_n$ の 1 つまで、および $E$ は有限に生成され、$E_n$ は $A$ モジュールであるため、次のような整数 $n_1$ が存在します。 $E_{n_1} = E$。一方、$n_0$ を $n \geq n_0$ に対して $mE_n = E_{n+1}$ となるようにします。次に、$n > n_0 - n_1$ については、
$m^n E \subset E_{n+n_1} = m^{n+n_1-n_0} E_{n_0} \subset m^{n+n_1-n_0} E$、これは命題を証明します。

#### 定理 2 (クルル) {#ac-iii-s3-thm-2 .statement tag=04G9}

*$A$ を可換ネーター 環、$m$ を $A$ のイデアル、$E$ を有限生成された $A$ 加群、および $E$ の $F$ 部分加群とします。 次に、$F$ の $m$ 進数位相は、$E$ の $m$ 進数位相によって誘導されます。

no. 1、命題 1 から、$E$ での $m$ 進濾過によって $F$ で誘発された濾過は m-good であることがわかり、結論は命題 4 から得られます。

#### 系 {#ac-iii-s3-n2-cor-1 .statement tag=04GA}

*Let $A$ be a commutative Noetherian ring, $m$ an ideal of $A$, $E$ an $A$-module and $F$ a finitely generated $A$-module. すべての $A$ 線形マッピング $u : E \to F$ は、*$m$ 進トポロジ* の厳密な射* (一般位相、章 111、§ 2, no. 8) です。

$u(m^nE) = m^n u(E)$ として、$u$ は、これら 2 つの加群上の $m$ 進トポロジーの $u(E)$ への $E$ の厳密な射であり、$u(E)$ 上の $m$ 進位相は、 $m$-進数位相オン $F$ by 定理 2.

#### 命題 5 {#ac-iii-s3-prop-5 .statement tag=04GB}

*$A$ を可換ネーター 環、$m$ を $A$ のイデアル、$E$ を有限生成された $A$ 加群とする。 $m$-進数位相に関する $E$ の $\{0\}$ の閉包* $\bigcap_{n=1}^m m^nE$ * は $x \in E$ の集合であり、これに対して元 $m \in m$ が存在し、* $(1 - m)x = 0$ となります。

$x = mx$ の場合、$m \in m$、整数 $n \geq 0$ ごとに $x = m^n x \in m^nE$、したがって $x \in F = \bigcap_{n=0}^m m^nE$ になります。逆に、$x \in F$の場合、$Ax$は$E$の0の近傍の共通部分に含まれます。次に、定理 2 から、$E$ の$Ax$ の$m$ 進数位相が最も粗い位相であることがわかります。 $mx$ は 0 の定義近傍とこの位相, $mx = Ax$ により、したがって $x = mx$ となる $m \in m$ が存在します。

$mF = F$ 以降とも言えます
$$
F = \bigcap_{n=1}^\infty m^{n+1}E \subset m. \bigcap_{n=1}^\infty m^nE = mF;
$$
$A$ はネーター であるため、$F$ は有限生成された $A$ 加群です。その場合、章 II, § 2, no. 2、系 3 から命題 4 を適用するだけで十分です。

#### 系 (クルル) {#ac-iii-s3-n2-cor-2 .statement tag=04GC}

*$A$を可換ネーター環、$m$を$A$の理想とする。理想* $\bigcap_{n=1}^m m^n$ *は元* $x \in A$ の集合です* $m \in m$ * $(1 - m)x = 0$ が存在します。 *特に* $\bigcap_{n=1}^\infty m^n = \{0\}$ については、 * $1 + m$ の元が * $0$ * の因子に * $A$ 含まれないことが必要かつ十分です。

命題を適用する 5 ～ $E = A$ までで十分です。

#### 注意 {#ac-iii-s3-n2-rem-1 .statement tag=04GD}

この系では$A$が*ネーター*である仮定が必須です。たとえば、$A$ を、$\mathbf{R}$ からそれ自体まで無限微分可能な写像の環とし、$m$ を、写像 $f$ の$A$ からなるの（極大）イデアルとします。 $f(0) = 0$。 $\bigcap_{n=0}^\infty m^n$ が写像 $f$ の集合であることは明らかであり、すべての $n \geq 0$ に対して $f^{(n)}(0) = 0$ が存在し、すべての $x \neq 0$ に対して $f(x) \neq 0$ を持つそのような写像が存在します。 写像 $f$ は、$x \neq 0$ および $f(0) = 0$ に対して $f(x) = e^{-1/x^2}$ によって定義されます。

#### 定義 1 {#ac-iii-s3-def-1-bis .statement tag=04GE}

*$\mathbf{A}$を位相幾何学的な環とします。 $\mathbf{A}$ の両側イデアル $m$ が、$\mathbf{A}$ 上の指定された位相が $m$ 進数位相であるような場合、$m$ は定義イデアルと呼ばれ、$\mathbf{A}$ 上の位相と呼ばれます。

$A$ を可換ネーター 環、$m$ $A$ および $t$ をその根基 (章 II, § 2, no. 6) とします。 $m'$ が $m$ 進数位相の定義的なイデアである場合、${m'}^n \subset m$ ($§ 2$, no. 5)、したがって $m' \subset t$ となるような整数 $n > 0$ が存在します。逆に、$A$ はネーター であるため、$t^k \subset m$ (章 II, § 2, no. 6, 命題 15) となる整数 $k > 0$ が存在し、したがって $t$ は *最大のが理想を定義する* ことになります。 $m$-進数位相。

### 3. ザリスキー 環

#### 命題 6 {#ac-iii-s3-prop-6 .statement tag=04GF}

*$A$を可換ネーター環、$m$を$A$の理想とする。次のプロパティは同等です。
(a) $m$ は、$A$ のヤコブソン根基に含まれています。
(b) *有限に生成されたすべての $A$ モジュールは、$m$ 進数位相を持つハウスドルフです。*
(c) *有限生成されたすべての $A$ モジュール $E$ について、$E$ のすべての部分加群は、$E$ の $m$ 進数位相に関して閉じられます。
(d) *$A$ のすべての最大イデアルは、$m$ 進数位相に関して閉じられています。*

(a) が (b) を意味することを示しましょう。 $m$ が $A$ の Jacobson 根基に含まれていると仮定し、$E$ を有限生成された $A$ 加群とする。 $x \in E$ と $m \in m$ が $(1 - m)x = 0$ となるような場合、$1 - m$ は $A$ で可逆であるため、$x = 0$ になります。次に (no. 2, 命題 5) $E$ は、$m$ 進数位相を持つハウスドルフです。

(b) が (c) を意味することを証明しましょう。 (b) が成り立つと仮定します。 $E$ を有限生成された $A$ モジュール、および $E$ の $F$ 部分加群とします。次に、$E/F$ は $m$ 進数位相を持つハウスドルフであり、これは $E$ 上の $m$ 進数位相の商位相です。その後、$F$は$E$でクローズされます。

明らかに (c) は (d) を意味します。 最後に、(d) が (a) を意味することを示しましょう。 (d) から、$A$ のすべての最大イデアル $a$ に対して、$A$ 加群 $A/a$ は $m$ 進数位相を持つハウスドルフであることがわかります。 This implies $m(A/a) \neq A/a$, unless the $m$-adic topology on $A/a$ were the coarsest topology and $A/a$ were reduced to 0, which is absurd since $A/a$ is *ajield*. したがって、$A/a$の$m$の標準像は、$A/a$とは異なる$A/a$の理想であり、したがって0に減らされます。次に$m \subset a$、これは$m$が$A$のヤコブソン根基に含まれていることを証明します。

#### 定義 2 {#ac-iii-s3-def-2 .statement tag=04GG}

*位相幾何学的環 $A$ は、可換でネーター であり、$A$ 満たす上の位相に対して、命題 6 の等価条件に対する定義的なイデアル $m$ が存在する場合、ザリスキー 環と呼ばれます。

ザリスキー 環 $A$ は必然的に *ハウスドルフ* (命題 6) であり、その位相を定義する理想の *すべて* が $A$ のヤコブソン根基に含まれています。

*例のザリスキー 環*

#### 例 1 {#ac-iii-s3-n3-exa-1 .statement tag=04GH}

$A$ を可換ネーター 環とし、$m$ を $A$ のイデアルとします。 $A$ が *Hausdorff で、m 進数位相* で完了する場合、$A$ は、§ 2, no. 13、補題 3 のおかげで、この位相を持つザリスキー 環になります。

#### 例 2 {#ac-iii-s3-n3-exa-2 .statement tag=04GI}

ザリスキー 環のすべての *商環* $A/b$ は、ザリスキー 環です。なぜなら、それはネーター であり、$m$ が $A$ の定義的な理想である場合、$m(A/b) = (m + b)/b$ は $A/b$ のジェイコブソン根基に含まれます。 (*代数*、章 VIII, § 6, no. 3、命題 7)。

#### 例 3 {#ac-iii-s3-n3-exa-3 .statement tag=04GJ}

$A$ を *ネーター 準ローカル* 環とし、$r$ をそのジェイコブソン根基とします。次に、$r$-進数位相を持つ $A$ は、ザリスキー 環です。 ネーター 準局所リングをトポロジカル環として考慮する場合、これは常に位相になります (〜でない限り別途記載)。

#### 命題 7 {#ac-iii-s3-prop-7 .statement tag=04GK}

*$A, A'$ を 2 つの可換環と $h : A \to A'$ 環準同型とします。 $A$ がネーター で、$A'$ が有限生成された $A$ モジュール ($h$ によって定義された構造を持つ) であると仮定します。 $m$を$A$の理想とし、$m' = mA'$とします。それから：*

(i) *$A'$ の $m'$ 進数位相がハウスドルフであるためには、$1 + h(m)$ の元が $A'$ の $0$ の因子ではないことが必要かつ十分です。*

(ii) * $m$ 進数位相を持つ $A$ がザリスキー 環である場合、$m'$ 進数位相を持つ $A'$ はザリスキー 環です。

(iii) *If $h$ is injective (thus identifying $A$ with a subring of $A'$), the $m'$-adic topology on $A'$ induces on $A$ the $m$-adic topology.*

$A'$ 一致するの $m'$ 進フィルタリングと *A-加群* $A'$ (§ 2, no. 1、*例 3*) の $m$ 進フィルタリングを思い出してください。したがって、主張 (i) は no. 2 の命題 5 の特殊なケースであり、主張 (iii) no. 2 の定理 2 の特殊なケースです。最後に(ii)を示します。 $A$ が $m$ 進数位相を持つザリスキー 環であり、$E'$ を有限生成された $A'$ 加群であるとします。また、有限生成された $A$ モジュールと、$E'$ 一致するの $m$ 進数および $m'$ 進数のフィルタリングでもあります。この場合、$E'$ は $m'$ 進数位相を持つハウスドルフです。最後に、$A$加群$A'$はネーター、よって環$A'$はネーターとなり、$A'$がザリスキー環である証明が完成します。

### 4. ネーター 環のハウスドルフ完成

Let $A$ be a commutative ring, $m$ an ideal of $A$ and $E$ an $A$-module; let $\hat{A}$ and $\hat{E}$ denote the respective Hausdorff completions of $A$ and $E$ with respect to the $m$-adic topology and $j_E$ the canonical mapping $E \to \hat{E}$. $\hat{A} \times E$ から $\hat{E}$ 定義するへの $A$ 双線形マッピング $(a, x) \mapsto aj_E(x)$ および $A$ 線形マッピング

$$
\alpha_E : \hat{A} \otimes_A E \to \hat{E},
$$

*正規*と呼ばれます。 Let $u : E \to F$ be an $A$-module homomorphism and let $\hat{u} : E \to \hat{F}$ be the mapping obtained by passing to the Hausdorff completions; for $a \in \hat{A}$, $x \in E$,

$$
\alpha_F(a \otimes u(x)) = aj_F(u(x)) = a\hat{u}(j_E(x)) = \hat{u}(\alpha_E(a \otimes x)),
$$

その他語、図式

$$
\begin{array}{ccc}
\hat{A} \otimes_A E & \xrightarrow{1 \otimes u} & \hat{A} \otimes_A F \\
\downarrow \alpha_E & & \downarrow \alpha_F \\
\hat{E} & \xrightarrow{\hat{u}} & \hat{F}
\end{array}
$$

可換です。最後に、§ 2, no. 12, 命題 16 から、E が有限生成される場合、準同型 $\alpha_E$ は全射であることがわかります。

#### 定理 3 {#ac-iii-s3-thm-3 .statement tag=04GL}

*A を可換ネーター 環とし、A と E、F、G の 3 つの有限生成された A 加群のイデアルとします。それから：*

(i) ** $E \xrightarrow{u} F \xrightarrow{v} G$ * が A-線型写像の完全系列である場合、数列* $\hat{E} \xrightarrow{\hat{u}} \hat{F} \xrightarrow{\hat{v}} \hat{G}$ *ハウスドルフ完全化 (m 進トポロジーに関して) 移行によって取得されたものは正確です。*

(ii) *正準 A-線型写像* $\alpha_E : \hat{A} \otimes_A E \to \hat{E}$ *全単射です*。

(iii) *A-加群* $\hat{A}$ *フラットです*

$u$ と $v$ はトポロジカル群 (no. 2、系から定理 2) の厳密な射であることがわかりました。 主張 (i) は、§ 2, no. 12、補題 2 から続きます。 主張 (ii) は、$E = A$ のときに明らかであり、E がフリーの場合有限生成A-加群はすぐにそれに帰着できます。一般的なケースでは、E は有限のプレゼンテーションを許可します。

$$
L \xrightarrow{u} L' \xrightarrow{v} E \longrightarrow 0
$$

(章 I, § 2, no. 8、補題 8)。可換図式を導き出します。

$$
\begin{array}{ccccccccc}
\hat{A} \otimes_A L & \xrightarrow{1 \otimes u} & \hat{A} \otimes_A L' & \xrightarrow{1 \otimes v} & \hat{A} \otimes_A E & \longrightarrow & 0 \\
\downarrow \alpha_L & & \downarrow \alpha_{L'} & & \downarrow \alpha_E \\
\hat{L} & \longrightarrow & \hat{L}' & \longrightarrow & \hat{E} & \longrightarrow &
\end{array}
$$

最初の行は正確 (章 I, § 2, no. 1, 補題 1) であり、(i) による 2 行目も同様です。 $\alpha_E$ は全射法 (§ 2, no. 12, 命題 16) であることはすでにわかっています。一方、$\alpha_L$ と $\alpha_{L'}$ は全単射であり、$1 \otimes v$ は全単射であるため、章 I, § 1, no. 4、系 2 ～ 命題 2 により、$\alpha_E$ は単射です。これは(ii)を示しています。

次に、(i) と (ii) から、$a$ が A のイデアル (必然的に有限に生成される) である場合、標準写像 $\hat{A} \otimes_A a \to \hat{A}$ は単射であり、$\hat{a} \to \hat{A}$ と $\alpha_E$ の合成であり、$\hat{A}$ が平坦な$A$ 加群であることが証明されます。 (章 I, § 2, no. 3、命題 1)。

定理 3 の条件の下では、標準写像 $\alpha_E$ によって 3 $\hat{A} \otimes_A E$ が $E$ と識別されることがよくあります。 $u : E \to F$ が有限生成された $A$ 加群の準同型である場合、$\hat{u} : E \to \hat{F}$ は図式の可換性によって $1 @ u$ と識別されます (4)。

#### 系 1 {#ac-iii-s3-thm-3-cor-1 .statement tag=04GM}

$A$ を可換ネーター 環、$m$ $A$ のイデアル、$E$ を有限生成された $A$ 加群、$F$ と $G$ を 2 つの部分加群とします。 $E$。 $A, E, F, G$ に $m$ 進トポロジが与えられ、$i$ が $E$ から $e$ までの標準写像であるとします。次に:

$$
\hat{F} = \hat{A}.i(F), \quad (F + G)^{\wedge} = \hat{F} + \hat{G}, \quad (F \cap G)^{\wedge} = \hat{F} \cap \hat{G},
$$
$$
(F : G)^{\wedge} = \hat{F} : \hat{G}.
$$

さらに、$a$と$b$が$A$と$c = ab, \hat{c} = \hat{a}\hat{b}$の2つの理想であるとします。

定理 3 により、$\hat{E}, \hat{F}, \hat{G}$ は正規に $\hat{A} \otimes_A E, \hat{A} \otimes_A F, \hat{A} \otimes_A G$ と識別され、最初の 2 つの式が確立されます。 3 番目と 4 番目は、それぞれ章 I, § 2, no. 6、命題 6、no. 10、命題 12 と続きます。最後に、$\hat{a} = \hat{A}i(a), \hat{b} = \hat{A}i(b), \hat{c} = \hat{A}i(c)$ として、
$$
\hat{c} = \hat{A}i(ab) = \hat{A}i(a)i(b) = \hat{a}\hat{b}.
$$

#### 系 2 {#ac-iii-s3-thm-3-cor-2 .statement tag=04GN}

$A$ を可換ネーター 環、$m$ を $A$ のイデアル、$\hat{A}$ を $m$ 進数位相に関する $A$ のハウスドルフ完成とします。 元 $a \in A$ が $A$ の 0 の因子ではない場合、$\hat{A}$ の標準像 $a'$ は、$\hat{A}$ の 0 の因子ではありません。

$\hat{A}$ はフラットな $A$ モジュールであるため、系は章 I, § 2, no. 4、命題 3 (i) の特殊なケースです。

#### 系 3 {#ac-iii-s3-thm-3-cor-3 .statement tag=04GO}

$A$ が可換ネーター 環の場合、形式冪系列 $A[[X_1, \ldots, X_n]]$ の環はフラット $A$ 加群です。

多項式環の完成です
$$
B = A[X_1, \ldots, X_n]
$$
$m$ 進数位相に関して、$m$ は定数項 ($§ 2,$ no. 12, 例 1) を持たない多項式の集合です。 $B$ はネーター ($§ 2,$ no. 10、系 2 ～ 定理 2)、$A[[X_1, \ldots, X_n]]$ は定理 3 によるフラット $B$ モジュール、$B$ と同様に無料です$A$ モジュール、$A[[X_1, \ldots, X_n]]$ はフラット $A$ モジュール (章 I, § 2, no. 7、系 3 ～ 命題 8)。

#### 命題 8 {#ac-iii-s3-prop-8 .statement tag=04GP}

$A$ を可換ネーター 環、$m$ を $A$ のイデアル、$\hat{A}$ を $m$ 進数位相に関する $A$ のハウスドルフ完成とします。 $j$ 標準写像 $A$ から $\hat{A}$ まで。の:
(i) $\hat{A}$ はザリスキー 環であり、$\hat{m} = \hat{A}.j(m)$ は $\hat{A}$ の決定的な理想です。

(ii) *写像* $n \mapsto A = \hat{A}.j(n)$ * の最大理想の集合の全単射 $A$ *含む* $m$ * の最大理想の集合 $\hat{A}$ *および* $q \mapsto j^{-1}(q)$ *は逆全単射* です。

(iii) *$n$ *$A$ *含む* $m$ の最大の理想とする*。 *準同型* $j': A_n \to \hat{A}_{\hat{n}}$ *由来* $j$ *は単射; * $A$ の場合、* $j$ * $\hat{A}$ の部分環によって識別され、* $A_n$ 上の* $(nA_n)$*-進数位相は * $A$*-進数位相によって誘導されます。 * $\hat{A}_{\hat{n}}$ * と* $A_n$ * $A$ に密集しており、 * $A$* 進数位相* が含まれています。

(i) を示しましょう。 $m$ は有限生成されたイデアルであるため、$(m^n)^{\wedge} = (\hat{m})^n = m^n \hat{A}$ (§ 2, no. 12、系 2 ～ 命題 16) と $\hat{A}$ 上の位相は $m$ 進数位相です。 $\hat{A}/\hat{m}$ は $A/m$ と同型であるため、ネーター 環であり、$\hat{m} = m \hat{A}$ は有限生成された $A$ 加群であるため、$\hat{A}$ はネーター (§ 2, no. 10, 系) 5から定理 2);最後に、$\hat{A}$ はハウスドルフであり、$m$ 進数位相に関して完全であるため、$\hat{A}$ はザリスキー 環 (no. 3, *例* 1) です。

主張 (ii) は、$j$ から導出された標準準同型 $A/m + \hat{A}/\hat{m}$ が全単射であるという事実と、$\hat{A}$ がザリスキー 環とジェイコブソンであるため、$\hat{A}$ 含む $\hat{m}$ のすべての最大イデアルが成り立つという事実からすぐに続きます。 $\hat{A}$ の根基次に、含む $m$ (no. 3、命題 6)。

最後に(iii)を証明しましょう。 $n = j^{-1}(A)$、$j(A - n) \subset \hat{A} - \hat{n}$、$j$ のように、確かに定義する準同型 $j': A_n \to \hat{A}_{\hat{n}}$ (章 II, § 2, no. 1, 命題 2)。 $j'$ が単射であることを示しましょう。 $a \in A, s \in A - n$ を次のようにしましょう
$$
j'(a/s) = j(a)/j(s) = 0;
$$
その場合、$s'j(a) = 0$ (章 II, § 2, no. 1, *注意* 3) および $\hat{A}$ の $j(a)$ の消滅子が$\hat{n}$ に含まれないような $s' \in \hat{A} - \hat{n}$ が存在します。ここで、$b$ が $A$ の $a$ の消滅子である場合、$\hat{A}$ の $j(a)$ の消滅子は $b$ (系 1 ～ 定理 3) です。したがって $b \notin n$ は、$a/s = 0$ を示します。

さらに、可換図式があります。
$$
\begin{array}{ccc}
A/n^k & \longrightarrow & A_n/(nA_n)^k \\
h \downarrow & & h' \downarrow \\
\hat{A}/\hat{n}^k & \longrightarrow & \hat{A}_{\hat{n}}/(\hat{n}\hat{A}_{\hat{n}})^k
\end{array}
$$
ここで、$h$ と $h'$ はそれぞれ $j$ と $j'$ から導出され、水平矢印は章 II, § 3, no. 3、命題 9 の標準同型です。 $n^k$ は $A$ の開いた理想です (以来含む $m^k$)、$h$ は全単射なので、$h'$ も同様です。これはまず、$A_n$ の $(nA_n)^k = j'((\hat{n}\hat{A}_{\hat{n}})^k)$、したがって位相が $A_n$ の⟦ によって誘発されることを示しています。さらに、$k > 0$すべてに対して$\hat{A}_{\hat{n}} = A_n + (\hat{n}\hat{A}_{\hat{n}})^k$、したがって$A_n$は$A_n$のどこにでも密集しています。

#### 系 {#ac-iii-s3-n4-cor-1 .statement tag=04GQ}

*$A$ *ネーター ローカル* (それぞれ *セミローカル*) *環および* $m$ *そのジェイコブソン根基とします。すると* $\hat{A}$ *はネーター ローカル* (または *セミローカル*) *環そのジェイコブソン根基は* $\hat{m}$ です。

$\hat{A}$ は命題 8 (i) によるネーター であり、残りは命題 8 (ii) と系 1 から定理 3 の 3 番目の公式に続きます。

### 5. ザリスキーの完成環

#### 命題 9 {#ac-iii-s3-prop-9 .statement tag=04GR}

$A$ を可換ネーター 環とし、$m$ を $A$ の理想とします。 $A$ に $m$ 進数位相を与えましょう。 $\hat{A}$ が忠実にフラットな $A$ モジュールであるためには、$A$ がザリスキー 環であることが必要かつ十分です。

For every finitely generated $A$-module $M$, the canonical mapping $M \to M \otimes_A \hat{A}$ is identified with the canonical mapping $M \to \hat{M}$ from $M$ to its Hausdorff completion with respect to the $m$-adic topology (no. 4, Theorem 3) and the kernel of this mapping is then the closure of $\{0\}$ in $M$ with respect to this topology. $\hat{A}$ がフラット $A$ モジュール (no. 4、定理 3) であることはすでにわかっていますが、命題は忠実にフラット加群 (章 I, § 3, no. 1、命題 1 (b)) の特徴付けから続き、ザリスキー環の特徴付け（no. 3、命題6）。

$A$ がザリスキー 環で、$E$ が有限生成された $A$ 加群である場合、標準写像を使用して、命題 9 のおかげで $\hat{E}$ の部分集合を使用して同一視する $E$ を得ることができます。 $j_E : E \to \hat{E}$。この識別情報を使用すると、次のようになります。

#### 系 1 {#ac-iii-s3-prop-9-cor-1 .statement tag=04GS}

$A$ をザリスキー 環、$E$ を有限生成された $A$ 加群、$E$ の $F$ 部分加群とします。次に$F = \hat{F} \cap E = (\hat{A}F) \cap E$。

これは章 I, § 3, no. 5、命題 10 (ii) の特殊なケースであり、no. 3、命題 6 からも続きます。

#### 系 2 {#ac-iii-s3-prop-9-cor-2 .statement tag=04GT}

$A$ をザリスキー 環とし、$E$ を有限生成された $A$ 加群とする。 $\hat{E}$ が無料の $A$ モジュールである場合、$E$ は無料の $A$ モジュールです。

$m$ を $A$ の定義的な理想とする。したがって、それは $A$ のヤコブソン根基に含まれる。 章 II, § 3, no. 5、命題 5 の基準を適用します: 標準写像 $j_E : E \to \hat{E}$ 定義する全単射 $i_E : E/mE \to \hat{E}/(mE)^{\wedge}$;同様に、標準写像 $j_A : A \to \hat{A}$ 定義する全単射 $i_A : A/m \to \hat{A}/\hat{m}$、つまり環同型です。次に、$(mE)^{\wedge} = \hat{A}.mE = \hat{m}\hat{E}$ (no. 4, 定理 3) となり、$\hat{E}/(mE)^{\wedge}$ には $(\hat{A}/\hat{m})$ モジュール構造が与えられ、したがって ($i_A$ によって) $(A/m)$ モジュール構造が与えられます。 $i_E$ が $(A/m)$ 線形であるため、$(A/m)$ 加群同型となるのは明らかです。 $\hat{E}/\hat{m}\hat{E}$ は無料の $(\hat{A}/\hat{m})$ モジュールであるため、$E/mE$ は無料の $(A/m)$ モジュールです。

一方、$\nu : m \otimes_A E \to E$ を標準準同型とします。 $(m \otimes_A E) \otimes_A \hat{A}$ は正規的に $m \otimes_A \hat{E}$ と、$E \otimes_A \hat{A}$ は $\hat{E}$ (no. 4、定理 3) と識別され、仮定 $\hat{E}$ が無料の $\hat{A}$ モジュールであることは、準同型 $\nu \otimes 1 : \hat{m} \otimes_{\hat{A}} \hat{E} \to \hat{E}$ が単射的な。 $\hat{A}$ は忠実に平坦な $A$ 加群 (命題 9) であるため、$\nu$ が単射であることを結論する (章 I, § 3, no. 1、命題 2)、上記の適用に対して条件確かに基準は満たされています。

#### 系 3 {#ac-iii-s3-prop-9-cor-3 .statement tag=04GU}

$A$ を、$\hat{A}$ が整域となるようなザリスキー 環とし、$a$ を $A$ の理想とする。 $\hat{A}$ の理想的な $a\hat{A}$ が主である場合、$a$ が主です。

これは系 2 の特殊なケースです。

#### 系 4 {#ac-iii-s3-prop-9-cor-4 .statement tag=04GV}

$A$ をザリスキー 環とし、$\hat{A}$ が $\hat{A}$ の分数の整域、$L$ 体、および $K \subset L$ 体の分数となるようにします。 $A$;それから$\hat{A} \cap K = A$。

明らかに$A \subset \hat{A} \cap K$;一方、$x \in \hat{A} \cap K$ の場合は、$\hat{A}x \subset \hat{A}$ となり、$\hat{A}x = \hat{A} \otimes_A (Ax)$ (no. 4, 定理 3)、$\hat{A} \otimes_A ((Ax + A)/A) = 0$ となります。 $\hat{A}$ は忠実に平坦な $A$ 加群 (命題 9) であるため、$Ax \subset A$、よって $x \in A$ と推定されます。

#### 系 5 {#ac-iii-s3-prop-9-cor-5 .statement tag=04GW}

$A$ を可換ネーター 環、$E, F$ の 2 つの有限生成された $A$ 加群、および $u : E \to F$ を $A$ 準同型とする。 $A$ のすべての最大イデアル $m$ について、$A(m)$ (それぞれ $E(m), F(m)$) が、$m$ 進数位相に関する$A$ (それぞれ $E, F$) のハウスドルフ完成を表すものとします。 $u(m) : E(m) \to F(m)$ 対応する準同型から $u$ まで。 $u$ が単射的であるためには (それぞれ全単射、全単射、零)、すべての最大理想 $m \notin A$ に対して $u(m)$ がそうであることが必要かつ十分です。

$u$ が単射法 (全単射、全単射、零) であるためには、$A$ (章 II, § 3, no. 3, 定理 1) のすべての最大理想 $m$ について、$u_m : E_m \to F$ がそうであることが必要かつ十分であることがわかっています。ここで、$A$ はネーター 局所環 (章 II, § 2, no. 4, 系 2 から命題 10) であるため、ザリスキー 環があり、標準的 $A$-代数同型写像が存在することに注意してください。 $\hat{A}_m \to A(m)$ (§ 2, no. 13、命題 18)。一方 (no. 4 の始まり) には、可換な図式があります。

$$
\begin{array}{ccc}
E_m \otimes_{A_m} A(m) & \longrightarrow & E \otimes_A A(m) \longrightarrow E(m) \\
u_m \otimes 1 \downarrow & & \downarrow u \otimes 1 \downarrow u(m) \\
F_m \otimes_{A_m} A(m) & \longrightarrow & F \otimes_A A(m) \longrightarrow F(m)
\end{array}
$$

ここで、左側の水平矢印は、テンソル積と同型 $E_m \to E \otimes_A A_m, F_m \to F \otimes_A A_m$ の結合から生じます。 $E$ と $F$ は有限生成された $A$ モジュールであるため、no. 4, 定理 3 から、この図式の行は同型で構成されることがわかります。したがって、証明に還元されます。つまり、$u_m$ が単射詞 (全単射、全単射、零) であることは、$u_m \otimes 1$ がそうであることと同等です。しかし、これは、$\hat{A}_m$ (したがって、$A(m)$) は、命題 9 (章 I, § 3, no. 1、命題 1 および 2) による忠実にフラットな $A_m$ モジュールであるという事実から派生します。

#### 命題 10 {#ac-iii-s3-prop-10 .statement tag=04GX}

$A, B$ を 2 つのザリスキー 環、$\hat{A}, \hat{B}$ の補完、$f : A \to B$ $f$ から移行で補完まで得られた連続環準同型と $\hat{f} : \hat{A} \to \hat{B}$ 準同型とします。 $\hat{f}$ が全単射である場合、$A$ 加群 $B$ は忠実に平坦です。

$A$ と $B$ はハウスドルフであるため、 $\hat{f}$ が全単射であるという仮定は、まず $f$ が単射であることを意味します。オフという手段によって $A$ と $f(A)$ を (代数的に) $\hat{f}$ によって $\hat{A}$ と $\hat{B}$ を（代数的に）識別すると、包含物 $A \subset B \subset \hat{A} = \mathbf{8}$ が得られます。 $\hat{A}$ は忠実にフラットな $A$ モジュールと忠実にフラットな $B$ モジュール (命題 9) であることがわかります。 結論するは、$B$ が忠実にフラットな $A$ モジュール (章 I, § 3, no. 4, 注意 2) であることがわかります。

#### 命題 11 {#ac-iii-s3-prop-11 .statement tag=04GY}

$\mathbf{A}$ をネーター 局所環とし、$m$ をその最大理想とし、$\hat{\mathbf{A}}$ を $m$ 進数完了とし、$\mathbf{A} \subset B \subset \hat{\mathbf{A}}$ となるように $B$ 環とします。 $B$ がネーター 局所環であり、その最大理想 $n$ が関係 $n = mB$ を満たすとします。それから

$$
n^k = m^kB = \hat{m}^k \cap B
$$

すべての $k \geq 1$ について、$B$ の $n$ 進数位相は、$\hat{\mathbf{A}}$ の $m$ 進数位相によって誘導され、$B$ は忠実にフラットな $\mathbf{A}$ モジュールであり、 $\hat{\mathbf{A}}$ の同型は、$B$ の $n$ 進数完了 $\hat{B}$ に、拡大する標準単射 $\mathbf{A} \to B$ になります。

関係 $n^k = \hat{m}^k \cap B$ を検証するだけで十分です。なぜなら、$B$ が $\hat{\mathbf{A}}$ に密集しており、$n$ 進数位相が $m$ 進数位相によって誘導されるため、*General から最後の主張が続きます。 位相*、章 II, § 3, no. 9、系 1 から命題 18 と命題 10 からの最後から 2 つ。単射 $j_A : \mathbf{A} \to \hat{\mathbf{A}}$ (それぞれ $j : B \to \hat{\mathbf{A}}$) 定義する商単射準同型

$$
i_1 : \mathbf{A}/(\hat{m} \cap \mathbf{A}) \to \hat{\mathbf{A}}/\hat{m}
$$

(それぞれ $i_B : B/(\hat{m} \cap B) \to \hat{\mathbf{A}}/\hat{m}$)。 $m \cap \mathbf{A} = m$ と $i_A$ は全単射であることがわかっているため、 $i_B$ は全単射であり、これは $B/(\hat{m} \cap B)$ が体であることを示しており、したがって $\hat{m} \cap B$ は $B$ の最大理想であり、したがって $m \cap B = n$ であることがわかります。 $\mathbf{A} = \mathbf{A} + m$、$B = A + n = A + mB$ として。 $k$の帰納法までに、私たちは次のように推測します

$$
B = A + m^kB = A + n^k
$$

すべての$k > 1$に。 $n^k \subset \hat{m}^k \cap B$ として、$\hat{m}^k \cap B \subset n^k$ を示すだけで十分です。 $b \in \hat{m}^k \cap B$ の場合、$a \in \mathbf{A}$、$z \in n^k$ の場合、$b = a + z$ と書くことができます。 よって

$$
a = b - z \in \hat{m}^k \cap \mathbf{A} = m^k \subset n^k
$$

そして$b \in n^k$。

\* これが当てはまる重要なケースは次のとおりです: $B$ は、完全な値体に対する $n$ 変数の整数系列の環で、0 の近傍に収束し、$\mathbf{A}$ は局所環

$$
K[X_1, \ldots, X_n]_{\mathfrak{p}}
$$

ここで、$\mathfrak{p}$ は定数項を持たない多項式の最大理想値からなるであり、$\hat{\mathbf{A}}$ は形式的な冪系列 $K[[X_1, \ldots, X_n]]$ の環です。 \*

#### 注意 {#ac-iii-s3-n5-rem-1 .statement tag=04GZ}

局所環 $B$ は、その最大理想値 $n$ が $mB$ に等しく、その $n$ 進数位相が $\mathbf{A}$ 上の $m$ 進数位相によって誘導される $\mathbf{A} \subset B \subset \hat{\mathbf{A}}$ であるとは限りません。 ネーター (練習問題 14)。

#### 命題 12 {#ac-iii-s3-prop-12 .statement tag=04H0}

$A$ を可換ネーター 環、$m$ $A$ のイデアル、$S$ を $A$ の乗法部分集合 $1 + m$、および $E$ を有限生成された $A$ 加群とする。これら条件の下:

(i) $S^{-1}A$ は、($S^{-1}m$) 進数位相を持つザリスキー 環です。

(ii) *標準写像* $f : E \to S^{-1}E$ *は、* $E$ * に m 進数位相が与えられ、* $S^{-1}E$ * $(S^{-1}m)$ 進数位相および $\hat{f} : E \to (S^{-1}E)^{\wedge}$ * が同型である場合* は連続です。

$1 + (S^{-1}m)$ のすべての元は形になります
$$
1 + (m/(1 + m')) = (1 + m + m')/(1 + m)
$$
ここで、$m \in m$ と $m' \in m$;したがって、$S^{-1}A$ では反転可能であり、$S^{-1}m$ が $S^{-1}A$ のヤコブソン根基に含まれていることを証明します。 $S^{-1}A$ はネーター (章 II, § 2, no. 4、系 2 ～ 命題 10) であるため、$S^{-1}A$ は $(S^{-1}m)$ 進数位相を持つザリスキー 環であり、これは (i) を証明します。 (ii)を示しましょう。 $n > 0$ 全員にとって、
$$
\bar{f}^{-1}((S^{-1}m)^nE) = \bar{f}'(S^{-1}(m^nE)) = m^nE:
$$
明らかにまず第一に $f(m^nE) \subset S^{-1}m^nE$ です。逆に、$x$ を $\bar{f}^{-1}(S^{-1}m^nE)$ の元とします。次に、$(1 + m')((1 + m'')x - x'') = 0$、よって $(1 - m)x = x'$ となる $m$ と $x'' \in m^nE$ のうち元 $m', m''$ が存在します。
$$
m = -(m' + m'' + m'm'') \in m
$$
そして$x' = (1 + m')x'' \in m^nE$;私たち結論するそれ
$$
x = (1 + m + \cdots + m^{n-1})x' + m^n x \in m^nE.
$$
これは、$f$ が厳密な射であることを証明します。さらに、$sx = 0$となる$s \in S$が存在する$x \in E$の集合である$f$の核は、標準写像$j : E \to \hat{E}$の核と同一です（no. 2, 命題 5)。次に、$f = f_0 \circ j$ のようなトポロジカル同型 $f_0 : j(E) \to f(E)$ があります。 $\hat{f}$ はトポロジー 同型、問題簡約するであるため、$f(E)$ が $S^{-1}E$ で密であることを検証します。ここで、$S^{-1}E$ のすべての元は、$m \in m$ である $x/(1 - m)$ と書くことができ、すぐに次のことが検証されます。
$$
x/(1 - m) \equiv ((1 + m + \cdots + m^{n-1})x)/1 \pmod{S^{-1}m^nE}
$$
これで証明が完了します。

### 練習問題 {#ac-iii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
