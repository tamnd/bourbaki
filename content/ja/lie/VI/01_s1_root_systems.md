---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VI
chapter_title: ROOT SYSTEMS
section: 1
section_title: Root systems
lang: ja
source: lie-iv-vi
pdf_pages: 0168-0198, 0248-0253
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF A ROOT SYSTEM
      page: 0
      pdf_page: 168
    - "no": 2
      title: DIRECT SUM OF ROOT SYSTEMS
      page: 0
      pdf_page: 172
    - "no": 3
      title: RELATION BETWEEN TWO ROOTS
      page: 0
      pdf_page: 173
    - "no": 4
      title: REDUCED ROOT SYSTEMS
      page: 0
      pdf_page: 177
    - "no": 5
      title: CHAMBERS AND BASES OF ROOT SYSTEMS
      page: 0
      pdf_page: 178
    - "no": 6
      title: POSITIVE ROOTS
      page: 0
      pdf_page: 181
    - "no": 7
      title: CLOSED SETS OF ROOTS
      page: 0
      pdf_page: 186
    - "no": 8
      title: HIGHEST ROOT
      page: 0
      pdf_page: 191
    - "no": 9
      title: WEIGHTS, RADICAL WEIGHTS
      page: 0
      pdf_page: 192
    - "no": 10
      title: FUNDAMENTAL WEIGHTS, DOMINANT WEIGHTS
      page: 0
      pdf_page: 193
    - "no": 11
      title: COXETER TRANSFORMATION
      page: 0
      pdf_page: 195
    - "no": 12
      title: CANONICAL BILINEAR FORM
      page: 0
      pdf_page: 197
statements: 79
exercises: 24
content_sha256: 9703f3ba8670e27ba7e0a7c2773863b74e02589f3f206b557320ed450ce93d40
translated_from: content/en/lie/VI/01_s1_root_systems.md
translation_method: google
source_content_sha256: e928a5393f8d44d4601610a514808a5db0798a4a4348f1d6a9e230dc8b3576c6
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 0a9de914c64f407700664a0586df452c607a1a318c3c93037f6e4d36da4ffd40
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。 根系

この段落では、$k$は標数0の体を指します。 no. 3以降は$k = \mathbf{R}$とします。

### 1. 定義/根系

#### 補題 1 {#lie-vi-s1-lem-1 .statement tag=0AU4}

$V$ を $V$ 生成する $V$ の $k$、$R$ 有限部分集合を超えるベクトル空間とします。 $\alpha \neq 0$ などの $\alpha \in R$ については、$s(\alpha) = -\alpha$ や $s(R) = R$ などの $V$ の反映 $s$ が最大 1 つ存在します。

$G$ を $V$ の自己同型のうち群とし、$R$ を安定させます。 $R$ 生成する $V$ なので、$G$ は $R$ の対称群の部分群と同型であり、したがって有限です。 $s, s'$ を $V$ の反映として、$s(\alpha) = s'(\alpha) = -\alpha$、$s(R) = R$、$s'(R) = R$ とします。次に、$t = ss'$ 属するから $G$ となり、有限である位数 $m$ となります。一方、

$$
t(\alpha) = \alpha \quad \text{and} \quad t(x) \equiv x \mod. k\alpha \quad \text{for all } x \in V.
$$

したがって、$V$ には次のような線型形式 $f$ が存在します。

$$
t(x) = x + f(x)\alpha \quad \text{for all } x \in V
$$

そして$f(\alpha) = 0$。 $n$の帰納法までに、次のようになります。

$$
t^n(x) = x + nf(x)\alpha \text{ for all } x \in V.
$$

$n$ が $m$ と等しいとすると、すべての $x \in V$ に対して $mf(x) = 0$ となるため、$f = 0$、$t = 1$、$s = s'$ となります。

#### 定義 1 {#lie-vi-s1-def-1 .statement tag=0AU5}

$V$ を $k$ のベクトル空間とし、$V$ の $R$ 部分集合とします。次に、次の条件が満たされる場合、$R$ は $V$ で根系であると言われます。

(RS_I) $R$ は有限ですが、含む 0、および生成する $V$ は有限ではありません。
(RS_{II}) すべての $\alpha \in R$ に対して、$\langle \alpha, \alpha^\vee \rangle = 2$ と反射 $s_{\alpha, \alpha^\vee}$ (cf. 章 V, § 2) が離れるように、$V$ の双対 $V^*$ の元 $\alpha^\vee$ が存在します。 $R$安定。

(RS_{\text{III}}) $\alpha \in \mathbf{R}$、$\alpha^{\sim}(R) \subseteq \mathbf{Z}$ のすべて。

補題 1 により、反射 $s_{\alpha,\alpha^{\sim}}$ (したがって、線型形式 $\alpha^{\sim}$) は $\alpha$ によって一意に決定されるため、(RS_{\text{III}}) は意味を成します。 $s_{\alpha,\alpha^{\sim}} = s_{\alpha}$を入れます。次に、すべての $x \in V$ に対して $s_{\alpha}(x) = x - \langle \alpha^{\sim}, x \rangle \alpha$ です。

R の元は (系のうちの) 根と呼ばれます。 Vの次元は、系の階数と呼ばれます。

R を安定に残す V の自己同型を R の自己同型と呼びます。それらの形有限群は A(R) で表されます。 $s_{\alpha}$ によって生成される A(R) の部分群は R のワイル群と呼ばれ、W(R) または単に W で表されます。

#### 注意 1 {#lie-vi-s1-n1-rem-1 .statement tag=0AU6}

$k'$を$k$の拡大とします。 同一視する V は正規的に $V \otimes k'$ の部分集合と$V^*$ と $V^* \otimes k' = (V \otimes k')^*$ の部分集合です。すると、Rは$V \otimes k'$の根系で、$\alpha^{\sim}$は前にと同じになります。

#### 補題 2 {#lie-vi-s1-lem-2 .statement tag=0AU7}

R を V で根系とします。 $(x|y)$ を V 上で対称な双線形形式とし、W(R) のもとで非縮退かつ不変とする。この形によって$V^*$と同一視するV。 $\alpha \in R$ の場合、$\alpha$ は非等方性であり、

$$
\alpha^{\sim} = \frac{2\alpha}{(\alpha|\alpha)}.
$$

これは第 2 章の公式 (4) に続きます。 V, § 2, no. 3。

#### 命題 1 {#lie-vi-s1-prop-1 .statement tag=0AU8}

$V_Q$ (それぞれ $V_Q^*$) を、$\alpha$ (それぞれ $\alpha^{\sim}$) によって生成された V (それぞれ $V^*$) の Q ベクトル部分空間とします。次に、$V_Q$ (それぞれ $V_Q^*$) は、V (それぞれ $V^*$) 上の Q 構造です (代数、第 II, § 8, no. 1)。 $V \times V^*$ の正規の双線形形式の制限から $V_Q \times V_Q^*$ は、空間 $V_Q, V_Q^*$ のそれぞれの識別を、互いの双対で示します。 集合 R は $V_Q$ の根系です。

If $k = \mathbf{R}$, there exists a scalar product on V invariant under W(R) (Integration, Chap. VII, § 3, no. 1, Prop. 1); 補題 2 は、$\alpha^{\sim}$ 生成する $V^*$ を示します。 注意 1 までに、$k = \mathbf{Q}$ であれば、再び $\alpha^{\sim}$ 生成する $V^*$ になります。 次に、一般的なケースに進みます。 E = $V_Q$ と置きます。 (RS_{\text{III}}) により、各 $\alpha^{\sim}$ 写像 E から $\mathbf{Q}$ なので、$E^*$ の定義する元 $\tilde{\alpha}$ となります。 EのRが根系であるのは明らかであり、$E^*$の元対応するから$\alpha$が$\tilde{\alpha}$であるのです。 上で述べたことにより、$\tilde{\alpha}$ 生成するベクトル空間 $E^*$ となります。 標準準同型 $i : E \otimes_Q k \to V$ とその転置 $^t i : V^* \to E^* \otimes_Q k$ を考えてみましょう。 R 生成する V なので、$^t i$ は単射です。しかし、$^t i$ 含むの像は $\tilde{\alpha}$ なので、$^t i$ は全射です。 これから結論する、最終的に i と $^t i$ は同型になります。 したがって、$E \otimes k$ では同一視する V、$E^* \otimes k$ では$V^*$、$\tilde{\alpha}$ では$\alpha^{\sim}$、$E^*$ では$V_Q^*$ が可能です。 したがって、$V_Q$ (それぞれ $V_Q^*$) は、V (それぞれ $V^*$) 上の Q 構造です。 $V \times V^*$ の正規双線形形式の制限から $V_Q \times V_Q^*$ は、$E \times E^*$ の正規双線形形式と識別できるため、命題となります。

#### 注意 2 {#lie-vi-s1-n1-rem-2 .statement tag=0AU9}

命題 1 簡約する根系の考察から$k = \mathbf{Q}$ まで。 注意 1 簡約するは、実際のベクトル空間 $V_{\mathbf{R}} = V_{\mathbf{Q}} \otimes_{\mathbf{Q}} \mathbf{R}$ の根系の研究に続きます。これらの異なる系に関連付けられた Weyl 群は標準的に識別されます。

#### 注意 3 {#lie-vi-s1-n1-rem-3 .statement tag=0AUA}

Since the $\alpha \tilde{}$ generate $V^*$, the group $W(R)$, considered as a subgroup of $\mathbf{GL}(V_{\mathbf{R}})$, is essential (Chap. V, § 3, no. 7). さらに、Cor. Thの。第1章V, § 3, no. 2 は、所属から $W(R)$ までの反射が $s_{\alpha}$ だけであることを示しています。

#### 命題 2 {#lie-vi-s1-prop-2 .statement tag=0AUB}

*$\alpha \tilde{}$ 形根系は $V^*$ に、$\alpha \tilde{} = \alpha$ はすべての $\alpha \in R$ に含まれます。*

提案 1 による $\alpha \tilde{}$ 満たす (RS_I)。$s_{\alpha, \alpha \tilde{}}$ はベクトル空間 $V$ の自己同型に部分集合 $R$ が装備されているため、${}^t(s_{\alpha, \alpha \tilde{}})^{-1}$ は、集合 $R \tilde{}$ を残します。 $\alpha \tilde{}$安定。しかし、${}^t(s_{\alpha, \alpha \tilde{}})^{-1} = s_{\alpha \tilde{}, \alpha}$ は、$R \tilde{}$ が (RS_{II}) を満たし、$\alpha \tilde{} = \alpha$ を満たしていることを証明します。最後に、すべての $\alpha \tilde{} \in R \tilde{}$ と $\beta \in R$ に対して $\langle \alpha \tilde{}, \beta \rangle \in \mathbf{Z}$ なので、$R \tilde{}$ は満たされます (RS_{III})。

集合 $R \tilde{}$ は、* $R$ の * 逆数根系と呼ばれます。 写像 $\alpha \mapsto \alpha \tilde{}$ は、$R$ から $R \tilde{}$ までの全単射であり、$R$ *から* $R \tilde{}$ までの *標準全単射と呼ばれます。 $\alpha, \beta$ が $\alpha + \beta \in R$ となるような $R$ の元である場合、一般に $(\alpha + \beta) \tilde{} \neq \alpha \tilde{} + \beta \tilde{}$ になることに注意してください。

$s_{\alpha}(\alpha) = -\alpha$ から、公理 (RS_{II}) は $-R = R$ を示します。明らかに $(-\alpha) \tilde{} = -\alpha \tilde{}$ と $-1 \in A(R)$ (ただし、$-1 \in W(R)$ が常に真実であるとは限りません)。

等式 ${}^t(s_{\alpha, \alpha \tilde{}})^{-1} = s_{\alpha \tilde{}, \alpha}$ は、写像 $u \mapsto {}^t u^{-1}$ が群 $W(R)$ から群 $W(R \tilde{})$ までの同型であることを示します。私たちはこの同型によって、この 2 人群を同一視する結び付けます。他の語では、$W(R)$が$V$と$V^*$の両方で機能していると考えられます。 $A(R)$も同様です。

#### 命題 3 {#lie-vi-s1-prop-3 .statement tag=0AUC}

*$x, y \in V$の場合は*を入力してください
$$
(x|y) = \sum_{\alpha \in R} \langle \alpha \tilde{}, x \rangle \langle \alpha \tilde{}, y \rangle.
$$
*その後* $(x|y)$ * は* $V$ 上で非縮退対称双線形形式 、* $A(R)$ の下で*不変です。 *のため* $x, y \in V_{\mathbf{Q}}$ *私たちは* $(x|y) \in \mathbf{Q}$を持っています。 *正規拡大 of* $(x|y)$ *to*
$$
V_{\mathbf{R}} = V_{\mathbf{Q}} \otimes_{\mathbf{Q}} \mathbf{R}
$$
*非退化かつ陽性*です。

$(x|y)$ が $V$ 上で対称な双線形形式であることは明らかです。 $g \in A(R)$の場合、
$$
(g(x)|g(y)) = \sum_{\alpha \in R} \langle {}^t g(\alpha \tilde{}), x \rangle \langle {}^t g(\alpha \tilde{}), y \rangle = (x|y)
$$
${}^t g)(R \tilde{}) = R \tilde{}$から。 $x, y \in V_{\mathbf{Q}}$の場合、(RS_{III})により$(x|y) \in \mathbf{Q}$になります。提案 1 により、$z \in V_{\mathbf{R}}$ の場合は $(z|z) = \sum_{\alpha \in R} \langle \alpha \tilde{}, z \rangle^2 \geq 0$、$z \neq 0$ の場合は $(z|z) > 0$ となるため、$(x|y)$ から $V_{\mathbf{R}}$ までの正規の拡大は正で非縮退です。したがって、$(x|y)$ から $V_{\mathbf{Q}}$ の制限は非縮退であり、したがって、$V$ の形 $(x|y)$ は非縮退です。

#### 命題 4 {#lie-vi-s1-prop-4 .statement tag=0AUD}

(i) *$X$ を $\mathbf{R}$ の部分集合とし、$V_X$ を $X$ によって生成された $V$ のベクトル部分空間とし、$V'_X$ をベクトル部分空間とする$V^*$ は $\alpha^-$ によって生成され、$\alpha \in X$ です。すると、$V$ は $V_X$ の直和であり、$V'_X$ の直交補数です。 $V^*$ は $V'_X$ の直和であり、$V_X$ の直交補数であり、$V'_X$ は $V_X$ の双対と同一視されます。

(ii) $R \cap V_X$ は $V_X$ の根系であり、$R \cap V_X$ からその逆数根系までの正準全単射は、写像 $\alpha \mapsto \alpha^-$ から $R \cap V_X$ の制限と同一視されます。

*注意 2* により、$k = \mathbf{R}$ と仮定できます。提案 3 の対称双線形形式により、同一視する $V$ と $V^*$ が結合され、すべての $\alpha \in R$ (補題 2) に対して $\alpha^- = \frac{2\alpha}{(\alpha|\alpha)}$ が得られます。 $V$ のすべてのベクトル部分空間は非等方性であり、命題は透明になりました。

#### 系 {#lie-vi-s1-n1-cor-1 .statement tag=0AUE}

*$V_1$ を $V$ のベクトル部分空間とし、$V_2$ を $R \cap V_1$ によって生成されたベクトル部分空間とします。すると、$R \cap V_1$は$V_2$の根系になります。

これは、$X = R \cap V_1$ に適用される (ii) から続きます。

$\alpha, \beta \in R$には、
$$
\langle \alpha, \beta^- \rangle = n(\alpha, \beta).
$$
(1)

それから
$$
n(\alpha, \alpha) = 2
$$
(2)
$$
n(-\alpha, \beta) = n(\alpha, -\beta) = -n(\alpha, \beta).
$$
(3)

(RSIII) により、
$$
n(\alpha, \beta) \in \mathbf{Z}.
$$
(4)

$n(\alpha, \beta)$中定義までに、
$$
s_\beta(\alpha) = \alpha - n(\alpha, \beta)\beta.
$$
(5)

公式 (1) と提案 2 は、次のことを意味します。
$$
n(\alpha, \beta) = n(\beta^-, \alpha^-).
$$
(6)

$(x|y)$ を $V$ 上で対称な双線形形式とし、$W(R)$ の下で非縮退かつ不変とする (提案 3)。 補題 2までに、
$$
n(\alpha, \beta) = \frac{2(\alpha|\beta)}{(\beta|\beta)}.
$$
(7)

したがって、
$$
n(\alpha, \beta) = 0 \iff n(\beta, \alpha) = 0 \iff (\alpha|\beta) = 0 \iff s_\alpha \text{ and } s_\beta \text{ commute.}
$$
(8)

$(\alpha|\beta) \neq 0$ の場合、
$$
\frac{n(\beta, \alpha)}{n(\alpha, \beta)} = \frac{(\beta|\beta)}{(\alpha|\alpha)}.
$$
(9)

### 2. 直和/根系

V を $k$ の上のベクトル空間とします。つまり、ベクトル空間の家族 $(V_i)_{1 \leq i \leq r}$ の直和です。 同一視する $V^*$ と $V_i^*$ の直和 。すべての $i$ について、$R_i$ を $V_i$ の根系とします。すると、$R = \bigcup_i R_i$ は V の根系となり、その逆数系は $R^- = \bigcup_i R_i^-$ になります。 R から $R^-$ 拡大するまでの正規全単射、すべての $i$、$R_i$ から $R_i^-$ までの正規全単射。 集合 R は、根系* $R_i$ の *直和と呼ばれます。 $\alpha \in R_i$ にしましょう。 $j \neq i$、$\alpha^-$ 含む $V_j$ の核の場合、$V_j$ の ID は $s_\alpha$ 誘導するになります。一方、$k\alpha \subseteq V_i$ なので、$s_\alpha$ は $V_i$ を安定させます。これらの注意は、$W(R)$ が *$\prod_{i=1}^r W(R_i)$ と識別できる*ことを示しています。

根系 R は、$R \neq \varnothing$ であり、R が空ではない 2 つの根系の直和ではない場合、*既約*であると言われます。

#### 命題 5 {#lie-vi-s1-prop-5 .statement tag=0AUF}

*Vをk以上のベクトル空間、つまりベクトル空間* $V_1, \ldots, V_r$の直和とします。 ※RをVの根系とします。 * $R_i = R \cap V_i$ を置きます。 *次の 3 つの条件は同等です*:

(i) *$V_i$ *$W(R)$ の下では安定しています。
(ii) $R \subseteq V_1 \cup V_2 \cup \cdots \cup V_r$;
(iii) *すべて* $i$、$R_i$ *は$V_i$の根系、*そしてRは* $R_i$の直和です。
(iii) $\Longrightarrow$ (i): これは、この数の冒頭で述べたことに続きます。

(i) $\Longrightarrow$ (ii): $V_i$ が $W(R)$ の下で安定していると仮定します。 $\alpha \in R$ とし、H を $\alpha^-$ の核とします。第 3 章の提案 3 による。 V, § 2, no. 2、それぞれの $V_i$ は、H の部分空間の和と $k\alpha$ の部分空間です。したがって、$V_i$ 含む $k\alpha$ の 1 つ、つまり $\alpha \in V_1 \cup V_2 \cup \cdots \cup V_r$ になります。

(ii) $\Longrightarrow$ (iii): 条件 (ii) が満たされる場合、すべての $i$ に対して $R_i$ 生成する $V_i$ となるため、$V_i$ の $R_i$ は根系になります (提案 4)。 Rが$R_i$の直和であることは明らかです。

#### 系 {#lie-vi-s1-n2-cor-1 .statement tag=0AUG}

※RをVの根系とします。 次の条件は同等*です。
(i) *R は既約です*;
(ii) *$W(R)$*-モジュール* V *は単純です*。
(iii) *$W(R)$*-モジュール* V *は非常に単純です*。
(ii) $\Longleftrightarrow$ (i): これは、提案 5 およびマシュケの定理 (V 章、付録、提案 2) から導き出されます。
(iii) $\Longleftrightarrow$ (ii): これは第 2 章の提案 1 に続きます。 V, § 2, no. 1。

#### 命題 6 {#lie-vi-s1-prop-6 .statement tag=0AUH}

*すべての根系* R *in* V * は、添字集合* の全単射までの一意な、族* $(R_i)_{i \in I}$ *既約根系の直和です。

The existence of the $R_i$ is proved by induction on Card R: if R is non-empty and not irreducible, R is the direct sum of two root systems $R', R''$ such that Card $R' <$ Card $R$, Card $R'' <$ Card $R$, and the induction hypothesis applies to $R'$ and $R''$. 一意性を証明するには、$R$が$R'$と$R''$の直和である場合、すべての$R_i$は必ず$R'$または$R''$のいずれかに含まれることを証明すれば十分です。 $V', V'', V'_i, V''_i$ を、$R', R'', R' \cap R_i, R'' \cap R_i$ によって生成された $V$ のベクトル部分空間とします。 和 $V' + V''$ は直接ですので、和 $V'_i + V''_i$ は直接です。 $R_i \subseteq R' \cup R''$ なので、$R_i$ は根系 $R' \cap R_i$ と $R'' \cap R_i$ の直和です。したがって、$R' \cap R_i = \varnothing$ または $R'' \cap R_i = \varnothing$ となり、主張が証明されます。

$R_i$ は、$R$ の *既約成分* と呼ばれます。ゼロ以外のスカラー $\lambda_i$ の場合、$\lambda_i R_i$ の和集合は $V$ の根系であり、その逆数系は $\lambda_i^{-1} R_i$ の和集合であり、そのワイル群は $W(R)$ です。

#### 命題 7 {#lie-vi-s1-prop-7 .statement tag=0AUI}

*$R$ を $V$ の根系、$(R_i)$ 既約成分の族、$V_i$ $R_i$ によって生成された $V$ のベクトル部分空間、$B$ を提案 3 で定義した $V$ 上の不変対称双線形形式、および$B'$ $W(R)$ の下での不変式である $V$ 上の対称双線形形式。 この場合、$V_i$ は$B'$ に関してペアごとに直交し、すべての$i$、$B$ および$B'$ ～ $V_i$ の制限は比例します。*

$v_i \in V_i, v_j \in V_j, i \neq j$ の場合、および $w \in W(R_j)$ の場合、
$$
B'(v_i, w(v_j)) = B'(v_i, v_j),
$$
これは、$w(v_j) - v_j$が$B'$に関して$v_i$と直交していることを示しています。 $V_j$は$W(R_j)$に対して既約なので、$w(v_j) - v_j$によって生成され、したがって$V_i$と直交します。

$B$ と $B'$ のそれぞれの $V_i$ に対する制限が比例するという事実は、第 3 章の提案 1 から導き出されます。 V, § 2, no. 1。

#### 注意 {#lie-vi-s1-n2-rem-1 .statement tag=0AUJ}

選ぶ $W(R)$ の下での不変式である $V_R$ 上のスカラー 積。その場合、根の*長さ*と、2つの根の間の*角度*について話すことが可能になります。提案 7 は、この角度が、$R$ の *同じ*既約成分に対する属するである場合、2 つの根の長さの比と同様に、この角度がスカラー 積の選択から独立していることを示しています。

### 3. 2 つの間の関係根

*これからは $k = \mathbf{R}$ と仮定します*。 (no. 1 の *注意 2* に示されている方法を使用して、定義を拡張して一般的なケースに結果を適用する作業は読者に任せます。)

*以下を通じて、$R$はベクトル空間$V$の根系を表します。そして、$V$ には、$W(R)$、cf. 提案 3 の下でスカラー 積 $(x, y) \mapsto (x|y)$ 不変式が装備されています。

$\alpha, \beta \in R$ にしましょう。 no. 1 の公式 (7) までに、
$$
n(\alpha, \beta)n(\beta, \alpha) = 4 \cos^2 (\widehat{\alpha, \beta}) \leq 4.
$$

したがって、整数 $n(\alpha, \beta)n(\beta, \alpha)$ は、値 0、1、2、3、4 のいずれかをとらなければなりません。 V, § 2, no. 5、コル。提案6の、および第4章のページの脚注の。 V, § 4, no. 8 より、可能性は次の交換すること $\alpha$ および $\beta$ までであることがわかります。

1) $n(\alpha, \beta) = n(\beta, \alpha) = 0;$
   $$
   (\overline{\alpha, \beta}) = \frac{\pi}{2}; \quad s_{\alpha}s_{\beta} \text{ of order } 2;
   $$
2) $n(\alpha, \beta) = n(\beta, \alpha) = 1;$
   $$
   (\overline{\alpha, \beta}) = \frac{\pi}{3}; \quad s_{\alpha}s_{\beta} \text{ of order } 3;
   $$
   $$
   \| \alpha \| = \| \beta \|;
   $$
3) $n(\alpha, \beta) = n(\beta, \alpha) = -1;$
   $$
   (\overline{\alpha, \beta}) = \frac{2\pi}{3}; \quad s_{\alpha}s_{\beta} \text{ of order } 3;
   $$
   $$
   \| \alpha \| = \| \beta \|;
   $$
4) $n(\alpha, \beta) = 1,\ n(\beta, \alpha) = 2;$
   $$
   (\overline{\alpha, \beta}) = \frac{\pi}{4}; \quad s_{\alpha}s_{\beta} \text{ of order } 4;
   $$
   $$
   \| \beta \| = \sqrt{2}\ \| \alpha \|;
   $$
5) $n(\alpha, \beta) = -1,\ n(\beta, \alpha) = -2;$
   $$
   (\overline{\alpha, \beta}) = \frac{3\pi}{4}; \quad s_{\alpha}s_{\beta} \text{ of order } 4;
   $$
   $$
   \| \beta \| = \sqrt{2}\ \| \alpha \|;
   $$
6) $n(\alpha, \beta) = 1,\ n(\beta, \alpha) = 3;$
   $$
   (\overline{\alpha, \beta}) = \frac{\pi}{6}; \quad s_{\alpha}s_{\beta} \text{ of order } 6;
   $$
   $$
   \| \beta \| = \sqrt{3}\ \| \alpha \|;
   $$
7) $n(\alpha, \beta) = -1,\ n(\beta, \alpha) = -3;$
   $$
   (\overline{\alpha, \beta}) = \frac{5\pi}{6}; \quad s_{\alpha}s_{\beta} \text{ of order } 6;
   $$
   $$
   \| \beta \| = \sqrt{3}\ \| \alpha \|;
   $$
8) $n(\alpha, \beta) = n(\beta, \alpha) = 2;$
   $$
   \alpha = \beta;
   $$
9) $n(\alpha, \beta) = n(\beta, \alpha) = -2;$
   $$
   \alpha = -\beta;
   $$
10) $n(\alpha, \beta) = 1,\ n(\beta, \alpha) = 4;$
    $$
    \beta = 2\alpha;
    $$
11) $n(\alpha, \beta) = -1,\ n(\beta, \alpha) = -4;$
    $$
    \beta = -2\alpha.
    $$

特に:

#### 命題 8 {#lie-vi-s1-prop-8 .statement tag=0AUK}

(i) *2 つの根が比例する場合、比例関係の因子は $\pm 1, \pm \frac{1}{2}, \pm 2$ しかありません。*

(ii) *$\alpha$ と $\beta$ が 2 つの非比例根で、$\| \alpha \| \leq \| \beta \|$ の場合、$n(\alpha, \beta)$ は値 0、1、-1 のいずれかをとります。*

根 $\alpha \in \mathbf{R}$ が $\frac{1}{2}\alpha \notin \mathbf{R}$ となる場合、$\alpha$ は *不可分* 根と呼ばれます。

#### 定理 1 {#lie-vi-s1-thm-1 .statement tag=0AUL}

*$\alpha, \beta$を2の根とします。*

(i) *$n(\alpha, \beta) > 0$ の場合、$\alpha - \beta$ は根 〜でない限り $\alpha = \beta$ です。*
(ii) *$n(\alpha, \beta) < 0$ の場合、$\alpha + \beta$ は根 〜でない限り $\alpha = -\beta$ です。*

$n(\alpha, \beta) > 0$ の場合、上記のリストによる可能性は次のとおりです。

1) $n(\alpha, \beta) = 1$;次に$\alpha - \beta - s_{\beta}(\alpha) \in \mathbf{R}$;
2) $n(\beta, \alpha) = 1$;次に $\beta - \alpha = s_{\alpha}(\beta) \in \mathbf{R}$、つまり $\alpha - \beta \in \mathbf{R}$;
3) $\beta = \alpha$。

これは (i) を証明し、(ii) は続いて $\beta$ を $-\beta$ に変更します。

#### 系 {#lie-vi-s1-n3-cor-1 .statement tag=0AUM}

$\alpha$ と $\beta$ を 2 根とします。

(i) *$(\alpha|\beta) > 0$ の場合、$\alpha - \beta$ は根 〜でない限り $\alpha = \beta$ です。
(ii) *$(\alpha|\beta) < 0$ の場合、$\alpha + \beta$ は根 〜でない限り $\alpha = -\beta$ です。
(iii) *$\alpha - \beta \notin \mathbf{R} \cup \{0\}$ と $\alpha + \beta \notin \mathbf{R} \cup \{0\}$ の場合*、*その後* $(\alpha|\beta) = 0$。

主張 (i) と (ii) は Th から続きます。 no. 1 の 1 と公式 (7)。 主張 (iii) は (i) と (ii) から続きます。

$\alpha + \beta \in \mathbf{R}$、$(\alpha|\beta) = 0$ (cf. プレート X、系 B_2) の可能性があります。 $\alpha - \beta \notin \mathbf{R} \cup \{0\}$ と $\alpha + \beta \notin \mathbf{R} \cup \{0\}$、$\alpha$ と $\beta$ は *強い直交* であると言われます。

#### 命題 9 {#lie-vi-s1-prop-9 .statement tag=0AUN}

$\alpha$ と $\beta$ を 2 つの非比例根とします。

(i) *集合* I *of 整数* j *そのような* $\beta + j\alpha$ *is 根は区間* $[ -q, p ]$ *in* $\mathbf{Z}$ *含む* 0。
(ii) *S を $\beta + j\alpha$ の集合 *for* $j \in \mathrm{I}$ とします。 *それでは*、
$$
s_{\alpha}(S) = S \quad \text{and} \quad s_{\alpha}(\beta + p\alpha) = \beta - q\alpha.
$$
(iii) $p - q = -n(\beta, \alpha)$。

明らかに、$0 \in \mathrm{I}$。 $p$ (それぞれ $-q$) を I の最大の (それぞれ最小の) 元とします。 $[ -q, p ]$ 属する ～ I のすべての整数が存在しない場合、$[ -q, p ]$ には次のプロパティを持つ 2 つの整数 $r, s$ が存在します: $1 \leq k \leq s - r - 1$ に対して $s > r + 1, s \in \mathrm{I}, r \in \mathrm{I}, r + k \notin \mathrm{I}$。コルの記法と。 Thの。 1、$(\alpha|\beta + s\alpha) \leq 0, (\alpha|\beta + r\alpha) \geq 0$、これは不合理です。
$$
(\alpha|\beta + s\alpha) \leq 0 > (\alpha|\beta + r\alpha).
$$
これは(i)を証明します。

$s_{\alpha}(\beta + j\alpha) = \beta - n(\beta, \alpha)\alpha - j\alpha = \beta + j'\alpha$ と $j' = -j - n(\beta, \alpha)$ があります。従って、$s_{\alpha}(S) \subseteq S$、その結果、$s_{\alpha}(S) = S$になります。現在、$j \mapsto -j - n(\beta, \alpha)$ は I から I までの減少する全単射です。 $j = p$のときは$j' = -q$となり、$-q = -p - n(\beta, \alpha)$となります。これは (ii) と (iii) を証明します。

集合 S は、$\beta$ によって定義される根の $\alpha$ チェーンと呼ばれ、$\beta - q\alpha$ がその始点、$\beta + p\alpha$ がその終点、$p + q$ がその長さです。

#### 系 {#lie-vi-s1-n3-cor-2 .statement tag=0AUO}

S を根の $\alpha$ 鎖とし、S の原点を $\gamma$ とします。S の長さは $-n(\gamma, \alpha)$ です。それは 0、1、2、または 3 に相当します。

最初の主張は、提案 9、(iii) から派生し、$\beta = \gamma$ に適用され、$q = 0$ という事実を使用します。

一方、$\gamma$ は$\alpha$ に比例しないため、この番号の最初に示したリストは、は $|n(\gamma, \alpha)| \leq 3$ であるため、系であることを示しています。

#### 注意 {#lie-vi-s1-n3-rem-1 .statement tag=0AUP}

上記の記法を保持します。次に:

1) S の長さが 0 の場合、$(\alpha|\gamma) = 0$。

2) S の長さが 1 の場合、$n(\gamma, \alpha) = -1$ となり、次の 3 つのケースがあります。

$$
n(\alpha, \gamma) = -1, \quad (\alpha|\alpha) = (\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{1}{2}(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{2\pi}{3}
$$
$$
n(\alpha, \gamma) = -2, \quad (\alpha|\alpha) = 2(\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{1}{2}(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{3\pi}{4}
$$
$$
n(\alpha, \gamma) = -3, \quad (\alpha|\alpha) = 3(\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{1}{2}(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{5\pi}{6}
$$

![3 つの図式は根系を示し、角度は π/3、π/4、2π/3、およびベクトル γ + α、γ、γ + 2α とラベル付けされています](../images/root_systems_1.png)

3) S の長さが 2 の場合、$n(\gamma, \alpha) = -2$ なので、

$$
n(\alpha, \gamma) = -1, \quad (\alpha|\alpha) = \frac{1}{2}(\gamma|\gamma), \quad (\alpha|\gamma) = -(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{3\pi}{4}.
$$

![図式は角度 π/4、π/4、およびベクトル γ、γ + α、γ + 2α で根系を示しています](../images/root_systems_2.png)

4) S の長さが 3 の場合、$n(\gamma, \alpha) = -3$ なので、

$$
n(\alpha, \gamma) = -1, \quad (\alpha|\alpha) = \frac{1}{3}(\gamma|\gamma), \quad (\alpha|\gamma) = -\frac{3}{2}(\alpha|\alpha), \quad (\overline{\alpha, \gamma}) = \frac{5\pi}{6}.
$$

![図式は、角度 π/6、π/3、π/6、およびベクトルで根系を示しています。γ、γ + α、γ + 2α、γ + 3α](../images/root_systems_3.png)

これらすべてのケースが実際に実現されることを見てみましょう (プレート X、系 A₂、B₂、G₂)。

#### 命題 10 {#lie-vi-s1-prop-10 .statement tag=0AUQ}

*$\alpha, \beta$を2つの非比例根とし、$\beta + \alpha$が根となるようにします。提案 9 で $p, q$ を整数とします。すると*

$$
\frac{(\beta + \alpha|\beta + \alpha)}{(\beta|\beta)} = \frac{q + 1}{p}.
$$

S をその原点である $\beta, \gamma$ によって定義される $\alpha$ チェーンとします。 $\beta + \alpha$ は根なので、長さ $l$ は $\geq 1$ です。次のようなケースが考えられます。

1) $l = 1$;それから$\beta = \gamma, q = 0, p = 1, (\beta + \alpha|\beta + \alpha) = (\beta|\beta)$。
2) $l = 2, \beta = \gamma$;次に$q = 0, p = 2, (\beta + \alpha|\beta + \alpha) = \frac{1}{2}(\beta|\beta)$。
3) $l = 2, \beta = \gamma + \alpha$;次に$q = 1, p = 1, (\beta + \alpha|\beta + \alpha) = 2(\beta|\beta)$。

4) $l = 3, \beta = \gamma$;次に$q = 0, p = 3, (\beta + \alpha|\beta + \alpha) = \frac{1}{3}(\beta|\beta)$。
5) $l = 3, \beta = \gamma + \alpha$;次に$q = 1, p = 2, (\beta + \alpha|\beta + \alpha) = (\beta|\beta)$。
6) $l = 3, \beta = \gamma + 2\alpha$;それから$q = 2, p = 1, (\beta + \alpha|\beta + \alpha) = 3(\beta|\beta)$。

いずれの場合も、証明すべき公式は満たされます。

#### 命題 11 {#lie-vi-s1-prop-11 .statement tag=0AUR}

*R は既約であると仮定します。 $\alpha$ と $\beta$ を 2 つの根とし、$\| \alpha \| = \| \beta \|$ とします。 $g(\alpha) = \beta$ となるような $g \in W(R)$ が存在します。*

$W(R)$ 生成する V による $\alpha$ の変換 (no. 2、提案 5 の修正)。したがって、$(g(\alpha)|\beta) \neq 0$ となるような $g \in W(R)$ が存在します。これからは$(\alpha|\beta) \neq 0$と仮定します。 no. 1、$n(\alpha, \beta) = n(\beta, \alpha)$の公式(9)まで。 置き換えること $\beta$ $s_\beta(\beta) = -\beta$ までに必要であれば、$n(\alpha, \beta) > 0$ と仮定できます。次に、no. 3 の先頭のリストにより、$\alpha = \beta$ (この場合、命題はクリアです)、または $n(\alpha, \beta) = n(\beta, \alpha) = 1$ のいずれかになります。その場合

$$
s_\alpha s_\beta s_\alpha(\beta) = s_\alpha s_\beta(\beta - \alpha) = s_\alpha(-\beta - \alpha + \beta) = \alpha.
$$

### 4. 約根系

系のすべての根が割り切れない (no. 3) 場合、根系は *還元* されると言われます。

#### 命題 12 {#lie-vi-s1-prop-12 .statement tag=0AUS}

*R は既約であり、還元されると仮定します。*

(i) *$\alpha \in R, \beta \in R$ の比率 $\frac{(\beta|\beta)}{(\alpha|\alpha)}$ は、値 1、2、$\frac{1}{2}$、3、$\frac{1}{3}$ のいずれかを取る必要があります。*

(ii) *$\alpha \in R$ の $(\alpha|\alpha)$ の集合には、最大 2 つの元が含まれます。*

R は既約なので、$W(R)$ 生成する V による根の変換 (no. 2、提案 5 の補正)。 したがって、任意の根 $\alpha, \beta$ に対して、$(\alpha|\beta') \neq 0$ と $(\beta'|\beta') = (\beta|\beta)$ のような根 $\beta'$ が存在します。 no. 1 の公式 (9) と no. 3 のリストにより、$\frac{(\beta'|\beta')}{(\alpha|\alpha)}$ は値 1、2、$\frac{1}{2}$、3、$\frac{1}{3}$ のいずれかをとります (系は削減されると仮定していることを思い出してください)。 $(x|y)$ に適切なスカラーを乗算すると、特定の根については $(\alpha|\alpha) = 1$ となり、$\beta \in R$ についての$(\beta|\beta)$ の他の可能な値は 2 と 3 であると仮定できます。 値 2 と 3 できないは両方とも達成されます。その場合、上で見たこととは逆に、$\frac{(\gamma|\gamma)}{(\beta|\beta)} = \frac{3}{2}$ となるような $\beta \in R, \gamma \in R$ が存在することになるからです。

#### 命題 13 {#lie-vi-s1-prop-13 .statement tag=0AUT}

*R は既約、非還元であり、階数 $\geq 2$ であると仮定します。*

(i) 不可分な根の*集合$R_0$は、Vの根系である。この系は既約であり、還元されます。そして$W(R_0) = W(R)$.*

(ii) *A を $(\alpha|\alpha)$ が最小の値 $\lambda$ となる、根 $\alpha$ の集合とする。この場合、A の任意の 2 つの非比例元は直交します。*

(iii) *B を $(\beta|\beta) = 2\lambda$ となるような $\beta \in R$ の集合とします。次に、$B \neq \varnothing$、$R_0 = A \cup B$、$R = A \cup B \cup 2A$。*

$\alpha \in R - R_0$ の場合、$\frac{1}{2} \alpha \in R$ ですが、$\frac{1}{2} (\frac{1}{2} \alpha) \notin R$ (提案 8) なので、$\frac{1}{2} \alpha \in R_0$ になります。これは、$R_0$ が (RS$_1$) を満たすことを証明します。すべての $\alpha \in R$、$s_{\alpha, \alpha^-}(R_0) = R_0$ について、$R_0$ が (RS$_{II}$) および (RS$_{III}$) を満たすことは明らかです。 $\alpha \in R - R_0$ は $\frac{1}{2} \alpha \in R_0$ を意味し、$s_\alpha = s_{\alpha/2}$ なので、$W(R) = W(R_0)$ になります。したがって、$R_0$ は既約であり (提案 5 の補正)、明らかに還元されます。

$R$は減らないので、$2\alpha \in R$となるような$\alpha \in R_0$が存在します。 $R_0$ は既約であり、$\dim V \geq 2$ であるため、$\alpha$ できないはすべての根に比例または直交します。 $\beta \in R_0$ を、$n(\beta, \alpha) \neq 0$ と $\beta$ が $\alpha$ に比例しないようにします。必要に応じて $\beta$ を $-\beta$ に変更すると、$n(\beta, \alpha) > 0$ と仮定できます。今は$\frac{1}{2} n(\beta, \alpha) = n(\beta, 2\alpha) \in \mathbf{Z}$なので、$n(\beta, \alpha) \in 2\mathbf{Z}$です。 no. 3、$n(\beta, \alpha) = 2$、$(\beta|\beta) = 2(\alpha|\alpha)$のリストから。 $R_0$ が減少するため、提案 12 は、すべての $\gamma \in R_0$ について、$(\gamma|\gamma) = (\alpha|\alpha)$ または $(\gamma|\gamma) = 2(\alpha|\alpha)$ のいずれかであることを示します。また、上記は、すべての $\gamma \in R - R_0$ に対して、ベクトル $\frac{1}{2} \gamma$ は $R_0$ の元であり、$(\frac{1}{2} \gamma|\frac{1}{2} \gamma) = (\alpha|\alpha)$ となることを示しています。したがって、$\lambda = (\alpha|\alpha)$、$B \neq \varnothing$、$R_0 = A \cup B$、$R \subseteq A \cup B \cup 2A$ となります。一方、$\gamma \in A$ の場合、$\gamma = g(\alpha)$ (提案 11) となるような $g \in W(R)$ が存在するため、$2\gamma = g(2\alpha) \in R$ となります。したがって、$2A \subseteq R$ と $R = A \cup B \cup 2A$ です。最後に、$\gamma, \gamma'$を$A$の2つの非比例元とします。それから

$$
n(2\gamma, \gamma') = 2n(\gamma, \gamma') = 4n(\gamma, 2\gamma') \in 4\mathbf{Z}, \quad \text{and} \quad |n(\gamma, \gamma')| \leq 1
$$

$\gamma$ と $\gamma'$ は同じ長さを持っているため、$n(\gamma, \gamma') = 0$ と $(\gamma|\gamma') = 0$ になります。

#### 命題 14 {#lie-vi-s1-prop-14 .statement tag=0AUU}

※$R$は既約で約分され、$(\alpha|\alpha)$は$\alpha \in R$に対して値$\lambda$と$2\lambda$がかかるとします。 $A$ を根 $\alpha$ の集合として、$(\alpha|\alpha) = \lambda$ とします。 $A$ の任意の 2 つの非比例元が直交していると仮定します。この場合、$R_1 = R \cup 2A$ は既約非還元根系であり、$R$ は$R_1$ の不可分な根の集合です。

$R_1$ が (RS$_1$) と (RS$_{III}$) を満たすことは明らかです。 $\alpha, \beta \in R_1$ の場合、$\langle \alpha^-, \beta \rangle \in \mathbf{Z}$ であることがわかります。 $\alpha \in R$であればこれはクリアです。 $\alpha \in A$の場合は$(2\alpha)^- = \frac{1}{2} \alpha^-$なので、$\alpha, \beta \in 2A$の場合は明らかになります。最後に、$\beta \in R$ と $\alpha = 2\gamma$ が $\gamma \in A$ であると仮定します。

1) $\gamma = \pm \beta$ の場合は、$\langle \alpha^-, \beta \rangle = \pm \frac{1}{2} \langle \gamma^-, \gamma \rangle = \pm 1$。
2) $\gamma$ が $\beta$ に比例しない場合、および $\beta \in A$ の場合、$A$ 上の仮定は $\langle \gamma^-, \beta \rangle = 0$ を意味するため、$\langle \alpha^-, \beta \rangle = 0$ になります。
3) $\beta \in R - A$ の場合、$(\beta|\beta) = 2\lambda = 2(\gamma|\gamma)$ となるため、no. 3 のリストにより、$\langle \beta, \gamma^- \rangle$ は 0、2、または -2 に等しくなります。したがって$\langle \beta, \alpha^- \rangle = \frac{1}{2} \langle \beta, \gamma^- \rangle \in \mathbf{Z}$。

したがって、$R_1$ は $V$ の根系であり、他の主張はクリアです。

### 5. チャンバーと根系の基底

すべての $\alpha \in R$ について、$L_\alpha$ を $s_\alpha$ の下で不変である $V$ のからなる 、点の超平面とします。 $L_\alpha$(V, § 1, no. 3章)の集合によって決定される$V$の部屋は、$R$の*部屋*と呼ばれます。 スカラー 積 $(x|y)$ で定義される全単射 $V \to V^*$ は、$\alpha \in R$ に対して $\alpha$ から $\frac{2\alpha^-}{(\alpha^-|\alpha^-)}$ を取り、したがって $L_\alpha$ から $L_{\alpha^-}$ となり、したがって $R$ のチャンバーから $R^-$ のチャンバーになります。 $C$が$R$のチャンバーである場合、$R^-$の対応するチャンバーは$C^-$で表されます。 no. 2 の提案 7 により、$C^-$ は $C$ のみに依存し、$(x|y)$ の選択には依存しません。

#### 定理 2 {#lie-vi-s1-thm-2 .statement tag=0AUV}

(i) *群* $W(R)$ *チャンバー*の集合に対して単純推移的に作用します。

(ii) *$C$ *を部屋とします。したがって、* $\overline{C}$ * は * $W(R)$ の基本ドメインです。

(iii) $C$ *is an open simplicial cone* (Chap. V, § 1, no. 6).

(iv) *$L_1, L_2, \ldots, L_l$*を*$C$の壁にしましょう。 *すべて* $i$ について、*固有の不可分な根* $\alpha_i$ *そのような* $L_i = L_{\alpha_i}$ *そしてそのような* $\alpha_i$ * は * $L_i$ * $C$ と同じ側にあります。

(v) *集合* $B(C) = \{ \alpha_1, \ldots, \alpha_l \}$ *は* $V$の基底です。

(vi) $C$ *は、* $x \in V$ の集合 * $\langle \alpha_i, x \rangle > 0$ * すべての* $i$ * (または同等に、* $x \in V$ の集合 * $(x|\alpha_i) > 0$ * すべての* $i$)。

(vii) *$S$ *を * $s_{\alpha_i}$ の集合とします。 *対* $(W(R), S)$ *はコクセター 系* (第 IV, § 1, no. 3 章)。

主張 (i) と (vii) は第 1 章から続きます。 V, § 3, no. 2、木。 1. 主張 (ii) は第 1 章の続きです。 V, § 3, no. 3、木。 2. 主張 (iv) はクリアです。 根 $\alpha_i$ は$L_i$ と直交し、$\alpha_i^-$ は$2\alpha_i / (\alpha_i|\alpha_i)$ と同一視されます。 $W(R)$ は必須なので (no. 1、*注意 3*)、主張 (iii)、(v)、(vi) は第 4 章から続きます。 V, § 3, no. 9、提案7。

#### 注意 1 {#lie-vi-s1-n5-rem-1 .statement tag=0AUW}

主張 (vii) は、特に $W(R)$ が反射 $s_{\alpha_i}$ によって *生成* されることを示しています。

#### 注意 2 {#lie-vi-s1-n5-rem-2 .statement tag=0AUX}

If $x, y \in C$, then $(x|y) > 0$ (Chap. V, § 3, no. 5, Lemma 6), in other words the angle $(x, y)$ is *acute*.

#### 注意 3 {#lie-vi-s1-n5-rem-3 .statement tag=0AUY}

$m(\alpha, \beta)$ を $s_{\alpha} s_{\beta}$ ($\alpha, \beta \in B(C)$) の位数とします。 The matrix $(m(\alpha, \beta))$ is identified with the *Coxeter matrix* (Chap. IV, § 1, no. 9) of $(W, S)$. $\alpha \neq \beta$ の場合、第 3 章の提案 3。 V, § 3, no. 4 は、角度 $(\alpha, \beta)$ が $\pi - \frac{\pi}{m(\alpha, \beta)}$ に等しいことを示します。特に、この角度は鈍角か、$\pi$ および $(\alpha|\beta) \leq 0$ に等しいです。 no. 3 のリストを使用すると、$m(\alpha, \beta)$ *は 2、3、4 *または* 6 に等しいことがわかります。

#### 定義 2 {#lie-vi-s1-def-2 .statement tag=0AUZ}

*部分集合* $B$ *of* $R$ *は基底 of* $R$ *チャンバーが存在する場合* $C$ *of* $R$ *そのような* $B = B(C)$。 *もし* $C$ *がチャンバー*である場合、 $B(C)$ *は* $R$ *によって定義される* $C$ の基底と呼ばれます。

#### 注意 4 {#lie-vi-s1-n5-rem-4 .statement tag=0AV0}

主張 (vi) Th. 2 shows that 写像 $C \mapsto B(C)$ is a *全単射* from 集合 of chambers to 集合 of 基底. Consequently, $W(R)$ acts *simply-transitively* on 集合 of 基底.

#### 注意 5 {#lie-vi-s1-n5-rem-5 .statement tag=0AV1}

Let $C$ be a chamber of $R$, and let $B$ be 対応する基底. If $\alpha \in B$, put $\varphi(\alpha) = \alpha^-$ if $2\alpha \notin R$ and $\varphi(\alpha) = \frac{1}{2}\alpha^-$ if $2\alpha \in R$. Then $\varphi(B)$ *is 基底 of* $R^-$ *defined by* $C^-$;これは、$C^-$の壁が$\alpha \in B$にとっての$L_{\alpha^-}$であるという事実からわかります。

#### 定義 3 {#lie-vi-s1-def-3 .statement tag=0AV2}

Let B be 基底 of R. The Cartan 行列 of R (relative to B) is 行列 $(n(\alpha, \beta))_{\alpha, \beta \in B}$.

$\alpha \in B$、$n(\alpha, \alpha) = 2$ 全員に。 $\alpha, \beta \in B$の場合、

$$
n(\alpha, \beta) = 2 \frac{(\alpha|\beta)}{(\beta|\beta)} = -2 \frac{\|\alpha\|}{\|\beta\|} \cos \frac{\pi}{m(\alpha, \beta)},
$$

where $m(\alpha, \beta)$ denotes as above 位数 of $s_\alpha s_\beta$. $\alpha \neq \beta$、$n(\alpha, \beta) = 0, -1, -2$、または$-3$ (cf. no. 3) の場合。

#### 注意 6 {#lie-vi-s1-n5-rem-6 .statement tag=0AV3}

カルタン行列 $(n(\alpha, \beta))$ をコクセター 行列 $(m(\alpha, \beta))$ と混同しないでください。 注意、特にカルタン行列は必ずしも対称ではないことに注意してください。

#### 注意 7 {#lie-vi-s1-n5-rem-7 .statement tag=0AV4}

正規のインデックス作成。 B と $B'$ が R の 2 つの基底である場合、$w(B) = B'$ となる一意元 $w \in W$ が存在します。私たちは持っています

$$
n(w(\alpha), w(\beta)) = n(\alpha, \beta) \quad \text{and} \quad m(w(\alpha), w(\beta)) = m(\alpha, \beta)
$$

$\alpha, \beta \in B$の場合。 Consequently, the Cartan and Coxeter 行列 associated to B can be obtained from those associated to $B'$ by 合成 with 全単射

$$
\alpha \mapsto w(\alpha)
$$

Bから$B'$まで。

The Cartan and Coxeter 行列 can actually be defined canonically in the following way. X を対 $(B, \alpha)$ の集合とします。ここで、B は R の基底と $\alpha \in B$ です。 群 W acts in an obvious way on X and each 軌道 of W on X meets each of 集合 $\{B\} \times B$ in exactly one 点. If I is 集合 of these 軌道, each 基底 B admits a canonical indexing $(\alpha_i)_{i \in I}$.さらに、型 $I \times I$ の一意の行列 $N = (n_{ij})$ (それぞれ $M = (m_{ij})$) が存在し、任意の基底 B に対して、B に関連付けられたカルタン (それぞれ Coxeter) 行列は、 B の正規インデックス付け。それは、R の標準カルタン行列 (それぞれ Coxeter 行列) と呼ばれます。

#### 命題 15 {#lie-vi-s1-prop-15 .statement tag=0AV5}

B を R の基底とし、$\alpha$ を不可分な根とします。 There exist $\beta \in B$ and $w \in W(R)$ such that $\alpha = w(\beta)$.

C を、$B = B(C)$ となるような部屋とします。 超平面 $L_\alpha$ is a wall of a chamber $C'$ of R, and there exists 元 of $W(R)$ that 変換 $C'$ to C.従って、$L_\alpha$ が C の壁である場合に帰着します。すると、$\alpha$はRの元$\beta$に比例します。$\alpha$と$\beta$は割り切れないので、$\alpha = \pm \beta$となります。 $\alpha = -\beta$ の場合、$\alpha = s_\beta(\beta)$、したがって命題となります。

#### 系 {#lie-vi-s1-n5-cor-1 .statement tag=0AV6}

$R_1$と$R_2$をベクトル空間$V_1$と$V_2$の2つの約根系とし、$B_1$と$B_2$を$R_1$と$R_2$の基底とします。 $R_1$ のカルタン行列を $R_2$ のカルタン変換とする $f : B_1 \to B_2$ を全単射とします。そして、$\alpha \in B_1$すべてに対して、同型$F : V_1 \to V_2$、変換$R_1$から$R_2$、$\alpha$から$f(\alpha)$が存在します。

$F$ を $V_1$ から $V_2$ までの同型とすると、すべての $\alpha \in B_1$ に対して $\alpha$ から $f(\alpha)$ がかかります。次に、$F$ 変換 $s_\alpha$ から $s_{f(\alpha)}$、したがって $W(R_1)$ から $W(R_2)$ (Th. 2)、したがって $R_1$ から $R_2$ (提案 15)。

#### 命題 16 {#lie-vi-s1-prop-16 .statement tag=0AV7}

$B$ を $R$ の基底とし、$G$ 部分群の $A(R)$ からなる元を安定させて、$B$ を安定させます。すると、$W(R)$は$A(R)$の通常の部分群、$A(R)$は$G$と$W(R)$の半直接積です。

If $\alpha \in R$ and $t \in A(R)$, then $ts_\alpha t^{-1} = s_{t(\alpha)}$; $W(R)$ は $s_\alpha$ によって生成されるため、$W(R)$ は $A(R)$ の通常の部分群であることがわかります。 構造の輸送、$A(R)$、変換、基底、$R$から$R$の基底まで。 $W(R)$ は基底の集合に対して単純推移的に作用するため、$A(R)$ のすべての元は形 $g_1 g_2$ ($g_1 \in W(R)$ と $g_2 \in G$) で一意に書くことができます。

#### 注意 8 {#lie-vi-s1-n5-rem-8 .statement tag=0AV8}

$R_1, \ldots, R_p$ をベクトル空間 $V_1, \ldots, V_p$、$R$ の$V = \prod_i V_i$、$C_i$ $R_i$、$B_i = B(C_i)$ のチャンバーの $R_i$ の直接和であるとします。 $C = \prod_i C_i$が$R$の部屋であり、$B(C) = \bigcup_i B_i$が明らかです。 それはThから続きます。このようにして、すべてのチャンバーと$R$の基底が得られることがわかります。

### 6. ポジティブ根

$C$ を $R$ の部屋とし、$B(C) = \{ \alpha_1, \ldots, \alpha_l \}$ を $R$ の対応する基底とします。 $C$ によって定義された $V$ (それぞれ $V^*$) の位数関係は、$V$ (それぞれ $V^*$) のベクトル空間構造と互換性のある位数関係です。 元 $\geq 0$ は、係数 $\geq 0$ と $\alpha_i$ (それぞれ $\alpha_i^*$) の線形結合です。 これら関係のうちの 1 つが陽性である元は、$C$ が陽性であるか、基底 $B(C)$ が陽性であると言われます。 これらの位数関係は、$W(R)$ の下でスカラー 積不変量を使用して $V$ を $V^*$ と識別することでわかるように、$C^*$ によっても定義されます。 Thの観点から、 $V^*$ の 2、no. 5、元は、$C$ の値が $\geq 0$ である場合に限り、$\geq 0$ になります。 $V$ の要素 $x$ は、$C^*$ の値が $\geq 0$ である場合、または同等に、すべての $y \in C$ について $(x|y) \geq 0$ である場合に限り、$\geq 0$ になります。

$\overline{C}$ の元は、第 1 章の補題 6 による $C$ の $\geq 0$ です。 V, § 3, no. 5。しかし、$C$ の元 $\geq 0$ の集合は、一般に $\overline{C}$ とは異なります (cf. プレート X、系 $A_2, B_2, G_2$)。

#### 定理 3 {#lie-vi-s1-thm-3 .statement tag=0AV9}

すべての根は $B(C)$ の元と同じ符号の整数係数を伴う線形結合です。特に、すべての根は、$C$ に対して正または負のいずれかになります。

$\alpha \in R$ の場合、$\alpha$ のカーネル $L_\alpha$ は $C^*$ を満たさないため、$\alpha$ は $C^*$ 全体で $> 0$ か、$C^*$ 全体で $< 0$ のいずれかであるため、2 番目のアサーションになります。 $\alpha$ が $B(C)$ によって生成された $V$ のサブグループ $P$ に含まれていることを示すことはまだ残っています。 $\alpha$ は分割できないと仮定できます。 現在、群 $P$ は、$\gamma \in B(C)$ に対して、$s_{\gamma}$ の下で明らかに安定しているため、Th による $W(R)$ の下でも安定しています。 2. $\alpha$ は形 $w(\beta)$ であるため、$w \in W(R)$ と $\beta \in B(C)$ (cf. 提案 15) により、$\alpha \in P$ が得られます。 Q.E.D.

$C$ に対して正である根の $R_+(C)$ 集合で示します。したがって、
$$
R = R_+(C) \cup (-R_+(C))
$$
は$R$の分割です。

#### 系 {#lie-vi-s1-n6-cor-1 .statement tag=0AVA}

*$\gamma$ を根の線形結合に整数係数を加え、$\alpha$ を割り切れない根とします。 $\gamma$ が $\alpha$ に比例する場合、$\gamma \in \mathbf{Z}\alpha$ となります。*

no. 5の提案15により、$C$は$\alpha \in B(C)$となるように選択できます。 Thさんより3、
$$
\gamma = \sum_{\beta \in B(C)} n_{\beta} \beta \quad \text{with} \quad n_{\beta} \in \mathbf{Z}.
$$
したがって、$\gamma$ が $\alpha$ に比例すると、$\gamma = n_{\alpha} \alpha$ となり、系が証明されます。

ここで、$S$ を $\alpha \in B(C)$ の反射 $s_{\alpha}$ の集合とし、$T$ を $W$ の下の $S$ の共役の和集合とします。 $\alpha \in B(C)$ と $w \in W$ の場合、$T$ の元 $t = ws_{\alpha}w^{-1}$ は、根 $\beta = w(\alpha)$ に関連付けられた直交反射$s_{\beta}$ です。逆に、分割不可能な根 $\beta$ に対して、$\alpha = w^{-1}(\beta) \in B(C)$ (提案 15) と $s_{\beta} = ws_{\alpha}w^{-1} \in T$ のような元 $w \in W$ が存在します。したがって、割り切れない根の集合から $\{\pm 1\} \times T$ までの *全単射* $\psi$ は、割り切れない根 $\beta$ 対 $(\varepsilon, s_{\beta})$ に関連付けることによって得られます。ここで、$\varepsilon = +1$ $\beta$ がプラス、$\beta$ がマイナスの場合は $\varepsilon = -1$ となります。

一方、$(W, S)$ は Coxeter 系 (Th. 2) であり、第 2 章の結果です。 IV, § 1, no. 4が適用できます。 $w$ が長さの $W$ の元 ($S$ に関して) $q$ に等しい場合、$q$ 元とともに、$T$ の部分集合 $T_w$ が存在することがわかりました。それが、$w = s_1 \ldots s_q$ と $s_i \in S$ の場合、および
$$
t_i = s_1 \ldots s_{i-1} s_i s_{i-1} \ldots s_1
$$
($1 \leq i \leq q$の場合)、次に$T_w = \{t_1, \ldots, t_q\}$。 § 1 数 $\eta(w, t)$ ($w \in W$ と $t \in T$ の場合) の no. 4 でも、$t \notin T_w$ の場合は $+1$ に、$t \in T_w$ の場合は $-1$ に等しいと定義したことを思い出してください。 最後に、集合 $\{\pm 1\} \times T$ から公式までに定義する写像 $U_w$ をそれ自体にすると、
$$
U_w(\varepsilon, t) = (\varepsilon \eta(w^{-1}, t), wt w^{-1}),
$$
写像 $w \mapsto U_w$ は、集合 $\{\pm 1\} \times T$ の置換の $W$ から群までの *準同型* です (IV, § 1, no. 4、補題 1 章)。

#### 命題 17 {#lie-vi-s1-prop-17 .statement tag=0AVB}

*$R$ が減少したと仮定し、$w \in W$ と $\alpha \in R$ とします。*

(i) *$\psi(w(\alpha)) = U_w(\psi(\alpha))$があります*。
(ii) *$\alpha$ が正であると仮定します。 根 $w(\alpha)$ は * の場合にのみ負です
$$
\eta(w^{-1}, s_{\alpha}) = -1,
$$
*他の語の場合* $s_{\alpha} \in T_{w^{-1}}$。

(iii) 部屋Cと$w(C)$が超平面$L_\alpha$の反対側にある場合に限り、$\eta(w, s_\alpha) = -1$が得られます。他の語、集合 $T_w$は、Cと$w(C)$を隔てる壁に対する反射で構成されています。

$\beta \in B(C)$ として、$s = s_\beta$ を置きます。明らかに $T_s = \{ s \}$ であり、その結果、

$$
U_s(\varepsilon, t) = \begin{cases}
(\varepsilon, st s^{-1}) & \text{if } t \neq s \\
(-\varepsilon, s) & \text{if } t = s.
\end{cases}
$$

一方、$\rho = \sum_{\gamma \in B(C)} n_\gamma(\rho) \gamma$ を正の根とします。置く

$$
s(\rho) = \sum_{\gamma \in B(C)} n_\gamma(s(\rho)) \gamma.
$$

$\rho \neq \beta$ の場合、$\gamma \neq \beta$ を伴う元 $\gamma \in B(C)$ が存在し、$n_\gamma(\rho) > 0$ となり、$n_\gamma(s(\rho)) = n_\gamma(\rho) > 0$ (no. 1, 公式 (5)) が得られます。従って、$s(\rho)$ は正です。私たちはすぐに次のことを推測します

$$
\psi(s(\varepsilon, \rho)) = \begin{cases}
(\varepsilon, ss_\rho s^{-1}) & \text{if } \rho \neq \beta \\
(-\varepsilon, s) & \text{if } \rho = \beta.
\end{cases}
$$

(12) と (13) を比較すると、すべての根 $\gamma$ とすべての $s \in S$ が $U_s(\psi(\gamma)) = \psi(s(\gamma))$ であることがわかります。 S 生成する W なので、(i) が続きます。

一方、$w(\alpha)$が負であるというは、というと同等です。

$$
\psi(w(\alpha)) = (-1, ws_\alpha w^{-1}),
$$

または、(i) によって、その $U_w(\psi(\alpha)) = (-1, ws_\alpha w^{-1})$。 加法 $\alpha$ が正の場合、$\psi(\alpha) = (+1, s_\alpha)$ と $U_w(\psi(\alpha)) = (\eta(w^{-1}, s_\alpha), ws_\alpha w^{-1})$、従って (ii)。

最後に、(ii) により、根 $\alpha$ と $w^{-1}(\alpha)$ の一方が正で、もう一方が負の場合に限り、$\eta(w, s_\alpha) = -1$ となります。これは、すべての $x \in C$ に対して $(\alpha|x).(w^{-1}(\alpha)|x) = (\alpha|x).(w|x) < 0$ であるというに相当するため、(iii) の最初の主張になります。 (iii) の 2 番目の主張がすぐに続きます。

#### 系 1 {#lie-vi-s1-prop-17-cor-1 .statement tag=0AVC}

$\beta \in B(C)$ にしましょう。反射$s_\beta$は、$\beta$に比例しない正の根を並べ替えます。

直ちに R が減少する場合を簡約する説明します。その場合、主張は (ii) と $T_{s_\beta} = s_\beta$ という事実から導き出されます。

#### 系 2 {#lie-vi-s1-prop-17-cor-2 .statement tag=0AVD}

Rが減少すると仮定します。 Let $w \in W$, let q be the length of $w$ with respect to S (Chap. IV, § 1, no. 1), and let $w = s_1 \ldots s_q$ be a reduced decomposition of $w$. $\alpha_1, \ldots, \alpha_q$ を $B(C)$ 対応する ～ $s_1, \ldots, s_q$ の元とします。 置く

$$
\theta_i = s_q s_{q-1} \ldots s_{i+1}(\alpha_i), \quad i = 1, \ldots, q.
$$

根 $\theta_i$ は、ペアごとに異なる $> 0$、$w(\theta_i) < 0$、および$w(\alpha) < 0$ が $\theta_i$ の 1 つと等しいようなすべての根 $\alpha > 0$ です。

X を $w(\alpha) < 0$ となるような $\alpha > 0$ の集合とします。 (ii)により、

$$
\operatorname{Card}(X) = \operatorname{Card}(T_{w^{-1}}) = l(w^{-1}) = l(w) = q.
$$

一方、$\alpha \in X$ の場合、次のような $i \in \{1, q\}$ が存在することは明らかです。

$$
s_{i+1} \ldots s_q(\alpha) > 0 \quad \text{and} \quad s_i s_{i+1} \ldots s_q(\alpha) < 0.
$$

コル著1 の場合、これは $s_{i+1} \ldots s_q(\alpha) = \alpha_i$ を意味し、したがって $\alpha = \theta_i$ を意味します。したがって、集合 X は、$\theta_i$ の集合に含まれます。 $\operatorname{Card}(X) = q$ 以降、これは、X が $\theta_i$ の集合に等しく、これらがペアごとに異なる場合にのみ可能です。したがって系です。

#### 系 3 {#lie-vi-s1-prop-17-cor-3 .statement tag=0AVE}

※Rが小さくなったとします。 W にはユニークな最長元 $w_0$ が存在します。その長さは、正の根と $w_0$ 変換の部屋 C から $-C$ の数に等しいです。すべての $w \in W$ に対して、$w_0^2 = 1$ と $l(ww_0) = l(w_0) - l(w)$ があります。*

$-C$ が部屋であることは明らかです。したがって、変換 C から $-C$ までの W の元 $w_0$ が存在します。次に、すべての正の根 $\alpha$ と Cor の最初の 2 つの主張に対して $w_0(\alpha) < 0$ が返されます。 3人はコルの明らか帰結です。 2. $w_0^2(C) = C$ があるので、$w_0^2 = 1$ です。最後に、$w \in W$ の場合、長さ $l(w)$ (それぞれ $l(ww_0)$) は、提案 17 (iii) により、C と $w(C)$ (それぞれ $ww_0(C) = -w(C)$) を隔てる壁の数に等しい。 $w(C)$ と $-w(C)$ はすべての壁の反対側にあるため、和 $l(w) + l(w_0)$ は壁の合計数、つまり $l(w_0)$ に等しくなります。

#### 命題 18 {#lie-vi-s1-prop-18 .statement tag=0AVF}

*$x \in V$にしておきます。次の 3 つのプロパティは同等です。

(i) $x \in \overline{C}$;
(ii) すべての $\alpha \in B(C)$ に対して $x \geq s_\alpha(x)$ (C によって定義される位数関係に関して)。
(iii) $w \in W$ 全員に対して $x \geq w(x)$。

$s_\alpha(x) = x - \langle x, \alpha^\vee \rangle \alpha$ と $\overline{C}$ は元 $x \in V$ の集合であるため、すべての $\alpha \in B(C)$ に対して $\langle x, \alpha^\vee \rangle \geq 0$、(i) と (ii) の同値は明らかです。一方、(iii) $\Longrightarrow$ (ii) は明らかです。 (i) $\Longrightarrow$ (iii) であることを示します。 $x \in \overline{C}$ とし、$w \in W$ とします。 長さ $l(w)$ の $w$ について帰納法で議論します。 $l(w) = 0$ のケースは些細なものです。 $l(w) \geq 1$なら、$w$は形$w = w' s_\alpha$に$\alpha \in B(C)$と$l(w') = l(w) - 1$で書けます。それから

$$
x - w(x) = x - w'(x) + w'(x - s_\alpha(x)).
$$

帰納法の仮定は、$x - w'(x)$ が陽性であることを示します。一方、

$$
w'(x - s_\alpha(x)) = w(s_\alpha(x) - x) = -\langle x, \alpha^\vee \rangle w(\alpha).
$$

現在は $s_\alpha \in T_{w^{-1}}$ であり、提案 17 (ii) は $w(\alpha) < 0$ を示しています。したがって、結果は次のとおりです。

#### 系 {#lie-vi-s1-n6-cor-2 .statement tag=0AVG}

元 $x \in C$ すべての $w \in W$ に対して $x > w(x)$ が$w \neq 1$ となる場合に限ります。

#### 命題 19 {#lie-vi-s1-prop-19 .statement tag=0AVH}

$(\beta_i)_{1 \leq i \leq n}$ をチャンバー $C$ の正の根の数列として、$\beta_1 + \beta_2 + \cdots + \beta_n$ が根となるようにします。次に、すべての $i \in \{1, 2, \ldots, n\}$ に対して、$\beta_{\pi(1)} + \beta_{\pi(2)} + \cdots + \beta_{\pi(i)}$ が根となるような置換 $\pi \in S_n$ が存在します。

私たちは$n$に対して帰納法によって議論し、命題は$n \leq 2$に対して明確です。 $\beta = \beta_1 + \cdots + \beta_n$を入れます。すると $\sum_{i=1}^n (\beta|\beta_i) = (\beta|\beta) > 0$ なので、$(\beta|\beta_k) > 0$ となるような添字 $k$ が存在します。 $\beta = \beta_k$ の場合、すべての $i$ については $\beta_i > 0$ 以降、$n = 1$ になります。それ以外の場合、$\beta - \beta_k$ は根 (no. 3、Th. 1 の Cor.) です。その場合、帰納法の仮定を $\beta - \beta_k = \sum_{i \neq k} \beta_i$ に適用するだけで十分です。

#### 系 1 {#lie-vi-s1-prop-19-cor-1 .statement tag=0AVI}

$\alpha \in R_+(C)$ にしましょう。次に、$\alpha$ が 2 つの正の根のうち和である場合に限り、$\alpha \in B(C)$ となります。

$\alpha$ が 2 つの正の根のうち和である場合、Th. 3 は $\alpha \in B(C)$ を示します。 $\alpha \notin B(C)$の場合、Th。 3 は、$k$ と $n \geq 2$ のすべてに対して $\alpha = \sum_{k=1}^n \beta_k$ と $\beta_k \in B(C)$ が含まれていることを示しています。

必要に応じて $\beta_k$ を並べ替えると、$\sum_{k=1}^{n-1}$ は根 (提案 19)、したがって $\alpha$ は正の根 $\sum_{k=1}^{n-1} \beta_k$ と $\beta_n$ の和であると仮定できます。

#### 系 2 {#lie-vi-s1-prop-19-cor-2 .statement tag=0AVJ}

$\varphi$ を $R$ からアーベル群 $\Gamma$ までの写像とし、次の特性を持ちます。

1) $\alpha \in R$ の場合は $\varphi(-\alpha) = -\varphi(\alpha)$;
2) $\alpha \in R, \beta \in R$ が $\alpha + \beta \in R$ となる場合、$\varphi(\alpha + \beta) = \varphi(\alpha) + \varphi(\beta)$。

$Q$ を、$R$ によって生成された $V$ の部分群とします。その後、$\varphi$ 拡大するから準同型 、$Q$ から $\Gamma$ となります。

$B$を$R$の基底とします。 $\psi$を$Q$から$\Gamma$までの一意な準同型とし、$B$に$\varphi$を加えた一致するとします。 $\alpha$ が $B$ に対して正の根であるとき、$\psi(\alpha) = \varphi(\alpha)$ が示されれば十分です。 $\alpha = \beta_1 + \cdots + \beta_m$ には、すべての $i$ には $\beta_i \in B$ が、すべての $h$ には $\beta_1 + \cdots + \beta_h \in R$ が含まれます (提案 19)。 $m$ の帰納法までに $\psi(\alpha) = \varphi(\alpha)$ であることがわかります。 $m = 1$であればこれはクリアです。 帰納法の仮定が与えます

$$
\psi(\beta_1 + \cdots + \beta_{m-1}) = \varphi(\beta_1 + \cdots + \beta_{m-1}),
$$

$\psi(\beta_m) = \varphi(\beta_m)$ があるため、$\psi(\alpha) = \varphi(\alpha)$ となり、系と証明されます。

$R$ の根 $\alpha = \sum_{\beta \in B(C)} n_\beta \beta$ については、$n_\beta \neq 0$ となるように、$\beta \in B(C)$ の $Y(\alpha)$ 集合で表します。さらに、$B(C)$ は、$W(R)$ と$s_{\alpha_i}$ によって形成される Coxeter のグラフ系の頂点の集合と識別できることに注目してください (cf. 章 IV, § 1, no. 9 および章 V, § 3, no. 2)。

#### 系 3 {#lie-vi-s1-prop-19-cor-3 .statement tag=0AVK}

a) $\alpha \in \mathbf{R}$ とします。そして、$Y(\alpha)$は$B(C)$の部分集合とつながったものになります（IV、付録章）。

b) $Y$ を、$B(C)$ の空ではない接続された部分集合とします。その後、$\sum_{\beta \in Y} \beta$ 属するから $\mathbf{R}$ となります。

a) を証明するには、$\alpha$ が正であると仮定できます。 $\mathrm{Card}(Y(\alpha))$ については帰納法によって議論され、$\mathrm{Card}(Y(\alpha)) = 1$ であれば主張は自明である。提案 19 により、$\alpha - \beta \in \mathbf{R}$ となるような $\beta \in B(C)$ が存在します。 $p$ を最大の整数 $\geqslant 0$ として、$\gamma = \alpha - p\beta \in \mathbf{R}$ とします。 $\gamma - \beta \notin \mathbf{R}$ と $\gamma + p\beta \in \mathbf{R}$ なので、$(\gamma|\beta) \neq 0$ (提案 9)。したがって、$\beta$ は $Y(\gamma)$ の少なくとも 1 つの元にリンクされています。しかし、$Y(\alpha) = Y(\gamma) \cup \{\beta\}$と$Y(\gamma)$は帰納法の仮定で結ばれています。したがって、$Y(\alpha)$ は接続されており、a) が証明されます。

ここで、$Y$ を、$B(C)$ の空ではない接続された部分集合とします。 $\mathrm{Card}(Y)$ の帰納法によって、$\sum_{\beta \in Y} \beta$ は根であることがわかります。 $\mathrm{Card}(Y) \leqslant 1$ が自明な場合。 $\mathrm{Card}(Y) \geqslant 2$ と仮定します。 $X$ は森林であるため (章 V, § 4, no. 8、提案 8)、$Y$ は木であり、終端頂点 $\beta$ を持ちます (章 IV、付録)。 集合 $Y - \{\beta\}$ が接続されており、その元の 1 つが $\beta$ にリンクされています。 帰納法の仮定、$\alpha = \sum_{\gamma \in Y - \{\beta\}} \gamma \in \mathbf{R}$、そして$(\alpha|\beta) < 0$ 以降は、$\alpha + \beta \in \mathbf{R}$ (木曜日 1) になります。 Q.E.D.

### 7. 閉店集合中根

#### 定義 4 {#lie-vi-s1-def-4 .statement tag=0AVL}

$P$を$\mathbf{R}$の部分集合とします。

(i) 条件 $\alpha \in P, \beta \in P, \alpha + \beta \in \mathbf{R}$ が $\alpha + \beta \in P$ を暗示する場合、$P$ は閉じていると言われます。

(ii) $P$ が閉じていて、$P \cup (-P) = \mathbf{R}$ の場合、$P$ は放物線であると言われます。

(iii) $P$ は、$P = -P$ であれば対称であると言われます。

#### 補題 3 {#lie-vi-s1-lem-3 .statement tag=0AVM}

$C$ を $\mathbf{R}$ の議場とし、$P$ を $\mathbf{R}$ 含む $R_+(C)$ の閉じた部分集合 (no. 6 の記法で) とします。 $\Sigma = B(C) \cap (-P)$ を、$Q$ を、$\Sigma$ の元の線形結合と非正の整数係数である根の集合とします。次に、$P = R_+(C) \cup Q$。

$P \cap (-R_+(C)) = Q$ を示すだけで十分です。 $-\alpha \in Q$ にしましょう。すると、$\alpha$は$n$の和、$\Sigma$の元になります。 $n$ の帰納法までに、$-\alpha \in P$ であることがわかります。 $n = 1$であればこれはクリアです。 $n > 1$ の場合、no. 6 の提案 19 により、$\gamma \in \Sigma$ と $\beta$ 和の $n - 1$ 元の $\Sigma$ で $\alpha = \beta + \gamma$ を書くことができます。 帰納法の仮定、$-\beta \in P$までに。 $-\gamma \in P$ 以降、$P$ は休業のため、$-\alpha \in P$ となります。したがって、$Q \subseteq P \cap (-R_+(C))$。逆に$-\alpha \in P \cap (-R_+(C))$とします。すると、$\alpha$は、$p$の和、$B(C)$の元となります。 $p$の帰納法までに$-\alpha \in Q$であることがわかります。 $p = 1$であればこれは明らかです。 $p > 1$ の場合、提案 19 により、$\gamma \in B(C)$ と $\beta$ 根で $\alpha = \beta + \gamma$ を書くことができます。つまり、$p - 1$ の和 $B(C)$ の元です。 $-\gamma = \beta + (-\alpha)$ と $P$ が休業であるため、$-\gamma \in P$、したがって $\gamma \in \Sigma$ になります。しかも、$P$が休みなので$-\beta = \gamma + (-\alpha)$なので$-\beta \in P$になります。 帰納法の仮定、$-\beta \in Q$までに、つまり$-\alpha = -\beta - \gamma \in Q$です。したがって、$P \cap (-R_+(C)) \subseteq Q$。

#### 命題 20 {#lie-vi-s1-prop-20 .statement tag=0AVN}

※$P$を$R$の部分集合とします。次の条件は同等です*:

(i) $P$ *放物線*;
(ii) $P$ * は閉じており、$P \supseteq R_+(C)$* となるような $R$ のチャンバー $C$ が存在します。
(iii) *$R$の$C$と$B(C)$の部分集合$\Sigma$が存在し、$P$は$R_+(C)$の和集合、根の集合$Q$となるつまり、線形結合 of 元 of $\Sigma$ と非正の整数係数* です。

(ii) $\Longrightarrow$ (iii): これは補題 3 から続きます。

(iii) $\Longrightarrow$ (i): (iii) の仮定と記法を採用します。 $P \cup (-P) = R$であることは明らかです。 $\alpha, \beta \in P$ が $\alpha + \beta \in R$ である場合、$\alpha + \beta \in P$ であることを示します。 根 $\alpha + \beta$ が正の場合、これは明らかです。 $\alpha + \beta$ が負であると仮定します。次に$\alpha + \beta = \sum_{\gamma \in B(C)} n_\gamma \gamma$、$n_\gamma \leq 0$となります。しかし、$\alpha$ または $\beta$ の$B(C) - \Sigma$ のすべての元 $\gamma$ の係数は $\geq 0$ です。従って、$\gamma \in B(C) - \Sigma$なら$n_\gamma = 0$、つまり$\alpha + \beta \in Q \subseteq P$です。

(i) $\Longrightarrow$ (ii): $P$ が放物線であると仮定します。 $C$ を、$\mathrm{Card}(P \cap R_+(C))$ ができるだけ大きくなるような部屋とします。 $\alpha \in B(C)$ として、$\alpha \in P$ と仮定すると、$-\alpha \in P$ となります。すべての $\beta \in P \cap R_+(C)$ について、$\beta$ は $\alpha$ に比例しません (仮定の場合、$\beta = 2\alpha$ は、$P$ が閉じているため、$\alpha = 2\alpha + (-\alpha) \in P$ を意味します)。従って、$s_\alpha(\beta) \in R_+(C)$ (no. 6、提案 17 のコリント 1)。 $C' = s_\alpha(C)$ とすると、$\beta = s_\alpha(s_\alpha(\beta)) \in s_\alpha(R_+(C)) = R_+(C)$、つまり $-\alpha \in P \cap R_+(C')$、従って $\mathrm{Card}(P \cap R_+(C')) > \mathrm{Card}(P \cap R_+(C))$ となります。 $\alpha \in P$ですから、これは不合理です。従って、提案 19 により $B(C) \subseteq P$、その結果として $R_+(C) \subseteq P$ が成立し、$P$ は閉じられます。

#### 系 1 {#lie-vi-s1-prop-20-cor-1 .statement tag=0AVO}

※$P$を$R$の部分集合とします。次の条件は同等です*:

(i) *$P = R_+(C)$* となるチャンバー $C$ が存在します。
(ii) *$P$ は閉じており、$\{P, -P\}$ は $R$* の分割です。

*チャンバー $C$ は、$P = R_+(C)$ が一意になります*。

$P = R_+(C)$ の場合、$C$ は $x^* \in V^*$ の集合で、すべての $x \in P$ に対して $\langle x^*, x \rangle > 0$ となるため、$C$ の一意性となります。

#### 系 2 {#lie-vi-s1-prop-20-cor-2 .statement tag=0AVP}

*$V$ には、注文されたベクトル空間の構造が装備されており、この構造では、$R$ のすべての根が正または負になると仮定します。この構造に対して根をプラスしたものを$P$を集合とします。次に、$P = R_+(C)$* のような$R$ の固有の部屋 $C$ が存在します。

確かに、$P$ は Cor の条件 (ii) を満たします。 1.

この系は、検討中の位数が合計で、$R$ の条件が自動的に満たされる場合に特に当てはまります。 このような位数は、たとえば、$V$ の基底 $(e_i)_{1 \leq i \leq n}$ を選択し、$V$ で辞書編集上の位数を取得することによって取得できることを思い出してください。したがって、すべての $\xi_i$ が 0 の場合、または $\xi_i > 0$ の場合、$x = \sum_i \xi_i e_i$ は $\geq 0$ になります。 最小の添字 $i$ では、$\xi_i \neq 0$ になります。

#### 系 3 {#lie-vi-s1-prop-20-cor-3 .statement tag=0AVQ}

*次の条件が満たされる場合に限り、R の部分集合 B は R の基底になります:*

(i) B の *元は線形独立です。*
(ii) *R のすべての根は B の元の線形結合であり、係数はすべて正であるか、すべて負です。*
(iii) *B のすべての根は分割できません。*

条件が必要であることはすでにわかっています (no. 5、Th. 2、および no. 6、Th. 3)。 条件 (i)、(ii)、(iii) が満たされると仮定します。 P を、係数 $\geq 0$ を持つ B の元の線形結合である根の集合とします。 P は Cor. の条件 (ii) を満たすので、 1、$P = R_+(C)$ のようなチャンバー C が存在します。 $B' = B(C)$、X と $X'$ を B と $B'$ によって生成された凸円錐とします。それから

$$
B \subseteq P \subseteq X \quad \text{and} \quad B' \subseteq P \subseteq X',
$$

これは、X と $X'$ が両方とも P によって生成され、したがって一致するが生成されることを示しています。しかし、B の元 (それぞれ $B'$) によって生成される半線は、X (それぞれ $X'$) の極端な生成元です。このような半線含むは、割り切れない根、$B = B'$ 1 つだけです。

#### 系 4 {#lie-vi-s1-prop-20-cor-4 .statement tag=0AVR}

*BをRの基底、Bの$B'$部分集合、$B'$によって生成されたVの$V'$ベクトル部分空間、および$R' = R \cap V'$とします。すると、$B'$ は根系 $B'$ の基底になります。*

これはコルからすぐに続きます。 3とコル。提案4の。

$R'$ 根系を $B'$ によって *生成* と呼びます。

#### 系 5 {#lie-vi-s1-prop-20-cor-5 .statement tag=0AVS}

*B を R、$A_1, A_2, \ldots, A_r$ B のペアごとの直交部分集合、および $A = A_1 \cup A_2 \cup \cdots \cup A_r$ の基底とします。 すると、A の元の線形結合であるすべての根 $\alpha$ は、実際には $A_i$ の 1 つの元の線形結合になります。 特に、R が既約の場合、対直交部分集合への B の分割は存在しません。

$E_1, \ldots, E_r, E$ をそれぞれ、$A_1, \ldots, A_r, A$ によって生成された V のベクトル部分空間とします。コル著4 では、$E = V$ と仮定できます。それから、Thさんによる。 no. 5 の 2 (vii)、$E_i$ は $W(R)$ の下で安定しているため、R は $R \cap E_i$ の和集合 (no. 2、提案 5)。

#### 系 6 {#lie-vi-s1-prop-20-cor-6 .statement tag=0AVT}

※提案20の仮説と記法を採用し、$V_1$を$\Sigma$によって生成されたVのベクトル部分空間とする。すると、$P \cap (-P) = Q \cup (-Q) = V_1 \cap R$ は基底 $\Sigma$ を含む $V_1$ の根系になります。

$P \cap (-P) = (R_+(C) \cup Q) \cap ((-R_+(C)) \cup (-Q)) = Q \cup (-Q)$ があります。 Th. 3 は $Q \cup (-Q) = V_1 \cap R$ を証明します。最後に、$\Sigma$ は Cor による根系 $V_1 \cap R$ の基底です。 4.

#### 命題 21 {#lie-vi-s1-prop-21 .statement tag=0AVU}

*C (それぞれ $C'$) を R、$\Sigma$ (それぞれ $\Sigma'$) 部分集合の $B(C)$ (それぞれ $B(C')$)、Q (それぞれ $Q'$) 集合の線形結合とする$\Sigma$ (それぞれ $\Sigma'$) の元と、マイナスの整数係数および $P = Q \cup R_+(C)$ (それぞれ $P' = Q' \cup R_+(C')$)。 P を $P'$ に変換するワイル群の元が存在する場合、C を $C'$ に、$\Sigma$ を $\Sigma'$ に変換するワイル群の元が存在します。

私たちは簡約するすぐに $P = P'$ の事件に取り組みます。 $V_1$ を、$P \cap (-P)$ によって生成された V のベクトル部分空間とします。 すると、$\Sigma$ と $\Sigma'$ は、$V_1$ の根系 $R_1 = P \cap (-P)$ の基底になります (提案 20 の Cor. 6)。 したがって、$g_1(\Sigma) = \Sigma'$ となるような $g_1 \in W(R_1)$ が存在します。 $g_1$ は、$\sigma \in \Sigma$ との対称性 $s_\sigma$ の積である $W(R)$ の元 $g$ によって誘発されることは明らかです。 $\gamma = \sum_{\beta \in B(C)} c_\beta \beta$ を $P - R_1$ の元とします。 次に、少なくとも 1 つの $\beta \in B(C) - \Sigma$ に対して $c_\beta > 0$ です。 さらに、$\sigma \in \Sigma$ の場合、$s_\sigma(\gamma) - \gamma \in V_1$ なので、$s_\sigma(\gamma)$ は$B(C)$ (no. 1, 公式 (5)) に関して少なくとも 1 つの座標 $> 0$ を持ち、したがって$s_\sigma(\gamma) \in R_+(C)$、そして最後に$s_\sigma(\gamma) \in P - R_1$ となります。 したがって、$P - R_1$ は $s_\sigma, \sigma \in \Sigma$ の下で安定しており、したがって $g$ の下でも安定しているため、$g(P) = P$ になります。 したがって、$P = P'$ と $\Sigma = \Sigma'$ のとき、私たちは証明命題に減ります。 この場合、$Q = Q'$、したがって $R_+(C) = P - Q = P - Q' = R_+(C')$、したがって $C = C'$ (提案 20 の訂正 1)。

#### 系 {#lie-vi-s1-n7-cor-1 .statement tag=0AVV}

*P、$P'$を、ワイル群の元によって互いに変換されたRの2つの放物線部分集合とする。 $R_+(C) \subseteq P$ と $R_+(C) \subseteq P'$ のような R の部屋 C が存在する場合、$P = P'$ になります。

C を C に変換する $W(R)$ の唯一の元が 1, cf. no. 5, Th であるため、これは補題 3 と提案 21 に続きます。 2.

#### 命題 22 {#lie-vi-s1-prop-22 .statement tag=0AVW}

*P を、$P \cap (-P) = \varnothing$ となる R の閉じた部分集合とします。すると、$P \subseteq R_+(C)$ となるような R の部屋 C が存在します。

1) コルの観点から。 Thの。 1、no. 3、仮定 $\alpha \in P, \beta \in P, (\alpha|\beta) < 0$ は、$\alpha + \beta \in P$ を暗示します。

2) P の元の和 $\alpha_1 + \cdots + \alpha_q$ ($q \geqslant 1$) は零ではないことを示します。 $q$の帰納法までに進みます。 主張は $q = 1$ に対してクリアなので、$q \geqslant 2$ と仮定します。 $\alpha_1 + \cdots + \alpha_q = 0$ の場合、

$$
-\alpha_1 = \alpha_2 + \cdots + \alpha_q,
$$

したがって $(-\alpha_1|\alpha_2 + \cdots + \alpha_q) > 0$ なので、$(\alpha_1|\alpha_j) < 0$ となるような $j \in \{2, q\}$ が存在します。 証明、$\alpha_1 + \alpha_j \in P$、関係 $(\alpha_1 + \alpha_j) + \sum_{i \neq 1, j} \alpha_i = 0$ 矛盾する帰納法の仮定の部分 1) によって。

3) すべての $\alpha \in P$ に対して $(\gamma|\alpha) \geqslant 0$ となるような、$V$ に非ゼロの元 $\gamma$ が存在することを示します。そうでない場合、1) の結果は、$P$ の元の無限の数列 $\alpha_1, \alpha_2, \ldots$ が次のように見つかる可能性があることを示します。
$$
\beta_i = \alpha_1 + \cdots + \alpha_i \in P
$$
すべての$i$; $\beta_i = \beta_j$ となるような 2 つの相異なる整数 $i, j$ が存在することになり、これは 2) の結果と矛盾します。

4) この命題を証明するには、$V$ の基底 $(\alpha_k)_{1 \leq k \leq l}$ が存在し、この基底によって定義される辞書編集順序では、$P$ のすべての要素が $> 0$ であることを示すだけで十分です。 $l = \dim V$ で帰納法まで進み、すべての次元 $< l$ に対して命題が成立すると仮定します。 $\gamma \in V$ を、すべての $\alpha \in P$ (cf. 3)) に対して $\gamma \neq 0$ および $(\gamma|\alpha) \geqslant 0$ となるようにします。 $L$を$\gamma$と直交する超平面、$R \cap L$で生成された$L$の$V'$部分空間とする。 すると、$R \cap L$は$V'$の根系で、$P \cap L$は$R \cap L$で閉じられます。 帰納法仮説により、$V'$ の基底 $(\beta_1, \ldots, \beta_{l'})$ が存在し、この基底によって定義される辞書編集順序では $P \cap L$ の要素が $> 0$ になります。 次に、最初の $l' + 1$ 元が $\gamma, \beta_1, \ldots, \beta_{l'}$ で、残りの元が $L$ にある $V$ の基底は、必要な性質を持ちます。

#### 命題 23 {#lie-vi-s1-prop-23 .statement tag=0AVX}

*$P$ を $R$ と $V_1$ (それぞれ $\Gamma$) 、$P$ によって生成された $V$ のベクトル部分空間 (それぞれサブグループ) とします。 次の条件は同等です:*

(i) *P は閉じており対称です。*
(ii) *P は閉じており、P は $V_1$ の根系;*
(iii) $\Gamma \cap R = P$。

※これら条件は満たされているものとします。任意の $\alpha \in P$ について、$\alpha_1 \tilde{}$ を $\alpha \tilde{}$ ～ $V_1$ の制限とします。したがって、写像 $\alpha \mapsto \alpha_1 \tilde{}$ は、根系 $P$ から $P \tilde{}$ までの正規の全単射です。*

(iii) $\Longrightarrow$ (i): クリア。

(i) $\Longrightarrow$ (ii): $P$ が閉じていて対称であると仮定します。まず、$P$は$V_1$の(RS_I)を満たします。 $\alpha, \beta \in P$ の場合、$s_\alpha(\beta) \in P$ であることがわかります。 $\alpha$ と $\beta$ が比例する場合、これは明らかです。それ以外の場合、0 から $n(\beta, \alpha)$ までのすべての有理数整数 $p$ に対して $s_\alpha(\beta) = \beta - n(\beta, \alpha)\alpha$ と $\beta - p\alpha \in R$ (提案 9、no. 3)、
$$
\beta - n(\beta, \alpha)\alpha \in P
$$
$P$ は閉じていて対称であるため。したがって、$s_{\alpha, \alpha_1}(P) = P$ と $P$ は (RS_{II}) を満たします。 $P$ が (RS_{III}) を満たすことは明らかです。したがって、$P$ は (ii) を満たし、同時に命題の最後の主張が証明されました。

(ii) $\Longrightarrow$ (iii): 条件 (ii) が満たされる場合、$\Gamma \cap R = P$ であることを示します。 $P \subseteq \Gamma \cap R$であることは明らかです。 $\beta \in \Gamma \cap R$ にしましょう。 $\beta \in \Gamma$と$P = -P$なので、$\beta = \alpha_1 + \alpha_2 + \cdots + \alpha_k$と$\alpha_1, \ldots, \alpha_k \in P$。 $\beta \in P$ を証明しましょう。 $k = 1$であればこれはクリアです。 $k$の帰納法までに議論します。私たちは持っています

$$
0 < (\beta|\beta) = \sum_{i=1}^{k} (\beta|\alpha_i),
$$
したがって、添字 $i$ の場合は $(\beta|\alpha_i) > 0$ です。 $\beta = \alpha_i$なら$\beta \in P$。それ以外の場合、$\beta - \alpha_i \in R$ (Th. 1 の Cor.、no. 3) なので、帰納法の仮定までの$\beta - \alpha_i \in P$、したがって、$P$ が閉じているので、$\beta \in P$ になります。

提案23の条件は、$V_1 = V$でも$P \neq R$でも実現できます。たとえば、これは、$R$ が型 $G_2$ の系および型 $A_2$ の $P$ 系である場合に当てはまります。 cf. プレートX。

#### 命題 24 {#lie-vi-s1-prop-24 .statement tag=0AVY}

*$R'$ を $R$ の共通部分と $V$ のベクトル部分空間とすると、$R'$ はベクトル部分空間 $V'$ の根系になります。 生成する (cf. 提案 4 の修正、no. 1)。 $B'$ を $R'$ の基底とします。*

(i) *$R$ 含む $B'$ のうち基底が存在します。*
(ii) *$R'$ は、$B'$ の元の線形結合である $R$ の元の集合です。

主張 (ii) は明らかです。 (i) を証明します。 $(\varepsilon_1, \varepsilon_2, \ldots, \varepsilon_l)$ を $V$ の基底として、$B' = (\varepsilon_{p+1}, \varepsilon_{p+2}, \ldots, \varepsilon_l)$ とします。 $V$ 対応するの辞書編集位数から、この基底定義する $R$ の室 $C$ まで。 $B'$ のすべての元が $R_+(C)$ で最小であることは明らかです。したがって$B' \subseteq B(C)$。

### 8. 最高根

#### 命題 25 {#lie-vi-s1-prop-25 .statement tag=0AVZ}

※$R$は既約であると仮定します。 $C$ を $R$ の部屋とし、$B(C) = \{\alpha_1, \ldots, \alpha_l\}$ を対応する基底とします。*

(i) *根 $\tilde{\alpha} = \sum_{i=1}^{l} n_i \alpha_i$ が存在し、根 $\sum_{i=1}^{l} p_i \alpha_i$ ごとに $n_1 \geq p_1, n_2 \geq p_2, \ldots, n_l \geq p_l$ が存在します。他の語では、$R$ は、$C$ で定義された順序に対して最大の元を持ちます。*
(ii) *$\tilde{\alpha} \in \overline{C}$があります*。
(iii) *根 $\alpha$ ごとに $(\tilde{\alpha}|\tilde{\alpha}) \geq (\alpha|\alpha)$ があります。*
(iv) *$\tilde{\alpha}$ に比例しないすべての正の根 $\alpha'$ については、$n(\alpha', \tilde{\alpha}) = 0$ または $1$ になります。*

1) $\alpha = \sum_{i=1}^{l} n_i \alpha_i$、$\beta = \sum_{i=1}^{l} p_i \alpha_i$ を、$C$ で定義される順序の 2 つの最大値根とします。 (i) が成立する $\alpha = \beta$ を証明します。

2) ある添字 $i$ に対して $(\alpha|\alpha_i) < 0$ であれば、$\alpha + \alpha_i \in R$ か $\alpha = -\alpha_i$ (Th. 1, no. 3 の相関) のどちらかになることになり、両方の可能性は $\alpha$ の最大値によって不合理になります。したがって、すべての $i$ に対して $(\alpha|\alpha_i) \geq 0$ となります。

3) $\alpha < 0$ の場合、$\alpha < -\alpha$ ですが、これは不合理です。したがって、すべての $i$ に対して $n_i \geq 0$ となります。 $J$ を $n_i > 0$ となるように $i$ の集合とし、$J'$ を $\{1, 2, \ldots, l\}$ の $J$ の補数とします。続いて$J \neq \varnothing$。 $J'$ が空でない場合、$(\alpha_i|\alpha_{i'}) < 0$ のような $i \in J$ と $i' \in J'$ が存在します (提案 20 の Cor. 5、no. 7)。そうすれば私たちはそうするでしょう

$$(\alpha | \alpha_{i'}) = \sum_{i \in I} n_i (\alpha_i | \alpha_{i'}) < 0$$

$(\alpha_j | \alpha_k) \leq 0$ 以降、$j$ と $k$ が異なる場合は常に、2) と矛盾します。したがって、すべての $i$ に対して $J' = \varnothing$ と $n_i > 0$ が対応します。

4) 2) までに、すべての $i$ に対して $(\beta | \alpha_i) \geq 0$ が得られます。 できないは、$\beta \neq 0$ 以降のすべての $i$ に対して $(\beta | \alpha_i) = 0$ を持っています。 3) から推測すると、

$$(\beta | \alpha) = \sum_i n_i (\beta | \alpha_i) > 0.$$

$\gamma = \alpha - \beta \in \mathbf{R}$ の場合、$\alpha > \beta$ または $\beta > \alpha$ (Th. 3、no. 6)、$\alpha$ と $\beta$ の最大値である矛盾する。したがって、$\alpha = \beta$ (Th. 1 のコル、no. 3)。

5) 2) までに、$\tilde{\alpha} \in \overline{C}$。 $\alpha' \in \mathbf{R}$ごとに$(\alpha' | \alpha') \leq (\tilde{\alpha} | \tilde{\alpha})$を証明します。 $\overline{C}$ は $W(\mathbf{R})$ の基本領域であるため、$\alpha' \in \overline{C}$ と仮定できます。 $\tilde{\alpha} - \alpha' \geq 0$ があるので、すべての $x \in \overline{C}$ に対して $(\tilde{\alpha} - \alpha' | x) \geq 0$ になります。特に $(\tilde{\alpha} - \alpha' | \tilde{\alpha}) \geq 0$ と $(\tilde{\alpha} - \alpha' | \alpha') \geq 0$ なので、$(\tilde{\alpha} | \tilde{\alpha}) \geq (\alpha' | \tilde{\alpha}) \geq (\alpha' | \alpha')$ になります。したがって、$\alpha'$ が $\tilde{\alpha}$ に比例しない場合、$n(\alpha', \tilde{\alpha})$ は 0、1、または -1 に等しくなければなりません。 $\alpha' \geq 0$ の場合、$(\tilde{\alpha} | \alpha') \geq 0$ by 2) なので、$n(\alpha', \tilde{\alpha}) \geq 0$ と $n(\alpha', \tilde{\alpha})$ は 0 または 1 でなければなりません。

#### 注意 {#lie-vi-s1-n8-rem-1 .statement tag=0AW0}

根

$$\tilde{\alpha} = \sum_i n_i \alpha_i$$

(i) は、($C$ に関して) $\mathbf{R}$ の最高根であると言われています。 (i) により、すべての $i$ に対して $n_i \geq 1$ が得られることに注意してください。

### 9. 重み、根基重み

$l = \dim V$ にしましょう。 $\mathbf{R}$ によって生成された $V$ の $Q(\mathbf{R})$ 部分群で表します。 $Q(\mathbf{R})$の元は、$\mathbf{R}$の根基、重みと呼ばれます。 Thさんよりno. 6 の 3、$Q(\mathbf{R})$ は、階数 $l$ の $V$ の離散部分群であり、$\mathbf{R}$ のすべての基底は、$Q(\mathbf{R})$ の基底です。

同様に、群 $Q(\mathbf{R}^*)$ は、階数 $l$ の $V^*$ の離散部分群です。

#### 命題 26 {#lie-vi-s1-prop-26 .statement tag=0AW1}

*すべての $y^* \in Q(\mathbf{R}^*)$ (または同等に、すべての $y^* \in \mathbf{R}^*$) の $\langle x, y^* \rangle \in \mathbf{Z}$ が $V$ 含む $Q(\mathbf{R})$ の離散部分群 $G$ となるような $x \in V$ の集合。 $B'$ が $\mathbf{R}^*$ の基底である場合、$B'$ の$V$ の基底は、$G$* の基底です。

$x \in V$ にしましょう。次の 3 つのプロパティは同等です。

(i) $y^* \in Q(\mathbf{R}^*)$ 全員に対して $\langle x, y^* \rangle \in \mathbf{Z}$;
(ii) $y^* \in B'$ 全員に対して $\langle x, y^* \rangle \in \mathbf{Z}$。
(iii) $B'$の双対基底に対する$x$の座標は$\mathbf{Z}$にあります。

これから、$B'$ に対する基底の双対は、$G$ の基底であると推測します。一方、(RSIII) は $\mathbf{R} \subseteq G$ であるため、$Q(\mathbf{R}) \subseteq G$ であることを証明します。

提案26の群 $G$は$P(\mathbf{R})$で表され、その元は$\mathbf{R}$の重みと呼ばれます。 $\mathbf{R}^*$の重みの群$P(\mathbf{R}^*)$も考慮できます。

$$
P(R)/Q(R), \quad P(\tilde{R})/Q(\tilde{R})
$$

は $\mathbf{Q}/\mathbf{Z}$ を超える双対性で有限群であるため、同型です。これら 2 つの群のうち共通の位数は、R (または $\tilde{R}$) の *接続添字* と呼ばれます。

R が根系 $R_i$ の直和である場合、群 Q(R) (または P(R)) は Q($R_i$) (または P($R_i$)) の直和と標準的に識別されます。

#### 命題 27 {#lie-vi-s1-prop-27 .statement tag=0AW2}

※$R_1$をRの部分集合、$R_1$で生成されたQ(R)の$Q_1$部分群、$s_\alpha$($\alpha \in R_1$)で生成されたW(R)の$W_1$部分群とします。 $p \in P(R)$ と $w \in W_1$ の場合、$p - w(p) \in Q_1$。*

$w = s_\alpha$ と $\alpha \in R_1$ の場合、

$$
p - w(p) = \langle p, \alpha^\vee \rangle \alpha \in \mathbf{Z}\alpha \subseteq Q_1.
$$

$w = s_{\alpha_1} s_{\alpha_2} \ldots s_{\alpha_r}$ が $\alpha_1, \ldots, \alpha_r \in R_1$ である場合でも、r の帰納法で分かるように、$p - w(p) \in Q_1$ は依然として真です。

群 A(R) は P(R) と Q(R) を不変のままにするため、商 P(R)/Q(R) に作用します。提案 27 により、群 W(R) は P(R)/Q(R) に対して自明に作用します。 移行から商を見ると、*剰余群* A(R)/W(R) (cf. 提案 16、no. 5) が *P(R)/Q(R) に *標準的に作用する*ことがわかります。

### 10. ファンダメンタル重み、ドミナント重み

R が *還元*されると仮定します。 C を R の部屋、B を R の対応する基底とします。R は還元されるので、$B^\vee = \{ \alpha^\vee \}_{\alpha \in B}$ は $R^\vee$ の基底です。したがって、$B^\vee$ の *双対基底* $(\overline{\omega}_\alpha)_{\alpha \in B}$ は、重みの群の基底です。その元は *基本重み* (B または C に対して) と呼ばれます。 Bの元が$(\alpha_1, \ldots, \alpha_l)$で表される場合、対応するの基本波重みは$(\overline{\omega}_1, \ldots, \overline{\omega}_l)$で表されます。

$x \in V$ にしましょう。次に、すべての $\alpha \in B$ に対して $\langle x, \alpha^\vee \rangle > 0$ である場合に限り、$x \in C$ になります。したがって、C は係数 $\geq 0$ を含む $\overline{\omega}_\alpha$ の線形結合の集合です。

カルタン行列のエントリ $n(\alpha, \beta) = \langle \alpha, \beta^\vee \rangle$ は、固定 $\alpha$ の場合、基底 $(\overline{\omega}_\beta)_{\beta \in B}$ に関する $\alpha$ の座標です。

$$
\alpha = \sum_{\beta \in B} n(\alpha, \beta) \overline{\omega}_\beta.
$$

したがって、カルタン行列は、標準単射の行列の転置です。

$$
Q(R) \to P(R)
$$

$\mathbf{Z}$ モジュール Q(R) および P(R) の基底 B および $(\overline{\omega}_\alpha)_{\alpha \in B}$ に関して。

A weight $\overline{\omega}$ is said to be *dominant* if it belongs to $\overline{C}$, in other words if its coordinates with respect to $(\overline{\omega}_\alpha)_{\alpha \in B}$ are integers $\geq 0$, or equivalently if $g(\overline{\omega}) \leq \overline{\omega}$ for all $g \in W(R)$ (no. 6, Prop. 18). $\overline{C}$ は $W(R)$ (Th. 2) の基本領域であるため、任意の重み $\overline{\omega}$ に対して、$\overline{\omega}'$ が $\overline{\omega}$ × $W(R)$ の変換であるような固有の重み $\overline{\omega}'$ が存在します。

私たちは持っています
$$
\langle \overline{\omega}_\alpha, \beta^\vee \rangle = (\overline{\omega}_\alpha | \frac{2\beta}{(\beta|\beta)}) = \delta_{\alpha\beta}
$$
$\alpha, \beta \in B$ ($\delta_{\alpha\beta}$ はクロネッカー記号を示す) の場合、
$$
s_\beta(\overline{\omega}_\alpha) = \overline{\omega}_\alpha - \delta_{\alpha\beta}\beta \quad \text{and} \quad (\overline{\omega}_\alpha |\beta) = \frac{1}{2}(\beta|\beta)\delta_{\alpha\beta}.
$$
他の語では、$\overline{\omega}_\alpha$ は *$\beta \neq \alpha$ に対して * $\beta$ に直交し、* $R\alpha$ に直交する射影 * は * $\frac{1}{2}\alpha$ です。 $\overline{\omega}_\alpha \in \overline{C}$ なので、$\alpha, \beta \in B$ に対して $(\overline{\omega}_\alpha |\overline{\omega}_\beta) \geqslant 0$、つまり角度 $(\overline{\omega}_\alpha, \overline{\omega}_\beta)$ は鋭角または直角です。支配的な重みは$\overline{\omega} \in V$で、$2(\overline{\omega}|\alpha)/(|\alpha|\alpha)$はすべての$\alpha \in B$に対して整数$\geqslant 0$になります。

#### 命題 28 {#lie-vi-s1-prop-28 .statement tag=0AW3}

*$B$ *を基* $R$、$B'$ *のサブセット* $B$、$V'$ *のベクトル部分空間* $V$ *によって生成* $B'$、$R' = R \cap V'$ *(これは* $V'$*のルートシステムです)、* $R'\tilde{}$ *逆根系 (* $R'$ *in* $R'\tilde{}$ の正準イメージで識別されます)、$V_1$ * の直交補数* $R'\tilde{}$ *in* $V$、*および* $p$ *射影* $V$ *上* $V'$ *平行* $V_1$。 *それでは* $Q(R') = Q(R) \cap V'$、$P(R') = p(P(R))$。 *支配的な重みのセット* $R'$ *は、* $R$ の支配的な重みのセットの* $p$ の下にある画像です。

確かに、$Q(R)$ は基底 $B$ を伴う $V$ の部分群であり、$Q(R')$ は基底 $B'$ を伴う $V'$ の部分群です (no. 7、提案 20 の Cor. 4)。 $Q(R') = Q(R) \cap V'$は明らかです。 $\overline{\omega} \in P(R)$ と $\alpha \in R'$ の場合、$\langle p(\overline{\omega}), \alpha^\vee \rangle = \langle \overline{\omega}, \alpha^\vee \rangle \in \mathbf{Z}$、つまり $p(\overline{\omega}) \in P(R')$、したがって $p(P(R)) \subseteq P(R')$ になります。 $\overline{\omega}' \in P(R')$、$\overline{\omega}'$ 拡大するから線型形式 $\overline{\omega}$ が $V^*$ で$(B - B')\tilde{}$ に消えた場合。すべての $\alpha \in B$ に対して $\langle \overline{\omega}, \alpha^\vee \rangle \in \mathbf{Z}$ があるため、$\overline{\omega} \in P(R)$ と $\overline{\omega}' = p(\overline{\omega})$ になります。したがって$P(R') \subseteq p(P(R))$です。 したがって、優勢な重みに関する$P(R') = p(P(R))$、主張も同様に証明されます。

#### 命題 29 {#lie-vi-s1-prop-29 .statement tag=0AW4}

*$\rho$ *を根* $> 0$ の半分和とします。

(i) $\rho = \sum_{\alpha \in B} \overline{\omega}_\alpha$; *これは* $C$ の元です。
(ii) $s_\alpha(\rho) = \rho - \alpha$ *全員に* $\alpha \in B$。
(iii) $(2\rho|\alpha) = (\alpha|\alpha)$ *全員に* $\alpha \in B$。

$R$ が減らされるので、$\alpha \in B$ に対して $s_\alpha(R_+(C) - \{\alpha\}) = R_+(C) - \{\alpha\}$ と $s_\alpha(\alpha) = -\alpha$ (no. 6、提案 17 の修正 1)、つまり $s_\alpha(2\rho) = 2\rho - 2\alpha$ になります。 $s_\alpha(\rho) = \rho - \langle \rho, \alpha^\vee \rangle$ 以降、次のことがわかります。
$$
\langle \rho, \alpha^\vee \rangle = 1 = \langle \sum_{\beta \in B} \overline{\omega}_\beta, \alpha^\vee \rangle.
$$
従って、$\rho = \sum_{\beta} \overline{\omega}_\beta$、その結果、$\rho \in C$になります。最後に、(iii) は$\langle \rho, \alpha^\vee \rangle = 1$ に相当します。

#### 系 {#lie-vi-s1-n10-cor-1 .statement tag=0AW5}

$\sigma$ を元 $> 0$ の $R^-$ の半分和とします ($B^-$ の場合)。 基底 $B$ に対する$\alpha$ の座標のすべての $\alpha \in V$、和は $\langle \alpha, \sigma \rangle$ です。 $\alpha \in R$ の場合、この和は $\frac{1}{2} \sum_{\beta \in R_+ (\mathbf{C})} n(\alpha, \beta)$ に等しいです。

交換すること上記の $R$ と $R^-$ の役割では、すべての $\alpha \in B$ に対して $\langle \alpha, \sigma \rangle = 1$ があり、したがって系になります。

### 11. コクセター変換

$C$ を $R$ の部屋とし、$\{ \alpha_1, \ldots, \alpha_l \}$ を $R$ の対応する基底とし、$c = s_{\alpha_1} \cdots s_{\alpha_l}$ とします。 The element $c$ of $W$ is called the *Coxeter transformation* of $W$ defined by $C$ and the bijection $i \mapsto \alpha_i$ (Chap. V, § 6, no. 1). その位数 $h$ は、$W$ (または $R$) の *Coxeter 数* と呼ばれます。

#### 命題 30 {#lie-vi-s1-prop-30 .statement tag=0AW6}

※$R$は既約であると仮定します。 $m$ を 1 と $h - 1$ の間の整数とし、$h$ まで素数とします。すると、$\exp(\frac{2i\pi m}{h})$ は重複度 1 の $c$ の固有値になります。*

特に、$m$ は、$W$、cf. 章の *指数* です。 V, § 6, no. 2。

まず補題を証明します。

#### 補題 4 {#lie-vi-s1-lem-4 .statement tag=0AW7}

*すべての $w \in W$ について、$w$ の特性多項式は整数係数になります。*

$\{ \alpha_1, \ldots, \alpha_l \}$ は、$R$ によって生成された $V$ の部分群 $Q(R)$ の基底であることがわかっています (no. 6、Th. 3)。 $w$ は $Q(R)$ を安定したままにするため、$\{ \alpha_1, \ldots, \alpha_l \}$ に関するその行列には整数のエントリがあります。従って、その特性多項式は整数係数になります。

$P$ を $c$ の特性多項式とします。 上の補題は、$P$の係数が整数であることを示しています。 章著。 V, § 6, no. 2、コル。提案 3 の 2、単位元 $z = \exp(\frac{2i\pi}{h})$ の原始 $h$ 番目根は、$P$ の単純な根です。 したがって、$\mathbf{Q}$ 上の $z$ のすべての *共役* は、$P$ の単純な根でもあります。 しかし、私たちは (*代数*、章 V)、統一の原始 $h$ 根が $\mathbf{Q}$ 上で共役であることを知っています。 したがって、それらはすべて単純な $P$ の根であり、命題が証明されます。

#### 命題 31 {#lie-vi-s1-prop-31 .statement tag=0AW8}

※$R$が既約、約分であるとして、$\beta = n_1 \alpha_1 + \cdots + n_l \alpha_l$を$R$(cf.no. 8)の最高根とする。次に、$n_1 + \cdots + n_l = h - 1$.*

$R_+$ を $C$ に対して正の根の集合とします。次に (no. 10、提案 29 の修正):

$$
n_1 + \cdots + n_l = \frac{1}{2} \sum_{\alpha \in R_+} n(\beta, \alpha)
$$
$$
= 1 + \frac{1}{2} \sum_{\alpha \in R_+, \alpha \neq \beta} n(\beta, \alpha) = 1 + \sum_{\alpha \in R_+, \alpha \neq \beta} \frac{(\alpha | \beta)}{(\alpha | \alpha)}
$$

no. 8、提案 25 (iv) により、すべての $\alpha \in R_+$ と $\alpha \neq \beta$、$n(\alpha, \beta) = 0$ または 1 について、$n(\alpha, \beta)^2 = n(\alpha, \beta)$、つまり $\frac{4(\alpha | \beta)^2}{(\beta | \beta)^2} = \frac{2(\alpha | \beta)}{(\beta | \beta)}$ になります。したがって、次のようになります。

$$
n_1 + \cdots + n_l + 1 = 2 + 2 \sum_{\alpha \in R_+, \alpha \neq \beta} \frac{(\alpha | \beta)^2}{(\alpha | \alpha)(\beta | \beta)}
= 2 \sum_{\alpha \in R_+} \frac{(\alpha | \beta)^2}{(\alpha | \alpha)(\beta | \beta)} = (\beta | \beta)^{-1} \sum_{\alpha \in R} \left( \frac{\alpha}{\| \alpha \|} | \beta \right)^2.
$$

章著。 V, § 6, no. 2、コル。 Thの。 1、

$$
\sum_{\alpha \in R} \left( \frac{\alpha}{\| \alpha \|} | \beta \right)^2 = h(\beta | \beta)
$$

だから$n_1 + \cdots + n_l + 1 = h$。

#### 命題 32 {#lie-vi-s1-prop-32 .statement tag=0AW9}

*R は既約であり、すべての根は同じ長さを持つと仮定します。 $\alpha \in R$ にしましょう。 $\alpha$と直交しないRの元の数は$4h - 6$です*。

$R'$ を $\alpha$ に比例せず、直交しない根の集合とします。
章著。 V, § 6, no. 2、コル。 Thの。 1、

$$
(\alpha | \alpha)^2 + (\alpha | -\alpha)^2 + \sum_{\beta \in R'} (\alpha | \beta)^2 = h(\alpha | \alpha)^2,
$$

つまり

$$
\sum_{\beta \in R'} (\alpha | \beta)^2 = (h - 2)(\alpha | \alpha)^2.
$$

$\beta \in R'$ の場合は、no. 3 のリストに従って $(\alpha | \beta) = \pm \frac{1}{2} (\alpha | \alpha)$ になります。したがって、

$$
\frac{1}{4} \operatorname{Card} R' = h - 2, \quad \operatorname{Card} R' = 4h - 8,
$$

そして、$\alpha$と直交しない根の数は$\operatorname{Card} R' + 2 = 4h - 6$です。

#### 命題 33 {#lie-vi-s1-prop-33 .statement tag=0AWA}

※Rは既約で還元されるものとします。 $s_{\alpha_i} = s_i$ を置き、$\Gamma$ を $c = s_1 \ldots s_l$ によって生成された W の部分群とします。*

(i) *$\theta_i = s_l s_{l-1} \ldots s_{i+1} (\alpha_i)$ ($i = 1, \ldots, l$) とします。次に、$\theta_i > 0, c(\theta_i) < 0$.*
(ii) *$\alpha$ が $c(\alpha) < 0$ となるような根 $> 0$ である場合、$\alpha$ は $\theta_i$ の 1 つに等しい。*
(iii) *家族$(\theta_i)_{1 \leq i \leq l}$はQ(R)の基底です。*
(iv) *$\Omega_i$を$\Gamma$の下の$\theta_i$の軌道とします。 集合 $\Omega_i$ はペアごとに互いに素であり、それらはすべて R 上の $\Gamma$ の軌道であり、それぞれ h 元を持ちます。*

Observe first that $(s_1, \ldots, s_l)$ is a *reduced decomposition* of $c$ (Chap. IV, § 1, no. 1) with respect to the set S of the $s_i$. 確かに、そうでなければ、$c \in W_X$ となるような S の $l - 1$ 元の部分集合 $X = S - \{ j \}$ が存在し、Cor と矛盾します。第 2 章の提案 7 の 2 IV, § 1, no. 8。

適用コル。 no. 6 から$c$ までの提案 17 の 2 は、主張 (i) と (ii) を与えます。

$Q_i$を$\alpha_j, j > i$によって生成されたQ(R)の部分群とします。 $Q_i$が$s_j, j > i$で安定しているのが明らか、その$s_j (\alpha_i) = \alpha_i$がMODです。 $Q_i$ は $j > i$ です。
したがって、次のようになります。

$$
\theta_i = s_l \ldots s_{i+1} (\alpha_i) = \alpha_i \text{ mod. } Q_i.
$$

他の語には、次のような整数 $c_{ij}$ が存在します。
$$
\theta_i = \alpha_i + \sum_{j > i} c_{ij} \alpha_j.
$$
部分 (iii) がすぐに続きます。

最後に、$\alpha$を根とします。 The element $\sum_{k=0}^{h-1} c^k(\alpha)$ is invariant under $c$, and hence zero (Chap. V, § 6, no. 2). したがって、$c^k(\alpha)$ できないはすべて同じ符号を持ち、$c^k(\alpha) > 0$ と $c^{k+1}(\alpha) < 0$ のような $k$ が存在します。 (ii) により、$c^k(\alpha)$ は $\theta_i$ の 1 つになります。 したがって、$R$ 上の $\Gamma$ のすべての軌道は、$\Omega_i$ の 1 つになります。 $V \otimes \mathbf{C}$ の拡大する $(x|y)$ からエルミート形まで。 $R$ の $\Gamma$ のそれぞれの軌道には最大 $h$ 元があり、上記の注意によって異なる軌道は最大 $l$ です。 ここで (V, § 6, no. 2 章、定理 2、ii))、$R$ の基数は $hl$ に等しく、これは直ちに (iv) を意味します。

### 12. 正規双線形形式

(no. 1、提案 3) は対称双線形形式であることを見てきました。
$$
(x, y) \mapsto B_R(x, y) = \sum_{\alpha \in R} \langle \alpha^*, x \rangle \langle \alpha^*, y \rangle
$$
$V$ では非縮退であり、$A(R)$ では不変です。 交換すること $R$ と $R^*$ の役割を考慮すると、$V^*$ 上の対称双線形形式 $(x^*, y^*) \mapsto B_{R^*}(x^*, y^*) = \sum_{\alpha \in R} \langle \alpha, x^* \rangle \langle \alpha, y^* \rangle$ は$A(R)$ では非縮退で不変であることがわかります。

$V$ (それぞれ $V^*$) 上の $B_{R^*}$ (それぞれ $B_R$) の逆形式は、$V$ (それぞれ $V^*$) 上の *正準双線形形式* と呼ばれ、$\Phi_R$ (それぞれ $\Phi_{R^*}$) で表されます。 $A(R)$ では非縮退で不変です。 $\sigma$ を $V$ から $V^*$ までの $B_{R^*}$ で定義される同型とします。 次に、$x \in V$ と $y \in V$ については次のようになります。
$$
\Phi_R(x, y) = B_{R^*}(\sigma(x), \sigma(y)) = \sum_{\alpha \in R} \langle \alpha, \sigma(x) \rangle \langle \alpha, \sigma(y) \rangle.
$$
でも$\langle \alpha, \sigma(x) \rangle = B_{R^*}(\sigma(\alpha), \sigma(x)) = \Phi_R(\alpha, x)$。 したがって、
$$
\Phi_R(x, y) = \sum_{\alpha \in R} \Phi_R(\alpha, x) \Phi(\alpha, y).
$$
(16)
no. 2 の提案 7 を考慮すると、$\Phi_R$ は、恒等式 (16) を満たす、$W(R)$ の下で唯一の非ゼロ対称双線形形式不変量です。

$\beta \in R$ の場合、(16) は次のようになります。
$$
\Phi_R(\beta, \beta) = \sum_{\alpha \in R} \Phi_R(\alpha, \beta)^2 = \frac{1}{4} \Phi_R(\beta, \beta)^2 \sum_{\alpha \in R} n(\alpha, \beta)^2,
$$
したがって
$$
4 \Phi_R(\beta, \beta)^{-1} = \sum_{\alpha \in R} n(\alpha, \beta)^2.
$$
さらに、no. 1 の補題 2 により、$x, y \in V$ については次のようになります。

$$
B_R(x, y) = \sum_{\alpha \in R} \Phi_R \left( \frac{2\alpha}{\Phi_R(\alpha, \alpha)}, x \right) \left( \frac{2\alpha}{\Phi_R(\alpha, \alpha)}, y \right)
= 4 \sum_{\alpha \in R} \Phi_R(\alpha, x) \Phi_R(\alpha, y) \Phi_R(\alpha, \alpha)^{-2}.
$$

したがって、$R$ が *既約* である場合、次のような定数 $\gamma(R) > 0$ が存在します。

$$
\sum_{\alpha \in R} \Phi_R(\alpha, x) \Phi_R(\alpha, y) \Phi_R(\alpha, \alpha)^{-2} = \gamma(R) \Phi_R(x, y).
$$ (18)

$\gamma(R)$ の定義までに $B_R(x, y) = 4\gamma(R) \Phi_R(x, y)$ になりますので、

$$
\Phi_{R^{\sim}}(x^*, y^*) = (4\gamma(R))^{-1} B_{R^{\sim}}(x^*, y^*)
$$

$x^*, y^* \in V^*$の場合。これは、$\gamma(R) = \gamma(R^{\sim})$ であることを証明します。一方、$\beta \in R$の場合は、

$$
\Phi_{R^{\sim}}(\beta^{\sim}, \beta^{\sim}) = (4\gamma(R))^{-1} \sum_{\alpha \in R} \langle \beta^{\sim}, \alpha \rangle^2
= \gamma(R)^{-1} \sum_{\alpha \in R} \frac{\Phi_R(\alpha, \beta)^2}{\Phi_R(\beta, \beta)^2}
$$

したがって、(16) により、

$$
\Phi_{R^{\sim}}(\beta^{\sim}, \beta^{\sim}) = \gamma(R)^{-1} \Phi_R(\beta, \beta)^{-2} \Phi_R(\beta, \beta)
$$

それとも最後に

$$
\Phi_R(\beta, \beta) \Phi_{R^{\sim}}(\beta^{\sim}, \beta^{\sim}) = \gamma(R)^{-1}.
$$ (19)

さらに、$R$ のすべての根が $\Phi_R$ に対して同じ長さ $\lambda$ を持つ場合、(16) と (18) は次のことを示します。

$$
\gamma(R) = \lambda^{-4}.
$$ (20)

さらに、$h$ が $W$ の Coxeter 数である場合、Cor. Thの。第1章V, § 6, no. 2 は次のことを示しています。

$$
h \Phi_R(x, x) = \sum_{\alpha \in R} \left( x, \frac{\alpha}{\lambda} \right)^2 \text{ for all } x \in V.
$$

(16) と比較すると、次のように推測されます。

$$
\lambda = h^{-1/2} \quad \text{or} \quad \gamma(R) = h^2.
$$ (21)

最後に、公式 (19) は、$R^{\sim}$ の根が $\Phi_{R^{\sim}}$ に対して長さ $\lambda$ を持っていることを示しています。

### 練習問題 {#lie-vi-s1-exercises}

以下で考慮されるすべての根系は、実際のベクトル空間と相対的です。ワイル群 (cf. no. 3) の下でスカラー 積不変量を $(x|y)$ で表します。

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
