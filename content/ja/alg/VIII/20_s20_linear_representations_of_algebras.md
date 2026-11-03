---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 20
section_title: Linear Representations of Algebras
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.373-A VIII.395
pdf_pages: 0390-0412
extraction: native+ocr
subsections:
    - "no": 1
      title: Linear Representations of Algebras
      page: 373
      pdf_page: 390
    - "no": 2
      title: Restricted Dual of an Algebra
      page: 375
      pdf_page: 392
    - "no": 3
      title: Coefficients of a Module
      page: 377
      pdf_page: 394
    - "no": 4
      title: Restricted Dual and Matrix Coefficients
      page: 379
      pdf_page: 396
    - "no": 5
      title: Dual of a Semisimple Algebra
      page: 380
      pdf_page: 397
    - "no": 6
      title: Character of a Representation
      page: 382
      pdf_page: 399
    - "no": 7
      title: Coefficients of a Set of Classes of Modules
      page: 387
      pdf_page: 404
    - "no": 8
      title: Cogebra Structure on the Restricted Dual
      page: 388
      pdf_page: 405
statements: 31
exercises: 6
content_sha256: 80fea5bc3301529c5afa43080c94201ac1cb299a6fa9ff74f2a44ff8f9627909
translated_from: content/en/alg/VIII/20_s20_linear_representations_of_algebras.md
translation_method: google
source_content_sha256: f366c2c3ce31096fbcd7ad9041a4e06384cc60f8e5e5fd661e93b1a5434b90dc
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 6dec24b0b87ff73dbcfbd379872c92883c4e8a04f5ba8c57d86474c962128b77
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 20。 線型表現/代数

この切断では、Kは可換環、AはK-代数です。 No. 2 以降、K は体であると仮定し、K に対するベクトル空間 A の双対を $A^*$ で表します。この切断では、記法 $A^*$ は決して環 A の乗法群を指しません。

### 1. 線型表現/代数

#### 定義 1 {#alg-viii-s20-def-1 .statement tag=00MD}

MをK-加群とします。 M の代数 A の線型表現は、A から代数 End$_K(M)$ までの K 準同型性 $\pi$ です。

また、対 $(M, \pi )$ は代数 A の線型表現であるとも言います。M が自由K-加群のとき、M の次元は $\pi$ の次数 (または次元) と呼ばれます。

$\pi$ を M の A の線型表現とします。M の加法法則と M の外部法則 $(a, x)\mapsto \pi (a)(x)$ 定義する左A-加群構造を$M_{\pi}$ で表します。 $M_{\pi}$ は表現 $\pi$ の加群であると言います。 M の K-加群構造は、$M_{\pi}$ の A-加群構造からスカラーの制限によって得られます。

逆に、E を左A-加群とします。 M を A から K までのスカラーの制限によって E から推定される K-加群とし、A から End$_K(M)$ までの準同型 $a\mapsto a_E$ を$\pi$ とします。すると、$\pi$はMのAの表現で、$E = M_{\pi}$が得られます。 $\pi$ は線型表現が A-加群 E に関連付けられていると言います。

A の A-加群または線型表現を勉強することは同じになります。 加群に関する特定の定義を線型表現の言語に翻訳します。

$\pi$ を M の A の線型表現とします。 準同型 $\pi$ の核は、A の両面イデアであり、単純に A-加群 $M_{\pi}$ の消滅子です。 準同型 $\pi$ は、A-加群 $M_{\pi}$ が忠実である場合にのみ単射法です。次に、$\pi$ は A の忠実な表現であると言います。

$(M, \pi )$と$(M', \pi ')$をAの線型表現とします。$M_{\pi}$から$M'_{\pi'}$までのA-線型写像は関係を満たすK-線型写像$u: M\rightarrow M'$です

$$
\pi '(a)\circ u=u\circ \pi (a) \tag{1}
$$

$a\in A$の場合。 $M_{\pi}$から$M'_{\pi'}$までの同型は、K-加群$u: M\rightarrow M'$満たす条件の同型です

$$
\pi '(a) =u\circ \pi (a)\circ u^{-1} \tag{2}
$$

$a\in A$の場合。 A-加群 $M_{\pi}$ と $M'_{\pi'}$ が同型である場合、 $\pi$ と $\pi '$ は同型であると言います。 $M_{\pi}$ が $M'_{\pi'}$ の部分加群 (それぞれ商加群) である場合、$\pi$ は $\pi '$ の部分表現 (それぞれ商表現) であると言います。

A の線型表現のファミリー $(M_i, \pi_i)$ が与えられたとします。M を K-加群、つまり $M_i$ の直和とします。任意の $a\in A$ について、$\pi (a)$ を M の自己準同型 $(x_i)_{i\in I}\mapsto (\pi_i(a)(x_i))_{i\in I}$ とします。すると、$\pi$ は M の A の線型表現になります。 A-加群 $M_{\pi}$ は A-加群の直和です$(M_i)_{\pi}(i\in I)$; $\pi$ は $\pi_i$ の直和であると言い、$\pi =\bigoplus\pi_{i^i}$ と書きます。

A-加群 $M_{\pi}$ が単純であれば、M における A の表現 $\pi$ は単純である、または既約であると言います。 M 上の A の表現 $\pi$ は半単純である、または A-加群 $M_{\pi}$ が半単純である場合に完全に還元可能であると言います。

$\pi$ を M の A の線型表現とします。 $M^*$ を M に対して双対な K-加群とします。 $A^o$ から End$_K(M^*)$ までの写像 $a\mapsto^t(\pi (a))$ は、$\pi$ の表現を転置したものです。

L を可換K-代数とし、$(M, \pi )$ を K-代数 A の線型表現とします。準同型 $\pi_{(L)}: A_{(L)}\rightarrow$ End$_L(M_{(L)})$ 対応するを$M_{(L)}$ の $A_{(L)}$ モジュール構造にすると、次のようになります。 L代数$A_{(L)}$の線型表現。 $\pi_{(L)}$ は、スカラー K の環を L に拡張することにより、表現 $\pi$ から推定される代数 $A_{(L)}$ の線型表現であると言います。

K が体で、L が非零可換K-代数であるとします。

$\pi$ と $\pi '$ を代数 A の線型表現とします。 VIII、p. 37、定理 3 から、表現 $\pi$ と $\pi '$ は、$\pi_{(L)}$ とその場合にのみ同型であることがわかります。 $\pi '_{(L)}$です。

K が体であるとします。 L を K の拡大とします。K 上で有限次元である A-加群のグロタンディーク群 $R_K(A)$ (それぞれ $R_L(A_{(L)})$) (L 上で有限次元である $A_{(L)}$ 加群のそれぞれ) を考えます。 群準同型を見てきました

$$
u: R_K(A)\longrightarrow R_L(A_{(L)})
$$

スカラーの拡大によって定義されるは単射です。さらに、元 $\xi \in R_K(A)$ は、$u(\xi )$ が (VIII、p. 195、定理 1) である場合にのみ有効です。

### 2. 代数の制限付きデュアル

ここからは K が体であると仮定します。

$a\in A$ については、A から A まで $\boldsymbol{\gamma }(a)$ 写像 $x\mapsto ax$ と $\boldsymbol{\delta }(a)$ 写像 $x\mapsto xa$ で表します。 すると、$\boldsymbol{\gamma }$ は A の A の線型表現であり、左の正則表現と呼ばれます。同様に、$\boldsymbol{\delta }$ は A の $A^o$ の線型表現であり、(言葉の乱用により) A の権利正則表現と呼ばれます。 転置により、代数 A の $\boldsymbol{\delta }$ と $\boldsymbol{\gamma }$ 線型表現およびベクトル空間 $A^*$ の $A^o$ から、$A^*$ 左A-加群構造と左の定義するが推定されます。 $A^o$モジュール構造。 これら 2 つの構造対応するを、公式によって定義された外部法則を含む $A^*$ の $(A$、A)-bimodule 構造に変換します。

$$
\langle af, b\rangle =\langle f, ba\rangle \tag{3}
$$

$$
\langle f a, b\rangle =\langle f, ab\rangle \tag{4}
$$

$a, b,\in A$ と $f\in A^*$ の場合。

(II, §2, No. 4, p. 234, 定義 4) を思い出してください。E が A の線形部分空間である場合、$A^*$ におけるその直交$E'$ は、E に対する制限が零である A 上の線型形式の集合です。同様に、$A^*$の線形部分空間FのAの直交$F'$は、Fに対する線型形式所属の核の共通部分です。

(II, §7, No. 5、p. 299、定理 7) 写像 $\varphi : E\mapsto E'$ は、有限余次元の A の線形部分空間の集合から、A の線形部分空間の集合までの全単射であることがわかります。 有限次元中$A^*$。逆行列写像 $\varphi^{-1}$ は、$A^*$ の有限次元部分空間 F を A の直交行列 $F'$ に送ります。

#### 命題 1 {#alg-viii-s20-prop-1 .statement tag=00ME}

a) 写像 $\varphi$ 誘導する全単射有限余次元の A の左 (それぞれ右、両面) 集合から右 A-部分加群 (それぞれ左 A-部分加群、部分両側加群) の集合まで有限次元の $A^*$ が K を超えています。

b) 有限余次元含むの A の左または右のすべての理想、有限余次元の両側の理想。

式 (3) と (4) は、E が A の左イデアルである場合、$E'$ は$A^*$ の右 A 部分加群であることを証明します。 V が $A^*$ の右 A サブモジュールである場合、$V'$ は A の左イデアルです。 正しい理想の場合と両面の理想の場合は同様に扱われます。 これは a) を証明します。

$\mathfrak{a}$を有限余次元のAの左イデアルとする。 左A-加群 $E = A_s/\mathfrak{a}$ は K 上の有限次元であり、End$_K(E)$ も同様です。従って、Aから終わり$_K(E)$までの準同型$a\mapsto a_E$の核は、$\mathfrak{a}$に含まれる有限余次元のAの両面の理想です。 移行から反対環 $A^o$ まで、有限余次元含むの A のすべての正しい理想が、有限余次元の両面の理想であることがわかります。

#### 定義 2 {#alg-viii-s20-def-2 .statement tag=00MF}

制限されたデュアル

Θ(A) で示される K-代数 A の は、有限余次元の A の両側イデアルの直交関数の $A^*$ における和集合です。

命題 1 により、次の Θ(A) と同等の記述を与えることができます。

– 有限余次元の A の左イデアルの直交関数の和集合

– 有限余次元の A の右イデアルの直交関数の和集合 – 有限余次元の A の両側イデアルの直交関数の和集合 – K 上の $A^*$ の有限次元の左の A-部分加群の和集合

– K 上の有限次元の $A^*$ の右側の A サブモジュールの結合

– $(A$ の和集合、K 上の有限次元の $A^*$ の A) サブバイモジュール。

A が K に対して有限次数を持っている場合、$\Theta (A) = \Theta (A^o)$ と $\Theta (A) = A^*$ があります。$f\in A^*$ とします。次に、$Af$ (それぞれ $fA, AfA$) が K 上の有限次元の $A^*$ の線形部分空間である場合に限り、 $f$ 属するから Θ(A) になります。

2 つの $(A$ の和、K 上の有限次元の $A^*$ の A) サブ双モジュールには、K 上の有限次元があります。従って、Θ(A) は $A^*$ の $(A$、A) サブ双モジュールであることがわかります。

### 3. 加群の係数

Eを左A-加群とします。 $E^*$ を K 上のベクトル空間 E の双数とします。私たちはそれに自然な右A-加群構造を与えます。 E の元 $x$ と $E^*$ の $x^*$ を考えると、$c_E(x, x^*)$ 線型形式で表されます

$$
c_E(x, x^*) :a\mapsto  \langle x^*, ax\rangle \tag{5}
$$

これらの線型形式はEの係数と呼ばれます。Eの係数によって生成された$A^*$の部分空間は$\Theta_E(A)$で表されます。 Eが非零なら非零です。

F が E と同型の A-加群であれば、E と F は同じ係数を持ち、$\Theta_F(A) = \Theta_E(A)$ が得られます。 $E^*$ を左側の $A^o$ モジュールとして見てみましょう。 Eの係数は、$E^*$の係数、および$\Theta_E(A)\subset \Theta_{E^*}(A^o)$です。その結果、E が K 上で有限次元である場合、E と $E^*$ は同じ係数を持ち、$\Theta_E(A) = \Theta_{E^*}(A^o)$ が得られます。

$(M, \pi )$ を代数 A の線型表現とします。A-加群 $M_{\pi}$ の係数は、表現 $\pi$ の係数とも呼ばれます。 係数 $c_{M_{\pi}}(x, x^*)$、$x\in M$ と $x^*\in M^*$ は、$c_{\pi}(x, x^*)$ とも表されます。 ベクトル空間 $\Theta_{M_{\pi}}(A)$ は $\Theta_{\pi}(A)$ とも表されます。

#### 注意 1 {#alg-viii-s20-n3-rem-1 .statement tag=00MG}

M が K 上で有限次元であるとします。$(e_1, . . . , e_n)$ を V の基底とし、$(e^*_1, . . . , e^*_n)$ をその双対基底とします。 Vの基底$(e_1, . . . , e_n)$に関して、$\pi (a)$の$(\pi_{ij}(a))$行列で表します。 $\pi_{ij}=$ $c_{\pi}(e_j, e^*_i)$ があります。 写像 $a\mapsto (\pi_{ij}(a))$ は、A から $\mathbf{M}_n(K)$ までの準同型です。このような準同型は、代数 A の行列表現と呼ばれるときどきです。

#### 注意 2 {#alg-viii-s20-n3-rem-2 .statement tag=00MH}

EをA-加群、$E'$をEの部分加群とします。定理の系、II, §7, No. 5、p. 299の5により、$\Theta_{E'}(A)\subset \Theta_E(A)$と$\Theta_{E/E'}(A)\subset \Theta_E(A)$が得られます。

$\gamma_E$ を $E\otimes_KE^*$ から $A^*$ までの一意なK-線型写像として、$x\otimes x^*$ を $c_E(x, x^*)$ に送信します。それは $(A$、A)-双線形であり、その像は $\Theta_E(A)$ です。そこから A-線型写像 $c'_E: E\rightarrow$ Hom$_A(E^*,A^*)$ と $c''_E: E^*\rightarrow$ Hom$_A(E,A^*)$ を推論すると、次のようになります。

$$
c'_E(x)(x^*) =c_E(x, x^*) =c''_E(x^*)(x)
$$

$\theta_E$ K-線型写像 $\theta_E: E\otimes E^*\rightarrow$ 関係で特徴付けられる終わり$_K(E)$ で示されます

$$
\theta_E(x\otimes x^*)(y) =\langle x^*, y\rangle x
$$

$x, y\in E$と$x^*\in E^*$の場合。その像は、有限階数のEの自己準同型の集合末$^f_K(E)$です（VIII、p. 463）。トレースの定義 (上記引用) までに、

トリ($\theta_E(x\otimes x^*)$) $=\langle x^*, x\rangle$

$x\in E$ と $x^*\in E^*$ の場合。したがって、私たちは

$\langle \gamma_E(x\otimes x^*), a\rangle =\langle x^*, ax\rangle =$ トリ($\theta_E(ax\otimes x^*)$) $=$ トリ($\theta_E(x\otimes x^*)a$)。

これにより、関係が得られます

$\langle \gamma_E(h), a\rangle =$ トリ($\theta_E(h)\circ a_E$)

$a\in A$と$h\in E\otimes_KE^*$の場合。これは、$\Theta_E(A)$ が A 上の線型形式 $a\mapsto$ Tr($u\circ a_E$) の集合であることを証明します。ここで、$u$ は End$^f_K(E)$ を通過します。

#### 補題 1 {#alg-viii-s20-lem-1 .statement tag=00MI}

写像 $c''_E$ は全単射です。 E が有限次元であれば、$c'_E$ も有限次元です。

Fが右A-加群、GがK-ベクトル空間のとき、II, §4, No. 1、p. 268、命題 1で、a) Hom$_K(F\otimes_AE,G)$からHom$_A(E$までのK-ベクトル空間の同型$\gamma$、ホム$_K(F,G))$。この同型写像は送る $\varphi : F\otimes_AE\rightarrow G$ から準同型 $e\mapsto (f\mapsto \varphi (f\otimes e))$ です。 $A_d\otimes_AE$ から標準同型を経て E (II, §3, No. 4、$249$ ページ)$,\gamma$ は、$F = A_d$ かつ G = K のとき、$c''_E$ と識別できます。

同様に、II, §4, No. 1、p. 268、命題 1、b) で定義された同型 $\beta$ は、Hom$_K(E^*\otimes_AA_s,K)$ から Hom$_A(E^*$、Hom$_K(A_s,K))$ までの同型 $\beta$ に特化します。 E が有限次元の場合、E は Hom$_K(E^*,K)$ および $E^*$ と $E^*\otimes_AA_s$ で正準的に識別できます。 準同型 $\beta$ は $c'_E$ と識別されます。

#### 命題 2 {#alg-viii-s20-prop-2 .statement tag=00MJ}

Eを左A-加群とします。

a) E の係数の集合は、E から $A^*$ までの A-線型写像の像の和集合です。

b) さらに、E が K に対して有限次元 $n$ を持つと仮定します。そのとき、左A-加群 $\Theta_E(A)$ は $E^n$ の商と同型であり、A-加群 E は $\Theta_E(A)^n$ の部分加群と同型であり、すべて$\Theta_E(A)$の元は$E^n$の係数です。

主張 a) は、$c''_E$ の全主観性から導かれます。

b)を証明しましょう。 $(e^*_1, . . . , e^*_n)$ を K 上の $E^*$ の基底とします。$\Theta_E(A)$ は E の係数によって生成されるため、A-線型写像

$$
(x_1, . . . , x_n)\mapsto \sum_{i=1}^nc_E(x_i, e^*_i)
$$

$E^n$ から $\Theta_E(A)$ は全射です。 a) により、$\Theta_E(A)$ のすべての元は $E^n$ の係数になります。さらに、A-線型写像

$$
x\mapsto (c_E(x, e^*_1), . . . , c_E(x, e^*_n))
$$

E から $\Theta_E(A)^n$ までは単射です。これにより b) が得られます。

#### 注意 3 {#alg-viii-s20-n3-rem-3 .statement tag=00MK}

E を $A^*$ の左 A-部分加群とします。 E の $\varepsilon$ を線型形式 $y\mapsto y(1)$ とします。E のすべての $x$ に対して、$x=c_E(x, \varepsilon )$ があるため、E は $\Theta_E(A)$ の A-部分加群です。

### 4. 制限付きデュアルおよび行列係数

#### 命題 3 {#alg-viii-s20-prop-3 .statement tag=00ML}

$(V, \pi )$ を、代数 A の有限次元線型表現とします。 $\pi$ の核 $\mathfrak{a}$ は、有限余次元の A の両側イデアルであり、$\Theta_{\pi}(A)$ は、次の $\mathfrak{a}$ の直交です。 $A^*$。 写像 $\pi$ 定義する同型のK-ベクトル空間 $\pi (A)$ から $\Theta_{\pi}(A)$ の転置。

End$_K(V)$ は$K,\mathfrak{a}$ 上で有限次元なので、有限余次元の A の両側イデアルです。 ベクトル空間 $\Theta_{\pi}(A)$ は $A^*$ の有限次元部分空間であり、A におけるその直交は $\mathfrak{a}$ に等しい。したがって、定理 7 of II, §7, No. 5, p. 301, 空間により、$\Theta_{\pi}(A)$ は、$A^*$ の $\mathfrak{a}$ の直交になります。また、$\mathfrak{a}$は$\pi$の核なので、$\pi (A)$の双対から$\mathfrak{a}$の直交へ写像$\pi$の転置が定義する同型となります。 $A^*$ (II, §7, No. 5、p. 299、系/定理 5)。

#### 系 {#alg-viii-s20-n4-cor-1 .statement tag=00MM}

A の制限双対 Θ(A) は、A の有限次元線型表現の係数の集合です。

定義により、Θ(A) は、有限余次元の A の両側イデアルの直交関数の和集合になります。したがって、A のすべての有限次元線型表現 $\pi$ に対して $\Theta_{\pi}(A)\subset \Theta (A)$ が得られます。逆に、$f$ を Θ(A) の元とし、$\mathfrak{a}$ を $f$ の核に含まれる有限余次元の両側イデアルとします。 (VIII、p. 376、定義 2)。 $A/\mathfrak{a}$のAの$\pi$線型表現を、Aの正則表現を左から移行から商で推定して表します。 $x$ を 1 の類 (mod $\mathfrak{a}$) とし、$x^*$ を $f$ から推定した $A/\mathfrak{a}$ の線型形式とします。 $f=c_{\pi}(x, x^*)$があるので、$f$は$\pi$の係数になります。

$(V, \pi )$ が K 上の有限次元ではない A の線型表現である場合、空間 $\Theta_{\pi}(A)$ は必ずしも Θ(A) に含まれるわけではないことに注意してください。

### 5. 半単純代数の二重

$\Theta^{ss}(A)$ を左A-加群 Θ(A) のソクル、つまり Θ(A) の (VIII, p. 65) 最大の半単純部分加群とします。 K 上の有限次元である単純 (左) A-加群の類の $\mathscr{S}_K$ 集合で表します。 A が K 上の有限次数の半単純代数であるとき、すべての左A-加群は半単純 (VIII、p. 138、命題 4) であるため、$A^*= \Theta (A) = \Theta^{ss}(A)$ になります。

#### 定理 1 {#alg-viii-s20-thm-1 .statement tag=00MN}

a) 集合 $\Theta^{ss}(A)$ は、A の有限次元半単純表現の係数で構成されます。これは、$A^*$ の $(A,A)$ サブバイモジュールです。

b) すべての $S\in \mathscr{S}_K$ について、型 S の Θ(A) の同型成分は $\Theta_S(A)$ に等しい。 左A-加群 $\Theta^{ss}(A)$ は部分加群 $\Theta_S(A)$ の直和で、S は $\mathscr{S}_K$ を通過します。

c) $\mathscr{S}_K$ のすべての S について、右A-加群 $S^*$ は単純であり、$\Theta_S(A)$ は右A-加群 Θ(A) の型 $S^*$ の同型成分です。 S を cl($S^*$) に送信する写像は、K 上の有限次元の単純な $A^o$ モジュールの類の $\mathscr{S}_K$ から集合までの全単射です。

d) 右A-加群として見ると、Θ(A) はソクル $\Theta^{ss}(A)$ を持ちます。

E を K 上の有限次元の半単純A-加群とします。 E から $A^*$ (VIII, p. 378, 命題 2) まで、E の属するから A-線型写像の像までの各係数とします。 属するから$\Theta^{ss}(A)$まで。逆に$f\in \Theta^{ss}(A)$とします。このとき、A-加群 $Af$ は K 上の有限次元であり、半単純です。 VIIIの注意までに、p. 367$,f$は$Af$の係数になります。

$\mathscr{S}_K$ のすべての S について、型 S の Θ(A) の同型成分は、S から $A^*$ までの A-線型写像の像によって生成されます。したがって、VIII、p. 378 の命題 2、a) により $\Theta_S(A)$ に等しくなります。 一方、S が K 上で有限次元ではない単純A-加群である場合、型 S の Θ(A) の同型成分は零です。実際、Θ(A) のすべての単純部分加群は単次であり、したがって K 上で有限次元です。 Θ(A) のソクルはその同型成分 (VIII, p. 65, 命題 4) の直和であるため、これは b) を証明します。

S を K 上の有限次元の単純A-加群とします。K-ベクトル空間 S は 0 に減らないので、同じことが $S^*$ にも当てはまります。 E を右A-加群 $S^*$ の部分加群とします。 S におけるその直交 $E'$ は S の A-部分加群です。S は単純なので、$E'= 0$ (その場合は $E = S^*$)、または $E'= S$ (この場合は E = 0) のいずれかになります。 したがって、$S^*$ は単純右A-加群です。

$\Theta (A^o) = \Theta (A)$ (VIII、p. 376) があります。 同一視する右A-加群と左側の $A^o$ モジュールです。 K 上の有限次元のすべてのベクトル空間はその双双対と同型であるため、上記は写像 $S\mapsto$ cl($S^*$) が、単純な $A^o$ モジュールの類の $\mathscr{S}_K$ から集合までの全単射であることを証明します。 Kを超える有限次元。 さて、$\mathscr{S}_K$ の S について、型 $S^*$ の $\Theta (A^o)$ の同型成分は、主張 b) 代数 $A^o$ に適用されることで $\Theta_{S^*}(A^o)$ に等しく、$\Theta_{S^*}(A^o) = \Theta_S(A)$ が得られます。 主張 c) と d) がすぐに続きます。

#### 系 1 {#alg-viii-s20-thm-1-cor-1 .statement tag=00MO}

K 上の有限次元のすべての単純A-加群は、Θ(A) の A-部分加群と同型です。

これは、非零 A-加群 E ごとに $\Theta_E(A)\not= 0$ があるため、定理 1、b) から導かれます。

#### 系 2 {#alg-viii-s20-thm-1-cor-2 .statement tag=00MP}

K 上の有限次元の 2 つの単純A-加群が共通の非零係数を持つ場合、それらは同型です。

$S_1$ と $S_2$ を、共通の非零係数を含む K 上の有限次元の単純A-加群とします。次に、$\Theta_{S_1}(A)\cap \Theta_{S_2}(A)\not= 0$ になります。さて、$\Theta_{S_1}(A)$ は型 $S_1$ の同型であり、$\Theta_{S_2}(A)$ は型 $S_2$ の同型です。したがって、$S_1$ は $S_2$ と同型です。

定理 1 により、$\Theta^{ss}(A)$ は、$\mathscr{S}_K$ まで実行される S の $(A$、A)-バイモジュール $\Theta_S(A)$ の $(A$、$A^*$、直和の A) サブバイモジュールです。これらの両側加群は、左A-加群としてすでに非同型であるため、ペアごとに非同型です。

$\mathscr{S}_K$ の S を修正します。 End$_A$(S)の反対側体をDで表し、Sを右D-加群、$S^*$を左D-加群とみなします。これらの規則では、S は $(A$、D)-bimodule、$S^*$ は $(D$、A)-bimodule、$S\otimes_DS^*$ は $(A$、A)-bimodule です。

#### 命題 4 {#alg-viii-s20-prop-4 .statement tag=00MQ}

a) $S\otimes_DS^*$ から $\Theta_S(A)$ までには群準同型 $\lambda_S$ が存在し、以下の特徴があります。

$$
\lambda_S(x\otimes x^*) =c_S(x, x^*) \tag{6}
$$

$x\in S$ と $x^*\in S^*$ の場合。この写像は、$(A,A)$-bimodules の同型です。

b) $(A,A)$-bimodule $\Theta_S(A)$ は単純です。

公式 $\gamma_S(x\otimes x^*) =c_S(x, x^*)$ によって特徴付けられる写像 $\gamma_S: S\otimes_KS^*\rightarrow \Theta_S(A)$ は、$(A$、A)-線形および全射であり、$x\in S,x^*\in S^*$ および $d\in D$ に対して $\gamma_S(xd\otimes x^*)$ $=\gamma_S(x\otimes dx^*)$ を満たします。したがって、それは定義する全射 $(A$、A)-線形写像 $\lambda_S: S\otimes_DS^*\rightarrow \Theta_S(A)$ は公式 (6) によって特徴付けられます。

$S\otimes_DS^*$ が単純な $(A$, A)-bimodule であることを証明しましょう。 VIII、p. 63 の系 2 により、すべての $(A$、$S\otimes_DS^*$ の A) サブバイモジュールは形 $S\otimes_DH$ になります。ここで、H は $(D$、A) サブバイモジュール $S^*$ です。 $S^*$ は単純右A-加群 (VIII, p. 380, 定理 1, c)) であるため、H = 0 または $H = S^*$ になります。 主張が続きます。

準同型 $\lambda_S$ は $(A$、A)-線形および非零; $S\otimes_DS^*$ は単純な両側加群であるため、$\lambda_S$ は単射法 (VIII, p. 47, 命題 2, a)) です。

#### 注意 {#alg-viii-s20-n5-rem-1 .statement tag=00MR}

体 K が代数的に閉じている場合、VIII、p. 47 の定理 1、および $\lambda_S$ は $(A$ の同型、A)-bimodules $S\otimes_KS^*$ から $\Theta_S(A)$ により D = K になります。

### 6. 表現中指標

E を K 上の有限次元の左A-加群とします。E の指標または Tr$_E$ で示される E のトレースは、線型形式 $a\mapsto$ Tr($a_E$) です。 $(e_1, . . . , e_n)$ を E の基底とし、$(e^*_1, . . . , e^*_n)$ をその双対基底とします。 定義までに関係になります

(7) Tr$_E=\sum_{i=1}^nc_E(e_i, e^*_i)$.

線型形式 Tr$_E$ 属するから $\Theta_E(A)$ まで。 E と $E'$ が 2 つの同型 A-加群である場合、Tr$_E=$ Tr$_{E'}$ が得られます。つまり、Tr$_E$はEの同型類のみに依存します。

$\pi$ を、K 上の有限次元のベクトル空間 V における A の線型表現とします。$\pi$、または $\pi$ のときどき指標は、A-加群の指標として定義されます。 $V_{\pi}$。これを Tr$_{\pi}$ で表します。 $(e_1, . . . , e_n)$ が K 上の V の基底であり、この基底に関して $(\pi_{ij}(a))$ が $\pi (a)$ の行列である場合、次のようになります。

(8) Tr$_{\pi}(a) =\sum_{i=1}^n\pi_{ii}(a)$.

線型形式 Tr$_{\pi}$ 属するから $\Theta_{\pi}(A)$ まで。

#### 命題 5 {#alg-viii-s20-prop-5 .statement tag=00MS}

S を K 上の有限次元の単純A-加群とし、D を S の交換子環の反対の体とし、Z を D の中心とします。以下のプロパティは同等です。

(i) S の指標 Tr$_S$ は零ではありません。

(ii) Tr$_{D/K}(d)\not= 0$となるような元$d\in D$が存在します。

(iii) K の拡大 Z は分離可能ですが、K の標数 $p$ は割る次数 [D : Z] ではありません。

右D-ベクトル空間 S は有限次元です。 $(e_1, . . . , e_n)$ を D 上の S の基底とし、$u$ を End$_D(S)$ の元とします。 $(d_{ij})$ を基底 $(e_1, . . . , e_n)$ に関して $u$ の行列とします。 $j\in [1, n]$には$u(e_j) =\sum^n_{i=1}e_id_{ij}$がございます。 $u_K$ 写像 $u$ を K-ベクトル空間 S の自己準同型として、K-ベクトル空間 S の分解 $(e_iD)$ に対して $u_K$ の $(u_{ij})$ 行列を直和として表します。 (II, §10, No. 5、p. 346)。 Tr($u_K$) $=\sum_i$ Tr($u_{ii}$) がいます。 また、$u_{ii}$は$d\in D$に対する$u_{ii}(e_id) =e_id_{ii}d$で定義されたK-ベクトル空間$e_iD$の自己準同型なので、そのトレースはTr$_{D/K}(d_{ii})$と等しくなります。 従って、私たちは等式を証明しました

(9) Tr($u_K$) $=$ Tr$_{D/K}(\sum_id_{ii})$。

バーンサイドの定理 (VIII、p. 83、系 1 of 命題 4) によれば、A から End$_D(S)$ までの写像 $a\mapsto a_S$ は全射法です。従って、性質 (i) と (ii) の同値は、公式 (9) から得られます。

K の拡大 Z が分離可能であれば、Tr$_{Z/K}(d)\not= 0$ (命題 1 の V, §8, No. 2, p. 49, 系) となる元 $d\in Z$ が存在します。さらに、Tr$_{D/K}(d) = [D : Z]$ Tr$_{Z/K}(d)$ (III, §9, No. 4、p. 548、系) があります。従って、$p$ が割る [D : Z] でない場合、Tr$_{D/K}(d)\not=$ 0 になります。これは、(iii) が (ii) を意味することを証明します。

K の拡大 Z が分離可能でない場合、すべての $x\in Z$ に対して Tr$_{Z/K}(x) = 0$ があり、したがってすべての $d\in D$ に対して Tr$_{D/K}(d) =$ Tr$_{Z/K}$(Tr$_{D/Z}(d)$) $= 0$ が得られます。

ここで、$p$ 割る次数 [D : Z] と仮定します。次に、Z に対する D の縮小次数が割るとなります。すべての $d\in D$ に対して、Tr$_{D/Z}(d) = 0$ (VIII, p. 344, 注意) があり、従って Tr$_{D/K}(d) =$ Tr$_{Z/K}$(Tr$_{D/Z}(d)$) となります。 $= 0$。これで、含意 (ii) $\Rightarrow$ (iii) の証明が完了します。

#### 系 {#alg-viii-s20-n6-cor-1 .statement tag=00MT}

体 K が完全な場合、性質 (i) から (iii) が成り立ちます。

体は完全なので、K の拡大 Z は分離可能です (V, §15, No. 5、p. 125、定理 3)。 性質 (iii) は、VIII、p. 323 の系 3 から続きます。

#### 命題 6 {#alg-viii-s20-prop-6 .statement tag=00MU}

$\mathscr{S}_0$ を、非零トレースを使用した K 上の類の単純A-加群の有限次元の集合とします。 線型形式 (Tr$_S$)$_{S\in\mathscr{S}_0}$ の家族は K を超えて無料です。

Fを$\mathscr{S}_0$の有限部分集合、SをFの元とします。仮定までに、Tr$_S(a)\not= 0$となる元$a\in A$が存在します。 命題 4 (VIII、p. 83) の系 1 までに、$T\in F-\{S\}$ ごとに $b_S=a_S$ と $b_T= 0$ が存在するように、元 $b\in A$ が存在します。 $T\in F-\{S\}$にはTr$_S(b)\not= 0$とTr$_T(b) = 0$がございます。したがって、家族 (Tr$_S$)$_{S\in F}$ は無料です。 命題 6が続きます。

#### 注意 {#alg-viii-s20-n6-rem-1 .statement tag=00RR}

$\mathscr{S}_K$ を、K 上の類の単純A-加群の有限次元の集合とします。 命題 6 は、$\mathscr{S}_K$ を通る S の $\Theta_S$(A) の和が直接であるという事実からもわかります。

させて

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

A-加群の完全系列、すべてK上の有限次元になります。III, §9, No. 2、p. 543の命題1により、Tr$_E=$ Tr$_{E'}+$ Tr$_{E''}$が得られます。 グロタンディーク群 $R_K(A)$ (VIII、p. 194) とその普遍性 (VIII、p. 186、命題 4) のうち定義までに、加法群の準同型が存在します。 $R_K(A)$ から $A^*$ までの $\theta$ は、K 上の有限次元のすべての A-加群 E に対して関係 $\theta ([E]) =$ Tr$_E$ によって特徴付けられます。特に、E の半簡略化のトレースは E のトレースと等しくなります。 $\theta$ から推論します。 K-線型写像 $\theta_K: K\otimes_{\mathbf{Z}}R_K(A)\rightarrow A^*$。

#### 系 {#alg-viii-s20-n6-cor-2 .statement tag=00MV}

a) 体 K が標数 0 を持つとします。準同型 $\theta$ と $\theta_K$ は単射です。 K 上の有限次元の 2 つの半単純A-加群は、それらの指標が等しい場合にのみ同型です。

b) 体 K が非零特性 $p$ の完全であると仮定します。すると、準同型 $\theta_K$ は単射であり、$\theta$ の核は $pR_K(A)$ です。 E を K 上の有限次元の半単純A-加群とします。 線型形式 Tr$_E$ は、E が $F^p$ と同型である A-加群 F が存在する場合に限り、 零になります。

$\mathscr{S}_K$ を K 上の類の単純A-加群の有限次元の集合とします。 元 [S]、ここで S は $\mathbf{Z}$ モジュールの $\mathscr{S}_K$、形基底を通過します。 $R_K$(A)、つまり、K-ベクトル空間 $K\otimes_{\mathbf{Z}}R_K(A)$ (VIII、p. 195) の元 $1\otimes [S]$ 形基底です。

体 K が完全であると仮定します。 VIII、p. 383、元 $\theta ([S]) =\theta_K(1\otimes [S]) =$ の命題 6 と系により、$A^*$ の Tr$_S$ は K に対して線形独立です。 したがって、準同型 $\theta_K$ は単射であり、 準同型 $\theta$ の核は、$S\in \mathscr{S}_K$ ごとに $n_S\cdot 1_K= 0$ となるように、$R_K(A)$ の元 $\sum_{S\in\mathscr{S}_K}n_S[S]$ で構成されます。したがって、$\theta$ の核は、$pR_K$(A) に等しくなります。ここで、$p$ は K の特性です。特に、K が特性 0 を持つ場合、準同型 $\theta$ は単射です。

a) の最後の主張は、VIII、p. 190 の系から続きます。

b) の仮定が満たされ、E が K 上の有限次元の半単純A-加群であるとします。 E が $p$ 部分加群の直和が F と同型であるような A-加群 F が存在する場合、加群 F は半単純であり、 K 上の有限次元であり、Tr$_E=p$ Tr$_F= 0$ が得られます。逆に、Tr$_E= 0$とします。 $[E]\in pR_K$(A) があるため、E のすべての単純加群 $S\in \mathscr{S}_K$ の重複度は、$p$ の倍数 (VIII、p. 190、命題 7) です。 $n_S\in \mathbf{N}$ を使用して $p n_S$ と書くことができます。家族$(n_S)$には有限台がいます。 集合 $F =\oplus_{S\in\mathscr{S}_K}S^{n_S}$。次に、$[E] = [F^p]$ があり、E と $F^p$ は同型になります (VIII、p. 190、系)。

E を K 上の有限次元の A-加群とします。$a\in A$ とします。 K[T] モジュール $E[T] = K[T]\otimes_KE$ (III, §8, No. 11、p. 541) の自己準同型 $1_E+ Ta_E$ の $\chi_E(a; T)$ 行列式で表します。 関係があります

(10) $\chi_E(a; T)\equiv 1 +$ Tr$_E(a)T$ (mod $T^2K[T]$)

(同上、公式 (49))。この多項式の定数項は 1 であるため、可逆形式冪系列 (IV, §4, No. 4, p. 30) です。さらに、もし

$$
0\longrightarrow E'\longrightarrow E\longrightarrow E''\longrightarrow 0
$$

が A-加群の完全系列であり、すべて K 上の有限次元である場合、$\chi_E(a; T) =\chi_{E'}(a; T)\chi_{E''}(a,T)$ (III, §8, No. 7, p. 534, 公式 (31)) になります。 グロタンディーク群 $R_K(A)$ (VIII, p. 194) とその普遍性 (VIII, p. 186, 命題 4) の定義によって、から一意な準同型 $\chi_a$ が存在します。 群 $R_K(A)$ から乗法群 1 + TK[[T]] で、K 上の有限次元のすべての A-加群 E に対して $\chi_a([E]) =\chi_E(a; T)$ が計算されます。公式 (10) 関係から推定します。

(11) $\chi_a(x)\equiv 1 +\theta (x)(a)T$ (mod $T^2K[[T]]$)

$x\in R_K(A)$と$a\in A$の場合。

E と $E'$ が K 上の有限次元の 2 つの A-加群であり、同型半単純化すると、$\chi_E(a; T) =\chi_{E'}(a; T)$ になります。

#### 定理 2 {#alg-viii-s20-thm-2 .statement tag=00MW}

$\mathscr{A}$ を K-ベクトル空間 A の生成部分集合とします。 準同型 $\chi_{\mathscr{A}}: R_K(A)\rightarrow$ (1 + TK[[T]])$^{\mathscr{A}}$ は、関係 $\chi_{\mathscr{A}}(x) = (\chi_a(x))_{a\in\mathscr{A}}$ は単射です。

$x$ を $R_K(A)$ の元として、$\chi_{\mathscr{A}}(x) = 1$ とします。 (11) により、$a\in \mathscr{A}$ ごとに $\theta (x)(a) = 0$ が得られ、$\theta (x)$ は A および $\mathscr{A}$ 生成する K-ベクトル空間 A 上の K 線形形式であるため、$\theta (x) = 0$ になります。K の特性が零である場合、これは意味します。 $x= 0$ (VIII、p. 384、系 of 命題 6)、したがってこの場合の結果。これから、K の特性 $p$ が非零であるとします。

まず、K が代数的に閉じている場合を扱います。上記により、loc。引用すると、$x\in pR_K(A)$ になります。 $y\in R_K(A)$ を $x=py$ となるようにします。 $\mathscr{A}$ の元 $a$ ごとに、$\chi_a(y)^p=\chi_a(py) =\chi_a(x) = 1$ があります。従って、$(\chi_a(y)-1)^p= 0$ があり、環 K[[T]] が整域であるため、$\chi_a(y) = 1$ となります。つまり、自己準同型 $\chi_{\mathscr{A}}$ の $y$ 属するから核になります。 帰納法が続き、整数 $n \geq 1$ ごとに $x$ 属するから $p^n R_K(A)$ になります。 $R_K(A)$ は自由な $\mathbf{Z}$ モジュールであるため、これは $x = 0$ を意味し、したがってこの場合の $\chi_{\mathscr{A}}$ の単射性を意味します。

$K$ が代数的に閉じているはずがない場合、$K$ の選ぶ代数閉包 $\overline{K}$ と、群と群準同型の図式を考慮します。

$$
\begin{array}{ccc}
R_K(A) & \xrightarrow{\chi_{\mathscr{A}}} & (1 + TK[[T]])^{\mathscr{A}} \\
|_u & & |_i \\
R_{\overline{K}}(A_{(\overline{K})}) & \xrightarrow{\overline{\chi}_{\mathscr{A}}} & (1 + T\overline{K}[[T]])^{\mathscr{A}},
\end{array}
$$

ここで、$u$ は $K$ から $\overline{K}$ (VIII、p. 195) のスカラーの拡大から推定される準同型、$i$ は標準単射、$\overline{\chi}_{\mathscr{A}}$ は準同型 $z \mapsto (\chi_{1 \otimes a}(z))_{a \in \mathscr{A}}$。 III, §9, No. 1, p. 542, 図式 (12) の公式 (12) は可換です。上記より、準同型 $\overline{\chi}_{\mathscr{A}}$ は単射法です。 $u$ は単射法 (VIII、p. 195、定理 1) なので、準同型 $\chi_{\mathscr{A}}$ は単射法です。

#### 系 1 {#alg-viii-s20-thm-2-cor-1 .statement tag=00MX}

*E と F を K 上の有限次元の半単純A-加群とし、$\mathscr{A}$ を K-ベクトル空間 A の生成部分集合とする。すべての $a \in \mathscr{A}$ について、K-ベクトル空間 E と F の自己準同型 $a_E$ と $a_F$ の特性多項式が次のようになると仮定します。等しい。この場合、A-加群 E と F は同型です。*

$a$を$\mathscr{A}$の元とします。 $a_E$ と $a_F$ の特性多項式は同じ次数を持つため、E の次元は F のそれと等しくなります。それを$n$で表します。 $\mathrm{Pc}_E(a; T)$ を $a_E$ の特性多項式とします。 $K(T)$ では、次の関係が成り立ちます。

$$
\chi_E(a; T) = \det(1 + a_E T) = (-T)^n \det \left( \frac{-1}{T} - a_E \right) = (-T)^n \mathrm{Pc}_E \left( a; \frac{-1}{T} \right),
$$

$\chi_F(a; T)$ は類似の公式によって与えられます。 仮定なので、$\chi_E(a; T) = \chi_F(a; T)$ があります。 定理 2 により、[E] = [F] が得られます。これは、E と F が同型であることを意味します (VIII、p. 190、系の命題 7)。

#### 系 2 {#alg-viii-s20-thm-2-cor-2 .statement tag=00MY}

*A を K 上の有限次数の中心単純代数とします。B を半単純 K-代数とし、f と g を B から A までの代数準同型とし、$\mathscr{B}$ を K-ベクトル空間 B の生成部分集合とします。以下のプロパティは同等です。

(i) $g = \theta \circ f$ となる A の内部自己同型 $\theta$ が存在します。
(ii) すべての $b \in \mathscr{B}$ に対して、$\mathrm{Pc}_{A/K}(f(b); X) = \mathrm{Pc}_{A/K}(g(b); X)$ が得られます。* K が標数0 を持つ場合、これらのプロパティは次と同等です。

(iii) すべての $b\in \mathscr{B}$ に対して、Tr$_{A/K}(f(b)) =$ Tr$_{A/K}(g(b))$ があります。

A の加法群にそれぞれ外部法則 $(b, a)\mapsto f(b)a$ と $(b, a)\mapsto g(b)a$ を与えて得られる M と N 左B-加群で表します。 命題 VIII, p. 257, 性質 (i) の 1 は、B-加群 M と N が同型であるという事実と等価です。 構成により、B の元 $b$ に関連付けられたホモテティー $b_M$ が、A の $f(b)$ により乗法に残されます。従って、関係となります。

PC$_M(b; X) =$ PC$_{A/K}(f(b); X)$、

トレ$_M(b) =$ トレ$_{A/K}(f(b))$

そして 2 つの類似した関係では、置き換える M と N、および $f$ と $g$ です。 VIII, p. 386, 系 1) は、$b\in \mathscr{B}$ ごとに Pc$_M(b; X) =$ Pc$_N(b; X)$ がある場合に限り、B-加群 M と N が同型であることがわかります。 体 K が特性 0 を持つとき、この関係も、すべての $b\in \mathscr{B}$ (命題 6 の VIII、p. 384、系) についての Tr$_M(b) =$ Tr$_N(b)$ と等価です。性質 (i) と (ii)、および K が特性 0 を持つ場合の (i) と (iii) の同値は次のようになります。

### 7. 係数/集合/類/加群

$\mathscr{C}$ を A-加群の類の世襲集合とします (VIII、p. 183、定義 1)。 型 $\mathscr{C}$ のすべての A-加群は K 上の有限次元であり、$\Theta_{\mathscr{C}}(A)$ 集合の係数 、A-加群 、型 $\mathscr{C}$ で表されると仮定します。 VIII、p. 378 の命題 2 により、集合 $\Theta_{\mathscr{C}}(A)$ は、E が $\mathscr{C}$ まで続く A 線形写像 $u: E\rightarrow A^*$ の画像の結合でもあります。それは、$A^*$ の部分空間 $\Theta_E(A)$ の和集合でもあり、E は $\mathscr{C}$ を通過します (上記参照)。 $(A$、$A^*$ の A) サブバイモジュール $(\Theta_E(A))_{E\in\mathscr{C}}$ のファミリーが指示されているため、その和集合 $\Theta_{\mathscr{C}}(A)$ は $(A$、A) サブバイモジュール $A^*$ です。

#### 命題 7 {#alg-viii-s20-prop-7 .statement tag=00MZ}

K 上の有限次元の $A^*$ の左 A-部分加群は、型 $\mathscr{C}$ の場合に限り、$\Theta_{\mathscr{C}}(A)$ に含まれます。

V を K 上の有限次元の $A^*$ の左 A-部分加群とします。VIII、p. 379、注意 3 で$V\subset \Theta_V(A)$ があることが分かりました。 V が型 $\mathscr{C}$ の場合、$\Theta_V(A)\subset \Theta_{\mathscr{C}}$ (A) があり、V は $\Theta_{\mathscr{C}}(A)$ に含まれます。逆に、$\Theta_{\mathscr{C}}(A)$にVが含まれているとします。 $\Theta_{\mathscr{C}}(A)$は有向族$(\Theta_E(A))_{E\in\mathscr{C}}$の和集合であり、VはK上の有限次元なので、Vが$\Theta_E(A)$に含まれるような型$\mathscr{C}$の加群Eが存在します。さて、$\Theta_E(A)$ が $E^n$ の商 (VIII, p. 378, 命題 2) と同型であるような自然数 $n$ が存在します。 $\mathscr{C}$は世襲なので、Vは型の$\mathscr{C}$になります。

#### 系 {#alg-viii-s20-n7-cor-1 .statement tag=00N0}

E を K 上の有限次元の A-加群とします。すると、$\Theta_E(A)$ が $\Theta_{\mathscr{C}}(A)$ に含まれる場合に限り、E は型 $\mathscr{C}$ になります。

条件は明らかに必要です。

逆に、$\Theta_{\mathscr{C}}(A)$ 含む $\Theta_E(A)$ とします。 A-加群 $\Theta_E(A)$ は K 上の有限次元 (VIII, p. 378, 命題 2) なので、型 $\mathscr{C}$ by 命題 7 です。 さて、E が次のような整数 $n\geqslant 0$ が存在します。 $\Theta_E(A)^n$ の A-部分加群 (VIII、p. 378、命題 2) と同型。 $\mathscr{C}$は世襲なので、Eは型$\mathscr{C}$です。

### 8. 制限付きデュアルの余代数構造

A の任意の $a$ について、Θ(A) 上の $\eta (a)$ 線型形式 $f\mapsto f(a)$ で表します。したがって、A から定義する K-線型写像 $\eta$ からベクトル空間 Θ(A) の双対 $\Theta (A)^*$ になります。 集合 $\varepsilon =\eta (1)$。

#### 命題 8 {#alg-viii-s20-prop-8 .statement tag=00N1}

ベクトル空間 Θ(A) には、写像 $\eta : A\rightarrow \Theta (A)^*$ が A から双対の代数 (III, §11, No. 2, p. 579) まで準同型となるような一意の余代数構造 (III, §11, No. 1, p. 574) が存在します。 Θ(A)。 余代数 Θ(A) は共結合的であり、$\varepsilon$ を余単位として認めます。

整数 $n\geqslant 1$ ごとに、$\Theta (A)^{\otimes n}$ から公式で特徴付けられる $A^{\otimes n}$ の双対までの K-線型写像 $j_n$ を考慮します。

$$
\langle j_n(f_1\otimes  \cdots  \otimes f_n), a_1\otimes  \cdots  \otimes a_n\rangle =\prod_{i=1}^n\langle f_i, a_i\rangle \tag{13}
$$

$A^n$の$(a_i)$と$\Theta (A)^n$の$(f_i)$。 命題 16 までに、II, §7, No. 7、p. 308、写像 $j_n$ の (ii) は単射です。 K と A の乗法から推定された $m_K: K\otimes K\rightarrow K$ と $m_A: A\otimes A\rightarrow A$ 写像で表します。 $f, g\in \Theta (A)$ と $a, b\in A$ については、

$$
\langle j_2(f\otimes g), a\otimes b\rangle =m_K\circ (\eta (a)\otimes \eta (b))(f\otimes g)
$$

したがって、私たちは

$$
\langle j_2(t), a\otimes b\rangle =m_K\circ (\eta (a)\otimes \eta (b))(t) \tag{14}
$$

$t\in \Theta (A)\otimes \Theta (A)$ごとに。

#### 補題 2 {#alg-viii-s20-lem-2 .statement tag=00RS}

$c : \Theta(A) \to \Theta(A) \otimes \Theta(A)$ を K-線型写像とします。次に、次の図式が交換する場合に限り、$\eta$ は $A$ から余代数 $(\Theta(A), c)$ の双対代数への準同型になります。

$$
\begin{array}{ccc}
\Theta(A) & \xrightarrow{c} & \Theta(A) \otimes \Theta(A) \\
| & & | \\
A^* & \xrightarrow{t m_A} & (A \otimes A)^*
\end{array}
$$

確かに、すべての $a, b \in A$ に対して $\eta(ab) = m_K \circ (\eta(a) \otimes \eta(b)) \circ c$ がある場合に限り、$\eta$ は $A$ から余代数 $(\Theta(A), c)$ の双対代数までの準同型です。

$$
\eta(ab)(f) = m_K \circ (\eta(a) \otimes \eta(b))(c(f))
$$

$a, b \in A$ と $f \in \Theta(A)$ の場合。さて、私たちは

$$
\eta(ab)(f) = f(ab) = \langle t m_A(j_1(f)), a \otimes b \rangle
$$

そして、(14)により、

$$
m_K \circ (\eta(a) \otimes \eta(b))(c(f)) = \langle j_2(c(f)), a \otimes b \rangle
$$

すべての $a, b \in A$ とすべての $f \in \Theta(A)$ に対して。 補題が続きます。

$j_2$ は単射なので、通勤する上に図式を作る線形写像 $c$ は最大 1 つ存在します。 その存在を証明するために、$t m \circ j_1$の像が$j_2$の中に含まれていることを証明しなければならない証明します。 他の語では、$\Theta(A)$、自然数 $n$、元 $f'_1, \ldots, f'_n, f''_1, \ldots, f''_n$ $\Theta(A)$ 満たす関係のすべての元 $f$ に対して、証明しなければならないが存在すると考えられます。

$$
f(ab) = \sum_{i=1}^n f'_i(a) f''_i(b)
$$

$a, b \in A$の場合。それでは、

$$
c(f) = \sum_{i=1}^n f'_i \otimes f''_i.
$$

VIII、p. 379の系までに、係数として$f$を持つ$K$の上に有限次元の左$A$モジュール$E$が存在します。 $(e_1, \ldots, e_n)$ を、$E$ の基底、$(e_1^*, \ldots, e_n^*)$ 双対基底、$x$ $E$ の元、および$E^*$ の $x^*$ 元として、$f = c_E(x, x^*)$ とします。 $i \in [1, n]$ の場合は集合 $f'_i = c_E(e_i, x^*)$ と $f''_i = c_E(x, e_i^*)$。 A の a、b については、次のようになります。

$$
f(ab) = \langle x^*, abx \rangle = \langle x^* a, bx \rangle = \left\langle \sum_i \langle x^* a, e_i \rangle e_i^*, bx \right\rangle
$$
$$
= \sum_i \langle x^* a, e_i \rangle \langle e_i^*, bx \rangle = \sum_i \langle x^*, ae_i \rangle \langle e_i^*, bx \rangle = \sum_i f_i'(a) f_i''(b),
$$
したがって (16)。

c の共結合性を証明しましょう。これについては、K-線型写像を検討してください。
$$
c' = (c \otimes 1_{\Theta(A)}) \circ c \quad \text{and} \quad c'' = (1_{\Theta(A)} \otimes c) \circ c
$$
$\Theta(A)$ から $\Theta(A)^{\otimes 3}$ まで。 関係あります
$$
\langle j_3(f \otimes c(g)), a \otimes b \otimes c \rangle = \langle f, a \rangle \langle j_2 \circ c(g), b \otimes c \rangle
$$
$$
= \langle f, a \rangle \langle g, bc \rangle
$$
$$
= \langle j_2(f \otimes g), a \otimes bc \rangle
$$
$$
= \langle t(\mathrm{Id}_A \otimes m_A) \circ j_2(f \otimes g), a \otimes b \otimes c \rangle
$$
$f, g \in \Theta(A)$ と $a, b, c \in A$ 用。このことから、次の図式が通勤していると推測されます。

$$
\begin{array}{ccc}
\Theta(A) \otimes \Theta(A) & \xrightarrow{\mathrm{Id}_{\Theta(A)} \otimes c} & \Theta(A) \otimes \Theta(A) \otimes \Theta(A) \\
\downarrow j_2 & & \downarrow j_3 \\
(A \otimes A)^* & \xrightarrow{t(\mathrm{Id}_A \otimes m_A)} & (A \otimes A \otimes A)^*.
\end{array}
$$

この図式の可換性と (15) のそれにより、 $f \in \Theta(A)$ と $a, a', a'' \in A$ については、
$$
\langle j_3 \circ c'(f), a \otimes a' \otimes a'' \rangle = \langle f, (aa')a'' \rangle;
$$
関係を表示できます
$$
\langle j_3 \circ c''(f), a \otimes a' \otimes a'' \rangle = \langle f, a(a'a'') \rangle
$$
同様に。 A の乗法は結合なので、$j_3 \circ c' = j_3 \circ c''$ が得られ、$j_3$ は単射なので $c' = c''$ になります。

最後に、公式 (16) と (17) は、$\Theta(A)$ が $\varepsilon$ を余単位として認めることを意味します。

#### 注意 1 {#alg-viii-s20-n8-rem-1 .statement tag=00N2}

$(\mathbf{V}, \pi)$ を代数 A の有限次元線型表現とします。 Vの基底$(e_1, \ldots, e_n)$と$\mathbf{V}^*$の双対基底$(e_1^*, \ldots, e_n^*)$を紹介します。 補題 2 の証明までに、関係が完成しました
$$
c(c_\pi(x, x^*)) = \sum_{k=1}^n c_\pi(e_k, x^*) \otimes c_\pi(x, e_k^*)
$$

$x\in V$ と $x^*\in V^*$ の場合。 $1\leqslant i, j\leqslant n$、集合 $\pi_{ij}=c_{\pi}(e_j, e^*_i)$の場合。すべての $a\in A$ について、V の基底 $(e_1, . . . , e_n)$ に対する $\pi (a)$ の行列は、$(\pi_{ij}(a))$ に等しくなります。 $1\leqslant i\leqslant n$ と $1\leqslant j\leqslant n$ については、次のようになります。

$$
c(\pi_{ij}) =\sum_{k=1}^n\pi_{ik}\otimes \pi_{kj} \tag{20}
$$

#### 定義 3 {#alg-viii-s20-def-3 .statement tag=00N3}

C を体 K 以上の余代数とし、$c$ を余積とします。 C の部余代数は、$c(C_1)$ が $C\otimes_KC$ の $C_1\otimes_KC_1$ の標準像に含まれるような、C の線形部分空間 $C_1$ です。

$j$を$C_1$の標準単射をCにします。この定義によって、次のような固有の線形写像 $c_1: C_1\rightarrow C_1\otimes_KC_1$ が存在します。

$$
c\circ j= (j\otimes j)\circ c_1 \tag{21}
$$

この関係は、$j$ が $(C_1, c_1)$ から $(C, c)$ (III, §11, No. 1、p. 574) までの余代数の射であることを意味します。

C が共結合である場合、$C_1$ は共結合です。 C が共可換である場合、$C_1$ も共可換です。 C に余単位 $\varepsilon$ がある場合、$\varepsilon$ から $C_1$ の制限は、$C_1$ の余単位になります。

#### 命題 9 {#alg-viii-s20-prop-9 .statement tag=00N4}

Θ を Θ(A) の線形部分空間とします。次のプロパティは同等です。

(i) Θ は Θ(A) の $(A,A)$ サブバイモジュールです。

(ii) Θ は Θ(A) の部余代数です。

(iii) $\Theta  = \Theta_{\mathscr{C}}(A)$ のような K を超える遺伝的集合 $\mathscr{C}$ の類の A-加群の有限次元が存在します。

これら(iii)の性質が成り立つ、集合、$\mathscr{C}$が一意に決まるとします。

最後の主張は、VIII、p. 388 の系から続きます: 集合 $\mathscr{C}$ は、$\Theta_E(A)$ が Θ に含まれるように、K 上の有限次元の A-加群 E の類で構成されます。

(iii) $\Rightarrow$ (ii): Let $\mathscr{C}$ be a hereditary 集合 of 類 of A-加群 of 有限次元 over K. Then $\Theta_{\mathscr{C}}(A)$ is 和集合 of the directed family $(\Theta_E(A))_{E\in\mathscr{C}}$. $\Theta_E(A)$ は、$E\in \mathscr{C}$ (VIII, p. 390, 公式 (19)) ごとに Θ(A) の部余代数であるため、$\Theta_{\mathscr{C}}(A)$ についても同じことが当てはまります。

(ii) $\Rightarrow$ (i): $f\in \Theta (A)$ とします。 $f'_1, . . . , f'_n, f''_1, . . . , f''_n$ を Θ(A) 満たす $c(f) =\sum f'_i\otimes f''_i$ の元とします。 A の $a,b$ には $f(ab) =\sum f'_i(a)f''_i(b)$ があるため、

$$
bf=\sum_{i=1}^nf''_i(b)f'_i,f a=\sum_{i=1}^nf'_i(a)f''_i
$$

(VIII、p. 375、公式 (3) および (4))。従って、Θ(A) の部余代数は、$(A$, A) サブバイモジュールです。

(i) $\Rightarrow$ (iii): Θ が Θ(A) の $(A$, A) サブバイモジュールであると仮定します。 $\mathscr{C}$ を K 上の有限次元の類の A-加群 E の集合とし、$\Theta_E(A)$ が Θ に含まれるようにします。 集合 $\mathscr{C}$ は遺伝性 (VIII、p. 377、注意 2) で、構成までに $\Theta_{\mathscr{C}}(A)\subset \Theta$ が生まれます。 $f\in \Theta$と$E = Af$としましょう。その場合、E は K 上で有限次元になります。その結果、E 上のすべての線型形式は、A の $a$ を含む形 $u_a:g\mapsto g(a)$ になります (II, §7, No. 5、p. 302、系 2)。さて、$a, b, x\in A$ については、

$$
c_E(af, u_b)(x) =\langle u_b, xaf\rangle =f(bxa) =af b(x)
$$

だから$c_E(af, u_b) =af b$。 We therefore have $\Theta_E(A)\subset \Theta$.従って、A-加群 E は型 $\mathscr{C}$ であり、$f$ はその係数の 1 つです。 We therefore have $\Theta \subset \Theta_{\mathscr{C}}(A)$ and, finally, $\Theta  = \Theta_{\mathscr{C}}(A)$.

#### 注意 2 {#alg-viii-s20-n8-rem-2 .statement tag=00N5}

ΘをΘ(A)の部余代数とします。 We endow K with the discrete 位相 and 代数 A with the coarsest 位相 for which 写像 $f: A\rightarrow K$ for $f$ running through Θ are continuous (Gen. Top., I, §2, No. 2, p. 175).この位相は A にトポロジー K-加群の構造を与えます。 A の両側イデアル $\mathfrak{a}$ は、それが有限余次元を持ち、その直交する $\mathfrak{a}'$ が Θ に含まれる場合に限り、開かれます。 By 命題 3 of VIII, p. 379, the open two-sided ideals of 形 a fundamental 系 of neighborhoods of 0 in A. 位相 on A is therefore compatible with its 環構造.

$\mathscr{C}$ を、$\Theta  = \Theta_{\mathscr{C}}$ (VIII, p. 391, 命題 9) となるような、K 上の類の A-加群の有限次元の遺伝的な集合とします。 E を K 上の有限次元の左A-加群とします。これに離散位相を与えます。次のプロパティは同等です。

(i) A-加群 E は型 $\mathscr{C}$ です。

(ii) A-加群 E の消滅子が A で開いています。

(iii) $A\times E$ から E までの写像 $(a, x)\mapsto ax$ は連続しています。

最後の性質は、E がトポロジカル A-加群であることを意味します。

$\Theta^*$ を余代数 Θ の双対代数とします。 $\Theta^*$ に最も粗い位相を与えます。これに対して、$\Theta^*$ から K までの写像 $\varphi \mapsto \varphi (u)$、Θ を通る $u$ は連続です。 代数 $\Theta^*$ の位相は、$\Theta^*$ の加法群構造と互換性があります。 形 $\Theta_E$の集合の $\Theta^*$ の直交行列。ここで、E は型 $\mathscr{C}$ の A-加群、形 0 の近傍の基本系です。 さて、そのような集合はΘの部余代数なので、その直交は$\Theta^*$のイデアルになります。 したがって、$\Theta^*$ の位相は、その環構造と互換性があります。 正準代数準同型性 $\eta : A\rightarrow \Theta^*$ ($a\in A$ を Θ 上の線形形式 $f\mapsto f(a)$ に送る) は、A の完成されたハウスドルフ空間 $\widehat{A}$ からの同型性を定義します (Gen. トップ.、II, §3, No. 7、p. 191) から $\Theta^*$。

### 練習問題 {#alg-viii-s20-exercises}

[§ 20 に対して練習問題](exercises/s20/)を参照してください。
