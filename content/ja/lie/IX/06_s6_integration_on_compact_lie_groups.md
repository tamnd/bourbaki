---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 6
section_title: Integration on compact Lie groups
lang: ja
source: lie-vii-ix
book_pages: 333-346, 409-414
pdf_pages: 0340-0353, 0416-0421
extraction: native
subsections:
    - "no": 1
      title: PRODUCT OF ALTERNATING MULTILINEAR FORMS
      page: 333
      pdf_page: 340
    - "no": 2
      title: INTEGRATION FORMULA OF H. WEYL
      page: 334
      pdf_page: 341
    - "no": 3
      title: INTEGRATION ON LIE ALGEBRAS
      page: 339
      pdf_page: 346
    - "no": 4
      title: INTEGRATION OF SECTIONS OF A VECTOR BUNDLE
      page: 341
      pdf_page: 348
    - "no": 5
      title: INVARIANT DIFFERENTIAL FORMS
      page: 344
      pdf_page: 351
statements: 25
exercises: 13
content_sha256: f9de797231ac262d42fbc54db83d3927ce87197751473afb7a2ded1e249d3d67
translated_from: content/en/lie/IX/06_s6_integration_on_compact_lie_groups.md
translation_method: google
source_content_sha256: 746c6186434593ae87ea52347a193f0e294cca0a933dcfbfbd4549276c4b772c
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 609de64d1d7c0bd7905628aea56a1d73e3bc166cf7aa18bb09daa810e2bbe2f1
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 6。 コンパクト・リー群での統合

§4 のうち記法を保持します。 $w(G) =$カード(W$_G(T)$)を置きます。総質量 1 の G (それぞれ T) のハール測度を $dg$ (それぞれ $dt$) で表し、G (それぞれ T) の $n$ (それぞれ $r$) 次元で表します。

### 1. 積/交代的多重線形形式

Aを可換環、MをA-加群とします。それぞれの整数 $r\geq 0$ について、M 上の交代的 $r$ の線形形式の Alt$^r(M)$ A-加群を表します。それは、A-加群 $\wedge \wedge^r(M) ($代数の二重で識別できます。 III, §7, no. 4、提案 7)。 $u\in$ Alt$^s(M)$ と $v\in$ Alt$^r(M)$ とします。 (代数、Chap. III, §11, no. 2、例 3) を思い出してください。$u$ と $v$ の交代的積は、次のように定義されている元 $u\wedge v\in$ Alt$^{s+r}(M)$ です。

$$
(u\wedge v)(x_1, . . . , x_{s+r}) =\sum_{\sigma\in\mathfrak{S}_{s,r}}\varepsilon_{\sigma}u(x_{\sigma(1)}, . . . , x_{\sigma(s)})v(x_{\sigma(s+1)}, . . . , x_{\sigma(s+r)})
$$

ここで、$\mathfrak{S}_{s,r}$ は、置換の対称群 $\mathfrak{S}_{s+r}$ からなるの部分集合であり、制限から $1, s$ および $s+ 1, s+r$ は増加するです。

さあ、しましょう

0 $\longrightarrow M'\longrightarrow^i$ 月 $\longrightarrow^pM''\longrightarrow$ 0

それぞれ完全系列、自由A-加群、階数、$r, r+s$、$s$になります。

#### 補題 1 {#lie-ix-s6-lem-1 .statement tag=01EX}

Alt$^s(M'')\times$ Alt$^r(M')$ から Alt$^{s+r}(M)$ までの A 双線形写像が存在し、$(u, v) \rightarrow u\cap v$ で示され、次の 2 つのプロパティのいずれかによって特徴付けられます。

a) $u_1\in$ Alt$^s(M)$ 形 $(x_1, . . . , x_s) \rightarrow u(p(x_1), . . . , p(x_s))$ で表し、$v_1\in$ Alt$^r(M)$ を $M'$ の $x'_1, . . . , x'_r$ に対して $v_1(i(x'_1), . . . , i(x'_r)) =v(x'_1, . . . , x'_r)$ となるように形とします。次に$u\cap v=u_1\wedge v_1$。

b) M のすべての $x_1, . . . , x_s$ と $M'$ の $x'_1, . . . , x'_r$ について、

$$
(u\cap v)(x_1, . . . , x_s, i(x'_1), . . . , i(x'_r)) =u(p(x_1), . . . , p(x_s))v(x'_1, . . . , x'_r) \tag{1}
$$

写像 $\varphi :$ Alt$^s(M'')\otimes_A$Alt$^r(M')\rightarrow$ Alt$^{s+r}(M)$ で、$\varphi (u\otimes v) =u\cap v$ は階数の自由A-加群の同型になります。

形 $v_1$ 満たす条件 a) の存在は、$\wedge \wedge^r(M) ($代数の $\wedge \wedge^r(M')$ から直和因子部分加群までの $\wedge \wedge^r(i)$ 誘導する同型という事実から導き出されます。 III, §7, no. 2）。 $v_1$ をそのような形とします。 $u\cap v=u_1\wedge v_1$を入れます。 公式 (1) は満たされます。なぜなら、$1\leq k\leq r$ に $i(x'_k) =x_{s+k}$ を代入すると、$1\leq i\leq s$ の $p(x_{\sigma(i)})\not= 0$ が恒等式となる $\mathfrak{S}_{s,r}$ の元 $\sigma$ だけが恒等式置換になるからです。一方、公式 (1) 決定する $u\cap v$ は一意です。確かに、$(e'_1, . . . , e'_r)$ を、$M', (f''_1, . . . , f''_s)$ の基底 $M''$ の基底、および M の $f_1, . . . , f_s$ 元とします。 $1\leq i\leq s$の場合は$p(f_i) =f''_i$。すると、$(f_1, . . . , f_s, i(e'_1), . . . , i(e'_r))$ は M の基底 (代数、Chap. II, §1, no. 11、Prop. 21) となり、公式 (1) と書くことができます。

$$
(u\cap v)(f_1, . . . , f_s, i(e'_1), . . . , i(e'_r)) =u(f''_1, . . . , f''_s)v(e'_1, . . . , e'_r) \tag{2}
$$

ただし、Alt$^{s+r}(M)$ の元は、基底の値によって決まります。

前述のことから、条件 a) と b) 決定する積 $u\cap v$ はそれぞれ一意であることがわかります。この積が双線形であることは明らかです。最後に、公式 (2) から補題の最後の主張が続きます。

### 2. H. ワイルの統合公式

$e$ を G の単位元とし、$\overline{e}$ を $G/T$ の類とします。 同一視する $e$ での G の接線空間は $\mathfrak{g}$ と、$e$ での T の接線空間は $\mathfrak{t}$ で、$G/T$ の接線空間は $\overline{e}$ で $\mathfrak{g}/\mathfrak{t}$ となります。 $\mathbf{R}$-双線形写像を $(u, v) \rightarrow u\cap v$ で表します

Alt$^{n-r}(\mathfrak{g}/\mathfrak{t})\times$ Alt$^r(\mathfrak{t})\rightarrow$ Alt$^n(\mathfrak{g})$

数 1 で定義されています。

(第 III, §3, no. 13、提案 50) を思い出してください。写像 $\omega  \rightarrow \omega (e)$ は、G (それぞれ T) 上の次数 $n$ (それぞれ $r$) の左不変微分形のベクトル空間から同型になります。 空間 Alt$^n(\mathfrak{g})$ (それぞれ Alt$^r(\mathfrak{t})$)。さらに、$\mathbf{R}^*$ 簡約するから単位元までのすべての接続されたコンパクト部分群が、すべての $g\in G$ について Ad $g= 1$ を決定するので、G 上の次数 $n$ の左不変微分形も右不変であり、 内部自己同型の下での不変量 (第 III, §3, no. 16 章、提案 54 の訂正): これからは、G 不変微分形について簡単に説明します。

同様に、第 4 章から続きます。 III, §3, no. 16、提案 56 とその前、写像 $\omega  \rightarrow \omega (\overline{e})$ は、$G/T$ から空間 Alt$^{n-r}(\mathfrak{g}/\mathfrak{t})$ 上の G 不変微分形の次数 $n-r$ の空間から同型です。

$\omega_{G/T}$ が $G/T$ 上の次数 $n-r$ の G 不変微分形であり、$\omega_T$ が T 上の次数 $r$ の不変微分形である場合、一意の不変微分を $\omega_{G/T}\cap \omega_T$ で表します。 G の次数 $n$ の形

$$
(\omega_{G/T}\cap \omega_T)(e) =\omega_{G/T}(\overline{e})\cap \omega_T(e)
$$

最後に、$f: (G/T)\times T\rightarrow G$ は、$G\times T$ から G への商 (§5, no. 4) への写像 $(g, t) \rightarrow gtg^{-1}$ によって誘導された多様体の射を示していることを思い出してください。 $\alpha$ と $\beta$ がそれぞれ $G/T$ と T 上の微分形である場合、単に $(G/T)\times T$ 上の $\alpha \wedge \beta$ 形 pr$^*_1\alpha \wedge$ pr$^*_2\beta$ で表します。

$t\in T$ については、広告 $t$ から商への通過によって誘導された $\mathfrak{g}/\mathfrak{t}$ の広告$_{\mathfrak{g}/\mathfrak{t}}(t)$ 自己準同型で表します。置く

$\delta_G(t) =$ デット(広告$_{\mathfrak{g}/\mathfrak{t}}(t)-1$) $=\prod_{\alpha\in R(G,T)}(t^{\alpha}-1)$。 (3)

$x\in \mathfrak{t}$ と $\alpha \in R(G,T)$ としましょう。 $\widehat{\alpha}$ 元 $(2\pi i)^{-1}\delta (\alpha )$ の $\mathfrak{t}^*$ で表されるため、

((経験値 $x$)$^{\alpha}-$ 1)((経験値 $x$)$^{-\alpha}-1$) $= (e^{2\pi i\widehat{\alpha}(x)}-1)(e^{-2\pi i\widehat{\alpha}(x)}-1) = 4$ 罪$^2\pi \widehat{\alpha}(x)$。

$R_+(G,T)$ が基底 B に対して$R(G,T)$ の正の根の集合を表す場合、次のようになります。

$\delta_G$(exp $x$) $=\prod_{\alpha\in R_+(G,T)}4$ 罪$^2\pi \widehat{\alpha}(x)$,

特に、すべての $t\in T_r$ に対して $\delta_G(t)>0$ です。 $\delta_G(t) =\delta_G(t^{-1})$ が $t\in T$ であることにも注目します。

#### 命題 1 {#lie-ix-s6-prop-1 .statement tag=01EY}

$\omega_G, \omega_{G/T}$ と $\omega_T$ を、それぞれ次数 $n, n-r$ と $r$ の $G,G/T$ と T 上の不変微分形とします。 $\omega_G=$ $\omega_{G/T}\cap \omega_T$ の場合、

$$
f^*(\omega_G) =\omega_{G/T}\wedge \delta_G\omega_T
$$

明らかに、$\omega_{G/T}$ と $\omega_T$ はゼロではないと仮定できます。その場合、$(G/T)\times T$ の差分形 $(u, t) \rightarrow \omega_{G/T}(u)\wedge \omega_T(t)$ は次数 $n$ であり、どこもゼロではありません。したがって、$(G/T)\times T$ には次のような数値写像 $\delta$ が存在します。

$$
f^*(\omega_G)(u, t) =\delta (u, t)\omega_{G/T}(u)\wedge \omega_T(t)
$$

ここで、$h\in G,u\in G/T,t\in$ T について、$f(h.u, t) =$ (Int $h$)$f(u, t)$ があることに注目してください。 $\omega_G$ は内部自己同型の下で不変なので、直ちに $\delta (h.u, t) =\delta (u, t)$ が続き、したがって $\delta (u, t) =\delta (\overline{e}, t)$ になります。

$p:\mathfrak{g}\rightarrow \mathfrak{g}/\mathfrak{t}$ 商写像と $\varphi :\mathfrak{g}/\mathfrak{t}\rightarrow \mathfrak{g}$ 写像で定義されます。

$\varphi (p(X)) =$ (広告 $t^{-1}$)$X-X$ $X\in \mathfrak{g}$; (§5, no. 4, 補題 4) の接線写像を思い出してください。

$$
T_{(e,t)}(f) : T_e(G/T)\times T_t(T)\rightarrow T_t(G)
$$

$(z, tH)$ から $t(\varphi (z) +H)$ までは $z\in \mathfrak{g}/\mathfrak{t}, H\in \mathfrak{t}$ かかります。

$z_1, . . . , z_{n-r}$ を $\mathfrak{g}/\mathfrak{t},H_1, . . . , H_r$ の元 $\mathfrak{t}$ の元とします。それから

$$
f^*\omega_G(\overline{e}, t)(z_1, . . . , z_{n-r}, tH_1, . . . , tH_r)
$$

$T_{(\overline{e},t)}(f)$の計算により$=\omega_G(t)(t\varphi (z_1), . . . , t\varphi (z_{n-r}), tH_1, . . . , tH_r)$

$\omega_G$ は不変であるため、$=\omega_G(e)(\varphi (z_1), . . . , \varphi (z_{n-r}), H_1, . . . , H_r)$

$=\omega_{G/T}(\overline{e})(p\varphi (z_1), . . . , p\varphi (z_{n-r})).\omega_T(e)(H_1, . . . , H_r)$ (いいえ$.1$、補題 1)

= det($p\varphi$ )$\omega_{G/T}(\overline{e})(z_1, . . . , z_{n-r}).\omega_T(e)(H_1, . . . , H_r)$

$$
=\delta_G(t)\omega_{G/T}(\overline{e})(z_1, . . . , z_{n-r}).\omega_T(t)(tH_1, . . . , tH_r)
$$

$\omega_T$ は不変なので

$$
=\delta_G(t)(\omega_{G/T}\wedge \omega_T)(\overline{e}, t)(z_1, . . . , z_{n-r}, tH_1, . . . , tH_r)
$$

だから$f^*\omega_G(\overline{e}, t) =\delta_G(t)(\omega_{G/T}\wedge \omega_T)(\overline{e}, t)$;したがって、$\delta (\overline{e}, t) =\delta_G(t)$、したがって命題となります。

多様体 $G,T$ と $G/T$ に、それぞれ形 $\omega_G, \omega_T$ と $\omega_{G/T}$ で定義された方向を与えます。 These forms define invariant measures on $G,T$ and $G/T$ (Chap. III, §3, no. 16, Props. 55 and 56), also denoted by $\omega_G, \omega_T$ and $\omega_{G/T}$.

#### 補題 2 {#lie-ix-s6-lem-2 .statement tag=01EZ}

$\omega_G=\omega_{G/T}\cap \omega_T$ の場合、

$$
\int_G\omega_G=\int_{G/T}\omega_{G/T}.\int_T\omega_T
$$

G から $G/T$ までの正規の射を $\pi$ で表します。 $g\in G$ を、$t_1, . . . , t_{n-r}$ を $T_{\pi(g)}(G/T)$ の元とします。 同一視するファイバー $\pi^{-1}(\pi (g)) =gT$ を翻訳 $\gamma (g)$ で T にします。 関係 $\omega_G=\omega_{G/T}\cap \omega_T$ は、等式を意味します (微分可能および解析多様体、結果、11.4.5):

$$
\omega_G\llcorner (t_1, . . . , t_{n-r}) = (\omega_{G/T}(t_1, . . . , t_{n-r}))\omega_T
$$

したがって、$\int_{\pi}\omega_G=(\int_T\omega_T)\omega_{G/T}($微分可能かつ解析的多様体、結果、11.4.6)、および

$$
\int_G\omega_G=\int_{G/}\int_{T\pi}\omega_G=\int_T\omega_T.\int_{G/T}\omega_{G/T}
$$

(微分可能および分析多様体、結果、11.4.8)。

#### 補題 3 {#lie-ix-s6-lem-3 .statement tag=01F0}

局所準同型性$f_r($積分の下で$G_r$のメジャー$dg$の$(G/T)\times T_r$で逆像 V, §6, no. 6) は測度 $\mu\otimes \delta_Gdt$ で、$\mu$ は総質量 1 の $G/T$ における固有の G 不変測度です。

選ぶ $\omega_T$ (それぞれ $\omega_{G/T}$) によって定義される尺度が $dt$ に等しいような、最大値次数の T (それぞれ $G/T$) の不変微分形 $\omega_T$ (それぞれ $\omega_{G/T}$) (それぞれ $\mu$)。 $\omega_G=\omega_{G/T}\cap \omega_T$を入れてください。 補題 2 は、$\omega_G$ で定義されたメジャーが $dg$ に等しいことを意味します。 U を $(G/T)\times T_r$ のオープン部分集合として、$f_r$ 誘導する同型が U から $G_r$ のオープン部分集合 V になるようにします。 $\varphi$ を、V のコンパクトなサポートを持つ連続的な写像とします。 $\varphi$ から $G_r$ の $\varphi$ 拡大によっても表され、V の外側に消えます。私たちは持っています

$$
\int_V\varphi  dg=\int_V\varphi  \omega_G=\int_U(\varphi \circ f_r)f_r^*(\omega_G)
$$

$=\int_U(\varphi \circ f_r)\omega_{G/T}\wedge \delta_G\omega_T$ (プロップ$.1$)

$$
=\int_U(\varphi \circ f_r)d\mu.\delta_Gdt
$$

したがって補題。

#### 定理 1 (H. ワイル) {#lie-ix-s6-thm-1 .statement tag=01F1}

G 上の小節 $dg$ は、小節 $dg\otimes \frac{1}{w(G)}\delta_Gdt$ の $G\times T$ から G までの写像 $(g, t) \rightarrow gtg^{-1}$ の下の像です。

$\delta_G(t) =$ デット(広告$_{\mathfrak{g}/\mathfrak{t}}(t)-1$) $=\prod_{\alpha\in R(G,T)}(t^{\alpha}-1)$。

同様に (統合、章 V, §6, no. 3、提案 $4$)$,dg$ は、措置 $\mu\otimes \frac{1}{w(G)}\delta_Gdt$ の写像 $f: (G/T)\times T\rightarrow G$ の下の像です。

最後の主張を証明します。 §5, no. 1 および微分可能および解析的多様体、結果$, 10.1.3c)$ から、G**--** $G_r$ は G および T **--** $T_r$ は T で無視できることがわかります。さらに、写像 $f_r$ により $(G/T)\times T_r$ が得られます。 群 W (§5, no. 4, Prop. $4b$)$)$ を含む$G_r$ の主カバー。 定理は、補題 3 と統合、第 4 章から続きます。 V, §6, no. 6、提案 11。

#### 系 1 {#lie-ix-s6-thm-1-cor-1 .statement tag=01F2}

(i) $\varphi$ を G の可積分関数とし、バナッハ空間または $\overline{\mathbf{R}}$ の値とします。ほぼすべての $t\in T$、G の写像 $g \rightarrow \varphi (gtg^{-1})$ は $dg$ に積分可能です。 写像 $t \rightarrow \delta_G(t)\int_G\varphi (gtg^{-1})dg$ は T 上で積分可能であり、次のようになります。

$$
\int_G\varphi (g)dg=\frac{1}{w(G)}\int_T(\int_G\varphi (gtg^{-1})dg)\delta_G(t)dt \tag{4}
$$

(「ヘルマン・ワイルの統合公式」)。

(ii) $\varphi$ を G 上の正の可測値写像とします。ほとんどすべての $t\in T$ について、G 上の写像 $g \rightarrow \varphi (gtg^{-1})$ は可測です。 T 上の写像 $t \rightarrow \int_G^*\varphi (gtg^{-1})dg$ は測定可能であり、

$$
\int_G^*\varphi (g)dg=\frac{1}{w(G)}\int_T^*(\int_G^*\varphi (gtg^{-1})dg)\delta_G(t)dt \tag{5}
$$

写像 $f$ は、写像 $(g, t) \rightarrow gtg^{-1}$ から $G\times T\rightarrow G$ への通過によって商に誘導されるので、第 3 章の積分を適用するだけで十分です。 V, §5、6、8 および統合、第 6 章VII, §2。

#### 系 2 {#lie-ix-s6-thm-1-cor-2 .statement tag=01F3}

$\varphi$ を G の中心写像とし（つまり、G のすべての $g$ と $h$ に対して $\varphi (gh) =$ $\varphi (hg)$ となるように）、バナッハ空間または $\overline{\mathbf{R}}$ の値とします。

a$)\varphi$ は、T に対するその制限が測定可能な場合にのみ測定可能です。

b$)\varphi$ は、写像 $(\varphi |T)\delta_G$ が T 上で可積分である場合にのみ可積分です。その場合、次のようになります。

$$
\int_G\varphi (g)dg=\frac{1}{w(G)}\int_T\varphi (t)\delta_G(t)dt \tag{6}
$$

2 番目の射影を $p: G/T\times T\rightarrow T$ で示します。 $\varphi \circ f$ = $(\varphi |T)\circ p$;さらに、$\mu\otimes \frac{1}{w(G)}\delta_Gdt$ の小節の $p$ の下の像は $\frac{1}{w(G)}\delta_Gdt$ です。 系は Th から続きます。上記１およびＴｈ．統合の 1、第 1 章V, §6, no. 2、2 つの適切な写像 $f$ と $p$ に適用されます。

#### 系 3 {#lie-ix-s6-thm-1-cor-3 .statement tag=01F4}

H を G 含む T の連結閉部分群、そのリー代数 $\mathfrak{h}$、総質量 1 の H 上のハール測度 $dh$ とします。$\varphi$ を G 上の積分可能な中心写像とし、バナッハの値とします。 空間または $\overline{\mathbf{R}}$ に。すると、写像 $h \rightarrow \varphi (h$)det(Ad$_{\mathfrak{g}/\mathfrak{h}}(h)-1$) は可積分可能で H の中心となり、次のようになります。

$\int_G\varphi (g)dg=\frac{w(H)}{w(G)}\int_H\varphi (h$)det(広告$_{\mathfrak{g}/\mathfrak{h}}(h)-1$)$dh$。 (7)

確かに、写像 $h \rightarrow \varphi (h$)det(Ad$_{\mathfrak{g}/\mathfrak{h}}(h)-1$) は H 上の中心写像であり、T に対する制限は写像 $t \rightarrow \varphi (t)\delta_G(t)\delta_H(t)^{-1}$ です。したがって、系は Cor から続きます。 2 は G と H に適用されます。

#### 注意 1 {#lie-ix-s6-n2-rem-1 .statement tag=01F5}

コルで$\varphi = 1$を取ると、 3、取得します

$\int_H$ det(広告$_{\mathfrak{g}/\mathfrak{h}}(h)-1$)$dh=w(G)/w(H)$ (8)

そして特に

$$
\int_T\delta_G(t)dt=w(G) \tag{9}
$$

#### 注意 2 {#lie-ix-s6-n2-rem-2 .statement tag=01F6}

$\nu$ を、次のように定義される商 $T/W$ のメジャーとします。

$$
\int_{T/W}\psi (\tau )d\nu (\tau ) =\frac{1}{w(G)}\int_T\psi (\pi (t))\delta_G(t)dt
$$

ここで、$\pi$ は、$T/W$ に対する T の正規の射影を表します。コル。 2 は、標準射影 $G\rightarrow G/$Int(G) の下での測度 $dg$ の同相同型 $T/W\rightarrow G/$Int(G) (§2, no. 5、提案 5 の Cor. 1) 輸送測度 $\nu$ から像であることを意味します。

#### 注意 3 {#lie-ix-s6-n2-rem-3 .statement tag=01F7}

G が単純接続されていると仮定します。 A を $\mathfrak{t}$ のアルコーブとし、$dx$ を $\int_Adx= 1$ となるような $\mathfrak{t}$ のハール測度とする。次に、測定値 $\nu$ は、測定値 $\frac{1}{w(G)}\prod_{\alpha\in R_+(G,T)}4$ sin$^2\pi \widehat{\alpha}(x)dx$ を $\overline{A}$ で転送することによっても取得できます。

準同型性$\overline{A}\rightarrow T/W ($§5, no. 2、Cor。提案 2 の 1)。

#### 例 {#lie-ix-s6-n2-exa-1 .statement tag=01F8}

G を群 $\mathbf{S}\mathbf{U}(2,\mathbf{C})$ とし、T を対角線行列 (§3, no. 6) の部分群とします。 同一視する $\mathfrak{t}$ と $\mathbf{R}$ による基底の選択 $\mathfrak{t}($ の $\{iH\}$ 。引用）。 $A = 0, \pi$を入れてください。こちらは$\mathfrak{t}$の床の間です。 区間 $A = 0, \pi$ は、G の共役類の空間、G の元 $\theta$ と識別できます

$(e^{i\theta}$ 0 $)$

$\overline{A}$ 対応するから $-_{i\theta}$ の共役類 。 $d\theta$ をルベーグとします

0 $e$

$0, \pi$ で測定します。前述のことから、G のハール測度の $\overline{A}$ の像は $\frac{2}{\pi}$ sin$^2\theta  d\theta$ の測度であることがわかります。

### 3. リー代数での統合

#### 命題 2 {#lie-ix-s6-prop-2 .statement tag=01F9}

H を次元 $m,\mathfrak{h}$ の (実数) リー群のリー代数とします。 $\omega_H$ を H 上の次数 $m$ の右不変微分形とし、$\omega_{\mathfrak{h}}$ を次数 $m$ の一致するの $\mathfrak{h}$ 上の並進不変微分形とします。原点の$\omega_H(e)$。 我々は持っています

(経験値$_H$)$^*\omega_H=\lambda_{\mathfrak{h}}\omega_{\mathfrak{h}}$ (10)

ここで、$\lambda_{\mathfrak{h}}$ は、$\mathfrak{h}$ 上の Ad(H) 不変量写像であり、次のとおりです。

$\lambda_{\mathfrak{h}}(x) =$ det $\sum(p+$ 1)!1 (ad $x$)$^p$ for $x\in \mathfrak{h}$。

$p\geq 0$

$x, x_1, . . . , x_m$ を $\mathfrak{h}$ の元とします。我々は持っています

(経験値$^*\omega_H$)$_x(x_1, . . . , x_m) = (\omega_H$(経験値$x$))$(T_x$(経験値)($x_1$)$, . . . ,T_x$(経験値)($x_m$))。 Denote by $\varpi (x) :\mathfrak{h}\rightarrow \mathfrak{h}$ the right differential of the exponential at $x$ (Chap. III, §3, no. 17, Def. 8); by definition,

$y\in \mathfrak{h}$すべてに対して$T_x$(exp)($y$).(exp$x$)$^{-1}=\varpi (x).y$。

形 $\omega_H$ は右不変なので、次のようになります。

$(\omega_H$(経験値$x$))$(T_x$(経験値)($x_1$)$, . . . ,T_x$(経験値)($x_m$))

$=\omega_H(e)(\varpi (x).x_1, . . . , \varpi (x).x_m) =$ (デット $\varpi (x)$)$\omega_{\mathfrak{h}}(x_1, . . . , x_m)$;

thus, exp$^*\omega_H=\lambda_{\mathfrak{h}}\omega_{\mathfrak{h}}$, with $\lambda_{\mathfrak{h}}(x) =$ det $\varpi (x) =$ det$\frac{exp ad x-1}{ad x}$ (Chap. III, §6, no. 4, Prop. 12).

$h\in H$ にしましょう。広告 $h$ は $\mathfrak{h}$ の自己同型であるため、

広告 ((広告$h$)$(x)$) $=$ 広告$h\circ$ 広告$x\circ$ (広告$h$)$^{-1}$、

だから $\lambda_{\mathfrak{h}}$((広告 $h$)$(x)$) $=\lambda_{\mathfrak{h}}(x)$。したがって、写像 $\lambda_{\mathfrak{h}}$ は Ad(H) の下で不変です。これで命題の証明が完了します。

#### 注意 {#lie-ix-s6-n3-rem-1 .statement tag=01FA}

写像 $\lambda_{\mathfrak{g}}$ がコンパクト・リー群 G に関連付けられていると考えてください。 §2, no. 1の観点から、Th。 1、計算する $\lambda_{\mathfrak{g}}$ までは、$\mathfrak{t}$ の値がわかれば十分です。しかし、$x\in \mathfrak{t}$ の場合、$\mathfrak{g}$ の自己準同型と $x$ は半単純で、固有値 0 (重複度 $r$ 付き) となり、すべての $\alpha \in R(G,T),\delta (\alpha )(x)$ (重複度 1 付き) になります。すぐに次のことがわかります

$$
\lambda_{\mathfrak{g}}(x) =\prod\frac{e^{\delta(\alpha)(x)} - 1}{\delta(\alpha)(x)}=\frac{\delta_{\mathfrak{g}}(x)}{\pi_{\mathfrak{g}}(x)} \tag{11}
$$

$\alpha \in R(G,T)$

$\delta_{\mathfrak{g}}(x) =\delta_G$(exp $x$) と $\pi_{\mathfrak{g}}(x) =\prod_{\alpha\in R(G,T)}\delta (\alpha )(x) =$ det ad$_{\mathfrak{g}/\mathfrak{t}}(x)$ です。

$\omega_{G/T}$ を $G/T$ 上の次数 $n-r$ の不変微分形とし、$\omega_{\mathfrak{t}}$ を $\mathfrak{t}$ 上の次数 $r$ の変換不変微分形とします。 no. 1の記法を用いて、$\omega_{\mathfrak{g}}(0) =\omega_{G/T}(\overline{e})\cap \omega_{\mathfrak{t}}(0)$となるような$\mathfrak{g}$上の次数$n$の一意の並進不変微分形$\omega_{\mathfrak{g}}$を$\omega_{G/T}\cap \omega_{\mathfrak{t}}$で表します。

最後に、写像 $(g, x) \rightarrow$ (Ad $g$)$(x)$ から商への通過によって $G\times \mathfrak{t}$ から $\mathfrak{g}$ に誘導された多様体の $\psi : (G/T)\times \mathfrak{t}\rightarrow \mathfrak{g}$ 射で表します。

#### 命題 3 {#lie-ix-s6-prop-3 .statement tag=01FB}

$\omega_{\mathfrak{g}},\omega_{\mathfrak{t}},\omega_{G/T}$ を、それぞれの次数 $n, r, n-r$ の$\mathfrak{g},\mathfrak{t}$、$G/T$ の不変微分形とします。 $\omega_{\mathfrak{g}}=\omega_{G/T}\cap \omega_{\mathfrak{t}}$ の場合、

$$
\psi^*\omega_{\mathfrak{g}}=\omega_{G/T}\wedge \pi_{\mathfrak{g}}\omega_{\mathfrak{t}}
$$

ここで、$\pi_{\mathfrak{g}}$ は、$\pi_{\mathfrak{g}}(x) =\prod_{\alpha\in R(G,T)}\delta (\alpha )(x)$ によって定義される $\mathfrak{t}$ 上の写像です。

$\omega_{\mathfrak{g}}$ (それぞれ $\omega_{\mathfrak{t}}$) を原点とする一致する G (それぞれ T) 上の最大値次数の不変微分形を $\omega_G$ (それぞれ $\omega_T$) で表します。可換図式を考えてみましょう

$$
(G/T)\times \mathfrak{t}\longrightarrow^{\psi}\mathfrak{g}
$$

(ID,exp$_T$) exp$_G$。

$(G/T)\times T\longrightarrow^f$G

no. 2 と関係 exp$^*_T\omega_T=\omega_{\mathfrak{t}}$ の提案 1 を考慮して、等式を推定します。

$\psi^*$経験値$^*_G\omega_G=\omega_{G/T}\wedge \delta_{\mathfrak{g}}\omega_{\mathfrak{t}}$。

提案による。$2,\psi^*$exp$^*_G\omega_G= (\psi^*\lambda_{\mathfrak{g}})\psi^*\omega_{\mathfrak{g}}$。 写像 $\lambda_{\mathfrak{g}}$ は Ad(G) の下では不変なので、$\overline{g}\in G/T, x\in \mathfrak{t}$ に対して $(\psi^*\lambda_{\mathfrak{g}})(\overline{g}, x) =\lambda_{\mathfrak{g}}(x) =\frac{\delta_{\mathfrak{g}}(x)}{\pi_{\mathfrak{g}}(x)}$ が得られます。

したがって、形 $\psi^*\omega_G(\overline{g}, x)$ と $\omega_{G/T}(\overline{g})\wedge \pi_{\mathfrak{g}}(x)\omega_{\mathfrak{t}}(x)$ 一致するで、$\delta_{\mathfrak{g}}(x)$ は非ゼロ、つまり密なオープン部分集合 $(G/T)\times \mathfrak{t}_r$ 上にあります。したがって、それらは等しいので、命題となります。

$|\omega_G|=dg$ と $|\omega_T|=dt$ のような最大次数の不変微分形式 $\omega_G$ と T 上の $\omega_T$ を選択します。原点の $\omega_G(e)$ (それぞれ $\omega_T(e)$) とハール測度 $dz$ (それぞれ $dx$) に一致する $\mathfrak{g}$ (それぞれ $\mathfrak{t}$) 上の並進不変微分形式を $\omega_{\mathfrak{g}}$ (それぞれ $\omega_{\mathfrak{t}}$) で表します。 $|\omega_{\mathfrak{g}}|$ (それぞれ $|\omega_{\mathfrak{t}}|$)。 推論を no. 2 と同様に準用すると、次の命題が得られます。

#### 命題 4 {#lie-ix-s6-prop-4 .statement tag=01FC}

$\mathfrak{g}$ の$dz$ は、$dg\otimes \frac{1}{w(G)}\pi_{\mathfrak{g}}dx$ の$G\times \mathfrak{t}$ から $\mathfrak{g}$ までの適切な写像 $(g, x) \rightarrow$ (Ad $g$)$(x)$ の下の像です。

コルの類似点の主張と証明は読者に任せます。 no. 2の1から3と注意の1から3。たとえば、$\varphi$ を $\mathfrak{g}$ の可積分関数とします (バナッハ空間または $\overline{\mathbf{R}}$ では値)。それから

$\int_{\mathfrak{g}}\varphi (z)dz=\frac{1}{w(G)}\int_{\mathfrak{t}}(\int_G\varphi$((広告$g$)$x$)$dg)\pi_{\mathfrak{g}}(x)dx$, (12)

特に、$\varphi$ が Ad(G) の下で不変の場合、

$$
\int_{\mathfrak{g}}\varphi (z)dz=\frac{1}{w(G)}\int_{\mathfrak{t}}\varphi (x)\pi_{\mathfrak{g}}(x)dx \tag{13}
$$

### 4. ベクトルバンドルの切断の統合

この数と次のX で、類 $C^r$ $(1\leq r\leq  \infty )$ の実数多様体を、有限次元の局所的に表します。

Y を類 $C^r$ の多様体とします。 $r <\infty$ の場合、$\mathscr{C}^r(X; Y)$ から $\mathscr{C}(X; J^r(X,Y)) ($ までの写像 $f \rightarrow$ $j^r(f)$ を考慮します。微分可能および解析的多様体、結果、12.3.7)。 $\mathscr{C}(X; J^r(X,Y))$ 上のコンパクトな収束の位相のこの写像の下の逆像は、$\mathscr{C}^r(X; Y)$ 上のコンパクトな $C^r$ 収束の位相と呼ばれます。それは、K 上の均一 $C^r$ 収束のトポロジーの上界 (微分可能および解析多様体、結果、12.3.10) であり、K は X のコンパクト部分集合の集合を通過します。

$r$ = $\infty$ の場合、コンパクト $C^k$ 収束のトポロジーの $\mathscr{C}^{\infty}(X; Y)$ 上界に対するコンパクト $C^{\infty}$ 収束の位相を、他の語では標準単射が適用される最も粗い位相を呼び出します。 $\mathscr{C}^{\infty}(X; Y)\rightarrow \mathscr{C}^k(X; Y)$は$0\leq k <\infty$まで続きます。

E を類 $C^r$ の基底 X との実ベクトルバンドルとし、$\mathscr{S}^r(X; E)$ を類 $C^r$ の E の切断のベクトル空間とします。この数では、コンパクトな $C^r$-収束の位相とも呼ばれる、$\mathscr{C}^r(X; E)$ 上のコンパクトな $C^r$-収束の位相によって誘導される $\mathscr{S}^r(X; E)$ 位相を与えます。それは、$\mathscr{S}^r(X; E)$ を完全に分離された局所凸トポロジカルベクトル空間にします (cf. 微分可能および解析的多様体、結果、15.3.1 およびスペクトル理論、準備中)。

ここで、H を類 $C^r$ の左演算のリー群、$m: H\times X\rightarrow X$ 法則とします。 $h\in H, x\in X$に$hx=m(h, x)$を入れます。 E を類 $C^r$ の基底 X との H-バンドルベクトルとします (章 III, §1, no. 8、定義 4)。 $s\in \mathscr{S}^r(X; E)$ と $h\in H$ については、E の $^hs$ 切断 $x \rightarrow h.s(h^{-1}x)$ で表します。 写像 $(h, s) \rightarrow^hs$ は、空間 $\mathscr{S}^r(X; E)$ の H の演算の法則です。

#### 補題 4 {#lie-ix-s6-lem-4 .statement tag=01FD}

演算 $H\times \mathscr{S}^r(X; E)\rightarrow \mathscr{S}^r(X; E)$ の法則は連続です。

$\mathscr{S}^r(X; E)$ の位相および位相の定義を考慮して、第 1 章。 X, §3, no. 4、木曜日。 3 では、任意の整数 $k\leq r$、写像 $f: H\times X\times \mathscr{S}^k(X; E)\rightarrow J^k(X; E)$ について、$f(h, x, s) =j_x^k(^hs)$ が連続であることを証明すれば十分です。 $h\in H$ については、X の $\tau_h$ (それぞれ $\theta_h$) 自己同型 $x \rightarrow hx$ (それぞれ E) で表します。 定義する写像

$$
f_1:H\times X\rightarrow J^k(X,X)
$$

$$
f_2:H\times E\rightarrow J^k(E,E)
$$

$$
g:H\times X\times \mathscr{S}^k(X; E)\rightarrow J^k(X,E)
$$

$f_1(h, x) =j^k_x(\tau_h), f_2(h, v) =j_v^k(\theta_h), g(h, x, s) =j_{hx}^k(s)$ によって。我々は持っています

$$
f(h, x, s) =f_2(h, s(h^{-1}x))\circ g(h^{-1}, x, s)\circ f_1(h^{-1}, x)
$$

従って、微分可能と解析多様体、結果、12.3.6 により、$f_1, f_2$ と $g$ が連続であることを証明するだけで十分です。

これで $g$ は合成写像になります

$$
H\times X\times \mathscr{S}^k(X; E)-------\longrightarrow^{(m,Id)}X\times \mathscr{S}^k(X; E)
$$

$$
-------\longrightarrow^{(Id,j^k)}X\times \mathscr{C}(X; J^k(X,E))\longrightarrow^{\varepsilon}J^k(X,E)
$$

with $\varepsilon (x, u) =u(x)$; the map $\varepsilon$ being continuous (General Topology, Chap. X, §3, no. 4, Cor. 1 of Th. $3$)$,g$ is continuous.

$(h_0, x_0)\in H\times X$ にしましょう。 $f_1$ が $(h_0, x_0)$ で連続であることを証明します。 X のチャート $(U, \psi ,F)$ と $(V, \chi ,F')$ と、$x_0\in U, h_0\in \Omega$ と $m(\Omega \times U)\subset V$ のような H のオープン部分集合 $\Omega$ が存在します。これらのチャートで$J^k(X,X)$の式を使用すると、証明、$1\leq l\leq k$、$\Omega \times U$から$P_l(F; F')$までの写像$(h, x) \rightarrow \Delta^l_x(\tau_h)$の$(h_0, x_0)$での連続性が$\Delta^l_x(\tau_h)(v) =$$\frac{1}{l!}D^l\tau_h(x).v$に縮小されます。 $v\in F ($微分可能および解析的多様体、結果、12.2)。しかし、$D^l\tau_h(x)$ は単に $x$ に関する $m(h, x)$ の $l$ 番目の偏導関数であり、仮定だけ連続です。従って、$f_1$ は連続です。 $f_2$が連続である証明は類似しているので、補題です。

#### 命題 5 {#lie-ix-s6-prop-5 .statement tag=01FE}

群 H がコンパクトで、総質量 1 の H のハール測度を $dh$ で表すと仮定します。$s$ を類 $C^r$ の E の切断とします。 $s^{\sharp}$ ベクトル積分 $\int_H^hs dh$ で表します。この場合、$s^{\sharp}$ は類 $C^r$ の E の切断であり、H の下で不変です。 $x\in X$ の場合、$s^{\sharp}(x) =\int_Hhs(h^{-1}x)dh\in E_x$ になります。 $\mathscr{S}^r(X; E)$ の自己準同型 $s \rightarrow s^{\sharp}$ は、H 不変量切断の部分空間上で射影です。

H から $\mathscr{S}^r(X; E)$ までの写像 $h \rightarrow^hs$ を考えてみましょう。 補題 4 によって連続です。空間 $\mathscr{S}^r(X; E)$ が分離されて完了しているため、$s^{\sharp}=$ $\int_H^hs dh$ 属するから$\mathscr{S}^r(X; E) ($ 整、第 3 章III, §3, no. 3、コル。 2)。 $\mathscr{S}^r(X; E)$ から $E_x$ までの線形写像 $s \rightarrow s(x)$ は連続なので、すべての $x\in X$ に対して $s^{\sharp}(x) =$ $\int_H^hs(x)dh$ が得られます。 $s^{\sharp}$ が H の下で不変であることは明らかです。 $s$ が H 不変量切断である場合、$s^{\sharp}=s$ があり、したがって最後の主張になります。

#### 系 1 {#lie-ix-s6-prop-5-cor-1 .statement tag=01FF}

F をバナッハ空間、$\rho : H\rightarrow \mathbf{G}\mathbf{L}(F)$ 解析関数線型表現、$f\in \mathscr{C}^r(X; F)$ とします。 $x\in X$には、

$$
f^{\sharp}(x) =\int_H\rho (h).f(h^{-1}x)dh
$$

次に、$f^{\sharp}$ は X から F までの類 $C^r$ の射であり、H の演算と互換性があります。 $x\in X$ については、次のようになります ($\tau_h$ は X の自己同型 $x \rightarrow hx$ を示します)

$$
d_xf^{\sharp}=\int_H(\rho (h)\circ d_{h^{-1}x}f\circ T_x(\tau_{h^{-1}}))dh\in \mathscr{L}(T_x(X); F) \tag{14}
$$

最初の主張は、演算 $(h; (x, f)) \rightarrow (hx, \rho (h).f)$ の法則を装備したバンドル $X\times$ F に適用される命題に続きます。 2 番目は、「統合」第 4 章からの続きです。 III, §3, no. 2、提案 2、適用からベクトルの積分 $f^{\sharp}$ 準同型 $d_x:\mathscr{C}^r(X; F)\rightarrow \mathscr{L}(T_x(X); F)$ は、コンパクトな $C^r$ 収束の位相の定義によって連続です。

#### 系 2 {#lie-ix-s6-prop-5-cor-2 .statement tag=01FG}

F をバナハ空間, $f\in \mathscr{C}^r(X; F)$ とします。置く

$$
f^{\sharp}(x) =\int_Hf(hx)dh
$$

$x\in X$の場合。 写像 $f^{\sharp}$ は類 $C^r$ の$f^{\sharp}(hx) =f^{\sharp}(x)$ は $x\in X$、$h\in H$ です。

#### 系 3 {#lie-ix-s6-prop-5-cor-3 .statement tag=01FH}

F を、X 上の次数 $p$ の差分形の Banach 空間、$p$ 整数 $\geq 0,^k\Omega^p(X; F)$ 空間とし、F に値を付け、 類 $C^k(2\leq k+ 1\leq r)$。 $\omega \in^k\Omega^p(X; F)$には$\omega^{\sharp}=\int_H\tau_h^*\omega  dh$を入れてください。この場合、写像 $\omega  \rightarrow \omega^{\sharp}$ は $^k\Omega^p(X; F)$ 上の射影であり、その像は H 不変量形の部分空間です。すべての $\omega \in^k\Omega^p(X; F)$ に対して $d(\omega^{\sharp}) = (d\omega )^{\sharp}$ があります。

最初の主張は、ベクトル H バンドル Alt$^p(T(X); F)$ に適用される命題の後に続きます (第 III, §1, no. 8、例)。 2 番目の主張を証明するには、統合の観点から十分です。 III, §3, no. 2、提案 2、最初 (または 2 番目) 空間にコンパクトな $C^k$ 収束 (それぞれ $C^{k-1}$ 収束) の位相が与えられたときに写像 $d:^k\Omega^p(X; F)\rightarrow^{k-1}\Omega^{p+1}(X; F)$ が連続であることを証明します。しかし、これは、半ノルム (スペクトル理論、準備中) と、$d$ が位数 $\leq 1 ($ 微分可能かつ解析的多様体、結果、14.4.2) の微分演算子であるという事実によって、これらのトポロジーの定義からすぐに得られます。

### 5. 不変微分形

X を、類 $C^{\infty}$ の局所有限次元実数多様体とし、$(g, x) \rightarrow gx$ を、連結コンパクト・リー群の類 $C^{\infty}$ の左演算の法則とします。 X で。 $g\in G$ の場合は、X の $\tau_g$ 自己同型 $x \rightarrow gx$ で表します。 X 上の類 $C^{\infty}$ の実微分形の $\Omega (X)$ 代数で表します (微分可能および解析多様体、結果、8.3.1)。

$\mathfrak{g}$ の元 $\xi$ については、X (III, §3, no. 5 章) では $D_{\xi}$ 対応するベクトル体と $\theta (\xi ), i(\xi )$ で表します。 $\Omega$(X) に対応する演算子を追加すると、公式になります (微分可能および解析多様体、結果、8.4.5 および 8.4.7)

$$
\theta (\xi )\omega =d(i(\xi )\omega ) +i(\xi )d\omega \tag{15}
$$

$$
d_**
$$

$$
(\tau_{expt\xi}\omega ) =\tau_{expt\xi}(\theta (\xi )\omega ) \tag{16}
$$

$$
dt
$$

すべての $g\in G$ に対して $\tau_g^*\omega =\omega$ であれば、微分形 $\omega \in \Omega (X)$ は不変です。 公式 (16) により、これはすべての $\xi \in \mathfrak{g}$ の $\theta (\xi )\omega = 0$ に相当します。 X 上の不変微分形の $\Omega (X)^G$ 空間で表します。 $\omega \in \Omega (X)^G$ の場合、$d\omega \in \Omega (X)^G$ があるため、$\Omega (X)^G$ は複素数 $(\Omega (X), d)$ の部分複素数になります。

#### 定理 2 {#lie-ix-s6-thm-2 .statement tag=01FI}

標準単射 $\iota :\Omega (X)^G\rightarrow \Omega (X)$ は複素数のホモトプリズムです (Algèbre, Chap. X, p. 33, déf. 5)。 写像 $\omega  \rightarrow \omega^{\sharp}=\int_G\tau_g^*\omega  dg$ はホモトピズムであり、ホモトピーまでの逆です。特に、写像 $H(\iota ) : H(\Omega (X)^G)\rightarrow H(\Omega (X))$ は全単射です。

コル著no. 4、写像 $\omega  \rightarrow \omega^{\sharp}$ の 3 は、$\Omega (X)$ から $\Omega (X)^G$ までの複合体の射であり、誘導するは部分複合体 $\Omega (X)^G$ 上の同一性です。したがって、定理を証明するには、次数 $-1$ の等級付けされた構成する準同型 $s:\Omega (X)\rightarrow \Omega$(X) で十分です。

$\omega \in \Omega (X)$ 全員に対して $\omega^{\sharp}-\omega = (d\circ s+s\circ d)(\omega )$。 (17)

統合の補題 1、章 IX, §2, no. 4、および§2, no. 2の注意 1 により、コンパクトサポートの$\mathfrak{g}$ にプラスの尺度 $d\xi$ が存在し、その指数写像の下の像は$dg$ に等しくなります。 $\omega \in \Omega$(X)の場合は、

$$
s(\omega ) =\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*(i(\xi )\omega ).d\xi \}dt
$$

公式 (17) が満足していることを示さなければなりません。コルの証明のように。 1 (no. 4)、公式を確認します

$$
ds(\omega ) =\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*d(i(\xi )\omega ).d\xi \}dt
$$

公式 (15) と (16) から等式を導き出します。

$$
ds(\omega ) +s(d\omega ) =\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*(d(i(\xi )\omega ) +i(\xi )d\omega ).d\xi \}dt
$$

$$
=\int_0^1\{\int_{\mathfrak{g}}\tau_{expt\xi}^*(\theta (\xi )\omega ).d\xi \}dt
$$

$$
=\int_{\mathfrak{g}}\{\int_0^1\frac{d}{dt}(\tau_{expt\xi}^*\omega )dt\}d\xi
$$

$$
=\int_{\mathfrak{g}}(\tau_{exp\xi}^*\omega -\omega )d\xi
$$

$$
=\omega^{\sharp}-\omega
$$

したがって、Th。 2.

X = G の場合、定理を左変換により G の作用に適用します。 G 上の微分形と単位元での値を関連付けると、$\Omega (G)^G$ から交代的の段階的代数 Alt($\mathfrak{g}$) への同型が得られることを思い出してください (第 III, §3, no. 13、提案 50)。 $\mathfrak{g}$の形。 Alt($\mathfrak{g}$)で同一視する $\Omega (G)^G$ この同型を利用します。 The operator $d$ is then given by the formula (Chap. III, §3, no. 14, Prop. 51)

$$
d\omega (a_1, . . . , a_{p+1})
$$

$$
=\sum_{i<j}(-1)^{i+j}\omega ([a_i, a_j], a_1, . . . , a_{i-1}, a_{i+1}, . . . , a_{j-1}, a_{j+1}, . . . , a_{p+1})
$$

Alt$^p(\mathfrak{g})$ の $\omega$ と $\mathfrak{g}$ の $a_1, . . . , a_{p+1}$ です。

$\xi \in \mathfrak{g}$ について、$L_{\xi}$ を対応する左不変ベクトル体とします (右変換による G 自体の作用によって定義されます、cf. 章 III, §3, no. 6)。演算子 $\theta (L_{\xi}), i(L_{\xi})$ は、左変換で定義された $\Omega (G)$ 上の G の作用と交換するため、誘導する演算子 $\Omega (G)^G$ の $\theta (\xi ), i(\xi )$ となります。前述の同定を使用すると、これらは公式 (微分可能および解析多様体、結果、8.3.2 および 8.4.2) で表されます。

$$
(\theta (\xi )\omega )(a_1, . . . , a_p) =-\sum_i\omega (a_1, . . . , a_{i-1},[\xi , a_i], a_{i+1}, . . . , a_p)
$$

$$
(i(\xi )\omega )(a_1, . . . , a_{p-1}) =\omega (\xi , a_1, . . . , a_{p-1})
$$

Alt$^p(\mathfrak{g})$ の $\omega$ と $\mathfrak{g}$ の $a_1, . . . , a_p$ です。

The subcomplex $^G\Omega (G)^G$ of biinvariant forms (Chap. III, §3, no. 13) can be identified with the subcomplex Alt($\mathfrak{g}$)$^G$ of alternating multilinear forms on $\mathfrak{g}$ invariant under the adjoint representation (that is, such that $\theta (\xi )\omega = 0$ for all $\xi \in \mathfrak{g}$). したがって、可換な図式の複素数が得られます。

$$
^G\Omega (G)^G\longrightarrow \Omega (G)^G\longrightarrow \Omega (G)
$$

(18)

Alt($\mathfrak{g}$)$^G\longrightarrow$ Alt($\mathfrak{g}$)

ここで、水平矢印は標準単射、垂直矢印は写像 $\omega  \rightarrow \omega (e)$ によって引き起こされる同型です。

#### 系 1 {#lie-ix-s6-thm-2-cor-1 .statement tag=01FJ}

a) 図式 (18) では、すべての射はホモトピズムです。

b) $\omega \in$ Alt($\mathfrak{g}$) とします。次に、すべての $\xi \in \mathfrak{g}$ に対して $d\omega = 0$ と $d(i(\xi )\omega ) = 0$ の場合に限り、$\omega$ 属するを Alt($\mathfrak{g}$)$^G$ にします。複素数 Alt($\mathfrak{g}$)$^G$ の微分は零です。

c) 等級付けされたベクトル空間 $H(\Omega (G))$ は Alt($\mathfrak{g}$)$^G$ と同型です。

左変換によって G 上の G の作用に適用される (G 上の $G\times G$ の作用 $((g, h);x) \rightarrow gxh^{-1}$ に) 定理は、標準単射 $\Omega (G)^G\rightarrow \Omega (G)$ (または $^G\Omega (G)^G\rightarrow \Omega (G)$) がホモトプリズムであることを意味します。アルジェブルの観点から、Chap. X、p. 34、Cor.、主張 a) が続きます。

b)を証明します。第51章の提案による。 III, §3, no. 14 では、左右不変である G 上のすべての微分形 $\alpha$ に対して、$d\alpha =-d\alpha$、つまり $d\alpha = 0$ が得られます。従って、$\omega \in$ Alt($\mathfrak{g}$)$^G$ の場合、$d\omega = 0$、その結果、$d(i(\xi )\omega ) =$ $\theta (\xi )\omega -i(\xi )d\omega = 0$ となります。逆に、$d\omega = 0$と$d(i(\xi )d\omega ) = 0$の場合は、$\theta (\xi )\omega = 0$となります。

主張 c) は a) と b) から続きます。

#### 注意 {#lie-ix-s6-n5-rem-1 .statement tag=01FK}

$\Omega (G) ($Algèbre の部分複素数 $Z(\Omega (G))$ と $B(\Omega (G))$ を考えてみましょう。 X、p. 25）。 2 つの形の積の微分を与える公式 (微分可能および解析多様体、結果、8.3.5) から、$Z(\Omega (G))$ は $\Omega (G)$ の部分代数であり、$B(\Omega (G))$ は $Z(\Omega (G))$ の理想であることがわかります。その結果、外装積誘導するは、$H(\Omega (G))$ で代数構造と評価されました。前述の例では、採点結果代数 $H(\Omega (G))\rightarrow$ Alt($\mathfrak{g}$)$^G$ の同型が得られます。

H を G の閉じた部分群とします。 Thを適用します。 2から$X = G/H$まで。章著。 III, §1, no. 8、コル。提案 17 の 1、$G/H$ 上の G 不変微分形は、Alt(T$_e(G/H)$) の H 不変量元、つまり H 不変であり、すべての演算子 $i(\xi )$ によって消滅する Alt($\mathfrak{g}$) の元と識別できます。 $\xi \in L(H)$。その結果：

#### 系 2 {#lie-ix-s6-thm-2-cor-2 .statement tag=01FL}

H を G の閉じた部分群とします。

a) 標準単射 $\Omega (G/H)^G\rightarrow \Omega (G/H)$ はホモトピズムです。

b) 複合体 $\Omega (G/H)^G$ は、Alt($\mathfrak{g}$) からなるの元 $\omega$ Alt($\mathfrak{g}$) の部分複合体と識別でき、これらは H の随伴表現の下で不変であり、すべての $\xi \in L(H)$ に対して $i(\xi )\omega = 0$ となるようなものです。 加法で H が接続されている場合、この部分複合体は、すべての $\xi \in L(H)$ に対して $\theta (\xi )\omega = 0$ と $i(\xi )\omega = 0$ となるように、$\omega \in$ Alt($\mathfrak{g}$) で構成されます。

### 練習問題 {#lie-ix-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
