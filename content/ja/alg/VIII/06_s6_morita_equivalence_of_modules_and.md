---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 6
section_title: Morita Equivalence of Modules and Algebras
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.95-A VIII.117
pdf_pages: 0112-0134
extraction: native+ocr
subsections:
    - "no": 1
      title: Commutant and Duality
      page: 95
      pdf_page: 112
    - "no": 2
      title: Generating Modules and Finitely Generated Projective Modules
      page: 98
      pdf_page: 115
    - "no": 3
      title: Invertible Bimodules and Morita Equivalence
      page: 100
      pdf_page: 117
    - "no": 4
      title: The Morita Correspondence of Modules
      page: 103
      pdf_page: 120
    - "no": 5
      title: Ordered Sets of Submodules
      page: 106
      pdf_page: 123
    - "no": 6
      title: Other Properties Preserved by the Morita Correspondence
      page: 109
      pdf_page: 126
    - "no": 7
      title: Morita Equivalence of Algebras
      page: 111
      pdf_page: 128
statements: 40
exercises: 8
content_sha256: 5fc8becc585e7c5cf1d2e35305f12489284294d0cbde8ffab672475a3e8ed24f
translated_from: content/en/alg/VIII/06_s6_morita_equivalence_of_modules_and.md
translation_method: google
source_content_sha256: e8ef2b43442fbc25b56375b83b63be74c37d7c8014a9723fb60c9bc369cd90cb
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 599212e4a0b39ecdf516f5cb7bd651cd834a62cac419069f732ed4e83d8aa21f
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 6。森田加群と代数の同値

この切断において、$k$は可換環を表します。

### 1. 可換子環と双対性

A と B を$k$-代数とする。 (III, §4, No. 3, p. 466) 代数 A と B 上の両側加群は、A と B-加群構造一致するから推定される 2 つの $k$ 加群構造が含まれる $(A$, B) 双加群 P であることを思い出してください。曖昧さを避けるために、P は $(A,B)_k$-bimodule であると言います。 P を $(A,B)_k$-bimodule とする。 $P^*$ によって、左A-加群の基礎となる P の二重 Hom$_A(P,A)$ を表します。これは、$(B,A)_k$ 双モジュール (II, §1, No. 14、p. 226) です。 $a\in A$、$b\in B,x\in P$、$x^*\in P^*$ については、

$$
\langle x, bx^*a\rangle =\langle xb, x^*\rangle a \tag{1}
$$

$_sA_d$ で、$(A,A)_k$-双加群 (上記引用) とみなされる代数 A を、$\Lambda  : P\otimes_BP^*\rightarrow_sA_d$ で次のように決定される $(A,A)_k$-双加群の準同型性を表します。

$$
\Lambda (x\otimes x^*) =\langle x, x^*\rangle \tag{2}
$$

$x\in P$ と $x^*\in P^*$ の場合。 P の基礎となる右B-加群の二重 Hom$_B(P,B)$ を $\widetilde{P}$ で表します。それは$(B,A)_k$-バイモジュールです。 (3) $\widetilde{\Lambda}(\widetilde{x}\otimes x) =\langle \widetilde{x}, x\rangle$ によって決定される $(B,B)_k$-bimodules の $\widetilde{\Lambda} :\widetilde{P}\otimes_AP\rightarrow_sB_d$ 準同型で表します

$x\in P$ と $\widetilde{x}\in \widetilde{P}$ の場合。

ここで、マッピング $b\mapsto b_P$ が B から End$_A(P)$ への全単射であると仮定します。したがって、B から End$_A(P)$ の逆の代数への同型写像になります。 $P^*\otimes_AP$ から End$_A(P)$ (II, §4, No. 2、p. 271) までの $\mathbf{Z}$ モジュールの標準準同型、その後 $\mathbf{Z}$ モジュールの $\Theta  : P^*\otimes_AP\rightarrow$ B の決定する準同型

$$
x\Theta (x^*\otimes y) =\langle x, x^*\rangle y \tag{4}
$$

$x, y\in P$ と $x^*\in P^*$ の場合。 (1) のため、この準同型は $(B$, B)-線形であり、次のようになります。

$$
\Theta (x^*\otimes y)y^*=x^*\langle y, y^*\rangle \tag{5}
$$

$y\in P$ と $x^*, y^*\in P^*$ の場合。 (4) と (5) から、$(B,B)_k$-bimodule $P^*\otimes_AP:$ で次の等式が導き出されます。

$$
(y^*\otimes x)\Theta (x^*\otimes y) =y^*\otimes  \langle x, x^*\rangle y=y^*\langle x, x^*\rangle  \otimes y= \Theta (y^*\otimes x)(x^*\otimes y)
$$

$x, y\in P$ と $x^*, y^*\in P^*$ の場合、したがって

$$
s\Theta (t) = \Theta (s)t \tag{6}
$$

$s, t\in P^*\otimes_AP$の場合。同様に、P の $x, y$ と $P^*$ の $x^*, y^*$ について、(4) と (5) から $(A,A)_k$-bimodule $P\otimes_BP^*$ で次の等式を推定します。

$$
(x\otimes x^*)\langle y, y^*\rangle =x\otimes \Theta (x^*\otimes y)y^*=x\Theta (x^*\otimes y)\otimes y^*=\langle x, x^*\rangle (y\otimes y^*)
$$

したがって

$$
u\Lambda (v) = \Lambda (u)v \tag{7}
$$

$u, v\in P\otimes_BP^*$の場合。

$P^*$ の任意の元 $x^*$ について、B-線型写像 $x\mapsto \Theta (x^*\otimes x)$ を P から B まで $\sigma (x^*)$ で表します。したがって、$P^*$ から $\widetilde{P}$ まで定義する写像 $\sigma$、つまり $(B$、A)-線形であり、定義によって、

$$
\Theta (x^*\otimes y) =\langle \sigma (x^*), y\rangle \tag{8}
$$

$x^*\in P^*$ と $y\in P$ 用。したがって、$\widetilde{\Lambda}$の定義までに、

$$
\Theta  =\widetilde{\Lambda}\circ (\sigma \otimes 1_P) \tag{9}
$$

A から End $_B(P)$ までの写像 $a\mapsto a_P$ が全単射であると仮定します。そのときは代数同型です。同様に、$(A,A)_k$-bimodules $\widetilde{\Theta} : P\otimes_B\widetilde{P}\rightarrow_sA_d$ の定義する準同型を設定で計算します。

$$
\widetilde{\Theta}(x\otimes \widetilde{y})y=x\langle \widetilde{y}, y\rangle \tag{10}
$$

$x, y\in P$と$\widetilde{y}\in \widetilde{P}$の場合。また、設定による $(B,A)_k$-bimodules $\widetilde{\sigma}:\widetilde{P}\rightarrow P^*$ の定義する準同型

$$
\widetilde{\Theta}(x\otimes \widetilde{y}) =\langle x,\widetilde{\sigma}(\widetilde{y})\rangle \tag{11}
$$

$x\in P,\widetilde{y}\in \widetilde{P}$の場合。私たちは持っています

$$
\widetilde{\Theta} = \Lambda \circ (1_P\otimes \widetilde{\sigma}) \tag{12}
$$

#### 命題 1 {#alg-viii-s6-prop-1 .statement tag=006R}

写像 $b\mapsto b_P$ B から End$_A(P)$ と $a\mapsto a_P$ A から End$_B(P)$ が全単射であるとします。すると、$\sigma$ と $\widetilde{\sigma}$ は逆同型となり、関係となります。

$$
\Lambda  =\widetilde{\Theta}\circ (1_P\otimes \sigma ) \tag{13}
$$

$$
\widetilde{\Lambda} = \Theta \circ (\widetilde{\sigma}\otimes 1_P) \tag{14}
$$

$x\in P,x^*\in P^*$ および $y\in P$ については、関係 (4)、(8)、(10)、および (11) により、次のようになります。

$$
(15)\langle x, x^*\rangle y=x\Theta (x^*\otimes y) =x\langle \sigma (x^*), y\rangle =\widetilde{\Theta}(x\otimes \sigma (x^*))y=\langle x,\widetilde{\sigma}(\sigma (x^*))\rangle y
$$

同様に、$x\in P,\widetilde{y}\in \widetilde{P}$ と $y\in P$ については、

$$
x\langle \widetilde{y}, y\rangle =\widetilde{\Theta}(x\otimes \widetilde{y})y=\langle x,\widetilde{\sigma}(\widetilde{y})\rangle y=x\Theta  (\widetilde{\sigma}(\widetilde{y})\otimes y) =x\langle \sigma (\widetilde{\sigma}(\widetilde{y})), y\rangle \tag{16}
$$

仮定のため、P は A-加群と B-加群として忠実です。 関係 (15) と (16) から、それぞれ $\widetilde{\sigma}\circ \sigma = 1_{P^*}$ と $\sigma \circ \widetilde{\sigma}=$ $1_{\widetilde{P}}$ が導き出されます。 関係 (13) と (14) は、それぞれ (12) と (9) から続きます。

#### 注意 1 {#alg-viii-s6-n1-rem-1 .statement tag=006S}

B から End $_A(P)$ までの写像 $b\mapsto b_P$ が全単射であるとします。それから

a) B-加群 P は P の対加群と識別できます。したがって、それは忠実でバランスが取れています。

b) A から終わりまでの写像 $a\mapsto a_P$ $_B(P)$ は、A-加群 P が忠実でバランスが取れている場合に限り、全単射となります。

#### 注意 2 {#alg-viii-s6-n1-rem-2 .statement tag=006T}

命題 1 の仮定では、A-加群 P はバランスが取れています。 環 $A_P$ と $A'_P$ は同じ中心 (VIII, p. 77) なので、環 A の中心 Z(A) から同型 $\varphi$ が存在します。 中心 Z(B) の環 B、$z\in Z(A)$ の関係 $\varphi (z)_P=z_P$ によって決定されます。さらに、$(A,B)_k$-バイモジュール P の自己準同型は、$z$ が Z(A) を通る相似関数 $z_P$ です。 $(A,B)_k$-bimodule P の自己同型は相似関数 $z_P$ で、$z$ は Z(A) で可逆です。

### 2. 生成加群と有限生成射影加群

#### 命題 2 {#alg-viii-s6-prop-2 .statement tag=006U}

A と B を $k$ 以上の代数とし、P を $(A,B)_k$ バイモジュールとします。 B から End$_A(P)$ までの写像 $b\mapsto b_P$ が全単射であるとします。次の主張は同等です。

(i) A-加群 P は射影であり、有限に生成されます。

(ii) 写像 Θ (VIII, p. 96) は、$P^*\otimes_AP$ から $_sB_d$ までの $(B,B)_k$ バイモジュールの同型です。

(iii) Θの像含む単位元 B.

さらに、A から End $_B(P)$ までの写像 $a\mapsto a_P$ が全単射である場合、上記の主張は次の主張と等価です。

(iv) $Q\otimes_AP$ から $_sB_d$ までの $(B,B)_k$ バイモジュールの $(B,A)_k$ バイモジュール Q と全射準同型が存在します。

II, §4, No. 2、p. 271、主張の系により、(i) は (ii) を意味します。また、(ii)から(iii)が導かれます。 $t\in B^*\otimes_AB$ を $\Theta (t) = 1$ とする。 $n$ を整数とし、$(x_1, . . . , x_n)\in P^n$ と $(x^*_1, . . . , x^*_n)\in P^{*n}$ を $t=\sum^n_{i=1}x^*_i\otimes x_i$ とする。 $x$ 所属から P まで、関係 $x\Theta (t) =x$ は次のように書くことができます。

$$
\sum_{i=1}^n\langle x, x^*_i\rangle x_i=x
$$

したがって、A-加群 P は族 $(x_i)_{1\leqslant i\leqslant n}$ によって有限に生成され、II, §2, No. 6、p. 238 の命題 12 を使用して、含意 (iii) $\Rightarrow$ (i) の結論する証明が生成されます。

明らかに (ii) $\Rightarrow$ (iv) があります。 Q を $Q\otimes_AP$ から $_sB_d$ までの $(B,B)_k$-bimodule の $(B,A)_k$-bimodule および $\theta$ 全射準同型とします。前の小節の記法には、$x\in P$ と $y\in Q$ に対して $\theta (y\otimes x) =\langle \zeta (y), x\rangle$ となるような $(B,A)_k$ バイモジュール $\zeta : Q\rightarrow \widetilde{P}$ の準同型が存在し、$\theta =\widetilde{\Lambda}\circ (\zeta \otimes 1_P)$ があります。 $\theta$は全射なので、$\widetilde{\Lambda}$も同様です。 A から End $_B(P)$ までの写像 $a\mapsto a_P$ が全単射である場合、VIII, p. 97 の命題 1 の関係 (14) により Θ は全射です。含意 (iv) $\Rightarrow$ (iii) が続きます。

#### 命題 3 {#alg-viii-s6-prop-3 .statement tag=006V}

A と B を $k$ 上の代数とし、P を $(A,B)_k$-bimodule とします。次のプロパティは同等です。

(i) A-加群 P は生成するです。

(ii) 写像の像 $P\otimes_BP^*$ から $_sA_d$ (VIII、p. 95) 含む単位元。

(iii) $P\otimes_BQ$ から $_sA_d$ までの$(A,A)_k$-bimodules の$(B,A)_k$-bimodule Q と全射準同型が存在します。

さらに、B から End $_A(P)$ までの写像 $b\mapsto b_P$ が全単射である場合、主張は次の主張と等価です。

(iv) 写像 Λ は、$P\otimes_BP^*$ から $_sA_d$ までの同型です。

(i) $\Leftrightarrow$ (ii): Λ の像は、理想的なトレース $\tau (P)$ (VIII、p. 80) です。したがって、(i) と (ii) の同値は、VIII、p. 80 の定理 1 から続きます。

(ii) $\Rightarrow$ (iii): $Q = P^*$ を取れば十分です。

(iii) $\Rightarrow$ (ii): Q を $(B,A)_k$-bimodule および $P\otimes_BQ$ から $_sA_d$ までの $(A,A)_k$-bimodule の $\psi$ 準同型とする。 Q から $P^*$ までの $(B,A)_k$ バイモジュール Ψ の準同型が存在し、$x\in P$ と $y\in Q$ に対して $\psi (x\otimes y) =\langle x,\Psi (y)\rangle$ があり、等式 $\psi = \Lambda \circ (1_P\otimes \Psi )$ があります。 $\psi$ が全射であれば、Λ も全射です。

(iv) が (ii) を意味することは明らかです。逆に、性質 (ii) が成り立ち、B から End$_A(P)$ までの写像 $b\mapsto b_P$ が全単射であるとします。 $e$ を $P\otimes_BP^*$ の元として、$\Lambda (e) = 1$ とします。 VIII、p. 96 の関係 (7) までに、$P\otimes_BP^*$ の $u$ ごとに $u= \Lambda (u)e$ が得られます。 Λ の単射性が続きます。

#### 命題 4 {#alg-viii-s6-prop-4 .statement tag=006W}

A と B を $k$-代数、P を $(A,B)_k$-双加群とする。 B から End $_A(P)$ までの写像 $b\mapsto b_P$ が全単射であるとします。

a) A-加群 P が生成するの場合、右B-加群 P は射影であり、有限に生成されます。

b) A-加群 P が射影で有限生成される場合、右B-加群 P は生成するです。

A-加群 P が生成するであるとします。その場合、忠実かつバランスが取れており (VIII、p. 82、定理 2)、その結果、A から End$_B(P)$ までの写像 $a\mapsto a_P$ は全単射になります (VIII、p. 97、注意 1)。さらに、写像 $\Lambda  : P\otimes_BP^*\rightarrow_sA_d$ は全単射です (VIII, p. 98, 命題 3)。 P を $(B^o,A^o)_k$-bimodule として見ます。 写像 Λ 誘導する全単射写像 $P^*\otimes_{B^o}P\rightarrow A^o$; by 命題 2 of VIII, p. 98, (iv) $\Rightarrow$ (i), 右B-加群 P は射影的で有限生成されます。

ここで、A-加群 P が射影的であり、有限に生成されると仮定します。このとき、写像 $\Theta  : P^*\otimes_AP\rightarrow_sB_d$ は全単射です (前掲書、(i) $\Rightarrow$ (ii))。上記の命題 3 の含意 (iii) $\Rightarrow$ (i) を $(B^o,A^o)_k$-bimodule P に適用すると、右B-加群 P は生成するになります。

#### 系 1 {#alg-viii-s6-prop-4-cor-1 .statement tag=006X}

生成加群の対加群は射影的であり、有限に生成されます。 有限生成射影加群の対加群は生成するです。

A を $k$-代数、M を A-加群とします。 代数 End$_A(M)$ の反対の $k$-代数を B で表します。 系は、$(A,B)_k$-bimodule M に適用された命題 4 から続きます。

#### 系 2 {#alg-viii-s6-prop-4-cor-2 .statement tag=006Y}

A と B を $k$-代数、P を $(A,B)_k$-双加群とする。次のプロパティは同等です。

(i) A-加群 P は生成するで、B から End$_A(P)$ までの写像 $b\mapsto b_P$ は全単射です。

(ii) 右B-加群 P は射影、有限生成、忠実、バランスがとれており、A から End$_B(P)$ までの写像 $a\mapsto a_P$ は全単射です。

含意 (i) $\Rightarrow$ (ii) は、命題 4、a) および注意 1 (VIII、p. 97) から導き出されます。 (ii) が成り立つと仮定します。その場合、A-加群 P は生成する (命題 4、b) が $(B^o,A^o)_k$-bimodule P に適用されます)。 B-加群 P は忠実でバランスが取れているため、(i) の 2 番目の主張も満たされます (VIII、p. 97、注意 1)。

### 3. 可逆双加群と森田同値

#### 定義 1 {#alg-viii-s6-def-1 .statement tag=006Z}

A と B を $k$-代数、P を $(A,B)_k$-双加群とする。 $P\otimes_BQ$ が $_sA_d$ と同型、$Q\otimes_AP$ が $_sB_d$ と同型であるような $(B,A)_k$ 双加群 Q が存在する場合、P は可逆であると言います。このような両側加群 Q は P の逆行列と呼ばれます。

A と B を $k$-代数、P を可逆 $(A,B)_k$-双加群とする。 C を $k$-代数、$P'$ を可逆 $(B,C)_k$-双加群とする。最後に、Q と $Q'$ をそれぞれ P と $P'$ の逆数両側加群とします。 テンソル積 (II, §3, No. 8, p. 258, 命題 8) と II, §3, No. 4, p. 249 の命題 4 の結合性により、$(C,A)_k$-bimodule $Q'\otimes_BQ$ は、 $(A,C)_k$-bimodule $P\otimes_BP'$ なので、$P\otimes_BP'$ は可逆な $(A,C)_k$-bimodule になります。

従って、関係

「A と B は$k$-代数であり、可逆な$(A,B)_k$-双加群が存在する」は同値関係です。

#### 定義 2 {#alg-viii-s6-def-2 .statement tag=0070}

可逆な$(A,B)_k$-双加群が存在する場合、2つの$k$-代数AとBは森田等価と呼ばれます。 $\mathbf{Z}$-代数 A と B が森田等価である場合、環 A と B は森田等価と呼ばれます。

2 つの同型 $k$-代数は森田等価です。 2 つの $k$-代数が森田等価である場合、それらの反対多元環は森田等価です。

P を可逆 $(A, B)_k$-bimodule とし、Q を P の逆数とします。すると、Q は可逆 $(B, A)_k$-bimodule となり、P を逆数とします。さらに、$(B^\circ, A^\circ)_k$-bimodule として見ると、P は可逆であり、その逆としての $(A^\circ, B^\circ)_k$-bimodule Q を持ちます。

#### 補題 1 {#alg-viii-s6-lem-1 .statement tag=0071}

— *A と B を K-代数、P を可逆 $(A, B)_k$ バイモジュール、M と N を B-加群、$u : M \to N$ を B-線型写像とします。 写像 $1_P \otimes u : P \otimes_B M \to P \otimes_B N$ が零 (それぞれ全単射) である場合、u も同様です。*

Q を P の逆数両側加群および $(B, B)_k$ バイモジュールの $\theta : Q \otimes_A P \to {}_s B_d$ 同型とします。 補題は図式の可換性から続きます

$$
\begin{array}{ccc}
Q \otimes_A P \otimes_B M & \xrightarrow{1_Q \otimes 1_P \otimes u} & Q \otimes_A P \otimes_B N \\
\downarrow \theta \otimes 1_M & & \downarrow \theta \otimes 1_M \\
M & \xrightarrow{u} & N.
\end{array}
$$

#### 定理 1 {#alg-viii-s6-thm-1 .statement tag=0072}

*AとBをK-代数、Pを$(A, B)_k$-bimoduleとします。 $(B, A)_k$-bimodule $\operatorname{Hom}_A(P, A_s)$ を $P^*$ で表します。次のプロパティは同等です。

(i) *$(A, B)_k$-bimodule P は反転可能です。*

(ii) *A-加群 P は射影的で有限生成され、B から $\operatorname{End}_A(P)^{\circ}$ までの生成するおよび写像 $b \mapsto b_P$ は K-代数同型です。*

(iii) *右B-加群 P は射影的で有限生成され、A から $\operatorname{End}_B(P)$ までの生成するおよび写像 $a \mapsto a_P$ は K-代数同型です。

これらが性質が成り立つの場合、準同型

$$
\Theta : P^* \otimes P \to {}_s B_d \quad \text{and} \quad \Lambda : P \otimes P^* \to {}_s A_d
$$

は同型であるため、$(B, A)_k$-bimodule $P^*$ は P の逆になります。

性質 (ii) が成り立つ場合、P は逆 $P^*$ (VIII、p. 98、命題 2 および p. 98、命題 3) をもつ可逆 $(A, B)_k$ 双加群です。これは、(ii) が (i) と最後の主張を意味することを証明します。

$(A, B)_k$-bimodule P が可逆であると仮定します。このとき、A-加群 P は生成する (VIII, p. 98, 命題 3, (iii) $\Rightarrow$ (i)) です。従って、忠実でバランスが取れており (VIII、p. 82、定理 2)、その結果、A から $\operatorname{End}_B(P)$ までの写像 $a \mapsto a_p$ は全単射です。

B から $\operatorname{End}_A(P)$ への写像 $b \mapsto b_P$ が全単射であることを証明しましょう。 Q を P の逆の $(B, A)_k$-bimodule とします。$u \in \operatorname{End}_A(P)$ とします。すると、$1_Q \otimes u$ は左B-加群 $Q \otimes_A P$ の自己準同型になります。 $(B, B)_k$-bimodule $Q \otimes_A P$ は $_s B_d$ と同型であるため、$1_Q\otimes u$ がホモテティー となり、右B-加群 $Q\otimes_AP$ の比 $b$ となるような B の一意元 $b$ が存在します。従って、$1_Q\otimes (u-b_P) = 0$ となります。従って、$u=b_P$ by 補題 1;これは、写像 $b\mapsto b_P$ B から End$_A(P)$ が全単射であることを証明します。

VIII、p. 98、A-加群の命題 2 により、P は射影され、有限に生成されます。従って、(i) と (ii) の同値が証明されました。

A と B の役割交換することにより、(i) と (iii) の同値が得られ、これは命題の結論する証明になります。

#### 系 1 {#alg-viii-s6-lem-1-cor-1 .statement tag=077O}

A と B を森田等価$k$-代数とし、P を可逆$(A,B)_k$-双加群とする。 Aの中心Z(A)からBの中心まで$z\in Z(A)$ごとに関係$\varphi (z)_P=z_P$で決まる同型$\varphi$が存在します。 $(A,B)_k$-bimodule P の自己同型は、$z_P$ であり、$z$ は Z(A) の可逆元です。

定理 1 が与えられると、これは VIII、p. 97 の注意 2 から続きます。

#### 系 2 {#alg-viii-s6-lem-1-cor-2 .statement tag=077P}

A と B を森田等価な $k$-代数とし、P を可逆 $(A,B)_k$-双加群とする。 P のすべての $(B,A)_k$-bimodule の逆は、P の双対 $P^*=$ Hom$_A(P,A)$ と同型です。より正確には、Q を P の逆である $(B,A)_k$-bimodule とし、$\lambda : P\otimes_BQ\rightarrow_sA_d$ を $(A,A)_k$-bimodule の同型とします。 $p\in P$と$q\in Q$には関係$\langle p, \tau (q)\rangle =\lambda (p\otimes q)$によって決定される一意な写像$\tau : Q\rightarrow P^*$が存在し、$\tau$は$(B,A)_k$-bimodulesの同型です。

写像 $\tau$ の存在と一意性は明らかです。これは、$(B,A)_k$-bimodules の準同型で、$\lambda = \Lambda \circ (1_P\otimes \tau )$ があります。 $\lambda$ と Λ は $(A,A)_k$ バイモジュール (VIII、p. 101、定理 1) の同型であるため、$1_P\otimes \tau$ も同様です。 補題 1 により、写像 $\tau$ は全単射になります。

#### 注意 {#alg-viii-s6-n3-rem-1 .statement tag=0075}

系の仮定の下で、$q$ を Q の元とし、$p\in P$ ごとに $\lambda (p\otimes q) = 0$ が得られるようにします。すると、$\tau (q) = 0$、つまり$q= 0$になります。同様に、$p$ が P の元で、すべての $q\in Q$ に対して $\lambda (p\otimes q) = 0$ が得られる場合、$p= 0$ になります。

#### 例 1 {#alg-viii-s6-n3-exa-1 .statement tag=0076}

B を $k$-代数、$n$ 整数 $\geqslant 1$、A を $k$-代数 $\mathbf{M}_n(B)$ とします。 右B-加群 $P = B^n_d$ は射影的で有限生成され、生成するであり、A は P (II, §10, No. 7, p. 349) の自己準同型環と識別できます。 定理 1 までに、$(A,B)_k$-bimodule P は可逆になります。従って、代数 B と $\mathbf{M}_n(B)$ は森田に相当します。

#### 例 2 {#alg-viii-s6-n3-exa-2 .statement tag=00SH}

A を可換 $k$-代数、P を A-加群とします。 P を、作用の 2 つの法則が等しい $(A,A)_k$-bimodule として見ます。 $(A,A)_k$-bimodule P が可逆であれば、A-加群 P は有限生成されます (定理 1)。通信の定理 3までに。 Alg.、II, §5, No. 4、p. 114、次のプロパティは同等です。

(i) $(A,A)_k$-bimodule P は可逆です。

(ii) $P\otimes_AQ$ が A と同型となるような A-加群 Q が存在します。

(iii) A-加群 P は射影的で、有限に生成され、階数 $1.*$ の

### 4. ザ・モリタ対応/加群

この小節において、文字 A と B は森田等価な $k$-代数を表し、P は可逆 $(A,B)_k$-双加群を表します。 選ぶ P および同型の逆の $(B,A)_k$ バイモジュール Q

$\lambda : P\otimes_BQ\rightarrow_sA_d$ と $\theta : Q\otimes_AP\rightarrow_sB_d$。

左B-加群 V については、B-加群 $\theta \otimes 1_V: Q\otimes_AP\otimes_BV\rightarrow V$ の $\theta_V$ 準同型で表します。 $\theta$は同型なので、同型です。同様に、左A-加群 M ごとに、A-加群 $\lambda \otimes 1_M: P\otimes_BQ\otimes_AM\rightarrow M$ の $\lambda_M$ 準同型で表します。 $\lambda$は同型なので、同型です。

#### 定理 2 (森田) {#alg-viii-s6-thm-2 .statement tag=00S2}

a) V と W を左B-加群とします。 写像 $g\mapsto 1_P\otimes g$ は、ホム$_B(V,W)$ からホム$_A(P\otimes_BV,P\otimes_BW)$ までの全単射です。 逆全単射は Hom$_A(P\otimes_BV,P\otimes_BW)$ の元 $h$ を Hom$_B(V,W)$ の元 $\theta_W\circ (1_Q\otimes h)\circ \theta_V^{-1}$ に送信します。

b) すべての左A-加群 M は形 $P\otimes_BV$ の加群と同型であり、V は左B-加群です。

V と W を左B-加群とします。 Hom$_B(V,W)$からHom$_A(P\otimes_BV,P\otimes_BW)$までのVIII、p. 101、写像$\varphi :g\mapsto 1_P\otimes g$の補題1は単射です。 交換すること P と Q (および A と B) の役割によって、Hom$_A(P\otimes_BV,P\otimes_BW)$ から Hom$_A(Q\otimes_AP\otimes_BV,Q\otimes_AP\otimes_BW)$ までの写像 $\psi :h\mapsto 1_Q\otimes h$ も単射であることがわかります。さて、合成 $\psi \circ \varphi$ は写像 $g\mapsto \theta^{-1}_W\circ g\circ \theta_V$ です。これは全単射なので、$\psi$ も同様です。従って、$\varphi$ は全単射であり、その逆数は写像 $h\mapsto \theta_W\circ (1_Q\otimes h)\circ \theta^{-1}_V$ となります。

主張 b) は、$\lambda_M$ が $P\otimes_B$ $\otimes_A\otimes M$ から M までの同型であるという事実から続きます。

V を左B-加群とし、V の W 部分加群とします。 B-加群 P は射影 (VIII、p. 101、定理 1) なので、$P\otimes_BW$ から $P\otimes_BV$ までの標準写像は単射です。私たちは同一視する $P\otimes_BW$ と$P\otimes_BV$ の像がこの写像を通して続きます。 P と B を Q と A に置き換える場合も、同様の規則を採用します。

#### 命題 5 {#alg-viii-s6-prop-5 .statement tag=0077}

Vを左B-加群とします。 写像 $W\mapsto P\otimes_BW$ は、V の B-部分加群の集合から、包含順の $P\otimes_BV$ の A-部分加群の集合までの同型です。 逆同型は、B-部分加群の $\theta_V$ $Q\otimes_AP\otimes_BV$ の $Q\otimes_AN$ の下で、$P\otimes_BV$ の A-部分加群 N を像に送信します。

$D_B(V)$ 集合 B-部分加群または V を含む順に並べ、定義する集合 $D_A(P\otimes_BV)$ と $D_B(Q\otimes_AP\otimes_BV)$ も同様に表します。 $N\mapsto Q\otimes_AN$ で与えられる $D_A(P\otimes_BV)$ から $D_B(Q\otimes_AP\otimes_BV)$ までの $\varphi : D_B(V)\rightarrow$ $D_A(P\otimes_BV)$ を写像 $W\mapsto P\otimes_BW$ と $\psi$ 写像とします。これらは増加する写像であり、合成 $\psi \circ \varphi$ は写像 $W\mapsto \theta^{-1}_V$(W) であり、これは全単射です。従って、$\varphi$ は単射的であり、$\psi$ は全射的です。 置き換えること B と A、および V と $P\otimes_BV$ により、$\psi$ も単射であることがわかります。従って、$\varphi$ と $\psi$ は全単射であり、$\varphi$ の逆数写像は確かに命題で記述されたものになります。

#### 例 1 {#alg-viii-s6-n4-exa-1 .statement tag=0078}

VIII、p. 104 の命題を適用する 5 を、具体的なケース $V = B_s$ に当てはめてみましょう。

a) 写像 $J\mapsto$ PJ は、B の左イデアルの順序付き集合 $D(B_s)$ から、P の A-部分加群の順序付き集合 D(P) への同型です。その逆写像は、P の A-部分加群 M を左に送ります。 M 含む $Pb$ となるような B の理想的な J(M) 元 $b$ の B からなる。

b) 写像 $K\mapsto$ KP は、A の正しい理想の順序付けられた集合 $D(A_d)$ から、P の B-部分加群の順序付けられた集合 D(P) までの同型です。その逆写像は、B-部分加群を送信します。 P の V を、A の元 $a$ のからなるの右理想 K(V) にすると、V 含む $aP$ になります。

実際、A-加群 $P\otimes_BB_s$ は P と正準的に識別できます。J が B の左イデアルである場合、この識別を通じて $P\otimes_BB_s$ 対応するの $P\otimes_BJ$ の標準像が PJ になります。従って、写像 $J\mapsto$ PJ は、$D(B_s)$ から D(P) までの順序集合の同型です。 $J\in D(B_s)$ にしましょう。 PJ 含む $Pb$ が $J'$ になるように、B の元 $b$ の集合を表します。 B の左イデアル含む J であり、PJ$'\subset$ PJ があります。 写像 $J\mapsto$ PJ は順序集合の同型であるため、必然的に PJ$'=$ PJ と $J = J'$ が存在します。これは a) を証明します。

主張 b) は、可逆 $(B^o,A^o)_k$-bimodule P に適用される主張 a) から続きます。

B-加群 P が単純な場合に限り、環 A は体であることに注意してください。

#### 例 2 {#alg-viii-s6-n4-exa-2 .statement tag=0079}

それぞれ A の両側イデアル、B の両側イデアル、および P の $(A,B)_k$ サブバイモジュールの $\mathscr{B}_A,\mathscr{B}_B$ および $\mathscr{B}_P$ 集合で表します。

a) 写像 $\mathfrak{b}\mapsto P\mathfrak{b}$ は、$\mathscr{B}_B$ から $\mathscr{B}_P$ までの順序集合の同型です。 逆同型は、$Pb\subset P'$ となるように、P の $(A,B)_k$ サブバイモジュール $P'$ を、元 $b$ の B からなるの両側イデアルに送信します。

b) 写像 $\mathfrak{a}\mapsto \mathfrak{a}P$ は、$\mathscr{B}_A$ から $\mathscr{B}_P$ までの順序集合の同型です。 逆同型は、$aP\subset P'$ となるように、元 $a$ のからなるの両側イデアルに P の $(A,B)_k$ サブバイモジュール $P'$ を送信します。

確かに、J を B と $P'=$ PJ の左イデアルとします。このとき、$P'$ は P の A-部分加群であり、例 1 により、理想的な J は $Pb\subset P'$ となる B の元 $b$ で構成されます。さらに、J が B の両側イデアルである場合に限り、$P'$ は P の $(A,B)_k$ サブ双加群です。 したがって、a) は loc から続きます。引用。

主張 b) は、可逆 $(B^o,A^o)_k$-bimodule P に適用される主張 a) から続きます。

#### 命題 6 {#alg-viii-s6-prop-6 .statement tag=007A}

A の両側イデアルと B の両側イデアルを $\mathscr{B}_A$ と $\mathscr{B}_B$ 集合で表します。

a) 次の性質によって決定される $\mathscr{B}_A$ から $\mathscr{B}_B$ までの順序集合 $f$ の同型が存在します。$\mathfrak{a}$ が A の両側イデアルであり、$\mathfrak{b}$ が B の両側イデアルである場合、関係 $f(\mathfrak{a}) =\mathfrak{b}$ は $\mathfrak{a}P = P\mathfrak{b}$ と同等です。

b) 環 A が可換であると仮定します。そのため、A は B の中心と識別できます (VIII, p. 102, 系 1)。 同型 $f:\mathscr{B}_A\rightarrow$ $\mathscr{B}_B$ は、A の理想 $\mathfrak{a}$ を B の両面理想 $B\mathfrak{a}$ に送り、$\mathfrak{a}= A\cap B\mathfrak{a}$ が得られます。

主張 a) は例 2 から続きます。

ここで、A が可換で、同一視する A と B の中心があるとします。$\mathfrak{a}$ を A のイデアルとします。そのとき、$B\mathfrak{a}$ は B の両側イデアルです。 PB$\mathfrak{a}=\mathfrak{a}P$なので$f(\mathfrak{a}) = B\mathfrak{a}$です。 $\mathfrak{a}'$ を A の理想的な $A\cap B\mathfrak{a}$ とします。これは $B\mathfrak{a}$ と含む $\mathfrak{a}$ に含まれるため、$B\mathfrak{a}'$ は $B\mathfrak{a}$ に等しくなります。 $f$ は全単射なので、$\mathfrak{a}'=\mathfrak{a}$ になります。

#### 例 3 {#alg-viii-s6-n4-exa-3 .statement tag=007B}

Vを左B-加群とします。次に、上記の対応は、B-加群 V の消滅子を A-加群 $P\otimes_BV$ の消滅子に送信します。確かに、A-加群 $P\otimes_BV$ の消滅子を $\mathfrak{a}$ で表し、B-加群 V のそれを $\mathfrak{b}$ で表します。 W を、V のすべての元 $v$ に対して $p\otimes v= 0$ となる、元の P からなるの$(A,B)_k$ サブバイモジュールとします。 $P\mathfrak{b}\subset W$ が含まれています。逆に、$p\in W$ と $q\in Q$ ごとに、$\theta (q\otimes p)$ 属するから $\mathfrak{b}$ になります。したがって、$D(B_s)$ 対応するの元 $\mathfrak{b}$ から D(P) の元 W になります。同様に、$\mathfrak{a}\in D(A_d)$ 対応するを W に入力します。

#### 例 4 {#alg-viii-s6-n4-exa-4 .statement tag=007C}

A の任意の両側イデアル $\mathfrak{a}$ について、$\mathfrak{a}$ に $\mathbf{M}_n(\mathfrak{a})$ を入力して、$\mathbf{M}_n(A)$ の部分集合と行列のからなるを表します。 $\mathbf{M}_n(A)$の両面理想です。 $\mathbf{M}_n(\mathfrak{a})A^n=\mathfrak{a}^n= A^n\mathfrak{a}$があります。 命題 6 から、$\mathbf{M}_n(A)$ のすべての両側イデアルは形 $\mathbf{M}_n(\mathfrak{a})$ であることがわかります。ここで、$\mathfrak{a}$ は A の両側イデアルです。

#### 注意 {#alg-viii-s6-n4-rem-1 .statement tag=007D}

上記の仮定と記法を保持し、 $(B,A)_k$ バイモジュール Q が A-加群 P の双対 $P^*$ であり、 同型 $\lambda$ と $\theta$ が標準写像 $\Lambda  : P\otimes_BP^*\rightarrow_sA_d$ と Θ であると仮定します。 $P^*\otimes_AP\rightarrow_sB_d$ (VIII、p. 101、定理 1)。 A-加群 P は射影的で有限生成されるため、A-加群 M (II, §4, No. 2, p. 271, 系) ごとに標準同型 $\vartheta_M: P^*\otimes_AM\rightarrow$ Hom$_A(P,M)$ が得られます。 小節 3 と 4 の結果を置き換えること構成 $M\mapsto Q\otimes_AM$ と構成 $M\mapsto$ Hom$_A(P,M)$ で再定式化するのは読者に任せます。

### 5. 部分加群中順序集合

この小節において、AとBは$k$代数、Mは左A-加群、Vは左B-加群です。 D(M) (それぞれ D(V)) 部分加群の M (それぞれ V) の集合を包含順に表します。 順序集合 $\varphi : D(V)\rightarrow D(M)$ のうち同型が与えられたと仮定します。

森田の定理 (VIII、p. 103、定理 2) により、次の状況でそのような同型写像が得られます: P は可逆 $(A,B)_k$ 双加群、M は A 加群 $P\otimes_BV$、そして $V,\varphi (W)$ のすべての部分加群 W は M の $P\otimes_BW$ の正準像です。

加群 M またはその部分加群の一部のプロパティは、順序付けされた集合 D(M) の項で表現できます。それらは、表 I および II にリストされています。

加群 M は、$i\in I$ ごとに $M =\sum_{i\in I}M_i$ と $M_i\cap \sum_{j\not=i}M_j= 0$ がある場合に限り、家族の直和部分加群の $(M_i)_{i\in I}$ です。この注意と表 I を調べると、次の結果が得られます。

#### 命題 7 {#alg-viii-s6-prop-7 .statement tag=007E}

a) $\varphi (0) = 0$ と $\varphi (V) = M$ があります。

b) $(V_i)_{i\in I}$ を V の部分加群の家族とする。我々は持っています

$$
\varphi (\sum_{i\in I}V_i)=\sum_{i\in I}\varphi (V_i),\varphi (\bigcap_{i\in I}V_i)=\bigcap_{i\in I}\varphi (V_i)
$$

部分加群/M 注文集合 D(M)

零部分加群最小の元の D(M)

部分加群 M 最大の元 D(M)

$\bigcap_{i\in I}M_i$ 最大の下界詳細$_{i\in I}M_i$

$\sum_{i\in I}M_i$ 最低上界以上$_{i\in I}M_i$

補部分加群 inf(M$',M''$) $= 0$、sup(M$',M''$) $= M$

単純部分加群 M 最小元 D(M) $-\{0\}$

極大部分加群のM 極大元のD(M) $-\{M\}$

ソクル $\mathscr{S}(M)$ of M 最低上界 in D(M) of 集合 of M

D(M)$-\{0\}$ の最小元

$*$根基 $\mathfrak{R}(M)$ の M 最大の下界の D(M) の集合

$$
*
$$

(VIII、p. 151) の極大元の D(M)$-\{M\}$

表 I。

加群 M の特性 D(M) の特性

Mはネーターです。注文した集合 D(M) はネーター (集合)

理論、III, §6, No. 5、p. 190）。

Mはアルティンです。 $\supset$ によって注文された集合 D(M) は、

ネーター。

Mは不分解です。 M $\not= 0$ はありますが、

2 つの非零元 $M'$ と $M''$

D(M) 満たす inf(M$',M''$) $= 0$,

すぷ(M$',M''$)$= M$。

M は有限に生成されます。すべての家族のために $(M_i)_{i\in I}$ in D(M)

上界 M、有限が存在する

M = sup$_{j\in I}M_j$となるようなIの部分集合 J。 Mはシンプルです。カード(D(M)) = 2。

Mは半単純です。 M は D(M) の中で最小の上界、

集合の最小限の元

D(男)$-\{0\}$。

表 II。

c) B-加群 V は、M がファミリー $(\varphi (V_i))_{i\in I}$ の直和である場合に限り、ファミリー 部分加群の $(V_i)_{i\in I}$ の直和です。

$V'$ と $V''$ を V の部分加群として、$V'$ が $V''$ に含まれるようにします。 集合 $M'=\varphi (V')$ と $M''=\varphi (V'')$ なので、$M''$ 含む $M'$ になります。 D(V)の部分加群Wのからなる、Vの$V'\subset W\subset V''$、D(M)の定義する区間$[M',M'']$で$[V',V'']$区間で表します。 写像 $W\mapsto W/V'$ は、$[V',V'']$ から $D(V''/V')$ までの順序集合の同型です。私たち$[M',M'']$から$D(M''/M')$までの順序集合の定義する同型も同様です。 $\varphi$ は区間 $[V',V'']$ を $[M',M'']$ に送信するため、順序集合の定義する同型 $\varphi$ が $D(V''/V')$ から $D(M''/M')$ に送信されます。これから命題、表、I、IIが導き出されます。

#### 命題 8 {#alg-viii-s6-prop-8 .statement tag=007F}

a) $V'$ と $V''$ を $V''$ 含む $V'$ となるように V の部分加群とします。 B-加群 $V''/V'$ は、A-加群 $\varphi (V'')/\varphi (V')$ が単純である場合に限り、単純です。

b) $V'$ が V の単純部分加群、極大部分加群、または直因子である場合、$\varphi (V')$ はそれぞれ M の単純部分加群、極大部分加群、または直因子です。

c) 同型 $\varphi$ 変換ソクル V の $\mathscr{S}(V)$ を $M*$ および根基のソクル $\mathscr{S}(M)$ (VIII、p. 151、 定義 1) V の$\mathfrak{R}(V)$ を M$.*$ の根基 $\mathfrak{R}(M)$ に

d) $(V_i)_{0\leqslant i\leqslant n}$ を V の部分加群の有限列とします。 $(\varphi (V_i)_{0\leqslant i\leqslant n})$ が M のジョーダン – ヘルダー 系列である場合に限り、それは V のジョーダン – ヘルダー 系列です。

#### 補題 2 {#alg-viii-s6-lem-2 .statement tag=007G}

H と $H'$ を $H\cap H'= 0$ となるような V の部分加群とします。 B-加群 H と $H'$ は、A-加群 $\varphi (H)$ と $\varphi (H')$ が同型である場合に限り、同型です。

私たちは同一視する $H+H'$ と積 $H\times H'$ です。 Hから$H'$までの同型のグラフはV満たすの部分加群$H''$です

$$
H\cap H''= H'\cap H''= 0,H + H'= H + H''= H'+ H'' \tag{17}
$$

逆に、これらの特性を持つすべての部分加群は、H から $H'$ までの同型のグラフになります。 命題 7 により、関係 $H\cap H'= 0$ は $\varphi (H)\cap \varphi (H') = 0$ に相当し、関係 (17) は関係に相当します。

$$
\varphi (H)\cap \varphi (H'') =\varphi (H')\cap \varphi (H'') = 0
$$

$$
\varphi (H) +\varphi (H') =\varphi (H) +\varphi (H'') =\varphi (H') +\varphi (H'')
$$

補題が続きます。

#### 命題 9 {#alg-viii-s6-prop-9 .statement tag=00R6}

S を V の単純部分加群 、M の T 単純部分加群 $\varphi (S)$ とします。$V_S$ が型 S の V の同型成分と、$M_T$ の M の同型成分を表すとします。 型 T なら、$\varphi (V_S) = M_T$ です。

S とは異なる V のすべての単純部分加群 $S'$ は $S'\cap S = 0$ を満たします。したがって、$\varphi (S')$ が T (補題 2) と同型である場合に限り、それは S と同型です。さて、$V_S$ は S と同型の V の単純部分加群の和であり、$M_T$ は T と同型の M の単純部分加群の和です。 したがって、命題 9 は命題 7 と 8 のすぐ後に続きます。

#### 命題 10 {#alg-viii-s6-prop-10 .statement tag=007H}

a) M がそうである場合に限り、B-加群 V はアルティン (それぞれネーター、分解不可能、単純、有限生成) です。

b) A-加群 M が有限長を持つ場合に限り、B-加群 V は有限長を持ち、その場合、long$_B(V) =$ long$_A(M)$ が得られます。

c) A-加群 M が半単純 (それぞれ同型) である場合に限り、B-加群 V は半単純 (それぞれ同型) です。この場合、long$_B(V) =$ long$_A(M)$ になります。

主張 a) は、表 II にリストされている 2 番目の性質に続きます。

主張 b) は命題 8, d) から続きます。

加群 V は、ソクル $\mathscr{S}(V)$ と等しい場合に限り、半単純になります。 $V = V_S$ となるような V の単純部分加群 S が存在する場合にのみ同型です。したがって、主張 c) は、命題 7、c)、8、c)、および 9 (VIII、p. 106、および 109) から続きます。

### 6. 森田家のその他の保存資産対応

A と B を森田等価な $k$-代数、P を可逆 $(A,B)_k$-双加群とする。

#### 命題 11 {#alg-viii-s6-prop-11 .statement tag=007I}

させて

$$
(\mathscr{E})V'-\overset{f}{\rightarrow}V-\overset{g}{\rightarrow}V''
$$

B-加群と B-線型写像の図式にして、

$$
(P\otimes \mathscr{E})P\otimes_BV'\longrightarrow^{1_P\otimes f}P\otimes_BV\longrightarrow^{1_P\otimes g}P\otimes_BV''
$$

A-加群の対応する図式になります。次に、$(P\otimes \mathscr{E})$ が完全系列である場合に限り、$(\mathscr{E})$ は完全系列になります。

数列 $(\mathscr{E})$ が正確であると仮定します。 右B-加群 P は射影であるため、数列 $(P\otimes \mathscr{E})$ は正確です (II, §3, No. 6、p. 251、命題 5 および II, §3, No. 7、p. 257、系 6)。

逆に、数列 $(P\otimes \mathscr{E})$ が正確であるとします。 Q を P の逆の $(B,A)_k$ バイモジュール、および $\theta : Q\otimes_AP\rightarrow_sB_d$ 同型とします。可換図式を考えてみましょう

$Q\otimes_AP\otimes_B{V'}^{1_Q\otimes 1_P\otimes f}/$/ $Q\otimes_AP\otimes_BV^{1_Q\otimes 1_P\otimes g}/$/ $Q\otimes_AP\otimes_BV''$

$\theta \otimes 1_{V'}\theta \otimes 1_V\theta \otimes 1_{V''}$

$V'f$ // V $g$ // $V''$。

Q は射影 A-加群であり、数列 $(P\otimes \mathscr{E})$ は正確であるため、この図式の最初の行は完全系列です。垂直矢印は同型なので、2行目も正確です。

#### 系 {#alg-viii-s6-n6-cor-1 .statement tag=007J}

$f: V\rightarrow W$をB-線型写像とします。したがって、$1_P\otimes f$ がそうである場合にのみ、$f$ は単射法 (それぞれ全単射法) になります。

#### 命題 12 {#alg-viii-s6-prop-12 .statement tag=007K}

V を左B-加群とします。 B-加群 V は射影的 (それぞれ生成する、忠実、$*$単射的、有限表現)

$$
*
$$

A-加群 $P\otimes_BV$ です。

a) V が射影であると仮定します。 V が $B^{(I)}_s$ の直和因子部分加群と同型となるような集合 I が存在します。 A-加群 $P\otimes_BV$ は $P^{(I)}$ の直和因子部分加群と同型です。 P は射影 A-加群なので、同じことが $P\otimes_BV$ にも当てはまります。

b) B-加群 V が生成するであると仮定します。 MをA-加群とします。 M が $P\otimes_BW$ と同型となるような B-加群 W が存在します。 VIII、p. 80 の定理 1 までに、集合 I と射影 $\varphi : V^{(I)}\rightarrow W$ が存在します。 系, 写像 $P\otimes (V^{(I})$ から $P\otimes_AW$ までの$1_P\otimes \varphi$ は全射であり、全射$(P\otimes V)^{(I)}\rightarrow M$ になります。 定理までに、VIII、p. 80、$P\otimes V$の1は生成A-加群になります。

c) B-加群 V は、その消滅子が 0 に減らされた場合にのみ忠実です。 主張 c) したがって、VIII、p. 105 の例 3 から続きます。

$*$d) V が単射だと仮定します。 VIII、p. 106、A-加群の注意により、$P\otimes_BV$ は Hom$_B(Q,V)$ と同型であり、Q は A の逆 $(B,A)_k$ 双加群です。 A-加群 Q は射影であるため、平坦 (X, §1, n$^o3$、p. 9、例 1)、A-加群 Hom$_B(Q,V)$ は、X, §1、n$^o8$、p. 18、命題 11 によって単射になります。

e) V が有限表現 $L_1\rightarrow L_0\rightarrow V\rightarrow 0$ (X, §1, n$^o4$, p. 10) を認めると仮定します。 テンソル積を P とすることで、A-加群 $N'_1-\overset{u}{\rightarrow}N'_0\rightarrow P\otimes_BV\rightarrow 0$ の完全系列を推定します。ここで、$N'_1$ と $N'_0$ は射影で有限生成されます (命題 11 と a))。 $N''_0$ を有限生成A-加群として、加群 $N_0= N'_0\oplus N''_0$ が自由で有限に生成されるようにし、$u': N'_1\oplus N''_0\rightarrow N_0$ を準同型 $(u,1_{N''_0})$ とします。その場合、$P\otimes_BV$ は $u'$ の余核と識別できます。 $N_1$ を有限生成された自由A-加群と $p: N_1\rightarrow N'_1\oplus N''_0$ 全射準同型とします。 数列 $N_1\longrightarrow^{u'\circ p}N_0\rightarrow P\otimes_BV\rightarrow 0$ は A-加群 $P\otimes_BV.*$ の有限表現です

f) A-加群 $P\otimes_BV$ が射影的であると仮定します (それぞれ生成する、忠実、$*$単射的、有限表現 )。 適用までに上記(交換すること)

$$
*
$$

A と B、P と Q の役割)、B-加群 $Q\otimes_AP\otimes_BV$ にもこの性質があることがわかります。従って、同じことが B-加群 V にも当てはまり、これと同型です。

#### 系 {#alg-viii-s6-n6-cor-2 .statement tag=007L}

環 B がそうである場合に限り、環 A は左アルティン的 (それぞれ左ネーター) になります。

Bの左イデアルの順序付けられた集合とPのA-部分加群の集合の間の同型のため、A-加群Pがアルティン(それぞれアルティン)である場合に限り、環Bは左アルティン的(それぞれ左ネーター)になります。 ネーター）。しかし、定理までに、VIII、p. 101、A-加群の 1 つが生成するとなり、有限に生成されます。特に、$A_s$ は、整数 $n\geqslant 1$ の $P^n$ の直因子と同型です。従って、A が左アルティン的 (または左ネーター) である場合に限り、P はアルティン (またはネーター) になります。

### 7. 森田同値/代数

#### 命題 13 {#alg-viii-s6-prop-13 .statement tag=007M}

a) 2 つの $k$-代数が森田等価である場合、それらの中心は同型の $k$-代数です。

b) 2 つの可換$k$-代数は、それらが同型である場合に限り、森田等価です。

c) 体である 2 つの $k$-代数は、それらが同型である場合にのみ森田等価です。

d) $i= 1,2$ について、$A_i$ と $B_i$ を森田等価な $k$-代数、および $P_i$ を可逆な $(A_i,B_i)_k$-双加群とする。 集合 $A = A_1\otimes_kA_2,B = B_1\otimes_kB_2$、および $P = P_1\otimes_kP_2$。 $k$-代数 A と B は森田等価であり、P は可逆な $(A,B)_k$-双加群です。

e) A と B が森田等価 $k$-代数で、$k'$ が可換 $k$-代数である場合、$k'$-代数 $A_{(k')}$ と $B_{(k')}$ は森田等価です。

主張 a) は、VIII、p. 102 の系 1 から続き、b) を暗示します。

K と L を体である $k$-代数とし、P を可逆な $(K,L)_k$-双加群とする。右の L ベクトル空間 P は単純加群 (VIII, p. 104) なので、次元 1 なので、$k$-代数 End$_L(P)$ と L は同型です。 VIII, p. 101, 定理 1, 写像 $a\mapsto a_P$ K から End$_L(P)$ までは同型です。従って、体 K と L は $k$ に対して同型です。 主張 c) が続きます。

d) の仮定では、$Q_i(i= 1,2)$ を $P_i$ の逆 $(B_i,A_i)_k$-bimodule とします。 $(B,A)_k$-bimodule $Q_1\otimes_kQ_2$ を Q で表します。標準的 $k$-linear 同型 $(P_1\otimes_kP_2)\otimes_k(Q_1\otimes_kQ_2)\rightarrow (P_1\otimes_kQ_1)\otimes_k$ $(P_2\otimes_kQ_2)$; を考えてみましょう。 移行から商のとき、それは定義する射

$$
(P_1\otimes_kP_2)\otimes_B(Q_1\otimes_kQ_2)\rightarrow (P_1\otimes_{B_1}Q_1)\otimes_k(P_2\otimes_{B_2}Q_2)
$$

つまり、$(A$、A)-線形です。逆に、逆同型 $(P_1\otimes_kQ_1)\otimes_k(P_2\otimes_k$ $Q_2)\rightarrow (P_1\otimes_kP_2)\otimes_k(Q_1\otimes_kQ_2)$ 定義する $(A$、A)-線形射 $(P_1\otimes_{B_1}$ $Q_1)\otimes_k(P_2\otimes_{B_2}Q_2)\rightarrow (P_1\otimes_kP_2)\otimes_B(Q_1\otimes_kQ_2)$。これら 2 つの射は互いの逆数であるため、同型になります。 $(A_i,A_i$)-双モジュール $P_i\otimes_{B_i}Q_i$ は $A_i$ と同型なので、 $(A$, A)-線形同型 $P\otimes_B$ $Q\rightarrow A$ が得られます。同様に、$(B$, B) 線形同型 $Q\otimes_AP\rightarrow B$ が得られ、d) の証明が完成します。

e) の仮定では、P を可逆的な $(A,B)_k$-bimodule とします。この場合、$P_{(k')}$ は可逆的な $(A_{(k')},B_{(k')})_{k'}$-bimodule です。

A を $k$-代数、$e$ を A の冪等とする。 A の$k$ の加法、乗法、作用を備えた集合 $eAe$ は、 $k$-代数と単位元 $e$。

#### 命題 14 {#alg-viii-s6-prop-14 .statement tag=007N}

A と B を$k$-代数とする。すると、A と B は、次の条件 $\mathbf{M}_n(B)$ 満たすに整数 $n\geqslant 1$ と平方行列 $e= (e_{ij})$ が存在する場合に限り、森田等価です。

(i) $e^2=e$ があります。

(ii) 元 $e_{ij}$ によって生成される B の両側イデアルは B に等しい。

(iii) $k$-代数 A は $e\mathbf{M}_n(B)e$ と同型である。

条件 (i) と (ii) が満たされる場合、$(e\mathbf{M}_n(B)e,B)_k$-bimodule $eB^n_d$ は反転可能です。

定理 1 (VIII, p. 101) を考慮すると、$k$-代数 A は、有限生成された射影の自己準同型環および生成する右B-加群と同型である場合に限り、B と森田等価です。したがって、命題は以下の補題 3 と 4 から続きます。

#### 補題 3 {#alg-viii-s6-lem-3 .statement tag=007O}

右B-加群 P は射影的で有限生成され、整数 $n\geqslant 0$ と、以下の特性を持つ $\mathbf{M}_n(B)$ の冪等 $e= (e_{ij})$ が存在する場合に限り、生成するになります。

(i) B-加群 P は $eB^n_d$ と同型です。

(ii) 元 $e_{ij}$ によって生成される B の両側イデアルは B に等しい。

P を右B-加群とします。この場合、P は射影であり、それが形 $B^n_d$ の B-加群の直和因子部分加群と同型である場合に限り、有限生成されます。ここで、$n$ は整数 $\geqslant 0$ (II, §2, No. 2, p. 232, 系 1)。 $k$-代数 $\mathbf{M}_n(B)$ と End(B$^n_d$) を同一視するとすると、これは、P が $eB^n_d$ と同型であるような冪等 $e$ が $\mathbf{M}_n(B)$ に存在することを意味します。

B-加群 P は、そのトレース理想値 $\tau (P)$ が B に等しい場合、つまり $\tau (eB^n_d) = B$ (VIII、p. 80、定理 1) である場合に限り、生成するになります。 $x_1, . . . , x_n$ を $B^n_d$ 対応するから列の行列 $e$ の元とし、$eB^n_d$ の線型形式 $(b_1, . . . , b_n)\mapsto b_i$ を $x^*_i$ ($1\leqslant i\leqslant n$ の場合) とします。 家族 $(x_1, . . . , x_n)$ 生成する B-加群 $eB^n_d$ と家族 $(x^*_1, . . . , x^*_n)$ 生成するはその二重です。 さて、$\langle x^*_i, x_j\rangle =e_{ij}$ があるので、$\tau (eB^n_d)$ は、$e_{ij}$ によって生成された B の両側イデアルです。 これは補題 3 を証明します。

#### 補題 4 {#alg-viii-s6-lem-4 .statement tag=007P}

V を B-加群とし、E 自己準同型 $k$-代数 V とする。 $e$ を V の射影子および $e$ の P 像とします。 B-加群 P の $v\in eEe$ を自己準同型 $x\mapsto v(x)$ に送る写像は、$eEe$ から End$_B(P)$ までの $k$-代数の同型です。

主張で説明されている写像を $\varphi :eEe\rightarrow$ End$_B(P)$ で表します。それは$k$-代数の準同型です。 $u\in$ 終了$_B(P)$ にしましょう。 $x\in V$ の $v(x) =u(e(x))$ によって定義される V の $v$ 自己準同型によって示されます。 $x\in P$、つまり $\varphi (eve) =u$ に対して $(eve)(x) =$ $u(x)$ があります。従って、$\varphi$ は全射法です。 $w$ を $\varphi$ の核の元とします。 $w$の制限から核と$e$の像は零なので、$w$は零となり、$\varphi$が単射であることがわかります。

#### 例 1 {#alg-viii-s6-n7-exa-1 .statement tag=007Q}

A を $k$-代数、$e$ を $AeA = A$ となるような A の冪等とする。 $k$-代数 $eAe$ は、$A_d$ (補題 4) の部分加群 $eA_d$ の自己準同型 $k$-代数と同一視できます。 $AeA = A$ なので、命題 14 から、$eA_d$ は可逆な $(eAe,A)_k$-双加群であるため、$k$-代数 $eAe$ と A は森田等価です。さらに、森田の定理 (VIII, p. 103) は次の結果を暗示します。

a) M と N を左A-加群とします。 M から N までの $eM$ から $eN$ 拡大するから A-線型写像までのすべての $eAe$ 線形マッピング。

b) $k$-代数 $eAe$ 上のすべての左加群は、形 $eM$ の加群と同型であり、M は左A-加群です。

#### 例 2 {#alg-viii-s6-n7-exa-2 .statement tag=007R}

A を $k$-代数および $n\geqslant 1$ 整数とします。私たちは同一視する行列環 $\mathbf{M}_n(A)$ と右A-加群 $A^n_d$ の自己準同型環です。 A と $\mathbf{M}_n(A)$ が森田に相当することを見てきました。 左A-加群 M ごとに、同一視する $A^n_d\otimes_AM$ と $M^n$。 代数 $\mathbf{M}_n(A)$ は $M^n$ に左作用を持ち、次のようになります。

$$
(a\cdot m)_i=\sum_{j=1}^na_{ij}m_j
$$

$\mathbf{M}_n(A)$の$a= (a_{ij})$と$M^n$の$m= (m_i)$。森田の定理は次の結果を暗示しています。

a) 代数 $\mathbf{M}_n(A)$ 上のすべての左加群は、形 $M^n$ の加群と同型であり、M は左A-加群です。

b) M を左A-加群とします。 写像 $N\mapsto N^n$ は、M の A-部分加群の集合から $M^n$ の $\mathbf{M}_n$(A) サブモジュールの集合までの全単射です。

c) M と N を左A-加群とします。 A-線型写像 $g: M\rightarrow N$ の場合、$g_n$ を $M^n$ から $N^n$ までの写像 $(m_i)\mapsto (g(m_i))$ とします。すると写像$g\mapsto g_n$はホム$_A(M,N)$からホム$_{\mathbf{M}_n(A)}(M^n,N^n)$までの全単射です。

d) M を左A-加群とします。 環 $\mathbf{M}_n(A)$ に対する加群 $M^n$ は、A-加群 M が存在する場合に限り、分解不可能です (それぞれ半単純、単純、アルティン、ネーター、有限生成)。

#### 例 3 {#alg-viii-s6-n7-exa-3 .statement tag=007S}

A を主イデアル整域および L 非零として、有限生成された自由A-加群とします。 B を L の自己準同型環とします。この場合、L は可逆 $(A,B)_{\mathbf{Z}}$-bimodule であり、環 A と B は森田等価です。森田の定理、命題 10、a) (VIII、p. 109)、および有限生成A-加群 (VII, §4, No. 4、p. 19、定理 2) の構造定理により、すべて有限生成されます。 B-加群は $\oplus^m_{i=1}(L/\mathfrak{a}_iL)$ と同型で、$m$ は自然数で、$\mathfrak{a}_i$ は満たす $\mathfrak{a}_1\subset \mathfrak{a}_2\subset  \cdots  \subset \mathfrak{a}_m$ と $\mathfrak{a}_m\not= A$ の理想です。 整数 $m$ と理想 $\mathfrak{a}_i$ は一意に決まります。 VIII、p. 105 の命題 6 により、B のすべての両面イデアルは形 $dB$ になります。ここで、$d$ は A の元です。

### 練習問題 {#alg-viii-s6-exercises}

[§ 6 に対して練習問題](exercises/s6/)を参照してください。
