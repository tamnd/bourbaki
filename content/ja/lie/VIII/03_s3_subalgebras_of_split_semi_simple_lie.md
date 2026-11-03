---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 3
section_title: Subalgebras of split semi-simple Lie algebras
lang: ja
source: lie-vii-ix
book_pages: 86-95, 229-231
pdf_pages: 0094-0103, 0237-0239
extraction: native
subsections:
    - "no": 1
      title: SUBALGEBRAS STABLE UNDER ad $\mathfrak{h}$
      page: 86
      pdf_page: 94
    - "no": 2
      title: IDEALS
      page: 89
      pdf_page: 97
    - "no": 3
      title: BOREL SUBALGEBRAS
      page: 90
      pdf_page: 98
    - "no": 4
      title: PARABOLIC SUBALGEBRAS
      page: 92
      pdf_page: 100
    - "no": 5
      title: NON-SPLIT CASE
      page: 94
      pdf_page: 102
statements: 28
exercises: 14
content_sha256: 366856b08c284d4fe68749c656d811b72b4cdc70be0a694d4b227fba922c7b77
translated_from: content/en/lie/VIII/03_s3_subalgebras_of_split_semi_simple_lie.md
translation_method: google
source_content_sha256: 043e172960e451fa011db5fc5b2cdd69d22334e7720054bdacde767c930f9a50
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 20e4b79281c2ebe8783441f433a280420d62c2e34eb53066fceab1b12f5a9ca6
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 3。 部分代数/分裂半単純リー代数

この段落では、$(\mathfrak{g},\mathfrak{h})$ 分裂半単純リー代数を表し、根系を R で表します。

### 1. 部分代数広告下で安定 $\mathfrak{h}$

#### 補題 1 {#lie-viii-s3-lem-1 .statement tag=00ZO}

V を $\mathfrak{g}$ のベクトル部分空間および $\mathfrak{g}^{\alpha}\subset V$ となるように $\alpha \in R$ の R(V) 集合とします。次に、$(V\cap \mathfrak{h}) +\sum_{\alpha\in R(V)}\mathfrak{g}^{\alpha}$ は、広告 $\mathfrak{h}$ の下で、V の最大のベクトル部分空間です。

ベクトル部分空間 V の W が広告 $\mathfrak{h}$ の下で安定しているのは、次の場合に限ります。

$$
W = (W\cap \mathfrak{h}) +\sum_{\alpha\in R}(W\cap \mathfrak{g}^{\alpha})
$$

(代数、第 VII, §2, no. 2、コリント 1 章 1)。 $\mathfrak{h}$ の下で安定している V の最大のベクトル部分空間は、$(V\cap \mathfrak{h}) +\sum_{\alpha\in R}(V\cap \mathfrak{g}^{\alpha})$ になります。 ただし、$\alpha \in R(V)$ の場合は $V\cap \mathfrak{g}^{\alpha}=\mathfrak{g}^{\alpha}$、$\mathfrak{g}^{\alpha}= 1$ が暗いため、$\alpha  \notin R(V)$ の場合は $V\cap \mathfrak{g}^{\alpha}= 0$ です。 Q.E.D.

R の任意の部分集合 P に対して、

$$
\mathfrak{g}^P=\sum_{\alpha\in P}\mathfrak{g}^{\alpha}\mathfrak{h}_P=\sum_{\alpha\in P}\mathfrak{h}_{\alpha}
$$

$P\subset R$ と $Q\subset R$ の場合、明らかに

$$
[\mathfrak{h},\mathfrak{g}^P]\subset \mathfrak{g}^P \tag{1}
$$

$$
[\mathfrak{g}^P,\mathfrak{g}^Q] =\mathfrak{g}^{(P+Q)\cap R}+\mathfrak{h}_{P\cap(-Q)} \tag{2}
$$

Recall (Chap. VI, §1, no. 7, Def. 4) that a subset P of R is said to be closed if the conditions $\alpha \in P, \beta \in P, \alpha +\beta \in R$ imply $\alpha +\beta \in P$, in other words if $(P + P)\cap R\subset P$.

#### 補題 2 {#lie-viii-s3-lem-2 .statement tag=00ZP}

$\mathfrak{h}'$ を $\mathfrak{h}$ のベクトル部分空間および R の P 部分集合とします。すると、P が R の閉じた部分集合である場合に限り、$\mathfrak{h}'+\mathfrak{g}^P$ は $\mathfrak{g}$ の部分代数になります。

$$
\mathfrak{h}'\supset \mathfrak{h}_{P\cap(-P)}
$$

確かに、

$$
[\mathfrak{h}'+\mathfrak{g}^P,\mathfrak{h}'+\mathfrak{g}^P] = [\mathfrak{h}',\mathfrak{g}^P] + [\mathfrak{g}^P,\mathfrak{g}^P] =\mathfrak{h}_{P\cap(-P)}+ [\mathfrak{h}',\mathfrak{g}^P] +\mathfrak{g}^{(P+P)\cap R}
$$

したがって、次の場合に限り、$\mathfrak{h}'+\mathfrak{g}^P$ は $\mathfrak{g}$ の部分代数になります。

$\mathfrak{h}_{P\cap(-P)}\subset \mathfrak{h}'$ と $\mathfrak{g}^{(P+P)\cap R}\subset \mathfrak{g}^P$

これは補題を証明します。

#### 命題 1 {#lie-viii-s3-prop-1 .statement tag=00ZQ}

(i) ad$\mathfrak{h}$ で安定した $\mathfrak{g}$ の部分代数は、形 $\mathfrak{h}'+\mathfrak{g}^P$ のベクトル部分空間であり、P は R の閉じた部分集合で、$\mathfrak{h}'$ は R のベクトル部分空間です。 $\mathfrak{h}$ 含む $\mathfrak{h}_{P\cap(-P)}$。

(ii) $\mathfrak{h}',\mathfrak{h}''$ を $\mathfrak{h}$ のベクトル部分空間と $P,Q$ を R の $\mathfrak{h}'\supset \mathfrak{h}_{P\cap(-P)},\mathfrak{h}''\subset \mathfrak{h}'$ と $Q\subset P$ で閉じた部分集合とする。したがって、$\mathfrak{h}''+\mathfrak{g}^Q$ は、次の場合に限り、$\mathfrak{h}'+\mathfrak{g}^P$ の理想となります。

$(P + Q)\cap R\subset Q$ と $\mathfrak{h}_{P\cap(-Q)}\subset \mathfrak{h}''\subset \bigcap_{\alpha\in P,\alpha  \notin Q}$ カー $\alpha$。

主張 (i) は、補題 1 と 2 の直後に続きます。$\mathfrak{h}',\mathfrak{h}'',P,Q$ を (ii) のようにします。それから

$$
[\mathfrak{h}'+\mathfrak{g}^P,\mathfrak{h}''+\mathfrak{g}^Q] =\mathfrak{h}_{P\cap(-Q)}+ [\mathfrak{h}',\mathfrak{g}^Q] + [\mathfrak{h}'',\mathfrak{g}^P] +\mathfrak{g}^{(P+Q)\cap R}
$$

したがって、$\mathfrak{h}''+\mathfrak{g}^Q$ は、次の場合に限り、$\mathfrak{h}'+\mathfrak{g}^P$ の理想となります。

$$
\mathfrak{h}_{P\cap(-Q)}\subset \mathfrak{h}'',[\mathfrak{h}'',\mathfrak{g}^P]\subset \mathfrak{g}^Q,\mathfrak{g}^{(P+Q)\cap R}\subset \mathfrak{g}^Q
$$

これは (ii) を意味します。

#### 命題 2 {#lie-viii-s3-prop-2 .statement tag=00ZR}

$\mathfrak{a}$ を ad$\mathfrak{h}$ で安定した $\mathfrak{g}$ の部分代数とし、$\mathfrak{h}'\subset \mathfrak{h}$、$P\subset R$ を $\mathfrak{a}=\mathfrak{h}'+\mathfrak{g}^P$ となるようにします。

(i) $\mathfrak{k}$ を、すべての $\alpha \in P\cap (-P)$ に対して $\alpha (x) = 0$ となるように、$x\in \mathfrak{h}'$ の集合とします。 $\mathfrak{a}$の根基は$\mathfrak{k}+\mathfrak{g}^Q$で、Qは$\alpha \in P$の集合で、$-\alpha  \notin P$になります。さらに、$\mathfrak{g}^Q$ は $\mathfrak{a}$ の無力のイデアです。

(ii) $\mathfrak{a}$ は、$P =-P$ と $\mathfrak{h}'=\mathfrak{h}_P$ の場合に限り、半単純になります。

(iii) $\mathfrak{a}$ は、$P\cap (-P) =\emptyset$ の場合にのみ解決可能です。その場合、$[\mathfrak{a},\mathfrak{a}] =\mathfrak{g}^S$、ここで

$$
S = ((P + P)\cap R)\cup  \{\alpha \in P|\alpha (\mathfrak{h}')\not= 0\}
$$

(iv) $\mathfrak{a}$ は、$P =-P$ の場合にのみ、$\mathfrak{g}$ で還元的です。

(v) $\mathfrak{a}$ は、$\mathfrak{h}'= 0$ の場合に限り、冪零元から構成されます。次に、$P\cap (-P) =$ $\emptyset$、そして $\mathfrak{a}$ はゼロになります。

(v) を証明します。 $\mathfrak{a}$ が冪零元で構成されている場合、$\mathfrak{a}$ は明らかに無能であり、$\mathfrak{h}$ の元は半単純であるため、$\mathfrak{h}'= 0$ になります。 $\mathfrak{h}'= 0$ と仮定します。提案 1 (i)、$P\cap (-P) =\emptyset$ による。章著。 VI, §1, no. 7、提案 22、$P\subset R_+(C)$ となるような R の部屋 C が存在します。したがって、次の特性を持つ整数 $n >0$ が存在します: $\alpha_1, . . . , \alpha_n\in P$ と $\beta \in R\cup  \{0\}$ の場合、

$$
\alpha_1+\cdots +\alpha_n+\beta  \notin R\cup  \{0\}
$$

これは、$\mathfrak{g}^P$ のすべての元が無能であることを意味します。したがって (v)。

(iii) を証明します。 $P\cap (-P) =\emptyset ,\mathfrak{g}^P$ が $\mathfrak{g}$ の部分代数であり (提案 1 (i))、(v) により零能である場合。今

$$
[\mathfrak{a},\mathfrak{a}] = [\mathfrak{h}',\mathfrak{g}^P] + [\mathfrak{g}^P,\mathfrak{g}^P] = [\mathfrak{h}',\mathfrak{g}^P] +\mathfrak{g}^{(P+P)\cap R}\subset \mathfrak{g}^P
$$

したがって、$\mathfrak{a}$ は解け、$[\mathfrak{a},\mathfrak{a}]$ は命題の公式によって与えられます。 $P\cap (-P)\not=\emptyset$ の場合、$\alpha \in P$ は $-\alpha \in P$ となるようにします。すると、$\mathfrak{h}_{\alpha}+\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$は$\mathfrak{a}$の単純部分代数なので、$\mathfrak{a}$は解けません。

(i) を証明します。 Pが休みなので$(P + Q)\cap R\subset P$。 $\alpha \in P, \beta \in Q$ と $\alpha +\beta \in R$ の場合、できないには $\alpha +\beta \in  -P$ があり、P が閉じているため、これは $\beta \in Q$ に対して $-\beta =-(\alpha +\beta ) +\alpha \in P$ であることを意味します。従って、$(P + Q)\cap R\subset Q$。これは、$\mathfrak{g}^Q$ が $\mathfrak{a}$ のイデアルであり、(v) によって零であることを証明します。 $P\cap (-Q) =\emptyset$と$P\cap (-P) = P\cap \complement Q$があるので、$\mathfrak{h}_{P\cap(-Q)}\subset \mathfrak{k}\subset \bigcap_{\alpha\in P,\alpha  \notin Q}$カー$\alpha$です。提案 1 (ii) により、

$\mathfrak{k}+\mathfrak{g}^Q$は$\mathfrak{a}$の理想です。 $Q\cap (-Q) =\emptyset$ 以降、この理想は (iii) によって解決できます。従って、$\mathfrak{a}$の根基$\mathfrak{r}$に含まれます。 $\mathfrak{r}$ はすべての導分で安定しているため、$\mathfrak{a},\mathfrak{r}$ は広告 $\mathfrak{h}$ で安定しています。従って、$\mathfrak{r}= (\mathfrak{r}\cap \mathfrak{h}) +\mathfrak{g}^S$となるような P の部分集合 S が存在します。 $\alpha \in S$ と $-\alpha \in P$ と仮定します。次に、$\mathfrak{h}_{\alpha}= [\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}]\subset \mathfrak{r}$、つまり $\mathfrak{g}^{-\alpha}= [\mathfrak{h}_{\alpha},\mathfrak{g}^{-\alpha}]\subset \mathfrak{r}= 0$、つまり $-\alpha \in S$ です。 (iii) により、この矛盾するは $\mathfrak{r}$ が解決可能であるという事実がわかります。その結果、$S\subset Q$となります。最後に、$x\in \mathfrak{r}\cap \mathfrak{h}$ と $\alpha \in P\cap (-P)$ の場合、$[x,\mathfrak{g}^{\alpha}]\subset \mathfrak{g}^{\alpha}\cap \mathfrak{r}= 0$、つまり $\alpha (x) = 0$ です。これは$x\in \mathfrak{k}$を示しています。従って、(i) の$\mathfrak{r}\subset \mathfrak{k}+\mathfrak{g}^Q$ と証明が完了します。

(iv) を証明します。 By (i), the adjoint representation of $\mathfrak{a}$ on $\mathfrak{g}$ is semi-simple if and only if ad$_{\mathfrak{g}}x$ is semi-simple for all $x\in \mathfrak{k}+\mathfrak{g}^Q$ (Chap. I, §6, no. 5, Th. 4); by (v), this is the case if and only if $Q =\emptyset$, in other words $P =-P$.

(ii)を証明します。 $\mathfrak{a}$ が半単純の場合、(i) により $P =-P$ なので、$\mathfrak{h}_P\subset \mathfrak{h}'$;さらに$\mathfrak{a}= [\mathfrak{a},\mathfrak{a}]\subset \mathfrak{h}_P+\mathfrak{g}^P$、その結果$\mathfrak{h}'=\mathfrak{h}_P$となります。 $P =-P$ と $\mathfrak{h}'=\mathfrak{h}_P,\mathfrak{a}$ が (iv) と $\mathfrak{a}=\sum_{\alpha\in P}\mathfrak{s}_{\alpha}$ で還元できる場合、$\mathfrak{a}= [\mathfrak{a},\mathfrak{a}]$ と $\mathfrak{a}$ は半単純になります。

#### 命題 3 {#lie-viii-s3-prop-3 .statement tag=00ZS}

$\mathfrak{a}$ を ad($\mathfrak{h}$) の下で安定な $\mathfrak{g}$ の半単純部分代数とし、P を $\mathfrak{a}=\mathfrak{h}_P+\mathfrak{g}^P$ となるような R の部分集合とする。

(i) $\mathfrak{h}_P$ は $\mathfrak{a}$ の分裂カルタン部分代数です。

(ii) $(\mathfrak{a},\mathfrak{h}_P)$ の根系は、P の制限の集合から P の元の $\mathfrak{h}_P$ です。

$\mathfrak{h}_P$ は ad $\mathfrak{h}$ の下で安定しているため、$\mathfrak{a}$ の正規化器は ad $\mathfrak{h}$ の下で安定しており、したがって $Q\subset P$ (補題 1) である形 $\mathfrak{h}_P+\mathfrak{g}^Q$ になります。 $\alpha \in Q$の場合、

$$
\mathfrak{g}^{\alpha}= [\mathfrak{h}_{\alpha},\mathfrak{g}^{\alpha}]\subset [\mathfrak{h}_P,\mathfrak{g}^{\alpha}]\subset \mathfrak{h}_P
$$

それは不合理です。したがって、$Q =\emptyset$ と $\mathfrak{h}_P$ は、$\mathfrak{a}$ における独自のノーマライザーです。これは、$\mathfrak{h}_P$が$\mathfrak{a}$のカルタン部分代数であることを証明します。 $x\in \mathfrak{h}_P$、ad$_{\mathfrak{g}}x$、およびなおさら ad$_{\mathfrak{a}}x$ は三角化可能です。したがって、(i) は証明され、(ii) は明らかです。

提案 1 (i) により、$\mathfrak{g}$ 含む $\mathfrak{h}$ の部分代数は集合 $\mathfrak{h}+\mathfrak{g}^P$ であり、P は R の閉じた部分集合です。 VII, §3、提案 3、$\mathfrak{h}+\mathfrak{g}^P$ のすべてのカルタン部分代数は、$\mathfrak{g}$ のカルタン部分代数です。

#### 命題 4 {#lie-viii-s3-prop-4 .statement tag=00ZT}

$\mathfrak{a}$ を $\mathfrak{g}$ の部分代数含む $\mathfrak{h},x$ $\mathfrak{a},s$ の元と $n$ をその半単純とゼロポテント成分とします。続いて$s\in \mathfrak{a}$と$n\in \mathfrak{a}$。

(ad $x$)$\mathfrak{a}\subset \mathfrak{a}$ があるので、(ad $s$)$\mathfrak{a}\subset \mathfrak{a}$ と (ad $n$)$\mathfrak{a}\subset \mathfrak{a}$ です。 $\mathfrak{a}$ は $\mathfrak{g}$ (提案 $4$ の Cor. 4 の VII, §2, no. 1 章) $,s\in \mathfrak{a}$ と $n\in \mathfrak{a}$ における独自のノーマライザーであるため。

#### 命題 5 {#lie-viii-s3-prop-5 .statement tag=00ZU}

P を R の閉じた部分集合とします。

(i) $\mathfrak{h}+\mathfrak{g}^P$ は、$P\cap (-P) =\emptyset$ の場合にのみ解決可能です。その場合は$[\mathfrak{h}+\mathfrak{g}^P,\mathfrak{h}+\mathfrak{g}^P] =\mathfrak{g}^P$です。

(ii) $\mathfrak{h}+\mathfrak{g}^P$ は、$P =-P$ の場合にのみ還元的です。

主張 (i) は提案 2 (iii) から続きます。 $P =-P,\mathfrak{h}+\mathfrak{g}^P$ が還元的である場合 (提案 2 (iv))。 $\mathfrak{a}=\mathfrak{h}+\mathfrak{g}^P$ が還元的であると仮定します。それから

$$
\mathfrak{g}^P= [\mathfrak{h},\mathfrak{g}^P]\subset [\mathfrak{a},\mathfrak{a}]\subset \mathfrak{h}+\mathfrak{g}^P
$$

したがって、$[\mathfrak{a},\mathfrak{a}]$ は形 $\mathfrak{h}'+\mathfrak{g}^P$ と $\mathfrak{h}'\subset \mathfrak{h}$ です。 $[\mathfrak{a},\mathfrak{a}]$ は半単純, $P =-P$ であるため (提案 2 (ii))。

### 2. 理想

#### 命題 6 {#lie-viii-s3-prop-6 .statement tag=00ZV}

$R_1, . . . ,R_p$ を R の既約成分とします。$i= 1, . . . , p$ には、$\mathfrak{g}_i=\mathfrak{h}_{R_i}+\mathfrak{g}^{R_i}$ を代入します。すると、$\mathfrak{g}_1, . . . ,\mathfrak{g}_p$は$\mathfrak{g}$の単純成分になります。

$\mathfrak{g}_i$ は $\mathfrak{g}$ の理想です (提案 1 (ii))。 $\mathfrak{g}$ が $\mathfrak{g}_i$ の直和であるため、$\mathfrak{g}_i$ の積であることは明らかです。 $\mathfrak{a}$ と $\mathfrak{b}$ を $\mathfrak{g}$ の補完的な理想とする。この場合、$\mathfrak{a}$ と $\mathfrak{b}$ は半単純であり、広告 $\mathfrak{h}$ の下で安定しているため、$\mathfrak{a}=\mathfrak{h}_P+\mathfrak{g}^P,\mathfrak{b}=\mathfrak{h}_Q+\mathfrak{g}^Q$ となるような R の部分集合 $P,Q$ が存在します。このとき、$\mathfrak{h}_P,\mathfrak{h}_Q$ は殺人形の$\mathfrak{h}$ で互いに直交補数であるため、P と Q は R の既約成分の和集合です。これは、$\mathfrak{g}_i$ が$\mathfrak{g}$ の最小イデアルであることを証明します。

#### 系 1 {#lie-viii-s3-prop-6-cor-1 .statement tag=01IZ}

$\mathfrak{g}$ は、R が既約である場合にのみ単純です (他の語では、その Dynkin グラフが接続されています)。

これは提案 6 から導かれます。

$k$ のすべての拡大 $k'$ に対して、$k'$-リー代数 $\mathfrak{a}_{(k')}$ が単純である場合、リー代数 $\mathfrak{a}$ は絶対に単純であると言われます。

#### 系 2 {#lie-viii-s3-prop-6-cor-2 .statement tag=00ZW}

分割可能なシンプルなリー代数は非常にシンプルです。

これはコルからの続きです。 1.

$\mathfrak{g}$ が型の場合、$A_l(l\geq 1)$ または $B_l(l\geq 1)$ または $C_l(l\geq 1)$ または $D_l(l\geq 3),\mathfrak{g}$ は、古典的な分割可能な単純なリー代数と言われます。 $\mathfrak{g}$ が型 $E_6, E_7, E_8, F_4$ の場合、または $G_2,\mathfrak{g}$ が例外的に分割可能な単純なリー代数であると言われます。

### 3. ボレル部分代数

#### 命題 7 {#lie-viii-s3-prop-7 .statement tag=00ZX}

$\mathfrak{b}=\mathfrak{h}+\mathfrak{g}^P$ を $\mathfrak{g}$ 含む $\mathfrak{h}$ の部分代数とします。次の条件は同等です。

(i) $\mathfrak{b}$ は、$\mathfrak{g}$ の最大の解ける部分代数です。

(ii) $P = R_+(C)$ となるような R の部屋 C が存在します。

(iii) $P\cap (-P) =\emptyset$ と $P\cup (-P) = R$。

(i) $=\Rightarrow$ (ii): $\mathfrak{b}$ が解けるなら、$P\cap (-P) =\emptyset$。次に、$P\subset R_+(C)$ となるような R の部屋 C が存在します (章 VI, §1, no. 7、提案 22)。この場合、$\mathfrak{h}+\mathfrak{g}^{R_+(C)}$ は、$\mathfrak{g}$ 含む $\mathfrak{b}$ の可解な部分代数であるため、$\mathfrak{b}$ が最大の場合、$\mathfrak{b}$ と等しくなります。

(ii) $=\Rightarrow$ (iii): これは明らかです。

(iii) $=\Rightarrow$ (i): $P\cap (-P) =\emptyset$ と $P\cup (-P) = R$ を仮定します。すると$\mathfrak{b}$は解けます。 $\mathfrak{b}'$ を、$\mathfrak{g}$ 含む $\mathfrak{b}$ の解ける部分代数とします。 $\mathfrak{b}'=\mathfrak{h}+\mathfrak{g}^Q$となるようなRの部分集合Qが存在します。次に、$Q\cap (-Q) =\emptyset$ と $Q\supset P$ なので、Q = P および $\mathfrak{b}'=\mathfrak{b}$ になります。

#### 定義 1 {#lie-viii-s3-def-1 .statement tag=00ZY}

$\mathfrak{g}$ 含む $\mathfrak{h}$ および満たすの部分代数は、提案 7 の条件に相当するものを $(\mathfrak{g},\mathfrak{h})$ のボレル部分代数と呼びます。

$\mathfrak{b}$ が $(\mathfrak{g},\mathfrak{h}')$ のボレル部分代数であるような、$\mathfrak{g}$ の分割カルタン部分代数 $\mathfrak{h}'$ が存在する場合、分割可能代数 $\mathfrak{g}$ の部分代数 $\mathfrak{b}$ は、$\mathfrak{g}$ のボレル部分代数と呼ばれます。

$(\mathfrak{g},\mathfrak{h})$ を分解的簡約リー代数とします。 $\mathfrak{g}=\mathfrak{c}\times \mathfrak{s}$ を $\mathfrak{c}$ と可換、$\mathfrak{s}$ 半単純とします。 形の $\mathfrak{g}$ $\mathfrak{c}\times \mathfrak{b}$ の部分代数は、$\mathfrak{b}$ が $(\mathfrak{s},\mathfrak{h}\cap \mathfrak{s})$ のボレル部分代数であり、 $(\mathfrak{g},\mathfrak{h})$ のボレル部分代数と呼ばれます。

提案 7 の記法により、$\mathfrak{b}$ は、$\mathfrak{h}$ と C (またはC に関連付けられた R の $\mathfrak{h}$ と基底) によって定義される $\mathfrak{g}$ のボレル部分代数であるとも言えます。

#### 注意 {#lie-viii-s3-n3-rem-1 .statement tag=00ZZ}

$R_+(C)$ を R のチャンバー C に関連付ける写像は単射法です (提案 20 のVI, §1, no. 7 章、Cor. 1)。従って、$C \rightarrow \mathfrak{h}+\mathfrak{g}^{R_+(C)}$はRの部屋の集合から$(\mathfrak{g},\mathfrak{h})$のボレル部分代数の集合までの全単射になります。従って、$(\mathfrak{g},\mathfrak{h})$のボレル部分代数の数は、Rのワイル群の位数に等しい（VI, §1, no. 5章、Th.2）。

#### 命題 8 {#lie-viii-s3-prop-8 .statement tag=0100}

$\mathfrak{b}$ を $\mathfrak{g},k'$ の部分代数 $k$ の拡大とします。そして、$\mathfrak{b}$が$(\mathfrak{g},\mathfrak{h})$のボレル部分代数である場合に限り、$\mathfrak{b}\otimes_kk'$は$(\mathfrak{g}\otimes_kk',\mathfrak{h}\otimes_kk')$のボレル部分代数になります。

これは、提案 7 の条件 (iii) から明らかです。

#### 命題 9 {#lie-viii-s3-prop-9 .statement tag=0101}

$\mathfrak{b}$ を R のチャンバー C によって定義される $(\mathfrak{g},\mathfrak{h})$ のボレル部分代数とします。$\mathfrak{n}=\mathfrak{g}^{R_+(C)}=\sum_{\alpha\in R,\alpha >0}\mathfrak{g}^{\alpha}$ とします。 $l=$ を暗くして$\mathfrak{h}$ にしましょう。

(i) $h\in \mathfrak{h}$ と $x\in \mathfrak{n}$ の場合、ad$_{\mathfrak{g}}(h+x)$ の固有多項式は $T^l\prod_{\alpha\in R}(T-\alpha (h))$ です。

(ii) $\mathfrak{b}$ の最大の零イデアルは、$\mathfrak{n}$ および$[\mathfrak{b},\mathfrak{b}]$ に等しい。これは、$\mathfrak{g}$ では $\mathfrak{b}$ の元の集合も無能です。

(iii) B を C に関連付けられた R の基底とします。すべての $\alpha \in B$ について、$X_{\alpha}$ を $\mathfrak{g}^{\alpha}$ の非ゼロ元とします。次に、$(X_{\alpha})_{\alpha\in B}$ 生成するリー代数 $\mathfrak{n}$ となります。 $[\mathfrak{n},\mathfrak{n}] =\sum_{\alpha\in R,\alpha >0,\alpha  \notin B}\mathfrak{g}^{\alpha}$があります。

$\mathfrak{h}^*_{\mathbf{Q}}$ にはそのベクトル空間構造と互換性のある合計位数が存在し、$R_+(C)$ の元が $>0$ になります (第 VI, §1, no. 7 章)。 $h, x$ を (i) と $y\in \mathfrak{g}^{\alpha}$ と同様にします。 次に、$[h+x, y] =\alpha (h)y+z$ が $z\in \sum_{\beta >\alpha}\mathfrak{g}^{\beta}$ になります。 それから、

$\mathfrak{g}$ の適切な基底に関して、ad$_{\mathfrak{g}}(h+x)$ の行列には次の特性があります。

1) 下三角です。

2) 行列の対角エントリーは数 $0 (l$ 倍)、$\alpha \in R$ の$\alpha (h)$。

これは(i)を証明します。また、ad$_{\mathfrak{b}}(h+x)$ の特性多項式が $T\prod_{\alpha\in R_+(C)}^l(T-\alpha (h))$ であることも示しています。前述のことから、

$\mathfrak{g}$の$\mathfrak{b}$の元の集合、および$\mathfrak{b}$の最大ののゼロの理想は、$\mathfrak{n}$に等しい。提案 5 (i) により、$\mathfrak{n}= [\mathfrak{b},\mathfrak{b}]$ が得られます。最後に、主張 (iii) は、§2、提案 4 (ii) および第 4 章から続きます。 VI, §1, no. 6、提案 19。

#### 系 {#lie-viii-s3-n3-cor-1 .statement tag=0102}

$\mathfrak{b}$ を $\mathfrak{g}$ のボレル部分代数とします。

(i) $\mathfrak{b}$ のすべてのカルタン部分代数は、$\mathfrak{g}$ の分裂カルタン部分代数です。

(ii) $\mathfrak{h}_1,\mathfrak{h}_2$ が $\mathfrak{b}$ のカルタン部分代数である場合、$e^{ad_{\mathfrak{g}}x}\mathfrak{h}_1=\mathfrak{h}_2$ となるような $x\in [\mathfrak{b},\mathfrak{b}]$ が存在します。

主張 (i) は、提案 9 (i) および第 2 章に続きます。 VII, §3, no. 3、提案 3. 主張 (ii) は提案 9 (ii) および第 4 章の続きです。 VII, §3, no. 4、木。 3.

#### 命題 10 {#lie-viii-s3-prop-10 .statement tag=0103}

$\mathfrak{b},\mathfrak{b}'$ を $\mathfrak{g}$ のボレル部分代数とします。 $\mathfrak{b}\cap \mathfrak{b}'$に含まれる$\mathfrak{g}$の分裂カルタン部分代数が存在します。

$\mathfrak{h}$ を $\mathfrak{b},\mathfrak{n}= [\mathfrak{b},\mathfrak{b}],\mathfrak{n}'= [\mathfrak{b}',\mathfrak{b}'],\mathfrak{p}=\mathfrak{b}\cap \mathfrak{b}'$ のカルタン部分代数とし、$\mathfrak{b}+\mathfrak{b}'$ を補う $\mathfrak{g}$ の $\mathfrak{s}$ ベクトル部分空間とします。 $\mathfrak{g}$ の Killing 形に対する $\mathfrak{s},\mathfrak{b},\mathfrak{b}'$ の直交補数を $\mathfrak{s}^{\bot},\mathfrak{b}^{\bot},\mathfrak{b}^{'\bot}$ で表します。 $l=$ dim$\mathfrak{h}, n=$ dim$\mathfrak{n}, p=$ dim$\mathfrak{p}$ を置きます。 次に、薄暗くします$\mathfrak{b}=$薄暗くします$\mathfrak{b}'=l+n$、

薄暗い$\mathfrak{s}^{\bot}=$ 薄暗い($\mathfrak{b}+\mathfrak{b}'$) $= 2(l+n)-p$,

など

ディム($\mathfrak{s}^{\bot}\cap \mathfrak{p}$)$\geq$ ディム$\mathfrak{s}^{\bot}+$ ディム$\mathfrak{p}-$ ディム$\mathfrak{g}$ (3)

$$
= 2(l+n)-p+p-(l+ 2n) =l
$$

§2 の提案 1 により、いいえ。 $2,\mathfrak{n}\subset \mathfrak{b}^{\bot},\mathfrak{n}'\subset \mathfrak{b}^{'\bot}$。 $\mathfrak{p}\cap \mathfrak{n}$ の元は、$\mathfrak{g}$ (提案 9 (ii))、および属するから $\mathfrak{b}'$、従って $\mathfrak{n}'$ (提案 9 (ii)) では無能です。従って、$\mathfrak{p}\cap \mathfrak{n}\subset \mathfrak{n}\cap \mathfrak{n}'\subset \mathfrak{b}^{\bot}\cap \mathfrak{b}^{'\bot}$、つまり$\mathfrak{s}^{\bot}\cap \mathfrak{p}\cap \mathfrak{n}= 0$となります。 (3) を考慮すると、$\mathfrak{s}^{\bot}\cap \mathfrak{p}$ は $\mathfrak{b}$ の $\mathfrak{n}$ の補数であることがわかります。 $z$ を $\mathfrak{g}$ の正規の $\mathfrak{h}$ の元とします。 $y+z\in \mathfrak{s}^{\bot}\cap \mathfrak{p}$ となるような $y\in \mathfrak{n}$ が存在します。提案 9 (i) により、ad$_{\mathfrak{g}}(y+z)$ は ad$_{\mathfrak{g}}z$ と同じ特性多項式を持つため、$\mathfrak{g}$ では $x=y+z$ が正則となり、$\mathfrak{b}$ と $\mathfrak{b}'$ ではなおさらが正則となります（VII, §2, no. 2 章、提案 9）。 $\mathfrak{g},\mathfrak{b},\mathfrak{b}'$ は同じ階数を持っているため、$\mathfrak{b}^0(x) =\mathfrak{g}^0(x) ={\mathfrak{b}'}^0(x)$ は同時に$\mathfrak{b}$、$\mathfrak{g}$、$\mathfrak{b}'$ のカルタン部分代数です（VII, §3, no. 3、第 2 章）。最後に、この$\mathfrak{g}$のカルタン部分代数はコルによって分裂です。提案9の。

#### 系 {#lie-viii-s3-n3-cor-2 .statement tag=0104}

群 Aut$_e(\mathfrak{g})$ は、対の $(\mathfrak{t},\mathfrak{b})$ の集合で推移的に動作します。ここで、$\mathfrak{t}$ は $\mathfrak{g}$ の分裂カルタン部分代数であり、$\mathfrak{b}$ は $(\mathfrak{g},\mathfrak{t})$ のボレル部分代数です。

$(\mathfrak{t}_1,\mathfrak{b}_1)$ と $(\mathfrak{t}_2,\mathfrak{b}_2)$ を 2 つの対とします。 $\mathfrak{b}_1\cap \mathfrak{b}_2$ に含まれる $\mathfrak{g}$ の分裂カルタン部分代数 $\mathfrak{t}$ が存在します (提案 10)。コルによって。提案 9 の場合、$\mathfrak{t}_1=\mathfrak{t}_2=\mathfrak{t}$ の場合に帰着します。 S を $(\mathfrak{g},\mathfrak{t})$ の根系とします。 $B_i(i= 1,2)$に$\mathfrak{b}_i$が対応するようなSの基底$B_1,B_2$が存在し、$B_2$に変換$B_1$を加えた$s\in W(S)$が存在します。最後に、$a|\mathfrak{t}=s($§2, no. 2、Cor. となるような$a\in$ Aut$_e(\mathfrak{g})$ が存在します。 Thの。 2)。続いて$a(\mathfrak{t}) =\mathfrak{t}$と$a(\mathfrak{b}_1) =\mathfrak{b}_2$。

### 4. パラボリック部分代数

#### 命題 11 {#lie-viii-s3-prop-11 .statement tag=0105}

$\mathfrak{p}=\mathfrak{h}+\mathfrak{g}^P$ を $\mathfrak{g}$ 含む $\mathfrak{h}$ の部分代数とします。次の条件は同等です。

(i) $\mathfrak{p}$ 含むボレル部分代数の $(\mathfrak{g},\mathfrak{h})$;

(ii) $P\supset R_+(C)$ となるような R のチャンバー C が存在します。

(iii) P is parabolic, in other words (Chap. VI, §1, no. 7, Def. 4), $P\cup (-P) =$ R.

条件 (i) と (ii) は提案 7 により同等です。 条件 (ii) と (iii) は提案 7 により同等です。 VI, §1, no. 7、提案 20。

#### 定義 2 {#lie-viii-s3-def-2 .statement tag=0106}

$\mathfrak{g}$ 含む $\mathfrak{h}$ および満たすの部分代数は、提案 11 の条件に相当し、$(\mathfrak{g},\mathfrak{h})$ の放物線部分代数と呼ばれます。 $\mathfrak{g}$ の放物線部分代数は、$(\mathfrak{g},\mathfrak{h}')$ の放物線部分代数であり、$\mathfrak{h}'$ は $\mathfrak{g}$ の分裂カルタン部分代数です。

この定義拡大するは、$(\mathfrak{g},\mathfrak{h})$ が分解的簡約リー代数の場合にすぐに適用されます。

#### 注意 {#lie-viii-s3-n4-rem-1 .statement tag=0107}

B を R の基底、$\mathfrak{b}$ 対応するボレル部分代数とします。 $\Sigma \subset B$ の場合、係数 $\leq 0$ を含む $\Sigma$ の元の線形結合である根の $Q_{\Sigma}$ 集合によって示されます。 $\mathfrak{p}(\Sigma ) = R_+(B)\cup Q_{\Sigma}$と$\mathfrak{p}_{\Sigma}=\mathfrak{h}\oplus \mathfrak{g}^{P(\Sigma)}$を入れます。章著。 VI, §1, no. 7、補題 3、提案$20,\mathfrak{p}_{\Sigma}$ は放物線部分代数含む $\mathfrak{b}$ であり、$\mathfrak{g}$ 含む $\mathfrak{b}$ のすべての放物線部分代数はこのようにして得られます。

#### 補題 3 {#lie-viii-s3-lem-3 .statement tag=0108}

V を有限次元の実ベクトル空間、S を S の放物線部分集合の集合である $V^*,\mathscr{P}$ の根系とします。 $\mathscr{H}$ を $\alpha \in S$ の Ker $\alpha$ の集合とし、$\mathscr{F}$ を $\mathscr{H}$ に対する V のファセットの集合とする (V, §1, no. 2 章、定義 1)。

$P\in \mathscr{P}$ の場合、F(P) を $v\in V$ の集合とし、すべての $\alpha \in P$ に対して $\alpha (v)\geq 0$ とします。 $F\in \mathscr{F}$ の場合、P(F) をすべての $v\in F$ に対して $\alpha (v)\geq 0$ となるように、$\alpha \in R$ の集合とします。

すると、$F \rightarrow P(F)$ は $\mathscr{F}$ から $\mathscr{P}$ までの全単射になります。すべての $F\in \mathscr{F}$ に対して、F(P(F)) は F の閉包です。

a) $P\in \mathscr{P}$ とします。 There exists a chamber C of S and a subset $\Sigma$ of the basis B(C) such that $P = S_+(C)\cup Q$ where Q is the set of linear combinations of elements of $\Sigma$ with non-positive integer coefficients (Chap. VI, §1, no. 7, Prop. 20). 置く

$$
B(C) =\{\alpha_1, . . . , \alpha_l\}, \Sigma =\{\alpha_1, . . . , \alpha_m\}
$$

$v\in V$ の場合、次の同値があります。

$\alpha (v)\geq 0$ 全員$\alpha \in P$

$$
\Leftarrow \Rightarrow \alpha_1(v)\geq 0, . . . \alpha_l(v)\geq 0, \alpha_1(v)\leq 0, . . . , \alpha_m(v)\leq 0
$$

$$
\Leftarrow \Rightarrow \alpha_1(v) =\cdots =\alpha_m(v) = 0, \alpha_{m+1}(v)\geq 0, . . . , \alpha_l(v)\geq 0
$$

したがって、F(P) は集合の閉包です

$$
\{v\in V|\alpha_1(v) =\cdots =\alpha_m(v) = 0, \alpha_{m+1}(v)>0, . . . , \alpha_l(v)>0\}
$$

集合は、Sのすべての元が$\alpha_1, . . . , \alpha_l$の線形結合であり、係数はすべて$\geq 0$かすべて$\leq 0$のいずれかであるため、$\mathscr{H}$に対するファセットFです。また、$\beta =u_1\alpha_1+\cdots +u_l\alpha_l\in S$の場合、

$$
\beta \in P(F)\Leftarrow \Rightarrow u_{m+1}\geq 0, . . . , u_l\geq 0
$$

$\Leftarrow \Rightarrow \beta \in S_+(C)$ または $(-\beta \in S_+(C)$ および $u_{m+1}=. . .=u_l= 0)$

$$
\Leftarrow \Rightarrow \beta \in S_+(C)\cup Q = P
$$

したがって、P(F) = P。

b) $F\in \mathscr{F}$ とします。 $P(F)\in \mathscr{P}$であることは明らかです。 一方、F は $\mathscr{H}$ に対する部屋の閉包に含まれており (V, §1, no. 3 式 (6))、この部屋の壁の集合に対するファセットでもある (V, §1, no. 4 章、提案 9)。 従って、$\overline{F}$ はすべての $\alpha \in T\}$ に対して形 $\{v\in V|\alpha (v)\geq 0$ であり、T は S の部分集合であり、明らかに P(F) に等しいとみなすことができます。 従って、$\overline{F}= F(P(F))$。 Q.E.D.

$P\in \mathscr{P}$ の場合、P = P(F) となるファセット F は P に関連付けられていると言われます。それをF(P)で表します。これらの規則を、$(\mathfrak{g},\mathfrak{h})$ が分裂還元的である場合に拡大する適用します。

#### 命題 12 {#lie-viii-s3-prop-12 .statement tag=0109}

$\mathscr{H}$ を、R の $\mathfrak{h}_{\mathbf{R}}$ の超平面の集合 、核の根のからなるとします。 $\mathscr{F}$ を、$\mathscr{H}$ に対する $\mathfrak{h}_{\mathbf{R}}$ のファセットの集合とします。 $\mathscr{S}$を$(\mathfrak{g},\mathfrak{h})$の放物線部分代数の集合とします。すべての $\mathfrak{p}=\mathfrak{h}+\mathfrak{g}^P\in \mathscr{S}$ について、$F(\mathfrak{p})$ を P に関連付けられたファセットとします。すると、$\mathfrak{p} \rightarrow F(\mathfrak{p})$ は $\mathscr{S}$ から $\mathscr{F}$ までの全単射になります。 $\mathfrak{p}_1,\mathfrak{p}_2\in \mathscr{P}$の場合、

$$
\mathfrak{p}_1\supset \mathfrak{p}_2\Leftarrow \Rightarrow F(\mathfrak{p}_1)\subset \overline{F(\mathfrak{p}_2)}
$$

これは補題 3 の直後に続きます。

#### 例 {#lie-viii-s3-n4-exa-1 .statement tag=010A}

$(\mathfrak{g},\mathfrak{h})$ 含むボレル代数 $\mathfrak{b}$ の放物線部分代数へのファセット対応するは、$\mathfrak{b}$ (上記の cf. 注意) に関連付けられたチャンバーの閉鎖に含まれるファセットです。

#### 命題 13 {#lie-viii-s3-prop-13 .statement tag=010B}

$\mathfrak{p}=\mathfrak{h}+\mathfrak{g}^P$ を $(\mathfrak{g},\mathfrak{h})$ の放物線部分代数、$\alpha \in P$ の Q 集合を$-\alpha  \notin P$、$\mathfrak{s}=\mathfrak{h}+\mathfrak{g}^{P\cap(-P)}$ とする。そして、$\mathfrak{p}=\mathfrak{s}\oplus \mathfrak{g}^Q,\mathfrak{s}$は$\mathfrak{g}$で還元的であり、$\mathfrak{g}^Q$は$\mathfrak{p}$の零ポテンシャル最大のと$\mathfrak{p}$の零ポテント根基です。 $\mathfrak{p}$の中心は零です。

提案によると、$2,\mathfrak{s}$ は $\mathfrak{g}$ で還元的であり、$\mathfrak{g}^Q$ は $\mathfrak{p}$ の零イデアルです。 $\mathfrak{n}$ が $\mathfrak{p},\mathfrak{g}^Q\subset \mathfrak{n}\subset \mathfrak{h}+\mathfrak{g}^Q$ の最大のである場合 (提案 2 (i))。 $x\in \mathfrak{n}\cap \mathfrak{h}$ の場合、ad$_{\mathfrak{p}}x$ はゼロポテントなので、すべての $\alpha \in P$ に対して $\alpha (x) = 0$、従って $x= 0$ になります。これは $\mathfrak{n}=\mathfrak{g}^Q$ であることを証明します。 $[\mathfrak{h},\mathfrak{g}^Q] =\mathfrak{g}^Q$ 以降、$\mathfrak{p}$ 含む $\mathfrak{g}^Q$ のゼロポテント根基は、$\mathfrak{g}^Q$ に等しくなります。 $z=h+\sum_{\alpha\in P}u_{\alpha}$ ($h\in \mathfrak{h}, u_{\alpha}\in \mathfrak{g}^{\alpha}$) を

元/中心/$\mathfrak{p}$。すべての $h'\in \mathfrak{h}, 0 = [h', z] =\sum\alpha (h')u_{\alpha}$ については、すべての $\alpha \in P$ について $u_{\alpha}= 0$ となります。すべての $\beta \in P$ に対して $[h,\mathfrak{g}^{\beta}] = 0$ となるため、$h= 0$ になります。

### 5. 非分割ケース

#### 命題 14 {#lie-viii-s3-prop-14 .statement tag=010C}

$k'$ を $k$ と $\mathfrak{g}'=\mathfrak{g}\otimes_kk'$ の拡大とします。 $\mathfrak{m}$を$\mathfrak{g}$と$\mathfrak{m}'=\mathfrak{m}\otimes_kk'$の部分代数とします。 $\mathfrak{m}'$ が放物線 (ボレル) の場合、$\mathfrak{g}',\mathfrak{m}$ の部分代数は放物線 (ボレル) $\mathfrak{g}$ の部分代数です。

提案 8 と 11 により、$\mathfrak{g}$ の $\mathfrak{m}$ 含む分裂カルタン部分代数を証明するのに十分です。 $\mathfrak{b}$を$\mathfrak{g}$のボレル部分代数とします。すると、$\mathfrak{b}'=\mathfrak{b}\otimes_kk'$ は $\mathfrak{g}'$ のボレル部分代数なので、$\mathfrak{g}'$ の $\mathfrak{m}'\cap \mathfrak{b}'$ 含むカルタン部分代数になります (提案 10)。 $\mathfrak{t}$を$\mathfrak{m}\cap \mathfrak{b}$のカルタン部分代数とします。すると、$\mathfrak{t}\otimes_kk'$ は $\mathfrak{m}'\cap \mathfrak{b}'$ のカルタン部分代数となり、従って $\mathfrak{g}'$ になります (VII, §3, no. 3 章、提案 3)。従って、$\mathfrak{t}$は$\mathfrak{g}$のカルタン部分代数で、$\mathfrak{b}$に含まれるので分裂となります。

#### 定義 3 {#lie-viii-s3-def-3 .statement tag=010D}

$\mathfrak{a}$ を $k$ の半単純 (またはより一般的に還元的) リー代数および $\overline{k}$ 代数閉包とします。 $\mathfrak{a}$ の部分代数 $\mathfrak{m}$ は、$\mathfrak{m}\otimes_k\overline{k}$ が $\mathfrak{a}\otimes_k\overline{k}$ の放物線 (それぞれ Borel ) 部分代数である場合、放物線 (それぞれ Borel ) であると言われます。

$\mathfrak{a}$ が分割可能である場合、提案 14 は、この定義が定義 2 (それぞれ定義 1) と同等であることを示します。

#### 命題 15 {#lie-viii-s3-prop-15 .statement tag=010E}

$\mathfrak{a}$ を $k$ の還元型リー代数、$k'$ 拡大、および $\mathfrak{a}$ の $\mathfrak{m}$ 部分代数とします。このとき、$\mathfrak{m}\otimes_kk'$ が $\mathfrak{a}\otimes_kk'$ の放物線 (それぞれ Borel ) 部分代数である場合に限り、 $\mathfrak{m}$ は $\mathfrak{a}$ の放物線 (それぞれ Borel ) 部分代数になります。

これは提案 14 の直後に続きます。

### 練習問題 {#lie-viii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
