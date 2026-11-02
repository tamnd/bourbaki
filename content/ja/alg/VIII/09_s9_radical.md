---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 9
section_title: Radical
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.151-A VIII.172
pdf_pages: 0168-0189
extraction: native
subsections:
    - "no": 1
      title: The Radical of a Module
      page: 151
      pdf_page: 168
    - "no": 2
      title: The Radical of a Ring
      page: 154
      pdf_page: 171
    - "no": 3
      title: Nakayama’s Lemma
      page: 158
      pdf_page: 175
    - "no": 4
      title: Lifts of Idempotents
      page: 159
      pdf_page: 176
    - "no": 5
      title: Projective Cover of a Module
      page: 161
      pdf_page: 178
statements: 49
exercises: 31
content_sha256: a2b09163c728e4210f3843e8c46ef54302925f522b3e9995830c17b291842773
translated_from: content/en/alg/VIII/09_s9_radical.md
translation_method: google
source_content_sha256: 89095724e574bba079cd13ef874a02941adc59513c6a22e5a09bd9f01b4fa6cc
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 3464155655c4f1247b276be3f63a9c2dac8687fd6c3054b879d1733c37a9efa3
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 9。 根基

### 1. 加群中根基

#### 定義 1 {#alg-viii-s9-def-1 .statement tag=00A1}

A を環とします。 The radical of an A-module M is the submodule defined as the intersection of the maximal submodules of M (VIII, p. 48, Definition 2) or, equivalently, the set of elements of M annihilated by every homomorphism from M to a simple A-module.

この章の残りでは、A-加群 M の根基を $\mathfrak{R}_A(M)$ または単に $\mathfrak{R}(M)$ で表します。

Aを環とします。 A-加群の根基は、$\cap_{i\in I}$が存在するような単純A-加群の家族$(S_i)_{i\in I}$とA-線型写像$f_i: M\rightarrow S_i$の家族$(f_i)_{i\in I}$が存在する場合に限り、Mは0に減らされます（この場合、言葉の乱用により、Mには根基がないと言います）。カー($f_i$)$= 0$。これは、M が単純A-加群の積の部分加群と同型であることに相当します。

#### 例 1 {#alg-viii-s9-n1-exa-1 .statement tag=00A2}

$\mathfrak{a}$ を A の左イデアルとします。 A-加群 $A_s/\mathfrak{a}$ の根基は $\mathfrak{a}'/\mathfrak{a}$ に等しく、ここで $\mathfrak{a}'$ は含む $\mathfrak{a}$ の最大左イデアルの共通部分です。特に、$\mathbf{Z}$ モジュール $\mathbf{Z}$ の根基は 0 に減らされ、$\mathbf{Z}$ モジュール $\mathbf{Z}/p^n\mathbf{Z}$ の根基は、すべての素数数 $p$ およびすべての整数 $n\geqslant 1$ について $p\mathbf{Z}/p^n\mathbf{Z}$ に等しくなります。

#### 例 2 {#alg-viii-s9-n1-exa-2 .statement tag=00A3}

A を体ではない主イデアル整域とし、K をその分数の体とします。 K-加群として、Kには根基がありません。 K の根基を A-加群として見て、K に等しいことを証明しましょう。同等に、K から単純A-加群 S までのすべての A-線型写像 $f$ は零であると証明しなければならないなります。 VII, §4, No. 8、p. 25 により、S は $A/(\pi )$ に等しいと仮定できます。ここで、$\pi$ は A の既約元です。 $\pi S = 0$ であるため、$x\in K$ ごとに $f(x) =f(\pi \frac{x}{\pi})=\pi f(\frac{x}{\pi})= 0$ が得られます。

#### 命題 1 {#alg-viii-s9-prop-1 .statement tag=00A4}

M と N を M から N までA-加群と $f$ 準同型とします。 $f$が全射で、$f$の核がMの根基に含まれる場合、$f(\mathfrak{R}(M))\subset \mathfrak{R}(N)$があり、さらに等式もあります。

$g$ を N から単純A-加群までの準同型とします。すると、$\mathfrak{R}(M)$は$g\circ f$の核に含まれるため、$f(\mathfrak{R}(M))$は$g$の核に含まれます。したがって、$f(\mathfrak{R}(M))\subset \mathfrak{R}(N)$ となります。ここで、$f$ が全射的であり、その核が $\mathfrak{R}(M)$ に含まれると仮定します。 $y$ を $\mathfrak{R}$(N) の元とし、$x$ を $y$ の逆像の元とします。 $g$ が M から単純A-加群 S までの準同型である場合、その核含む根基は、$f$ の核となります。 準同型 $f$ は全射なので、$g=h\circ f$ となるような N から S までの準同型 $h$ が存在します。 $y=f(x)$ 属するから $\mathfrak{R}$(N) までなので、$h(f(x)) = 0$、つまり $g(x) = 0$ になります。したがって、$x$ 属するから $\mathfrak{R}$(M)​​ となり、$\mathfrak{R}(N)\subset f(\mathfrak{R}(M))$ が含まれることが証明されます。

#### 系 1 {#alg-viii-s9-prop-1-cor-1 .statement tag=00A5}

M を M の A-加群、N を部分加群とします。

a) $\mathfrak{R}(N)\subset \mathfrak{R}(M)\cap N$ があります。

b) $(\mathfrak{R}(M) + N)/N\subset \mathfrak{R}(M/N)$ があります。 N が $\mathfrak{R}(M)$ に含まれる場合、等式 $\mathfrak{R}(M/N) =\mathfrak{R}(M)/N$ になります。

c) 加群 $M/\mathfrak{R}(M)$ には根基がありません。 加群 $M/N$ に根基がなければ、$\mathfrak{R}(M)\subset N$ になります。

主張 a) 命題 1 から標準単射に N から M まで適用され、主張 b) 命題 1 から標準写像に M から $M/N$ まで適用されます。 b) から、$N =\mathfrak{R}(M)$ であれば $M/N$ には根基が無く、$M/N$ に根基がなければ $\mathfrak{R}(M)\subset N$ があると推測します。

例 1 から、$M/N$ の根基が零ではないような部分加群 N 含む $\mathfrak{R}(M)$ が存在し得ることがわかります。

#### 系 2 {#alg-viii-s9-prop-1-cor-2 .statement tag=00A6}

$(M_i)_{i\in I}$ を A-加群の家族、P を積 、S を直和とします。 $\mathfrak{R}(P)\subset \prod_{i\in I}\mathfrak{R}(M_i)$と$\mathfrak{R}(S) =\bigoplus_{i\in I}\mathfrak{R}(M_i)$があります。

$i\in I$ の場合、$\pi_i$ を P から $M_i$ までの添字 $i$ で射影とします。 命題 1 までに、$i\in I$ ごとに $\pi_i(\mathfrak{R}(P))\subset \mathfrak{R}(M_i)$ が得られます。これは最初の主張を証明します。 $S\subset P$ があるため、

$$
\mathfrak{R}(S)\subset S\cap \mathfrak{R}(P)\subset S\cap \prod_{i\in I}\mathfrak{R}(M_i) =\bigoplus_{i\in I}\mathfrak{R}(M_i)
$$

さらに、$i\in I$ ごとに $M_i\subset S$ があり、従って $\mathfrak{R}(M_i)\subset \mathfrak{R}(S)$ となり、結果として $\oplus_{i\in I}\mathfrak{R}(M_i)\subset \mathfrak{R}(S)$ になります。

積の根基が根基の積(VIIIの3練習問題、p. 166)と同型ではないような加群の族が存在します。

#### 命題 2 {#alg-viii-s9-prop-2 .statement tag=00A7}

M を有限生成A-加群とします。

a) M が 0 に減らない場合、$\mathfrak{R}(M)\not= M$ になります。

b) N が $N +\mathfrak{R}(M) = M$ となるような M の部分加群である場合、N = M になります。

N を M の真部分加群とします。VIII、p. 49 の命題 3 により、M 含む N の極大部分加群 L が存在します。$N +\mathfrak{R}(M)\subset L$ となおさら $N +\mathfrak{R}(M)\not= M$ があります。これは b) を証明します。特定のケース N = 0 では主張 a) が得られます。

#### 系 {#alg-viii-s9-n1-cor-1 .statement tag=00A8}

M を M の A-加群、$(x_i)_{i\in I}$ 生成するファミリ、および M の $x$ 元とします。以下のプロパティは同等です。

(i) $x\in \mathfrak{R}(M)$ があります。

(ii) $N + Ax= M$ が M に等しくなるように、M のすべての部分加群 N。

(iii) A の各家族 $(a_i)_{i\in I}$ 元に対して、家族 $(x_i+a_ix)_{i\in I}$ 生成する A-加群 M.

(i) $\Rightarrow$ (ii): $x$ 属する ～ $\mathfrak{R}(M)$ とします。 N を $N + Ax= M$ となるような M の部分加群とします。 $N +\mathfrak{R}(M) = M$ があります。従って、A-加群 $M/N$ は、命題 1) の根基 (系 1, b) に等しい。単次なので、零 (命題 2) となり、M = N となります。

(ii) $\Rightarrow$ (iii): $(a_i)_{i\in I}$ を A の元の族とする。$(x_i+a_ix)_{i\in I}$ 族によって生成された M の N 部分加群で表す。 $i\in I$ ごとに $x_i\in N + Ax$ があるため、$N + Ax= M$ になります。 性質 (ii) が成り立つ場合、N は M に等しくなります。

(iii) $\Rightarrow$ (i): $x$ が $\mathfrak{R}(M)$ に属するしないと仮定します。すると、含む $x$ を持たない M の極大部分加群 N が存在します。 N が最大であるため、$N + Ax= M$ になります。従って、元 $x_i$ はそれぞれ、$y_i\in N$ と $a_i\in A$ を組み合わせて $y_i-a_ix$ と書くことができます。ファミリ $(x_i+a_ix)_{i\in I}$ は N に含まれるため、生成する M には含まれません。

#### 命題 3 {#alg-viii-s9-prop-3 .statement tag=00A9}

a) 半単純加群には根基がありません。

b) 加群は半単純であり、根基とアルティンがない場合に限り、有限に生成されます。

定義により、単純加群の根基は0になります。 加群 M が半単純である場合、それは単純部分加群の家族 $(S_i)_{i\in I}$ の直和であり、上記の命題 1 の系 2 によって $\mathfrak{R}(M) =\bigoplus_{i\in I}\mathfrak{R}(S_i)$ が得られるため、$\mathfrak{R}(M) = 0$ になります。

さらに、M が有限生成されるとすると、VIII, p. 71 の命題 10 によりアルティンとなります。

逆に、M がアルティンで、根基がないとします。 VIII, p. 2 を M の極大部分加群の集合に適用すると、共通部分が 0 に減らされる M の極大部分加群の有限族 $(N_i)_{i\in I}$ が存在します。そのとき、M は $\bigoplus_{i\in I}(M/N_i)$ の部分加群と同型です。従って、半単純であり、有限長があり、なおさらが有限生成されます。

### 2. 環中根基

#### 定義 2 {#alg-viii-s9-def-2 .statement tag=00AA}

環 A のヤコブソン根基 (または単に根基) は、$\mathfrak{R}(A)$ で示され、A-加群 $A_s$ の根基、つまり A の最大左イデアの共通部分です。

言葉の乱用により、$\mathfrak{R}(A) = 0$ がある場合、環 A には根基がないと言います。

#### 命題 4 {#alg-viii-s9-prop-4 .statement tag=00AB}

環 A は、左アルティン的であり、根基がない場合に限り、半単純です。

これは、命題 3、b) からA-加群 $A_s$ に適用されます。

#### 例 1 {#alg-viii-s9-n2-exa-1 .statement tag=00AC}

A が局所環の場合、A の非可逆元の固有の最大左イデアル $\mathfrak{r}$、からなる (VIII、p. 25、命題 1) が存在します。従って、$\mathfrak{r}$ は A の根基です。特に、体には根基がありません。

#### 例 2 {#alg-viii-s9-n2-exa-2 .statement tag=00AD}

変数 $X_i$ の形式的冪系列の K を可換体と E 代数 $K[[X_i]]_{i\in I}$ とし、K に係数を代入します。前の例と例 4 の VIII、p. 26 により、 E の根基は、定数項零を伴う形式的な冪系列で構成されます。 環 E が整域であり、その根基が 0 に減らないこと、さらにはけれども E が分数の体の部分環であり、根基が無いことに注目してください。

#### 例 3 {#alg-viii-s9-n2-exa-3 .statement tag=00AE}

Aを主イデアル整域とし、Pを既約元(VII, §1, No. 3、p. 3)の代表からなるの系とする。 A が体の場合、例 1 によって根基はありません。集合 P が無限大の場合、A の最大理想値 $Ap$ の共通部分は 0 に減らされるため、A には根基がありません。しかし、P が有限で空でないで、集合 $x=\prod_{p\in P}p$ の場合、A の根基は $\cap_{p\in P}Ap= Ax$ (VII, §1, No. 2, p. 3, 命題 4) に等しいため、0 には減りません。

$y$ を A の非零元とします。これを $y=up^{i_1}_1\cdots p^{i_r}_r$ と書きます。ここで、$u$ は $A,p_1, . . . , p_r$ で可逆であり、ペアごとに異なる P の元であり、$i_1, . . . , i_r$ は厳密には正の整数です。 環 $A/Ay$ の最大の理想は $Ap_1/Ay, . . . ,Ap_r/Ay$ です。従って、環 $A/Ay$ の根基が理想的な $Ap_1\cdots p_r/Ay$ になります。特に、環 $A/Ay$ には、$i_1=\cdots =i_r= 1$ がある場合に限り、根基がありません。この場合、$y$ には倍数因子がないと言えます。

#### 命題 5 {#alg-viii-s9-prop-5 .statement tag=00AF}

a) 環 A の根基は単純A-加群の消滅子の共通部分です。それは半単純A-加群の最小の消滅子でもあります。特に、これは A の両側イデアルです。A が 0 に還元されない場合、A の根基は A とは異なります。

b) $\mathfrak{a}$ を A の両面理想とします。$(\mathfrak{R}(A) +\mathfrak{a})/\mathfrak{a}\subset \mathfrak{R}(A/\mathfrak{a})$ があります。 $\mathfrak{a}$が$\mathfrak{R}(A)$に含まれる場合、$\mathfrak{R}(A/\mathfrak{a}) =\mathfrak{R}(A)/\mathfrak{a}$になります。

c) 環 $A/\mathfrak{R}(A)$ には根基がありません。逆に、$A/\mathfrak{a}$ が根基含む $\mathfrak{R}(A)$ を持たないような A のすべての両面理想 $\mathfrak{a}$ 。

d) A の根基は、A の最大の両面イデアルの共通部分に含まれます。

$x\in A$ にしましょう。 Saying that $x$ belongs to the annihilator of every simple A-module is equivalent to saying that $x$ belongs to the annihilator of every element of every simple A-module, in other words (VIII, p. 46, Proposition 1), to every maximal left ideal of A.

M を半単純A-加群とします。その消滅子は M の単純部分加群の消滅子の共通部分なので、含む $\mathfrak{R}(A)$ です。さらに、$\mathscr{S}$ が単純A-加群 (VIII、p. 51) の類の集合である場合、直和 $\oplus_{\lambda\in\mathscr{S}}\lambda$ は消滅子が $\mathfrak{R}(A)$ である半単純A-加群です。 A が 0 に減らないと仮定します。 関係 $\mathfrak{R}(A)\not= A$ は、命題 2、VIII、p. 153 の a) からA-加群 $A_s$ に適用されます。私たちは a) を証明しました。

$\mathfrak{a}$ を A の両面理想とする。 $A/\mathfrak{a}$ の最大左理想は形 $\mathfrak{m}/\mathfrak{a}$ の理想であり、$\mathfrak{m}$ は含む $\mathfrak{a}$ の最大左理想です。 従って、環 $A/\mathfrak{a}$ の根基は、A-加群 $A_s/\mathfrak{a}$ の根基と等しくなります。 従って、主張 b) と c) は、VIII の 1、p. 152 から系に続きます。

$\mathfrak{a}$ を A の最大の両側イデアルとします。 環 $A/\mathfrak{a}$ では、両側イデアルは 0 と $A/\mathfrak{a}$ だけです。 環 $A/\mathfrak{a}$ は 0 に減らないため、その根基は $A/\mathfrak{a}$ に等しくなりません。従って、環 $A/\mathfrak{a}$ には根基がなく、c) により $\mathfrak{R}(A)\subset \mathfrak{a}$ が得られます。これは d) を証明します。

A の左 (または右) イデアルが冪零元で構成される場合、それはゼロイデアルであると言います。 We say that a two-sided ideal $\mathfrak{a}$ of A is nilpotent if there exists an integer $n\geqslant 1$ such that $\mathfrak{a}^n= 0$, that is (I, §8, No. 9, p. 107), such that we have $x_1\cdots x_n= 0$ for every sequence $(x_1, . . . , x_n)$ of elements of $\mathfrak{a}$. すべてのゼロイデアルはゼロイデアルですが、ゼロイデアルには含まれないゼロイデアルが存在する可能性があります (VIII、p. 167、練習問題 9)。

#### 定理 1 (ジェイコブソン) {#alg-viii-s9-thm-1 .statement tag=00S5}

環 A の根基は、$1 +ax$ が $a\in A$ ごとに反転可能なまま (I, §2, No. 3、p. 15) になるように、元 $x\in A$ で構成されます。また、$1 +x$ が $x\in \mathfrak{a}$ ごとに反転できるような最大の両面イデアル $\mathfrak{a}$ でもあります。 含むの根基 A のすべての左の nil 理想。

元 1 生成する A-加群 $A_s$、および $1 +ax$ は、生成する A-加群 $A_s$ の場合に限り、反転可能のままになります。従って、定理 1 の最初の主張は、命題 2 (VIII、p. 153) の系の特定のケースになります。

$x\in \mathfrak{R}(A)$ にしましょう。上記により、$1 +x$ は反転可能なままになります。 $y$ を A の元とし、$y(1 +x) = 1$ とします。次に、$1-y=yx$ があるため、$1-y$ 属するから $\mathfrak{R}(A)$ になります。従って、$y$ は反転可能なままになります。 $y$ も右反転であるため、これは反転可能 (I, §2, No. 3、p. 16、命題 3) であり、その右反転 $1 +x$ も同様です。

$\mathfrak{a}$ を、$1 +x$ がすべての $x\in \mathfrak{a}$ に対して可逆であるような A の左イデアルとする。これは、例えば、関係 $x^n= 0$ は $1-x+\cdots + (-x)^{n-1}$ が $1 +x$ の逆数であることを意味するため、$\mathfrak{a}$ が nil イデアルである場合に当てはまります。 $x\in \mathfrak{a}$ にしましょう。 $a\in A$ ごとに $ax\in \mathfrak{a}$ があるため、$1 +ax$ は反転可能です。従って、$x\in \mathfrak{R}(A)$ となります。 $\mathfrak{a}$は$\mathfrak{R}(A)$に含まれることになります。

#### 系 1 {#alg-viii-s9-thm-1-cor-1 .statement tag=00AG}

A の根基は、反対環 $A^o$ の根基、つまり A の最大右イデアの共通部分に等しい。

すべての $x\in \mathfrak{R}$(A) について、$1 +x$ は環 A で反転可能であるため、環 $A^o$ では反転可能です。 $\mathfrak{R}(A)$は$A^o$の両面理想なので、$\mathfrak{R}(A)\subset \mathfrak{R}(A^o)$になります。 等式の後に、交換すること A と $A^o$ の役割が続きます。

#### 系 2 {#alg-viii-s9-thm-1-cor-2 .statement tag=00AH}

A の元は、環 $A/\mathfrak{R}(A)$ の標準像が可逆である場合に限り、可逆です。

条件は明らかに必要です。それが十分であることを証明しましょう。 $x$ を、環 $A/\mathfrak{R}(A)$ の標準像が可逆である A の元とします。すると、$xy$ 属するから $1 +\mathfrak{R}(A)$ となるような A の元 $y$ が存在します。 定理までに 1$,xy$ は反転可能です。従って、$x$ は右反転可能です。 $x$ が反転可能なままである証明も同様です。

#### 系 3 {#alg-viii-s9-thm-1-cor-3 .statement tag=00AI}

家族の積の根基、環の$(A_i)_{i\in I}$は、$\mathfrak{R}(A_i)$の積です。

$x= (x_i)_{i\in I}$を$\prod_{i\in I}A_i$の元とします。 $\prod_{i\in I}A_i$ のすべての元 $a= (a_i)_{i\in I}$ について、元 $1 +ax$ は、$i\in I$ ごとに $A_i$ で$1 +a_ix_i$ が反転可能なままである場合に限り、反転可能なままになります。 系 3が続きます。

#### 系 4 {#alg-viii-s9-thm-1-cor-4 .statement tag=00AJ}

環 A は、環 $A/\mathfrak{R}(A)$ が体である場合にのみローカルです。この場合、$\mathfrak{R}(A)$はAの非可逆元の集合になります。

A の非可逆元の集合を $\mathfrak{r}$ で表します。 環 A がローカルの場合、その根基は $\mathfrak{r}$ (VIII、p. 154、例 1) に等しく、環 $A/\mathfrak{r}$ は体 (VIII、p. 26) です。逆に、環 $A/\mathfrak{R}(A)$ が体であるとします。 系 2 までに、$\mathfrak{r}=\mathfrak{R}$(A) が得られるため、$\mathfrak{r}$ は A の両側イデアルです。したがって、環 A は局所的です (VIII, p. 26, 定義 1)。

#### 例 4 {#alg-viii-s9-n2-exa-4 .statement tag=00AK}

K を整域、I 空でない集合、A を多項式環 $K[X_i]_{i\in I}$ とします。 環 A には根基が存在しないことを証明しましょう。 A の可逆元は K の可逆元 (IV, §1, No. 5、p. 9、系 2) だけです。 $f\in \mathfrak{R}(A)$ にしましょう。 選ぶ元 $i\in I$。このとき、$1 +fX_i$ は可逆 (定理 1) であり、これは $f= 0$ を意味します。

K が可換体のとき、環 $A = K[X_i]_{i\in I}$ は $B = K[[X_i]]_{i\in I}$ の部分環であり、$\mathfrak{R}(A) = 0$ と $A\cap \mathfrak{R}(B)\not= 0$ (cf. VIII, p. 154, 例 2) があることに注意してください。

#### 例 5 {#alg-viii-s9-n2-exa-5 .statement tag=00AL}

$\mathfrak{a}$ を A の両側イデアルとします。 A の $\mathfrak{a}$ 進数位相は、A の環構造と互換性のある位相であり、イデアル $\mathfrak{a}^n$ ($n\geqslant 1$ の場合) 形は 0 の近傍の基本系です。 (将軍トップ、III, §6, No. 3、p. 275、例 3)。 環 A がハウスドルフであり、この位相に対して完全 (Gen. Top.、III, §6, No. 5、p. 276) であるとします。これは、たとえば、イデアル $\mathfrak{a}$ が零能である場合に当てはまります。 $x\in \mathfrak{a}$ ごとに、系列 $\sum^{\infty}_{n=0}(-x)^n$ が収束します。 $y$ をその和とします。 $y-1 =\sum^{\infty}_{n=1}(-x)^n=-xy$があるので、$(1 +x)y= 1$です。同様に、$y(1 +x) = 1$があるので、$1 +x$は反転可能です。 定理 1 により、理想的な $\mathfrak{a}$ は A の根基に含まれることになります。

#### 注意 1 {#alg-viii-s9-n2-rem-1 .statement tag=00AM}

定理 1 までに、環 A の左の nil イデアルはすべて、

根基です。 $x$ をゼロポテントで A の中心となる元とします。その場合、$Ax$ は A の nil イデアルなので、A の $x$ 属するから根基になります。ただし、A の非零冪零元は存在しますが、A には根基が存在しない可能性があります。たとえば、体上のすべての整数 $n\geqslant 2$、行列環 $\mathbf{M}_n(K)$ について、K は単純なので、根基 (VIII、p. 154、命題 4) がなければ、含む冪零元、たとえば行列単位 $E_{ij}$ と $i\not=j$。

#### 注意 2 {#alg-viii-s9-n2-rem-2 .statement tag=00AN}

A を可換環とします。 The set of nilpotent elements $a$ of A is an ideal $\mathfrak{N}(A)$ of A, called the nilradical of A; it is the intersection of the prime ideals of A (V, §15, No. 1, p. 118, Proposition 2). We have $\mathfrak{N}(A)\subset \mathfrak{R}(A)$; $*$we have equality if A is an Artinian ring (VIII, p. 173, Corollary 2) or a finitely generated commutative algebra over a commutative field (Comm. 代数、V, § 3、n$^{\circ}4$、定理 $3$)$*$。 確かに$\mathfrak{N}(A)\not=\mathfrak{R}(A)$を得ることができます。 これは、A が環 K[[X]]、K が可換体の場合に当てはまります。その場合、$\mathfrak{N}(A) = 0$ と $\mathfrak{R}(A) =$ AX (VIII, p. 154, 例 2) が得られます。

### 3. 中山さんの補題

#### 命題 6 {#alg-viii-s9-prop-6 .statement tag=00AO}

A-加群 M ごとに、$\mathfrak{R}(A)M\subset \mathfrak{R}(M)$ が得られます。 A-加群 M が射影の場合、等式が得られます。

P を M の極大部分加群とします。 A-加群 $M/P$ は単純なので、VIII、p. 155 の命題 5 によって $\mathfrak{R}(A)$ によって消滅します。したがって、M の極大部分加群 P ごとに $\mathfrak{R}(A)M\subset P$ があり、したがって $\mathfrak{R}(A)M\subset \mathfrak{R}(M)$ になります。

明らかに$\mathfrak{R}(A_s) =\mathfrak{R}(A)A_s$ があります。 A-加群 M が射影である場合、$M\oplus N$ が自由であるような A-加群 N が存在します。つまり、加群が $A_s$ と同型である族 $(L_i)_{i\in I}$ の直和が存在します。 VIII、p. 152 の系 2 までに、$\mathfrak{R}(M\oplus N) =\mathfrak{R}(M)\oplus \mathfrak{R}(N)$ と $\mathfrak{R}(\bigoplus_{i\in I}L_i)=\bigoplus_{i\in I}\mathfrak{R}(L_i)$ ができます。次に、等式 $\mathfrak{R}(L_i) =\mathfrak{R}(A)L_i$ から $\mathfrak{R}(M) =\mathfrak{R}(A)M$ を導き出します。

#### 定理 2 (「中山の補題」) {#alg-viii-s9-thm-2 .statement tag=00S6}

M を A-加群および A の両側イデアルである $\mathfrak{a}$ とします。次の条件のいずれかが満たされるとします。

(i) A-加群 M は有限生成され、A の根基には $\mathfrak{a}$ が含まれる。

(ii) 理想 $\mathfrak{a}$ は無能です。

N が $M = N +\mathfrak{a}M$ となる M の部分加群である場合、N = M になります。特に、加群 M が非零である場合、$M\not=\mathfrak{a}M$ になります。

M が有限に生成され、$\mathfrak{a}\subset \mathfrak{R}(A)$ があると仮定します。 N を M の部分加群とし、$M = N +\mathfrak{a}M$ とします。 命題 6 により、$M = N +\mathfrak{R}$(M) が得られるため、命題 2、b) VIII、p. 153 により M = N となります。

ここで、$\mathfrak{a}$ が零能であると仮定し、N を $M = N +\mathfrak{a}M$ となるような M の部分加群とします。 整数 $n\geqslant 0$ 帰納法までに、関係 $M = N +\mathfrak{a}^nM$ を確立します。 仮定までに、$\mathfrak{a}^n= 0$ となるような整数 $n\geqslant 0$ が存在します。したがって、M = Nです。

定理の最後の主張は、N を 0 として上記から導き出されます。

#### 系 1 {#alg-viii-s9-thm-2-cor-1 .statement tag=00R9}

定理の仮定を保持します。 2. $(x_i)_{i\in I}$ を M の元の家族とし、$\overline{x}_i$ を $M/\mathfrak{a}M$ の $x_i$ の標準像とします。ファミリ $(\overline{x}_i)_{i\in I}$ 生成するが $(A/\mathfrak{a})$ モジュール $M/\mathfrak{a}M$ の場合、ファミリ $(x_i)_{i\in I}$ 生成する A-加群 M.

これは、ファミリー $(x_i)_{i\in I}$ によって生成された M の部分加群 N に適用される定理 2 から続きます。

#### 系 2 {#alg-viii-s9-thm-2-cor-2 .statement tag=00AP}

定理 2 の仮定を維持します。さらに、$M'$ を A-加群、$u: M'\rightarrow M$ を準同型とします。 移行から商によって $u$ から推定される $M'/\mathfrak{a}M'$ から $M/\mathfrak{a}M$ の準同型 $\overline{u}$ が全射である場合、$u$ は全射です。

確かに、$u:$の像に定理を適用する2を加えるだけで十分です。実際、$\overline{u}$の像は$(N +\mathfrak{a}M)/\mathfrak{a}M$なので、$N +\mathfrak{a}M = M$がある場合に限り、$\overline{u}$は全射になります。

### 4. 冪等の持ち上げ

#### 補題 1 {#alg-viii-s9-lem-1 .statement tag=00AQ}

$a$ を環 A の元とし、$a-a^2$ がゼロになるようにします。 $X + (X-X^2)\mathbf{Z}[X]$ には、$P(a)$ が A において冪等であるような多項式 P が存在します。

$n$ を、$(a-a^2)^n= 0$ となるような厳密な正の整数とします。 集合 P(X) = $1-(1-X^n)^n$。多項式 P(X) は $X^n$ の倍数であり、多項式 $1-P(X)$ は $(1-X)^n$ の倍数であるため、$P(X)-P(X)^2$ は $(X-X^2)^n$ の倍数であり、次のようになります。 $P(a) = P(a)^2$。さらに、$X-P(X)$はXと$1-X$の倍数なので、$X-X^2$の倍数です。

#### 命題 7 {#alg-viii-s9-prop-7 .statement tag=00AR}

$\mathfrak{a}$ を A の両側ゼロイデアルとし、$\overline{e}$ を環 $A/\mathfrak{a}$ の冪等とする。 A には、$A/\mathfrak{a}$ の標準像が $\overline{e}$ に等しい冪等 $e$ が存在します。

$a$ を A の $\overline{e}$ の任意の代表とします。A の元 $a-a^2$ は、属するから $\mathfrak{a}$ であるため、零能です。 選ぶ多項式 $P\in \mathbf{Z}[X]$ 満たす条件 of 補題 1. $a-P(a)\in A(a-a^2)$ があるので、A の元 $e= P(a)$ は所望の性質になります。

環 $A/\mathfrak{a}$ の $\overline{e}$ 属するから中心とします。 $\overline{e}$ (VIII、p. 172、練習問題 31) をリフティングする A の中心 Z には冪等 $e$ が必ずしも存在するわけではありません。ただし、$A/\mathfrak{a}$ の Z の像に対して $\overline{e}$ 属するの場合、$Z\cap \mathfrak{a}$ は Z のゼロイデアルであるため、Z の冪等には持ち上げになります。

#### 系 1 {#alg-viii-s9-prop-7-cor-1 .statement tag=00AS}

P から M までの M と P を A-加群と $u$ 全射A-線型写像とします。 Suppose that P is projective and that there exists a nilpotent two-sided ideal $\mathfrak{a}$ of A such that the kernel N of $u$ is contained in $\mathfrak{a}P$. $M'$ と $M''$ を、直和が M である M の部分加群とします。 この場合、P は部分加群 $P'$ と $P''$ の直和となり、$u(P') = M'$ と $u(P'') = M''$ になります。

B 部分環 of End$_A(P)$ からなる of 自己準同型 $f$ $f(N)\subset N$ となるように表します。 $\overline{B}$ を M の自己準同型環とします。$f\in B$ について、$\overline{f}$ を M の一意な自己準同型とし、$\overline{f}\circ u=u\circ f$ とします。 写像 $f\mapsto \overline{f}$ は、B から B への環準同型です。 加群 P は射影であるため、この準同型は全射です。その核 $\mathfrak{b}$ は自己準同型 $f\in B$ で構成され、$f(P)\subset N$ になります。 $n$ を自然数とし、$\mathfrak{a}^n= 0$ とします。我々は持っています

$$
P =\mathfrak{a}^0P\supset \mathfrak{a}^1P\supset  \cdots  \supset \mathfrak{a}^{n-1}P\supset \mathfrak{a}^nP = 0
$$

そして、$f\in \mathfrak{b}$ および整数 $j\geqslant 0$ ごとに、

$$
f(\mathfrak{a}^jP) =\mathfrak{a}^jf(P)\subset \mathfrak{a}^jN\subset \mathfrak{a}^{j+1}P
$$

なぜなら$N\subset \mathfrak{a}P$ by 仮定だからです。したがって、すべての自然数 $j$ とすべての $f\in \mathfrak{b}^j$ に対して $f(P)\subset \mathfrak{a}^jP$ が存在します。特に$\mathfrak{b}^n= 0$があります。

$\varepsilon '$ を、像 $M'$ と核 $M''$ を含む M の射影子とします。 命題 7 を環 B と冪能の両側イデアル $\mathfrak{b}$ に適用すると、$\overline{e'}=\varepsilon '$、つまり $\varepsilon '\circ u=u\circ e'$ となる冪等 $e'$ が B に存在します。 集合 $e''= 1-e'$、$\varepsilon ''=\overline{e''}, P'=e'$(P)、$P''=e''(P)$。すると、P は部分加群 $P'$ と $P''$ の直和となり、次のようになります。

$$
u(P') =u(e'(P)) =\varepsilon '(u(P)) =\varepsilon '(M) = M'
$$

等式 $u(P'') = M''$ も同様に証明されます。

#### 系 2 {#alg-viii-s9-prop-7-cor-2 .statement tag=00AT}

A を環とし、$\mathfrak{a}$ を A の冪能双辺イデアルとします。 P が射影 A-加群の場合、$P/\mathfrak{a}P$ は $A/\mathfrak{a}$ 上で射影加群であり、$A/\mathfrak{a}$ 加群の場合に限り、A-加群 P は分解不可能です$P/\mathfrak{a}P$は不分解です。

P を射影 A-加群とし、$\overline{P}$ を $A/\mathfrak{a}$ 加群 $P/\mathfrak{a}P$ とします。 The A-module P is zero if and only if $\overline{P}$ is zero (Theorem 2 of VIII, p. 158). ここで、$P\not= 0$ と仮定します。 $A/\mathfrak{a}$加群 P は $\overline{A}\otimes_AP$ と同型であるため、射影 (命題 4 の II, §5, No. 1、p. 279、系) です。 P が分解不可能であれば、$\overline{P}$ by 系 1 も分解不可能です。 逆に、P が分解可能で非零であると仮定し、$P'$ と $P''$ を $P = P'\oplus P''$ となるような P の 2 つの非零部分加群とします。 中山の補題 (VIII、p. 158、定理 2) により、$P'+\mathfrak{a}P\not= P$ と $P''+\mathfrak{a}P\not= P$ が得られます。 $\overline{P}'$ と $\overline{P}''$ が P の $P'$ と $P''$ の標準像である場合、$\overline{P}'\not= P,\overline{P}''\not= P$ と $\overline{P}=\overline{P}'\oplus \overline{P}''$ があります。 これは、$\overline{P}$ が分解可能であることを証明しています。

### 5. 加群の投影カバー

#### 定義 3 {#alg-viii-s9-def-3 .statement tag=00AU}

Aを環、MをA-加群とします。 M の射影カバーは対 $(P, u)$ で、P は P から M への射影 A-加群と $u$ 全射準同型であり、P のすべての適切な A-部分加群 $P'$ に対して $u(P')\not= M$ が得られます。

#### 注意 1 {#alg-viii-s9-n5-rem-1 .statement tag=00AV}

すべての射影 A-加群 M に対して、対 $(M,1_M)$ は M の射影カバーです。

#### 注意 2 {#alg-viii-s9-n5-rem-2 .statement tag=00AW}

$(P, u)$ が A-加群 M の射影カバーであるとします。 $(x_i)_{i\in I}$ を P の元の族とし、$P'$ を P の部分加群として、生成するとします。次に、$u(P')$ はファミリー $(u(x_i))_{i\in I}$ によって生成されます。従って、家族 $(x_i)_{i\in I}$ 生成する A-加群 P は、家族 $(u(x_i))_{i\in I}$ 生成する A-加群 M の場合に限り、M が有限に生成される場合に限り、P は有限に生成されます。

#### 命題 8 {#alg-viii-s9-prop-8 .statement tag=00AX}

M と $M'$ を、それぞれ M と $M'$ の射影カバー A-加群、$(P, u)$、$(P', u')$、および $g: M\rightarrow M'$ A-線型写像とします。

a) $u'\circ f=g\circ u$ となるような A-線型写像 $f: P\rightarrow P'$ が存在します。

b) $f$ をそのような写像とします。 $g$ が全射（それぞれ全単射）の場合、$f$ は全射（それぞれ全単射）です。 $g$ が単射であり、その像が $M'$ の直因子である場合、$f$ は単射であり、その像は $P'$ の直因子です。

仮定により、A-加群 P は射影的であり、写像 $u'$ は全射的です。従って、$g\circ u=u'\circ f$ (II, §2, No. 2, p. 231, 命題 4) となるような A-線型写像 $f: P\rightarrow P'$ が存在します。 主張 a) が続きます。

a)と同様に$f$を写像とします。 $g$ が全射であると仮定します。 $u$は全射なので、$M'=g(u(P)) =u'(f(P))$になります。 $(P', u')$ は M’ の射影カバーなので、$f(P) = P'$ があり、$f$ は全射です。ロケ地にて。前掲書、$f$ の核は補部分加群 $P_1$ を認めるので、$f(P_1) = P'$ になります。ここで、$g$ が全単射であると仮定します。 $g(u(P_1)) =u'(f(P_1)) =u'(P') = M'$があるので、$u(P_1) = M$です。 $(P, u)$ は M の射影カバーなので、$P_1= P$ があり、従って Ker($f$) $= 0$ となります。従って、$f$ は単射法です。 $f$ が全単射であることはすでにわかっているので、$f$ は全単射です。

結論するに対して、$g$ が単射であり、その像が $M'$ の直因子であると仮定します。すると、$g'\circ g= 1_M$ となるような A-線型写像 $g': M'\rightarrow M$ が存在します。 a) により、$u\circ f'=g'\circ u'$ となるような A-線型写像 $f': P'\rightarrow P$ が存在します。 $u\circ (f'\circ f) =g'\circ u'\circ f= (g'\circ g)\circ u$ があります。前の段落で、写像 $f'\circ f$ は全単射です。 逆全単射を $h$ で表します。 $(h\circ f')\circ f= 1_P$ があるので、$f$ は単射であり、その像は $P'$ の直因子 (II, §1, No. 9, p. 212, 系 2) です。

#### 系 1 {#alg-viii-s9-prop-8-cor-1 .statement tag=00AY}

M をA-加群とします。 $(P, u)$ と $(P', u')$ を M の射影覆いとします。 P から $P'$ まで、$u=u'\circ f$ となるような同型 $f$ が存在します。

$f$ は、関係 $u=u'\circ f$ (VIII、p. 170、練習問題 21) によって必ずしも一意に決定されるわけではないことに注意してください。

#### 系 2 {#alg-viii-s9-prop-8-cor-2 .statement tag=00AZ}

$(P, u)$ を A-加群 M の射影カバーとします。Q が射影 A-加群で、$g: Q\rightarrow M$ が全射線形写像である場合、$g=u\circ f$ のような全射線形写像 $f: Q\rightarrow P$ が存在します。

#### 命題 9 {#alg-viii-s9-prop-9 .statement tag=00B0}

M を A-加群および M の射影カバーである $(P, u)$ とします。環 A の根基を $\mathfrak{r}$ で表します。 準同型 $\overline{u}: P/\mathfrak{r}P\rightarrow M/\mathfrak{r}M$ から移行によって$u$ から商を推定すると、同型になります。

準同型 $u$ は定義により全射なので、$\overline{u}$ は全射です。 $u$の核をNで表します。$u^{-1}(\mathfrak{r}M) = N +\mathfrak{r}P$があります。 $\overline{u}$ の単射性を意味する $N\subset \mathfrak{r}P$ があることを証明しましょう。 P のすべての極大部分加群 $P'$ に対して、$u(P')\not= M$ があり、したがって $P'+ N\not= P$ になります。 $P'$ が最大なので、$N\subset P'$ になります。したがって、P の部分加群 N は、P の根基に含まれます。ここで、後者は、VIII、p. 158 の命題 6 により、$\mathfrak{r}P$ に等しくなります。

#### 系 {#alg-viii-s9-n5-cor-1 .statement tag=00B1}

A-加群 M に突起カバーがある場合、$A/\mathfrak{r}$ モジュール $M/\mathfrak{r}M$ は突起です。

実際、$(P, u)$ が M の射影カバーである場合、$(A/\mathfrak{r}$) 加群 $M/\mathfrak{r}M$ は $P/\mathfrak{r}P$ (命題 9) と同型です。 A-加群 P は射影であるため、$(A/\mathfrak{r}$) 加群 $P/\mathfrak{r}P$ も射影です。

#### 注意 3 {#alg-viii-s9-n5-rem-3 .statement tag=00B2}

環 A に根基がないとします。 $u$ が同型である場合に限り、命題 9 までに、$(P, u)$ は A-加群 M の射影カバーになります。したがって、射影カバーは射影 A-加群に対してのみ存在できます。

環 $\mathbf{Z}$ には根基 (VIII、p. 154、例 3) がありません。 $n\geqslant 2$を整数とします。 $\mathbf{Z}$ モジュール $\mathbf{Z}/n\mathbf{Z}$ は投影型ではないため、投影型カバーを使用できません。

#### 注意 4 {#alg-viii-s9-n5-rem-4 .statement tag=00B3}

すべての有限生成A-加群に投影カバーがあると仮定します。すると、A の商 $A'$ は、その根基によって半単純になります。実際、環 $A'$ 上のすべての有限生成加群は系によって射影されます。特に、$A'$ のすべての左イデアル $\mathfrak{a}$ について、$A'$ 加群 $A'_s/\mathfrak{a}$ は射影的です。次に、主張は、VIII、p. 138 の命題 4 から続きます。

$A/\mathfrak{r}$ が半単純である可換環 A の例と射影カバーを認めない有限生成A-加群 M の例 (VIII, p. 170, 練習問題 22) を与えることができます。

#### 命題 10 {#alg-viii-s9-prop-10 .statement tag=00B4}

M を A-加群、P を射影 A-加群、および $u: P\rightarrow M$ 線形写像とします。 $\mathfrak{a}$ を A の両側イデアルとします。 移行によって $u$ から商まで推定される線形写像 $\overline{u}: P/\mathfrak{a}P\rightarrow M/\mathfrak{a}M$ が全単射であり、次の条件のいずれかが満たされるとします。

(i) A-加群 M と P は有限生成され、A の根基には $\mathfrak{a}$ が含まれます。

(ii) 理想 $\mathfrak{a}$ は無能です。

続いて$(P, u)$はMの射影カバーです。

仮定では、準同型 $u$ は全射法 (VIII、p. 159、系 2) であり、その核 N は $\mathfrak{a}P$ に含まれます。 $P'$ を P の真部分加群とします。中山の補題 (VIII, p. 158, 定理 2) により、$P'+\mathfrak{a}P\not= P$ となり、したがって $u(P')\not= M$ となります。つまり、$(P, u)$ は M の投影カバーです。

#### 系 1 {#alg-viii-s9-prop-10-cor-1 .statement tag=00B5}

P を射影 A-加群とします。 P が有限に生成される、または A の根基 $\mathfrak{r}$ が冪能の両側イデアルであると仮定します。 P から標準写像を $u$ で $P/\mathfrak{r}P$ と表します。そして$(P, u)$は$P/\mathfrak{r}P$の射影カバーです。

#### 系 2 {#alg-viii-s9-prop-10-cor-2 .statement tag=00B6}

$\mathfrak{a}$ を、$(A/\mathfrak{a})$ モジュール $M/\mathfrak{a}M$ が自由になるような A と M の両側イデアル A-加群とします。次の条件のいずれかが満たされると仮定します。

(i) 加群 M は有限生成され、A の根基には $\mathfrak{a}$ が含まれる。

(ii) 理想 $\mathfrak{a}$ は無能です。

それからMには突起カバーがあります。

More precisely, let P be a free A-module, $(e_i)_{i\in I}$ a basis of P, and let $u: P\rightarrow M$ be a homomorphism such that the canonical images of the elements $u(e_i)$ of $M/\mathfrak{a}M$ form a basis of the $(A/\mathfrak{a})$-module $M/\mathfrak{a}M$. そして$(P, u)$はMの投影カバーです。

$(A/\mathfrak{a}$) モジュール $P/\mathfrak{a}P$ は無料で、$P/\mathfrak{a}P$ から $M/\mathfrak{a}M$ までの準同型 $\overline{u}$ は、移行から商によって $u$ から推定され、$P/\mathfrak{a}P$ の変換基底になります。 $M/\mathfrak{a}M$ の基底になるため、全単射です。

$\mathfrak{a}$ が零能である場合、命題を適用する 10 で十分です。 ここで、環 A が非零であり、加群 M が有限生成されると仮定します。 $(A/\mathfrak{a}$) モジュール $M/\mathfrak{a}M$ も同様であり、その結果、$(A/\mathfrak{a}$) モジュール $P/\mathfrak{a}P$ も同様です。 $P/\mathfrak{a}P$ のすべての基底は有限になります。従って、集合 I は有限であり、A-加群 P は有限に生成されます。その後、再び命題を適用する 10 になります。

#### 系 3 {#alg-viii-s9-prop-10-cor-3 .statement tag=00B7}

局所環上のすべての有限生成加群には突起カバーがあります。

Aを局所環、$\mathfrak{r}$を根基とします。 A (VIII, p. 155, 命題 5, a)) の両面理想であり、環 $A/\mathfrak{r}$ は体 (VIII, p. 157, 系 4) です。 M が A-加群の場合、$M/\mathfrak{r}M$ は体 $A/\mathfrak{r}$ よりもベクトル空間であるため、自由な $(A/\mathfrak{r}$) モジュールになります。その場合、系を適用する 2 で十分です。

#### 注意 5 {#alg-viii-s9-n5-rem-5 .statement tag=00B8}

Aを局所環、$\mathfrak{r}$を根基とします。 M を有限生成A-加群、P を有限生成射影 A-加群、および $u: P\rightarrow$ M 準同型とします。 系 VIII、p. 36、A-加群の 6 までに P が無料になります。 P. 集合 $x_i=u(e_i)$ の選ぶ基底 $(e_i)_{i\in I}$、$M/\mathfrak{r}M$ の $x_i$ の標準像を $\overline{x}_i$ で示します。次のプロパティは同等です。

(i) 対 $(P, u)$ は M の射影カバーです。

(ii) 家族 $(x_i)_{i\in I}$ は、A-加群 M の最小生成する家族です。

(iii) 家族 $(\overline{x}_i)_{i\in I}$ は、体 $A/\mathfrak{r}$ 上のベクトル空間 $M/\mathfrak{r}M$ の基底です。

(i) $\Rightarrow$ (ii) VIII、p. 161 の注意 2 によるもの、および (iii) $\Rightarrow$ (i) 系 2 によるものがあります。 さらに、家族 $(x_i)$ が A-加群 M の最小生成する家族である場合、家族は$(\overline{x}_i)$ は最小の生成するファミリ、つまりベクトル空間 $M/\mathfrak{r}M$ の $A/\mathfrak{r}$ (VIII、p. 158、系 1) の基底です。

#### 命題 11 {#alg-viii-s9-prop-11 .statement tag=00B9}

A を環および $\mathfrak{a}$ として A の冪能両側イデアルとします。M を射影 $A/\mathfrak{a}$ 加群とします。 核 $\mathfrak{a}P$ を伴う射影 A-加群 P と全射A-線型写像 $u: P\rightarrow M$ が存在します。

このような対 $(P, u)$ は、A-加群として見た M の投影カバーです。

$M\oplus M'$ が空き $A/\mathfrak{a}$ モジュールであるような $A/\mathfrak{a}$ モジュール $M'$ が存在します。 選ぶ自由A-加群 L および全射A-線型写像 $v: L\rightarrow M\oplus M'$ と核 $\mathfrak{a}L$。 命題 7 (VIII, p. 159) の系 1 までに、$v(P) = M$ と $v(P') = M'$ のような直和分解 $L = P\oplus P'$ が存在します。 A-加群 P は射影であり、P から M までの A-線型写像 $u$ は、P に $v$ が付いている一致するは、核 $\mathfrak{a}P$ と全射です。最初の主張が続きます。

P を、核 $\mathfrak{a}P$ による P から M への射影 A-加群および $u$ 準同型とする。 命題 10 までに、対 $(P, u)$ は M の投影カバーです。

#### 系 {#alg-viii-s9-n5-cor-2 .statement tag=00RA}

P と $P'$ を射影 A-加群とします。 加群 $P/\mathfrak{a}P$ と $P'/\mathfrak{a}P'$ が同型である場合、P と $P'$ は同型です。

$P/\mathfrak{a}P$ と $P'/\mathfrak{a}P'$ は射影であるため、射影カバー (VIII、p. 162、系 1) の命題 11 と一意性から系が続きます。

### 練習問題 {#alg-viii-s9-exercises}

[§ 9 に対して練習問題](exercises/s9/)を参照してください。
