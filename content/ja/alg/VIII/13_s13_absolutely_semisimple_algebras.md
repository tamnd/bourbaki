---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 13
section_title: Absolutely Semisimple Algebras
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.229-A VIII.249
pdf_pages: 0246-0266
extraction: native+ocr
subsections:
    - "no": 1
      title: Absolutely Semisimple Modules
      page: 229
      pdf_page: 246
    - "no": 2
      title: Algebras over Separably Closed Fields
      page: 230
      pdf_page: 247
    - "no": 3
      title: Absolutely Semisimple Algebras
      page: 231
      pdf_page: 248
    - "no": 4
      title: Characterization of Absolutely Semisimple Modules
      page: 235
      pdf_page: 252
    - "no": 5
      title: Derivations on Semisimple Algebras
      page: 236
      pdf_page: 253
    - "no": 6
      title: Cohomology of Algebras
      page: 239
      pdf_page: 256
    - "no": 7
      title: Cohomology of Absolutely Semisimple Algebras
      page: 241
      pdf_page: 258
    - "no": 8
      title: The Splitting of Artinian Algebras
      page: 243
      pdf_page: 260
statements: 33
exercises: 12
content_sha256: 49c1c41f857946f9bcaa157fa93b2eddf5c5f7404c1646cf0d4e64aadf86f66d
translated_from: content/en/alg/VIII/13_s13_absolutely_semisimple_algebras.md
translation_method: google
source_content_sha256: 20e8293964011d4b021666f811555994484c4df5ad3a8aa7a6c4c31c70bdaac0
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 1a8bfdbfc448afc5848f36751131b5cd1f29c5dbfc0e3cfc6b8522a8934f81fa
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 13。 絶対半単純多元環

### 1. 絶対半単純加群

#### 定義 1 {#alg-viii-s13-def-1 .statement tag=00F9}

K を可換体、A を K-代数とします。 $A_{(L)}$ モジュール $M_{(L)}$ が K のすべての拡大 L に対して半単純である場合、A-加群 M 絶対半単純と呼びます。

すべての絶対半単純加群は半単純です。 Conversely, if the field K is perfect, then every semisimple A-module that is finite-dimensional over K is absolutely semisimple (VIII, p. 222, Corollary 1, a)) because every extension of a perfect field is separable (V, §7, No. 1, p. 36, Proposition 2).

#### 命題 1 {#alg-viii-s13-prop-1 .statement tag=00FA}

Kを可換体、AをK-代数とします。

a) 絶対半単純 A-加群のすべての直和は絶対半単純 A-加群です。 絶対半単純加群のすべての部分加群と商加群は絶対半単純です。

b) M を A-加群とし、L を体 K の拡大とする。$A_{(L)}$ モジュール $M_{(L)}$ が絶対半単純である場合に限り、A-加群 M は絶対半単純となる。

主張 a) は、半単純加群に対する類似の主張から続きます (VIII、p. 56、系 1 および 3)。

A-加群 M が絶対半単純で、$L'$ が L の拡大であるとします。 $A_{(L')}$ 加群として、$L'\otimes_LM_{(L)}$ は $M_{(L')}$ (II, §5, No. 1、p. 273、命題 2) と同型です。したがって、それは半単純加群です。これは$M_{(L)}$が絶対半単純であることを証明します。

逆に、$M_{(L)}$が絶対半単純だとします。 $L'$ を K の拡大とします。L と $L'$ (V, §2, No. 4, p. 13, 系) の合成拡大 $(\Omega , u, v)$ が存在します。 同一視する L と $L'$ は Ω のサブエクステンションです。 $A_{(\Omega )}$ 加群 $M_{(\Omega )}$ は $(M_{(L)})_{(\Omega )}$ と同型です。したがって、それは半単純です。しかし、$M_{(\Omega )}$ は$(M_{(L')})_{(\Omega )}$ と同型であり、命題 8、VIII、p. 222 の a) は、$M_{(L')}$ が半単純であることを意味します。つまり、M は絶対半単純です。

#### 命題 2 {#alg-viii-s13-prop-2 .statement tag=00FB}

K を可換体、A K-代数、K 上の有限次元である M A-加群とします。次のプロパティは同等です。

(i) A-加群 M は絶対半単純です。

(ii) $A_{(P)}$ 加群 $M_{(P)}$ が半単純となるような完全体である K の拡大 P が存在します。

(iii) A-加群 M は半単純であり、その交換子環の中心は体 K 上のエタール代数です。

(i) が (ii) を意味することは明らかです。 (ii) が成り立つと仮定します。その場合、$A_{(P)}$ モジュール $M_{(P)}$ は、系 1、a) の VIII、p. 222 によって絶対半単純になります。 命題 1、b) により、M は絶対半単純になります。したがって、(ii) は (i) を意味します。

M が半単純であるとします。 Z を M の交換子環の中心とします。 体 K 上の有限次数の可換代数です。 L が K の拡大である場合、VIII、p. 222 の命題 8、b) から、$A_{(L)}$ モジュール $M_{(L)}$ は次のようになります。 環 $Z_{(L)}$ が減らされた場合に限り、半単純したがって、(i) と (iii) の同値は、V, §6, No. 7、p. 34 の定理 4 から続きます。

### 2. 代数分離閉体

#### 補題 1 {#alg-viii-s13-lem-1 .statement tag=00FC}

D を体、Z を中心とします。 Z の特性指数を $p$ で表します。 D のすべての元 $a$ に対して、$a^{p^m}$ 属するから Z となるような整数 $m\geqslant 0$ が存在するとします。そのとき、体 D は可換です。

$p= 1$ の場合、D = Z。したがって、$p >1$ と仮定します。

矛盾によって証明を与え、D が可換でないものと仮定しましょう。 $a$ を D-Z の元および $p$ の $q$ 冪とし、$a^q$ 属するを Z とします。 D 上の恒等写像を I で表し、$a$ に関連付けられた D から D までの内部自己同型 $x\mapsto axa^{-1}$ を $\sigma$ で表します。 Z に対して $a^q$ 属するであるため、$\sigma^q= I$ があります。 $a$ は Z に対して属するを持たないため $\sigma -I\not= 0$ があり、Z には特性 $p$ があるため $(\sigma -I)^q=\sigma^q-I = 0$ があります。 $f$ を最大の自然数として、$(\sigma -I)^f\not= 0$ とします。 $f\geqslant 1$ があります。 $(\sigma -I)^f(c)\not= 0$、および集合などの D の選ぶ元 $c$

$$
x= (\sigma -I)^{f-1}(c),y= (\sigma -I)(x) = (\sigma -I)^f(c)
$$

構成までに、$y\not= 0$と$\sigma (y) =y$ができます。 集合 $z=y^{-1}x$ とすれば、次のようになります。

$$
\sigma (z) =\sigma (y)^{-1}\sigma (x) =y^{-1}(y+x) = 1 +z
$$

したがって、自然数 $j$ ごとに $\sigma (z^{p^j}) = 1 +z^{p^j}$ となります。 選ぶ整数 $m\geqslant 0$ は、$z^{p^m}$ 属するから中心 Z of D になります。我々は持っています

$$
z^{p^m}=az^{p^m}a^{-1}=\sigma (z^{p^m}) = 1 +z^{p^m}
$$

この矛盾は補題 1 を意味します。

#### 命題 3 {#alg-viii-s13-prop-3 .statement tag=00FD}

K を分離閉体 (V, §7, No. 8, p. 45, 定義 4) とし、D を K 上の有限次数の代数、つまり体とします。この場合、D は可換です。

K の特性指数を $p$ で表します。 $a$ を D の元とします。 環 $K[a]$ は K (V, §3, No. 1, p. 17, 系 1) の代数拡大です。 体 K は可分閉であるため、V, §7, No. 7、p. 44、命題 13 から、代数 $K[a]$ は K の $p$ 根拡張であることがわかります。従って、$a^{p^m}$ となるような整数 $m\geqslant 0$ が存在します。 属するから K。補題 1 により、体 D は可換になります。

#### 系 {#alg-viii-s13-n2-cor-1 .statement tag=00FE}

K を K 上の有限次数の分離閉体および A 半単純代数とします。すると、A が代数と同型となるように、有限次数の K の整数 $r\geqslant 0$、厳密には正の整数 $n_1, . . . , n_r$、および拡大 $K_1, . . . ,K_r$ が存在します。 $\prod_{i=1}^r\mathbf{M}_{n_i}(K_i)$。

半単純代数 (VIII、p. 135、定理 1) に対する構造定理により、A は代数 $\prod^r_{i=1}\mathbf{M}_{n_i}(D_i)$ と同型であり、$r$ は整数 $\geqslant 0,n_1, . . . , n_r$ は厳密には正の整数であり、 $D_1, . . . ,D_r$は、有限次数のK-代数、つまり体です。 体 K は可分に閉じているため、各体 $D_i$ は命題 3 によって可換です。 系が続きます。

### 3. 絶対半単純多元環

#### 定義 2 {#alg-viii-s13-def-2 .statement tag=00FF}

Kを可換体とします。 K のすべての拡大 L に対して環 $A_{(L)}$ が半単純である場合、K-代数 A は絶対半単純であると言います。

絶対半単純多元環は半単純です。 A-加群 $A_s$ が絶対半単純である場合に限り、K-代数 A は絶対半単純になります。従って、VIII、p. 229の命題 1により、次の結果が得られます: LがKの拡大である場合、K-代数 Aが絶対半単純である場合に限り、L-代数$A_{(L)}$は絶対半単純になります。

#### 定理 1 {#alg-viii-s13-thm-1 .statement tag=00FG}

Kを可換体、AをK-代数とします。次のプロパティは同等です。

(i) K-代数 A は絶対半単純です。

(ii) 代数 A は K 上に有限次数を持ち、K の完全体である拡大 P が存在し、その P 代数 $A_{(P)}$ は半単純です。

(iii) K-代数 A は半単純で、K 上に有限次数があり、その中心はエタール K-代数です。

(iv) There exists a finite family $(n_i,D_i)_{i\in I}$, where $n_i$ is a strictly positive integer and $D_i$ a K-algebra of finite degree that is a field, such that the center $Z_i$ of $D_i$ is a separable extension of K for every $i\in I$ and A is isomorphic to the product of the matrix rings $\mathbf{M}_{n_i}(D_i)$.

(v) L-代数 $A_{(L)}$ が代数 $\prod_{i\in I}\mathbf{M}_{n_i}(L)$ と同型となるような、K の拡大 L と整数 $(n_i)_{i\in I}$ の有限族が存在します。

(vi) $A_{(L)}$ が行列環 $\mathbf{M}_{n_i}(L)$ の積と同型となるような、有限次数の K のガロア拡大 L と整数 $(n_i)$ の有限族が存在します。

まず、含意 (v) $\Rightarrow$ (iv) $\Rightarrow$ (iii) $\Rightarrow$ (ii) $\Rightarrow$ (i) を証明します。 A の中心を Z で表します。

性質 (v) が成り立つ場合、L-代数 $A_{(L)}$ は半単純で、L 上の有限次数とその中心 ($Z_{(L)}$、III、p. 41、 系) は、一部の整数 $r\geqslant 0$ では $L^r$ と同型です。 系 2 により、VIII, p. 222, 代数の a) A は半単純であり、K 上で有限次数を持ちます。従って、環 $\prod_{i\in I}\mathbf{M}_{n_i}(D_i)$ の有限積と $n_i\geqslant 1$ と同型です。すべての $i\in I$ に対して、体 $D_i$ は、K 上の有限次数の代数です。中心 $D_i$ の $Z_i$ は、K の拡大である可換体であり、Z は次と同型です。 $\prod_{i\in I}Z_i$。従って、$Z_{(L)}$ は、一方では$\prod_{i\in I}(Z_i)_{(L)}$、他方では$L^r$ と同型です。他の語, 代数 $\prod_{i\in I}Z_i$ は体 K (V, §6, No. 3, p. 28, 定義 1) 上でエタールであり、拡大 $Z_i$ はそれぞれ K (V, §6, No. 4, p. 31、系、およびV, §7, No. 1、p. 42）。従って、(v) は (iv) を意味します。

性質 (iv) が成り立つ場合、A は半単純代数であり、K に対して有限次数を持つことは明らかです。その中心 Z は、有限次数の K の分離拡大の積 $\prod_{i\in I}Z_i$ と同型です。従って、それはエタール代数 (前掲) です。従って、(iv) は (iii) を意味します。

(iii) $\Rightarrow$ (ii) $\Rightarrow$ (i) の意味は、VIII の命題 2、p. 230 からA-加群 $A_s$ に適用されます。

#### 補題 2 {#alg-viii-s13-lem-2 .statement tag=00FH}

L を代数閉体とし、その中心で D 体含む L とします。 D が L と異なる場合、環 $D\otimes_LL'$ は左アルティン的ではない、L の拡大 $L'$ が存在します。

$x$ を D の元 - L とします。 L は代数的に閉じているため、L の拡大 $L'= L(x)$ は代数的ではなく、$x$ は L を超越しています。 環 $B = L'\otimes_LL'$ は、V, §17, No. 4、p. 141 の命題 5 により整域になります。

B の元 $y=x\otimes 1-1\otimes x$ は零ではありませんが、$\varphi$ が B から $L'$ への準同型で、$\xi \otimes \eta$ を $\xi \eta$ に送信すると、$\varphi (y) = 0$ があり、従って $y$ は B で反転できません。 環 $C = D\otimes_LL'$ を部分環 B 上の右加群として。 D は部分体 $L'$ を超える右ベクトル空間であるため、それは自由加群です。 $y$ は整域 B の非零と非可逆元なので、C の $y$ による右乗法は写像 $R_y$ となり、単射ですが全単射ではありません。さて、$R_y$ は左の C モジュール $C_s$ の自己準同型です。従って (VIII, p. 28, 系 1)、環 C は左アルティン的ではありません。

ここで、(i) が (v) を意味することを証明しましょう。これは次の補題中の帰結です。

#### 補題 3 {#alg-viii-s13-lem-3 .statement tag=00FI}

A を K の絶対半単純 K-代数および L 代数閉拡大とします。すると、代数 $A_{(L)}$ は、L 上の有限多の行列環の積と同型です。

L-代数 $A_{(L)}$ は半単純です。従って、形 $\mathbf{M}_{n_i}(D_i)$ の有限多代数の積と同型です。ここで、$D_i$ は、中心と $n_i$ で体含む L です。 整数 $\geqslant 1$ (VIII、p. 137、注意 1)。

$L'$をLの拡大とします。 K-代数 A は絶対半単純であるため、環 $A_{(L')}$ は半単純、したがって左アルティン的です。さて、環 $A_{(L')}$ は $L'\otimes_LA_{(L)}$ と同型なので、$\prod_{i\in I}\mathbf{M}_{n_i}(L'\otimes_LD_i)$ となります。 命題 VIII、p. 7 の 5 より、それぞれの環 $\mathbf{M}_{n_i}(L'\otimes_LD_i)$ は左アルティン的になります。

$n\geqslant 1$を整数、Bを環とします。 $(\mathfrak{b}_r)_{r\geqslant 0}$をBの左イデアの減少列とする。 $\mathfrak{c}_r$ 集合、正方行列、位数 $n$ で表され、$\mathfrak{b}_r$ にエントリが含まれます。すると、$(\mathfrak{c}_r)_{r\geqslant 0}$は$\mathbf{M}_n(B)$の左理想の減少列になります。特に、環 $\mathbf{M}_n(B)$ が左アルティン的であれば、B も同様です。

上記により、L のすべての $i\in I$ とすべての拡大 $L'$ に対して、環 $D_i\otimes_LL'$ は左アルティン的になります。 補題 2 までに、$i\in I$ ごとに $D_i= L$ が得られ、これは補題 3 を意味します。

次の補題を使用して、含意 (i)$\Rightarrow$(vi) を証明します。

#### 補題 4 {#alg-viii-s13-lem-4 .statement tag=00FJ}

A と B を有限生成集合を持つ体 K 上の代数とし、$K'$ を K の拡大とします。 $K'$-代数 $A_{(K')}$ と $B_{(K')}$ が同型である場合、 L-代数 $A_{(L)}$ と $B_{(L)}$ が同型となるように、K 上で有限生成された $K'$ の部分拡張 L が存在します。

代数 A と B に対して、$(e_i)_{i\in I}$ と $(f_j)_{j\in J}$ をそれぞれ有限生成集合とします。 $u$ を $A_{(K')}$ から $B_{(K')}$ および $v$ 逆同型の同型とします。 K 上で有限生成された $K'$ の部分拡張 L が存在し、$i\in I$ ごとに $u(1\otimes e_i)\in B_{(L)}$ が、$j\in J$ ごとに $v(1\otimes f_j)\in A_{(L)}$ が存在します。その結果、$u$ は $A_{(L)}$ を $B_{(L)}$ に送信し、$v$ は $B_{(L)}$ を $A_{(L)}$ に送信します。誘導された写像 $u': A_{(L)}\rightarrow B_{(L)}$ と $v': B_{(L)}\rightarrow A_{(L)}$ は環準同型です。彼らは逆全単射です。

含意 (i)$\Rightarrow$(vi) の証明を完了しましょう。 $K'$ を K (V, §7, No. 8, p. 45) の分離閉包とします。すると、$A_{(K')}$は$K'$より絶対半単純多元環になります。含意 (i)$\Rightarrow$(iv) により、$K'$-代数 $A_{(K')}$ は積 $\mathbf{M}_{n_1}(D_1)\times \cdots \times \mathbf{M}_{n_r}(D_r)$ と同型であり、ここで $D_i$ は体である有限次数の $K'$-代数です。 中心 $Z_i$ は $K'$ の分離拡大です。 $K'$は別々に閉じられるので、$Z_i= K'$になります。 命題により、VIII、p. 231、体 $D_i$ の 3 は可換です。従って、$D_i= K'$ となります。 K-代数 $\mathbf{M}_{n_1}(K)\times  \cdots  \times \mathbf{M}_{n_r}(K)$ を B で表します。$K'$-代数 $A_{(K')}$ と $B_{(K')}$ は上記と同型です。 K 上で有限生成される $K'$ のすべての部分拡張は分離可能であり、K 上で有限次数を持ちます。従って、ガロアである $K'$ と K 上の有限次数の部分拡張 L に含まれます (V, §10, No. 1, p. 57, 命題 2)。従って、その意味は補題 4 から続きます。

含意 (vi)$\Rightarrow$(v) は明らかです。

#### 系 1 {#alg-viii-s13-lem-4-cor-1 .statement tag=00FK}

Kを可換体、$A_1$と$A_2$をK-代数とします。 $A_1$ が絶対半単純であるとします。

a) $A_2$ が半単純であれば、$A_1\otimes_KA_2$ も同様です。

b) $A_2$ が絶対半単純であれば、$A_1\otimes_KA_2$ も同様です。

$A_1$の中心を$Z_1$で表し、$A_2$のそれを$Z_2$で表します。 $A_1\otimes_KA_2$の中心Zは、III, §4, No. 4、p. 468の系により$Z_1\otimes_KZ_2$に等しくなります。 $A_2$ が半単純であると仮定します。その場合、$Z_2$ は縮小された代数 (VIII、p. 137、命題 2 および 3) です。 定理 1 により、$Z_1$ はエタールとなり、K-代数と分離可能になります。 命題までに、V, §15, No. 2、p. 120、環 $Z = Z_1\otimes_KZ_2$ のうちの 5 が減ります。 $A_1$ は K (定理 1) よりも有限次数なので、VIII、p. 221 の命題 7 から、環 $A_1\otimes_KA_2$ は半単純になります。

ここで、$A_2$ が絶対半単純であると仮定します。 L を K の拡大とします。すると、代数 $A_{1(L)}$ は絶対半単純、代数 $A_{2(L)}$ は半単純となります。したがって、a) により、代数 $A_1\otimes_KA_{2(L)}$ は半単純となります。

#### 系 2 {#alg-viii-s13-lem-4-cor-2 .statement tag=00FL}

K を分離閉体、A を絶対半単純 K-代数とします。次に、代数 A が代数 $\prod_{i=1}^r\mathbf{M}_{n_i}(K)$ と同型となるような整数 $r\geqslant 0$ と厳密には正の整数 $n_1, . . . , n_r$ が存在します。

定理 1 により、A は、整数 $r\geqslant 0$、整数 $n_1, . . . , n_r$、および有限次数 $D_1, . . . ,D_r$ の K-代数について、形 $\prod^r_{i=1}\mathbf{M}_{n_i}(D_i)$ の代数と同型です。 体、その中心は K の分離拡大であるため、K に等しくなります。 VIII、p. 231 の命題 3 により、$i\in [1, r]$ に対して $D_i= K$ が得られます。

#### 例 {#alg-viii-s13-n3-exa-1 .statement tag=00FM}

可換K-代数は、エタールである場合に限り、絶対半単純です。これは、定理 1 のプロパティ (i) および (v) の定義 (V, §6, No. 3、p. 28、定義 1) および同値から続きます。

### 4. 絶対半単純加群中特徴付け

#### 命題 4 {#alg-viii-s13-prop-4 .statement tag=00FN}

Kを可換体、AをK-代数とします。

a) M を半単純A-加群とします。 A-加群 M は、M のサポートに対するすべての単純加群所属が存在する場合に限り、絶対半単純になります。

b) S を単純A-加群とし、D をその交換子環とします。次のプロパティは同等です。

(i) A-加群 S は絶対半単純です。

(ii) K-代数 D は絶対半単純です。

(iii) K-代数 D は体で、K 上に有限次数があり、その

中心は K の分離拡大です。

主張 a) は、VIII、p. 229 の命題 1、a) から続きます。 S と D を b) のようにし、L を K の拡大とします。 $A_{(L)}$ モジュール $S_{(L)}$ は、環 $D_{(L)}$ が (VIII、p. 222、命題 8、c)) である場合に限り、半単純になります。 これにより、(i)と(ii)の同値が証明され、Dが体であるため、定理1から(ii)と(iii)の⟧が証明されます。

#### 系 {#alg-viii-s13-n4-cor-1 .statement tag=00RF}

K を可換体、$A_1$ と $A_2$ を K-代数、$M_1$ を絶対半単純 $A_1$ モジュールと $M_2$ 半単純 $A_2$ モジュールとします。すると、$M_1\otimes_KM_2$ は環 $A_1\otimes_KA_2$ を超えて半単純加群になります。

加群 $M_1$ は、絶対半単純の単純な $A_1$ モジュール (命題 4) の直和です。したがって、加群 $M_1$ および $M_2$ が単純な場合、主張を証明すれば十分です。 交換子環を $D_1$ と $D_2$ で表します。 K-代数 $D_1$ は絶対半単純 (前述)。 by 系 VIII、p. 234、K-代数 $D_1\otimes_KD_2$ の 1 は半単純です。次に、VIII、p. 215 の系 1 から、$(A_1\otimes_KA_2$) モジュール $M_1\otimes_KM_2$ は半単純であることがわかります。

### 5. 半単純代数の導分

この小節と次のものでは、K は可換環、A K-代数、B K-代数 $A\otimes_KA^o$、および A の $x, y$ に対して $\varepsilon (x\otimes y) =xy$ によって定義される B から A への $\varepsilon$ K-線型写像です。

(III, §4, No. 3, p. 467) を思い出してください。すべての $(A$, A) バイモジュール P は、A の $a, a'$ と P の $p$ に対して $(a\otimes a')p=apa'$ によって与えられる外部法則とともに、左B-加群として見ることができます。逆に、すべての B-加群は、 $(A,A)$-バイモジュール。 A に標準的な $(A$、A) バイモジュール構造と対応する B-加群構造を与えます。 B に $(A$、A) バイモジュール構造対応するから B-加群 $B_s$ を与えます。したがって、私たちは

$$
a(x\otimes y)a'= (a\otimes a')(x\otimes y) =ax\otimes ya'
$$

A の $a, a', x, y$ について、積 $ya'$ は代数 A で計算されます。

K-線型写像 $\varepsilon$ は、$(A$、A) バイモジュールの準同型です。

#### 命題 5 {#alg-viii-s13-prop-5 .statement tag=00FO}

次のプロパティは同等です。

(i) B-加群 A は射影です。

(ii) $(A,A)$ バイモジュール B 満たすの元 $e$ には、$a\in A$ ごとに $\varepsilon (e) = 1$ と $ae=ea$ の 2 つの条件が存在します。

写像 $\varepsilon : B\rightarrow A$ は、$a\in A$ ごとに $\varepsilon (a\otimes 1) =a$ があるため、全射です。それは $(A$、A) モジュールの準同型であるため、B-線型写像です。 B-加群 A が射影である場合、$\varepsilon$ の切断 $s$ (II, §2, No. 2, p. 231, 命題 4) が存在します。それは $(A$ の準同型、A) から B までのバイモジュールです。集合 $e=s$(1) とすると、$a\in A$ ごとに $\varepsilon (e) =\varepsilon (s(1)) = 1$ と $ae=s(a) =ea$ が得られます。従って、(i) は (ii) を意味します。

逆に、$e$を(ii)のB満たす条件の元とします。 定義する写像 $s$ A から B まで公式

$$
s(a) =ae=ea \tag{1}
$$

それは $(A$、A) モジュールの準同型で、$\varepsilon \circ s= 1_A$ があります。他の語では、$s$ は全射写像 $\varepsilon$ の B 線形切断です。従って、B-加群 A は $B_s$ (II, §1, No. 9, p. 211, 命題 15) の直和因子部分加群 $s(A)$ と同型であり、したがって射影 (II, §2, No. 2, p. 231, 命題 4) です。これは、(ii) が (i) を意味することを証明します。

#### 注意 1 {#alg-viii-s13-n5-rem-1 .statement tag=00FP}

$e=\sum^r_{i=1}a_i\otimes a'_i$をBの元とします。命題5の項目(ii)の条件を公式に変換します。

$$
\sum_{i=1}^ra_ia'_i= 1 \tag{2}
$$

(3) $a\in A$ごとに$\sum_{i=1}^raa_i\otimes a'_i=\sum_{i=1}^ra_i\otimes a'_ia$。

それらが満足されると、$e$ は B の冪等です。実際、そのとき、関係が得られます。

$$
e^2=\sum_{i=1}^ra_iea'_i=\sum_{i=1}^rea_ia'_i=e
$$

#### 注意 2 {#alg-viii-s13-n5-rem-2 .statement tag=00FQ}

K を可換体、A を K-代数、M を A-加群とします。 群 End$_K(M)$ には、$(A$、A) バイモジュール構造が備わっており、次のように定義されます。

$$
aua'(x) =au(a'x)
$$

すべての $a, a'\in A$、すべての $u\in$ End$_K$(M)、およびすべての $x\in M$ に対して。付随した B-加群構造を付与します。 命題 5 の部分 (ii) における B 満たす条件の元を $e=\sum^r_{i=1}a_i\otimes a'_i$ とします。従って、関係 (2) と (3) も同様です。 $p\in$ End$_K(M)$ が射影子で、像 N が M の A-部分加群である場合、$ep$ は同じ像を持つ A 線形射影子です。

実際、$ep$ の像は N に含まれます。$x$ 属するが N に含まれる場合、$a'_ix$ も含まれるため、$p(a'_ix) =a'_ix$ が得られ、

$$
ep(x) =\sum_{i=1}^ra_ia'_ix=x
$$

公式作 (2)。 公式 (3) から、すべての $a\in A$ とすべての $x\in M$ に対して $aep(x) =ep(ax)$ が推定され、$ep$ が A 線形であることが証明されます。

#### 定理 2 {#alg-viii-s13-thm-2 .statement tag=00RG}

Kを可換体、AをK-代数とします。次のプロパティは同等です。

(i) K-代数 A は絶対半単純です。

(ii) K-代数 $B = A\otimes_KA^o$ は半単純です。

(iii) B-加群 A は射影です。

(iv) $(A,A)$-bimodule B 満たす $\varepsilon (e) = 1$ および $ae=ea$ の $a\in A$ ごとに元 $e$ が存在します。

代数 A が絶対半単純であるため、半単純であるとします。すると、代数 $A^o$ は半単純 (VIII, p. 137, 命題 2) となり、VIII, p. 234 の系 1 から、$B = A\otimes_KA^o$ は半単純となります。 K-代数。従って、(i) は (ii) を意味します。

半単純環上のすべての加群は射影 (VIII、p. 138、命題 4) であるため、(ii) は (iii) を意味します。

(iii) と (iv) の同値は命題 5 から続きます。 証明を完成させるために、(iv) が (i) を意味することを示しましょう。 命題 5 の項目 (ii) の B 満たす条件の元を $e=\sum^r_{i=1}a_i\otimes a'_i$ とします。 L を体 K の拡大とします。 証明しなければならない環 $A_{(L)}$ は半単純である、または同等に、すべての $A_{(L)}$ モジュールは半単純 (VIII、p. 138、命題 4) であると考えられます。 M を $A_{(L)}$ モジュール、N を M の部分加群とします。 M を左の $(A$, L) バイモジュールと見なし、N を部分両側加群 (III, §4, No. 3, p. 466) と見なします。 L は体であるため、M には像 N との L 線形射影子 $u$ が存在します。 A の元 $a$ に関連付けられた相似関係 $a_M$ はL-線形では、元 $a\otimes a'$ を L-線形マッピング $x\mapsto au(a'x)$ に送信する $A\otimes_KA^o$ から End$_L(M)$ までの一意な群準同型が存在します。 $e$の像をこの準同型を$v$で表します。 注意 2 から、$v$ は像 N を持つ $A_{(L)}$ 線形射影子であることがわかります。 $v$ の核は、N を補足する M の $A_{(L)}$ サブモジュールです。 系 2 よりVIII、p. 56の$A_{(L)}$モジュールMは半単純です。

#### 注意 3 {#alg-viii-s13-n5-rem-3 .statement tag=00FR}

私たちは (VIII, p. 234, 系 1) 可換体上の 2 つの絶対半単純多元環のテンソル積が絶対半単純であることを知っています。従って、代数 A が絶対半単純である場合、代数 $B = A\otimes_KA^o$ も同様です。

### 6. コホモロジー/代数

この小節では、K は可換環、A K-代数、B K-代数 $A\otimes_KA^o$、および $\varepsilon$ K-線型写像で、A の $x, y$ に対して $\varepsilon (x\otimes y) =$ $xy$ によって定義される B から A までです。 $n\in \mathbf{N}$、K-加群 A の $n+ 2$ コピーの K 上のテンソル積を $B_n$ で表します。私たちはそれを$(A$, A)-bimodule (そしてB-加群) とみなします。 テンソル積の最初の因子の左A-加群構造から推定された左A-加群の構造と、右A-加群から推定された右A-加群の構造が与えられます。前回の因子の構造。特に、$B_0$ は単なる $(A$、A)-bimodule B です。

整数 $n\geqslant 1$ ごとに、両側加群 $d_n^i$ の定義する準同型を、$i\in [0, n]$ と $d_n$ から公式までに$B_n$ から $B_{n-1}$ にします。

$$
d_n^i(x_0\otimes  \cdots  \otimes x_{n+1}) =x_0\otimes  \cdots  \otimes x_ix_{i+1}\otimes  \cdots  \otimes x_{n+1} \tag{4}
$$

$i\in [0, n]$ と

$$
d_n=\sum_{i=0}^n(-1)^id_n^i \tag{5}
$$

写像 $\varepsilon : B_0\rightarrow A$ を $d_0=d^0_0$ で表します。

$n$ を整数 $\geqslant 1$ とします。 $0\leqslant i < j\leqslant n$ については、

$$
d_{n-1}^i\circ d_n^j=d_{n-1}^{j-1}\circ d_n^i \tag{6}
$$

そしてこれから推測します

$$
d_{n-1}\circ d_n=\sum_{0\leqslant i<j\leqslant n}(-1)^{i+j}d_{n-1}^i\circ d_n^j+\sum_{0\leqslant j\leqslant i\leqslant n-1}(-1)^{i+j}d_{n-1}^i\circ d_n^j
$$

$$
=\sum_{0\leqslant i<j\leqslant n}(-1)^{i+j}d_{n-1}^{j-1}\circ d_n^i+\sum_{0\leqslant j\leqslant i\leqslant n-1}(-1)^{i+j}d_{n-1}^i\circ d_n^j
$$

そしてその結果として

$$
d_{n-1}\circ d_n= 0 \tag{7}
$$

P を $(A$, A)-bimodule とします。任意の整数 $n\geqslant 0$ について、$A^n$ から P までの K 多重線形写像の K-加群を $C^n(A,P)$ で表します。 写像 $\alpha^n: C^n(A,P)\rightarrow$ Hom$_B(B_n,P)$ は $f\in C^n(A,P)$ を準同型 $\alpha^n(f)$ に送信します。

$$
\alpha^n(f) (x_0\otimes  \cdots  \otimes x_{n+1}) =x_0f(x_1, . . . , x_n)x_{n+1} \tag{8}
$$

K-加群の同型です。

$C^n(A, P)$ から $C^{n+1}(A, P)$ までを $\partial^n$ ($n \geq 0$ の場合) 一意なK-線型写像で表すと、次の図式が可換になります。

$$
\begin{array}{ccc}
C^n(A, P) & \xrightarrow{\partial^n} & C^{n+1}(A, P) \\
| \downarrow \alpha^n | & & | \downarrow \alpha^{n+1} | \\
\operatorname{Hom}_B(B_n, P) & \xrightarrow{\operatorname{Hom}(d_{n+1}, 1_P)} & \operatorname{Hom}_B(B_{n+1}, P).
\end{array}
$$

したがって、定義までに、

$$
(9) \quad (\alpha^{n+1} \circ \partial^n)(f) = \alpha^n(f) \circ d_{n+1}
$$

$f \in C^n(A, P)$ごとに。他の語では、

$$
\partial^n(f)(x_0, \ldots, x_n) = \alpha^n(f)(d_{n+1}(1 \otimes x_0 \otimes \cdots \otimes x_n \otimes 1))
$$

Aの$x_0, \ldots, x_n$と$C^n(A, P)$の$f$、つまり、

$$
\begin{align*}
(10) \quad \partial^n(f)(x_0, \ldots, x_n) &= x_0 f(x_1, \ldots, x_n) \\
&+ \sum_{i=0}^{n-1} (-1)^{i+1} f(x_0, \ldots, x_{i-1}, x_i x_{i+1}, x_{i+2}, \ldots, x_n) \\
&\phantom{=} + (-1)^{n+1} f(x_0, \ldots, x_{n-1}) x_n.
\end{align*}
$$

(7) と (9) により、次のようになります。

$$
(11) \quad \partial^{n+1} \circ \partial^n = 0 \qquad \text{for every } n \geq 0.
$$

K-加群 $\operatorname{Ker} \partial^0$ を $H^0(A, P)$ で表し、$n \geq 1$ の場合、K-加群 $\operatorname{Ker} \partial^n / \operatorname{Im} \partial^{n-1}$ を $H^n(A, P)$ で表します。 P と私たちは同一視する K-加群 $C^0(A, P)$ で、$C^1(A, P) = \operatorname{Hom}_K(A, P)$ がいます。 $n \leq 2$ に対する写像 $\partial^n$ は公式によって与えられます

$$
\begin{align*}
(12) \quad \partial^0(p)(a) &= ap - pa \qquad \text{for every } p \in P, \\
(13) \quad \partial^1(f)(a, a') &= af(a') - f(aa') + f(a)a' \qquad \text{for } f \in C^1(A, P), \\
(14) \quad \partial^2(f)(a, a', a'') &= af(a', a'') - f(aa', a'') + f(a, a'a'') - f(a, a')a''
\end{align*}
$$

$f \in C^2(A, P)$の場合。

したがって、$H^0(A, P)$ は、元 $p$ の P からなるの K サブモジュールであり、$a \in A$ ごとに $ap = pa$ となり、$H^1(A, P)$ は、A からの K 導出の K-加群 $\operatorname{Der}_K(A, P)$ の商になります。 K サブモジュールからなるの導分形 $a \mapsto ap - pa$ と $p \in P$ (*内部導分* と呼ばれる) による P (III, §10, No. 2、p. 553) へ。

### 7. コホモロジー/絶対半単純多元環

#### 命題 6 {#alg-viii-s13-prop-6 .statement tag=00FS}

Kを可換環、AをK-代数とします。 VIII、p. 236の命題の項目(ii)の$B = A\otimes_KA^o$満たす条件の元を$e=\sum^r_{i=1}a_i\otimes a'_i$とします。 整数 $n\geqslant 1$ および $C^n(A,P)$ の任意の元 $f$ については、公式によって定義される $C^{n-1}(A,P)$ の $\gamma^n(f)$ 元で表します。

$$
\gamma^n(f)(x_1, . . . , x_{n-1}) =\sum_{i=1}^ra_if(a'_i, x_1. . . , x_{n-1}) \tag{15}
$$

次に、

$$
\partial^{n-1}(\gamma^n(f)) +\gamma^{n+1}(\partial^n(f)) =f \tag{16}
$$

整数 $n\geqslant 1$ ごと、および $f\in C^n(A,P)$ ごとに。

#### 注意 1 {#alg-viii-s13-n7-rem-1 .statement tag=00SF}

$*$射 $\partial^n: C^n(A,P)\rightarrow C^{n+1}(A,P)$ 定義する K-加群 (X, §2、n$^o1$、p. 24) の複合体 $(C(A,P), \partial )$。 写像 $\gamma_n$ 従って、定義する 0 を Id$_{C(A,P)}$ にリンクするこの複素数からそれ自体へのホモトピー (X, §2, n$^o4$, p. 32、定義 $4$)$.*$

No.6の記法を保持します。 整数 $n\geqslant 0$ ごとに、公式までに定義する写像 $h_n: B_n\rightarrow B_{n+1}$ になります

$$
h_n(x) =d^1_{n+2}(e\otimes x) =\sum_{i=1}^ra_i\otimes a'_ix
$$

$(A$の準同型、A)-bimodules (公式 (3)) です。

#### 補題 5 {#alg-viii-s13-lem-5 .statement tag=00FT}

関係があります

$$
d_{n+1}\circ h_n+h_{n-1}\circ d_n= 1_{B_n} \tag{17}
$$

$n\geqslant 1$ごとに。

$x\in B_n$ にしましょう。我々は持っています

$$
(d_{n+1}\circ h_n)(x) = (d_{n+1}\circ d^1_{n+2})(e\otimes x)
$$

$$
= (d^0_{n+1}\circ d^1_{n+2})(e\otimes x)-\sum^{n+2}_{i=2}(-1)^i(d_{n+1}^{i-1}\circ d^1_{n+2})(e\otimes x)
$$

従って、公式 (6) までに、

$$
(d_{n+1}\circ h_n)(x) = (d^0_{n+1}\circ d^0_{n+2})(e\otimes x)-\sum^{n+2}_{i=2}(-1)^i(d^1_{n+1}\circ d_{n+2}^i)(e\otimes x)
$$

しかし、私たちは持っています

$$
(d^0_{n+1}\circ d^0_{n+2})(e\otimes x) =\varepsilon (e)x=x
$$

性質 (ii) の命題 5 の VIII、p. 236、および $i\geqslant 2$ の場合、

$$
d^i_{n+2}(e\otimes x) =e\otimes d^{i-2}_n(x)
$$

それは与える

$$
(d_{n+1}\circ h_n)(x) =x-d^1_{n+1}(e\otimes d_n(x)) =x-h_{n-1}\circ d_n(x)
$$

従って、公式 (17)。

補題 5 を使用して、命題 6 の証明を完了できます。$n$ を $C^n(A,P)$ の整数 $\geqslant 1$ と $f$ 元とします。 構成までに、

$$
\alpha^{n-1}(\gamma^n(f)) =\alpha^n(f)\circ h_{n-1} \tag{18}
$$

その結果、公式 (9) と (18) により、

$$
\alpha^n(\partial^{n-1}(\gamma^n(f)) +\gamma^{n+1}(\partial^n(f))) =\alpha^{n-1}(\gamma^n(f))\circ d_n+\alpha^{n+1}(\partial^n(f))\circ h_n
$$

$$
=\alpha^n(f)\circ h_{n-1}\circ d_n+\alpha^n(f)\circ d_{n+1}\circ h_n
$$

$$
=\alpha^n(f)
$$

ここで、最後の等式は (17) から続きます。 $\alpha^n$ は全単射なので、命題が続きます。

#### 定理 3 {#alg-viii-s13-thm-3 .statement tag=00FU}

K を可換環、A K-代数、P を $(A,A)$ バイモジュールとします。 $(A\otimes_KA^o)$-モジュール A が射影であると仮定します。次に、整数 $n\geqslant 1$ ごとに $H^n(A,P) = 0$ が得られます。

証明しなければならない、整数 $n\geqslant 1$、$C^n(A,P)$ と $\partial^n(f) = 0$ のすべての元 $f$ は、$C^{n-1}(A,P)$ の元 $g$ に対して形 $\partial^{n-1}(g)$ であると考えます。 命題 5 までに、これは命題 6 の明らか帰結になります。

#### 系 {#alg-viii-s13-n7-cor-1 .statement tag=00FV}

A から P までのすべての K 導出は内部です。

等式 $H^1(A,P) = 0$ の翻訳です。

#### 注意 2 {#alg-viii-s13-n7-rem-2 .statement tag=00FW}

定理 3 の仮定は、特に、K が体および A 絶対半単純 K-代数 (VIII, p. 238, 定理 2) のときに満たされます。

#### 注意 3 {#alg-viii-s13-n7-rem-3 .statement tag=00FX}

K-加群 A が射影であると仮定します。 定理 3 は次のように証明することもできます。複素数 $(\bigoplus_{n\geqslant 0}B_n, d)$ および準同型 $\varepsilon : B_0\rightarrow A$ 定義するの射影解像度は B-加群 A です。従って、すべての $n\geqslant 0$、K-加群 $H^n(A,P)$ は Ext$^n_B(A,P)$ (X, §6、n$^o1$、p. 100、定理 1) と同型です。 B-加群 A が射影である場合、K-加群 Ext$^n_B(A,P)$ は、$n\geqslant 1$ (X, §5, n$^o3$, p. 88, 系 de la 命題 5) の零になります。これは、次のことを意味します。 $H^n(A,P)$は零です。逆に、すべての $(A$, A)-bimodule P に対して $H^1(A,P)$ が零である場合、B-加群 A は射影 (X, §5, n$^o5$, p. 93, 命題 $10$)$.*$

### 8. 分裂/アルティン代数

この小節では、Kは可換環、AはK-代数です。 $\mathfrak{r}$ を A の根基とします。 商代数 $A/\mathfrak{r}$ を $\overline{A}$ で表し、A から $\overline{A}$ までの標準写像を $\pi$ で表します。 $A = S\oplus \mathfrak{r}$ のような A の部分代数 S に興味があります。

A の $\alpha , \beta$ に対して、K 線形の切断 $s$ $\pi$ 満たす $s(\alpha \beta ) =$ $s(\alpha )s(\beta )$ を Σ 集合で表します。このような切断は必ず $s(1) = 1$ を満たすことに注意してください（他の式では語、$s$ は環準同型): 確かに $s(1)^2=s$(1) があり、$s(1)$ は属するから $1 +\mathfrak{r}$ (VIII、p. 156、定理) であるため可逆です。 1)。 $s$ が Σ の元である場合、$s$ の像 S は A の部分代数であり、$A = S\oplus \mathfrak{r}$ が得られます。逆に、S が $A = S\oplus \mathfrak{r}$ となるような A の部分代数である場合、S に対する $\pi$ の制限は全単射であり、像 S に対する Σ の逆全単射定義する元です。

ジェイコブソンの定理 (前述) によれば、$1 +\mathfrak{r}$ のすべての元は A で反転可能です。形 $a\mapsto xax^{-1}$ と $x\in 1 +\mathfrak{r}$ の A の内部自己同型を特別な自己同型と呼びます。

#### 命題 7 {#alg-viii-s13-prop-7 .statement tag=00FY}

$(A\otimes_K\overline{A}^o)$ モジュール $\overline{A}$ が射影であると仮定します。

a) $S_1$ と $S_2$ を満たす $A = S_1\oplus \mathfrak{r}= S_2\oplus \mathfrak{r}$ の部分代数とします。 $S_1$ を $S_2$ に変換する A の特別な自己同型が存在します。

b) $\pi$ が K 線形切断を持ち、A の根基 $\mathfrak{r}$ が nilpotent であると仮定します。すると、満たす $A = S\oplus \mathfrak{r}$ の部分代数 S が存在します。

$S_1$ と $S_2$ を a) のようにします。 $s_1$と$s_2$を集合Σ対応するから部分代数$S_1$と$S_2$の元とします。 $\varepsilon$ を $A\otimes_KA$ から $\varepsilon (a\otimes b) =ab$ で与えられる A までの K-線型写像とします。 VIIIの命題 5、p. 236、およびVIII、p. 237の注意 1までに、$\overline{A}\otimes_KA$ 満たす $\sum^r_{i=1}\alpha_i\alpha '_i= 1$の元 $e=\sum^r_{i=1}\alpha_i\otimes \alpha '_i$が存在し、 $\alpha \in A$ごとに$\sum^r_{i=1}\alpha \alpha_i\otimes \alpha '_i=\sum^r_{i=1}\alpha_i\otimes \alpha '_i\alpha$。 集合 $x=\sum^r_{i=1}s_1(\alpha_i)s_2(\alpha '_i)$。 $\pi (x) =\sum^r_{i=1}\alpha_i\alpha '_i= 1$ があるため、$x\in 1 +\mathfrak{r}$ になります。 $\alpha$ を A の元とします。

$$
s_1(\alpha )x=\sum_{i=1}^rs_1(\alpha \alpha_i)s_2(\alpha '_i) = (\varepsilon \circ (s_1\otimes s_2))(\sum_{i=1}^r\alpha \alpha_i\otimes \alpha '_i)
$$

$$
= (\varepsilon \circ (s_1\otimes s_2))(\sum_{i=1}^r\alpha_i\otimes \alpha '_i\alpha )=\sum_{i=1}^rs_1(\alpha_i)s_2(\alpha '_i\alpha ) =xs_2(\alpha )
$$

等式 $x^{-1}S_1x= S_2$ が続き、主張 a) が得られます。

b)の仮定の下で、さらに$\mathfrak{r}^2= 0$と仮定します。この場合、$(A$, A)-bimodule $\mathfrak{r}$ は $\mathfrak{r}$ によって消滅するため、それを $(A$, A)-bimodule と見なします。 選ぶ $\pi$ の K 線形切断 $\sigma$。我々は持っています

(19) $\alpha x=\sigma (\alpha )x$ と $x\alpha =x\sigma (\alpha )$

$\alpha \in \overline{A}$ と $x\in \mathfrak{r}$ の場合。 集合

$$
\varphi (\alpha , \beta ) =\sigma (\alpha \beta )-\sigma (\alpha )\sigma (\beta ) \tag{20}
$$

$\alpha , \beta \in A$の場合。 $\alpha , \beta \in A$には関係$\pi (\varphi (\alpha , \beta )) =\alpha \beta -\alpha \beta = 0$がございます。したがって、$C^2(A,\mathfrak{r})$ の $\varphi$ 定義する元となります。 $\alpha , \beta , \gamma$ を A の元とします。 (19) を考慮すると、

$$
\partial^2\varphi (\alpha , \beta , \gamma ) =\alpha \varphi (\beta , \gamma )-\varphi (\alpha \beta , \gamma ) +\varphi (\alpha , \beta \gamma )-\varphi (\alpha , \beta )\gamma
$$

$$
=\sigma (\alpha )\varphi (\beta , \gamma )-\varphi (\alpha \beta , \gamma ) +\varphi (\alpha , \beta \gamma )-\varphi (\alpha , \beta )\sigma (\gamma )
$$

$$
=\sigma (\alpha )(\sigma (\beta \gamma )-\sigma (\beta )\sigma (\gamma ))-\sigma (\alpha \beta \gamma ) +\sigma (\alpha \beta )\sigma (\gamma ) +\sigma (\alpha \beta \gamma )
$$

$$
-\sigma (\alpha )\sigma (\beta \gamma )-(\sigma (\alpha \beta )-\sigma (\alpha )\sigma (\beta ))\sigma (\gamma )
$$

$$
= 0
$$

定理により、VIII、p. 242、K-加群 $H^2(A,\mathfrak{r})$ の 3 が零に減ります。 Hence there exists an element $\psi$ of $C^1(A,\mathfrak{r})$ such that $\partial^1\psi =\varphi$, in other words, such that we have

(21) $\overline{A}$ の $\alpha , \beta$ に対して $\varphi (\alpha , \beta ) =\alpha \psi (\beta )-\psi (\alpha \beta ) +\psi (\alpha )\beta$。

$\mathfrak{r}^2$ は零であるため、$\psi (\alpha )\psi (\beta ) = 0$ になります。 (19) と (20) から、(22) $(\sigma +\psi )(\alpha \beta ) = (\sigma +\psi )(\alpha )(\sigma +\psi )(\beta )$ を推定します。

$\pi$ 属するの K 線形切断 $\sigma +\psi$ が Σ になるようにします。その像は、$A = S +\mathfrak{r}$ となる A の部分代数 S です。

ここで、一般的な場合における S の存在を証明しましょう。 We reason by induction on the least integer $p\geqslant 1$ such that $\mathfrak{r}^p= 0$; the case $p= 1$ is trivial. $p\geqslant 2$ と集合 $A'= A/\mathfrak{r}^{p-1}$ を仮定します。 The radical $\mathfrak{r}'$ of $A'$ is equal to $\mathfrak{r}/\mathfrak{r}^{p-1}$ (Proposition 5 of VIII, p. 155), so satisfies ${\mathfrak{r}'}^{p-1}= 0$, and the algebra $A'/\mathfrak{r}'$ is isomorphic to $\overline{A}= A/\mathfrak{r}$ and is therefore absolutely semisimple. 帰納法の仮定までに、$A'= S'\oplus \mathfrak{r}'$となるような$A'$の部分代数$S'$が存在します。 この場合、$S'$ は形 $A''/\mathfrak{r}^{p-1}$ であり、$A''$ は含む $\mathfrak{r}^{p-1}$ の部分代数であり、次のようになります。

$$
A = A''+\mathfrak{r},\mathfrak{r}^{p-1}= A''\cap \mathfrak{r} \tag{23}
$$

代数 $A''/\mathfrak{r}^{p-1}$ は $A'/\mathfrak{r}'$ と同型です。 $(\mathfrak{r}^{p-1})^2= 0$ があるので、$\mathfrak{r}^{p-1}$ は $A''$ の根基です。先ほど扱ったケースでは、$A''= S\oplus \mathfrak{r}^{p-1}$ となる $A''$ の部分代数 S が存在します。 (23) から関係 $A = S\oplus \mathfrak{r}$ を導き出します。

#### 系 1 (ウェダーバーンの定理) {#alg-viii-s13-prop-7-cor-1 .statement tag=00S8}

K を可換体、A K-代数、A の $\mathfrak{r}$ 根基とします。K-代数 $A/\mathfrak{r}$ が絶対半単純であるとします。

a) $S_1$ と $S_2$ を満たす $A = S_1\oplus \mathfrak{r}= S_2\oplus \mathfrak{r}$ の部分代数とします。 $S_1$ を $S_2$ に変換する A の特別な自己同型が存在します。

b) $\mathfrak{r}$ が零能である場合、満たす A = $S\oplus \mathfrak{r}$ の部分代数 S が存在します。

これは、VIII、p. 238 の命題 7 と定理 2 に続きます。

#### 系 2 {#alg-viii-s13-prop-7-cor-2 .statement tag=00FZ}

A を完全体 K 上の有限次数の可換代数とし、$\mathfrak{r}$ をその根基とします。 $A = S\oplus \mathfrak{r}$ となるような A の固有の部分代数 S が存在します。さらに、S は、有限次数の K の有限多拡大の積と同型です。

K-代数 $A/\mathfrak{r}$ は半単純 (VIII、p. 173、命題 1) で、有限次数があります。 体 K は完全なので、絶対半単純です (VIII、p. 232、定理 1)。イデアル $\mathfrak{r}$ は零能であり、A は可換であるため、S の存在と一意性は系 1 から続きます。 S は半単純で可換であり、有限次数があるため、最後の主張は命題 3 の帰結です。 VIII、p. 137。

#### 注意 1 {#alg-viii-s13-n8-rem-1 .statement tag=00G0}

$A/\mathfrak{r}$ が絶対半単純であるという仮定は、系 1 (VIII、p. 246、練習問題 4) では必須です。

#### 注意 2 {#alg-viii-s13-n8-rem-2 .statement tag=00G1}

A が体 K 上でアルティン代数であるとします。A が可換である場合、A が代数 $A_1\times  \cdots  \times A_n$ の積と同型であることを (VIII, p. 180, 練習問題 9) 示すことができます。つまり、$A_i/\mathfrak{R}(A_i)$ は $i$ ごとに体になります。逆に、A が可換でない場合、A は、$A_i/\mathfrak{R}(A_i)$ がすべての $i$ (VIII、p. 247、練習問題) に対して単純な環となるように、代数 $A_1\times  \cdots  \times A_n$ の積と同型ではない可能性があります。 5)。

### 練習問題 {#alg-viii-s13-exercises}

[§ 13 に対して練習問題](exercises/s13/)を参照してください。
