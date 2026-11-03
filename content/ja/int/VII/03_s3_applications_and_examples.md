---
book: int
book_title: Integration
chapter: VII
chapter_title: HAAR MEASURE
section: 3
section_title: Applications and examples
lang: ja
source: int-vii-ix
book_pages: INT VII.53-INT VII.73, INT VII.91-INT VII.94
pdf_pages: 0059-0079, 0097-0100
extraction: ocr
subsections:
    - "no": 1
      title: Compact groups of linear mappings
      page: 53
      pdf_page: 59
    - "no": 2
      title: Triviality of fibered spaces and of group extensions
      page: 55
      pdf_page: 61
    - "no": 3
      title: Examples
      page: 60
      pdf_page: 66
statements: 24
exercises: 12
content_sha256: 967809fe9d8c14480f63e554969b798eba35fc1185d828fa3102fe8fcbb647ae
translated_from: content/en/int/VII/03_s3_applications_and_examples.md
translation_method: google
source_content_sha256: 77d86192dc78c3caea75d568c8ef5d05992c7bdcaed4b1daac8f963f1400d1ea
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: d5a43600de6a4819b24311a3462354d9ea44d05d792b239ed25f49d2b3bc5039
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。アプリケーションと例

### 1. コンパクトな群/線形写像

$E$ を $\mathbf{R}, \mathbf{C}$ または $\mathbf{H}$ よりも有限次元ベクトル空間とします。 この場合、$\mathrm{End}(E)$ は $\mathbf{R}$ 上の有限次元代数であり、$\mathrm{End}(E)$ (§ 1, No. 10) 上の正規の位相はコンパクト収束の位相です。 群 $\mathrm{Aut}(E) = \mathbf{GL}(E)$ は $\mathrm{End}(E)$ のオープン部分集合であるため、局所的にコンパクトな群です。 Let $(e_1, e_2, \ldots, e_n)$ be a basis of $E$ and, for every endomorphism $u$ of $E$, let $M(u) = (\alpha_{ij}(u))$ be the matrix of $u$ with respect to this basis; to say that a subset $S$ of $\mathrm{End}(E)$ is relatively compact in $\mathrm{End}(E)$ is equivalent to saying that the functions $\alpha_{ij}(u)$ are bounded in $S$.

#### 命題 1 {#int-vii-s3-prop-1 .statement tag=09GS}

— *G を Aut(E)* の部分群とします。 *次の 3 つのプロパティは同等です*:

(i) *G は End(E)* 内で比較的コンパクトです。
(ii) *G は Aut(E)* では比較的コンパクトです。
(iii) *G は、E* 上で非縮退$^1$ 正のエルミート形を不変のまま残します。

(iii) $\Rightarrow$ (i): $G$ が非縮退正のエルミート形 $\Psi$ を不変のまま残すと仮定します。 $(e_1, \ldots, e_n)$ を $\Psi$ の正規直交値基底とします (*Alg.*、Ch. IX, § 6, No. 1、Th. 1 の Cor. 1)。すべての $u \in G$ について、$(e_i)$ に関して $(u_{ij})$ をその行列とします。任意の $j$ については $\sum_{i=1}^n |u_{ij}|^2 = 1$ があり、したがってすべての $i$ と $j$ については $|u_{ij}| \leq 1$ となり、(i) が証明されます。

(i) $\Rightarrow$ (ii): これは GT、X, § 3, No. 5、Cor. から続きます。 Thの。 4、$\mathrm{End}(E)$の位相がコンパクトな収束であるという事実を考慮します。

(ii) $\Rightarrow$ (iii): $\mathrm{Aut}(E)$ の$G$ の閉包 $\overline{G}$ がコンパクトであるとします。 $\Phi$ を $E$ に対する非縮退ポジティブエルミート形とします。スカラーの体が$\mathbf{R}$または$\mathbf{C}$の場合、$\Phi$を与えると$E$は有限次元のヒルベルト空間になり、条件(iii)は次の補題の結果となります。

$^1$ 非一般的。 EVT では、項は séparante に置き換えられ、その後「分離」と翻訳されます (TVS、V, § 1, No. 1)。

#### 補題 1 {#int-vii-s3-lem-1 .statement tag=09GT}

F をヒルベルト空間、K をコンパクト群、および $\mathscr{L}(F; F)$ の可逆元の群における K の s ↦ U(s) 表現を点単位収束の位相にわたって連続するとします。 F には次のような非縮退正のエルミート形 $\varphi$ が存在します。

$$
\varphi(U(s)x, U(s)y) = \varphi(x, y)
$$

すべての $s \in K, x \in F, y \in F$ について、および $\varphi$ (TVS、V, §1, No. 3) によって定義される F のトポロジー ベクトル空間構造が F の元の構造と同一であるようにします。

$\alpha$ を K のハール測度としましょう。F の任意の $x, y$ について、写像 $s \mapsto (U(s)x|U(s)y)$ は連続です。 集合

$$
\varphi(x, y) = \int (U(s)x|U(s)y)\, d\alpha(s).
$$

$\varphi(x, y)$ が F 上のセスクリニア形であるのは明らかです。 自己準同型 $U(s)$ の集合は $\mathscr{L}_s(F; F)$ でコンパクトなので、すべての $s \in K$ に対して $\|U(s)\| \leq M$ となるような定数 M が存在します。したがって、$x \in F$ ごとに、

$$
M^{-1}\|x\| \leq \|U(s)x\| \leq M\|x\|,
$$

よって不平等

$$
M^{-2}\alpha(K)\|x\|^2 \leq \varphi(x, x) \leq M^2\alpha(K)\|x\|^2,
$$

これは、$\varphi$ が正で非縮退であること、およびノルム $\varphi(x, x)^{1/2}$ がノルム $\|x\|$ と同等であることを示しています。最後に$t \in K$の皆様、

$$
\begin{align*}
\varphi(U(t)x, U(t)y) &= \int (U(st)x|U(st)y)\, d\alpha(s) \\
&= \int (U(s)x|U(s)y)\, d\alpha(s) = \varphi(x, y).
\end{align*}
$$

スカラーの体が $\mathbf{H}$ の場合、$\mathbf{H}$ の値を使用して、G で定義された写像 $s \mapsto \Phi(sx, sy)$ によって、どこでも写像 $s \mapsto (U(s)x|U(s)y)$ の置き換えることで前にとまったく同じように議論できます。これで命題の証明が完了です。

#### 注意 {#int-vii-s3-n1-rem-1 .statement tag=09GU}

$\Phi$ を E 上の非縮退正エルミート形とします。ユニタリ群 $\mathbf{U}(\Phi)$ は $\mathrm{Aut}(E)$ で閉じているため、コンパクトです (提案 1)。提案 1 は、$\mathrm{Aut}(E)$ のすべてのコンパクト部分群が形 $\mathbf{U}(\Phi)$ の部分群に含まれることも示しています。ここで $\mathbf{U}(\Phi)$ が $\mathrm{Aut}(E)$ のコンパクト部分群 K に含まれている場合、$\mathbf{U}(\Phi) \subset K \subset \mathbf{U}(\Phi')$ のような非縮退正のエルミート形 $\Phi'$ が E 上に存在することがわかり、簡単に続きます。

(例 1) $\Phi$ と $\Phi'$ は比例する、よって $\mathbf{U}(\Phi) = K$。したがって、$\mathrm{Aut}(E)$ の最大コンパクト部分群は、形 $\mathbf{U}(\Phi)$ の部分群です。

### 2. ファイバー化された空間と群拡大の自明性

#### 命題 2 {#int-vii-s3-prop-2 .statement tag=09GV}

*X を局所コンパクト空間とし、局所コンパクト群 H が $(x, \xi) \mapsto x\xi$ までに右側に継続的かつ適切に作用するようにします。 X/H がパラコンパクトであると仮定します。 g を $\mathbf{R}^n$ の H の連続表現とする。次に、X から $\mathbf{R}^n$ への連続写像 f が存在し、すべての $x \in X$ と $\xi \in H$ に対して $f(x\xi) = f(x) + g(\xi)$ になります。

$n = 1$ の場合にはすぐに 1 つの簡約するが発生します。 加法群 $\mathbf{R}$ は乗法群 $\mathbf{R}_+^*$ と同型なので、命題は §2, No. 4 の提案 7 の明らか帰結になります。

#### 系 {#int-vii-s3-n2-cor-1 .statement tag=09GW}

*X を、有限次元実数ベクトル空間 V が右側で $(x, v) \mapsto xv$ まで継続的かつ適切に作用する、局所的にコンパクトな空間とします。 $\pi$をXの標準写像を$B = X/V$にするとします。 B がパラコンパクトであると仮定します。*

a) *すべての $x \in X$ と $v \in V$ に対して $f(xv) = f(x) + v$ となるように、 X から V への連続写像 f が存在します。

b) *f が a) の写像満たす条件である場合、写像 $x \mapsto (\pi(x), f(x))$ は X の $B \times V$ への同写写像です。

主張 a) は、g が V の恒等写像であるとみなされる提案 2 からの結果です。 f を a) の写像満たす条件とします。 X から X への写像 $x \mapsto x \cdot (-f(x))$ は連続であり、各軌道で定数であるため、 形 $\varphi \circ \pi$ になります。ここで、$\varphi$ は B から写像への連続です。 X; $b \in B$、$\pi(\varphi(b)) = b$ごとに。 写像 X の $x \mapsto (\pi(x), f(x))$ から $B \times V$ と $B \times V$ の $(b, v) \mapsto \varphi(b) \cdot v$ から X は、$\varphi(\pi(x)) \cdot f(x) = x \cdot (-f(x)) \cdot (f(x)) = x$、$\pi(\varphi(b) \cdot v) = \pi(\varphi(b)) = b$、そして $b = \pi(y)$ の場合、

$$
f(\varphi(\pi(y)) \cdot v) = f(y \cdot (-f(y)) \cdot v) = f(y) - f(y) + v = v .
$$

これらの写像は連続なので、準同型です。

#### 注意 {#int-vii-s3-n2-rem-1 .statement tag=09GX}

— E を有限次元の実アフィン空間、T をコンパクト空間、$\mu$ を *総質量* 1 の T 上の測度、f を T から E への連続写像とする。E の原点 a が選択されると、E はベクトル空間構造を備え、積分したがって、$\int_T f(t) d\mu(t)$ には意味があります。これは、次のような E の点 x を表します。

$$
x - a = \int_T (f(t) - a) d\mu(t) .
$$

この点は、$a$の選択とは独立しています。というのは、$a' \in \mathbf{E}$ と $x' \in \mathbf{E}$ が $x' - a' = \int_{\mathbf{T}} (f(t) - a') d\mu(t)$ になるとします。それから

$$
x' - a = (x' - a') + (a' - a) = \int_{\mathbf{T}} (f(t) - a') d\mu(t) + \int_{\mathbf{T}} (a' - a) d\mu(t)
$$
$$
= \int_{\mathbf{T}} (f(t) - a) d\mu(t) = x - a,
$$

よって $x' = x$。したがって、$\mathbf{E}$ の起源の選択を指定せずに、記号 $\int_{\mathbf{T}} f(t) d\mu(t)$ を使用してもよいでしょう。 $u$ が $\mathbf{E}$ の他の有限次元アフィン空間 $\mathbf{E}'$ へのアフィン写像である場合、

$$
u \left( \int_{\mathbf{T}} f(t) d\mu(t) \right) = \int_{\mathbf{T}} u(f(t)) d\mu(t).
$$

なぜなら、$\mathbf{E}$ と $\mathbf{E}'$ は、$u$ が線形写像になるような方法でベクトル空間と同一視される可能性があり、その場合、公式が知られます (Ch. III, §3, No. 2、提案 2 および No. 3、提案 7)。

#### 補題 2 {#int-vii-s3-lem-2 .statement tag=09GY}

*$G$ をコンパクト群、$\mu$ を $G$ の正規化ハール測度、$\mathbf{E}$ を有限次元の実アフィン空間、$A$ を $\mathbf{E}$ のアフィン群とします。 $\rho$ 準同型の $G$ を $A$ にします。 $x \in \mathbf{E}$ごとに、$G$から$\mathbf{E}$への写像$s \mapsto \rho(s)x$が連続していると仮定します。その後、$x \in \mathbf{E}$ ごとに、点*

$$
x_0 = \int_G \rho(s)x\, d\mu(s) \in \mathbf{E}
$$

*は $G$ では不変です。*

$t \in G$ごとに、

$$
\rho(t)x_0 = \int_G \rho(t)\rho(s)x\, d\mu(s) = \int_G \rho(ts)x\, d\mu(s) = \int_G \rho(s)x\, d\mu(s) = x_0.
$$

#### 命題 3 {#int-vii-s3-prop-3 .statement tag=09GZ}

*$G$を局所的にコンパクトな群とします。 $H$ を $G$ の閉じた法線部分群とし、$\mathbf{R}^n$ と同型で、$G/H$ がコンパクトになるようにします。*

a) *$G$ が $L$ と $H$ の位相的半直接積であるような、$G$ の閉じた部分群 $L$ が存在します。

b) *$M$ が $G$ のコンパクト部分群である場合、$x^{-1}Mx \subset L$ となるような元 $x \in H$ が存在します。

c) *$G$ のすべてのコンパクト部分群は、最大コンパクト部分群に含まれます。*

d) *$G$の最大コンパクト部分群は、$L$の変換×$G$の内部自己同型である部分群です。

$\pi$ を $G$ の標準準同型から $K = G/H$ に移します。 $G \times H$ の商、写像 $(s, h) \mapsto shs^{-1}$ が $H$ 定義するに進み、$K \times H$ の$H$ に連続する写像 $(\sigma, h) \mapsto \sigma \cdot h$ が続き、$shs^{-1} = \pi(s) \cdot h$ になります。 $\mathbf{R}^n$ で同一視する $H$ を計算します (したがって、場合に応じて、$H$ の群法則に対して乗法または加法記法を使用します)。 コルによって。提案 2 の場合、$x \in G, h \in H$ に対して $f(xh) = f(x) + h$ となるような、$G$ から $H$ への連続する写像 $f$ が存在します。 すべての $x \in G$ について、$p(x) = x \cdot (-f(x))$ とします。これは、$H$ に関する $x$ の剰余類にのみ依存します。 集合

$$
\begin{align*}
(1) \quad F(x, y) &= p(xy)^{-1} p(x)p(y) = f(xy)y^{-1}x^{-1}x(-f(x))y(-f(y)) \\
&= f(xy)[y^{-1}(-f(x))y](-f(y)) \\
&= f(xy) - \pi(y)^{-1}f(x) - f(y).
\end{align*}
$$

*if* $F(x, y) = 0$ *for all* $x, y$ *in* $G$ である場合、$p(G) = L$ は $G$ の部分群であり、$H$ の各剰余類を 1 つだけ点で交差します。 $p$ は連続であるため、$G$ は $L$ と $H$ (GT, III, §2, No. 10) の位相的半直接積になります。

さて、任意の $h, h' \in H$ について、

$$
\begin{align*}
F'(xh, yh') &= f(xhyh') - \pi(y)^{-1}f(xh) - f(yh') \\
&= f(xhy) + h' - \pi(y)^{-1}f(x) - \pi(y)^{-1}h - f(y) - h' \\
&= f(xy(\pi(y)^{-1}h)) - \pi(y)^{-1}f(x) - f(y) - \pi(y)^{-1}h \\
&= f(xy) - \pi(y)^{-1}f(x) - f(y) = F(x, y).
\end{align*}
$$

したがって、$F$ 定義するは、商への通過によって、$K \times K$ から $H$ への継続的な写像 $\varphi$ になります。

一方、$G$ のすべての $x, y, z$ については、

$$
\begin{align*}
F(z, xy) + F(x, y) &= f(zxy) - \pi(xy)^{-1}f(z) - f(xy) + f(xy) \\
&\phantom{=} - \pi(y)^{-1}f(x) - f(y) \\
&= \pi(y)^{-1}f(zx) - \pi(xy)^{-1}f(z) - \pi(y)^{-1}f(x) + f(zxy) \\
&\phantom{=} - \pi(y)^{-1}f(zx) - f(y) \\
&= \pi(y)^{-1}F(z, x) + F(zx, y),
\end{align*}
$$

したがって、$K$ のすべての $x', y', z'$ について、

$$
-\varphi(x', y') = \varphi(z', x'y') - {y'}^{-1}\varphi(z', x') - \varphi(z'x', y').
$$

$K$ の正規化ハール測度 $\alpha$ を使用して、$z'$ に関して積分してみましょう。 設定 $\psi(x') = \int \varphi(z', x')\, d\alpha(z')$、$\psi$ は K 上で連続する写像であり、(観察するとでは $\mathbf{R}^n$ の K の演算は GT、VII, §2, No. 1、Prop による $\mathbf{R}^n$ のベクトル空間構造を尊重します。 1)、得られるのは

$$
-\varphi(x', y') = \psi(x'y') - {y'}^{-1}\psi(x') - \psi(y').
$$

その他の語、設定 $k - \psi \circ \pi$では、Gで写像が連続し、

(2)
$$
-F(x, y) = k(xy) - \pi(y)^{-1}k(x) - k(y).
$$

(1) と (2) を比較すると、$f$ が連続する写像 $f + k$ (検証済みの性質 $f(xh) = f(x) + h$ が残る) に置き換えられると、F が 0 に置き換えられ、前に見たように、これで a の証明が完了することがわかります。

すべての $g \in G$ について、$l_g$ (それぞれ $h_g$) を L (それぞれ H) の一意元とし、$g = h_g l_g$ とします。 $h_1 \in H$ と $g \in G$ の場合、

$$
gh_1 = h_g l_g h_1 = h_g(l_g h_1 l_g^{-1})l_g,
$$

従って、$h_g h_1 = h_g + l_g h_1 l_g^{-1}$。すべての $g \in G$ について、$\psi_g$ を H の写像とし、次のように定義します。

$$
\psi_g(h_1) = h_g + l_g h_1 l_g^{-1}.
$$

$G \times H$ の H への写像 $(g, h_1) \mapsto \psi_g(h_1)$ は連続であり、H を G に対して同次の空間にし、原点の固定群は L であることがわかります。さらに、H が $\mathbf{R}^n$ と同一視されるとき、$\psi_g$ は H のそれ自体への *アフィン* 写像であることが観察されます。つまり、M を G の圧縮部分群とします。 補題 2 までに、*すべて* $m \in M$ に対して $\psi_m(x) = x$ となるような $x \in H$ が存在します。 $y \in H$ の場合、$\psi_y$ はベクトル $y$ との翻訳です。従って、$m \in M$、$\psi_{x^{-1}} \circ \psi_m \circ \psi_x$ 変換ごとに H の原点がそれ自体に入り、従って $x^{-1}mx \in L$ になるということになります。これは、$x^{-1}Mx \subset L$、よって b) を証明します。

$L'$ を G 含む L の閉じた部分群とします。 この場合、$L'$ は、L と $L' \cap H$ のトポロジカル半直接積です。 $L'$ がコンパクトであれば、$L' \cap H$ もコンパクトであるため、簡約するから点 (GT、IV, §2, No. 2、Th. 2 の Cor. 1)、従って $L' = L$ になります。 これは、L が G の最大コンパクト部分群であることを証明します。従って、Lの変換×Gの内部自己同型である部分群にも同じことが当てはまります。 提案 3 の主張 c) と d) は、b) の明らか帰結になります。

#### 命題 4 {#int-vii-s3-prop-4 .statement tag=09H0}

*K = G/H がコンパクトとなるように、G を局所的にコンパクトな群 、H を G の閉じた法線部分群とします。次に、$\mathbf{R}$ の H のすべての連続表現 u は、すべての $\xi \in H$ と $s \in G$ の $u(s\xi s^{-1}) = u(\xi)$ が、$\mathbf{R}$ の G の連続表現に拡張できます。

$L = G \times \mathbf{R}$ を、M を $(\xi, -u(\xi))$ の集合とします。ここで、$\xi$ は H を超えます。M が L の閉じた法線部分群であることは明らかです。 $L' = L/M$ と $\pi$ を $L'$ 上の L の標準写像とします。 M と R によって生成された L の部分群は H × R であるため、閉じられます。従って、π(R) は L' の閉じた部分群 N です。 π から R への制限 ρ は、R から N への全単射連続表現です。 付録 1 の補題 2 は、ρ が共連続であることを証明します。さらに、L'/N は L/(H × R) = G/H と同型であるため、コンパクトです。提案 3 により、N が L' の中心にあるという事実を考慮すると、L' は、他の部分群を含む N の積になります。従って、N 上では L' の連続表現が存在し、N 上では簡約するから恒等写像まで存在します。従って、R 上では自明な L の連続表現 v が存在し、R 上では恒等写像までの簡約するが存在します。 ξ ∈ H の場合、v((ξ, 0)) = v((ξ, −u(ξ))(e, u(ξ))) = u(ξ) となり、証明が完成します。

#### 補題 3 {#int-vii-s3-lem-3 .statement tag=09H1}

G を e のコンパクトな近傍によって生成されたトポロジー 群とします。 H を、同次空間 G/H がコンパクトになるような G の閉じた部分群とします。次に、H 内の e のコンパクトな近傍によって H が生成されます。

C を G = CH となるようなコンパクト集合とします。必要に応じて C を拡大すると、C 生成する G および G = ĈH と仮定できます。この場合、C^2 はコンパクトであり、開いた Ĉs (s ∈ H) によって覆われます。従って、H には C^2 ⊂ Ĉs_1 ∪ ... ∪ Ĉs_n となる s_1, ..., s_n が存在します。 Γ を s_i によって生成された H の部分群とします。次に C^2 ⊂ CΓ です。 帰納法により、n ごとに C^n ⊂ CΓ となるため、G = CΓ となります。 H のすべての元は、a ∈ C、b ∈ Γ、よって a ∈ H、よって a ∈ C ∩ H を持つ形 ab に入れることができます。 従って、H は C ∩ H によって生成され、 s_i、つまりコンパクトな集合によるものです。

#### 補題 4 {#int-vii-s3-lem-4 .statement tag=09H2}

G を接続されたトポロジカル群、D を G の完全に切断された法線部分群とします。すると、D は G の中心に含まれます。

d ∈ D とします。連続写像 x ↦ xdx^{-1} の下での G の像は D の部分集合であり、したがって簡約するが {d} に接続されます。これは、すべての x ∈ G について xd = dx であることを証明します。

#### 命題 5 {#int-vii-s3-prop-5 .statement tag=09H3}

G を、K = G/D がコンパクトであり、K の交換子部分群が K 内で密であるような、離散法線部分群 D を許容する接続トポロジー 群とします。その場合、D は有限で、G はコンパクトです。

群 G は局所的に K (GT, III, §2, No. 6, 提案 19) と同型であるため、局所的にコンパクトです。接続されているため、e のコンパクトな近傍によって生成されます。 補題 3 と 4 により、D は有限生成されたアーベル群であるため、D_1 有限 (A, VII, §4, No. 7, Th. 3) と群 $\mathbf{Z}^r \times D_1$ に同型です。 r > 0 であると仮定します。 すると、$\mathbf{Z}$上にDの表現fが存在します。 提案 4 により、f は R の G の連続表現 g に拡張できます。 商に進むと、$\mathbf{R}/\mathbf{Z}$ の $K$ の連続する定義する表現 $g'$。 $\mathbf{R}/\mathbf{Z}$ は $g'$ のアーベル、核含む交換子部分群 $K$ であるため、$g'$ は自明です。他には語、$g(G) \subset \mathbf{Z}$。 $G$ がつながっているので、$g(G) = \{0\}$ になりますが、$f(D) = \mathbf{Z}$ なので不合理です。 従って、$r = 0$ と $D$ は有限です。 その結果、$G$ はコンパクトになります (GT、III, §4, No. 1、提案 2 の Cor. 2)。

### 3. 例

この小節 (例 7 と 8 を除く) では、$K$ は非離散の局所的にコンパクトな可換体を表します。 $dx$ は、$K$ の加法群の Haar 測定値を示します。

$K = \mathbf{R}$のときは$\operatorname{mod} x = |x|$、$K = \mathbf{C}$のときは$\operatorname{mod} x = |x|^2$、$K = \mathbf{Q}_p$のときは$\operatorname{mod} x = |x|_p$であることを思い出してください。

#### 例 1 {#int-vii-s3-n3-exa-1 .statement tag=09H4}

一般リニア群。

$A$ を代数 $M_n(K)$ とします。 $A$の可逆元の群$A^*$は、一般的な線形群$\mathbf{GL}(n, K)$に他なりません。 $X \in A$ ごとに、被約ノルム $\operatorname{Nrd}_{A/K}(X)$ は $\det X$ になります。その結果、$N_{A/K}(X) = (\det X)^n$ (Alg.、Ch. VIII, §12, No. 3、提案 8; cf. A、III, §9, No. 3、例 3)。 $X \mapsto {}^t X$は$A$の同型を反対多元環にすると、

$$
N_{A^0/K}(X) = N_{A/K}({}^t X) = \det ({}^t X)^n = (\det X)^n.
$$

次に、§1, No. 11 の提案 16 は、この措置が次のことを証明します。

$$
\operatorname{mod}(\det X)^{-n} \cdot \bigotimes_{i,j} dx_{ij} \quad (X = (x_{ij}))
$$

$\mathbf{GL}(n, K)$の左右のハール尺度です。

決定する $\mathbf{GL}(n, K)$ における比較的不変の尺度を決定するするには、次の補題に依存します。

#### 補題 5 {#int-vii-s3-lem-5 .statement tag=09H5}

$\mathbf{C}^*$の$\mathbf{GL}(n, K)$の連続表現は形$X \mapsto \chi(\det X)$の写像で、$\chi$は$\mathbf{C}^*$の$K^*$の連続表現です。

このような写像は、明らかに$\mathbf{C}^*$の$\mathbf{GL}(n, K)$の連続した表現です。逆に、$\psi$が$\mathbf{C}^*$の$\mathbf{GL}(n, K)$の連続表現だとします。 $x \in K^*$、集合の場合

$$
\tilde{x} = \begin{pmatrix}
x & & \\
& 1 & 0 \\
& & 1 \\
0 & \cdots & 1
\end{pmatrix}
$$

そして$\chi(x) = \psi(\widetilde{x})$。次に、行列 $X \in \mathbf{GL}(n, K)$ ごとに、$(\det X^{-1}) \sim \cdot X \in \mathbf{SL}(n, K)$ が得られます。 $\mathbf{SL}(n, K)$ は $\mathbf{GL}(n, K)$ の交換子部分群であるため (A、III, §8, No. 9、提案 17 の修正)、$\psi((\det X^{-1}) \sim \cdot X) = 1$、よって
$$
\psi(X) = \psi((\det X) \sim) = \chi(\det X).
$$
これは確立しました、コル。 §1, No. 8 の提案 10 の 1 は、$\mathbf{GL}(n, K)$ の比較的不変な測度が、定数因子までは形の測度であることを証明しています。
$$
(4) \quad \chi(\det X) \cdot \bigotimes_{ij} dx_{ij} \qquad (X = (x_{ij})),
$$
ここで、$\chi$ は、$\mathbf{C}^*$ の $K^*$ の連続する表現です。

#### 例 2 {#int-vii-s3-n3-exa-2 .statement tag=09H6}

**アフィン群.**
すべての $X \in \mathbf{GL}(n, K)$ とすべての $x \in K^n$ について、$(X, x)$ を $K^n$ のアフィン線形写像 $\xi \mapsto X\xi + x$ とします。 $(X, x)$ の集合は、$K^n$ (A、II, §9, No. 4) のアフィン群 $G$ です。翻訳の集合 $T$ は、$G$ の閉じた正規形部分群であり、正準的に $K^n$ と同型です。一方、$\mathbf{GL}(n, K)$は$G$のクローズド部分群、$G$は$\mathbf{GL}(n, K)$と$T = K^n$のセミダイレクト積です。 1 つは、$G$ に (局所的にコンパクトな) 位相を装備しており、その$G$ は、$\mathbf{GL}(n, K)$ と $T$ (GT、III, §2, No. 10) のトポロジカル半直接積です。 1つは持っています
$$
(X, x) = (1, x) \cdot (X, 0).
$$
一方、$X \in \mathbf{GL}(n, K)$ と $x \in T$ の場合、$\xi \in K^n$ ごとに、
$$
(X, 0)(1, x)(X, 0)^{-1}\xi = X(X^{-1}\xi + x) = \xi + Xx = (1, Xx)\xi,
$$
したがって、$T$ の自己同型 $(1, x) \mapsto (X, 0)(1, x)(X, 0)^{-1}$ は法$\mod(\det X)$ を持ちます (§1, No. 10、提案 15)。 例 1 と §2, No. 9、*注意* を考慮すると、この措置は
$$
(5) \quad \mod(\det X)^{-n-1} \cdot \left( \bigotimes_{ij} dx_{ij} \right) \otimes \left( \bigotimes_i dx_i \right) \qquad (X = (x_{ij}), \ x = (x_i))
$$
$G$の左ハール対策です。一方、§2, No. 9の提案14により、
$$
\Delta_G((X, x)) = \Delta_{\mathbf{GL}(n, K)}(X) \Delta_{K^n}(x) (\mod \det X)^{-1},
$$
または
$$
(6) \quad \Delta_G((X, x)) = \mod(\det X^{-1}).
$$

したがって、$G$ における正しいハール測度は次のように与えられます。

$$
(\mod \det X)^{-n} \cdot \left( \bigotimes_{ij} dx_{ij} \right) \otimes \left( \bigotimes_i dx_i \right).
$$

#### 例 3 {#int-vii-s3-n3-exa-3 .statement tag=09H7}

**厳密な三角形群.**

$[1, n]$ を整数 $m$ の集合として、$1 \leq m \leq n$ とします。 $J$ を、次の条件の $[1, n] \times [1, n]$ 満たすの部分集合とします。
1) $(i, j) \in J$ の場合、$i < j$;
2) $(i, j) \notin J$ の場合、$i < k < j$ の 2 つの対 $(i, k)$ と $(k, j)$ のうちの少なくとも 1 つが属するから $J$ にならないように、整数 $k$ ごとに。

$T_J$ を行列 $Z = (z_{ij})_{1 \leq i \leq n, 1 \leq j \leq n}$ の集合とし、$K$ に元を加え、$i \neq j$ と $(i, j) \notin J$ の場合は $z_{ii} = 1$ 、$z_{ij} = 0$ とします。こちらは$\mathbf{GL}(n, K)$の部分集合が閉店です。 写像 $Z \mapsto (z_{ij})_{(i, j) \in J}$ は、$T_J$ の $K^s$ への同型写像です ($s$ は、$J$ の元の数を表します)。 $Z' = (z'_{ij}) \in T_J$の場合、$Z'Z = (z''_{ij})$

$$
z''_{ij} = z_{ij} + z'_{ij} + \sum_{i < h < j} z'_{ih} z_{hj} \quad \text{for } i < j,
$$
$$
z''_{ij} = 0 \text{ for } i > j, \quad z''_{ii} = 1,
$$

よって $Z'Z \in T_J$。 $T_J$ が $K^s$ と同一視される場合、写像 $Z \mapsto Z'Z$ (固定 $Z'$ の場合) はアフィン写像と同一視され、対 $(i, j) \in J$ を辞書編集的に並べ替えることでわかるように、その行列式は 1 になります。 適用次の補題:

#### 補題 6 {#int-vii-s3-lem-6 .statement tag=09H8}

** $L$ を完全に順序付けられた有限の集合とします。すべての $\lambda \in L$ について、$V_\lambda$ を可換環 $k$ 上の有限次元の自由加群とします。 $L$ の $\lambda, \mu$ に対して、$\lambda \leq \mu$ は $f_{\lambda \mu} \in \mathrm{Hom}_k(V_\mu, V_\lambda)$ とします。それから線形写像
$$
(v_\lambda)_{\lambda \in L} \mapsto \left( \sum_{\mu \geq \lambda} f_{\lambda \mu}(v_\mu) \right)_{\lambda \in L},
$$
$\prod_{\lambda \in L} V_\lambda$ から $\prod_{\lambda \in L} V_\lambda$ まで、行列式 $\prod_{\lambda \in L} \det f_{\lambda \lambda}$ があります。

$L$ が整数の区間である場合に 1 つの簡約するがすぐに続き、A、III, §8, No. 6、公式から補題が続きます (31)。

$Z \in T_J$ の場合、$Z'Z = I_n$、よって $Z' = Z^{-1}$ のような $Z' \in T_J$ が存在することがわかります。したがって、$T_J$ は、$\mathbf{GL}(n, K)$ の閉じた部分群です。一方、§1, No. 10の提案15は、この措置が

$$
\bigotimes_{(i, j) \in J} dz_{ij}
$$

は$T_J$の左ハールメジャーです。 $ZZ'$ を計算すると、この測定値が $T_J$ における正しい Haar 測定値であることが同じようにわかります。

$T_J$ の定義で、行と列の役割が交換された場合にも、同様の結果が得られます。

When $J$ is the set of pairs $(i, j)$ such that $i < j$, the group $T_J$ is called the *upper strict triangular group* of order $n$ over $K$, and is denoted $T_1(n, K)$. その転置は *下限厳密三角形群* と呼ばれます。

#### 例 4 {#int-vii-s3-n3-exa-4 .statement tag=09H9}

— *大きな三角形群.*

$n_1, \ldots, n_r$ を整数 $\geqslant 1$ とします。 集合 $p_k = n_1 + \ldots + n_{k-1}$ と $n = p_{r+1} = n_1 + \cdots + n_r$。 $I_k$ を整数 $j$ の集合として、$p_k < j \leqslant p_{k+1}$、$k < l$ の $I_k \times I_l$ の $J$ 和集合とします。 $G$ を、元が行列 $(Z_{kl})_{1 \leqslant k \leqslant r, 1 \leqslant l \leqslant r}$ である $\mathbf{GL}(n, K)$ の閉じた部分群とします。
1) それぞれの $Z_{kl}$ は、$n_k$ 行と $n_l$ 列からなる $K$ の元の行列 $(z_{ij})_{i \in I_k, j \in I_l}$ です。
2) $k > l$ の場合は $Z_{kl} = 0$;
3) $1 \leqslant k \leqslant r$ の場合は $Z_{kk} \in \mathbf{GL}(n_k, K)$。

ブロック乗法に対して公式

$$
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
\begin{pmatrix}
1 & Z_{12} & \ldots & Z_{1r} \\
0 & 1 & \ldots & Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & 1
\end{pmatrix}
$$

$$
= \begin{pmatrix}
Z_{11} & Z_{11}Z_{12} & \ldots & Z_{11}Z_{1r} \\
0 & Z_{22} & \ldots & Z_{22}Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
$$

は、$G$ が部分群 $D$ 元 $(Z_{kl}) \in G$ のトポロジカル半直接積であり、 $k \neq l$ の $Z_{kl} = 0$ および例 3 の部分群 $T_J$ であることを示しています。 $D$ は、$1 \leqslant k \leqslant r$ に対する群 $\mathbf{GL}(n_k, K)$ の直接の積と同型です。

$J'$ を $(i, j) \in J$ の対 $(j, i)$ の集合とし、$H$ を所属 ～ $J'$ ではなく、対 $(i, j) \in [1, n] \times [1, n]$ の集合とします。 $Z' = (z_{ij})_{1 \leqslant i \leqslant n, 1 \leqslant j \leqslant n}$を$G$の元とします。 §2, No. 9 の提案 14 と上記の例 1 および 3 により、像の測度を取得することにより、$G$ の左ハール測度が得られます。

$$
\bigotimes_{k=1}^r ((\mathrm{mod}\ \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij}) \otimes \left( \bigotimes_{(i,j) \in J} dz_{ij} \right)
$$

写像未満

$$
((Z_{kk}), (Z_{kl})) \mapsto \begin{pmatrix}
Z_{11} & Z_{11}Z_{12} & \ldots & Z_{11}Z_{1r} \\
0 & Z_{22} & \ldots & Z_{22}Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}.
$$

さて、$k < l$、行列 $Z_{kl} = (z_{ij})_{i \in I_k, j \in I_l}$ のベクトル空間について考えてみましょう。 $h \neq j$ に対して $z_{ih} = 0$ となるように、行列によって形成された $n_l$ 部分空間 $M_j$ ($j \in I_l$) の直和です。これら部分空間 $M_j$ はそれぞれ写像 $Z_{kl} \mapsto Z_{kk}Z_{kl}$ で安定しており、この写像 ～ $M_j$ のうち制限には行列 $Z_{kk}$ が存在します。その結果、(§ 1, No. 10、提案 15) 写像 $Z_{kl} \mapsto Z_{kk}Z_{kl}$ に基づく尺度 $\bigotimes_{i \in I_k, j \in I_l} dz_{ij}$ の像は次のようになります。

$$
(\operatorname{mod} \det Z_{kk})^{-n_l} \cdot \bigotimes_{i \in I_k, j \in I_l} dz_{ij}.
$$

従って、$G$ における左ハール測度は次のように与えられます。

$$
\prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{-q_k} \cdot \bigotimes_{(i,j) \in H} dz_{ij}
$$

$q_k = \sum_{k \leq l \leq r} n_l = n - p_k$と。

再び§ 2の提案14を使用して、$G$の*係数*を計算するにしてみましょう。 群 $D$ と $T_J$ はユニモジュラーです。一方:

$$
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}
\begin{pmatrix}
1 & Z_{12} & \ldots & Z_{1r} \\
0 & 1 & \ldots & Z_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & 1
\end{pmatrix}
\begin{pmatrix}
Z_{11} & 0 & \ldots & 0 \\
0 & Z_{22} & \ldots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & Z_{rr}
\end{pmatrix}^{-1}
$$
$$
= \begin{pmatrix}
1 & Z'_{12} & \ldots & Z'_{1r} \\
0 & 1 & \ldots & Z'_{2r} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \ldots & 1
\end{pmatrix},
$$

$Z'_{kl} = Z_{kk}Z_{kl}Z_{ll}^{-1}$ です。 例 3 と § 1, No. 10 の提案 15 を考慮し、上記のように議論すると、$X = \operatorname{diag}(Z_{11}, \ldots, Z_{rr}) \in D$ の場合、$T_J$ の自己同型 $Z \mapsto X^{-1}ZX$ の係数は次のようになります。

$$
\prod_{k < l} (\operatorname{mod} \det Z_{kk})^{-n_l} (\operatorname{mod} \det Z_{ll})^{n_k},
$$

したがって

$$
\Delta_G(Z) = \prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{n+n_k-2q_k}.
$$

$G$ の転置された群 $G'$ も同様に検討されます。 $G'$ については、左のハール測度として求められます。

$$
\prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{-p_{k+1}} \cdot \bigotimes_{(j,i) \in H} dz_{ij},
$$

そして係数として

$$
\prod_{k=1}^r (\operatorname{mod} \det Z_{kk})^{n+n_k-2p_{k+1}}.
$$

特に$n_1 = \ldots = n_r = 1$を取ると、行列$X = (x_{ij})$によって形成される可逆元の部分代数の$M_n(K)$の群$G$群$T(n, K)^*$として、$x_{ij} = 0$が成り立つことがわかります。 $i > j$。この代数を $T(n, K)$ と表記しますが、*上三角代数* と呼ばれ、群 $T(n, K)^*$ は $K$ 上の位数 $n$ の *上大三角群* と呼ばれます。前の公式から次の形を取得します。 $T(n, K)^*$ の左ハール測度は次のようになります。

$$(9\ bis)$$
$$
\prod_{i=1}^n (\operatorname{mod} z_{ii})^{i-n-1} \cdot \bigotimes_{i \leq j} dz_{ij} \quad (Z = (z_{ij}))
$$

$T(n, K)^*$ の係数は

$$(10\ bis)$$
$$
\Delta_{T(n,K)^*}(Z) = \prod_{i=1}^n (\operatorname{mod} z_{ii})^{2i-n-1} \quad (Z = (z_{ij})).
$$

$T(n, K)^*$ の転置、または *下側の大きな三角形群* については、左ハール測度として求められます。

$$
\prod_{i=1}^n (\operatorname{mod} z_{ii})^{-i} \cdot \bigotimes_{i \geq j} dz_{ij},
$$

そして係数として

$$
\prod_{i=1}^n (\operatorname{mod} z_{ii})^{n+1-2i}.
$$

#### 注意 {#int-vii-s3-n3-rem-1 .statement tag=09HA}

群 $T(n, K)^*$ は、$\mathbf{GL}(n, K)$ と $\Delta_{T(n, K)^*}((z_{ij})) = \prod_{i=1}^n (\operatorname{mod} z_{ii})^{2i-n-1}$ のクローズド部分群です。 例 1 で $\Delta_{\mathbf{GL}(n, K)} = 1$ を見ました。 $n > 1$、写像の場合
$$
\Delta_{T(n, K)^*}/\Delta_{\mathbf{GL}(n, K)}
$$
$T(n, K)^*$ できないは、$\mathbf{C}^*$ の $\mathbf{GL}(n, K)$ の連続表現に拡張されます (そのような表現は、補題 5 により $\mathbf{SL}(n, K)$ では 1 に等しくなりますが、$z_{11}$ では $\operatorname{mod}(z_{11})^{1-n} \neq 1$ が適切です選ばれました）。したがって、同次空間 $\mathbf{GL}(n, K)/T(n, K)^*$ は、$n > 1$ (§ 2, No. 6、Th. 3 の Cor. 1) の場合 *比較的不変の測度を認めない* ということになります。

この均一な空間は、$n = 2$ に関して、$K$ 上の *射影線* で識別される可能性があります。というのは、$(e_1, e_2)$を$K^2$の標準基底とします。 群 $\mathbf{GL}(2, K)$ は、$K^2$ の集合に対して 0 を省略して推移的に動作し、$Ke_1 - \{0\}$ の固定群は$T(2, K)^*$ になります。

#### 例 5 {#int-vii-s3-n3-exa-5 .statement tag=09HB}

— *特別な三角群.*
例 4 の冒頭の記法を再度取り上げ、部分群 $G_1 = G \cap \mathbf{SL}(n, K)$ を考えてみましょう。この部分群は、群 $D_1 = D \cap \mathbf{SL}(n, K)$ と $T_J$ の位相的半直接積です。 群 $D_1$ は、$\mathbf{SL}(n_r, K)$ と同型の正規の部分群 $A$ を持っています。つまり、元 $\operatorname{diag}(Z_{kk})$ の部分群からなると、$k < r$ の $Z_{kk} = 1$ です。 準同型
$$
\varphi : \operatorname{diag}(Z_{11}, \ldots, Z_{rr}) \mapsto (Z_{11}, \ldots, Z_{r-1, r-1})
$$
$D_1$ から $\mathbf{GL}(n_1, K) \times \cdots \times \mathbf{GL}(n_{r-1}, K)$ は全射法で、核 $A$ になります。一方、$\varphi$は連続です。 付録 I の補題 2 を考慮すると、$D_1/A$ は $\mathbf{GL}(n_1, K) \times \cdots \times \mathbf{GL}(n_{r-1}, K)$ と識別される可能性があります。 $A$ (cf. 例 6) のハール測度を $\mu$ で表します。
$$
\alpha = \bigotimes_{k=1}^{r-1} \left( (\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij} \right) \otimes' d\mu(Z_{rr})
$$
$D_1$ のハール測度は次のようになります
$$
\alpha/\mu = \bigotimes_{k=1}^{r-1} \left( (\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij} \right)
$$
(§ 2, No. 7、提案 10)。次に、例 4 のように、$G_1$ の左ハール測度が次の式で与えられることがわかります。
$$
\operatorname{mod} \left( \prod_{k=1}^{r-1} (\det Z_{kk})^{n_k-q_k} \right)
$$
$$
\cdot \left[ \bigotimes_{k=1}^{r-1} ((\operatorname{mod} \det Z_{kk})^{-n_k} \cdot \bigotimes_{i,j \in I_k} dz_{ij}) \otimes' d\mu(Z_{rr}) \right] \otimes \bigotimes_{(i,j) \in J} dz_{ij}.
$$

$G$では$G_1$が正規であるため、$G_1$の*係数*は$G$の*係数*の制限になります(§ 2, No. 7、提案10 b))。

$n_r = 1$、部分群 $A$ 簡約するからニュートラル元、そして$G$ の左ハール測定は次のようになります。

$$
\operatorname{mod}\left( \prod_{k=1}^{r-1} (\det Z_{kk})^{-q_k} \right) \cdot \bigotimes_{k=1}^{r-1} \left( \bigotimes_{i,j \in I_k} dz_{ij} \right) \otimes \bigotimes_{(i,j) \in J} dz_{ij}.
$$

$n_1 = n_2 = \ldots = n_r = 1$ をとった場合、得られる群 $G_1$ は *上特殊三角形群* と呼ばれ、その転置 $G'_1$ は *下特殊三角形群* と呼ばれます。 $G_1$ の左ハール測度は次のとおりです。

$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{i-n-1} \right) \cdot \left( \bigotimes_{i=1}^{n-1} dz_{ii} \right) \otimes \left( \bigotimes_{1 \leq i < j \leq n} dz_{ij} \right)
$$
$G_1$ の係数は
$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{2i-2n} \right).
$$
$G'_1$ については、同様に左ハール測度を見つけます。
$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{n-i-1} \right) \cdot \left( \bigotimes_{i=1}^{n-1} dz_{ii} \right) \otimes \left( \bigotimes_{1 \leq j < i \leq n} dz_{ij} \right)
$$
と弾性率
$$
\operatorname{mod} \left( \prod_{i=1}^{n-1} z_{ii}^{2n-2i} \right).
$$

#### 例 6 {#int-vii-s3-n3-exa-6 .statement tag=09HC}

— *特殊リニア群.*
$\mathbf{GL}(n, K)$ の閉じた部分群 $T_1(n, K)$ と ${}^t(T(n, K)^*)$ には共通部分 $\{e\}$ があります。したがって、写像 $(M, N) \mapsto M \cdot N$ は、$T_1(n, K) \times {}^t(T(n, K)^*)$ の全単射 $\varphi$ から $\mathbf{GL}(n, K)$ の部分集合 $\Omega$ への連続です。

#### 補題 7 {#int-vii-s3-lem-7 .statement tag=09HD}

— a) *$U = (u_{ij}) \in \mathbf{GL}(n, K)$としましょう。 $U \in \Omega$の位数では、$k = 2, 3, \ldots, n$に対して$\det(u_{ij})_{k \leq i, j \leq n} \neq 0$が必要十分です*。
b) $\Omega$ * は $\mathbf{GL}(n, K)$* のオープン部分集合です。
c) *写像 $\varphi$ は、$T_1(n, K) \times {}^t(T(n, K)^*)$ の $\Omega$* への同写写像です。

$U \in \Omega$ である位数では、$ZU \in {}^t(T(n, K))$ となるような $Z = (z_{ij}) \in T_1(n, K)$ が存在することが必要かつ十分です (したがって必然的に

$U$ と $Z$ は反転可能なため、$ZU \in {}^t(T(n, K)^*)$)。先ほど見たことから、$Z$ が存在する場合、それは一意です。したがって、位数の $U \in \Omega$ では、線形系が必要かつ十分です。

$$
\sum_{k=1}^n z_{ik} u_{kj} = 0 \qquad (1 \leq i < j \leq n)
$$

($(z_{ij}) \in T_1(n, K)$) は一意の解を認めます。さて、この系は次のように書くことができます

$$
(13) \qquad \sum_{k=i+1}^n z_{ik} u_{kj} = -u_{ij} \qquad (1 \leq i < j \leq n).
$$

固定 $i$ の場合、未知数 $z_{i,i+1}, z_{i,i+2}, \ldots, z_{i,n}$ には $n-i$ 方程式のうち系が存在します。これら系が独自の解を認めるためには、次のことが必要かつ十分です。

$$
\det(u_{kj})_{i+1 \leq k \leq n,\ i+1 \leq j \leq n} \neq 0
$$

$i = 1, 2, \ldots, n-1$の場合。これは a) を証明します。このことから、$\Omega$ は $\mathbf{GL}(n, K)$ にオープンしていることがわかります。一方、クラマーの公式を用いて系 (13)を解くと、$\Omega$の分母が非零である$u_{ij}$の有理写像として$z_{ij}$が得られるため、$Z$は連続的に$U$に依存します。 $\Omega$、これは c) を証明します。

ここで、$G'_1 \subset {}^t(T(n, K)^*)$ を特別な下三角群とします。 写像 $(M, N) \mapsto M \cdot N$ は、$T_1(n, K) \times G'_1$ の全単射 $\psi$ から $\mathbf{SL}(n, K)$ の部分集合 $\Omega'$ への連続です。

#### 補題 8 {#int-vii-s3-lem-8 .statement tag=09HE}

**a)** *$U = (u_{ij}) \in \mathbf{SL}(n, K)$ としましょう。 $U \in \Omega'$の位数において、$k = 2, 3, \ldots, n$に対して$\det(u_{ij})_{k \leq i, j \leq n} \neq 0$があれば必要十分です。

b) $\Omega'$ * は $\mathbf{SL}(n, K)$* のオープン部分集合です。

c) *写像 $\psi$ は、$\Omega'$* に対する $T_1(n, K) \times G'_1$ の同型写像です。

$M \in T_1(n, K)$ と $N \in {}^t(T(n, K)^*)$ としましょう。 $M \cdot N \in \mathbf{SL}(n, K)$の位数では、$N \in G'_1$があれば必要十分です。したがって、補題 7 から $\Omega' = \mathbf{SL}(n, K) \cap \Omega$ と補題 8 がすぐに続きます。

#### 命題 6 {#int-vii-s3-prop-6 .statement tag=09HF}

**a)** *群 $\mathbf{SL}(n, K)$ はユニモジュラーです。*

b) *$\mu_1$ と $\mu_2$ をそれぞれ、上の厳密な三角形群 $T_1(n, K)$ と下の特別な三角形群 $G'_1$ のハール測度としておきます。 $\Omega'$ への $T_1(n, K) \times G'_1$ の同型写像 $(M, N) \mapsto M \cdot N^{-1}$ の下での $\mu_1 \otimes \mu_2$ の像は、$\mathbf{SL}(n, K)$* 上のハール測度の制限から $\Omega'$ です。

c) *$\mathbf{SL}(n, K)$ の $\Omega'$ の補数は、$\mathbf{SL}(n, K)$* のハール測度では無視できます。

群 $\mathbf{GL}(n, K)$ はユニモジュラー (例 1)、$\mathbf{SL}(n, K)$ は $\mathbf{GL}(n, K)$ の通常の部分群であるため、ユニモジュラーです (§ 2, No. 7、提案 10 b))。 主張 b) は、a)、補題 8、および§ 2, No. 9 の提案 13 から続きます。 c)を証明しましょう。 補題 8 a) までに、次のことを証明すれば十分です: $p((u_{ij})_{1 \leq i,j \leq n})$ が多項式であり、$\mathbf{SL}(n, K)$ 上の零と同じではない場合、$p(U) = 0$ がハール測度にとって無視できるような $U \in \mathbf{SL}(n, K)$ の集合 E です。 § 1, No. 10 を考慮すると、Cor。提案 13 の $\mathbf{SL}(n, K)$ の位相には可算な基底があります。したがって、すべての $U_0 \in E$ について、$\mathbf{SL}(n, K)$ に $U_0$ の近傍が存在し、その共通部分と E は無視できることを証明すれば十分です。または、再度、$U_0^{-1}E \cap W$ が無視できるように、$\mathbf{SL}(n, K)$ にI の近傍 W が存在します。 $W = \Omega'$ を見てみましょう。 b) を考慮すると、結局のところ、$p(U_0 MN) = 0$ は $\mu_1 \otimes \mu_2$ にとって無視できるほど、対 $(M, N) \in T_1(n, K) \times G'_1$ の集合が示されることになります。 $\mu_1$ と $\mu_2$ の式 (例 3 と 5 で計算) により、これは次の補題の結果となります。

#### 補題 9 {#int-vii-s3-lem-9 .statement tag=09HG}

*$\psi$を$K[X_1, \ldots, X_r]$の多項式$\neq 0$とします。 空間 $K^r$ では、$\psi(x_1, \ldots, x_r) = 0$ によって定義される集合 N はハール測度では無視できます。*

$r$の帰納法までに議論しましょう。 $r = 1$ については、N が有限の集合であるため、補題は明らかです。必要に応じて変数の番号付けを変更すると、$\psi \notin K[X_1, \ldots, X_{r-1}]$ と仮定できます。書く

$$
\psi(X_1, \ldots, X_r) = X_r^m \psi_0(X_1, \ldots, X_{r-1}) + \cdots + \psi_m(X_1, \ldots, X_{r-1})
$$

$m > 0$ と $\psi_0 \neq 0$ です。 空間 $K^{r-1}$ では、$N_0$ を $\psi_0(x_1, \ldots, x_{r-1}) = 0$ によって定義される集合とします。これは、帰納法の仮定によって無視できます。 $(x_1, \ldots, x_{r-1}, x_r) \in N$ が有限であるため、$x_r \in K$ のすべての $(x_1, \ldots, x_{r-1}) \notin N_0$、集合について、無視できます。 $K^r$ は無限大で可算であるため (§ 1, No. 10、提案 13 の修正)、$N \cap [(K^{r-1} - N_0) \times K]$ は $K^r$ では無視できます (Ch. V, § 8, No. 2、提案 4)。したがって、N は無視できます。

#### 例 7 {#int-vii-s3-n3-exa-7 .statement tag=09HH}

*岩沢分解/$\mathbf{GL}(n, K)$.*

この例において、Kは体$\mathbf{R}, \mathbf{C}, \mathbf{H}$のいずれかを表します。 $\lambda \in K$の場合、$\overline{\lambda}$は、$K = \mathbf{R}$の場合は$\lambda$、$K = \mathbf{C}$または$\mathbf{H}$の場合は$\lambda$の共役と等しいと定義されます。 E を次元 $n$ の K 上の右ベクトル空間とし、$\Phi$ を E 上の非縮退正のエルミート形とします。

#### 補題 10 {#int-vii-s3-lem-10 .statement tag=09HI}

*$(f_1, f_2, \ldots, f_n)$をEの基底とします。*
a) *すべての $i$ に対して $\alpha_{ii} > 0$ を持つ $f_i = e_1 \alpha_{i1} + e_2 \alpha_{i2} + \cdots + e_i \alpha_{ii}$ ($i = 1, 2, \ldots, n$) となるような E の正規直交関数基底 $(e_1, e_2, \ldots, e_n)$ が 1 つだけ存在します。
b) *固定$\Phi$の場合、$e_i$と$\alpha_{ij}$は継続的に$(f_1, \ldots, f_n) \in E^n$に依存します。*

次元 $i$ を持つ $E_i = f_1 K + f_2 K + \cdots + f_i K$ とします。 $g_i$ を $E_{i-1}$ に直交する $E_i$ の非零元とし、$\Phi(g_i, g_i) = 1$ とする。 $i$ の帰納法により、$(g_1, \ldots, g_i)$ が $E_i$ の正規直交基底であることがわかります。特に、$(g_1, \ldots, g_n)$ は $E$ の正規直交基底です。 $\lambda_i = \Phi(f_i, g_i)$ にしましょう。 $f_i \notin E_{i-1}$ 以降、1 つは $\lambda_i \neq 0$ になります。 集合 $e_i = g_i |\lambda_i| \lambda_i^{-1}$。それから

$$
\Phi(e_i, e_i) = |\lambda_i|^2 \overline{\lambda_i}^{-1} \Phi(g_i, g_i) \lambda_i^{-1} = 1,
$$

したがって、$(e_1, \ldots, e_i)$ は $E_i$ の正規直交基底でもあります。さらに、$\Phi(e_i, f_i) = |\lambda_i| \overline{\lambda_i}^{-1} \Phi(g_i, f_i) = |\lambda_i| > 0$、したがって、$e_i$ は a) の特性を持ちます。 $(e'_1, \ldots, e'_n)$ を、同じ特性を持つ $E$ の他の正規直交基底とします。 $i$ の帰納法までに、$(e'_1, \ldots, e'_i)$ は $E_i$ の基底である必要があることがわかり、したがって、一部の $\mu_i \in \mathbf{K}$ では $e'_i = e_i \mu_i$ になります。それから

$$
1 = \Phi(e'_i, e'_i) = \overline{\mu_i} \Phi(e_i, e_i) \mu_i = \overline{\mu_i} \mu_i ,
$$

および$0 < \Phi(e'_i, f_i) = \overline{\mu_i} \Phi(e_i, f_i)$、したがって$\mu_i > 0$および$\mu_i^2 = 1$、したがって$\mu_i = 1$、よって a) $e_i$ と $\alpha_{ij}$ が $i < i_0$ について $(f_1, \ldots, f_n)$ に継続的に依存していることがすでに証明されているとします。そして、$e_{i_0}$ と $\alpha_{i_0 j}$ が継続的に $(f_1, \ldots, f_n)$ に依存していることを証明しましょう。 $j < i_0$ の場合、$\overline{\alpha}_{i_0 j} = \Phi(f_{i_0}, e_j)$ は継続的に帰納法の仮定によって $(f_1, \ldots, f_n)$ に依存します。一方、

$$
\Phi(f_{i_0}, f_{i_0}) = |\alpha_{i_0 1}|^2 + |\alpha_{i_0 2}|^2 + \cdots + |\alpha_{i_0, i_0 - 1}|^2 + \alpha_{i_0 i_0}^2 ,
$$

したがって、$\alpha_{i_0 i_0}$ は継続的に $(f_1, \ldots, f_n)$ に依存します。したがって、

$$
e_{i_0} = (f_{i_0} - e_1 \alpha_{i_0 1} - \cdots - e_{i_0 - 1} \alpha_{i_0, i_0 - 1}) \alpha_{i_0 i_0}^{-1}
$$

継続的に$(f_1, \ldots, f_n)$に依存します。

以降、$E = K^n$ とし、$\Phi$ 形とします

$$
\overline{x}_1 y_1 + \cdots + \overline{x}_n y_n .
$$

$\mathbf{U}(n, \mathbf{K})$ は対応するユニタリ群を表すことを思い出してください。 $\mathbf{K}$ が非可換である場合でも、対角要素がすべて 1 である $\mathbf{M}_n(\mathbf{K})$ の上三角行列の $\mathbf{T}_1(n, \mathbf{K})$ 群で再度表します。

#### 命題 7 {#int-vii-s3-prop-7 .statement tag=09HJ}

*$D_+^*$を対角線行列と対角線元$> 0$の群とします。 写像 $(U, D, T) \mapsto UDT$ は、$\mathbf{U}(n, \mathbf{K}) \times D_+^* \times \mathbf{T}_1(n, \mathbf{K})$ の $\mathbf{GL}(n, \mathbf{K})$ への準同型写像です。*

$(\varepsilon_1, \ldots, \varepsilon_n)$を$K^n$の標準基底とします。 $X \in \mathbf{GL}(n, K)$ にしましょう。次に、E の $X \cdot \varepsilon_i = f_i$ 形基底。これに基底 $(f_i)$ に、補題 10 のように基底 $(e_i)$ を関連付けることができます。$U$ をユニタリ自己同型の行列とします。 E の変換 $\varepsilon_i$ を $e_i$ にします。それから

$$
U^{-1} \cdot f_i = \varepsilon_1 \alpha_{i1} + \varepsilon_2 \alpha_{i2} + \cdots + \varepsilon_i \alpha_{ii}
$$

$\alpha_{ii} > 0$ は $i = 1, 2, \ldots, n$ です。したがって、$X = UC$、$C$ は行列

$$
\begin{pmatrix}
\alpha_{11} & \alpha_{21} & \cdots & \alpha_{n1} \\
0 & \alpha_{22} & \cdots & \alpha_{n2} \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & \alpha_{nn}
\end{pmatrix}.
$$

さらに、$U$ と $C$ は補題 10 によって X に継続的に依存します。 一方、公式 (8) は、$C$ に継続的に依存して、$D \in \mathbf{D}_+^*$、$T \in \mathbf{T}_1(n, K)$、$D$、$T$ により、$C$ が形 $DT$ に入れられる可能性があることを示しています。 分解 $X = UDT$ の一意性は、補題 10 の一意性性質から続きます。

提案 7 の準同型性は、$\mathbf{GL}(n, K)$ の *Iwasou 分解* と呼ばれます。

群 $G = \mathbf{D}_+^* \cdot \mathbf{T}_1(n, K)$ は、対角線元が $> 0$ である K 上の上三角行列の集合です。この群の元 $(z_{ij})$ を元と同一視しましょう

$$
((z_{ii})_{1 \leq i \leq n}, (z_{ij})_{1 \leq i < j \leq n}) \in (\mathbf{R}_+^*)^n \times K^{n(n-1)/2}.
$$

例 4 とまったく同じように議論すると、この群の尺度 ($K = \mathbf{R}$ のとき) について *正しい* ハール尺度が得られます。

$$
\left( \prod_{i=1}^n z_{ii}^{-i} \right) \cdot \left( \bigotimes_{i=1}^n dz_{ii} \right) \otimes \left( \bigotimes_{i < j} dz_{ij} \right).
$$

次に、§2, No. 9 の適用提案 13 により、$\mathbf{GL}(n, K)$ が写像 $(U, S) \mapsto US$ によって $\mathbf{U}(n, K) \times G$ と同一視される場合、$\mathbf{GL}(n, K)$ のハール測度は ($K = \mathbf{R}$ のとき) によって与えられることがわかります。

$$
\left( \prod_{i=1}^n z_{ii}^{-i} \right) \cdot \alpha \otimes \left( \bigotimes_{i=1}^n dz_{ii} \right) \otimes \left( \bigotimes_{i < n} dz_{ij} \right),
$$

ここで、$\alpha$ は $\mathbf{U}(n, K)$ の Haar 測定値を表します。

#### 例 8 {#int-vii-s3-n3-exa-8 .statement tag=09HK}

エルミート形の空間。

この例において、Kは常に体$\mathbf{R}, \mathbf{C}, \mathbf{H}$のいずれかを表します。 $\delta = \dim_{\mathbf{R}} K$ (つまり $\delta = 1, 2$ または 4) と書きます。 右ベクトル空間 $K^n$ にエルミート形 $\Phi$ が書かれる場合があります

$$
\Phi(x, y) = \Phi(x_1, \ldots, x_n, y_1, \ldots, y_n) = \sum_{i,j=1}^n \overline{x_i} h_{ij} y_j
$$

$i$ と $j$ のすべてに $h_{ij} = \overline{h_{ji}}$ が付きます。 $M_n(K)$ のエルミート行列によって形成される $\mathbf{R}$ を $\mathfrak{H}$ ベクトル空間で表します。 写像 $(h_{ij}) \mapsto \Phi$ は、$K^n$ の $\mathfrak{H}$ のベクトル空間とエルミート形の同型であり、これにより、これら 2 つの空間を同一視するにすることになります。 $\mathfrak{H}_+^* \subset \mathfrak{H}$ を $K^n$ 上の非退化陽性エルミート形の集合とします。 集合 $\mathfrak{H}_+^*$ は $\mathfrak{H}$ に *凸* です。なぜなら、$\Phi_1, \Phi_2$ が $\mathfrak{H}_+^*$ にあり、$\lambda, \mu$ が 2 つの数 $> 0$ で、$\lambda + \mu = 1$ である場合、$\lambda \Phi_1 + \mu \Phi_2$ が正のエルミート形であることは明らかです。一方、$(\lambda \Phi_1 + \mu \Phi_2)(x, x) = 0$ の場合、$\Phi_1(x, x) = \Phi_2(x, x) = 0$、したがって $x = 0$ となり、$\lambda \Phi_1 + \mu \Phi_2$ は非縮退となります。 ここで、$\mathfrak{H}_+^*$ が $\mathfrak{H}$ の *オープン* 部分集合であることを示しましょう。 S を $x_1 \overline{x}_1 + \cdots + x_n \overline{x}_n = 1$ となるような $x = (x_1, \ldots, x_n) \in K^n$ の集合とします。これは$K^n$のコンパクトな部分集合です。 $\Phi \in \mathfrak{H}_+^*$、写像 $x \mapsto \Phi(x, x)$ が連続で、S 上で $> 0$ の場合、その下限は $> 0$ です。 $\Phi' \in \mathfrak{H}$ が $\Phi$ に十分近い場合、すべての $x \in S$ について $\Phi'(x, x) > 0$ となり、$\Phi'$ は正で非縮退となります。

一般的な線形群 $\mathbf{GL}(n, K)$ は、$\mathfrak{H}$ $(X, \Phi) \mapsto \Phi \circ X$、つまり $(X, H) \mapsto t \overline{X} \cdot H \cdot X$ で右側に連続的に動作します。ここで、$H$ はエルミート行列対応するから $\Phi$ を表します。 $\mathfrak{H}_+^*$ が $\mathbf{GL}(n, K)$ の下で安定していることは明らかです。より正確には、*Alg.*、Ch. IX, §6, No. 1、コル。 Thの1 1,$^1$ $\mathfrak{H}_+^*$ は、形 $\sum_{i=1}^n \overline{x_i} y_i$ 対応するの $\mathbf{GL}(n, K)$ の下にある軌道であり、同一性行列 $I_n$ です。この形の固定群は$\mathbf{U}(n, K)$です。アプリの補題 2 までに。 I、$\mathfrak{H}_+^*$ は、$\mathbf{GL}(n, K)/\mathbf{U}(n, K)$ と位相的に同次の空間として識別される可能性があります。

すべての $X \in \mathbf{GL}(n, K)$ について、$\widetilde{X}$ を *実数* ベクトル空間 $\mathfrak{H}$ の自己同型 $H \mapsto t \overline{X} \cdot H \cdot X$ とします。 $\mu$ が加法群 $\mathfrak{H}$ のハール測度を表す場合、$\widetilde{X}^{-1}(\mu) = |\det \widetilde{X}| \cdot \mu$ になります (§ 1, No. 10、提案 15 の Cor. 1)。それを見せてみましょう

$$
| \det \widetilde{X} | = | N(X) |^\lambda ,
$$

ここで、N は $M_n(K)$ *$\mathbf{R}\text{-algebra}$ とみなされる* のノルムを表し、$\lambda = 1 - \frac{\delta - 2}{\delta n}$ を表します。 系を超える $X$ について (15) を検証するだけで十分です。

(1) 参照。 TVS、V, §2, No. 4、Cor. Thの1 2.

$\mathbf{GL}(n, K)$ の生成元、従って、次の型の $X$ については (A、II, §10, No. 13、提案 14 の Cor. 2):

a) $X$ は形の写像の行列です
$$
(x_1, \ldots, x_n) \mapsto (x_{\sigma(1)}, \ldots, x_{\sigma(n)}),
$$
どこ$\sigma \in \mathfrak{S}_n$。この場合、$X$ の冪は 1 に等しいため、$|\det \widetilde{X}| = |N(X)| = 1$ になります。

b) $X$ は形の写像の行列です
$$
(x_1, \ldots, x_n) \mapsto (ax_1, x_2, \ldots, x_n).
$$
次に、$(h_{ij}) \in \mathfrak{H}$の場合、$h'_{11} = \overline{a} h_{11} a = |a|^2 h_{11}$と$\widetilde{X}((h_{ij})) = (h'_{ij})$、$i > 1$の場合は$h'_{1i} = \overline{a} h_{1i}$、$i > 1, j > 1$の場合は$h'_{ij} = h_{ij}$になります。従って
$$
|\det \widetilde{X}| = |a|^2 |a|^{\delta(n-1)} = |a|^{2+\delta(n-1)}.
$$
一方、$Y = (y_{ij}) \in M_n(K)$の場合は、$i > 1$に対して$y'_{1j} = ay_{1j}$と$y'_{ij} = y_{ij}$を合わせた$XY = (y'_{ij})$になります。従って、$|N(X)| = |a|^{\delta n}$。 公式 (15) が再度検証されます。

c) $X$ は形の写像の行列です
$$
(x_1, \ldots, x_n) \mapsto (x_1 + bx_2, x_2, \ldots, x_n).
$$
次に、$\widetilde{X}((h_{ij})) = (h'_{ij})$と$h'_{11} = h_{11}$、$h'_{12} = h_{12} + h_{11} b$、$h'_{1i} = h_{1i}$が$i > 2$、$h'_{22} = h_{22} + \overline{b} h_{12} + \overline{h}_{12} b + \overline{b} h_{11} b$、$h'_{2i} = h_{2i} + \overline{b} h_{1i}$が$i > 2$、$h'_{ij} = h_{ij}$が$i > 2, j > 2$となります。 補題 6 を考慮すると、$|\det \widetilde{X}| = 1$ であることがわかります。同様に、公式の証明を完了する $|N(X)| = 1$ も検証します (15)。

これにより、$\mathfrak{H}$ の尺度 $|N(H)|^{-\lambda/2} d\mu(H)$ は、$\mathbf{GL}(n, K)$ の下でも不変です。
$$
\widetilde{X}^{-1}(|N(H)|^{-\lambda/2} d\mu(H)) = |N(\widetilde{X}(H))|^{-\lambda/2} \cdot |\det \widetilde{X}| d\mu(H)
= |N(H)|^{-\lambda/2} |N(X)|^{-\lambda} |\det \widetilde{X}| d\mu(H) = |N(H)|^{-\lambda/2} d\mu(H).
$$

$H \in \mathfrak{H}_+^*$ の場合、一部の $X \in \mathbf{GL}(n, K)$ については $H = \widetilde{X}(I_n) = {}^t \overline{X} X$、従って $N(H) = \overline{N(X)} N(X) > 0$ になります。従って、$\mathfrak{H}_+^*$ では、$\mathbf{GL}(n, K)$ (cf. §2, No. 6、Th. 3) の下で一意の (定数因子まで) 不変の測度が測度になります。
$$
d\gamma(H) = N(H)^{-\lambda/2} d\mu(H).
$$
特に、
$$
d\gamma(H) = (\det H)^{-(n+1)/2} d\mu(H) \quad \text{when } K = \mathbf{R},
$$
$$
d\gamma(H) = (\det H)^{-n} d\mu(H) \quad \text{when } K = \mathbf{C}.
$$

### 練習問題 {#int-vii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
