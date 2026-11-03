---
book: int
book_title: Integration
chapter: V
chapter_title: INTEGRATION OF MEASURES
section: 5
section_title: Measures defined by numerical densities
lang: ja
source: int-i-vi
book_pages: INT V.38-INT V.62, INT V.99-INT V.107
pdf_pages: 0293-0317, 0354-0362
extraction: ocr
subsections:
    - "no": 1
      title: Locally integrable functions
      page: 38
      pdf_page: 293
    - "no": 2
      title: Measures defined by numerical densities
      page: 40
      pdf_page: 295
    - "no": 3
      title: Integration with respect to a measure defined by a density
      page: 42
      pdf_page: 297
    - "no": 4
      title: Behavior of the product with respect to the usual operations
      page: 45
      pdf_page: 300
    - "no": 5
      title: Characterization of measures with base $\mu$
      page: 48
      pdf_page: 303
    - "no": 6
      title: Equivalent measures
      page: 52
      pdf_page: 307
    - "no": 7
      title: Alien measures
      page: 54
      pdf_page: 309
    - "no": 8
      title: 'Applications: I. Duality of the spaces $L^p$'
      page: 56
      pdf_page: 311
    - "no": 9
      title: 'Applications: II. Functions of measures'
      page: 60
      pdf_page: 315
    - "no": 10
      title: Diffuse measures; atomic measures
      page: 61
      pdf_page: 316
statements: 52
exercises: 31
content_sha256: b2f71bc39cc57a23f1e25e59edb25044258b2fdebe3266d6b155266233051872
translated_from: content/en/int/V/05_s5_measures_defined_by_numerical_densities.md
translation_method: google
source_content_sha256: d1c0e47776f33ebac3f5f4eb44ad8e2e1b76c65670899f2de059c9d70818f487
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: e91241ec962711c57b250b5d5b4fa26cf460a3913332ce8a44799e4e55ef029c
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 5。数値密度によって定義される尺度

### 1. ローカルで可積分関数

#### 命題 1 {#int-v-s5-prop-1 .statement tag=092D}

* g を T のほぼどこでも (正の尺度 $\mu$) で局所的に定義され、Banach 空間 F (それぞれ $\overline{\mathbf{R}}$) で値を使用して、写像とします。次のプロパティは同等です:*

a) *すべての点 $t \in T$ に対して、写像 $g \varphi_V$ が $\mu$ 可積分となるような t の近傍 V が存在します。

b) *写像 g は $\mu$ で測定可能であり、すべてのコンパクトでは集合 $K \subset T$、$\int^* |g|\varphi_K\,d\mu < +\infty$ です。*

c) *すべての数値写像 $h \in \mathscr{K}(T)$ について、$gh$ は $\mu$ 積分可能です。*

a) が b) を意味することを示しましょう。 写像 g は局在化の原理によって測定可能です (Ch. IV, §5, No. 2、提案 4)。 一方、$t \in K$ごとに、仮定までに、$g \varphi_{V_t}$が可積分となるような$T$の$t$の近傍$V_t$が存在します。したがって、写像 $g \varphi_{V_i}$ が可積分となるように、近傍 $V_i$ ($1 \leq i \leq n$) の有限数で $K$ をカバーできます。 $|g| \varphi_K \leq \sum_{i=1}^n |g| \varphi_{V_i}$ 以降、1 つは $\int^* |g| \varphi_K \, d\mu < +\infty$ になります。

第二に、b) は c) を暗示します。なぜなら、$gh$ が測定可能であり、$L$ が $h$ のコンパクトサポートである場合、$|gh| \leq \|h\| \cdot |g| \varphi_L$、したがって仮定による $\int^* |gh| \, d\mu < +\infty$ です。したがって、$gh$ は積分可能性の基準によって積分可能です (Ch. IV, §5, No. 6、木。 5)。

最後に、c) は a) を意味します。実際、すべての $t \in T$ について、$V$ を $t$ のコンパクトな近傍とします。 $T$ から $[0,1]$ への連続した写像 $h$ が存在し、$V$ の 1 に等しく、コンパクトなサポート (Ch. III, §1, No. 2、補題 1) が付いています。 仮定による $gh$ は可積分であるため、$g \varphi_V = (gh) \varphi_V$ も可積分です (Ch. IV, §5, No. 6、Th. 5 のコリント 3)。

#### 定義 1 {#int-v-s5-def-1 .statement tag=092E}

*写像* $g$、*ほぼどこでもローカルに定義* $T$ (*積極的な対策* $\mu$)、*Banach 空間* $F$ の値 (*それぞれ* $\overline{\mathbf{R}}$)、 * についてローカルに積分可能と言われています* $\mu$ (*またはローカル* $\mu$*-可積分*) *それが提案 1 の条件* a)、b)、c) を満たす場合* *** $\theta$ * が複素測度である場合、 写像* $g$ *ローカルに定義* $\theta$*-ほとんどどこでもポジティブ測度* $|\theta|$ に対して局所的に積分可能である場合は、局所的に* $\theta$*-積分可能。

$g$ が局所的に $\theta$ 可積分である場合、局所的にほぼどこでも $g$ に等しいすべての写像が局所的に可積分可能です。ローカルにある 2 つの可積分関数のうち和がローカルに可積分であることは明らかです。 写像と $F$ の値は、*どこでも定義* されており、$\theta$、形ベクトル空間は $\mathscr{L}_{loc}^1(T, \theta; F)$ で示され、ローカルに積分可能です。 $F = \mathbf{R}$ または $\mathbf{C}$ の場合、曖昧さがなければ $F$ の記載は省略されることがよくあります。この空間には、(反対の明示的な言及がない限り) 準標準 $g \mapsto \int |g \varphi_K| \, d|\theta|$ によって定義された位相が常に装備されます。ここで、$K$ は、$T$ のコンパクトな部分集合の集合を上回ります。関連するハウスドルフ空間、$\mathscr{L}_{loc}^1(T, \theta; F)$ の商 by 写像の部分空間 $\mathscr{N}_F^\infty$ は、ほぼどこでも局所的に零であり、$L_{loc}^1(T, \theta; F)$ で示されます。 空間 $L_{loc}^1(T, \theta; F)$ と $L_{loc}^1(T, |\theta|; F)$ は同一です。

たった今定義したトポロジカルベクトル空間が *完全* であることがわかります (例 31)。

すべての可測写像 $g$ は、本質的にすべてのコンパクト集合で境界付けられており、局所的に積分可能です。 $1 \leq p \leq +\infty$ のようなすべての数 $p$ に対して、すべての写像 $g \in \mathscr{L}_F^p$ はローカルに積分可能です。実際、写像 $h \in \mathscr{H}(T)$、$h$ 属する ～ $\mathscr{L}^q$ ($q$ は指数共役 ～ $p$) ごとに、$gh$ は可積分です (Ch. IV, §6, No. 4、Cor. Th 2)の4。

$F, G, H$ を 3 つのバナッハ空間とし、$(u, v) \mapsto \Phi(u, v)$ を $F \times G$ から $H$ への連続双線形写像とします。 $f$ が局所的に可積分であり、その値を F に取る場合、および $g \in \mathscr{L}_G^\infty$ の場合、$\Phi(f, g)$ は局所的に可積分可能です (Ch. IV, §6, No. 4、Th. 2 の Cor. 1)。

### 2. 数値密度によって定義される尺度

Let $g$ be a positive numerical function defined locally $\mu$-almost everywhere in T and locally $\mu$-integrable; the set of $t$ such that $g(t) = +\infty$ is then locally $\mu$-negligible, because $g \varphi_K$ is $\mu$-integrable for every compact set K (Ch. IV, §2, No. 3、提案 7)。 ここで、$g'$ を局所的な可積分関数とし、正で有限であり、ほぼどこでも $g$ 局所的な $\mu$ に等しいとします。 集合 $\lambda'_t = g'(t) \varepsilon_t$。 T の $\mathscr{M}_+(T)$ への写像 $t \mapsto \lambda'_t$ は、漠然と $\mu$ 測定可能であり、スカラー的に本質的に積分可能です (または、再度、I が T の恒等写像である対 $(I, g')$ は、$\mu$ 適応されます)。整 $\nu = \int \lambda'_t d\mu(t)$ は特定の写像 $g'$ には依存せず、局所的にほぼどこでも $g$ に等しく、$\lambda'_t$ の尺度定義で使用されます。 この尺度 $\nu$ は条件によって決定されます

$$
\int f(t)\,d\nu(t) = \int f(t)g(t)\,d\mu(t) \quad \text{for } f \in \mathscr{K}(T).
$$

If now $\theta$ is a complex measure, and if $u$ is a complex function (or a function with values in $\overline{\mathbf{R}}$) defined locally $\theta$-almost everywhere and locally integrable for $\theta$, one can write

$$
\begin{align*}
u &= g_1 - g_2 + i(g_3 - g_4) \\
\theta &= \mu_1 - \mu_2 + i(\mu_3 - \mu_4)
\end{align*}
$$

ここで、$\mu_1 = (\Re \theta)^+$、$\mu_2 = (\Re \theta)^-$、$\mu_3 = (\Im \theta)^+$、$\mu_4 = (\Im \theta)^-$ (Ch. III, §1, No. 5)、および$g_1, g_2, g_3, g_4$ は同様の意味を持ちます。 $|u|$ は局所的に $|\theta|$ 積分可能であるため、正の写像 $g_i$ ($i = 1, 2, 3, 4$) はそれぞれの正の測度 $\mu_j$ ($j = 1, 2, 3, 4$) に対して局所的に積分可能であるため、 写像

$$
f \mapsto \int f(t)u(t)\,d\theta(t)
$$

$\mathscr{K}(T)$ は複雑な尺度です。

#### 定義 2 {#int-v-s5-def-2 .statement tag=092F}

*$\theta$ を複素測度とし、$u$ を複素数写像 (または $\overline{\mathbf{R}}$ に値を含む写像) とし、ローカルに $\theta$ - ほぼどこでも、ローカルに $\theta$ - 積分可能に定義します。 T 上の複素小節 $f \mapsto \int fu\,d\theta$ は、$\theta$ 写像 $u$ による小節の積、または $\theta$ に対する稠密度 $u$ の小節であると言われ、$u \cdot \theta$ と表されます。

局所的に $\mu$ 積分可能な関数による正の測度 $\mu$ の積であるすべての複素測度は、基底 $\mu$ を持つ測度と呼ばれます。

関係 $\eta = u \cdot \theta$ は、慣例により、再び書かれます。

$$
d\eta(t) = u(t)\, d\theta(t).
$$

$u$ がどこでも定義され連続している場合、第 3 章で与えられた定義が回復します。 III, §1, No. 4。 $u_1$ と $u_2$ が局所的に $\theta$ 可積分であれば、$(u_1 + u_2) \cdot \theta = u_1 \cdot \theta + u_2 \cdot \theta$ であることは明らかです。同様に、$\theta_1$ と $\theta_2$ が $T$ 上の 2 小節であり、$u$ が $\theta_1$ と $\theta_2$ に対して局所的に積分可能な写像である場合、$u$ は $\theta_1 + \theta_2$ に対して局所的に積分可能であり、1 つは $u \cdot (\theta_1 + \theta_2) = u \cdot \theta_1 + u \cdot \theta_2$ になります。

今後は、どこでも定義された写像の場合に限定します。ほとんどどこでもローカルに定義されている拡大から写像は、常に明白ですが、読者に委ねられています。

次の命題により、大部分の部分は、複雑な措置のケースを積極的な措置のケースに減らすことができます。

#### 命題 2 {#int-v-s5-prop-2 .statement tag=092G}

*$\theta$ を複素測度、$u$ を局所的に $\theta$ 可積分可能な複素数写像とします。それから*

$$
|u \cdot \theta| = |u| \cdot |\theta|.
$$

補助的な結果から始めます。

#### 補題 1 {#int-v-s5-lem-1 .statement tag=092H}

— *$\theta$ を複素測度とし、$f$ を $\overline{\mathscr{L}}^1_C(T, \theta)$ の元とします。それから*

$$
\langle|\theta|, |f|\rangle = \sup_{c \in \mathscr{K}_1} |\langle\theta, cf\rangle| = \sup_{c \in \mathscr{B}_1} |\langle\theta, cf\rangle|,
$$

*ここで、$\mathscr{K}_1$ (それぞれ$\mathscr{B}_1$) は、$|c| \leq 1$ のように、コンパクトなサポート (それぞれ Borel) と連続する複素数写像 $c$ の集合を表します。

まず、$f \in \mathscr{K}(T; \mathbf{C})$ の場合を扱いましょう。明らかに

$$
\sup_{c \in \mathscr{K}_1} |\langle\theta, cf\rangle| \leq \sup_{c \in \mathscr{B}_1} |\langle\theta, cf\rangle| \leq \langle|\theta|, |f|\rangle
$$

(Ch. IV, §4, No. 2、提案 2)。 On the other hand, let $g$ be an element of $\mathscr{K}(T; \mathbf{C})$ such that $|g| \leq |f|$; $g$ is the uniform limit of a sequence $(g_n)$ of elements of $\mathscr{K}(T; \mathbf{C})$ whose supports are contained in the open set $U$ formed by the $t$ such that $f(t) \neq 0$, and one may clearly suppose that $|g_n| \leq |f|$ for every $n$. $t \in U$の場合は集合、$c_n(t) = g_n(t)/f(t)$、$t \notin U$の場合は$c_n(t) = 0$。次に $c_n \in \mathscr{K}_1$、$g = \lim_{n \to \infty} c_n f$、したがって $|\langle\theta, g\rangle| = \lim_{n \to \infty} |\langle\theta, c_n f\rangle|$、そして最後に

$$
\sup_{|g| \leq |f|, g \in \mathscr{K}(T; \mathbf{C})} |\langle\theta, g\rangle| \leq \sup_{c \in \mathscr{K}_1} |\langle\theta, cf\rangle|.
$$

結論する x 観察するとで、この不等式の最初のメンバーが $\langle |\theta|, |f| \rangle$ に等しい (Ch. III, §1, No. 6, 公式 (12))。

次に、$\overline{\mathscr{L}}_C^1(\theta)$ の $f$ 元で表し、(4) が再び真であることを示します。この関係の 3 つのメンバーは、密集上で一致するであるため、$\overline{\mathscr{L}}_C^1(\theta)$ の位相について継続的に $f$ に依存することを検証するだけで十分です。 部分空間 $\mathscr{K}(T; \mathbf{C})$。これは、次の不等式からすぐに得られます。ここで、$f$ と $f'$ は、$\overline{\mathscr{L}}_C^1(\theta)$ の元を表します。

$$
|\langle |\theta|, |f| \rangle - \langle |\theta|, |f'| \rangle| \leq \langle |\theta|, |f - f'| \rangle = \overline{N}_1(f - f')
$$
$$
|\langle \theta, cf \rangle - \langle \theta, cf' \rangle| \leq \langle |\theta|, |c||f - f'| \rangle \leq \overline{N}_1(f - f')
$$

すべての$c \in \mathscr{B}_1$に。こうして補題が成立します。

命題 2 の移行 ～ 証明に、$h$ 属するを $\mathscr{K}_+(T)$ として、補題を写像 $uh$ に当てはめてみましょう。これにより、次の結果が得られます。

$$
\langle |\theta|, |uh| \rangle = \sup_{c \in \mathscr{K}_1} |\langle \theta, cuh \rangle| = \sup_{c \in \mathscr{K}_1} |\langle u \cdot \theta, ch \rangle| = \langle |u \cdot \theta|, h \rangle .
$$

ただし、最初のメンバーも次と等しくなります。

$$
\langle |\theta|, |u|h \rangle = \langle |u| \cdot |\theta|, h \rangle .
$$

したがって、2 つのメジャー $|u| \cdot |\theta|$ と $|u \cdot \theta|$ は等しいです。

#### 系 {#int-v-s5-n2-cor-1 .statement tag=092I}

*Let $g_1$ and $g_2$ be two locally $\mu$-integrable numerical functions; then*

$$
\inf(g_1 \cdot \mu, g_2 \cdot \mu) = \inf(g_1, g_2) \cdot \mu ; \quad \sup(g_1 \cdot \mu, g_2 \cdot \mu) = \sup(g_1, g_2) \cdot \mu .
$$

*特に、$g$ が局所的に $\mu$ 積分可能な数値写像である場合、*

$$
(g \cdot \mu)^+ = g^+ \cdot \mu ; \quad (g \cdot \mu)^- = g^- \cdot \mu .
$$

これは、第 2 章の提案 2 および公式 (6) からすぐに続きます。 II, §1, No. 1。

### 3. 稠密度で定義されたメジャーに関する積分

*この小節の主張では、$g$は正の数値写像を表し、どこでも局所的に$\mu$可積分可能に定義され、$\theta$は複素測度を表し、$u$は局所的に$\theta$可積分可能な複素数写像を表します。

No. 2の注意は、§4の結果が$\nu = g \cdot \mu = \int g(t) \varepsilon_t \, d\mu(t)$の尺度に適用できることを示しています（けれどもでも$g(t) \varepsilon_t$の尺度は定義されていません〜でない限り$g(t) \neq +\infty$）。したがって、次の主張が得られます。

#### 命題 3 {#int-v-s5-prop-3 .statement tag=092J}

*$T$ で定義されたすべての数値写像 $f \geqslant 0$ について、*

$$
\int^\bullet f \, d\nu = \int^\bullet (f g) \, d\mu .
$$

これはThから続きます。 §4, No. 2 の 1。

#### 系 1 {#int-v-s5-prop-3-cor-1 .statement tag=092K}

*In order that a function $\mathbf{f}$, with values in a Banach space or in $\overline{\mathbf{R}}$, be locally negligible for the measure $u \cdot \theta$, it is necessary and sufficient that $u \mathbf{f}$ be locally negligible for $\theta$.*

$\mathbf{f}$ (それぞれ $u \mathbf{f}$) が $u \cdot \theta$ (それぞれ $\theta$) に対して局所的に無視できるということは、$|\mathbf{f}|$ (それぞれ $|u| \cdot |\mathbf{f}|$) が $|u \cdot \theta|$ (それぞれ $|\theta|$) に対して局所的に無視できるというというと同等です。したがって、No. 2 の提案 2 を考慮すると、$\mathbf{f}, u, \theta$ が正である場合に帰着します。 主張は提案 3 からすぐに続きます。

#### 系 2 {#int-v-s5-prop-3-cor-2 .statement tag=092L}

*$u_1$ と $u_2$ を 2 つの局所的 $\theta$ 可積分複素数写像とします。 位数の $u_1 \cdot \theta = u_2 \cdot \theta$ では、$u_1$ と $u_2$ がほぼどこでも局所的に等しいことが必要かつ十分です。*

直ちに、$u \cdot \theta = 0$ が局所的にほぼどこでも $u(t) = 0$ を暗示することを示すことに帰着します。しかし、$u \cdot \theta = 0$ は、写像 1 が測度 $u \cdot \theta$ に対して局所的に無視できることを意味します。次に、系 1 が適用されます。

#### 系 3 {#int-v-s5-prop-3-cor-3 .statement tag=092M}

*$u$ を正の測度 $\mu$ に対して局所的に積分可能な複素数写像とします。 $u \cdot \mu$ が積極的な対策となるためには、ほぼどこでも局所的に $u(t) \geqslant 0$ が達成されることが必要かつ十分です。*

なぜなら、$u \cdot \mu$ は $u \cdot \mu = |u \cdot \mu| = |u| \cdot \mu$ の場合にのみ正であり (提案 2)、これはほぼどこでも局所的に $u = |u|$ と同等です (提案 2)。

#### 命題 4 {#int-v-s5-prop-4 .statement tag=092N}

*For a mapping $f$ of $T$ into a topological space $G$ to be measurable for the measure $u \cdot \theta$, it is necessary and sufficient that the restriction of $f$, to the $\theta$-measurable set $S$ of the $t$ such that $u(t) \neq 0$, be $\theta$-measurable.*

$u$ と $\theta$ が正の場合、これは §4, No. 3 の提案 3 からすぐに続きます。提案 2 のおかげで、$u$ と $\theta$ が複素数である場合の結果は拡大するになります。

#### 系 {#int-v-s5-n3-cor-1 .statement tag=092O}

*$\mathbf{f}$ を $T$ で定義された写像とし、Banach 空間 $F$ または $\overline{\mathbf{R}}$ で値を定義します。 $\mathbf{f}$ が $(u \cdot \theta)$ 測定可能であるためには、 $u \mathbf{f}$ が $\theta$ 測定可能であることが必要かつ十分です。*

なぜなら、$u \mathbf{f}$は$(u \mathbf{f})|S$から$T$の0により拡大になります。

#### 定理 1 {#int-v-s5-thm-1 .statement tag=092P}

*$\mathbf{f}$ を $T$ で定義された写像とし、Banach 空間 $F$ または $\overline{\mathbf{R}}$ で値を定義します。 $\mathbf{f}$ が測度 $\eta = u \cdot \theta$ に対して本質的に可積分である位数では、$uf$ が本質的に $\theta$ 可積分であることが必要かつ十分であり、その場合、

$$
\int f \, d\eta = \int (uf) \, d\theta .
$$

さらに、$u$ が連続で、すべての $t \in T$ に対して $u(t) \neq 0$ であると仮定します。この場合、$uf$ が $\theta$ に対して積分可能である場合に限り、$f$ は測度 $\eta$ に対して積分可能です。

Thから$u$と$\theta$が陽性のケースが一気に続きます。 §4, No. 4の2。 主張の最初と最後の主張がすぐに続きます。これは、$f$ が $|\eta| = |u| \cdot |\theta|$ に対して本質的に可積分 (可積分可能) である場合に限り、$\eta = u \cdot \theta$ に関して本質的に可積分 (可積分可能) であるためです。最後に、$f$ は本質的に $\eta$ (したがって $|\eta|$) に対して可積分であると仮定します。 分解 (2) を利用します。これらのメジャーは $\leq |\eta|$ であるため、$f$ は各メジャー $\eta_{ij} = g_i \cdot \mu_j$ ($i = 1, 2, 3, 4,\ j = 1, 2, 3, 4$) に対して本質的に積分可能です。私たちは持っています

$$
\int f \, d\eta_{ij} = \int g_i f \, d\mu_j .
$$

公式 (6) はこの直後に続きます。

#### 系 {#int-v-s5-n3-cor-2 .statement tag=092Q}

測度 $u \cdot \theta$ が制限されるためには、$u$ が本質的に $\theta$ 可積分であることが必要かつ十分です。

#### 例 {#int-v-s5-n3-exa-1 .statement tag=092R}

$A$ を $T$ の部分集合とします。 $\varphi_A$ が局所的に $\mu$ 可積分であるためには、$A$ が $\mu$ 可測であることが必要かつ十分です。 条件が満たされると仮定すると、集合 $\nu = \varphi_A \cdot \mu$; $T$ で定義されたすべての数値写像 $f \geq 0$ について、次のようになります。

$$
\int^\bullet f \, d\nu = \int^\bullet f \varphi_A \, d\mu ,
$$

$\int_A^\bullet f \, d\mu$ (cf. Ch. IV, §5, No. 6) によっても示される量。 $T$ の写像 $g$ をトポロジカル空間 $G$ が $\nu$ 可測となるためには、 $g$ の制限が $A$ であることが必要かつ十分です。 $\mu$-測定可能。 $T$ の写像 $f$ を Banach 空間 $F$ に、または $\overline{\mathbf{R}}$ が本質的に $\nu$ 積分可能であるためには、$f \varphi_A$ が本質的に $\mu$ 積分可能であることが必要かつ十分であり、その場合、

$$
\int f \, d\nu = \int f \varphi_A \, d\mu ,
$$

$\int_A f \, d\mu$ とも表される式。 $T$ の 2 つの写像が $A$ 上の $G$ (それぞれ $F, \overline{\mathbf{R}}$) 一致するになる場合、そのうちの 1 つが $\nu$ 可測 (本質的に $\nu$ 可積分) であるためには、もう一方もそうであることが必要かつ十分であることに注意してください。 今、$g$ が $T$ の任意の部分集合 $B \supset A$ の $G$ に写像である場合、任意の拡大が$A$ であれば、$g$ は *on* $\mu$ 測定可能であると言います。 $g$から$A$の制限の$T$は$\nu$で測定可能であり、これは$g$から$A$の制限が$\mu$で測定可能であるというというになります。 $B$ の写像 $f$ を Banach 空間 $F$ に、または $\overline{\mathbf{R}}$ に変換することは、拡大 $\overline{f}$ を * $A$ に * 本質的に* $\mu$ 積分可能であると言われています。 $f$ から $A$ の制限の $T$ は、本質的に $\nu$ 可積分です。 1、その後集合
$$
\int_A f \, d\mu = \int_A \overline{f} \, d\mu = \int \overline{f} \varphi_A \, d\mu,
$$
そしてある人は、$\int_A f \, d\mu$ は $A$ の *整* $f$ (または $A$ に *拡張) であると言います。 $f$ が $B \supset A$ で定義された数値写像 $\geqslant 0$ である場合、$\int_A^* f \, d\mu$ と $\int_A^\bullet f \, d\mu$ は 1 つの定義するになります。 Finally, a numerical function $g$ defined on $B \supset A$ is said to be *locally* $\mu$-integrable *on* $A$ if some extension $\overline{g}$ to $T$ of the restriction of $g$ to $A$ is locally $\nu$-integrable: this is equivalent to saying that, for every compact subset $K$ of $T$, $\overline{g} \varphi_{K \cap A}$ is $\mu$-integrable.

### 4. 通常の演算に対する積の動作

#### 命題 5 {#int-v-s5-prop-5 .statement tag=092S}

*$(\lambda_\alpha)_{\alpha \in A}$ *$T$、*関係* $\leqslant$、*$\mathscr{M}(T)$ *最高* $\lambda$ に向けた前向きな措置の家族にしましょう。 *正の数値写像* $g$ *局所的* $\lambda$-*積分可能であるためには、* $g$ *局所的* $\lambda_\alpha$-*すべてに対して積分可能* $\alpha \in A$ *そして家族* $(g \cdot \lambda_\alpha)$ *上に境界があること* $\mathscr{M}(T)$ が必要かつ十分です。 *この場合、
$$
g \cdot \lambda = \sup_{\alpha \in A} g \cdot \lambda_\alpha.
$$
条件が必要であることは明らかです。逆に、$g$ が各測度 $\lambda_\alpha$ に対して局所的に積分可能であり、族 $(g \cdot \lambda_\alpha)_{\alpha \in A}$ が上で有界であると仮定します。その最高値を$\lambda'$で示します。 写像 $g$ は $\lambda$ で測定可能です (§ 1, No. 4、提案 11 の Cor. 2)。さらに、写像 $h \in \mathscr{K}_+(T)$ ごとに、
$$
\int^\bullet (hg) \, d\lambda = \sup_{\alpha \in A} \int^\bullet (hg) \, d\lambda_\alpha = \sup_{\alpha \in A} \int^\bullet h \, d(g \cdot \lambda_\alpha) = \int^\bullet h \, d\lambda'
$$
(§ 1, No. 4、提案 11)。これは、まず、任意の $h$ に対して最初のメンバーが有限であるため、$g$ が局所的に $\lambda$ 可積分であることを意味します。したがって、記号 $\int^\bullet$ は $\int$ に置き換えられ、公式は $\int h \, d(g \cdot \lambda) = \int h \, d\lambda'$ と書かれる可能性があります。続いて$g \cdot \lambda = \lambda'$が続き、証明が完成します。

#### 系 {#int-v-s5-n4-cor-1 .statement tag=092T}

— $\mu$ が T 上のメジャーの族 $(\mu_\alpha)_{\alpha \in A}$ の和であるとします。 T 上で定義された正の数値写像 g が局所的に $\mu$ 積分可能であるためには、g がすべての $\alpha \in A$ について局所的に $\mu_\alpha$ 積分可能であり、族 $(g \cdot \mu_\alpha)_{\alpha \in A}$ が加算可能であることが必要かつ十分です。この場合、

$$
g \cdot \mu = \sum_{\alpha \in A} g \cdot \mu_\alpha.
$$

$(g_\alpha)_{\alpha \in A}$ を T 上で定義された $\mu$ 測定可能な正の写像の族とする。$S_\alpha$ を $g_\alpha(t) \neq 0$ となるような $t \in T$ の集合とする。家族 $(S_\alpha)$ が局所的に可算である場合、家族 $(g_\alpha)$ は *局所的に可算* であると言います (Ch. IV, §5, No. 9)。これは、T のすべてのコンパクト集合 K に対して、$g_\alpha|K$ が零ではない$\alpha \in A$ の集合が可算であるというになります。

#### 命題 6 {#int-v-s5-prop-6 .statement tag=092U}

— $(g_\alpha)_{\alpha \in A}$ を、T 上で定義された局所的 $\mu$ 積分可能な正の数値写像の局所的に可算な族とします。 写像 $g = \sum_{\alpha \in A} g_\alpha$ が局所的に $\mu$ 積分可能である位数では、メジャー $(g_\alpha \cdot \mu)_{\alpha \in A}$ の族が合計可能であることが必要かつ十分であり、その場合、

$$
g \cdot \mu = \sum_{\alpha \in A} g_\alpha \cdot \mu.
$$

$g$ が $\mu$ で測定可能であることは明らかです (第 2 章、IV, §5, No. 2、提案 4 およびNo. 4、修正 1)。したがって、$g$ が局所的に $\mu$ 可積分であるためには、$f \in \mathscr{H}_+(T)$ ごとに $\mu^\bullet(gf)$ が有限であることが必要かつ十分です。さて、$g_\alpha f \neq 0$ が可算であるような $\alpha \in A$ の集合なので、$\mu^\bullet(gf) = \sum_{\alpha \in A} \mu^\bullet(g_\alpha f)$ (§1, No. 1、提案 2 の補正) が得られます。 集合 $\nu_\alpha = g_\alpha \cdot \mu$; 条件 $\mu^\bullet(gf) < +\infty$ は条件 $\sum_{\alpha \in A} \nu_\alpha(f) < +\infty$ と同等です。他の語では、家族 $(\nu_\alpha)$ が加算可能な場合にのみ、$g$ はローカルで $\mu$ 積分可能です。この族の和を $\nu$ で表すと、前の計算では等式 $\nu(f) = \mu^\bullet(gf)$ が得られ、これは (8) と等価です。

#### 系 {#int-v-s5-n4-cor-2 .statement tag=092V}

— $(g_\alpha)$ を局所的 $\mu$ 可積分数値写像の数列とし、メジャー $g_n \cdot \mu$ の数列が増加するとなるようにします。この数列が T 上の実測度の順序付きベクトル空間 $\mathscr{M}(T)$ に上界をもつ位数では、写像 $g = \sup g_n$ が局所的に $\mu$ 積分可能であることが必要かつ十分です。 数列 $(g_n \cdot \mu)$ の $\mathscr{M}(T)$ の最高値は、メジャー $g \cdot \mu$ になります。

提案 6 を写像 (ほぼどこでも局所的に肯定的) $g'_n = g_{n+1} - g_n$ に適用するだけで十分です。

#### 命題 7 {#int-v-s5-prop-7 .statement tag=092W}

— X を無限で可算な局所的にコンパクトな空間とし、$t \mapsto \lambda_t$ を T の $\mathscr{M}_+(X)$ への $\mu$ に適した写像とする。

$g$ を、$X$ で定義された正の数値写像とし、測度 $\nu = \int \lambda_t d\mu(t)$ に対して局所的に積分可能とします。 $g$ が局所的に $\lambda_t$ 積分可能ではないような、$t \in T$ の集合は、$\mu$ について局所的に無視でき、写像 $t \mapsto g \cdot \lambda_t$ (局所的に $\mu$ - ほぼどこでも定義される) は $\mu$ で十分であり、

$$
g \cdot \nu = \int (g \cdot \lambda_t) d\mu(t).
$$

$(K_n)_{n \in \mathbf{N}}$ を、内部が $X$ をカバーする $X$ のコンパクト部分集合の増加する数列とします。 $\eta$ が $X$ に関する何らかの肯定的な測度である場合、$g$ が局所的に $\eta$ 可積分であると言うのは、$g \varphi_{K_n}$ がすべての $n$ について $\eta$ 可積分であるというと同等です。ここで、$H_n$ を $t \in T$ の集合として、$g \varphi_{K_n}$ が $\lambda_t$ 積分可能ではないようにし、$H = \bigcup_n H_n$ とします。 $H_n$ はすべての $n$ (§ 3, No. 3、Th. 1) に対して局所的に $\mu$ は無視できるため、同じことが $H$ にも当てはまり、主張の最初の主張が確立されます。 $H$ の $t$ に対して置き換えること $\lambda_t$ を 0 で計算すると ($\nu$ の尺度変更ではありません)、$g$ はすべての $t \in T$ に対して局所的に $\lambda_t$ 積分可能であると仮定できます。 $X$ に定義されたすべての $\nu$ 測定可能な陽性写像 $h$ について、§ 3, No. 2 の提案 3 と提案 5 により、

$$
\int^\bullet h d(g \cdot \nu) = \int^\bullet (gh) d\nu = \int^\bullet d\mu(t) \int^\bullet (gh) d\lambda_t = \int^\bullet d\mu(t) \int^\bullet h d(g \cdot \lambda_t).
$$

This formula and Prop. 5 of § 3, No. 2 first show (on taking $h \in \mathscr{K}_+(X)$) that the mapping $t \mapsto g \cdot \lambda_t$ is scalarly essentially $\mu$-integrable, and that its integral is $g \cdot \nu$; in other words, the relation (9) holds. 次に、正の尺度 $\mu' \leq \mu$ によって置き換える $\mu$ とし、$h$ を正の下半連続写像とします。これらの関係から、$t \mapsto g \cdot \lambda_t$ は $\mu$ 十分であることがすぐにわかります (§ 3, No. 1、定義 1)。

#### 命題 8 {#int-v-s5-prop-8 .statement tag=092X}

*$\theta$を$T$の複素測度、$g_1$を局所的に$\theta$可積分な複素数写像、$\theta_1$を測度$g_1 \cdot \theta$とする。 $T$ で定義された複素数写像 $g_2$ が局所的に $\theta_1$ 積分可能であるためには、$g_2 g_1$ が局所的に $\theta$ 積分可能であることが必要かつ十分であり、その場合*

$$
g_2 \cdot \theta_1 = g_2 \cdot (g_1 \cdot \theta) = (g_2 g_1) \cdot \theta
$$
(「結合性公式」)。

提案 4 の系により、$g_2$ が $\theta_1$ 可測であると言うのは、$g_2 g_1$ が $\theta$ 可測であるというというと同等です。この条件が満たされると仮定しましょう。 写像 $f \in \mathscr{K}_+(T)$ ごとに、命題 2 と 3 によって、

$$
\int^\bullet |g_2| f d|\theta_1| = \int^\bullet |g_2| f |g_1| d|\theta| = \int^\bullet |g_2 g_1| f d|\theta|.
$$

したがって、$g_2$ が局所的に $\theta_1$ 積分可能であると言うのは、$g_2 g_1$ が局所的に $\theta$ 積分可能であるというというと同等です。この条件が満たされると仮定すると、Th によって、 1 我々は持っています

$$
\int f \, d(g_2 \cdot \theta_1) = \int f g_2 \, d\theta_1 = \int f g_2 g_1 \, d\theta = \int f \, d(g_2 g_1 \cdot \theta),
$$

公式 (10) に相当します。

### 5. 基底 $\mu$ による対策の特徴付け

#### 定理 2 (ルベーグ–ニコディム) {#int-v-s5-thm-2 .statement tag=092Y}

— *$\mu$と$\nu$を$T$の2つの前向きな指標とします。次のプロパティは同等です:*

1) $\nu$ * は基底 $\mu$* の小節です。
2) *すべてのローカル $\mu$-無視できる集合は、ローカル $\nu$-無視可能*です。
3) *すべての$\mu$-無視できるコンパクト集合は$\nu$-無視可能*です。

1) が 2) を意味すること (提案 3 の訂正 1)、および 2) が 3) を意味することは明らかです。 3) が 1) を意味することを示します。まず、条件 3) が満たされる場合、*普遍的に測定可能*で局所的に $\mu$ が無視できるすべての集合 $A$ が局所的に $\nu$ が無視できることに注意します。 $\nu^\bullet(A) = \sup \nu(K)$ では、$K$ は、$A$ (§ 1, No. 3、提案 10、a) および第 6 章に含まれるコンパクト集合の集合を上回ります。 IV, § 4, No. 6、コル。 Thの2。 4)。次に補題を2つ確立します。

#### 補題 2 {#int-v-s5-lem-2 .statement tag=092Z}

— *$\alpha$ を $T$ の有界正の測度、$\beta$ を $|\beta| \leq M \alpha$ のような $T$ の実測度とし、$M$ は正の定数です。すると、$\beta = u \cdot \alpha$* となるような、実数写像 $u$, $\alpha$ 可積分が存在します。

$g$ を空間 $\mathscr{L}_\mathbf{R}^2(T, \alpha)$ の元とします。 $g$は$\beta$-測定可能であり、$\int^\bullet |g|^2 \, d|\beta| \leq M \int^\bullet |g|^2 \, d\alpha < +\infty$です。 写像 $g$ したがって、属するから $\mathscr{L}^2(T, |\beta|)$ になり、$\beta$ が有界であるため、$\mathscr{L}^1(T, |\beta|)$ にもなります。コーシー・シュワルツ不等式より、

$$
|\beta(g)|^2 \leq \left( \int |g| \, d|\beta| \right)^2 \leq \left( \int d|\beta| \right) \left( \int |g|^2 \, d|\beta| \right) \leq M^2 \alpha(1) \, \alpha(|g|^2).
$$

したがって、写像 $g \mapsto \beta(g)$ は、$\mathscr{L}^2(T, \alpha)$ で連続する線型形式です。ヒルベルト空間である$\mathscr{L}^2(T, \alpha)$ に関連付けられたハウスドルフ空間は、実際の写像 $u \in \mathscr{L}^2(T, \alpha)$ が存在します (TVS、Ch. V, § 1, No. 7、Th. 3)。したがって、所属から $\mathscr{L}^1(T, \alpha)$ も存在します。 $g \in \mathscr{L}^2(T, \alpha)$ごとに$\beta(g) = \alpha(ug)$。 $g \in \mathscr{K}(T)$ の適用この関係を見ると、$\beta = u \cdot \alpha$ であることがわかります。

#### 補題 3 {#int-v-s5-lem-3 .statement tag=0930}

— *正の尺度 $\nu$ が、すべての $\mu$ 無視できるコンパクト集合が $\nu$ 無視できるようなものであると仮定します。 $\mathfrak{K}$ を、以下の性質を持つコンパクト部分集合 $K$ の $T$ の集合とします。

(11) $\varphi_K \cdot \nu \leq M \varphi_K \cdot \mu$ となるような定数 $M \geq 0$ が存在します。
集合 $\mathscr{K}$ は、$T$ では $\mu$ 密になります。

If $K$ satisfies (11), and if $A$ is a Borel set contained in $K$, it follows at once from Prop. 8 that $\varphi_A \cdot \nu \leq M \varphi_A \cdot \mu$; from this, one deduces that the union of two elements $K, K'$ of $\mathscr{K}$ belongs to $\mathscr{K}$ because $\varphi_{K \cup K'} = \varphi_K + \varphi_A$, where $A = K' \cap \complement K$. 補題を確立するには、$\mu(L) > 0$ 含むとなるようなすべてのコンパクト集合 $L$ と、$\mu(K) > 0$ となるようなコンパクト集合 $K \in \mathscr{K}$ を証明する必要があります。 IV, §5, No. 8、提案 12)。 選ぶ数 $M > \nu(L)/\mu(L)$ を計算し、補題 1 を有界正のメジャー $\alpha = \varphi_L \cdot (\nu + M \mu)$ とメジャー $\beta = \varphi_L \cdot (\nu - M \mu)$ に適用します。 Replacing if necessary the function $u$ such that $\beta = u \cdot \alpha$ by a function equal to it $\alpha$-almost everywhere, one can suppose that $u$ is universally measurable (§3, No. 4, Prop. 7) and is zero outside of $L$. $t \in T$ の集合 $H$ は、$L$ に含まれる $u(t) < 0$ は $\mu$ 無視できません。その場合、$\nu$ は無視できます (Th. 2 の証明の初めに作成された注意によって)、したがって、$\alpha$ は無視でき、$M$ の矛盾する選択である $\beta(L) > 0$ が得られます。 $K$ を $H$ に含まれる圧縮集合とし、$\mu(K) > 0$ とします。 $K \in \mathscr{K}$ が補題を確立することを示しましょう。 提案 8 により、

$$
\varphi_K \cdot (\nu - M \mu) = \varphi_K \cdot \beta = \varphi_K \cdot (u \cdot \alpha) = (\varphi_K u) \cdot \alpha .
$$

写像 $\varphi_K u$ は負なので、確かに $\varphi_K \cdot \nu \leq M \varphi_K \cdot \mu$ になります。

ここで、定理 2 の証明を完成させましょう。 条件 3) が検証され、補題 3 のように定義する $\mathscr{K}$ が検証されたと仮定します。 $(K_\alpha)_{\alpha \in A}$ を、ペアごとに互いに素元の局所的に可算可能な族とします。 $\mathscr{K}$、集合 $N = T - \bigcup_{\alpha \in A} K_\alpha$ が局所的には $\mu$ 無視できるものとなる (Ch. IV, §5, No. 9、提案 14)。家族 $(K_\alpha)$ は局所的に可算可能であり、$N$ は普遍的に測定可能であるため、局所的に $\nu$ は無視できます。 集合 $\mu_\alpha = \varphi_{K_\alpha} \cdot \mu$、$\nu_\alpha = \varphi_{K_\alpha} \cdot \nu$; 写像 $\varphi_{K_\alpha}$ 形はローカルで可算可能な家族であり、その和は $\mu$ と $\nu$、命題のローカルほぼどこでも 1 に等しく、6 は $\mu = \sum_{\alpha \in A} \mu_\alpha$、$\nu = \sum_{\alpha \in A} \nu_\alpha$ を意味します。一方、$\mathscr{K}$の定義までに、$\alpha$ごとに$\nu_\alpha \leq M_\alpha \mu_\alpha$となるような定数$M_\alpha$が存在します。したがって、補題 2 は写像 $g_\alpha$ の存在を意味し、これは $K_\alpha$ の外側で零であり、$\nu_\alpha = g_\alpha \cdot \mu_\alpha$ のように正であると仮定できます (提案 3 の Cor. 3)。したがって (No. 4、提案 8)

$$
\nu_\alpha = g_\alpha \cdot \mu_\alpha = g_\alpha \cdot (\varphi_{K_\alpha} \cdot \mu) = (g_\alpha \varphi_{K_\alpha}) \cdot \mu = g_\alpha \cdot \mu .
$$

集合 $g = \sum_{\alpha \in A} g_\alpha$;家族 $(g_\alpha)$ は局所的に可算であり、家族 $(\nu_\alpha)$ は加算可能であるため、命題 6 は、$g$ が局所的に $\mu$ 可積分であり、$\nu = g \cdot \mu$ が暗黙的に示され、定理が確立されます。

#### 系 1 {#int-v-s5-thm-2-cor-1 .statement tag=0931}

— $\mathscr{N}$ を基底 $\mu$ による積極的な措置の集合とし、$\mathscr{M}(T)$ で最高$\nu$ を認めます。この場合、$\nu$ は基底 $\mu$ によるメジャーです。

コル。提案 2 により、$\mathscr{N}$ が増加する有向集合の場合への縮約が可能になります。ローカルで無視できる $\mu$ 集合 $A$ ごとに、§1, No. 4 の提案 11 により、

$$
\nu^\bullet(A) = \sup_{\lambda \in \mathscr{N}} \lambda^\bullet(A) = 0.
$$

したがって、定理 2 は、$\nu$ が基底 $\mu$ を含むメジャーであることを意味します。

#### 系 2 {#int-v-s5-thm-2-cor-2 .statement tag=0932}

— $\nu$ を $T$ の実際の尺度とします。完全格子配列空間 $\mathscr{M}(T)$ (Ch. II, §1, No. 5) の $\mu$ によって生成される帯域に $\nu$ 属するを加える位数では、$\nu$ が基底の尺度であることが必要かつ十分です。 $\mu$。

$\nu^+$ と $\nu^-$ を考慮すると、すぐに積極的な手段 $\nu$ の場合に帰着します (No. 2、提案 2 の修正)。それでは、集合 $\nu_n = \inf(n\mu, \nu)$ にしましょう。 $\nu$ 属するは、$\nu = \sup_n \nu_n$ の場合に限り、$\mu$ によって生成された帯域に適用されます (提案 6 の修正II, §1, No. 5)。さて、$\nu_n$ は、$n\mu$ によって上に囲まれており、基底 $\mu$ による Th によるメジャーです。 2;したがって、関係 $\nu = \sup_n \nu_n$ は、$\nu$ が基底 $\mu$ を含むメジャーであることを意味します (Cor. 1)。逆に、$\nu$ が基底 $\mu$: $\nu = g \cdot \mu$ の測度であるとします。ここで、$g$ は局所的に $\mu$ 積分可能で正です。次に、$\nu_n = \inf(g, n) \cdot \mu$ (提案 2 の修正)、そしてルベーグの定理 (Ch. IV, §4, No. 3、提案 4) からすぐに $\nu = \sup_n \nu_n$ が続きます。

#### 系 3 {#int-v-s5-thm-2-cor-3 .statement tag=0933}

— $\theta$ を複素測度としましょう。普遍的に測定可能な写像 $v$ が存在し、$|v| = 1$ は、$\theta = v \cdot |\theta|$、$|\theta| = \overline{v} \cdot \theta$ のようになります。

$\theta = \theta_1 - \theta_2 + i(\theta_3 - \theta_4)$、$\theta_1 = (\Re \theta)^+$、$\theta_2 = (\Re \theta)^-$、$\theta_3 = (\Im \theta)^+$、$\theta_4 = (\Im \theta)^-$ と書きます。ポジティブ測度 $\theta_i$ ($i = 1, 2, 3, 4$) は、$|\theta|$ (Ch. III, §1, No. 6, 公式 (17)) によって境界付けられており、基底 $|\theta|$ by 定理 2 による測度です。局所的に $|\theta|$ 積分可能な関数が存在することがわかります。 $v$ は $\theta = v \cdot |\theta|$ になります。 命題 2 は関係 $|\theta| = |v| \cdot |\theta|$ を生成します。これは、ほぼどこでも $|v| = 1$ が局所的に $|\theta|$ であることを意味します (提案 3 の Cor. 2)。最後に、提案 8、$\overline{v} \cdot \theta = (v \overline{v}) \cdot |\theta| = |\theta|$ によります。 写像 $v$ は局所的な $|\theta|$ が無視できる写像までのみ定義されているため、$v$ は普遍的に測定可能であり (§3, No. 4、提案 7)、どこでも $|v| = 1$ であると仮定できます。

#### 注意 1 {#int-v-s5-n5-rem-1 .statement tag=0934}

$\lambda$ が正の尺度であり、$v$ が $\lambda$ で測定可能な写像であるとします。その結果、$|v| = 1$ は局所的に $\lambda$ ほぼどこでも (これは、$v$ が局所的に $\lambda$ 可積分であることを意味します)、 $\theta = v \cdot \lambda$。提案 2 はすぐに $\lambda = |\theta|$ を示します。他の語、前述の主張の性質は、前向きの措置 $|\theta|$ を特徴づけています。

#### 注意 2 {#int-v-s5-n5-rem-2 .statement tag=0935}

$|\theta| \leq a \mu$ ($\mu$ がプラスの指標であり、$a$ が数 $\geq 0$ である場合) の場合、$\theta$ は基底 $\mu$ の指標になります。

#### 系 4 {#int-v-s5-thm-2-cor-4 .statement tag=0936}

— $\rho$ と $\theta$ を 2 つの複雑なメジャーとします。 $\rho = u \cdot \theta$ となるような局所的に $\theta$ 積分可能な関数 $u$ が存在する位数では、すべての $\theta$ 無視できるコンパクト集合が $\rho$ 無視可能であることが必要かつ十分です。

条件は明らかに必要です。逆に、すべての $\theta$-無視できるコンパクト集合が $\rho$-無視できると仮定します。 定理 2 は、$|\rho| = g \cdot |\theta|$ のような、局所的に $|\theta|$ 積分可能な関数 $g$ の存在を意味します。一方、Cor. 3 は、絶対的な値 1 で、$\rho = v_1 \cdot |\rho|$ (それぞれ $|\theta| = \overline{v_2} \cdot \theta$) のように、尺度 $|\rho|$ (それぞれ $\theta$) で測定可能な写像 $v_1$ (それぞれ $v_2$) の存在を意味します。次に、提案 8 により、$\rho = u \cdot \theta$ と $u = v_1 g \overline{v_2}$ が決まります。

#### 系 5 {#int-v-s5-thm-2-cor-5 .statement tag=0937}

— $\mu$ と $\nu$ を T に関する 2 つの肯定的な尺度とします。 条件 Th の 1)、2)、3)。 2 は次のものとも同等です。

4) すべての $\nu$ 可積分数値写像 $f \geq 0$ およびすべての数 $\varepsilon > 0$ に対して、関係 $0 \leq h \leq f$ および $\int^* h \, d\mu \leq \delta$ が $\int^* h \, d\nu < \varepsilon$ を暗示するような $\delta > 0$ が存在します。

5) すべての写像 $g \in \mathscr{K}_+(\mathrm{T})$ とすべての数 $\varepsilon > 0$ に対して、$g$ と満たす $\int h \, d\mu \leq \delta$ で囲まれたすべての $h \in \mathscr{K}_+(\mathrm{T})$ に対して、$\int h \, d\nu \leq \varepsilon$ が存在するような $\delta > 0$ が存在します。

6) すべてのコンパクト集合 $K \subset \mathrm{T}$ とすべての数 $\varepsilon > 0$ に対して、関係 $A \subset K$ と $\mu^*(A) \leq \delta$ が $\nu^*(A) \leq \varepsilon$ を暗示するような $\delta > 0$ が存在します。

4) $\Rightarrow$ 6) $\Rightarrow$ 3) の意味は明らかです。

$\nu = k \cdot \mu$ など、普遍的に測定可能で局所的に $\mu$ 積分可能な有限の写像 $k \geq 0$ が存在すると仮定し、条件 4) が満たされることを示しましょう。 $f$ を $\nu$ 可積分関数 $\geq 0$ とし、$\varepsilon > 0$ とします。すべての整数 $n \geq 0$ について、$A_n$ を $t \in \mathrm{T}$ の集合とし、$k(t) \geq n$ とします。 写像 $f \varphi_{A_n}$ 形減少列は、その上が $f$ で囲まれ、点方向に 0 に向かう傾向があるため、$\int f \varphi_{A_N} \, d\nu \leq \varepsilon/2$ となるような $N$ が存在します (Ch. IV, §4, No. 3、提案 4)。 $h$ が $\mathrm{T}$ 満たす $0 \leq h \leq f$ および $\int^* h \, d\mu \leq \varepsilon/2N$ で写像である場合、

$$
\nu^*(h) \leq \nu^*(h \varphi_{A_N}) + \nu^*(h(1 - \varphi_{A_N}))
$$
$$
\leq \nu^*(f \varphi_{A_N}) + \mu^*(h(1 - \varphi_{A_N})k)
$$
$$
\leq \frac{\varepsilon}{2} + N \mu^*(h) \leq \varepsilon.
$$

したがって、条件 4) と 6) が Th の条件と同等であることが証明されました。 2.

4) が 5) を意味することは明らかです。最後に、条件 5) が満たされる場合、$\mu$ (Ch. II, §2, No. 2、提案 5) によって生成された帯域に $\nu$ 属するが​​適用され、したがって基底 $\mu$ (Cor. 2) になります。

#### スコリウム {#int-v-s5-n5-sch-1 .statement tag=0938}

$\dot{f} \in L^1_{\mathrm{loc}}(\mathrm{T}, \mu; \mathbf{R})$、集合 $\varphi(\dot{f}) = f \cdot \mu$ ごとに、$f \in \dot{f}$; 写像 $\varphi$ は線形、増加するおよび単射的 (提案 3 の Cor. 2)、および $\mathscr{M}(T)$ の像は $\mu$ (Th. 2 の Cor. 2) によって生成されるバンド B です。したがって、写像 $\varphi$ により、$L^1_{\text{loc}}(T, \mu; \mathbf{R})$ を T の実測度の空間と識別することができます。 空間 $L^p_R(T, \mu)$ はすべて $L^1_{\text{loc}}(T, \mu; \mathbf{R})$ の部分空間であるため、それらも $\mathscr{M}(T)$ の部分空間と同一視される可能性があります。同様の考慮事項が複素数値写像とメジャーにも当てはまります。上記で考慮された写像 $\varphi$ は、$L^1_{\text{loc}}$ と B の順序付けられたベクトル空間構造の同型ですが、これらの *トポロジカルベクトル空間* 構造では明らかに同型ではないことに注意してください。 空間。

完全に格子配列された空間のすべてのバンドはそれ自体完全に格子配列された空間 (Ch. II, §1, No. 5) であるため、空間 $L^1_{\text{loc}}$ は *完全に格子配列* であることがわかります。しかし、同値類の不可算族 $(\dot{f}_\alpha)$ の $L^1_{\text{loc}}$ の最高値は、写像 $f_\alpha$ の上部包絡線の類と必ずしも同一ではないことを思い出す価値があります。しかし、上部包絡線 $f$ が局所 $\mu$ 積分可能である局所 $\mu$ 積分可能な関数の *増加する数列* $(f_n)$ では、$f \cdot \mu$ が測度 $(f_n \cdot \mu)$ の数列の上限であることが分かりました。 $\mathscr{M}(T)$ (提案 6 の修正)。

これは Th の系 3 の興味深い帰結です。 2:

#### 命題 9 {#int-v-s5-prop-9 .statement tag=0939}

*$\theta$ を有界複素測度とする。 $\theta$ が前向きの尺度であるためには、$\| \theta \| = \theta(1)$.* であることが必要かつ十分です。

条件は明らかに必要です。逆に、$\| \theta \| = \int d\theta$ と仮定し、$\theta = v \cdot |\theta|$ となるような絶対値 1 の $|\theta|$ 可測写像を $v$ で表します。 $\| \theta \| = \int d|\theta|$ (Ch. IV, §4, No. 7、提案 12) と $\int d\theta = \int v \cdot d|\theta|$ (Th. 1) 以来、仮定は $\int (1 - v) \, d|\theta| = 0$、したがって $\int \mathscr{R}(1 - v) \, d|\theta| = 0$ を意味します。 写像 $\mathscr{R}(1 - v)$ は正なので、ほぼどこでも零であり、これは $v = 1$ がほぼどこでもで、証明が完成することを意味します。

### 6. 同等の措置

#### 命題 10 {#int-v-s5-prop-10 .statement tag=093A}

*$\mu$ と $\nu$ を T の 2 つの肯定的な尺度とします。次の条件は同等です。
a) 局所的に無視できる集合は、$\mu$ と $\nu$ で同じです。
b) $\mathscr{M}(T)$ の $\mu$ と $\nu$ によって生成されたバンドは同一です。
c) 1 つは $\nu = g \cdot \mu$ で、$g$ は局所的に $\mu$ 積分可能であり、$\mu$ のほぼどこでも局所的に $g(t) > 0$ です。

条件 a) と b) は Cor によって同等です。 Thの2。 No. 5の2。それらが満足される場合、$\nu = g \cdot \mu$ と $\mu = h \cdot \nu$ になります。ここで、$g$ (それぞれ $h$) は正であり、$\mu$ (それぞれ $\nu$) に対して局所的に積分可能です。したがって、(No. 4、提案 8) $hg$ は局所的に $\mu$ 積分可能であり、$\mu = (hg) \cdot \mu$ です。 (No. 3、提案 3 の Cor. 2) $hg$ は、$\mu$ については局所的にほぼどこでも 1 に等しいため、$\mu$ については局所的にほぼどこでも $g(t) > 0$ と $h(t) = 1/g(t)$ が 1 に等しいことがわかります。逆に、$\mu$ のほぼどこでも局所的に $g(t) > 0$ を伴う $\nu = g \cdot \mu$ を仮定します。

$(1/g)g$ はほぼどこでもローカルに定義されており、ローカルで $\mu$ 積分可能であるため、$1/g$ はローカルで $\nu$ 積分可能であり、$(1/g) \cdot \nu = \mu$ (No. 4、提案 8)。

#### 定義 3 {#int-v-s5-def-3 .statement tag=093B}

*局所コンパクト空間 $T$ 上の 2 つの複素尺度 $\theta, \theta'$ は、提案 10 の尺度 $|\theta|$ および $|\theta'|$ 満たす条件 a)、b)、c) が等しい場合、同等であると言われます。

従って、$\theta$ と $\theta'$ が同等であるためには、$|\theta|$ と $|\theta'|$ が同等であることが必要かつ十分です。

#### 注意 {#int-v-s5-n6-rem-1 .statement tag=093C}

— $\mu$ と $\nu$ が 2 つの等価な肯定的な測度である場合、$T$ で定義される可測写像は、位相幾何学的空間 $G$ の値とともに、$\mu$ と $\nu$ について *同じ* であり、これは、次の提案 4 からすぐにわかります。 No. 3。

#### 命題 11 {#int-v-s5-prop-11 .statement tag=093D}

*$\mu$を$T$に対するプラスの尺度とします。 $T$ が無限に可算である場合、すべての $t \in T$ に対して $h(t) > 0$ となり、測度 $\nu = h \cdot \mu$ ($\mu$ に相当) が有界であるような連続写像 $h$ が存在します。

Let $(K_n)$ be a sequence of compact sets forming a covering of $T$ and, for every $n$, let $f_n$ be a function in $\mathscr{H}(T)$ such that $0 \leq f_n \leq 1$ and $f_n(t) = 1$ on $K_n$ (Ch. III, §1, No. 2、補題 1)。 $(a_n)$ を数 $> 0$ の数列として、$\sum_n a_n < +\infty$ とします。 系列 $h = \sum_n a_n f_n$ は通常 $T$ に収束し、その結果、$h$ は $T$ 上で連続する写像となり、構成によってすべての $t \in T$ に対して $h(t) > 0$ になります。 設定 $\nu = h \cdot \mu$ とすると、(提案 3 と第 4 章 ) となります。 IV, §1, No. 3、提案 13)

$$
\nu^*(1) = \int^* h \, d\mu \leq \sum_n a_n \int f_n \, d\mu .
$$

たとえば、$\int f_n \, d\mu > 1$の場合は$a_n = 2^{-n} (\int f_n \, d\mu)^{-1}$、それ以外の場合は$a_n = 2^{-n}$とすると、$\sum_n a_n < +\infty$と$\nu^*(1) < +\infty$があり、命題が証明されます。

#### 命題 12 {#int-v-s5-prop-12 .statement tag=093E}

*$(\mu_n)$ を $T$ の有界ポジティブ指標の数列とします。 $T$ には、関係 $\mu^*(N) = 0$ が «すべての $n$ について$\mu_n^*(N) = 0$ に相当するような、有界正の尺度 $\mu$ が存在します。各メジャー $\mu_n$ には基底 $\mu$ があります。さらに、$\mu'$がこの性質を持つ$T$に対する2番目の肯定的な尺度である場合、$\mu$と$\mu'$は同等です*。

主張の最後の部分は、Def からすぐに続きます。 3. $\mu$ の存在を証明するには、$n$ ごとに $\mu_n \neq 0$ である場合に限定できます。メジャーの族 $\mu_n / 2^n \| \mu_n \|$ は $\mathscr{M}(T)$ で合計可能であり、その和 $\mu$ は $\| \mu \| \leq 1$ となります。さらに、$\mu_n \leq 2^n \| \mu_n \| \cdot \mu$ から、関係 $\mu(N) = 0$ は、すべての $n$ に対して $\mu_n(N) = 0$ を意味します。逆に、$N$ がすべての $\mu_n$ に対して無視できる集合である場合、$\mu$ については局所的に無視できます。

(§2, No. 2、提案 1 の Cor. 2)、したがって、$\mu$ は有界であるため、$\mu$ は無視できます (§1, No. 2、提案 7 の Cor. 2)。

### 7. 外国人対策

$T$ に 2 つの実際の尺度 $\rho, \sigma$ が与えられた場合、$\mathscr{M}(T)$ で $\inf(|\rho|, |\sigma|) = 0$ の場合、$\rho$ と $\sigma$ は（互いに）異質であると言われることを思い出してください。 II, §1, No. 1)。 特定のメジャーとは異なる実際のメジャーは、バンドで形知られています (Ch. II, §1, No. 5、木。 1)。 この定義は、複雑な措置の場合にも直ちに拡張される可能性があります。

#### 定義 4 {#int-v-s5-def-4 .statement tag=093F}

*$T$の複雑な測度$\theta$は$T$の部分集合$M$に集中している、または$\mathbf{C}M$が$\theta$に対して局所的に無視できる場合、$M$は$\theta$を運ぶとも言われています。

集合 $M$ は、$|\theta|$ を運ぶ場合に限り、$\theta$ を運びます。 それは、$M$ が $\theta$ を運ぶ、または $M$ が $\theta$ 可測であり、$\theta = \varphi_M \cdot \theta$ であると言うのと同じです。 $\theta$ が $M$ に集中している場合、基底 $|\theta|$ のすべてのメジャーは $M$ に集中しています。

#### 命題 13 {#int-v-s5-prop-13 .statement tag=093G}

*$T$上の2つの複素測度$\rho$と$\sigma$が互いに異質である位数において、$T$には$\rho$が集中するように2つの互いに素集合$R$と$S$が存在することが必要十分である。 $S$の$R$と$\sigma$。 $R$ と $S$ は普遍的に測定可能であると考えられるかもしれません。*

集合 $\mu = |\rho|$、$\nu = |\sigma|$、$\lambda = \mu + \nu$; $\mu$ と $\nu$ は上で $\lambda$ によって制限されているため、$\mu = u \cdot \lambda$、$\nu = v \cdot \lambda$ などの 2 つのローカルで $\lambda$ 積分可能な関数 $u$ と $v$ (これは§3, No. 4、提案 7 によって普遍的に測定可能であると想定できます) が存在します。それから

$$
\inf(|\rho|, |\sigma|) = \inf(\mu, \nu) = \inf(u, v) \cdot \lambda
$$

(No. 2、提案 2 の修正)。 $A$ (それぞれ $B$) を $t \in T$ の集合とし、$u(t) > 0$ と $v(t) = 0$ (それぞれ $u(t) = 0$ と $v(t) > 0$) とします。 $\rho$ と $\sigma$ が異質である場合、$\inf(u, v) = 0$ は局所的に $\lambda$ - ほぼどこでも (No. 3、提案 3 の Cor. 2)、したがって互いに素は普遍的に測定可能集合 $A$ と $B$ は次のようになります。それぞれ$\mu$と$\nu$。逆に、$\mu$ と $\nu$ が、それぞれ互いに素集合 $R$ と $S$ によって運ばれるとします。 $\varphi_R$ は、$\mu = u \cdot \lambda$ および $\mu = \varphi_R \cdot \mu$ のメジャーで測定可能です。 No. 4 の提案 8 により、写像 $u' = u \varphi_R$ は $\lambda$ 可測であり、$\mu = u' \cdot \lambda$ です。同様に、$v' = v \varphi_S$ の場合は $\nu = v' \cdot \lambda$ です。 1 つは結論するで、$\inf(u', v') = 0$ (No. 2、提案 2 の修正) と述べています。

#### 系 1 {#int-v-s5-prop-13-cor-1 .statement tag=093H}

*$T$ 上の各実際のメジャー $\nu$ には、それぞれ $\nu^+$ と $\nu^-$ を運ぶ 2 つの互いに素集合 $M, N$ が存在します。

$\nu$の指標を支持する概念と、$\nu$が集中する集合の支持を混同しないように注意しなければなりません。 $\nu$ のサポート S は、$\nu$ を運ぶ最小のクローズ集合 (Ch. III, § 2, No. 2、提案 2 および Ch. IV, §2, No. 2、提案 5)。ただし、S とは異なり、$\nu$ を運ぶ S の部分集合が存在する可能性があります。より一般的には、同じサポートを持つ 2 つのポジティブな指標 $\mu$ と $\nu$ に対して $\inf(\mu, \nu) = 0$ を得ることができます (例 5)。

注意また、$\nu$ を運ぶ集合の共通部分は点 $t \in T$ の集合であるため、$|\nu|(\{t\}) > 0$ は空になる可能性があります (たとえば、ルベーグ測度の場合)。したがって、一般に最小の集合が $\nu$ を運ぶことはありません。

#### 系 2 {#int-v-s5-prop-13-cor-2 .statement tag=093I}

— $\rho$ と $\sigma$ を 2 つの異質な複素尺度とし、$\rho'$ と $\sigma'$ をそれぞれ $\rho$ と $\sigma$ に対する密度を許容する 2 つの複素尺度とします。その場合、$\rho'$ と $\sigma'$ はエイリアンです。

#### 系 3 {#int-v-s5-prop-13-cor-3 .statement tag=093J}

— $\rho$ と $\sigma$ を 2 つの異質な複雑な尺度とします。それから$|\rho + \sigma| = |\rho| + |\sigma|$。

$v$ (それぞれ $w$) によって、$\rho = v \cdot |\rho|$ (それぞれ $\sigma = w \cdot |\sigma|$) (Th. 2 の Cor. 3) となるような絶対値 1 の普遍的に測定可能な写像を表し、A によって普遍的に測定可能な集合を運ぶ$\rho$、$B = \mathbf{C}A$ が$\sigma$ を運ぶ (提案 13)。それから$\rho + \sigma = (v \varphi_A + w \varphi_B) \cdot (|\rho| + |\sigma|)$も。 写像 $v \varphi_A + w \varphi_B$ の絶対値値は 1 に等しいため、系は提案 2 に従います。

#### 定理 3 (ルベーグ) {#int-v-s5-thm-3 .statement tag=093K}

— T 上のすべての複雑な測度 $\theta$ は、形 $\theta = g \cdot \mu + \theta'$ で唯一の 1 つの方法で書くことができます。ここで、$g$ は局所的に $\mu$ 積分可能であり、$\theta'$ は $\mu$ とは異質な測度です。それから$|\theta| = |g| \cdot \mu + |\theta'|$。

$\theta$ が正の場合、これは、F. Riesz (Ch. II, §1, No. 5、Th. 1) の定理を、T 上の完全に格子順序付けされた実測度の空間 $\mathscr{M}(T)$ と、この空間の $\mu$ によって生成された帯域に適用して、すぐに続きます。アカウント Cor. No. 5の2、Th。 2;さらに、$\theta'$ と $g \cdot \mu$ は正であり、これは、$g$ が局所的に $\mu$、ほぼどこでも正であることを意味します (提案 3 の Cor. 3)。 $\theta$ が正ではない、集合 $\nu = |\theta|$、$\nu = f \cdot \mu + \nu'$ ($f$ が正で、$\nu'$ と $\mu$ が互いに異質である)、および $\theta = v \cdot \nu$ ($v$ は普遍的に測定可能な値である) の場合を処理します。絶対的な値 1 の写像 (Th. 2 の Cor. 3)。次に、(提案 8) $\theta = g \cdot \mu + \theta'$、$g = v f$ (つまり $|g| = f$) と $\theta' = v \cdot \nu'$ (つまり提案 2 により $|\theta'| = \nu'$) が得られます。 $\theta'$ と $\mu$ は Cor によって互いに異質です。提案 13 の 2。あとは一意性の分解を確立するだけです。したがって、$\theta'$ と $\theta'_1$ が $\mu$ とは異質である $\theta = g \cdot \mu + \theta' = g_1 \cdot \mu + \theta'_1$ と仮定します。 $|\theta' - \theta'_1|$ は上で $|\theta'| + |\theta'_1|$ によって境界付けられているため、$\theta' - \theta'_1$ は $\mu$ に対して異質であり、したがって $(g_1 - g) \cdot \mu$ にも異質です。 関係 $\theta' - \theta'_1 = (g_1 - g) \cdot \mu$ は、2 人のメンバーが零であることを意味し、一意性であることが証明されます。

空間 $L^1_{loc}(T, \mu; \mathbf{C})$ が (写像 $g \mapsto g \cdot \mu$ によって) $\mathscr{M}_\mathbf{C}(T)$ の部分空間と識別される可能性があること (No. 5、Th. 2 および Scholium) を思い出してください。この規則により、定理 3 は次の形をとります。

#### 系 {#int-v-s5-n7-cor-1 .statement tag=093L}

— *空間 $L^1_{\text{loc}}(T, \mu; \mathbf{C})$ 上に空間 $\mathscr{M}_\mathbf{C}(T)$ の射影子 p が存在し、その核 $\overline{p}^{-1}(0)$ は $\mu$ とは異質な複雑な測度の集合であり、次のような*

$$
|\theta| = |p(\theta)| + |\theta - p(\theta)|,\quad p(|\theta|) = |p(\theta)|
$$

*すべての複雑なメジャー $\theta$.*

$p$ が有界メジャーの集合に制限されている場合、空間 $\mathscr{M}_\mathbf{C}^1(T)$ の射影子 $p^1$ が空間 $L^1_\mathbf{C}(T, \mu)$ に得られます。 関係 $\| \theta \| = |\theta|(1)$ は、すべての有界複素測度 $\theta$ に対して $\| \theta \| = \| p^1(\theta) \| + \| \theta - p^1(\theta) \|$ を意味します。

### 8. アプリケーション: I。 空間 $L^p$ の二重性

ここでは、実際の空間 $L^p$ の場合のみを扱います。

$1 \leq p \leq +\infty$、$1 \leq q \leq +\infty$、$1/p + 1/q = 1$ のような 2 つの数 $p, q$ が *共役指数* と言われていることを思い出してください (Ch. IV, §6, No. 4)。 写像 $g \in \mathscr{L}^q$ 定義するごとに、$\mathscr{L}^p$ の線型形式 $f \mapsto \int fg\,d\mu$ から始まる移行から商によって得られる、$L^p$ の連続線型形式 $\theta_g$ $N_q(g) = \| \theta_g \|$ (Ch. IV, §6, No. 4、提案 3 の修正)。 移行から商まで、写像 $g \mapsto \theta_g$ から $L^q$ の等角線形写像 $\varphi$ を$L^p$ の双対$(L^p)'$ に演繹します。 $1 \leq p < +\infty$、$\varphi$ 写像 $L^q$ *上* $(L^p)'$ を示し、今後同一視するバナハ空間 $L^q$ をバナハ空間とできるようにします同型 $\varphi$ により $(L^p)'$ 。その他項に記載:

#### 定理 4 {#int-v-s5-thm-4 .statement tag=093M}

— *p と q を 2 共役指数として、$1 \leq p < +\infty$ とします。 $\mathscr{L}^p(T, \mu)$ 上のすべての連続線型形式は型 $f \mapsto \int fg\,d\mu$ です。ここで、g は $\mathscr{L}^q(T, \mu)$ の写像であり、$L^q$ の類は明確に定義されています。*

$\theta$ を $\mathscr{L}^p$ で連続する線型形式とします。従って、写像 $f \in \mathscr{L}^p$ ごとに $|\theta(f)| \leq a \cdot N_p(f)$ となるような数 $a \geq 0$ が存在します。コンパクトサポートを持つ$\theta$の制限から連続写像の空間$\mathscr{K}(T)$を考えてみましょう:Tのすべてのコンパクト部分集合Kとすべての写像$f \in \mathscr{K}(T, K)$(Kに含まれるコンパクトサポートを持つ連続写像の空間)について、 $N_p(f) \leq (\mu(K))^{1/p} \| f \|$;従って、$\mathscr{L}^p$の$\mathscr{K}(T, K)$によって誘導される位相は、一様収束の位相より粗く、$\theta$から各$\mathscr{K}(T, K)$への制限は、結果的に後者の位相に対して連続となります。これは、$\theta$ から $\mathscr{K}(T)$ の制限が *実際の尺度* $\nu$ であることを意味します (Ch. III, §1, No. 3、定義 2)。

$\mathscr{K}(T)$ のすべての写像 $f$ が $|\nu|(|f|) \leq a \cdot N_p(f)$ であることを示しましょう。これを$f \geq 0$に対して公式を証明すれば十分です。さて、$|\psi| \leq f$ などの $\mathscr{K}(T)$ のすべての写像 $\psi$ について、
$$
|\nu(\psi)| \leq a \cdot N_p(\psi) \leq a \cdot N_p(f);
$$
私たちの主張は、第 4 章で与えられた測定値の絶対値値の式から得られます。 III, §1, No. 6、公式 (12)。 関係 $|\nu|(|f|) \leq a (\mu(|f|^p))^{1/p}$ 拡大するは、$f$ がコンパクト集合の特性写像である場合に、下側エンベロープへの通過によって一度に適用され、すべての $\mu$ 無視できるコンパクト集合が$\nu$ は無視できるため、$\nu$ は * 基底* $\mu$ (No. 5、Th. 2) を含むメジャーです。

従って、すべての写像 $f \in \mathscr{K}(T)$ に対して $|\nu|(f) = \int f h_1 d\mu$ となるような、局所的に $\mu$ 積分可能な正の写像 $h_1$ が存在します。 $h_1$ が局所的にほぼどこでも $\mathscr{L}^q$ の写像に等しいことを示しましょう。 $\mathscr{K}(T)$ の写像 $f \geq 0$ が $N_p(f) \leq 1$ となる場合、$\int f h_1 d\mu = |\nu|(f) \leq a$ になります。従って、コンパクトなサポートを使用して、T の写像 $f_0$ が $[0,1]$ に連続する場合、$f$ が $\mathscr{K}(T)$ で写像 $\geq 0$ の集合を実行するため、$N_p(f) \leq 1$ のように $\sup \int (f_0 h_1) f d\mu \leq a$ が得られます。このことから、第 8 章の公式 (11) によって推測されます。 IV, §6, No. 4、あの$N_q(f_0 h_1) \leq a$。このことから、K が T の圧縮部分集合の集合を超えると $\sup_{K} N_q(\varphi_K h_1) \leq a$ が得られ、これは私たちの主張 (§1、提案 9) を証明します。

$v$ を、$\nu = v \cdot |\nu|$ (Th. 2 の Cor. 3) となるような絶対値 1 の普遍的に測定可能な (実数) 写像とし、$g = v h_1$ とします。次に$\nu = g \cdot \mu$、$g$属するから$\mathscr{L}^q$となります。 写像 $f \in \mathscr{K}(T)$ ごとに、$\theta(f) = \nu(f) = \int f g d\mu$ があります。他の語では、$\mathscr{K}(T)$に線型形式$\theta$と$\theta_g$一致するが連続します。従って、$\mathscr{K}(T)$ は$\mathscr{L}^p$ で密であるため、$\mathscr{L}^p$ では等しく、これで証明が完成します。

#### 系 {#int-v-s5-n8-cor-1 .statement tag=093N}

— *$1 < p < +\infty$ となるすべての数 p に対して、バナッハ空間 $L^p(T, \mu)$ は再帰的です。*

一般に、$L^\infty$ の双対は $L^1$ と同型ではないため、$L^1$ と $L^\infty$ は再帰的ではありません (Exer. 10)。 $\mathscr{L}^\infty$の$g \mapsto \int f g d\mu$から$g \in \mathscr{L}^1$の線型形式から商への通過によって、$L^\infty$の連続線型形式を特徴づけます。

順序付けられたベクトル空間 $L^\infty(T, \mu)$、つまり $L^1_{loc}(T, \mu)$ の部分空間は *完全に格子順序付けされています*。なぜなら、$(f_\alpha)$ が $\mathscr{L}^\infty$ の正の写像の族で、類 $(\dot{f}_\alpha)$ の集合が $L^\infty$ で上に制限されている場合、すべての $\alpha$ に対して $N_\infty(f_\alpha) \leq a$ となるような $a \geq 0$ が存在します。 $L^1_{loc}(T, \mu)$ は完全に格子順序付けされているため、族 $(\dot{f}_\alpha)$ は $L^1_{loc}(T, \mu)$ の最高値 $\dot{h}$ を認めます。しかし、$\alpha$ごとに$\dot{a} \geq \dot{f}_\alpha$なので、$\dot{h} \leq \dot{a}$となり、その結果、$N_\infty(h) \leq a$、よってが主張となります。

#### 命題 14 {#int-v-s5-prop-14 .statement tag=093O}

— *位数において、$\mathscr{L}^\infty$ のポジティブな線型形式 $\theta$ は型 $f \mapsto \int f g d\mu$ のものであり、$g \in \mathscr{L}^1$ では、* 増加するのすべての増加するの家族 $(f_\alpha)_{\alpha \in A}$ がポジティブな写像であることが必要かつ十分です。 $\mathscr{L}^\infty$ の類 $(\dot{f}_\alpha)_{\alpha \in A}$ の集合は $L^\infty$ で上に制限され、$\dot{h}$ をこの空間の最高値として認めます。

$$
\theta(h) = \sup_{\alpha \in A} \theta(f_\alpha).
$$

まず、条件が必要であることを示しましょう。 $h \cdot \mu$ は、$f_\alpha \cdot \mu$ (No. 5、Scholium) の集合の $\mathscr{M}(T)$ における最高値です。したがって (Ch. II, §2, No. 2)、$\mathscr{K}(T)$ の写像 $\varphi \geq 0$ ごとに、$\int h \varphi \, d\mu = \sup_{\alpha \in A} \int f_\alpha \varphi \, d\mu$ が得られます。ここで、$a$ が数 $\geq 0$ で、すべての $\alpha \in A$ に対して $N_\infty(f_\alpha) \leq a$ となる場合 (これは $N_\infty(h) \leq a$ を意味します)、すべての $\varepsilon > 0$ に対して $\varphi \geq 0$ と $N_1(g - \varphi) \leq \varepsilon$ となる $\varphi \in \mathscr{K}(T)$ が存在し、そこから次のように推測されます。 $\alpha \in A$、および$\int h |g - \varphi| \, d\mu \leq a \varepsilon$すべてに対して$\int f_\alpha |g - \varphi| \, d\mu \leq a \varepsilon$。 $\sup_{\alpha \in A} \int f_\alpha g \, d\mu \leq \int h g \, d\mu$ 以降、この不等式の 2 つのメンバーが等しいことが証明されます。

条件で十分であることを確認するには、次の補題を使用します。

#### 補題 4 {#int-v-s5-lem-4 .statement tag=093P}

1° *$f$ を、$T$ 上の半連続かつ有界の正の写像とします。次に、$L^\infty$ の類 $\dot{f}$ は、類 $\dot{\varphi}$ の集合の上限であり、$\varphi$ は、$\mathscr{K}(T)$ の写像の集合を超え、$0 \leq \varphi \leq f$ のようになります。

2° * $f$ を、$T$ 上の測定可能で有界な正の写像とします。次に、$L^\infty$ の類 $\dot{f}$ は、類 $\dot{\psi}$ の集合の下限であり、$\psi$ は、$T$ の下部半連続および有界写像の集合を超えます。 $\geq f$.*

1° $f'$ を $\mathscr{L}^\infty$ の写像とし、$\dot{f}'$ が類の集合の $L^\infty$ 写像の $\dot{\varphi}$ $\mathscr{K}(T)$ の $\varphi$ の最高値となるようにします。 $0 \leq \varphi \leq f$;明らかに$\dot{f}' \leq \dot{f}$。 $U$ を $T$ の比較的コンパクトなオープン部分集合とします。 $\mathscr{K}(T)$ のすべての写像 $h$ について、$0 \leq h \leq f \varphi_U$ は、定義までに局所的にほぼどこでも $h(t) \leq f'(t)$ になるため、ほぼどこでも $h(t) \leq f'(t) \varphi_U(t)$ になります。その結果、$\int h \, d\mu \leq \int f' \varphi_U \, d\mu$ となります。 ただし、$f \varphi_U$ は下位の半連続である $\int f \varphi_U \, d\mu = \sup \int h \, d\mu$ であるため、$h$ は $\mathscr{K}(T)$ の写像の集合を超え、$0 \leq h \leq f \varphi_U$ となります (Ch. IV, §1, No. 1、デフォルト。 1);したがって

$$
\int f \varphi_U \, d\mu \leq \int f' \varphi_U \, d\mu,
$$

そして $f' \varphi_U \leq f \varphi_U$ からほぼどこでも、必然的に $f \varphi_U = f' \varphi_U$ ほぼどこでも、よって $f = f'$ はローカルでほぼどこでもです。

2° $f'$ を $\mathscr{L}^\infty$ の写像とし、$\dot{f}'$ が、有界で下側の半連続写像 $\psi$ の類 $\dot{\psi}$ の集合の $L^\infty$ の下限となるようにします。 $\geq f$;それから$\dot{f}' \geq \dot{f}$。 $K$ を $T$ の圧縮部分集合とします。有界および $\geq f \varphi_K$ の下の半連続写像 $h$ ごとに、$\overline{h}$ を $K$ では $h$ に、$T - K$ では $\|f\| + \|h\|$ に等しい写像とします。次に、$\overline{h}$ は半連続で低く、$\geq f$ であるため、ほぼどこでも局所的には定義 $\overline{h}(t) \geq f'(t)$ になります。したがって、ほぼどこでも $h(t) \geq f'(t)\varphi_K(t)$、よって $\int h d\mu \geq \int f'\varphi_K d\mu$ になります。しかし、$\int f\varphi_K d\mu = \inf \int h d\mu$では、$h$が、境界のある下半連続写像の集合と$\geq f\varphi_K$を越えます（Ch.IV, §1, No. 3、定義3）。したがって

$$
\int f\varphi_K d\mu \geq \int f'\varphi_K d\mu,
$$

そして、ほぼどこでも $f\varphi_K \leq f'\varphi_K$ 以降、ほぼどこでも必然的に $f\varphi_K = f'\varphi_K$ になり、ほぼどこでもよって $f = f'$ になります。

補題が証明されたので、提案 14 の主張で $\mathscr{L}^\infty$ 満たす条件に対して $\theta$ を正の線型形式とします。 The restriction of $\theta$ to the space $\mathscr{K}(T)$ is a positive measure $\nu$ on $T$. 正の写像 $f \in \mathscr{L}^\infty(T, \mu)$ ごとに、$\theta(f) = \nu^*(f)$ があることを示します。 まず、$f$ が下位半連続 (かつ有界) であると仮定します。 補題 4 により、$f$ は類 $\dot{\varphi}$ の増加する有向集合の上限であり、$\varphi$ は $\mathscr{K}(T)$ で写像の有向集合 $\Phi$ を超えます。 $0 \leq \varphi \leq f$。 仮定 $\theta(f) = \sup_{\varphi \in \Phi} \theta(\varphi)$ と $\nu^*(f) = \sup_{\varphi \in \Phi} \nu(\varphi)$ 定義により、この場合、主張が証明されます。 次に、$f$ が $\mu$ 測定可能であり、有界であると仮定します。次に、定義、$\nu^*(f) = \inf_{\psi \in \Psi} \nu^*(\psi)$までに、$\psi$が、有界の下半連続写像の減少する有向集合$\Psi$と$\geq f$を越えます。 If $a \geq \|f\|$ then, applying the hypothesis of the statement to the increasing directed set of classes of the functions $a - \psi$, where $\psi \in \Psi$ and $\psi \leq a$, one sees, by virtue of the lemma, that $\theta(f) = \inf_{\psi \in \Psi} \theta(\psi)$, therefore indeed $\theta(f) = \nu^*(f)$. 特に、すべての $\mu$ 無視できる写像 $f \geq 0$ について、$\theta(f) = 0$ があり、従って $\nu^*(f) = 0$ となり、その結果 (No. 5, Th. 2) $\nu$ は * 基底* $\mu$ を伴う尺度になります。さらに、$\nu^*(1) = \theta(1) < +\infty$ は、結果として (Th. 1 の Cor.) $\nu = g \cdot \mu$ と $g \in \mathscr{L}^1(T, \mu)$ です。 最後に、すべての$\mu$可測写像は$\nu$可測であるため、すべての正の写像$f \in \mathscr{L}^\infty(T, \mu)$は$\nu$可積分および$\int fg d\mu = \nu^*(f) = \theta(f)$で、証明が完成します。

提案 14 の 1 つの結論するは、型 $f \mapsto \int fg d\mu$ の $\mathscr{L}^\infty$ 上の線型形式が、$g \in \mathscr{L}^1$ の差分 $\theta_1 - \theta_2$ であり、$\theta_1$ と $\theta_2$ は正である線型形式満たす提案14の条件。

### 9. アプリケーション: II。 写像の対策

$\mu_1, \mu_2, \ldots, \mu_n$ を T 上の実測度、$u(x_1, \ldots, x_n)$ を有限数値写像とし、$\mathbf{R}^n$ で定義され、正に同次である、つまり (Ch. I, §1, No. 1) とします。

$$
u(\alpha x_1, \ldots, \alpha x_n) = \alpha u(x_1, \ldots, x_n)
$$

すべてのスカラー $\alpha \geqslant 0$ に対して。 T には、$1 \leqslant i \leqslant n$ に対して $|\mu_i| \leqslant \lambda$ となるような肯定的な尺度 $\lambda$ が存在します (たとえば、和 $\sum_{i=1}^n |\mu_i|$)。 $\lambda$ と $\lambda'$ を T 上の 2 つのそのような尺度とします。 $\mu_i = f_i \cdot \lambda = f'_i \cdot \lambda'$ と書くことができます。ここで、$f_i$ (それぞれ $f'_i$) は測定可能であり、基本的に尺度 $\lambda$ (それぞれ $\lambda'$) (No. 5、Th. 2) に制限されます。次の結果を確立します: *位数では、数値写像 $u(f_1, \ldots, f_n)$ が $\lambda$ に対して局所的に可積分であること、写像 $u(f'_1, \ldots, f'_n)$ が $\lambda'$ に対して局所的に可積分であることが必要十分であり、その場合*

$$
u(f_1, \ldots, f_n) \cdot \lambda = u(f'_1, \ldots, f'_n) \cdot \lambda'.
$$

$|\mu_i| \leqslant \inf(\lambda, \lambda')$ 以降、$\lambda \leqslant \lambda'$ の場合に限定できます。次に、$\lambda = g \cdot \lambda'$、ここで、$g$ は、$0 \leqslant g \leqslant 1$ (No. 5、Th. 2) のように、$\lambda'$ で測定可能な写像です。 よって (No. 4、提案 8)

$$
\mu_i = f_i \cdot (g \cdot \lambda') = (f_i g) \cdot \lambda';
$$

(No. 3、提案 3 の Cor. 2) $f_i g$ は、局所的にほぼどこでも $\lambda'$ に対して $f'_i$ に等しいことがわかります。従って、(12) より、

$$
u(f'_1, \ldots, f'_n) = u(f_1 g, \ldots, f_n g) = u(f_1, \ldots, f_n) g
$$

$\lambda'$ は地元のほぼどこでも。 位数では、$u(f'_1, \ldots, f'_n)$ が局所的に $\lambda'$ 可積分であるため、$u(f_1, \ldots, f_n) g$ が $\lambda'$ に対して局所的に可積分であることが必要かつ十分であり、従って (No. 4、提案 8) $u(f_1, \ldots, f_n)$ が $\lambda$ に対して局所的に可積分であることが必要かつ十分です。そして (No. 4、提案 8)

$$
u(f'_1, \ldots, f'_n) \cdot \lambda' = (u(f_1, \ldots, f_n) g) \cdot \lambda' = u(f_1, \ldots, f_n) \cdot \lambda.
$$

従って、尺度 $u(f_1, \ldots, f_n) \cdot \lambda$ は尺度 $\mu_1, \ldots, \mu_n$ と写像 $u$ にのみ依存します。 $u(\mu_1, \ldots, \mu_n)$ とも表されます。従って、この測度は、$u$ が正の同次値写像である場合に常に定義されます。そのため、すべての $|\mu_i|$ に対して上界である正の測度 $\lambda$ について、$u(f_1, \ldots, f_n)$ は局所的に $\lambda$ 積分可能です。ここで、$f_i$ は、 $\lambda$ に対する $\mu_i$ の稠密度 。この条件は、 $u$ が確実に均一かつ *連続* である場合に満たされることに注意してください。
$$
|u(x_1, \ldots, x_n)| \leq a(|x_1| + |x_2| + \cdots + |x_n|)
$$
(*u* は $(0, \ldots, 0)$ の十分に小さい近傍で境界付けられています))、そして、$u(f_1, \ldots, f_n)$ は $\lambda$ 可測であるため (Ch. IV, §5, No. 3、Th. 1)、積分可能性の基準によって局所的に $\lambda$ 積分可能です (Ch. IV, §5, No. 6、Th. 1)。 5)。

$u_1, \ldots, u_p$ を、$p$ 写像 $g_k = u_k(f_1, \ldots, f_n)$ $(1 \leq k \leq p)$ が局所的に $\lambda$ 可積分であるように、$\mathbf{R}^n$ で定義された正の同次数値写像とする。 $v$ を、$v(g_1, \ldots, g_p)$ が局所的に $\lambda$ 可積分となるように、$\mathbf{R}^p$ で定義された正に同次な数値写像とします。 集合
$$
w(x_1, \ldots, x_n) = v(u_1(x_1, \ldots, x_n), \ldots, u_p(x_1, \ldots, x_n)).
$$
このとき、写像 $w$ は正同次であり、$w(f_1, \ldots, f_n)$ は局所的に $\lambda$ 可積分であり、定義により、
$$
w(\mu_1, \ldots, \mu_n) = v(u_1(\mu_1, \ldots, \mu_n), \ldots, u_p(\mu_1, \ldots, \mu_n)).
$$

写像 $x^+, x^-, |x|, x+y, \inf(x, y), \sup(x, y)$ の特殊なケースでは、先ほど説明した手順によって定義された測定値一致するが、それぞれ $\mu^+, \mu^-, |\mu|, \mu+\nu, \inf(\mu, \nu), \sup(\mu, \nu)$ で示されます。これはコルからすぐに続きます。 No. 2の提案2の。 $\mu$ と $\nu$ が 2 つの実際のメジャーである場合、$\theta = \mu + i\nu$ の場合、$|\theta| = \sqrt{\mu^2 + \nu^2}$ になります。 $\lambda$ を、$|\mu|$ と $|\nu|$ の上界である測度 $\geq 0$ とし、$f, g$ を、$\mu = f \cdot \lambda,\ \nu = g \cdot \lambda$ のような局所的な $\lambda$ 可積分関数とします。それから
$$
\sqrt{\mu^2 + \nu^2} = \sqrt{f^2 + g^2} \cdot \lambda,
$$
$$
\theta = (f + ig) \cdot \lambda,\ \text{therefore (No. 2, Prop. 2)}\ |\theta| = \sqrt{f^2 + g^2} \cdot \lambda.
$$
この方法は、$\mathbf{R}^n$ の曲線の正に均一な写像 $(x_1^2 + \ldots + x_n^2)^{1/2}$ から定義する長さに適用できます。

### 10. 対策を拡散する。核対策

#### 定義 5 {#int-v-s5-def-5 .statement tag=093Q}

T の *メジャー $\theta$ は、* $|\theta|(\{t\}) = 0$ *すべて* $t \in T$ の場合に拡散していると言われます。

#### 例 {#int-v-s5-n10-exa-1 .statement tag=093R}

— $\mathbf{R}$ のルベーグ測度は拡散しています (Ch. IV, §1, No. 3、*注意* 1)。

$\theta$ が $T$ の拡散測度であると言うのは、有限補数を持つすべての集合が $|\theta|$ を運ぶ、または再び $|\theta|$ がすべての点測度に対して異質であるというというに相当します。したがって、拡散は $\mathscr{M}(T)$ (Ch. II, §1, No. 5、Th. 1) のバンド形を測定します。

(Ch. III, §1, No. 3) を思い出してください。$T$ 上の複素測度 $\rho$ が形 $\sum_{t \in T} \alpha(t) \varepsilon_t$ の場合、*原子* であると言われます。ここで、$\alpha$ は、すべてのコンパクトに対して $\sum_{t \in K} |\alpha(t)| < +\infty$ となるような $T$ 上の複素数写像です。 $T$ の部分集合 $K$ は、ファミリー $(\alpha(t) \varepsilon_t)_{t \in T}$ が合計可能であることを表します (§2, No. 1, 注意 2)。コルに続いて注意から続きます。 Thの3。 $|\rho| = \sum_{t \in T} |\alpha(t)| \varepsilon_t$のNo. 5の2。この公式中に出現する写像$\alpha$は$\alpha(t) = \rho(\{t\})$なので一意に決まります。原子測定と拡散測定は互いに異質です。

#### 命題 15 {#int-v-s5-prop-15 .statement tag=093S}

*$T$ 上のすべての複雑なメジャー $\sigma$ は、形 $\rho + \theta$ で唯一の 1 つの方法で記述できます。ここで、$\rho$ は原子メジャー、$\theta$ は拡散メジャーです。その場合、1 つは $|\sigma| = |\rho| + |\theta|$.* になります。

分解の一意性は明らかです。$\rho$ は原子であり、$\theta$ は拡散しているため、必然的に $\rho = \sum_{t \in T} \rho(\{t\}) \varepsilon_t = \sum_{t \in T} \sigma(\{t\}) \varepsilon_t$ と $\theta = \sigma - \rho$ になります。存在を確立するには、すべてのコンパクト集合 $K$ に対して $\sum_{t \in K} |\sigma(\{t\})| \leq |\sigma|(K) < +\infty$ を観察するだけで十分です。つまり、集合 $\sum_{t \in T} \sigma(\{t\}) \varepsilon_t = \rho$ が可能です。 $\sigma - \rho$ の尺度は明らかに拡散しており、関係 $|\sigma| = |\rho| + |\sigma - \rho|$ がコルからすぐに続きます。 No. 7の提案13の3。

この証明は、$\sigma$ が集合 $M$ によって運ばれ、$t \in M$ ごとに $|\sigma|(\{t\}) > 0$ がある場合、$\sigma$ は *原子* であることを示していることがわかります。

### 練習問題 {#int-v-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
