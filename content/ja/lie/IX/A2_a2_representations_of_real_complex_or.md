---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 2
section_title: Representations of real, complex or quaternionic type
appendix: true
lang: ja
source: lie-vii-ix
book_pages: 385-388
pdf_pages: 0392-0395
extraction: native
subsections:
    - "no": 1
      title: REPRESENTATIONS OF REAL ALGEBRAS
      page: 385
      pdf_page: 392
    - "no": 2
      title: REPRESENTATIONS OF COMPACT GROUPS
      page: 387
      pdf_page: 394
statements: 6
exercises: 0
content_sha256: 21064d5486268e466878b47a8f6e91828d50f95f7bcbe3e96043009d27731335
translated_from: content/en/lie/IX/A2_a2_representations_of_real_complex_or.md
translation_method: google
source_content_sha256: 166c8e4a3ff2601758b90e2cbc28e90c5ad2ac9dc57f18a2eb1d30f70fa6ca87
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 69f437a9f9c1aa3d7d056e0b233bb1cf16a9371eca508ff0c12e14bd0f1df985
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 付録 II

# 表現の実数、複素数、または四元数型

### 1. 本物の代数の表現

$\sigma$ 自己同型 $\alpha  \rightarrow \overline{\alpha}$ の $\mathbf{C}$ で表します。 W が複素数ベクトル空間の場合、W で $\mathbf{C}$ ベクトル空間 $\sigma_*(W)$ を表します (つまり、$\alpha \in \mathbf{C}, w\in W$ に対して演算 $(\alpha , w) \rightarrow \overline{\alpha w}$ の法則を含む群 W)。

#### 命題 1 {#lie-ix-a2-prop-1 .statement tag=01IS}

A を $\mathbf{R}$-代数 (結合的および単体)、V を $\mathbf{R}$ 上の有限次元単純A-加群とする。その場合、次の 3 つの状況のいずれかに該当する必要があります。

V (代数、VIII, § 5, no. 1) の $\alpha )$ 交換子環は $\mathbf{R}$ と同型であり、$A_{(\mathbf{C})}$ 加群 $V_{(\mathbf{C})}$ は単純です。

V の $\beta )$ 交換子環は $\mathbf{C}$ と同型です。 $A_{(\mathbf{C})}$ モジュール $V_{(\mathbf{C})}$ は、$\sigma \otimes 1_V$ によって交換される 2 つの非同型単純な $A_{(\mathbf{C})}$ サブモジュールの直和です。

V の $\gamma )$ 交換子環は $\mathbf{H}$ と同型です。 $A_{(\mathbf{C})}$ モジュール $V_{(\mathbf{C})}$ は、$\sigma \otimes 1_V$ によって交換される 2 つの同型の単純な $A_{(\mathbf{C})}$ サブモジュールの直和です。

V の交換子環 E は体、$\mathbf{R}($代数の有限拡大です。 VIII, §3, no. 2、提案 2)、したがって、$\mathbf{R},\mathbf{C}$ または $\mathbf{H}($代数、第 4 章と同型です。 VIII, §15）。 $A_{(\mathbf{C})}$ モジュール $V_{(\mathbf{C})}$ は半単純 (代数、Chap. VIII, §11, no. 4) であり、その交換子環は $\mathbf{C}\otimes_{\mathbf{R}}E ($代数、Chap. と識別できます。 VIII, §11, no. 2、補題 1)。

E が $\mathbf{R}$ と同型の場合、$V_{(\mathbf{C})}$ の交換子環は $\mathbf{C}$ と同型で、$V_{(\mathbf{C})}$ は単純な $A_{(\mathbf{C})}$ 加群になります (代数、VIII, §11, no. 4 章)。

E が $\mathbf{R}$ と同型でない場合、含む体は $\mathbf{C}$ と同型です。したがって、V は $V^c$ で示される $A_{(\mathbf{C})}$ モジュール構造を持つことになります。この場合、$V^c$ は単純な $A_{(\mathbf{C})}$ モジュールであり、$\mathbf{C}$ 線形写像 $\psi : V_{(\mathbf{C})}\rightarrow V^c\oplus \overline{V}^c$ は、$\alpha \in \mathbf{C},v\in V$ に対する $\psi (\alpha \otimes v) =$ $(\alpha v,\overline{\alpha v})$ は同型 (代数、第 3 章) となります。 V, §10, no. 4、提案 8)。さらに、この同型の下の $\sigma \otimes 1_V$ 対応するは、 $V^c\oplus \overline{V}^c$ の $\mathbf{R}$ 自己同型 $(v, v') \rightarrow (v', v)$ になり、したがって 2 つの $A_{(\mathbf{C})}$ サブモジュール $\psi^{-1}(V^c)$ と $\psi^{-1}(V^c)$ が交換されます。

$V_{(\mathbf{C})}$ の交換子環 $E_{(\mathbf{C})}$ したがって、含む $\mathbf{C}\times \mathbf{C}$ は、$V^c\oplus \overline{V}^c$ で相似関係により演算されます。 $V^c$ から $\overline{V}^c$ までの $A_{(\mathbf{C})}$ 加群の同型は、$E_{(\mathbf{C})}$ 簡約するから $\mathbf{C}\times \mathbf{C}$ まで、つまり E が $\mathbf{C}$ と同型である場合にのみ存在します。これで証明は完了です。

#### 命題 2 {#lie-ix-a2-prop-2 .statement tag=01IT}

A を $\mathbf{R}$-代数 (結合的および単体)、W を $\mathbf{C}$ 上の有限次元の単純な $A_{(\mathbf{C})}$-加群とする。その場合、次の 3 つの状況のいずれかに該当する必要があります。

a) W から $\overline{W}$ まで $\theta \circ \theta = 1_W$ との $A_{(\mathbf{C})}$ 同型写像 $\theta$ が存在します。 このとき、$\theta$ の不動点の集合 V は W 上の $\mathbf{R}$ 構造であり、可換項 $\mathbf{R}.1_V$ を持つ単純な A モジュールです。 さらに、$W_{[\mathbf{R}]}$ は 2 つの同型単純A-加群の直和です。

b) $A_{(\mathbf{C})}$ モジュール W と $\overline{W}$ は同型ではありません。その場合、$W_{[\mathbf{R}]}$ は交換子環 $\mathbf{C}.1_W$ を含む単純A-加群になります。

c) W から $\overline{W}$ まで $\theta \circ \theta =-1_W$ との $A_{(\mathbf{C})}$ 同型写像 $\theta$ が存在します。次に、A-加群 $W_{[\mathbf{R}]}$ は単純で、その交換子環は体 $\mathbf{C}.1_W\oplus \mathbf{C}.\theta$ であり、$\mathbf{H}$ と同型です。

複合体ベクトル空間 Hom$_{A_{(\mathbf{C})}}(W,W)$ は、次元 $\leq 1 ($代数、Chap. VIII, §3, no. 2); $\theta \in$ Hom$_{A_{(\mathbf{C})}}(W,W)$ の場合、W の自己準同型 $\theta \circ \theta$ はホモテティー で、比率は $\alpha \in \mathbf{C}$ です。すべての $w\in W$ に対して、$\alpha \theta (w) =\theta \circ \theta \circ \theta (w) =$ $\theta (\alpha w) = \overline{\alpha \theta}(w)$ があるため、$\alpha$ は実数です。 $\theta '=\lambda \theta$ の場合、$\lambda \in \mathbf{C}$ の場合、$\theta '\circ \theta '=|\lambda |^2\theta \circ \theta$。したがって、次の 3 つの可能性のうち 1 つが実現されます。

a) $\theta \in$ Hom$_{A_{(\mathbf{C})}}(W,W)$ と $\theta \circ \theta = 1_W$ が存在します。

b) ホム$_{A_{(\mathbf{C})}}(W,W) =\{0\}$;

c) $\theta \circ \theta =-1_W$ とともに $\theta \in$ Hom$_{A_{(\mathbf{C})}}(W,W)$ が存在します。

In case a), the set V of fixed points of $\theta$ is an $\mathbf{R}$-structure on W (Algebra, Chap. V, p. 61, Prop. 7); since $V_{(\mathbf{C})}$ is isomorphic to W, the A-module V is simple with commutant $\mathbf{R}.1_V$ (Prop. 1), and $W_{[\mathbf{R}]}$ is not simple.

逆に、$W_{[\mathbf{R}]}$ が単純でない場合、V を $W_{[\mathbf{R}]}$ の単純な A-部分加群とします。 $A_{(\mathbf{C})}$ モジュール W は単純なので、$V +iV = W$ と $V\cap iV =\{0\}$、つまり $W = V\oplus iV$ です。従って、V は W 上の $\mathbf{R}$ 構造であり、V の $v$ と $v'$ の $\theta (v+iv') =v-iv'$ が $\theta \circ \theta = 1_W$ を満たすように、W から $\overline{W}$ までの同型 $\theta$ です。

従って、b) と c) の場合、A-加群 $W_{[\mathbf{R}]}$ は単純です。提案 1 によれば、その交換子環 E は、b) の場合は $\mathbf{C}$、c) の場合は $\mathbf{H}$ と同型です。さらに、ケース c) では E 含む $\mathbf{C}.1_W$、および $\mathbf{C}.\theta$、したがって命題であることは明らかです。

命題の仮定では、$A_{(\mathbf{C})}$ 加群 W は、$a),b)$ または c) の場合、それぞれ実数、複素数、または四元数の型 (A に対して) であると言われます。

$K =\mathbf{R}$ または $\mathbf{C}$ については、K 上の有限次元単純な $A_{(K)}$ 加群の類の $\mathfrak{S}_K(A)$ 集合で表します。 群 $\Gamma =$ Gal($\mathbf{C}/\mathbf{R}$) は $\mathfrak{S}_{\mathbf{C}}(A)$ で演算します。前の 2 つの命題は、$\mathfrak{S}_{\mathbf{R}}(A)$ と商集合 $\mathfrak{S}_{\mathbf{C}}(A)/\Gamma$ の間に全単射詞対応を確立します。

### 2. コンパクト群の表現

G をコンパクトなトポロジー 群とし、$\rho : G\rightarrow \mathbf{G}\mathbf{L}(W)$ を有限次元複素数ベクトル空間上の G の連続表現とします。これが (代数 $A =\mathbf{R}^{(G)}$ に対して) $\mathbf{C}^{(G)}$ 加群 W の場合に当てはまる場合、$\rho$ は実数、複素数、または四元数の型の既約であると言えます。 H を W 上の分離正のエルミート形とし、G の下で不変とします。

#### 命題 3 {#lie-ix-a2-prop-3 .statement tag=01IU}

$\rho$ が既約であると仮定します。

a) 表現 $\rho$ は、G の下で不変で、W 上に非ゼロ対称双線形形式 B が存在する場合に限り、実数型になります。この場合、形 B は分離しています。 $w\in W$ の集合 V は、すべての $x\in W$ に対する $H(w, x) = B(w, x)$ が G の下で W 不変量の $\mathbf{R}$ 構造になります。

b) 表現 $\rho$ は、G の下で W 不変量に非ゼロ双線形形式が存在しない場合に限り、複素数型になります。

c) 表現 $\rho$ は、W 上に非ゼロ交代的双線形形式が存在し、G の下で不変である場合に限り、四元数型になります。そのような形は必然的に分離します。

$\theta \in$ ホム$_{\mathbf{C}^{(G)}}(W,W)$ と $x, y\in W$ には、$B_{\theta}(x, y) = H(\theta x, y)$ を入力します。この場合、$B_{\theta}$ は W では双線形形式であり、G の下で不変であり、$\theta$ がゼロ以外の場合は分離されます。 G の下で W 不変量の双線形形式の $\mathscr{B}(W)^G$ 空間で表します。 Hom$_{\mathbf{C}^{(G)}}(W,W)$ から $\mathscr{B}(W)^G$ までの写像 $\theta  \rightarrow B_{\theta}$ は、$\mathbf{C}$ ベクトル空間の同型です。これは、特に主張 b) を意味します。

$\theta$ を、$\alpha \in  \{-1,+1\}$ を伴う $\theta \circ \theta =\alpha_W$ となるような W から $\overline{W}$ までの $\mathbf{C}^{(G)}$ 同型写像とする (提案 2)。 $\mathscr{B}(W)^G$ は次元 1 であるため、次のような $\varepsilon \in \mathbf{C}$ が存在します。

$W$ のすべての $x, y$ に対して $B_{\theta}(y, x) =\varepsilon B_{\theta}(x, y)$。

反復すると、$B_{\theta}(y, x) =\varepsilon B_{\theta}(x, y) =\varepsilon^2B_{\theta}(y, x)$ が得られるため、$\varepsilon^2$ = 1 および $\varepsilon \in  \{-1,+1\}$ となります。また、Wの$x$については、

$$
H(\theta x, \theta x) = B_{\theta}(x, \theta x) =\varepsilon B_{\theta}(\theta x, x) =\varepsilon H(\theta \circ \theta (x), x) =\varepsilon \alpha H(x, x)
$$

H が正なので、$\varepsilon \alpha  >0$、つまり $\varepsilon =\alpha$ です。 主張 a) と c) は提案 2 に従います。

G 上の総質量 1 のハール測度を $dg$ で示します。

#### 補題 1 {#lie-ix-a2-lem-1 .statement tag=01IV}

$W^G$ を G の下で不変な W の部分空間元のからなるとする。W の自己準同型 $\int_G\rho (g)dg$ は像 $W^G$ を持つ射影であり、G の演算と互換性がある。特に、暗い $W^G=\int_G$トラ$\rho (g)dg$。

$p=\int_G\rho (g)dg$を入れてください。 $h\in G$ の場合、

$$
\rho (h)\circ p=\int_G\rho (hg)dg=\int_G\rho (g)dg=p
$$

同様に$p\circ \rho (h) =p$。したがって、$p$ は G の演算と互換性があり、その像は $W^G$ に含まれます。 $w\in W^G$ の場合、$p(w) =\int_G\rho (g)w dg=w$ があるため、補題になります。

#### 補題 2 {#lie-ix-a2-lem-2 .statement tag=01IW}

$u$ を、体 K 上の有限次元ベクトル空間 E の自己準同型とします。

トレ$u^2=$ トレ$\mathbf{S}^2(u)-$ トレ$\wedge \wedge^2(u)$。

$\chi_u(X) =\prod_{i=1}^n(X-\alpha_i)$ を、$u$ の特性多項式の分解を、K の適切な拡大で線形因子にするとします。 Tr $u^2=\sum_i\alpha^2_i$、Tr $\wedge \wedge^2(u) =\sum_{i<j}\alpha_i\alpha_j$、Tr $\mathbf{S}^2(u) =\sum_{i\leq j}\alpha_i\alpha_j$ (cf. 代数、第 3 章) VII, §5, no. 5、Cor. 3)、したがって結果は次のとおりです。

#### 命題 4 {#lie-ix-a2-prop-4 .statement tag=01IX}

$\rho$ が既約であると仮定します。次に、整 $\int_G$ Tr$\rho (g^2)dg$ が 1 (それぞれ 0、それぞれ $-1$) に等しい場合にのみ、$\rho$ は実数 (それぞれ複素数、それぞれ四元数) 型になります。

$W^*$ ($\check{\rho}(g) =^t\rho (g^{-1})$ で定義) 上の $\rho$ の反格表現を $\check{\rho}$ で表します。 適用補題 2 から $\check{\rho}(g)$ を G 上で積分すると、次のようになります。

$\int_G$ トレ$\rho (g^2)dg=\int_G$ トレ $^t\rho (g^{-2})dg=\int_G$ トレ $\mathbf{S}^2( \check{\rho}(g))dg-\int_G$ トレ $\wedge \wedge^2( \check{\rho}(g))dg$

したがって、補題 1 までに、

$\int_G$ Tr $\rho (g^2)dg=$ ディム($\mathbf{S}^2W^*$)$^G-$ ディム($\wedge \wedge^2W^*$)$^G$。

しかし、$\mathbf{S}^2W^*$ (それぞれ$\wedge \wedge^2W^*$) は、W 上の対称 (それぞれ交代的) 双線形形式の空間と識別できます。 したがって、命題は、提案 3 の直後に続きます。
