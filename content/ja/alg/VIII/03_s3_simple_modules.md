---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 3
section_title: Simple Modules
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.45-A VIII.54
pdf_pages: 0062-0071
extraction: native
subsections:
    - "no": 1
      title: Simple Modules
      page: 45
      pdf_page: 62
    - "no": 2
      title: Schur’s Lemma
      page: 47
      pdf_page: 64
    - "no": 3
      title: Maximal Submodules
      page: 48
      pdf_page: 65
    - "no": 4
      title: Simple Modules over an Artinian Ring
      page: 50
      pdf_page: 67
    - "no": 5
      title: Classes of Simple Modules
      page: 51
      pdf_page: 68
statements: 23
exercises: 10
content_sha256: 2d5d5513fd6a6f1b5f4a03d086304398296e7c03e7bfefeb60aeb0bbe62b6648
translated_from: content/en/alg/VIII/03_s3_simple_modules.md
translation_method: google
source_content_sha256: 0317407d0c3ced7b2648e2b8d2e1ca2a46c305400b4715365d0e28e9e8310de8
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 66a1854813a23708468ca3cde1bc2d00b75e971a9e8afae4d67c699f5df6f743
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3. 単純加群

### 1. 単純加群

次の定義 (II, §1, No. 10、p. 212) を思い出してください。

#### 定義 1 {#alg-viii-s3-def-1 .statement tag=0035}

Let A be 環. A-加群 M が非零で、0 や M と異なる部分加群を持たない場合、M は単純と呼ばれます。

A-加群 M が単純であるのは、M が相似関係 $A_M$ の環上で単純加群である場合に限ります。すべての単純加群は長さ 1 であり、分解不可能であり、したがって原始的です (VIII, p. 31, 命題 4, b))。

#### 例 1 {#alg-viii-s3-n1-exa-1 .statement tag=0036}

A が体 (I, §9, No. 1、p. 115、定理 1) である場合に限り、加群 $A_s$ は単純A-加群になります。 単純A-加群は、体 A に対する次元 1 のベクトル空間です。

#### 例 2 {#alg-viii-s3-n1-exa-2 .statement tag=0037}

A を体ではない主イデアル整域 (VII, §1, No. 1, p. 1, 定義 1) とします。 A のすべての既約元 $\pi$ に対して、A-加群 $A_s/(\pi )$ は単純であり、すべての単純A-加群はそのような加群 (VII, §4, No. 8, p. 25, 注意 4) と同型です。 $n\geqslant 2$ の場合、A-加群 $A_s/(\pi^n)$ は分解不可能 (VII, §4, No. 8、p. 24、命題 8) ですが、単純ではありません。

#### 例 3 {#alg-viii-s3-n1-exa-3 .statement tag=0038}

K を体 K 上で体, V 非零右ベクトル空間とし、A 部分環 of 環 End$_K(V)$ 含む自己準同型 of V とする有限階数 (たとえば、A = 終了$_K(V)$)。 V が単純A-加群であることを証明しましょう。W を V の非零 A-部分加群と W の $x$ 非零元とします。 V には $\varphi (x)\not= 0$ (II, §7, No. 5, p. 300, 定理 6) となるような線型形式 $\varphi$ が存在します。 V、写像 $z\mapsto y\varphi (z)$ のすべての $y$ について、A に対する階数 $\leqslant 1$、属するの線形です。従って、$Ax= V$ となり、なおさら W = V となり、V が単純A-加群であることが証明されます。

#### 命題 1 {#alg-viii-s3-prop-1 .statement tag=00QZ}

Let A be 環.

a) $\mathfrak{m}$ を A の左イデアルとします。A-加群 $A_s/\mathfrak{m}$ は、$\mathfrak{m}$ が最大左イデアルである場合にのみ単純です。

b) M を単純A-加群、$x$ を M の非零元とします。等式 $M = Ax$、$x$ の消滅子 $\mathfrak{m}$ は A の最大左イデアルであり、写像 $a\mapsto ax$ 定義する、移行から商まで、同型から $A_s/\mathfrak{m}$ まで M.

c) M を非零 A-加群とします。 M の非零元 $x$ ごとに $M = Ax$ がある場合、M は単純です。

$A_s/\mathfrak{m}$ の部分加群は形 $\mathfrak{n}/\mathfrak{m}$ であり、$\mathfrak{n}$ は含む $\mathfrak{m}$ (I, §4, No. 6, p. 41, 定理 4) の左イデアルです。従って、A-加群 $A_s/\mathfrak{m}$ は、$\mathfrak{m}\not= A$ があり、含む $\mathfrak{m}$ の左すべてのイデアル $\mathfrak{n}$ が $\mathfrak{n}/\mathfrak{m}= 0$ または $\mathfrak{n}/\mathfrak{m}= A_s/\mathfrak{m}$ を満たす場合、つまり $\mathfrak{n}=\mathfrak{m}$ または$\mathfrak{n}= A$。これは a) を証明します。

b) の仮定では、$Ax$ は M の非零部分加群であるため、M に等しい。その結果、移行から商により、写像 $a\mapsto ax$ 定義する、 $A_s/\mathfrak{m}$からMまで同型。従って、A-加群 $A_s/\mathfrak{m}$ は単純であり、左の理想値 $\mathfrak{m}$ は a) によって最大になります。これは b) を証明します。

c) の仮定では、N を M の非零部分加群とします。$x$ が N の非零元である場合、$Ax\subset N$ と $Ax= M$ があり、従って M = N になります。従って、M は単純です。

#### 系 1 {#alg-viii-s3-prop-1-cor-1 .statement tag=0039}

環 A が 0 に減らない場合、単純A-加群が存在します。

実際、クルルの定理 (I, §8, No. 6, p. 104, 定理 1) によれば、A の最大左理想が存在します。

#### 系 2 {#alg-viii-s3-prop-1-cor-2 .statement tag=003A}

A を局所環 (VIII, p. 26, 定義 1) およびその最大理想を $\mathfrak{r}$ とします。 A-加群 $A_s/\mathfrak{r}$ は単純で、すべての単純A-加群は $A_s/\mathfrak{r}$ と同型です。

#### 注意 1 {#alg-viii-s3-n1-rem-1 .statement tag=003B}

Aを可換環、Aの理想を$\mathfrak{m}$とすると、$\mathfrak{m}$はA-加群$A_s/\mathfrak{m}$の消滅子(II, §1, No. 12, p. 219, 定義 11)となります。従って、$\mathfrak{m}$ と $\mathfrak{m}'$ が A の異なるイデアルである場合、A-加群 $A_s/\mathfrak{m}$ と $A_s/\mathfrak{m}'$ は同型ではありません。 (0) が A の最大理想である場合、つまり A が体である場合に限り、忠実な単純A-加群 (II, §1, No. 12, p. 219) が存在します。

#### 注意 2 {#alg-viii-s3-n1-rem-2 .statement tag=003C}

非可換環 A の例と、A-加群 $A_s/\mathfrak{m}$ と $A_s/\mathfrak{m}'$ が同型となるような A の 2 つの異なる最大左イデアル $\mathfrak{m}$ と $\mathfrak{m}'$ を与えることができます (VIII, p. 52, 練習問題) 3)。

### 2. Schur’s 補題

#### 命題 2 {#alg-viii-s3-prop-2 .statement tag=003D}

A を環、M と N を 2 つ A-加群、M から N までを $f$ 非零準同型とします。

a) M が単純な場合、$f$ は単射法です。

b) N が単純な場合、$f$ は全射です。

c) M と N が単純な場合、$f$ は同型です。

$f$の核はMの真部分加群、$f$の像はNの非零部分加群です。

a) M が単純な場合、Ker($f$) $= 0$ があるため、$f$ は単射法です。

b) N が単純な場合、Im($f$) $= N$ があるため、$f$ は全射です。

c) M と N が単純な場合、$f$ は単射的かつ全射的です。

#### 系 (シュールの補題) {#alg-viii-s3-n2-cor-1 .statement tag=00RZ}

単純加群の自己準同型環は体です。

M が単純A-加群の場合、非零環 End$_A(M)$ のすべての非零元は反転可能 (命題 2, c)) であるため、End$_A(M)$ は体です。

#### 定理 1 {#alg-viii-s3-thm-1 .statement tag=003E}

K を代数的に閉じた可換体、A K-代数、M 単純A-加群とします。 K 上のベクトル空間としての M の次元が有限であるか、より一般的には K の基数より厳密に小さいとします。そのとき、A-加群 M の自己準同型環は $\alpha \in K$ との相似関係 $\alpha_M$ で構成されます。

E を A-加群 M の自己準同型環とします。それは、命題 2 の系と体 K 上の代数による体です。M を体 E 上の左ベクトル空間と見なすと、dim$_KM =$ になります。 (薄暗い$_EM$)$[E : K]$ by 命題 II, §1, No. 13、p. 222の25、したがって薄暗い$_KM\geqslant [E : K]$。 仮定による dim$_KM<$ Card(K) なので、等式 $E = K\cdot 1_M$ は次の補題の帰結になります。

#### 補題 1 {#alg-viii-s3-lem-1 .statement tag=003F}

E を体とし、E の中心の K 部分体は E に等しくありません。体 K が代数的に閉じている場合、$[E : K]\geqslant$ カード (K) が得られます。

$x$ を E - K の元とし、L を $K\cup  \{x\}$ によって生成された E の (可換) 部分体とします。 K は代数的に閉じているため、$x$ は K を超越します。L の VII, §2, No. 3、p. 10、定理 2 および p. 11、元 $(x-\alpha )^{-1}$ により、$\alpha$ は K を通過し、線形独立です。 K を超えています。したがって、$[E : K]\geqslant [L : K]\geqslant$ Card(K) があります。

#### 例 {#alg-viii-s3-n2-exa-1 .statement tag=003G}

$*$ A を元の可算族によって生成される $\mathbf{C}$-代数とする。 $\mathbf{C}$ には数えられる次元があります。 M を単純A-加群とします。それは単次なので、$\mathbf{C}$ にわたる可算数の基底が認められます。 体 $\mathbf{C}$ は数えられないので (Gen. Top.、IV, §4, No. 1、p. 44)、$[M :\mathbf{C}]<$ カード ($\mathbf{C}$) があります。したがって、A-加群 M の自己準同型は、$\alpha \in \mathbf{C}$ と相似関係にある $\alpha_M$ です。これは特に、A が $\mathbf{C}($Lie、I, §2, No. 7、p. 21、系 $3).*$ 上の有限次元リー代数の普遍包絡代数である場合に当てはまります。

#### 系 1 {#alg-viii-s3-lem-1-cor-1 .statement tag=003H}

定理の仮定を 1 に保ち、さらに、代数 A が可換であると仮定します。すると、M は K に対して次元 1 を持ちます。

環 A は可換であるため、$a_M$ は、$a\in A$ ごとに A-加群 M の自己準同型になります。したがって、定理 1 によって、$A_M= K\cdot 1_M$ が得られ、M は単純な K-加群、つまり体 K 上の 1 次元のベクトル空間です。

#### 系 2 {#alg-viii-s3-lem-1-cor-2 .statement tag=003I}

K を可換体、A を K-代数、M を A-加群とします。 K のすべての拡大 L に対して、$A_{(L)}$ 加群 $M_{(L)}$ が単純であると仮定します。すると、M の自己準同型環は、$\alpha \in K$ との相似関係 $\alpha_M$ で構成されます。

I を、K を超える M の次元より厳密に大きい基数の集合とします (たとえば、M の部分集合の集合)。 L を体 $K((X_i)_{i\in I})$ の代数閉包とします (V, §4, No. 3、p. 23、定理 2)。 選ぶは $\varphi (1) = 1$ となるような L 上の K 線形形式 $\varphi$ であり、$v: M_{(L)}\rightarrow M$ は $v(\alpha \otimes m) =\varphi (\alpha )m$ によって特徴付けられる K-線型写像とします。 $u$ を M の自己準同型とします。 L 上の $M_{(L)}$ の次元は、K 上の M の値と等しく、厳密には L の基数よりも小さくなります。 定理 1 により、$A_{(L)}$ モジュール $M_{(L)}$ の自己準同型 $1_L\otimes u$ は、$\lambda \in L$ を持つ形 $\lambda \otimes 1_M$ になります。 $x\in M$ ごとに、

$$
u(x) =v(1\otimes u(x))=v((1_L\otimes u)(1\otimes x))
$$

$$
=v((\lambda \otimes 1_M)(1\otimes x))=v(\lambda \otimes x) =\varphi (\lambda )x
$$

従って、$u$ はホモテティー $\varphi (\lambda )_M$ になります。

### 3. 極大部分加群

#### 定義 2 {#alg-viii-s3-def-2 .statement tag=003J}

Aを環、MをA-加群とします。 M の極大部分加群は、M の真部分加群の集合の極大元です。

$A_s$ の極大部分加群は、単に A の左最大イデアルです。

N を M の部分加群とします。 The submodules of $M/N$ are of the form $P/N$, where P is a submodule of M containing N (I, §4, No. 6, p. 41, Theorem 4). 従って、加群 $M/N$ が単純な場合に限り、N は M の極大部分加群になります。

#### 命題 3 {#alg-viii-s3-prop-3 .statement tag=003K}

M を有限生成A-加群とします。 M のすべての真部分加群は極大部分加群に含まれます。

N を M の真部分加群とします。M 含む N の真部分加群の $\mathscr{S}$ 集合を包含順に並べて表します。 $\mathscr{S}$ が帰納的であることを証明しましょう。 $\mathscr{F}$ を $\mathscr{S}$ の完全に順序付けられた部分集合とします。 $\mathscr{F}$ が空の場合、$\mathscr{S}$ の $\mathscr{F}$ の N は上界です。逆の場合は、$\mathscr{F}$の元のQ和集合で表します。このとき、Q は M の部分加群です。F を M の有限生成部分集合とします。Q が M に等しい場合、F は部分加群 $P\in \mathscr{F}$ に含まれることになります。これは、$\mathscr{F}$ の定義とは反対に、P = M を意味します。従って、$Q\in \mathscr{S}$ が得られ、$\mathscr{S}$ が帰納的であることが証明されます。 命題 3 は、集合理論、III, §2, No. 4、p. 155 の系 1 から続きます。

#### 系 1 {#alg-viii-s3-prop-3-cor-1 .statement tag=003L}

M を非零有限生成A-加群とします。 A の $\mathfrak{a}$、単純A-加群の消滅子という両側理想が存在し、$\mathfrak{a}M$ は M に等しくありません。

N を M (命題 3) の極大部分加群とし、$\mathfrak{a}$ を単純A-加群 $M/N$ の消滅子とします。それは A の両面理想であり、$\mathfrak{a}(M/N) = 0$、よって $\mathfrak{a}M\subset N$、そして結果的に $\mathfrak{a}M\not= M$ になります。

#### 系 2 {#alg-viii-s3-prop-3-cor-2 .statement tag=003M}

Aを可換環、BをA-代数とします。 M を有限生成A-加群である単純B-加群とし、$\mathfrak{m}$ を A-加群 M の消滅子とします。すると、$\mathfrak{m}$ は A の最大イデアルであり、M は体 $A/\mathfrak{m}$ を超える有限次元ベクトル空間です。

環 A は可換であるため、単純A-加群の消滅子は A の最大イデアル (VIII, p. 46, 命題 1) です。 系 1 を A-加群 M に適用すると、$\mathfrak{a}M\not= M$ となる A の最大理想 $\mathfrak{a}$ が存在します。しかし、$\mathfrak{a}M$ は単純B-加群 M の部分加群です。従って、$\mathfrak{a}M = 0$ があり、その結果、$\mathfrak{a}\subset \mathfrak{m}$ になります。理想的な $\mathfrak{m}$ は A とは異なるため、$\mathfrak{a}$ に等しいため、$\mathfrak{m}$ が最大になります。 加群 M は有限生成加群体 $A/\mathfrak{m}$ を超えています。 最後の主張が続きます。

### 4. 単純加群アルティン環

A を環とします。言葉の乱用により、包含順に並べた A の集合の非零の最小の元である場合、左イデアル $\mathfrak{a}$ は A の最小の左イデアルであると言います。私たちは、最小理想と両面最小理想を同様に定義する正しいものとします。

$\mathfrak{a}$ を A の左イデアルとします。すると、それが A の最小左イデアルである場合に限り、$\mathfrak{a}$ は単純A-加群になります。

左アルティン的 (VIII、p. 1、定義 1) 環含むの最小左イデアルのすべての非零左イデアル。

#### 命題 4 {#alg-viii-s3-prop-4 .statement tag=003N}

A を最小左イデアル $\mathfrak{a}$ を持つ環とします。すべての信者単純A-加群は A-加群 $\mathfrak{a}$ と同型です。

M を忠実な単純A-加群にしましょう。 $\alpha$を$\mathfrak{a}$の非零元とします。 A-加群 M は忠実なので、$\alpha x\not= 0$ となるような M の元 $x$ が存在します。 $\mathfrak{a}$ から M までの準同型 $a\mapsto ax$ は非零です。従って、VIII、p. 47 の 2 である命題により、同型となります。

#### 命題 5 {#alg-viii-s3-prop-5 .statement tag=003O}

A を左アルティン的環とし、M を忠実な A-加群とします。

a) $M^m$の$A_s$から部分加群まで自然数$m$と同型が存在します。

b) M がジョーダン・ヘルダー 系列 $(M_i)_{0\leqslant i\leqslant n}$ を認める場合、すべての単純A-加群は商 $M_i/M_{i+1}$ の 1 つと同型です。

By VIII, p. 2 applied to the A-module $A_s$ and the annihilators of the elements of M, there exist elements $x_1, . . . , x_m$ of M such that the annihilator of M is the intersection of the annihilators of the $x_i$. A-加群 M は忠実なので、$A_s$ から $M^m$ までの A-線型写像 $a\mapsto (ax_1, . . . , ax_m)$ は単射であり、よって a)。

Under the assumption of b), every simple quotient of $A_s$ is isomorphic to a quotient of a Jordan–Hölder series of $M^m$ (I, §4, No. 7, p. 43, Corollary), hence to one of the modules $M_i/M_{i+1}$ (I, §4, No. 7, p. 43, Theorem 6). すべての単純A-加群は $A_s$ の商と同型であると結論する考えます。

#### 注意 {#alg-viii-s3-n4-rem-1 .statement tag=003P}

命題 5 は、特に次の 2 つの場合に適用されます。

a) A を可換体 K 上の代数とし、M を K 上の忠実な有限次元加群とします。その場合、M は有限長の A-加群であり、M の対加群は有限生成されます。 環 A は左アルティン的 (VIII、p. 9、命題 6) です。 A-加群 M の Jordan–Hölder 系列 $(M_i)_{0\leqslant i\leqslant n}$ が存在し、すべての単純A-加群は $0\leqslant i\leqslant n-1$ の加群 $M_i/M_{i+1}$ のいずれかと同型です。

b) A を左アルティン的環とします。 加群 $A_s$ には有限長 (VIII、p. 6、定理 1) があります。 A-加群 $A_s$ には有限長があるので、$\mathfrak{a}_0= A$ と $\mathfrak{a}_n= 0$ があり、$1\leqslant i\leqslant n$ に対して A-加群 $S_i=\mathfrak{a}_{i-1}/\mathfrak{a}_i$ が単純であるような A の左イデアルの減少列 $(\mathfrak{a}_i)_{0\leqslant i\leqslant n}$ が存在します。従って、すべての単純A-加群は加群 $S_1, . . . ,S_n$ のいずれかと同型になります。

### 5. 単純加群の類

Is$_A(X,Y)$ 関係で表します

「A は環で、$X,Y$ は同型 A-加群です。」

これはXとYに関して同値関係です。XがA-加群であれば、Is$_A$のXに相当するオブジェクトの類をcl(X)で表し、A-加群の類と呼びます。 X (集合理論、II, §6, No. 9、p. 122)。 By 定義, cl(X) is A-加群 isomorphic to X; moreover, two A-加群 X and Y are isomorphic if and only if we have cl(X) = cl(Y).

A を環とします。 関係

「$\lambda$は有限生成A-加群の類です」

$\lambda ($集合理論、II, §1, No. 4、p. 68）で集団化しています。実際、すべての有限生成A-加群は形 $A^n_s/R$ の A-加群と同型であり、$n$ は自然数および $A^n_s$ の R 部分加群であるため、主張は集合の後に続きます。 理論、II, §6, No. 9、p. 122。

有限生成A-加群の類の集合を$\mathscr{F}(A)$で表します。すべての単純A-加群は単属 (VIII、p. 46、命題 1) であり、その結果、単純A-加群の類形部分集合は $\mathscr{F}$ (A) であり、これをこれから次のように表します。 $\mathscr{S}(A)$ (または単に $\mathscr{S}$)。 環 A が可換である場合、写像 $\mathfrak{m}\mapsto$ cl(A$/\mathfrak{m}$) は、A の最大イデアルの集合から集合 $\mathscr{S}(A)$ までの全単射 (上記および VIII、p. 46、 注意 1）。 A が左アルティン的のとき、集合 $\mathscr{S}(A)$ は有限です (VIII、p. 51、注意 b))。

### 練習問題 {#alg-viii-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
