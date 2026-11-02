---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 8
section_title: Semisimple Rings
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.135-A VIII.150
pdf_pages: 0152-0167
extraction: native
subsections:
    - "no": 1
      title: Semisimple Rings
      page: 135
      pdf_page: 152
    - "no": 2
      title: Modules over a Semisimple Ring
      page: 138
      pdf_page: 155
    - "no": 3
      title: Factors of a Semisimple Ring
      page: 141
      pdf_page: 158
    - "no": 4
      title: Idempotents and Semisimple Rings
      page: 145
      pdf_page: 162
statements: 30
exercises: 6
content_sha256: 45796d6e1ae60b3ae5d9a62199338534c6b0ebbb08f97640f50a8f553958321e
translated_from: content/en/alg/VIII/08_s8_semisimple_rings.md
translation_method: google
source_content_sha256: c3520cd3a5b6efacdd841870c3c2e342b0341edbd32074687bd212bc32731ee7
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 1a3773dba5b2dc16078f5f9c835f52dce7883842383c3ee7081a66c08a69da49
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 8。 半単純環

### 1. 半単純環

#### 定理 1 (ウェダーバーン) {#alg-viii-s8-thm-1 .statement tag=00S4}

Aを環とします。次のプロパティは同等です。

(i) A-加群 $A_s$ は半単純です。

(ii) A の左イデアル $\mathfrak{a}$ ごとに、$A_s$ が $\mathfrak{a}$ と $\mathfrak{b}$ の直和となるような A の左イデアル $\mathfrak{b}$ が存在します。

(iii) 環 A は左アルティン的、$(A,A)$-bimodule $_sA_d$ は半単純です。

(iv) 環 A は、単純な環の有限族の積と同型です。

(v) 環 A が行列環 $\mathbf{M}_{r_i}(D_i)$ の積と同型となるような整数 $s\geqslant$ 0、体 $D_1, . . . ,D_s$、整数 $r_1\geqslant 1, . . .,r_s\geqslant 1$ が存在します。

(vi) 環 A は左アルティン的であり、忠実な者と半単純左A-加群が存在します。

(i)と(ii)の同値は、VIIIの系2、p. 56から続き、(iv)と(v)のそれは、VIII、p. 120の定理1から続きます。

A-加群 $A_s$ は有限に生成されます。 半単純の場合は、左アルティン的 (VIII、p. 71、命題 10) です。 A-加群 $A_s$ は忠実であるため、これは (i) が (vi) を意味することを証明します。逆に、性質 (vi) が成り立つと仮定します。 Mを忠実な人にしましょう半単純A-加群。 $A_s$ が $M^m$ (VIII, p. 50, 命題 5, a)) の部分加群と同型であるような整数 $m\geqslant 1$ が存在します。 M は半単純なので、$A_s$ についても同じことが当てはまります。したがって、(i) と (vi) の同値を証明しました。

(i) が (iii) を意味することを証明しましょう。 環 A が性質 (i) を持っているとします。 A が左アルティン的であることはすでに観察しました。さて、左A-加群 $A_s$ の自己準同型は、A の元による右側乗法です。 $(A$, A)-bimodule $_sA_d$ は半単純から、命題 6 から続きます。 VIII、p. 86。

(iii) が (iv) を意味することを示しましょう。 $(A$, A)-bimodule $_sA_d$ が半単純であるとします。それは有限に生成されるため、単純な $(A$ の有限ファミリー $(\mathfrak{a}_i)_{i\in I}$、A) サブバイモジュール直和 $_sA_d$ が存在します。他の語では、$\mathfrak{a}_i$はAの非零の両側イデアルであり、Aの加法群は$\mathfrak{a}_i$の直和であり、すべての$i\in I$について、$\mathfrak{a}_i$に含まれるAのすべての両側イデアルは0または0に等しい。 $\mathfrak{a}_i$。 $i\in I$ ごとに集合 $\mathfrak{b}_i=\sum_{j\not=i}\mathfrak{a}_j$。これは A の両面理想です。写像 $a\mapsto (a+\mathfrak{b}_i)_{i\in I}$ は、環 A から環 $A/\mathfrak{b}_i$ の積までの同型です。 $(A$、A) 双加群 $\mathfrak{a}_i$ および $A/\mathfrak{b}_i$ は同型であるため、$A/\mathfrak{b}_i$ のすべての両側イデアルは 0 または $A/\mathfrak{b}_i$ に等しくなります。 環 A が左アルティン的の場合、同じことが環 $A/\mathfrak{b}_i$ にも当てはまり、したがって単純です (VIII, p. 120, 定義 1)。

最後に、(iv) が (i) を意味することを証明しましょう。 A が単純な環の有限族 $(A_i)_{i\in I}$ の積であると仮定します。 A から $A_i$ までの添字 $i$ を含む $\pi_i$ 射影と、その基礎となる加法群 $A_i$ と法則を含む $M_i$ A-加群で表します。 作用 $(a, x)\mapsto \pi_i(a)x$。 環 $A_i$ は単純なので、$A_i$ モジュール $(A_i)_s$ は半単純なので、A-加群 $M_i$ は半単純になります。 A-加群 $A_s$ は積 $\prod_{i\in I}M_i$ に他ならないので、半単純になります。

#### 定義 1 {#alg-viii-s8-def-1 .statement tag=0093}

環 A が定理 1 と同等の性質 (i) から (vi) を持っている場合、半単純であると言います。 可換環 $k$ 上の代数 A は、基になる A が環である場合、半単純代数です。 半単純。

#### 命題 1 {#alg-viii-s8-prop-1 .statement tag=0094}

Aを半単純環とします。 $A_s=\oplus_{i\in I}\mathfrak{m}_i$ のような A の最小左イデアルの有限族 $(\mathfrak{m}_i)_{i\in I}$ が存在します。 $(\mathfrak{m}_i)_{i\in I}$ がそのような族である場合、すべての単純A-加群は $\mathfrak{m}_i$ の 1 つと同型になります。 単純A-加群の類の集合は有限です。

最初の主張は、A-加群 $A_s$ が半単純であり、有限に生成されるという事実から導き出されます。すべての単純加群は、$A_s$ の商 (VIII、p. 46、命題 1) と同型です。 2 番目の主張は、VIII の系 3、p. 56 に続き、3 番目の主張は 2 番目の明らか帰結です。

#### 例 {#alg-viii-s8-n1-exa-1 .statement tag=0095}

G を有限群、K を可換体とします。 $*$さらに (VIII, p. 401, 系 1) で、体 K に対する群 G の代数 K[G] は、K の特性指数が の位数と素数である場合に限り、半単純環であることがわかります。 $G.*$

#### 注意 1 {#alg-viii-s8-n1-rem-1 .statement tag=0096}

K を可換体とし、A を K 上の半単純代数とします。すると、K-代数 A が積 $\prod^s_{i=1}\mathbf{M}_{r_i}(D_i)$ と同型となるように、体と整数 $r_1\geqslant 1, . . . , r_s\geqslant 1$ である K-代数 $D_1, . . . ,D_s$ が存在します。

#### 注意 2 {#alg-viii-s8-n1-rem-2 .statement tag=0097}

K を代数閉体とし、A を K 上の有限次数の代数とする。 VIII、p. 122、代数の注意 4 より、A が以下と同型であるような整数 $n_1\geqslant 1, . . . , n_r\geqslant 1$ が存在する場合に限り、A は半単純となる。 代数 $\mathbf{M}_{n_1}(K)\times  \cdots  \times \mathbf{M}_{n_r}(K)$。

#### 命題 2 {#alg-viii-s8-prop-2 .statement tag=0098}

a) 半単純環の中心は半単純です。

b) 半単純環の反対環は半単純です。

c) 半単純環の商は、両面理想により半単純環になります。

d) 半単純環の有限族の積は半単純環です。

A を半単純環とします。 有限族の積 $(A_i)_{i\in I}$ の単純な環と同型です。 A の中心は $A_i$ の中心の積と同型であり、$A^o$ は $A^o_i$ の積環と同型です。 従って、主張 a) と b) は、VIII の 1、p. 121 から系に続きます。

$\mathfrak{a}$ を A の両側イデアルとします。半単純A-加群 $A_s$ のA-加群 $A_s/\mathfrak{a}$、商は、半単純です。従って、$(A/\mathfrak{a}$) モジュール $A_s/\mathfrak{a}$ は半単純です。 主張 c) が続きます。

環は、単純な環の有限族の積と同型である場合に限り、 半単純になります。 主張 d) が続きます。

#### 命題 3 {#alg-viii-s8-prop-3 .statement tag=0099}

A を可換環とします。次のプロパティは同等です。

(i) 環 A は半単純です。

(ii) 環 A はアルティンで減算されます (V, §6, No. 7、p. 34)。

(iii) 環 A は、可換体の有限族の積と同型です。

可換単純環は可換体 (VIII, p. 120, 注意 1) です。従って、(i) は (iii) と同等です。

(iii) が (ii) を意味することは明らかです。逆に、環 A がアルティンとなり減算されたとします。 A の素イデアルの集合の共通部分は、A の冪零元 (V, §15, No. 1、p. 118、命題 2) で構成され、A が約定されるため 0 に減らされます。 VIII、p. 2 までに、$\mathfrak{p}_1\cap  \cdots  \cap \mathfrak{p}_r= 0$ となるような A の異なる素イデアル $\mathfrak{p}_1, . . . ,\mathfrak{p}_r$ が存在します。 VIII、p. 8 の系までに、アルティン環 A の各素イデアル $\mathfrak{p}_i$ が最大になります。従って、$i$ と $j$ が異なる場合は常に $\mathfrak{p}_i+\mathfrak{p}_j= A$ になります。 I, §8, No. 11、p. 110、標準準同型の命題9により、Aから環$\prod^r_{i=1}(A/\mathfrak{p}_i)$は同型になります。 環 $A/\mathfrak{p}_i$ は、$i$ ごとに体となるため、(ii) は (iii) を意味します。

体の有限次数の可換代数はアルティン可換環です。従って、命題 3 は、V, §6, No. 7、p. 34 の命題 5 を一般化します。

### 2. 加群半単純環

#### 命題 4 {#alg-viii-s8-prop-4 .statement tag=009A}

A を環とします。次のプロパティは同等です。

(i) 環 A は半単純です。

(ii) すべての A-加群は半単純です。

(iii) 生成すると半単純A-加群が存在します。

(iv) 有限生成された対加群を持つ忠実な半単純A-加群が存在する。

(v) すべての A-加群は射影的です。

(vi) すべての単次 A-加群は射影的です。

$*$その他の半単純環の特徴付けについては、X, §8、n$^o4$の命題6を参照してください。 $140.*$

まず、(i) が (ii) と (v) を意味することを証明しましょう。 環 A が半単純で、左A-加群 M を考えます。仮定までに、A-加群 $A_s$ は半単純となるため、すべての自由A-加群は半単純になります。 II, §1, No. 11、p. 218の命題20までに、LからMまで自由A-加群L、全射A-線型写像$u$が存在します。Nを$u$の核とします。 A-加群 L は半単純なので、L (VIII, p. 56, 定理 1) の N を補足する半単純部分加群 $N'$ が存在します。 A-加群 $N'$ は射影であり、$N'$ から M まで $u$ 誘導する同型です。その結果、M は半単純で射影です。

(ii) $\Rightarrow$ (iii): すべての A-加群が半単純である場合、A-加群 $A_s$ は半単純です。しかも生成するです。

(iii) $\Rightarrow$ (iv): M が生成A-加群の場合、それは忠実 (定理 1 の VIII、p. 80、系) であり、その対加群は有限生成されます (VIII、p. 99、系) 1)。

(iv) $\Rightarrow$ (i): M を忠実であり、有限生成された対加群を持つ半単純A-加群とします。 VIII, p. 8 の補題 4 までに、$A_s$ が $M^m$ の部分加群と同型となるような自然数 $m$ が存在します。 A-加群 $M^m$ は半単純であるため、$A_s$ も同様です。

含意 (v) $\Rightarrow$ (vi) は明らかです。

(vi) $\Rightarrow$ (i): すべての単次 A-加群が射影であると仮定します。 $\mathfrak{a}$ を A の左イデアルとします。 A-加群 $A_s/\mathfrak{a}$ は射影であるため、$A_s$ が $\mathfrak{a}$ と $\mathfrak{b}$ の直和 (II, §2, No. 2, p. 231, 命題 4) となるような A の左イデアル $\mathfrak{b}$ が存在します。 従って、環 A は半単純 (VIII, p. 135, 定理 1) となります。

#### 補題 1 {#alg-viii-s8-lem-1 .statement tag=009B}

A を左アルティン的環、M を単純A-加群とします。そうすると、環 $A_M$ は簡単です。

環 A は左アルティン的なので、VIII, p. 7 の命題 5 により、環 $A_M$ にも同じことが当てはまります。さて、M は忠実で単純な $A_M$ モジュールであるため、環 $A_M$ は単純です (VIII、p. 119、命題 1)。

#### 命題 5 {#alg-viii-s8-prop-5 .statement tag=009C}

環 A が半単純であるとします。 M を左A-加群とします。 M の対加群は有限に生成され、$A_M= A''_M$ が得られます。

まず、M が単純A-加群の場合を考えます。 補題 1、環 $A_M$ までは簡単です。 VIII、p. 120 の補題 1 から命題 5 が続きます。

次に、一般的な場合を考えてみましょう。 単純A-加群の類の集合$\mathscr{S}$は有限です(VIII、p. 136、命題1)。 類 $\lambda$ のすべての $\lambda \in \mathscr{S}$、選ぶ A-加群 $S_{\lambda}$ について、$S_{\lambda}$ の交換子環の反対側の体を $D_{\lambda}$ で表します。 補題までに、単純な環 $A_{S_{\lambda}}, S_{\lambda}$ に 1 を適用すると、体 $D_{\lambda}$ よりも有限次元ベクトル空間になります。その次元を$m(\lambda )$で示します。 B を M の自己準同型環の反対環とします。VIII、p. 84 で、B-加群および同型として単純な $(D_{\lambda}$、B)-バイモジュール $V_{\lambda}$ が存在することを見てきました。 $(A$、B)-M から $\oplus_{\lambda\in\mathscr{S}}S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ までのバイモジュール。 B-加群として、M は $\oplus_{\lambda\in\mathscr{S}}V^{m(\lambda)}_{\lambda}$ と同型です。 $\mathscr{S}$ と $m(\lambda )$ は有限であるため、M は有限に生成される B-加群です。

A-加群 M は半単純であり、その対加群は有限生成されます。従って、VIII、p. 83 の命題 4 により $A_M= A''_M$ が得られます。

#### 命題 6 {#alg-viii-s8-prop-6 .statement tag=009D}

M を有限生成された半単純A-加群とします。そのサポート (VIII、p. 66) を $\mathscr{S}_M$ で表し、その自己準同型環を B で表します。 類 $\lambda$ のすべての $\lambda \in \mathscr{S}_M$、選ぶ単純A-加群 $S_{\lambda}$ について、 左B-加群オム$_A(S_{\lambda},M)$ by $V_{\lambda}$。

a) 環 B は半単純です。

b) 写像 $\lambda \mapsto$ cl(V$_{\lambda}$) は、M のサポート $\mathscr{S}_M$ から単純B-加群の類の集合までの全単射です。

c) すべての $\lambda \in \mathscr{S}_M$ について、A-加群 M の型 $\lambda$ の同型成分は、B-加群 M の型 $V_{\lambda}$ の同型成分に等しい。

B-加群として見ると、M は半単純 (VIII、p. 85、命題 5) であり、忠実です。 $A_M\subset$ End$_B(M)$ があるため、その対加群は有限に生成されます。従って、環 B は半単純 (命題 4) です。 $(x_1, . . . , x_r)$ が A-加群 M の生成する数列である場合、$B_s$ から $M^r$ までの写像 $b\mapsto (bx_1, . . . , bx_r)$ は B 線形で単射です。すべての単純B-加群は、$B_s$ (VIII、p. 136、命題 1) の部分加群と同型であるため、M の B-部分加群と同型です。命題は、VIII の命題 5 の直後に続きます。 p. 85。

#### 命題 7 {#alg-viii-s8-prop-7 .statement tag=009E}

A を半単純環とします。

a) すべての有限生成A-加群は再帰的です (II, §2, No. 7、p. 239)。

b) すべての単純な左A-加群 S、右A-加群 $S^*$ S への二重化は単純で、写像 $\lambda \mapsto$ cl($\lambda^*$) 定義する全単射集合の類の単純A-加群から集合/類/単純右A-加群。

c) M を有限生成された左A-加群とする。 M に対する双対の右A-加群 $M^*$ は有限に生成され、M と同じ長さを持ちます。さらに、単純A-加群 S ごとに $[M : S] = [M^*: S^*]$ があります。

M を有限生成A-加群とします。

VIII、p. 138、A-加群の命題 4 により、M は有限生成され射影的になります。従って、II, §2, No. 7、p. 240 の系 4 によって再帰的になります。特に、すべての単純A-加群は再帰的です。また、有限に生成された 2 つの左加群は、その双対が同型である場合にのみ同型であるということになります。

S を単純な左A-加群とします。 $(T_i)_{i\in I}$ を S の双対 $S^*$ である直和を持つ単純右A-加群の族とします。S は再帰的であるため、$(S^*)^*$ と同型であり、したがって $\prod_{i\in I}T^*_i$ と同型です。 加群 $T_i$ はそれぞれ再帰的です。特に、$i\in I$ ごとに $T^*_i\not= 0$ があります。 単純加群 S は $\prod_{i\in I}T^*_i$ と同型なので、集合 I は単一の元を持ち、したがって $S^*$ は単純です。

Mは半単純で有限生成なので、単純部分加群$S_1, . . . ,S_r$の直和です。次に、$M^*$ は族 $S^*_1, . . . ,S^*_r$ の直和と同型であり、加群 $S^*_i$ が単純であることがわかりました。 主張 c) がすぐに続きます。

### 3. 半単純環中因子

この小節では、半単純環 Aを考えます。

単純な左A-加群の類の集合を $\mathscr{S}$ (VIII, p. 51) で表します。それは有限です (VIII、p. 136、命題 1)。 $\lambda \in \mathscr{S}$ ごとに、選ぶ単純A-加群 $S_{\lambda}$ の類 $\lambda$ になります。その消滅子を$\mathfrak{b}_{\lambda}$で表し、その交換子環端$_A(S_{\lambda})$の反対側の体を$D_{\lambda}$で表します。

#### 命題 8 {#alg-viii-s8-prop-8 .statement tag=009F}

a) すべての $\lambda \in \mathscr{S},S_{\lambda}$ は、体 $D_{\lambda}$ 上の有限次元右ベクトル空間です。 移行から商、写像$a\mapsto a_{S_{\lambda}}$定義する環同型の場合、$A/\mathfrak{b}_{\lambda}$から終了$_{D_{\lambda}}(S_{\lambda})$まで。

b) すべての $\lambda \in \mathscr{S}$ について、環 $A/\mathfrak{b}_{\lambda}$ は単純で、A から $\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$ までの標準準同型 $\psi$ は環同型です。

環 $A/\mathfrak{b}_{\lambda}$ は $A_{S_{\lambda}}$ と同型です。 VIII、p. 139の補題 1により、この環は簡単です。 $A/\mathfrak{b}_{\lambda}$ から End$_{D_{\lambda}}(S_{\lambda})$ までの与えられた写像は、$A_{S_{\lambda}}$ から $A''_{S_{\lambda}}$ までの写像と識別できます。 VIII、p. 139の命題5までに、同型になります。

A-加群 $A_s$ は半単純で、忠実でバランスが取れています。 準同型 $\psi$ は、$A_s$ の双可換子から $\prod_{\lambda\in\mathscr{S}}$ 末$_{D_{\lambda}}(S_{\lambda})$ までの射 、つまり同型 (VIII, p. 86, 命題 7, c)) と識別できます。

単純な環 $A/\mathfrak{b}_{\lambda}$ は、型 $\lambda$ の A の単純因子と呼ばれます。

#### 例 {#alg-viii-s8-n3-exa-1 .statement tag=009G}

K を代数的に閉じた可換体とし、A を K 上の有限次数の半単純代数とする。$(V_i)_{i\in I}$ を、すべての単純A-加群が一意の $V_i$ と同型となるような単純A-加群の族とする。この場合、I は有限集合 (VIII, p. 136, 命題 1)、ベクトル空間 $V_i$ は体 K 上の有限次元であり、$V_i$ の交換子環は以下に等しい$K\cdot 1_{V_i}$ (VIII、p. 47、定理 1)、写像 $a\mapsto (a_{V_i})_{i\in I}$ は、A から $\prod_{i\in I}$ エンド$_K(V_i)$ (命題 8) までの代数同型です。

We have defined (VIII, p. 50) a minimal two-sided ideal as a minimal element of the set of nonzero two-sided ideals, ordered by inclusion. 他の語では、A の最小の両側イデアル $\mathfrak{a}$ は、$_sA_d$ の単純な $(A$、A) サブバイモジュールです。 同様に、A の最大の両側イデアルを、A の適切な両側イデアルの集合の極大元として定義するとします。 A の最大の両側イデアル $\mathfrak{a}$ は、単に $_sA_d$ (VIII, p. 48, 定義 2) の最大の $(A$, A) サブバイモジュールです。 環 A が単純な場合、イデアル 0 は A の最大の両側イデアルであり、A は最小の両側イデアルです。

任意の $\lambda \in \mathscr{S}$ について、型 $\lambda$ の A-加群 $A_s$ の同型成分を $\mathfrak{a}_{\lambda}$ で表します。 $\mathscr{S}$ の部分集合 Λ については、集合 $\mathfrak{a}_{\Lambda}=\sum_{\lambda\in\Lambda}\mathfrak{a}_{\lambda}$ となります。

#### 命題 9 {#alg-viii-s8-prop-9 .statement tag=009H}

a) 包含による A の両面理想の $\mathscr{S}$ の部分集合および集合 $\mathscr{B}_A$ の位数集合 $\mathfrak{P}(\mathscr{S})$。 写像 $\Lambda \mapsto \mathfrak{a}_{\Lambda}$ は、$\mathfrak{P}(\mathscr{S})$ から $\mathscr{B}_A$ までの順序集合の同型です。

b) A の最小の両側イデアルは、イデアル $\mathfrak{a}_{\lambda}$ です。

c) すべての$\lambda \in \mathscr{S}$に対して$\mathfrak{b}_{\lambda}=\mathfrak{a}_{\mathscr{S}-\{\lambda\}}$があり、イデアル$\mathfrak{b}_{\lambda}$はAの最大の両側イデアルです。

d) A から $A/\mathfrak{b}_{\lambda}$ までの $\lambda \in \mathscr{S}$ 、 標準写像 、 $\mathfrak{a}_{\lambda}$ から $A/\mathfrak{b}_{\lambda}$ までの A-加群の誘導する同型について。

主張 a) は、命題 8 から続き、VIII、p. 87 の d) は、A-加群 $A_s$ に適用されます。 A の最小の両側イデアルは $\mathfrak{a}_{\lambda}$ であり、最大の両側イデアルは $\mathfrak{c}_{\lambda}=\mathfrak{a}_{\mathscr{S}-\lambda}$ ($\lambda \in \mathscr{S}$ の場合) であるということになります。

$\lambda \in \mathscr{S}$ごとに$\mathfrak{b}_{\lambda}$と$\mathfrak{c}_{\lambda}$の等式を表示する必要があります。 $\mathscr{S}$ では $\lambda$ と $\mu$ を区別します。 The A-submodule $\mathfrak{a}_\mu S_{\lambda}$ of $S_{\lambda}$ is the union of the images of the linear mappings $a\mapsto ax$ from $\mathfrak{a}_\mu$ to $S_{\lambda}$ for $x\in S_{\lambda}$. 従って、零となり、$\mathfrak{a}_\mu\subset \mathfrak{b}_{\lambda}$となります。 従って、$\mathfrak{c}_{\lambda}$ は A の最大の両側イデアルであり、$\mathfrak{b}_{\lambda}$ は A とは異なるため、$\mathfrak{c}_{\lambda}\subset \mathfrak{b}_{\lambda}$ が得られ、最後に $\mathfrak{c}_{\lambda}=\mathfrak{b}_{\lambda}$ が得られます。

#### 系 {#alg-viii-s8-n3-cor-1 .statement tag=009I}

$(A_i)_{i\in I}$ を A から $\prod_{i\in I}A_i$ までの単純な環と $f$ 同型の有限族とする。すべての $i\in I$ に対して、pr$_i\circ f$ の核が $\mathfrak{b}_{\varphi(i)}$ となるように、$\mathscr{S}$ の一意元 $\varphi (i)$ が存在します。 写像 $\varphi$ は、I から $\mathscr{S}$ までの全単射です。 写像 pr$_i\circ f$ 誘導する同型 $f_i$ $A/\mathfrak{b}_{\varphi(i)}$ から $A_i$ まで、$i\in I$ ごとに。

従って、$f$は、半単純環の分解の$f_i($「一意性」から推定される、Aから$\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$までの標準同型の合成と、$\prod_{\lambda\in\mathscr{S}}A/\mathfrak{b}_{\lambda}$から$\prod_{i\in I}A_i$までの同型です。シンプルな環の積」）。

系を証明しましょう。 $i\in I$ にしましょう。 pr$_i\circ f$の核を$\mathfrak{b}'_i$で示します。単純な環 $A_i$ は $A/\mathfrak{b}'_i$ と同型であるため、A の両側イデアル $\mathfrak{b}'_i$ は最大になります。 命題 8, c) までに、$\mathscr{S}$ のうち一意元 $\varphi (i)$ が存在し、$\mathfrak{b}'_i=\mathfrak{b}_{\varphi(i)}$ が得られます。 移行から商の場合、$A/\mathfrak{b}_{\varphi(i)}$ から $A_i$ までは $_i\circ f$ 定義する同型 $f_i$ となります。さらに、$i\not=j$と$\cap_{i\in I}\mathfrak{b}'_i= 0$なら$\mathfrak{b}'_i+\mathfrak{b}'_j= A$になります（cf.I, §8, No. 11、p. 110、命題10）。これと命題 8 から、$\varphi$ は I から $\mathscr{S}$ までの全単射であることがわかります。

#### 命題 10 {#alg-viii-s8-prop-10 .statement tag=009J}

Aの中心をZで表します。$\lambda \in \mathscr{S}$の場合、$Z_{\lambda}$を体の$D_{\lambda}$の中心とします。

a) 写像 $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}}$ は、環 Z から積 $\prod_{\lambda\in\mathscr{S}}Z_{\lambda}$ までの同型です。

b) Z のイデアルの位数集合 $\mathscr{I}_Z$ および包含による A の両側イデアルの集合 $\mathscr{B}_A$。 写像 $\mathfrak{a}\mapsto \mathfrak{a}A$ は、$\mathscr{I}_Z$ から $\mathscr{B}_A$ までの順序集合の同型です。 逆同型は、A の両側理想 $\mathfrak{b}$ を Z の理想 $\mathfrak{b}\cap Z$ に送信します。

この命題は、VIII、p. 87の命題8をA-加群$A_s$に適用したもので、その双可換子はAです。

#### 系 {#alg-viii-s8-n3-cor-2 .statement tag=009K}

Bを環とします。次のプロパティは同等です。

(i) 環 B は単純です。

(ii) 環 B は半単純で、その中心は体です。

(iii) 環 B は半単純であり、B 単純モジュールの類は 1 つだけ存在します。

#### 命題 11 {#alg-viii-s8-prop-11 .statement tag=009L}

$\lambda \in \mathscr{S}$ にしましょう。 A の同型成分 $\mathfrak{a}_{\lambda}$ は、型 $S_{\lambda}$ の $A_s$ の同型成分と型の $A_d$ の同型成分の両方です$S^*_{\lambda}$。さらに、私たちは、

(1) $[A_s: S_{\lambda}] = [A_d: S^*_{\lambda}] =$ 薄暗い$_{D_{\lambda}}S_{\lambda}$

そして

(2) 長(A) = 長(A$^o$) $=\sum_{\lambda\in\mathscr{S}}$ 薄$_{D_{\lambda}}S_{\lambda}$。

最初の主張は、命題 6、c) の VIII、p. 139 の特定のケース $M = A_s$ です。 等式 $[A_s: S_{\lambda}] = [A_d: S^*_{\lambda}]$ は、左A-加群 $A_s$ の双対が右A-加群 $A_d$ と同型であるため、VIII、p. 140 の命題 7 から続きます。 命題 8、a) および 9、c)、写像 $a\mapsto a_{S_{\lambda}}$ 定義する同型左A-加群から$\mathfrak{a}_{\lambda}$ まで$_{D_{\lambda}}(S_{\lambda})$ まで。 $[A_s: S_{\lambda}]$ は、定義により、左A-加群 $\mathfrak{a}_{\lambda}$ の長さなので、補題 2 の VIII から関係 $[A_s: S_{\lambda}] =$ 薄$_{D_{\lambda}}S_{\lambda}$ が続きます。 p. 121。最後に、和に$\lambda$を掛けて、(1)から関係(2)が得られます。

#### スコリウム {#alg-viii-s8-n3-sch-1 .statement tag=009M}

A を半単純環、Z を中心とします。次の集合の間には正規の全単射が存在します。

a) 集合 $\mathscr{S}(A)$ の類の単純な左A-加群

b) 集合 $\mathscr{S}(A^o)$ の類の単純右A-加群

c) A の最小の両面理想の集合

d) A の最大の両側イデアルの集合

e) シンプルな Z モジュールの集合 $\mathscr{S}(Z)$ の類

f) Z の最小限の理想の集合

g) Z の最大理想の集合。

したがって、$\mathscr{S}$ (A) のすべての元 $\lambda$ には、単純右A-加群 $S^*_{\lambda}$ の対応する類 $\lambda^*$、$S_{\lambda}$ の双対、A の最小の両側理想$\mathfrak{a}_{\lambda}$ (等型) が存在します。 成分 of $A_s$ of 型 $\lambda$ )、A の最大両側イデアル $\mathfrak{b}_{\lambda}$ (消滅子 of 単純加群 $S_{\lambda}$)、単純な Z モジュールの類 $Z\cap \mathfrak{a}_{\lambda}$、最小イデアルZの$Z\cap \mathfrak{a}_{\lambda}$とZの最大理想$Z\cap \mathfrak{b}_{\lambda}$。

#### 命題 12 {#alg-viii-s8-prop-12 .statement tag=009N}

M を半単純環 A および M のサポート $\mathscr{S}_M\subset \mathscr{S}$ 上の加群とします。そのとき、M の消滅子 Ann(M) は両側イデアル $\sum_{\lambda\in\mathscr{S}-\mathscr{S}_M}\mathfrak{a}_{\lambda}$ であり、M のトレース イデアル $\tau (M)$ は両側イデアル $\sum_{\lambda\in\mathscr{S}_M}\mathfrak{a}_{\lambda}$ です。特にAはアン(M)の直和と$\tau (M)$です。

定義 (VIII, p. 84)$,\mathscr{S}_M$ は、M の単純部分加群の類で構成されます。 加群 M は半単純なので、M の消滅子は、$\mathscr{S}_M$ を通る $\lambda$ に対して、消滅子の共通部分 $\mathfrak{b}_{\lambda}$ の類 $\lambda$ の加群です。 これで、$\lambda \in \mathscr{S}$ (命題 9) ごとに $\mathfrak{b}_{\lambda}=\sum_{\mu\not=\lambda}\mathfrak{a}_\mu$ が得られます。 A は族 $(\mathfrak{a}_{\lambda})_{\lambda\in\mathscr{S}}$ の直和であるため、M の消滅子は確かに $\sum_{\lambda\in\mathscr{S}-\mathscr{S}_M}\mathfrak{a}_{\lambda}$ に等しい。

定義 (VIII、p. 80) により、理想的なトレース $\tau (M)$ は、M から $A_s$ までの A-線型写像の像によって生成される $A_s$ の A-部分加群です。 Mは半単純なので、$A_s$の単純部分加群と類所属から$\mathscr{S}_M$によって$\tau (M)$が生成されると言うのと同じになります。したがって、$\tau (M) =\sum_{\lambda\in\mathscr{S}_M}\mathfrak{a}_{\lambda}$ となります。

#### 系 {#alg-viii-s8-n3-cor-3 .statement tag=009O}

M を半単純環 A 以上の加群とします。以下のプロパティは同等です。

(i) A-加群 M は忠実です。

(ii) M のサポートは $\mathscr{S}$ に等しい。

(iii) A-加群 M は生成するです。

確かに、M が忠実であるというというは、そのトレースが A (VIII、p. 80、定理 1) に等しい場合にのみ、その消滅子が 0 に減らされ、M が生成するであることを意味します。

### 4. べき等と半単純環

Aを環とします。 $e^2=e$ がある場合、A の元 $e$ は冪等 (I, §1, No. 4, p. 7) と呼ばれることを思い出してください。これは、A の反対環 $A^o$ の冪等元でもあります。

#### 命題 13 {#alg-viii-s8-prop-13 .statement tag=009P}

a) A の左イデアル $\mathfrak{a}$ は、$\mathfrak{a}= Ae$ となるような冪等 $e$ が A に存在する場合に限り、$A_s$ で補充を認めます。理想的な $\mathfrak{a}$ は、$x=xe$ となるような A の元 $x$ で構成されます。

b) A において $e$ と $f$ を冪等とします。$ef=e$ がある場合に限り、$Ae\subset Af$ が得られます。

c) M をA-加群とします。この場合、M が $Ae$ と同型であるような冪等 $e$ が A に存在する場合に限り、M は射影的かつ単次性になります。

A-加群 $A_s$ の自己準同型は、A の元による右側乗法です。 したがって、A-加群 $A_s$ の射影子は写像 $x\mapsto xe$ になります。ここで、$e$ は A の冪等です。 さらに、$A_s$の部分加群は左の理想であり、そのような部分加群は、射影子の像(II, §1, No. 9、p. 211、命題14)である場合に限り、補充を認めます。 主張 a) が続きます。

関係 $Ae\subset Af$ は $e\in Af$ と同等です。従って、a) により、それは $e=ef$ と同等になります。 主張 b)が続きます。

A-加群 M が一次であれば、全射A-線型写像 $u: A_s\rightarrow M$ が存在します。さらに、M が射影である場合、$u$ の核を補足する $A_s$ の部分加群 $\mathfrak{a}$ が存在します。次に、$\mathfrak{a}$ から M への $u$ 誘導する同型です。逆に、M が $A_s$ の直因子と同型の場合、それは単次で射影です。 主張したがって、c) は a) から続きます。

#### 注意 1 {#alg-viii-s8-n4-rem-1 .statement tag=009Q}

$\mathfrak{a}$ を A の左イデアルとします。 上記の証明と、A の冪等 $e$ の集合から、II, §1, No. 8、p. 209、写像 $e\mapsto A(1-e)$ 定義する全単射の命題 12 の系により、次のようになります。 $A_s=\mathfrak{a}\oplus \mathfrak{b}$ となるような A の左理想$\mathfrak{b}$ の$\mathfrak{a}= Ae$ から集合 。

#### 注意 2 {#alg-viii-s8-n4-rem-2 .statement tag=009R}

$e$ と $f$ を A の冪等とします。 命題 13、b) までに、$ef=e$ と $f e=f$ の場合に限り、$Ae= Af$ が得られます。従って、環 A が可換である場合、関係 $Ae= Af$ は $e=f$ と等価です。 例 $A =\mathbf{M}_2(\mathbf{Z}), e = \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix}$ および $f = \begin{pmatrix} 1 & 0 \\ 1 & 0 \end{pmatrix}$ が示すように、これは一般には当てはまりません。

環 A のべき等 $e$ と $e'$ は、$ee'=$ $e'e= 0$ の場合に直交すると言います。 $(e_i)_{i\in I}$ を A のペアごとの直交冪等の有限族とします。

$$
(\sum_ie_i)^2=\sum_ie^2_i+\sum_{i\not=j}e_ie_j=\sum_ie_i
$$

A の元 $\sum_{i\in I}e_i$ はべき等です。

A の冪等 $e$ の分割は、$e=\sum_{i\in I}e_i$ となる A の対直交冪等の有限族 $(e_i)_{i\in I}$ です。 0 と $e$ とは異なるペアごとの直交冪等の $e$ からなるの分割が存在する場合、A の冪等 $e$ が分解可能であると言います。逆の場合は、不分解であると言います。 0 は分解可能な冪等であることに注意してください。

#### 命題 14 {#alg-viii-s8-prop-14 .statement tag=009S}

$e$ を A の冪等とします。

a) $(e_i)_{i\in I}$ が $e$ の分割である場合、A-加群 $Ae$ はファミリー $(Ae_i)_{i\in I}$ の直和です。

b) $(\mathfrak{a}_i)_{i\in I}$ を、直和 $Ae$ を持つ A の左イデアルの有限族とする。 $i\in I$については、$\mathfrak{a}_i$の$e$の成分を$e_i$で表します。すると、$(e_i)_{i\in I}$ は $e$ の分割となり、$i\in I$ ごとに $\mathfrak{a}_i= Ae_i$ が得られます。

c) A-加群 $Ae$ は、べき等 $e$ が分解不可能な場合に限り、分解不可能です。

$(e_i)_{i\in I}$ を $e$ の分割とします。 $i\in I$ ごとに、

$$
e_ie=\sum_je_ie_j=e^2_i+\sum_{j\not=i}e_ie_j=e_i
$$

従って $Ae_i\subset Ae$ です。すべての $i\in I$ に対して、設定 $p_i(x) =xe_i$ により、$Ae$ の A 線形射影子 $p_i$ が定義する計算されます。 $i\not=j$ であれば $p_ip_j= 0$ があり、$Ae$ では $x$ ごとに、

$$
x=xe=\sum_ixe_i=\sum_ip_i(x)
$$

従って、(II, §1, No. 8, p. 20, 命題 $12$)$, Ae$ は、$p_i$ の像の直和です。今、$ee_i=e_ie=e_i$があるので、$p_i$の像は$Ae_i$です。これは a) を証明します。

b)の記法と仮定を取ります。 $i\in I$ にしましょう。 $e_i$ 属するから $Ae$ なので、$e_i=e_ie=\sum_je_ie_j$ になります。 $Ae$は$j$ごとに$\mathfrak{a}_j$と$e_ie_j$属するから$\mathfrak{a}_j$の直和なので、$i\not=j$には$e_i=e_ie_i$と$e_ie_j= 0$が入ります。他の語では、$(e_i)_{i\in I}$は冪等$e$の分割です。 a)により、$Ae$は$Ae_i$の直和になります。 仮定までに$Ae_i\subset \mathfrak{a}_i$があり、$Ae$は$\mathfrak{a}_i$の直和です。従って、$i\in I$ ごとに $Ae_i=\mathfrak{a}_i$ が得られます。 b)を証明しました。

最後に、a) と b) の直後に c) が続きます。

#### 注意 3 {#alg-viii-s8-n4-rem-3 .statement tag=00R8}

適用 A の反対環までの以前の結果から、特に、M が $eA$ と同型であるような冪等 $e$ が A に存在する場合に限り、単次の右A-加群 M は射影であることがわかります。さらに、$e$ が分解不可能である場合に限り、$eA$ は分解不可能な権利加群です。

ここで、環 A が半単純であると仮定し、単純な左A-加群の類の集合を $\mathscr{S}$ で表します。 A-加群 $A_s$ は半単純で、$A_s$ のすべての部分加群は直因子です。 $\mathfrak{a}$ を A の左イデアルとします。上記により、$\mathfrak{a}= Ae$ および A-加群 $\mathfrak{a}$ が分解不可能な場合に限り、つまり $e$ が分解不可能な場合に限り、A に冪等な $e$ が存在します。

$(\mathfrak{m}_i)_{i\in I}$ を、$A_s=\oplus_{i\in I}\mathfrak{m}_i$ となるような A の最小左イデアルの族とする。 命題 14 までに、$i\in I$ ごとに $\mathfrak{m}_i= A\varepsilon_i$ となるような分解不可能な冪等の 1 からなるのうち分割 $(\varepsilon_i)_{i\in I}$ が存在します。

すべての $\lambda \in \mathscr{S}$ について、$S_{\lambda}$ を類 $\lambda$ の A-加群とし、$\mathfrak{a}_{\lambda}$ を型 $\lambda$ の A-加群 $A_s$ の同型成分とします。 A は家族 $(\mathfrak{a}_{\lambda})_{\lambda\in\mathscr{S}}$ の直和であるため、$\lambda \in \mathscr{S}$ ごとに $\mathfrak{a}_{\lambda}= Ae_{\lambda}$ となる 1 の分割 $(e_{\lambda})_{\lambda\in\mathscr{S}}$ が存在します。 $\lambda \in \mathscr{S}$ については、単純A-加群 $\mathfrak{m}_i$ が型 $\lambda$ となるように、添字 $i\in I$ の $I(\lambda )$ 集合で表します。 命題 4、b) の VIII、p. 65 までに、

$$
\mathfrak{a}_{\lambda}=\bigoplus_{i\in I(\lambda)}\mathfrak{m}_i \tag{3}
$$

冪等元 $e_{\lambda}$ は $\mathfrak{a}_{\lambda}$ の 1 の成分なので、$e_{\lambda}=\sum_{i\in I(\lambda)}\varepsilon_i$ です。

#### 命題 15 {#alg-viii-s8-prop-15 .statement tag=009T}

環 A が半単純であるとします。

a) すべての $\lambda \in \mathscr{S},e_{\lambda}$ は、満たす関係 $(e_{\lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$ の中心 Z の一意元と、$\mu\not=\lambda$ の $(e_{\lambda})_{S_\mu}= 0$ です。

b) 環 Z の分解不可能なべき等は $e_{\lambda}$ であり、Z の最小イデアルは $\lambda \in \mathscr{S}$ の $Ze_{\lambda}$ です。

c) M を A-加群およびその同型成分のファミリーである $(M_{\lambda})_{\lambda\in\mathscr{S}}$ とします。 $M_{\lambda}$ (VIII、p. 65) の直和に M の分解を関連付けた射影子のファミリーは $((e_{\lambda})_M)_{\lambda\in\mathscr{S}}$ であり、$\lambda \in \mathscr{S}$ ごとに $M_{\lambda}=\mathfrak{a}_{\lambda}M$ があります。

$\mathscr{S}$ では、$\lambda$ と $\mu$ を区別します。 $e_{\lambda}\in \mathfrak{a}_{\lambda}$ があり、$\mathfrak{a}_{\lambda}$ は A-加群 $S_\mu$ (VIII、p. 142、命題 9) の消滅子 $\mathfrak{b}_\mu$ に含まれます。従って、$(e_{\lambda})_{S_\mu}= 0$ となります。 $1 =\sum_{\nu\in\mathscr{S}}e_{\nu}$ があるため、関係 $(e_{\lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$ が続きます。 主張 a) は、VIII、p. 141 の 8 の命題の帰結になります。

$\lambda$ を $\mathscr{S}$ に入れます。 A の両側理想 $\mathfrak{a}_{\lambda}$ は、$x=xe_{\lambda}$ となるような元 $x$ で構成されます。従って、$Z\cap \mathfrak{a}_{\lambda}= Ze_{\lambda}$ があり、従って b) 命題 10 により、b)。

c)を証明しましょう。 $x$ を M の元とします。すべての $\lambda \in \mathscr{S}$ に対して $e_{\lambda}\in \mathfrak{a}_{\lambda}$ が得られます。 $A_s$ から M までの写像 $a\mapsto ax$ は A 線形であるため、$\mathfrak{a}_{\lambda}x\subset M_{\lambda}$ (VIII、p. 66、命題 5)、特に $e_{\lambda}x\in M_{\lambda}$ が得られます。 $1 =\sum_{\lambda\in\mathscr{S}}e_{\lambda}$ があるため、$x=\sum_{\lambda\in\mathscr{S}}e_{\lambda}x$ になります。従って、$e_{\lambda}x$は$M_{\lambda}$の$x$の成分になります。

#### 注意 4 {#alg-viii-s8-n4-rem-4 .statement tag=009U}

環 A が半単純であるとします。 Let $(e_i)_{i\in I}$ be a partition of 1 consisting of nonzero idempotents in the center Z of A. Card(I) = Card($\mathscr{S}$) の場合、$e_i$ は Z の分解不可能な冪等です。

### 練習問題 {#alg-viii-s8-exercises}

[§ 8 に対して練習問題](exercises/s8/)を参照してください。
