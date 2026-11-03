---
book: int
book_title: Integration
chapter: IV
chapter_title: EXTENSION OF A MEASURE. LP SPACES
section: 6
section_title: Convexity inequalities
lang: ja
source: int-i-vi
book_pages: INT IV.89-INT IV.100, INT IV.134-INT IV.142
pdf_pages: 0196-0207, 0241-0249
extraction: ocr
subsections:
    - "no": 1
      title: The convexity theorem
      page: 89
      pdf_page: 196
    - "no": 2
      title: Inequality of the mean
      page: 90
      pdf_page: 197
    - "no": 3
      title: The spaces $L^\infty_F$
      page: 91
      pdf_page: 198
    - "no": 4
      title: Hölder’s inequality
      page: 93
      pdf_page: 200
    - "no": 5
      title: 'Application: relations between the spaces $L^p_F$ ($1 \leq p \leq +\infty$)'
      page: 98
      pdf_page: 205
statements: 22
exercises: 20
content_sha256: 8b7f38b5f3dd5ae902fc5cacb81ca06fadf1056f7ffb4f0a9799e479f53b7727
translated_from: content/en/int/IV/06_s6_convexity_inequalities.md
translation_method: google
source_content_sha256: 5da8e094f0389b678ca69f52f247e8417940837f7695de9c80ebdf9dcbcce321
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: b6d931767a0cc0363c041b3b5bc327c35c27ec3ab05478a75d450d155c4a573d
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 6。凸不等式

### 1. 凸性定理

#### 定理 1 {#int-iv-s6-thm-1 .statement tag=08XD}

— $X$ を局所コンパクト空間、$\mu$ を $X$ の正の測度、$F$ を実際の Banach 空間、$D$ を $F$ の閉じた凸型集合、および $f$ 写像とします。 $X$ では $f(X) \subset D$ になります。 $fg$ が可積分であるような無視できない積分可能な数値写像 $g \geqslant 0$ については、点 $\frac{\int fg\, d\mu}{\int g\, d\mu}$ 属するから $D$ になります。

なぜなら、$F'$ を $F$ の双対とし、$\langle z, a' \rangle \leqslant \alpha$ ($a' \in F', \alpha \in \mathbf{R}$) を閉じた半空間含む $D$ を定義する関係とします。 $fg$ は可積分であるため、数値写像 $\langle fg, a' \rangle = \langle f, a' \rangle g$ も可積分です、そして

$$
\int \langle fg, a' \rangle\, d\mu = \left\langle \int fg\, d\mu, a' \right\rangle
$$

(§ 4, No. 2、Th. 1 のコリント 1);しかし、仮定までに、すべての $x \in X$ に対して $\langle f(x), a' \rangle \leqslant \alpha$ となるため、$\langle f(x)g(x), a' \rangle \leqslant \alpha g(x)$ になります。統合に関しては、

$$
\left\langle \int fg\, d\mu, a' \right\rangle \leqslant \alpha \int g\, d\mu .
$$

これは、すべての閉じたハーフスペース含む $D$ に対して点 $\frac{\int fg\, d\mu}{\int g\, d\mu}$ 属するであることを証明します。しかし、ハーン・バナッハ定理によれば、$D$ は閉じたハーフスペース含むの共通部分 (TVS、II, §5, No. 3、提案 4 の Cor. 1)、よって定理です。

#### 系 {#int-iv-s6-n1-cor-1 .statement tag=08XE}

— *正の尺度 $\mu$ の総質量が 1 に等しい場合、および $f$ が可積分である場合、$F$* の$f(X)$ の閉じた凸包絡線に $\int f\, d\mu$ 属するを加えます。

$g$ には定数写像 1 をとれば十分です。

### 2. 平均値の不等式

Thを研いでいきます。 1 は数値的に測定可能な写像 (有限であるかどうか)。

#### 定義 1 {#int-iv-s6-def-1 .statement tag=08XF}

— X を局所的にコンパクトな空間、$\mu$ を X 上のメジャーとします。 X のほぼどこでもローカルに定義されている数値写像 f (有限であるかどうか) が与えられると、写像 f の測定値の最大値、または $\mu$-最大値 (それぞれ測定値の最小値、または $\mu$-最小値) と呼ばれ、$M_\infty(f)$ (それぞれ $m_\infty(f)$) で表されます。 数 $\alpha$ の集合の下限 (または上限) は、局所的にほぼどこでも ($\mu$ の場合) $f(x) \leq \alpha$ (または $f(x) \geq \alpha$) になります。

定義からはすぐに $m_\infty(f) = -M_\infty(-f)$ が得られ、したがって、小節内の最大値の性質ごとに、小節内の最小値の対応する性質が推定されます。

$x \in X$ のすべての $\alpha > M_\infty(f)$、集合について、$f(x) > \alpha$ は局所的に無視できます。今、$x \in X$の集合は、$f(x) > M_\infty(f)$が集合の和集合で、$f(x) > r_n$で、$r_n$が有理数数$> M_\infty(f)$の集合を超えています。したがって、ほぼどこでもローカルに $f(x) \leq M_\infty(f)$ (§ 5, No. 2) になります。同様に、ほとんどどこでもローカルに$f(x) \geq m_\infty(f)$。 $\mu$ の尺度が非零であれば、$m_\infty(f) \leq M_\infty(f)$ になります。さらに、関係 $m_\infty(f) = M_\infty(f)$ はというと等価であり、$f$ は局所的にほぼどこでも定数と等しくなります。メジャー $\mu$ が非零である場合、次のことが明らかです。

$$
\inf_{x \in X} f(x) \leq m_\infty(f) \leq M_\infty(f) \leq \sup_{x \in X} f(x).
$$

2 つの写像 $f, g$ がほぼどこでも局所的に等しい場合、$m_\infty(f) = m_\infty(g)$ と $M_\infty(f) = M_\infty(g)$ になります。

最後に、$f$ と $g$ が 2 つの写像で、$f + g$ がほぼどこでもローカルに定義される場合、次のようになります。

(1)
$$
M_\infty(f + g) \leq M_\infty(f) + M_\infty(g)
$$
2 番目のメンバーが定義されている場合、定義からすぐに次のようになります。 1;同様に、$f$ と $g$ が両方とも $\geq 0$ で、ほぼどこでも $fg$ がローカルに定義されるような場合、

(2)
$$
M_\infty(fg) \leq M_\infty(f) M_\infty(g)
$$
ただし、2 番目のメンバーが定義されている場合に限ります。

$M_\infty(f) < +\infty$ の場合、ほぼどこでもローカルに $f(x) < +\infty$ になりますが、必ずしもほぼどこでもというわけではありません。数値写像 $f$ は、それがほぼどこでも定義されて有限である場合、さらに、数 $m_\infty(f)$ と $M_\infty(f)$ が両方とも有限である場合 (後者の条件はというに相当します) は、(メジャー $\mu$ の場合) メジャーで有界であると言われます。 $M_\infty(|f|) < +\infty$）。

#### 命題 1 (平均値の不等式) {#int-iv-s6-prop-1 .statement tag=08XG}

— *f を測定範囲内にある測定可能な数値写像とします。すべての可積分数値写像 $g \geqslant 0$、写像 $fg$ (ほぼどこでも定義されている) は可積分可能であり、*

$$
m_\infty(f) \int g d|\mu| \leqslant \int fg d|\mu| \leqslant M_\infty(f) \int g d|\mu|.
$$

さらに、*不等式 (3) できないの 3 つのメンバーのうち 2 つは 〜でない限りに等しく、$x \in X$ の集合では、$g(x) \neq 0$、f はほぼどこでも $M_\infty(f)$ に等しいか、ほぼどこでも $m_\infty(f)$ に等しい*。

確かに、$fg$ は測定可能です (§ 5, No. 3、Th. 1 のコリント 5)。 moreover, 不等式 $m_\infty(f)g(x) \leqslant f(x)g(x) \leqslant M_\infty(f)g(x)$ holds, not only locally almost everywhere, but even almost everywhere, because 集合 of 点 $x \in X$ where $g(x) \neq 0$ is a countable 和集合 of integrable 集合 (§ 5, No. 6, 補題 1)。したがって、$fg$ は可積分 (§ 5, No. 6, Th. 5) であり、不等式 (3) が成り立ちます。一方、写像 $M_\infty(f)g - fg$ はほぼどこでも定義されており、$(M_\infty(f) - f)g$ と同等です。したがって、$X$ のほぼどこでも $\geqslant 0$ です。 関係 $M_\infty(f) \int g d|\mu| = \int fg d|\mu|$ は $\int (M_\infty(f) - f)g d|\mu| = 0$ と等しいため、写像 $(M_\infty(f) - f)g$ が無視できる場合にのみ成立し、証明が完成します。

設定 $\int g d|\mu| = 0$、不等式 (3) が Th から演繹される可能性があるという自明なケースは別として。 No. 1 の 1 が区間 $D = [m_\infty(f), M_\infty(f)]$ に適用されます。 Thに持っていくことができます。 No. 1 の 1 は、提案 1 の補数に類似しており、点 $(\int fg d\mu)/(\int g d\mu)$ 属するが D の境界にある場合を指定します (例 2)。

### 3. 空間 $L^\infty_F$

#### 定義 2 {#int-iv-s6-def-2 .statement tag=08XH}

*$X$ の写像 $f$ を Banach 空間 $F$ に変換するごとに、集合 $N_\infty(f) = M_\infty(|f|)$ が 1 つずつ追加されます。 $N_\infty(f)$ が有限である場合、$f$ は (メジャー $\mu$ に対して) メジャーが有界であると言われます。 $X$ の写像から $F$ までの集合は、測定可能で測定範囲が制限されているもので、$\mathscr{L}_F^\infty(X, \mu)$ (または $\mathscr{L}_F^\infty(\mu)$、または単に $\mathscr{L}_F^\infty$) と表されます。

したがって、$\mathscr{L}_F^\infty$ の写像 $f$ は、$f$ とほぼどこでも局所的に等しい*有界可測* 写像が存在するという事実によって特徴付けられる可能性があります。

(1) からすぐに次のことがわかります。

$$
N_\infty(f + g) \leqslant N_\infty(f) + N_\infty(g);
$$

一方、すべてのスカラー $\alpha$ に対して $N_\infty(\alpha f) = |\alpha| N_\infty(f)$ です。したがって、集合 $\mathscr{L}_F^\infty$ は、$X$ のすべての写像から $F$ への空間の *線形部分空間* であり、$N_\infty(f)$ はこのベクトル空間の準ノルムです。 $(f_n)$ を、半ノルム $N_\infty(f)$ で定義される位相に対して $f \in \mathscr{L}_F^\infty$ に収束する $\mathscr{L}_F^\infty$ の写像の数列とします。 整数 $m$ ごとに、局所的に無視できる集合 $H_m$ と整数 $n_0$ が存在し、整数 $n \geq n_0$ および$x \notin H_m$ ごとに $|f(x) - f_n(x)| \leq 1/m$ が存在します (可算すべて) 和集合は局所的に無視できる集合は局所的に無視できる）。 $H_m$ の和集合 $H$ は局所的に無視でき、$f_n(x)$ は局所的に無視できる集合 $H$ の補数で *一様に $f(x)$ になる傾向があることがわかります。 逆は明らかです。

すべての写像が、$\mathscr{L}_F^\infty$ 属するから $\mathscr{L}_F^\infty$ まで、局所的にほぼどこでも写像に等しいことは明らかです。特に、$F$ 形の値を使用して $X$ で定義された *局所的に無視できる* 写像は、関係 $N_\infty(f) = 0$ によって特徴付けられる、$\mathscr{L}_F^\infty$ の線形部分空間 $\mathscr{N}_F^\infty$ ( 位相は $N_\infty(f)$ によって定義されます）。 $\mathscr{L}_F^\infty$ に関連付けられたハウスドルフ空間、つまり商空間 $\mathscr{L}_F^\infty / \mathscr{N}_F^\infty$ は、$L_F^\infty(X, \mu)$ (または $L_F^\infty(\mu)$ または $L_F^\infty$) で表されます。その位相は、$N_\infty$ から商への経過によって推定される *ノルム* によって定義されます。 類 $\dot{f} \in L_F^\infty$ のノルムは、$N_\infty(\dot{f})$、または $\| \dot{f} \|_\infty$ と表されます。 $F = \mathbf{R}$ (それぞれ $\mathbf{C}$) の場合、混乱が生じない限り、$\mathscr{L}_\mathbf{R}^\infty$ と $L_\mathbf{R}^\infty$ (それぞれ $\mathscr{L}_\mathbf{C}^\infty$ と $L_\mathbf{C}^\infty$) の代わりに $\mathscr{L}^\infty$ と $L^\infty$ と書きます。

#### 命題 2 {#int-iv-s6-prop-2 .statement tag=08XI}

*空間* $\mathscr{L}_F^\infty$ *完了です。 空間* $L_F^\infty$ * はバナッハ空間* です。

というのは、$(f_n)$ を $\mathscr{L}_F^\infty$ の Cauchy 数列とします。 整数 $n$ ごとに、$r \geq k_n$ と $s \geq k_n$ に対して $N_\infty(f_r - f_s) \leq 1/n$ となるような整数 $k_n$ が存在します。したがって、すべての $x \notin A_{rs}$ に対して $|f_r(x) - f_s(x)| \leq 1/n$ となるような、局所的に無視できる集合 $A_{rs}$ が存在します。 $A_n$ が集合 $A_{rs}$ の和集合である場合 ($r \geq k_n$ と $s \geq k_n$ の場合)、$A_n$ は局所的に無視でき、すべての $x \notin A_n$ について、すべての添字 $r \geq k_n, s \geq k_n$ について$|f_r(x) - f_s(x)| \leq 1/n$ になります。 Let $A$ be the locally negligible set formed by the union of the $A_n$, and set $g_n(x) = f_n(x)$ for $x \notin A$, $g_n(x) = 0$ for $x \in A$; then $g_n$ belongs to $\mathscr{L}_F^\infty$ and, by the definition of $A$, the sequence $(g_n)$ converges *uniformly* on $X$ to a function $g$. したがって、写像 $g$ は測定可能です (§ 5, No. 4、Th. 2)。さらに、$g$ は $|g_{k_1}(x)| \leq N_\infty(g_{k_1})$ の $x \in X$ の集合で境界があり、この集合の補数が局所的に無視できるため、$g$ 属するから $\mathscr{L}_F^\infty$ になります。 $\mathscr{L}_F^\infty$ では、数列 $(g_n)$ には極限 $g$ があることは明らかであり、したがって、すべての $n$ について $N_\infty(f_n - g_n) = 0$ であるため、数列 $(f_n)$ にも同じことが当てはまります。 命題の 2 番目の部分は、これからすぐに推測できます。

#### 注意 {#int-iv-s6-n3-rem-1 .statement tag=08XJ}

— 1) $F$ 属するから $\mathscr{L}_F^\infty$ までの値を含む、$X$ のすべての*有界連続* 写像 $f$、および

$$
N_\infty(f) \leq \| f \| = \sup_{x \in X} |f(x)| .
$$

すべての有界連続写像 $f$ に対して $N_\infty(f) = \|f\|$ である位数では、測度 $\mu$ のサポートが $X$ に等しいことが必要かつ十分です。というのは、無視できるほどコンパクトなサポートを伴う継続的な写像 $f$ が存在し、同一の零ではない場合、$N_\infty(f) = 0$ と $\|f\| > 0$ です。逆に、$\mu$ のサポートが $X$ に等しい場合、すべての有界連続写像 $f$ およびすべての数 $\alpha < \|f\|$、$x \in X$ の集合について、$|f(x)| > \alpha$ がオープンで、空でないが外側になるため、 $> 0$ を測定すると、$N_\infty(f) = \|f\|$ であることがわかります。

$\mu$ のサポートが $X$ に等しい場合、$X$ で有界連続写像 、$F$ で値 、空間の部分空間の正規化空間 $C^b(X; F)$ を同一視するとすることができます。 $L_F^\infty$。 $L_F^\infty$ は一般にハウスドルフではないため、部分空間 $C^b(X; F)$ は一般に $L_F^\infty$ で閉じられていませんが、$L_F^\infty$ の標準像は $L_F^\infty$ の閉じた部分空間です (さらに、考えられているケースでは $C^b(X; F)$ と識別できます)。 一般に、$C^b(X; F)$ は $L_F^\infty$ とは異なります。つまり、任意の有界可測写像 $f$ に対して、局所的にほぼどこでも $f$ に等しい連続的な写像 $g$ は一般に存在しません (§ 5、Exer. 12)。 これは、$X$ の写像から $F$ への空間 $\mathscr{H}(X; F)$ は、コンパクトなサポートで連続しており、$L_F^\infty$ では一般に稠密ではないが、$1 \leq p < +\infty$ (§ 3, No. 4) の空間 $L_F^p$ のそれぞれでは稠密であることを意味します。 デフ。 2)。

2) 準ノルム$N_\infty$によって定義される位相が、尺度収束(§ 5, No. 11)の位相によって$L_F^\infty$に誘導される位相よりもより細かいとなる明らかです。

### 4. ヘルダーさん不等式

この番号では、$p$ と $q$ は 2 つの実数を表し、$1 \leq p \leq +\infty$、$1 \leq q \leq +\infty$ が関係 $1/p + 1/q = 1$ によって結合されます。したがって、$1 < p < +\infty$の場合は$q = p/(p-1)$、$p = 1$の場合は$q = +\infty$、$p = +\infty$の場合は$q = 1$になります。 $p$ と $q$ は共役指数と呼ばれます。 関係 $1 \leq p \leq 2$ は $2 \leq q \leq +\infty$ と同等であることに注意してください。 $p = q$は、$p$と$q$が2に等しい場合のみです。

#### 定理 2 (ヘルダーの不等式) {#int-iv-s6-thm-2 .statement tag=08XK}

— $f$ と $g$ を 2 つの数値写像とします。これらはほぼどこでも有限であり、$f$ はほぼどこでも $L^p$ の写像に、$g$ から $L^q$ の写像に等しくなります。次に、写像 $fg$ (ほぼどこでも定義されている) は可積分可能であり、

$$
N_1(fg) \leq N_p(f) N_q(g).
$$

$f_1$ (それぞれ $g_1$) が $L^p$ (それぞれ $L^q$) の写像であるとします。これにほぼどこでも $f$ (それぞれ $g$) が等しくなります。 $fg$ は、ほとんどどこでも写像 $f_1 g_1$ に等しく、これはどこでも定義され有限であり、測定可能であり、測定可能な 2 つの写像のうちの積 (§ 5, No. 3、コリント 1 章 5)。 $1 < p < +\infty$ の場合、上部積分に対するヘルダーの不等式 (Ch. I、No. 3、提案 4) は不等式 (4) を生成し、関係 $N_1(fg) < +\infty$ は $fg$ が積分可能であることを示します。 (§ 5, No. 6、木曜日5)。 $p = 1$, $q = +\infty$, 不等式 (4) と $fg$ が可積分であるという事実は、平均値の不等式の明らか帰結です (No. 2、提案 1)。したがって、すべての場合において定理が証明されます。

#### 系 1 {#int-iv-s6-thm-2-cor-1 .statement tag=08XL}

— $F, G, H$ を 3 つのバナハ空間とし、$(u, v) \mapsto \Phi(u, v)$ を $|\Phi(u, v)| \leq |u| \cdot |v|$ となるような $F \times G$ から $H$ への連続双線形写像とする。 $f \in \mathscr{L}_F^p$ と $g \in \mathscr{L}_G^q$ の場合、写像 $\Phi(f, g)$ は可積分であり、

$$
\left| \int \Phi(f, g)\, d\mu \right| \leq \int |\Phi(f, g)|\, d|\mu| \leq N_p(f) N_q(g).
$$

なぜなら、$\Phi(f, g)$ は測定可能であるからです (§ 5, No. 3、Th. 1 のコリント 5)。 $|\Phi(f, g)| \leq |f| \cdot |g|$ なので、Th から系が続きます。 2 と § 5, No. 6 の積分可能性基準、Th。 5.

Cor の 2 つの特殊なケース。 1 はアプリケーションにおいて重要です。

#### 系 2 {#int-iv-s6-thm-2-cor-2 .statement tag=08XM}

— $F$ を実際の (それぞれ複合体) Banach 空間、$F'$ をその強力な双対 (TVS、III, § 3, No. 1) とし、$(z, z') \mapsto \langle z, z' \rangle$ を $F \times F'$ の正規の双線形形式とします。 $f \in \mathscr{L}_F^p$ と $g \in \mathscr{L}_{F'}^q$ の場合、実数 (それぞれ複素数) 写像 $\langle f, g \rangle$ は可積分であり、

$$
\left| \int \langle f, g \rangle\, d\mu \right| \leq \int |\langle f, g \rangle|\, d|\mu| \leq N_p(f) N_q(g).
$$

$|\langle z, z' \rangle| \leq |z| \cdot |z'|$ のために。

$F$ が実数または複素数のヒルベルト空間である場合、その双対 $F'$ (TVS、V, § 1, No. 7) で正規に識別できることがわかります。 空間 $L_F^2$ が完了したため、次の結果が得られます。

#### 系 3 {#int-iv-s6-thm-2-cor-3 .statement tag=08XN}

— $\mu$ を $X$ 、$F$ の実数 (それぞれ複素数) ヒルベルト空間に対する正の尺度とします。 空間 $L_F^2$ では、対称 (それぞれエルミート) 形

$$
(\widetilde{f}, \widetilde{g}) \mapsto \int \langle f, g \rangle\, d\mu
$$

定義するはヒルベルト空間構造で、ノルムは $\| \widetilde{f} \|_2$ に等しい。

#### 系 4 {#int-iv-s6-thm-2-cor-4 .statement tag=08XO}

— $F$ をバナハ空間、$f$ 写像を$\mathscr{L}_F^p$、$g$ を写像所属 ～ $\mathscr{L}^q$ の数値とします。したがって、 写像 $fg$ は可積分であり、

$$
\left| \int fg\, d\mu \right| \leq \int |fg|\, d|\mu| \leq N_p(f) N_q(g).
$$

#### 系 5 {#int-iv-s6-thm-2-cor-5 .statement tag=08XP}

— $f_1, f_2, \ldots, f_n$ を n 正の可積分関数とし、$\alpha_1, \alpha_2, \ldots, \alpha_n$ を n 数 $> 0$ とし、$\sum_{i=1}^n \alpha_i = 1$ とします。これらの条件、写像 $f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}$ は可積分であり、

$$
\int f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n} d|\mu| \leqslant
\left( \int f_1 d|\mu| \right)^{\alpha_1} \left( \int f_2 d|\mu| \right)^{\alpha_2} \cdots \left( \int f_n d|\mu| \right)^{\alpha_n}.
$$

なぜなら、積 $f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}$ は測定可能であり、測定可能な写像 (§ 5, No. 3、Th. 1 とその Cor. 5) の積であるからです。 不等式 (8) は上積分 (Ch. I、No. 2、提案 2 の補正) に真であるため、写像 $f_1^{\alpha_1} f_2^{\alpha_2} \cdots f_n^{\alpha_n}$ は可積分です (§ 5, No. 6、Th. 5)、よって系。

コル。 Thの2。 2 は次の命題によってシャープ化されます。

#### 命題 3 {#int-iv-s6-prop-3 .statement tag=08XQ}

— $\mu$ を X の正の測度、F を実数または複素バナッハ空間、F' をその強い双対、そして $(z, z') \mapsto \langle z, z' \rangle$ を $F \times F'$ の正規の双線形形式とします。

写像 $f \in \mathscr{L}_F^p$ ($1 \leq p \leq +\infty$) ごとに 1°、

$$
N_p(f) = \sup \left| \int \langle f, g \rangle \, d\mu \right|
$$

g は $\mathscr{L}_{F'}^q$ の写像の集合を超えて、 $N_q(g) \leq 1$ になります。

写像 $g \in \mathscr{L}_{F'}^q$ ($1 \leq q \leq +\infty$) ごとに 2°、

$$
N_q(g) = \sup \left| \int \langle f, g \rangle \, d\mu \right|
$$

f が $\mathscr{L}_F^p$ で写像の集合を超えると、 $N_p(f) \leq 1$ になります。

まず関係 (9) を証明しましょう。 2 つの場合を区別します。

(i) $1 \leq p < +\infty$。 $N_p(f) = 0$ の場合、関係 (9) は自明であるため (f と $\langle f, g \rangle$ が無視できるため)、f にスカラーを乗算すると、常に $N_p(f) = 1$ と仮定できます。まず、f が可積分ステップ写像, $f = \sum_{k=1}^n a_k \varphi_{A_k}$ であり、$A_k$ がペアごとに互いに素 (§ 4, No. 9, 補題) であると仮定します。したがって、$\sum_{k=1}^n |a_k|^p \mu(A_k) = 1$ by 仮定。 $\varepsilon > 0$ ごとに、(添字 k ごとに) ベクトル $a'_k \in F'$ が存在し、$p > 1$ の場合は $|a'_k|^q = |a_k|^p$ ($p = 1$ の場合は $|a'_k| = 1$)、および $\langle a_k, a'_k \rangle \geq (1 - \varepsilon)|a_k| \cdot |a'_k|$ (TVS、IV,

§1, No. 3、提案 8)。 設定 $g = \sum_{k=1}^n a_k' \varphi_{A_k}$、$p > 1$ の場合は $\sum_{k=1}^n |a_k'|^q \mu(A_k) = 1$ ($p = 1$ の場合は $\sup_{1 \leq k \leq n} |a_k'| = 1$)、つまり $N_q(g) = 1$ です。一方、

$$
\int \langle f, g \rangle d\mu = \sum_{k=1}^n \langle a_k, a_k' \rangle \mu(A_k) \geq (1 - \varepsilon) \sum_{k=1}^n |a_k| \cdot |a_k'| \mu(A_k)
$$

そして、$|a_k'| = |a_k|^{p/q} = |a_k|^{p-1}$ の場合 $p > 1$ (それぞれ $|a_k'| = 1$ の場合 $p = 1$) なので、次のようになります。

$$
\int \langle f, g \rangle d\mu \geq (1 - \varepsilon) \sum_{k=1}^n |a_k|^p \mu(A_k) = (1 - \varepsilon) N_p(f) = 1 - \varepsilon,
$$

この場合、これは関係 (9) を証明します。

$f$ が $N_p(f) = 1$ となるような $\mathscr{L}_F^p$ のいずれかの元である場合に移りましょう。 $\varepsilon > 0$ ごとに、$N_p(f - f_1) \leq \varepsilon$ となるようなステップ写像 $f_1 \in \mathscr{L}_F^p$ が存在します (§ 4, No. 10、提案 19 の訂正 1)。これまで見てきたことから、写像 $g \in \mathscr{L}_F^q$ が存在し、$N_q(g) = 1$ と

$$
\int \langle f_1, g \rangle d\mu \geq N_p(f_1) - \varepsilon \geq 1 - 2\varepsilon.
$$

さて、

$$
\int \langle f, g \rangle d\mu = \int \langle f_1, g \rangle d\mu + \int \langle f - f_1, g \rangle d\mu
$$

そして、(6)により、

$$
\left| \int \langle f - f_1, g \rangle d\mu \right| \leq N_p(f - f_1) N_q(g),
$$

よって

$$
\left| \int \langle f, g \rangle d\mu \right| \geq 1 - 3\varepsilon,
$$

これは (9) を証明します。

(ii) $p = +\infty$。ここでも、$N_\infty(f) > 0$ の場合に限定してみましょう。 $\alpha$ を $0 < \alpha < N_\infty(f)$ となるような任意の数とします。 $x \in X$ の仮定、集合により、$|f(x)| > \alpha$ は測定可能で局所的に無視できないため、含むは測定$> 0$ のコンパクトな集合 $K$ になります。 $f$ は可測であるため、$f$ から $K_1$ の制限が連続するような、$> 0$ 測定のコンパクトな集合 $K_1 \subset K$ が存在します。したがって、$\varepsilon > 0$ごとに、可積分可能な集合の有限数に$K_1$の分割が存在し、それぞれの$f$の振動は$\leq \varepsilon$です。これら集合 $A$ の少なくとも 1 つはメジャー > 0 です。$a$ を $A$ の $f$ の値の 1 つとします。次に、すべての $x \in A$ に対して $|a| > \alpha$ と $|f(x) - a| \leq \varepsilon$ が続きます。 $|a'| = 1$ と $|\langle a, a' \rangle| \geq |a| - \varepsilon$ のようなベクトル $a' \in F'$ が存在します。 写像 $g = \varphi_A \cdot a'/\mu(A)$ は可積分であり、$N_1(g) = 1$;一方、

$$
\int \langle f, g \rangle d\mu = \frac{1}{\mu(A)} \int \langle f, a' \rangle \varphi_A d\mu.
$$

さて、次のように書くことができます

$$
\int \langle f, a' \rangle \varphi_A d\mu = \langle a, a' \rangle \mu(A) + \int \langle f - a, a' \rangle \varphi_A d\mu,
$$

そしてそれ以来

$$
|\langle f - a, a' \rangle \varphi_A| \leq \varepsilon \varphi_A,
$$

私たちはそれを見てます

$$
\left| \int \langle f, g \rangle d\mu \right| \geq |\langle a, a' \rangle| - \varepsilon \geq |a| - 2\varepsilon > \alpha - 2\varepsilon;
$$

$\varepsilon$ は任意であり、$\alpha$ は数 < $N_\infty(f)$ であるため、この場合、関係 (9) も検証されます。

$1 \leq q < +\infty$ の場合と $q = +\infty$ の場合を別々に検討し、すべての $z' \in F'$ について、$F'$ のノルムの定義によって $|z'| = \sup_{|z| \leq 1} |\langle z, z' \rangle|$ が成り立つという事実を使用して、関係 (10) を証明するためにまったく同じ方法で議論します。

#### 注意 {#int-iv-s6-n4-rem-1 .statement tag=08XR}

— 1) $\mathscr{E}$ を $\mathscr{L}_{F'}^q$ の密な線形部分空間とします。そして、$g$が$\mathscr{L}_{F'}^q$の写像の集合$B$で$N_q(g) \leq 1$のように$\mathscr{E}$の共通部分を超えるとき、公式(9)が成り立ちます。 なぜなら、$\overset{\circ}{B}$が開いているので、$B$の内部$\overset{\circ}{B}$が$B$で密であり、$\overset{\circ}{B} \cap \mathscr{E}$が$\overset{\circ}{B}$で密であることを観察すれば十分だからです。 この注意は、特に$1 \leq q < +\infty$、つまり$1 < p \leq +\infty$のときのコンパクトサポート（$F'$の値）を伴う連続写像の集合$\mathscr{E} = \mathscr{K}(X; F')$に当てはまります。 しかしこの場合、$g$ が $p = 1$ であっても$B \cap \mathscr{K}(X; F')$ を超えるので、公式 (9) は真です。 なぜなら、上記のように、$f$ がステップ写像である場合に限定することができるからです。 $N_1(f) = 1$ の場合、$\varepsilon > 0$ ごとにステップ写像 $g \in \mathscr{L}_{F'}^\infty$ が存在し、すべての $x \in X$ と $|\int \langle f, g \rangle d\mu| \geq 1 - \varepsilon$ に対して $|g(x)| \leq 1$ となることが分かりました。 There exists a finite number of pairwise disjoint compact sets $K_i$ such that $g$ has a constant value $a'_i$ on each $K_i$ and such that, if $K$ is the union of the $K_i$, then $\int |f| \varphi_{\mathscr{C}_K} d\mu \leq \varepsilon$. $U_i$ を、集合 $U_i$ がペアごとに互いに素となるような $K_i$ の近傍とし、$h_i$ を、$U_i$ に含まれ、サポートが 1 に等しい、$X$ から $[0, 1]$ への連続写像とする。 $K_i$。 設定 $h = \sum a'_i h_i$、$K$ には $h(x) = g(x)$、$X$ には $|h(x)| \leq 1$ があります。

$$
\int |\langle f, h \rangle| \varphi_{\mathscr{C}_K} d\mu \leq \varepsilon
$$

その結果、$|\int \langle f, h \rangle d\mu| \geq 1 - 3\varepsilon$ となり、主張が証明されます。同様の注意を公式 (10) に対して作成できます。

2) $\mu$ を、$X$、$f$ の可測写像 $\geq 0$ (有限かどうか) の正の測度とし、そのサポートがコンパクト集合 $K_n$ の可算和集合に含まれるようにします。次に、$1 \leq p \leq +\infty$ となる $p$ ごとに、

$$
(11) \quad N_p(f) = \sup \int^* |fg| d\mu,
$$

$g$ は $\mathscr{H}(X; \mathbf{R})$ の写像の集合を超え、$N_q(g) \leq 1$ になります。なぜなら、$f$ は $\mathscr{L}^p$ (§ 5, No. 6、Th. 5) の写像と等価であるため、$N_p(f) < +\infty$ の場合、公式 (11) は (9) の特殊なケースとなります。 $N_p(f) = +\infty$ の場合、整数 $n > 0$ 集合 $f_n = \inf(n, f \varphi_{K_n})$ ごとに。それから

$$
N_p(f_n) = \sup \int^* |f_n g| d\mu \leq \sup \int^* |f g| d\mu,
$$

よって、移行から極限 (数列 $(K_n)$ が増加するであると仮定して) では、$\sup \int^* |f g| d\mu = +\infty$ (§ 1, No. 3、Th. 3) があります。

#### 系 {#int-iv-s6-n4-cor-1 .statement tag=08XS}

— *$\mu$を$X$、$F$をバナッハ空間、$F'$をその強力なデュアル、そして$g$を$\mathscr{L}^q_{F'}$の写像に対してポジティブな尺度とします。次に、$\mathscr{L}^p_F$の線型形式$f \mapsto \int \langle f, g \rangle d\mu$から商への通過によって推定される$L^p_F$の線型形式は連続しており、ノルム$N_q(g)$になります*。

### 5. 適用: 空間 $L^p_F$ ($1 \leq p \leq +\infty$) の間の関係

#### 命題 4 {#int-iv-s6-prop-4 .statement tag=08XT}

— *$f$ をバナッハ空間 $F$ の値で可測な写像とします。 $1 \leq p \leq +\infty$ と $N_p(f)$ が有限であるような数 $p$ の集合 $I$ は、空であるか、$\overline{\mathbf{R}}$ の区間です。 $I$が空でないなら、写像$p \mapsto N_p(f)$の制限～$I$が連続します。さらに、$f$ が無視できない場合、$\log N_p(f)$ は$1/p$ が$\bar{I}$ に凸の写像になります。

私たちはすでに、*有限* 数 $p \geq 1$ の集合 $J$ が、$N_p(f) < +\infty$ が空か区間であり、$\log N_p(f)$ が凸であることを知っています (Ch. I、No. 3、提案 5)。 $J$ の $1/p$ の写像 ($f$ が無視できない場合)。これはもちろん、$J$ での $p \mapsto N_p(f)$ の連続性を意味します。

$J$ が空の場合は、$I = \varnothing$ または $I = \{+\infty\}$ のいずれかになります。この場合、命題は明らかです。以降、$J$ が空でないであると仮定します。 $f$ が無視できる場合、命題も明らかです。今後、$f$ は無視できないものと仮定します。 $s \in J$ の場合、平均の有限数 $p > s$、$|f|^p = |f|^s |f|^{p-s}$、不等式ごとに次のことがわかります。

$$
(12) \quad N_p(f) \leq (N_s(f))^{s/p} (N_\infty(f))^{(p-s)/p}.
$$

$p$ が $+\infty$ になる傾向があるとすると、次のようになります。

$$
\limsup_{p \to +\infty} N_p(f) \leq N_\infty(f).
$$

これは、$+\infty \in I$ の場合、$J$ 含むは任意に大きい数であることを証明します。したがって、$I$ は確かに $\overline{\mathbf{R}}$ と $\overline{I} = \overline{J}$ の区間です。 $p \mapsto N_p(f)$ が $\overline{J}$ で連続であることを示せば、命題が証明され、$J$ の端点で連続性を確立するだけで十分です。さらに、$J$ は簡約するから点にならないと仮定できます。 $r$ と $s$ を $J$ ($r < s \leq +\infty$) の左右の端点とします。 $A$ を $|f(x)| \geq 1$ となるような $x \in X$ の (測定可能な) 集合とします。それから

$$
\int |f|^p d|\mu| = \int |f|^p \varphi_A d|\mu| + \int |f|^p \varphi_{C_A} d|\mu|.
$$

$p \in J$ は $r$ になる傾向があり、$|f|^p \varphi_A$ は減少するの間 $|f|^r \varphi_A$ になる傾向があり、$|f|^p \varphi_{C_A}$ は増加するの間 $|f|^r \varphi_{C_A}$ になる傾向があります。したがって、$\int |f|^p \varphi_{C_A} d|\mu|$ は $\int^* |f|^r \varphi_{C_A} d|\mu|$ (§ 1, No. 3、Th. 3) になる傾向があります。一方、$|f|^p \varphi_A$ は $p \in J$ に対して可積分であり、$\int |f|^p \varphi_A d|\mu|$ は $\int |f|^r \varphi_A d|\mu|$ になる傾向があります (§ 4, No. 3、提案 4)。したがって、$\int |f|^p d|\mu|$ は $\int^* |f|^r d|\mu|$ になる傾向があり、これは $r$ での $p \mapsto N_p(f)$ の連続性を証明します。

$s < +\infty$ の場合、同じ推論が点 $s$ にも適用される可能性があります。最後に、$s = +\infty$ だとします。 (13) を考慮すると、次のことを証明すれば十分です。

$$
\liminf_{p \to +\infty} N_p(f) \geq N_\infty(f).
$$

さて、$a$ を数とし、$0 < a < N_\infty(f)$ とします。 仮定までに、$x \in X$ の $N_p(f) < +\infty$、集合 $A$ となるような $p$ の有限の値が存在するので、可測で無視できない $|f(x)| \geq a$ は、次のおかげで積分可能です。 不等式 $\varphi_A \leq (|f|/a)^p$;さらに、この不等式から$N_p(f) \geq a \cdot (|\mu|(A))^{1/p}$と推測します。 $p$ を $+\infty$ にすると、$\liminf_{p \to +\infty} N_p(f) \geq a$ が続き、証明が完成します。

#### 系 {#int-iv-s6-n5-cor-1 .statement tag=08XU}

— *もし* $r, s, p$ *3 数が次のような*

$$
1 \leq r < p < s \leq +\infty,
$$

*その後共通部分* $\mathscr{L}_F^r \cap \mathscr{L}_F^s$ *は $\mathscr{L}_F^p$ に含まれます。

一般に、$\mathscr{L}_F^p$ ($r < p < s$) のトポロジーによって共通部分 $\mathscr{L}_F^r \cap \mathscr{L}_F^s$ に誘導されるトポロジーは *別個* であることに注意してください。 $\mu$ でそれ以上仮定が行われない場合、$\mathscr{L}_F^r$ と $\mathscr{L}_F^s$ のトポロジーによって $\mathscr{L}_F^r \cap \mathscr{L}_F^s$ に誘発されるトポロジーは一般に比較できません (他の語では、比率 $N_r(f)/N_s(f)$ は任意に大きい値と任意に小さい値を取ることができます) $\mathscr{L}_F^r \cap \mathscr{L}_F^s$; cf. エクサー。

提案 4 は、$\mu$ が制限された尺度である場合にシャープ化される可能性があります。

#### 命題 5 {#int-iv-s6-prop-5 .statement tag=08XV}

— $\mu$ を有界測度とし、$f$ をバナッハ空間 $F$ の値を持つ $\mu$ 可測写像とします。 $1 \leq p \leq +\infty$ と $N_p(f)$ が有限であるような数 $p$ の集合 I は、空であるか、左端点 $p = 1$ と含むがこの点である区間です。さらに、$(|\mu|(X))^{-1/p} N_p(f)$はIの$p$の増加する写像です。

これは、上記の提案 4 およびコルの明らか帰結です。第 4 章の提案 4 I、No. 3。

#### 系 {#int-iv-s6-n5-cor-2 .statement tag=08XW}

— メジャー $\mu$ が有界である場合、関係 $r < s$ は $\mathscr{L}_F^s \subset \mathscr{L}_F^r$ を意味します。さらに、位数 $s$ の平均収束の位相は、位数 $r$ ($\mathscr{L}_F^s$) の平均収束の位相よりもより細かいです。

一般に、位数 $s$ の平均での収束の位相は、位数 $r$ の平均での収束の位相より厳密により細かいであることがわかります (例 8)。

#### 命題 6 {#int-iv-s6-prop-6 .statement tag=08XX}

— $X$ を離散空間、$\mu$ を $X$ の各点に質量 $+1$ を配置することによって定義される $X$ のメジャーとします。 $f$ がバナッハ空間 $F$ への $X$ の写像である場合、集合数 $p$ の I は、$1 \leq p \leq +\infty$ と $N_p(f)$ が有限であるか、空であるか、 区間と右端点 $+\infty$ と含むこの点;さらに、$N_p(f)$はIの$p$の減少する写像です。

写像 $f$ (§ 1, No. 1、例)、および $N_\infty(f) = \|f\| = \sup_{x \in X} |f(x)|$ ごとに $\mu^*(|f|) = \sum_{x \in X} |f(x)|$。 $x \in X$ の無限多くの値に対して $|f(x)| \geq \alpha$ となるような数 $\alpha > 0$ が存在する場合、有限の $p$ ごとに $N_p(f) = +\infty$ になります。逆の場合、$|f(x_0)| = \|f\|$、よってとなるような $x_0 \in X$ が存在します。

$$
N_\infty(f) = |f(x_0)| \leq N_p(f)
$$

有限の$p$ごとに。 写像 $\log N_p(f)$ は $1/p$ に対して凸であり、点 $+\infty$ でその最小の値を取るので、I では必然的に $p$ の減少する写像になります (FRV、 I, § 4, No. 3、提案 5)、これで証明が完了します。

#### 系 {#int-iv-s6-n5-cor-3 .statement tag=08XY}

— $X$ が離散で、測定値 $\mu$ が $X$ の各点における質量 $+1$ によって定義される場合、関係 $r < s$ は $\mathscr{L}_F^r \subset \mathscr{L}_F^s$ を意味します。さらに、位数 $r$ の平均収束の位相は、位数 $s$ ($\mathscr{L}_F^r$) の平均収束の位相よりもより細かいです。

### 練習問題 {#int-iv-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
