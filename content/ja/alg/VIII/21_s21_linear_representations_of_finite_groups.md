---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 21
section_title: Linear Representations of Finite Groups
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.397-A VIII.434
pdf_pages: 0414-0451
extraction: native+ocr
subsections:
    - "no": 1
      title: Linear Representations
      page: 397
      pdf_page: 414
    - "no": 2
      title: Maschke’s Theorem
      page: 401
      pdf_page: 418
    - "no": 3
      title: Induced and Coinduced Representations
      page: 402
      pdf_page: 419
    - "no": 4
      title: Representations and the Grothendieck Group
      page: 404
      pdf_page: 421
    - "no": 5
      title: Fourier Inversion Formula
      page: 406
      pdf_page: 423
    - "no": 6
      title: Schur Orthogonality Relations
      page: 409
      pdf_page: 426
    - "no": 7
      title: Orthogonality Relation for Characters
      page: 410
      pdf_page: 427
    - "no": 8
      title: Central Functions on a Finite Group
      page: 411
      pdf_page: 428
    - "no": 9
      title: The Case of Abelian Groups
      page: 414
      pdf_page: 431
    - "no": 10
      title: Characters and Grothendieck Groups
      page: 415
      pdf_page: 432
    - "no": 11
      title: Dimension of Simple Representations
      page: 415
      pdf_page: 432
    - "no": 12
      title: Change of Base Field
      page: 416
      pdf_page: 433
    - "no": 13
      title: Complex Linear Representations
      page: 421
      pdf_page: 438
statements: 36
exercises: 30
content_sha256: a39b4fae8ba03a1a6aca3fa70ca2b80ef512889332253d738436b2b66e489a0a
translated_from: content/en/alg/VIII/21_s21_linear_representations_of_finite_groups.md
translation_method: google
source_content_sha256: 9b88499ec4cd1b75b385f04753440e80043e0341bcb3af756c5dd1b9f9bd76d6
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: cec170b187b96a5548694b303eede09b2db6189eab902907d550fdb3745008f0
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 21。 有限群中線型表現

この切断では、Gは群、Kは可換環です。 G が有限群の場合、K の $|G|$ 元 Card(G)$\cdot 1$ で表します。 No. 5 以降、群 G は有限で、環 K は代数閉体で、$|G|$ は有限であると仮定します。 零。

### 1. 線型表現

#### 定義 1 {#alg-viii-s21-def-1 .statement tag=00NC}

M をK-加群とします。 M の G の線型表現は、G から線形群 $\mathbf{G}\mathbf{L}(M)$ (II, §1, No. 2, p. 195) への群準同型です。

$\pi$ を K-加群 M の G の線型表現とします。また、対 $(M, \pi )$ は G の線型表現であるとも言います。 K が非零で M が自由K-加群のとき、M の次元はと呼ばれます表現 $\pi$ の次数 (または次元)。

G から群 G の代数 K[G] までの標準写像 $g\mapsto e_g$ は、K-加群 K[G] の基底であることを思い出してください。 記法の乱用により、K[G] の元 $e_g$ を $g$ で表します。 G の線型表現 $\pi : G\rightarrow \mathbf{G}\mathbf{L}(M)$ が与えられると、K[G] から End$_K(M)$ まで、拡大する $\pi$ (III, §2, No. 6, p. 447, 例) である K-代数の一意な準同型が存在します。また、この拡大を $\pi$ で表します。 M (VIII, p. 373, 定義 1) の代数 K[G] の表現であるため、M は K[G] モジュールです。逆に、M の代数 K[G] のすべての線型表現 $\rho$ は、$g\mapsto \rho (g)$ によって与えられる M の G の定義する線型表現です。

K[G]モジュール構造に関する用語を群 Gの線型表現に自由に適用します。たとえば、部分表現、単純な表現、表現の直和などについて話します。$(M, \pi )$と$(M', \pi ')$を次のようにします。 Gの線型表現; M から $M'$ までの K[G] 加群の準同型の Hom$_G(\pi , \pi ')$ K-加群 Hom$_{K[G]}(M,M')$ で表します。[^1]

G の元のすべての対 $(g, g')$ に $f(gg') =$ $f(g'g)$ がある場合、G から K までの写像 $f$ は中心写像と呼ばれます。等価的に、G の元 $g, h$ のすべての対に対して $f(ghg^{-1}) =$ $f(h)$ が得られます。従って、中央の写像は G 上の写像であり、各共役類に対する制限は定数です。 G から K までは、形部分加群、空間、写像で、$\mathscr{Z}_K(G)$ で示されます。 G が有限の場合、K-代数 $\mathscr{Z}_K(G)$ は、G の次元の自由K-加群共役類の数です。 代数 K[G] の中心 Z(K[G]) は、元で構成されます$h\in G$ごとに$hah^{-1}=a$となるようなK[G]の$a=\sum a_gg$。さて、私たちは

$$
hah^{-1}=\sum_{g\in G}a_{h^{-1}gh}g
$$

従って、G が有限の場合、代数 K[G] の中心 Z(K[G]) は中心の写像で構成されます。

$(M, \pi )$ を G の線型表現とします。M を有限次元自由K-加群とします。 $\pi$ のトレースは、$\pi$ に関連付けられた K[G] の表現のトレース、つまり (VIII, p. 382)、K[G] 上の線型形式 $a\mapsto$ Tr($\pi (a)$) です。この線型形式は、G から K までの写像 $g\mapsto$ Tr($\pi (g)$) によって決定され、これを表現 $\pi$ の指標と呼び、$\chi_{\pi}$ で表します。 表現の指標は中央の写像 (II, §4, No. 3、p. 273、命題 3) です。

M と $M'$ を有限次元自由K-加群とします。 $\pi$ と $\pi '$ をそれぞれ M の G の線型表現と $M'$ とします。すると、$M\oplus M'$ は有限次元自由K-加群となり、命題 III, §9, No. 2 の 1、p. 543 により、次のようになります。

$$
\chi_{\pi\oplus\pi'}=\chi_{\pi}+\chi_{\pi'}
$$

より一般的には、

$$
0\longrightarrow M'\longrightarrow M\longrightarrow M''\longrightarrow 0
$$

K[G] 加群の完全系列を、$\pi ,\pi '$ と $\pi ''$ を、それぞれ $M, M'$ と $M''$ に関連付けられた G の線型表現とします。 K-加群 $M'$ と $M''$ が自由で有限次元であると仮定します。次に、M (II, §1, No. 11、p. 218、命題 21) も同様です。

$$
\chi_{\pi}=\chi_{\pi'}+\chi_{\pi''} \tag{1}
$$

#### 命題 1 {#alg-viii-s21-prop-1 .statement tag=00ND}

K が可換体であるとします。 $\pi$ と $\pi '$ を G の有限次元半単純 K 線形表現とします。

a) $\pi (g)$ と $\pi '(g)$ の特性多項式がすべての $g\in G$ で同じである場合、表現 $\pi$ と $\pi '$ は同型です。

b) さらに、K が標数 0 を持つとします。指標 $\chi_{\pi}$ と $\chi_{\pi'}$ が等しい場合、表現 $\pi$ と $\pi '$ は同型です。

主張 a) 系 1/VIII、p. 386 から続きます。 主張 b) は、VIII、p. 384 の系の部分 a) から続きます。

#### 例 1 {#alg-viii-s21-n1-exa-1 .statement tag=00NE}

G の単位元または自明な表現は表現 $(K, \varepsilon )$ であり、$g\in G$ ごとに $\varepsilon (g) =$ Id$_K$ です。その指標は、値 1 を持つ定数写像です。

#### 例 2 {#alg-viii-s21-n1-exa-2 .statement tag=00NF}

G の (左) 正則表現は、$g\in G$ と $x\in K[G]$ に対して $\boldsymbol{\gamma }(g)(x) =gx$ によって定義される K[G] の G の表現 $\boldsymbol{\gamma }$ です。 代数 K[G] (VIII, p. 375) の正則表現の左に対応するあります。 群 G が有限であると仮定します。 正則表現には有限次数があります。単位と異なる G の元 $g$ ごとに、標準基底に関して K[G] で $g$ だけ左の乗法の行列は、点を固定せずに置換の行列になります。したがって、私たちは

$|G|$ $g$ が単位元の場合、

$$
\chi_{\boldsymbol{\gamma }}(g) = \tag{2}
$$

それ以外の場合は 0。

私たち定義するも同様にGの右側正則表現です。 G の複正規表現は、$(g, g')\in G\times G$ と $x\in K[G]$ の $\rho (g, g')(x) =gxg^{'-1}$ によって定義される K[G] の $G\times G$ の表現 $\rho$ です。

#### 例 3 {#alg-viii-s21-n1-exa-3 .statement tag=00NG}

G の線型表現 $(M, \pi )$ が与えられると、$\pi$ の対数または双対表現 $\pi^{\vee}$ は、$g\in G$ (cf.) ごとに関係 $\pi^{\vee}(g) =^t\pi (g^{-1})$ によって定義される M に対する双対 K-加群における G の表現です。 II, §2, No. 5、p. 234）。 M が有限次元自由K-加群である場合、その双対も同様であり、すべての $g\in G$ に対して $\chi_{\pi^{\vee}}(g) =\chi_{\pi}(g^{-1})$ が得られます。

#### 例 4 {#alg-viii-s21-n1-exa-4 .statement tag=00NH}

$(M, \pi )$と$(M', \pi ')$をGの線型表現とします。VIII、p. 198の例1では、$M\otimes_KM'$にK[G]モジュール構造を定義しました。 対応する線型表現は、$\pi$ と $\pi '$ のテンソル積と呼ばれ、$\pi \otimes \pi '$ で表されます。 $g\in G,x\in M$ と $x'\in M'$ の場合は、$((\pi \otimes \pi ')(g))(x\otimes x') =\pi (g)x\otimes \pi '(g)x'$ になります。

M と M' が有限次元自由K-加群の場合、III, §9, No. 2、p. 543 の命題 2 により、次のようになります。

(3)
$$
\chi_{\pi \otimes \pi'} = \chi_{\pi} \chi_{\pi'}.
$$

#### 例 5 {#alg-viii-s21-n1-exa-5 .statement tag=00NI}

G が 2 つの群の積 $G' \times G''$ であると仮定します。 $K[G'] \otimes_K K[G'']$ から $K[G]$ までの K-線型写像は、$g' \in G'$ に対して $g' \otimes g''$ から $(g', g'')$ を送信し、$g'' \in G''$ は代数同型です。 $(M', \pi')$ を $G'$ の線型表現および $G''$ の $(M'', \pi'')$ 線型表現とします。 $\pi' \otimes \pi''$ で示される $\pi'$ と $\pi''$ の外部テンソル積は、$(g', g'') \in G' \times G''$ の $(\pi' \otimes \pi'')(g', g'') = \pi'(g') \otimes \pi''(g'')$ によって定義されるベクトル空間 $M' \otimes M''$ の $G' \times G''$ の表現です。 $M'$ と $M''$ が有限次元自由K-加群の場合、$M' \otimes_K M''$ は有限次元自由K-加群で、表現 $\pi' \otimes \pi''$ の指標は公式で与えられます。
$$
\chi_{\pi' \otimes \pi''}(g', g'') = \chi_{\pi'}(g') \chi_{\pi''}(g'')
$$
$g' \in G'$ と $g'' \in G''$ 用 (命題 III, §9, No. 2、p. 542 の 2)。

#### 例 6 {#alg-viii-s21-n1-exa-6 .statement tag=00NJ}

$(V, \pi)$ を G の線型表現とし、V が有限次元自由K-加群となるようにします。私たちは定義する表現 $\rho$/$G \times G$ で $\operatorname{End}_K(V)$ までに公式
$$
\rho(g, g')(u) = \pi(g') \circ u \circ \pi(g^{-1}).
$$
K-加群同型 $\theta_V : V^* \otimes_K V \to \operatorname{End}_K(V)$ の II, §4, No. 2、p. 271 は、外部のテンソル積 $\pi^\vee \otimes \pi$ から $\rho$ からの表現の同型です。 写像 $g \mapsto \rho(1, g)$ (それぞれ $g \mapsto \rho(g, 1)$) は、$\pi^{\dim_K V}$ (それぞれ $(\pi^\vee)^{\dim_K V}$) と同型の G の表現です。

L を可換K-代数とし、$(M, \pi)$ を群 G の線型表現とします。 $g \mapsto \operatorname{Id}_L \otimes \pi(g)$ によって定義される群準同型 $\pi_{(L)} : G \to \mathbf{GL}(M_{(L)})$ は、L モジュール $M_{(L)}$ の G の線型表現です。 表現 $\pi$ から、スカラー K の環の拡大からL までの G の線型表現が推定されます。

K が体で、L が非零可換 K 代数であると仮定します。 $(M, \pi)$ と $(M', \pi')$ を G の線型表現とします。 表現 $\pi$ と $\pi'$ は、$\pi_{(L)}$ と $\pi'_{(L)}$ が (VIII, p. 37, 定理 3) である場合にのみ同型です。

さらに、代数 L が K の拡大であるとします。 VIII、p. 198 の例 1 で定義された環 $R_K(G)$ と $R_L(G)$ を考えてみましょう。スカラーの拡大定義する環準同型
$$
u : R_K(G) \longrightarrow R_L(G).
$$

この準同型は単射的であり、元 $\xi \in R_K(G)$ は、$u(\xi )$ が (VIII、p. 195、定理 1) である場合にのみ有効です。

### 2. マシュケさん定理

#### 定理 1 {#alg-viii-s21-thm-1 .statement tag=00NK}

群 G が有限であると仮定します。 M を K[G] モジュール、N を M の K[G] サブモジュールとしましょう。N が K-加群 M の直因子であり、$|G|$ が K で可逆であると仮定します。そのとき、N は K[G] モジュール M の直因子です。

$p$ を、像 N を持つ M の K 線形射影子とします。K-加群 M の設定の定義する自己準同型 $q$

$$
q(x) =|G|^{-1}\sum_{g\in G}g p(g^{-1}x)
$$

$x\in M$ごとに。 N は G の作用および N 上の恒等式 $p$ 誘導するの下で安定しているため、$q$ が M を N に送信し、N 上の恒等式誘導するを送信することがわかります。

従って、K-加群 M は、$q$ の像 N の直和と $q$ の核です。すべての $x\in M$ と $g\in G$ に対して $g q(x) =q(gx)$ があるため、$q$ の核は M の K[G] 部分加群です。これは、N が K[G] 加群 M の直因子であることを証明します。

#### 系 1 (マシュケ) {#alg-viii-s21-thm-1-cor-1 .statement tag=00SC}

群 G が有限で、K が可換体であると仮定します。 代数 K[G] は、体 K の元 $|G|$ が零ではない場合に限り、半単純になります。

$|G| \not= 0$ と仮定します。 定理 1 までに、$K[G]_s$ のすべての K[G] サブモジュールは直因子になります。従って、K[G] は半単純です。

逆に、$|G|$が零だとし、K[G]の中心の$\varepsilon$元$\sum_{g\in G}g$で表します。 $\varepsilon \not= 0$ はありますが、$\varepsilon^2=|G|\varepsilon = 0$ なので、K[G] は半単純 (VIII, p. 153, 命題 3, a) および VIII, p. 157, 注意 1) ではありません。

#### 系 2 {#alg-viii-s21-thm-1-cor-2 .statement tag=00NL}

群 G は有限で、$|G|$ は K で可逆であるとします。K[G] 加群分裂の完全系列は、分裂が K-加群の完全系列である場合に限ります。

完全系列の K[G] モジュールが与えられる

0 // ${M'}^f$ // M // $M''$ // $0$,

射 $f$ の定理を適用する 1 ～ 像で十分です。

#### 系 3 {#alg-viii-s21-thm-1-cor-3 .statement tag=00NM}

群 G が有限で、$|G|$ が K において可逆であると仮定します。K[G] 加群は、K-加群のように射影である場合にのみ射影です。

P を K[G] モジュールとする。 P が自由な K[G] モジュール M の直因子である場合、それは自由K-加群 M のなおさら直因子です。 逆は、II, §2, No. 2、p. 231 を考慮して、系 2 から続きます。 命題 4、d）。

#### 系 4 {#alg-viii-s21-thm-1-cor-4 .statement tag=00NN}

a) 群 G が有限で、K が標数 0 の可換体であると仮定します。 G の 2 つの有限次元線型表現は、同じ指標を持つ場合にのみ同型です。

b) K が素数数 $p$ の完全体であり、群 G が $p$ までの素数基数の有限であると仮定します。 G の有限次元線型表現の指標は、この表現が $p$ の対同型表現の直和と同型である場合に限り、 零になります。

系の仮定では、G のすべての有限次元線型表現は半単純です。 VIII、p. 384の系から系が続きます。

#### 系 5 {#alg-viii-s21-thm-1-cor-5 .statement tag=00NO}

群 G が有限で、K が $|G| \not= 0$ である可換体であると仮定します。 $\pi$ と $\pi '$ を G の有限次元線型表現とします。すると、G のすべての $g$ について、自己準同型 $\pi (g)$ と $\pi '(g)$ が同じ特性を持つ場合に限り、$\pi$ と $\pi '$ は同型になります。多項式。

これは、VIII、p. 386の系1から続きます。

### 3. 誘発および共誘発表現

H を群 G の部分群とします。

$(V, \pi )$ が G の線型表現である場合、H に対する $\pi$ の制限は、V の H の線型表現です。これを Res$^G_H(\pi )$ で表します。 Res$^G_H(\pi )$ に関連付けられた K[H]加群は、スカラー (II, §1, No. 13, p. 221) の制限によって K[G] モジュール V から単純に加群と推定されます。 Vが有限次元自由K-加群なら、Res$^G_H(\pi )$の指標は$\pi$の指標の制限になります。

$(M, \sigma )$をHの表現とします。

K[G] を $(K[G]$、K[H]) バイモジュール、M を K[H] モジュールと見なします。 G の K[G] モジュール $\mathscr{T}(M) = K[G]\otimes_{K[H]}M$ (VIII, p. 58) 定義する線型表現は、Ind$^G_H(\sigma )$ で示され、$\sigma$ によって誘導される G の表現と呼ばれます。 $(V, \pi )$ が G の線型表現である場合、K[H] モジュール $\mathscr{H}(V) =$ Hom$_{K[G]}(K[G],V)$ は、K[H] モジュール対応するから表現 Res$^G_H(\pi )$ と識別できます。その結果、随伴射 (VIII, p. 59) は、Hom$_H(\sigma$、Res$^G_H(\pi ))$ から Hom$_G$(Ind$^G_H(\sigma ), \pi$ ) まで、正規と呼ばれる K-加群同型を与えます。 (「フロベニウスの相互法則」)。

K[G] を $(K[H]$, K[G]) バイモジュールと見なします。 G の K[G] 加群 $\mathscr{H}(M) =$ Hom$_{K[H]}(K[G],M)$ 定義する表現は Coind$^G_H(\sigma )$ で示され、$\sigma$ によって共誘起される G の表現と呼ばれます。 $(V, \pi )$ が G の線型表現である場合、K[H] モジュール $\mathscr{T}(V) = K[G]\otimes_{K[G]}V$ は K[H] モジュール対応するから表現 Res$^G_H(\pi )$ と識別できます。その結果、随伴射 (上記参照) は、Hom$_H$(Res$^G_H(\pi ), \sigma$ ) から Hom$_G(\pi$、Coind$^G_H(\sigma ))$ まで、正規と呼ばれる K-加群同型を与えます。

$\varepsilon : K[G]\rightarrow K[H]$ を、$h\in$ H の場合は関係 $\varepsilon (h) =h$、$g\in G$ - H の場合は $\varepsilon (g) = 0$ によって特徴付けられる K-加群準同型とします。 写像 $\varepsilon$ は $(K[H]$ の準同型です、 K[H])-ビモジュール。 $(M, \sigma )$ を H の線型表現とします。 Hom$_{K[H]}(K[H],M)$ から Hom$_{K[H]}(K[G],M)$ までの写像 $v\mapsto v\circ \varepsilon$ は、K[H] 加群の準同型です。 M を Hom$_{K[H]}(K[H],M)$ と同定することで、M から Res$^G_H$(Coind$^G_H(\sigma )$) までの K[H] モジュールの準同型が得られます。 フロベニウスの相互法則は、関係によって特徴付けられる Ind$^G_H(\sigma )$ から Coind$^G_H(\sigma )$ までの K[G] モジュールの準同型 $\iota$ にそれを送信します。

$$
\iota (g\otimes m)(g') =\varepsilon (g'g)m
$$

$g, g'\in G$ と $m\in M$ の場合。この準同型は正規と呼ばれます。

#### 命題 2 {#alg-viii-s21-prop-2 .statement tag=00NP}

H を G の部分群とし、$(M, \sigma )$ を H の線型表現とします。 標準準同型 $\iota :$ Ind$^G_H(\sigma )\rightarrow$ Coind$^G_H(\sigma )$ は単射です。 部分群 H が G に有限の添字を持つ場合、$\iota$ は K[G] 加群の同型です。

$S\subset G$を$G/H$の代表の系とします。ファミリ $(s)_{s\in S}$ は、右側の K[H] モジュール K[G] の基底です。従って、$(m_s)_{s\in S}\mapsto \sum_{s\in S}s\otimes m_s$ によって定義される写像 $M^{(S)}\rightarrow$ Ind$^G_H(\sigma )$ は、K-加群の同型であることがわかります。すべての $s, s'\in S$ とすべての $m\in M$ について、関係があります。

$$
\iota (s'\otimes m)(s^{-1}) =\begin{cases} m & \text{if } s=s',\\ 0 & \text{otherwise.}\end{cases}
$$

従って、$\iota '$ は単射法であることがわかります。

H の G に有限の添字があるとします。 集合 S は有限です。 $\rho$ を、$u\mapsto \sum_{s\in S}s\otimes u(s^{-1})$ で与えられる Coind$^G_H(\sigma )$ から Ind$^G_H(\sigma )$ までの写像とします。 $u\in$ Coind$^G_H(\sigma )$ と $s\in S$ に対して $(\iota \circ \rho (u))(s^{-1}) =u(s^{-1})$ を満たします。 ファミリ $(s^{-1})_{s\in S}$ は左 K[H]-モジュール K[G] の基底であるため、写像 $\iota \circ \rho$ は恒等写像です。 従って、$\iota$ は逆全単射 $\rho$ と全単射です。

H を有限添字の G の部分群とします。 $u$ を H の中心写像とします。 G 上の $u^0$ 写像によって拡大する $u$ が表され、G - H の点ごとに零になります。S を $G/H$ の代表の系とします。 $g\in G$、集合の場合

(4) インド$^G_H(u)(g) =\sum_{s\in S}u^0(s^{-1}gs)$。

すべての $x, g\in G$ とすべての $h\in H$ について、$u^0((xh)^{-1}gxh) =$ $u^0(x^{-1}gx)$ があることに注意してください。したがって、Ind$^G_H(u)$ は S の選択に依存しない G 上の中心写像であることがわかります。したがって、$\mathscr{Z}_K(H)$ から $\mathscr{Z}_K(G)$ までの定義する K-線型写像 Ind$^G_H$ となります。

#### 命題 3 {#alg-viii-s21-prop-3 .statement tag=00NQ}

H を有限添字の G の部分群とします。 $(M, \sigma )$ を H の線型表現とします。M を有限次元自由K-加群とします。 $\sigma$ によって誘発された G の $(V, \pi )$ 表現で表します。すると、K-加群 V は自由で有限次元となり、

(5) $\chi_{\pi}=$ 指標$^G_H(\chi_{\sigma})$。

S を $G/H$ の代表者の系とします。上で見たように、$(m_s)_{s\in S}\mapsto \sum_{s\in S}s\otimes m_s$ によって与えられる線形写像 $M^S\rightarrow$ Ind$^G_H(M)$ は K-加群同型です。特にVは有限次元自由K-加群です。任意の $g\in G$ については、M の $M_g$ 像を写像 $m\mapsto g\otimes m$ で表します。すべての $g, g'\in G$ について、$gH =g'H$ の場合にのみ $M_g= M_{g'}$ があり、V は $s\in S$ の部分加群 $M_s$ の直和です。すべての$g, g'\in G$に対して、$\pi (g)M_{g'}= M_{gg'}$もあります。任意の $g\in G$ については、$s^{-1}gs\in H$ となるように S の元 $s$ の $S_g$ 集合で表します。 $g^{'-1}gg'\in H$、自己同型 $\pi (g)$/V 誘導する自己同型 $\pi (g)_{g'}$/$M_{g'}$ などのすべての $g, g'\in G$ について、

Tr($\pi (g)$) $=\sum_{s\in S_g}$ Tr($\pi (g)_s$) $=\sum_{s\in S_g}$ Tr($\sigma (s^{-1}gs)$)。

命題の最後の主張が続きます。

### 4. 表現とグロタンディーク群

この小節では、Kが可換体であると仮定します。 G の有限次元線型表現 $(M, \pi )$ を考えると、グロタンディーク環 $R_K(G)$ (VIII, p. 198, 例 1) の K[G] 加群 M の $[\pi ]$ 類で表します。

環 $R_K$(G) 上の合成の法則の定義により、$\pi$ と $\pi '$ が G の有限次元線型表現である場合、次のようになります。

$$
[\pi \oplus \pi '] = [\pi ] + [\pi '],[\pi \otimes \pi '] = [\pi ] [\pi ']
$$

環 $R_K(G)$ の単位元は、G の単位表現の類です (VIII、p. 399、例 1)。

環 $R_K(G)$ は、K 上の有限次元の単純な K[G] 加群の類の基底集合を備えた自由な $\mathbf{Z}$ 加群です。 $|G|$ が K で可逆であるとき、2 つの有限次元表現は、 $R_K(G)$ の類 (VIII、p. 190、系および p. 401、系 1) も同様です。

G のすべての有限次元線型表現 $(M, \pi )$ に対して、反比例 $\pi^{\vee}$ も有限次元です。 表現 $\pi$ と $(\pi^{\vee})^{\vee}$ は同型です。 $\pi '$ も G の有限次元線型表現である場合、表現 $(\pi \otimes \pi ')^{\vee}$ と $\pi^{\vee}\otimes \pi^{'\vee}$ は同型です。もし

$$
0\longrightarrow M'\longrightarrow M\longrightarrow M''\longrightarrow 0
$$

は K 上の有限次元の K[G] 加群の完全系列である場合、反比例表現は K[G] 加群の完全系列を与えます

$$
0\longrightarrow M^{''\vee}\longrightarrow M^{\vee}\longrightarrow M^{'\vee}\longrightarrow 0
$$

(II, §7, No. 5、p. 299、系/定理 5)。 グロタンディーク群 (VIII, p. 186, 命題 4) の普遍性により、すべての有限次元線型表現に対して $[\pi ]^{\vee}= [\pi^{\vee}]$ によって特徴付けられる環 $R_K(G)$ の自己同型 $c\mapsto c^{\vee}$ が存在します。 Gの$\pi$; $R_K(G)$ の元 $c$ ごとに $(c^{\vee})^{\vee}=c$ があります。

H を G の部分群とします。制限は完全系列を保持します。 グロタンディーク群 (上記参照) の普遍性により、結果として、関係によって特徴付けられる $R_K(G)$ から $R_K(H)$ まで、Res$^G_H$ で示される群準同型が存在します。

(6) レス$^G_H[\pi ] =$ [レス$^G_H(\pi )]$]

G のすべての有限次元線型表現 $\pi$ に対して。 環準同型です。 H が G に有限の添字を持つ場合、II, §7, No. 7、p. 306 の命題 14 によって、定義するができます。同様に、関係によって特徴付けられる $R_K(H)$ から $R_K(G)$ までの群準同型 Ind$^G_H$ ができます。

(7) インド$^G_H[\sigma ] =$ [インド$^G_H(\sigma )]$]

H のすべての有限次元線型表現 $\sigma$ に対して。

VIII、p. 399 の関係 (1) および VIII、p. 400 の関係 (3) と上記のグロタンディーク群の普遍的性質により、G 上の中心関数の代数 $\mathscr{Z}_K(G)$ への $R_K(G)$ から環準同型性 $\Theta_G$ が存在し、すべての関数に対して $\Theta_G([\pi ]) =\chi_{\pi}$ によって特徴付けられます。 G の有限次元表現 $\pi$

H が G の部分群である場合、群 G と H に関連付けられた準同型 $\Theta_G$ と $\Theta_H$ は、演算 Res$^G_H$ および Ind$^G_H$ (VIII、p. 402、VIII、 p. 404、命題 3)。

G が 2 つの群の積 $G'\times G''$ であるとします。 VIII、p. 213、注意 2 により、$\pi '$ に対する関係 $\kappa ([\pi ']\otimes [\pi '']) = [\pi '\pi '']$ によって特徴付けられる $R_K(G')\otimes_{\mathbf{Z}}R_K(G'')$ から群 $R_K(G'\times G'')$ までの $\mathbf{Z}$ 線形写像 $\kappa$ が存在します。 $\pi ''$) $G'$ の有限次元表現 (それぞれ $G''$) と $\pi '\pi ''$ の外部テンソル積 (VIII、p. 400、例 5)。 環準同型です。 体 K が代数的に閉じている場合、写像 $\kappa$ は同型 (VIII, p. 213, 注意 2) です。

G が 2 つの群の積 $G'\times G''$ であると仮定します。 $\mathscr{Z}_K(G')\otimes_K\mathscr{Z}_K(G'')$ から $\mathscr{Z}_K(G)$ までの $\psi$ 準同型は、$f'\otimes f''$ から写像 $(g', g'')\mapsto f'(g')f''(g'')$ に送信されます。次の図式の通勤:

$R_K(G')\otimes_{\mathbf{Z}}R_K(G'')^{\kappa}$ // $R_K(G)$

$\Theta_{G'}\otimes \Theta_{G''}\Theta_G$

$\mathscr{Z}_K(G')\otimes_K\mathscr{Z}_K(G'')^{\psi}$ /$/\mathscr{Z}_K(G)$。

### 5. フーリエ反転公式

この切断の残りについて、群 G は有限であり、K は代数閉体であり、その特性は G の割る位数ではないため、K の元 $|G|$ は零ではないと仮定します。

代数 K[G] は半単純 (マシュケの定理) であり、有限次元です。 単純な K[G] モジュールの $\widehat{G}$ 集合の類で表します。 G のすべての $\lambda \in \widehat{G}$、選ぶ線型表現 $(V_{\lambda}, \pi_{\lambda})$ について、付随した K[G] モジュールは類 $\lambda$ になります。 集合 $\widehat{G}$ は有限であり、ベクトル空間 $V_{\lambda}$ は有限次元 (VIII、p. 141、例) です。 任意の $\lambda \in \widehat{G}$ について、表現 $\pi_{\lambda}$ の $d_{\lambda}$ 次数、つまり K-ベクトル空間 $V_{\lambda}$ の次元で表し、その指標を $\chi_{\lambda}$ で表します。

$F(\widehat{G})$ 積代数 $\prod_{\lambda \in \widehat{G}} \operatorname{End}_K(V_\lambda)$ と、$\overline{\mathscr{F}}(a) = (\pi_\lambda(a))_{\lambda \in \widehat{G}}$ で定義される $K[G]$ から $F(\widehat{G})$ までの$\overline{\mathscr{F}}$ 写像で表します。 体 $K$ は代数的に閉じているため、*写像 $\overline{\mathscr{F}}$ は代数同型* です (上記参照)。

$\lambda \in \widehat{G}$ ごとに、代数 $\operatorname{End}_K(V_\lambda)$ の次元は $d_\lambda^2$ です。 代数 $K[G]$ のそれは $\operatorname{Card}(G)$ です。したがって、関係となります。

$$
\operatorname{Card}(G) = \sum_{\lambda \in \widehat{G}} d_\lambda^2.
$$

代数 $K[G]$ のトレースを $\tau$ で示します。 定義による、元 $a$ の $K[G]$ のトレース $\tau(a)$ は、$K[G]$ (III, §7, No. 7、p. 515) の自己準同型 $x \mapsto ax$ のトレースです。 $a = \sum_{g \in G} a_g g$ を $K[G]$ の元とします。 公式 (2) により、$g \in G$ ごとに $\tau(ag^{-1}) = |G| a_g$ が得られるため、関係

$$
a = |G|^{-1} \sum_{g \in G} \tau(ag^{-1})\ g.
$$

代数 $F(\widehat{G})$ のトレースを $\widehat{\tau}$ で示します。 $A = (A_\lambda)_{\lambda \in \widehat{G}}$ を $F(\widehat{G})$ の元とします。 (cf. III, §9, No. 3, p. 545, 例 3)

$$
\widehat{\tau}(A) = \sum_{\lambda \in \widehat{G}} d_\lambda \operatorname{Tr}(A_\lambda).
$$

写像 $\overline{\mathscr{F}}$ は $K$-代数同型なので、 $\widehat{\tau} \circ \overline{\mathscr{F}} = \tau$ があり、したがって、

$$
\tau(a) = \widehat{\tau}(\overline{\mathscr{F}}(a)) = \widehat{\tau}\left((\pi_\lambda(a))_{\lambda \in \widehat{G}}\right) = \sum_{\lambda \in \widehat{G}} d_\lambda \operatorname{Tr}(\pi_\lambda(a)) = \sum_{\lambda \in \widehat{G}} d_\lambda \operatorname{Tr}_\lambda(a)
$$

$a \in K[G]$ ごと、つまり

$$
\tau = \sum_{\lambda \in \widehat{G}} d_\lambda \operatorname{Tr}_\lambda.
$$

したがって、$g \in G$ に対して、VIII、p. 399 の (2) により、

$$
\sum_{\lambda \in \widehat{G}} d_\lambda \chi_\lambda(g) = \begin{cases}
|G| & \text{if } g \text{ is the identity element,} \\
0 & \text{otherwise.}
\end{cases}
$$

$a \in K[G]$ の場合、関係 (9) は次の形をとります。

$$
a = |G|^{-1} \sum_{g \in G} \sum_{\lambda \in \widehat{G}} d_\lambda \operatorname{Tr}(\pi_\lambda(a)\pi_\lambda(g^{-1}))\ g;
$$

したがって、$F(\widehat{G})$ の各元 $A = (A_\lambda)_{\lambda \in \widehat{G}}$ について、

$$
\overline{\mathscr{F}}^{-1}(A) = |G|^{-1} \sum_{g \in G} \sum_{\lambda \in \widehat{G}} d_\lambda \operatorname{Tr}(A_\lambda \pi_\lambda(g^{-1}))\ g
$$

(「フーリエ反転公式」)。

$\mu\in \widehat{G}$ については、$j_\mu:$ End$_K(V_\mu)\longrightarrow \prod_{\lambda\in\widehat{G}}$ End$_K(V_{\lambda})$ 写像で$j_\mu(u) = (v_{\lambda})$ のように表します。$\lambda \not=\mu$ と $v_\mu=u$ の場合は $v_{\lambda}= 0$ です。 公式 (14) までに、

(15) $\overline{\mathscr{F}}^{-1}(j_\mu(u)) =|G|^{-1}d_\mu\sum_{g\in G}$ トリ($u\pi_\mu(g^{-1})$)$g$。

代数 $F(\widehat{G}) =\prod_{\lambda\in\widehat{G}}$ End$_K(V_{\lambda})$ の中心はファミリー $(a_{\lambda}1_{V_{\lambda}})_{\lambda\in\widehat{G}}$ で構成されており、$(a_{\lambda})$ は K の元のファミリーです。 代数 K[G] の中心の $\overline{\mathscr{F}}$ による像です。 したがって、中心には関係によって特徴付けられる基底 $(e_{\lambda})_{\lambda\in\widehat{G}}$ があります。

$$
\pi_{\lambda}(e_\mu) =\delta_{\lambda \mu}1_{V_{\lambda}} \tag{16}
$$

$\lambda , \mu\in \widehat{G}$ の場合、$\delta_{\lambda \mu}$ はクロネッカー デルタ写像です。 公式 (15) までに、$\mu\in \widehat{G}$ ごとに、

$$
e_\mu=|G|^{-1}d_\mu\sum_{g\in G}\chi_\mu(g^{-1})g \tag{17}
$$

これら元満たす関係

(18) $\sum_{\lambda\in\widehat{G}}e_{\lambda}= 1,e^2_\mu=e_\mu$ と $e_\mu e_{\nu}= 0$

$\mu\not=\nu$ などのすべての $\mu, \nu \in \widehat{G}$ に対して。それらは Z(K[G]) の分解不可能な冪等です (VIII, p. 147, 命題 15)

#### 注意 {#alg-viii-s21-n5-rem-1 .statement tag=00NR}

$(V, \pi )$ を G の線型表現とします。Maschke の定理により、K[G] モジュール V は半単純です。任意の $\lambda \in \widehat{G}$ について、K[G] モジュール V の型 $\lambda$ の同型成分を $V^{\lambda}$ で示します。 $V =\bigoplus_{\lambda\in\widehat{G}}V^{\lambda}$ があります。 VIII、p. 147、公式の命題 15 により、V の射影子と、この V の分解に関連付けられた像 $V^{\lambda}$ は次と等しくなります。

$$
\pi (e_{\lambda}) =|G|^{-1}d_{\lambda}\sum_{g\in G}\chi_{\lambda}(g^{-1})\pi (g) \tag{19}
$$

適用この公式を $\pi =\pi_{\lambda}$ にすると、K の元 $d_{\lambda}\cdot 1$ が零ではないことがわかります。さらに (VIII、p. 420、系 2) で、G の $d_\mu$ 割る基数がわかります。

$\lambda$ を $\widehat{G}$ の元とします。 写像 $\pi_{\lambda}$ K[G] から End$_K(V_{\lambda})$ 誘導する同型の $(K[G]$、K[G])-bimodules $e_{\lambda}K[G]$ から End$_K(V_{\lambda})$。 VIII、p. 147 の命題 15 により、K[G] サブモジュール $e_{\lambda}K[G]$ は、型 $\lambda$ の K[G] の同型成分になります。また、G の右側正則表現 (VIII、p. 143、命題 11) の型 $\lambda^{\vee}$ の同型成分および型の同型成分でもあります。 $\lambda \times \lambda^{\vee}$ は複正規表現 (VIII、p. 381、命題 4) です。

### 6. シュールの直交関係

前回の小節の記法を保持します。 $\lambda$ を $\widehat{G}$ の元とし、$u$ と $v$ を End$_K(V_{\lambda})$ の元とします。 公式 (10) までに、

$\widehat{\tau}(j_{\lambda}(u)j_{\lambda}(v)) =d_{\lambda}$ トリ($uv$)。 $\tau =\widehat{\tau}\circ \mathscr{F}$ なので、公式 (2) と (15) から関係を導き出します。

$d^2_{\lambda}|G|^{-1}\sum_{g\in G}$ Tr($u\pi_{\lambda}(g)$) Tr($v\pi_{\lambda}(g^{-1})$) $=d_{\lambda}$ Tr($uv$)。

以前、体 K で $d_{\lambda}.1\not= 0$ が観測されました。 (20) $|G|^{-1}\sum_{g\in G}$ Tr($u\pi_{\lambda}(g)$) Tr($v\pi_{\lambda}(g^{-1})$) $=d^{-1}_{\lambda}$ Tr($uv$) となります。

この関係を、$u$ と $v$ が階数 $\leqslant 1$ を持つ場合に適用してみましょう。 (21) $|G|^{-1}\sum_{g\in G}\langle x^*, \pi_{\lambda}(g)x\rangle  \langle y^*, \pi_{\lambda}(g^{-1})y\rangle =d^{-1}_{\lambda}\langle x^*, y\rangle \langle y^*, x\rangle$ を取得します

$V_{\lambda}$の$x,y$と$V_{\lambda}$のデュアル$V^*_{\lambda}$の$x^*, y^*$。

$\lambda \in \widehat{G}$ ごとに、$(e_{\lambda ,j})_{1\leqslant j\leqslant d_{\lambda}}$ を $V_{\lambda}$ の基底とします。この基底に対して、自己準同型の$\pi_{\lambda}(g)$、$V_{\lambda}$の$(\pi^{\lambda}_{ij}(g))$行列で表します。 $V^*_{\lambda}$ と $(e_{\lambda ,j})$ の双対である $(e^*_{\lambda ,i})_{1\leqslant i\leqslant d_{\lambda}}$ 基底で表すと、$\pi^{\lambda}_{ij}(g) =\langle e^*_{\lambda ,i}, \pi_{\lambda}(g)e_{\lambda ,j}\rangle$ となり、したがって (22) $|G|^{-1}\sum_{g\in G}\pi_{ij}^{\lambda}(g)\pi^{\lambda}_{k\ell}(g^{-1}) =d^{-1}_{\lambda}\delta_{i\ell}\delta_{jk}$ となります。

ここで、$\lambda$ と $\mu$ を $\widehat{G}$ の 2 つの異なる元とし、$u\in$ End$_K(V_{\lambda})$ と $v\in$ End$_K(V_\mu)$ とします。再び関係 (15) により、(23) $\sum_{g\in G}$ Tr($u\pi_{\lambda}(g)$) Tr($v\pi_\mu(g^{-1})$) $= 0$ となります。

上記のように、(24) $\sum_{g\in G}\langle x^*, \pi_{\lambda}(g)x\rangle  \langle y^*, \pi_\mu(g^{-1})y\rangle = 0$ と推定されます。

$x\in V_{\lambda},x^*\in V^*_{\lambda},y\in V_\mu$、および$y^*\in V^*_\mu$の場合。 $[1, d_{\lambda}]$の$i, j$と$[1, d_\mu]$の$k, \ell$には、(25)$\sum_{g\in G}\pi^{\lambda}_{ij}(g)\pi^\mu_{k\ell}(g^{-1}) = 0$もあります。

関係 (20) から (25) は、シュールの直交関係として知られています。

#### 注意 {#alg-viii-s21-n6-rem-1 .statement tag=00NS}

同一視する代数 $V_{\lambda}$ の基底 $(e_{\lambda ,j})$ を経て、 行列環 $\mathbf{M}_{d_{\lambda}}(K)$ で$_K(V_{\lambda})$ が終わります。 写像 $\mathscr{F}^{-1}$ は、代数 $\prod_{\lambda}\mathbf{M}_{d_{\lambda}}(K)$ から代数 K[G] までの同型です。 $\mu\in \widehat{G}$ の場合、インデックス $\mu$ の成分が $\mathbf{M}_{d_\mu}(K)$ (II, §10, No. 3, p. 341) の行列単位 $E_{ij}$ であり、他の成分がゼロである $\prod_{\lambda}\mathbf{M}_{d_{\lambda}}(K)$ の要素を $E^\mu_{ij}$ で表します。 $u^\mu_{ij}=\mathscr{F}^{-1}(E^\mu_{ij})$を設定します。 $\lambda \in \widehat{G}, 1\leqslant i\leqslant d_{\lambda}$、$1\leqslant j\leqslant d_{\lambda}$ の元 $u^{\lambda}_{ij}$ の族は、代数 K[G] の基底です。 乗法表は

$$
u^{\lambda}_{ij}u^\mu_{k\ell}=\delta_{\lambda \mu}\delta_{jk}u^{\lambda}_{i\ell} \tag{26}
$$

さらに、公式 (15) までに、

$$
u^{\lambda}_{ij}=|G|^{-1}d_{\lambda g}\sum_{\in G}\pi^{\lambda}_{ji}(g^{-1})g \tag{27}
$$

### 7. 指標の直交関係

小節 5 と 6 の記法を保持します。Z(K[G]) が中央の写像で構成されていることを思い出してください。

定義する $K[G]\times K[G]$ から K までの対称双線形写像を公式で計算します。

$$
\langle f, f'\rangle_G=|G|^{-1}\sum_{g\in G}f_gf'_{g^{-1}} \tag{28}
$$

$f=\sum f_gg$ と $f'=\sum f_g'g$ 所属ごとに K[G] に。 $\langle f, f'\rangle_G=$ $|G|^{-2}\tau (f f')$ があります。

#### 命題 4 (直交関係は指標) {#alg-viii-s21-prop-4 .statement tag=00SG}

$\widehat{G}$ の $\lambda$ と $\mu$ には、$\langle \chi_{\lambda}, \chi_\mu\rangle_G=\delta_{\lambda \mu}$ があります。

これは、自己準同型 $u$ と $v$ が恒等であるとみなされる場合の、関係 (20) と (23) の具体的なケースです。

#### 系 {#alg-viii-s21-n7-cor-1 .statement tag=00NT}

$\pi$ と $\pi '$ を G の有限次元線型表現とします。 体 K では、次のようになります。

(29) $\langle \chi_{\pi}, \chi_{\pi'}\rangle_G=$ (薄暗い$_K$ ホム$_G(\pi , \pi ')$)$\cdot 1$。

まず、$\pi$ と $\pi '$ が単純な表現であると仮定します。 ベクトル空間 Hom$_G(\pi , \pi ')$ は、$\pi$ と $\pi '$ が同型であるかどうかに応じて、次元 1 または 0 になります (シュールの補題、VIII、p. 47、命題 2)。この場合、命題 4 から公式 (29) が続きます。

一般的な場合、表現 $\pi$ (それぞれ $\pi '$) は、単純な表現 $\pi_1, . . . , \pi_m$ (それぞれ $\pi '_1, . . . , \pi '_n$) の直和です。 空間 Hom$_G(\pi , \pi ')$ は、$1\leqslant i\leqslant m$、$1\leqslant j\leqslant n$ について、空間 Hom$_G(\pi_i, \pi '_j)$ の直和と同型です。

$$
\chi_{\pi}=\chi_{\pi_1}+\cdots +\chi_{\pi_m},\chi_{\pi'}=\chi_{\pi'_1}+\cdots +\chi_{\pi'_n}
$$

線形性により、公式 (29) の証明は単純な表現の場合に還元されます。

### 8. 中心部写像オン有限群

#### 命題 5 {#alg-viii-s21-prop-5 .statement tag=00NU}

ファミリ $(\chi_{\lambda})_{\lambda\in\widehat{G}}$ は、中央写像のベクトル空間の基底です。 G の単純な線型表現の類の数は、G の共役類の数に等しい。

$a=\sum_{g\in G}a_gg\in K[G]$ には、$a^{\vee}=\sum_{g\in G}a_{g^{-1}}g$ と書き込みます。 写像 $a\mapsto a^{\vee}$ は、代数 K[G] の包含反自己同型です。 公式 (17) までに、$\lambda \in \widehat{G}$ ごとに $e_{\lambda}=|G|^{-1}d_{\lambda}\chi^{\vee}_{\lambda}$ が得られます。 命題は、家族 $(e_{\lambda})_{\lambda\in\widehat{G}}$ が K[G] の中心の基底であるという事実から続きます。

G の共役類の $\mathscr{C}$ 集合で表します。C を $\mathscr{C}$ の元とします。 写像 $g\mapsto g^{-1}$ による C の像 $C^{-1}$ は共役類です。 Cの元の交換子環は相互にGの共役部分群です。彼らの基数 $d(C)$ は満足します

(30) カード(G) = カード(C) $d(C)$。

特に、体 K には $d(C)\cdot 1\not= 0$ があります。

$f$ を G の中心写像とします。任意の共役類 C について、$x\in C$ の $f(x)$ の $f(C)$ 共通の値で表します。これにより、指標 (VIII, p. 410, 命題 4) に対する記法, 直交関係は次のように書くことができます。

$$
\sum_{C\in\mathscr{C}}\chi_{\lambda}(C^{-1})\chi_\mu(C)d(C)^{-1}=\delta_{\lambda \mu} \tag{31}
$$

$\widehat{G}$の$\lambda$と$\mu$用。

$\chi_{\lambda}(C)$ のエントリを持つ型 $\widehat{G}\times \mathscr{C}$ の A 行列と、$\chi_{\lambda}(C^{-1})d(C)^{-1}$ のエントリを持つ型 $\mathscr{C}\times \widehat{G}$ の B 行列によって表されます。 集合 $\widehat{G}$ と $\mathscr{C}$ は同じ基数 (命題 5) を持ちます。 関係 (31) は、行列積 AB が型 $\widehat{G}\times \widehat{G}$ の行列単位であることを表します。 II, §10, No. 12、p. 360、行列積のうち命題 11 までに、BA は型 $\mathscr{C}\times \mathscr{C}$ の行列単位です。他の語には関係があります

$$
\sum_{\lambda\in\widehat{G}}\chi_{\lambda}(C^{-1})\chi_{\lambda}(C') =d(C)\delta_{CC'} \tag{32}
$$

$\mathscr{C}$のCと$C'$用（ときどきは「指標の2番目の直交関係」と呼ばれます）。

HをGの部分群とします。整数カード(H)割るカード(G)であり、$|G|$がKの零ではないことに注意してください。したがって、K には $|H| \not= 0$ が入ります。

Z(K[G]) から Z(K[H]) までの Res$^G_H$ 線形写像で表され、G の中心写像をその制限に H に送信します。 $\chi_{\pi}$ が G の有限次元表現 $\pi$ の指標である場合、Res$^G_H(\chi_{\pi})$ は次のようになります。 H の指標表現解像度$^G_H(\pi )$

#### 命題 6 {#alg-viii-s21-prop-6 .statement tag=00NV}

$f$ を G の中心写像とし、$u$ を H の中心写像とします。

(33) $\langle$Ind$^G_H(u), f\rangle_G=\langle u$、Res$^G_H(f)\rangle_H$。

単純な G の指標表現 Z(K[G]) の形基底 (VIII, p. 411, 命題 5)、そして同じことが H にも当てはまります。 したがって、$f$ が G の単純な表現 $\pi$ の指標 $\chi_{\pi}$ であり、$u$ が H の単純な表現 $\sigma$ の指標 $\chi_{\sigma}$ である場合、(33) を確立するだけで十分です。 この場合、Ind$^G_H(u)$ は G の表現 Ind$^G_H(\sigma )$ の指標であり、VIII、p. 410、系により、次のようになります。

$\langle$Ind$^G_H(u), f\rangle_G=$ (dim$_K$ Hom$_G$(Ind$^G_H(\sigma ), \pi$ ))$\cdot 1$。

関係を表示します

$\langle u$、レス$^G_H(f)\rangle_H=$ (ディム$_K$ ホム$_H(\sigma$、レス$^G_H(\pi )$))$\cdot 1$

同様に、等式 (33) の後にフロベニウスの相互法則が続きます。

#### 命題 7 {#alg-viii-s21-prop-7 .statement tag=00NW}

$f$ を G から K までの写像とします。次の主張は同等です。

(i) $f=a\chi_{\lambda}$ となるような K の $\widehat{G}$ の元 $\lambda$ と元 $a$ があります。

(ii) G の元のすべての対 $(g, g')$ について、次のようになります。

$$
f(g)f(g') =|G|^{-1}f(1)\sum_{h\in G}f(hgh^{-1}g') \tag{34}
$$

$\lambda$ を $\widehat{G}$ の元とします。 $V_{\lambda}$、集合の自己準同型 $u$ ごとに

$$
u^{\natural}=|G|^{-1}\sum_{h\in G}\pi_{\lambda}(h)u \pi_{\lambda}(h^{-1}) \tag{35}
$$

$V_{\lambda}$ の自己準同型 $u^{\natural}$ は K[G]-線形です。シュールの補題 (VIII, p. 47, 定理 1)$,u^{\natural}$ はホモテティー です。 $u$ と $u^{\natural}$ は同じトレースを持っているため、次のようになります。

$u^{\natural}=d^{-1}_{\lambda}$ トリ($u$) $1_{V_{\lambda}}$。

$u$ と $v$ を $V_{\lambda}$ の自己準同型とします。それは次のとおりです

(36) Tr($u$) Tr($v$) $=d_{\lambda}$ Tr($u^{\natural}v$) $=d_{\lambda}|G|^{-1}\sum_{h\in G}$ Tr($\pi_{\lambda}(h)u \pi_{\lambda}(h^{-1})v$)。

公式 (36) で $u=\pi_{\lambda}(g)$ と $v=\pi_{\lambda}(g')$ を取得します。 $f=\chi_{\lambda}$ の関係 (34) が続きます。

逆に、主張 (ii) が成り立つとします。 $f(1) = 0$ がある場合、G の元の対 $(g, g')$ ごとに $f(g)f(g') = 0$ となり、従って $f= 0$ になります。従って、$f(1)\not= 0$ と仮定できます。 (34) に $g'= 1$ を入れると、関係が得られます。

$$
f(g) =|G|^{-1}\sum_{h\in G}f(hgh^{-1})
$$

すべての $g\in G$ について、これは $f$ が中心の写像であることを意味します。 命題 5 までに、$f=\sum_{\lambda\in\widehat{G}}a_{\lambda}\chi_{\lambda}$ となるような K の元の家族 $(a_{\lambda})$ が存在します。 公式 (34) のこの式を使って置き換える $f$ を考えてみましょう。 指標 $\chi_{\lambda}$ のそれぞれがこの関係も満たしていることを考慮すると、次のようになります。

$$
\sum_{\lambda ,\mu\in\widehat{G}}a_{\lambda}a_\mu\chi_{\lambda}(g)\chi_\mu(g') =\sum_{\lambda\in\widehat{G}}a_{\lambda}d^{-1}_{\lambda}f(1)\chi_{\lambda}(g)\chi_{\lambda}(g') \tag{37}
$$

$g, g'\in G$の場合。この関係は次のように書くこともできます。

$$
\sum_{\lambda ,\mu}(a_{\lambda}a_\mu-\delta_{\lambda \mu}a_{\lambda}d^{-1}_{\lambda}f(1))\chi_{\lambda}(g)\chi_\mu(g') = 0 \tag{38}
$$

$g, g'\in G$の場合。さて、$\lambda \in \widehat{G}$ の写像 $\chi_{\lambda}$ は線形独立です (VIII、p. 411 の命題 5)。それは次のとおりです

$$
a_{\lambda}a_\mu=\delta_{\lambda \mu}a_{\lambda}d^{-1}_{\lambda}f(1)
$$

$\lambda , \mu\in \widehat{G}$の場合。 特に、$\lambda \not=\mu$ の場合は常に $a_{\lambda}a_\mu= 0$ です。 従って、$a_{\lambda}\not= 0$ となる$\widehat{G}$ の要素 $\lambda$ は最大 1 つ存在し、$f=a_{\lambda}\chi_{\lambda}$ が存在するため、(i) になります。

### 9. アーベル群の場合

この小節では、群 G がアーベルであると仮定します。

シュールの補題 (VIII、p. 48、系 1) によれば、G のすべての単純な表現には次元 1 が含まれます。 $(M, \pi )$ をその表現とし、$\chi$ をその指標とします。 $g\in G$ と $x\in M$ ごとに、$\pi (g)(x) =\chi (g)x$ があります。 従って、指標 $\chi$ は、G から K の乗法群 $K^*$ までの準同型です。 逆に、G から $K^*$ までのすべての準同型は、次数 1 の G の表現の指標です。 従って、単純な K[G] 加群のクラスの集合 $\widehat{G}$ は、G から $K^*$ までの準同型写像の集合 Hom(G$,K^*$) と識別できます。 このことから、$\widehat{G}$ でアーベル群構造を推測します。 $\widehat{G}$ 対応するから表現のテンソル積までの積。 群 G と $\widehat{G}$ は、VIII、p. 411 の命題 5 によって同じ基数を持ちます。 G 上のすべての写像が中心であり、$\widehat{G}$ は G から K までの写像のベクトル空間の基底です (上記参照)。 指標に対する直交関係のため、そのような写像 $f$ は、基底 $\widehat{G}:$ に関して次の一意の分解を持ちます。

$$
f=\sum_{\chi\in\widehat{G}}\langle \chi , f\rangle_G\chi \tag{39}
$$

G から K までの写像 $f$ と $f'$ の場合、関係になります。

$$
\langle f, f'\rangle_G=\sum_{\chi\in\widehat{G}}\langle \chi , f\rangle_G\langle \chi , f'\rangle_G \tag{40}
$$

$(V, \pi )$ を G の線型表現とします。 任意の $\chi \in \widehat{G}$ について、$g\in G$ ごとに $\pi (g)(v) =\chi (g)v$ となるようなベクトル $v$ から構成される V の部分空間を $V^{\chi}$ で表します。 空間 $V^{\chi}$ は、K[G] モジュール V の型 $\chi$ の同型成分です。 空間 V は家族 $(V^{\chi})_{\chi\in\widehat{G}}$ の直和であり、この分解に関連付けられた像 $V^{\chi}$ を持つ V の射影子 $p_{\chi}$ は次のように与えられます。

$$
p_{\chi}=|G|^{-1}\sum_{g\in G}\chi (g^{-1})\pi (g) \tag{41}
$$

関係 (19) のため。

#### 注意 {#alg-viii-s21-n9-rem-1 .statement tag=00NX}

$n$ を群 G の基数とし、$\mu_n(K)$ を K の単位元の $n$ 番目の根の群とします。$g\in G$ ごとに、$g^n= 1$ が得られます。従って、$\widehat{G}$ は群 Hom(G$, \mu_n(K)$) と識別できます。 群 $\mu_n(K)$ は、位数 $n$ (V, §11, No. 2、p. 78、定理 1) の循環です。従って、群 $\widehat{G}$ は群 D(G) = Hom(G$,\mathbf{Q}/\mathbf{Z}$) と同型です。 VII, §4, No. 9、p. 26、命題 10、群 $\widehat{G}$ は群 G と同型で、写像は G の元 $g$ を準同型に送信します。 $\widehat{G}$から$K^*$までの$\chi \mapsto \chi (g)$は、Gから$\widehat{\widehat{G}}$までの同型です。

### 10. 指標とグロタンディーク群

$K\otimes_{\mathbf{Z}}R_K(G)$ から $\mathscr{Z}_K(G)$ までの $\theta_G$ K-代数準同型は、有限次元表現 $\pi$ ごとに $1\otimes [\pi ]$ から $\chi_{\pi}$ を送信します。

#### 命題 8 {#alg-viii-s21-prop-8 .statement tag=00NY}

a) 準同型 $\theta_G$ は、$K\otimes_{\mathbf{Z}}R_K(G)$ から $\mathscr{Z}_K(G)$ までの同型です。

b) K が特性 0 を持つとします。すると、$R_K(G)$ から $\mathscr{Z}_K(G)$ の部分環線形結合の指標 $\chi_{\lambda}$ の $\lambda$ のからなるが$\theta_G$ 定義する同型となります。 $\widehat{G}$ と整数係数。

ファミリ $([\lambda ])_{\lambda\in\widehat{G}}$ は、$\mathbf{Z}$ モジュール $R_K$(G) の基底であり、ファミリ $(\chi_{\lambda})_{\lambda\in\widehat{G}}$ は、K-ベクトル空間 $\mathscr{Z}_K(G)$ の基底です。 主張 a) と b) は (VIII、p. 411、命題 5) に続きます。

### 11. シンプル表現の次元

群 G の基数を $n$ で表します。 $\pi$ を有限次元 K-ベクトル空間 M の G の線型表現とします。すべての $g\in G$ に対して、$\pi (g)^n= 1_M$ が得られるため、最小多項式は $\pi (g)$ 割る $T^n-1$ となります。 K の $n\cdot 1\not= 0$ であるため、この最小多項式は分離可能 (V, §11, No. 2, p. 78) であり、体 K は代数的に閉じているため、M の自己準同型 $\pi (g)$ は対角化可能です (VII, §5, No. 7, p. 40, 命題) 12)。 $\pi (g)$の固有値は単位元の$n$番目の根であり、$\alpha \in K$ごとに、$\alpha$の幾何学的重複度は$\pi (g)$の固有値 (VII, §5, No. 2, p. 30, 定義 1) $\pi (g)$ の特性多項式の根として、$\alpha$ の重複度に等しい。 単位元の $n$ 番目の根の集合 $\mu_n(K)$ によって生成された K の $\mathscr{O}_n$ 部分群で表します。それは有限生成された $\mathbf{Z}$ モジュールであり、K の部分環です。 $\pi$ の指標は、$\mathscr{O}_n$ でその値を受け取ります。

#### 命題 9 {#alg-viii-s21-prop-9 .statement tag=00NZ}

体 K が標数0 を持っているとします。次に、すべての単純な次数表現 G 割る基数の G。

$(V, \pi )$ を G の単純な表現とし、$\chi$ をその指標とします。 Z(K[G]) の元 $a$ ごとに、V の自己準同型 $\pi (a)$ はホモテティー (VIII, p. 47, 定理 1) です。 $\varphi (a)$ は、$\pi (a) =\varphi (a)_V$ のようなスカラーを表します。 結果として得られる写像 $\varphi$ Z(K[G]) から K までは代数準同型です。 $a=\sum_{g\in G}\chi (g^{-1})g$ を考えてみましょう。 VIII、p. 408 の注意により、$\varphi (a) =$ (薄暗い $V$)$^{-1}|G|$ が得られます。 一方、K[G] の $a$ 属するから部分環 $\mathscr{O}_n[G]\cap Z(K[G])$ は、有限生成された $\mathbf{Z}$ 加群 (VII, §3、p. 15、系) です。 つまり、K の属するから K の部分環までの元 $\varphi (a) =$ (dim $V$)$^{-1}|G|$ は、有限生成された $\mathbf{Z}$ 加群です。 私たちはを用いて結論する次の補題を行います。

#### 補題 {#alg-viii-s21-n11-lem-1 .statement tag=00O0}

L を $\mathbf{Q}$ の拡大とします。 A を L の部分環とします。 A が有限生成された $\mathbf{Z}$ モジュールであると仮定します。 $A\cap \mathbf{Q}=\mathbf{Z}$ があります。

$\mathbf{Z}$加群$A\cap \mathbf{Q}$は有限生成されるため、$A\cap \mathbf{Q}$が$\frac{1}{N}\mathbf{Z}$に含まれるような正の整数Nが厳密に存在します。 $x$ を $\mathbf{Q}-\mathbf{Z}$ の元とします。 $x=\frac{p}{q}$と書きます。ここで、$p$と$q$は互いに素である整数と$q\geqslant 2$です。 $q^N\geqslant 2^N>N ($集合理論、III, §3, No. 6、p. 165、定理 2)、整数 $p^N$ と $q^N$ は相互に素であり、結果として $x^N\notin\frac{1}{N}\mathbf{Z}$ です。従って、$x$ は A に対して属するではありません。これは、補題の結論する証明です。

次の小節では、K の特性が G の割る位数に当てはまらないとだけ仮定した場合を拡大する命題 9 とします。

### 12. 基礎体中変更

以前の小節の記法を保持します。 $K'$ を、$K'$ の要素 $n\cdot 1$ がゼロではないような代数的に閉じた体とする。 群 $\mu_n(K)$ と $\mu_n(K')$ は、位数 $n$ (V, §11, No. 2、p. 78、定理 1) の循環です。 選ぶ同型 $\varphi$ $\mu_n(K)$ から $\mu_n(K')$ まで。 $\pi$ を有限次元 K-ベクトル空間における G の線型表現とし、$\pi '$ を有限次元 $K'$ ベクトル空間における G の線型表現とする。 すべての $g\in G$ と $\omega \in \mu_n$(K) について、 $\pi (g)$ の固有値が次のように $\omega$ の重複度が $\varphi (\omega )$ の重複度に等しい場合、 $\pi$ と $\pi '$ は ( $\varphi$ を通じて) 関連していると言います。 $\pi '(g)$中固有値。 この場合、$g= 1$ を取るとわかるように、$\pi$ と $\pi '$ は同じ次元を持ちます。

$\pi_1$ と $\pi_2$ (それぞれ $\pi '_1$ と $\pi '_2$) を K (それぞれ $K'$) 上の有限次元ベクトル空間における G の線型表現とします。次のようなプロパティがあります。

a) $\pi_1$ が $\pi '_1$ と $\pi '_2$ に関連している場合、$\pi '_1$ と $\pi '_2$ は同型です。

b) $\pi_1$ が $\pi '_1$ に、$\pi_2$ が $\pi '_2$ に関連付けられている場合、$\pi_1\oplus \pi_2$ は $\pi '_1\oplus \pi '_2$ に関連付けられ、$\pi_1\otimes \pi_2$ は $\pi '_1\otimes \pi '_2$ に関連付けられます。

主張 a) は、VIII、p. 402、主張の系 5 から続き、b) は明らかです。

ここで、以前は $\widehat{G}$ で示されていた単純な K[G] モジュールの類の $\mathscr{S}_K(G)$ 集合で示され、同様に定義する $\mathscr{S}_{K'}(G)$ となります。 集合 $\mathscr{S}_K(G)$ と $\mathscr{S}_{K'}(G)$ は両方とも有限で、共役類の基数数 (VIII、p. 411、命題 5) です。

#### 命題 10 {#alg-viii-s21-prop-10 .statement tag=00O1}

$\mathscr{S}_K(G)$ から $\mathscr{S}_{K'}(G)$ までの一意な写像 $\varphi_G$ が存在し、$\mathscr{S}_K(G)$ のすべての $\lambda$ に対して、$\lambda$ と $\varphi_G(\lambda )$ が $\varphi$ を介して関連付けられます。また、$\varphi_G$は全単射です。

$\varphi_G$ の一意性は、上記の性質 a) から続きます。

A) 体 K が特性 0 を持つとします。

群 $\mu_n(K)$ は循環です (V, §11, No. 2、p. 78、定理 1)。この群の選ぶ生成元$\zeta$。 X を $\zeta$ に送信する環準同型 $\rho :\mathbf{Z}[X]\rightarrow \mathscr{O}_n$ を考えてみましょう。それは客観的です。円分多項式 $\Phi_n(X)$ は $\mathbf{Q}[X]$ (V, §11, No. 5, p. 84, 定理 2) では既約です。従って、それは $\mathbf{Q}$ に対する $\zeta$ の最小多項式になります。多項式 $\Phi_n$ は、整数係数 (V, §11, No. 4, p. 81) とモニックです。 $P\in \mathbf{Z}[X]$ を $P(\zeta ) = 0$ のような多項式とします。多項式 (IV, §1, No. 6, p. 10) のユークリッド除算により、$\mathbf{Z}[X]$ には P = QΦ$_n+ R$ および deg(R) $<$ deg(Φ$_n$) となる 2 つの多項式 Q と R が存在します。 $R(\zeta ) = 0$ があり、$\Phi_n$ が $\zeta$ の最小多項式であるため、R = 0 となります。従って、$\rho$の核は$\mathbf{Z}[X]$の$\Phi_n\mathbf{Z}[X]$、$\mathbf{Z}[X]/\Phi_n\mathbf{Z}[X]$から$\mathscr{O}_n$までは$\rho$誘導する環同型となります。

集合 $\zeta '=\varphi (\zeta )$;これは、$K'$ の単位元の原始 $n$ 番目の根であるため、$\Phi_n(\zeta ') = 0$ (V, §11, No. 5, p. 83, 補題 3) になります。従って、環 $\mathscr{O}_n$ から体 $K'$ までの変換 $\zeta$ から $\zeta '$ までの準同型 $\varphi_0$ が存在します。それは $\mu_n(K)$ から $\mu_n(K')$ まで拡大する写像 $\varphi$ です。 $\mathscr{O}$を$a\in \mathscr{O}_n$と$r\in \mathbf{N}$で元$\frac{a}{n^r}$のKからなるの部分環とします。 $n\cdot 1$は$K'$で可逆なので、準同型 $\varphi_0$ 拡大するから準同型 $\varphi_1$ $\mathscr{O}$ から $K'$ になります。

群の同一視する代数$\mathscr{O}[G]$は、代数K[G]の部分環と定義する環準同型Φで$\mathscr{O}[G]$から$K'[G]$まで$\mathscr{O}$を越えます。 公式

$$
\Phi (\sum_{g\in G}a_gg)=\sum_{g\in G}\varphi_1(a_g)g \tag{42}
$$

G の共役類の $\mathscr{C}$ 集合で表します。$\mathscr{C}$ の C については、$\mathscr{O}[G]$ の $u_C$ 元 $\sum_{g\in C}g$ で表します。家族$(u_C)_{C\in\mathscr{C}}$は、中心の$\mathscr{O}$、代数の$Z(\mathscr{O}[G])$、$\mathscr{O}[G]$（VIII、p. 398）を超える基底です。 $\mathscr{S}_K$(G) の任意の元 $\lambda$ について、$\chi_{\lambda}$ はその指標、$d_{\lambda}$ はその次元、そして以下で定義される K[G] の $e_{\lambda}$ 元を表します。

$$
e_{\lambda}=|G|^{-1}d_{\lambda}\sum_{g\in G}\chi_{\lambda}(g^{-1})g \tag{43}
$$

ファミリ $(e_{\lambda})$ は、環 K[G] (VIII, p. 408) の中心 Z(K[G]) の K 上の基底です。我々は持っています

$$
e_{\lambda}=\sum_{C\in\mathscr{C}}\alpha_{\lambda ,C}u_C \tag{44}
$$

と

$$
\alpha_{\lambda ,C}=|G|^{-1}d_{\lambda}\chi_{\lambda}(C^{-1}) \tag{45}
$$

$C\in \mathscr{C}$と$\lambda \in \mathscr{S}_K$(G)の場合は、集合 $\beta_{C,\lambda}=|G|d^{-1}_{\lambda}d(C)^{-1}\chi_{\lambda}(C)$。 行列 $(\alpha_{\lambda ,C})$ のエントリは $\mathscr{O}$ にあり、VIII、p. 411 の公式 (31) から、その逆数行列は行列 $(\beta_{C,\lambda})$ となり、そのエントリも $\mathscr{O}$ にあります。 命題 VIII の 9、p. 415。従って、ファミリー $(e_{\lambda})$ は、$\mathscr{O}$ モジュール $Z(\mathscr{O}[G])$ の基底になります。

$K'[G]$ 形基底の元 $\Phi (u_C) =\sum_{g\in C}g$ が中心の $K'$ 環 $K'[G]$ の $Z(K'[G])$ を超えています。我々は持っています

$$
\Phi (e_{\lambda}) =\sum_{C\in\mathscr{C}}\varphi_1(\alpha_{\lambda ,C}) \Phi (u_C) \tag{46}
$$

$\varphi_1(\alpha_{\lambda ,C})$ のエントリを持つ行列は反転可能です。したがって、$\Phi (e_{\lambda})$ のファミリーは $Z(K'[G])$ の基底になります。ファミリ $(e_{\lambda})$ は、Z(K[G]) のべき等 1 (VIII、p. 146、および p. 408) の分割です。他の語では、

$\lambda \not=\mu$なら$\sum_{\lambda}e_{\lambda}= 1,e^2_{\lambda}=e_{\lambda},e_{\lambda}e_\mu= 0$。

したがって、$\Phi (e_{\lambda})$ の族は $Z(K'[G])$ の冪等 1 の分割になります。この族は $K'$ 上の $Z(K'[G])$ の基底であるため、その元は $Z(K'[G])$ (VIII, p. 148, 注意 4) の分解不可能な冪等です。

$\mathscr{S}_{K'}$(G)、定義する、$\chi_{\lambda'},d_{\lambda'}$、$e_{\lambda'}$の$\lambda '$については上記と同様。 VIII、p. 408、元 $e_{\lambda'}$ は、$Z(K'[G])$ の分解不可能な冪等です。したがって、$\mathscr{S}_K(G)$ から $\mathscr{S}_{K'}(G)$ までは全単射 $\varphi_G$ が存在し、$\mathscr{S}_K(G)$ のすべての $\lambda$ に対して $\Phi (e_{\lambda}) =e_{\varphi_G(\lambda)}$ が存在します。

$\lambda$ を $\mathscr{S}_K(G)$ にしましょう。 集合 $\lambda '=\varphi_G(\lambda )$。 $(V_{\lambda}, \pi_{\lambda})$ (それぞれ $(V_{\lambda'}, \pi_{\lambda'})$) を、付随した K[G] モジュール (それぞれ $K'$[G] モジュール) が類 $\lambda$ (それぞれ $\lambda '$) を持つ G の線型表現とします。 $\lambda$ と $\lambda '$ が関連していることを証明しましょう。 $g$ を G の元とします。 $\delta (T)$ を K[T] モジュール $K[T]\otimes_KV_{\lambda}$ の自己準同型 $1 + T\pi_{\lambda}(g)$ の行列式とします。 $\omega_1, . . . , \omega_{d_{\lambda}}$ を $\pi_{\lambda}(g)$ の固有値とします。私たちは持っています

$$
\delta (T) = (1 + T\omega_1)\cdots (1 + T\omega_{d_{\lambda}})
$$

同様に定義する $\delta '(T)$とし、$\pi_{\lambda'}(g)$の固有値を$\omega '_1, . . . , \omega '_{d_{\lambda'}}$で表します。 $\mathscr{O}$ モジュール $\mathscr{O}[G]$ には基底 G があり、K-ベクトル空間 K[G] には基底 G があります。 $\mathscr{O}$[T]-モジュール $\mathscr{O}[T]\otimes_{\mathscr{O}}\mathscr{O}[G]$ の乗法の $1 +e_{\lambda}gT$ を Δ(T) 行列式で表します。 これは、K[T] モジュール $K[T]\otimes_KK[G]$ の $1 +e_{\lambda}gT$ による乗法の行列式でもあります。 $\overline{\varphi}_1$ を $\mathscr{O}[T]$ から $K'[T]$ までの準同型 、拡大する $\varphi_1$ とし、T を T に送信します。 G は、$K'$ ベクトル空間 $K'[G]$ の基底であるため、多項式 $\overline{\varphi}_1(\Delta (T))$ は、$K'$ ベクトル空間 $K'[G]$ の乗法の $1 +e_{\lambda'}gT$ の行列式 $\Delta '(T)$ に等しくなります。

代数 K[G] は、$\mathscr{S}_K(G)$ を通る $\mu$ の単純成分 $e_\mu K[G]$ の直和です。 $\mu$は$\lambda$と異なり、元$e_{\lambda}g$は$e_\mu K[G]$を全滅させます。 さらに、$e_{\lambda}g$の乗算は、$e_{\lambda}K[G]$の$g$の乗算と一致します。 VIII、p. 409、例を考慮すると、$e_{\lambda}K[G]$ の G の 6VIII、p. 400、表現は、$d_{\lambda}$ 表現の類 $\lambda$ の直和です。 従って、$\Delta (T) =\delta (T)^{d_{\lambda}}$ になります。

同様に、$\Delta '(T) =\delta '(T)^{d_{\lambda'}}$ もあります。

関係 $\Delta '(T) =\overline{\varphi}_1$(Δ(T)) から、まず $d^2_{\lambda}=d^2_{\lambda'}$ 、従って $d_{\lambda}=d_{\lambda'}$ が推定され、次に数列 $(\omega '_1, . . . , \omega '_{d'_{\lambda'}})$ から集合の置換によって数列 $\varphi (\omega_1), . . . , \varphi (\omega_{d_{\lambda}})$ が推定できることがわかります。 添字。

これは G のすべての元 $g$ に当てはまるため、表現 $\lambda$ と $\lambda '$ は関連しています。従って、体 K が標数 0 を持つとき、命題 10 を証明しました。

B) 一般的なケース。

L を特性 0 の代数閉体とします (たとえば、$\mathbf{Q}$ の代数閉包)。単純な L[G] モジュールの $\mathscr{S}_L(G)$ 集合または類で表します。 選ぶ同型 $\eta$ 群 $\mu_n(L)$ から群 $\mu_n$(K)、集合 $\eta '=\varphi \circ \eta$。 証明の部分 A)までに、全単射が存在します

$$
\eta_G:\mathscr{S}_L(G)\rightarrow \mathscr{S}_K(G),\eta '_G:\mathscr{S}_L(G)\rightarrow \mathscr{S}_{K'}(G)
$$

次の性質: $\mathscr{S}_L$(G) のすべての $\lambda$ について、表現 $\lambda$ と $\eta_G(\lambda )$ は $\eta$ を介して関連付けられ、表現 $\lambda$ と $\eta '_G(\lambda )$ は $\eta '$ を介して関連付けられます。 全単射 $\varphi_G=\eta '_G\circ \eta_G^{-1}$ には望ましいプロパティがあります。

$\mathscr{I}_K(G)$ から $\mathscr{I}_{K'}(G)$ 拡大するから同型までの全単射 $\varphi_G$、グロタンディーク群 $R_K(G)$ から群 $R_{K'}(G)$ までの$\varphi_G$ とも表されます。

#### 注意 1 {#alg-viii-s21-n12-rem-1 .statement tag=00O2}

$K'$ が $K$ の拡大であり、同型 $\varphi$ が写像 $\xi \mapsto \xi \cdot 1$ であると仮定します。この場合、写像 $\varphi_G$ は、$K$ から $K'$ までのスカラーの拡大によって与えられます。

#### 系 1 {#alg-viii-s21-prop-10-cor-1 .statement tag=00O3}

※写像 $\varphi_G$は、$R_K(G)$から$R_{K'}(G)$までの環同型です。 $K$ ベクトル空間内の $G$ のすべての有限次元表現 $\pi$ に対して、$\varphi_G([\pi]) = [\pi']$ が得られます。ここで、$\pi'$ は $\pi$ から $\varphi$* に関連する表現です。

これは、$G$ の表現と VIII、p. 416 の性質 b) の半単純性から導き出されます。

#### 系 2 {#alg-viii-s21-prop-10-cor-2 .statement tag=00O4}

*それぞれの単純な次元 $G$ 割る位数 $G$* の表現。

これは、VIII、p. 415 の命題 10 と命題 9 に続きます。

#### 注意 2 {#alg-viii-s21-n12-rem-2 .statement tag=00O5}

群 $G$ が *アーベル* であるとします。 VIII、p. 414 の注意で、$\mathscr{I}_K(G)$ が集合 $\operatorname{Hom}(G, \mu_n(K))$ と識別できることが分かりました。同様に、$\mathscr{I}_{K'}(G)$ は $\operatorname{Hom}(G, \mu_n(K'))$ と識別できます。これらの識別により、全単射 $\varphi_G$ は単純に写像 $\chi \mapsto \varphi \circ \chi$ になります。

#### 注意 3 {#alg-viii-s21-n12-rem-3 .statement tag=00O6}

$\pi_1$と$\pi_2$を、$K$に対する有限次元ベクトル空間の$G$の線型表現とします。 $i = 1, 2$ について、$\pi_i'$ を $\pi_i$ から $\varphi$ に関連する表現とします。私たちは持っています
$$
\dim_K \operatorname{Hom}_K(\pi_1, \pi_2) = \dim_{K'} \operatorname{Hom}_{K'}(\pi_1', \pi_2') .
$$
証明は、系 VIII、p. 410 の後に、$\pi_i$ (従って $\pi_i'$) が単純な場合に還元されます。

#### 注意 4 {#alg-viii-s21-n12-rem-4 .statement tag=00O7}

$H$ を $G$ の基数 $m$ の部分群とします。 同型 $\varphi$ 制限するから同型 、$\mu_m(K)$ から $\mu_m(K')$ 、その結果、 環同型 $\varphi_H$ $R_K(H)$ から $R_{K'}(H)$ になります。次の図式の通勤:

$$
\begin{array}{ccc}
R_K(G) & \xrightarrow{\operatorname{Res}_H^G} & R_K(H) \\
\downarrow \varphi_G & & \downarrow \varphi_H \\
R_{K'}(G) & \xrightarrow{\operatorname{Res}_H^{G'}} & R_{K'}(H) ,
\end{array}
$$

$$
\begin{array}{ccc}
R_K(H) & \xrightarrow{\operatorname{Ind}_H^G} & R_K(G) \\
\downarrow \varphi_H & & \downarrow \varphi_G \\
R_{K'}(H) & \xrightarrow{\operatorname{Ind}_H^{G'}} & R_{K'}(G) .
\end{array}
$$

最初の図の可換性は明らかであり、2 番目の図の可換性は、フロベニウスの相反性と式 (47) を使用してそこから導き出されます。

#### 注意 5 {#alg-viii-s21-n12-rem-5 .statement tag=00O8}

G が 2 つの有限群の積 $G'\times G''$ であると仮定します。前回の例と同様に、定義する同型 $\varphi_{G'}$ と $\varphi_{G''}$ です。

可換図式があります

$R_K(G')\otimes_{\mathbf{Z}}R_K(G'')^{\kappa}$ // $R_K(G)$

$\varphi_{G'}\otimes \varphi_{G''}\varphi_G$

$R_{K'}(G')\otimes_{\mathbf{Z}}R_{K'}(G'')^{\kappa'}$ // $R_{K'}(G)$,

ここで、同型 $\kappa$ および $\kappa '$ は、VIII、p. 406 で定義されたものです。

### \*13.コンプレックス線型表現

この小節において、Kは複素数の体$\mathbf{C}$であると仮定します。

$(M, \pi )$ を G の線型表現とします。 次の場合、M 上のエルミート形 Φ は G の下で不変であると言います。

$$
\Phi (\pi (g)x, \pi (g)x') = \Phi (x, x') \tag{48}
$$

すべての $x, x'\in M$ とすべての $g\in G$ に対して。これは、M のすべての $g\in G$、自己同型 $\pi (g)$ が Φ に関してユニタリであることも意味します。

#### 命題 11 {#alg-viii-s21-prop-11 .statement tag=00O9}

$(M, \pi )$ を G の有限次元線型表現とします。

a) M エルミート形上に、G のもとで正で分離的かつ不変であるものが存在します。

b) 表現 $\pi$ が単純であると仮定します。 Φ と Ψ が G の下で不変である M 上の非零エルミート形である場合、$\Psi  =a\Phi$ となるような実数 $a$ が存在します。

選ぶベクトル空間 M 上の分離の正のエルミート形を$\Phi_0$ で表します。私たちは定義する設定により G の下で不変である分離正のエルミート形 Φ を定義します。

$$
\Phi (x, x') =\sum_{g\in G}\Phi_0(\pi (g)x, \pi (g)x') \tag{49}
$$

$x, x'\in M$の場合。

Ψ を M 上でエルミート形とします。 M の $x, x'$ に対して $\Psi (x, x') = \Phi (x,Ax')$ となるような M の一意な自己準同型 A が存在します。さらに、Ψ が G の下で不変であれば、自己準同型 A は $g\in G$ に対して自己同型 $\pi (g)$ と可換です。 表現 $\pi$ が単純な場合、シュールの補題 (VIII, p. 47, 定理 1) により、A はホモテティー となり、従って $\Psi  =a\Phi$ となる複素数 $a$ が存在します。 ΦとΨはエルミート、Φは非零なので、$a$は実数です。 命題が続きます。

G 上の複素数写像のベクトル空間 $\mathbf{C}[G]$ に、ヒルベルト空間構造を与え、その内部積は次のように与えられます。

$$
\langle f|f'\rangle_G=|G|^{-1}\sum_{g\in G}\overline{f(g)}f'(g) \tag{50}
$$

任意の写像 $f\in \mathbf{C}[G]$ について、次のように定義される $f^*$ 写像で表します。

$$
f^*(g) =\overline{f(g^{-1})} \tag{51}
$$

$g\in G$の場合; 写像 $f\mapsto f^*$ は、$\mathbf{C}[G]$ の半線形累積です。私たちも持っています

$$
\langle f|f'\rangle_G=\langle f^*, f'\rangle_G \tag{52}
$$

$f, f'\in \mathbf{C}[G]$、公式の記法 (28)、VIII、p. 410。従って、私たちは

$$
\langle f|f'\rangle_G=|G|^{-2}\tau (f^*f') \tag{53}
$$

$(M, \pi )$ を G の有限次元線型表現とします。ベクトル空間 M に、自己準同型 $\pi (g)$ が単一 (命題 11) であるヒルベルト空間の構造を与えます。この構造に対するMの自己準同型Aの随伴物を$A^*$で表すと、Tr($A^*$)$=$Tr(A)となります。 $g\in G$ ごとに $\pi (g^{-1}) =\pi (g)^*$ があり、従って $\chi_{\pi}(g^{-1}) =\chi_{\pi}(g)$ になります。他の語には$\chi_{\pi}=\chi^*_{\pi}$があります。 直交関係の指標 (VIII、p. 410、命題 4) は形になります

$$
\langle \chi_{\lambda}|\chi_\mu\rangle_G=\delta_{\lambda \mu} \tag{54}
$$

$\lambda , \mu\in \widehat{G}$の場合。これは、G の単純な表現の指標 $(\chi_{\lambda})_{\lambda\in\widehat{G}}$ の族が、中心写像のヒルベルト空間 $Z(\mathbf{C}[G])$ の正規直交基底であるという事実を表します。

$\pi$ と $\pi '$ を G の有限次元線型表現とします。 関係 $\langle \chi_{\pi}|\chi_{\pi'}\rangle_G=$ dim$_{\mathbf{C}}$ Hom$_G(\pi , \pi ')$ (VIII, p. 410, 系) があります。 表現 $\pi$ は、$\langle \chi_{\pi}|\chi_{\pi}\rangle_G= 1$ の場合にのみ既約です。

$\widehat{G}$ の元 $\lambda$ ごとに、ベクトル空間 $V_{\lambda}$ に、自己同型 $\pi_{\lambda}(g)$ が単一であるヒルベルト空間の構造を与えます。 2 つの元 $v, v'$ の $V_{\lambda}$ の $\langle v|v'\rangle_{\lambda}$ 内部積と $V_{\lambda}$ の自己準同型 $u$ の随伴物 $u^*$ で表します。 $A = (A_{\lambda})_{\lambda\in\widehat{G}}$と$A'= (A'_{\lambda})_{\lambda\in\widehat{G}}$を$F(\widehat{G})$の元とします。 $A^*= (A^*_{\lambda})_{\lambda\in\widehat{G}}$と書きます。 $\mathbf{C}[G]$ の元 $a$ ごとに $\mathscr{F}(a^*) = (\mathscr{F}(a))^*$ があります。 集合 (55) $\langle A|A'\rangle_{\widehat{G}}=|G|^{-2}\widehat{\tau}(A^*A')$。 VIII、p. 407の公式(10)までに、

(56) $\langle A|A'\rangle_{\widehat{G}}=\frac{1}{|G|^2}\sum_{\lambda\in\widehat{G}}d_{\lambda}$ Tr(A$^*_{\lambda}$A$'_{\lambda}$)。

$\widehat{\tau}\circ \mathscr{F}=\tau$ なので、公式 (53) と (55) は、写像 $\mathscr{F}$ が$\mathbf{C}[G]$ から$F(\widehat{G})$ までのヒルベルト空間の同型であることを意味します。

シュールの直交関係 (VIII、p. 410) は、ヒルバート式内部積を使用して再定式化できます。 関係 (21) と (24) から次の主張を与えます。 $V_{\lambda}$ の $\lambda \in \widehat{G}$ と $x, x', y, y'$ については、(57) $|G|^{-1}\sum_{g\in G}\overline{\langle x|\pi_{\lambda}(g)x'\rangle}_{\lambda}\langle y|\pi_{\lambda}(g)y'\rangle_{\lambda}=d^{-1}_{\lambda}\overline{\langle x|y\rangle}_{\lambda}\langle x'|y'\rangle_{\lambda}$ になります。

$\lambda$ と $\mu$ が $\widehat{G}$ の 2 つの異なる元である場合、$V_{\lambda}$ の $x, x'$ と $V_\mu$ の $y, y'$ について、(58) $\sum_{g\in G}\overline{\langle x|\pi_{\lambda}(g)x'\rangle}_{\lambda}\langle y|\pi_\mu(g)y'\rangle_\mu= 0$ が得られます。

$\lambda \in \widehat{G}$ ごとに、$V_{\lambda}$ の正規直交基底 $(e_{\lambda ,i})_{1\leqslant i\leqslant d_{\lambda}}$ を選ぶとします。 任意の $g\in G$ について、この基底に関して、自己準同型 $\pi_{\lambda}(g)$ $V_{\lambda}$ の $(\pi^{\lambda}_{ij}(g))$ 行列で表します。 (59) $\pi^{\lambda}_{ij}(g) =\langle e_{\lambda ,i}|\pi_{\lambda}(g)e_{\lambda ,j}\rangle_{\lambda}$ があります。

自己準同型 $\pi_{\lambda}(g)$ はユニタリであるため、その逆数は $\pi_{\lambda}(g)^*$ に等しいため、(60) $\overline{\pi^{\lambda}_{ij}(g)}=\pi^{\lambda}_{ji}(g^{-1})$ となります。次に、VIII、p. 409、および (25)、p. 409 の公式 (22) から、$\lambda \in \widehat{G},1\leqslant i\leqslant d_{\lambda},1\leqslant j\leqslant d_{\lambda}$、形のヒルベルト空間の正規直交基底に対して、写像 $(d_{\lambda})^{1/2}\pi_{ij}^{\lambda}$ が続きます。 $\mathbf{C}[G].*$

### 練習問題 {#alg-viii-s21-exercises}

[§ 21 に対して練習問題](exercises/s21/)を参照してください。

[^1]: The elements of Hom$_G(\pi , \pi ')$ are sometimes called intertwining operators of $\pi$ and $\pi '$.
