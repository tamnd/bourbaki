---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 7
section_title: Simple Rings
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.119-A VIII.133
pdf_pages: 0136-0150
extraction: native
subsections:
    - "no": 1
      title: Simple Rings
      page: 119
      pdf_page: 136
    - "no": 2
      title: Modules over a Simple Ring
      page: 122
      pdf_page: 139
    - "no": 3
      title: Degrees
      page: 124
      pdf_page: 141
    - "no": 4
      title: Ideals of Simple Rings
      page: 126
      pdf_page: 143
statements: 24
exercises: 16
content_sha256: a9efd3594ab3332eac678f09e7cbd3e1db11d9db4e46a88e42b30efa6efa8221
translated_from: content/en/alg/VIII/07_s7_simple_rings.md
translation_method: google
source_content_sha256: 0477da2a1cd441904c225c6cad3222346fc38778e44066ddeda16e447e7b81dd
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 9853da46981761e5d22a271aaa563254909ed48947937c8f8a64aacab8cda37a
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 7。シンプル環

### 1. シンプル環

#### 命題 1 {#alg-viii-s7-prop-1 .statement tag=0081}

A を非零環とします。次の条件は同等です。

(i) A-加群 $A_s$ は同型です。

(ii) 環 A は左アルティン的であり、A のすべての両側イデアルは 0 または A に等しい。

(iii) 環 A は左アルティン的であり、単純かつ忠実な左A-加群 S が存在します。

これらの条件が満たされる場合、A-加群 $A_s$ は有限長を持ち、型 S と同型であり、すべての単純A-加群は S と同型です。

(i) が (ii) を意味することを証明しましょう。 (i) が満たされると仮定します。 すると、有限生成A-加群 $A_s$ は半単純なので、有限長があり、アルティン (VIII, p. 71, 命題 10) になります。従って、環 A は左アルティン的となります。 左A-加群 $A_s$ の自己準同型は、A の元による右側乗法です。 左A-加群 $A_s$ は同型であるため、VIII、p. 86 の命題 6、b) から、$(A$、A)-bimodule $_sA_d$ は単純であることがわかります。 The sub-bimodules of $_sA_d$ are the two-sided ideals of A, so (i) implies (ii).

(ii) が (iii) を意味することを証明しましょう。 環 A は 0 に減らされません。その結果、単純A-加群 S が存在します。S の消滅子は、A の適切な両側イデアルです。(ii) が満たされると仮定すると、消滅子は 0 に等しくなります。その場合、A-加群 S は忠実であり、(ii) は (iii) を意味します。

(iii) が (i) を意味することを証明しましょう。 (iii) が満たされていると仮定します。次に、$A_s$ が $S^m$ の部分加群 (VIII, p. 50, 命題 5, a)) と同型となるような整数 $m\geqslant 1$ が存在します。 $S^m$ は型 S の等型A-加群であるため、同じことが $A_s$ (VIII、p. 61、命題 2) にも当てはまります。従って、(iii) は (i) を意味します。

条件 (i) ～ (iii) が満たされるとします。上で、A-加群 $A_s$ が有限長を持ち、型 S と同型であることを見てきました。すべての単純な左A-加群は $A_s$ の商と同型であるため、S と同型です。

#### 定義 1 {#alg-viii-s7-def-1 .statement tag=0082}

環 A は、命題 1 の同等の条件 (i)、(ii)、(iii) を満たす場合、単純であると言います。K を可換体とします。 K-代数は、その基礎となる環が単純である場合、単純であると呼ばれます。

#### 注意 1 {#alg-viii-s7-n1-rem-1 .statement tag=0083}

II, §9, No. 1、p. 115 の定理 1 により、次のプロパティは同等であることを思い出してください。

(i) A-加群 $A_s$ は単純です。

(ii) 環 A は 0 に還元されず、0 または A とは異なる A の左イデアルは存在しません。

(iii) 環 A は体です。

従って、命題 1 (条件 (ii)) により、可換単純環は可換体に他なりません。

#### 注意 2 {#alg-viii-s7-n1-rem-2 .statement tag=0084}

ときどきは、環 A が 0 に還元されず、その両面の理想が 0 と A だけである場合、環 A は準単純であると言います。忠実な単純加群を認める場合、A は原始的であると言います。 命題 1 までに、すべての単純な環は準単純になります。すべての非零環は単純加群と単純加群の消滅子が両面の理想であるため、すべての準単純環は原始的であることがわかります。ただし、単純ではない準単純環や準単純 (VIII、p. 128、練習問題 2) ではない原始環も存在します。そのような環は左アルティン的ではありません。

#### 定理 1 (ウェダーバーン) {#alg-viii-s7-thm-1 .statement tag=00S3}

環は、行列環 $\mathbf{M}_r(D)$ と同型である場合にのみ単純です。ここで、$r\geqslant 1$ は整数および D 体です。

#### 補題 1 {#alg-viii-s7-lem-1 .statement tag=0085}

A を単純な環、S を単純な左A-加群、D を体 End$_A(S)$ の反対環とします。この場合、S は可逆 $(A,D)$-bimodule です。また、D 上の有限次元右ベクトル空間であり、A から End$_D(S)$ までの写像 $a\mapsto a_S$ は環同型です。

命題 1 により、A-加群 $A_s$ は有限長を持ち、型 S と同型です。 従って、A-加群 $A_s$ と $S^m$ が同型であるような整数 $m\geqslant 1$ が存在します。この場合、A-加群 S は射影的であり、有限に生成されます。 VIII、p. 101、(ii)$\Rightarrow$(i)、(ii)$\Rightarrow$(iii)の定理1から続く生成する(VIII、p. 80、定理1)、補題1です。 $(A,D)_{\mathbf{Z}}$-ビモジュール S.

#### 補題 2 {#alg-viii-s7-lem-2 .statement tag=00R7}

D を D 上の有限次元 $r\geqslant 1$ の体と V 右ベクトル空間とする。すると、V は環 E = End$_D(V)$ 上の単純加群であり、その交換子環は $D_V$ に等しい。 環 E は単純で、その左の長さは $r$ に等しい。

V は単純な E モジュール (VIII、p. 45、例 3) であり、その交換子環は $D_V$ (VIII、p. 82、系 1) に等しいことがわかっています。 $(x_i)_{1\leqslant i\leqslant r}$ を体 D 上の V の基底とします。 写像 $u\mapsto (u(x_i))_{1\leqslant i\leqslant r}$ は、E モジュール $E_s$ から E モジュール $V^r$ までの同型です。従って、E 加群 $E_s$ は長さ $r$ と同型であるため、環 E は単純です。

定理 1 を証明しましょう。(II, §10, No. 7, p. 349) 環 $\mathbf{M}_r(D)$ は右D-ベクトル空間 $D^r_d$ の自己準同型環と同一視できることを思い出してください。さらに、体 D 上の有限次元 $r$ のすべての右ベクトル空間は $D^r_d$ (II, §7, No. 1, p. 292) と同型です。従って、定理 1 は、補題 1 と 2 から続きます。

#### 注意 3 {#alg-viii-s7-n1-rem-3 .statement tag=0086}

A を体 End$_A(S)$ の単純な環、S 単純A-加群、D 反対環とします。この場合、A-加群 $A_s$ は有限長を持ち、dim$_D(S)$ は long(A) に等しくなります。実際、補題 1 により、環 A は End$_D(S)$ と同型です。次に、補題 2 を適用します。

#### 系 1 {#alg-viii-s7-lem-2-cor-1 .statement tag=0087}

a) 単純な環の中心は体です。

b) 単純な環の反対環は単純です。

c) 単純な環の左の長さは、その右長さと等しい。

D を体、Z を中心、D の有限次元 $r\geqslant 1$ に対して V 右ベクトル空間とします。 V の自己準同型環を E で表します。

写像 $z\mapsto z_V$ は、VIII、p. 83 の系 2 により、Z から E の中心までの同型です。 主張 a) が続きます。 V の双対 $V^*$ は、D の反対側の体 $D^o$ に対して右ベクトル空間であり、その次元は $r$ に等しい。 写像 $u\mapsto^tu$ は、E の反対環 $E^o$ から環エンド$_{D^o}(V^*)$ までの同型です。従って、環 $E^o$ は単純であり、環 E と $E^o$ は同じ左長さを持ち、$r$ (補題 2) に等しくなります。

#### 系 2 {#alg-viii-s7-lem-2-cor-2 .statement tag=0088}

$r$ と $r'$ を厳密に正の整数とし、D と $D'$ を体とします。 環 $\mathbf{M}_r(D)$ と $\mathbf{M}_{r'}(D')$ は、$r=r'$ と体 D と $D'$ が同型である場合に限り、同型です。

条件で十分であることは明らかです。

逆に、環 $B =\mathbf{M}_r(D)$ と $B'=\mathbf{M}_{r'}(D')$ が同型であるとします。 $r$は$B_s$の長さと$B'_s$の$r'$(補題2)なので、$r=r'$になります。また、BはDと$B'$～$D'$（VIII、p. 102、例1）に相当する森田です。従って、体 D と $D'$ は森田等価であり、したがって同型です (VIII, p. 111, 命題 13, c))。

#### 系 3 {#alg-viii-s7-lem-2-cor-3 .statement tag=0089}

K を可換体とし、A を有限次数の K-代数とし、単純な基礎となる環を持たせます。 体である K 上に有限次数の整数 $r$ と K-代数 D が存在し、A は $M_r(D)$ と同型です。特に、K が代数的に閉じている場合、A は K 上で行列環と同型です。

S を単純な左A-加群とします。それは、K 上の有限次元 K-ベクトル空間です。従って、その交換子環は、K 上の有限次数の代数です。最初の主張は、補題 1 から続きます。K が代数的に閉じている場合、D = K VIII の定理 1 により、 p. 47。

#### 注意 4 {#alg-viii-s7-n1-rem-4 .statement tag=008A}

K を代数的に閉じた可換体とし、A を K 上の有限次数の代数とする。 代数 A は、A が $M_n(K)$ と同型であるような整数 $n\geqslant 1$ が存在する場合に限り、単純である。その中心は K と同型です。

### 2. シンプルな環よりも加群

#### 補題 3 {#alg-viii-s7-lem-3 .statement tag=008B}

A を単純な環とし、S を単純A-加群とします。 S の交換子環の反対の体を D で表します。すべての A-加群は形 $S\otimes_DV$ の A-加群と同型で、V は体 D 上の左ベクトル空間です。

これは、VIII、p. 120 の補題 1、および森田の定理 (VIII、p. 103) に続きます。

#### 命題 2 {#alg-viii-s7-prop-2 .statement tag=008C}

A を単純な環および S 単純A-加群とします。

a) すべての A-加群は射影であり、型 S と同型であるため、半単純です。 長さ $\mathfrak{a}$ がある場合、$S^{(\mathfrak{a})}$ と同型です。

b) すべての非零 A-加群は生成するです。

c) 2 つの A-加群は、同じ長さを持っている場合にのみ同型です。

S の交換子環の反対の体を D で表します。 VIII、p. 120 の補題 1 により、S は可逆 $(A$、D) 双加群です。 M を A-加群とします。 補題 3 により、形 $S\otimes_DV$ の加群と同型であり、V は体 D 上の左ベクトル空間です。

D-加群 V は射影であり、型 $D_s$ の同型です。 0 に減らされない場合に限り、それは生成するです。 最後に、$S\otimes_DV$ の長さは D-ベクトル空間 V の次元に等しく、2 つのベクトル空間は同じ次元を持つ場合にのみ同型です。 命題 VIII、p. 109 の 10 と VIII、p. 110 の 12 を考慮して、命題 2 が続きます。

$r\geqslant 1$を整数とします。 $\mathfrak{a}=r\mathfrak{b}$ となるような基数 $\mathfrak{b}$ が存在する場合、基数 $\mathfrak{a}$ は $r$ で割り切れると言います。これは、$r\mathfrak{a}=\mathfrak{a}($集合理論、III, §6, No. 3、p. 188、系があるため、$\mathfrak{a}$ が無限である場合に当てはまります 3)。この発言から、基数 $\mathfrak{a}$ が $r$ で割り切れる場合、$\mathfrak{a}=r\mathfrak{b}$ のような一意の基数 $\mathfrak{b}$ が存在することがわかります。

#### 系 {#alg-viii-s7-n2-cor-1 .statement tag=008D}

$k$ を可換体とし、A を $k$ 上の有限次数の単純な $k$-代数とします。すべての単純A-加群は $k$ にわたって有限次元です。 2 つの A-加群は、$k$ 上の次元が等しい場合にのみ同型です。

すべての単純A-加群は $A_s$ の商と同型であるため、$k$ 上で有限次元になります。 系 then follows from 命題 2, c).

#### 命題 3 {#alg-viii-s7-prop-3 .statement tag=008E}

A を単純な環とします。 A-加群 M は、その長さが A の長さで割り切れる場合に限り、自由です。その場合、M のすべての基底は同じ基数を持ち、dim$_A(M)$ (II, §7, No. 3, p. 294, 注意 2) で示され、次のように決定されます。 関係

(1) 長い$_A(M) =$ 長い(A) $\cdot$ 暗い$_A(M)$。

M が自由で、$(e_i)_{i\in I}$ を M の基底とします。 A-加群 M は、A-加群 $Ae_i$ の直和であり、それぞれ $A_s$ と同型です。 集合 $r=$ 長さ$_A(A_s)$;これは、整数 1 以上です (VIII、p. 119、命題 1)。 VIII、p. 73の公式(13)によるロング$_A(M) =r$カード(I)を持っています。

逆に、基数long$_A(M)$が$r$で割り切れるとします。 $\mathfrak{a}$ を $_A(M) =r\mathfrak{a}$ ほど長い基数とします。この場合、A-加群 M は $A^{(\mathfrak{a})}_s$ と同じ長さを持ち、したがって命題 2 によってそれに同型です。これは M が自由であることを証明します。

#### 命題 4 {#alg-viii-s7-prop-4 .statement tag=008F}

A を単純な環および M 非零 A-加群とします。 A-加群 M の自己準同型環を B で表し、M を左B-加群と見ます。

a) 写像 $a\mapsto a_M$ は、A から B-加群 M の自己準同型環までの同型です。

b) M が A-加群として有限長を持っているとします。すると、環 B は単純で、次のようになります。

(2) ロング$_A(M) =$ ロング(B) とロング$_B(M) =$ ロング(A)。

A-加群 M は、VIII、p. 122 の命題 2 により、生成するになります。 定義までに $B = A'_M$ が得られ、主張 a) は、VIII、p. 82 の定理 2 から続きます。

M が有限長の A-加群であるとします。 選ぶ単純A-加群 S、そして D を S の自己準同型環の反対の体とします。 補題 3 により、A-加群 M は形 $S\otimes_DV$ の加群と同型になります。 V は体 D を超える左ベクトル空間です。 ベクトル空間 V は有限次元です。 VIII、p. 64、環の定理 3 により、B は End$_D(V)$ と同型です。従って、補題 2 (VIII, p. 121), 環 B は単純です。 VIII、p. 63 の注意 1 を考慮すると、次の等式が得られます。

ロング(B) = ディム$_D(V) =$ ロング$_A(M)$。

By Remarks 1 of VIII, p. 63 and 3 of VIII, p. 121, we have the relations

ロング$_B(M) =$ ロング$_{End_D(V)}(S\otimes_DV) =$ ディム$_D(S) =$ ロング(A)、

これで最後の関係が得られます。

### 3. 次数

B の環 B と部分環 A を考えます。B に、$_sB_d$ の $(B$, B)-バイモジュール構造からスカラーの制限によって推定される $(A$, A)-バイモジュールの構造を与えます。

#### 命題 5 {#alg-viii-s7-prop-5 .statement tag=008G}

Bを環、AをBの単純な部分環、Sを単純な左A-加群とします。するとBは次元ロング$_A(B\otimes_AS)$のフリー左A-加群です。

$r$ を A の長さとします。 A-加群 $A_s$ は $S^r$ と同型です。さて、左A-加群 B は $B\otimes_AA_s$ (II, §3, No. 4, p. 249) と同型なので、$(B\otimes_AS)^r$ (II, §3, No. 7, p. 255, 命題 7) となります。従って、ロング$_A(B) =r$ロング$_A(B\otimes_AS)$があり、VIII、p. 123の命題3から命題5が続きます。

#### 定義 2 {#alg-viii-s7-def-2 .statement tag=008H}

Bを環、AをBの単純な部分環とします。自由左A-加群Bの次元は、A上のBの(左)次数と呼ばれ、[^1]$[B : A]_s$で表されます。

置き換えること A と B と反対環により、上記から B は自由な右A-加群であると推定されます。その次元を $[B : A]_d$ で表し、A 上の B の右側次数と呼びます。

We can give an example of a field B and a subfield A such that the degrees $[B : A]_s$ and $[B : A]_d$ differ.[^2]

Bを環、AをBの単純な部分環、Sを単純な左A-加群とします。 M を左A-加群とし、$\mathfrak{a}$ を長さとします。 A-加群 M と $S^{(\mathfrak{a})}$ は同型 (VIII、p. 122、命題 2) であるため、B-加群 $B\otimes_AM$ と $(B\otimes_AS)^{(\mathfrak{a})}$ も同様です。 関係

(3) 長い$_A(B\otimes_AM) = [B : A]_s$ 長い$_A(M)$

命題 5 と定義 2 から続きます。

#### 命題 6 {#alg-viii-s7-prop-6 .statement tag=008I}

Cを環、BをCの単純な部分環、AをBの単純な部分環とします。すると、$[C : A]_s= [C : B]_s[B : A]_s$が得られます。

左B-加群として見たCの基底$(e_i)_{i\in I}$と左A-加群として見たBの基底$(f_j)_{j\in J}$を紹介しましょう。次に、家族 $(f_je_i)_{j\in J,i\in I}$ は、左A-加群 (II, §1, No. 13、p. 222、命題 25) として表示される、C の基底です。 命題 6が続きます。

#### 注意 1 {#alg-viii-s7-n3-rem-1 .statement tag=008J}

A が単純な環 B の単純な部分環であり、右辺次数 $[B : A]_d$ が有限であると仮定します。 C を右A-加群として見た B の自己準同型環とします。それは、VIII、p. 123 の命題 4、b) による単純な環です。 B の任意の $b$ について、B から B までの $\gamma (b)$ を写像 $x\mapsto bx$ とします。すると、$\gamma :b\mapsto \gamma (b)$はBからCの部分環までの同型です。さらに、$(x_1, . . . , x_m)$が右A-加群Bの基底であれば、$c$を$(c(x_1), . . . , c(x_m))$に送る射は、Cから$B^m_s$までの左B-加群の同型になります。従って、関係となります。

$$
[C :\gamma (B)]_s= [B : A]_d \tag{4}
$$

VIII、p. 123 の関係 (2) を右A-加群 B に適用すると、次のことがわかります。

(5) ロング(C) $= [B : A]_d$ ロング(A)。

#### 注意 2 {#alg-viii-s7-n3-rem-2 .statement tag=008K}

Kを可換体とします。 A が K 上の有限次数の代数 B の単純部分代数である場合、A 上の B の左次数は、VIII、p. 125 の命題 6 によって、関係 $[B : A]_s[A : K] = [B : K]$ を満たします。同様に、$[B : A]_d[A : K] = [B : K]$もあります。 等式 $[B : A]_s= [B : A]_d$ が続きます。

### 4. シンプル環の理想

D を有限次元 $n\geqslant 1$ の D に対して体および V 右ベクトル空間とします。単純な環 A = End$_D(V)$ を考えてみましょう。 V の線形部分空間 W について、元の集合満たすの $a$ $aW = 0$ (それぞれ $aV\subset W$) を $\mathfrak{a}(W)$ (それぞれ $\mathfrak{b}(W)$) で表します。

#### 命題 7 {#alg-viii-s7-prop-7 .statement tag=008L}

a) 写像 $W\mapsto \mathfrak{a}(W)$ は、A の左イデアルのV から集合の線形部分空間の集合からの全単射です。

b) 写像 $W\mapsto \mathfrak{b}(W)$ は、A の正しい理想のV から集合の線形部分空間の集合からの全単射です。

c) $W_1$ と $W_2$ を V の線形部分空間とします。 関係 $W_1\subset W_2$、$\mathfrak{a}(W_1)\supset \mathfrak{a}(W_2)$、$\mathfrak{b}(W_1)\subset \mathfrak{b}(W_2)$ は同等です。

主張 b) は、関係 $W_1\subset W_2$ および $\mathfrak{b}(W_1)\subset \mathfrak{b}(W_2)$ の同値と同様に、VIII、p. 104 の $(D^o,A^o$)-bimodule V に適用される例 1、b) から続きます。

$V^*$ を、D の反対側の体 $D^o$ に対する右ベクトル空間として見た、V の双対とします。 V の任意の部分空間 W について、$V^*$ における W の直交を $W'$ で表します。 写像 $W\mapsto W'$ は、V の部分空間の集合から $V^*$ の部分空間の集合までの全単射です。 $W_1$ と $W_2$ が V の 2 つの部分空間である場合、関係 $W_1\subset W_2$ と $W'_1\supset W'_2$ は同等です。さて、写像 $u\mapsto^tu$ は、A から End$_{D^o}(V^*)$ の反対環までの同型です。 変換 A の左理想を End$_{D^o}(V^*)$ と $\mathfrak{a}(W)$ の右理想を集合 $\mathfrak{b}(W')$ 自己準同型 $h$ $V^*$ のように$h(V^*)\subset W'$ になります。 主張 a)、ならびに関係 $W_1\subset W_2$ および $\mathfrak{a}(W_1)\supset \mathfrak{a}(W_2)$ の同値から、V の双対 $V^*$ について b) と同様に主張から続きます。

#### 系 {#alg-viii-s7-n4-cor-1 .statement tag=008M}

a) A の最小左イデアルはイデアル $\mathfrak{a}(H)$ で、H は V の超平面です。 A の最大左イデアルは、イデアル $\mathfrak{a}(L)$ です。ここで、L は V の線です。

b) A の最小の正しい理想は、理想 $\mathfrak{b}(L)$ です。ここで、L は V の線です。 A の最大右イデアルはイデアル $\mathfrak{b}(H)$ で、H は V の超平面です。

$(L_i)_{i\in I}$ を直和 V の線の族とします。 $(\varepsilon_i)_{i\in I}$ を、分解 $V =\oplus_{i\in I}L_i$ に関連付けられた射影子のファミリーとします。 $\varepsilon_i$ は A でべき等であり、$i\not=j$ と $\sum_{i\in I}\varepsilon_i= 1$ に対して $\varepsilon_i\varepsilon_j= 0$ が得られます。 超平面 $\sum_{j\not=i}L_j$ を $H_i$ で表します。 $\varepsilon_i$の核です。次に、

$$
\mathfrak{a}(H_i) = A\varepsilon_i,\mathfrak{b}(L_i) =\varepsilon_iA
$$

The A-module $A_s$ is the direct sum of the family $(\mathfrak{a}(H_i))_{i\in I}$ of minimal left ideals, and $A_d$ is the direct sum of the family $(\mathfrak{b}(L_i))_{i\in I}$ of minimal right ideals.

特定のケース $V = D^n_d$ と同一視する A と行列環 $\mathbf{M}_n(D)$ を考えてみましょう。 Denote the interval $[1, n]$ in $\mathbf{N}$ by I and the canonical basis of V by $(v_i)_{i\in I}$; set $L_i=v_iD$, and denote by $E_{ij}$ the matrix units (II, §10, No. 3, p. 341). すると$\varepsilon_i= E_{ii}$になります。 左の理想 AE$_{ii}$ は DE$_{1i}+\cdots +$ DE$_{ni}$ に等しく、行列と零に等しい $i$ 番目を除くすべての列で構成されます。 右イデアル $E_{ii}A$ は DE$_{i1}+\cdots +$ DE$_{in}$ に等しく、行列で構成され、$i$ 番目を除くすべての行が零に等しい。 関係もあります

$$
E_{ii}A E_{jj}= E_{ii}A\cap A E_{jj}= D E_{ij}
$$

1 と $n$ の間の $i$ と $j$ の場合。

### 練習問題 {#alg-viii-s7-exercises}

[§ 7 に対して練習問題](exercises/s7/)を参照してください。

[^1]: A と B が可換体の場合、[B : A] に等しい次数と、V, §6, No. 5、p. 31 で定義され、$[B : A]_s$ で示される A の分離可能な拡大 B の次数を混同しないように注意してください。
[^2]: cf. A. H. スコフィールド、アーティンのスキュー 体拡大の問題、数学。 手順 ケンブリッジ・フィロス。 社会 **97** (1985)、1 ～ 6 ページ。
