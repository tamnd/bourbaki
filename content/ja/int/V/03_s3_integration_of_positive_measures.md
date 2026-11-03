---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 3
section_title: Integration of positive measures
lang: ja
source: int-i-vi
book_pages: INT V.96-INT V.98
pdf_pages: 0270-0286, 0351-0353
extraction: ocr
subsections:
    - "no": 1
      title: Functions with values in a space of measures
      page: 0
      pdf_page: 270
    - "no": 2
      title: Superimposed integrals of positive functions
      page: 20
      pdf_page: 275
    - "no": 3
      title: Superimposed integrals of functions with values in a Banach space
      page: 24
      pdf_page: 279
    - "no": 4
      title: Universally measurable functions
      page: 25
      pdf_page: 280
    - "no": 5
      title: Diffusions
      page: 26
      pdf_page: 281
    - "no": 6
      title: Composition of bounded diffusions
      page: 29
      pdf_page: 284
statements: 30
exercises: 11
content_sha256: 9cbccf43fe43f2d18c20164c14089c2fb71393eee002d4d573e1c9c07eb38b04
translated_from: content/en/int/V/03_s3_integration_of_positive_measures.md
translation_method: google
source_content_sha256: 4363fec5ea39b1d12c9673dd8324ba6983ab374b2f5f144cb72fb7d26d6dfd8e
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: ff3bb7ebeb326e08b7b858c18fd7418a9f45d414760e3f6a2ee37c5d349494e0
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。積極的な施策の統合

### 1. 写像と値の空間の対策

$X$ を局所コンパクト空間、$\mathscr{M}_+(X)$ を $X$ 上のポジティブ測度の凸円錐とします。この章の残り全体を通して、$\mathscr{M}_+(X)$には、$\mathscr{M}(X)$の曖昧な位相によって誘発される位相が装備されます（Ch.III, §1, No. 9）。 thus, to say that 写像 $\Lambda : t \mapsto \lambda_t$ of the locally compact 空間 $T$ into $\mathscr{M}_+(X)$ is continuous means that, for every 写像 $f \in \mathscr{K}(X)$, the numerical 写像 $t \mapsto \lambda_t(f)$ is continuous.この場合、$\Lambda$ は$T$ 上で漠然と連続しているとも言えます。 To say that 写像 $\Lambda : t \mapsto \lambda_t$ is $\mu$-measurable means that 集合 of compact 部分集合 $K$ of $T$, such that 制限 of $\Lambda$ to $K$ is vaguely continuous, is

$\Lambda : t \mapsto \lambda_t$ を T の写像から $\mathscr{M}_+(X)$ にするとします。すべての写像 $f \in \mathscr{K}(X)$ について、写像 $t \mapsto \lambda_t(f)$ が本質的に μ 積分可能である場合、Λ は測度 μ に対してスカラー的に本質的に積分可能であると言えます。 集合 $\nu(f) = \int \lambda_t(f)\, d\mu(t)$ の場合、ν が $\mathscr{K}(X)$ で正の線型形式であることは明らかであり、したがって X のメジャーになります (Ch. III, §1, No. 5、Th. 1)。 νは$\mathscr{M}_+(X)$の値と写像Λの積分であるとし、$\nu = \int \lambda_t\, d\mu(t)$と書きます。

前述の定義は弱積分の概念の特殊なケースであり、第 92 章で一般的な方法で扱われます。 VI。

$f$ が $\mathscr{K}(X)$ の元を表す場合、記法を乱用すると、整 $\int \lambda_t(f)\, d\mu(t)$ も $\int d\mu(t) \int f(x)\, d\lambda_t(x)$ と表されます。整 $\nu = \int \lambda_t\, d\mu(t)$ の定義を書き込むことができます

$$
\int f(x)\, d\nu(x) = \int d\mu(t) \int f(x)\, d\lambda_t(x).
$$

We shall make analogous abuses of 記法 in the sequel, for upper integrals, essential upper integrals, and integrals of 写像 with 値 in a Banach 空間.

#### 例 1 {#int-v-s3-n1-exa-1 .statement tag=090W}

T が離散空間であり、μ が T の各点に質量 +1 を配置することによって定義される T 上の尺度であると仮定します (Ch. III, §1, No. 3)。 h を T 上で定義された写像 $\geqslant 0$ とします。 写像 h は T、$\mu^*(h) = \mu^\bullet(h) = \sum_{t \in T} h(t)$ (Ch. IV, §1, No. 1、例) では下位半連続 (連続でも) であるため。

したがって、測定μについては、可積分関数の概念と本質的に可積分関数は同一です。そうなると、T の $\mathscr{M}_+(X)$ への写像 $t \mapsto \lambda_t$ がスカラー的に本質的にμ積分可能であると言うのは、というとなり、族 $(\lambda_t)_{t \in T}$ は加算可能 (§2, No. 1) となり、その場合、$\int \lambda_t\, d\mu(t) = \sum_{t \in T} \lambda_t$ が得られます。 写像 $t \mapsto \lambda_t$ は漠然と連続していることに注意してください。

#### 例 2 {#int-v-s3-n1-exa-2 .statement tag=090X}

写像 $t \mapsto \varepsilon_t$ of T into $\mathscr{M}_+(T)$ is vaguely continuous, scalarly essentially μ-integrable for every positive measure μ on T, and one has $\int \varepsilon_t\, d\mu(t) = \mu$.

#### 命題 1 {#int-v-s3-prop-1 .statement tag=090Y}

μ が T に関する正の測度の増加する有向族 $(\mu_i)_{i \in I}$ の上限であると仮定します。 位数で、$\Lambda : t \mapsto \lambda_t$ がスカラー的に本質的に μ 積分可能であることは、Λ がすべての $i \in I$ に対して本質的にスカラー的に本質的に $\mu_i$ 積分可能であること、および族 $(\int \lambda_t\, d\mu_i(t))_{i \in I}$ が $\mathscr{M}(X)$ で上に有界であることが必要かつ十分です。すると、ある人は、

$$
\int \lambda_t\, d\mu(t) = \sup_{i \in I} \int \lambda_t\, d\mu_i(t).
$$

なぜなら、$\Lambda$ が $T$ 上の正の測度 $\eta$ に対してスカラー的に本質的に積分可能であることを検証することは、$t \mapsto \lambda_t(g)$ が $\eta$ 可測であり、写像ごとに $\eta$ に関して有限本質上積分を認めることを検証することになるからです。 $g \in \mathscr{H}_+(X)$。したがって、命題は、§1, No. 4 の提案 11 とその系 2 からすぐに続きます。

#### 系 {#int-v-s3-n1-cor-1 .statement tag=090Z}

— *$\mu$ が、$T$ における肯定的な尺度の合計可能な族 $(\mu_\alpha)_{\alpha \in A}$ の和であると仮定します。 位数では、$\Lambda : t \mapsto \lambda_t$ がスカラー的に本質的に $\mu$ 積分可能であること、$\Lambda$ がすべての $\alpha \in A$ について本質的にスカラー的に $\mu_\alpha$ 積分可能であること、および測度群 $\int \lambda_t d\mu_\alpha(t)$ が合計可能であることが必要かつ十分です。その場合、*

$$
\int \lambda_t d\mu(t) = \sum_{\alpha \in A} \int \lambda_t d\mu_\alpha(t).
$$

すべてのスカラー的に本質的に $\mu$ 積分可能写像は、すべてのメジャー $\mu' \leq \mu$ についてもスカラー的に本質的に $\mu'$ 積分可能であることがすぐにわかります。

この切断では、次の定義で性質を検討した、$T$ の $\mathscr{M}_+(X)$ へのスカラー的に本質的に積分可能な写像の研究を極限行います。

#### 定義 1 {#int-v-s3-def-1 .statement tag=0910}

— *$X$を局所的にコンパクトな空間、$\Lambda : t \mapsto \lambda_t$をスカラー的に本質的に$\mu$積分可能な$T$の$\mathscr{M}_+(X)$への写像、$\nu$を$\Lambda$の積分とする。

$X$ で定義される下半連続写像 $f \geq 0$ ごとに、写像 $t \mapsto \int^\bullet f d\lambda_t$ が $T$ で $\mu$ 測定可能であり、* の場合、$\Lambda$ は $\mu$ 事前適切であると言います。

$$
\int^\bullet f(x) d\nu(x) = \int^\bullet d\mu(t) \int^\bullet f(x) d\lambda_t(x).
$$

*すべての肯定的な指標 $\mu' \leq \mu$ に対して $\Lambda$ が $\mu'$-事前適切である場合、$\Lambda$ は $\mu$-適切 (*) であると言います。

It can be shown that if $\Lambda$ is $\mu$-pre-adequate and if the measure $\nu = \int \lambda_t d\mu(t)$ is moderated—in particular if $X$ is countable at infinity—then $\Lambda$ is $\mu$-adequate (Exer. 7); however, it is not known if these concepts are in general equivalent. 以下の番号 2 と 3 の主張では、主張の前に a) または b) 拡大するが一度に写像に達するのに対し、c) が前にあるものは十分な写像の場合にのみ有効です。

(*) 初版では、「$\mu$-十分」写像は、スカラー的に本質的に $\mu$-積分可能で、漠然と $\mu$-測定可能写像であると定義されました。ここで挙げた定義はより一般的です (下記の提案 2)。

次の命題により、多くの場合、特定の写像が $\mu$ で適切であることを検証できます。

#### 命題 2 {#int-v-s3-prop-2 .statement tag=0911}

— $\Lambda : t \mapsto \lambda_t$ をスカラー的に本質的に $T$ から $\mathscr{M}_+(X)$ に積分可能な $\mu$ 写像とし、$\nu = \int \lambda_t \, d\mu(t)$ とします。

a) *$\Lambda$ が漠然と連続している場合、$X$ で定義された下位半連続写像 $f \geqslant 0$ に対して、写像 $t \mapsto \lambda_t^\bullet(f)$ は下位半連続であり、$\Lambda$ は $\mu$ で十分であり、関係* が得られます。

$$
\int^* f(x) \, d\nu(x) = \int^* d\mu(t) \int^* f(x) \, d\lambda_t(x).
$$

b) *$\Lambda$ が漠然と $\mu$ 測定可能である場合、$\Lambda$ は $\mu$ で十分です。*

c) *$X$ の位相が可算基底を認める場合、$\Lambda$ は漠然と $\mu$ 可測です (したがって $\mu$ 十分でもあります)。

$f$ を、$X$ で定義された下位の半連続写像 $\geqslant 0$ とします。 $F$ を集合とし、写像 $g \in \mathscr{K}(X)$ の関係 $\leqslant$ に向けて、$0 \leqslant g \leqslant f$ となるようにします。 $g \in F$ については、$h_g(t) = \lambda_t(g)$ によって $T$ に定義された $h_g$ 写像で表します。同様に、集合

$$
h_f(t) = \lambda_t^*(f) = \lambda_t^\bullet(f) = \sup_{g \in F} h_g(t)
$$

(§1, No. 1、提案 4)。次の仮定を a) よりも弱くしてみましょう: $\Lambda$ から $S$ までの制限が漠然と連続していて、$S$ が$T$ の閉じた部分集合であり、含むが$\mu$ のサポートであるとだけ仮定します。 $g \in F$ の場合、$S$ には $h_g$ があり、$C_S$ には値 $+\infty$ がある一致するという数値写像を $\overline{h}_g$ で示します。 集合 $\overline{h}_f = \sup_{g \in F} \overline{h}_g$;その後、$S$に$\overline{h}_f = h_f$。 $g \in F$ ごとに、写像 $\overline{h}_g$ は下位の半連続です。したがって、$\overline{h}_f$ は下位の半連続であり、家族 $(\overline{h}_g)_{g \in F}$ が指示されているため、

$$
\mu^*(\overline{h}_f) = \sup_{g \in F} \mu^*(\overline{h}_g) = \sup_{g \in F} \mu^*(h_g) = \sup_{g \in F} \nu(g) = \nu^*(f)
$$

(Ch. IV, §1, No. 1、Th. 1 および §2, No. 3、提案 6)。 $S$ の $h_f = \overline{h}_f$ なので、ほぼどこでも、これは (5) と同じ $\mu^*(h_f) = \nu^*(f)$、等式と書かれることもあります。同様に、$f$ と $\overline{h}_f$ は下位の半連続であるため、その前の関係は等式 $\mu^\bullet(\overline{h}_f) = \nu^\bullet(f)$ (§1, No. 1、提案 4) を生成します。 $S$ の $\overline{h}_f = h_f$ から、$\mu^\bullet(h_f) = \nu^\bullet(f)$ (§1, No. 1、提案 1)、等式は (4) と同一になります。したがって、写像 $\Lambda$ は $\mu$ より前に適しています。しかし、$\Lambda$ も本質的にスカラー的に $\mu'$ 積分可能であり、$S$ 含むは $\mu'$ のサポートであるため、この引数のどこでも $\mu$ を $\mu' \leqslant \mu$ に、$\nu$ を $\nu' = \int \lambda_t \, d\mu'(t)$ に置き換えることもできます。このことから、$\Lambda$ は $\mu$ で十分であることがわかります。

$\Lambda$ が漠然と連続していると仮定します。 $S = T$ を取るかもしれません。次に、$h_f = \overline{h}_f$ は下位の半連続であり、部分の証明 a) の主張が完了します。

$\Lambda$ が漠然と $\mu$-測定可能であると仮定し、b) を証明しましょう。 $\Lambda$ から K までの制限が連続して $\mu$ 密であるような、コンパクトな部分集合 K の T の集合 $\mathscr{K}$ (Ch. IV, §5, No. 10、提案 15)、T には次のようなメジャーの加算可能な族 $(\mu_\alpha)_{\alpha \in A}$ が存在します。 $\mu = \sum_{\alpha \in A} \mu_\alpha$ および$\mu_\alpha$ 属するから $\mathscr{K}$ までの各措置の支持 (§2, No. 3、提案 4)。すべての $\alpha \in A$ に対して、写像 $\Lambda$ は本質的にスカラー的に $\mu_\alpha$ 可積分可能であり、集合 $\nu_\alpha = \int \lambda_t d\mu_\alpha(t)$ です。ファミリ $(\nu_\alpha)$ は加算可能であり、その和は $\nu$ に等しい (提案 1 の補正)。 $f$ が X で定義された正の下限半連続写像である場合、証明の最初の部分がメジャー $\mu_\alpha$ と終了集合 $S_\alpha$ に適用されると、次のことがわかります。

$1^\circ$ $h_f$ は、$\alpha \in A$ ごとに $\mu_\alpha$ で測定可能であるため、$\mu$ は測定可能です (§2, No. 2、提案 2)。

$2^\circ$ $\int^* f(x) d\nu_\alpha(x) = \int^* d\mu_\alpha(t) \int^* f(x) d\lambda_t(x)$。

公式 (4) は、$\alpha$ (§2, No. 2、提案 1) の合計に続きます。 適用任意の測度 $\mu' \leq \mu$ に対する前述の議論 ($\Lambda$ はスカラー的に本質的に $\mu'$ 積分可能であり、漠然と $\mu'$ 可測であるため、これは正当です、cf. §2, No. 2、提案 2)、 結論するは、$\Lambda$ が $\mu'$-事前適切であること、および b) が証明されます。

最後に、X の位相が可算基底を認めると仮定して、T の $\mathscr{M}_+(X)$ へのすべてのスカラー的に本質的に $\mu$ 積分可能な写像 $\Lambda : t \mapsto \lambda_t$ は漠然と $\mu$ 可測であることを示しましょう。これは、次の補題の結果となります。

#### 補題 {#int-v-s3-n1-lem-1 .statement tag=0912}

*Xを可算数基底を持つ局所コンパクト空間とする。次に、$\mathscr{K}(X)$ には、以下の性質を持つ可算部分集合 S が存在します。 写像 $f \in \mathscr{K}(X)$ ごとに、S の元の数列 $(f_n)$ と、次のような正の写像 $\varphi \in S$ が存在します。 n が十分大きいである場合、すべての数 $\varepsilon > 0$、$|f_n - f| \leq \varepsilon \varphi$ に対して。*

$X'$ を X の Alexandroff コンパクト化とし、これは計量可能コンパクト空間 (GT、IX, §2, No. 9、Prop. 16 および Cor.) です。私たちは同一視する $\mathscr{K}(X)$ と $\mathscr{C}(X')$ の部分集合です。 $S'$ をバナハ空間 $\mathscr{C}(X')$ (GT, X, §3, No. 3, Th. 1) の可算密集部分集合とする。 $n \in \mathbf{N}$ ごとに $S'$ 含むが定数写像 $n$ であると仮定できます。 $(U_n)$ を、X で比較的コンパクトなオープン集合の数列とし、和集合 X を使用して、すべての n (GT、I, §9, No. 9、提案 15) について $\overline{U}_n \subset U_{n+1}$ を$\varphi_n$ とします。 $\mathscr{K}_+(X)$の写像は、$\overline{U}_n$の1に等しい。 形 $\varphi_n g$ ($n \in \mathbf{N}, g \in S'$) の$\mathscr{K}(X)$ の元の可算集合を S で表します。 $f \in \mathscr{K}(X)$の場合、$(g_n)$を$f$に一様に収束する$S'$の元の数列とし、$f$のサポートが$U_k$に含まれるようにkを整数とします。最後に、m を写像 $g_n$ のノルムに対する上界である整数とします。 写像 $f_n = \varphi_k g_n$ 属するを S および満たす主張に、$\varphi = m \varphi_k$ を付けます。

補題が確立されており、写像 $t \mapsto \lambda_t(g)$ は基本的に $g \in S$ ごとに $\mu$ 積分可能であるため、$\mathbf{R}^S$ への T の写像 $t \mapsto (\lambda_t(g))_{g \in S}$ は$\mu$ 可測です (Ch. IV, §5, No. 3、Th 1)。この写像から K までの制限が連続するようなコンパクトな T の部分集合 K の集合 $\mathscr{K}$ は、したがって $\mu$ 密であり、すべての $\Lambda$ の制限が証明できれば十分です。 $K \in \mathscr{K}$は連続です。ここで、$f$ を、補題の S 満たす主張の $\mathscr{K}(X)$、$f_n$、および $\varphi$ 元のいずれかの元とします。 写像 $t \mapsto \lambda_t(f)$ は、連続写像 $t \mapsto \lambda_t(f_n)$ の K 上の均一極限です。したがって、K 上で連続であり、命題が証明されます。

### 2. 正の写像の重畳積分

切断の残りについては、反対の明示的な言及がない限り、局所的にコンパクトな空間を X で、T の $\mu$ から $\mathscr{M}_+(X)$ への適切な写像を $\Lambda : t \mapsto \lambda_t$ で、そして の積分を $\nu$ で表すことにします。 $\Lambda$。

#### 命題 3 {#int-v-s3-prop-3 .statement tag=0913}

— f を、X で定義された数値写像 $\geqslant 0$ とします。
a) 次の不等式が成り立ちます。

$$
\int^* f(x)\, d\nu(x) \geqslant \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x) \geqslant \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x).
$$

b) $\Lambda$ が漠然と連続している場合、

$$
\int^* f(x)\, d\nu(x) \geqslant \int^* d\mu(t) \int^* f(x)\, d\lambda_t(x).
$$

c) $\lambda_t^\bullet(1) < +\infty$ ローカルに $\mu$ - ほぼどこでも、

$$
\int^\bullet f(x)\, d\nu(x) \geqslant \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x) = \int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x).
$$

g を $f \leqslant g$ となるような、X 上の下位半連続写像とします。 $t \in T$ごとに、

$$
\int^* f(x)\, d\lambda_t(x) \leqslant \int^* g(x)\, d\lambda_t(x),
$$

したがって、(4) と §1 の提案 4 により、

$$
\int^\bullet d\mu(t) \int^* f(x)\, d\lambda_t(x) \leqslant \int^\bullet d\mu(t) \int^* g(x)\, d\lambda_t(x) = \int^* g(x)\, d\nu(x).
$$

最初の不等式 (6) は、$\int^* f(x)\, d\nu(x)$ (Ch. IV, §1, No. 3、定義 3) の定義から続き、2 番目はそこからすぐに続きます。 不等式 (7) は、$\Lambda$ が漠然と連続している場合、(4) の代わりに (5) を使用して、同様の方法で証明されます。

(8)の証明に進みます。 写像 $t \mapsto \lambda_t^*(1)$ は測定可能であり、局所的に有限です $\mu$ - ほぼどこでも。 $t \mapsto \lambda_t^*(1)$から$K$までの制限などの$T$のコンパクト部分集合の集合$\mathscr{K}$は有限で連続は$\mu$密であり、§2, No. 3の提案4は加算可能な族$(\mu_\alpha)_{\alpha \in A}$の存在を意味します。 所属から$\mathscr{K}$まで、$\mu = \sum_{\alpha \in A} \mu_\alpha$となるような前向きな措置。 写像 $\Lambda$ は、$\alpha \in A$ ごとに $\mu_\alpha$ が適切です。 集合 $\nu_\alpha = \int \lambda_t d\mu_\alpha(t)$。 提案 1 は、$\mu_\alpha$ と写像 1 に適用される $\nu = \sum_{\alpha \in A} \nu_\alpha$ と関係 (4) が、$\nu_\alpha$ が有界のメジャーであることを示しています ($\lambda_t^*(1)$ は $\operatorname{Supp}(\mu_\alpha)$ で制限されているため)。 次に、$\int^\bullet$ による最初のメンバーのメジャー $\mu_\alpha$、置き換えることのシンボル $\int^*$ に対して公式 (6) を書きましょう。これは、§1 の提案 7 によって正当です。それから

$$
\int^\bullet f(x) d\nu_\alpha(x) \geq \int^\bullet d\mu_\alpha(t) \int^* f(x) d\lambda_t(x) = \int^\bullet d\mu_\alpha(t) \int^\bullet f(x) d\lambda_t(x)
$$

(最後の等式は、$\lambda_t$ がほぼどこでも局所的に制限されているという事実と、§ 1 の提案 7 によるものです)。 (8) の不等式は、$\alpha$ を合計することによって得られます (§2, No. 2、提案 1)。

c) と同様の仮定が作成されない場合、不等式 (8) は失敗する可能性があります (例 2)。

#### 系 1 {#int-v-s3-prop-3-cor-1 .statement tag=0914}

— *$f$ を $X$ で定義された写像 $\geq 0$ とし、$H$ を $f$ が $\lambda_t$ 無視できないように $t \in T$ の集合とする。
a) *$f$ $\nu$ が無視できる場合、$H$ は局所的に $\mu$ が無視できます。*
b) *$f$ が $\nu$ で無視でき、$\Lambda$ が漠然と連続している場合、$H$ は $\mu$ で無視できます。*
c) *$f$ が局所的に $\nu$ で無視でき、$\lambda_t^\bullet(1) < +\infty$ が局所的に $\mu$ でほぼどこでもある場合、$H$ は局所的に $\mu$ で無視できます。*

#### 系 2 {#int-v-s3-prop-3-cor-2 .statement tag=0915}

— *$f$ を、$X$、$\nu$ 測定可能、および $\nu$ で定義された写像 $\geq 0$ とします。 $f$ が $\lambda_t$ で緩和されていないような $t \in T$ の集合は、局所的に $\mu$ が無視できます ($\Lambda$ が漠然と連続している場合は、$\mu$ も無視できます)。

For, $f$ is the sum of a sequence of functions $f_n \geq 0$ such that $f_n$ is zero outside a compact set $K_n$ for $n \geq 1$, and $f_0$ is $\nu$-negligible (§1, No. 2, Prop. 6); $f_0$ is then $\lambda_t$-negligible except for $t$ forming a set that is locally $\mu$-negligible (and even $\mu$-negligible, if $\Lambda$ is vaguely continuous) by Cor. 1, and the statement then follows at once.

#### 命題 4 {#int-v-s3-prop-4 .statement tag=0916}

— *$f$ を $X$ で定義された $\nu$ 可測写像とし、値をトポロジカル空間 $G$ とし、$M$ を $f$ となる $t \in T$ の集合とします。 $\lambda_t$-測定可能ではありません。*
a) *$f$ が $X$ の $\nu$ で緩和された部分集合の補数で一定であると仮定します。その場合、$M$ はローカルでは $\mu$ は無視されます。*

b) * f が X の ν 緩和部分集合の補数で定数であり、Λ が漠然と連続であると仮定します。この場合、M はμ-無視できます。*

c) *ほとんどどこでも $\lambda_t^\bullet(1) < +\infty$ が局所的に μ であると仮定します。この場合、M は局所的にμが無視できます。*

まず a) (それぞれ b)) を証明しましょう。 すべての ν 積分可能集合は ν 積分可能開集合に含まれるため、写像 f は ν 積分可能開集合の可算和集合の補数 B 上で定数です。 各 $K_n$ に対する f の制限が連続となるように、ν 無視できる集合 N とコンパクト集合の数列 $(K_n)$ によって形成される X − B の分割が存在します。 N が $\lambda_t$ 無視できないように、S を $t \in T$ の集合とします。 S は、Cor によって局所的に μ 無視可能 (それぞれ μ 無視可能) です。提案 3 の 1。 集合 $K_n, B, N$ はX の小節ごとに測定可能であり、それぞれの f の制限は $t \notin S$ ごとに $\lambda_t$-測定可能です。 したがって、写像 f は、$t \notin S$ ごとに $\lambda_t$ 測定可能です (Ch. IV, §5, No. 10、提案 16)。

c) を確立するために、提案 3 の証明の記法をもう一度取り上げてみましょう。 f は ν 可測であるため、各尺度 $\nu_\alpha \leq \nu$ について可測です。ここで、これらの尺度は制限されているため緩和されており、a) から、M はすべての $\alpha \in A$ について局所的に $\mu_\alpha$ 無視できることがわかります。これは、M が局所的にμ-無視できることを意味します (§2, No. 2、提案 1 の Cor. 2)。

#### 命題 5 {#int-v-s3-prop-5 .statement tag=0917}

* f を X で定義された ν 可測の正の数値写像とし、N を $\lambda_t$ 可測かつ $\lambda_t$ 緩和の両方にならないように、N を $t \in T$ の集合とします。

a) * f が ν 緩和されていると仮定します。 集合 N は局所的にμが無視でき、写像 $t \mapsto \int^\bullet f(x) d\lambda_t(x)$ はμが測定可能であり、*

$$
\int^\bullet f(x) d\nu(x) = \int^\bullet d\mu(t) \int^\bullet f(x) d\lambda_t(x).
$$

b) * f が ν 緩和されており、Λ が漠然と連続していると仮定します。 集合 N はμが無視でき、写像 $t \mapsto \int^* f(x) d\lambda_t(x)$ はμが測定可能でμが緩和され、*

$$
\int^* f(x) d\nu(x) = \int^* d\mu(t) \int^* f(x) d\lambda_t(x).
$$

c) *ほとんどどこでも $\lambda_t^\bullet(1) < +\infty$ が局所的に μ であると仮定します。 集合 N は局所的にμ-無視でき、写像 $t \mapsto \int^\bullet f(x) d\lambda_t(x)$ はμ-測定可能であり、(9) が成り立ちます。*

f が ν 緩和されていると仮定して、最初に a) (それぞれ b)) を証明しましょう。 集合 N に関する主張はすでに確立されている（提案 4、提案 3 の裏付け 2）。 §1, No. 2 の提案 6 により、以下の特殊なケースのそれぞれで、極限自身を証明 a) (それぞれ b)) にすることができます。

1) 写像 $f$ は $\nu$ は無視できます。
2) $f$が$K$の外側に零で、$f$～$K$の制限が連続するようなコンパクト集合$K$が存在します。

特殊なケース 1) はすでに処理されています (提案 3 の訂正 1)。 To treat the second, we denote by $G$ a $\nu$-integrable open set containing $K$, by $M$ a constant upper bound for $f$, by $h$ the lower semi-continuous function $M \varphi_G$, and by $g$ the function $h - f$. 写像 $f$は$X$の上半連続なので、$g$は下半連続でプラスです。 さらに、$f, g, h$ は $\nu$ 可積分です。

次に、公式 (4) (それぞれ (5)) を下側の半連続写像 $h$ と $g$ に適用しましょう。引き算すると、写像であることがわかります。

$$
t \mapsto \int^\bullet f(x)\, d\lambda_t(x) \quad (\text{resp. } \int^* f(x)\, d\lambda_t(x))
$$

は$\mu$-可測であり、公式 (9) (それぞれ (10)) が成り立ちます。最後に、b) の仮定の下で、写像 $t \mapsto \int^* f(x)\, d\lambda_t(x)$ は有限の上積分を持ち、したがって実際に $\mu$ 緩和されます。

c)を証明するために、提案3の証明の措置$\mu_\alpha$と$\nu_\alpha$をもう一度取り上げてみましょう。 $f$ は $\nu_\alpha$ 測定可能であり、$\nu_\alpha$ は緩和されているため、主張 a) は、$t \mapsto \int^\bullet f(x)\, d\lambda_t(x)$ は $\mu_\alpha$ 測定可能であり、

$$
\int^\bullet f(x)\, d\nu_\alpha(x) = \int^\bullet d\mu_\alpha(t) \int^\bullet f(x)\, d\lambda_t(x).
$$

残るは$\alpha$、適用の小道具の和までです。 §2, No. 2の1と2。

$f$ が $\nu$ で緩和されていると仮定されておらず、c) で仮定を作成しない場合、関係 (9) は成立しない可能性があります (例 3)。

#### 系 {#int-v-s3-n2-cor-1 .statement tag=0918}

— *$\mathbf{f}$ を $X$ で定義された写像とし、値を Banach 空間 $F$ または $\overline{\mathbf{R}}$ で定義します。つまり、$\nu$ が測定可能で、$\nu$ が緩和されます。 $\mathbf{f}$ が $\nu$ 積分可能であるためには、次のことが必要かつ十分です*

$$
\int^\bullet d\mu(t) \int^\bullet |\mathbf{f}(x)|\, d\lambda_t(x) < +\infty.
$$

これは、提案 5 と積分可能性の基準 (Ch. IV, §5, No. 6、Th. 5) からすぐに得られます。

### 3. Banach 空間における写像と値の重ね合わせ積分

#### 定理 1 {#int-v-s3-thm-1 .statement tag=0919}

— $f$ をバナッハ空間 $F$ または $\overline{\mathbf{R}}$ の値を持つ写像とし、$H$ を $f$ が $\lambda_t$ 積分可能ではない $t \in T$ の集合とする。

a) *$f$ が $\nu$ 積分可能である場合、$H$ は局所的に $\mu$ 無視可能であり、写像 $t \mapsto \int f(x)\, d\lambda_t(x)$ ($t \notin H$ について定義) は本質的に $\mu$ 積分可能であり、*

$$
\int f(x)\, d\nu(x) = \int d\mu(t) \int f(x)\, d\lambda_t(x).
$$

b) *If $f$ is $\nu$-integrable and $\Lambda$ is vaguely continuous, then $H$ is moreover $\mu$-negligible and the function $t \mapsto \int f(x)\, d\lambda_t(x)$ (defined for $t \notin H$) is $\mu$-integrable.*

c) *ほぼどこでも $\lambda_t^*(1) < +\infty$ が局所的に $\mu$ である場合、a) の結論は、本質的に $\nu$ 可積分関数である $f$ に当てはまります。

まず、a) (それぞれ b)) を確立します。この主張は、$f$ が正の数値写像の場合に当てはまります (提案 5)。 $f$ が可積分関数で、$\overline{\mathbf{R}}$ に値がある場合、この結果は、正の写像 $f^+$ と $f^-$ に適用されるため、減算によって拡大するが一度に $f$ になります。 $F$の値で写像のケースを扱うことが残っています。 $\mathscr{H}$を線形結合で形成された$\mathscr{L}_F^1(\nu)$の部分空間とし、$F$の係数、$\mathscr{K}(X)$の写像の部分空間とします。実数写像に関する結果は、$\mathscr{H}$ の元に対する主張の妥当性を直ちに暗示します。さて、$\mathscr{H}$は$\mathscr{L}_F^1(\nu)$に密集しています。したがって、すべての $f \in \mathscr{L}_F^1(\nu)$ に対して、次のプロパティを持つ $\mathscr{H}$ の元のうち数列 $(f_n)$ が存在します。

1) 数列 $(f_n)$ は、$\mathscr{L}_F^1(\nu)$ および $\nu$ の平均値で $f$ にほぼどこでも収束します。
2) 写像 $g = |f_0| + \sum_{n \in \mathbf{N}} |f_{n+1} - f_n|$ は $\nu^*(g) < +\infty$ となる (第 3 章、IV, §3, No. 4)。

$N_1$ を $\lambda_t^*(g) = +\infty$ となるような $t \in T$ の集合とします。 $N_1$ は、公式 (6) (それぞれ (7)) によって局所的に $\mu$ 無視可能 (それぞれ $\mu$ 無視可能) です。 $t \notin N_1$ については、$f_n$ 属するから $\mathscr{L}_F^1(\lambda_t)$、数列 $(f_n)$ はほぼどこでも $\lambda_t$ に収束し、$\mathscr{L}_F^1(\lambda_t)$ の平均値の位相についても収束します (Ch. IV, §3, No. 3、提案 6)。 $M$ を $f_n(x)$ が $f(x)$ に収束しないように $x \in X$ の集合とします。 $M$ は $\nu$ 無視できるので、 $M$ が収束しないように $t \in T$ の集合 $N_2$ とします。 $\lambda_t$-negligible は、Cor による局所的な $\mu$-negligible (それぞれ $\mu$-negligible) です。提案 3 の 1。

$t$ が属するから $N_1 \cup N_2$ にならないとします。 数列 $(f_n)$ は $\mathscr{L}_F^1(\lambda_t)$ で平均値に収束し、$\lambda_t$ - ほぼどこでも $f$ に収束します。したがって、$f \in \mathscr{L}_F^1(\lambda_t)$ と $\int f\, d\lambda_t = \lim_{n \to \infty} \int f_n\, d\lambda_t$ (Ch. IV, §4, No. 1)。したがって、主張の集合 $H$ は $N_1 \cup N_2$ に含まれます。したがって、局所的には $\mu$ は無視できます (それぞれ $\mu$ は無視できます)。一方、写像 $t \mapsto \int f\, d\lambda_t$ は、局所的に $\mu$ - ほぼどこでも、$\mu$ の数列 - 測定可能な写像の極限に等しい。したがって、$\mu$-測定可能です。最後に、$t \notin N_1 \cup N_2$ と $n$ ごとに、
$$
\left| \int f_n(x)\, d\lambda_t(x) \right| \leq \int^* g(x)\, d\lambda_t(x)
$$
不等式 $|f_n| \leq g$ および第 2 章の提案 2 によりIV, §4, No. 2。さて、写像 $t \mapsto \int^* g(x)\, d\lambda_t(x)$ は、提案 5 により本質的に $\mu$ 可積分 (それぞれ $\mu$ 可積分) です。 したがって、ルベーグの定理を適用すると、次のようになります。
$$
\int d\mu(t) \int f(x)\, d\lambda_t(x) = \lim_{n \to \infty} \int d\mu(t) \int f_n(x)\, d\lambda_t(x) = \lim_{n \to \infty} \int f_n(x)\, d\nu(x).
$$
$\int f_n(x)\, d\nu(x)$ は $\int f(x)\, d\nu(x)$ になる傾向があり、$n$ は $\infty$ になる傾向があるため、数列 $(f_n)$ で立てられた仮説により、関係 (11) が続き、a) (それぞれ b)) が証明されました。

ここで、$\lambda_t^\bullet(1) < +\infty$ がローカルで $\mu$ - ほぼどこでも、そして $g$ が本質的に $\nu$ 可積分関数であると仮定します。 $f$ を、$g = f$ が局所的に $\nu$ ほぼどこでも (§ 1, No. 3) となるような $\nu$ 積分可能な関数とします。次に、$\lambda_t$ のほぼどこでも $g = f$ ですが、局所的に $\mu$ 無視できる集合 $P$ を形成する $t$ を除きます (提案 3 の Cor. 1 c)。したがって、すべての $t \notin P \cup H$ に対して $\int g\, d\lambda_t = \int f\, d\lambda_t$ となり、これで証明が完成します。

#### 注意 {#int-v-s3-n3-rem-1 .statement tag=091A}

$\Lambda : t \mapsto \lambda_t$ を $T$ から $\mathscr{M}_+(X)$ に相当する $\mu$ 写像とします。 If a mapping $\Lambda' : t \mapsto \lambda'_t$ of $T$ into $\mathscr{M}_+(X)$ is equal to $\Lambda$ locally $\mu$-almost everywhere, it follows at once from the definitions that $\Lambda'$ is also $\mu$-adequate, and that $\Lambda$ and $\Lambda'$ have the same integral. ここで、$H : t \mapsto \eta_t$ が写像で、$\mathscr{M}_+(X)$ に値があり、ローカルに定義されている $\mu$ - ほぼどこでも、$H$ が$\mu$ - ローカルに等しい場合、$\mu$ - ほぼどこでも写像 $\Lambda : t \mapsto \lambda_t$ に等しいと再び言えます。定義されており、$\mu$-適切です。 次に、写像 $\Lambda$ に依存しない集合 $\int \eta_t\, d\mu(t) = \int \lambda_t\, d\mu(t)$、定義を利用します。 前述の番号拡大するから $\mu$ で証明された命題が、ローカルに定義された $\mu$ の適切な写像をほぼすべての場所で検証するタスクは、読者に委ねられます。

### 4. 普遍的に測定可能写像

#### 定義 2 {#int-v-s3-def-2 .statement tag=091B}

* T の写像 f をトポロジカル空間に変換したものは、T 上のすべての正の測度 $\mu$ について $\mu$ 可測である場合、普遍的に可測であると言われます。

特性写像が普遍可測である T の部分集合を普遍可測集合と呼びます。彼らは形 T の部族 (Ch. IV, §5, No. 4、Th. 2 の Cor. 2)、 含むボレル族集合 (同じ参照、Cor. 3)、T がメトリズ可能であればスースリン族集合 (Ch. IV, §5, No. 1、提案 3 の Cor. 2)。 T の写像 $f$ を、計化可能かつ分離可能なトポロジカル空間 F に変換して普遍的に測定可能にするためには、F のすべての閉じた球の $f$ の下にある逆像が T の普遍的に測定可能な部分集合であることが必要かつ十分です (Ch. IV, §5, No. 5, 4）。

#### 命題 6 {#int-v-s3-prop-6 .statement tag=091C}

*T の写像 $f$ をトポロジカル空間 F に普遍的に測定可能にするためには、コンパクトなサポートを備えた T 上のすべての正の測度に対して $f$ が測定可能であることが必要かつ十分です。

条件は明らかに必要です。一方、すべての肯定的な尺度 $\mu$ は、コンパクトなサポート (§2, No. 3、提案 4) を備えた一連の尺度の和であるため、これで十分です。 主張は、§2, No. 2 の提案 2 から続きます。

#### 命題 7 {#int-v-s3-prop-7 .statement tag=091D}

*$\mu$ を T の正の測度とし、$f$ を T からトポロジカル空間 F への $\mu$ 可測の写像とする。すると、局所的に $f = f'$ が成り立つような、T から F への普遍的に可測な写像 $f'$ が存在する。 $\mu$-ほぼどこにでも。*

$\mathscr{K}$ を、K までの $f$ の制限が連続となるように、T における圧縮集合の集合とします。 $\mathscr{K}$ は $\mu$ 密であるため (Ch. IV, §5, No. 10、提案 15)、集合 $N = T - \bigcup_{i \in I} K_i$ が局所的に $\mu$ 無視できるような、$\mathscr{K}$ の対互いに素元の局所的に可算な族 $(K_i)_{i \in I}$ が存在します (Ch. IV, §5, No. 9、提案 14)。 $x$ を F の元とします。 集合

$$
f'(t) = f(t) \quad \text{if } t \in \bigcup_{i \in I} K_i,
$$
$$
f'(t) = x \quad \text{if } t \in N.
$$

写像 $f$ と $f'$ は、局所的には $\mu$ - ほぼどこでも等しいです。 一方、$N \cap K$ は、族 $(K_i)$ が局所的に可算であるため、T のすべてのコンパクト集合 K に対する K のボレル部分集合です。 したがって、N は普遍的に測定可能な集合であり、$f'$ は普遍的に測定可能な写像であるということになります (Ch. IV, §5, No. 10、提案 16)。

### 5. 拡散

#### 定義 3 {#int-v-s3-def-3 .statement tag=091E}

*Xを局所的に圧縮した空間とし、$\Lambda : t \mapsto \lambda_t$をTの$\mathscr{M}_+(X)$への写像とする。 写像 $\Lambda$ は、X における T の拡散* であると言われます。Λ がコンパクトなサポートを備えた T のすべての正の測度に適切である場合です。すべての尺度 λ_t が有界であり、$\sup_{t \in T} \| \lambda_t \| < +\infty$ である場合、拡散 Λ は有界であると言われます。この量はΛのノルムと呼ばれ、$\| \Lambda \|$と表されます。

次の命題は、単に定義を翻訳するだけです。

#### 命題 8 {#int-v-s3-prop-8 .statement tag=091F}

— T の写像 $\Lambda : t \mapsto \lambda_t$ が $\mathscr{M}_+(X)$ に拡散するには、次の条件が満たされることが必要かつ十分です。
1) X で定義された下半連続写像 $f \geqslant 0$ ごとに、写像 $t \mapsto \lambda_t^\bullet(f)$ は T で普遍的に測定可能です。
2) すべての写像 $g \in \mathscr{K}_+(X)$ に対して、写像 $t \mapsto \lambda_t(g)$ は T 内で局所的に有界されます。
3) X で定義されたすべての下位半連続写像 $f \geqslant 0$ と、コンパクトサポートを備えた T 上のすべての正の測定値 $\mu$ について、次の関係が成り立ちます。ここで、$\nu$ は $\int \lambda_t d\mu(t)$ を表します。

$$
\int^\bullet f(x) d\nu(x) = \int^\bullet d\mu(t) \int^\bullet f(x) d\lambda_t(x).
$$

$\Lambda$ が拡散であると仮定します。 条件 1) は、適切な写像 (No. 1、定義 1) と提案 6 の定義によって満たされます。 $\Lambda$ は $\mu$ で十分であるため、条件 3) は公式 (4) によって満たされます。 $g \in \mathscr{K}_+(X)$ と $u$ を写像 $t \mapsto \lambda_t(g)$ (普遍的に測定可能、1)) とします。 $u$ が局所的に有界されていないと仮定します。その場合、$u$ が K で制限されないようなコンパクトな集合 K が存在するため、すべての $n \geqslant 1$ に対して $u(t_n) \geqslant n^2$ となるような K の元の数列 $(t_n)$ が存在することになります。この場合、$\Lambda$ の仮定とは対照的に、$u$ はコンパクト サポートを備えたメジャー $\mu = \sum_{n \geqslant 1} \frac{1}{n^2} \varepsilon_{t_n}$ に対して積分可能ではありません。これは、$t \mapsto \lambda_t(g)$ がコンパクト サポートを備えたすべてのポジティブ メジャーに対して積分可能であることを意味します。したがって、上記の 3 つの条件が必要になります。逆に、条件 1) と 2) は、$\Lambda$ がコンパクトなサポートを備えたすべてのメジャー $\mu$ に対して本質的にスカラー的に $\mu$ 積分可能であることを意味します。コンパクト サポートを持つメジャー $\mu$ によって上に境界付けられるすべてのメジャー $\mu' \geqslant 0$ もコンパクト サポートを持つため、条件 1) と 3) は、コンパクト サポートを持つすべてのポジティブ メジャーに対して $\Lambda$ が $\mu$ で適切であることを表しており、これは実際に求められている結果です。

#### 命題 9 {#int-v-s3-prop-9 .statement tag=091G}

— $\Lambda : t \mapsto \lambda_t$ を $\mathscr{M}_+(X)$ への T の写像として、写像 $t \mapsto \lambda_t(g)$ が普遍的に測定可能であり、すべての $g \in \mathscr{K}_+(X)$ について T 内で局所的に限定されるようにします。以下のそれぞれの場合において、$\Lambda$ は拡散であると断言できます。

a) X の *位相は可算基底* を認めます。
b) *Λ は曖昧な位相* に対して普遍的に測定可能です。

というのは、$\mu$ をコンパクトなサポートで $T$ に対する積極的な尺度とします。 写像 $\Lambda$ は本質的にスカラー的に $\mu$ 積分可能であるため、a) または b) のいずれかが満たされる場合には $\mu$ が適切です (No. 1、提案 2)。

この切断の残りの部分については、次の記法を採用します。正の $\eta$ 可測写像 $h$ の、正の測度 $\eta$ の上部本質積分を $⟨\eta, h⟩$ で表します。 写像 $\Lambda : t \mapsto \lambda_t$ は、$X$ の $T$ の拡散になります。 $f$ が $X$ で定義された正の普遍的に測定可能な写像である場合、$\Lambda f$ 写像 $t \mapsto \lambda_t^*(f)$ で表します。 $\mu$ が $T$ に対する正の測度であり、$\Lambda$ がスカラー的に本質的に $\mu$ 可積分である場合、測度 $\int \lambda_t d\mu(t)$ を $\mu\Lambda$ で表すものとします。積分の定義には形がかかります

$$
⟨\mu\Lambda, f⟩ = ⟨\mu, \Lambda f⟩ \quad \text{for } f \in \mathscr{K}_+(X).
$$

$\Lambda$ が $\mu$ 適切である場合、$T$ *属するの$\Lambda$* の定義域に対する正の測度 $\mu$ は、$\Lambda$ がスカラー的に本質的に等しいと言えます。これは、というになります。 $\mu$ 積分可能、およびすべてのポジティブな測定値 $\mu' \leq \mu$ およびすべての下位の半連続ポジティブ写像 $f$ の $⟨\mu'\Lambda, f⟩ = ⟨\mu', \Lambda f⟩$。

#### 命題 10 {#int-v-s3-prop-10 .statement tag=091H}

*$f, g$ を $X$ 上の普遍的に測定可能な 2 つのポジティブな写像とし、$a$ を数 $\geq 0$ とし、$\mu$ と $\nu$ を $T$ 上の 2 つのポジティブな尺度とします。それから：*

a) $\Lambda(f + g) = \Lambda f + \Lambda g$、$\Lambda(af) = a\Lambda f$。
b) *$\mu$ と $\nu$ 属するが $\Lambda$ の領域にある場合、$\mu + \nu$ と $a\mu$ も同様になり、1 つは * $(\mu + \nu)\Lambda = \mu\Lambda + \nu\Lambda$、$(a\mu)\Lambda = a(\mu\Lambda)$ になります。

唯一の非自明な点は、 $\Lambda$ の領域に対する $\mu + \nu$ 属するであり、これは観察するとによって処理され、その上で $\mu + \nu$ で囲まれたすべての正の測度は形 $\mu' + \nu'$ のものであり、ここで $\mu' \leq \mu$、$\nu' \leq \nu$ ( 「分解補題」、Ch. II, §1, No. 1)。 次の命題もご覧ください。

#### 命題 11 {#int-v-s3-prop-11 .statement tag=091I}

*$T$ から属するの$\Lambda$ の領域に対する積極的な測度 $\mu$ については、$\Lambda$ がスカラー的に本質的に $\mu$ 積分可能であることが必要かつ十分です。

この条件は明らかに必要です。逆に、それが満たされると仮定し、$f$ を $X$ で定義された下位の半連続正の写像とします。 写像 $\Lambda f$ は普遍的に測定可能であるため、$\mu$ も測定可能です。 $⟨\mu, \Lambda f⟩ = ⟨\mu\Lambda, f⟩$; ということを証明していきます。この等式はすべての正の測度 $\mu' \leq \mu$ にも有効であり、$\Lambda$ もスカラー的に本質的に $\mu'$ 積分可能であるため、$\Lambda$ は $\mu$ で十分であることがわかります。

$(\mu_i)_{i\in I}$ を、$\mu = \sum_{i\in I} \mu_i$ (§2, No. 3、提案 4) のような、コンパクトなサポートを備えた要約可能なポジティブ指標群とします。測定値ファミリー $\mu_i \Lambda$ は合計可能であり、 $\mu \Lambda = \sum_{i \in I} \mu_i \Lambda$ (No. 1、提案 1 の補正)。従って、$\langle \mu \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i \Lambda, f \rangle$ (§ 2, No. 2、提案 1)。しかし、$\Lambda$ は $\mu_i$ で十分であるため、$\langle \mu_i \Lambda, f \rangle = \langle \mu_i, \Lambda f \rangle$ になります。再度、適用 § 2 の提案 1 を実行すると、目的の等式が得られます。

$$
\langle \mu \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i \Lambda, f \rangle = \sum_{i \in I} \langle \mu_i, \Lambda f \rangle = \langle \mu, \Lambda f \rangle .
$$

#### 系 1 {#int-v-s3-prop-11-cor-1 .statement tag=091J}

— *$\Lambda$ が有界拡散の場合、すべての有界正測度 $\mu$ 属するは $\Lambda$ および $\| \mu \Lambda \| \leq \| \mu \| \| \Lambda \|$ の領域になります。*

#### 系 2 {#int-v-s3-prop-11-cor-2 .statement tag=091K}

— *$\mu$ が、$\Lambda$ の領域に対する肯定的な測度所属の加算可能な族 $(\mu_\alpha)_{\alpha \in A}$ の和であると仮定します。 $\Lambda$ の領域に対する $\mu$ から属するについては、メジャーの族 $\mu_\alpha \Lambda$ が合計可能であることが必要かつ十分であり、その場合は $\mu \Lambda = \sum_{\alpha \in A} \mu_\alpha \Lambda$* になります。

No. 1の提案1の系を適用すれば十分です。

命題 5 を拡散の言語で表現すると、次のような形になります。

#### 命題 12 {#int-v-s3-prop-12 .statement tag=091L}

— *$\mu$ を $\Lambda$ の領域に対する属するである $T$ での正の尺度とし、$f$ を $X$ で定義される普遍的に測定可能な写像 $\geq 0$ とします。 $f$ が $\mu \Lambda$ の測定値に対して緩和されている場合、または $\lambda_t$ の測定値が制限されている場合、 写像 $\Lambda f$ は $\mu$ 測定可能であり、*

$$
\langle \mu \Lambda, f \rangle = \langle \mu, \Lambda f \rangle .
$$

#### 系 {#int-v-s3-n5-cor-1 .statement tag=091M}

— *$X$ が無限に可算である場合、またはメジャー $\lambda_t$ が有界である場合、写像 $\Lambda f$ は、$X$ で定義されるすべての普遍的に測定可能な写像 $f \geq 0$ について、$T$ で普遍的に測定可能であり、(13)が成立します。*

### 6. 有界拡散の合成

#### 命題 13 {#int-v-s3-prop-13 .statement tag=091N}

— *$T, X, Y$ を 3 つの局所コンパクト空間、$\Lambda : t \mapsto \lambda_t$ を $X$ の $T$ の有界拡散、$H : x \mapsto \eta_x$ を $Y$ の $X$ の有界拡散とする。 写像 $t \mapsto \lambda_t H$ は、$Y$ での $T$ の有界拡散であり、$\Lambda H$ で示され、*

$$
\| \Lambda H \| \leq \| \Lambda \| \| H \|.
$$

*$f$ を$Y$ で定義された普遍的に測定可能な写像 $\geq 0$ とし、$\mu$ を $T$ での測定値とします。 $\mu$ 属するを $\Lambda$ のドメインに、* μΛ 属するを H のドメインにするとします。次に μ 属するを ΛH の領域に、そして

$$
\langle \mu(\Lambda H), f \rangle = \langle \mu \Lambda, Hf \rangle = \langle \mu, \Lambda Hf \rangle;
$$
(15)
$$
(\mu \Lambda)H = \mu(\Lambda H); \quad \Lambda(Hf) = (\Lambda H)f.
$$

集合 $\gamma_t = \lambda_t H$; T の $\Gamma$ 写像 $\Lambda H$ を $\mathscr{M}_+(Y)$ に、そして $\Gamma f$ 写像 $t \mapsto \langle \gamma_t, f \rangle$ で表します ($\Gamma$ が拡散であるかどうかまだわからないため、記法の乱用)。次に、(13) によって $\langle \gamma_t, f \rangle = \langle \lambda_t H, f \rangle = \langle \lambda_t, Hf \rangle$ が計算されます。 写像 $Hf$ は正であり、X で普遍的に測定可能であるため (提案 12 の修正)、まず第一に $\Gamma f = \Lambda(Hf)$ が続き、次に $\Gamma f$ が T で普遍的に測定可能であることがわかります (同じ参照)。すべてのメジャー $\gamma_t$ の合計質量が最大でも $\| \Lambda \| \| H \|$ に等しいことは明らかです。従って、$\Gamma g$ は普遍的に測定可能であり、すべての写像 $g \in \mathscr{K}_+(Y)$ に対して限界があります。従って、$\Gamma$ は、T 上のすべての有界メジャー、特にコンパクトなサポートを持つすべてのメジャーに対して本質的にスカラー的に積分可能です。より一般的には、$\mu$ が $\Lambda$ の領域の測度であり、H の領域に対して $\mu \Lambda$ 属するとなる場合、$g \in \mathscr{K}_+(Y)$ については、

$$
\langle \mu, \Gamma g \rangle = \langle \mu, \Lambda(Hg) \rangle = \langle \mu \Lambda, Hg \rangle = \langle (\mu \Lambda)H, g \rangle.
$$

最後の量は有限であるため、$\Gamma$ は本質的にスカラー的に $\mu$ 可積分であることがわかります。整 $\int \gamma_t d\mu(t)$ を $\mu \Gamma$ で表しましょう ($\Gamma$ が拡散であるかどうかまだわからないため、記法の乱用です)。その後、前述の関係を書き込むことができます

$$
\langle \mu \Gamma, g \rangle = \langle (\mu \Lambda)H, g \rangle,
$$

または、$\mathscr{K}_+(Y)$ では $g$ は任意であるため、$\mu \Gamma = (\mu \Lambda)H$ も使用できます。

普遍的に測定可能な写像 $f \geqslant 0$ を改めて考えてみましょう。私たちは持っています

$$
\langle \mu \Gamma, f \rangle = \langle (\mu \Lambda)H, f \rangle = \langle \mu \Lambda, Hf \rangle = \langle \mu, \Lambda(Hf) \rangle = \langle \mu, \Gamma f \rangle.
$$

$f$ が下位の半連続で、$\mu$ がコンパクトなサポートでポジティブな尺度の集合を超えるとき、これらの関係は、$\Gamma$ が Y における T の拡散であることを表します。主張は、上記の過程で得られた関係を明示するにすぎません。 証明。

#### 定義 4 {#int-v-s3-def-4 .statement tag=091O}

*記法は命題 13 の拡散であるため、拡散 $\Lambda H$ は有界拡散 H と $\Lambda$ の合成拡散 (または合成) と呼ばれます。

$X_1, X_2, X_3, X_4$ を 4 つの局所コンパクト空間と、$\Lambda_1, \Lambda_2, \Lambda_3$ 3 つの有界拡散 (それぞれ、$X_2$ の $X_1$、$X_3$ の $X_2$、$X_4$ の $X_3$) とします。提案 13 からすぐに次のことがわかります。

$$
(\Lambda_1 \Lambda_2) \Lambda_3 = \Lambda_1 (\Lambda_2 \Lambda_3).
$$

従って、これらの記法を括弧なしで拡散の合成に使用します。

#### 例 {#int-v-s3-n6-exa-1 .statement tag=091P}

$u$ を T のX への普遍的に可測な写像とし、$v$ を Y へのX の普遍的に可測な写像とします。提案 2 b) による、公式による 1 つの定義する拡散 $\Lambda$ および $H$

$$
\lambda_t = \varepsilon_{u(t)}, \quad \eta_x = \varepsilon_{v(x)};
$$

拡散 $\Gamma = \Lambda H$ は次のように与えられます。

$$
\gamma_t = \varepsilon_{(vou)(t)}.
$$

従って、拡散の合成の位数は、通常の写像の合成の位数の逆であることに注意してください。

### 練習問題 {#int-v-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
