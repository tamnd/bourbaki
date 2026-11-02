---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 5
section_title: Commutation
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.77-A VIII.94
pdf_pages: 0094-0111
extraction: native
subsections:
    - "no": 1
      title: The Commutant and Bicommutant of a Module
      page: 77
      pdf_page: 94
    - "no": 2
      title: Generating Modules
      page: 79
      pdf_page: 96
    - "no": 3
      title: The Bicommutant of a Generating Module
      page: 82
      pdf_page: 99
    - "no": 4
      title: The Countermodule of a Semisimple Module
      page: 84
      pdf_page: 101
    - "no": 5
      title: Density Theorem
      page: 88
      pdf_page: 105
    - "no": 6
      title: Application to Field Theory
      page: 89
      pdf_page: 106
statements: 37
exercises: 19
content_sha256: 7a6d342e21ca1a69283cee0417c1717b1609437a999544db1d642892e960f92f
translated_from: content/en/alg/VIII/05_s5_commutation.md
translation_method: google
source_content_sha256: 92146afa3071a759dfd60b0a1909d5b82cb570c6ed50a098e57fa1acd8ea9c00
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: a04b0cb03bd246e73498e9023e6ebcd8e980db267c56b1670c1260a8468140c9
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 5。 交換

### 1. 加群の交換子環と双可換子

EをEの環、BをEの部分集合とします。 The commutant (or centralizer) of B in E is the subring $B'$ of E consisting of the elements that commute with every element of B. $B'$ の交換子環 $B''$ は、B の双可換子 (またはバイセントラライザー) と呼ばれます。 $B\subset B''$、$B'$ 一致するとその双可換子 (III, §1, No. 2、p. 429) があります。 The center of a subring B of E is $B\cap B'$; the common center of $B'$ and $B''$ is $B'\cap B''$. B が E の可換部分環である場合、$B\subset B'$ があり、$B''$ は $B'$ (III, §1, No. 2, p. 430) の中心です。

A を環、M を左 (それぞれ右) A-加群とします。 これらの定義を、E が M の加法群の自己準同型環と、B が M の相同性 $A_M$ の環である場合に適用してみましょう。 E の $A_M$ の交換子環 $A'_M$ は M の交換子環と呼ばれます。 A-加群Mの自己準同型環です。 Eの$A_M$の双可換子$A''_M$はMの双可換子と呼ばれます。 M の対加群の自己準同型環 (VIII、p. 8、定義 3) です。 $A_M\subset A''_M$、環 $A_M\cap A'_M$ は $A_M$ の中心 、$A'_M\cap A''_M$ は $A'_M$ と $A''_M$ の共通中心です。

#### 定義 1 {#alg-viii-s5-def-1 .statement tag=005E}

A-加群 M は、$A_M= A''_M$ があればバランスが取れています。

A-加群 M のバランスが取れている場合、環 $A_M$ と $A'_M$ は同じ中心 $A_M\cap A'_M$ を持ちます。 加群 M は、平衡型 $A_M$ モジュールである場合に限り、平衡型 A-加群です。 対加群の A-加群 M は忠実でバランスが取れています。

When the ring A is commutative, the bicommutant $A''_M$ of M is the center of $A'_M=$ End$_A(M)$; that M is balanced means that the center of End$_A(M)$ is reduced to the homotheties.

A の任意の元 $a$ について、A から A までの右側のホモテティー $x\mapsto xa$ を $\boldsymbol{\delta }_a$ で表し、左側のホモテティー $x\mapsto ax$ (I, §8, No. 1、p. 97) を $\boldsymbol{\gamma }_a$ で表します。 写像 $a\mapsto \boldsymbol{\delta }_a$ は、左A-加群 $A_s$ の$A^o$ から交換子環までの環同型です（cf. II, §10, No. 7、p. 349、$I =\{1\}$ に適用）。 写像 $a\mapsto \boldsymbol{\gamma }_a$ は、右A-加群 $A_d$ の A から交換子環までの環同型です (上記参照)。この写像を介して$A_d$の交換子環と同一視するAを結合すると、$A_d$の対加群は$A_s$と識別されます。従って、A-加群 $A_d$ はバランスが取れています。同様に、A-加群 $A_s$ もバランスがとれています。

$n$ を整数 $\geqslant 1$ とします。 $A^n$ を左の $\mathbf{M}_n$(A) モジュールと見なします (上記参照)。 A-加群 $A^n_d$ の自己準同型 $x\mapsto mx$ に $m\in \mathbf{M}_n(A)$ を送る写像は、右A-加群 $A^n_d$ の $\mathbf{M}_n(A)$ から交換子環までの環同型です (loc.引用）。

#### 命題 1 {#alg-viii-s5-prop-1 .statement tag=005F}

$(A_i)_{i\in I}$ を環のファミリーとし、すべての $i\in I$ に対して、$M_i$ を $A_i$ モジュールとします。 集合 $A =\prod A_i,M =\prod M_i$、および $N =\bigoplus M_i$。 Endow M with the structure of an A-module with law of action $((a_i),(x_i))\mapsto (a_ix_i)$. 集合 N は M の A-部分加群です。

a) 写像 $(u_i)\mapsto \prod u_i$ $\prod$ 終了$_{\mathbf{Z}}(M_i)$ から終了$_{\mathbf{Z}}(M)$ (II, §1, No. 5、p. 200) 制限するから環同型 $\prod(A_i)_{M_i},\prod(A_i)'_{M_i}$ および$\prod(A_i)''_{M_i}$ からそれぞれ$A_M,A'_M$、$A''_M$。

b) 写像 $(u_i)\mapsto \bigoplus u_i$ $\prod$ 終了$_{\mathbf{Z}}(M_i)$ から終了$_{\mathbf{Z}}(N)$ (II, §1, No. 6、p. 203) 制限するから環同型 $\prod(A_i)_{M_i},\prod(A_i)'_{M_i}$ および$\prod(A_i)''_{M_i}$ からそれぞれ$A_N,A'_N$、$A''_N$。

命題 1 で定義された環同型は正規と呼ばれます。 積 $\prod(A_i)_{M_i}$ は、同型を通じて、$A_M$ と、$\prod(A_i)'_{M_i}$ は $A'_M$ などと同一視されることがよくあります。

$\prod$ 終わり$_{\mathbf{Z}}(M_i)$ から終わり$_{\mathbf{Z}}(M)$ までの写像 $\varphi : (u_i)\mapsto \prod u_i$ は単射環準同型です。 M の A-加群構造の定義までに、$\varphi (\prod(A_i)_{M_i}) = A_M$ になります。 $u\in A'_M$ にしましょう。すべての $i\in I$ について、 A の $h_i$ 元で表します。ただし、 0 に等しい添字 $i$ を除き、すべての成分は 1 に等しくなります。 $x$ が M の元で、添字 $i$ の成分が 0 に等しい場合、$x=h_ix$ となり、pr$_i(u(x)) =$ pr$_i(u(h_ix)) =$ pr$_i(h_iu(x)) = 0$ となります。従って、$y\in M$ ごとに pr$_i(u(y)) =u_i$(pr$_i(y)$) となる一意な群準同型 $u_i: M_i\mapsto M_i$ が存在します。 $u=\prod u_i$があります。 写像 $u$ は A 線形であるため、写像 $u_i$ は $i\in I$ ごとに $A_i$ 線形です。これは、$\varphi$ 含む $A'_M$ の下に $\prod(A_i)'_{M_i}$ の像が成り立つことを証明します。逆の包含は明らかです。これを M の適用から対加群までにすると、$A''_M$ から $\prod_i(A_i)''_{M_i}$ まで $\varphi$ 誘導する同型と推定されます。これは主張 a) を証明します。

b)の証明はa)と同様です。

#### 命題 2 {#alg-viii-s5-prop-2 .statement tag=005G}

Aを環、MをA-加群とします。 Iを集合とします。次に、A-加群 $M^{(I)}$ 一致するの $A''_M$ モジュール $M^{(I)}$ の相同性の環の双可換子です。

$i\in I$ については、$M^{(I)}$ から M までの射影準同型を$\pi_i: (x_j)_{j\in I}\mapsto x_i$ で表し、対応する標準単射 (I, §4, No. 9, p. 47) を$\iota_i: M\rightarrow M^{(I)}$ で表します。

$u$をEnd$_A(M^{(I)})$の元とします。 M のすべての $i, j\in I$、合成 $u_{i,j}=\pi_j\circ u\circ \iota_i$ 属するから交換子環 $A'_M$ について、$A''_M$ のすべての元 $b$ とすべての $(x_i)\in M^{(I)}$ について、関係が得られます。

$$
bu((x_i)_{i\in I})=b(\sum_{i\in I}u_{i,j}(x_i))_{j\in I}=(\sum_{i\in I}u_{i,j}(bx_i))_{j\in I}=u(b(x_i)_{i\in I})
$$

ホモテティー $b_{M^{(I)}}$ したがって、A-加群 $M^{(I)}$ の属するから双可換子になります。

逆に、$b$を$M^{(I)}$の双可換子の元とします。 $i, j\in I$、集合 $b_{i,j}=\pi_j\circ b\circ \iota_i$の場合。 $i, j\in I$を$i\not=j$と組み合わせます。 A-加群 $M^{(I)}$ の $\iota_j\circ \pi_j$ 属するから交換子環まで、

$$
b_{i,j}=\pi_j\circ \iota_j\circ \pi_j\circ b\circ \iota_i=\pi_j\circ b\circ \iota_j\circ \pi_j\circ \iota_i= 0
$$

同様に、私たちも、

$$
b_{j,j}=\pi_j\circ b\circ \iota_j=\pi_i\circ \iota_i\circ \pi_j\circ b\circ \iota_j=\pi_i\circ b\circ \iota_i\circ \pi_j\circ \iota_j=b_{i,i}
$$

しかも$b_{i,i}$属するから$A''_M$まで。 $b$ 一致すると $A''_M$ モジュール $M^{(I)}$ のホモテティー が続きます。

### 2. 生成加群

Aを環とします。

#### 定義 2 {#alg-viii-s5-def-2 .statement tag=005H}

M から N までの A-線型写像の像によってすべての A-加群 N が生成される場合、A-加群 M は生成すると呼ばれます。

M を左A-加群とします。 M の双対を $M^*$ で表し、$M\times M^*$ (II, §2, No. 3, p. 233) の正規双線形形式を表します。

$$
(x, x^*)\mapsto  \langle x, x^*\rangle =x^*(x)
$$

形 $\sum^n_{i=1}\langle x_i, x^*_i\rangle$ の A の元の $\tau (M)$ 集合で表します。ここで、$x_1, . . . , x_n$ は M の元で、$x^*_1, . . . , x^*_n$ は $M^*$ の元です。これは、M のトレース イデアルと呼ばれる A の両面イデアルです。A-加群 $A_s$ のトレース イデアルは A です。加群、つまり A-加群の家族 $(M_i)_{i\in I}$ の直和のトレース イデアルは、イデアル $\sum_{i\in I}\tau (M_i)$ です。 M が射影 A-加群の場合、命題 II, §2, No. 6、p. 238 の 12 から、$M =\tau (M)M$ が得られます。

#### 定理 1 {#alg-viii-s5-thm-1 .statement tag=005I}

M を左A-加群とします。次のプロパティは同等です。

(i) A-加群 M は生成するです。

(ii) A-加群 N ごとに、$M^{(I)}$ から N までの集合 I と全射A-線型写像が存在します。

(iii) $M^n$から$A_s$まで整数$n\geqslant 0$と全射A-線型写像が存在します。

(iv) $A_s$ が $M^n$ の直和因子部分加群と同型であるような整数 $n\geqslant 0$ が存在します。

(v) トレース理想 $\tau (M)$ は A に等しい。

(vi) M の整数 $n\geqslant 0$、元 $x_1, . . . , x_n$、$M^*$ 満たす $\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$ の元 $x^*_1, . . . , x^*_n$ が存在します。

(i) $\Rightarrow$ (ii): M を生成する、N を左A-加群とします。 $N =\sum_{i\in I}u_i(M)$ となるような M から N までの A-線型写像の族 $(u_i)_{i\in I}$ が存在します。 写像 $(x_i)\mapsto \sum_{i\in I}u_i(x_i)$ から $M^{(I)}$ までは A 線形で全射です。

(ii) $\Rightarrow$ (iii): 性質 (ii) が成立すると仮定し、$N = A_s$ をとります。次に、集合 I と全射法線形写像 $u: M^{(I)}\rightarrow A_s$ が得られます。 $A_s$は元1によって生成されるので、$u(M^{(J)}) = A_s$,よってとなるようなIの有限部分集合Jが存在します(iii)。

(iii) $\Rightarrow$ (iv): これは、II, §1, No. 12、p. 218 の命題 21 から続きます。

(iv) $\Rightarrow$ (v): $A_s$ が M の直和因子部分加群と同型となるように、$n\geqslant 1$ を整数とします。$A =\tau (A_s)\subset \tau (M^n) =\tau (M)$ があるため、$\tau (M) = A$ になります。

(v) $\Rightarrow$ (vi): これは明らかです。

(vi) $\Rightarrow$ (i): $n$ を M の整数 $\geqslant 0,x_1, . . . , x_n$ 元と、$M^*$ 満たす $\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$ の $x^*_1, . . . , x^*_n$ 元とします。 N を N の左A-加群と $y$ 元とします。M から N までの写像 $u_i:x\mapsto  \langle x, x^*_i\rangle y$ は A 線形であり、$y=\sum^n_{i=1}u_i(x_i)$ が得られます。これにより、M は生成A-加群であることが証明されます。

#### 系 {#alg-viii-s5-n2-cor-1 .statement tag=00R1}

生成A-加群は忠実です。

$a\in A$ 満たす $aM = 0$ とします。 定理 1 の含意 (i) $\Rightarrow$ (iv) を使用すると、$aA_s= 0$、したがって $a= 0$ が得られます。 系が続きます (II, §1, No. 12、p. 219)。

#### 例 1 {#alg-viii-s5-n2-exa-1 .statement tag=005J}

A-加群 $A_s$ は生成するです。

#### 例 2 {#alg-viii-s5-n2-exa-2 .statement tag=005K}

すべての非零自由A-加群は生成するです。より一般的には、生成する商を伴うすべての加群は、それ自体生成するです。

#### 例 3 {#alg-viii-s5-n2-exa-3 .statement tag=005L}

M を半単純A-加群とし、その対加群は有限生成されます。すると、M は生成する $A_M$ モジュールになります。実際、VIII, p. 8 の補題 4 により、$(A_M)_s$ が $M^m$ の部分加群と同型となる自然数 $m$ が存在します。 $M^m$ は半単純 $A_M$ 加群であるため、$(A_M)_s$ は $M^m$ の直和因子部分加群と同型であり、M は生成する $A_M$ 加群 (定理 1) です。

#### 例 4 {#alg-viii-s5-n2-exa-4 .statement tag=005M}

A を主イデアル整域、P を有限生成A-加群とします。 P が $A/\mathfrak{a}_i$ (VII, §4, No. 4, p. 19, 定理) の直和と同型となるような A のイデアル $(\mathfrak{a}_i)_{1\leqslant i\leqslant n}$ の整数 $n\geqslant 1$ と増加する数列が存在します。 2); P の消滅子 $\mathfrak{a}$ は $\mathfrak{a}_1$ に等しい。すると、P は環 $A/\mathfrak{a}$ よりも生成加群になります。 P が捩れ加群でない場合、$\mathfrak{a}= 0$ となり、P は生成A-加群になります。

#### 補題 1 {#alg-viii-s5-lem-1 .statement tag=005N}

A を可換環、M を有限生成A-加群、アン(M) を消滅子とします。 $\mathfrak{a}$ を A のイデアルとします。次のプロパティは同等です。

(i) $\mathfrak{a}M = M$。

(ii) アン(男) $+\mathfrak{a}= A$。

(iii) $m\in M$ ごとに $am=m$ となるような $\mathfrak{a}$ の元 $a$ が存在します。

(i) $\Rightarrow$ (ii): $(x_1, . . . , x_n)$ を A-加群 M の生成するファミリーとします。 $\mathfrak{a}M = M$ の場合、各 $x_i$ は $\sum^n_{j=1}c_{ij}x_j$ として記述できます。ここで、$c_{ij}$ 属するから $\mathfrak{a}$ までです。 行列 $(c_{ij})$ を C で表し、列行列を$x_1, . . . , x_n$ X で表します。 ($I_n-C$)X = 0 となります。$d$ を行列式とし、V を行列 $I_n-C$ の余因子行列とします。 III, §8, No. 6, p. 532 の公式 (26) により、$dX=^tV$($I_n-C$)X = 0 となり、$d\in$ Ann(M) となります。一方、$c_{ij}$ 属するから $\mathfrak{a}$ なので、$d\equiv$ 1(mod $\mathfrak{a}$) (III, §8, No. 5, p. 529, (18)) となり、$1\in$ Ann(M) $+\mathfrak{a}$ となります。

(ii) $\Rightarrow$ (iii): (ii) が成り立つと仮定すると、$a+b= 1$ となるような$a\in \mathfrak{a}$ と $b\in$ Ann(M) が存在します。従って、$m\in M$ ごとに $am=m$ が得られます。

(iii) $\Rightarrow$ (i): これは明らかです。

#### 命題 3 {#alg-viii-s5-prop-3 .statement tag=00R2}

Aを可換環とします。有限で生成された忠実な射影 A-加群はすべて生成するです。より一般的には、有限生成された射影 A-加群 P は生成する $A_P$ モジュールです。

P を有限生成射影 A-加群とします。 $\tau (P)P = P$ (VIII、p. 80) があります。

A-加群 P が忠実である場合、イデアル $\tau (P)$ は A (補題 1) に等しく、A-加群 P は生成する (定理 1) です。これは最初の主張につながります。 2 番目は、以下の補題 2 に続きます。

#### 補題 2 {#alg-viii-s5-lem-2 .statement tag=005O}

A を環 、M を射影 A-加群とします。 $A_M$モジュール M は射影です。

$(x_i)_{i\in I}$ を A-加群 M の生成するファミリーとします。A-加群 M 上に線型形式のファミリー $(x^*_i)_{i\in I}$ が存在し、$x\in M$ ごとに、ファミリー $(\langle x, x^*_i\rangle )_{i\in I}$ には有限台と $x=\sum_{i\in I}\langle x, x^*_i\rangle x_i$ が含まれます。 (II, §2, No. 6、p. 238、命題 12)。すべての $i\in I$ に対して、写像 $x\mapsto  \langle x, x^*_i\rangle_M$ は、$A_M$ モジュール M の線型形式であり、すべての $x\in M$ に対して $x=\sum_{i\in I}\langle x, x^*_i\rangle_Mx_i$ があります。ロケ地にて。前述のとおり、M は射影 $A_M$ 加群です。

### 3. 双可換子/生成加群

#### 定理 2 {#alg-viii-s5-thm-2 .statement tag=005P}

生成加群はバランスが取れています。

A を環、M を生成A-加群とします。 定義によって、M の整数 $n\geqslant 0$、元 $x_1, . . . , x_n$、および M 満たす $\sum^n_{i=1}\langle x_i, x^*_i\rangle = 1$ の双対$M^*$ の元 $x^*_1, . . . , x^*_n$ が存在します。 (II, §4, No. 2、p. 271) 定義する群準同型 $\theta : M^*\otimes_AM\rightarrow$ 公式 $\theta (x^*\otimes y)(x) =\langle x, x^*\rangle y$ までに$_A(M)$ が終了することを思い出してください。 $u$ が M の双可換子の元である場合、End$_A(M)$ と可換です。従って、$y\in M$ ごとに、

$$
u(y) =u(\sum_{i=1}^n\langle x_i, x^*_i\rangle y)=\sum_{i=1}^nu(\theta (x^*_i\otimes y)(x_i))
$$

$$
=\sum_{i=1}^n\theta (x^*_i\otimes y)(u(x_i)) =(\sum_{i=1}^n\langle u(x_i), x^*_i\rangle )y
$$

従って、$u$ 属する ～ $A_M$ となり、M は均衡します。

#### 系 1 {#alg-viii-s5-thm-2-cor-1 .statement tag=005Q}

自由加群はバランスが取れています。

これは、加群が零、非零自由加群が生成する (VIII, p. 81, 例 2) であれば明らかです。

#### 系 2 {#alg-viii-s5-thm-2-cor-2 .statement tag=00R3}

A を環、$n$ を整数 $\geqslant 0$ とします。 $\mathbf{M}_n(A)$ の中心は、A の中心のエントリを持つスカラー 行列で構成されます。$A^n$ を左の $\mathbf{M}_n(A)$ モジュール (II, §10, No. 7、p. 349) として見ます。この加群のうち自己準同型は写像 $x\mapsto xa$ で、$a$ は A を通過します。

M を右A-加群 $A^n_d$ とします。 系 1 によってバランスが取れています。その結果、$A_M, A'_M$ の中心と $A''_M$ 一致するになります。 系 2 は、$A_M$ が A と同一視され、$A'_M$ が $\mathbf{M}_n(A)$ と同一視されるという事実から導かれます。

#### 注意 {#alg-viii-s5-n3-rem-1 .statement tag=005R}

M をA-加群とします。 $A_M$ モジュール M が生成するの場合、定理 2 による $A_M= A''_M$ が $A_M$ モジュール M に適用されるため、M はバランスのとれた A-加群になります。

#### 系 3 {#alg-viii-s5-thm-2-cor-3 .statement tag=005S}

可換環を超えるすべての有限生成射影加群はバランスが取れています。

実際、有限生成射影加群 M は、VIII、p. 82 の命題 3 による生成する $A_M$ モジュールです。従って、系は上記の注意から続きます。

#### 系 4 {#alg-viii-s5-thm-2-cor-4 .statement tag=005T}

主イデアル整域を超えるすべての有限生成加群はバランスが取れています。

確かに、主イデアル整域 A 上の有限生成加群 M は生成する $A_M$ モジュール (VIII, p. 81, 例 4) です。

#### 系 5 {#alg-viii-s5-thm-2-cor-5 .statement tag=005U}

K を K 上の可換体、V 有限次元ベクトル空間、そして V の $u$ と $v$ 自己準同型とします。次のプロパティは同等です。

(i) K[X] には $v= P(u)$ のような多項式 P が存在します。

(ii) 自己準同型 $v$ は、$u$ と通勤する V のすべての自己準同型と通勤します。

A を環 K[X] とし、M を V と $u$ (VII, §5, No. 1, p. 28) から推定される K[X] モジュールとします。 主張 (i) は $v\in K[X]_M$ を意味し、(ii) は $v\in K[X]''_M$ を意味します。従って、系 5 は系 4 の特殊なケースです。

#### 命題 4 {#alg-viii-s5-prop-4 .statement tag=005V}

半単純加群と有限生成された対加群はバランスがとれています。

これは、VIII、p. 81、注意の例 3 から続きます。

#### 系 1 {#alg-viii-s5-prop-4-cor-1 .statement tag=005W}

$(S_i)_{i\in I}$ を対非同型単純A-加群の有限族とする。 $i\in I$ の場合は、$D_i$ 体の自己準同型または $S_i$ の反対環で表します。すべての $i\in I$ について、$D_i$ ベクトル空間 $S_i$ が有限次元であると仮定します。すると、Aから$\prod_{i\in I}$終わり$_{D_i}(S_i)$まで写像$a\mapsto (a_{S_i})_{i\in I}$が全射になります。

A-加群 $M =\prod_{i\in I}S_i$ を考えてみましょう。 I は有限なので、$M =\bigoplus_{i\in I}S_i$ もあり、M の $S_i$ の像は、型 $S_i$ の M の同型成分です。その結果、A-加群 M の自己準同型は写像 $(s_i)\mapsto (s_id_i)$ となり、$(d_i)_{i\in I}$ は $\prod_{i\in I}D_i$ を通過します (VIII, p. 66, 命題 5)。 I は有限であり、すべての $i\in I$ に対して、右 $D_i$ ベクトル空間 $S_i$ は有限次元であるため、M の対加群は有限に生成されます。 命題 4 までに、A-加群 M のバランスが取れています。さて、A-加群 M の双可換子は、形 $\prod_{i\in I}u_i$ の End$_{\mathbf{Z}}(M)$ の元で構成されます。ここで、$(u_i)\in \prod_{i\in I}$ End$_{D_i}(S_i)$ (VIII, p. 78, 命題) 1) End$_{D_i}(S_i)$ は $S_i$ の双可換子であるため。 系はこの続きです。

この系は、特に、A が可換体 K 上で代数であり、各 $S_i$ が K-ベクトル空間として有限次元である単純A-加群である場合に当てはまります。実際、$D_i$ の場合、含むは相似関係になります。 $\alpha_{S_i}$、ここで、$\alpha$ は K を通過し、$S_i$ は K を超えているため、$D_i$ 上で有限次元になります。

#### 系 2 (バーンサイドの定理) {#alg-viii-s5-prop-4-cor-2 .statement tag=00S0}

A を代数的に閉じた可換体 K 上の代数とし、S を K-ベクトル空間として有限次元である単純A-加群とします。すると、A から End $_K(S)$ まで写像 $a\mapsto a_S$ は全射になります。

確かに、A-加群 S の自己準同型の体は、$\alpha_S$ と $\alpha \in K$ (VIII, p. 47, 定理 1) の相似関係から構成されます。次に、系を適用する 1 から単純A-加群 S になります。

### 4. 対加群/半単純加群

Aを環とします。 単純A-加群の類の集合を$\mathscr{S}$で表します。 類 $\lambda$ のすべての $\lambda \in \mathscr{S}$、選ぶ単純A-加群 $S_{\lambda}$ について、$S_{\lambda}$ の体の自己準同型の反対環を $D_{\lambda}$ で表します。 $S_{\lambda}$ を $(A,D_{\lambda}$)-bimodule として見ます。

M を半単純A-加群、B を M の自己準同型環とします。M の双可換子を C で表します。すべての $\lambda \in \mathscr{S}$ について、左の $(D_{\lambda}$、B)-bimodule Hom$_A(S_{\lambda},M)$ を $V_{\lambda}$ で表します。最後に、A-加群 M のサポートを $\mathscr{S}_M$ (VIII, p. 66) で表します。また、$V_{\lambda}$ は非零となるように、$\mathscr{S}$ の元 $\lambda$ も集合です。

#### 注意 1 {#alg-viii-s5-n4-rem-1 .statement tag=00R4}

A-加群の標準的記述 $\alpha_M$ M は、左 $(A$ の同型、B)-バイモジュールです。 命題 9, VIII, p. 71, 写像の系により $f\mapsto ($Hom(1$_{S_{\lambda}}, f$))$_{\lambda\in\mathscr{S}_M}$ B から $\prod_{\lambda\in\mathscr{S}_M}$ End$_{D_{\lambda}}(V_{\lambda})$ は環同型。

#### 命題 5 {#alg-viii-s5-prop-5 .statement tag=005X}

a) M の対加群は半単純です。

b) すべての $\lambda \in \mathscr{S}_M$ について、B-加群 $V_{\lambda}$ は単純で、その交換子環は $(D_{\lambda})_{V_{\lambda}}$ に等しい。

c) 写像 $\lambda \mapsto$ cl(V$_{\lambda}$) は、A-加群 M のサポートからその対加群のサポートまで、全単射です。

d) すべての $\lambda \in \mathscr{S}_M$ について、B-部分加群 $M_{\lambda}$ は B-加群 M の型 $V_{\lambda}$ の同型成分であり、M の $V_{\lambda}$ の重複度は以下に等しい薄暗い$_{D_{\lambda}}(S_{\lambda})$。

e) $s\in S$ については、$V_{\lambda}=$ Hom$_A(S_{\lambda},M)$ から M までの写像 $\varphi \mapsto \varphi (s)$ を$\widetilde{s}$ で表します。 B線形です。 結果として得られる写像 $S_{\lambda}$ から Hom$_B(V_{\lambda},M)$ までの $s\mapsto \widetilde{s}$ は、$(A,D_{\lambda})$ バイモジュールの同型です。

$\lambda \in \mathscr{S}_M$ にしましょう。 環終わり$_{D_{\lambda}}(V_{\lambda})$ を $E_{\lambda}$ で表します。 $V_{\lambda}$ は非零 $D_{\lambda}$ ベクトル空間であるため、単純な $E_{\lambda}$ モジュール (VIII, p. 45, 例 3) であり、その交換子環は $(D_{\lambda})_{V_{\lambda}}$ に等しい(VIII、p. 82、系 1/定理 2)。 $E_{\lambda}$ は B-加群 $V_{\lambda}$ (命題 9 の VIII, p. 71, 系) の環であるため、これは b) を証明します。

M 定義する同型 $\alpha_{\lambda}$ の $V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$ から $M_{\lambda}$ の標準的記述 $\alpha_M$。 $V_{\lambda}$ は単純B-加群であるため、B-加群 $V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$ は型 $V_{\lambda}$ (VIII, p. 61, 命題 1) と同型です。したがって、同じことが B-加群 $M_{\lambda}$ にも当てはまり、a) が証明されます。

上記の注意 1 により、$\mathscr{S}_M$ を通る $\lambda$ に対して B の元 $e_{\lambda}$ が存在し、$\mu\not=\lambda$ を伴う $\mu\in \mathscr{S}_M$ に対して $(e_{\lambda})_{V_{\lambda}}= 1_{V_{\lambda}}$ と $(e_{\lambda})_{V_\mu}$ = 0 になります。したがって、単純B-加群 $V_{\lambda}$ はペアごとに非同型であり、これは c) と d) の最初の主張を証明します。 B-加群 $M_{\lambda}$ は $V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$ と同型なので、dim$_{D_{\lambda}}(S_{\lambda})$ は M の $V_{\lambda}$ の重複度です (II, §3, No. 7, p. 255, 系 1)。

$\bigoplus_{\lambda\in\mathscr{S}_M}V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}$ から M への写像 $\sum_{\lambda\in\mathscr{S}_M}\alpha_{\lambda}$ は、半単純 B-加群 M の記述 (VIII、p. 69、定義 5) を提供します。VIII、p. 70、命題により8、b)、e) で説明した $S_{\lambda}$ から Hom$_B(V_{\lambda},M)$ までのすべての $\lambda \in \mathscr{S}_M$、写像は全単射であり、$D_{\lambda}$ 線形です。明らかに A-linear であるため、これは e) を証明します。

#### 注意 2 {#alg-viii-s5-n4-rem-2 .statement tag=00R5}

証明から写像となります。

$$
\sum_{\lambda\in\mathscr{S}_M}V_{\lambda}\otimes_{D^o_{\lambda}}S_{\lambda}\longrightarrow M
$$

M の標準的記述によって引き起こされるものは、M の対加群の記述です。

#### 命題 6 {#alg-viii-s5-prop-6 .statement tag=005Y}

a) $(A,B^o)$-バイモジュールとして見ると、M は半単純です。

b) すべての $\lambda \in \mathscr{S}_M,M_{\lambda}$ は M の単純な $(A,B^o)$ サブモジュールです。

c) M のすべての $(A,B^o)$ サブバイモジュール N に対して、N が $\oplus_{\lambda\in\Lambda}M_{\lambda}$ に等しいような $\mathscr{S}_M$ の一意の部分集合 Λ が存在します。

$\lambda$ を $\mathscr{S}_M$ に入れます。 左A-加群 $S_{\lambda}$ と右B-加群 $V_{\lambda}$ は単純で、$D_{\lambda}$ は体の自己準同型の $S_{\lambda}$ の反対環です。 VIII, p. 63 の系 2 により、$(A,B^o$)-bimodule $S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ は単純であり、これと同型である $M_{\lambda}$ にも同じことが当てはまります。 これは b) を証明し、a) が続きます。

$\mathscr{S}_M$ で $\lambda$ と $\mu$ が異なる場合、$M_{\lambda}$ と $M_\mu$ は A-加群と同型ではなく、なおさらは $(A,B^o$)-bimodule と同型ではありません。 主張 c) の後に、系 VIII、p. 68 の 2 が続きます。

#### 命題 7 {#alg-viii-s5-prop-7 .statement tag=005Z}

a) M の双可換子 C のすべての元 $c$ とすべての $\lambda \in \mathscr{S}_M$ に対して、End$_{D_{\lambda}}(S_{\lambda})$ の一意元 $c_{\lambda}$ が存在し、すべての $\varphi \in$ Hom$_A(S_{\lambda},M)$ とすべての $s\in S_{\lambda}$ について、 $c\varphi (s) =\varphi (c_{\lambda}s)$。

b) $\lambda$ から $\mathscr{S}_M$ までを実行する$S_{\lambda}$ に、a) で定義された C モジュール構造を与えます。すると、$\bigoplus_{\lambda\in\mathscr{S}_M}S_{\lambda}\otimes_{D_{\lambda}}V_{\lambda}$ から M までの標準写像 $\alpha_M$ は、$(C,B^o)$-bimodules の同型になります。

c) 写像 $c\mapsto (c_{\lambda})_{\lambda\in\mathscr{S}_M}$ は、C から $\prod_{\lambda\in\mathscr{S}_M}$ 終了$_{D_{\lambda}}(S_{\lambda})$ までの同型です。

主張 a) と c) は、VIII、p. 71、命題 9 から続きます。なぜなら、$\bigoplus_{\lambda\in\mathscr{S}}(S_{\lambda}\otimes_{D_{\lambda}}W_{\lambda})$ から M までの標準写像 $\alpha_M$ は、B-加群 M (注意 2) の記述を提供するからです。さらに、$\alpha_M$ は $(C,B^o$)-線形であり、b) が証明されます。

#### 注意 3 {#alg-viii-s5-n4-rem-3 .statement tag=0060}

$\lambda \in \mathscr{S}_M$ に対して、命題 7、a) で与えられる C モジュール構造を$S_{\lambda}$ に与えます。 If we replace A with B and B with C in Proposition 5 (VIII, p. 85), then we see that for every $\lambda \in \mathscr{S}_M$, the left C-module $S_{\lambda}$ is simple, with commutant $D_{\lambda}$, that the isotypical component of type $S_{\lambda}$ of the C-module M is equal to $M_{\lambda}$, and that the mapping $\lambda \mapsto$ cl$_C(S_{\lambda})$ is a bijection from the support of the A-module M to the support of the C-module M. 最後に、$S_{\lambda}$ から M への A-線型写像と C の線形マッピングが同一であり、M の A-部分加群と C サブモジュールも同一であり、環 End$_A(M)$ と End$_C(M)$ が等しいことを観察します。

Mを半単純A-加群とします。 Z 中心の双可換子 C の A-加群 M で表します。また、M. Endow M の交換子環 B の中心と、$\lambda \in \mathscr{S}_M$ の $S_{\lambda}$ であり、C モジュール構造からのスカラーの制限によって推定された Z モジュール構造を備えています。 $\lambda \in \mathscr{S}_M$ ごとに、体 $D_{\lambda}$ の中心を $Z_{\lambda}$ で表します。

#### 命題 8 {#alg-viii-s5-prop-8 .statement tag=0061}

a) 写像 $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$ は、体 $Z_{\lambda}$ の Z から積までの同型です。

b) A-加群 M は同型であり、Z が体である場合に限り、非零です。

c) Λ を $\mathscr{S}_M$ の部分集合とします。 $\lambda \in \Lambda$ は $(e_{\Lambda})_{S_{\lambda}}= 1_{S_{\lambda}}$、$\lambda \in \mathscr{S}_M-\Lambda$ は $(e_{\Lambda})_{S_{\lambda}}= 0$ となるように、Z の $e_{\Lambda}$ 一意元で表します。 $\lambda \in \Lambda$には$(e_{\Lambda})_{M_{\lambda}}= 1_{M_{\lambda}}$、$\lambda \in \mathscr{S}_M-\Lambda$には$(e_{\Lambda})_{M_{\lambda}}= 0$がございます。

d) If the support $\mathscr{S}_M$ of M is finite, then the mapping $\Lambda \mapsto e_{\Lambda}Z$ is a bijection from the set of subsets of $\mathscr{S}_M$ to the set of ideals of Z, and the mapping $\mathfrak{a}\mapsto \mathfrak{a}M$ is a bijection from the set of ideals of Z to the set of $(A,B^o)$-sub-bimodules of M. これらの全単射は順序集合の同型です。 逆の全単射は、M の $(A,B^o)$ サブバイモジュール N を、N を M に送信する Z の元 $z$ の理想的なからなるに送信します。

$\lambda \in \mathscr{S}_M, Z_{\lambda}$ は、交換子環 $D_{\lambda}$ の共通中心と A-加群 $S_{\lambda}$ の双可換子 $C_{\lambda}$ です。上記の命題 7、c) により、写像 $c\mapsto (c_{\lambda})_{\lambda\in\mathscr{S}_M}$ は C から $\prod_{\lambda\in\mathscr{S}_M}C_{\lambda}$ までの同型になります。 制限から中心により、Z から $\prod_{\lambda\in\mathscr{S}_M}Z_{\lambda}$、よって a) までの同型 $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$ が得られます。

b) 集合 $\mathscr{S}_M$ に 1 つの元、よってがある場合に限り、環 $\prod_{\lambda\in\mathscr{S}_M}Z_{\lambda}$ は体になります。

主張 c) は命題 7、a) から続きます。 $\mathscr{S}_M$ が有限であると仮定します。 a) と I, §8, No. 10、p. 109 の命題 8 から、写像 $\Lambda \mapsto e_{\Lambda}Z$ は、Z の理想の $\mathfrak{P}(\mathscr{S}_M)$ から集合までの順序集合の同型であることがわかります。Λ を次の部分集合とします。 $\mathscr{S}_M$。 c) により、関係 $e_{\Lambda}$ZM $=e_{\Lambda}M =$ $\bigoplus_{\lambda\in\Lambda}M_{\lambda}$ となります。 命題 6、c) VIII、p. 86 のため、逆全単射について説明する必要があります。しかし、$z\in Z$ は、$z=e_{\Lambda}z$、つまり $z\in e_{\Lambda}Z$ の場合に限り、M を $\bigoplus_{\lambda\in\Lambda}M_{\lambda}$ に送ります。

#### 系 {#alg-viii-s5-n4-cor-1 .statement tag=0062}

A が代数的に閉じた可換体 K 上で代数であり、M が K 上でベクトル空間として有限次元である半単純A-加群であるとします。 $\mathscr{S}_M$ のすべての $\lambda$ について、M の $e_{\lambda}$ 射影子で表します。 像 $M_{\lambda}$ と核 $\oplus_{\lambda\not=\mu}M_\mu$すると、$(e_{\lambda})_{\lambda\in\mathscr{S}_M}$ は K 上のベクトル空間 Z の基底です。

M は K より有限次元ベクトル空間であるため、非零部分加群 $(M_{\lambda})_{\lambda\in\mathscr{S}_M}$ の族の直和であるため、集合 $\mathscr{S}_M$ は有限であり、$\lambda \in \mathscr{S}_M$ に対する空間 $S_{\lambda}$ のそれぞれは、 体 K は代数的に閉じているので、$D_{\lambda}= Z_{\lambda}= K$ (VIII, p. 47, 定理 1) があり、写像 $z\mapsto (z_{S_{\lambda}})_{\lambda\in\mathscr{S}_M}$ は Z から $K^{\mathscr{S}_M}$ まで同型です。 (命題 8、a))。 系は、命題 8 の部分 c) から続きます。

### 5. 密度定理

#### 定理 3 (ジェイコブソン) {#alg-viii-s5-thm-3 .statement tag=00S1}

M を半単純A-加群とし、$c$ を加法群 M の自己準同型とします。次に、次の条件を満たす場合に限り、M の $c$ 属するから双可換子 $A''_M$ となります。

(D) M のすべての有限部分集合 F に対して、F に $a_M$ を持つ $c$ 一致するとなる A の元 $a$ が存在します。

まず、$c$ が条件 (D) を満たすとします。 $u$を$A'_M$の元とします。 $x$をMの元とし、条件(D)を部分集合$F =\{x, u(x)\}$に当てはめます。 $c(x) =ax$と$c(u(x)) =au(x)$となるようなAの元$a$が存在するので、$u(c(x)) =u(ax) =au(x) =c(u(x))$になります。 $x$ は任意なので、$cu=uc$ になります。これはすべての $u$ に当てはまるので、$c\in A''_M$ になります。

逆には、次の補題を使用します。

#### 補題 3 {#alg-viii-s5-lem-3 .statement tag=0063}

M を半単純A-加群とします。 B を A-加群 M の双可換子とします。すると、M のすべての A-部分加群は M の B-部分加群になります。

N を M の A-部分加群とします。VIII, p. 56 の系 2 により、像 N を持つ A-加群 M の射影子 $p$ が存在します。それは属するから$A'_M$です。 $b\in B$ ごとに関係 $pb=bp$ があるため、N は M の B-部分加群であることがわかります。

定理 3 の結論する証明とします。 $c$ 属するから $A''_M$ とし、F = $\{x_1, . . . , x_n\}$ を M の有限部分集合とします。 $M^n$ の元 $(x_1, . . . , x_n)$ を $x$ で表します。 A-加群 $M^n$ は半単純で、VIII、p. 79 の命題 2 により、その双可換子一致するは $A''_M$ 加群 $M^n$ の相似性となります。 補題 3 により、$M^n$ の A-部分加群 $Ax$ は $M^n$ の $A''_M$ サブモジュールになります。 $a\in A$ を、$(cx_1, . . . , cx_n)$ が $ax$ に等しいものとします。 次に、$c$ 一致すると $\{x_1, . . . , x_n\}$ の $a_M$ は、条件を意味します (D)。

#### 注意 {#alg-viii-s5-n5-rem-1 .statement tag=0064}

M の加法群の自己準同型環を E で表します。M に離散位相を与えます。 環 E は M から M までの写像で構成され、$M^M$ 上の積位相によって誘導される位相を与えることができます (「M の単純な収束の位相」、Gen. Top.、I, §2, No. 3、p. 31)。 E の位相はハウスドルフであり、E の加法群構造と互換性があります。E のすべての $f$ に対して、E から E までの写像 $g\mapsto f\circ g$ と $g\mapsto g\circ f$ は連続です。従って、E のすべての部分集合の交換子環は E で閉じられます。従って、定理 3 は、$A''_M$ が E の $A_M$ の閉包であることを意味します。

### 6. 体理論への申請

#### 命題 9 {#alg-viii-s5-prop-9 .statement tag=0065}

L を体とし、E 部分環を End$_{\mathbf{Z}}(L)$ とし、$a\in L$ ごとに含む写像 $\boldsymbol{\gamma }_a:x\mapsto ax$ とします。 L のすべての $x$ と E のすべての $u$ に対して $u(xa) =u(x)a$ となるように、元の$a$ L の K 集合で表します。 Lの部分体です。

V を右辺 K-ベクトル空間 L の有限次元線形部分空間とし、$h$ を V から L までの K-線型写像とします。 Vに$h$を持つ一致するであるEの元が存在します。

L を左側の E モジュールと見なします。 E 含むは左乗法 $\boldsymbol{\gamma }_a$ なので、L のすべての E サブモジュールは体 L の左イデアルです。従って、E モジュール L は単純です。 $\boldsymbol{\gamma }_a$ と通勤する L の加法群のすべての自己準同型は、L の $b$ とともに形 $\boldsymbol{\delta }_b:x\mapsto xb$ になります。従って、$b\mapsto \boldsymbol{\delta }_b$はKからEnd$_E$(L)の反対環まで同型、つまり体になります。

従って、E モジュール L の双可換子 $E''$ は、右側 K-ベクトル空間 L の自己準同型で構成されます。 $v$ を K-ベクトル空間 L の自己準同型とし、制限を V 一致すると$h$ で表します。 $E''$の元です。 $(x_i)_{i\in I}$ を K 上の V の基底とします。 定理 3 (VIII, p. 88) により、$i\in I$ に対して $u(x_i) =v(x_i) =h(x_i)$ となるような E の元 $u$ が存在します。線形性により、V のすべての $x$ に対して $u(x) =h(x)$ が得られます。

#### 系 {#alg-viii-s5-n6-cor-1 .statement tag=0066}

Lを体とします。 Let Γ be a subgroup of the automorphism group of the field L, and let K be the field of invariants of Γ. V を K 上の有限次元 $n$ の L の右 K 線形部分空間とします。 次に、次の性質を伴う Γ の元 $\sigma_1, . . . , \sigma_n$ が存在します。 V から L までの K-線型写像 $u$ ごとに、L の元 $a_1, . . . , a_n$ が存在し、すべてに $u(x) =\sum_{i=1}^na_i\sigma_i(x)$ が存在します。 Vの$x$。

形 $x\mapsto$ $\sum_{\sigma\in\Gamma}a_{\sigma}\sigma (x)$ の L から L までの写像の E 集合で表します。ここで、$(a_{\sigma})_{\sigma\in\Gamma}$ は L と有限台の元のファミリーです。 L のすべての $a$ に対して $\boldsymbol{\gamma }_a\in E$ があり、E は自己準同型の部分環 L の加法群の環です。さらに、体 K は、L のすべての $x$ と E のすべての $u$ に対して $u(xa) =u(x)a$ となるように、L の元 $a$ で構成されます。

H を左 L-ベクトル空間 Hom$_K(V,L)$ とします。 次元 $n$ があります。 命題9により、Γの元の制限からVまで生成されます。 Lを超えるHの制限からV形基底を持つΓの$n$元$\sigma_1, . . . , \sigma_n$が存在します。 系はこれに続きます。

#### 注意 {#alg-viii-s5-n6-rem-1 .statement tag=0067}

体 L が可換である場合、この系簡約するは Artin の定理 (V, §10, No. 6, p. 65) になります。

### 練習問題 {#alg-viii-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
