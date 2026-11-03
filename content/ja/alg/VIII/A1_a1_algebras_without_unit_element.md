---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 1
section_title: Algebras without Unit Element
appendix: true
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.435-A VIII.446
pdf_pages: 0452-0463
extraction: native
subsections:
    - "no": 1
      title: Regular Ideals
      page: 435
      pdf_page: 452
    - "no": 2
      title: Adjunction of a Unit Element
      page: 437
      pdf_page: 454
    - "no": 3
      title: The Radical of an Algebra
      page: 439
      pdf_page: 456
    - "no": 4
      title: Density Theorem
      page: 442
      pdf_page: 459
statements: 20
exercises: 15
content_sha256: 703e6bb3b678590d4de9794514b4c8bb468392645c944cb258ee268dcac0063d
translated_from: content/en/alg/VIII/A1_a1_algebras_without_unit_element.md
translation_method: google
source_content_sha256: 98c6a5e57906681f8c0a6b353e8a358c25cc514a68622fa99dc2d3817a1b28f4
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: a6022be12d7935926eba230fddaf2c03033e239b84f1512e644ca874d77c094c
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 付録 1 代数単位元なし

この付録では、$k$ は可換環です。 $k$-代数は結合的であると想定されていますが、必ずしも単体であるとは限りません。

### 1. 定期的な理想

A を$k$-代数とする。 (III, §1, No. 2, p. 430) を思い出してください。A の左イデアルは、関係 $a\in A, x\in \mathfrak{a}$ が $ax\in \mathfrak{a}$ を暗示するような A の $k$ 部分加群 $\mathfrak{a}$ です。私たち定義する概念も同様に、正しい理想と両面の理想を持ちます。 A が $k$-代数、$\mathfrak{a}$ が A の両面イデアルである場合、移行から商になると、$k$ 加群の定義するの $k$-代数構造で乗法 $A/\mathfrak{a}$ (上記参照)。

A の左イデアルは、包含対象の A の適切な左イデアルの集合の極大元である場合に極大と呼ばれます。

#### 定義 1 {#alg-viii-a1-def-1 .statement tag=00P4}

A を $k$-代数、$\mathfrak{a}$ を A の左イデアルとします。 $a\in A$ ごとに $au-a$ 属するから $\mathfrak{a}$ となるような A の元 $u$ を剰余類における右単元 $\mathfrak{a}$ と呼びます。 剰余類における右単元 $\mathfrak{a}$ が存在する場合、理想的な $\mathfrak{a}$ は規則的であると言います。

同様に、A が $\mathfrak{b}$ を法とする左単位元、つまり $a\in A$ ごとに $va-a\in \mathfrak{b}$ となるような元 $v$ を持つ場合、A の右イデアル $\mathfrak{b}$ は正規であると言います。イデアルが両面である場合、それが左イデアルとして規則的であるか右イデアルとして規則的であるかを指定する必要があります。

代数 A がユニタルの場合、A の単位元は、A の左イデアル $\mathfrak{a}$ ごとに剰余類における右単元 $\mathfrak{a}$ になります。この場合、A の左 (または右) のイデアルはすべて規則的です。一方、A が元がすべて零である $k$-代数である場合、A は正則である A の唯一の (左または右) イデアルです。

$\mathfrak{a}$ を A の正規の左イデアルとし、$u$ 剰余類における右単元 $\mathfrak{a}$ とします。 $\mathfrak{b}$ が含む $\mathfrak{a}$ の左イデアルである場合、$u$ は剰余類における右単元 $\mathfrak{a}$ であるため、$\mathfrak{b}$ は正則です。したがって、最大で規則的な A の左イデアルは、A の正規の適切な左イデアルの集合の極大元です。さらに、含む $\mathfrak{a}$ の左イデアル $\mathfrak{b}$ は、$u$ が属するから $\mathfrak{b}$ にならない場合に限り、適切です。したがって、適切な左イデアルの集合含む $\mathfrak{a}$ の $\mathfrak{b}$ を包含順に並べると、帰納的集合になります。この集合に集合理論、III, §2, No. 4、p. 154 の 2 つ定理を適用すると、次の結果が得られます。

#### 命題 1 {#alg-viii-a1-prop-1 .statement tag=00P5}

A のすべての正規の適切な左 (または右) イデアルは、通常の最大の左 (または右) イデアルに含まれます。

#### 命題 2 {#alg-viii-a1-prop-2 .statement tag=00P6}

A を可換 $k$-代数とする。 A のイデアル $\mathfrak{a}$ は、擬似リング $A/\mathfrak{a}$ (I, §8, No. 1, p. 98) が体である場合に限り、通常の最大イデアルです。

A の元 $u$ は、$A/\mathfrak{a}$ の $u$ の標準像が代数 $A/\mathfrak{a}$ の単位元である場合に限り、A の (右または左) 単位元モジュロ $\mathfrak{a}$ です。したがって、理想的な $\mathfrak{a}$ は、代数 $A/\mathfrak{a}$ が単元である場合に限り、正規になります。これら条件が満たされているとします。

写像 $\mathfrak{b}\mapsto \mathfrak{b}/\mathfrak{a}$ は、代数含む $\mathfrak{a}$ の集合から代数 $A/\mathfrak{a}$ の理想の集合までの全単射です。これらは環 $A/\mathfrak{a}$ の理想です。なぜなら、この代数は統一的だからです。最後に、定理により、I, §9, No. 1、p. 115、環 $A/\mathfrak{a}$ の 1 は、非零であり、その理想値が 0 とそれ自体である場合に限り、体になります。 命題が続きます。

#### 例 1 {#alg-viii-a1-n1-exa-1 .statement tag=00P7}

V を可換体の無限次元ベクトル空間とします。 K. End$^f_K(V)$ を End$_K(V)$ の K-部分代数 、 有限階数の自己準同型のからなるとします。 W を V の線形部分空間とし、$\mathfrak{a}_W$ を核含む W である End$^f_K(V)$ の元の集合とします。 End$^f_K(V)$の左イデアルです。エンド$^f_K(V)$の元$u$は、$x\in W$ごとに$u(x) =x$がある場合に限り、剰余類における右単元$\mathfrak{a}_W$になります。このような元 $u$ は存在します。つまり、W が有限次元である場合に限り、$\mathfrak{a}_W$ は正則です。理想的な $\mathfrak{a}_W$ は、W が次元 1 である場合に限り、最大かつ規則的になります。

#### 例 2 {#alg-viii-a1-n1-exa-2 .statement tag=00P8}

T を局所コンパクト空間とし、$\mathscr{C}_0(T)$ を無限遠で 0 になる傾向がある T から $\mathbf{C}$ までの連続写像の可換$\mathbf{C}$-代数とする (Gen. Top., X, §4, No. 4, p. 316)。 T がコンパクトな場合にのみ単体になります。 F を T の閉じた部分集合とし、$\mathfrak{a}_F$ を $\mathscr{C}_0(T)$ の元の集合とし、F に対する制限は零写像とします。それは$\mathscr{C}_0(T)$の理想です。 $t\in F$ごとに$u(t) = 1$がある場合に限り、$\mathscr{C}_0(T)$の元$u$は$\mathfrak{a}_F$を法とする単位元です。このような元 $u$ は存在します。つまり、F がコンパクトである場合に限り、$\mathfrak{a}_F$ は正則です。 写像 $t\mapsto \mathfrak{a}_{\{t\}}$ は、$\mathscr{C}_0(T)$ (TS、I, §3、n$^o2$、p. 32、系 1) の通常の最大イデアの T から集合までの全単射です。 T がコンパクトではないと仮定し、コンパクト サポートを使用して $\mathfrak{a}$ 部分集合の $\mathscr{C}_0(T)$ からなるの写像で表すとします。その場合、$\mathfrak{a}$ は、$\mathscr{C}_0(T)$ の通常の理想には含まれない、$\mathscr{C}_0(T)$ の理想です。

#### 例 3 {#alg-viii-a1-n1-exa-3 .statement tag=00P9}

$L^1(\mathbf{R})$ を局所的にコンパクトな群 $\mathbf{R}$ の畳み込み代数とします。 (cf. Int.、VIII, §4, No. 5、p. 38) を思い出してください。$L^1(\mathbf{R})$ はルベーグ測度で積分可能な$\mathbf{R}$ 上の関数のクラスの空間です。 2 つの写像 $f$ と $g$ の類の積は、公式によって定義される写像 $f*g$ の類です

$$
(f*g)(s) =\int_{-\infty}^{+\infty}f(t)g(s-t)dt
$$

ほぼすべての $s\in \mathbf{R}$ に対して。 代数 $L^1(\mathbf{R})$ は単一ではありません。 $\mathbf{R}$ の $a$ については、$\mathfrak{m}_a$ 集合元 $f$ $L^1(\mathbf{R})$ 満たすで表します

$$
\int_{-\infty}^{+\infty}f(t)e^{-iat}dt= 0
$$

TS によると、II, §3、n$^o2$、p. 252、定理 1、写像 $a\mapsto \mathfrak{m}_a$ は、代数 $L^1(\mathbf{R}).*$ の通常の最大理想の $\mathbf{R}$ から集合までの全単射です。

### 2. 単位元中随伴

A を$k$-代数とする。 III, §1, No. 2、p. 431 では、単位元 $e$ の随伴によって A から推定される単位代数 $\widetilde{A}$ を定義しました。私たち同一視する A は、$\widetilde{A}$ という両面の理想を持っています。 $k$ モジュール $\widetilde{A}$ は、部分加群 $ke$ および A の直和です。

#### 命題 3 {#alg-viii-a1-prop-3 .statement tag=00PA}

a) $\widetilde{\mathfrak{a}}$ を $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ となるような $\widetilde{A}$ の左イデアルとする。私たちは集合 $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$です。 $u-e$ 属する ～ $\widetilde{\mathfrak{a}}$ となるような A の元 $u$ が存在します。 $u$ がそのような元である場合、それは $\mathfrak{a}$ を法とする A の権利単位元であり、$\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$ が得られます。特に理想的な$\mathfrak{a}$は規則的です。

b) 逆に、$\mathfrak{a}$ を A の正規の左イデアルとし、$u$ を $\mathfrak{a}$ を法とする A の右イデアル単位元とします。 集合 $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$。すると、$\widetilde{\mathfrak{a}}$ は $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ となるような $\widetilde{A}$ の左イデアルであり、$\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$ が得られます。

c) $k$ が体の場合、条件 $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ は、$\widetilde{\mathfrak{a}}$ が A に含まれていないというに相当します。

a)の仮定の下で、$\widetilde{A}$の元$e$は、$u\in A$と$u-e\in \widetilde{\mathfrak{a}}$を使って$(e-u)+u$と書くことができます。 $x=\lambda e+a$ を $\widetilde{A}$ の元とします。ここで、$\lambda \in k$ と $a\in A$ です。 $x$ 属するから $\widetilde{\mathfrak{a}}$ の場合、属するから $\mathfrak{a}$ の元 $y=a+\lambda u=x+\lambda (u-e)$ となり、$x=y-\lambda (u-e)$ になります。これは等式 $\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$ を証明します。 さらに、A のすべての $a$ について、A の要素 $au-a=a(u-e)$ は $\mathfrak{a}$ に属するため、$u$ は $\mathfrak{a}$ を法とする正しい単位です。 これは主張 a) を証明します。

$\mathfrak{a}$ と $u$ を b) のようにします。 $\widetilde{A}$はAの直和と$k(u-e)$なので、$\widetilde{\mathfrak{a}}+ A =\widetilde{A}$と$\widetilde{\mathfrak{a}}\cap A =\mathfrak{a}$ができます。 $\widetilde{\mathfrak{a}}$ のすべての元は、$x\in \mathfrak{a}$ と $\lambda \in k$ を含む形 $x+\lambda (u-e)$ です。 $a\in A$ ごとに、

$$
a(x+\lambda (u-e)) =ax+\lambda (au-a)
$$

$u$ は $\mathfrak{a}$ を法とする A の右単位元なので、和 $ax+\lambda (au-a)$ 属するから $\mathfrak{a}$ なので、$\widetilde{\mathfrak{a}}$ は A の左イデアルです。これは b) を証明します。

最後に、$k$ が体である場合、A は $\widetilde{A}$ の超平面であり、$\widetilde{A}$ は $\widetilde{\mathfrak{a}}$ の和であり、$\widetilde{\mathfrak{a}}$ が A に含まれていない場合に限り、A になります。

#### 系 {#alg-viii-a1-n2-cor-1 .statement tag=00PB}

A の通常の左イデアルは、形 $A\cap \widetilde{\mathfrak{a}}$ のイデアルです。ここで、$\widetilde{\mathfrak{a}}$ は、$\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ となる $\widetilde{A}$ の左イデアルです。

#### 命題 4 {#alg-viii-a1-prop-4 .statement tag=00PC}

a) $\mathfrak{a}$ を A の通常の最大左イデアルとします。$\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ と $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$ のような、$\widetilde{A}$ の一意の左イデアル $\widetilde{\mathfrak{a}}$ が存在します。この理想は最大であり、含む A にはなりません。

b) 写像 $\widetilde{\mathfrak{a}}\mapsto \widetilde{\mathfrak{a}}\cap A$ は、A の通常の最大左イデアルの含むから集合ではなく、$\widetilde{A}$ の最大左イデアルの集合からの全単射です。

$\mathfrak{a}$ を A の通常の最大左イデアルとします。 命題 3、a) により、$\widetilde{A}$ の左イデアル $\mathfrak{b}$ は、$\mathfrak{b}+ A =\widetilde{A}$ と $\mathfrak{b}\cap A =\mathfrak{a}$ がイデアル $\mathfrak{a}+k(u-e)$ となり、$u$ は剰余類における右単元となります。 $\mathfrak{a}$。したがって、$\widetilde{\mathfrak{a}}$の一意性を証明するには、$\mathfrak{a}$を法とするAの2つの正しい単位元$u$と$u'$が$\mathfrak{a}$を法として合同であることを証明すれば十分です。矛盾によって推論し、$u-u'$ が属するから $\mathfrak{a}$ にならないと仮定しましょう。 公式 $x(u-u') = (xu-x)-(xu'-x)$ は、$A(u-u')\subset \mathfrak{a}$ があることを示します。したがって、$\mathfrak{a}+k(u-u')$ は含む $\mathfrak{a}$ の左イデアルであり、$\mathfrak{a}$ とは異なります。 $\mathfrak{a}$ が最大であるため、$\mathfrak{a}+k(u-u') = A$ があり、AA $\subset \mathfrak{a}$ になります。すべての $x\in A$ に対して、$x\equiv xu$ (mod $\mathfrak{a}$) が得られるため、上記により $x\in \mathfrak{a}$ となり、矛盾する仮定 $\mathfrak{a}\not= A$ となります。

従って、$\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ と $\mathfrak{a}=\widetilde{\mathfrak{a}}\cap A$ のような、$\widetilde{A}$ の固有の左イデアル $\widetilde{\mathfrak{a}}$ が存在します。 $\mathfrak{b}$ を、$\widetilde{A}$ 含む $\widetilde{\mathfrak{a}}$ の適切な左理想とする。すると$\mathfrak{b}\cap A$は含む$\mathfrak{a}$の正しい左イデアルになります。従って、$\mathfrak{a}$が最大であるため、$\mathfrak{a}$と等しくなります。これは、VIII、p. 4の2である補題によって$\mathfrak{b}=\widetilde{\mathfrak{a}}$を意味します。これは、$\widetilde{\mathfrak{a}}$ が $\widetilde{A}$ の最大の理想であることを証明します。このような理想の場合、条件 $\widetilde{A} =\widetilde{\mathfrak{a}}+ A$ は、$\widetilde{\mathfrak{a}}$ が含む A ではないことを意味します。

$\widetilde{\mathfrak{a}}$ が含む A ではない $\widetilde{A}$ の最大左イデアルである場合、A の左イデアル $\mathfrak{a}= A\cap \widetilde{\mathfrak{a}}$ が最大であることを証明する必要があります。 $\mathfrak{b}$ を含む $\mathfrak{a}$ の適切な左理想とする。 $u$ を剰余類における右単元 $\mathfrak{a}$ とし、$\widetilde{\mathfrak{a}}=\mathfrak{a}+k(u-e)$ (命題 3) とします。 剰余類における右単元 $\mathfrak{b}$ でもあります。 $\widetilde{\mathfrak{b}}$ は、$\widetilde{A}$ の理想的な $\mathfrak{b}+k(u-e)$ を表します。 命題 3、b) までに、$\mathfrak{b}= A\cap \widetilde{\mathfrak{b}}$ になります。 $\mathfrak{a}+k(u-e)$ に等しい理想的な $\widetilde{\mathfrak{a}}$ は $\widetilde{\mathfrak{b}}$ に含まれており、$\widetilde{\mathfrak{b}}$ が $\widetilde{A}$ とは異なり、$\widetilde{\mathfrak{a}}$ が最大であるため、$\widetilde{\mathfrak{b}}$ に等しくなります。その結果、$\mathfrak{a}=\mathfrak{b}$があり、$\mathfrak{a}$が最大となります。

命題 3 と 4 を正しい理想に翻訳するのは読者に任せます。

### 3. 代数中根基

A を$k$-代数とする。 A 上の左擬加群は、疑似リング A (II、付録、No. 2、p. 378) 上で左擬加群の構造を備えた $k$ モジュール M であり、$\lambda \in k$ に対して $a(\lambda x) =\lambda (ax) = (\lambda a)x$ が得られます。 $a\in A$、および$x\in M$。同様に、A に対して定義するが正しい擬加群です。

M を A に対して左擬加群とします。私たちは定義する設定によって正規と呼ばれる M 上の左の $\widetilde{A}$ モジュール構造です

$(\lambda e+a)x=\lambda x+ax$ は $\lambda \in k, a\in A, x\in M$ です。

逆に、左側のすべての $\widetilde{A}$ モジュールは、演算子の環を $k$ と A に制限し、A 上の左擬加群の構造を正規に与えられています。 従って、A 上の左擬加群の構造と $\widetilde{A}$ 上の加群の種は同等です。 (集合理論、IV, §1, No. 7、p. 262)。

M を A 上の左擬加群とし、N を M の $k$ サブモジュールとします。このとき、N は、A の作用の下で安定している場合に限り、M の $\widetilde{A}$ サブモジュールになります。次に、N は M の部分擬加群であると言います。

環の場合と同様に、Aの上に定義する左擬加群 $A_s$と右擬加群 $A_d$を重ねます。 A の左 (右) の理想は、$A_s$ (それぞれ $A_d$) の部分擬加群です。

$\mathfrak{a}$ を A の正規左イデアルとし、$u$ 剰余類における右単元 $\mathfrak{a}$ とします。 集合 $M = A_s/\mathfrak{a}$、M の $u$ の像を $z$ で表します。 $M = Az$があり、$\mathfrak{a}$は$z$の消滅子です。

逆に、M を A に対して左擬加群とし、$z$ を M の元とし、$M = Az$ とします。すると、$z=uz$となるようなAの元$u$が存在します。 $a\in A$ ごとに $(au-a)z= 0$ があるため、$z$ の $au-a$ 属するから消滅子 $\mathfrak{a}$ となります。従って、$\mathfrak{a}$ は A の正規左イデアルであり、元 $u$ は剰余類における右単元 $\mathfrak{a}$ であり、移行から商になると、写像 $a\mapsto az$ 定義する同型となります。 $A_s/\mathfrak{a}$ Mさんへ

#### 定義 2 {#alg-viii-a1-def-2 .statement tag=00PD}

AM $\not= 0$ があり、0 と M が M の唯一の部分擬加群である場合、A 上の擬加群 M は単純であると言います。

この対応するからというは、$\widetilde{A}$ モジュール M は単純であり、その消滅子は含む A ではないということです。A が環で M が A-加群のとき、AM = M なので、定義 2 一致するとなります。 定義 VIII、p. 45 の 1。

#### 命題 5 {#alg-viii-a1-prop-5 .statement tag=00PE}

a) $\mathfrak{m}$ を A の通常の最大左イデアルとします。すると、擬加群 $A_s/\mathfrak{m}$ は単純で、消滅子 $\mathfrak{m}$ を持つ $A_s/\mathfrak{m}$ の非零元が存在します。

b) M を単純な擬加群とし、$x$ を M の非零元とします。$M = Ax$、$x$ の消滅子 $\mathfrak{m}$ は A の通常の最大左イデアルであり、移行から商のとき、 写像 $a\mapsto ax$ 定義する同型 $A_s/\mathfrak{m}$ から M.

c) M を 0 に減らさない擬加群とします。そのとき、M の非零元 $x$ ごとに $M = Ax$ がある場合に限り、M は単純です。

$\mathfrak{m}$ を A の通常の最大左イデアルとします。消滅子が $\mathfrak{m}$ に等しく、$Az= A_s/\mathfrak{m}$ となるような $A_s/\mathfrak{m}$ の非零元 $z$ が存在することを見てきました。特に、$A(A_s/\mathfrak{m})\not= 0$ があります。さらに、$A_s/\mathfrak{m}$ のすべての部分擬加群は形 $\mathfrak{n}/\mathfrak{m}$ のものであり、$\mathfrak{n}$ は含む $\mathfrak{m}$ の左イデアルです。 $\mathfrak{m}$ が最大であるため、可能性は $\mathfrak{n}=\mathfrak{m}$ と $\mathfrak{n}= A$ だけであるため、擬加群 $A_s/\mathfrak{a}$ は単純です。これは a) を証明します。

b) の仮定では、M の元 $y$ の集合により、$Ay= 0$ は M の部分擬加群が M と異なるため、0 に減らされます。その結果、$Ax$ は M の非零部分擬加群になります。 $M = Ax$ を意味します。 主張 b) から注意前に定義 2.

M を非零擬加群とします。 M のすべての非零元 $x$ に対して $Ax= M$ があるとします。特に AM $\not= 0$ があります。 N を M の非零部分擬加群とし、$x$ を N の非零元とします。$Ax= M$ があるため、N = M です。従って、M は単純です。逆に、M が単純な場合、b) により、すべての $x\not= 0$ に対して $M = Ax$ が得られます。

#### 定義 3 {#alg-viii-a1-def-3 .statement tag=00RT}

$\Re (A)$ で示される $k$-代数 A の根基は、A の正則最大左イデアルの共通部分です。

A が環のとき、A の左イデアルはすべて正則なので、根基一致するの定義と、VIII の 2 つである定義 、p. 154 です。

#### 例 1 {#alg-viii-a1-n3-exa-1 .statement tag=00PF}

$k$-代数 End$^f_k(V)$ の根基は 0 に還元されます (VIII, p. 436, 例 1)$.*$ 代数 $\mathscr{C}_0(T)$ と $L^1(\mathbf{R}).*$ についても同様です

#### 例 2 {#alg-viii-a1-n3-exa-2 .statement tag=00PG}

A をすべての元が nilpotent である擬似リングとする。 A は唯一の正規左イデアルであるため、A の根基は A に等しい。

命題 5 は次の結果を直ちに暗示します。

#### 命題 6 {#alg-viii-a1-prop-6 .statement tag=00PH}

代数 A の根基は、単純な擬加群の消滅子の共通部分です。特に、A の両面の理想です。

#### 命題 7 {#alg-viii-a1-prop-7 .statement tag=00PI}

A の根基は、$\widetilde{A}$ の根基の A 上のトレースです。また、反対多元環 $A^o($ の根基、つまり A) の通常の最大右イデアルの共通部分にも等しい。 環 $k$ に根基がない場合、A の根基は $\widetilde{A}$ の根基と等しくなります。

等式 $\Re (\widetilde{A})\cap A =\Re (A)$ は、VIII、p. 438、b) の命題 4 から続きます。 $\widetilde{A}$ と $\widetilde{A}^o$ は同じ根基 (VIII, p. 156, 系 1) なので、等式 $\Re (A) =\Re (A^o)$ が続きます。 $k$ に根基がない場合、$\widetilde{A}$ 含む A の最大左イデアルの共通部分は A に等しい。その結果、$\Re (\widetilde{A})$ は A に含まれているため、$\Re (A)$ に等しい。

#### 注意 {#alg-viii-a1-n3-rem-1 .statement tag=00PJ}

$x$ と $y$ を A の元とします。 $\widetilde{A},x-e$ が $y-e$ の左逆逆である場合、つまり $x+y=xy$ がある場合、$x$ は $y$ の左逆である、または $y$ は $x$ の右逆であると言います。 命題 7 とジェイコブソンの定理 (VIII, p. 156, 定理 1) により、A の根基は A の元 $x$ で構成され、$ux-e$ は可逆のままになります。 $\widetilde{A}$ の $u$ ごとに $\widetilde{A}$。 $(a+\lambda e)x-e=ax+\lambda x-e$ ($a\in A,\lambda \in k$ の場合) があるため、A の根基は、A の元の $x$ の集合となり、$ax+\lambda x$ は、$a\in A$ と $\lambda \in k$ ごとに A に左逆効果が生じます。

### 4. 密度定理

A を$k$-代数とする。 左擬加群 M は、単純な左擬加群族の直和であれば、半単純と呼ばれます。

#### 補題 1 {#alg-viii-a1-lem-1 .statement tag=00PK}

M を半単純左 A 擬似モジュールとする。 B を $\widetilde{A}$ モジュール M の双可換子とします。すると、M のすべての A サブ擬似モジュールは M の B-部分加群になります。

$\widetilde{A}$ モジュール M は半単純です。 N を M の A サブ擬似モジュールとします。このとき、N は M の $\widetilde{A}$ サブモジュールです。VIII, p. 56 の系 2 により、像 N を持つ A-加群 M の射影子 $p$ が存在します。 $b\in B$ごとに関係 $pb=bp$があり、NがMのB-部分加群であることがわかります。

#### 補題 2 {#alg-viii-a1-lem-2 .statement tag=00PL}

M を左 A 疑似モジュールの半単純とし、$x$ を M の元とします。 $ax=x$ となるような元 $a\in A$ が存在します。

N を左の A 擬似モジュール $\widetilde{A}x/Ax$ とします。 AN $=\{0\}$ を満たします。 VIII、p. 56 の系 3 を $\widetilde{A}$ モジュール M と $\widetilde{A}x$ に適用すると、A 疑似モジュール N は半単純になります。 定義までに、N のすべての単純な部分擬加群 S は AS $\not=\{0\}$ を満たします。従って、擬加群 N は零となり、$x\in Ax$ が得られます。

#### 定理 1 (ジェイコブソンの密度定理) {#alg-viii-a1-thm-1 .statement tag=00SD}

M を半単純左 A 擬似モジュールとする。 $b$ を $\widetilde{A}$ モジュール M の双可換子の元とします。 $F =\{x_1, . . . , x_n\}$ を M の有限部分集合とします。すると、$i\in [1, n]$ ごとに $bx_i=ax_i$ となる元 $a\in A$ が存在します。

B を $\widetilde{A}$ モジュール M の双可換子とします。A 疑似モジュール $M^n$ は半単純です。 $\boldsymbol{x}= (x_1, . . . , x_n)\in M^n$ にしましょう。 補題 2 から、$\boldsymbol{x}\in$ $A\boldsymbol{x}$ が続きます。 $\widetilde{A}$ モジュール $M^n$ 一致するの双可換子は、B-加群 $M^n$ (VIII、p. 79、命題 2) と相似です。従って、補題 1 により、$M^n$ の A サブ疑似モジュール $A\boldsymbol{x}$ は $M^n$ の B-部分加群になります。従って、$B\boldsymbol{x}\subset A\boldsymbol{x}$ が含まれます。従って、$b\boldsymbol{x}=a\boldsymbol{x}$ となるような $a\in A$ が存在します。結果は次のとおりです。

### 練習問題 {#alg-viii-a1-exercises}

[練習問題付録 1](exercises/a1/)を参照してください。
