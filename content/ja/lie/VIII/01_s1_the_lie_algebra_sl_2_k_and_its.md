---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 1
section_title: The Lie algebra sl(2, k) and its representations
lang: ja
source: lie-vii-ix
book_pages: 69-77, 219-226
pdf_pages: 0077-0085, 0227-0234
extraction: native+ocr
subsections:
    - "no": 1
      title: CANONICAL BASIS OF $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)
      page: 69
      pdf_page: 77
    - "no": 2
      title: PRIMITIVE ELEMENTS OF $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)-MODULES
      page: 70
      pdf_page: 78
    - "no": 3
      title: THE SIMPLE MODULES V($\boldsymbol{m}$)
      page: 72
      pdf_page: 80
    - "no": 4
      title: LINEAR REPRESENTATIONS OF THE GROUP SL(2$\boldsymbol{, k}$)
      page: 74
      pdf_page: 82
    - "no": 5
      title: SOME ELEMENTS OF SL(2$\boldsymbol{, k}$)
      page: 76
      pdf_page: 84
statements: 23
exercises: 18
content_sha256: 3c578e61685c46de048332ab99cf38d135a97e12833da5969f4caf4de2f43771
translated_from: content/en/lie/VIII/01_s1_the_lie_algebra_sl_2_k_and_its.md
translation_method: google
source_content_sha256: d56ad334c8b961365f3d72d7c521802edd95553bc6c867158ffa18290345692f
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 556ae4a0ccddd9a2370fd4fbbd8abc8ce8e3dc53258c261d177ac2fc0a4ae5c0
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。 リー代数 $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$) とその表現

### 1. $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)の標準基底

#### 補題 1 {#lie-viii-s1-lem-1 .statement tag=00XS}

A を、$[H, X] = 2X$ となるような A の $k,H$ および $X$ 元に対する結合代数とします。

(i) 整数 $n\geq 0$ の場合は $[H, X^n] = 2nX^n$。

(ii) $Z$ が $[Z, X] =H$ となるような A の元である場合、任意の整数 $n >0$ について、

$$
[Z, X^n] =nX^{n-1}(H+n-1) =n(H-n+ 1)X^{n-1}
$$

AからAへの写像 $T \rightarrow [H, T]$は導分であり、これは(i)を意味します。 (ii)の仮定では、

$$
[Z, X^n] =\sum_{i+j=n-1}X^iHX^j
$$

$$
=\sum_{i+j=n-1}(X^iX^jH+X^i2jX^j)
$$

$$
=nX^{n-1}H+ 2X^{n-1}\frac{n(n- 1)}{2}
$$

$$
=nX^{n-1}(H+n-1)
$$

一方、(i)の$X^{n-1}(H+n-1) = (H-n+ 1)X^{n-1}$。 Q.E.D.

$\mathfrak{s}\mathfrak{l}(2, k)$ リー代数からなる of 正方行列 of 位数 2、トレース零、および $k$ のエントリで表されることを思い出してください。 このリー代数は次元3（I, §6, no. 7、例章）の単純なものです。 $\mathfrak{s}\mathfrak{l}(2, k)$ の標準基底は基底 $(X_+, X_-, H)$ です。ここで、

$(01)($ 0 $0)(1$ 0 $)$

$X_+=$ 0 0 $X_-=-1$ 0 $H=$ 0 $-1$。

我々は持っています

$$
[H, X_+] = 2X_+[H, X_-] =-2X_-[X_+, X_-] =-H \tag{1}
$$

$\mathfrak{s}\mathfrak{l}(2, k)$ の恒等表現は単射であるため、$H$ は $\mathfrak{s}\mathfrak{l}(2, k)$ の半単純元であり、$X_+, X_-$ は $\mathfrak{s}\mathfrak{l}(2, k)$ の冪零元です (第 3 章 I, §6, no. 3)。章著。 VII, §2, no. 1、例 $4,kH$ は、$\mathfrak{s}\mathfrak{l}(2, k)$ のカルタン部分代数です。 写像 $U \rightarrow  -^tU$ は、リー代数 $\mathfrak{s}\mathfrak{l}(2, k)$ の包含自己同型であり、$\mathfrak{s}\mathfrak{l}(2, k)$ の正規包含と呼ばれます。それは変換 $(X_+, X_-, H)$ から $(X_-, X_+,-H)$ になります。

#### 補題 2 {#lie-viii-s1-lem-2 .statement tag=00XT}

$\mathfrak{s}\mathfrak{l}(2, k)$を包み込む代数の中で、

$$
[H, X_+^n] = 2nX_+^n[H, X_-^n] =-2nX_-^n
$$

整数 $n\geq 0$ の場合、および

$$
[X_-, X_+^n] =nX_+^{n-1}(H+n-1) =n(H-n+ 1)X_+^{n-1}
$$

$$
[X_+, X_-^n] =nX_-^{n-1}(-H+n-1) =n(-H-n+ 1)X_-^{n-1}
$$

$n >0$の場合。

最初と 3 番目の関係は、補題 1 から続きます。その他は、$\mathfrak{s}\mathfrak{l}(2, k)$ の正準累乗を使用してそれらから推定できます。

### 2. プリミティブ元 OF $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$) モジュール

E を $\mathfrak{s}\mathfrak{l}(2, k$) モジュールとする。 $A\in \mathfrak{s}\mathfrak{l}(2, k)$ と $x\in E$ の場合、$A_Ex$ の代わりに $Ax$ と書くことがよくあります。 $\lambda \in k$ にしましょう。 $Hx=\lambda x$ が言葉の乱用により、$x$ は重み $\lambda$ の E の元である、または $\lambda$ は $x$ の重みであると言った場合。 E が有限次元の場合、$H_E$ は半単純であるため、重み $\lambda$ の元の集合は、$H_E$ と $\lambda$ に対する E の主要な部分空間です (cf. 第 3 章)。 VII, §1, no. 1）。

#### 補題 3 {#lie-viii-s1-lem-3 .statement tag=00XU}

$x$ が重み $\lambda$ の元である場合、$X_+x$ は重み $\lambda + 2$ の元であり、$X_-x$ は重み $\lambda -2$ の元です。

Indeed, $HX_+x= [H, X_+]x+X_+Hx= 2X_+x+X_+\lambda x= (\lambda + 2)X_+x$, and similarly $HX_-x= (\lambda -2)X_-x$ (cf. also Chap. VII, §1, no. 3, Prop. 10 (ii)).

#### 定義 1 {#lie-viii-s1-def-1 .statement tag=00XV}

E を $\mathfrak{s}\mathfrak{l}(2, k)$ モジュールとします。 E の元は、$H_E$ と $X_{+E}$ の属する ～ 核の非ゼロ固有ベクトルである場合、原始的であると言われます。

E の非ゼロ元 $e$ は、$ke$ が $kH+kX_+$ の演算で安定している場合に限り、プリミティブです。これは、たとえば補題 3 から続きます。

例元 $X_+$ は、$\mathfrak{s}\mathfrak{l}(2, k)$ の随伴表現に対する重み 2 のプリミティブです。 $k^2$ の元 $(1,0)$ は、$k^2$ 上の $\mathfrak{s}\mathfrak{l}(2, k)$ の恒等性表現に対する重み 1 のプリミティブです。

#### 補題 4 {#lie-viii-s1-lem-4 .statement tag=00XW}

E を非ゼロの有限次元 $\mathfrak{s}\mathfrak{l}(2, k)$ 加群とする。この場合、E はプリミティブ元を持ちます。

$X_+$ は $\mathfrak{s}\mathfrak{l}(2, k),X_{+E}$ の冪零元であるため、零です。 $X_{+E}^{m-1}\not= 0$ および $X_{+E}^m$ = 0 と仮定します。 補題 2 により、

$$
m(H_E-m+ 1)X_{+E}^{m-1}= [X_{-E}, X_{+E}^m] = 0
$$

したがって、$X_+^{m-1}(E)$**--** $\{0\}$ の元はプリミティブです。

#### 命題 1 {#lie-viii-s1-prop-1 .statement tag=00XX}

E を $\mathfrak{s}\mathfrak{l}(2, k)$ モジュール、$e$ を重み $\lambda$ の E のプリミティブ元とします。 $n\geq 0$と$e_{-1}= 0$に$e_n=\frac{(-1)^n}{n}X_-^ne$を入れます。それから

$$
He_n= (\lambda -2n)e_n
$$

$$
X_-e_n=-(n+ 1)e_{n+1} \tag{2}
$$

$$
X_+e_n= (\lambda -n+ 1)e_{n-1}
$$

最初の公式は補題 3 から続き、2 番目は $e_n$ の定義から続きます。 3番目を$n$の帰納法によって証明します。 $e_{-1}= 0$から$n= 0$は満足です。 $n >0$の場合、

$$
nX_+e_n=-X_+X_-e_{n-1}=-[X_+, X_-]e_{n-1}-X_-X_+e_{n-1}
$$

$$
=He_{n-1}-X_-(\lambda -n+ 2)e_{n-2}
$$

$$
= (\lambda -2n+ 2 + (n-1)(\lambda -n+ 2))e_{n-1}
$$

$$
=n(\lambda -n+ 1)e_{n-1}
$$

#### 系 {#lie-viii-s1-n2-cor-1 .statement tag=00XY}

$e$ によって生成された E の部分加群は、$e_n$ によって生成されたベクトル部分空間です。

これは公式 (2) から続きます。

整数 $n\geq 0$ により、$e_n\not= 0$ が $\mathbf{N}$ の区間を構成し、対応する元 $e_n$ 形基底が部分加群の $k$ を超えるようになります。 $e$ (実際、それらは別個の重みの非ゼロ元であるため、線形独立です)。この基底は、原始的な元 $e$ に関連付けられていると言われます。

#### 命題 2 {#lie-viii-s1-prop-2 .statement tag=00XZ}

プリミティブ元 $e$ によって生成された E の部分加群 V が有限次元の場合、次のようになります。

(i) $e$ の重み $\lambda$ は整数で、dim $V-1$ に等しい。

(ii) $(e_0, e_1, . . . , e_{\lambda})$ は V の基底、および $n > \lambda$ の $e_n= 0$ です。

(iii) $H_V$ のうち固有値は $\lambda , \lambda -2, \lambda -4, . . . ,-\lambda$ です。それらはすべて重複度 1 です。

(iv) V のすべてのプリミティブ元は $e$ に比例します。

(v) 加群 V の交換子環はスカラーに還元されます。特に、V は非常にシンプルです。

$m$ を最大の整数として、$e_m\not= 0$ とします。次に、$0 =X_+e_{m+1}=$ $(\lambda -m)e_m$、つまり $\lambda =m$; $(e_0, e_1, . . . , e_m)$ は V の基底であるため、これは (i) と (ii) を証明します。 主張 (iii) は等式 $He_n= (\lambda -2n)e_n$ から続きます。 $1\leq n\leq m$ には $X_+e_n\not= 0$ があるため、(iv) になります。 $c$ を交換子環の加群 V の元とします。次に $Hc(e) =cH(e) =\lambda c(e)$ なので、$c(e) =\mu e$ となるような $\mu\in k$ が存在します。それから

$$
cX_-^qe=X_-^qce=\mu X_-^qe
$$

すべて $q\geq 0$ なので、$c=\mu.1$、証明 (v)。

#### 系 {#lie-viii-s1-n2-cor-2 .statement tag=00Y0}

E を有限次元 $\mathfrak{s}\mathfrak{l}(2, k)$ 加群とする。

(i) 自己準同型 $H_E$ は対角化可能であり、その固有値は有理数整数です。

(ii) 任意の $p\in \mathbf{Z}$ について、$E_p$ を $H_E$ 対応するから固有値 $p$ の固有空間とする。 $i$ を整数 $\geq 0$ とします。 写像 $X_{-E}^i|E_p: E_p\rightarrow E_{p-2i}$ は、$i\leq p$ に対して単射、$i=p$ に対して全単射、$i\geq p$ に対して全単射です。 写像 $X_{+E}^i|E_{-p}: E_{-p}\rightarrow E_{-p+2i}$ は、$i\leq p$ に対して単射、$i=p$ に対して全単射、$i\geq p$ に対して全単射です。

(iii) E の長さは、dim Ker$X_{+E}$ および dim Ker$X_{-E}$ に等しい。

(iv) $E'$ (それぞれ $E''$) を、$p$ 偶数 (それぞれ奇数) の $E_p$ の和とします。すると、$E'$ (それぞれ$E''$) は、奇数 (それぞれ偶数) 次元の E の単純部分加群の和です。そして$E = E'\oplus E''$。 $E'$の長さは薄暗い$E_0$、$E''$のそれは薄暗い$E_1$です。

(v) Ker$X_{+E}\cap$ Im$X_{+E}\subset \sum_{p>0}E_p$ と Ker$X_{-E}\cap$ Im$X_{-E}\subset \sum_{p<0}E_p$。

E が単純な場合、E はプリミティブ元 (補題 4) によって生成され、命題を適用する 1 と 2 で十分です。すべての有限次元 $\mathfrak{s}\mathfrak{l}(2, k$) モジュールは半単純であるため、一般的なケースが続きます。

### 3. 単純加群 V($\boldsymbol{m}$)

$(u, v)$ を $k^2$ の標準基底とします。 $\mathfrak{s}\mathfrak{l}(2, k)$ のアイデンティティ表現については、

$$
X_+u= 0Hu=uX_-u=-v
$$

$$
X_+v=uHv=-vX_-v= 0
$$

$k^2($代数の対称的な代数 $\mathbf{S}(k^2)$ を考えてみましょう。 III, §6, no. 1、デフォルト。 1)。 $\mathfrak{s}\mathfrak{l}(2, k)$ の元拡大するは $\mathbf{S}(k^2)$ の導分に固有であり、$\mathfrak{s}\mathfrak{l}(2, k$) モジュールの $\mathbf{S}(k^2)$ 構造が与えられます (第 I, §3, no. 2 章)。 $V(m)$ を同次の集合元の $\mathbf{S}(k^2)$ の次数 $m$ とします。このとき、$V(m)$ は、次元 $m+ 1$ の $\mathbf{S}(k^2)$ の $\mathfrak{s}\mathfrak{l}(2, k$) 部分加群であり、$V(1) =k^2$ の $m$ 番目の対称冪 (第 III、付録) です。 $m, n$ が整数で $0\leq n\leq m$ になる場合、

$$
e^{(m)}_n=(m)u^{m-n}v^n\in V(m)
$$

$$
n
$$

#### 命題 3 {#lie-viii-s1-prop-3 .statement tag=00Y1}

任意の整数 $m\geq 0$ にとって、$V(m)$ は非常に単純な $\mathfrak{s}\mathfrak{l}(2, k)$ モジュールです。この加群において、$e^{(m)}_0=u^m$は重み$m$のプリミティブです。

$X_+u^m= 0$ と $Hu^m=mu^m$ があるので、$u^m$ は重み $m$ の原始関数です。 $u^m$ によって生成された $V(m)$ の部分加群は、次元 $m+ 1$ のものであるため (提案 2 (i))、$V(m)$ と等しくなります。提案 2 (v) により、$V(m)$ は非常に簡単です。

#### 定理 1 {#lie-viii-s1-thm-1 .statement tag=00Y2}

有限次元 $n$ のすべての単純な $\mathfrak{s}\mathfrak{l}(2, k)$ モジュールは $V(n-1)$ と同型です。すべての有限次元 $\mathfrak{s}\mathfrak{l}(2, k)$ 加群は、加群 $V(m)$ と同型の部分加群の直和です。

これは、補題 4 および提案 1、2、および 3 に続きます。

#### 注意 1 {#lie-viii-s1-n3-rem-1 .statement tag=00Y3}

単純な $\mathfrak{s}\mathfrak{l}(2, k$) モジュールの $\mathfrak{s}\mathfrak{l}(2, k)$ 構造上の $\mathfrak{s}\mathfrak{l}(2, k)$ 定義するの随伴表現。この加群は、$u^2$ ～ $X_+, 2uv$ ～ $-H$、および $v^2$ ～ $X_-$ を取る同型による V(2) と同型です。

#### 注意 2 {#lie-viii-s1-n3-rem-2 .statement tag=00Y4}

$n\geq 0$と$m > n$の場合、

$$
X_-e^{(m)}_n=-(m-n)(m)u^{m-n-1}v^{n+1}=-(n+ 1)e^{(m)}_{n+1}
$$

$$
n
$$

したがって、$(e_0^{(m)}, e_1^{(m)}, . . . , e_m^{(m)})$ は、プリミティブ元 $e_0^{(m)}$ に関連付けられた $V(m)$ の基底です。

#### 注意 3 {#lie-viii-s1-n3-rem-3 .statement tag=00Y5}

$\Phi$ を $V(m)$ の双線形形式とすると、次のようになります。

$n+n'\not=m$なら$\Phi (e^{(m)}_n, e^{(m)}_{n'}) = 0$

$$
\Phi (e^{(m)}_n, e^{(m)}_{m-n}) = (-1)^n(m)
$$

$$
n
$$

$x=au+bv$ と $y=cu+dv$ の場合は、$\Phi (x^m, y^m) = (ad-bc)^m$ です。 $\Phi$ が不変であること、$\Phi$ が $m$ の偶数に対して対称であること、交代的が奇数の $m$ に対して対称であることを確認するのは簡単です。

#### 命題 4 {#lie-viii-s1-prop-4 .statement tag=00Y6}

E を、重み $m$ の原始関数元の有限次元 $\mathfrak{s}\mathfrak{l}(2, k)$ 加群、$m$ 整数 $\geq 0$、$P_m$ 集合とする。 L を、$\mathfrak{s}\mathfrak{l}(2, k)$ モジュール $V(m)$ から $\mathfrak{s}\mathfrak{l}(2, k)$ モジュール E までの準同型のベクトル空間とします。 L から E までの写像 $f \rightarrow f(u^m)$ は線形で単射的であり、その像 $P_m\cup  \{0\}$です。

この写像は明らかに線形であり、$u^m$ 生成するは $\mathfrak{s}\mathfrak{l}(2, k$) 加群 $V(m)$ であるため単射的です。 $f\in L$の場合、

$$
X_+(f(u^m)) =f(X_+u^m) = 0,H(f(u^m)) =f(Hu^m) =mf(u^m)
$$

だから$f(u^m)\in P_m\cup  \{0\}$。 $e$ によって生成された E の $e\in P_m$ と V 部分加群とします。提案 1 により、加群 $V(m)$ から加群 V まで、$u^m$ から $e$ にかかる同型が存在します。続いて$L(u^m) = P_m\cup  \{0\}$。

#### 系 {#lie-viii-s1-n3-cor-1 .statement tag=00Y7}

型 $V(m)$ の E の同型成分には長さがあります

薄暗い(P$_m\cup  \{0\}$.

### 4. 群 SL(2$\boldsymbol{, k}$)の線型表現

Recall (Algebra, Chap. III, §8, no. 9) that we denote by $\mathbf{S}\mathbf{L}(2, k)$ the group of square matrices of order 2 with coefficients in $k$ whose determinant is equal to 1. $x\in \mathfrak{s}\mathfrak{l}(2, k)$ が無能である場合、$x^2= 0 ($代数、第 4 章。 VII, §5、コル。提案 5 の 3) および$e^x= 1 +x\in \mathbf{S}\mathbf{L}(2, k)$。 If E is a finite dimensional vector space and $\rho$ is a linear representation of $\mathfrak{s}\mathfrak{l}(2, k)$ on E, then $\rho (x)$ is nilpotent and so $e^{\rho(x)}$ is defined (Chap. I, §6, no. 3).

#### 定義 2 {#lie-viii-s1-def-2 .statement tag=00Y8}

E を有限次元ベクトル空間とし、E 上の $\mathfrak{s}\mathfrak{l}(2, k)$ (それぞれ $\mathbf{S}\mathbf{L}(2, k)$) の $\rho$ (それぞれ $\pi$ ) 線型表現とします。すると、冪零元ごとに、$\rho$ と $\pi$ は互換性があると言われます。 $\mathfrak{s}\mathfrak{l}(2, k),\pi (e^x) =e^{\rho(x)}$中$x$。

In other words, $\rho$ and $\pi$ are compatible if, for every nilpotent element $x$ of $\mathfrak{s}\mathfrak{l}(2, k)$, the restriction of $\rho$ to $kx$ is compatible with the restriction of $\pi$ to the group $1 +kx$ (Chap. VII, §3, no. 1).

$\rho$ と $\pi$ が互換性がある場合、$\rho$ と $\pi$ の二重表現、$m$ 番目のテンソル冪、$m$ 番目の対称冪も互換性があります（第 2 章）。 VII, §5, no. 4、補題 1 (i) および (ii))。同様に、ベクトル部分空間で$\rho$ と $\pi$ によって誘発された表現も、$\rho$ と $\pi ($ loc の下で安定しています。引用）。

特に、$V(m)$ (no. 3) 上の $\mathfrak{s}\mathfrak{l}(2, k)$ の表現 $\rho_m$ は、$\mathbf{S}\mathbf{L}(2, k)$ の恒等表現 $\pi_1$ の $m$ 対称べき乗 $\pi_m$ と互換性があります。 上記のように $e^{(m)}_n=(^m_n)u^{m-n}v^n$ を置くと、

$(m)(m)m-nn$

$\pi_m(s)e_n$ = $(su)(sv)$ (3)

$$
n
$$

$s\in \mathbf{S}\mathbf{L}(2, k)$ と $0\leq n\leq m$ の場合。

#### 定理 2 {#lie-viii-s1-thm-2 .statement tag=00Y9}

$\rho$ を有限次元ベクトル空間 E 上の $\mathfrak{s}\mathfrak{l}(2, k)$ の線型表現とします。

(i) E には、$\rho$ と互換性のある$\mathbf{S}\mathbf{L}(2, k)$ の固有の線型表現 $\pi$ が存在します。

(ii) ベクトル部分空間 E の F は、$\rho$ で安定している場合に限り、$\pi$ で安定します。

(iii) $x\in E$ とします。次に、$x$ が $\rho ($ の下で不変である場合に限り、すべての $s\in \mathbf{S}\mathbf{L}(2, k)$ に対して $\pi (s)x=x$、つまりすべての $a\in \mathfrak{s}\mathfrak{l}(2, k))$ に対して $\rho (a)x= 0$ になります。

$\pi$ の存在は、前と Th に続きます。 1. 一方、群 $\mathbf{S}\mathbf{L}(2, k)$ は形の元によって生成されることがわかります。

$$
_{tX}(1t)_{-tX_-}(10)
$$

$e^+=e$ =

0 1 $t$ 1

ここで、$t\in k($代数、章。 III, §8, no. 9、提案 17)。これは$\pi$の一意性を証明します。

主張 (ii) と (iii) は、第 1 章と合わせて、これまで述べたことに続きます。 VII, §3, no. 1、補題 1 (i)。 Q.E.D.

したがって、すべての有限次元 $\mathfrak{s}\mathfrak{l}(2, k$) 加群は固有の $\mathbf{S}\mathbf{L}(2, k)$ 加群構造を持ち、これはその $\mathfrak{s}\mathfrak{l}(2, k$) 加群構造に関連付けられていると言われています。

#### 注意 {#lie-viii-s1-n4-rem-1 .statement tag=00YA}

$k$ が $\mathbf{R}$ または $\mathbf{C}$、または完全な非離散ウルトラメトリック体である場合、$\mathfrak{s}\mathfrak{l}(2, k)$ は $\mathbf{S}\mathbf{L}(2, k)$ のリー代数です。 $\rho$ と $\pi$ を Th のようにします。 2. 準同型 $\pi$ は、$\mathbf{S}\mathbf{L}(2, k)$ から $\mathbf{G}\mathbf{L}(E):$ までのリー群の準同型です。これは $E = V(m)$ の時点で明らかであり、Th を考慮すると、一般的な場合は次のようになります。 1. 章による。 VII, §3、いいえ。 $1,\rho (X_+) = L(\pi )(X_+),\rho (X_-) = L(\pi )(X_-)$。したがって、$\rho = L(\pi )$ (逆については、例題 18 を参照)。

#### 命題 5 {#lie-viii-s1-prop-5 .statement tag=00YB}

E、F を有限次元 $\mathfrak{s}\mathfrak{l}(2, k)$ 加群とし、$f\in$ Hom$_k(E,F)$ とします。次の条件は同等です。

(i) $f$ は $\mathfrak{s}\mathfrak{l}(2, k)$ モジュールの準同型です。

(ii) $f$ は、$\mathbf{S}\mathbf{L}(2, k)$ モジュールの準同型です。

条件 (i) は、$f$ が $\mathfrak{s}\mathfrak{l}(2, k$) モジュール Hom$_k(E,F)$ の不変式元であることを意味し、条件 (ii) は、$f$ が $\mathbf{S}\mathbf{L}(2, k$) モジュールの不変式元であることを意味しますホム$_k(E,F)$。これらの加群構造は Chap によって関連付けられているため、 VII, §5, no. 4、補題 1 (iii)、命題は Th から続きます。 2(iii)。

#### 定義 3 {#lie-viii-s1-def-3 .statement tag=00YC}

群 $\mathbf{S}\mathbf{L}(2, k)$ の随伴表現は、$\mathfrak{s}\mathfrak{l}(2, k)$ 上の $\mathbf{S}\mathbf{L}(2, k)$ の線型表現 Ad です。

広告($s$)$.a=sas^{-1}$

すべての$a\in \mathfrak{s}\mathfrak{l}(2, k)$とすべての$s\in \mathbf{S}\mathbf{L}(2, k)$に。 $k$ が $\mathbf{R}$ または $\mathbf{C}$、または完全な非離散ウルトラメトリック体である場合、Def は回復します。第7章III, §3, no. 12 (cf. 引用文献、提案 49)。

章著。 VII, §5, no. 4、補題 1 (i) および (ii)、$\mathfrak{s}\mathfrak{l}(2, k)$ と $\mathbf{S}\mathbf{L}(2, k)$ の随伴表現は互換性があります。章著。 VII, §3, no. 1、注意 2、広告($\mathbf{S}\mathbf{L}(2, k)$) $=$ Aut$_e(\mathfrak{s}\mathfrak{l}(2, k))$。

### 5. SL 元一部 (2$\boldsymbol{, k}$)

$t\in k^*$ には、次のように入力します。

$$
\theta (t) =e^{tX_+}e^{t^{-1}X_-}e^{tX_+}
$$

$(1t)(($ 1 $0)((1t)$

= 0 1 $-t^{-1}$ 1 0 1

$($ 0t)

= $-t^{-1}$ 0

$$
=e^{t^{-1}X_-}e^{tX_+}e^{t^{-1}X_-}
$$

no. 3 の記法では、

$$
\theta (t)u=-t^{-1}v\theta (t)v=tu
$$

それで

$$
\theta (t)e^{(m)}_n= (-1)^{m-n}t^{2n-m}e^{(m)}_{m-n} \tag{4}
$$

したがって、元 $\theta (t)^2=(-1$ 0 $)$ は、$V(m)$ に $(-1)^m$ によって演算されます。もし

0 $-1$

E は奇数次元の単純な $\mathfrak{s}\mathfrak{l}(2, k$) 加群であるため、$\theta (t)_E$ はベクトル空間 E の包含自己同型です。特に、E を随伴体表現とすると、次のようになります。

$$
\theta (t)_EX_+=t^{-2}X_-\theta (t)_EX_-=t^2X_+\theta (t)_EH=-H \tag{5}
$$

そのため、$\theta (1)_E=\theta (-1)_E$ は $\mathfrak{s}\mathfrak{l}(2, k)$ の正準累乗となります。

$t\in k^*$ には、

$$
h(t) =(0tt^-0_1)=\theta (t)\theta (-1)
$$

それから$h(t)u=tu,h(t)v=t^{-1}v$なので、

$$
h(t)e^{(m)}_n=t^{m-2n}e^{(m)}_n \tag{6}
$$

#### 命題 6 {#lie-viii-s1-prop-6 .statement tag=01L4}

E を有限次元の $\mathfrak{s}\mathfrak{l}(2, k)$ 加群、および $t\in k^*$ とします。 $E_p$ を重み $p$ の E の元の集合とします。

(i) $\theta (t)_E|E_p$ は、$E_p$ から $E_{-p}$ までの全単射です。

(ii) $h(t)_E|E_p$ はホモテティー で、$E_p$ に対する比率は $t^p$ です。

$E = V(n)$ の場合、公式 (4) と (6) から命題が続きます。一般的なケースは Th から導き出されます。 1.

#### 系 {#lie-viii-s1-n5-cor-1 .statement tag=00YD}

$E = E'\oplus E''$ を Cor で定義されている E の分解とします。提案 2. $\mathbf{S}\mathbf{L}(2, k)$ の元 $(-10)$ は、$E'$ に +1 で作用します

0 $-1$

そして$E''$の$-1$までに。

これは (ii) に続き、$t=-1$ に適用されます。

### 練習問題 {#lie-viii-s1-exercises}

基礎体 $k$ は標数0 のものであると想定されます。

〜でない限り明示的にそうでない場合、リー代数は有限次元であると想定されます。

$\mathfrak{s}$ リー代数 $\mathfrak{s}\mathfrak{l}(2, k)$ で表します。

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
