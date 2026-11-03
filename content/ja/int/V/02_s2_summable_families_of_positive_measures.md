---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 2
section_title: Summable families of positive measures
lang: ja
source: int-i-vi
book_pages: INT V.95-INT V.96
pdf_pages: 0266-0270, 0350-0351
extraction: ocr
subsections:
    - "no": 1
      title: Definition of summable families of measures
      page: 11
      pdf_page: 266
    - "no": 2
      title: Integration with respect to a sum of positive measures
      page: 12
      pdf_page: 267
    - "no": 3
      title: Decomposition of a measure as a sum of measures with compact support
      page: 14
      pdf_page: 269
statements: 12
exercises: 4
content_sha256: 09c887ca5563ca138a54dd59cf45bece255dd4d47e3031621cff3f84352214e9
translated_from: content/en/int/V/02_s2_summable_families_of_positive_measures.md
translation_method: google
source_content_sha256: ec7d58f4d9ead5ad76e61a986e1e25bc88d93ca5a6598bf0f04e740c0b11cee4
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 1a370453af145c68de3be841dea1d892cbf81ab88a17b6dd92146d7a665c72f8
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 2。積極的な対策の合計可能なファミリー

### 1. 要約可能なメジャーファミリーの定義

$(\lambda_\alpha)_{\alpha \in A}$ を局所コンパクト空間 X に関する積極的な措置のファミリーとします。ファミリー $(\lambda_\alpha)_{\alpha \in A}$ は、曖昧な位相 (GT、III, §5, No. 1) を備えた X 上の実際のメジャーのベクトル空間 $\mathscr{M}(X)$ で合計可能である場合、*合計可能なメジャーファミリー* であると言われます。これは、というとなり、写像 $f \in \mathscr{K}(X)$ ごとに、数 $\lambda_\alpha(f)$ の族が $\mathbf{R}$ で合計可能になります。なぜなら、この条件は明らかに必要だからです。逆に、それが満たされる場合、$\mathscr{K}(X)$ 上の線型形式 $f \mapsto \sum_{\alpha \in A} \lambda_\alpha(f)$ は正であるため、正の測度 $\nu$ (Ch. III, §1, No. 5、Th. 1) となり、族 $(\lambda_\alpha)$ の有限部分和が漠然と以下に収束することが直ちに検証されます。 $\nu$、A (GT、III, §5, No. 1、Def. 1) の有限部分集合の集合の切断フィルターに関して。

$\mathscr{K}(X)$ のすべての元は $\mathscr{K}_+(X)$ の 2 つの元の差であるため、家族 $(\lambda_\alpha)$ は次の場合にのみ合計可能です。
$$
\sum_{\alpha \in A} \lambda_\alpha(f) < +\infty
$$

写像 $f \in \mathscr{K}_+(X)$ごとに。この条件は次と同等です。

(2)
$$
\sum_{\alpha \in A} \lambda_\alpha(K) < +\infty
$$
すべてのコンパクト集合 $K \subset X$ に対して。

なぜなら、$f \leq \|f\| \cdot \varphi_S$ により (2) は (1) を意味します。ここで、S は $f$ のコンパクトなサポートを示します。逆に、K がコンパクト集合である場合、$\varphi_K \leq f$ (Ch. III, §1, No. 2, 補題 1) となる写像 $f \in \mathscr{K}_+(X)$ が存在し、(1) は (2) を含意することになります。

#### 注意 1 {#int-v-s2-n1-rem-1 .statement tag=090G}

族 $(\lambda_\alpha)_{\alpha \in A}$ が加算可能な場合、その和が有限部分和 $\sum_{\alpha \in J} \lambda_\alpha$ の $\mathscr{M}_+(X)$ の最高点となるのは明らかであり、ここで J は A の有限部分集合の集合を超えます。

#### 注意 2 {#int-v-s2-n1-rem-2 .statement tag=090H}

$(\theta_\alpha)_{\alpha \in A}$ を X の複雑な測度の族とします。ポジティブメジャーのファミリー $(|\theta_\alpha|)$ が合計可能であれば、ファミリー $(\theta_\alpha)$ は *合計可能* であると言われます。 *このためには、家族 $(\theta_\alpha)$ が曖昧な位相 (cf. Exer. 3) を備えたベクトル空間 $\mathscr{M}(X; \mathbf{C})$ で要約可能であるだけでは十分ではありません。

### 2. 和の積極的措置に関する統合

*この No.* 全体で、X は局所的にコンパクトな空間、$(\lambda_\alpha)_{\alpha \in A}$ は X の積極的な対策の合計可能なファミリー、および $\nu$ は対策 $\sum_{\alpha \in A} \lambda_\alpha$ を示します。

#### 命題 1 {#int-v-s2-prop-1 .statement tag=090I}

— *f を、X で定義された正の数値写像とします。それから*
$$
\nu^\bullet(f) = \sum_{\alpha \in A} \lambda_\alpha^\bullet(f).
$$

これは、注意 1、§1, No. 3 の提案 11、§1, No. 1 の提案 3 から一気に続きます。

#### 系 1 {#int-v-s2-prop-1-cor-1 .statement tag=090J}

— *すべてのコンパクト (それぞれオープンおよび比較的コンパクト) 部分集合 M の X、
$$
\nu(M) = \sum_{\alpha \in A} \lambda_\alpha(M).
$$*

#### 系 2 {#int-v-s2-prop-1-cor-2 .statement tag=090K}

— *X の部分集合 N が局所的に $\nu$ 無視できるためには、すべての $\alpha \in A$ について N が局所的に $\lambda_\alpha$ 無視できることが必要かつ十分です。*

#### 系 3 {#int-v-s2-prop-1-cor-3 .statement tag=090L}

— *写像 $f \in \mathscr{F}_+(X)$ごとに、
$$
\nu^*(f) \geq \sum_{\alpha \in A} \lambda_\alpha^*(f).
$$*

$f$ が $\nu$ で調整されていない場合、$\nu^*(f) = +\infty$ ($§ 1$、No. 2、提案 7) であるため、不等式は明らかです。 $f$ が $\nu$ で緩和されている場合、すべての $\nu$ 積分可能なオープン集合は $\lambda_\alpha$ で積分可能であるため、$f$ はすべての $\alpha \in A$ に対して $\lambda_\alpha$ で緩和されます。 関係 (4) は、(3) と $§ 1$、No. 2 の提案 7 からすぐに続きます。

$A$ が可算で、それぞれの $\lambda_\alpha$ が点メジャーである場合でも、(4) の 2 つの要素が等しくない場合があります ($§ 1$、Exer. 4 a))。

#### 命題 2 {#int-v-s2-prop-2 .statement tag=090M}

— *$f$ を $X$ の写像としてトポロジカル空間 $G$ にします。 $f$ が $\nu$ で測定可能であるためには、 $\alpha \in A$ ごとに $f$ が $\lambda_\alpha$ で測定可能であることが必要かつ十分です。

これはコルからすぐに続きます。 $§ 1$ の提案 11 の 2。

#### 命題 3 {#int-v-s2-prop-3 .statement tag=090N}

— *For a mapping $f$ of $X$ into a Banach space $F$ to be essentially $\nu$-integrable, it is necessary and sufficient that $f$ be essentially $\lambda_\alpha$-integrable for every $\alpha \in A$ and that*

$$
\sum_{\alpha \in A} \int^\bullet |f| \, d\lambda_\alpha < +\infty .
$$

*ファミリー $(\int f \, d\lambda_\alpha)_{\alpha \in A}$ は $F$ で絶対に合計可能であり、*

$$
\int f \, d\nu = \sum_{\alpha \in A} \int f \, d\lambda_\alpha .
$$

実際、$f$ が本質的に $\nu$ 積分可能 (それぞれ本質的に $\lambda_\alpha$ 積分可能) であるためには、$f$ が測度 $\nu$ (それぞれ $\lambda_\alpha$) と $\nu^\bullet(|f|) < +\infty$ (それぞれ $\lambda_\alpha^\bullet(|f|) < +\infty$) について可測であることが必要かつ十分です。 $§ 1$、No. 3の提案9。したがって、主張の最初の部分は Props からすぐに続きます。 2 と 1. $f$ が本質的に $\nu$ 可積分である場合、不等式

$$
\sum_{\alpha \in A} \left| \int f \, d\lambda_\alpha \right| \leq \sum_{\alpha \in A} \int |f| \, d\lambda_\alpha = \nu(|f|)
$$

これは、族 $(\int f \, d\lambda_\alpha)$ が $F$ で絶対に合計可能であり、 和のノルムが $\mathscr{L}_F^1(\nu)$ の $f$ のノルム以下であることを意味します。 $f \in \mathscr{L}_F^1(\nu)$の集合、つまり満たす (6) は$\mathscr{L}_F^1(\nu)$の閉じた線形部分空間 $\mathscr{H}$です。さて、この部分空間は $\mathscr{L}_F^1(\nu)$ でも密です。なぜなら、形 $f \cdot a$ の含む写像であり、$a \in F$ と $f$ は有限可積分正の写像を示します (提案 1)。 したがって$\mathscr{H} = \mathscr{L}_F^1(\nu)$と命題が成立します。

提案 3 は、§3 (No. 3、Th. 1) で証明される積分に関する一般的な定理からも推定できます。

#### 系 1 {#int-v-s2-prop-3-cor-1 .statement tag=090O}

— $f$ が $\nu$ 可積分であると仮定します。この場合、$f$ はすべての $\alpha \in A$ に対して $\lambda_\alpha$ 積分可能であり、公式 (6) が成り立ちます。逆に、集合 $A$ が有限で、$f$ が $\alpha \in A$ ごとに $\lambda_\alpha$ 可積分である場合、写像 $f$ は $\nu$ 可積分です。

$f$ が $\nu$ 積分可能である場合、$f$ は本質的に $\nu$ 積分可能であり、$\nu$ 緩和されます (§ 1, No. 3、提案 9 の裏付け)。したがって、$f$ は本質的に $\alpha \in A$ ごとに $\lambda_\alpha$ 積分可能であり、$\lambda_\alpha$ が緩和され、したがって $\lambda_\alpha$ が積分可能です。逆に、$A$ が有限で、$f$ がすべての $\alpha \in A$ に対して $\lambda_\alpha$ 積分可能である場合、$f$ は提案 3 によって本質的に $\nu$ 積分可能であり、$\nu^*(|f|) < +\infty$ が検証されるだけで十分です。これは関係 $\nu^* = \sum_{\alpha \in A} \lambda_\alpha^*$ (Ch. IV, §1, No. 3、提案 15) からすぐに続きます。

#### 系 2 {#int-v-s2-prop-3-cor-2 .statement tag=090P}

— $\theta$ を $X$ の複素メジャーとします。 集合 $\theta_1 = (\Re \theta)^+$、$\theta_2 = (\Re \theta)^-$、$\theta_3 = (\Im \theta)^+$、$\theta_4 = (\Im \theta)^-$。 位数では、$X$ の写像 $f$ をトポロジカル空間 $G$ (それぞれバナッハ空間 $F$) にすると、その測度は可測 (それぞれ本質的に可積分、積分可能) になります。 $\theta$、それぞれの尺度 $\theta_i$ ($i = 1, 2, 3, 4$) について、それが測定可能 (それぞれ本質的に積分可能、積分可能) であることが必要かつ十分です。

$f$ が $\theta$ に対して測定可能 (それぞれ本質的に可積分、積分可能) である場合、$f$ は、$|\theta|$ について定義によって測定可能 (それぞれ、本質的に可積分、積分可能) であり、したがって、$\theta_i$ についても測定可能です。 $\leq |\theta|$。逆に、$f$ が尺度 $\theta_i$ に対して測定可能 (それぞれ本質的に積分可能、積分可能) である場合、提案 2 (それぞれ提案 3、提案 3 の補正 1) は、$f$ が尺度 $\theta_1 + \theta_2 + \theta_3 + \theta_4$ に対して測定可能 (それぞれ本質的に積分可能、積分可能) であることを意味します。 $\geq |\theta|$。

### 3. 分解の対策と和のコンパクトなサポートによる対策

#### 命題 4 {#int-v-s2-prop-4 .statement tag=090Q}

— $\mu$ を局所的にコンパクトな空間 $T$ に対する正の測度とし、$\mathfrak{K}$ を $T$ のコンパクト部分集合の $\mu$ 密な集合とします。 $T$ には、$\mu = \sum_{\alpha \in A} \mu_\alpha$ のようなポジティブ指標の加算可能な族 $(\mu_\alpha)_{\alpha \in A}$ が存在し、指標 $\mu_\alpha$ 属するから $\mathfrak{K}$ と形の局所的に可算なペアごとの互いに素コンパクト集合の族が存在します。

$\mu$ が緩和された場合、添字集合 $A$ は可算であるとみなされる可能性があります。

集合 $N = T - \bigcup_{\alpha \in A} K_\alpha$ が局所的に $\mu$ 無視できるようなペアワイズ互いに素元の $\mathfrak{K}$ の局所的に可算な族 $(K_\alpha)_{\alpha \in A}$ を考えます。

(Ch. IV, §5, No. 9、提案 14)。 写像 $f \in \mathscr{K}(T)$、集合ごとに
$$
\mu_\alpha(f) = \mu(f \varphi_{K_\alpha});
$$
$\mathscr{K}(T)$ の線型形式 $\mu_\alpha$ はポジティブであるため、$K_\alpha$ にサポートが含まれるポジティブな指標です。 $\mathfrak{K}$ 属するから $\mathfrak{K}$ の元にすべてのコンパクト集合が含まれるため、すべての $\alpha \in A$ に対して $\operatorname{Supp}(\mu_\alpha) \in \mathfrak{K}$ が含まれます。 残っているのは、族 $(\mu_\alpha)$ が合計可能であり、その和が $\mu$ に等しいこと、他の語では写像 $f \in \mathscr{K}_+(T)$ ごとに $\sum_{\alpha \in A} \mu_\alpha(f) = \mu(f)$ であることを示すことだけです。

ここで、$S$ を $f$ の (コンパクトな) サポートとし、$A'$ を $S \cap K_\alpha \neq \varnothing$ となるように $\alpha \in A$ によって形成される可算数集合とします。 集合 $N \cap S$ は $\mu$ で無視できるため、
$$
\begin{align*}
\mu(f) &= \mu(f \varphi_S) = \sum_{\alpha \in A'} \mu(f \varphi_{S \cap K_\alpha}) = \sum_{\alpha \in A'} \mu(f \varphi_{K_\alpha}) \\
&= \sum_{\alpha \in A} \mu(f \varphi_{K_\alpha}) = \sum_{\alpha \in A} \mu_\alpha(f).
\end{align*}
$$
これで一般的なケースの証明が完了します。 $\mu$ が緩和されている場合、集合 $T$ は $\mu$ が緩和されているため、$T$ はコンパクトな集合の数列 $(L_n)$ と無視できる程度の集合の和集合になります。 (§ 1, No. 2、提案 5); $A'$ を、$K_\alpha$ が $L_n$ の 1 つと交差するように、$\alpha \in A$ の可算数集合とします。次に、$\alpha \notin A'$ に対して $\mu_\alpha = 0$ が続き、すぐに主張の最後の文が続きます。

#### 注意 {#int-v-s2-n3-rem-1 .statement tag=090R}

A positive measure may be the sum of a sequence of measures with compact support, and not be moderated (see Exer. 4 a) of § 1).

### 練習問題 {#int-v-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
