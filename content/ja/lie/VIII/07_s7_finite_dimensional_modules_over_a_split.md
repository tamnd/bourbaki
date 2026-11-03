---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 7
section_title: Finite dimensional modules over a split semi-simple Lie algebra
lang: ja
source: lie-vii-ix
book_pages: 124-140, 238-250
pdf_pages: 0132-0148, 0246-0258
extraction: native+ocr
subsections:
    - "no": 1
      title: WEIGHTS OF A FINITE DIMENSIONAL SIMPLE $\mathfrak{g}$-MODULE
      page: 124
      pdf_page: 132
    - "no": 2
      title: HIGHEST WEIGHT OF A FINITE DIMENSIONAL SIMPLE $\mathfrak{g}$-MODULE
      page: 126
      pdf_page: 134
    - "no": 3
      title: MINUSCULE WEIGHTS
      page: 130
      pdf_page: 138
    - "no": 4
      title: TENSOR PRODUCTS OF $\mathfrak{g}$-MODULES
      page: 132
      pdf_page: 140
    - "no": 5
      title: DUAL OF A $\mathfrak{g}$-MODULE
      page: 134
      pdf_page: 142
    - "no": 6
      title: REPRESENTATION RING
      page: 136
      pdf_page: 144
    - "no": 7
      title: CHARACTERS OF $\mathfrak{g}$-MODULES
      page: 139
      pdf_page: 147
statements: 46
exercises: 27
content_sha256: 4b866aff411b3633372bb88d05f916247d021d2f325b0270e5cc27595c9a6069
translated_from: content/en/lie/VIII/07_s7_finite_dimensional_modules_over_a_split.md
translation_method: google
source_content_sha256: ed5e53f6a5d3e5a763b2ce062b4bcc72122e2012ef339cee5d3bb3a328b965ff
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: fba54326f0c3094f7ec2783dc323cb92da796b0dbb0af3d9d7da52f9e91204fd
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 7。有限次元加群分裂半単純リー代数

この段落では、§6 の一般的な記法を保持します。 R の重みの P (または Q) 群 (R の根基重み) で表します。 B によって定義される順序関係に対して正である P (または Q) の要素の集合を $P_+$ (または $Q_+$) で表します。 We denote by $P_{++}$ the set of dominant weights of R relative to B (Chap. VI, §1, no. 10). すべての $\lambda (H_{\alpha}),\alpha \in B$ が整数 (それぞれ整数 $\geq 0$) である場合に限り、$\mathfrak{h}^*$ 属するの元 $\lambda$ を P (それぞれ $P_{++}$) にします。 We have $P_{++}\subset P_+$ (Chap. VI, §1, no. 6). $w\in W$ の場合、$w$ の $\varepsilon (w)$ 行列式で表され、1 または $-1$ に等しくなります。 $\rho =\frac{1}{2}\sum_{\alpha\in R_+}\alpha$を入れます。

### 1. 有限次元単純 $\mathfrak{g}$-モジュールの重み

#### 命題 1 {#lie-viii-s7-prop-1 .statement tag=0138}

V を有限次元 $\mathfrak{g}$ 加群とする。

(i) V 属するのすべての重みを P にします。

(ii) $V =\bigoplus_{\mu\in P}V^\mu$。

(iii) すべての $\mu\in \mathfrak{h}^*,V^\mu$ は、すべての $h\in \mathfrak{h}$ について $h.x=\mu(h)x$ となるように、$x\in V$ の集合です。

すべての $\alpha \in B$ に対して、$\mathfrak{s}\mathfrak{l}(2, k)$ から $\mathfrak{g}$ までの準同型が存在し、$H$ から $H_{\alpha}$ までかかります。従って、§1, no. 2までに、Cor.提案 $2, (H_{\alpha})_V$ は対角化可能であり、その固有値は整数です。従って、$\alpha \in B$ に対する $(H_{\alpha})_V$ の集合は対角化可能です (代数、Chap. VII, §5, no. 6、Prop. 13)。従って、すべての $h\in \mathfrak{h},h_V$ は対角化可能です。章著。 VII, §1, no. 3、提案$9, V =\bigoplus_{\mu\in\mathfrak{h}^*}V^\mu$。一方、$V^\mu\not= 0$ の場合、前述の式はすべての $\alpha \in B$ に対して $\mu(H_{\alpha})\in \mathbf{Z}$ であるため、$\mu\in P$ になります。これにより、(i) と (ii) が証明されます。同様に、$\mathfrak{h}_V$ は対角化可能であることがわかり、従って (iii) になります。

#### 系 {#lie-viii-s7-n1-cor-1 .statement tag=0139}

$\rho$ を、$\rho$ に関連付けられた $\mathfrak{g}$ および $\Phi$ 双線形形式の有限次元表現とします。

(i) $x, y\in \mathfrak{h}_{\mathbf{Q}}$ の場合、$\Phi (x, y)\in \mathbf{Q}$ と $\Phi (x, x)\in \mathbf{Q}_+$。

(ii) $\rho$ が単射である場合、$\Phi$ ～ $\mathfrak{h}$ の制限は非縮退です。

主張 (i) は、P の元が $\mathfrak{h}_{\mathbf{Q}}$ で有理値を持つため、提案 1 から導かれます。 If $\rho$ is injective, $\Phi$ is non-degenerate (Chap. I, §6, no. 1, Prop. 1), so the restriction of $\Phi$ to $\mathfrak{h}$ is non-degenerate (Chap. VII, §1, no. 3, Prop. 10 (iii)).

#### 補題 1 {#lie-viii-s7-lem-1 .statement tag=013A}

V を $\mathfrak{g}$ モジュール、$\rho$ 対応する表現を $\mathfrak{g}$ とします。

(i) $a$ が $\mathfrak{g}$ の冪零元であり、$\rho (a)$ が局所的に零能である場合、

$$
\rho (e^{ada}b) =e^{\rho(a)}\rho (b)e^{-\rho(a)}
$$

すべての$b\in \mathfrak{g}$に。

(ii) $\alpha \in R$ と、$\mathfrak{g}^{\alpha}$ の元および $\mathfrak{g}^{-\alpha}$ の $\rho$ の下の像が局所的に零である場合、V の重みの集合は反射 $s_{\alpha}$ の下で安定です。

(i) の仮定では、すべての $n\geq 0$ に対して $\rho$((ad $a$)$^nb$) $=$ (ad $\rho (a)$)$^n\rho (b)$ となるため、$\rho (e^{ada}b) =e^{ad\rho(a)}\rho (b)$ となります。一方、

$$
e^{ad\rho(a)}\rho (b) =e^{\rho(a)}\rho (b)e^{-\rho(a)}
$$

は、第 2 章の主張 (ii) です。 VII, §3, no. 1、補題 1.

(ii)では仮定を採用します。 $\theta_{\alpha}=e^{adX_{\alpha}}e^{adX_{-\alpha}}e^{adX_{\alpha}}$ にしましょう。 (i) により、すべての $b\in \mathfrak{g}$ に対して $\rho (\theta_{\alpha}b) = S\rho (b)S^{-1}$ となるような $S\in \mathbf{G}\mathbf{L}(V)$ が存在します。現在、$\theta_{\alpha}|\mathfrak{h}$ は $s_{\alpha}($§2, no. 2 の転置、補題 1) です。 $\lambda$をVの重みとします。すべての $h\in \mathfrak{h}$ に対して $\rho (h)x=\lambda (h)x$ となるような V の非ゼロ元 $x$ が存在します。それから

$$
\rho (h)S^{-1}x= S^{-1}\rho (^ts_{\alpha}h)x= S^{-1}\lambda (^ts_{\alpha}h)x= (s_{\alpha}\lambda )(h)S^{-1}x
$$

すべての$h\in \mathfrak{h}$のために。従って、$s_{\alpha}\lambda$はVの重みとなります。

#### 命題 2 {#lie-viii-s7-prop-2 .statement tag=013B}

V を有限次元 $\mathfrak{g}$ 加群とし、$s\in$ Aut$_0(\mathfrak{g})$ とします。

(i) すべての $x\in \mathfrak{g}$ に対して $(s(x))_V= Sx_VS^{-1}$ となるような $S\in \mathbf{G}\mathbf{L}(V)$ が存在します。

(ii) $s\in$ Aut$_e(\mathfrak{g})$ の場合、S は V のすべての $\mathfrak{g}$ サブモジュールを安定させたまま、$\mathbf{S}\mathbf{L}(V)$ の元になるように選択できます。

主張 (ii) は補題 1 (i) から続きます。ここで、$s\in$ Aut$_0(\mathfrak{g})$ とし、V によって定義される $\mathfrak{g}$ の $\rho$ 表現を表します。 (ii) により、表現 $\rho$ と $\rho \circ s$ はスカラーの後で拡大と等価になります。従って、それらは等価であり (章 I, §3, no. 8、提案 13)、従って S が存在します。

#### 注意 1 {#lie-viii-s7-n1-rem-1 .statement tag=013C}

提案 2 (i) の S 満たす条件を $\mathfrak{h}'=s(\mathfrak{h})$ とします。 $\mathfrak{h}^*$ から $\mathfrak{h}^{'*}$ までを $s^*$ 同型 $\lambda  \rightarrow \lambda \circ s^{-1}$ で示します。それは明らかです

$$
S(V^{\lambda}) = V^{s^*\lambda}
$$

特に:

#### 系 1 {#lie-viii-s7-prop-2-cor-1 .statement tag=013D}

同型 $s^*$ は、$\mathfrak{h}$ に対する V の重みを、$\mathfrak{h}'$ に対する V の重みとします。 対応する重みは同じ重複度を持っています。

#### 系 2 {#lie-viii-s7-prop-2-cor-2 .statement tag=013E}

$w\in W$ にしましょう。すべての $\lambda \in \mathfrak{h}^*$、ベクトル部分空間 $V^{\lambda}$、$V^{w\lambda}$ は同じ次元を持ちます。 Vの重みの集合はW下で安定しています。

確かに、$w$ は形 $s^*$ と $s\in$ Aut$_e(\mathfrak{g},\mathfrak{h}) ($§2, no. 2、Cor です。 Thの。 2)。

#### 注意 2 {#lie-viii-s7-n1-rem-2 .statement tag=01L8}

コル著提案 2 の 1 と §5, no. 3、注意 2 を考慮すると、$\mathfrak{g}$ の正規のカルタン部分代数とその多重性に関して、V の重みについて話すのは理にかなっています。

#### 注意 3 {#lie-viii-s7-n1-rem-3 .statement tag=013F}

補題 1 (i) と提案 2 は、$\mathfrak{g}$ が分割可能であると想定されていない場合でも、同じ証明とともに有効なままです。

### 2. 有限次元単純 $\mathfrak{g}$-モジュールの最高重量

#### 定理 1 {#lie-viii-s7-thm-1 .statement tag=013G}

単純な $\mathfrak{g}$ 加群は、最高重量所属から $P_{++}$ を持っている場合に限り、有限次元になります。

単純な $\mathfrak{g}$ モジュールを V で表し、重みの集合を $\mathscr{X}$ で表します。

a) V が有限次元であると仮定します。その場合、$\mathscr{X}$ は有限で空ではありません (提案 1)、極大元 $\omega$ も同様です。 $\alpha \in B$ にしましょう。次に、$\omega +\alpha  \notin \mathscr{X}$ ですが、これは、$\omega$ が V の最高重量 (§6, no. 2、補題 2) であることを証明します。一方、$\mathfrak{s}\mathfrak{l}(2, k)$から$\mathfrak{g}$までは$H$から$H_{\alpha}$までかかる準同型が存在します。 §1、提案 2 (i) より、$\omega (H_{\alpha})$ は整数 $\geq 0$ なので、$\omega \in P_{++}$ です。

b) V に最高重量 $\omega \in P_{++}$ があると仮定します。 $\alpha \in B$ と $e$ を V の重み $\omega$ のプリミティブ元とします。 $j\geq 0$に$e_j=X_{-\alpha}^je$を入れます、

$m=\omega (H_{\alpha})\in \mathbf{N}$、N = $\sum_{j=0}^mke_j$。 §1, no. 2 により、提案$1,X_{\alpha}e_{m+1}$ = 0。

$\beta \in B$ と $\beta \not=\alpha$ の場合、$[X_{\beta}, X_{-\alpha}] = 0$ なので、$X_{\beta}e_{m+1}=X_{\beta}X_{-\alpha}^{m+1}e$ = $X_{-\alpha}^{m+1}X_{\beta}e= 0$ となります。 $e_{m+1}\not= 0$ の場合、$e_{m+1}$ は原始的であることが結論するわかりますが、これは不合理です (§6、提案 3 (i))。だから$e_{m+1}= 0$。 したがって、§1, no. 2 によると、Cor.提案 1 の場合、N は $H_{\alpha}, X_{\alpha}$ と $X_{-\alpha}$ によって生成される部分代数 $\mathfrak{s}_{\alpha}$ の下で安定です。 Now $\mathfrak{s}_{\alpha}$ is reductive in $\mathfrak{g}$, so the sum of the finite dimensional subspaces of V that are stable under $\mathfrak{s}_{\alpha}$ is a $\mathfrak{g}$-submodule of V (Chap. I, §6, no. 6, Prop. 7); since this sum is non-zero, it is equal to V. このことから、$(X_{\alpha})_V$ と $(X_{-\alpha})_V$ は局所的に nilpotent であることがわかります。 補題 1 (ii) を考慮すると、$\mathscr{X}$ は $s_{\alpha}$ の下で安定しており、これはすべての $\alpha$ に当てはまります。 したがって、$\mathscr{X}$ は W の下で安定です。 Now every orbit of W on P meets $P_{++}$ (Chap. VI, §1, no. 10). 一方、$\lambda \in \mathscr{X}\cap P_{++}$ の場合、すべての $\alpha \in B$ に対して $n_{\alpha}\in \mathbf{N}$ と $n'_{\alpha}\geq 0$ を含む $\lambda =\omega -\sum_{\alpha\in B}n_{\alpha}\alpha =\sum_{\alpha\in B}n'_{\alpha}\alpha$

(第 V, §3, no. 5、補題 6)。 したがって、$\mathscr{X}\cap P_{++}$ は有限であり、したがって $\mathscr{X}$ も有限です。 それぞれの重みは有限の重複度 (§6, no. 1、提案 1 (ii)) を持つため、V は有限次元です。

#### 系 1 {#lie-viii-s7-thm-1-cor-1 .statement tag=013H}

$\lambda \in \mathfrak{h}^*$ と $\lambda  \notin P_{++}$ の場合、$\mathfrak{g}$ モジュール $E(\lambda ) ($§6, no. 3) は無限次元です。

#### 系 2 {#lie-viii-s7-thm-1-cor-2 .statement tag=013I}

$\lambda \in P_{++}$ の $\mathfrak{g}$ 加群 $E(\lambda )$ は、有限次元の単純な $\mathfrak{g}$ 加群の類の代表の集合を構成します。

$\lambda$ が基本重みである $\mathfrak{g}$ モジュール $E(\lambda )$ は、基本 $\mathfrak{g}$ モジュールと呼ばれます。 対応する表現は、$\mathfrak{g}$ の基本音表現と呼ばれます。それらは絶対に還元不可能です (§6, no. 2、提案 3 (iv))。

V が有限次元 $\mathfrak{g}$ 加群および $\lambda \in P_{++}$ である場合、型 $E(\lambda )$ の V の同型成分は最高重量の同型成分と呼ばれます。 V中$\lambda$。

#### 注意 1 {#lie-viii-s7-n2-rem-1 .statement tag=013J}

$E(\lambda ),s\in$ Aut($\mathfrak{g}$) の $\mathfrak{g}$ の $\lambda \in P_{++},\rho_{\lambda}$ 表現と、Aut(R$,B$) $($§5, no. 3 の $s$ の $\sigma$ 標準像とします。提案 5 の 1)。したがって、$\rho_{\lambda}\circ s$ は $\rho_{\sigma \lambda}$ と等価です。実際、$s\in$ Aut$_0(\mathfrak{g}),\rho_{\lambda}\circ s$ と $\rho_{\sigma \lambda}$ が $\rho_{\lambda}$ と同等である場合 (提案 2)。そして、$s$ が $\mathfrak{h}$ と B を安定させた場合、$\rho_{\lambda}\circ s$ は最高重量 $\sigma \lambda$ の単純なものです。

特に、基本的な表現は $s$ によって置換されており、この置換は、$s\in$ Aut$_0(\mathfrak{g})$ の場合にのみ恒等となります。

#### 命題 3 {#lie-viii-s7-prop-3 .statement tag=013K}

V を有限次元 $\mathfrak{g}$ 加群とし、$\mathscr{X}$ をその重みの集合とします。 $t\in \mathbf{Z}$ の $\lambda \in \mathscr{X},\alpha \in R$、I 集合を、I の $\lambda +t\alpha \in \mathscr{X},p$ (それぞれ $-q$) 最大の (それぞれ最小の) 元とする。 $m_t$を$\lambda +t\alpha$の重複度とします。

(i) I = $-q, p$ および $q-p=\lambda (H_{\alpha})$。

(ii) 整数 $u\in 0, p+q,\lambda + (p-u)\alpha$ および $\lambda + (-q+u)\alpha$ は、$s_{\alpha}$ および $m_{-q+u}=m_{p-u}$ の下では共役です。

(iii) $t\in \mathbf{Z}$ と $t <(p-q)/2$ の場合、$(X_{\alpha})_V$ 写像 $V^{\lambda+t\alpha}$ を$V^{\lambda+(t+1)\alpha}$ に単射的に代入します。

(iv) 写像 $t \rightarrow m_t$ は、$-q,(p-q)/2$ では増加する、$(p-q)/2, p$ では減少するです。

$\alpha \in B$ にしましょう。 V に、$\mathfrak{g}$ の元 $X_{\alpha}, X_{-\alpha}, H_{\alpha}$ で定義された $\mathfrak{s}\mathfrak{l}(2, k$) モジュール構造を与えます。 $V^{\lambda+p\alpha}$ のゼロ以外のすべての元はプリミティブになります。従って、$(\lambda +p\alpha )(H_{\alpha})\geq 0$ と $(X_{-\alpha})^rV^{\lambda+p\alpha}\not= 0$ は

$$
0\leq r\leq (\lambda +p\alpha )(H_{\alpha}) =\lambda (H_{\alpha}) + 2p
$$

(§1, no. 2、提案 2)。従って、$p\geq t\geq p-(\lambda (H_{\alpha}) + 2p)$ に対して $V^{\lambda+t\alpha}\not= 0$ となるため、$p+q\geq \lambda (H_{\alpha}) + 2p$ となります。 適用この結果を $-\alpha$ にすると、次のようになります。

$$
p+q\geq \lambda (H_{-\alpha}) + 2q=-\lambda (H_{\alpha}) + 2q
$$

従って、$p\geq t\geq  -q$ に対する $q-p=\lambda (H_{\alpha})$ と $\lambda +t\alpha \in \mathscr{X}$ は、(i) を証明します。

$\mu\in \mathfrak{h}^*$には$s_{\alpha}(\alpha ) =-\alpha$、$s_{\alpha}(\mu)\in \mu+k\alpha$がございます。 W は $\mathscr{X}$ を安定に残すため (提案 $2$ の Cor. 2) $,s_{\alpha}$ は $\{\lambda -q\alpha , \lambda -q\alpha +\alpha , . . . , \lambda +p\alpha \}$ を安定に残し、すべての $u\in k$ に対して $\lambda -q\alpha +u\alpha$ から $\lambda +p\alpha -u\alpha$ がかかります。 Corを使用する。提案 2 の 2 を再度実行すると、整数 $u\in 0, p+q$ ごとに $m_{-q+u}=m_{p-u}$ であることがわかります。これは(ii)を証明します。

§1、Cor.提案$2, (X_{\alpha})_V|V^{\lambda+t\alpha}$のは$t <(p-q)/2$の単射法です。現在$(X_{\alpha})_V$写像$V^{\lambda+t\alpha}$から$V^{\lambda+(t+1)\alpha}$です。従って、$t <(p-q)/2$ は $m_{t+1}\geq m_t$ となります。 $\alpha$ を $-\alpha$ に変更すると、$t >(p-q)/2$ が $m_{t+1}\leq m_t$ であることがわかります。これは (iii) と (iv) を証明します。

#### 系 1 {#lie-viii-s7-prop-3-cor-1 .statement tag=013L}

$\lambda \in \mathscr{X}$と$\lambda (H_{\alpha})\geq 1$の場合、$\lambda -\alpha \in \mathscr{X}$。 $\lambda +\alpha \in \mathscr{X}$ と $\lambda (H_{\alpha}) = 0$ の場合は、$\lambda \in \mathscr{X}$ と $\lambda -\alpha \in \mathscr{X}$ です。

これは提案 3 (i) の直後に続きます。

#### 系 2 {#lie-viii-s7-prop-3-cor-2 .statement tag=01J4}

$\mu\in P_{++}$と$\nu \in Q_+$としましょう。 $\mu+\nu \in \mathscr{X}$なら$\mu\in \mathscr{X}$。

$\alpha \in B$ をすべて $c_{\alpha}\in \mathbf{N}$ として、$\nu =\sum_{\alpha\in B}c_{\alpha}.\alpha$ と書きます。 系はクリアです

$\sum_{\alpha\in B}c_{\alpha}= 0$のとき; $\sum_{\alpha\in B}c_{\alpha}>0$と仮定して、$\sum_{\alpha\in B}c_{\alpha}$について帰納法によって議論します。 $(\cdot  | \cdot )$ を、$\mathfrak{h}^*_{\mathbf{R}}$ 上の W 不変非縮退正対称双線形形式とします。次に $(\nu |\sum_{\alpha\in B}c_{\alpha}.\alpha )>0$ なので、$c_{\beta}\geq 1$ となるような $\beta \in B$ が存在し、

$(\nu |\beta )>0$、従って $\nu (H_{\beta})\geq 1$。 $\mu\in P_{++}$ なので、$(\mu+\nu )(H_{\beta})\geq 1$ になります。コル著$1,\mu+ (\nu -\beta )\in \mathscr{X}$、帰納法の仮定を適用すれば十分です。

#### 系 3 {#lie-viii-s7-prop-3-cor-3 .statement tag=013M}

$v\in V$ を重み $\omega$ の原始関数とします。 $\Sigma$ を $\alpha \in B$ の集合として、$\omega (H_{\alpha}) = 0$ とします。線分$kv$の$\mathfrak{g}$の固定群は、$\Sigma ($§3, no. 4、注意に関連付けられた放物線部分代数$\mathfrak{p}_{\Sigma}$です）。

$v$ によって生成された $\mathfrak{g}$ サブモジュールによる置き換えること V は、必要に応じて、V が単純であると仮定できます。 $\mathfrak{s}$を固定群とします。 $(\mathfrak{n}_+)_Vv$ = 0、$(\mathfrak{h})_Vv\subset kv$ があります。 $\alpha \in B$ を $\omega (H_{\alpha}) = 0$ となるようにします。 $\omega +\alpha  \notin \mathscr{X}$ があるため、$\omega -\alpha  \notin \mathscr{X}$ (提案 3 (i))、その結果、$(\mathfrak{g}^{-\alpha})_Vv= 0$ になります。上記は $\mathfrak{p}_{\Sigma}\subset \mathfrak{s}$ であることを証明します。 $\mathfrak{p}_{\Sigma}\not=\mathfrak{s}$ の場合、$\mathfrak{s}=\mathfrak{p}_{\Sigma'}$、ここで、$\Sigma '$ は厳密には B の部分集合含む $\Sigma$ です。 $\beta \in \Sigma '$ **--** $\Sigma$ とします。次に、$\mathfrak{g}^{-\beta}$ は $kv$ を安定させ、従って $v$ を消滅させます。しかし、$\omega (H_{\beta})>0$以降、この矛盾する案3(iii)。 Q.E.D.

P の部分集合 $\mathscr{X}$ が次の条件を満たす場合、R 飽和と呼ばれます: すべての $\lambda \in \mathscr{X}$ とすべての $\alpha \in R$ について、0 から $\lambda (H_{\alpha})$ までのすべての整数 $t$ について $\lambda -t\alpha \in \mathscr{X}$ があります。 $s_{\alpha}(\lambda ) =\lambda -\lambda (H_{\alpha})\alpha$ 以降、R で飽和した P の部分集合は W の下で安定であることがわかります。 $\mathscr{Y}\subset P$ にしましょう。 $\mathscr{Y}$ の要素 $\lambda$ は、すべての $\alpha \in R$ について、$\lambda +\alpha  \notin \mathscr{Y}$ または $\lambda -\alpha  \notin \mathscr{Y}$ のいずれかである場合、$\mathscr{Y}$ では R 極値と呼ばれます。

#### 命題 4 {#lie-viii-s7-prop-4 .statement tag=013N}

V を有限次元 $\mathfrak{g}$ 加群とし、$d$ 整数 $\geq 1$ とします。 重みの集合 、 V 、 重複度 $\geq d$ は R 飽和です。

これは提案 3 の直後の結果です。

#### 命題 5 {#lie-viii-s7-prop-5 .statement tag=013O}

V を有限次元の単純な $\mathfrak{g}$ モジュール、$\omega$ をその最高重量、$\mathscr{X}$ を重みの集合とします。 選ぶは $\mathfrak{h}^*_{\mathbf{R}}$ 上の W 不変非縮退正対称双線形形式 $(\cdot |\cdot )$ であり、$\lambda  \rightarrow  \|\lambda \|= (\lambda |\lambda )^{1/2}$ は対応するノルムとします。

(i) $\mathscr{X}$ は P 含む $\omega$ の最小の R 飽和部分集合です。

(ii) $\mathscr{X}$ の R 極値元は、$\omega$ の W 変換です。

(iii) $\mu\in \mathscr{X}$ の場合、$\|\mu\| \leq  \|\omega \|$ になります。 加法、$\mu\not=\omega$ の場合、$\|\mu+\rho \|<\|\omega +\rho \|$ があります。 $\mathscr{X}$ で $\mu$ が R 極値でない場合は、$\|\mu\|<\|\omega \|$ です。

(iv) $\mathscr{X}= W.(\mathscr{X}\cap P_{++})$ があります。 $\omega -\lambda \in Q_+$ の場合に限り、$P_{++}$ 属するから $\mathscr{X}\cap P_{++}$ までの元 $\lambda$。

(i) $\mathscr{X}'$ を P 含む $\omega$ の R 飽和最小の部分集合とします。 $\mathscr{X}'\subset \mathscr{X}$ (提案 4) があります。 $\mathscr{X}\not=\mathscr{X}'$ と仮定します。 $\lambda$ を $\mathscr{X}$ **--** $\mathscr{X}'$ の極大元とします。 $\lambda \not=\omega$ 以降、$\lambda +\alpha \in \mathscr{X}$ となるような $\alpha \in B$ が存在します。 提案 3 のように $p$ と $q$ を導入します。 $\lambda$ は $\mathscr{X}$ **--** $\mathscr{X}',\lambda +p\alpha \in \mathscr{X}'$ で最大なので。 提案 3 (ii) より、$\mathscr{X}'$ は W の下で安定であるため、$\lambda -q\alpha \in \mathscr{X}'$ となります。 したがって、区間 $-q, p$ のすべての整数 $u$ は $\lambda +u\alpha \in \mathscr{X}'$ となります。 これは矛盾する $\lambda  \notin \mathscr{X}'$ であり、(i) が証明されます。

(ii) $\omega$ が $\mathscr{X}$ の R 極値元であることは明らかです。したがって、その W 変換は、$\mathscr{X}$ でも R 極値になります。 $\lambda$ を $\mathscr{X}$ の R 極値元とします。 $\lambda \in W.\omega$ を証明します。 $w\lambda \in P_{++}$(VI, §1, no. 10章)となるような$w\in W$が存在するので、$\lambda \in P_{++}$と仮定できます。 $\alpha \in B$ にしましょう。提案 3 のように $p$ と $q$ を導入します。$\lambda$ は R 極値なので、$p= 0$ または $q= 0$ のいずれかになります。以来

$$
q-p=\lambda (H_{\alpha})\geq 0
$$

私たちできないには$p >0$がいます。したがって、$p= 0$ と $\lambda =\omega$ です。

(iii) $\mu\in \mathscr{X}\cap P_{++}$ とします。次に、$\omega +\mu\in P_{++}$ と $\omega -\mu\in Q_+($§6, no. 1、提案 1)、つまり $0\leq (\omega -\mu|\omega +\mu) = (\omega |\omega )-(\mu|\mu)$;したがって、ワイル群を使用して、$(\mu|\mu)\leq (\omega |\omega )$、およびこの拡大するをすべての $\mu\in \mathscr{X}$ に変換します。 $\mu\in \mathscr{X}$ **--** $\{\omega \}$ の場合、

$$
(\mu+\rho |\mu+\rho ) = (\mu|\mu) + 2(\mu|\rho ) + (\rho |\rho )\leq (\omega |\omega ) + 2(\mu|\rho ) + (\rho |\rho )
$$

$$
= (\omega +\rho |\omega +\rho )-2(\omega -\mu|\rho )
$$

現在 $\omega -\mu=\sum_{\alpha\in B}n_{\alpha}\alpha$ と整数 $n_{\alpha}\geq 0$ はすべての零ではないので、すべての $\alpha \in B$ については $(\rho |\alpha )>0$ から $(\omega -\mu|\rho )>0$ となります（第 VI, §1, no. 10 案、提案 29 (iii)）。 $\mu$ が $\mathscr{X}$ で R 極値でない場合、$\mu+\alpha \in \mathscr{X}$ と $\mu-\alpha \in \mathscr{X}$ のような $\alpha \in R$ が存在します。それから

$\|\mu\|<$サップ($\|\mu+\alpha \|,\|\mu-\alpha \|$)$\leq$サップ$_{\lambda\in\mathscr{X}}\|\lambda \|$

そしてこの最後の上界は、その前の$\|\omega \|$ になります。

(iv) 第 4 章の$\mathscr{X}= W.(\mathscr{X}\cap P_{++})$ があります。 VI, §1, no. 10。 $\lambda \in \mathscr{X}$ の場合、$\omega -\lambda \in Q_+($§6, no. 1、提案 1)。 $\lambda \in P_{++}$ と $\omega -\lambda \in Q_+$ の場合、$\lambda \in \mathscr{X}$ (提案 3 の Cor. 2)。

#### 系 {#lie-viii-s7-n2-cor-1 .statement tag=013P}

$\mathscr{X}$ を P の有限 R 飽和部分集合とします。 重みの集合が $\mathscr{X}$ である有限次元 $\mathfrak{g}$ 加群が存在します。

$\mathscr{X}$ は $W,\mathscr{X}$ では安定なので、 最小の R-飽和集合含む $\mathscr{X}\cap P_{++}$ です。提案 5 (i) により、$\mathscr{X}$ は $\bigoplus_{\lambda\in\mathscr{X}\cap P_{++}}E(\lambda )$ の重みの集合です。

#### 注意 2 {#lie-viii-s7-n2-rem-2 .statement tag=013Q}

Recall (Chap. VI, §1, no. 6, Cor. 3 of Prop. 17) that there exists a unique element $w_0$ of W that transforms B into $-B$; we have $w_0^2= 1$. and $-w_0$ respects the order relation on P. With this in mind, let V be a finite dimensional simple $\mathfrak{g}$-module, $\omega$ its highest weight. すると、$w_0(\omega )$ は V の最低の重みであり、その重複度は 1 になります。

### 3. ミニスキュール重み

#### 命題 6 {#lie-viii-s7-prop-6 .statement tag=013R}

$\lambda \in P$ と $\mathscr{X}$ 最小のが P 含む $\lambda$ の R 飽和部分集合であるとします。 選ぶノルム $\| \cdot  \|$ は提案 5 と同様です。次の条件は同等です。

(i) $\mathscr{X}= W.\lambda$;

(ii) $\mathscr{X}$ のすべての元は同じノルムを持ちます。

(iii) すべての $\alpha \in R$ に対して、$\lambda (H_{\alpha})\in  \{0,1,-1\}$ があります。

P 含む元 $\lambda$ 満たすの空でないすべての R-飽和部分集合は上記条件です。

条件を紹介します:

(ii$'$) 0 から $\lambda (H_{\alpha})$ までのすべての $\alpha \in R$ およびすべての整数 $t$ について、

$$
\|\lambda -t\alpha \| \geq  \|\lambda \|
$$

(i) $=\Rightarrow$ (ii) $=\Rightarrow$ (ii$'$)$:$ これは明らかです。

(ii$'$) $=\Rightarrow$ (iii): 条件 (ii$'$) が満たされると仮定します。 $\alpha \in R$ にしましょう。 $\|\lambda \|=\|\lambda -\lambda (H_{\alpha})\alpha \|$ があるので、厳密に 0 から $\lambda (H_{\alpha})$ の間の整数 $t$ ごとに $\|\lambda -t\alpha \|<\|\lambda \|$ になります。したがって、そのような整数は存在しないため、$|\lambda (H_{\alpha})| \leq 1$ になります。

(iii) $=\Rightarrow$ (i): 条件 (iii) が満たされると仮定します。 $w\in W$ と $\alpha \in R$ としましょう。次に$(w\lambda )(H_{\alpha}) =\lambda (H_{w^{-1}\alpha})\in  \{0,1,-1\}$;したがって、$t$ が 0 と $(w\lambda )(H_{\alpha}),w\lambda -t\alpha$ の間の整数である場合、$w\lambda$ または $s_{\alpha}(w\lambda )$ に等しくなります。これは、$W.\lambda$ が R 飽和しているため、$\mathscr{X}= W.\lambda$ であることを証明します。

$\mathscr{Y}$ を P の空でない R 飽和部分集合とします。最小値ノルムの $\mathscr{Y}$ 元 $\lambda$ が存在します。 $\lambda$ が条件 (ii$'$) を満たすことは明らかであり、したがって命題の最後の主張になります。

#### 命題 7 {#lie-viii-s7-prop-7 .statement tag=013S}

V を有限次元の単純な $\mathfrak{g}$ 加群、V の重みの $\mathscr{X}$ 集合、および $\mathscr{X}$ の $\lambda$ 最高元とします (cf. 提案 5 (i))。 条件提案 6 の (i)、(ii)、(iii) は以下と同等です。

(iv) すべての $\alpha \in R$ とすべての $x\in \mathfrak{g}^{\alpha}$ に対して、$(x_V)^2= 0$ が得られます。

これらの条件が満たされる場合、V のすべての重みは重複度 1 を持ちます。

(i) が満たされる場合、$\mathscr{X}= W.\lambda$ と重みはすべて $\lambda$ と同じ重複度 (提案 2 の Cor. 2)、その他の語、重複度 1 を持ちます。さらに、$w\in W$ と $\alpha \in R,w\lambda +t\alpha$ できないがV 〜でない限り $|t| \leq 1$ の重み;したがって、$x\in \mathfrak{g}^{\alpha}$ の場合、

$$
(x_V)^2(V^{w(\lambda)})\subset V^{w(\lambda)+2\alpha}= 0
$$

したがって、$(x_V)^2= 0$、これは (i) $=\Rightarrow$ (iv) を証明します。

逆に、(iv)が満たされるとする。 $\alpha \in R$ とし、$\mathfrak{g}$ の元 $X_{\alpha}, X_{-\alpha}, H_{\alpha}$ によって定義される $\mathfrak{s}\mathfrak{l}(2, k)$ モジュール構造を V に与えます。 条件 (iv) は、$x=X_{\alpha}$ に適用され、$\mathfrak{s}\mathfrak{l}(2, k$) モジュール V 属するの重みが $\{0,1,-1\}$ に適用されることを意味します (cf. §1, no. 2、提案 2 の修正)。特に、$\lambda (H_{\alpha})\in  \{0,1,-1\}$ なので、(iv) $=\Rightarrow$ (iii) です。

#### 命題 8 {#lie-viii-s7-prop-8 .statement tag=013T}

$\mathfrak{g}$ が単純であると仮定します。 B の $\alpha_1, . . . , \alpha_l$ 元で表します。$\varpi_1, . . . , \varpi_l$ を対応する基本波重みとします。 $H$ = $n_1H_{\alpha_1}+\cdots +n_lH_{\alpha_l}$ を $R^{\vee}$ の最高根とし、$n_i= 1$ となるように $i\in  \{1, . . . , l\}$ の J 集合とします。 $\lambda \in P_{++}$ **--** $\{0\}$ とします。したがって、提案 6 の条件 (i)、(ii)、および (iii) は、以下の条件のそれぞれに相当します。

(v) $\lambda (H) = 1$;

(vi) $\lambda =\varpi_i$ となるような $i\in J$ が存在します。

$P(R)/Q(R)$ の非ゼロ元の P(R) の代表者の $i\in J$、形系の $\varpi_i$。

$\lambda =u_1\varpi_1+\cdots +u_l\varpi_l$ とします。ここで、$u_1, . . . , u_l$ は整数 $\geq 0$ であり、すべての零ではありません。次に、$\lambda (H) =u_1n_1+\cdots +u_ln_l$ と $n_1\geq 1, . . . , n_l\geq 1$ により、(v) と (vi) の同値が​​すぐに得られます。一方、$\lambda (H) =$ sup$_{\alpha\in R_+}\lambda (H_{\alpha})$、および$\lambda (H)>0$ は、$\lambda$ が$P_{++}$ の非ゼロ元であるためです。したがって、

条件 (v) は、提案 6 のその他の語 ～ 条件 (iii) では、すべての $\alpha \in R$ について条件 $\lambda (H_{\alpha})\in  \{0,1\}$ に相当します。

命題の最後の主張は第2章から続きます。 VI, §2, no. 3、コル。提案6の。

#### 定義 1 {#lie-viii-s7-def-1 .statement tag=013U}

$\mathfrak{g}$ が単純であると仮定します。 $(\mathfrak{g},\mathfrak{h})$ のミニスキュール重みは、$P_{++}$ **--** $\{0\}$ の元であり、提案 6、7、および 8 の同等の条件 (i)、(ii)、(iii)、(iv)、(v)、および (vi) を満たします。

#### 注意 {#lie-viii-s7-n3-rem-1 .statement tag=013V}

$\mathfrak{g}$ が単純であると仮定します。 $\Sigma^{'\vee}$ をアフィン ワイル群 $W_a(R^{\vee})$ の Coxeter グラフとします。 $\Sigma^{'\vee}$ の頂点は、$W(R^{\vee})$ の Coxeter グラフ $\Sigma^{\vee}$ の頂点に補助頂点 0 を加えたものであることを思い出してください。 群 $A(R^{\vee})$ は 0 を固定したまま、$\Sigma^{'\vee}$ で演算します。 群 Aut($\Sigma^{'\vee}$) は、群 $\Gamma_C$ (cf. Chap. VI, §2, no. 3 および Chap. VI, §4, no. 3) を含む $A(R^{\vee})/W(R^{\vee})$ の半直接積と正準的に同型です。明らかに (Aut $\Sigma^{'\vee}$)$(0) =\Gamma_C(0)$;そして$\Gamma_C(0)$は0と、$i\in J$の$\Sigma^{\vee}$対応するから$\varpi_i$までの頂点で構成されます（cf.Chap.VI, §2、Prop.5と注意no. 3の1）。要約すると、ミニスキュール重みは、Aut($\Sigma^{'\vee}$) の元の演算によって 0 から得られる、$\Sigma^{\vee}$ の頂点に対する基本的な重み対応するです。

第3章の記法とVI、プレート I から IX まで、前述のことから、ミニスキュール重みは次のように推測されます。

型 $A_l(l\geq 1):\varpi_1, . . . , \varpi_l$ の場合。

型 $B_l(l\geq 2):\varpi_l$ の場合。

型 $C_l(l\geq 2):\varpi_1$ の場合。

型 $D_l(l\geq 3):\varpi_1, \varpi_{l-1}, \varpi_l$ の場合。

型 $E_6:\varpi_1, \varpi_6$ の場合。

型 $E_7:\varpi_7$ の場合。

型 $E_8,F_4,G_2$ にはミニスキュール重みはありません。

### 4. $\mathfrak{g}$ モジュールのテンソル積

$E,F$ を $\mathfrak{g}$ モジュールとします。 For all $\lambda , \mu\in \mathfrak{h}^*, E^{\lambda}\otimes F^\mu\subset (E\otimes F)^{\lambda+\mu}$ (Chap. VII, §1, no. 1, Prop. 2 (ii)). E と F が有限次元の場合、$E =\sum_{\lambda\in P}E^{\lambda}$

そして$F =\sum_{\mu\in P}F^\mu$;その結果、

$$
(E\otimes F)^{\nu}=\sum_{\lambda ,\mu\in P,\lambda+\mu=\nu}E^{\lambda}\otimes F^\mu
$$

他の語には、型$P, E\otimes F$の等級ベクトル空間EおよびFの等級テンソル積が装備されています。

#### 命題 9 {#lie-viii-s7-prop-9 .statement tag=013W}

$E,F$ をそれぞれ最高重量 $\lambda , \mu$ を持つ有限次元の単純な $\mathfrak{g}$ 加群とする。

(i) 最高重量 $\lambda +\mu$ の $E\otimes F$ の成分は、$(E\otimes F)^{\lambda+\mu}= E^{\lambda}\otimes F^\mu$ によって生成された単純部分加群です。

(ii) $E\otimes F$ の任意の単純部分加群の最高重量は $\leq \lambda +\mu$ (cf. §9、提案 2)。

$\alpha , \beta \in P$ と $E^{\alpha}\otimes F^{\beta}\not= 0$ の場合、$\alpha \leq \lambda$ と $\beta \leq \mu$。従って、$(E\otimes F)^{\lambda+\mu}$ は $E^{\lambda}\otimes F^\mu$ に等しいため、次元 1 となり、$\lambda +\mu$ は $E\otimes F$ の最高重量になります。 $E^{\lambda}\otimes F^\mu$ のゼロ以外のすべての元はプリミティブです。 §6, no. 2 の提案 4 により、最高重量 $\lambda +\mu$ の$E\otimes F$ の同型成分の長さは 1 です。

#### 注意 {#lie-viii-s7-n4-rem-1 .statement tag=013X}

提案 9 の記法を維持し、C を最高重量 $\lambda +\mu$ の $E\otimes F$ の同型成分とします。次に、C は E と F のみに依存し、$\mathfrak{h}$ の選択と基底 B には依存しません。他の語では、$\mathfrak{h}'$ を $\mathfrak{g}, R'$ の分裂カルタン部分代数 $(\mathfrak{g},\mathfrak{h}')$ の根系とします。そして $R'$ の $B'$ 基底; $\lambda ', \mu'$ を $\mathfrak{h}'$ と $B'$ に対する $E,F$ の最高重量とします。 $C'$ を最高重量 $\lambda '+\mu'$ の $E\otimes F$ の同型成分とします。それから$C'= C$。実際、これを証明するには、基礎体の拡大により、$k$ が代数的に閉じていると仮定できます。次に、$\mathfrak{h}$から$\mathfrak{h}', R$、$R', B$から$B'$までかかる$s\in$Aut$_e(\mathfrak{g})$が存在します。 $S\in \mathbf{S}\mathbf{L}(E\otimes F)$ に no. 1 の提案 2 のプロパティを持たせます。すると、$S((E\otimes F)^{\lambda+\mu}) = (E\otimes F)^{\lambda'+\mu'}$、S(C) = Cとなります。したがって、$(E\otimes F)^{\lambda'+\mu'}\subset C'\cap S(C) = C'\cap C$、したがって、$C'= C$。したがって、2 類の有限次元の単純な $\mathfrak{g}$ 加群に、正規に 3 番目の加群を関連付けることができます。他の語では、有限次元単純な $\mathfrak{g}$ 加群合成法則の類の集合 $\mathfrak{S}_{\mathfrak{g}}$ を定義しました。この構造により、$\mathfrak{S}_{\mathfrak{g}}$ は加法モノイド $P_{++}$ と正準的に同型になります。

#### 系 1 {#lie-viii-s7-prop-9-cor-1 .statement tag=01J5}

$(\varpi_{\alpha})_{\alpha\in B}$ を B に対する基本的な重みの族とします。$\lambda =\sum_{\alpha\in B}m_{\alpha}\varpi_{\alpha}\in P_{++}$ とします。すべての $\alpha \in B$ について、$E_{\alpha}$ を最高重量 $\varpi_{\alpha}$ の単純な $\mathfrak{g}$ モジュールとします。 $\mathfrak{g}$ モジュール $\bigotimes_{\alpha\in B}(\bigotimes^{m_{\alpha}}E_{\alpha})$ では、最高重量 $\lambda$ の同型成分は長さ 1 です。

これは、$\sum_{\alpha\in B}m_{\alpha}$の帰納法による提案9に続きます。

#### 系 2 {#lie-viii-s7-prop-9-cor-2 .statement tag=013Y}

$k$ が $\mathbf{R}$ または $\mathbf{C}$、または非離散完全ウルトラメトリック体であると仮定します。 G をリー群とリー代数 $\mathfrak{g}$ とします。 $\mathfrak{g}$ の基本的な表現 $\rho$ に対して、$\rho = L(\rho ')$ となるような G の解析線型表現 $\rho '$ が存在すると仮定します。次に、$\mathfrak{g}$ の有限次元線型表現 $\pi$ に対して、$\pi = L(\pi ')$ となるような G の解析的線型表現 $\pi '$ が存在します。

Corの記法を使用しています。 1. X の $\mathfrak{g}$ モジュール構造に対して $L(\sigma )$ 対応するとなるような、$X =\bigotimes_{\alpha\in B}(\bigotimes^{m_{\alpha}}E_{\alpha})$ 上の G の表現 $\sigma$ が存在します (提案 41 のIII, §3, no. 11 章、Cor. 3)。 C を最高重量 $\lambda$ の X の同型成分とします。章の観点から。 III, §3, no. 11、提案 40、C が $\sigma (G)$ の下で安定であることを証明すれば十分です。 $g\in G$ と $\varphi =$ を広告($g$) にします。次に、すべての $a\in \mathfrak{g}$ に対して $\sigma (g)a_X\sigma (g)^{-1}= (\varphi (a))_X$ です。一方、$\varphi$は$\mathfrak{g}$の自己同型で、$\mathfrak{h}$から$\mathfrak{h}', R$、$R'= R(\mathfrak{g},\mathfrak{h}'), B$から基底、$R'$の$B'$、そして$\varpi_{\alpha}$から最高重量がかかります。 $\mathfrak{h}'$ および $B'$ に対する $E_{\alpha}$ の $\varpi '_{\alpha}$ ($\varphi$ 変換 $E_{\alpha}$ が $E_{\alpha}$ と同型の $\mathfrak{g}$ 加群になるため)。したがって、$\varphi$ は $\lambda$ から $\sum m_{\alpha}\varpi '_{\alpha}$ になります。上記注意までに$\sigma (g)(C) = C$まで。

#### 命題 10 {#lie-viii-s7-prop-10 .statement tag=013Z}

$\lambda , \mu\in P_{++}$ にしましょう。 $E,F,G$ を最高重量 $\lambda , \mu, \lambda +\mu$ を含む単純な $\mathfrak{g}$ モジュールとします。 $\mathscr{X}$ (それぞれ $\mathscr{X}',\mathscr{X}''$) を E (それぞれ $F,G$) の重みの集合とします。次に$\mathscr{X}''=\mathscr{X}+\mathscr{X}'$。

$E =\bigoplus_{\nu\in P}E^{\nu},F =\bigoplus_{\sigma\in P}F^{\sigma}$ があるので、$E\otimes F$ は次の直接和です。

$$
(E\otimes F)^{\tau}=\sum_{\nu+\sigma=\tau}E^{\nu}\otimes F^{\sigma}
$$

提案 9 により、G は $E\otimes F$ の $\mathfrak{g}$ サブモジュールで識別できるため、$\mathscr{X}''\subset \mathscr{X}+\mathscr{X}'$ となります。 $G^{\tau}= G\cap (E\otimes F)^{\tau}$ があり、$\nu \in \mathscr{X}$ と $\sigma \in \mathscr{X}'$ について、$G\cap (E\otimes F)^{\nu+\sigma}\not= 0$ があることが示されれば十分です。 $(e_1, . . . , e_n)$ (それぞれ $(f_1, . . . , f_p)$) を E (それぞれ F) の基底元のからなるとし、それぞれ属するをいくつかの $E^{\nu}$ (それぞれ $F^{\sigma}$) とし、$e_1\in E^{\lambda}$ (それぞれ $f_1\in F^\mu$) とします。 $E\otimes F$ の $e_i\otimes f_j$ 形基底。 証明される結果が偽であると仮定します。 すると、G のすべての元の添字 $(i, j)$ の座標が零となるような対 $(i, j)$ が存在します。 U を、U の $U,c$ 余積の双対である $\mathfrak{g}, U'$ を包む代数とします。 すべての $u\in U$ について、$x_i(u)$ (それぞれ $y_j(u)$) を添字 $i$ (それぞれ $j$) の $u(e_1)$ (それぞれ $u(f_1)$) の座標とします。 $z_{ij}(u)$ を $u(e_1\otimes f_1)$ の添字 $(i, j)$ の座標とします。 次に$x_i, y_j, z_{ij}\in U'$。 ここで、$e_1$ 生成するは $\mathfrak{g}$ モジュール E なので、$x_i\not= 0$、同様に $y_j\not= 0$ になります。 By the definition of the $\mathfrak{g}$-module $E\otimes F$ (Chap. I, §3, no. 2), if $c(u) =\sum u_s\otimes u'_s$, we have

$$
z_{ij}(u) =\sum_sx_i(u_s).y_j(u'_s) =\langle c(u), x_i\otimes y_j\rangle
$$

他の語では、$z_{ij}$は$x_i$の積と、代数$U'$の$y_j$です。 しかし、この代数は整域（第II, §1, no. 5章、提案10）なので、$z_{ij}\not= 0$です。 すべての$u\in U$に対して$u(e_1\otimes f_1)\in G$なので、これは矛盾です。

### 5. $\mathfrak{g}$ モジュールのデュアル

$E,F$ を $\mathfrak{g}$ モジュールとします。 Recall (Chap. I, §3, no. 3) that Hom$_k(E,F)$ has a canonical $\mathfrak{g}$-module structure. $\varphi$ をホム$_k(E,F)$ の重み $\lambda$ の元とします。 If $\mu\in \mathfrak{h}^*$, then $\varphi (E^\mu)\subset F^{\lambda+\mu}$ (Chap. VII, §1, no. 1, Prop. 2 (ii)). したがって、E と F が有限次元である場合、Hom$_k(E,F)$ の重み $\lambda$ の元は、代数の意味で次数 $\lambda$ の等級付けされた準同型になります。 II, §11, no. 2、デフォルト。 4.

#### 命題 11 {#lie-viii-s7-prop-11 .statement tag=0140}

E を有限次元 $\mathfrak{g}$ 加群とし、$\mathfrak{g}$ 加群 $E^*=$ Hom$_k(E, k)$ を考えます。

(i) $-\lambda$ が E の重みであり、$E^*$ の $\lambda$ の重複度が E の $-\lambda$ と等しい場合に限り、元 $\lambda \in P$ は $E^*$ の重みです。

(ii) E が単純で最高重量 $\omega ,E^*$ が単純で最高重量 $-w_0(\omega )$ (cf. no. 2, 注意 2) がある場合。

$k$ を、元が重み 0 である自明な $\mathfrak{g}$ モジュールとして考えてみましょう。 上で述べたことにより、重み $\lambda$ の $E^*$ の元は、E から $k$ までの準同型であり、$\mu\not=-\lambda$ であれば $E^\mu$ に消えます。 これは(i)を証明します。 If E is simple, $E^*$ is simple (Chap. I, §3, no. 3), and the last assertion follows from Remark 2 of no. 2.

#### 注意 1 {#lie-viii-s7-n5-rem-1 .statement tag=0141}

$E,E^*$ を提案 11 のようにし、$\sigma \in$ Aut($\mathfrak{g},\mathfrak{h}$) を §5, no. 1 の記法の $\varepsilon (\sigma ) =-w_0$ とする (§5, no. 2、提案 2)。 $\rho , \rho '$ を $E,E^*$ に関連付けられた $\mathfrak{g}$ の表現とします。この場合、$\rho \circ \sigma$ は $\mathfrak{g}$ に最高重量 $-w_0(\omega )$ を加えた単純な表現であるため、$\rho \circ \sigma$ は $\rho '$ と等価です。

#### 注意 2 {#lie-viii-s7-n5-rem-2 .statement tag=0142}

$w_0=-1$ と仮定します。 次に、任意の有限次元 $\mathfrak{g}$ 加群 E について、E は $E^*$ と同型です。 Recall that, if $\mathfrak{g}$ is simple, $w_0=-1$ in the following cases: $\mathfrak{g}$ of type $A_1,B_l(l\geq 2), C_l(l\geq 2), D_l(l$ even $\geq 4), E_7,E_8,F_4,G_2$ (Chap. VI, Plates).

#### 補題 2 {#lie-viii-s7-lem-2 .statement tag=0143}

$h^0=\sum_{\alpha\in R_+}H_{\alpha}$ にしましょう。次に、$h^0=\sum_{\alpha\in B}a_{\alpha}H_{\alpha}$、$a_{\alpha}$ は整数 $\geq 1$ です。 $(b_{\alpha})_{\alpha\in B},(c_{\alpha})_{\alpha\in B}$ を、すべての $\alpha \in B$ に対して $b_{\alpha}c_{\alpha}=a_{\alpha}$ となるようなスカラーの族とする。 $x=\sum_{\alpha\in B}b_{\alpha}X_{\alpha}, y=\sum_{\alpha\in B}c_{\alpha}X_{-\alpha}$を入れます。 準同型 $\varphi$ が存在します

$\mathfrak{s}\mathfrak{l}(2, k)$ から $\mathfrak{g}$ まで、$\varphi (H) =h^0, \varphi (X_+) =x, \varphi (X_-) =y$ になります。

The fact that the $a_{\alpha}$ are integers $\geq 1$ follows from the fact that $(H_{\alpha})_{\alpha\in B}$ is a basis of the root system $(H_{\alpha})_{\alpha\in B}$ (cf. Chap. VI, §1, no. 5, Remark 5). 我々は持っています：

$$
\alpha (h^0) = 2 \tag{1}
$$

for all $\alpha \in B$ (Chap. VI, §1, no. 10, Cor. of Prop. 29), so

$$
[h^0, x] =\sum_{\alpha\in B}b_{\alpha}\alpha (h^0)X_{\alpha}= 2x \tag{2}
$$

$$
[h^0, y] =\sum_{\alpha\in B}c_{\alpha}(-\alpha (h^0))X_{-\alpha}=-2y \tag{3}
$$

一方で、

$$
[x, y] =\sum_{\alpha ,\beta\in B}b_{\alpha}c_{\beta}[X_{\alpha}, X_{-\beta}] =\sum_{\alpha\in B}b_{\alpha}c_{\alpha}[X_{\alpha}, X_{-\alpha}] =-\sum_{\alpha\in B}a_{\alpha}H_{\alpha}=-h^0 \tag{4}
$$

従って、準同型 $\varphi$ が存在します。

#### 命題 12 {#lie-viii-s7-prop-12 .statement tag=0144}

E を有限次元の単純な $\mathfrak{g}$ 加群、$\omega$ その最高重量、および E 上の $\mathfrak{g}$ 不変双線形形式の $\mathscr{B}$ ベクトル空間とします。$m$ を整数 $\sum_{\alpha\in R_+}\omega (H_{\alpha})$ とすると、$m/2$は、B に関する $\omega$ の座標の和です (提案 29 のVI, §1, no. 10 章)。 $w_0$ を W の元とし、$w_0(B) =-B$ とします。

(i) $w_0(\omega )\not=-\omega$ の場合は、$\mathscr{B}= 0$。

(ii) $w_0(\omega ) =-\omega$ と仮定します。この場合、$\mathscr{B}$ は次元 1 であり、$\mathscr{B}$ のゼロ以外のすべての元は非縮退です。 $m$ が偶数 (または奇数) の場合、$\mathscr{B}$ のすべての元は対称です (それぞれ交代的)。

a) $\Phi \in \mathscr{B}$ とします。 E から $E^*$ までの写像 $\varphi$ は、$x, y\in E$ に対して、$\varphi (x)(y) =$ $\Phi (x, y)$ によって定義され、$\mathfrak{g}$ モジュールの準同型です。 $\Phi \not= 0$ の場合、$\varphi \not= 0$ なので、$\varphi$ はシュールの補題により同型となり、従って $\Phi$ は非縮退です。従って、$\mathfrak{g}$ モジュール E は $\mathfrak{g}$ モジュール $E^*$ と同型であるため、$w_0(\omega ) =-\omega$ になります。従って、(i) が証明されました。

b) これから$w_0(\omega)=-\omega$と仮定します。このとき、E は $E^*$ と同型です。 ベクトル空間 $\mathscr B$ は $\operatorname{Hom}_{\mathfrak g}(E,E^*)$ と同型であり、したがって次元 1 の $\operatorname{Hom}_{\mathfrak g}(E,E)$ と同型です (§6, no. 1、提案 1 (iii))。従って$\dim \mathscr B=1$です。 $\mathscr B$ のゼロ以外のすべての元 $\Phi$ は、a) によって非縮退です。 $x,y\in E$に$\Phi_1(x,y)=\Phi(y,x)$を入れます。上記により、すべての $x,y\in E$ に対して $\Phi_1(x,y)=\lambda\Phi(x,y)$ となるような $\lambda\in k$ が存在します。次に$\Phi(y,x)=\lambda\Phi(x,y)=\lambda^2\Phi(y,x)$、つまり$\lambda^2=1$と$\lambda=\pm1$です。従って、$\Phi$ は対称または交代的のいずれかです。

c) 第 2 章による。 VII, §1, no. 3、提案 9 (v)、$E^\lambda$ および $E^\mu$ は、$\lambda+\mu\ne0$ の場合、$\Phi$ に関して直交します。 $\Phi$ は非縮退であるため、$E^\omega,E^{-\omega}$ は $\Phi$ に関して直交しないことになります。

d) $\mathfrak{sl}(2,k)$ から $\mathfrak g$ の部分代数まで、$H$ を要する準同型 $\varphi$ が存在します。
$$
\sum_{\alpha\in R_+}H_\alpha
$$
(補題2)。この準同型を介して E を $\mathfrak{sl}(2,k)$ モジュールとして考えます。すると、$E^\lambda$の元は重み$\lambda\left(\sum_{\alpha\in R_+}H_\alpha\right)$になります。 $\lambda\in P$ が $E^\lambda\ne0$ と $\lambda\ne\omega,\lambda\ne-\omega$ である場合、$-\omega<\lambda<\omega$ となるので、
$$
-m=-\omega\left(\sum_{\alpha\in R_+}H_\alpha\right)<\lambda\left(\sum_{\alpha\in R_+}H_\alpha\right)<\omega\left(\sum_{\alpha\in R_+}H_\alpha\right)=m.
$$
G を $\mathfrak{sl}(2,k)$ 加群 E の型 V$(m)$ の同型成分とします。上記により、G は長さ 1 および含む $E^\omega,E^{-\omega}$ になります。 c)により、Gに対する$\Phi$の制限は非ゼロになります。 §1, no. 3, 注意 3 により、この制限は対称または交代的に従って、$\pi$ は偶数または奇数になります。 b)を考慮すると、これで証明が完了します。

#### 定義 2 {#lie-viii-s7-def-2 .statement tag=01J6}

$\mathfrak g$ の有限次元既約表現 $\rho$ は、E 上に $\rho$ のもとで不変の非縮退対称 (それぞれ交代的) 双線形形式が存在する場合、直交 (それぞれシンプレクティック) であると言われます。

### 6. 表現環

$\mathfrak a$ を有限次元リー代数とします。 $\mathscr F_{\mathfrak a}$ (それぞれ $\mathscr G_{\mathfrak a}$) を、有限次元 (それぞれ有限次元単純) $\mathfrak a$ モジュールの類の集合とします。 $\mathscr R(\mathfrak a)$ を自由なアーベル群 $\mathbf Z^{(\mathscr G_{\mathfrak a})}$ とします。任意の有限次元の単純な $\mathfrak a$ 加群 E について、その類を $[E]$ で表します。 F を有限次元 $\mathfrak a$ 加群とする。させてください
$$
(F_n,F_{n-1},\ldots,F_0)
$$
F のジョーダン ヘルダー 系列になる。 元
$$
\sum_{i=1}^{n}[F_i/F_{i-1}]
$$
$\mathscr R(\mathfrak a)$ は F のみに依存し、ヨルダン ヘルダー 系列の選択には依存しません。それを$[F]$で表します。もし
$$
0\longrightarrow F'\longrightarrow F\longrightarrow F''\longrightarrow0
$$
は有限次元 $\mathfrak a$ 加群の完全系列であり、次に $[F]=[F']+[F'']$ です。

F を有限次元半単純 $\mathfrak{a}$ 加群とする。すべての $E\in \mathfrak{S}_{\mathfrak{a}}$ について、$n_E$ を型 E の F の同型成分の長さとします。その場合、[F] = $\sum_{E\in\mathfrak{S}_{\mathfrak{a}}}n_E.E$ となります。 $F,F'$ が有限次元半単純 $\mathfrak{a}$ 加群で、[F] = $[F']$ の場合、F と $F'$ は同型です。

#### 補題 3 {#lie-viii-s7-lem-3 .statement tag=0145}

G を加法的に書くとアーベル群、そして $\varphi :\mathscr{F}_{\mathfrak{a}}\rightarrow G$ 写像とします。 記法の乱用により、任意の有限次元 $\mathfrak{a}$ 加群 F の類の $\varphi$ の下の $\varphi (F)$ 像で表します。 任意の完全系列について、次のように仮定します。

$$
0\longrightarrow F'\longrightarrow F\longrightarrow F''\longrightarrow 0
$$

有限次元 $\mathfrak{a}$ 加群の場合、$\varphi (F) =\varphi (F') +\varphi (F'')$ があります。すると、すべての有限次元 $\mathfrak{a}$ 加群 F に対して $\theta ([F]) =\varphi (F)$ となる一意な準同型 $\theta :\mathscr{R}(\mathfrak{a})\rightarrow G$ が存在します。

$\mathscr{R}(\mathfrak{a})$ から G までの一意な準同型 $\theta$ が存在し、すべての有限次元単純 $\mathfrak{a}$ 加群 E に対して $\theta ([E]) =\varphi (E)$ が成り立ちます。F を有限次元 $\mathfrak{a}$ 加群、$(F_n,F_{n-1}, . . . ,F_0)$ を F のジョーダン・ヘルダー 系列とします。 $n >0$ の場合、$n$ の帰納法までに、

$$
\theta ([F]) =\sum_{i=1}^n\theta ([F_i/F_{i-1}]) =\sum_{i=1}^n\varphi (F_i/F_{i-1}) =\varphi (F)
$$

$n= 0$ の場合、[F] = 0 なので $\theta ([F]) = 0$;一方、完全系列 $0\longrightarrow 0\longrightarrow 0\longrightarrow 0\longrightarrow 0$ を考慮すると、$\varphi (0) = 0$ であることがわかります。

#### 例 {#lie-viii-s7-n6-exa-1 .statement tag=0146}

$G =\mathbf{Z}$ と $\varphi (F) =$ を dim F に取ります。 $\mathscr{R}(\mathfrak{a})$ から $\mathbf{Z}$ までの対応する準同型は dim で表されます。 $c$ を次元 1 の自明な $\mathfrak{a}$ 加群の類とし、$\psi$ を $\mathbf{Z}$ から $\mathscr{R}(\mathfrak{a})$ までの準同型 $n \rightarrow nc$ とします。それは明らかです

薄暗い$\circ \psi =$ ID$_{\mathbf{Z}}$,

したがって、$\mathscr{R}(\mathfrak{a})$はカーディムの直和と$\mathbf{Z}c$になります。

#### 補題 4 {#lie-viii-s7-lem-4 .statement tag=0147}

加法群 $\mathscr{R}(\mathfrak{a})$ には、すべての有限次元 $\mathfrak{a}$ 加群 E、F に対して $[E][F] = [E\otimes F]$ となるような、加法にわたる一意の乗法分布が存在します。このようにして、$\mathscr{R}(\mathfrak{a})$ には可換環の構造が与えられます。 次元 1 の自明な $\mathfrak{a}$ モジュールの類は、この環の単位元です。

一意性はクリアです。 $\mathscr{R}(\mathfrak{a}) =\mathbf{Z}^{(\mathfrak{S}_{\mathfrak{a}})}$ には可換乗法が存在し、それは加法上で分配的であり、すべての $E,F\in \mathfrak{S}_{\mathfrak{a}}$ に対して $[E][F] = [E\otimes F]$ となるようなものです。 $E_1,E_2$ を有限次元の $\mathfrak{a}$ モジュール、$l_1$ と $l_2$ をそれらの長さとします。 $l_1+l_2$ の帰納法によって $[E_1][E_2] = [E_1\otimes E_2]$ であることがわかります。 $l_1+l_2\leq 2$であればこれは明らかです。一方、$F_1$ を 0 と $E_1$ から区別する $E_1$ の部分加群とします。それから

帰納法の仮定による$[F_1][E_2] = [F_1\otimes E_2]$と$[E_1/F_1][E_2] = [(E_1/F_1)\otimes E_2]$。一方、$(E_1\otimes E_2)/(F_1\otimes E_2)$ は $(E_1/F_1)\otimes E_2$ と同型です。したがって、

$$
[E_1][E_2] = ([E_1/F_1] + [F_1]).[E_2] = [(E_1/F_1)\otimes E_2] + [F_1\otimes E_2] = [E_1\otimes E_2]
$$

それは私たちの主張を証明します。上記で定義された乗法は結合的であるため、$\mathscr{R}(\mathfrak{a})$ は可換環の構造を持ちます。最後に、次元 1 の自明な $\mathfrak{a}$ 加群の類がこの環の単位元であることは明らかです。

#### 補題 5 {#lie-viii-s7-lem-5 .statement tag=0148}

すべての有限次元 $\mathfrak{a}$ 加群 E に対して $[E]^*= [E^*]$ となるような、環 $\mathscr{R}(\mathfrak{a})$ の固有の包含自己同型 $X \rightarrow X^*$ が存在します。

一意性はクリアです。 補題 3 までに、加法群 $\mathscr{R}(\mathfrak{a})$ からそれ自体までの準同型 $X \rightarrow X^*$ が、有限次元の$\mathfrak{a}$ 加群 E ごとに $[E]^*= [E^*]$ となるように存在します。$(X^*)^*= X$ があるので、この準同型は含積的です。 $(E\otimes F)^*$ はすべての有限次元 $\mathfrak{a}$ 加群 E および F について $E^*\otimes F^*$ と同型なので、環 $\mathscr{R}(\mathfrak{a})$ の自己同型です。

$U(\mathfrak{a})$ を $\mathfrak{a}, U(\mathfrak{a})^*$ ベクトル空間の$U(\mathfrak{a})$ の双対を包む代数とします。 Recall (Chap. II, §1, no. 5) that the coalgebra structure of $U(\mathfrak{a})$ defines on $U(\mathfrak{a})^*$ a commutative, associative algebra structure with unit element. 任意の有限次元 $\mathfrak{a}$ 加群 E の場合、$U(\mathfrak{a})$ から $k$ までの写像 $u \rightarrow$ Tr($u_E$) は、$U(\mathfrak{a})^*$ の元 $\tau_E$ です。 $0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0$ が有限次元 $\mathfrak{a}$ 加群の完全系列である場合、$\tau_E=\tau_{E'}+\tau_{E''}$ です。 従って、補題 3 によって、加法群 $\mathscr{R}(\mathfrak{a})$ から群 $U(\mathfrak{a})^*$ までの一意な準同型が存在し、すべての有限次元 $\mathfrak{a}$ 加群 E に対して Tr[E] $=\tau_E$ となります。 $k$ が次元 1 の自明な $\mathfrak{a}$ 加群を表す場合、Tr[$k]$ が $U(\mathfrak{a})^*$ の単位元であることを確認するのは簡単です。 最後に、E と F を有限次元 $\mathfrak{a}$ 加群とする。 $u\in U(\mathfrak{a})$ と $c$ を $U(\mathfrak{a})$ の余積とします。 By definition of the U-module $E\otimes F$ (Chap. I, §3, no. 2), if $c(u) =\sum_iu_i\otimes u'_i$,

$$
u_{E\otimes F}=\sum_i(u_i)_E\otimes (u'_i)_F
$$

その結果

$\tau_{E\otimes F}(u) =\sum_i$ トリ($u_i$)$_E$ トリ($u'_i$)$_F=\sum_i\tau_E(u_i)\tau_F(u'_i)$

$$
= (\tau_E\otimes \tau_F)(c(u))
$$

これは、$\tau_E\tau_F=\tau_{E\otimes F}$ を意味します。従って、Tr$:\mathscr{R}(\mathfrak{a})\rightarrow U(\mathfrak{a})^*$は環の準同型です。

$\mathfrak{a}_1$と$\mathfrak{a}_2$を$\mathfrak{a}_1$から$\mathfrak{a}_2$までのリー代数、$f$準同型とします。すべての有限次元 $\mathfrak{a}_2$ 加群 E 定義するは、$f$ による $\mathfrak{a}_1$ 加群、したがって、$\mathscr{R}(\mathfrak{a}_2)$ と $\mathscr{R}(\mathfrak{a}_1)$ の元を暫定的に $[E]_2$ と $[E]_1$ で表します。 補題 3 により、群 $\mathscr{R}(\mathfrak{a}_2)$ から群 $\mathscr{R}(\mathfrak{a}_1)$ まで、$\mathscr{R}(f)$ で示される一意な準同型が存在し、有限次元 $\mathfrak{a}_2$ 加群 E ごとに $\mathscr{R}(f)[E]_2=[E]_1$ となります。 $\mathscr{R}(f)$は環の準同型です。 U(f) が U($\mathfrak{a}_1$) から U($\mathfrak{a}_2$) まで $f$ 延長された準同型である場合、次の図式は可換です

$$
\begin{array}{ccc}
\mathscr{R}(\mathfrak{a}_2) & \xrightarrow{\mathscr{R}(f)} & \mathscr{R}(\mathfrak{a}_1)\\
\Big\downarrow\scriptstyle{\operatorname{Tr}} & & \Big\downarrow\scriptstyle{\operatorname{Tr}}\\
U(\mathfrak{a}_2)^* & \xrightarrow{t_{U(f)}} & U(\mathfrak{a}_1)^*.
\end{array}
$$

以下では、分割可能な半単純リー代数 $\mathfrak{g}$ を $\mathfrak{a}$ として取り上げます。 環 $\mathscr{R}(\mathfrak{g})$ は、$\mathfrak{g}$ の *表現環* と呼ばれます。すべての $\lambda\in P_{++}$ について、最高重量 $\lambda$ の単純な $\mathfrak{g}$ モジュール E($\lambda$) の $[\lambda]$ 類で表します。

### 7. $\mathfrak{g}$ モジュールの指標

$\Delta$ を加法的に書かれた可換モノイドとし、$\mathbf{Z}$ 上のモノイド $\Delta$ の $\mathbf{Z}[\Delta]=\mathbf{Z}^{(\Delta)}$ 代数とします (代数、III, §2, no. 6 章)。 $\mathbf{Z}[\Delta]$ の $(e^\lambda)_{\lambda\in\Delta}$ 標準基底で表します。すべての$\lambda,\mu\in\Delta$に対して、$e^{\lambda+\mu}=e^\lambda e^\mu$があります。 0 が $\Delta$ の中立値元である場合、$e^0$ は $\mathbf{Z}[\Delta]$ の単位元です。それは 1 で示されます。

E を体 $\kappa$ を超える $\Delta$ で評価されたベクトル空間とし、$(E^\lambda)_{\lambda\in\Delta}$ をその卒業度とします。それぞれの $E^\lambda$ が有限次元である場合、ch(E) で示される E の *指標* は、$\mathbf{Z}^{\Delta}$ の元 $(\dim E^\lambda)_{\lambda\in\Delta}$ です。 E 自体が有限次元である場合、

$$
\operatorname{ch}(E)=\sum_{\lambda\in\Delta}(\dim E^\lambda)e^\lambda\in\mathbf{Z}[\Delta].
\tag{5}
$$

E′、E、E'' を $\Delta$ 等級付けベクトル空間とし、E′${}^\lambda$、E${}^\lambda$、E''${}^\lambda$ が次数 0 の等級付け準同型の $\kappa$ および $0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow0$ 完全系列で有限次元となるようにします。 明らかそれ

$$
\operatorname{ch}(E)=\operatorname{ch}(E')+\operatorname{ch}(E'').
\tag{6}
$$

特に、F$_1$、F$_2$ が $\Delta$ 段階化ベクトル空間で、F$_1^\lambda$ と F$_2^\lambda$ が $\kappa$ にわたって有限次元である場合、

$$
\operatorname{ch}(F_1\oplus F_2)=\operatorname{ch}(F_1)+\operatorname{ch}(F_2).
\tag{7}
$$

F$_1$ と F$_2$ が有限次元であれば、次のようになります。

$$
\operatorname{ch}(F_1\otimes F_2)=\operatorname{ch}(F_1)\mathbin{.}\operatorname{ch}(F_2).
\tag{8}
$$

#### 例 {#lie-viii-s7-n7-exa-1 .statement tag=01JX}

$\Delta=\mathbf{N}$ と仮定します。 T を不定数とします。すべての $n\in\mathbf{N}$ に対して $e^n$ から $T^n$ を要する代数 $\mathbf{Z}[\mathbf{N}]$ から代数 $\mathbf{Z}[T]$ までの一意の同型が存在します。任意の有限次元 $\mathbf{N}$ 級数ベクトル空間 E の場合、$\mathbf{Z}[T]$ の ch(E) の像は E のポアンカレ多項式です (第 V, §5, no. 1 章)。

E を、$E =\sum_{\lambda\in\mathfrak{h}^*}E^{\lambda}$ が成り、各 $E^{\lambda}$ が次のようになるような $\mathfrak{g}$ モジュールとする

有限次元。 $(E^{\lambda})_{\lambda\in\mathfrak{h}^*}$ はベクトル空間 E の卒業であることがわかっています。以下では、$\mathfrak{h}^*$ で評価されたベクトル空間とみなされる E の指標に対して記法 ch(E) を予約します。したがって、指標 ch(E) は $\mathbf{Z}^{\mathfrak{h}^*}$ の元です。 E が有限次元の場合、ch(E) $\in \mathbf{Z}[P]$。 no. 6 の公式 (6) と補題 3 により、任意の有限次元 $\mathfrak{g}$ 加群 E に対して、E を ch(E) とする群 $\mathscr{R}(\mathfrak{g})$ から $\mathbf{Z}[P]$ までの一意な準同型が存在します。この準同型は ch で示されます。 関係 (8) は、ch が環 $\mathscr{R}(\mathfrak{g})$ から環 $\mathbf{Z}[P]$ までの準同型であることを示します。

#### 注意 {#lie-viii-s7-n7-rem-1 .statement tag=0149}

P 定義するのすべての元は、次元 1 の単純な $\mathfrak{h}$ モジュールであるため、群 $\mathbf{Z}[P]$ から群 $\mathscr{R}(\mathfrak{h})$ までの準同型、つまり単射準同型環。合成したのは明らかです

$$
\mathscr{R}(\mathfrak{g})\longrightarrow \mathbf{Z}[P]\longrightarrow \mathscr{R}(\mathfrak{h})
$$

準同型は、$\mathfrak{h}$ の標準単射によって $\mathfrak{g}$ (no. 6) に定義されます。

ワイル群 W は群 P の自己同型によって動作するため、$\mathbf{Z}^P$ に動作します。すべての $\lambda \in P$ とすべての $w\in W$ に対して、$we^{\lambda}=e^{w\lambda}$ があります。 $\mathbf{Z}[P]^W$ を W の下で不変である $\mathbf{Z}[P]$ のからなると元の部分環とする。

#### 補題 6 {#lie-viii-s7-lem-6 .statement tag=014A}

$\lambda \in P_{++}$ の場合、ch[$\lambda ]\in \mathbf{Z}[P]^W$. ch[$\lambda ]$ (章 VI, §3, no. 2、定義 1) の一意の最大値項は $e^{\lambda}$ です。

最初の主張は、Cor. の no. 1 から続きます。提案 2 の 2、および§6, no. 1 の 2 つ目、提案 1 (ii)。

#### 定理 2 {#lie-viii-s7-thm-2 .statement tag=014B}

(i) $(\varpi_{\alpha})_{\alpha\in B}$ を B に対する基本要素重みの族とします。$(T_{\alpha})_{\alpha\in B}$ を不定数の族とします。 $\mathbf{Z}[(T_{\alpha})_{\alpha\in B}]$ から $\mathscr{R}(\mathfrak{g})$ までの写像 $f \rightarrow f(([\varpi_{\alpha}])_{\alpha\in B})$ は、環の同型です。

(ii) 準同型 ch $\mathscr{R}(\mathfrak{g})$ ～ $\mathbf{Z}[P]$ 誘導する同型環 $\mathscr{R}(\mathfrak{g})$ ～ 環 $\mathbf{Z}[P]^W$。

(iii) E を有限次元 $\mathfrak{g}$ 加群とする。 ch $E =\sum_{\lambda\in P_{++}}m_{\lambda}$ch[$\lambda ]$ の場合、最高重量 $\lambda$ の E の同型成分は長さ $m_{\lambda}$ を持ちます。

ファミリ $([\lambda ])_{\lambda\in P_{++}}$ は $\mathbf{Z}$ モジュール $\mathscr{R}(\mathfrak{g})$ の基底であり、ファミリ (ch[$\lambda ]$)$_{\lambda\in P_{++}}$] は $\mathbf{Z}$ モジュール $\mathbf{Z}[P]^W$ (補題 6、および第 4 章) の基底です。 VI, §3, no. 4、提案 3)。これは (ii) と (iii) を証明します。 主張 (i) は (ii)、補題 6 および第 4 章から続きます。 VI, §3, no. 4、木曜日。 1.

#### 系 {#lie-viii-s7-n7-cor-1 .statement tag=014C}

$E,E'$ を有限次元 $\mathfrak{g}$ 加群とする。このとき、ch E = ch $E'$ である場合に限り、E は $E'$ と同型です。

これはThから続きます。 2 (ii) と、$E,E'$ が半単純であるという事実。

### 練習問題 {#lie-viii-s7-exercises}

考慮されるすべての $\mathfrak{g}$ モジュール (演習 14 と 15 のものを除く) は有限次元であると仮定されます。

[§ 7 に対して練習問題](exercises/s7/)を参照してください。
