---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: IX
chapter_title: COMPACT REAL LIE GROUPS
section: 8
section_title: Fourier transform
lang: ja
source: lie-vii-ix
book_pages: 359-369, 417-418
pdf_pages: 0366-0376, 0424-0425
extraction: native
subsections:
    - "no": 1
      title: FOURIER TRANSFORMS OF INTEGRABLE FUNCTIONS
      page: 360
      pdf_page: 367
    - "no": 2
      title: FOURIER TRANSFORMS OF INFINITELY-DIFFERENTIABLE FUNCTIONS
      page: 362
      pdf_page: 369
    - "no": 3
      title: FOURIER TRANSFORMS OF CENTRAL FUNCTIONS
      page: 366
      pdf_page: 373
    - "no": 4
      title: CENTRAL FUNCTIONS ON G AND FUNCTIONS ON T
      page: 368
      pdf_page: 375
statements: 9
exercises: 6
content_sha256: 15a3e78041ec19c56ad11384a02c38d4745f9e9038e89421cad3a8a13ef031b8
translated_from: content/en/lie/IX/08_s8_fourier_transform.md
translation_method: google
source_content_sha256: 6e2618147afc628c71099020ffa7e02b28b7fa041ad48e0d3fc7f7f992c4cf3b
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 361230828d1642afeca5cdd40a4c833bf54362e74896a1f289e0c51ee86ab527
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 8。フーリエ変換

当社は、記法および前段落の規約を保持します。

場所の$^5$ 証明前掲書は、分裂半単純リー代数についてのみ記載されており、

分解的簡約リー代数の場合、変更なしで有効です。

### 1. フーリエ変換/可積分関数

この数では、いくつかの定義とスペクトル理論$^6$の結果を思い出します。

G の $\widehat{G}$ 集合の類の既約表現 (有限次元複素数ベクトル空間上) で表します。 すべての $u\in \widehat{G}$ について、$u$ と $d(u)$ の次元を $Eu$ 空間で表します。 $u$ の下で不変である $E_u$ 上に分離正のエルミート形が存在し、そのような 2 つの形は比例します。 これらの形式の 1 つに対する End(E$_u$) の要素 A の随伴物 (ノルム) を $A^*$ (または $\|A\|_{\infty}$) で表します。すべての $g\in G$ に対して、$u(g)^*=u(g)^{-1}=u(g^{-1})$ と $\|u(g)\|_{\infty}= 1$ があります。 $x\in \mathfrak{g}$ 全員に対して、$u(x)^*=-u(x) =u(-x)$ があります。

スカラー 積が次のようなヒルベルト空間構造を End(E$_u$) に与えます。

$\langle A|B\rangle =d(u)\mathrm{Tr}(A^*B) =d(u)\mathrm{Tr}(BA^*)$、(1)

そして置きます

$\|A\|_2=\langle A|A\rangle^{1/2}= (d(u)\mathrm{Tr}(A^*A))^{1/2}$。 (2)

我々は持っています

$$
\surd\overline{d(u)}\|A\|_{\infty}\leq  \|A\|_2\leq d(u)\|A\|_{\infty} \tag{3}
$$

それで

$$
|\langle A|B\rangle | \leq d(u)^2\|A\|_{\infty}\|B\|_{\infty} \tag{4}
$$

すべての $g\in G$ に対して、$\|u(g)\|_2=d(u)$ があります。

$F( \widehat{G})$ 代数 $\prod_{u\in\widehat{G}}$ End(E$_u$) で表します。ヒルベルト空間 End(E$_u$) のヒルベルト和を $L^2( \widehat{G})$ で示します。これは、スカラー 積を使用した、$\sum_u\|A_u\|^2_2<\infty$ となる家族 $A= (A_u)\in F( \widehat{G})$ の空間です。

$\langle A|B\rangle =\sum_{u\in\widehat{G}}\langle A_u|B_u\rangle =\sum_{u\in\widehat{G}}d(u$)Tr(A$^*_uB_u$)。 (5)

$L^2( \widehat{G})$ 上のヒルベルトノルムも $\| \|_2$ で表し、$A\in L^2( \widehat{G})$ に対して $\|A\|^2_2=\sum_{u\in\widehat{G}}\|A_u\|^2_2$ を表します。

$f$ が G 上の可積分複素数写像である場合、次のようにします。

$u(f) =\int_Gf(g)u(g)dg\in$ エンド(E$_u$) (6)

すべての$u\in \widehat{G}$に。 $\|u(f)\|_{\infty}\leq \int_G|f(g)|dg=\|f\|_1$ があります。 $\mathscr{F}(f)$ で示される $f$ のフーリエ共変換は、ファミリー $(u(f))_{u\in\widehat{G}}\in F( \widehat{G})$ です。 $f\in L^2( \widehat{G})$の場合、

$^6$ 注意 $^1$、§7、p. 66 を参照。

$$
\|f\|^2_2=\sum_{u\in\widehat{G}}\langle u(f)|u(f)\rangle =\|\overline{\mathscr{F}}(f)\|^2_2
$$

したがって、$\overline{\mathscr{F}}$ 誘導する他の語のヒルベルト空間 $L^2(G)$ からヒルベルト空間 $L^2( \widehat{G}):$ までの等角線形写像、$L^2$(G) の $f$ と $f'$ について、持っています

$\int_G\overline{f(g)}f'(g)dg=\langle \overline{\mathscr{F}}(f)|\overline{\mathscr{F}}(f')\rangle =\sum_{u\in\widehat{G}}d(u$)トリ($u(f)^*u(f')$)。 (7)

$L^1$(G) の $f$ と $f'$ について、$f$ と $f'$ の畳み込み積 $f*f'$ は次のように定義されます。

$$
(f*f')(h) =\int_Gf(hg^{-1})f'(g)dg=\int_Gf(g)f'(g^{-1}h)dg
$$

(積分はほぼすべての $h\in G$ で意味を成します)。

$f*f'\in L^1(G)$ と、すべての $u\in \widehat{G},u(f*f') =u(f)u(f')$ があるので、

$$
\overline{\mathscr{F}}(f*f') =\overline{\mathscr{F}}(f).\overline{\mathscr{F}}(f') \tag{8}
$$

逆に、$A = (A_u)_{u\in\widehat{G}}$ を $F( \widehat{G})$ の元とします。すべての $u\in \widehat{G}$ について、$\mathscr{F}_uA$ を次のように定義される G 上の (解析的) 写像とします。

$(\mathscr{F}_uA)(g) =\langle u(g)|A_u\rangle =d(u$)Tr(A$_uu(g)^{-1}$)。 (9)

$A\in L^2( \widehat{G})$ の場合、家族 $(\mathscr{F}_uA)_{u\in\widehat{G}}$ は $L^2(G)$ で要約可能です。 $\mathscr{F}$(A) で示される A のフーリエ変換は、この族の和です。 写像 $\mathscr{F}$ と $\mathscr{F}$ は、ヒルベルト空間 $L^2(G)$ と $L^2( \widehat{G})$ の間の逆同型です。

その他語:

#### 命題 1 {#lie-ix-s8-prop-1 .statement tag=01GZ}

G 上のすべての平方可積分複素数写像 $f$ は、$(f_u)_{u\in\widehat{G}}$ 族のヒルベルト空間 $L^2(G)$ の和です。ここで、すべての $h\in G$ とすべての $u\in \widehat{G}$ について、

$$
f_u(h) =\langle u(h)|u(f)\rangle
$$

$=d(u)\int_Gf(g$)トリ($u(gh^{-1})$)$dg=d(u)\int_Gf(gh$)トリ($u(g)$)$dg$。 (10)

すべての $u\in \widehat{G}$ 選ぶは $E_u$ の正規直交基底 $Bu$ であり、この基底の $u(g)$ の $(u_{ij}(g))$ 行列で表されます。提案 1 は、$\widehat{G}$ の $u$ と $B_u$ の $i, j$ の写像 $\surd\overline{d(u)}u_{ij}$ の族が、空間 $L^2(G)$ の正規直交基底であることも意味します。

$f$ が G 上の可積分関数で、族 $(f_u)$ が一様に合計可能である場合、この族の和は、$f$ とほぼどこでも一致するが​​連続する写像です。他の語では、加法で $f$ が連続であると仮定すると、すべての $h\in G$, $f(h) =\sum_{u\in\widehat{G}}d(u)\int_Gf(gh$)Tr($u(g)$)$dg$ になります。 (11)

逆に、$A\in F( \widehat{G})$; とします。ファミリ $(\mathscr{F}_uA)_{u\in\widehat{G}}$ が一様に合計可能な場合、写像

$g \rightarrow \sum_{u\in\widehat{G}}(\mathscr{F}_uA)(g) =\sum_{u\in\widehat{G}}d(u$)Tr(A$_uu(g)^{-1}$)

は、フーリエ共変換が A である G 上の連続写像です。

$f$ を G の可積分関数とし、$s\in G$ とします。 $\gamma (s)f=\varepsilon_s*f,\delta (s)f=f*\varepsilon_{s^{-1}}$ で定義される G 上の $\gamma (s)f$ と $\delta (s)f$ 写像で表します。つまり、

$g\in G$ の場合は $(\gamma (s)f)(g) =f(s^{-1}g),(\delta (s)f)(g) =f(gs)$、

(第 III, §3, no. 4 章および統合、第 VII, §1, no. 1 章)。我々は持っています

$$
u(\gamma (s)f) =\int_Gf(s^{-1}g)u(g)dg=\int_Gf(g)u(sg)dg
$$

それで

$$
u(\gamma (s)f) =u(s)u(f) \tag{12}
$$

そして同様に

$$
u(\delta (s^{-1})f) =u(f)u(s) \tag{13}
$$

When G is commutative, $\widehat{G}$ is the underlying set of the dual group of G (Spectral Theories, Chap. II, §1, no. $1$)$,d(u) = 1$ for all $u\in \widehat{G}$, and we recover the definitions of the Fourier transform given in Spectral Theories, Chap. II.

### 2. 無限微分可能写像のフーリエ変換

U(G) は、$\{e\}$ に含まれるサポートを含む G 上の分布の代数を表すことを思い出してください (第 III, §3, no. 1、定義 2)。 $\mathfrak{g}$ の標準単射を U(G) 拡大するから同型にリー代数 $\mathfrak{g}$ の代数から U(G) へ (上記、no. 7、提案 25)。これからは同一視するこの2人代数がこの同型になります。 $f$ が G 上の無限微分可能な複素数写像で、$t\in U(G)$ の場合、次のように定義される G 上の $L_tf$ と $R_tf$ 写像で表します。

$$
L_tf(g) =\langle \varepsilon_g*t, f\rangle ,R_tf(g) =\langle t*\varepsilon_g, f\rangle
$$

(cf. 前掲書、no. 6)。 $g\in G$の皆様、

$$
L_t\circ \gamma (g) =\gamma (g)\circ L_t,R_t\circ \delta (g) =\delta (g)\circ R_t
$$

$u\in \widehat{G}$ にしましょう。 $u$ の $Eu$ 空間で表します。 リー群 $u: G\rightarrow \mathbf{G}\mathbf{L}(E_u)$ の射は、(実数) リー代数 $\mathfrak{g}\rightarrow$ End(E$_u$) の準同型を与えるので、U(G) から代数の準同型も$u$ で表されます。終了(E$_u$)。 $t\in U(G)$ で、$f$ が G 上で無限微分可能な写像である場合、

$$
u(L_tf) =u(f)u(t^{\vee}), u(R_tf) =u(t^{\vee})u(f) \tag{14}
$$

where $t^{\vee}$ denotes the image of $t$ under the principal anti-automorphism of U(G) (Chap. I, §2, no. 4); indeed, it suffices to verify this for $t\in \mathfrak{g}$, in which case it follows by differentiation from formulas (12) and (13) (cf. Chap. III, §3, no. 7, Prop. 27).

すべての $u\in \widehat{G}$ について、$u($§7, no. 2 の $\lambda (u)$ 最高重量で表します。 1) したがって、$u \rightarrow \lambda (u)$ は、X(T) のドミナント元の $\widehat{G}$ から集合 $X_{++}$ までの全単射写像です。

$\Gamma \in U(G)$ を G (§7, no. 6) のカシミール元とします。すべての $u\in \widehat{G}$、自己準同型 $E_u$ の $u(\Gamma )$ はホモテティー で、その比率を $\widetilde{\Gamma}(u)$ で表すと、$\widehat{G}$ から $\mathbf{C}$ までの写像 $u \rightarrow \widetilde{\Gamma}(u)$ になります。

$\varphi$ と $\psi$ が正の実数値を持つ $\widehat{G}$ 上の 2 つの関数である場合、「すべての $u\in \widehat{G}$ に対して $\varphi (u)\leq M\psi (u)$ となるような $M>0$ が存在する」関係を「$\varphi \preccurlyeq \psi$」または「$\varphi (u)\preccurlyeq \psi (u$)」で表します。これは、正の実数値を持つ $\widehat{G}$ 上の関数のセットに関する事前順序関係です。

#### 命題 2 {#lie-ix-s8-prop-2 .statement tag=01H0}

$m \rightarrow  \|m\|$ を $\mathbf{R}$ ベクトル空間 $\mathbf{R}\otimes X(T)$ 上でノルムとし、$\Gamma$ を G のカシミール元とする。$\varphi$ を、正の実数値を持つ $\widehat{G}$ 上で写像とする。

a) 次の条件は同等です。

(i) $\varphi (u)\preccurlyeq (\|\lambda (u)\|+ 1)^n$ となるような整数 $n >0$ が存在します (それぞれ整数 $n >0$ に対して、$\varphi (u)\preccurlyeq (\|\lambda (u)\|+ 1)^{-n}$ が存在します)。

(ii) $\varphi (u)\preccurlyeq ( \widetilde{\Gamma}(u) + 1)^n$ となるような整数 $n >0$ が存在します (整数 $n >0$ ごとに、$\varphi (u)\preccurlyeq ( \widetilde{\Gamma}(u) + 1)^{-n}$ が存在します)。

b) G が半単純の場合、条件 (i) および (ii) も次と同等です。

(iii) $\varphi (u)\preccurlyeq d(u)^n$ となるような整数 $n >0$ が存在します (それぞれの整数 $n >0$ に対して、$\varphi (u)\preccurlyeq d(u)^{-n}$ が存在します)。

注意まず第一に、条件 (i) はノルムの選択から明らかに独立しています。したがって、$\Gamma ($§7, no. 6 に関連付けられた二次式形 $Q_{\Gamma}$ によって定義されたノルムを使用できます (提案 4)。それから

$$
0\leq \widetilde{\Gamma}(u) =\|\lambda (u) +\rho \|^2- \|\rho \|^2
$$

したがって $\widetilde{\Gamma}(u) + 1\preccurlyeq (\|\lambda (u)\|+ 1)^2\preccurlyeq \widetilde{\Gamma}(u) + 1$、したがって a)。

さらに、G が半単純の場合、

$\|\lambda (u) +\rho \|\preccurlyeq d(u)\preccurlyeq \|\lambda (u) +\rho \|^N$、ここで $N = 1/$2(暗さ $G-$ 暗さ T)

(§7, no. 5、Th. 3 のコリント 1)、したがって $\|\lambda (u)\|+ 1\preccurlyeq d(u)\preccurlyeq (\|\lambda (u)\|+ 1)^N$、したがって b)。

提案 2 から、条件 (i) は最大トーラス、チャンバー、ノルムの選択から独立しており、条件 (ii) はカシミール元の選択から独立していることがわかります。 写像 $\varphi$ 満たす条件 (i) と (ii) は中等度増加する (それぞれ急速減少する) と言われます。 2 つの中程度の積増加する写像は中程度の増加するです。緩やかな増加する写像と急速な減少する写像の積は急速な減少するです。 $\varphi$ が急速に減少するになる場合、ファミリー $(\varphi (u))_{u\in\widehat{G}}$ は合計可能です。

#### 例 {#lie-ix-s8-n2-exa-1 .statement tag=01H1}

写像 $u \rightarrow d(u)$ は中程度の増加する (§7, no. 5、Th. 3 のコリント 1)。 $\mathbf{R}\otimes X(T)$ のノルム $\| \|$ の場合、写像 $u \rightarrow  \|\lambda (u)\|$ は中程度の増加するです。どのカシミール元 $\Gamma$ についても、写像 $u \rightarrow \widetilde{\Gamma}(u)$ は中程度の増加するです。より一般的には:

#### 命題 3 {#lie-ix-s8-prop-3 .statement tag=01H2}

すべての$t\in$ U(G)、$\widehat{G}$ の写像 $u \rightarrow  \|u(t)\|_{\infty}$ および $u \rightarrow  \|u(t)\|_2$ は中程度の増加するです。

2 つの中程度増加する写像のうち積は中程度増加するであるため、その場合 §7, no. 6 と不等式の注意から主張が続く $t\in \mathfrak{g}:$ でこれを証明すれば十分です。

$$
\|u(t)\|_2\leq d(u)\|u(t)\|_{\infty}
$$

#### 定理 1 {#lie-ix-s8-thm-1 .statement tag=01H3}

a) $f$ を G 上の無限微分可能な複素数写像とします。すると、$f_u(g) =\langle u(g)|u(f)\rangle$ である族 $(f_u)_{u\in\widehat{G}}$ は G 上で一様に加算可能であり、すべての $h\in G$ について、

$f(h) =\sum_{u\in\widehat{G}}\langle u(h)|u(f)\rangle =\sum_{u\in\widehat{G}}d(u)\int_Gf(g$)Tr($u(gh^{-1})$)$dg$。

b) $f$ を G の可積分関数とします。その場合、$f$ は、写像 $u \rightarrow  \|u(f)\|_{\infty}$ が $\widehat{G}$ で急速に減少するになる場合に限り、ほぼどこでも無限微分可能な写像と等しくなります。

$f$ を G 上の無限微分可能な写像とし、$\Gamma$ を G のカシミール元とする。 公式 (14) 著、

$$
\widetilde{\Gamma}(u)^nu(f) =u(f)u(\Gamma )^n=u((L_{\Gamma})^nf)
$$

すべての$n\geq 0$にとって、そしてその結果として

$\widetilde{\Gamma}(u)^n\|u(f)\|_{\infty}\leq  \|(L_{\Gamma})^nf\|_1\leq$ sup$_{g\in G}|((L_{\Gamma})^nf)(g)|$; (15)

従って、写像 $u \rightarrow  \|u(f)\|_{\infty}$ は確かに急速に減少するになります。

逆に、写像 $u \rightarrow  \|A_u\|_{\infty}$ が急速に減少するとなるように、$A = (A_u)_{u\in\widehat{G}}$ を $F( \widehat{G})$ の元とします。 $f_u(g) =\langle u(g)|A_u\rangle$を入れてください。 写像 $g \rightarrow f_u(g)$ は解析的であるため、無限微分可能です。章著。 III, §3, no. 7、提案 27、

$$
(L_xf_u)(g) =\langle u(g)u(x)|A_u\rangle
$$

すべての$x\in \mathfrak{g}$に。 $t\in U(G)$ にしましょう。前の公式により、

$$
(L_tf_u)(g) =\langle u(g)u(t)|A_u\rangle
$$

そしてその結果として

$$
|(L_tf_u)(g)|=|\langle u(g)u(t)|A_u\rangle  \leq d(u)^2\|u(t)\|_{\infty}\|u(g)\|_{\infty}\|A_u\|_{\infty}
$$

$$
=d(u)^2\|u(t)\|_{\infty}\|A_u\|_{\infty}
$$

$d(u)$ と $\|u(t)\|_{\infty}$ は中程度の増加する (提案 3)、$\|A_u\|_{\infty}$ は急速に減少するであるため、写像 $u \rightarrow$ sup$_g|(L_tf_u)(g)|$ は急速に減少するです。従って、族 $(L_tf_u)_{u\in\widehat{G}}$ は一様に合計可能です。 $^7$ より、族 $(f_u)$ の和は G 上で無限微分可能な写像であり、そのフーリエ共変換は $(A_u)$ であるため、定理になります。

写像 $u \rightarrow  \|A_u\|_{\infty}$ が $\widehat{G}$ で急速に減少するになるように、家族 $A = (A_u)_{u\in\widehat{G}}$ の $L^2( \widehat{G})$ からなるの $\mathscr{S}( \widehat{G})$ ベクトル部分空間で表します。 定理から、複合体ベクトル空間 $\mathscr{C}^{\infty}(G;\mathbf{C})$ と $\mathscr{S}( \widehat{G})$ の間に写像 $\mathscr{F}:f \rightarrow (u(f))_{u\in\widehat{G}}$ と $\mathscr{F}: A \rightarrow \sum_{u\in\widehat{G}}\langle u(g)|A_u\rangle$ 誘導する逆同型が続きます。 $t\in U(G)$ および空間 $\mathscr{S}( \widehat{G})$ に対する半規範 $f \rightarrow$ sup$_{g\in G}|L_tf(g)|$ の族によって定義できる一様 $C^{\infty}$ 収束 (§6, no. 4) の空間 $\mathscr{C}^{\infty}(G;\mathbf{C})$ 位相を与えます。 位相は準規範 $p_n: A \rightarrow$ sup$_{u\in\widehat{G}}( \widetilde{\Gamma}(u) + 1)^n\|A_u\|_{\infty}$ の数列によって定義されます。 前述の証明の公式(15)は、$\overline{\mathscr{F}}$が連続であることを示しています。 $t\in U(G)$ とし、$A = (A_u)_{u\in\widehat{G}}$ を $\mathscr{S}( \widehat{G})$ の元とします。 $f_n(g) =\langle u(g)|A_u\rangle$を入れます。 $p$ を整数とし、$\sum_{u\in\widehat{G}}\widetilde{\Gamma}(u)^{-p}= M<\infty$ とします。 前述の証明により、すべての $g\in G$ に対して、次のような正の整数 $m$ が存在します。

$$
|(L_tf_u)(g)| \leq d(u)^2\|u(t)\|_{\infty}\|A_u\|_{\infty}\leq m.(1 + \widetilde{\Gamma}(u))^m\widetilde{\Gamma}(u)^{-p}\|A_u\|_{\infty}
$$

だから$|(L_t\mathscr{F}(A))(g)| \leq mMp_m(A)$;これは、$\mathscr{F}$ が連続であることを証明します。その結果：

#### 系 {#lie-ix-s8-n2-cor-1 .statement tag=01H4}

トポロジー ベクトル空間 $\mathscr{C}^{\infty}(G;\mathbf{C})$ と $\mathscr{S}( \widehat{G})$ の間の写像 $\overline{\mathscr{F}}:f \rightarrow (u(f))_{u\in\widehat{G}}$ と $\mathscr{F}: A \rightarrow \sum_{u\in\widehat{G}}\langle u(g)|A_u\rangle$ 誘導する逆同型。

$^7$ これは、空間 $\mathscr{C}^{\infty}(G;\mathbf{C})$、制服の位相という事実から導き出されます。

$C^{\infty}$-収束(§6, no. 4)、完了しました。

### 3. フーリエ変換の中心写像

すべての $u\in \widehat{G}$ について、$\chi_u$ 指標または $u$ で表します。従って、

$\chi_u(g) =$ トリ($u(g)$)$,(g\in G)$。 (16) スペクトルからのリコール理論公式

$$
\chi_u*\chi_v= 0(u, v\in \widehat{G}, u\not=v) \tag{17}
$$

$$
\chi_u*\chi_u=\frac{1}{d(u)}\chi_u(u\in \widehat{G}) \tag{18}
$$

すべての $u\in \widehat{G}$ について、$E_u$ の同一性写像を $\varepsilon_u$ で表します。 ZL$^2(G)$ は、中心となる関数 $f$ のクラスで構成される $L^2(G)$ の部分空間を表していることを思い出してください (§7, no. 4)。つまり、すべての $s\in G$ について $f\circ$ Int $s=f$、または同等のすべての $s\in G$ について $\gamma (s)f=\delta (s^{-1})f$ です。

#### 命題 4 {#lie-ix-s8-prop-4 .statement tag=01H5}

$f\in L^2(G)$ にしましょう。次に、$u(f)$ がすべての $u\in \widehat{G}$ に対してホモテティー である場合に限り、$f$ が中心となります。その場合

$$
u(f) =\frac{\varepsilon_u}{d(u)}\int_Gf(g)\chi_u(g)dg \tag{19}
$$

提案 1 (no. 1) によれば、$f$ が中心であるということは、すべての $s\in G$ とすべての $u\in \widehat{G}$ について $u(\gamma (s)f) =$ $u(\delta (s^{-1})f)$ を意味します。しかし、これは、すべての $s\in G$ とすべての $u\in \widehat{G}$ (公式 (12) および (13)) に対して $u(s)u(f) =u(f)u(s)$ と書くこともできるため、提案 4 (シュールの補題) の最初の主張となります。 $u(f)$がホモテティーの場合、$u(f) =\lambda_u\varepsilon_u$は

$\lambda_u=\frac{1}{d(u)}$ トリ($u(f)$) $=\frac{1}{d(u)}\int_Gf(g$) トリ($u(g)$) $dg=\frac{1}{d(u)}\int_Gf(g)\chi_u(g)dg$。

従って、$f\in$ ZL$^2(G)$ については、

$$
u(f) =\langle \overline{\chi}_u|f\rangle \frac{\varepsilon_u}{d(u)}\rangle \tag{20}
$$

それで

$$
\overline{\mathscr{F}}(f) =(\langle \overline{\chi}_u|f\rangle \frac{\varepsilon_u}{d(u)})_{u\in\widehat{G}} \tag{21}
$$

と

$$
\|\overline{\mathscr{F}}(f)\|^2_2=\sum||||\langle \overline{\chi}_u|f\rangle \frac{\varepsilon_u}{d(u)}||||^{22}=\sum|\langle \overline{\chi}_u|f\rangle |^2
$$

$uu$

逆に、$\varphi$ が $\widehat{G}$、$F( \widehat{G})$ 属するから $L^2( \widehat{G})$ の元 $(\frac{\varphi(u)}{d(u)}\varepsilon_u)_{u\in\widehat{G}}$ 上の平方積分可能複素数写像であり、 (公式 (9)) $(\mathscr{F}_u(\frac{\varphi(u)}{d(u)}\varepsilon_u))(g) =d(u$)Tr $(\frac{\varphi(u)}{d(u)}\varepsilon_uu(g)^{-1})=\varphi (u)\overline{\chi}_u(g)$ がある場合、

それで

$$
\mathscr{F}((\frac{\varphi(u)}{d(u)}\varepsilon_u))=\sum\varphi (u)\overline{\chi}_u \tag{22}
$$

$u\in \widehat{G}$

注意、特に公式 (20) と (21) は、$\widehat{G},^8$ の $u, v$ に対して与えられます。

$u(\overline{\chi}_v) = 0$ $u\not=v$ の場合、(23)

$u(\overline{\chi}_u) =\frac{\varepsilon_u}{d(u)}\in$ エンド(E$_u$)、(24)

$\overline{\mathscr{F}}(\chi_u) =\frac{\varepsilon_u}{d(u)}\in$ 終了(E$_u$)$\subset F( \widehat{G})$。 (25)

#### 命題 5 {#lie-ix-s8-prop-5 .statement tag=01H6}

$f$ を G 上の連続中心写像とします。すると、写像 $u \rightarrow  |\langle \chi_u|f\rangle |$ が $\widehat{G}$ 上で急速に減少するになる場合に限り、$f$ は無限微分可能です。その場合、

$$
f(g) =\sum_{u\in\widehat{G}}\langle \chi_u|f\rangle \chi_u(g)
$$

$g\in G$ 全員に。

Thさんより$1b)$、写像 $\overline{f}$ は、写像 $u \rightarrow  \|u(\overline{f})\|_{\infty}$ が急速に減少するになる場合に限り、無限微分可能です。しかし、(20)までに、

$$
\|u(\overline{f})\|_{\infty}=\frac{1}{d(u)}|\langle \chi_u|f\rangle |
$$

したがって、最初の主張は、写像 $d(u)$ と $\frac{1}{d(u)}$ が中程度の増加するであるためです。

$f$ は無限微分可能であると仮定します。 Th 著$1a),f(g) =\sum_{u\in\widehat{G}}f_u(g)$ はすべての $g\in G$ なので、

$f_u(g) =\langle u(g)|u(f)\rangle =d(u$)トリ($u(g)^{-1}.u(f)$)$=d(u$)トリ$(u(g)^{-1}\langle \overline{\chi}_u|f\rangle \frac{\varepsilon_u}{d(u)})$

$=\langle \overline{\chi}_u|f\rangle$Tr($u(g)^{-1}$)$=\langle \overline{\chi}_u|f\rangle \overline{\chi}_u(g)$。

したがって、$f(g) =\sum_{u\in\widehat{G}}\langle \overline{\chi}_u|f\rangle \overline{\chi}_u(g)$;しかし、すべての $u\in \widehat{G}$ について、$u$ の反比例表現 $u'$ は $\overline{\chi}_u=\chi_{u'}$ を満たし、写像 $u \rightarrow u'$ は $\widehat{G}$ の置換です。したがって、$f(g) =\sum_{u\in\widehat{G}}\langle \chi_u|f\rangle \chi_u(g)$ もあるので、命題となります。

$^8$ End(E$_u$) を積 $F( \widehat{G}) =\prod_{v\in\widehat{G}}$ End(E$_v$) に関連付けて埋め込みます。

$A\in$ $A_u= A$ と $A_v= 0$ が $v\not=u$ になるように、家族 $(A_v)_{v\in\widehat{G}}$ を終了(E$_u$)します。

#### 系 {#lie-ix-s8-n3-cor-1 .statement tag=01H7}

$f$ を G 上の連続中心写像とします。すると、T に対する $f$ の制限が無限微分可能である場合に限り、$f$ は無限微分可能です。

確かに、Cor による。 §7, no. 4 の 4、

$\langle \chi_u|f\rangle =\int_G\overline{\lambda(u)(t)}\varphi (t)dt$、ここで$\varphi (t) =\prod_{\alpha >0}(1-\alpha (t)^{-1})f(t)$。

$f|T$ が無限微分可能である場合、$\varphi$ も無限微分可能です。提案 5 により、群 T、$\widehat{T} = X(T)$ の写像 $\mu \rightarrow \int_T\overline{\mu(t)}\varphi (t)dt$ は急速に減少するになり、写像 $u \rightarrow  \langle \chi_u|f\rangle$ も同様です。したがって、写像 $f$ は無限微分可能です (提案 5)。 逆はクリアです。

### 4. 中心的 G の写像および T の写像

G 上の連続複素数値写像の $\mathscr{C}(G)$ 空間と無限微分可能写像の $\mathscr{C}^{\infty}(G)$ 部分空間で表します。次に、インクルージョンが数列あります

$$
\Theta (G)\subset \mathscr{C}^{\infty}(G)\subset \mathscr{C}(G)\subset L^2(G)
$$

これらのさまざまな空間の中央写像の部分空間からなるを、それぞれ$Z\Theta (G),Z\mathscr{C}^{\infty}(G),Z\mathscr{C}(G)$、ZL$^2$(G)で表します。 空間 $\Theta (T),\mathscr{C}^{\infty}(T),\mathscr{C}(T),L^2(T)$も同様に紹介します。このリスト内の任意の空間 E については、不変式 (反不変式) の $E^W$ (それぞれ $E^{-W}$) 部分空間からなる 、ワイル群 W の演算については元で表します。 図式

$$
Z\mathscr{C}(G)\longrightarrow^{a_c}\mathscr{C}(T)^W
$$

$$
Z\mathscr{C}^{\infty}(G)\longrightarrow^{a_{\infty}}\mathscr{C}^{\infty}(T)^W
$$

$$
Z\Theta (G)\longrightarrow^{a_{\Theta}}\Theta (T)^W
$$

ここで、垂直矢印は標準単射を表し、写像 $a_c, a_{\infty}, a_{\Theta}$ は $\mathscr{C}(G)$ から $\mathscr{C}(T)$ まで制限写像によって誘導されます。

写像 $a_c, a_{\infty}, a_{\Theta}$ は全単射です (§2, no. 5、提案 5 の Cor. 1、§8, no. 3、提案 5 の Cor.、および §7, no. 3、提案 2 の Cor.)。

ここで、X(T) に対する正の根属するの半和 $\rho$ が、T 上のすべての連続写像 $\varphi$ と $\varphi .J(\rho )$ に関連する写像 $b$ を考えます。可換図式があります

ZL$^2(G)--------------------\longrightarrow^uL^2(T)^{-W}$

$$
Z\mathscr{C}(G)\longrightarrow^{a_c}\mathscr{C}(T)^W\longrightarrow^{b_c}\mathscr{C}(T)^{-W}
$$

$$
Z\mathscr{C}^{\infty}(G)\longrightarrow^{a_{\infty}}\mathscr{C}^{\infty}(T)^W\longrightarrow^{b_{\infty}}\mathscr{C}^{\infty}(T)^{-W}
$$

$$
Z\Theta (G)\longrightarrow^{a_{\Theta}}\Theta (T)^W\longrightarrow^{b_{\Theta}}\Theta (T)^{-W}
$$

ここで、垂直矢印は正準包含物であり、写像 $b_c, b_{\infty}, b_{\Theta}$ は $b$ によって、$u$ 拡大する $b_c\circ a_c$ は連続性によって誘発されます (§7, no. 4、Th. 2 の Cor. 3)。 写像 $u$ と $b_{\Theta}$ は全単射です (上記引用)。 $b_{\infty}$ (演習 5) も同様です。一方、$b_c$ は一般に全射ではありません (例題 6)。

### 練習問題 {#lie-ix-s8-exercises}

[§ 8 に対して練習問題](exercises/s8/)を参照してください。
