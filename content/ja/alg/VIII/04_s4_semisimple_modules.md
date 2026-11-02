---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 4
section_title: Semisimple Modules
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.55-A VIII.75
pdf_pages: 0072-0092
extraction: native
subsections:
    - "no": 1
      title: Semisimple Modules
      page: 55
      pdf_page: 72
    - "no": 2
      title: The homomorphism $\bigoplus_i$ Hom$_A(M,N_i)\longrightarrow$ Hom$_A(M,\bigoplus_iN_i)$
      page: 57
      pdf_page: 74
    - "no": 3
      title: Some Operations on Modules
      page: 58
      pdf_page: 75
    - "no": 4
      title: Isotypical Modules
      page: 61
      pdf_page: 78
    - "no": 5
      title: Description of an Isotypical Module
      page: 62
      pdf_page: 79
    - "no": 6
      title: Isotypical Components of a Module
      page: 65
      pdf_page: 82
    - "no": 7
      title: Description of a Semisimple Module
      page: 69
      pdf_page: 86
    - "no": 8
      title: Multiplicities and Lengths in Semisimple Modules
      page: 71
      pdf_page: 88
statements: 43
exercises: 8
content_sha256: 1c386c3bc796b159446f0a7ec662fb4f7041cc32eb2a46d089605b0eb0db359e
translated_from: content/en/alg/VIII/04_s4_semisimple_modules.md
translation_method: google
source_content_sha256: 9d4584b8ed5e9b2ea8bfc7a3b377164098496c5ee0e2c21f520fa31ff9205f9d
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: f7a69f031ea3c34e9daa8c29f97ab1b28da55b2a3a92238848ee87b5a6eb945b
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 4。 半単純加群

### 1. 半単純加群

#### 定義 1 {#alg-viii-s4-def-1 .statement tag=0040}

単純加群.[^1] の家族の直和の場合、加群は半単純と呼ばれます。

単純なマルチモジュールのファミリー (cf. I, §4, No. 4、p. 37、定義 7) の直和である場合、マルチモジュールは半単純と呼ばれます。

A-加群 M は、$A_M$ の環に対して加群として見たときに、半単純である場合に限り、半単純になります。

#### 例 1 {#alg-viii-s4-n1-exa-1 .statement tag=0041}

加群は 0 に減らされ、単純加群は半単純加群になります。

#### 例 2 {#alg-viii-s4-n1-exa-2 .statement tag=0042}

A が体の場合、すべての A-加群は II, §7, No. 1、p. 292 の 1 つである定理によって半単純になります。 これは、一般に、半単純加群がいくつかの方法で単純部分加群の直和に分解されることを示しています (ただし、VIII の系 2、p. 68 を参照)。

#### 例 3 {#alg-viii-s4-n1-exa-3 .statement tag=0043}

Aを主イデアル整域、PをAの既約元の代表からなる(VII, §1, No. 3、p. 3)の系とします。 M を A-加群とし、$\pi \in P$ ごとに、$M(\pi )$ を $\pi x= 0$ となるように $x\in M$ の集合とします。 VII, §2, No. 2、p. 9、A-加群により、M は部分加群 $M(\pi )$ の和である場合に限り、半単純になります。従って、これら部分加群のうちの直和になります。この例はさらに一般化されます (VIII、p. 65)。

$A_1$ と $A_2$ を可換環 K の上の代数とします。 III, §4, No. 3、p. 466 では、左の両側加群の概念を代数 $A_1$ と $A_2$ の上に導入し、これが次のことを示しました概念は、環 $A_1\otimes_KA_2$ を超える左加群に相当します。 M が環 $A_1\otimes_KA_2$ 上の単純 (それぞれ半単純、有限生成) 加群である場合、M は単純 (それぞれ半単純、有限生成) 両側加群であると言います。

#### 定理 1 {#alg-viii-s4-thm-1 .statement tag=0044}

M を単純部分加群の家族 $(S_i)_{i\in I}$ の (必ずしも直接ではない) 和である加群とし、N を M の部分加群とします。 M が N の族からなるの直和であり、J を通る $j$ に対して加群 $S_j$ となるような I の部分集合 J が存在します。

Let $\mathscr{S}$ be the set of subsets $I'$ of I such that the sum of the family consisting of the modules N and $S_i$ for $i$ in $I'$ is direct. 集合 $\mathscr{S}$ は有限の指標: I 属するから $\mathscr{S}$ の部分集合 J は、同じことが J のすべての有限部分集合に当てはまる場合に限ります。 従って、集合 $\mathscr{S}$ は極大元 J (集合理論, III, §4, No. 5, p. 171) になります。 集合 $N'= N +\sum_{j\in J}S_j$。 $i$ を I にしましょう - J. J は $\mathscr{S}$ で最大なので、集合 $J\cup  \{i\}$ は属するから $\mathscr{S}$ にならないので、$S_i\cap N'\not= 0$ になります。 $S_i$ は単純加群なので、$S_i\cap N'= S_i$ になります。 従って、$i\in I$、よって $N'= M$ ごとに $S_i\subset N'$ が得られます。 これで証明は完了です。

#### 系 1 {#alg-viii-s4-thm-1-cor-1 .statement tag=0045}

単純加群の家族の和であるすべての加群は半単純です。

N = 0 の場合には定理を適用する 1 で十分です。

#### 系 2 {#alg-viii-s4-thm-1-cor-2 .statement tag=0046}

加群 M は、M のすべての部分加群が直因子である場合に限り、半単純になります。

条件は定理1までに必要です。

逆に、M のすべての部分加群が補充を認めるとします。 $M'$ を M の単純部分加群の和とし、$M''$ を M の $M'$ の補充とします。$M'\not= M$ があるため、$M''\not= 0$ があるとします。 N を $M''$ の非零単一種部分加群とします。 VIII, p. 49 の命題 3 により、N の極大部分加群 P が存在します。Q を M の P を補足する部分加群とします。そのとき、$N\cap Q$ は N の部分加群で、N の P を補足します。従って、$N/P$ と同型です。 (II, §1, No. 9、p. 210、命題13)。従って、$N\cap Q$は、$M'$の定義とは逆に、$M''$の単純部分加群になります。

従って、$M'= M$ があり、加群 M は系 1 により半単純になります。

#### 系 3 {#alg-viii-s4-thm-1-cor-3 .statement tag=0047}

M を M の半単純加群と N 部分加群とします。加群 N と $M/N$ は半単純です。より正確には、M が単純加群の族 $(S_i)_{i\in I}$ の直和である場合、$M/N$ が $\bigoplus_{j\in J}S_j$ に、N が $\bigoplus_{i\in I-J}S_i$ に同型となるような I の部分集合 J が存在します。

選ぶ定理 1 と同様に、加群 $N'=\bigoplus_{j\in J}S_j$ は M の N を補足します。従って、$M/N$ と同型です。さらに、M の部分加群 N と $\bigoplus_{i\in I-J}S_i$ はどちらも $N'$ を補足するものであるため、$M/N'$ と同型です。

#### 系 4 {#alg-viii-s4-thm-1-cor-4 .statement tag=0048}

M を半単純加群とします。すると、M の自己準同型環 E が体である場合に限り、M は単純です。

M が単純な場合、E は VIII、p. 47 の命題 2 の系により体になります。

E が体の場合、加群 M は分解不可能です (VIII, p. 31, 命題 4, a))。しかも半単純なので簡単です。

#### 注意 {#alg-viii-s4-n1-rem-1 .statement tag=0049}

K を代数的に閉じた可換体および A K-代数とします。 M を半単純A-加群、つまり有限次元ベクトル空間が体 K より大きいとします。 次に、A-加群 M のすべての自己準同型が K に $\alpha$ を含む形 $x\mapsto \alpha x$ である場合に限り、M は単純です。これは、VIII、p. 47 の定理 1 によって必要であり、上記の系 4 によって十分です。

### 2. 準同型 $\bigoplus_i$ ホム$_A(M,N_i)\longrightarrow$ ホム$_A(M,\bigoplus_iN_i)$

A を環、M を A-加群、$(N_i)_{i\in I}$ を A-加群の家族とします。 $\bigoplus_i$ Hom$_A(M,N_i)$ のいずれかの元 $(u_i)$ と、Hom$_A(M,\bigoplus_iN_i)$ の元 $m\mapsto (u_i(m))$ が関連付けられます。私たちはこうして定義する標準準同型

$\varphi :\bigoplus_i$ ホム$_A(M,N_i)\longrightarrow$ ホム$_A(M,\bigoplus_iN_i)$。

$\varphi$ が単射であることは明らかです。 $u$をホム$_A(M,\bigoplus_iN_i)$の元とします。次に、pr$_i\circ u\not= 0$ が有限であるような添字 $i$ の集合である場合に限り、 $\varphi$ の $u$ 属するから像までです。この条件は、加群 M が有限生成されると自動的に満たされます。

従って、加群 M が有限生成される場合、準同型 $\varphi$ は全単射になります。

### 3. 加群に一部の演算

A と B を環、P を $(A$, B)-bimodule (II, §1, No. 14, p. 225) とします。 定義する 2 つの手順を実行します。1 つは左B-加群から左A-加群に進む手順で、もう 1 つは左A-加群から左B-加群に進む手順です。

3.1. 演算 $\mathscr{T}$。 — V を左B-加群とします。 左A-加群 $P\otimes_BV$ (II, §3, No. 4、p. 247) を $\mathscr{T}(V)$ で表します。 $\mathscr{T}(V)$ の作用の法則は公式によって与えられます

$$
a(p\otimes v) = (ap)\otimes v \tag{1}
$$

$a\in A,p\in P$ と $v\in V$ の場合。

$V'$を左B-加群とします。 V から $V'$ までのすべての B-線型写像 $g$ に対して、$\mathscr{T}(V)$ から $\mathscr{T}(V')$ までの写像 $1_P\otimes g$ は A 線形です。それを$\mathscr{T}(g)$で表します。 Hom$_B(V,V')$ から Hom$_A(\mathscr{T}(V),\mathscr{T}(V'))$ までの写像 $g\mapsto \mathscr{T}(g)$ は $\mathbf{Z}$ 線形であり、次のようになります。

$$
\mathscr{T}(1_V) = 1_{\mathscr{T}(V)},\mathscr{T}(g'\circ g) =\mathscr{T}(g')\circ \mathscr{T}(g) \tag{2}
$$

$V, V', V''$ が左B-加群で、$g: V\rightarrow V',g': V'\rightarrow V''$ が B-線型写像の場合。 テンソル積は直和と通勤しているので、部分加群 $(V_i)_{i\in I}$ の家族の直和が V である場合、同一視できる A-加群 $\mathscr{T}(V)$ は $\bigoplus_i\mathscr{T}(V_i)$ となります。

3.2. 演算 $\mathscr{H}$。 — M を左A-加群とします。 左B-加群 Hom$_A(P,M)$ (II, §1, No. 14、p. 225) を $\mathscr{H}(M)$ で表します。 $\mathscr{H}(M)$ の作用のうち法則は公式によって与えられます

$$
(bf)(p) =f(pb) \tag{3}
$$

$b\in B,f\in$ オム$_A(P,M)$ と $p\in P$ の場合。

$M'$を左A-加群とします。 M から $M'$ までのすべての A-線型写像 $g$ に対して、$\mathscr{H}(M)$ から $\mathscr{H}(M')$ までの写像 Hom$_A(1_P, g)$ は B 線形です。それを$\mathscr{H}(g)$で表します。 Hom$_A(M,M')$ から Hom$_B(\mathscr{H}(M),\mathscr{H}(M'))$ までの写像 $g\mapsto \mathscr{H}(g)$ は $\mathbf{Z}$ 線形であり、次のようになります。

$$
\mathscr{H}(1_M) = 1_{\mathscr{H}(M)},\mathscr{H}(g'\circ g) =\mathscr{H}(g')\circ \mathscr{H}(g) \tag{4}
$$

$M, M', M''$ が左A-加群で、$g: M\rightarrow M',g': M'\rightarrow M''$ が A-線型写像の場合。さらに、P が有限生成A-加群であると仮定します。 M が部分加群 $(M_i)_i$ の家族の直和である場合、VIII、p. 57 により、$\bigoplus_i\mathscr{H}(M_i)$ と同一視できる $\mathscr{H}(M)$ になります。 3.3. 関係 $\mathscr{T}$と$\mathscr{H}$の間。 — II, §4, No. 1、p. 268 の命題 1 により、すべての左A-加群 M とすべての左B-加群 V に対して、一意な群同型が存在します。

(5) $\gamma :$ ホム$_A(\mathscr{T}(V),M)\longrightarrow$ ホム$_B(V,\mathscr{H}(M))$

関係が特徴

$$
(\gamma (h)(v))(p) =h(p\otimes v) \tag{6}
$$

$h\in$ ホム$_A(\mathscr{T}(V),M),v\in V$ と $p\in P$ の場合。 同型 $\gamma$ は随伴同型と呼ばれます。

M を左A-加群とします。 A-加群 $\mathscr{T}(\mathscr{H}(M))$ は単に A-加群 $P\otimes_B$ Hom$_A(P,M)$ です。上記を適用から B-加群 $\mathscr{H}$ (M) までにすると、 写像であることがわかります。

$\alpha_M=\gamma^{-1}$(ID$_{\mathscr{H}(M)}$) $:\mathscr{T}(\mathscr{H}(M))\longrightarrow M$

一意な写像満たすです

$$
\alpha_M(p\otimes f) =f(p) \tag{7}
$$

$p\in P$ と $f\in$ オム$_A(P,M)$ 用。 $\alpha_M$ は $\mathscr{T}(\mathscr{H}(M))$ から M までの正規の A-線型写像であると言います。すべての A-線型写像 $g: M\rightarrow M'$ に対して、可換図式が存在します。

$\mathscr{T}(\mathscr{H}(M))^{\alpha_M}$ // む

(I) $\mathscr{T}_{(\mathscr{H}(g))}g$

$\mathscr{T}(\mathscr{H}(M'))^{\alpha_{M'}}$ // $M'$。

その逆

$\gamma^{-1}:$ ホム$_B(V,\mathscr{H}(M))\longrightarrow$ ホム$_A(\mathscr{T}(V),M)$

随伴同型一致すると写像 $h\mapsto \alpha_M\circ \mathscr{T}(h)$。実際、(6) と (7) により、関係が得られます。

$$
\gamma^{-1}(h)(p\otimes v) = (h(v))(p) =\alpha_M(p\otimes h(v)) =\alpha_M\circ \mathscr{T}(h)(p\otimes v)
$$

すべての$h\in$ Hom$_B(V,\mathscr{H}$ (M))、$v\in V$、および$p\in P$。

VをB-加群とします。 B-加群 $\mathscr{H}(\mathscr{T}(V))$ は単に B-加群 Hom$_A(P,P\otimes_BV)$ です。 適用 (5) から A-加群 $\mathscr{T}$ (V) により、V から $\mathscr{H}(\mathscr{T}(V))$ までの B-線型写像 $\beta_V=\gamma$(Id$_{\mathscr{T}(V)}$) が関係によって特徴付けられていることがわかります。

$$
\beta_V(v)(p) =p\otimes v \tag{8}
$$

$p\in P$ と $v\in V$ の場合。 V から $\mathscr{H}(\mathscr{T}(V))$ までの$\beta_V$ を正規の B-線型写像と呼びます。すべての B-加群 $V'$ とすべての B-線型写像 $g: V\rightarrow V'$ には、可換図式があります。

V $^{\beta_V}$ /$/\mathscr{H}(\mathscr{T}(V))$

(II) $g\mathscr{H}_{\mathscr{T}}$

( $(g)$)

${V'}^{\beta_{V'}}$ /$/\mathscr{H}(\mathscr{T}(V'))$。

随伴射 (5) 一致すると写像が $u$ を $\mathscr{H}(u)\circ \beta_V$ に送信することに注意してください。実際、関係 (6) と (8) から、次の等式が導き出されます。

$$
(\gamma (u)(v))(p) =u(p\otimes v) =u\circ (\beta_V(v))(p)
$$

すべての$u\in$ Hom$_A(\mathscr{T}(V),M),v\in V$、および$p\in P$。

#### 注意 1 {#alg-viii-s4-n3-rem-1 .statement tag=004A}

V と $V'$ を B-加群とします。 随伴同型

$\gamma :$ ホム$_A(\mathscr{T}(V),\mathscr{T}(V'))\longrightarrow$ ホム$_B(V,\mathscr{H}(\mathscr{T}(V')))$

すべての $f\in$ Hom$_B(V,V')$ に対して関係 $\gamma (\mathscr{T}(f)) =\beta_{V'}\circ f$ を満たします。

$$
(\gamma (\mathscr{T}(f))(v))(p) =\mathscr{T}(f)(p\otimes v) =p\otimes f(v) = (\beta_{V'}\circ f)(v)(p)
$$

M と $M'$ を A-加群とします。 the inverse of 随伴同型

$\gamma^{-1}:$ ホム$_B(\mathscr{H}(M),\mathscr{H}(M'))\longrightarrow$ ホム$_A(\mathscr{T}(\mathscr{H}(M)),M')$

$u\in$ Hom$_B(M,M')$ ごとに関係 $\gamma^{-1}(\mathscr{H}(u)) =u\circ \alpha_M$ を満たします。確かに、私たちは関係を持っています

$$
\gamma^{-1}(\mathscr{H}(u))(p\otimes v) = (\mathscr{H}(u)(v))(p) =u(v(p)) =u\circ \alpha_M(p\otimes v)
$$

すべての$u\in$ Hom$_B(M,M'),v\in \mathscr{H}$ (M) と $p\in P$ です。

#### 注意 2 {#alg-viii-s4-n3-rem-2 .statement tag=004B}

M を左A-加群とします。 B-線型写像

$\beta_{\mathscr{H}(M)}:\mathscr{H}(M)\rightarrow \mathscr{H}(\mathscr{T}(\mathscr{H}(M)))$ と $\mathscr{H}(\alpha_M) :\mathscr{H}(\mathscr{T}(\mathscr{H}(M)))\rightarrow \mathscr{H}(M)$ 満たす関係 $\mathscr{H}(\alpha_M)\circ \beta_{\mathscr{H}(M)}= 1_{\mathscr{H}(M)}$。一般にそれらは全単射的ではありません。

Vを左B-加群とします。 A-線型写像

$\mathscr{T}(\beta_V) :\mathscr{T}(V)\rightarrow \mathscr{T}(\mathscr{H}(\mathscr{T}(V)))$ と $\alpha_{\mathscr{T}(V)}:\mathscr{T}(\mathscr{H}(\mathscr{T}(V)))\rightarrow \mathscr{T}(V)$ 満たす関係 $\alpha_{\mathscr{T}(V)}\circ \mathscr{T}(\beta_V) = 1_{\mathscr{T}(V)}$。一般にそれらは全単射的ではありません。

#### 注意 3 {#alg-viii-s4-n3-rem-3 .statement tag=004C}

P が A-加群として有限生成されるとします。 M を A-加群の家族 $(M_i)_{i\in I}$ の直和とします。 A-加群 $\mathscr{T}(\mathscr{H}(M))$ と $\bigoplus_i\mathscr{T}(\mathscr{H}(M_i))$ は標準的に同型です。それらを同一視するすると、$\alpha_M$は$\bigoplus_i\alpha_{M_i}$と同一視されます。同様に、V を B-加群の家族 $(V_j)_{j\in J}$ の直和とします。 B-加群 $\mathscr{H}(\mathscr{T}(V))$ は $\bigoplus_j\mathscr{H}(\mathscr{T}(V_j))$ と識別され、線形写像 $\beta_V$ は $\bigoplus_j\beta_{V_j}$ と識別されます。

### 4. 等型加群

Aを環、Sを単純な左A-加群とします。 D を S の自己準同型環の反対環とします。 体です。 A と D の作用を備えた S は、$(A$, D)-バイモジュールです。

#### 命題 1 {#alg-viii-s4-prop-1 .statement tag=004D}

M をA-加群とします。次のプロパティは同等です。

(i) M が $S^{(I)}$ と同型となる集合 I が存在します。

(ii) 加群 M は、S と同型の部分加群族の直和です。

(iii) 加群 M は、S と同型の部分加群族の和です。

(iv) A-加群 M が $S\otimes_DV$ と同型となるような体 D 上に左ベクトル空間 V が存在します。

(i)と(ii)の同値は明らかで、(ii)と(iii)の定理はVIII、p. 56の1をN=0の場合に適用します。 D 上のすべての左ベクトル空間は、形 $D_s^{(I)}$ のベクトル空間と同型です。ここで、I は集合 (II, §7, No. 1, p. 292, 定理 1) です。 テンソル積は直和と可換であるため、(i) は (iv) と同等です。

#### 定義 2 {#alg-viii-s4-def-2 .statement tag=004E}

A-加群 M は、命題 1 と同等の性質を持つ場合、型 S と同型です。 加群 M は、M が型 T と同型であるような単純A-加群 T が存在する場合、同型と呼ばれます。

すべての等型加群は半単純です。

#### 命題 2 {#alg-viii-s4-prop-2 .statement tag=004F}

加群が型 S の同型部分加群の和である場合、型 S の同型です。 型 S の等型加群の部分加群と商加群は型 S の同型です。

最初の主張は定義から続き、2 番目は VIII、p. 56 の系 3 から続きます。

#### 注意 {#alg-viii-s4-n4-rem-1 .statement tag=004G}

型 S のすべての非零等型加群には、S と同型の商加群と部分加群があります。従って、M と $M'$ が型 S の非零等型A-加群である場合、群 Hom$_A(M,M')$ は 0 に減らされません。

#### 命題 3 {#alg-viii-s4-prop-3 .statement tag=004H}

a) M を型 S の等型A-加群とします。$\alpha_M(s\otimes f) =f(s)$ (VIII, p. 59) によって特徴付けられるA-線型写像 $\alpha_M: S\otimes_D$Hom$_A(S,M)\rightarrow M$ は全単射です。

b) V を体 D 上で左ベクトル空間とする。 $\beta_V(v)(s) =s\otimes v$ (VIII, p. 59) によって定義される D 線形写像 $\beta_V: V\rightarrow$ Hom$_A(S,S\otimes_DV)$ は全単射である。

左のD-ベクトル空間 Hom$_A(S,M)$を$\mathscr{H}(M)$で表します。 A-加群 M は、仮定により、部分加群の族の直和が S と同型です。 A-加群 S は単一です。 写像 $\alpha_M$ が全単射であることを証明するには、M = S (VIII, p. 60, 注意 3) の場合を考慮するだけで十分です。ここで、$\mathscr{H}(S)$ は単に D-ベクトル空間 $D_s$ であり、$\alpha_S$ は単に $\iota (s\otimes d) =sd$ によって定義された同型 $\iota : S\otimes_DD_s\rightarrow S$ です。

同様に、b) を証明するには、$V = D_s$ の場合を考慮するだけで十分です。 写像 $\alpha_S$ は全単射なので、写像 $\beta_{D_s}=\beta_{\mathscr{H}(S)}$ も全単射です (VIII、p. 60、注意 2)。

### 5. 等型加群中記述

前の小節と同様に、Aは環、Sは単純な左A-加群、Dは体終わり$_A(S)^o$を表します。 S を $(A$, D)-バイモジュールと見なします。

#### 定義 3 {#alg-viii-s4-def-3 .statement tag=004I}

M を型 S の等型A-加群とします。S に関する M の記述は対 $(V, \alpha )$ で、V は体 D 以上の左ベクトル空間であり、$\alpha : S\otimes_DV\rightarrow M$ は A-加群の同型です。

Every isotypical A-module M of type S has a canonical description: it is the pair (Hom$_A(S,M), \alpha_M$), where $\alpha_M: S\otimes_D$ Hom$_A(S,M)\rightarrow M$ is the isomorphism of A-modules characterized by $\alpha_M(s\otimes f) =f(s)$ (VIII, p. 62, Proposition 3, a)).

#### 定理 2 {#alg-viii-s4-thm-2 .statement tag=004J}

M を型 S の等型A-加群および M の $(V, \alpha )$ 記述とします。V の D 線形部分空間を包含順に並べた $\mathscr{D}_D(V)$ 集合と、M の A-部分加群の$\mathscr{D}_A(M)$ で表します。 $W\in$ $\mathscr{D}_D(V)$、同一視する A-加群 $S\otimes_DW$ ごとに、$S\otimes_DV$ には標準像が入ります。

a) 写像 $W\mapsto \alpha (S\otimes_DW)$ は、$\mathscr{D}_D(V)$ から $\mathscr{D}_A(M)$ までの順序集合の同型です。

b) 逆同型は、$s\in S$ ごとに $\alpha (s\otimes v)$ 属するが N になるように、M の部分加群 N を V からなるの元 $v$ の線形部分空間に送信します。

$W\in \mathscr{D}_D$(V)、集合 $\varphi (W) =\alpha (S\otimes_DW)$の場合。 $N\in \mathscr{D}_A$(M)​​の場合、$s\in S$ごとに$\alpha (s\otimes v)\in N$となるように、元$v\in V$の$\psi (N)$集合で表します。この定義するは 2 つの写像 $\varphi :\mathscr{D}_D(V)\rightarrow \mathscr{D}_A(M)$ と $\psi :\mathscr{D}_A(M)\rightarrow \mathscr{D}_D(V)$ です。明らかに増加するです。

N を M の部分加群とします。これは型 S (VIII, p. 61, 命題 2) と同型です。 集合 $W =\psi (N)$。 命題 3 により、VIII、p. 62、A-線型写像の b) $h: S\rightarrow M$ は単に写像 $s\mapsto \alpha (s\otimes v)$ となり、$v$ は V まで続きます。 N に像が含まれるものは、写像 $s\mapsto \alpha (s\otimes w)$ で、$w$ は W を通過します。 N は型 S と同型であるため、彼らの像生成する N です。したがって、$\alpha (S\otimes_DW) = N$、つまり $\varphi (\psi (N)) = N$ が得られます。これは、$\varphi \circ \psi$が$\mathscr{D}_A(M)$の恒等写像であることを証明します。特に、$\varphi$ は全射法、$\psi$ は単射法です。

証明を終えるには、写像 $\varphi$ が単射であることを証明すれば十分です。 W と $W'$ を $\varphi (W) =\varphi (W')$ となるような V の線形部分空間とする。 $S\otimes_DV$ の線形部分空間として見た場合、ベクトル空間 $S\otimes_DW$ と $S\otimes_DW'$ 一致する。 選ぶ非零線型形式 $f$ を D-ベクトル空間 S に置き、$g: S\otimes_DV\rightarrow V$ を $g(s\otimes v) =f(s)v$ によって定義される群準同型とします。 $W =g(S\otimes_DW) =g(S\otimes_DW') = W'$があるので、$\varphi$は単射法です。

#### 注意 1 {#alg-viii-s4-n5-rem-1 .statement tag=004K}

M を型 S の等型A-加群と M の $(V, \alpha )$ 記述とします。すると、V が有限次元である場合に限り、M は有限長になります。この場合、関係になります。

長い$_A(M) =$ 暗い$_D(V)$。

#### 系 1 {#alg-viii-s4-thm-2-cor-1 .statement tag=004L}

M を型 S の等型A-加群とします。 For every A-submodule N of M, identify Hom$_A(S,N)$ with the linear subspace of Hom$_A(S,M)$ consisting of the mappings with image contained in N.

a) 写像 $N\mapsto$ Hom$_A(S,N)$ は、$\mathscr{D}_A(M)$ から $\mathscr{D}_D$(Hom$_A(S,M)$) までの順序集合の同型です。

b) 逆全単射は Hom$_A(S,M)$ の線形部分空間 W を M の部分加群 $\sum_{h\in W}h(S)$ に送信します。

これは、$(V, \alpha )$ を M の標準的記述として、定理 2 を再定式化したものです。

#### 系 2 {#alg-viii-s4-thm-2-cor-2 .statement tag=004M}

V を D 上の左ベクトル空間および V の自己準同型の $\mathscr{F}$ 集合とします。 An A-submodule of $S\otimes_DV$ is stable under all endomorphisms $1_S\otimes u$, where $u$ runs through $\mathscr{F}$, if and only if it is of the form $S\otimes_DW$, where W is a linear subspace of V that is stable under all endomorphisms belonging to $\mathscr{F}$.

実際、定理 2 までに、$S\otimes_DV$ のすべての A-部分加群 N は $S\otimes_DW$ に等しくなります。ここで W は、元 $v$ のV からなるの線形部分空間であり、すべての$s\otimes v$ 属するが N になります。 $s\in S$。

#### 定理 3 {#alg-viii-s4-thm-3 .statement tag=004N}

Mと$M'$を型Sの等型A-加群とします。$(V, \alpha )$と$(V', \alpha ')$をそれぞれMと$M'$の記述とします。任意の D 線形写像 $f: V\rightarrow V'$ について、次の図式を可換にする一意の A-線型写像を $\widetilde{f}: M\rightarrow M'$ で示します。

$S\otimes_DV^{\alpha}$ //M

$$
1_{_S\otimes f}\widetilde{f} \tag{9}
$$

$S\otimes_D{V'}^{\alpha'}$ // $M'$。

ホム$_D(V,V')$からホム$_A(M,M')$までの写像$f\mapsto \widetilde{f}$は群同型です。

Hom$_D(V,V')$ から Hom$_A(S\otimes_DV,S\otimes_DV')$ への $\mathbf{Z}$ 線形写像 $u\mapsto 1_S\otimes u$ が全単射であることを証明すれば十分です。 $(A$、D)-bimodule S に適用された No.3 の記法では、この対応するは写像を示しています

$\mathscr{T}:$ ホム$_D(V,V')\longrightarrow$ ホム$_A(\mathscr{T}(V),\mathscr{T}(V'))$

全客観的です。しかし、VIII, p. 60 の注意 1 により、随伴同型 (VIII, p. 59) は全単射であるため、この対応するは、$u$ を $\beta_{V'}\circ u$ に送信する写像が全単射であることを示します。 D 線形写像 $\beta_{V'}$ は全単射です (VIII, p. 62, 命題 3, b))。

定理 3 の記法を保持します。 $M''$ を型 S の等型A-加群とし、$(V'', \alpha '')$ を $M''$ の記述とします。すべての $f\in$ Hom$_D(V,V')$ とすべての $g\in$ Hom$_D(V',V'')$ に対して、$g]\circ f=\widetilde{g}\circ \widetilde{f}$ があります。特に、$M = M'$、$V = V'$、$\alpha =\alpha '$の場合、End$_D(V)$からEnd$_A(M)$までの写像$f\mapsto \widetilde{f}$は環同型です。

#### 注意 2 {#alg-viii-s4-n5-rem-2 .statement tag=004O}

M を型 S の等型A-加群とし、$(V, \alpha )$ を M の記述とします。 B を環 End$_A(M)^o$ の部分環とします。 End$_D(V)^o$ から End$_A(M)^o$ までの環同型は、V に $(D$, B)-bimodule の構造を与え、$\alpha$ は $(A$, B)-bimodule の同型になります。 There exists an isomorphism from the set of $(D$, B)-sub-bimodules of V, ordered by inclusion, to the set of $(A$, B)-sub-bimodules of M (VIII, p. 62, Theorem 2 and VIII, p. 63, Corollary 2).

#### 系 {#alg-viii-s4-n5-cor-1 .statement tag=004P}

M と $M'$ を型 S の等型A-加群とします。 写像 $u\mapsto$ Hom$_A(M,M')$ から Hom$_D$ (Hom$_A(S,M)$, Hom$_A(S,M')$) までの Hom(1$_S, u$) は群同型です。 Mが$M'$に等しい場合、End$_A(M)$からEnd$_D$(Hom$_A(S,M)$)までは環同型です。

VIII、p. 59の図式(I)の可換性により、この系は定理3から続き、Mと$M'$の標準的記述に適用されます。

### 6. 加群の同型成分

#### 定義 4 {#alg-viii-s4-def-4 .statement tag=004Q}

A を環、M A-加群、S 単純A-加群とします。 $M_S$ で示される M の型 S の同型成分は、S と同型の M の部分加群の和です。

$M_S$ が型 S の同型である M の最大の部分加群であることは明らかです。 $M_S$ のすべての部分加群は型 S (VIII、p. 61、命題 2) の同型であるため、次のようになります。 M の部分加群 N ごとに $N_S= M_S\cap N$

$S'$ が S と同型の単純A-加群である場合、明らかに $M_S=$ $M_{S'}$ が存在するため、$M_S$ は S (VIII、p. 51) の類にのみ依存します。

M をA-加群とします。 M には最大の半単純部分加群が存在し、M のソクルと呼ばれます。それは、M の単純部分加群の和であり、M の同型成分の和でもあります。特に、M は、そのソクルと等しい場合に限り、半単純です。

#### 命題 4 {#alg-viii-s4-prop-4 .statement tag=004R}

A を環とします。 集合、類、単純A-加群を$\mathscr{S}$で表します。 M を半単純A-加群とします。

a) 加群 M は、同型成分のファミリー $(M_{\lambda})_{\lambda\in\mathscr{S}}$ の直和です。

b) M が単純部分加群の家族 $(N_i)_{i\in I}$ の直和であると仮定します。すべての $\lambda \in \mathscr{S}$ について、$I(\lambda )$ を添字 $i\in I$ の集合とし、$N_i$ は類 $\lambda$ とします。 $M_{\lambda}=\bigoplus_{i\in I(\lambda)}N_i$があります。

c) M が有限に生成される場合、$M_{\lambda}\not= 0$ が有限となるように、$\lambda \in \mathscr{S}$ の集合が生成されます。

d) M のすべての部分加群 N とすべての $\lambda \in \mathscr{S}$ に対して、$N_{\lambda}= N\cap M_{\lambda}$ と $(M/N)_{\lambda}= (M_{\lambda}+ N)/N$ があります。

Mは半単純なので、家族$(M_{\lambda})_{\lambda\in\mathscr{S}}$の和です。この和が直接的であることを証明しましょう。 $\lambda \in \mathscr{S}$ にしましょう。家族$(M_\mu)_{\mu\in\mathscr{S}-\{\lambda\}}$の和を$M'_{\lambda}$で表します。 加群 $M'_{\lambda}$ は、単純加群の族の直和であり、$\lambda$ (VIII、p. 56、定理 1) と同型ではありません。 系 3 の定理 1 の VIII、p. 56、$M'_{\lambda}$ は含むの類 $\lambda$ のいずれの単純部分加群も含みません。従って、$M_{\lambda}\cap M'_{\lambda}= 0$ となります。従って、主張 a) が証明されます。 構成までに $M_{\lambda}\supset \bigoplus_{i\in I(\lambda)}N_i$ が得られるので、主張 b) 注意 1 の II, §1, No. 8、p. 208 から続きます。

主張 c) は、a) と II, §1, No. 12、p. 221 の 23 命題から続きます。

NをMと$\lambda \in \mathscr{S}$の部分加群とします。 N の型 $\lambda$ の同型成分 $N_{\lambda}$ は、$M_{\lambda}$ と $M_{\lambda}\cap N\subset N_{\lambda}$ に含まれます。従って、共通部分 $N\cap M_{\lambda}$ は、型 $\lambda$ の N の同型成分です。

すべての $\lambda \in \mathscr{S}$ について、加群 $M_{\lambda}+N/N$ は $M_{\lambda}/(M_{\lambda}\cap N)$ と同型です。従って、これは型 $\lambda$ と同型であり、$(M/N)_{\lambda}$ に含まれます。 最後の主張は a) と II, §1, No. 8、p. 208、注意 1 から続きます。

#### 系 {#alg-viii-s4-n6-cor-1 .statement tag=004S}

A を環と類の単純A-加群の $\mathscr{S}$ 集合とします。 M を M の半単純A-加群と N 部分加群とします。そうすると、$N =\bigoplus_{\lambda\in\mathscr{S}}N\cap M_{\lambda}$ と $M/N =\bigoplus_{\lambda\in\mathscr{S}}(M_{\lambda}+ N)/N$ が得られます。

N と $M/N$ は半単純 (VIII, p. 56, 系 3) であるため、系は命題 4, d) から続きます。

半単純A-加群 M の支持体は、類 $\lambda$ の単純A-加群の集合であり、型 $\lambda$ の M の同型成分は非零です。有限に生成された半単純A-加群のサポートは有限です。

#### 命題 5 {#alg-viii-s4-prop-5 .statement tag=004T}

A を環とし、$\mathscr{S}$ を類の単純A-加群の集合とします。 M と N をA-加群とします。

a) $f: M\rightarrow N$ を準同型とします。 $M_{\lambda}$ から $N_{\lambda}$ までの $\lambda \in \mathscr{S},f$ 誘導する準同型 $f_{\lambda}$ ごと。 M が半単純と $f$ の全射であれば、 準同型 $f_{\lambda}$ はそれぞれ全射です。

b) M が半単純であると仮定します。 写像 $f\mapsto (f_{\lambda})_{\lambda\in\mathscr{S}}$ は、ホム$_A(M,N)$ から $\prod_{\lambda\in\mathscr{S}}$ ホム$_A(M_{\lambda},N_{\lambda})$ までの群同型です。 M が N に等しいとき、写像は、端$_A(M)$ から$\prod_{\lambda\in\mathscr{S}}$ 端$_A(M_{\lambda})$ までの環同型です。

すべての $\lambda \in \mathscr{S}$ について、N の部分加群 $f(M_{\lambda})$ は、型 $\lambda$ の等型加群の商と同型です。従って、それは型 $\lambda$ の同型であり、その結果、 $N_{\lambda}$ に含まれます。

M が半単純および $f$ 全射であると仮定します。次に、$M/$ Ker($f$) から N への $f$ 誘導する同型が、$(M_{\lambda}$+Ker($f$))$/$ Ker($f$) を $f(M_{\lambda})$ に送信します。 VIII、p. 65 の命題 4 までに、$N_{\lambda}=f(M_{\lambda})$ が得られ、a) の証明が完了します。

b) で考慮される写像は明らかに群準同型であり、M が N に等しいとき、それは環準同型です。 $(f_{\lambda})_{\lambda\in\mathscr{S}}$ を $\prod_{\lambda\in\mathscr{S}}$ Hom(M$_{\lambda},N_{\lambda}$) の元とします。 b) の写像の下にある逆像の一意元は、 準同型 $f: M\rightarrow N$ で定義されます。

$$
f((\sum_{\lambda\in\mathscr{S}}x_{\lambda})=\sum_{\lambda\in\mathscr{S}}f_{\lambda}(x_{\lambda})
$$

$(x_{\lambda})_{\lambda\in\mathscr{S}}\in \bigoplus_{\lambda}M_{\lambda}$ごとに。

#### 注意 {#alg-viii-s4-n6-rem-1 .statement tag=004U}

A と B を環とします。 M を $(A$、B)-bimodule とします。 命題 5 から、A-加群 M の同型成分は M の部分両側加群であることがわかります。これは、特に M が A-加群で B が End$_A(M)$ の反対環である場合に当てはまります。

#### 例 {#alg-viii-s4-n6-exa-1 .statement tag=004V}

環 A が可換である場合を考えてみましょう。最大理想値 $\mathfrak{m}$ を cl(A$/\mathfrak{m}$) に送信する写像は、A の最大理想値集合から単純A-加群の類の集合 $\mathscr{S}$ までの全単射です (VIII, p. 51）。 逆全単射は $\lambda$ をその消滅子 $\mathfrak{m}_{\lambda}$ に送信します。

M をA-加群とします。すべての $\lambda \in \mathscr{S}$ について、M の型 $\lambda$ の同型成分 $M_{\lambda}$ は、$\mathfrak{m}_{\lambda}$ によって消滅した元で構成されており、$M_{\lambda}$ は体に対するベクトル空間として見ることができます。 $A/\mathfrak{m}_{\lambda}$。 M が半単純、N が他の A-加群である場合、命題 5 から Hom$_A(M,N)$ から $\prod_{\lambda\in\mathscr{S}}$ Hom$_{A/\mathfrak{m}_{\lambda}}(M_{\lambda},N_{\lambda})$ まで群同型を推定できます。

#### 系 1 {#alg-viii-s4-prop-5-cor-1 .statement tag=004W}

M を M の半単純A-加群 、N 部分加群とします。次のプロパティは同等です。

(i) M には N を補足する固有の部分加群が存在します。

(ii) Hom$_A(M/N,N) = 0$ がいます。

(iii) $N =\bigoplus_{\lambda\in\Lambda}M_{\lambda}$ となるような $\mathscr{S}$ の部分集合 Λ が存在します。

選ぶ部分加群 $N'$ M の N を補足します (VIII、p. 56、系 2)。 $N'\times N$ で M を同一視するとすると、N を補足する M の部分加群は、$N'$ から N までの A-線型写像のグラフになります。 $N'$ は $M/N$ と同型なので、性質 (i) と (ii) の同値が証明されました。 命題 5, b) により、群 Hom$_A(N',N)$ は群 $\prod_{\lambda\in\mathscr{S}}$ Hom$_A(N'_{\lambda},N_{\lambda})$ と同型です。 $\lambda \in \mathscr{S}$ごとに$N_{\lambda}= 0$または$N'_{\lambda}= 0$(VIII、p. 61、注意)、つまり$N_{\lambda}= 0$または$N_{\lambda}= M_{\lambda}$がある場合にのみ、零になります。これは、性質 (ii) と (iii) の同値を証明します。

#### 系 2 {#alg-viii-s4-prop-5-cor-2 .statement tag=00R0}

M をA-加群とします。次の 2 つの条件は同等です。

(i) M のすべての部分加群は、一意の補部分加群を許容します。

(ii) 加群 M は、単純なペア非同型加群の族 $(S_i)_{i\in I}$ の直和です。

M がこれら条件を満たすとする。次に、M のすべての部分加群 N に対して、$N =\bigoplus_{j\in J}S_j$ があり、M のすべての単純部分加群が $S_i$ の 1 つに等しいような、I の一意の部分集合 J が存在します。

条件 (i) と (ii) はどちらも M が半単純であることを意味します。

条件 (i) が満たされるとします。 $\lambda \in \mathscr{S}$ にしましょう。 系 1 の (i) と (iii) の同値により、$M_{\lambda}$ のすべての部分加群は零または $M_{\lambda}$ に等しくなります。従って、$M_{\lambda}$ は零または単純であり、(ii) M が族 $(M_{\lambda})_{\lambda\in\mathscr{S}}$ の直和であるという事実から導かれます。

逆に、条件 (ii) が満たされる場合、$M_{\lambda}$ は $\lambda \in \mathscr{S}$ ごとに零または単純になります。 N が M の部分加群である場合、$N\cap M_{\lambda}$ は $\lambda \in \mathscr{S}$ ごとに 0 または $M_{\lambda}$ に等しくなります。 $N =\bigoplus_{\lambda\in\mathscr{S}}(N\cap M_{\lambda})$ (VIII, p. 66, 系) があるため、部分加群 N は系 1 の性質 (iii) を持ち、従って M に一意の補部分加群が認められます。これは、(ii) が (i) を暗黙的に示すだけでなく、(ii) が (i) を意味することを証明します。 系の最後の主張。

MをA-加群、Sを単純A-加群とします。 体 End$_A(S)$ の反対環を D で表し、S を $(A$, D)-bimodule として見ます。次に、Hom$_A(S,M)$ は D 上で左ベクトル空間、Hom$_A(M,S)$ は D 上で右ベクトル空間です。左の D-ベクトル空間 Hom$_A(S,M)$ の双対は、D 上で右ベクトル空間です (II, §2, No. 3, p. 232, 定義 2)。ホム$_A(S,M)$からホム$_A(S,S) = D$までの$u\in$ホム$_A(M,S)$、写像$h(u) :v\mapsto u\circ v$の左側は線型形式D-ベクトル空間ホム$_A(S,M)$です。

#### 命題 6 {#alg-viii-s4-prop-6 .statement tag=004X}

上の記法をそのままにして、A-加群Mが半単純であると仮定します。 右D-ベクトル空間 Hom$_A(M,S)$ から左双対 D-ベクトル空間 Hom$_A(S,M)$ までの写像 $u\mapsto h(u)$ は D 線形で全単射です。

$u\in$ ホム$_A(M,S),v\in$ ホム$_A(S,M)$ と $d\in D$ とします。私たちは持っています

$$
h(ud)(v) =h(d\circ u)(v) =d\circ u\circ v=d\circ (h(u)(v)) =h(u)(v)d
$$

これは、写像 $h$ が D 線形であることを証明します。それは単に、ホム$_A(M,S)$からホム$_D$(ホム$_A(S,M)$, ホム$_A(S,S)$)まで$u\mapsto$ホム(1$_S, u$)から与えられる写像です。それが全単射であることを証明するには、VIII、p. 66 の命題 5、b) によって、M が型 S と同型である場合を扱うだけで十分です。次に、VIII、p. 65 の系を適用できます。

### 7. 記述/半単純加群

この切断の余りについて、Aは環、$\mathscr{S}$は単純A-加群の類の集合です。 $\lambda \in \mathscr{S}$ ごとに、類 $\lambda$ の選ぶ単純加群 $S_{\lambda}$ (たとえば、 $S_{\lambda}=\lambda$ )。 反対環、体、自己準同型、$S_{\lambda}$を$D_{\lambda}$で表します。 $S_{\lambda}$ を $(A,D_{\lambda}$)-bimodule として見ます。

M をA-加群とします。 $\lambda \in \mathscr{S}$ ごとに、ホム$_A(S_{\lambda},M)$ は体 $D_{\lambda}$ を超えて左ベクトル空間になります。 VIII、p. 59、および II, §1, No. 6、p. 202、命題 6 までに、正規と呼ばれる固有の A-線型写像が存在します。

$\alpha_M:\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}$ ホム$_A(S_{\lambda},M))\rightarrow M$

満たす関係

$$
\alpha_M(s\otimes f) =f(s) \tag{10}
$$

$\lambda \in \mathscr{S},s\in S_{\lambda}$、および$f\in$ ホム$_A(S_{\lambda},M)$ 用。 $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M))$ と M に End$_A$(M) モジュールの自然な構造を与えると、写像 $\alpha_M$ は End$_A$(M)-linear になります。

#### 命題 7 {#alg-viii-s4-prop-7 .statement tag=004Y}

M をA-加群とします。 標準写像 $\alpha_M$ は単射法です。すべての $\lambda \in \mathscr{S}$ について、$S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M)$ の $\alpha_M$ の下にある像は、型 $\lambda$ の M の同型成分です。 $\alpha_M$ の像は M のソクルです。 A-加群 M は、写像 $\alpha_M$ が全単射である場合に限り、 半単純です。

$\lambda \in \mathscr{S}$ にしましょう。 型 $\lambda$ の M の同型成分を $M_{\lambda}$ で表します。 $S_{\lambda}$ から M までのすべての A-線型写像は、$M_{\lambda}$ で値になります (VIII、p. 66、命題 5)。その結果、命題 3 までに、a) VIII、p. 62、写像 $\alpha_M$ 誘導する全単射 $S_{\lambda}\otimes_{D_{\lambda}}$ Hom$_A(S_{\lambda},M)$ から$M_{\lambda}$ まで。 命題が続きます。なぜなら、M のソクルは家族 $(M_{\lambda})_{\lambda\in\mathscr{S}}$ の直和であり、加群 M は、ソクルと等しい場合に限り、半単純であるからです。

#### 定義 5 {#alg-viii-s4-def-5 .statement tag=004Z}

M を半単純A-加群とします。 M の記述 (家族 $(S_{\lambda})_{\lambda\in\mathscr{S}}$ に関して) は対 $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$ で、$V_{\lambda}$ は各 $\lambda \in \mathscr{S}$ の体 $D_{\lambda}$ を超える左ベクトル空間であり、$\alpha :\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda})\rightarrow M$ は同型ですA-加群。

命題 7 までに、すべての半単純A-加群 M は標準的記述になります。それは対 ((Hom$_A(S_{\lambda},M)$)$_{\lambda\in\mathscr{S}}, \alpha_M$) です。ここで、$\alpha_M$ は公式 (10) で定義される A-線型写像です。

#### 命題 8 {#alg-viii-s4-prop-8 .statement tag=0050}

M を M の半単純A-加群と $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$ 記述とします。

a) A-加群 $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ から型 $\lambda$ の M の同型成分までのすべての $\lambda \in \mathscr{S}$、写像 $\alpha$ 誘導する同型について。

b) $\beta_{\lambda}(v)(s) =\alpha (s\otimes v)$ によって定義されるすべての $\lambda \in \mathscr{S}$、写像 $\beta_{\lambda}: V_{\lambda}\rightarrow$ Hom$_A(S_{\lambda},M)$ は、$D_{\lambda}$-線形かつ全単射です。

c) N を M の部分加群とします。以下の特性を持つ一意の族 $(W_{\lambda})_{\lambda\in\mathscr{S}}$ が存在します: $W_{\lambda}$ は、$\lambda \in \mathscr{S}$ ごとに $V_{\lambda}$ の $D_{\lambda}$ 線形部分空間であり、N は加群の $\alpha$ の下で像です。 $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}W_{\lambda})$ は、加群 $\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda})$ の標準像と同一視されます。すべての $\lambda \in \mathscr{S},W_{\lambda}$ は元 $v\in V_{\lambda}$ の集合であるため、$s\in S_{\lambda}$ ごとに $\alpha (s\otimes v)$ 属するが N になります。

A-加群 $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ は、$\lambda \in \mathscr{S}$ ごとに型 $\lambda$ と同型です。 主張 a) は、$\alpha$ が同型であり、M が $(M_{\lambda})_{\lambda\in\mathscr{S}}$ (VIII, p. 65, 命題 4, a)) の直和であるという事実から導かれます。

$\lambda \in \mathscr{S}$ にしましょう。 $\alpha$ の制限を $\alpha_{\lambda}: S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}\rightarrow$ M で$S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ と表します。 With the notation of No. 3 applied to the $(A,D_{\lambda}$)-bimodule $S_{\lambda}$, we have

$$
\beta_{\lambda}=\gamma (\alpha_{\lambda}) =\mathscr{H}(\alpha_{\lambda})\circ \beta_{V_{\lambda}}
$$

ここで、最後の等式は VIII、p. 60 の後に続きます。従って、$\beta_{\lambda}$ は、$D_{\lambda}$ 線形準同型 $\mathscr{H}(\alpha_{\lambda})$ と $\beta_{V_{\lambda}}$ の合成です。 主張 b) は、命題 3、b) の VIII、p. 62 から続きます。

N を M の部分加群とします。$N =\bigoplus_{\lambda\in\mathscr{S}}(N\cap M_{\lambda})$ (VIII, p. 66, 系) があるため、c) は VIII の定理 2、p. 62 から求まります。

#### 系 {#alg-viii-s4-n7-cor-1 .statement tag=0051}

M を半単純A-加群とします。 M のすべての部分加群 N と $\mathscr{S}$ のすべての元 $\lambda$ に対して、同一視する Hom$_A(S_{\lambda},N)$ は Hom$_A(S_{\lambda},M)$ の $D_{\lambda}$ 線形部分空間写像のからなるとNに含まれる像。

a) 写像 $N\mapsto$ (Hom$_A(S_{\lambda},N)$)$_{\lambda\in\mathscr{S}}$ は、M の A-部分加群の集合から家族 $(W_{\lambda})_{\lambda\in\mathscr{S}}$ の集合までの全単射であり、$\lambda \in \mathscr{S}$ ごとに $W_{\lambda}$ はホム$_A(S_{\lambda},M)$の$D_{\lambda}$-リニア部分空間。

b) 逆全単射は家族 $(W_{\lambda})_{\lambda\in\mathscr{S}}$ を M の A-部分加群 $\sum_{\lambda\in\mathscr{S}}\sum_{w\in W_{\lambda}}w(S_{\lambda})$ に送信します。

これは、M の標準的記述に適用される命題 8, c) の再定式化です。

#### 命題 9 {#alg-viii-s4-prop-9 .statement tag=0052}

M と $M'$ を半単純A-加群として、それぞれ M と $M'$ の記述 $((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$ と $((V'_{\lambda})_{\lambda\in\mathscr{S}}, \alpha ')$ を考えます。 $\prod_{\lambda\in\mathscr{S}}$ Hom$_{D_{\lambda}}(V_{\lambda},V_{\lambda}')$ のすべての家族 $\boldsymbol{f}= (f_{\lambda})_{\lambda\in\mathscr{S}}$ には、次の図式が通勤する固有の A-線型写像 $\varphi (\boldsymbol{f})\in$ Hom$_A(M,M')$ が存在します。

$\bigoplus(S_{\lambda}\otimes_DV_{\lambda})^{\alpha}$ //M

$$
\lambda \in \mathscr{S}\lambda
$$

$$
\bigoplus(1_S\otimes f_{\lambda})
$$

$$
_{\lambda}\varphi (\boldsymbol{f})
$$

$\lambda \in \mathscr{S}$

$\bigoplus(S_{\lambda}\otimes_DV'_{\lambda})^{\alpha'}$ // $M'$。

$\lambda \in \mathscr{S}\lambda$

このように定義された写像 $\varphi :\prod_{\lambda\in\mathscr{S}}$ Hom$_{D_{\lambda}}(V_{\lambda},V'_{\lambda})\rightarrow$ Hom$_A(M,M')$ は、群同型となります。 $\lambda \in \mathscr{S}$ と $\alpha =\alpha '$ ごとに $M = M',V_{\lambda}= V'_{\lambda}$ がある場合、写像 $\varphi$ は、$\prod_{\lambda\in\mathscr{S}}$ 端$_{D_{\lambda}}(V_{\lambda})$ から端$_A(M)$ までの環同型です。

In view of the description of the isotypical components of M and $M'$ given in Proposition 8, a), this follows from Theorem 3 of VIII, p. 64 and Proposition 5, b) of VIII, p. 66.

#### 系 {#alg-viii-s4-n7-cor-2 .statement tag=0053}

M を半単純A-加群および $M'$ A-加群とします。 写像 $u\mapsto$ (ホム(1$_{S_{\lambda}}, u$))$_{\lambda\in\mathscr{S}}$ ホム$_A(M,M')$ から

$\prod_{\lambda\in\mathscr{S}}$ ホム$_{D_{\lambda}}$(ホム$_A(S_{\lambda},M)$、ホム$_A(S_{\lambda},M')$)

群同型です。 $M'$がMに等しいとき、環端$_A(M)$から環$\prod_{\lambda\in\mathscr{S}}$端$_{D_{\lambda}}$(Hom$_A(S_{\lambda},M)$)までの同型です。

これは、命題 9 を M の標準的記述と $M'$ のソクルに適用した再定式化です。

### 8. 多重度と半単純加群の長さ

#### 命題 10 {#alg-viii-s4-prop-10 .statement tag=0054}

M を半単純A-加群とします。 $(M_i)_{i\in I}$ を直和 M を持つ単純部分加群の族とします。以下のプロパティは同等です。

(i) M は有限長を持っています。

(ii) M はアルティンです。

(iii) M はネーター です。

(iv) M は有限に生成されます。

(v) I は有限です。

M がこれらの特性を持っている場合、M の長さは I の基数に等しいです。

集合 I が有限である場合、M は特性 (i)、(ii)、(iii)、および (iv) を持ちます。 集合 I が無限であると仮定します。 例 VIII、p. 2、加群の 2 までに、M はアルティンでもネーター でもありません。 有限長のすべての加群はアルティンとネーター (VIII、p. 2、命題 1) であるため、M には有限長もありません。最後に、部分加群 $M_i$ の有限数の M 属するから和までの各元なので、M は有限には生成されません。これにより、性質 (i) ～ (v) の同値が証明されます。これらが成立する場合、ロング(M) $=\sum_{i\in I}$ ロング(M$_i$) $=$ カード(I) (II, §1, No. 10, p. 213, 系 5) になります。

#### 命題 11 {#alg-viii-s4-prop-11 .statement tag=0055}

M を単純部分加群の家族 $(M_i)_{i\in I}$ の直和である半単純A-加群とします。すべての $\lambda \in \mathscr{S}$ について、添字 $i\in I$ の $I(\lambda )$ 集合で表し、$M_i$ は類 $\lambda$ になります。 $I(\lambda )$の基数は、左$D_{\lambda}$-ベクトル空間Hom$_A(S_{\lambda},M)$の次元に等しい。

型 $\lambda$ の A の同型成分は、$S_{\lambda}^{(I(\lambda))}$ (VIII, p. 65, 命題 4, b)) と同型です。 $D_{\lambda}$ ベクトル空間 Hom$_A(S_{\lambda},M)$ は Hom$_A(S_{\lambda},M_{\lambda})$ と同一視できるため、$D_{\lambda}^{(I(\lambda))}$ (No. 2) と同型です。これは命題を証明します。

すべての単純加群は原始的 (VIII、p. 45) であるため、すべての半単純加群は半原始的です。 M を半単純A-加群とし、$\lambda \in \mathscr{S}$ とします。 M の $\lambda$ の重複度は、VIII、p. 34 で定義された M の $\lambda$ の原始多重度 $[M :\lambda ]$ です。 命題 11 は等式に変換されます

(11) $[M :\lambda ] =$ 薄暗い$_{D_{\lambda}}$(ホム$_A(S_{\lambda},M)$)。

より一般的には、$((V_{\lambda})_{\lambda\in\mathscr{S}}, \alpha )$ が M の記述である場合、$[M :\lambda ]$ は dim$_{D_{\lambda}}(V_{\lambda})$ に等しいです。 VIII、p. 68 の命題 6 までに、

(12) $[M :\lambda ] =$ 薄暗い$_{D_{\lambda}}$(ホム$_A(M,S_{\lambda})$)

重複度 $[M :\lambda ]$ が有限のとき。 半単純A-加群 M と $M'$ は、すべての $\lambda \in \mathscr{S}$ に対して $[M :\lambda ] = [M':\lambda ]$ がある場合に限り、同型です。

M を半単純A-加群とします。次の性質を持つ基数 $\mathbf{I}$ が存在します: M の分解 $M =\bigoplus_{i\in I}M_i$ が単純加群の直和になるごとに、I の基数は $\mathbf{I}$ (VIII, p. 34、系 2)。この基数は半単純A-加群Mの長さと呼ばれ、long$_A(M)$またはlong(M)で表されます。 M が有限長を持つとき、この定義は、命題 10 によって、II, §1, No. 10、p. 212 の定義と互換性があります。

単純A-加群は長さ 1 の半単純A-加群で、公式があります

(13) 長い$_A(\bigoplus_{j\in J}M_j)=\sum_{j\in J}$ 長い$_A(M_j)$

すべての家族 $(M_j)_{j\in J}$ の半単純A-加群に。 命題 11 までに、

(14) 長い$_A(M) =\sum_{\lambda\in\mathscr{S}}$ 暗い$_{D_{\lambda}}$ ホム$_A(S_{\lambda},M)$。

この公式から$M_{\lambda}$まで適用により、$\lambda \in \mathscr{S}$ごとに$[M :\lambda ] =$長$_A(M_{\lambda})$が得られます。

A が体の場合、単純A-加群は次元 1 のベクトル空間です。すべての A-加群は半単純 (II, §7, No. 1, p. 292, 定理 1) であり、その長さは単に A (II, §7, No. 2, p. 293) 上のベクトル空間としての次元です。

### 練習問題 {#alg-viii-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。

[^1]: By Corollary 2 of VIII, p. 56, this definition coincides with that given in VII, §2, No. 2, p. 9
