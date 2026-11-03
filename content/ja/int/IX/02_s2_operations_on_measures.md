---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 2
section_title: Operations on measures
lang: ja
source: int-vii-ix
book_pages: INT IX.22-INT IX.41, INT IX.108
pdf_pages: 0204-0223, 0290-0290
extraction: ocr
subsections:
    - "no": 1
      title: Induced measure on a measurable subspace
      page: 22
      pdf_page: 204
    - "no": 2
      title: Measures defined by numerical densities
      page: 24
      pdf_page: 206
    - "no": 3
      title: Image of a measure
      page: 26
      pdf_page: 208
    - "no": 4
      title: Lifting of measures
      page: 29
      pdf_page: 211
    - "no": 5
      title: Product of two measures
      page: 31
      pdf_page: 213
    - "no": 6
      title: Integration with respect to the product of two measures
      page: 33
      pdf_page: 215
    - "no": 7
      title: A result on the disintegration of measures
      page: 37
      pdf_page: 219
statements: 41
exercises: 3
content_sha256: 00d4b2d7d29d9ee421c823f3abf9ca7ec91cd99b6ae84eaa0013901d5c45fbba
translated_from: content/en/int/IX/02_s2_operations_on_measures.md
translation_method: google
source_content_sha256: d7699f39ec1644b116484ef30c5ca9df84de13c33a79612bcf054973c062c5c9
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: c8a3bc4e1389a3e97315fe7bdd7cf37be56201f669241c0671dee90202ca800f
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。 演算対策について

前述の切断と同様に、$T$ はハウスドルフ トポロジカル空間を表し、$\mu$ は $T$ のメジャーを表します。すべての措置は肯定的なものと想定されており、反対の言及がないことを思い出してください。

### 1. 測定可能なものに対する誘導測定部分空間

$X$を$T$の部分集合とし、$\nu$を写像の$\mu : K \mapsto \mu_K$から集合の$X$のコンパクト部分集合の制限とする。 $\nu$が$X$に対する事前対策であることは明らかです。一方、$x \in X$ と $V$ を、$\mu^\bullet(V) < +\infty$ となるような $T$ の $x$ の開いた近傍とする。それから

$$
\nu^\bullet(X \cap V) = \sup_{\substack{K \text{ compact} \\ K \subset X \cap V}} \mu^\bullet(K) \leq \mu^\bullet(V) < +\infty
$$

§1, No. 2 の *注意 3* によって、$\nu$ がメジャーになります。

$X$ が $\mu$ で測定可能でない場合、負担 $\nu^\bullet$ と $(\mu^\bullet)_X$ は必ずしも等しいとは限らず、測定値 $\nu$ には利子がありません。

#### 定義 1 {#int-ix-s2-def-1 .statement tag=09OF}

*$X$を$T$の$\mu$で測定可能な部分集合とします。 $\mu : K \mapsto \mu_K$の制限から$X$のコンパクト部分集合の集合は、部分空間$X$の$\mu$によって引き起こされる措置と呼ばれ、$\mu_X$または$\mu|X$で表されます*。

#### 命題 1 {#int-ix-s2-prop-1 .statement tag=09OG}

*$X$を$T$の$\mu$可測部分集合とする。負担 $(\mu_X)^\bullet$ は、$X$ (§1, No. 1) で $\mu^\bullet$ によって引き起こされる負担 $(\mu^\bullet)_X$ に等しくなります。他の場合は、写像 $g \in \mathscr{F}_+(X)$ ごとに語、$(\mu_X)^\bullet(g) = \mu^\bullet(g^0)$ です。

$f \in \mathscr{F}_+(X)$と$f^0$を$f$から$T$の0により拡大とします。 1 つは $(\mu^\bullet)_X(f) = \mu^\bullet(f^0) = \sup_L \mu^\bullet(f^0 \varphi_L)$ で、$L$ は $T$ のコンパクト部分集合の集合を超えます (§1, No. 2、提案 2)。同様に$(\mu_X)^\bullet(f) = \sup_K \mu_K^\bullet(f_K) = \sup_K \mu^\bullet(f^0 \varphi_K)$、ここで$K$は$X$のコンパクトな部分集合の集合を超えます。したがって、結局のところ、すべてのコンパクト部分集合 $L$ の $T$ について $\mu^\bullet(f^0 \varphi_L) = \sup_K \mu^\bullet(f^0 \varphi_K)$ が示され、ここで $K$ は $L \cap X$ のコンパクト部分集合の集合を超えます。ここで、$(K_n)$ を、$L \cap X$ に含まれるコンパクトな集合の増加する数列とし、$(L \cap X) - \bigcup_n K_n$ が局所的に$\mu$ 無視できるようにします (§1, No. 8、提案 11)。 $f^0$ は $X$ の外側に零あり、$f^0 \varphi_L$ は $L \cap X$ の外側に零であるため、数列 $(f^0 \varphi_{K_n})$ の上部エンベロープとほぼどこでも局所的に等しくなります。これは、$\mu^\bullet(f^0 \varphi_L) = \sup_n \mu^\bullet(f^0 \varphi_{K_n})$、よってが望ましい結果であることを意味します。*

#### 注意 1 {#int-ix-s2-n1-rem-1 .statement tag=09OH}

関係 $(\mu_X)^\bullet = (\mu^\bullet)_X$ では、記法 $\mu_X^\bullet$ を曖昧さなく使用できます。今後もそうします。 §1, No. 2 の前述の提案 1 と提案 2 は、$K$ コンパクトに関してこれまで$\mu_K$ で示されていた措置が、確かに定義の意味で誘導された措置であることを示しています。 1. 同様に、$T$ が局所的にコンパクトで、$X$ が $T$ の局所的にコンパクトな部分空間である場合、上記の提案 1 と第 3 章の提案 1 は成り立ちます。 V, §7, No. 1 は、Def. 1 一致すると Ch. の定義 IV, §5, No. 7。

#### 注意 2 {#int-ix-s2-n1-rem-2 .statement tag=09OI}

デフ。 1 は、$\mu$ が $T$ の複素測度である場合に拡張できます。この場合、事前メジャー $\mu_X$ がメジャーであることを示すには、$X$ (§1, No. 2) のすべてのコンパクト部分集合 $K$ に対して $|\mu_K| = |\mu|_K$ を観察するだけで十分です。

提案 1 によれば、$X$ の部分集合 $Y$ は、$\mu$ 測定可能 (局所的に $\mu$ 無視できる) である場合に限り、$\mu_X$ 測定可能 (局所的に $\mu_X$ 無視可能) になります。 $Y$ が $\mu_X$ 測定可能、したがって $\mu$ 測定可能である場合、誘導測度 $(\mu_X)_Y$ と $\mu_Y$ は、提案 1 (* 誘導測度の推移性 *) により明らかに等しい。

注意 3）。 — X を T の $\mu$ 測定可能な部分集合とします。 $g = \varphi_X$ に適用される§1, No. 8 の提案 10 により、$\alpha \in A$ ごとに $K_\alpha \subset X$ または $K_\alpha \subset \mathbf{C}X$ のいずれかになるような T の破砕 $(K_\alpha)_{\alpha \in A}$ が存在します。 §1, No. 8 の Scholium の手順で T の位相を修正すると、$T'$ によって誘導された位相を X に装備することで得られる空間 $X'$ は局所的にコンパクトであり、$\mu$ (それぞれ$\mu_X$) $\mu$ (それぞれ $\mu_X$) と同じ本質的な上積分を認める、$T'$ (それぞれ $X'$) 上の測度 $\mu'$ (それぞれ $\nu$): これは、$\mu'_{X'} = \nu$ を意味します。局所的に無視できる集合、測定可能な写像、およびバナッハ空間の値を伴う本質的な可積分関数は、$\mu$ と $\mu'$、および $\mu_X$ と $(\mu_X)' = \nu = \mu'_{X'}$ で同じであるため、 理論簡約する章で扱われたものに対する誘導措置に関する統合の理論ローカルコンパクト空間の特別なケースの V, §7。結果を転記する作業は読者に任せます。

### 2. 数値密度によって定義される尺度

#### 定義 2 {#int-ix-s2-def-2 .statement tag=09OJ}

* T 上で定義された写像 f は、$\overline{\mathbf{R}}$ またはバナッハ空間の値を使用して、f が $\mu$ 可測で、すべての点 $x \in T$ が次のような近傍 V を認める場合、局所的に $\mu$ 積分可能であると言われます。 $\mu^\bullet(|f|\varphi_V) < +\infty$.*

この定義一致するは、第 3 章で与えられたものと一致します。 V, §5, No. 1、T が局所的にコンパクトな場合。

$f$ を局所的に $\mu$ 積分可能な正の写像とします。 写像 $K \mapsto f_K \cdot \mu_K$ は事前措置 (第 1 章 V, §7, No. 1、コリント 2) であり、$f \cdot \mu$ で示されます。

#### 命題 2 {#int-ix-s2-prop-2 .statement tag=09OK}

*f が正の局所的 $\mu$ 積分可能な関数の場合、すべての写像 $g \in \mathscr{F}_+(T)$ に対して、関係* が得られます。

$$
(f \cdot \mu)^\bullet(g) = \mu^\bullet(fg).
$$

実際、T のすべてのコンパクト集合 K について、

$$
(f \cdot \mu)_K^\bullet(g_K) = (f_K \cdot \mu_K)^\bullet(g_K) = \mu_K^\bullet(f_K g_K) = \mu_K^\bullet((fg)_K),
$$

$f \cdot \mu$ の定義と第 3 章の提案 3 の使用についてV, §5, No. 3。提案 2 は、これから移行で K の最高値に続きます。

ここで、$x \in T$ と V を、$\mu^\bullet(f \varphi_V) < +\infty$ となるような x の近傍とします (定義 2)。その場合、$(f \cdot \mu)^\bullet(V) = \mu^\bullet(f \varphi_V) < +\infty$、したがって、$f \cdot \mu$ がメジャーになります。

#### 定義 3 {#int-ix-s2-def-3 .statement tag=09OL}

* f を局所的に $\mu$ 積分可能な正の写像とする。 $f \cdot \mu : K \mapsto f_K \cdot \mu_K$ の測度は、$\mu$ に対する稠密度 f の測度*、または $\mu$ の写像 $f$ の積の測度と呼ばれます。 形 $f \cdot \mu$ のすべての測度 ($f$ は正で局所的に $\mu$ 積分可能) は、基底 $\mu$ の測度と呼ばれます。

#### 注意 1 {#int-ix-s2-n2-rem-1 .statement tag=09OM}

$f \cdot \mu$ 拡大するの定義を、$f$ が局所的に複合体可積分関数である場合に変換します。次に $|f \cdot \mu| = |f| \cdot \mu$ があり、これは $f \cdot \mu$ が単なる事前測定ではなく測定であることをすぐに暗示します。このように定義された複雑なメジャーを指定するために、「基底 $\mu$ でメジャー」という表現を保持します。

#### 注意 2 {#int-ix-s2-n2-rem-2 .statement tag=09ON}

Similarly, if $\theta$ is a complex measure, $f$ is said to be locally $\theta$-integrable if it is locally $|\theta|$-integrable, and one defines the measure $f \cdot \theta : K \mapsto f_K \cdot \theta_K$. 1 つは $|f \cdot \theta| = |f| \cdot |\theta|$ (Ch. V, §5, No. 2、提案 2)。 この No. では、非積極的な対策に関するすべてのことは脇に置きます。

#### 命題 3 {#int-ix-s2-prop-3 .statement tag=09OO}

— $\nu$ を T 上の測度とします。 $\nu$ が形 $f \cdot \mu$ であるためには、$f$ は局所的に $\mu$ 可積分の正の写像であり、すべての $\mu$ 無視できるコンパクト集合が以下であることが必要かつ十分です。 $\nu$-無視できるほど。 $f'$ が、$\nu = f' \cdot \mu$ のようなローカルで 2 番目の $\mu$ 積分可能な関数である場合、$f = f'$ はローカルで $\mu$ - ほぼどこでも可能です。

条件は明らかに必要です (提案 2)。逆に、すべての $\mu$-無視できるコンパクト集合が $\nu$-無視できると仮定します。 $\mu + \nu$ の対策に T の粉砕 $(K_\alpha)_{\alpha \in A}$ を導入して、集合 $N = T - \bigcup_{\alpha \in A} K_\alpha$ にしましょう。 $(K_\alpha)_{\alpha \in A}$ が $\mu$ と $\nu$ にとって破砕であることは明らかであり、したがって、§1, No. 8 の提案 9 は、すべての $g \in \mathscr{F}_+$ に対して次の関係を意味します。

$$
\mu^\bullet(g) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet(g_{K_\alpha}), \quad \nu^\bullet(g) = \sum_{\alpha \in A} \nu_{K_\alpha}^\bullet(g_{K_\alpha}).
$$

$\mu_{K_\alpha}$ が無視できるコンパクトな集合 $C \subset K_\alpha$ を考えてみましょう。次に、$C$ は局所的には $\mu$ で無視でき、したがって局所的には $\nu$ は無視でき、最後に $\nu$ の定義によって $\nu_{K_\alpha}$ は無視できます。 その後、ルベーグ – ニコディム定理 (Ch. V, §5, No. 5、木。 2) $\nu_{K_\alpha}$ は、$\mu_{K_\alpha}$ に関して稠密度 $f_\alpha$ を認めます。 $f$ を写像と一致するとし、集合 $K_\alpha$ のそれぞれに $f_\alpha$ を、$N$ に 0 を付けます。 写像 $f$ は $\mu$ で測定可能です (Ch. IV, §5, No. 10、提案 16)、およびすべての写像 $g \in \mathscr{F}_+$ について、上記の関係と第 3 章の提案 3 により、 V, §5, No. 3、

$$
\nu^\bullet(g) = \sum_{\alpha \in A} \nu_{K_\alpha}^\bullet(g_{K_\alpha}) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet(f_\alpha g_{K_\alpha}) = \sum_{\alpha \in A} \mu_{K_\alpha}^\bullet((f g)_{K_\alpha}) = \mu^\bullet(f g).
$$

次に、まず、$f$ が局所的に $\mu$ 可積分であることがわかります。$x$ が T の点であり、$V$ が $\nu^\bullet(V) < +\infty$ となるような $x$ の近傍である場合、$\mu^\bullet(f \varphi_V) < +\infty$ です。次に、提案 2 は、$\nu$ と $f \cdot \mu$ の本質的な上積分が同じであることを示しています。したがって、それらは等しい（§1, No. 2、提案 2 の Cor.）。コンパクトな空間の場合から$f$の一意性は自明であり、命題が成立します。

注意 3)。 — $\nu = f \cdot \mu$ 簡約するを理論まで一度に統合する理論 V。 なぜなら、$(K_\alpha)_{\alpha \in A}$ を $\mu$ 、したがって $\nu$ の T の粉砕であるとし、$T'$ を §1, No. 8 の Scholium で定義された局所的にコンパクトな空間であるとします。 $T'$ 上の測度 $\mu'$ (それぞれ $\nu'$) を $\mu$ (それぞれ $\nu$) に関連付けることができます。これは、可測関数、バナッハ空間の値を持つ本質的に可積分関数、および正の関数の本質的な上積分が $\mu$ および$\mu'$ ($\nu$ と $\nu'$ に対応)。 したがって、写像 $f$ は $\mu'$ 測定可能です。 $T'$ は局所的にコンパクトであり、$T'$ のコンパクト部分集合はコンパクト集合 $K_\alpha$ ($\alpha \in A$) の有限数とのみ交差するため、局所的に $\mu'$ 積分可能です。 最後に、関係 ${\nu'}^\bullet(g) = \nu^\bullet(g) = \mu^\bullet(fg) = {\mu'}^\bullet(fg)$ は $\nu' = f \cdot \mu'$ を証明します (Ch. V, §5, No. 3、提案 3)。 第 3 章の結果を転記する作業は読者に任せます。 V, §5。

### 3. 小節の像

#### 定義 4 {#int-ix-s2-def-4 .statement tag=09OP}

$\pi$ を T の写像としてトポロジカル空間 X にします。 $\pi$ が $\mu$ 可測であり、X のすべての点 x が $\mu^\bullet(\overline{\pi}(V)) < +\infty$ となるような近傍 V を認める場合、$\pi$ は $\mu$ 適切であると言われます。

#### 注意 1 {#int-ix-s2-n3-rem-1 .statement tag=09OQ}

T と X が局所的にコンパクトな場合、この定義は Ch のそれと等価です。 V, §6, No. 1。

#### 注意 2 {#int-ix-s2-n3-rem-2 .statement tag=09OR}

T から X への適切な連続写像 (GT、I, §10, No. 1、定義 1) は、すべての小節 $\mu$ に対して $\mu$-適切です。というのは、$x \in X$ としましょう。 $\overline{\pi}(x)$ はコンパクトなので (loc. cit.、No. 2、Th. 1)、集合 $\overline{\pi}(x)$ には $\mu^\bullet(H) < +\infty$ のようなオープン近傍 H があります。 集合 $V = X - \pi(T - H)$; $\pi$ が閉じているため、X、含む x ではV が開き、$\overline{\pi}(V) \subset H$、よって $\mu^\bullet(\overline{\pi}(V)) \leq \mu^\bullet(H) < +\infty$ が満たされます。

#### 注意 3 {#int-ix-s2-n3-rem-3 .statement tag=09OS}

$\mu$ が有界である場合、X への T のすべての $\mu$ 可測写像は $\mu$ 固有です。

#### 注意 4 {#int-ix-s2-n3-rem-4 .statement tag=09OT}

$\theta$ が T 上の複素測度である場合、$\pi$ が正の測度 $|\theta|$ に対して適切であれば、$\pi$ は $\theta$-適切であると言われます。

#### 命題 4 {#int-ix-s2-prop-4 .statement tag=09OU}

$\pi$ を、トポロジー 空間 X への T の $\mu$ 固有写像とします。 X には、$\nu^\bullet$ が像負担$\pi(\mu^\bullet)$ (§1, No. 1) に等しいような唯一のメジャー $\nu$ が存在し、他の語には、すべての $g \in \mathscr{F}_+(X)$ に対して $\nu^\bullet(g) = \mu^\bullet(g \circ \pi)$ が存在します。

一意性は明らかです (§1, No. 2、提案 2 の修正)。存在を確立するために、まず、$\mu$ がコンパクト集合 K によって運ばれ、$\pi$ から K までの制限が連続である場合を扱います。そうすると、$L = \pi(K)$ はコンパクトになります。 $\pi'$ を $\pi$ によって誘導された L への K の連続写像とし、$\nu'$ を像 L での$\pi'(\mu_K)$ の測定、$\nu$ を $\nu'$ で定義された X での測定とします。 (§1, No. 3、例 2)。 $g \in \mathscr{F}_+(X)$ごとに、

$$
\nu^\bullet(g) = {\nu'}^\bullet(g_L) = \mu_K^\bullet(g_L \circ \pi') = \mu_K^\bullet((g \circ \pi)_K) = \mu^\bullet((g \circ \pi)_K^0) = \mu^\bullet(g \circ \pi)
$$

(§1, No. 3の公式(3)、V, §6, No. 2章の提案2、$\mu_K^\bullet$の定義、そして$\mu$がKによって運ばれるという事実を連続して使用しました。)他には語、$\nu^\bullet = \pi(\mu^\bullet)$。

ここで一般的なケースに移りましょう。プロップスによる。 §1, No. 8 の 10 と 9、$\mu$ は、$\pi$ の制限から $\mu_\alpha$ のサポート $K_\alpha$ までが $\alpha \in A$ ごとに連続するように、コンパクトなサポートを備えた合計可能な族 $(\mu_\alpha)_{\alpha \in A}$ の和です。上で処理した特別なケースでは、T の各小節 $\mu_\alpha$ に X の小節 $\nu_\alpha$ を $\nu_\alpha^\bullet = \pi(\mu_\alpha^\bullet)$ のように関連付けることができます。次に、$g \in \mathscr{F}_+(X)$ については、

$$
\sum_{\alpha \in A} \nu_\alpha^\bullet(g) = \sum_{\alpha \in A} \mu_\alpha^\bullet(g \circ \pi) = \mu^\bullet(g \circ \pi).
$$

$\pi$ は $\mu$-proper であるため、制約 $\pi(\mu^\bullet)$ はローカルに制限されます。したがって、族 $(\nu_\alpha)_{\alpha \in A}$ は合計可能であり (§1, No. 7、提案 7)、その和 $\nu$ は主張を満たします。

#### 定義 5 {#int-ix-s2-def-5 .statement tag=09OV}

*$\pi$ が位相幾何学的空間 X への T の $\mu$ 固有写像である場合、すべての $g \in \mathscr{F}_+(X)$ に対して $\nu^\bullet(g) = \mu^\bullet(g \circ \pi)$ となるような X 上の固有の測度 $\nu$ は、$\mu$ の像測度と呼ばれます。 $\pi$ では、$\pi(\mu)$.* と表示されます。

#### 例 {#int-ix-s2-n3-exa-1 .statement tag=09OW}

— K を T の圧縮部分空間、K の T への i 標準単射、および K の測定値 $\lambda$ とする。 i は連続であり、$\lambda$ は有界であるため、i は $\lambda$-proper です。 §1, No. 3の公式(3)は、「$\lambda$によって定義されるTに関するメジャー」が像メジャー$i(\lambda)$であることを示しています。

*注意 5).* — $\theta$ が実際の尺度で、$\pi$ が $\theta$ 適切である場合、$\theta^+$ および $\theta^-$ の尺度には $\pi$ が適切です。 1 つ、次に集合 $\pi(\theta) = \pi(\theta^+) - \pi(\theta^-)$。 $\theta$ が複素尺度で、$\pi$ が $\theta$ 適切である場合、実際の尺度 $\Re(\theta)$ と $\Im(\theta)$ には $\pi$ が適切です。 1 つ目集合

$$
\pi(\theta) = \pi(\Re(\theta)) + i \pi(\Im(\theta)).
$$

#### 命題 5 {#int-ix-s2-prop-5 .statement tag=09OX}

*$\pi$ をトポロジカル空間 X への T の $\mu$ 固有写像とし、f をトポロジカル空間 F への X の写像とする（ハウスドルフかどうか）。 f が $\pi(\mu)$ 可測であるためには、 $f \circ \pi$ が $\mu$ 可測であることが必要かつ十分です。*

提案 4 の証明を再度取り上げ、最初に扱った特別なケースから始めましょう。同じ記法です。 g は、$g_L$ が $\nu'$ 可測 (§1, No. 5, *例*) である場合に限り、$\pi(\mu) = \nu$ の測度に対して可測です。さて、これは、$g_L \circ \pi' = (g \circ \pi)_K$ が $\mu_K$ 測定可能であるというというに相当します (Ch. V, §6, No. 2、提案 3)、そして最後に、$g \circ \pi$ は $\mu$ 測定可能です (§1, No. 5、*例*)。 次に、提案 4 の証明と同じ記法を使用した一般的なケースに移りましょう。 f が $\nu$ 測定可能であるのは、 f がすべての $\alpha \in A$ について $\nu_\alpha$ 測定可能である場合に限り (§1, No. 7、提案 8)、したがって、 $f \circ \pi$ がすべての $\alpha \in A$ について $\mu_\alpha$ 測定可能である場合に限り (前述の特別な場合)、そして最後に、次の場合に限り、 $f \circ \pi$ は $\mu$ で測定可能です ($§ 1$、No. 7、提案 8)。

#### 系 {#int-ix-s2-n3-cor-1 .statement tag=09OY}

— *X と Y を 2 つのトポロジー 空間、$\pi$ を T の $\mu$-適切な写像から X に、$\pi'$ を X の $\pi(\mu)$-適切な写像を Y にするとします。 写像 $\pi'' = \pi' \circ \pi$ は $\mu$ が適切で、$\pi''(\mu) = \pi'(\pi(\mu))$ (「小節の像の推移性」) です。

なぜなら、$\pi''$ は$\mu$ 測定可能であるからです (提案 5)。 集合 $\mu' = \pi(\mu)$; 像負担 $\pi'({\mu'}^\bullet) = \pi'(\pi(\mu^\bullet))$ は明らかに $\pi''(\mu^\bullet)$ に等しいです。局所的に有界されているため、$\pi''$ は $\mu$-proper です。 $\pi''(\mu)$ と $\pi'(\mu')$ は同じ本質的な上積分を持ち、したがって等しいです。

#### 命題 6 {#int-ix-s2-prop-6 .statement tag=09OZ}

— *$\pi$ を、トポロジカル空間 X への T の $\mu$ 固有写像とし、B を X の $\pi(\mu)$ 可測部分集合とする。 集合 $A = \overline{\pi^{-1}(B)}$、そして A の $\pi'$ 写像によって B に、A に $\pi$ を持つ一致するが表されます。集合 A は $\mu$ 可測であり、$\pi_A$ と $\pi'$ は$\mu_A$-適切、および*

$$
(\pi(\mu))_B = (\pi_A(\mu_A))_B = \pi'(\mu_A).
$$

集合 A は、$\varphi_B$ に適用される提案 5 によって $\mu$ で測定可能です。 写像 $\pi_A$ は明らかに $\mu_A$ が誘導措置 (No. 1) の定義によって測定可能であり、その結果、$\pi'$ が測定可能であることがわかります。 $f$ を $\mathscr{F}_+(B)$ の元とします。 零指数拡大を X の 0 で表し、T では次のようになります。

$$
(\pi(\mu)_B)^\bullet(f) = \pi(\mu)^\bullet(f^0) = \mu^\bullet(f^0 \circ \pi) = \mu^\bullet((f \circ \pi')^0) = \mu_A^\bullet(f \circ \pi'),
$$

よって $(\pi(\mu)_B)^\bullet = \pi'(\mu_A^\bullet)$。制約 $(\pi(\mu)_B)^\bullet$ は局所的に有界されているため、同じことが $\pi'(\mu_A^\bullet)$ にも当てはまり、したがって $\pi'$ は $\mu_A$-proper になります。メジャー $\pi'(\mu_A)$ と $(\pi(\mu))_B$ は同じ本質的な上積分を持っているため、等しいです。他の関係も同様の方法で確立できます。

#### 命題 7 {#int-ix-s2-prop-7 .statement tag=09P0}

— *T をトポロジー 空間 X の部分空間とし、i を T の X への単射とする。

a) *$\mu$ が T 上のメジャーであり、i が $\mu$-proper である場合、$i(\mu)$ のメジャーは T に集中し、1 つは $(i(\mu))_T = \mu$ になります。

b) *$\lambda$ が X 上の測度であり、T が $\lambda$ 測定可能である場合、i は $\lambda_T$ 適切であり、$i(\lambda_T) = \varphi_T \cdot \lambda$ です。

a) 集合 $\nu = i(\mu)$; 関係 $\nu^\bullet(A) = \mu^\bullet(A \cap T)$ を $A = X - T$ に適用すると、$\nu$ が T に集中していることがわかります。 関係 $\nu_T = \mu$ は、$B = T = A$ を取る場合の関係 (2) の特殊なケースです。

b) $f$ を、X で定義された正の写像とします。 設定 $\mu = \lambda_T$、1 つは $\mu^\bullet(f \circ i) = \lambda_T^\bullet(f_T) = \lambda^\bullet(f \varphi_T) \leq \lambda^\bullet(f)$ です (提案 1)。つまり、私は$\mu$-正しいということになります。一方、$\mu^\bullet(f \circ i)$ (それぞれ $\lambda^\bullet(f \varphi_T)$) は、$i(\mu)$ (それぞれ $\varphi_T \cdot \lambda$) に対する $f$ の本質的な上積分です。したがって、これら 2 つの尺度は等しいです。

*注意 6).* — $\pi$ を、トポロジー 空間 $X$ への $T$ の $\mu$ 固有写像とします。 1 つの簡約する理論は、第 3 章で扱った像測定$\nu = \pi(\mu)$ から理論に関する統合です。 V, §6、次の方法で。 $(K_\alpha)_{\alpha \in A}$ (それぞれ $(L_\beta)_{\beta \in B}$) を、$\mu$ (それぞれ $\nu$) および集合 $N = T - \bigcup_{\alpha \in A} K_\alpha,\ P = X - \bigcup_{\beta \in B} L_\beta$ に対する $T$ (それぞれ $X$) の粉砕であるとします。 $\pi$ から各 $K_\alpha$ までの制限は連続していると仮定できます (§1, No. 8、提案 10)。 $T', X'$ を、§1, No. 8 の Scholium と同様に構築された局所的にコンパクトな空間とし、$\mu'$ と $\nu'$ を、$\mu$ と $\nu$ に関連付けられたこれらの空間の尺度とします。 部分空間 $K_\alpha$ のトポロジーと $N$、$\pi$ の離散トポロジーの合計である $T'$ のトポロジーは、$T'$ から $X$ への連続マッピングであり、関係 ${\mu'}^\bullet(g \circ \pi) = \mu^\bullet(g \circ \pi) = \nu^\bullet(g)$ ($g \in \mathscr{F}_+(X)$ の) は、$\pi$ が$\mu'$-適切、そしてその$\pi(\mu') = \nu$。 一方、$X$ の $X'$ への恒等写像 $i$ は、$\nu$-proper であり、$i(\nu) = \nu'$ です。 したがって、$\pi$ は $T'$ から $X'$ への $\mu'$ 固有の写像であり、$\pi$ の下の $\mu'$ の像は $\nu'$ であるということになります（提案 5 の裏付け）。 第 3 章の結果を転記する作業は読者に任せます。 V, §6。

### 4. 措置の解除

#### 命題 8 {#int-ix-s2-prop-8 .statement tag=09P1}

*$T$と$X$を$T$から$X$への2つの位相空間、$\pi$写像とする。

a) $\nu$ を $X$ の有界メジャーとします。 位数では、$\pi$ が $\mu$ 適切であり、$\pi(\mu) = \nu$ であるような尺度 $\mu$ が$T$ に存在するということは、数 $\varepsilon > 0$ ごとに、次のようなコンパクトな集合 $K_\varepsilon \subset T$ が存在することで十分であり、 $\pi$～$K_\varepsilon$の制限は連続で$\nu^\bullet(X - \pi(K_\varepsilon)) < \varepsilon$です。

b) $\pi$ が単射だと仮定します。 $\mu$ と $\mu'$ を $T$ の 2 小節とし、$\mu$ と $\mu'$ には $\pi$ が適切で、$\pi(\mu) = \pi(\mu')$ には適切であるとします。次に$\mu = \mu'$。

*a)*に記載の条件は必須です。なぜなら、$\pi$ が $\mu$-proper かつ $\pi(\mu) = \nu$ である場合、関係 $\mu^\bullet(1) = \nu^\bullet(1) < +\infty$ は $\mu$ が有界であることを意味します。 写像 1 に適用される §1, No. 2 の提案 2 は、$\mu^\bullet(T - K) < \varepsilon/2$ のような $T$ のコンパクト部分集合 $K$ の存在を意味します。 $\pi$は$\mu$可測であるため、$\pi$から$K_\varepsilon$の制限が連続し、$\mu^\bullet(K - K_\varepsilon) < \varepsilon/2$となるようなコンパクトな集合$K_\varepsilon \subset K$が存在します。次に (No. 3、提案 4)

$$
\nu^\bullet(X - \pi(K_\varepsilon)) = \mu^\bullet(T - \overline{\pi}^{-1}(\pi(K_\varepsilon))) < \varepsilon.
$$

条件で十分であることを示すために、まず特殊なケースを扱います。

#### 補題 1 {#int-ix-s2-lem-1 .statement tag=09P2}

U と V を 2 つのコンパクトな空間とし、U を V に連続する写像とします。 $\mathscr{M}_+(U)$ の $\mathscr{M}_+(V)$ への写像 $\lambda \mapsto h(\lambda)$ は全射になります。

なぜなら、a を $\mathscr{C}(V)$ の $\mathscr{C}(U)$ に線形写像 $f \mapsto f \circ h$ とする。 h は全射なので、a は $\mathscr{C}(U)$ の部分空間 H に対する $\mathscr{C}(V)$ の等角投影です。 $\theta$ を V のポジティブな指標とします。この場合、$\theta \circ a^{-1}$ は H 上の連続した線型形式であり、ハーン・バナッハ定理 (TVS、II, §3, No. 2、Th. 1 の Cor. 3) によって、同じノルムを使用して $\mathscr{C}(U)$ の線型形式 $\eta$ まで拡張可能です。 $\eta$ は U に関するメジャーであり、すべての $f \in \mathscr{C}(V)$ に対して $\theta(f) = \eta(f \circ h)$ なので、$\theta = h(\eta)$ になります。最後に、$\theta(1) = \| \theta \| = \| \eta \|$ と $\theta(1) = \eta(1)$ により、$\eta$ が正になります (Ch. V, §5, No. 5、提案 9)。

ここで、a) で述べた条件の十分性を証明しましょう。 条件は、T のコンパクトな部分集合の数列 $(K_n)_{n \geq 1}$ の存在を暗示し、各 $K_n$ に対する $\pi$ の制限が連続し、すべての $n$、$\nu^\bullet(X - \pi(K_n)) < 1/n$ について同様です。 数列 $(K_n)$ は増加すると仮定できます。 集合 $L_n = \pi(K_n)$ は、$L_0 = \varnothing$ の規則に従って、$L_n$ のメジャー $\varphi_{L_n - L_{n-1}} \cdot \nu_{L_n}$ を $\nu'_n$ で示します。

制限 $\pi_{K_n}$ が連続である場合、$K_n$ には $\pi_{K_n}(\mu'_n) = \nu'_n$ (補題 1) となるメジャー $\mu'_n$ が存在します。 $K_n$の標準単射の下で$\mu_n$を$\mu'_n$の像とし、gを$\mathscr{F}_+(X)$の元とする。 $\nu$が$\bigcup L_n$に集中していることを引き続き利用して、§1, No. 5の提案4。 §1, No. 2の提案2; No. 3 の提案 4、そして最後に No. 3 の提案 7、

$$
\nu^\bullet(g) = \sum_n \nu^\bullet(\varphi_{L_n - L_{n-1}} g) = \sum_n \nu'_n \bullet (g_{L_n}) = \sum_n \mu'_n \bullet (g_{L_n} \circ \pi_{K_n})
$$
$$
= \sum_n \mu'_n \bullet ((g \circ \pi)_{K_n}) = \sum_n \mu_n^\bullet (g \circ \pi).
$$

この公式の $g = 1$ を考慮すると、族 $(\mu_n)$ が合計可能であり、その和が有界測度 $\mu$ であることがわかります (§1, No. 7、提案 7)。 No. 3 の提案 5 により、$\pi_{K_n}$ は連続であるため、$\mu'_n$ は測定可能であるため、写像 $\pi$ はすべての $n$ に対して $\mu_n$ 測定可能です。したがって、$\pi$ は$\mu$ 可測であり (§1, No. 7、提案 8)、したがって、$\mu$ は有界であるため、$\mu$ は適切です。上記の関係は、尺度 $\pi(\mu)$ と $\nu$ が同じ本質的な上積分を持ち、したがって等しいことを証明します (§1, No. 2、提案 2 の裏付け)。

最後に、$\pi$ が単射であると仮定して、b) を証明しましょう。 f を $\mathscr{F}_+(T)$ の元とします。 $\pi$ は単射なので、 $f = g \circ \pi$ と設定 $\nu = \pi(\mu) = \pi(\mu')$ となる写像 $g \in \mathscr{F}_+(X)$ が存在します。No. 3 の提案 4 により、次のようになります。

$$
\mu^\bullet(f) = \mu^\bullet(g \circ \pi) = \nu^\bullet(g) = {\mu'}^\bullet(g \circ \pi) = {\mu'}^\bullet(f).
$$

したがって、2 つのメジャー $\mu$ と $\mu'$ は同じ本質的な上積分を持ち、これはそれらの等式 (§ 1, No. 2、提案 2 の裏付け) を意味します。

#### 注意 {#int-ix-s2-n4-rem-1 .statement tag=09P3}

$\pi$ が単射だと仮定します。 $\theta$ を、$\pi$ が $\theta$-proper であり、$\pi(\theta) = 0$ であるような複素尺度とします。それから$\theta = 0$。実際、$\theta$ を実数と虚数の部分に分離することで、$\theta$ が実数である場合を簡約する理解できます。次に、$\pi(\theta^+) = \pi(\theta^-)$、したがって $\theta^+ = \theta^-$ (提案 8)、そして最後に $\theta = 0$ になります。

ここは、提案 8 の条件 a) が常に満たされる重要なケースです。

#### 命題 9 {#int-ix-s2-prop-9 .statement tag=09P4}

— *T をスーリン空間* (GT、IX, §6, No. 2、定義 2)、*X ハウスドルフ空間*、$\pi$ *T の X* への連続写像、および $\nu$ * X*。 *その後、T には $\pi(\mu) = \nu$* となるような有界メジャー $\mu$ が存在します。

この仮説は、X がスーリン空間であることを明らかに示唆しています。

$\mathfrak{P}(T)$ の集合写像 $c : A \mapsto \nu^\bullet(\pi(A))$ を考えてみましょう。 関係 $A \subset B$ は $c(A) \leq c(B)$ を意味します。 $(A_n)$ が T の部分集合の増加する数列であり、$A = \bigcup_{n \in \mathbf{N}} A_n$ であれば、$\nu^\bullet$ が負担であることから $c(A) = \sup_n c(A_n)$ となります。最後に、$A \subset T$ と $\varepsilon$ を数 $> 0$ とします。 選ぶ X 含む $\pi(A)$ の開いた部分集合 G、つまり $\nu^\bullet(G) \leq \nu^\bullet(\pi(A)) + \varepsilon$ (§ 1, No. 9、提案 13)。 T 含む A のオープン部分集合 $H = \overline{\pi^{-1}(G)}$ と $c(H) \leq c(A) + \varepsilon$。従って、写像 c は T 上の右連続容量 (TG、IX, §6, No. 10、定義 9)(1) であり、容量性に関する定理 (*loc. cit.*、Th. 6) は等式 $c(T) = \sup_K c(K)$ を意味し、ここで K はコンパクトの集合を超えます。 T. Prop. 8 の部分集合は、望ましい尺度 $\mu$ の存在を暗示します。

### 5. 2 小節中積

S と T を 2 つの位相幾何学空間とし、それぞれ 2 つの (正の) 事前測度 $\lambda$ と $\mu$ を備え、X を積空間 $S \times T$ とします。 K を X のコンパクト部分集合とする。 S と T 上の K の A と B 射影と集合で表しましょう

$$
\nu_K = (\lambda_A \otimes \mu_B)_K .
$$

従って、定義するはXの事前対策となります。なぜなら、L を X 含む K の圧縮部分集合とし、C と D をその 2 つの射影とするからです。その後、$A \subset C$、$B \subset D$、

(1) T 上の容量 $f$ は、T のすべてのコンパクト集合 K に対して、U が開いた集合 $U \supset K$ 上を走るときに $f(K) = \inf_U f(U)$ になる場合、右連続であると言われます。この概念は GT では定義されておらず、第 3 章の以前の版から翻訳されています。 IX。

従って、誘導措置の推移性と第2章の提案12を使用します。 V, §8, No. 5、私たちは持っています

$$
(\nu_L)_K = ((\lambda_C \otimes \mu_D)_L)_K = (\lambda_C \otimes \mu_D)_K \\
= ((\lambda_C \otimes \mu_D)_{A \times B})_K = (\lambda_A \otimes \mu_B)_K = \nu_K .
$$

#### 定義 6 {#int-ix-s2-def-6 .statement tag=09P5}

*(3) で定義された事前測定値 $\nu$ は、$\lambda$ と $\mu$ の事前測定値積と呼ばれ、$\lambda \otimes \mu$ と表されます。

この定義は、$\lambda$ と $\mu$ が複雑な事前措置であり、その場合に $|\lambda \otimes \mu| = |\lambda| \otimes |\mu|$ がある場合に明らかに拡大するします (Ch. III, §4, No. 2、Prop. 3 および Ch. IV, §5, No. 7、補題 3)。

Ch.の記法を保存します。 III, §4とCh. V, §8 はメジャーの積および反復積分に対して相対的です。特に、$f$ と $g$ がそれぞれ $S$ と $T$ で定義された 2 つの写像で、$\overline{\mathbf{R}}_+$ または $\mathbf{C}$ に値が定義されている場合、写像 $(s, t) \mapsto f(s)g(t)$ は$S \times T$は$f \otimes g$と表記されます。

#### 命題 10 {#int-ix-s2-prop-10 .statement tag=09P6}

*$\nu$を$\lambda$と$\mu$の前尺積とします。 写像 $f \in \mathscr{F}_+(S)$ および写像 $g \in \mathscr{F}_+(T)$ ごとに、*

$$
\nu^\bullet(f \otimes g) = \lambda^\bullet(f)\mu^\bullet(g) .
$$

*premeasure $\nu$ は、(4) を満たす $S \times T$ の唯一の premeasure です。*

$K$ (それぞれ $L$) は、$S$ (それぞれ $T$) のコンパクト部分集合の集合を超えるため、次のようになります。

$$
\begin{align*}
\nu^\bullet(f \otimes g) &= \sup_{K,L} \nu^\bullet_{K \times L}((f \otimes g)_{K \times L}) = \sup_{K,L} (\lambda_K \otimes \mu_L)^\bullet(f_K \otimes g_L) \\
&= \sup_{K,L} \lambda_K^\bullet(f_K) \cdot \mu_L^\bullet(g_L) = (\sup_K \lambda_K^\bullet(f_K)) (\sup_L \mu_L^\bullet(g_L)) \\
&= \lambda^\bullet(f)\mu^\bullet(g)
\end{align*}
$$

第 8 章の提案による。 V, §8, No. 3。

$\eta$ を $S \times T$ 満たす (4) の 2 番目の前措置とし、$K$ と $L$ をそれぞれ $S$ と $T$ のコンパクト部分集合、$f$ と $g$ 元とします。それぞれ$\mathscr{F}_+(K)$と$\mathscr{F}_+(L)$。 拡大 x 0 の間には関係 $(f \otimes g)^0 = f^0 \otimes g^0$ があるため、(§1, No. 2、提案 2)

$$
\eta^\bullet_{K \times L}(f \otimes g) = \eta^\bullet((f \otimes g)^0) = \eta^\bullet(f^0 \otimes g^0) \\
= \lambda^\bullet(f^0)\mu^\bullet(g^0) = \lambda_K^\bullet(f)\mu_L^\bullet(g) .
$$

特に、$f \in \mathscr{K}_+(K)$、$g \in \mathscr{K}_+(L)$ を取ると、$\eta_{K \times L}$ が積小節 $\lambda_K \otimes \mu_L$ の特徴性質を持っていることがわかります (Ch. III, §4, No. 1、Th. 1)。したがって、$\eta_{K \times L} = \nu_{K \times L}$; $S \times T$ のすべてのコンパクト部分集合は形 $K \times L$ の集合に含まれるため、誘導措置の推移性は $\eta = \nu$ を意味します。

#### 系 1 {#int-ix-s2-prop-10-cor-1 .statement tag=09P7}

— *$\lambda$と$\mu$がメジャーの場合、$\nu$はメジャーです。*

というのは、$x = (s, t)$ を $X$ の点とし、$U$ と $V$ をそれぞれ $s, t$ の近傍とし、$\lambda^\bullet(U) < +\infty$、$\mu^\bullet(V) < +\infty$ とします。 (4) により、集合 $U \times V$ は $x$ と $\nu^\bullet(U \times V) = \lambda^\bullet(U)\mu^\bullet(V) < +\infty$ の近傍になります。したがって、制約 $\nu^\bullet$ は局所的に制限されており、事前測定 $\nu$ は測定です。

この結果は、複雑な対策に対して一度に拡大するをもたらします。

#### 系 2 {#int-ix-s2-prop-10-cor-2 .statement tag=09P8}

— *$A$ が $\lambda$ に対して局所的に無視できる $S$ の部分集合である場合、$A \times T$ は局所的に $\nu$ が無視できます。*

#### 系 3 {#int-ix-s2-prop-10-cor-3 .statement tag=09P9}

— *$\lambda$ (それぞれ $\mu$) が、$S$ (それぞれ $T$) 上のメジャーの加算可能な族 $(\lambda_\alpha)_{\alpha \in A}$ (それぞれ $(\mu_\beta)_{\beta \in B}$) の和であると仮定します。ファミリ $(\lambda_\alpha \otimes \mu_\beta)_{(\alpha, \beta) \in A \times B}$ は合計可能であり、その和は $\lambda \otimes \mu$ になります。*

というのは、$p$ を負担$\sum_{\alpha, \beta} (\lambda_\alpha \otimes \mu_\beta)^\bullet$ とするからです。 $f \in \mathscr{F}_+(S)$ と $g \in \mathscr{F}_+(T)$ の場合、明らかに $p(f \otimes g) = \lambda^\bullet(f)\mu^\bullet(g)$ です。コルの証明次に、1 は、$p$ が局所的に有界であるため、ファミリー $(\lambda_\alpha \otimes \mu_\beta)$ が合計可能であることを示します (§ 1, No. 7、提案 7)。その和 $\eta$ は $\eta^\bullet = p$ (§ 1, No. 7、提案 7) を満たし、提案 10 は $\eta = \nu$ を暗示します。

### 6. 2 つの尺度の積に関する統合

※このNo.の$\lambda$と$\mu$はそれぞれ$S$と$T$の対策、$\nu$は$S \times T$の製品対策$\lambda \otimes \mu$を示します。 加法では、$f$ が $S \times T$ で正の写像である場合、$s \in S$ ごとに、$T$ では $f_s$ 写像 $t \mapsto f(s, t)$、そして $I_f$ 写像 $s \mapsto \mu^\bullet(f_s)$ で表します。 $S$に*

#### 補題 2 {#int-ix-s2-lem-2 .statement tag=09PA}

*$f$ を $S \times T$ での $\nu$ 測定可能な陽性写像とします。 $T$ の各コンパクト部分集合 $L$ について、$I_f^L$ を $S$ の写像 $s \mapsto \mu^\bullet(f_s \varphi_L)$ とします。その場合、写像 $I_f^L$ は $\lambda$ 可測であり、*

$$
(5) \quad I_f = \sup_L I_f^L
$$
$$
(6) \quad \nu^\bullet(f) = \sup_L \lambda^\bullet(I_f^L),
$$

*ここで、$L$ は、$T$ のコンパクトな部分集合の集合を上回ります。*

まず、包含 $L \subset L'$ が $I_f^L \leq I_f^{L'}$ を意味することに注目します。一方、$s \in S$すべてに対して$I_f^L(s) = \mu_L^\bullet((f_s)_L)$。したがって、公式 (5) は、で与えられる負担$\mu^\bullet$ の定義の明らか帰結になります。

§1, No. 2。 K が S のコンパクト部分集合、および L T のコンパクト部分集合である場合、構成によって $\nu_{K \times L} = \lambda_K \otimes \mu_L$ が成り立ち、Ch. の提案 7 が成り立ちます。 V, §8, No. 3 は関係を意味します

$$
\nu^\bullet(f \varphi_{K \times L}) = \lambda_K^\bullet((I_f^L)_K).
$$

さらに、$S \times T$ のすべてのコンパクト部分集合は、形 $K \times L$ のコンパクト集合に含まれます。 移行をすべての K および前述の公式のL にわたる上部エンベロープにすると、次の結果が得られます。

$$
\nu^\bullet(f) = \sup_L \sup_K \lambda_K^\bullet((I_f^L)_K) = \sup_L \lambda^\bullet(I_f^L),
$$

すなわち(6)です。

最後に、第 7 章の提案 7。 V, §8, No. 3 は、S のすべてのコンパクト部分集合 K に対する $I_f^L$ の制限が $\lambda_K$ 可測であることを意味します。これは、$I_f^L$ が $\lambda$ 可測であるというに相当します。

#### 命題 11 {#int-ix-s2-prop-11 .statement tag=09PB}

*f を $X = S \times T$ で定義された下位半連続写像 $\geqslant 0$ とします。*

a) *写像 $f_s : t \mapsto f(s, t)$ は、$s \in S$ ごとに T 上で半連続的に低くなります。*

b) *写像 $I_f : s \mapsto \int^\bullet f(s, t) d\mu(t)$ は S で下位の半連続であり、*

$$
\iint_X^\bullet f(s, t) d\nu(s, t) = \int_S^\bullet d\lambda(s) \int_T^\bullet f(s, t) d\mu(t).
$$

性質 *a)* は明らかです。なぜなら、T の $\overline{\mathbf{R}}$ への写像 $t \mapsto f(s, t)$ は、$f$ の合成であり、T の X への連続した写像 $t \mapsto (s, t)$ であるからです。 *b)* を確立するには、補題を利用します。

#### 補題 3 {#int-ix-s2-lem-3 .statement tag=09PC}

— *X をトポロジー 空間 (ハウスドルフかどうか)、f を X で定義された下位半連続写像 $\geqslant 0$ とします。この場合、f は X 上の下半連続写像の増加する数列 $(f_n)_{n \in \mathbf{N}}$ の極限であり、各写像 $f_n$ は特性写像の正の係数を持つ線形結合になります。オープン集合.*

2 つの整数 $k \geqslant 1$ と $n \geqslant 1$ が与えられた場合、区間 $]k/2^n, +\infty]$ の $\overline{\mathbf{R}}$ の特性写像を $J_{kn}$ で表しましょう。 $x \in \overline{\mathbf{R}}_+$、集合ごとに

$$
u_n(x) = 2^{-n} \sum_{k=1}^{n \cdot 2^n} J_{kn}(x);
$$

数列 $(u_n(x))_{n \geqslant 1}$ が増加するであり、x を極限として認めるのは明らかです。従って、写像 $f_n = u_n \circ f$ の数列は増加するで、$f$ に収束し、1 つは $f_n = 2^{-n} \sum_{k=1}^{n \cdot 2^n} \varphi_{U(k,n)}$ になります。
ここで、$U(k,n)$ は $X$ のオープン集合 $f^{-1}([k/2^n, +\infty])$ です。

b)の証明に進みます。 写像 $I_f$ は、写像 $I_f^L$ の増加する有向族の上の包絡線であり、$L$ は $T$ (補題 2) のコンパクト部分集合の集合を超えています。 写像 $I_f^L$ は下位の半連続です。 公式 (9) は、(6) から移行により、$L$ の上部包絡線まで演繹される可能性があります (§ 1, No. 6、提案 5)。

従って、$\mathscr{H}$ を、$S \times T$ 上の正の下位半連続写像 $f$ の集合とし、$T$ のすべてのコンパクト部分集合 $L$ について$I_f^L$ を下位半連続とします。 § 1, No. 6 の提案 5 により、$\mathscr{H}$ 属するから $\mathscr{H}$ までのすべての増加する有向集合元の上限。 従って、補題 3 までに、$S \times T$ 属するから $\mathscr{H}$ のオープン集合 $W$ の特性写像が証明されるだけで十分です。 さらに、$S \times T$の積位相の定義までに、オープン集合$W$は増加するの有向家族和集合、形のオープン集合の$(W_\alpha)_{\alpha \in A}$になります。
$$
W = \bigcup_{1 \leq i \leq n} (U_i \times V_i),
$$
ここで、$U_i$は$S$で開き、$V_i$は$T$で開きます。上で作成した注意によって、そのようなオープンな集合属するから$\mathscr{H}$の特徴写像を示すだけで十分です。 次に、$s \in S$ を、$s$ を含む開集合 $U_i$ によって形成されるファミリー (おそらく空) の共通点を $U$ とします。すべての $s' \in U$ と $t \in T$ に対して $\varphi_W(s,t) \leq \varphi_W(s',t)$ であることがすぐに分かります。従って、統合により、すべての $s' \in U$ に対して $I_{\varphi_W}^L(s) \leq I_{\varphi_W}^L(s')$ になります。 従って、$I_{\varphi_W}^L$は下位半連続となり、命題が成立します。

#### 系 1 {#int-ix-s2-lem-3-cor-1 .statement tag=09PD}

*$f$ を $X = S \times T$ で定義された正の数値写像とします。それから*
$$
\iint_X^* f(s,t)\, d\nu(s,t) \geq \int_S^* d\lambda(s) \int_T^* f(s,t)\, d\mu(t).
$$

なぜなら、$g$ を $g \geq f$ となるような $X$ の下位の半連続写像とします。提案 11 により、
$$
\iint_X^* g(s,t)\, d\nu(s,t) = \iint^* g(s,t)\, d\nu(s,t) = \int^* d\lambda(s) \int^* g(s,t)\, d\mu(t)
$$
$$
= \int^* d\lambda(s) \int^* g(s,t)\, d\mu(t) \geq \int^* d\lambda(s) \int^* f(s,t)\, d\mu(t).
$$
不等式 (10) は、$g$ の下側エンベロープに移行を加えることで得られます。

#### 系 2 {#int-ix-s2-lem-3-cor-2 .statement tag=09PE}

— $f$ を、$S \times T$ および $\nu$ で定義された数値写像とします。すると、写像 $f_s : t \mapsto f(s, t)$ は $\mu$ - $\lambda$ - ほぼすべての $s \in S$ に対して無視できます。

#### 命題 12 {#int-ix-s2-prop-12 .statement tag=09PF}

— $f$ を $X = S \times T$ で定義された $\nu$ で測定可能な正の写像とします。 $f$ が $\nu$ で緩和されていると仮定します (それぞれ $\mu$ が緩和されている)。次に:
a) 写像 $f_s : t \mapsto f(s, t)$ が $\mu$ 測定可能ではないような $s \in S$ の集合 $N$ は、$\lambda$ に関して無視できます (それぞれ局所的に無視できます)。
b) 写像 $s \mapsto \int^\bullet f(s, t) \, d\mu(t)$ は $\lambda$ 測定可能であり、

$$
\iint_X^\bullet f(s, t) \, d\nu(s, t) = \int_S^\bullet d\lambda(s) \int_T^\bullet f(s, t) \, d\mu(t).
$$

まず、$f$ が $\nu$ で緩和される場合の b) を確立することから始めます。 補題 2 までに、この主張の部分は、$f$ が $S \times L$ の外側にある零であるような、$T$ のコンパクト部分集合 $L$ が存在するときに有効になります。この場合、$T$ 含む $L$ のすべてのコンパクト部分集合 $L'$ に対して $I_f = I_f^{L'}$、および公式 (11) 簡約するから (6) です。特に、b) は、$S \times T$ のコンパクト部分集合の外側である零写像 $f$ に対して成立します。一方、Cor.提案 11 の 1 は、$f$ が $\nu$ が無視できる場合に b) が真であることを意味します。すべての $\nu$ で緩和された写像は、$\nu$ で無視できる写像の和と、コンパクトなサポート (§ 1, No. 9、提案 14 の Cor. 3) を備えた写像の数列であるため、主張 b) は真です$f$ が $\nu$ で管理されている場合。

同様に、主張 b) は、$\mu$ が $T$ (補題 2) のコンパクト部分集合 $L$ によって運ばれるとき、明らかです。 $\mu$ がモデレートされていると仮定します。その場合、$\mu = \sum_n \mu_n$ (§ 1, No. 9、提案 14 の Cor. 5)、よって $\nu = \sum_n \lambda \otimes \mu_n$ (No. 5、提案 10 の Cor. 3) のように、$T$ にはコンパクトなサポートを持つ数列 $(\mu_n)_{n \in \mathbf{N}}$ の措置が存在します。 主張 b) は、$\nu_n = \lambda \otimes \mu_n$ の各対策に有効ですが、$\nu = \sum_n \nu_n$ にも有効です。

a)を証明しましょう。 $f_s$ が $\mu$ 可測ではないように、$s \in S$ の $N$ 集合で表します。 $T$ のすべてのコンパクト部分集合 $L$ についても、同様に、$f_s \varphi_L$ が $\mu$ 可測ではないように、$s \in S$ の $N_L$ 集合で表されます。 $K$ と $L$ がそれぞれ $S$ と $T$ でコンパクトな集合である場合、$f_{K \times L}$ は測度 $\nu_{K \times L} = \lambda_K \otimes \mu_L$ と第 3 章の提案 2 に関して測定可能です。 V, § 8, No. 2 は、集合 $N_L$ が $\lambda_K$ に対して局所的に無視できることを示しています。 $K$ は任意であるため、$N_L$ は局所的には $\lambda$ は無視できます。

$f$ が形 $K \times L$ のコンパクト集合の外側にある零であるとします。次に$N = N_L$、そして$N$は$K$に含まれます。したがって、$N$ は $\lambda$ は無視できることになります。同様に、$f$ が $\nu$ 無視できる場合、Cor.提案 11 の 2 は、$N$ が $\lambda$ 無視できることを意味します。 $f$ が $\nu$ で緩和されているケースは、前述の 2 つのケースを組み合わせて、上記のように処理できます。

$\mu$ が $T$ のコンパクト部分集合 $L$ によって運ばれると仮定します。次に、再び$N = N_L$となるため、$N$は局所的には$\lambda$-無視できます。すべての緩和措置は、コンパクトなサポート ($§ 1$、No. 9、提案 14 の Cor. 5) を備えた措置の和のうち数列であるため、この結果は、$§ 1$ の提案 8 を使用すると、$\mu$ が緩和された場合にすぐに拡大するになります。 No. 7。

#### 注意 {#int-ix-s2-n6-rem-1 .statement tag=09PG}

— $(K_\alpha)_{\alpha \in A}$ を $\lambda$ に対する $S$ の粉砕とし、$M = S - \bigcup_{\alpha \in A} K_\alpha$ とします。 $T$ のメジャー $\mu$ に対して、同様の方法で $(L_\beta)_{\beta \in B}$ と $N$ を定義する使用します。 $S$ の部分空間 $K_\alpha$ と *離散* 空間 $M$ の合計である局所的にコンパクトな空間を $S'$ で表します。空間$T'$も同様に定義され、$X' = S' \times T'$を設定します。 局所的にコンパクトな空間 $X'$ は、$X$ のコンパクト部分空間の族 $(K_\alpha \times L_\beta)_{(\alpha, \beta) \in A \times B}$ の和と、$X$ の局所的に $\nu$ 無視できる部分集合である部分空間 $P = (M \times T) \cup (S \times N)$ です。 $P$ は一般に、離散的な空間ではありません)。 $§ 1$、No. 8 の *Scholium* で、$S'$ に測度 $\lambda'$ が存在し、可測写像、正の写像の本質的な上積分、本質的に可積分関数とそれらの積分が $\lambda$ と同じであることを見ました。 $\lambda'$。 引用した Scholium に従って、$T'$ の測定値 $\mu'$ を $\mu$ に関連付け、$X'$ の測定値 $\nu'$ を $\nu$ に関連付けます。 $f \in \mathscr{F}_+(S)$ と $g \in \mathscr{F}_+(T)$ が ${\nu'}^\bullet(f \otimes g) = {\lambda'}^\bullet(f) {\mu'}^\bullet(g)$ であることがすぐにわかります。したがって、No. 5 の提案 10 により $\nu' = \lambda' \otimes \mu'$ となります。 $X'$の位相は$X$のより細かいであるため、すべての$\nu$-緩和された写像は$\nu'$-緩和されます。 この手順により、新しい証明を使用せずに Lebesgue-Fubini 定理を拡張することができます (Ch. V、$§ 8$、No. 4、TH。 １）現状まで。

### 7. 対策崩壊の結果

#### 命題 13 {#int-ix-s2-prop-13 .statement tag=09PH}

*$X$ をトポロジー 空間、$\nu$ を $X$、$p$ をトポロジカル空間 $T$、$\mu = p(\nu)$ への $X$ の $\nu$-適切な写像とする。 $X$ のすべてのコンパクト部分空間がメトリズ可能であると仮定します。次に、以下のプロパティを持つ $T$ の写像 $t \mapsto \lambda_t$ が $\mathscr{M}_+(X)$ に存在します。

a) $t \in T$ ごとに、メジャー $\lambda_t$ が $\overline{p}^{-1}(t)$ によって実行されます。
b) $X$ で普遍的に測定可能なすべての$^{(1)}$ 陽性写像 $f$ について、写像 $t \mapsto \lambda_t^\bullet(f)$ は$T$ で普遍的に測定可能であり、*

$$
\int_X f(x)\, d\nu(x) = \int_T d\mu(t) \int_X f(x)\, d\lambda_t(x);
$$

(1) トポロジカル空間 $X$ からトポロジカル空間 $Y$ への写像は、$X$ (cf.) のすべての測度 $\mu$ について $\mu$ 可測である場合、 *普遍的に可測* であると言われます。章V、$§ 3$、No. 4）。

c) $\lambda_t(1) \neq 1$ が局所的に $\mu$ を無視できるような $t \in T$ の集合。
さらに、$t \mapsto \lambda'_t$ が $T$ の写像を $\mathscr{M}_+(X)$ 満たす条件 a) および b) にすると、$\lambda_t \neq \lambda'_t$ が局所的に$\mu$ 無視できるように、$t \in T$ の集合になります。
補助的な結果が必要になります。

#### 補題 4 {#int-ix-s2-lem-4 .statement tag=09PI}

$X$ をトポロジー 空間、$\nu$ を $X$ のメジャー、$f$ を $X$ の $\nu$ 可測写像をトポロジー 空間 $F$ にするとします。 （ハウスドルフかどうか）。 $X$ から $F$ への普遍的に測定可能な写像 $f'$ が存在し、局所的には $\nu$ に等しい $f$ がほぼどこでも存在します。

証明は、第 4 章の提案 7 と同じです。 V, §3, No. 4、§1, No. 8の提案10を考慮した上で。

提案 13 の証明に進みます。
A) $X$ がコンパクトで計化可能であり、$p$ が連続で全射であると仮定します。
空間 $T$ はコンパクトで計量化可能です (GT、IX, §2, No. 10)。 Thさんより1章 VI, §3, No. 1、$T$ の $\mathscr{M}_+(X)$ への写像 $H : t \mapsto \eta_t$ が存在し、漠然と $\mu$ 可測でスカラー的に本質的に $\mu$ 積分可能であり、$\nu = \int_T \eta_t \, d\mu(t)$ や$\eta_t$ は総質量 1 を持ち、 $t \in T$ごとに$\overline{p}(t)$。 $(S_n)_{n \in \mathbf{N}}$ を $\mu$ に対する $T$ の破砕とし、各集合 $S_n$ に対する $H$ の制限が連続するようにします (§1, No. 8、提案 10 および 11)。 $\Lambda : t \mapsto \lambda_t$ によって、$T$ から $\mathscr{M}_+(X)$ へのマッピングを表します。これは、$S = \bigcup_{n \in \mathbf{N}} S_n$ では $H$、$T - S$ では 0 に等しくなります。 $\nu = \int_T \lambda_t \, d\mu(t)$ と $\Lambda$ が主張の条件 a) を満たすことは明らかです。
$\theta$ を $T$ のメジャーとします。 写像 $\Lambda$ は漠然と $\theta$ 測定可能であり、スカラー的に本質的に $\theta$ 積分可能であるため、$\theta$ も適切です (Ch. V, §3, No. 1、提案 2 b))。 $f$ を、$X$ に対する普遍的に測定可能なポジティブな写像とします。第 5 章の提案による。 $\int \lambda_t \, d\theta(t)$、写像 $t \mapsto \lambda_t^\bullet(f)$ に適用されるV, §3, No. 2 は、$\theta$ 可測であるため、$\theta$ の恣意性を考慮すると普遍的に可測である。
公式 (12) は、第 5 章の提案 5 からの結果です。 V, §3, No. 2。
B) メジャー $\nu$ を運ぶ $X$ のコンパクト部分集合 $X'$ が存在し、$p_{X'}$ が連続であると仮定します。
集合 $T' = p(X')$、および $p' = p_{X'}$; $\nu_{X'}$ の小節を $\nu'$ で表し、$T'$ の$p'(\nu')$ の小節を $\mu'$ 像で表します。 $p'$ は連続で全射的であり、$X'$ はコンパクトで計数可能であるため、A) により、$T'$ の写像 $\Lambda' : t' \mapsto \lambda'_{t'}$ が $\mathscr{M}_+(X')$ 満たすに次の条件として存在します。
a') $t' \in T'$ ごとに、メジャー $\lambda'_{t'}$ が $X' \cap \overline{p}'(t')$ によって実行されます。
b') $X'$ の普遍的に測定可能なすべての陽性写像 $f'$ について、写像 $t' \mapsto {\lambda'_{t'}}^\bullet(f')$ は $T'$ に普遍的に測定可能であり、
$$
\int_{X'} f'(x') \, d\nu'(x') = \int_{T'} d\mu'(t') \int_{X'} f'(x') \, d\lambda'_{t'}(x').
$$

$t \in T$ にしましょう。 $t$ が $T'$ に属する場合、$X'$ を $X$ に正規注入した後の $\lambda'_t$ のイメージを $\lambda_t$ で表し、$t$ が $T - T'$ に属する場合、$\lambda_t = 0$ を設定します。 読者は、写像 $t \mapsto \lambda_t$ が条件主張の a) および b) を満たすことを問題なく検証するでしょう。

C) *一般的な場合の存在*:

$X$ の措置 $\nu$ が緩和されると、$\nu$ の統合可能なオープン集合の $X$ からなるの$(U_m)_{m \in \mathbf{N}}$ を選ぶカバーすることができます。 加法 $(X_n)_{n \in \mathbf{N}}$ を、$p$ の制限からそれぞれの集合 $X_n$ が連続となるように、$X$ の $\nu$ 粉砕とする（§ 1, No. 8、提案 10 および 11）。 $X$ の小節 $\varphi_{X_n} \cdot \nu$ を $\nu_n$ で表し、$p$ の下の像を $\mu_n$ で表します。 B) により、$T$ の整数 $n \in \mathbf{N}$、写像 $t \mapsto \alpha^n_t$ ごとに、$\mathscr{M}_+(X)$ 満たすに次の条件が存在します。

$a'')$ メジャー $\alpha^n_t$ は、すべての $t \in T$ に対して $\overline{p}(t)$ によって実行されます。

$b'')$ $f$ が $X$ の普遍的に測定可能なポジティブ写像である場合、$T$ のポジティブ写像 $t \mapsto (\alpha^n_t)^*(f)$ は普遍的に測定可能であり、

$$
\int_X f(x)\, d\nu_n(x) = \int_T d\mu_n(t) \int_X f(x)\, d\alpha^n_t(x).
$$

1 つは $\nu = \sum_{n \in \mathbf{N}} \nu_n$ と $\mu = \sum_{n \in \mathbf{N}} \mu_n$ です。 No. 2 の提案 3 と上記の補題 4 からすぐに、$T$ には普遍的に測定可能な陽性写像の数列 $(g_n)_{n \in \mathbf{N}}$ が存在し、すべての $n \in \mathbf{N}$ に対して$\mu_n = g_n \cdot \mu$ となり、$\sum_{n \in \mathbf{N}} g_n = 1$ となることがわかります。すべての $t \in T$ について、$X$ の措置 $g_n(t) \cdot \alpha^n_t$ を $\beta^n_t$ で、$X$ の負担 $\sum_{n \in \mathbf{N}} (\beta^n_t)^*$ を $q_t$ で表します。 $f$ を、$X$ における普遍的に測定可能なポジティブな写像とします。 No. 2 の提案 2 を使用し、(13) で $n$ を合計すると、次のようになります。

$$
\int_X f(x)\, d\nu(x) = \int_T q_t(f)\, d\mu(t);
$$

さらに、$T$ 上の写像 $t \mapsto q_t(f)$ は普遍的に測定可能であることは明らかです。

すべての $m \in \mathbf{N}$ について、$E_m$ を $t \in T$ の集合とし、$q_t(U_m) = +\infty$ とします。 集合 $E_m$ は、写像 $t \mapsto q_t(U_m)$ にも当てはまるため普遍的に測定可能であり、$\nu^*(U_m)$ は有限であるため、$E_m$ は$f = \varphi_{U_m}$ に適用される公式 (14) によって局所的に $\mu$ は無視できます。したがって、集合 $E = \bigcup_{m \in \mathbf{N}} E_m$ は普遍的に測定可能であり、局所的には $\mu$ は無視できます。私たちは $t \in E$ に対して集合 $\lambda_t = 0$ です。さらに、$t \in T - E$; とします。オープン集合 $U_m$ カバー$X$ と$q_t(U_m)$ が有限であるため、制約$q_t$ は局所的に有界です。 § 1, No. 7の提案7により、$X$には$q_t = \lambda_t^*$と$\lambda_t = \sum_{n \in \mathbf{N}} \beta^n_t$のような尺度$\lambda_t$が存在します。 写像 $t \mapsto \lambda_t$ が主張の条件 a) と b) を満たすのは明らかです。

D) c)* の *証明:
$f$ を、正で有界である $X$ で普遍的に測定可能な写像とします。 $T$ における普遍的に測定可能な写像 $h_f : t \mapsto \lambda_t^\bullet(f)$ は、$\mu = p(\nu)$ に対する尺度 $\mu_f = p(f \cdot \nu)$ に対して稠密度であることを示します。 $K$を$T$の圧縮部分集合とし、$A = \overline{p}^{-1}(K)$とします。 $t \in T$ ごとに、$\lambda_t$ のメジャーは $\overline{p}^{-1}(t)$ によって実行されます。 $t$ 属するから $K$ の場合、$\overline{p}^{-1}(t) \subset A$、よって $\lambda_t^\bullet(f \varphi_A) = \lambda_t^\bullet(f)$;一方、$t$ 属するから $T - K$ の場合、$\overline{p}^{-1}(t) \subset X - A$、よって $\lambda_t^\bullet(f \varphi_A) = 0$ となります。 適用公式 (12) から $f \cdot \varphi_A$,$^{(1)}$ を取得します

$$
\mu_f(K) = \int_A^\bullet f(x)\, d\nu(x) = \int_K^\bullet d\mu(t) \int_X^\bullet f(x)\, d\lambda_t(x) = \int_K^\bullet h_f(t)\, d\mu(t),
$$

これにより、関係 $\mu_f = h_f \cdot \mu$ が確立されます。

$f = 1$ とすると、写像 $h_1 : t \mapsto \| \lambda_t \|$ は、$\mu$ に対するメジャー $\mu_1 = \mu$ の稠密度であるため、局所的には $\mu$ - $T$ のほぼどこでも 1 に等しいことがわかります。

E) *一意性*:
$t \mapsto \lambda_t^i$ ($i = 1, 2$ の場合) を、$T$ の 2 つの写像を $\mathscr{M}_+(X)$ 満たす条件 a) と b) 主張にするとします。 C) と同様に、選ぶは、$n \in \mathbf{N}$ および集合 $N = X - \bigcup_{n \in \mathbf{N}} X_n$ ごとに $p_{X_n}$ が連続するように、$X$ の $\mu$ を破砕する $(X_n)_{n \in \mathbf{N}}$ です。 整数 $n \in \mathbf{N}$、選ぶごとに、$X$ に正の写像、$X_n$ の外側に零の可算集合 $D_n$ があり、制限から $X_n$ までです。 形は、標準の空間 $\mathscr{C}(X_n)$ における密な集合 (GT の Th. 1、X, §3, No. 3 を計量可能コンパクト空間 $X_n$ に適用)。私たちは集合 $D = \bigcup_{n \in \mathbf{N}} D_n$です。

$f \in D$ にしましょう。 D による)、写像 $t \mapsto (\lambda_t^1)^\bullet(f)$ と $t \mapsto (\lambda_t^2)^\bullet(f)$ は、$\mu$ に関するメジャー $\mu_f$ の密度であるため、$T$ には局所的に無視できる$\mu$ 集合 $E_f$ が存在します。 $(\lambda_t^1)^\bullet(f) = (\lambda_t^2)^\bullet(f)$ は $t \in T - E_f$ です。さらに、(12) により、$t \in T$ の集合 $F_i$ は、$(\lambda_t^i)^\bullet(N) \neq 0$ が局所的に $\mu$ から $i = 1, 2$ に対して無視できるものになります。 $D$ は可算であるため、集合 $G = (\bigcup_{f \in D} E_f) \cup F_1 \cup F_2$ は局所的には $\mu$ は無視できます。 $t \in T - G$ の場合、§1, No. 8 の提案 9 により、$(\lambda_t^1)^\bullet(N) = (\lambda_t^2)^\bullet(N) = 0$ と $(\lambda_t^1)_{X_n} = (\lambda_t^2)_{X_n}$、よって $\lambda_t^1 = \lambda_t^2$ が得られます。

Q.E.D.

#### 注意 {#int-ix-s2-n7-rem-1 .statement tag=09PJ}

— 1) $X$ がスーリン空間である場合、$X$ のすべてのコンパクト部分空間はスーリン空間であるため、計量化可能です (TG、IX、付録 I、Prop. 2 の Cor. 2)。 3)、$^{(2)}$

(1) $f \cdot \varphi_A$ が普遍的に測定できない場合は、以下の *注意 2*) を使用します。
(2) この結果は GT には現れません (cf. §1, No. 9 の *注意 1* の脚注)。

そして、X のすべての小節は緩和されます (§ 1, No. 9、注意 1)。したがって、提案 13 によれば、X のすべての措置 $\nu$ は、すべての $\nu$ の適切な写像に関して崩壊を認めることになります。

2) 提案 13 の記法により、$f$ を正の $\nu$ 可測写像とします。 1 つの証明できる、第 3 章と同様。 V, § 3, No. 2、提案 5、$f$ が $\lambda_t$ 測定可能ではないような $t \in T$ の集合は局所的に $\mu$ 無視できるものであり、$t \mapsto \lambda_t^\bullet(f)$ は $\mu$ 測定可能であり、 関係 (12) が再び成り立ちます。

### 練習問題 {#int-ix-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
