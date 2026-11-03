---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 6
section_title: Images of a measure
lang: ja
source: int-i-vi
book_pages: INT V.62-INT V.74, INT V.107-INT V.112
pdf_pages: 0317-0329, 0362-0367
extraction: ocr
subsections:
    - "no": 1
      title: Image of a positive measure
      page: 62
      pdf_page: 317
    - "no": 2
      title: Integration with respect to the image of a positive measure
      page: 64
      pdf_page: 319
    - "no": 3
      title: Properties of the image of a positive measure
      page: 65
      pdf_page: 320
    - "no": 4
      title: Image of a complex measure
      page: 68
      pdf_page: 323
    - "no": 5
      title: 'Application: change of variable in the Lebesgue integral'
      page: 69
      pdf_page: 324
    - "no": 6
      title: Decomposition into slices. Inverse image of a measure under a local homeomorphism
      page: 71
      pdf_page: 326
statements: 29
exercises: 22
content_sha256: 5285925c99703dfae749264a19c99cc28ea15a988225f1effc9f4f5bf5fef554
translated_from: content/en/int/V/06_s6_images_of_a_measure.md
translation_method: google
source_content_sha256: b4ee00e28c0ad5363315a73bf228d2a58c397d50dececefce928f935c44c92bb
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 6ae31135c0c6217fc8f187988b68c1588fe5b621fcc8e34e23e2b81848960fdf
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 6。小節の像

### 1. 前向きな措置の像

$X$ を局所的にコンパクトな空間、$\pi$ を $T$ から $X$ への $\mu$ 可測写像とする。 対 $(\pi, 1)$ が *$\mu$ 適応* (§4, No. 1) であると言うのは、というがすべての写像 $f \in \mathscr{K}(X)$, 写像 $f \circ \pi$ が *本質的に $\mu$ 可積分*であることと同等です。

#### 命題 1 {#int-v-s6-prop-1 .statement tag=094O}

*$\pi$を、局所的にコンパクトな空間$X$への$T$の$\mu$可測写像とする。次の 2 つのプロパティは同等です:*

a) *すべての写像* $f \in \mathscr{K}(X)$、$f \circ \pi$ は *本質的に* $\mu$-*積分可能*です。

b) *すべてのコンパクト集合* $K \subset X$、$\overline{\pi}^{-1}(K)$ は *本質的に* $\mu$-*積分可能*。

私たちは、a) が対 $(\pi, 1)$ が $\mu$ に適応されていることを意味していることを観察しました。従って (§ 4, No. 4, Th. 2)、すべてのコンパクト集合 $K \subset X$、写像 $\varphi_K \circ \pi = \varphi_A$ について、$A = \overline{\pi}^{-1}(K)$ は本質的に $\mu$ 可積分であり、他の語では、a) は b) を意味します。

逆に、$\overline{\pi}^{-1}(K)$ が $X$ のすべてのコンパクト部分集合 $K$ に対して本質的に $\mu$ 積分可能であると仮定し、a) が検証されることを示しましょう。確かに、$S$ を $f$ のサポートにしましょう。 $S$ はコンパクトなので、設定 $A = \overline{\pi}^{-1}(S)$ は、仮定までに、

$$
\int^\bullet |f(\pi(t))| \, d\mu(t) \leq \|f\| \int^\bullet \varphi_S(\pi(t)) \, d\mu(t) = \|f\| \int^\bullet \varphi_A(t) \, d\mu(t) < +\infty.
$$

$f \circ \pi$ は $\mu$ 可測であるため (Ch. IV, § 5, No. 3、Th. 1)、$f \circ \pi$ は本質的に $\mu$ 可積分であることがわかります (§ 1, No. 3、提案 9)。

性質 b) は明らかに次のものと同等です (従って、これは a)) とも同等です。

c) *すべての点* $x$ *of* $X$ に対して、 *近傍が存在します* $V$ *of* $x$ *そのような* $\overline{\pi}^{-1}(V)$ *本質的に* $\mu$-*積分可能*。

#### 定義 1 {#int-v-s6-def-1 .statement tag=094P}

*$\mu$ *を局所的にコンパクトな空間* $T$ に対するポジティブな尺度とします。 *写像* $\pi$ *の* $T$ *ローカルコンパクトに空間* $X$ *あると言われている* $\mu$*-適切* (*または尺度として適切* $\mu$) *対* $(\pi, 1)$ *が* $\mu$*-adapted*、*つまり* (§ 4, No. 1)、*if* $\pi$ *が* $\mu$*-測定可能であり、提案 1* の (同値) 条件を満たします。 *測定* $\int \varepsilon_{\pi(t)} \, d\mu(t)$ *on* $X$ *その後、* $\mu$ *under* $\pi$ *$\pi(\mu)$ の像と呼ばれます*。

したがって、$\nu = \pi(\mu)$ の場合、定義までに、$f \in \mathscr{K}(X)$ については、

$$
\int f(x) \, d\nu(x) = \int f(\pi(t)) \, d\mu(t).
$$

#### 注意 {#int-v-s6-n1-rem-1 .statement tag=094Q}

— 1) $\mu$ が *有界* である場合 (特に、$\mu$ がコンパクトなサポートを持っている場合)、$T$ から $X$ に入るすべての $\mu$ 可測写像は $\mu$ 適切です (Ch. IV, § 5, No. 3、Th. 1 およびNo. 6、Th 5)。

2) $\pi$ が $\mu$ 可測で、$X$ のすべてのコンパクト部分集合 $K$ について、$\overline{\pi}^{-1}(K)$ が比較的コンパクトである場合、$\pi$ は $\mu$ に適切です (Ch. IV, § 5, No. 5、Prop. 7 および No. 6、Th 5)。特に、$T$ から $X$ (GT, I, § 10, No. 2, Th. 1) へのすべての *真の* 連続写像は、$T$ のすべての肯定的な測度 $\mu$ に対して $\mu$-適切です。より具体的には、これは、$T$ から X へのすべての *同相同型* $\pi$ に当てはまります。したがって、小節$\nu = \pi(\mu)$は、$\pi$による$\mu$の輸送であるXの小節にほかなりません（Ch.III, §1, No. 3）。

3) X の位相が可算基底を許容すると仮定します。すると、提案 1 の条件 b) を満たす X への T のすべての写像 $\pi$ は、$\mu$ 測定可能であり、したがって $\mu$ が適切です。 Thを適用すれば十分です。第4章IV, §5, No. 5、観察するとでは、X は計量可能 (GT、IX, §2, No. 9、提案 16 の補正)、および X の位相と互換性のある計量については、すべての閉じたボールはコンパクトの可算な和集合である集合。

### 2. 積極的な措置の像に関する統合

$\pi$ を X への T の $\mu$ 固有の写像とし、$\nu = \pi(\mu)$ とします。 適用 §4 の結果から、次の主張が得られます。

#### 命題 2 {#int-v-s6-prop-2 .statement tag=094R}

— *すべての数値写像* $f \geqslant 0$ *上に定義* X、
$$
\int^\bullet f(x)\, d\nu(x) = \int^\bullet f(\pi(t))\, d\mu(t).
$$
(2)

これはThから続きます。 §4, No. 2 の 1 つ。

#### 系 1 {#int-v-s6-prop-2-cor-1 .statement tag=094S}

— *部分集合* A *of* X ごとに、
$$
\nu^\bullet(A) = \mu^\bullet(\pi^{-1}(A)).
$$

#### 系 2 {#int-v-s6-prop-2-cor-2 .statement tag=094T}

— *部分集合* の * X が *$\nu$ に対して局所的に無視できる* ためには、 *$\pi^{-1}(A)$ が *$\mu$ に対して *局所的に無視できる* ことが必要かつ十分です。

#### 系 3 {#int-v-s6-prop-2-cor-3 .statement tag=094U}

— *測定値* $\mu$ *が集合* M に集中している場合、*その後* $\pi(\mu)$ * は $\pi(M)$ に集中しています。

なぜなら、$N = X - \pi(M)$ の場合、$\pi^{-1}(N)$ は M と交差しないため、局所的に $\mu$ は無視でき、その結果 (Cor. 2) N は局所的に $\nu$ は無視できるからです。

#### 系 4 {#int-v-s6-prop-2-cor-4 .statement tag=094V}

— *S を *$\mu$ のサポートにしましょう。 ** $\pi$ *が連続している場合、* $\pi(\mu)$ *は* $\pi(S)$ になります。

なぜなら、それはコルから続くからです。 3 では、$\pi(\mu)$ が $\pi(S)$ に集中しているため、$S'$ が$\pi(\mu)$ のサポートである場合は、$S' \subset \pi(S)$ になります。一方、$\pi^{-1}(X - S')$ は局所的には $\mu$ 無視できるオープン集合 (Cor. 2) であるため、$\mu$ は無視できます (Ch. IV, §5, No. 2、提案 5 の Cor. 2)。従って$\pi^{-1}(X - S') \subset T - S$、従って$\pi(S) \subset S'$となり、系が証明されます。

#### 命題 3 {#int-v-s6-prop-3 .statement tag=094W}

— *写像* f *of* X *トポロジカル空間* G *が $\nu$*-可測であるためには、* $f \circ \pi$ *である* $\mu$*-可測であることが必要かつ十分である*。

§4, No. 3の提案3の明らか帰結です。

#### 系 {#int-v-s6-n2-cor-1 .statement tag=094X}

— X の部分集合 A が $\nu$ 可測であるためには、 $\pi^{-1}(A)$ が $\mu$ 可測であることが必要かつ十分です。

ただし、T の $\mu$ 可測部分集合 M の $\pi$ の下の像は、$\pi$ が連続で M が $\mu$ 無視できる場合でも、必ずしも $\nu$ 可測とは限りません (例 7 および §8、例 1)。

#### 定理 1 {#int-v-s6-thm-1 .statement tag=094Y}

— f を、$\overline{\mathbf{R}}$ の値またはバナッハ空間 F で X で定義された写像とします。 f が本質的に $\nu$ 可積分であるためには、$f \circ \pi$ が本質的に $\mu$ 可積分であることが必要かつ十分であり、その場合、

$$
\int f(x)\, d\nu(x) = \int f(\pi(t))\, d\mu(t).
$$

さらに、$\pi$ が連続的で適切であると仮定します。従って、 f が $\nu$ 可積分であるためには、 $f \circ \pi$ が $\mu$ 可積分であることが必要かつ十分です。

Thを適用すれば十分です。 §4, No. 4 の 2 つ。

#### 系 {#int-v-s6-n2-cor-2 .statement tag=094Z}

— X の部分集合 A が本質的に $\nu$ 積分可能であるためには、$\pi^{-1}(A)$ が本質的に $\mu$ 積分可能であることが必要かつ十分であり、その場合は $\nu(A) = \mu(\pi^{-1}(A))$ です。

特に、すべてのコンパクト集合 $K \subset X$、$\nu(K) = \mu(\pi^{-1}(K))$ に対して。これとコルから次のことが分かります。提案 2 の 3 は、$\mu$ がアトミック (§ 5, No. 10) であれば、$\pi(\mu) = \nu$ もアトミックであるというものです。なぜなら、M を $\mu(\{t\}) \neq 0$ となるような $t \in T$ の集合とします。 $\mu$ は M によって運ばれるため、$\nu$ は $\pi(M)$ によって運ばれます。さらに、$\pi^{-1}(x)$ 含むから M の少なくとも 1 つの点があるため、$x \in \pi(M)$ ごとに $\nu(\{x\}) = \mu(\pi^{-1}(x)) > 0$ が得られます。従って、$\nu$ は原子的です (§ 5, No. 10、提案 15)。

### 3. ポジティブ尺度の像の特性

#### 命題 4 {#int-v-s6-prop-4 .statement tag=0950}

— T、T'、T'' を 3 つの局所的にコンパクトな空間、$\mu$ T の正の測度、$\pi$ T から T' への $\mu$ 測定可能な写像、$\pi'$ T' から T'' への写像、および $\pi'' = \pi' \circ \pi$ とします。

a) $\pi$ が $\mu$-proper であると仮定し、$\mu' = \pi(\mu)$ とします。 $\pi'$が$\mu'$-適切であるためには、$\pi''$が$\mu$-適切であることが必要かつ十分であり、その場合、$\pi''(\mu) = \pi'(\pi(\mu))$（小節の像の推移性）になります。

b) $\pi'$ が連続で、$\pi''$ が $\mu$-proper であると仮定します。その場合、$\pi$は$\mu$-適切、$\pi'$は$\pi(\mu)$-適切、そして$\pi''(\mu) = \pi'(\pi(\mu))$です。

a)の仮説のもとでは、$\pi''$が$\mu$可測であるためには、$\pi'$が$\mu'$可測であることが必要かつ十分である(No. 2、提案3)。一方、$K$ が $T''$ の圧縮部分集合である場合、$\pi''(K) = \pi^{-1}(\pi'(K))$ になります。 $\pi''(K)$ が本質的に $\mu$ 積分可能であるためには、$\pi'(K)$ が本質的に $\mu'$ 積分可能であることが必要かつ十分である、と Cor. Thの。 1. 最後に、$\pi''$ が $\mu$ 適切である場合、設定 $\mu'' = \pi''(\mu)$、写像 $f \in \mathscr{H}(T'')$ ごとに、

$$
\int f(t'')\, d\mu''(t'') = \int f(\pi''(t))\, d\mu(t)
$$
$$
= \int f\left(\pi'\left(\pi(t)\right)\right)\, d\mu(t) = \int f(\pi'(t'))\, d\mu'(t')
$$

Th 著No. 2 の 1。これで a) の証明が完了します。

b) の仮説の下で、$K'$ を $T'$ の圧縮部分集合とする。この場合、$K'' = \pi'(K')$ はコンパクトであるため、$\pi''(K'')$ は本質的に $\mu$ 積分可能であり、したがって $\pi^{-1}(K') \subset \pi''(K'')$ は本質的に $\mu$ 積分可能 (Ch. IV, §5, No. 5、提案 7)、したがって $\pi$ は $\mu$ 固有となります。 証明は、主張の適用部分 a) によって終了します。

#### 系 {#int-v-s6-n3-cor-1 .statement tag=0951}

*$T$と$T'$を2つの局所的にコンパクトな空間、$\mu$を$T$の正の測度、$\pi$を$T$の$T'$への全単射写像、そして$\pi^{-1}$をその逆とする写像。 $\pi$ が $\mu$-proper であると仮定し、$\mu' = \pi(\mu)$ とします。したがって、$\pi^{-1}$ は $\mu'$-proper であり、$\pi^{-1}(\pi(\mu)) = \mu$ です。*

#### 命題 5 {#int-v-s6-prop-5 .statement tag=0952}

*$T$と$X$を局所的にコンパクトな2つの空間、$\mu$を$T$、$\pi$を$T$の$\mu$-適切な写像を$X$、$g$有限数値にするとします。 写像 $\geqslant 0$、$X$ で定義され、$g \circ \pi$ は$\mu$ に対してローカルに積分可能です。 位数では、$g$ が $\pi(\mu)$ に対して局所的に可積分可能であること、$\pi$ が測度 $(g \circ \pi) \cdot \mu$ に対して適切であることが必要かつ十分であり、その場合*

$$
\pi((g \circ \pi) \cdot \mu) = g \cdot \pi(\mu).
$$

集合 $\nu = \pi(\mu)$。 $g$ が局所的に $\nu$ 積分可能であるためには、$gf$ がすべての写像 $f \in \mathscr{H}(X)$ に対して $\nu$ 積分可能であることが必要かつ十分です。 $gf$ はコンパクトなサポートを持っているため、$gf$ は本質的に $\nu$ 積分可能であると言えることになり、これは $(g \circ \pi)(f \circ \pi)$ が本質的に $\mu$ 積分可能であるというと同等になります (Th. 1)。しかし、Thによる。 §5, No. 3の1、これは$f \circ \pi$が本質的に$\rho = (g \circ \pi) \cdot \mu$に対して可積分であることを意味し、定義により、これは$\pi$が$\rho$-適切であることを示します（$\pi$は明らかに$\rho$可測であるため）。さらに、

$$
\int fg\, d\nu = \int f(\pi(t))g(\pi(t))\, d\mu(t) = \int f(\pi(t))\, d\rho(t)
$$

(No. 2、Th. 1 および §5、Th. 1)、これは関係 (4) を証明します。

#### 命題 6 {#int-v-s6-prop-6 .statement tag=0953}

— T と X を、局所的にコンパクトな 2 つの空間、$(\lambda_\alpha)_{\alpha \in A}$ 、関係 $\leq$ に向けられた T 上の積極的な措置のファミリーとし、$\mathscr{M}(T)$ で最高値 $\mu$ を認めます。 X への T の写像 $\pi$ が $\mu$-proper であるという位数では、それがすべての $\alpha \in A$ に対して $\lambda_\alpha$-proper であること、そして族 $(\pi(\lambda_\alpha))_{\alpha \in A}$ が $\mathscr{M}(X)$ で上に境界づけられることが必要かつ十分です。この場合、

$$
\pi(\mu) = \sup_\alpha \pi(\lambda_\alpha).
$$

$\pi$ が $\mu$ 測定可能であるためには、 $\pi$ がすべての $\alpha \in A$ に対して $\lambda_\alpha$ 測定可能であることが必要かつ十分である (§ 1, No. 4、提案 11 の訂正 2)。この条件が満たされると仮定します。 $\pi$ が $\mu$ であると言うのは、写像 $f \in \mathscr{K}_+(X)$ ごとに、というと同等になります。

$$
\mu^\bullet(f \circ \pi) < +\infty.
$$

さて、

$$
\int^\bullet (f \circ \pi)\, d\mu = \sup_\alpha \int^\bullet (f \circ \pi)\, d\lambda_\alpha = \sup_\alpha \int^\bullet f\, d(\pi(\lambda_\alpha))
$$

(§ 1, No. 4、提案 11);したがって、家族 $(\pi(\lambda_\alpha))$ が $\mathscr{M}(X)$ の最高値 $\theta$ を認めた場合にのみ、最初のメンバーはすべての $f \in \mathscr{K}_+(X)$ に対して有限になります。その場合、$\int (f \circ \pi)\, d\mu = \int f\, d\theta$、関係は (5) に相当します。

#### 系 1 {#int-v-s6-prop-6-cor-1 .statement tag=0954}

— $(\mu_\alpha)_{\alpha \in A}$ を、$\mu = \sum_{\alpha \in A} \mu_\alpha$ のような、T に関する肯定的な測度の合計可能な族とします。 T の写像 $\pi$ を局所的にコンパクトな空間 X に変換する場合、$\mu$-proper であるためには、すべての $\alpha \in A$ に対して $\mu_\alpha$-proper であり、族 $(\pi(\mu_\alpha))_{\alpha \in A}$ が合計可能であることが必要かつ十分です。この場合、

$$
\pi(\mu) = \sum_{\alpha \in A} \pi(\mu_\alpha).
$$

#### 系 2 {#int-v-s6-prop-6-cor-2 .statement tag=0955}

— T と X を、T のポジティブ測度の局所的にコンパクトな 2 つの空間、$(\lambda_i)_{1 \leq i \leq n}$ 有限列とし、$\mu = \sum_{i=1}^n \lambda_i$ とします。 X への T の写像 $\pi$ が $\mu$-適切であるためには、すべての添字 i について $\lambda_i$-適切であることが必要かつ十分であり、その場合

$$
\sum_{i=1}^n \pi(\lambda_i) = \pi\left( \sum_{i=1}^n \lambda_i \right).
$$

### 4. 複雑なメジャーの像

$\theta$ を $T$ の複素測度とし、$\pi$ を $T$ の写像として局所的にコンパクトな空間 $X$ にします。 $\pi$ は $\theta$ 可測であり、それぞれの $f \in \mathscr{K}(X; \mathbf{C})$、$f \circ \pi$ は本質的に $\theta$ 可積分であると仮定します。 写像が $\theta$ または $|\theta|$ に関して可測（本質的に可積分）であると言うのと同じなので、これは $\pi$ が $|\theta|$ に固有であることを意味します。 $f \in \mathscr{K}(X; \mathbf{C})$の場合、

$$
\left| \int (f \circ \pi) \, d\theta \right| \leq \int (|f| \circ \pi) \, d|\theta| ;
$$

$\mathscr{K}(X; \mathbf{C})$ の線型形式 $f \mapsto \int (f \circ \pi) \, d\theta$ が $X$ では *複雑な測定* であることがすぐにわかります (Ch. III, §1, No. 3、提案 6)、次の定義を作ることができます。

#### 定義 2 {#int-v-s6-def-2 .statement tag=0956}

*$\theta$ を局所的にコンパクトな空間 $T$ 上の複素測度とする。 $T$ の写像 $\pi$ を局所的に圧縮した空間 $X$ が $|\theta|$-proper である場合、$\theta$-proper であると言われます。次に、メジャー $f \mapsto \int (f \circ \pi) \, d\theta$ は、$\pi$ の下で $\theta$ の像と呼ばれ、$\pi(\theta)$.* と表示されます。

関係 (7) は次の形に代入できます。

$$
|\pi(\theta)| \leq \pi(|\theta|) .
$$

$T$ 空間を 2 点 $a, b$ に減じ、$\theta$ を$\varepsilon_a - \varepsilon_b$ に、$\pi$ を定数とするとすぐにわかるように、$\theta$ が零でなくても、$\pi(\theta)$ は零になる可能性があります。 写像。

$\theta$ と $\theta'$ を $T$ の 2 つの複素メジャーとします。 $\pi$ が $\theta$-proper および $\theta'$-proper である場合、それは Cor から続きます。提案 6 の 2 は、$|\theta + \theta'| \leq |\theta| + |\theta'|$ 以来、$\pi$ は $(\theta + \theta')$ であり、明らかに $\pi(\theta + \theta') = \pi(\theta) + \pi(\theta')$ です。

特に、$\theta$ が実際の尺度であり、$\pi$ が $\theta$-proper である場合、

$$
\pi(\theta) = \pi(\theta^+) - \pi(\theta^-) .
$$

拡大するに確立された複数の結果を同時に複雑な対策に適用します。その中で最も重要なものを引用します。

#### 命題 7 {#int-v-s6-prop-7 .statement tag=0957}

*$\theta$を$T$、$\pi$、$T$の$\theta$適切な写像を局所的にコンパクトな空間$X$、$\nu$像メジャー$\pi(\theta)$に複素メジャーとします。

a) $A$ を $X$ の部分集合とします。 $\overline{\pi^{-1}}(A)$ が局所的に $\theta$ で無視できる場合、$A$ は局所的に $\nu$ で無視できます。

b) $f$ を $X$ の写像としてトポロジカル空間にします。 $f \circ \pi$ が $\theta$ 測定可能である場合、 $f$ は $\nu$ 測定可能です。*

c) $f$ を $X$ で定義された写像とし、値を Banach 空間 $F$ に含めます。 $f \circ \pi$ が本質的に $\theta$ 可積分である場合、$f$ は本質的に $\nu$ 積分可能であり、

$$
\int f(\pi(t))\ d\theta(t) = \int f(x)\ d\nu(x).
$$

公式 (8) を考慮すると、これらの結果は Cor.提案 2 の 2、提案 3 から、および Th から。 No. 2 の 1。

### 5. 応用: ルベーグ積分の変数の変更

I を $\mathbf{R}$ の区間 (有界かどうか)、$a$ をその左端点、$\overline{\mathbf{R}}$ の右端点を $b$、I のルベーグ測度を $\mu$ とします。すべての $\mu$ 積分可能関数 $f$ とすべての区間 $H \subset I$ について、左端点 $\alpha$ と右端点 $\beta$ を使用して、$\int_H f(t)\ dt = \int_H f\ d\mu$ の代わりに $\int_{\alpha}^{\beta} f(t)\ dt$ と書き、集合 $\int_{\beta}^{\alpha} f(t)\ dt = -\int_{\alpha}^{\beta} f(t)\ dt$ とします。このようにしてこれらのシンボル一致するに与えられた意味は、$f$ がコンパクトなサポートを備えた規制された写像である場合に、FRV、II, §§1、および 2 に帰属するものとなります (Ch. IV, §4, No. 4、例)。

$g$ を、I で定義された数値写像とし、*局所的に $\mu$* 積分可能、I の $x_0$ 点とします。 $x \in I$、集合ごとに

$$
G(x) = c + \int_{x_0}^{x} g(t)\ dt \quad (c \text{ a constant}).
$$

数字の写像 G は I に *連続* します。これは、ルベーグの定理 (Ch. IV, §4, No. 3、Th. 2 の Cor. 1) からすぐに続きます。$g$ の積と、エンドポイント $x$ と $x+h$ を持つ区間の特性写像は、無視できるほど小さい傾向があるためです。 写像は $h$ として 0 になる傾向があります。したがって、G(I) は $\mathbf{R}$ の *区間* です。この番号全体を通して、G を局所的にコンパクトな空間 G(I) 上の I の写像とみなします。 I のメジャー $g \cdot \mu$ を $\lambda$ で示します。

まず、$g$ が $\mu$*可積分*であると仮定します。次に、上記と同じ推論は、極限 $G(a+)$ と $G(b-)$ が存在し、*有限*であることを示します。さらに、メジャー $|\lambda|$ は *有界* (§5, No. 3、Th. 1 の Cor.) であり、I の G(I) への写像 G は *$\lambda$*-proper です。

#### 命題 8 {#int-v-s6-prop-8 .statement tag=0958}

*g が $\mu$* 可積分であるとします。 J がエンドポイント $G(a+)$ と $G(b-)$ を持つ $\mathbf{R}$ のオープン区間を表す場合、メジャー $g \cdot \mu$ の G の下の像は、$G(a+) \leq G(b-)$ の場合はメジャー $\varphi_J \cdot \nu$ であり、$G(a+) \geq G(b-)$ の場合はメジャー $-\varphi_J \cdot \nu$ です (ここで$\nu$ は G(I)) のルベーグ測度を示します。*

写像 $f \in \mathscr{K}(G(I))$ ごとに、

$$
\int_{G(a+)}^{G(b-)} f(\xi) d\xi = \int_a^b f(G(t))g(t)\,dt.
$$

さて、この公式はすでに$g \in \mathscr{K}(I)$(FRV,II, §2, No. 1,公式(1))について証明されています。一般的なケースに移りましょう。 $\mathscr{K}(I)$ には写像の数列 $(g_n)$ が存在し、次のようになります: $1^\circ$ 数列 $(g_n(t))$ は $I$ のほぼどこでも $g(t)$ になる傾向があります。 $2^\circ$ すべての $n$ に対して $|g_n| \leq h$ となるような $\mu$ 可積分関数 $h \geq 0$ が存在します (Ch. IV, §3, No. 4、Th. 3)。ルベーグの定理から、設定 $G_n(x) = c + \int_{x_0}^x g_n(t)\,dt$、数列 $(G_n)$ は$I$ で$G$ に一様に収束し、数 $G_n(a+)$ と $G_n(b-)$ は次の傾向になることがすぐにわかります。それぞれ$G(a+)$と$G(b-)$に。 $f'$ を $\mathscr{K}(\mathbf{R})$ の写像として、拡大する $f$ とします。上記は、$f'(G_n(t))$ がすべての $t \in I$ に対して $f'(G(t)) = f(G(t))$ になる傾向があることを証明しています。 適用ルベーグの定理を見ると、公式 (12) は公式の結果であることがわかります。

$$
\int_{G_n(a+)}^{G_n(b-)} f'(\xi)\,d\xi = \int_a^b f'(G_n(t))g_n(t)\,dt
$$

極限までの通路で。

#### 系 {#int-v-s6-n5-cor-1 .statement tag=0959}

*$\overline{\mathbf{R}}$ またはバナッハ空間の値を持つ、$G(I)$ で定義された関数 $\mathbf{f}$ が、ルベーグ測度の$I$ で関数 $t \mapsto \mathbf{f}(G(t))g(t)$ が積分可能である場合、ルベーグ測度の$\mathbf{f}$ は、$J$ で積分可能であり、*

$$
\int_{G(a+)}^{G(b-)} \mathbf{f}(\xi)\,d\xi = \int_a^b \mathbf{f}(G(t))g(t)\,dt
$$

(ルベーグ積分の変数の変更に対して公式)。

なぜなら、$\mathbf{f}(G(t))$ は測度 $|g|\cdot\mu$ に対して積分可能であるため、測度 $g^+\cdot\mu$ と $g^-\cdot\mu$ に対しても可積分です。それはThから導かれます。 1 (No. 2) $\mathbf{f}$ は、$G(g^+\cdot\mu)$ と $G(g^-\cdot\mu)$ の測度像に対して可積分であるため、測度 $\varphi_J \cdot \nu$ に対しても可積分可能であり、提案 8 と公式 (9) を考慮すると、(13) が成り立ちます。

$\mathbf{f}$ はルベーグ測度の $J$ では可積分可能ですが、$t \mapsto \mathbf{f}(G(t))g(t)$ はルベーグ測度の $I$ では可積分できないことが起こります (Exer. 10)。

ここで、$g$ がほぼどこでも *定数符号* を維持している (そして局所的には $\mu$ 可積分である) と仮定します。たとえば、$I$ のほぼどこでも $g(t) \geq 0$ であると考える人もいるかもしれません。この場合、$G$ は $I$ で増加する連続写像であるため、$G(a+)$ と $G(b-)$ が存在します (ただし、無限である可能性があります)。さらに、$G$ は、$I$ の $G(I)$ への *$\lambda$ 固有* 写像です。つまり、$G(b-) \in G(I)$ の場合、$G$ が $x \geq x_1$ に対して定数であるような $x_1 \geq x_0$ があり、次の場合に逆像コンパクトな区間 $[G(x_0), G(b-)]$ の $G$ は $\lambda$ に統合可能です。逆に、$G(b-) \notin G(I)$ の場合、$G(I)$ に含まれる左端点 $G(x_0)$ を持つすべてのコンパクト区間の $G$ の下の逆像は、コンパクト区間と最大で $\lambda$ 無視できる程度の区間の差です。右端点 $G(x_0)$、よっての主張を持つコンパクト区間についても同様に議論できます。さらに:

#### 命題 9 {#int-v-s6-prop-9 .statement tag=095A}

*$g \geq 0$ とローカルで $\mu$ が積分可能であると仮定します。すると、正の測度$g \cdot \mu$の$G$の下の像は、$G(I)$のルベーグ測度です。 $G(I)$ で定義された写像 $f$ が、$\overline{\mathbf{R}}$ の値またはバナッハ空間でルベーグ測度の $G(I)$ で積分可能であるためには、写像 $t \mapsto f(G(t))g(t)$ が積分可能であることが必要かつ十分ですルベーグ測度の $I$ では、関係 (13) が成り立ちます。*

主張の最初の部分は、公式 (12) がすべての写像 $f \in \mathscr{K}(G(I))$ に対して有効であるという事実から導かれます。なぜなら、写像 $t \mapsto f(G(t))$ のサポートは、上記の注意のおかげで、$g$ が可積分である区間 $K \subset I$ に含まれており、$K$ に提案 8 を適用するだけで十分です。 2番目の部分はThの帰結です。 No. 2の1。

### 6. 分解をスライスします。局所準同型性のもとでの測度の逆像

$X$ をローカル コンパクト空間、$\pi$ 写像を $X$ のローカル コンパクト空間 $T$、$\mu$ を $T$、$\Lambda : t \mapsto \lambda_t$ の正の尺度として本質的にスカラー的に定義します。 $\mu$-積分可能で漠然と $\mu$-$T$ の写像を $\mathscr{M}_+(X)$ に測定可能。 $\nu = \int \lambda_t d\mu(t)$ にしましょう。 $\lambda_t$ が $t \in T$ ごとに $\overline{\pi}^{-1}(t)$ によって*運ばれる*場合、等式 $\nu = \int \lambda_t d\mu(t)$ は、$\pi$ に対する $\nu$ の *分解のスライス* (または *崩壊*) であると言われます。この概念については、第 3 章で詳しく説明します。 VI。

#### 命題 10 {#int-v-s6-prop-10 .statement tag=095B}

※上記記法において、$\pi$が$\nu$可測であるとします。 $g$ を $T$ に写像 $t \mapsto \lambda_t^*(1)$ とします。 $\pi$ が $\nu$-適切であるためには、$g$ がローカルで $\mu$-積分可能であることが必要かつ十分であり、その場合*

$$
\pi(\nu) = g \cdot \mu.
$$

まず、仮定で、$g$ は局所的に有限である、$\mu$ ほぼどこでも、有限であると主張します。 証明の最後に、この補助文字仮定を削除します。 $\pi$ は仮定 $\nu$ によって測定可能であるため、$\pi$ が $\nu$ であると言うのは、写像 $f \in \mathscr{K}_+(T)$ ごとに $\nu^*(f \circ \pi) < +\infty$ であるというと同等です。 $g$ はほぼどこでも局所的に有限なので、適用主張 c) §3, No. 2 の提案 5 の条件を下回ります。したがって、

$$
\int^\bullet (f \circ \pi)\, d\nu = \int^\bullet d\mu(t) \int^\bullet (f \circ \pi)\, d\lambda_t = \int^\bullet f(t)g(t)\, d\mu(t),
$$

$\lambda_t$が$\overline{\pi}^{-1}(t)$に集中していることから。 $\Lambda$ は $\mu$ で十分であるため (§ 3, No. 1、定義 1)、$g$ は $\mu$ 測定可能であることがわかります。したがって、最初のメンバーがすべての $f \in \mathscr{K}_+(T)$ に対して有限であると言うのは、$g$ が局所的に $\mu$ 積分可能であるというというと等価であり (§ 5、提案 1)、この場合 (14) は上記の関係からすぐに続きます。

したがって、残るのは補助的な仮定を削除することだけです。 $g$ が局所的に $\mu$-可積分である場合、$g$ は局所的に $\mu$- ほぼどこでも有限であり、仮定は実際に満たされます。 $\pi$ が $\nu$-proper であると仮定し、$g$ がほぼどこでも局所的に有限であることを示しましょう。 $\mathfrak{K}$ を、$\Lambda|K$ が漠然と連続するようなコンパクトな集合 $K$ の $\mu$ 密集合とします。 $g$ は可測であるため、$g|K = +\infty$ が $\mu$ 無視できるように、すべてのコンパクト集合 $K \in \mathfrak{K}$ を示すことになります。さて、$\mathscr{H}$ を写像 $h \in \mathscr{K}_+(X)$ の集合として、$h \leq 1$ とします。 集合 $g_h(t) = \lambda_t(h)$、$\Lambda_h$ は$\mu$ の適切な写像 $t \mapsto h \cdot \lambda_t$、$\nu_h$ は$\Lambda_h$ の積分、$f$ 元は$\mathscr{K}_+(T)$ を表します。 $f \geq \varphi_K$ のようになります。 適用公式 (14) を $\Lambda_h$ にすると、満たす補助仮定が得られます。

$$
\int (f \circ \pi)\, d\nu \geq \int (f \circ \pi)\, d\nu_h = \int fg_h\, d\mu.
$$

しかし、$K$ に連続する写像の写像 $fg_h|K$ 形増加する有向集合は、その上部エンベロープが値 $+\infty$ になります。 Dini の定理 (GT, X, §4, No. 1, Th. 1) により、$fg_h|K$ が任意の正の数 $n$ 以上になるように選ぶ $h$ ができ、その結果 $\int (f \circ \pi)\, d\nu \geq n\, \mu(K)$ が続きます。 $\pi$ は $\nu$-proper であるため、最初のメンバーは有限なので、その後 $\mu(K) = 0$ が続きます。

#### 系 1 {#int-v-s6-prop-10-cor-1 .statement tag=095C}

— *$\pi$が$\nu$可測であると仮定します。*

a) *$N \subset T$ が局所的に $\mu$ 無視できる場合、$\overline{\pi}^{-1}(N)$ は局所的に $\nu$ 無視可能です。*
b) *$f$ が $T$ の $\mu$ 可測写像をトポロジカル空間 $G$ にすると、$f \circ \pi$ は $\nu$ 可測になります。

前の証明の終わりの記法 $\Lambda_h$、$\nu_h$、$g_h$ を再度取り上げます。$\nu_h$ はすべての $h \in \mathscr{H}$ の制限された尺度であり、$\pi$ は $\nu_h$ に適切であり、$g_h$ はローカルです。 $\mu$ 可積分、および $\pi(\nu_h) = g_h \cdot \mu$、基底 $\mu$ のメジャー。 従って、$N$ は測度 $\pi(\nu_h)$ (§ 5, No. 3、提案 3 と提案 4 の補正 1) に対して局所的に無視できる (それぞれ $f$ が測定可能である) ということになります。 従って、$\overline{\pi}^{-1}(N)$ は、尺度 $\nu_h$ (の Cor. 2) に対して局所的に無視できます (それぞれ $f \circ \pi$ は測定可能です)。

提案 2、それぞれ提案 3)。最後に、措置 $\nu_h$ 形増加するは、最高値が $\nu$ である積極的な措置のファミリーを指向していることに注目し、Cor. §1, No. 4 の提案 11 の 1 (それぞれ Cor. 2)。

#### 系 2 {#int-v-s6-prop-10-cor-2 .statement tag=095D}

*$\pi$ が $\nu$-proper であると仮定します。 $f$ を $T$ で定義された写像とし、値を Banach 空間または $\overline{\mathbf{R}}$ で定義します。 $f \circ \pi$ が本質的に $\nu$ 積分可能であるためには、$gf$ が本質的に $\mu$ 積分可能であることが必要かつ十分です。*

提案 10 を考慮すると、これは Th からすぐに得られます。 §5, No. 3 と Th の 1 です。 No. 2 の 1 つ。

#### 例 {#int-v-s6-n6-exa-1 .statement tag=095E}

— $X$ と $T$ を 2 つの局所的にコンパクトな空間とし、$\pi$ を $X$ から $T$* への * 局所同型写像とする。他の語 (GT、I, §11、Exer. 25) では、すべての点 $x \in X$ が、$\pi|V$ が $\pi(x)$ の近傍に対する $V$ の準同型であるような近傍 $V$ を認めると仮定します。必要に応じて $x$ の比較的コンパクトなオープン近傍 $W$ によって置き換えること $V$ を計算すると、$\overline{W} \subset V$ のような比較的コンパクトなオープン近傍部分集合 $U$ の $X$ の集合 $\mathscr{U}$ が推定されます。 $\pi|\overline{U}$ は、その像に対する $\overline{U}$ の同相写像であり、$X$ の *オープンカバー* です。ここで、$\mu$ を $T$ に対するプラスの指標とします。 $U$ が $\mathscr{U}$ の元である場合、$\pi(U)$ はコンパクト空間 $\pi(\overline{U})$ のオープン集合であるため、$T$ の局所コンパクト部分空間となり、測度定義するの方法がわかります。 $\mu|\pi(U)$ は $\pi(U)$ に $\mu$ によって誘発されました (Ch. IV, §5, No. 7)。 $\pi|U$ の逆同型写像の下で、$\nu_U$ を $\mu|\pi(U)$ の像とします。 $X$ には 1 つのメジャー $\nu$ が存在し、すべてのオープン集合 $U \in \mathscr{U}$ には誘導するメジャー $\nu_U$ が存在することを示します。この測度は、局所同型写像 $\pi$* の下で $\mu$ の *逆像と呼ばれ、$\pi^{-1}(\mu)$ と表されます。

$\nu$ の一意性は、ローカライゼーションの原理 (Ch. III, §2, No. 1、提案 1 の修正) からすぐに適用されます。存在を確立するために、$t \in T$ の場合、すべての点 $x \in \pi^{-1}(t)$ は、点 $x$ でのみ $\pi^{-1}(t)$ と交差する近傍を認めるため、$\pi^{-1}(t)$ は $X$ の *離散* 部分空間となり、家族 $(\varepsilon_x)_{x \in \pi^{-1}(t)}$ は要約可能です。その和を $\lambda_t$ で表します。次に、写像 $t \mapsto \lambda_t$ がスカラー的に本質的に $\mu$ 積分可能であり、その積分 $\nu = \int \lambda_t d\mu(t)$ が求められる逆像であることを示します。これは、次の補題からすぐに得られます。

#### 補題 {#int-v-s6-n6-lem-1 .statement tag=095F}

— a) *$f$を$\mathscr{K}_+(X)$の元とします。 写像 $t \mapsto \lambda_t(f)$ はポジティブ、上部半連続、コンパクトなサポートで、制限から $\pi(X)$ は連続です。*

b) *$U$を$\mathscr{U}$の元、$\nu$をスカラー的に本質的に$\mu$積分可能な関数$t \mapsto \lambda_t$の積分とする。 $\pi|U$ の下の小節 $\nu|U$ の像は $\mu|\pi(U)$ に等しい。*

a) を確立するには、$f$ のサポート $S$ が開いた集合 $U \in \mathscr{U}$ に含まれる場合、単位元 (Ch. III, §1, No. 2、補題 1) の分割によって簡約するを行うことができます。 $g$ を写像 $t \mapsto \lambda_t(f)$ とします。 $\pi|U$ は同型なので、$g|\pi(U)$ 属する ～ $\mathscr{K}_+(\pi(U))$ なので、($\pi(U)$ は $\pi(X)$ の開集合である) $g$ ～ $\pi(X)$ の制限は連続です。 $g$ は正であり、$g$ からコンパクトな集合までの $\pi(S)$ の制限は連続であるため、$g$ は$T$ の上半連続であることがわかります。従って、$g$ は $\mu$ 可積分であることがわかります。

b)を確立するには、$\mathscr{K}(\pi(U))$の要素を$g$、その0から$T$までの拡張を$g^\circ$、関数$g \circ (\pi|U)$を$f$、$f$から$X$の0による拡張を$f^\circ$で表します。 主張 b) は等式 $\int g^\circ d\mu = \int f^\circ d\nu$ と同等です。 しかし、$f \in \mathscr{K}(U)$ なので $f^\circ \in \mathscr{K}(X)$ となり、2 番目の積分は $\int \lambda_t(f^\circ) d\mu(t)$ に等しくなります。 最後に$\lambda_t(f^\circ) = g^\circ(t)$、これで証明が完成します。

ここで、$\pi(X)$ が $T$ で *オープン* であるため、$\mu$ が測定可能であることがわかります。 写像 $\Lambda : t \mapsto \lambda_t$ は、集合 $\pi(X)$ と $\mathbf{C}\pi(X)$ のそれぞれに対する制限が漠然と連続しているため、漠然と $\mu$ 測定可能です。これらの条件、公式 $\overline{\pi}^{-1}(\mu) = \int \lambda_t d\mu(t)$ 定義する分解が $\pi$ に対して $\overline{\pi}^{-1}(\mu)$ のスライスに分割され、提案 10 により次の結果が得られます。

#### 命題 11 {#int-v-s6-prop-11 .statement tag=095G}

*$\pi$ を局所コンパクト空間 $X$ から局所コンパクト空間 $T$ への局所同型写像とし、$\mu$ を $T$ の正の測度とする。この数が有限である場合、$\overline{\pi}^{-1}(t)$の元、数のすべての$t \in T$数に関連する数値写像を$n$とし、逆の場合は$+\infty$とします。 $\pi$ が $\overline{\pi}^{-1}(\mu)$-適切であるためには、$n$ が局所的に $\mu$ 積分可能であることが必要かつ十分であり、その場合*

$$
\pi\left( \overline{\pi}^{-1}(\mu) \right) = n \cdot \mu .
$$

### 練習問題 {#int-v-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
