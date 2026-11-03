---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 4
section_title: Integrable functions and sets
lang: ja
source: int-i-vi
book_pages: INT IV.32-INT IV.59, INT IV.120-INT IV.127
pdf_pages: 0139-0166, 0227-0234
extraction: ocr
subsections:
    - "no": 1
      title: Extension of the integral
      page: 32
      pdf_page: 139
    - "no": 2
      title: Properties of the integral
      page: 34
      pdf_page: 141
    - "no": 3
      title: Passage to the limit in integrals
      page: 36
      pdf_page: 143
    - "no": 4
      title: Characterizations of integrable numerical functions
      page: 37
      pdf_page: 144
    - "no": 5
      title: Integrable sets
      page: 41
      pdf_page: 148
    - "no": 6
      title: Criteria for the integrability of a set
      page: 43
      pdf_page: 150
    - "no": 7
      title: Characterization of bounded measures
      page: 46
      pdf_page: 153
    - "no": 8
      title: Integration with respect to a measure with compact support
      page: 47
      pdf_page: 154
    - "no": 9
      title: Clans and additive set functions
      page: 50
      pdf_page: 157
    - "no": 10
      title: Approximation of continuous functions by step functions
      page: 52
      pdf_page: 159
    - "no": 11
      title: Extension of a measure defined on a family of sets
      page: 53
      pdf_page: 160
statements: 63
exercises: 23
content_sha256: 759fb0d058f06d9e29bb912c7e1ccef51561f2939a9fa6d48c00fb5be0fc9c54
translated_from: content/en/int/IV/04_s4_integrable_functions_and_sets.md
translation_method: google
source_content_sha256: 66721e72e10dd21f47f9c185589d7f3417a3df9407a6866398253f6c67ed1e54
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: ca40be6ee4d31417c5bf31ebfe972726c632d5c8cba1b732f6d9670faabce5e7
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 4。 可積分関数と集合

### 1. 積分の拡大

空間 $\mathscr{L}_F^p$ の定義から、コンパクトサポートを備えた連続写像の部分空間 $\mathscr{K}_F$ が $\mathscr{L}_F^p$ (§ 3, No. 4、定義 2) で *密* であることがわかります。したがって、$\mathscr{K}_F$ で定義され、その値を *完全なハウスドルフ* トポロジベクトル空間 $G$ でとったすべての連続 (位数 $p$ の収束の位相について) 線形写像は、次の形式で *連続性によって拡張* できます。 $\mathscr{L}_F^p$ で定義された連続線形写像と $G$ の値 (GT、II, § 3, No. 6、Th. 2 および III, § 3, No. 1、提案 3)。

さて、バナッハ空間 $F$ の値を使用して、コンパクト サポートを備えたすべての連続写像 $f$ について、次のように定義しました。 III, § 3, No. 1) $F$ の元である $\mu$ に関する *整* $\mu(f) = \int f \, d\mu$ を証明しました (Ch. III, § 3, No. 2、提案 6) 不等式

$$
\left| \int f \, d\mu \right| \leqslant \int |f| \, d|\mu| = N_1(f).
$$

この不等式は、$\mathscr{K}_F$から$F$への線形写像$f \mapsto \int f \, d\mu$が、$\mathscr{K}_F$の平均収束の位相の間連続であることを証明しています。したがって、連続性によって空間 $\mathscr{L}_F^1$ 全体に拡張でき、次の定義を作成できます。

#### 定義 1 {#int-iv-s4-def-1 .statement tag=08RY}

*写像所属から $\mathscr{L}_F^1(X, \mu)$ は、測度 $\mu$* に関して積分可能であると言われます (または、再度、$\mu$ 積分可能であると言われます)。 *可積分関数 $f$ の ($\mu$ に関する) 積分は、拡大の $f$ で定義値により、線形写像の $\mathscr{L}_F^1$ $\mathscr{H}_F$ の $g \mapsto \int g\, d\mu$ に続きます。 $F$;それは再び $\mu(f)$ または $\int f\, d\mu$ または $\int f(x)\, d\mu(x)$ または $\int f\mu$ または $\int f(x)\mu(x)$ と表されます。

#### 例 {#int-iv-s4-n1-exa-1 .statement tag=08RZ}

— $X$ を *離散* 空間、$\mu$ を $X$ のメジャー、$x \in X$ ごとに集合 $\alpha(x) = \mu(\varphi_{\{x\}})$ とします。 $\mathscr{F}_F^1$ の写像は *可積分* であり、他の語 $\mathscr{L}_F^1 = \mathscr{F}_F^1$ では *可積分* です。さらに、写像 $f \in \mathscr{L}_F^1$ ごとに、

$$
\int f\, d\mu = \sum_{x \in X} \alpha(x)f(x).
$$

というのは、$f \in \mathscr{F}_F^1$ としましょう。 $|\mu|^*(|f|) = \sum_{x \in X} |\alpha(x)| \cdot |f(x)| < +\infty$ (§ 1, No. 3, *例*) があります。 $\varepsilon > 0$ ごとに、$X$ の有限部分集合 $M$ が存在します。

$$
\sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon.
$$

写像 $g$ は、点 $x \in M$ では $f$ に等しく、$|f|$ は有限であり、他の場所では 0、属するから $\mathscr{H}(X; F)$ に等しく、作成された規則によれば、

$$
|\mu|^*(|f - g|) \leq \sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon,
$$

それは$f \in \mathscr{L}_F^1$を証明します。一方で、

$$
\left| \mu(g) - \sum_{x \in X} \alpha(x)f(x) \right| \leq \sum_{x \in X - M} |\alpha(x)| \cdot |f(x)| \leq \varepsilon,
$$

よって 2 番目の主張。

他の語では、$\mu$ 可積分関数 $f$ は、族 $(\alpha(x)f(x))_{x \in X}$ が *絶対加算可能* である関数 (GT、IX, §3, No. 6) であり、整 $\int f\, d\mu$ はこの族の和です。

$\mu(f)$ は $\mathscr{L}_F^1$ で定義まで連続であり、ハウスドルフ空間でその値を取るので、属するから $\mathscr{L}_F^1$ の 0 の閉包までの写像ごとに $\mu(f) = 0$ が得られます。つまり、*無視できます*。 $f$ と $g$ が 2 つ *等しい* 可積分関数の場合、$\mu(f) = \mu(g)$ です。 他の語、$\mu(f)$ の値は、可積分関数 $f$ の類 $\tilde{f}$ にのみ依存します。それは再び$\mu(\tilde{f})$と表され、写像$\tilde{f} \mapsto \mu(\tilde{f})$は$L^1_F$から$F$への連続した線形写像です。 $F$ に値が含まれ、$X$ のほぼどこでも定義されている写像 $f$ が可積分関数と同等である場合、再び $f$ は *可積分* であると言い、$\int f\, d\mu = \mu(\tilde{f})$ と書きます。 1 つの定義するも同様に可積分関数と $\overline{\mathbf{R}}$ の値は、ほぼどこでも定義され有限であり、その積分も同様です。

### 2. 積分の性質

#### 命題 1 {#int-iv-s4-prop-1 .statement tag=08S0}

*すべての正の $\mu$ 可積分数値写像 $f$ について、*

$$
\int f\, d|\mu| = \int^* f\, d|\mu| = N_1(f) \geqslant 0.
$$

なぜなら、$\int f\, d|\mu|$ と $N_1(f)$ は $\mathscr{L}^1$ で連続しており、コンパクトなサポートを備えたすべての連続写像 $f \geqslant 0$ と等しくなります。一方、$\mathscr{L}^1$ のすべての写像 $f \geqslant 0$ は、コンパクトなサポートを備えた連続写像 $\geqslant 0$ の数列 (平均の収束という意味で) 極限です (§ 3, No. 5、提案 11)。 よって命題。

#### 系 1 {#int-iv-s4-prop-1-cor-1 .statement tag=08S1}

*すべての可積分関数 $f \in \mathscr{L}^1_F$ について、$|f|$ は積分可能であり、*

$$
\int |f|\, d|\mu| = \int^* |f|\, d|\mu| = N_1(f).
$$

私たちは提案 1 とその修正案を頻繁に使用します。 1、可積分関数 $\geqslant 0$ を扱う場合、置き換えること $\int^* f\, d|\mu|$ または $N_1(f)$ で $\int f\, d|\mu|$ に。たとえば、2 つの可積分関数 $f, g$ が *同等* であるためには、$\int |f - g|\, d|\mu| = 0$ であることが必要かつ十分です。

写像 $f$ から属するへ $\mathscr{L}^p_F$ について、写像 $|f|^{p-1} \cdot f$ 属するから $\mathscr{L}^1_F$ (§ 3, No. 8、Th. 7 コリント 1) が必要かつ十分であること、つまり、それが可積分であることを思い出します。これが「p-th 冪可積分関数」という用語の理由です。さらに：

#### 系 2 {#int-iv-s4-prop-1-cor-2 .statement tag=08S2}

*すべての写像 $f \in \mathscr{L}^p_F$ について、数値写像 $|f|^p$ は可積分可能であり、*

$$
N_p(f) = \left( \int |f|^p\, d|\mu| \right)^{1/p}.
$$

これは、$|f|$ 属するから $\mathscr{L}^p$ (§ 3, No. 5、提案 11) および公式 (2) という事実からすぐに得られます。

#### 命題 2 {#int-iv-s4-prop-2 .statement tag=08S3}

— 可積分関数 $f$ ごとに、

$$
\left| \int f \, d\mu \right| \leq \int |f| \, d|\mu|.
$$

これは、(3) と $\mathscr{L}_F^1$ での $N_1(f)$ の連続性を考慮して、不等式 (1) から極限への移行によって一気に続きます。

#### 定理 1 {#int-iv-s4-thm-1 .statement tag=08S4}

— $F$ と $G$ を 2 つのバナッハ空間、$u$ を $F$ から $G$ に連続する線形写像とします。 $F$ の値を含むすべての可積分関数 $f$ について、$u \circ f$ は可積分であり、

$$
\int u(f(x)) \, d\mu(x) = u \left( \int f(x) \, d\mu(x) \right).
$$

$u \circ f$ が可積分であることはすでにわかっています (§ 3, No. 5、Th. 4)。 関係 (6) は、恒等式の拡大の原理により、すべての $f \in \mathscr{H}_F$、拡大するからすべての可積分関数 $f$ に対して有効です。なぜなら、不等式から以下のように、$f \mapsto u \circ f$ は平均収束の位相まで連続です。 $N_1(u \circ f) \leq \|u\| \cdot N_1(f)$。

#### 系 1 {#int-iv-s4-thm-1-cor-1 .statement tag=08S5}

— $a'$ を $F$ で連続する線型形式とします。 $f$ が $F$ に値が含まれる可積分関数である場合、数値写像 $\langle f, a' \rangle$ は可積分であり、

$$
\int \langle f(x), a' \rangle \, d\mu(x) = \left\langle \int f(x) \, d\mu(x), a' \right\rangle.
$$

第 3 章で見てみましょう。 VI, § 1、エクサーズ。 7、11、12 より、無限次元バナッハ空間 $F$ に値を伴う写像 $f$ が存在し、$\langle f, a' \rangle$ は$F$ 上のすべての連続線型形式 $a'$ に対して積分可能であることがわかります。 $f$ は統合可能です。

#### 系 2 {#int-iv-s4-thm-1-cor-2 .statement tag=08S6}

— $a_k$ ($1 \leq k \leq n$) が $F$ のベクトルで、$f_k$ ($1 \leq k \leq n$) が可積数写像である場合、写像 $f = \sum_{k=1}^n a_k f_k$ は可積分であり、

$$
\int \left( \sum_{k=1}^n a_k f_k \right) d\mu = \sum_{k=1}^n a_k \int f_k \, d\mu.
$$

### 3. 積分における極限への通過

#### 命題 3 {#int-iv-s4-prop-3 .statement tag=08S7}

— $\mathscr{B}$ を $\mathscr{L}_F^1$ のフィルター 基底とします。すべての集合 $M \in \mathscr{B}$ に対して、すべての写像 $f \in M$ が $K$ でサポートされるようなコンパクト集合 $K \subset X$ が存在すると仮定します。これらの条件の下で、$\mathscr{B}$ が $X$ から $f_0$ に一様に収束する場合、写像 $f_0$ は可積分であり、

$$
\int f_0 \, d\mu = \lim_{\mathscr{B}} \int f \, d\mu .
$$

なぜなら、$\mathscr{B}$ は平均して $f_0$ に収束します (§ 3, No. 3、提案 4)。

#### 命題 4 {#int-iv-s4-prop-4 .statement tag=08S8}

— $(f_n)$ を可積分数値写像の増加する (それぞれ減少する) 数列とします。 数列の上部 (または下部) エンベロープ $f$ が積分可能であるためには、$\sup_n \int f_n \, d|\mu| < +\infty$ (それぞれ $\inf_n \int f_n \, d|\mu| > -\infty$) であることが必要かつ十分です。この場合、

$$
\int f \, d\mu = \lim_{n \to \infty} \int f_n \, d\mu .
$$

私たち極限自身も増加する数列を検討します。 数列 $g_n = f_n + f_1^-$ は増加するで、可積分関数 $\geqslant 0$ で構成されます。上部エンベロープが $g = f + f_1^-$ であるため、Th から命題が続きます。 § 3, No. 6の5。

#### 定理 2 {#int-iv-s4-thm-2 .statement tag=08S9}

— $A$ を、可算数基底のフィルタ $\mathfrak{F}$ でフィルタリングした、添字の集合とします。 $(f_\alpha)_{\alpha \in A}$ を、フィルター $\mathfrak{F}$ に関して、ほぼどこでも点的に写像 $f$ に収束する可積分関数の族とする。 $\int^* g \, d|\mu| < +\infty$ および $X$ のほぼどこでも $\alpha \in A$ に対して $|f_\alpha(x)| \leqslant g(x)$ となるような数値写像 $g \geqslant 0$ が存在する場合、写像 $f$ は可積分であり、

$$
\int f \, d\mu = \lim_{\mathfrak{F}} \int f_\alpha \, d\mu .
$$

定理は、主張の条件の下で、$f_\alpha$ が $\mathfrak{F}$ に関して$f$ に平均的に収束するため、ルベーグの定理 (§ 3, No. 7、Th. 6 の Cor.) から続きます。

#### 系 1 {#int-iv-s4-thm-2-cor-1 .statement tag=08SA}

— $\Omega$ を、次の特性を持つ $F$ に近傍の可算基本系、$X \times \Omega$ の $f$ 写像を認めるトポロジカル空間、$t_0$ 点の $\Omega$ とします。
a) $t \in \Omega$、写像 $x \mapsto f(x, t)$ ごとに可積分です。
b) $x \in X$ ごとに、写像 $t \mapsto f(x, t)$ は $t_0$ で連続します。

c) t_0 の近傍 U と、X で定義された数値写像 g \geqslant 0 が存在し、すべての $x \in X$ と $t \in U$ に対して $\int^* g d|\mu| < +\infty$ と $|\mathbf{f}(x,t)| \leqslant g(x)$ が存在します。

これら条件, 写像 $\Omega$ の F への$t \mapsto \int \mathbf{f}(x,t) d\mu(x)$ は、点 $t_0$ で連続します。

#### 系 2 {#int-iv-s4-thm-2-cor-2 .statement tag=08SB}

— $(\mathbf{f}_n)$ を可積分関数の数列として、系列と一般的な項 $\mathbf{f}_n(x)$ がほぼどこでも収束するようにします。 $\int^* g d|\mu| < +\infty$ などの写像 $g \geqslant 0$ が存在し、ほぼすべての整数 $n$、$\left| \sum_{k=1}^n \mathbf{f}_k(x) \right| \leqslant g(x)$ に対して、系列の和 $\mathbf{f}(x)$ (ほぼすべての場所で定義) と一般的な項 $\mathbf{f}_n(x)$統合可能であり、

$$
\int \mathbf{f} d\mu = \sum_{n=1}^\infty \int \mathbf{f}_n d\mu
$$

(「系列の用語ごとの統合」)。

### 4. 可積分数値写像の特徴付け

#### 命題 5 {#int-iv-s4-prop-5 .statement tag=08SC}

— 数値写像 $f \geqslant 0$ (有限であるかどうか)、X の下位半連続が可積分であるためには、$\int^* f d|\mu| < +\infty$ であることが必要かつ十分です。

結局のところ、条件で十分であるということは、証明に帰着します。 $|\mu|^*(f)$ の定義 (§ 1, No. 1、定義 1) は、すべての $\varepsilon > 0$ に対して、$g \leqslant f$ や $|\mu|^*(f) \leqslant |\mu|(g) + \varepsilon$ などのコンパクトなサポートを備えた連続的な写像 $g \geqslant 0$ が存在することを証明します。しかし、$f - g$ は下位の半連続であり、$\geqslant 0$ なので (§ 1, No. 1、Th. 2)

$$
|\mu|^*(f) = |\mu|(g) + |\mu|^*(f - g),
$$

他の語 $N_1(f - g) = |\mu|^*(f - g) = |\mu|^*(f) - |\mu|(g) \leqslant \varepsilon$ では、$f$ が可積分であることが証明されます (§ 3, No. 4、提案 7)。

#### 系 1 {#int-iv-s4-prop-5-cor-1 .statement tag=08SD}

— X 上で半連続の有限数値写像 $f \geqslant 0$ が可積分であるためには、$\int^* f d|\mu| < +\infty$ であることが必要かつ十分です。

なぜなら、$|\mu|^*(f) < +\infty$ の場合、$f \leqslant h$ と $|\mu|^*(h) < +\infty$ のような下位の半連続写像 $h$ が存在します。 $h - f$ はどこでも定義されており、下位は半連続であり、$|\mu|^*(h - f) \leqslant |\mu|^*(h) < +\infty$;したがって、$h - f$ は可積分であり、$f(x) = h(x) - (h(x) - f(x))$ はほぼどこでも可積分であるため、$f$ は可積分です。

#### 系 2 {#int-iv-s4-prop-5-cor-2 .statement tag=08SE}

— $\mathbf{H}$ を空でない集合とし、下位 (それぞれ上位) の半連続かつ積分可能な数値写像の関係 $\leqslant$ (それぞれ $\geqslant$) に向けます。もし

$$
\sup_{f \in \mathbf{H}} \int f \, d|\mu| < +\infty \quad \text{(resp. } \inf_{f \in \mathbf{H}} \int f \, d|\mu| > -\infty \text{)},
$$

その場合、$\mathbf{H}$ の上部 (または下部) エンベロープ $g$ は積分可能です。

$$
\int g \, d\mu = \lim_{f \in \mathbf{H}} \int f \, d\mu,
$$

および $\int g \, d|\mu| = \sup_{f \in \mathbf{H}} \int f \, d|\mu|$ (それぞれ $\int g \, d|\mu| = \inf_{f \in \mathbf{H}} \int f \, d|\mu|$)。

極限は、下位の半連続写像の場合に該当する可能性があります。 写像 $f^+$ (それぞれ $f^-$)、$f$ が$\mathbf{H}$ を通過すると、形有向集合が下側 (または上側) の半連続写像の $\leqslant$ (それぞれ $\geqslant$) になります。 $\geqslant 0$; $f \in \mathbf{H}$ の場合、$f^+$ (それぞれ $f^-$) の上部 (下部) エンベロープは、$g^+$ (それぞれ $g^-$) に等しくなります。 一方、$\geqslant f_0$、一部の写像、$f_0 \in \mathbf{H}$の$f \in \mathbf{H}$の切断（これと最終的なもの）、からなるのいずれかによって置き換える$\mathbf{H}$が可能です。次に$\int f^+ \, d|\mu| \leqslant \int f \, d|\mu| + \int f_0^- \, d|\mu|$;したがって、$\mathbf{H}$ が正の写像で構成される場合、系の 2 つの主張が証明に還元されることがわかります。 $\mathbf{H}$ が $\leqslant$ に向けられており、下位の半連続写像 $\geqslant 0$ で構成されている場合、次のことがわかります (§ 1, No. 1、Th. 1)。

$$
|\mu|^*(g) = \sup_{f \in \mathbf{H}} |\mu|^*(f) = \sup_{f \in \mathbf{H}} \int f \, d|\mu| < +\infty,
$$

したがって、下位の半連続である $g$ は、提案 5 によって積分可能です。 $\int g \, d|\mu| = \lim_{f \in \mathbf{H}} \int f \, d|\mu|$ があり、$f \leqslant g$ から$\lim_{f \in \mathbf{H}} N_1(g - f) = 0$ が得られます。これは、$f$ が $\mathbf{H}$ に関して平均して $g$ に収束することを示しており、したがってこの場合は系が証明されます。 $\mathbf{H}$ が $\geqslant$ に向けられており、$0 \leqslant f \leqslant f_1$ と $f_1 \in \mathbf{H}$ のような上部の半連続可積分関数 $f$ で構成されている場合、$f_1 \leqslant h$ のような下部の半連続可積分関数 $h$ が存在します。 $f = h - f'$、$f(x) < +\infty$の場合は$f'(x) = h(x) - f(x)$、それ以外の場合は$f'(x) = 0$と書くことができます。 $f'$ 形有向集合は、$\leqslant$ に対して、下半連続可積分関数 $\geqslant 0$ であることは明らかです。

$$
\int f' \, d|\mu| \leqslant \int h \, d|\mu| < +\infty;
$$

上で証明したことをそれらに当てはめることができます。 $g'$ が $f'$ の上部エンベロープである場合、$h$ と $g'$ はほぼどこでも有限であるため、$h - g'$ はほぼどこでも定義され、ほぼどこでも $g$ と等しくなります。これから、この場合、系の結論がすぐに得られます。

#### 系 3 {#int-iv-s4-prop-5-cor-3 .statement tag=08SF}

— $f$ を有界数値写像とし、$X$ で上部の半連続でコンパクトなサポートを持つものとします。すると、曖昧な位相に対して写像$\mu \mapsto \int f\, d\mu$が$\mathscr{M}_+(X)$の上半連続となります。

$h$ が $\mathscr{K}_+(X)$ の写像で、$|f| \leq h$ (Ch. III, §1, No. 2, 補題 1) である場合、$0 \leq f + h \leq 2h$ となり、$f + h$ は上部半連続であるため、Cor から続きます。 1 $f$ は、$X$ の各メジャー $\mu$ に対して $\mu$ 積分可能です。さらに$\mu(f) = \mu(h) - \mu(h - f)$と$h - f$は下位半連続写像$\geq 0$です。 写像 $\mu \mapsto \mu(h - f)$ は曖昧な位相に対して $\mathscr{M}_+(X)$ よりも低い半連続であるため (§1, No. 1、提案 4)、これは系を証明します。

#### 定理 3 {#int-iv-s4-thm-3 .statement tag=08SG}

— 数値写像 $f \geq 0$ が積分可能であるためには、すべての $\varepsilon > 0$ に対して、有限の値とコンパクトなサポートを備えた上部の半連続写像 $g \geq 0$ と、下部の半連続可積分関数が存在することが必要かつ十分です。 $h$、つまり $g \leq f \leq h$ と $\int (h - g)\, d|\mu| \leq \varepsilon$ です。

条件は、積分可能性の一般的な基準 (§3, No. 4、提案 8)、提案 5 とその系 1. 条件が必要であることを示しましょう。 $f \geq 0$ が可積分である場合、$\varepsilon > 0$ ごとに、$N_1(f - u) \leq \varepsilon/4$ などの、連続的でコンパクトなサポートを備えた写像 $u \geq 0$ が存在します。 $N_1$ の定義により、これは、$|\mu|^*(v) \leq \varepsilon/2$ と $|f - u| \leq v$ のような下位の半連続写像 $v \geq 0$ が存在することを意味します。したがって、すべての $x \in X$ に対して $-v(x) \leq f(x) - u(x) \leq v(x)$ となり、$u(x)$ はどこでも有限であるため、すべての $x \in X$ に対して $(u(x) - v(x))^+ \leq f(x) \leq u(x) + v(x)$ となります。 写像 $g = (u - v)^+$ および $h = u + v$ は要件を満たしています。

#### 系 {#int-iv-s4-n4-cor-1 .statement tag=08SH}

— すべての可積分 (それぞれ可積分と $\geq 0$) 数値写像 $f$ に対して、可積分 (それぞれ可積分、有限値をもつ) の上部半連続写像の増加する数列 $(g_n)$ が存在します。 $\geq 0$、コンパクトサポート付き)、および下部半連続可積分関数の減少列 $(h_n)$、次のようになります。
すべての $x \in X$ とすべての整数 $n$ に対して $1^\circ$ $g_n(x) \leq f(x) \leq h_n(x)$。
$2^\circ$ $f(x)$ は、ほぼどこでも数列 $(h_n)$ の下側エンベロープ $h$ と、数列 $(g_n)$ の上側エンベロープ $g$ に等しい。
$3^\circ$ $\int f\, d\mu = \lim_{n \to \infty} \int g_n\, d\mu = \lim_{n \to \infty} \int h_n\, d\mu$。

まず$f \geq 0$とします。 Thさんより3 $n$ ごとに、下側の半連続可積分関数 $v_n$ と、有限値とコンパクトなサポートを備えた上側の半連続写像 $u_n \geq 0$ が存在します。

$$
u_n \leq f \leq v_n \quad \text{and} \quad \int (v_n - u_n)\, d|\mu| \leq 1/n;
$$

設定 $g_n = \sup(u_1, u_2, \ldots, u_n)$ および $h_n = \inf(v_1, v_2, \ldots, v_n)$、数列 $(g_n)$ および $(h_n)$ は要件を満たしています。なぜなら、$g \leq f$ より、$g$ は No. 3 の命題 4 によって積分可能であり、
$$
\int (f - g_n) d|\mu| \leq \int (v_n - u_n) d|\mu| \leq 1/n
$$
私たちは持っています
$$
\int (f - g) d|\mu| = \lim_{n \to \infty} \int (f - g_n) d|\mu| = 0
$$
(No. 3、提案 4)、これは、$f$ と $g$ が同等であることを証明します。 数列 $(h_n)$ についても同様の議論があります。

$f$ が正でない場合、上記を $f^+$ と $f^-$ に適用できます。したがって、上部半連続可積分関数の 2 つの増加する数列 $(g'_n), (g''_n)$ と下部半連続の 2 つの減少列 $(h'_n), (h''_n)$ が存在します。 可積分関数、次のようになります: $1^\circ \ g'_n \leq f^+ \leq h'_n,\ g''_n \leq -f^- \leq h''_n;$
$2^\circ \ f^+$ (それぞれ $-f^-$) は、ほぼどこでも $g'_n$ の上部エンベロープおよび $h'_n$ の下部エンベロープ (それぞれ $g''_n$ の上部エンベロープおよび $h''_n$ の下部エンベロープ) と等しくなります。そして$3^\circ$:
$$
\int f^+ d\mu = \lim_{n \to \infty} \int g'_n d\mu = \lim_{n \to \infty} \int h'_n d\mu,
$$
$$
-\int f^- d\mu = \lim_{n \to \infty} \int g''_n d\mu = \lim_{n \to \infty} \int h''_n d\mu.
$$
さらに、$g'_n$ と $h''_n$ はどこでも有限であると仮定できます。したがって、数列 $g_n = g'_n + g''_n$ および $h_n = h'_n + h''_n$ が要件を満たしていることは明らかです。

#### 例 {#int-iv-s4-n4-exa-1 .statement tag=08SI}

$\mathbf{R}$ のすべてのポジティブなメジャー $\mu$ について、コンパクトなサポートを備えたすべての *ステップ写像* は $\mu$ 積分可能です。なぜなら、オープン (またはクローズ) 区間の特性写像は下側 (または上側) の半連続であり、各ステップ写像はそのような特性写像の線形結合です。その結果、$\mathbf{f}$ がコンパクトサポート (FRV、II, §1, No. 3) を備えた $\mathbf{R}$ 上の *規制* 写像である場合、サポートを備えたステップ写像 $\mathbf{g}_n$ の数列の一様極限であるため、$\mathbf{f}$ は積分可能です。固定コンパクト集合 (No. 3、提案 3) に含まれる。しかも$\int \mathbf{f}\, d\mu = \lim_{n \to \infty} \int \mathbf{g}_n\, d\mu$。

特に、$\mu$ がルベーグ測度であるとすると、コンパクトサポートを備えたすべての規制された写像 $\mathbf{f}$ について、整 $\int \mathbf{f}\, d\mu$ は FRV、II, §2, No. 1 で定義された積分 $\int_{-\infty}^{+\infty} \mathbf{f}(x)\, dx$ に等しいことがわかります。

#### 注意 1 {#int-iv-s4-n4-rem-1 .statement tag=08SJ}

$\mathbf{f}$ を、ルベーグ測度 $\mu$ に関して積分可能な $\mathbf{R}$ 上の規制された写像とします。その場合、$|\mathbf{f}|$ も可積分であり (No. 2、提案 1 の Cor. 1)、設定 $I_n = [-n, n]$, $|\mathbf{f}|$ は、規制されている写像 $|\mathbf{f}| \varphi_{I_n}$ の増加する数列の上位包絡線であるため、 $\int |\mathbf{f}|\, d\mu = \lim_{n \to \infty} \int_{-n}^{n} |\mathbf{f}(x)|\, dx$ by Th. 2/No. 3;したがって、整 $\int_{-\infty}^{+\infty} f(x) dx$ は *絶対収束* (FRV、II, §2, No. 3) です。さらに、Th の$\int f\, d\mu = \int_{-\infty}^{+\infty} f(x) dx$。 No. 3の2。逆に、$\int_{-\infty}^{+\infty} f(x) dx$ が絶対に収束すると仮定します。もう一度、Th によって。 No. 3、$\int f\, d\mu = \int_{-\infty}^{+\infty} f(x) dx$の2つ。整 $\int_{-\infty}^{+\infty} f(x) dx$ は収束しますが、完全には収束しないことに注意してください。その場合、$f$ はルベーグ測度に関して *積分可能ではありません*。

#### 注意 2 {#int-iv-s4-n4-rem-2 .statement tag=08SK}

ルベーグ測度と規制された写像に適用されると、No. 3 の提案 3 は、コンパクトな区間上の規制された写像の積分について極限に移行すると、新たに定理を生成します (FRV、II, §3, No. 1、提案 1)。規制されている写像の *数列* (または可算数の基底を持つフィルター) の場合、Th. 2 of No. 3 は、この命題を大幅に改善します。これは、コンパクトな区間上で一様に制限された規制された写像に対して、*均一* 収束の代わりに *点ごとの* 収束を使用するためです (cf. §5, No. 4、Th. 2)。ただし、非コンパクトな区間上の規制された写像の*絶対収束* 積分に対する極限への移行に関しては、Th の条件が重要であることに注意してください。 No. 3 の 2 は、考慮中の積分が *一様に収束* (FRV、II, §3, No. 2 で定義されている意味で) であることを意味しており、したがって、写像の収束に関する場合を除いて、書籍 IV (*loc. cit.*) で与えられている収束に関しては条件より改善されません。すべてのコンパクト区間で $f_\alpha$。最後に、規制された写像の *非絶対収束* 積分として与えられた移行から極限に対する条件は、この章で開発された理論の外側に残ります。

### 5. 統合可能集合

#### 定義 2 {#int-iv-s4-def-2 .statement tag=08SL}

*部分集合* $A$ *局所コンパクト空間* $X$ *測度に関して可積分であると言われる* $\mu$ *on* $X$ *(または* $\mu$*可積分である)* *特性の場合写像* $\varphi_A$ *of* $A$ *は可積分です* *有限数* $\mu(A) = \int \varphi_A\, d\mu$ *は* $A$の測度と呼ばれます。

すべての積分可能な集合 $A$、$|\mu|(A) = |\mu|^*(A)$ (No. 2、提案 1)。 集合が *無視できる* ためには、それが $|\mu|$ に関して * 測定値零であることが必要かつ十分です。

#### 命題 6 {#int-iv-s4-prop-6 .statement tag=08SM}

*有限族の和集合* $(A_i)_{1 \leq i \leq n}$ *可積分の集合は可積分*、そして

$$
|\mu| \left( \bigcup_{i=1}^n A_i \right) \leq \sum_{i=1}^n |\mu|(A_i).
$$

*さらに、* $A_i$ * がペアで互いに素である場合、*

$$
\mu \left( \bigcup_{i=1}^n A_i \right) = \sum_{i=1}^n \mu(A_i).
$$

なぜなら、$A = \bigcup_{i=1}^n A_i$ の場合、$\varphi_A = \sup \varphi_{A_i}$ であるため、(§ 3, No. 5、提案 12 の補正) $A_i$ が可積分であれば、$A$ も可積分であるからです。 関係 (13) は、関係 $|\mu|(A) = |\mu|^*(A)$ を考慮した、外側の措置 (§ 1, No. 4、提案 18) に対する類似の関係の特別なケースです。最後に、$A_i$ がペアで互いに素である場合、$\varphi_A = \sum_{i=1}^n \varphi_{A_i}$、よって (14)。

#### 命題 7 {#int-iv-s4-prop-7 .statement tag=08SN}

1° *A と B が 2 つ可積分集合で、$B \subset A$ である場合、集合 $C = A - B$ は可積分であり、*

$$
\mu(C) = \mu(A) - \mu(B).
$$

可算群集合の 2° *共通部分は可積分です。*

最初の部分は、$\varphi_C = \varphi_A - \varphi_B$ という事実から続きます。一方、$(A_n)$ が可積分集合の数列で、$A$ がその共通部分である場合、$\varphi_A = \inf_n \varphi_{A_n}$ であるため、$A$ は可積分です (No. 3、提案 4)。

#### 系 {#int-iv-s4-n5-cor-1 .statement tag=08SO}

*$(A_n)$ が可積分集合の減少列である場合、* $\mu(\bigcap_n A_n) = \lim_{n \to \infty} \mu(A_n)$ です。

なぜなら、$A = \bigcap_n A_n$ の場合、$\varphi_A$ は減少列 $(\varphi_{A_n})$ の下側包絡線です (No. 3、提案 4)。

#### 命題 8 {#int-iv-s4-prop-8 .statement tag=08SP}

*$(A_n)$ を積分可能な集合の増加する数列とします。 和集合 $A = \bigcup_n A_n$ が可積分であるためには、* $\sup_n |\mu|(A_n) < +\infty$ であることが必要かつ十分であり、*その場合*

$$
\mu(A) = \lim_{n \to \infty} \mu(A_n).
$$

というのは、可積分関数の $\varphi_{A_n}$ 形増加する数列と $\varphi_A = \sup_n \varphi_{A_n}$ です。したがって、命題は、No. 3 の提案 4 から導かれます。

#### 系 {#int-iv-s4-n5-cor-2 .statement tag=08SQ}

*$(A_n)$ を可積分集合の数列として、* $\sum_{n=1}^\infty |\mu|(A_n) < +\infty$ とします。 *和集合* $A = \bigcup_n A_n$ *可積分可能であり、*

$$
|\mu| \left( \bigcup_n A_n \right) \leq \sum_{n=1}^\infty |\mu|(A_n).
$$

$\varphi_A = \sup_n \varphi_{A_n}$ および

$$
|\mu|^*(A) \leq \sum_{n=1}^\infty |\mu|^*(A_n) = \sum_{n=1}^\infty |\mu|(A_n) < +\infty
$$

(§1, No. 4、提案 18);したがって、A は可積分であり (§3, No. 6、コリント 2 of Th. 5)、$|\mu|(A) = |\mu|^*(A)$ 以降、実際に (17) になります。

#### 命題 9 {#int-iv-s4-prop-9 .statement tag=08SR}

— $(A_n)$ を、$\sum_{n=1}^\infty |\mu|(A_n) < +\infty$ となるようなペアごとの互いに素可積分集合の数列とします。それから

$$
\mu\left(\bigcup_n A_n\right) = \sum_{n=1}^\infty \mu(A_n).
$$

というのは、$A = \bigcup_n A_n$ の場合、$\varphi_A = \sum_{n=1}^\infty \varphi_{A_n}$ となり、命題は (17) と Cor から求まります。 Thの2。 No. 3の2。

関係 (18) は、測度 $\mu$ が $X$ の可積分部分集合の集合において完全に加法であることも、というによって表現されます。

### 6. 集合の可積分性の基準

#### 命題 10 {#int-iv-s4-prop-10 .statement tag=08SS}

— $X$ の開いた (それぞれ閉じた) 集合 $A$ が可積分であるためには、$|\mu|^*(A) < +\infty$ であることが必要かつ十分です。

$\varphi_A$ は下位 (それぞれ上位) 半連続であるため、No. 4 の提案 5 とその系 1 から命題が得られます。

#### 系 1 {#int-iv-s4-prop-10-cor-1 .statement tag=08ST}

— すべてのコンパクト集合は統合可能です。比較的コンパクトなオープン集合はすべて統合可能です。

#### 系 2 {#int-iv-s4-prop-10-cor-2 .statement tag=08SU}

— $X$ のすべてのプラスの指標 $\mu$ に対して、$A \mapsto \mu^*(A)$ は $X$ の容量です (cf. GT、IX, §6, No. 9、例)。

#### 例 {#int-iv-s4-n6-exa-1 .statement tag=08SV}

$\mathbf{R}$ 上のルベーグ測度 $\mu$ の場合、提案 10 から、すべての有界開区間 $[a, b[$ は積分可能であり、測度 $b - a$ (\§1, No. 2、提案 9) を持つことがわかります。 点に減少するすべての集合はルベーグ測度では無視できるため、エンドポイント $a$ と $b$ を持つすべての区間は同じ測度 $b - a$ を持つことになります。

#### 命題 11 {#int-iv-s4-prop-11 .statement tag=08SW}

— $\mathscr{G}$ を $X$ の積分可能開集合の関係 $\subset$ に向けた集合とします。 $A = \bigcup_{G \in \mathscr{G}} G$ が可積分であるためには、$\sup_{G \in \mathscr{G}} |\mu|(G) < +\infty$ が必要かつ十分であり、その場合は $\mu(A) = \lim_\mathscr{G} \mu(G)$ と $|\mu|(A) = \sup_{G \in \mathscr{G}} |\mu|(G)$ です。

なぜなら、人は $|\mu|^*(A) = \sup_{G \in \mathscr{G}} |\mu|(G)$ (\§1, No. 2、提案 7) を知っているからです。したがって、命題は提案 10 から導かれます。

#### 系 {#int-iv-s4-n6-cor-1 .statement tag=08SX}

— $\mathfrak{F}$ を集合とし、$X$ の可積分閉集合の関係 $\supset$ に向けます。この場合、閉じた集合 $B = \bigcap_{H \in \mathfrak{F}} H$ は可積分であり、次の式が得られます。
$$
\mu(B) = \lim_{\mathfrak{F}} \mu(H) \quad \text{and} \quad |\mu|(B) = \inf_{H \in \mathfrak{F}} |\mu|(H).
$$
というのは、$H_0$ を $\mathfrak{F}$ の集合とします。 $H_0$ は積分可能であるため、積分可能な開いた集合 $U$ (§ 1, No. 4、提案 19) に含まれます。 関係 $\subset$ に向けられた開いた集合 $U \cap \mathbf{C}H$ 形集合は、$U$ に含まれ、和集合 $U \cap \mathbf{C}B$ を持ちます。したがって、提案 11 に帰着します。

#### 定理 4 {#int-iv-s4-thm-4 .statement tag=08SY}

— 集合 $A$ が積分可能であるためには、すべての $\varepsilon > 0$ に対して、積分可能な開集合 $G$ とコンパクト集合 $K$ が存在し、$K \subset A \subset G$ と
$$
|\mu|(G - K) = |\mu|(G) - |\mu|(K) \leq \varepsilon.
$$

a) $\varphi_K \leq \varphi_A \leq \varphi_G$ と $\int (\varphi_G - \varphi_K) d|\mu| \leq \varepsilon$ を意味するため、条件は *十分* です。 $\varphi_G$ と $\varphi_K$ は可積分であるため、 $\varphi_A$ (§ 3, No. 4、提案 8) も可積分です。

b) 条件は*必須*です。 $A$ が可積分である場合、$|\mu|^*(G)$ が任意に $|\mu|^*(A) = |\mu|(A)$ に近づくような開いた集合 $G \supset A$ が存在します (§ 1, No. 4、提案 19)。したがって、すべての証明は、$\varepsilon > 0$ ごとに、$|\mu|(A) - |\mu|(K) \leq \varepsilon$ となるようなコンパクトな集合 $K \subset A$ が存在するということになります。 $\varphi_A$ は可積分であるため、$f \leq \varphi_A$ と $\int (\varphi_A - f) d|\mu| \leq \varepsilon/2$ (No. 4、Th. 3) のように、上部半連続でコンパクトなサポート $S$ を備えた写像 $f \geq 0$ が存在します。 $\delta > 0$ を任意の数とし、$K$ を $f(x) \geq \delta$ となるような点 $x \in X$ の集合とする。 $K$ は閉じており、$S$ に含まれているため *コンパクト* であり、$f \leq \varphi_A$ 以降は $K \subset A$ になります。 集合 $B = A - K$ は積分可能、$f \leq \varphi_K + \delta \varphi_B$、よって
$$
\int f d|\mu| \leq |\mu|(K) + \delta \cdot |\mu|(B) \leq |\mu|(K) + \delta \cdot |\mu|(A),
$$
そして最後に
$$
|\mu|(A) \leq \int f d|\mu| + \frac{\varepsilon}{2} \leq |\mu|(K) + \delta \cdot |\mu|(A) + \frac{\varepsilon}{2},
$$
$\delta$ は任意なので、これで証明が完成します。

#### 系 1 {#int-iv-s4-thm-4-cor-1 .statement tag=08SZ}

— 集合 $A$ が可積分であるためには、すべての $\varepsilon > 0$ に対して、$|\mu|^*(A - K) \leq \varepsilon$ のようなコンパクトな集合 $K \subset A$ が存在することが必要かつ十分です。したがって、尺度 $|\mu|(A)$ は、コンパクト集合 $K \subset A$ の尺度 $|\mu|(K)$ の最高値集合になります。

定理 4 の $G$ と $K$ 満たす条件の場合、$|\mu|^*(A - K) \leq |\mu|^*(G - K) \leq \varepsilon$ であるため、条件が必要です。

条件で十分です。なぜなら、平均収束の位相に対して、$\varphi_A$ は可積分関数 $\varphi_K$ の集合 ($K$ $A$ の任意のコンパクト部分集合) の閉包にあるからです。

#### 系 2 {#int-iv-s4-thm-4-cor-2 .statement tag=08T0}

— 可積分可能なすべての集合 $A$ には、次のものが存在します。

$1^\circ$ 集合 $A_1 \supset A$、$A_1 - A$ が無視できるような可算開集合の可算共通部分。

$2^\circ$ 集合 $A_2 \subset A$、$A - A_2$ が無視できるように、ペアごとの互いに素コンパクト集合の可算和集合。

$1^\circ$ 整数 $n$ ごとに、$|\mu|(G_n) - |\mu|(A) \leq 1/n$ となるような積分可能な開いた集合 $G_n \supset A$ が存在します。 $A_1$ が $G_n$ の共通部分である場合、$|\mu|(A_1) = |\mu|(A)$ (No. 5、提案 7 の補正)、したがって、$A_1 - A$ は無視できます。

$2^\circ$ 定義する集合 $K_n$ を次のように帰納的に圧縮しましょう: $K_1 \subset A$ と $|\mu|(A - K_1) \leq 1$; $K_n \subset A - \bigcup_{i=1}^{n-1} K_i$ と $|\mu|(A \cap \mathbf{C}(\bigcup_{i=1}^{n-1} K_i) \cap \mathbf{C}K_n) \leq 1/n$ は $n > 1$ (木曜日 4)。 $A_2$ が $K_n$ の和集合である場合、$|\mu|(A_2) = |\mu|(A)$ (No. 5、提案 8)、したがって $A - A_2$ は無視できます。

#### 系 3 {#int-iv-s4-thm-4-cor-3 .statement tag=08T1}

— 有限の外側測度のすべての集合は、無視できる集合の和集合と、測度が有限である対ごとの互いに素コンパクト集合和の可算族に含まれます。

与えられた集合を可積分オープン集合含むに系を適用する 2 するだけで十分です。

#### 系 4 {#int-iv-s4-thm-4-cor-4 .statement tag=08T2}

— $X$ のオープン集合 $U$ ごとに、$|\mu|^*(U)$ はコンパクト集合 $K \subset U$ のメジャー $|\mu|(K)$ の上限です。

$|\mu|^*(U) < +\infty$ の場合、これは Th からの明らかです。 4. 次の議論は、$|\mu|^*(U) = +\infty$ の場合もカバーしています。 $X$ は局所的にコンパクトで、$U$ はオープンであるため、$\varphi_U$ は、写像の集合 $H$ $f \in \mathscr{K}_+$ の上部エンベロープであり、$f \leq \varphi_U$ と $\operatorname{Supp}(f) \subset U$ (cf. 証明 §1, No. 1、補題)、$H$ は $\leq$ に向けられているため、§1, No. 1 までに $|\mu|^*(U) = \sup_{f \in H} |\mu|(f)$ が得られます。 1; $f \in H$ と $K = \operatorname{Supp}(f)$ であれば、$f \leq \varphi_K \leq \varphi_U$ であるという事実から、系は明らかになります。

$|\mu|^*(U)$ は、$\overline{G} \subset U$ のような比較的コンパクトなオープン集合の尺度 $|\mu|(G)$ の上限でもあることに注意してください。なぜなら、$K$が$U$に含まれるコンパクトな集合である場合、$x \in K$ごとに、$\overline{V} \subset U$のような$x$の比較的コンパクトな開いた近傍$V$が存在するからです。これらの近傍の有限の数で $K$ をカバーすると、それらの和集合 $G$ は、$\overline{G} \subset U$ と $K \subset G$、よって $|\mu|(K) \leq |\mu|(G) \leq |\mu|^*(U)$ のように、比較的コンパクトで開いた集合になります。

### 7. 制限付き措置の特徴付け

#### 命題 12 {#int-iv-s4-prop-12 .statement tag=08T3}

— 局所的にコンパクトな空間 $X$ 上の測度 $\mu$ が制限されるためには (Ch. III, §1, No. 8)、 $X$ が $\mu$ に関して可積分な集合であること (または、同じことになると、すべての有限定数が可積分であること) が必要かつ十分です。 写像積分可能であること);この場合、

$$
\| \mu \| = | \mu |(X) = \int d|\mu|.
$$

なぜなら、私たちは$|\mu|^*(X) = \| \mu \|$ (§ 1, No. 2) を見てきました。したがって、命題は、No. 6 の提案 10 から導き出されます。

すべての有界測度 $\mu$ について、$\mu(X)$ は $\mu$ の総質量であると再度​​言います。

それはThから続きます。 No. 6 の 4 より、$\mu$ が制限されたメジャーである場合、$\varepsilon > 0$ ごとに、$|\mu|(CK) \leq \varepsilon$ となるようなコンパクトな集合 $K$ が存在します。

#### 命題 13 {#int-iv-s4-prop-13 .statement tag=08T4}

— $\mu$ を $X$ に限定された測定値とします。 $\mathscr{B}$ を、次のプロパティを持つ $\mathscr{L}_F^p$ のフィルター 基底とします。
$1^\circ$ 写像 $f \in M$ が $X$ で一様に境界されるような集合 $M \in \mathscr{B}$ が存在します。
$2^\circ$ $\mathscr{B}$ は、$X$ から写像 $f_0$ までのすべてのコンパクト部分集合に一様に収束します。
これら条件、$f_0$ 属する～$\mathscr{L}_F^p$、$\mathscr{B}$ は、位数 $p$～$f_0$ の平均に収束します。

まず最初に、すべての $x \in X$ とすべての写像 $f \in M$ に対して $|f(x)| \leq a$ があれば、すべての $x \in X$ に対して $|f_0(x)| \leq a$ もあることに注意してください。そうなると、すべての $\varepsilon > 0$ に対して、$|\mu|(CK) \leq \varepsilon^p$ と集合 $N \in \mathscr{B}$ のようなコンパクト集合 $K$ が存在し、すべての写像 $f \in N$、$|f(x) - f_0(x)| \leq \varepsilon(|\mu|(K))^{-1/p}$ がすべての $x \in K$ に対して存在します。さて、次のように書いてみましょう

$$
f - f_0 = (f - f_0)\varphi_K + (f - f_0)\varphi_{CK};
$$

前述のことから、$f \in M \cap N$ の場合、$N_p((f - f_0)\varphi_K) \leq \varepsilon$ と $N_p((f - f_0)\varphi_{CK}) \leq 2a\varepsilon$、よって $N_p(f - f_0) \leq (2a + 1)\varepsilon$ となり、命題が証明されます。

#### 系 {#int-iv-s4-n7-cor-1 .statement tag=08T5}

— $X$ の有界メジャー $\mu$ の場合、$X$ のすべての有界連続写像 $f$ を $F$ 属するからそれぞれの $\mathscr{L}_F^p$ ($1 \leq p < +\infty$) に変換します。

$X$ の各コンパクト部分集合 $K$ について、$M_K$ を $X$ の写像の集合を形 $hf$ の $F$ にします。ここで、$h$ は連続写像です。 $X$ を $[0, 1]$ に変換し、$K$ で 1 に等しく、コンパクトなサポートを使用します。 $\mathscr{L}_F^p$ 上の集合 $M_K$ 形フィルタ基底 $\mathscr{B}$、写像所属から $M_K$ までが一様に制限されており、$\mathscr{B}$ が以下に一様に収束することは明らかです。 $X$、よって系のすべてのコンパクト部分集合に $f$。

特に、写像 $f$ は積分可能であり、その積分 $\int f\, d\mu$ は積分 $\int h f\, d\mu$ の $\mathscr{B}$ に対して極限です。

コルを新たに入手します。 §5, No. 6 における積分可能性の一般基準の帰結としての提案 13 の。

第 4 章の記法 No. 2 の公式 (3) と (4) により、写像 $f \in \mathscr{C}^b(X; F)$、よってごとに III, §1, No. 2、$|f| \leq \|f\| \cdot 1$、

$$
N_p(f) \leq \|f\| \cdot N_p(1) = \|f\| \cdot \|\mu\|^{1/p}.
$$

特に、$p = 1$ の場合、No. 2 の公式 (5) が得られます。

$$
\left| \int f\, d\mu \right| \leq \|f\| \cdot \|\mu\|,
$$

従って、写像 $f \mapsto \int f\, d\mu$ は Banach 空間 $\mathscr{C}^b(X; F)$ 上で連続します。 $\mathscr{C}^b(X; F)$ の $\mathscr{K}(X; F)$ の閉包 $\mathscr{C}^0(X; F)$ までの制限、つまり、無限遠で点で 0 になる傾向がある連続写像の空間まで (Ch. III, §1, No. 2、提案 3)、従って、連続性により拡大になります。積分の$\mathscr{C}^0(X; F)$。

### 8. コンパクトなサポートによるメジャーに関する統合

$\mu$ を $X$ のメジャーとし、そのサポート $S = \operatorname{Supp}(\mu)$ はコンパクトです。オープン集合 $X - S$ は無視できます (§2, No. 2、提案 5)。従って、ベクトル空間 $F$ または $\overline{\mathbf{R}}$ の値を含むすべての写像 $f$ について、写像 $f$ および $f \varphi_S$ は等価です (§2, No. 4)。従って、$f$ が $\mu$ 可積分であるためには ($F$ がバナッハ空間である場合)、$f \varphi_S$ が可積分であることが必要かつ十分であり、その場合 (No. 1)

$$
\int f\, d\mu = \int f \varphi_S\, d\mu.
$$

さらに、$f$ が $S$ で制限されている場合、(20) から次のようになります。

$$
\left| \int f\, d\mu \right| \leq \|\mu\| \cdot \sup_{x \in S} |f(x)|.
$$

特に、$f$ が $X$ で連続である場合、$S$ ではすべての写像 $h \in \mathscr{K}(X; \mathbf{R})$ の $fh \in \mathscr{K}(X; F)$ が 1 に等しいため、$f$ は $\mu$ 積分可能です (Ch. III, §1, No. 2、補題 1)。より正確には:

#### 命題 14 {#int-iv-s4-prop-14 .statement tag=08T6}

— X を局所的にコンパクトな空間とし、F を 0 に減らされていない Banach 空間とします。 Xのすべての連続写像の空間$\mathscr{C}(X; F)$をコンパクトコンバージェンスの位相でFに装備します。 X の測度 $\mu$ が、$\mathscr{K}(X; F)$ の F への線形写像 $f \mapsto \int f d\mu$ が F への $\mathscr{C}(X; F)$ の連続線形写像に拡張可能であるためには、$\operatorname{Supp}(\mu)$ がコンパクトであることが必要かつ十分です。このような拡張は一意であり、No. 1 で定義された積分と一致します。

$\mu$ がコンパクトなサポートを持っている場合、整 $\int f d\mu$ がすべての写像 $f \in \mathscr{C}(X; F)$ に対して定義され、F への $\mathscr{C}(X; F)$ の写像 $f \mapsto \int f d\mu$ がコンパクト収束の位相に対して連続であることを見てきました。 逆に、コンパクト収束の位相において$\mathscr{K}(X; F)$において$f \mapsto \int f d\mu$が連続であるとします。 次に、写像 $f \in \mathscr{K}(X; F)$ ごとに $|\mu(f)| \leq a \cdot \sup_{x \in K} |f(x)|$ となるようなコンパクト集合 $K \subset X$ と数 $a > 0$ があります。特に、$g \in \mathscr{K}(X; F)$ のサポートが K と交差しない場合は、$\mu(g) = 0$ になります。 $g = h a$ を取ると、$a \neq 0$ は F のベクトルであり、$h \in \mathscr{K}(X; \mathbf{C})$ であるため、サポートが K と交差しないすべての写像 $h \in \mathscr{K}(X; \mathbf{C})$ に対して $\mu(h) = 0$ であることがわかり、$\operatorname{Supp}(\mu) \subset K$ が証明されます。 最後に、拡大の一意性は、コンパクト収束の位相に対して $\mathscr{C}(X; F)$ で $\mathscr{K}(X; F)$ が密であるという事実から導き出されます (Ch. III, §1, No. 2、提案 4)。

提案 14 により、拡大から $\mathscr{C}(X; \mathbf{C})$ までの連続するコンパクトなサポートを使用して、X 上のメジャーを識別することができます。 従って、コンパクトサポートを備えたXの小節の集合は、ハウスドルフの局所的に凸な空間$\mathscr{C}(X; \mathbf{C})$の二重$\mathscr{C}'(X; \mathbf{C})$と識別される可能性があります。 $\mathscr{C}(X; \mathbf{C})$ は完全である (GT、X, §1, No. 6、Th. 2 の Cor. 3) が、必ずしもバレル化されているわけではない (Exer. 17) ことを思い出してください。 しかし、X が無限に可算である場合、従って、$K_n \subset \overset{\circ}{K}_{n+1}$ となるようなコンパクト集合 $K_n$ の増加系列の和集合となり、$\mathscr{C}(X; \mathbf{C})$ のトポロジーは半ノルムの可算族 $p_n(f) = \sup_{x \in K_n} |f(x)|$ によって定義できます。従って、この場合 $\mathscr{C}(X; \mathbf{C})$ はフレシェ空間です。 その結果、有界の集合によって$\mathscr{C}(X; \mathbf{C})$の$\mathscr{G}$をカバーするすべてについて、空間$\mathscr{C}'(X; \mathbf{C})$は$\mathscr{G}$トポロジー（TVS、III, §4, No. 2、Th.1のCor.4）に対して準完全になります。

特に、コンパクトな収束の$\mathscr{C}'(X; \mathbf{C})$ 位相 ($\mathscr{C}(X; \mathbf{C})$ のコンパクトな部分集合に対する一様収束の位相) について検討します。 $\mathscr{C}(X; \mathbf{C})$ の比較的コンパクトな部分集合 H は次の特性 (GT、X, §2, No. 5、Th. 2 の Cor. 3) によって特徴付けられることを思い出してください。

$1^\circ$ H は等連続です。

$f$ が H を越える $f(x)$ のすべての $x \in X$、集合 $H(x)$ の $2^\circ$ は、$\mathbf{C}$ で制限されます。

#### 命題 15 {#int-iv-s4-prop-15 .statement tag=08T7}

— X を局所コンパクト空間とし、すべての $x \in X$ について、$\varepsilon_x$ を点 x でのディラック測度とする。 X から $\mathscr{C}'(X; \mathbf{C})$ への写像 $x \mapsto \varepsilon_x$ は、$\mathscr{C}'(X; \mathbf{C})$ でのコンパクトな収束の位相の間連続します。

この位相の $\mathscr{C}'(X; \mathbf{C})$ の $\varepsilon_{x_0}$ の近傍を考えます。これは、$\mathscr{C}(X; \mathbf{C})$ のコンパクトな部分集合 H である数 $\delta > 0$ を取り、次のようなコンパクトなサポートを備えた X 上のメジャー $\mu$ の集合を考慮することによって定義されると想定できます。 写像 $f \in H$ ごとに $|\mu(f) - \varepsilon_{x_0}(f)| \leq \delta$ です。 H は等連続であるため、X には $x_0$ の近傍 U が存在し、関係 $f \in H$ はすべての $x \in U$ に対して $|f(x) - f(x_0)| \leq \delta$ を暗示し、これは $|\varepsilon_x(f) - \varepsilon_{x_0}(f)| \leq \delta$ と書くこともでき、命題を証明します。(*)

#### 命題 16 {#int-iv-s4-prop-16 .statement tag=08T8}

— K を、K に含まれるサポートを持つ、X 上のメジャー $\mu$ のX、L ベクトル空間のコンパクト部分集合とします。L では、$\mathscr{C}'(X; \mathbf{C})$ でのコンパクトな収束の位相 $\mathscr{T}$ によって誘導されるトポロジーと、 位相 $\mathscr{T}'$ は、$\mathscr{M}(X; \mathbf{C})$ (Ch. III, §1, No. 10) 一致するに厳密にコンパクトに収束します。

Lでは、$\mathscr{T}$によって誘発された位相は、$\mathscr{T}'$によって誘発された位相よりもより細かいであることが明らかです。逆に、H を $\mathscr{C}(X; \mathbf{C})$ のコンパクトな部分集合とし、$\mathscr{K}(X; \mathbf{C})$ の h 写像は K の 1 に等しいとします。 写像 $fh$ の集合 H' ($f$ が H を超えている) は、$\mathscr{K}(X; \mathbf{C})$ では厳密にコンパクトであり、すべてのメジャーについて、 写像 $f \in H$、よってごとに $\mu \in L$、$\mu(f) = \mu(fh)$ の結論。

#### 系 1 {#int-iv-s4-prop-16-cor-1 .statement tag=08T9}

— X のすべてのコンパクト部分集合 K と、X 上のメジャー $\mu$ のすべての数 $a > 0$、集合 B について、$\operatorname{Supp}(\mu) \subset K$ と $\| \mu \| \leq a$ がコンパクトな $\mathscr{C}'(X; \mathbf{C})$ の等連続部分集合となる位相 $\mathscr{T}$ のコンパクト コンバージェンス用。

なぜなら、H を、K 上で一様に制限される関数で構成される $\mathscr{C}(X; \mathbf{C})$ の部分集合であるとします。 (22) により、すべての関数 $f \in H$ およびすべてのメジャー $\mu \in B$ に対して $|\mu(f)| \leq c \cdot \| \mu \| \leq ac$ となるような数 $c > 0$ が存在します。したがって、$\mathscr{C}(X; \mathbf{C})$の双対$\mathscr{C}'(X; \mathbf{C})$の$B \subset acH^\circ$は、Bの等連続性を証明します。 B が $\mathscr{T}$ に対してコンパクトであるという事実は、B 上で $\mathscr{T}$ と曖昧なトポロジーが同じトポロジーを誘導するという事実から帰結します (提案 16 と 16 章 )。 III, §1, No. 10、提案 17)、B が漠然とコンパクトであるという事実 (Ch. III, §1, No. 9、コル。提案 15 の 2 および§2, No. 2、提案 6)。

#### 系 2 {#int-iv-s4-prop-16-cor-2 .statement tag=08TA}

— コンパクトなサポートを持つすべてのメジャー (それぞれ、コンパクトなサポートを持つすべてのポジティブなメジャー) $\mu$ は、コンパクトな収束の位相 $\mathscr{T}$、メジャーの集合の$\mathscr{C}'(X; \mathbf{C})$ の閉包内にあります。

(*) 実際、写像 $x \mapsto \varepsilon_x$ は X の $\mathscr{C}'(X; \mathbf{C})$ への同型写像です (Ch. VI, §1, No. 6, 注意 1)。

ポジティブな手段）そのサポートは有限で Supp(\mu) に含まれており、ノルムは $\| \mu \|$ に等しい。

なぜなら、$\mathrm{Supp}(\nu) \subset \mathrm{Supp}(\mu)$と$\| \nu \| \leq \| \mu \|$のような措置$\nu$の集合Bでは、曖昧な位相によって引き起こされる位相は、$\mathscr{T}$によって引き起こされる位相と同一であり、したがって系は第3章から続きます。 III, §2, No. 4、コルス。 Thの2と3。 1.

### 9. クランと加法的集合写像

#### 定義 3 {#int-iv-s4-def-3 .statement tag=08TB}

*空でない集合 $\Phi$ 集合 $A$ の部分集合は、実数値写像の代数 $\mathscr{A}$ ($\mathbf{R}$ 以上) からなるが存在する場合、クランと言われます。 $A$、関係 $M \in \Phi$ と $\varphi_M \in \mathscr{A}$ は同等です。*

#### 例 {#int-iv-s4-n9-exa-1 .statement tag=08TC}

$\mu$ が局所コンパクト空間 $X$ 上の測度である場合、可積分集合形の特性写像の実数係数をもつ線形結合は、*代数* $\mathscr{A}$ です。 集合 $M, N$、写像 $\varphi_M \varphi_N = \varphi_{M \cap N}$ は可積分です (No. 5、提案 7)。その後、Defs から続きます。 2と3では、$X$の統合可能な部分集合の集合がクランです。

#### 命題 17 {#int-iv-s4-prop-17 .statement tag=08TD}

*集合 $A$ の部分集合の空でない集合 $\Phi$ がクランであるためには、次の条件を満たすことが必要かつ十分です。

(CL) *集合 $M, N$ 所属 ～ $\Phi$、 集合 $M \cup N$ および $M \cap \mathbf{C}N$ 属する ～ $\Phi$ の対ごとに。*¹

条件は、関係のおかげで *必要*です

$$
\varphi_{M \cup N} = \varphi_M + \varphi_N - \varphi_M \varphi_N , \quad \varphi_{M \cap \mathbf{C}N} = \varphi_M - \varphi_M \varphi_N .
$$

それが *十分* であることを示すために、まず、$\Phi$ の任意の 2 つの集合 $M, N$ について、$M \cap N = M \cap \mathbf{C}(M \cap \mathbf{C}N)$ 以降、$M \cap N$ 属するから $\Phi$ までであることを意味していることを観察します。 $\mathscr{E}(\Phi)$ を線形結合の集合とし、$\Phi$ の集合の特性写像の実係数とします。 $\varphi_M \varphi_N = \varphi_{M \cap N}$なので、$\mathscr{E}(\Phi)$は代数です。すべては、$M$ が $A$ の部分集合である場合、$\varphi_M = \sum_i c_i \varphi_{M_i}$ となり、$M_i$ 属するから $\Phi$ が$M \in \Phi$ であることを示すことに帰着します。これは、次の補題の結果となります。

#### 補題 {#int-iv-s4-n9-lem-1 .statement tag=08TE}

*$\Phi$ を公理 (CL) の $A$ 満たすの部分集合の空でない集合とします。 $\Phi$ の集合の有限族 $(M_i)_{1 \leq i \leq n}$ が与えられると、* が存在します。

¹ 集合 $A$ の部分集合のクラン $\Phi$ は、集合の *環* (または *ブール値環*) としても知られています。さらに、$A \in \Phi$ の場合、$\Phi$ は、集合 (cf. GT、I, §6、Exer. 20 および II, §4、Exer. 12) の *代数* (または *ブール値代数*) と呼ばれます。可算値和集合の下で閉じられたブール値代数は、*トライブ*、または *$\sigma$*-*代数* (GT、IX, §6, No. 3、定義 3) と呼ばれます。

$\Phi$ のペアごとの互いに素集合の有限族 $(N_j)_{1 \leq j \leq m}$ で、各 $M_i$ は $N_j$ の特定の数の和集合になります。

というのは、形 $\bigcap_{i=1}^n P_i$ の $2^n - 1$ 集合を考えてみましょう。ここで、$P_i = M_i$ は確かに添字 $i$、$P_i = \mathbf{C} M_i$ であり、$P_i$ の少なくとも 1 つは $M_i$ に等しいからです。これら集合をいくつかの位数に並べて$(N_j)_{1 \leq j \leq m}$ を数列とします。それらは互いに素と属するから$\Phi$のペアです。一方、家族 $(P_i)$ にとって、すべての集合 $M_k$ は集合 $N_j = \bigcap_{i=1}^n P_i$ 対応するの和集合であり、$P_k = M_k$ となり、補題が証明されます。

補題が確立され、形 $\sum_{i=1}^n c_i \varphi_{M_i}$ の各写像 ($M_i \in \Phi$ は形 $\sum_{j=1}^m d_j \varphi_{N_j}$ で、$N_j$ 属するから $\Phi$ まで) はペアで書き込まれます。 互いに素; $\varphi_M = \sum_{j=1}^m d_j \varphi_{N_j}$ の場合、添字 $j$ ごとに必然的に $d_j = 0$ または $d_j = 1$ となるため、$M$ は $N_j$ の特定の数の和集合となり、したがって属するになります。 $\Phi$。

すべてのクラン $\Phi$ の部分集合の $A$ 含む空の部分集合 $\varnothing$ の $A$。なぜなら、少なくとも 1 つの部分集合 $M \in \Phi$ が存在するため、$M - M = \varnothing$ 属するから $\Phi$ になります。 注意また、シングル部分集合 $\varnothing$ の $A$ からなるの部分集合の集合もクランです。

#### 定義 4 {#int-iv-s4-def-4 .statement tag=08TF}

*クラン $\Phi$ の部分集合 of 集合 $A$ とバナッハ空間 $F$ の場合、ステップ写像*² *$\Phi$ の集合 (または $\Phi$-ステップ) を呼び出します。 写像)、$F$ に値、形* $\sum_i a_i \varphi_{M_i}$ のすべての写像、*ここで、$a_i$ 属するから $F$、および $M_i$ から $\Phi$ です*。

$F$で値を伴う$\Phi$ステップ写像の集合$\mathscr{E}_F(\Phi)$が、$\mathbf{R}$または$\mathbf{C}$を超えるベクトル空間であることは明らかです。提案 17 で、実数値 $\Phi$ ステップ写像の集合 $\mathscr{E}(\Phi)$ が $\mathbf{R}$ 上の *代数* であることを確認しました。それは、$\Phi$の集合の特性写像によって生成された$\mathbf{R}^A$の線形部分空間でもあります。

補題までに、$\mathscr{E}_F(\Phi)$ のすべての写像は $f = \sum_j c_j \varphi_{N_j}$ として書き込まれ、$N_j \in \Phi$ はペアで互いに素になります。これから、$|f| = \sum_j |c_j| \varphi_{N_j}$ 属するから $\mathscr{E}(\Phi)$ となります。特に、$\mathscr{E}(\Phi)$ 属するから $\mathscr{E}(\Phi)$ の 2 つの写像の上の包絡線なので、$\mathscr{E}(\Phi)$ は *Riesz 空間* です。

#### 注意 {#int-iv-s4-n9-rem-1 .statement tag=08TG}

— Def. であることは容易にわかります。 4 は次と同等です: $F$ に値を含む $\Phi$ ステップ写像は写像 $f$ であり、値の有限数のみを受け取り、$F$ のすべての $a \neq 0$ に対して、 集合 $f(a)^{-1}$ 属するから $\Phi$ まで。

² 機能の説明、よって記法 $\mathscr{E}(\Phi)$ は以下の通りです。

#### 定義 5 {#int-iv-s4-def-5 .statement tag=08TH}

— *実数値写像* $\lambda$ *クランで定義* $\Phi$ *集合の部分集合* $A$ *すべての対* $M, N$ *互いに素集合の場合、加算的であると言われます所属から * $\Phi$、$\lambda(M \cup N) = \lambda(M) + \lambda(N)$。

特にこの定義から$\lambda(\varnothing) = 0$が続きます。

#### 命題 18 {#int-iv-s4-prop-18 .statement tag=08TI}

— *$\lambda$ *をクラン* $\Phi$ で定義された加法的集合写像とします。 *唯一の線型形式* (再び $\lambda$ と表記) *実数値* $\Phi$* ステップ写像* のベクトル空間* $\mathscr{E}(\Phi)$ に、*集合* $M \in \Phi$ ごとに * $\lambda(\varphi_M) = \lambda(M)$ が存在します。 *さらに、* $\lambda(M) \geqslant 0$ *すべて* $M \in \Phi$ の場合、*その後* $\lambda$ * $\mathscr{E}(\Phi)$ では正の線型形式になります。

$\Phi$ 生成するベクトル空間 $\mathscr{E}(\Phi)$ の集合の特性写像があるため、線型形式 $\lambda$ の *一意性* は明らかです。 $\lambda$ の *存在* を証明するには、$M_i$ が空でない集合所属から $\Phi$ である関係 $\sum_i c_i \varphi_{M_i} = 0$ が $\sum_i c_i \lambda(M_i) = 0$ を意味することを証明するだけで十分です。

さて、補題までに、$\Phi$ に互いに素空でない集合の有限族 $(N_j)$ が存在し、すべての添字 $i$、$\varphi_{M_i} = \sum_j a_{ij} \varphi_{N_j}$ と $a_{ij} = 0$ または $a_{ij} = 1$ が存在します。したがって、関係 $\sum_i c_i \varphi_{M_i} = 0$ は、$\sum_j \left( \sum_i c_i a_{ij} \right) \varphi_{N_j} = 0$ と書くこともでき、添字 $j$ ごとに $\sum_i c_i a_{ij} = 0$ になることを意味します。デフによる。 5、そうすると、

$$
\sum_i c_i \lambda(M_i) = \sum_j \left( \sum_i c_i a_{ij} \right) \lambda(N_j) = 0,
$$

それは$\lambda$の存在を証明します。最後に、$M \in \Phi$ ごとに $\lambda(M) \geqslant 0$ があるとします。 写像 $f \in \mathscr{E}(\Phi)$ ごとに、$f = \sum_i c_i \varphi_{M_i}$ と書くことができます。ここで、$M_i \in \Phi$ はペアごとの互いに素です。 $f \geqslant 0$ の場合、添字 $i$ ごとに $c_i \geqslant 0$ となり、$M_i$ は空でない、よって $\lambda(f) = \sum_i c_i \lambda(M_i) \geqslant 0$ になります。

### 10. 連続写像をステップ写像で近似

#### 命題 19 {#int-iv-s4-prop-19 .statement tag=08TJ}

— ** $X$ * をローカルコンパクト空間、* $\Phi$ * $X$ の部分集合のクラン、* $X$ のコンパクト部分集合の *含む集合とします。 *すべての連続写像* $f$ *of* $X$ *Banach 空間* $F$ *(それぞれ、すべての連続の実数値写像* $f \geqslant 0$ *on* $X$) *コンパクト サポート付き* $K$、*存在します数列* $(g_n)$ *of 写像の* $\mathscr{E}_F(\Phi)$ *含まれるサポート付き* $K$ *(それぞれ数列* $(g_n)$ *of 写像の* $\mathscr{E}(\Phi)$ *そのような* $0 \leqslant g_n \leqslant f$ *すべて* $n$) *一様に* $f$ *(それぞれ $f$) に収束します。

$f$ は $K$ 上で一様連続であるため、各 $M_i$ の $f$ の振動が $\leq 1/n$ となるように、コンパクトな集合 $M_i$ ($1 \leq i \leq m$) の有限数で $K$ をカバーできます。 $M_i$と$K$ 属するから$\Phi$なので、集合 $N_j \in \Phi$に$K$の分割が存在し、集合 $M_i \cap K$はそれぞれ特定の和集合になります$N_j$ の数 (No. 9、補題)。 $a_j$ を $F$ の元として、$N_j$ に $|f(x) - a_j| \leq 1/n$ が来るようにします。この場合、設定 $g_n = \sum_j a_j \varphi_{N_j}$、$|f - g_n| \leq 1/n$、よって命題があります。 $a_j = \inf_{x \in N_j} f(x)$ と $g_n = \sum_j a_j \varphi_{N_j}$ をとり、連続実数値写像 $f$ についても同様に議論します。

#### 系 1 {#int-iv-s4-prop-19-cor-1 .statement tag=08TK}

*$\mu$を$X$のメジャーとします。 空間 $\mathscr{E}_F(\Phi)$ は、空間 $\mathscr{L}_F^p$ ($1 \leq p < +\infty$) のそれぞれに密集しています。*

なぜなら、提案 19 と、コンパクトなサポート (§ 3, No. 3、提案 4) を使用した写像の一様な極限の平均収束の基準から、次の閉包における位数 $p$ の平均収束の位相に対して、$\mathscr{E}_F(\Phi)$ は密であることがわかります。コンパクトサポート付きの連続写像の空間$\mathscr{K}_F$、よって系。

#### 系 2 {#int-iv-s4-prop-19-cor-2 .statement tag=08TL}

*$X$ のすべての閉じた部分集合 $S$ について、すべての写像 $f \in \mathscr{K}(X, S; \mathbf{C})$ は、線形結合 $\sum_i \lambda_i \varphi_{K_i}$ の均一な極限です。ここで、$\lambda_i$ 属するから $\mathbf{C}$ と $K_i$ は次のとおりです。コンパクトな部分集合/$S$。*

このような線形結合の集合$\mathscr{A}$は$\mathbf{C}$-代数です。 $\Phi$ を部分集合の集合 $X$ の $M$ として、$\varphi_M \in \mathscr{A}$ とします。したがって、$\Phi$ は、元がすべて、$S$ の部分集合、含む $S$ のコンパクトな部分集合、および $\mathscr{E}_C(\Phi) \subset \mathscr{A}$ である *クラン* です。次に、提案 19 をローカルコンパクト空間 $S$ とクラン $\Phi$ に適用するだけで十分です。

#### 系 3 {#int-iv-s4-prop-19-cor-3 .statement tag=08TM}

*$\mu$ と $\nu$ が $X$ 上の 2 小節であり、$X$ の各コンパクト部分集合 $K$ に対して $\mu(K) = \nu(K)$ となる場合、$\mu = \nu$ となります。*

なぜなら、それはコルから続くからです。 $X$、$\mu$、$\nu$ のすべてのコンパクト部分集合 $S$ に対して、$\mathscr{K}(X, S; \mathbf{C})$ の同じ値を取る小節の 2 と定義。

### 11. 集合のファミリーで定義されたメジャーの拡大

$\Phi$ を局所コンパクト空間 $X$ の部分集合の空でない集合とします。 実数値関数 $M \mapsto \alpha(M)$ が定義され、$\Phi$ に $\geq 0$ が与えられると、$\Phi$ の集合が $\mu$ 積分可能であり、すべての $M \in \Phi$ に対して $\mu(M) = \alpha(M)$ となるような、$X$ に正の測度 $\mu$ が存在する条件を求めることを提案します。 極限集合 $\Phi$ が次の条件を満たす場合を考えてみましょう。

(PC_I) *$\Phi$ 属するから $\Phi$ の 2 つの集合のうち、和集合と共通部分。*

(PC_{II}) *$K \subset U$ となるX のコンパクト集合 K とオープン集合 U の各対からなるに対して、$K \subset M \subset U$ となる集合 $M \in \Phi$ が存在します。*

条件 (PC_{II}) は、$K = U = \varnothing$ を取ることで $\varnothing \in \Phi$ を意味することに注意してください。ただし、集合 $\Phi$ は必ずしもクランである必要はありません。たとえば、X のすべてのコンパクトな部分集合のうちの集合は、条件 (PC_I) および (PC_{II}) を満たしますが、一般にクランではありません。M と N がコンパクトである場合、同じことが一般に $M \cap \mathbf{C}N$ に当てはまらないからです。

加法では、$\Phi$ で定義された写像 $\alpha$ が次の条件を満たすと仮定します (問題が解を持つためには明らかに必要です)。

(PM_I) *関係 $M \subset N$ は $\alpha(M) \leq \alpha(N)$ を意味します。*
(PM_{II}) *$\Phi$、$\alpha(M \cup N) \leq \alpha(M) + \alpha(N)$ の任意の M と N に対応します。*
(PM_{III}) *関係 $M \cap N = \varnothing$ は $\alpha(M \cup N) = \alpha(M) + \alpha(N)$ を意味します。*

条件 (PM_{III}) で $N = \varnothing$ を取ると、$\alpha(\varnothing) = 0$ であると推測されます。 条件 (PM_I) は、$M \in \Phi$ ごとに $\alpha(M) \geq 0$ を示します。

#### 定理 5 {#int-iv-s4-thm-5 .statement tag=08TN}

*$\Phi$ を局所的にコンパクトな空間 X、満たす (PC_I) および (PC_{II}) の部分集合の集合とし、$\alpha$ を実数値の写像とします。 $\Phi$、満たす条件 (PM_I)、(PM_{II})、(PM_{III})。 位数では、$\Phi$ の集合が $\mu$ 可積分であり、すべての $M \in \Phi$ に対して $\mu(M) = \alpha(M)$ となるような、X に正の測度 $\mu$ が存在するということは、$\alpha$ 満たすが必要かつ十分であるということです。 加法次の条件:*

(PM_{IV}) *すべての $\varepsilon > 0$ とすべての $M \in \Phi$ には、すべての $N \in \Phi$ 満たす関係のように、コンパクト集合 $K \subset M$ とオープン集合 $U \supset M$ が存在します。 $K \subset N \subset U$、1 つは $|\alpha(N) - \alpha(M)| \leq \varepsilon$ です。*

*さらに、条件 (PM_{IV}) が満たされる場合、メジャー $\mu$ は一意です。すべてのコンパクト集合 $K$、$\mu(K) = \inf_{M \in \Phi, M \supset K} \alpha(M)$;オープンするたびに集合 $U$、$\mu^*(U) = \sup_{M \in \Phi, M \subset U} \alpha(M)$.*

条件 (PM_{IV}) は、次の 2 つの結合と同等であることに注意してください。

(PM'_{IV}) *すべての $\varepsilon > 0$ とすべての $M \in \Phi$ には、$U$、$\alpha(N) \leq \alpha(M) + \varepsilon$ に含まれるすべての $N \in \Phi$ のように、開いた集合 $U \supset M$ が存在します。
(PM''_{IV}) *すべての $\varepsilon > 0$ とすべての $M \in \Phi$ に対して、すべての $N \in \Phi$ 含む $K$、$\alpha(N) \geq \alpha(M) - \varepsilon$ のように、コンパクトな集合 $K \subset M$ が存在します。*

なぜなら、(PM'_{IV}) と (PM''_{IV}) が (PM_{IV}) を暗示していることは明らかだからです。逆に、たとえば、(PM_{IV}) が (PM'_{IV}) を意味することを示しましょう。K をコンパクト集合とし、U をオープン集合として、$P \in \Phi$ 満たすごとに $K \subset M \subset U$ と $|\alpha(P) - \alpha(M)| \leq \varepsilon$ が成り立つようにします。 $K \subset P \subset U$。次に、$N \in \Phi$と$N \subset U$なら、$M \cup N$属するから$\Phi$と$K \subset M \cup N \subset U$、よって$\alpha(M \cup N) \leq \alpha(M) + \varepsilon$と*なおさら*$\alpha(N) \leq \alpha(M) + \varepsilon$となります。

集合 $\Phi$、満たす (PC_I) および (PC_{II}) が *compact* 集合で構成されている場合、条件 (PM''_{IV}) は自明に検証され、(PM_{IV}) は次のようになります。 (PM'_{IV}) と同等になります。

条件 (PM_{IV}) は *必須*: これは Th からすぐに続きます。コンパクトな集合と開いた集合による積分可能な集合の「近似」に関するNo. 6の4。 定理のもう一方の主張を証明するには、いくつかの手順を進めます。

$\mathfrak{P}(X)$の位相の1°定義。

$X$ のコンパクト集合 $K$ とオープン集合 $U$ のすべての対 $(K, U)$ からなるを、部分集合 $M \subset X$ の $I(K, U)$ 集合で表します。 $K \subset M \subset U$; 位数において、$I(K, U)$が空でないであることは、$K \subset U$であることが必要かつ十分です。 $(K', U')$ が、コンパクト集合 $K'$ とオープン集合 $U'$ によって形成される 2 番目の対である場合、次のようになります。
$$
I(K, U) \cap I(K', U') = I(K \cup K', U \cap U').
$$
$T$ を $\mathfrak{P}(X)$ の位相とします。$K$ は $X$ のコンパクト部分集合の集合を超え、$U$ は部分集合 $I(K, U)$ の集合によって生成されます。 集合/オープン部分集合/$X$;上記により、位相 $T$ (GT、I, §1, No. 3) の$I(K, U)$ 形基底となります。

$T$ の定義は、$\mathfrak{P}(X)$ では、$X$ のコンパクトな部分集合の集合が密であることを意味していることがわかります。 条件 (PC_{II}) は、$\Phi$ が$\mathfrak{P}(X)$ で密であることを表し、条件 (PM_{IV}) は、位相に対して写像 $\alpha$ が$\Phi$ で連続であることを表します。 $T$。最後に、Th. No. 6の4は、$T$によって誘導された位相に対して、写像$M \mapsto \mu(M)$が$\mu$可積分集合の一族上で連続していることを表しています。

$\mu$の2°一意性。

部分集合 $M \subset X$ の $\overline{\Phi}$ 集合によって、$\alpha(N)$ は有限の極限に向かう傾向があり、$N$ は (位相 $T$ の場合) $M$ に向かう傾向にありますが、 $\Phi$;次に、$\overline{\Phi}$ から $\mathbf{R}$ への連続写像 $\overline{\alpha}$ を一方向のみで拡大する $\alpha$ にすることができます (GT、I, §8, No. 5、Th. 1)。要件を満たす尺度$\mu$が存在する場合、上記の注意は、$\mu$可分集合の氏族$\Psi$が$\overline{\Phi}$に含まれ、$M \in \Psi$ごとに$\mu(M) = \overline{\alpha}(M)$が含まれることを証明します。この関係は、特に $X$ のすべてのコンパクト部分集合 $M$ に当てはまり、$\mu$ の一意性が証明されます (No. 10、提案 19 の Cor. 3)。

$\alpha$の3°拡大をコンパクトな集合に。

$\mu$の存在を仮定せずに、$\alpha$から$\overline{\Phi}$の集合$\overline{\Phi}$と拡大$\overline{\alpha}$を検討していきます。まず、すべてのコンパクト集合 $K$ 属するから $\overline{\Phi}$ と $\overline{\alpha}(K) = \inf_{P \in \Phi, P \supset K} \alpha(P)$ を示します。 集合 $a = \inf_{P \in \Phi, P \supset K} \alpha(P)$; $\varepsilon > 0$ ごとに、$K \subset M$ と $\alpha(M) \leq a + \varepsilon$ のような $M \in \Phi$ が存在します。 (PM'_{IV}) までに、$U$ に含まれるすべての $N \in \Phi$ に対して、$\alpha(N) \leq \alpha(M) + \varepsilon \leq a + 2\varepsilon$ が存在するような、開いた集合 $U \supset M$ が存在します。 $K \subset N \subset U$ のようなすべての $N \in \Phi$ に対して、$a \leq \alpha(N) \leq a + 2\varepsilon$ があり、定義までに$K \in \overline{\Phi}$ と $\overline{\alpha}(K) = a$ が示されます。

この結果は、$K_1$ と $K_2$ が $K_1 \subset K_2$ となるような 2 つのコンパクトな集合である場合、$\overline{\alpha}(K_1) \leq \overline{\alpha}(K_2)$ であることがすぐに証明されます。 $K_1$ と $K_2$ が任意の 2 つのコンパクト集合である場合、(PM_{II}) により $\overline{\alpha}(K_1 \cup K_2) \leq \overline{\alpha}(K_1) + \overline{\alpha}(K_2)$ が得られます。さらに、$K_1$ と $K_2$ が互いに素である場合、$\overline{\alpha}(K_1 \cup K_2) = \overline{\alpha}(K_1) + \overline{\alpha}(K_2)$ であることがわかります。なぜなら、$K_1 \subset U_1$、$K_2 \subset U_2$ のように 2 つの互いに素オープン集合 $U_1, U_2$ が存在します (GT、II, §4、提案 4)。したがって、(PC_{II}) により、$K_1 \subset M_1 \subset U_1$ と $K_2 \subset M_2 \subset U_2$ という 2 つの集合 $M_1 \in \Phi$, $M_2 \in \Phi$ も存在します。ここで、$P$ を $\Phi$ 含む $K_1 \cup K_2$ のいずれかの集合とします。 (PC_{I}) により 2 つの集合 $P \cap M_1$ と $P \cap M_2$ 属するのうち和集合が $\Phi$ となり、この 2 つの集合が互いに素であるため、(PM_I) と(PM_{III}) の収量

$$
\alpha(P) \geq \alpha(P \cap M_1) + \alpha(P \cap M_2) \geq \overline{\alpha}(K_1) + \overline{\alpha}(K_2),
$$

それが私たちの主張を確立します。

**4° 拡大から $\alpha$ に対して開いた集合.**

ここで、オープン集合$U$から属する、そして$\overline{\Phi}$の場合、$K$が$U$のコンパクト部分集合の集合を超えるので、数の上限が必要かつ十分であることがわかります。 $\overline{\alpha}(K)$ は有限です。さらに、$\overline{\alpha}(U)$ はこの上限と等しくなります。

というのは、$U$ を $\overline{\Phi}$ に対するオープン集合所属とします。 $\varepsilon > 0$ ごとにコンパクトな集合 $K \subset U$ が存在し、集合 $M \in \Phi$ 満たす $K \subset M \subset U$ ごとに $|\overline{\alpha}(U) - \alpha(M)| \leq \varepsilon$、よって $|\overline{\alpha}(U) - \overline{\alpha}(K)| \leq \varepsilon$ が含まれます。一方、$K'$ が $U$ に含まれる任意のコンパクト集合である場合、$K \subset K \cup K' \subset U$、よって $|\overline{\alpha}(U) - \overline{\alpha}(K \cup K')| \leq \varepsilon$、したがって $\overline{\alpha}(U) \geq \overline{\alpha}(K \cup K') - \varepsilon \geq \overline{\alpha}(K') - \varepsilon$ になります。したがって、$K$ は$U$ のコンパクトな部分集合の集合を超えるので、$\overline{\alpha}(U)$ は確かに数 $\overline{\alpha}(K)$ の上限に等しい。

逆に、$U$ をオープン集合として、$b = \sup_{K \subset U} \overline{\alpha}(K) < +\infty$ ($K$ が $U$ のコンパクト部分集合の集合の上を走る) とし、$U \in \overline{\Phi}$ を示します。 $\varepsilon > 0$ ごとに、$b - \varepsilon \leq \overline{\alpha}(K) \leq b$ となるようなコンパクトな集合 $K \subset U$ が存在します。 (PM''_{IV}) によって、$K \subset M \subset U$ となるすべての集合 $M \in \Phi$ に対して、次のようなコンパクト集合 $K' \subset M$ が存在します。

$$
\alpha(M) \leq \overline{\alpha}(K') + \varepsilon \leq b + \varepsilon;
$$

したがって $b - \varepsilon \leq \alpha(M) \leq b + \varepsilon$ となり、これは $U \in \overline{\Phi}$ であることを証明します。

このオープン集合 $U \in \overline{\Phi}$ と $\overline{\alpha}(U)$ の特徴付けから、まず、$U_1$ と $U_2$ が 2 つのオープン集合で、$U_1 \subset U_2$ と $U_2 \in \overline{\Phi}$ である場合、$U_1 \in \overline{\Phi}$ と$\overline{\alpha}(U_1) \leq \overline{\alpha}(U_2)$。一方、$U_1$と$U_2$が集合所属から$\overline{\Phi}$に2つ開いている場合、$U_1 \cup U_2$と$\overline{\alpha}(U_1 \cup U_2) \leq \overline{\alpha}(U_1) + \overline{\alpha}(U_2)$にも同じことが当てはまります。なぜなら、$K$を$U_1 \cup U_2$に含まれる任意のコンパクト集合とするからです。 点 $x \in K$ ごとに、$U_1$ または $U_2$ のいずれかに含まれる$x$ のコンパクトな近傍が存在します。したがって、これらの近傍の有限の数によって $K$ をカバーできます。 $K_1$ (それぞれ $K_2$) が、$U_1$ (それぞれ $U_2$) に含まれるものの和集合である場合、$K \subset K_1 \cup K_2$、よって

$$
\overline{\alpha}(K) \leq \overline{\alpha}(K_1 \cup K_2) \leq \overline{\alpha}(K_1) + \overline{\alpha}(K_2) \leq \overline{\alpha}(U_1) + \overline{\alpha}(U_2),
$$

これにより、主張された性質が確立されます。

**$\overline{\Phi}$ および $\overline{\alpha}$ の 5° 特性。**

$\overline{\Phi}$ と $\overline{\alpha}$ の定義は、次のように変換できます ((PC_{II}) を考慮して): $M \in \overline{\Phi}$ の位数では、すべての $\varepsilon > 0$ に対して、コンパクトな集合 $K$ とオープンな集合が存在することが必要かつ十分です。 集合 $U \in \overline{\Phi}$ は $K \subset M \subset U$ と $\overline{\alpha}(U) - \overline{\alpha}(K) \leq \varepsilon$ のようになります。さらに、$\overline{\alpha}(M)$ は、オープン集合 $U \in \overline{\Phi}$ 含む $M$ の $\overline{\alpha}(U)$ の*下限*、コンパクト集合 $K \subset M$ の $\overline{\alpha}(K)$ の *上限* です。

これから、まず、$M_1, M_2$ と $M_1 \cup M_2$ 属するが $\overline{\Phi}$ になると、$\overline{\alpha}(M_1 \cup M_2) \leq \overline{\alpha}(M_1) + \overline{\alpha}(M_2)$ になると推測します。実際、$U_1$ と $U_2$ がそれぞれ $\overline{\Phi}$ 含む $M_1$ と $M_2$ の 2 つのオープン集合であり、$\overline{\alpha}(U_1) \leq \overline{\alpha}(M_1) + \varepsilon$ と $\overline{\alpha}(U_2) \leq \overline{\alpha}(M_2) + \varepsilon$ である場合、$U_1 \cup U_2$ 属するは次のようになります。 $\overline{\Phi}$、含む $M_1 \cup M_2$、そしてその結果

$$
\overline{\alpha}(M_1 \cup M_2) \leq \overline{\alpha}(U_1 \cup U_2) \leq \overline{\alpha}(U_1) + \overline{\alpha}(U_2) \leq \overline{\alpha}(M_1) + \overline{\alpha}(M_2) + 2\varepsilon,
$$

よって私たちの主張。

次に、$K$ がコンパクト集合で、$U$ が $K \subset U$ となるような $\overline{\Phi}$ のオープン集合である場合、$\overline{\alpha}(U - K) = \overline{\alpha}(U) - \overline{\alpha}(K)$ であることを示します。以上により、$\overline{\alpha}(U) \leq \overline{\alpha}(K) + \overline{\alpha}(U - K)$ となります。一方、コンパクト集合 $K' \subset U - K$ ごとに、

$$
\overline{\alpha}(K \cup K') = \overline{\alpha}(K) + \overline{\alpha}(K') \leq \overline{\alpha}(U);
$$

$U - K$ がオープンで、属するから $\overline{\Phi}$ までなので、$\overline{\alpha}(U - K)$ は $\overline{\alpha}(K')$ の上限であり、$\overline{\alpha}(K) + \overline{\alpha}(U - K) \leq \overline{\alpha}(U)$ であることがわかります。

従って、$\overline{\Phi}$ の定義は次のように表現できます。$M \in \overline{\Phi}$ を実現するには、すべての $\varepsilon > 0$ に対して、$K \subset M \subset U$ と $\overline{\alpha}(U - K) \leq \varepsilon$ のようなコンパクト集合 $K$ と開集合 $U \in \overline{\Phi}$ が存在することが必要かつ十分です。

私たちは現在、$\overline{\Phi}$ が *クラン* であり、$\overline{\alpha}$ が $\overline{\Phi}$ の *加法的集合写像* であることを証明できる立場にあります。まず、$M$ と $N$ 属するから $\overline{\Phi}$ の場合、$M \cap \mathbf{C}N$ と $M \cup N$ も同様であることを示します。 仮定までに、$\varepsilon > 0$ ごとに 2 つのコンパクトな集合 $K, K'$ と、$\overline{\Phi}$ の 2 つのオープンな集合 $U, U'$ が存在します。

$$
K \subset M \subset U,\quad K' \subset N \subset U',\quad \overline{\alpha}(U - K) \leq \varepsilon,\quad \overline{\alpha}(U' - K') \leq \varepsilon.
$$

集合 $K'' = K \cap \mathbf{C}U'$はコンパクト、集合 $U'' = U \cap \mathbf{C}K'$はオープン、属する～$\overline{\Phi}$、$K'' \subset M \cap \mathbf{C}N \subset U''$。一方、$U'' - K''$は$U \cap \mathbf{C}K$と$U' \cap \mathbf{C}K'$、よって$\overline{\alpha}(U'' - K'') \leq 2\varepsilon$の和集合に含まれており、$M \cap \mathbf{C}N \in \overline{\Phi}$であることが証明されます。同様に$U_1 = U \cup U'$はオープン、属する～$\overline{\Phi}$、$K_1 = K \cup K'$はコンパクト、$K_1 \subset M \cup N \subset U_1$はオープンです。一方、$U_1 - K_1$は$U - K$と$U' - K'$の和集合に含まれ、よっては再び$\overline{\alpha}(U_1 - K_1) \leq 2\varepsilon$、$M \cup N$属するから$\overline{\Phi}$に含まれます。最後に、$M$ と $N$ が互いに素である場合、

$$
\overline{\alpha}(K_1) = \overline{\alpha}(K) + \overline{\alpha}(K') \geq \overline{\alpha}(M) + \overline{\alpha}(N) - 2\varepsilon,
$$

従って、$\overline{\alpha}(M \cup N) \geq \overline{\alpha}(M) + \overline{\alpha}(N) - 2\varepsilon$; $\varepsilon$ は任意なので、$\overline{\alpha}(M \cup N) = \overline{\alpha}(M) + \overline{\alpha}(N)$ になります。

**6° 対策$\mu$の存在。**

No. 9 の提案 18 により、$\overline{\Phi}$ ステップ写像のベクトル空間 $\mathscr{E}(\overline{\Phi})$ に正の線型形式 $\beta$ が 1 つだけ存在し、すべての $M \in \overline{\Phi}$ に対して $\beta(\varphi_M) = \overline{\alpha}(M)$ になります。 $X$ のすべてのコンパクトなサブセット $K$ について、$K$ にサポートが含まれている $\mathscr{E}(\overline{\Phi})$ の関数の *均一な制限* の空間を $\mathscr{G}(K)$ で表します。 $\beta$ は正なので、サポートが $K$ に含まれるすべての関数 $f \in \mathscr{E}(\overline{\Phi})$ に対して $|\beta(f)| \leq \overline{\alpha}(K) \cdot \|f\|$ です。これらの関数の空間に対する $\beta$ の制限は、一様収束のトポロジーの *連続* 線形形式です。したがって、$\mathscr{G}(K)$ 上の正の連続線形形式 $\overline{\beta}_K$ に拡張できます。 さらに、$K \subset K_1$の場合、$\overline{\beta}_{K_1}$から$\mathscr{G}(K)$の制限は$\overline{\beta}_K$と同一であるため、$\mathscr{G}(K)$の和集合$\mathscr{G}$、つまりそれぞれ拡大するに正の線型形式$\overline{\beta}$が存在します。 形 $\overline{\beta}_K$。

さて、すべてのコンパクト集合属するから $\overline{\Phi}$ まで、コンパクト サポートを備えた連続実数値写像の空間 $\mathscr{H}$ は $\mathscr{G}$ の *部分空間* です (No. 10、提案 19)。したがって、プラスの線型形式 $\overline{\beta}$ の *制限* から $\mathscr{H}$ は、プラスの *メジャー* $\mu$ です。すべてのコンパクト集合 $K$、$\mu(K) = \overline{\alpha}(K)$ についてそれを示してみましょう。 $\varepsilon > 0$ ごとに、$K \subset U$、$\mu(U) \leq \mu(K) + \varepsilon$、$\overline{\alpha}(U) \leq \overline{\alpha}(K) + \varepsilon$ などのオープンな集合 $U \in \overline{\Phi}$ が存在します。 $f$ を $X$ から $[0, 1]$ への連続した写像とし、そのサポートは $U$ に含まれており、$K$ 上の $f(x) = 1$ となります (Ch. III, §1, No. 2、補題 1)。それから$\mu(K) \leq \mu(f) \leq \mu(U) \leq \mu(K) + \varepsilon$、そして一方で、

$$
\overline{\alpha}(K) = \beta(\varphi_K) \leq \overline{\beta}(f) \leq \beta(\varphi_U) = \overline{\alpha}(U) \leq \overline{\alpha}(K) + \varepsilon;
$$

$\mu(f) = \overline{\beta}(f)$ なので、$|\mu(K) - \overline{\alpha}(K)| \leq \varepsilon$ であることがわかり、$\varepsilon$ は任意であるため、$\mu(K) = \overline{\alpha}(K)$ になります。

オープン集合所属から $\overline{\Phi}$ の特徴付け、Cor と組み合わせます。 Thの4。 No. 6 の 4 は、$\overline{\Phi}$ までの開いた集合所属が $\mu$ 積分可能な開いた集合に他ならず、そのような集合 $U$ に対して、$\mu(U) = \overline{\alpha}(U)$ があることを示します。 Th. 5°で与えられたNo. 6の4と$\overline{\Phi}$の集合の特徴付けは、$\mu$積分可能な集合が$\overline{\Phi}$の集合であり、そのような集合$M$に対して、 $\mu(M) = \overline{\alpha}(M)$。最後に、(PC$_{II}$) と Cor から、オープン集合 $U$ ごとに $\mu^*(U) = \sup_{M \in \Phi, M \subset U} \alpha(M)$ がすぐに得られます。 Thの4。 No. 6 の 4 つ。

したがって、定理 5 は完全に証明されます。

#### 系 {#int-iv-s4-n11-cor-1 .statement tag=08TO}

— *X を、Borel 集合 of X、$\beta$ 写像 of $\Psi$ の可算基底、$\Psi$ 集合を含む局所コンパクト空間とします。 $[0, +\infty]$ 満たす以下条件:*

(i) *$(B_1, B_2, \ldots)$ * が互いに素ボレル集合の X の数列である場合、* $\beta(B_1 \cup B_2 \cup \ldots) = \beta(B_1) + \beta(B_2) + \ldots$。

(ii) *B が X のコンパクト部分集合である場合、* $\beta(B) < +\infty$。

*すると、X には、* $\beta(B) = \mu^*(B)$ *すべて* $B \in \Psi$ となるような唯一の肯定的な尺度 $\mu$ が存在します。

$\Phi$を$X$のコンパクト部分集合の集合とし、$\alpha$を$\beta$から$\Phi$の制限とします。その後、条件 (PC$_I$)、(PC$_{II}$)、(PM$_I$)、(PM$_{II}$)、(PM$_{III}$)、(PM$_{IV}'$) が満たされます。 $K$ を $X$ と $\varepsilon > 0$ の圧縮部分集合とします。すると、$K$は減少列の共通部分、$X$の比較的コンパクトなオープン集合の$(U_1, U_2, \ldots)$になります（GT、IX, §2, No. 5、提案7）。 $\sum_{n=1}^{\infty} \beta(U_n - U_{n+1}) = \beta(U_1 - K) < +\infty$ があるため、

$$
\beta(U_n) - \beta(K) = \beta(U_n - K) = \sum_{p=n}^{\infty} \beta(U_p - U_{p+1})
$$

$n$ が $\infty$ になる傾向があるように、0 になる傾向があります。これは、条件 $(\mathrm{PM}'_{\mathrm{IV}})$ が満たされることを証明します。 Thさんより5 では、$X$ のすべてのコンパクト部分集合 $K$ に対して $\mu(K) = \alpha(K)$ となるような、$X$ に正の尺度 $\mu$ が存在します。 $X$ のすべてのオープン集合 $U$ は、コンパクト部分集合の増加する数列の和集合であるため、$\mu^*(U) = \beta(U)$ になります。 $L$を$X$の圧縮部分集合とします。 No. 5 の提案 7 により、$L$ 形の $\mu$ 統合可能な部分集合は、$L$ の部分集合の部族になります。したがって、$B$が$L$に含まれる$\Psi$の元であれば、$B$は$\mu$可積分です。 $\varepsilon > 0$ ごとに、$K \subset B \subset U$ と $\mu^*(U) - \mu(K) \leq \varepsilon$ (No. 6、Th. 4) のように、$X$ にはコンパクトな集合 $K$ とオープンな集合 $U$ が存在します。 $\beta(U) = \mu^*(U)$ と $\beta(K) = \mu(K)$ なので、$|\mu^*(B) - \beta(B)| \leq 2\varepsilon$ であることがわかります。したがって$\beta(B) = \mu^*(B)$。最後に、$X$ のすべての Borel 集合 $C$ は、互いに素のペアの数列の和集合であり、比較的コンパクトな Borel 集合、よって $\beta(C) = \mu^*(C)$ です。 $\mu$の一意性がThから一気に続きます。 5.

### 練習問題 {#int-iv-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
