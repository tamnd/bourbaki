---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 3
section_title: Conjugacy theorems
lang: ja
source: lie-vii-ix
book_pages: 20-27, 57-62
pdf_pages: 0030-0037, 0066-0071
extraction: native
subsections:
    - "no": 1
      title: ELEMENTARY AUTOMORPHISMS
      page: 20
      pdf_page: 30
    - "no": 2
      title: CONJUGACY OF CARTAN SUBALGEBRAS
      page: 22
      pdf_page: 32
    - "no": 3
      title: APPLICATIONS OF CONJUGACY
      page: 24
      pdf_page: 34
    - "no": 4
      title: CONJUGACY OF CARTAN SUBALGEBRAS OF SOLVABLE LIE ALGEBRAS
      page: 25
      pdf_page: 35
    - "no": 5
      title: LIE GROUP CASE
      page: 26
      pdf_page: 36
statements: 17
exercises: 18
content_sha256: 3924b8b318e743aa9b77aa48d9f81f722e2f17200ca109755829e56a844d7e27
translated_from: content/en/lie/VII/03_s3_conjugacy_theorems.md
translation_method: google
source_content_sha256: 2f94c55e447063be8de93e14acb2f2791b356caa14408181f0dee22d40d924cb
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 85c70cb4e6c15961655ebc1c24e5565d2ee87ba7ff1dd2e9074236253909d5bd
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 3。共役定理

この段落では、基礎体 $k$ は特性 0 です。

### 1. 初級自己同型

$\mathfrak{g}$をリー代数とします。 自己同型の群を Aut($\mathfrak{g}$) で表します。 If $x\in \mathfrak{g}$ and if ad $x$ is nilpotent, $e^{adx}\in$ Aut($\mathfrak{g}$) (Chap. I, §6, no. 8).

#### 定義 1 {#lie-vii-s3-def-1 .statement tag=00V0}

有限積 of 自己同型 of $\mathfrak{g}$ of 形 $e^{adx}$ で、$x$ nilpotent をもつものは、$\mathfrak{g}$ の初等自己同型と呼ばれます。 $\mathfrak{g}$ の初級自己同型の群は Aut$_e(\mathfrak{g})$ で表されます。

$u\in$ Aut($\mathfrak{g}$)$,ue^{adx}u^{-1}=e^{adu(x)}$ の場合。 Aut$_e(\mathfrak{g})$ は Aut($\mathfrak{g}$) の正規の部分群ということになります。 $k=\mathbf{R}$ または $\mathbf{C}$ の場合、Aut$_e(\mathfrak{g})$ は $\mathfrak{g}$ の内部自己同型の群 Int($\mathfrak{g}$) に含まれます (III, §6, no. 2 章、定義 2)。

\* 一般的な場合、Aut$_e(\mathfrak{g})$ は代数群 Aut($\mathfrak{g}$) の恒等式成分に含まれます。\*

#### 補題 1 {#lie-vii-s3-lem-1 .statement tag=00V1}

V を有限次元ベクトル空間、$\mathfrak{n}$ を $\mathfrak{a}=\mathfrak{g}\mathfrak{l}(V)$ からなるの冪零元の嘘部分代数とします。

(i) 写像 $x \rightarrow$ exp $x$ は、$\mathfrak{n}$ から単能性要素からなる $\mathbf{G}\mathbf{L}(V)$ の部分群 N への全単射である (II, §6, no. 1 章、注釈 4)。 $\mathfrak{n}=$ ログ (exp$\mathfrak{n}$) があります。 写像 $f \rightarrow f\circ$ ログは、$\mathfrak{n}$の多項式関数の代数から制限の代数、End(V)の多項式関数のNまでの同型です。

(ii) $x\in \mathfrak{n}$ と $a\in \mathfrak{a}$ の場合、

(exp ad$_{\mathfrak{a}}x$)$.a=$ (exp $x$)$a$(exp($-x$))。

(iii) $V'$ を有限次元ベクトル空間、$\mathfrak{n}'$ を $\mathfrak{n}$ から $\mathfrak{n}'$ までの$\mathfrak{g}\mathfrak{l}(V')$ からなるの冪零元、$\rho$ 準同型の嘘部分代数とする。 $\pi$ を exp$\mathfrak{n}$ から exp$\mathfrak{n}'$ までの写像 exp $x \rightarrow$ exp $\rho (x)$ とします。すると$\pi$は群準同型になります。

エンゲルの定理により、$\mathfrak{n}$が$\mathfrak{n}(n, k)$の部分代数となるように、同一視できるVを$k^n$とします（下三角の$\mathbf{M}_n(k)$からなるの嘘部分代数） 行列と対角線上の零)。 $s\geq 0$の場合、$\mathfrak{n}_s(n, k)$を$(x_{ij})_{1\leq i,j\leq n}\in \mathbf{M}_n(k)$の集合とし、$i-j < s$に対して$x_{ij}= 0$とします。それから

$$
[\mathfrak{n}_s(n, k),\mathfrak{n}_{s'}(n, k)]\subset \mathfrak{n}_{s+s'}(n, k)
$$

(Chap. II, §4, no. 6, Remark), and the Hausdorff series defines a polynomial map $(a, b) \rightarrow H(a, b)$ from $\mathfrak{n}(n, k)\times \mathfrak{n}(n, k)$ to $\mathfrak{n}(n, k)$ (Chap. II, §6, no. 5, Remark 3); this map makes $\mathfrak{n}(n, k)$ into a group (Chap. II, §6, no. 5, Prop. 4). 章著。 II, §6, no. 1、注意 4、写像 $x \rightarrow$ exp $x$ $\mathfrak{n}(n, k)$ から $1 +\mathfrak{n}(n, k)$ および $y \rightarrow$ log $y$ $1 +\mathfrak{n}(n, k)$ から $\mathfrak{n}(n, k)$ は逆全単射であり、多項式;章著II, §6, no. 5、提案 3、$\mathfrak{n}(n, k)$ に群法則 $(a, b) \rightarrow H(a, b)$ が与えられ、$1 +\mathfrak{n}(n, k)$ が $\mathbf{G}\mathbf{L}_n(k)$ の部分群とみなされる場合、これらの写像は群の同型になります。 主張補題の (i) と (iii) が続きます。 $x\in \mathfrak{n}$ にしましょう。 $\mathfrak{a}$ から $\mathfrak{a}$ までの $L_x,R_x$ 写像 $u \rightarrow xu, u \rightarrow ux$ で表します。これらは可換で零能です。 広告$_{\mathfrak{a}}x= L_x-R_x$ があるので、すべての $a\in \mathfrak{a}$ について、

(exp ad$_{\mathfrak{a}}x$)$a=$ (exp(L$_x-R_x$))$a=$ (exp $L_x$)(exp $R_{-x}$)$a$ (1)

$=\sum Li^{ix}$! $Rj\overset{j-x}{!}a=$ (経験値 $x$) $a$ (経験値 ($-x$))。

$i,j\geq 0$

補題 $1,\pi$ の記法は、$V'$ の $\mathfrak{n}$ の指定された表現 $\rho$ と互換性のある exp $\mathfrak{n}$ の線型表現と呼ばれます。 $k$ が $\mathbf{R}$、$\mathbf{C}$、または指数関数写像の性質による非離散完全ウルトラメトリック体、$\rho = L(\pi )$ の場合 (III, §4, no. 4 章、提案 8 の Cor. 2)。

#### 命題 1 {#lie-vii-s3-prop-1 .statement tag=00V2}

$\mathfrak{g}$ を $\mathfrak{g}$ のリー代数、$\mathfrak{n}$ 部分代数とし、ad$_{\mathfrak{g}}x$ がすべての $x\in \mathfrak{n}$ に対して nilpotent であるようにします。すると$e^{ad_{\mathfrak{g}}\mathfrak{n}}$はAut$_e(\mathfrak{g})$の部分群です。

これは補題 1 (i) の直後に続きます。

特に、$\mathfrak{n}$ が$\mathfrak{g},e^{ad_{\mathfrak{g}}\mathfrak{n}}$ の零根基である場合、$\mathfrak{g}$ の特殊な自己同型の群になります (I, §6, no. 8 章、定義 6)。

#### 注意 1 {#lie-vii-s3-n1-rem-1 .statement tag=00V3}

V を有限次元ベクトル空間、$\mathfrak{g}$ $\mathfrak{a}=\mathfrak{g}\mathfrak{l}$(V)、$\mathfrak{g}$ の $x$ 元を嘘部分代数とし、広告$_{\mathfrak{g}}x$ がゼロになるようにします。 次に、ad$_{\mathfrak{a}}n$ 拡大する ad$_{\mathfrak{g}}x$ となる $\mathfrak{a}$ の冪零元 $n$ が存在します。 確かに、$s, n$ を半単純とし、$x$ の無力成分とします。 ad$_{\mathfrak{a}}s$ と ad$_{\mathfrak{a}}n$ は ad$_{\mathfrak{a}}x$ の半単純と無能成分 (章 I, §5, no. 4、補題 2) なので、ad$_{\mathfrak{a}}s$ と ad$_{\mathfrak{a}}n$ は $\mathfrak{g}$ を安定させ、ad$_{\mathfrak{a}}s|\mathfrak{g}$ とad$_{\mathfrak{a}}n|\mathfrak{g}$ は半単純であり、ad$_{\mathfrak{g}}x$ の無力成分です。従って、ad$_{\mathfrak{g}}x=$ ad$_{\mathfrak{a}}n|\mathfrak{g}$ となり、主張であることが証明されます。 補助定理 1 (ii) を考慮すると、$\mathfrak{g}$ のすべての基本自己同型は、$u \rightarrow mum^{-1}$ ここで $m\in \mathbf{G}\mathbf{L}(V)$ の形式の $\mathfrak{a}$ の自己同型に拡張されます。

#### 注意 2 {#lie-vii-s3-n1-rem-2 .statement tag=00V4}

V を有限次元ベクトル空間とします。すべての $g\in \mathbf{S}\mathbf{L}$(V) について、$\varphi (g)$ を $\mathfrak{g}\mathfrak{l}(V)$ の自己同型 $x \rightarrow gxg^{-1}$ とします。それから

オート$_e(\mathfrak{g}\mathfrak{l}(V)) =\varphi (\mathbf{S}\mathbf{L}(V))$。

確かに、(1) により、Aut$_e(\mathfrak{g}\mathfrak{l}(V))$ は $\varphi (\mathbf{S}\mathbf{L}$(V)) に含まれ、反対の包含が代数から続きます。 III, §8, no. 9、提案 17 および (1)。同様の議論は、Aut$_e(\mathfrak{s}\mathfrak{l}(V))$ が $\varphi (\mathbf{S}\mathbf{L}(V))$ から $\mathfrak{s}\mathfrak{l}(V)$ の制限の元の集合であることを示します。

### 2. カルタン部分代数の共役

$\mathfrak{g}$ をリー代数、$\mathfrak{h}$ を$\mathfrak{g}$ の冪能部分代数、R を $\mathfrak{g}$ の $\mathfrak{h}$ の非ゼロ重みの集合、つまり $\mathfrak{g}^{\lambda}(\mathfrak{h})\not= 0$、cf. のような $\mathfrak{h}$ 上の線形形式 $\lambda \not= 0$ の集合とする。 §1, no. 3、提案 9 (iii)。 次のように仮定します。

$$
\mathfrak{g}=\mathfrak{g}^0(\mathfrak{h})\oplus \sum_{\lambda\in R}\mathfrak{g}^{\lambda}(\mathfrak{h})
$$

これは、$k$ が代数的に閉じている場合に当てはまります (§1, no. 3、提案 9 (i))。 $\lambda \in R$ と $x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$ の場合、広告 $x$ は無能です (§1, no. 3、提案 10 (iv))。 $e^{adx}$ によって生成された Aut$_e(\mathfrak{g})$ の $E(\mathfrak{h})$ 部分群で表します。$x$ は上記の形です。 $u\in$ Aut($\mathfrak{g}$) なら、$uE(\mathfrak{h})u^{-1}= E(u(\mathfrak{h}))$ は明らかです。

#### 補題 2 {#lie-vii-s3-lem-2 .statement tag=00V5}

(i) $\mathfrak{h}_r$ を $x\in \mathfrak{h}$ の集合とし、$\mathfrak{g}^0(x) =\mathfrak{g}^0(\mathfrak{h})$ とします。これは$x\in \mathfrak{h}$の集合で、すべての$\lambda \in R$に対して$\lambda (x)\not= 0$があり、ザリスキー位相の$\mathfrak{h}$では$\mathfrak{h}_r$が開いていて密集しています。

(ii) $\lambda_i$ が相互に異なるところに $R =\{\lambda_1, \lambda_2, . . . , \lambda_p\}$ を置きます。 F を公式によって定義される $\mathfrak{g}^0(\mathfrak{h})\times \mathfrak{g}^{\lambda_1}(\mathfrak{h})\times  \cdots  \times \mathfrak{g}^{\lambda_p}(\mathfrak{h})$ から $\mathfrak{g}$ までの写像とします。

$$
F(h, x_1, . . . , x_p) =e^{adx_1}. . . e^{adx_p}h
$$

この場合、F は支配多項式写像 (App. I) になります。

主張 (i) はクリアです。 (ii)を証明します。 $n=$ を$\mathfrak{g}$ 暗くしましょう。 $\lambda \in R$ と $x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$ の場合、(ad $x$)$^n= 0$ になります。したがって、$(y, x) \rightarrow e^{adx}y$ は $\mathfrak{g}\times \mathfrak{g}^{\lambda}(\mathfrak{h})$ から $\mathfrak{g}$ までの多項式写像です。 帰納法により、F は多項式であることがわかります。 $h_0\in \mathfrak{h}_r$ とし、DF を $(h_0,0, . . . ,0)$ における F の接線直線写像とします。 DF が全射的であることを示します。 $h\in \mathfrak{g}^0(\mathfrak{h}), F(h_0+h,0, . . . ,0) =h_0+h$ の場合、DF($h,0, . . . ,0$) $=h$ と Im(DF) $\supset \mathfrak{g}^0(\mathfrak{h})$ です。一方、$x\in \mathfrak{g}^{\lambda_1}(\mathfrak{h})$ については、

$F(h_0, x,0, . . . ,0) =e^{adx}h_0=h_0+$ (広告$x$)$.h_0+$ (広告2!$x$)$^2h_0+\cdots$

つまり、DF(0$, x,0, . . . ,0$) $=$ (広告 $x$)$.h_0=-$(広告 $h_0$)$x$; $\mathfrak{g}^{\lambda_1}(\mathfrak{h})$ の広告 $h_0$ 誘導する自己同型以来、私(DF) $\supset \mathfrak{g}^{\lambda_1}(\mathfrak{h})$。同様に、

イム(DF) $\supset \mathfrak{g}^{\lambda_i}(\mathfrak{h})$

すべての $i$ に対して、したがって DF の主観性が生じます。アプリの提案 4 I は F が優勢であることを示しています。

#### 命題 2 {#lie-vii-s3-prop-2 .statement tag=00V6}

$k$ が代数的に閉じていると仮定します。 $\mathfrak{g}$ を $\mathfrak{g}$ のリー代数、$\mathfrak{h}$、$\mathfrak{h}'$ カルタン部分代数とします。 $u(\mathfrak{h}) =u'(\mathfrak{h}')$ となるような $u\in E(\mathfrak{h})$ と $u'\in E(\mathfrak{h}')$ が存在します。

補題 2 の記法を保持します。$\mathfrak{h}$ と $\mathfrak{h}'$ がカルタン部分代数であるという事実から、$\mathfrak{g}^0(\mathfrak{h}) =\mathfrak{h}$ と $\mathfrak{g}^0(\mathfrak{h}') =\mathfrak{h}'$ が求まります。 補題 2 および App の Prop. 3 による。 $I, E(\mathfrak{h})\mathfrak{h}_r$ と $E(\mathfrak{h}')\mathfrak{h}'_r$ 含むは、ザリスキー 位相の $\mathfrak{g}$ の密な部分集合を開きます。したがって、$E(\mathfrak{h})\mathfrak{h}_r\cap E(\mathfrak{h}')\mathfrak{h}'_r\not=\emptyset$。他の語には、$u(h) =u'(h')$のような$u\in E(\mathfrak{h}), u'\in E(\mathfrak{h}'), h\in \mathfrak{h}_r, h'\in \mathfrak{h}'_r$が存在します。それから

$$
u(\mathfrak{h}) =u(\mathfrak{g}^0(\mathfrak{h})) =\mathfrak{g}^0(u(h)) =\mathfrak{g}^0(u'(h')) =u'(\mathfrak{h}')
$$

#### 系 {#lie-vii-s3-n2-cor-1 .statement tag=00V7}

$E(\mathfrak{h}) = E(\mathfrak{h}')$。

$u, u'$ を提案 2 のようにします。

$$
E(\mathfrak{h}) =uE(\mathfrak{h})u^{-1}= E(u(\mathfrak{h})) = E(u'(\mathfrak{h}')) =u'E(\mathfrak{h}')u^{'-1}= E(\mathfrak{h}')
$$

したがって系です。

この結果のため、$k$ が代数的に閉じている場合、単に E 群 $E(\mathfrak{h})$ で表します。ここで、$\mathfrak{h}$ は $\mathfrak{g}$ のカルタン部分代数です。

一般に、Aut$_e(\mathfrak{g})\not= E$ (たとえば、$\mathfrak{g}$ が nilpotent の場合、$\mathfrak{g}$ が非可換であれば、E 簡約するから単位元、さらにはけれどもの非自明な初等自己同型も存在します)。 However, it can be shown (Chap. VIII, §10, Exerc. 5) that Aut$_e(\mathfrak{g}) = E$ for $\mathfrak{g}$ semi-simple.

#### 定理 1 {#lie-vii-s3-thm-1 .statement tag=00V8}

$k$ が代数的に閉じていると仮定します。 $\mathfrak{g}$をリー代数とします。 群 E は Aut($\mathfrak{g}$) では通常であり、$\mathfrak{g}$ のカルタン部分代数の集合で推移的に動作します。

$\mathfrak{h}$ を $\mathfrak{g}$ のカルタン部分代数、および $v\in$ Aut($\mathfrak{g}$) とします。それから

$$
vE(\mathfrak{h})v^{-1}= E(v(\mathfrak{h})) = E(\mathfrak{h})
$$

したがって、Aut($\mathfrak{g}$) では $E(\mathfrak{h}) = E$ が正常です。 $\mathfrak{h}'$ が $\mathfrak{g}$ の他のカルタン部分代数である場合、提案$2,u^{'-1}u(\mathfrak{h}) =\mathfrak{h}'$ の記法および$u^{'-1}u\in E$ になります。

### 3. 共役の応用

#### 定理 2 {#lie-vii-s3-thm-2 .statement tag=00V9}

$\mathfrak{g}$をリー代数とします。

(i) $\mathfrak{g}$ のカルタン部分代数はすべて同じ次元、つまり rk($\mathfrak{g}$) であり、同じゼロ能類です。

(ii) 元 $x\in \mathfrak{g}$ は、$\mathfrak{g}^0(x)$ が $\mathfrak{g}$ のカルタン部分代数である場合にのみ正規です。このようにして、すべてのカルタン部分代数が取得されます。

(i) を証明するには、$k$ が代数的に閉じていると仮定できます (cf. §2、提案 3 および提案 6)。 no. 2 の 1 つ。 主張 (ii) は (i) と §2 から続きます。 1 (i) および (iv)。

#### 命題 3 {#lie-vii-s3-prop-3 .statement tag=00VA}

$\mathfrak{g}$ を $\mathfrak{g}$ のリー代数、$\mathfrak{g}'$ 部分代数とします。次の条件は同等です。

(i) $\mathfrak{g}$ の $\mathfrak{g}'$ 含む正則元、および rk($\mathfrak{g}$) $=$ rk($\mathfrak{g}'$);

(ii) $\mathfrak{g}$ の$\mathfrak{g}'$ 含むカルタン部分代数;

(iii) $\mathfrak{g}'$ のすべてのカルタン部分代数は $\mathfrak{g}$ のカルタン部分代数です。

(i) $=\Rightarrow$ (ii): rk($\mathfrak{g}$) $=$ rk($\mathfrak{g}'$) であり、$\mathfrak{g}$ に正規の $x\in \mathfrak{g}'$ が存在すると仮定します。 $\mathfrak{h}=\mathfrak{g}^0(x),\mathfrak{h}'={\mathfrak{g}'}^0(x) =\mathfrak{h}\cap \mathfrak{g}'$を入れてください。それから

rk($\mathfrak{g}'$)$\leq$ 暗い$\mathfrak{h}'\leq$ 暗い$\mathfrak{h}=$ rk($\mathfrak{g}$) $=$ rk($\mathfrak{g}'$)

それで$\mathfrak{h}=\mathfrak{h}'\subset \mathfrak{g}'$。これは(ii)を証明します。

(ii) $=\Rightarrow$ (iii): $\mathfrak{g}$ の $\mathfrak{g}'$ 含むカルタン部分代数 $\mathfrak{h}$ を仮定し、$\mathfrak{h}_1$ を $\mathfrak{g}'$ のカルタン部分代数とします。 $\mathfrak{h}_1$ が $\mathfrak{g}$ のカルタン部分代数であることを証明するには、$k$ が代数的に閉じていると仮定できます。 $E(\mathfrak{h})$ と $E'(\mathfrak{h})$ を、$\mathfrak{h}$ (no. 2) に関連付けられた $\mathfrak{g}$ と $\mathfrak{g}'$ の自己同型の群とします。 Thさんより1、$f(\mathfrak{h}) =\mathfrak{h}_1$となるような$f\in E'(\mathfrak{h})$が存在します。現在、$E'(\mathfrak{h})$ のすべての元は、$E(\mathfrak{h})$ の元によって誘発されます。実際、これを $e^{adx}$ について、$x\in {\mathfrak{g}'}^{\lambda}(\mathfrak{h}),\lambda \not= 0$ で検証するだけで十分です。この場合、${\mathfrak{g}'}^{\lambda}(\mathfrak{h})\subset \mathfrak{g}^{\lambda}(\mathfrak{h})$ が含まれることになります。したがって、$\mathfrak{h}_1$ は $\mathfrak{g}$ のカルタン部分代数です。

(iii) $=\Rightarrow$ (i): 条件 (iii) が満たされると仮定します。 $\mathfrak{h}$を$\mathfrak{g}'$のカルタン部分代数とします。これは$\mathfrak{g}$のカルタン部分代数なので、$\mathfrak{g}$の含む正則元(Th.2(ii))、一方、rk($\mathfrak{g}$)$=$dim($\mathfrak{h}$)$=$ rk($\mathfrak{g}'$)。

#### 系 {#lie-vii-s3-n3-cor-1 .statement tag=00VB}

$\mathfrak{h}$ を $\mathfrak{g}$ の nilpotent 部分代数とします。 部分代数 $\mathfrak{g}^0(\mathfrak{h})$ は、提案 3 の特性 (i)、(ii)、(iii) を持ちます。

実際、§2, no. 3 の提案 11 は、$\mathfrak{g}^0(\mathfrak{h})$ が性質 (ii) であることを示しています。

#### 命題 4 {#lie-vii-s3-prop-4 .statement tag=00VC}

$\mathfrak{g}$ をリー代数、$\mathfrak{g},c$ の $l$ 階数、$\mathfrak{g}$ のカルタン部分代数のゼロポテンシー 類、および $x\in \mathfrak{g}$ とします。 $\mathfrak{g}$ の $l$ 次元部分代数が存在し、その零能類は $\leq c$ であり、含む $x$ です。

T を不定数とします。 $k'=k(T)$と$\mathfrak{g}'=\mathfrak{g}\otimes_kk'$としましょう。 $\mathfrak{h}$ が $\mathfrak{g},\mathfrak{h}\otimes_kk'$ のカルタン部分代数で、$\mathfrak{g}'$ のカルタン部分代数である場合、$\mathfrak{g}'$ の階数は $l$ であり、$\mathfrak{g}'$ のカルタン部分代数のゼロポテンシー 類 $c$です。

選ぶ正則元 $y$/$\mathfrak{g}$。 §2, no. 2の記法により、$a_l(y)\not= 0$になります。 $\mathfrak{g}'$ の $a_l$ 多項式関数が拡大する $a_l$ であることも示します。次に、$k[T]$ の元 $a_l(x+ Ty)$ は係数 $a_l(y)$ が優勢です。特に$x+ Ty$は$\mathfrak{g}'$のレギュラーです。 $\mathfrak{h}'$を$\mathfrak{g}'$の広告($x+ Ty$)のゼロスペースとします。次に、$\mathfrak{h}'=l$ が暗くなり、$\mathfrak{h}'$ の無能類は $c$ になります。 $\mathfrak{k}=\mathfrak{h}'\cap (\mathfrak{g}\otimes_kk[T])$を入れてください。次に$\mathfrak{k}\otimes_{k[T]}k(T) =\mathfrak{h}'$。

$\varphi$ を $k[T]$ から $k$ までの準同型とし、$\varphi (T) = 0$ とし、$\psi$ を $\mathfrak{g}\otimes_kk[T]$ から $\mathfrak{g}$ までの準同型 $1\otimes \varphi$ とします。すると、$\psi (\mathfrak{k})$ は $\mathfrak{g}$ の部分代数であり、その無能性類は $\leq c$ であり、含む $\psi (x+ Ty) =x$ です。

無料の $k$[T] モジュールでは、$\mathfrak{g}\otimes_kk[T],\mathfrak{k}$ は階数 $l$ の部分加群であり、$(\mathfrak{g}\otimes_kk[T])/\mathfrak{k}$ は捩れなので、部分加群 $\mathfrak{k}$ は次の直接加数です。 $\mathfrak{g}\otimes_kk[T] ($代数、章。 VII, §4, no. 2、木曜日。 1)。したがって、薄暗い$_k\psi (\mathfrak{k}) =l$、これで証明が完成します。

### 4. 可解リー代数のカルタン部分代数の共役

$\mathfrak{g}$を可解リー代数とします。 $\mathfrak{g}$ の下降中心系列の項の $\mathscr{C}^{\infty}(\mathfrak{g})$ 共通部分で表します（I, §1, no. 5 章）。これは $\mathfrak{g}$ の特徴的なイデアであり、$\mathfrak{g}/\mathfrak{m}$ が零になるような $\mathfrak{g}$ の最小のイデア $\mathfrak{m}$ です。 $\mathscr{C}^{\infty}(\mathfrak{g})\subset [\mathfrak{g},\mathfrak{g}],\mathscr{C}^{\infty}(\mathfrak{g})$ は $\mathfrak{g}$ の無能のイデアであるため (第 1 章、コリント 5 章 I, §5, no. 3)。 no. 1の提案1により、$x\in \mathscr{C}^{\infty}(\mathfrak{g})$の$e^{adx}$の集合は、特別な自己同型の群に含まれるAut($\mathfrak{g}$)の部分群になります(I, §6, no. 8章、定義6)。

#### 定理 3 {#lie-vii-s3-thm-3 .statement tag=00VD}

$\mathfrak{g}$ を可解リー代数とし、$\mathfrak{h},\mathfrak{h}'$ を $\mathfrak{g}$ のカルタン部分代数とします。 $e^{adx}\mathfrak{h}=\mathfrak{h}'$となるような$x\in \mathscr{C}^{\infty}(\mathfrak{g})$が存在します。

$\mathfrak{g}= 0$ が自明である場合、dim$\mathfrak{g}$ について帰納法によって議論します。 $\mathfrak{n}$ を $\mathfrak{g}$ の最小非ゼロ可換イデアルとします。 $\varphi :\mathfrak{g}\rightarrow \mathfrak{g}/\mathfrak{n}$ を正規の射とします。 Then $\varphi (\mathscr{C}^{\infty}\mathfrak{g}) =\mathscr{C}^{\infty}(\mathfrak{g}/\mathfrak{n})$ (Chap. I, §1, no. 5, Prop. 4). $\varphi (\mathfrak{h})$ と $\varphi (\mathfrak{h}')$ は $\mathfrak{g}/\mathfrak{n}($§2, no. 1 のカルタン部分代数であるため、Cor.提案 4 の 2) では、帰納法の仮定までに、$e^{ad\varphi(x)}\varphi (\mathfrak{h}) =\varphi (\mathfrak{h}')$ となるような $x\in \mathscr{C}^{\infty}(\mathfrak{g})$ が存在します。 置き換えること $\mathfrak{h}$ $e^{adx}\mathfrak{h}$ により、$\varphi (\mathfrak{h}) =\varphi (\mathfrak{h}')$、他の語では、

$$
\mathfrak{h}+\mathfrak{n}=\mathfrak{h}'+\mathfrak{n}
$$

すると、$\mathfrak{h}$と$\mathfrak{h}'$は$\mathfrak{h}+\mathfrak{n}$のカルタン部分代数になります。 $\mathfrak{h}+\mathfrak{n}\not=\mathfrak{g}$の場合、帰納法の仮定から主張が証明されます。これから$\mathfrak{h}+\mathfrak{n}=\mathfrak{h}'+\mathfrak{n}=\mathfrak{g}$とします。

$\mathfrak{n}, [\mathfrak{g},\mathfrak{n}] =\{0\}$ または $[\mathfrak{g},\mathfrak{n}] =\mathfrak{n}$ の最小値によって。 $[\mathfrak{g},\mathfrak{n}] =\{0\}$ の場合、$\mathfrak{n}\subset \mathfrak{h}$ および $\mathfrak{n}\subset \mathfrak{h}'($§2, no. 1、提案 5)、したがって、$\mathfrak{h}=\mathfrak{h}+\mathfrak{n}=\mathfrak{h}'+\mathfrak{n}=\mathfrak{h}'$。 $[\mathfrak{g},\mathfrak{n}] =\mathfrak{n}$ であるため、$\mathfrak{n}\subset \mathscr{C}^{\infty}(\mathfrak{g})$ となる場合を検討する必要があります。理想的な $\mathfrak{n}$ は単純な $\mathfrak{g}$ モジュールです。 $\mathfrak{g}=\mathfrak{h}+\mathfrak{n}$ 以降、および $[\mathfrak{n},\mathfrak{n}] =\{0\}$ 以降、$\mathfrak{n}$ は単純な $\mathfrak{h}$ モジュールであることがわかります。 $\mathfrak{h}\cap \mathfrak{n}\not=\{0\}$なら$\mathfrak{n}\subset \mathfrak{h}$なので、$\mathfrak{g}=\mathfrak{h}$と$\mathfrak{h}'=\mathfrak{h}$です。ここで$\mathfrak{h}\cap \mathfrak{n}=\{0\}$と仮定します。次に、$\mathfrak{h}$ と $\mathfrak{h}'$ は同じ次元なので、$\mathfrak{g}=\mathfrak{h}\oplus \mathfrak{n}$ となり、したがって $\mathfrak{g}=\mathfrak{h}'\oplus \mathfrak{n}$ となります。

すべての $x\in \mathfrak{h}$ について、$f(x)$ を $\mathfrak{n}$ の一意元とし、$x-f(x)\in \mathfrak{h}'$ とします。 $x, y\in \mathfrak{h}$の場合、

$$
[x, y]-[x, f(y)]-[f(x), y] = [x-f(x), y-f(y)]\in \mathfrak{h}'
$$

だから$f([x, y]) = [x, f(y)] + [f(x), y]$。 §1, no. 3、Cor.提案 9 の場合、すべての $x\in \mathfrak{h}$ に対して $f(x) = [x, a]$ となるような $a\in \mathfrak{n}$ が存在します。 (広告 $a$)$^2(\mathfrak{g})\subset$ (広告 $a$)$(\mathfrak{n}) = 0$ があるので、すべての $x\in \mathfrak{h}$ について、

$$
e^{ada}x=x+ [a, x] =x-f(x)
$$

したがって、$e^{ada}(\mathfrak{h}) =\mathfrak{h}'$。 $a\in \mathscr{C}^{\infty}(\mathfrak{g})$からこれで証明が完了です。

#### 補題 3 {#lie-vii-s3-lem-3 .statement tag=00VE}

$\mathfrak{g}$ をリー代数、$\mathfrak{r}$ を根基、$\varphi$ 標準準同型を $\mathfrak{g}$ から $\mathfrak{g}/\mathfrak{r},v$ まで、$\mathfrak{g}/\mathfrak{r}$ の初等自己同型とします。 $\varphi \circ u=v\circ \varphi$ のような $\mathfrak{g}$ の基本自己同型 $u$ が存在します。

$v$ は形 $e^{adb}$ であると仮定できます。ここで、$b\in \mathfrak{g}/\mathfrak{r}$ と広告 $b$ はゼロポテントです。 $\mathfrak{s}$ を $\mathfrak{g}$ の Levi 部分代数とし (章 I, §6, no. 8、定義 7)、$a$ を $\varphi (a) =b$ となる $\mathfrak{s}$ の元とします。 ad$_{\mathfrak{s}}a$ は nilpotent であるため、ad$_{\mathfrak{g}}a$ も nilpotent であり (提案 3 の Cor. I, §6, no. 3 章)、$u=e^{ad_{\mathfrak{g}}a}$ は $\varphi \circ u=v\circ \varphi$ となるような $\mathfrak{g}$ の基本自己同型です。

#### 命題 5 {#lie-vii-s3-prop-5 .statement tag=00VF}

$\mathfrak{g}$をリー代数、$\mathfrak{r}$をその根基、$\mathfrak{h}$と$\mathfrak{h}'$を$\mathfrak{g}$のカルタン部分代数、$\mathfrak{g}$から$\mathfrak{g}/\mathfrak{r}$までの$\varphi$標準準同型とします。次の条件は同等です。

(i) $\mathfrak{h}$ と $\mathfrak{h}'$ は、$\mathfrak{g}$ の初等自己同型により共役になります。

(ii) $\varphi (\mathfrak{h})$ と $\varphi (\mathfrak{h}')$ は、$\mathfrak{g}/\mathfrak{r}$ の初級自己同型により共役になります。

(i) $=\Rightarrow$ (ii): これは明らかです。

(ii) $=\Rightarrow$ (i): 条件 (ii) が満たされると仮定し、(i) を証明します。 補題 3 までに、$\varphi (\mathfrak{h}) =\varphi (\mathfrak{h}')$ の場合に減ります。 $\mathfrak{g}$ の解ける部分代数である $\mathfrak{k}=$ $\mathfrak{h}+\mathfrak{r}=\mathfrak{h}'+\mathfrak{r}$ を置きます。すると、$\mathfrak{h}$と$\mathfrak{h}'$は$\mathfrak{k}$のカルタン部分代数なので、$e^{ad_{\mathfrak{k}}x}\mathfrak{h}=\mathfrak{h}'$となるような$x\in \mathscr{C}^{\infty}(\mathfrak{k})$が存在します(Th.3)。 $\mathfrak{k}/\mathfrak{r}$ は無能であるため、$\mathscr{C}^{\infty}(\mathfrak{k})\subset \mathfrak{r}$;一方、$\mathscr{C}^{\infty}(\mathfrak{k})\subset [\mathfrak{k},\mathfrak{k}]\subset [\mathfrak{g},\mathfrak{g}]$ なので、$x\in \mathfrak{r}\cap [\mathfrak{g},\mathfrak{g}]$;章著I, §5, no. 3、木曜日。 1、ad$_{\mathfrak{g}}x$ はゼロポテントなので、$e^{ad_{\mathfrak{g}}x}$ は $\mathfrak{h}$ を $\mathfrak{h}'$ に変換する $\mathfrak{g}$ の初等自己同型です。

### 5. リー群ケース

#### 命題 6 {#lie-vii-s3-prop-6 .statement tag=00VG}

$k$ が $\mathbf{R},\mathbf{C}$ または特性 0 の非離散完全超計量体であると仮定します。 $G$ を $k,e$ の単位元、$\mathfrak{g}$ のリー代数にわたる有限次元リー群とします。 $\mathfrak{h}$ カルタン部分代数の $\mathfrak{g},\mathfrak{h}_r$ 集合の正則元の $\mathfrak{g}$ 所属から $\mathfrak{h}$ まで。

(i) $\mathfrak{s}$ を、指数関数写像が定義されている $\mathfrak{s}$ の 0 の $\mathfrak{g},\mathfrak{s}_0$ 近傍と $h_0\in \mathfrak{h}_r$ の $\mathfrak{h}$ の補数であるベクトル空間とします。 写像 $(s, h) \rightarrow F(s, h) =$ (exp ad $s$)$.h$ $\mathfrak{s}_0\times \mathfrak{h}$ から $\mathfrak{g}$ は $(0, h_0)$ でのエターレです。

(ii) 写像 $(g, h) \rightarrow F'(g, h) =$ (Ad $g$)$.h$ $G\times \mathfrak{h}_r$ から $\mathfrak{g}$ は水没です。特に、像 $\Omega$ は開いています。すべての $x\in \Omega ,\mathfrak{g}^0(x)$ は、Ad(G) の $\mathfrak{g}$ 共役から $\mathfrak{h}$ のカルタン部分代数です。

(iii) $h_0\in \mathfrak{h}_r$ とします。 G の $e$ のいずれかの近傍 U の場合、集合 $\bigcup_{a\in U}$(Ad $a$)$(\mathfrak{h}_r)$

$\mathfrak{g}$の$h_0$の近傍です。

$h_0$ と $\mathfrak{s}$ を (i) のようにします。 T を $(0, h_0)$ における F の接線線形写像とします。 次に、すべての $h\in \mathfrak{h}$ に対して $F(0, h) =h$、つまりすべての $h\in \mathfrak{h}$ に対して $T(0, h) =h$ となります。 一方、$\mathfrak{s}_0$ が十分に小さい場合、$\mathfrak{s}_0$ から End($\mathfrak{g}$) までの写像 $s \rightarrow$ exp ad $s$ の 0 における接線線形写像は、$\mathfrak{s}$ から写像 $s \rightarrow$ ad $s$ になります。終了($\mathfrak{g}$)。 したがって、すべての $s\in \mathfrak{s}$ に対して $T(s,0) = [s, h_0]$ となります。 さて、広告 $h_0$ から商への通過によって引き起こされる $\mathfrak{g}/\mathfrak{h}$ から $\mathfrak{g}/\mathfrak{h}$ への写像は全単射です。 したがって、T は全単射であるため、(i) になります。 すべての $s\in \mathfrak{s}$ の exp ad $s=$ Ad exp $s$ が 0 に十分近いため、(iii) と (ii) の最初の主張が続きます。 すべての $x\in \Omega$ は、形 (広告 $a$)$(h)$ と $a\in G$ および $h\in \mathfrak{h}_r$ であるため、$\mathfrak{g}^0(x) =$ (広告 $a$)$(\mathfrak{g}^0(h)) =$ (広告 $a$)$(\mathfrak{h})$ は、部分代数になります広告(G)の下の$\mathfrak{g}$共役から$\mathfrak{h}$まで。

### 練習問題 {#lie-vii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
