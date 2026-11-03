---
book: evt
book_title: Topological Vector Spaces
chapter: V
chapter_title: HILBERTIAN SPACES (ELEMENTARY THEORY)
section: 3
section_title: Tensor product of hilbertian spaces
lang: ja
source: evt-i-v
book_pages: TVS V.25-TVS V.37, TVS V.73-TVS V.74
pdf_pages: 0283-0295, 0331-0332
extraction: ocr
subsections:
    - "no": 1
      title: Tensor product of prehilbertian spaces
      page: 25
      pdf_page: 283
    - "no": 2
      title: Hilbertian tensor product of hilbertian spaces
      page: 28
      pdf_page: 286
    - "no": 3
      title: Symmetric hilbertian powers
      page: 29
      pdf_page: 287
    - "no": 4
      title: Exterior hilbertian powers
      page: 33
      pdf_page: 291
    - "no": 5
      title: Exterior multiplication
      page: 35
      pdf_page: 293
statements: 20
exercises: 2
content_sha256: 0f81ec7ca8d8cb13157e52732bed2c748165160504bcad18e2f8f92c0e8a4333
translated_from: content/en/evt/V/03_s3_tensor_product_of_hilbertian_spaces.md
translation_method: google
source_content_sha256: 02cb54c6e38040afaaa4704bd9864f0e39ab141fc23dcd61afa7b042aa7a7e87
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: e5033c45ab29860840e6c2eb70ba346637bc6219724f38ccf5d576db3f6eeac4
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 3。ヒルバーティアンのテンソル積空間

### 1. プレヒルバーティアンのテンソル積空間

$E_1$ と $E_2$ を 2 つの前ヒルバーティアン空間とし、$F = E_1 \otimes E_2$ をベクトル空間 $E_1$ と $E_2$ のテンソル積とします。 $x_1 \in E_1$ と $x_2 \in E_2$ としましょう。 $E_1 \times E_2$ から K への写像 $(y_1, y_2) \mapsto \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle$ は双線形であるため、$E_1 \otimes E_2$ には次のような線型形式 $\phi_{x_1, x_2}$ が存在します。
$$
\phi_{x_1, x_2}(y_1 \otimes y_2) = \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle
$$
$y_1 \in E_1$と$y_2 \in E_2$の場合。 $z \in F$ にしましょう。 $E_1 \times E_2$ から K への写像 $(x_1, x_2) \mapsto \overline{\phi_{x_1, x_2}(z)}$ は双線形です。これは、形 $z = \sum_{i=1}^n y_{i,1} \otimes y_{i,2}$ に $y_{i,1} \in E_1$ と $1 \leq i \leq n$ に $y_{i,2} \in E_2$ を付けて $z$ を書くことでわかります。次に、$F = E_1 \otimes E_2$ には次のような線型形式 $\psi_z$ が存在します。
$$
\psi_z(x_1 \otimes x_2) = \overline{\phi_{x_1, x_2}(z)} \quad (x_1 \in E_1, x_2 \in E_2).
$$
F の $z, t$ に $\Phi(z, t) = \psi_z(t)$ を入れます。$\Phi$ が、次の特徴を持つ $E_1 \otimes E_2$ 上のセスキ線形であることがすぐにわかります。
$$
\Phi(x_1 \otimes x_2, y_1 \otimes y_2) = \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle
$$
(cf.A、IX, § 1, No. 11)。

#### 命題 1 {#evt-v-s3-prop-1 .statement tag=080B}

— $E_1 \otimes E_2$ 上のセスキロ形 $\Phi$ はエルミートで正であるため、プレヒルバーティアン空間の構造を $E_1 \otimes E_2$ に割り当てます。 $E_1$と$E_2$がハウスドルフなら、この空間はハウスドルフです。

$z = x_1 \otimes x_2$ と $t = y_1 \otimes y_2$ の場合、(3) から公式 $\Phi(z, t) = \overline{\Phi(t, z)}$ が続きます。一般的な場合は線形性によって得られるため、$\Phi$ はエルミートになります。

$E_1$ と $E_2$ がハウスドルフであると仮定します。 エルミート形 $\Phi$ が正で分離していることを証明します。 $z = \sum_{i=1}^n x_i \otimes y_i$ を $F = E_1 \otimes E_2$ の非ゼロ元とします。 $(e_1, ..., e_n)$ を、$x_1, ..., x_n$ (V, p. 23, cor. 1) によって生成された $E_1$ の部分空間の正規直交基底とします。 $E_2$ には元 $f_1, ..., f_m$ が存在しますが、$z = \sum_{i=1}^n e_i \otimes f_i$ のようにすべてが null ではないため、
$$
\Phi(z, z) = \sum_{i,j=1}^m \Phi(e_i \otimes f_i, e_j \otimes f_j)
$$
$$
= \sum_{i,j} \langle e_i | e_j \rangle \langle f_i | f_j \rangle = \sum_{i=1}^m \| f_i \|^2 > 0.
$$

一般的なケースでは、$\Phi$ が正であることを証明します。 $\tilde{E}_i$ を $E_i$ に関連付けられたハウスドルフプレヒルバーティアン空間とし、$\pi_i$ を $E_i$ から $\tilde{E}_i$ ($i = 1, 2$) までの標準写像とします。 $\pi = \pi_1 \otimes \pi_2$を入れます。 $\Phi$と同じ方法で構築された$\tilde{E}_1 \otimes \tilde{E}_2$上の$\tilde{\Phi}$をエルミート形とします。私たちは持っています
$$
\Phi(z, t) = \Phi(\pi(z), \pi(t)) \quad (z \in F, \ t \in F),
$$
$\tilde{\Phi}$ は正なので、$\Phi$ も正です。

prop で定義されたプレヒルバーティアン空間。 1 は、プレヒルバーティアン空間* $E_1$ と $E_2$ の *テンソル積と呼ばれ、$E_1 \otimes E_2$ と書きます。今後、$\Phi(z, t)$ を $\langle z|t \rangle$ と書きますので、定義までに
$$
\langle x_1 \otimes x_2 | y_1 \otimes y_2 \rangle = \langle x_1 | y_1 \rangle \langle x_2 | y_2 \rangle;
$$
$\langle z|z \rangle^{1/2}$ には $\|z\|_2$ または $\|z\|$ とも書きます。 (4) から、次のようになります。
$$
\|x_1 \otimes x_2\|_2 = \|x_1\| \cdot \|x_2\|,
$$
この場合、$E_1 \times E_2$ から $E_1 \otimes E_2$ への双線形マッピング $(x_1, x_2) \mapsto x_1 \otimes x_2$ は連続です。

$i = 1, 2$ について、$F_i$ を、誘導前ヒルバーティアン構造を備えた $E_i$ のベクトル部分空間とします。すると、$F_1 \otimes F_2$ は、$E_1 \otimes E_2$ のベクトル部分空間と識別できます (A、II, § 7, No. 7)。 公式 (4) は、$E_1 \otimes_2 E_2$ のプレヒルバーティアン空間構造を伴う $F_1 \otimes F_2$ が、正確に $F_1 \otimes_2 F_2$ であることを示しています。今後は同一視する $F_1 \otimes_2 F_2$ を $E_1 \otimes_2 E_2$ の前ヒルバーティアン部分空間とします。

#### 命題 2 {#evt-v-s3-prop-2 .statement tag=080C}

*$i = 1, 2$の場合、$E_i$と$F_i$を2つのハウスドルフプレヒルベルト空間とし、$u_i \in \mathscr{L}(E_i; F_i)$とします。 線形写像 $u_1 \otimes u_2$ $E_1 \otimes_2 E_2$ から $F_1 \otimes_2 F_2$ は連続であり、*
$$
\|u_1 \otimes u_2\| = \|u_1\| \cdot \|u_2\|.
$$

によって与えられる $E_1$ の正のエルミート形を考えてみましょう。
$$
f(x_1, y_1) = \|u_1\|^2 \langle x_1 | y_1 \rangle - \langle u_1(x_1) | u_1(y_1) \rangle.
$$

プロップにより。 1 (V, p. 25)、$E_1 \otimes E_2$ には次のような *正* エルミート形 $\Phi$ が存在します。
$$
\Phi(x_1 \otimes x_2, y_1 \otimes y_2) = f(x_1, y_1) \langle x_2 | y_2 \rangle =
$$
$$
= \|u_1\|^2 \langle x_1 \otimes x_2 | y_1 \otimes y_2 \rangle - \langle (u_1 \otimes 1)(x_1 \otimes x_2) | (u_1 \otimes 1)(y_1 \otimes y_2) \rangle
$$
$E_1$の$x_1, y_1$と$E_2$の$x_2, y_2$。線形性により、次のようになります。
$$
\Phi(z, t) = \|u_1\|^2 \langle z|t \rangle - \langle (u_1 \otimes 1)(z) | (u_1 \otimes 1)(t) \rangle
$$
$E_1 \otimes E_2$の$z, t$用。 $\Phi$ は正なので、$\Phi(z, z) \geq 0$、つまり $\|(u_1 \otimes 1).z\|_2$ が得られます。

$$
\leq \|u_1\| \cdot \|z\|_2 \text{ for } z \in E_1 \otimes_2 E_2, \text{ or } \|u_1 \otimes 1\| \leq \|u_1\|. \text{ Similarly we prove the inequality } \|1 \otimes u_2\| \leq \|u_2\|, \text{ and since } u_1 \otimes u_2 = (u_1 \otimes 1) \circ (1 \otimes u_2), \text{ we get}
$$
$$
\|u_1 \otimes u_2\| \leq \|u_1\| \cdot \|u_2\|.
$$
一方、
$$
\|u_1\| \cdot \|u_2\| = \sup_{\|x_1\| \leq 1, \|x_2\| \leq 1} \|u_1(x_1)\| \cdot \|u_2(x_2)\|
$$
$$
= \sup_{\|x_1\| \leq 1, \|x_2\| \leq 1} \|(u_1 \otimes u_2)(x_1 \otimes x_2)\|_2 \leq \|u_1 \otimes u_2\|.
$$
これでプロップの証明が完成しました。 2.Q.E.D.

$E_1, ..., E_n$ をプレヒルバーティアン空間 ($n \geq 2$) とします。私たちは定義するテンソル積 $E_1 \otimes_2 ... \otimes_2 E_n$ ($\bigotimes_{i=1}^n E_i$ とも表記) によって帰納法によって、
$$
E_1 \otimes_2 ... \otimes_2 E_n = (E_1 \otimes_2 ... \otimes_2 E_{n-1}) \otimes_2 E_n.
$$
したがって、スカラー 積の定義により、次のようになります。
$$
\langle x_1 \otimes ... \otimes x_n | y_1 \otimes ... \otimes y_n \rangle = \prod_{i=1}^n \langle x_i | y_i \rangle,
$$
特に$^1$
$$
\|x_1 \otimes ... \otimes x_n\|_2 = \|x_1\| \cdots \|x_n\|,
$$
$E_i$ ($1 \leq i \leq n$) の $x_i, y_i$ について。 $E_i$ がハウスドルフなら、$E_1 \otimes_2 ... \otimes_2 E_n$ も同様です。

$F_1, ..., F_n$ をプレヒルバーティアン空間とし、$u_i \in \mathscr{L}(E_i; F_i)$ を $1 \leq i \leq n$ とします。 $n$ の帰納法までに、提案します。 2 は、$u_1 \otimes ... \otimes u_n$ が $E_1 \otimes_2 ... \otimes_2 E_n$ から $F_1 \otimes_2 ... \otimes_2 F_n$ まで連続する線形写像であることを意味します。
$$
\|u_1 \otimes ... \otimes u_n\| = \|u_1\| \cdots \|u_n\|.
$$
$\sigma \in S_n$ を集合 $\{1, 2, ..., n\}$ の置換とします。 (6) により、線形写像 $p_\sigma$ が $E_1 \otimes_2 ... \otimes_2 E_n$ から $E_{\sigma^{-1}(1)} \otimes_2 ... \otimes_2 E_{\sigma^{-1}(n)}$ に特徴付けられます。
$$
p_\sigma(x_1 \otimes ... \otimes x_n) = x_{\sigma^{-1}(1)} \otimes ... \otimes x_{\sigma^{-1}(n)}
$$
プレヒルバーティアン空間同型 (「テンソル積の可換性」) です。

同様に、$\{1, 2, ..., n\}$の分割を、$1 \leq k \leq m$の$I_k = [a_k, a_{k+1} - 1]$と連続する区間$I_1, ..., I_n$を$m$と考えます。置く
$$
F_k = \bigotimes_{i=a_k}^{a_{k+1}-1} E_i \quad (1 \leq k \leq m).
$$

$^1$ ここでも$E_1 \otimes_2 ... \otimes_2 E_n$の$z$に$\|z\|_2 = \langle z|z \rangle^{1/2}$を入れます。

$F_1 \otimes ... \otimes F_m$ から $E_1 \otimes ... \otimes E_n$ への変換 $\bigotimes_{k=1}^{m} \bigotimes_{i=a_k}^{a_{k+1}-1} x_i$ から $x_1 \otimes ... \otimes x_n$ への標準同型 (A, II, § 3, No. 9) は、プレヒルバーティアン空間同型 (« テンソル積の結合性 ») です。

### 2. ヒルバーティアンテンソル積の ヒルバーティアン空間

#### 定義 1 {#evt-v-s3-def-1 .statement tag=080D}

$E_1, ..., E_n$ をヒルベルト空間とします。ハウスドルフプレヒルバーティアン空間* $E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$ の * 完成は、 $E_i$ のヒルバーティアンテンソル積と呼ばれ、 $E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$ (または $\hat{\otimes}_{2 \atop 1 \leq i \leq n} E_i$) で表されます。

$F_1, ..., F_n$ をヒルバーティアン空間とし、$u_i \in \mathscr{L}(E_i, F_i)$ を $1 \leq i \leq n$ とします。 $E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$ から $F_1 \hat{\otimes}_2 ... \hat{\otimes}_2 F_n$ まで、線形写像 $u_1 \otimes ... \otimes u_n$ から拡大するの連続線形写像 $u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n$ が続きます。私たちは持っています

$$
\|u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n\| = \|u_1\| ... \|u_n\|
$$

V、p. 27の公式 (8) 作。さらに、$1_E$ が任意のヒルバーシアン空間 $E$ の恒等写像を表す場合、次のようになります。

$$
1_{E_1} \hat{\otimes}_2 ... \hat{\otimes}_2 1_{E_n} = 1_E \quad \text{with} \quad E = E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n .
$$

最後に、$G_1, ..., G_n$ が $1 \leq i \leq n$ に対するヒルベルト空間と $v_i \in \mathscr{L}(F_i; G_i)$ である場合、次のようになります。

$$
(v_1 \circ u_1) \hat{\otimes}_2 ... \hat{\otimes}_2 (v_n \circ u_n) = (v_1 \hat{\otimes}_2 ... \hat{\otimes}_2 v_n) \circ (u_1 \hat{\otimes}_2 ... \hat{\otimes}_2 u_n) .
$$

プレヒルバーティアン空間について上で述べたことと同様に、ヒルバーティアンテンソル積の« 可換性 » と« 結合性» を定式化する作業は読者に委ねます。

#### 注意 {#evt-v-s3-n2-rem-1 .statement tag=080E}

$E_1, ..., E_n$ をハウスドルフプレヒルバーティアン空間とし、$\hat{E}_1, ..., \hat{E}_n$ をそれぞれの完成形とします。この場合、$E_1 \otimes_2 ... \otimes_2 E_n$ は $\hat{E}_1 \otimes_2 ... \otimes_2 \hat{E}_n$ のプレヒルバーティアン部分空間です。 $\hat{E}_1 \times ... \times \hat{E}_n$から$\hat{E}_1 \otimes_2 ... \otimes_2 \hat{E}_n$までの写像$(x_1, ..., x_n) \mapsto x_1 \otimes ... \otimes x_n$は連続なので、$\hat{E}_1 \otimes_2 ... \otimes_2 \hat{E}_n$では$E_1 \otimes_2 ... \otimes_2 E_n$が密です。 *なおさら* $E_1 \otimes_2 ... \otimes_2 E_n$ の完成はまさにヒルバート空間 $\hat{E}_1 \hat{\otimes}_2 ... \hat{\otimes}_2 \hat{E}_n$ です。この補完は、ときどき単に $E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$ (または $\hat{\otimes}_{2 \atop 1 \leq i \leq n} E_i$) と書かれます。

#### 命題 3 {#evt-v-s3-prop-3 .statement tag=080F}

$E_1, ..., E_n$ をヒルバーティアン空間とします。 $1 \leq i \leq n$ 空間 $E_i$ が、閉じたベクトル部分空間の族 $(E_{i,\alpha})_{\alpha \in A(i)}$ のヒルバーティアン和であるとします。次に、$E_1 \otimes_2 ... \otimes_2 E_n$ は、部分空間 $E_{1,\alpha_1} \hat{\otimes}_2 ... \hat{\otimes}_2 E_{n,\alpha_n}$ の族のヒルバーティアン和であり、$(\alpha_1, ..., \alpha_n)$ は $A(1) \times ... \times A(n)$ を超えます。

Vの公式(6)により、p. 27、部分空間 $E_1 \hat{\otimes}_2 ... \hat{\otimes}_2 E_n$の$E_{1,\alpha_1} \hat{\otimes}_2 ... \hat{\otimes}_2 E_{n,\alpha_n}$は相互に直交します。 1 から $n$ までの整数 $i$ ごとに、集合 $\bigcup_{\alpha \in A(i)} E_{i,\alpha}$ が $E_i$ に合計され、多重線形マッピング $(x_1, ..., x_n) \mapsto x_1 \otimes ... \otimes x_n$ は連続です。

したがって、部分空間 $E_{1,\alpha_1} \hat{\otimes}_2 ... \hat{\otimes}_2 E_{n,\alpha_n}$ の和集合は合計であるため、prop となります。 3.

#### 系 1 {#evt-v-s3-prop-3-cor-1 .statement tag=080G}

— $1 \leq i \leq n$ について、$(e_{i,\alpha})_{\alpha \in A(i)}$ を $E_i$ の正規直交値基底とします。この場合、$(\alpha_1, \ldots, \alpha_n)$ の範囲が $A(1) \times \cdots \times A(n)$ にわたるベクトル $e_{1,\alpha_1} \otimes \ldots \otimes e_{n,\alpha_n}$ の族は、$E_1 \hat{\otimes}_2 \ldots \hat{\otimes}_2 E_n$ の正規直交基底になります。

#### 系 2 {#evt-v-s3-prop-3-cor-2 .statement tag=080H}

— $E_1$ と $E_2$ を 2 ヒルベルト空間とし、$(e_i)_{i \in I}$ を $E_1$ の正規直交値基底とします。 $(y_i)_{i \in I}$ を $E_2$ の元の家族とし、$\sum_{i \in I} \| y_i \| ^2 < + \infty$ とします。すると、家族 $(e_i \otimes y_i)_{i \in I}$ は $E_1 \hat{\otimes}_2 E_2$ で要約可能です。さらに、$E_1 \otimes E_2$ のすべての元は、形 $\sum_{i \in I} e_i \otimes y_i$ と $\sum_{i \in I} \| y_i \| ^2 < + \infty$ で一意に書くことができます。

$F_i$ を、$e_i$ ($i \in I$) によって生成された $E_1$ の行とします。次に、$E_1$ は、部分空間 $(F_i)_{i \in I}$ の族のヒルバーティアン和です。プロップにより。 3、空間 $E_1 \hat{\otimes}_2 E_2$ は、部分空間 $(F_i \hat{\otimes}_2 E_2)_{i \in I}$ の族のヒルバーティアン和であるため、cor です。 2が続きます。

#### 例 1 {#evt-v-s3-n2-exa-1 .statement tag=080I}

コルによって。 1、空間 $\ell^2(I) \hat{\otimes}_2 \ell^2(J)$ は $\ell^2(I \times J)$ と正準同型で、$x = (x_i)_{i \in I}$ と $y = (y_j)_{j \in J}$ のテンソル積 $x \otimes y$ は族 $(x_i y_j)_{i \in I, j \in J}$ と識別できます。 同様に、cor. 2、ヒルバート空間 $E$ のすべての $y$ に対して $(x_i)_{i \in I} \otimes y = (x_i y)_{i \in I}$ が得られるように、$\ell^2(I) \hat{\otimes}_2 E$ は $\ell^2_E(I)$ と識別できます。

#### 例 2 {#evt-v-s3-n2-exa-2 .statement tag=080J}

\* $X$ をハウスドルフ トポロジカル空間とし、$\mu$ を $X$ の正の尺度とします。 $E$ をヒルバーティアン空間とします。 同一視できる $L^2(X, \mu) \hat{\otimes}_2 E$ と $L^2_E(X, \mu)$ を正規の方法で計算します。 : $f$ が $X$ 上の平方可積分スカラー 写像 $f$ の類であり、$a$ 属するである場合、 $E$ の場合、$f \otimes a$ は、$E$ に値が入った写像 $x \mapsto f(x).a$ の類です。

$Y$ をハウスドルフ トポロジカル空間とし、$\nu$ を $Y$ の正の測度とする。同様の方法で、ヒルバーティアン空間 $L^2(X, \mu) \hat{\otimes}_2 L^2(Y, \nu)$ と $L^2(X \times Y, \mu \otimes \nu)$ を同一視できるとします。その場合、$f \otimes g$ は、$X \times Y$ の写像 $(x, y) \mapsto f(x)g(y)$ の類と識別できます。 \*

### 3. 対称ヒルバーシアン冪

$E$ をヒルバーティアン空間とし、$n$ を正の整数とします。 $\hat{T}^n(E)$ または $E^{\hat{\otimes} n}$ が、それぞれ $E$ に等しい $n$ ヒルバーティアン空間のテンソル積を表すものとします。他の語では、$\hat{T}^n(E)$ は、によって定義されるハウスドルフ プレヒルベルト空間構造の空間 $T^n(E) = E \otimes \ldots \otimes E$ ($n$ 因子) の完成です。

$$
\langle x_1 \otimes \ldots \otimes x_n | y_1 \otimes \ldots \otimes y_n \rangle = \prod_{i=1}^n \langle x_i | y_i \rangle .
$$

$(e_i)_{i \in I}$ が $E$ の正規直交基底である場合、$I$ の $i_1, \ldots, i_n$ のベクトル $e_{i_1} \otimes \ldots \otimes e_{i_n}$ の族は、$\hat{T}^n(E)$ の正規直交基底 (V、p. 29、cor. 1)。 $\hat{T}^\circ(E) = K$ を取得します。

$\sigma \in S_n$ を集合 $\{ 1, 2, \ldots, n \}$ の置換とします。 V, p. 27 までに、以下の特徴を持つ $\hat{T}^n(E)$ の自己同型 $p_\sigma$ が存在します。

$$
p_\sigma(x_1 \otimes \ldots \otimes x_n) = x_{\sigma^{-1}(1)} \otimes \ldots \otimes x_{\sigma^{-1}(n)} .
$$

$\mathfrak{S}_n$ の $\sigma, \tau$ には $p_{\sigma \tau} = p_{\sigma} p_{\tau}$ があり、その結果、ベクトル空間 $\hat{\mathbf{T}}^n(E)$ の自己準同型 $\Pi_n = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} p_{\sigma}$ は、$\mathfrak{S}_n$ によって不変のまま残されたすべての元の部分空間へのオルソプロジェクターです。ただし、(A, III, § 6, No. 3)、$\Pi_n$ 写像は、位数 $n$ のすべての対称テンソルの部分空間 $\mathbf{TS}^n(E)$ に«代数» テンソル積 $\mathbf{T}^n(E)$ が加わります。他の語、$\Pi_n$の像は、$\mathbf{T}^n(E)$のスカラー積を備えた空間$\mathbf{TS}^n(E)$の完成です。この完了は $\widetilde{\mathbf{TS}}^n(E)$ で示されます。

$\mathbf{S}^n(E)$ をベクトル空間 $E$ (A, III, § 6, No. 1) の $n$ 番目の対称冪とします。 $\mathbf{T}^n(E)$ から $\mathbf{S}^n(E)$ への正準写像は、$\mathbf{TS}^n(E)$ から $\mathbf{S}^n(E)$ への同型写像 $\lambda_n$ を制限により定義します。 逆同型が次によって与えられることをすぐに検証します。

$$
\mu_n(x_1 \ldots x_n) = \Pi_n(x_1 \otimes \ldots \otimes x_n) = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} x_{\sigma^{-1}(1)} \otimes \ldots \otimes x_{\sigma^{-1}(n)}
$$

$E$の$x_1, \ldots, x_n$用。

私たちは、$\mathbf{S}^n(E)$ に定義するハウスドルフ プレヒルベルト派空間構造を置きます。

$$
\langle u|v \rangle = n! \langle \mu_n(u)|\mu_n(v) \rangle .
$$

次に、(A の公式 (29)、III, § 11, No. 5 と比較)

$$
\langle x_1 \ldots x_n|y_1 \ldots y_n \rangle = \sum_{\sigma \in \mathfrak{S}_n} \prod_{i=1}^n \langle x_i|y_{\sigma(i)} \rangle ,
$$

そして特に

$$
\langle x^n|y^n \rangle = n! \langle x|y \rangle^n .
$$

$\hat{\mathbf{S}}^n(E)$ はプレヒルバーシアン空間 $\mathbf{S}^n(E)$ と、$\hat{\mathbf{S}}(E)$ ヒルバーシアン空間 $\hat{\mathbf{S}}^n(E)$ の外部ヒルバーシアン和の完成を表すものとします。 代数 $\mathbf{S}(E)$ できないの乗法が連続性によって $\mathbf{S}(E)$, 〜でない限り $E$ に拡張されることを示すことができます (V、p. 73、練習問題 1)。

#### 命題 4 {#evt-v-s3-prop-4 .statement tag=080K}

*$(e_i)_{i \in I}$ をヒルバーシアン空間 $E$ の正規直交値基底とします。 $\mathbf{N}^{(I)}$ の $\alpha$ ごとに * を入れます

$$
z_{\alpha} = \prod_{i \in I} e_i^{\alpha_i}/(\alpha_i!)^{1/2} .
$$

*すると、$(z_{\alpha})_{\alpha \in \mathbf{N}^{(I)}}$ は $\hat{\mathbf{S}}(E)$ の正規直交基底になります。*

$E_0$ を、$I$ にわたる$i$ に対して、ベクトル $e_i$ によって生成された $E$ のベクトル部分空間とします。次に、ベクトル空間 $\mathbf{S}(E_0)$ の $z_{\alpha}$ 形基底 (A、III, § 6, No. 6)。しかし、$E_0$ は $E$ で密であり、$E \times \cdots \times E$ から $\mathbf{S}(E)$ までの多重線形写像 $(x_1, \ldots, x_n) \mapsto x_1 \ldots x_n$ はすべての $n \geqslant 1$ で連続です。したがって、$\mathbf{S}(E_0)$ は $\mathbf{S}(E)$ に密集しています。 $z_\alpha$ の族が正規直交であることを証明するにはこれで十分です。まず、$\hat{S}^n(E)$ と $\hat{S}^m(E)$ が $n \neq m$ に対して直交していることを観察します。したがって、公式を証明するだけで十分です

$$
\langle z_\alpha | z_\beta \rangle = \left\{ \begin{array}{ll}
1 & \text{if } \alpha = \beta \\
0 & \text{if } \alpha \neq \beta
\end{array} \right.
$$

$|\alpha| = \sum_{i \in I} \alpha_i$ と $|\beta| = \sum_{i \in I} \beta_i$ が同じ整数 $n$ に等しい場合。

集合 $\{ 1, 2, ..., n \}$ の分割 $(P_i)_{i \in I}$ が、すべての $i \in I$ に対してカード $P_i = \alpha_i$ になるように考えてください。 $k$ 属するを $P_i$ にしたら、$x_k = e_i$ を入れて、$x_1 ... x_n = \prod_{i \in I} e_i^{\alpha_i}$ とします。同様に、定義する $(Q_i)_{i \in I}$ と $y_k$ をカード $Q_i = \beta_i$ と $y_1 ... y_n = \prod_{i \in I} e_i^{\beta_i}$ になるようにします。 $e_i$ は相互に直交しているため、$k \in P_i$ と $\sigma(k) \in Q_i$ のようなインデックス $i \in I$ が存在する場合を除いて、$\langle x_k | y_{\sigma(k)} \rangle = 0$ になります。 公式 (15) により、$\langle x_1 ... x_n | y_1 ... y_n \rangle = 0$ 〜でない限りが得られ、すべての $i \in I$ に対して $\sigma(P_i) = Q_i$ となるような置換 $\sigma \in \mathfrak{S}_n$ が存在します。これは、$\alpha = \beta$ を意味します。次に、$\langle z_\alpha | z_\beta \rangle = 0$ が $\alpha \neq \beta$ になります。同じ議論は、$\| x_1 ... x_n \| ^2$ が $\sigma \in \mathfrak{S}_n$ の数に等しいこと、つまりすべての $i \in I$ に対して $\sigma(P_i) = P_i$ であるため、$\prod_{i \in I} \alpha_i !$ に等しいことが証明されます。 $\| z_\alpha \| = 1$ が得られ、命題が証明されます。

#### 系 {#evt-v-s3-n3-cor-1 .statement tag=080L}

— *ヒルバーシアン空間 E が直交部分空間 M と N の直和であるとします。 $S(M) \otimes S(N)$ から $S(E)$ (A, III, § 6, No. 6) 拡大するへのヒルバーシアン固有の標準同型 g $\hat{S}(M) \hat{\otimes}_2 \hat{S}(N)$ から $\hat{S}(E)$ まで、空間同型時間です。

$(e_i)_{i \in I}$ (それぞれ $(f_j)_{j \in J}$) をヒルバート空間 M (それぞれ N) の正規直交基底とし、$M_0$ (それぞれ $N_0$) をベクトルによって生成された E のベクトル部分空間とします。 $e_i$ (それぞれ $f_j$)。 $E_0 = M_0 + N_0$を置き、$g_0$を$S(M_0) \otimes S(N_0)$から$S(E_0)$に標準同型とします。置く

$$
z_\alpha = \prod_{i \in I} e_i^{\alpha_i}/(\alpha_i!)^{1/2}, \quad t_\beta = \prod_{j \in J} f_j^{\beta_j}/(\beta_j!)^{1/2}
$$

$\alpha \in \mathbf{N}^{(I)}$と$\beta \in \mathbf{N}^{(J)}$の場合。プロップにより。したがって、$\hat{S}(M)$ に対して正規直交基底 $(z_\alpha)_{\alpha \in \mathbf{N}^{(I)}}$、$\hat{S}(N)$ に対して$(t_\beta)_{\beta \in \mathbf{N}^{(J)}}$、$\hat{S}(E)$ に対して$(z_\alpha t_\beta)_{\alpha \in \mathbf{N}^{(I)}, \beta \in \mathbf{N}^{(J)}}$ を定義しました。 $z_\alpha t_\beta = g_0(z_\alpha \otimes t_\beta)$ があり、元 $z_\alpha \otimes t_\beta$ 形が $\hat{S}(M) \hat{\otimes}_2 \hat{S}(N)$ (V, p. 29, cor. 1) の正規直交基底であるため、$g_0$ 拡大するが a になることがわかります。ヒルバーティアン空間同型 $h : \hat{S}(M) \hat{\otimes}_2 \hat{S}(N) \to \hat{S}(E)$。 構成までに、

$$
h(x_1 ... x_m \otimes y_1 ... y_n) = x_1 ... x_m y_1 ... y_n
$$

$M_0$ のすべてのベクトル $x_1, ..., x_m$ と $N_0$ の $y_1, ..., y_n$ です。連続性により、同じ関係は M のベクトル $x_1, ..., x_n$ と N のベクトル $y_1, ..., y_n$ にも当てはまります。他には語、$h$、拡大する、$g$。 $h$の一意性はクリアです。

E と F を 2 つのヒルベルト空間と $u \in \mathscr{L}(E; F)$ とします。 $\hat{T}^n(E)$ から $\hat{T}^n(F)$ までの線形写像 $\hat{T}^n(u) = u \hat{\otimes}_2 ... \hat{\otimes}_2 u$ ($n$ 因子) は、ノルム $\|u\|^n$ (V, p. 28, 公式 (10)) と連続します。さらに、V, p. 30 の公式 (13) と (14) は、$\hat{S}^n(E)$ から $\hat{T}^n(E)$ の部分空間 $\widehat{T S^n}(E)$ までに同型 $\phi_{n,E}$ が存在することを示しています。

$$
(18) \quad \phi_{n,E}(x_1 \ldots x_n) = \frac{1}{(n!)^{1/2}} \sum_{\sigma \in \mathfrak{S}_n} x_{\sigma(1)} \otimes \ldots \otimes x_{\sigma(n)} \quad (x_1, ..., x_n \text{ in } E) .
$$

したがって、$\hat{S}^n(E)$ から $\hat{S}^n(F)$ まで連続する線形写像 $\hat{S}^n(u)$ が存在し、次の図式を可換にするものは 1 つだけです。

$$
\begin{array}{ccc}
\hat{S}^n(E) & \xrightarrow{\phi_{n,E}} & \hat{T}^n(E) \\
\downarrow \hat{S}^n(u) & & \downarrow \hat{T}^n(u) \\
\hat{S}^n(F) & \xrightarrow{\phi_{n,F}} & \hat{T}^n(F)
\end{array}
$$

公式を証明します

$$
(19) \qquad \| \hat{S}^n(u) \| = \| u \|^{n} .
$$

明らかに$\| \hat{S}^n(u) \| \leq \| \hat{T}^n(u) \| = \| u \|^{n}$ があります。さらに、すべての $x \in E$ に対して、$\hat{S}^n(u)(x^n) = u(x)^n, \| x^n \| = (n!)^{1/2} \| x \|^{n}$ と $\| u(x)^n \| = (n!)^{1/2} \| u(x) \|^{n}$ があり、次のようになります。

$$
\| \hat{S}^n(u) \| \cdot \| x \|^{n} \geq \| u(x) \|^{n} ;
$$

直ちに $\| \hat{S}^n(u) \| \geq \| u \|^{n}$ が続き、したがって公式 (19) になります。

公式があることは明らかです

$$
(20) \qquad \hat{S}^n(1_E) = 1_{\hat{S}_n(E)}
$$
$$
(21) \qquad \hat{S}^n(v \circ u) = \hat{S}^n(v) \circ \hat{S}^n(u) \quad \text{for} \quad v \in \mathscr{L}(F ; G) .
$$

最後に、A で定義された線形写像 $S^n(u) : S^n(E) \to S^n(F)$ を含む $S^n(E)$ の $\hat{S}^n(u)$ 一致するは、$E$ のすべての $x_1, ..., x_n$ に対して変換 $x_1 ... x_n$ が $u(x_1) ... u(x_n)$ になるため、III, § 6, No. 2 になります。

#### 例 1 {#evt-v-s3-n3-exa-1 .statement tag=080M}

$d \geq 1$ を整数とし、$\omega$ を $\mathbf{R}^d$ 上の正の写像とし、ルベーグ測度 $\mu$ に関して局所的に可積分します。 $E$ をヒルバーティアン空間 $L^2(\mathbf{R}^d, \omega.\mu)$ とし、$S = S(E)$ とします。次に、$S$ はすべての数列 $f = (f_n)_{n \geq 0}$ の空間と識別できます。ここで、各 $f_n$ は $(\mathbf{R}^d)^n$ 上の写像であり、これはルベーグ測度 $\mu \otimes ... \otimes \mu$ ($n$) に関して測定可能です因子) および $(\mathbf{R}^d)^n$ の $n$ 因子の置換の下で *不変量* であり、次のようなものです

$$
(22) \qquad \| f \|^{2} = \sum_{n=0}^{\infty} n! \int_{\mathbf{R}^d} ... \int_{\mathbf{R}^d} |f_n(x_1, ..., x_n)|^2 \omega(x_1) ... \omega(x_n) dx_1 ... dx_n
$$

有限です。 $S$ のノルム $\| f \|$ は、公式 (22) によって定義されます。上記で定義されたヒルバーティアン空間 $S$ は、*重み* $\omega$ に対する *対称フォック空間* 対応すると呼ばれます。

#### 例 2 {#evt-v-s3-n3-exa-2 .statement tag=080N}

$X$ をハウスドルフ トポロジカル空間、$\mu$ を $X$ 上のノルム 1 の正の測度、$E$ を実数ヒルバーティアン空間 $L^2_{\mathbf{R}}(X, \mu)$ のヒルバーティアン部分空間とします。次の同等の条件が満たされる場合、 $E$ は *ガウス空間* であると言います。

a) すべての $f \in E$ に対して、私たちは $\int_X e^{i f} d\mu = \exp(-\| f \|^{2}/2) ;$ を持っています

b) ノルム 1 を持つすべての $f \in E$ について、$f$ の下のメジャー $\mu$ の像がメジャーです
$$
(2\pi)^{-1/2}\ e^{-x^2/2} dx .
$$
$\mathbf{R}$に。

*$E$ がガウス空間であるとします。* $f_1, ..., f_n$ を写像とし、その類 $f_i$ 属するから $E$ とします。私たち定義する写像 : $f_1 ... f_n$ : X ($f_1, ..., f_n$の« Wick’s 積 » と呼ばれています) by 公式
$$
(23)\quad :f_1 ... f_n: = \sum_{0 \leq 2p \leq n} (-1)^p \sum_{\sigma \in I_p} \prod_{i=1}^p \langle f_{\sigma(2i-1)}|f_{\sigma(2i)} \rangle \prod_{j=2p+1}^n f_{\sigma(j)},
$$
ここで、$I_p$ は置換の集合 $\{1, 2, ..., n\}$ の $\sigma$ であり、次のようになります。
$$
\begin{align*}
&\sigma(1) < \sigma(2), ..., \sigma(2p-1) < \sigma(2p) \\
&\sigma(1) < \sigma(3) < ... < \sigma(2p-1) \\
&\sigma(2p+1) < \sigma(2p+2) < ... < \sigma(n).
\end{align*}
$$

次に、*$\hat{S}(E)$ *から* $L^2_R(X, \mu)$ のヒルバーシアン部分空間に *同型* $\phi$ が存在し、$\hat{S}(E)$ で計算された $f_1, ..., f_n$ の変換積 $f_1 ... f_n$ は、 $(:f_1 ... f_n:)$。 X がスースリン空間で、類属するから E までであり、X の点を分離する写像の可算家族 $(f_n)$ が存在するとします。すると、$\phi$は$\hat{S}(E)$から$L^2_R(X, \mu)$への同型です。 \*

### 4. 外装ヒルバーティアン冪

E をヒルバーティアン空間および $n$ 正の整数とします。すべての置換 $\sigma \in \mathfrak{S}_n$ について、$\varepsilon_\sigma$ がその署名を表します。 $a_n = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma p_\sigma$を$\mathscr{L}(\hat{T}^n(E))$(V、p. 29)に入れます。

$a_n$ がオルソ射影であるのは明らかで、その像 $\overline{\mathbf{A}'_n}(E)$ はすべての反対称位数 $n$ のテンソルの空間 $\mathbf{A}'_n(E)$ の $\hat{T}^n(E)$ における閉包です (A, III, § 7, No. 4)。 $\Lambda^n(E)$ から $\mathbf{A}'_n(E)$ まで同型 $\pi_n$ が存在します。
$$
(24)\quad \pi_n(x_1 \wedge ... \wedge x_n) = a_n(x_1 \otimes ... \otimes x_n) = \frac{1}{n!} \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma x_{\sigma(1)} \otimes ... \otimes x_{\sigma(n)}
$$
Eの$x_1, ..., x_n$用。 次のようにすることで、空間構造を$\Lambda^n(E)$ に定義するハウスドルフプレヒルバーティアンにすることができます。
$$
(25)\quad \langle u|v \rangle = n!\langle \pi_n(u)|\pi_n(v) \rangle .
$$
より明確に言うと、次のようになります (A の公式 (30)、III, § 11, No. 5 と比較してください)。
$$
(26)\quad \langle x_1 \wedge ... \wedge x_n|y_1 \wedge ... \wedge y_n \rangle = \det(\langle x_i|y_j' \rangle)
$$
E のすべての $x_1, ..., x_n$ と $y_1, ..., y_n$ について。

$\hat{\Lambda}^n(E)$ はプレヒルバーティアン空間 $\Lambda^n(E)$ の完成を表し、$\hat{\Lambda}(E)$ はヒルバーティアン空間 $\hat{\Lambda}^n(E)$ の外部ヒルバーティアン和を表すものとします。

#### 例 {#evt-v-s3-n4-exa-1 .statement tag=080O}

— *V、p. 32の例1の記法を使用して、同一視できるヒルバーシアン空間$\hat{\Lambda}(E)$を、すべての数列$(f_n)_{n \geq 0}$の測定可能な写像の集合とします。 (22) で定義された * 数 $\|f\|$ は有限であり、各写像 $f_n$ は *反対称*、つまり関係を満たします。

$$
f_n(x_{\sigma(1)}, ..., x_{\sigma(n)}) = \varepsilon_\sigma f_n(x_1, ..., x_n)
$$

置換 $\sigma \in \mathfrak{S}_n$ ごとに。ヒルバート空間 $\hat{\Lambda}(E)$ は、*重み* $\omega$ に対する *反対称フォック空間* 対応すると呼ばれます。 \*

#### 命題 5 {#evt-v-s3-prop-5 .statement tag=080P}

*$(e_i)_{i \in I}$ * をヒルバーシアン空間* E の正規直交基底とします。 *Endow* I * 完全に順序付けされた構造を使用します。次に、すべての元* $e_{i_1} \wedge ... \wedge e_{i_n}$ *for* $i_1 < ... < i_n$ * の集合は、* $\hat{\Lambda}^n(E)$ の基底です。

(A, III, § 7, No. 8) は、問題の元ベクトル空間 $\Lambda^n(E_0)$ の形基底が、$E_0$ がベクトル $e_i$ によって生成された E のベクトル部分空間であることを知っています。さらに、$i_1 < ... < i_n$ の場合、スカラー 積 $\langle e_{i_k}|e_{i_l} \rangle$ の行列は、位数 n の単位元行列です。 (26) までに、$\|e_{i_1} \wedge ... \wedge e_{i_n}\| = 1$ が得られます。最後に、$(i_1, ..., i_n)$ と $(j_1, ..., j_n)$ が 2 つの異なるもの、つまり I の元の真に増加する数列である場合、$i_1, ..., i_n$ とは異なる元 $j_\ell$ が存在するため、$1 \leq k \leq n$ に対して $\langle e_{i_k}|e_{j_\ell} \rangle = 0$ が得られます。そして (26) までに、$\langle e_{i_1} \wedge ... \wedge e_{i_n}|e_{j_1} \wedge ... \wedge e_{j_n} \rangle = 0$。他の語では、$i_1 < ... < i_n$ の元 $e_{i_1} \wedge ... \wedge e_{i_n}$ の族は正規直交です。

しかし、$E_0$はEで密であり、$E \times \cdots \times E$から$\Lambda^n(E)$までの写像$(x_1, ..., x_n) \mapsto x_1 \wedge ... \wedge x_n$は連続です。その結果、$\Lambda^n(E)$には$\Lambda^n(E_0)$が密集し、命題5が続きます。

#### 系 {#evt-v-s3-n4-cor-1 .statement tag=080Q}

*ヒルバーシアン空間* E * が 2 つの直交部分空間* M * と* N の直和であるとします。 *標準同型* g *from* $\Lambda(M) \otimes \Lambda(N)$ *onto* $\Lambda(E)$ *(A, III, § 7, No. 7)* *拡大する inヒルバーティアン空間同型から* $\hat{\Lambda}(M) \hat{\otimes}_2 \hat{\Lambda}(N)$ *から* $\hat{\Lambda}(E)$ へのユニークな方法。

証明はプロップの系に類似しています。 4 (V、p. 31)。

E と F を 2 つのヒルベルト空間と $u \in \mathscr{L}(E; F)$ とします。対称冪 $\hat{S}^n(E)$ (V, p. 32) の場合のように、$\hat{\Lambda}^n(E)$ から $\hat{\Lambda}^n(F)$ (A, III, § 7, No. 4) 拡大するへ線形写像 $\hat{\Lambda}^n(u)$ が連続になることを示します。 線形写像 $\hat{\Lambda}^n(u)$ $\hat{\Lambda}^n(E)$ から $\hat{\Lambda}^n(F)$ へ。 関係あります

$$
\hat{\Lambda}^n(1_E) = 1_{\hat{\Lambda}^n(E)} , \tag{27}
$$
$$
\hat{\Lambda}^n(v \circ u) = \hat{\Lambda}^n(v) \circ \hat{\Lambda}^n(u) \quad \text{if } v \text{ belongs to } \mathscr{L}(F; G) , \tag{28}
$$
$$
\|\hat{\Lambda}^n(u)\| \leq \|u\|^n . \tag{29}
$$

一般に、公式 (29) (TS、IV, § 6) には等式はありません。最後に、$\hat{\Lambda}^n(E)$ から $\hat{T}^n(E)$ の部分空間 $\overline{\mathbf{A}}'_n(E)$ への同型 $\psi_n = \psi_{n,E}$ が次のように定義されます。

$$
\psi_n(x_1 \wedge ... \wedge x_n) = \frac{1}{(n!)^{1/2}} \sum_{\sigma \in \mathfrak{S}_n} \varepsilon_\sigma x_{\sigma(1)} \otimes ... \otimes x_{\sigma(n)} . \tag{30}
$$

### 5. 外観乗法

E をヒルバーティアン空間とします。 整数 $n \geqslant 0$ ごとに、$\theta_n$ を $T^n(E)$ から $\Lambda^n(E)$ まで標準写像とします。それから

$$
\theta_n(x_1 \otimes \ldots \otimes x_n) = x_1 \wedge \ldots \wedge x_n
$$

E の $x_1, \ldots, x_n$ について。$p$ と $q$ を 2 つの正の整数とします。 公式 (30) と (31) のおかげで、

$$
u \wedge v = \theta_{p+q}\left( \frac{1}{(p!)^{1/2}} \psi_p(u) \otimes \frac{1}{(q!)^{1/2}} \psi_q(v) \right)
$$

$u \in \Lambda^p(E)$と$v \in \Lambda^q(E)$の場合。 $\| \theta_n \| \leq (n!)^{1/2}$ なので、不等式になります。

$$
\| u \wedge v \| \leq \left( \frac{(p+q)!}{p! \ q!} \right)^{1/2} \| u \| \cdot \| v \|
$$

$u \in \Lambda^p(E)$ と $v \in \Lambda^q(E)$ の場合。その結果、$\hat{\Lambda}^p(E) \times \hat{\Lambda}^q(E)$ から $\hat{\Lambda}^{p+q}(E)$ までの双線形写像への連続性により写像 $(u, v) \mapsto u \wedge v$ 拡大するとなり、ノルムは最大でも $\left( \frac{(p+q)!}{p! \ q!} \right)^{1/2}$ (cf. V, p. 73, 2）を実行します。これを再び$(u, v) \mapsto u \wedge v$で表します。

#### 命題 6 {#evt-v-s3-prop-6 .statement tag=080R}

*E をヒルバーティアン空間とします。我々は持っています*

$$
\| x \wedge u \| \leq \| x \| \cdot \| u \|
$$

* $x \in E$ * および* $u \in \hat{\Lambda}(E)$ 用。

$\| x \| = 1$ の場合を考慮するだけで十分であることは明らかです。

F を、x に直交するすべてのベクトルの E からなるのヒルベルト部分空間とします。 E は F と直線 K.x のヒルバーティアン和であるため、V、p. 34 の系から、写像 $(v, w) \mapsto v + x \wedge w$ は $\hat{\Lambda}(F) \oplus \hat{\Lambda}(F)$ から空間同型のヒルバーティアンであることがわかります。 $\hat{\Lambda}(E)$。 $\hat{\Lambda}(F)$ に $v, w$ がある $u = v + x \wedge w$ の場合、$x \wedge u = x \wedge v$ があり、従って $\| x \wedge u \| = \| v \| \leq (\| v \|^2 + \| w \|^2)^{1/2} = \| u \|$ になります。

#### 系 1 {#evt-v-s3-prop-6-cor-1 .statement tag=080S}

*a)* *$x_1, \ldots, x_n$ *をヒルバート空間* の元とします。 *私たちは*

$$
\| x_1 \wedge \ldots \wedge x_n \| \leq \| x_1 \| \ldots \| x_n \|,
$$

*ここで、等式は、* $x_i$ * の 1 つが null である場合、または数列* $(x_1, \ldots, x_n)$ * が直交している場合にのみ成立します。

*b)* *$x_1, \ldots, x_n, y_1, \ldots, y_n$ *をヒルバート空間* の元とします。 *私たちは*

$$
|\det(\langle x_i, y_j \rangle)| \leq \| x_1 \| \ldots \| x_n \| \cdot \| y_1 \| \ldots \| y_n \|;
$$

ベクトル $x_i$ および $y_i$ が null でない場合。 等式は、$(x_1, ..., x_n)$ と $(y_1, ..., y_n)$ がそれぞれ E の同じベクトル部分空間の直交基底である場合に限り、(36) で成り立ちます。

不等式 (35) はプロップから続きます。 6 by 帰納法 、$n$; 不等式 (36) は、$\Lambda^n(E)$ の適用コーシー・シュワルツ不等式と V、p. 33 の公式 (26) によって演繹できます。

数列 $(x_1, ..., x_n)$ が直交しているとします。それから

$$
\| x_1 \wedge ... \wedge x_n \|^2 = \det(\langle x_i | x_j \rangle) = \prod_{i=1}^n \| x_i \|^2
$$

$\langle x_i | x_j \rangle = 0$ から $i \neq j$ まで。

ここで、ベクトル $x_1, ..., x_n$ は null ではなく、形は直交数列ではないと仮定します。 $\| x_1 \wedge ... \wedge x_n \|$ はベクトル $x_1, ..., x_n$ に対称的に依存するため、$x_1$ は $x_2, ..., x_n$ によって生成される E の部分空間 F に直交せず、F は単純に 0 ではないと仮定できます。 $x_1$ を形 $x'_1 + y$ で分解できます。 Fの$y \neq 0$とFに直交する$x'_1$。次に$\| x'_1 \| < \| x_1 \|$。しかし

$$
x_1 \wedge x_2 \wedge ... \wedge x_n = x'_1 \wedge x_2 \wedge ... \wedge x_n,
$$

など

$$
\begin{align*}
\| x_1 \wedge ... \wedge x_n \| &\leq \| x'_1 \| \| x_2 \| ... \| x_n \| \\
&< \| x_1 \| \| x_2 \| ... \| x_n \|.
\end{align*}
$$

ベクトル $x_i$ とベクトル $y_i$ が null ではないとします。 関係 (36) の等式は等式の結合に相当します

(37) $$ |\langle x_1 \wedge ... \wedge x_n | y_1 \wedge ... \wedge y_n \rangle| = \| x_1 \wedge ... \wedge x_n \| \cdot \| y_1 \wedge ... \wedge y_n \| $$

(38) $$ \| x_1 \wedge ... \wedge x_n \| = \| x_1 \| ... \| x_n \| , \quad \| y_1 \wedge ... \wedge y_n \| = \| y_1 \| ... \| y_n \| . $$

証明の最初の部分によって、等式 (38) は、数列 $(x_1, ..., x_n)$ と $(y_1, ..., y_n)$ がそれぞれ直交していることを意味し、それは今度は $x_1 \wedge ... \wedge x_n \neq 0$ と $y_1 \wedge ... \wedge y_n \neq 0$ を意味します。これらの条件、関係 (37) は、$y_1 \wedge ... \wedge y_n = \lambda x_1 \wedge ... \wedge x_n$ (V, p. 3, 注意 1) のようなスカラー $\lambda \neq 0$ が存在することを意味します。他の語では、$(x_1, ..., x_n)$と$(y_1, ..., y_n)$はE(A、III, § 11, No. 13)の同じベクトル部分空間の基底です。

#### 系 2 {#evt-v-s3-prop-6-cor-2 .statement tag=080T}

— $(a_{ij})_{1 \leq i,j \leq n}$ をエルミート行列、複素数元、および行列式 D とします。不等式と仮定します。

$$
\sum_{i,j=1}^n a_{ij} \overline{z}_i z_j \geq 0
$$

すべての複素数 $z_1, ..., z_n$ に当てはまります。それから

$$
0 \leq D \leq a_{11} ... a_{nn}.
$$

D が null ではないとします。 等式 $D = a_{11} ... a_{nn}$ は、すべての $i \neq j$ に対して $a_{ij} = 0$ である場合にのみ成立します。

ベクトル空間 $\mathbf{C}^n$ で、$\Phi$ をエルミート形とします。

$$
\Phi(\mathbf{z}, \mathbf{z}') = \sum_{i,j=1}^n a_{ij} \overline{z}_i z'_j
$$

$\mathbf{C}^n$の$\mathbf{z} = (z_1, ..., z_n)$と$\mathbf{z}' = (z'_1, ..., z'_n)$用。 仮定までに、$\Phi$はプラスになります。

まず、$\Phi$ が分離している、つまり D が null ではないと仮定します。 $(e_1, ..., e_n)$ が $\mathbf{C}^n$ の標準基底である場合、$\Phi(e_i, e_j) = a_{ij}$ と cor が得られます。 2 は cor の直後に続きます。 1、a) $x_i = e_i$ を入れます。

$a_{ii} = \Phi(e_i, e_i) \geq 0$なので、$D = 0$なら不等式(40)もあります。

#### 系 3 (« アダマールの不等式 ») {#evt-v-s3-prop-6-cor-3 .statement tag=080U}

— $(a_{ij})_{1 \leq i, j \leq n}$ を行列と複素数元および行列式 D とします。

$$
c_i = \left( \sum_{j=1}^n |a_{ij}|^2 \right)^{1/2} \quad \text{for} \quad 1 \leq i \leq n,
$$

そして$m = \sup_{i,j} |a_{ij}|$。それでは、

$$
|D| \leq c_1 ... c_n \leq m^n \cdot n^{n/2}.
$$

$D \neq 0$ の場合、$|D| = c_1 ... c_n$ の位数では、行列 $(a_{ij})_{1 \leq i, j \leq n}$ の行 $y_i = (a_{ij})_{1 \leq j \leq n}$ が 2 × 2 直交するベクトルであることが必要かつ十分です。

空間 $\mathbf{C}^n$ に、次のように定義されるスカラー 積を割り当てます。

$$
\langle \mathbf{z}|\mathbf{z}' \rangle = \sum_{i=1}^n \overline{z}_i z'_i.
$$

$(\mathbf{x}_1, ..., \mathbf{x}_n)$を$\mathbf{C}^n$の標準基底と$\mathbf{y}_i$ベクトルとし、$1 \leq j \leq n$を成分$a_{ij}$とします。 $1 \leq i \leq n$には$\| \mathbf{x}_i \| = 1$と$\| \mathbf{y}_i \| = c_i$があります。 $\langle \mathbf{x}_i|\mathbf{y}_j \rangle = a_{ji}$も。 不等式 $|D| \leq c_1 ... c_n$ と等式の条件は、V、p. 35、cor の特殊なケースになります。 1. 明らかに $c_i \leq m \cdot n^{1/2}$ があるため、$c_1 ... c_n \leq m^n \cdot n^{n/2}$ になります。

### 練習問題 {#evt-v-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
