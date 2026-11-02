---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 14
section_title: Central Simple Algebras
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.251-A VIII.276
pdf_pages: 0268-0293
extraction: native
subsections:
    - "no": 1
      title: Central Simple Algebras
      page: 251
      pdf_page: 268
    - "no": 2
      title: Two Lemmas on Bimodules
      page: 254
      pdf_page: 271
    - "no": 3
      title: Conjugacy Theorems
      page: 256
      pdf_page: 273
    - "no": 4
      title: Automorphisms of Semisimple Algebras
      page: 257
      pdf_page: 274
    - "no": 5
      title: Simple Subalgebras of Simple Algebras
      page: 259
      pdf_page: 276
    - "no": 6
      title: Maximal Commutative Subalgebras
      page: 261
      pdf_page: 278
    - "no": 7
      title: Maximal Étale Subalgebras
      page: 264
      pdf_page: 281
    - "no": 8
      title: Diagonalizable Subalgebras of Simple Algebras
      page: 266
      pdf_page: 283
statements: 36
exercises: 19
content_sha256: 557f52f08bb86c25e0e2f0d1300ee2e37e6259d0061c8dd08d9f71fb9b40aebe
translated_from: content/en/alg/VIII/14_s14_central_simple_algebras.md
translation_method: google
source_content_sha256: 6b4399d77699c060fb6846778021967e62ae015f18624ee87348066955fdf6f2
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: f8f477e11274ab60c4e55554cbe01046656b041c1f664515a6eb1f94e262d505
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 14。中央単純代数

この切断において、Kは可換体です。

### 1. 中央単純代数

#### 定義 1 {#alg-viii-s14-def-1 .statement tag=00GE}

写像 $\lambda \mapsto \lambda 1$ が K から A の中心までの全単射である場合、体 K 上の代数 A が中心であると言います。

中心の代数は 0 に減りません。すべての整数 $n\geqslant 1$、行列 K-代数 $\mathbf{M}_n(K)$ は中心 (VIII、p. 83、系 2) と単純 (VIII、p. 120、 定理 1）。より一般的には、D を有限次数の中心の K-代数とします。そうすると、$\mathbf{M}_n(D)$も中心になります。 A を単純な環とします。その中心 Z は体 (VIII, p. 121, 系 1) であり、従って A は Z 上の中心単純代数です。体 K が代数的に閉じている場合、K 上の有限次数の単純代数が中心になります。 (VIII、p. 122、系 3)。中央の単純代数の反対多元環は中央のシンプルです。

#### 注意 1 {#alg-viii-s14-n1-rem-1 .statement tag=00GF}

A と B をK-代数とします。 $A\otimes_KB$ が中心の単純代数である場合、A と B (命題 6 の III, §4, No. 4、p. 468、系および VIII、p. 221、命題 6) も同様です。 Conversely, if A and B are central simple algebras and if one of them has finite degree over K, then $A\otimes_KB$ is a central simple algebra (III, §4, No. 4, p. 468, Corollary of Proposition 6 and VIII, p. 222, Corollary 2).

#### 注意 2 {#alg-viii-s14-n1-rem-2 .statement tag=00GG}

A を体 K の K-代数および L 拡大とします。L-代数 $A_{(L)}$ が中心単純である場合、K-代数 A は中心単純です。逆に、次数 [A : K] と [L : K] のいずれかが有限で、A が中心単純K-代数の場合、L-代数 $A_{(L)}$ は中心単純です。これは、VIII、p. 222の系2から続きます。

#### 注意 3 {#alg-viii-s14-n1-rem-3 .statement tag=00GH}

A と B を森田相当K-代数とします。 代数 A は、B が (VIII, p. 105, 命題 6; p. 111, 系; および p. 102, 系 1) である場合に限り、中心単純です。

#### 注意 4 {#alg-viii-s14-n1-rem-4 .statement tag=00GI}

特に、A が中心単純K-代数および $n\geqslant 1$ の場合、$\mathbf{M}_n(A)$ は中心単純K-代数 (VIII、p. 102、例 1) です。

#### 定理 1 {#alg-viii-s14-thm-1 .statement tag=00GJ}

A を有限次数の K-代数とします。次のプロパティは同等です。

(i) 代数 A は中心単純です。

(ii) 代数 A は中心であり、根基はありません。

(iii) The canonical homomorphism from the K-algebra $A\otimes_KA^o$ to the K-algebra End$_K(A)$ that sends $a\otimes a'$ to the K-linear mapping $x\mapsto axa'$ from A to A is bijective.

(iv) 体 K と整数 $n\geqslant 1$ の拡大 L が存在し、L-代数 $A_{(L)}$ と $\mathbf{M}_n(L)$ が同型となる。

(v) K のすべての分離閉包 $K'$ に対して、$K'$-代数 $A_{(K')}$ と $\mathbf{M}_n(K')$ が同型であるような整数 $n\geqslant 1$ が存在します。

(vi) There exist a Galois extension L of the field K of finite degree and an integer $n\geqslant 1$ such that the L-algebras $A_{(L)}$ and $\mathbf{M}_n(L)$ are isomorphic.

(vii) There exist a K-algebra of finite degree D that is a field with center K and an integer $n\geqslant 1$ such that the algebra A is isomorphic to the algebra $\mathbf{M}_n(D)$.

環は、それが半単純であり、その中心が体 (命題 10 の VIII、p. 143、系) である場合に限り、単純です。 A は体 K 上の有限次数の代数であるため、左アルティン的環です。従って、根基 (VIII、p. 154、命題 4) がない場合に限り、半単純になります。 (i)と(ii)の同値が続きます。

集合 $E = A\otimes_KA^o$ および F = 終了$_K(A)$; A の $x, a, a'$ に対して関係 $\varphi (a\otimes a')(x) =axa'$ によって定義される E から F までの $\varphi$ 標準準同型で表します。 代数 A が中心単純である場合、$A^o$ も中心単純であり、従って E (注意 1) であるため、$\varphi$ は単射です。今、$[E : K] = [A : K]^2= [F : K]$があるので、$\varphi$は全単射です。逆に、$\varphi$ が全単射であると仮定します。 代数 F は中心単純であるため (行列環 $\mathbf{M}_m$(K) と同型であるため)、E も同様であり、従って A (注意 1) も同様です。これで、(i) と (iii) の同値が証明されました。

注意 4 により、主張 (vii) は主張 (i) を意味します。 逆の含意は、VIII、p. 122 の系 3、および VIII、p. 83 の系 2 から続きます。

注意 2 によって、(vi) が (iv) を暗示し、(iv) が (i) を暗示することは明らかです。

(i)$\Rightarrow$(v)$\Rightarrow$(vi) の意味を証明することはまだ残っています。 A が中心単純であると仮定し、 $K'$ を K (V, §7, No. 8, p. 45) の分離閉包とします。すると、$A_{(K')}$ は、$K'$ (VIII、p. 251、注意 2) の上に、有限次数の中央の単純代数になります。 VIII, p. 231 の系により、$A_{(K')}$ から $\mathbf{M}_n(K')$ までの $K'$-代数の整数 $n\geqslant 1$ と同型が存在します。 $K'$-代数 $\mathbf{M}_n(K')$ と $\mathbf{M}_n(K)_{(K')}$ が同型であることに注目してください。 VIII, p. 234 の補題 4 までに、$K'$ の部分拡張 L が K 上で有限生成され、L-代数 $A_{(L)}$ と $\mathbf{M}_n(K)_{(L)}$ が同型となるように存在します。このとき、L は分離可能であり、K 上の有限次数であるため、ガロアである $K'$ と K 上の有限次数の部分拡張 $L'$ (V, §10, No. 1, p. 57, 命題 2) に含まれます。 $L'$-代数 $A_{(L')}$ と $\mathbf{M}_n(L')$ は同型です。

#### 系 1 {#alg-viii-s14-thm-1-cor-1 .statement tag=00GK}

A を分離閉体 K 上の有限次数の中心単純代数とします。A が行列環 $\mathbf{M}_n(K)$ と同型となるような整数 $n\geqslant 1$ が存在します。

実際、K のすべてのガロア拡大は K に等しい。 定理 1 の特性 (i) と (v) の同値を適用すれば十分です。

#### 系 2 {#alg-viii-s14-thm-1-cor-2 .statement tag=00GL}

A を K 上の有限次数の中心単純代数とします (たとえば、K 上の有限次数の中心 K の体)。 $[A : K] =n^2$ となるような整数 $n\geqslant 1$ が存在します。

L を K の拡大とし、$n$ を厳密には正の整数とし、L-代数 $A_{(L)}$ と $\mathbf{M}_n(L)$ が同型であるようにします。我々は持っています

$$
[A : K] = [A_{(L)}: L] = [\mathbf{M}_n(L) : L] =n^2
$$

系 2 の記法において、整数 $n$ は A の縮小された次数と呼ばれます。

#### 注意 5 {#alg-viii-s14-n1-rem-5 .statement tag=00GM}

A を K 上の有限次数の中心単純代数とし、その還元された次数は素数数 $\ell$ です。この場合、A は体であるか、A は $\mathbf{M}_{\ell}(K)$ と同型です。確かに、A は形 $\mathbf{M}_n$(D) の代数と同型であり、D は体と中心 K であり、次のようになります。

$$
\ell^2= [A : K] =n^2[D : K]
$$

A が体ではない場合、$n\not= 1$ なので、$n=\ell$ となり、D = K となります。

### 2. 両側加群に 2 つの補題

A と B を環とします。 B から A までの任意の準同型 $f$ について、$(b, a)\mapsto f(b)a$ で与えられる左B-加群構造に対して、基礎となる右A-加群 $A_d$ および外部法則を持つ $(B$, A)-bimodule を $A^f$ で表します。

#### 補題 1 {#alg-viii-s14-lem-1 .statement tag=00GN}

$f$ と $g$ を B から A までの準同型とします。次の条件は同等です。

(i) $(B,A)$-バイモジュール $A^f$ と $A^g$ は同型です。

(ii) $g=\theta \circ f$ となる A の内部自己同型 (I, §8, No. 4, p. 102, 例 2) $\theta$ が存在します。

右A-加群 $A_d$ の自己同型は写像 $x\mapsto ax$ で、$a$ は A の可逆元です。そのような自己同型は、$A^f$ から $A^g$ までの B-線型写像です。

$$
g(b)ax=af(b)x
$$

A のすべての $x$ と B のすべての $b$ に対して。 この関係は、B のすべての $b$ の $g(b) =af(b)a^{-1}$、つまり $g=\theta \circ f$ に相当します。ここで、$\theta$ は A の内部自己同型 $x\mapsto axa^{-1}$ です。

#### 補題 2 {#alg-viii-s14-lem-2 .statement tag=00GO}

B が中心 Z に対して有限生成加群である半単純環であるとします。M と N を $(B,A)$ ビモジュールとします。彼らが有限長を持っていると仮定します (これは特に、有限長の右A-加群である場合に当てはまります)。 M と N が $(Z,A)$-bimodule と同型である場合、それらは $(B,A)$-bimodule と同型です。

A) まず、B が可換体 L よりも有限次元 $d$ のベクトル空間の自己準同型環である場合を考えてみましょう。 すると、Z = L となります。 S を $(B$, Z)-bimodule として見ます。 環 B は単純、S は単純B-加群、Z は S の交換子環です。すべての B-加群は型 S (VIII、p. 122、命題 2 a)) と同型です。 $(V, \alpha )$ (それぞれ $(W, \beta )$) を B-加群 M (それぞれ N) の記述とします。 The set V (resp. W) is endowed with a $(Z$, A)-bimodule structure such that $\alpha$ (resp. $\beta$ ) is an isomorphism of $(B$, A)-bimodules (VIII, p. 64, Remark 2). As $(Z$, A)-bimodules, M is isomorphic to $V^d$ and N to $W^d$, and there exists an isomorphism from the set of $(Z$, A)-sub-bimodules of V, ordered by inclusion, to that of the $(B$, A)-sub-bimodules of M (loc. cit.). したがって、V は $(Z$、有限長の A)-bimodule であり、W も同様です。 $(Z,A)$-bimodules $V^d$ と $W^d$ は同型であるため、$(Z$、A)-bimodule V および W は、VIII、p. 37 の定理 2、d) を環に適用することによって同型です。 $Z\otimes_{\mathbf{Z}}A^o$。 最後に、$(B$、A)-バイモジュール M と N は同型です。

B) ここで、B が Z モジュールとして有限生成される単純な環である場合を考えてみましょう。 このとき、Z は体で、B は体 Z 上の有限次数の中心単純代数です。 VIII, p. 252 の定理 1 により、$Z'$-代数 $B'= B_{(Z')}$ が有限次元 $Z'$-ベクトル空間の自己準同型環と同型となるように、Z 上で有限次数の Z の拡大 $Z'$ が存在します。 集合 $M'= M_{(Z')}$ と $N'= N_{(Z')}$。 すると、$M'$ と $N'$ は $(B'$、A) 有限長の双モジュールです。 $(Z'$、A)-bimodule、$M'$、$N'$ は同型であると見なされます。 $A), M'$ と $N'$ は $(B'$, A)-bimodules と同型であり、なおさらは $(B$, A)-bimodules と同型です。 集合 $r= [Z': Z]$。 $(B$、A)-bimodule $M'= Z'\otimes_ZM$ は $M^r$ と同型であり、同様に、$(B$、A)-bimodule $N'$ は $N^r$ と同型です。 M と N は有限長の $(B$, A)-双モジュールであるため、VIII, p. 37 の定理 2, d) から、$(B$, A)-双モジュール M と N は同型であることがわかります。

C) 最後に、B が Z 加群として有限生成される半単純環である一般的な場合を考えてみましょう。 $\mathscr{S}$ を集合 of 類 of 単純B-加群とします。それは有限です (VIII、p. 136、命題 1)。任意の $\lambda \in \mathscr{S}$ について、B-加群 M (それぞれ N) の型 $\lambda$ の同型成分を $M_{\lambda}$ (それぞれ $N_{\lambda}$) で表します。それは M (それぞれ N) の $(B$、A) サブバイモジュールです (注意、VIII、p. 67)。 $\lambda \in \mathscr{S}$ については、B-加群 $\lambda$ の消滅子を $\mathfrak{b}_{\lambda}$、集合 $B_{\lambda}= B/\mathfrak{b}_{\lambda}$ で表します。 $Z_{\lambda}$を$B_{\lambda}$の中心とします。 $\lambda \in \mathscr{S}$ の場合、$(B_{\lambda}$、A) ビモジュール $M_{\lambda}$ および $N_{\lambda}$ には有限長があります。次に、単純な環 $B_{\lambda}$ の積で同一視する B を、$Z_{\lambda}$ (VIII、p. 141、命題 8) の積で Z を得ることができます。さらに、$\prod_{\lambda\in\mathscr{S}}M_{\lambda}$で同一視できるM、$\prod_{\lambda\in\mathscr{S}}N_{\lambda}$でNです。 仮定までに、M と N は $(Z$、A)-bimodules と同型になります。従って、$\lambda \in \mathscr{S}, M_{\lambda}$ と $N_{\lambda}$ は同型の $(Z_{\lambda}$、A)-双加群であることがわかります。 B) で扱ったケースでは、$(B_{\lambda}$, A)-双モジュール $M_{\lambda}$ と $N_{\lambda}$ は同型であり、従って $(B$, A)-双モジュール M と N も同型です。

#### 注意 {#alg-viii-s14-n2-rem-1 .statement tag=00GP}

補題 2 の証明から、M と N は有限長の $(Z,A)$ 双モジュールであることがわかります。従って、B と A が、それぞれの中心 Z(B) と Z(A) 上で有限生成加群である 2 つの半単純環である場合、(Z(B),Z(A)) 双加群と同型である有限長の 2 つの $(B$, A) 双加群は同型です。

### 3. 共役定理

#### 定理 2 {#alg-viii-s14-thm-2 .statement tag=00GQ}

B を半単純環、Z を中心とします。 B が有限生成された Z モジュールであると仮定します。 B から A まで、A を右アルティン環、$f$ と $g$ を環準同型とします。 $f$ と $g$ の制限に $f_Z$ と $g_Z$ を Z に書き込みます。次のプロパティは同等です。

(i) $g=\theta \circ f$ となる A の内部自己同型 $\theta$ が存在します。

(ii) $g_Z=\theta \circ f_Z$となるような A の内部自己同型 $\theta$ が存在します。

環 A は右アルティンなので、$A_d$ は有限長の右A-加群 (VIII, p. 6, 定理 1) です。従って、$A^f$ と $A^g$ は $(B$、A) 有限長の双加群です。 補題 1 (VIII, p. 254) により、主張 (i) は、$A^f$ と $A^g$ が同型の $(B$、A)-双モジュールであり、主張 (ii) が同型であることを意味します。 $(Z,A)$-バイモジュール。従って、(i) と (ii) の同値は、補題 2 (VIII, p. 254) から続きます。

#### 系 {#alg-viii-s14-n3-cor-1 .statement tag=00GR}

A と B が体 K よりも代数であるとします。B が中心単純で有限次数であり、A が右アルティンであると仮定します。 $f$と$g$をBからAまでK-代数準同型とします。$g=\theta \circ f$となるようなAの内部自己同型$\theta$が存在します。

定理 2 の記法では、Z = K であるため、$f_Z= 1_Z=g_Z$ となります。

#### 定理 3 (スコレム-ネーター) {#alg-viii-s14-thm-3 .statement tag=00S9}

A と B を単純K-代数とし、Z(A) と Z(B) を中心とします。 代数 B が K に対して有限次数を持ち、代数 $Z(A)\otimes_KZ(B)$ が体であると仮定します (これは、特に A または B が中心である場合に当てはまります)。 $f$と$g$をBからAまでK-代数準同型とします。$g=\theta \circ f$となるようなAの内部自己同型$\theta$が存在します。

VIII, p. 254 の補題 1 により、$(B,A)$ バイモジュール $A^f$ と $A^g$ が同型であることを証明するのに十分です。ここで、$A^f$ と $A^g$ を代数 $C = B\otimes_KA^o$ 上の左加群として見ることができます。これは、VIII、p. 221 の命題 7 によって簡単になります。 右A-加群、$A^f$、$A^g$ は $A_d$ と同型なので、環 A は単純 (VIII, p. 121, 系 1) であるため、有限長になります。 なおさら、$A^f$、$A^g$ は、有限長の C モジュールです。 S を単純な C モジュールとしましょう。 $A^f$ が $S^m$ と同型、$A^g$ が $S^n$ となるように、厳密に正の整数 $m$ と $n$ が存在します。従って、右A-加群 S は非零有限長になります。 $A^f$ と $A^g$ の基礎となる右A-加群は同型であるため、同じ長さを持ちます。従って、$m=n$ があり、C 加群 $A^f$ と $A^g$ は同型になります。

#### 系 1 {#alg-viii-s14-thm-3-cor-1 .statement tag=00GS}

A を K 上の中心単純代数とし、L を有限次数の K の拡大とします。 $f$と$g$がLからAまでK-代数準同型である場合、$g=\theta \circ f$となるようなAの内部自己同型$\theta$が存在します。

#### 系 2 {#alg-viii-s14-thm-3-cor-2 .statement tag=00GT}

AをK上の中心単純代数とし、LをAの部分代数つまり体とします。 A の L から拡大する内部自己同型までの K-代数準同型ごと。

#### 系 3 {#alg-viii-s14-thm-3-cor-3 .statement tag=00GU}

D を中心 K で K を超える有限次数の体とします。 D のすべての元は K に対して代数的です。 Let $x$ and $y$ be elements of D; there exists an element $a$ of $D^*$ such that $y=axa^{-1}$ if and only if $x$ and $y$ have the same minimal polynomial over K.

最初の主張は、V, §3, No. 1、p. 17 の系 1 から続きます。

$y=axa^{-1}$ となるような $D^*$ の元 $a$ が存在すると仮定します。 K[X] のすべての多項式 P に対して、$P(y) =aP(x)a^{-1}$ が得られ、特に、$P(y) = 0$ の場合に限り、$P(x) = 0$ が得られます。従って、$x$ と $y$ は、K に関する同じ最小多項式 (V, §3, No. 1、p. 16、定理 1) を持ちます。

逆に、$x$ と $y$ が同じ最小多項式を持つと仮定します。ロケ地にて。前述のとおり、$u(x) =y$ および $K[x]$ が体となるような、$K[x]$ から $K[y]$ までの K-同型写像 $u$ が存在します。 D の系 2$,u$ 拡大するから内部自己同型 $\theta :z\mapsto aza^{-1}$ により、$y=\theta (x) =axa^{-1}$ が得られます。

#### 命題 1 {#alg-viii-s14-prop-1 .statement tag=00GV}

A を K 上の有限次数の中心単純代数とします。B を K-代数とし、B から A までの $f$ と $g$ を代数準同型とします。以下のプロパティは等価です。

(i) $g=\theta \circ f$ となる A の内部自己同型 $\theta$ が存在します。

(ii) 左B-加群と同様に、$A^f$ と $A^g$ は同型です。

補題 1 (VIII, p. 254) により、性質 (i) は、$A^f$ と $A^g$ が $(B$, A)-bimodules と同型であるという事実と等価です。 A は $K, A^f$ 上で有限次元なので、$A^g$ は有限長の B-加群です。 A の中心は K に等しいため、(i) と (ii) の同値は、VIII の補題 2 から続き、$(A^o,B^o$) バイモジュール $A^f$ と $A^g$ に適用される p. 254 です。

### 4. 自己同型/半単純代数

#### 定理 4 {#alg-viii-s14-thm-4 .statement tag=00GW}

A を半単純環、Z を中心、A の $u$ 自己同型とします。A が有限生成された Z モジュールで、Z の $z$ ごとに $u(z) =z$ があるとします。その場合、$u$ は内部自己同型になります。

これは、$f=$ Id$_A$ および $g=u$ を適用したVIII、p. 256 の定理 2 から続きます。

#### 例 {#alg-viii-s14-n4-exa-1 .statement tag=00RH}

定理 4 は、次の 2 つの特定のケースに適用されます。

a) D を体、Z を中心とします。 D が Z に対して有限次数を持つ場合、Z の元を固定する D のすべての自己同型は内部自己同型になります。 D が Z に対して有限次数を持つという仮定が必須です (VIII、p. 269、練習問題 4)。

b) V を体 K 以上の有限次元ベクトル空間とします。K-代数の終わり$_K(V)$ のすべての自己同型は内部自己同型です。この結果拡大するは、空間 V が​​ K 上の有限次元ではない場合 (VIII, p. 272, 練習問題 13) です。

特に、行列環 $\mathbf{M}_n(K)$ ($n\geqslant$ 1 を含む) のすべての自己同型は内部自己同型です。この結果から、以下の一般化が認められます。

#### 命題 2 {#alg-viii-s14-prop-2 .statement tag=00GX}

L を可換環とし、V を有限次元 $m$ の空き L モジュールとします。 $M^m$ が $L^m$ と同型であるようなすべての L 加群 M が L と同型であると仮定します。すると、L-代数終わり$_L(V)$ のすべての自己同型は内部自己同型になります。

集合 B = 終了$_L(V)$。 $u$ を L-代数 B の自己同型とします。V を左B-加群と見ます。 $u_*(V)$ を左B-加群と $u$ 、外部法則 $(b, v)\mapsto u(b)(v)$ (II, §1, No. 13, p. 221) に関連付けます。 $(e_1, . . . , e_m)$ を L モジュール V の基底とします。 V の元 $v_1, . . . , v_m$ が与えられると、$1\leqslant i\leqslant m$ に対して $b(e_i) =v_i$ が得られるような B の一意元 $b$ が存在します。他の語、元 $e= (e_1, . . . , e_m)$の$V^m$は、B-加群 $V^m$の基底を提供します。 $u$ は自己同型であるため、$e$ は B-加群 $u_*(V^m) =u_*(V)^m$ の基底も与えます。従って、これは $V^m$ と同型です。 $(B$、L) バイモジュール V は可逆です (VIII、p. 102、例 1)。 VIII, p. 103 の定理 2, b) により、B-加群 $u_*(V)$ が $V\otimes_LM$ と同型となるような L 加群 M が存在します。従って、B-加群 $V\otimes_LL^m$ と $V\otimes_LM^m$ は、それぞれ $V^m$ と $u_*(V)^m$ と同型です。ロケ地にて。前述のとおり、L モジュール $L^m$ と $M^m$ は同型です。 仮定が与えられると、M は L と同型です。従って、$V\otimes_LM$ と同型である B-加群 $u_*$(V) は、V と同型です。 $h$ を V から $u_*(V)$ までの B-加群同型とします。特に、L モジュール V の自己同型、つまり B の可逆元です。B の $b$ と V の $v$ については、$h(b(v)) =u(b)(h(v))$ があり、従って $u(b) =hbh^{-1}$ になります。

命題 2 の条件は、特に、可換環 L が主イデアル整域 (VII, §3, p. 15, 系 3) であるか、アルティン (VIII, p. 37、定理 2、d)) またはローカル (VIII、p. 36、系 6)。

### 5. 単純部分代数/単純代数

#### 定理 5 {#alg-viii-s14-thm-5 .statement tag=00GY}

A を中心単純K-代数とし、B を K 上の有限次数の A の半単純部分代数とします。

a) A の B の交換子環 $B'$ は単純部分代数で、B は A の $B'$ の交換子環です。さらに、代数 $B\cap B'$ は K 上の有限次数の半単純可換代数です。 Bの共通中心と$B'$です。

b) B が単純であると仮定します。従って、$B'$ は単純であり、等式が成り立ちます。

$$
[A : B']_s= [B : K],[A : B]_s= [B': K],[A : K] = [B : K][B': K]
$$

(左次数 $[A : B]_s.$の定義については、VIII、p. 124、定義2を参照してください)

K-代数 $A^o$ は中央のシンプルで、K-代数 B は半単純と有限次数です。 系により、VIII、p. 221、代数 $C = B\otimes_KA^o$ の 1 は半単純になります。 M を、A と同じ加法群と、A の $a, a'$ と B の $b$ に対して公式 $(b\otimes a)a'=ba'a$ によって与えられる外部法則を持つ C モジュールとします。 $u$をEnd$_{\mathbf{Z}}(A)$の元とします。 次に、C モジュール M の $u$ 属するから交換子環 $C'_M$ は、$u$ が右 A 線形で左 B 線形である場合に限り、他の語では、$u$ 属するから交換子環である場合に限り、 A-加群 $A_s$ の相似関係の環における $B_M$。 We consequently define an isomorphism $\gamma$ from $B'$ to $C'_M$ by the relation $\gamma (b')(x) =b'x$ for $b'$ in $B'$ and $x$ in M. ここで、環 C は半単純で、C モジュール M は A の元 1 によって生成されます。 VIII、p. 139、環の命題 6 により、$C'_M$ は半単純なので、代数 $B'$ は半単純になります。

$\varphi$ を $A\otimes_KA^o$ から End$_K(M)$ までの K-代数準同型とし、$a\otimes a'$ を K-線型写像 $x\mapsto axa'$ M から M に送信します。 K-代数 A と $A^o$ は中心単純であるため、$A\otimes_KA^o$ の両側イデアルは 0 と $A\otimes_KA^o$ (VIII、p. 218、系) のみです。 $C_M=\varphi (B\otimes A^o)$ と $C'_M=\varphi (B'\otimes K)$ があります。 準同型 $\varphi$ は零ではありません。従って、それは単射的です。 環 C は半単純なので、VIII, p. 139 の命題 5 により $C''_M= C_M$ が得られます。 従って、$A\otimes_KA^o$ の部分代数 $B\otimes_KA^o$ は、部分代数 $B'\otimes_KK$ の交換子環になります。 従って、$A\otimes_KK$の$B'\otimes_KK$の交換子環は、II, §7, No. 9、p. 311の命題19により$(B\otimes_KA^o)\cap (A\otimes_KK)$、つまり$B\otimes K$と等しくなります。 従って、A の $B'$ の交換子環は B に等しいです。 代数 $L = B\cap B'$ は B の中心です。 B は K 上の有限次数の半単純代数であるため、代数 L は可換であり、半単純で K 上の有限次数を持ちます。 BはAの$B'$の交換子環なので、$B'$の中心も$L = B\cap B'$(VIII、p. 77)に等しい。 私たちは a) を証明しました。

ここで、代数 B が単純であると仮定します。 系 VIII、p. 222、環 C の 2 つまでは簡単です。 VIII の命題 4 により、p. 123 は C 加群 M に適用されます。その交換子環は $B'$ と同型で、環 $B'$ は単純で、M は次の $B'$ 加群です有限長。他の語では、$B'$は単純な環Aの単純な部分環であり、左の次数$[A : B']_s$は整数$m\geqslant 1$です。左の$B'$加群として見ると、A は有限の基底 $(a_1, . . . , a_m)$ を持ちます。さらに (上記参照)、C から $C''_M=$ までの $_{B'}$(A) までの制限同型による $\varphi$ 誘導する、および C から $A^m$ までの写像 $c\mapsto (ca_1, . . . , ca_m)$ は、したがって客観的です。従って、C は、次元 $m$ の無料の右A-加群です。今、$C = B\otimes A^o$ があるので、C は次元のフリーの右A-加群 [B : K] です。従って、$[A : B']_s=m= [B : K]$となります。 VIII、p. 125 の命題 6 から、

$$
[A : K] = [A : B']_s[B': K] = [B : K] [B': K]
$$

私たちも持っているので

$$
[A : K] = [A : B]_s[B : K]
$$

[B : K] は有限であり、非零、等式 $[A : B]_s= [B': K] ($集合理論、III, §6, No. 3、p. 188、系があることを結論するとします 3)。 b)を証明しました。

A を有限次数の中心単純K-代数とします。 満たす $[A : K]\not=$ $[B : K] [B': K]$ の半単純可換部分代数 B (VIII の練習問題 1、p. 269) が存在する可能性があります。

#### 定理 6 {#alg-viii-s14-thm-6 .statement tag=00GZ}

Aを中心単純K-代数、Bを有限次数のAの部分代数、そして$B'$をAの交換子環とします。

a) B が中心単純であると仮定します。この場合、$B'$ は中央単純であり、$b\otimes b'$ を $bb'$ に送信する K-代数準同型 $\theta : B\otimes_KB'\rightarrow A$ は同型です。

b) B が半単純であると仮定し、$L = B\cap B'$ とします。 すると、$B'$は半単純代数になります。 The commutant $L'$ of L in A is a semisimple ring with center L, and the ring homomorphism $\psi : B\otimes_LB'\rightarrow L'$ that sends $b\otimes b'$ to $bb'$ is an isomorphism.

a)を証明しましょう。 B が中心単純である場合、$B'$ は、VIII、p. 259 の定理 5 によって中心単純になります。従って、K-代数 $B\otimes_KB'$ は単純 (VIII、p. 222、系 2) であり、準同型 $\theta : B\otimes_KB'\rightarrow A$ は単射です。さて、$[A : B']_s$ の等式と [B : K] (定理 5) により、左側の $B'$ モジュール $B\otimes_KB'$ と A は同じ有限次元から解放されます。従って、それらは同じ有限長の $B'$ モジュールです。 系 2/II, §1, No. 10 著、p. $213,\theta$は全単射です。

b)を証明しましょう。 定理 5 により、代数 L は K 上の有限次数と半単純の可換です。ロケ地にて。引用。 L に適用すると、A の交換子環 $L'$ は半単純代数で、L は A の $L'$ の交換子環であるため、L は $L'$ の中心になります。 L は半単純環 $L', B$ と $B'$ の中心であるため、単純な環 $L'_i$ ($i\in I$ の場合) の有限積を使用して同一視できる $L'$ を計算すると、次のようになります。

$$
L =\prod_{i\in I}L_i,B =\prod_{i\in I}B_i,B'=\prod_{i\in I}B'_i
$$

ここで、$L_i$ は $L'_i$ の中心であり、$B_i$ と $B'_i$ は $L'_i$ の部分代数であり、$L'_i$ の中心 $L_i$ はお互いの交換子環です。私たちは$L'_i$を可換体$L_i$の上の中心単純代数として、$B_i$を有限次数の中心の単純な$L_i$-代数として見ます。 主張 a) により、$b_i\otimes b'_i$ を $b_ib'_i$ に送信する標準写像 $\psi_i: B_i\otimes_{L_i}B'_i\rightarrow L'_i$ は、環同型になります。さて、同一視できる $B\otimes_LB'$ と $\prod_{i\in I}(B_i\otimes_{L_i}B'_i)$ なので、$\psi$ は写像 $(\psi_i)_{i\in I}$ の家族の積になります。従って、$\psi$ は環同型となります。

#### 系 {#alg-viii-s14-n5-cor-1 .statement tag=00H0}

体 K が代数的に閉じており、A が K 上の有限次数の単純代数であるとします。B を A の単純部分代数とし、$B'$ を A における B の交換子環とします。そのとき、$B'$ は単純K-代数、B は交換子環です。 $B'$、$[A : K] = [B : K][B': K]$があり、$B\otimes_KB'$からAまでの標準準同型はK-代数同型です。

K 上の有限次数のすべての単純代数が中心であるため、定理 5 と 6 から系が続きます。

### 6. 最大可換部分代数

K-代数 A の部分代数が、A の可換部分代数の集合の極大元である場合、A の最大可換部分代数であると言います。

#### 補題 3 {#alg-viii-s14-lem-3 .statement tag=00H1}

A を A の K-代数と L 部分代数とします。

a) 代数 L は、L が A の交換子環 $L'$ に等しい場合に限り、A の最大値可換部分代数になります。

b) $K'$ を非零可換K-代数とします。この場合、$L_{(K')}$ が $A_{(K')}$ の最大可換部分代数である場合に限り、L は A の最大可換部分代数になります。

a)を証明しましょう。まず、L が $L'$ と等しいと仮定します。この場合、L は可換です。 M が含む L の可換部分代数である場合、L の $x$ と M の $y$ には $xy=yx$ があり、従って $M\subset L'$ となり、M = L となります。従って、L は A の最大値可換部分代数になります。

逆に、L が A の最大値可換部分代数であると仮定し、$x$ を $L'$ の元とします。 $L\cup  \{x\}$ によって生成された A の部分代数 M は可換であり、含む L です。 L が最大であるため、M = L となり、$x\in L$、最後に $L = L'$ となり、a) が得られます。

By Proposition 6 of III, §4, No. 4, p. 468, the commutant of $L_{(K')}$ in $A_{(K')}$ is $L'_{(K')}$. Since the equalities $L = L'$ and $L_{(K')}= L'_{(K')}$ are equivalent (II, §7, No. 9, p. 311, Proposition 19), assertion b) follows from a).

#### 命題 3 {#alg-viii-s14-prop-3 .statement tag=00H2}

A を有限次数の中心単純K-代数とし、L を A の半単純可換部分代数とします。以下のプロパティは同等です。

(i) 代数 L は A の最大値可換部分代数です。

(ii) 左側のL-モジュール A は、次元 [L : K] の空きです。

(iii) $[A : K] = [L : K]^2$ があります。

さらに、A が代数 End$_K(V)$ であり、V が K 上の非零有限次元のベクトル空間であると仮定します。その場合、前のプロパティも次と等価です。

(iv) V は、次元 1 の無料の L モジュールです。

A) A が形 End$_K$(V) であると仮定します。ここで、V は体 K 上の非零有限次元のベクトル空間です。 図式に続き、条件 (i) から (iv) の同値を確立します。

(i) $=\Rightarrow$ (iv) $=\Rightarrow$ (ii) $=\Rightarrow$ (iii) $=\Rightarrow$ (i) 。

Since L is a semisimple commutative algebra of finite degree over K, we can identify it with a finite product $\prod_{i\in I}L_i$ of extensions of K of finite degree (VIII, p. 137, Proposition 3). すべての $i\in I$ について、$V_i$ を L モジュール V の型 $L_i$ の同型成分とします。 V は忠実な L モジュール (VIII、p. 144、系) であるため、$L_i$ よりも非零有限次元のベクトル空間です。 次に、$\prod_{i\in I}V_i$ を使用して同一視する V を実行できます。 これらの条件、A の L の交換子環 $L'$、つまり単に代数 End$_L$(V) は、積 $\prod_{i\in I}$ End$_{L_i}(V_i)$ で識別できます。

L が End$_K(V)$ の最大値可換部分代数であるとします。 補題 3, a) までに、$L = L'$ があるので、$L'$ は可換であり、$i\in I$ ごとに dim$_{L_i}(V_i) = 1$ が得られます。従って、(i) は (iv) を意味します。

L モジュール V に次元 1 が含まれていないとします。 $(e_1, . . . , e_r)$ を K 上の V の基底とします。 写像 $a\mapsto (ae_1, . . . , ae_r)$ は左A-加群の同型であるため、 L - A から $V^r$ までのモジュール。その結果、A は次元 $r$ の空き左 L 加群となり、$r=$ dim$_K(V) = [L : K]$ が得られます。従って、(iv) は (ii) を意味します。

(i) が (iii) を意味することは明らかです。

最後に、$[A : K] = [L : K]^2$、他の語、dim$_K(V) = [L : K]$ があるとします。次に、$\sum_i$ dim$_{L_i}(V_i)[L_i: K] =\sum_i[L_i: K]$ があるため、$V_i$ は $i$ ごとに $L_i$ に 1 を超える次元が含まれます。次に、$i$ ごとに End$_{L_i}(V_i) = L_i$ があり、従って $L'= L$ になります。 補題 3、a) により、L は A の最大値可換部分代数です。従って、(iii) は (i) を意味します。

B) 一般的なケースを続けましょう。 VIII, p. 252 の定理 1 により、$K'$-代数 $A_{(K')}$ が代数 End$_{K'}(V')$ と同型となるように、有限次数の K の分離拡大 $K'$ が存在します。 $V'$ は、非零有限次元の $K'$ のベクトル空間です。すると、$K'$-代数 $L_{(K')}$ は可換であり、 半単純 (VIII, p. 222, 系 2) となります。 証明の最初の部分までに、次のプロパティは同等になります。

(i$'$) 代数 $L_{(K')}$ は、$A_{(K')}$ の最大可換部分代数です。

(ii$'$) 次元 $[L_{(K')}: K']$ の左側の $L_{(K')}$ モジュール $A_{(K')}$ は空いています。

(iii$'$) $[A_{(K')}: K'] = [L_{(K')}: K']^2$ があります。

補題 3、b) により、性質 (i) と (i’) は同等です。

集合 $n= [L : K]$;次に$n= [L_{(K')}: K']$。 性質 (ii) は、左側の L モジュール A と $L^n$ が同型であることを意味します。 VIII、p. 37 の定理 3 により、これは、$L_{(K')}$ 加群 $A_{(K')}$ と $(L_{(K')})^n$ が同型であることに相当します。 (ii)と(ii$'$)の同値が続きます。

最後に、$[A : K] = [A_{(K')}: K']$ と $[L : K] = [L_{(K')}: K']$ があり、同値のプロパティ (iii) と (iii$'$) が得られます。これで、性質 (i)、(ii)、(iii) の同値が証明されました。

#### 系 {#alg-viii-s14-n6-cor-1 .statement tag=00H3}

A を K 上の有限次数の中心単純代数とし、L を半単純可換K-代数とし、[A : K] が $[L : K]^2$ に等しくなるようにします。 LからAまで$f$と$g$を単射準同型とします。$g=\theta \circ f$となるようなAの内部自己同型$\theta$が存在します。

集合 $n= [L : K]$。 部分環 $f$(L) よりも左加群として見ると、A は次元 $n$ から解放されます。これは、命題 3 のプロパティ (ii) と (iii) の同値から続きます。 $f$ は L から $f$(L) までの同型であるため、左側の L モジュール $A^f$ (その作用の法則は $(x, a)\mapsto f(x)a$ によって与えられます) は次元 $n$ から解放されます。同じことが$A^g$にも当てはまり、従って$A^f$と同型です。私たちは、命題 1 (VIII、p. 257) のプロパティ (i) と (ii) のを用いて結論する同値を定義します。

A が K 上の有限次数の中心単純代数であると仮定します。 A の半単純ではなく、$[A : K]\not= [L : K]^2$ (VIII、p. 270、練習問題 5) ではない最大可換部分代数 L が存在する可能性があります。

### 7. 極大エタール部分代数

#### 補題 4 {#alg-viii-s14-lem-4 .statement tag=00H4}

A を、K とは異なる、K 上の有限次数の中心単純代数とします。K とは異なる A のエタール (V, §6, No. 3, p. 28, 定義 1) 部分代数が存在します。

ウェダーバーンの定理 (VIII, p. 120, 定理 1) により、A は形 $\mathbf{M}_n$(D) であると仮定できます。ここで、$n$ は厳密には正の整数であり、D 体は中心 K です。

$n >1$ と仮定します。 K にエントリを持つ対角線行列の代数は、K とは異なる A のエタール部分代数です。

$n= 1$ と仮定します。 $p$ を D の特性指数とします。 VIII、p. 230 の補題 1 により、$a^{p^m}$ がどの自然数についても K に対して属するとならないような D の元 $a$ が存在します。 $m$。従って、$m$ 十分大きい、元 $x=a^{p^m}$ は K 上で分離可能 (V, §7, No. 7、p. 44、命題 13) ですが、属するは K に対して分離できません。A の部分代数 $K(x)$ は次のようになります。 有限次数の体 K の分離拡大なので、K よりもエタール部分代数です。 Kとは別物です。

#### 命題 4 {#alg-viii-s14-prop-4 .statement tag=00H5}

A を K 上の有限次数の中心単純代数とします。 L を A の部分代数とし、$L'$ を A の L の交換子環とします。

a) A の半単純可換部分代数の中で L が最大である場合、$L = L'$ があり、L は A の最大可換部分代数です。

b) L が A のエタール部分代数の中で最大である場合、$L = L'$ があり、L は A の最大可換部分代数です。

関係 $L = L'$ は、L が A (VIII, p. 261, 補題 3, a)) の最大値可換部分代数であることを意味します。 L が半単純であり、可換であり、$L'$ とは異なるものであるとします。 VIIIの定理5までに、p. 259$, L'$は半単純、Lは$L'$の交換子環、従って$L'$の中心になります。従って、$L'$ は可換ではありません。 L および含む L とは異なる A の M 半単純可換部分代数が存在し、L がエターレである場合、それはエターレであることを証明すれば十分です。

半単純環 (VIII, p. 135, 定理 1) に対する構造定理により、$L'$ から $B_1\times  \cdots  \times B_r$ までの単純な環 $B_1, . . . ,B_r$ と同型 $\varphi$ が存在します。 $1\leqslant i\leqslant r$ の場合、$B_i$ の中心を $E_i$ で表します。次に、$\varphi (L) = E_1\times  \cdots  \times E_r$ になります。 $L'$ は可換ではないため、たとえば $B_1$ は可換ではないと仮定できます。従って、$B_1\not= E_1$ があり、補題 4 までに、$E_1$ とは異なり、$E_1$ を超える可換である $B_1$ の部分代数 $M_1$ が存在します。 集合 $M =\varphi^{-1}(M_1\times E_2\times  \cdots  \times E_r)$;それは含む L の半単純可換部分代数であり、L とは異なります。 L が K 上のエタールであると仮定します。 M がエタールであることを証明しましょう。 K の拡大 $E_i$ は分離可能です (V, §6, No. 4、p. 30、命題 3)。 さらに、$E_1$代数$M_1$とK-代数$E_1$はエタールであるため、K-代数$M_1$もエタールです(V, §6, No. 5,p. 32,系2)。 従って、K-代数 $M_1\times E_2\times  \cdots  \times E_r$ はエタールであり、従って M も同様です。

A を K 上の有限次数の中心単純代数とします。 A の半単純可換部分代数の中で最大である A の部分代数を A の最大半単純可換部分代数と呼びます。 命題 4、項 「最大」とは、 性質が可換であること、または半単純で可換であること。 Aのエタール部分代数のうち最大となるAの部分代数をAの極大エタール部分代数と呼びます。

#### 系 1 {#alg-viii-s14-prop-4-cor-1 .statement tag=00H6}

A を有限次数の中心単純K-代数とします。 A のすべての半単純 (それぞれエタール) 可換部分代数は、A の最大可換部分代数、つまり半単純 (それぞれエタール) に含まれます。

#### 系 2 {#alg-viii-s14-prop-4-cor-2 .statement tag=00H7}

D を中心 K で K を超える有限次数の体とします。

a) D の最大可換部分体は、D の最大可換部分代数であり、また D の最大半単純可換部分代数です。D のすべての可換部分体 L は最大可換部分体に含まれます。

b) L を、K の分離拡大である D の可換部分体とする。それは、K の分離拡大である D の最大可換部分体に含まれています。

c) L を D の可換部分体とします。すると、$[D : K] = [L : K]^2$ がある場合に限り、L は D の最大可換部分体になります。

D の部分代数は体 (V, §2, No. 2、p. 10、命題 1) であるため、半単純です。 さらに、D含むKの最大可換部分体。 主張 a) と b) から、系 1 と主張 c) の命題 3 (VIII、p. 262) が続きます。

#### 命題 5 {#alg-viii-s14-prop-5 .statement tag=00H8}

A を K 上の有限次数の中心単純代数とします。B を A の半単純部分代数とし、$B'$ を B の交換子環とします。

a) 代数 B 含む B 含む $B'$ の場合に限り、A の最大半単純可換部分代数。

b) B 含む $B'$ とし、B から A までの$g$ を K-代数準同型とします。B に$g$ を持つ一致するである A の内部自己同型 $\theta$ が存在します。

L を A の最大値可換部分代数とします。 VIII、p. 261、L の補題 3 は、A の交換子環 $L'$ に等しい。B 含む L の場合、その交換子環 $B'$ は $L'$ に含まれるため、B に含まれる。

逆に、Bに$B'$が含まれているとします。 すると、$B'$はBの中心で、半単純可換代数(VIII、p. 137、命題2)となります。 系 1 までに、含む $B'$ の最大値半単純可換部分代数 L が存在します。 The commutant of L is L (VIII, p. 261, Lemma 3, a)), and that of $B'$ is equal to B (VIII, p. 259, Theorem 5). したがって、関係 $L\supset B'$ は $L\subset B$ を意味します。 私たちは a) を証明しました。

b)を証明しましょう。 a)によって存在する、Bに含まれるAの最大値半単純可換部分代数LをB含む$B'$、選ぶとする。 BからAまでの$g$を準同型とします。VIII、p. 262の3つ命題により、等式$[A : K] = [L : K]^2$が得られます。 VIII, p. 263の系により、Lに$g$を持つ一致するであるAの内部自己同型$\theta_1$が存在します。 $f$がBの標準単射をAにすると、$B'$はLに含まれるため、準同型$g$と$\theta_1\circ f$はBの制限から中心$B'$と同じになります。 VIII, p. 256 の定理 2 により、$g=\theta \circ f$ となる A の内部自己同型 $\theta$ が存在します。他には語、$\theta$、拡大する、$g$。

### 8. 単純代数中対角化可能部分代数

D を体である K-代数とし、V を D 上の有限次元右ベクトル空間とします。 L を、対角化可能な K-代数 (V, §6, No. 3, p. 28) である End$_D(V)$ の K-部分代数とします。 定義までに、L は K 上に有限次数を持ち、K 上に以下の特性を持つ L の基底 $(\varepsilon_i)_{i\in I}$ が存在します。

$i\not=j ,\sum_{i\in I}\varepsilon_i= 1$の場合は$\varepsilon^2_i=\varepsilon_i, \varepsilon_i\varepsilon_j= 0$。

I の $i$ ごとに集合 $V_i=\varepsilon_i(V)$。この場合、$(V_i)_{i\in I}$ は、直和 V (II, §1, No. 8、p. 209、命題 12) を含む V の非零線形部分空間の族になります。 $u$ を V の自己準同型とします。次に、$u$ 属するから L は、$i\in I$ ごとに、$x\in V_i$ ごとに $u(x) =\lambda_ix$ となるような K の元 $\lambda_i$ が存在する場合に限ります。

逆に、V が非零線形部分空間の族 $(V_i)_{i\in I}$ の直和であるとします。 $K^I$ の任意の元 $\boldsymbol{\lambda }= (\lambda_i)_{i\in I}$ については、$x\in V_i$ に対して $u_{\boldsymbol{\lambda }}(x) =\lambda_ix$ となるように、D-ベクトル空間 V の $u_{\boldsymbol{\lambda }}$ 自己準同型で表します。 The set L of endomorphisms $u_{\boldsymbol{\lambda }}$ for $\boldsymbol{\lambda }\in K^I$ is a diagonalizable subalgebra of End$_D(V)$ having the family $(\varepsilon_i)_{i\in I}$ as basis, where $\varepsilon_i$ is the projector with image $V_i$ and kernel $\sum_{j\not=i}V_j$. L は、直和分解 $V =\oplus_{i\in I}V_i$ に関連付けられた End$_D(V)$ の対角化可能部分代数であると言います。 [L : K] = カード(I) $\leqslant$ dim$_D(V)$ があります。

#### 命題 6 {#alg-viii-s14-prop-6 .statement tag=00H9}

L を、直和分解 $V =\oplus_{i\in I}V_i$ に関連付けられた End$_D(V)$ の対角化可能部分代数とします。

a) 代数 L は、すべての $V_i$ が D 上に次元 1 を持っている場合に限り、K-代数 End$_D(V)$ の対角化可能部分代数の中で最大になります。

b) 代数 L は、D = K で、すべての $V_i$ が K を超える次元 1 を持つ場合に限り、End$_D(V)$ の最大可換部分代数です。

すべてのベクトル空間 $V_i$ に D 上の次元 1 がある場合、次のようになります。

[L : K] = カード(I) = 暗$_D(V)$,

従って、L は End$_D(V)$ の対角化可能部分代数の中で最大です。 逆の場合、$_D(V_j)\geqslant 2$ が薄くなるような添字 $j\in I$ が存在します。 選ぶ 2 つの非零リニア部分空間 $V'_j$ と $V_j$ の $V''_j$ と直和 $V_j$。 The diagonalizable subalgebra of End$_D(V)$ associated with the direct sum decomposition $V = (\oplus_{i\in I-\{j\}}V_i)\oplus V'_j\oplus V''_j$ contains L and is not equal to L; assertion a) follows.

End$_D(V)$のLの交換子環$L'$は、形$(x_i)\mapsto (u_i(x_i))$の自己準同型と、$(u_i)\in \prod_{i\in I}$End$_D(V_i)$で構成されています。 代数 L は、$L = L'$ (VIII, p. 261, 補題 3, a)) がある場合に限り、End$_D(V)$ の最大可換部分代数です。従って、この関係は、「$i\in$ I ごとに終了$_D(V_i) = K$」に相当します。 主張 b) が続きます。

#### 命題 7 {#alg-viii-s14-prop-7 .statement tag=00HA}

L を K 上の有限次数の可換代数とします。次のプロパティは同等です。

(i) 代数 L はエターレです。

(ii) Kを対角化した有限次数のKの分離拡大が存在します。

含意 (ii)$\Rightarrow$(i) は、V, §6, No. 3、p. 29、命題 2 から導き出されます。

含意 (i)$\Rightarrow$(ii) を証明しましょう。 ΩをKの分離閉包とします。V, §6, No. 7、p. 34の定理4により、Ωに含まれる有限次数のKの拡大$L_1, . . . ,L_n$が存在し、Lは積と同型になります。 $L_1\times  \cdots  \times L_n$。 N を、含むの $L_i$ (V, §10, No. 1, p. 58) である K のガロア拡大とし、$L_{(N)}$ が対角化可能であることを証明しましょう。原始元定理 (V, §7, No. 4, p. 40, 定理 1) により、$i\in [1, n]$ ごとに、$L_i$ が $K[X]/(P_i)$ と同型となるような既約分離多項式 $P_i\in K[X]$ が存在します。 N は、$P_i$ が根を許容する K の正規拡大なので、N[X] の多項式 $P_i$ 分裂は単純な根です。従って、$N[X]/(P_i)$ と同型の N-代数 $L_{i(N)}$ は、$N^{[L_i:K]}$ と同型です。従って、$L_{(N)}$ は対角化可能です。

#### 定理 7 {#alg-viii-s14-thm-7 .statement tag=00HB}

A を有限次数の中心単純K-代数および A の L 部分代数とします。以下のプロパティは同等です。

(i) 代数 L は A の極大エタール部分代数です。

(ii) 対角行列の$L_{(K')}$～集合を送る$A_{(K')}$から$\mathbf{M}_n(K')$まで、Kの拡大$K'$、整数$n\geqslant 1$、同型$\theta$が存在します。

(iii) (ii) と同様に $K',n$ と $\theta$ が存在します。ここで、拡大 $K'$ はガロアと仮定され、有限次数です。

(iii) が (ii) を意味することは明らかです。

性質 (ii) が成り立つ場合、$L_{(K')}$ は $A_{(K')}$ (命題 6) の最大可換部分代数であり、対角化可能です。 K-代数 L はエタール (V, §6, No. 3, p. 28, 定義 1) であり、A (VIII, p. 261, 補題 3, b)) の最大値可換部分代数です。 (ii) が (i) を意味することを証明しました。

性質 (i) が成り立つとします。 L は K 上のエタールなので、命題 7 により、$K_1$-代数 $L_{(K_1)}$ が対角化できるように、有限次数の K のガロア拡大 $K_1$ が存在します。 The algebra A is central simple; by (VIII, p. 252, Theorem 1), there exist a Galois extension $K_2$, a vector space V of finite dimension $n$ over $K_2$, and an isomorphism $\theta$ from $A_{(K_2)}$ to End$_{K_2}(V)$. V、p. 55 の命題 1 までに、$K_1= K_2$ と仮定できます。 命題 4、b) VIII、p. 264、補題 3、b) VIII により、p. 261$, L_{(K')}$ は $A_{(K')}$ の最大値可換部分代数であるため、$\theta (L_{(K')})$ は最大値です可換部分代数の終わり$_{K'}(V')$。 Let us apply Proposition 6 to the diagonalizable algebra $\theta (L_{(K')}):$ there exists a basis $(e_1, . . . , e_n)$ of $V'$ over $K'$ such that $\theta (L_{(K')})$ consists of the endomorphisms of $V'$ with diagonal matrix with respect to this basis. したがって、(i) は (iii) を意味します。

### 練習問題 {#alg-viii-s14-exercises}

[§ 14 に対して練習問題](exercises/s14/)を参照してください。
