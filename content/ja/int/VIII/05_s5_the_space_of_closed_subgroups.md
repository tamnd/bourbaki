---
book: int
book_title: Integration
chapter: VIII
chapter_title: CONVOLUTION AND REPRESENTATIONS
section: 5
section_title: The space of closed subgroups
lang: ja
source: int-vii-ix
book_pages: INT VIII.73-INT VIII.74
pdf_pages: 0146-0159, 0173-0174
extraction: ocr
subsections:
    - "no": 1
      title: The space of Haar measures on the closed subgroups of G
      page: 46
      pdf_page: 146
    - "no": 2
      title: Semi-continuity of the volume of the homogeneous space
      page: 48
      pdf_page: 148
    - "no": 3
      title: The space of closed subgroups of G
      page: 51
      pdf_page: 151
    - "no": 4
      title: The case of groups without arbitrarily small finite subgroups
      page: 53
      pdf_page: 153
    - "no": 5
      title: The case of abelian groups
      page: 55
      pdf_page: 155
    - "no": 6
      title: Another interpretation of the topology of the space of closed subgroups
      page: 56
      pdf_page: 156
statements: 20
exercises: 6
content_sha256: 9bc52b31a1fd0496a0c244194f66dad53fc228706d48882ec10237181b1f19a2
translated_from: content/en/int/VIII/05_s5_the_space_of_closed_subgroups.md
translation_method: google
source_content_sha256: 0d59b39eb609eb19a1cde4e7e71ffe935476923daecf7a76ec5c3f620241a549
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: a1e369f387b76cd41f53b42d26a81f81d7473d2ceab8d6e4503e577dcabe5cc8
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 5。 空間 / 閉店中部分群

この切断を通して、G は局所的にコンパクトな群を表し、$\mu$ は G 上の右ハール測度を表します。

### 1. Gの閉鎖部分群に対するハール措置の空間

#### 補題 1 {#int-viii-s5-lem-1 .statement tag=09LY}

$\alpha$ を G、S のサポートに対する肯定的な尺度 $\neq 0$ とします。次の 2 つの条件は同等です。
a) S は G の閉じた部分群であり、S 上の $\alpha$ によって誘導される測度は S 上の右 Haar 測度です。
b) $s \in S$ごとに$\delta(s)\alpha = \alpha$。
さらに、これら条件が満たされると、$t \in G$の集合が$\delta(t)\alpha = \alpha$とSに等しくなります。
a) が b) を意味することは明らかです。逆に、関係 b) は、$x \in S$ ごとに $Sx = S$ を意味します。他の語、関係、$x \in S$、$y \in S$は、$y \in Sx$、または再び$yx^{-1} \in S$を暗示し、Sは空でないであるため、SはGの閉じた部分群です。 $St = S$ が S 自体、よって最後の主張と等しくなるような $t \in G$ の集合。

残りの切断については、G 上のポジティブな措置 $\neq 0$ 補題 1 の満たす条件を $\Gamma$ 集合で表し、すべての $\alpha \in \Gamma$ について、G のサポートである G のクローズド部分群を$H_\alpha$ で表します。 $\alpha$。

#### 命題 1 {#int-viii-s5-prop-1 .statement tag=09LZ}

集合 $\Gamma$ は、曖昧な位相を装備した空間 $\mathscr{M}_+(G) - \{0\}$ で閉じられます。
まず次の補題を証明します。

#### 補題 2 {#int-viii-s5-lem-2 .statement tag=09M0}

X を局所コンパクト空間とし、すべてのメジャー $\alpha \in \mathscr{M}_+(X) - \{0\}$ について、$S_\alpha$ を $\alpha$ のサポートとします。 $\Phi$ を、$\alpha_0 \neq 0$ の測定値に漠然と収束する $\mathscr{M}_+(X) - \{0\}$ のフィルターとします。次に、$\alpha_0$ のサポートの点のすべての近傍V に対して、集合 $M \in \Phi$ が存在し、$\alpha \in M$ ごとに $V \cap S_\alpha \neq \varnothing$ が存在します。
なぜなら、$\varphi \in \mathscr{K}_+(X)$ が写像で、V に含まれるサポートがあり、$\int \varphi(x) d\alpha_0(x) > 0$ である場合、定義までに集合 $M \in \Phi$ が存在し、すべての $\alpha \in M$ に対して $\int \varphi(x) d\alpha(x) > 0$ が存在し、これは$V \cap S_\alpha \neq \varnothing$ を意味します。

#### 補題 3 {#int-viii-s5-lem-3 .statement tag=09M1}

E をフィルタ $\Phi$ でフィルタリングした集合とし、E の写像を $\xi \mapsto \alpha(\xi)$ とし、$\Phi$ に関して測定$\alpha_0 \neq 0$ に漠然と収束する $\Gamma$ とします。一方、$\xi \mapsto t_\xi$を$E$の写像を$G$にすると、$\xi \in E$ごとに$t_\xi \in H_{\alpha(\xi)}$になります。 $s$ が $\Phi$ に関して写像 $\xi \mapsto t_\xi$ のクラスター 点である場合、$\delta(s)\alpha_0 = \alpha_0$ です。

置き換えること必要に応じて $\Phi$ より細かいフィルターを使用すると、$s$ は $\Phi$ に関して $\xi \mapsto t_\xi$ の極限であると仮定できます。 $\xi \in E$ ごとに補題 1、$\delta(t_\xi)\alpha(\xi) = \alpha(\xi)$ によって計算され、$G \times \mathscr{M}_+(G)$ での写像 $(u, \lambda) \mapsto \delta(u)\lambda$ の連続性から結論が得られます (§ 3, No. 3、提案 13)。

提案 1 を証明するには、$\Gamma$ のフィルター $\Psi$ が測定値 $\alpha_0 \neq 0$ に曖昧に収束し、$s$ 属するが $\alpha_0$ のサポートに収束する場合、$\delta(s)\alpha_0 = \alpha_0$ が補題 1 によって示されれば十分です。さて、$G$の$s$のすべての近隣$V$には、$\alpha \in M$ごとに、補題2までに$V \cap H_\alpha \neq \varnothing$が存在するような$M \in \Psi$が存在します。$s$のすべての近隣$V$とすべての$\alpha \in \Gamma$について、 $V \cap H_\alpha \neq \varnothing$ の場合は $t_{V,\alpha}$ を $V \cap H_\alpha$ の点とし、その逆の場合は $H_\alpha$ のいずれかの点とします。 $\Theta$ が $s$ の近傍フィルターの切断フィルターであり、$\Phi$ が積フィルター $\Theta \times \Psi$ である場合、$s$ は、前述のとおり、以下に関して $(V, \alpha) \mapsto t_{V,\alpha}$ のクラスター 点になります。 $\Phi$。一方、写像 $(V, \alpha) \mapsto \alpha$ は、$\Phi$ に対して極限として $\alpha_0$ を持っているため、補題 3 から命題が続きます。

#### 命題 2 {#int-viii-s5-prop-2 .statement tag=09M2}

— $\varphi$ を $\mathscr{K}_+(G)$ の写像とし、$\varphi(e) > 0$ とします。次に、曖昧な位相に対して $\int \varphi(x)\,d\alpha(x) = 1$ がコンパクトになるように、$\alpha \in \Gamma$ の措置の集合 $\Gamma_\varphi$ を実行します。

集合 $\Gamma_\varphi$ は、$\Gamma$ の共通部分と $\mathscr{M}(G)$ の超平面が$\alpha$ によって形成され、$\int \varphi(x)\,d\alpha(x) = 1$ になります。この超平面は $\mathscr{M}(G)$ で曖昧に閉じられており、含む 0 ではないので、提案 1 から、$\Gamma_\varphi$ は $\mathscr{M}(G)$ で曖昧に閉じられていることがわかります。したがって、$G$ のすべてのコンパクト部分集合 $K$ について、$\sup_{\alpha \in \Gamma_\varphi} \alpha(K) < +\infty$ があることを示すだけで十分です (Ch. III, §1, No. 9、提案 15)。ここで、$U$ を、不等式 $\varphi(x) > \varphi(e)/2$ によって定義される $G$ の $e$ の開いた近傍とします。 $\alpha \in \Gamma_\varphi$の$1 = \int \varphi(x)\,d\alpha(x) \geq \int_U \varphi(x)\,d\alpha(x)$から、設定 $c = 2/\varphi(e)$には、$\alpha \in \Gamma_\varphi$ごとに$\alpha(U) \leq c$があることがわかります。 $V$ を、$V^2 \subset U$ となるような $G$ における $e$ の対称な開いた近傍とする。すべての $x \in G$ とすべての $\alpha \in \Gamma_\varphi$ に対して $\alpha(Vx) \leq c$ であることを示しましょう。実際、$Vx$ が $\alpha$ のサポート $H_\alpha$ と交差しない場合、この関係は自明です。逆に、$h \in Vx \cap H_\alpha$ が存在する場合、$v \in V$、よってについては $h = vx$
$$
Vx = Vv^{-1}h \subset V^2h \subset Uh,
$$
$\delta(h)\alpha = \alpha$ なので、$\alpha(Vx) \leq \alpha(Uh) = \alpha(U) \leq c$ になります。さて、$(x_i)_{1 \leq i \leq n}$ を $K$ の点の数列として、$Vx_i$ 形が $K$ をカバーするようにします。上記のことから、$\alpha \in \Gamma_\varphi$ごとに$\alpha(K) \leq \sum_{i=1}^n \alpha(Vx_i) \leq nc$が得られます。 Q.E.D.

#### 命題 3 {#int-viii-s5-prop-3 .statement tag=09M3}

— *提案 2 の仮説の下では、写像* $\alpha \mapsto \left( \langle \varphi, \alpha \rangle, \frac{\alpha}{\langle \varphi, \alpha \rangle} \right)$ * は、積空間* $\mathbf{R}_+^* \times \Gamma_\varphi$ に対する* $\Gamma$ * の同型写像です。

写像 $\alpha \mapsto \langle \varphi, \alpha \rangle$ は漠然と連続しているため、$e$ 属するから$\alpha$ と $\varphi(e) > 0$ のサポート $H_\alpha$ まで、$\alpha \in \Gamma$ の小節ごとに $\langle \varphi, \alpha \rangle \neq 0$ であることを観察すれば十分です。

### 2. 均質体の体積の半連続性空間

この番号では、各小節 $\alpha \in \Gamma$ に対して集合

$$
Q_\alpha = G / H_\alpha ,
$$

そして、$\pi_\alpha$ 標準写像 $G \to Q_\alpha$ で表します。

$\Gamma^0$ を、$G$ の $H_\alpha$ 部分群が *ユニモジュラー* となるように、$\alpha$ の尺度によって形成された $\Gamma$ の部分集合とします。 $\Gamma^0$ の元は、写像 $f \in \mathscr{K}(G)$ ごとに $\alpha(f) = \alpha(\dot{f})$ になるという事実によって特徴付けられます ($\mathscr{K}(H_\alpha)$ のすべての写像は、ウリソーンの定理によって $\mathscr{K}(G)$ の写像まで拡張可能です)。つまり、$\Gamma^0$ は $\Gamma$ の *クローズ* 部分集合です。 $\alpha \in \Gamma^0$、商ごとに、$Q_\alpha$ の$\mu_\alpha = \mu / \alpha$ の測定値が定義され、$G$ では比較的不変であることを思い出してください (Ch. VII, §2, No. 6、Th. 3)。また、写像 $f \in \mathscr{K}(G)$ ごとに、

$$
\int_G f(x) d\mu(x) = \int_{Q_\alpha} d\mu_\alpha(\dot{x}) \int_{H_\alpha} f(xs) d\alpha(s) ,
$$

ここで、$\dot{x} = \pi_\alpha(x)$ は $Q_\alpha$ の $x \in G$ の標準像です。

#### 命題 4 {#int-viii-s5-prop-4 .statement tag=09M4}

— *$\Gamma^0$ *メジャーの集合とする* $\alpha \in \Gamma$ *そのような* $H_\alpha$ *単モジュールであり、すべての* $\alpha \in \Gamma^0$ *集合* $\mu_\alpha = \mu / \alpha$; *then 写像* $\alpha \mapsto \| \mu_\alpha \|$ *of* $\Gamma^0$ *into* $\overline{\mathbf{R}}$ *曖昧な位相* の下半連続です。

$\alpha \in \Gamma^0$ および写像 $f \in \mathscr{K}(G)$、集合ごとに

$$
f_\alpha(\dot{x}) = \int_{H_\alpha} f(xs) d\alpha(s) = (f * \alpha)(x) ,
$$

ここで、畳み込み積は正しい Haar 測定値 $\mu$ に対して取得され、$\dot{\alpha} = \alpha$ (§ 4, No. 4, 公式 (11)) という事実が利用されます。 私たちは知っています（Ch. VII, §2, No. 1、提案 2) $\mathscr{K}_+(G)$ の $\mathscr{K}_+(Q_\alpha)$ への写像 $f \mapsto f_\alpha$ は *全射* です。従って、(2) により、

$$
\| \mu_\alpha \| = \sup_{f \in \mathscr{K}_+(G), f \neq 0} \mu_\alpha(f_\alpha) / \| f_\alpha \| = \sup_{f \in \mathscr{K}_+(G), f \neq 0} \mu(f) / \| f_\alpha \|,
$$

集合があるところ

$$
\|f_\alpha\| = \sup_{\dot{x} \in Q_\alpha} |f_\alpha(\dot{x})| = \sup_{x \in G} |(f * \alpha)(x)| .
$$

命題を確立するには、$f \in \mathscr{H}_+(G)$ が与えられた場合、写像 $\alpha \mapsto \|f_\alpha\|$ が漠然と連続していることを示すだけで十分です。さて、K を $f$ のサポートとする。 写像 $f * \alpha$ は、$KH_\alpha$ に含まれるサポートを持ち、$H_\alpha$ の下で右側で不変です。その結果

$$
\|f_\alpha\| = \sup_{x \in K} |(f * \alpha)(x)| .
$$

従って、曖昧なトポロジーを備えた$\mathscr{M}_+(G)$の、コンパクトな収束トポロジーを備えた$\mathscr{C}(G)$への写像$\alpha \mapsto f * \alpha$は連続であるという事実から結論が得られます(§ 4, No. 2、備考1)。

測度 $\alpha \in \Gamma^0$ に対して、$\|\mu_\alpha\|$ が有限である場合、G は必然的に単モジュールであることを思い出してください (Ch. VII, §2, No. 6、Th. 3 の Cor. 3)。

#### 命題 5 {#int-viii-s5-prop-5 .statement tag=09M5}

*g を $\mu$ 可積分の正の数値写像とし、$\Gamma^0(g)$ をすべての $x \in G$ に対して $\int^* g(xs)\, d\alpha(s) \geq 1$ となるようなメジャー $\alpha \in \Gamma^0$ の集合とする。次に、$\Gamma^0(g)$ から $\overline{\mathbf{R}}$ への写像 $\alpha \mapsto \|\mu_\alpha\|$ は漠然と連続しています。*

すべてのメジャー $\alpha \in \Gamma^0(G)$ について、(Ch. VII, §2, No. 3、提案 5) 写像を思い出してください。

$$
g_\alpha(\dot{x}) = \int_{H_\alpha} g(xs)\, d\alpha(s)
$$

$\mu_\alpha$ - $Q_\alpha$ のほぼどこでも定義され、$\mu_\alpha$ - 積分可能、そして

$$
\int_G g(x)\, d\mu(x) = \int_{Q_\alpha} g_\alpha(\dot{x})\, d\mu_\alpha(\dot{x}) .
$$

提案 4 を考慮すると、$\Gamma^0(g)$ において、$\alpha \mapsto \|\mu_\alpha\|$ が*上* 半連続であることを証明すれば十分です。 メジャー $\alpha \in \Gamma^0(g)$ を固定し、K を G のコンパクト部分集合とします。 $Q_\alpha$ には、コンパクトなサポートを持つ連続した写像が存在し、その $[0, 1]$ の値は、コンパクトな集合 $\pi_\alpha(K)$ の 1 に等しくなります。 写像 $f \mapsto f_\alpha$ から $\mathscr{H}_+(G)$ への $\mathscr{H}_+(Q_\alpha)$ は全射法なので (Ch. VII, §2, No. 1、提案 2)、次のような写像 $f \in \mathscr{H}_+(G)$ が存在することがわかります。

$$
(f * \alpha)(x) = \int_G f(xs)\, d\alpha(s) \left\{ \begin{array}{ll}
\leq 1 & \text{for all } x \in G \\
= 1 & \text{for all } x \in K .
\end{array} \right.
$$

$\beta \mapsto f * \beta$ は、漠然とした位相を備えた $\mathscr{M}_+(G)$ の連続写像であり、コンパクトな収束 (§ 4, No. 2、注意 1) の位相を備えた $\mathscr{C}(G)$ になるため、$\varepsilon > 0$ ごとに、 集合 $U_\varepsilon$/$\beta \in \Gamma^0(G)$ は次のようになります
$$
f_\beta(\dot{x}) = \int_G f(xs)\, d\beta(s) > 1 - \varepsilon \quad \text{for all } x \in K
$$
$\Gamma^0(g)$の$\alpha$の開けた地域です。 $\beta \in U_\varepsilon$ ごとに、公式 (2) により、
$$
(5) \quad \| \mu_\alpha \| \geq \int_G f(x)\, d\mu(x) = \int_{Q_\beta} f_\beta(\dot{x})\, d\mu_\beta(\dot{x}) \geq (1 - \varepsilon) \mu_\beta(\pi_\beta(K)).
$$
数 $\varepsilon > 0$ が与えられた場合、$\int_G |g(x) - h(x)|\, d\mu(x) \leq \varepsilon$ となるように選ぶ写像 $h \in \mathscr{K}_+(G)$ を考え、前述の$K = \mathrm{Supp}(h)$ を考えてみましょう。したがって、$\beta \in \Gamma^0(g)$ ごとに、仮定 $g_\beta(\dot{x}) \geq 1$ までに、$Q_\beta$ のほぼどこでも ($\mu_\beta$ の場合)、
$$
\mu_\beta(Q_\beta - \pi_\beta(K)) \leq \int_{Q_\beta - \pi_\beta(K)} g_\beta(\dot{x})\, d\mu_\beta(\dot{x}) = \int_{G - KH_\beta} g(x)\, d\mu(x)
$$
(4) により。 $h$ は $K$ の外側で零であり、$KH_\beta$ の外側では $a fortiori$ であるため、次のようになります。
$$
\mu_\beta(Q_\beta - \pi_\beta(K)) \leq \int_{G - KH_\beta} |g(x) - h(x)|\, d\mu(x) \\
\leq \int_G |g(x) - h(x)|\, d\mu(x) \leq \varepsilon;
$$
この結果を (5) と組み合わせると、次のことがわかります。
$$
\| \mu_\beta \| \leq \varepsilon + \| \mu_\alpha \|/(1 - \varepsilon)
$$
$\beta \in U_\varepsilon$ のとき、証明が完了します。

#### 系 1 {#int-viii-s5-prop-5-cor-1 .statement tag=09M6}

— $K$ を $G$ のコンパクト部分集合、$V$ を $G$、$c$ 実数 $> 0$ の $e$ の対称コンパクト近傍とする。 $G = KH_\alpha$ と $\alpha(V) \geq c$ が曖昧に連続するような $\alpha \in \Gamma^0$ のセットへのマッピング $\alpha \mapsto \| \mu_\alpha \|$ の制限。

というのは、$g \in \mathscr{K}_+(G)$ を写像として、$x \in KV$ に対して $g(x) \geq 1/c$ となるようにします。 $x \in K$ ごとに、
$$
\int g(xs)\, d\alpha(s) \geq \int_V g(xs)\, d\alpha(s) \geq 1
$$

$\alpha$ 満たす条件/主張の場合。さらに、$\pi_\alpha(K) = Q_\alpha$ には $\alpha \in \Gamma^0(g)$、よって系があるためです。

#### 系 2 {#int-viii-s5-prop-5-cor-2 .statement tag=09M7}

*A を、G の $\mu$ 積分可能な部分集合とする。 $G = AH$ が漠然と連続であるような、G の離散部分群 H の正規化ハール測度の写像 $\alpha \mapsto \| \mu_\alpha \|$ から集合 $N_A$ の制限とする。

$a \in A$ と $\alpha \in N_A$ の場合、

$$
\int \varphi_A(as)\ d\alpha(s) \geq \varphi_A(a) = 1,
$$

そして、$\pi_\alpha(A) = Q_\alpha$ 以降、$N_A \subset \Gamma^0(\varphi_A)$ があり、したがって系は提案 5 に従います。

### 3. 空間の閉鎖部分群の G

G の *closed 部分群* の $\Sigma$ 集合で表しましょう。 if one associates to each measure $\alpha \in \Gamma$ 部分群 $H_\alpha$ that is the support of $\alpha$, one obtains 写像 (called canonical) of $\Gamma$ into $\Sigma$, which is clearly surjective and permits canonically identifying $\Sigma$ with 集合 of $\Gamma$ の相同性の群のうち軌道の比率は $> 0$ です。 $\Gamma$に曖昧な位相の商位相を装備した集合$\Sigma$は、Gのクローズ部分群*の*空間と呼ばれます。

#### 定理 1 {#int-viii-s5-thm-1 .statement tag=09M8}

*G を局所コンパクト群とする。 Gの空間$\Sigma$は閉じた部分群はコンパクトです。さらに、次の特性があります:*

(i) *集合 $\Sigma^0$ のユニモジュラー閉じた G の部分群は $\Sigma$ で閉じられています (したがってコンパクトです)。*

(ii) *G が e のコンパクト近傍によって生成される場合、G の商空間 $G/H$ がコンパクトであり、$\Sigma^0$ で開いている (したがって局所的にコンパクトである) ような、G のユニモジュラー閉部分群 H の集合 $\Sigma_c^0$ が生成されます。

(iii) *G の e の比較的コンパクトな開いた近傍 U ごとに、$H \cap U = \{e\}$ が $\Sigma^0$ で閉じられるように、G の離散部分群 H の集合 $D_U$ (したがってコンパクトです)。*

No. 1 の命題 3 から、$\Sigma$ は $\Gamma_\varphi$ と同相であるため、No. 1 の命題 2 によりコンパクトになります。さらに、No. 2 の冒頭で、$H_\alpha$ が単モジュールであるような対策 $\alpha \in \Gamma$ の集合 $\Gamma^0$ が $\Gamma$ で閉じられることが指摘されました。 $\Gamma^0$ は比 $> 0$ の相同性のもとで安定であるため、$\Sigma$ における $\Gamma^0$ の像 $\Sigma^0$ は、$\Sigma$ の閉じた部分集合であり、これは (i) を証明します。

性質 (ii) は、次の命題の帰結になります。

#### 命題 6 {#int-viii-s5-prop-6 .statement tag=09M9}

*局所的にコンパクトな群 G が e のコンパクトな近傍によって生成されると仮定します。すると、$G/H_\alpha$がコンパクトになる$\alpha \in \Gamma^0$*の集合$\Gamma_c^0$が$\Gamma^0$に開いており、写像$\alpha \mapsto \| \mu_\alpha \|$の制限～$\Gamma_c^0$が漠然と連続しています。

No. 2 の提案 5 の記法により、$g \in \mathscr{K}_+(G)$ について、

$$
\Gamma^0(g) \subset \Gamma_c^0.
$$

なぜなら、K が $g$ のサポートである場合、すべての $x \in G$ に対する関係 $\int g(xs)\, d\alpha(s) \geq 1$ は $KH_\alpha = G$ を意味し、積分は明らかに $KH_\alpha$ の補数で零であるため、$G/H_\alpha = \pi_\alpha(K)$ はコンパクトです。 したがって、尺度 $\alpha \in \Gamma_c^0$ が与えられると、$\Gamma^0(g)$ が $\Gamma^0$ の $\alpha$ の近傍となるように、定義する写像 $g \in \mathscr{K}_+(G)$ で十分です。 $G/H_\alpha$ はコンパクトであり、$\mathscr{K}_+(G)$ の $\mathscr{K}_+(G/H_\alpha)$ への標準写像 $f \mapsto f_\alpha$ は全射的であるため (Ch. VII, §2, No. 2)、*すべての* $x \in G$ に対して $\int g(xs)\, d\alpha(s) = 2$ となるような写像 $g \in \mathscr{K}_+(G)$ が存在します。 K を、G を生成する G 内の e の対称コンパクト近傍である $g$、L の (コンパクトな) サポートとします。 $\mathscr{M}_+(G)$ の $\mathscr{C}(G)$ への写像 $\beta \mapsto g * \beta$ が漠然と連続している場合 (§ 4, No. 2、*注釈* 1)、 $\Gamma^0$ には次のような $\alpha$ の近傍 W が存在します。

$$
(g * \beta)(x) = \int g(xs)\, d\beta(s) \geq 1
$$

すべての $\beta \in W$ と $x \in LK$ に対して。 (7) の最初のメンバーが $KH_\beta$ の外側の零に等しいことは、関係 $\beta \in W$ を意味します。

$$
LK \subset KH_\beta,
$$

そこから、$n$ の帰納法によって、整数 $n > 0$ ごとに $L^n K \subset KH_\beta$ が推定されます。 L 生成する G から、すべての小節 $\beta \in W$ に対して $G = KH_\beta$ が得られ、これは $W \subset \Gamma_c^0$ であることを証明します。一方、$H_\beta$, 不等式 (7) の下で右側で不変である (7) の最初のメンバーは、$x \in LKH_\beta = G$ でも有効です。したがって $W \subset \Gamma^0(g)$ となり、命題が証明されます。

最後に、(iii) は次の命題の帰結になります。

#### 命題 7 {#int-viii-s5-prop-7 .statement tag=09MA}

*$N \subset \Gamma^0$ を G の離散部分群上の正規化ハール測度の部分空間とし、G の e の比較的コンパクトな開いた近傍 U ごとに、$N_U$ を $H_\alpha \cap U = \{e\}$ となるように $\alpha$ によって形成される N の部分集合とします。 次に:
a) $N_U$ はコンパクトです。
b) U が G の e の比較的コンパクトな開いた近傍の集合の上を走るため、N の集合 $N_U$ の内部は N のカバーを形成します。
c) N の部分集合 M が N 内で比較的コンパクトであるためには、$M \subset N_U$* となるような、G 内に e の比較的コンパクトな開いた近傍 U が存在することが必要かつ十分です。

$D_U$ は正準連続写像 $\Gamma \to \Sigma$ の下で $N_U$ の像であるため、Th の主張 (iii)。提案 7 a) から直ちに 1 が得られます。

提案 7 を証明するために、$N_U$ は、$\alpha$ によって形成される $\Gamma^0$ の部分集合として定義できることがわかります。

$$
\alpha(\{e\}) \geq 1 \quad \text{and} \quad \alpha(U) \leq 1.
$$

さて、$A$が$G$でコンパクト（それぞれオープンで比較的コンパクト）である場合、$\mathscr{M}_+(G)$の$\alpha \mapsto \alpha(A)$から$\mathbf{R}$への写像は、曖昧な位相にとって上部（それぞれ下部）半連続です（提案5のIV, §4, No. 4、コリント3）。および引用文献、§1, No. 1、提案 4)。したがって、$N_U$ は $\Gamma^0$ の閉じた部分集合であることがわかります。さらに、$\varphi \in \mathscr{K}_+(G)$ を写像として、$G - U$ で $\varphi(e) = 1$ と $\varphi(x) = 0$ が成り立つようにします。すべての $\alpha \in N_U$ に対して $\int \varphi(x) d\alpha(x) = 1$ であることは明らかです。したがって、No. 1 の提案 2 は、$N_U$ がコンパクトな集合であることを示し、a) を証明します。一方、$V$ を、$\overline{V} \subset U$ のような$G$ の$e$ の比較的コンパクトな開いた近傍とし、$\varphi \in \mathscr{K}_+(G)$ を$U$ に含まれるサポートと$V$ の$\varphi(x) = 1$ とする。次に、$\alpha \in N_U$ に対して$\alpha(\varphi) = 1$、したがって、$\beta \in W$ に対して$\beta(\varphi) < 2$ となるように、$N$ に$\alpha$ の近傍$W$ が存在します。したがって、$W \subset N_V$、したがって$N_V$ は$N_U$ の近傍であることが明らかです。 $N_U$ が $N$ をカバーしているので、これは b) を証明します。最後に、$N$ のすべてのコンパクト部分集合 $M$ は、集合 $N_{U_i}$ ($1 \leq i \leq n$) の有限和集合に含まれており、$\bigcup_i N_{U_i} \subset N_U$ 以降、$U = \bigcap_i U_i$ であるため、これは c) を証明します。

#### 系 {#int-viii-s5-n3-cor-1 .statement tag=09MB}

— *部分空間* $N$ *of* $\Gamma^0$ *局所的にコンパクト*。

### 4. 任意の小さな有限有限部分群を持たない群の場合

#### 定理 2 {#int-viii-s5-thm-2 .statement tag=09MC}

— *$G$ * を局所的にコンパクトな群満たす次の条件* とします:
(L) *$G$ に * $e$ * の近傍が存在します * $G$ * $e$ に * 還元されない* 含む有限の部分群はありません。
*次のプロパティが保持されます*:
(i) * $G$ の離散部分群の *集合* $D$ *は、局所的に閉じられています* $\Sigma$ *(局所的にコンパクトであるというと同等です)*。
(ii) *閉じた部分集合* $A$ *of* $D$ *コンパクトであるためには、$U$ *of* $e$ *in* $G$ *そのような* $H \cap U = \{e\}$ *部分群* ごとに近隣* が存在することが必要かつ十分です。 $H \in A$。
(iii) *加法* $G$ * が $e$ のコンパクトな近傍によって生成される場合、 *その後集合* $D_c$ *離散部分群* $H$ *の* $G$ *そのような* $G/H$ *コンパクトはローカルに閉じられています* $\Sigma$ *(したがってローカルにコンパクトです)*。

$D_c = D \cap \Sigma_c^0$ があるので、(iii) は (i) の帰結であり、Th です。 No. 3の1(ii)。

No. 3 の記法、提案 7 により、証明 (i) および (ii) について、次のことを証明するだけで十分です。

#### 命題 8 {#int-viii-s5-prop-8 .statement tag=09MD}

*N から D への正準全単射は同相写像です。*

ここで、$\Gamma_d$ が$G$ の離散部分群上のハール測度の集合である場合、$D$ は比を持つ$\Gamma_d$ の同種の軌道の群の空間と正準同型です。 $> 0$ (GT、I, §5, No. 2、提案 4)。したがって、$\Gamma_d$ の $\mathbf{R}_+^* \times \mathbf{N}$ への標準写像 $\alpha \mapsto (\alpha(\{e\}), \alpha/\alpha(\{e\}))$ が *同相同型* であることを証明すれば十分であり、これは次の補題から得られます。

#### 補題 4 {#int-viii-s5-lem-4 .statement tag=09ME}

*群 G が条件 (L) を満たす場合、$\Gamma_d$ から $\mathbf{R}_+^*$ への写像 $\alpha \mapsto \alpha(\{e\})$ は漠然と連続です。

メジャー $\alpha \in \Gamma_d$ を考えてみましょう。 $V_0$ を、$H_\alpha \cap V_0 = \{e\}$ となり、$V_0$ に含まれ、$e$ に還元されない$G$ の有限部分群が存在しないように、$G$ の$e$ の比較的コンパクトな開いた近傍とする。 $V$ を $V^3 \subset V_0$ となるような $e$ の対称なコンパクト近傍とし、$U$ を $U^2 \subset V$ となるような $e$ の対称な近傍とする。 $\varphi$ (それぞれ $\psi$) を $\mathscr{H}_+(G)$ の写像とし、$[0, 1]$ の値を $V^3$ (それぞれ点 $e$) の 1 に等しく、 $V_0$ (それぞれ$U$)。 $|\beta(\varphi) - \alpha(\varphi)| \leq \varepsilon$ と $|\beta(\psi) - \alpha(\psi)| \leq \varepsilon$ が $\alpha$ の近傍 $W$ となるようなメジャー $\beta \in \Gamma_d$ の集合。 $\varepsilon$ が十分に小さいと仮定すると、$H_\beta \cap V = \{e\}$ *すべての* $\beta \in W$; を示すことを提案します。次に、$\beta(\psi) = \beta(\{e\})$ が続き、したがって $|\beta(\{e\}) - \alpha(\{e\})| \leq \varepsilon$ となり、補題が証明されます。

$\beta \in W$ について、次のことを示すだけで十分です。

$$
(V^2 - V) \cap H_\beta = \varnothing.
$$

というのは、この点が確立されていると仮定します。そのとき、$V \cap H_\beta$の$x$と$y$については、$xy^{-1} \in V^2 \cap H_\beta$が得られます。しかし、(8) のおかげで、これは $xy^{-1} \in V \cap H_\beta$ を意味します。他の語では、$V \cap H_\beta$ は $G$ の *部分群* であり、明らかに離散的でコンパクトであるため、有限です。しかしその後、$V_0$の選択までに、これは確かに$V \cap H_\beta = \{e\}$であることを意味します。

矛盾によって議論して、$V^2 - V$ のうち属するから $H_\beta$ までの点 $z$ が存在すると仮定しましょう。 $U$ と $V$ の選択により、$G$ に $\psi(sz^{-1}) + \psi(s) \leq \varphi(s)$ があり、関係 $z \notin U^2$ は $Uz \cap U = \varnothing$ を暗示します。以来

$$
\int \psi(sz^{-1})\, d\beta(s) = \int \psi(s)\, d\beta(s),
$$

したがって、$2\beta(\psi) \leq \beta(\varphi) \leq \alpha(\varphi) + \varepsilon$;しかし、私たちにもあります
$$
\beta(\psi) \geq \alpha(\psi) - \varepsilon,
$$
そして構成 $\alpha(\varphi) = \alpha(\psi) = \alpha(\{e\})$ によって。したがって、$\varepsilon < \alpha(\{e\})/3$ を取ると矛盾に到達します。 Q.E.D.

図項、群 $G$ 満たす条件 (L) は *任意に小さい有限部分群を持たないと言われています。* すべてのリー群は条件 (L) を満たすことがわかります。しかし、この条件はリー群の特徴ではありません。たとえば、1 mod $p$ に合同な $p$-進数整数の乗法群は (L) を満たします。*

### 5. アーベル群の場合

Let $G$ be a locally compact group, $N \subset \Gamma^0$ the subspace of normalized Haar measures on the discrete subgroups of $G$, and $N_c$ the subset of $N$ corresponding to the discrete subgroups $H$ of $G$ such that $G/H$ is *compact*; thus $N_c = N \cap \Gamma_c^0$ in the notations of No. 3, Prop. 6; and if the group $G$ is generated by a compact neighborhood of $e$, it follows from No. 3, Prop. 6 that $N_c$ is *open* in $N$ (hence is *locally compact* by No. 3, Cor. of Prop. 7) and that the restriction to $N_c$ of the mapping $\alpha \mapsto \| \mu_\alpha \|$ is *vaguely continuous*.

#### 命題 9 {#int-viii-s5-prop-9 .statement tag=09MF}

*$G$ を、$e$ のコンパクトな近傍によって生成された局所的にコンパクトなアーベル群とします。 $N_c$ のサブセット $A$ が $N_c$ で比較的コンパクトであるためには、次の 2 つの条件を満たすことが必要かつ十分です。

(i) *すべての $\alpha \in A$ に対して $H_\alpha \cap U = \{e\}$ となるような、$G$ の $e$ の開いた近傍 $U$ が存在します。

(ii) *すべての $\alpha \in A$ に対して $\mu_\alpha(G/H_\alpha) \leq k$ となるような定数 $k$ が存在します。

$N_c$ で$A \subset N_c$ が比較的コンパクトであれば、$N$ では *なおさら* なので、条件 (i) と (ii) の必然性は、No. 3 の Props から続きます。 6 と 7 ($G$ がアーベルであるとは想定しません)。 逆に、$A \subset N_c$ がこれらの条件を満たすとします。 $\overline{A}$ が $N$ の *$A$ の閉包である場合、No. 3、提案 7 により $\overline{A}$ はコンパクトになります。さらに、曖昧な位相 (No. 2、提案 4) に対して $\alpha \mapsto \| \mu_\alpha \|$ は $\Gamma^0$ の下位半連続であるため、条件 (ii) はすべての $\alpha \in \overline{A}$ に対して $\| \mu_\alpha \| \leq k$ も持つことを意味します。 さて、$G$ はアーベルなので、$\mu_\alpha = \mu/\alpha$ は群 $G/H_\alpha$ の Haar 測度であり、したがって $G/H_\alpha$ はすべての $\alpha \in \overline{A}$ に対してコンパクトです (Ch. VII, §1, No. 2、提案 2)。 これは、$\overline{A} \subset N_c$、つまり$A$ が$N_c$ で比較的コンパクトであることを意味します。

#### 系 {#int-viii-s5-n5-cor-1 .statement tag=09MG}

*$G$ を、No. 4 の $e$ と満たす条件 (L) のコンパクト近傍によって生成される局所的にコンパクトなアーベル群とします。

$D_c$ を、$G/H$ がコンパクトになるように、$G$ の離散部分群 $H$ の集合とし、$H \in D_c$ ごとに、$v(H)$ を総質量$\mu_\alpha(G/H)$ とし、$\mu_\alpha$ を商の測定値とします。 $H$ の正規化ハール測度 $\alpha$ による $\mu$ 。 空間 $D_c$ の部分集合 $A$ が $D_c$ で比較的コンパクトであるためには、次の 2 つの条件が満たすであることが必要十分です。

(i) $G$ には、すべての $H \in A$ に対して $H \cap U = \{e\}$ となるような、$e$ の開いた近傍 $U$ が存在します。

(ii) すべての $H \in A$ に対して $v(H) \leq k$ となるような定数 $k$ が存在します。

提案 9 を考慮すると、これは、$N$ の正準全単射から $D$ 上で $D_c$ が $N_c$ の像であるという事実、および作成された仮説の下では、この全単射が同型であるという事実からすぐに得られます (No. 4、提案 8)。

#### 例 {#int-viii-s5-n5-exa-1 .statement tag=09MH}

$G = \mathbf{R}^n$ と $\mu$ についてルベーグ測度を考えてみましょう。コルのすべての仮説。提案 9 は満たされている。 $G/H$ がコンパクトであるような $G$ の離散部分群 $H$ は、*階数* $n$ (GT, VII, §1, No. 1, Th. 1) の離散部分群に他なりません。このような部分群 $H$ は $\mathbf{R}^n$ の基底 $(a_i)_{1 \leq i \leq n}$ によって生成され、

$$
v(H) = |\det(a_1, \ldots, a_n)|
$$

(行列式は $\mathbf{R}^n$ の標準基底に関して取られています) (Ch. VII, §2, No. 10、Th. 4)。ここで、空間 $D_c$ は次のように解釈できます。すべての部分群 $H \in D_c$ は、部分群 $\mathbf{Z}^n$ の変換 $g \cdot \mathbf{Z}^n$ と元 $g \in \mathbf{GL}(n, \mathbf{R})$、および部分群です。 $\mathbf{Z}^n$ 安定を離れる $\mathbf{GL}(n, \mathbf{R})$ は $\mathbf{GL}(n, \mathbf{Z})$ と識別される場合があります。その結果、$D_c$ は、$\mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z})$ と (非トポロジカルな) 同次の空間として正規に識別される可能性があります。一方、$\mathbf{GL}(n, \mathbf{R})$ は$\mathbf{R}^n$ で継続的に動作するため、曖昧な位相 (§3, No. 3、提案 13) に対して$\mathscr{M}_+(\mathbf{R}^n)$ も動作し、従って$\mathscr{M}_+(\mathbf{R}^n)$ の$N_c$ で部分空間も動作します。さらに、$N_c$ の $D_c$ への正準同型写像 (No. 4、提案 8) は、$\mathbf{GL}(n, \mathbf{R})$ の演算の法則と互換性があります。 $\mathbf{GL}(n, \mathbf{R})$ は無限可算であり、$D_c$ は局所的にコンパクトであるため、上記で定義された $D_c$ への $\mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z})$ の全単射は *同相同相* (Ch. VII、App. I、補題 2)。コル。従って、提案 9 は、均質な空間 $\mathbf{GL}(n, \mathbf{R})/\mathbf{GL}(n, \mathbf{Z})$ におけるコンパクトさの基準を与えます。

### 6. 他のクローズド部分群の空間の位相の解釈

$\mathfrak{F}$ を $G$ のクローズド部分集合の集合とします。 $\mathfrak{F}$ 上の *ハウスドルフ均一構造* を 1 つ定義する以下のようにします: $G$ のすべてのコンパクト部分集合 $K$ と $G$ の $e$ のすべての近傍 $V$ について、$P(K, V)$ を次のようにします集合の対 $(X, Y)$ の元の $\mathscr{F}$ は両方とも

$$
(9) \quad X \cap K \subset VY \quad \text{and} \quad Y \cap K \subset VX.
$$

$P(K, V)$ の集合が、$\mathscr{F}$ のハウスドルフのユニフォーム構造 $\mathscr{U}$ の側近の基本系であることを示しましょう。 GT の公理 $(U'_I)$ と $(U'_{II})$、II, §1, No. 1 は明らかに満たされています。さらに、関係 $K \subset K'$ と $V' \subset V$ は $P(K', V') \subset P(K, V)$ を暗示します。 $(U'_{III})$ を検証するには、$V$ が $e$ の対称でコンパクトな近傍であるため、$VK$ がコンパクトである場合を極限で検証することができます。 $(X, Y) \in P(VK, V)$ と $(Y, Z) \in P(VK, V)$ があるとします。次に $X \cap K \subset X \cap VK \subset VY$、そして $y \in Y$ が一部の $v \in V$ に対して $vy \in K$ である場合、必然的に $y \in VK$ となるため、

$$
X \cap K \subset V(Y \cap VK);
$$

一方、$Y \cap VK \subset VZ$、よって $X \cap K \subset V^2Z$、そして 1 つは同様に $Z \cap K \subset V^2X$ を示し、$(U'_{III})$ を証明します。 最後に、$X, Y$ が $\mathscr{F}$ の 2 つの異なる元である場合、例えば $a \notin Y$ のような点 $a \in X$ が存在するため、$Va \cap Y = \varnothing$、つまり $a \notin VY$ のような $e$ の対称コンパクト近傍 $V$ が存在します。 *なおさら* $(X, Y) \notin P(Va, V)$、これで主張の証明が完了します。

これが確立されたので、先ほど定義したユニフォーム空間 $\mathscr{F}$ の位相によって引き起こされる $G$ 位相 $\mathscr{T}$ のクローズド部分群の集合 $\Sigma$ を考えてみましょう。 この位相が No. 3* で定義された位相と * 同一であることがわかります。 $\Sigma$ にトポロジー $\mathscr{T}$ が装備されている場合、$\Gamma$ の $\Sigma$ へのマッピング $\alpha \mapsto H_\alpha$ が *連続* であることを証明すれば十分です。つまり、このマッピングの $\Gamma_\varphi$ への制限にも同じことが当てはまります (No. 1、提案 2 のような表記を使用)。全単射;しかし、$\Gamma_\varphi$ はコンパクトであり、トポロジー $\mathscr{T}$ は分離されているため、$\Gamma_\varphi$ の $\Sigma$ への写像 $\alpha \mapsto H_\alpha$ は準同型写像になります。

したがって、$\alpha_0$ を $\Gamma$ の点とし、$\Phi$ を $\alpha_0$ に収束する $\Gamma$ のフィルターとします。 $\Phi$ に関して、$H_\alpha$ は位相 $\mathscr{T}$ に対して $H_{\alpha_0}$ になる傾向があることを示します。 $K$ を $G$ のコンパクト部分集合、$V$ を $G$ の $e$ の対称コンパクト近傍とする。 $x \in H_{\alpha_0} \cap K$ ごとに集合 $M(x) \in \Phi$ が存在し、$\alpha \in M(x)$ ごとに $Vx \cap H_\alpha \neq \varnothing$ (No. 1, 補題 2)、よって $Vx \subset V^2H_\alpha$ が存在します。 集合 $Vx_i$ の有限数で $H_{\alpha_0} \cap K$ をカバーすると、$M = \bigcap_i M(x_i)$ であれば、$\alpha \in M$ ごとに $H_{\alpha_0} \cap K \subset V^2H_\alpha$ になることがわかります。

逆に、$G$ に $e$ の開いた近傍 $U$ が存在し、集合 $L \in \Phi$ ごとに $H_\alpha \cap K \not\subset UH_{\alpha_0}$ を含む $\alpha \in L$ が少なくとも 1 つ存在すると仮定します。 $\omega(L)$ が、この性質を持つ $\alpha \in L$ の集合である場合、$\omega(L)$ は、$\Phi$ よりも $\Gamma$ より細かいのフィルタ $\Phi'$ の形基底になります。 $L \in \Phi$ に対する $\omega(L)$ の $\alpha$ 所属から和集合 $E$ には、所属から $UH_{\alpha_0}$ ではなく $t_\alpha \in H_\alpha \cap K$ が存在します。 $\alpha \notin E$ の場合は、$H_\alpha$ のいずれかの点を $t_\alpha$ とします。 $K \cap C(UH_{\alpha_0})$ はコンパクトなので、$\Phi'$、所属 ～ $K \cap C(UH_{\alpha_0})$ に関して、$\alpha \mapsto t_\alpha$ のクラスター点 $s$ が存在します。しかし、$\Phi'$ は $\Gamma$ で $\alpha_0$ に収束するため、この矛盾する補題は No. 1 の 3 になります。

練習問題

### 練習問題 {#int-viii-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
