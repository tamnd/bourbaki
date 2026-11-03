---
book: top
book_title: General Topology
chapter: VIII
chapter_title: Complex numbers
section: 3
section_title: Infinite sums and products of complex numbers
lang: ja
source: top-v-x
pdf_pages: 0121-0124, 0132-0133
extraction: ocr
subsections:
    - "no": 1
      title: INFINITE SUMS OF COMPLEX NUMBERS
      page: 0
      pdf_page: 121
    - "no": 2
      title: MULTIPLIABLE FAMILIES IN $\mathbf{C}^*$
      page: 0
      pdf_page: 121
    - "no": 3
      title: INFINITE PRODUCTS OF COMPLEX NUMBERS
      page: 0
      pdf_page: 123
statements: 9
exercises: 5
content_sha256: ece0e8694c218e2512f4a2e5db622a9cd058257bbd614aca968e926e3f0216f0
translated_from: content/en/top/VIII/03_s3_infinite_sums_and_products_of_complex.md
translation_method: google
source_content_sha256: 07d4fe8c1f201c515f0cbf75d3cd066fc09084c3035b0204be862ef63ea6d88e
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 10f59d3de2a6a00056d5b5d1cb21bb06619361d2dfee59804864b5e175328bed
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 3. 複素数の無限和と積

### 1. 無限和/複素数

体 $\mathbf{C}$ の加法群は加法群 $\mathbf{R}^2$ と同じであるため、$\mathbf{C}$ の加算可能な家族と系列は、章の一般的な理論に含まれるため、特別に検討する必要はありません。 VII, § 3;この理論の結果を複素数の理論の言語に翻訳するのは読者練習問題に委ねられます。 章 VII, § 3, no. 1 のうち、系から命題までの 3 つである次の命題のみを記載します。

#### 命題 1 {#top-viii-s3-prop-1 .statement tag=0C0I}

*もし* $(u_\lambda)_{\lambda \in L}$ *と* $(v_\mu)_{\mu \in M}$ *が複素数の2つの加算可能な族である場合、その族* $(u_\lambda v_\mu)_{(\lambda, \mu) \in L \times M}$ *は加算可能であり、次のようになります*

$$
\sum_{(\lambda, \mu) \in L \times M} u_\lambda v_\mu = \left( \sum_{\lambda \in L} u_\lambda \right) \left( \sum_{\mu \in M} v_\mu \right).
$$

クォータニオンの対応するの結果を述べるのは読者に任せます。

### 2. $\mathbf{C}^*$ の多世帯家族

非ゼロ複素数の乗法群 $\mathbf{C}^*$ では、族 $(z_i)_{i \in I}$ できないは、$I$ の有限部分集合 (章) の補数のフィルターに関して乗算可能です 〜でない限り $\lim z_i = 1$ III, § 5, no. 2、命題 1);さらに、$\mathbf{C}^*$ のすべての点には、近傍の可算基本系、添字 $i$ の集合があるため、族 $(z_i)$ が乗算可能な場合、$z_i \neq 1$ は可算になります。 (章 III, § 5, no. 2、系 ～ 命題 1)。

#### 命題 2 {#top-viii-s3-prop-2 .statement tag=0C0J}

*ファミリー* $(z_i)$ *複素数* $z_i = r_i (\cos \theta_i + i \sin \theta_i)$ *ファミリー* $(r_i)$ *絶対値の* $z_i$ *が* $\mathbf{R}_+^*$ *およびファミリー* $(\theta_i)$ *振幅の場合にのみ乗算可能です* $z_i$ *は角度* $\mathfrak{A}$ の群で合計できます。

群 $\mathbf{C}^*$ の構造 ($\S$ 1、no. 3、命題 1) を考慮すると、命題は明らか帰結の命題 4 です。 章 III、$\S$ 5、no. 4。

写像各角度 $\theta$ をそのメジャーの 1 つ (任意の基底 $a$ に) 属するから区間 $] - \frac{1}{2} a, \frac{1}{2} a ]$ にすると、$\mathfrak{A}$ の *ローカル同型* が得られます。 $\mathbf{R}$ ($\S$ 2、no. 2); $I$ の有限部分集合の補数のフィルターに関して $\lim \theta_i = 0$ があるため、置き換える条件 (命題 2 の主張で) $\theta_i$ は以下によって $\mathfrak{A}$ で合計可能であるはずです。 条件属するから $] - \frac{1}{2} a, \frac{1}{2} a ]$ までの角度 $\theta_i$ の *メジャー* の族 $(t_i)$ は $\mathbf{R}$ で合計できるはずです。

次の定理は、形 $(1 + u_i)$ に代入される複素数のファミリーに対する他の基準を与え、$\mathbf{C}^*$ で乗算されます。 (章 IV、$\S$ 7、no. 4 のうち定理 4 を一般化します。章 IX、付録、no. 2、命題 1 も参照してください):

#### 定理 1 {#top-viii-s3-thm-1 .statement tag=0C0K}

*ファミリー* $(1 + u_i)_{i \in I}$ *は乗算可能* $\mathbf{C}^*$ *ファミリー* $(|u_i|)$ *が加算可能* $\mathbf{R}$である場合に限ります。

$I$ の各有限部分集合 $J$ に、

$$
p_J = \prod_{i \in J} (1 + a_i), \quad s_J = \sum_{i \in J} a_i, \quad \sigma_J = \sum_{i \in J} |a_i|.
$$

#### 補題 1 {#top-viii-s3-lem-1 .statement tag=0C0L}

*それぞれの有限部分集合* $J$ *of* $I$、*let* $\varphi(J) = \sup_{L \subset J} (p_L - 1)$。 *その後、それぞれ部分集合* $L$ *of* $J$ *私たちは*

$$
|p_L - 1 - s_L| \leq \varphi(J) \sigma_L.
$$

$L$ が空であればこれはクリアです。カード$(L)$の帰納法まで進みます。 $L = K \cup \{ \lambda \}$、ここで$\lambda \notin K$ とします。次に、$p_L = p_K (1 + a_\lambda)$ と $s_L = s_K + a_\lambda$ なので、$p_L - 1 - s_L = (p_K - 1 - s_K) + (p_K - 1)a_\lambda$ になります。したがって、$\varphi(J)$ の帰納的仮定と定義により、次のようになります。

$$
|p_L - 1 - s_L| \leq \varphi(J) \sigma_K + \varphi(J)|a_\lambda| = \varphi(J) \sigma_L,
$$

これは補題を証明します。

#### 補題 2 {#top-viii-s3-lem-2 .statement tag=0C0M}

*もし* $J$ *が* $I$の有限部分集合である*場合* $\varphi(J) < 1/4$、*その後*

$$
|\sigma_J| \leq 4 \varphi(J)/(1 - 4 \varphi(J)).
$$

なぜなら、$J$ のすべての部分集合 $L$ について $\sigma_L \leq \sigma_J$ であるため、(2) から $|s_L| \leq \varphi(J) \sigma_J + |p_L - 1| \leq (1 + \sigma_J)\varphi(J)$ が得られます。しかし、章 VII、$\S$ 3、no. 1、命題 2 により、$|\sigma_J| \leq 4 \sup_{L \subset J} |s_L|$、したがって $\sigma_J \leq 4 \varphi(J)(1 + \sigma_J)$ となり、結果は次のようになります。

ここで、定理 1 で述べた条件で十分であることを示しましょう。 仮定族 $(|u_i|)$ が $\mathbf{R}$ で加算可能であるということは、族 $(1 + |u_i|)$ が $\mathbf{R}_+^*$ (章 IV, § 7, no. 4, 定理 4) で乗算可能であることを意味します。したがって、それぞれの $\varepsilon > 0$ には、$I$ の有限部分集合 $J_0$ があり、$J_0$ を満たさない$I$ のそれぞれの有限部分集合 $L$ には、$\prod_{i \in L} (1 + |u_i|) - 1 \leq \varepsilon$ があります。しかし、$\prod_{i \in L} (1 + u_i) - 1$ を形 $\sum_M \left( \prod_{i \in M} u_i \right)$ に書くことができます。ここで、$M$ は、$L$ の空でないすべての部分集合を通過します。 $\left| \prod_{i \in M} u_i \right| = \prod_{i \in M} |u_i|$ 以来、

$$
\left| \prod_{i \in L} (1 + u_i) - 1 \right| \leq \sum_M \left( \prod_{i \in M} |u_i| \right) = \prod_{i \in L} (1 + |u_i|) - 1 \leq \varepsilon.
$$

$\mathbf{C}^*$ は完全な群であるため、コーシーの基準により、これは私たちの主張を証明します。

定理 1 の条件が必要であることを示す必要があります。 $(1 + u_i)_{i \in I}$ が $\mathbf{C}^*$ の乗法族である場合、$J$ を満たさない$I$ のすべての有限部分集合 $H$ に対して、$\left| \prod_{i \in H} (1 + u_i) - 1 \right| \leq 1/8$ が存在するように、$I$ の有限部分集合 $J$ が存在します。 補題 2 までに、$J$ を満たさない$I$ のすべての有限部分集合 $H$ に対して $\sum_{i \in H} |u_i| \leq 1$ が成り立ち、したがって族 $(|u_i|)$ は $\mathbf{R}$ (章 IV, § 7, no. 1, 定理 1）。

上記の証明は、必要な変更を加えて、特定の非可換除算環および代数における (順序付き) 無限積にも適用されます (練習問題 6、および章 IX、付録を参照)。

### 3. 無限の積/複素数

一般因子 $z_n = r_n (\cos \theta_n + i \sin \theta_n)$ を伴う非ゼロ複素数の無限積が $\mathbf{C}^*$ に収束するには、群 $\mathbf{C}^*$ の構造から、一般因子を伴う積が必要かつ十分です。 $r_n$ は $\mathbf{R}_+^*$ と系列に収束し、一般的な項 $t_n$ (]$-\frac{1}{2}a$、$\frac{1}{2}a$] にある $\theta_n$ の尺度) は $\mathbf{R}$ に収束します。

#### 定義 1 {#top-viii-s3-def-1 .statement tag=0C0N}

*一般因子* $1 + u_n$ を持つ複素数の無限積、 *一般因子* $1 + |u_n|$ と積が *収束する* (または、同等に、一般系列の場合) は絶対に収束するといいます項 $|u_n|$ は収束します)。

#### 命題 3 {#top-viii-s3-prop-3 .statement tag=0C0O}

*複素数の無限積は、絶対収束する場合に限り、可換収束します。*

#### 注意 1 {#top-viii-s3-n3-rem-1 .statement tag=0C0P}

積と一般的な因子 $|1 + u_n|$ は収束する可能性があり、実際に $\mathbf{R}_i^*$ では絶対に収束しますが、積と一般的な因子 $1 + |u_n|$ は収束しません (練習問題 4 を参照)。もちろん、このできないは、すべての $u_n$ が本物で、特定の添字以降の $> 0$ が本物である場合に発生します。

#### 注意 2 {#top-viii-s3-n3-rem-2 .statement tag=0C0Q}

因子 $> 0$ の積についてすでに述べたように、系列と一般項 $u_n$ の収束は、積と一般因子 $1 + u_n$ の収束には必要でも十分でもありません。

### 練習問題 {#top-viii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
