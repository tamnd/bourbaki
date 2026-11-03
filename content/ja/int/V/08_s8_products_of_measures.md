---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 8
section_title: Products of measures
lang: ja
source: int-i-vi
book_pages: INT V.114-INT V.122
pdf_pages: 0334-0349, 0369-0377
extraction: ocr
subsections:
    - "no": 1
      title: Interpretation of the product measure as an integral of measures
      page: 79
      pdf_page: 334
    - "no": 2
      title: Functions measurable with respect to a product of two measures
      page: 81
      pdf_page: 336
    - "no": 3
      title: Integration of positive functions
      page: 83
      pdf_page: 338
    - "no": 4
      title: Integration of functions with values in a Banach space
      page: 87
      pdf_page: 342
    - "no": 5
      title: Operations on the product of two measures
      page: 89
      pdf_page: 344
    - "no": 6
      title: Integration with respect to a finite product of measures
      page: 91
      pdf_page: 346
    - "no": 7
      title: 'Application: Measure of the Euclidean ball in $\mathbf{R}^n$'
      page: 93
      pdf_page: 348
statements: 31
exercises: 21
content_sha256: 3d2db9a691f68f28030dcc3db9f7efbfd0b4e5f2251d22f1b55643c97dece1eb
translated_from: content/en/int/V/08_s8_products_of_measures.md
translation_method: google
source_content_sha256: 80b705b3f9f0e254836af8cc36405c37a16c85755c16c07cdd40f1fdbc7ea3e4
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 4a4f4238b6ab6b8e70c4eaf436b863862fcc5fb71569061f8f0a2ab711ec5903
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 8。対策の積

### 1. 積メジャーの積分としてのメジャーの解釈

この切断を通して、T と T' は 2 つの局所的にコンパクトな空間、$\mu$ T のポジティブなメジャー、$\mu'$ T' のポジティブなメジャー、および $\nu = \mu \otimes \mu'$ 積 $X = T \times T'$ のメジャーを表します (Ch. III, §4, No. 1)。

すべての $t \in T$、写像 $t' \mapsto (t, t')$ の T' から X への変換は連続的で適切です。この写像の下で$\lambda'_t$を$\mu'$の像とします。 $\lambda'_t$ は X の正の尺度であり、$f \in \mathscr{K}(X)$ の場合、部分写像 $t' \mapsto f(t, t')$ を $f_t$ で表すと、次のようになります。

$$
\int f \, d\lambda'_t = \int f_t \, d\mu',
$$

関係 $\lambda'_t = \varepsilon_t \otimes \mu'$ でも表されます。

さらに、写像 $t \mapsto \lambda'_t(f)$ は連続であり、コンパクトなサポート (Ch. III, §4, No. 1、補題 2) があるため、T の $\mathscr{M}(X)$ への写像 $t \mapsto \lambda'_t$ は漠然と連続しています (そして、*なおさら* は漠然と$\mu$-測定可能);従って、一連の対策 $t \mapsto \lambda'_t$ は $\mu$ で十分です ($§ 3$、No. 1、提案 2a))。メジャー $\int \lambda'_t \, d\mu(t)$ に対する $f$ の積分は、定義によって求められます。

$$
\int \langle f, \lambda'_t \rangle \, d\mu(t) = \int d\mu(t) \int f_t(t') \, d\mu'(t') = \int f(t, t') \, d\nu(t, t')
$$

(Ch. III, §4, No. 1、Th. 2);従って、$\nu = \int \lambda'_t \, d\mu(t)$。

同様に、すべての元 $t' \in T'$ について、$\lambda_{t'}$ を X への T の写像 $t \mapsto (t, t')$ の下の $\mu$ の像とします。 写像 $t' \mapsto \lambda_{t'}$ は $\mu'$ が適当で漠然と連続しており、$\nu = \int \lambda_{t'} \, d\mu'(t')$ です。次の補題が必要になります。

#### 補題 1 {#int-v-s8-lem-1 .statement tag=096Y}

*X で定義されたすべての数値写像 $f \geqslant 0$ について、*

$$
\int^* f_t \, d\mu' = \int^* f \, d\lambda'_t.
$$

$t' \mapsto (t, t')$ は連続した適切な写像であるため、これは §4, No. 2 の提案 2 から導き出されます。

#### 補題 2 {#int-v-s8-lem-2 .statement tag=096Z}

$f$ を $X$ の写像としてトポロジカル空間にします。 $f$が$\lambda'_t$測定可能であるためには、$f_t$が$\mu'$測定可能であることが必要かつ十分です。
§6, No. 2の提案3の帰結です。

#### 補題 3 {#int-v-s8-lem-3 .statement tag=0970}

$f$ を $X$ で定義された写像とし、$\overline{\mathbf{R}}$ またはバナッハ空間で値を指定します。 $f$ が $\lambda'_t$ 積分可能であるためには、 $f_t$ が $\mu'$ 積分可能であることが必要かつ十分であり、その場合、

$$
\int f_t \, d\mu' = \int f \, d\lambda'_t .
$$

これはThから続きます。 $t' \mapsto (t, t')$ が連続的で適切であるという事実を考慮した、§4, No. 4 の 2。

#### 注意 {#int-v-s8-n1-rem-1 .statement tag=0971}

補題 1,2,3 は、§§4 と 6 の結果を利用せずに、直接引数によって非常に簡単に証明できます。たとえば、$f \in \mathscr{K}(T \times T')$ であれば、関係 (2) は定義によって明らかです。 $f$ が $X = T \times T'$ の下側半連続である場合、$t' \mapsto f_t(t')$ が写像 $t' \mapsto g_t(t') = g(t, t')$ の上側エンベロープであり、$g$ が $0 \leq g \leq f$ のように$\mathscr{K}(X)$ の写像の集合を超えていることを観察するだけで十分です。最後に、任意の $f$ について、$h \geq f$ が $X$ で下位半連続である場合、$t' \mapsto h(t, t')$ は $T'$ で下位半連続であることに注意してください。逆に、$t' \mapsto u(t')$ が $T'$ で半連続的に低く、すべての $t' \in T'$ で $u(t') \geq f(t, t')$ である場合、写像 $h$ は、$t_1 \neq t'$ で$h(t, t') = u(t')$、$h(t_1, t') = +\infty$ が半連続で低くなります。 $X$ であり、$h \geq f$ を満たします。 補題 1 が証明されると、そこから集合 $(T - \{t\}) \times T'$ が $\lambda'_t$ 無視できることが推測され、補題 2 と 3 を証明するのは非常に簡単です。

関係 (3) では、混乱の危険なく、その 2 つのメンバーを $\int f(t, t') \, d\mu'(t')$ で表すことができます。同様の結果が$\lambda_{t'} = \mu \otimes \varepsilon_{t'}$ の尺度にも明らかに当てはまります。

記法の代わりに

$$
\int^* f(t, t') \, d\nu(t, t'), \quad \int^\bullet f(t, t') \, d\nu(t, t'), \quad \int f(t, t') \, d\nu(t, t'),
$$

記法を採用します

$$
\iint^* f(t, t') \, d\mu(t) \, d\mu'(t'), \quad \iint^\bullet f(t, t') \, d\mu(t) \, d\mu'(t'), \quad \iint f(t, t') \, d\mu(t) \, d\mu'(t'),
$$

第 2 章で採用された記法と一致します。 III, §4, No. 1。

測度 $\nu$ を積分 $\int \lambda'_t \, d\mu(t)$ として解釈すると、§3 の結果を積測度の言語に翻訳できるようになります。 一方、メジャー $\lambda'_t$ は $\{t\} \times T' = \overline{\mathrm{pr}}_1^{-1}(t)$ によって運ばれるため、$\nu$ のこの積分定義する分解は、$T \times T'$ の射影 $\mathrm{pr}_1$ から$T$ (§6, No. 6) に相対的にスライスされます。 前に得られた結果のリストを示します。ここに役立つ性質があります。

#### 命題 1 {#int-v-s8-prop-1 .statement tag=0972}

— $(\mu_\alpha)_{\alpha \in A}$ (それぞれ $(\mu'_\beta)_{\beta \in B}$) を、T (それぞれ T' における) のポジティブ測度の合計可能な族とし、和を $\mu$ (それぞれ $\mu'$) で表します。ファミリ $(\mu_\alpha \otimes \mu'_\beta)_{(\alpha, \beta) \in A \times B}$ は $T \times T'$ に合計可能です、そして

$$
\mu \times \mu' = \sum_{(\alpha, \beta) \in A \times B} \mu_\alpha \otimes \mu'_\beta.
$$

これらの性質は、A と B が有限である場合には明らかです。したがって、$A'$ (それぞれ $B'$) が A (それぞれ B) の有限部分集合である場合、

$$
\sum_{(\alpha, \beta) \in A' \times B'} \mu_\alpha \otimes \mu'_\beta \leq \mu \otimes \mu'.
$$

したがって、ファミリー $(\mu_\alpha \otimes \mu'_\beta)$ は合計可能です。 (4) の 2 つの要素が等しいことを示すには、2 番目の要素が積尺度 (Ch. III, §4, No. 1、Th. 1) の特性性質を満たすことを証明すれば十分であり、これは次の計算で示されます。

$f$ を $\mathscr{K}_+(T)$ の元、$\mathscr{K}_+(T')$ の $f'$ 元とします。 $f \otimes f'$ は $T \times T'$ の写像 $(t, t') \mapsto f(t)f'(t')$ を表し、属するから $\mathscr{K}_+(T \times T')$ (A、II, §7, No. 7) を表します。そして、積小節中定義により、

$$
\sum_{(\alpha, \beta) \in A \times B} \langle \mu_\alpha \otimes \mu'_\beta, f \otimes f' \rangle = \sum_{(\alpha, \beta) \in A \times B} (\langle \mu_\alpha, f \rangle \langle \mu'_\beta, f' \rangle)
= \left( \sum_{\alpha \in A} \langle \mu_\alpha, f \rangle \right) \left( \sum_{\beta \in B} \langle \mu'_\beta, f' \rangle \right)
= \langle \mu, f \rangle \langle \mu', f' \rangle
= \langle \mu \otimes \mu', f \otimes f' \rangle.
$$

### 2. 写像 2 つの尺度のうち積に関して測定可能

#### 命題 2 {#int-v-s8-prop-2 .statement tag=0973}

— $f$ を $T \times T'$ で定義された $\nu$ 可測写像とし、値をトポロジカル空間 G に置き、M を写像 $t' \mapsto f(t, t')$ が成立しないように $t \in T$ の集合とする。 $\mu'$-測定可能。

a) $f$ が $T \times T'$ の $\nu$ で緩和された部分集合の補数で一定である場合、M は $\mu$ で無視できます。

b) $\mu'$ が緩和されている場合、M は $\mu$ を無視できます。

主張 a) は、§3, No. 2 の提案 4b) および No. 1 の注意から導かれます。 b) を扱うには、$\mu'$ が有界測定値の数列 $\mu'_n$ の和であることに注意してください (§2, No. 3、提案 4)。 $f$ は $\mu \otimes \mu'_n \leq \nu$ に関して測定可能であり、集合 $M$ は$\mu'_n$ の測定値に関連付けられた集合 $M_n$ の和集合です (§ 2, No. 2、提案 2)。したがって、$\mu'$ が有界である場合に帰着され、これは § 3, No. 2 の提案 4c) から導き出されます。

この主張拡大するは、直ちに複雑な措置に適用されます (Ch. III, § 4, No. 2、提案 3)。

#### 系 {#int-v-s8-n2-cor-1 .statement tag=0974}

— *A を $T \times T'$ の $\nu$ 可測の部分集合とし、M を $t \in T$ の集合とし、t における A の切断 $A(t)$ は $\mu'$ 可測ではないようにします。*

a) *A が $\nu$ 程度である場合、M は $\mu$ 無視可能です。*

b) *$T'$ 上の A の射影が $\mu'$ で緩和されている場合、M は局所的には $\mu$ 無視可能です。*

主張 a) は提案 2 の直後に続きます。b) を確立するには、$T'$ の $\mu'$ 可積分開集合の数列の B 集合、和集合で、A の含む射影を表します。 $T'$、$\mu'_1$ は緩和措置 $\varphi_B \cdot \mu'$ を示します。 A は $\mu \otimes \mu'_1 \leq \mu \otimes \mu'$ に関して可測であるため、提案 2 は、局所的に $\mu$ 無視できる集合を形成する $t$ を除いて、$A(t)$ が $\mu'_1$ 可測であることを意味します。しかし、$A(t) \subset B$ 以降、$A(t)$ が $\mu'_1$ 可測であると言うのは、$A(t)$ が $\mu'$ 可測であるというというと同等です (§ 5, No. 3、提案 4 の裏付け)。

#### 命題 3 {#int-v-s8-prop-3 .statement tag=0975}

— *f を T の写像をトポロジカル空間 F にするとします。 f が $\mu$ 可測であれば、 写像 $(t, t') \mapsto f(t)$ は $\nu$ 可測です。逆に、$\mu' \neq 0$ で、この写像が $\nu$ 可測であれば、写像 f は $\mu$ 可測です。*

最初の主張は Cor から続きます。 § 6, No. 6 の提案 10 の 1。 $\mu' \neq 0$ が、$\mu'_1$ 非零メジャーで表され、その上が $\mu'$、$\nu_1$ メジャー $\mu \otimes \mu'_1$、および集合 $a = \| \mu'_1 \|$ によって境界付けられるコンパクトなサポートを持つメジャーであるとします。 The projection $\mathrm{pr}_1$ of $T \times T'$ onto T is then $\nu_1$-proper, and the image measure $\mathrm{pr}_1(\nu_1)$ is equal to $a \mu$ (§ 6, No. 6, Prop. 10). $(t, t') \mapsto f(t)$ が $\nu$ 測定可能である場合、$\nu_1$ も測定可能であるため、$f$ は$a \mu$ (§ 6, No. 2、提案 3)、$a \neq 0$ 以降の結果よってに関して測定可能です。

前述の主張拡大するは、次の帰結と同様に、すぐに複雑な措置に適用されます (Ch. III, § 4, No. 2、提案 3)。

#### 系 1 {#int-v-s8-prop-3-cor-1 .statement tag=0976}

— *F、F'、G を 3 つのトポロジー 空間とし、u を G への $F \times F'$ の連続写像とする。 f (それぞれ $f'$) を T (それぞれ $T'$) で定義された写像とし、F (それぞれ $F'$) には値を定義し、 $\mu$ (それぞれ $\mu'$) について測定可能です。その場合、写像 $(t, t') \mapsto u(f(t), f'(t'))$ は $\mu \otimes \mu'$ に対して測定可能です。*

写像 $(t, t') \mapsto f(t)$、$(t, t') \mapsto f'(t')$ は$\nu$ であり、提案 3 によって測定可能であるため、これは Th から導き出されます。 1章IV, § 5, No. 3。

#### 系 2 {#int-v-s8-prop-3-cor-2 .statement tag=0977}

— *$A \subset T$ と $A' \subset T'$ が (それぞれ $\mu$ と $\mu'$ について) 測定可能である場合、$A \times A'$ は $\mu \otimes \mu'$ について測定可能です。
これはコルからすぐに続きます。 1.

#### 系 3 {#int-v-s8-prop-3-cor-3 .statement tag=0978}

— *2 つの正の数値 (それぞれ複素数値) $T$ で定義された写像 $f$ と $T'$ で定義された $f'$ を考えます。これらの写像がそれぞれ $\mu$ と $\mu'$ で測定可能である場合、写像*

$$
f \otimes f' : (t, t') \mapsto f(t)f'(t')
$$

*$\mu \otimes \mu'$まで測定可能です。*

複素数写像または有限実数写像の場合は、Cor の明らか帰結です。 1. 正の数値写像の場合を扱うには、整数 $n \geqslant 0$ ごとに集合 $f_n = \inf(f, n)$、$f'_n = \inf(f', n)$ を計算し、結果は (通常の規則 $0 \cdot (+\infty) = 0$ を使用して) $f \otimes f' = \sup_n (f_n \otimes f'_n)$、よってになります。

#### 命題 4 {#int-v-s8-prop-4 .statement tag=0979}

— *$A$を$T$の部分集合とします。 $A$ が局所的に $\mu$ 無視できる場合、$A \times T'$ は局所的に $\nu$ 無視可能です。逆に、$A \times T'$ が局所的に $\nu$ で無視できる場合、および $\mu' \neq 0$ の場合、$A$ は局所的に $\mu$ で無視可能です。*

最初の主張は Cor から続きます。 §6, No. 6の提案10の1。 2 番目の主張を確立するために、提案 3 の証明の記法をもう一度取り上げましょう。 $A \times T' = \mathrm{pr}_1^{-1}(A)$ は測度 $\nu_1$ に対して局所的に無視できるため、$A$ は $a\mu$ (§ 6, No. 2、提案 2 の補正)、$a \neq 0$ 以降の結果よってに対して局所的に無視できます。

前の主張拡大するは、次の系と同様に、2 つの複雑な措置 (Ch. III, §4, No. 2、提案 3) の積に一度に適用されます。

#### 系 {#int-v-s8-n2-cor-2 .statement tag=097A}

— *メジャー $\mu$ (それぞれ $\mu'$) が $M$ (それぞれ $M'$) に集中している場合、$\mu \otimes \mu'$ は $M \times M'$ に集中しています。*

なぜなら、$(T \times T') - (M \times M')$ は集合 $(T - M) \times T'$ と $T \times (T' - M')$ の和集合であり、提案 4 により、$\mu \times \mu'$ は局所的に無視できます。

### 3. ポジティブ写像の統合

定義する積 $0 \cdot (+\infty)$ が 0 に等しいことに同意したことを思い出してください。この規則には特に次の帰結があります: $f$ が正の尺度を備えた局所的にコンパクトな空間で定義された数値写像 $\geqslant 0$ である場合$\lambda$、次に、$0 \leqslant a \leqslant +\infty$ となるすべての定数 $a$ に対して $\lambda^*(af) = a \cdot \lambda^*(f)$ です。 $a = 0$ の場合、これは明らかです。 $a = +\infty$ の場合、$f$ が $\lambda$ 無視できるかどうかに応じて、$\lambda^*(af) = a \cdot \lambda^*(f) = 0$ または $\lambda^*(af) = a \cdot \lambda^*(f) = +\infty$ になります。最後に、$0 < a < +\infty$ であれば、$\lambda^*(af) = a \cdot \lambda^*(f)$ であることが分かります。

#### 命題 5 {#int-v-s8-prop-5 .statement tag=097B}

— $f$ を数値写像 $\geqslant 0$ とし、$T \times T'$ の下側半連続とします。それでは、写像

$$
t \mapsto \int^* f(t, t') \, d\mu'(t')
$$

$T$ では下位の半連続であり、

$$
\iint^* f(t, t') \, d\mu(t) \, d\mu'(t') = \int^* d\mu(t) \int^* f(t, t') \, d\mu'(t').
$$

これは、No. 1の補題1を考慮した、§3, No. 1の提案2の帰結です。

#### 系 1 {#int-v-s8-prop-5-cor-1 .statement tag=097C}

— $f$ (それぞれ $f'$) を、$T$ (それぞれ $T'$) で定義された下位の半連続写像 $\geqslant 0$ とします。 写像 $f \otimes f' : (t, t') \mapsto f(t)f'(t')$ はその後、$T \times T'$ で半連続的に下落し、

$$
\iint^* f(t)f'(t') \, d\mu(t) \, d\mu'(t') = \left( \int^* f(t) \, d\mu(t) \right) \left( \int^* f'(t') \, d\mu'(t') \right).
$$

$G$ (それぞれ $G'$) を写像 $g \in \mathscr{K}_+(T)$ (それぞれ $g' \in \mathscr{K}_+(T')$) の集合として、$g \leqslant f$ (それぞれ $g' \leqslant f'$) とします。それから

$$
f \otimes f' = \sup_{g \in G,\ g' \in G'} g \otimes g'.
$$

写像 $g \otimes g'$ 属するから $\mathscr{K}_+(T \times T')$ なので、$f \otimes f'$ は確かに下位の半連続であり、(6) は提案 5 からすぐに続きます (または、前の公式の極限への移行によって直接)。

#### 系 2 {#int-v-s8-prop-5-cor-2 .statement tag=097D}

— Let $A$ be a $\mu$-moderated 部分集合 of $T$, and $A'$ a $\mu'$-moderated 部分集合 of $T'$;その場合、$A \times A'$ は $T \times T'$ で $\nu$ が緩和されます。

緩和された集合 (§1, No. 2、提案 5) の定義を考慮すると、$B$ が $T$ の積分可能なオープン集合であり、$B'$ が集合の積分可能なオープン集合である場合を示すだけで十分です。 $T'$, then the open 集合 $B \times B'$ is integrable.これはコルからすぐに続きます。 1.

#### 系 3 {#int-v-s8-prop-5-cor-3 .statement tag=097E}

— Let $A$ be a $\mu$-negligible 部分集合 of $T$, and let $B'$ be a $\mu'$-moderated 部分集合 of $T'$;その場合、$A \times B'$ は $\nu$ で無視できます。

なぜなら、$A \times B'$ は局所的には $\nu$ 無視できる (提案 4) し、$\nu$ は緩和される (修正 2) ため、$\nu$ は無視できる (§1, No. 2、提案 7 の修正 1)。

コルス。 2 and 3 may be extended to 積 of two complex measures, on 適用主張 to their absolute 値 (Ch. III, §4, No. 2, Prop. 3).

#### 命題 6 {#int-v-s8-prop-6 .statement tag=097F}

— Let $f$ be a numerical 写像 $\geqslant 0$ defined on $T \times T'$.それから

$$
\iint^* f(t, t') d\mu(t) d\mu'(t') \geqslant \int^* d\mu(t) \int^* f(t, t') d\mu'(t').
$$

This follows from Prop. 3 of §3, No. 2, on taking (2) into account.

#### 命題 7 {#int-v-s8-prop-7 .statement tag=097G}

— Let $f$ be a $\nu$-measurable positive numerical 写像 defined on $T \times T'$.

a) *$f$ が $\nu$ で調整されている場合、写像* $t \mapsto \int^* f(t, t') d\mu'(t')$、$t' \mapsto \int^* f(t, t') d\mu(t)$ * はそれぞれ $\mu$ と $\mu'$ について測定可能で調整され、*

$$
\iint^* f(t, t') d\mu(t) d\mu'(t') = \int^* d\mu(t) \int^* f(t, t') d\mu'(t')
$$
(7)
$$
= \int^* d\mu'(t') \int^* f(t, t') d\mu(t).
$$

b) *If the measure $\mu'$ is moderated, then 写像* $t \mapsto \int^* f(t, t') d\mu'(t')$ *is $\mu$-measurable, and*

$$
\iint^* f(t, t') d\mu(t) d\mu'(t') = \int^* d\mu(t) \int^* f(t, t') d\mu'(t').
$$
(8)

主張 a), as well as 主張 b) when $\mu'$ is bounded, are 帰結 of Prop. 5 of §3, No. 2. $\mu'$ が緩和されている場合を扱うために、$\mu'$ を有界措置の数列の和 $\sum_{n \in \mathbf{N}} \mu'_n$ として表します (§ 2, No. 3、提案 4)。 写像 $t \mapsto \int^* f(t, t') d\mu'_n(t')$ is then $\mu$-measurable, and
$$
\iint^* f(t, t') d\mu(t) d\mu'_n(t') = \int^* d\mu(t) \int^* f(t, t') d\mu'_n(t').
$$
しかし、$\mu \otimes \mu' = \sum_{n \in \mathbf{N}} (\mu \otimes \mu'_n)$ (提案 1); 主張 b) is then obtained by summing on $n$ (§ 2, No. 2, Prop. 1).

#### 系 1 {#int-v-s8-prop-7-cor-1 .statement tag=097H}

— Let $H$ be a subset of $T \times T'$, and let $A$ be the set of $t \in T$ such that the section $H(t)$ of $H$ at $t$ is not $\mu'$-negligible.

a) *$H$ が $\nu$ で無視できる場合、$A$ は $\mu$ で無視可能です。*

b) *$H$ が局所的に $\nu$ 無視可能で、$\mu'$ が中程度である場合、$A$ は局所的に $\mu$ 無視可能です。*

性質 a) は提案 7 (または提案 6) からすぐに続きます。 b) の仮説の下では、$H(t)$ が局所的に μ’ 無視できる、または μ’ が緩和されているため μ’ 無視できると言うのは同じことになります (§1, No. 2、提案 7)。したがって、性質 b) は公式 (8) から導かれます。

この系拡大するは、絶対的な値への移行によって、2 つの複雑な尺度の積に至ります。以下の系も同様です。

#### 系 2 {#int-v-s8-prop-7-cor-2 .statement tag=097I}

— *集合* $A \subset T \times T'$ *が ν 積分可能である場合、 切断* $A(t)$ *of* $A$ *at* $t$ *ほぼすべて* $t \in T$、*写像* $t \mapsto \mu'(A(t))$ *はμ積分可能、および*

$$
\nu(A) = \int \mu'(A(t))\, d\mu(t).
$$

#### 命題 8 {#int-v-s8-prop-8 .statement tag=097J}

— *For every pair of numerical functions* $f \geq 0$, $f' \geq 0$ *defined on* $T$ *and* $T'$, *respectively,

$$
\iint^\bullet f(t)f'(t')\, d\mu(t)\, d\mu'(t') = \left( \int^\bullet f(t)\, d\mu(t) \right) \left( \int^\bullet f'(t')\, d\mu'(t') \right).
$$

まず、$\mu$ と $\mu'$ が *コンパクトなサポート* を備えたメジャーである場合を扱います。同じことが$\mu \otimes \mu'$にも当てはまり、すべての記号$\int^\bullet$、$\iint^\bullet$は上位積分に置き換えることができます。提案 6 により、

$$
\iint^* f(t)f'(t')\, d\mu(t)\, d\mu'(t') \geq \int^* d\mu(t) \int^* f(t)f'(t')\, d\mu'(t')
$$
$$
= \left( \int^* f(t)\, d\mu(t) \right) \left( \int^* f'(t')\, d\mu'(t') \right).
$$

逆の不等式を確立するには、下の半連続写像の下側エンベロープ数列 $(h_n)$ (それぞれ $(h'_n)$) である選ぶ写像 $h \geq f$ (それぞれ $h' \geq f'$) を考えてみましょう。

$$
\int^* h(t)\, d\mu(t) = \int^* f(t)\, d\mu(t)
$$

(それぞれ $\int^* h'(t')\, d\mu'(t') = \int^* f'(t')\, d\mu'(t')$);このような写像の存在は、上部積分の定義の直後に続きます (Ch. IV, §1, No. 3、デフォルト。 3）とルベーグの定理。 適用提案 7 を測定可能な写像 $h \otimes h'$ に当てはめると、次のようになります。

$$
\iint^* f(t)f'(t')\, d\mu(t)\, d\mu'(t') \leq \iint^* h(t)h'(t')\, d\mu(t)\, d\mu'(t')
$$
$$
= \left( \int^* h(t)\, d\mu(t) \right) \left( \int^* h'(t')\, d\mu'(t') \right)
$$
$$
= \left( \int^* f(t)\, d\mu(t) \right) \left( \int^* f'(t')\, d\mu'(t') \right),
$$

それが求められている不等式です。したがって、$\mu$と$\mu'$がコンパクトなサポートを持つメジャーである場合、命題が確立されます。一般的なケースを扱うには、$\mu$ (それぞれ $\mu'$) を、コンパクトなサポート (§ 2, No. 3、提案 4) を備えたメジャーの族 $(\mu_\alpha)_{\alpha \in A}$ (それぞれ $(\mu'_\beta)_{\beta \in B}$) の和として表し、各メジャー $\mu_\alpha \otimes \mu'_\beta$ に対して公式 (10) を記述するだけで十分です。提案 1 (§ 2, No. 2、提案 1) を考慮して、$(\alpha, \beta)$ に和を適用します。

#### 系 1 {#int-v-s8-prop-8-cor-1 .statement tag=097K}

*提案 8 のように記法を使用すると、

$$
\iint^* f(t)f'(t')\,d\mu(t)\,d\mu'(t') = \left( \int^* f(t)\,d\mu(t) \right) \left( \int^* f'(t')\,d\mu'(t') \right)
$$

ただし、2 番目のメンバーの因子の 1 つが 0 に等しく、もう 1 つが $+\infty$ に等しい場合は除きます。

2 番目のメンバーの 2 つの因子が有限である場合、写像 $f$ と $f'$ は緩和されます (§ 1, No. 2、提案 7)。したがって、写像 $f \otimes f'$ は緩和されます (提案 5 の Cor. 2)。上記の等式したがって、簡約するから公式 (10) (§ 1, No. 2、提案 7)。 2 番目のメンバーの因子の 1 つが値 $+\infty$ を持ち、もう 1 つが零ではない場合、2 番目のメンバーは値 $+\infty$ を持ち、上記の等式は提案 6 から導き出されます。

#### 系 2 {#int-v-s8-prop-8-cor-2 .statement tag=097L}

*$f$と$f'$を、$\mathbf{C}$または$\overline{\mathbf{R}}$に値を含む2つの写像とし、それぞれ$T$と$T'$で定義し、$\mu$と$\mu'$の尺度に対して本質的に積分可能（それぞれ積分可能）であるとします。それぞれ。 写像 $f \otimes f'$ は、測度 $\mu \otimes \mu'$ に対して本質的に積分可能 (それぞれ可積分) であり、*

$$
\iint f(t)f'(t')\,d\mu(t)\,d\mu'(t') = \left( \int f(t)\,d\mu(t) \right) \left( \int f'(t')\,d\mu'(t') \right).
$$

$f$ と $f'$ が正の場合、$f \otimes f'$ は Cor によって測定可能です。 主張は、公式 (10) (それぞれ (11)) および本質的な積分可能性の基準 (§ 1, No. 3、提案 9) (それぞれ、第 3 章の積分可能性基準) から続きます。 IV, § 5, No. 6、木。 5)。 一般的なケースがすぐに続きます。

系 2 拡大するを 2 つの複雑なメジャーの積に同時に実行します。

### 4. Banach 空間における写像と値の統合

#### 定理 1 (ルベーグ–フビニ) {#int-v-s8-thm-1 .statement tag=097M}

— *$f$ を $T \times T'$ で定義された写像とし、Banach 空間 $F$ または $\overline{\mathbf{R}}$ で値を定義します。 $N$ を $t \in T$ の集合として、写像 $t' \mapsto f(t,t')$ が $\mu'$ 積分可能ではないようにします。

a) $f$ が $\nu$ 可積分であると仮定します。この場合、$N$ は $\mu$ 無視可能、写像 $t \mapsto \int f(t,t')\,d\mu'(t')$ ($t \notin N$ に対して定義) は $\mu$ 積分可能、および*

$$
\iint f(t,t')\,d\mu(t)\,d\mu'(t') = \int d\mu(t) \int f(t,t')\,d\mu'(t').
$$

b) *$f$ は本質的に $\nu$ 可積分であり、尺度 $\mu'$ は緩和されていると仮定します。この場合、$N$ は局所的に $\mu$ 無視可能であり、写像 $t \mapsto \int f(t, t')\, d\mu'(t')$ ($t \notin N$ に対して定義) は本質的に $\mu$ 積分可能であり、(13) が成り立ちます。

主張 a) Th からすぐに続きます。 §3, No. 3 の 1 つ。 b) を確立するために、ほぼどこでも局所的に $f$ に等しい $\nu$ 可積分関数を $g$ で表し、$f(t, t') \neq g(t, t')$ となるような $(t, t')$ の集合を$H$ で表します。コル著提案 7 の 1、切断 $H(t)$ は、局所的に $\mu$ 無視できる集合を形成する $t \in T$ を除いて、$\mu'$ は無視できます。 $f$ に関する結果は、主張 a) を $g$ に適用することで推定できます。

#### スクリウム {#int-v-s8-n4-sch-1 .statement tag=097N}

— *$f$ を $T \times T'$ で定義された写像とし、$\overline{\mathbf{R}}$ またはバナハ空間で値を定義します。つまり、$\nu$ 測定可能で $\nu$ 緩和されます。 3 つの積分の場合*

$$
\iint f(t, t')\, d\mu(t)\, d\mu'(t'), \quad \int d\mu(t) \int f(t, t')\, d\mu'(t'), \quad \int d\mu'(t') \int f(t, t')\, d\mu(t)
$$

*存在し、平等であるためには、2 つの数* のうちの 1 つが必要かつ十分です。

$$
\int^* d\mu(t) \int^* |f(t, t')|\, d\mu'(t'), \quad \int^* d\mu'(t') \int^* |f(t, t')|\, d\mu(t)
$$

*有限であること*

こちらはThの明らか帰結です。 1、提案 7 および積分可能性基準 (Ch. IV, §5, No. 6、Th. 5)。

#### 注意 {#int-v-s8-n4-rem-1 .statement tag=097O}

— 1) 尺度 $\mu'$ が緩和されていない場合、$t \in T$ のどの値についても、$f$ は本質的に $\nu$ 積分可能であり、写像 $t' \mapsto f(t, t')$ は本質的に $\mu'$ 積分可能ではないことが起こります (§3、Exer. 4)。

2) $\mu$ と $\mu'$ を 2 つの複素測度とし、$\nu = \mu \otimes \mu'$ とします。 $f$ が $\nu$ 可積分である場合 (他の語、$|\nu|$ 可積分可能)、定理を$|\mu|$ と $|\mu'|$ に適用し、その積は $|\nu|$ になります (Ch. III, §4, No. 2、Prop. 3) は、$t' \mapsto f(t, t')$ が $\mu$ に対してほぼすべての $t$ に対して $\mu'$ 積分可能であることを意味します。このことから、対策$\mu$と$\mu'$を積極的対策の線形結合として分解すると、a)拡大するの主張が複雑な対策となることが推測されます。 b)についても同様に議論できます。

#### 命題 9 {#int-v-s8-prop-9 .statement tag=097P}

*$F$、$F'$、$G$を3つのバナハ空間とし、$(x, y) \mapsto [x \cdot y]$を$F \times F'$から$G$への連続双線形写像とする。 $f$ (それぞれ $f'$) を $T$ (それぞれ $T'$) で定義された写像と、$F$ (それぞれ $F'$) の値が定義され、本質的に $\mu$ (それぞれ $\mu'$) に対して積分可能であるとします。 $g$ を写像 $(t, t') \mapsto [f(t) \cdot f'(t')]$ とします。その場合、$g$ は本質的に $\mu \otimes \mu'$ に対して積分可能であり、*

$$
\iint [f(t) \cdot f'(t')] \, d\mu(t)\, d\mu'(t') = \left[ \left( \int f\, d\mu(t) \right) \cdot \left( \int f'(t')\, d\mu'(t') \right) \right].
$$

*さらに、$f$ と $f'$ が可積分であれば、 $g$ も可積分です。

写像 $(t, t') \mapsto [\mathbf{f}(t) \cdot \mathbf{f}'(t')]$ は、Cor によって $(\mu \otimes \mu')$ で測定可能です。提案 3 の 1. 一方、$b$ が双線形写像 $(\mathbf{x}, \mathbf{y}) \mapsto [\mathbf{x} \cdot \mathbf{y}]$ のノルムを表す場合、

$$
\iint^\bullet |[\mathbf{f}(t) \cdot \mathbf{f}'(t')]| d\mu(t) d\mu'(t') \leq b \iint^\bullet |\mathbf{f}(t)| \cdot |\mathbf{f}'(t')| d\mu(t) d\mu'(t')
$$
$$
= b \left( \int^\bullet |\mathbf{f}(t)| d\mu(t) \right) \left( \int^\bullet |\mathbf{f}'(t')| d\mu'(t') \right)
$$

これは、$[\mathbf{f}(t) \cdot \mathbf{f}'(t')]$ が $\mu \otimes \mu'$ に対して本質的に可積分であることを示しています (§ 1, No. 3、提案 9)。 $\mathbf{f}$ と $\mathbf{f}'$ が可積分であると仮定します。その場合、$\mathbf{f}$ と $\mathbf{f}'$ は緩和され、$\mathbf{g}$ は緩和され (提案 5 の正解 2)、したがって可積分です (§ 1, No. 3、提案 9 の正解)。この場合、公式 (14) は、ルベーグ・フビニ定理と積分の線形性 (Ch. IV, § 4, No. 2、Th. 1) から得られます。 $\mathbf{f}$ と $\mathbf{f}'$ が本質的に可積分である場合の処理を完了するには、(14) を 2 つの可積分関数 $\mathbf{f}_1$ と $\mathbf{f}_1'$ に適用します。これは局所的にほぼどこでも $\mathbf{f}$ と $\mathbf{f}'$ に等しく、観察するとでは局所的にほぼどこでも $[\mathbf{f} \cdot \mathbf{f}'] = [\mathbf{f}_1 \cdot \mathbf{f}_1']$ に等しくなります。 $T \times T'$ (提案 4)。

この結果、拡大するから積までの複雑な対策が行われます。

### 5. 2 小節の積の演算

#### 命題 10 {#int-v-s8-prop-10 .statement tag=097Q}

— $g$ (それぞれ $g'$) を、$T$ (それぞれ $T'$) で定義された複素数写像 (または $\overline{\mathbf{R}}$ に値を含む写像) とします。
a) $g$ (それぞれ $g'$) が $\mu$ (それぞれ $\mu'$) に対してローカルに積分可能である場合、写像 $g \otimes g': (t, t') \mapsto g(t)g'(t')$ は $\nu = \mu \otimes \mu'$ に対してローカルに積分可能であり、

$$
(g \cdot \mu) \otimes (g' \cdot \mu') = (g \otimes g') \cdot (\mu \otimes \mu').
$$

b) 逆に、$g \otimes g'$ が局所的に $\nu$ 積分可能であり、$g'$ が局所的に $\mu'$ 無視できない場合、$g$ は局所的に $\mu$ 積分可能です。

a) $K$ と $K'$ を、それぞれ $T$ と $T'$ の 2 つのコンパクト部分集合とします。コル。提案 8 の 2 は、$(g\varphi_K) \otimes (g'\varphi_{K'})$ に等しい写像 $(t, t') \mapsto g(t)g'(t')\varphi_{K \times K'}(t, t')$ が $\nu$ 可積分であることを示しています。従って、$g \otimes g'$ は局所的に $\nu$ 積分可能です。次に、(15) の 2 番目のメンバーが積尺度の特性性質を満たすことを直ちに検証します (Ch. III, § 4, No. 1、Th. 1)。

b) ここで、$g \otimes g'$ が局所的に $\nu$ 可積分であり、$g'$ が局所的に $\mu'$ 無視できないと仮定します。 $\mu_1$ を、$\mu_1 \leq \mu$ のようなコンパクトなサポートを備えた積極的な手段とします。 $g \otimes g'$ は $(\mu_1 \otimes \mu')$ 測定可能であるため、$t \mapsto g(t)g'(t')$ は、$t'$ の値のうち無視できる局所的な $\mu'$ 集合を除いて $\mu_1$ 測定可能です。

$g'$ は局所的に $\mu'$ ではなく、ほぼどこでも零であるため、これから、$g$ は $\mu_1$ で測定可能であり、その後、$\mu$ をコンパクトなサポートを備えた一連のメジャーの和に分解すると、$\mu$ は測定可能であると推測されます。 (§ 2, No. 3、提案4および§ 2, No. 2、提案2)。この点を確立した後、必要に応じて、$g$ と $g'$ が $\geqslant 0$ である場合、置き換えること $g$ と $g'$ を絶対値によって簡約するすることができます。 $K$ を $T$ の任意のコンパクト部分集合とし、$K'$ を $\int g' \varphi_{K'} d\mu' \neq 0$ となるような $T'$ のコンパクト部分集合とします。提案 8 により、

$$
\left( \int^\bullet g \varphi_K d\mu \right) \left( \int^\bullet g' \varphi_{K'} d\mu' \right) = \iiint^\bullet (g \otimes g') \varphi_{K \times K'} d\mu d\mu' < +\infty .
$$

したがって、最初のメンバーの最初の因子は有限であり、これで証明が完成します。

This proposition extends to complex measures, thanks to Prop. 3 of Ch. III, § 4, No. 2。

#### 命題 11 {#int-v-s8-prop-11 .statement tag=097R}

*$\pi$ (それぞれ $\pi'$) を $T$ (それぞれ $T'$) の写像を局所的にコンパクトな空間 $T_1$ (それぞれ $T'_1$) にします。*

a) *$\pi$ (それぞれ $\pi'$) が $\mu$-適切 (それぞれ $\mu'$-適切) である場合、写像 $\pi \times \pi'$ は $(\mu \otimes \mu')$-適切および $(\pi \times \pi')(\mu \otimes \mu') = \pi(\mu) \otimes \pi'(\mu')$ です。*

b) *逆に、$\pi \times \pi'$ が $(\mu \otimes \mu')$-proper および $\mu' \neq 0$ である場合、$\pi$ は $\mu$-proper です。*

a) なぜなら、$\pi \times \pi'$ は Cor によって$(\mu \times \mu')$ 測定可能です。 No. 2の提案3の1。一方、$K$ (それぞれ $K'$) が $T_1$ (それぞれ $T'_1$) のコンパクト部分集合である場合、$\pi^{-1}(K)$ と ${\pi'}^{-1}(K')$ はそれぞれ $\mu$ と $\mu'$ に対して本質的に積分可能であるため、$\pi^{-1}(K) \times {\pi'}^{-1}(K')$は本質的に $\mu \otimes \mu'$ に対して可積分です (提案 8 の Cor. 2)。これは、$\pi \times \pi'$ が $(\mu \times \mu')$ として正しいことを証明します。次に、$\mu_1 = \pi(\mu)$、$\mu'_1 = \pi'(\mu')$、$\nu_1 = (\pi \times \pi')(\mu \otimes \mu')$ とします。 $f \in \mathscr{K}(T_1)$ と $f' \in \mathscr{K}(T'_1)$ については、

$$
\iint f(\pi(t)) f'(\pi'(t')) d\mu(t) d\mu'(t')
$$
$$
= \left( \int f(\pi(t)) d\mu(t) \right) \left( \int f'(\pi'(t')) d\mu'(t') \right)
$$

(提案 8 の Cor. 2)、これは $\nu_1 = \mu_1 \otimes \mu'_1$ (Ch. III, § 4, No. 1、Th. 1) を証明します。

b) ここで、$\pi \times \pi'$ が $\mu \otimes \mu'$-proper であり、$\mu' \neq 0$ であると仮定します。 $\mu_1$ をコンパクトなサポートのメジャー $\leq \mu$ とします。 写像 $\pi \times \pi'$ は $\mu_1 \otimes \mu'$ について測定可能であり、写像 $t \mapsto (\pi(t), \pi'(t'))$ は、局所的に $\mu'$ 無視できる集合を形成する $t'$ を除き、$\mu$ が測定可能です (No. 2、提案 2)。 $\mu' \neq 0$ なので、$\pi$ は $\mu_1$ 可測であり、最後に $\pi$ は $\mu$ 可測であるということになります。

(§2, No. 3、提案4および§2, No. 2、提案2)。 写像 $f \in \mathscr{K}_+(\mathrm{T}_1)$ ごとに $\mu^\bullet(f \circ \pi) < +\infty$ であることを示す必要があります。 $\mu$が零なら、この性質は明らかです。 $\mu$ が零でない場合、$\mu \otimes \mu'$ も$(\pi \times \pi')(\mu \otimes \mu') \neq 0$ となります (§6, No. 2、提案 2 の訂正 1)。 補題 1 章までIII, §4, No. 1、写像 $g \in \mathscr{K}_+(\mathrm{T}_1)$、$g' \in \mathscr{K}_+(\mathrm{T}'_1)$ は次のように 2 つ存在します。

$$
\langle (\pi \times \pi')(\mu \otimes \mu'), g \otimes g' \rangle \neq 0.
$$

この式は、像メジャーの定義によって $\langle \mu \otimes \mu', (g \circ \pi) \otimes (g' \circ \pi') \rangle$ に等しいため、提案 8 は ${\mu''}^\bullet(g' \circ \pi') \neq 0$ を意味します。次に、提案 8 と §6, No. 2 の提案 2 により、

$$
\left( \int^\bullet (f \circ \pi) d\mu \right) \left( \int^\bullet (g' \circ \pi') d\mu' \right) = \iint^\bullet (f \circ \pi) \otimes (g' \circ \pi') d\mu d\mu'
$$
$$
= \iint^\bullet (f \otimes g') d((\pi \times \pi')(\mu \otimes \mu')) < +\infty.
$$

従って、最初の要素の最初の積分は有限であり、証明が完成します。

この結果は、2 つの複雑な測定値の積に一度に拡大するを与えます (絶対値値に主張を適用します)。以下命題も同様です。

#### 命題 12 {#int-v-s8-prop-12 .statement tag=097S}

— X (それぞれ X') を T (それぞれ T') の局所的にコンパクトな部分空間とします。次に、$T \times T'$ の局所的にコンパクトな部分空間 $X \times X'$ で誘導された測度 $(\mu \otimes \mu')_{X \times X'}$ は、それぞれ $\mu$ と $\mu'$ によって X と X' に誘導された測度の積 $\mu_X \otimes \mu'_{X'}$ に等しくなります。

$f \in \mathscr{K}(X)$ と $f' \in \mathscr{K}(X')$ の場合、

$$
\iint_{X \times X'} f(t)f'(t') d\mu(t) d\mu'(t') = \left( \int_X f(t) d\mu(t) \right) \left( \int_{X'} f'(t') d\mu'(t') \right)
$$

コル著提案 8 の 2 は、誘導措置 (Ch. IV, §5, No. 7) の定義によって次のことを証明します。

$$
(\mu \otimes \mu')_{X \times X'} = \mu_X \otimes \mu'_{X'}
$$

(Ch. III, §4, No. 1、Th. 1)。

### 6. 有限な積の尺度に関する積分

前述の結果は、有限の数の尺度のうち積まで問題なく拡張できます。たとえば、$T_1, T_2, T_3$ を 3 つの局所的にコンパクトな空間、$\mu_i$ を $T_i$ ($i = 1, 2, 3$) の正の測度とし、ν = μ₁ ⊗ μ₂ ⊗ μ₃ を T = T₁ × T₂ × T₃ における積の測度とする。 f を $\overline{\mathbf{R}}$ の値または Banach 空間の ν 可積分関数としましょう。ルベーグ・フビニ定理の最初の適用は、無視できる集合 ($\mu_1 \otimes \mu_2$ の場合) を形成する点 $(t_1, t_2) \in T_1 \times T_2$ を除いて、写像 $t_3 \mapsto f(t_1, t_2, t_3)$ は $\mu_3$ 可積分であり、写像であることを示します。

$$
(t_1, t_2) \mapsto \int f(t_1, t_2, t_3) \, d\mu_3(t_3),
$$

$T_1 \times T_2$ のほぼどこでも定義されており、$(\mu_1 \otimes \mu_2)$ 積分可能であり、

$$
\iiint f(t_1, t_2, t_3) \, d\nu(t_1, t_2, t_3) = \iint d\mu_1(t_1) \, d\mu_2(t_2) \int f(t_1, t_2, t_3) \, d\mu_3(t_3).
$$

同じ定理の 2 番目の適用は、ほぼすべての $t_1 \in T_1$ について、写像 $t_2 \mapsto \int f(t_1, t_2, t_3) \, d\mu_3(t_3)$ が $T_2$ のほぼどこでも定義されており、$\mu_2$ 積分可能であることを示しています。さらに、写像

$$
t_1 \mapsto \int d\mu_2(t_2) \int f(t_1, t_2, t_3) \, d\mu_3(t_3),
$$

$T_1$ のほぼどこでも定義されており、$\mu_1$ 積分可能であり、

$$
\iiint f(t_1, t_2, t_3) \, d\nu(t_1, t_2, t_3) = \int d\mu_1(t_1) \int d\mu_2(t_2) \int f(t_1, t_2, t_3) \, d\mu_3(t_3).
$$

ほぼすべての $t_1 \in T_1$、写像 $(t_2, t_3) \mapsto f(t_1, t_2, t_3)$ は $(\mu_2 \otimes \mu_3)$ 可積分であり、写像も同様に証明されます。

$$
t_1 \mapsto \iint f(t_1, t_2, t_3) \, d\mu_2(t_2) \, d\mu_3(t_3),
$$

ほぼどこでも定義されており、$\mu_1$-積分可能であり、

$$
\iiint f(t_1, t_2, t_3) \, d\nu(t_1, t_2, t_3) = \int d\mu_1(t_1) \iint f(t_1, t_2, t_3) \, d\mu_2(t_2) \, d\mu_3(t_3).
$$

2 つの尺度の積について上記で証明された他の結果と同じ方法で一般化する作業は読者に任せます。

### 7. 用途: $\mathbf{R}^n$ のユークリッドボールの測定

$\mu$ を $\mathbf{R}$ のルベーグ測度、$\mu_n$ $\mathbf{R}^n$ のルベーグ測度、$n$ 因子の積が $\mu$ に等しいとします。 ユークリッド単位元ボールの計算する $V_n = \mu_n(\mathbf{B}_n)$ を提案します。コル著提案 7 の 2、

$$
V_n = \int_{-1}^{+1} \mu_{n-1}(\mathbf{B}_n(z_n)) dz_n .
$$

さて、切断 $\mathbf{B}_n(z_n)$ は、関係 $\sum_{i=1}^{n-1} z_i^2 \leq 1 - z_n^2$ によって定義される $\mathbf{R}^{n-1}$ の部分集合であり、他の語では、ホモテティー によるボール $\mathbf{B}_{n-1}$ の変換であり、比率 $\sqrt{1 - z_n^2}$ です。しかし、それは提案 11 と公式からすぐに続きます。

$$
\alpha \int_{-\infty}^{+\infty} f(\alpha x) dx = \int_{-\infty}^{+\infty} f(z) dz
$$

$f \in \mathscr{K}(\mathbf{R})$ の場合、ホモテティー $\mathbf{x} \mapsto \alpha \mathbf{x}$ の下の $\mu_{n-1}$ の像が $\alpha^{1-n} \mu_{n-1}$ のメジャーです。したがって

$$
\mu_{n-1}(\mathbf{B}_n(z_n)) = \left( \sqrt{1 - z_n^2} \right)^{n-1} V_{n-1} .
$$

(16) に代入し、変数 $z_n = \sin \varphi$ の変更を ($-\frac{\pi}{2} \leq \varphi \leq \frac{\pi}{2}$ で) とすると、次のようになります。

$$
V_n = V_{n-1} \int_{-\frac{\pi}{2}}^{+\frac{\pi}{2}} \cos^n \varphi d\varphi = 2 V_{n-1} \int_0^{\frac{\pi}{2}} \cos^n \varphi d\varphi .
$$

ただし (FRV、Ch. VII, §1, No. 3、公式 (20))

$$
\int_0^{\frac{\pi}{2}} \cos^m \varphi d\varphi = \frac{1}{2} \frac{\Gamma \left( \frac{1}{2} \right) \Gamma \left( \frac{m+1}{2} \right)}{\Gamma \left( \frac{m+2}{2} \right)}
$$

そして、関係 (17) に代入し、$\Gamma \left( \frac{1}{2} \right)$ (FRV, VII, §1, No. 3, 公式 (21)) の式を考慮すると、最終的に次のようになります。

$$
V_n = \frac{\pi^{n/2}}{\Gamma \left( \frac{n}{2} + 1 \right)} .
$$

練習問題

### 練習問題 {#int-v-s8-exercises}

[§ 8 に対して練習問題](exercises/s8/)を参照してください。
